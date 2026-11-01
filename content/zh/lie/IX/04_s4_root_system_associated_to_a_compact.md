---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 4
section_title: Root system associated to a compact group
lang: zh
source: lie-vii-ix
book_pages: 304-324, 396-405
pdf_pages: 0311-0331, 0403-0412
extraction: native+ocr
subsections:
    - "no": 1
      title: THE GROUP X(H)
      page: 304
      pdf_page: 311
    - "no": 2
      title: NODAL GROUP OF A TORUS
      page: 305
      pdf_page: 312
    - "no": 3
      title: WEIGHTS OF A LINEAR REPRESENTATION
      page: 307
      pdf_page: 314
    - "no": 4
      title: ROOTS
      page: 309
      pdf_page: 316
    - "no": 5
      title: NODAL VECTORS AND INVERSE ROOTS
      page: 311
      pdf_page: 318
    - "no": 6
      title: FUNDAMENTAL GROUP
      page: 314
      pdf_page: 321
    - "no": 7
      title: SUBGROUPS OF MAXIMAL RANK
      page: 316
      pdf_page: 323
    - "no": 8
      title: ROOT DIAGRAMS
      page: 317
      pdf_page: 324
    - "no": 9
      title: COMPACT LIE GROUPS AND ROOT SYSTEMS
      page: 319
      pdf_page: 326
    - "no": 10
      title: AUTOMORPHISMS OF A CONNECTED COMPACT LIE GROUP
      page: 322
      pdf_page: 329
statements: 60
exercises: 22
content_sha256: ce1338953b9a31332ca83092904aa5e8e175f885714c5f5b74f653846b777cc5
translated_from: content/en/lie/IX/04_s4_root_system_associated_to_a_compact.md
translation_method: google
source_content_sha256: e5b8a3582b57fb78f4dd12b6e9730ed0ae0bc70a11963071c72fa1b2877b4759
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: f0faccf2a217327e5ab2fd6901c8ed39c557154ed8bb6ac40645187a22bf2760
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。 根系与紧凑型群相关

在第4至8段中，我们用G表示连接的紧李群，用T表示G的最大环面。我们用G的$\mathfrak{g}$（分别$\mathfrak{t}$）李代数（分别T）表示，用$\mathfrak{g}_{\mathbf{C}}$（分别$\mathfrak{t}_{\mathbf{C}}$）表示复数$\mathfrak{g}$（或$\mathfrak{t}$）的李代数，以及W相对于T（§2, no. 5）的G的Weyl 群。

### 1.群X(H)

设 H 为紧李群。用 X(H) 表示从 H 到拓扑群 $\mathbf{C}^*$ 连续同态的（交换）群。由章。 III, §8, no. 1，周四。 1、X(H)元素为李群态射；对于所有$a\in X(H)$，$a$的微分是$\mathbf{R}$线性映射$L(a) : L(H)\rightarrow L(\mathbf{C}^*)$。从现在开始，我们将$\mathbf{C}^*$的认同李代数与$\mathbf{C}$进行计算，使得$\mathbf{C}^*$重合的指数映射与映射$z \rightarrow e^z$从$\mathbf{C}$到$\mathbf{C}^*$。然后，与任意元素$a\in X(H)$相关联的是元素$L(a)\in$Hom$_{\mathbf{R}}(L(H),\mathbf{C})$；我们用Hom$_{\mathbf{C}}(L(H)_{(\mathbf{C})},\mathbf{C})$的$\delta (a)$元素表示它的对应（即，其限制到$L(H)\subset L(H)_{(\mathbf{C})}$等于$L(a)$）。

对于所有 $x\in L(H)$ 和所有 $a\in X(H)$，我们有

$a$(exp$_Hx$) $=e^{\delta(a)(x)}$,

由指数映射的函数性（第 III, §6, no. 4 章，命题 10）。

我们经常将群 X(H) 表示为相加；在这种情况下，我们用 $g^a$ 表示 $\mathbf{C}^*$ 的元素 $a(g)$。有了这个记号，我们就有了公式

$$
g^{a+b}=g^ag^b,g\in H, a, b\in X(H)
$$

和

（经验$_Hx$）$^a=e^{\delta(a)(x)}, x\in L(H), a\in X(H)$。

由于H是紧的，X(H)的元素取绝对值1的复数的子群$\mathbf{U}=\mathbf{U}(1,\mathbf{C})$中的值，因此X(H)可以用连续的群来辨识（或解析）同态从H到$\mathbf{U}$。由此可见，对于所有$a\in L(H)$，映射$L(a)$在$\mathbf{C}$的子空间$\mathbf{R}i$中取值，因此$\delta (a)$映射L(H) $\mathbf{R}i$。

如果 H 是可交换的，X(H) 只是 H 的（离散）对偶群（谱理论，第 II, §1, no. 1）。如果 H 是可交换的且有限的，则 X(H) 可以用对偶有限群 D(H) = Hom$_{\mathbf{Z}}(H,\mathbf{Q}/\mathbf{Z})$ 来识别（其中，如VII, §4, no. 9、例 1 章中的代数所示，我们将认同 $\mathbf{Q}/\mathbf{Z}$ 与子群 / $\mathbf{C}^*$ 由同态 $r \rightarrow$ exp(2$\pi ir$))。

对于紧李群中的任何态射$f: H\rightarrow H'$，我们用$X(f)$同态$a \rightarrow a\circ f$表示从$X(H')$到X(H)。如果K是闭集

正常子群 / 紧李群 H，我们有正合序列 / $\mathbf Z$-模块
$$
0\longrightarrow X(H/K)\longrightarrow X(H)\longrightarrow X(K).
$$

#### 命题 1 {#lie-ix-s4-prop-1 .statement tag=01JH}

— *对于任何紧李群* H，** $\mathbf Z$-*模* $X(H)$ *是有限的型。如果* H *连通，则免费。*

首先假设H是连通的； $X(H)$的每个元素都消失在H的导出群$D(H)$上，因此我们有同态$X(H/D(H))\longrightarrow X(H)$。但$H/D(H)$是连通且可交换的，因此是环面，而$X(H/D(H))$是有限型的自由$\mathbf Z$模（*谱理论*，第II, §2, no. 1章，第1条命题的Cor.2）。一般情况下，根据序列的正确性得出
$$
0\longrightarrow X(H/H_0)\longrightarrow X(H)\longrightarrow X(H_0),
$$
其中 $X(H_0)$ 不受有限型的影响，$X(H/H_0)$ 是有限的，$X(H)$ 是有限的型。

#### 命题 2 {#lie-ix-s4-prop-2 .statement tag=01JI}

— *设* H *是可交换的紧李群，并且* $(a_i)_{i\in I}$ *元素的族* $X(H)$； *该* $a_i$ *生成* $X(H)$ *当且仅当* $\operatorname{Ker}a_i$ *约化到单位元素的交。*

作者：*光谱理论*，第一章。 II, §1, no. 7，周四。 4、$a_i$的核的正交补为$a_i$生成的$X(H)$的子群$A_i$；由*loc。引用。*，Cor。 2 Th。 4、$\bigcap\operatorname{Ker}a_i$的正交补是由$A_i$生成的$X(H)$的子群，因此是命题。

### 2.节点群 OF 环面

环面 S 的*节点群*，用 $\Gamma(S)$ 表示，是指数映射 $\mathscr L(S)\longrightarrow S$ 的核。这是$\mathscr L(S)$的离散子群，其秩等于S的维数，以及$\Gamma(S)$的扩展典范嵌入的$\mathbf R$线性映射$\mathbf R\otimes_{\mathbf Z}\Gamma(S)\longrightarrow\mathscr L(S)$ $\mathscr L(S)$ 是双射的。通过商同构得到诱导
$$
\mathbf R/\mathbf Z\otimes_{\mathbf Z}\Gamma(S)\longrightarrow S.
$$

对于例，$\mathbf U$的节点群$\Gamma(\mathbf U)$是$\mathscr L(\mathbf U)=i\mathbf R$的子群$2\pi i\mathbf Z$。

