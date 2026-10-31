---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 2
section_title: Examples of algebras
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 438-457, 618-626
pdf_pages: 0462-0481, 0642-0650
extraction: ocr
subsections:
    - "no": 1
      title: ENDOMORPHISM ALGEBRAS
      page: 438
      pdf_page: 462
    - "no": 2
      title: MATRIX ELEMENTS
      page: 438
      pdf_page: 462
    - "no": 3
      title: QUADRATIC ALGEBRAS
      page: 439
      pdf_page: 463
    - "no": 4
      title: CAYLEY ALGEBRAS
      page: 441
      pdf_page: 465
    - "no": 5
      title: CONSTRUCTION OF CAYLEY ALGEBRAS. QUATERNIONS
      page: 443
      pdf_page: 467
    - "no": 6
      title: ALGEBRA OF A MAGMA, A MONOID, A GROUP
      page: 446
      pdf_page: 470
    - "no": 7
      title: FREE ALGEBRAS
      page: 448
      pdf_page: 472
    - "no": 8
      title: DEFINITION OF AN ALGEBRA BY GENERATORS AND RELATIONS
      page: 450
      pdf_page: 474
    - "no": 9
      title: POLYNOMIAL ALGEBRAS
      page: 452
      pdf_page: 476
    - "no": 10
      title: TOTAL ALGEBRA OF A MONOID
      page: 454
      pdf_page: 478
    - "no": 11
      title: FORMAL POWER SERIES OVER A COMMUTATIVE RING
      page: 455
      pdf_page: 479
statements: 17
exercises: 25
content_sha256: fbbe0c59baeee276aaa480a6bc23861bf5d82dabf1a209abf39e243a5b8866de
translated_from: content/en/alg/III/02_s2_examples_of_algebras.md
translation_method: google
source_content_sha256: 523c00d5d47e83c328fe974b4b99f51c3c18998f5e378badbbbbd303ed1feec8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 1180c30008a694ff9a7fe7606211c20e01fa34e5c4e98f9eec1b7cefde1d1760
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 2。 例 / 代数

在本段中，A 表示交换环。

### 1.内同态代数

令 B 为结合律 A-代数，其中单位元用 1 表示，并令 M 为右B-模。我们知道B的环$E = \mathrm{End}_B(M)$还有模结构超过中心。现在A到B的同态$h : \alpha \mapsto \alpha . 1$的像包含在B的中心中（§ 1, no. 1）；因此 $h$ 给出 E A-模结构。此外，对于 E 中的 $\alpha \in A$ 和 $f, g$，

$$
\alpha(f \circ g) = f \circ (\alpha g) = (\alpha f) \circ g;
$$

因此，E 中的乘法和 E 上的 A-模结构定义是 E 上的联想 A-代数结构； M 的恒等映射是这个代数的单位元。

### 2.矩阵元素

设 B 是 B (II, § 10, no. 7) 上阶 n 的平方矩阵的酉结合A-代数和$\mathbf{M}_n(B)$ 集合。那么$\mathbf{M}_n(B)$有由$\alpha . (b_{ij}) = (\alpha b_{ij})$($\alpha \in A, b_{ij} \in B, 1 \leq i \leq n, 1 \leq j \leq n$)定义的A-模结构；这个结构和矩阵乘法定义是$\mathbf{M}_n(B)$上的统一联想A-代数结构。 $\mathbf{M}_n(B)$到$\mathrm{End}_B(B_d^n)$（II, § 10, no. 7）的规范双射是A-代数同构。

当$B = A$、A-代数$\mathbf{M}_n(A)$承认矩阵单位(II, § 10, no. 3)的典范基$(E_{ij})$由……组成时； 相应的乘法表是

$$
E_{ij} E_{hk} = \delta_{jh} E_{ik}.
$$

单位元 $I_n$ 等于 $\sum_{i=1}^n E_{ii}$。

### 3.二次代数

令$\alpha, \beta$为A的两个元素和$A^2$的$(e_1, e_2)$典范基。 A 上的型 $(\alpha, \beta)$ 的二次代数为 A-模 $A^2$，其中代数结构由乘法表 (§ 1, no. 7) 定义

$$
e_1^2 = e_1, \quad e_1 e_2 = e_2 e_1 = e_2, \quad e_2^2 = \alpha e_1 + \beta e_2.
$$

与二次代数同构的A-代数E也称为二次代数。这相当于说 E 承认两个元素中的基，其中一个是单位元。

可以证明，每个允许两个元素中的基的单位A-代数都是二次代数（习题1）。

如果A-代数的基$(e_1, e_2)$有乘法表(2)，则称为型$(\alpha, \beta)$的基。通过滥用语言，当基为型 $(\alpha, \beta)$ 时，二次代数被称为型 $(\alpha, \beta)$。

#### 命题 1 {#alg-iii-s2-prop-1 .statement tag=05YX}

*二次代数 E 是结合律和交换律。*

E 是可交换的，这一事实由 (2) 中的方程 $e_1 e_2 = e_2 e_1$ 得出；类似地，要验证结合性，只要看到当$x, y, z$分别等于$e_1$或$e_2$时，$x(yz) = (xy)z$就足够了。现在，如果元素 $x, y, z$ 至少有一个等于$e_1$，则关系是显而易见的；对于 $x = y = z = e_2$ 也是如此，因为 E 是可交换的； 从而命题。

令$e$表示二次代数E的单位元，令$(e, i)$为型$(\alpha, \beta)$E的基；因此，E 包含于 $e$ 的所有其他基都是形式 $(e, j)$ 和 $j = \gamma e + \delta i$（II, § 7, no. 2，命题 3 的推论）；此外，要使$(e, j)$成为E的基，$\delta$在A中可逆是充分必要的； 条件显然就足够了；反之，如果$E/Ae$、$\bar{i}$和$\bar{j} = \delta \bar{i}$中$\bar{i}$是$i$的典范像，则必须$E/Ae$、从而各形式、基的必要性条件。然后

$$
j^2 = (\gamma^2 + \alpha \delta^2)e + (2\gamma \delta + \beta \delta^2)i = (\alpha \delta^2 - \gamma^2 - \beta \gamma \delta)e + (2\gamma + \beta \delta)j;
$$

由此可知E为型

$$
(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)
$$

对于所有可逆的$\delta \in A$和所有$\gamma \in A$。特别是，如果 $E$ 为型 $(\alpha, 2\beta')$，则 $i$ 也为型 $(\alpha + {\beta'}^2, 0)$，如取 $\gamma = -\beta'$ 和 $\delta = 1$ 所示。

#### 命题 2 {#alg-iii-s2-prop-2 .statement tag=05YY}

*设$E$为二次$A$代数，$e$为单位元。对于所有$u \in E$，令$T(u)$为自由$A$-模块$E$（II, § 4, no. 3）的自同态$m_u : x \mapsto ux$的踪迹。那么对于所有 $u \in E$，由 $s(u) = T(u).e - u$ 定义的映射 $s$ 是代数 $E$ 和 $s^2(u) = u$ 的自同构。*

设$(e, i)$为型$(\alpha, \beta)$$E$基；然后$T(e) = 2$，当$s(e) = e$，以及$T(i) = \beta$，从而$s(i) = \beta e - i$。因此，$(e, s(i))$是$E$的基，其型由(3)与$\gamma = \beta$和$\delta = -1$给出，这又给出$(\alpha, \beta)$；由此可见，$s$ 是代数 $E$ 中的自同构。由于$A$模块$E$的$m_{s(u)} = s m_u s^{-1}$、自同态$m_u$和$m_{s(u)}$具有相同的迹线（II, § 4, no. 3、命题3）、从而

$$
s^2(u) = T(u).e - s(u) = T(u).e - (T(u).e - u) = u
$$

对于所有$u \in E$。

自同构 $s$ 称为$A$代数$E$的*共轭*和$s(u)$$u$的*共轭*。

如果$u = \xi e + \eta i$，$A$中有$\xi, \eta$，则$s(u) = (\xi + \beta \eta)e - \eta i$，从而

