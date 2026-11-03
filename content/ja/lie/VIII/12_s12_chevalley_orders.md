---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 12
section_title: Chevalley orders
lang: ja
source: lie-vii-ix
book_pages: 173-189
pdf_pages: 0181-0197
extraction: native
subsections:
    - "no": 1
      title: LATTICES AND ORDERS
      page: 173
      pdf_page: 181
    - "no": 2
      title: DIVIDED POWERS IN A BIGEBRA
      page: 173
      pdf_page: 181
    - "no": 3
      title: INTEGRAL VARIANT OF THE POINCARÉ-BIRKHOFF-WITT THEOREM
      page: 174
      pdf_page: 182
    - "no": 4
      title: 'EXAMPLE: POLYNOMIALS WITH INTEGER VALUES'
      page: 176
      pdf_page: 184
    - "no": 5
      title: SOME FORMULAS
      page: 178
      pdf_page: 186
    - "no": 6
      title: BIORDERS IN THE ENVELOPING ALGEBRA OF A SPLIT REDUCTIVE LIE ALGEBRA
      page: 180
      pdf_page: 188
    - "no": 7
      title: CHEVALLEY ORDERS
      page: 185
      pdf_page: 193
    - "no": 8
      title: ADMISSIBLE LATTICES
      page: 187
      pdf_page: 195
statements: 34
exercises: 0
content_sha256: bd828896b990c5e64e8dd8e6a4c2f919e15761f051eecd5f7776a10a94e355e3
translated_from: content/en/lie/VIII/12_s12_chevalley_orders.md
translation_method: google
source_content_sha256: 50f43a34a9ae42cb38e10e1f32022dc1fddb5d2b07911570fec5baa09a40ebdf
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 1c6f7775285e7d7783f9e04e3d9baed035e71771cb5a4146e8f2684071fcd9ce
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 12。シュバレー 位数

### 1. 格子と位数

V を $\mathbf{Q}$ ベクトル空間とします。 V の格子は、$\mathscr{V}$ の単射によって V に誘導される $\mathbf{Q}$ 線形写像 $\alpha_{\mathscr{V},V}:\mathscr{V}\otimes_{\mathbf{Z}}\mathbf{Q}\rightarrow V$ が全単射であるような、V の自由 $\mathbf{Z}$ サブモジュール $\mathscr{V}$ です。 V が有限次元である場合、これは、$\mathscr{V}$ が $\mathbf{Q}$ ベクトル空間 V を生成する有限タイプの $\mathbf{Z}$ サブモジュールであると言っているのと同じです (有限タイプのねじれのない $\mathbf{Z}$ モジュールは代数、第 3 章によって自由であることを思い出してください)。 VII, §4, no. 4、コリント 2)。さらに、この場合、私たちの定義は可換代数の定義の特殊なケースです。 VII, §4, no. 1、デフォルト。 １（上記引用、例３）。 W が V のベクトル部分空間で、$\mathscr{V}$ が V の格子である場合、$\mathscr{V}\cap W$ は W の格子です。

V が $\mathbf{Q}$-代数である場合、V の位数は、基礎となるベクトル空間の格子 $\mathscr{V}$ であり、V の $\mathbf{Z}$-部分代数です。 写像 $\alpha_{\mathscr{V},V}$ は、$\mathbf{Q}$-代数の同型になります。 V がユニタル $\mathbf{Q}$-代数である場合、V のユニタル位数は、V 含む単位元の位数です。

V が余積 $c$ と余単位 $\gamma$ を持つ $\mathbf{Q}$-bigebra であると仮定します。 $\mathscr{V}$ がベクトル空間 V の格子である場合、正規の写像 $i:\mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V}\rightarrow V\otimes_{\mathbf{Q}}V$ は単射です。 V の双順序は、代数 V の単位位数 $\mathscr{V}$ で、$\gamma (\mathscr{V})\subset \mathbf{Z}$ と $c(\mathscr{V})\subset i(\mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V})$ になります。 写像

$\gamma_{\mathscr{V}}:\mathscr{V}\rightarrow \mathbf{Z}$ と $c_{\mathscr{V}}:\mathscr{V}\rightarrow \mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V}$

$\gamma$ と $c$ によって誘導されると、$\mathbf{Z}$-bigebra の $\mathscr{V}$ 構造が得られ、写像 $\alpha_{\mathscr{V},V}$ は $\mathbf{Q}$-bigebra の同型になります。

### 2. bigebra で冪を分割

A をユニタル $k$-代数、$x\in A,d\in k,n\in \mathbf{N}$ とします。置く

$$
x(x-d). . .(x-d(n-1))^{n-1}
$$

$$
x^{(n,d)}==\prod(x-id)/(i+ 1) \tag{1}
$$

$n$!

$i=0$

特に$x^{(0,d)}= 1,x^{(1,d)}=x$。私たちは、$n$ 整数 $<0$ に対して $x^{(n,d)}= 0$ に同意します。置く

$x^{(n)}=x^{(n,0)}=xn^n$! (2)

$(nx)=x^{(n,1)}=x(x-1). . .n($!$x-n+ 1)$。 (3)

#### 命題 1 {#lie-viii-s12-prop-1 .statement tag=017V}

A を余積 $c$ と $x$ を A の原始関数元 (第 II, §1, no. 2 章) とする双眼鏡とします。

$$
c(x^{(n,d)}) =\sum x^{(p,d)}\otimes x^{(q,d)} \tag{4}
$$

$p\in \mathbf{N},q\in \mathbf{N},p+q=n$

$n\leq 0$ にとって命題は簡単です。 $n$について帰納法までに議論します。 公式 (4) が $n$ に対して真である場合、

$$
(n+ 1)c(x^{(n+1,d)}) =c(x-dn)c(x^{(n,d)})
$$

$$
= (x\otimes 1 + 1\otimes x-dn1\otimes 1)c(x^{(n,d)})
$$

$$
=\sum_{p+q=n}[xx^{(p,d)}\otimes x^{(q,d)}+x^{(p,d)}\otimes xx^{(q,d)}-(p+q)dx^{(p,d)}\otimes x^{(q,d)}]
$$

$$
=\sum_{p+q=n}(x-pd)x^{(p,d)}\otimes x^{(q,d)}+\sum_{p+q=n}x^{(p,d)}\otimes (x-qd)x^{(q,d)}
$$

$$
=\sum_{p+q=n}(p+ 1)x^{(p+1,d)}\otimes x^{(q,d)}+\sum_{p+q=n}(q+ 1)x^{(p,d)}\otimes x^{(q+1,d)}
$$

$$
=\sum_{r+s=n+1}rx^{(r,d)}\otimes x^{(s,d)}+\sum_{r+s=n+1}sx^{(r,d)}\otimes x^{(s,d)}
$$

$$
= (n+ 1)\sum_{r+s=n+1}x^{(r,d)}\otimes x^{(s,d)}
$$

したがって、$n+ 1$ の場合は公式 (4) となります。

### 3. ポアンカレ-バークホフ-ウィットの整数型バリアント定理

$\mathfrak{g}$ を有限次元の $\mathbf{Q}$-リー代数、$U(\mathfrak{g})$ を包む双数とします。 I が完全に順序付けられた集合、$\mathbf{x}= (x_i)_{i\in I}$ が $\mathfrak{g}$ の元のファミリー、および $\mathbf{n}=$ $(n_i)_{i\in I}\in \mathbf{N}^{(I)}$ が複数のインデックスである場合、次のようにします。

$\mathbf{x}^{(\mathbf{n})}=\prod x\overset{ni}{n_{i}}$!$^{^i}$、(5)

$i\in I$

積は、注文された集合 I に従って $U(\mathfrak{g})$ で計算されます。

#### 定理 1 {#lie-viii-s12-thm-1 .statement tag=017W}

$\mathscr{U}$ を大角$U(\mathfrak{g})$ の双順序とします。 リー代数 $\mathfrak{g}$ の位数を $\mathscr{G}=\mathscr{U}\cap \mathfrak{g}$ とします。 $(x_i)_{i\in I}$を$\mathscr{G}$の基底とします。 I に合計位数を与え、$\mathscr{U}$ のすべての $\mathbf{n}\in \mathbf{N}^I$、元 $[\mathbf{n}]$ について、$[\mathbf{n}]-\mathbf{x}^{(\mathbf{n})}$ が $U(\mathfrak{g})$ で濾過$<|\mathbf{n}|$ を持つように与えられると仮定します。すると、$\mathbf{n}\in \mathbf{N}^I$ の$[\mathbf{n}]$ のファミリーは、$\mathbf{Z}$ モジュール $\mathscr{U}$ の基底になります。

For $p\in \mathbf{N}$, let $U_p(\mathfrak{g})$ be the set of elements of $U(\mathfrak{g})$ of filtration $\leq p$; then the images in $U_p(\mathfrak{g})/U_{p-1}(\mathfrak{g})$ of the $\mathbf{x}^{(\mathbf{n})}$ such that $|\mathbf{n}|=p$ form a basis of this $\mathbf{Q}$-vector space (Chap. I, §2, no. 7, Th. 1); hence the $[\mathbf{n}]$ form a basis of the $\mathbf{Q}$-vector space $U(\mathfrak{g})$. 次の主張 (ここに$M =\mathbf{N}^I$)$:$ を証明することが残っています。

