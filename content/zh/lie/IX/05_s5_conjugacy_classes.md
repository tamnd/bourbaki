---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 5
section_title: Conjugacy classes
lang: zh
source: lie-vii-ix
book_pages: 324-333, 405-409
pdf_pages: 0331-0340, 0412-0416
extraction: native
subsections:
    - "no": 1
      title: REGULAR ELEMENTS
      page: 324
      pdf_page: 331
    - "no": 2
      title: CHAMBERS AND ALCOVES
      page: 325
      pdf_page: 332
    - "no": 3
      title: AUTOMORPHISMS AND REGULAR ELEMENTS
      page: 327
      pdf_page: 334
    - "no": 4
      title: THE MAPS (G$\boldsymbol{/}$T) $\times \mathbf{T}\rightarrow$ G AND (G$\boldsymbol{/}$T) $\times \mathbf{A}\rightarrow \mathbf{G}_{\boldsymbol{r}}$
      page: 331
      pdf_page: 338
statements: 26
exercises: 12
content_sha256: 719cc9db98bf50fcf530d145503a1c2d3e0656b999a9d30db4239a34ab25c896
translated_from: content/en/lie/IX/05_s5_conjugacy_classes.md
translation_method: google
source_content_sha256: 67b7c3bf0335e1b8bfbe872472e7bd56c7dbf0d52741cf029286e2edabbf3e06
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 17218e28c01a545ae64f649011011cf48e6787a893425b5b2f239eb0a9e1dc86
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 5。 共轭类

我们保留§4的记号。

### 1. 正则元素

由科. 4 Th。 G 的 §2, no. 2、正则元素 $g$ 的 2 可以用以下任一属性来表征：

a) Ad $g$ 固定的$\mathfrak{g}$ 的子代数为嘉当子代数。

$b) Z(g)_0$是G的最大环面。

G 的正则元素的集合在 G 中是开稠密的。

