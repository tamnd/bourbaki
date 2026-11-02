---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 19
section_title: Quaternion Algebras
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.361-A VIII.371
pdf_pages: 0378-0388
extraction: native+ocr
subsections:
    - "no": 1
      title: General Properties of Quaternion Algebras
      page: 361
      pdf_page: 378
    - "no": 2
      title: The Center of a Quaternion Algebra
      page: 363
      pdf_page: 380
    - "no": 3
      title: Simplicity of Quaternion Algebras
      page: 363
      pdf_page: 380
    - "no": 4
      title: Criteria for a Quaternion Algebra to Be a Field
      page: 366
      pdf_page: 383
    - "no": 5
      title: Algebras over Maximal Ordered Fields
      page: 367
      pdf_page: 384
statements: 16
exercises: 8
content_sha256: fda3a990cf2015f598e1a27d6a4f2e21b1e5c829b81ad9625c34b8d37f6351a3
translated_from: content/en/alg/VIII/19_s19_quaternion_algebras.md
translation_method: google
source_content_sha256: 108f7dda8f7849f663b2ef3f83020f45b2cebb199a339be51e597d680bf6aafa
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 2922eb70fd5372ce4c4770a18f0e838f6452054893a7220ac6344bb9434bb82f
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 19。 四元数代数

この切断では、Kは可換体です。

### 1. 四元数代数の一般特性

$\alpha , \beta , \gamma$ を K の元とし、F を型 $(\alpha , \beta , \gamma )$ の四元数代数とします。 (III, §2, No. 5, p. 445)[^1] F は K 満たす関係に対して基底 $(1, i, j, k)$ を持つ結合単位 K-代数であることを思い出してください。

$$
i^2=\alpha +\beta i ,j^2=\gamma  ,ij=k ,ji=\beta j-k \tag{1}
$$

これは、活用が満たされる Cayley 代数 (III, §2, No. 4, p. 441, 定義 1) です。

$$
\overline{i}=\beta -i ,\overline{j}=-j ,\overline{k}=-k \tag{2}
$$

Cayley トレースと F のノルムは、$T_F(q) =q+\overline{q}$ と $N_F(q) =qq$ によって定義される F から K までの写像 $T_F$ と $N_F$ であることを思い出してください。

F の線形部分空間 E と基底 $(1, i)$ は、F の可換 Cayley 部分代数です。それは型 $(\alpha , \beta )$ の二次代数であり、F は $\gamma$ (III, §2, No. 5, p. 444) によって定義される E の Cayley 拡大と識別できます。 $z\in E$ ごとに、$zj=jz$ があります。 F のすべての元 $q$ は、$x, y\in E$ を使用した $x+jy$ として一意に書くことができます。

$$
\overline{q}=\overline{x}-jy ,T_F(q) =x+\overline{x},N_F(q) =xx-\gamma yy \tag{3}
$$

#### 命題 1 {#alg-viii-s19-prop-1 .statement tag=00LQ}

F の特性多項式元 $q$ は $(X^2-T_F(q)X + N_F(q))^2$ に等しい。

以上により、代数 F は、基底 $(1, j)$ を持つ自由な右 E モジュールになります。従って、F[X] は、基底 $(1, j)$ を持つ自由権 E[X] モジュールです。 $P\in F[X]$ に対して $u(P) =$ $(X-q)P$ によって定義される右側の E[X]-モジュール F[X] の $u$ 自己準同型で表します。 $q$ の特性多項式は、K[X] モジュール F[X] の自己準同型として見られる $u$ の行列式です。 III, §9, No. 4, p. 546 の命題 6 により、N(det $u$) に等しくなります。ここで、N は E[X] から K[X] までのノルムを表します。 $q$を$x+jy$と$x, y\in E$で書きましょう。 基底 $(1, j)$ に対する $u$ の行列は $\begin{pmatrix} X-x & -\gamma y \\ -y & X-\overline{x} \end{pmatrix}$ です。その行列式は $D = (X-x)(X-\overline{x})-\gamma yy= X^2-T_F(q)X + N_F(q)$ (cf. 公式 (3)) に等しい。 D 属するから K[X] までなので、$N(D) = D^2$ になります。 命題 1 が続きます。

