---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 4
section_title: Some classes of operators in hilbertian spaces
lang: zh
source: evt-i-v
book_pages: TVS V.74-TVS V.79
pdf_pages: 0295-0318, 0332-0337
extraction: ocr
subsections:
    - "no": 1
      title: Adjoint
      page: 38
      pdf_page: 296
    - "no": 2
      title: Partially isometric linear mappings
      page: 41
      pdf_page: 299
    - "no": 3
      title: Normal endomorphisms
      page: 43
      pdf_page: 301
    - "no": 4
      title: Hermitian endomorphisms
      page: 44
      pdf_page: 302
    - "no": 5
      title: Positive endomorphisms
      page: 45
      pdf_page: 303
    - "no": 6
      title: Trace of an endomorphism
      page: 48
      pdf_page: 306
    - "no": 7
      title: Hilbert-Schmidt mappings
      page: 52
      pdf_page: 310
    - "no": 8
      title: Diagonalization of Hilbert-Schmidt mappings
      page: 55
      pdf_page: 313
    - "no": 9
      title: Trace of a quadratic form with respect to another
      page: 57
      pdf_page: 315
statements: 49
exercises: 15
content_sha256: 572cbbb906314c6b764e000fea81b424bd8d50bf37bc72f93a7a5dee2608e1fe
translated_from: content/en/evt/V/04_s4_some_classes_of_operators_in_hilbertian.md
translation_method: google
source_content_sha256: cb9870367ecf6e5e9e4940666c860653cc61494e1c8cc7bf56a66fd20a2556ef
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 297e8d88ea944c6b820dce6a9cbc8786e6363917eac9bdf7b67903f554bd1d11
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 4。一些类希尔伯特空间运算符

在本段中，$l_E$表示希尔伯特空间E的恒等映射。两个线性映射的合成$v \circ u$通常用$vu$或$v.u$表示。

### 1. 伴随

#### 命题 1 {#evt-v-s4-prop-1 .statement tag=080X}

— 令 E 和 F 为两个希尔伯特空间。对于每个映射 $u \in \mathscr{L}(E; F)$，都存在唯一映射 $u^* \in \mathscr{L}(F; E)$ 使得

$$
\langle u(x)|y \rangle_F = \langle x|u^*(y) \rangle_E
$$

对于所有 $x \in E$ 和所有 $y \in F$。从$\mathscr{L}(E, F)$到$\mathscr{L}(F; E)$的映射$u \mapsto u^*$是双射、等距和半线性的（相对于K的自同构$\xi \mapsto \overline{\xi}$）。

令$\mathscr{S}(E, F)$为$E \times F$上所有连续倍半线性形式的空间，赋予范数

$$
\| \Phi \| = \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi(x, y)| .
$$

我们定义空间$\mathscr{S}(F, E)$类似。我们定义了（V，p. 16，cor.2）从$\mathscr{L}(E; F)$到$\mathscr{S}(F, E)$的Banach空间同构，用$u \mapsto \Phi_u$表示，其特征为

$$
\Phi_u(y, x) = \langle y|u(x) \rangle_F \quad (x \in E, \ y \in F) .
$$

以类似的方式，我们从 $\mathscr{L}(F, E)$ 定义同构到 $\mathscr{S}(E, F)$。最后我们从 $\mathscr{S}(F, E)$ 定义映射 $\Phi \mapsto \Phi^*$ 到$\mathscr{S}(E, F)$

$$
\Phi^*(x, y) = \overline{\Phi(y, x)} \quad (x \in E, \ y \in F) .
$$

这个映射是双射、半线性和等距的。但公式 (1) 翻译为$\Phi_{u^*} = (\Phi_u)^*$，因此是命题。

#### 定义 1 {#evt-v-s4-def-1 .statement tag=080Y}

— 令 E 和 F 为两个希尔伯特空间。对于每个连续线性映射$u : E \to F$，由公式(1)定义的从F到E的连续线性映射称为u的伴随，记为$u^*$。

我们有

$$
\begin{align*}
(u + v)^* &= u^* + v^* \\
(\lambda u)^* &= \overline{\lambda} u^* \\
(u^*)^* &= u \\
(1_E)^* &= 1_E \\
(wu)^* &= u^* w^* ;
\end{align*}
$$

在所有这些公式，$u$和$v$属于到$\mathscr{L}(E; F)$中，$\lambda$在K中，$w$在$\mathscr{L}(F; G)$中，其中G是希尔伯特空间。 公式 (5) 和 (6) 意味着 $u \mapsto u^*$ 是半线性的。 公式 (8) 显而易见。为了证明(7)，我们取(1)的两个成员的共轭，得到$\langle u^*(y)|x\rangle = \langle y|u(x)\rangle$，这就证明了$u$是$u^*$的伴随。最后，对于 (9) 的记号，我们有 $z \in G$

$$
\langle w(u(x))|z\rangle = \langle u(x)|w^*(z)\rangle = \langle x|u^*(w^*(z))\rangle ,
$$

因此$u^*w^*$是$wu$的伴随物。

令$u : E \to F$为双射且连续的线性映射；那么它也是双连续的（I，p. 19，cor.1）。从 (8) 和 (9) 我们立即推断 $u^*$ 是双射且双连续的，并且

(10)
$$
(u^{-1})^* = (u^*)^{-1} .
$$

#### 命题 2 {#evt-v-s4-prop-2 .statement tag=080Z}

*对于每$u \in \mathscr{L}(E ; F)$，我们有*

(11)
$$
\|u^*u\| = \|uu^*\| = \|u\|^2 = \|u^*\|^2 .
$$

通过道具。 1、$\|u^*\| = \|u\|$，因此$\|u^*u\| \leq \|u^*\|\cdot\|u\| \leq \|u\|^2$。另一方面，

$$
\|u\|^2 = \sup_{\|x\| \leq 1} \|u(x)\|^2 = \sup_{\|x\| \leq 1} \langle u(x)|u(x)\rangle = \sup_{\|x\| \leq 1} \langle x|u^*u(x)\rangle \leq \|u^*u\| ,
$$

因此$\|u^*u\| = \|u\|^2$。 替换$u$乘以$u^*$，我们得到$\|uu^*\| = \|u^*\|^2$，因此从$\|u\| = \|u^*\|$开始有(11)。

令$E_1, ..., E_n$和$F_1, ..., F_n$为希尔伯特空间，对于1和$n$之间的每个整数$i$，令$u_i$为从$E_i$到$F_i$的连续线性映射。然后

(12)
$$
(u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n)^* = u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^* .
$$

令 $v$ 为连续线性映射 $u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$

$$
E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n \quad \text{into} \quad F = F_1 \hat{\otimes}_2 ... \hat{\otimes}_2 F_n
$$

以及$w$从$F$到$E$连续的线性映射$u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^*$。对于$x \in E$和$y \in F$证明等式$\langle y|v(x)\rangle = \langle w(y)|x\rangle$就足够了。通过线性和连续性，我们约化到$x$和$y$有以下形式的情况

$$
x = x_1 \otimes ... \otimes x_n , \quad y = y_1 \otimes ... \otimes y_n
$$

$x_i \in E_i$ 和 $y_i \in F_i$ 代表 $1 \leq i \leq n$。从张量积中标量乘积的定义 (V, p. 27, 公式 (6))，我们得到

$$
\langle y|v(x)\rangle = \prod_{i=1}^n \langle y_i|u_i(x_i)\rangle = \prod_{i=1}^n \langle u_i^*(y_i)|x_i\rangle = \langle w(y)|x\rangle .
$$

这证明了我们的断言。

令$E$和$F$是两个希尔伯特空间、$u \in \mathscr{L}(E ; F)$和$n$正整数。如果我们将$u_1 = ... = u_n = u$放入公式（12），我们得到的结果是，从$\hat{T}^n(F)$到$\hat{T}^n(E)$的连续线性映射$\hat{T}^n(u^*)$是从$\hat{T}^n(E)$到线性映射$\hat{T}^n(u)$的伴随物$\hat{T}^n(F)$。 公式

$$
\hat{S}^n(u)^* = \hat{S}^n(u^*) , \quad \hat{\Lambda}^n(u)^* = \hat{\Lambda}^n(u^*)
$$

可以按照与公式 (12) 相同的方式建立，考虑到 $\hat{S}^n(E)$ (V, p. 30, 公式 (15)) 和 $\hat{\Lambda}^n(E)$ (V) 中标量乘积的定义， p. 33、公式 (26))。

#### 注 1 {#evt-v-s4-n1-rem-1 .statement tag=0810}

假设希尔伯特空间 E 不约化到 0。我们认同 $\mathscr{L}(K;E)$ 与 E 映射 $u \mapsto u(1)$；在其他字中，E的向量 x从K到E用映射$\lambda \mapsto \lambda.x$标识。那么x的伴随物是由$x^*(y) = \langle x|y \rangle$给出的映射$x^*:E \to K$。在其他字中，$x \mapsto x^*$ 是从 E 到其对偶 (V, p. 15) 的规范半线性映射。

同样，我们将 E 的认同数 $\lambda \in K$ 与自同态 $\lambda.1_E$ 进行组合。那么 $\lambda^*$ 正好是 $\lambda$ 的共轭。

通过这些标识，我们可以定义乘积 $t_1 ... t_n$，其中每个 $t_i$ 是 K 中的数，或 E 中的向量，或 E' 中的线性形式属于，或 E' 中的元素 $\mathscr{L}(E)$，前提是以下型之一永远不存在两个连续的因子 $t_i$ 和 $t_{i+1}$ ：
• xy，其中x、y 均在E 中，或均在E' 中；
• xA 或Ax' 具有$A \in \mathscr{L}(E)$、$x \in E$ 和$x' \in E'$。

我们有以下合成规则：
a）结合性；
b) K 中的每个元素都与所有其他因子通勤；
c) 我们有 $(t_1 ... t_n)^* = t_n^* ... t_1^*$；在其他字中，乘积的伴随词是阶的逆伴随词的乘积。还有$t^{**} = t$。

对于例，令x、y在E中，并令A在$\mathscr{L}(E)$中。那么$x^*y$代表标量乘积$\langle x|y \rangle$，$x^*Ay$代表标量乘积$\langle x|Ay \rangle$。我们还有$(A^*x)^* = x^*A^{**} = x^*A$，因此$(A^*x)^*y = x^*Ay$，可以解释为

