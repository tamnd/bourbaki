---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 6
section_title: Morita Equivalence of Modules and Algebras
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.95-A VIII.117
pdf_pages: 0112-0134
extraction: native+ocr
subsections:
    - "no": 1
      title: Commutant and Duality
      page: 95
      pdf_page: 112
    - "no": 2
      title: Generating Modules and Finitely Generated Projective Modules
      page: 98
      pdf_page: 115
    - "no": 3
      title: Invertible Bimodules and Morita Equivalence
      page: 100
      pdf_page: 117
    - "no": 4
      title: The Morita Correspondence of Modules
      page: 103
      pdf_page: 120
    - "no": 5
      title: Ordered Sets of Submodules
      page: 106
      pdf_page: 123
    - "no": 6
      title: Other Properties Preserved by the Morita Correspondence
      page: 109
      pdf_page: 126
    - "no": 7
      title: Morita Equivalence of Algebras
      page: 111
      pdf_page: 128
statements: 40
exercises: 8
content_sha256: 0daef8d30578412aeb6f8080ff1c4517f23b3d8e79f2edee89a0dd17e475061d
translated_from: content/en/alg/VIII/06_s6_morita_equivalence_of_modules_and.md
translation_method: google
source_content_sha256: e8ef2b43442fbc25b56375b83b63be74c37d7c8014a9723fb60c9bc369cd90cb
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 0119eec1cbbdcd17db2c5c26272911a57b538b62784aa6028ebbddc26120ac24
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 6。 森田等价 / 模和代数

在这个截面中，$k$表示交换环。

### 1. 对易子和对偶性

设 A 和 B 为 $k$-代数。回想一下 (III, §4, No. 3, p. 466)，代数 A 和 B 上的双模是一个 $(A$, B)-双模 P，其中两个 $k$-模结构从 A- 和 B-模结构重合推导出来。为了避免任何歧义，我们说 P 是一个 $(A,B)_k$ 双模。令 P 为 $(A,B)_k$ 双模。我们用$P^*$表示左A-模底层P的对偶Hom$_A(P,A)$。它是一个$(B,A)_k$双模（II, §1, No. 14，p. 226）；对于 $a\in A$、$b\in B,x\in P$ 和 $x^*\in P^*$，我们有

$$
\langle x, bx^*a\rangle =\langle xb, x^*\rangle a \tag{1}
$$

我们用 $_sA_d$ 代数 A 表示被视为 $(A,A)_k$-双模（前述），并用 $\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ 同态表示 $(A,A)_k$-双模，由下式确定：

$$
\Lambda (x\otimes x^*) =\langle x, x^*\rangle \tag{2}
$$

对于 $x\in P$ 和 $x^*\in P^*$。我们用$\widetilde{P}$表示底层P的右B-模的对偶Hom$_B(P,B)$；它是一个 $(B,A)_k$ 双模块。我们用 $(B,B)_k$ 双模的 $\widetilde{\Lambda} :\widetilde{P}\otimes_AP\rightarrow_sB_d$ 同态表示，该双模由 (3) $\widetilde{\Lambda}(\widetilde{x}\otimes x) =\langle \widetilde{x}, x\rangle$ 确定

对于 $x\in P$ 和 $\widetilde{x}\in \widetilde{P}$。

现在，假设从 B 到 End$_A(P)$ 映射 $b\mapsto b_P$ 是双射；那么从B到End$_A(P)$的反代数就是同构。从 $P^*\otimes_AP$ 到 End$_A(P)$ (II, §4, No. 2, p. 271) 的 $\mathbf{Z}$-模块中的典范同态，然后是$\mathbf{Z}$-模块 $\Theta  : P^*\otimes_AP\rightarrow$ 的确定同态 B 定义为

$$
x\Theta (x^*\otimes y) =\langle x, x^*\rangle y \tag{4}
$$

对于 $x, y\in P$ 和 $x^*\in P^*$。由于 (1)，这个同态是 $(B$, B)-线性，并且我们有

$$
\Theta (x^*\otimes y)y^*=x^*\langle y, y^*\rangle \tag{5}
$$

对于 $y\in P$ 和 $x^*, y^*\in P^*$。从(4)和(5)，我们推导出$(B,B)_k$-双模$P^*\otimes_AP:$中的以下等式

$$
(y^*\otimes x)\Theta (x^*\otimes y) =y^*\otimes  \langle x, x^*\rangle y=y^*\langle x, x^*\rangle  \otimes y= \Theta (y^*\otimes x)(x^*\otimes y)
$$

对于 $x, y\in P$ 和 $x^*, y^*\in P^*$，因此

$$
s\Theta (t) = \Theta (s)t \tag{6}
$$

$s, t\in P^*\otimes_AP$。同样，对于P中的$x, y$和$P^*$中的$x^*, y^*$，我们从(4)和(5)推导出$(A,A)_k$双模$P\otimes_BP^*$中的以下等式：

$$
(x\otimes x^*)\langle y, y^*\rangle =x\otimes \Theta (x^*\otimes y)y^*=x\Theta (x^*\otimes y)\otimes y^*=\langle x, x^*\rangle (y\otimes y^*)
$$

因此

$$
u\Lambda (v) = \Lambda (u)v \tag{7}
$$

$u, v\in P\otimes_BP^*$。

对于$P^*$的任何元素$x^*$，用$\sigma (x^*)$表示从P到B的B-线性映射$x\mapsto \Theta (x^*\otimes x)$。因此，我们从$P^*$到$\widetilde{P}$定义映射$\sigma$，即$(B$，A)-线性，并满足定义，

$$
\Theta (x^*\otimes y) =\langle \sigma (x^*), y\rangle \tag{8}
$$

对于 $x^*\in P^*$ 和 $y\in P$。通过 $\widetilde{\Lambda}$ 的定义，我们有

$$
\Theta  =\widetilde{\Lambda}\circ (\sigma \otimes 1_P) \tag{9}
$$

假设从 A 到 End$_B(P)$ 映射 $a\mapsto a_P$ 是双射；那么就是代数同构。类似地，我们将 $(A,A)_k$-双模 $\widetilde{\Theta} : P\otimes_B\widetilde{P}\rightarrow_sA_d$ 乘以设定定义同态

$$
\widetilde{\Theta}(x\otimes \widetilde{y})y=x\langle \widetilde{y}, y\rangle \tag{10}
$$

对于 $x, y\in P$ 和 $\widetilde{y}\in \widetilde{P}$。我们还通过设定 $(B,A)_k$-双模块 $\widetilde{\sigma}:\widetilde{P}\rightarrow P^*$ 定义同态

$$
\widetilde{\Theta}(x\otimes \widetilde{y}) =\langle x,\widetilde{\sigma}(\widetilde{y})\rangle \tag{11}
$$

对于$x\in P,\widetilde{y}\in \widetilde{P}$。我们有

$$
\widetilde{\Theta} = \Lambda \circ (1_P\otimes \widetilde{\sigma}) \tag{12}
$$

#### 命题 1 {#alg-viii-s6-prop-1 .statement tag=006R}

假设从B到End$_A(P)$的映射$b\mapsto b_P$和从A到End$_B(P)$的$a\mapsto a_P$是双射的。那么$\sigma$和$\widetilde{\sigma}$是逆同构，我们有关系

$$
\Lambda  =\widetilde{\Theta}\circ (1_P\otimes \sigma ) \tag{13}
$$

$$
\widetilde{\Lambda} = \Theta \circ (\widetilde{\sigma}\otimes 1_P) \tag{14}
$$

对于 $x\in P,x^*\in P^*$ 和 $y\in P$，通过关系 (4)、(8)、(10) 和 (11)，我们有