(*) $u\in \mathscr{U}, (a_{\mathbf{n}})\in \mathbf{Z}^{(M)}$ と $d\in$ **N --**$\{0\}$ が次のような場合

$$
du=\sum_{\mathbf{n}\in M}a_{\mathbf{n}}[\mathbf{n}] \tag{6}
$$

次に、$d$ 割るがそれぞれ $a_{\mathbf{n}}$ となります。

それぞれの整数 $r\geq 0$ に対して、反復された余積を導入します。

$$
c_i:\mathscr{U}\rightarrow \mathbf{T}^r(\mathscr{U}) =\mathscr{U}\otimes \mathscr{U}\otimes  \cdots  \otimes \mathscr{U}
$$

定義により、$c_0$ は $\mathscr{U},c_1=$ Id$_{\mathscr{U}},c_2=c$ の余単位 ($\mathscr{U}$ の余積) であり、$r\geq 2,c_{r+1}$ については複合 $p\circ (c_r\otimes 1)\circ c:$ として定義されます。

$$
\mathscr{U}\longrightarrow^c\mathscr{U}\otimes_{\mathbf{Z}}\mathscr{U}^c\longrightarrow^{^r\otimes 1}\mathbf{T}^r(\mathscr{U})\otimes_{\mathbf{Z}}\mathscr{U}\longrightarrow^p\mathbf{T}^{r+1}(\mathscr{U})
$$

ここで、$p$ は、代数 $\mathbf{T}(\mathscr{U})$ の乗法を使用して定義されます。さらに、$\mathscr{U}^+=$ Ker $c_0$ に対する $\mathscr{U}$ の正規射影 $\pi$ とその合成を考えてみましょう。

$$
c^+_r=\mathbf{T}^r(\pi )\circ c_r:\mathscr{U}\rightarrow \mathbf{T}^r(\mathscr{U}^+)
$$

#### 補題 1 {#lie-viii-s12-lem-1 .statement tag=017X}

$\mathbf{n}\in \mathbf{N}^I$ にしましょう。 $|\mathbf{n}|< r$ の場合は、$c^+_r([\mathbf{n}]) = 0$ です。 $|\mathbf{n}|=r$ の場合、

$$
c^+_r([\mathbf{n}]) =\sum_{\varphi}x_{\varphi(1)}\otimes x_{\varphi(2)}\otimes  \cdots  \otimes x_{\varphi(r)} \tag{7}
$$

ここで、$\varphi$ 属するから集合の写像は、$\{1,2, . . . , r\}$ から I までで、それぞれ値 $i\in In_i$ 回かかります。

提案 1 により、

$$
c_r(\mathbf{x}^{(\mathbf{n})}) =\sum\mathbf{x}^{(\mathbf{p}_1)}\otimes  \cdots  \otimes \mathbf{x}^{(\mathbf{p}_r)}
$$

ここで、M の数列 $(\mathbf{p}_1, . . . ,\mathbf{p}_r)$ の $r$ 元の集合の合計拡大するは $\mathbf{p}_1+\cdots +\mathbf{p}_r=\mathbf{n}$ になります。章の観点から。 II, §1, no. 3、提案6、写像 $c^+_r$は、$U(\mathfrak{g})$から$\mathbf{T}^r(U^+(\mathfrak{g}))$まで線形性によって写像まで拡張され、$U_{r-1}(\mathfrak{g})$に消滅します。したがって、$r\geq  |\mathbf{n}|$ については、

$$
c^+_r([\mathbf{n}]) =c^+_r(\mathbf{x}^{(\mathbf{n})}) =\sum\pi (\mathbf{x}^{(\mathbf{p}_1)})\otimes  \cdots  \otimes \pi (\mathbf{x}^{(\mathbf{p}_r)}) \tag{8}
$$

$r >|\mathbf{n}|$、関係 $\mathbf{p}_1+\cdots +\mathbf{p}_r=\mathbf{n}$ は、$\mathbf{p}_i$ の少なくとも 1 つが零、つまり $c^+_r([\mathbf{n}]) = 0$ であることを意味します。 $r=|\mathbf{n}|$ の場合、(8) の 3 番目のメンバーの唯一の非ゼロ項は、$|\mathbf{p}_1|=\cdots =|\mathbf{p}_r|= 1$ となるものであるため、(7) になります。

Th の証明に戻ります。 1. (*) の記法を保持し、$|\mathbf{n}|$ で帰納法を降下することにより、$d$ 割る $a_{\mathbf{n}}$ であることを証明します。これは、$|\mathbf{n}|$ が十分大きいである場合に明らかです。 $|\mathbf{n}|> r$ に対して $d$ 割る $a_{\mathbf{n}}$ の場合、

$$
u'=u-\sum_{|\mathbf{n}|>r}(a_{\mathbf{n}}/d)[\mathbf{n}]\in \mathscr{U}
$$

私たちは持っています

$$
du'=\sum_{|\mathbf{n}|\leq r}a_{\mathbf{n}}[\mathbf{n}] \tag{9}
$$

$\{1,2, . . . , r\}$ から I までの写像 $\varphi$ については、

$$
e_{\varphi}=x_{\varphi(1)}\otimes  \cdots  \otimes x_{\varphi(r)}
$$

そして$a_{\varphi}=a_{\mathbf{n}}$ $\mathbf{n}=$ (カード$\varphi^{-1}(i)$)$_{i\in I}$。 補題 1 により、(9) は次のことを意味します。