在本段的其余部分中，我们用 G（分别为 T）的点的 $G_r$（分别为 $T_r$）集合表示 G 中的正则。当且仅当 $Z(g)_0$ 等于 T 时，G 属于到 $T_r$ 的元素 $g$； $G_r$的每个元素是$T_r($§2, no. 2的共轭到元素，Th。 2）。

T 属于到 $T_r$ 的元素 $t$ 当且仅当对于每个根 $\alpha \in R(G,T)$ 有 $t^{\alpha}\not= 1$；因而，T **--** $T_r$ 是 $R(G,T)$ 中 $\alpha$ 的 subtori Ker $\alpha$ 的并。

#### 命题 1 {#lie-ix-s5-prop-1 .statement tag=01DV}

将$n=$暗淡G。存在维数$n-3$的紧实解析流形V和映射$\varphi : V\rightarrow G$，其像是G **--** $G_r$。

设 $\alpha \in R(G,T)$；将 $V_{\alpha}= (G/$Z(Ker$\alpha$ ))$\times$ (Ker$\alpha$ )，并让 $\varphi_{\alpha}$ 成为从 $V_{\alpha}$ 到 G 的态射，这样，对于所有 $g\in G$ 和所有 $t\in$ Ker $\alpha$，我们有$\varphi_{\alpha}(\overline{g}, t) =gtg^{-1}$（我们用$\overline{g}$表示$g$模Z(Ker$\alpha$)的陪集）。那么$V_{\alpha}$是维数的紧实解析流形

暗淡 $V_{\alpha}=$ 暗淡 $G-$ 暗淡 Z(Ker $\alpha$ ) $+$ 暗淡 Ker$\alpha$

$=n-$（暗淡T + 2）+（暗淡$T-1$）$=n-3$

(§4, no. 5，Th.$1$)$;\varphi_{\alpha}$是实解析流形的态射，$\varphi_{\alpha}$的像由G共轭的元素到Ker$\alpha$的元素组成。现在只需将 V 变为流形 $V_{\alpha}$ 的和，并将 $\varphi$ 变为态射，在每个 $V_{\alpha}$ 上归纳出 $\varphi_{\alpha}$。

#### 注 {#lie-ix-s5-n1-rem-1 .statement tag=01DW}

如果 $Z(g)$ 是 G 的最大值环面，则称 G 的元素 $g$ 非常规则。如果且仅当 $w(g)\not=g$ 对于 $W_G(T) ($§4, no. 7 的每个非恒等元素 $w$，则 $g\in T,g$ 非常规则，命题 14）。因而，正则元素的集合是G的密集开子集（§2, no. 5，命题5的Cor.2）。

### 2. 房间和壁龛

用元素$x\in \mathfrak{t}$的$\mathfrak{t}_r$集合表示，使得exp$x$是正则的，在其他字属于到$T_r$。 $\mathfrak{t}$ 属于的元素 $x$ 到$\mathfrak{t}$ **--** $\mathfrak{t}_r$ 当且仅当存在根 $\alpha \in R(G,T)$ 使得$\delta (\alpha )(x)\in 2\pi i\mathbf{Z}$。对于每个根$\alpha \in R(G,T)$和每个整数$n$，用$x\in \mathfrak{t}$的$H_{\alpha ,n}$集合表示，使得$\delta (\alpha )(x) = 2\pi in$。 $H_{\alpha ,n}$被称为$\mathfrak{t}$的单数超平面，而$\mathfrak{t}$ **--** $\mathfrak{t}_r$是单数超平面的并。 $\mathfrak{t}$的凹室是$\mathfrak{t}_r$的连通的分量，而室是那些经过原点的单数超平面的并的$\mathfrak{t}$的补集的连通的分量（即$H_{\alpha ,0}=$） Ker$\delta (\alpha ),\alpha \in R(G,T)$）。

我们有 $\Gamma (T)\subset \mathfrak{t}$**--** $\mathfrak{t}_r$；表示由节点向量 (§4, no. 5) 生成的 $\Gamma (T)$ 的 $N(G,T)$ 子群；根据§4, no. 6的第11条命题，商$\Gamma (T)/N(G,T)$可以与G的基群等同。

最后，用 W 表示 G 相对于 T 的 Weyl 群，视为 T 的自同构和 $\mathfrak{t}$ 的群，并用仿射的自同构的 $W_a$（分别为 $W'_a$）群表示空间 $\mathfrak{t}$ 由 W 生成，并且翻译 $t_{\gamma}:x \rightarrow x+\gamma$ 为 $\gamma \in N(G,T)$（分别为 $\gamma \in \Gamma (T)$）。

令 $w\in W,\gamma \in \Gamma$ (T)、$\alpha \in R(G,T)$ 和 $n\in \mathbf{Z}$。我们有：

$$
w(H_{\alpha ,n}) = H_{w\alpha ,n},t_{\gamma}(H_{\alpha ,n}) = H_{\alpha ,n+\langle\gamma ,\alpha\rangle}
$$

由此可见，对于所有室 C 和所有 $w\in W,w(C)$ 都是室，对于所有凹室 A 和所有 $w\in W'_a,w(A)$ 都是凹室。请注意，当$X(T)\otimes \mathbf{R}$通过同构$(2\pi i)^{-1}\delta$与$\mathfrak{t}^*$识别时，$\mathfrak{t}$和群$W_a$的凹室是与根系关联的凹室和仿射Weyl群 $R(G,T)$（第VI, §2, no. 1章）。

#### 命题 2 {#lie-ix-s5-prop-2 .statement tag=01DX}

a) 群 $W_a$（分别为 $W'_a$）是 W 乘以 $N(G,T)$（分别为 $\Gamma (T)$）的半直接乘积； $W'_a$子群$W_a$是正常的。

b) 群 W（分别为 $W_a$）在集合房间（分别为凹室）上简单传递地运行。

c) 令 C 为房间，A 为凹室。那么$\overline{C}$（分别为A，分别为A）是W在$\mathfrak{t}$上的运算（分别为$\mathfrak{t}$上的$W_a$，以及$\mathfrak{t}$**--** $\mathfrak{t}_r$上的$W_a$）的基本域。如果$x\in \mathfrak{t}_r$和$w\in W_a$使得$w(x) =x$，则$w=$Id。

d) 对于每个房间C，都存在一个唯一的凹室A，使得$A\subset C$和$\gamma \in \frac{0}{A}.\in \overline{A}$。对于每个凹室 A，都存在一个唯一的 $\gamma \in N(G,T)$，使得

如果$w\in W$和$\gamma \in \Gamma$(T)，则$wt_{\gamma}w^{-1}=t_{w(\gamma)}$和$wt_{\gamma}w^{-1}t^{-1}_{\gamma}=t_{w(\gamma)-\gamma}$，以及$w(\gamma )-\gamma \in N(G,T)$；这立即意味着a)。 命题的其余部分来自第 1 章。 VI, §1, no. 5 和§2，编号。 1 和 2。

#### 推论 1 {#lie-ix-s5-prop-2-cor-1 .statement tag=01DY}

令 A 为其封闭的 $\mathfrak{t},\overline{A}$ 的凹室，以及 A 在 $W'_a$ 中的 $H_A$ 稳定子。

a) 群 $W'_a$ 是$H_A$ 乘以$W_a$ 的半直接乘积。

b) 指数映射 $\overline{A}\rightarrow T$ 和典范嵌入 $T\rightarrow G$ 诱导通过通向商和子集同胚

$\overline{A}/H_A\rightarrow T/W\rightarrow G/$整数(G)