对于环$f:S\longrightarrow S'$的任何态射，用$L(f)$诱导的$\Gamma(f)$同态$\Gamma(S)\longrightarrow\Gamma(S')$表示。我们有一个可交换的图表
$$
\begin{array}{ccccccccc}
0&\longrightarrow&\Gamma(S)&\longrightarrow&\mathscr L(S)&\xrightarrow{\exp_S}&S&\longrightarrow&0\\
&&\downarrow{\Gamma(f)}&&\downarrow{\mathscr L(f)}&&\downarrow f&&\\
0&\longrightarrow&\Gamma(S')&\longrightarrow&\mathscr L(S')&\xrightarrow{\exp_{S'}}&S'&\longrightarrow&0.
\end{array}
\tag{1}
$$

让$a\in X(S)$； 应用前面的态射从S到$\mathbf U$由a定义，我们看到no. 1映射$\Gamma(S)$到$2\pi i\mathbf Z$的$\mathbf C$线性映射$\delta(a):\mathscr L(S)_{\mathbf C}\longrightarrow\mathbf C$。因此，我们可以通过将 $X(S)\times\Gamma(S)$ 定义 $\mathbf Z$ 双线性形式
$$
\langle a,X\rangle=\frac{1}{2\pi i}\delta(a)(X),\qquad a\in X(S),\quad X\in\Gamma(S).
\tag{2}
$$

#### 命题 3 {#lie-ix-s4-prop-3 .statement tag=01BP}

双线性形式 $(a, X) \rightarrow  \langle a, X\rangle$ 在 $X(S)\times \Gamma (S)$ 上是可逆的。

回想一下（代数，第IX），通过定义，这意味着与此双线性形式相关的线性映射$X(S)\rightarrow$Hom$_{\mathbf{Z}}(\Gamma (S),\mathbf{Z})$和$\Gamma (S)\rightarrow$Hom$_{\mathbf{Z}}(X(S),\mathbf{Z})$是双射的。

直接的如果命题的结论对于两个环都成立，那么对于他们的乘积也成立。因此，由于维数$n$的每个环面都同构于$\mathbf{U}^n$，所以我们被简化为$S =\mathbf{U}$的情况。在这种特殊情况下，断言是直接的。

设$f: S\rightarrow S'$为环面的态射。然后，线性映射 $X(f) : X(S')\rightarrow X(S)$ 和 $\Gamma (f) :\Gamma (S)\rightarrow \Gamma (S')$ 都是另一个的转置：对于所有 $a'\in X(S')$ 和所有 $X\in \Gamma$(S)，

$$
\langle X(f)(a'), X\rangle =\langle a', \Gamma (f)(X)\rangle \tag{3}
$$

#### 命题 4 {#lie-ix-s4-prop-4 .statement tag=01BQ}

令 S 和 $S'$ 为环面。从S到$S'$用李群态射$M(S,S')$群表示。 映射 $f \rightarrow X(f)$ 和 $f \rightarrow \Gamma (f)$ 分别是从 $M(S,S')$ 到 Hom$_{\mathbf{Z}}(X(S'),X(S))$ 和到 Hom$_{\mathbf{Z}}(\Gamma (S), \Gamma (S'))$ 的同构或群。

如果$f$是从S到$S'$的李群的态射，则同态$X(f)$只是光谱理论意义上的$f$的对偶，第1章。 II, §1, no. 7。 映射 $\varphi  \rightarrow \widehat{\varphi}$ 从 Hom$_{\mathbf{Z}}(X(S'),X(S))$ 到 $M(S,S')$ 在 loc 中定义。引用。是映射 $f \rightarrow X(f)$ 从 $M(S,S')$ 到 Hom$_{\mathbf{Z}}(X(S'),X(S))$ 的倒数；因此，后者是双射的。如果我们认同$\Gamma (S)$（或$\Gamma (S')$）与X（S）（或$X(S')$）的双$\mathbf{Z}$模（道具$3$）$,\Gamma (f)$重合与转置同态$X(f)$，因此命题。

#### 注 1 {#lie-ix-s4-n2-rem-1 .statement tag=01BR}

令 $f$ : S $\rightarrow S'$ 为 tori 的态射。与（1）相关的蛇图表（代数，第X, §1, no. 2）给出正合序列

0 $\longrightarrow$ 克尔$\Gamma (f)\longrightarrow$ 克尔$L(f)\longrightarrow$ 克尔$f\longrightarrow^d$ (4)

$\longrightarrow^d$焦化器$\Gamma (f)\longrightarrow$焦化器$L(f)\longrightarrow$焦化器$f\longrightarrow 0$。

特别是，假设 $f$ 是满射，且核 N 有限，因此我们有正合序列

0 $\longrightarrow$ N $\longrightarrow^i$ S $\longrightarrow^fS'\longrightarrow 0$,

其中 $i$ 是典范嵌入。那么，$L(f)$是双射的，并且（4）给出同构$N\rightarrow$Coker$\Gamma (f)$，因此正合序列

0 $\longrightarrow \Gamma (S)\overset{\Gamma(f)}{\longrightarrow}\Gamma (S')\longrightarrow$ N $\longrightarrow 0$。 (5)

此外，通过光谱理论，第一章。 II, §1, no. 7，周四。 4、序列

0 $\longrightarrow X(S')\overset{X(f)}{\longrightarrow}$ X(S) $\longrightarrow^{X(i)}$ X(N) $\longrightarrow$ 0 (6)

是准确的。

#### 注 2 {#lie-ix-s4-n2-rem-2 .statement tag=01BS}

根据命题4，从$M(\mathbf{U},S)$到$\Gamma (S)$的映射$f \rightarrow \Gamma (f)(2\pi i)$是同构；如果$a\in X(S) = M(S,\mathbf{U})$和$f\in M(\mathbf{U},S)$，则复合$a\circ f\in M(\mathbf{U},\mathbf{U})$是自同态$u \rightarrow u^r$，其中$r=\langle a, \Gamma (f)(2\pi i)\rangle$。从现在开始，我们将认同$M(\mathbf{U},\mathbf{U}) = X(\mathbf{U})$与$\mathbf{Z}$关联，$\mathbf{Z}$中的元素$r$关联到自同态$u \rightarrow u^r$；因此，对于上面的记号，

$$
a\circ f=\langle a, \Gamma (f)(2\pi i)\rangle
$$

#### 注 3 {#lie-ix-s4-n2-rem-3 .statement tag=01BT}

正合序列$0\rightarrow \Gamma (S)\rightarrow L(S)\longrightarrow^{exp_S}S\rightarrow 0$与$\Gamma (S)$的同构与S的基本群相关联，在续集中称为规范。对于环面$f: S\rightarrow S',\Gamma (f)$的任何态射，可以通过典范同构$\Gamma (S)\rightarrow \pi_1(S)$和$\Gamma (S')\rightarrow \pi_1(S')$以及由$f$诱导的同态$\pi_1(f) :\pi_1(S)\rightarrow \pi_1(S')$来识别。 注，这给出了正合序列（5）的另一个解释（cf.一般拓扑，第XI章，正在准备中）。

#### 注 4 {#lie-ix-s4-n2-rem-4 .statement tag=01BU}

$\mathbf{Z}$-模块$\delta : X(S)\rightarrow$ Hom$_{\mathbf{C}}(L(S)_{(\mathbf{C})},\mathbf{C})$和$\iota :\Gamma (S)\rightarrow L(S)_{(\mathbf{C})}(\iota$的同态由$\Gamma (S)$的典范嵌入诱导成L(S))扩展到同构 $\mathbf{C}$-向量空间

$u:\mathbf{C}\otimes X(S)\rightarrow$坎$_{\mathbf{C}}(L(S)_{(\mathbf{C})},\mathbf{C})$

$$
v:\mathbf{C}\otimes \Gamma (S)\rightarrow L(S)_{(\mathbf{C})}
$$

我们将在续集中将其称为规范。 注，如果我们扩展X(S)和$\Gamma (S)$之间的配对通过$\mathbf{C}$-线性到双线性形式$\ll ,\gg$在$(\mathbf{C}\otimes X(S))\times (\mathbf{C}\otimes \Gamma$(S))上，那么

$$
\langle u(a), v(b)\rangle = 2\pi i\ll a, b\gg
$$

### 3. 权线性表示

其中数$k$表示域$\mathbf{R}$或$\mathbf{C}$之一。

令V是$k$上的有限维向量空间，$\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$是V上相连的紧李群G的连续（因此实解析，第III, §8, no. 1，第1章）表示。 定义复数向量空间$\widetilde{V}$和连续表示$\widetilde{\rho}: G\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$如下：如果$k=\mathbf{C}$，集合$\widetilde{V} = V, \widetilde{\rho}=\rho$；如果$k=\mathbf{R}$、集合、$\widetilde{V} = V_{(\mathbf{C})}$和$\widetilde{\rho}$是$\rho$与典范同态$\mathbf{G}\mathbf{L}(V)\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$的复合。

对于所有$\lambda \in X(G)$，用$v\in \widetilde{V}$的$\widetilde{V}$由……组成的$\widetilde{V}_{\lambda}(G)$向量子空间表示，这样$\widetilde{\rho}(g)v=g^{\lambda}v$对于所有$g\in G$（cf.） VII, §1, no. 1）。按地点。引文，第 3 条命题中，$\widetilde{V}_{\lambda}(G)$（对于$\lambda$属于到X(G)）的和是直接的。此外：

#### 引理 1 {#lie-ix-s4-lem-1 .statement tag=01BV}

如果 G 是可交换的，则 $\widetilde{V}$ 是 $\lambda \in X(G)$ 的 $\widetilde{V}_{\lambda}(G)$ 的直和。

由于$\rho$是半单(§1, no. 1)，因此在$\rho$很简单的情况下证明引理就足够了。 在这种情况下，End( $\widetilde{V}$) 约化中 $\rho (G)$ 的交换子 Z 到同位 (代数，第 1 章)。 VIII, §3, no. 2，Th。 1）；因而，同态$\widetilde{\rho}$的像包含在GL($\widetilde{V}$)的子群$\mathbf{C}^*.1_V$中，并且存在$\lambda \in X(G)$使得$\widetilde{V} = \widetilde{V}_{\lambda}(G)$。

#### 定义 1 {#lie-ix-s4-def-1 .statement tag=01BW}

G 的表示 $\rho$ 的权，相对于 G 的最大环面 T，是 X(T) 的元素 $\lambda$，使得 $\widetilde{V}_{\lambda}(T)\not= 0$。

用$P(\rho ,T)$表示，如果T的选择、$\rho$的权相对于T的集合不存在混淆的可能性，则用$P(\rho )$表示。用引理1，

$$
\widetilde{V} =\bigoplus_{\lambda\in P(\rho ,T)}\widetilde{V}_{\lambda}(T) \tag{7}
$$

令$T'$为G的另一个最大环面和G的$g$元素，使得(Int$g$)$T = T'($§2, no. 2，Th。 2）。对于所有$\lambda \in X(T)$，

$\widetilde{\rho}(g)( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{\lambda'}(T')$，其中 $\lambda '=$ X(Int $g^{-1}$)$(\lambda )$。 (8)

最后，

X(整数$g$)$(P(\rho ,T')) = P(\rho ,T)$。 (9)

Weyl 群 $W = W_G(T)$ 在 $\mathbf{Z}$ 模 X(T) 的左侧通过 $w \rightarrow X(w^{-1})$ 进行运算；因而，对于$t\in T, \lambda \in X(T), w\in W$，我们有$t^{w\lambda}= (w^{-1}(t))^{\lambda}$。

#### 命题 5 {#lie-ix-s4-prop-5 .statement tag=01BX}

集合 $P(\rho ,T)$ 在Weyl 群 W 的运算下是稳定的。设$n\in N_G(T)$，并令$w$为其在W中的类；对于$\lambda \in X(T)$，我们有$\rho (n)( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{w\lambda}(T)$和暗淡$\widetilde{V}_{w\lambda}(T) =$暗淡$\widetilde{V}_{\lambda}(T)$。

公式(9)，与$T'= T, g=n$，意味着$P(\rho ,T)$在$w$下是稳定的；此外，$\widetilde{\rho}(n)$诱导同构从$\widetilde{V}_{\lambda}(T)$到$\widetilde{V}_{w\lambda}(T)$（公式（8）），因此命题。

#### 命题 6 {#lie-ix-s4-prop-6 .statement tag=01BY}

同态 $\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ 是单射当且仅当 $P(\rho ,T)$ 生成 $\mathbf{Z}$-模 X(T)。

同态 $\rho$ 是单射的当且仅当其限制到 T 是单射的（§2, no. 6，命题 9）。此外，由于典范同态$\mathbf{G}\mathbf{L}(V)\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$是单射的，我们可以通过$\widetilde{\rho}$来替换$\rho$。则从(7)可知，$\rho$到T的限制到T的核是$P(\rho ,T)$的元素核的交。因而，结论由no. 1的命题2得出。

$\mathfrak{g}\mathfrak{l}( \widetilde{V})$ 扩展至 $\mathbf{C}$ 的同态 - 李代数中的 $\mathfrak{t}$ 线性表示 $L(\rho )$

$$
\widetilde{L}(\rho ) :\mathfrak{t}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}( \widetilde{V})
$$

此外，回想一下 (no. 1)，我们已将 $\mathfrak{t}_{\mathbf{C}}$ 上的 X(T) 线性形式 $\delta (\lambda )$ 的每个元素 $\lambda$ 关联起来，这样

(exp$_Tx$)$^{\lambda}=e^{\delta(\lambda)(x)},x\in \mathfrak{t}$。 (10)

最后回想一下（第 VII, §1, no. 1 章），对于任何映射 $\mu:\mathfrak{t}_{\mathbf{C}}\rightarrow \mathbf{C}$，我们用 $v$ 的 $\widetilde{V}$ 由……组成的 $\widetilde{V}_\mu(\mathfrak{t}_{\mathbf{C}})$ 向量子空间表示，这样对于所有$(\widetilde{L}(\rho )(u))(v) =\mu(u).v$ $u\in \mathfrak{t}_{\mathbf{C}}$。

我们现在从 (7) 和 loc 中推出。引文，提案 3：

#### 命题 7 {#lie-ix-s4-prop-7 .statement tag=01BZ}

a) 对于所有$\lambda \in X(T)$，我们有$\widetilde{V}_{\lambda}(T) = \widetilde{V}_{\delta(\lambda)}(\mathfrak{t}_{\mathbf{C}})$。

b) $\widetilde{V}$$\mathfrak{t}_{\mathbf{C}}$权$P(\rho ,T)$至集合映射$\delta : X(T)\rightarrow$坎$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C})$诱导双射。

注首先，如果 W 通过关联到 $\mathfrak{t}_{\mathbf{C}}$ 的 W 自同态 $L(w)_{(\mathbf{C})}$ 中的任意元素 $w$ 对 $\mathfrak{t}_{\mathbf{C}}$ 进行操作，则映射 $\delta$ 与 W 上的运算兼容X（T）和坎$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C})$。

现在假设$k=\mathbf{R}$。用$\sigma$表示$\widetilde{V}$相对于V的共轭，由$\sigma (x+iy) =x-iy$定义为V中的$x, y$；对于$\widetilde{V}$的每个复数向量子空间E，$\widetilde{V}$有理数$\mathbf{R}$的最小的子空间和包含E是$E +\sigma (E)$。特别是，对于所有$\lambda \in X(T)$，存在V的实向量子空间$V(\lambda )$，使得$\widetilde{V}$的子空间$V(\lambda )_{(\mathbf{C})}$是$\widetilde{V}_{\lambda}(T) + \widetilde{V}_{-\lambda}(T)$（注即$\sigma ( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{-\lambda}(T)$）。我们有$V(\lambda ) = V(-\lambda )$，$V(\lambda )$是由$\rho$诱导的V上T的表示的同型成分。

### 4.根

G 相对于 T 的根是 G 的伴随表示的非零权。G 相对于 T 的根的集合表示为 $R(G,T)$，或者在不存在混淆风险的情况下简单地表示为 R。根据第 6 号提案，映射

$$
\delta : X(T)\rightarrow \mathfrak{t}^*_{\mathbf{C}}
$$

$(\mathfrak{t}^*_{\mathbf{C}}$ 表示复数向量空间 $\mathfrak{t}_{\mathbf{C}})$ 映射 $R(G,T)$ 双射到分裂的还原代数根的集合 $R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$（第VIII, §2, no. 2、注4章）。如果我们把

$$
\mathfrak{g}^{\alpha}= (\mathfrak{g}_{\mathbf{C}})_{\alpha}(T) = (\mathfrak{g}_{\mathbf{C}})_{\delta(\alpha)}(\mathfrak{t}_{\mathbf{C}}) \tag{11}
$$

对于所有 $\alpha \in R$，则每个$\mathfrak{g}^{\alpha}$ 的维数 1 超过 $\mathbf{C}($loc。引用，Th。 1) 和

$$
\mathfrak{g}_{\mathbf{C}}=\mathfrak{t}_{\mathbf{C}}\oplus \bigoplus_{\alpha\in R}\mathfrak{g}^{\alpha} \tag{12}
$$

对于每个$\alpha \in R$，用$V(\alpha )$表示$\mathfrak{g}$的二维子空间，使得$V(\alpha )_{(\mathbf{C})}=\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$； T 的伴随表示的$\mathfrak{g}$ 的非零同型分量是$\mathfrak{t}$ 和$V(\alpha )$。此外，令 K 为与 $\mathfrak{g}$ 的杀戮形式相关的二次方形式；它是负数（§1, no. 3，命题1）并且它的限制$K(\alpha )$到$V(\alpha )$是负数并且是分离的。对于 T 的每个元素 $t$，Ad $t$ 使 $K(\alpha )$ 保持稳定，因此给出态射或李群

$$
\iota_{\alpha}: T\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))
$$

存在唯一的同构$\rho_{\alpha}:\mathbf{U}\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))$使得$\iota_{\alpha}=\rho_{\alpha}\circ \alpha$。事实上，让$X$是$\mathfrak{g}^{\alpha}$的非零元素，并且在$\mathfrak{g}_{\mathbf{C}}$相对于$\mathfrak{g}$的共轭下，让$Y$是$X$的像；然后$Y\in \mathfrak{g}^{-\alpha}$，我们通过放入$U=X+Y, V=i(X-Y)$得到$V(\alpha )$的基$(U, V)$；由Ad $t,t\in T$诱发的$V(\alpha )$自同态矩阵，相对于基$(U, V)$为