$$
dc^+_r(u') =\sum_{\varphi\in I^r}a_{\varphi}e_{\varphi} \tag{10}
$$

だから$c^+_r(u')\in \mathbf{T}^r(\mathscr{U}^+)\cap \mathbf{Q}\mathbf{T}^r(\mathscr{G})$。 しかし、$\mathscr{U}^+$ の部分加群 $\mathscr{G}$ は直因子 (代数、Chap. VII, §4, no. 3、Th. 1 の Cor.) であるため、部分加群 $\mathbf{T}^r(\mathscr{G})$ は $\mathbf{T}^r(\mathscr{U}^+)$ の直因子、したがって $c^+_r(u')\in \mathbf{T}^r(\mathscr{G})$ です。 一方、$\mathscr{G}$の$x_i$ 形基底は仮定によるので、$\mathbf{T}^r(\mathscr{G})$の$e_{\varphi}$ 形基底です。 次に、(10) は $d$ 割るが $a_{\varphi}$、つまり $|\mathbf{n}|=r$ の $a_{\mathbf{n}}$ であることを証明します。 これは(*)を証明します。

### 4. 例: 整数値の多項式

Vを有限次元の$\mathbf{Q}$ベクトル空間、$V^*$をその双対、$\mathscr{V}$をVの格子、$\mathscr{V}^*$を$\mathscr{V}$の双対$\mathbf{Z}$加群とし、$V^*,\mathbf{S}(V)$の格子で正規に識別できるものとします。 V の対称的な代数、および

$$
\lambda :\mathbf{S}(V)\rightarrow A(V^*)
$$

$V^*($代数の多項式関数の$\mathbf{S}(V)$から代数までの正規全単射、第4章。 IV, §5, no. 11、注意 1)。 $A(V^*)\otimes_{\mathbf{Q}}A(V^*)$ で同一視する $A(V^*\times V^*)$ を計算すると、$\mathbf{S}(V)$ の $\lambda$ 変換余積が写像 $A(V^*)\rightarrow A(V^*\times V^*)$ になり、$V^*$ の多項式関数 $\varphi$ に関連付けられます。 多項式関数

$$
(x, y) \rightarrow \varphi (x+y)
$$

$V^*\times V^*($代数、章。 IV, §5, no. 11、注意 2)。

$\mathbf{S}(V)$ からなるの元の $(^{\mathscr{V}}_{\mathbf{Z}})$ 部分集合で、対応するを $V^*$ から $\mathbf{Q}$ までの多項式写像に変換し、$\mathscr{V}^*$ で整数値をとります。

#### 命題 2 {#lie-viii-s12-prop-2 .statement tag=017Y}

(i) $(^{\mathscr{V}}_{\mathbf{Z}})$ は、bigebra $\mathbf{S}(V)$ および $(^{\mathscr{V}}_{\mathbf{Z}})\cap V =\mathscr{V}$ の双順序です。

(ii) $\mathbf{Z}$-代数 $(^{\mathscr{V}}_{\mathbf{Z}})$ は $h\in \mathscr{V}, n\in \mathbf{N}$ に対する $(^h_n)$ によって生成されます。

(iii) $(h_1, . . . , h_r)$ が $\mathscr{V}$ の基底の場合、元

$$
(h)(h_1)(h_r)
$$

= $\cdots$、

$$
\mathbf{n}n_1n_r
$$

ここで、$\mathbf{Z}$ モジュール $(^{\mathscr{V}}_{\mathbf{Z}})$ の $\mathbf{n}= (n_1, . . . , n_r)$ 属するから $\mathbf{N}^r$、形基底です。

$m\in \mathbf{N}$には、$\mathbf{S}_m(V) =\sum_{i\leq m}\mathbf{S}^i$(V)、$\mathbf{S}_m(\mathscr{V}) =\sum_{i\leq m}\mathbf{S}^i(\mathscr{V})$を入れます。 代数章、 IV, §5, no. 9、提案 15 および注意、

$\mathbf{S}_m(\mathscr{V})\subset \mathbf{S}_m(V)\cap (\mathscr{V}\mathbf{Z})\subset m1$!$\mathbf{S}_m(\mathscr{V})$

だから$(^{\mathscr{V}}_{\mathbf{Z}})\cap V =\mathscr{V}$。 $\mathbf{S}_m(\mathscr{V})$は$\mathbf{S}_m$(V)の格子であるため、$\mathbf{S}_m(V)\cap (_{\mathbf{Z}}^{\mathscr{V}})$は$\mathbf{S}_m(V)$の格子でもあります。一方、$\mathbf{S}_m(V)\cap (^{\mathscr{V}}_{\mathbf{Z}})$ は $\mathbf{S}_{m+1}(V)\cap (_{\mathbf{Z}}^{\mathscr{V}})$ の直因子であるため (商にはねじれがないため)、自由な $\mathbf{Z}$ 加群である補数が認められます。したがって、$(^{\mathscr{V}}_{\mathbf{Z}})$ は無料の $\mathbf{Z}$ モジュールです。これが代数 $\mathbf{S}(V)$ の単位位数であることは明らかです。 $(u_n)_{n\in\mathbf{N}}$ を $\mathbf{Z}$ モジュール $(^{\mathscr{V}}_{\mathbf{Z}})$ の基底とします。これは、$\mathbf{Q}$ モジュール $\mathbf{S}(V)$ の基底です。

$$
\varphi \in \mathbf{S}(V\times V) =\mathbf{S}(V)\otimes_{\mathbf{Q}}\mathbf{S}(V)
$$

$\varphi =\sum u_n\otimes v_n$ のような、$\mathbf{S}(V)$ の元の固有の数列 $(v_n)$ が存在します。上記と同様に、$A(V^*)$では同一視する $\mathbf{S}(V)$、$A(V^*\times V^*)$では$\mathbf{S}(V)\otimes \mathbf{S}(V)$となります。 $\varphi \in (^{\mathscr{V}\times\mathscr{V}}_{\mathbf{Z}})$の場合、$y\in \mathscr{V}^*$すべてに対して多項式関数 $x \rightarrow \varphi (x, y)$ 属するから$(^{\mathscr{V}}_{\mathbf{Z}})$になります。したがって、すべての $n$ とすべての $y\in \mathscr{V}^*$ については $v_n(y)\in \mathbf{Z}$ となり、他の語では $v_n\in (^{\mathscr{V}}_{\mathbf{Z}})$ となります。これは、余積写像 $(^{\mathscr{V}}_{\mathbf{Z}})$ ～ $(_{\mathbf{Z}}^{\mathscr{V}})\otimes_{\mathbf{Z}}(_{\mathbf{Z}}^{\mathscr{V}})$ であることを証明します。 $h\in \mathscr{V}$と$n\in \mathbf{N}$なら、$(_n^h)$ 写像 $u\in \mathscr{V}^*$から整数 $(^{u(h)}_n)$なので、$(^h_n)\in (_{\mathbf{Z}}^{\mathscr{V}})$になります。 主張 (iii) は、適用 Th によって取得されます。 1 から可換リー代数 V に、(ii) が続きます。

#### 系 {#lie-viii-s12-n4-cor-1 .statement tag=017Z}

X を不定値とします。多項式 $(^X_n)$、多項式 $P\in k[X]$ の $\mathbf{Z}$ モジュールからなるの $n\in \mathbf{N}$、形基底は、$P(\mathbf{Z})\subset \mathbf{Z}$ になります。

$P(\mathbf{Z})\subset \mathbf{Z}$ の場合、ラグランジュ補間公式 (代数、章 IV, §2, no. 1、提案 6) は、P 属するから $\mathbf{Q}$ の係数を示します。したがって、$k=\mathbf{Q}$ を仮定し、$V =\mathbf{Q},\mathscr{V}=\mathbf{Z}$ で提案 2 を適用できます。

### 5. 一部公式

この数において、Aは単位結合代数を表します。 $x\in A$ の場合、広告$_Ax$ の代わりに広告 $x$ と書きます。

#### 補題 2 {#lie-viii-s12-lem-2 .statement tag=0180}

$x, y\in A$ と $n\in \mathbf{N}$ の場合、

(広告$nx$! )$^ny=\sum(-1)^qxp^p$! $yxq^q$! = $\sum(-1)^qx^{(p)}yx^{(q)}$。 (11)

$p+q=np+q=n$

実際、A から A まで $L_x$ と $R_x$ 写像 $z \rightarrow xz$ と $z \rightarrow zx$ で表すと、 $L_x$ と $R_x$ は通勤するので、

$n1$!(広告$x$)$^n=n1$!$(L_x-R_x)^n=\sum_{p+q=n}(-1)^qp1$! $L^p_xq1$! $R^q_x$。

#### 補題 3 {#lie-viii-s12-lem-3 .statement tag=0181}

$x, h\in A$ と $\lambda \in k$ を (ad $h$)$x=\lambda x$ とする。すべての $n\in \mathbf{N}$ とすべての $P\in k[X]$ に対して、私たちは

$$
P(h)x^{(n)}=x^{(n)}P(h+n\lambda ) \tag{12}
$$

ad $h$ は A の導分であり、(ad $h$)$x$ は $x$ と交換できるため、次のようになります。

(広告$h$)$x^n=nx^{n-1}$((広告$h$)$x$)$=n\lambda x^n$、(13)

(広告$h$)$x^{(n)}=n\lambda x^{(n)}$。

したがって、特殊な場合から公式 (12) が得られます。

$$
P(h)x=xP(h+\lambda ) \tag{14}
$$

置き換えること $x$ $x^{(n)}$ および $\lambda$ $n\lambda$ によって。 $P = X^m$のとき、$m$の帰納法までに(14)を証明すれば十分です。 $m= 0,1$の時点でクリアです。 (14) が $P = X^m$ に当てはまる場合、

$$
h^{m+1}x=h.h^mx=hx(h+\lambda )^m=x(h+\lambda )^{m+1}
$$

これは (12) を証明します。

#### 補題 4 {#lie-viii-s12-lem-4 .statement tag=0182}

$x, y, h\in A$ を次のようにしましょう

$$
[y, x] =h,[h, x] = 2x,[h, y] =-2y \tag{15}
$$

(i) $m, n\in \mathbf{N}$ については、

$$
_{(n)(m)}\sum_{(m-p)}(m+n-p-1-h)_{(n-p)}
$$

$xy$ = $yx$。 (16)

$$
p
$$

$p\geq 0$

(ii) $m\in \mathbf{N}$ に対して $x^{(m)}$ と $y^{(m)}$ によって生成された A の $\mathbf{Z}$ 部分代数を $A'$ とします。次に、すべての $n\in \mathbf{N}$ に対して $(^h_n)\in A'$ です。

公式 (16) は同等の形で書くことができます

$$
_{(n)(m)}\sum_{(m-p)}(m+n-p-1-h)_{(n-p)}
$$

(広告$x$)$y$ = $yx.(17_m)$

$$
p
$$

$p\geq 1$

$m= 0$ にとってこれは些細なことです。 $m$の帰納法までに議論します。 $(17_m)$ から、次のようになります。

$(m+$ 1)(広告$x^{(n)}$)$y^{(m+1)}=$ (広告$x^{(n)}$)$y^{(m)}.y+y^{(m)}$.(広告$x^{(n)}$)$y$ (18)

$$
_{(m-p)}(m+n-p-1-h)_{(n-p)(m)}-
$$

$$
=\sum yxy+y(n-1-h)x^{(n1)}
$$

$$
p
$$

$p\geq 1$

(§1, no. 1、補題 1)。さて、適用同じ補題、そして補題 3、

私たちは持っています

$$
(m+n-p-1-h)_{(n-p)}
$$

$$
xy
$$

$$
p
$$

$$
(m+n-p-1-h)_{(n-p)}-_-
$$

= $(yx+ (n-p-1-h)x^{(np1)})$

$$
p
$$

$$
(m+n-p+ 1-h)_{(n-p)}
$$

$$
=yx
$$

$$
p
$$

$$
(m+n-p-1-h)_{--}
$$

+ $(n-p-1-h)x^{(np1)}$。

$$
p
$$

これを (18) に代入すると、次のようになります。

$(m+$ 1)(広告 $x^{(n)}$)$y^{(m+1)}$

$$
_-(m+n-p+ 1-h)_-
$$

$$
=\sum(m-p+ 1)y^{(mp+1)}x^{(np)}
$$

$$
p
$$

$p\geq 1$

$$
_-(m+n-p-1-h)_{--}
$$

$+\sum y^{(mp)}(n-p-1-h)x^{(np1)}$

$$
p
$$

$p\geq 1$

$$
+y^{(m)}(n-1-h)x^{(n-1)}
$$

$$
_-(m+n-p+ 1-h)_-
$$

$=\sum(m-p+ 1)y^{(mp+1)}x^{(np)}$

$$
p
$$

$p\geq 1$

$$
_{(m-p)}(m+n-p-1-h)_{--}
$$

$+\sum y(n-p-1-h)x^{(np1)}$。

$$
p
$$

$p\geq 0$ 2 番目の和で $p$ を $p-1$ に変更し、項を再グループ化すると、次のようになります。

$(m+$ 1)(広告 $x^{(n)}$)$y^{(m+1)}=\sum_{p\geq 1}y^{(m-p+1)}A_px^{(n-p)}$ (19)

と

$$
(m+n-p+ 1-h)(m+n-p-h)
$$

$A_p= (m-p+ 1)+ (n-p-h)$。

$$
pp-1
$$

$z=m+n-p-h$ とすると、これは次のように書くこともできます。

$A_p=p1$!$(m-p+ 1)(z+ 1)z(z-1). . .(z-p+ 2)$

+1 $(z-m)z(z-1). . .(z-p+ 2)$

$(p-$ 1)!

$=p1$! $z(z-1). . .(z-p+ 2)[(m-p+ 1)(z+ 1) +p(z-m)]$

$$
(z)((m+ 1) +n-p-1-h)
$$

$$
= (m+ 1)= (m+ 1)
$$

$$
pp
$$

これを (19) に代入すると、$(17_{m+1})$ が得られるので、(i) になります。

$p < n$ に対して $(^h_p)\in A'$ を仮定します。次に、$P(\mathbf{Z})\subset \mathbf{Z}$ となる次数 $< n$ のすべての $P\in \mathbf{Q}[T]$ に対して、$P(h)\in A'$ (no. 4、提案 2 の補正) が得られます。したがって、$m=n$ を使用して (16) を考慮すると、

$$
(h)(n-1-h)
$$

$(-1)^n$ =

$$
nn
$$

$$
^{n-1}_-(2n-p-1-h)_-'
$$

$=-x^{(n)}y^{(n)}+\sum y^{(np)}x^{(np)}\in A$ ;

$$
p
$$

$p=0$

したがって、(ii) $n$ の帰納法までに。

### 6. 分解的簡約リー代数の代数を包む双順序

$\mathfrak{g}$ を、$\mathfrak{g}$ の $\mathbf{Q},\mathfrak{h}$ 分裂カルタン部分代数、および $R = R(\mathfrak{g},\mathfrak{h}) ($§2, no. 1、注意に対する還元リー代数とする 5)。

#### 定義 1 {#lie-viii-s12-def-1 .statement tag=0183}

$\mathfrak{h}$ の格子 $\mathscr{H}$ は、すべての $\alpha \in R$ に対して $H_{\alpha}\in \mathscr{H}$ と $\alpha (\mathscr{H})\subset \mathbf{Z}$ が存在する場合、($\mathfrak{g}$ に対して) 許容されると言われます。

#### 注意 1 {#lie-viii-s12-n6-rem-1 .statement tag=0184}

BをRの基底とします。$\mathfrak{h}$の格子$\mathscr{H}$は、すべての$\alpha \in B$に対して$H_{\alpha}\in \mathscr{H}$と$\alpha (\mathscr{H})\subset \mathbf{Z}$である場合にのみ許容されます。

#### 注意 2 {#lie-viii-s12-n6-rem-2 .statement tag=0185}

$\mathfrak{c}$を$\mathfrak{g}$の中心とします。次に、$\mathfrak{h}$ の格子 $\mathscr{H}$ は、$Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})\oplus \mathfrak{c}$ の場合にのみ許容されます。格子 $\mathscr{H}\cap \mathscr{D}\mathfrak{g}$ は、$\mathscr{D}\mathfrak{g}$ のカルタン部分代数 $\mathfrak{h}\cap \mathscr{D}\mathfrak{g}$ で許可されます。 $\mathscr{H}\not= (\mathscr{H}\cap \mathscr{D}\mathfrak{g})\oplus (\mathscr{H}\cap \mathfrak{c})$ (cf. §13, no. 1.IX) のような許容格子 $\mathscr{H}$ が存在する可能性があります。