(4)
$$
T(u)e = u + s(u) = (2\xi + \beta \eta)e
$$
(5)
$$
u.s(u) = (\xi^2 + \beta \xi \eta - \alpha \eta^2)e = N(u)e
$$

我们写了$N(u) = \xi^2 + \beta \xi \eta - \alpha \eta^2$。 元素$T(u)$和$N(u)$（或者，当$A$和$Ae$被规范识别时，元素$T(u)e$和$N(u)e$）分别称为$u$的*trace*和*范数*。

当$\beta = 0$时，上面的公式简化为

(6)
$$
s(\xi e + \eta i) = \xi e - \eta i, \quad T(\xi e + \eta i) = 2\xi, \quad N(\xi e + \eta i) = \xi^2 - \alpha \eta^2.
$$

显然，$T$是$E$*上的*线性形式*，并且*$N$是$E$(IX, § 3, no. 4)*上的*二次形式*。由于 $E$ 是可交换和结合的，因此从 (5) 可以得出：

(7)
$$
N(uv) = N(u)N(v).
$$

对于$u$在*$E$中*可逆，$N(u)$在*$A$中*可逆是充分必要的。因为，作为$N(e) = 1$，条件的必要性由(7)得出，写作$v = u^{-1}$。相反，如果 $N(u)$ 在 $A$ 中是可逆的，则从 (5) 可以得出 $u$ 是可逆的，并且

(8)
$$
u^{-1} = (N(u))^{-1}s(u).
$$

*可以证明$N(u)$是自同态$m_u$的行列式(§ 8, no. 1)(cf.§ 9 no. 3,例1)*

以下命题给出二次代数与交换域的结构：

#### 命题 3 {#alg-iii-s2-prop-3 .statement tag=05YZ}

*设 E 为型* $(\alpha, \beta)$ 的二次A-代数。

(i) *如果 A 是域并且包含没有元素* $\zeta$ *使得* $\zeta^2 = \alpha + \beta \zeta$，*E 是（可交换的）域* (cf. V, § 3)。

(ii) *如果环* A *包含元素* $\zeta$ *使得* $\zeta^2 = \alpha + \beta \zeta$ *且* $\beta - 2\zeta$ *可逆*（分别零），*E 与* A $\times$ A *同构的。为型* $(0, 0))$。

我们证明（i）。设$\xi, \eta$是A和$u = \xi e + \eta i$的两个元素。如果$\eta \neq 0$并且我们写$\theta = -\xi \eta^{-1}$，那么通过(5)可以得到$\mathrm{N}(u) = \eta^2 (\theta^2 - \beta \theta - \alpha)$，通过A上的假设可以得到从而$\mathrm{N}(u) \neq 0$；如果$\eta = 0$，则$\mathrm{N}(u) = \xi^2$。无论如何，如果$u \neq 0$，则$\mathrm{N}(u) \neq 0$，因此$\mathrm{N}(u)$在A中可逆，因此$u$在E中可逆。

我们现在证明(ii)。 代数 A $\times$ 的典范基 $(e_1, e_2)$ A 的型 $(0, 1)$。我们已经看到 (公式 (3)) E 的值是型

$$
(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)
$$

对于A中所有$\gamma \in A$和所有$\delta$可逆。如果$\beta - 2\zeta$可逆，则取$\delta = (\beta - 2\zeta)^{-1}$和$\gamma = -\zeta (\beta - 2\zeta)^{-1}$；然后 $2\gamma + \beta \delta = 1$ 和

$$
\alpha \delta^2 - \gamma^2 - \beta \gamma \delta = \delta^2 (\alpha - \zeta^2 + \beta \zeta) = 0;
$$

因此E是型$(0, 1)$，因此与A$\times$A同构。如果$\beta - 2\zeta = 0$，已经指出E是型$(\alpha + \zeta^2, 0)$，因此从$\alpha + \zeta^2 = 2\zeta^2 - \beta \zeta = 0$开始是型$(0, 0)$。

型 $(0, 0)$ 的二次方 A-代数也称为 A 上的对偶数* 的 *代数。

### 4.凯利代数

#### 定义 1 {#alg-iii-s2-def-1 .statement tag=05Z0}

*Cayley 代数 over* A *是有序对* (E, s)，*其中* E *是代数 over* A *与单位元* e *和* s *是* E *的反自同构，使得*

$$
u + s(u) \in Ae \quad \text{and} \quad u.s(u) \in Ae
$$

*对于所有人*$u \in E$。

$s$ 被称为 Cayley 代数 (E, s) 的*共轭* 和 $s(u)$ $u$ 的 *共轭*。 条件 $u + s(u) \in Ae$ 意味着 $u$ 和 $s(u)$ 是*可改变的*。我们写

(9) $$
T(u) = u + s(u)
$$
(10) $$
N(u) = u.s(u) = s(u).u
$$

子代数 $Ae$ 的元素分别称为$u$ 的*凯莱迹* 和*范数*。

二次代数 E 的有序对由……组成及其共轭 s（这是反自同构，因为 E 是可交换的）(no. 3) 是凯莱代数。

令 (E, s) 为凯莱代数；如$s(e) = e,\ s(u + s(u)) = u + s(u)$，其他字$s(u) + s^2(u) = u + s(u)$或也

$$
s^2(u) = u
$$

因此 $s^2$ 是 E 的恒等映射。由此可知

$$
T(s(u)) = T(u), \quad N(s(u)) = N(u).
$$

最后，关系$(u - u)(u - s(u)) = 0$给出

$$
u^2 - T(u).u + N(u) = 0
$$

对于所有$u \in E$。

#### 命题 4 {#alg-iii-s2-prop-4 .statement tag=05Z1}

*设 E 为 A-代数，并且 s 和 s' E 的反自同构，使得 (E, s) 和 (E, s') 为 Cayley 代数。如果 E 承认基包含单位元 e，则 s' = s.*

显然 $s'(u) = s(u) = u$ 对于所有$u \in Ae$。如果 T, N（分别为 T', N'）是迹，且范数函数对于 (E, s)（分别为 (E, s')），则从 (13) 得出

$$
(T(u) - T'(u)).u - (N(u) - N'(u)) = 0.
$$

设 B 为 E 包含 e 的基，且不同于 e 的 B 的 u 元素；然后$T(u) - T'(u) = 0$，从而$s(u) = s'(u)$。由于 B 上的 s 和 s' 重合相等。

接下来，我们写$\bar{u} = s(u)$，这样

$$
\left\{\begin{array}{lll}
u + \bar{u} = T(u), & u\bar{u} = \bar{u}u = N(u), & \bar{u} = u \\
u + v = \bar{u} + \bar{v}, & \alpha u = \alpha \bar{u}, & uv = \bar{v}.\bar{u}
\end{array}\right.
$$

对于E中的$u, v$，$\alpha \in A$；而且

$$
T(e) = 2e, \quad N(e) = e.
$$

来自公式

$$
T(uv) = uv + \overline{uv} = uv + \bar{v}.\bar{u} = uv + (T(v) - v)(T(u) - u),
$$

我们推断

$$
uv + vu = T(u)v + T(v)u + (T(uv) - T(u)T(v))
$$

从而，交换$u$和$v$，

$$
T(vu) = T(uv).
$$

另一方面，$N(u + v) = (u + v)(\bar{u} + \bar{v}) = N(u) + N(v) + T(u\bar{v})$、从而

(18)
$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v).
$$

现在，将 (16) 应用的 $u$ 替换为 $\bar{u}$ 给出
$$
T(u\bar{v}) = T(u)T(v) + \bar{u}v + v\bar{u} - T(u)v - T(v)\bar{u} = T(u)T(v) - uv - \bar{v}.\bar{u};
$$
从而

(19)
$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v) = T(u)T(v) - T(uv).
$$

最后，对于所有$\alpha \in A$来说，显然，

(20)
$$
N(\alpha u) = \alpha^2 N(u);
$$
特别是 $N(2u) = 4N(u)$，因此公式 (19) 给出