$A/H_A\rightarrow T_r/W\rightarrow G_r/$Int(G)。

让$w'\in W'_a$；则$w'(A)$是$\mathfrak{t}$的凹室，且存在$W_a$的（命题$2b$）$)$唯一元素$w$使得$w(A) =w'$(A)，即$w^{-1}w'\in H_A$。由于 $W_a$ 在 $W'_a$ 中是正规的，这就证明了 a)。

$\overline{A}$的典范嵌入变成$\mathfrak{t}$诱导连续的双射$\theta :\overline{A}\rightarrow$$\mathfrak{t}/W_a$（命题$2c$）$)$，这是一个同胚，因为A是紧的。由于$W_a$在$W'_a$中是正常的，群$H_A$在$\mathfrak{t}/W_a($代数上规范地运行，第1章。 I, §5, no. 4）和$\mathfrak{t}/W'_a$可以用商$(\mathfrak{t}/W_a)/H_A$来识别； 映射$\theta$与$H_A$的运算兼容，因此诱导通过到商同胚$A/H_A\rightarrow \mathfrak{t}/W'_a$。此外，exp$_{\Gamma}$诱导是从$\mathfrak{t}/\Gamma (T)$到T的同态，因此也是从$\mathfrak{t}/W'_a$到$T/W$的同态。 断言 b) 由此得出，Cor. §2, no. 4第 5 号提案 1。

#### 注 1 {#lie-ix-s5-n2-rem-1 .statement tag=01DZ}

群 $H_A$ can be identified naturally with $\Gamma (T)/N(G,T)$, hence also with $\pi_1(G)$. Thus, it 约化 to 单位元素 when G is simply-connected.

#### 注 2 {#lie-ix-s5-n2-rem-2 .statement tag=01E0}

设 $x\in A$；那么exp $x\in T_r$，所以Z(exp $x$)$_0= T$。 Further, exp $x$ is very regular (no. 1, 注) if and only if $w(x)\not=x$ for all $w\in W'_a$ distinct from the identity.由科. 1, this also means that $h(x)\not=x$ for all $h\in H_A$ distinct from the identity. In particular, if G is simply-connected, then $Z_G(t) = T$ for all $t\in T_r$, and every 正则元素 of G is very regular.

#### 注 3 {#lie-ix-s5-n2-rem-3 .statement tag=01E1}

The special 点 of $W_a$ (Chap. VI, §2, no. 2) are 元素 $x$ of $\mathfrak{t}$ such that $\delta (\alpha )(x)\in 2\pi i\mathbf{Z}$ for all $\alpha \in R(G,T) ($loc. cit., Prop. 3), that is such that exp $x\in C(G) ($§4, no. 4, Prop. 8).对于这样的元素$x$，我们对所有$w\in W$有$wx-x\in N(G,T)$（第VI, §1, no. 9章，第27条提案），因而$W_a$和$W'_a$重合中的$x$有稳定子。设S为A的特殊点的集合；这是从前文和 Cor 得出的。 1 that 群 $H_A$ operates freely on S, and that the exponential 映射诱导双射 from $S/H_A$ to C(G).

#### 推论 2 {#lie-ix-s5-prop-2-cor-2 .statement tag=01E2}

Let C be a chamber of $\mathfrak{t}$ and $\overline{C}$ its closure. 典范嵌入 $\overline{C}\rightarrow \mathfrak{t}\rightarrow \mathfrak{g}$ 诱导 by passage to 商 homeomorphisms

$\overline{C}\rightarrow \mathfrak{t}/W\rightarrow \mathfrak{g}/$广告(G)。

The canonical 映射 $\overline{C}\rightarrow \mathfrak{t}$ and $\mathfrak{t}\rightarrow \mathfrak{t}/W$ are proper (General 拓扑, Chap. III, §4, no. 1, Prop. $2c$)$)$. 映射 $\overline{C}\rightarrow \mathfrak{t}/W$ is continuous, proper and bijective (Prop. $2c$)$)$; thus, it is a homeomorphism, hence 推论 in view of the Cor. §2, no. 5第6号提案。

#### 注 4 {#lie-ix-s5-n2-rem-4 .statement tag=01E3}

Denote by $\mathfrak{g}_{reg}$ 集合 of 正则元素 of $\mathfrak{g}$ (Chap. VII, §2, no. 2, Def. 2) and put $\mathfrak{t}_{reg}=\mathfrak{t}\cap \mathfrak{g}_{reg}$.对于$x\in \mathfrak{t}$，我们有

det(X$-$广告$_{\mathfrak{g}}x$)$= X^{dim}\prod_{\alpha\in R(G,T)}^{\mathfrak{t}}(X-\delta (\alpha )(x))$,

