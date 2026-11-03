---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 13
section_title: Absolutely Semisimple Algebras
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.229-A VIII.249
pdf_pages: 0246-0266
extraction: native+ocr
subsections:
    - "no": 1
      title: Absolutely Semisimple Modules
      page: 229
      pdf_page: 246
    - "no": 2
      title: Algebras over Separably Closed Fields
      page: 230
      pdf_page: 247
    - "no": 3
      title: Absolutely Semisimple Algebras
      page: 231
      pdf_page: 248
    - "no": 4
      title: Characterization of Absolutely Semisimple Modules
      page: 235
      pdf_page: 252
    - "no": 5
      title: Derivations on Semisimple Algebras
      page: 236
      pdf_page: 253
    - "no": 6
      title: Cohomology of Algebras
      page: 239
      pdf_page: 256
    - "no": 7
      title: Cohomology of Absolutely Semisimple Algebras
      page: 241
      pdf_page: 258
    - "no": 8
      title: The Splitting of Artinian Algebras
      page: 243
      pdf_page: 260
statements: 33
exercises: 12
content_sha256: ed8268dd8bfd6a89661fd6ca9b3f36783342e8d4e155bcba0096866542105ae4
translated_from: content/en/alg/VIII/13_s13_absolutely_semisimple_algebras.md
translation_method: google
source_content_sha256: 20e8293964011d4b021666f811555994484c4df5ad3a8aa7a6c4c31c70bdaac0
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 3248250d3c1ced2c35075b2fb850d47f5b865960be3615ea0965504a538624c2
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 13。 绝对半单代数

### 1. 绝对半单模

#### 定义 1 {#alg-viii-s13-def-1 .statement tag=00F9}

设 K 为交换域，A K-代数。如果对于 K 的每个扩张 L，$A_{(L)}$-模 $M_{(L)}$ 是半单，我们称A-模 M 绝对半单的。

每个绝对半单模都是半单。相反，如果域 K 是完美的，则 K 上的每个有限维半单A-模都是绝对半单的 (VIII, p. 222, 推论 1, a))，因为完美域的每个扩张都是可分的（V, §7, No. 1、p. 36、命题2）。

#### 命题 1 {#alg-viii-s13-prop-1 .statement tag=00FA}

设 K 为交换域，A K-代数。

a) 绝对半单的 A-模中的每个直和都是绝对半单的 A-模。 绝对半单模的每个子模和商模都是绝对半单的。

b) 设 M 为 A-模，并令 L 为域 K 的扩张。A-模 M 为绝对半单的当且仅当 $A_{(L)}$ 模 $M_{(L)}$ 为绝对半单的。

断言 a) 由类似的断言推导出半单模（VIII、p. 56，推论 1 和 3）。

假设A-模 M 为绝对半单的，并令$L'$ 为L 的扩张。作为 $A_{(L')}$ 模块，$L'\otimes_LM_{(L)}$ 与 $M_{(L')}$ 同构的（II, §5, No. 1、p. 273、命题 2）；因此是半单模。这就证明$M_{(L)}$是绝对半单的。

相反，假设$M_{(L)}$是绝对半单的。设$L'$为K的扩张。存在L和$L'$的复合扩张$(\Omega , u, v)$(V, §2, No. 4,p. 13,推论)；我们认同 L 和 $L'$ 带有 Ω 的子扩展。 $A_{(\Omega )}$-模块$M_{(\Omega )}$同构于$(M_{(L)})_{(\Omega )}$；因此是半单。但$M_{(\Omega )}$也同构于$(M_{(L')})_{(\Omega )}$，且命题 8，VIII、p. 222的a)意味着$M_{(L')}$是半单。所以M是绝对半单的。

#### 命题 2 {#alg-viii-s13-prop-2 .statement tag=00FB}

设 K 为交换域、A K-代数和 M A-模，它们是 K 上的有限维。以下属性是等效的：

(i) A-模 M 为绝对半单的。

(ii) 存在 K 的扩张 P 为完美域，使得$A_{(P)}$-模$M_{(P)}$ 为半单。

(iii) A-模 M 是半单，并且其交换子中的中心是域 K 上的 étale 代数。

显然，(i) 意味着(ii)。假设 (ii) 成立；那么$A_{(P)}$-模$M_{(P)}$是绝对半单的乘以推论1，a) of VIII，p. 222。通过命题 1，b)，M 则为绝对半单的。因此，(ii) 意味着(i)。

假设M是半单。设Z为M的交换子中心；它是有限次数的交换代数超过域K。如果L是K的扩张，那么从VIII、p. 222的命题8，b)得出$A_{(L)}$模当且仅当环 $Z_{(L)}$ 减少时，$M_{(L)}$ 才为半单。因此，(i)和(iii)的等价由V, §6, No. 7、p. 34的定理 4得出。

### 2. 代数超过可分闭域

#### 引理 1 {#alg-viii-s13-lem-1 .statement tag=00FC}

设 D 为域，Z 为中心。用$p$表示Z的特征指数。假设对于 D 的每个元素 $a$，都存在整数 $m\geqslant 0$，使得 $a^{p^m}$ 属于到 Z。则域 D 是可交换的。

如果 $p= 1$，则 D = Z。因此我们假设 $p >1$。

让我们通过反证法给出证明并假设 D 不可交换。令 $a$ 为 D-Z 的元素和 $p$ 的 $q$ 幂，使得 $a^q$ 属于到 Z。用 I 和内自同构表示 D 上的恒等映射 $x\mapsto axa^{-1}$从D到D通过$\sigma$与$a$相关联；我们有$\sigma^q= I$，因为$a^q$属于到Z。我们有$\sigma -I\not= 0$，因为$a$没有属于到Z，我们有$(\sigma -I)^q=\sigma^q-I = 0$，因为Z具有特征$p$。令$f$为最大的自然数，使得$(\sigma -I)^f\not= 0$；我们有$f\geqslant 1$。 D 的选择元素 $c$ 使得 $(\sigma -I)^f(c)\not= 0$ 和集合

$$
x= (\sigma -I)^{f-1}(c),y= (\sigma -I)(x) = (\sigma -I)^f(c)
$$

到构造，我们有$y\not= 0$和$\sigma (y) =y$；如果我们集合 $z=y^{-1}x$，那么可以得出结论

$$
\sigma (z) =\sigma (y)^{-1}\sigma (x) =y^{-1}(y+x) = 1 +z
$$