#### 注意 3 {#lie-viii-s12-n6-rem-3 .statement tag=0186}

$\mathfrak{g}$ が半単純の場合、$\mathfrak{h}$ で許容される格子は $Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})$ となる $\mathfrak{h}$ の部分群 $\mathscr{H}$ になります。

この数の残りの部分では、$R = R(\mathfrak{g},\mathfrak{h})$ の分解的簡約リー代数 $(\mathfrak{g},\mathfrak{h})$、基底 B、そしてそれぞれの $\alpha \in B$、対 $(x_{\alpha}, y_{\alpha})$ が固定されていると仮定します。

$$
y_{\alpha}\in \mathfrak{g}^{-\alpha},x_{\alpha}\in \mathfrak{g}^{\alpha},[y_{\alpha}, x_{\alpha}] =H_{\alpha} \tag{20}
$$

$x_{\alpha}$ (それぞれ $y_{\alpha}$) によって生成された $\mathfrak{g}$ の $\mathfrak{n}_+$ (それぞれ $\mathfrak{n}_-$) 部分代数で次のことが分かります (§3, no. 3、提案 9 (iii))。

$$
\mathfrak{g}=\mathfrak{n}_-\oplus \mathfrak{h}\oplus \mathfrak{n}_+ \tag{21}
$$

$$
U(\mathfrak{g}) = U(\mathfrak{n}_-)\otimes_{\mathbf{Q}}U(\mathfrak{h})\otimes_{\mathbf{Q}}U(\mathfrak{n}_+) \tag{22}
$$

(ここで、$U(\mathfrak{g}), . .$. は、$\mathfrak{g}, . . .$ を囲む代数です)。

$\alpha \in B$ と $n\in \mathbf{N}$ の $x^{(n)}_{\alpha}$ によって生成された $U(\mathfrak{n}_+)$ の $\mathbf{Z}$ 部分代数を $\mathscr{U}_+$ で表します。 W を B に対する正の根の $R, R_+$ 集合のワイル群とします。

#### 補題 5 {#lie-viii-s12-lem-5 .statement tag=0187}

(i) $\mathscr{U}_+$ はベクトル空間 $U(\mathfrak{n}_+)$ の格子です。

(ii) すべての $\alpha \in B$ に対して、$\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha}) =\bigoplus_{n\in\mathbf{N}}\mathbf{Z}x^{(n)}_{\alpha}$ があります。

定義により、$\mathscr{U}_+$ は元により $\mathbf{Z}$ モジュールとして生成されます

$x(\varphi \mathbf{n})$ = $1\leq \prod i\leq rx(\varphi n((ii)$))

ここで、$r\in \mathbf{N},\varphi = (\varphi (i))\in B^r$と$\mathbf{n}= (n(i))\in \mathbf{N}^r$です。 代数 $U(\mathfrak{n}_+)$ に、各 $\mathfrak{g}^{\alpha}(\alpha \in R_+)$ が次数 $\alpha$ と同次である型 Q(R) の目盛を与えます。前の型の単項式 $x^{(\mathbf{n})}_{\varphi}$ は次数と同次です

$$
\sum_{1\leq i\leq r}n(i)\varphi (i)\in Q(R)
$$

与えられた次数 $q$ を持つこの種の単項式は、次数 $q$ の $U(\mathfrak{n}_+)$ の同次成分上で数と $\mathbf{Q}$ 上の生成するで有限です。これは(i)を証明します。

$\alpha \in B,\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha})$が、$\alpha$の倍数である次数の同種成分の和に含まれている場合。したがって、前述の式により、$\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha})$ は $\sum n(i)\varphi (i)\in \mathbf{N}\alpha$ となるように $x^{(\mathbf{n})}_{\varphi}$ によって生成され、すべての $i$ に対して $\varphi (i) =\alpha$ が強制されます (B は R の基底であるため)。

$x^{(\mathbf{n})}_{\varphi}=x^{(n(1))}_{\alpha}. . . x^{(n(r))}_{\alpha}=(n(1) +n$(1)!$\cdots . . . n+(nr$)!$(r$))! $x^{(n(1)+\cdot \cdot \cdot+n(r))}_{\alpha}$。

したがって、$\mathscr{U}_+\cap \mathscr{U}(\mathfrak{g}^{\alpha})\subset \bigoplus_n\mathbf{Z}x^{(n)}_{\alpha}$、よって (ii)。 Q.E.D.

この段落の残りの部分では、E と F が $U(\mathfrak{g})$ の $\mathbf{Z}$ サブモジュールである場合、積 $ab$ によって生成された $U(\mathfrak{g})$ の $\mathbf{Z}$ サブモジュールを $E.F$ で表します。ここで、$a\in E, b\in F$ です。

#### 命題 3 {#lie-viii-s12-prop-3 .statement tag=0188}

$\mathscr{H}$を$\mathfrak{h}$の許容格子とします。 $\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$ を、元 $x_{\alpha}^{(n)}$ $(\alpha \in B,n\in \mathbf{N}),y_{\alpha}^{(n)}(\alpha \in B, n\in \mathbf{N}),(^h_n)(h\in \mathscr{H}, n\in \mathbf{N})$ によってそれぞれ生成された $U(\mathfrak{g})$ の $\mathbf{Z}$ 部分代数とする。 $\mathscr{U}$ を $\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$ によって生成された $U(\mathfrak{g})$ の $\mathbf{Z}$ 部分代数とする。

