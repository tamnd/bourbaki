---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 7
section_title: Vector spaces
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 292-316, 400-409
pdf_pages: 0316-0340, 0424-0433
extraction: ocr
subsections:
    - "no": 1
      title: BASES OF A VECTOR SPACE
      page: 292
      pdf_page: 316
    - "no": 2
      title: DIMENSION OF VECTOR SPACES
      page: 293
      pdf_page: 317
    - "no": 3
      title: DIMENSION AND CODIMENSION OF A SUBSPACE OF A VECTOR SPACE
      page: 295
      pdf_page: 319
    - "no": 4
      title: RANK OF A LINEAR MAPPING
      page: 298
      pdf_page: 322
    - "no": 5
      title: DUAL OF A VECTOR SPACE
      page: 299
      pdf_page: 323
    - "no": 6
      title: LINEAR EQUATIONS IN VECTOR SPACES
      page: 304
      pdf_page: 328
    - "no": 7
      title: TENSOR PRODUCTS OF VECTOR SPACES
      page: 306
      pdf_page: 330
    - "no": 8
      title: RANK OF AN ELEMENT OF A TENSOR PRODUCT
      page: 309
      pdf_page: 333
    - "no": 9
      title: EXTENSION OF SCALARS FOR A VECTOR SPACE
      page: 310
      pdf_page: 334
    - "no": 10
      title: MODULES OVER INTEGRAL DOMAINS
      page: 312
      pdf_page: 336
statements: 87
exercises: 39
content_sha256: 5638396056c6eb8c64d82d6eeff46db28f20e6fb78df9d5ed4c9c8b6c901f094
translated_from: content/en/alg/II/07_s7_vector_spaces.md
translation_method: google
source_content_sha256: 4fff0cdb1537b620d81d2d1d46ed26cb35c156c51e85408f9907b6d12e29297b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: b5c9439cdf9840dd229a0c66c92784ff163c2fc080eab608cf8d7b5cc26f7432
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 7。 向量空间

### 1. 基向量空间

#### 定理 1 {#alg-ii-s7-thm-1 .statement tag=05RI}

每超过域 K 向量空间就是自由K-模。

必须证明每个向量空间都承认基；这可以从以下更精确的定理得出：

#### 定理 2 {#alg-ii-s7-thm-2 .statement tag=05RJ}

给定向量空间 E 的生成的系统 S 在域 K 上，并且 S 中包含 E 的自由子集 L，则存在 E 的基 B，使得 L ⊂ B ⊂ S。

定理 1 由叙述通过取 L = ∅ 得出。

为了证明定理 2，我们注，根据§ 1, no. 11，S中包含的E的自由子集的集合Λ，按包含排序，是归纳集合（集合理论，III, § 2, no. 4）；自由子集包含 L 的集合 M 也包含在 S 中。根据 Zorn 的引理，M 承认极大元素 B，并且足以证明 B 生成的 E 的向量子空间等于 E。这立即从定义得出B 和以下引理：

#### 引理 1 {#alg-ii-s7-lem-1 .statement tag=05RK}

令 (a_i)_{i \in I} 为 E 的元素自由族；如果 b \in E 不是 (a_i) 生成的属于到子空间 F，则 a_i 和 b 的 E 由……组成的子集是空闲的。

假设所有$i \in I$有关系$\mu b + \sum_i \lambda_i a_i = 0$，其中$\mu \in K$和$\lambda_i \in K$，家庭$(\lambda_i)$有有限支撑；如果$\mu \neq 0$，则$b = -\sum_i (\mu^{-1} \lambda_i) a_i$，因此$b \in F$与假设相反；因此$\mu = 0$和关系变成$\sum_i \lambda_i a_i = 0$，这意味着$\lambda_i = 0$对于所有$i \in I$乘以假设； 从而引理。

#### 推论{#alg-ii-s7-n1-cor-1 .statement tag=05RL}

对于子集 B 或向量空间 E，以下属性是等效的：
(a) B 是 E 的基。
(b) B 是 E 的最大自由子集。
(c) B 是 E 的最小生成的系统。
这紧随定理 2。

#### 例 {#alg-ii-s7-n1-exa-1 .statement tag=05RM}

给定 A 的环 A 和子域 K，A 是 K 上的（右或左）向量空间，因此承认基；特别是，域 K 的每个扩张域都有基作为 K 上的左（或右）向量空间。
*因此，实数的域R承认（无限）基作为向量空间超过有理数的域Q；这样的 R 基称为 Hamel 基。*

#### 注 {#alg-ii-s7-n1-rem-1 .statement tag=05RN}

对于$(a_i)_{i \in I}$ 元素向量空间 $E$ 超过域 $K$ 的家庭来说，要*自由*，有充分必要，对于所有$\kappa \in I$、$a_\kappa$ 属于至无$E$的子空间由指标$i \neq \kappa$的$a_i$生成。我们知道这个条件对于任何模都是必要的（§ 1, no. 11，*注*1）。凭借引理 1 就足够了，正如通过*归谬法*立即论证并考虑$(a_i)$的最小相关亚族所见。

### 2.维数向量空间

#### 定理 3 {#alg-ii-s7-thm-3 .statement tag=05RO}

*两个基相同的向量空间* $E$ *超过域* $K$ *是等价的*。

我们首先注，如果$E$承认一个*无限*基$B$，则从§ 1, no. 12，推论2到命题23，$E$的所有其他基等价于$B$。因此，我们可以将注意力集中在$E$具有有限基为$n$元素的情况。我们注，每一个超过$K$的*单生*向量空间，不减少到0，都是一个*简单*$K$-模块（I, § 4, no. 4，定义7），因为它是由它的每个元素$\neq 0$生成的，凭借关系$\mu a = (\mu \lambda)(\lambda^{-1}a)$适用于$\mu \in K$、$\lambda \in K$和$\lambda \neq 0$。因此，如果 $(a_i)_{1 \leq i \leq n}$ 是 $E$ 的基，则 $E = \bigoplus_{i=1}^n Ka_i$ 最大为同构，子空间 $E_k = \bigoplus_{i=1}^\kappa Ka_i$ 为 $0 \leq k \leq n$ 形式 a *Jordan-Hölder 级数* $E$、$E_k/E_{k-1}$与$Ka_k$同构的。在这种情况下，定理 3 紧随 Jordan-Hölder 定理（I, § 4, no. 7，定理 6）。

证明可以独立于Jordan-Hölder 定理给出，通过$n$上的归纳表明，如果$E$承认$n$元素的基，则每隔一个基$B'$有*至多* $n$元素。 命题对于$n = 0$来说是明显的。如果$n \geq 1$、$B'$非空；然后让$a \in B'$。到定理 2 (no. 1) 时，存在 $B$ 的子集 $C$，使得 $\{a\} \cup C$ 是 $E$ 和 $a \notin C$ 的基，因为 $\{a\} \cup B$ 显然是生成的系统 / $E$。由于$B$是$E$的基，$C = B$是不可能的（no. 1，定理2的推论），因此$C$至多有$n - 1$元素。令$V$为由$C$生成的子空间，并由$B' - \{a\}$生成$V'$子空间； $V$和$V'$都是$E$的子空间$Ka$的补充，因此是同构的（§ 1, no. 10，命题13）。由于$V$承认基最多有$n - 1$元素，$B' - \{a\}$最多有$n - 1$元素乘以归纳假设，因此$B'$最多有$n$元素。

#### 定义 1 {#alg-ii-s7-def-1 .statement tag=05RP}

*向量空间* $E$*维数*超过域*$K$，*表示为*$\dim_K E$*或*$[E:K]$（*或简单地*$\dim E$）*是*$E$的基中任何一个的基数。 *如果*$M$*是*$E$的子集，*$M$*的秩*（超过*$K$*），表示为*$\operatorname{rg} M$*或*$\operatorname{rg}_K M$，*是向量的维数子空间属于* $E$ *由* $M$ 生成。

说$E$是有限维的，就等价于说，$E$是*有限长度*和$\dim_K E = \operatorname{long}_K E$的$K$模。

#### 推论{#alg-ii-s7-n2-cor-1 .statement tag=05RQ}

*对于 E 的每个子集 M，M 的秩至多等于暗淡 E。*