(21)
$$
(T(u))^2 - T(u^2) = 2N(u).
$$

显然，$T$ 是$(Ae)$-模块$E$ 上的线性形式。由于$(u, v) \mapsto T(v\bar{u})$在此模上是双线性形式，*从(18)和(20)得出$N$是二次形式(cf.IX, § 3, no. 4)。*

### 5.凯利的构造代数。四元数

令$(E, s)$为$A$上的凯莱代数，为此我们将使用no. 4的记号，并令$\gamma \in A$。令$F$为代数超过$A$，其底层模为$E \times E$，其乘法定义为

(22)
$$
(x, y)(x', y') = (xx' + \gamma \bar{y}'y, y\bar{x}' + y'x);
$$
显然$(e, 0)$是$F$的单位元，$E \times \{0\}$是$F$的子代数，与$E$同构的；我们将在下文中*认同*它与$E$，以便$x \in E$与$(x, 0)$标识，特别是$e$与$F$的单位元标识。

令 $t$ 为 $F$ 的置换定义为

(23)
$$
t((x, y)) = (\bar{x}, -y) \quad (x \in E, y \in E).
$$

#### 命题 5 {#alg-iii-s2-prop-5 .statement tag=05Z2}

(i) *有序对 $(F, t)$ 是 Cayley 代数超过 $A$*。

(ii) *设 $j = (0, e)$，因此 $(x, y) = xe + yj$ 对应 $x \in E, y \in E$。凯莱迹以及 $F$ 的范数 $T_F$ 和 $N_F$ 由公式* 给出

(24)
$$
T_F(xe + yj) = T(x), \quad N_F(xe + yj) = N(x) - \gamma N(y).
$$

(iii) *要使 $F$ 具有结合性，$E$ 具有结合性和交换性是必要且充分的。*

对于$(x, y) \in \mathbf{F}$，

$$
(x, y) + t((x, y)) = (x + \overline{x}, 0) = T(x)e
$$
(25)
$$
(x, y)t((x, y)) = (x, y)(\overline{x}, -y) = (xx - \gamma \overline{y}y, y\overline{x} - yx)
= (\mathrm{N}(x) - \gamma \mathrm{N}(y), 0) = (\mathrm{N}(x) - \gamma \mathrm{N}(y))e.
$$
(26)