#### 注意 1 {#alg-viii-s19-n1-rem-1 .statement tag=00LR}

K の特性が 2 と集合 $i'= 2i-\beta$ と異なるとします。すると、$(1, i')$ は K 上の E の基底で、${i'}^2= 4\alpha +\beta^2$ になります。従って、E は型 $(4\alpha +\beta^2,0)$ の二次代数と同型であり、F は型 $(4\alpha +\beta^2,0, \gamma )$ の四元数代数と同型です。

#### 注意 2 {#alg-viii-s19-n1-rem-2 .statement tag=00LS}

型 $(\alpha ,0, \gamma )$ の四元数代数は、型 $(\gamma ,0, \alpha )$ (III, §2, No. 5, p. 445) の四元数代数と同型です。また、K の非零元のすべての対 $(a, c)$ の型 $(\alpha a^2,0, \gamma c^2)$ の四元数代数にも同型です。

#### 注意 3 {#alg-viii-s19-n1-rem-3 .statement tag=00LT}

$q$ を F の元とします。すると、$q$ は、その特性多項式が $X^4$、つまり $T_F(q) = N_F(q) = 0$ に等しい場合にのみゼロポテントになります。すると$q^2= 0$になります。

#### 例 {#alg-viii-s19-n1-exa-1 .statement tag=00LU}

行列環 $\mathbf{M}_2(K)$ は、型 $(0,1,1)$ の四元数代数と同型です。実際、二次代数 $E = K\times K$ (型 $(0,1)$) と四元数代数 $F = E + Ej$ (元 $\gamma = 1$ によって定義される E の Cayley 拡大) を考えてみましょう。 写像 $(a, b)\mapsto \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix}$ は、E から $\mathbf{M}_2(K)$ までの代数準同型です。 K の $a, b$ については、次のようになります。

$$
(01)((01)(10)(01)((a0)(b0)((01)
$$

=、=、

1 0 1 0 0 1 1 0 0 $b$ 0 $a$ 1 0

この準同型拡大するから代数準同型 $\theta : F\longrightarrow \mathbf{M}_2(K)$ は次のように定義されます

$$
(ac)
$$

$$
\theta ((a, b) + (c, d)j)=
$$

$$
db
$$

この準同型は全単射です。 K の標数が 2 と異なる場合、代数 $\mathbf{M}_2(K)$ は型 $(1,0,1)$ (注意 1) の四元数代数とも同型です。

### 2. 四元数代数中中心

$\alpha ,\beta ,\gamma$ を K の元とし、F を型 $(\alpha , \beta , \gamma )$ の四元数代数とします。

#### 命題 2 {#alg-viii-s19-prop-2 .statement tag=00LV}

a) 体 K が 2 とは異なる特性を持っているとします。$\gamma$ または $4\alpha +\beta^2$ が非零の場合、F の中心は K に等しくなります。それ以外の場合は、次元 2 があり、1 と $ij-ji$ によって生成されます。

b) 体 K が特性 2 を持つと仮定します。$\beta \not= 0$ の場合、F の中心は K に等しくなります。 $\beta = 0$ の場合、代数 F は可換です。

III, §2, No. 5、p. 444 の公式 (30) までに、

$$
ij-ji=-\beta j+ 2k ,jk-kj=\beta \gamma -2\gamma i ,ki-ik=-2\alpha j-\beta k \tag{4}
$$

F の元 $q=x+yi+zj+tk$ は、$i$ および $j$ と可換である場合に限り、中心になります。

(5) $2z+\beta t=-\beta z+ 2\alpha t= 0$ と $2\gamma t=\beta \gamma t= 2y=\beta y= 0$。

まず、K の特性が 2 とは異なると仮定します。$\gamma$ が非零の場合、(5) の等式は $y=t= 0$、次に $z= 0$ を意味します。従って、$q\in K$ となります。 $\gamma = 0$ と $4\alpha +\beta^2\not= 0$ の場合、それらは $y=z=t= 0$ を意味するため、$q\in K$ になります。 $\gamma = 4\alpha +\beta^2= 0$なら、系 (5) 簡約するから$y= 2z+\beta t= 0$なので、$q=x+t/2(ij-ji)$となり、a)の証明が完成します。