如果 V 是 M 生成的 E 的向量子空间，则 V 的 M 包含基 B' (no. 1, 定理 2) 并且由于 B' 是 E 的自由子集，因此它包含在 E 的基 B 中 (no. 1, 定理) 2）；那么 Card(B') $\leq$ Card(B), 从而是推论。

定理 2 和 3 立即暗示以下命题：

#### 命题 1 {#alg-ii-s7-prop-1 .statement tag=05RR}

(i) *对于 K 上的左向量空间为有限维 n，它与 K_s^n 同构是充分必要的。*

(ii) *对于两个向量空间 K_s^m 和 K_s^n 同构（m 和 n 整数 $\geq 0$），m = n 是充分必要的。*

(iii) *在有限维 n 的向量空间 E 中，每个生成的系统至少有n 个元素； E 的生成的系统与 n 元素是 E 的基。*

(iv) *在有限维 n 的向量空间 E 中，每个空闲子集至多有n 个元素；一个自由子集与 n 元素是 E 的基。*

#### 命题 2 {#alg-ii-s7-prop-2 .statement tag=05RS}

*设 (E_t)_{t \in I} 是 K 上的向量空间族。那么*

$$
\dim_K \left( \bigoplus_{t \in I} E_t \right) = \sum_{t \in I} \dim_K E_t.
$$

如果 E_t 被规范地标识为 $E = \bigoplus_{t \in I} E_t$ 的子空间，并且 B_t 是 E_t ($t \in I$) 的基，则 $B = \bigcup_{t \in I} B_t$ 是 E ($§ 1$、no. 11、命题 19) 的基； 从而关系 (1) 因为 B_t 是成对的不相交的。

#### 注 {#alg-ii-s7-n2-rem-1 .statement tag=05RT}

(1) 例可以由模给出，承认两个有限基不具有与元素相同的数 ($§ 1$, 习题 16(c))。然而：

#### 命题 3 {#alg-ii-s7-prop-3 .statement tag=05RU}

*设A为环，使得域D中存在A的同态$\rho$；那么对于每个自由A-模 E，E 的任何两个基都是等价的。*

考虑通过将标量的环扩展到D（$§ 5$，no. 1）而获得的D上的向量空间$\rho^*(E) = D \otimes_A E$，并令$\phi : x \mapsto 1 \otimes x$为E的典范映射到$\rho^*(E)$；如果$(a_\lambda)$是E的基，$(\phi(a_\lambda))$是$\rho^*(E)$的基（$§ 5$，no. 1，命题4）；然后从定理 3 得出命题。

#### 推论{#alg-ii-s7-n2-cor-2 .statement tag=05RV}

*如果A是交换环$\neq 0$且E自由A-模，则E的任意两个基是等价的。*

A 中至少存在一个最大理想 m (I, $§ 8$, no. 6, 定理 1)，且当 A/m 为域时，满足命题 3 中的条件。

#### 注 {#alg-ii-s7-n2-rem-2 .statement tag=05RW}

(2) 当自由A-模 E使得E的任意两个基等价时，E的任意基对A的基数也称为E的*维数*或*秩*，用$\dim_A E$或$\dim E$表示。

(3) 令$A$为环，使得自由$A$模块的任意两个基等价，并令$K$为$A$的子域，使得$A$可被视为$K$上的*左向量空间*限制标量。每个自由$A$-模块$E$类似地可以被视为$K$上的左向量空间，然后从§ 1, no. 13，命题25得出

$$
\dim_K E = \dim_K E \cdot \dim_K A_s.
$$

(4) 在章VIII中，我们将看到环满足的例是命题3的结论，但看不到假设。

### 3. 维数和子空间向量空间的维数

#### 命题 4 {#alg-ii-s7-prop-4 .statement tag=05RX}

*向量空间$E$的每个子空间$F$是$E$的直因子并且*

$$
\dim F + \dim(E/F) = \dim E.
$$

由于向量空间 $E/F$的商为自由模，我们知道（§ 1, no. 11，命题 21）$F$是$E$的直因子； 关系 (3) 是公式 (1) (no. 2) 的特例。

#### 推论 1 {#alg-ii-s7-prop-4-cor-1 .statement tag=05RY}

*If $E, F, G$ are vector spaces over a field $K$, every exact sequence of linear mappings $0 \to E \to F \to G \to 0$ splits.*

这是另一个命题 4 (§ 1, no. 9) 的表达方式。

#### 推论 2 {#alg-ii-s7-prop-4-cor-2 .statement tag=05RZ}

*设$(E_i)_{0 \leq i \leq n}$是向量空间超过域$K$的有限族。如果存在线性映射*中的正合序列

$$
0 \longrightarrow E_0 \xrightarrow{u_0} E_1 \xrightarrow{u_1} E_2 \longrightarrow \cdots \longrightarrow E_{n-1} \xrightarrow{u_{n-1}} E_n \xrightarrow{u_n} 0
$$

*关系*

$$
\sum_{2k+1 \leq n} \dim E_{2k+1} = \sum_{2k \leq n} \dim E_{2k}
$$

*成立，或​​者，如果所有空间都是有限维的，*

$$
\sum_{i=1}^n (-i)^i \dim E_i = 0.
$$

设$I_k = \operatorname{Im}\ u_k = \operatorname{Ker}\ u_{k+1}$为$0 \leq k \leq n-1$；因此 $I_{k+1}$ 与 $E_{k+1}/I_k$ 同构的，因此 (公式 (3)) $\dim I_k + \dim I_{k+1} = \dim E_{k+1}$ 对应于 $0 \leq k \leq n-2$，此外还有 $\dim I_0 = \dim E_0$ 和 $I_{n-1} = E_n$，因此$\dim I_{n-1} = \dim E_n$。 替换$\dim E_i$将其表达式为式(5)两边$\dim I_k$的函数，我们在每一边都得到$\sum_{k=0}^{n-1} \dim I_k$，从而的推论。

#### 推论 3 {#alg-ii-s7-prop-4-cor-3 .statement tag=05S0}

*如果M和N是向量空间E中的两个子空间，那么*

(7) $$
\dim(M + N) + \dim(M \cap N) = \dim M + \dim N.
$$

将推论2应用到正合序列就足够了

$$ 0 \to M \cap N \to M \oplus N \to M + N \to 0 $$

(§ 1, no. 8, 命题 10) 考虑到这一事实

$$
\dim(M \oplus N) = \dim M + \dim N
$$

（no. 2，命题2）。

#### 推论 4 {#alg-ii-s7-prop-4-cor-4 .statement tag=05S1}

*对于向量空间 E 的每子空间 F，$\dim F \leq \dim E$；如果 E 是有限维的，关系 $\dim F = \dim E$ 等价于 $F = E$。*

第一个断言由 (3) 可知；进一步，如果$\dim E$是有限的，关系$\dim F = \dim E$通过(3)隐含$\dim(E/F) = 0$和维数0约化到0的向量空间。

#### 推论 5 {#alg-ii-s7-prop-4-cor-5 .statement tag=05S2}

*如果向量空间 E 是向量子空间的家庭 $(F_i)$ 的和，则*

(8) $$
\dim E \leq \sum_i \dim F_i.
$$

*如果进一步$\dim E$是有限的，则(8)的两侧相等当且仅当E是族$(F_i)$的直和。*

不等式 (8) 由 (3) 得出，并且 E 同构于 $\bigoplus_i F_i$ (§ 1, no. 7, 公式 (28)) 的商。第二个断言是§ 1, no. 10的特例，推论5到命题16，对于(8)两侧的等式意味着$\dim F_i = 0$，除了指标的有限数。

#### 定义 2 {#alg-ii-s7-def-2 .statement tag=05S3}

*给定向量空间 E，E 的子空间 F 的余维（相对于 E），用 $\operatorname{codim}_E F$ 表示，或简称为 $\operatorname{codim} F$，是 $E/F$ 的维数（等于 E 中 F 的任何补充的余维）。*

关系 (3) 则可写成

(9) $$
\dim F + \operatorname{codim} F = \dim E.
$$

#### 命题 5 {#alg-ii-s7-prop-5 .statement tag=05S4}

*令F，F'为向量空间E中的两个子空间，使得$F \subset F'$。然后$\operatorname{codim}_E F' \leq \operatorname{codim}_E F \leq \dim E$。如果 $\operatorname{codim}_E F$ 是有限的，关系 $\operatorname{codim}_E F' = \operatorname{codim}_E F$ 意味着 $F = F'$。*

不等式 $\operatorname{codim}_E F \leq \dim E$ 从 (9) 中显而易见，并且如果 $\dim E$ 是有限的关系 $\operatorname{codim}_E F = \dim E$ 意味着$\dim F = 0$，因此$F = \{0\}$。由此得出命题的余数，对于
$$
\operatorname{codim}_E F' = \operatorname{codim}_{E/F'}(F'/F),
$$
因为 $E/F'$ 与 $(E/F)/(F'/F)$ (I, § 4, no. 7, 定理 4) 是标准同构的。

#### 命题 6 {#alg-ii-s7-prop-6 .statement tag=05S5}

*如果M和N是向量空间E中的两个子空间，那么*
$$
\operatorname{codim}(M + N) + \operatorname{codim}(M \cap N) = \operatorname{codim} M + \operatorname{codim} N.
$$
(10)
只要应用命题 4 的推论2 到正合序列就足够了
$$
0 \to E/(M \cap N) \to (E/M) \oplus (E/N) \to E/(M + N) \to 0
$$
（§ 1, no. 7、命题 10）并使用 no. 2、命题 2。

注如果E是有限维的，则(10)是(7)和(9)的推论。

#### 命题 7 {#alg-ii-s7-prop-7 .statement tag=05S6}

*如果$(F_i)$是子空间的向量空间E的有限族，那么*
$$
\operatorname{codim}\left(\bigcap_i F_i\right) \leq \sum_i \operatorname{codim} F_i.
$$
如果$F = \bigcap_i F_i$，$E/F$同构于$E/F_i$的直和的子空间(§ 1, no. 7，公式(27))。

向量子空间 / 维数 1（或维数 2）或向量空间 E 通常称为*线经过到 0*（或*平面经过到 0*）（或简称为*线*（或*平面*）如果不产生混淆（cf.§ 9, no. 3）），与经典几何语言类比；如果 E 的子空间的余维为 1，则称为 *超平面经过到 0*（或简称为 *超平面*）。超平面也可以定义为集合 $\mathscr{S}$ 的*极大* 元素 E *与 E 不同*的向量子空间，按包含排序。 E 包含子空间 H 的子空间与 $E/H$ 的子空间之间存在一一对应的对应 (I, § 4, no. 7, 定理 4)；如果 E 为维数 $\geq 1$，$\mathscr{S}$ 非空，并且说 H 在 $\mathscr{S}$ 中最大意味着 $E/H$ 包含没有子空间与 $\{0\}$ 和 $E/H$ 不同，这意味着$E/H$由其任何元素$\neq 0$生成，在其他字中它是维数1。

在有限维 $n \geq 1$ 中的向量空间中，超平面是维数* $n - 1$ 中的子空间 * 公式 (3)。

#### 命题 8 {#alg-ii-s7-prop-8 .statement tag=05S7}

*在向量空间 E 和域 K 中，每个向量子空间 F 是超平面的交，其中包含它。*

只要证明对于所有 $x \notin F$ 都存在超平面 H 包含 F 而不是包含 x。通过假设 $F \cap Kx = \{0\}$，因此 F 和 $Kx$ 的和 M 是直接的。设N是E中M的补充；那么E是$H = F + N$和$Kx$的直和，因此H是超平面和所需性质。

#### 注 {#alg-ii-s7-n3-rem-1 .statement tag=05S8}

大多数属性都在这方面得到了证明。对于向量空间的子空间 ，对于定义了维数 ($§ 2,$ no. 7, 注 2) 的自由模的子模不成立。 *对于例，交换环的理想不一定承认基，因为存在整环$A$，其中某些理想不是主要的（VII，$§ 1,$no. 1）以及其中任何两个元素环是线性相关的（$§ 1,$ no. 11，注 1）。* 自由 $A$ 模块的子模 $E$ 可能是免费的，与 $E$ 不同，并且具有与维数相同的维数 $E$，如整环$A$中的主要理想所示；同样的例还证明，自由$A$模块的自由子模不一定承认补充。

### 4.秩线性映射

