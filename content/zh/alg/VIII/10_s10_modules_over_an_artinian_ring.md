---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 10
section_title: Modules over an Artinian Ring
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.173-A VIII.181
pdf_pages: 0190-0198
extraction: native
subsections:
    - "no": 1
      title: The Radical of an Artinian Ring
      page: 173
      pdf_page: 190
    - "no": 2
      title: Modules over an Artinian Ring
      page: 174
      pdf_page: 191
    - "no": 3
      title: Projective Modules over an Artinian Ring
      page: 175
      pdf_page: 192
statements: 12
exercises: 11
content_sha256: f1ff059ee8dfb4f2484cfeebe854d915a7cda5e565c4ec5ea8605f84f4ccb835
translated_from: content/en/alg/VIII/10_s10_modules_over_an_artinian_ring.md
translation_method: google
source_content_sha256: f88ff60a0976a0441aed75f5328135625983a714fc53ed6dc1504425eb26923f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 9fe1eebeb477e67767c61b6944ad2a8ca93a5fae9bd68e24043e070166714377
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 10。 模超过阿廷环

### 1. 阿廷环的根

#### 命题 1 {#alg-viii-s10-prop-1 .statement tag=00C5}

设 A 为左阿廷的环。 A 的根基 $\mathfrak{r}$ 是 A 的最大的幂幂双面理想，环 $A/\mathfrak{r}$ 是半单。

我们知道 (VIII, p. 156, 定理 1) A 的每一个幂零双面理想都包含在 $\mathfrak{r}$ 中。让我们证明$\mathfrak{r}$是幂零的。由于双面理想$\mathfrak{r}^n$的环A是左阿廷的且序列是递减，因此存在整数$p\geqslant 0$使得我们有$\mathfrak{r}^p=\mathfrak{r}^{p+1}$。由于 A 为阿廷的，A-模 $A_s$ 具有有限长度（VIII、p. 6、定理 1），因此为诺特。因而，左理想$\mathfrak{r}^p$是有限生成的。通过中山引理（定理 2 of VIII，p. 158），得出$\mathfrak{r}^p= 0$。

环 $A/\mathfrak{r}$ 没有根基 (VIII, p. 155, 命题 5);因为它是左阿廷的，所以它是半单（VIII，p. 154，命题 4）。

#### 推论 1 {#alg-viii-s10-prop-1-cor-1 .statement tag=00C6}

环是半单当且仅当它是左阿廷的并且除了 0 之外没有幂等两侧理想。

半单环是左阿廷的并且没有根基 (VIII、p. 154、命题 4)；因而，除了 0 之外，它没有幂等双面理想。逆命题由命题 1 得出。

#### 推论 2 {#alg-viii-s10-prop-1-cor-2 .statement tag=00C7}

在左阿廷的环 A 中，根基由元素 $x$ 组成，使得 axe 对于 A 中的每个 $a$ 都是幂零的。

如果 A 是左阿廷的，则根基是幂零双面理想 (命题 1)。每个左零理想都包含在 Jacobson 的定理（VIII、p. 156、定理 1）的根基中。接下来是推论2。

### 2. 模超过阿廷环

#### 命题 2 {#alg-viii-s10-prop-2 .statement tag=00C8}

设 A 为左阿廷的环。对于每个 A-模 M，以下属性是等效的：

(i) M 为半单。

(ii) M 没有根基。

(iii) M 被 A 的根基 $\mathfrak{r}$ 湮灭。

我们知道 (i) 蕴含 (ii) (VIII, p. 153, 命题 3)。另一方面，$\mathfrak{r}M$包含在M的根基中（VIII，p. 158，命题6），因而（ii）蕴涵（iii）。

假设A-模 M 被$\mathfrak{r}$ 湮灭。我们可以将其视为模超过环$A/\mathfrak{r}$。现在，环$A/\mathfrak{r}$是半单（VIII，p. 173，命题1），并且半单环上的每个模是半单（VIII， p. 138、命题 4)。因而，M 是半单模超过环 $A/\mathfrak{r}$ 且更不必说超过环 A。因而 (iii) 意味着 (i)。

#### 推论 {#alg-viii-s10-n2-cor-1 .statement tag=00C9}

设 A 为左阿廷的环。对于每个 A-模 M，M 的根基等于 $\mathfrak{r}M$。

M 包含于 $\mathfrak{r}M$ 的根基 $\mathfrak{R}(M)$（VIII、p. 158、命题 6）。而且，A-模$M/\mathfrak{r}M$被$\mathfrak{r}$湮灭。因而，到命题 2 时，它就没有根基，这意味着 $\mathfrak{R}(M)\subset \mathfrak{r}M$ (VIII, p. 152, 推论 1, c))。

#### 命题 3 {#alg-viii-s10-prop-3 .statement tag=00CA}

