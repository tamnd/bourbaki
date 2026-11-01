---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 15
section_title: Brauer Groups
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.277-A VIII.284
pdf_pages: 0294-0301
extraction: native
subsections:
    - "no": 1
      title: Classes of Algebras
      page: 277
      pdf_page: 294
    - "no": 2
      title: Definition of the Brauer Group
      page: 278
      pdf_page: 295
    - "no": 3
      title: Change of Base Field
      page: 281
      pdf_page: 298
    - "no": 4
      title: Examples of Brauer Groups
      page: 283
      pdf_page: 300
statements: 12
exercises: 2
content_sha256: 1f32c39c6966218f20539bfef09843b02f6621846f985be4aae945ef297c75aa
translated_from: content/en/alg/VIII/15_s15_brauer_groups.md
translation_method: google
source_content_sha256: de0ee49b9fce0132064e5387825b803ddb4c6aeb3c6c606b44846dc5403449fc
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 321238357e1521bdda043de86b591160481d313afebf6e1b7722694f3e0d99de
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 15。 布劳尔群

在这个截面中，K是交换域。

### 1. Classes of Algebras

我们用 Iso$_K(A,B)$ 关系表示

“A 和 B 是 K-代数有限次数同构。”

这是关于 A 和 B 的等价关系。设 A 为有限次数的 K-代数； A 的类，表示为 cl(A)（或有时 cl$_K$(A)），对于关系 Iso$_K($集合理论，II, §6, No. 9、p. 122，对象的类相当于 A。由定义，cl(A)与A K-代数同构；当且仅当有限次数中的两个K-代数同构时，它们才属于同一个类。

我们用对$(W, \mu)$的$\mathscr{A}$集合表示，其中W是$K^{(\mathbf{N})}$的线性子空间，它是K上的有限维，$\mu$是从$W\times W$到W的K双线性映射到W，使W成为（结合且单位的） K-代数。 有限次数的每个 K-代数都同构于这样的代数。按地点。前述，关系

“$\alpha$是有限次数的K-代数中的类”

因此在$\alpha ($集合理论中是集合化，II, §1, No. 4，p. 68）。我们用$\mathscr{C}_K$表示有限次数的K-代数、类的集合。

#### 命题 1 {#alg-viii-s15-prop-1 .statement tag=00HV}

集合 $\mathscr{C}_K$，赋予由 $(\alpha , \beta )\mapsto$ cl($\alpha \otimes_K\beta$ ) 给出的合成律，是一个可交换幺半群。 $\mathscr{C}_K$的单位元素是K-代数K的类$\varepsilon$。此外，如果A和B是有限次数的K-代数，那么我们有关系

(1) cl(A $\otimes_KB$) $=$ cl(A) cl(B)。

设A、B、C为有限次数的K-代数，分别为类、$\alpha$、$\beta$、$\gamma$。 K-代数 A 和 $\alpha$ 是同构的，B 和 $\beta$ 也是同构的。 因而，K-代数$A\otimes_KB$和$\alpha \otimes_K\beta$是同构的，我们有cl(A$\otimes_KB$)$=$cl($\alpha \otimes_K\beta$)，它给出公式(1)。 It follows that $(\alpha \beta )\gamma$ is the class of the K-algebra $(A\otimes_KB)\otimes_KC$ and $\alpha (\beta \gamma )$ that of the K-algebra $A\otimes_K(B\otimes_KC)$. 现在，这些K-代数是同构的（III, §4, No. 1，p. 461），所以我们有等式$(\alpha \beta )\gamma =\alpha (\beta \gamma )$。 类似地，关系$\alpha \varepsilon =\varepsilon \alpha =\alpha$由K-代数$A\otimes_KK, K\otimes_KA$和A同构得出，关系$\alpha \beta =\beta \alpha$由代数$A\otimes_KB$和$B\otimes_KA$同构得出。

在集合$\mathscr{C}_K$、关系“$\alpha$和$\beta$是莫里塔等价代数”是等价关系（VIII、p. 100）。 $\mathscr{C}_K$、VIII、p. 111的命题13、d)与合成的律兼容。我们用$\mathscr{M}_K$表示$\mathscr{C}_K$的商幺半群，用这个等价关系和从$\mathscr{C}_K$到$\mathscr{M}_K$的$\varphi$典范同态。对于有限次数的每个 K-代数 A，我们用 $\varphi$ 表示 cl(A) 的 [A] 像。如果 A 和 B 是有限次数的 K-代数，那么我们有 [A] = [B] 当且仅当 K-代数 A 和 B 是 Morita 等价的；此外，我们还有关系

$$
[A\otimes_KB] = [A][B] \tag{2}
$$

在幺半群$\mathscr{M}_K$中。

#### 引理 1 {#alg-viii-s15-lem-1 .statement tag=00HW}

设 A 为有限次数的 K-代数，K 上有限次数的 D 域。 当且仅当存在整数 $n\geqslant 1$ 且 A 与 $\mathbf{M}_n(K)$ 同构时，$\mathscr{M}_K$ 中才有 [A] = [D]。

通过定义，我们有 [A] = [D] 当且仅当存在可逆 $(A$, D)-双模，即 (VIII, p. 101, 定理 1), 非零有限维的右向量空间 V 在 D 上赋予同构 K-代数$A\rightarrow$结束$_D(V)$。接下来是引理1。

### 2. Definition of the Brauer Group

我们用形式[A]的$\mathscr{M}_K$的元素的Br(K)集合表示，其中A是K上有限次数的中心单代数。

#### 命题 2 {#alg-viii-s15-prop-2 .statement tag=00HX}

集合 Br(K) 是$\mathscr{M}_K$ 的可逆元的集合，其中Br(K) 的元素 [A] 的倒数是$[A^o]$。因而，幺半群 $\mathscr{M}_K$ 上的合成律赋予 Br(K) 结构阿贝尔的群。

设 A 是 K 上有限次数的中心单代数。代数 $A^o$ 是 K 上有限次数的中心简单（VIII，p. 251）。 代数 $A\otimes_KA^o$ 与矩阵代数 $\mathbf{M}_n$(K) 同构，其中 $n^2=$ dim(A) (VIII, p. 252, 定理 1)。因此我们有 $[A][A^o] = [A\otimes_KA^o] = [K]$ (引理 1)，它证明 [A] 是可逆的，且有逆 $[A^o]$。

相反，令 A 为 K-代数 / 有限次数。如果 [A] 在 $\mathscr{M}_K$ 中可逆，则存在有限次数的 K-代数 B，使得 [A][B] = [K]；由公式 (2) 和引理 1，这意味着 K-代数 $A\otimes_KB$ 与矩阵代数 $\mathbf{M}_n(K)$ 和 $n\geqslant 1$ 同构。由 VIII、p. 251、代数中的注 1 则 A 是中心简单。

#### 定义 1 {#alg-viii-s15-def-1 .statement tag=00HY}

阿贝尔的群 Br(K) 称为域 K 的布劳尔群。

#### 引理 2 {#alg-viii-s15-lem-2 .statement tag=00HZ}

令I和J为有限集合，$k$为交换环，且A和B为$k$-代数。用 $\mathbf{M}_I(A)$ 表示型 $(I,I)$ 的方阵的 $k$ 代数，其中条目位于 A 中，定义同样表示 $k$ 代数 $\mathbf{M}_J(B)$ 和 $\mathbf{M}_{I\times J}(A\otimes_KB)$。存在唯一的$k$-代数同构

$$
\varphi :\mathbf{M}_I(A)\otimes_k\mathbf{M}_J(B)\longrightarrow \mathbf{M}_{I\times J}(A\otimes_kB)
$$

这样 $\varphi ((a_{ii'})\otimes (b_{jj'}))$ 是矩阵，其中指标 $((i, j),(i', j'))$ 等于 $a_{ii'}\otimes b_{jj'}$。

$k$线性双射$\varphi$与引理中所述的性质的存在源自张量积与直和（II, §3, No. 7，p. 255，命题7）的兼容性。 $\varphi$ 是代数同态是从乘积矩阵的定义得出的。

#### 命题 3 {#alg-viii-s15-prop-3 .statement tag=00I0}

设 A 和 B 为中心单K-代数 / 有限次数。以下属性是等效的：

(i) 布劳尔群 Br(K) 中有 [A] = [B]。

(ii) 存在整数$t\geqslant 1$使得K-代数$A\otimes_KB^o$与矩阵代数$\mathbf{M}_t(K)$同构。

(iii) 严格存在正整数$r$和$s$使得K-代数$A\otimes_K\mathbf{M}_r(K)$和$B\otimes_K\mathbf{M}_s(K)$同构。

(iv) 存在域 D 包含 K 和整数 $m\geqslant 1$ 和$n\geqslant 1$，使得A 与$\mathbf{M}_m(D)$ 同构，B 与$\mathbf{M}_n(D)$ 同构。

(v) K-代数 A 和 B 是森田等价的。

假设我们有 [A] = [B]。由于$[B^o]$是布劳尔群中[B]的逆，所以我们有$[K] = [B][B^o] = [A][B^o] = [A\otimes_KB^o]$。到引理 1，存在整数$t\geqslant 1$，使得代数$A\otimes_KB^o$和$\mathbf{M}_t(K)$同构。因此 (i) 意味着 (ii)。

假设 (ii) 成立。由于 $B^o\otimes_KB$ 与矩阵代数 $\mathbf{M}_s(K)$ 与 $s\geqslant 1$ (VIII, p. 252, 定理 1) 同构，代数 $A\otimes_KB^o\otimes_KB$ 同构于 $A\otimes_K\mathbf{M}_s$(K)，一方面，另一方面，到 $\mathbf{M}_t(K)\otimes_KB$。所以性质(ii)意味着性质(iii)。

假设 (iii) 成立。根据 Wedderburn 的定理 (VIII, p. 120, 定理 1)，K 上存在整数 $m\geqslant 1$ 和 $n\geqslant 1$ 和域 D 和 $D'$ 有限次数中心 K 使得 A 与 $\mathbf{M}_m(D)$ 同构，B 与 $\mathbf{M}_n(D')$ 同构。那么代数$A\otimes_K\mathbf{M}_r(K)$同构于$\mathbf{M}_{mr}$(D)，代数$B\otimes_K\mathbf{M}_{r'}(K)$同构于$\mathbf{M}_{nr'}(D')$(引理2)。由推论2 VIII、p. 121、K-代数 D 和$D'$ 同构。因此 (iii) 意味着 (iv)。

假设 (iv) 成立。 代数 A 和 D 是森田等效的，代数 B 和 D (VIII、p. 114、例 2) 也是如此。因此，A和B是森田等价的，因此(iv)蕴涵(v)。

最后，蕴涵(v)$\Rightarrow$(i)是集合Br(K)的定义。

当命题的等价性质成立时，我们说代数A和B相似。

#### 推论{#alg-viii-s15-n2-cor-1 .statement tag=00I1}

设A和B是K上有限次数的中心单代数。那么A和B是同构的当且仅当它们相似并且具有相同的次数。

这是从命题 3 的属性 (i) 和 (iv) 的等价以及 dim$_K(\mathbf{M}_n(D)) =$ dim$_K(D)\times n^2$ 的事实得出的。

#### 命题 4 {#alg-viii-s15-prop-4 .statement tag=00I2}

令$\mathscr{K}_K$为有限次数中央K-代数类集合即域。从 $\mathscr{K}_K$ 到 Br(K) 的映射 $D\mapsto [D]$ 是双射的。

这是从 VIII、p. 278 和 Wedderburn 的定理（VIII、p. 120、定理 1）中的引理 1 得出的。

### 3. Change of Base Field

令L为域K中的扩张。令A和B为有限次数中的K-代数；那么L-代数$A_{(L)}$和$B_{(L)}$都是有限次数。 L-代数$A_{(L)}\otimes_LB_{(L)}$和$(A\otimes_KB)_{(L)}$是同构的（III, §4, No. 1、p. 462、命题 3）。 L-代数$K_{(L)}$同构于L。因而，从 $\mathscr{C}_K$ 到 $\mathscr{C}_L$ 存在一个唯一的幺半群同态 $\rho_{L/K}$，使得

(3) $\rho_{L/K}$(cl(A)) = cl(A$_{(L)}$)

对于有限次数的每个K-代数 A。

如果 K-代数 A 和 B 是 Morita 等价的，那么L-代数 $A_{(L)}$ 和 $B_{(L)}$ (VIII, p. 111, 命题 13, e)) 也是森田等价的。如果 K-代数 A 是中心单形并且是有限次数，那么L-代数$A_{(L)}$ (VIII, p. 251, 注 2) 也是如此。所以我们可以从 Br(K) 推导出 $\rho_{L/K}$ 群同态 $r_{L/K}$ 到 Br(L) 使得