因此，每自然数 $j$ 就有 $\sigma (z^{p^j}) = 1 +z^{p^j}$。 选择整数$m\geqslant 0$使得D的$z^{p^m}$属于到中心Z；我们有

$$
z^{p^m}=az^{p^m}a^{-1}=\sigma (z^{p^m}) = 1 +z^{p^m}
$$

这个矛盾意味着引理 1。

#### 命题 3 {#alg-viii-s13-prop-3 .statement tag=00FD}

令 K 为可分闭域 (V, §7, No. 8, p. 45, 定义 4)，并令 D 为有限次数与 K 域上的代数。那么D是可交换的。

用 $p$ 表示 K 的特征指数。令 $a$ 为 D 的元素。环 $K[a]$ 是 K 的代数扩张 (V, §3, No. 1, p. 17, 推论 1)。由于域 K 是可分离闭的，因此从 V, §7, No. 7、p. 44、命题 13 可以得出，代数 $K[a]$ 是 K 的 $p$ 根式扩展。因而，存在整数 $m\geqslant 0$，使得$a^{p^m}$ 属于到 K。通过引理 1，域 D 因此是可交换的。

#### 推论 {#alg-viii-s13-n2-cor-1 .statement tag=00FE}

设 K 为可分闭域，且有限次数的 A 半单代数在 K 上。则存在整数 $r\geqslant 0$，严格地正整数 $n_1, . . . , n_r$，以及有限次数的 K 扩张 $K_1, . . . ,K_r$，使得 A与代数 $\prod_{i=1}^r\mathbf{M}_{n_i}(K_i)$ 同构的。

通过结构定理对于半单代数（VIII，p. 135，定理1），A与代数$\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$同构的，其中$r$严格是整数$\geqslant 0,n_1, . . . , n_r$ 正整数和$D_1, . . . ,D_r$是有限次数中的K-代数，即域。由于域 K 是可分离闭的，因此每个域 $D_i$ 可交换命题 3；接下来是推论。

### 3. 绝对半单代数

#### 定义 2 {#alg-viii-s13-def-2 .statement tag=00FF}

令 K 为交换域。如果对于 K 的每个扩张 L，环 $A_{(L)}$ 是半单，我们说K-代数 A 是绝对半单的。

绝对半单代数是半单。 K-代数 A 是绝对半单的当且仅当A-模 $A_s$ 是绝对半单的。通过VIII、p. 229的命题 1，我们得到以下结果：如果L是K的扩张，则L代数$A_{(L)}$是绝对半单的当且仅当K-代数A是绝对半单的。

#### 定理 1 {#alg-viii-s13-thm-1 .statement tag=00FG}

设 K 为交换域，A K-代数。以下属性是等效的：

(i) K-代数 A 为绝对半单的。

(ii) 代数 A 对 K 具有有限次数，并且存在 K 的扩张 P，即完美域，其中 P 代数$A_{(P)}$ 为半单。

(iii) K-代数 A 是半单并且在 K 上有有限次数，并且它的中心是一个 étale K-代数。

(iv) 存在有限族$(n_i,D_i)_{i\in I}$，其中$n_i$严格是正整数和有限次数的$D_i$K-代数即域，使得$D_i$的中心$Z_i$为对于每个 $i\in I$，K 的可分扩张且 A 同构于矩阵环 $\mathbf{M}_{n_i}(D_i)$ 的乘积。

(v) 存在 K 的扩张 L 和整数 $(n_i)_{i\in I}$ 的有限族，使得L-代数$A_{(L)}$ 同构于代数 $\prod_{i\in I}\mathbf{M}_{n_i}(L)$。

(vi) 存在有限次数的K的伽罗瓦扩张L和整数$(n_i)$的有限族，使得$A_{(L)}$同构于矩阵代数$\mathbf{M}_{n_i}(L)$的乘积。

我们首先证明含义 (v) $\Rightarrow$ (iv) $\Rightarrow$ (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i)。用 Z 表示 A 的中心。

如果性质 (v) 成立，则 L-代数 $A_{(L)}$ 为半单，且有限次数大于 L，且其中心（同构于 $Z_{(L)}$、III，对于某些整数 $r\geqslant 0$，p. 41、推论) 与 $L^r$ 同构的。到推论 2，VIII、p. 222、代数的 a) A 是半单并且在 K 上有有限次数。因而，它与环 $\prod_{i\in I}\mathbf{M}_{n_i}(D_i)$ 的有限乘积同构$n_i\geqslant 1$ 对于每个 $i\in I$，其中域 $D_i$ 是有限次数的代数超过 K。中心 $Z_i$ $D_i$ 是交换域即扩张 K 的，Z 与 $\prod_{i\in I}Z_i$ 同构的。因而，$Z_{(L)}$ 一方面与 $\prod_{i\in I}(Z_i)_{(L)}$ 同构的，另一方面与 $L^r$ 同构的。在其他字中，代数 $\prod_{i\in I}Z_i$ 在域 K 上是完整的（V, §6, No. 3，p. 28，定义 1），并且扩张 $Z_i$ 中的每一个都在 K 上可分离（V, §6, No. 4、p. 31、推论、V, §7, No. 1、p. 42）。因而 (v) 蕴涵 (iv)。

若性质(iv)成立，则可知A为半单代数且对K有有限次数。其中心Z与有限次数K的可分扩张乘积$\prod_{i\in I}Z_i$同构的；因而，它是一个étale 代数（loc. cit.）。因而 (iv) 意味着 (iii)。

含义 (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i) 来自 VIII 中的命题 2，p. 230 适用于 A-模 $A_s$。

#### 引理 2 {#alg-viii-s13-lem-2 .statement tag=00FH}

设 L 为代数闭域，且 D 域包含 L 位于其中心中。如果 D 与 L 不同，则存在 L 的扩张 $L'$，使得环 $D\otimes_LL'$ 不是左阿廷的。

令 $x$ 为 D - L 的元素；由于L是代数闭的，L的扩张$L'= L(x)$不是代数的，并且$x$超越L。 环 $B = L'\otimes_LL'$ 那么整环乘命题 5 of V, §17, No. 4, p. 141。