$$
(15)\langle x, x^*\rangle y=x\Theta (x^*\otimes y) =x\langle \sigma (x^*), y\rangle =\widetilde{\Theta}(x\otimes \sigma (x^*))y=\langle x,\widetilde{\sigma}(\sigma (x^*))\rangle y
$$

同样，对于$x\in P,\widetilde{y}\in \widetilde{P}$和$y\in P$，我们有

$$
x\langle \widetilde{y}, y\rangle =\widetilde{\Theta}(x\otimes \widetilde{y})y=\langle x,\widetilde{\sigma}(\widetilde{y})\rangle y=x\Theta  (\widetilde{\sigma}(\widetilde{y})\otimes y) =x\langle \sigma (\widetilde{\sigma}(\widetilde{y})), y\rangle \tag{16}
$$

由于假设，P 忠实于A-模和B-模。分别从关系 (15) 和 (16) 推导出 $\widetilde{\sigma}\circ \sigma = 1_{P^*}$ 和 $\sigma \circ \widetilde{\sigma}=$ $1_{\widetilde{P}}$。 关系 (13) 和 (14) 分别由 (12) 和 (9) 得出。

#### 注 1 {#alg-viii-s6-n1-rem-1 .statement tag=006S}

假设从 B 到 End$_A(P)$ 映射 $b\mapsto b_P$ 是双射的。然后

a) B-模 P 可以用 P 的对模来识别；因此它是忠实且平衡的；

b) 从A到End$_B(P)$的映射$a\mapsto a_P$是双射当且仅当A-模P是忠实且平衡的。

#### 注 2 {#alg-viii-s6-n1-rem-2 .statement tag=006T}

在命题 1 的假设下，A-模 P 是平衡的；由于环$A_P$和$A'_P$具有相同的中心（VIII，p. 77），因此从环A的中心Z(A)到中心有同构$\varphi$ 环 B 的 Z(B)，由 $z\in Z(A)$ 的关系 $\varphi (z)_P=z_P$ 确定。此外，$(A,B)_k$-双模P的自同态是同位$z_P$，其中$z$穿过Z(A)； $(A,B)_k$-双模 P 的自同构是同位 $z_P$，其中 $z$ 在 Z(A) 中可逆。

### 2. 生成模和有限生成射影模

#### 命题 2 {#alg-viii-s6-prop-2 .statement tag=006U}

设 A 和 B 为代数超过 $k$，并令 P 为 $(A,B)_k$ 双模。假设从 B 到 End$_A(P)$ 映射 $b\mapsto b_P$ 是双射的。以下断言是等效的：

(i) A-模 P 是射影且有限生成的。

(ii) 映射 θ (VIII, p. 96) 是从 $P^*\otimes_AP$ 到 $_sB_d$ 的 $(B,B)_k$ 双模的同构。

(iii) B 的 θ 包含单位元的像。

此外，如果从 A 到 End$_B(P)$ 映射 $a\mapsto a_P$ 是双射，则上面的断言等价于下面的叙述：

(iv) 从$Q\otimes_AP$到$_sB_d$存在$(B,A)_k$-双模Q和满同态的$(B,B)_k$-双模。

由 II, §4, No. 2、p. 271、断言的推论 (i) 意味着 (ii)。此外，(iii) 由(ii) 得出。令$t\in B^*\otimes_AB$ 使得$\Theta (t) = 1$。令$n$为整数，并令$(x_1, . . . , x_n)\in P^n$和$(x^*_1, . . . , x^*_n)\in P^{*n}$为$t=\sum^n_{i=1}x^*_i\otimes x_i$。对于每个 $x$ 属于到 P，关系 $x\Theta (t) =x$ 可以写成

$$
\sum_{i=1}^n\langle x, x^*_i\rangle x_i=x
$$

由此可见，A-模 P 由$(x_i)_{1\leqslant i\leqslant n}$族有限生成，并且我们使用II, §2, No. 6、p. 238的命题 12 来得到蕴涵 (iii) $\Rightarrow$ (i) 的结论证明。

显然我们有 (ii) $\Rightarrow$ (iv)。设Q是从$Q\otimes_AP$到$_sB_d$的$(B,B)_k$双模的$(B,A)_k$双模和$\theta$满同态。在前面的小节的记号中，存在$(B,A)_k$双模$\zeta : Q\rightarrow \widetilde{P}$的同态，使得$\theta (y\otimes x) =\langle \zeta (y), x\rangle$对应于$x\in P$和$y\in Q$，我们有$\theta =\widetilde{\Lambda}\circ (\zeta \otimes 1_P)$。由于 $\theta$ 是满射，因此$\widetilde{\Lambda}$ 也同样成立。如果从A到End$_B(P)$的映射$a\mapsto a_P$是双射，则θ是VIII、p. 97的命题 1的关系(14)满射；蕴涵 (iv) $\Rightarrow$ (iii) 如下。

#### 命题 3 {#alg-viii-s6-prop-3 .statement tag=006V}

设 A 和 B 为 $k$ 上的代数，且 P 为 $(A,B)_k$ 双模。以下属性是等效的：

(i) A-模 P 为生成的。

(ii) 映射Λ中的像从$P\otimes_BP^*$到$_sA_d$（VIII，p. 95）包含单位元。

(iii) 从$P\otimes_BQ$到$_sA_d$存在$(B,A)_k$-双模Q和满同态的$(A,A)_k$-双模。

此外，如果从 B 到 End$_A(P)$ 映射 $b\mapsto b_P$ 是双射，则断言等价于以下叙述：

(iv) 映射Λ是同构从$P\otimes_BP^*$到$_sA_d$。

(i) $\Leftrightarrow$ (ii): Λ 的像是理想迹$\tau (P)$ (VIII, p. 80)。因此，(i)和(ii)的等价由VIII、p. 80的定理 1得出。

(ii)$\Rightarrow$ (iii)：取$Q = P^*$即可。

(iii) $\Rightarrow$ (ii)：令 Q 为从 $P\otimes_BQ$ 到 $_sA_d$ 的$(A,A)_k$-双模的 $(B,A)_k$ 双模和 $\psi$ 同态。从 Q 到 $P^*$ 存在 $(B,A)_k$ 双模 Ψ 的同态，使得 $\psi (x\otimes y) =\langle x,\Psi (y)\rangle$ 对应于 $x\in P$ 和 $y\in Q$，并且我们有等式 $\psi = \Lambda \circ (1_P\otimes \Psi )$。如果 $\psi$ 是满射，那么 Λ 也是满射。

显然，(iv) 暗示着(ii)。相反，假设性质 (ii) 成立，并且从 B 到 End$_A(P)$ 映射 $b\mapsto b_P$ 是双射的。令 $e$ 为 $P\otimes_BP^*$ 的元素，使得 $\Lambda (e) = 1$。到VIII、p. 96的关系(7)，$P\otimes_BP^*$中每$u$就有$u= \Lambda (u)e$； Λ 的单射性如下。

#### 命题 4 {#alg-viii-s6-prop-4 .statement tag=006W}

设 A 和 B 为 $k$-代数，P 为 $(A,B)_k$-双模。假设从 B 到 End$_A(P)$ 映射 $b\mapsto b_P$ 是双射的。

a) 如果 A-模 P 是生成的，则右B-模 P 是射影且有限生成的。

b) 如果 A-模 P 是射影且有限生成的，则右B-模 P 是生成的。

假设A-模 P 是生成的。那么它是忠实且平衡的（VIII，p. 82，定理2），因此从A到End$_B(P)$的映射$a\mapsto a_P$是双射的（VIII，p. 97，注1）。此外，映射$\Lambda  : P\otimes_BP^*\rightarrow_sA_d$是双射（VIII，p. 98，命题3）。我们将 P 视为 $(B^o,A^o)_k$ 双模。 映射 Λ 诱导双射映射 $P^*\otimes_{B^o}P\rightarrow A^o$；由 VIII、p. 98、(iv) $\Rightarrow$ (i)、右B-模的命题 2 P 是射影且有限生成的。