#### 定义 3 {#alg-ii-s7-def-3 .statement tag=05S9}

*设$E, F$是向量空间除域$K$。对于$E$的每个线性映射$u$到$F$，$F$的子空间$u(E)$的维数称为$u$的秩，并用$\mathrm{rg}(u)$表示。

若 $N = \mathrm{Ker}(u)$, $E/N$ 同构于 $u(E)$, 从而关系
$$
\mathrm{rg}(u) = \mathrm{codim}_E(\mathrm{Ker}(u))
$$
因此
$$
\mathrm{rg}(u) + \dim(\mathrm{Ker}(u)) = \dim E.
$$
此外，通过公式 (3)
$$
\mathrm{rg}(u) + \dim(\mathrm{Coker}(u)) = \dim F.
$$

#### 命题 9 {#alg-ii-s7-prop-9 .statement tag=05SA}

*令$E, F$是域$K$和$u : E \to F$线性映射的两倍向量空间。*
（一）$\mathrm{rg}(u) \leq \inf(\dim E, \dim F)$。
(ii) *假设$E$是有限维的；在阶和 $\mathrm{rg}(u) = \dim E$ 中，$u$ 是单射的必要且充分。*
(iii) *假设$F$是有限维的；在阶和 $\mathrm{rg}(u) = \dim F$ 中，$u$ 是满射是必要且充分的。*

这紧随关系 (12) 和 (13) 而来。

#### 推论{#alg-ii-s7-n4-cor-1 .statement tag=05SB}

*令$E$为有限维$n$中的向量空间和$E$中的$u$自同态。以下属性是等效的：*
(a) $u$ 是双射；
(b) $u$ 是单射的；
(c) $u$ 是满射；
(d) $u$ 是右可逆的；
(e) $u$ 是可逆的；
(f) $u$ 为秩 $n$。

如果 E 是无限维向量空间，则 E 的单射（或满射）自同态不是双射 (习题 9)。

设 K、K' 是两个域、$\sigma : K \to K'$ 一个 K 的 *同构的* 到 K'、E 向量 K 空间、E' 向量 K' 空间和 $u : K \to K'$ 相对于 $\sigma$ (§ 1, no. 13) 的 *半线性* 映射； E'的子空间$u(E)$的维数又称为$u$的*秩*。它也被认为是 $u$ 的秩被视为 E 到 $\sigma_*(E')$ 的线性映射，对于 $u(E)$ 的每个基也是 $\sigma_*(u(E))$ 的基。

### 5.双向量空间

#### 定理 4 {#alg-ii-s7-thm-4 .statement tag=05SC}

向量空间* E *的对偶* $E^*$ *的维数至少等于* E 的维数。 *对于* $E^*$ *是有限维的，* E * 是这样的充分必要条件，然后* $\dim E^* = \dim E$。

如果 K 是 E 标量的域，则 E 同构于空间 $K_s^{(I)}$，因此 $E^*$ 同构于 $K_d^I$ (§ 2, no. 6, 命题 10)。由于$K_s^{(I)}$是$K_d^I$、$\dim E = \mathrm{Card}(I) \leq \dim E^*$的子空间（no. 3，推论4到命题4）；此外，如果 I 是有限的，则 $K_d^I = K_d^{(I)}$ (cf. 习题 3(d))。

#### 推论{#alg-ii-s7-n5-cor-1 .statement tag=05SD}

*对于向量空间* E，*关系* $E = \{0\}$ *和* $E^* = \{0\}$ *是等价的*。

#### 定理 5 {#alg-ii-s7-thm-5 .statement tag=05SE}