B 的元素$y=x\otimes 1-1\otimes x$不是零，但如果$\varphi$是从B到$L'$的同态，将$\xi \otimes \eta$发送到$\xi \eta$，则我们有$\varphi (y) = 0$，所以$y$在B中不可逆。 环 $C = D\otimes_LL'$ 作为其子环 B 的右模；它是自由模因为 D 是右向量空间超过它的子域 $L'$。由于$y$是整环B的非零的和不可逆元素，所以C中的$y$右乘法是映射$R_y$，这是单射但不是双射。现在，$R_y$是左侧C-模块$C_s$的自同态；因而 (VIII, p. 28, 推论 1), 环 C 不是左阿廷的。

现在让我们证明 (i) 蕴涵 (v)。这是以下引理中的推论。

#### 引理 3 {#alg-viii-s13-lem-3 .statement tag=00FI}

设A为K的绝对半单的K-代数和L代数闭扩张。则代数$A_{(L)}$同构于L上的有限多个矩阵代数的乘积。

L-代数$A_{(L)}$是半简单的；因而，它同构于$\mathbf{M}_{n_i}(D_i)$形式的有限多个代数的乘积，其中$D_i$是一个在其中心包含L的域，$n_i$是一个整数$\geqslant 1$（VIII，p. 137，备注1）。

设$L'$为L的扩张。由于K-代数 A 是绝对半单的，环 $A_{(L')}$ 是半单，因此左阿廷的。现在，环$A_{(L')}$同构于$L'\otimes_LA_{(L)}$，因此也同构于$\prod_{i\in I}\mathbf{M}_{n_i}(L'\otimes_LD_i)$；通过VIII、p. 7中的命题 5，因此环$\mathbf{M}_{n_i}(L'\otimes_LD_i)$中的每一个都是左阿廷的。

设 $n\geqslant 1$ 为整数，B 环。设$(\mathfrak{b}_r)_{r\geqslant 0}$为B左理想的递减序列；由阶 $n$ 的方阵的 $\mathfrak{c}_r$ 集合表示，条目在 $\mathfrak{b}_r$ 中。那么$(\mathfrak{c}_r)_{r\geqslant 0}$就是$\mathbf{M}_n(B)$的左理想的递减序列。特别是，如果环$\mathbf{M}_n(B)$是左阿廷的，那么B也是。

由上可知，对于L中的每一个$i\in I$和每一个扩张$L'$，环$D_i\otimes_LL'$都是左阿廷的。到引理 2 时，每 $i\in I$ 就有 $D_i= L$，这意味着引理 3。

我们将使用下面的引理来证明蕴涵(i)$\Rightarrow$(vi)。

#### 引理 4 {#alg-viii-s13-lem-4 .statement tag=00FJ}

设 A 和 B 为域 K 上的代数，且具有有限生成集合，并令 $K'$ 为 K 的扩张。如果 $K'$ 代数 $A_{(K')}$ 和 $B_{(K')}$ 同构，则存在子扩张$K'$的L，在K上有限生成，使得L-代数$A_{(L)}$和$B_{(L)}$是同构的。

Let $(e_i)_{i\in I}$ and $(f_j)_{j\in J}$ be 有限生成集合 for 代数 A and B, respectively. Let $u$ be 同构的 from $A_{(K')}$ to $B_{(K')}$ and $v$ 逆同构;存在$K'$的子扩展L，在K上有限生成，这样我们对于每个$i\in I$有$u(1\otimes e_i)\in B_{(L)}$，对于每个$j\in J$有$v(1\otimes f_j)\in A_{(L)}$。 Consequently, $u$ sends $A_{(L)}$ into $B_{(L)}$, and $v$ sends $B_{(L)}$ into $A_{(L)}$.诱导的映射$u': A_{(L)}\rightarrow B_{(L)}$和$v': B_{(L)}\rightarrow A_{(L)}$为环同态；他们是逆双射。

让我们完成蕴涵 (i)$\Rightarrow$(vi) 的证明。令 $K'$ 为 K (V, §7, No. 8, p. 45) 的可分闭包。那么 $A_{(K')}$ 是绝对半单代数超过 $K'$。根据 (i)$\Rightarrow$(iv) 的蕴涵，$K'$-代数 $A_{(K')}$ 同构于乘积 $\mathbf{M}_{n_1}(D_1)\times \cdots \times \mathbf{M}_{n_r}(D_r)$，其中 $D_i$ 是有限次数的 $K'$-代数，即域，其中心 $Z_i$ 是 $K'$ 中的可分扩张。 Since $K'$ is separably closed, we have $Z_i= K'$. 命题 3 of VIII、p. 231、域 $D_i$ 是可交换的。因此我们有$D_i= K'$。 We denote K-代数 $\mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$ by B. The $K'$-algebras $A_{(K')}$ and $B_{(K')}$ are isomorphic by the above.在 K 上有限生成的 $K'$ 的每个子外延都是可分的，并且在 K 上有有限次数，因此包含在 $K'$ 的子外延 L 中，即伽罗瓦和 K 上的有限次数 (V, §10, No. 1, p. 57, 命题 2)。因而，其含义是从引理 4 得出的。

蕴涵(vi)$\Rightarrow$(v)是直接的。

#### 推论 1 {#alg-viii-s13-lem-4-cor-1 .statement tag=00FK}

Let K be 交换域, and let $A_1$ and $A_2$ be K-代数.假设$A_1$是绝对半单的。

a) 如果$A_2$ 是半单，那么$A_1\otimes_KA_2$ 也是。

b) 如果$A_2$ 是绝对半单的，那么$A_1\otimes_KA_2$ 也是。

用$Z_1$表示$A_1$的中心，用$Z_2$表示$A_2$的中心。 $A_1\otimes_KA_2$的中心Z等于$Z_1\otimes_KZ_2$除以III, §4, No. 4、p. 468的推论。假设$A_2$为半单；那么 $Z_2$ 是减少的代数（VIII、p. 137、命题 2 和 3）。到定理 1 时，$Z_1$ 是一个 étale，因此可分离 K-代数。由V, §15, No. 2、p. 120、环$Z = Z_1\otimes_KZ_2$中的命题 5 减少；因为$A_1$的有限次数大于K（定理1），所以从VIII、p. 221的命题7得出环$A_1\otimes_KA_2$是半单。

现在假设 $A_2$ 是绝对半单的。设L为K的扩张，则代数$A_{1(L)}$为绝对半单的，代数$A_{2(L)}$为半单。因此，根据a)，代数$A_1\otimes_KA_{2(L)}$为半单。

#### 推论 2 {#alg-viii-s13-lem-4-cor-2 .statement tag=00FL}