(i) $\mathscr{U}$ は、大角$U(\mathfrak{g})$ の双順序です。

(ii) $\mathscr{U}=\mathscr{U}_-.\mathscr{U}_0.\mathscr{U}_+,\mathscr{U}\cap \mathfrak{h}=\mathscr{H}$ があり、すべての $\alpha \in B$ について、

$$
\mathscr{U}\cap \mathfrak{g}^{\alpha}=\mathbf{Z}x_{\alpha},V\cap \mathfrak{g}^{-\alpha}=\mathbf{Z}y_{\alpha}
$$

By 補題 5 と Prop. $2,\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$ は、それぞれ $\mathbf{Q}$-代数 $U(\mathfrak{n}_+),U(\mathfrak{n}_-),U(\mathfrak{h})$ の位数であり、

$$
(\pm h+q)
$$

$h\in \mathscr{H}, q\in \mathbf{Z}, p\in \mathbf{N}$の$\in \mathscr{U}_0$。 (23)

$$
p
$$

$\mathscr{L}=\mathscr{U}_-.\mathscr{U}_0.\mathscr{U}_+\subset U(\mathfrak{g})$を入れます。 (22) により、$\mathscr{L}$ は $U(\mathfrak{g})$ の格子になります。 構成までに、

$$
\mathscr{U}_-.\mathscr{L}\subset \mathscr{L} \tag{24}
$$

$$
\mathscr{L}.\mathscr{U}_+\subset \mathscr{L} \tag{25}
$$

一方、補題 3 と (23) は次のことを意味します。

$$
\mathscr{U}_0.\mathscr{L}\subset \mathscr{L} \tag{26}
$$

$$
\mathscr{L}.\mathscr{U}_0\subset \mathscr{L} \tag{27}
$$

$\alpha \in B, n\in \mathbf{N}, r\in \mathbf{N}, \varphi = (\varphi (i))\in B^r$ にして、

$$
(m(1), . . . , m(r))\in \mathbf{N}^r
$$

私たちはそれを示します

$$
x^{(n)}_{\alpha}y_{\varphi(1)}^{(m(1))}. . . y_{\varphi(r)}^{(m(r))}\in \mathscr{L} \tag{28}
$$

または同等に、(25) を考慮すると、

$$
[x^{(n)}_{\alpha}, y^{(m(1))}_{\varphi(1)}. . . y_{\varphi(r)}^{(m(r))}]\in \mathscr{L} \tag{29}
$$

$r$の帰納法までに議論します。研究対象のブラケットは項の和です

$(m(1))(m(k))(n)(m(k+1))(m(k+2))(m(r))$

$y_{\varphi(1)}. . . y_{\varphi(k)}[x_{\alpha}, y_{\varphi(k+1)}]y_{\varphi(k+2)}. . . y_{\varphi(r)}$。 (30) $\alpha \not=\varphi (k+ 1),x_{\alpha}$ と $y_{\varphi(k+1)}$ は通勤なので、$[x^{(n)}_{\alpha}, y^{(m(k+1))}_{\varphi(k+1)}] = 0$ です。 $\alpha =\varphi (k+ 1)$ の場合、式 (30) は、(17) により、形の式の和になります。

$(m(1))(m(k))(m(k+1)-p)(q-h)(n-p)(m(k+2))(m(r))$

$$
y_{\varphi(1)}. . . y_{\varphi(k)}y_{\varphi(k+1)}x_{\alpha}y_{\varphi(k+2)}. . . y_{\varphi(r)} \tag{31}
$$

$$
p
$$

ここで、$q\in \mathbf{Z}, p\in$ **N --** $\{0\}, h\in \mathscr{H}$。 帰納法の仮定は、(24) および (26) と合わせて、式 (31) 属するから $\mathscr{L}$ であることを証明します。したがって、(28) を証明しました。

(28) までに、$x^{(n)}_{\alpha}\mathscr{U}_-\subset \mathscr{L}$;したがって、(25) と (27) より、$x^{(n)}_{\alpha}\mathscr{L}\subset \mathscr{L}$、したがって $\mathscr{U}_+.\mathscr{L}\subset \mathscr{L}$、

$$
\mathscr{L}.\mathscr{L}\subset \mathscr{U}_-.\mathscr{U}_0.\mathscr{L}\subset \mathscr{U}_-.\mathscr{L}\subset \mathscr{L}
$$

したがって、$\mathscr{L}$ は $U(\mathfrak{g})$ の $\mathbf{Z}$ 部分代数なので、$\mathscr{U}=\mathscr{L}$ です。 $c$ が $U(\mathfrak{g}),c(\mathscr{U})\subset \mathscr{U}\otimes_{\mathbf{Z}}\mathscr{U}$ の余積である場合 (no. 2、提案 1)。 $\gamma$を$U(\mathfrak{g})$の余単位とします。 $n >0$の$\gamma (x^{(n)}_{\alpha}) =\gamma (y^{(n)}_{\alpha}) =\gamma ((^h_n))= 0$なので、$\gamma (\mathscr{U})\subset \mathbf{Z}$になります。これは(i)を証明します。一方、

$$
\mathscr{U}\cap \mathfrak{h}=\mathscr{L}\cap \mathfrak{h}=\mathscr{U}_0\cap \mathfrak{h}=\mathscr{H}
$$

no. 4の提案2による。同様に、

$$
\mathscr{U}\cap \mathfrak{g}^{\alpha}=\mathscr{U}_+\cap \mathfrak{g}^{\alpha}=\mathbf{Z}x_{\alpha}
$$

by 補題 5. これは (ii) を証明します。

#### 注意 4 {#lie-viii-s12-n6-rem-4 .statement tag=0189}

§4, no. 4 の提案 5 により、すべての $\alpha \in B$ に対して $\theta (x_{\alpha}) =y_{\alpha}$ と $\theta (y_{\alpha}) =x_{\alpha}$、すべての $h\in \mathfrak{h}$ に対して $\theta (h) =-h$ となるように、$\mathfrak{g}$ の固有の自己同型 $\theta$ が存在します。 $\theta^2= 1$があります。 $\mathscr{U}$の構成までに、$U(\mathfrak{g})$の自己同型により、拡大する$\theta$は$\mathscr{U}$が安定したままになることがわかります。

#### 系 1 {#lie-viii-s12-prop-3-cor-1 .statement tag=018A}

$\mathscr{G}=\mathscr{U}\cap \mathfrak{g}$を入れます。すると、$\mathscr{G}$はリー代数$\mathfrak{g}$の位数となり、$\theta$以下で安定します。 $\mathscr{G}=\mathscr{H}+\sum_{\alpha\in R}(\mathscr{G}\cap \mathfrak{g}^{\alpha})$があります。すべての $\alpha \in B$ とすべての $n\in \mathbf{N}$、写像 (広告 $x_{\alpha}$)$^n/n$!、(広告 $y_{\alpha}$)$^n/n$! $\mathscr{U}$ と $\mathscr{G}$ を安定させておきます。

最初の主張はクリアです。 2つ目は、$U(\mathfrak{g})$と$\mathscr{U}$の型Q(R)の卒業を考慮して続きます。 3 番目は、no. 5 の補題 2 から続きます。

#### 系 2 {#lie-viii-s12-prop-3-cor-2 .statement tag=018B}

$w\in W$ にしましょう。 $\theta$ と交換し、$\mathscr{G}$ と $\mathscr{U}$ を安定させ、拡大する $w$ を残す $\mathfrak{g}$ の基本自己同型 $\varphi$ が存在します。

$w$ が形 $s_{\alpha}(\alpha \in B)$ である場合を扱うだけで十分です。 注意まず第一に、広告 $x_{\alpha}$ と広告 $y_{\alpha}$ は $U(\mathfrak{g})$ では局所的にゼロであり、他の語では、すべての $u\in U(\mathfrak{g})$ に対して (広告 $x_{\alpha}$)$^nu=$ となるような整数 $n$ が存在します。 (広告$y_{\alpha}$)$^nu= 0$。

これにより、定義する自己同型 $e^{adx_{\alpha}}=\sum_{n=0}^{\infty}\frac{1}{n!}$(ad $x_{\alpha}$)$^n$ と $U(\mathfrak{g})$ の $e^{ady_{\alpha}}$ が可能になります。これらの $U(\mathfrak{g})$ の自己同型が $\mathscr{U}$ のままであることを直ちに確認します。 $\varphi_1=e^{adx_{\alpha}}e^{ady_{\alpha}}e^{adx_{\alpha}},\varphi_2=e^{ady_{\alpha}}e^{adx_{\alpha}}e^{ady_{\alpha}}$を入れます。 $\varphi_1|\mathfrak{g}=$ $\varphi_2|\mathfrak{g}($§2, no. 2、公式 (1)) があるので、$\varphi_1=\varphi_2$ です。 $\varphi_1=\varphi_2=\varphi$を入れてください。 $\theta \varphi \theta^{-1}=\varphi$なので、$\theta$と$\varphi$が通勤です。一方、§2, no. 2による$\varphi |\mathfrak{h}=w$、補題 1．