*给定向量空间中的两个正合序列 （在相同的域* K* 上）和线性映射*
$$
\begin{align*}
0 &\to E' \to E \to E'' \to 0 \\
0 &\to F' \to F \to F'' \to 0
\end{align*}
$$
*和两个向量空间* G，H *超过* K，*相应的序列*
$$
\begin{align*}
0 &\to \mathrm{Hom}(E'', G) \to \mathrm{Hom}(E, G) \to \mathrm{Hom}(E', G) \to 0 \\
0 &\to \mathrm{Hom}(H, F') \to \mathrm{Hom}(H, F) \to \mathrm{Hom}(H, F'') \to 0
\end{align*}
$$
*准确且分裂的*。

这是因为每个向量子空间都是直因子（no. 3，命题4）以及§ 2, no. 1，命题1和2。

#### 推论{#alg-ii-s7-n5-cor-2 .statement tag=05SF}

*每正合序列*
$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$
* 向量空间超过相同的域* K * 和线性映射序列*
$$
0 \longrightarrow E''* \xrightarrow{t_v} E^* \xrightarrow{t_u} {E'}^* \longrightarrow 0
$$
*准确且分裂的*。

特别是，对于 E 典范同态 $E^*/M' \to M^*$ 的每个向量子空间 M，其中 $M'$ 是与 M (§ 2, no. 4) 正交的 $E^*$ 的子空间，是*双射*。

#### 定理 6 {#alg-ii-s7-thm-6 .statement tag=05SG}

*对于向量空间 E 超过域 K，典范映射 $c_E : E \to E^{**}$ (§ 2, no. 7) 是单射的；要使其成为双射，E 必须是有限维的。*

第一个断言以及如果E是有限维的$c_E$是双射的事实是§ 2, no. 7、命题14的特殊情况。假设E是无限维的，因此我们可以假设$E = K_s^{(L)}$，其中L是无限集合，因此是$E^* = K_d^L$。令$(e_\lambda)_{\lambda \in L}$为E的典范基，并令$(e_\lambda^*)_{\lambda \in L}$为$E^*$（§ 2, no. 6）中形式坐标族的相应的；由$e_\lambda^*$生成的$E^*$的向量子空间正好是直和$F' = K_d^{(L)}$，而假设L无限意味着$F' \neq E^*$。那么存在 $E^*$ 包含于 $F'$ (no. 3, 命题 8) 的超平面 $H'$，且由于 $E^*/H'$ 非零，其对偶也非零（定理 4 的推论），可通过$E^{**}$ 中$H'$ 的正交$H''$（§ 2, no. 6，命题 9 的推论）。但$H'' \cap c_E(E)$包含在E中$F'$正交的$c_E$下的像中，即定义 0；因此$c_E(E) = E^{**}$是不可能的。

E 通常被*识别*为 $E^{**}$ 的子空间像 $c_E$。

令 E、F 为域 K 和 $u : E \to F$ 线性映射之二向量空间。我们将定义 *典范同构*：

(1) *Im(u) = u(E) 的对偶到 Im($^t u$) = $^t u(F^*)$.*

(2) *Ker(u) = $^{-1}u(0)$ 的对偶到 Coker($^t u$) = $E^*/^t u(F^*)$.*

(3) *Coker(u) = F/u(E) 的对偶到 Ker($^t u$) = $^t u^{-1}(0)$.*

我们写 I = Im(u), N = Ker(u), C = Coker(u); 正合序列起

(14) $0 \to N \to E \xrightarrow{p} I \to 0,\quad 0 \to I \xrightarrow{j} F \to C \to 0$

我们通过转置（定理 5 的推论）得出正合序列

(15)
$$
\begin{array}{ccccccccc}
0 & \to & I^* & \xrightarrow{^t p} & E^* & \to & N^* & \to & 0, \\
0 & \to & C^* & \to & F^* & \xrightarrow{^t j} & I^* & \to & 0.
\end{array}
$$

此外，如$u = j \circ p,\ ^t u = ^t p \circ ^t j$； 正合序列 (15) 因此 $C^*$ 的定义典范同构到 Ker($^t u$)，$I^*$ 到 Im($^t u$) 以及 $N^*$ 到 Coker($^t u$)，因为 $^t p$ 是单射和 $^t j$ 满射。准确地说，让$y \in \mathrm{Im}(u)$，$z \in \mathrm{Ker}(u)$，$t \in \mathrm{Coker}(u)$，$y' \subset \mathrm{Im}(^t u)$，$z' \in \mathrm{Coker}(^t u)$，$t' \in \mathrm{Ker}(^t u)$；当$y'$、$z'$、$t'$分别在$\mathrm{Im}(u)$、$\mathrm{Ker}(u)$和$\mathrm{Coker}(u)$上被规范地标识为线性形式时，则

(16) $\langle y, y' \rangle = \langle x, y' \rangle$ 对于所有 $x \in E$ 使得 $u(x) = y$；

(17) $\langle z, z' \rangle = \langle z, x^* \rangle$ 对于所有 $x^* \in E^*$ 其类 mod。 $^t u(F)$等于$z'$；

(18) $\langle t, t' \rangle = \langle s, t' \rangle$ 对于所有 $s \in F$ 其类 mod。 $u(E)$等于$t$。

我们特别从这些结果中得出：

#### 命题 10 {#alg-ii-s7-prop-10 .statement tag=05SH}

*设 E、F 是两个向量空间在相同的域 K 和 u 上：E \to F 线性映射。*

(i) *为了使 u 是单射（或满射），$^t u$ 是满射（或单射）是必要且充分的。*

(ii) $\operatorname{rg}(u) \leq \operatorname{rg}(^t u)$ 和$\operatorname{rg}(u) = \operatorname{rg}(^t u)$，如果 $\operatorname{rg}(u)$ 是有限的。

第二个断言由上式和定理 4 得出。

#### 定理 7 {#alg-ii-s7-thm-7 .statement tag=05SI}

*设 E 为域 K 上的向量空间，E 的 F 子空间，F' 为 E* 中 F 的正交。*

(i) $\dim F' \geq \operatorname{codim}_E F;$ $\dim F'$ 有限，$\operatorname{codim}_E F$ 有限，然后$\dim F' = \operatorname{codim}_E F$ 是充分必要的。

(ii) *E 中 F' 的正交等于 F。*

(iii) *E* 的每个有限维子空间 G' 都是 E 的某个子空间的正交，必然等于 E 中的 G' 与有限余维的正交。*

(i) 我们知道 F' 同构于对偶 (E/F)*（§ 2, no. 6，命题 9 的推论），因此断言由定理 4 得出，从 $\dim(E/F) = \operatorname{codim}_E F$ 到定义。

(ii) 令 $F_1$ 为 E 中 F' 的正交；显然$F \subset F_1$且$F_1$的正交$F'_1$等于F'（§ 2, no. 4）；因此，$E/F \to E/F_1$ 的规范线性映射 $(E/F_1)^* \to (E/F)^*$、转置是双射的（§ 2, no. 6，命题 10 的推论）；然后从命题 10 可以得出典范映射 $E/F \to E/F_1$ 是双射的，这意味着 $F_1 = F$。

(iii) 令G'为有限维$p$的E*的子空间，并令F为其在E中的正交；然后$\operatorname{codim}_E F \leq \dim G'$。例如，如果$(a_i^*)_{1 \leq i \leq p}$是G'的基，则F是从E到$K_s^p$的线性映射$x \mapsto (\langle x, a_i^* \rangle)$的核，其中秩至多$p$（no. 4，命题9）， 从而结论（no. 4）。然后令F'为F在E*中的正交；从 (i) 可以得出 $\dim F' \leq \dim G'$；但另一方面显然$G' \subset F'$，从而$F' = G'$（§ 2, no. 3，推论4到命题4）。

#### 注 {#alg-ii-s7-n5-rem-1 .statement tag=05SJ}

E* 的无限维子空间 G' 不一定是 E 的子空间的正交，在其他字中，如果 F 是 E 中 G' 的正交，则 E* 中 F 的正交 F' 可能与 G' 不同 (习题 20(b))。†

† 通过给出 E 和 E* 合适的拓扑，并且仅考虑 E 和 E* 子空间相对于这些拓扑闭合，当 E 是无限维时（cf. 拓扑向量空间，II, § 6），可以在 E 和 E* 的属性之间重新建立完美的对称性。

#### 推论 1 {#alg-ii-s7-thm-7-cor-1 .statement tag=05SK}

令 $(x_i^*)_{1 \leq i \leq p}$ 为 E 上线性形式的有限序列，并令 F 为 x 的 E 由……组成的子空间，使得

$$
\langle x, x_i^* \rangle = 0 \quad \text{for } 1 \leq i \leq p.
$$

那么$\operatorname{codim}_E F$等于$x_i^*$的集合的秩，并且E上的每个线性形式（即F上的零）都是$x_i^*$的线性组合。那么$\operatorname{codim}_E F \leq p$和阶中的$\operatorname{codim}_E F = p$，$x_i^*$线性无关是充分必要的。

$x_i^*$的线性组合的集合$G'$是$E^*$的子空间，并且F是E中$G'$的正交，因此$\operatorname{codim}_E F = \dim G'$乘以定理7；进一步$\dim G' \leq p$和关系$\dim G' = p$意味着$(x_i^*)$是免费的系统（no. 2，命题1）；由此得出推论。

#### 推论 2 {#alg-ii-s7-thm-7-cor-2 .statement tag=05SL}

(i) *设*$(x_i^*)_{1 \leq i \leq p}$*为*E上的线性形式有限序列。*对于*$(x_i^*)$*为自由的系统，存在*E*的元素*序列*$(x_i)_{1 \leq i \leq p}$*是充分必要的那*$\langle x_i, x_j^* \rangle = \delta_{ij}$*（克罗内克指标）*。

(ii) *设* $(x_i)_{1 \leq i \leq p}$ *为* E 的元素有限序列。 *对于*$(x_i)$*成为自由的系统，在*E*上存在序列*$(x_i^*)_{1 \leq i \leq p}$*的线性形式*使得*$\langle x_i, x_j^* \rangle = \delta_{ij}$是必要且充分的。

显然，(ii) 由 (i) 得出，通过将 E 视为通过 $c_E$ (定理 6) 与$E^{**}$ 的子空间来确定。设$G'$为由$x_i^*$生成的$E^*$的子空间，且F与E正交； E/F 和 $G'$ 都可以与另一个的对偶进行规范地识别；如果族$(x_i^*)$空闲，则E/F基$(\dot{x}_i)$存在$(x_i^*)$的对偶，并且类$\dot{x}_i$的每个代表系统$(x_i)$都具有所需的属性。相反，系统 $(x_i)$ 的存在使得 $\langle x_i, x_j^* \rangle = \delta_{ij}$ 意味着对于与 K 正交的 $E^*$ 的所有$i$ 子空间，$x_i$ 包含指标的$x_j^*$ $j \neq i$ 但不包括包含 $x_i^*$，因此系统 $(x_i^*)_{1 \leq i \leq p}$ 是免费的。

#### 推论 3 {#alg-ii-s7-thm-7-cor-3 .statement tag=05SM}

*设 S 为 S 的映射的右向量 K 空间* $K_d^S$ *到 K* 的集合和 V 向量子空间。 *在阶*$\dim V \geq p$*（其中p是整数）*，*存在S的p元素*$s_i$*和V*$(1 \leq i \leq p)$*的p元素*$f_i$*使得*$f_i(s_j) = \delta_{ij}$是必要且充分的。

对于$s \in S$和$f \in K_s^S$，空间$K_d^S$被规范地识别为$E = K_d^{(S)}$和$f(s) = \langle e_s, f \rangle$的对偶，$(e_s)_{s \in S}$是E的典范基。 推论 2 表明条件是足够的。 反之，假设$\dim V \geq p$，则维数$p$的V存在子空间$G'$；设F是E中$G'$的正交，因此$\dim(E/F) = p$。 It follows from no. 1, Theorem 2 that there exist $p$ elements $s_i \in S$ such that the $e_{s_i}$ $(1 \leq i \leq p)$ form a basis of a supplement F of E (applying Theorem 2 (no. 1) to a free subset consisting of a basis of E and the generating system the union of this free subset and the canonical basis of E); we then take the $f_i$ to be the elements of a basis of G' dual to the basis of E/F consisting of the classes of the $e_{s_i}$ mod. F。

#### 推论 4 {#alg-ii-s7-thm-7-cor-4 .statement tag=05SN}

*设E为向量空间且M、N有限余维E的两个子空间；如果M'、N'是E*中M和N的正交，则E*中M∩N的正交为M'+N'。

由于 M（分别 N）是 E (定理 7) 中 M'（分别 N'）的正交，M ∩ N 是 E 中 M' + N' 的正交，因此 M' + N' 是 E* (定理 7 (iii)) 中 M ∩ N 的正交。

#### 推论 5 {#alg-ii-s7-thm-7-cor-5 .statement tag=05SO}

*令 E 为有限维 n 中的向量空间。对于维数 p 的 E 的每个子空间 F，E* 中 F 的正交 F' 为维数 n − p。对于维数 q 的 E* 的每个子空间 G'，E 中 G' 的正交 G 是维数 n − q，并且 G' 是 E* 中 G 的正交。

定理 7 给出 E 中 *超平面* 的另一个刻画：

#### 命题 11 {#alg-ii-s7-prop-11 .statement tag=05SP}

*对于向量空间 E 中的每个超平面 H，E 上都存在线性形式 $x_0^*$，使得 H = $x_0^{*-1}(0)$。给定这样的形式 $x_0^*$，对于 E 上的线性形式 $x^*$ 到满足 H = $x^{*-1}(0)$，$x^* = x_0^* \alpha$ 是充分必要的，其中 $\alpha$ 是一个标量 ≠ 0。相反，对于每个线性形式 E 上的 $x^* \neq 0$，子空间 $x^{*-1}(0)$ 是 E 的超平面。*

这个叙述仅表示余维1的E的子空间和维数1的E*的子空间表示定理7。

如果 H 为超平面且 $x_0^*$ 线性形式，则 H = $x^{*-1}(0)$，关系

$$
\langle x, x_0^* \rangle = 0
$$

表征元素$x \in H$，称为*H*方程。

更一般地，如果$(x_i^*)$是E和F上线性形式的族，表示超平面$x_i^{*-1}(0)$的向量子空间交，关系“对于所有$i, \langle x, x_i^* \rangle = 0$”表征F的元素； 关系

$$
\langle x, x_i^* \rangle = 0 \quad \text{for all } i
$$

子空间 F 的方程组* 形式 *系统。 定理 7 (ii) 表示*E 的每一个向量子空间都可以由方程组的系统定义*。

定理 7 (i) 和 (ii) 此外证明*有限*余维 $p$ 的子空间 F 可以由 $p$ 方程的系统定义

(19)
$$
\langle x, x_i^* \rangle = 0, \quad 1 \leq i \leq p,
$$

其中形式 $x_i^*$ *线性独立*。相反，推论1至定理7表明，由$p$方程(19)的系统定义的子空间F具有余维$\leq p$，并且当且仅当$x_i^*$线性无关时，它具有余维$p$；等同于说F不能由方程(19)的至多$p - 1$中的系统由……组成定义。

### 6. 向量空间中的线性方程

#### 命题 12 {#alg-ii-s7-prop-12 .statement tag=05SQ}

令 E、F 为域 K 和 $u : E \to F$ 线性映射上的两个向量空间。对于线性方程

$$
u(x) = y_0
$$

为了具有至少一个解$x \in E$，$y_0$与转置映射${}^t u$中的核正交是必要且充分的。

$F^*$ 中$u(E)$ 的正交为 ${}^t u^{-1}(0)$（§ 2, no. 5，命题 8 的推论），因此 F 中${}^t u^{-1}(0)$ 的正交为 $u(E)$（no. 5，定理 7 (ii)）。

我们将得到一个更方便的标量线性方程系统判据

$$
\langle x, x_i^* \rangle = \eta_i \quad (i \in I)
$$

其中未知的$x$在向量空间E中在域K上取其值，$x_i^*$是E上的线性形式以及K的右侧$\eta_i$元素。

如果我们考虑 E 的基 $(a_\lambda)_{\lambda \in L}$，系统 (21) 等价于方程的系统

$$
\sum_{\lambda \in L} \xi_\lambda \langle a_\lambda, x_i^* \rangle = \eta_i \quad (i \in I)
$$

(22)的$x = \sum_{\lambda \in L} \xi_\lambda a_\lambda$、解是有限支撑的K的元素的必然族$(\xi_\lambda)$。

#### 定义 4 {#alg-ii-s7-def-4 .statement tag=05SR}

由族$(x_i^*)$生成的$E^*$子空间维数称为系统秩(21)。

#### 命题 13 {#alg-ii-s7-prop-13 .statement tag=05SS}

为了使系统(21)为有限秩r，E到$K_s^I$的线性映射$u : x \mapsto (\langle x, x_i^* \rangle)$为秩r是必要且充分的。

如果F'是$x_i^*$生成的$E^*$的子空间，则u的核就是E中F'的正交F；如果 F' 为维数 r，则 F 为余维 r，反之亦然 (no. 5, 定理 7) 和 $\mathrm{rg}(u) = \mathrm{codim}_E F$ (no. 4, 公式 (11))。

#### 定理 8 {#alg-ii-s7-thm-8 .statement tag=05ST}

让

$$
\langle x, x_i^* \rangle = \eta_i \quad (i \in I)
$$

是向量空间 E 上域 K 上的标量线性方程的系统。为了使该系统至少有一个解，有必要对于有限支撑的标量的每个族 $(\rho_i)$ 使得 $\sum_i x_i^* \rho_i = 0,\ \sum_i \eta_i \rho_i = 0.$ *如果秩系统(21)是有限的，这个条件也足够了。*

条件显然是必要的。它表示，如果$F'$是$(x_i^*)$族生成的$E^*$的子空间，则存在线性映射$f : F' \to K_d$，使得所有$i \in I$都有$f(x_i^*) = \eta_i$。如果$F'$是有限维$r$，则$F'$是余维$r$（no. 5，定理7）的$E$的子空间$F$与$F'$的正交被识别为$E/F$的对偶（§ 2, no. 6，命题9的推论）；因此，$f$ 是双数 $(E/F)**$ 的元素。由于$E/F$是有限维的，因此存在且仅一个元素$y \in E/F$，使得$f(x^*) = \langle y, x^* \rangle$对于所有$x^* \in F'$（no. 5，定理6）。 (21) 的解就是$x \in E$，其$E/F$ 中的典范像是$y$。

#### 注 {#alg-ii-s7-n6-rem-1 .statement tag=05SU}

当系统 (21) 的秩是*无穷大*时，定理 8 的条件就不再足够了。对于例，假设$x_i^*$是空间$E = K_s^{(I)}$上的*坐标形式*，$I$是无限的（§ 2, no. 6）；由于$x_i^*$是线性独立的，定理8的条件对于每个家庭$(\eta_i)$都成立，但是如果家庭$(\eta_i)$有有限支撑，系统(21)只有解。

如果系统 (21) 只有*有限数个方程*，并且它的秩 *至多等于* 数方程 (no. 2, 命题 1)，则它始终为有限秩。类似地，如果 $E$ 为有限维 $n$（对于系统 (22) 对应，只有*有限数 n 个未知数*），其对偶 $E^*$ 为维数 $n$，因此系统 (21) 的秩至多等于 $n$（no. 3，推出 4 到命题 4）。由此我们推论：

#### 推出 1 {#alg-ii-s7-thm-8-cor-1 .statement tag=05SV}

*向量空间中的标量线性方程的系统，左手边线性独立形式的有限方程数的由……组成，总是承认解。*

#### 推出 2 {#alg-ii-s7-thm-8-cor-2 .statement tag=05SW}

*对于系数在域 $K$ 的 n 个未知数的齐次线性方程系统 (22)，要承认 $K$ 的元素的非平凡解由……组成，其秩 < 是充分必要的名词*

如果方程的数是有限的并且 < n，情况总是如此。

#### 推出 3 {#alg-ii-s7-thm-8-cor-3 .statement tag=05SX}

*对于 n 个未知数的 n 个方程的域 $K$、由……组成中系数和右侧的线性系统 (22)，要在 $K$ 的元素中拥有且仅有一个解由……组成，有必要且足以保证关联的齐次系统没有非平凡的解*（或者，相当于相同，这个系统的左侧是*线性独立的形式*）。

### 7. 张量积向量空间

与自由或投射模相关的§§ 3、4和5的结果特别适用于向量空间，并给出以下属性：

#### 命题 14 {#alg-ii-s7-prop-14 .statement tag=05SY}

*给出正合序列*

(23)
$$
0 \to E' \to E \to E'' \to 0
$$
*右向量空间超过域K和线性映射和左向量空间F超过K，$\mathbf{Z}$线性映射的相应的序列*
$$
0 \to E' \otimes_K F \to E \otimes_K F \to E'' \otimes_K F \to 0
$$
*准确且分裂的*。

作为序列 (23) 分裂的，这是 § 3, no. 7、推出 5 到命题 7 和 § 3, no. 6、命题 5 的特例。

由于命题 14，当 $E'$ 为 $E$、$j : E' \to E$ 典范嵌入的向量子空间时，$E' \otimes_K F$ 通常被*标识*为*子-$\mathbf{Z}$*-模块$E \otimes_K F$通过单射$j \otimes 1_F$。有了这个约定：

#### 推出{#alg-ii-s7-n7-cor-1 .statement tag=05SZ}

*设K为域，E右向量空间超过K，F左向量空间超过K，$(M_\alpha)_{\alpha \in A}$E的向量子空间的族和$(N_\beta)_{\beta \in B}$F的向量子空间的族。则*
$$
\left( \bigcap_{\alpha \in A} M_\alpha \right) \otimes_K \left( \bigcap_{\beta \in B} N_\beta \right) = \bigcap_{(\alpha, \beta) \in A \times B} (M_\alpha \otimes_K N_\beta).
$$

显然足以证明具体情况
$$
\left( \bigcap_{\alpha \in A} M_\alpha \right) \otimes_K F = \bigcap_{\alpha \in A} (M_\alpha \otimes_K F).
$$

显然，(25) 的左侧包含在右侧中。为了证明逆命题，我们考虑F的基$(f_\lambda)_{\lambda \in L}$。$E \otimes_K F$的每个元素都可以在形式$\sum_{\lambda \in L} x_\lambda \otimes f_\lambda$中唯一表达，其中$x_\lambda \in E$（§ 3, no. 7，推论1到命题7）；如果$E'$是E的向量子空间，对于所有$\lambda \in L$，关系$\sum_{\lambda \in L} x_\lambda \otimes f_\lambda \in E' \otimes_K F$等价于命题14，到$x_\lambda \in E'$。因此，对于每个$M_\alpha \otimes_K F$来说，$\sum_{\lambda \in L} x_\lambda \otimes f_\lambda$属于意味着对于所有$\lambda \in L$和所有$\alpha \in A$、$x_\lambda \in M_\alpha$，即对于所有$\lambda \in L$来说$x_\lambda \in \bigcap_{\alpha \in A} M_\alpha$，这证明(25)的右侧包含在左侧。

#### 命题 15 {#alg-ii-s7-prop-15 .statement tag=05T0}

*如果$(E_\lambda)_{\lambda \in L}$是右向量空间超过域K的家庭，并且$(F_\mu)_{\mu \in M}$是左向量空间超过K的家庭，则典范映射*
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K \left( \prod_{\mu \in M} F_\mu \right) \to \prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_K F_\mu)
$$
*(§ 3, no. 7, 公式 (22)) 是单射的。*

我们写$F = \prod_{\mu \in M} F_\mu$； 映射 (26) 是合成 / 典范映射
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K F \to \prod_{\lambda \in L} (E_\lambda \otimes_K F)
$$
和
$$
\prod_{\lambda \in L} (E_\lambda \otimes_K F) \to \prod_{\lambda \in L} \left( \prod_{\mu \in M} (E_\lambda \otimes_K F_\mu) \right);
$$
因为$F$和$E_\lambda$比向量空间大于$K$，所以约化到§ 3, no. 7，推论3到命题7。

当命题 15 中的条件满足时，张量积
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K \left( \prod_{\mu \in M} F_\mu \right)
$$
通常用它的典范像来识别
$$
\prod_{\lambda, \mu} (E_\lambda \otimes_K F_\mu).
$$
有了这个约定：

#### 推论{#alg-ii-s7-n7-cor-2 .statement tag=05T1}

*令 $F$ 大于$K$ 左向量空间；对于每个集合$X$，左向量空间$K_d^X \otimes_K F$被识别为$X$的所有映射中的空间$F^X$的子空间到$F$，由……组成映射 $u$，使得 $u(X)$ 是 $F$ 中的有限秩。*

如果$(f_\lambda)$是$F$的基，则$K_d^X \otimes_K F$的元素$\sum_{\lambda \in L} v_\lambda \otimes f_\lambda$在(26)下被识别为映射$x \mapsto \sum_\lambda v_\lambda(x) f_\lambda$。由于除了$L$的指标$\lambda$属于至有限子集$H$之外的$v_\lambda = 0$，上述映射下的$X$的像包含在子空间的有限维子空间中$F$由指标$\lambda \in H$的$f_\lambda$生成。相反，令$u : X \to F$为映射，使得$u(X)$包含在$F$的有限维子空间$G$中，并令$(b_i)_{1 \leq i \leq n}$为$G$的基。对于所有$x \in X$，我们可以写成$u(x) = \sum_{i=1}^n v_i(x) b_i$，其中$v_i(x)$很好地确定了$K$的元素；因此 $n$ 映射 $v_i : X \to K$ 被定义，并且显然 $u$ 被识别为元素 $\sum_{i=1}^n v_i \otimes b_i$。

同样，对于$K$和集合$Y$上的右向量空间$E$，$E \otimes_K K_s^Y$被识别为空间$E^Y$的子空间、映射的由……组成 $v : Y \to E$使得$v(Y)$等于有限秩。更具体地，对于每个域$K$，$K_d^X \otimes_K K_s^Y$被识别为$X \times Y$的映射的子空间、空间的$K^{X \times Y}$到$K$（$K$被认为是$(K, K)$-双模）； 元素 $\sum_i u_i \otimes v_i$，其中 $u_i$ 是 $X$ 到 $K$ 的映射，以及 $Y$ 到 $K$ 的 $v_i$ 映射，用映射进行标识$(x, y) \mapsto \sum_i u_i(x) v_i(y)$ 中的 $X \times Y$ 变为 $K$。

#### 命题 16 {#alg-ii-s7-prop-16 .statement tag=05T2}

(i) *设 K、L 为两个域，E 左向量空间在 K 上，F 左向量空间在 L 上，G 为 (K, L)-双模。然后是规范的$\mathbf{Z}$-同态*

$$
\nu : \operatorname{Hom}_K(E, G) \otimes_L F \to \operatorname{Hom}_K(E, G \otimes_L F)
$$

(§ 4, no. 2, 公式 (7)) *是单射；当向量空间 E, F 之一是有限维*时，它是双射的。

(ii) *令 $E_1, E_2, F_1, F_2$ 为向量空间除交换域 K 的四倍；那么规范的 K-同态*

$$
\lambda : \operatorname{Hom}(E_1, F_1) \otimes \operatorname{Hom}(E_2, F_2) \to \operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)
$$

(§ 4, no. 4, 公式 (21)) *是单射；如果有序对 $(E_1, E_2), (E_1, F_1), (E_2, F_2)$ 之一由有限维空间* 组成，则它是双射的。

断言 (i) 是 § 4, no. 2, 命题 2 的特例。类似地，(ii) 的第二个断言是 § 4, no. 4, 命题 4 的特例。最后，要看到同态 (28) 始终是单射的，请观察$\operatorname{Hom}(E_i, F_i)$ 是 $F_i^{E_i}$ ($i = 1, 2$) 的向量子空间并且

$$
\operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)
$$