设K为可分闭域，设A为绝对半单的K-代数。则存在整数 $r\geqslant 0$ 和严格的正整数 $n_1, . . . , n_r$，使得代数 A 同构于代数 $\prod_{i=1}^r\mathbf{M}_{n_i}(K)$。

通过定理 1，A 同构于形式 $\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$ 的代数（对于整数 $r\geqslant 0$、整数 $n_1, . . . , n_r$ 和有限次数的 K-代数） $D_1, . . . ,D_r$ 是域，并且其中心是 K 的可分扩张，因此等于 K。通过 VIII、p. 231 的命题 3，我们有 $i\in [1, r]$ 的 $D_i= K$。

#### 例 {#alg-viii-s13-n3-exa-1 .statement tag=00FM}

交换K-代数是绝对半单的当且仅当它是 étale 时：这源自定理 1 的属性 (i) 和 (v) 的定义 (V, §6, No. 3, p. 28, 定义 1) 和等价。

### 4. 刻画 / 绝对半单模

#### 命题 4 {#alg-viii-s13-prop-4 .statement tag=00FN}

设 K 为交换域，A K-代数。

a) 设 M 为半单A-模。 A-模 M 是绝对半单的当且仅当每个单模属于对 M 的支持是。

b) 令S为单A-模，令D为其交换子。以下属性是等效的：

(i) A-模 S 为绝对半单的。

(ii) K-代数 D 为绝对半单的。

(iii) K-代数 D 是域，有有限次数大于 K，且其

中心是 K 的可分扩张。

断言 a) 由VIII、p. 229 的命题 1, a) 得出。令S和D如b)中那样，并令L为K的扩张。$A_{(L)}$模$S_{(L)}$为半单当且仅当环$D_{(L)}$为(VIII, p. 222, 命题 8，c))。这就证明了 (i) 和 (ii) 的等价，并且 (ii) 和 (iii) 的定理 1 可以得出，因为 D 是域。

#### 推论 {#alg-viii-s13-n4-cor-1 .statement tag=00RF}

令K为交换域，令$A_1$和$A_2$为K-代数，令$M_1$为绝对半单的$A_1$-模和$M_2$半单$A_2$-模。那么 $M_1\otimes_KM_2$ 是半单模超过环 $A_1\otimes_KA_2$。

模 $M_1$ 是绝对半单的简单 $A_1$ 模块 (命题 4) 中的直和。因此，在模$M_1$和$M_2$很简单的情况下，证明断言就足够了。用 $D_1$ 和 $D_2$ 表示它们的交换子。 K-代数 $D_1$ 是绝对半单的（前述）；由 VIII、p. 234、K-代数 $D_1\otimes_KD_2$ 中的推论 1 得到半单。然后从VIII、p. 215的推论 1 得出$(A_1\otimes_KA_2$)-模块$M_1\otimes_KM_2$是半单。

### 5. 推导半单代数

在这个小节和接下来的小节和接下来的小节和接下来的交换环，A K-代数，B K-代数$A\otimes_KA^o$和$\varepsilon$K-线性映射从B到A由$\varepsilon (x\otimes y) =xy$定义为A中的$x, y$。

回想一下 (III, §4, No. 3, p. 467)，每个 $(A$, A)-双模 P 都可以被视为左B-模，对于 A 中的 $a, a'$ 和 P 中的 $p$，外法则由 $(a\otimes a')p=apa'$ 给出。相反，每个 B-模可以被视为一个$(A,A)$-双模块。我们赋予 A 其规范的 $(A$, A)-双模结构和相应的 B-模结构；我们赋予 B $(A$，A)-双模结构相应的到 B-模 $B_s$。因此我们有

$$
a(x\otimes y)a'= (a\otimes a')(x\otimes y) =ax\otimes ya'
$$

对于 A 中的 $a, a', x, y$，其中乘积 $ya'$ 在代数 A 中计算。

K-线性映射 $\varepsilon$ 是 $(A$ 的同态，A)-双模。

#### 命题 5 {#alg-viii-s13-prop-5 .statement tag=00FO}

以下属性是等效的：

(i) B-模 A 是射影。

(ii) 对于每个$a\in A$，$(A,A)$-双模B满足存在元素$e$以下两个条件：$\varepsilon (e) = 1$和$ae=ea$。

映射 $\varepsilon : B\rightarrow A$ 是满射，因为每个 $a\in A$ 都有 $\varepsilon (a\otimes 1) =a$；它是$(A$，A)-模块中的同态，因此是B-线性映射。如果 B-模 A 是射影的，则存在 $\varepsilon$ 的截面 $s$ (II, §2, No. 2, p. 231, 命题 4)；它是$(A$的同态，A)从A到B的双模。如果我们集合$e=s$(1)，那么对于每个$a\in A$，我们有$\varepsilon (e) =\varepsilon (s(1)) = 1$和$ae=s(a) =ea$。因而 (i) 意味着 (ii)。

相反地​​，设$e$为第(ii)项中B满足条件的元素。 定义映射 $s$ 从 A 到 B 由公式

$$
s(a) =ae=ea \tag{1}
$$

它是$(A$中的同态，A)-模块，我们有$\varepsilon \circ s= 1_A$；在其他字中，$s$是满射映射$\varepsilon$的B线性截面。因而，B-模 A 同构于 $B_s$ (II, §1, No. 9, p. 211, 命题 15) 的直因子子模 $s(A)$，因此是射影 (II, §2, No. 2, p. 231, 命题 4)。这证明(ii)蕴涵(i)。

#### 注 1 {#alg-viii-s13-n5-rem-1 .statement tag=00FP}

设$e=\sum^r_{i=1}a_i\otimes a'_i$为B的元素。命题5第(ii)项中的条件转换为公式

$$
\sum_{i=1}^ra_ia'_i= 1 \tag{2}
$$

(3) 每 $a\in A$ $\sum_{i=1}^raa_i\otimes a'_i=\sum_{i=1}^ra_i\otimes a'_ia$。

当他们满足时，$e$在B中是幂等的。事实上，我们有关系

$$
e^2=\sum_{i=1}^ra_iea'_i=\sum_{i=1}^rea_ia'_i=e
$$

#### 注 2 {#alg-viii-s13-n5-rem-2 .statement tag=00FQ}

令K为交换域，令A为K-代数，令M为A-模。 群 End$_K(M)$ 被赋予了 $(A$, A)-双模结构，定义为

$$
aua'(x) =au(a'x)
$$

