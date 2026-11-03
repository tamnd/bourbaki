---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 19
section_title: Quaternion Algebras
lang: zh
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
content_sha256: d1f063f57d6a89a788e74089dc9b9756badacbd7a4f9f2ba8a74af8e0c308be0
translated_from: content/en/alg/VIII/19_s19_quaternion_algebras.md
translation_method: google
source_content_sha256: 108f7dda8f7849f663b2ef3f83020f45b2cebb199a339be51e597d680bf6aafa
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: d94fdf2557b1d893159d069d6cfa8ef7aa6badad112cfd60821ed9393e5a9fa7
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 19。 四元数代数

在这个截面中，K是交换域。

### 1. 四元数代数的一般性质

令$\alpha , \beta , \gamma$为K的元素，并令F为型$(\alpha , \beta , \gamma )$的四元数代数。回想一下 (III, §2, No. 5, p. 445)[^1]，F 是一个结合单位 K-代数，在 K 满足关系上有基 $(1, i, j, k)$

$$
i^2=\alpha +\beta i ,j^2=\gamma  ,ij=k ,ji=\beta j-k \tag{1}
$$

它是一个 Cayley 代数 (III, §2, No. 4, p. 441, 定义 1)，其共轭满足

$$
\overline{i}=\beta -i ,\overline{j}=-j ,\overline{k}=-k \tag{2}
$$

回想一下，F 的凯莱迹和范数是由 $T_F(q) =q+\overline{q}$ 和 $N_F(q) =qq$ 定义的从 F 到 K 的映射 $T_F$ 和 $N_F$。

F 与基 $(1, i)$ 的线性子空间 E 是 F 的可交换凯莱子代数；它是型$(\alpha , \beta )$的二次代数，并且F可以与由$\gamma$（III, §2, No. 5，p. 444）定义的E的凯莱扩张识别。对于每个$z\in E$，我们有$zj=jz$。 F 的每个元素 $q$ 都可以唯一地写为 $x+jy$ 和 $x, y\in E$，并且我们有

$$
\overline{q}=\overline{x}-jy ,T_F(q) =x+\overline{x},N_F(q) =xx-\gamma yy \tag{3}
$$

#### 命题 1 {#alg-viii-s19-prop-1 .statement tag=00LQ}

F 的元素$q$特征多项式等于$(X^2-T_F(q)X + N_F(q))^2$。

综上所述，代数 F 是一个自由右 E 模，基 $(1, j)$。因而，F[X] 是一个自由右 E[X] 模，具有基 $(1, j)$。我们用 $u(P) =$ $(X-q)P$ 定义的右 E[X]-模块 F[X] 的$u$ 自同态来表示 $P\in F[X]$。 $q$的特征多项式是$u$的行列式，被视为K[X]-模F[X]的自同态。通过III, §9, No. 4、p. 546的命题 6，它等于N(det $u$)，其中N表示从E[X]到K[X]的范数。让我们将$q$写成$x+jy$和$x, y\in E$。 $u$相对于基$(1, j)$的矩阵为$\begin{pmatrix} X-x & -\gamma y \\ -y & X-\overline{x} \end{pmatrix}$；它的行列式等于$D = (X-x)(X-\overline{x})-\gamma yy= X^2-T_F(q)X + N_F(q)$（cf.公式（3））。从 D 属于到 K[X]，我们有 $N(D) = D^2$；接下来是命题1。

#### 注 1 {#alg-viii-s19-n1-rem-1 .statement tag=00LR}

假设K的特性不等于2，且集合$i'= 2i-\beta$。那么$(1, i')$是E除以K的基，我们有${i'}^2= 4\alpha +\beta^2$。由此可知，E 与型 $(4\alpha +\beta^2,0)$ 的二次代数同构，F 与型 $(4\alpha +\beta^2,0, \gamma )$ 的四元数代数同构。

#### 注 2 {#alg-viii-s19-n1-rem-2 .statement tag=00LS}

型 $(\alpha ,0, \gamma )$ 的四元数代数与型 $(\gamma ,0, \alpha )$ 的四元数代数同构 (III, §2, No. 5, p. 445)。对于 K 的非零元素的每个对 $(a, c)$，它也同构于型 $(\alpha a^2,0, \gamma c^2)$ 的四元数代数。

#### 注 3 {#alg-viii-s19-n1-rem-3 .statement tag=00LT}

令$q$为F的元素，则$q$幂零当且仅当其特征多项式等于$X^4$，即$T_F(q) = N_F(q) = 0$；那么我们就有$q^2= 0$。

#### 例 {#alg-viii-s19-n1-exa-1 .statement tag=00LU}

矩阵代数$\mathbf{M}_2(K)$同构于型$(0,1,1)$的四元数代数。事实上，考虑二次代数$E = K\times K$（型$(0,1)$）和四元数代数$F = E + Ej$，这是由元素$\gamma = 1$定义的E的凯莱扩张。从E到$\mathbf{M}_2(K)$，映射$(a, b)\mapsto \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix}$是代数同态。因为对于 K 中的$a, b$，我们有

