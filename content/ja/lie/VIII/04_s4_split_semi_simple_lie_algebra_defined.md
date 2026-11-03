---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 4
section_title: Split semi-simple Lie algebra defined by a reduced root system
lang: ja
source: lie-vii-ix
book_pages: 95-106, 231-233
pdf_pages: 0103-0114, 0239-0241
extraction: native
subsections:
    - "no": 1
      title: FRAMED SEMI-SIMPLE LIE ALGEBRAS
      page: 95
      pdf_page: 103
    - "no": 2
      title: A PRELIMINARY CONSTRUCTION
      page: 96
      pdf_page: 104
    - "no": 3
      title: EXISTENCE THEOREM
      page: 100
      pdf_page: 108
    - "no": 4
      title: UNIQUENESS THEOREM
      page: 104
      pdf_page: 112
statements: 23
exercises: 7
content_sha256: b5f4a87ea2ad7134940cac7b199799a9d7421367eb79c6734e2b946726dadd53
translated_from: content/en/lie/VIII/04_s4_split_semi_simple_lie_algebra_defined.md
translation_method: google
source_content_sha256: d31efd9ddbb6c9db525488b6ea28a82ed909217def1e86239e848957a5f5eb01
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 852ddceb7ccb9610e331c2994bd757ba503225c882c29218e0403db3705eefeb
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。 分裂半単純リー代数によって定義されます約根系

### 1. 額入り半単純リー代数

#### 命題 1 {#lie-viii-s4-prop-1 .statement tag=010T}

$(\mathfrak{g},\mathfrak{h})$ を分裂半単純リー代数、R をその根系、B を R の基底、そして $(n(\alpha , \beta ))_{\alpha ,\beta\in B}$ 対応するカルタン行列とします。すべての $\alpha \in B$ について、$X_{\alpha}\in \mathfrak{g}^{\alpha}, X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ にします。次に、$\alpha , \beta \in B$については、

$$
[H_{\alpha}, H_{\beta}] = 0 \tag{1}
$$

$$
[H_{\alpha}, X_{\beta}] =n(\beta , \alpha )X_{\beta} \tag{2}
$$

$$
[H_{\alpha}, X_{-\beta}] =-n(\beta , \alpha )X_{-\beta} \tag{3}
$$

$[X_{-\alpha}, X_{\beta}] = 0$ $\alpha \not=\beta$ の場合 (4)

(広告 $X_{\alpha}$)$^{1-n(\beta ,\alpha)}X_{\beta}= 0$ if $\alpha \not=\beta$ (5)

(広告 $X_{-\alpha}$)$^{1-n(\beta ,\alpha)}X_{-\beta}= 0$ $\alpha \not=\beta$ の場合。 (6)

ファミリ $(H_{\alpha})_{\alpha\in B}$ は $\mathfrak{h}$ の基底です。すべての$\alpha \in B$に対して$X_{\alpha}\not= 0$と$X_{-\alpha}\not= 0$があれば、$X_{\alpha}$と$X_{-\alpha}(\alpha \in B)$によってリー代数$\mathfrak{g}$が生成されます。

($\alpha , \beta \in B$ と $\alpha \not=\beta ,n(\beta , \alpha )$ が整数 $\leq 0$ である場合、公式 (5) と (6) は意味を成します。)

公式 (1)、(2)、(3) はクリアです。 R のすべての元が B の元の線形結合であり、整数係数はすべて同じ符号であるため、$\alpha \not=\beta ,\beta -\alpha$ が根でない場合 (第 3 章、VI, §1, no. 6)。 これは (4) を証明します。 章の観点から。 VI, §1, no. 3、提案 9、これは、$\beta$ によって定義される $\alpha$ チェーンが

$$
\{\beta , \beta +\alpha , . . . , \beta -n(\beta , \alpha )\alpha \}
$$

したがって $\beta +(1-n(\beta , \alpha ))\alpha  \notin R$ となり、(5) が証明されます。 等式 (6) も同様に成立します。ファミリ $(H_{\alpha})_{\alpha\in B}$ は $R^{\vee}$ の基底であり、したがって $\mathfrak{h}$ の基底です。すべての $\alpha \in B$ に対して $X_{\alpha}\not= 0$ と $X_{-\alpha}\not= 0$ の場合、$\lambda_{\alpha}\not= 0$ で $[X_{\alpha}, X_{-\alpha}] =\lambda_{\alpha}H_{\alpha}$ となるため、§3, no. 3、提案 9 (iii) から最後の主張が続きます。

#### 定義 1 {#lie-viii-s4-def-1 .statement tag=010U}

$(\mathfrak{g},\mathfrak{h})$ を分裂半単純リー代数とすると、R は根系となります。 $(\mathfrak{g},\mathfrak{h})$ のフレーミングは対 $(B,(X_{\alpha})_{\alpha\in B})$ であり、B は R の基底であり、すべての $\alpha \in B,X_{\alpha}$ は $\mathfrak{g}^{\alpha}$ の非ゼロ元です。フレーム化された半単純リー代数は数列 $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ で、$(\mathfrak{g},\mathfrak{h})$ は分裂半単純リー代数で、$(B,(X_{\alpha})_{\alpha\in B})$ は $(\mathfrak{g},\mathfrak{h})$ のフレーム化です。

$\mathfrak{g}$ のフレームは $(\mathfrak{g},\mathfrak{h})$ のフレームであり、$\mathfrak{h}$ は $\mathfrak{g}$ の分裂カルタン部分代数です。

$a_1= (\mathfrak{g}_1,\mathfrak{h}_1,B_1,(X_{\alpha}^1)_{\alpha\in B_1})$ と $a_2= (\mathfrak{g}_2,\mathfrak{h}_2,B_2,(X_{\alpha}^2)_{\alpha\in B_2})$ を半単純リー代数で囲みます。 $a_1$から$a_2$までの同型は、$\mathfrak{g}_1$から$\mathfrak{g}_2$までの同型$\varphi$で、すべて$\mathfrak{h}_1$から$\mathfrak{h}_2, B_1$、$B_2$、$X_{\alpha}^1$から$X_{\psi \alpha}^2$かかります$\alpha \in B_1$ ($\psi$ は $\varphi |\mathfrak{h}_1$ の反格写像です)。この場合、$\varphi$は変換、枠$(B_1,(X_{\alpha}^1)_{\alpha\in B_1})$は枠$(B_2,(X_{\alpha}^2)_{\alpha\in B_2})$と言われます。

$(B,(X_{\alpha})_{\alpha\in B})$ が $(\mathfrak{g},\mathfrak{h})$ のフレームである場合、$\mathfrak{g}^{-\alpha}$ のすべての $\alpha \in B$、一意元 $X_{-\alpha}$ について、$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}($§2, no. 2 が存在します。 1(iv))。ファミリ $(X_{\alpha})_{\alpha\in B\cup(-B)}$ は、フレーミング (cf. Prop.1) によって定義される生成するファミリと呼ばれます。これも、フレーミング $(-B,(X_{\alpha})_{\alpha\in -B})$ によって定義される生成するファミリです。すべての $\alpha \in B\cup (-B)$ について、$t_{\alpha}\in k^*$ とし、すべての $\alpha \in B$ について $t_{\alpha}t_{-\alpha}= 1$ と仮定します。この場合、$(t_{\alpha}X_{\alpha})_{\alpha\in B\cup(-B)}$ は、枠組み $(B,(t_{\alpha}X_{\alpha})_{\alpha\in B})$ によって定義される生成するファミリになります。

