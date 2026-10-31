---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 10
section_title: Inverse and direct limits
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 118-123, 179
pdf_pages: 0142-0147, 0203-0203
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE SYSTEMS OF MAGMAS
      page: 118
      pdf_page: 142
    - "no": 2
      title: INVERSE LIMITS OF ACTIONS
      page: 119
      pdf_page: 143
    - "no": 3
      title: DIRECT SYSTEMS OF MAGMAS
      page: 120
      pdf_page: 144
    - "no": 4
      title: DIRECT LIMIT OF ACTIONS
      page: 123
      pdf_page: 147
statements: 5
exercises: 2
content_sha256: 8906d8819ffcd1a676707c08b8bcc730b352302b7f09ac432e9448410cbd60e6
translated_from: content/en/alg/I/10_s10_inverse_and_direct_limits.md
translation_method: google
source_content_sha256: 3a49dcd1591d3ccd8d3da36eb91e210dee0ffea0f51202486e0a783d55ffe2f0
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: e97ccb15c4ac6c8ad251873a057cb8cd5630523ce2ae6172f6774bc78e0f1f1a
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 10。逆与直极限

在本段中，我将表示非空预排序集合，$\alpha \leq \beta$ I 上的预排序。概念相对于索引集合 I 的集合的逆（或直接）系统在 *集合理论*、III, § 7, no. 1（或直接）系统中定义。 *集合理论*，III, § 7, no. 5，在假设下，我的方向是正确的）。

### 1. 逆系岩浆

#### 定义 1 {#alg-i-s10-def-1 .statement tag=05JH}

*岩浆的逆系相对于索引集合I是集合*$(\mathbf{E}_\alpha, f_{\alpha\beta})$的逆系*相对于I，每个*$\mathbf{E}_\alpha$*有岩浆结构和每个*$f_{\alpha\beta}$*是岩浆同态。*

令 $(\mathbf{E}_\alpha, f_{\alpha\beta})$ 为律乘法书写的岩浆的逆系。 逆极限集合$E = \lim_{\leftarrow} \mathbf{E}_\alpha$是$(x_\alpha)_{\alpha \in I}$家族的乘积岩浆$\prod_{\alpha \in I} \mathbf{E}_\alpha$由……组成的子集，使得$x_\alpha = f_{\alpha\beta}(x_\beta)$代表$\alpha \leq \beta$。如果$(x_\alpha)$和$(y_\alpha)$属于到E，那么对于$\alpha \leq \beta$，$x_\alpha = f_{\alpha\beta}(x_\beta)$和$y_\alpha = f_{\alpha\beta}(y_\beta)$，因此$x_\alpha y_\alpha = f_{\alpha\beta}(x_\beta) f_{\alpha\beta}(y_\beta) = f_{\alpha\beta}(x_\beta y_\beta)$；因此E是$\prod_{\alpha \in I} \mathbf{E}_\alpha$的次岩浆。 E 将得到由 $\prod_{\alpha \in I} \mathbf{E}_\alpha$ 引起的律；获得的岩浆称为

† 我们避免当前的术语，其中正数意味着 $> 0$。

逆极限岩浆$E_\alpha$的岩浆。它享有以下泛性质：

(a) 对于所有$\alpha \in I$，$E$到$E_\alpha$的典范映射$f_\alpha$是$E$到$E_\alpha$的岩浆同态。 $f_\alpha = f_{\alpha \beta} \circ f_\beta$ 为 $\alpha \leq \beta$。

(b) 假设给定岩浆$F$和同态$u_\alpha : F \to E_\alpha$，使得$u_\alpha = f_{\alpha \beta} \circ u_\beta$对应$\alpha \leq \beta$。存在且仅有一个同态 $u : F \to E$，使得$u_\alpha = f_\alpha \circ u$适用于所有$\alpha \in I$（即$x \mapsto u(x) = (u_\alpha(x))_{\alpha \in I}$）。

如果岩浆 $E_\alpha$ 是结合的（或可交换的），那么 $E$ 也是如此。假设每个岩浆$E_\alpha$承认单位元素$e_\alpha$并且同态$f_{\alpha \beta}$是统一的。然后$e = (e_\alpha)_{\alpha \in I}$属于到$E$为$e_\alpha = f_{\alpha \beta}(e_\beta)$为$\alpha \leq \beta$，就是岩浆$E$的单位元素；上面的记号、同态 $f_\alpha$ 是单位，如果 $u_\alpha$ 是单位，那么 $u$ 也是单位。此外，$E$的元素$x = (x_\alpha)_{\alpha \in I}$是可逆的，当且仅当$x_\alpha$中的每一个在相应的岩浆$E_\alpha$和$x^{-1} = (x_\alpha^{-1})_{\alpha \in I}$中都是可逆的；这是从公式 $f_{\alpha \beta}(x_\beta^{-1}) = f_{\alpha \beta}(x_\beta)^{-1} = x_\alpha^{-1}$ 到 $\alpha \leq \beta$ 得出的。