令A和B为从A到B的环和$f$同态，使得B由B中$f(A)$的并和$f(A)$的交换子$f(A)'$生成。令M为左B-模。假设环 A 是左阿廷的或 A-模 $f_*(M)$ 由 M 通过限制标量 (II, §1, No. 13, p. 221) 推导出来是有限生成的。那么我们就有$\mathfrak{R}_A(f_*(M))\subset \mathfrak{R}_B(M)$。

令 S 为单B-模。假设 A 是左阿廷的或 A-模 $f_*(S)$ 是有限生成的。我们将证明$f_*(S)$没有根基。对于每个$b\in f(A)'$，位似$b_S$是A-模$f_*(S)$的自同态，因此保留$\mathfrak{R}_A(f_*(S))$（VIII，p. 152，命题1）。由于B是由$f(A)\cup f(A)'$生成的，根基$\mathfrak{R}_A(f_*(S))$是S的B-子模，因此等于0或S。如果$f_*(S)$是有限生成A-模，那么我们有$\mathfrak{R}_A(f_*(S))\not=f_*(S)$（VIII，p. 153， 命题2)。如果环 A 是左阿廷的，则我们有 $\mathfrak{R}_A(f_*(S)) =f(\mathfrak{r})S$，其中 $\mathfrak{r}$ 是 A 的根基（VIII、p. 174、推论的命题 2），并且从 $\mathfrak{r}$ 开始是 A 的幂幂双面理想 (VIII, p. 173, 命题 1)，我们不能有 $S =f(\mathfrak{r})S$。因而，在这两种情况下我们都有 $\mathfrak{R}_A(f_*(S)) = 0$。

令 $u$ 为从 M 到简单 M 模 S 的非零的 B-线性映射。 映射 $u$ 是满射；因而，如果 $f_*(M)$ 是有限生成的，那么 $f_*(S)$ 也是有限生成的。在命题 3 的假设下，A-模$f_*(S)$没有根基，$u$是从$f_*(M)$到$f_*(S)$的A-线性映射。因而，$u$包含于$\mathfrak{R}_A(f_*(M))$中的核乘以VIII中的命题1，p. 152。由于$u$是任意的，所以我们有$\mathfrak{R}_A(f_*(M))\subset \mathfrak{R}_B(M)$。

#### 推论 {#alg-viii-s10-n2-cor-2 .statement tag=00CB}

设 A 为交换环，B 为 A 上的代数。假设环 A 为阿廷的或 B 为有限生成A-模。然后我们就有$\mathfrak{R}(A)B\subset \mathfrak{R}(B)$。

到命题 3，根基 $\mathfrak{R}_A(B_s)$包含在$\mathfrak{R}_B(B_s)$中，这只不过是环 B 的根基。此外，我们还有$\mathfrak{R}(A)B\subset \mathfrak{R}_A(B_s)$到VIII、p. 158的命题 6。接下来是推论。

### 3. 投射模超过阿廷环

#### 命题 4 {#alg-viii-s10-prop-4 .statement tag=00CC}

每个模超过左阿廷的环都有一个投影覆盖。

设 A 为左阿廷的环，M 为 A 上的模。A 的根基 $\mathfrak{r}$ 是幂幂双面理想，环 $A/\mathfrak{r}$ 为半单 (VIII, p. 173, 命题1)。由此可见，$A/\mathfrak{r}$模$M/\mathfrak{r}M$是射影的。 断言然后从命题 11 of VIII、p. 164 开始。

#### 命题 5 {#alg-viii-s10-prop-5 .statement tag=00CD}

设 A 为左阿廷的环，$\mathfrak{r}$ 为根基。

a) 令 P 为射影 A-模。用 $u$ 表示从 P 到 $P/\mathfrak{r}P$ 的典范映射。那么$(P, u)$是$P/\mathfrak{r}P$的投影覆盖。特别是，当且仅当 $P/\mathfrak{r}P$ 时，A-模 P 是有限生成的。

b) 令 M 为模大于环 $A/\mathfrak{r}$。那么M，被视为A-模，有一个投影覆盖。如果$(P, u)$是这样的射影覆盖，那么当经过到商时，$u$诱导同构从$P/\mathfrak{r}P$到M。而且，P不可分解当且仅当M是简单的。

c) 设 M 和 $M'$ 为模大于环 $A/\mathfrak{r}$。令$(P, u)$和$(P', u')$为A-模M和$M'$的投影覆盖。则 M 和 $M'$ 同构当且仅当 P 和 $P'$ 同构的。

A 的根基 $\mathfrak{r}$ 是幂幂双面理想 (VIII, p. 173, 命题 1)。 断言 a) 因此从VIII、p. 163 的推论 1 和VIII、p. 161 的注 2 得出。

让我们证明断言 b)。 M 的射影覆盖$(P, u)$ 的存在从命题 4 和同构从$P/\mathfrak{r}P$ 到VIII、p. 162 的命题 9 的M。由于环$A/\mathfrak{r}$是半单，模超过这个环是不可分解的当且仅当它是简单的。 最后一个断言则由推论 2 of VIII、p. 160 得出。