$$
\langle A^*x|y \rangle = \langle x|Ay \rangle
$$

与伴随的定义一致。我们观察到$yx^*$是E的自同态$z \mapsto y \langle x|z \rangle$，因为$yx^*z$可以通过结合性解释为$y(x^*z)$，或者解释为$y.\langle x|z \rangle$。

继狄拉克$^1$之后，在大多数数学物理著作中，E的元素用符号$|x\rangle$表示，E'的$\langle t|$表示。标量乘积写为$\langle x|y \rangle = \langle x|.|y \rangle$，乘积中的第一条禁止规则排除了$|$和$|<$的组合，对于例$|x\rangle|y\rangle$。

#### 命题 3 {#evt-v-s4-prop-3 .statement tag=0811}

— 令 E 和 F 为两个希尔伯特空间和 $u \in \mathscr{L}(E;F)$。以下条件是等效的：

(i) $u$ 是拓扑向量空间同构，其逆等于 $u^*$；
(ii) $u$ 是满射且 $u^*u = 1_E$；
(iii) $u$ 是单射且 $uu^* = 1_F$；
(iv) $u$是范数空间的同构；
(v) $u$ 是希尔伯特空间同构。

条件 (1) 意味着我们有 $u^*u = 1_E$ 和 $uu^* = 1_F$。因此，(i)、(ii) 和 (iii) 的等价由 E、II, § 3, No. 8 命题得出。 8. 我们已经看过(iv)和(v)的等价（V，p. 5）。最后，关系$u^*u = 1_E$相当于

$^1$ 参见 P. A. M. Dirac，《量子力学》，牛津大学出版社，纽约，1935 年。

$
\langle x|u^*u(y)\rangle = \langle x|y\rangle$，即$E$中的所有$x, y$到$\langle u(x)|u(y)\rangle = \langle x|y\rangle$，显然意味着$u$是单射的；这就证明了(ii)和(v)的等价。

希尔伯特空间$E$的自同构也称为*酉算子*，即算子$u \in \mathscr{L}(E)$满足$uu^* = u^*u = 1_E$。

#### 注 2 {#evt-v-s4-n1-rem-2 .statement tag=0812}

— 关系 $u^*u = 1_E$ 并不能表征希尔伯特空间 $E$ 的所有自同构。对于例，对于$n \geq 1$和$u(x)_0 = 0$，让$E = \ell^2(\mathbf{N})$和$u$由$u(x_n) = x_{n-1}$定义。对于所有 $x \in E$，我们有 $\|u(x)\| = \|x\|$，即 $u^*u = 1_E$，但 $u$ 不是满射的。

#### 注 3 {#evt-v-s4-n1-rem-3 .statement tag=0813}

— 伴随$u^*$的定义 (1) 也可以写成
$$
\langle y|u(x)\rangle = \langle u^*(y)|x\rangle ,
$$
或者，通过V，p. 15，作为
$$
\langle u(x), y^*\rangle = \langle x, (u^*(y))^*\rangle .
$$
但我们也有$\langle u(x), y^*\rangle = \langle x, {}^t u(y^*)\rangle$，因此我们可以表达项中转置的伴随，
$$
(u^*(y))^* = {}^t u(y^*) .
$$

### 2. 部分等轴测线性映射

#### 定义 2 {#evt-v-s4-def-2 .statement tag=0814}

*令$E$和$F$为两个希尔伯特空间和$u \in \mathscr{L}(E; F)$。 $E$中$u$的核正交被称为$u$的初始子空间，$F$中$u$的像的闭包称为$u$的最终子空间。从$E$（或$F$）到$u$的初始（或最终）子空间的正射投影称为$u$的初始（或最终）正射投影。*

令$P$为$u$的初始子空间。由于$E$是$P$的直和和$u$的核，所以我们有$u(P) = u(E)$。

#### 命题 4 {#evt-v-s4-prop-4 .statement tag=0815}

(i) *$u^*$的初始（或最终）子空间等于$u$的最终（或初始）子空间。*

(ii) *假设$E = F$。令 $M$ 为 $E$ 的闭向量子空间，且$M^\circ$ 与其正交。 关系 $u(M) \subset M$ 和 $u^*(M^\circ) \subset M^\circ$ 等效。*

令$Q = \overline{u(E)}$为$u$的最终子空间。 $F$中$Q$的正交$Q^\circ$由所有向量$y$组成，使得$\langle u(x)|y\rangle = 0$对于所有$x \in E$；这相当于：对于所有$x \in E$，$\langle x|u^*(y)\rangle = 0$，或$u^*(y) = 0$。因此我们有$Q^\circ = \mathrm{Ker}\, u^*$，$Q$是$u^*$的初始子空间。由于$u$是$u^*$的伴随，$u^*$的最后一个子空间也是$u$的初始子空间。这就证明了(i)。

关系$u(M) \subset M$意味着$u(M)$与$M^\circ$正交，关系$u^*(M^\circ) \subset M^\circ$意味着$u^*(M^\circ)$与$M$正交。但对于所有 $x \in M$ 和 $y \in M^\circ$，我们都有 $\langle u(x)|y\rangle = \langle u^*(y)|x\rangle$；因此 (ii) 如下。

我们注那个道具。 4可以根据注3、V、p. 41从转置（II、p. 51、cor.2）的一般性质推导出来。

#### 定义 3 {#evt-v-s4-def-3 .statement tag=0816}

*令$E$和$F$为两个希尔伯特空间。如果 $\|u(x)\| = \|x\|$ 对于所有 $x$ 属于到 $u$ 的初始子空间，映射 $u \in \mathscr{L}(E; F)$ 被认为是部分等距的。

设$u \in \mathscr{L}(E; F)$，$N$为其核，$I$为其像。说$u$是部分等距的，与从$u$推导出线性映射$\tilde{u}: E/N \to I$是等距的说是一样的（V，p. 13）。那么$F$的子空间$I$是完整的，因此关闭，是$u$的最终子空间。因而，$u$诱导是一个希尔伯特空间同构，从$u$的初始子空间到最终的子空间。

#### 命题 5 {#evt-v-s4-prop-5 .statement tag=0817}

*设$u \in \mathscr{L}(E; F)$，$P$为其初始子空间，$Q$为最终子空间。让$p$（或$q$）表示$u$的初始（或最终）正射投影。假设 $u$ 是部分等轴测的。*

(i) *映射 $u^* \in \mathscr{L}(F; E)$ 部分等轴测，初始子空间 $Q$ 和最终子空间 $P$。由 $u$ 引起的从 $P$ 到 $Q$ 的同构是由 $u^*$ 引起的从 $Q$ 到 $P$ 的同构的倒数。*

(ii) *我们有 $u^*u = p$ 和 $uu^* = q$。*

由于道具。 4(i)，断言(i)是(ii)的推论。

我们现在证明(ii)。从$u^*$的$P$包含像开始，映射$u^*u$映射$E$变为$P$。设 $x \in E$ 和 $y \in P$，则

$$
\langle u^*u(x)|y \rangle = \langle u(x)|u(y) \rangle .
$$

如果 $x$ 属于到 $P$，则部分等距映射的 $\langle u(x)|u(y) \rangle = \langle x|y \rangle$ 乘定义；如果$u$的$x$属于到核$N$，则$u(x) = 0$，因而$\langle u(x)|u(y) \rangle = 0$和$\langle x|y \rangle = 0$，因为$N$和$P$是正交的。从$E = P \oplus N$开始，在所有情况下我们都有$\langle u^*u(x) - x|y \rangle = 0$，因而$u^*u$是从$E$到$P$的正射投影$p$。上面的$uu^* = q$后面是交换、$u$和$u^*$。

#### 命题 6 {#evt-v-s4-prop-6 .statement tag=0818}

*对于每个$u \in \mathscr{L}(E; F)$，以下条件是等效的：*

(i) *$u$ 部分等距；*
(ii) *$u^*$ 部分等轴测；*
(iii) *$u^*u$ 是正射投影仪；*
(iv) *$uu^*$ 是正射投影仪；*
(v) *$uu^*u = u ;*$
(六) *$u^*uu^* = u^* .*$

通过道具。 5、(i)相当于(ii)。

(i) $\Rightarrow$ (v) ：假设 $u$ 是部分等距的。那么$u^*u$就是$u$通过prop的初始正射投影。 5. 因此，对于$u$中的每个$x \in E$，$u^*u(x) - x$属于到核，即$uu^*u(x) = u(x)$。

(v) $\Rightarrow$ (iii) : 假设$uu^*u = u$并设$p = u^*u$；然后是$p = p^*$和$p^2 = p$。令$M$（或$N$）为$p$的像（或核）。对于$x \in M$和$y \in N$，我们有$\langle x|y \rangle = \langle p(x)|y \rangle = \langle x|p^*(y) \rangle = \langle x|p(y) \rangle = 0$。由于 $M$ 和 $N$ 正交，因此 $p$ 是从 $E$ 到 $M$ 的正射投影。

(iii) $\Rightarrow$ (i) : 假设 $p = u^*u$ 是具有像 $M$ 和核 $N$ 的正射投影仪。

对于所有$x \in E$，我们有
$$
\|u(x)\|^2 = \langle u^*u(x)|x \rangle = \langle p(x)|x \rangle .
$$
因此，$u(x) = 0$代表$x \in N$，$\|u(x)\| = \|x\|$代表$x \in M$，因此$u$与核$N$和初始子空间$M$部分等距。

我们已经证明了(i)、(iii)和(v)的等价。 替换 $u$ 由$u^*$，可推导出(ii)、(iv)、(vi)的等价。这证明了。 6.

### 3. 正常自同态

#### 定义 4 {#evt-v-s4-def-4 .statement tag=0819}

令$E$为希尔伯特空间和$u \in \mathscr{L}(E)$。 We say that $u$ is normal if it commutes with its adjoint $u^*$.

对于例，希尔伯特空间$E$的每个自同构$u$都是正常的，因为我们有$uu^* = u^*u = 1_E$。

#### 命题 7 {#evt-v-s4-prop-7 .statement tag=081A}