被规范地标识为空间 $(F_1 \otimes F_2)^{E_1 \times E_2}$ (II, § 3, no. 1, 命题 1) 的向量子空间；当进行这些识别并且（28）的左侧也被识别为$F_1^{E_1} \otimes F_2^{E_2}$（命题 14）的子空间时，典范映射（28）变为限制到典范映射（26）的子空间，并且已经看到（命题15）后者是单射的。

#### 推论 1 {#alg-ii-s7-prop-16-cor-1 .statement tag=05T3}

*设 E 和 F 为域 K 上的 2 向量空间； 典范映射*

$$
E^* \otimes_K F \to \operatorname{Hom}_K(E, F)
$$

(§ 4, no. 2, 公式 (11)) *是单射；当 E 或 F 是有限维*时，它是双射的。

这是命题 16 (i) 的特例。

#### 推论 2 {#alg-ii-s7-prop-16-cor-2 .statement tag=05T4}

*设 E 为右向量空间，F 左向量空间在相同的域 K 上； 典范映射*

$$
E \otimes_K F \to \operatorname{Hom}_K(E^*, F)
$$

(§ 4, no. 2, 公式 (15)) *是单射；当 E 是有限维*时，它是双射的。

这是§ 4, no. 2、注 2 的特例。

#### 注 {#alg-ii-s7-n7-rem-1 .statement tag=05T5}