#### 系 3 {#lie-viii-s12-prop-3-cor-3 .statement tag=018C}

$\alpha \in R$ にしましょう。 $x\in \mathscr{G}\cap \mathfrak{g}^{\alpha}$ と $n\in \mathbf{N}$ の場合、$x^{(n)}\in \mathscr{U}$ と (広告 $x$)$^n/n$ があります。 $\mathscr{G}$ と $\mathscr{U}$ は安定しています。

これは、$\mathscr{U}$ と Cor の構成により、$\alpha \in B$ であれば明らかです。 1. In the general case, there exists $w\in W$ such that $w(\alpha )\in B$ (Chap. VI, §1, no. 5, Prop. 15). コル著2、$\mathfrak{g}$の自己同型$\varphi$が存在し、$\mathscr{G}$と$\mathscr{U}$は安定し、$\mathfrak{g}^{\alpha}$から$\mathfrak{g}^{w(\alpha)}$までかかります。したがって、構造の輸送によって系になります。

#### 系 4 {#lie-viii-s12-prop-3-cor-4 .statement tag=018D}

$(\mathfrak{g},\mathfrak{h}) ($§2, no. 4、Def に Chevalley 系 $(X_{\alpha})_{\alpha\in R}$ が存在します。 3) $\alpha \in B$ に対して $X_{\alpha}=x_{\alpha}$ と $X_{-\alpha}=y_{\alpha}$ が一致するようにします。これらの特性を持つすべての Chevalley 系 $(X'_{\alpha})_{\alpha\in R}$ について、およびすべての $\alpha \in R,X'_{\alpha}$ は $\mathscr{G}\cap \mathfrak{g}^{\alpha}$ の基底になります。

$\alpha \in B$には$X_{\alpha}=x_{\alpha}, X_{-\alpha}=y_{\alpha}$を入れてください。 $\alpha \in R_+$ **--** B の場合、選ぶは $w\in W$ で、$\mathfrak{g}$ の $w(\alpha )\in B$ と自己同型 $\varphi$ は、$h\in \mathfrak{h}$ に対して $\theta \varphi =\varphi \theta ,\varphi (\mathscr{G}) =\mathscr{G}$ と $\varphi (h) =w^{-1}(h)$ になります (Cor. 2)。 $X_{\alpha}=\varphi (x_{w(\alpha)}), X_{-\alpha}=\varphi (y_{w(\alpha)})$を入れます。それから

$$
[X_{-\alpha}, X_{\alpha}] =\varphi ([y_{w(\alpha)}, x_{w(\alpha)}]) =\varphi (H_{w(\alpha)}) =w^{-1}(H_{w(\alpha)}) =H_{\alpha}
$$

$$
\theta (X_{\alpha}) =\theta \varphi (x_{w(\alpha)}) =\varphi \theta (x_{w(\alpha)}) =\varphi (y_{w(\alpha)}) =X_{-\alpha}
$$

したがって、$(X_{\alpha})_{\alpha\in R}$ はシュバレー 系です。さらに、

$$
\mathscr{G}\cap \mathfrak{g}^{\alpha}=\varphi (\mathscr{G}\cap \mathfrak{g}^{w(\alpha)}) =\varphi (\mathbf{Z}x_{w(\alpha)}) =\mathbf{Z}X_{\alpha} \tag{32}
$$

$$
\mathscr{G}\cap \mathfrak{g}^{-\alpha}=\varphi (\mathscr{G}\cap \mathfrak{g}^{-w(\alpha)}) =\varphi (\mathbf{Z}y_{w(\alpha)}) =\mathbf{Z}X_{-\alpha} \tag{33}
$$

$(X'_{\alpha})_{\alpha\in R}$ を、$\alpha \in B$ に対して $X'_{\alpha}=x_{\alpha}, X'_{-\alpha}=y_{\alpha}$ となるようなシュバレー 系とします。 S を $X'_{\alpha}=\pm X_{\alpha}$ となるような $\alpha \in R$ の集合とします。 §2, no. 4、提案 7 により、S は根の閉じた集合です。 $S\supset B\cup (-B)$ なので、S = R になります（VI, §1, no. 6 章、提案 19）。 したがって、(32) と (33) により、すべての $\alpha \in R$ に対して $\mathscr{G}\cap \mathfrak{g}^{\alpha}=\mathbf{Z}X'_{\alpha}$ が得られます。

#### 注意 5 {#lie-viii-s12-n6-rem-5 .statement tag=018E}

$(X_{\alpha})_{\alpha\in R}$ を上で構築した Chevalley 系とします。 $\alpha , \beta , \alpha +\beta \in R$ と$[X_{\alpha}, X_{\beta}] = N_{\alpha ,\beta}X_{\alpha+\beta}$ を置くと、$[X_{\alpha}, X_{\beta}]\in$ $\mathscr{G}\cap \mathfrak{g}^{\alpha+\beta}$ が得られ、$N_{\alpha ,\beta}\in \mathbf{Z}$ という事実が得られます (cf. §2, no. 4、提案 7)。

#### 注意 6 {#lie-viii-s12-n6-rem-6 .statement tag=018F}

移行で、補題 4、§2 とは独立して、シュヴァレー 系 (cf. §4, no. 4、提案 5 の補正) の新しい証明が得られました。

### 7. シュバレー 位数

$(\mathfrak{g},\mathfrak{h})$ を $\mathbf{Q}, R$ よりも分解的簡約リー代数にして、その根系とします。 選ぶ:

a) $\mathfrak{h}$ の許容格子 $\mathscr{H}$ (no. 6、定義 1)。

b) すべての $\alpha \in R$ について、$\mathfrak{g}^{\alpha}$ の格子 $\mathscr{G}^{\alpha}$。

$\mathscr{G}=\mathscr{H}\oplus \sum_{\alpha\in R}\mathscr{G}^{\alpha}$を入れてください。 $\mathfrak{g}$の格子です。 $\mathbf{Z}$-部分代数を $\mathscr{U}$ で表す

$(^h_n)(h\in \mathscr{H}, n\in \mathbf{N})$ と $x^{(n)}(x\in \mathscr{G}^{\alpha}, \alpha \in R$、$n\in \mathbf{N})$ によって生成された $U(\mathfrak{g})$ 。最後に、$\alpha \in R$ と $x\in \mathfrak{g}^{\alpha}$ **--** $\{0\}$ に、

$w_{\alpha}(x) =$ (exp ad $x$)(exp ad $y$)(exp ad $x$)、

ここで、$y$ は $[y, x] =H_{\alpha}$ となるような $\mathfrak{g}^{-\alpha}$ の一意元です。これらの記法:

#### 定理 2 {#lie-viii-s12-thm-2 .statement tag=018G}

次の条件は同等です。

(i) すべての $\alpha \in R$ に対して $\mathscr{G}_{\alpha}=\mathbf{Z}X_{\alpha}$ となるような $(\mathfrak{g},\mathfrak{h})$ の Chevalley 系 $(X_{\alpha})_{\alpha\in R}$ が存在します。

(ii) すべての $\alpha \in R$ に対して $\mathscr{U}\cap \mathfrak{g}=\mathscr{G}$ と $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$。

(iii) $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}$、自己準同型 (広告 $x$)$^n/n$ 全員に! $\mathfrak{g}$ 写像 $\mathscr{G}$ から $\mathscr{G}$ および $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$ 。

(iv) すべての $\alpha \in R$ と、$\mathscr{G}^{\alpha},w_{\alpha}(x)$ 写像 $\mathscr{G}$ ～ $\mathscr{G}($ のすべての基底 $x$、つまりすべての $\beta \in R)$ について写像 $\mathscr{G}^{\beta}$ ～ $\mathscr{G}^{s_{\alpha}(\beta)}$ について。

(i) $=\Rightarrow$ (ii): $(X_{\alpha})_{\alpha\in R}$ を $(\mathfrak{g},\mathfrak{h})$ のシュバレー 系とし、すべての $\alpha \in R$ に対して $\mathscr{G}^{\alpha}=$ $\mathbf{Z}X_{\alpha}$ とし、B を R の基底とする。$\alpha \in B$ については、$x_{\alpha}=X_{\alpha}, y_{\alpha}=$ を置く$X_{-\alpha}$。 $\mathscr{U}'$ を no. 6 の提案 3 によって $\mathscr{H}$、$x_{\alpha}$ および $y_{\alpha}$ に関連付けられる双順序とします。 $\mathscr{U}'\subset \mathscr{U}$であることは明らかです。コル著提案$3,x^{(n)}\in \mathscr{U}'$の3と4は、$\alpha \in R,x\in \mathscr{G}^{\alpha}$と$n\in \mathbf{N}$すべてに適用されます。したがって、$\mathscr{U}=\mathscr{U}'$ となり、(ii) が証明されます。

(ii) $=\Rightarrow$ (iii): これは、no. 5 の補題 2 によってクリアされます。

