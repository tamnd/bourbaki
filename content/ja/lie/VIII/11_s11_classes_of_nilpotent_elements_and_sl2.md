---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 11
section_title: Classes of nilpotent elements and sl2 -triplets
lang: ja
source: lie-vii-ix
book_pages: 163-173, 261-266
pdf_pages: 0171-0181, 0269-0274
extraction: native+ocr
subsections:
    - "no": 1
      title: DEFINITION OF $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS
      page: 163
      pdf_page: 171
    - "no": 2
      title: $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS IN SEMI-SIMPLE LIE ALGEBRAS
      page: 165
      pdf_page: 173
    - "no": 3
      title: SIMPLE ELEMENTS
      page: 167
      pdf_page: 175
    - "no": 4
      title: PRINCIPAL ELEMENTS
      page: 170
      pdf_page: 178
statements: 29
exercises: 17
content_sha256: 522bf0716a4679c3d1e679cb1b6b2e91fbc4b71cfcbd22a1fff200d29b136440
translated_from: content/en/lie/VIII/11_s11_classes_of_nilpotent_elements_and_sl2.md
translation_method: google
source_content_sha256: c1241130b0c6145fe39e8ebf582c74a6fd108d7391d43fb0cba572e8a86bff67
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 1b137365007792a8dad8f46fbd9c8d85bd989d5d875c4b94bf4bd9d93b4203bc
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 11。 冪零元および $\mathfrak{s}\mathfrak{l}_{2}$ の 3 つ子の類

この段落では、$\mathfrak{g}$ は有限次元のリー代数を表します。

### 1. $\mathfrak{s}\mathfrak{l}_{2}$-三つ子の定義

#### 定義 1 {#lie-viii-s11-def-1 .statement tag=0170}

$\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$ トリプレットは、$\mathfrak{g}$ の元の数列 $(x, h, y)$ であり、$(0,0,0)$ とは異なります。

$$
[h, x] = 2x,[h, y] =-2y,[x, y] =-h
$$

$(x, h, y)$ を $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$ 三重項とします。 $\mathfrak{s}\mathfrak{l}(2, k)$ から $\mathfrak{g}$ までの線形写像 $\tau$ は、$\tau (X_+) =x, \tau (H) =h, \tau (X_-) =y$ が非ゼロであり、したがって単射的である準同型写像であり ($\mathfrak{s}\mathfrak{l}(2, k)$ は単純であるため)、イメージ $kx+kh+ky$ を伴います。 したがって、$\mathfrak{s}\mathfrak{l}(2, k)$から$\mathfrak{g}$までの単射準同型の$\mathfrak{g}$から集合の$\mathfrak{s}\mathfrak{l}_2$トリプレットの集合から正規の全単射が得られます。 $\mathfrak{g}$ が半単純で、$(x, h, y)$ が $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$ 三重項である場合、$x$ と $y$ は $\mathfrak{g}$ の虚元であり、$h$ は $\mathfrak{g}$ の半単純元です (第 3 章)。 I, §6, no. 3、提案 4)。

#### 補題 1 {#lie-viii-s11-lem-1 .statement tag=0171}

$x, h, y, y'\in \mathfrak{g}$ にしましょう。 $(x, h, y)$ と $(x, h, y')$ が $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$ の三つ子である場合、$y=y'$ になります。

