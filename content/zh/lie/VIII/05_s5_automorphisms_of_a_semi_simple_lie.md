---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 5
section_title: Automorphisms of a semi-simple Lie algebra
lang: zh
source: lie-vii-ix
book_pages: 106-115, 233-237
pdf_pages: 0114-0123, 0241-0245
extraction: native+ocr
subsections:
    - "no": 1
      title: AUTOMORPHISMS OF A FRAMED SEMI-SIMPLE LIE ALGEBRA
      page: 106
      pdf_page: 114
    - "no": 2
      title: AUTOMORPHISMS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA
      page: 107
      pdf_page: 115
    - "no": 3
      title: AUTOMORPHISMS OF A SPLITTABLE SEMI-SIMPLE LIE ALGEBRA
      page: 111
      pdf_page: 119
    - "no": 4
      title: ZARISKI TOPOLOGY ON Aut($\mathfrak{g}$)
      page: 113
      pdf_page: 121
    - "no": 5
      title: LIE GROUP CASE
      page: 115
      pdf_page: 123
statements: 25
exercises: 13
errata:
    - says: Chap. VII, §13, no. 1
      read: Chap. VIII, §13, no. 1
      why: Chapter VII has five sections and no section 13. The sentence says that the groups Aut$_0(\mathfrak{g})$ and Aut$_e(\mathfrak{g})$ can be distinct, and the place that shows it is no. 1 of section 13 of this chapter, on the algebras of type $A_l$, which computes Aut$_0(\mathfrak{g}) =\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$, identifies the quotient Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ with $\mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)/\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$, and over the reals finds it isomorphic to $\mathbf{Z}/2\mathbf{Z}$ when $l+1$ is even. Chapter VII names neither group anywhere.
content_sha256: 4b1a19430c4dc001ba10230100a3f9c2404091828022d83ae00207ad4a6e155e
translated_from: content/en/lie/VIII/05_s5_automorphisms_of_a_semi_simple_lie.md
translation_method: google
source_content_sha256: 952a7b9240fa2d193986215a77b227fd820dee9114e1cdbfa00e8cbcdb6611b5
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: e6ed198a1a15a7024f5b42baded9c2dff1a789ce3192b38eec56998316e7c1ba
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。 自同构半单李代数

在本段中，$\mathfrak{g}$表示半单李代数。

### 1. 自同构镶框半单李代数

回想一下（第 VII, §3, no. 1 章），Aut($\mathfrak{g}$) 表示 $\mathfrak{g}$ 的自同构的群。如果$\mathfrak{h}$是$\mathfrak{g}$嘉当子代数，我们用Aut($\mathfrak{g},\mathfrak{h}$)表示$\mathfrak{g}$自同构群，使得$\mathfrak{h}$保持稳定。假设$\mathfrak{h}$为分裂，令R为$(\mathfrak{g},\mathfrak{h})$的根系。如果$s\in$ Aut($\mathfrak{g},\mathfrak{h}$)，$s|\mathfrak{h}$的同积映射是A(R)的元素（R的自同构的群），我们在本段中用$\varepsilon (s)$表示。因此

$\varepsilon :$自动($\mathfrak{g},\mathfrak{h}$)$\rightarrow A(R)$

是同态 / 群。

对于任何根系 R 和 R 的任何基 B，我们用 R 的自同构的 Aut(R$,B$) 群表示，使 B 保持稳定。 Recall (Chap. VI, §1, no. 5, Prop. 16 and §4, no. 2, Cor. of Prop. 1) that A(R) is the semi-direct product of Aut(R$,B$) and W(R), and that $A(R)/W(R)$ is canonically isomorphic to the group of automorphisms of the Dynkin graph of R.

#### 命题 1 {#lie-viii-s5-prop-1 .statement tag=011N}

设$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$为框架半单李代数，R根系为$(\mathfrak{g},\mathfrak{h})$。令G为使B保持稳定的$s\in$Aut($\mathfrak{g},\mathfrak{h}$)的集合，并且使得$s(X_{\alpha}) =X_{\varepsilon(s)\alpha}$对于$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B}))$的自同构的其他字集合中的所有$\alpha \in B ($。那么$\varepsilon$到G的限制就是从G到Aut(R$,B$)的同构。

如果$s\in G$，显然$\varepsilon (s)\in$Aut(R$,B$)。另一方面，映射

$\varepsilon |G : G\rightarrow$ 自动(R$,B$)

是 Th 双射的。 2 个§4, no. 4。

### 2. 自同构分裂的半单李代数

令 E 为可​​交换的群，且 $A =\bigoplus_{\gamma\in E}A^{\gamma}$ 为 E 分级的代数。对于从群 E 到乘法群 $k^*$ 的任何同态 $\varphi$，令 $f(\varphi )$ 为从 A 到 A 的 $k$ 线性映射，其中限制与每个$A^{\gamma}$ 的位似的比率$\varphi (\gamma )$；显然，$f(\varphi )$是分级代数A的自同构，$f$是同态，从群Hom(E$, k^*$)到分级代数A的自同构的群。

令$\mathfrak{h}$为$\mathfrak{g}$的分裂嘉当子代数，以及$(\mathfrak{g},\mathfrak{h})$的R根系。回想一下，P(R)（分别为 Q(R)）表示 R 的权（分别为根式权）的群。

$T_P=$Hom(P(R)$, k^*$)$T_Q=$Hom(Q(R)$, k^*$)。

我们可以将$\mathfrak{g}=\mathfrak{g}^0+\sum_{\alpha\in R}\mathfrak{g}^{\alpha}$视为Q(R)分级的代数。前面从$T_Q$到Aut($\mathfrak{g},\mathfrak{h}$)的注定义典范同态，在本段中用$f$表示。另一方面，典范嵌入从Q(R)到P(R)定义同态从$T_P$到$T_Q$，用$q:$表示

$T_P\longrightarrow^qT_Q\longrightarrow^f$自动（$\mathfrak{g},\mathfrak{h}$）。

如果$s\in$ Aut($\mathfrak{g},\mathfrak{h}$)，则令$s^*$为$^t(s|\mathfrak{h})^{-1}$到Q(R)的限制。那么，对于所有$\varphi \in T_Q$，

$$
f(\varphi \circ s^*) =s^{-1}\circ f(\varphi )\circ s \tag{1}
$$

事实上，设 $\gamma \in Q(R)$ 和 $x\in \mathfrak{g}^{\gamma}$；然后 $sx\in \mathfrak{g}^{s^*\gamma}$ 和

$$
f(\varphi \circ s^*)x= (\varphi \circ s^*)(\gamma ).x=s^{-1}(\varphi (s^*\gamma )sx) = (s^{-1}\circ f(\varphi )\circ s)(x)
$$

#### 命题 2 {#lie-viii-s5-prop-2 .statement tag=011O}

序列 / 同态

1 $\longrightarrow T_Q\longrightarrow^f$ 自动($\mathfrak{g},\mathfrak{h}$)$\longrightarrow^{\varepsilon}$ A(R) $\longrightarrow$ 1

是准确的。

a) 让 $\varphi \in$ Ker $f$。然后 $\varphi (\alpha ) = 1$ 代表所有 $\alpha \in R$。因为 R 生成群 $Q(R),\varphi$ 是 $T_Q$ 的单位元素。

