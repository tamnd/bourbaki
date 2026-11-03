---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 6
section_title: Modules over a split semi-simple Lie algebra
lang: ja
source: lie-vii-ix
book_pages: 115-123, 238
pdf_pages: 0123-0131, 0246-0246
extraction: native
subsections:
    - "no": 1
      title: WEIGHTS AND PRIMITIVE ELEMENTS
      page: 116
      pdf_page: 124
    - "no": 2
      title: SIMPLE MODULES WITH A HIGHEST WEIGHT
      page: 118
      pdf_page: 126
    - "no": 3
      title: EXISTENCE AND UNIQUENESS THEOREM
      page: 119
      pdf_page: 127
    - "no": 4
      title: COMMUTANT OF $\mathfrak{h}$ IN THE ENVELOPING ALGEBRA $\mathbf{O}\mathbf{F}\mathfrak{g}$
      page: 122
      pdf_page: 130
statements: 17
exercises: 5
content_sha256: 67e0387142cb518c86dacc0698863daa87f151922788ed8f4f8583124eb8956b
translated_from: content/en/lie/VIII/06_s6_modules_over_a_split_semi_simple_lie.md
translation_method: google
source_content_sha256: 487388bd8ad7aeeaec7bc35a084734841a8e2e5b22d8bc35a3035539d1b008d8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 3431eab56cf4609e5544599692fbd48cf2d121a3ed0bf315af382da2a57165e5
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 6。 加群分裂半単純リー代数

この段落では、$(\mathfrak{g},\mathfrak{h})$は分裂半単純リー代数、Rはその根系、Wはそのワイル群、BはRの基底、Bに対してポジティブ（それぞれネガティブ）根の$R_+$（それぞれ$R_-$）集合を表します。置く

$\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha},\mathfrak{b}_+=\mathfrak{h}+\mathfrak{n}_+$ と $\mathfrak{b}_-=\mathfrak{h}+\mathfrak{n}_-$。

$\mathfrak{n}_+= [\mathfrak{b}_+,\mathfrak{b}_+],\mathfrak{n}_-= [\mathfrak{b}_-,\mathfrak{b}_-]$ があります。

すべての $\alpha \in R$、選ぶ元 $X_{\alpha}\in \mathfrak{g}^{\alpha}$ について、