ここで、体 K が標数 2 を持つと仮定します。 系 (5) は、$\beta t=\beta z=\beta y= 0$ と書くことができます。 主張 b)が続きます。

### 3. 四元数代数のシンプルさ

#### 命題 3 {#alg-viii-s19-prop-3 .statement tag=00LW}

$\alpha ,\beta ,\gamma$ を K の元とし、$f$ を型 $(\alpha , \beta , \gamma )$ の四元数代数とします。その Cayley トレースとノルムを $T_F$ と $N_F$ で表します。次のプロパティは同等です。

(i) 代数 F は中心単純です。

(ii) F のすべての非零元 $x$ に対して、$T_F(xy)\not= 0$ となるような F に元 $y$ が存在します。

(iii) $(4\alpha +\beta^2)\gamma \not= 0$ があります。

これらが性質が成り立つだとします。次に、F のすべての $x$ について、$x$ の縮小特性多項式は $X^2-T_F(x)X + N_F(x)$ になります。特に、$T_F(x)$は$x$の簡約トレースであり、$N_F(x)$はその被約ノルムです。

(i)⇒(ii): If the algebra F is central simple, then it follows from Proposition 1 of VIII, p. 361 and the definition of the reduced trace (VIII, p. 340, Definition 2) that $T_F$ is its reduced trace; assertion (ii) follows (VIII, p. 343, Proposition 5).

(ii)⇔(iii): 型 $(\alpha, \beta, \gamma)$ (III, §2, No. 5, p. 445) の F の基底を $(e_i)_{1 \leq i \leq 4}$ とします。 行列 $(T_F(e_i e_j))$ は次と等しい

$$
\begin{pmatrix}
2 & \beta & 0 & 0 \\
\beta & 2\alpha + \beta^2 & 0 & 0 \\
0 & 0 & 2\gamma & \beta\gamma \\
0 & 0 & \beta\gamma & -2\alpha\gamma
\end{pmatrix}.
$$

その行列式は$-\gamma^2 (4\alpha + \beta^2)^2$です。性質 (ii) および (iii) の同値は、V, §8, No. 2、p. 49、補題 1 から続きます。

(iii)⇒(i): $(4\alpha + \beta^2)\gamma \neq 0$ とします。次に、$\gamma \neq 0$ が得られ、K が特性 2 を持つ場合は $\beta \neq 0$ が得られます。命題 2 までに、代数 F が中心になります。 x をジェイコブソンの元根基の F とします。すべての $y \in F$ に対して、$xy$ は零であるため、$T_F(xy) = 0$ (注意 VIII、p. 362 の 3) となります。 (ii) は (iii) と同等なので、$x = 0$ になります。これは、F が半単純 K-代数であることを証明します。 中心はKなので簡単です。

最後の主張は、簡約特性多項式 (VIII、p. 340、定義 1) の VIII、p. 361、定義の命題 1 から続きます。

K の特性を p で表します。 命題 3 までに、$p \neq 2$ の場合、$K^*$ の $\alpha$ と $\gamma$ を含む型 $(\alpha, 0, \gamma)$ の K 上のすべての四元数代数が中心単純です。 $p = 2$ の場合、型 $(\alpha, 1, \gamma)$ のすべての四元数代数と $\alpha \in K$ と $\gamma \in K^*$ が中心単純です。逆に次のようなこともあります。

#### 命題 4 {#alg-viii-s19-prop-4 .statement tag=00LX}

*A を K 上の次数 4 の中心単純代数とする。K の特性を p で表す。*

a) * $p \neq 2$ の場合、代数 A が型 $(\alpha, 0, \gamma)$ の四元数代数と同型となるような K の非零元 $\alpha$ と $\gamma$ が存在します。