现在，假设 A-模 P 是射影且有限生成的。那么映射 $\Theta  : P^*\otimes_AP\rightarrow_sB_d$ 是双射 (loc. cit., (i) $\Rightarrow$ (ii))。将上述命题 3 的 (iii) $\Rightarrow$ (i) 应用于$(B^o,A^o)_k$-双模 P，右B-模 P 为生成的。

#### 推论 1 {#alg-viii-s6-prop-4-cor-1 .statement tag=006X}

生成模的对模是射影且有限生成的。 有限生成射影模中的对模是生成的。

设 A 为 $k$ 代数，M 为 A-模。我们用 B 表示代数 End$_A(M)$ 的相反 $k$ 代数。推论来自应用于 $(A,B)_k$ 双模 M 的命题 4。

#### 推论 2 {#alg-viii-s6-prop-4-cor-2 .statement tag=006Y}

设 A 和 B 为 $k$-代数，P 为 $(A,B)_k$-双模。以下属性是等效的：

(i) A-模 P 是生成的，并且从 B 到 End$_A(P)$ 的映射 $b\mapsto b_P$ 是双射的。

(ii) 右B-模 P 是射影、有限生成、忠实且平衡的，并且从 A 到 End$_B(P)$ 的映射 $a\mapsto a_P$ 是双射的。

蕴涵 (i) $\Rightarrow$ (ii) 由命题 4, a) 和注 1 (VIII, p. 97) 得出。假设 (ii) 成立；那么 A-模 P 是生成的 (命题 4, b) 应用于$(B^o,A^o)_k$-双模 P)。由于B-模 P 是忠实且平衡的，因而 (i) 的第二个断言也满足 (VIII, p. 97, 注 1)。

### 3. 可逆双模和森田等价

#### 定义 1 {#alg-viii-s6-def-1 .statement tag=006Z}

设 A 和 B 为 $k$-代数，P 为 $(A,B)_k$ 双模。如果存在$(B,A)_k$双模Q，使得$P\otimes_BQ$同构于$_sA_d$且$Q\otimes_AP$同构于$_sB_d$，我们称P是可逆的。这样的双模 Q 被称为 P 的逆。

设 A 和 B 为 $k$-代数，并令 P 为可逆 $(A,B)_k$ 双模。令C为$k$代数，$P'$为可逆的$(B,C)_k$双模。最后，令Q和$Q'$分别是P和$P'$的逆双模。通过张量积 (II, §3, No. 8, p. 258, 命题 8) 的结合性和 II, §3, No. 4, p. 249 的命题 4，$(C,A)_k$ 双模 $Q'\otimes_BQ$ 是$(A,C)_k$-双模$P\otimes_BP'$，因而$P\otimes_BP'$是可逆的$(A,C)_k$-双模。

因而，关系

“A和B是$k$-代数，并且存在可逆的$(A,B)_k$-双模”是等价关系。

#### 定义 2 {#alg-viii-s6-def-2 .statement tag=0070}

如果存在可逆 $(A,B)_k$-双模，则两个 $k$-代数 A 和 B 称为 Morita 等价。如果 $\mathbf{Z}$-代数 A 和 B 是 Morita 等价的，环 A 和 B 被称为 Morita 等价。

两个同构 $k$-代数是 Morita 等价的。如果两个$k$-代数是森田等价的，那么它们的反代数是森田等价的。

设 P 是可逆 $(A, B)_k$ 双模，Q 是 P 的逆。那么 Q 是可逆 $(B, A)_k$ 双模，并且 P 作为逆。此外，将 P 视为 $(B^\circ, A^\circ)_k$ 双模，P 是可逆的，且 $(A^\circ, B^\circ)_k$ 双模 Q 是逆的。

#### 引理 1 {#alg-viii-s6-lem-1 .statement tag=0071}

— *设 A 和 B 为 K-代数，P 为可逆 $(A, B)_k$ 双模，M 和 N 为 B-模，$u : M \to N$ 为 B-线性映射。如果映射 $1_P \otimes u : P \otimes_B M \to P \otimes_B N$ 是零（分别是双射），那么 u 也是。*

令 Q 为 P 的双模逆，且为 $(B, B)_k$ 双模的 $\theta : Q \otimes_A P \to {}_s B_d$ 同构的。 引理源自图表的交换律

$$
\begin{array}{ccc}
Q \otimes_A P \otimes_B M & \xrightarrow{1_Q \otimes 1_P \otimes u} & Q \otimes_A P \otimes_B N \\
\downarrow \theta \otimes 1_M & & \downarrow \theta \otimes 1_M \\
M & \xrightarrow{u} & N.
\end{array}
$$

#### 定理 1 {#alg-viii-s6-thm-1 .statement tag=0072}

*设 A 和 B 为 K-代数，P 为 $(A, B)_k$ 双模。用 $P^*$ 表示 $(B, A)_k$-双模 $\operatorname{Hom}_A(P, A_s)$。以下属性是等效的：

(i) *$(A, B)_k$-双模 P 是可逆的。*

(ii) *A-模 P 是射影、有限生成的，并且从 B 到 $\operatorname{End}_A(P)^{\circ}$ 的生成的和映射 $b \mapsto b_P$ 是 K-代数同构。*

(iii) *右B-模 P 是射影、有限生成的，并且从 A 到 $\operatorname{End}_B(P)$ 的生成的和映射 $a \mapsto a_P$ 是 K-代数同构。*

如果这些性质成立，那么同态

$$
\Theta : P^* \otimes P \to {}_s B_d \quad \text{and} \quad \Lambda : P \otimes P^* \to {}_s A_d
$$

是同构，因而$(B, A)_k$双模$P^*$是P的逆。

如果性质 (ii) 成立，则 P 是可逆 $(A, B)_k$ 双模，具有逆 $P^*$ (VIII, p. 98, 命题 2 和 p. 98, 命题 3)。这证明了 (ii) 蕴涵 (i) 和最后一个断言。

假设 $(A, B)_k$-双模 P 是可逆的。那么A-模 P 就是生成的 (VIII, p. 98, 命题 3, (iii) $\Rightarrow$ (i))。因而，它是忠实且平衡的（VIII、p. 82、定理 2），因而，从 A 到 $\operatorname{End}_B(P)$ 的映射 $a \mapsto a_p$ 是双射的。

现在让我们证明从B到$\operatorname{End}_A(P)$的映射$b \mapsto b_P$是双射的。设 Q 为 $(B, A)_k$ 双模，与 P 相反。设 $u \in \operatorname{End}_A(P)$；那么$1_Q \otimes u$是左B-模$Q \otimes_A P$中的自同态。由于$(B, B)_k$双模$Q \otimes_A P$与$_s B_d$同构的，因此存在B的唯一元素$b$，使得$1_Q\otimes u$是位似，比率$b$为右B-模$Q\otimes_AP$。因而，我们有 $1_Q\otimes (u-b_P) = 0$。因而，$u=b_P$乘以引理1；这证明从 B 到 End$_A(P)$ 映射 $b\mapsto b_P$ 是双射的。

通过 VIII、p. 98、A-模的命题 2，然后 P 是射影且有限生成的。因此我们证明了 (i) 和 (ii) 的等价。

通过交换A和B的角色，我们得到(i)和(iii)的等价，其中命题的结论证明。

#### 推论 1 {#alg-viii-s6-lem-1-cor-1 .statement tag=077O}

设 A 和 B 为 Morita 等价的 $k$-代数，并令 P 为可逆的 $(A,B)_k$ 双模。对于每个$z\in Z(A)$，从A的中心Z(A)到B的中心存在同构$\varphi$，由关系$\varphi (z)_P=z_P$确定。 $(A,B)_k$-双模 P 的自同构是同位$z_P$，其中 $z$ 是 Z(A) 的可逆元。