从这些注可以推断，如果岩浆$E_\alpha$是幺半群（分别是群）并且$f_{\alpha \beta}$是幺半群同态，那么岩浆$E$是幺半群（分别是群）。在这种情况下，我们谈论幺半群的逆系（或群）。 泛性质立即转到此案例。

留给读者去验证环$(E_\alpha, f_{\alpha \beta})$的定义逆系，并验证$E = \lim \leftarrow E_\alpha$是乘积环$\prod_{\alpha \in I} E_\alpha$的子环，称为环的逆极限环 $E_\alpha$；对于本例可以验证泛性质扩展。

令 $\mathfrak{C} = (E_\alpha, f_{\alpha \beta})$ 和 $\mathfrak{C}' = (E'_\alpha, f'_{\alpha \beta})$ 为相对于相同索引集合的两个逆系岩浆（分别为幺半群、群、环）。 $\mathfrak{C}$的同态到$\mathfrak{C}'$是映射$u_\alpha : E_\alpha \to E'_\alpha$的逆系$(u_\alpha)_{\alpha \in I}$，这样每个$u_\alpha$都是同态。在这些条件下，$\lim \leftarrow E_\alpha$到$\lim \leftarrow E'_\alpha$的映射$u = \lim \leftarrow u_\alpha$是同态（cf.集合理论，III, § 7, no. 2）。

### 2. 逆极限的作用

假设给定两个集合、$(\Omega_\alpha, \phi_{\alpha \beta})$和$(E_\alpha, f_{\alpha \beta})$相对于相同索引集合$I$的逆系。假设对于 $E_\alpha$ 上的 $\Omega_\alpha$ 的所有 $\alpha \in I$ 作用给出，使得