### 2. 予備構成

この数と次のベクトル空間VのR約根系とRのB基底で表します。Bに対するカルタン行列を$(n(\alpha , \beta ))_{\alpha ,\beta\in B}$で表します。$n(\alpha , \beta ) =\langle \alpha , \beta^{\vee}\rangle$を思い出してください。 R が分裂半単純リー代数の根系であり、同型までは一意であることを示します。主に、提案 1 の関係によって定義されるリー代数を検討します。

この数の構成は、行列式が非ゼロの $k$ を超える平方行列 $(n(\alpha , \beta ))_{\alpha ,\beta\in B}$ に適用され、すべての $\alpha \in B$ に対して $n(\alpha , \alpha ) = 2$ が適用されます (cf. 第 3 章)。 VI, §1, no. 10、公式 (14))。

E を $k$ 上の集合 B の自由結合代数とします。 E は $\mathbf{N}$ 段階に評価されている (代数、Chap. III, §3, no. 1、例 3) ことを思い出してください。 ベクトル空間 E、次数 $1,0,-1$ のそれぞれの $\alpha \in B$ 自己準同型 $X_{-\alpha}^0, H_{\alpha}^0, X_{\alpha}^0$ に関連付けます。 B の元の任意の語 $(\alpha_1, . . . , \alpha_n)$ について、

$$
X_{-\alpha}^0(\alpha_1, . . . , \alpha_n) = (\alpha , \alpha_1, . . . , \alpha_n) \tag{7}
$$

$$
H_{\alpha}^0(\alpha_1, . . . , \alpha_n) =(-\sum_{i=1}^nn(\alpha_i, \alpha ))(\alpha_1, . . . , \alpha_n) \tag{8}
$$

一方、$X_{\alpha}^0(\alpha_1, . . . , \alpha_n)$ は、公式を使用して、$n$ の帰納法によって定義されます。

$$
X_{\alpha}^0(\alpha_1, . . . , \alpha_n) = (X_{-\alpha_1}^0X_{\alpha}^0-\delta_{\alpha ,\alpha_1}H_{\alpha}^0)(\alpha_2, . . . , \alpha_n) \tag{9}
$$

ここで、$\delta_{\alpha ,\alpha_1}$ はクロネッカー記号です。 $(\alpha_1, . . . , \alpha_n)$が空の語であれば、$X_{\alpha}^0(\alpha_1, . . . , \alpha_n)$は零であることがわかります。

#### 補題 1 {#lie-viii-s4-lem-1 .statement tag=010V}

$\alpha , \beta \in B$ の皆様には、

$$
[X_{\alpha}^0, X_{-\alpha}^0] =-H_{\alpha}^0 \tag{10}
$$

$$
[H_{\alpha}^0, H_{\beta}^0] = 0 \tag{11}
$$

$$
[H_{\alpha}^0, X_{\beta}^0] =n(\beta , \alpha )X_{\beta}^0 \tag{12}
$$

$$
[H_{\alpha}^0, X_{-\beta}^0] =-n(\beta , \alpha )X_{-\beta}^0 \tag{13}
$$

$\alpha \not=\beta$なら$[X_{\alpha}^0, X_{-\beta}^0] = 0$。 (14)

確かに、関係 (9) は次のように書くことができます。

$$
(X_{\alpha}^0X_{-\alpha_1}^0)(\alpha_2, . . . , \alpha_n) = (X_{-\alpha_1}^0X_{\alpha}^0)(\alpha_2, . . . , \alpha_n)-\delta_{\alpha ,\alpha_1}H_{\alpha}^0(\alpha_2, . . . , \alpha_n)
$$

これは (10) と (14) を証明します。 関係 (11) はクリアです。次

$$
[H_{\alpha}^0, X_{-\beta}^0](\alpha_1, . . . , \alpha_n) =H_{\alpha}^0(\beta , \alpha_1, . . . , \alpha_n)+(\sum_{i=1}^nn(\alpha_i, \alpha ))(\beta , \alpha_1, . . . , \alpha_n)
$$

$$
=-n(\beta , \alpha )(\beta , \alpha_1, . . . , \alpha_n)
$$

$$
=-n(\beta , \alpha )X_{-\beta}^0(\alpha_1, . . . , \alpha_n)
$$

したがって(13)。最後に、

$0 = [H_{\alpha}^0,[X_{\beta}^0, X_{-\gamma}^0]]$ by $(10),(11),(14)$ (15)

$$
= [[H_{\alpha}^0, X_{\beta}^0], X_{-\gamma}^0] + [X_{\beta}^0,[H_{\alpha}^0, X_{-\gamma}^0]]
$$

$= [[H_{\alpha}^0, X_{\beta}^0]-n(\gamma , \alpha )X_{\beta}^0, X_{-\gamma}^0]$ by (13)

$= [[H_{\alpha}^0, X_{\beta}^0]-n(\beta , \alpha )X_{\beta}^0, X_{-\gamma}^0]$ by (14);

さて、空の語を考えると、すぐに次のようになります。

$$
([H_{\alpha}^0, X_{\beta}^0]-n(\beta , \alpha )X_{\beta}^0)(\emptyset ) = 0
$$

したがって、(15) は次のことを意味します

$$
([H_{\alpha}^0, X_{\beta}^0]-n(\beta , \alpha )X_{\beta}^0)X_{-\gamma_1}^0X_{-\gamma_2}^0. . . X_{-\gamma_n}^0(\emptyset ) = 0
$$

すべての$\gamma_1, . . . , \gamma_n\in B$;これは (12) を証明します。

#### 補題 2 {#lie-viii-s4-lem-2 .statement tag=010W}

自己準同型 $X_{\alpha}^0,H_{\beta}^0,X_{-\gamma}^0$、ここで $\alpha , \beta , \gamma \in B$ は線形独立です。

$X_{-\alpha}^0(\emptyset ) =\alpha$ なので、$X_{-\alpha}^0$ が線形独立であることは明らかです。

$\sum_{\alpha}a_{\alpha}H_{\alpha}^0= 0$; と仮定します。それでは、$\beta \in B$ 全員に対して、

$$
0 =[\sum_{\alpha}a_{\alpha}H_{\alpha}^0, X_{-\beta}^0]=-\sum_{\alpha}a_{\alpha}n(\beta , \alpha )X_{-\beta}^0
$$

det($n(\beta , \alpha )$)$\not= 0$ なので、すべての $\alpha$ について $a_{\alpha}$ = 0 となります。 $\sum_{\alpha}a_{\alpha}X_{\alpha}^0= 0$ と仮定します。 公式 (7)、(8)、(9) を考慮すると、

$$
X_{\alpha}^0(\beta ) = 0
$$

$$
X_{\alpha}^0(\beta , \beta ) = 2\delta_{\alpha \beta}\beta
$$

すべての$\beta \in B$のために。すべての $\beta$ に対して $a_{\beta}= 0$ ということになります。 $X_{\alpha}^0, H_{\alpha}^0, X_{-\alpha}^0$ はそれぞれ次数 $-1,0,1$ であるため、前にの後には補題が続きます。