b) *$p = 2$ の場合、K の元 $\alpha$ と $K^*$ の元 $\gamma$ が存在し、代数 A は型 $(\alpha, 1, \gamma)$ の四元数代数と同型です。

ウェダーバーンの定理 (VIII, p. 120, 定理 1) によれば、A が $\mathbf{M}_r(D)$ と同型であるような中心 K を持つ整数 $r \geq 1$ と体 D が存在します。次に、$r^2[D : K] = [A : K] = 4$ になります。 $r = 2$ の場合、A は $\mathbf{M}_2(K)$ と同型で、命題 4 は VIII、p. 362 の例から続きます。それ以外の場合、$r = 1$ があり、A は中心 K を含む体になります。すると、K の分離拡大である最大可換部分体 E があります。 A は K に対して次数 4 を持っているため、拡大 E は K に対して次数 2 を持っています (VIII、p. 265、系 2)。したがって、これは 2 次 (III, §2, No. 3, p. 439) です。 $s$ を E の共役 (III, §2, No. 3, p. 440) とします。 Skolem-Noether 定理 (VIII, p. 256, 系 1) により、E のすべての $x$ に対して $s(x) =jxj^{-1}$ が得られるような A の可逆元 $j$ が存在します。 体 E は K 上で分離可能であるため、次のようになります。 $s\not=$ Id$_E$、つまり $j \notin E$。 A は K 上の次元 4 のベクトル空間であるため、E 上の次元 2 の左ベクトル空間なので、$A = E\oplus Ej$ になります。 $s^2=$ Id$_E$ があるため、A の属するから中心までの元 $j^2$ です。したがって、$j^2=\gamma$ となる $K^*$ の元 $\gamma$ が存在します。

$p\not= 2$ のとき、E の元 $i$ と元 $\alpha \in K^*$ が存在し、$E = K(i)$ と $i^2=\alpha$ (V, §11, No. 9, p. 93, 例 3) になります。この場合、A は型 $(\alpha ,0, \gamma )$ の四元数代数と同型です。 $p= 2$ のとき、E の元 $i$ と K の元 $\alpha$ が存在し、$E = K(i)$ と $i^2=i+\alpha$ (V, §11, No. 9, p. 93, 例 2) となるため、A は次と同型です。 型 $(\alpha ,1, \gamma )$の四元数代数。

#### 系 1 {#alg-viii-s19-prop-4-cor-1 .statement tag=00LY}

A を有限次数 $>1$ の中心単純K-代数とし、その元はすべて K 上の次数 $\leqslant 2$ の代数であるとします。そのとき、A は K 上の四元数代数と同型です。

K が有限の場合、代数 A は行列環 $\mathbf{M}_n(K)$ (VIII, p. 357, 系 2) と同型であるため、K 上の次数 $n$ の含む元です。 仮定は $n= 2$ を意味するため、この場合の結果は (VIII、p. 362、例) になります。 体 K が無限大であると仮定します。 L を A の極大エタール部分代数とします。 V, §7, No. 4、p. 41、命題 7 より、K-代数 L が $K[x]$ に等しいような A の元 $x$ が存在します。 仮定には次数 $\leqslant 2$ があります。 $[A : K] = [L : K]^2$ (VIII、p. 264、命題 4 および p. 262、命題 3) があるため、結論する [A : K] = 4 となります。系 1 は、命題 4 から続きます。

#### 系 2 {#alg-viii-s19-prop-4-cor-2 .statement tag=00LZ}

$(E, s)$ を K 上のケイリー 代数とし、K-代数 E が K 上の有限次数 $>1$ の中心単純となるようにします。このとき、E は K 上の四元数代数と同型です。

E のすべての元 $u$ は $u^2-T_E(u)u+ N_E(u) = 0$ を満たすため、K-代数 E は四元数代数 (系 1) と同型です。

### 4. 四元数代数が体になるための基準