$$
[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

(§2, no. 4);以下の定義はどれもこの選択に依存しません。

### 1. 重みとプリミティブ元

V を $\mathfrak{g}$ モジュールとします。 For all $\lambda \in \mathfrak{h}^*$, denote by $V^{\lambda}$ the primary subspace, relative to $\lambda$, of V considered as an $\mathfrak{h}$-module (Chap. VII, §1, no. 1). $V^{\lambda}$ の元は、$\mathfrak{g}$ モジュール V の重み $\lambda$ の元と呼ばれます。 $V^{\lambda}$の和は直接的です（VII, §1, no. 1章、提案3）。 For all $\alpha \in \mathfrak{h}^*$ and $\lambda \in \mathfrak{h}^*,\mathfrak{g}^{\alpha}V^{\lambda}\subset V^{\alpha+\lambda}$ (Chap. VII, §1, no. 3, Prop. 10 (ii)). $V^{\lambda}$の次元は、Vでは$\lambda$の重複度と呼ばれます。それが$\geq 1$の場合、つまり、$V^{\lambda}\not= 0,\lambda$がVの重みと言われている場合。 V が有限次元の場合、$\mathfrak{h}$ の元によって定義される V の相似性は半単純であるため、$V^{\lambda}$ は $x\in V$ の集合となり、すべての $H\in \mathfrak{h}$ に対して $Hx=\lambda (H)x$ になります。

#### 補題 1 {#lie-viii-s6-lem-1 .statement tag=012M}

V を $\mathfrak{g}$ モジュール、$v\in V$ とします。次の条件は同等です。

(i) $\mathfrak{b}_+v\subset kv$;

(ii) $\mathfrak{h}v\subset kv$ および $\mathfrak{n}_+v= 0$;

(iii) すべての $\alpha \in B$ に対して $\mathfrak{h}v\subset kv$ と $\mathfrak{g}^{\alpha}v= 0$。

(i) $=\Rightarrow$ (ii): $\mathfrak{b}_+v\subset kv$ と仮定します。 $v\in V^{\lambda}$となるような$\lambda \in \mathfrak{h}^*$が存在します。 $\alpha \in R_+$ にしましょう。次に$\mathfrak{g}^{\alpha}.v\subset V^{\lambda}\cap V^{\lambda+\alpha}= 0$。したがって$\mathfrak{n}_+v= 0$です。

(ii) $=\Rightarrow$ (iii): これは明らかです。

(iii) $=\Rightarrow$ (i): これは、$(X_{\alpha})_{\alpha\in B}$ 生成する $\mathfrak{n}_+($§3, no. 3、提案 9 (iii)) という事実から導かれます。

#### 定義 1 {#lie-viii-s6-def-1 .statement tag=012N}

V を $\mathfrak{g}$ モジュールおよび $v\in V$ とします。そして、$v\not= 0$と$v$が補題1の条件を満たす場合、$v$はVの原始元であると言われます。

プリミティブ元属するから $V^{\lambda}$ の 1 つまで。すべての $\lambda \in \mathfrak{h}^*, V_{\pi}^{\lambda}$ は、$\mathfrak{b}_+v\subset kv$ となる $v\in V^{\lambda}$ の集合を表します。したがって、重み $\lambda$ のプリミティブ元は、$V_{\pi}^{\lambda}$ の非ゼロ元です。

#### 命題 1 {#lie-viii-s6-prop-1 .statement tag=012O}

V を $\mathfrak{g}$ モジュール、$v$ を V のプリミティブ元、および $v$ の $\omega$ 重みとします。 V が $v$ によって $\mathfrak{g}$ モジュールとして生成されると仮定します。

(i) $U(\mathfrak{n}_-)$ が $\mathfrak{n}_-$ を包む代数を表す場合、$V = U(\mathfrak{n}_-).v$ が得られます。

(ii) すべての $\lambda \in \mathfrak{h}^*,V^{\lambda}$ は、すべての $H\in \mathfrak{h}$ について $Hx=\lambda (H)x$ となるように、$x\in V$ の集合です。 $V =\bigoplus_{\lambda\in\mathfrak{h}^*}V^{\lambda}$ があり、それぞれの $V^{\lambda}$ は有限次元です。 空間

$V^{\omega}$ は次元 1 であり、V のすべての重みは形 $\omega -\sum_{\alpha\in B}n_{\alpha}.\alpha$ であり、$n_{\alpha}$ は整数 $\geq 0$ です。

(iii) V は分解不可能な $\mathfrak{g}$ モジュールであり、その交換子環簡約するはスカラーに変換されます。

(iv) $U(\mathfrak{g})$ を $\mathfrak{g}$ の代数と $U(\mathfrak{g})$ の $\mathscr{Z}$ 中心を囲むものとします。 $\mathscr{Z}$ から $k$ までの一意な準同型 $\chi$ が存在し、すべての $z\in \mathscr{Z}$ に対して、$z_V$ はホモテティー となり、比率は $\chi (z)$ になります。

$U(\mathfrak{b}_+)$ を $\mathfrak{b}_+$ を囲む代数とします。 We have $U(\mathfrak{g}) = U(\mathfrak{n}_-).U(\mathfrak{b}_+)$ (Chap. I, §2, no. 7, Cor. 6 of Th. 1). したがって、

$$
V = U(\mathfrak{g}).v= U(\mathfrak{n}_-).U(\mathfrak{b}_+).v= U(\mathfrak{n}_-).v
$$

$R_+$ の異なる元を $\alpha_1, . . . , \alpha_n$ で示します。それから

$$
(X_{-\alpha_1}^{p_1}X_{-\alpha_2}^{p_2}. . . X_{-\alpha_n}^{p_n})_{(p_1,...,p_n)\in\mathbf{N}^n}
$$

は $U(\mathfrak{n}_-)$ の基底なので、

V = $\sum kX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v$。 (1)

$(p_1,...,p_n)\in \mathbf{N}^n$

$\lambda \in \mathfrak{h}^*$には、

$$
T_{\lambda}=\sum kX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v
$$

$(p_1,...,p_n)\in \mathbf{N}^n, \omega -p_1\alpha_1-\cdot \cdot \cdot -p_n\alpha_n=\lambda$

章著。 VII, §1, no. 1、提案 2 (ii)、$h\in \mathfrak{h},h_V|T_{\lambda}$ がホモテティー で比率 $\lambda (h)$ の場合。ということで$T_{\lambda}\subset V^{\lambda}$。一方、(1) は次のことを意味します。

V = $\sum T_{\lambda}$。

$\lambda \in \omega -\mathbf{N}\alpha_1-\cdot \cdot \cdot -\mathbf{N}\alpha_n$

$V^{\lambda}$の和は直接的です（VII, §1, no. 1章、提案3）。これらの観察から、$V^{\lambda}= T_{\lambda}$、Vは$V^{\lambda}$の直和、$V^{\lambda}$は$x\in V$の集合で、すべての$h\in \mathfrak{h}$に対して$hx=\lambda (h)x$となることがわかります。一方、dim $V^{\lambda}$ は、$p_1\alpha_1+\cdots +p_n\alpha_n=\omega -\lambda$ となるように、$(p_1, . . . , p_n)\in \mathbf{N}^n$ の集合の基数がせいぜいです。これは、$\omega -\lambda  \notin \sum_{\alpha\in B}\mathbf{N}\alpha$なら$V^{\lambda}= 0$、

暗い$V^{\omega}= 1$と$V^{\lambda}$はすべて有限次元です。

$c$ を V の交換子環の元とします。 $h\in \mathfrak{h}$ 全員にとって、

$$
hc(v) =ch(v) =\omega (h)c(v)
$$

だから$c(v)\in V^{\omega}$;したがって、$c(v) =tv$ となるような $t\in k$ が存在します。さて、$(p_1, . . . , p_n)\in \mathbf{N}^n$の皆さん、

$$
cX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v=X_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}cv=tX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v
$$