I を集合 $B\times  \{-1,0,1\}$ とします。 $x_{\alpha}= (\alpha ,-1),h_{\alpha}= (\alpha ,0)$と$x_{-\alpha}= (\alpha ,1)$を入れます。 $\mathfrak{a}$ を、生成する家族 I とそれに続く関係者の集合 $\mathscr{R}$ によって定義されるリー代数とします。

$$
[h_{\alpha}, h_{\beta}]
$$

$$
[h_{\alpha}, x_{\beta}]-n(\beta , \alpha )x_{\beta}
$$

$$
[h_{\alpha}, x_{-\beta}] +n(\beta , \alpha )x_{-\beta}
$$

$$
[x_{\alpha}, x_{-\alpha}] +h_{\alpha}
$$

$\alpha \not=\beta$なら$[x_{\alpha}, x_{-\beta}]$

(cf.章II, §2, no. 3)。 補題 1 までに、E には次のような固有の線型表現 $\rho$ の $\mathfrak{a}$ が存在します。

$$
\rho (x_{\alpha}) =X_{\alpha}^0, \rho (h_{\alpha}) =H_{\alpha}^0, \rho (x_{-\alpha}) =X_{-\alpha}^0
$$

補題 2 を考慮すると、これは次の結果を証明します。

#### 補題 3 {#lie-viii-s4-lem-3 .statement tag=010X}

元 $x_{\alpha}, h_{\beta}, x_{-\gamma}$ の $\mathfrak{a}$ の標準像 ($\alpha , \beta , \gamma \in B$) は線形独立です。

以下では、私たちは同一視する $x_{\alpha}, h_{\alpha}, x_{-\alpha}$ と彼らの標準像は $\mathfrak{a}$ にあります。

#### 補題 4 {#lie-viii-s4-lem-4 .statement tag=010Y}

次のような $\mathfrak{a}$ の固有の包含自己同型 $\theta$ が存在します。

$$
\theta (x_{\alpha}) =x_{-\alpha}, \theta (x_{-\alpha}) =x_{\alpha}, \theta (h_{\alpha}) =-h_{\alpha}
$$

$\alpha \in B$ 全員のために。

確かに、自由なリー代数 L(I) 満たすこれら条件の包含的な自己同型が存在します。 $\mathscr{R}\cup (-\mathscr{R})$ は安定したままになるため、定義するは商への通過により、$\mathfrak{a}$ 満たす条件の補題の包含的な自己同型になります。 一意性は、$\mathfrak{a}$ が元 $x_{\alpha}, h_{\alpha}, x_{-\alpha}(\alpha \in B)$ によって生成されるという事実から導き出されます。

この自己同型は、$\mathfrak{a}$の正準包含自己同型と呼ばれます。

Let Q be the set of radical weights of R; this is a free $\mathbf{Z}$-module with basis B (Chap. VI, §1, no. 9). There exists a graduation of type Q on the free Lie algebra L(I) such that $x_{\alpha}, h_{\alpha}, x_{-\alpha}$ are of degrees $\alpha ,0,-\alpha$, respectively (Chap. II, §2, no. 6). これで、$\mathscr{R}$ の元が同種になりました。 したがって、$\mathfrak{a}$のリー代数構造と互換性があり、$x_{\alpha}, h_{\alpha}, x_{-\alpha}$がそれぞれ次数$\alpha ,0,-\alpha$であるような$\mathfrak{a}$には型Qという固有の段階が存在します。 任意の $\mu\in Q$ について、次数 $\mu$ の同種の元の $\mathfrak{a}$ の $\mathfrak{a}^\mu$ 集合で表します。

#### 補題 5 {#lie-viii-s4-lem-5 .statement tag=010Z}

$z\in \mathfrak{a}$ にしましょう。次に、すべての $\alpha \in B$ に対して $[h_{\alpha}, z] =\langle \mu, \alpha^{\vee}\rangle z$ である場合に限り、$z\in \mathfrak{a}^\mu$ になります。

$\mu\in Q$ の場合、$\mathfrak{a}^{(\mu)}$ を $x\in \mathfrak{a}$ の集合とし、すべての $\alpha \in B$ に対して $[h_{\alpha}, x] =\langle \mu, \alpha^{\vee}\rangle x$ とします。 $\mathfrak{a}^{(\mu)}$ の和は直接です。 したがって、補題を証明するには、$\mathfrak{a}^\mu\subset \mathfrak{a}^{(\mu)}$ を示すだけで十分です。 $\alpha \in B$ にしましょう。 $u|\mathfrak{a}^\mu=\langle \mu, \alpha^{\vee}\rangle .1$ が $\mathfrak{a}$ の導分であるように、$x=x_{\beta}, x=h_{\beta}, x=x_{-\beta}$ に対して $ux=$ (広告 $h_{\alpha}$)$.x$ となるように、ベクトル空間 $\mathfrak{a}$ の自己準同型 $u$。したがって、$u=$ と $h_{\alpha}$ は、主張であることを証明します。

#### 注意 {#lie-viii-s4-n2-rem-1 .statement tag=0110}

補題 5 から、$\mathfrak{a}$ のすべての理想は、広告 $h_{\alpha}$ の下で安定しているため、均一であることがわかります。

B の $Q_+$ (それぞれ $Q_-$) 集合、線形結合、元を、すべて零ではなく、プラス (それぞれマイナス) 整数係数で表します。 $\mathfrak{a}_+=$ $\sum_{\mu\in Q_+}a^\mu$ と $\mathfrak{a}_-=\sum_{\mu\in Q_-}\mathfrak{a}^\mu$ を入れます。 $Q_++ Q_+\subset Q_+$ と $Q_-+ Q_-\subset Q_-,\mathfrak{a}_+$ から

と $\mathfrak{a}_-$ は $\mathfrak{a}$ の嘘部分代数です。

#### 命題 2 {#lie-viii-s4-prop-2 .statement tag=0111}

(i) リー代数 $\mathfrak{a}_+$ は家族 $(x_{\alpha})_{\alpha\in B}$ によって生成されます。

(ii) リー代数 $\mathfrak{a}_-$ は家族 $(x_{-\alpha})_{\alpha\in B}$ によって生成されます。

(iii) 家族 $(h_{\alpha})_{\alpha\in B}$ はベクトル空間 $\mathfrak{a}^0$ の基底です。

(iv) ベクトル空間 $\mathfrak{a}$ は $\mathfrak{a}_+,\mathfrak{a}^0,\mathfrak{a}_-$ の直和です。

$\mathfrak{r}$ (それぞれ $\mathfrak{n}$) を、$(x_{\alpha})_{\alpha\in B}$ (それぞれ $(x_{-\alpha})_{\alpha\in B}$) によって生成された $\mathfrak{a}$ の嘘部分代数と、$(h_{\alpha})_{\alpha\in B}$ によって生成された $\mathfrak{a}$ の$\mathfrak{h}$ ベクトル部分空間とします。 $x_{\alpha}$ は均質であるため、$\mathfrak{a}_+,\mathfrak{r}$ の元は $\mathfrak{a}_+$ の等級付けされた部分代数です。したがって、$[\mathfrak{h},\mathfrak{r}]\subset \mathfrak{r}$ なので、$\mathfrak{h}+\mathfrak{r}$ は $\mathfrak{a}$ の部分代数です。以来

