---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 7
section_title: Irreducible representations of connected compact Lie groups
lang: zh
source: lie-vii-ix
book_pages: 347-359, 414-417
pdf_pages: 0354-0366, 0421-0424
extraction: native
subsections:
    - "no": 1
      title: DOMINANT CHARACTERS
      page: 347
      pdf_page: 354
    - "no": 2
      title: HIGHEST WEIGHT OF AN IRREDUCIBLE REPRESENTATION
      page: 348
      pdf_page: 355
    - "no": 3
      title: THE RING R(G)
      page: 351
      pdf_page: 358
    - "no": 4
      title: CHARACTER FORMULA
      page: 353
      pdf_page: 360
    - "no": 5
      title: DEGREE OF IRREDUCIBLE REPRESENTATIONS
      page: 356
      pdf_page: 363
    - "no": 6
      title: CASIMIR ELEMENTS
      page: 358
      pdf_page: 365
statements: 28
exercises: 8
content_sha256: 8c387c18aa7f6c1a1e87a8fc6cfa3297e47d1a92e004a4b769ddf23630b85ad9
translated_from: content/en/lie/IX/07_s7_irreducible_representations_of.md
translation_method: google
source_content_sha256: 375df81cdee840da6e0b458ac2f5db5264d7654fce07a342d3dce277a3f78519
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 426f6d8ab8ec6ef21236b8d9b0ba8f6fb4ef6480eb9c4d5c92aa39f0bfbb70c2
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 7。 不可约表示已连接紧李群

我们保留 §6 中的记号。 G 的表示是从 G 到群 $\mathbf{G}\mathbf{L}(V)$ 的连续（因此是解析的）同态，其中 V 是有限维复数向量空间。 G 的每个表示都是半单 (§1, no. 1)。

$\mathfrak{t}($§5, no. 2）的选择室C），并放入$\Gamma (T)_{++}=\overline{C}\cap \Gamma (T)$。

### 1. 优势特征

用X(T)的元素$\lambda$的$X_+$集合表示，使得$\langle \lambda , x\rangle  \geq 0$对于所有$x\in \Gamma (T)_{++}$，即线性形式$\delta (\lambda ) :\mathfrak{t}_{\mathbf{C}}\rightarrow \mathbf{C}$映射室C $\mathfrak{t}$至$i\mathbf{R}_+$。

给出 X(T) 有序的群结构，其正元素是$X_+$的正值；输入$R_+= R(G,T)\cap X_+$和$R_-=-R_+$。 $R_+$中的元素称为正根，$R_-$称为负根；每个根要么是正数，要么是负数（第 VI, §1, no. 6 章，第 3 章）。不是两个正根中的和的正根被称为简单；每个正数根都是简单根的和（前述）；由根、子群生成的X(T)的子群的简单根形式基可以用$X(T/C(G))$(§4, no. 4)来识别；关于简单的根生成 Weyl 群 $W = W_G(T)$ 的思考（第 VI, §1, no. 5，第 2 章）。

#### 引理 1 {#lie-ix-s7-lem-1 .statement tag=01FZ}

设$\lambda$为X(T)中的元素。以下条件是等效的：

(i) $\lambda -w(\lambda )\geq 0$（或$>0$）对于所有$w\in W$，使得$w\not= 1$；

(ii) 对于所有$w\in W$，使得$w\not= 1,\lambda -w(\lambda )$是线性组合，并且简单根的正系数（分别为正系数，并非所有零）；

(iii) 对于每个正根 $\alpha$，$\langle \lambda , K_{\alpha}\rangle  \geq 0$（或$>0$）；

(iv) 对于每个简单的根 $\alpha$，$\langle \lambda , K_{\alpha}\rangle  \geq 0$（或 $>0$）。

等价如果 (iii) 和 (iv) 是直接的。由于$K_{\alpha}$的集合可以与$R(G,T) ($§4, no. 5的逆根系等价），因此（i）和（iii）的等价可从第1章得出。 VI, §1, no. 6，第 18 号提案和 Cor.蕴涵 (ii) $\Rightarrow$ (i) 是微不足道的，相反的蕴涵由 loc 得出。引用。

用X(T)的元素的$X_{++}$集合表示，使得$\langle \lambda , K_{\alpha}\rangle  \geq 0$对于每个正根$\alpha$。据说$X_{++}$中的元素占主导地位。它们形式是X(T)上W的运算的基本域（第VI, §1, no. 10章）。我们有$X_{++}\subset X_+$。

如果 G 是单连通的，对于每个简单根 $\alpha$，存在 X(T) 的元素 $\varpi_{\alpha}$，使得对于每个简单根 $\beta$ $\langle \varpi_{\beta}, K_{\alpha}\rangle =\delta_{\alpha \beta}$，即 $s_{\alpha}(\varpi_{\alpha}) =$ $\varpi_{\alpha}-\alpha ,s_{\beta}(\varpi_{\alpha}) =\varpi_{\alpha}$ 对于每个简单的根 $\beta \not=\alpha$； $\varpi_{\alpha}$ 称为基本主权；它们是交换性群 X(T) 和交换幺半群 $X_{++}$ 的形式基；更准确地说，X(T)的每个元素$\lambda$都可以写成形式$\lambda =\sum_{\alpha}\langle \lambda , K_{\alpha}\rangle \varpi_{\alpha}$。

用 $X(T)\otimes \mathbf{Q}$ 的 $\rho$ 元素表示，使得

$$
2\rho =\sum_{\alpha\in R_+}\alpha
$$

对于每个简单的根 $\alpha$，我们都有$\langle \rho , K_{\alpha}\rangle = 1$（第 VI, §1, no. 10 章，提案 29）。如果 G 是单连通的，$\rho$ 是基本显性权的和。

### 2. 最高权 / 不可约表示

关联到从 $\mathbf{C}$-李代数 $\mathfrak{g}_{\mathbf{C}}$ 到 End(V) 的任何表示 $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ 同态 $L(\tau )_{(\mathbf{C})}$，在实向量空间基础上延伸 $\mathfrak{g}$ 的线性表示 $L(\tau )$ V（第III, §3, no. 11章）。根据§4, no. 3、映射 $\delta$的第7条规定，从X(T)到Hom$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C}) =\mathfrak{t}^*_{\mathbf{C}}$ 诱导双射，从$\tau$的权集合相对于T到集合 of 权 of $L(\tau )_{(\mathbf{C})}$ relative to 嘉当子代数 $\mathfrak{t}_{\mathbf{C}}$ of $\mathfrak{g}_{\mathbf{C}}$.

