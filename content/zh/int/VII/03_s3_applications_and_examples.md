---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 3
section_title: Applications and examples
lang: zh
source: int-vii-ix
book_pages: INT VII.53-INT VII.73, INT VII.91-INT VII.94
pdf_pages: 0059-0079, 0097-0100
extraction: ocr
subsections:
    - "no": 1
      title: Compact groups of linear mappings
      page: 53
      pdf_page: 59
    - "no": 2
      title: Triviality of fibered spaces and of group extensions
      page: 55
      pdf_page: 61
    - "no": 3
      title: Examples
      page: 60
      pdf_page: 66
statements: 24
exercises: 12
content_sha256: 26ba83b5523fd3829c5a4a663c586422cfec84c8d010f5043f6577233ba44886
translated_from: content/en/int/VII/03_s3_applications_and_examples.md
translation_method: google
source_content_sha256: 77d86192dc78c3caea75d568c8ef5d05992c7bdcaed4b1daac8f963f1400d1ea
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: e54d95e44fe8ecf65d66d4b1cefc8ff870429b8f3983de8af42ce274cead37dd
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 3。应用程序和例

### 1. 紧凑群线性映射

令 $E$ 为有限维向量空间超过 $\mathbf{R}, \mathbf{C}$ 或 $\mathbf{H}$。那么$\mathrm{End}(E)$是$\mathbf{R}$上的有限维代数，$\mathrm{End}(E)$（§ 1, No. 10）上的规范拓扑是紧致收敛的拓扑。 群$\mathrm{Aut}(E) = \mathbf{GL}(E)$是$\mathrm{End}(E)$的开子集，因此是局部紧的群。令$(e_1, e_2, \ldots, e_n)$为$E$的基，并且对于$E$的每个自同态$u$，令$M(u) = (\alpha_{ij}(u))$相对于此基为$u$的矩阵；说$\mathrm{End}(E)$的子集$S$在$\mathrm{End}(E)$中相对紧凑，相当于函数$\alpha_{ij}(u)$在$S$有界的说。

#### 命题 1 {#int-vii-s3-prop-1 .statement tag=09GS}

— *令 G 为 Aut(E)* 的子群。 *以下三个属性是等效的*：

(i) *G 在 End(E)* 中相对紧凑；
(ii) *G 在 Aut(E)* 中相对紧凑；
(iii) *G 在 E* 上留下不变的非简并$^1$正厄米特形式。

(iii) $\Rightarrow$ (i)：假设 $G$ 留下不变的非简并正值厄米特形式 $\Psi$。令 $(e_1, \ldots, e_n)$ 为 $\Psi$ 的标准正交基（*Alg.*，Ch.IX, § 6, No. 1，Th.1 的 Cor.1）。对于每个$u \in G$，令$(u_{ij})$为其相对于$(e_i)$的矩阵。对于任何$j$，我们有$\sum_{i=1}^n |u_{ij}|^2 = 1$，因此对于所有$i$和$j$都有$|u_{ij}| \leq 1$，这证明了(i)。

(i) $\Rightarrow$ (ii)：这源自 GT，X, § 3, No. 5，Cor。的 Th。 4、考虑到$\mathrm{End}(E)$的拓扑是紧收敛的。

(ii) $\Rightarrow$ (iii)：假设$\mathrm{Aut}(E)$中$G$的闭包$\overline{G}$是紧的。令 $\Phi$ 为 $E$ 上的非简并正厄米特形式。如果标量的域是$\mathbf{R}$或$\mathbf{C}$，则给出$\Phi$使得$E$成为有限维希尔伯特空间，并且条件(iii)将由以下引理产生：

$^1$ 非退化；在 EVT 中，项被 séparante 取代，随后翻译为“分离”（TVS，V, § 1, No. 1）。

#### 引理 1 {#int-vii-s3-lem-1 .statement tag=09GT}

令F为希尔伯特空间，K为紧致群，K的s↦U(s)表示在$\mathscr{L}(F; F)$的可逆元的群中，对于逐点收敛的拓扑连续。 F 上存在非简并正厄米特形式 $\varphi$ 使得

$$
\varphi(U(s)x, U(s)y) = \varphi(x, y)
$$

对于所有$s \in K, x \in F, y \in F$，并且由$\varphi$（TVS，V, §1, No. 3）定义的F的拓扑向量空间结构与F的原始结构相同。

令 $\alpha$ 为 K 上的 Haar 测度。对于 F 中的任何 $x, y$，映射 $s \mapsto (U(s)x|U(s)y)$ 是连续的。 集合

$$
\varphi(x, y) = \int (U(s)x|U(s)y)\, d\alpha(s).
$$

$\varphi(x, y)$是F上的倍半线性形式，直接的。由于自同态$U(s)$的集合在$\mathscr{L}_s(F; F)$中是紧的，因此存在一个常数M，使得对于所有$s \in K$都有$\|U(s)\| \leq M$。因此，对于每个 $x \in F$，我们有

$$
M^{-1}\|x\| \leq \|U(s)x\| \leq M\|x\|,
$$

从而不平等

$$
M^{-2}\alpha(K)\|x\|^2 \leq \varphi(x, x) \leq M^2\alpha(K)\|x\|^2,
$$

这表明$\varphi$是正的且非简并的，并且范数$\varphi(x, x)^{1/2}$等价于范数$\|x\|$。最后，对于所有$t \in K$，

$$
\begin{align*}
\varphi(U(t)x, U(t)y) &= \int (U(st)x|U(st)y)\, d\alpha(s) \\
&= \int (U(s)x|U(s)y)\, d\alpha(s) = \varphi(x, y).
\end{align*}
$$

当标量的域为 $\mathbf{H}$ 时，人们认为在函数 $s \mapsto (U(s)x|U(s)y)$ 处由函数 $s \mapsto \Phi(sx, sy)$ 在 G 上定义，与替换上的之前完全相同，值在 $\mathbf{H}$ 中。这样就完成了命题的证明。

#### 注 {#int-vii-s3-n1-rem-1 .statement tag=09GU}

令$\Phi$为E上的非简并正厄米特形式。酉群$\mathbf{U}(\Phi)$在$\mathrm{Aut}(E)$中闭，因此是紧的（命题1）。命题1还表明，$\mathrm{Aut}(E)$的每个紧致子群都包含在形式$\mathbf{U}(\Phi)$的子群中。如果现在 $\mathbf{U}(\Phi)$ 包含在 $\mathrm{Aut}(E)$ 的紧致子群 K 中，则可以看出 E 上存在非简并正厄米特形式 $\Phi'$，使得 $\mathbf{U}(\Phi) \subset K \subset \mathbf{U}(\Phi')$，并且很容易遵循

（例1）$\Phi$和$\Phi'$成比例，从而$\mathbf{U}(\Phi) = K$。因此，$\mathrm{Aut}(E)$的最大紧凑子群是形式$\mathbf{U}(\Phi)$的子群。

### 2. 纤维空间和群扩张的琐碎

#### 命题 2 {#int-vii-s3-prop-2 .statement tag=09GV}

*设 X 为局部紧致空间，其中局部紧致群 H 通过 $(x, \xi) \mapsto x\xi$ 连续正确地作用于右侧。假设 X/H 是仿紧的。令g为H在$\mathbf{R}^n$中的连续表示。那么在 $\mathbf{R}^n$ 中存在一个连续的 X f 映射 f，使得对于所有 $x \in X$ 和 $\xi \in H$ 都有 $f(x\xi) = f(x) + g(\xi)$。*

一个约化立即对应到 $n = 1$ 的情况。由于加法群$\mathbf{R}$与乘法群$\mathbf{R}_+^*$同构的，命题则为§2, No. 4第7条命题的直接的推论。

#### 推论 {#int-vii-s3-n2-cor-1 .statement tag=09GW}

*设 X 为局部紧致空间，其中有限维实数向量空间 V 在右侧连续正确地按 $(x, v) \mapsto xv$ 运算。设$\pi$是X的典范映射到$B = X/V$。假设 B 是仿紧的。*

a) *存在X到V的连续映射 f，使得对于所有$x \in X$和$v \in V$都有$f(xv) = f(x) + v$。*

