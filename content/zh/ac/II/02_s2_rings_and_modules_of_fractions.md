---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 2
section_title: Rings and modules of fractions
lang: zh
source: ac-i-vii
book_pages: 55-79, 123-136
pdf_pages: 0075-0099, 0143-0156
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF RINGS OF FRACTIONS
      page: 55
      pdf_page: 75
    - "no": 2
      title: MODULES OF FRACTIONS
      page: 60
      pdf_page: 80
    - "no": 3
      title: CHANGE OF MULTIPLICATIVE SUBSET
      page: 64
      pdf_page: 84
    - "no": 4
      title: PROPERTIES OF MODULES OF FRACTIONS
      page: 67
      pdf_page: 87
    - "no": 5
      title: IDEALS IN A RING OF FRACTIONS
      page: 70
      pdf_page: 90
    - "no": 6
      title: NILRADICAL AND MINIMAL PRIME IDEALS
      page: 73
      pdf_page: 93
    - "no": 7
      title: FRACTIONS OF TENSOR PRODUCTS AND HOMOMORPHISM MODULES
      page: 75
      pdf_page: 95
    - "no": 8
      title: APPLICATION TO ALGEBRAS
      page: 77
      pdf_page: 97
    - "no": 9
      title: MODULES OF FRACTIONS OF GRADED MODULES
      page: 78
      pdf_page: 98
statements: 52
exercises: 27
content_sha256: b919f8fc018ab4ff7767c279d5ebb64291263f5a0c32af9cae27f96aaee7a63b
translated_from: content/en/ac/II/02_s2_rings_and_modules_of_fractions.md
translation_method: google
source_content_sha256: 463e49262f632d4a137e725a82bdc25960c4aa1e43d83744037d89388a37100c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 6c2ed14f1d9ab1d3820379cfd045cd50a4653116fbeded2d8df50f391da4736f
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 2. 环和模的分数

### 1. 定义环分数

#### 定义 1 {#ac-ii-s2-def-1 .statement tag=045K}

*设$A$为环。 A subset $S$ of $A$ is called multiplicative if every finite product of elements of $S$ belongs to $S$.*

This is the same as saying that $1 \in S$ and that the product of two elements of $S$ belong to $S$.

*例*
(1) 对于每个$a \in A$，$a^n$的集合，其中$n \in \mathbf{N}$，是$A$的乘法子集。
(2) 令$p$为$A$的理想。对于$A - p$是$A$的乘法子集，$p$是质数是充分必要的。
(3) $A$的元素中的集合不是零的除子，是$A$的乘法子集。

(4) 如果 S 和 T 是 A 的乘法子集，则乘积 st 的集合 ST，其中 s ∈ S 且 t ∈ T，是乘法子集。

(5) 令 G 为 A 的乘法子集的有向集合（相对于关系 ⊂ ）。则 T = ⋃_{S ∈ G} S 是 A 的乘法子集，因为 T 属于的任意两个元素到某个子集 S ∈ G，因此它们的乘积属于至 T。

(6) A 的乘法子集的每个交都是乘法子集。

对于环 A 的每个子集 S，对于例 A 本身，都存在包含 S 的乘法子集。所有这些子集中的交是包含 S 的最小的乘法子集；据说它是由 S 生成的。因此它是 S 的元素的所有有限乘积中的集合由……组成。

#### 命题 1 {#ac-ii-s2-prop-1 .statement tag=045L}

设A为A的环和S子集。存在A到A'的环A'和同态h，具有以下性质：
(1) h(S) 的元素在 A 中可逆；
(2) 对于 A 到环 B 的每个同态 u，使得 u(S) 的元素在 B 中可逆，则存在 A 到 B 的唯一同态 u'，使得 u = u' ∘ h。