让我们证明c）。设$f$为同构，从P到$P'$；它从$P/\mathfrak{r}P$到$P'/\mathfrak{r}P'$诱导同构$\overline{f}$。通过b)，这些商分别同构于M和$M'$。因此，M 与 $M'$ 同构的。相反，通过VIII、p. 161的命题 8，从M到$M'$提升到同构$\widetilde{f}$，每同构$f$从P到$P'$，使得$f\circ u=u'\circ \widetilde{f}$。

#### 推论 {#alg-viii-s10-n3-cor-1 .statement tag=00CE}

对于射影A-模的每个类 P，将模$P/\mathfrak{r}P$的类$\varphi (P)$与环$A/\mathfrak{r}$相关联。 模（或有限生成模）在环$A/\mathfrak{r}$上的每个类都是形式$\varphi (P)$，对于射影A-模（或有限生成的射影）的唯一类P A-模）。

设 A 为左阿廷的环，$\mathfrak{r}$ 根基。用 $\mathscr{S}$ 表示单A-模类集合；它是有限的（VIII，p. 51）。通过VIII、p. 174的命题2，可以在半单环$A/\mathfrak{r}$上与单模类的集合进行规范地识别。对于每个$\lambda \in \mathscr{S}$，令$S_{\lambda}$为类$\lambda$的单A-模，并且选择为$S_{\lambda}$的投影覆盖$(P_{\lambda}, u_{\lambda})$（VIII，p. 175，命题4）。到命题 5，A-模 $P_{\lambda}$ 是射影且不可分解的，并且 $u_{\lambda}$ 定义同构从 $P_{\lambda}/\mathfrak{r}P_{\lambda}$ 到 $S_{\lambda}$。此外，如果 P 是射影且不可分解的 A-模，则存在唯一的 $\lambda \in \mathscr{S}$，使得 P 同构于 $P_{\lambda}:$；它是唯一的 $\lambda \in \mathscr{S}$，使得 $P/\mathfrak{r}P$ 同构于 $S_{\lambda}$。

#### 命题 6 {#alg-viii-s10-prop-6 .statement tag=00CF}

设 A 为左阿廷的环，$\mathfrak{r}$ 为根基。令 P 为射影 A-模。

a) A-模 $\overline{P}= P/\mathfrak{r}P$ 是半单，A-模 P 与 $\bigoplus_{\lambda\in\mathscr{S}}P^{([P:\lambda])}_{\lambda}$ 同构的。

b) 令 $(Q_i)_{i\in I}$ 为 P 与直和 P 的不可分解射影子模族。那么对于 $i\in I$ 的集合 $I(\lambda )$ 的每个 $\lambda \in \mathscr{S}$，基数使得 $Q_i$ 同构于$P_{\lambda}$等于$[P :\lambda ]$。

$\overline{P}$ 是半单是从命题 2 (VIII, p. 174) 得出的。 A-模 $Q =\oplus_{\lambda\in\mathscr{S}}P^{([P:\lambda])}_{\lambda}$ 是投影。由于$P_{\lambda}/\mathfrak{r}P_{\lambda}$与$S_{\lambda}$同构的，所以商$Q/\mathfrak{r}Q$同构于$\oplus_{\lambda\in\mathscr{S}}S^{([P:\lambda])}_{\lambda}$，即$\overline{P}= P/\mathfrak{r}P$。到命题 5，A-模 P 和 Q 同构的。

假设给定一个射影且不可分解的子模族$(Q_i)_{i\in I}$和直和P。到命题5，A-模$Q_i/\mathfrak{r}Q_i$对于每个$i\in I$都是简单的。对于$\lambda \in \mathscr{S}$，用$i\in I$的$I(\lambda )$集合表示，使得$Q_i/\mathfrak{r}Q_i$与$S_{\lambda}$同构的，因此与$P_{\lambda}/\mathfrak{r}P_{\lambda}$同构的；它也是$i\in I$的集合，使得$Q_i$与$P_{\lambda}$同构的。由于$\overline{P}= P/\mathfrak{r}P$是家庭$(Q_i/\mathfrak{r}Q_i)_{i\in I}$的直和，我们有VIII、p. 32中的定理 1张卡(I($\lambda$))$= [P :\lambda ]$。

#### 例 {#alg-viii-s10-n3-exa-1 .statement tag=00CG}

取P等于$A_s$。 对于$\lambda \in \mathscr{S}$，用$D_{\lambda}$表示单A-模$S_{\lambda}$的交换子的对数域，并用$m(\lambda )$表示$S_{\lambda}$的维数视为右向量空间超过域$D_{\lambda}$。 我们知道$m(\lambda )$等于重数$[A_s/\mathfrak{r}A_s:\lambda ]$（VIII，p. 143，命题11）。 因而，A-模$A_s$同构于$\oplus_{\lambda\in\mathscr{S}}P^{m(\lambda)}_{\lambda}$。

### 习题{#alg-viii-s10-exercises}

参见[习题为 § 10](exercises/s10/)。