每$a, a'\in A$、每$u\in$结束$_K$(M)、每$x\in M$。我们赋予它相关的B-模结构。设$e=\sum^r_{i=1}a_i\otimes a'_i$为命题5的部分(ii)中B满足条件的元素，关系(2)和(3)也是如此。如果$p\in$End$_K(M)$是投影算子，其中像N是M的A-子模，则$ep$是具有相同像的A线性投影算子。

事实上，$ep$的像包含在N中。如果$x$属于包含在N中，那么$a'_ix$也包含在N中，因此我们有$p(a'_ix) =a'_ix$并且

$$
ep(x) =\sum_{i=1}^ra_ia'_ix=x
$$

公式 (2)。我们从公式 (3) 推论出对于每个$a\in A$和每个$x\in M$都有$aep(x) =ep(ax)$，从而证明$ep$是A线性的。

#### 定理 2 {#alg-viii-s13-thm-2 .statement tag=00RG}

设 K 为交换域，A K-代数。以下属性是等效的：

(i) K-代数 A 为绝对半单的。

(ii)K-代数$B = A\otimes_KA^o$为半单。

(iii) B-模 A 是射影。

(iv) 对于每个$a\in A$，存在$(A,A)$双模B满足$\varepsilon (e) = 1$和$ae=ea$的元素$e$。

假设代数 A 是绝对半单的，因此半单。那么代数$A^o$就是半单（VIII，p. 137，命题2），并且从VIII，p. 234的推论1可以得出$B = A\otimes_KA^o$是半单 K-代数。因而，(i) 意味着(ii)。

由于半单环上的每个模都是投影（VIII，p. 138，命题4），（ii）意味着（iii）。