因此，为了证明 (i) 和 (ii)，只需证明 $t$ 是 $\mathbf{F}$ 的反自同构。显然 $t$ 是 A 线性双射。另一方面，
$$
t((x, y) \cdot (x', y')) = t((xx' + \gamma \overline{y}'y, y\overline{x}' + y'x)) = (\overline{x}'\overline{x} + \gamma \overline{y}y', -y\overline{x} - y'x)
= (\overline{x}', -y')(\overline{x}, -y) = t((x', y'))t((x, y))
$$
因此 $t$ 是一个反自同构。

仍有待证明(iii)。由于 E 与 F 的子代数相同，因此可以假设 E 是结合的。令 $u = (x, y)$, $u' = (x', y')$, $u'' = (x'', y'')$ 为 F 的元素，则
$$
\begin{cases}
(uu')u'' = ((xx' + \gamma \overline{y}'y)x'' + \gamma \overline{y}''(\overline{y}x' + y'x), \\
\phantom{(uu')u'' = } (y\overline{x}' + y'x)\overline{x}'' + y''(xx' + \gamma \overline{y}'y)) \\
u(u'u'') = (x(x'x'' + \gamma \overline{y}''y') + (\gamma(x''\overline{y}' + \overline{x}'\overline{y}'')y, \\
\phantom{u(u'u'') = } y(\overline{x}''\overline{x}' + \gamma \overline{y}'y'') + (y'\overline{x}'' + y''x')x).
\end{cases}
$$
(27)

检查这些公式表明，E的交换律意味着F的结合性。相反，如果F是结合律，公式(27)与$y = y' = 0$、$x'' = 0$和$y'' = e$应用的，得到$(0, x'x) = (0, xx')$，即$x'x = xx'$对于 E 中的所有 $x, x'$；因此 E 是可交换的。

注另外，在上面的记号中，对于E中的$x, y$，
$$
yj = j\overline{y}, \quad x(yj) = (yx)j, \quad (xj)y = (x\overline{y})j, \quad (xj)(yj) = \overline{y}xe
$$
(28)
$$
j^2 = e.
$$
(29)

Cayley 代数 $(\mathbf{F}, t)$ 被称为* $(\mathbf{E}, s)$ *定义的 *Cayley 扩张 *由* $\gamma$ 定义。

#### 例 {#alg-iii-s2-n5-exa-1 .statement tag=05Z3}

(1) 如果我们取$\mathbf{E} = \mathbf{A}$（因此$s = 1_A$），则代数$\mathbf{F}$是一个*二次A-代数*，其中基$(e, j)$，其中$j^2 = \gamma e$。

(2) 取E为型* $(\alpha, \beta)$的*二次代数，使得E的底层模为$\mathbf{A}^2$，乘法表 (2) (no. 3)为典范基。取 s 为 E (no. 3, 命题 2) 的共轭。那么，对于所有$\gamma \in \mathbf{A}$，由$\gamma$定义的$(\mathbf{E}, s)$的Cayley 扩张 F称为型* $(\alpha, \beta, \gamma)$的*四元数代数，它与no. 3、命题 1和命题*结合* 5以上；它的底层模是$\mathbf{A}^4$，如果$(e, i, j, k)$表示$\mathbf{A}^4$的典范基，则相应的乘法表由下式给出
$$
\left\{\begin{array}{lll}
i^2 = \alpha e + \beta i, & ij = k, & ik = \alpha j + \beta k, \\
ji = \beta j - k, & j^2 = \gamma e, & jk = \beta \gamma e - \gamma i, \\
ki = -\alpha j, & kj = \gamma i, & k^2 = -\alpha \gamma e.
\end{array}\right.
$$
(30)

此外，对于$u = \rho e + \xi i + \eta j + \zeta k$（$\mathbf{A}$中有$\rho, \xi, \eta, \zeta$），我们有（用$\bar{u}$代替$t(u)$，并用$\mathbf{Ae}$识别$\mathbf{A}$）：

$$
\left\{
\begin{array}{l}
u = (\rho + \beta \xi)e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho + \beta \xi \\
N_F(u) = \rho^2 + \beta \rho \xi - \alpha \xi^2 - \gamma (\eta^2 + \beta \eta \zeta - \alpha \zeta^2).
\end{array}
\right.
$$

公式 (30) 由 (28) 和 (29) 得出，公式 (31) 由 (23) 和 (24) 得出，考虑到二次代数 E 的公式。

那么，对于 F 中的 $u, v$，

$$
N_F(uv) = N_F(u)N_F(v)
$$

对于$N_F(uv) = uv.\overline{uv} = uv(\overline{v}.\overline{u}) = u(v\overline{v})\overline{u} = (u\overline{u})(v\overline{v})$，凭借结合性以及F的$N_F(u)$属于到中心这一事实。

与四元数代数同构的A-代数也称为*四元数代数*；如果这样的代数中的基具有乘法表(30)，则称为型*$(\alpha, \beta, \gamma)$的*基。通过滥用语言，当基为型 $(\alpha, \beta, \gamma)$ 时，四元数代数被称为*型* $(\alpha, \beta, \gamma)$。

当 $\beta = 0$、公式 (30) 和 (31) 简化为

$$
\left\{
\begin{array}{lll}
i^2 = \alpha e, & ij = k, & ik = \alpha j, \\
ji = -k, & j^2 = \gamma e, & jk = -\gamma i, \\
ki = -\alpha i, & kj = \gamma i, & k^2 = -\alpha \gamma e,
\end{array}
\right.
$$

和

$$
\left\{
\begin{array}{l}
\bar{u} = \rho e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho \\
N_F(u) = \rho^2 - \alpha \xi^2 - \gamma \eta^2 + \alpha \gamma \zeta^2.
\end{array}
\right.
$$

然后在上面的表达式中$(\alpha, \beta, \gamma)$就被$(\alpha, \gamma)$替换了。 It is immediate that the quaternion algebras of types $(\alpha, \gamma)$ and $(\gamma, \alpha)$ are *isomorphic*.

注公式 (32) 证明当$-1 \neq 1$在$\mathbf{A}$中时F不可交换。

*取A为实数和$\alpha = \gamma = -1, \beta = 0$的域$\mathbf{R}$，相应的代数F称为哈密顿四元数*的*代数，记为$\mathbf{H}$。如果$u = \rho e + \xi i + \eta j + \zeta k$（$\mathbf{R}$中的$\rho, \xi, \eta, \zeta$）是$\mathbf{H}$中的元素$\neq 0$，则公式$u\bar{u} = \bar{u}u = \rho^2 + \xi^2 + \eta^2 + \zeta^2$（cf.（34））表明$\mathbf{R}$中的$N(u) \neq 0$，因此$u$ 承认 $\mathbf{H}$ 中有一个*逆* $u^{-1} = N(u)^{-1}\bar{u}$，因此 $\mathbf{H}$ 是一个*非交换域*。

(3) 如果E取为四元数代数 (cf. *例 2*)，则由元素 $\delta \in \mathbf{A}$定义的E的凯莱扩张一般是非关联的

（命题5）；它被称为 A 上的八元数代数 (cf. 附录, no. 3)。

### 6. 岩浆的代数，幺半群，群

回想一下，岩浆是集合和律合成 (I, § 1, no. 1)。设 S 为乘法写成的岩浆，设 E = A^{(S)} 为 S 的元素形式线性组合的 A-模 (II, § 1, no. 11)；我们知道典范映射 s \mapsto e_s 被定义为 S 到 A^{(S)} 中，这样族 (e_s)_{s \in S} 是 A^{(S)} 的基 （称为规范），然后 A^{(S)} 的每个元素被唯一地写在形式 $\sum_{s \in S} \alpha_s e_s$ 中，其中(\alpha_s) 是有限支撑 A 的元素族。那么 A-代数结构在 E 上定义为典范基的乘法表

$$
e_s e_t = e_{st}.
$$

这样定义的代数 E 称为 A 上的岩浆 S 的代数。如果 $x = \sum_{s \in S} \xi_s e_s$ 和 $y = \sum_{s \in S} \eta_s e_s$ 是 E 的两个元素，则

$$
xy = \sum_{s \in S} \left( \sum_{tu = s} \xi_t \eta_u \right) e_s.
$$

当 S 是幺半群（分别为群）时，E 称为幺半群（分别为群）S 在 A 上的代数；那么它是一个结合律代数 (§ 1, no. 7)；类似地，当S是交换幺半群时，它的代数是结合律和交换律的。最后如果岩浆S承认单位元素u，$e_u$就是代数E的单位元；由于元素 $e_u$ 是自由的，因此 A 可以用 E 的子代数 Ae_u 来标识。

当 A \neq \{0\} 时，S 被有时识别为单射 s \mapsto e_s 下的像，因此 E 的元素写为 $\sum_{s \in S} \alpha_s s$；但当 S 被附加地写入时，这种识别是不可能的（不会引起混乱）。那么也经常写$e^s$来代替$e_s$。

设B为另一个交换环和$\rho : A \to B$环同态；考虑 A 和 B 上相同岩浆 S 的代数 E = A^{(S)} 和 E' = B^{(S)}，并令 $(e_s)_{s \in S}$ 和 $(e'_s)_{s \in S}$ 分别为它们各自的规范基。 代数 B^{(S)} 在 A-线性映射 j 下被规范地识别，使得 $j(e_s \otimes 1) = e'_s$ 对于所有 $s \in S$，其中代数 A^{(S)} \otimes_A B 通过将标量的环扩展到 B 而从 A^{(S)} 获得（II, § 1, no. 11，推论3 至命题 17)。

#### 命题 6 {#alg-iii-s2-prop-6 .statement tag=05Z4}

*令 S 为岩浆，F A-代数和 f 同态 *

S 转化为 F，仅具有乘法结构。那么存在且仅有一个 A-代数同态 $\bar{f}: A^{(S)} \to F$ 渲染交换图表

$$
\begin{array}{ccc}
S & \xrightarrow{f} & F \\
| & & | \\
A^{(S)} & \xrightarrow{\bar{f}} & F
\end{array}
$$

（其中左侧的垂直箭头是典范映射 $s \mapsto e_s$）。

设$\bar{f}: A^{(S)} \to F$是唯一的A-模同态，使得$\bar{f}(e_s) = \bar{f}(s)$（II, § 1, no. 11，推论3到命题17）；只需验证$\bar{f}$是代数同态，为此，只需证明$\bar{f}(e_s e_t) = \bar{f}(e_s) \bar{f}(e_t)$，它紧随定义和假设$f(st) = f(s)f(t)$。

命题 6 表示$A^{(S)}$和典范映射$s \mapsto e_s$的有序对由……组成是普遍映射问题的解（集合理论，IV, § 3, no. 1），其中$\Sigma$是A-代数结构的类以及 S 的 $\alpha$ 映射同态到 A-代数的乘法律。

#### 推论{#alg-iii-s2-n6-cor-1 .statement tag=05Z5}

令S、S'为两块岩浆且$g: S \to S'$同态。那么存在且仅有一个 A-代数同态 $u: A^{(S)} \to A^{(S')}$ 渲染交换图表

$$
\begin{array}{ccc}
S & \xrightarrow{g} & S' \\
| & & | \\
A^{(S)} & \xrightarrow{u} & A^{(S')}
\end{array}
$$

（其中垂直箭头是典范映射）。

应用命题 6 取$f$作为复合映射$S \xrightarrow{g} S' \to A^{(S')}$就足够了。

特别是，如果 T 是岩浆 S (I, § 1, no. 4) 的稳定子集，则$A^{(S)}$的元素$\sum_{s \in T} \alpha_s e_s$的集合是$A^{(S)}$的子代数，与代数$A^{(T)}$自然同构，并且有时等同于后者。

#### 例 {#alg-iii-s2-n6-exa-1 .statement tag=05Z6}

设 V 为A-模，S 为对左侧 V 进行运算的幺半群；这意味着 (I, § 5, no. 1) 给定 S 的映射 $(s, x) \mapsto s.x$ 到 V 中，使得 S 中的 $s, t$ 具有$s.(x + y) = s.x + s.y, s.(\alpha x) = \alpha(s.x)$ 和 $s.(t.x) = (st).x$，V 中的 $x, y$ 和$\alpha \in A$，并且用 S 的 e 单位元素表示，e.x = x 对于 x ∈ V。 f(s)(x) = s.x，f 是 S 的同态到代数 End_A(V)（仅具有其乘法律），映射单位元素 e 到单位元 l_V。得到应用命题6，A-代数同态$\bar{f}: A^{(S)} \to \mathrm{End}_A(V)$，这给出了V左模结构在$A^{(S)}$上的基础群。

这使我们能够通过约化研究群与运算符的交换模。让 M 是一个可交换的群，其运算符是加法编写的，所有外法则都是乘法编写的。令$\Omega$为M上各个外法则的算子域的和集合（集合理论，II, § 4, no. 8），这些域中的每一个都被规范地标识为$\Omega$的子集。令 Mo($\Omega$) 为在 $\Omega$ 上构造的自由幺半群 (I § 7, no. 2)； 律 / 作用

$$
(s, x) \mapsto s.x
$$

定义在 M 上，以 Mo($\Omega$) 作为算子域，通过 Mo($\Omega$) 中字 s 的长度上的归纳定义；如果 s 为长度 0，则它是空的字 e，我们为所有 $x \in M$ 写为 $e.x = x$。如果x为长度$n \geq 1$，则可以唯一地写为$s = tu$，其中u为长度$n - 1$，t为长度1，因此$t \in \Omega$；然后我们写$s.x = t.(u.x)$。对于任何两个字 s，Mo($\Omega$) 中的 $s'$，关系 $s.(s'.x) = (ss').x$ 由 s 的长度上的归纳验证。

然后如上所述的应用方法，在M上得到左$\mathbf{Z}^{(Mo(\Omega))}$模结构，并且不费力地验证了带有算子的群理论中通常的概念（稳定的子群，同态）与可交换的带有算子的群和由此关联的模是相同的和他们在一起。

### 7.免费代数

#### 定义 2 {#alg-iii-s2-def-2 .statement tag=05Z7}

*让我成为集合；设 M(I)（分别为 Mo(I)、分别为 $\mathbf{N}^{(I)}$）表示从 I 导出的自由岩浆（分别为自由幺半群、分别为自由交换幺半群）。 M(I)（分别为 Mo(I)、分别为 $\mathbf{N}^{(I)}$）在 A 上的代数称为自由代数（分别为自由结合体） 代数，分别是集合 I 超过环 A 的自由交换联想代数（或者，滥用语言，自由交换代数））。

我们将用 Lib_A(I)（分别为 Libas_A(I)、分别为 Libasc_A(I)）来表示 I 在 A 上的自由代数（分别为自由结合代数、分别为自由交换代数）。通过将 I 的典范映射组合成 M(I)（分别为 Mo(I)、分别为 $\mathbf{N}^{(I)}$）和 M(I) 的典范映射（分别为 Mo(I)、分别为 $\mathbf{N}^{(I)}$) 为 Lib_A(I)（分别为 Libas_A(I)、分别为 Libasc_A(I)）， 典范映射由 I 获得到 Lib_A(I)（分别为 Libas_A(I) 和 Libasc_A(I)），如果 $A \neq \{0\}$ 则它是单射的。我们将在典范映射下用$X_i$表示元素$i \in I$的像，并且我们将说$X_i$是Lib_A（I）（分别是Libas_A（I），分别是Libasc_A（I））的指标i的不确定。

由于 Mo(I) 和 $\mathbf{N}^{(I)}$ 各有单位元素，因此 Libas_A(I) 和 Libasc_A(I) 是单位结合律代数，并且 Libasc_A(I) 是可交换的。如果 e 是 Libas_A(I)（分别为 Libasc_A(I)）的单位元，映射 $\alpha \mapsto \alpha e$ 是 A 的同构到 Libas_A(I)（分别为 Libasc_A(I)）的中心的子环，其用 A (no. 1) 标识。

#### 命题 7 {#alg-iii-s2-prop-7 .statement tag=05Z8}

*设 I 为 A 上的集合和 F 代数（分别为单位结合律代数，分别为单位交换结合律代数）。对于每一个映射 $f : I \to F$，存在且仅有一个同态（分别为单位同态）将 Lib_A(I)（分别为 Libas_A(I)、分别为 Libasc_A(I)）的 $\bar{f}$ 转换为 F，使得 $\bar{f}(X_i) = f(i)$ 对于所有 $i \in I$。*

令 $F_m$ 为通过将集合 F 与合成相乘律获得的岩浆（或幺半群）。 M(I)（分别为 Mo(I)、分别为 $\mathbf{N}^{(I)}$）在 $F_m$ 中存在且仅有一个同态（分别为单位同态）$g$，使得 $g(i) = f(i)$ 对于所有 $i \in I$（I, § 7，编号 1、2 和 7）；然后从 no. 6、命题 6 得出命题 7。

#### 注 {#alg-iii-s2-n7-rem-1 .statement tag=05Z9}

(1) 我们稍后将 Libas_A(I) 的定义同构放到自由模 $A^{(I)}$ (§ 5, no. 5) 的张量代数上，并将 Libasc_A(I) 的同构放到 $A^{(I)}$ 的对称代数上（§ 6, no. 6）。

(2) 设 $\rho$ 为 A 到交换环 B 的单位同态。正如已经看到的 (§ 2, no. 6)，同构 $\sigma$ 是从 Lib_B(I)（分别为 Libas_B(I)、分别为 Libasc_B(I)）的 $\rho$ 导出到通过$\rho$将标量扩展到B而获得代数$(\mathrm{Lib}_A(I))_{(B)}$（分别$(\mathrm{Libas}_A(I))_{(B)}$、$(\mathrm{Libasc}_A(I))_{(B)}$）；如果$X_i^A, X_i^B$分别是A和B的指标$i$相应的的不定式，则$\sigma(X_i^B) = X_i^A \otimes 1$。

(3) 令J为I的子集；我们知道 M(J) 与岩浆 M(I) 的稳定子集一致，因此 (no. 6) Lib_A(J) 与 Lib_A(I) 的子代数一致，由 $X_i$ 生成，使得 $i \in J$；据说 Lib_A(J) 的元素中仅出现指标属于到 J 的不定式。岩浆的代数的no. 6给出的定义表明，当J穿过I的*有限*子集的集合时，Lib_A(I)是子代数Lib_A(J)有向族的并。对于Libas_A(I)也有类似的结果和 Libasc_A(I)。

(4) 与 M(I)（分别为 Mo(I)、分别为 $\mathbf{N}^{(I)}$）的元素 s 关联其 *长度* $l(s)$，即整数 $\geqslant 1$（分别为 $\geqslant 0$），使得 $l(ss') = l(s) + l(s')$ (I, § 7， 1、2 和 7 号）。如果 $e_s$ 是 Lib_A(I)（分别为 Libas_A(I)、分别为 Libasc_A(I)）相应的到 s 的元素，则 *总计次数* （或简单地为元素 $x = \sum_s \alpha_s e_s \neq 0$ 的 *次数*当 s 穿过元素的（假设非空）集合使得 $\alpha_s \neq 0$ 时，Lib_A(I)（分别为 Libas_A(A) 和 Libasc_A(I)）为数 $l(s)$ 的最大的。 例，如果$i, j, k$是I的三个不同的元素，则元素$(X_i(X_jX_k))X_i - (X_iX_j)(X_kX_i)$是Lib_A(I)中总共次数4的元素$\neq 0$。

### 8. 生成元和关系的代数的定义

设F是A上的代数，并且$(x_i)_{i \in I}$是F的元素族。通过no. 7，命题7，存在唯一同态$f : \mathrm{Lib}_A(I) \to F$，使得$f(X_i) = x_i$对于所有$i \in I$。为了使$f$是满射，$(x_i)_{i \in I}$是F的生成的系统是充分必要的。

如果$U \in \mathrm{Lib}_A(I)$，则$f(U)$被称为从U导出的F的*元素，通过用元素$x_i$代替不定数$X_i$*，或者也称为U的*值*代替不定数的值$x_i$ $X_i$；通常用$U((x_i)_{i \in I})$表示；特别是$U((X_i)_{i \in I}) = U$。如果$\lambda$是F的同态到A上的代数$F'$，那么
$$
\lambda(U((x_i)_{i \in I})) = U((\lambda(x_i))_{i \in I}).
$$

特别考虑$F = \mathrm{Lib}_A(J)$的情况，其中J是另一个集合；对于$\mathrm{Lib}_A(J)$元素每个家庭$(H_i)_{i \in I}$和A-代数$F'$每个元素家庭$(y_j')_{j \in J}$，
$$
U((H_i)_{i \in I}))((y_j')_{j \in J}) = U((H_i((y_j')_{j \in J})))_{i \in I}).
$$
(37)

在上面的记号中，$\mathrm{Lib}_A(I)$的每个元素U，使得$U((x_i)_{i \in I}) = 0$，或者也使得$f(U) = 0$，被称为F中族$(x_i)_{i \in I}$的*关系子*。这些元素的双面理想$\mathrm{Ker}(f)$由……组成被称为*理想$(x_i)$ 的关系者*。

设$(R_j)_{j \in J}$是$\mathrm{Lib}_A(I)$的元素的家庭。如果$(x_i)_{i \in I}$是F的生成的系统，并且由$R_j$生成的$\mathrm{Lib}_A(I)$的两侧理想等于$(x_i)_{i \in I}$族关系者的理想，则$((x_i)_{i \in I}, (R_j)_{j \in J})$被称为代数F的*表示*； $x_i$ 称为*生成元*，$R_j$ 称为演示文稿的*相关者*。

现在考虑任何集合我和$\mathrm{Lib}_A(I)$的元素家庭$(R_j)_{j \in J}$。 $(R_j)$族生成的双边理想所得到的$\mathrm{Lib}_A(I)$的商代数E被称为由关系族*$(R_j)_{j \in J}$与生成的系统I定义的*通用代数。显然，如果$\overline{X}_i$表示E中$X_i$的像，
$$
((\overline{X}_i)_{i \in I}, (R_j)_{j \in J})
$$
此外，如果$(x_i)_{i \in I}$是代数F和$R_j((x_i)_{i \in I}) = 0$的元素族，对于所有$j \in J$，存在唯一同态$g : E \to F$，使得$g(\overline{X}_i) = x_i$对于所有$i \in I$；对于 $((x_i)_{i \in I}, (R_j)_{j \in J})$ 是 F 的表示，$g$ 是*双射的*是必要且充分的。

这些注证明了以下滥用语言的合理性：而不是说“*$((x_i)_{i \in I}, (R_j)_{j \in J})$是F*的表示”，还说“*F是由生成元$x_i$生成的代数受制于关系$R_j((x_i)_{i \in I}) = 0$*”。当$R_j$为形式$P_j - Q_j$时，也称“*F是由$x_i$服从关系$P_j((x_i)) = Q_j((x_i))$*生成的代数”。

设H为集合；我们可以说，$\mathrm{Lib}_A(H)$的元素 S是A-代数的*通用*关系器，对于F的元素的*每个*系列$(x_h)_{h \in H}$，A-代数F是$S((x_h)_{h \in H}) = 0$，其中H作为索引集合。

#### 例 {#alg-iii-s2-n8-exa-1 .statement tag=05ZA}

(1) 取$H = \{1, 2, 3\}$； 代数承认
$$
(X_1 X_2) X_3 - X_1 (X_2 X_3)
$$
作为通用关系词的是联想词代数。承认$X_1 X_2 - X_2 X_1$为通用关系子的代数是交换代数。 *代数承认通用关系子 $X_1 X_1$ 和
$$
(X_1 X_2) X_3 + (X_2 X_3) X_1 + (X_3 X_1) X_2
$$
因为通用关系器是李代数.*

让我集合；给定 Lib_A(H) 的元素的族 $(S_k)_{k \in K}$，并考虑形式 $S_k((U_h))_{h \in H}$ 的 Lib_A(I) 的元素的集合 T，其中 k 穿过 K，对于每个 k，$(U_h)_{h \in H}$ 穿过 的族的集合 Lib_A(I)的元素，以H为索引集合；考虑一个家庭 $(R_j)_{j \in J}$，其中 T 为集合或元素。然后设 F 为生成的系统 I 与$(R_j)_{j \in J}$相关的全称代数，并令$u : \mathrm{Lib}_A(I) \to F$为典范同态，这样对于所有$k \in K$和所有$(U_h)_{h \in H}$族，Ker(u)由元素$S_k((U_h)_{h \in H})$生成Lib_A(I) 的元素；显然，每个$S_k$（$k \in K$）都是F的*通用关系器*。现在让F'为代数，承认生成的系统$(x_i)_{i \in I}$，其中每个$S_k$都是一个通用关系器，并让$u' : \mathrm{Lib}_A(I) \to F'$为同态使得$u'(X_i) = x_i$对于所有$i \in I$；显然 Ker(u) $\subset$ Ker(u') ，因此 $u'$ 可以唯一地写成形式 $u' = h \circ u$，其中 $h : F \to F'$ 是同态，使得$h(\overline{X}_i) = x_i$ 对于所有$i \in I$。因此，F 被称为*通用代数，由生成的系统 I*、*相应的定义为通用关系器家族* $(S_k)_{k \in K}$。通过滥用语言，F 被有时称为由 I 生成的通用代数，并且服从于 F 的元素的每个家庭 $(u_h)_{h \in H}$ 的*身份* $S_k((u_h)) = 0$。

*例* 2. 令L'为由I生成的全称代数，并服从L'的每一个三族元素的恒等式$(uv)w - u(vw) = 0$，并令L''为通过与L'邻接单位元获得的代数；那么 Libas_A(I) 上存在一个唯一的 L'' 同构 g ，使得对于所有 $i \in I$ 都有$g(\overline{X}_i) = X_i$。因为显然 L'' 是结合律，并且同态 g 的存在源自 L' 的定义和其前面的注；但显然 L'' 满足泛性质 (no. 7, 命题 7)，这表征了 Libas_A(I)，从而的结论。

与上述类似的考虑可以应用于结合律代数（分别是交换结合律代数），同时考虑以下注。当上下文充分表明代数被认为是统一的代数时，通过滥用语言，元素$(x_i)_{i \in I}$的代数$F$的家族，使得子代数由$x_i$（$i \in I$）生成，并且单位元等于$F$，常称为$F$的生成的系统。然后令$F$是$A$上的统一结合律代数，并令$(x_i)_{i \in I}$是元素和$F$的族；由于no. 7、命题 7，存在唯一的单位同态$f : \mathrm{Libas}_A(I) \to F$，使得$f(X_i) = x_i$对于所有$i \in I$；如果$U \in \mathrm{Libas}_A(I)$，$f(U)$也称为$F$的元素，由$U$派生，用元素$x_i$代替不定式$X_i$，也用$U((x_i)_{i \in I})$表示。然后关系器、表示和通用关系器的概念立即转到联想代数；只需替换 $\mathrm{Lib}_A(I)$ 即可完成 $\mathrm{Libas}_A(I)$。 *通用单位结合律代数由生成的系统定义，由关系族相关*$(R_j)_{j \in J}$是由族$(R_j)$生成的双边理想对$\mathrm{Libas}_A(I)$的商代数。由生成的系统 $I$、相应的生成的全称单位结合律代数也有类似的定义。我们留给读者的任务是陈述相对于交换结合律代数的类似定义，并用$\mathrm{Libasc}_A(I)$替代$\mathrm{Libas}_A(I)$。

#### 例 3 {#alg-iii-s2-n8-exa-3 .statement tag=05ZB}

令 $L'$ 为由 $I$ 生成的通用单位结合律代数，并服从于 $L'$ 的两个元素的每个家庭的恒等式 $uv - vu = 0$。可以看出，如*例 2* 所示，$L'$ 与$\mathrm{Libasc}_A(I)$ 是规范同构的。

### 9. 多项式代数

令 $B$ 为单位*交换*结合律 $A$ 代数，并令 $(x_i)_{i \in I}$ 为 $B$ 的元素族；由$x_i$（$i \in I$）和单位元生成的$B$的子代数用$A[(x_i)_{i \in I}]_B$表示，或者在不会引起混淆的情况下简单地用$A[(x_i)_{i \in I}]$表示。因此，对于每个集合$I$，代数$\mathrm{Libasc}_A(I)$等于$A[(X_i)_{i \in I}]$（也用$A[X_i]_{i \in I}$表示）；后一个记号，它的优点是表明记号被选择来表示不定，是我们在本文的其余部分中通常使用的。 $A[(X_i)_{i \in I}]$ 的元素称为*不定式中的多项式* $X_i$ ($i \in I$) *系数为* $A$；按照惯例，当说“让$A[(X_i)_{i \in I}]$是多项式代数”时，$X_i$总是被理解为不定式。对于$I$的每个子集$J$，使用上述记号相当于将$\mathrm{Libasc}_A(J)$与由指标$i \in J$的$X_i$生成的$\mathrm{Libasc}_A(I)$的代数进行识别，并且单位元（cf.no. 7，*注（3）*）。对于 $I = \{1, 2, \ldots, n\}$，我们写为 $A[X_1, X_2, \ldots, X_n]$ 而不是 $A[(X_i)_{i \in I}]$。

如果$I$和$I'$是两个等价的集合，则代数$\mathrm{Libasc}_A(I)$和$\mathrm{Libasc}_A(I')$同构。 $A[X]$ 通常用于表示多项式代数相应的到未指定的索引集合，其中*单个* 元素，$X$ 表示唯一的不定式；类似地，$A[X, Y]$、$A[X, Y, Z]$、... 用于表示未指定索引集合的多项式代数相应的，其中 2、3、... 元素。 注，根据上述约定，如果$A \neq \{0\}$，则$A[X]$和$A[Y]$适用于例（不同）子代数或$A[X, Y, Z]$。

元素
$$
X^\nu = \prod_{i \in I} X_i^{\nu(i)},
$$
其中 $\nu$ 穿过多项式代数 $A[(X_i)_{i \in I}]$ 的 $\mathbf{N}^{(I)}$ 形式基。这些元素在不定式$X_i$中称为*单项式*，数$|\nu| = \sum_{i \in I} \nu(i)$称为单项式$X^\nu$的*次数*（或*总计次数*）。 次数 0 的唯一单项式是$A[(X_i)_{i \in I}]$的单位元；它通常被识别为单位元 1 of $A$。 $A[(X_i)_{i \in I}]$ 的每个多项式 $u$ 都可以唯一地写为
$$
u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu
$$
与 $\alpha_\nu \in A$； 元素 $\alpha_\nu$、零，除了指标 $\nu \in \mathbf{N}^{(I)}$ 的有限数之外，被称为 $u$ 的*系数*； 元素$\alpha_\nu X^\nu$被称为$u$的*项*（元素$\alpha_\nu X^\nu$常被称为“$X^\nu$中的项”）；特别是项$\alpha_0 X^0$（用$\alpha_0 \in A$标识）被称为$u$的*常数项*。如果$J$是$I$的子集，$u$属于到$A[(X_i)_{i \in J}]$当且仅当$\alpha_\nu = 0$对于$\nu \notin \mathbf{N}^{(J)}$。由此可见，$A[(X_i)_{i \in I}]$是子代数$A[(X_i)_{i \in J}]$的并，其中$J$贯穿$I$的有限子集的集合。如果 $\alpha_\nu = 0$ 对应 $|\nu| > n$，则 $u$ 被认为是 *次数* $\leq n$ 的多项式。当$\alpha_\nu = 0$时，（通过滥用语言）$u$据说是*包含，在*$X^\nu$中没有项；特别是，当 $\alpha_0 = 0$ 时，$u$ 被称为多项式*，没有常数项*。

对于每个*非零*多项式$u = \sum \alpha_\nu X^\nu$，$u$的*次数*（或*总计次数*）是多索引$\nu$的整数$|\nu|$的最大的，使得$\alpha_\nu \neq 0$。

令$F$为单位结合$A$代数，并令$(x_i)_{i \in I}$为$F$的元素族，它们是*成对可置换*。由 $x_i$ 和单位元生成的 $F$ 的子代数 $F'$ 是可交换的 (§ 1, no. 7)，这使得我们可以定义用 $x_i$ 代替多项式 $u \in A[(X_i)_{i \in I}]$ 中的 $X_i$（尽管$F$不一定是可交换的）：$u((x_i)_{i \in I})$是$F'$的元素，因此$F$和$h: u \to u((x_i)_{i \in I})$是$A[(X_i)_{i \in I}]$到$F$的同态。 $h$的核的元素是$A[(X_i)_{i \in I}]$族$(x_i)$的关系因子，也称为$x_i$之间的*多项式关系因子*（系数在$A$）。 同态 $h$ 的像是子代数 $F'$，也用 $A[(x_i)_{i \in I}]$ 表示（即使$F$ 不可交换）；如果 $a$ 是 $x_i$ 之间的多项式关系器的理想，则存在正合序列个 $A$ 模
$$
0 \longrightarrow a \longrightarrow A[(X_i)_{i \in I}] \xrightarrow{h} A[(x_i)_{i \in I}] \longrightarrow 0.
$$

#### 命题 8 {#alg-iii-s2-prop-8 .statement tag=05ZC}

*令$A[(X_i)_{i \in I}]$为$I$的多项式代数、$J$子集以及$K$$I$中$J$的补集。写$A' = A[(X_j)_{j \in J}]$并用$X'_k$ ($k \in K$)表示多项式代数 Libasc_{A'}(K) = A'[(X'_k)_{k \in K}]中的*不定式，则存在A'[(X'_k)_{k \in]唯一的环同构 K}] 到 A[(X_i)_{i \in I}] 上，其中重合具有 A' 上的恒等式，并且映射 X'_k 到 X_k 对于所有 k \in K。

显然，A[(X_i)_{i \in I}] 是由 X_k 对于 k \in K 生成的 A' 代数。另一方面，作为 X_k (k \in K) 与 A' 中系数之间的多项式关系器，可以唯一地写为 $\sum_v h_v((X_j)_{j \in J}) X^v$，其中 v 穿过 $\mathbf{N}^{(K)}$ 的有限子集，并且 h_v 是元素 A[(X_j)_{j \in J}]，h_v 必须是 X_j 与 A 中的系数之间的多项式关系器，因此都是零，从而证明命题。

命题 8 中描述的同构通常用于 A[(X_i)_{i \in I}] 的认同元素，其中多项式的系数为 A' = A[(X_j)_{j \in J}]。如果 u 是 A[(X_i)_{i \in I}] 的元素 $\neq 0$，则其总次数视为 A'[(X_k)_{k \in K}] 的元素，相对于指标 i \in K 的 X_i 也称为其次数。

#### 注 {#alg-iii-s2-n9-rem-1 .statement tag=05ZD}

令 I 和 J 为两个集合且 (P_j)_{j \in J} 为 $\mathbf{Z}[(X_i)_{i \in I}]$ 的元素族；如果 Q 是 $\mathbf{Z}[(X_j)_{j \in J}]$ 的元素，使得 $Q((P_j)_{j \in J}) = 0$，则对于环 B 的成对可置换元素的每个族 $(b_i)_{i \in I}$，
$$
Q((P_j((b_i)_{i \in I}))_{j \in J}) = 0.
$$
关系包含形式 $Q((P_j)_{j \in J}) = 0$ 有时称为多项式恒等式。 例
$$
(X_1 + X_2)^2 - X_1^2 - X_2^2 - 2X_1X_2 = 0
$$
与
$$
Q = Y_1^2 - Y_2, \quad P_1 = X_1 + X_2, \quad P_2 = X_1^2 + X_2^2 + 2X_1X_2
$$
$$
X_1^n - X_2^n - (X_1 - X_2)(X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}) = 0
$$
与
$$
Q = Y_1 - Y_2Y_3, \quad P_1 = X_1^n - X_2^n, \quad P_2 = X_1 - X_2,
$$
$$
P_3 = X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}
$$
是多项式恒等式。

### 10. 幺半群的总计代数

A 上幺半群 S 的代数（如 A-模）乘积 $A^S$ 由……组成有限支撑族$(\alpha_s)_{s \in S}$ 子模； 乘法在此代数由关系$(\alpha_s)(\beta_s) = (\gamma_s)$定义，其中，对于所有$s \in S$，
$$
\gamma_s = \sum_{tu = s} \alpha_t \beta_u
$$

（cf.no. 6，公式（35））。 (38) 右侧的和是有意义的，因为$(\alpha_s)$ 和$(\beta_s)$ 是有限支撑的族，因此双族$(\alpha_t\beta_u)_{(t,u)\in S\times S}$ 也是如此。但是，当幺半群$S$满足以下条件时，(38)的右侧对于$A^S$的*任意*元素$(\alpha_s),\ \beta_s)$也有意义：

(D) *对于所有* $s\in S$，*仅存在一个有限的数有序对* $(t,u)$ *在* $S\times S$ *使得* $tu=s$。

假设$S$满足条件(D)；然后可以通过公式 (38) 在乘积 A-模 $A^S$ 上定义乘法律。这样在$A^S$上定义的乘法是A-双线性的，直接的；它也是*关联的*，因为对于 $A^S$ 中的 $\alpha,\beta,\gamma$，

$$
\sum_{uvw=t} \alpha_u\beta_v\gamma_w = \sum_{rw=t} \left( \left( \sum_{uv=r} \alpha_u\beta_v \right) \gamma_w \right) = \sum_{us=t} \left( \alpha_u \left( \sum_{vw=s} \beta_v\gamma_w \right) \right).
$$

乘法和 A-模结构在 $A^S$ 上，因此定义在 $A^S$ 上，是 A 上的统一*关联代数* 结构；我们可以说，集合$A^S$，加上这个结构，就是幺半群S在A上的*总代数*。

直接的，幺半群 S 在 A 上的 *代数* $A^{(S)}$（必要时也称为 S 的*受限代数*，以避免混淆）是 S 在 A 上的总代数* 的 *子代数*（当 S 有限时与后者相同）。 *通过滥用语言*，S 在 A 上的总代数中的每一个元素 $(\xi_s)_{s\in S}$ 也用与 S 的受限制代数的元素相同的记号 $\sum_{s\in S} \xi_s e_s$（甚至$\sum_{s\in S} \xi_s s$）表示；当然，这个记号对应中出现的求和符号没有代数运算，因为它一般是项$\neq 0$的*无穷大*。有了这个记号，S的总代数中的乘法也由no. 6的公式(35)给出。

如果 S 是可交换的，那么它的总代数 $A^S$ 也是可交换的。如果 T 是 S 的子幺半群，则幺半群的总代数 $A^T$ 规范地与 S 的总代数中的子代数一致。如果 $\rho : A \to B$ 是环同态，则规范化扩张$\rho^S : A^S \to B^S$是A上S的总代数到B上S的总代数的A同态，其中扩展典范同态$A^{(S)} \to B^{(S)}$。

### 11. 正式幂级数超过交换环

对于每个集合 I，加法幺半群$N^{(I)}$满足no. 10的条件 (D)；因为，如果 $s = (n_i)_{i\in I}$ 与 $n_i = 0$ 除了 I 的有限子集 H 中的指标 $i$，则关系 $s = t + u$ 与 $t = (p_i)_{i\in I}$ 和 $u = (q_i)_{i\in I}$ 等价于所有的 $p_i + q_i = n_i$ $i$；但这意味着 $i \notin H$ 为 $p_i = q_i = 0$，$p_i \leq n_i, q_i \leq n_i$ 为 $i \in H$；因此，$N^{(I)}$中有$\prod_{i\in H} (n_i + 1)$有序对$(t, u)$，使得$t + u = s$。

因此，我们可以考虑幺半群$\mathbf{N}^{(I)}$超过$A$的总代数，其中包含是该幺半群的（受限）代数$A[\mathbf{X}_i]_{i \in I}$。它是不定式$X_i \ (i \in I)$中形式幂级数的单位交换结合律代数，称为代数，系数在$A$中，并用$A[[\mathbf{X}_i]]_{i \in I}$表示；它的元素在不定式$X_i \ (i \in I)$中称为形式幂级数，系数为$A$。按照no. 10中制定的惯例，这样的元素$(\alpha_v)_{v \in \mathbf{N}^{(I)}}$也表示为$\sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v$； $\alpha_v$是形式幂级数的系数，$\alpha_v X^v$是项的系数；因此，$X_i$ 中的多项式是形式的幂级数，只有有限的数项 $\neq 0$。

显然，代数同构$A[[\mathbf{X}_i]]_{i \in I_1} \to A[[\mathbf{X}_i]]_{i \in I_2}$规范地源自每个双射$\sigma : I_1 \to I_2$，由映射正式的幂级数$\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_i^{n_i}$到正式的幂级数$\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_{\sigma(i)}^{n_i}$。

设$J$为$I$的子集； 代数 $A[[\mathbf{X}_i]]_{i \in J}$ 可以与正式幂级数 $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ 的$A[[\mathbf{X}_i]]_{i \in I}$ 由……组成的子代数进行识别，其中$\alpha_{(n_i)} = 0$ 对于每个元素 $(n_i) \in \mathbf{N}^{(I)}$ 使得$n_i \neq 0$至少一个指标 $i \in I - J$。此外，如果 $K = I - J$、$A[[\mathbf{X}_i]]_{i \in I}$ 被规范地标识为 $(A[[\mathbf{X}_j]]_{j \in J})[[\mathbf{X}_k]]_{k \in K}$，则通过将形式幂级数 $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ 与形式幂级数 $\sum_{(m_k)} \beta_{(m_k)} \cdot \prod_{k \in K} X_k^{m_k}$ 进行标识，其中
$$
\beta_{(m_k)} = \sum_{(p_j)} \gamma_{(p_j)} \cdot \prod_{j \in J} X_j^{p_j}
$$
其中$\gamma_{(p_j)} = \alpha_{(n_i)}$代表序列$(n_i)$，$n_i = p_i$代表$i \in J$，$n_i = m_i$代表$i \in K$。

给定一个正式的幂级数$u = \sum_v \alpha_v X^v$、项$\alpha_v X^v$，使得$|v| = p$在总次数$p$中的$u$中被称为项。正式的幂级数$u_p$，其总次数$p$中的项是$u$的项，而其他项是零，称为齐次部分 $u$ 共次数 $p$；当$I$有限时，$u_p$是所有$p$的多项式； $u_0$ 与$A$ 的元素相同（也称为$u$ 的常数项）。如果$u$和$v$是两个形式幂级数和$w = uv$，那么
$$
w_p = \sum_{r=0}^p u_r v_{p-r}
$$
每整数 $p \geq 0$。

对于每个正式的幂级数$u \neq 0$，最小的整数$p \geq 0$使得$u_p \neq 0$被称为$u$的总阶（或简称为阶）。如果这个阶用$\omega(u)$表示并且$u$和$v$是两个形式的幂级数$\neq 0$，那么
$$
\omega(u + v) \geq \inf(\omega(u), \omega(v)) \quad \text{if } u + v \neq 0 \\
\omega(uv) \geq \omega(u) + \omega(v) \quad \text{if } uv \neq 0.
$$

进一步，如果$\omega(u) \neq \omega(v)$，则$u + v \neq 0$必然与(40)的两侧相等。

注 0 的阶 *未定义*。 By an abuse of language, it is a convention to say that "f is a formal power series of order $\geq p$ (resp. $> p$)" if the homogeneous part of f of degree n is zero for all $n < p$ (resp. $n \leq p$); 0 is therefore a "formal power series of order $> p$" for *every* integer $p \geq 0$.

令 J 为 I 的子集，并令 $A[[X_i]]_{i \in I}$ 与上面的 $B[[X_k]]_{k \in K}$ 相同，其中 $K = I - J$ 和 $B = A[[X_j]]_{j \in J}$； 相应的对上述定义适用于$B[[X_k]]_{k \in K}$，正式幂级数$u \in A[[X_i]]_{i \in I}$新增了定义； 项$\alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$据说是指标的$X_i$中的次数p的*$i \in K$如果$\sum_{i \in K} n_i = p$和$B[[X_k]]_{k \in K}$的正式幂级数与相同的项次数$p$与$u$一样，其他零*被称为指标*$i \in K$的$X_i$中次数p的齐次部分。 如果$u \neq 0$，则指标$i \in K$相对于$X_i$的*阶*$\omega_K(u)$是整数$p \geq 0$的最小的，使得$u$的齐次部分为指标$i \in K$的$X_i$中的次数$p$是$\neq 0$。 当 $\omega$ 被 $\omega_K$ 替代时，不等式 (40) 和 (41) 仍然成立。

### 习题{#alg-iii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