$$
[x_{-\alpha}, x_{\beta}] =\delta_{\alpha \beta}h_{\alpha}
$$

$\alpha \in B$ 全員に対して $[x_{-\alpha},\mathfrak{r}]\subset \mathfrak{h}+\mathfrak{r}$。同様に、$\mathfrak{n}$ は $\mathfrak{a}_-$ の部分代数であり、$[\mathfrak{h},\mathfrak{n}]\subset \mathfrak{n},\mathfrak{h}+\mathfrak{n}$ は $\mathfrak{n}$ の部分代数であり、すべての $\alpha \in B$ については $[x_{\alpha},\mathfrak{n}]\subset \mathfrak{h}+\mathfrak{n}$ です。 $\mathfrak{a}'=\mathfrak{r}+\mathfrak{h}+\mathfrak{n}$を入れます。前述の結果は、$\mathfrak{a}'$ が、すべての $\alpha \in B$ に対して ad $x_{\alpha}$、ad $h_{\alpha}$、ad $x_{-\alpha}$ の下で安定しており、したがって $\mathfrak{a}$ の理想であることを示しています。 $\mathfrak{a}'$ 含む $x_{\alpha}, h_{\alpha}, x_{-\alpha}$ 以降、すべての $\alpha \in B,\mathfrak{a}'=\mathfrak{a}$ に対して。このことから、包含物 $\mathfrak{r}\subset \mathfrak{a}_+,\mathfrak{h}\subset \mathfrak{a}^0$、$\mathfrak{n}\subset \mathfrak{a}_-$ は等価であることがわかり、命題が証明されます。

#### 命題 3 {#lie-viii-s4-prop-3 .statement tag=0112}

リー代数 $\mathfrak{a}_+$ (それぞれ $\mathfrak{a}_-$) は、基本ファミリー $(x_{\alpha})_{\alpha\in B}$ (それぞれ $(x_{-\alpha})_{\alpha\in B}$) (cf. チャプター II, §2, no. 3) を備えた無料のリー代数です。

Bが生成したEの嘘部分代数をLとします。 章著。 II, §3、木。 1、Lは、Bが生成した無料のリー代数と識別できます。 それ自体の E の左の正則表現は明らかに単射であり、制限から L までの定義するは E のリー代数 L の単射表現 $\rho '$ です。 $\varphi$ を L から $\mathfrak{a}_-$ までの一意な準同型とすると、すべての $\alpha \in B$ に対して $\alpha$ から $x_{-\alpha}$ がかかります。 すると、すべての $\alpha \in B,\rho (\varphi (\alpha ))$ は E 上の $\alpha$ による左乗法の自己準同型であるため、$\rho \circ \varphi =\rho '$ となり、$\varphi$ が単射であることが証明されます。 したがって、$(x_{-\alpha})_{\alpha\in B}$ は $\mathfrak{a}_-$ の基本ファミリです。 すべての$\alpha$ (cf. 補題 $4$)$, (x_{\alpha})_{\alpha\in B}$ に対する$\theta (x_{-\alpha}) =x_{\alpha}$ が、$\mathfrak{a}_+$ の基本ファミリーです。

### 3. 存在定理

仮説と前述の数の記法を保持します。 $\alpha , \beta \in B$ の場合、および $\alpha \not=\beta$ の場合、$n(\beta , \alpha )\leq 0$ であることを思い出してください。さらに、$n(\beta , \alpha ) = 0$ の場合は、$n(\alpha , \beta ) = 0$ (VI, §1, no. 1、公式 (8) 章)。 B の個別の元の任意の対 $(\alpha , \beta )$ について、

$x_{\alpha \beta}=$ (広告$x_{\alpha}$)$^{1-n(\beta ,\alpha)}x_{\beta}y_{\alpha \beta}=$ (広告$x_{-\alpha}$)$^{1-n(\beta ,\alpha)}x_{-\beta}$。

次に$x_{\alpha \beta}\in \mathfrak{a}_+, y_{\alpha \beta}\in \mathfrak{a}_-$。 $\theta$ が $\mathfrak{a}$、$\theta (x_{\alpha \beta}) =y_{\alpha \beta}$ の正規の自己同型を表す場合。

#### 補題 6 {#lie-viii-s4-lem-6 .statement tag=0113}

$\alpha , \beta \in B$ を $\alpha \not=\beta$ とします。それから

$$
[\mathfrak{a}_+, y_{\alpha \beta}] = 0[\mathfrak{a}_-, x_{\alpha \beta}] = 0
$$

2 番目の公式は、自己同型 $\theta$ を使用して最初の公式に続きます。最初のことを証明するには、すべての $\gamma \in B$ に対して $[x_{\gamma}, y_{\alpha \beta}] = 0$ であることを証明すれば十分です。 3 つのケースを区別します。

ケース 1$:\gamma \not=\alpha$ と $\gamma \not=\beta$。この場合、$x_{\gamma}$ は $x_{-\alpha}$ および $x_{-\beta}$ と交換するため、$y_{\alpha \beta}$ と交換します。

ケース2$:\gamma =\beta$。この場合、$x_{\gamma}$ は $x_{-\alpha}$ と通勤するため、

$[x_{\gamma}, y_{\alpha \beta}] =$ (広告 $x_{-\alpha}$)$^{1-n(\beta ,\alpha)}[x_{\gamma}, x_{-\beta}]$

$=-$(広告$x_{-\alpha}$)$^{1-n(\beta ,\alpha)}h_{\beta}=-n(\alpha , \beta$)(広告$x_{-\alpha}$)$^{-n(\beta ,\alpha)}x_{-\alpha}$。

$n(\beta , \alpha )<0$ の場合、(ad $x_{-\alpha}$)$.x_{-\alpha}= 0$ 以降、この式は零になります。 $n(\beta , \alpha ) = 0$の場合は、$n(\alpha , \beta ) = 0$。どちらの場合も、$[x_{\gamma}, y_{\alpha \beta}] = 0$です。

ケース 3$:\gamma =\alpha$。 $\mathfrak{a}$の自己準同型の代数、$[$-広告$h_{\alpha}$、広告$x_{-\alpha}] = 2$広告$x_{-\alpha}$

そして [広告 $x_{\alpha}$, 広告 $x_{-\alpha}] =$-広告 $h_{\alpha}$;従って、§1、補題 1、

[広告 $x_{\alpha}$, (広告 $x_{-\alpha}$)$^{1-n(\beta ,\alpha)}] = (1-n(\beta , \alpha$))(広告 $x_{-\alpha}$)$^{-n(\beta ,\alpha)}($-広告 $h_{\alpha}-n(\beta , \alpha ))$。

その結果、

$[x_{\gamma}, y_{\alpha \beta}] =$ [広告$x_{\alpha}$, (広告$x_{-\alpha}$)$^{1-n(\beta ,\alpha)}]x_{-\beta}+$ (広告$x_{-\alpha}$)$^{1-n(\beta ,\alpha)}$(広告$x_{\alpha}$)$x_{-\beta}$

$=-(1-n(\beta , \alpha$))(広告$x_{-\alpha}$)$^{-n(\beta ,\alpha)}$(広告$h_{\alpha}+n(\beta , \alpha )$)$x_{-\beta}$