(iii) 和 (iv) 的等价源自命题 5。为了完成证明，让我们证明(iv)蕴涵(i)。令$e=\sum^r_{i=1}a_i\otimes a'_i$为命题5的第(ii)项中B满足条件的元素。令L为域K的扩张；我们必须证明环 $A_{(L)}$ 是半单，或者等效地，每个$A_{(L)}$-模块是半单（VIII，p. 138，命题 4）。设 M 为 $A_{(L)}$ 模，N 为 M 的子模；我们将 M 视为左 $(A$, L) 双模，将 N 视为子双模 (III, §4, No. 3, p. 466)。由于 L 是域，因而 M 中存在L-线性投影算子 $u$ 和像 N。由于与 A 的元素 $a$ 相关的同位$a_M$ 为L-线性，从$A\otimes_KA^o$到End$_L(M)$存在唯一群同态，将元素$a\otimes a'$发送到L-线性映射$x\mapsto au(a'x)$。我们用同态用$v$表示$e$的像；从注 2 可以得出，$v$ 是$A_{(L)}$-线性投影算子，其中像 N。$v$ 的核是 M 的 $A_{(L)}$ 子模，对 N 进行补充。通过推论 2 VIII，p. 56，$A_{(L)}$模M为半单。

#### 注 3 {#alg-viii-s13-n5-rem-3 .statement tag=00FR}

我们知道（VIII，p. 234，推出 1）两个绝对半单代数除交换域之和张量积等于绝对半单的。因而，如果代数 A 是绝对半单的，那么代数 $B = A\otimes_KA^o$ 也是。

### 6. 上同调 / 代数

在这个小节中，K是交换环，A K-代数，B K-代数$A\otimes_KA^o$，以及从B到A的$\varepsilon$K-线性映射，由A中$x, y$的$\varepsilon (x\otimes y) =$$xy$定义。 $n\in \mathbf{N}$，我们用$B_n$表示K-模A的$n+ 2$副本中的K个张量积。我们将其视为$(A$，A)-双模（也视为B-模）；我们赋予它从张量积的第一个因子的左A-模结构推导出来的左A-模的结构以及从右A-模推导出来的右A-模的结构最后因子的结构。特别是，$B_0$ 只是 $(A$，A)-双模 B。

对于每个整数$n\geqslant 1$，我们将双模$d_n^i$中的定义同态用于$i\in [0, n]$和$d_n$，从$B_n$到$B_{n-1}$乘以公式

$$
d_n^i(x_0\otimes  \cdots  \otimes x_{n+1}) =x_0\otimes  \cdots  \otimes x_ix_{i+1}\otimes  \cdots  \otimes x_{n+1} \tag{4}
$$

$i\in [0, n]$ 和

$$
d_n=\sum_{i=0}^n(-1)^id_n^i \tag{5}
$$

我们用$d_0=d^0_0$表示映射$\varepsilon : B_0\rightarrow A$。

令$n$为整数$\geqslant 1$。对于$0\leqslant i < j\leqslant n$，我们有

$$
d_{n-1}^i\circ d_n^j=d_{n-1}^{j-1}\circ d_n^i \tag{6}
$$

由此我们推断

$$
d_{n-1}\circ d_n=\sum_{0\leqslant i<j\leqslant n}(-1)^{i+j}d_{n-1}^i\circ d_n^j+\sum_{0\leqslant j\leqslant i\leqslant n-1}(-1)^{i+j}d_{n-1}^i\circ d_n^j
$$

$$
=\sum_{0\leqslant i<j\leqslant n}(-1)^{i+j}d_{n-1}^{j-1}\circ d_n^i+\sum_{0\leqslant j\leqslant i\leqslant n-1}(-1)^{i+j}d_{n-1}^i\circ d_n^j
$$

因而

$$
d_{n-1}\circ d_n= 0 \tag{7}
$$

令 P 为 $(A$, A)-双模。对于任何整数$n\geqslant 0$，我们用$C^n(A,P)$表示从$A^n$到P的K-多重线性映射的K-模。 映射$\alpha^n: C^n(A,P)\rightarrow$Hom$_B(B_n,P)$将$f\in C^n(A,P)$发送到同态$\alpha^n(f)$，其特征在于

$$
\alpha^n(f) (x_0\otimes  \cdots  \otimes x_{n+1}) =x_0f(x_1, . . . , x_n)x_{n+1} \tag{8}
$$

是同构 / K-模。

我们用$\partial^n$（对于$n \geq 0$）唯一的K-线性映射表示从$C^n(A, P)$到$C^{n+1}(A, P)$，这使得以下图表可交换：

$$
\begin{array}{ccc}
C^n(A, P) & \xrightarrow{\partial^n} & C^{n+1}(A, P) \\
| \downarrow \alpha^n | & & | \downarrow \alpha^{n+1} | \\
\operatorname{Hom}_B(B_n, P) & \xrightarrow{\operatorname{Hom}(d_{n+1}, 1_P)} & \operatorname{Hom}_B(B_{n+1}, P).
\end{array}
$$

到定义，我们有

$$
(9) \quad (\alpha^{n+1} \circ \partial^n)(f) = \alpha^n(f) \circ d_{n+1}
$$

对于每个$f \in C^n(A, P)$。在其他字中，我们有

$$
\partial^n(f)(x_0, \ldots, x_n) = \alpha^n(f)(d_{n+1}(1 \otimes x_0 \otimes \cdots \otimes x_n \otimes 1))
$$

对于 A 中的 $x_0, \ldots, x_n$ 和 $C^n(A, P)$ 中的 $f$，即

$$
\begin{align*}
(10) \quad \partial^n(f)(x_0, \ldots, x_n) &= x_0 f(x_1, \ldots, x_n) \\
&+ \sum_{i=0}^{n-1} (-1)^{i+1} f(x_0, \ldots, x_{i-1}, x_i x_{i+1}, x_{i+2}, \ldots, x_n) \\
&\phantom{=} + (-1)^{n+1} f(x_0, \ldots, x_{n-1}) x_n.
\end{align*}
$$

由(7)和(9)，我们有

$$
(11) \quad \partial^{n+1} \circ \partial^n = 0 \qquad \text{for every } n \geq 0.
$$

我们用$H^0(A, P)$表示K-模$\operatorname{Ker} \partial^0$，对于$n \geq 1$，K-模$\operatorname{Ker} \partial^n / \operatorname{Im} \partial^{n-1}$用$H^n(A, P)$表示。我们与 P 认同 K-模 $C^0(A, P)$，我们有 $C^1(A, P) = \operatorname{Hom}_K(A, P)$。 $n \leq 2$ 的映射 $\partial^n$ 由公式给出

$$
\begin{align*}
(12) \quad \partial^0(p)(a) &= ap - pa \qquad \text{for every } p \in P, \\
(13) \quad \partial^1(f)(a, a') &= af(a') - f(aa') + f(a)a' \qquad \text{for } f \in C^1(A, P), \\
(14) \quad \partial^2(f)(a, a', a'') &= af(a', a'') - f(aa', a'') + f(a, a'a'') - f(a, a')a''
\end{align*}
$$

对于$f \in C^2(A, P)$。

因此，$H^0(A, P)$是元素$p$的P由……组成的K子模，使得$ap = pa$对于每个$a \in A$，$H^1(A, P)$是从A到P的K-导数的K-模$\operatorname{Der}_K(A, P)$的商 (III, §10, No. 2, p. 553) 由形式 $a \mapsto ap - pa$ 的推导和 $p \in P$ 的 K 子模块由……组成（称为 *内部推导*）。

### 7. 上同调 / 绝对半单代数

#### 命题 6 {#alg-viii-s13-prop-6 .statement tag=00FS}

设 K 为交换环，A K-代数。设$e=\sum^r_{i=1}a_i\otimes a'_i$为VIII、p. 236的命题5的第(ii)项中的$B = A\otimes_KA^o$满足条件的元素。对于任何整数$n\geqslant 1$和$C^n(A,P)$的任何元素$f$，我们用公式定义的$C^{n-1}(A,P)$的$\gamma^n(f)$元素表示

$$
\gamma^n(f)(x_1, . . . , x_{n-1}) =\sum_{i=1}^ra_if(a'_i, x_1. . . , x_{n-1}) \tag{15}
$$

然后我们有

$$
\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f)) =f \tag{16}
$$

对于每个整数$n\geqslant 1$和每个$f\in C^n(A,P)$。

#### 注 1 {#alg-viii-s13-n7-rem-1 .statement tag=00SF}

$*$态射$\partial^n: C^n(A,P)\rightarrow C^{n+1}(A,P)$定义$(C(A,P), \partial )$K-模（X, §2，n$^o1$，p. 24）。 映射 $\gamma_n$ 因此定义从这个复合体到自身的同伦，将 0 连接到 Id$_{C(A,P)}$ (X, §2, n$^o4$, p. 32, 定义 $4$)$.*$

我们保留No.6中的记号。对于每整数 $n\geqslant 0$，我们定义映射 $h_n: B_n\rightarrow B_{n+1}$ 公式

$$
h_n(x) =d^1_{n+2}(e\otimes x) =\sum_{i=1}^ra_i\otimes a'_ix
$$

它是 $(A$ 的同态，A)-双模 (公式 (3))。

#### 引理 5 {#alg-viii-s13-lem-5 .statement tag=00FT}

我们有关系

$$
d_{n+1}\circ h_n+h_{n-1}\circ d_n= 1_{B_n} \tag{17}
$$

每$n\geqslant 1$。

让$x\in B_n$；我们有

$$
(d_{n+1}\circ h_n)(x) = (d_{n+1}\circ d^1_{n+2})(e\otimes x)
$$

$$
= (d^0_{n+1}\circ d^1_{n+2})(e\otimes x)-\sum^{n+2}_{i=2}(-1)^i(d_{n+1}^{i-1}\circ d^1_{n+2})(e\otimes x)
$$

所以，通过公式 (6)，

$$
(d_{n+1}\circ h_n)(x) = (d^0_{n+1}\circ d^0_{n+2})(e\otimes x)-\sum^{n+2}_{i=2}(-1)^i(d^1_{n+1}\circ d_{n+2}^i)(e\otimes x)
$$

但我们有

$$
(d^0_{n+1}\circ d^0_{n+2})(e\otimes x) =\varepsilon (e)x=x
$$

性质 (ii) 命题 5 VIII、p. 236 以及$i\geqslant 2$，

$$
d^i_{n+2}(e\otimes x) =e\otimes d^{i-2}_n(x)
$$

这给出了

$$
(d_{n+1}\circ h_n)(x) =x-d^1_{n+1}(e\otimes d_n(x)) =x-h_{n-1}\circ d_n(x)
$$

因此公式 (17)。

我们可以使用引理 5 来完成命题 6 的证明。令 $n$ 为整数 $\geqslant 1$ 和 $C^n(A,P)$ 的 $f$ 元素。到构造，我们已经

$$
\alpha^{n-1}(\gamma^n(f)) =\alpha^n(f)\circ h_{n-1} \tag{18}
$$

因而，通过公式 (9) 和 (18)，

$$
\alpha^n(\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f))) =\alpha^{n-1}(\gamma^n(f))\circ d_n+\alpha^{n+1}(\partial^n(f))\circ h_n
$$