$c=t.1$になります。したがって、スカラーでは、V 簡約するの交換子環になります。これは、(iv) と V が分解不可能であるという事実を意味します。

#### 定義 2 {#lie-viii-s6-def-2 .statement tag=012P}

提案 1 (iv) の準同型 $\chi$ は、$\mathfrak{g}$ モジュール V の中心指標と呼ばれます。

#### 命題 2 {#lie-viii-s6-prop-2 .statement tag=012Q}

V を、重み $\omega$ のプリミティブ元 $e$ および X 半単純 $\mathfrak{g}$ モジュールによって生成された $\mathfrak{g}$ モジュールとします。 $\Phi$ を、$\mathfrak{g}$ モジュール V から $\mathfrak{g}$ モジュール X までの準同型の集合とします。すると、$\varphi  \rightarrow \varphi (e)$はベクトル空間$\Phi$からベクトル空間$X^{\omega}_{\pi}$の同型になります。

すべての $\varphi \in \Phi$ に対して $\varphi (e)\in X^{\omega}_{\pi}$ であることは明らかです。 $\varphi \in \Phi$ と $\varphi (e) = 0$ の場合、$e$ 生成するの $\mathfrak{g}$ モジュール V なので、$\varphi = 0$ になります。 $f$ が $X^{\omega}_{\pi}$ の非ゼロ元である場合、$\varphi (e) =f$ となるような $\varphi \in \Phi$ が存在することを示します。 $X'$を、$f$によって生成されたXの部分加群とします。提案によると、$1, X'$ は分解不可能であり、X は半単純なので単純です。 元 $(e, f)$ は、$\mathfrak{g}$ モジュール $V\times X$ のプリミティブです。 N を $(e, f)$ によって生成された $V\times X$ の部分加群とします。次に、$N\cap X\subset$ pr$_2(N) = X'$、つまり $N\cap X = 0$ または $X'$; $N\cap X = X', N$ 含むが重み $\omega$ の原始関数である線形独立元 $(e, f)$ と $(0, f)$ の場合。これは不合理なので (提案 1)、$N\cap X = 0$。したがって、pr$_1|N$ は N から V までの単射詞写像 $h$ です。この写像は像含む $e$ なので全射法です。したがって、$\varphi =$ pr$_2\circ h^{-1}$ は、$\mathfrak{g}$ モジュール V から $\mathfrak{g}$ モジュール X までの準同型となり、$\varphi (e) =f$ となります。

### 2. 単純加群と最高重量

$\mathfrak{h}^*_{\mathbf{Q}}$ で B 定義する位数関係を固定したことを思い出してください (第 VI, §1, no. 6 章)。 $\geq 0$ である $\mathfrak{h}^*_{\mathbf{Q}}$ の元は、有理数係数 $\geq 0$ を持つ B の元の線形結合です。

より一般的には、元 $\lambda , \mu\in \mathfrak{h}^*:$ の間で次の位数関係を考慮します。

$\lambda -\mu$ は、有理数係数 $\geq 0$ を持つ B の元の線形結合です。

#### 補題 2 {#lie-viii-s6-lem-2 .statement tag=012R}

V を単純な $\mathfrak{g}$ モジュール、V の $\omega$ 重みとします。次の条件は同等です。

(i) V のすべての重みは形 $\omega -\mu$ であり、$\mu$ は根基重み $\geq 0$ です。