b) *如果 f 是 a) 的映射满足条件，则映射 $x \mapsto (\pi(x), f(x))$ 是 X 到 $B \times V$ 的同胚。*

断言 a) 由命题2得出，其中g被取为V的恒等映射。令 f 为 a) 的映射满足条件。 X到X的映射$x \mapsto x \cdot (-f(x))$是连续的，并且在每个轨道上是恒定的，因此是形式$\varphi \circ \pi$，其中$\varphi$是B到X的连续映射；对于每个$b \in B$，$\pi(\varphi(b)) = b$。 X的映射$x \mapsto (\pi(x), f(x))$进入$B \times V$和$B \times V$的$(b, v) \mapsto \varphi(b) \cdot v$进入X是互逆的，因为$\varphi(\pi(x)) \cdot f(x) = x \cdot (-f(x)) \cdot (f(x)) = x$，$\pi(\varphi(b) \cdot v) = \pi(\varphi(b)) = b$，并且，如果$b = \pi(y)$，则

$$
f(\varphi(\pi(y)) \cdot v) = f(y \cdot (-f(y)) \cdot v) = f(y) - f(y) + v = v .
$$

由于这些映射是连续的，因此它们是同胚。

#### 注 {#int-vii-s3-n2-rem-1 .statement tag=09GX}

— 令 E 为有限维实仿射空间，T 为紧致空间，$\mu$ T 上*总质量* 1 的度量，f 为 T 到 E 中的连续映射。如果选择 E 中的原点 a，则 E 将配备向量空间结构和积分 $\int_T f(t) d\mu(t)$因此有意义；它代表 E 的点 x，使得

$$
x - a = \int_T (f(t) - a) d\mu(t) .
$$

这个点独立于$a$的选择。例如，令$a' \in \mathbf{E}$和$x' \in \mathbf{E}$使得$x' - a' = \int_{\mathbf{T}} (f(t) - a') d\mu(t)$。然后

$$
x' - a = (x' - a') + (a' - a) = \int_{\mathbf{T}} (f(t) - a') d\mu(t) + \int_{\mathbf{T}} (a' - a) d\mu(t)
$$
$$
= \int_{\mathbf{T}} (f(t) - a) d\mu(t) = x - a,
$$

从而$x' = x$。因此，我们可以使用符号$\int_{\mathbf{T}} f(t) d\mu(t)$，而不指定选择源自$\mathbf{E}$。如果$u$是$\mathbf{E}$到另一个有限维仿射空间$\mathbf{E}'$的仿射映射，则

$$
u \left( \int_{\mathbf{T}} f(t) d\mu(t) \right) = \int_{\mathbf{T}} u(f(t)) d\mu(t).
$$

因为，$\mathbf{E}$和$\mathbf{E}'$可以用向量空间来识别，使得$u$变成线性映射，在这种情况下公式是已知的（第III, §3, No. 2，第2条命题和No. 3，第7条命题）。

#### 引理 2 {#int-vii-s3-lem-2 .statement tag=09GY}

*令$G$为紧致群，$\mu$为$G$的归一化哈尔测度，$\mathbf{E}$为有限维实仿射空间，$A$为$\mathbf{E}$的仿射群，以及将$G$中的$\rho$同态转换为$A$。假设对于每个$x \in \mathbf{E}$，$G$到$\mathbf{E}$的映射$s \mapsto \rho(s)x$是连续的。然后，对于每个 $x \in \mathbf{E}$，点*

$$
x_0 = \int_G \rho(s)x\, d\mu(s) \in \mathbf{E}
$$

*在$G$下不变。*

对于每 $t \in G$，

$$
\rho(t)x_0 = \int_G \rho(t)\rho(s)x\, d\mu(s) = \int_G \rho(ts)x\, d\mu(s) = \int_G \rho(s)x\, d\mu(s) = x_0.
$$

#### 命题 3 {#int-vii-s3-prop-3 .statement tag=09GZ}

*令$G$为局部紧致群。令 $H$ 为 $G$ 的闭法线子群，与 $\mathbf{R}^n$ 同构的，且 $G/H$ 是紧致的。*

a) *存在$G$的闭子群$L$，使得$G$是$L$和$H$的拓扑半直接乘积。*

b) *如果$M$是$G$的紧子群，则存在元素$x \in H$使得$x^{-1}Mx \subset L$。*

c) *$G$的每个紧凑子群都包含在最大紧凑子群中。*

d) *最大紧凑$G$的子群是子群，即$L$的变换乘以$G$的内自同构。*

设$\pi$是$G$到$K = G/H$的典范同态。通过将$G \times H$的商、映射$(s, h) \mapsto shs^{-1}$转入$H$定义，将$K \times H$的连续映射$(\sigma, h) \mapsto \sigma \cdot h$转入$H$，从而得到$shs^{-1} = \pi(s) \cdot h$。我们将认同 $H$ 与 $\mathbf{R}^n$ （因此，视情况而定，对 $H$ 中的群运算使用乘法或加法记号）。由科。根据命题2，存在$G$到$H$的连续映射$f$，使得$f(xh) = f(x) + h$对应$x \in G, h \in H$。对于每个$x \in G$，设$p(x) = x \cdot (-f(x))$，它仅取决于$x$相对于$H$的陪集。 集合

$$
\begin{align*}
(1) \quad F(x, y) &= p(xy)^{-1} p(x)p(y) = f(xy)y^{-1}x^{-1}x(-f(x))y(-f(y)) \\
&= f(xy)[y^{-1}(-f(x))y](-f(y)) \\
&= f(xy) - \pi(y)^{-1}f(x) - f(y).
\end{align*}
$$

我们看到*如果* $F(x, y) = 0$ *对于所有* $x, y$ *在* $G$，则$p(G) = L$是$G$的子群，与$H$的每个陪集相交于一个且唯一的一个点。由于$p$是连续的，因此$G$是$L$和$H$的拓扑半直接乘积（GT，III, §2, No. 10）。

现在，对于任意 $h, h' \in H$，

$$
\begin{align*}
F'(xh, yh') &= f(xhyh') - \pi(y)^{-1}f(xh) - f(yh') \\
&= f(xhy) + h' - \pi(y)^{-1}f(x) - \pi(y)^{-1}h - f(y) - h' \\
&= f(xy(\pi(y)^{-1}h)) - \pi(y)^{-1}f(x) - f(y) - \pi(y)^{-1}h \\
&= f(xy) - \pi(y)^{-1}f(x) - f(y) = F(x, y).
\end{align*}
$$

因此$F$定义，通过商，$K \times K$的连续映射$\varphi$进入$H$。

另一方面，对于$G$中的所有$x, y, z$，我们有

$$
\begin{align*}
F(z, xy) + F(x, y) &= f(zxy) - \pi(xy)^{-1}f(z) - f(xy) + f(xy) \\
&\phantom{=} - \pi(y)^{-1}f(x) - f(y) \\
&= \pi(y)^{-1}f(zx) - \pi(xy)^{-1}f(z) - \pi(y)^{-1}f(x) + f(zxy) \\
&\phantom{=} - \pi(y)^{-1}f(zx) - f(y) \\
&= \pi(y)^{-1}F(z, x) + F(zx, y),
\end{align*}
$$

因此，对于$K$中的所有$x', y', z'$，