+ (広告$x_{-\alpha}$)$^{1-n(\beta ,\alpha)}$(広告$x_{\alpha}$)$x_{-\beta}$。

今$[h_{\alpha}, x_{-\beta}] +n(\beta , \alpha )x_{-\beta}= 0$と$[x_{\alpha}, x_{-\beta}] = 0$なので、$[x_{\gamma}, y_{\alpha \beta}] = 0$です。

#### 補題 7 {#lie-viii-s4-lem-7 .statement tag=0114}

$x_{\alpha \beta}(\alpha , \beta \in B, \alpha \not=\beta )$が生み出す$\mathfrak{a}_+$の理想$\mathfrak{n}$は、$\mathfrak{a}$の理想です。 $y_{\alpha \beta}(\alpha , \beta \in B, \alpha \not=\beta )$ によって生成される $\mathfrak{a}_-$ の理想は、$\mathfrak{a}$ の理想であり、$\theta (\mathfrak{n})$ に等しくなります。

$\mathfrak{n}'=\sum_{\alpha ,\beta\in B,\alpha\not=\beta}kx_{\alpha \beta}$ にしましょう。それぞれの $x_{\alpha \beta}$ は $\mathfrak{a}, [\mathfrak{a}^0,\mathfrak{n}']\subset \mathfrak{n}'$ で同次であるため

(補題 5 および提案 2)。 U (それぞれ V) を、$\mathfrak{a}$ (それぞれ $\mathfrak{a}_+$) を包む代数とし、$\mathfrak{a}$ の随伴表現によって定義される $\mathfrak{a}$ 上の U の$\sigma$ 表現とします。 $\mathfrak{n}'$が生み出す$\mathfrak{a}$の理想は$\sigma (U)\mathfrak{n}'$です。現在、$\mathfrak{a}=\mathfrak{a}_++\mathfrak{a}^0+\mathfrak{a}_-$ (提案 $2$)$,\sigma (\mathfrak{a}_-)\mathfrak{n}'= 0$ (補題 6)、および前述の$\sigma (\mathfrak{a}^0)\mathfrak{n}'\subset \mathfrak{n}'$ です。ポアンカレ・バーコフ・ウィット定理、$\sigma (U)\mathfrak{n}'=\sigma (V)\mathfrak{n}'$ により、補題の最初の主張が証明されます。したがって、$\theta (x_{\alpha \beta}) =y_{\alpha \beta}(\alpha , \beta \in B, \alpha \not=\beta )$によって生成される$\theta (\mathfrak{a}_+) =\mathfrak{a}_-$の理想は、$\mathfrak{a}$の理想$\theta (\mathfrak{n})$となる。 Q.E.D.

$\mathfrak{a}$ の理想的な $\mathfrak{n}+\theta (\mathfrak{n})$ は、均質な元によって生成されるため、等級付けされます。従って、リー代数 $\mathfrak{a}/(\mathfrak{n}+\theta (\mathfrak{n}))$ は Q グレードのリー代数です。この段落の残りの部分では、$\mathfrak{g}_B$ または単に $\mathfrak{g}$ で示されます。提案 2 により、$\mathfrak{g}^\mu\not= 0$ の場合は、$\mu\in Q_+$、または $\mu\in Q_-$、または $\mu= 0$ になります。 $\mathfrak{g}$ の $x_{\alpha}$ (それぞれ $h_{\alpha}, x_{-\alpha}$) の $X_{\alpha}$ (それぞれ $H_{\alpha}, X_{-\alpha}$) 標準像で表します。 $\mathfrak{a},\mathfrak{n}$ と $\theta (\mathfrak{n})$ の定義を考慮すると、$\mathfrak{g}$ は生成する家族 $((X_{\alpha}, H_{\alpha}, X_{-\alpha}))_{\alpha\in B}$ と関係によって定義されるリー代数であることがわかります。

$$
[H_{\alpha}, H_{\beta}] = 0 \tag{16}
$$

$$
[H_{\alpha}, X_{\beta}]-n(\beta , \alpha )X_{\beta}= 0 \tag{17}
$$

$$
[H_{\alpha}, X_{-\beta}] +n(\beta , \alpha )X_{-\beta}= 0 \tag{18}
$$

$$
[X_{\alpha}, X_{-\alpha}] +H_{\alpha}= 0 \tag{19}
$$

$$
[X_{\alpha}, X_{-\beta}] = 0(\alpha \not=\beta ) \tag{20}
$$

(広告$X_{\alpha}$)$^{1-n(\beta ,\alpha)}X_{\beta}= 0(\alpha \not=\beta )$ (21)

(広告$X_{-\alpha}$)$^{1-n(\beta ,\alpha)}X_{-\beta}= 0(\alpha \not=\beta )$。 (22)

$z\in \mathfrak{g}$と$\mu\in Q$としましょう。次に、すべての $\alpha \in B$ が $[H_{\alpha}, z] =\langle \mu, \alpha^{\vee}\rangle z$ である場合に限り、$z\in \mathfrak{g}^\mu$ になります。これは補題 5 から続きます。

$\mathfrak{a}^0\cap (\mathfrak{n}+\theta (\mathfrak{n})) = 0$ 以降、$\mathfrak{a}^0$ から $\mathfrak{g}^0$ までの正規の写像は同型です。従って、$(H_{\alpha})_{\alpha\in B}$ はベクトル空間 $\mathfrak{g}^0$ の基底です。 $\mathfrak{g}_B$ の可換部分代数 $\mathfrak{g}^0$ は、$\mathfrak{h}_B$ または単に $\mathfrak{h}$ で表されます。すべての $\mu\in V$ とすべての $\alpha \in B$ に対して $\langle \mu_B, H_{\alpha}\rangle =\langle \mu, \alpha^{\vee}\rangle$ となるように、V から $\mathfrak{h}^*$ までの一意の同型 $\mu \rightarrow \mu_B$ が存在します。

$\mathfrak{a}$ 定義するの包含自己同型 $\theta$ は、商への通過により、$\mathfrak{g}$ の包含自己同型となり、$\theta$ によっても示されます。 $\alpha \in B\cup (-B)$、$\theta (H_{\alpha}) =-H_{\alpha}$には$\theta (X_{\alpha}) =X_{-\alpha}$がございます。

#### 定理 1 {#lie-viii-s4-thm-1 .statement tag=0115}

R を R の約根系、B 基底とします。$\mathfrak{g}$ を、生成するファミリー$((X_{\alpha}, H_{\alpha}, X_{-\alpha}))_{\alpha\in B}$ と関係 (16) ～ (22) で定義されるリー代数とします。 $\mathfrak{h}=\sum_{\alpha\in B}kH_{\alpha}$ にしましょう。すると、$(\mathfrak{g},\mathfrak{h})$は分裂半単純リー代数となります。 同型 $(\mathfrak{g},\mathfrak{h})$ の V から $\mathfrak{h}^*$ 写像 R から根系までの $\mu \rightarrow \mu_B$。すべてにおいて、$\mu\in R,\mathfrak{g}^\mu$ は根 $\mu$ に対する固有空間です。

証明は、補題 8、9、10、11 に続きます。

#### 補題 8 {#lie-viii-s4-lem-8 .statement tag=0116}