$$
(01)((01)(10)(01)((a0)(b0)((01)
$$

=,=,

1 0 1 0 0 1 1 0 0 $b$ 0 $a$ 1 0

这个同态扩展到代数同态 $\theta : F\longrightarrow \mathbf{M}_2(K)$ 定义为

$$
(ac)
$$

$$
\theta ((a, b) + (c, d)j)=
$$

$$
db
$$

这个同态是双射的。当K的特性不等于2时，代数$\mathbf{M}_2(K)$也同构于型$(1,0,1)$（注1）的四元数代数。

### 2. 四元数代数的中心

令$\alpha ,\beta ,\gamma$为K的元素，并令F为型$(\alpha , \beta , \gamma )$的四元数代数。

#### 命题 2 {#alg-viii-s19-prop-2 .statement tag=00LV}

a) 假设域 K 具有不同于 2 的特性。如果$\gamma$ 或$4\alpha +\beta^2$ 为非零的，则 F 的中心等于 K；否则，它有维数 2 并且由 1 和 $ij-ji$ 生成。

b) 假设域 K 具有特征2。如果$\beta \not= 0$，则F 的中心等于K；如果$\beta = 0$，则代数 F 是可交换的。

通过III, §2, No. 5、p. 444的公式(30)，我们有

$$
ij-ji=-\beta j+ 2k ,jk-kj=\beta \gamma -2\gamma i ,ki-ik=-2\alpha j-\beta k \tag{4}
$$

F 的元素 $q=x+yi+zj+tk$ 是中心当且仅当它与 $i$ 和 $j$ 通勤，也就是说，我们有

(5)$2z+\beta t=-\beta z+ 2\alpha t= 0$和$2\gamma t=\beta \gamma t= 2y=\beta y= 0$。

首先假设K的特性不同于2。如果$\gamma$是非零的，则(5)中的等式隐含$y=t= 0$，然后隐含$z= 0$；因而，我们有 $q\in K$。如果$\gamma = 0$和$4\alpha +\beta^2\not= 0$，那么它们意味着$y=z=t= 0$，所以我们有$q\in K$。如果$\gamma = 4\alpha +\beta^2= 0$，则系统 (5) 约化到$y= 2z+\beta t= 0$，所以我们有$q=x+t/2(ij-ji)$，它完成了a)的证明。

现在假设域 K 具有特征2。则系统 (5) 可写为$\beta t=\beta z=\beta y= 0$； 断言 b)如下。

### 3. 四元数代数的简单性

#### 命题 3 {#alg-viii-s19-prop-3 .statement tag=00LW}

令$\alpha ,\beta ,\gamma$为K的元素，并令$f$为型$(\alpha , \beta , \gamma )$的四元数代数。用 $T_F$ 和 $N_F$ 表示其凯莱迹和范数。以下属性是等效的：

(i) 代数 F 是中心单形。

(ii) 对于 F 的每个非零元素 $x$，F 中都存在元素 $y$，使得 $T_F(xy)\not= 0$。

(iii) 我们有$(4\alpha +\beta^2)\gamma \not= 0$。

假设这些性质成立。那么对于F中的每一个$x$，$x$的约简特征多项式就是$X^2-T_F(x)X + N_F(x)$。特别地，$T_F(x)$是$x$的约化迹，$N_F(x)$是它的约化范数。

(i)⇒(ii): 如果代数 F 是中心单式，则从 VIII、p. 361 和定义约化迹 (VIII、p. 340、定义 2) 的命题 1 得出$T_F$ 是它的约化迹； 断言 (ii) 遵循 (VIII, p. 343, 命题 5)。

(ii)⇔(iii)：令$(e_i)_{1 \leq i \leq 4}$为型$(\alpha, \beta, \gamma)$(III, §2, No. 5，p. 445)的F的基。 矩阵 $(T_F(e_i e_j))$ 等于