(iii) $=\Rightarrow$ (iv): $\alpha \in R$ と $x$ を $\mathscr{G}^{\alpha}$ の基底とします。 $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$ 以降、$[y, x] =H_{\alpha}$ 属するから $\mathscr{G}^{-\alpha}$ などの一意の $y\in \mathfrak{g}^{-\alpha}$ です。 exp ad $x$ と exp ad $y$ は (iii) までに $\mathscr{G}$ を安定させるため、$w_{\alpha}(x)$ も安定します。

(iv) $=\Rightarrow$ (i): B を R の基底とする。すべての $\alpha \in B$ について、選ぶ基底 $x_{\alpha}$ の $\mathscr{G}^{\alpha}$ とする。 $y_{\alpha}\in \mathscr{G}^{-\alpha}$ を $[y_{\alpha}, x_{\alpha}] =H_{\alpha}$ となるようにします。 §1, no. 5, 公式 (5) により、$y_{\alpha}=w_{\alpha}(x_{\alpha}).x_{\alpha}$ が得られるので、$y_{\alpha}$ は (iv) により $\mathscr{G}^{-\alpha}$ の基底になります。 $\mathscr{H}$、$x_{\alpha}$、および$y_{\alpha}$ (no. 6、提案 3 の Cor. 1) によって定義される $\mathfrak{g}$ の位数を $\mathscr{G}'$ とします。次に、$\mathscr{G}'$ は (ad $x_{\alpha}$)$^n/n$!、(ad $y_{\alpha}$)$^n/n$ の下で安定します! (上記引用)、したがって、$w_{\alpha}(x_{\alpha})$ の下にあります。

では、$\beta \in R$ にしましょう。次のような $\alpha_0, \alpha_1, . . . , \alpha_r\in B$ が存在します。

$$
\beta =s_{\alpha_r}s_{\alpha_{r-1}}. . . s_{\alpha_1}(\alpha_0)
$$

（VI, §1, no. 5章、提案15）。 次に、(iv) によって $w_{\alpha_r}(x_{\alpha_r}).w_{\alpha_{r-1}}(x_{\alpha_{r-1}}). . . w_{\alpha_1}(x_{\alpha_1})$ 写像 $\mathscr{G}^{\alpha_0}$ から $\mathscr{G}^{\beta}$ が、前項によって写像 $\mathscr{G}'\cap \mathfrak{g}^{\alpha_0}$ から $\mathscr{G}'\cap \mathfrak{g}^{\beta}$ になります。 $\mathscr{G}'\cap \mathfrak{g}^{\alpha_0}=\mathscr{G}^{\alpha_0}$ (提案 3 (ii)) なので、$\mathscr{G}'\cap \mathfrak{g}^{\beta}=\mathscr{G}^{\beta}$ になります。 したがって

$$
\mathscr{G}'=\mathscr{H}\oplus \sum_{\beta\in R}(\mathscr{G}'\cap \mathfrak{g}^{\beta}) =\mathscr{H}\oplus \sum_{\beta\in R}\mathscr{G}^{\beta}=\mathscr{G}
$$

そしてコル。提案 3 の 4 結論する証明。

#### 定義 2 {#lie-viii-s12-def-2 .statement tag=018H}

条件 Thの(i)〜(iv)の場合。 2 は満足しており、$\mathscr{G}$ は $(\mathfrak{g},\mathfrak{h})$ のシュバレー 位数であると言われています。

#### 注意 {#lie-viii-s12-n7-rem-1 .statement tag=018I}

$(\mathfrak{g},\mathfrak{h})$ の Chevalley 位数は常に存在します。確かに、シュバレー 位数は形 $\mathscr{H}\oplus \sum_{\alpha\in R}\mathbf{Z}X_{\alpha}$ の集合であり、$(X_{\alpha})_{\alpha\in R}$ は $(\mathfrak{g},\mathfrak{h})$ のシュバレー 系であり、$\mathscr{H}$ は $\mathfrak{h}$ の格子です。

$$
Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})\oplus \mathfrak{c}
$$

$(\mathfrak{c}$ は $\mathfrak{g})$ の中心です。

#### 定理 3 {#lie-viii-s12-thm-3 .statement tag=018J}

no. 7 の先頭で記法を保持し、$\mathscr{G}$ が $(\mathfrak{g},\mathfrak{h})$ の Chevalley 位数であると仮定します。

(i) $\mathscr{U}$ は $U(\mathfrak{g})$ の双順序です。

(ii) B を R の基底とし、$(X_{\alpha})_{\alpha\in B\cup(-B)}$ を $\alpha \in B\cup (-B)$ に対して $\mathscr{G}^{\alpha}=\mathbf{Z}X_{\alpha}$ となるような $\mathfrak{g}$ の元の族とする。 $\mathbf{Z}$代数$\mathscr{U}$は、$(^h_n)$と$X_{\alpha}^{(n)}(h\in \mathscr{H}, \alpha \in B\cup (-B), n\in \mathbf{N})$によって生成されます。 $\mathfrak{g}$ が半単純と $\mathscr{H}= Q(R^{\vee})$ である場合、$X_{\alpha}^{(n)}(\alpha \in B\cup (-B), n\in \mathbf{N})$ によって $\mathbf{Z}$-代数 $\mathscr{U}$ が生成されます。

(iii) B を R の基底、正の根、$R_-=-R_+,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha}$ の $R_+$ 対応する集合とします。それから、

$$
\mathscr{U}= (\mathscr{U}\cap U(\mathfrak{n}_-)).(\mathscr{U}\cap U(\mathfrak{h})).(\mathscr{U}\cap U(\mathfrak{n}_+))
$$

$(h_i)_{i\in I}$ を $\mathscr{H}$ の基底とします。すべての $\alpha \in R$ について、$X_{\alpha}$ を $\mathscr{G}^{\alpha}$ の基底とします。 集合 $I\cup R$ に合計位数を与えます ( $I\cap R =\emptyset$ と仮定します)。 $\lambda \in I\cup R$と$n\in \mathbf{N}$には、$\lambda \in I,e^{\langle n\rangle}_{\lambda}=X_{\lambda}^{(n)}$の場合$\lambda \in R$であれば$e^{\langle n\rangle}_{\lambda}=(^{h_{\lambda}}_n)$を入れます。次に、積 $\prod_{\lambda\in I\cup R}e^{\langle n_{\lambda}\rangle}_{\lambda}$、$(n_{\lambda})$ 属するから $\mathbf{N}^{I\cup R}$、$\mathbf{Z}$ モジュール $\mathscr{U}$ の形基底です。の

積 $\prod_{\lambda\in I}(^{h_{\lambda}}_{n_{\lambda}})$、$(n_{\lambda})$ 属するから $\mathbf{N}^I$、$\mathbf{Z}$ モジュール $\mathscr{U}\cap U(\mathfrak{h})$ の形基底。 積 $\prod_{\lambda\in R_+}X_{\lambda}^{(n_{\lambda})}$、$(n_{\lambda})$ 属するから $\mathbf{N}^{R_+}$、$\mathbf{Z}$ モジュール $\mathscr{U}\cap U(\mathfrak{n}_+)$ の形基底。

B と $(X_{\alpha})_{\alpha\in B\cup(-B)}$ を (ii) のように、$[X_{-\alpha}, X_{\alpha}] =H_{\alpha}$ とする。 $\mathscr{U}'$ を、$(_n^h)$ と $X_{\alpha}^{(n)}$ $(h\in \mathscr{H}, \alpha \in B\cup (-B), n\in \mathbf{N})$ によって生成された $U(\mathfrak{g})$ の $\mathbf{Z}$ 部分代数とします。 Thの証明で見ました。 2、(i) $=\Rightarrow$ (ii)、$\mathscr{U}'$ は $\mathscr{U}$ に等しく、$U(\mathfrak{g})$ では双順序です。これは (i) と (ii) の最初の主張を証明します。 2 番目は補題 4 (ii) に続きます。 主張 (iii) は Th から続きます。提案 1 (no. 3) および提案 3 (no. 6)。

### 8. 許容される格子

加群 M のベクトル空間、自己準同型 $u$ に採用されている用語を一般化すると、この基底に対して $u$ の行列が対角となるような M の基底が存在する場合、M は対角化可能であると言われます。

#### 補題 6 {#lie-viii-s12-lem-6 .statement tag=018K}

M を有限型 、M の $u$ 自己準同型、および $M\otimes_{\mathbf{Z}}\mathbf{Q}$ の $v$ 自己準同型 $u\otimes 1$ の自由 $\mathbf{Z}$ 加群とする。すべての $n\in \mathbf{N}$ に対して $(^v_n)(M)\subset M$ であると仮定します。この場合、$u$ は対角化可能です。

a) $P(\mathbf{Z})\subset \mathbf{Z}$ のような多項式 $P\in \mathbf{Q}[T]$ については、$P(v)(M)\subset M$ (no. 4、提案 2 の相関) があるため、$P(v)\in \mathbf{Z}$ を決定します。

b) $v$ の特性多項式を $\chi_v(t) =t^d+\alpha_1t^{d-1}+\cdots$ で表します。 $k\in \mathbf{Z}, n\in \mathbf{N}$ にしましょう。 適用 a) 多項式 $(^{T-k}_n)$ に対して、数がわかります。