$$
(\mathscr{R}(t^{\alpha})-\mathscr{I}(t^{\alpha}))
$$

$$
\mathscr{I}(t^{\alpha})\mathscr{R}(t^{\alpha})
$$

因此断言。

#### 命题 8 {#lie-ix-s4-prop-8 .statement tag=01C0}

令 Q(R) 为由 G 的根生成的 X(T) 的子群。

a) G 的中心 C(G) 是 T 的闭子群，等于根的核的交。规范映射 $X(T/C(G))\rightarrow X(T)$ 与像 Q(R) 是单射的。

b) 紧致群 C(G) 同构于离散群 $X(T)/Q(R) ($谱理论，第 1 章。 II, §1, no. 1，防御。 2）。

c) C(G) 约化到单位元素当且仅当 Q(R) 等于 X(T)。

§2, no. 2，科。 2 Th。 2、C(G)包含在T中。由于这是伴随表示的核，所以它是根的核交，在其他字子群Q(R)的正交补X(T)。因此，命题来自光谱理论，第 1 章。 II, §1, no. 7，周四。 4 和 no. 5，Th。 2.

#### 命题 9 {#lie-ix-s4-prop-9 .statement tag=01C1}

李群 G 的每个自同构，诱导 T 上的恒等式为形式 Int $t$，其中$t\in T$。

首先假设C(G)约化到单位元素，在其他字中X(T) = Q(R)（命题8）。设$f$为G的自同构在T上的恒等式，以及$\varphi = L(f)_{(\mathbf{C})}$；那么$\varphi$是$\mathfrak{g}_{\mathbf{C}}$的自同构，归纳出$\mathfrak{t}_{\mathbf{C}}$上的恒等式。由章。 VIII, §5, no. 2，命题2，存在唯一同态$\theta : Q(R)\rightarrow \mathbf{C}^*$，使得每个$\mathfrak{g}^{\alpha}$位似上都有$\varphi$诱导，比率为$\theta (\alpha )$。由于$\varphi$使$\mathfrak{g}_{\mathbf{C}}$的实形式$\mathfrak{g}$保持稳定，因此它与$\mathfrak{g}_{\mathbf{C}}$的共轭$\sigma$相对于$\mathfrak{g}$交换；但是 $\sigma (\mathfrak{g}^{\alpha}) =\mathfrak{g}^{-\alpha}$，所以 $\theta (-\alpha ) =\overline{\theta(\alpha)}$ 对于所有 $\alpha \in R$。这意味着$\theta (\alpha )\theta (\alpha ) =\theta (\alpha )\theta (-\alpha ) = 1$。由此可见，$\theta$在$\mathbf{U}$中取值，因此对应通过对偶性与T的元素$t$，使得(Ad$t$)$_{(\mathbf{C})}=\varphi$，因此Int$t=f$。

一般情况下，上述适用于群$G/C(G)$，其中心约化至单位元素，及其最大值环面$T/C(G)$。由此可见，如果 $f$ 是 G 的自同构推导出 T 上的恒等式，则存在 T 的元素 $t$，使得 $f$ 和 Int $t$ 诱导通过与 $G/C(G)$ 的商相同的自同构进行传递。但是，由于规范的态射 $D(G)\rightarrow G/C(G)$ 是有限覆盖（§1, no. 4，第 4 号命题的 Cor. 1），$f$ 和 Int $t$ 诱导与 D(G) 相同的自同构，因此与 $D(G)\times C(G)$ 相同，因此也与 G 相同（loc.1）。引用。）。

#### 推论{#lie-ix-s4-n4-cor-1 .statement tag=01C2}

设$u$为G的自同构，H为$u$的固定点的G由……组成的闭子群。那么，自同构$u$是内部当且仅当$H_0$是最大的秩。

如果 $u$ 等于 Int $g$，且 $g\in G$，则子群 $H_0= Z(g)_0$ 的最大值为秩（§2, no. 2，Cor. 3）。相反，如果 H 包含最大环面 S，则自同构 $u$ 为形式 Int $s$ 和 $s\in S$（命题 9）。

### 5. 节点向量和逆根

#### 引理 2 {#lie-ix-s4-lem-2 .statement tag=01C3}

设 S 是 T 的闭子群，Z(S) 是 G 中的归一化器。

(i) $R(Z(S)_0,T)$ 是$\alpha \in R(G,T)$ 的集合，使得$\alpha (S) =\{1\}$。

(ii) $Z(S)_0$ 的中心是$\alpha \in R(Z(S)_0,T)$ 的 Ker$\alpha$ 的交。

(iii) 如果 S 连通，则 Z(S) 连通。

