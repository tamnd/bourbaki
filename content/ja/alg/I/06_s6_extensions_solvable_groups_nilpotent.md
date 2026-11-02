---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 6
section_title: Extensions, solvable groups, nilpotent groups
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 65-81, 147-159
pdf_pages: 0089-0105, 0171-0183
extraction: ocr
subsections:
    - "no": 1
      title: EXTENSIONS
      page: 65
      pdf_page: 89
    - "no": 2
      title: COMMUTATORS
      page: 68
      pdf_page: 92
    - "no": 3
      title: LOWER CENTRAL SERIES, NILPOTENT GROUPS
      page: 71
      pdf_page: 95
    - "no": 4
      title: DERIVED SERIES, SOLVABLE GROUPS
      page: 74
      pdf_page: 98
    - "no": 5
      title: $p$-GROUPS
      page: 76
      pdf_page: 100
    - "no": 6
      title: SYLOW SUBGROUPS
      page: 78
      pdf_page: 102
    - "no": 7
      title: FINITE NILPOTENT GROUPS
      page: 80
      pdf_page: 104
statements: 58
exercises: 41
content_sha256: 328a0aa2b98bd5e68e75c3e48b19283a82b9afd1cb90b504ed0c4787066b398a
translated_from: content/en/alg/I/06_s6_extensions_solvable_groups_nilpotent.md
translation_method: google
source_content_sha256: d821e97942b895b17be8ce1e792e14c608c04537847a1c472436cfaf015e5b24
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: b57d4de8cce83434ea60262bd547ab54e7ea3cfcac86da7da52403392025b3cf
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 6。 拡大、可解群、無能群

この段落全体を通じて、群法則は、〜でない限りは、特に明記されていない限り、乗算的に書かれています。

### 1. 拡大

#### 定義 1 {#alg-i-s6-def-1 .statement tag=05CQ}

$F$ と $G$ を 2 つの群とします。 $G$の$F$による拡大はトリプル$\mathscr{E} = (E, i, p)$で、$E$は群、$F$の$i$単射準同型が$E$、$p$全射準同型になります。 $E$ を $G$ にすると、$\operatorname{Im}(i) = \operatorname{Ker}(p)$ になります。 準同型 $s : G \to E$ (それぞれ $r : E \to F$)、$p \circ s = \operatorname{Id}_G$ (それぞれ $r \circ i = \operatorname{Id}_F$) は、拡大 $\mathscr{E}$ の切断 (それぞれ後退) と呼ばれます。

$G$ の $F$ の拡大 $\mathscr{E} = (E, i, p)$ は、図式 $\mathscr{E} : F \xrightarrow{i} E \xrightarrow{p} G$ で表されることが多く、混乱が生じない限り、$i$ と $p$ はときどきが省略されます。 $F$による$G$の拡大が群$E$であると簡単に言うとときどきです。

群 $E$ が $F$ によって $G$ の拡大になるためには、 剰余群が成り立つような含む部分群 $F'$ が $F$ と同型であることが必要かつ十分です。 $E/F'$ は $G$ と同型です。

像 $i(F)$ が $E$ の中心に含まれる場合、拡大 $\mathscr{E} : F \xrightarrow{i} E \xrightarrow{p} G$ は中央と呼ばれます。これは、$F$ が可換である場合にのみ可能です。

$\mathscr{E} : F \xrightarrow{i} E \xrightarrow{p} G$と$\mathscr{E}' : F \xrightarrow{i'} E' \xrightarrow{p'} G$を、$G$×$F$の2つの拡大とします。 $\mathscr{E}$ の $\mathscr{E}'$ への射は、$p' \circ u = p$ と $u \circ i = i'$ となるように準同型 $u : E \to E'$ になります。または、他の語では、次の図式が可換です。

$$
\begin{array}{ccc}
& & E \\
& i & \\
F & \xrightarrow{i'} & E' \\
& \downarrow & \downarrow \\
& & E \\
& p & \\
& & G
\end{array}
$$

$$
u \uparrow \quad \text{and} \quad p' \uparrow
$$

#### 命題 1 {#alg-i-s6-prop-1 .statement tag=05CR}

$\mathscr{E}: F \xrightarrow{i} E \xrightarrow{p} G$と$\mathscr{E}': F \xrightarrow{i'} E' \xrightarrow{p'} G$を$G$の$F$による拡大とします。 $u: E \to E'$が$\mathscr{E}$の射から$\mathscr{E}'$になる場合、$u$は$E$の同型から$E'$になり、$u^{-1}$は$\mathscr{E}'$の射から$\mathscr{E}$になります。

$x \in E$ を $u(x) = e$ となるようにします。次に、$p(x) = p'(u(x)) = e$、よって、$x \in i(F)$。 $y \in F$ を $x = i(y)$ となるようにします。次に$i'(y) = u(i(y)) = e$。 $i'$は単射なので、$y = e$と$x = e$。したがって、$u$ は単射法です。 § 4, no. 6、系 1 ～ 命題 7 により、$u(i(F)) = i'(F)$ から $u$ は全射になります。 最後の主張は明らかです。

他の語、拡大、$\mathscr{E}$、$\mathscr{E}'$ は、$\mathscr{E}$ の射が $\mathscr{E}'$ に存在する場合にのみ *同型* になります。

$F$ と $G$ を 2 つの群として、$E_0 = F \times G$ と書きます。 $i: F \to E_0$を標準単射、$p: E_0 \to G$を正規の射影とします。 拡大 $\mathscr{E}_0: F \xrightarrow{i} E_0 \xrightarrow{p} G$ と同型の $F$ による $G$ のすべての拡大は *自明な拡大* と呼ばれます。

#### 命題 2 {#alg-i-s6-prop-2 .statement tag=05CS}

*$\mathscr{E}: F \xrightarrow{i} E \xrightarrow{p} G$を$G$の$F$による拡大とします。次の条件は同等です*:

(i) $\mathscr{E}$ は自明な拡大です。
(ii) $\mathscr{E}$ にはリトラクション $r$ があります。
(iii) $\mathscr{E}$ には切断 $s$ があり、$s(G)$ が $i(F)$ のセントラライザーに含まれるようになります。

明らかに (i) は (ii) と (iii) を意味します。 (ii) が成り立つ場合、写像 $(r, p): E \to F \times G$ は、$\mathscr{E}$ の射を$\mathscr{E}_0$、よって (i) に変換します。 (iii) が成立する場合、$F \times G$ の $E$ 対応するから $(i, s)$ への準同型 ($\S$ 4、no. 9、命題 12) は、$\mathscr{E}_0$ の $\mathscr{E}$ への射、 よって (i)。

拡大 $\mathscr{E}: F \to E \to G$ は自明ではないが、群 $E$ は $F \times G$ (練習問題 6) と同型である可能性があります。

#### 定義 2 {#alg-i-s6-def-2 .statement tag=05CT}

*$F$と$G$を$G$の群と$\tau$準同型を$F$の自己同型群にします。 $g \in G$と$f \in F$には$\tau(g)(f) = gf$と書きます。 集合 $F \times G$ と法則の合成*

$$
((f, g), (f', g')) \mapsto (f, g) \cdot_{\tau} (f', g') = (f \cdot gf', gg')
$$

*は、$\tau$を基準とした$F$による$G$の外部半直接積と呼ばれます。