$$
-\varphi(x', y') = \varphi(z', x'y') - {y'}^{-1}\varphi(z', x') - \varphi(z'x', y').
$$

让我们通过 $K$ 的归一化哈尔测度 $\alpha$ 对 $z'$ 进行积分。 设定$\psi(x') = \int \varphi(z', x')\, d\alpha(z')$，$\psi$是K上的连续函数，并且（在注意到上$\mathbf{R}^n$中K的运算尊重$\mathbf{R}^n$的向量空间结构由GT，VII, §2, No. 1，Prop. 1)、得到

$$
-\varphi(x', y') = \psi(x'y') - {y'}^{-1}\psi(x') - \psi(y').
$$

另外字、设定$k - \psi \circ \pi$，是G上连续的函数，

(2)
$$
-F(x, y) = k(xy) - \pi(y)^{-1}k(x) - k(y).
$$

比较 (1) 和 (2)，我们可以看到，如果 $f$ 被连续的函数 $f + k$ 替换（这留下了已验证的性质 $f(xh) = f(x) + h$），F 被 0 替换，正如我们之前看到的，这完成了 a) 的证明。

对于每个$g \in G$，令$l_g$（或$h_g$）为L（或H）的唯一元素，使得$g = h_g l_g$。如果$h_1 \in H$和$g \in G$，那么

$$
gh_1 = h_g l_g h_1 = h_g(l_g h_1 l_g^{-1})l_g,
$$

因而$h_g h_1 = h_g + l_g h_1 l_g^{-1}$。对于每个 $g \in G$，令 $\psi_g$ 为 H 的映射定义为

$$
\psi_g(h_1) = h_g + l_g h_1 l_g^{-1}.
$$

可以看出，$G \times H$到H中的映射$(g, h_1) \mapsto \psi_g(h_1)$是连续的，并且使H成为G的齐次空间，其中原点的稳定子是L。此外，我们观察到，当 H 等同于 $\mathbf{R}^n$ 时，$\psi_g$ 是 H 自身的“仿射”映射。也就是说，设 M 是 G 的紧子群；到引理 2，存在$x \in H$，使得$\psi_m(x) = x$代表*所有* $m \in M$。对于$y \in H$，$\psi_y$是与向量$y$的翻译；由此可见，对于每一个 $m \in M$，$\psi_{x^{-1}} \circ \psi_m \circ \psi_x$ 变换 H 的原点都是自身，因而$x^{-1}mx \in L$。这就证明了$x^{-1}Mx \subset L$，从而b)。

令 $L'$ 为 G 包含于 L 的闭子群。那么$L'$就是L和$L' \cap H$的拓扑半直接乘积。如果 $L'$ 是紧致的，则 $L' \cap H$ 是紧致的，因此约化到点（GT，IV, §2, No. 2，Th. 2 的 Cor. 1），因而 $L' = L$。这证明L是G的最大紧致子群；因而，子群也是如此，即L的变换乘以G的内自同构。第3条命题的断言c)和d)则为b)的直接的推论。

#### 命题 4 {#int-vii-s3-prop-4 .statement tag=09H0}

*令 G 为局部紧致群，H 为 G 的闭法线子群，使得 K = G/H 是紧致的。然后$\mathbf{R}$中H的每个连续表示u，使得对于所有$\xi \in H$和$s \in G$的$u(s\xi s^{-1}) = u(\xi)$，可以扩展到$\mathbf{R}$中G的连续表示。*

设 $L = G \times \mathbf{R}$ 并令 M 为 $(\xi, -u(\xi))$ 的集合，其中 $\xi$ 越过 H。很明显，M 是 L 的闭法线子群。令 $L' = L/M$ 且令 $\pi$ 为 L 的典范映射到$L'$。 M 和 R 生成 L 的子群是 H × R，因此是闭集；因而 π(R) 是 L' 的闭子群 N。 π 到 R 的限制 ρ 是 R 到 N 上的双射连续表示。附录 1 的引理 2 证明 ρ 是双连续的。此外，L'/N 与 L/(H × R) = G/H 同构的，因此是紧的。根据命题3，并考虑到N在L'的中心中，L'是N的乘积和另一个子群。因而，N 上存在L' 的连续表示，N 到恒等映射上存在约化。因而，在 R 上存在 L 的连续表示 v，在 M 上是微不足道的，并且在 R 上存在约化到恒等映射。对于 ψ ∈ H，有 v((ψ, 0)) = v((ψ, −u(ψ))(e, u(ψ))) = u(ψ)，从而完成证明。

#### 引理 3 {#int-vii-s3-lem-3 .statement tag=09H1}

设 G 是由 e 的紧邻域生成的拓扑群。令 H 为 G 的闭子群，使得齐次空间 G/H 是紧的。然后 H 由 H 中 e 的紧邻域生成。

令C为紧集，使得G = CH。如有必要，放大 C，我们可以假设 C 生成 G 并且 G = ĈH。那么 C^2 是紧致的，并且被开路的 Ĉs (s ∈ H) 覆盖。因而，H 中存在 s_1, ..., s_n 使得 C^2 ⊂ Ĉs_1 ∪ ... ∪ Ĉs_n。令 Γ 为 s_i 生成的 H 的子群。然后C^2⊂CΓ。根据归纳，对于每个 n 都有C^n ⊂ CΓ，因而 G = CΓ。 H 的每个元素都可以放入形式 ab 中，其中 a ε C、b ε Γ、从而 a ε H、从而 a ε C ∩ H。 因而 H 由 C ∩ H 和 s_i 生成，即到紧集。

#### 引理 4 {#int-vii-s3-lem-4 .statement tag=09H2}

设G是连通拓扑群，D是G的完全不连通法线子群。则D包含在G的中心中。

例如，设 d ∈ D。在连续映射 x ↦ xdx^{-1} 下，G 的像是 D 的连通子集，因此约化到 {d}，这证明对于所有 x ∈ G，xd = dx。

#### 命题 5 {#int-vii-s3-prop-5 .statement tag=09H3}

令 G 为连通拓扑群，允许离散法线子群 D，使得 K = G/D 是紧的，并且 K 的换位子子群在 K 中是稠密的。则 D 是有限的，G 是紧的。

群 G 与 K 局部同构（GT，III, §2, No. 6，命题 19），因此是局部紧的；因为它是连通的，所以它是由 e 的紧邻域生成的。通过引理 3 和 4，D 是有限生成的阿贝尔的群，因此与群 $\mathbf{Z}^r \times D_1$ 同构的，其中 D_1 有限（A，VII, §4, No. 7，Th.3）。假设 r > 0。则在 $\mathbf{Z}$ 上存在 D 的表示 f。根据命题 4，f 可以扩展到 R 中 G 的连续表示 g。通过商，g 定义 $\mathbf{R}/\mathbf{Z}$ 中$K$ 的连续表示 $g'$；由于$\mathbf{R}/\mathbf{Z}$是阿贝尔的，$g'$包含换位子子群$K$的核，因而$g'$是平凡的；其他字，$g(G) \subset \mathbf{Z}$。由于$G$是连通的，因此得出$g(G) = \{0\}$，从$f(D) = \mathbf{Z}$开始这是荒谬的。因而 $r = 0$ 和 $D$ 是有限的。因而 $G$ 是紧致的（GT，III, §4, No. 1，Prop.2 的 Cor.2）。

### 3. 例

在这个小节（例 7和8除外）中，$K$表示非离散局部紧致交换域； $dx$表示$K$的加法群的Haar测度。

回想一下，$K = \mathbf{R}$时为$\operatorname{mod} x = |x|$，$K = \mathbf{C}$时为$\operatorname{mod} x = |x|^2$，$K = \mathbf{Q}_p$时为$\operatorname{mod} x = |x|_p$。

#### 例 1 {#int-vii-s3-n3-exa-1 .statement tag=09H4}

一般线性群。

设$A$为代数$M_n(K)$。 $A$的可逆元的群$A^*$无非就是一般的线性群$\mathbf{GL}(n, K)$。对于每个$X \in A$，约化范数$\operatorname{Nrd}_{A/K}(X)$等于$\det X$；因而 $N_{A/K}(X) = (\det X)^n$（阿尔格.，第 VIII, §12, No. 3，第 8 条命题；cf. A，III, §9, No. 3，例 3）。由于$X \mapsto {}^t X$是$A$的同构到反代数，

$$
N_{A^0/K}(X) = N_{A/K}({}^t X) = \det ({}^t X)^n = (\det X)^n.
$$

那么§1, No. 11的第16条提案证明了该措施

$$
\operatorname{mod}(\det X)^{-n} \cdot \bigotimes_{i,j} dx_{ij} \quad (X = (x_{ij}))
$$

是 $\mathbf{GL}(n, K)$ 上的左右 Haar 测度。

对于确定在$\mathbf{GL}(n, K)$上相对不变的测度，我们依赖以下引理：

#### 引理 5 {#int-vii-s3-lem-5 .statement tag=09H5}

$\mathbf{C}^*$中$\mathbf{GL}(n, K)$的连续表示是形式$X \mapsto \chi(\det X)$的映射，其中$\chi$是$\mathbf{C}^*$中$K^*$的连续表示。