因而，$\mathfrak{t}_{reg}$是元素的集合，$\mathfrak{t}$的$x$，这样对于所有$\alpha \in R(G,T)$来说，$\delta (\alpha )(x)\not= 0$，即$\mathfrak{t}$的室的并（所以$\mathfrak{t}_r\subset \mathfrak{t}_{reg}$）。因而$C\cap \mathfrak{t}_{reg}= C$，所以我们有同胚

$C\rightarrow \mathfrak{t}_{reg}/W\rightarrow \mathfrak{g}_{reg}/$广告(G)。

#### 推论 3 {#lie-ix-s5-prop-2-cor-3 .statement tag=01E4}

假设G是单连通的；令$g$为G的正则元素。存在G的最大环面S和L(S)的凹室A，两者都是唯一确定的，使得$g\in$exp(A)和$0\in \overline{A}$。

我们可以假设$g$属于到$T_r($§2, no. 2，Th。 2）。令$x$为$\mathfrak{t}_r$的元素，使得exp$x=g$，并令$A'$为$\mathfrak{t}$包含$x$的凹室。 $\mathfrak{t}$ 的凹室 A，使得 $g\in$ exp(A) 是 $\gamma \in \Gamma (T)$ 的凹室 $A'-\gamma$；因此，断言是从命题$2d)$得出的。

### 3. 自同构和正则元素

#### 引理 1 {#lie-ix-s5-lem-1 .statement tag=01E5}

设$u$为G的自同构，H集合为其固定的点。

a) H 是 G 的闭子群。

b) 如果 $H_0$ 是 G 的中心，则 G 是可交换的（因此 G = T）。

断言 a) 很清楚。为了证明b)，我们可以通过D(G)来替换G（§1，命题4的Cor.1），因此可以假设G是半单。那么，如果$H_0$是G的中心，我们有$L(H) =\{0\}$，所以自同态$L(u)-$Id of $\mathfrak{g}$是双射的。令$f$为流形G的自同态，由$f(g) =u(g)^{-1}g$对$g\in G$定义；它是étale，因为如果$g\in G$和$x\in \mathfrak{g}$，我们有$T(f)(xg) =u(g)^{-1}(x-L(u)(x))g$，所以$f$在$g$的切线映射是双射的。由此可见，$f$的像是开紧的，因此重合与G，因为G是连通的。现在让 E 为 G (§4, no. 10, Def. 3) 的框架，$u(E)$ 是$u$ 下的像。根据 loc. 19 号提案。如上所述，G 存在元素 $h$，使得 (Int $h$)$(E) =u(E)$。令 $g\in G$ 使得 $h=f(g) =u(g)^{-1}g$；然后

$u\circ$整数$g=$（整数$u(g)$）$\circ u=$整数$g\circ$（整数$h$）$^{-1}\circ u$，

所以框架(Int $g$)$(E)$在$u$下是稳定的。如果(Int $g$)$(E) = (T_1,B,(U_{\alpha})_{\alpha\in B})$，则$\sum U_{\alpha}\in L(H)$；因为$L(H) =\{0\}$，这意味着$B =\emptyset$，所以$G = T_1$，并且G是可交换的。

#### 引理 2 {#lie-ix-s5-lem-2 .statement tag=01E6}

设$x$是T的元素，S是T的子托。如果$Z(x)\cap Z(S)$约化对T恒等式分量，则存在S的元素$s$，使得$xs$是正则的。

对于所有$\alpha \in R(G,T)$，令$S_{\alpha}$是S的元素$s$的S由……组成的子流形，使得$(xs)^{\alpha}= 1$。如果 S 不存在元素 $s$ 使得 $xs$ 是正则，则 S 是子流形 $S_{\alpha}$ 的并，因此等于其中之一。因此，$R(G,T)$中存在$\alpha$，使得$(xs)^{\alpha}= 1$对于所有$s\in S$；但这意味着 $x^{\alpha}= 1$ 和 $\alpha |S = 1$，因此 $Z(x)\cap Z(S)\supset$ Z(Ker $\alpha$ )，因此引理。

#### 引理 3 {#lie-ix-s5-lem-3 .statement tag=01E7}

假设 G 是单连通的。令C为$\mathfrak{t}$的腔室，且$u$为G的自同构，使得T和C在$u$下稳定。然后将由$u$固定的T的点与集合连接起来。

由于 G 是单连通的，$\Gamma (T)$ 由节点向量 $K_{\alpha}$ $(\alpha \in R(G,T))$ 生成，因此具有 $K_{\alpha}$ 系列的基由……组成，其中 $\alpha$ 属于到基 B(C)由C定义（第VI, §1, no. 10章）。因此，只要证明，如果$\varphi$是环面T的自同构，留下$\Gamma$(T)的稳定基，则$\varphi$的固定点的集合是连通的。将这个基分解为$\varphi$生成的群的轨道的不相交的并，我们就简化为$T =\mathbf{U}^n$和$\varphi$是自同构$(z_1, . . . , z_n) \rightarrow (z_2, . . . , z_n, z_1)$的情况；在这种情况下，$\varphi$的固定点是$z\in \mathbf{U}$的点$(z, z, . . . , z)$，其中形式与T的子群相连。