(1) Let K be a *commutative* field, E, F two vector spaces over K, (a_\lambda) a basis of E and (b_\mu) a basis of F; then (a_\lambda \otimes b_\mu) is a basis of the vector K-space E \otimes_K F (II, § 3, no. 7, Corollary 2 to Proposition 2) and therefore
$$
\dim_K(E \otimes_K F) = \dim_K E \cdot \dim_K F.
$$
(2) Let K be a *commutative* field, E_1, E_2, F_1, F_2 four vector spaces over K and u:E_1 \to F_1, v:E_2 \to F_2 two linear mappings; then
$$
\operatorname{rg}(u \otimes v) = \operatorname{rg}(u) \cdot \operatorname{rg}(v).
$$
It is immediate that $(u \otimes v)(E_1 \otimes E_2)$ is the canonical image of $u(E_1) \otimes v(E_2)$ in $F_1 \otimes F_2$ and hence (Proposition 14) is isomorphic to $u(E_1) \otimes v(E_2)$; the conclusion then follows from (30).
(3) Under the same hypotheses as in *Remark* 1,
$$
\dim_K(\operatorname{Hom}_K(E, F)) \geq \dim_K E \cdot \dim_K F.
$$
If E is isomorphic to $K^{(I)}$, $\operatorname{Hom}(E, F)$ is isomorphic to $(\operatorname{Hom}(K, F))^I$ (§ 1, no. 6, Corollary 1 to Proposition 6) and hence to $F^I$ (§ 1, no. 14); as $F^{(I)}$ is a subspace of $F^I$ and $\dim(F^{(I)}) = \operatorname{Card}(I) \cdot \dim F = \dim E \cdot \dim F$ (no. 2, Proposition 2), the inequality (32) follows from no. 3, Corollary 4 to Proposition 4. 同样的论证表明，当 $\dim E$ 是*有限*时，(32) 的两侧相等（cf. § 10，第 3 条和第 4 条）。

### 8. 秩元素张量积

设 E 为右向量空间，F 左向量空间在相同的域 K 上；对于每个元素 $u \in E \otimes_K F$，规范地在 (29) 同态 $u_1 \in \operatorname{Hom}_K(E^*, F)$ 下有对应；如果 $u = \sum_i x_i \otimes y_i$ 与 $x_i \in E, y_i \in F$，则元素 $u_1$ 为线性映射
$$
x^* \mapsto \sum_i \langle x^*, x_i \rangle y_i.
$$
另一方面，$E \otimes_K F$在规范上与$F \otimes_{K^0} E$等同，其中E被视为左向量空间，F被视为右向量空间，而相反的域$K^0$；因此，对应规范地为 $u$ 同态 $u_2 \in \operatorname{Hom}_K(F^*, E)$ 给出
$$
y^* \mapsto \sum_i x_i \langle y_i, y^* \rangle;
$$
$u_1$（或$u_2$），被视为$E^*$的映射到$F^{**}$（或$F^*$到$E^{**}$）只是$u_2$（或转置）的*转置*。 $u_1$）。 因此，$u_1$和$u_2$的*秩*等于*相同的*有限*数$r$、F的子空间$u_1(E^*)$和E的$u_2(F^*)$的公共的维数，其中每一个都是规范的同构于另一个的对偶 (no. 5)；我们可以说，$r$（表示为$\operatorname{rg}(u)$）是$E \otimes_K F$的元素$u$的*秩*，$u_1(E^*)$和$u_2(F^*)$是子空间（分别是F和E）与$u$*关联*。

#### 命题 17 {#alg-ii-s7-prop-17 .statement tag=05T6}

Let u be an element of $E \otimes_K F$ and $M \subset E$ and $N \subset F$ its associated subspaces. 对于$u$的每个表达式$u = \sum_{i=1}^s x_i \otimes y_i$，其中$x_i \in E$和$y_i \in F$代表$1 \leq i \leq s$，子空间$M$（或$N$）包含在$E$（或$F$）的子空间中，由$x_i$（分别为$y_i$）。 此外，以下属性是等效的：

(a) 整数 $s$ 等于 $u$ 的秩。
(b) 家庭$(x_i)_{1 \leq i \leq s}$ 是$M$ 中的基。
(c) 家庭$(y_i)_{1 \leq i \leq s}$ 是基 $N$。
(d) $(x_i)_{1 \leq i \leq s}$和$(y_i)_{1 \leq i \leq s}$家庭都是免费的。

由(33)(或(34))，$N = u_1(E^*)$(或$M = u_2(F^*)$)的每个元素是$y_i$(或$x_i$)的线性组合； 从而第一个断言。如果由 $x_i$（分别为 $y_i$）与维数 $\leq \dim M$（分别为 $\leq \dim N$）和包含 $M$（分别为 $N$）生成的 $s = r$、子空间与其相同，因此 (a) 意味着（b）和（c）以及*更不必说*（d）。相反，条件 (b) 和 (c) 均意味着 (a) 除以 $\mathrm{rg}(u)$ 的定义。最后，如果 (d) 成立，则存在$E^*$的元素的$(x_i^*)_{1 \leq i \leq s}$族，使得$\langle x_i, x_j^* \rangle = \delta_{ij}$（no. 5，推论1到定理7），因此从(33)可以得出，$(y_i)$是基 $N$，完成证明。

#### 推论 1 {#alg-ii-s7-prop-17-cor-1 .statement tag=05T7}

* u 的秩是最小的整数 s，因此存在一个表达式* $u = \sum_{i=1}^s x_i \otimes y_i$，*其中* $x_i \in E$ *和* $y_i \in F$ *对于* $1 \leq i \leq s$。

这紧接着命题 17 和 no. 2、命题 1。

#### 推论 2 {#alg-ii-s7-prop-17-cor-2 .statement tag=05T8}

*设 K 为交换域，E、F 为 K 上的两个向量空间，L 为 K 的交换律扩张域。设 u 为* $E \otimes_K F$ 的元素，*M 和 N 与 u 中的子空间和 u' 典范像相关* $(E \otimes_K F)_{(L)}$ *（规范地标识为* $E_{(L)} \otimes_L F_{(L)}$、*cf. § 5, no. 1、命题 3）；那么与 u' 伴随的* $\mathrm{rg}(u') = \mathrm{rg}(u)$ *和子空间被规范地标识为* $M_{(L)}$ *和* $N_{(L)}$。

如果$u = \sum_{i=1}^r x_i \otimes y_i$，其中家庭$(x_i)$和$(y_i)$是免费的，则$u' = \sum_{i=1}^r (1 \otimes x_i) \otimes (1 \otimes y_i)$以及家庭$(1 \otimes x_i)$和$(1 \otimes y_i)$分别在$E_{(L)}$和$F_{(L)}$中是免费的（§ 5, no. 1，命题4）。

### 9. 向量空间的标量扩张

回想一下 (I, § 9, no. 1, 定理 2)，域 K 的同态到非零环 A 必然是*单射的*。

#### 命题 18 {#alg-ii-s7-prop-18 .statement tag=05T9}

令$\varphi$为域$K$到环$A$的同态。对于向量$K$-空间和$K$-线性映射中的每个正合序列

$$
E' \xrightarrow{u} E \xrightarrow{v} E''
$$

序列

$$
E'_{(A)} \xrightarrow{u_{(A)}} E_{(A)} \xrightarrow{v_{(A)}} E''_{(A)}
$$

是准确的。

这是 no. 7、命题 14 的特例，考虑到 § 1, no. 4、注 4。

#### 推论 {#alg-ii-s7-n9-cor-1 .statement tag=05TA}

对于每个$K$-线性映射$f : E' \to E$、$\operatorname{Im}(f_{(A)}) = (\operatorname{Im}(f))_{(A)}$、$\operatorname{Ker}(f_{(A)}) = (\operatorname{Ker}(f))_{(A)}$、$\operatorname{Coker}(f_{(A)}) = (\operatorname{Coker}(f))_{(A)}$，到典范同构之内。

#### 命题 19 {#alg-ii-s7-prop-19 .statement tag=05TB}

设$\varphi$为域$K$到环$A$的单同态。对于超过 $K$ 的每个左向量空间 $E$，典范映射 $\phi : E \to \varphi^*(E) = A \otimes_K E$ 是单射的。此外，对于$E$的每个向量子空间$E'$，$\varphi^*(E') = A \otimes_K E'$都被规范地标识为$A \otimes_K E$的直因子子$A$模块，并且通过此标识，