这样的映射显然是$\mathbf{C}^*$中$\mathbf{GL}(n, K)$的连续表示。相反，假设$\psi$是$\mathbf{GL}(n, K)$在$\mathbf{C}^*$中的连续表示。 $x \in K^*$、集合

$$
\tilde{x} = \begin{pmatrix}
x & & \\
& 1 & 0 \\
& & 1 \\
0 & \cdots & 1
\end{pmatrix}
$$

和$\chi(x) = \psi(\widetilde{x})$。那么，对于每个矩阵$X \in \mathbf{GL}(n, K)$，我们有$(\det X^{-1}) \sim \cdot X \in \mathbf{SL}(n, K)$。由于$\mathbf{SL}(n, K)$是$\mathbf{GL}(n, K)$的换位子子群（A，III, §8, No. 9，第17号提案的Cor.），$\psi((\det X^{-1}) \sim \cdot X) = 1$，从而
$$
\psi(X) = \psi((\det X) \sim) = \chi(\det X).
$$
这成立了，Cor。 §1, No. 8 的第 10 条命题 1 证明，$\mathbf{GL}(n, K)$ 上相对不变的测度是，直到常数因子时，形式的测度
$$
(4) \quad \chi(\det X) \cdot \bigotimes_{ij} dx_{ij} \qquad (X = (x_{ij})),
$$
其中$\chi$是$\mathbf{C}^*$中$K^*$的连续表示。

#### 例 2 {#int-vii-s3-n3-exa-2 .statement tag=09H6}

**仿射群.**
对于每个$X \in \mathbf{GL}(n, K)$和每个$x \in K^n$，令$(X, x)$为$K^n$中的仿射线性映射$\xi \mapsto X\xi + x$。 $(X, x)$的集合是$K^n$的仿射群$G$（A，II, §9, No. 4）。翻译的集合$T$是$G$的闭法线子群，与$K^n$自然同构；另一方面，$\mathbf{GL}(n, K)$是$G$的闭子群，$G$是$\mathbf{GL}(n, K)$和$T = K^n$的半直接乘积。其中，$G$配备（局部紧凑）拓扑，其中$G$是$\mathbf{GL}(n, K)$和$T$的拓扑半直接乘积（GT，III, §2, No. 10）。一个有
$$
(X, x) = (1, x) \cdot (X, 0).
$$
另一方面，如果 $X \in \mathbf{GL}(n, K)$ 和 $x \in T$ 那么，对于每个 $\xi \in K^n$，
$$
(X, 0)(1, x)(X, 0)^{-1}\xi = X(X^{-1}\xi + x) = \xi + Xx = (1, Xx)\xi,
$$
因此 $T$ 的自同构 $(1, x) \mapsto (X, 0)(1, x)(X, 0)^{-1}$ 的模数为 $\mod(\det X)$（§1, No. 10，命题 15）。鉴于例 1 和§2, No. 9，*注*，该措施
$$
(5) \quad \mod(\det X)^{-n-1} \cdot \left( \bigotimes_{ij} dx_{ij} \right) \otimes \left( \bigotimes_i dx_i \right) \qquad (X = (x_{ij}), \ x = (x_i))
$$
是 $G$ 上的左哈尔测度。另一方面，根据§2, No. 9第14号提案，
$$
\Delta_G((X, x)) = \Delta_{\mathbf{GL}(n, K)}(X) \Delta_{K^n}(x) (\mod \det X)^{-1},
$$
或
$$
(6) \quad \Delta_G((X, x)) = \mod(\det X^{-1}).
$$

因此，$G$ 的正确 Haar 测度由下式给出

$$
(\mod \det X)^{-n} \cdot \left( \bigotimes_{ij} dx_{ij} \right) \otimes \left( \bigotimes_i dx_i \right).
$$

#### 例 3 {#int-vii-s3-n3-exa-3 .statement tag=09H7}

**严格的三角形群。**

令$[1, n]$为整数$m$的集合，使得$1 \leq m \leq n$。令$J$为$[1, n] \times [1, n]$满足以下条件中的子集：
1) 如果$(i, j) \in J$则$i < j$；
2) 如果$(i, j) \notin J$，则对于每个整数$k$，使得$i < k < j$，两个对、$(i, k)$和$(k, j)$中至少一个不属于到$J$。

令$T_J$为矩阵$Z = (z_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}$的集合，其中$K$中有元素，这样$z_{ii} = 1$，并且如果$i \neq j$和$(i, j) \notin J$则为$z_{ij} = 0$。这是 $\mathbf{GL}(n, K)$ 的闭子集。 映射$Z \mapsto (z_{ij})_{(i, j) \in J}$是$T_J$到$K^s$的同胚（其中$s$表示$J$的元素的数）。如果 $Z' = (z'_{ij}) \in T_J$，则 $Z'Z = (z''_{ij})$ 与

$$
z''_{ij} = z_{ij} + z'_{ij} + \sum_{i < h < j} z'_{ih} z_{hj} \quad \text{for } i < j,
$$
$$
z''_{ij} = 0 \text{ for } i > j, \quad z''_{ii} = 1,
$$

从而$Z'Z \in T_J$。如果 $T_J$ 被识别为 $K^s$，那么映射 $Z \mapsto Z'Z$（对于固定的 $Z'$）被仿射映射识别，并且它的行列式是 1，正如按字典顺序对对 $(i, j) \in J$ 排序所看到的那样以及应用以下引理：

#### 引理 6 {#int-vii-s3-lem-6 .statement tag=09H8}

**令 $L$ 为全序有限集合。对于每个$\lambda \in L$，令$V_\lambda$为有限维中的自由模超过交换环$k$；对于$L$中的$\lambda, \mu$，使得$\lambda \leq \mu$，令$f_{\lambda \mu} \in \mathrm{Hom}_k(V_\mu, V_\lambda)$。然后线性映射
$$
(v_\lambda)_{\lambda \in L} \mapsto \left( \sum_{\mu \geq \lambda} f_{\lambda \mu}(v_\mu) \right)_{\lambda \in L},
$$
从$\prod_{\lambda \in L} V_\lambda$到$\prod_{\lambda \in L} V_\lambda$，有行列式$\prod_{\lambda \in L} \det f_{\lambda \lambda}$。

一个约化紧接着$L$是整数的区间，然后从A，III, §8, No. 6，公式（31）得出引理。

如果$Z \in T_J$，则可以看到存在$Z' \in T_J$，使得$Z'Z = I_n$、从而$Z' = Z^{-1}$。因此，$T_J$是$\mathbf{GL}(n, K)$的闭子群。另一方面，§1, No. 10第15号提案表明该措施

$$
\bigotimes_{(i, j) \in J} dz_{ij}
$$

是 $T_J$ 上的左哈尔测度。通过计算$ZZ'$，我们可以以同样的方式看到该测度是$T_J$ 上的正确哈尔测度。

如果在$T_J$中的定义中，行和列的角色互换，也会得到类似的结果。

当$J$是对$(i, j)$的集合时，$i < j$、群$T_J$称为阶$n$的*上严格三角形群* $K$，记作$T_1(n, K)$。它的转置称为*下严格三角形群*。

#### 例 4 {#int-vii-s3-n3-exa-4 .statement tag=09H9}

— *大三角形群.*

设$n_1, \ldots, n_r$为整数$\geqslant 1$。 集合$p_k = n_1 + \ldots + n_{k-1}$和$n = p_{r+1} = n_1 + \cdots + n_r$。令$I_k$为整数$j$的集合，使得$p_k < j \leqslant p_{k+1}$，并且使$k < l$的$I_k \times I_l$为$J$并。令 $G$ 为 $\mathbf{GL}(n, K)$ 的闭子群，其元素为矩阵 $(Z_{kl})_{1 \leqslant k \leqslant r, 1 \leqslant l \leqslant r}$，这样：
1) 每个$Z_{kl}$为$K$的元素矩阵$(z_{ij})_{i \in I_k, j \in I_l}$，有$n_k$行和$n_l$列；
2) $Z_{kl} = 0$换$k > l$；
3) $Z_{kk} \in \mathbf{GL}(n_k, K)$ 换$1 \leqslant k \leqslant r$。

公式块乘法

$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix}
$$

$$
= \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
$$