#### 引理 2 {#lie-ix-s7-lem-2 .statement tag=01G0}

Let $\varphi$ be 线性表示 of the complex 李代数 $\mathfrak{g}_{\mathbf{C}}$ on a finite dimensional complex 向量空间 V.在V上存在G的表示$\tau$，使得$L(\tau )_{(\mathbf{C})}=\varphi$当且仅当$\varphi$是半单并且在V属于到$\delta (X(T))$上存在$\mathfrak{t}_{\mathbf{C}}$的权。

如果存在 G 的表示 $\tau$ 使得 $L(\tau )_{(\mathbf{C})}=\varphi$，则 $\varphi$ 为半单，因为 G 是连通的并且 $\tau$ 为半单（第 13 条命题第 III, §6, no. 5 的 Cor.2），以及权 $\mathfrak{t}_{\mathbf{C}}$ on V 属于 to 像 of $\delta$.因此，条件是必要的；我们将证明它是足够的。 If $\varphi$ is 半单, V is 直和 of the $V_\mu(\mathfrak{t}_{\mathbf{C}})$, where $\mu$ 属于 to 集合 of 权 of $\mathfrak{t}_{\mathbf{C}}$ on V (Chap. VII, §2, no. 4，第 2 条第 3 条）；如果$\delta$的所有权属于到像，则在V上存在T的表示$\tau_T$，使得$L(\tau_T)_{(\mathbf{C})}=\varphi |\mathfrak{t}_{\mathbf{C}}:$确实，只需将$\tau_T(t)v=t^{\lambda}v$放入$t\in T$并且$v\in V_{\delta(\lambda)}(\mathfrak{t}_{\mathbf{C}})$。 引理现在遵循§2, no. 6 的第 8 条提案。

#### 定理 1 {#lie-ix-s7-thm-1 .statement tag=01G1}

a) 令$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$为G的不可约表示。则$\tau$（相对于T）的权的集合有最大的元素$\lambda$，为主导，空间 $V_{\lambda}(T)$等于维数1。

b) Two 不可约表示 of G are equivalent if and only if their 最高权 are equal.

c) For every dominant 元素 $\lambda$ of X(T), there exists 不可约表示 of G of 最高权 $\lambda$.

由引理2，G对应不可约表示等价类双射到$\mathfrak{g}$的有限维不可约表示类，其权属于到$\delta (X(T))$。

用 $\mathscr{C}\mathfrak{g}_{\mathbf{C}}$ 中心表示，并用 $\mathscr{D}\mathfrak{g}_{\mathbf{C}}$ 表示 $\mathfrak{g}_{\mathbf{C}}$ 的导出李代数，从而得到 $\mathfrak{g}_{\mathbf{C}}=\mathscr{C}\mathfrak{g}_{\mathbf{C}}\oplus \mathscr{D}\mathfrak{g}_{\mathbf{C}}$。对于$\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}\mathfrak{g}_{\mathbf{C}}$上的每个双线性形式$\mu$，用$E(\mu)$表示第1章中介绍的简单$\mathscr{D}\mathfrak{g}_{\mathbf{C}}$模块。 VIII, §6, no. 3；对于$\mathscr{C}\mathfrak{g}_{\mathbf{C}}$上的每个线性形式$\nu$，用$\mathbf{C}(\nu )$表示与其关联的$\mathbf{C}$上的一维$\mathscr{C}\mathfrak{g}_{\mathbf{C}}$模。然后 $\mathfrak{g}_{\mathbf{C}}$-模块 $\mathbf{C}(\nu )\otimes E(\mu)$ 很简单，并且由第 1 章介绍。 VIII, §7, no. 2，科。 2 Th。 1 和代数，第 1 章。 VIII, §11, no. 1，周四。 1、每个有限维简单$\mathfrak{g}_{\mathbf{C}}$模都同构于模$\mathbf{C}(\nu )\otimes E(\mu)$之一；此外（前述）$\mathbf{C}(\nu )\otimes E(\mu)$ 是有限维的当且仅当对于每个简单的根 $\alpha$ $\mu(H_{\alpha})$ 是正整数。如果我们用$\mathfrak{t}_{\mathbf{C}}$上的$\nu +\mu$线性形式表示$\mathscr{C}\mathfrak{g}_{\mathbf{C}}$上的诱导$\nu$和$\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}\mathfrak{g}_{\mathbf{C}}$上的$\mu$，则$(\nu +\mu)(H_{\alpha}) =\mu(H_{\alpha})$；此外，$\mathbf{C}(\nu )\otimes E(\mu)$的权是$\nu +\lambda$，其中$\lambda$是$E(\mu)$的任何权，因此是形式$\nu +\mu-\theta$，其中$\theta \in \delta (X_+)$（第VIII, §6, no. 2章， 引理2)。

我们结论认为$\mathfrak{g}$模$\mathbf{C}(\nu )\otimes E(\mu)$是有限维的当且仅当对于每个简单的根$\alpha$，$(\nu +\mu)(H_{\alpha})$是正整数，并且它的权属于到$\delta (X(T))$当且仅当$\nu +\mu$属于至$\delta (X(T))$。这两个条件中的合取表示$\nu +\mu$属于到$\delta (X_{++})$；在这种情况下，$\nu +\mu$ 是 $\mathbf{C}(\nu )\otimes E(\mu)$ 的最高权。因此，我们为最高权$\lambda$的G的X(T)不可约表示的每个主导权$\lambda$构建，并因此获得了直到等价的G的所有不可约表示。从向量开始维数 1、证明中的$\mathbf{C}(\nu )\otimes E(\mu)$ 形式子空间权 $\nu +\mu$ 已完成。

#### 推论 {#lie-ix-s7-n2-cor-1 .statement tag=01G2}

群 G 有一个（有限维）忠实的线性表示。