李代数 $L(Z(S))_{(\mathbf{C})}$ 由 S 在 $\mathfrak{g}_{\mathbf{C}}$ 上的不变量组成（第 III, §9, no. 3 章，第 8 条），因此是 $\mathfrak{t}_{\mathbf{C}}$ 的直和和$\mathfrak{g}^{\alpha}$，$\alpha (S) =\{1\}$，因此 (i)。 断言 (ii) 由第 8 条命题 (no. 4) 得出，断言 (iii) 已被证明（§2, no. 2，第 2 条的 Cor. 5）。

#### 定理 1 {#lie-ix-s4-thm-1 .statement tag=01C4}

让$\alpha \in R(G,T)$。 $\alpha$的核的扶正器$Z_{\alpha}$是G的连通闭子群；它的中心是Ker$\alpha$；它的导出群$D(Z_{\alpha}) = S_{\alpha}$是秩1的G的连通闭半单子群。我们有$R(Z_{\alpha},T) =\{\alpha ,-\alpha \}$和暗淡$Z_{\alpha}=$暗淡T + 2。

令 $Z'_{\alpha}$ 为 (Ker $\alpha$ )$_0$ 的中心化子。到引理 2，这是 G 的连通闭子群，$R(Z'_{\alpha},T)$ 是 $\beta \in R(G,T)$ 的集合，使得 $\beta$((Ker$\alpha$ )$_0$) $=\{1\}$。显然，$\{\alpha ,-\alpha \} \subset R(Z'_{\alpha},T)$。反之，设 $\beta \in R(Z'_{\alpha},T)$；由于 (Ker $\alpha$ )$_0$ 在 Ker $\alpha$ 中具有有限指标，因此存在整数 $r\not= 0$，使得 $t^{r\beta}= 1$ 对于 $t\in$ Ker $\alpha$。从序列的精确度来看

$0\longrightarrow \mathbf{Z}\longrightarrow X(T)\longrightarrow$X(克$\alpha$)$\longrightarrow 0$

相应的由对偶性变为正合序列

0 $\longrightarrow$ Ker$\alpha \longrightarrow$ T $\longrightarrow^{\alpha}\mathbf{U}\longrightarrow 0$,

由此可见，$r\beta$ 是 $\alpha$ 的倍数；由章。 VIII, §2, no. 2，周四。 2 (i)，这意味着 $\beta \in  \{\alpha ,-\alpha \}$。因此，$R(Z'_{\alpha},T) =\{\alpha ,-\alpha \}$。由此可见 (引理 2) $Z'_{\alpha}$ 的中心是 Ker$\alpha$，因此$Z'_{\alpha}= Z_{\alpha}$。最后，由 Cor.第 4 条命题 1 (§1, no. 4)，$D(Z_\alpha)$ 是 $G$ 的连通闭半单子群；它是秩$1$，因为$\mathscr{L}(Z_\alpha)(\mathbf C)=\mathfrak{g}^\alpha+\mathfrak{g}^{-\alpha}+[\mathfrak{g}^\alpha,\mathfrak{g}^{-\alpha}]$。

#### 推论{#lie-ix-s4-n5-cor-1 .statement tag=01C7}

— *存在态射或李群* $\nu:\mathbf{SU}(2,\mathbf C)\to G$ *具有以下属性：*

a) *像共* $\nu$ *通勤需核共* $\alpha$。

b) *对于所有人* $a\in\mathbf U$，*我们有*
$$
\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\in\mathbf T
\quad\text{and}\quad
\alpha\circ\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}=a^2.
$$

*如果* $\nu_1$ *和* $\nu_2$ *是两个态射，从* $\mathbf{SU}(2,\mathbf C)$ *到* $G$ *具有前述属性，则存在* $a\in\mathbf U$ *这样*
$$
\nu_2=\nu_1\circ\operatorname{Int}
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}.
$$

由 Th. 1和§3, no. 6的命题6，李群存在态射
$$
\nu:\mathbf{SU}(2,\mathbf C)\to S_\alpha
$$
这是具有离散核的满射。那么$\nu^{-1}(\mathbf T\cap S_\alpha)$是$\mathbf{SU}(2,\mathbf C)$的最大环面（§2, no. 3，命题1）。由于$\mathbf{SU}(2,\mathbf C)$的最大环面为共轭（§2, no. 2，Th.2），如果需要，我们可以假设替换$\nu$乘$\nu\circ\operatorname{Int}s$（与$s\in\mathbf{SU}(2,\mathbf C)$），$\nu^{-1}(\mathbf T\cap S_\alpha)$是对角线的群矩阵 $\mathbf{SU}(2,\mathbf C)$。然后
$$
\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\in\mathbf T
$$
对于所有 $a\in\mathbf U$ 和映射
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
\longmapsto
\alpha\circ\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
$$
是 $\mathbf{SU}(2,\mathbf C)$ 的根，因此等于两个映射之一
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\longmapsto a^2
$$
或
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\longmapsto a^{-2}
$$
（§3, no. 6，公式（19））。在第一种情况下，同态$\nu$具有所需的属性；在第二种情况下，同态$\nu\circ\operatorname{Int}\theta$有它们（loc.cit.，公式（18））。

如果$\nu_1$和$\nu_2$是两个态射，从$\mathbf{SU}(2,\mathbf C)$到$G$满足指定的条件，它们都映射$\mathbf{SU}(2,\mathbf C)$到$S_\alpha$（条件a）），因此是$S_\alpha$ 的两种通用覆盖物。因此，存在$\mathbf{SU}(2,\mathbf C)$的自同构$\varphi$使得$\nu_2=\nu_1\circ\varphi$，并且我们通过使用no. 4的第9条命题结论。

根据前面的推论，同态$\nu_{\mathbf T}$从$\mathbf U$到$\mathbf T$，定义为
$$
\nu_{\mathbf T}(a)=\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
$$
对于$a\in\mathbf U$，独立于$\nu$的选择。用$\Gamma(\mathbf U)=2\pi i\mathbf Z$元素$2\pi i$$\Gamma(\nu_{\mathbf T})$下的$K_\alpha\in\Gamma(\mathbf T)$像表示；它被称为与根* $\alpha$ 伴随的 *节点向量。我们有$\langle\alpha,K_\alpha\rangle=2$，其他字（no. 2，公式（2））$\delta(\alpha)(K_\alpha)=4\pi i$；从$\mathfrak t$和$\mathscr L(S_\alpha)(\mathbf C)$的$K_\alpha$属于到交，我们有
$$
K_\alpha=2\pi iH_{\delta(\alpha)},
\tag{13}
$$
其中 $H_{\delta(\alpha)}$ 是与 $(\mathfrak g_{\mathbf C},\mathfrak t_{\mathbf C})$ 的根* $\delta(\alpha)$ 相关的*逆根（第 VIII, §2, no. 2 章）。在其他字中，当$\Gamma(\mathbf T)\otimes\mathbf R$通过配对与$X(T)\otimes \mathbf{R}$对偶识别时，$\langle ,\rangle ,K_{\alpha}$与逆根$\alpha^{\vee}\in (X(T)\otimes \mathbf{R})^*$识别。

#### 注 {#lie-ix-s4-n5-rem-1 .statement tag=01C5}

对于所有$x\in \mathbf{R}$，我们有

$($exp(2$\pi ix$) 0 $)_{2\pi ix}$

$\nu$ 0 经验值($-2\pi ix$)$=\nu_T(e$) = 经验值($xK_{\alpha}$)。 (14)

特别是：

$\nu (-0$1 $-01)=\nu_T(-1) =$ $(\frac{1}{2}K_{\alpha})$。 (15)

由此可见，$\nu$是单射的当且仅当$K_{\alpha}\notin2\Gamma$(T)，在其他字中，如果存在$\lambda \in X(T)$使得$\langle \lambda , K_{\alpha}\rangle \notin2\mathbf{Z}$。当$\mathfrak{g}_{\mathbf{C}}$很简单时，$\nu$是单射除非，$\mathfrak{g}_{\mathbf{C}}$是型$B_n, C(G) =\{1\}$，$\alpha$是短根（cf.第VI，板）。

在本段的其余部分中，我们用节点向量$K_{\alpha}$中的$R^{\vee}(G,T)$集合来表示$\alpha \in R(G,T)$。这是$\Gamma (T)$典范嵌入到$\mathfrak{t}_{\mathbf{C}}$与位似与$\delta (R)$的倒数根系$R^{\vee}(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}) =\{H_{\delta(\alpha)}\}$的比率$2\pi i$等同的$\Gamma (T)$子集。由此可见，$R^{\vee}(G,T)$生成是$\mathbf{R}$向量空间$L(T\cap D(G))$，因此X(T)中的正交补是$X(T/(T\cap D(G)))$。

用李群 T 自同构 Aut(T) 群表示； Weyl 群 $W = W_G(T) ($§2, no. 5) 可以用 Aut(T) 的子群来识别。另一方面，回想一下（第VIII, §2, no. 2，注 4），分裂的还原代数$(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$的Weyl群$W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$在$\mathfrak{t}_{\mathbf{C}}$上运行，因此规范地与子群相同$\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$。

#### 命题 10 {#lie-ix-s4-prop-10 .statement tag=01C6}

映射 $u \rightarrow L(u)_{(\mathbf{C})}$ 从 Aut(T) 到 $\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$ 诱导同构从 W 到分裂约化李代数 $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ 的 Weyl 群。对于所有$\alpha \in R$，$W_{Z_{\alpha}}(T)$是阶2，$W_{Z_{\alpha}}(T)$的非恒等元素前面的同构下的像是反射$s_{H_{\delta(\alpha)}}$。

所考虑的映射是单射的。还需要证明它的像等于$W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$。

让$g\in N_G(T)$。第 1 章中有记号。 VIII, §5, no. 2，我们有 Ad $g\in$ Aut($\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}$)$\cap$ Int($\mathfrak{g}_{\mathbf{C}}$)，所以 Ad $g\in$ Aut$_0(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}) ($loc。前述，no. 5，提案 11）。按地点。前述，no. 2，第 4 号提案，由广告 $g$ 属于至 $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ 诱导的 $\mathfrak{t}_{\mathbf{C}}$ 自同构。因此，$\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$中的W的像包含在$W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$中。

令$\alpha \in R(G,T)$，并令$\nu :\mathbf{S}\mathbf{U}(2,\mathbf{C})\rightarrow G$为具有Cor中属性的李群的态射。的 Th。 1. The image under $\nu$ of the element $\theta$ of $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ has the following properties (§3, no. 6, formulas (17)):

a）（Int$\nu (\theta )$）$(t) =t$如果$t\in$Ker$\alpha$，

b) (Int$\nu (\theta )$)$(t) =t^{-1}$如果$t\in T\cap S_{\alpha}$。