$$
r_{L/K}([A]) = [A_{(L)}] \tag{4}
$$

对于有限次数的每个中心单K-代数 A。

设 M 为域 L 中的扩张。因为标量的扩张是传递的（III, §1, No. 5，p. 434），所以我们有关系

$$
r_{M/K}=r_{M/L}\circ r_{L/K} \tag{5}
$$

设 A 为有限次数的中心单K-代数，并令 L 为 K 的扩张。 如果L-代数$A_{(L)}$同构于整数$n\geqslant 1$的矩阵代数$\mathbf{M}_n(L)$，我们说L对于A（或分裂的A）来说是分裂域。 上述记号中，同态$r_{L/K}:$Br(K)$\rightarrow$Br(L)的Br(K)属于至核，该对应至说、类。

如果 B 与 A 相似，则 A 的 L 是分裂域当且仅当 B 的分裂域时。

如果对于A来说L是分裂域，那么L的每一个扩张对于A来说都是分裂域。由VIII的定理1，p. 252，存在有限次数的K的伽罗瓦扩张即A的分裂域， K 的每个可分闭包对于 A 来说都是分裂域。

#### 命题 5 {#alg-viii-s15-prop-5 .statement tag=00I3}

设A为有限次数的中心单K-代数，并令L为有限次数的K的扩张。以下属性是等效的：