首先观察X(T)的每个元素等于两个显性权之差：更准确地说，让$\varpi$是$X_{++}$的元素，这样对于每个简单的根$\alpha$，$\langle \varpi , K_{\alpha}\rangle >0$；对于所有$\lambda \in X(T)$，存在正整数$n$，这样对于每个简单的根$\alpha$，都存在$\langle \lambda +n\varpi , K_{\alpha}\rangle  \geq 0$，即(no. 1，引理$1$)$\lambda +n\varpi \in X_{++}$。

因而，存在$X_{++}$生成的$\mathbf{Z}$模X(T)的元素的有限族$(\lambda_i)_{i\in I}$。对于$i\in I$，令$\tau_i$为最高权$\lambda_i$G不可约表示(Th.1)；设表示$\tau$为$\tau_i$的直和。由$\tau$(相对于T)生成$\mathbf{Z}$-模X(T)权构造集合$P(\tau ,T)$。现在从§4, no. 3的第6条命题可以得出，同态$\tau$是单射的，因此推论。

#### 注 1 {#lie-ix-s7-n2-rem-1 .statement tag=01G3}

令$\mathfrak{n}_+$为$\mathfrak{g}_{\mathbf{C}}$的子代数，即$\alpha  >0$的$\mathfrak{g}^{\alpha}$的和。令$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$为不可约表示，$\lambda \in X_{++}$为最高权，由$\tau$诱发$\tau ':\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}(V)$表示。那么$V_{\lambda}(T)$就是V中向量$v$的子空间由……组成，这样对于所有$x\in \mathfrak{n}_+$来说$\tau '(x)v= 0$。

事实上，这是从 $\mathfrak{g}_{\mathbf{C}}$ 模块 $\mathbf{C}(\nu )\otimes E(\mu)$ 的相应的叙述得出的（第 VIII, §6, no. 2 章，提案 3）。

#### 注 2 {#lie-ix-s7-n2-rem-2 .statement tag=01G4}

设$\Theta (G)$为G上的连续代表函数的代数，其中$\mathbf{C}($代数中的值，第1章。 VIII）。让G通过左平移和右平移对$\Theta (G)$进行运算。对于每个$\lambda \in X_{++}$，令$(V_{\lambda}, \tau_{\lambda})$为最高权$\lambda$（第1章）的G的不可约表示，以及$(V^*_{\lambda},\check{\tau}_{\lambda})$的对立表示（第III, §3, no. 11）；根据谱理论，对于$X_{++}$中的所有$\lambda$，$\Theta (G)$上的$G\times G$的表示同构于表示$(V_{\lambda}\otimes V^*_{\lambda}, \tau_{\lambda}\otimes \check{\tau}_{\lambda})$的直和。 注 1 现在意味着以下叙述：设$\lambda \in X_{++}$，并令$E_{\lambda}$为G上连续代表函数$f$的$\Theta (G)$由……组成的向量子空间，使得$f(gt) =\lambda (t)^{-1}f(g)$对于所有$g\in G$和所有$t\in T$，并且$f*x= 0$对于所有$x\in \mathfrak{n}_-=\bigoplus_{\alpha <0}\mathfrak{g}^{\alpha}$。

那么$E_{\lambda}$在左平移下是稳定的，并且左平移下G在$E_{\lambda}$上的表示是不可约的最高权$\lambda$。

#### 注 3 {#lie-ix-s7-n2-rem-3 .statement tag=01G5}

设$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$为不可约表示。 X(C(G)) 存在元素 $\nu$，使得$\tau (s)v=\nu (s)v$ 对于所有$s\in C(G), v\in V:$ 事实上，$\tau (C(G))$ 包含在$\tau$(G) 的交换子中，等于$\mathbf{C}^*.1_V($代数，第 1 章VIII, §3, no. 2，周四。 1).对于$\tau$中的每一个权$\lambda$，$\lambda$到C(G)中的限制等于$\nu$。

#### 注 4 {#lie-ix-s7-n2-rem-4 .statement tag=01G6}

第 1 章的定义和叙述 VIII, §7，编号。 2至5可以毫无困难地推广到目前的情况；我们把细节留给读者。

#### 命题 1 {#lie-ix-s7-prop-1 .statement tag=01G7}

令$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$为最高权$\lambda \in X_{++}$的G的不可约表示。令$m$为整数$\sum_{\alpha\in R_+}\langle \lambda , K_{\alpha}\rangle$，并令$w_0$

是 Weyl 群的元素，使得 $w_0(R_+) = R_-$（第 VI, § 6 章，第 17 号提案第 3 条）。有三种可能的情况：

a$)w_0(\lambda ) =-\lambda$ 和 $m$ 是偶数。则V上存在分离对称双线性形式的G不变量； 表示$\tau$是真正的型（附录II）。

b$)w_0(\lambda )\not=-\lambda$。 V 上的每个 G 不变双线性形式都是零； 表示 $\tau$ 是复数型（前述）。

c$)w_0(\lambda ) =-\lambda$ 和 $m$ 是奇数。那么在 V 上存在分离交错的双线性形式的 G 不变量； 表示 $\tau$ 属于四元数型（前述）。

如果$\tau$到$C(G)_0$的限制不是微不足道的，我们就处于情况b)。

V 上的双线性形式 B 在 G 下是不变的当且仅当它在 $\mathfrak{g}_{\mathbf{C}}$ 下不变（第 III, §6, no. 5 章，Cor. 3）。因此，如果 G 是半单，则命题由第 1 章得出。 VIII, §7, no. 5、附录II第 12 号提案和第 3 号提案。

一般情况下，放入$C(G)_0= S$，认同$X(T/S)$，子群为X(T)（W下稳定）。如果$\tau (S) =\{1_V\},\tau$诱导通过最高权$\lambda$前往商表示$\tau ': G/S\rightarrow \mathbf{G}\mathbf{L}(V)$；在这种情况下，命题源自前面的内容，应用于$G/S$。