b) 设 $\varphi \in T_Q$。 $f(\varphi )$到$\mathfrak{h}=\mathfrak{g}^0$的限制是恒等式，所以

我$f\subset$ Ker$\varepsilon$。

c) 设 $s\in$ Ker$\varepsilon$。然后$s|\mathfrak{h}=$Id$_{\mathfrak{h}}$。对于所有$\alpha \in R$，我们有$s(\mathfrak{g}^{\alpha}) =\mathfrak{g}^{\alpha}$，并且存在一个$t_{\alpha}\in k^*$，使得对于所有$x\in \mathfrak{g}^{\alpha}$有$sx=t_{\alpha}x$。记下条件即$s\in$Aut($\mathfrak{g}$)，我们得到关系

$t_{\alpha}t_{-\alpha}= 1$ 所有人 $\alpha \in R$

$t_{\alpha}t_{\beta}=t_{\alpha+\beta}$当$\alpha , \beta , \alpha +\beta \in R$。

在这些条件下，存在$\varphi \in T_Q$，使得$\varphi (\alpha ) =t_{\alpha}$适用于所有$\alpha \in R$（第VI, §1, no. 6章，第19号提案的Cor.2）。然后$s=f(\varphi )$。因此，Ker $\varepsilon \subset$ Im $f$。

d) §2, no. 2，Cor，在 $\varepsilon$ 包含 W(R) 下的 Aut($\mathfrak{g},\mathfrak{h}$) 像。的 Th。 2，以及命题 1 的包含 Aut(R$,B$)。因此，像等于 A(R)。

#### 推论 1 {#lie-viii-s5-prop-2-cor-1 .statement tag=011P}

令$(B,(X_{\alpha})_{\alpha\in B})$为$(\mathfrak{g},\mathfrak{h})$的框架。令 G 为 $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) 的集合，从而保持框架不变。那么Aut($\mathfrak{g},\mathfrak{h}$)就是G和$\varepsilon^{-1}(W(R))$的半直接乘积。

事实上，根据第 1 条命题，$G\cap \varepsilon^{-1}(W(R)) =\{1\}$，并且

自动($\mathfrak{g},\mathfrak{h}$) $= G.\varepsilon^{-1}(W(R))$

因为 $\varepsilon$ 是满射的（命题 2）。

#### 推论 2 {#lie-viii-s5-prop-2-cor-2 .statement tag=011Q}

群 $\varepsilon^{-1}(W(R))$ 在 $(\mathfrak{g},\mathfrak{h})$ 的帧的集合上进行简单传递操作。

事实上，Aut($\mathfrak{g},\mathfrak{h}$) 在 $(\mathfrak{g},\mathfrak{h})$ 到 §4, no. 4 的框架集合上进行传递操作，Th。 2.Cor。 2 现在来自 Cor. 1.

#### 推论 3 {#lie-viii-s5-prop-2-cor-3 .statement tag=011R}

令B为R的基。群Ker$\varepsilon =f(T_Q)$在形式$(B,(X_{\alpha})_{\alpha\in B})$的$(\mathfrak{g},\mathfrak{h})$的帧的集合上进行简单传递操作。

这直接来自于提案 2。

设$\alpha \in R,X_{\alpha}\in \mathfrak{g}^{\alpha},X_{-\alpha}\in \mathfrak{g}^{-\alpha}$使得$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$。我们已经看到（§2, no. 2，Th.2），对于初等自同构的所有$t\in k^*$，限制

$$
\theta_{\alpha}(t) =e^{adtX_{\alpha}}e^{adt^{-1}X_{-\alpha}}e^{adtX_{\alpha}}
$$

到$\mathfrak{h}$是$s_{\alpha}$中的转置；所以$\varepsilon (\theta_{\alpha}(t)) =s_{\alpha}$，因而$\theta_{\alpha}(t)\theta_{\alpha}(-1)\in$ Ker $\varepsilon$。

#### 引理 1 {#lie-viii-s5-lem-1 .statement tag=011S}

