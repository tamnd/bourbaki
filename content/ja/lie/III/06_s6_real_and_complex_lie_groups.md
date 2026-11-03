---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 6
section_title: Real and complex Lie groups
lang: ja
source: lie-i-iii
book_pages: 304-326, 383-391
pdf_pages: 0322-0344, 0401-0409
extraction: ocr
subsections:
    - "no": 1
      title: PASSAGE FROM LIE ALGEBRA MORPHISMS TO LIE GROUP MORPHISMS
      page: 304
      pdf_page: 322
    - "no": 2
      title: INTEGRAL SUBGROUPS
      page: 306
      pdf_page: 324
    - "no": 3
      title: PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS
      page: 310
      pdf_page: 328
    - "no": 4
      title: EXPONENTIAL MAPPING
      page: 311
      pdf_page: 329
    - "no": 5
      title: APPLICATION TO LINEAR REPRESENTATIONS
      page: 315
      pdf_page: 333
    - "no": 6
      title: NORMAL INTEGRAL SUBGROUPS
      page: 316
      pdf_page: 334
    - "no": 7
      title: PRIMITIVES OF DIFFERENTIAL FORMS WITH VALUES IN A LIE ALGEBRA
      page: 318
      pdf_page: 336
    - "no": 8
      title: PASSAGE FROM LAWS OF INFINITESIMAL OPERATION TO LAWS OF OPERATION
      page: 318
      pdf_page: 336
    - "no": 9
      title: EXPONENTIAL MAPPING IN THE LINEAR GROUP
      page: 320
      pdf_page: 338
    - "no": 10
      title: COMPLEXIFICATION OF A FINITE-DIMENSIONAL REAL LIE GROUP
      page: 322
      pdf_page: 340
statements: 71
exercises: 30
content_sha256: 0a8ad80b08d0b1c8f7ba1bb3e7d584324f366fbab1731325a95f7c51e3655a82
translated_from: content/en/lie/III/06_s6_real_and_complex_lie_groups.md
translation_method: google
source_content_sha256: e472279781ec8c0c5cc2af6e1e4dd1a20a67a73d7a8042acdd1dea73f6ae558d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: af97e06fbb4e89aae2b9c68460fc596e5233f024ecbfd4f84ea015535252f553
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 6。現実的かつ複雑リー群

この段落では、K は $\mathbf{R}$ または $\mathbf{C}$ に等しいと想定されます。

### 1. リー代数射からリー群射への通路

#### 補題 1 {#lie-iii-s6-lem-1 .statement tag=0AE8}

*Let G be a simply connected† topological group, W a symmetric connected open neighbourhood of e, H a group and f a mapping of $W^3$ into H such that*

$$
f(xyz) = f(x)f(y)f(z)
$$

*W の x、y、z について。H には $f' \mid W = f \mid W$ となるような G の射 $f'$ が存在します。*

$(g, h) \in G \times H$ と U について、W の e のオープン近傍に対して、$A(g, h, U)$ を $u \in U$ の $(gu, hf(u)) \in G \times H$ の集合とします。次に$(g, h) \in A(g, h, U)$と$A(g, h, U_1) \cap A(g, h, U_2) = A(g, h, U_1 \cap U_2)$。 $(s, t) \in A(g, h, U)$ にしましょう。次に、$s = gu$ と $t = hf(u)$ が $u \in U$ になります。 $uU' \in U$ となるような W の e の開いた近傍 $U'$ が存在します。次に、$u' \in U'$ については、

$$
(su', tf(u')) = (guu', hf(uu')) \in A(g, h, U)
$$

† 参照。 *一般位相* の章 XI (登場予定)。この章で、$G_1, G_2$ がトポロジー 群で接続されている場合、$\phi$ は$G_1$ の$G_2$ 上の離散核の開連続準同型であり、$G_2$ は単純に接続されており、$\phi$ は準同型性。一方、単純に接続された空間が接続されていることを思い出してください。

したがって $A(s, t, U') \subset A(g, h, U)$ です。 次に、$G \times H$ の位相の $A(g, h, U)$ 形基底が続きます。 We shall denote by $Y$ the set $G \times H$ with this topology and denote by $p$ the canonical projection of $Y$ onto $G$, which is open. $p$ から $A(g, h, U)$ の制限は、$A(g, h, U)$ の $gU$ への同型写像です。 したがって、$(Y, p)$ は $G$ のカバー 空間です。 $Y_0$ を $A(e, e, W)$ によって生成された $Y$ の部分群とし、$\mathfrak{B}$ を $A(e, e, U)$ の集合とします。 明らかに、$\mathfrak{B}$ は *一般位相*、章 III, § 1, no. 2 の条件 (GV$_1'$) および (GV$_1''$) を満たします。 The set $Y_0'$ of $y \in Y_0$ such that the mappings $z \mapsto yzy^{-1}$ and $z \mapsto y^{-1}zy$ of $Y_0$ into $Y_0$ are continuous at $(e, e)$ is a subgroup of $Y_0$. $w \in W$ にしましょう。 $W$ から $G$ への写像 $w' \mapsto ww'w^{-1}$ は連続であるため、写像

$$
(w', f(w')) \mapsto (ww'w^{-1}, f(ww'w^{-1}))
$$

$A(e, e, W)$ から $Y$ へは $(e, e)$ で連続します。現在は$f(ww'w^{-1}) = f(w)f(w')f(w^{-1})$、つまり$(ww'w^{-1}, f(ww'w^{-1})) = (w, f(w))(w', f(w'))(w, f(w))^{-1}$です。

$w^{-1} \in W$ として、$(w, f(w)) \in Y_0'$ であることがわかります。したがって、$A(e, e, W) \subset Y_0'$、つまり $Y_0' = Y_0$ になります。 群 $Y_0$ は、フィルター 基底 $\mathfrak{B}$ を使用すると、*一般位相*、章 III, § 1, no. 2 の条件 (GV$_{III}'$) を満たします。として

$$
(g, h).A(e, e, U) = A(g, h, U),
$$

$Y_0$ は、$A(e, e, W)$ が接続されているため、接続されているトポロジー 群です。すると、$G$が接続されているため、$p(Y_0)$は$G$、よって、$p(Y_0) = G$のオープン部分群になります。 $p \mid Y_0$の核は離散的です。 $G$は単純に接続されているので、$p \mid Y_0$は$Y_0$の$G$への同写写像です。したがって、$Y_0$は$G$の射$f'$を$H$にグラフ化したものになります。 $g \in W$、$(g, f(g)) \in A(e, e, W) \subset Y_0$、よって $f'(g) = f'(g)$の場合。

#### 定理 1 {#lie-iii-s6-thm-1 .statement tag=0AE9}

*$G$と$H$をリー群と$h$を$L(G)$から$L(H)$に続く射とします。 $G$ が単純に接続されているとします。すると、$H$ には $h = L(\phi)$ となる $G$ のリー群射 $\phi$ が 1 つだけ存在します。*

$\phi$ の存在は、補題 1 と § 4, no. 1、定理 1 (i) から続きます。 $\phi$ の一意性は、§ 4, no. 1、定理 1 (ii) と$G$ が接続されているという事実から導き出されます。

#### 系 {#lie-iii-s6-n1-cor-1 .statement tag=0AEA}

※$G$を有限次元の単純結合したリー群とします。 核が離散的である $G$ の有限次元解析線型表現が存在します。

リー代数 $\mathrm{End}(E)$ には (章 I, § 7, 定理 2) 有限次元ベクトル空間 $E$ と $L(G)$ の単射詞射 $h$ が存在します。 定理 1 までに、$G$ の $\mathbf{GL}(E)$ に $L(\phi) = h$ となるように射 $\phi$ が存在します。 したがって、$\phi$ は浸漬であり、したがってその核は離散です。

#### 注意 {#lie-iii-s6-n1-rem-1 .statement tag=0AEB}

(1) 有限次元単射解析線型表現 (練習問題 2) をもたない有限次元単結合リー群が存在する。

(2) $G$ のすべての有限次元解析線型表現が非離散核 (練習問題 3 および 4) を持つように、接続された有限次元リー群 $G$ が存在します。

### 2. インテグラル部分群

#### 定義 1 {#lie-iii-s6-def-1 .statement tag=0AEC}

G をリー群とします。 G の積分部分群は、リー群構造が接続された部分群 H であり、G への H の標準単射は浸漬です。

G の 1 パラメータ部分群は、G の 1 次元積分部分群です。

H を G の積分部分群および H の i 標準単射を G に変換するとします。次に、トポロジカル補充を認める L(G) のリー 部分代数上に L(H) の L(i) 定義する同型を加えます。 L(H) は、L(i) の像と識別されます。

#### 例 {#lie-iii-s6-n2-exa-1 .statement tag=0AED}

(1) G の接続された嘘部分群は G の積分部分群です。

(2) G が有限次元であると仮定します。 H を G の部分群とします。 G (§ 4, no. 5, 定義 3) のリー群構造によって誘導される構造を与えます。このとき、その単位成分 H_0 は G の積分部分群であり、e における H の接線部分代数は L(H_0) (§ 4, no. 5, 命題 9 (ii)) です。

(3) G を複素数リー群、H を G の積分部分群および G_1 (それぞれ H_1) を G (それぞれ H) の基礎となる実リー群とします。この場合、H_1 は G_1 の積分部分群であり、L(H_1) は L(H) の基礎となる実数リー代数です。

#### 定理 2 {#lie-iii-s6-thm-2 .statement tag=0AEE}

G をリー群とします。

(i) 写像 H ↦ L(H) は、トポロジカル補充を認める L(G) の Lie 部分代数の集合上に G の積分部分群の集合の全単射です。

(ii) H を G の積分部分群とする。リー代数 L(H) と接続された G のすべてのリー 部分群ジャームは、生成する H である H の開部分多様体である。

(a) h をトポロジー 補充を認める L(G) の嘘部分代数とする。 H_1 を、L(H_1) = h (§ 4, 定理 3) となる G の Lie 部分群胚芽とする。 H_1 を選択して接続することができます。 HをH_1によって生成されたGの部分群とする。 H 上に (§ 1、系から命題 22) リー群構造が存在し、H_1 が H の開部分多様体であり、H から G への標準単射が浸漬です。 H_1 が接続されているため、H も接続されており、G の積分部分群になります。すると、L(H) = L(H_1) = h となります。これは、(i) で考慮した写像が全射であることを証明します。