假设$\tau (S)\not=\{1_V\}$。存在X(S) 的非零元素 $\nu$，使得$\tau (s) =\nu (s)_V$ 对于所有$s\in S$ (注 3)。那么$\nu$就是限制同态$X(T)\rightarrow X(S)$下$\lambda$的像；由于 W 对 X(S) 的运算很简单，等式 $w_0(\lambda ) =-\lambda$ 意味着 $\nu =-\nu$，这是不可能的：因此是 $w_0(\lambda )\not=-\lambda$。另一方面，如果 B 是 V 上的 G 不变双线性形式，对于 V 中的所有 $x, y$ 和 S 中的 $s$，我们有，

$$
B(\nu (s)x, \nu (s)y) = B(x, y) =\nu (s)^2B(x, y)
$$

这意味着 B = 0，因此命题。

设$\mathfrak{S}_{\mathbf{R}}(G)$为有限维实数向量空间上G的不可约连续表示类集合。命题1和附录II的结果给出双射$\Phi : X_{++}/\Sigma \rightarrow \mathfrak{S}_{\mathbf{R}}$(G)，其中$\Sigma$表示Aut(X(T))的子群$\{1,-w_0\}$。更准确地说，令$\lambda \in X_{++}$，并且令$E_{\lambda}$为最高权$\lambda$G的表示；然后

$\Phi (\{\lambda ,-w_0(\lambda )\}) = E_{\lambda[\mathbf{R}]}$ 如果$\lambda \not=-w_0(\lambda )$ 或如果$\sum_{\alpha\in R_+}\langle \lambda , K_{\alpha}\rangle \notin2\mathbf{Z}$

$\Phi (\{\lambda ,-w_0(\lambda )\}) = E'_{\lambda}$如果$\lambda =-w_0(\lambda )$和$\sum_{\alpha\in R_+}\langle \lambda , K_{\alpha}\rangle  \in 2\mathbf{Z}$

其中$E'_{\lambda}$是G下$E_{\lambda}$不变量的$\mathbf{R}$结构。

### 3. 环R(G)

令 R(G) 为 G 的表示的环（连续，在有限维复数向量空间上）（代数，第 VIII, §10, no. 6）。如果$\tau$是G的表示，则用$[\tau ]$表示其在R(G)中的类；如果$\tau$和$\tau '$是G的两个表示，则通过定义，我们有，

$$
[\tau ] + [\tau '] = [\tau \oplus \tau ']
$$

$$
[\tau ][\tau '] = [\tau \otimes \tau ']
$$

由于G的每一个表示都是半单，所以$\mathbf{Z}$模R(G)是自由的，承认G的不可约表示类基集合，集合可以通过Th与$X_{++}$识别。 1. 映射$\tau  \rightarrow L(\tau )_{(\mathbf{C})}$诱导同态$l$从环R(G)到$\mathfrak{g}_{\mathbf{C}}$表示的环$\mathscr{R}(\mathfrak{g}_{\mathbf{C}})$（第VIII, §7, no. 6章）。

设$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$为G的表示；我们考虑$\mathbf{C}$向量空间V的渐变$(V_{\lambda}(T))_{\lambda\in X(T)}$。用Ch(V)表示，或者用Ch($\tau$)表示，分级的向量空间V(第VIII, §7, no. 7)中的特征标；如果 $(e^{\lambda})_{\lambda\in X(T)}$ 表示代数 $\mathbf{Z}[X(T)] =\mathbf{Z}^{(X(T))}$ 中的典范基，则通过定义，我们有，

Ch($\tau$)$=\sum_{\lambda\in X(T)}$(暗淡$V_{\lambda}(T)$)$e^{\lambda}$。

我们以同样的方式计算定义（见上文）环的同态，也用Ch表示，从R(G)到$\mathbf{Z}[X(T)]$。如果 G 是半单，我们有交换律图表

R(G) $\longrightarrow^{Ch}\mathbf{Z}[X(T)]$

$$
_{l\widetilde{\delta}} \tag{1}
$$

$$
\mathscr{R}(\mathfrak{g}_{\mathbf{C}})\longrightarrow^{ch}\mathbf{Z}[P]
$$

其中P表示$R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$的权和$\widetilde{\delta}$同态由$\delta$引起的群。

Weyl 群 W 在群 X(T) 上由自同构运营，因此在环 $\mathbf{Z}[X(T)]$ 运营。根据§4, no. 3的命题5，Ch的像包含在W下元素不变量的子环$\mathbf{Z}[X(T)]^W$由……组成中。

#### 命题 2 {#lie-ix-s7-prop-2 .statement tag=01G8}

同态 Ch 诱导同构从 R(G) 到 $Z[X(T)]^W$。

对于$\lambda \in X_{++}$，用最高权$\lambda$的不可约表示的R(G)中的$[\lambda ]$类表示。由于族$([\lambda ])_{\lambda\in X_{++}}$是$\mathbf{Z}$模R(G)的基，因此只需证明以下断言：

系列 (Ch[$\lambda ]$)$_{\lambda\in X_{++}}$ 是 $\mathbf{Z}$ 模块 $\mathbf{Z}[X(T)]^W$ 的基。

对于$\mathbf{Z}[X(T)]$的每个元素$u=\sum_{\lambda}a_{\lambda}e^{\lambda}$，如果$\lambda$是$\mu\in X(T)$的集合的极大元素，则$u$中的项$a_{\lambda}e^{\lambda}$被称为最大，使得$a_\mu\not= 0$。 Th。 1 意味着 Ch[$\lambda ]$ 具有唯一的最大值项，即 $e^{\lambda}$。因此，命题源自以下引理。

#### 引理 3 {#lie-ix-s7-lem-3 .statement tag=01G9}

对于每个$\lambda \in X_{++}$，令$C_{\lambda}$为$\mathbf{Z}[X(T)]^W$中的元素，具有唯一的最大值项$e^{\lambda}$。那么家庭$(C_{\lambda})_{\lambda\in X_{++}}$就是$\mathbf{Z}[X(T)]^W$的基。

证明与第 1 章的命题 3 相同。 VI, §3, no. 4、替换 A 乘以 $\mathbf{Z}, P$ 乘以 X(T) 以及 $P\cap \overline{C}$ 乘以 $X_{++}$。