$\alpha \in B\cup (-B)$ にしましょう。この場合、広告 $X_{\alpha}$ は局所的には無能です。$^1$

$\alpha \in B$ と仮定します。 $\mathfrak{g}'$ を $z\in \mathfrak{g}$ の集合として、十分大きい $p$ に対して (ad $X_{\alpha}$)$^pz= 0$ とします。 ad $X_{\alpha}$ は $\mathfrak{g},\mathfrak{g}'$ の導分であるため、 $\mathfrak{g}$ の部分代数です。 (21) までに、$X_{\beta}\in \mathfrak{g}'$ はすべての $\beta \in B$ に適用されます。 (17)、(19)、(20)、$H_{\beta}\in \mathfrak{g}'$、$X_{-\beta}\in \mathfrak{g}'$ により、すべての $\beta \in B$ が対象となります。したがって、$\mathfrak{g}'=\mathfrak{g}$ と広告 $X_{\alpha}$ は局所的に nilpotent です。 ad $X_{-\alpha}=\theta$(ad $X_{\alpha}$)$\theta^{-1}$ なので、ad $X_{-\alpha}$ は局所的に nilpotent であることがわかります。

$\mathfrak{g}$ は有限次元であるため、広告 $X_{\alpha}$ は実際には零能であることがわかります。

#### 補題 9 {#lie-viii-s4-lem-9 .statement tag=0117}

$\mu, \nu \in Q$ と $w\in W(R)$ を $w\mu=\nu$ となるようにします。 $\mathfrak{g}^\mu$から$\mathfrak{g}^{\nu}$までかかる$\mathfrak{g}$の自己同型が存在します。

すべての $\alpha \in B$ について、$s_{\alpha}$ を $\alpha$ によって定義された V の反映とします。 W(R) は$s_{\alpha}$ (VI, §1, no. 5, 注意 1 章) によって生成されるため、$w=s_{\alpha}$ のときに補題を証明すれば十分です。 補題 8 を考慮すると、定義するが可能です

$$
\theta_{\alpha}=e^{adX_{\alpha}}e^{adX_{-\alpha}}e^{adX_{\alpha}}
$$

第 4 章のように検証されます。 I, §6, no. 8、その$\theta_{\alpha}$は$\mathfrak{g}$の自己同型です。私たちは持っています

ベクトル空間 V の $^1$ 自己準同型 $u$ は、局所的には無能 (またはほぼゼロ) と呼ばれます

無能) $v\in V$ ごとに、$u^n(v) = 0$ となるような正の整数 $n$ が存在する場合

(cf. 可換代数、章 IV, §1, no. 4、定義 2)。すると、exp($u$)、つまり$e^u$は、

すべての $v\in V$ に対して公式 $e^u(v) =\sum_{n\geq 0}(1/n$!)$u^n(v)$ によって定義されます。 $\theta_{\alpha}(H_{\alpha}) =e^{adX_{\alpha}}e^{adX_{-\alpha}}(H_{\beta}-n(\alpha , \beta )X_{\alpha})$

$$
=e^{adX_{\alpha}}(H_{\beta}-n(\alpha , \beta )X_{\alpha}+n(\alpha , \beta )X_{-\alpha}-n(\alpha , \beta )H_{\alpha}-\frac{n(\alpha , \beta)}{2}2X_{-\alpha})
$$

$$
=e^{adX_{\alpha}}(H_{\beta}-n(\alpha , \beta )H_{\alpha}-n(\alpha , \beta )X_{\alpha})
$$

$$
=H_{\beta}-n(\alpha , \beta )H_{\alpha}-n(\alpha , \beta )X_{\alpha}-n(\alpha , \beta )X_{\alpha}-n(\alpha , \beta )(-2X_{\alpha})
$$

$$
=H_{\beta}-n(\alpha , \beta )H_{\alpha}
$$

$z\in \mathfrak{g}^\mu$の場合、

$$
[H_{\beta}, \theta_{\alpha}^{-1}z] =\theta_{\alpha}^{-1}[H_{\beta}-n(\alpha , \beta )H_{\alpha}, z]
$$

$$
=\theta_{\alpha}^{-1}(\langle \mu, \beta^{\vee}\rangle z-n(\alpha , \beta )\langle \mu, \alpha^{\vee}\rangle z)
$$

$$
=\langle \mu- \langle \alpha^{\vee}, \mu\rangle \alpha , \beta^{\vee}\rangle \theta^{-1}_{\alpha}z=\langle s_{\alpha}\mu, \beta^{\vee}\rangle \theta^{-1}_{\alpha}z
$$

だから$\theta_{\alpha}^{-1}z\in \mathfrak{g}^{s_{\alpha}\mu}$。これは$\theta^{-1}_{\alpha}\mathfrak{g}^\mu\subset \mathfrak{g}^{s_{\alpha}\mu}$を示しています。 $\theta_{\alpha}$ は自己同型であり、この包含はすべての $\mu\in Q$ に当てはまりますので、$\theta_{\alpha}^{-1}\mathfrak{g}^\mu=\mathfrak{g}^{s_{\alpha}\mu}$ がわかり、補題が証明されます。

#### 補題 10 {#lie-viii-s4-lem-10 .statement tag=0118}

$\mu\in Q$ とし、$\mu$ が根の倍数ではないと仮定します。 基底 B に対する $w\mu$ の座標の特定が $>0$ であり、それらの特定の座標が $<0$ であるような $w\in W(R)$ が存在します。

$V_{\mathbf{R}}$ をベクトル空間 $Q\otimes_{\mathbf{Z}}\mathbf{R}$ とし、R を根系とします。 仮定までに、すべての $\alpha \in R$ と $\langle f, \mu\rangle = 0$ に対して $\langle f, \alpha \rangle  \not= 0$ となる $f\in V^*_{\mathbf{R}}$ が存在します。 $f\in C$ のような $R^{\vee}$ の部屋 C が存在します。章著。 VI, §1, no. 5、TH。 2 (i) では、B に関連付けられたチャンバーに $wf$ 属するとなるような $w\in W(R)$ が存在し、他の語にはすべての $\alpha \in B$ に対して $\langle wf, \alpha \rangle >0$ が存在します。 $w\mu=\sum_{\alpha\in B}t_{\alpha}\alpha$と書きます。それから

$$
0 =\langle f, \mu\rangle =\langle wf, w\mu\rangle =\sum_{\alpha\in B}t_{\alpha}\langle wf, \alpha \rangle
$$

これは、特定の $t_{\alpha}$ が $>0$ であり、他のものは $<0$ であることを証明します。

#### 補題 11 {#lie-viii-s4-lem-11 .statement tag=0119}

$\mu\in Q$ にしましょう。 $\mu \notin R\cup \{0\}$の場合は、$\mathfrak{g}^\mu= 0$。 $\mu\in R$ の場合は、$\mathfrak{g}^\mu= 1$ を暗くします。

1) $\mu$ が R の元の倍数ではない場合、$w\mu \notin Q_+\cup Q_-$ (補題 10) となるような $w\in W$ が存在するため、$\mathfrak{a}^{w\mu}= 0,\mathfrak{g}^{w\mu}= 0$、したがって $\mathfrak{g}^\mu= 0$ (補題 9) となります。