为了使$u \in \mathscr{L}(E)$正常，$\|u(x)\| = \|u^*(x)\|$对于所有$x \in E$是必要且充分的。

我们在 $E$ 定义厄米特形式 $\Phi$
$$
\Phi(x, y) = \langle uu^*(x)|y \rangle - \langle u^*u(x)|y \rangle .
$$
要使$u$正常，$\Phi = 0$是必要且充分的。通过极化公式（V，p. 2），这相当于所有$x \in E$的$\Phi(x, x) = 0$。 命题现在跟随
$$
\Phi(x, x) = \|u^*(x)\|^2 - \|u(x)\|^2 .
$$

#### 命题 8 {#evt-v-s4-prop-8 .statement tag=081B}

假设$u \in \mathscr{L}(E)$是正常的。 令$N$为$u$的核和$M$在$E$中$N$的正交；令$m$和$n$是两个正整数，使得$m + n \geq 1$。 Then $N$ is the kernel of $u^m(u^*)^n$ and $M$ is both the initial and the final subspace of $u^m(u^*)^n$. 特别地，$M$既是$u$和$u^*$的初始和最终子空间，并且在$u$和$u^*$下稳定。

命题7表明$u$和$u^*$有相同的核$N$。通过道具。 4、(ii) V、p. 41、$E$的子空间$M$在$u$和$u^*$下是稳定的，因为对于$N = M^\circ$也是如此，因为$M \cap N = \{0\}$、自同态由$M$引起$u$ 和 $u^*$ 是单射的。令 $v = u^m(u^*)^n$；前面的论证表明，$v$到$M$（或$N$）的限制是单射的（或空），因而$N$是$v$的核。因而，$M = N^\circ$是$v$的初始子空间。通过道具。 4、(i)V、p. 41，$v$最后的子空间等于$v^*$最初的子空间。但是$v^* = u^n(u^*)^m$，所以$v^*$的初始子空间等于前面的$M$。

#### 推论{#evt-v-s4-n3-cor-1 .statement tag=081C}

让$\lambda \in K$。以下子空间与 $E$ 相等：
a) $u$相对于$\lambda$的特征值子空间；
b) $u^*$相对于$\overline{\lambda}$的特征值子空间；

c) *u 相对于* $\lambda$ 的主子空间（在其他字中，通过 LIE，E 的所有向量 $x$ 的VII, § 1, No. 1、集合，其中存在整数 $n \geqslant 0$，使得 $(u - \lambda.1_E)^n(x) = 0$）；
d) ** $u^*$ *主要子空间 *相对于* $\overline{\lambda}$。

很明显，$w = u - \lambda.1_E$是E的正常自同态，因此E的自同态$w, w^* = u^* - \overline{\lambda}.1_E, w^n$和$(w^*)^n$通过prop具有相同的核。 8.

### 4. 厄米特自同态

#### 定义 5 {#evt-v-s4-def-5 .statement tag=081D}

*设 E 为希尔伯特空间，并设*$u \in \mathscr{L}(E)$。 *我们说如果* $u^* = u$，你就是厄米特。

让$\mathscr{H}(E)$表示$\mathscr{L}(E)$的所有厄米特元素中的集合；这是向量子空间除以向量空间$\mathscr{L}(E)_{[\mathbf{R}]}$超过$\mathbf{R}$，这是通过限制标量从$\mathscr{L}(E)$推导出来的。

对于每个$u \in \mathscr{L}(E)$，我们在$E \times E$上关联了（V，p. 16，cor.2）一个倍半线性的形式$\Phi_u : (x, y) \mapsto \langle x|u(y)\rangle$。我们有

$$
\Phi_{u^*}(x, y) = \overline{\Phi_u(y, x)} \quad (x, y \text{ in } E);
$$

因而，当且仅当形式$\Phi_u$是厄米特时，$u$是厄米特。当 K 为 $\mathbf{C}$ 时，足以假设 $\Phi_u(x, x) = \langle x|u(x)\rangle$ 对于所有 $x \in E$（V、p. 2、*注*）都是实数。

让$u \in \mathscr{L}(E)$。我们已经看到（V，p. 16，cor.2）$u$的范数可以通过公式计算

$$
\|u\| = \sup_{\|x\| \leqslant 1, \|y\| \leqslant 1} |\Phi_u(x, y)|.
$$

当$u$为厄米特时，我们得到以下结果：

#### 命题 9 {#evt-v-s4-prop-9 .statement tag=081E}

*对于* E 的每个厄米特自同态 u，*我们有*

$$
\|u\| = \sup_{\|x\| \leqslant 1} |\langle x|u(x)\rangle|.
$$

放入$\Phi = \Phi_u$和$c = \sup_{\|x\| \leqslant 1} |\Phi(x, x)|$，显然是$c \leqslant \|u\|$。令$x, y$在E中使得$\|x\| \leqslant 1, \|y\| \leqslant 1$。然后

$$
\Phi(x + y, x + y) = \Phi(x, x) + \Phi(y, y) + 2\Re\Phi(x, y),
$$
因而
$$
4\Re\Phi(x, y) = \Phi(x + y, x + y) - \Phi(x - y, x - y);
$$
但 $|\Phi(t, t)| \leqslant c\|t\|^2$ 对于所有 $t \in E$，因而
$$
4|\Re\Phi(x, y)| \leqslant c(\|x + y\|^2 + \|x - y\|^2) = 2c(\|x\|^2 + \|y\|^2) \leqslant 4c.
$$
让$a = \Phi(x, y)$；存在复数 $\lambda$ 且绝对值 1 使得

λa = |a|。 替换 y 除以前面不等式中的λy，我们得到$|\Phi(x, y)| \leq c$。根据 (15)，可得到 $\|u\| \leq c$ 和命题。 Q.E.D.

显然每个厄米特自同态都是正常的。反之：

#### 命题 10 {#evt-v-s4-prop-10 .statement tag=081F}

— 假设 K 为 C。让$u \in \mathscr{L}(E)$。那么E的厄米特自同态存在唯一的对$(h_1, h_2)$，使得$u = h_1 + ih_2$。 u正常的阶中，$h_1$与$h_2$通勤是充分必要的。

对于，关系 « $u = h_1 + ih_2,\ h_1^* = h_1,\ h_2^* = h_2$ » 相当于

$$
\text{« } h_1 = \frac{1}{2}(u + u^*) \text{ and } h_2 = \frac{i}{2}(u^* - u) \text{ »}.
$$

在加法，我们有$h_1 h_2 - h_2 h_1 = \frac{i}{2}(uu^* - u^*u)$。这证明了。 10.

#### 命题 11 {#evt-v-s4-prop-11 .statement tag=081G}

— 让$p \in \mathscr{L}(E)$。在阶中，p 是从 E 到 E 的闭向量子空间的正射投影，$p^2 = p = p^*$ 是充分必要的。

假设$p^2 = p$。设 M 为 p 的像，N 为核。 E 是 M 和 N 的拓扑直和。在阶中，p 是正交投影，M 与 N 正交是充分必要的，也就是说，对于 E 中的所有 x、y，我们有 $\langle p(x)|y - p(y) \rangle = 0$。后者关系相当于 $p = p^*p$，并且意味着： $p^* = (p^*p)^* = p^*p = p$；相反，如果$p^* = p$，我们就有$p = p^2 = p^*p$。

### 5. 积极自同态

#### 定义 6 {#evt-v-s4-def-6 .statement tag=081H}

— 令 E 为希尔伯特空间和 $u \in \mathscr{L}(E)$。我们说 u 是正数，如果 u 是厄米特并且对于所有 $x \in E$ 都是 $\langle x|u(x) \rangle \geq 0$，则写为 $u \geq 0$。

当K等于C、关系时

$$
\langle x|u(x) \rangle \geq 0 \quad \text{for all } x \in E
$$

意味着 u 是厄米特 (V, p. 2, 注)，因此是正数。

让$\mathscr{L}_+(E)$表示$\mathscr{L}(E)$的所有正元素中的集合；这是真实向量空间$\mathscr{L}(E)_{[\mathbf{R}]}$底层$\mathscr{L}(E)$中的正尖凸锥。在阶中，u为正，则与u相关的$E \times E$上的倍半线性形式$\Phi_u$为正厄米特是充分必要的。给定$\mathscr{L}(E)$中的u和v，关系$u - v \geq 0$也可以写成$u \geq v$或$v \leq u$；这是$\mathscr{L}(E)_{[\mathbf{R}]}$上的序关系与其真实的向量空间结构兼容。

#### 命题 12 {#evt-v-s4-prop-12 .statement tag=081I}

— 令 u 为 $\mathscr{L}(E)$ 的厄米特（分别为正）元素，并令 v 为从 E 到希尔伯特空间 F 的连续线性映射。则 $vuv^*$ 为厄米特（分别为正）元素 $\mathscr{L}(F)$。

因为，我们有$(vuv^*)^* = v^{**}u^*v^* = vuv^*$。另一方面，如果$u \geq 0$，我们有

$$
\langle y|vuv^*(y) \rangle = \langle v^*(y)|u(v^*(y)) \rangle \geq 0
$$

对于所有$y \in F$，因此$vuv^* \geq 0$。

命题 12 特别表明，$vv^*$ 对于所有$v \in \mathscr{L}(E; F)$ 都是正数。特别是，由于正射投影$p$满足$p = p^2 = pp^*$，因此它是正的。

#### 注 1 {#evt-v-s4-n5-rem-1 .statement tag=081J}

对于$\mathscr{L}(E)$中的每个厄米特$u$，放入$m(u) = \inf_{\|x\|=1} \langle x|u(x)\rangle$，$M(u) = \sup_{\|x\|=1} \langle x|u(x)\rangle$。如果$E$不只是0，$m(u)$和$M(u)$是有限的；此外，$M(u)$是最小的实数$\lambda$使得$u \leq \lambda \cdot 1_E$和$m(u)$最大的实数$\mu$使得$u \geq \mu \cdot 1_E$。显然我们有$m(-u) = -M(u)$和$M(-u) = -m(u)$。很明显，
$$
\sup(|m(u)|, |M(u)|) = \sup_{\|x\|=1} |\langle x|u(x)\rangle|
$$
和道具。 9 (V, p. 44) 意味着（对于 $E \neq \{0\}$）
$$
\|u\| = \sup(|m(u)|, |M(u)|).
$$
\* 对于当 $K$ 为 $\mathbf{C}$ 时，此公式的另一个证明，请参阅 prop。 TS 14，I, § 6, No. 8。 \*