令$\Theta (G)$（或$\Theta (T)$）为G（或T）上连续代表函数的$\mathbf{C}$-代数，令$Z\Theta (G)$（或$\Theta (T)^W$）为中心的子代数由……组成（或W-不变式） 函数。 限制映射$\Theta (G)\rightarrow \Theta (T)$诱导同态共环$r: Z\Theta (G)\rightarrow \Theta (T)^W$。另一方面，与表示$\tau$关联的映射其特征标（即函数$g \rightarrow$Tr$\tau (g)$）$\mathbf{C}$-代数的扩展到同态 Tr$:\mathbf{C}\otimes_{\mathbf{Z}}R(G)\rightarrow Z\Theta (G)$，根据光谱理论，是同构。类似地，$\mathbf{C}$-代数$\iota :\mathbf{C}[X(T)]\rightarrow \Theta$(T)的典范嵌入$X(T)\rightarrow \Theta (T)$诱导同构，其中诱导同构$\iota :\mathbf{C}[X(T)]^W\rightarrow \Theta (T)^W$。 图表

$$
\mathbf{C}\otimes_{\mathbf{Z}}R(G)\overset{1\otimes Ch}{\longrightarrow}\mathbf{C}[X(T)]^W
$$

$$
_{Tr}^{\iota} \tag{2}
$$

$$
Z\Theta (G)\longrightarrow^r\Theta (T)^W
$$

是可交换的：事实上，对于每个表示 $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ 和所有 $t\in T$，

Tr $\tau (t) =\sum_{\lambda\in X(T)}$(暗淡$V_{\lambda}(T)$)$\lambda (t) =\iota$(Ch$\tau$)$(t)$,

即$(r\circ$ Tr)[$\tau ] = (\iota \circ$ Ch)[$\tau ]$。

我们现在可以从命题推出以下结果。

#### 推论 {#lie-ix-s7-n3-cor-1 .statement tag=01GA}

限制映射 $r: Z\Theta (G)\rightarrow \Theta (T)^W$ 是双射。

### 4. 特征标公式

在这个数中，我们乘法写出群X(T)，并将其元素视为T上的复值函数。我们假设$X(T)\otimes \mathbf{Q}$属于的元素$\rho$为X(T)。

T 上用$L^2(T)$表示平方可积复形函数的类的希尔伯特空间，并用连续代表函数的$\Theta (T)$子空间由……组成表示。根据谱理论，X(T) 是$L^2(T)$ 的正交基和$\Theta (T)$ 的代数基。

对于$f\in L^2(T)$和$w\in W$，用$^wf(t) =f(w^{-1}(t))$定义的$L^2(T)$的$^wf$元素表示；因而，对于$\lambda \in X(T)$，我们有$^w\lambda =w(\lambda )$。用$\varepsilon : W\rightarrow  \{1,-1\}$表示签名（唯一同态使得对于每个反射$s$都有$\varepsilon (s) =$$-1$）；对于 $f\in L^2$(T)，输入

$$
J(f) =\sum_{w\in W}\varepsilon (w)^wf
$$

如果 $\lambda \in X_{++}$、特征标 $^w(\lambda \rho )$ 不同；事实上，只要证明 $^w(\lambda \rho )\not=\lambda \rho$ 对于所有 $w\not= 1$ 就足够了；但这是从引理 1 (no. 1) 和$\langle \lambda \rho , K_{\alpha}\rangle =\langle \lambda , K_{\alpha}\rangle + 1>0$ 对于每个正根 $\alpha$ 的事实得出的。因而，

$\|J(\lambda \rho )\|^2=$卡(W)$=w(G)$。

如果$^wf=\varepsilon (w)f$对于所有$w\in W$（即，如果$^sf=-f$对于每个反射$s$），则元素$f\in L^2(T)$被称为反不变性。我们将证明$\frac{1}{w(G)}J$是$L^2(T)$到反不变量元素的子空间的正交投影。事实上，令$f, f'$在$L^2$(T)中，且$f'$反不变量；那么 $J(f)$ 是反对不变的并且

$$
\langle f',J(f)\rangle =\sum_{w\in W}\varepsilon (w)\langle f',^wf\rangle =\sum_{w\in W}\langle^wf',^wf\rangle
$$

$$
=\sum_{w\in W}\langle f', f\rangle =w(G)\langle f', f\rangle
$$

#### 命题 3 {#lie-ix-s7-prop-3 .statement tag=01GB}

元素 $J(\lambda \rho )/\surd\overline{w(G)}$，对于 $\lambda \in X_{++}$，形式反不变量子空间的正交基 $L^2(T)$ 元素，以及反不变量子空间的代数基元素共 $\Theta (T)$。

证明与第 1 章相同。 VI, §3, no. 3，命题 1。

由章。 VI，位置。前述，提案 2，

$$
J(\rho ) =\rho \prod_{\alpha >0}(1-\alpha^{-1}) =\rho^{-1}\prod_{\alpha >0}(\alpha -1) \tag{3}
$$

所以

$$
J(\rho )J(\rho ) =\prod_{\alpha}(\alpha -1) \tag{4}
$$

由科. 2 Th。 1 (§6, no. 2)，我们推出：

#### 引理 4 {#lie-ix-s7-lem-4 .statement tag=01GC}

如果$\varphi$和$\psi$是G上两个连续的中心函数，

$$
\int_G\overline{\varphi(g)}\psi (g)dg=\frac{1}{w(G)}\int_T\overline{(\varphi(t)J(\rho)(t))}.(\psi (t)J(\rho )(t))dt
$$

对于所有$\lambda \in X_{++}$，用最高权$\lambda$G不可约表示$\chi_{\lambda}$特征标表示。

#### 定理 2（H.韦尔）{#lie-ix-s7-thm-2 .statement tag=01GD}

对于所有$\lambda \in X_{++}$，我们有$J(\rho ).\chi_{\lambda}|T = J(\lambda \rho )$。

函数$J(\rho ).\chi_{\lambda}|T$在W下是反对不变量，并且X(T)的元素与整数系数为线性组合。因此，由章。 VI, §3, no. 3，第 1 条，它可以写成 $\sum_\mu a_\mu J(\mu\rho )$，其中 $\mu$ 属于到 $X_{++}$，$a_\mu$ 是整数，几乎都是有限的，其中许多是零；从$\int_G|\chi_{\lambda}(g)|^2dg= 1$开始