#### 命题 3 {#lie-ix-s5-prop-3 .statement tag=01E8}

令$u$为G的自同构，并令$x$为由$u$固定的G的点。

a) 存在$\mathfrak{g}$的元素$a$，由$L(u)$和Ad$x$固定，使得$x$exp$a$是正则的。

b) 存在由$u$固定且与$x$交换的G的正则元素$g$。

令H为$u, S$的固定点的群和$Z(x)\cap H$的最大环面，且K为$Z(S)\cap Z(x)$的恒等式分量。这是 G 的连通闭子群；此外，Cor. 5 Th。 §2, no. 2的2个，存在最大环面G包含S和$x$，所以K最大为秩和包含S和$x$。另一方面，K 在 $u$ 下是稳定的，因为 S 和 $x$ 是；用K中$u$的固定点的V集合表示。则

$$
S\subset V_0\subset K\cap H\subset Z(S)\cap Z(x)\cap H
$$

所以$V_0$包含在$(Z(x)\cap H)_0$中S的扶正子中；但后者约化到S（loc.cit.，Cor.6），因此最终$V_0= S$。 引理 1 现在意味着 K 是可交换的，因此是 G 的最大值环面（因为它是连通的且最大值为秩）。它包含 S 和$x$，等于$Z(S)\cap Z(x)$ 的恒等式分量； 断言 a) 现在由引理 2 推出。我们通过取 $g=x$ exp $a$ 推导出 b)。

#### 推论 {#lie-ix-s5-n3-cor-1 .statement tag=01E9}

令$\mathfrak{s}$为紧李代数，令$\varphi$为$\mathfrak{s}$的自同构。存在由$\varphi$固定的$\mathfrak{s}$的正则元素。

替换 $\mathfrak{s}$乘以$\mathscr{D}\mathfrak{s}$，我们可以假设$\mathfrak{s}$是半单。令 S 为紧单连接李群与李代数 $\mathfrak{s}$，并令 $u$ 为 S 的自同构，使得 $L(u) =\varphi$。命题3意味着$\mathfrak{s}$存在元素$a$，由$\varphi$固定，使得exp$a$在S中是正则；特别是，$a$在$\mathfrak{s}$（no. 2，注4）中是规则的。

#### 定理 1 {#lie-ix-s5-thm-1 .statement tag=01EA}

设 $u$ 为连通的紧李群 G 的自同构。

a) G 的$u$包含正则元素固定点的群恒等式分量。

b) 存在 G 的最大环面 K 和L(K) 的室，在 $u$ 下稳定。

c) 如果 G 是单连通的，则 $u$ 的固定点的集合是连通的。

断言 a) 是命题 3 的特例 $x=e$。我们现在假设 G 是单连通的并证明 b) 和 c)。令$x$为由$u$固定的G的元素，并令$g$为G的正则元素，由$u$固定并与$x$交换（命题3）。 $g$的扶正器K是G的最大环面（no. 2，注2），在$u$、包含于、$x$和$g$下稳定。由科.根据no. 2的命题2的3，存在L(K)的唯一凹室A，使得$g\in$exp A和$0\in A$；由于 $g$ 由 $u, L(u)$ 叶 A 固定，因此 L(K) 包含于 A 的室也是稳定的。这证明了 b);此外，由$u$固定的K的点的集合连接(引理3)和包含$x$和$e$，因此$c) ($一般拓扑，第1章。 I, §11, no. 1，提案 2）。

一般情况下还有待证明b)。现在，如果$\widetilde{D}(G)$是D(G)的通用覆盖，并且如果$f: \widetilde{D}(G)\rightarrow G$是规范的态射，则存在$\widetilde{D}(G)$的自同构$\widetilde{u}$使得$f\circ \widetilde{u}=u\circ f$。如果$\widetilde{K}$是$\widetilde{D}(G)$的最大值环面，并且$\widetilde{C}$是$L( \widetilde{K})$的一个室，在$\widetilde{u}$下稳定（这已经被证明存在），则存在（§2, no. 3，注2）一个唯一的最大值G 的环面 K 和L(K) 的独特室C 使得$\widetilde{K} =f^{-1}(K)$ 和$\widetilde{C} = L(f)^{-1}$(C)，我们立即看到K 和C 在$u$ 下是稳定的，因此在一般情况下断言 b)。

#### 推论 1 {#lie-ix-s5-thm-1-cor-1 .statement tag=01EB}

假设$\mathbf{Z}$-模块$\pi_1(G)$无扭转。