#### 注 2 {#evt-v-s4-n5-rem-2 .statement tag=081K}

令$M$和$N$为$E$的两个闭向量子空间，以及$p_M$（或$p_N$）从$E$到$M$（或$N$）的正射投影仪。那么$M \subset N$当且仅当$p_M \leq p_N$。因为，我们有 $p_M^* p_M = p_M$，因此
$$
\|p_M(x)\|^2 = \langle p_M(x)|p_M(x)\rangle = \langle x|p_M^* p_M(x)\rangle = \langle x|p_M(x)\rangle
$$
对于所有$x \in E$。因此，关系 $p_M \leq p_N$ 相当于 « $\|p_M(x)\| \leq \|p_N(x)\|$ 对于所有 $x \in E$ »。如果$M \subset N$，我们有$p_M = p_M p_N$，因此从$\|p_M\| \leq 1$开始就有$\|p_M(x)\| \leq \|p_N(x)\|$。相反，如果$\|p_M(x)\| \leq \|p_N(x)\|$对于所有$x \in E$，$p_M$包含核$p_N$中的核，即$M^\circ \supset N^\circ$，这意味着$M \subset N$。

#### 命题 13 {#evt-v-s4-prop-13 .statement tag=081L}

— *令 $\mathscr{H}(E)$ 为希尔伯特空间 $E$ 的所有连续厄米特自同态的集合。令$\mathscr{F}$为非空、有向递增且$\mathscr{H}(E)$有界子集。*

(i) *集合$\mathscr{F}$在$\mathscr{H}(E)$中有上界$u_0$；我们有*
$$
\langle x|u_0(x)\rangle = \sup_{u \in \mathscr{F}} \langle x|u(x)\rangle \quad \text{for all} \quad x \in E .
$$

(ii) *$\mathscr{F}$的截面滤波器在空间$\mathscr{L}(E)$中收敛到$u_0$，赋予拓扑简单收敛性。*

设$\Sigma$为$\mathscr{F}$的截面的滤波器；对于每个 $u \in \mathscr{H}(E)$，令 $\Phi_u$ 为 $E$ 上的连续厄米特形式定义为
$$
\Phi_u(x, y) = \langle x|u(y)\rangle .
$$
让
$$
\Psi_u(x) = \Phi_u(x, x)
$$
对于 $u \in \mathscr{H}(E)$ 和 $x \in E$。通过极化公式 (V, p. 2)，我们有
$$
\begin{align*}
(19) \quad 4\Phi_u(x, y) &= \Psi_u(x+y) - \Psi_u(x-y) & \text{if } K = \mathbf{R} \\
(20) \quad 4\Phi_u(x, y) &= \Psi_u(x+y) - \Psi_u(x-y) - i\Psi_u(x+iy) + i\Psi_u(x-iy) & \text{if } K = \mathbf{C} .
\end{align*}
$$

对于每个$x \in E$，从$\mathbf{R}$到映射$u \mapsto \Psi_u(x)$是递增并且有界，因此相对于$\Sigma$有极限。由前面的公式、极限
$$
\lim_{u,\Sigma} \Phi_u(x, y) = \Phi(x, y)
$$
存在于对$(x, y)$/元素/$E$。很明显，$\Phi$在$E$上是厄米特形式。如果$v_1 \in \mathscr{F}$和$v_2$是$\mathscr{F}$的界限，则厄米特形式$f_1 = \Phi - \Phi_{v_1}$和$f_2 = \Phi_{v_2} - \Phi$为正；存在实数 $M \geq 0$ 使得
$$
f_1(x, x) + f_2(x, x) = \Phi_{v_2 - v_1}(x, x) \leq M \|x\|^2,
$$
因而
$$
f_1(x, x) \leq M \|x\|^2, \quad f_2(x, x) \leq M \|x\|^2 \quad (x \in E);
$$
因此半范数$x \mapsto f_i(x, x)^{1/2}$在$E$上连续。自从
$$
f_2 - f_1 = \Phi_{v_2} + \Phi_{v_1} - 2\Phi,
$$
我们结论知道$x \mapsto \Phi(x, x)$是$E$上的连续函数，并且通过公式（19）和（20），$\Phi$在$E \times E$上连续。因而，存在$\mathscr{H}(E)$的(V，p. 16，cor.2)元素$u_0$使得$\Phi = \Phi_{u_0}$。显然满足公式(18)，因而$u_0$是$\mathscr{H}(E)$中$\mathscr{F}$的上界。这就证明了(i)。

我们已经，到构造
$$
\lim_{u,\Sigma} \langle x|(u_0 - u)(x)\rangle = 0 \quad \text{for all } x \in E.
$$
让$v_1 \in \mathscr{F}$；给定一个$u \in \mathscr{F}$使得$u \geq v_1$，让$v = u_0 - u$。如果我们将柯西-施瓦茨不等式应用于$E$上的正厄米特形式$\Phi_v$，我们得到
$$
\begin{align*}
\|v(x)\|^4 &= |\Phi_v(v(x), x)|^2 \leq \Phi_v(v(x), v(x)) \cdot \Phi_v(x, x) \\
&= \langle v(x)|v^2(x)\rangle \langle x|v(x)\rangle \leq \|v\|^3 \|x\|^2 \langle x|v(x)\rangle \\
&\leq \|u_0 - v_1\|^3 \|x\|^2 \langle x|v(x)\rangle,
\end{align*}
$$
从 $\|v\| \leq \|u_0 - v_1\|$ 到 V、p. 44，道具。 9. 然后通过(21)我们得到所有$x \in E$的$\lim_{u,\Sigma} \|(u_0 - u)(x)\| = 0$；这就证明了断言 (ii)。

特别是，道具。 13可以应用于递增和$\mathscr{H}(E)$的元素有界序列$(u_n)_{n \in \mathbf{N}}$的情况。那么存在$\mathscr{H}(E)$的元素$v$，其特征为
$$
\langle x|v(x)\rangle = \lim_{n \to \infty} \langle x|u_n(x)\rangle = \sup_{n \in \mathbf{N}} \langle x|u_n(x)\rangle \quad (x \in E),
$$
我们为所有 $x \in E$ 提供了 $v(x) = \lim_{n \to \infty} u_n(x)$。另外，$v$是$\mathscr{H}(E)$中的$u_n$的集合上界。

### 6. 自同态的痕迹

令 E 和 F 为两个希尔伯特空间。根据V、p. 40的约定，我们设$ba^*$，对于E中的$a$和F中的$b$，表示从E到F的连续线性映射$x \mapsto b \langle a|x \rangle$。

#### 引理 1 {#evt-v-s4-lem-1 .statement tag=081M}

*从E到F的所有有限秩连续线性映射中，存在从向量空间$F \otimes E'$到空间$\mathscr{L}_f(E; F)$的同构$\theta$，其特征为$a \in E, b \in F$为$\theta(b \otimes a^*) = ba^*$。

由A，II, § 4, No. 2，存在从$F \otimes E'$到$\mathscr{L}(E; F)$的单射线性映射$\theta$，并且只有一个这样的单射，其中变换$b \otimes a'$到线性映射$x \mapsto ba'(x)$对于$a' \in E', b \in F$。显然$\theta(b \otimes a^*) = ba^*$，$\theta$中的像包含在$\mathscr{L}_f(E; F)$中。然而，令$u \in \mathscr{L}_f(E; F)$和$(e_1, ..., e_n)$为F中$u$的像的正交基。令$f_i = u^*(e_i)$代表$1 \leq i \leq n$。对于每$x \in E$，我们有

$$
u(x) = \sum_{i=1}^n \langle e_i|u(x) \rangle \cdot e_i = \sum_{i=1}^n \langle f_i|x \rangle \cdot e_i,
$$

因此$u = \sum_{i=1}^n e_i f_i^* = \theta(\sum_{i=1}^n e_i \otimes f_i^*)$。因此$\theta$的像等于$\mathscr{L}_f(E; F)$。