$\alpha , \beta , \gamma$ を体 K の元とし、F を型 $(\alpha , \beta , \gamma )$ の四元数代数とします。 No.1と同様に、Fの標準基底を$(1, i, j, k)$で、Fの部分代数$K + Ki$をEで表します。

#### 命題 5 {#alg-viii-s19-prop-5 .statement tag=00M0}

次のプロパティは同等です。

(i) 四元数代数 F は体です。

(ii) $T_F(q) = N_F(q) = 0$ となるような非零元 $q\in F$ は存在しません。

(iii) 二乗零の F のすべての元は零です。

(iv) $K^4$ には、次のような非零ベクトル $(x, y, z, t)$ は存在しません。

$$
x^2+\beta xy-\alpha y^2-\gamma (z^2+\beta zt-\alpha t^2) = 0
$$

(v) $K^3$ には、次のような非零ベクトル $(x, y, z)$ は存在しません。

$$
x^2+\beta xy-\alpha y^2-\gamma z^2= 0
$$

(vi) 二次代数 E は体であり、$\gamma$ は E の元のノルムではありません。

F の元 $q$ は、$N_F(q)$ が 0 でない場合にのみ反転可能です。 したがって、(i) および (iv) の同値は、III, §2, No. 5、p. 445 の公式 (31) から続きます。 (i) が (iii) を意味し、(iv) が (v) を意味することは明らかです。

(ii)と(iii)の同値は、VIII、p. 362の注意3から続きます。

F が体ではないとします。 $\gamma (4\alpha +\beta^2)\not= 0$ の場合、代数 F は K 上の次数 4 の中心単純です。これは代数 $\mathbf{M}_2(K)$ (VIII, p. 120, 定理 1) と同型なので、二乗零の含む非零元となります。 $\gamma = 0$ の場合、$j^2= 0$ になります。 $4\alpha +\beta^2= 0$の場合、Kが2とは異なる特性を持っていれば、$(2i-\beta )^2= 0$と$2i-\beta \not= 0$が得られます。最後に、Kが特性2を持ち、$\beta$が零であれば、$q\in F$ごとに$T_F(q) = 0$が得られます（III, §2, No. 5、p. 445、公式） (31))。 F は体ではないので、$N_F(q) = 0$ となるような F の非零元 $q$ が存在します。 $q^2= 0$があります。これは、(iii)$\Rightarrow$(i) の含意を証明します。

$q=x+yi$ を E の元とします。$N_{E/K}(q) =x^2+\beta xy-\alpha y^2$ があります。 性質 (v) が成り立つとします。 $q\not= 0$ の場合、$N_{E/K}(q)-\gamma \not= 0$ と $N_{E/K}(q)\not= 0$ があり、したがって (vi) になります。

最後に、性質 (vi) が成り立つと仮定します。 $q$ を F の非零元とします。 E で $u$ と $v$ を使用して、$u+vj$ と書きます。$v$ が零の場合、$q$ は可逆です。 $v$ が零でない場合、III, §2, No. 5、p. 443、公式により $N_F(q) = N_F(v)N_F(v^{-1}u+j) =$ $N_{E/K}(v)(N_{E/K}(v^{-1}u)-\gamma )$ が得られます (24)。 $\gamma$ はノルムではないため、$N_F(q)$ は零ではなく、$q$ は反転可能です。

#### 注意 {#alg-viii-s19-n4-rem-1 .statement tag=00RQ}

四元数代数 F が体であるとします。 等式 $j^2=\gamma$ から、$\gamma \not= 0$ が得られます。 VIII、p. 363、中心の命題により、F の 〜でない限り K は標数 2 を持ち、$\beta$ は零となり、この場合代数 F は可換です。

### 5. 代数極大順序体

R を極大順序体 (VI, §2, No. 5, p. 25) とします。 C を型 $(-1,0)$ の 2 次式 R-代数とします。 $(1, i)$ がその標準基底であれば、$i^2=-1$ になります。また、CはR(VI, §2, No. 6、p. 26、定理3)の代数閉包です。 H を型 $(-1,0,-1)$ の四元数 R-代数とします。 H の標準基底 $(1, i, j, k)$ の乗法表は次のように与えられます。