给定定理 1，这是从 VIII、p. 97 的注 2 得出的。

#### 推论 2 {#alg-viii-s6-lem-1-cor-2 .statement tag=077P}

设 A 和 B 为 Morita 等价的$k$-代数，并令 P 为可逆的$(A,B)_k$-双模。 P 的每个 $(B,A)_k$-双模逆元都同构于 P 的对偶 $P^*=$ Hom$_A(P,A)$。更准确地说，令 Q 为 P 的逆元 $(B,A)_k$-双模，并令 $\lambda : P\otimes_BQ\rightarrow_sA_d$ 为 $(A,A)_k$-双模的同构。对于$p\in P$和$q\in Q$，存在由关系$\langle p, \tau (q)\rangle =\lambda (p\otimes q)$确定的唯一映射$\tau : Q\rightarrow P^*$，$\tau$是$(B,A)_k$双模的同构。

映射$\tau$的存在性和唯一性是明确的。它是$(B,A)_k$双模的同态，我们有$\lambda = \Lambda \circ (1_P\otimes \tau )$。由于$\lambda$和Λ是$(A,A)_k$双模（VIII、p. 101、定理 1）的同构，$1_P\otimes \tau$也是如此。到引理 1 时，映射 $\tau$ 是双射的。

#### 注 {#alg-viii-s6-n3-rem-1 .statement tag=0075}

在推论的假设下，令$q$为Q的元素，这样对于每个$p\in P$我们都有$\lambda (p\otimes q) = 0$。那么我们就有$\tau (q) = 0$，即$q= 0$。同样，如果$p$是P的元素，这样对于每个$q\in Q$我们都有$\lambda (p\otimes q) = 0$，那么$p= 0$。

#### 例 1 {#alg-viii-s6-n3-exa-1 .statement tag=0076}

设 B 为 $k$ 代数，$n$ 整数 $\geqslant 1$，A 为 $k$ 代数 $\mathbf{M}_n(B)$。 右B-模 $P = B^n_d$ 是射影、有限生成的，生成的，A 可以用 P 的内同态代数来标识（II, §10, No. 7，p. 349）。到定理 1，$(A,B)_k$-双模 P 是可逆的。因此代数 B 和$\mathbf{M}_n(B)$ 是森田等价的。

#### 例 2 {#alg-viii-s6-n3-exa-2 .statement tag=00SH}

设 A 是可交换的 $k$ 代数，P A-模。我们将 P 视为一个 $(A,A)_k$ 双模，其作用的两个律相等。如果 $(A,A)_k$ 双模 P 是可逆的，则 A-模 P 是有限生成的 (定理 1)。 定理 3 通讯。代数，II, §5, No. 4，p. 114，以下性质是等价的：

(i) $(A,A)_k$-双模 P 是可逆的。

(ii) 存在 A-模 Q 使得 $P\otimes_AQ$ 与 A 同构的。

(iii) A-模 P 是射影，有限生成，且为秩 $1.*$

### 4. The Morita Correspondence of Modules

在这个小节中，字母A和B表示森田等价的$k$-代数，P表示可逆的$(A,B)_k$-双模。 选择 $(B,A)_k$-双模 Q 与 P 和同构逆

$\lambda : P\otimes_BQ\rightarrow_sA_d$ 和 $\theta : Q\otimes_AP\rightarrow_sB_d$。

对于任意左B-模V，用B-模$\theta \otimes 1_V: Q\otimes_AP\otimes_BV\rightarrow V$的$\theta_V$同态表示；它是同构，因为$\theta$是同构。同样，对于每个左A-模 M，用A-模$\lambda \otimes 1_M: P\otimes_BQ\otimes_AM\rightarrow M$的$\lambda_M$同态表示；它是同构，因为$\lambda$是同构。

#### 定理 2（森田）{#alg-viii-s6-thm-2 .statement tag=00S2}

a) 令 V 和 W 为左B-模。从 Hom$_B(V,W)$ 到 Hom$_A(P\otimes_BV,P\otimes_BW)$ 映射 $g\mapsto 1_P\otimes g$ 为双射。 逆双射将Hom$_A(P\otimes_BV,P\otimes_BW)$的元素$h$发送到Hom$_B(V,W)$的元素$\theta_W\circ (1_Q\otimes h)\circ \theta_V^{-1}$。

b) 每个左A-模 M 都同构于形式 $P\otimes_BV$ 的模，其中V 是左B-模。

令 V 和 W 为左B-模。通过VIII、p. 101、映射$\varphi :g\mapsto 1_P\otimes g$的引理 1，从Hom$_B(V,W)$到Hom$_A(P\otimes_BV,P\otimes_BW)$是单射的。通过交换 P 和 Q（以及 A 和 B）的角色，我们看到从 Hom$_A(P\otimes_BV,P\otimes_BW)$ 到 Hom$_A(Q\otimes_AP\otimes_BV,Q\otimes_AP\otimes_BW)$ 的映射 $\psi :h\mapsto 1_Q\otimes h$ 也是单射的。现在，合成$\psi \circ \varphi$是映射$g\mapsto \theta^{-1}_W\circ g\circ \theta_V$。它是双射的，因而 $\psi$ 也是双射的。因而，$\varphi$是双射，它的逆矩阵是映射$h\mapsto \theta_W\circ (1_Q\otimes h)\circ \theta^{-1}_V$。

断言 b) 从$\lambda_M$是同构这一事实得出，从$P\otimes_B$$\otimes_A\otimes M$到M。

设 V 为左B-模，W 子模为 V。由于 B-模 P 是射影（VIII、p. 101、定理 1），因此从 $P\otimes_BW$ 到 $P\otimes_BV$ 的典范映射是单射的。我们认同$P\otimes_BW$及其像在$P\otimes_BV$通过这个映射。当 P 和 B 被 Q 和 A 替代时，我们采用类似的约定。

#### 命题 5 {#alg-viii-s6-prop-5 .statement tag=0077}

设V为左B-模。 映射$W\mapsto P\otimes_BW$是从V的B-子模的集合（按包含排序）到$P\otimes_BV$的A-子模的集合（按包含排序）的同构。 逆同构将$P\otimes_BV$的A-子模N发送给$Q\otimes_AP\otimes_BV$的B-子模$Q\otimes_AN$的$\theta_V$下的像。

用V B-子模$D_B(V)$集合表示，按包含排序，定义集合$D_A(P\otimes_BV)$和$D_B(Q\otimes_AP\otimes_BV)$同理。 设$\varphi : D_B(V)\rightarrow$$D_A(P\otimes_BV)$为映射$W\mapsto P\otimes_BW$和$\psi$映射，从$D_A(P\otimes_BV)$到$D_B(Q\otimes_AP\otimes_BV)$由$N\mapsto Q\otimes_AN$给出。 它们是单调递增映射，合成 $\psi \circ \varphi$ 是映射 $W\mapsto \theta^{-1}_V$(W)，它是双射的。 因而，$\varphi$是单射的，$\psi$是满射的。 通过替换 B 与 A 以及 V 与 $P\otimes_BV$，我们看到 $\psi$ 也是单射的。 因而，$\varphi$和$\psi$是双射的，$\varphi$的逆映射确实是命题中描述的。

#### 例 1 {#alg-viii-s6-n4-exa-1 .statement tag=0078}

让我们将 VIII、p. 104 中的应用命题 5 组合到具体情况$V = B_s$。

a) 映射 $J\mapsto$ PJ 是从 B 的左理想的有序集合 $D(B_s)$ 到 P 的 A-子模的有序集合 D(P) 的同构。 逆映射将 P 的 A-子模 M 发送到 B 的左理想 J(M) B 的元素 $b$ 的由……组成使得 M 包含 $Pb$。