$$
=\alpha^n(f)\circ h_{n-1}\circ d_n+\alpha^n(f)\circ d_{n+1}\circ h_n
$$

$$
=\alpha^n(f)
$$

其中最后一个等式由 (17) 得出。由于 $\alpha^n$ 是双射，因此命题遵循。

#### 定理 3 {#alg-viii-s13-thm-3 .statement tag=00FU}

设 K 为交换环，A K-代数，P 为 $(A,A)$ 双模。假设 $(A\otimes_KA^o)$ 模 A 是射影的。然后，每整数 $n\geqslant 1$ 就有 $H^n(A,P) = 0$。

我们必须证明对于每个整数$n\geqslant 1$，$C^n(A,P)$和$\partial^n(f) = 0$的每个元素$f$是形式$\partial^{n-1}(g)$对于元素$g$ $C^{n-1}(A,P)$。到命题 5 时，这是命题 6 中的直接的推论。

#### 推论 {#alg-viii-s13-n7-cor-1 .statement tag=00FV}

从 A 到 P 的每个 K 导数都是内部。

这是等式$H^1(A,P) = 0$的翻译。

#### 注 2 {#alg-viii-s13-n7-rem-2 .statement tag=00FW}

特别地，当K为域且A绝对半单的K-代数(VIII、p. 238、定理2)时，满足定理3中的假设。

#### 注 3 {#alg-viii-s13-n7-rem-3 .statement tag=00FX}

假设 K-模 A 是射影的。 定理 3 也可以证明如下。复数 $(\bigoplus_{n\geqslant 0}B_n, d)$ 和同态 $\varepsilon : B_0\rightarrow A$ 定义 B-模 A 的投影分辨率；因而，对于每个$n\geqslant 0$，K-模$H^n(A,P)$同构于Ext$^n_B(A,P)$（X, §6，n$^o1$，p. 100，定理1）。如果 B-模 A 是射影的，则 K-模 Ext$^n_B(A,P)$ 对于 $n\geqslant 1$ 来说是零 (X, §5, n$^o3$, p. 88, 推论 de la 命题 5)，这意味着$H^n(A,P)$ 是零。相反，如果对于每个 $(A$, A)-双模 P，$H^1(A,P)$ 都是零，则 B-模 A 是射影 (X, §5, n$^o5$, p. 93, 命题 $10$)$.*$

### 8. 分裂 / 阿廷代数

在这个小节中，K是交换环，A是K-代数。令$\mathfrak{r}$为A的根基。我们用$\overline{A}$表示商代数$A/\mathfrak{r}$，并用$\pi$表示从A到$\overline{A}$的典范映射。我们对 A 的子代数 S 感兴趣，使得$A = S\oplus \mathfrak{r}$。

对于A中的$\alpha , \beta$，我们用$\pi$满足$s(\alpha \beta ) =$$s(\alpha )s(\beta )$的K-线性截面$s$的Σ集合表示。注意，这样的截面必然满足$s(1) = 1$（在其他情况下） 字，$s$是环同态）：我们确实有$s(1)^2=s$（1），并且$s(1)$是可逆的，因为它属于到$1 +\mathfrak{r}$（VIII，p. 156， 定理 1)。如果$s$是Σ的元素，那么$s$的像S就是A的子代数，并且我们有$A = S\oplus \mathfrak{r}$。相反，如果 S 是 A 的子代数，使得 $A = S\oplus \mathfrak{r}$，则 $\pi$ 到 S 的限制是双射，并且 Σ 与像 S 的逆双射定义元素。

根据 Jacobson 的定理（前述），$1 +\mathfrak{r}$ 的每个元素在 A 中都是可逆的。我们将形式 $a\mapsto xax^{-1}$ 的 A 的内自同构与 $x\in 1 +\mathfrak{r}$ 称为特殊的自同构。

#### 命题 7 {#alg-viii-s13-prop-7 .statement tag=00FY}

假设 $(A\otimes_K\overline{A}^o)$-模 $\overline{A}$ 是射影的。

a) 设$S_1$和$S_2$为满足$A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$中的子代数。 A 存在一个特殊的自同构，将 $S_1$ 转换为 $S_2$。

b) 假设 $\pi$ 具有 K 线性截面并且 A 的根基 $\mathfrak{r}$ 是幂零的。那么存在满足$A = S\oplus \mathfrak{r}$的子代数S。

令$S_1$和$S_2$如a)中所示。设$s_1$和$s_2$为集合Σ相应的到子代数$S_1$和$S_2$的元素。令 $\varepsilon$ 为 K-线性映射，从 $A\otimes_KA$ 到由 $\varepsilon (a\otimes b) =ab$ 给出的 A。由VIII、p. 236中的命题5和VIII、p. 237中的注1，存在$\overline{A}\otimes_KA$满足$\sum^r_{i=1}\alpha_i\alpha '_i= 1$中的元素$e=\sum^r_{i=1}\alpha_i\otimes \alpha '_i$每$\alpha \in A$对应$\sum^r_{i=1}\alpha \alpha_i\otimes \alpha '_i=\sum^r_{i=1}\alpha_i\otimes \alpha '_i\alpha$。 集合$x=\sum^r_{i=1}s_1(\alpha_i)s_2(\alpha '_i)$。我们有 $\pi (x) =\sum^r_{i=1}\alpha_i\alpha '_i= 1$，因此有 $x\in 1 +\mathfrak{r}$。令 $\alpha$ 为 A 的元素。我们有

$$
s_1(\alpha )x=\sum_{i=1}^rs_1(\alpha \alpha_i)s_2(\alpha '_i) = (\varepsilon \circ (s_1\otimes s_2))(\sum_{i=1}^r\alpha \alpha_i\otimes \alpha '_i)
$$

$$
= (\varepsilon \circ (s_1\otimes s_2))(\sum_{i=1}^r\alpha_i\otimes \alpha '_i\alpha )=\sum_{i=1}^rs_1(\alpha_i)s_2(\alpha '_i\alpha ) =xs_2(\alpha )
$$

等式$x^{-1}S_1x= S_2$紧随其后，给出断言a)。

