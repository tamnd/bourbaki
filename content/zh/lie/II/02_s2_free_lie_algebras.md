---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 2
section_title: Free Lie algebras
lang: zh
source: lie-i-iii
book_pages: 122-136, 181-186
pdf_pages: 0140-0154, 0199-0204
extraction: ocr
subsections:
    - "no": 1
      title: REVISION OF FREE ALGEBRAS
      page: 122
      pdf_page: 140
    - "no": 2
      title: CONSTRUCTION OF THE FREE LIE ALGEBRA
      page: 122
      pdf_page: 140
    - "no": 3
      title: PRESENTATIONS OF A LIE ALGEBRA
      page: 124
      pdf_page: 142
    - "no": 4
      title: LIE POLYNOMIALS AND SUBSTITUTIONS
      page: 124
      pdf_page: 142
    - "no": 5
      title: FUNCTORIAL PROPERTIES
      page: 125
      pdf_page: 143
    - "no": 6
      title: GRADUATIONS
      page: 126
      pdf_page: 144
    - "no": 7
      title: LOWER CENTRAL SERIES
      page: 128
      pdf_page: 146
    - "no": 8
      title: DERIVATIONS OF FREE LIE ALGEBRAS
      page: 129
      pdf_page: 147
    - "no": 9
      title: ELIMINATION THEOREM
      page: 130
      pdf_page: 148
    - "no": 10
      title: HALL SETS IN A FREE MAGMA
      page: 132
      pdf_page: 150
    - "no": 11
      title: HALL BASES OF A FREE LIE ALGEBRA
      page: 134
      pdf_page: 152
statements: 32
exercises: 16
content_sha256: 9aec6dd04fcbdffb41f0c67ebba02754fe785c07c3540c14aacf443ac1c731c8
translated_from: content/en/lie/II/02_s2_free_lie_algebras.md
translation_method: google
source_content_sha256: ad0797e551cb1458568c1bb8b924dc5cc8828593371854e1c541a2937d5882cd
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 319b50b81b817360e2324c8859bdf7301258eafc1bc21f8bc1e88c7c0f07e4ec
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。免费李代数

### 1.免费代数的修订