$\tau$ を基準とした $F$ による $G$ の外部半直接積は、$F \times_{\tau} G$ で示されます。

#### 命題 3 {#alg-i-s6-prop-3 .statement tag=05CU}

※外部セミダイレクト積$F \times_{\tau} G$は群となります。 $i(f) = (f, e)$ によって定義される写像 $i: F \to F \times_{\tau} G$、$p(f, g) = g$ によって定義される$p: F \times_{\tau} G \to G$、および$s(g) = (e, g)$ によって定義される$s: G \to F \times_{\tau} G$ は、群準同型です。トリプル $(F \times_{\tau} G, i, p)$ は $G$ の $F$ の拡大であり、$s$ は拡大の切断です。*

私たちは以下のものを持っています:

$$
((f, g) \cdot_{\tau} (f', g')) \cdot_{\tau} (f'', g'') = (f.gf', gg') \cdot_{\tau} (f'', g'')
= (f.gf'.gg'f'', gg'g'');
$$
$$
(f, g) \cdot_{\tau} ((f', g') \cdot_{\tau} (f'', g'')) = (f, g) \cdot_{\tau} (f'g'f'', g'g'')
= (f.g(f'.g'f''), gg'g'').
$$

さて$g(f'.g'f'') = gf'.gg'f''$は、(1)で定義された合成の法則が結合していることを示しています。 元 $(e, e)$ は、この法則のアイデンティティです。 元 $(f, g)$ は逆数 $(g^{-1}f^{-1}, g^{-1})$ として認められます。したがって、$F \times_{\tau} G$の合成の法則は群法則です。残りの主張は明らかです。

命題 3 の記法を使用すると、$\mathscr{E}_{\tau}$ は拡大を表します

$$
F \xrightarrow{i} F \times_{\tau} G \xrightarrow{p} G.
$$

$\mathscr{E}' : F \xrightarrow{i'} E' \xrightarrow{p'} G$ を $F$ により $G$ の拡大とし、$\mathscr{E}'$ の $s' : G \to E'$ 切断とします。私たちは群 $F$ に定義する演算 $\tau$/$G$ でした:

(2)
$$
i'(\tau(g, f)) = s'(g)i'(f)s'(g)^{-1} = \operatorname{Int}(s'(g))(i'(f)).
$$

#### 命題 4 {#alg-i-s6-prop-4 .statement tag=05CV}

※上記記法では、$u \circ s = s'$となる$\mathscr{E}'$上に$\mathscr{E}_{\tau}$の同型uが一つだけ存在します。

$$(f, g) = (f, e) \cdot_{\tau} (e, g) = i(f) \cdot_{\tau} s(g).$$ したがって、$u$が解から問題であれば、必然的に$u(f, g) = i'(f).s'(g)$、$u$のよって一意性になります。私たちは存在を証明します。 $u(f, g) = i'(f).s'(g)$と書きます。それから

$$
\begin{align*}
u(f, g).u(f', g') &= i'(f)s'(g)i'(f')s'(g') \\
&= i'(f)(s'(g)i'(f')s'(g)^{-1})s'(g)s'(g') \\
&= i'(f)i'(\tau(g, f')).s'(g)s'(g') \\
&= i'(f.\tau(g, f')).s'(gg') \\
&= u((f, g) \cdot_{\tau} (f', g')).
\end{align*}
$$

したがって、$u$は$F \times_{\tau} G$の$E'$の準同型です。明らかに、$u \circ i = i'$、$p' \circ u = p$、$u \circ s = s'$です。

#### 注意 {#alg-i-s6-n1-rem-1 .statement tag=05CW}

公式による演算 $\tau$ の定義 (2) は、拡大 $\mathscr{E}'$ と切断 $s'$ に依存します。 $F$ が可換である場合、演算 $\tau$ は $s'$ に依存しません。 $\operatorname{Int}(s'(g)) | i'(F)$ の場合、$s'(g)$ mod の剰余類のみに依存します。 $i'(F)$。

より一般的には、$\mathscr{E} : F \to E \to G$ を可換群 $F$ により $G$ の拡大とします ($\mathscr{E}$ が切断を認めるとは想定されていません)。 群 $E$ は内部自己同型によって $F$ に作用しますが、この像は $F$ の像では自明であり、したがって $F$ では $G$ の定義する演算になります。 $\mathscr{E}$ が切断を認める場合、この演算は公式 (2) によって定義されるものになります。

#### 系 {#alg-i-s6-n1-cor-1 .statement tag=05CX}

*$G$を群と$H$と$K$として、$G$の2つの部分群を加えて、$H$が正常、$H \cap K = \{e\}$と$H.K = G$とします。 $\tau$を$H$の$G$の内部自己同型による$K$の演算とします。 写像 $(h, k) \mapsto hk$ は、$H \times_{\tau} K$ の $G$ 上の同型です。

この系の仮説のもとでは、$G$は$H$による$K$の半直接的な積であると言われています。

#### 例 {#alg-i-s6-n1-exa-1 .statement tag=05CY}