设$\alpha \in R$和$t\in k^*$。设从 Q(R) 到 $k^*$ $\varphi$ 为同态 $\lambda  \rightarrow t^{\lambda(H_{\alpha})}$。然后$f(\varphi ) =\theta_{\alpha}(t)\theta_{\alpha}(-1)$。

令 $\rho$ 为与 $X_{\alpha}$ 伴随的 $\mathfrak{g}$ 上的 $\mathfrak{s}\mathfrak{l}(2, k)$ 的表示。令$\pi$为$\mathbf{S}\mathbf{L}(2, k)$中与$\rho$兼容的表示。介绍§1, no. 5中的记号$\theta (t), h(t)$。由于$\rho (H) =$和$H_{\alpha}$，$\mathfrak{g}^{\lambda}$的元素对于$\rho$来说是权$\lambda (H_{\alpha})$。到§2，没有。 $2,\theta_{\alpha}(t)\theta_{\alpha}(-1) =\pi (\theta (t)\theta (-1)) =\pi (h(t))$。因而，$\theta_{\alpha}(t)\theta_{\alpha}(-1)$与$\mathfrak{g}^{\lambda}$的限制是位似与$t^{\lambda(H_{\alpha})}($§1, no. 5之比，命题6），因此引理。

#### 命题 3 {#lie-viii-s5-prop-3 .statement tag=011T}

复合材料的像同态

$T_P\longrightarrow^qT_Q\longrightarrow^f$自动($\mathfrak{g},\mathfrak{h}$)

包含在 Aut$_e(\mathfrak{g})$ 中。

设B为R的基，则$(H_{\alpha})_{\alpha\in B}$为$R^{\vee}$的基，$\mathfrak{h}^*$中$(H_{\alpha})_{\alpha\in B}$的对偶基为群P(R)的基。因此群$T_P$是由同态$\lambda  \rightarrow t^{\lambda(H_{\alpha})}(t\in k^*, \alpha \in B)$生成的。如果$\varphi$是这样的同态到Q(R)的限制，引理1证明$f(\varphi )\in$Aut$_e(\mathfrak{g})$，因此命题。

设$\overline{k}$为$k$的代数闭包。与$\mathfrak{g}$自同构$s\otimes 1$或$\mathfrak{g}\otimes_k\overline{k}$中的任意自同构$s$相关联的映射是从Aut($\mathfrak{g}$)到Aut($\mathfrak{g}\otimes_k\overline{k}$)的单同态。我们用Aut$_0(\mathfrak{g})$表示Aut($\mathfrak{g}$)的正常子群，即在此同态下的Aut$_e(\mathfrak{g}\otimes_k\overline{k})$的逆像；这是$\mathfrak{g}$自同构集合，将基域从$k$延伸到$\overline{k}$就成为基本的。很明显，Aut$_e(\mathfrak{g})$ 独立于选择或 $\overline{k}$，并且 Aut$_e(\mathfrak{g})\subset$ Aut$_0(\mathfrak{g})$。 群 Aut$_0(\mathfrak{g})$ 和 Aut$_e(\mathfrak{g})$ 可以不同（第 VII, §13, no. 1 章）。如果$\mathfrak{h}$是$\mathfrak{g}$中的嘉当子代数，则将

自动$_e(\mathfrak{g},\mathfrak{h}) =$自动$_e(\mathfrak{g})\cap$自动($\mathfrak{g},\mathfrak{h}$)、自动$_0(\mathfrak{g},\mathfrak{h}) =$自动$_0(\mathfrak{g})\cap$自动($\mathfrak{g},\mathfrak{h}$)。

#### 引理 2 {#lie-viii-s5-lem-2 .statement tag=011U}

令$\mathfrak{h}$为$\mathfrak{g}$的分裂嘉当子代数，以及$s\in$Aut$_0(\mathfrak{g},\mathfrak{h})$。假设$s$到$\sum_{\alpha\in R}\mathfrak{g}^{\alpha}$中的限制不像特征值那样为1。

然后$\varepsilon (s) = 1$。

到$k$的扩张，我们就减少到$s\in$Aut$_e(\mathfrak{g},\mathfrak{h})$的情况。 $s-1$ 的零空间的维数至少是昏暗的 $\mathfrak{h}$（第 VII, §4, no. 4 章，第 9 条命题）。因而 $(s-1)|\mathfrak{h}$ 是幂零的。由于$s|\mathfrak{h}\in A(R^{\vee}),s|\mathfrak{h}$是有限的阶，因此半单（第V，附录，命题2）。因而，$(s-1)|\mathfrak{h}= 0$，证明了$\varepsilon (s) = 1$。

#### 引理 3 {#lie-viii-s5-lem-3 .statement tag=011V}

(i) 设 $m= (P(R) : Q(R))$。如果$\varphi$是$T_Q$中元素的第$m$第幂，则$\varphi \in q(T_P)$。

(ii) 如果 $k$ 是代数闭的，则 $q(T_P) = T_Q$。

存在 P(R) 的基 $(\lambda_1, . . . , \lambda_l)$ 和整数 $n_1\geq 1, . . . , n_l\geq 1$，使得 $(n_1\lambda_1, . . . , n_l\lambda_l)$ 是 Q(R) 的基。我们有$m=n_1. . . n_l$。设$\psi \in T_Q$并放入$\psi (n_1\lambda_1) =t_1, . . . , \psi (n_l\lambda_l) =t_l$。对于 $i= 1, . . . , l$，输入 $m_i=$ $\prod_{j\not=i}n_j$。令$\chi$为$T_P$的元素，使得$\chi (\lambda_1) =t^{m_1}_1, . . . , \chi (\lambda_l) =t^{m_l}_l$。然后

$$
\chi (n_i\lambda_i) =t^{m_in_i}_i=t^m_i= (\psi^m)(n_i\lambda_i)
$$

所以$\chi |Q(R) =\psi^m$。这就证明了(i)。如果$k$是代数闭的，$k^*$的每个元素都是$k^*$的元素的第$m$第幂，所以$T_Q$的每个元素都是第$m$ $T_Q$元素幂；因此，(ii) 由(i) 得出。

#### 命题 4 {#lie-viii-s5-prop-4 .statement tag=011W}

我们有$f(T_Q)\subset$Aut$_0(\mathfrak{g},\mathfrak{h})$和$\varepsilon^{-1}(W(R)) =$Aut$_0(\mathfrak{g},\mathfrak{h})$。

a) 令 $\varphi \in T_Q$ 且令 $\overline{k}$ 为代数闭包 / $k$。由引理 $3,\varphi$ 扩展至元素前往 Hom(P(R)$, k^*$)。根据第 3 条命题，