2) $\alpha \in B$ を$m$ を整数とします。 $\mathfrak{a}_+$ は基本ファミリー $(x_{\alpha})_{\alpha\in B}$ を持つ無料のリー代数であるため、$m >1$ には dim$\mathfrak{a}^{\alpha}= 1$ と $\mathfrak{a}^{m\alpha}= 0$ があります (章 II, §2, no. 6、提案 4)。従って、$m >1$の場合は$\mathfrak{g}^{\alpha}\leq 1$と$\mathfrak{g}^{m\alpha}= 0$が暗くなります。 できないには $\mathfrak{g}^{\alpha}= 0$ があり、これは $x_{\alpha}\in \mathfrak{n}+\theta \mathfrak{n}$ を意味するため、$\mathfrak{n}+\theta \mathfrak{n}$ 含む $h_{\alpha}=-[x_{\alpha}, x_{-\alpha}]$ に対し、$\mathfrak{a}^0\cap (\mathfrak{n}+\theta \mathfrak{n}) = 0$ となります。従って、暗$\mathfrak{g}^{\alpha}= 1$。

3) $\mu\in R$ の場合、$w(\mu)\in B$ となるような $w\in W(R)$ が存在するので (章 VI, §1, no. 5、提案 15)、$\mathfrak{g}^\mu=$ を暗くし、$\mathfrak{g}^{w\mu}= 1$ を暗くします。さらに、$n$ が整数 $>1$ であれば、$\mathfrak{g}^{nw(\mu)}= 0$ となり、$\mathfrak{g}^{n\mu}= 0$ となります。

証明/定理 1.

dim$\mathfrak{g}^0=$ カード B なので、補題 11 から、$\mathfrak{g}$ は有限次元でカード B + カード R に等しいことがわかります。$\mathfrak{g}$ は半単純であることがわかります。 $\mathfrak{k}$ を $\mathfrak{g}$ の可換イデアルとします。 $\mathfrak{k}$はad($\mathfrak{h}$)$,\mathfrak{k}= (\mathfrak{k}\cap \mathfrak{h}) +\sum_{\mu\in R}(\mathfrak{k}\cap \mathfrak{g}^\mu)$で安定なので。

すべてにおいて、$\alpha \in B,\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}+kH_{\alpha}$ が $\mathfrak{s}\mathfrak{l}(2, k)$ と同型であることは明らかです。 補題 9 から見ると、すべての $\mu\in R,\mathfrak{g}^\mu$ は、$\mathfrak{s}\mathfrak{l}(2, k)$ と同型の $\mathfrak{g}$ の部分代数に含まれます。従って、$\mathfrak{k}\cap \mathfrak{g}^\mu= 0$、つまり $\mathfrak{k}\subset \mathfrak{h}$;従って

$$
[\mathfrak{k},\mathfrak{g}^\mu]\subset \mathfrak{k}\cap \mathfrak{g}^\mu= 0
$$

つまり、すべての $\mu\in R$ に対して $\mu_B(\mathfrak{k}) = 0$ です。従って、$\mathfrak{k}= 0$ となり、$\mathfrak{g}$ が半単純であることが証明されます。

$\mu\in R$ にしましょう。 $\langle \mu, \alpha^{\vee}\rangle  \not= 0$ となるような $\alpha \in B$ が存在し、(ad $H_{\alpha}$)$|\mathfrak{g}^\mu$ は非ゼロホモテティー になります。従って、$\mathfrak{h}$ は $\mathfrak{g}$ の独自のノーマライザーと等しく、従って $\mathfrak{g}$ のカルタン部分代数となります。すべての $u\in \mathfrak{h}$ に対して、広告 $u$ は対角化可能であるため、$(\mathfrak{g},\mathfrak{h})$ は分裂半単純リー代数になります。

すべての $\mu\in R$ について、$\mu_B$ が $(\mathfrak{g},\mathfrak{h})$ の根であり、$\mathfrak{g}^\mu$ が対応する固有空間であることは明らかです。 $(\mathfrak{g},\mathfrak{h})$の根の数は、カードRの$\mathfrak{g}-$が暗い$\mathfrak{h}=$です。したがって、写像$\mu \rightarrow \mu_B$は、Vから$\mathfrak{h}^*$写像Rから根系になります。 $(\mathfrak{g},\mathfrak{h})$。

### 4. 一意性定理

#### 命題 4 {#lie-viii-s4-prop-4 .statement tag=011A}

$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$を枠付きの半単純リー代数とします。 $(n(\alpha , \beta ))_{\alpha ,\beta\in B}$ と $(X_{\alpha})_{\alpha\in B\cup(-B)}$ を対応する Cartan 行列と生成するファミリーとします。

(i) no. 3 のファミリー$((X_{\alpha}, H_{\alpha}, X_{-\alpha}))_{\alpha\in B}$ と関係 (16) から (22) は、$\mathfrak{g}$ のプレゼンテーションを構成します。

(ii) no. 3 のファミリー $(X_{\alpha})_{\alpha\in B}$ と関係 (21) は、$(X_{\alpha})_{\alpha\in B}$ によって生成された $\mathfrak{g}$ の部分代数のプレゼンテーションを構成します。

R を $(\mathfrak{g},\mathfrak{h})$ の根系とします。 適用は番号のRとB構成に。 2 と 3 により、$\mathfrak{a}',\mathfrak{g}', X'_{\alpha}, H'_{\alpha}, . .$ で示すオブジェクトが得られます。 $\mathfrak{a},\mathfrak{g}, X_{\alpha}, H_{\alpha}, . .$ の代わりに..

リー代数 $\mathfrak{g}'$ からリー代数 $\mathfrak{g}$ までの準同型 $\varphi$ が存在し、すべての $\alpha \in B$ に対して $\varphi (X'_{\alpha}) =X_{\alpha},\varphi (H'_{\alpha}) =H_{\alpha},\varphi (X'_{-\alpha}) =X_{-\alpha}$ になります (提案 1)。 dim $\mathfrak{g}'$ = カード R + カード B = dim $\mathfrak{g},\varphi$ は全単射なので。これは(i)を証明します。

$(X'_{\alpha})_{\alpha\in B}$ によって生成された $\mathfrak{g}'=\mathfrak{a}'/(\mathfrak{n}'\oplus \theta '\mathfrak{n}') = (\mathfrak{a}'_+\oplus {\mathfrak{a}'}^0\oplus \mathfrak{a}'_-)/(\mathfrak{n}'\oplus \theta '\mathfrak{n}')$ の部分代数は、$\mathfrak{a}'_+/\mathfrak{n}'$ で識別できます。 $\mathfrak{n}'$ の提案 3 と定義を考慮すると、これは (ii) を証明します。

#### 系 {#lie-viii-s4-n4-cor-1 .statement tag=011B}

すべてのフレーム化された半単純リー代数は、$\mathbf{Q}$ から $k$ までのスカラーの拡大によるフレーム化された半単純 $\mathbf{Q}$-リー代数から得られます。

これは命題の直後に続きます。

#### 定理 2 {#lie-viii-s4-thm-2 .statement tag=011C}