(b) H を G の積分部分群とし、N_1 を G のリー 部分群ジャームとリー代数 L(H) で接続したものとする。 H の G への標準単射は浸漬であるため、H の開いた部分群ジャーム H_1 が存在します。これは同時に G の部分多様体であり、したがってリー代数 L(H) を持つ G のリー 部分群ジャームが存在します。一方、N を N_1 によって生成された G の部分群とします。 証明の部分 (a) により、N_1 が N の開部分多様体となるような G の積分部分群の構造を持ちます。 § 4, 定理 3 により、H_1 ∩ N_1 は H_1 と N_1 で開きます。したがって、H_1 ∩ N_1 によって生成される G の部分群は、一方では H に等しく、他方では N に等しい。したがって、リー群 H と N は等しい。これは (ii) を証明し、また (i) で考慮された写像が単射であることも証明します。

#### 注意 1 {#lie-iii-s6-n2-rem-1 .statement tag=0AEF}

H を G の整数部分群とします。 Y を L(H) に関連付けられた G の左葉とします。 $g \in G$ の場合、H 上の値から $\gamma(g)$ によって導出された $gH$ に多様体構造が与えられるとします。 微分可能かつ解析的多様体、R、9.3.2、$gH$ の標準単射を Y にすると、射になります。 この射はエターレです。 したがって、Y の最大連結リーフは H を法とする左剰余類です。

#### 命題 1 {#lie-iii-s6-prop-1 .statement tag=0AEG}

*G と M をリー群とし、H は G の部分群と M の $\phi$ 射を G に積分して $L(\phi)(L(M)) \subset L(H)$ となるようにします。 M が接続されているとします。すると、$\phi(M) \subset H$ と $\phi$ は、M から H への写像とみなされて、リー群射となります*。

注意 1 の記法では、M が接続されているため、$\phi$ は M の Y への射 (*微分可能および解析的多様体*、R、9.3.2) となり、したがって $\phi(M) \subset H$ になります。

#### 系 1 {#lie-iii-s6-prop-1-cor-1 .statement tag=0AEH}

※GとHを、Gのリー群、$\phi$、リー群、射をH、$\phi$、$h = L(\phi)$のN核とします。 G が接続されており、H が有限次元であると仮定します。*
(i) *N は G と $L(N) = \mathrm{Ker}\ h$ の嘘部分群です。*
(ii) *H' を H とリー代数 Im h の積分部分群とします。次に、$\phi(G) = H'$.*
(iii) *移行～商がリー群同型のとき、$\phi$から導かれるG/Nの写像をH'に変換します。

(i) はすでに証明されています (§ 3, no. 8, 命題 28)。

$\psi$ を移行から商のとき $\phi$ から導出された H への G/N のリー群射とします。それは没入です (§ 3, no. 8、命題 28)。 命題 1 により、$\psi$ は G/N のリー群射を H' に変換します。この射はエタールであり、H' が接続されているため $\psi(G/N) = H'$ になります。これは(ii)を証明します。すると、$\psi : G/N \to H'$ は全単射でリー群同型となり、(iii) が証明されます。

#### 系 2 {#lie-iii-s6-prop-1-cor-2 .statement tag=0AEI}

*G をリー群とし、H_1 と H_2 を G の積分部分群とします。$L(H_2) \subset L(H_1)$ の場合、H_2 は H_1 の積分部分群です。

$i_1 : H_1 \to G, i_2 : H_2 \to G$を標準単射とします。 Then
$$
L(i_2)(L(H_2)) = L(H_2) \subset L(H_1).
$$
By Proposition 1, $i_2$ is an analytic mapping of $H_2$ into $H_1$ and even an immersion of $H_2$ into $H_1$ since $L(i_2)$ is an isomorphism of $L(H_2)$ onto a subalgebra of $L(H_1)$ admitting a topological supplement.

#### 系 3 {#lie-iii-s6-prop-1-cor-3 .statement tag=0AEJ}

*G を有限次元リー群とし、$(H_i)_{i \in I}$ を G の嘘部分群の族とする。すると、$H = \bigcap_{i \in I} H_i$ は G の嘘部分群であり、*
$$
L(H) = \bigcap_{i \in I} L(H_i).
$$
$\bigcap_{i \in J} L(H_i)$ がすべての L(H_i) の共通部分 M に等しいような I の有限部分集合 J が存在します。 H^* = \bigcap_{i \in J} H_i は、L(H^*) = M (§ 3, no. 8, 系 2 ～ 命題 29) となるような嘘部分群であることがわかっています。 H_0 を H^* のアイデンティティ成分とします。これは G の嘘部分群と L(H_0) = M です。 系 2 より、すべての i に対して H_0 \部分集合 H_i となり、したがって H_0 \部分集合 H \部分集合 H^*, よって系となります。

#### 系 4 {#lie-iii-s6-prop-1-cor-4 .statement tag=0AEK}

*G を有限次元接続リー群とする。次の条件は同等です:*
(i) *G はユニモジュラー* (統合、章 VII, § 1, no. 3、定義 3);
(ii) *det Ad g = 1 すべての g \in G*;
(iii) *Tr ad a = 0 (すべての a \in L(G)*)。

写像 g \mapsto det Ad g は、G の射 $\phi$ を K* に変換します。 § 3、命題 35 (no. 10) および 44 (no. 12) までに、すべての $a \in L(G)$ に対して $L(\phi)a = Tr\ ad\ a$。明らかに Im $L(\phi) = \{0\}$ または K です。最初 (または 2 番目) の場合、Im $\phi = \{1\}$ (それぞれ Im $\phi = K^*$) は系 1 により、したがって G は § 3, no. 16、系から命題 55 により単モジュール化されます (それぞれ単モジュール化されません)。

#### 命題 2 {#lie-iii-s6-prop-2 .statement tag=0AEL}

*G を有限次元リー群とし、H を G の積分部分群とします。次の条件は同等です:*
(i) *H は閉じています*;
(ii) H 上の *位相は G* 上の *位相によって誘導されます。
(iii) *H は G* の嘘部分群です。
(i) $\Rightarrow$ (iii): これは、§ 1、命題 2 (iv) (no. 1) および 14 (iii) (no. 7) から続きます。
(iii) $\Rightarrow$ (ii): 明らかです。
(ii) $\Rightarrow$ (i): H 上の位相が G 上の⟧ によって誘導される場合、H は完了しているため、H は閉じます (§ 1, no. 1、命題 1)。

#### 命題 3 {#lie-iii-s6-prop-3 .statement tag=0AEM}

*G をリー群、H を G の積分部分群、M を空でない接続された分析多様体、f 写像を M から G に、r \in N_K とします。次の条件を考慮してください:*
(i) *f は類 C^r および f(M) \部分集合 H* です。
(ii) *f(M) \部分集合 H および f は、M から H への写像と見なされ、類 C^r* になります。
(iii) *f は類 C^r であり、f(M) は H と一致し、T_m(M) の像は f(m) に含まれます。M* のすべての m についてL(H)。

※次に、(ii)$\Leftrightarrow$(iii)$\Rightarrow$(i)となります。 H の位相が可算基底を認める場合、3 つの条件は同等です。*
(ii) $\Rightarrow$ (i) および (ii) $\Rightarrow$ (iii): 明らかです。
(iii) $\Rightarrow$ (ii): 条件 (iii) が成り立つと仮定します。 *微分可能かつ解析的多様体* により、R、9.2.8、f は、M の類 C^r の射で、L(H) に関連付けられた左側の葉構造になります。 M が接続されているため、f(M) \部分集合 H となります。

H 上の位相が可算基底を認める場合、条件 (i) は、f が H への M の類 C^r の写像であることを意味します (*微分可能および解析多様体*、R、9.2.8)。したがって、(i) $\Rightarrow$ (ii)。

#### 系 1 {#lie-iii-s6-prop-3-cor-1 .statement tag=0AEN}

G を有限次元リー群、H を G の積分部分群とします。そのとき、 e (§ 4, no. 5、定義 2 および 3) における H に接するリー 部分代数は L(H) であり、H 上のリー群構造は、それによって誘導される構造です。 Gで。

H は接続されており有限次元であるため、その位相は可算の基底を許容します。

#### 系 2 {#lie-iii-s6-prop-3-cor-2 .statement tag=0AEO}

G をリー群とし、H_1 と H_2 を G の積分部分群とします。H_1 上の位相が可算数基底を許容するとします。それから

$$
H_2 \subset H_1 \Leftrightarrow L(H_2) \subset L(H_1)
$$

そして、これら条件が成立する場合、H_2 は H_1 の整数部分群になります。

最後の主張と含意 $L(H_2) \subset L(H_1) \Rightarrow H_2 \subset H_1$ は系 2 から命題 1 に続きます。 逆含意は命題 3 から続きます。

#### 系 3 {#lie-iii-s6-prop-3-cor-3 .statement tag=0AEP}

G をリー群とし、H_1 と H_2 を G の積分部分群とし、位相は可算基底を許容します。 H_1 と H_2 の基礎となる集合が同じ場合、H_1 と H_2 のリー群構造は同じです。

これは系 2 から続きます。

#### 注意 2 {#lie-iii-s6-n2-rem-2 .statement tag=0AEQ}

G を有限次元リー群とします。 H を G の部分群とします。言葉の乱用により、H にリー群構造 S が存在する場合、H は G の積分部分群であり、H は S とともに G の積分部分群であるとします。 系 3 から命題 3 までにより、S が存在する場合、S は一意です。

#### 注意 3 {#lie-iii-s6-n2-rem-3 .statement tag=0AER}

V を類 C^r の多様体とします。 M を V の部分集合とし、M の x と y 元とします。 次の性質について考えてみましょう。

P_{M, x, y}: there exist I, x_0, x_1, \ldots, x_n, f_1, \ldots, f_n such that: (a) I is a connected open subset of \mathbf{K}; (b) x_0, \ldots, x_n are in M, x_0 = x, x_n = y; (c) for 1 \leq i \leq n, f_i is a mapping of class C^r of I into V which takes the values x_{i-1} and x_i and f_i(I) \subset M.

M のすべての元 x, y について、性質 P_{M, x, y} が成り立つ場合、M は V の C^r 接続された部分集合であると言います。

#### 命題 4 {#lie-iii-s6-prop-4 .statement tag=0AES}

G を G の有限次元リー群および H 部分群とします。r \in \mathbf{N}_\mathbf{K} とします。次の条件は同等です。
(i) H は G の整数部分群です。
(ii) G 上のリー群構造により誘導されると、H が接続されます。
(iii) H は C^r 連結。
(iii) \Rightarrow (i): 明らかです。
(i) \Rightarrow (iii): H が G の整数部分群となるように、H がリー群構造を持つとします。 性質 P_{H, e, y} が成り立つように、H に注意 3 の記法、y の集合を使用すると、オープンになります。 H の部分群。H が接続されているため、この部分群は H に等しいため、条件 (iii) が満たされます。