$$
\begin{pmatrix}
2 & \beta & 0 & 0 \\
\beta & 2\alpha + \beta^2 & 0 & 0 \\
0 & 0 & 2\gamma & \beta\gamma \\
0 & 0 & \beta\gamma & -2\alpha\gamma
\end{pmatrix}.
$$

它的行列式是$-\gamma^2 (4\alpha + \beta^2)^2$。属性 (ii) 和 (iii) 的等价由 V, §8, No. 2、p. 49、引理 1 得出。

(iii)⇒(i): 假设$(4\alpha + \beta^2)\gamma \neq 0$。然后我们有 $\gamma \neq 0$，如果 K 具有特征 2，我们就有 $\beta \neq 0$。根据命题 2，代数 F 是中心。令x为F的Jacobson 根基的元素。对于每个$y \in F$，$xy$是幂零的，因此$T_F(xy) = 0$（VIII，p. 362的注 3）。由于 (ii) 等价于 (iii)，因此我们有 $x = 0$。这就证明F是半单K-代数。因为它的中心是K，所以很简单。

最后一个断言由约化特征多项式 (VIII、p. 340、定义 1) 的VIII、p. 361 和定义的命题 1 得出。

用 p 表示 K 的特性。到命题 3，如果$p \neq 2$，则$K^*$中型$(\alpha, 0, \gamma)$的K上的每个四元数代数以及$\alpha$和$\gamma$都是中心简单。如果$p = 2$，则型$(\alpha, 1, \gamma)$与$\alpha \in K$和$\gamma \in K^*$的每个四元数代数都是中心简单。相反，我们有以下情况。

#### 命题 4 {#alg-viii-s19-prop-4 .statement tag=00LX}

*设 A 为 K 上次数 4 的中心单代数。用 p 表示 K 的特征。*

a) *如果$p \neq 2$，则存在K的非零元素$\alpha$和$\gamma$，使得代数A与型$(\alpha, 0, \gamma)$的四元数代数同构。*

b) *如果$p = 2$，则存在K的元素$\alpha$和$K^*$的元素$\gamma$，使得代数A同构于型的四元数代数 $(\alpha, 1, \gamma)$.*

根据 Wedderburn 的定理 (VIII, p. 120, 定理 1)，存在整数 $r \geq 1$ 和域 D 以及中心 K，使得 A 与 $\mathbf{M}_r(D)$ 同构的。那么我们就有$r^2[D : K] = [A : K] = 4$。如果$r = 2$，则A与$\mathbf{M}_2(K)$同构的，命题4由VIII、p. 362的例推出。否则，我们有 $r = 1$，A 是域和中心 K。然后它有极大交换子域 E，即 K 的可分扩张；因为 A 比 K 有次数 4，扩张 E 比 K 有次数 2（VIII、p. 265、推论 2）。因此它是二次的（III, §2, No. 3，p. 439）。令 $s$ 为 E (III, §2, No. 3, p. 440) 的共轭。根据 Skolem–Noether 定理 (VIII, p. 256, 推论 1)，存在 A 的可逆元 $j$，因此对于 E 中的每个 $x$，我们都有 $s(x) =jxj^{-1}$。 域 E 是可分的超过 K，所以我们有 $s\not=$ Id$_E$，因此$j \notin E$。因为 A 是 K 上的维数 4 的向量空间，所以它是 E 上的维数 2 的左向量空间，所以我们有 $A = E\oplus Ej$。我们有$s^2=$Id$_E$，所以A的属于到中心的元素$j^2$；因此存在$K^*$的元素$\gamma$使得$j^2=\gamma$。

当$p\not= 2$时，存在E的元素$i$和元素$\alpha \in K^*$使得$E = K(i)$和$i^2=\alpha$（V, §11, No. 9，p. 93，例3）；在这种情况下，A 同构于型 $(\alpha ,0, \gamma )$ 的四元数代数。当$p= 2$时，存在E的元素$i$和K的元素$\alpha$，使得$E = K(i)$和$i^2=i+\alpha$（V, §11, No. 9，p. 93，例2），所以A是同构于型 $(\alpha ,1, \gamma )$ 的四元数代数。

#### 推论 1 {#alg-viii-s19-prop-4-cor-1 .statement tag=00LY}

设A是有限次数$>1$的中心单K-代数，其元素都是次数$\leqslant 2$在K上的代数。则A与K上的四元数代数同构。