由此可见，Ad $\nu (\theta )$ 诱导是 Ker $\delta (\alpha )\subset \mathfrak{t}_{\mathbf{C}}$ 上的身份，诱导映射 $x \rightarrow  -x$ 是 $[\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]$ 上的身份，因此重合具有反射 $s_{H_{\delta(\alpha)}}$。因此，W 包含中的像全部为 $s_{H_{\delta(\alpha)}}$，因此等于 $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$。特别是 $W_{Z_{\alpha}}(T)$ 的值为阶 2，因此由恒等式和 Int $\nu (\theta )$ 组成。这样就完成了命题的证明。

#### 推论{#lie-ix-s4-n5-cor-2 .statement tag=01JJ}

假设G是半单。那么G的每个元素都是G的两个元素的换位子。

令 $c$ 为 Weyl 群 $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$（第 V, §6, no. 1 章）的 Coxeter 变换，并令 $n$ 为 $N_G(T)$ 的元素，其 W 中的类通过同构与 $c$ 标识，定义于命题。从T到T用$f_c$态射$t \rightarrow (n, t)$表示；对于$x\in \mathfrak{t}_{\mathbf{C}}$，我们有$L(f_c)_{(\mathbf{C})}(x) =$（广告$n$）$(x)-x=$$c(x)-x$。

由 Th.第 1 章$\mathfrak{t}_{\mathbf{C}}$的V, §6, no. 2、自同态$c$没有特征值等于1。因而，$L(f_c)$是满射，$f_c$也是满射。由此可见，T 的每个元素都是 G 的两个元素的换位子，这暗示了针对 Th 的推论。 2、§2, no. 2。

### 6. 基础群

在下面的命题中，$f(G,T)$表示从$\Gamma (T)$到$\pi_1(G)$的同态，它是$\Gamma (T)$到$\pi_1(T)$的典范同构（no. 2，注3）和同态的合成$\pi_1(\iota )$，其中 $\iota$ 是典范嵌入 $T\rightarrow G$。

#### 命题 11 {#lie-ix-s4-prop-11 .statement tag=01C8}

同态 $f(G,T) :\Gamma (T)\rightarrow \pi_1(G)$ 是满射。它的核是由节点向量$(K_{\alpha})_{\alpha\in R(G,T)}$家族产生的$\Gamma (T)$中的子群$N(G,T)$。

同态 $f(G,T)$ 根据命题 3 (§2, no. 4) 是满射。我们用$A(G,T)$断言表示：“$f(G,T)$的核是由$K_{\alpha}$生成的”，这还有待证明，并区分几种情况：

$a) G$ 是单连通的。令 $\rho :\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ 为有限维复数向量空间 V 上 $\mathfrak{g}_{\mathbf{C}}$ 的线性表示。限制在$\mathfrak{g}$，我们在真实的向量空间$V_{(\mathbf{R})}$上得到$\mathfrak{g}$的表示；由于 G 是单连通的，因此存在 G 在 $V_{(\mathbf{R})}$ 上的解析线性表示 $\pi$，使得 $\rho = L(\pi )$。根据no. 3的第7条命题，$\mathfrak{t}^*_{\mathbf{C}}$包含中X(T)的像$\delta (X(T))$在V上$\rho$的所有权。对于 $\mathfrak{g}_{\mathbf{C}}$ 的每一个表示 $\rho$ 都是如此，这是从第 1 章得出的结论。 VIII, §7, no. 2，周四。 1 $\delta$(R)的权的$\delta (X(T))$包含群，由$\lambda \in \mathfrak{t}^*_{\mathbf{C}}$的定义集合使得$\lambda (H_{\delta(\alpha)})\in \mathbf{Z}$对于所有$\alpha \in R$，在其他情况下字，$\lambda (K_{\alpha})\in 2\pi i\mathbf{Z}$ 适合所有 $\alpha \in R$。因而，$X(T)\otimes \mathbf{Q}$的群X(T)包含所有元素$\lambda$使得$\langle \lambda , K_{\alpha}\rangle  \in \mathbf{Z}$对于所有$\alpha \in R$，这通过对偶性意味着$\Gamma (T)$是由$K_{\alpha}$生成的，因此断言$A(G,T)$。

$b) G$ 是单连群 $G'$ 和环面 S 的直接乘积。则 T 是 $G'$ 的最大环面 $T'$ 与 $S,\Gamma (T)$ 的直接乘积可以识别为$\Gamma (T')\times \Gamma$(S)、$\pi_1(G)$ 与 $\pi_1(G')\times \pi_1$(S) 以及 $f(G,T)$ 与同态以及组件 $f(G',T')$ 和 $f(S,S)$。由于 $f(S,S)$ 是双射的，因此规范的映射 $\Gamma (T')\rightarrow \Gamma (T)$ 映射 Ker $f(G',T')$ 双射到 Ker $f(G,T)$。而且，G的导出群$G'$的$K_{\alpha}$属于到李代数，因此到$\Gamma (T')$的像，所以$A(G',T')$蕴含$A(G,T)$是直接的，因此断言$A(G,T)$，鉴于a)。

c) 一般情况。存在有限核的满射态射 $p: G'\rightarrow G$，其中 $G'$ 是由环面简单连接的群的直接乘积（§1, no. 4，命题 4）。如果$T'$是$G'$中T的逆像（这是§2, no. 3乘以$G'$的最大环面，命题1），并且$p$的N核，我们有正合序列$0\rightarrow N\rightarrow G'\rightarrow G\rightarrow 0$和 $0\rightarrow N\rightarrow T'\rightarrow T\rightarrow 0$，因此是具有精确行的交换式图表（no. 2、注 1 和一般拓扑，第 XI 章，正在准备中）