(iii) ⇒ (ii): 条件 (iii) が満たされ、H に G 上のリー群構造によって誘起される構造が与えられるとします。 h を e における H に接する部分代数とします。 H の単位成分 H_0 は、L(H_0) = h となる G の積分部分群です。 H = H_0 であることを示します。 It suffices to prove the following: let I be a connected open subset of K, f a mapping of class C^r of I into G such that f(I) ⊂ H and λ and μ two points of I; if f(λ) ∈ H_0, then f(μ) ∈ H_0. しかし、すべての v ∈ I について、h の定義によって (T_v f)(K) ⊂ f(v)h となるため、主張は命題 3 から続きます。

#### 注意 4 {#lie-iii-s6-n2-rem-4 .statement tag=0AET}

K = R の場合、G の積分部分群は、G の積分によって引き起こされる位相と弧状に接続された部分群として特徴付けることもできます (§ 8, 練習問題 4)。ただし、部分群は接続されていても一体ではありません (可換代数、章 VI, § 9、練習問題 2)。

#### 系 {#lie-iii-s6-n2-cor-1 .statement tag=0AEU}

G を有限次元リー群とし、H_1 と H_2 を G の 2 つの積分部分群とします。H_1 と H_2 によって生成された G の部分群と G の部分群 (H_1, H_2) は G の積分部分群とします。

G の部分群 (G, G) は常に閉じているとは限りません (§ 9, 練習問題 6)。

a が有限次元代数の場合、Aut(a) は GL(a) の Lie 部分代数であり、L(Aut(a)) は a の導分のリー代数であることを思い出してください (§ 3, no. 11、系 5 から命題 41)。

#### 定義 2 {#lie-iii-s6-def-2 .statement tag=0AEV}

a を有限次元リー代数とします。 Ad(a) または Int(a) が、Aut(a) とリー代数 ad(a) の積分部分群を表すものとします。この群の元をaの内部自己同型と呼びます。

構造の輸送までに、ad(a) は Aut(a) の下で不変であるため、Aut(a) では Int(a) が正規になります。 By § 4, no. 4, Corollary 1 to Proposition 8 and the fact that Int(a) is connected, the elements of Int(a) are the finite products of automorphisms of the form exp ad x where x ∈ a. 一般に、Int(a) は Aut(a) (練習問題 14) の嘘部分群ではありません。

### 3. リー代数からリー群への通路

#### 定理 3 {#lie-iii-s6-thm-3 .statement tag=0AEW}

(i) L が有限次元リー代数である場合、L(G) が L と同型となるような単純結合リー群 G が存在します。

(ii) G_1 と G_2 を 2 つ接続リー群とし、G_1 を単純接続します。 f を L(G_1) の同型を L(G_2) に、G_1 の φ 射を G_2 に、L(φ) = f および φ の N 核とする。この場合、N は、G_1 の中心と G_1/N の G_2 への射の離散部分群であり、φ はリー群同型から導出されます。 G_2を単純に接続するとφは同型となります。

L を有限次元のリー代数とします。 L が End(E) の嘘部分代数と同一視できるような有限次元ベクトル空間 E が存在します (章 I, § 7, 定理 2)。 H を GL(E) の積分部分群とします。

リー代数 L。 $\hat{H}$ をその普遍的なカバー ($§ 1$、no. 9、*注意*) とします。この場合、$L(\hat{H})$ は L、よって (i) と同型です。

$G_1, G_2, f, \phi, N$ を (ii) のようにします。この場合、$\phi$ はエタールであるため、$\phi(G_1)$ は $G_2$ のオープン部分群となり、したがって $\phi(G_1) = G_2$ になります。一方、N は離散的であるため、$G_1$ の中心 (*積分*、章 VII、$§ 3$、補題 4) に含まれます。明らかに、$\phi$ から派生した $G_2$ への $G_1/N$ の射は、リー群同型です。 $G_2$ が単純に接続されている場合、$G_1$ から $G_2$ へのすべてのエタール写像は単射なので、$N = \{e\}$ になります。

#### 命題 5 {#lie-iii-s6-prop-5 .statement tag=0AEX}

*G を接続された実リー群とします。 $L(G)$ がその実正規正規数リー代数構造と互換性のある複素正規正規数リー代数構造 $L'$ を持つと仮定します。 G には、実リー群構造およびリー代数 $L'$ と互換性のある複合体リー群構造が 1 つだけ存在します。*

$§ 4$、no. 2、系 2 から定理 2 までにより、$L'$ の構造が Ad G の下で不変であることを証明するのに十分です。$\phi$ を G の指数写像とします。$§ 4$ により、 no. 4、系 3 (i) から命題 8 まで、$L(G)$ には 0 の近傍 V が存在し、$L'$ の構造は Ad $\phi(V)$ の下で不変です。ただし、G が接続されているため、Ad $\phi(V)$ 生成する G です。

G が接続されていると仮定されていない場合 (練習問題 7)、命題 5 の結論は必ずしも真ではありません。

#### 命題 6 {#lie-iii-s6-prop-6 .statement tag=0AEY}

*G を接続された複合体リー群とします。 G がコンパクトな場合、G は可換です。*

G の $\mathscr{L}(L(G))$ への正則写像 $g \mapsto \mathrm{Ad}\,g$ は定数 (*微分可能および解析的多様体*、R、3.3.7) であるため、すべての $a \in L(G)$ ($§ 3$、no. 12、命題 44) に対して $\mathrm{ad}\,a = 0$ です。したがって、G は可換です ($§ 4$, 系 3 から定理 1)。

### 4. 指数関数写像

#### 定理 4 {#lie-iii-s6-thm-4 .statement tag=0AEZ}

※Gをリー群とします。 $L(G)$ に定義された G の指数関数写像は 1 つだけ存在します。*