(i) 对于 A，扩张 L 是分裂域。

(ii) 存在类似于包含的有限次数的中心单K-代数，并且最大交换子代数同构于L。

让我们证明 (ii) 蕴涵 (i)；只要考虑L是A的最大交换子代数的情况就足够了。令$\psi : A\otimes_KA^o\rightarrow$End$_K(A)$为典范同构，将$a\otimes a'$发送到K-线性映射$x\mapsto axa'$（VIII，p. 252， 定理1)。我们将 A 视为右向量空间超过 L；然后$\psi$将$A\otimes_KL$发送到End$_K(A)$和诱导的子空间End$_L(A)$，通过L-代数$\psi ': A\otimes_KL\rightarrow$End$_L(A)$的限制、单同态。 集合$n= [L : K]$。到VIII、p. 262、命题 3，我们有$[A : L] =n$，因此有$[A\otimes_KL : L] = [A : K] =n^2$和[End$_L(A) : L] =n^2$。因而，$\psi '$是同构，这证明了(i)。

逆命题由下面的引理 3 得出。

#### 引理 3 {#alg-viii-s15-lem-3 .statement tag=00I4}

设A为有限次数的中心单K-代数，并令L为有限次数的K的扩张，即A的分裂域。令V为简单的$A_{(L)}$模，因此自然的态射$\varphi : A_{(L)}\rightarrow$结束$_L(V)$是同构。设C为环End$_A(V)$。那么C与$A^o$类似，$L\otimes 1\subset A_{(L)}$的像是C的最大交换子代数。