確かに、$y-y'\in$ Ker(ad$_{\mathfrak{g}}x$) と (ad$_{\mathfrak{g}}h$)$(y-y') =-2(y-y')$ です。しかし、ad$_{\mathfrak{g}}x$ は、整数 $p >0 ($§1, no. 2 ごとに Ker($p+$ ad$_{\mathfrak{g}}h$) に対して単射法です。提案 2)。

#### 補題 2 {#lie-viii-s11-lem-2 .statement tag=0172}

$\mathfrak{n}$ を $\mathfrak{g}$ の部分代数として、すべての $n\in \mathfrak{n}$ に対して、ad$_{\mathfrak{g}}(n)$ がゼロになるようにします。 $h\in \mathfrak{g}$ を $[h,\mathfrak{n}] =\mathfrak{n}$ となるようにします。次に$e^{ad_{\mathfrak{g}}\mathfrak{n}}.h=h+\mathfrak{n}$。

$e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h\subset h+\mathfrak{n}$であることは明らかです。 $v\in \mathfrak{n}$ の場合、$h+v\in e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h$ であることを証明します。すべての $p\geq 1$ について $h+v\in e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h+\mathscr{C}0\mathfrak{n}$ であることを証明すれば十分です (十分大きい $p$ については $\mathscr{C}^p\mathfrak{n}= 0$ であるため)。これは、$\mathscr{C}^1\mathfrak{n}=\mathfrak{n}$以降の$p= 1$では明らかです。ここで、$h+v=e^{ad_{\mathfrak{g}}y_p}.h+z_p$ となるような $y_p\in \mathfrak{n}$ と $z_p\in \mathscr{C}^p\mathfrak{n}$ の存在が証明されたと仮定します。 (ad$_{\mathfrak{g}}h$)$(\mathfrak{n}) =\mathfrak{n}$、(ad$_{\mathfrak{g}}h$)$|\mathfrak{n}$は$\mathfrak{n}$から$\mathfrak{n}$までの全単射であるため、$\mathscr{C}^p\mathfrak{n}$が安定したままの制限から$\mathscr{C}^p\mathfrak{n}$も全単射です。従って、$z_p= [z, h]$ となるような $z\in \mathscr{C}^p\mathfrak{n}$ が存在します。それから

$$
e^{ad_{\mathfrak{g}}(y_p+z)}h-e^{ad_{\mathfrak{g}}y_p}h\in [z, h] +\mathscr{C}^{p+1}\mathfrak{n}
$$

それで

$$
e^{ad_{\mathfrak{g}}(y_p+z)}h\in h+v-z_p+ [z, h] +\mathscr{C}^{p+1}\mathfrak{n}=h+v+\mathscr{C}^{p+1}\mathfrak{n}
$$

これにより、$p$の帰納法までに主張が確立されます。

#### 補題 3 {#lie-viii-s11-lem-3 .statement tag=0173}

$x\in \mathfrak{g},\mathfrak{p}=$ カー(広告 $x$)$,\mathfrak{q}=$ 私(広告 $x$) にしましょう。すると$[\mathfrak{p},\mathfrak{q}]\subset \mathfrak{q}$、そして$\mathfrak{p}\cap \mathfrak{q}$は$\mathfrak{g}$の部分代数です。

$u\in \mathfrak{p}$ と $v\in \mathfrak{q}$ の場合、$v= [x, w]$ となるような $w\in \mathfrak{g}$ が存在します。

$$
[u, v] = [u,[x, w]] = [x,[u, w]]-[[x, u], w] = [x,[u, w]]\in \mathfrak{q}
$$

一方、$\mathfrak{p}$は$\mathfrak{g}$の部分代数なので、$[\mathfrak{p}\cap \mathfrak{q},\mathfrak{p}\cap \mathfrak{q}]\subset \mathfrak{p}\cap \mathfrak{q}$です。

#### 補題 4 {#lie-viii-s11-lem-4 .statement tag=0174}

$(x, h, y)$ と $(x, h', y')$ を $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$ の三つ子とします。 ad$_{\mathfrak{g}}z$が無能であり、次のような$z\in \mathfrak{g}$が存在します。

$$
e^{ad_{\mathfrak{g}}z}x=x,e^{ad_{\mathfrak{g}}z}h=h',e^{ad_{\mathfrak{g}}z}y=y'
$$

$\mathfrak{n}=$ カー(ad $x$)$\cap$ Im(ad $x$) とします。すべての $p\in \mathbf{Z}$ に対して、$\mathfrak{g}_p=$ Ker(ad $h-p$) とします。 §1, no. 3 ($\mathfrak{g}$ 上の $kx+ky+kh$ の随伴部分表現に適用) により、$\mathfrak{n}\subset \sum_{p>0}\mathfrak{g}_p$ が得られるため、ad$_{\mathfrak{g}}n$ はすべての $n\in \mathfrak{n}$ と $[h,\mathfrak{n}] =\mathfrak{n}$ に対して零になります。 $[x, h'-h] = 0$と$[x, y-y'] =h'-h$があるので、$h'-h\in \mathfrak{n}$です。 補題 2 と 3 までに、$e^{ad_{\mathfrak{g}}z}h=h'$ となるような $z\in \mathfrak{n}$ が存在します。 $z\in$ Ker ad$_{\mathfrak{g}}x$ なので、$e^{ad_{\mathfrak{g}}z}x=x$ になります。 補題 1 は $e^{ad_{\mathfrak{g}}z}y=y'$ であることを証明します。 Q.E.D.

G を $\mathfrak{g}$ の自己同型の群とします。次に、$gx=x'$、$gh=h', gy=y'$ のような $g\in G$ が存在する場合、2 つの $\mathfrak{s}\mathfrak{l}_2$ トリプレット $(x, h, y)$、$(x', h', y')$ は G 共役であると言われます。

#### 命題 1 {#lie-viii-s11-prop-1 .statement tag=0175}