$L(G)$ に 0 の凸型の開いた近傍 U と、U 上で定義された G の指数関数写像が存在します。十分に小さい U を選択することで、次のように仮定できます。
$$
\phi((\lambda + \lambda')a) = \phi(\lambda a)\phi(\lambda'a)
$$
K では $a \in L(G)$、$\lambda, \lambda'$、U では $\lambda a, \lambda'a, (\lambda + \lambda')a$ です。

$a \in L(G)$ にしましょう。 $\frac{1}{n} a \in U$ となるような整数 $n > 0$ が存在します。 m が $\frac{1}{m} a \in U$ となるような他の整数である場合、$\frac{1}{nm} a \in U$ と関係 (1) は次のことを意味します。
$$
\phi\left(\frac{1}{n} a\right) = \left(\phi\left(\frac{1}{nm} a\right)\right)^m, \quad \phi\left(\frac{1}{m} a\right) = \left(\phi\left(\frac{1}{nm} a\right)\right)^n;
$$

したがって $\left( \phi \left( \frac{1}{n} a \right) \right)^n = \left( \phi \left( \frac{1}{m} a \right) \right)^m$ です。 $a \in L(G)$ に対して $\psi(a) = \left( \phi \left( \frac{1}{n} a \right) \right)^n$ となるような $\phi$ の拡大 $\psi : L(G) \to G$ と、$\frac{1}{n} a \in U$ となる$n$ 整数 $> 0$ が存在します。明らかに、$\psi$ は解析的であり、$G$ の指数関数写像です。 $\psi' : L(G) \to G$ が $G$ の指数関数写像である場合、0 の近傍上の $\psi$ と $\psi'$ 一致するは、$L(G)$ が接続されているため等しいです。

今後、$G$ の *指数関数写像* について話すときは、定理 4 で考慮された写像を意味します。混乱の危険がない場合は、$\exp_G$ または $\exp$ で表されます。

#### 例 {#lie-iii-s6-n4-exa-1 .statement tag=0AF0}

$A$ を完全な標準単位結合代数とします。このとき、$\exp_{A^*}$ は、章 II, § 7, no. 3 で定義された指数写像です。

#### 命題 7 {#lie-iii-s6-prop-7 .statement tag=0AF1}

※$G$を$L(G)$のリー群と$a$元とします。 The mapping $\lambda \mapsto \exp(\lambda a)$ of $K$ into $G$ is the unique morphism $\phi$ of the Lie group $K$ into $G$ such that $(T_0 \phi)1 = a$.

$K \times K$ から $G$ への写像 $(\lambda, \lambda') \mapsto \exp(\lambda a) \exp(\lambda' a)$ と $(\lambda, \lambda') \mapsto \exp(\lambda + \lambda') a$ は分析的であり、$(0, 0)$ の近傍では一致するです。 $K \times K$が繋がっているので、この写像は等しくなります。したがって、$\phi : \lambda \mapsto \exp(\lambda a)$ は、$K$ のリー群射が $G$ になります。 0 から $\lambda \mapsto \lambda a$ までの接線写像は写像 $\lambda \mapsto \lambda a$ です。そして$T_e(\exp) = \mathrm{Id}_{L(G)}$;したがって$(T_0 \phi)1 = a$です。 一意性主張の命題は定理 1 から続きます。*

#### 命題 8 {#lie-iii-s6-prop-8 .statement tag=0AF2}

※$G$をリー群とします。 $L(G)$ と $n$ 整数のすべての $x, y$ について、

$$
\exp(x + y) = \lim_{n \to + \infty} \left( \left( \exp \frac{1}{n} x \right) \left( \exp \frac{1}{n} y \right) \right)^n
$$

$$
\exp[x, y] = \lim_{n \to + \infty} \left( \left( \exp \frac{1}{n} x \right) \left( \exp \frac{1}{n} y \right) \left( \exp \frac{1}{n} x \right)^{-1} \left( \exp \frac{1}{n} y \right)^{-1} \right)^{n^2}.
$$

命題 7 までに、これは § 4, no. 3 の命題 4 から $\lambda = \frac{1}{n}$ を取って続きます。

#### 命題 9 {#lie-iii-s6-prop-9 .statement tag=0AF3}

*$G$を複合体リー群、$G'$をその基礎となる実リー群とします。それから$\exp_G = \exp_{G'}$。

これは、§ 4, no. 3 の命題 5 と、$\exp_G$ と $\exp_{G'}$ の分析から続きます。

#### 命題 10 {#lie-iii-s6-prop-10 .statement tag=0AF4}

※$G$と$H$を$G$のリー群と$\phi$射を$H$とします。
(i) $\phi \circ \exp_G = \exp_H \circ L(\phi)$。
(ii) *$G$ が $H$ の整数部分群である場合、$\exp_G = \exp_H | L(G)$。*

指数関数写像

等式 (i) の 2 つの辺は、$L(G)$ の $H$ への解析的な写像で、0 の近傍の一致する ($§ 4$、命題 8、no. 4) であるため、等しいです。 主張 (ii) は (i) の特殊なケースです。

#### 系 1 {#lie-iii-s6-prop-10-cor-1 .statement tag=0AF5}

*$G$をリー群、$G'$を$G$と$a \in L(G)$の嘘部分群とします。次の条件は同等です*:
(i) $a \in L(G')$;
(ii) すべての $\lambda \in K$ および $|\lambda|$ に対して $\exp(\lambda a) \in G'$ は十分に小さい。
(iii) $\lambda \in K$ 全員に対して $\exp(\lambda a) \in G$。
引数は、$§ 4$、no. 4、系 1 ～ 命題 8 のようになります。

#### 系 2 {#lie-iii-s6-prop-10-cor-2 .statement tag=0AF6}

*$G$をリー群、$H$を$G$と$a \in L(G)$の整数部分群とします。次の条件* を考慮してください。
(i) $a \in L(H)$;
(ii) $\lambda \in K$ 全員に対して $\exp_G(\lambda a) \in H$。
※では、(i)$\Rightarrow$(ii)となります。 $H$ の位相が可算基底を認める場合、(i) $\Leftrightarrow$ (ii)*。
$i$を$H$の標準単射を$G$とします。 $a \in L(H)$ の場合、
$$
\exp_G(\lambda a) = (\exp_G \circ L(i))(\lambda a) = (i \circ \exp_H)(\lambda a) \in H.
$$
したがって、(i) $\Rightarrow$ (ii) となります。 $H$ に可算数の基底がある場合、逆は命題 3 から続きます。

#### 系 3 {#lie-iii-s6-prop-10-cor-3 .statement tag=0AF7}

*$G$ をリー群、$\rho$ を $G$、$x \in L(G)$、$g \in G$ の分析線型表現とします。
(i) $\rho(\exp x) = \exp L(\rho)x$;
(ii) $\mathrm{Ad}(\exp x) = \exp \mathrm{ad}\, x$;
(iii) $g(\exp x)g^{-1} = \exp(\mathrm{Ad}\, g.x)$。
議論は$§ 4$、no. 4、系2と3から命題8のようになります。

#### 系 4 {#lie-iii-s6-prop-10-cor-4 .statement tag=0AF8}

*$G$を有限次元接続されたリー群*とします。
(i) $\mathrm{Int}(L(G)) = \mathrm{Ad}(G)$。
(ii) ※$Z$を$G$の中心とします。すると、$Z$は$G$の嘘部分群で、そのリー代数は$L(G)$の中心です。 移行～商がリー群同型*のとき、$G/Z$の写像を$g \mapsto \mathrm{Ad}\, g$から$\mathrm{Int}\, L(G)$に変換します。
主張 (i) は、系 3 (ii) および注意後で定義 2 から続きます。$g \in G$ とします。 位数の $\mathrm{Ad}\, g = \mathrm{Id}_{L(G)}$ では、$e$ ($§ 4$, no. 1, 定理 1 (ii)) の近傍で $\mathrm{Id}_G$ を伴う $\mathrm{Int}\, g$ 一致するが必要かつ十分です。 $G$;他の語では、$g \in Z$があれば十分です。次に (ii) は系 1 から命題 1 まで続きます。

#### 定義 3 {#lie-iii-s6-def-3 .statement tag=0AF9}

*$G$を有限次元接続されたリー群とします。 リー群 $\mathrm{Int}(L(G)) = \mathrm{Ad}(G)$ は、$G$* の随伴物群と呼ばれます。

#### 命題 11 {#lie-iii-s6-prop-11 .statement tag=0AFA}

*$G$を連結可換リー群*とします。
(i) *exp は、リー群 $L(G)$ を $G$* に加えたエタール射です。

(ii) *K = \mathbf{R} で G が有限次元の場合、G は形 $\mathbf{R}^p \times \mathbf{T}^q$ ($p, q$ 整数 $\geqslant 0$) のリー群と同型です。*

ハウスドルフ公式によれば、$x, y$ の $(\exp x)(\exp y) = \exp(x + y)$ は 0 に十分に近く、したがって解析継続による $L(G)$ のすべての $x, y$ についても同様です。したがって、$\exp$ は群準同型であり、étale です。

$$
T_e(\exp) = \mathrm{Id}_{L(G)}.
$$

したがって、(i)。 主張 (ii) は (i) と *一般位相*、章 VII, § 1、命題 9 から続きます。

#### 命題 12 {#lie-iii-s6-prop-12 .statement tag=0AFB}

※Gをリー群と$L = L(G)$とする。すべての $x \in L$ について、$T_x(L)$ を $L$ と同一視すると、$x$ における$\exp$ の右微分$\varpi(x)$ は、$L$ から$L$ への線形写像になります。 $x \in L$の皆様、

$$
\varpi(x) = \sum_{n \geqslant 0} \frac{1}{(n + 1)!} (\mathrm{ad}\ x)^n.
$$

両辺は $x$ の解析的写像であり、$x$ は 0 に十分近い (§ 4, no. 3, 命題 6) と等しくなります。

#### 注意 {#lie-iii-s6-n4-rem-1 .statement tag=0AFC}

$\varpi(x) \cdot (\mathrm{ad}\ x) = \exp \mathrm{ad}\ x - 1$。 記法の悪用によって、私たちは次のように書きます。

$$
\varpi(x) = \frac{\exp \mathrm{ad}\ x - 1}{\mathrm{ad}\ x}.
$$

#### 系 {#lie-iii-s6-n4-cor-1 .statement tag=0AFD}

*G を複素数リー群と $x \in L(G)$ とする。 $x$ から $\exp_G$ への接線写像は核 $\bigoplus_{n \in \mathbf{Z} - \{0\}} \mathrm{Ker}(\mathrm{ad}\ x - 2i\pi n)$ になります。

$z \neq 0$ の $\frac{e^z - 1}{z}$ に等しい積分写像 $z \mapsto \sum_{n \geqslant 0} \frac{1}{(n + 1)!} z^n$ は、$2\pi i \mathbf{Z} - \{0\}$ の零点として認められ、これらはすべて単純な零です。 系は、命題 12 と次の補題から続きます。

#### 補題 2 {#lie-iii-s6-lem-2 .statement tag=0AFE}

*E を複素バナッハ空間、u 元の $\mathscr{L}(E)$、S を $\mathscr{L}(E)$ (スペクトル理論、章 I, § 1, no. 2) の u のスペクトル、f を開いた近傍上の正則複素写像とします。 S の $\Omega$。 f が $\Omega$ において、多重度 $h_1, \ldots, h_n$ のうち、別個の零 $z_1, \ldots, z_n$ のうちの有限数のみを許容するとします。すると、$\mathrm{Ker}\ f(u)$は$1 \leqslant i \leqslant n$の$\mathrm{Ker}(u - z_i)^{h_i}$の直和になります。

($f(u)$ の定義については、スペクトル理論、章 I, § 4, no. 8 を参照してください。)

$\Omega$ には正則な写像 g が存在し、$f(z) = (z - z_1)^{h_1} \ldots (z - z_n)^{h_n} g(z)$ など、ゼロ以外の場所にはどこでも存在します。次に$g(u)g^{-1}(u) = g^{-1}(u)g(u) = 1$、したがって$\mathrm{Ker}\ f(u) = \mathrm{Ker} \prod_{i=1}^n (u - z_i)^{h_i}$となります。 $h \in \mathbf{C}[X]$、$x \in \mathrm{Ker}\ f(u)$ に対する外部法則 $(h, x) \mapsto h(u)x$ による $\mathrm{Ker}\ f(u)$ を $\mathbf{C}[X]$ モジュールとして考えると、*代数* を使用して、Ker $f(u)$ が $\mathrm{Ker}(u - z_i)^{n_i}$ の直和であることがわかります。 章 VII, § 2, no. 1、命題 1.

### 5. お申し込みは線型表現まで

#### 命題 13 {#lie-iii-s6-prop-13 .statement tag=0AFF}

*$G$ を接続されたリー群とし、$\varphi$ を完全正規化可能な空間 $E$ 上の $G$ の分析線型表現とします。 $E_1, E_2$ を、$E_2 \subset E_1$ となるように $E$ の 2 つの閉じたベクトル部分空間とします。次の条件は同等です:*

(i) すべての $g \in G$ およびすべての $x \in E_1$ に対して $\varphi(g)x \equiv x \pmod{E_2}$;
(ii) $L(\varphi)(L(G))$ 写像 $E_1$ を $E_2$ に変換します。

$$
\begin{align*}
&\varphi(g)x \equiv x \quad (\text{mod } E_2) \quad \text{for all } g \in G \text{ and all } x \in E_1 \\
\Leftrightarrow &\varphi(\exp a)x \equiv x \quad (\text{mod } E_2) \quad \text{for all } a \in L(G) \text{ and all } x \in E_1 \\
\Leftrightarrow &(\exp L(\varphi)a)x \equiv x \quad (\text{mod } E_2) \quad \text{for all } a \in L(G) \text{ and all } x \in E_1.
\end{align*}
$$

一方、$u \in \mathscr{L}(E)$ の場合、

$$
\begin{align*}
&\exp(\lambda u)x \equiv x \quad (\text{mod } E_2) \quad \text{for all } \lambda \in K \text{ and all } x \in E_1 \\
\Leftrightarrow &u(E_1) \subset E_2
\end{align*}
$$

よって命題。

#### 系 1 {#lie-iii-s6-prop-13-cor-1 .statement tag=0AFG}

*$E_1$が$\varphi$で安定するためには、$E_1$が$L(\varphi)$で安定することが必要かつ十分です。

命題13で$E_1 = E_2$を取れば十分です。

#### 系 2 {#lie-iii-s6-prop-13-cor-2 .statement tag=0AFH}

※$\varphi$が有限次元であると仮定します。 $\varphi$ が単純である (それぞれ半単純) ためには、$L(\varphi)$ が単純である (それぞれ半単純) ことが必要かつ十分です。*

これは系 1から続きます。

#### 系 3 {#lie-iii-s6-prop-13-cor-3 .statement tag=0AFI}

*$x \in E$にしておきます。 $x$が$\varphi(G)$の下で不変であるためには、$x$が$L(\varphi)(L(G))$によって消滅することが必要かつ十分です（つまり、$x$は、章、I, § 3、定義の意味で、$L(\varphi)$の下で不変であるということです） 3).*

命題 13の$E_1 = Kx$と$E_2 = 0$を取れば十分です。

#### 系 4 {#lie-iii-s6-prop-13-cor-4 .statement tag=0AFJ}

*$\varphi'$ を完全正規化可能な空間 $E'$ 上の $G$ の他のを分析的線型表現とします。 $T \in \mathscr{L}(E, E')$ にしましょう。次の条件は同等です:*

(i) $g \in G$ 全員に対して $T\varphi(g) = \varphi'(g)T$;
(ii) $a \in L(G)$ 全員に対して $TL(\varphi)(a) = L(\varphi')(a)T$。

$\varphi$と$\varphi'$から導出された$\mathscr{L}(E, E')$上の$G$の線型表現を$\sigma$とします（§ 3, no. 11、系1から命題41）。 条件 (i) は、$T$ が $\sigma(G)$ の下で不変であることを意味します。 条件(ii)は、$T$が$L(\sigma)(L(G))$によって全滅することを意味します。その場合、系を適用する 3 で十分です。

#### 系 5 {#lie-iii-s6-prop-13-cor-5 .statement tag=0AFK}

$\rho$ と $\rho'$ が有限次元であると仮定します。 $\rho$ と $\rho'$ が同等であるためには、 $L(\rho)$ と $L(\rho')$ が同等であることが必要かつ十分です。

これは系 4 の特殊なケースです。

#### 系 6 {#lie-iii-s6-prop-13-cor-6 .statement tag=0AFL}

$G$ が有限次元であると仮定します。 $t \in U(G)$ にしましょう。 $L_t$ (それぞれ $R_t$) が右 (それぞれ左) 不変であるためには、$U(G)$ の $t$ 属するから中心であることが必要かつ十分です。

$L_t$ (それぞれ $R_t$) が右 (それぞれ左) 不変であるためには、すべての $g \in G$ に対して $\varepsilon_g * t = t * \varepsilon_g$、つまり $(\mathrm{Int}\, g)_* t = t$ が必要かつ十分です。 $t \in U_n(G)$ となるような整数 $n$ が存在します。 § 3, no. 12 の系 3 と命題 45 により、すべての $a \in L(G)$ に対して $[a, t] = 0$ である場合に限り、つまり、$t$ が $U(G)$ と交換できる場合に限り、すべての $g \in G$ に対して $(\mathrm{Int}\, g)_* t = t$ になります。

### 6. 正規積分部分群

#### 補題 3 {#lie-iii-s6-lem-3 .statement tag=0AFM}

$G$ をリー群、$H_1$、$H_2$ の整数部分群とし、位相は可算の基底と $g \in G$ を許容します。それから

$$
g H_1 g^{-1} = H_2 \Leftrightarrow (\mathrm{Ad}\, g)(L(H_1)) = L(H_2).
$$

$\mathrm{Ad}\, g = T_e(\mathrm{Int}\, g)$。したがって、構造の輸送までに、$(\mathrm{Int}\, g)(H_1)$ はリー代数 $(\mathrm{Ad}\, g)(L(H_1))$ になります。 $H_1$ と $H_2$ は可算基底なので、集合 $H_2$ と $(\mathrm{Int}\, g)(H_1)$ はというに等しく、積分部分群 $H_2$ と $(\mathrm{Int}\, g)(H_1)$ は等しい (no. 2, 系 3 ～ 命題 3)。次に、定理 2 (i) から補題が続きます。

#### 命題 14 {#lie-iii-s6-prop-14 .statement tag=0AFN}

$G$ をリー群とし、$H$ を整数部分群とし、位相は可算基底を許容します。次の条件は同等です。
(i) $H$ は $G$ では正常です。
(ii) $L(H)$ は $\mathrm{Ad}(G)$ の下で不変です。
さらに $G$ が接続されている場合、これらの条件は以下と同等になります。
(iii) $L(H)$ は $L(G)$ の理想です。
さらに$G$が単純に接続され、$L(H)$が$L(G)$の有限余次元である場合、これらの条件は、$H$が$G$の嘘部分群であり、$G/H$が単純に接続されていることを意味します。

同値 (i) $\Leftrightarrow$ (ii) は補題 3 から続きます。 さらに$G$を接続すると、条件(ii)は、$L(H)$が$\mathrm{ad}\, L(G)$(no. 5、系1～命題13、§ 3, no. 12、命題44)で安定であるというと等価になります。

$G$を単純に結んで、$L(H)$が$L(G)$の有限余次元の理想であるとします。 no. 3 の定理 3 により、$L(G')$ が $L(G)/L(H)$ と同型となるように単純に接続されたリー群 $G'$ が存在します。 $L(G)$ から $L(G')$ に核 $L(H)$ が続く連続した射 $f$ が存在します。 no. 1の定理1により、$G$の$G'$には$L(\phi) = f$となる射$\phi$が存在します。 この射は水没であるため、その核 $N$ は $L(N) = \mathrm{Ker}\, f = L(H)$ となるような $G$ の嘘部分群です。 したがって、$H$ は $N$ の同一性成分であり、したがって G の嘘部分群です。 移行から商のとき、$\phi$から導かれる$G'$に$G/H$の射を$\psi$とします。 この射はエタールです。 G は単純に接続されているため、$\psi$ は $G'$ 上の $G/H$ の同型です。

#### 系 1 {#lie-iii-s6-prop-14-cor-1 .statement tag=0AFO}

*G を有限次元単純結合リー群とする。 m, h を、L(G) が m × h の半直接積となるように、L(G) の Lie 部分代数とします。 M, H を G の対応する積分部分代数とします。そのとき、M と H は単純に G の部分群に接続され、リー群として、G は H による M の半直接積です。

命題 14 までに、H は G の通常の嘘部分群であり、リー群 G/H は単純に接続されています。 $\pi$ を G から G/H への標準的な射とします。 M には、$L(\theta)$ が $L(M) = m$ 上の $L(G)/L(H) = L(G)/h$ の標準同型となるような G/H の射 $\theta$ が存在します。それから

$$
L(\pi \circ \theta) = L(\pi) \circ L(\theta) = \mathrm{Id}_{L(G/H)}
$$

したがって $\pi \circ \theta = \mathrm{Id}_{G/H}$ です。 no. 1、系 1 から命題 1、$\theta(G/H) = M$ まで。 § 1, no. 4の命題8により、MはGの嘘部分群であり、リー群GはHによるMの半直接積です。

#### 系 2 {#lie-iii-s6-prop-14-cor-2 .statement tag=0AFP}

*G を有限次元単純結合リー群、H を G の正規結合 Lie 部分群、および G の G/H への正規射を $\pi$ とします。

(i) $\pi \circ \varphi = \mathrm{Id}_{G/H}$ となるような G/H の G への解析的写像 $\varphi$ が存在します。

(ii) (i) の特性を持つすべての写像 $\varphi$ について、$H \times (G/H)$ の写像 $(h, m) \mapsto h \varphi(m)$ を G に変換すると、解析的多様体の同型になります。

(iii) H と G/H を単純に接続します。

$n = \dim G - \dim H$ にしましょう。 系は $n = 0$ にとって明らかです。 n について帰納法で議論します。

L(G) と L(H) とは異なる、L(G) 含む L(H) という理想が存在すると仮定します。 H' を G の対応するに接続された嘘部分群とします。$\pi_1 : G \to G/H'$ と $\pi_2 : H' \to H'/H$ を正規の射とします。 帰納法の仮定までに、$\pi_1 \circ \rho_1 = \mathrm{Id}_{G/H'}$、$\pi_2 \circ \rho_2 = \mathrm{Id}_{H'/H}$ などの分析的な写像 $\rho_1 : G/H' \to G$、$\rho_2 : H'/H \to H'$ が存在します。させて

$$
\pi_3 : G/H \to G/H'
$$

正規の射であること。 $x \in G/H$ で、y が G の x の代表である場合、y と $\rho_1(\pi_3(x))$ は同じ標準像モジュロ H' を持ち、したがって $x^{-1} \pi(\rho_1(\pi_3(x))) \in H'/H$ になります。させて

$$
\rho(x) = \rho_1(\pi_3(x)) \rho_2(\pi(\rho_1(\pi_3(x))))^{-1} x \in G.
$$

明らかに $\rho$ は G/H から G への解析写像であり、

$$
\pi(\rho(x)) = \pi(\rho_1(\pi_3(x))) \pi_2(\rho_2(\pi(\rho_1(\pi_3(x))))^{-1} x)) \\
= \pi(\rho_1(\pi_3(x))) \pi(\rho_1(\pi_3(x)))^{-1} x = x.
$$

ここで、L(G) 含む L(H) の唯一の理想が L(G) と L(H) である場合、リー代数 $L(G)/L(H)$ は 1 次元または単純です。どちらの場合も、$L(G)$ は $L(H)$ による部分代数の半直接積です。これは最初のケースでは明らかであり、2 番目のケースでは、章 I, § 6、系 3 から定理 5 に続きます。主張 (i) は、系 1 に続きます。

主張 (ii) は明らかです。 主張 (iii) は (i) と (ii) から続きます。

G が無限次元である場合、または H が正規でない場合 (練習問題 8 および 15)、系 2 の結論は必ずしも真ではなくなります。

#### 系 3 {#lie-iii-s6-prop-14-cor-3 .statement tag=0AFQ}

*G を有限次元接続リー群とし、H を G の通常接続 Lie 部分群とします。 $\pi_1(H)$ から $\pi_1(G)$ への標準射は単射法です。

$G_1$ を G と $G_1$ の $\lambda$ 標準写像を G 上に覆う普遍的なカバーとします。$G_1$ のリー代数は $L(G)$ と識別されます。 $G_1$ の嘘部分群 $\lambda^{-1}(H)$ は、$G_1$ では正常であり、そのリー代数は $L(H)$ です。 $H_1$ を $\lambda^{-1}(H)$ と $\lambda_1 = \lambda | H_1$ の同一性成分とします。次に、$L(H_1) = L(H)$、したがって$\lambda_1$ は、H への$H_1$ のエタール射です。一方、$H_1$ は単純に接続されているため (系 2)、したがって H の普遍的なカバーと同一視されます。その後、*一般位相* によって、章 XI、$\pi_1(H)$ から $\pi_1(G)$ への標準的な射は、Ker $\lambda_1$ から Ker $\lambda$ への標準単射と同一視されます。

### 7. リー代数の値との差分形のプリミティブ

#### 命題 15 {#lie-iii-s6-prop-15 .statement tag=0AFR}

*G をリー群、M 多様体の類 $C^r$ ($r \geq 2$)、および $\alpha$ を類 $C^{r-1}$ と次数 1 と M の差分形と値とします。 $L(G)$、そのような$d\alpha + [\alpha]^2 = 0$。 M が単純に接続されているとします。すべての $x \in M$ とすべての $s \in G$ に対して、M の類 $C^{r-1}$ を G に変換した $f(x) = s$ と $f^{-1} \cdot df = \alpha$ となる写像が 1 つだけ存在します。

f の一意性は、§ 3, no. 17、系 2 から命題 59 と M が接続されているという事実に続きます。 f の存在を証明します。 M のオープンカバー $(U_i)_{i \in I}$ と、$U_i$ に $g_i^{-1} \cdot dg = \alpha$ (§ 4, no. 6、定理 5) のような、$i \in I$、写像、類 $C^{r-1}$ の$g_i : U_i \to G$ が存在します。 § 3, no. 17、系 2 から命題 59 まで、$g_i g_j^{-1}$ は $U_i \cap U_j$ でローカルに一定です。 $g_i g_j^{-1} = g_{ij}$ にしましょう。 $G_d$ を離散位相を使用して群 G とします。 $g_{ij} : U_i \cap U_j \to G_d$は連続しており、$U_i \cap U_j \cap U_k$には$g_{ij} g_{jk} = g_{ik}$が続きます。 Mは単純につながっているので、$U_i \cap U_j$に$g_i g_j^{-1} = \lambda_i \lambda_j^{-1}$という連続した写像$\lambda_i : U_i \to G_d$が存在します。 g を M から G の写像とし、制限から $U_i$ はすべての $i \in I$ で $\lambda_i^{-1} g_i$ となります。この写像は類$C^{r-1}$と$g^{-1} dg = \alpha$のものです。 $f = s(g(x))^{-1} g$ によって定義される G への M の写像 f は、条件 $f^{-1} \cdot df = \alpha$ および $f(x) = s$ を満たします。

### 8. 無限小演算の法則から演算の法則への通過

#### 補題 4 {#lie-iii-s6-lem-4 .statement tag=0AFS}

*G を、X 上の G の左 (右) の演算のハウスドルフ トポロジ空間と $f_1, f_2$ 法則が接続されたトポロジカル群、X として、すべての $x \in X$、写像* $G$から$X$の$s \mapsto f_1(s, x),\ s \mapsto f_2(s, x)$は連続しています。 $G \times X$に$\{e\} \times X$の近傍$V$が存在し、$V$には$f_1$と$f_2$一致するが存在するとします。それから$f_1 = f_2$。

$x \in X$ と $A$ を $g \in G$ の集合とし、$f_1(g, x) = f_2(g, x)$ とします。その後、$A$は$G$で閉じられます。一方、$g \in A$; としましょう。 $y = f_1(g, x) = f_2(g, x)$と書きます。 $G$には$t \in U$に対して$f_1(t, y) = f_2(t, y)$となるように$e$の近傍$U$が存在し、他の語には$t' \in Ug$に対して$f_1(t', x) = f_2(t', x)$（それぞれ$gU$）が存在します。したがって、$A$ は $G$ にオープンし、したがって $A = G$ にオープンします。

#### 命題 16 {#lie-iii-s6-prop-16 .statement tag=0AFT}

G を、G の類 C^r のハウスドルフ多様体と左 (右それぞれ) の f_1、f_2 法則演算類 C^r を接続したリー群、X とします。 X。 f_1 と f_2 に関連付けられた微小な演算の法則が等しい場合、f_1 = f_2 になります。

§ 4, no. 7, 系から命題 11 までには、G \times X に \{e\} \times X の近傍 V が存在し、V に f_1 と f_2 一致するが成立します。したがって、f_1 = f_2 (補題 4)。

#### 補題 5 {#lie-iii-s6-lem-5 .statement tag=0AFU}

Let G be a simply connected topological group, X a Hausdorff topological space, U an open neighbourhood of e in G and \psi a continuous mapping of U \times X into X such that \psi(e, x) = x and \psi(s, \psi(t, x)) = \psi(st, x) for all x \in X and s, t in U such that st \in U. W を、W^3 \部分集合 U となるような e の対称接続オープン近傍とします。 X 上の G の連続左演算 \psi' の法則は、W \times X 上の \psi' と \psi 一致するが 1 つだけ存在します。 G が類 C^r のリー群および X 多様体で、\psi が類 C^r である場合、\psi' は類 C^r になります。

\psi の一意性は補題 4 から続きます。P を X の置換群とします。 u \in W^3 の場合、写像 x \mapsto \psi(u, x) は P の元 f(u) であり、

$$ f(u_1u_2u_3) = f(u_1)f(u_2)f(u_3) $$

W の u_1、u_2、u_3 について、no. 1 の適用補題 1 から、G の射 f' が P に得られ、拡大する f|W になります。 G \times X のすべての (g, x) \psi'(g, x) = f'(g)(x) とします。すると、\psi' は X 上の G の左演算の法則で、\psi on W \times X の一致するになります。 \psi'(g, \psi'(g', x)) = \psi'(gg', x) for (g, g', x) \in G \times G \times X として、 W \times X 上の \psi の連続性は、すべての g \in G に対する gW \times X 上の \psi' の連続性を意味します。 \psi' は連続です。 \psi が類 C^r である場合、\psi' は類 C^r であることが同様に見られます。

#### 定理 5 {#lie-iii-s6-thm-5 .statement tag=0AFV}

G を単純に接続されたリー群、X 類 C^r (r \geq 2) のコンパクト多様体と、類の左 (右) 無限小演算の \mapsto D_a 法則とします。 XのL(G)のC^{r-1}。 There exists one and only one law of left (resp. right) operation of class C^{r-1} of G on X such that the associated law of infinitesimal operation is a \mapsto D_a.

一意性は命題 16 から続きます。§ 4, no. 7、系 1 から定理 6 までに、G \times X と法則の \{e\} \times X の近傍 V が存在します。 V で定義された、X 上の G の左 (それぞれ右) 演算の類 C^{r-1} のチャンク。無限小演算の関連する法則は \mapsto D_a になります。 X はコンパクトなので、V は形 U × X であると仮定できます。ここで、U は G の e の開近傍です。その場合、補題 5 を適用するだけで十分です。

### 9. 線形群における指数関数写像

#### 命題 17 {#lie-iii-s6-prop-17 .statement tag=0AFW}

Δ を z ∈ C の集合とし、−π < J(z) < π および z ∈ C の Δ' 集合は実数 ≤ 0 ではありません。E を C および A (それぞれ A') 上の完全な正規化可能な空間とします。 集合 of x ∈ L(E)、そのスペクトル Sp(x) は Δ (それぞれ Δ') に含まれます。この場合、A (または A') は、L(E) (それぞれ GL(E)) の開部分集合であり、写像 exp: A → A' および log: A' → A (スペクトル理論、章 I, § 4, no. 9) は、解析的多様体の逆同型です。

これはスペクトル理論、章 I, § 4、命題 10、no. 9 から導き出されます。

#### 定理 6 {#lie-iii-s6-thm-6 .statement tag=0AFX}

E を実数または複素数のヒルベルト空間とし、U を E のユニタリー 群とします。

(i) L(E) のエルミート元の集合 H は、実ノルム空間構造とともに、トポロジー 補充を認める L(E) の閉じたベクトル部分空間です。

(ii) GL(E) の元 ≥ 0 の集合 H' は、GL(E) の実解析部分多様体です。

(iii) 写像 exp の H に対する制限は、H' に対する H の実解析的多様体の同型です。

(iv) GL(E) への H × U の写像 (h, u) ↦ (exp h)u は、実解析的多様体の同型です。

x ∈ L(E) の場合、x* は x の随伴を表すことを思い出してください。 H_1 を x ∈ L(E) の集合とし、x* = −x とします。 公式 x = $\frac{1}{2}(x + x^*) + \frac{1}{2}(x - x^*)$ は、その実ノルム空間構造により、L(E) が H と H_1, よって (i) のトポロジカル直和であることを証明します。

K = C と仮定します。 命題 17 の記法では、H' は、S h ⊂ R^*_+ となるような h ∈ H ∩ A' の集合です。 exp(R) = R^*_+ であるため、(ii) と (iii) は命題 17 とスペクトル理論、章 I, § 4、命題 8 および § 6, no. 5 から続きます。 H × U の GL(E) への写像 (h, u) ↦ y = (exp h)u は、スペクトル理論、章 I, § 6、命題 15 により全単射です。上記により、実際の解析的になります。 写像 y ↦ h = $\frac{1}{2} \log(y y^*)$ は実際の解析的であり、写像 y ↦ u = (exp h)^{-1}y も同様です。したがって、(iv)。

K = R とします。Ē を E の複素化ヒルベルト空間と、Ē の Ē への J 写像 ξ + iη ↦ ξ − iη (ξ、E の η の場合) を Ē とします。 Ũ, Ũ', Ũ は、E の H, H', U と同様に Ē に対して定義された集合を表すものとします。すると、H (それぞれ H', U) は、JxJ^{-1} = x となるように、x ∈ Ũ (それぞれ Ũ', Ũ) の集合と識別されます。特性 (ii)、(iii)、および (iv) は、(i) および複雑な場合の類似の特性から簡単に得られます。

#### 命題 18 {#lie-iii-s6-prop-18 .statement tag=0AFY}

E を、C、v ∈ L(E) および g = exp v 上の完全なノルマブル空間とします。Sp(v) 含むが n ∈ Z − {0} の点 2inπn のいずれでもないと仮定します。したがって、すべての x ∈ E について、条件 vx = 0 と gx = x は等価です。

これは、no. 4 の補題 2 から写像 z ↦ e^z − 1 に適用されます。

#### 系 1 {#lie-iii-s6-prop-18-cor-1 .statement tag=0AFZ}

*E を、$E^n$ から E への連続 n 線形写像の$\mathbf{C}$ および F 空間上の完全なノルマブル空間とする。すべての $v \in \mathscr{L}(E)$ について、$\sigma(v)$ を、* で定義される $\mathscr{L}(F)$ の元とする。

$$
(\sigma(v)f)(x_1, \ldots, x_n) = v(f(x_1, \ldots, x_n)) - \sum_{i=1}^n f(x_1, \ldots, vx_i, \ldots, x_n).
$$

*すべての $g \in \mathbf{GL}(E)$ について、$\rho(g)$ を * によって定義される $\mathbf{GL}(F)$ の元とします。

$$
(\rho(g)f)(x_1, \ldots, x_n) = g(f(g^{-1}x_1, \ldots, g^{-1}x_n)).
$$

*$u \in \mathscr{L}(E)$ を、すべての $z \in \mathrm{Sp}\,u$ が $|\mathscr{J}(z)| < \frac{2\pi}{n+1}$ を満たすようにします。したがって、すべての $f \in F$、条件、$\sigma(u)f = 0$、および $\rho(\exp u)f = f$ は等価です。*

$\mathbf{L}(\rho) = \sigma$ (§ 3, no. 11、系 1 ～ 命題 41)

$$
\rho(\exp u) = \exp \sigma(u)
$$

(no. 4、系 3 ～ 命題 10)。 命題 18 までに、$\mathrm{Sp}\,\sigma(u)$ が $2i\pi(\mathbf{Z} - \{0\})$ を満たさないことを証明すれば十分です。しかし、これは次の補題からわかります。

#### 補題 6 {#lie-iii-s6-lem-6 .statement tag=0AG0}

*$v \in \mathscr{L}(E)$ の場合、$\mathrm{Sp}\,\sigma(v) \subset \mathrm{Sp}\,v + \mathrm{Sp}\,v + \cdots + \mathrm{Sp}\,v$、和は $n+1$ 項です。*

私たち定義する元 $v_0, v_1, \ldots, v_n$ $\mathscr{L}(F)$ $f \in F$全員のために、

$$
\begin{align*}
(v_0f)(x_1, \ldots, x_n) &= v(f(x_1, \ldots, x_n)) \\
(v_if)(x_1, \ldots, v_n) &= -f(x_1, \ldots, vx_i, \ldots, x_n) \quad \text{for } 1 \leq i \leq n.
\end{align*}
$$

この場合、$\sigma(v) = \sum_{i=0}^n v_i$ と $v_i$ はペアごとに置換可能です。 A を、$v_i$ によって生成された$\mathscr{L}(F)$ の合計クローズ部分代数とします。それは可換です (*スペクトル理論*、章 I, § 1, no. 4) および $\mathrm{Sp}_{\mathscr{L}(F)} v' = \mathrm{Sp}_A v' \subset \sum_{i=0}^n \mathrm{Sp}\,v_i$ (*スペクトル理論*、章 I, § 3、命題 3 (ii))。さて、$\lambda \in \mathbf{C}$ が $v - \lambda$ が可逆である場合、明らかに $v_i - \lambda_i$ は可逆であり、したがってすべての $i$ について $\mathrm{Sp}\,v_i \subset \mathrm{Sp}\,v$ になります。

#### 系 2 {#lie-iii-s6-prop-18-cor-2 .statement tag=0AG1}

*E を $\mathbf{C}$ と $w \in \mathscr{L}(E)$ 上の完全正規数代数とする。すべての $z \in \mathrm{Sp}\,w$ が $|\mathscr{J}(z)| < \frac{2\pi}{3}$ を満たすとします。次の条件は同等です:*
(i) *w は E の導分;*
(ii) *exp w は E の自己同型です。*
これは、系 1 から E の $n = 2$ および $f$ 乗法に続きます。

#### 命題 19 {#lie-iii-s6-prop-19 .statement tag=0AG2}

E を $\mathbf{C}$、$v \in \mathscr{L}(E)$、および $g = \exp v$ 上の完全正規数空間とする。すべての $z \in \mathrm{Sp}\, v$ が $-\pi < \mathscr{J}(z) < \pi$ を満たすとします。すると、$E$ の閉じたベクトル部分空間 $E'$ ごとに、条件 $v(E') \subset E'$ と $g(E') = E'$ は等価になります。

条件 $v(E') \subset E'$ は $g(E') \subset E'$ と $g^{-1}(E') \subset E'$ を意味し、したがって $g(E') = E'$ を意味します。 $g(E') = E'$ だとします。 命題 17 の記法 $\Delta, \Delta'$ を使用します。 $\mathrm{Sp}\, v$ は $\Delta$ のコンパクトな部分集合であるため、$\mathrm{Sp}\, v \subset Q \subset \Delta$ のようなコンパクトな長方形 $Q = (a, b) \times (a', b')$ が存在します。 集合 $\Delta - Q$ が接続されています。したがって、$\mathrm{Sp}\, g \subset \exp Q \subset \Delta'$、集合 $\exp Q$ はコンパクトで、集合 $\Delta' - \exp Q$ は接続されます。後者含む $]-\infty, 0]$ の閉鎖、したがって

$$
(\Delta' - \exp Q) \cup ]-\infty, 0] = \mathbf{C} - \exp Q
$$

連結。 この場合、$\exp Q$ は凸多項式 (*スペクトル理論*、章 I, § 3、系 2 ～ 命題 9) であるため、$\Delta'$ で定義された写像 $\log$ は、次の $\mathscr{O}(\exp Q)$ では極限になります。 多項式関数 (*スペクトル理論*、章 I, § 4、命題 3)。 Hence $v = \log g$ is the limit in $\mathscr{L}(E)$ of elements of the form $P(g)$, where $P$ is a polynomial (*Spectral Theories*, Chapter I, § 4, Theorem 3). $P(g)(E') \subset E'$ であるため、$v(E') \subset E'$ となります。

#### 系 {#lie-iii-s6-n9-cor-1 .statement tag=0AG3}

E を、$\mathbf{C}$、$v \in \mathscr{L}(E)$、$g = \exp v$ 上の完全な正規化空間とする。すべての $z \in \mathrm{Sp}\, v$ が $-\frac{\pi}{2} < \mathscr{J}(z) < \frac{\pi}{2}$ を満たすとします。すると、$\mathscr{L}(E)$、条件、$gMg^{-1} = M$、$[v, M] \subset M$ の閉じたベクトル部分空間 M ごとに等価になります。

$F = \mathscr{L}(E)$、$g'$ を F から F への写像 $f \mapsto gfg^{-1}$ とし、$v'$ を F から F への写像 $f \mapsto [v, f]$ とします。そして、$g' = \exp v'$ (no. 4、系 3 から命題 10、そして§ 3, no. 11、系 1 ～ 命題 41)。 補題 6 は、すべての $z \in \mathrm{Sp}\, v'$ に対して $-\pi < \mathscr{J}(z) < \pi$ であることを証明します。その場合、命題を適用する 19 で十分です。

### 10. 有限次元実リー群の複素化

#### 補題 7 {#lie-iii-s6-lem-7 .statement tag=0AG4}

B を群、A を B の通常の部分群、C 群 $B/A$、$i : A \to B$ と $p : B \to C$ を正規の射とします。 $A'$を群、Aの$f$準同型を$A'$とします。 $\omega$をBの射から$A'$の自己同型群とします。 $a \in A'$、$a' \in A'$、$b \in B$ について、

$$
f\left(bab^{-1}\right) = \omega(b)f(a), \quad \omega(a)a' = f(a)a'f(a)^{-1}.
$$

$B''$ を $\omega$ に対する $A'$ による B の半直接積とし、q を B に対する $B''$ の正規射とします。

(i) $B''$ への A の写像 $a \mapsto (f(a^{-1}), i(a))$ は、$B''$ の通常の部分群 D への A の射です。 $B' = B''/D$と$i' : A' \to B'$、$g : B \to B'$を$A'$の射とし、$A'$の標準単射から商を取り、Bを$B''$にすると導き出されるBを$B'$とします。

(ii) The morphism $p \circ q$ of $B''$ into C defines when passing to the quotient a morphism of $B'$ into C.

(iii) $i'$ は単射、$p'$ は全射、$\mathrm{Ker}(p') = \mathrm{Im}(i')$ と次の図式は可換です

$$
\begin{array}{ccc}
A & \xrightarrow{i} & B \xrightarrow{p} C \\
f \downarrow & & g \downarrow \mathrm{Id}_C \\
A' & \xrightarrow{i'} & B' \xrightarrow{p'} C.
\end{array}
$$

(iv) *$b \in B$ および $a' \in A'$ の場合、
$$
g(b)i'(a')g(b)^{-1} = i'(\omega(b)a').
$$

(i) $A$ の $a_1, a_2$ について、$B''$ では、
$$
(f(a_1^{-1}), i(a_1))(f(a_2^{-1}), i(a_2)) = (f(a_1^{-1})(\omega(a_1)f(a_2^{-1})), i(a_1)i(a_2))
= (f(a_1^{-1})f(a_1a_2^{-1}a_1^{-1}), i(a_1a_2))
= (f((a_1a_2)^{-1}, i(a_1a_2))
$$
したがって、$a \mapsto (f(a^{-1}), i(a))$ は $A$ の準同型 $h$ から $B''$ になります。 $a \in A$、$a' \in A'$、$b \in B$ とします。その後、$B''$に、
$$
bh(a)b^{-1} = bf(a^{-1})ab^{-1} = (\omega(b)f(a^{-1}))(bab^{-1})
= f(ba^{-1}b^{-1})(bab^{-1}) = h(bab^{-1})
$$
$$
a'h(a){a'}^{-1} = a'f(a^{-1})a{a'}^{-1} = a'f(a^{-1})(\omega(a){a'}^{-1})a
= a'f(a^{-1})f(a){a'}^{-1}f(a^{-1})a = h(a)
$$
したがって、$B''$ では $h(A) = D$ が正常です。