$a_n=$ デット $(v-k)=1_d$ デット ($v-k$) デット ($v-k-1$) $. .$。デット($v-k-n+ 1$)

$n(n$!)

$$
=\frac{(-1)^n}{4}\chi_v(k)\chi_v(k+ 1). . . \chi_v(k+n-1)
$$

$(n$!)

は整数です。 $k-1<-\alpha_1/d$ を取ります。それから

$$
\chi_v(k+n-1) =n^d+ (\alpha_1+ (k-1)d)n^{d-1}+\cdots
$$

そして

$$
|a_n|=\frac{|\chi_v(k + n- 1)|}{d}|a_{n-1}|
$$

$$
n
$$

従って、すべての $n\in \mathbf{N}$ に対して $a_n\not= 0$ である場合、$|a_n|$ の数列は、$n$ 十分大きいに対して真に減少するとなり、これは不合理です。従って、$v$ には整数固有値 $\lambda$ が含まれます。 $M'=$ カー($u-\lambda .1$) と $M''= M/M'$ を入れます。この場合、$M'$ は共通部分で、M は $M\otimes_{\mathbf{Z}}\mathbf{Q}$ のベクトル部分空間であるため、$\mathbf{Z}$ 加群 $M''$ は有限型のねじれがなく、その結果階数がありません。 $< d$。 $d$ の帰納法と $u$ によって引き起こされた $M''$ の自己準同型に対する適用帰納法の仮定によって、$v$ のすべての固有値が代数閉拡大にあると結論する主張します。 $\mathbf{Q}$は整数です。

c) $v$ が対角化可能であることを示します。 $\lambda$ を $v$ の固有値とし、$x\in M\otimes_{\mathbf{Z}}\mathbf{Q}$ を $(v-\lambda )^2x= 0$ となるようにします。 $v(vx-\lambda x) =\lambda (vx-\lambda x)$ があるので、

$n1$!$(v-\lambda -n+ 1)(v-\lambda -n+ 2). . .(v-\lambda -1)(v-\lambda )x$

$$
=\frac{(-1)^{n-1}}{n}(vx-\lambda x)
$$

a) により、これはすべての $n\in \mathbf{N}$ に対して $vx-\lambda x\in nM$、つまり $(v-\lambda )x= 0$ を意味します。

d) $\lambda$ を $v$ の固有値とし、$\lambda -a, \lambda +b$ を $v$ の $\mathbf{Z}$ 含むすべての固有値の区間とする。多項式を考えてみましょう

$$
(T-\lambda -1)(T-\lambda -2). . .(T-\lambda -b)
$$

$$
P(T) = (-1)^b
$$

$b$!

$$
(T-\lambda + 1)(T-\lambda + 2). . .(T-\lambda +a)
$$

$$
\times
$$

$a$!

$\mu\in \mathbf{Z}\cap (\lambda -a, \lambda +b)$と$\mu\not=\lambda$には$P(\mathbf{Z})\subset \mathbf{Z},P(\lambda ) = 1,P(\mu) = 0$がございます。 $a), P(v)(M)\subset M$までに。 $c), P(v)$ により、固有空間対応するから $\lambda$ 上では $M\otimes_{\mathbf{Z}}\mathbf{Q}$ の射影になります。 Q.E.D.

#### 注意 1 {#lie-viii-s12-n8-rem-1 .statement tag=018L}

$v$ が整数固有値と対角化可能であるとだけ仮定する場合、$u$ は必ずしも対角化可能ではありません (たとえば、すべての $(x, y)\in M$ に対して $M =\mathbf{Z}^2$ と $u(x, y) =$ $(y, x)$ を取ります)。

$\mathfrak{g},\mathfrak{h},R,\mathscr{H},\mathscr{G}^{\alpha},\mathscr{G},\mathscr{U}$ は no. 7 と同じであり、$\mathscr{G}$ は $(\mathfrak{g},\mathfrak{h})$ の Chevalley 位数であると仮定します。

#### 定義 3 {#lie-viii-s12-def-3 .statement tag=018M}

E を $\mathfrak{g}$ モジュールとします。次の条件が満たされる場合、E の格子 $\mathscr{E}$ は ($\mathscr{G}$ に対して) 許容されると言われます。

(i) $\mathscr{U}$ 写像 $\mathscr{E}$ ～ $\mathscr{E}$;

(ii) $\mathscr{E}$ は、すべての $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}, h\in \mathscr{H}$ に対して、$(^h_n)$ と $x^{(n)}$ の下で安定しています。

#### 注意 2 {#lie-viii-s12-n8-rem-2 .statement tag=018N}

$\rho$ を $U(\mathfrak{g})$ 上の $\mathfrak{g}$ の随伴物表現とします。 $\alpha , x, n, h$を上記(ii)と同様とする。 補題 2 までに $\rho (x^{(n)}).\mathscr{U}\subset \mathscr{U}$ があります。一方、$p\in \mathbf{N}$ の場合、

$((h))_{(n)}($ 広告 $h)_{(n)}(n\alpha (h))_{(n)}$

$\rho x$ = $x$ = $x$

$$
ppp
$$

(no. 5、公式 (13)) なので、$\rho ((^h_p)).\mathscr{U}\subset \mathscr{U}$。これは、$\mathscr{U}$ が $U(\mathfrak{g})$ で許容される格子であることを証明し、$\mathscr{G}$ が $\mathfrak{g}$ (随伴物表現の場合) で許容される格子であることがわかります。

#### 注意 3 {#lie-viii-s12-n8-rem-3 .statement tag=018O}

E を有限次元 $\mathfrak{g}$ 加群、$\mathscr{E}$ を E の許容格子、$\mathfrak{g}$ の $\mathfrak{c}$ 中心とします。 補題 6 までに、$\mathfrak{c}$ 定義するのすべての元は E の対角化可能な自己準同型になります。したがって、E は半単純になります (第 4 章 I, §6, no. 5)。したがって、E は、$\mathfrak{c}$ 誘導するが相似である単純な $\mathscr{D}\mathfrak{g}$ 加群の直和です。 補題 $6,\mathscr{E}=\oplus (\mathscr{E}\cap E^{\lambda})$、そして E のすべての重み $\lambda$ までに、

$$
\lambda (\mathscr{H})\subset \mathbf{Z}
$$

#### 注意 4 {#lie-viii-s12-n8-rem-4 .statement tag=018P}

$\mathfrak{g}$が半単純と$\mathscr{H}= Q(R^{\vee})$の場合、条件はDef.の(i)と(ii)になります。 Th によると、3 は同等です。 3(ii)、へ

(iii) $\mathscr{E}$ は、すべての $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}$ に対して $x^{(n)}$ で安定しています。

#### 注意 5 {#lie-viii-s12-n8-rem-5 .statement tag=018Q}

B を R の基底とします。上記条件 (i) および (ii) において、「$\alpha \in$ R」は「$\alpha \in B\cup (-$B)」に置き換えることができます (引用箇所)。

#### 定理 4 {#lie-viii-s12-thm-4 .statement tag=018R}

E を有限次元 $\mathfrak{g}$ 加群とする。次の条件は同等です。

(i) E には許容可能な格子があります。

(ii) $\mathscr{H}$ 定義するの各元は、E の整数固有値で対角化可能な自己準同型です。

(i) $=\Rightarrow$ (ii): これは注意 3 から続きます。

(ii) $=\Rightarrow$ (i): 条件 (ii) が満たされると仮定し、(i) を証明します。 Thさんより第4章I, §6, no. 5 では、E の $\mathfrak{c}$ 定義するの元が相似であり、E は単純な $\mathscr{D}\mathfrak{g}$ 加群であると仮定できます。 B を R の基底、および $\mathfrak{g}$ の $\mathfrak{g}=\mathfrak{n}_-\oplus \mathfrak{h}\oplus \mathfrak{n}_+$ 対応する分解とします。 $\lambda$ を $\mathscr{D}\mathfrak{g}$ モジュール E の最高重量とし、$e\in E^{\lambda}$ **--** $\{0\}$ とします。 $\mathscr{E}=\mathscr{U}.e$を入れます。 $\mathscr{U}.\mathscr{E}\subset \mathscr{E}$であることは明らかです。 E は単純なので、$U(\mathfrak{g}).e= E$、したがって $\mathbf{Q}$ ベクトル空間としての $\mathscr{E}$ 生成する E になります。 $h\in \mathscr{H}$ と $n\in \mathbf{N}$ には $(^h_n)e=(^{\lambda(h)}_n)e\in \mathbf{Z}e$ があるため、

$$
(\mathscr{U}\cap U(\mathfrak{h})).e=\mathbf{Z}e
$$

$U(\mathfrak{n}_+).e= 0$ なので、提案 3 により $\mathscr{E}= (\mathscr{U}\cap U(\mathfrak{n}_-)).e$ が得られます。 3 (iii) $\mathscr{E}$ は有限型の $\mathbf{Z}$ 加群である。

#### 系 {#lie-viii-s12-n8-cor-1 .statement tag=018S}

$\mathfrak{g}$ が半単純および $\mathscr{H}= Q(R^{\vee})$ である場合、すべての有限次元 $\mathfrak{g}$ 加群には許容可能な格子があります。