从今以后，我们将假设$E = F$，并且我们集合$\mathscr{L}_f(E) = \mathscr{L}_f(E; E)$。到引理 1，$\mathscr{L}_f(E)$上存在唯一的线性形式$\tau$，使得$\tau(\theta(a \otimes a')) = a'(a)$对应$a \in E, a' \in E'$；在其他字中，我们有

(22)
$$
\tau(ba^*) = \langle a|b \rangle \quad \text{for } a, b \text{ in } E.
$$

当 E 是有限维时，我们有 $\mathscr{L}_f(E) = \mathscr{L}(E)$，$\tau(u)$ 是 E (A, II, § 4, No. 3) 自同态 $u$ 的*迹*。

#### 引理 2 {#evt-v-s4-lem-2 .statement tag=081N}

*令 $(e_i)_{i \in I}$ 为 E 的正交基。那么*

$$
\tau(u) = \sum_{i \in I} \langle e_i|u(e_i) \rangle
$$

*对于所有人*$u \in \mathscr{L}_f(E)$。

考虑E中$u = ba^*$和$a, b$的情况就足够了。那么

$$
\langle e_i|u(e_i) \rangle = e_i^* b \cdot a^* e_i = \overline{\langle e_i|a \rangle} \langle e_i|b \rangle
$$

引理2由V、p. 22的公式(22)和公式(3)推出。

#### 引理 3 {#evt-v-s4-lem-3 .statement tag=081O}

*令 u 为 E 的连续且正的自同态，以及 E 上所有有限秩正射投影的 $\mathscr{F}$ 集合。那么对于 E 的每个正交法线基 $(e_i)_{i \in I}$，我们有（在 $\mathbf{R}_+$ 中）等式*

$$
\sum_{i \in I} \langle e_i|u(e_i) \rangle = \sup_{p \in \mathscr{F}} \tau(pup).
$$

对于I的每个有限子集 J，放入$p_J = \sum_{i \in J} e_i e_i^*$；这是由向量 $e_i$ 生成的从 E 到向量子空间的正射投影，其中 i 的范围大于 J。我们有
$$
p_J u p_J = \sum_{i \in J, j \in J} \langle e_i | u(e_j) \rangle e_i e_j^* ,
$$
因此$\tau(p_J u p_J) = \sum_{i \in J} \langle e_i | u(e_i) \rangle$。从$p_J \in \mathscr{F}$开始，
$$
\sum_{i \in J} \langle e_i | u(e_i) \rangle \leq \sup_{p \in \mathscr{F}} \tau(p u p) ;
$$
所以我们结论
$$
\sum_{i \in I} \langle e_i | u(e_i) \rangle = \sup_J \sum_{i \in J} \langle e_i | u(e_i) \rangle \leq \sup_{p \in \mathscr{F}} \tau(p u p) .
$$

令$v$为有限秩连续且E的正自同态，并令$p \in \mathscr{F}$。到了。 2 of V, p. 23 存在 E 的正交基 $(f_\alpha)_{\alpha \in A}$ 和 A 的有限子集 B，使得 $(f_\alpha)_{\alpha \in B}$ 是 p 的像的正交基。然后我们有$p = \sum_{\alpha \in B} f_\alpha f_\alpha^*$，所以，如上所述，关系$\tau(p v p) = \sum_{\alpha \in B} \langle f_\alpha | v(f_\alpha) \rangle$。到引理 2 (V, p. 48) 我们有 $\tau(v) = \sum_{\alpha \in A} \langle f_\alpha | v(f_\alpha) \rangle$，这给出公式
$$
\sum_{\alpha \in B} \langle f_\alpha | v(f_\alpha) \rangle \leq \tau(v) .
$$
应用这个不等式对于$v = p_J . u p_J$且J是I的有限子集的情况，我们得到
$$
\sum_{\alpha \in B} \langle p_J(f_\alpha) | u p_J(f_\alpha) \rangle \leq \sum_{i \in J} \langle e_i | u(e_i) \rangle .
$$
对于每个$x \in E$，我们有$p_J(x) = \sum_{i \in J} \langle e_i | x \rangle e_i$，因此对于I的有限子集J的有序有向集合，我们有$x = \lim_J p_J(x)$。在(23)中的J上经过到极限，我们得到
$$
\tau(p u p) = \sum_{\alpha \in B} \langle f_\alpha | u(f_\alpha) \rangle \leq \sum_{i \in I} \langle e_i | u(e_i) \rangle ,
$$
这样就完成了引理 3 中的证明。

#### 定义 7 {#evt-v-s4-def-7 .statement tag=081P}

*设 u 为希尔伯特空间 E 的连续正自同态。设*
$$
\operatorname{Tr}(u) = \sup_{p \in \mathscr{F}} \tau(p u p)
$$
*（$\overline{\mathbf{R}}_+$中的上界），其中$\mathscr{F}$是E上所有有限秩正射投影仪的集合。我们说$\operatorname{Tr}(u)$是u的迹。*

令 $p$ 为从 $E$ 到 $E$ 的有限维向量子空间的正射投影，并令 $(x_1, ..., x_m)$ 为 $F$ 的标准正交基。我们设立了关系
$$
\tau(pup) = \sum_{i=1}^m \langle x_i | u(x_i) \rangle.
$$
因而，我们可以定义追踪公式
$$
\text{Tr}(u) = \sup_{x_1, ..., x_m} \sum_{i=1}^m \langle x_i | u(x_i) \rangle,
$$
其中$(x_1, ..., x_m)$的范围超过$E$的向量的所有有限正交序列的集合。

到引理 3 (V, p. 48)，我们有
$$
\text{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle
$$
对于 $E$ 的每个正交基 $(e_i)_{i \in I}$。由此，我们推论
$$
\text{Tr}(u + v) = \text{Tr}(u) + \text{Tr}(v)
$$
$$
\text{Tr}(\lambda u) = \lambda \cdot \text{Tr}(u)
$$
对于$E$的所有连续且正的自同态$u$和$v$以及每个实数$\lambda \geq 0$（我们在（27）中制定约定$0.(+\infty) = 0$）。设 $\phi$ 为同构，从 $E$ 到希尔伯特空间 $F$；由于 $\phi$ 变换 $E$ 的每个正交基变为 $F$ 的正交基，我们从 (25) 得到
$$
\text{Tr}(\phi u \phi^{-1}) = \text{Tr}(u).
$$

设$(u_\alpha)_{\alpha \in A}$是$E$的非空有向递增和连续且正自同态的有界族；让$u = \sup_\alpha u_\alpha$，然后$\langle x | u(x) \rangle = \sup_\alpha \langle x | u_\alpha(x) \rangle$对于所有$x \in E$（V，p. 46，道具13）。我们有$\text{Tr}(u) = \sup_{J \subset I} \sum_{i \in J} \langle e_i | u(e_i) \rangle$，其中$J$范围涵盖$I$的所有有限子集，因而
$$
\text{Tr}(u) = \sup_\alpha \text{Tr}(u_\alpha) \quad \text{for} \quad u = \sup_\alpha u_\alpha.
$$

令 $p_F$ 为从 $E$ 到希尔伯特子空间 $F$ 的正射投影；存在 $E$ 的正交基 $(e_i)_{i \in I}$ 和 $I$ 的子集 $J$，使得 $(e_i)_{i \in J}$ 是 $F$ 的正交基。我们有$\text{Tr}(p_F up_F) = \sum_{i \in J} \langle e_i | u(e_i) \rangle$。这个公式有两个推论：首先，我们有$\text{Tr}(p_F up_F) \leq \text{Tr}(u)$；其次，取$u = 1_E$，我们得到
$$
\text{Tr}(p_F) = \begin{cases}
\dim F & \text{if } F \text{ is finite dimensional} \\
+ \infty & \text{if not}.
\end{cases}
$$

#### 定义 8 {#evt-v-s4-def-8 .statement tag=081Q}

— 令 E 为复希尔伯特空间。 We write $\mathscr{L}^1(E)$ for the vector subspace of $\mathscr{L}(E)$ generated by all continuous, positive endomorphisms of E with finite trace.

通过V、p. 50的公式 (25)，在$\mathscr{L}^1(E)$上追踪扩展到线性形式，再次用Tr表示，并且满足关系$\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle$对于所有$u$ $\mathscr{L}^1(E)$ 以及对于 E 的每个正交基 $(e_i)_{i \in I}$。对于每个 $u \in \mathscr{L}^1(E)$，我们有 $u^* \in \mathscr{L}^1(E)$ 和 $\operatorname{Tr}(u^*) = \overline{\operatorname{Tr}(u)}$。 V的公式(28)，p. 50扩展到$u$属于到$\mathscr{L}^1(E)$的情况。设 F 是 E 的希尔伯特子空间；通过公式 (30)，正射投影$p_F$ 属于到 $\mathscr{L}^1(E)$ 当且仅当 F 是有限维时。对于E中的每个$a$和$b$，我们有$4ab^* = \sum_{\varepsilon^4 = 1} \varepsilon(a + \varepsilon b)(a + \varepsilon b)^*$和$cc^*$是一个对所有$c \in E$具有有限迹的正算子；因而，如果$u$是有限秩，E的连续自同态，则$u \in \mathscr{L}^1(E)$和$\operatorname{Tr}(u) = \tau(u)$。

令 E 为实希尔伯特空间，并令 $E_{(c)}$ 为其复化（V，p. 5）。我们认同 E 与子集 $E_{(c)}$。然后$\mathscr{L}(E)$可以被识别为从$E_{(c)}$到$E_{(c)}$的所有连续线性映射$u$的$\mathscr{L}(E_{(c)})$由……组成的真实向量子空间，使得$u(E) \subset E$。在这种情况下，我们写 $\mathscr{L}^1(E) = \mathscr{L}(E) \cap \mathscr{L}^1(E_{(c)})$。对于每个 $u \in \mathscr{L}^1(E)$，迹 $\operatorname{Tr}(u)$ 是实数并且等于 $\operatorname{Tr}(u^*)$。 公式（25）和（28）再次有效，$\mathscr{L}_f(E) \subset \mathscr{L}^1(E)$和$\operatorname{Tr}(u) = \tau(u)$对于所有$u \in \mathscr{L}_f(E)$。最后，E 的闭向量子空间 F 是有限维的当且仅当 $p_F$ 属于到 $\mathscr{L}^1(E)$。

\* 注 1. — 我们稍后将核映射的定义概念从Banach空间E变成Banach空间F。我们将证明，当$\mathscr{L}^1(E)$由从E到E的所有核映射组成时，则E是实数或复数希尔伯特空间。 \*

#### 命题 14 {#evt-v-s4-prop-14 .statement tag=081R}

— 令$E_1, ..., E_n$为希尔伯特空间、$E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$和$u_i$，对于$1 \leq i \leq n$，$E_i$的连续自同态。如果 $u_1, ..., u_n$ 为正，则 $u = u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$ 也为正，并且

$$
\operatorname{Tr}(u) = \prod_{i=1}^n \operatorname{Tr}(u_i).
$$

如果 $u_i \in \mathscr{L}^1(E_i)$ 对于所有 $1 \leq i \leq n$，则 $u \in \mathscr{L}^1(E)$ 和公式 (31) 在这种情况下再次有效。

于$n$由归纳出发，立即约化前往案件$n = 2$。

对于$i = 1, 2$，我们在$E_i$上通过公式$\Phi_i(x, y) = \langle x | u_i(y) \rangle$对$E_i$中的$x, y$进行定义倍半线性形式$\Phi_i$。如果 $u_1$ 和 $u_2$ 为正，则形式 $\Phi_1$ 和 $\Phi_2$ 为厄米特且为正。通过道具。 V、p. 25 中的 1 个在向量空间 $E_1 \otimes E_2$ 上存在正厄米特形式 $\Phi$，使得

$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = \Phi_1(x_1, y_1) \cdot \Phi_2(x_2, y_2)
$$

对于$E_1$中的$x_1, y_1$和$E_2$中的$x_2, y_2$。我们立即验证$E_1 \otimes E_2$中的$z$和$t$的关系$\Phi(z, t) = \langle z | u(t) \rangle$。由于 $\Phi$ 是正数，因此对于 $E_1 \otimes E_2$ 中的所有 $z$，我们都有 $\langle z | u(z) \rangle \geq 0$。由于$u$是连续的，并且$E_1 \otimes E_2$在希尔伯特空间$E = E_1 \hat{\otimes}_2 E_2$中是稠密的，所以我们结论认为$u$是E的连续且正的自同态。

令 $(e_i)_{i \in I}$ 为 $E_1$ 的标准正交基，且 $(f_j)_{j \in J}$ 为 $E_2$ 的标准正交基；那么族 $(e_i \otimes f_j)_{i \in I, j \in J}$ 是 $E$ 的正交基并且我们有

$$
\operatorname{Tr}(u) = \sum_{i \in I} \sum_{j \in J} \langle e_i \otimes f_j | u(e_i \otimes f_j) \rangle \\
= \sum_{i \in I} \sum_{j \in J} \langle e_i | u_1(e_i) \rangle \cdot \langle f_j | u_2(f_j) \rangle \\
= \operatorname{Tr}(u_1) \cdot \operatorname{Tr}(u_2) .
$$

特别是，如果$u_1$和$u_2$是有限迹的正自同态，那么$u$也是如此。通过线性，我们推导出当$K = \mathbf{C}$时，$u$属于到$\mathscr{L}^1(E)$，对于$i = 1, 2$，$u_i$属于到$\mathscr{L}^1(E_i)$； 公式 (31) 扩展对于这种情况，通过线性关系。最后，当 $K = \mathbf{R}$ 和 $u_i \in \mathscr{L}^1(E_i)$ 约化到复杂情况乘以标量的扩张时。

#### 注 2 {#evt-v-s4-n6-rem-2 .statement tag=081S}

— 令$E$为希尔伯特空间，它是希尔伯特子空间的族$(E_i)_{i \in I}$的希尔伯特和。令$u$为$\mathscr{L}(E)$的元素，使得$u(E_i) \subset E_i$对于所有$i \in I$；令$u_i$为$\mathscr{L}(E_i)$的元素，其中重合与$u$在$E_i$上。那么当$u$为正时$\operatorname{Tr}(u) = \sum_{i \in I} \operatorname{Tr}(u_i)$，或者属于到$\mathscr{L}^1(E)$；这个关系源自V的公式(25)，p. 50应用于$E$的正交基，它是每个$E_i$的正交基的并。

### 7. 希尔伯特-施密特映射

#### 定义 9 {#evt-v-s4-def-9 .statement tag=081T}

*令$E$和$F$为两个希尔伯特空间。如果 $E$ 的正自同态 $u^*u$ 的迹是有限的，则从 $E$ 到 $F$ 的连续线性映射 $u$ 称为 Hilbert-Schmidt 映射。从 $E$ 到 $F$ 的所有 Hilbert-Schmidt 映射的集合表示为 $\mathscr{L}^2(E, F)$。*

当$E = F$时，我们将$\mathscr{L}^2(E; E)$写为$\mathscr{L}^2(E)$。

对于每个$u \in \mathscr{L}(E, F)$，令$\|u\|_2 = \operatorname{Tr}(u^*u)^{1/2}$，使得$u$属于到$\mathscr{L}^2(E; F)$当且仅当$\|u\|_2$是有限的。根据迹线的定义，我们得到

$$
\|u\|_2^2 = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \|u(x_i)\|^2
$$

其中$(x_1, \ldots, x_m)$的范围超过$E$中有限正交序列的集合。特别是，在公式 (32) 中取 $m = 1$，我们有

$$
\|u\| \leq \|u\|_2 \quad (u \in \mathscr{L}(E; F)) .
$$

令 $(e_i)_{i \in I}$ 为 $E$ 的标准正交基，并且 $(f_j)_{j \in J}$ 为 $F$ 的标准正交基。通过V、p. 50的公式(25)和帕塞瓦尔的关系(V、p. 22)，我们有

$$
\|u\|_2^2 = \sum_{i \in I} \|u(e_i)\|^2 = \sum_{i,j} |\langle f_j | u(e_i) \rangle|^2 .
$$

由于 $|\langle f_j|u(e_i)\rangle| = |\langle e_i|u^*(f_j)\rangle|$，公式 (34) 意味着
$$
\|u^*\|_2 = \|u\| ;
$$
因此，Hilbert-Schmidt 映射的伴随物是 Hilbert-Schmidt 映射。令$E_1, F_1$为希尔伯特空间且$v : E_1 \to E, w : F \to F_1$连续线性映射。从(32)我们立即推断出
$$
\|wu\|_2 \leq \|w\|.\|u\|_2 .
$$
由 (35), (36) 和关系 $uv = (v^*u^*)^*$，我们得到
$$
\|uv\|_2 \leq \|u\|_2\,\|v\| .
$$
特别是，如果$u$属于到$\mathscr{L}^2(E, F)$，则$wuv$属于到$\mathscr{L}^2(E_1, F_1)$。

#### 定理 1 {#evt-v-s4-thm-1 .statement tag=081U}

*设 E 和 F 为两个希尔伯特空间。*
(i) *集合$\mathscr{L}^2(E, F)$是$\mathscr{L}(E; F)$的向量子空间，$u \mapsto \|u\|_2$是希尔伯范数*（V，p. 6）*在$\mathscr{L}^2(E; F)$上。*
(ii) *同构$\theta$从$F \otimes E'$到$\mathscr{L}_f(E; F)$，其特征在于从$F \otimes_2 E'$到$\mathscr{L}^2(E; F)$的$\theta(y \otimes x^*) = yx^*$扩展到同构$\hat{\theta}$。特别是，$\mathscr{L}_f(E; F)$在$\mathscr{L}^2(E; F)$中是稠密的。*

令$(e_i)_{i \in I}$（或$(f_j)_{j \in J}$）为$E$（或$F$）的正交基。对于每个$u \in \mathscr{L}(E; F)$，令$\Lambda(u)$为$u$的矩阵，相对于为$E$和$F$选择的正交基（V，p. 22）。让$\|a\|_2$表示希尔伯特空间$\ell^2(J \times I)$的元素$a$的范数。通过公式 (34)，$\Lambda$ 是映射，从 $\mathscr{L}^2(E; F)$ 变为 $\ell^2(J \times I)$，使得 $\|\Lambda(u)\|_2 = \|u\|$；显然 $\Lambda$ 是*内射*。为了证明 (i)，只需证明 $\Lambda$ 是*满射*即可。设$a = (a_{ji})$为$\ell^2(J \times I)$的元素；通过柯西-施瓦茨不等式，我们有
$$
|\sum_{j,i} \overline{\eta}_j a_{ji} \xi_i|^2 \leq \sum_{j,i} |a_{ji}|^2 \sum_{j,i} |\overline{\eta}_j \xi_i|^2 = \|a\|_2^2\,\|\xi\|^2\,\|\eta\|^2
$$
对于$\ell^2(I)$中的每个$\xi = (\xi_i)$和$\ell^2(J)$中的$\eta = (\eta_j)$。那么$F \times E$上存在连续倍半线性形式$\Phi$，使得$E$中的$x = \sum_i \xi_i e_i$有$\Phi(y, x) = \sum_{j,i} \overline{\eta}_j a_{ji} \xi_i$，$F$中的$y = \sum_j \eta_j f_j$。令 $u \in \mathscr{L}(E; F)$ 使得 $\Phi(y, x) = \langle y|u(x)\rangle$ (V, p. 16, cor. 2)。我们得到
$$
a_{ji} = \Phi(f_j, e_i) = \langle f_j|u(e_i)\rangle \quad \text{for} \quad i \in I, j \in J ,
$$
因此$a = \Lambda(u)$。

由于$\Lambda$是从$\mathscr{L}^2(E; F)$到$\ell^2(J \times I)$的希尔伯特空间同构，并且由于$(f_j \otimes e_i^*)$是$F \otimes_2 E'$的正交基，因此存在同构$\hat{\theta}$ $F \otimes_2 E'$ 到 $\mathscr{L}^2(E; F)$ 这样
$$
\langle f_j|\hat{\theta}(t)\,e_i\rangle = \langle f_j \otimes e_i^*|t\rangle
$$

对于每个$i \in I,\ j \in I$和$t \in F \otimes_2 E'$。特别是，对于$t = y \otimes x^*$，我们发现
$$
\langle f_j | \hat{\theta}(y \otimes x^*) e_i \rangle = \langle f_j \otimes e_i^* | y \otimes x^* \rangle = \langle f_j | y \rangle \langle x | e_i \rangle = \langle f_j | y x^* e_i \rangle
$$
因此$\hat{\theta}(y \otimes x^*) = y x^*$。这就证明了(ii)。 Q.E.D.

#### 例 1 {#evt-v-s4-n7-exa-1 .statement tag=081V}

令I和J为两个集合。由上面给出的证明，在阶中，从$\ell^2(I)$到$\ell^2(J)$的映射$u$是希尔伯特-施密特映射，在$\ell^2(J \times I)$中存在矩阵$(a_{ji})$是充分必要的，使得$u(\xi)_j = \sum_{i \in I} a_{ji} \xi_i$适用于$\ell^2(I)$中的所有$\xi = (\xi_i)$。

#### 例 2 {#evt-v-s4-n7-exa-2 .statement tag=081W}

\* 令X和Y为两个Hausdorff拓扑空间，分别赋予正测度$\mu$和$\nu$。 We can show that the Hilbert-Schmidt mappings from $\mathscr{L}^2(X)$ into $\mathscr{L}^2(Y)$ correspond bijectively to classes of square integrable functions on $Y \times X$; to the class of a function $N \in \mathscr{L}^2(Y \times X, \nu \otimes \mu)$ corresponds the mapping $u_N$ given by
$$
(u_N f)(y) = \int_X N(y, x) f(x) \, d\mu(x)
$$
for $\nu$-almost all $y \in Y$ and $f \in \mathscr{L}^2(X, \mu)$. 我们有
$$
\| u_N \|_2^2 = \int_X \int_Y |N(y, x)|^2 \, d\mu(x) \, d\nu(y) .
$$

#### 注 1 {#evt-v-s4-n7-rem-1 .statement tag=081X}

假设$K = \mathbf{C}$。设$u$和$v$在$\mathscr{L}^2(E; F)$中。我们有关系
$$
4\, u^* v = \sum_{\varepsilon^4 = 1} \overline{\varepsilon}(u + \varepsilon v)^* (u + \varepsilon v),
$$
因此$u^* v$属于到$\mathscr{L}^1(E)$。希尔伯特空间 $\mathscr{L}^2(E; F)$ 中的标量乘积由下式给出
$$
\langle u | v \rangle = \operatorname{Tr}(u^* v)
$$
从$\mathscr{L}^2(E; F)$上的公式定义厄米特形式开始，我们得到$\langle u | u \rangle = \| u \|_2^2$。

如果$u \in \mathscr{L}^2(E; F)$和$v \in \mathscr{L}^2(F; E)$，则通过前面的$vu$属于到$\mathscr{L}^1(E)$和$uv$到$\mathscr{L}^1(F)$；此外，我们还有
$$
\operatorname{Tr}(uv) = \operatorname{Tr}(vu) .
$$
通过线性和连续性，当$u = y_1 x_1^*$和$v = x_2 y_2^*$（E中$x_1, x_2$，F中$y_1, y_2$）时，足以验证这个公式；但$uv$是映射$y \mapsto y_1 \langle x_1 | x_2 \rangle \langle y_2 | y \rangle$和$vu$映射$x \mapsto x_2 \langle y_2 | y_1 \rangle \langle x_1 | x \rangle$，并且(41)由V、p. 48的公式(22)得出。

因而，如果$u_1, u_2$是$\mathscr{L}^2(E; F)$的两个元素，则在希尔伯特空间$\mathscr{L}^2(F; E)$中，我们有，
$$
\langle u_1^* | u_2^* \rangle = \operatorname{Tr}(u_1 u_2^*) = \operatorname{Tr}(u_2^* u_1) = \langle u_2 | u_1 \rangle = \overline{\langle u_1 | u_2 \rangle} ;
$$
在其他字中，$u \mapsto u^*$是从希尔伯特空间$\mathscr{L}^2(E; F)$到希尔伯特空间$\mathscr{L}^2(F; E)$的共轭（V，p. 6）的同构。如果我们将认同这个共轭与$\mathscr{L}^2(F; E)$的对偶（V，p. 15），我们看到$\mathscr{L}^2(E; F)$可以用$\mathscr{L}^2(F; E)$的对偶来识别，规范的双线性形式$(v, u) \mapsto \langle v, u \rangle$可以用$(v, u) \mapsto \operatorname{Tr}(vu)$来识别。

#### 注 2 {#evt-v-s4-n7-rem-2 .statement tag=081Y}

假设$K = \mathbf{R}$。我们留给读者验证公式（40）和（41）再次有效，并证明$\mathscr{L}^2(E; F)$可以通过双线性形式$(u, v) \mapsto \operatorname{Tr}(uv)$与$\mathscr{L}^2(F; E)$的对偶进行识别。

### 8. 希尔伯特-施密特映射的对角化

#### 定理 2 {#evt-v-s4-thm-2 .statement tag=081Z}

*设E和F是两个希尔伯特空间，u是从E到F的希尔伯特-施密特映射。存在E的正交基$(e_i)_{i \in I}$，它被u变换成F中的正交族。*

令 B 表示 E 的（闭合）单位球，并为其指定弱化的拓扑；这是紧凑型空间（V、p. 17）。我们为所有 $x \in B$ 放置 $Q(x) = \|u(x)\|^2$。最后让 P 表示 E 满足中所有向量 x 的集合以下性质 ；

(H) *对于每个与 x 正交的 $y \in E$，E 的元素 $u(y)$ 与 $u(x)$ 正交。*

#### 引理 4 {#evt-v-s4-lem-4 .statement tag=0820}

*函数$Q : B \to \mathbf{R}$是连续的。*

令 $(f_j)_{j \in J}$ 为 F 的正交基。对所有 $j \in J$ 放置 $\lambda_j = \|u^*(f_j)\|^2$。从 $u$ 属于到 $\mathscr{L}^2(E; F)$，我们有 $u^* \in \mathscr{L}^2(F; E)$，因此有 $\sum_j \lambda_j < +\infty$。进一步，我们有
$$
Q(x) = \|u(x)\|^2 = \sum_j |\langle u^*(f_j)|x \rangle|^2
$$
由 Parseval 的公式 (V, p. 22) 和伴随的定义 (V, p. 38)。对于每个$x \in B$，$|\langle u^*(f_j)|x \rangle|^2 \leq \lambda_j$，柯西-施瓦茨不等式；因而，公式 (43) 中和的收敛性在 B 上是一致的，因此引理 4 (GT, X, § 1, No. 6)。

#### 引理 5 {#evt-v-s4-lem-5 .statement tag=0821}

*设$E_1$为E的闭向量子空间，在$u^*u$下稳定。如果$E_1 \neq \{0\}$，则$E_1 \cap P$中存在范数 1 的向量。*

由于 B 是弱紧的，所以 B 的弱闭子空间 $B \cap E_1$ 也是弱紧的。因而，在 $B \cap E_1$ 中存在 (GT, IV, § 6, No. 1, th. 1) 点 $x_0$，使得对于所有 $x \in B \cap E_1$ 都有 $Q(x_0) \geq Q(x)$。如果 $Q(x_0) = 0$，我们就有 $Q(x) = 0$，因此所有 $x \in B \cap E_1$ 都有 $u(x) = 0$。因而，在这种情况下，$E_1 \subset P$ 和引理 5 如下。

现在假设$Q(x_0) > 0$，然​​后$x_0 \neq 0$。从向量$\|x_0\|^{-1} \cdot x_0$属于到$B \cap E_1$，我们有
$$
Q(x_0) \geq Q(\|x_0\|^{-1} \cdot x_0) = Q(x_0)/\|x_0\|^2
$$
*即*$\|x_0\| = 1$。我们要向P证明$x_0$属于；令 $y \in E$ 与 $x_0$ 正交。只要证明$u(y)$与$u(x_0)$正交就足够了。但由于$y$是$E_1$和向量的向量的和与$E_1$正交，并且都与$x_0$正交（自$x_0 \in E_1$开始），因此考虑以下两种情况就足够了：

a) $y$ 与 $E_1$ 正交：因为 $E_1$ 在 $u^*u$、$u^*u(x_0) \in E_1$ 下稳定，因此$0 = \langle y|u^*u(x_0)\rangle = \langle u(y)|u(x_0)\rangle$。

b) $y$ 属于至 $E_1$：对于所有 $t \in \mathbf{R}$、向量 $x(t) = (x_0 + ty)/\|x_0 + ty\|$ 属于至 $B \cap E_1$。我们有$Q(xt) = f(t)/g(t)$
$$
f(t) = \|u(x_0)\|^2 + 2t \Re \langle u(x_0)|u(y)\rangle + t^2 \|u(y)\|^2 \\
g(t) = 1 + t^2 \|y\|^2 .
$$
鉴于$x_0$的定义，对于所有实数$t$，我们有$Q(x(0)) \geq Q(x(t))$，因此$\frac{d}{dt} Q(x(t))$对于$t = 0$来说是零。但是$f(0) = \|u(x_0)\|^2$、$g(0) = 1$、$f'(0) = 2 \Re \langle u(x_0)|u(y)\rangle$、$g'(0) = 0$。自从
$$
\frac{d}{dt} Q(x(t)) = \frac{f'(t)\,g(t) - f(t)\,g'(t)}{g(t)^2},
$$
我们结论即$f'(0) = 0$，即$\Re \langle u(x_0)|u(y)\rangle = 0$。当$K = \mathbf{R}$、$u(x_0)$与$u(y)$正交时，当$K = \mathbf{C}$、向量$iy$属于与$E_1$正交且与$x_0$正交时，因此$\mathscr{I} \langle u(x_0)|u(y)\rangle = -\Re \langle u(x_0)|u(iy)\rangle = 0$，最后$u(x_0)$ 与 $u(y)$ 正交。这就证明了引理5。

现在我们证明。 2. 应用th。 S 的 1，III, § 4, No. 5 我们看到，正如在V，p. 23 中一样，存在集合 $S$，它是$P$ 中包含的$E$ 的正交子集中最大的。令$E_1$为与$S$正交的所有向量中的集合。设 $y \in E_1$；如果 $x \in S$、向量 $x$ 和 $y$ 是正交的，并且从 $S \subset P$ 开始，我们结论 $u(x)$ 和 $u(y)$ 是正交的；然后
$$
\langle x|u^*u(y)\rangle = \langle u(x)|u(y)\rangle = 0
$$
并且$u^*u(y)$与$S$正交。因此$E_1$在$u^*u$下是稳定的。如果我们有$E_1 \neq \{0\}$，则$E_1 \cap P$（引理 5）中将存在范数 1的向量$x$，$S \cup \{x\}$将是$P$中包含的$E$的正交子集。这与 $S$ 的最大值特征标相矛盾。因此 $E_1 = \{0\}$ 和 $S$ 是 $E$ 的正交基。 Q.E.D.

#### 推论 1 {#evt-v-s4-lem-5-cor-1 .statement tag=0822}

— *令 $v$ 为连续正数自同态，具有希尔伯特空间 $E$ 的有限迹。存在 $E$ 的正交基 $(e_i)_{i \in I}$ 和正实数 $(\lambda_i)_{i \in I}$ 的可求和族，使得对于所有 $i \in I$ 都有 $v(e_i) = \lambda_i e_i$。*

让$\Phi(x, y) = \langle x|v(y)\rangle$换成$E$中的$x, y$。那么$\Phi$是$E$上的正厄米特形式。存在（V，p. 8，推论）希尔伯特空间$F$和从$E$到$F$的连续线性映射$u$，使得$\Phi(x, y) = \langle u(x)|u(y)\rangle$对于$x, y$ $E$。在其他字中，我们有$v = u^*u$。凭借def。 9（V，p. 52），$u$是从$E$到$F$的希尔伯特-施密特映射。到了。 2、存在$E$的正交基$(e_i)_{i \in I}$使得向量$u(e_i)$是二乘二正交。让$i \in I$；对于$I$中的每个$j \neq i$，我们有
$$
\langle e_j|v(e_i)\rangle = \langle u(e_j)|u(e_i)\rangle = 0
$$

因此 $v(e_i)$ 与 $e_i$ 成比例，且为形式 $\lambda_i e_i$，其中 $\lambda_i = \langle e_i | v(e_i) \rangle$；那么

$$
\lambda_i \geqslant 0 \quad \text{and} \quad \sum_{i \in I} \lambda_i = \operatorname{Tr}(v) < + \infty .
$$

#### 推论 2 {#evt-v-s4-lem-5-cor-2 .statement tag=0823}

*设 E 为希尔伯特空间。然后$\mathscr{L}^1(E) \subset \mathscr{L}^2(E)$.*

真实情况约化通过标量扩张到复杂情况；因此我们可以假设$K = \mathbf{C}$。

由于$\mathscr{L}^2(E)$是$\mathscr{L}(E)$的向量子空间，因此足以证明E的每个连续且正的自同态$v$具有有限迹属于到$\mathscr{L}^2(E)$。与记号相关。 1、我们有

$$
\sum_{i \in I} \| v(e_i) \|^2 = \sum_{i \in I} \lambda_i^2 \leq (\sum_i \lambda_i)^2 < + \infty .
$$

#### 推论 3 {#evt-v-s4-lem-5-cor-3 .statement tag=0824}

*令 v 为具有有限迹的希尔伯特空间 E 的连续正自同态。 E 存在正 Hilbert-Schmidt 自同态 w，使得 $v = w^2$ 并且 v 与 w 交换。*

与记号相关。 1、将自同态w其中变换向量$\sum_{i \in I} \xi_i e_i$考虑为向量$\sum_i \lambda_i^{1/2} \xi_i e_i$就足够了。

#### 注 {#evt-v-s4-n8-rem-1 .statement tag=0825}

— 与记号的。 2、令J为所有$i \in I$中的集合，使得$u(e_i) \neq 0$。对于所有$i \in J$，令$\lambda_i = \| u(e_i) \|$和$f_i = \lambda_i^{-1} u(e_i)$。那么$(e_i)_{i \in J}$（或$(f_i)_{i \in J}$）是u的初始（或最终）子空间的正交基，我们对所有$i \in J$有$u(e_i) = \lambda_i f_i$，并且$\sum_{i \in J} \lambda_i^2 = \| u \|_2^2$是有限的。

### 9. 二次方形式相对于另一个的迹

在这个截面中，E表示实数向量空间，Q、H表示E上的两个*正二次形式*。$E \times E$上存在两个对称的双线性形式、$(x, y) \mapsto \langle x | y \rangle_Q$和$(x, y) \mapsto \langle x | y \rangle_H$，其特征为

$$
Q(x) = \langle x | x \rangle_Q , \quad H(x) = \langle x | x \rangle_H
$$

对于所有$x \in E$。

我们将 Q 相对于 H* 的迹称为 *trace，并写为 $\operatorname{Tr}(Q/H)$，一个实正数数，无论是否有限，定义如下：

*a)* 如果存在$x \in E$、$H(x) = 0$和$Q(x) \neq 0$，我们放入$\operatorname{Tr}(Q/H) = + \infty$。