(ii) $a \in A$ の場合、
$$
(p \circ q)(h(a)) = p(q(f(a^{-1})a)) = p(a) = e
$$
したがって、$p \circ q$ は $D$ では自明です。

(iii) $a' \in A'$ を $i'(a') = e$ となるようにします。次に $a' \in D$ となり、したがって $a' = f(a^{-1})a$ となる $a \in A$ が存在します。これは、$a = e$、よって $a' = e$ を意味します。したがって、$i'$ は単射法です。 $p$ と $q$ が全射であるように、 $p'$ も全射です。

$r$ は、$B''$ から $B'$ への正規の射を表すものとします。 $a' \in A'$、$b \in B$、$b' = r(a'b)$ とします。 $b' \in \mathrm{Im}(i')$ の場合、$b' = r(a'_1)$ となるような $a'_1 \in A'$ が存在します。次に、$a'b = a'_1f(a^{-1})a$、よって $b = a \in A$ などの $a \in A$ が存在します。
$$
p'(b') = p(q(a'b)) = p(b) = e;
$$
したがって、$\mathrm{Im}(i') \subset \mathrm{Ker}(p')$。 記法 $a', b, b'$ を保存しますが、$b' \in \mathrm{Ker}(p')$ と仮定します。次に $e = p'(b') = p(q(a'b)) = p(b)$、したがって $b \in A$、よって
$$
b' = r(a'f(b)f(b^{-1})b) = r(a'f(b)) \in \mathrm{Im}(i');
$$
したがって$\mathrm{Ker}(p') \subset \mathrm{Im}(i')$。

$a \in A$ の場合、
$$
i'(f(a)) = r(f(a)) = r(f(a)f(a^{-1})a) = r(a) = g(i(a)).
$$

$b \in B$ の場合、
$$
p'(g(b)) = p(b)
$$
したがって、図式 (4) は可換です。

(iv) $b \in B, a' \in A'$ とします。それから
$$
g(b)i'(a')g(b)^{-1} = r(b)r(a')r(b)^{-1} = r(ba'b^{-1})
= r(\omega(b)a') = i'(\omega(b)a').
$$

#### 命題 20 {#lie-iii-s6-prop-20 .statement tag=0AG5}

*G を有限次元実リー群とします。*

(i) *G の $\tilde{G}$ への複素数リー群 $\tilde{G}$ と $\mathbf{R}$-解析射 $\gamma$ が存在し、次の特性を持ちます: すべての複素数リー群 H とすべての $\mathbf{R}$-解析射 $\phi$ G を H に変換すると、$\phi = \psi \circ \gamma$ となるような H に $\tilde{G}$ の $\mathbf{C}$-分析的射 $\psi$ が 1 つだけ存在します。*

(ii) *If $(\tilde{G}', \gamma')$ has the same properties as $(\tilde{G}, \gamma)$, there exists one and only one isomorphism $\theta$ of $\tilde{G}$ onto $\tilde{G}'$ such that $\theta \circ \gamma = \gamma'$.*

(iii) *拡大する $L(\gamma)$ が全射である $L(G) \otimes \mathbf{C}$ から $L(\tilde{G})$ への *$\mathbf{C}$ 線形写像。特に $\dim_{\mathbf{C}}(\tilde{G}) \leq \dim_{\mathbf{R}}(G)$.*

主張 (ii) は明らかです。性質 (i) と (iii) を使用して、順序付けられた対 $(\tilde{G}, \gamma)$ の存在を証明します。

(a) まず G が接続されているとします。 Let $g = L(G)$, $g_C = g \otimes_{\mathbf{R}} \mathbf{C}$ be the complexification of g, S (resp. S') the simply connected real (resp. complex) Lie group with Lie algebra g (resp. $g_C$) and $\sigma$ the unique $\mathbf{R}$-analytic morphism of S into S' such that $L(\sigma)$ is the canonical injection of g into $g_C$. $\pi$ を、$L(\pi) = \mathrm{Id}_{L(G)}$ および F = Ker $\pi$ となるような G に対する S の一意の $\mathbf{R}$-分析射とします。

$$
\begin{array}{ccc}
S & \xrightarrow{\sigma} & S' \\
\downarrow \pi & & \downarrow \lambda \\
G & \xrightarrow{\gamma} & G \\
& \searrow \phi & \swarrow \psi \\
& & H
\end{array}
$$

すべての複素数リー群 H と G から H へのすべての $\mathbf{R}$-解析射 $\phi$ について、$L(\phi): g \to L(H)$ には一意の $\mathbf{C}$-線形拡大から $g_C$ があり、この拡大は形です$L(\phi^*)$、ここで、$\phi^*$ は S' を H に変換した $\mathbf{C}$-解析射です。
$$
L(\phi \circ \pi) = L(\phi) \circ L(\pi) = L(\phi) = L(\phi^*) \circ L(\sigma) = L(\phi^* \circ \sigma)
$$
したがって $\phi \circ \pi = \phi^* \circ \sigma$ です。したがって、$\phi^*(\sigma(F)) = \phi(\pi(F)) = \{e\}$、よって
$$
\sigma(F) \subset \mathrm{Ker}\, \phi^*.
$$
P を変数 $\phi$ の $\mathrm{Ker}\, \phi^*$ の共通部分とします。これは S' の通常の嘘部分群 (no. 2、系 3 ～ 命題 1) です。 $\tilde{G} = S'/P$ と λ: S' → Ġ を正規の射とします。すると σ(F) ⊂ P となり、γ ∘ π = λ ∘ σ となる G の Ġ への R 解析射 γ が 1 つだけ存在します。 ψ: Ġ → H が移行から商のときの φ* から導出された射を表す場合、

$$(\varphi \circ \gamma) \circ \pi = \psi \circ (\lambda \circ \sigma) = \varphi^* \circ \sigma = \varphi \circ \pi$$

よって ψ ∘ γ = φ。明らかに、L(ψ)、したがって ψ は、等式 ψ ∘ γ = φ によって一意に決定されます。したがって、順序付けされた対 (\tilde{G}, γ) には特性 (i) と (iii) があることが証明されました。

(b) ここで一般的なケースに移ります。 F を G の恒等式成分とし、M = G/F、i: F → G および p: G → M を標準射とします。 証明の部分 (a) を F に適用します。順序付けられた対 (\tilde{F}, δ) が得られます。すべての g ∈ G に対して、Int g|F = ω'(g) は F の自己同型です。 \tilde{F} の普遍性により、δ ∘ ω'(g) = ω(g) ∘ δ となるような複素数リー群 \tilde{F} の自己同型 ω(g) が 1 つだけ存在します。明らかに、ω は G の Aut(\tilde{H}) の射です。 g ∈ G かつ f ∈ F の場合、

$$\delta(gf g^{-1}) = (\delta \circ \omega'(g))(f) = (\omega(g) \circ \delta)(f) = \omega(g)(\delta(f)).$$

f ∈ F の場合、δ ∘ (Int_F f) = (Int_\tilde{F} δ(f)) ∘ δ および Int_\tilde{F} δ(f) は複素数リー群 \tilde{F} の自己同型です。したがって、Int_\tilde{F} δ(f) = ω(f) となります。

したがって、補題 7 を適用すると、図式が得られます。

$$
\begin{array}{ccccc}
F & \xrightarrow{i} & G & \xrightarrow{p} & M \\
\downarrow{\delta} & & \downarrow{\gamma} & & \downarrow{\mathrm{Id}} \\
\tilde{F} & \xrightarrow{\tilde{i}} & \tilde{G} & \xrightarrow{\tilde{p}} & M.
\end{array}
$$

\tilde{F} を ī を使って \tilde{G} の通常の部分群と識別するとします。 群 \tilde{G} は \tilde{F} と γ(G) によって生成されます。したがって、 \tilde{G} の元によって定義される \tilde{F} の自己同型は、複素数リー群構造の自己同型です。 § 1, no. 9, 命題 18 までに、\tilde{G} には 1 つだけの複合体リー群構造が存在し、\tilde{F} は \tilde{G} の開いた嘘部分群になります。今後、\tilde{G} には構造が付きます。 δ は R 解析的であるため、γ も R 解析的です。

順序付けられた対 (\tilde{G}, γ) には、命題の性質 (iii) が含まれます。 性質 (i) があることを示します。 H を複素数リー群とし、ψ を H への G の R 解析射とします。 η ∘ δ = φ|F となるような \tilde{F} の H への C 解析射 η が存在します。 g ∈ G とします。 写像

$$f \mapsto \eta(\omega(g)f), \quad f \mapsto \phi(g)\eta(f)\phi(g)^{-1}$$

\tilde{F} の H への変換は C-分析的射;それらは δ(F) 上で一致するです。 f' ∈ F の場合、

$$\phi(g)\eta(\delta(f'))\phi(g)^{-1} = \phi(g)\phi(f')\phi(g)^{-1} = \phi(gf'g^{-1})$$
$$= \eta(\delta(gf'g^{-1})) = \eta(\omega(g)\delta(f'));$$

したがって、すべての $g \in G$ とすべての $f \in \tilde{F}$ は $\eta(\omega(g)f) = \phi(g)\eta(f)\phi(g)^{-1}$ となります。 $G'$ が $\omega$ に対する $\tilde{F}$ による $G$ の半直接積を表す場合、群 $G'$ から $H$ への射 $\zeta$ が存在します。 一致するは $G$ に $\phi$ が、$\tilde{F}$ には $\eta$ が付きます。 $f \in F$の場合、
$$
\zeta(\delta(f^{-1})f) = \eta(\delta(f^{-1}))\phi(f) = \phi(f^{-1})\phi(f) = e.
$$
したがって、移行の$\zeta$ 定義するは、$\tilde{G}$の商射 $\psi$から$H$になります。次に$\psi \circ \gamma = \phi$と$\psi \circ \tilde{i} = \eta$。後者の不等式は、$\psi$が$\mathbf{C}$分析的であることを意味します。

最後に、$\psi'$ を、$\phi = \phi' \circ \gamma$ となるように、$\tilde{G}$ を $H$ に変換する $\mathbf{C}$ 分析射とします。それから
$$
\psi' \circ \tilde{i} \circ \delta = \psi' \circ \gamma \circ i = \phi \circ i = \psi \circ \tilde{i} \circ \delta
$$
したがって $\psi' \circ \tilde{i} = \psi \circ \tilde{i}$ です。 $\tilde{G}$は$\tilde{i}(\tilde{F})$と$\gamma(G)$によって生成されるので、$\psi' = \psi$。

#### 定義 4 {#lie-iii-s6-def-4 .statement tag=0AG6}

$(G, \gamma)$、または単に $\tilde{G}$ は、$G$ の普遍的複雑化と呼ばれます。

#### 注意 {#lie-iii-s6-n10-rem-1 .statement tag=0AG7}

(1) $(\tilde{G}, \gamma)$ を $G$ の普遍複素数とします。 $G_0$ (それぞれ $\tilde{G}_0$) を $G$ (それぞれ $\tilde{G}$) の同一性成分とします。 命題 20 の証明により、$(\tilde{G}_0, \gamma|G_0)$ は $G_0$ と合成射の普遍的な複雑化です。
$$
G \to \tilde{G} \to \tilde{G}/\tilde{G}_0
$$
移行の定義するから$G/G_0$の商、$\tilde{G}/\tilde{G}_0$の同型。

(2) $G$ が単純に接続されているとします。 Let $g = L(G)$, $g_C$ be the complexification of $g$, $S'$ the simply connected complex Lie group with Lie algebra $g_C$ and $\sigma$ the morphism of $G$ into $S'$ such that $L(\sigma)$ is the canonical injection of $g$ into $g_C$. 再び命題 20、部分の証明の記法を使用します (a)。 $H = S'$ と $\phi = \sigma$ の場合、$\phi^* = \mathrm{Id}_{S'}$。 したがって、$(S', \sigma)$ は $G$ の普遍的な複素化です。 $\sigma$ は一般に単射ではないことに注意してください (練習問題 16)。ただし、$L(\sigma)$ は単射なので *その核は離散* です。 一方、$\theta$ を $g$ によって定義される $g_C$ の畳み込みとし、$\eta$ を $S'$ の基礎となる実リー群の対応する自己同型とします。 ${S'}^\eta$ を $\eta$ の下で不変である $S'$ の点の集合とします。それは、リー代数 $g$ (§ 3, no. 8、系 1 ～ 命題 29) を含む $S'$ の部分群という本当の嘘です。 By no. 1, Corollary 1 to Proposition 1, $\sigma(G)$ is a real integral subgroup of $S'$ with Lie algebra $g$ and hence $\sigma(G)$ *is the identity component of* ${S'}^\eta$; in particular $\sigma(G)$ is a real Lie subgroup of $S'$.

### 練習問題 {#lie-iii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