表明$G$是元素$(Z_{kl}) \in G$的子群$D$的拓扑半直接乘积，使得$Z_{kl} = 0$对于$k \neq l$和子群$T_J$对于例 3. 此外，对于$1 \leqslant k \leqslant r$，$D$同构于群$\mathbf{GL}(n_k, K)$的直接乘积。

对于$(i, j) \in J$，令$J'$为对$(j, i)$的集合，并让$H$为对$(i, j) \in [1, n] \times [1, n]$的集合，而不是属于到$J'$。令 $Z' = (z_{ij})_{1 \leqslant i \leqslant n, 1 \leqslant j \leqslant n}$ 为 $G$ 中的元素。根据§2, No. 9的第14条命题以及上面的例1和3，通过取像测度，可以得到$G$上的左哈尔测度

$$
\bigotimes_{k=1}^r ((\mathrm{mod}\ \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij}) \otimes \left( \bigotimes_{(i,j) \in J} dz_{ij} \right)
$$

映射以下

$$
((Z_{kk}), (Z_{kl})) \mapsto \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}.
$$

现在，考虑对于 $k < l$，向量空间或矩阵 $Z_{kl} = (z_{ij})_{i \in I_k, j \in I_l}$。它是由矩阵形成的$n_l$子空间$M_j$（$j \in I_l$）中的直和，使得$z_{ih} = 0$对应$h \neq j$。这些子空间$M_j$中的每一个都在映射$Z_{kl} \mapsto Z_{kk}Z_{kl}$下稳定，而这个映射到$M_j$中的限制有矩阵$Z_{kk}$。因而，映射$Z_{kl} \mapsto Z_{kk}Z_{kl}$下措施$\bigotimes_{i \in I_k, j \in I_l} dz_{ij}$的（§ 1, No. 10，提案15）像为

$$
(\operatorname{mod} \det Z_{kk})^{-n_l} \cdot \bigotimes_{i \in I_k, j \in I_l} dz_{ij}.
$$

因而，$G$ 的左哈尔测度由下式给出

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{-q_k} \cdot \bigotimes_{(i,j) \in H} dz_{ij}
$$

与$q_k = \sum_{k \leq l \leq r} n_l = n - p_k$。

让我们再次使用 § 2 的第 14 条命题来求计算 $G$ 的*模*。 群 $D$ 和 $T_J$ 是幺模；另一方面：

$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix}
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}^{-1}
$$
$$
= \begin{pmatrix}
1 & Z'_{12} & \ldots & Z'_{1r} \\
0 & 1 & \ldots & Z'_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix},
$$

其中$Z'_{kl} = Z_{kk}Z_{kl}Z_{ll}^{-1}$。考虑到例 3 和 § 1, No. 10 的第 15 条命题，并按上述论证，可以看出，如果 $X = \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \in D$，则 $T_J$ 的自同构 $Z \mapsto X^{-1}ZX$ 的模为

$$
\prod_{k < l} (\operatorname{mod} \det Z_{kk})^{-n_l} (\operatorname{mod} \det Z_{ll})^{n_k},
$$

所以

$$
\Delta_G(Z) = \prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{n+n_k-2q_k}.
$$

以同样的方式研究$G$的转置群$G'$。对于$G'$，可以找到左哈尔测度

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{-p_{k+1}} \cdot \bigotimes_{(j,i) \in H} dz_{ij},
$$

和作为模数

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{n+n_k-2p_{k+1}}.
$$

如果特别是取$n_1 = \ldots = n_r = 1$，则可以找到由矩阵$X = (x_{ij})$形成的$M_n(K)$子代数的可逆元素的群$T(n, K)^*$作为群$G$，使得对于$i > j$有$x_{ij} = 0$。 这个代数，我们将表示为$T(n, K)$，被称为*上三角代数*，群$T(n, K)^*$被称为阶$n$在$K$上的*上大三角群*。 前面的公式然后取下面的形式：$T(n, K)^*$上的左哈尔测度是

$$(9\ bis)$$
$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{i-n-1} \cdot \bigotimes_{i \leq j} dz_{ij} \quad (Z = (z_{ij}))
$$

$T(n, K)^*$ 的模为

$$(10\ bis)$$
$$
\Delta_{T(n,K)^*}(Z) = \prod_{i=1}^n (\operatorname{mod} z_{ii})^{2i-n-1} \quad (Z = (z_{ij})).
$$

对于$T(n, K)^*$的转置，或*下大三角形群*，可找到左哈尔测度

$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{-i} \cdot \bigotimes_{i \geq j} dz_{ij},
$$

和作为模数

$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{n+1-2i}.
$$

#### 注 {#int-vii-s3-n3-rem-1 .statement tag=09HA}

群$T(n, K)^*$是$\mathbf{GL}(n, K)$和$\Delta_{T(n, K)^*}((z_{ij})) = \prod_{i=1}^n (\operatorname{mod} z_{ii})^{2i-n-1}$的闭子群。我们在例1中看到了$\Delta_{\mathbf{GL}(n, K)} = 1$。如果$n > 1$，函数
$$
\Delta_{T(n, K)^*}/\Delta_{\mathbf{GL}(n, K)}
$$
在$T(n, K)^*$不能上扩展到$\mathbf{C}^*$中$\mathbf{GL}(n, K)$的连续表示（因为这样的表示将在$\mathbf{SL}(n, K)$上通过引理5等于1，而$\operatorname{mod}(z_{11})^{1-n} \neq 1$对于适当选择的$z_{11}$来说）。由此可见，如果 $n > 1$（§ 2, No. 6，Th. 3 的 Cor. 1），齐次空间 $\mathbf{GL}(n, K)/T(n, K)^*$ *不承认相对不变的测度*。

对于$n = 2$，可以通过$K$上的*投影线*来识别该齐次空间。例如，令 $(e_1, e_2)$ 为 $K^2$ 的典范基。 群$\mathbf{GL}(2, K)$在$K^2$行的集合上进行传递运算，省略0，$Ke_1 - \{0\}$的稳定子是$T(2, K)^*$。

#### 例 5 {#int-vii-s3-n3-exa-5 .statement tag=09HB}

— *特殊三角形群.*
让我们再次讨论例 4 开头的记号，并考虑子群$G_1 = G \cap \mathbf{SL}(n, K)$。这个子群是群$D_1 = D \cap \mathbf{SL}(n, K)$与$T_J$的拓扑半直接乘积。 群 $D_1$ 具有与 $\mathbf{SL}(n_r, K)$ 同构的普通子群 $A$，即元素 $\operatorname{diag}(Z_{kk})$ 的子群由……组成，$Z_{kk} = 1$ $k < r$。 同态
$$
\varphi : \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \mapsto (Z_{11}, \ldots, Z_{r-1, r-1})
$$
$D_1$ 到 $\mathbf{GL}(n_1, K) \times \cdots \times \mathbf{GL}(n_{r-1}, K)$ 是满射的并且有核 $A$。另一方面，$\varphi$是连续的。考虑到附录I中的引理2，$D_1/A$可以被识别为$\mathbf{GL}(n_1, K) \times \cdots \times \mathbf{GL}(n_{r-1}, K)$。我们用 $\mu$ 表示 $A$ (cf. 例 6) 的哈尔测度，并用
$$
\alpha = \bigotimes_{k=1}^{r-1} \left( (\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij} \right) \otimes' d\mu(Z_{rr})
$$
$D_1$ 的 Haar 测度使得
$$
\alpha/\mu = \bigotimes_{k=1}^{r-1} \left( (\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij} \right)
$$
（§ 2, No. 7，提案 10）。然后如例 4 所示，$G_1$ 上的左 Haar 测度由下式给出
$$
\operatorname{mod} \left( \prod_{k=1}^{r-1} (\det Z_{kk})^{n_k-q_k} \right)
$$
$$
\cdot \left[ \bigotimes_{k=1}^{r-1} ((\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij}) \otimes' d\mu(Z_{rr}) \right] \otimes \bigotimes_{(i,j) \in J} dz_{ij}.
$$

由于$G_1$在$G$中是正规的，$G_1$的*模*是$G$的限制（§ 2, No. 7，命题10 b））。

如果 $n_r = 1$、子群 $A$ 约化到中性元素，且$G$ 上的左哈尔测度为

$$
\operatorname{mod}\left( \prod_{k=1}^{r-1} (\det Z_{kk})^{-q_k} \right) \cdot \bigotimes_{k=1}^{r-1} \left( \bigotimes_{i,j \in I_k} dz_{ij} \right) \otimes \bigotimes_{(i,j) \in J} dz_{ij}.
$$

如果取$n_1 = n_2 = \ldots = n_r = 1$，得到的群$G_1$称为*上特殊三角形群*，其转置$G'_1$称为*下特殊三角形群*。 $G_1$ 的左哈尔测度是

$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{i-n-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq i < j \leq n} dz_{ij} \right)
$$
$G_1$ 的模数为
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2i-2n} \right).
$$
对于$G'_1$，我们可以类似地找到左哈尔测度
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{n-i-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq j < i \leq n} dz_{ij} \right)
$$
和模数
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2n-2i} \right).
$$