我们认同 A 与子环 $A_{(L)}$。我们将V视为K-向量空间。 环 C 是 End$_K(V)$ 中 $\varphi (A)$ 的交换子。 有限次数为中心单K-代数，从$A\otimes_KC$到End$_K(V)$的同态$a\otimes c\mapsto ac$为同构(VIII、p. 260、定理6、a))。因而，K-代数 A 和$C^o$ 相似（VIII、p. 279、命题 3）。

令$L_V$为L-向量空间V的同伦的环；它是 End$_L(V)$ 与 End$_K(V)$ 的交换子（VIII，p. 82，推论 1）。现在，K-代数End$_L(V)$是由$\varphi (A)$和$L_V$生成的；因而，在 End$_K$(V) 中，我们有

$L_V=$结束$_L(V)'=\varphi (A)'\cap L'_V= C\cap L'_V$,

其中，对于 End$_K$(V) 中的任意子集 B，End$_K(V)$ 中 B 的交换子用 $B'$ 表示。所以$L_V$是C（VIII，p. 261，引理3）的最大交换子代数，因此也是$C^o$。从L到$L_V$，映射$\lambda \mapsto \lambda_V$是K-代数同构。这就证明了引理。

#### 推论 1 {#alg-viii-s15-lem-3-cor-1 .statement tag=00I5}