$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$と$(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$を半単純リー代数にフレーム化し、Rと$R'$を$(\mathfrak{g},\mathfrak{h})$と$(\mathfrak{g}',\mathfrak{h}')$の根系とし、$(n(\alpha , \beta ))_{\alpha ,\beta\in B}$（それぞれ$(n'(\alpha , \beta ))_{\alpha ,\beta\in B'}$）をRのカルタン行列とするB (それぞれ $B'$) を基準とした (それぞれ $R'$)、B (それぞれ $B'$) を基準とした R (それぞれ $R'$) のディンキン グラフを $\Delta$ (それぞれ $\Delta '$) とします。

(i) $\varphi$ が $\varphi (R) = R'$ と $\varphi (B) = B'$ のような $\mathfrak{h}^*$ から $\mathfrak{h}^{'*}$ までの同型である場合、次のような $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ から $(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$ までの一意の同型 $\psi$ が存在します。 $\psi |\mathfrak{h}=^t\varphi^{-1}$。

(ii) $f$ が B から $B'$ までの全単射で、すべての $\alpha , \beta \in$ B に対して $n'(f(\alpha ), f(\beta )) =n(\alpha , \beta )$ である場合、$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ から $(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$ までの同型が存在します。

(iii) $\Delta$ から $\Delta '$ までに同型が存在する場合、$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ から $(\mathfrak{g}',\mathfrak{h}',B',(X'_{\alpha})_{\alpha\in B'})$ までに同型が存在します。

これは提案 4 (i) の直後に続きます (VI, §4, no. 2 章、提案 1 を部分 (iii) に利用)。

#### スコリウム {#lie-viii-s4-n4-sch-1 .statement tag=011D}

分割可能な半単純リー代数 $\mathfrak{g}$ には、決定する $\mathfrak{g}$ から同型までの Dynkin グラフが関連付けられます (Th. 2 (iii))。このグラフは空ではなく、$\mathfrak{g}$ が単純な場合にのみ接続されます (§3, no. 2、提案 6 の Cor. 1)。 Thさんよりno. 3 の 1、および第 1 章。 VI, §4, no. 2、木曜日。 3、分割可能な単純なリー代数は、型 $A_l(l\geq 1), B_l(l\geq 2), C_l(l\geq 3), D_l(l\geq 4)$、$E_6, E_7, E_8, F_4, G_2$ の代数です。このリストの 2 つの代数は同型ではありません。

#### 命題 5 {#lie-viii-s4-prop-5 .statement tag=011E}

$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ をフレーム化された半単純リー代数および $(X_{\alpha})_{\alpha\in B\cup(-B)}$ 対応する生成するファミリーとします。すべての $\alpha \in B\cup (-B)$ に対して $\theta (X_{\alpha}) =X_{-\alpha}$ となるような、$\mathfrak{g}$ のうちの固有の自己同型 $\theta$ が存在します。すべての $h\in \mathfrak{h}$ に対して $\theta^2=$ ID$_{\mathfrak{g}}$ と $\theta (h) =-h$ があります。

$(X_{\alpha})_{\alpha\in B\cup(-B)}$ 生成するリー代数 $\mathfrak{g}$ なので、一意性はクリアです。提案 4 を考慮すると、no. 3 前にで述べたことから、$\theta$ の存在が得られます。 1.

#### 系 {#lie-viii-s4-n4-cor-2 .statement tag=011F}

$(\mathfrak{g},\mathfrak{h})$ を分裂半単純リー代数とします。次に、$(\mathfrak{g},\mathfrak{h})$ は Chevalley 系 (§2, no. 4、Def. 3) を所有します。

R を $(\mathfrak{g},\mathfrak{h})$ の根系とします。すべての $\alpha \in R$ について、$X_{\alpha}$ を $\mathfrak{g}^{\alpha}$ の非ゼロ元とします。すべての $\alpha \in R ($§2, no. 4、補題に対して $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ となるように $X_{\alpha}$ が選択されたとします。 2) B を R の基底および $\mathfrak{g}$ の $\theta$ 自己同型とし、すべての $\alpha \in B\cup (-B)$ に対して $\theta (X_{\alpha}) =X_{-\alpha}$ とします。 $\theta |\mathfrak{h}=-$ID$_{\mathfrak{h}}$ があります。したがって、すべての $\alpha \in R$ に対して、$\theta X_{\alpha}=t_{\alpha}X_{-\alpha}$ となるような $t_{\alpha}\in k^*$ が存在します。私たちは持っています

$$
t_{\alpha}t_{-\alpha}H_{\alpha}= [t_{\alpha}X_{-\alpha}, t_{-\alpha}X_{\alpha}] = [\theta X_{\alpha}, \theta X_{-\alpha}] =\theta ([X_{\alpha}, X_{-\alpha}])
$$

$$
=\theta (-H_{\alpha}) =H_{\alpha}
$$

つまり、すべての $\alpha \in R$ に対して $t_{\alpha}t_{-\alpha}= 1$ です。 $N_{\alpha \beta}$を§2, no. 4と同様に導入します。 $\alpha , \beta , \alpha +\beta \in R$の場合、

$$
N_{-\alpha ,-\beta}t_{\alpha}t_{\beta}X_{-\alpha-\beta}=t_{\alpha}t_{\beta}[X_{-\alpha}, X_{-\beta}] = [\theta X_{\alpha}, \theta X_{\beta}] =\theta ([X_{\alpha}, X_{\beta}])
$$

$$
= N_{\alpha \beta}\theta X_{\alpha+\beta}= N_{\alpha \beta}t_{\alpha+\beta}X_{-\alpha-\beta}
$$

つまり、§2, no. 4、補題 4 を考慮すると、

$$
(q+ 1)^2t_{\alpha}t_{\beta}= N^2_{\alpha \beta}t_{\alpha+\beta}
$$

ここで、$q$ は整数です。したがって、$t_{\alpha}$ と $t_{\beta}$ が $k^*$ の平方である場合、$t_{\alpha+\beta}$ も同様です。すべての $\alpha \in B$ に対して $t_{\alpha}= 1$ であるため、第 1 章の提案 19 が適用されます。 VI, §1, no. 6は、$t_{\alpha}$がすべての$\alpha \in R$に対して平方であることを証明します。 選ぶ、すべての $\alpha \in R$ に対して、$u^2_{\alpha}=t_{\alpha}$ となる $u_{\alpha}\in k$。この選択は、すべての$\alpha \in R$に対して$u_{\alpha}u_{-\alpha}= 1$になるように作ることができます。 $X'_{\alpha}=u^{-1}_{\alpha}X_{\alpha}$を入れてください。それでは、$\alpha \in R$ 全員に、

$$
X'_{\alpha}\in \mathfrak{g}^{\alpha},[X'_{\alpha}, X'_{-\alpha}] = [X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

と $\theta (X'_{\alpha}) =\theta (u^{-1}_{\alpha}X_{\alpha}) =u^{-1}_{\alpha}t_{\alpha}X_{-\alpha}=u_{\alpha}X_{-\alpha}=u_{\alpha}u_{-\alpha}X'_{-\alpha}=X'_{-\alpha}$ なので、$(X'_{\alpha})_{\alpha\in R}$ は $(\mathfrak{g},\mathfrak{h})$ のシュバレー 系になります。

### 練習問題 {#lie-viii-s4-exercises}

この段落で考慮されるリー代数は必ずしも有限次元であるとは限りません。

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