a) G 的每个元素的扶正器都是连通的。

b) G 属于的任意两个交换元素到相同的最大值环面。

由科. §4, no. 6第11条命题3，D(G)是单连通的。我们有$G = C(G)_0.D(G)$；让 $x\in G$；写出$x=uv$，加上$u\in C(G)_0$和$v\in D(G)$。然后$Z(x) = C(G)_0.Z_{D(G)}(v)$。由 Th. $1c), Z_{D(G)}(v)$ 已连通，因此 $Z(x)$ 已连通，因此 a)。因此，通过 Cor. 3 Th。 §2 中的 2 个，没有。 $2, Z(x)$ 是 G 包含于 $x$ 最大环面的并，因此 b)。

#### 推论 2 {#lie-ix-s5-thm-1-cor-2 .statement tag=01EC}

令 $\Gamma$ 为 Aut(G) 的紧子群，其中性质：

(*) 存在$\Gamma$的元素$u_1, . . . , u_n$，使得对于所有$i$，由$u_1, . . . , u_i$生成的$\Gamma$的子群的闭包$\Gamma_i$是$\Gamma$的正规子群，并且$\Gamma_n=\Gamma$。

那么，在运算 $\Gamma$ 下，存在 G 的最大环面稳定。

我们通过归纳对G的维数进行论证。显然，我们可以假设$u_1\not=$Id；则$u_1$固定点的子群H与G不同，且在$\Gamma$的运算下稳定。而且，由于$\Gamma$是紧的，Aut(H$_0$)中$\Gamma$的像是$\Gamma$的商，因此也满足条件(*)。到归纳假设时，H在$\Gamma$下稳定存在最大环面 S。 G中S的扶正器K是连通的（§2, no. 2，Cor.5）并且在$\Gamma$下稳定；这是 G 的最大环面，因为 G 的 $H_0$ 包含正则元素 (Th. $1a$)$)$ 是 S 的共轭到元素（见上文，Cor. 4）。

#### 推论 3 {#lie-ix-s5-thm-1-cor-3 .statement tag=01ED}

令H为李群且$\Gamma$是H的紧子群。假设$H_0$是紧的并且$\Gamma$满足Cor的条件(*)。 2. 则存在最大环面 T 为 $H_0$，使得 $\Gamma \subset N_H(T)$。

#### 推论 4 {#lie-ix-s5-thm-1-cor-4 .statement tag=01EE}

紧李群的每个幂零子群都包含在最大环面的归一化器中。

令 H 为紧李群，N 为 H 的幂零子群。则 N 的闭包 $\Gamma$ 也是幂零群（第 III, §9, no. 1 章，第 1 条命题第 2 章），鉴于 Cor.1，它就足够了。 3、证明$\Gamma$满足条件(*)。现在 $\Gamma_0$ 是一个连通紧致幂零李群，因此是环面（§1, no. 4，第 4 条命题第 1 条），并且存在 $\Gamma$ 生成的的元素 $u_1$ 的稠密子群 $\Gamma_0($一般拓扑，第 1 章VII, §1, no. 3，第 8 条提案之前的文字）。 有限群$\Gamma /\Gamma_0$是幂零的，并且存在$\widetilde{u}_2, . . . ,\widetilde{u}_n\in \Gamma /\Gamma_0$生成的$\Gamma /\Gamma_0$，因此$(\widetilde{u}_2, . . . ,\widetilde{u}_r)$生成的$\Gamma /\Gamma_0$的子群对于$r= 2, . . . , n($代数来说是正常的，第1章。 I, §6, no. 5，周四。 1 和 no. 7，Th。 4).那么，如果$u_2, . . . , u_n$是$\Gamma$中$\widetilde{u}_2, . . . ,\widetilde{u}_n$的代表，则序列$(u_1, . . . , u_n)$具有所需的属性。

#### 例 {#lie-ix-s5-n3-exa-1 .statement tag=01EF}

取$G =\mathbf{U}(n,\mathbf{C})$。稍后我们将看到，G 中对角线矩阵的子群是 G 的最大值环面，并且其归一化器是单项式矩阵的集合（代数，第 II, §10, no. 7、例） G 中的 II)

我们结论，如果$\Phi$是有限维复数向量空间V上的分离正厄米特形式并且$\Gamma$是$\mathbf{U}(\Phi )$的幂零子群，则存在基 of V 其中矩阵 of 元素 of $\Gamma$ 是单项式（“Blichtfeldt 的定理”）。

### 4. 映射 (G$\boldsymbol{/}$T) $\times \mathbf{T}\rightarrow$ G 和 (G$\boldsymbol{/}$T) $\times \mathbf{A}\rightarrow \mathbf{G}_{\boldsymbol{r}}$