在b)的假设下，进一步假设$\mathfrak{r}^2= 0$。在这种情况下，$(A$，A)-双模$\mathfrak{r}$被$\mathfrak{r}$消灭，因此我们将其视为$(A$，A)-双模。 选择 $\pi$ 的 K 线性截面 $\sigma$。我们有

(19) $\alpha x=\sigma (\alpha )x$ 和 $x\alpha =x\sigma (\alpha )$

对于 $\alpha \in \overline{A}$ 和 $x\in \mathfrak{r}$。 集合

$$
\varphi (\alpha , \beta ) =\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta ) \tag{20}
$$

对于$\alpha , \beta \in A$。我们有关系 $\pi (\varphi (\alpha , \beta )) =\alpha \beta -\alpha \beta = 0$ 对应 $\alpha , \beta \in A$。因此，$\varphi$定义元素$C^2(A,\mathfrak{r})$。令$\alpha , \beta , \gamma$为A的元素；鉴于(19)，我们有

$$
\partial^2\varphi (\alpha , \beta , \gamma ) =\alpha \varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\gamma
$$

$$
=\sigma (\alpha )\varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\sigma (\gamma )
$$

$$
=\sigma (\alpha )(\sigma (\beta \gamma )-\sigma (\beta )\sigma (\gamma ))-\sigma (\alpha \beta \gamma ) +\sigma (\alpha \beta )\sigma (\gamma ) +\sigma (\alpha \beta \gamma )
$$

$$
-\sigma (\alpha )\sigma (\beta \gamma )-(\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta ))\sigma (\gamma )
$$

$$
= 0
$$

到 VIII、p. 242、K-模 $H^2(A,\mathfrak{r})$ 中的定理 3 减少到零。因此，存在$C^1(A,\mathfrak{r})$的元素$\psi$使得$\partial^1\psi =\varphi$，在其他字中，使得我们有

(21) $\overline{A}$ 中的 $\alpha , \beta$ 为 $\varphi (\alpha , \beta ) =\alpha \psi (\beta )-\psi (\alpha \beta ) +\psi (\alpha )\beta$。

我们有$\psi (\alpha )\psi (\beta ) = 0$，因为$\mathfrak{r}^2$是零；由(19)和(20)，我们推导出(22)$(\sigma +\psi )(\alpha \beta ) = (\sigma +\psi )(\alpha )(\sigma +\psi )(\beta )$，

使得$\pi$属于到Σ的K-线性截面$\sigma +\psi$。它的像是A的子代数S，使得$A = S +\mathfrak{r}$。

现在让我们证明一般情况下S的存在性。我们通过归纳对至少整数$p\geqslant 1$进行推理，使得$\mathfrak{r}^p= 0$；案例 $p= 1$ 是微不足道的。假设$p\geqslant 2$和集合$A'= A/\mathfrak{r}^{p-1}$。 $A'$的根基$\mathfrak{r}'$等于$\mathfrak{r}/\mathfrak{r}^{p-1}$（VIII、p. 155的命题 5），因此满足${\mathfrak{r}'}^{p-1}= 0$，且代数$A'/\mathfrak{r}'$与$\overline{A}= A/\mathfrak{r}$同构因此是绝对半单的。到归纳假设，存在$A'$的子代数$S'$使得$A'= S'\oplus \mathfrak{r}'$。那么$S'$是形式$A''/\mathfrak{r}^{p-1}$，其中$A''$是包含$\mathfrak{r}^{p-1}$的子代数，我们有

$$
A = A''+\mathfrak{r},\mathfrak{r}^{p-1}= A''\cap \mathfrak{r} \tag{23}
$$

代数 $A''/\mathfrak{r}^{p-1}$ 同构于 $A'/\mathfrak{r}'$；我们有 $(\mathfrak{r}^{p-1})^2= 0$，所以 $\mathfrak{r}^{p-1}$ 是 $A''$ 的根基。根据我们刚刚处理的情况，存在$A''$的子代数 S，使得$A''= S\oplus \mathfrak{r}^{p-1}$；我们从 (23) 推导出关系 $A = S\oplus \mathfrak{r}$。

#### 推出 1（韦德伯恩的定理）{#alg-viii-s13-prop-7-cor-1 .statement tag=00S8}

设K为A的交换域、A K-代数、A的$\mathfrak{r}$根基。假设K-代数$A/\mathfrak{r}$为绝对半单的。

a) 设$S_1$和$S_2$为满足$A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$中的子代数。 A 存在一个特殊的自同构，将 $S_1$ 转换为 $S_2$。

b) 如果$\mathfrak{r}$幂零，则存在满足 A = $S\oplus \mathfrak{r}$的子代数 S。

这是从VIII、p. 238 的命题 7 和定理 2 得出的。

#### 推出 2 {#alg-viii-s13-prop-7-cor-2 .statement tag=00FZ}

令A为有限次数除以完美域K的交换代数，并令$\mathfrak{r}$为其根基。 A 存在唯一的子代数 S，使得 $A = S\oplus \mathfrak{r}$。而且，S同构于有限次数的K的有限多个扩张的乘积。

K-代数 $A/\mathfrak{r}$ 是半单 (VIII, p. 173, 命题 1) 并且有有限次数；它是绝对半单的，因为域 K 是完美的（VIII、p. 232、定理 1）。由于理想 $\mathfrak{r}$ 是幂零的且 A 是可交换的，因此 S 的存在性和唯一性则从推论 1 得出。由于 S 是半单且可交换且具有有限次数，因此最后一个断言是命题 3 的推论 VIII，p. 137。

#### 注 1 {#alg-viii-s13-n8-rem-1 .statement tag=00G0}

假设 $A/\mathfrak{r}$ 是绝对半单的在推论 1 (VIII、p. 246、习题 4) 中是必需的。

#### 注 2 {#alg-viii-s13-n8-rem-2 .statement tag=00G1}

假设 A 是阿廷代数超过域 K。如果 A 是可交换的，那么我们可以证明 (VIII, p. 180, 习题 9) A 同构于代数 $A_1\times  \cdots  \times A_n$ 的乘积，使得 $A_i/\mathfrak{R}(A_i)$ 是每 $i$ 域。相反，如果 A 不可交换，则 A 可能不会与代数 $A_1\times  \cdots  \times A_n$ 的乘积同构，使得对于每个 $i$ (VIII, p. 247, 习题)，$A_i/\mathfrak{R}(A_i)$ 是一个简单的环 5）。

### 习题{#alg-viii-s13-exercises}

参见[习题为 § 13](exercises/s13/)。