0 $\longrightarrow \Gamma (T')\longrightarrow \Gamma (T)\longrightarrow$ N $\longrightarrow$ 0

$f(G',T')f(G,T)$ ID$_N$

0 $\longrightarrow \pi_1(G')\longrightarrow \pi_1(G)\longrightarrow$ N $\longrightarrow 0$。

直接从蛇图表（代数，第X，p. 4，命题2）得出$A(G',T')$意味着$A(G,T)$，因此鉴于b），命题。

#### 推论 1 {#lie-ix-s4-prop-11-cor-1 .statement tag=01C9}

G 是单连通的当且仅当族 $(K_{\alpha})_{\alpha\in R(G,T)}$ 生成 $\Gamma (T)$。

#### 推论 2 {#lie-ix-s4-prop-11-cor-2 .statement tag=01CA}

令 H 为 G 包含 T 的连通闭子群；有正合序列

$$
0\longrightarrow N(H,T)\longrightarrow N(G,T)\longrightarrow \pi_1(H)\longrightarrow \pi_1(G)\longrightarrow 0
$$

这是从代数，第 1 章得出的。 X，p. 4，命题 2（蛇图表），应用于交换律图表

0 $\longrightarrow N(H,T)\longrightarrow \Gamma (T)\longrightarrow \pi_1(H)\longrightarrow$ 0

0 $\longrightarrow N(G,T)\longrightarrow \Gamma (T)\longrightarrow \pi_1(G)\longrightarrow 0$。

#### 注 {#lie-ix-s4-n6-rem-1 .statement tag=01CB}

可以证明（cf.习题 2 of §5）$\pi_2(G/H)$是零。前面的序列的精确性则给出从$\pi_2(G/H)$到$N(G,T)/N(H,T)$的同构。

#### 推论 3 {#lie-ix-s4-prop-11-cor-3 .statement tag=01CC}

同态$\pi_1(D(G))\rightarrow \pi_1(G)$相应的将D(G)纳入G诱导同构，从$\pi_1(D(G))$到挠元子群$\pi_1(G)$。

事实上，$T\cap D(G)$是D(G)的最大环面（§2, no. 3，命题$1c$）$)$；来自正合序列

$$
0\longrightarrow \Gamma (T\cap D(G))\longrightarrow \Gamma (T)\longrightarrow \Gamma (T/(T\cap D(G)))\longrightarrow 0
$$

和命题 11，我们得到正合序列

$$
0\longrightarrow \pi_1(D(G))\longrightarrow \pi_1(G)\longrightarrow \Gamma (T/(T\cap D(G)))\longrightarrow 0
$$

因此推论，因为$\pi_1(D(G))$是有限的而$\Gamma (T/(T\cap D(G)))$是自由的。

### 7. 最大子群秩

回想一下（第 VI, §1, no. 7 章），如果$(P + P)\cap R\subset P$，子集 P 的$R = R(G,T)$ 被认为是封闭的，如果$P =-P$ 则被称为对称。

#### 命题 12 {#lie-ix-s4-prop-12 .statement tag=01CD}

令 $\mathscr{H}$ 为 G 包含于 T 的连通闭合子群的集合，按包含排序。 映射$H \rightarrow R(H,T)$是$R(G,T)$的对称闭子集的从$\mathscr{H}$到集合的递增双射，按包含排序。

如果$H\in \mathscr{H}$，则$L(H)_{(\mathbf{C})}$是$\mathfrak{t}_{\mathbf{C}}$的直和，$\mathfrak{g}^{\alpha}$是$\alpha \in R(H,T)$；因为这是$\mathfrak{g}_{\mathbf{C}}$中的约子代数，所以R的子集$R(H,T)$满足规定的条件（第VIII, §3, no. 1、引理2和命题2）。相反，如果 P 是 R 满足这些条件的子集，则 $\mathfrak{t}_{\mathbf{C}}\oplus \sum_{\alpha\in P}\mathfrak{g}^{\alpha}$ 是子代数

$\mathfrak{g}_{\mathbf{C}}($loc。引），它在$\mathbf{R}$（no. 3）上是有理数，因此是形式$\mathfrak{h}_{(\mathbf{C})}$，其中$\mathfrak{h}$是$\mathfrak{g}$的子代数。令H(P)为由$\mathfrak{h}$定义的G的积分子群；它已关闭（§2, no. 4，注1）。我们立即验证映射$H \rightarrow R(H,T)$和$P \rightarrow H(P)$是递增并且互为倒数。

#### 推论 1 {#lie-ix-s4-prop-12-cor-1 .statement tag=01CE}

G 包含于 T 仅有有限多闭子群。

令H为子群；那么$H_0\in \mathscr{H}$，$\mathscr{H}$是有限的。此外，H 是 $N_G(H_0)$ 包含于 $H_0$ 的子群，$N_G(H_0)/H_0$ 是有限的（§2, no. 4，命题 4 和注 2）。

#### 推论 2 {#lie-ix-s4-prop-12-cor-2 .statement tag=01CF}

设H为G 包含于 T的连通闭子群，并令$W^H_G(T)$为R的子集$R(H,T)$的$W_G(T)$中的稳定子。群$N_G(H)/H$同构于商群$W^H_G(T)/W_H(T)$。

事实上，根据应用于$N_G$(H)的§2, no. 5的第7条命题，$N_G(H)/H$同构于$W_{N(H)}(T)/W_H$(T)，其中$W_{N(H)}(T)$是$W_G(T)$的元素的集合，其代表在$N_G(T)$标准化H。令$n\in N_G$(T)，并令$w$为其$W_G(T)$中的类。由章。 III, §9, no. 4，命题 11，$n$ 标准化 H 当且仅当 (Ad $n$)$(L(H)) = L(H)$；鉴于no. 3的命题5，这也意味着R的子集$R(H,T)$在$w$下是稳定的，由此得出推论。

#### 注 1 {#lie-ix-s4-n7-rem-1 .statement tag=01CG}

群 $W^H_G(T)$ 也是 T 的子群 C(H) 的 $W_G(T)$ 中的稳定子：这源自no. 4 的第 8 条命题。

#### 命题 13 {#lie-ix-s4-prop-13 .statement tag=01CH}

令 H 为最大秩的 G 的连通闭子群，且C其中心。那么G的C包含中心，H是C的中心化器的恒等分量。

令S为H的最大环面。由于G的中心包含在S中，因此它包含在C中。把$L = Z(C)_0$；这是 G 包含于 H 的连通闭子群，因此最大秩，并且其中心等于C。分别用相对于S的H和L的$R_H$和$R_L$根系表示；然后$R_H\subset R_L\subset R(G,S)$。由于 C(H) = C(L)，第 8 条命题 (no. 4) 意味着等式 $Q(R_H) = Q(R_L)$；但是 $Q(R_H)\cap R_L= R_H$（第 VI, §1, no. 7 章，第 23 条命题），所以 $R_H= R_L$ 且 H = L（第 12 条命题）。

#### 注 2 {#lie-ix-s4-n7-rem-2 .statement tag=01CI}

如果存在 G 的最大环面 S 和 $R(G,S)$ 的子集 P，使得 $C =\bigcap_{\alpha\in P}$ Ker$\alpha$，则称 G 的子群 C 是激进的。根据第 13 条命题和 no. 5 的引理 2，映射 $H \rightarrow C(H)$ 诱导双射从最大秩的已连接闭合子群的集合到G. 逆双射的部首子群的集合是映射$C \rightarrow Z(C)_0$。

#### 推论 {#lie-ix-s4-n7-cor-1 .statement tag=01CJ}

$g\in G$的集合使得$T\cap gTg^{-1}\not= C(G)$是不同于G的G的有限闭解析子流形数的并。

确实，输入$A_g= T\cap gTg^{-1}$；我们有$T\subset Z(A_g)$和$gTg^{-1}\subset Z(A_g)$。因而，存在$x\in Z(A_g)$使得$xTx^{-1}=gTg^{-1}($§2, no. 2，Th。 2），这意味着$g\in Z(A_g).N_G(T)$。用 $\mathscr{A}$ 表示 G 包含 T 的闭子群且不同于 G 的有限（Cor.1）集合，并设 X = $\bigcup_{H\in\mathscr{A}}H.N_G(T)$；这是 G 的闭子流形的有限并，与 G 不同。如果 $A_g\not= C(G)$，则$Z(A_g)\in \mathscr{A}$，以及 $g$ 属于到 X。相反，如果$g\in H.N_G$(T)，与$H\in \mathscr{A}$，则$A_g$包含C(H)，所以$A_g\not= C(G)$（命题13）。

#### 命题 14 {#lie-ix-s4-prop-14 .statement tag=01CK}

令X为T的子集，并令$R_X$为根$\alpha \in R(G,T)$的集合，使得$\alpha (X) =\{1\}$。 群$Z_G(X)/Z_G(X)_0$同构于子群与$W_G(T)$的商，固定X除以由$s_{\alpha}$对$\alpha \in R_X$的反射产生的子群。

把$H = Z_G(X)$；由于$L(H)_{(\mathbf{C})}$是由Ad(X)固定的$\mathfrak{g}_{\mathbf{C}}$的点集合，所以$\mathfrak{t}_{\mathbf{C}}$的和和$\alpha (X) =\{1\}$的$\mathfrak{g}^{\alpha}$。因而，$R(H_0,T) =$$R_X$，因而$W_{H_0}(T)$是由$\alpha \in R_X$的反射$s_{\alpha}$生成的。现在应用§2, no. 5第7号提案就足够了。

我们将在下面看到（§5, no. 3，Th.1），如果G是单连通的并且X约化到点，则扶正器Z（X）是连通的。

### 8.根图表

#### 定义 2 {#lie-ix-s4-def-2 .statement tag=01CL}

根图表（或简称为图表，如果没有混淆的风险）是三元组 $D = (M,M_0,R)$，其中：

(RD$_0$)$M$是有限型的自由$\mathbf{Z}$模，子模$M_0$是M的直因子；

(RD$_I$)$R$是$M; R\cup M_0$生成的有限子集$\mathbf{Q}$向量空间$\mathbf{Q}\otimes M$；

(RD$_{II}$)对于所有$\alpha \in R$，存在$M^*=$Hom$_{\mathbf{Z}}(M,\mathbf{Z})$的元素$\alpha^{\vee}$，使得M的$\alpha^{\vee}(M_0) = 0,\alpha^{\vee}(\alpha ) = 2$和自同态$x \rightarrow x-\alpha^{\vee}(x)\alpha$使R保持稳定。

由章。 VI, §1, no. 1，对于$M^*$的所有$\alpha \in R$元素$\alpha^{\vee}$由$\alpha$唯一确定；我们用 M 的 $s_{\alpha}$ 自同态 $x \rightarrow x-\alpha^{\vee}(x)\alpha$ 表示。此外（前述），$\mathbf{Q}$向量空间$\mathbf{Q}\otimes M$是$\mathbf{Q}\otimes M_0$和向量子空间的直和 V(R) 由 R 生成，R 是 V(R) 中的根系（参见上文，定义 1）。

R 的元素称为根图表 D 的根，以及$M^*$ 的逆根的元素 $\alpha^{\vee}$。 The group generated by the automorphisms $s_{\alpha}$ of M is called the Weyl group of D and is denoted by W(D); the elements of W(D) induce the identity on $M_0$, and induce on V(R) the transformations of the Weyl group of the root system R.

#### 例 1 {#lie-ix-s4-n8-exa-1 .statement tag=01CM}

对于有限型 M 的每个自由 $\mathbf{Z}$ 模，三元组 $(M,M,\emptyset )$ 是根图表。

#### 例 2 {#lie-ix-s4-n8-exa-2 .statement tag=01CN}

如果$D = (M,M_0,R)$是根图表，则令$M^*_0$为$M^*$中V(R)的正交补，令$R^{\vee}$为D的逆根的集合，则$D^{\vee}= (M^*,M^*_0,R^{\vee})$为根图表，称为 D 的逆。对于所有 $\alpha \in R$，$M^*$ 的对称性 $s_{\alpha^{\vee}}$ 是 M 对称性 $s_{\alpha}$ 的反对自同构；从 W(D) 到 $W(D^{\vee})$，映射 $w \rightarrow^tw^{-1}$ 为同构。此外，$V(R^{\vee})$可以自然地识别为$\mathbf{Q}$向量空间$V(R), R^{\vee}$的对偶，然后识别为R的逆根系。

如果$M^*$的对偶用M表示，则$D^{\vee}$的逆图表用D表示。

#### 例 3 {#lie-ix-s4-n8-exa-3 .statement tag=01CO}

令 $(\mathfrak{g},\mathfrak{h})$ 为分裂的约简 $\mathbf{Q}$-李代数，且 $M\subset \mathfrak{h}$ 为许用格（第 VIII, §12, no. 6 章，定义 1）。令$M_0$为与$(\mathfrak{g},\mathfrak{h})$的根和$H_{\alpha},\alpha \in R(\mathfrak{g},\mathfrak{h})$的$R^{\vee}$集合正交的M的子群。那么$(M,M_0,R^{\vee})$是根图表，$(M^*,M^*_0,R(\mathfrak{g},\mathfrak{h}))$是图表的逆。

#### 例 4 {#lie-ix-s4-n8-exa-4 .statement tag=01CP}

令V在$\mathbf{Q}$之上成为向量空间，并且在V中R根系；由 R 的权的 P(R) 群和 R 的基团权的 Q(R) 群表示（第 1 章） VI, §1, no. 9）。 那么$(Q(R),0,R)$和$(P(R),0,R)$就是根图表。 A root diagram $(M,M_0,S)$ is isomorphic to a diagram of the form $(Q(R),0,R)$ (resp. $(P(R),0,R)$) if and only if M is generated by S (resp. $M^*$ is generated by $S^{\vee}$).

对于 P(R) 包含 $Q(R), (X,0,R)$ 的每个子群 X 是根图表，并且直到同构，每个图表 $(M,M_0,S)$ 使得 $M_0= 0$，在其他字使得 S有限指标的M的生成子群，就是这样产生的。

如果根系 R 减少，则根图表 $(M,M_0,R)$ 被称为减少（在其他字（VI, §1, no. 4），如果关系 $\alpha , \beta \in R,\lambda \in \mathbf{Z}$、$\beta =\lambda \alpha$ 暗示$\lambda = 1$ 或$\lambda =-1$）。 例 1) 和 3) 中的图表减少。

### 9. 紧李群和根系

有了前面数中引入的术语，数4和5的结果中一个重要的部分可以总结为下面的定理：

#### 定理 2 {#lie-ix-s4-thm-2 .statement tag=01CQ}

a$) (X(T),X(T/(T\cap D(G)),R(G,T)))$ 是根图表的约化；它的 Weyl 群由 $X(w)$ 和 $w\in W$ 组成； 群 X(C(G)) 同构于X(T) 与$R(G,T)$ 生成的子群的商。