如果 K 是有限的，则代数 A 同构于矩阵代数 $\mathbf{M}_n(K)$ (VIII, p. 357, 推论 2)，因此包含元素与次数 $n$ 在 K 上； 假设意味着 $n= 2$，因此本例中的结果为 (VIII、p. 362、例)。假设域 K 是无限的。设L为A的极大étale子代数。根据V, §7, No. 4、p. 41、命题7，存在A的元素$x$，使得K-代数L等于$K[x]$，因此假设有次数$\leqslant 2$。由于我们有 $[A : K] = [L : K]^2$ (VIII, p. 264, 命题 4 和 p. 262, 命题 3)，我们结论 [A : K] = 4。然后从命题 4 得出推论 1。

#### 推论 2 {#alg-viii-s19-prop-4-cor-2 .statement tag=00LZ}

设$(E, s)$是K上的凯莱代数，使得K-代数E是K上有限次数$>1$的中心单形。则E与K上的四元数代数同构。

E 的每个元素 $u$ 都满足 $u^2-T_E(u)u+ N_E(u) = 0$，因此 K-代数 E 同构于四元数代数 (推论 1)。

### 4. 判据四元数代数域

令$\alpha , \beta , \gamma$为域K的元素，并令F为型$(\alpha , \beta , \gamma )$的四元数代数。与No.1一样，我们用$(1, i, j, k)$表示F的典范基，用E表示F的子代数$K + Ki$。

#### 命题 5 {#alg-viii-s19-prop-5 .statement tag=00M0}

以下属性是等效的：

(i) 四元数代数 F 为域。

(ii) 不存在非零元素$q\in F$使得$T_F(q) = N_F(q) = 0$。

(iii) 平方为零的 F 的每个元素都是零。

(iv) $K^4$ 中不存在任何非零向量 $(x, y, z, t)$ 使得

$$
x^2+\beta xy-\alpha y^2-\gamma (z^2+\beta zt-\alpha t^2) = 0
$$

(v) $K^3$ 中不存在任何非零向量 $(x, y, z)$ 使得

$$
x^2+\beta xy-\alpha y^2-\gamma z^2= 0
$$

(vi)二次代数E是域，并且$\gamma$不是E的元素的范数。

F 的元素 $q$ 是可逆的，当且仅当 $N_F(q)$ 不为 0 时。因此，(i) 和 (iv) 的等价由 III, §2, No. 5、p. 445 的公式 (31) 得出；显然，(i) 意味着(iii)，(iv) 意味着(v)。

(ii)和(iii)的等价由VIII、p. 362的注 3得出。

假设 F 不是域。如果 $\gamma (4\alpha +\beta^2)\not= 0$，则代数 F 是次数 4 在 K 上的中心单形；它与代数 $\mathbf{M}_2(K)$ (VIII, p. 120, 定理 1) 同构的，因此包含非零元素等于平方为零。如果$\gamma = 0$，那么我们有$j^2= 0$。如果 $4\alpha +\beta^2= 0$，那么如果 K 具有不同于 2 的特征，则我们有 $(2i-\beta )^2= 0$ 和 $2i-\beta \not= 0$。最后，如果 K 具有特征 2 并且 $\beta$ 是零，那么对于每个 $q\in F$，我们有 $T_F(q) = 0$ (III, §2, No. 5，p. 445，公式) (31))。由于 F 不是域，因此 F 存在非零元素 $q$，使得 $N_F(q) = 0$；我们有$q^2= 0$。这就证明了蕴涵(iii)$\Rightarrow$(i)。

令$q=x+yi$为E的元素。我们有$N_{E/K}(q) =x^2+\beta xy-\alpha y^2$。假设性质 (v) 成立。如果 $q\not= 0$，我们有 $N_{E/K}(q)-\gamma \not= 0$ 和 $N_{E/K}(q)\not= 0$，因此 (vi)。

最后，假设性质 (vi) 成立。令$q$为F的非零元素；我们将它写为E中的$u+vj$和$u$和$v$。如果$v$是零，则$q$是可逆的。如果$v$不是零，那么我们有$N_F(q) = N_F(v)N_F(v^{-1}u+j) =$$N_{E/K}(v)(N_{E/K}(v^{-1}u)-\gamma )$乘以III, §2, No. 5、p. 443、公式 (24)。由于$\gamma$不是范数，$N_F(q)$不是零，并且$q$是可逆的。

#### 注 {#alg-viii-s19-n4-rem-1 .statement tag=00RQ}