(ii) $\omega$ は V の最高重量です。

(iii) すべての $\alpha \in B,\omega +\alpha$ は V の重みではありません。

(iv) 重み $\omega$ のプリミティブ元が存在します。

(i) $=\Rightarrow$ (ii) $=\Rightarrow$ (iii): これは明らかです。

(iii) $=\Rightarrow$ (iv): 条件 (iii) が満たされると仮定します。 $h\in \mathfrak{h}$の皆様へ、

カー($h_V-\omega (h)$)

はゼロではなく、$V^{\omega}$ に含まれ、$\mathfrak{h}_V$ で安定しています。薄暗い$\mathfrak{h}$の帰納法により、$\mathfrak{h}v\subset kv$のようなゼロ以外の$v$が$V^{\omega}$に存在することがわかります。 条件 (iii) は $\mathfrak{n}_+v= 0$ を意味するため、$v$ は原始的です。

(iv) $=\Rightarrow$ (i): $v$ を重み $\omega$ のプリミティブ元とします。 Vは単純なので、Vは$v$により$\mathfrak{g}$モジュールとして生成されます。 主張 (i) は提案 1 から導き出されます。

Q.E.D.

したがって、単純な $\mathfrak{g}$ モジュールの場合、プリミティブ元の存在は、最高重量の存在、または最大の重みの存在と同等です。 $\mathfrak{s}\mathfrak{l}(2,\mathbf{C}) ($§1 のカルタン部分代数 $\mathfrak{h}$ に対して重みを持たない単純な $\mathfrak{s}\mathfrak{l}(2,\mathbf{C}$) モジュール V が存在します。 $14f))$。これらの加群は、$\mathbf{C}($§1, no. 3 以上、無限の次元です。 1)。

#### 命題 3 {#lie-viii-s6-prop-3 .statement tag=012S}

V を、最高重量 $\omega$ を含む単純な $\mathfrak{g}$ モジュールとしましょう。

(i) V のプリミティブ元は、$V^{\omega}$ の非ゼロ元です。

(ii) V は、$\mathfrak{h}$ モジュールとしては半単純です。

(iii) $V =\bigoplus_{\lambda\in\mathfrak{h}^*}V^{\lambda}$ があります。すべての$\lambda \in \mathfrak{h}^*,V^{\lambda}$ は有限次元です。私たち

薄暗い$V^{\omega}= 1$があります。

(iv) $\mathfrak{g}$ モジュール V は非常に単純です。

主張 (i)、(ii)、(iii) は提案 1 および補題 2 に従う。 主張 (iv) は提案 1 (iii) および代数、第VIII, §7, no. 3。

#### 系 {#lie-viii-s6-n2-cor-1 .statement tag=012T}

V が有限次元の場合、標準準同型 $U(\mathfrak{g})\rightarrow$ End(V) は全射です。

これは、cf. 代数、第 4 章の (iv) に続きます。 VIII, §3, no. 3。

#### 命題 4 {#lie-viii-s6-prop-4 .statement tag=012U}

V を、最高重量 $\omega$、X 半単純 $\mathfrak{g}$ モジュール、および型の同型成分である $X'$ を含む単純な $\mathfrak{g}$ モジュールとします。 XのV。すると、$X'$ は、$X^{\omega}_{\pi}$ によって生成された X の部分加群になります。その長さは$X^{\omega}_{\pi}$の次元に等しい。

$X''$ を、$X^{\omega}_{\pi}$ によって生成された X の部分加群とします。 V と同型の X のすべての部分加群が $X''$ に含まれていることは明らかです。したがって$X'\subset X''$です。一方、$\mathfrak{g}$モジュールVから$\mathfrak{g}$モジュールXまでの準同型の集合を$\Phi$とします。 $X'$の長さが暗い$_k\Phi ($代数、Chap. VIII, §4, no. 4)、つまり暗い$_kX^{\omega}_{\pi}$ (提案 2)。

### 3. 存在と一意性定理

$\lambda \in \mathfrak{h}^*$ にしましょう。 Since $\mathfrak{b}_+=\mathfrak{h}\oplus \mathfrak{n}_+$ and since $\mathfrak{n}_+= [\mathfrak{b}_+,\mathfrak{b}_+]$, 写像 $h+n \rightarrow \lambda (h)$ (where $h\in \mathfrak{h},n\in \mathfrak{n}_+$) from $\mathfrak{b}_+$ to $k$ is a 1-dimensional 表現 of $\mathfrak{b}_+$.この表現で定義される$\mathfrak{b}_+$モジュール構造を備えた$k$ベクトル空間$k$を$L_{\lambda}$で表す。 Let $U(\mathfrak{g}), U(\mathfrak{b}_+)$ be the enveloping 代数 of $\mathfrak{g},\mathfrak{b}_+$, so that $U(\mathfrak{b}_+)$ is 部分代数 of $U(\mathfrak{g})$; $U(\mathfrak{g})$ は自由な権利 $U(\mathfrak{b}_+$) モジュールであることを思い出してください (Th. 1 の Cor. 5、I, §2, no. 7 章)。置く