b$) (\Gamma (T), \Gamma (C(G)_0),R^{\vee}(G,T))$ 是根图表的简化；它的 Weyl 群由 $\Gamma (w)$ 组成，对于 $w\in W$； 群$\pi_1(G)$同构于$R^{\vee}(G,T)$生成的$\Gamma (T)$除以子群的商。

c) 如果$\mathbf{Z}$-模X(T) 和$\Gamma (T)$ 中的每一个都可以用另一个的对偶来标识（no. 2，命题3），那么前面的根图表中的每一个都可以用另一个的逆来标识。

用$D^*(G,T)$图表$(X(T),X(T/(T\cap D(G)),R(G,T)))$和$D_*(G,T)$图表$(\Gamma (T), \Gamma (C(G)_0),R^{\vee}(G,T))$表示；它们分别称为 G（相对于 T）的逆变图表和协变图表。

#### 例 1 {#lie-ix-s4-n9-exa-1 .statement tag=01CR}

如果 G 是秩 1 的半单，则 $D^*(G,T)$ 和 $D_*(G,T)$ 必然同构于两个图表 $\Delta_2= (\mathbf{Z},0,\{2,-2\})$、$\Delta_1= (\mathbf{Z},0,\{1,-1\})$ 之一。如果 G 同构于 $\mathbf{S}\mathbf{U}(2,\mathbf{C}), D_*(G,T)$ 则同构于 $\Delta_1$（因为 G 是单连通的），所以 $D^*(G,T)$ 同构于 $\Delta_2$。如果 G 同构于 $\mathbf{S}\mathbf{O}(3,\mathbf{R}), D^*(G,T)$ 则同构于 $\Delta_1$（因为 $C(G) =\{1\}$），所以 $D_*(G,T)$ 同构于 $\Delta_2$。

#### 例 2 {#lie-ix-s4-n9-exa-2 .statement tag=01CS}

如果G和$G'$是两个连通的紧李群，分别具有最大圆环T和$T'$，并且如果$D^*(G,T) = (M,M_0,R)$和$D^*(G',T') =$$(M',M'_0,R')$，则$D^*(G\times G',T\times T')$可以与$(M\oplus M',M_0\oplus$$M'_0,R\cup R')$识别。对于协变图表也是如此。

#### 例 3 {#lie-ix-s4-n9-exa-3 .statement tag=01CT}

设 N 为 T 的闭子群，以 G 为中心，$(M,M_0,R)$ 为 G 相对于 T 的逆变图表。则 $G/N$ 相对于 $T/N$ 的逆变图表可以用 $(M',M'_0,R)$ 来识别，其中 $M'$ 为$\lambda$的M由……组成的子群使得$\lambda (N) =\{1\}$和$M'_0= M'\cap M_0$。

#### 例 4 {#lie-ix-s4-n9-exa-4 .statement tag=01CU}

类似地，令 N 为有限阿贝尔的群和 $\varphi :\pi_1(G)\rightarrow N$ 满同态。设$G'$为与此同态相关的G的覆盖；这是一个连通的紧李群，其中N是一个中心子群（总论拓扑，XI章，正在准备中），G可以自然地与$G'/N$等同。令$T'$为$G'$的最大环面，即T的逆像。如果$(P,P_0,S)$是G相对于T的协变图表，则$G'$相对于$T'$的协变图表可以识别为$(P',P'_0,S)$，其中$P'$是复合同态$\varphi \circ f(G,T) : P\rightarrow N$的核（cf.no. 6，命题11），以及$P'_0= P_0\cap P'$。

#### 注 1 {#lie-ix-s4-n9-rem-1 .statement tag=01CV}

设$\mathfrak{c}$为$\mathfrak{g}_{\mathbf{C}}$中的中心；然后$\mathfrak{c}= L(C(G))_{(\mathbf{C})}$。我们在 G 相对于 T 的图表和分裂的还原代数 $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}):$ 的正向和逆向根系之间有以下关系

a) 典范同构从$\mathbf{C}\otimes \Gamma (T)$到$\mathfrak{t}_{\mathbf{C}}$，诱导双射从$\mathbf{C}\otimes \Gamma (C(G)_0)$到$\mathfrak{c}$以及双射从$1\otimes R^{\vee}(G,T)$到$2\pi i.R^{\vee}(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$。

b) 典范同构从$\mathbf{C}\otimes X(T)$到$\mathfrak{t}_{\mathbf{C}}$诱导的对偶$\mathfrak{t}^*_{\mathbf{C}}$，双射从$\mathbf{C}\otimes X(T/(T\cap D(G)))$到$\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}(\mathfrak{g})_{\mathbf{C}}$的正交补集，以及双射从$1\otimes R(G,T)$到$R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$。

#### 注 2 {#lie-ix-s4-n9-rem-2 .statement tag=01CW}

假设群G为半单；用 R (resp. $R^{\vee}$) 根系 $R(G,T)$ (resp. $R^{\vee}(G,T)$) 表示，这样我们就有了包含项

$$
Q(R)\subset X(T)\subset P(R)Q(R^{\vee})\subset \Gamma (T)\subset P(R^{\vee})
$$

有限的阿贝尔的群 $P(R)/Q(R)$ 和 $P(R^{\vee})/Q(R^{\vee})$ 具有对偶性（第 VI, §1, no. 9 章）；如果$\widehat{M}$表示有限阿贝尔的群M的对偶群，我们从前面的典范同构推出

$$
\Gamma (T)/Q(R^{\vee})\rightarrow \pi_1(G)P(R^{\vee})/\Gamma (T)\rightarrow C(G)
$$

$$
P(R)/X(T)\rightarrow (\pi_1(G)\widehat{)}X(T)/Q(R)\rightarrow (C(G))\widehat{.}
$$

特别地，$\pi_1(G)$和C(G)的阶的乘积等于$R(G,T) ($loc的连接指标$f$。引用。）。

现在让$G'$与另一个连接紧李群、$T'$，最大环面为$G'$。令 $f: G\rightarrow G'$ 为李群的同构，使得 $f(T) = T'$；用$f_T$同构从T到$T'$表示定义。那么$X(f_T)$是从$D^*(G',T')$到$D^*(G,T)$的同构，用$D^*(f)$表示，$\Gamma (f_T)$是从$D_*(G,T)$到$D_*(G',T')$的同构，用$D_*(f)$表示。如果$t\in T$，并且如果我们放入$g=f\circ$ Int $t=$ (Int $f(t)$)$\circ f$，则$D^*(g) = D^*(f), D_*(g) = D_*(f)$。

#### 命题 15 {#lie-ix-s4-prop-15 .statement tag=01CX}

令从$D^*(G',T')$到$D^*(G,T)$（或从$D_*(G,T)$到$D_*(G',T')$）的$\varphi$为同构。存在同构 $f: G\rightarrow G'$，使得 $f(T) = T'$ 和 $\varphi = D^*(f)$（分别为 $\varphi = D_*(f)$）；如果$f_1$和$f_2$是两个这样的同构，则存在T的元素$t$使得$f_2=f_1\circ$Int$t$。

第二个断言紧随第9条命题（no. 4）；我们证明了协变图表和例的第一个。 用$G'$（分别$T'$）的$\mathfrak{g}'$（分别$\mathfrak{t}'$）李代数表示，并用$\mathfrak{g}'_{\mathbf{C}}$（分别$\mathfrak{t}'_{\mathbf{C}}$）表示其复数李代数。 由章。 VIII, §4, no. 4, Th. 2 (i), there exists an isomorphism $\psi :\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}'_{\mathbf{C}}$ that maps $\mathfrak{t}_{\mathbf{C}}$ to $\mathfrak{t}'_{\mathbf{C}}$ and induces on $\Gamma (T)\subset \mathfrak{t}_{\mathbf{C}}$ the given isomorphism $\varphi :\Gamma (T)\rightarrow \Gamma (T')$. 那么$\mathfrak{g}$和$\psi^{-1}(\mathfrak{g}')$是$\mathfrak{g}_{\mathbf{C}}$中的两个紧形式，它们具有与$\mathfrak{t}_{\mathbf{C}}$相同的交$\mathfrak{t}$；根据§3, no. 2，命题3，存在$\mathfrak{g}_{\mathbf{C}}$的内自同构$\theta$，归纳$\mathfrak{t}_{\mathbf{C}}$上的恒等式，从而$\theta (\mathfrak{g}) =\psi^{-1}(\mathfrak{g}')$。 通过替换 $\psi$ $\psi \circ \theta$，我们可以假设 $\psi$ 映射 $\mathfrak{g}$ 到 $\mathfrak{g}'$。 此外，根据no. 2的命题4，存在唯一态射$f_T: T\rightarrow T'$使得$\Gamma (f_T) =\varphi$。 那么$\psi$到$\mathfrak{t}$的限制是$L(f_T)$，并且根据§2, no. 6，第8条命题，存在唯一态射$f: G\rightarrow G'$，即T上的诱导$f_T$和$\mathfrak{g}_{\mathbf{C}}$上的$\psi$。 应用是$\varphi^{-1}$和$\psi^{-1}$的前面，我们得到态射到$f$的逆，因此是同构。 然后$D_*(f) =\Gamma (f_T) =\varphi$，因此命题。

注，如果 T 和 $T'$ 是 G 的两个最大环面，图表 $D^*(G,T)$ 和 $D^*(G,T')$ 同构的（如果 $g\in G$ 使得 $gTg^{-1}= T'$，则 Int $g$ 是从 G 到 G 的同构， 映射 T 至 $T'$）。用$D^*(G,T)$的$D^*(G)$同构类表示（cf.集合论，第II, §6, no. 2章）；这就是只依赖于G的根图表，称为G的逆变图表。G的协变图表$D_*(G)$类似地定义，我们得到：

#### 推论{#lie-ix-s4-n9-cor-1 .statement tag=01CY}

两个相连的紧李群 G 和 $G'$ 同构当且仅当图表 $D^*(G)$ 和 $D^*(G')$（分别为 $D_*(G)$ 和 $D_*(G')$）相等。

#### 命题 16 {#lie-ix-s4-prop-16 .statement tag=01CZ}

对于每个约简的根图表 D，都存在一个连通的紧李群 G，使得 $D^*(G)$（分别为 $D_*(G)$）与 D 同构的。

a) 通过替换 D，如有必要，通过它的逆图表，我们可以简化为构造 G，使得 $D^*(G)$ 与 D 同构。 把$D = (M,M_0,R)$；那么$\mathbf{Q}\otimes M$就是R生成的$\mathbf{Q}\otimes M_0$和向量子空间V(R)的直和。 而且，由于M上的逆根取整数值，与$\mathbf{Q}\otimes M_0$平行的V(R)上M的投影包含在R的权P(R)的群中，所以M是有限指标的$M_0\oplus P(R)$的子群。 用$D'$图表$(M_0\oplus P(R),M_0,R)$表示。