$$
(A \otimes_K E') \cap \phi(E) = \phi(E').
$$

第一个断言是§ 5, no. 1、命题4的特例；第二个是no. 7、命题14的特例；最后，为了证明（35），只需接受$A$（被视为右$K$模块）基$(a_\lambda)_{\lambda \in L}$，使得$a_{\lambda_0} = 1$对于某些指标$\lambda_0$（no. 1，定理） 2）； $A \otimes_K E$的元素可以唯一地写为$\sum \lambda a_\lambda \otimes x_\lambda$和$x_\lambda \in E$，并且对于这样的元素到属于到$A \otimes_K E'$，$x_\lambda \in E'$对于所有$\lambda$是必要且充分的。另一方面，$\phi(E)$中的元素是$x_\lambda = 0$对应$\lambda \neq \lambda_0$；对于元素$\sum \lambda a_\lambda \otimes x_\lambda$到属于到$(A \otimes_K E') \cap \phi(E)$，$x_\lambda = 0$对于$\lambda \neq \lambda_0$和$x_{\lambda_0} \in E'$，从而的结论是充分必要的。

#### 推论{#alg-ii-s7-n9-cor-2 .statement tag=05TC}

设$\varphi$是域$K$到环$A$的单同态。对于$K$线性映射$f : E \to F$（其中$E$和$F$是$K$上的两个向量空间）是单射（或满射，零），$f_{(A)} : E_{(A)} \to F_{(A)}$是单射（或零）是必要且充分的。满射，零）。

这紧随命题 19 和推论到命题 18。

#### 命题 20 {#alg-ii-s7-prop-20 .statement tag=05TD}

设$\rho$为域$K$到环$A$的同态。对于每个左向量空间$E$超过$K$，规范右$A$-模块同态

$$
v : (E^*)_{(A)} \to (E_{(A)})^*
$$

(§ 5, no. 4) 是单射的；当 $E$ 是有限维时，它是双射的。

第二个断言由§ 5, no. 4、命题 8得出。为了证明第一个注，$(E^*)_{(A)}$的每个元素都可以写成$\sum_i x_i^* \otimes \alpha_i$，其中$\alpha_i \in A$和$(x_i^*)_{1 \leq i \leq n}$是$E^*$中的自由族； $(E_{(A)})^*$ 线性形式 $y^*$ 中有对应，这样 $y^*(1 \otimes x) = \sum_i \rho(\langle x, x_i^* \rangle) \alpha_i$ 对于所有 $x \in E$。但是，$E$中存在一个$(x_i)_{1 \leq i \leq n}$族，使得$\langle x_i, x_j^* \rangle = \delta_{ij}$（no. 5，推论2到定理7），从而$y^*(1 \otimes x_i) = \alpha_i$；因此，关系$y^* = 0$意味着所有$i$都是$\alpha_i = 0$，这证明了我们的断言。

#### 命题 21 {#alg-ii-s7-prop-21 .statement tag=05TE}

设$K$为域，且$K$的$L$扩张域。

(i) 对于超过 $K$ 的每向量空间 $E$，$\dim_L(E_{(L)}) = \dim_K E$。

(ii) 对于每个$K$-线性映射$u : E \to F$，其中$E$和$F$是向量空间超过$K$、$\operatorname{rg}(u_{(L)}) = \operatorname{rg}(u)$。

如果$(e_i)_{i \in I}$在$K$上是$E$的基，$(1 \otimes e_i)_{i \in I}$在$L$上是$E_{(L)}$的基（§ 5, no. 1，命题4），从而第一个断言；第二个源自第一个，并且通过命题 18 的推论，$u_{(L)}(E_{(L)})$ 与 $(u(E))_{(L)}$ 被规范地等同。

#### 命题 22 {#alg-ii-s7-prop-22 .statement tag=05TF}

令$K$为交换域，$\rho : K \to A$是一个单射中心同态，$E, F$是$K$上的两个向量空间。然后典范同态

$$
\omega : A \otimes_K \operatorname{Hom}(E, F) \to \operatorname{Hom}_A(E_{(A)}, F_{(A)})
$$

(§ 5, no. 3, 公式 (17)) 是单射；如果$A$或$E$是有限维向量空间超过$K$，它是双射的。

这是 § 5, no. 3、命题 7 的特例。

### 10.模超过整环

#### 命题 23 {#alg-ii-s7-prop-23 .statement tag=05TG}

在模$E$超过整环$A$，非自由元素的集合$T$是$E$的子模。

如果$x$和$y$不是自由的，则$A$中存在两个非零元素$\alpha, \beta$，使得$\alpha x = 0$和$\beta y = 0$。 Then $\alpha \beta \neq 0$ since $A$ is an integral domain and $\alpha \beta (\lambda x + \mu y) = 0$ for all $\lambda$ and $\mu$ in $A$ since $A$ is commutative, hence $\lambda x + \lambda y$ is not free.

#### 注 {#alg-ii-s7-n10-rem-1 .statement tag=05TH}

令 $E$ 为模超过任意交换环 $A$。如果$x$是$E$的非自由元素，则子模$Ax$的每个元素都是非自由的。另一方面，如果$A$包含除子为0，$E$的两个非自由元素的和可能是自由的；对于例，在$\mathbf{Z}/6\mathbf{Z}$被视为模自身之上，3和4不是免费的，但$3 + 4 = 1$是免费的。

命题 23 导致以下定义：

#### 定义 5 {#alg-ii-s7-def-5 .statement tag=05TI}

*在模$E$超过整环$A$，$E$的挠元子模是非自由元素*的$E$由……组成的子模（也称为*挠元） 元素* 共 $E$)。

当$E$等于其挠元子模时（即$E$的每一个元素都被$A$的元素$\neq 0$湮灭）$E$称为*挠元模*。当$E$的挠元子模减少到0时（即$E$的每个非零元素都是*自由*）$E$（通过滥用语言）被称为*无扭转模块*。

自由 $A$ 模块的每个子模（特别是每个*投影*$A$-模块）都是无扭转的。 $\mathbf{Z}$-模块$\mathbf{Q}$是无扭转的。

#### 命题 24 {#alg-ii-s7-prop-24 .statement tag=05TJ}

*设$A$为整环。对于每个$A$-模块$E$，让$T(E)$表示$E$的挠元子模。令$f : E \to E'$为$A$线性映射，$E$和$E'$为$A$-模块。*

（一）$f(T(E)) \subset T(E')$。
(ii) *如果 $f$ 是单射的，$f(T(E)) = T(E') \cap f(E)$。*
(iii) *如果 $f$ 是满射且 $\operatorname{Ker}(f) \subset T(E)$，则 $f(T(E)) = T(E')$。*

断言 (i) and (ii) are obvious.另一方面，如果$f$是满射且$x' \in T(E')$，则$x' = f(x)$，其中$x \in E$，并且通过假设，$A$中存在$\alpha \neq 0$，使得$f(\alpha x) = \alpha x' = 0$； 从而$\alpha x \in \operatorname{Ker}(f)$，到假设时，$A$中存在$\beta \neq 0$，使得$\beta(\alpha x) = 0$；如$\beta \alpha \neq 0$、$x \in T(E)$。

#### Corollary 1 {#alg-ii-s7-prop-24-cor-1 .statement tag=05TK}

*对于每个 $A$-模块 $E$，$E/T(E)$ 都是无扭转的。*

如果$f : E \to E'$是$A$线性映射，则令$f_T$表示映射$T(E) \to T(E')$，与$f$到$T(E)$的限制具有相同的图。有了这个记号：

#### Corollary 2 {#alg-ii-s7-prop-24-cor-2 .statement tag=05TL}

*对于$A$-模块和$A$-线性映射中的每个正合序列*

$$
0 \longrightarrow E' \xrightarrow{f} E \xrightarrow{g} E''
$$

*序列*

$$
0 \longrightarrow T(E') \xrightarrow{f_T} T(E) \xrightarrow{g_T} T(E'')
$$

*准确*。

$$
\operatorname{Ker}(g_T) = \operatorname{Ker}(g) \cap T(E) = f(E') \cap T(E) = f(T(E')) = \operatorname{Im}(f_T).
$$

#### 命题 25 {#alg-ii-s7-prop-25 .statement tag=05TM}

*令$A$为整环和$(E_i)$一系列$A$模块；那么*

$$
T\left( \bigoplus_i E_i \right) = \bigoplus_i T(E_i).
$$

令 $(x_i)$ 为 $\bigoplus_i E_i$ 的元素，使得 $x_i \in T(E_i)$ 对于所有 $i$；那么每个$x_i$都被$A$的元素$\alpha_i \neq 0$湮灭，并且可以假设当$x_i = 0$时$\alpha_i = 1$；由于族$(x_i)$有有限支撑，定义了$A$的元素$\alpha = \prod_i \alpha_i$和$\neq 0$；显然它消灭了$\bigoplus_i x_i$，因此消灭了$\bigoplus_i T(E_i) \subset T\left(\bigoplus_i E_i\right)$； 逆命题是直接的。

如果$E$和$F$是两个$A$模，则显然$T(E) \otimes_A F$和$E \otimes_A T(F)$的$T(E \otimes_A F)$包含典范像；但例可以由*无扭转*$A$-模块$E, F$给出，这样$T(E \otimes_A F) \neq 0$（习题31）。

注挠元模的*无限* 乘积不一定是挠元模；对于例，在$\mathbf{Z}$-模块$\prod_{n=1}^\infty (\mathbf{Z}/p^n\mathbf{Z})$（$p$整数 > 1）中，所有坐标为1的元素都是空闲的。

#### 命题 26 {#alg-ii-s7-prop-26 .statement tag=05TN}

*令$A$为整环，$K$是分数的域，$E$是一个$A$模块，$E_{(K)} = K \otimes_A E$向量空间是通过扩展环运算符获得的$K$；让 $\phi$ 表示 $E$ 到 $E_{(K)}$ 的规范 $A$ 线性映射 $x \mapsto 1 \otimes x$。*

(i) *$E_{(K)}$的每个元素对于$\lambda \in A, \lambda \neq 0$和$x \in E$来说都是形式$\lambda^{-1} \phi(x)$。*
(ii) *$\phi$中的核是$E$中的挠元子模$T(E)$。*

(i) $E_{(K)}$的每个元素都是形式$z = \sum_{i=1}^n \xi_i \phi(x_i)$，其中$\xi_i \in K$和$x_i \in E$；对于所有$i$，存在$\alpha_i \in A$使得$\alpha_i \neq 0$和$\alpha_i \xi_i \in A$；如果$\alpha = \prod_{i=1}^n \alpha_i$，则$\alpha \neq 0$和$\alpha \xi_i = \beta_i \in A$对于所有$i$、从而，在$E_{(K)}$中，

$$
z = \alpha^{-1}(\alpha z) = \alpha^{-1} \sum_{i=1}^n \beta_i \phi(x_i) = \alpha^{-1} \phi\left( \sum_{i=1}^n \beta_i x_i \right)
$$

因为 $\phi$ 是 $A$ 线性的。

(ii) 如果$x \neq 0$在$E$中不自由，则$A$中存在$\alpha \neq 0$，使得$E_{(K)}$中存在$\alpha x = 0$、从而$\alpha \phi(x) = \phi(\alpha x) = 0$，这意味着$\phi(x) = 0$。相反，假设对于 $E_{(K)}$ 中的某些 $x \in E$、$1 \otimes x = 0$；我们证明$x$是$E$的挠元元素。我们考虑$K$的*单源*子$A$模块的集合$\mathfrak{M}$；这是关系下的有向集合包含权，对于$K$的任何两个元素$\alpha, \beta$都可以写成$\alpha = \zeta^{-1} \xi, \beta = \zeta^{-1} \eta$，其中$\xi, \eta, \zeta$属于到$A$和$\zeta \neq 0$，因此$A.\alpha \subset A.\zeta^{-1}$ 和 $A.\beta \subset A.\zeta^{-1}$。此外，$K$是模$M \in \mathfrak{M}$的并，因此可以被视为直接系统的*直极限*，由模$M \in \mathfrak{M}$和典范嵌入定义（§ 6, no. 2， *注*)。因此，在典范同构、$E_{(K)} = \lim \rightarrow (M \otimes_A E)$（§ 6, no. 3、命题 7）和$E_{(K)}$中的关系$1 \otimes x = 0$意味着存在