(1) Let $G$ be a group and $E$ a homogeneous principal $G$-set; let $\Gamma$ denote the automorphism group of $G$. Let $A$ be the set of permutations $f$ of $E$ with the following property:
There exists $\gamma \in \Gamma$ such that $f$ is a $\gamma$-morphism of $E$ into $E$ (that is, $f(gb) = \gamma(g)f(b)$ for $b \in E$ and $g \in G$).
The above formula $f(gb) = \gamma(g)f(b)$ shows that if $f \in A$ there exists a unique $\gamma \in \Gamma$ such that $f$ is a $\gamma$-morphism, we shall denote it by $p(f)$.
Let $f, f'$ be in $A$, $\gamma = p(f), \gamma' = p(f')$. 次に、すべての $b \in E$ とすべての $g \in G$ について、
$$
(f' \circ f)(gb) = f'(\gamma(g)f(b)) = \gamma'(\gamma(g))f'(f(b))
$$
これは、$f' \circ f \in A$ と $p(f' \circ f) = p(f')p(f)$ を証明します。 一方、$f(\gamma^{-1}(g)f^{-1}(b)) = gb$、よって、$f^{-1}(gb) = \gamma^{-1}(g)f^{-1}(b)$、$f^{-1} \in A$。 したがって、$A$ は $\mathscr{S}_E$ の部分群であり、$p$ は $A$ の $\Gamma$ である準同型です。 $p$の核は、$G$セット$E$の自己同型の集合$\mathrm{Aut}_G(E)$です。
$a \in E$を修正します。 We have defined in § 5, no. 6 an isomorphism $\psi_a$ of $G^0$ onto $\mathrm{Aut}_G(E)$ such that $\psi_a(x)(ga) = gxa$ for all $g, x$ in $G$. 一方、$\gamma \in \Gamma$ については、$s_a(\gamma)$ をすべての $g \in G$ について $s_a(\gamma)(ga) = \gamma(g)a$ によって定義される $E$ の置換とします。 $s_a$ が $\Gamma$ の準同型から $A$ になり、$p \circ s_a = \mathrm{Id}_{\tau}$ になることがすぐに検証されます。 したがって、$G^0 \xrightarrow{\psi_a} A \xrightarrow{p} \Gamma$は$\Gamma$の$G^0$による拡大であり、$s_a$はこの拡大の切断です。 This extension and this section define an operation of $\Gamma$ on $G^0$, $s_a(\Gamma)$ acting on $\psi_a(G^0)$ by inner automorphisms; we write this operation exponentially. この演算が自然な演算 ($§ 3$, no. 1, 例 3) であることを示します: $G$ と $\gamma \in \Gamma$ の $x, g$ について、
$$
(\psi_a(\gamma x))(ga) = (s_a(\gamma) \circ \psi_a(x) \circ s_a(\gamma)^{-1})(ga)
= (s_a(\gamma) \circ \psi_a(x))(\gamma^{-1}(g)a) = s_a(\gamma)(\gamma^{-1}(g)xa)
= g\gamma(x)a = \psi_a(\gamma(x))ga
$$
よって $^\gamma x = \gamma(x)$。
次に、命題 4 は、$G^0$ 上の$\mathrm{Aut}(G)$ の自然な演算の下で、$G^0$ によって $A$ が $\Gamma = \mathrm{Aut}(G)$ の半直積と同型であることを示します。 私たちが構築した同型は、一般に元 $a \in E$ の選択に依存することに注意してください。
(2) ※$A$を可換環とします。 上三角形群 $T(n, A)$ は、上厳密三角形群 $T_1(n, A)$ による対角線部分群 $D(n, A)$ の半直接積です。*

### 2. 交換子

#### 定義 3 {#alg-i-s6-def-3 .statement tag=05CZ}

$G$ を群と $x$ と $y$ 2 つの $G$ の元とします。 $G$の元$x^{-1}y^{-1}xy$は、$x$と$y$の交換子と呼ばれます。

(x, y) は、x と y の交換子を表すために使用されます。それから明らかに
$$(y, x) = (x, y)^{-1}.$$
x と y が通勤するには、$(x, y) = e$ であることが必要十分です。より一般的には、
$$xy = yx(x, y).$$
一方、私たちはこう書きます
(3)
$$x^y = y^{-1}xy = x(x, y) = (y, x^{-1})x.$$
写像 $x \mapsto x^y$ は内部自己同型 $\operatorname{Int}(y^{-1})$ であるため、すべての $x, y, z \in G$ に対して $(x, y)^z = (x^z, y^z)$ となります。

$x, y, z \in G$ については、次の関係を証明します。
(4)
$$(x, yz) = (x, z).(x, y)^z = (x, z).(z, (y, x)).(x, y)$$
(4ビス)
$$(xy, z) = (x, z)^y.(y, z) = (x, z).((x, z), y).(y, z)$$
(5)
$$(x^y, (y, z)).(y^z, (z, y)).(z^x, (x, y)) = e$$
(6)
$$(x, yz).(z, xy).(y, zx) = e$$
(6ビス)
$$(xy, z).(yz, x).(zx, y) = e.$$

今
$$
\begin{align*}
(x, yz) &= x^{-1}z^{-1}y^{-1}xyz = (x, z)z^{-1}x^{-1}y^{-1}xyz = (x, z)(x, y)^z \\
&= (x, z)(z, (x, y)^{-1})(x, y)
\end{align*}
$$
(3) により (4) が証明されます。 公式 (4 ビス) も同様に続きます。一方、
$$
\begin{align*}
(x^y, (y, z)) &= (x^y)^{-1}(z, y)(x^y)(y, z) \\
&= y^{-1}x^{-1}yz^{-1}y^{-1}zyy^{-1}xyy^{-1}z^{-1}yz \\
&= (yzy^{-1}xy)^{-1}(zxz^{-1}yz).
\end{align*}
$$
次に、$u = yzy^{-1}xy, v = zxz^{-1}xy$ と $w = xyx^{-1}zx$ を書くと、次のようになります。
$$(x^y, (y, z)) = u^{-1}v.$$
$x, y, z$ を巡回置換することで、$(y^z, (z, x)) = v^{-1}w$ を導き出し、
$$(z^x, (x, y)) = w^{-1}u,$$
これは直ちに (5) を意味します。最後に、(6) は、公式 $(x, yz) = x^{-1}z^{-1}y^{-1}xyz = (yzx)^{-1}(xyz)$ で $x, y, z$ を巡回置換することで得られる 3 つの公式の 2 つの辺を乗算することによって続きます。(6 の 2 ) についても同様です。

A と B が G の 2 つの部分群である場合、(A, B) は、$a \in A$ と $b \in B$ を含む交換子 $(a, b)$ によって生成された部分群を表します。† 次に、A が B を集中化する場合に限り、$(A, B) = \{e\}$ になります。 B が A を正規化する場合に限り、$(A, B) \subset A$ になります。 A と B が正規の場合(それぞれの特性)、$(A, B)$も同様です。

† ここでは、合成の法則を部分集合に拡張する § 1 で行われた表記規則を拒否します。

#### 命題 5 {#alg-i-s6-prop-5 .statement tag=05D0}

$A, B, C$を$G$の3つの部分群とします。

(i) 部分群 $A$ は部分群 $(A, B)$ を正規化します。

(ii) 部分群 $(B, C)$ が $A$ を正規化すると、元 $(a, (b, c))$ と $a \in A, b \in B$ と $c \in C$ によって部分群 $(A, (B, C))$ が生成されます。

(iii) $A, B$ と $C$ が正常であれば、

$$
(A, (B, C)) \subset (C, (B, A)).(B, (C, A)).
$$

(4 ビス) により、$a, a' \in A$ と $b \in B$ の場合、

$$
(a, b)^{a'} = (aa', b).(a', b)^{-1},
$$

よって (i)。ここで、$(B, C)$ が $A$ を正規化するとします。 $a \in A, b \in B, c \in C$ と $x \in G$ の場合、(4) は次のことを意味します。

$$
(a, (b, c).x) = (a, x).(x, ((b, c), a))(a, (b, c))
$$

そして、$(B, C)$は、$p$の帰納法によって$A$、よってを正規化するため、$((b, c), a) \in A$は、$b_i \in B, c_i \in C$、属するから部分群の元によって$\left( a, \prod_{i=1}^p (b_i, c_i) \right)$が生成されるという事実形 $(a, (b, c))$。最終的に$A, B$と$C$が正常であれば、部分群、$(A, (B, C))$、$(C, (B, A))$、$(B, (C, A))$も正常です。したがって、(ii) によって次のことが示されれば十分です。

$$
(a, (b, c)) \in (C, (B, A)).(B, (C, A))
$$

すべての $a \in A, b \in B$ と $c \in C$ に対して。 (5) までに $a^{b^{-1}} = u$ を書きます

$$
(a, (b, c)) = ((u^b), (b, c)) = (c^u, (u, b))^{-1}.(b^c, (c, u))^{-1},
$$

よって (iii)。

#### 定義 4 {#alg-i-s6-def-4 .statement tag=05D1}

$G$を群とします。 $G$の元の交換子によって生成された部分群は、$G$の導来群と呼ばれます。

したがって、$G$ の導来群は部分群 $(G, G)$ になります。 $D(G)$ とも表されます。 言葉の乱用により、それは $G$ の *交換子群* と呼ばれるときどきですが、一般に $G$ (練習問題 16) の交換子の元の集合とは区別されます。 $D(G) = \{e\}$ は、$G$ が可換である場合に限ります。

#### 命題 6 {#alg-i-s6-prop-6 .statement tag=05D2}

$f : G \to G'$を群準同型とします。 次に$f(D(G)) \subset D(G')$。 If $f$ is surjective, the homomorphism of $D(G)$ into $D(G')$ the restriction of $f$ is surjective.

$G$の元の交換子の$f$の下の像は、$G'$の元の交換子です。 $f$が全射であれば、$G$の交換子の集合の$f$の下の像は、$G'$の交換子の集合になります。したがって、命題は、§ 4, no. 3、系 3 から命題 2 に続きます。

#### 系 1 {#alg-i-s6-prop-6-cor-1 .statement tag=05D3}

群 $G$ の導来群は、$G$ の特性部分群です。特に$G$の通常の部分群です。

#### 系 2 {#alg-i-s6-prop-6-cor-2 .statement tag=05D4}

G を群とします。 剰余群 G/D(G) は可換です。 $\pi : G \to G/D(G)$ を標準準同型とします。可換群 G' への G のすべての準同型 f は、形 $f = \bar{f} \circ \pi$ で一意に表現できます。ここで、$\bar{f} : G/D(G) \to G'$ は準同型です。

現在$\pi(D(G)) = \{e\}$。 $\pi$は全射なので、$D(G/D(G)) = \{e\}$、よって、最初の主張ということになります。 2 番目は、§ 4, no. 4、命題 5 に続きます。

#### 系 3 {#alg-i-s6-prop-6-cor-3 .statement tag=05D5}

H を G の部分群とします。次の条件は同等です。

(i) $H \supset D(G)$;
(ii) H は通常の部分群であり、$G/H$ は可換です。
(ii) $\Rightarrow$ (i) 系 2 および (i) $\Rightarrow$ (ii) § 4, no. 7、定理 4、可換群のすべての部分群は正規であるため。

#### 系 4 {#alg-i-s6-prop-6-cor-4 .statement tag=05D6}

G を生成する G である G の群と X 部分集合とします。 群 D(G) は、X の元の交換子によって生成される G の正規の部分群です。

Let H be the normal subgroup of G generated by the commutators of elements of X and $\phi : G \to G/H$ the canonical homomorphism. 集合 $\phi(X)$ 生成する $G/H$。 The elements of $\phi(X)$ are pairwise permutable and hence H is commutative (§ 4, no. 3, Corollary 2 to Proposition 2). したがって、(系 3) H 含む D(G) となります。 一方、明らかに$H \subset D(G)$。

#### 注意 {#alg-i-s6-n2-rem-1 .statement tag=05D7}

(1) 系 2 は、$G/D(G)$ が$\pi$ とともに、G から可換群までの可換群および準同型に対して、G に対する普遍写像問題の解であることをというによって表すこともできます。

(2) 系 4 の仮説の下では、X の元の交換子によって生成される部分群は D(G) に含まれますが、一般に D(G) と等しくありません (cf. 練習問題 15e)。

#### 例 {#alg-i-s6-n2-exa-1 .statement tag=05D8}

(1) G が非可換単純群の場合、$D(G) = G$。したがって、G の可換群へのすべての準同型は自明です。

(2) 対称群 $S_n$ の導来群は交代的群 $A_n$ です。 $A_n$ は 2 つの転置の積によって生成されます。 $\tau = \tau_{x,y}$ と $\tau' = \tau_{x',y'}$ が 2 つの転置である場合、$\sigma$ は $\sigma(x') = x$ と $\sigma(y') = y$ となるように置換とします。すると$\tau' = \sigma^{-1} \tau \sigma$と$\tau \tau' = \tau^{-1} \tau' = \tau^{-1} \sigma^{-1} \tau \sigma$は交換子になります。したがって$A_n \subset D(S_n)$です。 $S_n/A_n$ は可換なので、$A_n \supset D(S_n)$ (系 3)。

### 3. 中央下部系列、無能群

Gを群、HをGの部分群、KをGの通常の部分群とします。G/KのHの像は、$(G, H) \subset K$の場合に限り、G/Kの中心に含まれます。

#### 定義 5 {#alg-i-s6-def-5 .statement tag=05D9}

Gを群とします。 G の下中央系列は、帰納的に次のように定義される G の部分群の数列 $(C^n(G))_{n \geq 1}$ です。
$$
C^1(G) = G, \quad C^{n+1}(G) = (G, C^n(G)).
$$

$f : G \to G'$を群準同型とします。 $n$ の帰納法によって、$f(C^n(G)) \subset C^n(G')$ がわかり、$f$ が全射であれば $f(C^n(G)) = C^n(G')$ になることがわかります。特に、すべての $n \geq 1$ にとって、$C^2(G)$ は $G$ の特性 (したがって正常) 部分群です。すべての$n \geq 1$に対して、$C^n(G)/C^{n+1}(G)$は$G/C^{n+1}(G)$の中心に含まれます。

$(G_1, G_2, \ldots)$ を、(1) $G_1 = G$ となるような $G$ の通常の部分群の減少列とします。 (2) 全ての$i$、$G_i/G_{i+1}$は$G/G_{i+1}$の中心に含まれます。次に、$i$ の帰納法に見られるように、$C^i(G) \subset G_i$ です。

今
$$
(C^m(G), C^n(G)) \subset C^{m+n}(G).
$$
なぜなら、この関係が $(F_{m,n})$ で表される場合、$(F_{m,n})$ から no. 2、命題 5 によって、
$$
\begin{align*}
(C^m(G), C^{n+1}(G)) &\subset (G, (C^m(G), C^n(G))).(C^n(G), (G, C^m(G))) \\
&\subset C^{m+n+1}(G).(C^{m+1}(G), C^n(G)).
\end{align*}
$$
したがって$((F_{m,n}) \text{ and } (F_{m+1,n})) \Rightarrow (F_{m,n+1})$です。 $(F_{m,1})$ と $(F_{1,n})$ は明らかなので、$(F_{m,n})$ の後には帰納法が続きます。

#### 定義 6 {#alg-i-s6-def-6 .statement tag=05DA}

*$C^{n+1}(G) = \{e\}$ となるような整数 $n$ が存在する場合、群 $G$ は nilpotent と呼ばれます。 $C^{n+1}(G) = \{e\}$ がゼロポテント群 $G$ のゼロポテンシー 類となるような最小の整数 $n$ を、ゼロポテンシー 類と呼びます。

$n \in \mathbf{N}$ の場合、類 $n$ の群は、類 $n$ のゼロ力群と呼ばれます。 ときどきは、$G$ がゼロポテンシャルである場合、群 $G$ のゼロポテンシー 類が有限であると言われています。

#### 例 {#alg-i-s6-n3-exa-1 .statement tag=05DB}

(1) 群は、単位元 (それぞれ可換である) で構成されている場合に限り、類 0 (それぞれ $\leq 1$) の零能です。

(2) *すべての可換環 $A$ とすべての整数 $n \geq 1$ について、上側の厳密な三角形群 $T_1(n, A)$ は類 $\leq n - 1$ に対してゼロポテントです (そして、$A \neq \{0\}$ の場合は正確に類 $n - 1$ もゼロポテントです)。

(3) $G$ を類 $n$ のゼロポテント群とします。 $G$ のすべての部分群 (それぞれ剰余群ごと) は、類 $\leq n$ の無力です。なぜなら、$H$が$G$の部分群であれば、$C^n(H) \subset C^n(G)$です。 $G'$ が $G$ の剰余群で、$\pi : G \to G'$ が標準準同型の場合、$C^n(G') = \pi(C^n(G))$ です。

(4) 零能群の有限積は零能である。

#### 命題 7 {#alg-i-s6-prop-7 .statement tag=05DC}

*$G$を群と$n$整数とします。次の条件は同等です:*

(a) $G$ は類 $\leq n$ の無能です。
(b) *$G$ の部分群の系列が存在します:*
$$
G = G^1 \supset G^2 \supset \ldots \supset G^{n+1} = \{e\}
$$
*そのような* $(G, G^{k'}) \subset G^{k'+1}$ *すべてに* $k \in \{1, n\}$。

(c) $G$の中心に含まれる$G$の部分群$A$が存在し、$G/A$は類$\leq n - 1$の零である。

(a) $\Rightarrow$ (b): $G^k = C^k(G)$ を取れば十分です。
(b) $\Rightarrow$ (a): $k$、$C^k(G) \subset G^k$ の帰納法まで。
(a) $\Rightarrow$ (c): $A = C^n(G)$ を取れば十分です。
(c) $\Rightarrow$ (a): $\pi : G \to G/A$ を標準準同型とする。次に $\pi(C^n(G)) = C^n(G/A) = \{e\}$、したがって $C^n(G) \subset A$、よって $C^{n+1}(G) = \{e\}$ となります。

もっと簡単に言うと、$n$ の連続する中央拡大によって群 $\{e\}$ から群が得られる場合、類 $\leq n$ の無能です。

#### 系 {#alg-i-s6-n3-cor-1 .statement tag=05DD}

*ゼロポテント群 (必ず可換な群による) の中心拡大はゼロポテントです。*

#### 命題 8 {#alg-i-s6-prop-8 .statement tag=05DE}

*$G$ を類 $\leq n$ のゼロポテント群とし、$H$ を $G$ の部分群とします。 部分群* のうち数列が存在します

$$
G = H^1 \supset H^2 \supset \ldots \supset H^{n+1} = H,
$$

*$H^{k+1}$ は $H^k$ で正規であり、$H^k/H^{k+1}$ はすべての $k \leq n$ に対して可換です。*

選ぶ数列 $(G^k)$ の部分群の $G$ 満たす条件の命題 7 (b) すべての $k$; $G$では$G^k$が正常です。書く：

$$
H^k = H.G^k.
$$

$H^{k+1}$ が $H^k = H.G^k$ で正規化されていることを確認する必要があります。 $H$ によって正規化されているため、$G^k$ によって正規化されていることを確認するだけで十分です。さて、$s \in G^k$ と $h \in H$ の場合、

$$
shs^{-1} = shs^{-1}h^{-1}.h \in (G, G^k).H
$$

$(G, G^k).H$ は $G^{k+1}.H = H^{k+1}$ に含まれます。したがって、$s.H^{k+1}.s^{-1} = H^{k+1}$ は、$H^k$ では $H^{k+1}$ が正常であることを示しています。

最後に、標準準同型 $G^k/G^{k+1} \to H^k/H^{k+1}$ は明らかに全射です。最初の群は可換であるため、2 番目も可換です。

#### 系 1 {#alg-i-s6-prop-8-cor-1 .statement tag=05DF}

*$G$ をゼロポテント群および $G$ の $H$ 部分群とします。 $H$ が $G$ と異なる場合、$G$ の $H$ のノーマライザー $N_G(H)$ は $H$ とは異なります。*

$k$ を最大の添字として、$H^k \neq H$ とします。 群 $H^k$ は $H$ を正規化し、$H$ とは区別されます。

#### 系 2 {#alg-i-s6-prop-8-cor-2 .statement tag=05DG}

*$G$ をゼロポテント群および $G$ の $H$ 部分群とします。 $H$ が $G$ と異なる場合、$G$ とは異なり、$G/N$ が可換であるような、$G$、含む $H$ の通常の部分群 $N$ が存在します。

$k$ を $H^k \neq G$ となる最小の添字とします。 群 $H^k$ は、必要な条件を満たします。

#### 系 3 {#alg-i-s6-prop-8-cor-3 .statement tag=05DH}

*G を G の冪能群および H 部分群とします。G = H.(G, G) の場合、G = H.*

含む H である G のすべての部分群 N、および G/N が可換であるような含む H.(G, G)。したがって、系 3 は系 2 から続きます。

系 3 は次のように定式化することもできます: X を G の部分集合とします。 X から生成する G については、G/D(G) 生成する G/D(G) の X の像が必要かつ十分です。

#### 系 4 {#alg-i-s6-prop-8-cor-4 .statement tag=05DI}

※f:G'→Gを群準同型とします。次のように仮定します*
(a) *G はゼロポテントです。*
(b) *準同型 f₁: G'/(G', G') → G/(G, G)、f から移行から商まで導出され、全射法です。*
*その場合、f は全射です。*

これは、系 3 を部分群 H = f(G') に適用した結果となります。

#### 命題 9 {#alg-i-s6-prop-9 .statement tag=05DJ}

*G を類 ≤ n の零能群とし、N を G の通常の部分群とします。 部分群の系列が存在します*

$$
N = N^1 \supset N^2 \supset \ldots \supset N^{n+1} = \{e\}
$$

*そのような* (G, N^k) ⊂ N^{k+1} *k = 1, ..., nの場合*

(G^k) が命題 7 の条件 (b) を満たす場合、

$$
N^k = G^k \cap N.
$$

#### 系 1 {#alg-i-s6-prop-9-cor-1 .statement tag=05DK}

*G をゼロポテント群、Z 中心 、N を G の正規部分群とします。N ≠ {e} の場合、N ∩ Z ≠ {e} となります。*

k を最大の添字とし、N^k ≠ {e} とします。 群 N^k は N に含まれます。一方、 (G, N^k) ⊂ N^{k+1} = {e};したがって、N^k は G の中心 Z に含まれます。

#### 系 2 {#alg-i-s6-prop-9-cor-2 .statement tag=05DL}

* f をゼロポテント群 G から群 G' までの準同型とします。 f の制限から G の中心が単射である場合、f は単射です。*

これは、Ker(f) に適用される系 1 です。

### 4. 導出系列、解決可能群

#### 定義 7 {#alg-i-s6-def-7 .statement tag=05DM}

※Gを群とします。 G の導出された系列は、次のように帰納的に定義される系列 (D^n(G))_{n \in \mathbf{N}} です。

$$
D^0(G) = G; \quad D^{n+1}(G) = D(D^n(G)) \quad \text{for } n \in \mathbf{N}.
$$

続いて$D^0(G) = C^1(G) = G,\ D^1(G) = C^2(G) = D(G) = (G, G)$。 \mathbf{N} のすべての n に対して、D^n(G) \部分集合 C^{2^n}(G) は、no. 3 の公式 (7) を使用した n の帰納法でわかります。

$f : G \to G'$を群準同型とします。 n 上の帰納法によって、$f(D^n(G)) \subset D^n(G')$ がわかり、$f$ が全射であれば $f(D^n(G)) = D^n(G')$ になることがわかります。特に、すべての $n \in \mathbf{N}$ について、$D^n(G)$ は G の特性 (したがって正規) 部分群です。すべての $n \in \mathbf{N}$ について、群 $D^n(G)/D^{n+1}(G)$ は、$G/D^{n+1}(G)$ の可換正規 (ただし一般に中心ではありません) 部分群です。

$(G_0, G_1, \ldots)$ を次のような G の部分群の減少列とします: (1) $G_0 = G$; (2) すべての $i$、$G_{i+1}$ は $G_i$ で正規であり、$G_i/G_{i+1}$ は可換です。次に、$i$ の帰納法に見られるように、すべての $i$ に対して $D^i(G) \subset G_i$ です。

#### 定義 8 {#alg-i-s6-def-8 .statement tag=05DN}

*$D^n(G) = \{e\}$ となるような整数 n が存在する場合、*群 G は可解と呼ばれます。 G が可溶性群の場合、$D^n(G) = \{e\}$ となる最小の整数 n を G の可溶性類と呼びます。*

可解性類 $n$ の可溶性群は、 類 $n$ の可溶性群と呼ばれます。 群はときどきが有限の可溶性であると言われており、可溶であれば類です。

#### 例 {#alg-i-s6-n4-exa-1 .statement tag=05DO}

(1) 群は、$\{e\}$ (可換である) に還元される場合に限り、類 0 (それぞれ $\leq 1$) から解けます。

(2) 類 $\leq 2^n - 1$ のすべての nilpotent 群は類 $\leq n$ で解けます。これは、上で証明された関係 $D^n(G) \subset C^{2^n}(G)$ から導き出されます。

(3) G を類 $\leq n$ の可解な群とする。 G のすべての部分群 (それぞれ剰余群) は、類 $\leq n$ で解けます (証明は、no. 3、例 3 のそれに類似しています)。

(4) G が類 $p$ の可溶群で、F が類 $q$ の可溶群である場合、F による G のすべての拡大 E は、類の可溶群です。 $\leq p + q$。というのは、$\pi : E \to G$ を射影とします。その場合は $\pi(D^p(E)) \subset D^p(G) = \{e\}$ となり、したがって $D^p(E) \subset F$ となります。 $D^{p+q}(E) = D^q(D^p(E)) \subset D^q(F) = \{e\}$ ということになります。

(5) 対称群 $S_n$ は、$n < 5$ (cf. § 5、練習問題 10 と 16) の場合にのみ解けます。

(6) *A が可換環の場合、上三角群 T(n, A) は解けますが、一般に零能ではありません。*

#### 命題 10 {#alg-i-s6-prop-10 .statement tag=05DP}

※Gを群、nを整数とします。次の条件は同等です:*

(i) *G は類 $\leq n$ で解けます。*
(ii) *G*の通常の部分群の系列が存在します
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
*群 $G^k/G^{k+1}$ は可換です。*
(iii) *G* の部分群の系列が存在します
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = e
$$
*すべての k について、$G^{k+1}$ は $G^k$ の通常の部分群であり、$G^k/G^{k+1}$ は可換です。*

(iv) $G/A$ が類 $\leq n - 1$ で解けるような、$G$ の通常の可換部分群 $A$ が存在します。

(i) $\Rightarrow$ (ii) の場合、$G^k$ を $D^k(G)$ と等しくすれば十分です。 (ii) $\Rightarrow$ (iii) 些細なこと。 (iii) $D^k(G)$ の$\Rightarrow$ (i) は必ず$G^k$ に含まれます。 (ii)と(iv)の同値は、$n$の帰納法による明らかです。

もっと簡単に言うと、群は、$n$ 可換群の連続する拡大によって得られる場合、類 $\leq n$ の解になります。

#### 系 {#alg-i-s6-n4-cor-1 .statement tag=05DQ}

$G$ を有限群とすると、
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
a Jordan-Hölder 系列 of $G$ $G$ が解けるには、商 $G^k/G^{k+1}$ が素数位数の巡回であることが必要かつ十分です。

$G$ の組成列の商が巡回であるため可換である場合、$G$ は命題 10 で解けます。逆に、$G$ が解ける場合、群 $G^k/G^{k+1}$ はすべての $k$ について解け、シンプル ($§ 4$、no. 7、命題 9)。さて、すべての解ける単純な群 $H$ は素数位数の巡回です。なぜなら、$D(H)$は$H$の通常の部分群です。その場合、$D^k(H) = H$ はすべての $k$ に対して $D(H) = H$ は不可能です。この場合、$D(H) = \{e\}$ と $H$ は可換です。 系は、$§ 4$、no. 10、系から命題 20 に続きます。

### 5. $p$-グループ

この数とそれに続く文字 $p$ は、素数数 ($§ 4$、いいえ 10、命題 16) を表します。

#### 定義 9 {#alg-i-s6-def-9 .statement tag=05DR}

位数が$p$の冪である有限群を$p$群と呼びます。

$G$ を位数 $p^r$ の $p$ グループとします。 $p^r$ のすべての因子は、$p$ の冪 ($§ 4$、no. 10、系 ～ 定理 7) です。したがって、$G$ のすべての部分群とすべての剰余群は、$p$ グループ ($§ 4$、no. 4、系 ～ 命題 4) です。 $G$ のすべての同次空間の基数は、$p$ の冪 ($§ 5$、no. 5、定理 1) です。

$p$グループの$p$グループによる拡大は$p$グループです。

*例。 (1) 可換 $p$ 群は、巡回群 $\mathbf{Z}/p^n\mathbf{Z}$ (cf. 練習問題 19 および VII、$§ 4$、no. 7、命題 7) の積と同型です。
(2) $k$を特性$p$の有限体とする。厳密な三角形群 $T_1(n, k)$ は $p$ 群です。
(3) 四元数の群 $\{ \pm 1, \pm i, \pm j, \pm k \}$ は 2 群 (cf. 練習問題 4) です。*

#### 命題 11 {#alg-i-s6-prop-11 .statement tag=05DS}

$E$ を有限の集合とし、$G$ を $E$ 上で作用する $p$ 群とする。 $E^G$ は、すべての $g \in G$ (固定の点) に対して $gx = x$ となるように、$x \in E$ の集合を表すものとします。それから
$$
\operatorname{Card}(E^G) \equiv \operatorname{Card}(E) \pmod{p}.
$$

E — E^G は軌道の互いに素和集合が点に減らない。このような軌道の基数は、$p$の冪であり、$p^0 = 1$とは異なり、したがって$p$の倍数です。

#### 系 {#alg-i-s6-n5-cor-1 .statement tag=05DT}

* G を p グループとする。 G が e に還元されない場合、その中心は e に還元されません。*

G を内部自己同型でそれ自体に作用させます。固定点の集合はGの中心Zです。命題11により、

$$
\operatorname{Card}(Z) \equiv \operatorname{Card}(G) \equiv 0 \pmod{p},
$$

よって $\operatorname{Card}(Z) \neq 1$ と $Z \neq \{e\}$。

#### 定理 1 {#alg-i-s6-thm-1 .statement tag=05DU}

*G を p グループとし、$p^r$ をその位数とします。 G* の部分群の数列が存在します

$$
G = G^1 \supset G^2 \supset \ldots \supset G^{r+1} = \{e\}
$$

*そのような* $(G, G^k) \subset G^{k+1}, 1 \leq k \leq r,$ と $G^k/G^{k+1}, 1 \leq k \leq r,$ *は位数* $p$ の循環です。

定理は $G = \{e\}$ に当てはまります。 $\operatorname{Card}(G)$の帰納法までにそれを証明します。 Z を G の中心、Z の $x \neq e$ 元 (系 ～ 命題 11)、および x の $p^s, s \neq 0,$ 位数とします。すると、$x^{p^s - 1}$ は位数 $p$ の元なので、位数 $p$ の巡回である Z 含む部分群 $G'$ になります。 帰納法の仮定までに、群 $G' = G/G'$ は、必要なプロパティを備えた部分群 $({G'}^k)_{1 \leq k \leq r}$ のうち系列を持ちます。 $\pi : G \to G'$を標準準同型とします。 $G^k = \pi^{-1}({G'}^k), 1 \leq k \leq r, G^{r+1} = \{e\}$ によって定義される G の部分群の数列は、$G^k/G^{k+1}$ の解であり、$1 \leq k \leq r$ の ${G'}^k/{G'}^{k+1}$ (§ 4, no. 7, 定理 4) と同型です。

#### 系 {#alg-i-s6-n5-cor-2 .statement tag=05DV}

*すべての p グループはゼロポテントです。*

これは、no. 3、命題 7 から続きます。

#### 命題 12 {#alg-i-s6-prop-12 .statement tag=05DW}

*G を p 基とし、G の H 部分群が G とは異なるものとする。すると、*

(a) *ノーマライザー* $N_G(H)$ *G の H は G* とは異なります。
(b) *G には添字 p の G の正規の部分群* N * が存在し、それは含む* H です。

主張 (a) は no. 3, 系 1 から命題 8 に続きます。(b) を証明します。 no. 3、系 2 から命題 8 までには、G とは異なり、$G/N'$ が可換であるような G 含む H の通常の部分群 $N'$ が存在します。 N を G 含む $N'$ とは異なる最大値部分群とする。この場合、N は正規 (no. 2、系 3 ～ 命題 6) であり、$G/N$ は単純な可換 $p$ 群であるため、位数 $p$ (§ 4, no. 10、系 ～ 命題) の循環となります。 20）。

#### 系 {#alg-i-s6-n5-cor-3 .statement tag=05DX}

* G を p グループとする。 添字 p の G のすべての部分群は正常です。*

### 6. シロウ部分群

#### 定義 10 {#alg-i-s6-def-10 .statement tag=05DY}

G を有限群とします。 G の Sylow p サブグループは、G 満たすの任意の部分群 P であり、条件に続く 2 つです。

(a) P は p 基です。
(b) (G : P) は p の倍数ではありません。

Gの位数を形$p^r m$に書き、mが$p$の倍数ではない場合、条件(a)と(b)は$\mathrm{Card}(P) = p^r$と等価です。

#### 例 {#alg-i-s6-n6-exa-1 .statement tag=05DZ}

(1) 群 $\mathfrak{S}_p$ において、$\zeta$ を位数 $p$ のサイクルとします。 $\zeta$ によって生成された部分群は、$p$ に対する $\mathfrak{S}_p$ の Sylow $p$ サブグループであり、割る $(p - 1)!$ ではありません。
(2) ※kを特性$p$の有限体、nを正の整数とする。厳密な三角形群 $T_1(n, k)$ は、群 $\mathbf{GL}(n, k)$ の Sylow $p$ 部分群です。*

#### 定理 2 {#alg-i-s6-thm-2 .statement tag=05E0}

すべての有限群含むが Sylow $p$ サブグループです。

証明は次の補題に依存します。

#### 補題 {#alg-i-s6-n6-lem-1 .statement tag=05E1}

$n = p^r m$ とします。ここで、m は $p$ の倍数ではない整数です。それから
$$
\binom{n}{p^r} \not\equiv 0 \pmod{p}.
$$

S を位数 $p^r$ (例えば $\mathbf{Z}/p^r \mathbf{Z}$) の群とし、T 集合を m 元とします。 $X = S \times T$ と書き、E を $p^r$ 元を含む X の部分集合の集合とします。 次に、$\mathrm{Card}(X) = n$、よって $\mathrm{Card}(E) = \binom{n}{p^r}$ (集合理論、III, § 5, no. 8、系 1 ～ 命題 11)。 S を $s.(x, y) = (sx, y) (s, x \in S, y \in T)$ によって X で演算し、この演算から E までの正規の拡大を考慮します。 no. 5の記法、命題 11、集合 $E^S$は、Xの軌道の集合、つまり部分集合の集合、形の$Y \subset X$です$S \times \{ t \}, t \in T$、よって $\mathrm{Card}(E^S) = m$。 no. 5、命題 11 までに、
$$
\binom{n}{p^r} = \mathrm{Card}(E) \equiv \mathrm{Card}(E^S) = m \not\equiv 0 \pmod{p},
$$
これは補題を証明します。

これで定理が証明されました。 G を有限群とし、n を位数とします。 $n = p^r m$と書きますが、mは$p$の倍数ではありません。 E を $p^r$ 元とする G の部分集合の集合とします。それから
$$
\mathrm{Card}(E) = \binom{n}{p^r};
$$
よって、補題、$\mathrm{Card}(E) \not\equiv 0 \pmod{p}$ のおかげで。左変換による G 自体の演算の E への拡大を考えてみましょう。 軌道がゼロ以外の基数 mod を持つ $X \in E$ が存在します。 $p$。 $H_X$ が X の固定群を表す場合、

$(G:H_x) \not\equiv 0 \pmod{p}$、つまり $p^r$ 割る $\mathrm{Card}(H_x)$ です。しかし、$H_x$ は $sX = X$ となるような $s \in G$ で構成されます。 $x \in X$の場合、$H_x \subset X.x^{-1}$、よって $\mathrm{Card}(H_x) \leqslant \mathrm{Card}(X) = p^r$。したがって$\mathrm{Card}(H_x) = p^r$です。

#### 系 {#alg-i-s6-n6-cor-1 .statement tag=05E2}

*G の位数が p で割り切れる場合、群 G 含む元の位数 p.*

定理 2 により、これは G が $p$ 基 $\neq \{e\}$ である場合に帰着します。 $x \in G$ が e と異なる場合、x によって生成される循環群は、位数 $p^n$ と $n \geqslant 1$ であり、したがって、位数 $p$ の含む部分群になります。

#### 注意 {#alg-i-s6-n6-rem-1 .statement tag=05E3}

Card(G) を分割するすべての素数数 q について、P_q を G の Sylow q 部分群とします。すると、P_q によって生成された G の部分群 H は、各 q について Card(P_q) の位数倍数であり、Card(G) の位数因子のものであるため、次と等しくなります。 G.

#### 定理 3 {#alg-i-s6-thm-3 .statement tag=05E4}

*G を有限群とします。*
(a) *G の Sylow p サブグループは共役から 1 つの他のです。それらの数は 1 mod に一致します。 p.*
(b) *p 群である G のすべての部分群は Sylow p 部分群に含まれます。*

P を G の Sylow $p$ 部分群 (定理 2)、H を G の $p$ 部分群とする。E = G/P とし、G/P 上の H の演算を考慮する。カードとして(E) $\not\equiv 0$ mod. $p$、命題 no. 5 の 11 は、すべての $h \in H$ に対して $hx = x$ となるような $x \in G/P$ が存在することを示しています。 g が G の x の代表である場合、これは $H \subset gPg^{-1}$, よって主張を意味します (b)。

H が Sylow $p$ 部分群である場合、Card(H) = Card(P) = Card($gPg^{-1}$)、よって $H = gPg^{-1}$ となり、(a) の最初の主張が証明されます。

次に、(a) の 2 番目の主張を証明します。 $\mathscr{S}$ を G の Sylow $p$ 部分群の集合とし、P を内部自己同型によって $\mathscr{S}$ に作用させるとします。 元 $P \in \mathscr{S}$ はこの演算の下で固定の点であり、それが唯一であることを示します。 $Q \in \mathscr{S}$ を固定の点とします。 Q は P で正規化された G の Sylow 部分群であるため、P は Q の正規化子 N に含まれます。 群 P と Q は N の Sylow $p$ サブグループです。したがって、$P = nQn^{-1} = Q$ となるような $n \in N$ が存在します。 no. 5、命題 11、カード($\mathscr{S}^P$) $\equiv$ カード($\mathscr{S}^{P^P}$) = 1 (修正$p$)。

#### 系 1 {#alg-i-s6-thm-3-cor-1 .statement tag=05E5}

*P を G の Sylow p 部分群とし、N を G 内のノーマライザーとし、M を G 含む N の部分群とする。G 内の M のノーマライザーは M に等しい。*

$s \in G$ を $sMs^{-1} = M$ となるようにします。 M の部分群 $sPs^{-1}$ は M の Sylow $p$ 部分群です。したがって、$sPs^{-1} = tPt^{-1}$ となるような $t \in M$ が存在します。次に$t^{-1}s \in N$、よって $s \in tN \subset M$。

#### 系 2 {#alg-i-s6-thm-3-cor-2 .statement tag=05E6}

※$f : G_1 \to G_2$を有限群の準同型とします。 $G_1$ のすべての Sylow p サブグループ $P_1$ に対して、$f(P_1) \subset P_2$ となるような $G_2$ の Sylow p サブグループ $P_2$ が存在します。

これは、定理 3 (b) を $G_2$ の部分群 $f(P_1)$ に適用した結果となります。

#### 系 3 {#alg-i-s6-thm-3-cor-3 .statement tag=05E7}

(a) $H$ を $G$ の部分群とします。 $H$ のすべての Sylow $p$ サブグループ $P$ に対して、$P = Q \cap H$ のような $G$ の Sylow $p$ サブグループ $Q$ が存在します。

(b) 逆に、$Q$ が $G$ の Sylow $p$ サブグループであり、$G$ で $H$ が正常である場合、群 $Q \cap H$ は $H$ の Sylow $p$ サブグループです。

(a) $p$ グループ $P$ は、$G$ の Sylow $p$ サブグループ $Q$ に含まれており、$Q \cap H$ は $H$ 含む $P$ の $p$ サブグループであり、したがって、$P$に等しい。

(b) $P'$ を $H$ の Sylow $p$ 部分群とする。 $gP'g^{-1} \subset Q$ となるような元 $g \in G$ が存在します。 $H$ が正常であるため、$P = gP'g^{-1}$ は $H$ に含まれ、したがって $Q \cap H$ に含まれます。 $Q \cap H$ は $H$ の $p$ サブグループであり、$P$ は $H$、$P = Q \cap H$ の Sylow $p$ サブグループです。

#### 系 4 {#alg-i-s6-thm-3-cor-4 .statement tag=05E8}

$N$を$G$の通常の部分群とします。 $G$ の Sylow $p$ サブグループの $G/N$ の像は、$G/N$ の Sylow $p$ サブグループであり、$G/N$ のすべての Sylow $p$ サブグループがこのようにして得られます。

Let $G' = G/N$ and $P'$ be the image in $G'$ of a Sylow $p$-subgroup $P$ of $G$. 群 $G$ は $G'/P'$ で推移的に動作するため、$G'/P'$ は $G/S$ と等価です。ここで、$S$ は $G$ 含む $P$ の部分群です。 したがって、$(G':P')$ 割る $(G:P)$ は、$p$ の倍数ではなく、$p$ グループ $P'$ は $G'$ の Sylow $p$ サブグループです。 $Q'$ を他の Sylow $p$ の $G'$ のサブグループとします。それから$Q' = g'P'{g'}^{-1}$、いくつかの$g' \in G'$。 $g \in G$が$g'$の代表である場合、群$Q'$は$Q = gPg^{-1}$の像です。

### 7. 有限の無能群

#### 定理 4 {#alg-i-s6-thm-4 .statement tag=05E9}

$G$を有限群とします。次の条件は同等です。

(a) $G$ は無能です。
(b) $G$ は $p$ グループの積です。
(c) すべての素数数 $p$ に対して、$G$ の正規 Sylow $p$ 部分群が存在します。
(b) $\Rightarrow$ (a) (no. 5、系 ～ 定理 1)。

(a) が成り立ち、$P$ を $G$ の Sylow $p$ サブグループとします。 $N$ が $G$ の $P$ のノーマライザーである場合、系 1 から定理 3 は、$N$ が独自のノーマライザーであることを示します。 § 6, no. 3、系から命題 8 までは、$N = G$ であることを示しています。したがって、(a) $\Rightarrow$ (c) となります。

(c) が成り立ち、$I$ を $\mathrm{Card}(G)$ を割った素数数の集合とする。すべての $p \in I$ について、$P_p$ を $G$ の通常の Sylow $p$ サブグループとします。すべての $p \neq q$、$P_p \cap P_q$ は、$p$ グループと $q$ グループの両方であるため、$e$ に減らされます。したがって、$P_p$ と $P_q$ は 1 つの他の ($§ 4$、no. 9、 命題 15）。 $\phi$を$\prod_{p \in I} P_p$の$G$に標準準同型($§ 4$、no. 9、命題12)とします。 準同型 $\phi$ は no. 6 の注意によって全射です。 $\mathrm{Card}\left(\prod_{p \in I} P_p\right) = \mathrm{Card}(G)$ であるため、$\phi$ は全単射であることがわかります。

#### 注意 {#alg-i-s6-n7-rem-1 .statement tag=05EA}

(1) G を有限群および $p$ を素数数とする。 no. 6、定理 3 (a) および no. 6、定理 2 により、次の条件は同等です。
(i) G の通常の Sylow $p$ サブグループが存在します。
(ii) G のすべての Sylow $p$ サブグループは正常です。
(iii) G の Sylow $p$ サブグループは 1 つだけ存在します。

(2) G をゼロ能有限群とします。 Iをカード(G)の素数因子の集合とします。 定理 4 と注意 1、$G = \prod_{p \in I} G_p$ により、$G_p$ は G の一意の Sylow $p$ グループです。

(3) 可換群, 定理 4 に適用すると、可換有限群の分解が主成分の積として得られます。これは、章のビューの他の点から学習されます。 VII。

#### 例 {#alg-i-s6-n7-exa-1 .statement tag=05EB}

群 $\mathfrak{S}_3$ は位数 6 のものです。 含むは位数 3 の通常の Sylow 3 部分群です: 群 $A_3$。それは含む位数 2 の 3 つの Sylow 2 サブグループです: 群 $\{e, \tau\}$、ここで $\tau$ は転置です。したがって、群 $\mathfrak{S}_3$ はゼロではありません。

### 練習問題 {#alg-i-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