$$
Z(\lambda ) = U(\mathfrak{g})\otimes_{U(\mathfrak{b}_+)}L_{\lambda} \tag{2}
$$

次に、$Z(\lambda )$ は左の $\mathfrak{g}$ モジュールです。 $Z(\lambda )$ の $e$ 元 $1\otimes 1$ で表します。

#### 命題 5 {#lie-viii-s6-prop-5 .statement tag=012V}

(i) 元 $e$ of $Z(\lambda )$ is primitive of 重み $\lambda$ and 生成する the $\mathfrak{g}$-module $Z(\lambda )$.

(ii) $Z^+(\lambda ) =\sum_{\lambda\not=\mu}Z(\lambda )^\mu$ とします。 Every 部分加群 of $Z(\lambda )$ distinct from $Z(\lambda )$

$Z^+(\lambda )$ に含まれています。

(iii) There exists 最大の部分加群 $F_{\lambda}$ of $Z(\lambda )$ distinct from $Z(\lambda )$. 商加群 $Z(\lambda )/F_{\lambda}$ is simple and has 最高重量 $\lambda$.

It is clear that $e$ 生成する the $\mathfrak{g}$-module $Z(\lambda )$. $x\in \mathfrak{b}_+$の場合、

$$
x.e= (x.1)\otimes 1 = (1.x)\otimes 1 = 1\otimes x.1 =\lambda (x)(1\otimes 1) =\lambda (x)e
$$

したがって (i)。

The $\mathfrak{h}$-module $Z(\lambda )$ is 半単純 (Prop. 1). If G is a $\mathfrak{g}$-submodule of $Z(\lambda )$, then $G =\sum_{\mu\in\mathfrak{h}^*}(G\cap Z(\lambda )^\mu)$. 仮定 $G\cap Z(\lambda )^{\lambda}\not= 0$ が意味するもの

その $G = Z(\lambda )$ は、$Z(\lambda )^{\lambda}= 1$ と $e$ 生成するが $\mathfrak{g}$ モジュール $Z(\lambda )$ であるためです。 $G\not= Z(\lambda )$の場合は、$G =\sum_{\mu\not=\lambda}G\cap Z(\lambda )^\mu\subset Z^+(\lambda )$。

$F_{\lambda}$ を、$Z(\lambda )$ とは異なる $Z(\lambda )$ の $\mathfrak{g}$ サブモジュールの和とします。 By (ii), $F_{\lambda}\subset Z^+(\lambda )$.したがって、$F_{\lambda}$ は、$Z(\lambda )$ の最大の部分加群であり、$Z(\lambda )$ とは異なります。 $Z(\lambda )/F_{\lambda}$ が単純であり、$Z(\lambda )/F_{\lambda}$ の $e$ の標準像が重み $\lambda$ の原始であることは明らかです。

この章の残りでは、提案5の$\mathfrak{g}$モジュール$Z(\lambda )/F_{\lambda}$は$E(\lambda )$で表されます。

#### 定理 1 {#lie-viii-s6-thm-1 .statement tag=012W}

$\lambda \in \mathfrak{h}^*$ にしましょう。 $\mathfrak{g}$ モジュール $E(\lambda )$ はシンプルで、最高重量 $\lambda$ があります。 最高重量 $\lambda$ のすべての単純な $\mathfrak{g}$ 加群は $E(\lambda )$ と同型です。

The first 主張 follows from Prop. 5 (iii). The second follows from Prop. 4.

#### 命題 6 {#lie-viii-s6-prop-6 .statement tag=012X}

V を $\mathfrak{g}$ モジュール、$\lambda$ 元の $\mathfrak{h}^*$、$v$ を重み $\lambda$ の V のプリミティブ元とします。

(i) $\psi (e) =v$ となる $\mathfrak{g}$ モジュール $\psi : Z(\lambda )\rightarrow V$ の一意な準同型が存在します。