#### 例 6 {#int-vii-s3-n3-exa-6 .statement tag=09HC}

— *特殊线性群.*
$\mathbf{GL}(n, K)$的封闭子群$T_1(n, K)$和${}^t(T(n, K)^*)$有交$\{e\}$。因此，映射$(M, N) \mapsto M \cdot N$是$T_1(n, K) \times {}^t(T(n, K)^*)$的连续双射$\varphi$到$\mathbf{GL}(n, K)$的子集$\Omega$。

#### 引理 7 {#int-vii-s3-lem-7 .statement tag=09HD}

— a) *设 $U = (u_{ij}) \in \mathbf{GL}(n, K)$。在阶$U \in \Omega$中，$\det(u_{ij})_{k \leq i, j \leq n} \neq 0$对于$k = 2, 3, \ldots, n$是必要且充分的。*
b) $\Omega$ *是 $\mathbf{GL}(n, K)$* 的开子集。
c) *映射 $\varphi$ 是 $T_1(n, K) \times {}^t(T(n, K)^*)$ 到 $\Omega$* 的同胚。

在阶即$U \in \Omega$中，存在$Z = (z_{ij}) \in T_1(n, K)$使得$ZU \in {}^t(T(n, K))$是充分必要的（那么必然

$ZU \in {}^t(T(n, K)^*)$，因为$U$和$Z$是可逆的）。根据我们之前看到的，如果 $Z$ 存在，那么它是唯一的。因此，在阶 $U \in \Omega$ 中，线性系统是充分必要的

$$
\sum_{k=1}^n z_{ik} u_{kj} = 0 \qquad (1 \leq i < j \leq n)
$$

（其中$(z_{ij}) \in T_1(n, K)$）承认唯一的解。现在，这个系统可以写成

$$
(13) \qquad \sum_{k=i+1}^n z_{ik} u_{kj} = -u_{ij} \qquad (1 \leq i < j \leq n).
$$

对于固定的$i$，未知数$z_{i,i+1}, z_{i,i+2}, \ldots, z_{i,n}$有系统个$n-i$方程；对于这些系统承认独特的解，有必要且充分：

$$
\det(u_{kj})_{i+1 \leq k \leq n,\ i+1 \leq j \leq n} \neq 0
$$

$i = 1, 2, \ldots, n-1$。这就证明了a）。由此可见，$\Omega$ 在$\mathbf{GL}(n, K)$ 中开放。另一方面，通过 Cramer 的公式求解系统 (13) 时，$z_{ij}$ 是作为 $\Omega$ 中分母为非零的的 $u_{ij}$ 的有理函数得到的，因此 $Z$ 连续依赖于$U$ 于 $\Omega$，证明 c)。

现在令 $G'_1 \subset {}^t(T(n, K)^*)$ 为下特殊三角形群。 映射 $(M, N) \mapsto M \cdot N$ 是 $T_1(n, K) \times G'_1$ 的连续双射 $\psi$ 到 $\mathbf{SL}(n, K)$ 的子集 $\Omega'$。

#### 引理 8 {#int-vii-s3-lem-8 .statement tag=09HE}

**a)** *设 $U = (u_{ij}) \in \mathbf{SL}(n, K)$。在阶和$U \in \Omega'$中，$\det(u_{ij})_{k \leq i, j \leq n} \neq 0$对于$k = 2, 3, \ldots, n$来说是充分必要的。*

b) $\Omega'$ *是 $\mathbf{SL}(n, K)$* 的开子集。

c) *映射 $\psi$ 是 $T_1(n, K) \times G'_1$ 到 $\Omega'$* 的同胚。

例如，令 $M \in T_1(n, K)$ 和 $N \in {}^t(T(n, K)^*)$。在阶、$M \cdot N \in \mathbf{SL}(n, K)$中，$N \in G'_1$是充分必要的。因此，$\Omega' = \mathbf{SL}(n, K) \cap \Omega$和引理8立即从引理7而来。

#### 命题 6 {#int-vii-s3-prop-6 .statement tag=09HF}

**a)** *群 $\mathbf{SL}(n, K)$ 是幺模的。*

b) *令$\mu_1$和$\mu_2$分别为上严格三角形群$T_1(n, K)$和下特殊三角形群$G'_1$的左哈尔测度。 $\mu_1 \otimes \mu_2$的像在$T_1(n, K) \times G'_1$到$\Omega'$的同胚$(M, N) \mapsto M \cdot N^{-1}$下是$\mathbf{SL}(n, K)$*上哈尔测度的限制到$\Omega'$。

c) *$\mathbf{SL}(n, K)$中$\Omega'$的补集对于$\mathbf{SL}(n, K)$*的哈尔测度可以忽略不计。

群 $\mathbf{GL}(n, K)$ 是单模 (例 1)，$\mathbf{SL}(n, K)$ 是 $\mathbf{GL}(n, K)$ 的正规子群，因此是单模（§ 2, No. 7，命题 10 b)）。 断言 b) 由a)、引理 8 和§ 2, No. 9 的第13 条命题得出。让我们证明c）。通过引理 8 a)，足以证明以下内容：如果$p((u_{ij})_{1 \leq i,j \leq n})$是多项式，与$\mathbf{SL}(n, K)$上的零不同，则$U \in \mathbf{SL}(n, K)$的集合 E，使得$p(U) = 0$对于哈尔测度可以忽略不计。考虑到§ 1, No. 10，Cor。根据第 13 条命题，$\mathbf{SL}(n, K)$ 的拓扑有一个可数的基。因此，只要证明对于每个$U_0 \in E$，在$\mathbf{SL}(n, K)$中存在一个$U_0$的邻域，其与E的交可以忽略不计；或者再次，在$\mathbf{SL}(n, K)$中存在I的邻域W，使得$U_0^{-1}E \cap W$可以忽略不计。让我们取$W = \Omega'$。鉴于b)，这一切都归结为证明对$(M, N) \in T_1(n, K) \times G'_1$中的集合使得$p(U_0 MN) = 0$对于$\mu_1 \otimes \mu_2$可以忽略不计。根据$\mu_1$和$\mu_2$的表达式（在例3和5中计算），这将由以下引理得出：

#### 引理 9 {#int-vii-s3-lem-9 .statement tag=09HG}

*令$\psi$为$K[X_1, \ldots, X_r]$的多项式$\neq 0$。在空间 $K^r$ 中，由 $\psi(x_1, \ldots, x_r) = 0$ 定义的集合 N 对于 Haar 度量可以忽略不计。*

让我们在$r$上以归纳争论吧。 引理对于$r = 1$来说是明显的，因为N是有限的集合。如果需要的话改变变量的编号，我们可以假设 $\psi \notin K[X_1, \ldots, X_{r-1}]$；写

$$
\psi(X_1, \ldots, X_r) = X_r^m \psi_0(X_1, \ldots, X_{r-1}) + \cdots + \psi_m(X_1, \ldots, X_{r-1})
$$

与 $m > 0$ 和 $\psi_0 \neq 0$。在空间$K^{r-1}$中，令$N_0$为$\psi_0(x_1, \ldots, x_{r-1}) = 0$定义的集合，归纳假设可以忽略不计。对于每个$(x_1, \ldots, x_{r-1}) \notin N_0$，$x_r \in K$的集合，使得$(x_1, \ldots, x_{r-1}, x_r) \in N$是有限的，因此可以忽略不计。由于 $K^r$ 在无穷大处可数（§ 1, No. 10，第 13 条命题），$N \cap [(K^{r-1} - N_0) \times K]$ 在 $K^r$ 中可以忽略不计（V, § 8, No. 2，第 4 条命题）。因此N可以忽略不计。