G を $\mathfrak{g}$ 含む Aut$_e(\mathfrak{g})$ の自己同型の群とします。 $(x, h, y)$ と $(x', h', y')$ を $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$ の三つ子とします。しましょう

$$
\mathfrak{t}=kx+kh+ky,\mathfrak{t}'=kx'+kh'+ky'
$$

次の条件について考えてみましょう。

(i) $x$ と $x'$ は G 共役体です。

(ii) $(x, h, y)$ と $(x', h', y')$ は G 共役体です。

(iii) $\mathfrak{t}$ と $\mathfrak{t}'$ は G 共役体です。

(i) $\Leftarrow \Rightarrow$ (ii) $=\Rightarrow$ (iii) があります。 $k$ が代数的に閉じている場合、3 つの条件は等価です。

(i) $\Leftarrow \Rightarrow$ (ii): これは補題 4 から続きます。

(ii) $=\Rightarrow$ (iii): これは明らかです。

$k$ が代数的に閉じていると仮定し、(iii) $=\Rightarrow$ (i) を証明します。 まず$\mathfrak{t}=\mathfrak{t}'=\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k)$の場合を扱います。 ad$_{\mathfrak{g}}x$ は nilpotent であるため、$k^2$ の準同型性 $x$ は nilpotent であるため (Chap. I, §6、Th. 3)、$AxA^{-1}=X$ となるような行列 $A\in \mathbf{G}\mathbf{L}(2, k)$ が存在し、その結果、次のような $\mathfrak{s}\mathfrak{l}(2, k)$ の自己同型性 $\alpha$ が存在します。 $\alpha (x) =x'$;現在$\alpha \in$ 秋$_e(\mathfrak{g}) ($§5, no. 3、コル。提案 5 の 2)。 ここで一般的なケースに移ります。 $\mathfrak{t}$ と $\mathfrak{t}'$ が G 共役であると仮定し、$x$ と $x'$ が G 共役であることを証明します。 $\mathfrak{t}=\mathfrak{t}'$ と仮定できます。 前述により、$\beta x=x'$ となるような $\beta \in$ Aut$_e(\mathfrak{t})$ が存在します。 ここで、$t\in \mathfrak{t}$ が ad$_{\mathfrak{t}}t$ が nilpotent である場合、ad$_{\mathfrak{g}}t$ は nilpotent です。従って、$\beta$ は Aut$_e(\mathfrak{g})$ の要素に拡張されます。

#### 注意 {#lie-viii-s11-n1-rem-1 .statement tag=0176}

$k=k^2$ (cf. 例題 1) だけを仮定する場合、提案 1 の 3 つの条件は同等です。

### 2. $\mathfrak{s}\mathfrak{l}_{2}$-半単純リー代数の三つ子

#### 補題 5 {#lie-viii-s11-lem-5 .statement tag=0177}

V を有限次元ベクトル空間、A と B V の自己準同型とします。 A が零能であり、$[A,[A,B]] = 0$ であると仮定します。この場合、AB は無能です。

$C = [A,B]$を入れてください。 $[A,C] = 0$ 以来、

$[A$、紀元前$^p] = [A,B]C^p= C^{p+1}$

整数 $p\geq 0$ ごとに。その結果、$p\geq 1$ に対して Tr(C$^p$) $= 0$ となり、C が無能であることが証明されます (代数、Chap. VII, §3, no. 5、提案 13 の Cor. 4)。ここで、$\overline{k}$ を $k$ の代数閉包とし、$\lambda \in \overline{k},x\in V\otimes_k\overline{k}$ を AB$x=\lambda x$、$x\not= 0$ となるようにします。 関係 $[[B,A],A] = 0$ は、整数 $p\geq 0$ ごとに $[B,A^p] =p[B,A]A^{p-1}$ になることを示します。 $r$ を最小の整数として、$A^rx= 0$ とします。それから

$\lambda A^{r-1}x= A^{r-1}$AB$x= A^rBx=$BA$^rx-[B,A^r]x=-r[B,A]A^{r-1}x$。

$[B,A]$ は零能であり、$A^{r-1}x\not= 0$ なので、これは $\lambda = 0$ であることを証明します。従って、AB のすべての固有値は零であるため、補題になります。

#### 補題 6 {#lie-viii-s11-lem-6 .statement tag=0178}

$h, x\in \mathfrak{g}$ を $[h, x] = 2x$ と $h\in$ (ad $x$)$(\mathfrak{g})$ とする。次に、$(x, h, y)$ が $(0,0,0)$ または $\mathfrak{s}\mathfrak{l}_2$ の三つ組であるような $y\in \mathfrak{g}$ が存在します。

$\mathfrak{g}'$ を可解リー代数 $kh+kx$ とします。 Since $x\in [\mathfrak{g}',\mathfrak{g}']$, ad$_{\mathfrak{g}}x$ is nilpotent (Chap. I, §5, no. 3, Th. 1); let $\mathfrak{n}$ be its kernel. [広告 $h$, 広告 $x] =$ 2 広告 $x$] なので、(広告 $h$)$\mathfrak{n}\subset \mathfrak{n}$ となります。 $z\in \mathfrak{g}$ を $h=-[x, z]$ となるようにします。 整数 $n\geq 0$ には、$M_n=$ (広告 $x$)$^n\mathfrak{g}$ を入れます。 $n >0$ の場合、(§1, no. 1, 補題 1) になります。

[広告 $z$,(広告 $x$)$^n] =n$((広告 $h$)$-n+$ 1)(広告 $x$)$^{n-1}$

つまり、$u\in M_{n-1}$ の場合、

$n$((広告$h$)$-n+ 1$)$u\in$ (広告$z$)(広告$x$)$u+ M_n$。

(ad $h$)$\mathfrak{n}\subset \mathfrak{n}$ なので、次のようになります。

((広告$h$)$-n+ 1$)$(\mathfrak{n}\cap M_{n-1})\subset \mathfrak{n}\cap M_n$。

広告 $x$ は無能であるため、十分大きい $n$ に対して $M_n= 0$ です。従って、広告$h|\mathfrak{n}$の固有値は整数$\geq 0$となります。従って、広告 $h+ 2$ から $\mathfrak{n}$ の制限は反転可能です。

現在 $[h, z] + 2z\in \mathfrak{n}$ 以来

$$
[x,[h, z] + 2z] = [[x, h], z] + [h,[x, z]] + 2[x, z]
$$

$$
= [-2x, z] + [h,-h] + 2[x, z] = 0
$$

したがって、$[h, z'] + 2z'= [h, z] + 2z$、つまり$y=z-z'$を入れると$[h, y] =-2y$となるような$z'\in \mathfrak{n}$が存在します。 $[x, y] = [x, z] =-h$なので、これで証明が完了です。

#### 命題 2 (ヤコブソン・モロゾフ) {#lie-viii-s11-prop-2 .statement tag=0179}

$\mathfrak{g}$ が半単純であると仮定します。 $x$ を $\mathfrak{g}$ の非ゼロ冪零元とします。 $(x, h, y)$ が $\mathfrak{s}\mathfrak{l}_2$ 三つ組であるような $h, y\in \mathfrak{g}$ が存在します。

$\mathfrak{n}=$ Ker(ad $x$)$^2$ にしましょう。 $z\in \mathfrak{n}$ の場合、[広告 $x$,[広告 $x$, 広告 $z]] =$ 広告([$x,[x, z]]$) $= 0$]。 補題 5 までに、ad $x\circ$ ad $z$ は無能であるため、Tr(ad $x\circ$ ad $z$) $= 0$ です。これは、$\mathfrak{g}$の殺害形$\Phi$に関して、$x$が$\mathfrak{n}$と直交していることを示しています。以来

$\Phi$((広告$x$)$^2y, y'$)$=\Phi (y$, (広告$x$)$^2y')$

すべての $y, y'\in \mathfrak{g}$ に対して、$\Phi$ は非縮退であるため、$\mathfrak{n}$ の直交補数は (ad $x$)$^2$ の像です。したがって、$x=$ (ad $x$)$^2y'$ となるような $y'\in \mathfrak{g}$ が存在します。置く

$$
h=-2[x, y']
$$

$[h, x] = 2x$ と $h\in$ (広告 $x$)$(\mathfrak{g})$ があります。ここで、補題 6 を適用するだけで十分です。

#### 系 {#lie-viii-s11-n2-cor-1 .statement tag=017A}

$\mathfrak{g}$ が半単純であると仮定します。 G を $\mathfrak{g}$ 含む Aut$_e(\mathfrak{g})$ の自己同型の群とします。 写像は、G 共役クラスの集合から商、全単射への通過により、$\mathfrak{g}$ 冪零元 $x$ 定義するの任意の $\mathfrak{s}\mathfrak{l}_2$ トリプレット $(x, h, y)$ に関連付けられます。非ゼロ冪零元の G 共役クラスの $\mathfrak{s}\mathfrak{l}_2$ トリプレットから集合まで。

これは提案 1 と 2 から導き出されます。

#### 補題 7 {#lie-viii-s11-lem-7 .statement tag=017B}

K を可換体とし、少なくとも 4 元とします。 G を行列 $(\alpha 0\alpha \beta_{-1})$ の群とします。ここで、$\alpha \in K^*,\beta \in K$ です。 $G'$ を群とします

行列のような $\alpha = 1$ 。次に$G'= (G,G)$。

$\alpha , \alpha '\in K^*$ と $\beta , \beta '\in K$ の場合、

$$
(\alpha \beta )((\alpha '\beta ')((\alpha \beta )^{-1}(\alpha '\beta ')^{-1}
$$

0 $\alpha^{-1}$ 0 $\alpha^{'-1}$ 0 $\alpha^{-1}$ 0 $\alpha^{'-1}$

$$
=(1-\alpha '\beta '-{\alpha \beta \alpha '}^2+\alpha^2\alpha '\beta '+\alpha \beta )
$$

0 1

特に、

$(1\beta )((\alpha '$ 0 $)((1\beta )^{-1}(\alpha '$ 0 $)^{-1}=(1\beta (1-{\alpha '}^2))$。

0 1 0 $\alpha^{'-1}$ 0 1 0 $\alpha^{'-1}$ 0 1

しかし、$\alpha '_0\not= 1$ と $\alpha '_0\not=-1$ 、そして $k.(1-{\alpha '_0}^2)$ $=k$ のような $\alpha '_0\in K^*$ が存在するため、補題になります。

#### 命題 3 {#lie-viii-s11-prop-3 .statement tag=017C}

$\mathfrak{g}$ が半単純であると仮定します。 群 Aut$_e(\mathfrak{g})$ はその導来群に等しい。 $\mathfrak{g}$ が分割可能な場合、Aut$_e(\mathfrak{g})$ は Aut$_0(\mathfrak{g})$ の導来群になります。

$x$ を $\mathfrak{g}$ の非ゼロ冪零元とします。 選ぶ $h, y\in \mathfrak{g}$ は、$(x, h, y)$ が $\mathfrak{s}\mathfrak{l}_2$ の三つ組になるようにします (提案 2)。 $(x, h, y)$ によって生成された $\mathfrak{g}$ の部分代数 $\mathfrak{s}$ は、$\mathfrak{s}\mathfrak{l}(2, k)$ で識別できます。 $\rho$ を表現 $z \rightarrow$ と $\mathfrak{g}$ の $\mathfrak{s}=\mathfrak{s}\mathfrak{l}(2, k)$ の $_{\mathfrak{g}}z$ とし、$\pi$ を $\rho ($§1, no. 4 と互換性のある $\mathbf{S}\mathbf{L}(2, k)$ の表現とします）。 $\pi$の像は、exp($t$ad$_{\mathfrak{g}}x$)と$t\in k($代数のexp($t$ad$_{\mathfrak{g}}y$)によって生成されます。 III, §8, no. 9、提案 17)、したがって、Aut$_e(\mathfrak{g})$ に含まれています。 $\mathbf{S}\mathbf{L}(2, k)$ はその導来群 (補題 7 および前述) に等しいので、exp(ad$_{\mathfrak{g}}x$) 属するから Aut$_e(\mathfrak{g})$ の導来群 G となります。したがって、Aut$_e(\mathfrak{g})$ は G に等しいです。ここで、$\mathfrak{g}$ が分割可能であると仮定します。 Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ は可換 (§5, no. 3, 注意 3) であるため、上記は Aut$_0(\mathfrak{g})$ の導来群が Aut$_e(\mathfrak{g})$ であることを証明します。

### 3. シンプル元

#### 定義 2 {#lie-viii-s11-def-2 .statement tag=017D}

$\mathfrak{g}$ の元 $h$ は、$(x, h, y)$ が $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$ 三重項であるような $x, y\in \mathfrak{g}$ が存在する場合、単純であると言われます。

また、$h$ は $\mathfrak{s}\mathfrak{l}_2$-3 つ$(x, h, y)$ の単純な元であるとも言います。

#### 命題 4 {#lie-viii-s11-prop-4 .statement tag=017E}

$h$ を $\mathfrak{g}$ の非ゼロ元とします。次に、$h$ は、$[h, x] = 2x$ と $h\in$ (ad $x$)$(\mathfrak{g})$ のような $x\in \mathfrak{g}$ が存在する場合にのみ単純です。

条件は明らかに必要です。 補題 6までに十分です。

#### 命題 5 {#lie-viii-s11-prop-5 .statement tag=017F}

$\mathfrak{g}$ は分割可能半単純であると仮定します。 $\mathfrak{h}$ を $\mathfrak{g}$ の分割カルタン部分代数、R を $(\mathfrak{g},\mathfrak{h})$ の根の集合、B を R の基底とします。 $h$ を $\mathfrak{g}$ 所属から $\mathfrak{h}$ の単純な元とします。 次に、$h$ は、Aut$_e(\mathfrak{g},\mathfrak{h})$ から $\mathfrak{h}$ の元 $h'$ の下の共役となり、すべての $\alpha \in B$ に対して $\alpha (h')\in  \{0,1,2\}$ になります。

固有値の広告$_{\mathfrak{g}}h$ 属するから $\mathbf{Z}($§1, no. 2、Cor。提案 2)。 したがって、$h\in \mathfrak{h}_{\mathbf{Q}}$です。 すべての$\alpha \in B$に対して$\alpha (wh)\geq 0$となるような$(\mathfrak{g},\mathfrak{h})$のワイル群の元$w$が存在します（VI, §1, no. 5章、Th.2（i））。 §2, no. 2 の観点から、Cor。 Thの。 2、すべての $\alpha \in B$ に対して $\alpha (h)\in \mathbf{N}$ の場合に帰着します。 $R_+$ を B に対する正の根の集合と $R_-=-R_+$ とします。 形 $(x, h, y)$ の $\mathfrak{g}$ には $\mathfrak{s}\mathfrak{l}_2$ 三重項が存在します。 T を $\beta (h) =-2$ となるような根 $\beta$ の集合とします。 次に、$T\subset R_-$ と $y\in \sum_{\beta\in T}\mathfrak{g}^{\beta}$ です。 そこにあると仮定します

$\alpha (h)>2$ となるような $\alpha \in B$ が存在します。すべての $\beta \in T$ に対して、$(\alpha +\beta )(h)>0$ があるため、$\alpha +\beta  \notin R_-$ と $\alpha +\beta \not= 0$ になります。一方、$\beta \in R_-$ と $\alpha \in B$ なので、$\alpha +\beta  \notin R_+$ になります。したがって$\alpha +\beta  \notin R\cup  \{0\}$、したがって$[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] = 0$。したがって、$[y,\mathfrak{g}^{\alpha}] = 0$。しかし、広告$_{\mathfrak{g}}y|\mathfrak{g}^{\alpha}$は、$\alpha (h)>0 ($§1, no. 2、Cor. 以来単射法です。提案 2)。この矛盾は、すべての $\alpha \in B$ に対して $\alpha (h)\leq 2$ であることを証明します。

#### 系 {#lie-viii-s11-n3-cor-1 .statement tag=017G}

$k$ が代数的に閉じていて、$\mathfrak{g}$ が階数 $l$ の半単純である場合、$\mathfrak{g}$ の単純な元の共役類の数は、Aut$_e(\mathfrak{g})$ と比較して、最大でも $3^l$ です。

実際、$\mathfrak{g}$ のすべての半単純元は、Aut$_e(\mathfrak{g})$ から $\mathfrak{h}$ の元の下では共役です。

#### 補題 8 {#lie-viii-s11-lem-8 .statement tag=017H}

$k$ が代数的に閉じており、$\mathfrak{g}$ が半単純であると仮定します。広告 $h$ の固有値が有理となるように、$h$ を $\mathfrak{g}$ の半単純元とします。 $\mathfrak{g}^0=$ カー(広告 $h$)$,\mathfrak{g}^2=$ カー(広告 $h-2$) とします。 $h$ を固定したまま、$G_h$ を初級の集合 $\mathfrak{g}$ の自己同型とします。 $x\in \mathfrak{g}^2$ を $[x,\mathfrak{g}^0] =\mathfrak{g}^2$ となるようにします。次に、ザリスキー位相の密でオープンな$\mathfrak{g}^2$の$G_hx$含む部分集合。

$\mathfrak{h}$ を $\mathfrak{g}^0$ のカルタン部分代数とします。 This is a Cartan subalgebra of $\mathfrak{g}$ containing $h$ (Chap. VII, §2, no. 3, Prop. 10). $h\in \mathfrak{h}_{\mathbf{Q}}$ があります。 R を $(\mathfrak{g},\mathfrak{h}), Q$ 群根基重みの根系とします。 すべての $\alpha \in B$ に対して $\alpha (h)\geq 0$ となるような R の基底 B が存在します。

U を $z\in \mathfrak{h}$ の集合として、すべての $\alpha \in B$ に対して $\alpha (z)\not= 0$ となるようにします。 $(H'_{\alpha})_{\alpha\in B}$ を、B に対する双対の $\mathfrak{h}$ の基底とします。 $z\in U$ の場合、$\gamma \in Q$ から $\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$ までの任意の準同型が Q から $k^*$ まで存在します。 §5、提案 2 および 4 により、

ベクトル空間 $\mathfrak{g}$ の自己準同型 $\varphi (z)$ は、$\mathfrak{g}^{\gamma}$ ホモテティー 上の誘導すると比率 $\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$ は、明らかに $\mathfrak{g}$ の基本的な自己同型です。

属するから$G_h$まで。

$s\in \mathfrak{h}$ にしましょう。 $\gamma \in R$ が $\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2\not= 0$ となる場合、

$$
2 =\gamma (h) =\gamma (\sum_{\alpha\in B}\alpha (h)H'_{\alpha})=\sum_{\alpha\in B}\alpha (h)\gamma (H'_{\alpha})
$$

すべての $\alpha \in B$ に対して $\alpha (h)\geq 0$ があり、$\gamma (H'_{\alpha})$ はすべて $\geq 0$ またはすべての $\leq 0$ のいずれかである整数であるため、すべての $\alpha \in B$ に対して $\gamma (H'_{\alpha})\in \mathbf{N}$ が得られます。したがって、($z\in \mathfrak{h}$の場合) ベクトル空間 $\mathfrak{g}^2$の自己準同型 $\psi (z)$は、$\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2$ ホモテティーの誘導するが比$\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$で考慮できます。 写像 $z \rightarrow \psi (z)$ $\mathfrak{h}$ から End($\mathfrak{g}^2$) までは多項式です。 $z\in U$の場合、$\psi (z) =\varphi (z)|\mathfrak{g}^2$があります。

$\gamma_1, . . . , \gamma_r$を、$h$に消える$(\mathfrak{g},\mathfrak{h})$の別個の根とします。 $y_1\in \mathfrak{g}^{\gamma_1}, . . .$、$y_r\in \mathfrak{g}^{\gamma_r}$ の場合、$e^{ady_1}. . . e^{ady_r}\in G_h$ になります。したがって、次のようにすると、 定義する写像 $\rho$ を $\mathfrak{h}\times \mathfrak{g}^{\gamma_1}\times  \cdots  \times \mathfrak{g}^{\gamma_r}$ から $\mathfrak{g}^2$ にできます。

$$
\rho (z, y_1, . . . , y_r) =\psi (z)e^{ady_1}. . . e^{ady_r}x
$$

$z\in \mathfrak{h}, y_1\in \mathfrak{g}^{\gamma_1}, . . . , y_r\in \mathfrak{g}^{\gamma_r}$の場合。この写像は多項式であり、 $\rho (U,\mathfrak{g}^{\gamma_1}, . . . ,\mathfrak{g}^{\gamma_r})$ $\subset G_hx$ です。章著。 VII、アプリ。 I、提案 3 と 4、$\rho$ の接線線形写像が、ある点で全射であることを証明すれば十分です。

ここで、T を $h_0=\sum_{\alpha\in B}H'_{\alpha}$ における $z \rightarrow \psi (z)$ の接線線形写像とします。すると、$T(z)$ は $\mathfrak{g}^2$ の自己準同型と、$\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2$ ホモテティー の誘導するが比率で表されます。

$$
\sum_{\alpha\in B}\gamma (H'_{\alpha})\alpha (h_0)^{\gamma(H'_{\alpha})-1}\alpha (z)\prod_{\beta\in B,\beta\not=\alpha}\beta (h_0)^{\gamma(H'_{\alpha})}=\sum_{\alpha\in B}\gamma (H'_{\alpha})\alpha (z) =\gamma (z)
$$

したがって、$h_0$における$z \rightarrow \rho (z,0, . . . ,0)$の接線線写像は写像$z \rightarrow [z, x]$です。その像は$[x,\mathfrak{h}]$です。 写像 $y_1 \rightarrow \rho (h_0, y_1,0, . . . ,0)$ の 0 における接線線形写像は写像 $y_1 \rightarrow \psi (h_0)[y_1, x]$ です。この最後の写像には像 $\psi (h_0)[x,\mathfrak{g}^{\gamma_1}] = [x,\mathfrak{g}^{\gamma_1}]$ があります。同様に、写像 $y_i \rightarrow \rho (h_0,0, . . . ,0, y_i,0, . . . ,0)$ の 0 における接線線形写像は像 $[x,\mathfrak{g}^{\gamma_i}]$ になります。最後に、$(h_0,0, . . . ,0)$における$\rho$の接線線写像は像になります

$$
[x,\mathfrak{h}+\mathfrak{g}^{\gamma_1}+\cdots +\mathfrak{g}^{\gamma_r}] = [x,\mathfrak{g}^0] =\mathfrak{g}^2.Q.E.D
$$

\* 群 $G_h$ は、リー代数と $\mathfrak{g}^0$ を組み合わせた代数群です。\*

#### 命題 6 {#lie-viii-s11-prop-6 .statement tag=017I}

$k$ が代数的に閉じており、$\mathfrak{g}$ が半単純であると仮定します。 G を $\mathfrak{g}$ 含む Aut$_e(\mathfrak{g})$ の自己同型の群とします。 $(x, h, y)$ と $(x', h', y')$ を $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$ の三つ子とします。次の条件は同等です。

(i) $h$ と $h'$ は G 共役体です。

(ii) $(x, h, y)$ と $(x', h', y')$ は G 共役体です。

含意 (i) $=\Rightarrow$ (ii) を証明するだけでよく、直ちに $h=h'$ の場合に帰着します。 補題のように $\mathfrak{g}^2$ と $G_h$ を導入します。 8. §1, no. 2、Cor による $x\in \mathfrak{g}^2$ と $[x,\mathfrak{g}^0] =\mathfrak{g}^2$ があります。従って、$\mathfrak{g}^2$ の $G_hx$ 含む部分集合はザリスキー 位相で密で開いており、$G_hx'$ も同様です。従って、$a(x) =x'$ となるような $a\in G_h$ が存在します。 $a(h) =h$ があり、その結果、$a(y) =y'$ (no. 1, 補題 1) になります。

#### 系 1 {#lie-viii-s11-prop-6-cor-1 .statement tag=017J}

写像は、$\mathfrak{s}\mathfrak{l}_2$-トリプレットの G 共役クラスの集合から G-共役クラスの集合への商全単射への通過によって、任意の $\mathfrak{s}\mathfrak{l}_2$-トリプレットの単純な元定義するに関連付けられます。シンプルな元。

#### 系 2 {#lie-viii-s11-prop-6-cor-2 .statement tag=017K}

rk($\mathfrak{g}$) $=l$ の場合、$\mathfrak{g}$ の非ゼロ冪零元の Aut$_e(\mathfrak{g})$ を基準とした共役類の数は最大でも $3^l$ です。

これはコルからの続きです。 1、コル。提案 2、および Cor.提案 5 の。

#### 系 3 {#lie-viii-s11-prop-6-cor-3 .statement tag=017L}

rk($\mathfrak{g}$) $=l$ の場合、Aut$_e(\mathfrak{g})$ を基準とした $\mathfrak{s}\mathfrak{l}(2, k)$ と同型の $\mathfrak{g}$ の部分代数の共役類の数は最大でも $3^l$ です。

これはコルからの続きです。 1、提案 1、および Cor.提案 5 の。

### 4. 校長元

#### 定義 3 {#lie-viii-s11-def-3 .statement tag=017M}

$\mathfrak{g}$ が半単純であると仮定します。

(i) Ker ad $x$ の次元が $\mathfrak{g}$ の階数である場合、$\mathfrak{g}$ の冪零元 $x$ がプリンシパルであると言われます。

(ii) $\mathfrak{g}$ の単純な元 $h$ は、$h$ が正規で、$k$ 属する ～ $2\mathbf{Z}$ の代数閉包にある広告 $h$ の固有値がプリンシパルであると言われます。

(iii) $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$ トリプレット $(x, h, y)$ は、$\mathfrak{g}$ の長さが、$kx+kh+ky$ の加群とみなされて、$\mathfrak{g}$ の階数に等しい場合、主であると言われます。

#### 命題 7 {#lie-viii-s11-prop-7 .statement tag=017N}

$\mathfrak{g}$ が半単純であると仮定します。 $(x, h, y)$ を $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}_2$-三重項 とします。次の条件は同等です。

(i) $x$ が元本です。

(ii) $h$ が元本です。

(iii) $(x, h, y)$ が本人です。

$p\in \mathbf{Z}$ については、$\mathfrak{g}^p=$ Ker(ad $h-p$) とします。 $\mathfrak{g}'=\sum_{p\in\mathbf{Z}}\mathfrak{g}^{2p}$ にしましょう。 $\mathfrak{g}$ を次のように考えた場合

$\mathfrak{a}=kx+kh+ky,\mathfrak{g}'$ 上の加群は、奇数次元の単純部分加群の和です (§1, no. 2、提案 2 の修正)。 $l$ (それぞれ $l'$) を $\mathfrak{a}$ モジュールとみなされる $\mathfrak{g}$ (それぞれ $\mathfrak{g}'$) の長さとします。 §1, no. 2までに、

ディム(カーアド$x$)$=l\geq l'=$ディム(カーアド$h$)$\geq$rk($\mathfrak{g}$)。

(i) と (iii) の同値がすぐに続きます。一方、条件 (ii) は、dim(Ker ad $h$) $=$ rk($\mathfrak{g}$) および $\mathfrak{g}'=\mathfrak{g}$ を意味し、他の語では、

dim(Ker ad $h$) $=$ rk($\mathfrak{g}$) と $l=l'$。 (ii)の同値とその他の条件が続きます。

#### 命題 8 {#lie-viii-s11-prop-8 .statement tag=017O}

$\mathfrak{g}$ が半単純 $\not= 0$ であると仮定します。 $\mathfrak{h}$を$\mathfrak{g}$の分割カルタン部分代数、Rを$(\mathfrak{g},\mathfrak{h})$の根系、BをR$,h^0$の基底とし、すべての$\alpha \in B$に対して$\alpha (h^0) = 2$となるような$\mathfrak{h}$の要素とする。

(i) 元 $h^0$ は単純かつ主要です。

(ii) $\mathfrak{g}$ の元 $x$ は、形 $(x, h^0, y)$ の $\mathfrak{s}\mathfrak{l}_2$ トリプレットが存在し、各 $\mathfrak{g}^{\alpha}$ に非ゼロの成分を持つ $\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$ の元が存在します。

元 $h^0$ は、§7, no. 5、補題 2 (cf. loc. cit.、公式 (1)) で考慮されたものです。この補題から、$h^0$は単純な主成分であり、$x\in \sum_{\alpha\in B}\mathfrak{g}^{\alpha}$の各$\mathfrak{g}^{\alpha}$にゼロ以外の成分がある場合、形$(x, h^0, y)$の$\mathfrak{s}\mathfrak{l}_2$トリプレットが存在することがわかります。逆に、$(x, h^0, y)$ を $\mathfrak{s}\mathfrak{l}_2$ の 3 つ組とします。 $[h^0, x] = 2x$があるので、$x\in \sum_{\gamma\in R,\gamma(h^0)=2}\mathfrak{g}^{\gamma}=\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$です。同様に$y\in \sum_{\alpha\in B}\mathfrak{g}^{-\alpha}$。書く

$h^0=\sum_{\alpha\in B}a_{\alpha}H_{\alpha}$ ここで、$a_{\alpha}>0$ はすべての $\alpha \in B$、

$x=\sum_{\alpha\in B}X_{\alpha}$ ここで、$X_{\alpha}\in \mathfrak{g}^{\alpha}$ はすべての $\alpha \in B$ に対して、

$y=\sum_{\alpha\in B}X_{-\alpha}$ ここで、$X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ はすべて $\alpha \in B$ です。

それから

$$
\sum_{\alpha\in B}a_{\alpha}H_{\alpha}=h^0= [y, x] =\sum_{\alpha ,\beta\in B}[X_{-\beta}, X_{\alpha}] =\sum_{\alpha\in B}[X_{-\alpha}, X_{\alpha}]
$$

つまり、すべての $\alpha \in B$ に対して $[X_{-\alpha}, X_{\alpha}]\not= 0$ です。

#### 系 {#lie-viii-s11-n4-cor-1 .statement tag=017P}

分割可能な半単純リー代数には、プリンシパル冪零元が存在します。

分割不可能な半単純リー代数では、0 が唯一の冪零元になる可能性があります。

#### 命題 9 {#lie-viii-s11-prop-9 .statement tag=017Q}

$k$ が代数的に閉じており、$\mathfrak{g}$ が半単純であると仮定します。 $\mathfrak{g}$ のすべての主単純 (それぞれ nilpotent) 元は、Aut$_e(\mathfrak{g})$ では共役です。

提案 8 の記法を維持します。$h$ を主単純元とします。 Aut$_e(\mathfrak{g})$ から $h'\in \mathfrak{h}$ までの共役は、すべての $\alpha \in B$ に対して $\alpha (h')\in  \{0,1,2\}$ となります (no. 3、提案 5)。 $h'$ は主単純なので、すべての $\alpha \in B$ に対して $\alpha (h')\not= 0$ と $\alpha (h')\in 2\mathbf{Z}$、つまりすべての $\alpha \in B$ に対して $\alpha (h') = 2$、したがって $h'=h^0$ になります。これは主単純元に対して主張を証明します。

$x, x'$ を校長冪零元とします。 $\mathfrak{s}\mathfrak{l}_2$の三つ子$(x, h, y)$、$(x', h', y')$が存在します。 By Prop. $7,h$ と $h'$ は主単純であるため、前述の Aut$_e(\mathfrak{g})$ の下で共役になります。したがって、$x$ と $x'$ は Aut$_e(\mathfrak{g})$ の下では共役になります (提案 6)。

#### 補題 9 {#lie-viii-s11-lem-9 .statement tag=017R}

提案 8 の記法により、$p\in \mathbf{Z}$ に $\mathfrak{g}^p=$ Ker(ad $h^0-p$) を入れます。 $\mathfrak{g}^2_*$ を 0 以外の成分を持つ $\mathfrak{g}^2=\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$ の元の集合とします。

それぞれの $\mathfrak{g}^{\alpha}$ で。 $R_+$ を B$,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha}$ と$x\in \mathfrak{g}^2_*$ に対して正の根の集合とします。次に$e^{ad\mathfrak{n}_+}.x=x+ [\mathfrak{n}_+,\mathfrak{n}_+]$。

$e^{ad\mathfrak{n}_+}.x\subset x+ [\mathfrak{n}_+,\mathfrak{n}_+]$であることは明らかです。 $v\in [\mathfrak{n}_+,\mathfrak{n}_+]$ なら $x+v\in e^{ad\mathfrak{n}_+}.x$ であることを証明します。 $\mathfrak{n}^{(p)}=\sum_{r\geq p}\mathfrak{g}^{2r}$を入れてください。それを証明すれば十分です

$$
x+v\in e^{ad\mathfrak{n}_+}.x+\mathfrak{n}^{(p)}
$$

すべての$p\geq 2$に。これは、$\mathfrak{n}^{(2)}$ $= [\mathfrak{n}_+,\mathfrak{n}_+] ($§3, no. 3、提案 9 (iii)) 以来、$p= 2$ については明らかです。 $v+x-e^{adz}.x\in$ $\mathfrak{n}^{(p)}$ となるような $z\in \mathfrak{n}_+$ が見つかったと仮定します。 形 $(x, h^0, y)$ の $\mathfrak{s}\mathfrak{l}_2$ トリプレットが存在するため (提案 8)、§1, no. 2、Cor。提案 2 は、$[x,\mathfrak{g}^{2p-2}] =\mathfrak{g}^{2p}$ を証明します。したがって、次のような $z'\in \mathfrak{g}^{2p-2}\subset \mathfrak{n}_+$ が存在します。

$$
v+x-e^{adz}.x\in [z', x] +\mathfrak{n}^{(p+1)}
$$

したがって、$v+x\in e^{ad(z+z')}.x+\mathfrak{n}^{(p+1)}$、そして私たちの主張は帰納法によって確立されます。

#### 命題 10 {#lie-viii-s11-prop-10 .statement tag=017S}

$\mathfrak{g}$ が半単純であると仮定します。 $\mathfrak{h}$ を $\mathfrak{g}$ の分裂カルタン部分代数、$(\mathfrak{g},\mathfrak{h})$ の R 根系、R の B 基底、B に対して正の根の $R_+$ 集合とします。 $\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha}$。プリンシパル冪零元所属から $\mathfrak{n}_+$ は、すべての $\alpha \in B$ の $\mathfrak{g}^{\alpha}$ に非ゼロの成分を持つ $\mathfrak{n}_+$ の元です。

提案 8 と補題 9 は、そのような元が主虚能であることを証明します。 逆を証明します。明らかに、$\mathfrak{g}$ は単純であると想定できます。 $h^0$ と $\mathfrak{g}^p$ を提案 8 と補題 9 のようにします。 $\omega$ を最高根として、$\omega (h^0) = 2q$ を置きます。 $q=h-1$ があります。ここで、$h$ は R、cf. 章の Coxeter 数です。 VI, §1, no. 11、提案 31。次に、$\mathfrak{g}^{2q}=\mathfrak{g}^{\omega},\mathfrak{g}^{-2q}=\mathfrak{g}^{-\omega}$、および $|k|> q$ に対して $\mathfrak{g}^{2k}= 0$。プリンシパル $\mathfrak{s}\mathfrak{l}_2$-トリプレット $(x^0, h^0, y^0)$ が存在します。 §1, no. 2、Cor.提案 2 の (広告 $x^0$)$^{2q}(\mathfrak{g}^{-\omega}) =\mathfrak{g}^{\omega}$、つまり (広告 $x^0$)$^{2q}\not= 0$。 $x$ を $\mathfrak{g}$ 所属から $\mathfrak{n}_+$ のプリンシパル冪零元とします。 $\overline{k}$ が $k,x\otimes 1$ の代数閉包であり、$x^0\otimes 1$ が $\mathfrak{g}\otimes_k\overline{k}$ の自己同型の下で共役である場合 (提案 9)、(ad $x$)$^{2q}\not= 0$ となります。 (ad $x$)$^{2q}\mathfrak{g}^{\lambda}\not= 0$ となるような $\lambda \in R$ が存在します。 $x_n\in \mathfrak{g}^{2n}$のところに$x=\sum_{n\geq 1}x_n$を入れます。

それから

(広告 $x$)$^{2q}\mathfrak{g}^{\lambda}\subset$ (広告 $x_1$)$^{2q}\mathfrak{g}^{\lambda}+\sum_{k>4q+\lambda(h^0)}\mathfrak{g}^k=$ (広告 $x_1$)$^{2q}\mathfrak{g}^{\lambda}$、$4q+\lambda (h^0)\geq 4q-2q= 2q$ 以来。現在 (ad $x_1$)$^{2q}\mathfrak{g}^{\lambda}\subset \mathfrak{g}^{4q+\lambda(h^0)}$、ここで $\lambda =-\omega$ です。したがって、(ad $x_1$)$^{2q}\mathfrak{g}^{-\omega}=\mathfrak{g}^{\omega}$。すべての$\alpha \in$ B (第 VI, §1, no. 8、注意) には、$\omega =\sum_{\alpha\in B}n_{\alpha}\alpha$ と $n_{\alpha}>0$ があります。 $x_1\in$ となるような $\alpha_0\in B$ が存在する場合

$\sum\mathfrak{g}^{\alpha}$, 関係

$\alpha \in B,\alpha \not=\alpha_0$

$$
\omega  \notin  -\omega +\sum_{\alpha\in B,\alpha\not=\alpha_0}k\alpha
$$

すべての $p$ に対して $\mathfrak{g}^{\omega}\not\subset$ (ad $x_1$)$^p\mathfrak{g}^{-\omega}$ を意味します。これは不合理なので、$\mathfrak{g}^{\alpha}$ の $x_1$ の成分は、すべての $\alpha \in B$ に対して非ゼロになります。

### 練習問題 {#lie-viii-s11-exercises}

[§ 11 に対して練習問題](exercises/s11/)を参照してください。