（谱理论），由命题3和引理4得出$\sum_\mu(a_\mu)^2= 1$；因此，除了必须等于 1 或 $-1$ 的一个之外，$a_\mu$ 都是零。但$\chi_{\alpha}|T$中$\lambda$的系数等于1（Th.1），因此$J(\rho ).\chi_{\lambda}|T$中$\lambda \rho$的系数等于1（VI, §3, no. 3，注2），这意味着$a_{\lambda \rho}= 1$，因此定理。

#### 推论 1 {#lie-ix-s7-thm-2-cor-1 .statement tag=01GE}

对于no. 3的记号，我们在$\mathbf{Z}[X(T)]$中有，

$(\sum_{w\in W}\varepsilon (w)e^{w\rho})$ Ch[$\lambda ] =\sum_{w\in W}\varepsilon (w)e^{w\lambda}e^{w\rho}$ 对于所有 $\lambda \in X_{++}$。

这是从定理和交换律图表 (2) (no. 3) 得出的。

#### 推论 2 {#lie-ix-s7-thm-2-cor-2 .statement tag=01GF}

对于 T 的所有 $\lambda \in X_{++}$ 和每个正则元素 $t$，

$$
\chi_{\lambda}(t) =\sum\sum^w\varepsilon_w(w\varepsilon )(\lambda w()wt\rho ()wt\rho ()wt) \tag{5}
$$

其中两个和超过W的元素$w$。

事实上，$J(\rho )(t)$ 是非零的，因为$t$ 是正则的 (公式 (4))。

如果$\varphi$是G上的中心函数，则$\varphi$到T的限制在W下是不变的，所以$J(\rho ).\varphi |T$在W下是反不变的。 此外，通过光谱理论和 Th。 1、族$(\chi_{\lambda})_{\lambda\in X_{++}}$是G上中心代表函数空间的代数基，也是G上平方可积中心函数类空间ZL$^2(G)$的正交基。

因此，根据 Prop. 3 和 Th. 2 我们推论：

#### 推论 3 {#lie-ix-s7-thm-2-cor-3 .statement tag=01GG}

映射与 G 上的任何连续中心函数 $\varphi$ 函数 $w(G)^{-1/2}J(\rho )(\varphi |T)$ 诱导同构从中心代表的空间 G 上的函数到反不变量的空间 $\Theta (T)$ 中的元素；它扩展通过从ZL$^2(G)$到$L^2(T)$的反不变量元素的子空间连续到希尔伯特空间的同构。

#### 推论 4 {#lie-ix-s7-thm-2-cor-4 .statement tag=01GH}

令$\varphi$为G上的连续中心函数。那么，

$$
\int_G\overline{\chi_{\lambda}(g)}\varphi (g)dg=\int_T\overline{\lambda(t)}\prod_{\alpha >0}(1-\alpha (t)^{-1})\varphi (t)dt=\int_T\overline{\lambda \rho(t)}.\varphi (t)J(\rho )(t)dt
$$

事实上，到引理 4 和 Th。 2、

$$
\int_G\overline{\chi_{\lambda}(g)}\varphi (g)dg=\frac{1}{w(G)}\int_T\chi_{\lambda}(t)J(\rho )(t)(\varphi (t)J(\rho )(t))dt
$$

$$
=\frac{1}{w(G)}\int_T\overline{J(\lambda \rho)(t)}\varphi (t)J(\rho )(t)dt
$$

但函数 $t \rightarrow \varphi (t)J(\rho )(t)$ 是反不变式，$\frac{1}{w(G)}J(\lambda \rho )$ 是 $\lambda \rho$ 的正交投影到 $L^2$(T) 的反不变式元素的子空间，所以

$$
\frac{1}{w(G)}\int_T\overline{J(\lambda \rho)(t)}\varphi (t)J(\rho )(t)dt=\int_T\overline{\lambda \rho(t)}\varphi (t)J(\rho )(t)dt
$$

最后，到公式 (3)，我们得到$\rho (t)J(\rho )(t) =\prod_{\alpha >0}(1-\alpha (t)^{-1})$，因此推论。

#### 注 1 {#lie-ix-s7-n4-rem-1 .statement tag=01GI}

对于所有$w\in W$，放入$\rho_w=^w\rho /\rho$；那么

$$
\sum_w\varepsilon (w)\rho_w=\prod_{\alpha >0}(1-\alpha^{-1}) =\rho^{-2}\prod_{\alpha >0}(\alpha -1) \tag{6}
$$

如果 $t$ 是 T 的正则元素，我们从 (5) 推出

$$
\chi_{\lambda}(t) =\sum\sum^w\varepsilon_w(w\varepsilon )(\overset{w}{w}\lambda )\rho (t_w)(\rho t^w)(t)=\sum\prod^w_{\alpha >}\varepsilon (_0w(1)\overset{w}{-}\lambda \alpha (t()t\rho )^{w-}(_1t)) \tag{7}
$$

请注意，$\rho_w$是根与整数系数的线性组合，因此属于到X(T)，即使我们不假设$\rho \in X(T)$。由此可见，在没有假设的情况下，公式 (7) 是有效的，$\rho \in X(T):$ 确实如此，为了证明这一点，我们通过合适的连通覆盖来证明替换 G，然后将其简化为 Cor。 2.

#### 注 2 {#lie-ix-s7-n4-rem-2 .statement tag=01GJ}

同样，Cor 的第一个等式。如果没有假设和 $\rho \in X(T)$，4 仍然有效。

#### 注 3 {#lie-ix-s7-n4-rem-3 .statement tag=01GK}

我们可以推导出Th。 2 来自类似的无穷小叙述（第 VIII, §9, no. 1 章，第 1 章）； Th 也是如此。下一个数的第 3 个（与前述第 2 个no. 2 的类似物）。

### 5. 次数 / 不可约表示

现在，我们返回群 X(T) 的加法记号，并且不再假设 $\rho$ 属于到 X(T)。

#### 定理 3 {#lie-ix-s7-thm-3 .statement tag=01GL}

最高权$\lambda$G不可约表示空间维数由下式给出

$$
\chi_{\lambda}(e) =\prod_{\alpha\in R_+}\frac{\langle\lambda + \rho , K_{\alpha}\rangle}{\langle\rho , K_{\alpha}\rangle}
$$