b) 映射 $K\mapsto$ KP 是从 A 的右理想的有序集合 $D(A_d)$ 到 P 的 B-子模的有序集合 D(P) 的同构。 逆映射将 P 的 B-子模 V 发送到A 的元素 $a$ 的由……组成的右理想 K(V) 使得 V 包含 $aP$。

事实上，A-模$P\otimes_BB_s$可以与P进行规范的等同。如果J是B的左理想，则$P\otimes_BB_s$对应中$P\otimes_BJ$的典范像通过这个等同于PJ。因而，从$D(B_s)$到D(P)，映射$J\mapsto$PJ是有序集中的同构。让$J\in D(B_s)$。将 B 的元素 $b$ 表示为集合，使得 PJ 包含 $Pb$ 为 $J'$。 包含 J 是 B 的左理想，我们有 PJ$'\subset$ PJ。由于映射$J\mapsto$PJ是有序集中的同构，所以我们必然有PJ$'=$PJ和$J = J'$。这就证明了a）。

断言 b) 由适用于可逆 $(B^o,A^o)_k$ 双模 P 的断言 a) 得出。

注环 A 是域当且仅当 B-模 P 是简单的。

#### 例 2 {#alg-viii-s6-n4-exa-2 .statement tag=0079}

分别用 A 的双边理想、B 的双边理想和 P 的 $(A,B)_k$ 子双模的 $\mathscr{B}_A,\mathscr{B}_B$ 和 $\mathscr{B}_P$ 集合表示。

a) 映射$\mathfrak{b}\mapsto P\mathfrak{b}$是从$\mathscr{B}_B$到$\mathscr{B}_P$的有序集中的同构； 逆同构将P的$(A,B)_k$子双模$P'$发送到元素$b$的B由……组成的双面理想，使得$Pb\subset P'$。

b) 映射$\mathfrak{a}\mapsto \mathfrak{a}P$是从$\mathscr{B}_A$到$\mathscr{B}_P$的有序集中的同构； 逆同构将P的$(A,B)_k$子双模$P'$发送到元素$a$的由……组成的双面理想，使得$aP\subset P'$。

事实上，令 J 为 B 和 $P'=$ PJ 的左理想。那么$P'$是P的A-子模，并且通过例1，理想的J由B的元素$b$组成，使得$Pb\subset P'$。此外，当且仅当 J 是 B 的双面理想时，$P'$ 是 P 的 $(A,B)_k$ 子双模。因此，a) 由 loc 推出。引用。

断言 b) 由适用于可逆 $(B^o,A^o)_k$ 双模 P 的断言 a) 得出。

#### 命题 6 {#alg-viii-s6-prop-6 .statement tag=007A}

用 A 的两侧理想和 B 的两侧理想的 $\mathscr{B}_A$ 和 $\mathscr{B}_B$ 集合表示。

a) There exists an isomorphism of ordered sets $f$ from $\mathscr{B}_A$ to $\mathscr{B}_B$ determined by the following property: if $\mathfrak{a}$ is a two-sided ideal of A and $\mathfrak{b}$ a two-sided ideal of B, then the relation $f(\mathfrak{a}) =\mathfrak{b}$ is equivalent to $\mathfrak{a}P = P\mathfrak{b}$.

b) 假设环 A 是可交换的，因此 A 可以与 B 的中心等价（VIII，p. 102，推论 1）。 同构 $f:\mathscr{B}_A\rightarrow$ $\mathscr{B}_B$ 将 A 的理想 $\mathfrak{a}$ 发送到 B 的双边理想 $B\mathfrak{a}$，得到 $\mathfrak{a}= A\cap B\mathfrak{a}$。

断言 a) 由例 2 推出。

现在，假设 A 是可交换的，认同 A 与 B 的中心。令 $\mathfrak{a}$ 为 A 的理想。则 $B\mathfrak{a}$ 为 B 的两侧理想；我们有 PB$\mathfrak{a}=\mathfrak{a}P$，因此有$f(\mathfrak{a}) = B\mathfrak{a}$。设$\mathfrak{a}'$为A的理想$A\cap B\mathfrak{a}$；它包含在$B\mathfrak{a}$和包含$\mathfrak{a}$中，所以$B\mathfrak{a}'$等于$B\mathfrak{a}$。由于$f$是双射的，因此$\mathfrak{a}'=\mathfrak{a}$。

#### 例 3 {#alg-viii-s6-n4-exa-3 .statement tag=007B}

设V为左B-模。然后上面给出的对应将B-模V的湮没子发送到A-模$P\otimes_BV$的湮没子。事实上，用$\mathfrak{a}$表示A-模$P\otimes_BV$的湮没子，用$\mathfrak{b}$表示B-模V。令 W 为元素的 P 由……组成的 $(A,B)_k$ 子双模，使得 $p\otimes v= 0$ 对于 V 的每个元素 $v$。我们有包含$P\mathfrak{b}\subset W$；相反，对于每个$p\in W$和$q\in Q$，我们有$\theta (q\otimes p)$属于到$\mathfrak{b}$。因此，D(P) 的 $D(B_s)$ 对应到元素 W 的元素 $\mathfrak{b}$。同样，$\mathfrak{a}\in D(A_d)$对应到W。

#### 例 4 {#alg-viii-s6-n4-exa-4 .statement tag=007C}

对于 A 的任何双面理想 $\mathfrak{a}$，用 $\mathbf{M}_n(\mathfrak{a})$ 表示 $\mathbf{M}_n(A)$ 由……组成的矩阵中的$\mathfrak{a}$ 中的子集。 这是$\mathbf{M}_n(A)$的双面理想。 我们有$\mathbf{M}_n(\mathfrak{a})A^n=\mathfrak{a}^n= A^n\mathfrak{a}$。 从命题 6 可以得出，$\mathbf{M}_n(A)$ 的每个双面理想都是形式 $\mathbf{M}_n(\mathfrak{a})$，其中 $\mathfrak{a}$ 是 A 的双面理想。

#### 注 {#alg-viii-s6-n4-rem-1 .statement tag=007D}

我们保留上面的假设和记号，并假设$(B,A)_k$双模Q是A-模P的对偶$P^*$，并且同构$\lambda$和$\theta$是典范映射$\Lambda  : P\otimes_BP^*\rightarrow_sA_d$和θ： $P^*\otimes_AP\rightarrow_sB_d$（VIII、p. 101、定理 1）。由于 A-模 P 是射影且有限生成的，因此对于每个 A-模 M，我们有典范同构 $\vartheta_M: P^*\otimes_AM\rightarrow$ Hom$_A(P,M)$（II, §4, No. 2，p. 271，推论）。我们留给读者用替换构造$M\mapsto Q\otimes_AM$和构造$M\mapsto$Hom$_A(P,M)$重新表述小节3和4的结果。

### 5. 有序集 / 子模

在这个小节中，A和B是$k$代数，M是左A-模，V是左B-模。我们用 D(M)（分别为 D(V)）表示 M 的子模的集合（分别为 V），按包含排序。我们假设给定同构或有序集 $\varphi : D(V)\rightarrow D(M)$。

根据 Morita 的定理 (VIII, p. 103, 定理 2)，我们在以下情况下得到这样的同构：P 是可逆的 $(A,B)_k$ 双模，M 是 A-模 $P\otimes_BV$，并且对于每个$V,\varphi (W)$的子模W在M中是$P\otimes_BW$的典范像。

模 M 或其子模的一些属性可以用有序集合 D(M) 的项来表示：它们列在表 I 和 II 中。

模 M 是子模的$(M_i)_{i\in I}$ 家庭的直和当且仅当我们对于每个$i\in I$ 都有$M =\sum_{i\in I}M_i$ 和$M_i\cap \sum_{j\not=i}M_j= 0$。这个注和表I的检查给出了以下结果。