在其他字中，（A'，h）是普遍映射问题的解（集合理论，章IV, § 3, no. 1），其中条件：结构的类 Σ被认为是环的环， 态射是环同态，a-映射是A到环的同态，使得在同态下的S的像由可逆元组成。回想一下（前述），如果 (A', h) 和 (A'_1, h_1) 都是问题的解，则存在唯一的同构 j : A' → A'_1 使得 h_1 = j ∘ h。

令$\overline{S}$为S生成的A的乘法子集。显然，上述普遍映射问题的每个解也是替换S乘$\overline{S}$得到的普遍映射问题的解，反之亦然。

考虑在集合 A × S 中，元素 (a, s), (a', s') 之间的以下关系 ：

(1) “存在 t ∈ $\overline{S}$ 使得 t (sa' − s'a​​) = 0”。

这个关系是等价关系：它显然是自反且对称的；它是传递性的，因为如果 t (sa' − s'a​​) = 0 且 t'(s'a'' − s''a') = 0，则 tt's'(sa' − s'a​​) = 0 且 tt's' ∈ $\overline{S}$。令A’为A×$\overline{S}$在此等价关系下的商集；对于每个有序对 (a, s) ∈ A × $\overline{S}$，我们用 A 中 (a, s) 的 a/s 典范像表示，并且对于所有 a ∈ A，集合 h(a) = a/1。我们将看到 A' 可以给定环结构，使得有序对 (A', h) 求解问题。

令 x = a/s 和 y = b/t 为 A' 的两个元素。 元素 (ta + sb)/st 和 $ab/st$ 仅取决于 $x$ 和 $y$；对于如果$x = a'/s'$，则存在假设$r \in \overline{S}$使得$r(s'a - sa') = 0$，从而

$$
r(s't(ta + sb) - st(ta' + s'b)) = 0
$$

和$r(s'tab - sta'b) = 0$。 容易验证合成$(x, y) \mapsto x + y = (ta + sb)/st$的律和$(x, y) \mapsto xy = ab/st$定义交换环结构在$\mathbf{A}'$上，其中$0/1$在加法下是单位元素，$1/1$是单位元。 Moreover, it is immediate that $h$ is a ring homomorphism and that, for all $s \in S$, $s/1$ is invertible in $\mathbf{A}'$, its inverse being $1/s$. 最后令$B$为环且$u : \mathbf{A} \to B$同态，使得元素$u(S)$在$B$中可逆；存在唯一映射 $u' : \mathbf{A}' \to B$ 使得

(2)
$$
u'(a/s) = u(a)(u(s))^{-1} \quad (a \in \mathbf{A}, s \in \overline{S}).
$$

如果$a/s = a'/s'$，则存在$t \in \overline{S}$使得$t(sa' - s'a) = 0$，从而$u(t)(u(s)u(a') - u(s')u(a)) = 0$，并且由于$u(t)$，$u(s)$和$u(s')$是可逆的，$u(a)(u(s))^{-1} = u(a')(u(s'))^{-1}$。容易验证$u'$相对于加法和乘法来说是同态；最后，显然$u' \circ h = u$和$u'$是唯一的同态满足这个关系，正如它所暗示的那样

$$
u'(a/s) = u'((a/1)(1/s)) = u'(1/s)u'(a/1) = u'(1/s)u(a)
$$

和 $1 = u'(1/1) = u'(s/1)u'(1/s) = u(s)u'(1/s)$、从而公式 (2)。

#### 定义 2 {#ac-ii-s2-def-2 .statement tag=045M}

令$\mathbf{A}$为环、$\mathbf{A}$的$S$子集以及$\overline{S}$由$S$生成的乘法子集。由$S$定义并用$\mathbf{A}[S^{-1}]$表示的$\mathbf{A}$的分数的环是等价关系(1)下的$\mathbf{A} \times \overline{S}$的商集，其中环结构定义为

$$
(a/s) + (b/t) = (ta + sb)/st, \qquad (a/s)(b/t) = (ab)/(st)
$$

对于$\mathbf{A}$中的$a, b$，$\overline{S}$中的$s, t$。 $\mathbf{A}$到$\mathbf{A}[S^{-1}]$的典范映射是同态$a \mapsto a/1$，这使得$\mathbf{A}[S^{-1}]$变成$A$代数。

在这个章中，我们通常用$i_A^S$来表示这个典范映射； 命题1的证明表明，有序对$(\mathbf{A}[S^{-1}], i_A^S)$满足该命题的叙述条件。

**注**

(1) 显然$\mathbf{A}[\overline{S}^{-1}] = \mathbf{A}[S^{-1}]$。

(2) $\mathbf{A}[S^{-1}]$ 中的两个元素始终可以写成形式 $a/s$ 和 $a'/s$（$\mathbf{A}$、$s \in \overline{S}$ 中的$a, a'$），并具有*相同*“分母”$s$，对于 if $b/t$和$b'/t'$是$\mathbf{A}[S^{-1}]$的两个元素，然后是$b/t = bt'/tt'$和$b'/t' = b't/tt'$。

(3) $i_A^S$的核是$a \in A$的集合，因此存在$s \in \overline{S}$满足$sa = 0$；为了使$i_A^S$是单射的，$S$包含在$A$中没有零的除子是必要且充分的。

(4) 如果$S$包含幂零元，则$0 \in \overline{S}$和环$A[S^{-1}]$减为0；这很容易从定义 2 得出。

(5) 对于$i_A^S$为双射，每个元素$s \in S$在$A$中可逆是充分必要的：条件显然是必要的，因为$s/1$在$A[S^{-1}]$中可逆；这是足够的，因为对于所有$t \in \overline{S}$，$t$在$A$中是可逆的，$a/t = at^{-1}/1$在$A[S^{-1}]$中是可逆的；因此 $i_A^S$ 是满射的，并且已经在注 3 中看到它是单射的。然后通过$i_A^S$来识别$A$和$A[S^{-1}]$。

例 (7)。如果$R$是$A$中元素的集合，且不是0的除子，则环$A[R^{-1}]$正是我们所说的$A$的分数的环（代数， 章I, §9, no. 4）；为了避免任何混淆，我们通常将其称为 $A$ 的分数的总和环。特别地，如果$A$是整环，则$A[R^{-1}]$是$A$的分数的域（前述）。

#### 命题 2 {#ac-ii-s2-prop-2 .statement tag=045N}

令$A, B$从$A$到$B$为$A$、$B$的$T$子集和$f$同态两个环、$S$子集这样那个$f(S) \subset T$。从$A[S^{-1}]$到$B[T^{-1}]$存在唯一同态$f'$，使得$f'(a/1) = f(a)/1$对于所有$a \in A$。

进一步假设$T$包含在$f(S)$生成的$B$的乘法子集中。那么，iff 是满射的（或单射的），$f'$ 也是。

第一个断言等于说，存在唯一同态 $f': A[S^{-1}] \to B[T^{-1}]$ 给出交换律图表：

$$
\begin{array}{ccc}
A & \xrightarrow{f} & B \\
i_A^S \downarrow & & \downarrow i_B^T \\
A[S^{-1}] & \xrightarrow{f'} & B[T^{-1}]
\end{array}
$$

现在关系$f(S) \subset T$意味着对于所有$s \in S$，$i_B^T(f(s))$在$B[T^{-1}]$中是可逆的，并且应用命题1到$i_B^T \circ f$就足够了。从 (2) 可以轻松得出，对于所有 $a \in A$ 和 $s \in \overline{S}$（由 $S$ 生成的 $A$ 的乘法子集），

$$
f'(a/s) = f(a)/f(s).
$$

假设$T$包含在$f(S)$生成的乘法子集中，恰好是$f(\overline{S})$。由(3)可知，iff 是满射的，$f'$ 也是满射的。

现在假设 $f$ 是单射的。令$a/s$为核中的元素'。由于$T$生成的乘法子集是$f(\overline{S})$，因此存在元素$s_1 \in \overline{S}$，使得$f(s_1)f(a) = 0$，从而$f(s_1a) = 0$，因而$s_1a = 0$，因为$f$是单射的；然后$a/s = 0$，证明$f'$是单射的。

注 (6)。如果$T$的元素在$B$中可逆，则$B[T^{-1}]$通过同构$i_B^T$和$f'$与$B$相同，则与$A[S^{-1}]$的唯一同态$u'$相同， $B$使得$u' \circ i_A^S = f$。

#### 推论 1 {#ac-ii-s2-prop-2-cor-1 .statement tag=045O}

*令$A$为环、$A$的$S$子集以及$A$至环$B$的$u$单同态，使得元素为$u(S)$ 在 $B$ 中可逆。 $A[S^{-1}]$ 到 $B$ 的唯一同态 $u'$ 使得 $u' \circ i_A^S = u$ 是单射的。*

这是命题 2 和注 6 中的直接的推论。

#### 推论 2 {#ac-ii-s2-prop-2-cor-2 .statement tag=045P}

*令$A$为环且$S$和$T$为$A$中的两个子集，使得$S \subset T$。从$A[S^{-1}]$到$A[T^{-1}]$存在唯一同态$i_A^{T,S}$使得$i_A^T = i_A^{T,S} \circ i_A^S$。*

对于所有$a \in A$、$i_A^{T,S}$，然后$A[S^{-1}]$中的映射元素$a/s$到$A[T^{-1}]$中的元素$a/s$。

注 (7)。 注，如果$i_A^T$是单射的，$i_A^{T,S}$也是单射的（推论1）。如果 $T$ 是 $A$ 的元素的集合 $R$，且除子不是 0，就会发生这种情况；那么可以将$A$生成的分数$A[R^{-1}]$的总环和$S$的元素的$A[R^{-1}]$的逆进行认同$A[S^{-1}]$和子环进行计算。

#### 推论 3 {#ac-ii-s2-prop-2-cor-3 .statement tag=045Q}

*令$A, B, C$为三个环、$S$（分别为$T, U$）、$A$（分别为$B, C$）、$f : A \to B$、$g : B \to C$两个同态和$h : A \to C$的乘法子集复合同态$g \circ f$；假设$f(S) \subset T$，$g(T) \subset U$。令 $f' : A[S^{-1}] \to B[T^{-1}]$、$g' : B[T^{-1}] \to C[U^{-1}]$、$h' : A[S^{-1}] \to C[U^{-1}]$ 同态相应的到 $f, g, h$；然后$h' = g' \circ f'$.*

这很容易从定义得出。

特别是，如果$S, T, U$是$A$的三个乘法子集，使得$S \subset T \subset U$，则$i_A^{U,S} = i_A^{U,T} \circ i_A^{T,S}$。

#### 推论 4 {#ac-ii-s2-prop-2-cor-4 .statement tag=045R}

*设$S$为环$A$中的子集，$A[S^{-1}]$包含$i_A^S(A)$中的$B$子环和$S'$集合$i_A^S(A)$。设$j$为$B$的典范嵌入入$A[S^{-1}]$； 唯一同态 $g$ 从 $B[{S'}^{-1}]$ 到 $A[S^{-1}]$，使得 $g \circ i_A^S = j$ 为同构。*

映射 $g$ 由推论 1 是单射的； 环 $g(B[{S'}^{-1}])$ 包含 $i_A^S(A)$ 以及 $S'$ 元素的逆；因此它等于 $A[S^{-1}]$。

若$A$为整环且$0 \notin S$，则记号$A[S^{-1}]$与代数、章IV, § 2, no. 1一致；另外，如果 $S$ 是乘法，则$A[S^{-1}]$ 重合在这种情况下，集合由代数、章 I, § 1, no. 1 中的$S^{-1}A$ 表示。

作为记号的扩张，对于环$A$的任何乘法子集$S$，我们从此用分数$A[S^{-1}]$的$S^{-1}A$环表示。如果$S$是$A$的素理想$p$的补集，我们写成$A$，而不是$S^{-1}A$。

如果$A$是整环和$0 \notin S$，则$S^{-1}A$总是被识别为$A$、包含、$A$、注7、分数、域、子环。

### 2.模分数

no. 1中定义的典范同态$i_A^S : A \to A[S^{-1}]$允许我们将每个$A[S^{-1}]$模块视为$A$模块。

#### 命题 3 {#ac-ii-s2-prop-3 .statement tag=045S}

令$A$为$A$的环、$S$子集、$M$为$A$模块、$M'$为$A$模块、$M \otimes_A A[S^{-1}]$和$f$规范$A$-$M$到$M'$的同态$x \mapsto x \otimes 1$。然后：
(1) 对于所有$s \in S$，$M'$的位似$z \mapsto sz$是双射的。
(2) 对于每个$A$模$N$，使得$s \in S$、$N$的位似$y \mapsto sy$都是双射的，并且$M$到$N$的每个同态$u$，存在$M'$到$N$的唯一同态$u'$使得$u = u' \circ f$。

在其他字中，$(M', f)$是普遍映射问题中的解（集合理论，章IV, § 3, no. 1），以及以下条件：结构中的类 $\Sigma$是$A$模，其中$S$的元素诱导的同位是双射，态射是$A$模同态，$a$映射也是$A$模同态。

对于每个$A$-模块$N$和所有$a \in A$，用$N$中的$h_a$位似$y \mapsto ay$表示；那么$a \mapsto h_a$就是从$A$到$\operatorname{End}_A(N)$的环同态。说$h_a$是双射意味着$h_a$是$\operatorname{End}_A(N)$的可逆元。假设对于所有$s \in S$，$h_s$在$\operatorname{End}_A(N)$中是可逆的； 元素$h_a$，其中$a \in A$，以及元素$h_s$的逆，其中$s \in S$，然后$\operatorname{End}_A(N)$中的生成交换律子环$B$和同态从$A$到$B$的$a \mapsto h_a$使得$S$的元素的像是可逆的。那么 (no. 1, 命题 1) 存在 $A[S^{-1}]$ 到 $B$ 的唯一同态 $h'$ 使得

$$
h'(a/s) = h_a(h_s)^{-1};
$$

我们知道 (代数, 章 II, , no. 14) N 上的同态定义是一个$A[S^{-1}]$-模块结构，使得 $(a/s).y = h_s^{-1}(a.y)$； A-模结构通过同态 $i_A^S$ 从此$A[S^{-1}]$ 模块结构衍生而来，正是最初给出的结构

相反，如果 N 是$A[S^{-1}]$模，并且通过$i_A^S$将其视为A-模，则$s \in S$的同位$y \mapsto sy$是双射的，因为$y \mapsto (1/s)y$是$y \mapsto sy$的逆映射；而通过上述过程从其A-模结构导出的N上的$A[S^{-1}]$模结构就是最初给出的$A[S^{-1}]$模结构。因此，$A[S^{-1}]$模和A-模之间存在规范的一对一对应，其中由S的元素引发的同位是双射的；此外，如果N，N'是两个A-模，其中性质每A-模同态$u : N \to N'$也是N和N'的$A[S^{-1}]$模结构的同态，对于盟友$\in N$和所有$s \in S$，我们可以写$u(y) = u(s.((1/s)y)) = s.u((1/s)y)$、从而$u((1/s)y) = (1/s)u(y)$； 逆命题是显而易见的。

This being so, the statement of Proposition 3 is just the characterization of the module obtained from M by extending the scalars to $A[S^{-1}]$, taking account of the above interpretation (Algebra, Chapter II, § 5, no. 1, Remark 1).

#### 定义 3 {#ac-ii-s2-def-3 .statement tag=045T}

令A为环，A的S子集，$\overline{S}$由S和M A-模生成的A的乘法子集。那么由S定义并用$M[S^{-1}]$或$\overline{S}^{-1}M$表示的M的分数的模就是$A[S^{-1}]$模$M \otimes_A A[S^{-1}]$。

在这个章中，我们通常用M的$i_M^S$典范映射$m \mapsto m \otimes 1$来表示

**注**
(1) 显然$M[\overline{S}^{-1}] = M[S^{-1}]$。
(2) 对于$m \in M$和$s \in \overline{S}$，我们也将$M[S^{-1}]$的元素$m \otimes (1/s)$写成$m/s$。 $M[S^{-1}]$的每个元素都是形式，因此元素是形式$\sum_i m_i \otimes (a_i/s)$，其中$m_i \in M, a_i \in A, s \in S$（no. 1，注2），并且

$$
m_i \in 3 (a_i/s) = (a_i m_i) \in 3 (1/s),
$$

因而$\sum_i m_i \otimes (a_i/s) = m \otimes (1/s)$，其中$m = \sum_i a_i m_i$。然后

(4)
$$
(m/s) + (m'/s') = (s'm + sm')/ss'
$$
(5)
$$
(a/s)(m/s') = (am)/(ss')
$$

其中 $m, m' \in M, a \in A$ 和 $s, s' \in S$。

(3) 如果S是A的素理想p的补，我们写M_p而不是S^{-1}M。

(4) 令M为A[S^{-1}]-模；如果 M 被视为规范地A-模，则 i_M^S 为双射，对于 M 的有序对由……组成和恒等映射 1，也很简单地由 M[S^{-1}] 求解普遍映射问题的解且i_M^S。那么M用M[S^{-1}]来标识。

#### 命题 4 {#ac-ii-s2-prop-4 .statement tag=045U}

*令 S 为 A 和 M A-模的乘法子集。对于 m|s = 0 (m \in M, s \in S)，存在 s' \in S 使得 s'm = 0 是充分必要的。*

如果 s' \in S 满足 s'm = 0，显然 m|s = (s'm)/(ss') = 0。反之，假设 m|s = 0。由于 1/s 在 S^{-1}A 中是可逆的，所以 m/1 = 0。对于 S^{-1}A 包含于 1 的每个子 A 模 P，我们用 \beta(P, m) 表示(m, 1) 的像在 M \times P 到 M \otimes_A P 的典范映射下；那么 \beta(S^{-1}A, m) = 0。我们知道（代数，章 II, § 6, no. 3，推论 4 到命题 7），存在 S^{-1}A 包含于 1 的*有限生成* 子模 P，并且使得 \beta(P, m) = 0. 对于所有 t \in S，我们用 a/t 的 A_t 集合表示，其中 a \in A；由于 P 是有限生成的，因此存在 t \in S 使得 P \子集 A_t (no. 1, 注 2), 从而 \beta(A_t, m) = 0。 映射 a \mapsto a/t 从 A 到 A_t 是满射的；设 B 为其核。它定义一个满射映射h：M \otimes_A A \到M \otimes_A A_t，其核是BM（M被识别为M \otimes A）；则 \beta(A_t, m) = h(tm) ，因而 tm 可以表示为形式 $\sum_{i=1}^r b_i m_i$，其中 b_i \in B，m_i \in M (1 \leq i \leq r)。由于对于 1 \leq i \leq r，b_i/t = 0，因而 S 中存在 t' \，使得对于 1 \leq i \leq r，t'b_i = 0，从而 t'tm = 0，从而证明命题 4。

#### 推论 1 {#ac-ii-s2-prop-4-cor-1 .statement tag=045V}

*对于 S^{-1}M 中的 m|s = m'|s'，存在 t \in S 使得 t(s'm - sm') = 0 是充分必要的。*

$$(m|s) - (m'|s') = (s'm - sm')/ss'.$$

#### 推论 2 {#ac-ii-s2-prop-4-cor-2 .statement tag=045W}

*设M为有限生成A-模。对于 S^{-1}M = 0，存在 s \in S 使得 sM = 0 是充分必要的。*

如果 M 上没有任何条件，显然关系 sM = 0 对于某些 s \in S 意味着 S^{-1}M = 0。相反，假设 S^{-1}M = 0 且令 (m_i)_{1 \leq i \leq n} 为 M 的生成元的系统； m_i/1 生成 S^{-1}A-模 S^{-1}M，因此说 S^{-1}M = 0 等于说，对于 1 \leq i \leq n，m_i/1 = 0；到命题 4，存在$s_i \in S$，使得$s_i m_i = 0$，并且对于所有$i$取$s = s_1 s_2 \cdots s_n$，$s m_i = 0$，因而$sM = 0$。

#### 推论 3 {#ac-ii-s2-prop-4-cor-3 .statement tag=045X}

*设M为有限生成A-模。对于理想的$a \& A$使得$aM = M$，存在$a \in a$使得$(1 + a)M = 0$是充分必要的。*

显然关系$(1 + a)M = 0$意味着$M = aM$。为了证明逆命题，我们使用以下引理：

#### 引理 1 {#ac-ii-s2-lem-1 .statement tag=045Y}

*对于 A 的每个理想 a，元素 $1 + a$ 的集合 S，其中 $a \in a$ 是 A 的子集和 $S^{-1}A$ 的元素的集合 $a'$ 形式 $a/s$，其中 $a \in a$ 和 $s \in S$，是包含在 $S^{-1}A$ 的雅各布森根式中的理想。*

第一个断言是显而易见的，而且$a'$是$S^{-1}A$的理想。另一方面，$(1/1) + (a/s) = (s + a)/s$和$s + a \in S$对于S的定义的所有$s \in S$和$a \in a$；因而，对于所有$a/s \in a'$，$(1/1) + (a/s)$在$S^{-1}A$中是可逆的，这完成了引理的证明（*代数*，章VIII, § 6, no. 3，定理1）。

既然如此，如果我们集合$N = S^{-1}M$，显然N是一个有限生成的$S^{-1}A$模；如果$aM = M$，则$a'N = N$，并且根据中山的引理得出$N = 0$（*代数*，章VIII, § 6, no. 3，推论到命题6）；然后从推论 2 得出推论。

#### 命题 5 {#ac-ii-s2-prop-5 .statement tag=045Z}

*设 A、B 为两个环，S 为 A 的乘法子集，T 为 B 的乘法子集，并且从 A 到 B 的 f 同态使得 $f(S) \subset T$。设 M 为从 M 到 N 的 A-模、N B-模和 u A-线性映射。则存在从 $S^{-1}M$ 到 $T^{-1}N$ 的唯一 $S^{-1}A$ 线性映射 $u'$，使得 $u'(m/1) = u(m)/1$ 对于所有 $m \in M$。*

从 M 到 $T^{-1}N$ 映射 $i_N^T \circ u$ 是 A 线性的。此外，如果$s \in S$，则$f(s) \in T$，因此由s在$T^{-1}N$上诱导的位似是双射的。 $u'$的存在性和唯一性则从命题3得出。然后，对于$m \in M$和$s \in S$，

$$
u'(m/s) = u(m)/f(s).
$$

同样的记号，令C为第三个环，U为C的乘法子集，从B到C的g同态，使得$g(T) \subset U$，P C-模，从N到P的v B-线性映射和$v'$$T^{-1}B$线性从 B 映射到与 v 相关的$U^{-1}P$。然后

$$
(v \circ u)' = v' \circ u'
$$

其中左侧是与 $v \circ u$ 相关联的 A-线性映射 $S^{-1}M \to U^{-1}P$。类似地，如果$u_1$是从M到N的第二个A-线性映射，那么

$$
(u + u_1)' = u' + u_;
$$

左侧是 A-线性映射 $S^{-1}M \to T^{-1}N$ 与 $u + u_1$ 相关联。

注 (5)。如果在命题 5中，我们取$B = A, T = S$和$f = 1_A$，很容易看出$u'$就是映射$u \otimes 1 : M \otimes S^{-1}A \to N \otimes S^{-1}A$。今后我们将用$S^{-1}u$来表示它；如果 S 是 A 的素理想 $p$ 的补集，我们写 $u_p$ 而不是 $S^{-1}u$。

#### 命题 6 {#ac-ii-s2-prop-6 .statement tag=0460}

令$f$为同态，从环A到环B，S为A的乘法子集。存在从$(f(S))^{-1}B$到$S^{-1}B$的唯一映射j（其中B通过以下方式被视为A-模） $f$），使得$j(b|f(s)) = b|s$适用于所有$b \in B, s \in S$。如果 $f' : S^{-1}A \to (f(S))^{-1}B$ 是与 $f$ (no. 1, 命题 2) 关联的环同态，则$j \circ f' = S^{-1}f$。 映射 j 是$(f(S))^{-1}B$上的$S^{-1}A$模块结构的同构，由$f'$定义到$S^{-1}B$上的模块结构，也是$(f(S))^{-1}B$上的B-模结构定义到$S^{-1}B$上的B-模结构 （所得的从定义$S^{-1}B = (S^{-1}A) \otimes_A B$）。

如果$b, b'$在B中，$s, s'$在S中，条件$b|s = b'|s'$和$b|f(s) = b'|f(s')$等价，由推论1到命题4，成立j的存在性，证明j是双射的； j 的唯一性是显而易见的。显然 j 是加法群同构。如果$a \in A, b \in B, s \in S, t \in S$，那么

$$
(a|s).(b|f(t)) = f'(a|s)(b|f(t)) = f(a)|f(s)(b|f(t)) = (f(a)b)|f(st),
$$

由此可知 j 是 $(S^{-1}A)$ 线性的。显然$j \circ f^1 = S^{-1}f$。最后，如果$b \in B, b' \in B, s \in S$，则$j(b.(b'|f(s))) = j(bb'|f(s)) = bb'|s = b.(b'|s)$，这就证明了最后一个断言。

命题 6 的映射 j 称为$(fS)^{-1}B$ 的典范同构到$S^{-1}B$。这两个集合一般是通过$f'$来识别的；然后$f' = S^{-1}f, i_B^S = i_B^{f(S)}$。

### 3. 乘法子集的变换

设 A 为环，S 为 A 和 M A-模的乘法子集。如果 T 是包含 S 的乘法子集，则从 no. 2 的命题 5 得出，存在唯一的 $S^{-1}A$ 线性映射 $i_M^{T,S} : S^{-1}M \to T^{-1}M$，使得 i_M^T = i_M^{T,S} \circ i_M^S； S^{-1}M 的映射 i_M^{T,S} 映射元素 m/s 到 T^{-1}M 的元素 m/s。很容易验证 i_M^{T,S} = i_A^{T,S} \otimes 1_M。如果 U 是 A 的第三次乘法子集，且 T \子集 U，则 i_M^{U,S} = i_M^{U,T} \circ i_M^{T,S}；此外，如果 u: M \to N 是 A-模同态，图表

$$
\begin{array}{ccc}
S^{-1}M & \xrightarrow{s^{-1}u} & S^{-1}N \\
i_M^{T,S} \downarrow & & \downarrow i_N^{T,S} \\
T^{-1}M & \xrightarrow{T^{-1}u} & T^{-1}N
\end{array}
$$

是可交换的。

#### 命题 7 {#ac-ii-s2-prop-7 .statement tag=0461}

设A为环，S、T为A的两个乘法子集。集合T' = i(T_A^S)。

(i) 存在从环 (ST)^{-1}A 到环 T'^{-1}(S^{-1}A) 的唯一同构 j，使得图表

$$
\begin{array}{ccc}
A & \xrightarrow{i_A^S} & S^{-1}A \\
i_M^{ST} \downarrow & & \downarrow i_{S^{-1}A}^{T'-1A} \\
(ST)^{-1}A & \xrightarrow{j} & {T'}^{-1}(S^{-1}A)
\end{array}
$$

是可交换的。

(ii) 设 M 为 A-模。存在从 (ST)^{-1}A-模 (ST)^{-1}M 到 T'^{-1}(S^{-1}A)-模块 T'^{-1}(S^{-1}M) 的 (ST)^{-1}A 同构 k，使得图表

$$
\begin{array}{ccc}
M & \xrightarrow{i_M^S} & S^{-1}M \\
i_A^{ST} \downarrow & & \downarrow i_{S^{-1}M}^{T'-1M} \\
(ST)^{-1}M & \xrightarrow{k} & {T'}^{-1}(S^{-1}M)
\end{array}
$$

是可交换的。

(i) 我们使用(ST)^{-1}A的定义作为普遍映射问题的解。令 B 为环，从 A 到 B 的 f 同态，使得 f(ST) 由可逆元组成。由于 f(S) 因此由可逆元组成，因此存在唯一同态 f': S^{-1}A \to B 使得 f = f' \circ i_A^S (no. 1, 命题 1)。对于 T 中的所有 t \in，f'(i_A^S(t)) = f(t) 在 B 中可通过hypo-\&\& 可逆。因而 f'(T') 由可逆元组成；则存在由 no. 1、命题 1、唯一同态 f'' 从 T'^{-1}(S^{-1}A) 到 B 使得 f'' = f'' \circ i_{S^{-1}A}^{T'}, 从而 f = f'' \circ u, 设定 u = i_{S^{-1}A}^{T'} \circ i_S^A。

此外，当且仅当$f''_1 : {T'}^{-1}(S^{-1}A) \to B$是第二个同态，使得$f''_1 \circ u = f$，然后$(f''_1 \circ i^{T'}_{S^{-1}A}) \circ i^S_A = (f'' \circ i^{T'}_{S^{-1}A}) \circ i^S_A$，从而$f''_1 \circ i^{T'}_{S^{-1}A} = f'' \circ i^{T'}_{S^{-1}A}$，因而$f''_1 = f''$。

由于${T'}^{-1}(S^{-1}A)$中ST的元素的$u$下的像是可逆的，有序对$({T'}^{-1}(S^{-1}A), u)$是no. 1中考虑的普遍映射问题（相对于A和ST）的解。这表明$j$的存在和唯一性。

(ii) 证明与 (i) 完全类似，在这种情况下使用no. 2，命题 3，留给读者。

#### 命题 8 {#ac-ii-s2-prop-8 .statement tag=0462}

设 A 为环，S、T 为 A 的两个乘法子集，使得 $S \subset T$。以下属性是等效的：

(a) *同态* $i^{T,S}_A : S^{-1}A \to T^{-1}A$ *是双射*。
(b) *对于每个 A-模 M，同态* $i^{T,S}_A : S^{-1}M \to T^{-1}M$ *是双射*。
(c) *对于所有*$t \in T$，*存在*$a \in A$*使得*$at \in S$（在其他字中，T的每个元素*除*S的元素）。
(d) *每个满足 T 的素理想都满足 S*。

上面已经看到$i^{T,S}_A = 1_M \otimes i^{T,S}_A$，它立即证明了（a）和（b）的等价。 集合$T' = i^S_A(T)$；那么 (命题 7) $T^{-1}A$ 与 ${T'}^{-1}(S^{-1}A)$ 相同，并且 (a) 等价于说，$T'$ 的元素在 $S^{-1}A$ 中*可逆* (no. 1, *注 5*)。现在，说$(t/1)(a/s) = 1/1$（$t \in T$，$a \in A, s \in S$）意味着存在$s' \in S$使得$tas' = ss'$，这表示（a）和（c）的等价。我们证明（d）蕴涵（c）。令$t$为T的元素，并假设$t/1$在$S^{-1}A$中不可逆；则存在 $S^{-1}A$ 包含 $t/1$ (*代数*, 章 I, § 8, no. 7, 定理 2) 的极大理想 $m'$，并且 $p = (i^S_A)^{-1}(m')$ 是包含的素理想$t$且不满足S（因为S的元素的$i^S_A$下的像是可逆的）。反之，如果存在满足T但不满足S的素理想$p$，则$p \cap T$的元素不能除元素；这证明了(c)蕴涵(d)并完成了证明。

It follows from Proposition 8 that, amongst the multiplicative subsets T of A containing S and satisfying the equivalent conditions of Proposition 8, there exists a *greatest*, consisting of *all* the elements of A which divide an element of S (cf. 习题1）。

#### 命题 9 {#ac-ii-s2-prop-9 .statement tag=0463}

令 I 为环 A 和 $S = \bigcup_{\alpha \in I} S_\alpha$ 的乘法子集的右向预序集合、$(S_\alpha)_{\alpha \in I}$ 递增族。我们将$\alpha \leq \beta$、$\rho_\alpha = i^{S_\alpha, S_\alpha}$写为$\rho_{\beta \alpha} = i^{S_\beta, S_\alpha}_{A^{S_\beta, S_\alpha}}$。那么$(S_\alpha^{-1}A, \rho_{\beta \alpha})$是Zings的直接系统，并且，如果对于所有$\alpha \in I$，$\rho'_\alpha$是$S_\alpha^{-1}A$到$\lim \rightarrow S_\alpha^{-1}A$的典范映射，则存在从$\lim \rightarrow S_\alpha^{-1}A$到$S^{-1}A$唯一的同构$j$这样对于所有 $\alpha \in I$ 都有$j \circ \rho'_\alpha = \rho_\alpha$。

对于$\alpha \leq \beta \leq \gamma$，$\rho_{\gamma \alpha} = \rho_{\gamma \beta} \circ \rho_{\beta \alpha}$（no. 1，推论3到命题2），因而$(S_\alpha^{-1}A, \rho_{\beta \alpha})$是直接系统。我们写$A' = \lim \rightarrow S_\alpha^{-1}A$；作为$\rho_\alpha = \rho_\beta \circ \rho_{\beta \alpha}$对于$\alpha \leq \beta$（no. 1，推论3到命题2），$(\rho_\alpha)$是同态的直接系统，$j = \lim \rightarrow \rho_\alpha$是从$A'$到$S^{-1}A$的唯一同态，使得$j \circ \rho'_\alpha = \rho_\alpha$ 对于所有$a \in I$。 同态 $\rho'_\alpha \circ i^{S}_{A^\alpha} : A \to A'$ 都相等，$\rho_{\beta \alpha} \circ i^{S}_{A^\alpha} = i^{S}_{A^\beta}$ $a \leq \beta$；让$u$成为他们的公共的值。显然，$u(S)$的元素在$A'$中是可逆的，这表明存在同态$h : S^{-1}A \to A'$使得$h \circ i^{S}_{A} = u$（no. 1，命题1）。然后

$$
j \circ h \circ i^{A}_{S} = j \circ u = j \circ \rho'_\alpha \circ i^{A^\alpha}_{S^\alpha} = \rho_\alpha \circ i^{S}_{A^\alpha} = i^{S}_{A}
$$

对于所有$\alpha \in I$，因而$j \circ h$是$S^{-1}A$的恒等式自同构。另一方面，对于所有$\alpha \in I$，

$$
h \circ j \circ \rho'_\alpha \circ i^{S}_{A^\alpha} = h \circ \rho_\alpha \circ i^{S}_{A^\alpha} = h \circ i^{S}_{A} = u = \rho'_\alpha \circ i^{S}_{A^\alpha},
$$

从而 $h \circ j \circ \rho'_\alpha = \rho'_\alpha$ 全部$\alpha \in I$；由此可见，$h \circ j$是$A'$的恒等式自同构，因而$j$是同构。

#### 推论{#ac-ii-s2-n3-cor-1 .statement tag=0464}

*在命题 9的假设下，令M为A-模。我们将所有$\alpha \in I$的$\alpha \leq \beta, f_\alpha = i^{S, S_\alpha}_{M}$写为$f_{\beta \alpha} = i^{S_\beta, S_\alpha}_{M}$，并让$f'_\alpha$从$S_\alpha^{-1}M$到$\lim \rightarrow S_\alpha^{-1}M$为典范映射；则存在$S^{-1}M$到$\lim \rightarrow S_\alpha^{-1}M$的$S^{-1}A$同构$g$，使得$g \circ f_\alpha = f'_\alpha$对于所有$a \in I$。*

推论立即从定义 $S_\alpha^{-1}M = M \otimes_A S_\alpha^{-1}A$ 和 $S^{-1}M = M \otimes_A S^{-1}A$ 得出，并且事实上，乘坐直极限与张量积通勤 (*代数*, 章 11, § 6, no. 3, 命题 7)。

### 4. 模分数的性质

*在本编号中，A 表示环，S 表示 A 的乘法子集。*

设$(M_\alpha, \phi_{\beta \alpha})$为A-模中的直接系统；那么 $(S^{-1}M_\alpha, S^{-1}\phi_{\beta \alpha})$ 是 $S^{-1}A$ 模块中的直接系统，而使用直极限与张量积 (*代数*, 章 II, § 6, no. 3, 命题 7) 通勤的事实允许我们定义典范同构

$$
\lim \rightarrow (S^{-1}M_\alpha) \to S^{-1} \lim \rightarrow M_\alpha.
$$

同样，使用直和与张量积通勤（代数、章 II、、no. 7、命题 7）这一事实使我们能够为每个家庭 $(M_i)_{i \in I}$ 的 $A$ 模块提供定义典范同构

$$
\bigoplus_{i \in I} S^{-1} M_i \to S^{-1} \bigoplus_{i \in I} M_i.
$$

最后我们注，如果$A$模块$M$是子模的$(N_i)_{i \in I}$系列的和，则$S^{-1}M$是由$i_M^S(N_i)$生成的子$S^{-1}A$模块系列的和。那么，如果$M$是有限生成的$A$模块（分别是有限呈现的$A$模块），则$S^{-1}M = S^{-1}A \otimes_A M$是有限生成的$S^{-1}A$模块（分别是有限呈现的$S^{-1}A$模块）。

#### 定理 1 {#ac-ii-s2-thm-1 .statement tag=0465}

*环$S^{-1}A$是一个扁平的$A$模块*（章I, § 2, no. 1，定义2）。

如果$u : M' \to M$是$A$模的单同态，则需要证明$S^{-1}u : S^{-1}M' \to S^{-1}M$是单射的。现在，如果$m'/s$ ($m' \in M'$, $s \in S$) 使得$u(m')/s = 0$，这意味着存在$s' \in S$使得$s'u(m') = 0$ (no. 2, 命题 4) 或$u(s'm') = 0$；由于 $u$ 是单射，因此有 $s'm' = 0$、从而 $m'/s = 0$。

事实上，$S^{-1}A$是一个扁平的$A$模块，这使得我们可以将章I, § 2的结果应用于它。特别是：
(1) 如果 $M$ 是 $A$ 模块，且 $N$ 子模为 $M$，则 $S^{-1}N$ 被规范地标识为由 $i_M^S(N)$ (章 I.) 生成的 $S^{-1}M$ *子模*。 § 2, no. 3,*注2*);通过此标识，$S^{-1}(M/N)$ 与 $(S^{-1}M)/(S^{-1}N)$ 进行标识，并且如果 $P$ 是 $M$ 的第二个子模，则

$$
S^{-1}(N + P) = S^{-1}N + S^{-1}P, \quad S^{-1}(N \cap P) = S^{-1}N \cap S^{-1}P
$$

（章I, § 2, no. 6，命题2）。
(2) 如果 $M$ 是一个*有限生成* $A$-模块，那么

$$
S^{-1} \operatorname{Ann}(M) = \operatorname{Ann}(S^{-1}M)
$$

（章I, § 2, no. 10，推论2至命题12）。

#### 命题 10 {#ac-ii-s2-prop-10 .statement tag=0466}

*令$M$为$A$模块。对于$S^{-1}A$模块$S^{-1}M$的每个子模$N'$，令$\phi(N')$为$i_M^S$下$N'$的逆像。然后：*
（一）$S\phi(N') = N'$。

(ii) 对于$M$中的每个子模$N$，$M$中的子模$\phi(S^{-1}N)$由那些存在$s \in S$使得$sm \in N$组成的$m \in M$组成。

(iii) $\phi$ 是 $S^{-1}M$ 子模块$S^{-1}A$ 的集合的同构（对于通过包含定义的顺序）到$M$ 子模 $Q$ 的集合，其中满足以下条件：

(MS) 如果$sm \in Q$，其中$s \in S$，$m \in M$，则$m \in Q$。

显然$S^{-1}\phi(N') \subset N'$；相反，如果$n' = m/s \in N'$，则$m/1 \in N'$，因而$m \in \phi(N')$，进而$n' \in S^{-1}(\phi(N'))$； 从而（一）。对于元素$m \in M$使得$m \in \phi(S^{-1}N)$，$m/1 \in S^{-1}N$是充分必要的，即存在$s \in S$和$n \in N$使得$m/1 = n/s$；这意味着存在$s' \in S$使得$s'sm = sn \in N$，从而 (ii)。最后，关系$sm \in \phi(N')$等价于定义到$sm/1 \in N'$，并且由于$s/1$在$S^{-1}A$中可逆，这意味着$m/1 \in N'$或$m \in \phi(N')$，因而$\phi(N')$满足条件 （女士）；另一方面，从(ii)可知，如果$N$满足(MS)，则$\phi(S^{-1}N) = N$，从而完成(iii)的证明。

子模 $\phi(S^{-1}N)$ 被称为 $M$ 中 $N$ 相对于 $S$ 的饱和度，子模满足条件 (MS)（因此等于它们的饱和度）被称为相对于 $S$ 饱和。 子模 $\phi(S^{-1}N)$ 是复合同态的核

$$
M \xrightarrow{h} M/N \xrightarrow{i_{M/N}^{S}} S^{-1}M/S^{-1}N
$$

其中 $h$ 是典范同态，如下从交换律到图表

$$
\begin{array}{ccc}
M & \xrightarrow{h} & M/N \\
i_M^S \downarrow & & i_{M/N}^S \downarrow \\
S^{-1}M & \xrightarrow{s^{-1}h} & S^{-1}M/S^{-1}N
\end{array}
$$

如果$S$是素理想$p$在$A$中的补集，则$\phi(S^{-1}N)$也称为$M$中$N$相对于$p$的饱和。

#### 推论 1 {#ac-ii-s2-prop-10-cor-1 .statement tag=0467}

令$N_1, N_2$为$A$模块$M$的两个子模。对于$S^{-1}N_1 \subset S^{-1}N_2$，$N_1$相对于$S$的饱和度包含在$N_2$的饱和度中是必要且充分的。

#### 推论 2 {#ac-ii-s2-prop-10-cor-2 .statement tag=0468}

*如果 M 为诺特*（分别为阿廷的）*A*-模，*S^{-1}M* 为诺特（分别为阿廷的）*S^{-1}A*-模。 *特别是，如果环 A 是诺特*（分别是阿廷的），*环 S^{-1}A* 也是如此。

### 5. 环 OF 分数的理想

#### 命题 11 {#ac-ii-s2-prop-11 .statement tag=0469}

*设 A 为环，S 为 A 的乘法子集。对于 S^{-1}A 的每个理想 b'，令 b = (i_A^S)^{-1}(b') 使得 b' = S^{-1}b。*

(i) *令 f 为典范同态 A \to A/b。从 S^{-1}A 到 (f(S))^{-1}(A/b) 的同态与 f (no. 1, 命题 2) 规范相关，它的核是 b'，其中定义，通过取商，典范同构为(S^{-1}A)/b' 到 (f(S))^{-1}(A/b)。此外，从 A/b 到 (f(S))^{-1}(A/b) 的典范同态是单射的。*

(ii) *映射 b' \mapsto b = (i_M^S)^{-1}(b')，限制于 S^{-1}A 的最大（或质数）理想的集合，是集合到 A 理想的集合的同构（关于包含），其中不满足 S 的那些中的最大值（分别是 A 不满足 S 的素理想的集合）。*

(iii) *如果 q' 是 S^{-1}A 的素理想且 q = (i_A^S)^{-1}(q')，则存在分数 A 的环的同构到环 (S^{-1}A)_{q'}，其中映射 a/b 为(a/1)/(b/1)，其中 a \in A，b \in A - q.*

(i) *(f(S))^{-1}(A/b) 可以通过这两个模 (no. 2, 命题 6) 之间的典范同构与 S^{-1}(A/b) 识别。 正合序列 0 \到 b \到 A \到 A/b \到 0 然后诱导正合序列*

$$
0 \to S^{-1}b \to S^{-1}A \to S^{-1}(A/b) \to 0
$$

(no. 4, 定理 1) 其存在证明了 (i) 的第一个断言，同时考虑到 b' = S^{-1}b。由于 b 对于 S 是饱和的，条件 a \in A, s \in S，因为 \in b 意味着 a \in b； A/b 上的比率 s 位似是单射的，这证明了 (i) 的第二个断言。

(ii) 我们首先注关系 b' = S^{-1}A 等价于关系 b \cap S \neq \varnothing，后者表达了 S^{-1}A 的 b' 包含可逆元的事实。从 no. 4, 命题 10 (iii) 可以看出，b' \mapsto b = (i_A^S)^{-1}(b') 是与 S^{-1}A 不同的 S^{-1}A 的理想的集合到集合 \mathscr{F} 的同构（关于包含） A 的理想不满足 S 和命题 10 的满足条件 (MS)。如果 b' 最大（或素数），则显然 b' 在 \mathscr{F}（或素数）中最大，反之亦然（通过 (i)）。另一方面，如果 r 是来自 S 的不相交的的理想，则其相对于 S 的饱和度 r_1 是来自 S 的包含 t 和不相交的的理想：对于某些 $s \in S$，没有元素 $a \in S$ 可以满足 $sa \in t$，因为它会遵循$sa \in t \cap S$。我们结论认为，如果$r$在$A$满足$S$的理想中最大，那么它在$\mathscr{F}$中最大。同样，如果$r$是不满足$S$的素理想，则它满足no. 4的条件（MS），命题10乘以定义的素理想，因此满足属于到$\mathscr{F}$。这就完成了 (ii) 的证明。

(iii) 假设 $q'$ 是素数，并且 $q$ 也是素数。 集合$T = A - q$是$A$的乘法子集，其中包含$S$、从而$ST = T$。我们写$T' = i_A^S(T)$；从 no. 3, 命题 7 (i) 可以得出，$T^{-1}A = A$ 存在唯一的同构 $j$，到 ${T'}^{-1}(S^{-1}A)$ 使得

$$
j(a/b) = (a/1)/(b/1),
$$

其中$a \in A$和$b \in T$。另一方面$T'$显然不满足$q'$；反之，设 $a/s \in S^{-1}A$；由于$1/s$在$S^{-1}A$中可逆，条件$a/s \notin q'$等价于$i_A^S(a) = a/1 \notin q'$，因此也等价于$a \notin q$；由此得出$S^{-1}A - q' = S^{-1}T'$，因此，通过no. 3的命题 8，得到${T'}^{-1}(S^{-1}A) = (S^{-1}A)_{q'}$。

(iii) 中定义的同构被称为规范的。如果$A$是整环，$A$的典范同构，以及$A$的分数$K$域子环和$(S^{-1}A)_{q'}$具有相同的像。

#### 注 {#ac-ii-s2-n5-rem-1 .statement tag=046A}

对于$A$到满足$S^{-1}a = S^{-1}A$的理想$a$（或者，no. 4、定理I、$S^{-1}(A/a) = 0$相当于同样的事情），$a \cap S \neq \varnothing$是必要且充分的，紧随定义。

#### 推论 1 {#ac-ii-s2-prop-11-cor-1 .statement tag=046B}

令$A$为环，且$S$为$A$的乘法子集。 $A$ 的每个理想 $p$ 在不满足 $S$ 的那些中最大的是素数。

通过命题 11，$p$上的假设意味着$p = (i_A^S)^{-1}(m')$，其中$m'$是$S^{-1}A$的极大理想；因为 $m'$ 是质数，$p$ 也是质数。

#### 推论 2 {#ac-ii-s2-prop-11-cor-2 .statement tag=046C}

令$A$为环，且$S$为$A$的乘法子集。对于$A$的每一个不满足$S$的理想$a$，都存在一个不满足$S$的素理想包含$a$。

$S^{-1}a \neq S^{-1}A$ (注)，因此存在$S^{-1}A$ 包含 $S^{-1}a$ (代数, 章 I, § 8, no. 7, 定理 2) 的最大理想，推论来自命题 11 (ii)。

#### 推论 3 {#ac-ii-s2-prop-11-cor-3 .statement tag=046D}

令$A, B$是从$A$到$B$的两个环、$\rho$同态以及$p$$A$的素理想。为了存在$B$的素理想$p'$使得$\overline{\rho}^{-1}(p') = p$，$\overline{\rho}^{-1}(B\rho(p)) = p$是充分必要的。

如果存在$B$的理想$p'$使得$\bar{\rho}^{-1}(p') = p$，则$\rho(p) \subset p'$、从而、$B_{\rho}(p) \subset p'$和$\bar{\rho}^{-1}(B_{\rho}(p)) \subset \bar{\rho}^{-1}(p') \subset p$；因为逆命题包含很明显，所以$\bar{\sigma}^{-1}(B_{\rho}(p)) = p$。相反，假设$\bar{\rho}^{-1}(B_{\rho}(p)) = p$并考虑$B$的乘法子集$S = \rho(A - p)$； 假设表明
$$
S \cap B_{\rho}(p) = \varnothing;
$$
由推论2，存在$B$包含$B_{\rho}(p)$的素理想$p'$且不满足$S$；那么 $\bar{\rho}^{-1}(p')$ 包含 $p$ 和不能包含 $A - p$ 中的任意元素，因此等于 $p$。

#### 推论 4 {#ac-ii-s2-prop-11-cor-4 .statement tag=046E}

*令$A, B$是从$A$到$B$的两个环和$\rho$同态。
(i) 假设存在一个$B$-模$E$，使得$\rho_*(E)$是一个忠实平坦的$A$-模。那么，对于$A$的每个素理想$p$，都存在一个$B$的素理想$p'$，使得$\bar{\rho}^{-1}(p') = p$。
(ii) 相反，假设$B$是一个扁平的$A$模。那么，如果对于$A$的每个素理想$p$，都存在一个$B$的理想$p'$，使得$\bar{\rho}^{-1}(p') = p$、$B$是忠实平坦的$A$模。*

(i) 假设意味着，对于 $A$、$\bar{\rho}^{-1}(B_{\rho}(a)) = a$ (章 I, § 3, no. 5、命题 8 (ii)) 的每个理想$a$，应用推论 3 就足够了。
(ii) 足以证明，对于$A$的每个最大理想$m$，都存在$B$的最大理想$m'$，使得$\bar{\rho}^{-1}(m') = m$ (章 I, § 2, no. 5, 命题 9 (e))。现在存在假设的理想$q$ $B$，使得 $\bar{\rho}^{-1}(q) = m$；作为$q \neq B$，存在最大理想$m'$为$B$包含$q$，因此存在$\bar{\rho}^{-1}(m') \supseteq m$；但是，如 $\bar{\rho}^{-1}(m')$ 不能包含 1、$\bar{\rho}^{-1}(m') = m$。

#### 推论 5 {#ac-ii-s2-prop-11-cor-5 .statement tag=046F}

*令$A$为环，$S$为$A$和$B$环的乘法子集，从而得到$i_A^S(A) \subset B \subset S^{-1}A$。令$q$为$B$的素理想，使得$A$的素理想$p = (i_A^S)^{-1}(q)$不满足$S$，并令$p'$为$S^{-1}A$的素理想$S^{-1}p$。然后$p' \cap B = q$.*

设 $S' = i_A^S(S)$； 典范同构已被定义为从${S'}^{-1}B$到$S^{-1}A$（no. 1，推论4到命题2）；我们通过这个同构认同这两个环。由于$q \cap S' = \varnothing$，$q' = {S'}^{-1}q$是$S^{-1}A = {S'}^{-1}B$的唯一素理想，使得$q' \cap B = (i_A^S)^{-1}(q') = q$ (命题 11 (ii)), 从而 $(i_A^S)^{-1}(q') = p$；因而 $q' = p'$ (命题 11 (ii))。

推论5的记号中，有$A$的典范同构，以及$(S^{-1}A)_q$上的$B_q$。 (命题 11 (iii))，因此是 *典范同构* $A, \to B_q$。

### 6. 极端的和最小的素理想

在（交换式）中，幂零元的环$A$集合是一个*理想*，因为如果$x, y$是$A$的元素使得$x^m = y^n = 0$，那么$(x + y)^{m+n} = 0$通过二项式定理。

#### 定义 4 {#ac-ii-s2-def-4 .statement tag=046G}

*（交换律）环 $A$ 的幂零元理想称为$A$的零根。如果$a$是$A$的理想，逆像，在典范映射$A \to A/a$下，$A/a$的零根称为$a$的根。*

我们经常用$r(a)$表示$A$的理想$a$的根式。

说元素 $x \in A$ 属于到 $a$ 的根部意味着存在整数 $n > 0$ 使得$x^n \in a$。如果f是从$A$到环$B$的同态，$b$是$B$的理想，$^{-1} (b)$的根式是$b$根式的*逆像* underf，也就是说$x^n \in f^{-1} (b)$ 意味着$(f(x))^n \in b$。

环 $A$ 的 nilradical 包含在其 Jacobson 部首中 (*代数*, 章 VIII, § 6, no. 3, 推论 3 至定理 1)，但可能与其不同；如果 $A$ 是 *阿廷的* (*代数*, 章 VIII, § 6, no. 4, 定理 3)，则它始终等于它。

我们说，环$A$的素理想$p$是*最小素理想*，如果它在按包含排序的$A$素理想中的集合中最小。

#### 命题 12 {#ac-ii-s2-prop-12 .statement tag=046H}

*令 $p$ 为环 $A$ 的最小素理想。对于所有 $x \in p$，存在 $s \in A - p$ 和整数 $k > 0$，使得 $sx^k = 0$。*

形式$sx^k$的元素的集合$S$（$k$整数$> 0$，$s \in A - p$）是$A$的乘法子集。如果$0 \notin S$，则存在不满足$S$的素理想$p'$（no. 5，推论2至命题11）。然后从$x \notin p'$开始有$p' = p$和$p' \# p$，与假设相反，$p$是最小的。

#### 命题 13 {#ac-ii-s2-prop-13 .statement tag=046I}

*环$A$的零根是$A$所有素理想中的交，也是$A$最小素理想中的交。*

显然，如果 $x \in A$ 幂零的，则它包含在 $A$ (§ 1, no. 1，定义 1) 的每个素理想中。相反，令$x$为$A$的非幂零元素； $x^k$ ($k$ 整数 $\geqslant 0$) 的集合 $S$ 是$A$ 的乘法子集而不是包含 0，因此存在一个素理想$p$ $A$不满足$S$（no. 5，推论2到命题11）和*更不必说*$x \notin p$；这建立了第一个断言。证明第二点，只要证明

#### 引理 2 {#ac-ii-s2-lem-2 .statement tag=046J}

*环$A$包含的每个素理想$A$的最小素理想。*

根据 Zorn 的引理，足以证明素理想的集合 P（按关系 $\supseteq$ 排序）是*归纳*的。现在，如果$G$是P的非空全有序子集，则理想$p \in G$的交$p_0$也是素理想：因为如果$x \notin p_0$和$y \notin p_0$，则存在理想$p \in G$使得$x \notin p$和$y \notin p$、从而 $xy \notin p$ 和 *更不必说* $xy \notin p_0$。

#### 注 {#ac-ii-s2-n6-rem-1 .statement tag=046K}

在§ 4, no. 3，推论3到命题14中，我们将证明在*诺特*环集合的最小素理想中是*有限的；此外，我们稍后会看到诺特环中的每个递减序列素理想都是*静止的*。

#### 推论 1 {#ac-ii-s2-lem-2-cor-1 .statement tag=046L}

*理想的根式* $a$ *在环* $A$ *是素理想包含* $a$的交 *并且它也是素数集合的最小元素的交理想。*

#### 推论 2 {#ac-ii-s2-lem-2-cor-2 .statement tag=046M}

*对于理想* $a$ *环* $A$ *我们用* $r(a)$ *根式* $a$ 表示。 *然后，对于两个理想* $a, b$ *of* $A$，
$$
r(a \cap b) = r(ab) = r(a) \cap r(b);
$$
*特别是，如果*$a \subset b$，*则*$r(a) \subset r(b)$。

对于包含$a \cap b$（或$ab$）的素理想，包含理想$a, b$之一（§ 1, no. 1，命题1）是必要且充分的。

#### 命题 14 {#ac-ii-s2-prop-14 .statement tag=046N}

*对于环的两个理想*$a, b$*互质，其根式*$r(a)$*和*$r(b)$*如此是必要且充分的。

由于$a \subset r(a)$和$b \subset r(b)$，条件的必要性是显而易见的； 条件满足§ 1, no. 2、命题 3。

#### 命题 15 {#ac-ii-s2-prop-15 .statement tag=046O}

*在环* $A$ *让* $a$ *是一个理想，并且* $b$ *有限生成的理想包含在* $a$的根部中。 *那么存在整数* $k > 0$ *这样* $b^k \subset a$。

令$(b_i)_{1 \leq i \leq n}$为$b$的生成元中的系统。到假设，存在整数$h$，使得$b_i^h \in a$对应$1 \leq i \leq n$。如果将系数在$A$的$b_i$的线性组合展开，则将$nh$元素的乘积展开，则每个项为$nh$因子的乘积倍数，其中每一个都等于$b_i$；其中因子中，至少有$h$对于某些$i$具有相同的指标$i$，因此，乘积属于到$a$和$nh$是所需的整数 $k$。

#### 推论{#ac-ii-s2-n6-cor-1 .statement tag=046P}

*在诺特环中，零激进是一个幂零理想*。

#### 命题 16 {#ac-ii-s2-prop-16 .statement tag=046Q}

*设*$B$*为环且*$A$*子环为*$B$。 *对于每个最小素理想* $p$ *of* $A$ *存在一个最小素理想* $q$ *of* $B$ *这样* $q \cap A = p$。

我们写$S = A - p$；那么环 $A_+ = S^{-1}A$ 被识别为 $S^{-1}B$ 的子环 (no. 1, 命题 2)，而另一方面 $A_+$ 只有一个素理想 $p'$，因为 $p$ 是最小的 (no. 5, 命题11）。由于 $S^{-1}B$ 不会减少到 0（因为它包含 $A_+$），因此它至少有一个素理想 $r'$，因此有 $r' \cap A_+ = p'$；如果 $j = i_B^S$ 并且我们写 $r = j'(t')$，那么
$$
i_A^S(r \cap A) \subset r' \cap A_+ = p'
$$
因此$r \cap A \subset p$，并且由于$p$是最小的，因此$t \cap A = p$；此外，$r$在$B$中是素数；如果 $q$ 是 $r$ (引理 1) 中包含的 $B$ 的最小素理想，则更不必说 $q \cap A = p$，因为 $p$ 是最小的。

#### 定义 5 {#ac-ii-s2-def-5 .statement tag=046R}

A ring $A$ is called reduced if its nilradical is reduced to 0, in other words if no element $\neq 0$ of $A$ is nilpotent.

如果 $\mathfrak{N}$ 是环 $A$ 的零根，$A/\mathfrak{N}$ 会减少，因为 if 类 mod。 元素$x \in A$的$\mathfrak{N}$在$A/\mathfrak{N}$上是幂零的，这意味着$x^h \in \mathfrak{N}$对于某些整数$h$，因此$x^{hk} = 0$对于某些整数$k$和$x \in \mathfrak{N}$。

#### 命题 17 {#ac-ii-s2-prop-17 .statement tag=046S}

设 $A$ 为环，$\mathfrak{N}$ 为零根。对于$A$的每个乘法子集$S$，$S^{-1}\mathfrak{N}$是$S^{-1}A$的零根。特别是，如果$A$减小，则$S^{-1}A$也减小。

如果$x \in A$，$s \in S$满足$(x/s)^n = x^n/s^n = 0$，则存在$s' \in S$使得$s'x^n = 0$（no. 1，注3）和更不必说$(s'x)^n = 0$，因此$s'x \in \mathfrak{N}$和$x/s = s'x/s's \in S^{-1}\mathfrak{N}$； 逆命题是直接的。

### 7. 分数张量积和同态模

#### 命题 18 {#ac-ii-s2-prop-18 .statement tag=046T}

令$A$为环，且$S$为$A$的乘法子集。

(i) 如果$M$和$N$是两个$A$模块，则$S^{-1}A$模块$(S^{-1}M) \otimes_A N, M \otimes_A (S^{-1}N)$、$(S^{-1}M) \otimes_{S^{-1}A} (S^{-1}N)$和$S^{-1}(M \otimes_A N)$是规范同构的。

(ii) 如果$M$和$N'$是两个$S^{-1}A$模块，则典范同态
$$
M' \otimes_A N' \to M' \otimes_{S^{-1}A} N'
$$
源自 $A$-双线性映射 $(x', y') \mapsto x' \otimes y'$ 从 $M' \times N'$ 到 $M' \otimes_{S^{-1}A} N'$
是双射的
断言 (i) 是直接的推论 / 定义 $S^{-1}M =$

M \otimes_A S^{-1}A 和张量积的结合性，得到典范同构

$$
(S^{-1}M \otimes_{S^{-1}A} (S^{-1}N)) = (S^{-1}M) \otimes_{S^{-1}A} (S^{-1}A \otimes N) = (S^{-1}M) \otimes_A N \\
= (S^{-1}A) \otimes_A M \otimes_A N = S^{-1}(M \otimes_A N).
$$

为了证明(ii)，我们注首先在$M'$和$N'$中，被视为$A$模，元素$s \in S$诱导的同位是双射的，因此$M' = S^{-1}M'$和$N' = S^{-1}N'$（no. 2， 注 4) 类似$S^{-1}(M' \otimes_A N') = M' \otimes_A N'$； (ii) 是 (i) 的特例。

#### 推论{#ac-ii-s2-n7-cor-1 .statement tag=046U}

令$M$为$A$模，$a$为$A$的理想。子$S^{-1}A$模块$(S^{-1}a)(S^{-1}M)$、$a(S^{-1}M)$、$(S^{-1}a)j(M)$（其中$j : M \to S^{-1}M$是典范映射）和$S^{-1}M$的$S^{-1}(aM)$是相同的。特别地，如果$a$和$b$是$A$的两个理想，那么

$$
(S^{-1}a)(S^{-1}b) = a(S^{-1}b) = (S^{-1}a)b = S^{-1}(ab).
$$

#### 注 {#ac-ii-s2-n7-rem-1 .statement tag=046V}

令$M, N, P$为三个$A$-模，$f : M \times N \to P$一个$A$-双线性映射和$S^{-1}f : (S^{-1}M) \times (S^{-1}N) \to (S^{-1}P)$通过将标量的环延伸到$S^{-1}A$从$f$获得的$S^{-1}A$-双线性映射 （代数，章IX, § 1, no. 4，命题1）。设$i : M \to S^{-1}M, j : N \to S^{-1}N$为典范同态；紧接着，如果$Q$是$f(M \times N)$生成的$P$的子$A$模块，则$S^{-1}Q$是$(S^{-1}f)(i(M) \times j(N))$生成的$S^{-1}P$的子$S^{-1}A$模块。

#### 命题 19 {#ac-ii-s2-prop-19 .statement tag=046W}

令$A$为环，且$S$为$A$的乘法子集。
(i) 如果 $M$ 和 $N$ 是两个 $A$ 模块，并且 $M$ 是有限生成的（或有限呈现的），则典范同态 (章 I, §2, no. 10, 公式 (10))

$$
S^{-1}\operatorname{Hom}_A(M, N) \to \operatorname{Hom}_{S^{-1}A}(S^{-1}M, S^{-1}N)
$$

是单射（或双射）。
(ii) 如果 $M', N'$ 是两个 $S^{-1}A$ 模块，则规范的双射

$$
\operatorname{Hom}_{S^{-1}A}(M', N') \to \operatorname{Hom}_A(M', N')
$$

是双射的。

由于 $S^{-1}A$ 是一个平面 $A$ 模，(i) 是章 I, §2, no. 10、命题 11 的特例。另一方面，我们已经指出，$S^{-1}A$ 模的每个 $A$ 同态必然是 $S^{-1}A$ 同态，在证明命题 3 课程，共 no. 2； 从而（二）。

#### 命题 20 {#ac-ii-s2-prop-20 .statement tag=046X}

令$A, A'$为两个环、$p : A \to A'$同态、$S$$A$、$S' = \rho(S)$和$\rho' : S^{-1}A \to {S'}^{-1}A'$同态相应的到$p$的乘法子集 （no. 1，命题2）。

(i) *对于每个* $A'$-模块$M'$，都存在唯一的$S^{-1}A$-同构
$$
j : S^{-1}\rho_*(M') \to \rho'_*({S'}^{-1}M')
$$
*这样*$j(m'/s) = m'/\rho(s)$*对于所有人*$m' \in M', s \in S$。

(ii) *对于每个* $A$-模块$M$，都存在一个唯一的同构
$$
j' : (S^{-1}M) \otimes_{S^{-1}A} ({S'}^{-1}A') \to {S'}^{-1}(M \otimes_A A')
$$
*的*${S'}^{-1}A'$*-模块* *使得*$j'((m/s) \otimes (a'/s')) = (m \otimes a')/(\rho(s)s')$。

(i) 如果我们通过复合同态$i^{S'}_{M'} \circ p$将${S'}^{-1}M'$视为$A$模，则$S$的元素诱导的同位是双射的，因此存在唯一同态$j$与所述性质 （no. 2，命题3）。由于 $\rho(S) = S'$，$j$ 是满射；此外，如果$m' \in M'$，$s \in S$，$m'/\rho(s) = 0$，则存在$t' \in S'$使得$t'm' = 0$；因为存在$t \in S$使得$\rho(t) = t', t'.m' = 0$在$\rho_*(M')$中，因此$m'/s = 0$在$S^{-1}\rho_*(M')$中。

(ii) 作为 $(S^{-1}M) \otimes_{S^{-1}A} ({S'}^{-1}A') = (M \otimes_A S^{-1}A) \otimes_{S^{-1}A} ({S'}^{-1}A')$ 和
$$
{S'}^{-1}(M \otimes_A A') = (M \otimes_A A') \otimes_{A'} ({S'}^{-1}A'),
$$
$j'$的存在源自结合性或张量积。

### 8. 申请代数

令$A$为环，$B$为$A$代数（不一定是结合律或交换律，也不一定拥有单位元），$S$为$A$的乘法子集。我们知道，在 $S^{-1}A$-模块 $S^{-1}B = B \otimes_A S^{-1}A$ 上，定义可能是一个规范的 $S^{-1}A$-*代数* 结构，据说是通过环标量到 $S^{-1}A$ 的扩张获得的(代数, 章 III, § 3) 并且乘积$(x/s)(y/t)$等于$(xy)/(st)$。如果 $e$ 是 $B$ 的单位元，$e/1$ 是 $S^{-1}B$ 的单位元，并且如果 $B$ 是结合律（或可交换的），则 *so* 是 $S^{-1}B$。

令 $A$ 为环且 $M$ 为 $A$ 模；我们用$T(M)$（分别为$\Lambda(M)$、$S(M)$）表示$M$（代数、章 111）的*张量* 代数（分别为外部代数、对称代数）。众所周知，对于每个交换$A$-代数$C$，都存在一个唯一的$T(M) \otimes_A C$到$T(M \otimes_A C)$的同构$j$（分别是$\Lambda(M) \oplus_A C$到$\Lambda(M \otimes_A C)$，$S(M) \otimes_A C$到$S(M \otimes_A C)$），这样那个
$$
i(x \otimes 1) = x \otimes 1
$$
对于所有 $x \in M$，$M$ 均被规范地标识为子模或 $T(M)$（分别为$\Lambda(M), S(M)$）（*loc.cit.*）。然后特别可以看出，对于$A$的每个乘法子集$R$，有*典范同构*
$$
R^{-1}T(M) \to T(R^{-1}M), \qquad R^{-1}\Lambda(M) \to \Lambda(R^{-1}M), \qquad R^{-1}S(M) \to S(R^{-1}M)
$$
其中约化对应于 $R^{-1}M$ 上的身份。

### 9. 模分数评分模

令$A$为分级环，$M$为分级$A$模，$A$次数幺半群；我们假设在这个没有。 $A$ 是 *群*。回想一下 (*代数*, 章 II, § 11)，$A$ 和 $M$ 分别是直和或加法群
$$
A = \bigoplus_{i \in \Delta} A_i, \qquad M = \bigoplus_{i \in \Delta} M_i
$$
$A_i A_j \subset A_{i+j}$ 和 $A_i M_j \subset M_{i+j}$ 代表所有 $i, j \in A$。令 $S$ 为 $A$ 的乘法子集 *所有元素都是齐次的*。对于所有$i \in A$，我们写为$S_i = S \cap A_i$并用元素$m'$的$(S^{-1}M)_i$集合表示$S^{-1}M$，其中存在$A$、元素的元素$j, k$ $m \in M_j$和元素$s \in S_k$使得$j - k = i$和$m' = m/s$。如果 $(m'_q)_{1 \leq q \leq r}$ 是元素 $S^{-1}M$ 的有限族，使得
$$
m'_q \in (S^{-1}M)_{j(q)},
$$
存在元素$j(q) \in A$和$k \in A$，元素$m_q \in M_{j(q)}$（$1 \leq q \leq r$）和$s \in S_k$，使得$m'_q = m_q/s$对于$1 \leq q \leq r$（no. 1，*注2*）。

#### 命题 21 {#ac-ii-s2-prop-21 .statement tag=046Y}

*环 $S^{-1}A$ 与家人一起 $((S^{-1}A)_i)$ 为环等级，$S^{-1}M$ 与家人一起 $((S^{-1}M)_i)$ 为模等级，高于环 $S^{-1}A$ 等级。 典范映射 $i^S_A$ 和 $i^S_M$ 是次数 0 的齐次。*

令 $m \in M$、$s \in S_k$、$m' \in M_{j'}$、$s' \in S_{k'}$ 并假设 $j - k = j' - k' = i$；然后$(m/s) - (m'/s') = (s'm - sm')/ss'$、$s'm - sm' \in M_{j'+k'} = M_{j'+k'}$、$ss' \in S_{k+k'}$，因此$(m/s) - (m'/s') \in (S^{-1}M)_i$乘以定义；这表明$(S^{-1}M)_i$是$S^{-1}M$的加法子群。 其中群中的和是$S^{-1}M$的整数：对于每个$x \in S^{-1}M$可以写成$m/s$，其中$m \in M, s \in S; s$与假设齐次，$m$是齐次元素$m_j$的和；因此，$x$是$m_j/s$的和，其中每个属于到子群$(S^{-1}M)_i$。 最后$(S^{-1}M)_i$的和是直接的；让我们考虑一个由元素 $x_q$ ($1 \leq q \leq n$) 组成的有限族，使得 $x_q \in (S^{-1}M)_{i(q)}$，其中指标 $i(q)$ 不同，并假设 $\sum_{q=1}^n x_q = 0$。 每个$x_q$可以写成$x_q = m_q/s$，其中$s \in S_k$和$m_q \in M_{i(q)+k}$； 假设意味着存在$s' \in S$使得$s'\left( \sum_{q=1}^n m_q \right) = 0$；如果$s'm_q$不全是零，我们就会产生矛盾，因为如果$s' \in S_d$，那么$s'm, \in M_{i(q)+d}$和$i(q) + d$都是不同的。 由此可见，对于每个指标$q$，$x_q = 0$。

立即验证，如果$a \in (S^{-1}A)_i$和$x \in (S^{-1}M)_j$，则$ax \in (S^{-1}M)_{i+j}$。 应用这个结果对应于$M = A$，我们首先看到$S^{-1}A$是由$(S^{-1}A)_i$评分的环；然后我们看到$S^{-1}M$的评分为模高于$S^{-1}A$。最后，由于 $1 \in A_0$、$i_A^S$ 和 $i_M^S$ 是次数 0 的齐次。

#### 命题 22 {#ac-ii-s2-prop-22 .statement tag=046Z}

设A（分别B）是型A的分级环，M（分别N）是分级模在分级环A（分别B）上的分级模，S（分别T）是A（分别B）的乘法子集，所有元素都是齐次的， $f : A \to B$ 次数 0 的齐次同态使得 $f(S) \subset T$ 和 $u : M \to N$ A-线性映射次数 k 齐次。那么从 f (no. 1, 命题 2) 导出的同态 $f' : S^{-1}A \to T^{-1}B$ 是次数 0 和$(S^{-1}A)$-线性映射的齐次

$$
u' : S^{-1}M \to T^{-1}N
$$

由 f 和 $u$ (no. 2, 命题 5) 导出是次数 k 的齐次。

这可以直接从方程 $f'(a/s) = f(a)/f(s)$ 和 $u'(m/s) = u(m)/f(s)$ 得出。

最后我们注，如果E是分级的A-代数，而S是齐次元素、$S^{-1}E$的由……组成的乘法子集及其$(S^{-1}A)$-代数结构（no. 8）和分级$(S^{-1}E)_i$ 是分级的 $S^{-1}A$ 代数，紧随定义如下。

### 习题 {#ac-ii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