$f(\varphi )\otimes 1\in$自动$_e(\mathfrak{g}\otimes_k\overline{k},\mathfrak{h}\otimes_k\overline{k})$。

因此，$f(\varphi )\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$，以及 Ker $\varepsilon \subset$ Aut$_0(\mathfrak{g},\mathfrak{h})$。

b) Aut$_e(\mathfrak{g},\mathfrak{h})$ 的像在 $\varepsilon$ 包含 W(R) 下（§2, no. 2，Th. 2 的 Cor.）。鉴于a)，我们看到$\varepsilon^{-1}(W(R))\subset$Aut$_0(\mathfrak{g},\mathfrak{h})$。

c) 仍有待证明Aut$_0(\mathfrak{g},\mathfrak{h})\subset \varepsilon^{-1}(W(R))$。鉴于b)，只需证明$\varepsilon$(Aut$_0(\mathfrak{g},\mathfrak{h})$)$\cap$Aut(R$,B$)，其中B表示R的基，约化至$\{1\}$。

令 $s\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$ 使得 $\varepsilon (s)\in$ Aut(R$,B$)。由 $\varepsilon (s)$ 生成的 A(R) 的子群在 R 上具有轨道的有限数。令 U 为基数 $r$ 和 $\mathfrak{g}^U=\sum_{\beta\in U}\mathfrak{g}^{\beta}$ 的轨道。设 $\beta_1\in U$，并代入$\beta_i=\varepsilon (s)^{i-1}\beta_1$

$1\leq i\leq r$，所以$U =\{\beta_1, . . . , \beta_r\}$。令$X_{\beta_1}$为$\mathfrak{g}^{\beta_1}$的非零元素，并将$X_{\beta_i}=s^{i-1}X_{\beta_1}$作为$1\leq i\leq r$。存在$c_U\in k^*$使得$s^rX_{\beta_1}=$$c_UX_{\beta_1}$，因此对于所有$i$来说$s^rX_{\beta_i}=c_UX_{\beta_i}$，因而$s^r|\mathfrak{g}^U=c_U.1$。设 $\varphi \in T_Q$ 和 $s'=s\circ f(\varphi )$，通过 a) 是 Aut$_0(\mathfrak{g},\mathfrak{h})$ 的元素。我们有 ${s'}^r|\mathfrak{g}^U=c'_U.1$，其中

$$
c'_U=c_U\prod_{i=1}^r\varphi (\beta_i) =c_U\varphi (\sum_{i=1}^r\beta_i)
$$

输入$B =\{\alpha_1, . . . , \alpha_l\}$和$\sum_{i=1}^r\beta_i=\sum_{j=1}^lm^U_j\alpha_j$。自 $\varepsilon (s)\in$ Aut(R$,B$) 起，

$m^U_j$ 与整数具有相同的符号，但并非所有零。我们有

$$
c'_U=c_U\prod_{j=1}^l\varphi (\alpha_j)^{m^U_j}
$$

现在可以选择$\varphi$，这样每个轨道U就有$c'_U\not= 1$；事实上，这个约化选择$k^*$的元素$\varphi (\alpha_1) =t_1, . . . , \varphi (\alpha_l) =t_l$，它们不会被$t_1, . . . , t_l$中的有限多项式数湮灭，不完全相同零。对于这样的选择除$\varphi ,\varepsilon (s') = 1$乘以引理2，所以