#### 命题 7 {#alg-viii-s6-prop-7 .statement tag=007E}

a) 我们有 $\varphi (0) = 0$ 和 $\varphi (V) = M$。

b) 设$(V_i)_{i\in I}$是V的子模的家庭。我们有

$$
\varphi (\sum_{i\in I}V_i)=\sum_{i\in I}\varphi (V_i),\varphi (\bigcap_{i\in I}V_i)=\bigcap_{i\in I}\varphi (V_i)
$$

子模 M 已订购集合 D(M)

D(M) 零子模最小的元素

子模 M 最大元素 D(M)

$\bigcap_{i\in I}M_i$下确界inf$_{i\in I}M_i$

$\sum_{i\in I}M_i$ 至少上界支持$_{i\in I}M_i$

补子模 inf(M$',M''$) $= 0$，sup(M$',M''$) $= M$

M 的简单子模最小 D(M) 的元素 $-\{0\}$

M 极大子模 D(M) 极大元素 $-\{M\}$

M 的底层 $\mathscr{S}(M)$ 集合的 D(M) 中最少上界

D(M)$-\{0\}$ 的最小元素

集合的 D(M) 中 M 下确界的$*$部首$\mathfrak{R}(M)$

$$
*
$$

D(M)$-\{M\}$极大元素(VIII、p. 151)

表I。

模 M 的性质 D(M) 的性质

M 为诺特。有序集合 D(M) 为诺特 (集合

理论，III, §6, No. 5，p. 190）。

M 为阿廷的。 集合 D(M)，按$\supset$排序，为

诺特。

M 不可分解。我们有 M $\not= 0$，但没有

两个非零元素 $M'$ 和 $M''$

D(中) 满足 inf(中$',M''$) $= 0$,

超级（M$',M''$）$= M$。

M 是有限生成的。对于 D(M) 中的每个家庭 $(M_i)_{i\in I}$

上界 M，存在有限个

子集 J 的 I 使得 M =sup$_{j\in I}M_j$。 M很简单。卡(D(M)) = 2。

M 为半单。 M 是最小上界，在 D(M) 中，

集合至少元素

D(M)$-\{0\}$。

表II。

c) B-模 V 是$(V_i)_{i\in I}$ 家族中子模的直和当且仅当M 是$(\varphi (V_i))_{i\in I}$ 家族中的直和。

设$V'$和$V''$为V的子模，使得$V'$包含在$V''$中； 集合$M'=\varphi (V')$和$M''=\varphi (V'')$，因此$M''$包含于$M'$。用 $[V',V'']$ 表示 V 的子模 W 的 D(V) 由……组成区间，这样我们就有 $V'\subset W\subset V''$，同样，定义也有 D(M) 中的区间 $[M',M'']$。 映射$W\mapsto W/V'$是从$[V',V'']$到$D(V''/V')$的有序集中的同构；我们同样从 $[M',M'']$ 有序集定义同构到 $D(M''/M')$。由于$\varphi$发送间隔$[V',V'']$到$[M',M'']$，所以从$D(V''/V')$到$D(M''/M')$，有序集的定义同构$\varphi$。由此我们推导出以下命题以及表I和II。

#### 命题 8 {#alg-viii-s6-prop-8 .statement tag=007F}

a) 设$V'$和$V''$为V的子模，使得$V''$包含于$V'$。 B-模 $V''/V'$ 是简单的当且仅当 A-模 $\varphi (V'')/\varphi (V')$ 是简单的。

b) 如果$V'$是V的简单子模、极大子模或直因子，则$\varphi (V')$分别是M的简单子模、极大子模或直因子。

c) 将V的同构$\varphi$变换底层$\mathscr{S}(V)$转换为$M*$的底层$\mathscr{S}(M)$以及部首（VIII，p. 151，将V的定义 1)$\mathfrak{R}(V)$转化为M$.*$的部首$\mathfrak{R}(M)$

d) 设 $(V_i)_{0\leqslant i\leqslant n}$ 为有限序列 / 子模 / V。当且仅当 $(\varphi (V_i)_{0\leqslant i\leqslant n})$ 是 M 的 Jordan-Hölder 级数时，它才是 V 的 Jordan–Hölder 级数。

#### 引理 2 {#alg-viii-s6-lem-2 .statement tag=007G}

令H和$H'$为V的子模，使得$H\cap H'= 0$。 B-模 H 和 $H'$ 同构当且仅当 A-模 $\varphi (H)$ 和 $\varphi (H')$ 同构的。

我们认同$H+H'$与乘积$H\times H'$。 同构从H到$H'$的图是V满足的子模$H''$

$$
H\cap H''= H'\cap H''= 0,H + H'= H + H''= H'+ H'' \tag{17}
$$

反之，每一个具有这些性质的子模都是同构从H到$H'$的图。通过命题 7，关系$H\cap H'= 0$相当于$\varphi (H)\cap \varphi (H') = 0$，关系(17)相当于关系

$$
\varphi (H)\cap \varphi (H'') =\varphi (H')\cap \varphi (H'') = 0
$$

$$
\varphi (H) +\varphi (H') =\varphi (H) +\varphi (H'') =\varphi (H') +\varphi (H'')
$$

接下来是引理。

#### 命题 9 {#alg-viii-s6-prop-9 .statement tag=00R6}

设S为V的简单子模，T为M的简单子模$\varphi (S)$。如果$V_S$表示型S的V的同型成分，$M_T$表示型T的M的同型成分，那么我们就有$\varphi (V_S) = M_T$。

V中与S不同的每个简单子模$S'$都满足$S'\cap S = 0$。因此，当且仅当 $\varphi (S')$ 同构于 T (引理 2) 时，它才同构于 S。现在，$V_S$是与S同构的V的简单子模的和，并且$M_T$是与T同构的M的简单子模的和。因此命题9紧随命题7和8。

#### 命题 10 {#alg-viii-s6-prop-10 .statement tag=007H}

a) B-模 V 是阿廷的（分别是诺特，不可分解，简单，有限生成）当且仅当 M 是。

b）B-模V有有限长度当且仅当A-模M有有限长度，然后我们有long$_B(V) =$long$_A(M)$。

c) B-模 V 是半单（分别是同型）当且仅当 A-模 M 是半单（分别是同型）。如果是这种情况，那么我们就有 long$_B(V) =$ long$_A(M)$。

断言 a) 从表 II 中列出的第二个性质开始。

断言 b) 由命题 8, d) 推出。

模 V 是半单当且仅当它等于其底层 $\mathscr{S}(V)$；当且仅当存在 V 的简单子模 S 使得 $V = V_S$ 时，它是同型的。因此，断言 c) 由命题 7, c), 8, c) 和 9 (VIII, p. 106 和 109) 得出。

### 6. 森田对应保留的其他属性

设 A 和 B 为 Morita 等价的 $k$-代数，P 为可逆的 $(A,B)_k$ 双模。

#### 命题 11 {#alg-viii-s6-prop-11 .statement tag=007I}

让

$$
(\mathscr{E})V'-\overset{f}{\rightarrow}V-\overset{g}{\rightarrow}V''
$$

是B-模和B-线性映射的图表，并且令

$$
(P\otimes \mathscr{E})P\otimes_BV'\longrightarrow^{1_P\otimes f}P\otimes_BV\longrightarrow^{1_P\otimes g}P\otimes_BV''
$$

是相应的图表或 A-模。那么$(\mathscr{E})$是正合序列当且仅当$(P\otimes \mathscr{E})$是正合序列。

假设序列 $(\mathscr{E})$ 是精确的。由于右B-模 P 是射影，序列 $(P\otimes \mathscr{E})$ 是精确的（II, §3, No. 6、p. 251、命题 5 和 II, §3, No. 7、p. 257，推论 6）。