令X为集合。回想一下在X（代数，章I, § 7, no. 1）上构造的自由岩浆M（X）的构造。在归纳整数 $n \geqslant 1$，我们通过写 $X_1 = X$ 并取 $X_n$ 为集合 $X_p \times X_{n-p}$ 和集合定义集合 $X_n$，其中$p = 1, 2, \ldots, n-1$；如果 X 是有限的，那么每个 $X_n$ 也是有限的。 $(X_n)_{n \geqslant 1}$族的和集合用M(X)表示；每个集合$X_n$（特别是X）都用M(X)的子集来标识。令w和$w'$在M(X)中；令 p 和 q 表示整数，使得 $w \in X_p$ 和 $w' \in X_q$ 并令 $n = p + q$； $X_p \times X_{n-p}$的典范嵌入下的有序对$(w, w')$的像进入$X_n$，记为$w.w'$，称为w和$w'$的乘积。 X的每个映射进入岩浆M都可以以独特的方式扩展到M（X）的岩浆同态进入M。

设w在M(X)中；唯一的整数 n，使得$w \in X_n$称为w的长度，并用$l(w)$表示。然后$l(w.w') = l(w) + l(w')$代表w，$w'$代表M(X)。 集合 X 是长度 M(X) 子集元素由……组成 1. 长度 $\geqslant 2$ 的每个元素 w 都可以唯一地写在形式中$w = w'.w''$。

系数为环K的岩浆M(X)的代数用Lib(X)表示，需要表示环K时则用Lib_K(X)表示。集合M(X)是基因此，K-模 Lib(X) 和X 将被识别为 Lib(X) 的子集。如果A是代数，则X的每个映射到A中都可以唯一扩展到Lib(X)的同态到A中(代数，章III, § 2, no. 7，命题7)。

### 2. 免费的构造李代数

#### 定义 1 {#lie-ii-s2-def-1 .statement tag=0A2Q}

*免费李代数除以集合X是商代数*
$$
L(X) = \mathrm{Lib}(X)/a,
$$
其中 a 是由形式之一的元素生成的 Lib(X) 的两侧理想
(1)
$$
Q(a) = a.a \quad \text{for } a \text{ in } \mathrm{Lib}(X),
$$
(2)
$$
J(a, b, c) = a.(b.c) + b.(c.a) + c.(a.b)
$$
对于$\mathrm{Lib}(X)$中的$a, b, c$。

显然$L(X)$是一个谎言K-代数； $L(X)$的两个元素$u, v$中的合成将由$[u, v]$表示。当需要注明环 K时，我们将$L(X)$写为$L_K(X)$。

下面的命题证明了给$L(X)$命名的*free*李代数是合理的。

#### 命题 1 {#lie-ii-s2-prop-1 .statement tag=0A2R}

*令$\psi$为Lib(X)的典范映射到$L(X)$和$\psi$到X的$\phi$限制。对于X到李代数$g$的每一个映射 f，存在且仅有一个同态 F：$L(X) \to g$，使得$f = F \circ \phi$。*

(a) *F*的存在性：设h是Lib(X)的同态延伸到$g$延伸f(no. 1)。对于 Lib(X) 中的所有$a$，$h(Q(a)) = h(a.a) = [h(a), h(a)] = 0$；类似地，$g$满足的雅可比恒等式意味着$h(J(a, b, c)) = 0$对应于Lib(X)中的$a, b, c$。由此可见，$h(a) = 0$，从而，$L(X)$有同态 F进入$g$，使得$h = F \circ \psi$。通过限制X，我们得到$f = F \circ \phi$。

(b) F*的*唯一性：令$F': L(X) \to g$为同态，使得$f = F' \circ \phi$。 Lib(X) 的同态 $F \circ \psi$ 和 $F' \circ \psi$ 转换为 X 上的 $g$ 重合，因此相等；因为 $\psi$ 是满射，$F = F'$。

#### 推论 1 {#lie-ii-s2-prop-1-cor-1 .statement tag=0A2S}

*家庭$(\phi(x))_{x \in X}$在$L(X)$中比K免费。*

令 $x_1, x_2, \ldots, x_n$ 不同于 X 的元素，且 $\lambda_1, \ldots, \lambda_n$ 不同于 K 的元素，使得

$$
\lambda_1 \cdot \phi(x_1) + \cdots + \lambda_n \cdot \phi(x_n) = 0.
$$

令 $g$ 为可交换的李代数，其中 K 作为底层模。对于$i = 1, 2, \ldots, n$，$L(X)$存在同态$F_i$到$g$，使得$F_i(\phi(x_i)) = 1$和$F_i(\phi(x)) = 0$对于$x \neq x_i$（命题1）； 应用$F_i$到关系（3），我们得到$\lambda_i = 0$。

#### 推论 2 {#lie-ii-s2-prop-1-cor-2 .statement tag=0A2T}

*令$a$为李代数。 $L(X)$ 到 $a$ 的每一个扩张都是无关紧要的。*

令$a \xrightarrow{\lambda} g \xrightarrow{\mu} L(X)$为扩张（章I, § 1, no. 7）。由于$\mu$是满射，因此存在X的映射 f进入$g$，使得$\phi = \mu \circ f$。令 F 为 $L(X)$ 到 $g$ 的同态，使得 $f = F \circ \phi$ (命题 1)。那么$(\mu \circ F) \circ \phi = \mu \circ f = \phi$和命题1表明$\mu \circ F$是$L(X)$的恒等式自同构。因此，给定的扩张是无关紧要的（章 I, § 1, no. 7、命题 6 和定义 6）。

由于环 K 不为零，推论 1 到命题 1 表明 $\phi$ 是单射的。 *因此集合X可以通过$\phi$与$L(X)$中的像来识别*；按照此约定，X 生成 $L(X)$ 以及 X 中的每个映射进入李代数 $g$ *可以扩展*至 $L(X)$ 中的李代数同态进入$g$。

#### 注 {#lie-ii-s2-n2-rem-1 .statement tag=0A2U}

当X为空时，$M(X)$为空，因此$L(X) = \{0\}$。如果X由单个元素$x$组成，则$L(X)$的子模$K.x$是子代数的谎言

L(X);如X生成L(X)，推论1到命题1表明L(X)与基{x}是自由模。

### 3. 李代数的展示

令g为李代数和$a = (a_i)_{i \in I}$g的元素族。令$f_a$为L(I)的同态转化为g映射，每个$i \in I$到$a_i$。 $f_a$的像是$a$生成的g的子代数； 元素、核、$f_a$被称为$a$家庭的*亲戚*。如果 $f_a$ 是满射（或单射、双射的），则族 $a$ 称为生成的（或自由、基本）。

设g为李代数。 g的*表示*是生成的家庭$a = (a_i)_{i \in I}$的有序对$(a, r)$由……组成和$a$生成的关系者的家庭$r = (r_j)_{j \in J}$L(I)核的理想$f_a$。我们还说 g 由关系者 $r_j$ ($j \in J$) 相关的家族 $a$ 呈现。

设I为集合，$r = (r_j)_{j \in J}$为自由李代数L（I）中的元素的家庭；设$a_r$为$r$生成的L(I)的理想。商代数$L(I, r) = L(I)/a_r$称为李代数，由I和关系族$(r_j)_{j \in J}$定义；我们还说 $L(I, r)$ 由表示 (I, r) 定义，或者也由 $(I; (r_j = 0)_{j \in J})$ 定义。当家里$r$空的时候，$L(I, r) = L(I)$。

令I和$r$如上；让$\xi_i$表示$L(I, r)$中$i$的像。 生成的家族$\xi = (\xi_i)_{i \in I}$和关系者家族$r$构成了$L(I, r)$的呈现。相反，如果 g 是李代数和 $(a, r)$，其中 $a = (a_i)_{i \in I}$ 是 g 的表示，则存在唯一的同构 $u : L(I, r) \to g$，使得对于所有 $i \in I$ 都有 $u(\xi_i) = a_i$。

### 4.李多项式和代换

令 I 为集合。令$T_i$表示L(I)中I的元素i的典范像（也用$L((T_i)_{i \in I})$表示有时）； L(I) 的元素被称为不定式$(T_i)_{i \in I}$ 中的*李多项式*。

设g为李代数。如果$t = (t_i)_{i \in I}$是g的元素族，则令$f_t$表示将L(I)的同态代入g，使得$f_t(T_i) = t_i$对于$i \in I$(no. 2，命题1)。 L(I)的元素P的$f_t$下的像用$P((t_i)_{i \in I})$表示。特别是$P((T_i)_{i \in I}) = P$；上面的元素$P((t_i)_{i \in I})$就是用$t_i$代替李多项式$P((T_i)_{i \in I})$中的$T_i$得到的有时称为g的元素。

设$\sigma : g \to g'$为李代数同态。对于g的元素的每个家庭$t = (t_i)_{i \in I}$和所有$P \in L(I)$，

$$
\sigma(P((t_i)_{i \in I})) = P((\sigma(t_i))_{i \in I}),
$$

$\sigma \circ f_t$ 映射 $T_i$ 至 $\sigma(t_i)$ $i \in I$。

令$(Q_j)_{j \in J}$为L(I)的元素的族，并令$P \in L(J)$。通过用 Q_j 代替 P 中的 T_j，我们得到李多项式 R = P((Q_j)_{j \in J}) \in L(I)。然后

(5)
$$
R((t_i)_{i \in I}) = P((Q_j((t_i)_{i \in I}))_{j \in J})
$$
对于李代数 g 的元素的每个家庭 $t = (t_i)_{i \in I}$，如通过对等式 $R = P((Q_j)_{j \in J})$ 操作同态 $f_t$ 并使用 (4) 可以看出。

令 g 为李代数、I、有限集合和 $P \in L(I)$。假设 g 是自由K-模。 映射
$$
\tilde{P} : g^I \to g
$$
由$\tilde{P}((t_i)_{i \in I}) = P((t_i)_{i \in I})$定义则为*多项式。*† 对于$g^I$的映射的集合 F到g中是李代数，其中括号由下式定义
$$
[\phi, \psi](t) = [\phi(t), \psi(t)];
$$
根据括号的双线性，$g^I$ 的多项式映射到 g 的集合 F' 是 F 的李子代数。然后，我们的断言可以从以下事实得出：对于所有i，映射$P \mapsto \tilde{P}$是李代数同态和$\tilde{T}_i = \mathrm{pr}_i \in F'$。

### 5. 函数属性

#### 命题 2 {#lie-ii-s2-prop-2 .statement tag=0A2V}

令X和Y为两个集合。每个映射$u : X \to Y$都可以唯一地扩展到李代数同态$L(u) : L(X) \to L(Y)$。对于每个映射 $v : Y \to Z$，$L(v \circ u) = L(v) \circ L(u)$。

$L(u)$的存在性和唯一性是从no. 2的命题1得出的。 同态 $L(v \circ u)$ 和 $L(v) \circ L(u)$ 具有相同的限制至 X，因此相等 (命题 1)。

#### 推论{#lie-ii-s2-n5-cor-1 .statement tag=0A2W}

如果 u 是单射（分别是满射、双射的），则 $L(u)$ 也是。

由于断言对于$X = \varnothing$来说是微不足道的，我们假设$X \neq \varnothing$。如果 u 是单射的，则存在 Y 的映射 v 进入 X，使得 $v \circ u$ 是 X 的恒等映射；通过命题 2，$L(v) \circ L(u)$ 是 $L(X)$ 的自同构的恒等式，因此 $L(u)$ 是单射的。当u是满射时，在X中存在Y的映射w，使得$u \circ w$是Y的恒等映射；那么$L(u) \circ L(w)$是$L(Y)$的恒等映射，这就证明$L(u)$是满射。

† 回忆一下自由模 M 的多项式映射的 (代数, 章 IV, § 5, no. 10) 定义到模 N：如果 q 是整数 $\geq 0$, 映射如果存在 $M^q$ 的多重线性映射 u 到 N 中，$f : M \to N$ 被称为 *次数* q 的齐次多项式，使得
$$
f(x) = u(x, \ldots, x) \quad \text{for all } x \in M.
$$
M 到 N 的映射被称为*多项式*，如果它是合适次数的齐次多项式映射的有限和。

令 X 为集合，且 S 子集为 X。上述推论表明，S 的典范嵌入到X可以扩展到$L(S)$的同构$\alpha$到S生成的$L(X)$的谎言子代数$L'(S)$上； *我们将认同*$L(S)$*和*$L'(S)$*通过*$\alpha$。

令$(S_\alpha)_{\alpha \in I}$是X的子集与并 S的*右有向族*。关系$S_\alpha \subset S_\beta$蕴含$L(S_\alpha) \subset L(S_\beta)$，因此$L(X)$的李子代数$L(S_\alpha)$族是正确的方向。因此$g = \bigcup_{\alpha \in I} L(S_\alpha)$是$L(X)$的谎言子代数；然后 $S \subset g$、从而 $L(S) \subset g$，以及对于所有 $\alpha \in I$、$g \subset L(S)$ 为 $L(S_\alpha) \subset L(S)$。因此

$$
L\left( \bigcup_{\alpha \in I} S_\alpha \right) = \bigcup_{\alpha \in I} L(S_\alpha)
$$

对于每个*正确定向*家庭$(S_\alpha)_{\alpha \in I}$子集X。

应用上述对于X的有限子集族，我们看到$L(X)$的每个元素都是形式$P(x_1, \ldots, x_n)$，其中P是n个不定数的李多项式，$x_1, \ldots, x_n$是元素 X。

#### 命题 3 {#lie-ii-s2-prop-3 .statement tag=0A2X}

*令$K'$为非零交换环和$u : K \to K'$环同态。对于每一个集合X，存在且仅有一个李$K'$-代数同态*

$$
v : L_K(X) \otimes K' \to L_{K'}(X)
$$