(ii) Assume that $v$ 生成する V. Then $\psi$ is surjective.さらに、$U(\mathfrak{n}_-),u_V$ の 0 以外のすべての元 $u$ が単射である場合に限り、$\psi$ は全単射です。

(iii) $U(\mathfrak{n}_-)$ から $Z(\lambda )$ までの写像 $u \rightarrow u\otimes 1$ は全単射です。

K を $L_{\lambda}$ の $U(\mathfrak{b}_+)$ の表現の核とします。 it is of codimension 1 in $U(\mathfrak{b}_+)$. $J = U(\mathfrak{g})K$ を K によって生成された $U(\mathfrak{g})$ の左イデアルとします。この場合、$L_{\lambda}$ は左の $U(\mathfrak{b}_+$) モジュールとして $U(\mathfrak{b}_+)/K$ で識別でき、$Z(\lambda )$ は左の $U(\mathfrak{g}$) モジュールとして $U(\mathfrak{g})/J$ で識別できます。 We have $K.v= 0$, so $J.v= 0$, which proves (i).

Now assume that $v$ 生成する V. It is clear that $\psi$ is surjective.

ポアンカレ・バーコフ・ウィット定理 (第 1 章 I, §2, no. 7、コリント 6) によれば、$k$ 上の$U(\mathfrak{n}_-)$ の基底は、右側の $U(\mathfrak{b}_+)$ 加群として $U(\mathfrak{g})$ の基底でもあります。従って、$U(\mathfrak{n}_-)$ から $U(\mathfrak{g})\otimes_{U(\mathfrak{b}_+)}L_{\lambda}$ までの写像 $\varphi :u \rightarrow u\otimes 1$ は全単射です。 $u\in U(\mathfrak{n}_-)$ にしましょう。すると、$U(\mathfrak{n}_-)$の$u$により、$\varphi^{-1}\circ u_{Z(\lambda)}\circ \varphi$は乗法になります。章の観点から。 I, §2, no. 7、コル。 Thの7。 $u\not= 0$ の場合、$1,u_{Z(\lambda)}$ は単射法です。従って、$\psi$ が全単射である場合、$U(\mathfrak{n}_-)$ の非ゼロ $u$ に対して $u_V$ は単射となります。

$\psi$ は単射的ではないと仮定します。 $u\not= 0$と$\psi (\varphi (u)) = 0$のような$u\in U(\mathfrak{n}_-)$が存在します。それから

$$
u_V.v=u_V.\psi (1\otimes 1) =\psi (u\otimes 1) =\psi (\varphi (u)) = 0
$$

#### 系 1 {#lie-viii-s6-prop-6-cor-1 .statement tag=012Y}

$\lambda \in \mathfrak{h}^*$ と $\alpha \in B$ が $\lambda (H_{\alpha}) + 1\in \mathbf{N}$ となるようにします。この場合、$Z(-\alpha +s_{\alpha}\lambda )$ は $Z(\lambda )$ の $\mathfrak{g}$ サブモジュールと同型です。

$m=\lambda (H_{\alpha})$を入れてください。 $x= X^{m+1}_{-\alpha}.e\in Z(\lambda )$ を、V を $x$ によって生成された $Z(\lambda )$ の部分加群とします。次に、$x\not= 0$ (提案 6)。一方、$x\in Z(\lambda )^{\lambda-(m+1)\alpha}$。 $\beta \in B$と$\beta \not=\alpha , [\mathfrak{g}^{-\alpha},\mathfrak{g}^{\beta}] = 0$と$\mathfrak{g}^{\beta}.e= 0$の場合、$\mathfrak{g}^{\beta}.x= 0$になります。最後に、$[X_{\alpha},X_{-\alpha}] =-H_{\alpha}$ 以降、

$$
[X_{\alpha}, X_{-\alpha}^{m+1}] = (m+ 1)X_{-\alpha}^m(-H_{\alpha}+m)
$$

(§1, no. 1, 補題 1 (ii))

$$
X_{\alpha}.x=X_{\alpha}X_{-\alpha}^{m+1}.e= [X_{\alpha}, X_{-\alpha}^{m+1}].e= (m+ 1)X_{-\alpha}^m(me-\lambda (H_{\alpha})e) = 0
$$

従って、$x$ は重み $\lambda -(m+ 1)\alpha$ のプリミティブです。提案 6 を考慮すると、$\mathfrak{g}$ 加群 V は $Z(-\alpha +\lambda -m\alpha ) = Z(-\alpha +s_{\alpha}\lambda )$ と同型です。

#### 系 2 {#lie-viii-s6-prop-6-cor-2 .statement tag=012Z}