M ∈ $\mathscr{P}$ 使得 l ∈ M 且 l ⊗ x = 0 in 张量积 M ⊗_A E（集合理论，III, § 7, no. 5，引理 1）。还可以进一步假设（替换，如果需要通过 K 的单生子模 M' ⊃ M 来表示 M）M = A.γ^{-1}，其中 γ ∈ A 且 γ ≠ 0。现在映射 ψ ↦ γψ 是 M 的同构到 A-模 A 上；另一方面，典范同构 A ⊗_A E → E (§ 3, no. 4, 命题 4) 映射 ψ ⊗ x 到 E 的元素 ψx；因此存在同构 M ⊗_A E → E，其中映射张量积 xi ⊗ x 到 E 的元素 (γψ)x。 M ⊗_A E 中的假设 l ⊗ x = 0 因此意味着 γx = 0。

#### 注 {#alg-ii-s7-n10-rem-2 .statement tag=05TO}

设α^{-1}φ(x)、β^{-1}φ(y)为E_{(K)}的两个元素，其中α ε A、β ε A、x ε E、y ε E、αβ ≠ 0。在阶中，α^{-1}φ(x) = β^{-1}φ(y)，有必要足以使 βx − αy 成为 E 的挠元元素，因此关系等价于 βφ(x) = αφ(y)，也可写为 φ(βx − αy) = 0。

#### 推论 1 {#alg-ii-s7-prop-26-cor-1 .statement tag=05TP}

*如果 E 是无扭转 A 模，则典范映射* φ : E → E_{(K)} *是单射*。

回想一下 (§ 5, no. 1)，对于 E 的每一个 A-线性映射到 K 上的向量空间 F，存在且仅有一个 K-线性映射 $\vec{f} : E_{(K)} \to F$ 使得 $f = \vec{f} \circ \phi$；我们可以说 $\vec{f}$ 与 $f$ *关联*。

#### 推论 2 {#alg-ii-s7-prop-26-cor-2 .statement tag=05TQ}

*设 f 为 E 的 A-线性映射到 K 上的向量空间 F；如果 Ker(f) ⊂ T(E), K-线性映射* $\vec{f}$ *与 f 相关联是单射*。

我们将 Ker($\vec{f}$) 的元素写在形式 $\lambda^{-1}\phi(x)$ 中，其中$\lambda \in A, \lambda \neq 0, x \in E$； 关系 $\vec{f}(\lambda^{-1}\phi(x)) = 0$ 相当于 F 中的 $\lambda^{-1}\vec{f}(\phi(x)) = 0$，因此也相当于 $f(x) = \vec{f}(\phi(x)) = 0$。通过假设，这意味着$x \in T(E)$，因此也意味着$\phi(x) = 0$，这证明了推论。

#### 推论 3 {#alg-ii-s7-prop-26-cor-3 .statement tag=05TR}

*设 E 为 A-模且 g A-线性映射将 E 转化为 K 上的向量空间 F，使得 g(E) 生成 F 且 Ker(g) ⊂ T(E)。那么与 g 相关的K-线性映射* $\bar{g}$ *是* E_{(K)} *到 F* 上的同构。

根据推论 2 和假设，$\bar{g}$ 是单射的，$g(E)$ 生成 F 意味着 $\bar{g}$ 是满射的。

对于每个 A-模 E，向量空间 E_{(K)} 据说与 E *关联*。对于 E 的每个子集 S，S 的 *秩* 超过 K（或者滥用语言，S 的 *秩*）是秩的典范像 E_{(K)}中S的$\phi(S)$，在由$\phi(S)$生成的E_{(K)}的向量子空间的K上的其他字(no. 2，定义1)维数。

当E是*无扭*A-模时，通常用E_{(K)}中的典范像$\phi(E)$来识别。根据此约定，E 包含的每个生成的系统都有 E_{(K)} 的 *基* (no. 1, 定理 2)。特别是：

#### 推论 4 {#alg-ii-s7-prop-26-cor-4 .statement tag=05TS}

*每个有限生成A-模都是有限秩*。

注该推论的逆命题不一定为真；对于例 $\mathbf{Q}$ 是秩 1 的 $\mathbf{Z}$ 模，但不是在 $\mathbf{Z}$ 上有限生成的。

回想一下（§ 5, no. 1），对于每个线性映射$f : E \to E'$（其中$E$和$E'$是$A$模块），$f_{(K)}$表示$K$线性映射$1_K \otimes f : E_{(K)} \to E'_{(K)}$。

#### 命题 27 {#alg-ii-s7-prop-27 .statement tag=05TT}

*每正合序列*

$$
E' \xrightarrow{f} E \xrightarrow{g} E''
$$

*$A$-线性映射，相应的序列，$K$-线性映射*

$$
E'_{(K)} \xrightarrow{f_{(K)}} E_{(K)} \xrightarrow{g_{(K)}} E''_{(K)}
$$

*准确。*

假设$g_{(K)}(\lambda^{-1} \otimes x) = 0$，有$\lambda \in A, \lambda \neq 0, x \in E$；这相当于$E''_{(K)}$中的$\lambda^{-1} \otimes g(x) = 0$，因此也相当于

$$
1 \otimes g(x) = \lambda(\lambda^{-1} \otimes g(x)) = 0;
$$

到命题 26，$A$中存在$\alpha \neq 0$，使得$E''$中存在$\alpha g(x) = 0$，或者也存在$g(\alpha x) = 0$。到假设，因此存在$x' \in E'$，使得$\alpha x = f(x')$，因此有$\lambda^{-1} \otimes x = f_{(K)}(\alpha^{-1}\lambda^{-1} \otimes x')$，这证明了命题。

#### 推论 1 {#alg-ii-s7-prop-27-cor-1 .statement tag=05TU}

*如果 $E'$ 是 $E$ 的子模，则 $E'_{(K)}$ 规范地与 $E_{(K)}$ 的向量子空间进行标识，$(E/E')_{(K)}$ 与 $E_{(K)}/E'_{(K)}$ 进行规范地标识。*

应用命题 27 至正合序列即可

$$
0 \to E' \to E \to E/E' \to 0.
$$

#### 推论 2 {#alg-ii-s7-prop-27-cor-2 .statement tag=05TV}

*对于每个$A$-线性映射$f : E \to F$、$\operatorname{Ker}(f_{(K)}) = (\operatorname{Ker}(f))_{(K)}$、$\operatorname{Im}(f_{(K)}) = (\operatorname{Im}(f))_{(K)}$、$\operatorname{Coker}(f_{(K)}) = (\operatorname{Coker}(f))_{(K)}$到典范同构以内。特别是，对于$f_{(K)}$是单射（或满射，或零），$\operatorname{Ker}(f) \subset T(E)$（或$\operatorname{Coker}(f)$是挠元模，或$\operatorname{Im}(f) \subset T(F)$）是必要且充分的。*

这是从推论 1 和命题 26 得出的。

#### 推论 3 {#alg-ii-s7-prop-27-cor-3 .statement tag=05TW}

*令$E$为$A$模块，$(x_\lambda)_{\lambda \in L}$为$E$的元素族。要使$(x_\lambda)$成为一个自由的家庭，向量$K$-空间$E_{(K)}$家庭$(1 \otimes x_\lambda)$自由是必要且充分的。*

$(x_\lambda)$定义是$A$线性映射$f : A^{(L)} \to E$，使得$f(e_\lambda) = x_\lambda$对于所有$\lambda \in L$（$(e_\lambda)$是$A^{(L)}$的典范基）并且说$(x_\lambda)$是免费的意味着$f$ 是单射的。将推论 2 应用到 $f$、注意到即可，$A^{(L)}$ 是无扭转的 (命题 25)。

### 习题{#alg-ii-s7-exercises}

请参阅[§ 7](exercises/s7/)的[习题]。
