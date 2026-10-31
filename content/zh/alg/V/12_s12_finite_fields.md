---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 12
section_title: Finite fields
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.166-A V.170
pdf_pages: 0207-0212, 0280-0284
extraction: ocr
subsections:
    - "no": 1
      title: The structure of finite fields
      page: 0
      pdf_page: 207
    - "no": 2
      title: Algebraic extensions of a finite field
      page: 94
      pdf_page: 208
    - "no": 3
      title: The Galois group of the algebraic closure of a finite field
      page: 96
      pdf_page: 210
    - "no": 4
      title: Cyclotomic polynomials over a finite field
      page: 97
      pdf_page: 211
statements: 11
exercises: 14
content_sha256: 13e544ffd4d39b7412ff075943f9fc919c032fc0ce7e92078ec21242005174a9
translated_from: content/en/alg/V/12_s12_finite_fields.md
translation_method: google
source_content_sha256: bd8e10c4a05eb5e291baa4ec9c998a38d9874d55fab72a3f4d3987c8ee8ea686
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 9073429474f15a4f07949ba8c74a9f1f9f79de79ec6972a3581412d53fe74712
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 12。 有限域

### 1. 结构 / 有限域

#### 命题 1 {#alg-v-s12-prop-1 .statement tag=06Q8}

— 令 K 为有限域，q 元素。

a) K 的特征是素数数 p，并且存在整数 f \geq 1 使得 q = p^f。

b) K 的加法群是阶 p 的 f 循环群的直和。

c) K 的乘法群是阶 q - 1 的循环。

由于 Z 无限而 K 有限，唯一的环同态 \varphi : Z \to K 不是单射的，其核是 Z 不等于 0 的素理想。因此 K 的特征是素数数并且 K 是代数超过 p 的域 \mathbf{F}_p 元素（V，p. 2）。令 f 为 K 在 \mathbf{F}_p 上的次数。如果 f 是无限的，对于 \mathbf{F}_p 上的每个整数 n \geq 0 子空间的维数 n 来说，K 包含，从而 q \geq p^n，这是荒谬的。因此 f 是有限的。因此 K 的加法群同构于 (\mathbf{F}_p)^f, 从而断言 a) 和 b)。

断言 c) 后面是引理 1 (V, p. 78)。

#### 命题 2 {#alg-v-s12-prop-2 .statement tag=06Q9}

— 令 K 为 q 元素的有限域。 域 K 是 \mathbf{F}_p[X] 的多项式 X^q - X 的分裂域，并且是该多项式所有根的集合。

1 根据章的约定，我们在这里只关心有限的交换域。事实上，每个有限域都是可交换的，正如我们将在章VIII（cf.V，p. 170，习题14）中看到的那样。

对于$K$中的每个$x \neq 0$，我们都有$x^{q-1} = 1$，因为$K^*$是阶$q-1$中的有限群（I，p. 52）。由此可见，$K$中的每个$x$都有$x^q = x$。 $\mathbf{F}_p[X]$的多项式$X^q - X$为次数$q$，并且在$K$、从而中有$q$根

$$
X^q - X = \prod_{\xi \in K} (X - \xi).
$$

由此立即得出命题2。

#### 推论{#alg-v-s12-n1-cor-1 .statement tag=06QA}

— *同一个基数的两个有限域是同构的。*

设$K'$为$q$元素中的有限域；它的特征是质数数$p'$除$q = p^f$、从而$p' = p$。因此$K'$是$\mathbf{F}_p[X]$（命题2）中多项式$X^q - X$的分裂域，因此$K$和$K'$同构（V，p. 22，Cor.）。

当 $K = \mathbf{F}_p$、公式 (1) 约化至关系

$$
X^p - X \equiv \prod_{i=0}^{p-1} (X - i) \mod p \mathbf{Z}[X]
$$

在多项式环$\mathbf{Z}[X]$。

公式 (2) 也可以写成

$$
X^{p-1} - 1 \equiv \prod_{i=1}^{p-1} (X - i) \mod p \mathbf{Z}[X]
$$