$$
\varepsilon(s)=\varepsilon(s')\varepsilon(f(\varphi))^{-1}=1.
$$

#### 推论{#lie-viii-s5-n2-cor-1 .statement tag=01J0}

— 令 $B$ 为 $R$ 中的基。 群$\operatorname{Aut}(\mathfrak g,\mathfrak h)$同构于群$\operatorname{Aut}(R,B)$和$\operatorname{Aut}_0(\mathfrak g,\mathfrak h)$的半直接乘积。

这是根据 Cor. 1 提案得出的。提案 2 中的第 1 条和提案 4。

#### 注 {#lie-viii-s5-n2-rem-1 .statement tag=011X}

令$\varepsilon',\varepsilon''$为$\varepsilon$至$\operatorname{Aut}_0(\mathfrak g,\mathfrak h)$、$\operatorname{Aut}_e(\mathfrak g,\mathfrak h)$中的限制。令$f'$为同态，从$T_P$到$\operatorname{Aut}_e(\mathfrak g,\mathfrak h)$，由$f$经由典范嵌入从$Q(R)$到$P(R)$诱导。前面我们建立了如下交换律图表：
$$
\begin{array}{ccccccccc}
1&\longrightarrow&T_Q&\xrightarrow{\ f\ }&\operatorname{Aut}(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon\ }&A(\mathbf R)&\longrightarrow&1\\
&&\uparrow&&\uparrow&&\uparrow&&\\
1&\longrightarrow&T_Q&\xrightarrow{\ f\ }&\operatorname{Aut}_0(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon'\ }&W(\mathbf R)&\longrightarrow&1\\
&&\uparrow^{q}&&\uparrow&&\uparrow&&\\
&&T_P&\xrightarrow{\ f'\ }&\operatorname{Aut}_e(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon''\ }&W(\mathbf R)&\longrightarrow&1
\end{array}
$$
其中$q$以外的垂直箭头表示典范嵌入。我们已经看到（命题 2 和命题 4）前两行是准确的。在第三行中，同态$\varepsilon''$是满射（§2, no. 2，Th.2的Cor.）；可以证明它的核是$f'(T_P)$（§7，Exerc.26d））。

### 3. 可拆分的自同构半单李代数

#### 命题 5 {#lie-viii-s5-prop-5 .statement tag=01J1}

— 假设 $\mathfrak g$ 是可分割的。 群 $\operatorname{Aut}_0(\mathfrak g)$ 在 $\mathfrak g$ 的帧的集合上进行简单传递操作。

令$e_1=(\mathfrak g,\mathfrak h_1,B_1,(X^1_\alpha)_{\alpha\in B_1})$、$e_2=(\mathfrak g,\mathfrak h_2,B_2,(X^2_\alpha)_{\alpha\in B_2})$为$\mathfrak g$的两个框架。 $\operatorname{Aut}_0(\mathfrak g)$中至少存在一个元素将变换$e_1$转化为$e_2$（命题1和命题4）。设$\overline{k}$为$k$的代数闭包。 $\operatorname{Aut}_e(\mathfrak g\otimes_k\overline{k})$存在元素，变换$\mathfrak h_1\otimes_k\overline{k}$进入$\mathfrak h_2\otimes_k\overline{k}$（第VII, §3, no. 2，第1章）。因此，根据 Prop. 4 和 Cor.根据命题2的2，存在$\operatorname{Aut}_e(\mathfrak g\otimes_k\overline{k})$的元素$\varphi$，即变换将$\mathfrak g\otimes_k\overline{k}$的框架$(\mathfrak g\otimes_k\overline{k},\mathfrak h_1\otimes_k\overline{k},B_1,(X^1_\alpha)_{\alpha\in B_1})$纳入框架$(\mathfrak g\otimes_k\overline{k},\mathfrak h_2\otimes_k\overline{k},B_2,(X^2_\alpha)_{\alpha\in B_2})$。由于$\mathfrak h_1$和$X^1_\alpha$（分别是$\mathfrak h_2$和$X^2_\alpha$）生成$\mathfrak g_1$（分别是$\mathfrak g_2$），我们有$\varphi(\mathfrak g_1)=\mathfrak g_2$，所以$\varphi$是形式 $\psi\otimes 1$，其中 $\psi\in\operatorname{Aut}_0(\mathfrak g)$，以及 $\psi$ 变换 $e_1$ 到 $e_2$。

#### 推论 1 {#lie-viii-s5-prop-5-cor-1 .statement tag=01J2}

— 令$(\mathfrak g,\mathfrak h,B,(X_\alpha)_{\alpha\in B})$为$\mathfrak g$的框架，并且$G$群（与$\operatorname{Aut}(R,B)$同构）为$\mathfrak g$的自同构，使该框架保持不变。那么$\operatorname{Aut}(\mathfrak g)$就是$G$和$\operatorname{Aut}_0(\mathfrak g)$的半直接乘积。

事实上，$\operatorname{Aut}(\mathfrak g)$变换$(\mathfrak g,\mathfrak h,B,(X_\alpha)_{\alpha\in B})$的每个元素都会进入$\mathfrak g$的框架。根据命题 5，$\operatorname{Aut}(\mathfrak g)$ 模$\operatorname{Aut}_0(\mathfrak g)$ 的每个陪集恰好在一个点中满足$G$。

Q.E.D.

这是从 Cor 得出的。 1 群 Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$可以与Aut(R$,B$)识别，并且与R的Dynkin图的自同构的群同构。

#### 推论 2 {#lie-viii-s5-prop-5-cor-2 .statement tag=01J3}

Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$，当$\mathfrak{g}$是型$A_1,B_n(n\geq 2)$、$C_n(n\geq 2)$、$E_7,E_8,F_4,G_2$的可分割简单李代数时。当$\mathfrak{g}$为型、$A_n(n\geq 2)$、$D_n(n\geq 5)$、$E_6$时，商Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$为阶2；当$\mathfrak{g}$为型$D_4$时，它与$\mathfrak{S}_3$同构的。

这是从 Cor 得出的。 1 和章。 VI，板片I至IX。

#### 注 1 {#lie-viii-s5-n3-rem-1 .statement tag=011Z}

令$e_1= (\mathfrak{g},\mathfrak{h}_1,B_1,(X_{\alpha}^1)_{\alpha\in B_1}),e_2= (\mathfrak{g},\mathfrak{h}_2,B_2,(X_{\alpha}^2)_{\alpha\in B_2})$、$e'_2= (\mathfrak{g},\mathfrak{h}_2,B_2,(Y_{\alpha}^2)_{\alpha\in B_2})$为Aut$_0(\mathfrak{g})$的$\mathfrak{g}$和$s$（分别为$s'$）元素，即变换$e_1$到$e_2$（分别为$e'_2$）。然后$s|\mathfrak{h}_1=s'|\mathfrak{h}_1$。事实上，$s^{'-1}s\in$Aut$_0(\mathfrak{g},\mathfrak{h}_1)$和$s^{'-1}s(B_1) = B_1$，所以$\varepsilon (s^{'-1}s) = 1$。

#### 注 2 {#lie-viii-s5-n3-rem-2 .statement tag=0120}

令X为对$(\mathfrak{h},B)$的集合，其中$\mathfrak{h}$为$\mathfrak{g}$的分裂嘉当子代数，以及$(\mathfrak{g},\mathfrak{h})$的根系的B基。如果$x= (\mathfrak{h},B)$和$x'= (\mathfrak{h}',B')$是X中的两个元素，则存在$s\in$Aut$_0(\mathfrak{g})$将变换$x$转化为$x'$（命题5），以及限制$s_{x',x}$ $s$ 到 $\mathfrak{h}$ 不依赖于$s$ (注 1) 的选择。特别是，如果$x, x', x''\in X$和$s_{x,x}= 1$则为$s_{x'',x'}\circ s_{x',x}=s_{x'',x}$。 集合家庭 $(h_x)_{x\in X}$ 满足条件

$a)h_x\in \mathfrak{h}$如果$x= (\mathfrak{h},B)$

$b)s_{x',x}(h_x) =h_{x'}$如果$x, x'\in X$

以一种自然的方式向量空间$\mathfrak{h}(\mathfrak{g})$，我们有时将其称为$\mathfrak{g}$的规范嘉当子代数。对于$x= (\mathfrak{h},B)$和$x'= (\mathfrak{h}',B'),s_{x',x}$，将B带到$B'$，因此$(\mathfrak{g},\mathfrak{h})$的根系到$(\mathfrak{g},\mathfrak{h}')$的根系；由此可见，$\mathfrak{h}(\mathfrak{g})$的对偶$\mathfrak{h}(\mathfrak{g})^*$自然会配备根系$R(\mathfrak{g})$以及$R(\mathfrak{g})$的基$B(\mathfrak{g})$。我们有时说$R(\mathfrak{g})$是$\mathfrak{g}$的规范根系，$B(\mathfrak{g})$是它的典范基。 群 Aut($\mathfrak{g}$) 在 $\mathfrak{h}(\mathfrak{g})$ 上运行，使 $R(\mathfrak{g})$ 和 $B(\mathfrak{g})$ 保持稳定； Aut($\mathfrak{g}$) 的元素在 $\mathfrak{h}(\mathfrak{g})$ 上进行平凡操作的是 Aut$_0(\mathfrak{g})$ 的那些。

#### 命题 6 {#lie-viii-s5-prop-6 .statement tag=0121}

令$\mathfrak{h}$为$\mathfrak{g}$的分裂嘉当子代数。我们有 no. 1 中的记号、Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$.Ker $\varepsilon =$ Aut$_e(\mathfrak{g}).f(T_Q)$。

§3, no. 3，科。第 10 号提案，Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$.Aut$_0(\mathfrak{g},\mathfrak{h})$。另一方面，$\varepsilon$(Aut$_e(\mathfrak{g},\mathfrak{h})$)$\supset W(R)$ by §2, no. 2，Cor。的 Th。 2、所以Aut$_0(\mathfrak{g},\mathfrak{h}) =$Aut$_e(\mathfrak{g},\mathfrak{h})$.Ker$\varepsilon$。

#### 注 3 {#lie-viii-s5-n3-rem-3 .statement tag=0122}

命题 6 表明典范同态

$\iota : T_Q/$我(T$_P$)$\rightarrow$自动$_0(\mathfrak{g})/$自动$_e(\mathfrak{g})$,

由图表在 no. 2 中诱发，是满射的。特别是Aut$_e(\mathfrak{g})$ 包含导出群 of Aut$_0(\mathfrak{g})$；我们将看到（§11, no. 2，命题 3）它们实际上是相等的。而且，可以证明$\iota$是单射的，在其他字中$f(T_Q)\cap$Aut$_e(\mathfrak{g}) =f'(T_P)$，

（cf.§7，练习。$26d$）$)$。

#### 命题 7 {#lie-viii-s5-prop-7 .statement tag=0123}

令$\mathfrak{g}$为$\mathfrak{g}$的可分割半单李代数、$\mathfrak{b}$博雷尔子代数，以及$\mathfrak{p}_1$和$\mathfrak{p}_2$不同的抛物线子代数为$\mathfrak{g}$包含$\mathfrak{b}$。那么$\mathfrak{p}_1$和$\mathfrak{p}_2$就不是Aut$_0(\mathfrak{g})$下的共轭。

我们可以假设 $k$ 是代数封闭的。令$s\in$Aut$_0(\mathfrak{g})$使得$s(\mathfrak{p}_1) =\mathfrak{p}_2$。令 $\mathfrak{h}$ 为 $\mathfrak{b}\cap s(\mathfrak{b}) ($§3, no. 3 中包含的 $\mathfrak{g}$ 的嘉当子代数，命题 10)。由于$\mathfrak{h}$和$s(\mathfrak{h})$是$s(\mathfrak{b})$的嘉当子代数，因此存在$u\in [\mathfrak{b},\mathfrak{b}]$使得$e^{adu}(\mathfrak{h}) =s(\mathfrak{h})$（第VII, §3, no. 4章，第3章）。 替换$s$乘以$e^{-adu}s$，我们被简化为这样的情况：$s(\mathfrak{h}) =\mathfrak{h}$，$s$然后诱导在Weyl群W的$\mathfrak{h}$元素$\sigma$上$(\mathfrak{g},\mathfrak{h})$（提案 4）。令 C 为 Weyl 室相应的至 $\mathfrak{b}$。然后将$\mathfrak{p}_1$和$\mathfrak{p}_2$对应转换为C闭包中包含的$\mathfrak{h}_{\mathbf{R}}$的面$F_1$和$F_2$。我们有$\sigma (F_1) = F_2$。由于$\sigma \in W$，这意味着$F_1= F_2$（第V, §3, no. 3章，第2章）所以$\mathfrak{p}_1=\mathfrak{p}_2$。

#### 注 4 {#lie-viii-s5-n3-rem-4 .statement tag=0124}

令$\mathfrak{g}$为$\mathfrak{g}$、集合的抛物线子代数的可分割半单李代数、$\mathscr{P}$集合，Aut$_0(\mathfrak{g})$在其上运行。保留注的记号 2. 令 $\Sigma$ 为 $B(\mathfrak{g})$ 的子集。给予$\Sigma$相当于给予B的每个$x= (\mathfrak{h},B)\in X$、子集$\Sigma_x$，使得对于任何$x, x'\in X$，$s_{x',x}$取$\Sigma_x$到$\Sigma_{x'}$。令$\mathfrak{p}_x$为$\mathfrak{g}$相应的到$\Sigma_x$的抛物线子代数（§3, no. 4，注）。 Aut$_0(\mathfrak{g})$下的$\mathfrak{p}_x$的轨道是$x'\in X$的$\mathfrak{p}_{x'}$的集合。这个定义映射从$\mathfrak{P}(B(\mathfrak{g}))$到$\mathscr{P}/$Aut$_0(\mathfrak{g})$。这个映射是§3, no. 4的注的满射，并且是第7条命题的单射。

### 4. 扎里斯基拓扑自动 ($\mathfrak{g}$)

#### 命题 8 {#lie-viii-s5-prop-8 .statement tag=0125}

令V为向量空间$\mathfrak{g}$中的自同态中的集合。然后，Zariski 拓扑的 Aut($\mathfrak{g}$) 在 V 关闭（章节 VII，附录 I）。

令 K 为 $\mathfrak{g}$ 的杀戮形式。如果$s\in$自动（$\mathfrak{g}$），

$$
[sx, sy] = [x, y] \tag{2}
$$

$$
K(sx, sy) = K(x, y) \tag{3}
$$

对于所有$x, y\in \mathfrak{g}$。相反，对于所有$x, y\in \mathfrak{g}$，令$s$为V满足(2)和(3)中的元素。然后 Ker($s$) $= 0$，因此 $s$ 是双射，$s\in$ Aut($\mathfrak{g}$)。但是，对于所有$x, y\in \mathfrak{g}$、映射、$s \rightarrow [sx, sy]$和$s \rightarrow K(sx, sy)$，从V到$\mathfrak{g}$和$k$都是多项式。

#### 命题 9 {#lie-viii-s5-prop-9 .statement tag=0126}

设$\mathfrak{h}$为$\mathfrak{g}$的分裂嘉当子代数。

(i) 群 $f(T_Q)$ 在 Zariski 拓扑的 Aut($\mathfrak{g}$) 关闭。

(ii) 群 $f(q(T_P))$ 在 Zariski 拓扑的 $f(T_Q)$ 中密集。

断言 (i) 源自等式 $f(T_Q) =$ Aut($\mathfrak{g},\mathfrak{h}$)$\cap$Ker$\varepsilon$（命题 2）。输入$m= (P(R) : Q(R))$。设F为V上的多项式函数；我们假设F在$f(T_Q)$的每元素的第$m$第幂消失，并证明$F|f(T_Q) = 0$；鉴于引理 3，这将证明(ii)。

V的元素的集合$V'$在$\mathfrak{h}$上诱导身份并且离开每个$\mathfrak{g}^{\alpha}$稳定可以用$k^R$来识别。设$F'$为F到$V'=k^R$的限制；这是多项式函数。我们有$f(T_Q)\subset V'$。令$B = (\alpha_1, . . . , \alpha_l)$为R的基。对于所有$t= (t_1, . . . , t_l)\in k^{*B}$，令$\varphi (t)$为从Q(R)到群$k^*$即扩展$t$的同态。那么$F'(f(\varphi (t)))$可以写成有限的和

$$
\sum_{n_1,...,n_l\in\mathbf{Z}}c_{n_1,...,n_l}t^{n_1}_1. . . t^{n_l}_l= H(t_1, . . . , t_l)
$$

假设，

$$
0 = H(t^m_1, . . . , t^m_l) =\sum_{n_1,...,n_l\in\mathbf{Z}}c_{n_1,...,n_l}t^{mn_1}_1. . . t^{mn_l}_l
$$

对于所有$t_1, . . . , t_l\in k^*$。因此，$c_{n_1,...,n_l}$是$l$变量中多项式的系数，该多项式在$k^{*l}$上消失；因此它们都是零。

#### 命题 10 {#lie-viii-s5-prop-10 .statement tag=0127}

假设$\mathfrak{g}$是可分割的。

(i) 群 Aut$_e(\mathfrak{g})$ 在 Zariski 拓扑中的 Aut$_0(\mathfrak{g})$ 密集。

(ii) 群 Aut$_e(\mathfrak{g})$ 和 Aut$_0(\mathfrak{g})$ 在 Zariski 拓扑连接。

根据提案$3,f(q(T_P))\subset$ Aut$_e(\mathfrak{g})$。对于所有 $s\in$ Aut$_e(\mathfrak{g})$，第 9 号提案关闭了 Zariski 拓扑包含 $s.f(T_Q)$ 中的 $s.f(q(T_P))$。因此，Aut$_e(\mathfrak{g})$ 包含 Aut$_e(\mathfrak{g}).f(T_Q) =$ Aut$_0(\mathfrak{g})$ 关闭（提案 6）。这就证明了(i)。

设Aut$_e(\mathfrak{g}) =\Omega \cup \Omega '$为由Zariski拓扑中相对开放的子集形成的Aut$_e(\mathfrak{g})$的划分，并与$\Omega \not=\emptyset$。如果$\omega \in \Omega$且$x$是$\mathfrak{g}$的幂零元，则从$k$到Aut$_e(\mathfrak{g})$的映射$\tau :t \rightarrow \omega$exp($t$ad$x$)是多项式，因此在Zariski拓扑中连续；因而，$\tau (k)$是连通的；从$\omega \in \tau (k)$开始，我们有$\tau (k)\subset \Omega$。因而，$\Omega$.(exp ad $kx$)$\subset \Omega$，因而$\Omega$.Aut$_e(\mathfrak{g})\subset \Omega$和$\Omega =$Aut$_e(\mathfrak{g})$。这证明Aut$_e(\mathfrak{g})$已连接。由此可见，通过 (i)，Aut$_0(\mathfrak{g})$ 已连接。 Q.E.D.

我们将看到（§8, no. 4，命题 6 的 Cor.），Aut$_0(\mathfrak{g})$ 在 Zariski 拓扑中的V 中闭合，并且它是 Aut($\mathfrak{g}$) 的单位元素的连通分量。另一方面，Aut$_e(\mathfrak{g})$ 在 Zariski 拓扑中一般不会关闭。

\*假设$(\mathfrak{g},\mathfrak{h})$是分裂的。 群 Aut$_0(\mathfrak{g})$ 是连接的半单代数群 G 与平凡中心（伴随群）的群 $G(k)$ 的 $k$ 点。 群$f(T_Q)$等于$H(k)$，其中H是G与李代数$\mathfrak{h}$的嘉当子群。 G 的通用覆盖$\widetilde{G}$（代数意义上）中 H 的逆像 $\widetilde{H}$ 具有 $T_P$ 作为其 $k$ 点的群。 $G(k) =$ Aut$_0(\mathfrak{g})$ 中的 $\widetilde{G}(k)$ 的像是群 Aut$_e(\mathfrak{g})$。\*

### 5. 李群情形

#### 命题 11 {#lie-viii-s5-prop-11 .statement tag=0128}

假设 $k$ 是 $\mathbf{R},\mathbf{C}$ 或非离散完全超度量域。设$\mathfrak{h}$为$\mathfrak{g}$的分裂嘉当子代数。

(i) Aut($\mathfrak{g},\mathfrak{h}$) 是 Aut($\mathfrak{g}$) 与李代数 ad$\mathfrak{h}$ 的谎言子群。

(ii) $f(T_Q)$ 和 $(q\circ f)(T_P)$ 于 Aut($\mathfrak{g},\mathfrak{h}$) 子群开放。

(iii) Aut$_e(\mathfrak{g})$ 是 Aut($\mathfrak{g}$) 的开子群。

(iv) 如果$k=\mathbf{R}$或$\mathbf{C}$，Aut$_e(\mathfrak{g})$是Aut($\mathfrak{g}$)的恒等分量，在其他字Int($\mathfrak{g}$)中。

由章。 III, §3, no. 8，科。第 29 条命题 2，以及第 36 条命题 no. 10，Aut($\mathfrak{g},\mathfrak{h}$) 是 Aut($\mathfrak{g}$) 的谎言子群，其李代数是 ad $x(x\in \mathfrak{g})$ 的集合，使得 (ad $x$)$\mathfrak{h}\subset \mathfrak{h}$，在其他情况下字广告$\mathfrak{h}$。

让$H\in \mathfrak{h}$。存在具有以下属性的$\varepsilon  >0$：对于$t\in k$和$|t|< \varepsilon$，为所有$\gamma \in P(R)$定义了exp($t\gamma (H)$)，并且从P(R)到映射$\gamma  \rightarrow$exp($t\gamma (H)$)为同态$\sigma_t$ $k^*$。对于$|t|< \varepsilon$，定义了exp($t$ ad H)，诱导在$\mathfrak{h}$上的恒等式和诱导在$\mathfrak{g}^{\alpha}$位似上的恒等式，比率为$\sigma_t(\alpha )$；因此exp $t$广告$H\in (q\circ f)(T_P)$。鉴于 (i)，这证明了 Aut($\mathfrak{g},\mathfrak{h}$) 中 1 的$(q\circ f)(T_P)$ 包含邻域，因此是 Aut($\mathfrak{g},\mathfrak{h}$) 的开子群。 更不必说$,f(T_Q)$是Aut($\mathfrak{g},\mathfrak{h}$)的开子群。

对于所有 $\alpha \in R$，exp ad $\mathfrak{g}^{\alpha}\subset$ Aut$_e(\mathfrak{g})$。鉴于(ii)，Aut($\mathfrak{g}$)中Aut$_e(\mathfrak{g})$包含邻域为1，从而证明(iii)。

假设$k=\mathbf{R}$或$\mathbf{C}$。那么Aut$_e(\mathfrak{g})$包含在Aut($\mathfrak{g}$)的恒等分量C中(VII, §3, no. 1)，并由(iii)在Aut($\mathfrak{g}$)中打开。因此Aut$_e(\mathfrak{g}) = C$。最后，C = Int($\mathfrak{g}$) 由章节。 III, §9, no. 8，提案 30 (i)。

### 习题 {#lie-viii-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