相反，假设序列 $(P\otimes \mathscr{E})$ 是精确的。令 Q 为 $(B,A)_k$ 双模，与 P 成逆，且$\theta : Q\otimes_AP\rightarrow_sB_d$ 同构。考虑交换律图表

$Q\otimes_AP\otimes_B{V'}^{1_Q\otimes 1_P\otimes f}/$/ $Q\otimes_AP\otimes_BV^{1_Q\otimes 1_P\otimes g}/$/ $Q\otimes_AP\otimes_BV''$

$\theta \otimes 1_{V'}\theta \otimes 1_V\theta \otimes 1_{V''}$

$V'f$ // V $g$ // $V''$。

由于 Q 是射影 A-模并且序列 $(P\otimes \mathscr{E})$ 是精确的，因此图表的第一行是正合序列。由于垂直箭头是同构，所以第二行也是精确的。

#### 推论{#alg-viii-s6-n6-cor-1 .statement tag=007J}

设$f: V\rightarrow W$为B-线性映射。那么 $f$ 是单射（或满射）当且仅当 $1_P\otimes f$ 是。

#### 命题 12 {#alg-viii-s6-prop-12 .statement tag=007K}

设V为左B-模。 B-模 V 是射影（分别是生成的，忠实，$*$内射，有限呈现）当且仅当

$$
*
$$

A-模$P\otimes_BV$是。

a) 假设 V 是射影的。存在集合 I 使得 V 同构于 $B^{(I)}_s$ 的直因子子模 。那么A-模$P\otimes_BV$同构于$P^{(I)}$的直因子子模；由于 P 是射影 A-模，因此同样适用于 $P\otimes_BV$。

b) 假设B-模V是生成的。令 M 为 A-模。存在 B-模 W 使得 M 与 $P\otimes_BW$ 同构。通过VIII、p. 80的定理 1，存在集合I和满射$\varphi : V^{(I)}\rightarrow W$。根据推论，从 $P\otimes (V^{(I})$ 到 $P\otimes_AW$ 的映射 $1_P\otimes \varphi$ 是满射，从而给出满射 $(P\otimes V)^{(I)}\rightarrow M$。到VIII、p. 80、$P\otimes V$ 中的定理 1 为生成A-模。

c) B-模 V 是忠实的，当且仅当其湮没子减少到 0。 断言 c) 因此从 VIII、p. 105 的例 3 得出。

$*$d) 假设V是单射的。 通过VIII、p. 106、A-模$P\otimes_BV$的注同构于Hom$_B(Q,V)$，其中Q是与A相反的$(B,A)_k$双模。 由于 A-模 Q 是射影，因此平坦（X, §1，n$^o3$，p. 9，例 1），A-模 Hom$_B(Q,V)$ 是 X, §1，n$^o8$，p. 18，命题 11 的内射。

e) 假设 V 承认有限表示 $L_1\rightarrow L_0\rightarrow V\rightarrow 0$ (X, §1, n$^o4$, p. 10)。通过将张量积与 P 结合，我们可以推导出 A-模 $N'_1-\overset{u}{\rightarrow}N'_0\rightarrow P\otimes_BV\rightarrow 0$ 的正合序列，其中 $N'_1$ 和 $N'_0$ 是射影且有限生成的（命题 11 和 a)）。令$N''_0$为有限生成A-模，使得模$N_0= N'_0\oplus N''_0$是自由且有限生成的，并令$u': N'_1\oplus N''_0\rightarrow N_0$为同态$(u,1_{N''_0})$；那么$P\otimes_BV$可以用$u'$的余核来识别。令$N_1$为有限生成的自由A-模和$p: N_1\rightarrow N'_1\oplus N''_0$满同态； 序列 $N_1\longrightarrow^{u'\circ p}N_0\rightarrow P\otimes_BV\rightarrow 0$ 是 A-模 $P\otimes_BV.*$ 的有限表示

f) 假设 A-模 $P\otimes_BV$ 是射影的（分别是生成的，忠实的，$*$内射的，有限呈现的）。到应用以上（交换

$$
*
$$

A和B以及P和Q的角色），我们看到B-模$Q\otimes_AP\otimes_BV$也有这个性质。因而，B-模V也是如此，它与它同构。

#### 推出{#alg-viii-s6-n6-cor-2 .statement tag=007L}

环 A 是左阿廷的（或左诺特的）当且仅当环 B 是。

由于同构介于B的左理想的有序集合和P的A-子模的集合之间，环B是左阿廷的（或左诺特的）当且仅当A-模P是阿廷的（分别为诺特）。然而，到 VIII、p. 101、A-模的定理 1 时，P 为生成的并且是有限生成的；特别是，对于整数$n\geqslant 1$，$A_s$同构于$P^n$的直因子。因而，当且仅当 A 为左阿廷的（或左诺特的）时，P 才为阿廷的（或诺特）。

### 7. 森田等价共代数

#### 命题 13 {#alg-viii-s6-prop-13 .statement tag=007M}

a) 如果两个$k$-代数是森田等价的，则它们的中心是同构的$k$-代数。

b) 两个交换 $k$-代数是 Morita 等价的当且仅当它们是同构的。

c) 两个域的$k$-代数是森田等价的当且仅当它们是同构的。

d) 对于$i= 1,2$，令$A_i$和$B_i$为森田等价的$k$代数和$P_i$可逆的$(A_i,B_i)_k$双模。 集合$A = A_1\otimes_kA_2,B = B_1\otimes_kB_2$和$P = P_1\otimes_kP_2$。 $k$-代数 A 和 B 是 Morita 等价的，P 是可逆的 $(A,B)_k$-双模。

e) 如果 A 和 B 是 Morita 等价的 $k$-代数，且 $k'$ 是可交换的 $k$-代数，则 $k'$-代数 $A_{(k')}$ 和 $B_{(k')}$ 是 Morita 等价的。

断言 a) 由VIII、p. 102 的推论 1 得出，并隐含 b)。

令 K 和 L 为$k$-代数且域，并令 P 为可逆的$(K,L)_k$-双模。右L向量空间P是单模(VIII,p. 104)，因此维数为1，所以$k$-代数End$_L(P)$和L是同构的。从K到End$_L(P)$经过VIII、p. 101、定理1、映射$a\mapsto a_P$是同构。因而，域 K 和 L 在 $k$ 上同构； 断言 c)如下。

在 d) 的假设下，令 $Q_i(i= 1,2)$ 为 $(B_i,A_i)_k$ 双模逆于 $P_i$。用 Q 表示 $(B,A)_k$-双模 $Q_1\otimes_kQ_2$。考虑规范的 $k$-线性同构 $(P_1\otimes_kP_2)\otimes_k(Q_1\otimes_kQ_2)\rightarrow (P_1\otimes_kQ_1)\otimes_k$ $(P_2\otimes_kQ_2)$；当经过为商时，定义态射

$$
(P_1\otimes_kP_2)\otimes_B(Q_1\otimes_kQ_2)\rightarrow (P_1\otimes_{B_1}Q_1)\otimes_k(P_2\otimes_{B_2}Q_2)
$$

即 $(A$, A)-线性。相反，逆同构$(P_1\otimes_kQ_1)\otimes_k(P_2\otimes_k$$Q_2)\rightarrow (P_1\otimes_kP_2)\otimes_k(Q_1\otimes_kQ_2)$定义和$(A$，A)-线性态射$(P_1\otimes_{B_1}$$Q_1)\otimes_k(P_2\otimes_{B_2}Q_2)\rightarrow (P_1\otimes_kP_2)\otimes_B(Q_1\otimes_kQ_2)$。这两个态射互为逆，因此是同构。由于$(A_i,A_i$)-双模$P_i\otimes_{B_i}Q_i$与$A_i$同构的，我们得到$(A$，A)-线性同构$P\otimes_B$$Q\rightarrow A$。我们同样获得$(B$，B)-线性同构$Q\otimes_AP\rightarrow B$，它完成了d)的证明。