(1)
$$
f_{\alpha \beta}(\omega_\beta x_\beta) = \phi_{\alpha \beta}(\omega_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$
对于$\alpha \leq \beta, x_\beta \in E_\beta, \omega_\beta \in \Omega_\beta$。那么作用的家庭被认为是作用的逆系。设 $\Omega = \lim \leftarrow \Omega_\alpha$ 和 $E = \lim \leftarrow E_\alpha$；如果$x = (x_\alpha)_{\alpha \in I}$属于到$E$且$\omega = (\omega_\alpha)_{\alpha \in I}$属于到$\Omega$，则$\omega . x = (\omega_\alpha . x_\alpha)_{\alpha \in I}$属于到E (1)。因此E上的$\Omega$的作用被定义为$E_\alpha$*上的$\Omega_\alpha$的作用的*逆极限。

上述情况尤其适用于$\Omega_\alpha$是幺半群且$E_\alpha$上$\Omega_\alpha$的每个作用是运算的情况。那么这些运算中的逆极限就是E上幺半群的运算。

留给读者对群的逆系和定义逆极限进行运算符，并验证这个极限是否是群。

### 3. 直接系统岩浆

在这个没有。接下来我们假设我是*正确的方向*。

#### 定义 2 {#alg-i-s10-def-2 .statement tag=05JI}

*岩浆的直接系统相对于索引集合I是集合*$(E_\alpha, f_{\beta\alpha})$的直接系统*相对于I，每个*$E_\alpha$*有岩浆结构和每个*$f_{\beta\alpha}$*是岩浆同态。*

令$(E_\alpha, f_{\beta\alpha})$为岩浆的直接系统。 E 将把 $E_\alpha$ 的直极限集合 $\lim_{\longrightarrow} E_\alpha$ 和 $f_\alpha$ 典范映射表示为 E。回想一下

(2)
$$
f_\beta \circ f_{\beta\alpha} = f_\alpha \quad \text{for } \alpha \leq \beta,
$$

(3)
$$
E = \bigcup_{\alpha \in I} f_\alpha(E_\alpha).
$$

由(2) 也可得

(4)
$$
f_\alpha(E_\alpha) \subset f_\beta(E_\beta) \quad \text{for } \alpha \leq \beta.
$$

如果$x_\alpha, y_\alpha \in E_\alpha$使得$f_\alpha(x_\alpha) = f_\alpha(y_\alpha)$，则存在$\beta \geq \alpha$使得$f_{\beta\alpha}(x_\alpha) = f_{\beta\alpha}(y_\alpha)$。

#### 命题 1 {#alg-i-s10-prop-1 .statement tag=05JJ}

*E 上存在一种且仅有一种岩浆结构，其中映射* $f_\alpha : E_\alpha \to E$ *为同态。如果岩浆* $E_\alpha$ * 是结合的（或可交换的），那么 E 也是结合的。如果岩浆* $E_\alpha$ * 和同态* $f_{\beta\alpha}$ * 是单位的，那么岩浆* E * 和同态* $f_\alpha$ 也是单位的。

岩浆$E_\alpha$将被乘法写入。

设$x, y$在E中。I中存在$\alpha$，$E_\alpha$中存在$x_\alpha, y_\alpha$，使得$x = f_\alpha(x_\alpha)$和$y = f_\alpha(y_\alpha)$。如果E上存在岩浆结构，其$f_\alpha$为同态，则$x.y = f_\alpha(x_\alpha y_\alpha)$、从而是该岩浆结构的*唯一性*。

为了证明存在性，我们必须证明对于I中的$\alpha, \beta$，$E_\alpha$中的$x_\alpha, y_\alpha$和$E_\beta$中的$x'_\beta, y'_\beta$，关系

(5)
$$
f_\alpha(x_\alpha) = f_\beta(x'_\beta), \qquad f_\alpha(y_\alpha) = f_\beta(y'_\beta)
$$
暗示$f_\alpha(x_\alpha y_\alpha) = f_\beta(x'_\beta y'_\beta)$。对于$\gamma \geq \alpha$和$\gamma \geq \beta$，我们集合$x_\gamma = f_{\gamma\alpha}(x_\alpha)$，$y_\gamma = f_{\gamma \alpha}(y_\alpha), x'_\gamma = f_{\gamma \beta}(x'_\beta), y'_\gamma = f_{\gamma \beta}(y'_\beta)$。到直极限的定义，$I$和$\gamma \geq \alpha, \gamma \geq \beta, x_\gamma = x'_\gamma, y_\gamma = y'_\gamma$中存在$\gamma$。然后
$$
f_\alpha(x_\alpha y_\alpha) = f_\gamma(f_{\gamma \alpha}(x_\alpha y_\alpha)) = f_\gamma(x_\gamma y_\gamma) = f_\gamma(x'_\gamma y'_\gamma) = f_\gamma(f_{\gamma \beta}(x'_\beta y'_\beta)) \\
= f_\beta(x'_\beta y'_\beta).
$$
假设岩浆 $E_\alpha$ 是结合的。让$x, y, z$在$E$中。 $E_\alpha$中存在$\alpha \in I$和元素$x_\alpha, y_\alpha, z_\alpha$使得
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha), \quad z = f_\alpha(z_\alpha).
$$
然后$xy = f_\alpha(x_\alpha y_\alpha)$、从而$(xy)z = f_\alpha((x_\alpha y_\alpha)z_\alpha)$；同样地
$$
x(yz) = f_\alpha(x_\alpha(y_\alpha z_\alpha)),
$$
从而 $(xy)z = x(yz)$ $(x_\alpha y_\alpha)z_\alpha = x_\alpha(y_\alpha z_\alpha)$。交换岩浆的情况也可以类似地处理。

最后假设每个岩浆$E_\alpha$都有单位元素$e_\alpha$，而$f_{\beta \alpha}(e_\alpha) = e_\beta$对应$\alpha \leq \beta$。对于$I$中的$\alpha, \beta$，$I$中存在$\gamma$以及$\gamma \geq \alpha$和$\gamma \geq \beta$、从而
$$
f_\alpha(e_\alpha) = f_\gamma(f_{\gamma \alpha}(e_\alpha)) = f_\gamma(e_\gamma) = f_\gamma(f_{\gamma \beta}(e_\beta)) = f_\beta(e_\beta)
$$
因此，$E$中存在元素$e$，使得$f_\alpha(e_\alpha) = e$对于所有$\alpha \in I$。设$x$在$E$中； 选择$\alpha \in I$和$x_\alpha \in E_\alpha$使得$x = f_\alpha(x_\alpha)$。然后
$$
ex = f_\alpha(e_\alpha) \cdot f_\alpha(x_\alpha) = f_\alpha(e_\alpha \cdot x_\alpha) = f_\alpha(x_\alpha) = x
$$
类似地，$x \cdot e = x$，因此$e$是$E$的单位元素。