#### 例 7 {#int-vii-s3-n3-exa-7 .statement tag=09HH}

*岩泽分解$\mathbf{GL}(n, K)$。*

在该例中，K表示域$\mathbf{R}, \mathbf{C}, \mathbf{H}$之一。如果$\lambda \in K$，则$\overline{\lambda}$定义为等于$\lambda$，如果$K = \mathbf{R}$，则定义为等于$\lambda$的共轭，如果$K = \mathbf{C}$或$\mathbf{H}$。令 E 为维数 $n$ 的 K 上的右向量空间，并令 $\Phi$ 为 E 上的非简并正厄米特形式。

#### 引理 10 {#int-vii-s3-lem-10 .statement tag=09HI}

*令 $(f_1, f_2, \ldots, f_n)$ 为 E 的基。*
a) *E 存在一个且仅有一个正交基 $(e_1, e_2, \ldots, e_n)$，使得 $f_i = e_1 \alpha_{i1} + e_2 \alpha_{i2} + \cdots + e_i \alpha_{ii}$ ($i = 1, 2, \ldots, n$) 和 $\alpha_{ii} > 0$ 对于所有$i$。
b) *对于固定的$\Phi$，$e_i$和$\alpha_{ij}$持续依赖于$(f_1, \ldots, f_n) \in E^n$。*

让$E_i = f_1 K + f_2 K + \cdots + f_i K$，它有维数$i$。令 $g_i$ 为与 $E_{i-1}$ 正交的 $E_i$ 的非零元素，并且使得 $\Phi(g_i, g_i) = 1$。到 $i$ 上的归纳时，我们可以看到 $(g_1, \ldots, g_i)$ 是 $E_i$ 的正交基。特别是，$(g_1, \ldots, g_n)$是$E$的正交基。让$\lambda_i = \Phi(f_i, g_i)$。从$f_i \notin E_{i-1}$开始，一个人就有了$\lambda_i \neq 0$。 集合$e_i = g_i |\lambda_i| \lambda_i^{-1}$。然后

$$
\Phi(e_i, e_i) = |\lambda_i|^2 \overline{\lambda_i}^{-1} \Phi(g_i, g_i) \lambda_i^{-1} = 1,
$$

因此 $(e_1, \ldots, e_i)$ 也是 $E_i$ 的正交基；此外，$\Phi(e_i, f_i) = |\lambda_i| \overline{\lambda_i}^{-1} \Phi(g_i, f_i) = |\lambda_i| > 0$，因此$e_i$具有a)的性质。令 $(e'_1, \ldots, e'_n)$ 为 $E$ 的另一个正交基，具有相同的性质。通过$i$上的归纳可知，$(e'_1, \ldots, e'_i)$一定是$E_i$的基，因此对于某些$\mu_i \in \mathbf{K}$来说，$e'_i = e_i \mu_i$。然后

$$
1 = \Phi(e'_i, e'_i) = \overline{\mu_i} \Phi(e_i, e_i) \mu_i = \overline{\mu_i} \mu_i ,
$$

和$0 < \Phi(e'_i, f_i) = \overline{\mu_i} \Phi(e_i, f_i)$，因此$\mu_i > 0$和$\mu_i^2 = 1$，因此$\mu_i = 1$，从而a)。假设已经证明$e_i$和$\alpha_{ij}$对于$i < i_0$持续依赖于$(f_1, \ldots, f_n)$，让我们证明$e_{i_0}$和$\alpha_{i_0 j}$持续依赖于$(f_1, \ldots, f_n)$。对于 $j < i_0$，$\overline{\alpha}_{i_0 j} = \Phi(f_{i_0}, e_j)$ 连续依赖于 $(f_1, \ldots, f_n)$ 归纳假设。另一方面，

$$
\Phi(f_{i_0}, f_{i_0}) = |\alpha_{i_0 1}|^2 + |\alpha_{i_0 2}|^2 + \cdots + |\alpha_{i_0, i_0 - 1}|^2 + \alpha_{i_0 i_0}^2 ,
$$

因此$\alpha_{i_0 i_0}$持续依赖于$(f_1, \ldots, f_n)$。因此

$$
e_{i_0} = (f_{i_0} - e_1 \alpha_{i_0 1} - \cdots - e_{i_0 - 1} \alpha_{i_0, i_0 - 1}) \alpha_{i_0 i_0}^{-1}
$$

持续依赖于$(f_1, \ldots, f_n)$。

从此以后设$E = K^n$，让我们取$\Phi$形式

$$
\overline{x}_1 y_1 + \cdots + \overline{x}_n y_n .
$$

回想一下，$\mathbf{U}(n, \mathbf{K})$表示相应的酉群。即使$\mathbf{K}$是不可交换的，我们仍将用$\mathbf{M}_n(\mathbf{K})$的上三角矩阵的$\mathbf{T}_1(n, \mathbf{K})$群来表示，其对角线元素都为1。

#### 命题 7 {#int-vii-s3-prop-7 .statement tag=09HJ}

*令$D_+^*$为对角线矩阵与对角线元素$> 0$的群。 映射 $(U, D, T) \mapsto UDT$ 是 $\mathbf{U}(n, \mathbf{K}) \times D_+^* \times \mathbf{T}_1(n, \mathbf{K})$ 到 $\mathbf{GL}(n, \mathbf{K})$ 的同胚。*

设$(\varepsilon_1, \ldots, \varepsilon_n)$为$K^n$的典范基。让$X \in \mathbf{GL}(n, K)$。那么E的$X \cdot \varepsilon_i = f_i$形式基。对于这个基$(f_i)$，我们可以将基$(e_i)$联系起来，如引理10。令$U$为酉自同构的矩阵 E 的变换 $\varepsilon_i$ 变为 $e_i$。然后

$$
U^{-1} \cdot f_i = \varepsilon_1 \alpha_{i1} + \varepsilon_2 \alpha_{i2} + \cdots + \varepsilon_i \alpha_{ii}
$$

$\alpha_{ii} > 0$ 为 $i = 1, 2, \ldots, n$。因此$X = UC$，其中$C$是矩阵

$$
\begin{pmatrix}
\alpha_{11} & \alpha_{21} & \cdots & \alpha_{n1} \\
0 & \alpha_{22} & \cdots & \alpha_{n2} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & \alpha_{nn}
\end{pmatrix}.
$$

此外，$U$和$C$连续依赖于X引理10。另一方面，公式（8）表明$C$可以与$D \in \mathbf{D}_+^*$一起放入形式$DT$， $T \in \mathbf{T}_1(n, K)$、$D$ 和 $T$ 持续依赖于 $C$。 分解 $X = UDT$ 的唯一性由引理 10 的唯一性性质得出。

命题 7 的同胚称为 $\mathbf{GL}(n, K)$ 的 *Iwasawa 分解*。

群 $G = \mathbf{D}_+^* \cdot \mathbf{T}_1(n, K)$ 是对角线元素为 $> 0$ 的 K 上三角形矩阵的集合。让我们将这个群与元素恒等元素$(z_{ij})$

$$
((z_{ii})_{1 \leq i \leq n}, (z_{ij})_{1 \leq i < j \leq n}) \in (\mathbf{R}_+^*)^n \times K^{n(n-1)/2}.
$$

与例 4 中的论证完全一样，人们发现对于这个群的度量（当 $K = \mathbf{R}$ 时），哈尔度量是*正确的*

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) \cdot \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i < j} dz_{ij} \right).
$$

然后§2, No. 9的应用第13条命题，我们可以看到，如果$\mathbf{GL}(n, K)$通过映射$(U, S) \mapsto US$与$\mathbf{U}(n, K) \times G$等同，则$\mathbf{GL}(n, K)$的哈尔测度由下式给出（当$K = \mathbf{R}$时）

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) \cdot \alpha \otimes \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i < n} dz_{ij} \right),
$$

其中$\alpha$表示$\mathbf{U}(n, K)$的Haar测度。