在e)的假设下，令P为可逆的$(A,B)_k$双模；那么$P_{(k')}$是可逆的$(A_{(k')},B_{(k')})_{k'}$双模。

设 A 为 $k$ 代数，并令 $e$ 为 A 中的幂等。集合 $eAe$，赋予 A 的 $k$ 的加法、乘法和作用，是$k$-代数与单位元 $e$。

#### 命题 14 {#alg-viii-s6-prop-14 .statement tag=007N}

设 A 和 B 为 $k$-代数。则 A 和 B 是 Morita 等价的当且仅当在 $\mathbf{M}_n(B)$ 满足中存在整数 $n\geqslant 1$ 和平方矩阵 $e= (e_{ij})$ 条件：

(i) 我们有 $e^2=e$。

(ii) 由元素 $e_{ij}$ 生成的 B 的两侧理想等于 B。

(iii) $k$-代数 A 与 $e\mathbf{M}_n(B)e$ 同构的。

如果满足条件 (i) 和 (ii)，则 $(e\mathbf{M}_n(B)e,B)_k$ 双模 $eB^n_d$ 可逆。

鉴于定理 1 (VIII, p. 101)，$k$-代数 A 是 Morita 等价于 B 当且仅当它与有限生成的射影内同态代数同构，并且生成的右B-模。因此，命题由下面的引理3和4得出。

#### 引理 3 {#alg-viii-s6-lem-3 .statement tag=007O}

右B-模 P 是射影的、有限生成的，并且生成的当且仅当存在整数 $n\geqslant 0$ 以及 $\mathbf{M}_n(B)$ 中的幂等 $e= (e_{ij})$ 且具有以下属性：

(i) B-模 P 与 $eB^n_d$ 同构的。

(ii) 由元素 $e_{ij}$ 生成的 B 的两侧理想等于 B。

设 P 为右B-模。那么 P 是射影且有限生成的当且仅当它同构于形式 $B^n_d$ 的 B-模的直因子子模，其中 $n$ 是整数 $\geqslant 0$（II, §2, No. 2，p. 232，推论 1）。如果我们认同$k$-代数$\mathbf{M}_n(B)$和End(B$^n_d$)，那么这意味着$\mathbf{M}_n(B)$中存在幂等$e$，使得P与$eB^n_d$同构的。

当且仅当其理想迹$\tau (P)$等于B，即$\tau (eB^n_d) = B$（VIII，p. 80，定理1）时，B-模P才是生成的。令$x_1, . . . , x_n$为$B^n_d$相应的的元素至矩阵$e$的列，并令$x^*_i$（对于$1\leqslant i\leqslant n$）为$eB^n_d$上的线性形式$(b_1, . . . , b_n)\mapsto b_i$。族$(x_1, . . . , x_n)$生成B-模$eB^n_d$，族$(x^*_1, . . . , x^*_n)$生成是双重的。现在，我们有了$\langle x^*_i, x_j\rangle =e_{ij}$，所以$\tau (eB^n_d)$是由$e_{ij}$生成的B的两侧理想。这就证明了引理3。

#### 引理 4 {#alg-viii-s6-lem-4 .statement tag=007P}

令 V 为 B-模，且 E 自同态 $k$ - V 的代数。令 $e$ 为 V 的投影算子，且 P 像为 $e$。将$v\in eEe$发送到B-模P的自同态$x\mapsto v(x)$的映射是从$eEe$到End$_B(P)$的$k$代数的同构。

将叙述中描述的映射表示为$\varphi :eEe\rightarrow$End$_B(P)$；它是 $k$-代数的同态。让$u\in$结束$_B(P)$。用$x\in V$的$v(x) =u(e(x))$定义的V的$v$自同态表示。我们有$(eve)(x) =$$u(x)$对应$x\in P$，即$\varphi (eve) =u$。因而，$\varphi$是满射的。设$w$为$\varphi$核元素； $w$的限制到核和$e$的像是零，所以$w$是零，这证明$\varphi$是单射的。

#### 例 1 {#alg-viii-s6-n7-exa-1 .statement tag=007Q}

设 A 是一个 $k$ 代数，并且 $e$ 是 A 中的幂等，使得 $AeA = A$。 $k$-代数$eAe$可以与$A_d$(引理4)的子模$eA_d$的自同态$k$-代数识别。由于$AeA = A$，从命题 14 可以得出$eA_d$是可逆的$(eAe,A)_k$双模，因而$k$-代数$eAe$和A是Morita等价的。此外，森田的定理（VIII，p. 103）意味着以下结果：

a) 设 M 和 N 为左A-模。从 M 到 N，从 $eM$ 到 $eN$ 扩展到 A-线性映射的每个 $eAe$ 线性映射都是唯一的。

b) $k$-代数$eAe$上的每个左模同构于形式$eM$的模，其中M是左A-模。

#### 例 2 {#alg-viii-s6-n7-exa-2 .statement tag=007R}

设 A 为 $k$ 代数且 $n\geqslant 1$ 整数。我们认同矩阵代数$\mathbf{M}_n(A)$与内同态代数右A-模$A^n_d$。我们已经看到 A 和 $\mathbf{M}_n(A)$ 是 Morita 等价的。对于每个左A-模 M，认同 $A^n_d\otimes_AM$ 和 $M^n$。 代数 $\mathbf{M}_n(A)$ 然后在 $M^n$ 上有一个左作用，我们有

$$
(a\cdot m)_i=\sum_{j=1}^na_{ij}m_j
$$

对于$\mathbf{M}_n(A)$中的$a= (a_{ij})$和$M^n$中的$m= (m_i)$。森田的定理意味着以下结果：

a) 代数 $\mathbf{M}_n(A)$ 上的每个左模同构于形式 $M^n$ 的模，其中 M 为左A-模。

b) 设 M 为左A-模。 映射$N\mapsto N^n$是双射，从M的A-子模的集合到$\mathbf{M}_n$(A)的集合-$M^n$的子模块。

c) 设 M 和 N 为左A-模。对于A-线性映射$g: M\rightarrow N$，令$g_n$为从$M^n$到$N^n$的映射$(m_i)\mapsto (g(m_i))$。那么从Hom$_A(M,N)$到Hom$_{\mathbf{M}_n(A)}(M^n,N^n)$的映射$g\mapsto g_n$就是双射。

d) 设 M 为左A-模。当且仅当 A-模 M 是时，模$M^n$超过环$\mathbf{M}_n(A)$不可分解（分别为半单，简单，阿廷的，诺特，有限生成）。

#### 例 3 {#alg-viii-s6-n7-exa-3 .statement tag=007S}

设 A 为主理想整环和 L 非零的，有限生成，自由A-模。设B为L的自同态环；则 L 是可逆的 $(A,B)_{\mathbf{Z}}$ 双模，环 A 和 B 是 Morita 等价的。由 Morita 的定理、命题 10、a) (VIII、p. 109) 和结构定理 for 有限生成A-模 (VII, §4, No. 4、p. 19、定理 2)，每个有限生成B-模与$\oplus^m_{i=1}(L/\mathfrak{a}_iL)$同构的，其中$m$是自然数，$\mathfrak{a}_i$是满足、$\mathfrak{a}_1\subset \mathfrak{a}_2\subset  \cdots  \subset \mathfrak{a}_m$和$\mathfrak{a}_m\not= A$的理想； 整数$m$和理想$\mathfrak{a}_i$是唯一确定的。到 VIII、p. 105 的命题 6，B 的每个双面理想都是形式 $dB$，其中 $d$ 是 A 的元素。

### 习题{#alg-viii-s6-exercises}

参见[习题为 § 6](exercises/s6/)。