$$
i^2=j^2=k^2=-1,ij=-ji=k,-ik=ki=j ,jk=-kj=i
$$

私たちは同一視する C と H の部分代数 $R + Ri$ です。H の元 $q=x+yi+zj+tk$ の共役は $\overline{q}=x-yi-zj-tk$ です。 Cayley トレースと $q$ のノルムは次のように与えられます。

$$
T(q) =q+\overline{q}= 2x ,N(q) =qq=x^2+y^2+z^2+t^2
$$

R が順序体なので、$q\not= 0$ なら $N(q)>0$ なので、H は体となり、中心 R (VIII, p. 363, 命題 2) となります。 H の元 $q$ の簡約トレースとノルムは、それぞれ $T(q)$ と $N(q)$ です。

#### 定理 1 {#alg-viii-s19-thm-1 .statement tag=00M1}

D を有限次数の R-代数、つまり体とします。このとき、D は R、C、または H と同型です。

Dの中心をZで表し、LをDの最大可換部分体とします。VIII、p. 265、系2により$[D : Z] = [L : Z]^2$が得られます。 C は R の代数閉包であるため、$[L : R]\leqslant 2$ もあります。従って、考えられるケースは 3 つあります。

a) R = Z = L であるため、[D : Z] = 1 および D = R となります。

b) $R\not= Z$ および Z = L があるため、[D : Z] = 1 および D = L となります。この場合、D は C と同型です。

c) R = Z および [L : R] = 2 であるため、[D : R] = 4 です。 VIII、p. 364、R-代数の命題 4 より、D は型 $(\alpha ,0, \gamma )$ の四元数代数と同型です。 $\alpha$ と $\gamma$ は R の非零元です。 $i\in D$- Z を $i^2=\alpha$ となるようにします。 $\alpha \not= 0$があります。 $\alpha  >0$ の場合、$a^2=\alpha$ (VI, §2, No. 6, p. 26, 定理 3) のような $a\in R$ が存在します。次に、$(a-i)(a+i) = 0$ になりますが、D は体であるため、これは不合理です。従って、$\alpha  <0$ になります。 不等式 $\gamma  <0$ も同様に表示されます。次に、$\alpha =-a^2$ と $\gamma =-c^2$ のように、$R^*$ の元 $a$ と $c$ が存在します (上記参照)。従って、代数 D は、型 $(-1,0,-1)$ (VIII, p. 362, 注意 2) の四元数代数、つまり H と同型です。

#### 注意 1 {#alg-viii-s19-n5-rem-1 .statement tag=00M2}

O を R 上の型 $(-1,0,-1,-1)$ の八元数代数とします (III、付録、No. 3、p. 615)。 D を R 上の別のケイリー 代数とし、D のすべての非零元が逆数を持つようにします。 証明できる (VIII, p. 370, 練習問題 5) は、D が R、C、H、または O と同型であると考えます。

#### 注意 2 {#alg-viii-s19-n5-rem-2 .statement tag=00M3}

上記は実数の体$\mathbf{R}$に適用されます。 有限次数、つまり体のすべての $\mathbf{R}$-代数は、$\mathbf{R},\mathbf{C}$ または $\mathbf{H}$ と同型です。

#### 注意 3 {#alg-viii-s19-n5-rem-3 .statement tag=00M4}

A を体 $\mathbf{R}$ 上の標準代数とする。 A が体であるとします。このとき、A は $\mathbf{R},\mathbf{C}$ または $\mathbf{H}$ (“Gelfand–Mazur 定理”) (cf. Comm. Alg., VI, §6, No. 4, p. 407, 定理 1 および TS, I, §2, n$^o5$, p. 26、系 $2$)$.*$

### 練習問題 {#alg-viii-s19-exercises}

[§ 19 に対して練習問題](exercises/s19/)を参照してください。

[^1]: In the case when $\beta = 0$, it is also said that F is a quaternion algebra of type $(\alpha , \gamma )$.