将 $\gamma =\frac{1}{2}\sum_{\alpha >0}K_{\alpha}$ 放入 $\delta (\alpha )(\gamma ) = 2\pi i$ 对应于每个简单的根 $\alpha$（第 VI, §1, no. 10 章，第 29 条命题）。行 $\mathbf{R}\gamma$ 不包含在任何超平面 Ker $\delta (\alpha )$ 中，因此对于所有足够小的 $z\in \mathbf{R}^*$，exp($z\gamma$ ) 是 G 的正则元素；对于所有 $\mu\in X(T)$ 和所有 $z\in \mathbf{R}$，我们有

$J(\mu$)(exp($z\gamma$))$=\sum_{w\in W}\varepsilon (w)e^{z\delta(\mu)(w^{-1}\gamma)}$。

让我们暂时接受以下引理：

#### 引理 5 {#lie-ix-s7-lem-5 .statement tag=01GM}

我们有

$J(\mu$)(exp($z\gamma$))$=e^{z\delta(\mu)(\gamma)}\prod_{\alpha >0}(1-e^{-z\delta(\mu)(K_{\alpha})})$。

因此，函数 $J(\mu$)(exp($z\gamma$ )) 是函数的乘积，当 $z$ 趋于 0 时趋于 1，并且

$$
z^N\prod_{\alpha >0}\delta (\mu)(K_{\alpha}) = (2\pi iz)^N\prod_{\alpha >0}\langle \mu, K_{\alpha}\rangle
$$

其中 N = 卡 $R_+$。

首先假设$\rho \in X(T)$； 应用科。 2 Th。 2 我们看到，随着 $z$ 趋于 $0,\chi_{\lambda}(z\gamma )$ 趋于

$$
\prod_{\alpha >0}\langle \lambda +\rho , K_{\alpha}\rangle /\prod_{\alpha >0}\langle \rho , K_{\alpha}\rangle
$$

因此在这种情况下是定理。

在一般情况下，只需指出，在证明 Th 中。 3，我们总是可以通过合适的连接覆盖来替换G，从而约化到前面的情况。

现在我们证明引理 5。设 $z\in \mathbf{C}$；用$\varphi_z$映射从$\mathfrak{t}$到$\mathbf{C}$-代数映射(X(T)$,\mathbf{C}$)的映射从X(T)到$\mathbf{C}$关联到$H\in \mathfrak{t}$映射

$\varphi_z(H) :\mu \rightarrow \mu$(exp $zH$) $=e^{z\delta(\mu)(H)}$。

我们有 $\varphi_z(H+H') =\varphi_z(H)\varphi_z(H')$，所以存在同态或环

$\psi_z:\mathbf{Z}[\mathfrak{t}]\rightarrow$ 映射(X(T)$,\mathbf{C}$)

这样$\psi_z(e^H)(\mu) =e^{z\delta(\mu)(H)}$。另一方面，由章。 VI, §3, no. 3，命题2，我们在$\mathbf{Z}[\mathfrak{t}]:$中有以下关系

$$
\sum_{w\in W}\varepsilon (w)e^{w\gamma}=e^{\gamma}\prod_{\alpha >0}(1-e^{-K_{\alpha}})
$$

应用同态 $\psi_z$，并使用等式

$$
\psi_z(e^{w\gamma})(\mu) =e^{z\delta(\mu)(w\gamma)}=e^{z\delta(w^{-1}\mu)(\gamma)}
$$

我们推导出所述的公式。

#### 推出 1 {#lie-ix-s7-lem-5-cor-1 .statement tag=01GN}

令$\| \|$在$X(T)\otimes \mathbf{R}$上为范数。对于所有$\lambda \in X_{++}$，令$d(\lambda )$为最高权$\lambda$G不可约表示空间维数。

a）sup$_{\lambda\in X_{++}}d(\lambda )/\|\lambda +\rho \|^N<\infty$，其中$N = 1/$2（暗淡$G-$暗淡T）。

b) 如果 G 是半单，则 inf$_{\lambda\in X_{++}}d(\lambda )/\|\lambda +\rho \|>0$。

a) 对于所有$\alpha \in R_+$，存在$A_{\alpha}>0$和$|\langle \lambda +\rho , K_{\alpha}\rangle | \leq A_{\alpha}\|\lambda +\rho \|$，因此存在$d(\lambda )/\|\lambda +\rho \|^N\leq \prod_{\alpha >0}A_{\alpha}/\langle \rho , K_{\alpha}\rangle$。

b) 假设G是半单，用$\beta_1, . . . , \beta_r$表示简单的根并放入$N_i=K_{\beta_i}$。然后

$$
d(\lambda )\geq \prod_{i=1}^r\frac{\langle\lambda + \rho , N_i\rangle}{\langle\rho , N_i\rangle}=\prod_{i=1}^r\langle \lambda +\rho , N_i\rangle
$$

从$\langle \lambda +\rho , N_i\rangle  \geq  \langle \rho , N_i\rangle = 1$开始，这意味着

$d(\lambda )\geq$支持$_i|\langle \lambda +\rho , N_i\rangle |$。

如果 G 是半单，$x \rightarrow$sup$|\langle x, N_i\rangle |$ 是$X(T)\otimes \mathbf{R}$ 上的范数，必然等价于给定的范数，因此 b)。

#### 推出 2 {#lie-ix-s7-lem-5-cor-2 .statement tag=01GO}

假设G为半单；设$d$为整数。 维数$\leq d$G表示类集合是有限的。

科。 $1b)$ 意味着 $X_{++}$ 的元素 $\lambda$ 的集合 $X_d$，使得 $d(\lambda )\leq d$ 是有限的。对于$X_d$中的所有$\lambda$，令$V_{\lambda}$为最高权$\lambda$中的不可约表示； 维数 $\leq d$ 中的每个表示都同构于直和 $\bigoplus_{\lambda\in X_d}V^{n_{\lambda}}_{\lambda}$，与 $n_{\lambda}\leq d$，因此推论。

### 6. 卡西米尔元素