$\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$と$\lambda , \mu\in \mathfrak{h}^*$としましょう。 R では $\lambda +\rho$ が優勢な重みであり、$\mu+\rho =w(\lambda +\rho )$ とともに $w\in W$ が存在すると仮定します。この場合、$Z(\mu)$ は $Z(\lambda )$ の部分加群と同型です。

$w= 1$の場合、主張はクリアです。 $w$が長さ$< q$のときは必ず成立するとします。 $w$ が長さ $q$ である場合、$l(w') =q-1$ を伴う $w=s_{\alpha}w^{'-1}$ となるような $\alpha \in B$ が存在します。 $w'(\alpha )\in R_+$ (提案 17 の章 VI, §1, no. 6、コリント 2) があるため、$w^{'-1}(\lambda +\rho )(H_{\alpha}) = (\lambda +\rho )(H_{w'\alpha})$ は整数 $\geq 0$ です。置く

$$
\mu'=w^{'-1}(\lambda +\rho )-\rho
$$

帰納法の仮定により、$Z(\mu')$ は $Z(\lambda )$ の部分加群と同型になります。一方、Chap。 VI, §1, no. 10、提案 29 (ii)、

$$
-\alpha +s_{\alpha}\mu'=-\alpha +s_{\alpha}w^{'-1}(\lambda +\rho )-s_{\alpha}\rho =w(\lambda +\rho )-\rho =\mu
$$

さらに、$\rho (H_{\alpha}) = 1$（第VI, §1、案29（ⅲ））なので、$\mu'(H_{\alpha})+1\in \mathbf{N}$です。コル。 1 は、$Z(\mu)$ が $Z(\mu')$ の部分加群と同型であること、したがって $Z(\lambda )$ の部分加群とも同型であることを意味します。

### 4. 代数 $\mathbf{O}\mathbf{F}\mathfrak{g}$ の$\mathfrak{h}$ の交換子環

U を、$\mathfrak{g}, V\subset U$ を包含する代数と、$\mathfrak{h}$ を包含する代数とします。 代数 V は、$\mathfrak{h}$ の対称的な代数 $\mathbf{S}(\mathfrak{h})$ と識別でき、また、$\mathfrak{h}^*$ の多項式関数の代数とも識別できます。 $\alpha_1, . . . , \alpha_n$ でペアごとに異なる正の根を示します。 $(H_1, . . . , H_l)$を$\mathfrak{h}$の基底とします。ポアンカレ・バーコフ・ヴィット著定理、元

$$
u((q_i),(m_i),(p_i)) =X_{-\alpha_1}^{q_1}. . . X_{-\alpha_n}^{q_n}H_1^{m_1}. . . H_l^{m_l}X_{\alpha_1}^{p_1}. . . X_{\alpha_n}^{p_n}
$$

$(q_i, m_i, p_i$ 整数 $\geq 0)$ 形基底ベクトル空間 U. すべての $h\in \mathfrak{h}$ について、私たちは

$$
[h, u((q_i),(m_i),(p_i))] = ((p_1-q_1)\alpha_1+\cdots +(p_n-q_n)\alpha_n)(h)u((q_i),(m_i),(p_i)).(3)
$$

ベクトル空間 U は、随伴表現の下の $\mathfrak{g}$ モジュール (したがって、$\mathfrak{h}$ モジュールでもあります) です。 $\lambda \in \mathfrak{h}^*$、部分空間、$U^{\lambda}$、$U_{\lambda}$ が定義されている場合 (VII, §1, no. 3 章)。 公式 (3) は、$U^{\lambda}= U_{\lambda}$ と $U =\bigoplus_{\lambda\in Q}U^{\lambda}$ を示します。

(Q は R の根基重みの群です)。特に、$U^0$ は、U では $\mathfrak{h}$ の交換子環、または V です。

#### 補題 3 {#lie-viii-s6-lem-3 .statement tag=0130}

$L = (\mathfrak{n}_-U)\cap U^0$を入れてください。

(i) $L = (U\mathfrak{n}_+)\cap U^0$ があり、L は$U^0$ の両面理想です。

(ii) $U^0= V\oplus L$ があります。

$\mathfrak{n}_-U$ (それぞれ $U\mathfrak{n}_+$) は、元 $u((q_i),(m_i),(p_i))$ の線形結合の集合であり、$\sum q_i>0$ (それぞれ $\sum p_i>0$) であることは明らかです。一方、

$$
u((q_i),(m_i),(p_i))\in U^0\Leftarrow \Rightarrow p_1\alpha_1+\cdots +p_n\alpha_n=q_1\alpha_1+\cdots +q_n\alpha_n
$$