#### 例 8 {#int-vii-s3-n3-exa-8 .statement tag=09HK}

空间厄米特形式。

在这个例中，K总是表示域$\mathbf{R}, \mathbf{C}, \mathbf{H}$之一。我们写 $\delta = \dim_{\mathbf{R}} K$（因此 $\delta = 1, 2$ 或 4）。 厄米特形式 $\Phi$ 右向量空间 $K^n$ 可以写成

$$
\Phi(x, y) = \Phi(x_1, \ldots, x_n, y_1, \ldots, y_n) = \sum_{i,j=1}^n \overline{x_i} h_{ij} y_j
$$

对于所有$i$和$j$，$h_{ij} = \overline{h_{ji}}$。我们用$M_n(K)$的厄米特矩阵形成的$\mathbf{R}$上的$\mathfrak{H}$向量空间来表示。 映射$(h_{ij}) \mapsto \Phi$是$\mathfrak{H}$的同构到$K^n$上的厄米特形式的向量空间，这样我们就可以认同这两个空间。令$\mathfrak{H}_+^* \subset \mathfrak{H}$为$K^n$上非简并正厄米特形式的集合。 集合 $\mathfrak{H}_+^*$ 在 $\mathfrak{H}$ 中是*凸*；因为，如果$\Phi_1, \Phi_2$在$\mathfrak{H}_+^*$中并且$\lambda, \mu$是两个数$> 0$，使得$\lambda + \mu = 1$，则显然$\lambda \Phi_1 + \mu \Phi_2$是正厄米特形式；另一方面，如果$(\lambda \Phi_1 + \mu \Phi_2)(x, x) = 0$，则$\Phi_1(x, x) = \Phi_2(x, x) = 0$，因此$x = 0$，因此$\lambda \Phi_1 + \mu \Phi_2$是非简并的。现在让我们证明 $\mathfrak{H}_+^*$ 是 $\mathfrak{H}$ 的*开* 子集。令 S 为 $x = (x_1, \ldots, x_n) \in K^n$ 的集合，使得 $x_1 \overline{x}_1 + \cdots + x_n \overline{x}_n = 1$；这是 $K^n$ 的紧凑型子集；如果 $\Phi \in \mathfrak{H}_+^*$、函数 $x \mapsto \Phi(x, x)$ 是连续的且 $> 0$ 在 S 上，则其下确界为 $> 0$；如果$\Phi' \in \mathfrak{H}$足够接近$\Phi$，则$\Phi'(x, x) > 0$对于所有$x \in S$，因此$\Phi'$是正的且非简并的。

一般线性群$\mathbf{GL}(n, K)$在$\mathfrak{H}$向右连续运行$(X, \Phi) \mapsto \Phi \circ X$，即$(X, H) \mapsto t \overline{X} \cdot H \cdot X$，其中$H$表示厄米特矩阵相应的到$\Phi$。显然$\mathfrak{H}_+^*$在$\mathbf{GL}(n, K)$下是稳定的。更准确地说，由 *Alg.*，Ch. IX, §6, No. 1，科。 1 Th。 1、$^1$$\mathfrak{H}_+^*$是形式$\sum_{i=1}^n \overline{x_i} y_i$相应的的$\mathbf{GL}(n, K)$下的轨道到身份矩阵$I_n$。这个形式中的稳定子是$\mathbf{U}(n, K)$。通过App的引理2。 I、$\mathfrak{H}_+^*$可以与$\mathbf{GL}(n, K)/\mathbf{U}(n, K)$一起识别为拓扑同质空间。

对于每个$X \in \mathbf{GL}(n, K)$，令$\widetilde{X}$为*真实*向量空间$\mathfrak{H}$的自同构$H \mapsto t \overline{X} \cdot H \cdot X$。如果$\mu$表示哈尔测度加法群$\mathfrak{H}$，则有$\widetilde{X}^{-1}(\mu) = |\det \widetilde{X}| \cdot \mu$（§ 1, No. 10，第15号提案的Cor.1）。让我们证明

$$
| \det \widetilde{X} | = | N(X) |^\lambda ,
$$

其中 N 表示 $M_n(K)$ 中的范数 *被视为* $\mathbf{R}\text{-algebra}$，并且其中 $\lambda = 1 - \frac{\delta - 2}{\delta n}$。足以验证 (15) $X$ 运行超过系统

(1) 参见。 TVS，V, §2, No. 4，科。 1 Th。 2.

$\mathbf{GL}(n, K)$ 的生成元，因而（A，II, §10, No. 13，第 14 条命题第 2 条）对于以下型的 $X$：

a) $X$ 是形式映射矩阵
$$
(x_1, \ldots, x_n) \mapsto (x_{\sigma(1)}, \ldots, x_{\sigma(n)}),
$$
其中$\sigma \in \mathfrak{S}_n$。在这种情况下，$X$的幂等于1，因而$|\det \widetilde{X}| = |N(X)| = 1$。

b) $X$ 是形式映射矩阵
$$
(x_1, \ldots, x_n) \mapsto (ax_1, x_2, \ldots, x_n).
$$
那么，如果$(h_{ij}) \in \mathfrak{H}$，则有$\widetilde{X}((h_{ij})) = (h'_{ij})$，$h'_{11} = \overline{a} h_{11} a = |a|^2 h_{11}$，$h'_{1i} = \overline{a} h_{1i}$对应$i > 1$，$h'_{ij} = h_{ij}$对应$i > 1, j > 1$；因而
$$
|\det \widetilde{X}| = |a|^2 |a|^{\delta(n-1)} = |a|^{2+\delta(n-1)}.
$$
另一方面，如果$Y = (y_{ij}) \in M_n(K)$，则$XY = (y'_{ij})$与$y'_{1j} = ay_{1j}$和$y'_{ij} = y_{ij}$对于$i > 1$；因而$|N(X)| = |a|^{\delta n}$。 公式(15)再次得到验证。

c) $X$ 是形式映射矩阵
$$
(x_1, \ldots, x_n) \mapsto (x_1 + bx_2, x_2, \ldots, x_n).
$$
然后$\widetilde{X}((h_{ij})) = (h'_{ij})$与$h'_{11} = h_{11}$、$h'_{12} = h_{12} + h_{11} b$、$h'_{1i} = h_{1i}$对应$i > 2$，$h'_{22} = h_{22} + \overline{b} h_{12} + \overline{h}_{12} b + \overline{b} h_{11} b$、$h'_{2i} = h_{2i} + \overline{b} h_{1i}$对应$i > 2$，$h'_{ij} = h_{ij}$对应$i > 2, j > 2$。考虑到引理 6，可以看出$|\det \widetilde{X}| = 1$。我们可以类似地验证 $|N(X)| = 1$，它完成公式的证明 (15)。

由此成立，$\mathfrak{H}$上的测度$|N(H)|^{-\lambda/2} d\mu(H)$在$\mathbf{GL}(n, K)$下是不变的，因为
$$
\widetilde{X}^{-1}(|N(H)|^{-\lambda/2} d\mu(H)) = |N(\widetilde{X}(H))|^{-\lambda/2} \cdot |\det \widetilde{X}| d\mu(H)
= |N(H)|^{-\lambda/2} |N(X)|^{-\lambda} |\det \widetilde{X}| d\mu(H) = |N(H)|^{-\lambda/2} d\mu(H).
$$

如果$H \in \mathfrak{H}_+^*$，则$H = \widetilde{X}(I_n) = {}^t \overline{X} X$对于某些$X \in \mathbf{GL}(n, K)$，因而$N(H) = \overline{N(X)} N(X) > 0$。因而，在 $\mathfrak{H}_+^*$ 上，$\mathbf{GL}(n, K)$ (cf. §2, No. 6, Th. 3) 下的唯一（直到常数因子）测度不变量是测度
$$
d\gamma(H) = N(H)^{-\lambda/2} d\mu(H).
$$
特别是，
$$
d\gamma(H) = (\det H)^{-(n+1)/2} d\mu(H) \quad \text{when } K = \mathbf{R},
$$
$$
d\gamma(H) = (\det H)^{-n} d\mu(H) \quad \text{when } K = \mathbf{C}.
$$

### 习题{#int-vii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