映射 $(g, t) \rightarrow gtg^{-1}$ 从 $G\times T$ 到 G 诱导通过解析流形商态射

$$
f: (G/T)\times T\rightarrow G
$$

这是满射的 (§2, no. 2, Th. 2)。由限制、$f$ 诱导一个满射态射

$$
f_r: (G/T)\times T_r\rightarrow G_r
$$

通过合成和Id$_{G/T}\times$exp$_T$，我们得到态射，也是满射的，

$$
\varphi : (G/T)\times \mathfrak{t}\rightarrow G
$$

$$
\varphi_r: (G/T)\times \mathfrak{t}_r\rightarrow G_r
$$

最后，如果 A 是 $\mathfrak{t},\varphi_r$ 诱导的凹室，则满射态射

$$
\varphi_A: (G/T)\times A\rightarrow G_r
$$

我们定义W在$G/T$上的右运算如下：设$w\in W$和$u\in G/T$； $N_G(T)$的提升$w$到元素$n$和G的$u$到元素$g$。则$G/T$中$gn$的像不依赖于$n$ 和 $g$ 中的选择；我们用$u.w$表示。

对于这个运算，W确实在$G/T:$上自由运算，前面的记号，假设$u.w=u$；然后$gn\in gT$，所以$n\in T$和$w= 1$。

我们在$(G/T)\times T$上定义右运算通过

$$
(u, t).w= (u.w, w^{-1}(t)),u\in G/T, t\in T, w\in W
$$

以及 $(G/T)\times \mathfrak{t}$ 上 $W'_a$ 的右运算

$$
(u, x).\omega = (u.\omega , \omega^{-1}(x)),u\in G/T, x\in \mathfrak{t}, \omega \in W'_a
$$

其中$\overline{\omega}$是商$W'_a/\Gamma (T) = W$中$\omega$的像。

如果A是$\mathfrak{t}$的凹室，并且如果$H_A$是稳定A的$W'_a$的子群，我们通过$(G/T)\times A$上的$H_A$的限制运算得到。

这些不同的运算与态射$f, \varphi$和$\varphi_A:$相容的$u\in G/T, t\in T, x\in \mathfrak{t}, y\in A, w\in W, \omega \in W'_a, h\in H_A$，我们有

$$
f((u, t).w) =f(u, t), \varphi ((u, x).\omega ) =\varphi (u, x), \varphi_A((u, y).h) =\varphi_A(u, y)
$$

#### 引理 4 {#lie-ix-s5-lem-4 .statement tag=01EG}

令$g\in G,t\in T$，并令$\overline{g}$为$G/T$中$g$的像。通过左平移，认同 $G/T$（分别为 T、分别为 G）在 $\overline{g}$（分别为 $t$、分别为 $gtg^{-1}$）与 $\mathfrak{g}/\mathfrak{t}$（分别为 $\mathfrak{t}$、分别为 $\mathfrak{g}$）的切线空间通过左平移$\gamma (g)$ $g$（分别$t$、$gtg^{-1}$）。然后，$f$在$(\overline{g}, t)$处的切线映射可与定义如下的线性映射$f': (\mathfrak{g}/\mathfrak{t})\times \mathfrak{t}\rightarrow \mathfrak{g}$识别：如果$z\in \mathfrak{g}, x\in \mathfrak{t}$，并且如果$\overline{z}$表示$\mathfrak{g}/\mathfrak{t}$中$z$的像，则

$f'(\overline{z}, x) =$（广告$gt^{-1}$）$(z-$（广告$t$）$z+x)$。

令 F 为从 $G\times T$ 到 T 的映射，使得 $F(g, t) =gtg^{-1}$。从$F\circ (\gamma (g)$，Id$_T) =$ Int $g\circ F$开始，我们有$T_{(g,t)}(F)(gz, tx) = T_t$(Int $g$)$\circ T_{(e,t)}(F)(z, tx)$；由章。 III, §3, no. 12，第 46 号提案，

$T_{(e,t)}(F)(z, tx) =t$((广告$t^{-1}$)$z-z$)$+tx=t$((广告$t^{-1}$)$(z-$(广告$t$)$z+x$))

因而

$T_{(g,t)}(F)(gz, tx) =gtg^{-1}$((广告$gt^{-1}$)$(z-$(广告$t$)$z+x$))。

引理紧接着从公式到商。

#### 命题 4 {#lie-ix-s5-prop-4 .statement tag=01EH}

a) 令$g\in G, t\in T, x\in \mathfrak{t}$，并令$\overline{g}$为$G/T$中$g$的像。以下条件是等价的：

(i) $t\in T_r$（分别为$x\in \mathfrak{t}_r$）。

(i bis) 元素 $f(\overline{g}, t)$ (resp. $\varphi (\overline{g}, x)$) 在 G 中是正则。