*b)* 否则，$\operatorname{Tr}(Q/H)$是形式$\sum_{i=1}^m Q(x_i)$的所有数的集合上界，其中$(x_1, ..., x_m)$范围超过E的元素的有限序列集合，使得$\langle x_i | x_j \rangle_H = \delta_{ij}$（克罗内克符号）。

#### 注 {#evt-v-s4-n9-rem-1 .statement tag=0826}

— 1) 对于 E 的每个子空间 F，令 $Q_F$ 表示 Q 到 F 的限制和 H 的 $H_F$。我们有 $\operatorname{Tr}(Q_F/H_F) \leq \operatorname{Tr}(Q/H)$ 和 $\operatorname{Tr}(Q/H)$ 是所有数的集合的上界 $\operatorname{Tr}(Q_F/H_F)$，其中$F$涵盖$E$的所有有限维向量子空间族。

2) 令$E_1$为实向量空间、$Q_1$和$H_1$关于$E_1$的两个正二次形式和$\pi : E \to E_1$满射线性映射。如果$Q = Q_1 \circ \pi$和$H = H_1 \circ \pi$，则$\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1)$。

#### 命题 15 {#evt-v-s4-prop-15 .statement tag=0827}

*假设$E$上存在真正的希尔伯特空间结构，使得$H(x) = \|x\|^2$对于所有$x \in E$。为了使$\operatorname{Tr}(Q/H)$是有限的，存在一个连续且正的$E$的自同态$u$且具有有限迹是充分必要的，使得$Q(x) = \langle x|u(x)\rangle$对于所有$x \in E$；这个自同态 $u$ 是独一无二的，我们有*