これは $(\mathfrak{n}_-U)\cap U^0= (U\mathfrak{n}_+)\cap U^0$ を意味します。最後に、$(\mathfrak{n}_-U)\cap U^0$ (それぞれ $(U\mathfrak{n}_+)\cap U^0$) は、$U^0$ の右 (それぞれ左) イデアルであるため、(i) になります。さらに、$U^0$ 属するから V (それぞれ L) にある元 $u((q_i),(m_i),(p_i))$ は、$p_1=\cdots =p_n=q_1=\cdots =q_n= 0$ (それぞれ $p_1+\cdots +p_n+q_1+\cdots +q_n>0$) である場合にのみ、したがって (ii) になります。 Q.E.D.

補題 3 を考慮すると、$U^0$ の射影が V に核 L で代数の準同型になります。それは、$U^0$ から V (B に対して) までの Harish-Chandra 準同型と呼ばれます。 V は、$\mathfrak{h}^*$ の多項式関数の代数と識別できることを思い出してください。

#### 命題 7 {#lie-viii-s6-prop-7 .statement tag=0131}

$\lambda \in \mathfrak{h}^*$, E を、重み $\lambda ,\chi$ のプリミティブ元、E の中央指標、および$\varphi$ $U^0$ からV までの Harish-Chandra 準同型によって生成された$\mathfrak{g}$ モジュールとします。次に、U の中心のすべての $z$ に対して $\chi (z) = (\varphi (z))(\lambda )$ です。

$v$ を、重み $\lambda$ の E の原始元と、U の中心の $z$ 元とします。 $z=\varphi (z) +u_1n_1+\cdots +u_pn_p$ となるような $u_1, . . . , u_p\in U$ と $n_1, . . . , n_p\in \mathfrak{n}_+$ が存在します。それから

$$
\chi (z)v=zv=\varphi (z)v+u_1n_1v+\cdots +u_pn_pv=\varphi (z)v= (\varphi (z))(\lambda )v
$$

#### 系 {#lie-viii-s6-n4-cor-1 .statement tag=0132}

$\langle  \cdot ,\cdot  \rangle$ を、$\mathfrak{g}$、C $\langle  \cdot ,\cdot  \rangle$ に関連付けられたカシミール元上の非縮退不変対称対称双線形形式とします。 $\langle  \cdot ,\cdot  \rangle$ から $\mathfrak{h}($§2, no. 3 の制限の $\mathfrak{h}^*$ の逆数形も $\langle  \cdot ,\cdot  \rangle$ で表します、提案 5)。次に$\chi (C) =\langle \lambda , \lambda + 2\rho \rangle$、ここで$\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$。

§2, no. 3 の記法、提案 6 を思い出します。

1 1

C = $\sum X_{\alpha}X_{-\alpha}+\sum X_{-\alpha}X_{\alpha}$

$$
_{\alpha\in R_-}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}\alpha^{\in}_{R_+}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}
$$

1 $'$

$$
+\sum[X_{\alpha}, X_{-\alpha}] +\sum H_iH
$$

$$
_{\alpha\in R_+}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}i_{\in I}^i
$$

それで

$$
\varphi (C) =\sum_{\alpha\in R_+}\frac{1}{\langle X_{\alpha}, X_{-\alpha}\rangle}[X_{\alpha}, X_{-\alpha}] +\sum_{i\in I}H_iH'_i
$$

提案 7 により、

1 $'$

$$
\chi (C) =\sum\lambda ([X_{\alpha}, X_{-\alpha}]) +\sum\lambda (H_i)\lambda (H)
$$

$$
_{\alpha\in R_+}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}i_{\in I}i
$$

$h_{\lambda}$ を、すべての $h\in \mathfrak{h}$ に対して $\langle h_{\lambda}, h\rangle =\lambda (h)$ となるように、$\mathfrak{h}$ の元とします。 §2, no. 2、提案 1 により、

$($ 1 $)\langle$ 1 $\rangle$

$\lambda [X_{\alpha}, X_{-\alpha}]$ = $h_{\lambda},[X_{\alpha}, X_{-\alpha}]=\alpha (h_{\lambda}) =\langle \lambda , \alpha \rangle$。

$$
\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}
$$

したがって、

$$
\chi (C) =((\sum_{\alpha\in R_+}\langle \lambda , \alpha \rangle )+\langle \lambda , \lambda \rangle =\langle \lambda , \lambda + 2\rho \rangle
$$

### 練習問題 {#lie-viii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