特别是对于 $X = 0$，我们得到 (« Wilson's 公式 »)

$$
(p-1)! \equiv -1 \mod p
$$

### 2. 有限域的代数扩张

#### 命题 3 {#alg-v-s12-prop-3 .statement tag=06QB}

— *令$K$为$q$元素中的有限域，$\Omega$代数闭扩张中$K$和$m$整数$\geqslant 1$。
a) 存在$\Omega$ 的唯一子扩展$K_m$，其在$K$ 上具有次数 $m$。
b) 域$K_m$有$q^m$元素以及$\Omega$的自同构$x \mapsto x^{q^m}$固定点集合。
c) 对于循环群$K_m^*$的每个生成元$\zeta$，我们有$K_m = K(\zeta)$。
令$p$为$K$和$f$次数的$K$超过$\mathbf{F}_p$的特征。我们有$q^m = p^{fm}$和映射，$x \mapsto x^{q^m}$因此是完美域$\Omega$的自同构（V，p. 7，命题4）。因此，$K[X]$的多项式$X^{q^m} - X$的根的集合$K_m$是$\Omega$的子域。由于$X^{q^m} - X$的导数等于$-1$，因此该多项式的所有根都是简单的（IV，p. 17，命题7），因此$K_m$有$q^m$元素。由此可见$[K_m : K] = m$。

现在让L是$\Omega$的子扩展，是次数$m$在$K$上的子扩展。由于向量空间超过$K$，$L$与$K^m$同构的，$q^m$元素也同构。因此，对于所有 $x \in L$（提案 2），我们有 $x^{q^m} = x$，从而 $L \subset K_m$。从$[L : K] = [K_m : K] = m$开始，我们终于有了$L = K_m$。

由此我们证明了断言 a) 和 b) 以及 c) 是微不足道的。

#### 推论{#alg-v-s12-n2-cor-1 .statement tag=06QC}

— *令$K$为有限域且$\Omega$代数闭扩张为$K$。 $\Omega$中$K$的相对代数闭包$\overline{K}$由()和单位元的根组成，是$K$的代数闭包。*

我们知道$K$是$K$的代数闭包（V，p. 22，例2），并且很明显，$\Omega$属于到$K$中单位元的每个根。此外，给定$\overline{K}$中的$x \neq 0$，次数$m$超过$K$，如果$K$有$q$元素，则域$K(x)$有$q^m$，从而 $x^{q^m - 1} = 1$，因此 $x$ 是 $\Omega$ 中单位元的根。

令$p$为素数数，令$\mathbf{F}_p = \mathbf{Z}/p\mathbf{Z}$为$p$元素的域。我们$\mathbf{F}_p$的选择代数闭包$\Omega$，其存在源于斯坦尼茨的定理（V，p. 23，Th.2）。令 $f$ 为正整数和 $q = p^f$。根据命题 3，存在唯一的子域 $\Omega$，其次数 $f$ 超过 $\mathbf{F}_p$；我们将用$\mathbf{F}_q(\Omega)$或滥用记号$\mathbf{F}_q$来表示它。它是 $\Omega$ 的独特子扩展，其中次数 $f$ 超过 $\mathbf{F}_p$。它是基数$q$的$\Omega$的唯一子域，并且基数$q$的每个域与$\mathbf{F}_q$同构的（不规范）（第2条的Cor.）。我们注，$\mathbf{F}_q$由$\Omega$中的$x$组成，其中$x^q = x$和$F, \subset \mathbf{F}_{q'}$当且仅当$q'$是$q$的幂。

#### 命题 4 {#alg-v-s12-prop-4 .statement tag=06QD}

— *令$\mathbf{K}$为$q$元素中的有限域，以及$K$中的有限次数$m$中的$\mathbf{K}_m$扩张。

a) 域$\mathbf{K}_m$是$K$的伽罗瓦扩张，其中伽罗瓦群是由自同构$\sigma_q : x \mapsto x^q$生成的阶$m$的循环群。

b) 对于$x$的每个$x \in \mathbf{K}_m$范数相对于$K$等于$x^{(q^m - 1)/(q - 1)}$。

c) $K$的每个元素都是$\mathbf{K}_m$的元素的踪迹（或范数）。*

令$\Gamma$为由$\sigma_q$生成的$\mathbf{K}_m$的自同构的循环群。 $\Gamma$的不变量域由$\mathbf{K}_m$的元素$x$组成，使得$x^q = x$等于$K$。因此$\mathbf{K}_m$是$K$的伽罗瓦扩张和伽罗瓦群$\Gamma$，后者的阶等于$[K_m : K] = m$（V，p. 66，Th.3）。因此a)如下。