$$
\operatorname{Tr}(u) = \operatorname{Tr}(Q/H) = \sum_{i \in I} Q(e_i)
$$

*对于 $E$ 的每个正交基 $(e_i)_{i \in I}$。*

假设 $\operatorname{Tr}(Q/H)$ 是有限的。对于范数 1 中的每一个 $x \in E$，我们有 $H(x) = 1$，因此有 $Q(x) \leq \operatorname{Tr}(Q/H)$。因而，$Q(x) \leq \operatorname{Tr}(Q/H) \cdot \|x\|^2$对于所有$x \in E$，并且

$$
|\langle x|y\rangle_Q| \leq Q(x)^{1/2} Q(y)^{1/2} \leq \operatorname{Tr}(Q/H) \cdot \|x\| \cdot \|y\|
$$

由柯西-施瓦茨不等式。因而，双线性形式$(x, y) \mapsto \langle x|y\rangle_Q$在$E \times E$上是连续的。存在(V,p. 16,cor.2)映射$u \in \mathscr{L}(E)$使得$\langle x|y\rangle_Q = \langle x|u(y)\rangle$。我们在$E$中有$x, y$对应$\langle x|y\rangle_Q = \langle y|x\rangle_Q$，因而$u$是厄米特；和 $\langle x|u(x)\rangle = Q(x) \geq 0$，因而 $u$ 为正。