(ii) 映射 $f$（分别为 $\varphi$）是在点 $(\overline{g}, t)$（分别为 $(\overline{g}, x)$）处的浸没。

(ii之二) 映射 $f$（分别为$\varphi$）的版本为点 $(\overline{g}, t)$（分别为$(\overline{g}, x)$）。

b) 映射 $f_r$（分别$\varphi_r$、$\varphi_A$）使 $(G/T)\times T_r$（分别$(G/T)\times \mathfrak{t}_r$、$(G/T)\times A$）成为 $G_r$ 和群 W（分别$W'_a$）的主覆盖，分别$H_A$）。

a) (i)和(i之二)的等价是明确的； (ii)和(ii之二)的结果来自关系dim((G$/T$)$\times T$)$=$dim((G$/T$)$\times \mathfrak{t}$)$=$dim(G)。当且仅当 $\mathfrak{g}=\mathfrak{t}+$ Im(Ad $t-$Id) 时，引理 4，$f$ 是点 $(\overline{g}, t)$ 的淹没，这意味着 $t$ 是规则的。最后，由于 $\varphi =f\circ$ (Id$_{G/T}\times$ exp$_T$)$,\varphi$ 的 étale 为点 $(\overline{g}, x)$ 当且仅当 $f$ 的 étale 为点 $(\overline{g}$，exp $x$)，通过前面的方法$x$属于至$\mathfrak{t}_r$。

b) 态射 $f_r, \varphi_r, \varphi_A$ 因此是étale。另一方面，W 在$G/T$ 上自由运行，更不必说在$(G/T)\times T$ 上自由运行。设G中的$g, g'$和$T_r$中的$t, t'$使得$f(\overline{g}, t) =f(\overline{g}', t')$；然后将 Int $g^{-1}g'$ 映射 $t'$ 到 $t$，因此将 T 归一化，因为 W 映射 $(\overline{g}, t)$ 中的 $T = Z(t)_0= Z(t')_0$ 和 $g^{-1}g'$ 的类 $w$ 为$(\overline{g}', t')$。由此可见，$f_r$ 是群 W 的主覆盖；这立即意味着$\varphi_r$是群$W'_a$的主覆盖，因此通过限制连接到$(G/T)\times \mathfrak{t}_r$的分量$(G/T)\times A$，$\varphi_A$是群$H_A$的主覆盖。

#### 注 1 {#lie-ix-s5-n4-rem-1 .statement tag=01EI}

根据§2, no. 4的命题3，流形$(G/T)\times A$是单连通的。由此可见$\varphi_A$是$G_r$的万能覆盖；由于 $\pi_1(G_r)$ 与 $\pi_1(G)$ 自然同构（no. 1，第 1 条命题和通则拓扑，第 XI 章，正在准备中），我们恢复了$\pi_1(G)$ 可以与 $H_A$（即$\Gamma (T)/N(G,T)$）识别的事实。

#### 注 2 {#lie-ix-s5-n4-rem-2 .statement tag=01EJ}

$\varphi_A$到$W\times A\subset (G/T)\times A$的限制使$W\times A$成为$T_r$与群$H_A$的主覆盖。这样我们就恢复了Cor。 no. 2 的第 2 号提案 1。

#### 注 3 {#lie-ix-s5-n4-rem-3 .statement tag=01EK}

用指数映射下的$G_r$的$\mathfrak{g}_r$逆像和由exp$_G$诱导的$\varepsilon :\mathfrak{g}_r\rightarrow G_r$映射表示。 映射$(g, x) \rightarrow$（广告$g$）$(x)$从$G\times \mathfrak{t}_r$到$\mathfrak{g}_r$定义，途经商映射$\psi_r: (G/T)\times \mathfrak{t}_r\rightarrow \mathfrak{g}_r$。我们有$\varepsilon \circ \psi_r=\varphi_r$。令 $w\in W, \gamma \in \Gamma (T)$ 和 $\omega \in W'_a$ 使得 $\omega (z) =w(z) +\gamma$ 对于所有 $z\in \mathfrak{t}$；那么 $\psi_r((\overline{g}, x)\omega ) =\psi_r(\overline{g}, x)-$ (Ad $g$)$(\gamma )$ 对应 $g\in G, x\in \mathfrak{t}_r$，所以 $\psi_r((\overline{g}, x)\omega ) =\psi_r(\overline{g}, x)$ 当且仅当 $\gamma = 0$。由此可见（cf.概述拓扑，第XI，准备中）$\psi_r$是$\mathfrak{g}_r$与群W的主覆盖，$\varepsilon :\mathfrak{g}_r\rightarrow G_r$是与主覆盖$\varphi_r$相关的覆盖，其纤维同构于$W'_a$-设置$W'_a/W$。

### 习题 {#lie-ix-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