我们有$\Gamma = \{1, \sigma_q, \sigma_q^2, \ldots, \sigma_q^{m-1}\}$； 范数元素 $x$ $\mathbf{K}_m$ 相对于 $K$ 因此是 $N(x) = \prod_{i=0}^{m-1} \sigma_q^i(x) = x^{1 + q + \cdots + q^{m-1}}$ 并且我们有 $1 + q + \cdots + q^{m-1} = \frac{q^m - 1}{q - 1}$。这证明了b)。设$\xi$为循环群$\mathbf{K}_m^*$的生成元； 范数$N : \mathbf{K}_m^* \to K^*$的像是元素$\xi = N(\xi) = \xi^{(q^m - 1)/(q - 1)}$生成的子群对$K^*$的循环；因为$\xi$是阶$q^m - 1$，$\xi$是阶$q - 1$，所以生成$K^*$。这证明了 K 的每个非零元素都是 K 的非零元素的范数 ；此外，我们还有$0 = N(0)$。

最后，由于 $K_m$ 是 K 的可分离代数扩张，因此迹在 K 上的向量空间 $K_m$ 上是非零线性形式（V，p. 49，Cor.）；所以K的每一个元素都是$K_m$的元素的迹。

### 3.有限域代数闭包伽罗瓦群

令$S \neq \{1\}$为整数$\geq 1$的集合稳定在乘法下；我们将阶关系 « m 除 n »。当 m 除 n 时，我们有 $m\mathbf{Z} \supset n\mathbf{Z}$，因此在环 $\mathbf{Z}/m\mathbf{Z}$ 上有环 $\mathbf{Z}/n\mathbf{Z}$ 的典范同态 $\pi_{m,n}$。我们用 S 索引的环 $(\mathbf{Z}/m\mathbf{Z}, \pi_{m,n})$ 逆系 $A(S)$ 逆极限表示。每个有限集合 $\mathbf{Z}/m\mathbf{Z}$ 配备离散的拓扑和 $A(S)$，并由拓扑诱导由乘积 $\prod_{n \in S} (\mathbf{Z}/n\mathbf{Z})$ 计算。

那么$A(S)$是一个紧拓扑环（Gen.Top.I，p. 64，第8条命题）。我们立即看到，$\mathbf{Z}$到$A(S)$的唯一环同态$\varphi$是与稠密的像单射； *我们将认同$\mathbf{Z}$及其像置于$\varphi$下$A(S)$*。对于$A(S)$在$\mathbf{Z}$上诱导的拓扑，*集合$m\mathbf{Z}$（对于$m \in S$）0*的邻域的形式基。

当$S = \mathbf{N}^*$时，$A(S)$写为$\hat{\mathbf{Z}}$。当S由素数数$l$的幂组成时，$A(S)$写作$\mathbf{Z}_l$，并称为I-adic整数的环。因此我们有

$$
\hat{\mathbf{Z}} = \lim_{\leftarrow m \geq 1} \mathbf{Z}/m\mathbf{Z} , \quad \mathbf{Z}_l = \lim_{\leftarrow n \geq 0} \mathbf{Z}/l^n\mathbf{Z} .
$$

当S和T是在乘法下稳定的整数的两个集合使得$S \supset T$时，我们有一个自然的投影$A(S) \to A(T)$，它是拓扑环的连续同态。特别是，对于每个素数数$l$，我们都有一个连续的同态$\mathbf{Z} \to \mathbf{Z}_l$。由此我们得到连续的同态

$$
\hat{\mathbf{Z}} \to \prod_l \mathbf{Z}_l
$$

（乘积扩展到所有素数数）；这是拓扑环*的*同构，如下来自第11条命题I、p. 112中到逆极限的段落。

令 K 为 q 元素的有限域和 K 的 K 代数闭包。对于每个整数 $m \geq 1$，我们用 $K_m$ 表示 K 的唯一子域，其比 K 次数 m（命题 3）。我们有$\overline{K} = \bigcup_{m \geq 1} K_m$。进一步我们用完美域$\overline{K}$的$\sigma_q$自同构$x \mapsto x^q$来表示；它被称为 K 的 *Frobenius 自同构*（相对于 K）。

#### 命题 5 {#alg-v-s12-prop-5 .statement tag=06QE}

— 存在拓扑群 $\pi_K : \mathbf{Z} \to \mathrm{Gal}(\bar{K}/K)$ 的唯一同构，使得 $\pi_K(1) = \sigma_q$。

令$\Gamma$为由$\sigma_q$生成的$\mathrm{Gal}(\bar{K}/K)$的子群。对于每个整数$m > 0$，我们对所有$x \in \bar{K}$都有$\sigma_q^m(x) = x^{q^m}$，因此$\sigma_q^m$的固定点的集合等于$K$。从$K \neq \bar{K}$开始，我们有$\sigma_q^m \neq 1$。因此，$\mathbf{Z}$有同构$\pi_0$到$\Gamma$，其中映射1到$\sigma_q$。