相反，令$u$是$E$的连续且正的自同态，使得$Q(x) = \langle x|u(x)\rangle$对于所有$x \in E$。然后

$$
\langle x|u(y)\rangle = \frac{1}{2}(Q(x + y) - Q(x) - Q(y)) = \langle x|y\rangle_Q,
$$

给出唯一性或 $u$。到公式 (24') (V, p. 50)，我们得到

$$
\operatorname{Tr}(u) = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \langle x_i|u(x_i)\rangle = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m Q(x_i),
$$

其中$(x_1, \ldots, x_m)$的范围超过$E$的元素的所有有限正交序列的集合。通过$\operatorname{Tr}(Q/H)$的定义，我们得到$\operatorname{Tr}(u) = \operatorname{Tr}(Q/H)$。最后，对于$E$的每个正交基$(e_i)_{i \in I}$，我们有$\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i|u(e_i)\rangle$乘V的公式(25)，p. 50，因而$\operatorname{Tr}(u) = \sum_{i \in I} Q(e_i)$。

#### 注 3 {#evt-v-s4-n9-rem-3 .statement tag=0828}

令$E$和$F$是两个希尔伯特空间和$v$，从$E$到$F$是线性的，不一定是连续的映射。让$H(x) = \|x\|^2$和$Q(x) = \|v(x)\|^2$代表所有$x \in E$。它来自道具。 15 $v$ 是 Hilbert-Schmidt 映射当且仅当 $\operatorname{Tr}(Q/H)$ 是有限的，然后$\operatorname{Tr}(Q/H) = \|v\|_2^2$。

#### 注 4 {#evt-v-s4-n9-rem-4 .statement tag=0829}

假设 $E$ 是有限维的。当二次形式 $H$ 可逆时，道具。 15 适用。令$(e_1, \ldots, e_n)$为$E$的基。把$q_{ij} = \langle e_i|e_j\rangle_Q$和$h_{ij} = \langle e_i|e_j\rangle_H$引入矩阵$q = (q_{ij})$和$h = (h_{ij})$。令 $u$ 为 $E$ 的自同态，使得 $Q(x) = \langle x|u(x)\rangle_H$ 对于所有 $x \in E$。我们有

$$
\langle x|y\rangle_Q = \langle x|u(y)\rangle_H \quad (x, y \in E),
$$

因此，$u$的矩阵相对于E的基$(e_1, ..., e_n)$等于$h^{-1} q$。通过道具。 15、我们有

$$
\text{Tr}(Q/H) = \text{Tr}(h^{-1} q) = \text{Tr}(qh^{-1}) .
$$

如果基 $(e_1, ..., e_n)$ 对于 H 是正交的，则 $h$ 是阶 $n$ 的单位矩阵，我们得到

$$
\text{Tr}(Q/H) = \text{Tr}(q) = \sum_{i=1}^n Q(e_i) ;
$$

这样在这种情况下我们就得到公式 (44)。

现在假设二次形式 H 不可逆。令N为H的核，并令$\pi$为从E到E/N的典范映射。 E/N 上存在可逆二次方程形式 $H_1$，使得 $H = H_1 \circ \pi$。令 $(e_1, ..., e_n)$ 为 E 的元素的序列，使得序列 $(\pi(e_1), ..., \pi(e_m))$ 为 E/N 的基，它是 $H_1$ 的正交。令 $(e_1, ..., e_n)$ 为 N 的基。那么 $(e_1, ..., e_n)$ 为 E 的基，我们有

$$
H(\xi_1 e_1 + \cdots + \xi_n e_n) = \xi_1^2 + \cdots + \xi_m^2
$$

对于所有实数 $\xi_1, ..., \xi_n$。

假设对于所有$x \in E$，关系$H(x) = 0$蕴涵$Q(x) = 0$；在其他字中，假设E/N上存在二次形式$Q_1$使得$Q = Q_1 \circ \pi$。通过注 2 和道具。 15、我们有，

$$
\text{Tr}(Q/H) = Q(e_1) + \cdots + Q(e_m) .
$$

习题

### 习题 {#evt-v-s4-exercises}

参见[习题为 § 4](exercises/s4/)。