岩浆$E$称为岩浆*$E_\alpha$的*直极限。

#### 命题 2 {#alg-i-s10-prop-2 .statement tag=05JK}

*设* $(E_\alpha, f_{\beta \alpha})$ *为岩浆的直接系统，并让* $E$ *为其直极限* $f_\alpha : E_\alpha \to E$ *典范同态。假设给定岩浆*$F$*和同态*$u_\alpha : E_\alpha \to F$*使得*$u_\alpha = u_\beta \circ f_{\beta \alpha}$*对于*$\alpha \leq \beta$。 *存在且仅有一个同态* $u : E \to F$ *使得* $u_\alpha = u \circ f_\alpha$ *对于所有* $\alpha \in I$。 *如果岩浆* $E_\alpha$ *和* $F$ *和同态* $f_{\beta \alpha}$ *和* $u_\alpha$ *是单一的，同态* $u$ *是单一的。*

我们知道（*集合理论*，III, § 7, no. 6，命题6）存在且仅有一个映射$u : E \to F$，使得$u_\alpha = u \circ f_\alpha$对于所有$\alpha \in I$。我们验证$u$是同态：让$x, y$在$E$中，$\alpha$在$I$中，$x_\alpha, y_\alpha$在$E_\alpha$中，使得$x = f_\alpha(x_\alpha)$和$y = f_\alpha(y_\alpha)$。然后$xy = f_\alpha(x_\alpha y_\alpha)$，从而
$$
u(xy) = u(f_\alpha(x_\alpha y_\alpha)) = u_\alpha(x_\alpha y_\alpha) = u_\alpha(x_\alpha)u_\alpha(y_\alpha) \\
= u(f_\alpha(u_\alpha))u(f_\alpha(y_\alpha)) = u(x)u(y).
$$
现在我们考虑单位情况，令$e_\alpha$表示$E_\alpha$的单位元素，$e$表示$E$，$e'$表示$F$。 选择$\alpha \in I$，然后$e = f_\alpha(e_\alpha)$，从而
$$
u(e) = u(f_\alpha(e_\alpha)) = u_\alpha(e_\alpha) = e'
$$
因为 $u_\alpha$ 是单位的。因此 $u$ 是单位的。

类比岩浆的概念或直接系统，可以公式化幺半群的直接系统或群。 命题 1 表明幺半群$(E_\alpha, f_{\beta\alpha})_{\alpha, \beta \in I}$ 的直接系统中的极限岩浆E 是幺半群。我们证明，如果 $E_\alpha$ 是群，则 E 是群：令 $x \in E, \alpha \in I$ 和 $x_\alpha \in E_\alpha$ 使得 $x = f_\alpha(x_\alpha)$； E 的元素 $y = f_\alpha(x_\alpha^{-1})$ 是 x (§ 2, no. 3) 的倒数。当直接系统是幺半群或群时，命题2的泛性质立即结束。

留给读者的是环的定义直接系统。令$(A_\alpha, f_{\beta\alpha})$为直接系统；让$A = \lim \overrightarrow{A_\alpha}$和$f_\alpha : A_\alpha \to A$典范同态。 A 上存在（命题 2），并且只有一个加法和乘法，其特征在于$A_\alpha$和$x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$中的$\alpha \in I, x_\alpha, y_\alpha$具有$x + y = f_\alpha(x_\alpha + y_\alpha), xy = f_\alpha(x_\alpha y_\alpha)$。在加法下，A是可交换的群，而乘法是结合律和单位的。最后，对于 A 中的 $x, y, z$、I 中的选择 $\alpha$ 以及 $A_\alpha$ 中的 $x_\alpha, y_\alpha$ 和 $z_\alpha$ ，
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha) \quad \text{and} \quad z = f_\alpha(z_\alpha).
$$
然后
$$
(x + y) \cdot z = f_\alpha(x_\alpha + y_\alpha)f_\alpha(z_\alpha) = f_\alpha((x_\alpha + y_\alpha)z_\alpha)
= f_\alpha(x_\alpha z_\alpha + y_\alpha z_\alpha) = f_\alpha(x_\alpha z_\alpha) + f_\alpha(y_\alpha z_\alpha) = xz + yz
$$
类似地证明关系$x(y + z) = xy + xz$。在其他字中，A具有环的结构，其特征在于，对于所有$\alpha \in I$，$f_\alpha$是环同态。

环 A 称为环 $A_\alpha$ 的直极限。 命题 2 扩展立即到环的情况。