b) 令$\mathfrak{a}$为复半单李代数，其规范根系同构于$R\subset \mathbf{C}\otimes V(R)$（第VIII, §4, no. 3章），并令$\mathfrak{g}_1$为$\mathfrak{a}($§3, no. 2的紧实数形式，Th。 1）。令$G_1$为单连通实李群，其李代数与$\mathfrak{g}_1$同构；那么 $G_1$ 是紧致的 (§1, no. 4, Th. 1)。令 $T_1$ 为 $G_1$ 的最大值环面。由 Th. 1、图表$D^*(G_1,T_1)$与$(P(R),0,R)$同构。

c) 令$T_0$为维数的环面等于$M_0$的秩；则 $D^*(T_0,T_0)$ 同构于 $(M_0,M_0,\emptyset )$，因而 $D^*(G_1\times T_0,T_1\times T_0)$ 同构于 $D'$ (例 2)。

d) 最后，令 N 为与 M 正交的 $T_1\times T_0$ 的有限子群。放入 $G = (G_1\times T_0)/N, T = (T_1\times T_0)/N$。那么G是连通的紧李群，T是G的最大环面，$D(G,T)$同构于D（例3）。

#### 学院{#lie-ix-s4-n9-sch-1 .statement tag=01D0}

因而，连接的紧李群直到同构的分类被减少为减少的根图表的分类。连接紧凑半单李群对应到约化根图表 $(M,M_0,R)$，使得 $M_0= 0$；给出这样的图表相当于在$\mathbf{Q}$和V的子群M中给出向量空间V中的约化根系R，使得$Q(R)\subset M\subset P(R)$。

#### 注 3 {#lie-ix-s4-n9-rem-3 .statement tag=01D1}

Let $T'$ be another maximal torus of G, B (resp. $B'$) a basis of the root system $R(G,T)$ (resp. $R(G',T')$) (Chap. VI, §1, no. 5，默认。 2）。 存在元素 $g\in G$，使得 Int $g$ 映射 T 到 $T'$，B 到$B'$，并且这些元素形式是唯一的陪集模 Int(T)（因为 T 和 $T'$ 是共轭，我们可以假设$T = T'$，应用第 1 章就足够了。 VI, §1, no. 5、注 4 和 no. 4 的第 9 条）。 由此可见，由 Int $g$ 引起的从 T 到$T'$ 的同构与$g$ 的选择无关；因而$D_*$(Int $g$)和$D^*$(Int $g$)也是如此。 释义章节。 VIII, §5, no. 3，注 2，经过必要的修改，我们现在可以得到定义 G 的规范极大值环面，$G,. .$ 的规范协变和逆变根图表..

### 10. 自同构连接的紧李群

用 G 的自同构的 Aut(G) 李群（第III, §10, no. 2）表示，并用 Aut(G$,T$) 表示元素 $u$ 的 Aut(G) 由……组成的闭子群，使得 $u(T) = T$。我们已经看到（§1, no. 4，命题 4 的 Cor.5），Aut(G) 的恒等分量是子群 Int(G) of 内自同构；用 G 的子群 H 的 Int(G) 中的 Int$_G(H)$ 像表示。

设 D 为 G 相对于 T 的协变图表；用 Aut(D) 群表示其自同构，用 W(D) 表示其 Weyl 群。从 Aut(G$,T$) 到 Aut(D) 映射 $u \rightarrow D_*(u)$ 为同态。 no. 9 的第 15 条命题立即给出：

#### 命题 17 {#lie-ix-s4-prop-17 .statement tag=01D2}

同态 Aut(G$,T$)$\rightarrow$ Aut(D) 是满射，具有核 Int$_G(T)$。

注 Aut(G$,T$)$\cap$ Int(G) = Int$_G(N_G(T))$ 并且 Aut(D) 中 Int$_G(N_G(T))$ 的像是 W(D)（no. 5，命题 10）。因而，命题 17 给出同构

自动（G$,T$）$/$（自动（G$,T$）$\cap$Int（G））$\rightarrow$自动（D）$/W(D)$。

此外，Aut(G) = Int(G).Aut(G$,T$)。事实上，如果 $u$ 属于到 Aut(G)，$u(T)$ 是 T 的最大环面，因此是共轭到 T，并且存在 G 的内自同构 $v$，使得 $u(T) =v$(T)，在其他字 $v^{-1}u\in$ 自动（G$,T$）。由此可见，Aut(G)$/$Int(G) 可以与 Aut(G$,T$)$/$(Aut(G$,T$)$\cap$Int(G)) 等价，因此根据前面的内容我们有正合序列

$1\rightarrow$ Int(G) $\rightarrow$ 自动(G) $\rightarrow$ 自动(D)$/W(D)\rightarrow 1$。 (16)

因而：

#### 命题 18 {#lie-ix-s4-prop-18 .statement tag=01K9}

群 Aut(G)$/$Int(G) 与 Aut(D)$/W(D)$ 同构。

特别地，假设G是半单；然后，群 Aut(D) 可以用 $A(R(G,T))$ 的子群（VI, §1, no. 1 章）由……组成或元素 $u$ 来识别，这样$u(X(T))\subset X(T)$ 和子群 W(D) 可以用$W(R(G,T))$。

#### 推论{#lie-ix-s4-n10-cor-1 .statement tag=01D3}

如果 G 是单连通的，或者如果 C(G) 约化到单位元素，则群 Aut(G)$/$Int(G) 同构于 $R(G,T)$ 的 Dynkin 图的自同构的群。

这是从前面的章节得出的。 VI, §4, no. 2，科。提案 1。

我们现在要证明扩张 (16) 承认截面。

对于所有$\alpha \in R(G,T)$，用$V(\alpha )$表示$\mathfrak{g}$的二维向量子空间，使得$V(\alpha )_{(\mathbf{C})}=\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$； K 表示与 $\mathfrak{g}$ 的杀戮形式相关的二次形式。

#### 定义 3 {#lie-ix-s4-def-3 .statement tag=01D4}

$(G,T)$ 的框架为对 $(B,(U_{\alpha})_{\alpha\in B})$，其中 B 为 $R(G,T)$ 的基（第 VI, §1, no. 5 章，定义 2），并且对于所有 $\alpha \in B,U_{\alpha}$ 为 $V(\alpha )$ 的元素，使得$K(U_{\alpha}) =-1$。

G 的成帧是 G 的最大环面 T 与$(G,T)$ 的成帧。

#### 引理 3 {#lie-ix-s4-lem-3 .statement tag=01D5}

令 $B_0$ 为 $R(G,T)$ 的基。 群Int$_G(T)$在形式$(B_0,(U_{\alpha})_{\alpha\in B_0})$的$(G,T)$帧的集合上进行简单传递操作。

对于所有 $\alpha \in B_0$，用形式 K 到 $V(\alpha )$ 的二次方的 $K(\alpha )$ 限制表示； T $V(\alpha )$ 定义态射 $\iota_{\alpha}: T\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))$ 的运算。我们在no. 4中看到，$\mathbf{S}\mathbf{O}(K(\alpha ))$可以与$\mathbf{U}$识别，就像$\iota_{\alpha}$可以与根$\alpha$识别一样。由于$B_0$是R的基，它是根生成的$\mathbf{Z}$模Q(R)的基，因此基是X(T)的子模$X(T/C(G))$。由此可见，态射$\iota_{\alpha}$诱导同构的乘积从$T/C(G)$到群$\mathbf{S}\mathbf{O}(K(\alpha ))$的乘积。但后者群在$(G,T)$的框架的集合上简单传递，其第一个组件是$B_0$。

#### 命题 19 {#lie-ix-s4-prop-19 .statement tag=01D6}

群 Int(G) 在 G 的框架集合上进行简单传递操作。

令$e= (T,B,(U_{\alpha}))$和$e'= (T',B',(U'_{\alpha}))$为G的两个框架。G中存在元素$g$使得(Int$g$)$(T) = T'$，并且这些元素形式为模$N_G(T)$的单个陪集。因此，我们可以假设$T = T'$，并且我们必须证明存在Int$_G(N_G(T))$的唯一元素，即变换$e$到$e'$。由章。 VI, §1, no. 5，注 4，W(R)存在唯一元素$w$使得$w(B) = B'$。由于W(R)可以用$N_G(T)/T$识别，因此存在$n\in N_G(T)$，使得$w=$ Int $n$，并且$n$唯一确定模T。因此，我们可以假设$B = B'$，并且我们必须证明存在唯一元素 Int$_G(T)$即变换$e$到$e'$，简单来说就是引理3。

#### 推论 {#lie-ix-s4-n10-cor-2 .statement tag=01D7}

令$e$为$(G,T)$的框架，并令E为G的自同构的群，使$e$保持稳定。那么Aut(G)就是E通过Int(G)半直接乘积，Aut(G$,T$)是E通过Int(G)$\cap$Aut(G$,T$)$=$Int$_G(N_G(T))$半直接乘积。

事实上，Aut(G) 变换 $e$ 的每个元素都成为 G 的一个框架。根据 Prop. 19，Aut(G) 模 Int(G) 的每个陪集在单个点中满足 E，因此第一个断言。第二个也用同样的方法证明。

#### 注 {#lie-ix-s4-n10-rem-1 .statement tag=01D8}

设G和$G'$为两个相连的紧李群，并令$e=$$(T,B,(U_{\alpha}))$和$e'= (T',B',(U'_{\alpha}))$分别为G和$G'$的框架。令X为从G到$G'$的同构中的集合，需要$e$到$e'$。 映射$f \rightarrow D^*(f)$（或$D_*(f)$）是双射从X到集合，同构从$D^*(G',T')$到$D^*(G,T)$（或$D_*(G,T)$到$D_*(G',T')$）， 映射 $B'$ 至 B（或 B 至 $B'$）。事实上，这直接来自第 15 号提案和引理 3。

### 习题 {#lie-ix-s4-exercises}

§ 4](exercises/s4/)参见[习题。