根据§1, no. 3的命题3，$\mathfrak{g}$上存在负对称双线性形式，在Ad(G)下分离且不变（若G为半单，则可以取$\mathfrak{g}$的Killing形式为例）。令F为形式。回想一下（第 I, §3, no. 7 章），与 F 关联的卡西米尔元素是包络代数 $U(\mathfrak{g})$ 的中心的元素 $\Gamma$，这样，对于任何基 $(e_i)$ $\mathfrak{g}$满足$F(e_i, e_j) =-\delta_{ij}$，我们有$\Gamma =-\sum e^2_i$。

在这个章的其余部分中，我们将通过 $\mathfrak{g}$ 上的负分离不变对称双线性形式来调用$U(\mathfrak{g})$ 的 G 元素的卡西米尔元素。如果$\Gamma$是G的卡西米尔元素，并且如果$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$是G的不可约表示，则V的自同态$\Gamma_V$是位似（代数，第VIII, §3, no. 2，Th.1），其比率我们用$\widetilde{\Gamma}(\tau )$表示。

#### 命题 4 {#lie-ix-s7-prop-4 .statement tag=01GP}

设$\Gamma$为G的卡西米尔元素。

a) 如果G$,\widetilde{\Gamma}(\tau )$的$\tau$是不可约表示是实数并且是正数。如果$\tau$不是平凡的表示，则$\widetilde{\Gamma}(\tau )>0$。

b) $X(T)\otimes \mathbf{R}$ 上存在唯一的二次形式 $Q_{\Gamma}$，使得对于 G 的每个不可约表示 $\tau$，

$$
\widetilde{\Gamma}(\tau ) = Q_{\Gamma}(\lambda +\rho )-Q_{\Gamma}(\rho )
$$

其中 $\lambda$ 是 $\tau$ 的最高权。 形式 $Q_{\Gamma}$ 在 W 下为正、分离且不变。

设 F 是定义 $\Gamma$ 的 $\mathfrak{g}$ 上的分离负对称双线性形式。设$\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$为G的不可约表示；令 $\langle ,\rangle$ 为 G (§1, no. 1) 下 V 不变量上的希尔伯特标量乘积，且 $\mathfrak{g}$ 的 $(e_i)$ 基使得$F(e_i, e_j) =-\delta_{ij}$。然后，对于 V 的每个元素 $v$ 在 G 下不不变，我们有

$$
\widetilde{\Gamma}(\tau )\langle v, v\rangle =\langle v, \Gamma_V(v)\rangle =-\sum_i\langle v,(e_i)^2_Vv\rangle =\sum_i\langle v,(e_i)^*_V(e_i)_Vv\rangle
$$

$$
=\sum_i\langle (e_i)_Vv,(e_i)_Vv\rangle >0
$$

因此a）。

令 B 为 F 由标量扩张引起的限制 $\mathfrak{t}^*_{\mathbf{C}}$ 上的形式到$\mathfrak{g}_{\mathbf{C}}$ 上双线性形式的$\mathfrak{t}_{\mathbf{C}}$ 的逆。由科。第 7 章提案VIII, §6, no. 4，我们有$^5\widetilde{\Gamma}(\tau ) = B(\delta (\lambda ), \delta (\lambda +2\rho ))$。 扩展 $\delta : X(T)\rightarrow$ $\mathfrak{t}^*_{\mathbf{C}}$ 到$\mathbf{R}$线性映射，从$X(T)\otimes \mathbf{R}$到$\mathfrak{t}^*_{\mathbf{C}}$，并让$Q_{\Gamma}$为$X(T)\otimes \mathbf{R}$上的二次方形式$x \rightarrow B(\delta (x), \delta (x))$；它在 W 下是分离且不变的，并且

$$
\widetilde{\Gamma}(\tau ) = B(\delta (\lambda +\rho ), \delta (\lambda +\rho ))-B(\delta (\rho ), \delta (\rho )) = Q_{\Gamma}(\lambda +\rho )-Q_{\Gamma}(\rho )
$$

我们证明形式 $Q_{\Gamma}$ 是正数。事实上，如果$\mathfrak{t}^*_{\mathbf{C}}$的$x\in X(T)\otimes \mathbf{Q}$、元素$\delta (x)$在$\mathfrak{t}$上取纯虚的值，因此在$i\mathfrak{t}$上取实数值；我们结论通过评论，对于$y\in i\mathfrak{t}$，我们有$F(y, y)\geq 0$。

仍有待证明b)中的唯一性断言。令 Q 为 $X(T)\otimes \mathbf{R}$ 满足上所需的条件的二次形式，并令 $\Phi$（或$\Phi_{\Gamma}$）为与 Q（或$Q_{\Gamma}$）关联的双线性形式。对于$\lambda , \mu\in X_{++}$，我们有

$$
\Phi (\lambda , \mu) = (Q(\lambda +\mu+\rho )-Q(\rho ))-(Q(\lambda +\rho )-Q(\rho ))-(Q(\mu+\rho )-Q(\rho ))
$$

$$
=\Phi_{\Gamma}(\lambda , \mu)
$$

由于$X(T)_{++}$生成$\mathbf{R}$向量空间$X(T)\otimes \mathbf{R}$，我们有$\Phi =\Phi_{\Gamma}$，所以$Q = Q_{\Gamma}$。

#### 注 {#lie-ix-s7-n6-rem-1 .statement tag=01GQ}

让$x\in \mathfrak{g}$。存在严格正的实数 A，使得对于 G 下的每个不可约表示 $\tau : G\rightarrow \mathbf{G}\mathbf{L}(V)$ 和V 不变量上的每个希尔伯特结构，

$$
\|L(\tau )(x)\|^2\leq A.\widetilde{\Gamma}(\tau )
$$

事实上，通过前面的证明中的记号，我们可以将$\mathfrak{g}$中的选择基$(e_i)$得出$x=ae_1,a\in \mathbf{R}$。那么，对于$v\in V$，我们有

$$
\langle x_Vv, x_Vv\rangle =|a|^2\langle e_1v, e_1v\rangle  \leq  |a|^2\widetilde{\Gamma}(\tau )\langle v, v\rangle
$$

### 习题 {#lie-ix-s7-exercises}

参见[习题为 § 7](exercises/s7/)。