#### 命题 3 {#alg-i-s10-prop-3 .statement tag=05JL}

(a) *如果 $A_\alpha$ 非零，则 A 也非零。*
(b) *如果$A_\alpha$是整环，则A是整环。*
(c) *如果 $A_\alpha$ 为域，则 A 为域。*

设$0_\alpha, 1_\alpha$为$A_\alpha$的零和单位以及A的0、1零和单位。存在$\alpha \in I$使得$f_\alpha(0_\alpha) = 0, f_\alpha(1_\alpha) = 1$。如果$0 = 1$，则存在$\beta \geq \alpha$使得$f_{\beta\alpha}(0_\alpha) = f_{\beta\alpha}(1_\alpha)$，即$0_\beta = 1_\beta$。这就证明了(a)。

假设$A_\alpha$是整环。那么 A 通过 (a) 是可交换的且非零。令 $x, y$ 为 A 的元素，使得 $xy = 0$。存在$\alpha \in I$和$x_\alpha, y_\alpha \in A_\alpha$使得$x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$。然后$f_\alpha(x_\alpha y_\alpha) = xy = 0 = f_\alpha(0_\alpha)$。因此存在$\beta \geq \alpha$使得$f_{\beta\alpha}(x_\alpha y_\alpha) = f_{\beta\alpha}(0_\alpha)$。由于$A_\beta$是整环，因此可以得出$f_{\beta\alpha}(x_\alpha) = 0_\beta$或$f_{\beta\alpha}(y_\alpha) = 0_\beta$，因此是$x = 0$或$y = 0$。这就证明了(b)。

假设$A_\alpha$是域。然后通过 (a) $A \neq \{0\}$。令$x$为A的非零元素。存在$\alpha \in I$和$x_\alpha \in A_\alpha$使得$x = f_\alpha(x_\alpha)$。那么$x_\alpha \neq 0$和$f_\alpha(x_\alpha^{-1})$就是A中$x$的逆。这就证明了(c)。

令$\mathfrak{E} = (E_\alpha, f_{\beta\alpha})$和$\mathfrak{E}' = (E'_\alpha, f'_{\beta\alpha})$为两个直接系统岩浆（分别为幺半群、群、环）。 $\mathfrak{E}$的同态到$\mathfrak{E}'$是映射$u_\alpha : E_\alpha \to E'_\alpha$的直接系统$(u_\alpha)_{\alpha \in I}$，这样每个$u_\alpha$都是同态。在这些条件下，从$E = \lim E_\alpha$到$E' = \lim E'_\alpha$的映射$u = \lim u_\alpha$是同态（cf.*集合理论*，III, § 7, no. 6）。

### 4. 直极限的作用

假设给定两个直接系统（集合$(\Omega_\alpha, \phi_{\beta \alpha})$和$(E_\alpha, f_{\beta \alpha})$）相对于相同的索引集合$I$，并且对于$E_\alpha$上的$\Omega_\alpha$的每个$\alpha \in I$作用。假设

$$
f_{\beta \alpha}(\omega_\alpha \cdot x_\alpha) = \phi_{\beta \alpha}(\omega_\alpha) \cdot f_{\beta \alpha}(x_\alpha)
$$

对于 $\alpha \leq \beta, \omega_\alpha \in \Omega_\alpha$ 和 $x_\alpha \in E_\alpha$。那么所考虑的作用家庭据说是作用*的*直接系统。容易验证，在命题2中，$E = \lim E_\alpha$上存在$\Omega = \lim \Omega_\alpha$的作用$h$，描述如下：设$\omega \in \Omega$和$x \in E$； 选择$\alpha \in I$和$\omega_\alpha \in \Omega_\alpha, x_\alpha \in E_\alpha$使得$\omega = \phi_\alpha(\omega_\alpha)$和$x = f_\alpha(x_\alpha)$（$\phi_\alpha : \Omega_\alpha \to \Omega$和$f_\alpha : E_\alpha \to E$表示典范映射）；然后$\omega \cdot x = f_\alpha(\omega_\alpha \cdot x_\alpha)$。 $E$上的$\Omega$的作用称为$E_\alpha$上的$\Omega_\alpha$的作用*的*直极限。

如果$\Omega_\alpha$是幺半群，$E_\alpha$上$\Omega_\alpha$的每个作用是运算，直极限作用是运算。

留给读者对群的直接系统和定义直极限进行算子验证，并验证这个极限是否是群进行算子。

### 习题{#alg-i-s10-exercises}

§ 10](exercises/s10/)参见[习题。