假设四元数代数 F 是域。 从等式 $j^2=\gamma$ 可以得出$\gamma \not= 0$。 根据VIII、p. 363的命题2，F的中心等于K，除非K具有特征2且$\beta$为零，在这种情况下代数F是可交换的。

### 5. 代数超过极大有序域

令 R 为极大有序域 (VI, §2, No. 5, p. 25)。令C为型$(-1,0)$的二次方R-代数；如果$(1, i)$是它的典范基，那么我们就有$i^2=-1$。另外，C是R的代数闭包(VI, §2, No. 6、p. 26、定理3)。令 H 为型 $(-1,0,-1)$ 的四元数 R-代数。 H 在其典范基 $(1, i, j, k)$ 中的乘法表由下式给出

$$
i^2=j^2=k^2=-1,ij=-ji=k,-ik=ki=j ,jk=-kj=i
$$

我们H的认同C和子代数$R + Ri$。H的元素$q=x+yi+zj+tk$共轭是$\overline{q}=x-yi-zj-tk$。凯莱迹和 $q$ 的范数由下式给出

$$
T(q) =q+\overline{q}= 2x ,N(q) =qq=x^2+y^2+z^2+t^2
$$

由于 R 为有序域，如果 $q\not= 0$，则有 $N(q)>0$，因而 H 为域，其中中心 R (VIII，p. 363，命题 2)。 H的元素$q$的约化迹和范数分别是$T(q)$和$N(q)$。

#### 定理 1 {#alg-viii-s19-thm-1 .statement tag=00M1}

令 D 为有限次数中的 R-代数，即域。则 D 同构于 R、C 或 H。

用 Z 表示 D 的中心，并设 L 为 D 的极大交换子域。我们通过 VIII、p. 265、推论 2 得到 $[D : Z] = [L : Z]^2$；我们还有$[L : R]\leqslant 2$，因为C是R的代数闭包。因此存在三种可能的情况：

a) 我们有 R = Z = L，因而 [D : Z] = 1 并且 D = R。

b) 我们有 $R\not= Z$ 且 Z = L，因而 [D : Z] = 1 且 D = L。在这种情况下，D 同构于 C。

c) 我们有 R = Z 且 [L : R] = 2，因而 [D : R] = 4。通过 VIII、p. 364、R-代数的命题 4，D 同构于型 $(\alpha ,0, \gamma )$ 的四元数代数，其中$\alpha$和$\gamma$是R的非零元素。令$i\in D$-Z使得$i^2=\alpha$。我们有$\alpha \not= 0$。如果$\alpha  >0$，则存在$a\in R$，使得$a^2=\alpha$ (VI, §2, No. 6，p. 26，定理 3)；然后我们有$(a-i)(a+i) = 0$，这是荒谬的，因为D是域。所以我们有$\alpha  <0$。 不等式 $\gamma  <0$ 类似地显示。则存在元素$a$和$c$或$R^*$使得$\alpha =-a^2$和$\gamma =-c^2$（前述）。因而，代数 D 同构于型 $(-1,0,-1)$ (VIII, p. 362, 注 2) 的四元数代数，即同构于 H。

#### 注 1 {#alg-viii-s19-n5-rem-1 .statement tag=00M2}

令 O 为型 $(-1,0,-1,-1)$ 在 R 上的八元数代数 (III, 附录, No. 3, p. 615)。令 D 为 R 上的凯莱代数代数，使得 D 的每个非零元素都有一个逆元。我们可以证明 (VIII, p. 370, 习题 5) D 与 R、C、H 或 O 同构的。

#### 注 2 {#alg-viii-s19-n5-rem-2 .statement tag=00M3}

以上适用于实数的域$\mathbf{R}$。 有限次数的每个$\mathbf{R}$-代数即域同构于$\mathbf{R},\mathbf{C}$或$\mathbf{H}$。

#### 注 3 {#alg-viii-s19-n5-rem-3 .statement tag=00M4}

设 A 是域 $\mathbf{R}$ 上的标准化代数。假设A是域。则 A 同构于 $\mathbf{R},\mathbf{C}$，或 $\mathbf{H}$ (“Gelfand–Mazur 定理”) (cf. Comm. Alg., VI, §6, No. 4, p. 407, 定理 1 和 TS, I, §2, n$^o5$, p. 26, 推论 $2$)$.*$

### 习题{#alg-viii-s19-exercises}

参见[习题为 § 19](exercises/s19/)。

[^1]: In the case when $\beta = 0$, it is also said that F is a quaternion algebra of type $(\alpha , \gamma )$.