设A为有限次数的中心单K-代数，并令L为有限次数的K的扩张。假设$[A : K] = [L : K]^2$。那么对于 A，L 是分裂域当且仅当包含子代数同构于 L。

假设从L到A存在态射$\varphi$，设M为最大半单交换子代数包含$\varphi (L)$。通过 VIII、p. 262 的命题 3，我们得到 $[A : K] = [M : K]^2$，因而 [M : K] = [L : K] 和 $M =\varphi (L)$。由命题 5，域 L 分裂的 A。反之，假设域 L 分裂的 A；那么它与类似于 A (命题 5) 的中心单K-代数 B 的最大交换子代数同构。我们有 $[B : K] = [L : K]^2$ (VIII, p. 262, 命题 3)，因而 [B : K] = [A : K]。因而，B 与 A 同构的（VIII，p. 280，推论）。推论 1 如下。

#### 推论 2 {#alg-viii-s15-lem-3-cor-2 .statement tag=00I6}

令 D 为中心 K 上的有限次数的域，并令 L 为有限次数的 K 的扩张，即 D 的分裂域。 D 除的约化次数 [L : K]。

将 D (VIII, p. 253) 减少的次数表示为 $r$；到定义，我们就有了$[D : K] =r^2$。到命题 5，存在与D相似的中心单K-代数 B，其中L是最大的交换子代数。由于 B 同构于矩阵代数 $\mathbf{M}_n(D)$ (VIII, p. 278, 引理 1)，因此我们有 $[B : K] =n^2r^2$，因此有 $[L : K] =nr$ (VIII, p. 262, 命题 3)。

### 4. 例 / 布劳尔群

在以下三种情况下，布劳尔群 Br(K) 会减少为单位元素：

a) K 是可分离闭的（VIII，p. 253，推论 1）。

$*$b) K 为有限域 (VIII, p. 357, 推论 2)。

c) K 有性质 $(C_1)$ (VIII, p. 357, 注 2)。

假设 K 为极大有序域 (VI, §2, No. 5, p. 25)。 K 的布劳尔群则为阶 2 的循环；它的元素是K的类和型$(-1,0,-1)$的四元数K-代数的类（III, §2, No. 5，p. 444和VIII，p. 367，定理1）。

假设 K 是局部紧致、非离散、可交换拓扑域。 如果 K 未连接，则对于离散评估来说，它是完整的域，且剩余类域有限（Comm. Alg., VI, §9, No. 3, p. 433, 定理 1), 从 Br(K) 到 $\mathbf{Q}/\mathbf{Z}$ (VIII, p. 332, 习题 17) 存在同构。 如果 K 是连通的，则它与 $\mathbf{R}$ 或 $\mathbf{C}$ 同构的。 域$\mathbf{R}$的布劳尔群是阶2的循环。 它的非平凡元素是汉密尔顿四元数的代数$\mathbf{H}$的类（Gen. 顶部., VIII, §1, No. 4, p. 104); $\mathbf{C}$的布劳尔群有阶 1。

### 习题{#alg-viii-s15-exercises}

参见[习题为 § 15](exercises/s15/)。