$\Gamma$的不变量域由$x \in K$组成，使得$x^q = x$等于$K$。因此 (V, p. 67, 引理 2) 群 $\Gamma$ 在 $\mathrm{Gal}(\bar{K}/K)$ 中是稠密的。由于有限次数的 $\bar{K}$ 在 $K$ 上的每一个子扩展都是域 $K_m$ 之一，子群 $\mathrm{Gal}(\bar{K}/K_m)$ 形式邻域的基本系统为 1 in $\mathrm{Gal}(\bar{K}/K)$。显然，$\Gamma \cap \mathrm{Gal}(\bar{K}/K_m)$是$\sigma_q^m$生成的循环群，因此等于$\pi_0(m\mathbf{Z})$。

从上述$\mathbf{Z}$同构$\pi_0 : \mathbf{Z} \to \Gamma$扩展的注约拓扑以独特的方式到拓扑群$\pi_K : \mathbf{Z} \to \mathrm{Gal}(\bar{K}/K)$的同构。

设$m \geq 1$为整数；显然，$\bar{K}$相对于$K$的弗罗贝尼乌斯自同构是$\sigma_q^m$。因此我们得到关系

$$
\pi_{K_m}(a) = \pi_K(ma) \quad \text{for } a \in \mathbf{Z}.
$$

### 4. 有限域上的分圆多项式

设$K$为$q$元素的有限域，$n \geq 1$整数不能被$K$和$R_n$的特征$p$整除，$n$的分圆扩张为$K$（V，p. 81）。我们知道$R_n$中单位元的$n$-第根的群$\mu_n(R_n) = \mu_n$，是阶$n$的循环，即$R_n = K(\mu_n)$且存在单同态

$$
\varphi_n : \mathrm{Gal}(R_n/K) \to (\mathbf{Z}/n\mathbf{Z})^*
$$

这样$\sigma(\zeta) = \zeta^j$代表$\sigma \in \mathrm{Gal}(R_n/K)$、$\zeta \in \mu_n$和$j \in \varphi_n(\sigma)$。

此外，如果$f$是$R_n$在$K$上的次数，则$R_n$在$K$上的伽罗瓦群是阶$f$的循环，由自同构$\sigma_q : x \mapsto x^q$生成（V，p. 95，提案 4）。我们立刻就有：

#### 命题 6 {#alg-v-s12-prop-6 .statement tag=06QF}

— Frobenius 自同构 $\sigma_q$ 的 $\varphi_n$ 下的像是 $q \mod n$ 的剩余类类。

因此，考虑到V、p. 84的第6号提案：

#### 推论{#alg-v-s12-n4-cor-1 .statement tag=06QG}

— $R_n$ 中的 $K$ 中的次数是最小的整数 $f \geq 1$，使得 $q^f \equiv 1 \pmod{n}$。为了使分圆多项式$\Phi_n$在$K$上不可约，群$(\mathbf{Z}/n\mathbf{Z})^*$应由$q$模$n$生成剩余类类是必要且充分的。

#### 例 1 {#alg-v-s12-n4-exa-1 .statement tag=06QH}

多项式 $\Phi_3(X) = X^2 + X + 1$ 在 $F_q[X]$ 中不可约，当且仅当 $q \equiv 2 \pmod{3}$。同样地，$\Phi_4(X) = X^2 + 1$在$F_q[X]$中是不可约的，当且仅当$q \equiv 3 \pmod{4}$并且对于$\Phi_5 = X^4 + X^3 + X^2 + X + 1$，不可约性条件读取为$q \equiv 2,\ 3 \pmod{5}$。

#### 例 2 {#alg-v-s12-n4-exa-2 .statement tag=06QI}

我们有 $5^2 \equiv 1 \pmod{12}$，因此 5 (mod 12) 的剩余类类不等于生成 $(\mathbf{Z}/12\mathbf{Z})^*$。所以多项式$\Phi_{12}(X) = X^4 - X^2 + 1$在$F_5[X]$中不是不可约的；事实上我们有
$$
\Phi_5(X) = (X^2 + 2X - 1)(X^2 - 2X - 1)
$$
在$F_5[X]$。

### 习题{#alg-v-s12-exercises}

§ 12](exercises/s12/)参见[习题。