*这样*$v(x \otimes 1) = x$*对于*$x \in X$。 *此外，v是同构。*

将应用命题 1到$g = L_{K'}(X)$视为谎言K-代数和映射将X的$x \mapsto x$代入g，我们得到一个K-同态$L_K(X) \to L_{K'}(X)$，从而有一个$K'$-同态$v : L_K(X) \otimes K' \to L_{K'}(X)$。 v 是唯一且为同构的事实源自以下事实：有序对 $(L_K(X) \otimes K', x \mapsto x \otimes 1)$ 是与有序对 $(L_{K'}(X), x \mapsto x)$ 相同的普遍映射问题的解。

#### 注 {#lie-ii-s2-n5-rem-1 .statement tag=0A2Y}

令$\mathfrak{h}'$为李$K'$代数，$\mathfrak{h}$为李K-代数，通过限制标量环从$\mathfrak{h}'$导出。如果$P \in L_K(X)$，我们可以定义$\tilde{P} : \mathfrak{h}^X \to \mathfrak{h}$（no. 4）。我们立即看到

$$
\tilde{P} = (v(P \otimes 1))^{-}.
$$

### 6. 毕业

令 $\Delta$ 为可交换幺半群，可加写。让$\phi_0$表示将X的映射转化为$\Delta$和将游离岩浆$M(X)$转化为$\Delta$的$\phi$同态，其中扩展$\phi_0$。对于所有$\delta \in \Delta$，令$\mathrm{Lib}^\delta(X)$为$\mathrm{Lib}(X)$的子模，以及基子集$\phi^{-1}(\delta)$为$M(X)$。家人$(\mathrm{Lib}^\delta(X))_{\delta \in \Delta}$是代数$\mathrm{Lib}(X)$的毕业，也就是

$$
\mathrm{Lib}(X) = \bigoplus_{\delta \in \Delta} \mathrm{Lib}^\delta(X)
$$
$$
\mathrm{Lib}^\delta(X) \cdot \mathrm{Lib}^{\delta'}(X) \subset \mathrm{Lib}^{\delta + \delta'}(X) \quad \text{for } \delta, \delta' \text{ in } \Delta
$$

#### 引理 1 {#lie-ii-s2-lem-1 .statement tag=0A2Z}

定义 1 的理想$a$ 已分级。
对于 Lib(X) 中的$a, b$，设$B(a, b) = a.b + b.a$。 公式
$$
(10)\quad B(a, b) = Q(a + b) - Q(a) - Q(b)
$$
$$
(11)\quad Q(\lambda_1.w_1 + \cdots + \lambda_n.w_n) = \sum_i \lambda_i^2 Q(w_i) + \sum_{i < j} \lambda_i \lambda_j B(w_i, w_j)
$$
对于$M(X)$中的$w_1, \ldots, w_n$和$K$中的$\lambda_1, \ldots, \lambda_n$，表明族$(Q(a))_{a \in \mathrm{Lib}(X)}$和$(Q(w), B(w, w'))_{w, w' \in M(X)}$生成与$\mathrm{Lib}(X)$的子模相同。由于 J 是三线性的，理想的 $a$ 由齐次元素 $Q(w), B(w, w')$ 和 $J(w, w', w'')$ 生成，其中 $w, w', w''$ 在 $M(X)$ 中，因此被分级（代数、章 III, § 3, no. 3、命题） 1）。

让李代数 $L(X) = \mathrm{Lib}(X)/a$ 得到商分级。 次数 $\delta$ $L(X)$的齐次分量用$L^\delta(X)$表示；它是由元素$w \in M(X)$的像生成$L(X)$的子模，使得$\phi(w) = \delta$。

我们将特别利用以下两种情况：
(a) *总毕业*：我们对所有$x \in X$取$\Delta = \mathbf{N}$和$\phi_0(x) = 1$，右$M(X)$中的$w$取从而$\phi(w) = l(w)$。 K-模$L^n(X)$是由$M(X)$中长度$n$的像或元素生成，我们将其称为*次数n*的替代。稍后我们将看到模 $L^n(X)$ 是自由的，并且承认次数 $n$ (no. 11, 定理 1) 的交替项基由……组成。那么$L(X) = \bigoplus_{n \geq 1} L^n(X)$和$L^1(X)$承认$X$为基（no. 2，推论1到命题1）。截至 $M(X)$ 构造，
$$
(12)\quad L^n(X) = \sum_{p=1}^{n-1} [L^p(X), L^{n-p}(X)]
$$
特别是
$$
(13)\quad [L^m(X), L^n(X)] \subset L^{m+n}(X).
$$

(b) *多级化*：我们将$\Delta$视为在$X$上构造的自由交换幺半群$\mathbf{N}^{(X)}$。 $X$到$\Delta$的映射$\phi_0$由$(\phi_0(x))(x') = \delta_{xx'}$定义，其中$\delta_{xx'}$是克罗内克符号。对于$w \in M(X)$和$x \in X$，整数$(\phi(w))(x)$是“字母$x$在$w$中出现的第数”。对于$\mathbf{N}^{(X)}$中的$\alpha$，我们为$M(X)$中的所有$w$写为$|\alpha| = \sum_{x \in X} \alpha(x)$，从而$|\phi(w)| = l(w)$。由此可见
$$
(14)\quad L^n(X) = \bigoplus_{|\alpha|=n} L^\alpha(X);
$$
显然
$$
(15)\quad [L^\alpha(X), L^\beta(X)] \subset L^{\alpha+\beta}(X) \quad \text{for } \alpha, \beta \text{ in } \mathbf{N}^{(X)}.
$$

#### 命题 4 {#lie-ii-s2-prop-4 .statement tag=0A30}

令 S 为 X 的子集。如果 $\mathbf{N}^{(S)}$ 与 $\mathbf{N}^{(X)}$ 中的典范像进行识别（代数、章 I, § 7, no. 7），则$L(S) = \sum_{\alpha \in \mathbf{N}^{(S)}} L^\alpha(X)$。此外，对于所有$\alpha \in \mathbf{N}^{(S)}$，$L(S)$上的多级化下次数$\alpha$的齐次分量等于$L^\alpha(X)$。

让$\alpha \in \mathbf{N}^{(S)}$。 模$L^\alpha(S)$由$M(S)$中元素$w$的$L(X)$中的像生成，使得$\phi(w) = \alpha$，即(代数，§ 7, no. 9，公式(23)和(24)) $M(X)$ 中$w$的集合使得$\phi(w) = \alpha$。因此$L^\alpha(S) = L^\alpha(X)$。

由此得出命题和关系$L(S) = \sum_{\alpha \in \mathbf{N}^{(S)}} L^\alpha(S)$。

#### 推论{#lie-ii-s2-n6-cor-1 .statement tag=0A31}

对于$(S_i)_{i \in I}$子集X的每个家庭，
$$
L\left(\bigcap_{i \in I} S_i\right) = \bigcap_{i \in I} L(S_i).
$$
这是从命题 4 和明显的公式得出的
$$
\mathbf{N}^{(S)} = \bigcap_{i \in I} \mathbf{N}^{(S_i)}
$$
我们写了$S = \bigcap_{i \in I} S_i$。

### 7. 中下城级数

#### 命题 5 {#lie-ii-s2-prop-5 .statement tag=0A32}

令$g$为李代数，且$P$为$g$的子模。我们将$g$的定义子模$P_n$乘以公式$P_1 = P$，将$P_{n+1} = [P, P_n]$乘以$n \geq 1$。然后
$$
[P_m, P_n] \subset P_{m+n},
$$
$$
P_n = \sum_{p=1}^{n-1} [P_p, P_{n-p}] \quad \text{for } n \geq 2.
$$
我们通过$m$上的归纳证明(18)。案例$m = 1$是显而易见的。由雅可比恒等式，
$$
[[P, P_m], P_n] \subset [P_m, [P, P_n]] + [P, [P_m, P_n]],
$$
那就是
$$
[P_{m+1}, P_n] \subset [P_m, P_{n+1}] + [P, [P_m, P_n]].
$$
归纳假设意味着 $[P_m, P_{n+1}] \subset P_{m+n+1}$ 和 $[P_m, P_n] \subset P_{m+n}$、从而
$$
[P_{m+1}, P_n] \subset P_{m+n+1} + [P, P_{m+n}] = P_{m+n+1}.
$$
公式 (18)、$P_n \supset \sum_{p=1}^{n-1} [P_p, P_{n-p}] \supset [P_1, P_{n-1}] = P_n$、从而 (19)。

当我们取$P = g$时，序列$(P_n)$是$g$（章I, § 1, no. 5）的下中央级数（$\mathscr{C}^n g$）。因此：

#### 命题 6 {#lie-ii-s2-prop-6 .statement tag=0A33}

令$g$为李代数，$(\mathscr{C}^n g)_{n \geq 1}$为$g$的下中央级数。然后
$$
[\mathscr{C}^m g, \mathscr{C}^n g] \subset \mathscr{C}^{m+n} g \quad \text{for } m \geq 1 \text{ and } n \geq 1.
$$

推广章 I, § 4, no. 1 的定义 1，我们可以说，如果 $\mathscr{C}^n g = \{0\}$ 对于 $n$ 足够大，李代数 $g$ 是“幂零的”。 幂零李代数$g$的*幂零性类*为最小的整数$n$，使得$\mathscr{C}^{n+1} g = \{0\}$。

#### 命题 7 {#lie-ii-s2-prop-7 .statement tag=0A34}

Let $X$ be a set and $n$ an integer $\geq 1$.
(a) $L^{n+1}(X) = [L^1(X), L^n(X)]$.
(b) *The module* $L^n(X)$ *is generated by the elements* $[x_1, [x_2, \ldots, [x_{n-1}, x_n] \ldots]]$
*where* $(x_1, \ldots, x_n)$ *runs through the set of sequences of* $n$ *elements of* $X$.
(c) *The lower central series of* $L(X)$ *is given by* $\mathscr{C}^n(L(X)) = \sum_{p \geq n} L^p(X)$.

(a) 我们应用命题 5 与 $g = L(X)$ 和 $P = L^1(X)$。通过$n$上的归纳，我们从(12)(no. 6)和(19)等式$P_n = L^n(X)$推出。那么所需的关系就等于定义 $[P, P_n] = P_{n+1}$。
(b) 这是从 (a) 到 $n$ 的归纳得出的。
(c) 设$g = L(X)$和$g_n = \sum_{p \geq n} L_p(X)$。那么no. 6的$g = g_1$和公式(13)意味着$[g_n, g_m] \subset g_{n+m}$，特别是$[g, g_n] \subset g_{n+1}$。 $n$、$\mathscr{C}^n g \subset g_n$ 归纳之前。另一方面，从(a)我们在$n$上通过归纳推出$L^n(X) \subset \mathscr{C}^n g$。由于$\mathscr{C}^n g$是$g$的理想，关系$L^p(X) \subset \mathscr{C}^n g$意味着
$$
L^{p+1}(X) = [L^1(X), L^p(X)] \subset \mathscr{C}^n g
$$
由(a)。因此$L^p(X) \subset \mathscr{C}^n g$代表$p \geq n$，从而$g_n \subset \mathscr{C}^n g$。

#### 推论{#lie-ii-s2-n7-cor-1 .statement tag=0A35}

设$g$为李代数，$(x_i)_{i \in I}$生成的为$g$的族。 $g$的下中央级数的第$n$第项$\mathscr{C}^n g$是模，由$p \geq n$的迭代括号$[x_{i_1}, [x_{i_2}, \ldots, [x_{i_{p-1}}, x_{i_p}] \ldots]]$和$I$中的$i_1, \ldots, i_p$生成。
让$f$是$L(I)$到$g$的同态，这样$f(i) = x_i$对于所有$i \in I$。作为$(x_i)_{i \in I}$生成$g$、$g = f(L(I))$、从而$\mathscr{C}^n g = f(\mathscr{C}^n(L(I)))$乘以章I, § 1, no. 5的命题4。然后从命题 7 的断言 (b) 和 (c) 得出推论。

### 8. 推导免费李代数

#### 命题 8 {#lie-ii-s2-prop-8 .statement tag=0A36}

令$X$为集合，令$M$为$L(X)$模块，令$d$为$X$到$M$的映射。 $L(X)$到$M$延伸$d$和满足关系存在且仅有一个线性映射$D$：
$$
D([a, a']) = a.D(a') - a'.D(a) \quad \text{for } a, a' \text{ in } L(X).
$$
我们通过括号将定义李代数 $g$ 与底层模 $M \times L(X)$ 一起使用
$$
[(m, a), (m', a')] = (a.m' - a'.m, [a, a']),
$$

对于$L(X)$中的$a, a'$和$M$中的$m, m'$（章I, § 1, no. 8）。令$f$为$L(X)$到$g$的同态，使得$f(x) = (d(x), x)$对于$X$中的所有$x$；让$f(a) = (D(a), u(a))$代表$L(X)$中的所有$a$。通过公式 (21)，$u$ 等于 $L(X)$ 的同态自身；作为$X$中的$x$的$u(x) = x$，$u(a) = a$对于$L(X)$中的所有$a$，从而

$$(22)$$
$$f(a) = (D(a), a).$$

通过(21)和(22)，从$f([a, a']) = [f(a), f(a')]$得出关系(20)。

相反，令 $D'$ 为 $L(X)$ 的映射变成 $M$ 满足关系 (20') 类似于 (20) 并扩展 $d$。令 $f'(a) = (D'(a), a)$ 为 $a \in L(X)$；通过(20')和(21)，$f'$是$L(X)$到$g$的同态，与$X$、从而、$f' = f$和$D' = D$上的$f$重合。

#### 推论{#lie-ii-s2-n8-cor-1 .statement tag=0A37}

*$X$的每个映射到$L(X)$都可以唯一地扩展到$L(X)$的推导*。

当$M$等于$L(X)$且有伴随表示时，关系(20)意味着$D$是推导。

### 9. 消除定理

#### 命题 9 {#lie-ii-s2-prop-9 .statement tag=0A38}

*令$S_1$和$S_2$为$S_1 \times S_2$的两个不相交的集合和$d$映射到$L(S_2)$。令$g$为$L(S_1 \cup S_2)$与元素$[s_1, s_2] - d(s_1, s_2)$与$s_1 \in S_1, s_2 \in S_2$生成的理想的商李代数；设$\psi$是$L(S_1 \cup S_2)$的典范映射到$g$。

(a) *对于$i = 1, 2$，$\psi$至$S_i$的限制$\phi_i$可以扩展到$L(S_i)$的同构到$g$的子代数$a_i$。

(b) $g = a_1 + a_2, a_1 \cap a_2 = \{0\}$和$a_2$是$g$的理想。

对于$i = 1, 2$，让$\psi_i$表示$L(S_i)$的同态到$g$，其中扩展$\phi_i$和$a_i$其像。显然$\phi_i(S_i)$生成$a_i$。

设 $s_1 \in S_1$；我们写$D = \operatorname{ad} \phi_1(s_1)$。将 $g$ 映射 $\phi_2(S_2)$ 的推导 $D$ 转换为 $a_2$ by 关系

$$
[\phi_1(s_1), \phi_2(s_2)] = \psi_2(d(s_1, s_2)) \quad \text{for } s_2 \in S_2;
$$

由于$g$的子代数$a_2$是由$\phi_2(S_2)$生成的，因此$D(a_2) \subset a_2$。 $x \in g$的集合，使得$\operatorname{ad} x$留下$a_2$不变，是$g$的谎言子代数，通过上面的包含$\phi_1(S_1)$，因此也是$a_1$。因此

$$(23)$$
$$[a_1, a_2] \subset a_2.$$

因此$a_1 + a_2$是$g$的谎言子代数，并且，因为它包含生成的集合$\phi_1(S_1) \cup \phi_2(S_2)$，

$$(24)$$
$$a_1 + a_2 = g.$$

对于所有 $s_1 \in S_1$ 都存在推导 $D_{s_1}$ $L(S_2)$ 使得

$$
D_{s_1}(s_2) = d(s_1, s_2)
$$

对于$S_2$中的所有$s_2$（no. 8，命题8的推论）。 映射$s_1 \mapsto D_{s_1}$可以扩展到$L(S_1)$的同态$D$扩展为$L(S_2)$的推导李代数。令$\mathfrak{h}$为$L(S_1)$由$L(S_2)$相应的到$D$（章I, § 1, no. 8）的半直接乘积。由于模 $\mathfrak{h}$ 等于 $L(S_1) \times L(S_2)$，特别是

$$
[(s_1, 0), (0, s_2)] = (0, d(s_1, s_2))
$$

对于 $s_1 \in S_1$ 和 $s_2 \in S_2$。

从(25)我们将$g$的同态$f$的存在性推导到$\mathfrak{h}$，使得$s_1 \in S_1$和$s_2 \in S_2$有$f(\phi_1(s_1)) = (s_1, 0)$和$f(\phi_2(s_2)) = (0, s_2)$。我们立即推断关系

$$
f(\psi_1(a_1) + \psi_2(a_2)) = (a_1, a_2)
$$

对于 $a_1 \in L(S_1)$ 和 $a_2 \in L(S_2)$。

关系 (26) 表明$\psi_1$ 和$\psi_2$ 是单射的并且$a_1 \cap a_2 = \{0\}$。 公式 (23) 和 (24) 则意味着命题。

#### 命题 10（消除定理）{#lie-ii-s2-prop-10 .statement tag=0A39}

*设X为集合，X的S子集和序列$(s_1, \ldots, s_n, x)$的T集合，其中$n \geq 0, s_1, \ldots, s_n$在S中，x在X$- S.$*†

(a) *模$L(X)$是$L(X)$的子代数$L(S)$的直和和$X - S$生成的$L(X)$的理想$a$。*

(b) *存在$L(T)$到$a$的李代数同构$\phi$，其中映射$(s_1, \ldots, s_n, x)$到$(\operatorname{ad} s_1 \circ \cdots \circ \operatorname{ad} s_n)(x)$。*

令 $g$ 为李代数，如命题 9 所示构造

$$
S_1 = S, \quad S_2 = T, \quad d(s, t) = (s, s_1, \ldots, s_n, x) \in T \subset L(T)
$$

对于 T 中的 $t = (s_1, \ldots, s_n, x)$ 和 $s \in S_1$。我们认同$L(S)$和$L(T)$以及他们的典范像在$g$（命题9（a））。

令 $\psi$ 为 T 的映射 $(s_1, \ldots, s_n, x) \mapsto (\operatorname{ad} s_1 \circ \cdots \circ \operatorname{ad} s_n)(x)$ 到 $L(X)$ 中。显然对于$s \in S$和$t \in T$有$\psi(d(s, t)) = [s, \psi(t)]$，因此存在同态$\alpha : g \to L(X)$，其限制对S是恒等式，限制对T是$\psi$。现在$X - S \subset T$、从而还有同态$\beta : L(X) \to g$，其限制到$X = S \cup (X - S)$是恒等式。

我们证明$\alpha$是同构并且$\beta$逆同构。作为$X - S$中$x$的$\psi(x) = x$，我们看到$\alpha \circ \beta$重合在X、从而$\alpha \circ \beta = \mathrm{Id}_{L(X)}$上具有恒等式。另一方面，$[s, t] = d(s, t)$在$g$中，对于$s \in S, t \in T$乘以构造；由此可见，$t = (s_1, \ldots, s_n, x)$ 等于 $g$ 至 $(\operatorname{ad} s_1 \circ \cdots \circ \operatorname{ad} s_2)(x)$ 从而 $t = \beta(\alpha(t))$。如 $\beta(\alpha(s)) = s$ 对应 $s \in S$ 和 $S \cup T$ 生成 $g$、$\beta \circ \alpha = \mathrm{Id}_g$。

由于 $\alpha$ 是 $g$ 的同构到 $L(X)$，命题 9 表明限制

† 对于$n = 0$，我们获得$X - S$、从而 $X - S \subset T$ 中的元素。

$\alpha$到$L(T)$的化合是$L(T)$的同构$\phi$到$L(X)$的理想$b$，使得模$L(X)$是$L(S)$的直和并且$b$。显然
$$
\phi(s_1, \ldots, s_n, x) = (\mathrm{ad}\ s_1 \circ \cdots \circ \mathrm{ad}\ s_n)(x)
$$
$T$ 中的 $(s_1, \ldots, s_n, x)$。

因此$\phi(T) \subset a$，而$b \subset a$是从$L(X)$的$\phi(T)$生成子代数$b$开始。但$b$是一个理想值，$X - S \subset \phi(T) \subset b$、从而$a \subset b$。

#### 推论{#lie-ii-s2-n9-cor-1 .statement tag=0A3A}

*让$y \in X$。自由李代数$L(X)$是自由子模$K.y$和谎言子代数的直和，承认$((\mathrm{ad}\ y)^n, z)$的家庭为基本家庭，其中$n \geqslant 0$和$z \in X - \{y\}$。*

将$S = \{y\}$放入命题10就足够了。

### 10. 大厅集合在免费岩浆中

令$X$为集合、$M(X)$在$X$和$M^n(X)$上构建的自由岩浆，其中长度$n$$M(X)$元素$n \in \mathbf{N}^*$、集合(no. 1)。 如果$w \in M(X)$和$l(w) \geqslant 2$，令$\alpha(w)$和$\beta(w)$表示由关系$w = \alpha(w)\beta(w)$确定的$M(X)$的元素；然后$l(\alpha(w)) < l(w)$，$l(\beta(w)) < l(w)$。 最后，对于$M(X)$中的$u, v$，令$u^mv$表示由归纳在整数$m \geqslant 0$上由$u^0v = v$和$u^{m+1}v = u(u^mv)$定义的元素。

#### 定义 2 {#lie-ii-s2-def-2 .statement tag=0A3B}

*大厅集合相对于$X$为$M(X)$满足以下条件总共有序子集$H$：*
(A) *如果 $u \in H, v \in H$ 和 $l(u) < l(v)$，则 $u < v$。*
(B) *$X \subset H$和$H \cap M^2(X)$由乘积$xy$和$X$和$x < y$中的$x, y$组成。*
(C) *长度 $\geqslant 3$ 属于 $M(X)$ 的元素 $w$ 至 $H$ 当且仅当它是形式 $a(bc)$ 与 $a, b, c$ 时$H$、$bc \in H$、$b \leqslant a < bc$ 和 $b < c$。*

#### 命题 11 {#lie-ii-s2-prop-11 .statement tag=0A3C}

*相对于$X$存在一个大厅集合。*

我们将在整数$n$集合$H_n \subset M^n(X)$上构造到归纳以及集合的总订购：
(a) 我们写下$H_1 = X$并给它一个总排序。
(b) 集合 $H_2$ 由乘积 $xy$ 以及$X$ 和$x < y$ 中的$x, y$ 组成。我们给它一个总排序。
(c) 设$n \geqslant 3$使得全序集$H_1, \ldots, H_{n-1}$已经定义。 集合 $H'_{n-1} = H_1 \cup \cdots \cup H_{n-1}$ 的总排序为诱导 $H_1, \ldots, H_{n-1}$ 上给定的关系，并且如果 $l(w) < l(w')$ 则为 $w < w'$。我们定义$H_n$是乘积$a(bc) \in M^n(X)$的集合和$a, b, c$在$H'_{n-1}$满足关系$bc \in H'_{n-1}$，$b \leqslant a < bc$，$b < c$和给$H_n$一个总排序。

我们写$H = \bigcup_{n \geqslant 1} H_n$；我们给$H$这样定义的总排序：$w \leqslant w'$当且仅当$l(w) < l(w')$或$l(w) = l(w') = n$和$w \leqslant w'$在集合$H_n$中。 $H$相对于$X$来说是集合大厅，这是直接的。

对于X的每个子集 S，我们认同自由岩浆M(S)及其在M(X)中的典范像。

#### 命题 12 {#lie-ii-s2-prop-12 .statement tag=0A3D}

令H为相对于X的霍尔集合，并令x、y位于X中。
（一）$H \cap M(\{x\}) = \{x\}$。
(b) 假设$x < y$，并令$d_y$为$M(X)$的同态到$\mathbf{N}$，使得$d_y(y) = 1$和$d_y(z) = 0$对应于$z \in X, z \neq y$。 集合或元素 $w \in H \cap M(\{x, y\})$，使得 $d_y(w) = 1$ 由元素 $x^n y$ 和 n 整数 $\geq 0$ 组成。

定义 2 (B)、$x \in H$ 和 $H \cap M^2(\{x\}) = \varnothing$。如果$w \in H \cap M(\{x\})$，其中$n = l(w) \geq 3$、元素、$\alpha(w)$和$\beta(w)$也由属于到$H \cap M(\{x\})$乘以定义2 (C)。紧接着是$n$上的归纳，$H \cap M^n(\{x\}) = \varnothing$对$n \geq 2$、从而 (a)。

现在我们证明(b)。由定义 2 (B)、$y \in H$ 和 $xy \in H$。我们通过$n$上的归纳来显示$x^n y \in H$代表$n$整数$\geq 2$。现在$x^n y = x(x(x^{n-2}y))$和归纳假设意味着$x^{n-2}y \in H$。现在$l(x) < l(x^{n-2}y)$代表$n > 2$和$x < y$，在任何情况下从而$x < x^{n-2}y$； 定义2的条件(C)表明$x^n y \in H$。另一方面，当然是$d_y(x^n y) = 1$。相反，令$w \in H \cap M(\{x, y\})$，与$d_y(w) = 1$。如果$l(w) = 1$，则$w = y$；如果$l(w) = 2$，则$w = xy$乘以定义2 (B)。如果 $l(w) \geq 3$，则$w = a(bc)$，其中 $a, b, c, bc$ 位于 $H \cap M(\{x, y\})$ (定义 2 (C))。 $d_y(bc) = 0$ 是不可能的，因为这意味着 $bc \in M(\{x\})$，而 (a) 是不可能的。因此，通过 (a) 可得 $d_y(bc) = 1$ 和 $d_y(a) = 0$、从而 $a = x$。紧接着 $n = l(w)$ 上的归纳是$w = x^{n-1}y$，从而完成 (b) 的证明。

#### 推论{#lie-ii-s2-n10-cor-1 .statement tag=0A3E}

如果卡X$\geq 2$，则每整数$n \geq 1$对应$H \cap M^n(X) \neq \varnothing$。

#### 命题 13 {#lie-ii-s2-prop-13 .statement tag=0A3F}

令 X 为有限集合，且至少有两个元素。令 H 表示相对于 X 的霍尔集合。则H上存在$\mathbf{N}$的严格递增的双射$p \mapsto w_p$和H的子集的序列$(P_p)_{p \in \mathbf{N}}$，具有以下性质：
（一）$P_0 = X$。
(b) 对于每个整数 $p \geq 0$，$w_p \in P_p$。
(c) 对于每个整数$n \geq 1$，都存在整数$p(n)$，使得$P_p$的每个元素对于所有$p \geq p(n)$来说都是长度$> n$。
(d) 对于每个整数 $p \geq 0$，集合 $P_{p+1}$ 由元素或形式 $w_p^i w$ 组成，其中 $i \geq 0$、$w \in P_p$ 和 $w \neq w_p$。

由于X是有限的，集合$M^n(X)$都是有限的。让$H_n = H \cap M^n(X)$代表所有$n \geq 1$。 命题 12 的推论表明有限集合 $H_n$ 非空。令$u_n$为$H_n$的基数；让$v_0 = 0$和$v_n = u_1 + \cdots + u_n$代表$n \geq 1$。由于$H_n$是全序有限集合，因此$\mathbf{N}$到$H_n$的区间$[v_{n-1}, v_n - 1]$存在严格递增的双射$p \mapsto w_p$。 $p \mapsto w_p$是$\mathbf{N}$的严格递增的双射到H上是直接的。

令 $P_0 = X$ 且对于每个整数 $p \geq 1$ 令 $P_p$ 为 H 的元素 $w$ 的集合，使得 $w \geq w_p$，并且，$w \in X$ 或 $\alpha(w) < w_p$ (注如果$w$是长度$\geq 2$关系$w \in H$意味着$\alpha(w) \in H$乘条件（C）定义2）。然后$w_p \in P_p$；如果$w_p \in X$，并且当$w_p \notin X$时，从不等式$l(\alpha(w_p)) < l(w_p)$和条件（A）得出定义2，这是清楚的。

因此条件 (a) 和 (b) 满足。

令$n$为整数$\geq 1$并令$p \geq v_n$。对于所有 $w \in P_p, l(w) \geq l(w_p) > n$ 到定义的映射 $p \mapsto w_p$。这就成立了(c)。

我们现在显示形式$u = w_p^i w$中的每个元素与$i \geq 0, w \in P_p$和$w \neq w_p$属于到$P_{p+1}$。如果$i \neq 0$，则$l(u) > l(w_p)$、从而、$u > w_p$和$u \geq w_{p+1}$；然后$u \notin X$和$\alpha(u) = w_p < w_{p+1}$，从而$u \in P_{p+1}$。如果$i = 0$，则$u \in P_p$和$u \neq w_p$；然后$u > w_p$、从而$u \geq w_{p+1}$；如果$u$不属于到$X$，则$\alpha(w) < w_p$，从而$\alpha(w) < w_{p+1}$；然后又$u \in P_{p+1}$。

相反，让$u \in P_{p+1}$。我们区分两种情况：

(α) 不存在$M(X)$的元素$v$使得$u = w_p v$。截至 $P_{p+1}$、$u > w_p$ 定义。此外，如果$u \notin X$，则从$u \in P_{p+1}$起，通过给定的假设和$\alpha(u) < w_{p+1}$得到$\alpha(u) \neq w_p$；因此$\alpha(u) < w_p$。因此$u \in P_p$和$u \neq w_p$。

(β) $M(X)$中存在$v$使得$u = w_p v$。到定义 2，必然是$w_p \in X, v \in X$和$w_p < v$，或者$v \notin X$和$\alpha(v) \leq w_p < v$。无论哪种情况，$v \in P_{p+1}$。

那么存在$M(X)$的整数$i \geq 0$和元素$w$使得$u = w_p^i w$，以及$w \in X$或$w \notin X$和$\alpha(w) \neq w_p$。如果$i = 0$，我们有上面的情况(α)，从而$w \in P_p$和$w \neq w_p$。如果上述(β)的$i > 0$、证明成立，则在$i$、关系、$w \in P_{p+1}$、$w \neq w_p$上经过归纳。假设$w \notin X$；从$w \in P_{p+1}$可以得出$\alpha(w) \leq w_p$，而作为$\alpha(w) \neq w_p$，我们结论即$w \in P_p$。这就完成了(d)的证明。

#### 例 {#lie-ii-s2-n10-exa-1 .statement tag=0A3G}

假设$X$有两个元素$x, y$；让$X$被排序使得$x < y$。 命题 11 的证明给出的构造给出集合 $H$，以及长度 $\leq 5$ 的 14 个元素在下面的表中给出：

$$
\begin{array}{cccc}
H_1 & w_1 = x \\
H_2 & w_3 = (xy) \\
H_3 & w_4 = (x(xy)) & w_5 = (y(xy)) \\
H_4 & w_6 = (x(x(xy)))) & w_7 = (y(x(xy)))) & w_8 = (y(y(xy)))) \\
H_5 & w_9 = (x(x(x(xy)))) & w_{10} = (y(x(x(xy)))) & w_{11} = (y(y(x(xy))))) \\
& w_{12} = (y(y(y(xy)))) & w_{13} = ((xy)(x(xy))) & w_{14} = ((xy)(y(xy))).
\end{array}
$$

（$H$中的元素已根据每个$H_n$上选择的总顺序进行编号。）

### 11. 基免费李代数大厅

我们保留前面的记号。

#### 定理 1 {#lie-ii-s2-thm-1 .statement tag=0A3H}

令$H$为相对于$X$和$M(X)$的$\Psi$典范映射进入空闲李代数$L(X)$的大厅集合。 $\Psi$到$H$中的限制是模$L(X)$中的基。

对于$H$的每一个元素$w$，我们写$\bar{w} = \Psi(w)$。

(A) *$X$ 有限的情况。*

如果 $X$ 为空，则 $M(X)$ 也为空，因此 $H$ 和 $L(X)$ 为零。如果 $X$ 有一个元素 $x$，则 $H \cap M^n(X)$ 对于 $n \geq 2$ 是空的 (命题 12 (a))。因此，$H = \{x\}$；我们还知道（no. 2，*注*）模$L(X)$是免费的并且有基$\{\bar{x}\}$。因此，当$X$至多有一个元素时，定理为真。

假设此后$X$至少有两个元素； 选择序列 $(w_p)$ 和 $(P_p)$ 具有命题 13 中所述的属性。对于每个整数 $p \geq 0$，令 $L_p$ 表示由 $L(X)$ 生成的子模元素$\bar{w}_i$与$0 \leq i < p$和$g_p$是家庭$(\bar{u})_{u \in P_p}$产生的$L(X)$的谎言子代数。

#### 引理 2 {#lie-ii-s2-lem-2 .statement tag=0A3I}

*对于每个整数$p \geq 0$，模$L_p$将$(\bar{w}_i)_{0 \leq i < p}$承认为基，李代数$g_p$承认$(\bar{u})_{u \in P_p}$为基本家庭，模$L(X)$为直和共 $L_p$ 和 $g_p$。*

$L_0 = \{0\}$ 和$g_0 = L(X)$ 以及引理对于$p = 0$ 成立。我们在$p$上争论归纳。假设引理对于某些整数 $p \geq 0$ 是正确的。让$u_i, w = (\mathrm{ad}\ \bar{w}_p)^i.\bar{w} = \Psi(w_p^i w)$换成$i \geq 0, w \in P_p, w \neq w_p$。根据 no. 9 命题 10 的推论，免费李代数 $g_p$ 是直和模 $T_p$ 基 $\{\bar{w}_p\}$ 和谎言子代数 $h_p$承认

$$
\mathscr{F} = (u_i, w)_{i \geq 0,\ w \in P_p,\ w \neq w_p}
$$

作为基本家庭。到命题 13 (d)，族$(\bar{u})_{u \in P_{p+1}}$等于$\mathscr{F}$，因此是$h_p = g_{p+1}$的基本族。因此，$L(X) = L_p \oplus T_p \oplus g_{p+1}$，以及$L_{p+1} = L_p + T_p$、$L(X) = L_{p+1} \oplus g_{p+1}$和$(\bar{w}_0, \bar{w}_1, \ldots, \bar{w}_{p-1}, \bar{w}_p)$，是模$L_{p+1}$的基。

设$n$为正整数。到命题 13 (c) 时，存在整数 $p(n)$，使得$P_p$ 对于$p \geq p(n)$ 仅有长度 $> n$ 的元素。对于$p \geq p(n)$，$L(X)$的谎言子代数$g_p$是由次数$> n$的元素生成的，因此$L^n(X) \cap g_p = \{0\}$。另一方面，$L(X)$的元素$\bar{w}_i$是同质的，$(w_i)_{0 \leq i < p}$族是$g_p$的补充模的基。紧接着，次数$n$的元素$\bar{w}_i$的家庭是模$L^n(X)$的基，序列$(\bar{w}_i)_{i \geq 0}$是模的基 $L(X)$。

(B) *一般情况。*

如果$S$是$X$的子集，回想一下，$M(S)$与$S$生成的$M(X)$的子大图进行识别，$L(S)$与$S$生成的$L(X)$的谎言子代数进行识别；我们已经看到，如果$w \in M(S)$是长度$\geq 2$，那么$\alpha(w) \in M(S)$和$\beta(w) \in M(S)$。紧接着，$H \cap M(S)$ 是相对于$S$ 的集合大厅。

对于$H$的每个有限子集$\Phi$，都存在$X$的有限子集$S$，使得

Φ ⊂ M(S)。情况 (A) 然后表明元素 $\bar{w}$ 与 $w \in \Phi$ 在 $L(S)$ 中线性无关，因此在 $L(X)$ 中线性无关。因此$(\bar{w})_{w \in H}$一家人是免费的。

对于$L(X)$的每个元素$a$，都存在$X$的有限子集$S$，使得$a \in L(S)$。在情况(A)中，$\Psi'(H)$生成模$L(S)$的子集$\Psi'(H \cap M(S))$，因此$a$是$\Psi'(H)$的元素的线性组合。因此$\Psi'(H)$生成模$L(X)$，从而完成证明。

#### 推论{#lie-ii-s2-n11-cor-1 .statement tag=0A3J}

*模* $L(X)$ *是免费的，子模* $L^\alpha(X)$ *其中* $\alpha \in \mathbf{N}^{(X)}$ *和* $L^n(X)$ *其中* $n \in \mathbf{N}$也是免费的。 *模* $L^\alpha(X)$ *属于有限秩，模* $L^n(X)$ *如果* $X$ *是有限的*。

相对于 $X$ (命题 11) 存在集合 $H$ 大厅。对于 $L(X)$ 属于的所有 $w \in H$、元素 $\Psi'(w)$ 到模 $L^\alpha(X)$（与 $\alpha \in \mathbf{N}^{(X)}$）和模 $L(X)$ 之一的直和子模$L^\alpha(X)$。进一步，对于所有$\alpha \in \mathbf{N}^{(X)}$，$M(X)$的元素的集合，其$\mathbf{N}^{(X)}$中的典范像等于$\alpha$是有限的；这表明模 $L^\alpha(X)$ 中的每一个都是免费的，有限秩和 $L(X)$ 中的每一个都是免费的。现在 $L^n(X) = \sum_{|\alpha|=n} L^\alpha(X)$ 以及 $L^n(X)$ 是免费的；当$X$有限时，$\alpha \in \mathbf{N}^{(X)}$的集合使得$|\alpha|=n$有限，因此$L^n(X)$是有限秩。

#### 定义 3 {#lie-ii-s2-def-3 .statement tag=0A3K}

*免费李代数* $L(X)$ 的大厅基 *是* $L(X)$ 的任何基 *这是相对于* $X$ 的集合大厅的典范像。

#### 注 {#lie-ii-s2-n11-rem-1 .statement tag=0A3L}

假设$X$由两个不同的元素、$x$和$y$组成，并令$L^{(\cdot,1)}$为$L^\alpha(X)$的$L(X)$和的子模，其中$\alpha \in \mathbf{N}^X$和$\alpha(y)=1$。紧接no. 10的定理 1和命题 12，$(\mathrm{ad}\,x)^n.y$的元素，其中$n$是整数$\geqslant 0$形式子模的*基* $L^{(\cdot,1)}$。由此可见，映射 ad* $x$ *限制到* $L^{(\cdot,1)}$ *是单射的*。

### 习题{#lie-ii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
