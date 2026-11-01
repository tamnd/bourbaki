---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 7
section_title: Finite dimensional modules over a split semi-simple Lie algebra
lang: zh
source: lie-vii-ix
book_pages: 124-140, 238-250
pdf_pages: 0132-0148, 0246-0258
extraction: native+ocr
subsections:
    - "no": 1
      title: WEIGHTS OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE
      page: 124
      pdf_page: 132
    - "no": 2
      title: HIGHEST WEIGHT OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE
      page: 126
      pdf_page: 134
    - "no": 3
      title: MINUSCULE WEIGHTS
      page: 130
      pdf_page: 138
    - "no": 4
      title: TENSOR PRODUCTS OF $\mathfrak{g}$-MODULES
      page: 132
      pdf_page: 140
    - "no": 5
      title: DUAL OF A $\mathfrak{g}$-MODULE
      page: 134
      pdf_page: 142
    - "no": 6
      title: REPRESENTATION RING
      page: 136
      pdf_page: 144
    - "no": 7
      title: CHARACTERS OF $\mathfrak{g}$-MODULES
      page: 139
      pdf_page: 147
statements: 46
exercises: 27
content_sha256: 5690a3c087bcb6d0eb3fbc8b7251fd64bfb4ae32a4137e6068f78bf604bd476c
translated_from: content/en/lie/VIII/07_s7_finite_dimensional_modules_over_a_split.md
translation_method: google
source_content_sha256: ed5e53f6a5d3e5a763b2ce062b4bcc72122e2012ef339cee5d3bb3a328b965ff
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: f398a86649a76bf46c8ffd60bef262b426784016735d4765982893a2b2080982
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 7。有限维模超过分裂的半单李代数

在本段中，我们保留了§6的一般记号。我们用 R 的权的 P（或 Q）群（或 R 的根权）表示。我们用P（或Q）的元素的$P_+$（或$Q_+$）集合表示，对于B定义的序关系为正。我们用R相对于B的主导权的$P_{++}$集合表示（第1章） VI, §1, no. 10）。 $\mathfrak{h}^*$ 属于的元素 $\lambda$ 到 P（分别为 $P_{++}$）当且仅当所有 $\lambda (H_{\alpha}),\alpha \in B$ 均为整数（分别为整数 $\geq 0$）。我们有$P_{++}\subset P_+$（第VI, §1, no. 6章）。如果$w\in W$，我们用$\varepsilon (w)$表示$w$的行列式，它等于1或$-1$。我们放$\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$。

### 1. 有限维简单$\mathfrak{g}$-模块的权

#### 命题 1 {#lie-viii-s7-prop-1 .statement tag=0138}

令 V 为有限维 $\mathfrak{g}$ 模。

(i) V 属于中的所有权到 P。

(ii) $V =\bigoplus_{\mu\in P}V^\mu$。

(iii) 对于所有$\mu\in \mathfrak{h}^*,V^\mu$ 是$x\in V$ 的集合，使得$h.x=\mu(h)x$ 对于所有$h\in \mathfrak{h}$。

对于所有$\alpha \in B$，存在从$\mathfrak{s}\mathfrak{l}(2, k)$到$\mathfrak{g}$的同态，需要$H$到$H_{\alpha}$。因而，通过 §1, no. 2，Cor。命题$2, (H_{\alpha})_V$可对角化，其特征值为整数。因而，对于$\alpha \in B$，$(H_{\alpha})_V$的集合是可对角化的（代数，第VII, §5, no. 6章，第13条命题）。因而，对于所有 $h\in \mathfrak{h},h_V$ 都是可对角化的。由章。 VII, §1, no. 3，提案$9, V =\bigoplus_{\mu\in\mathfrak{h}^*}V^\mu$。另一方面，如果$V^\mu\not= 0$，则前面的内容表明$\mu(H_{\alpha})\in \mathbf{Z}$对于所有$\alpha \in B$，因而$\mu\in P$。这就证明了(i)和(ii)。我们以同样的方式看到 $\mathfrak{h}_V$ 是可对角化的，因而 (iii)。

#### 推论{#lie-viii-s7-n1-cor-1 .statement tag=0139}

令 $\rho$ 为与 $\rho$ 相关联的 $\mathfrak{g}$ 和 $\Phi$ 双线性形式的有限维表示。

(i) 如果$x, y\in \mathfrak{h}_{\mathbf{Q}}$，则$\Phi (x, y)\in \mathbf{Q}$ 和$\Phi (x, x)\in \mathbf{Q}_+$。

(ii) 如果$\rho$是单射的，则$\Phi$到$\mathfrak{h}$的限制是非简并的。

断言 (i) 由命题 1 得出，因为 P 的元素在 $\mathfrak{h}_{\mathbf{Q}}$ 上有理数值。如果 $\rho$ 是单射的，$\Phi$ 是非简并的（第 I, §6, no. 1 章，命题 1），因而 $\Phi$ 到 $\mathfrak{h}$ 的限制是非简并的（第 VII, §1, no. 3 章，命题 10 (iii)）。

#### 引理 1 {#lie-viii-s7-lem-1 .statement tag=013A}

令 V 为 $\mathfrak{g}$ 模块，且 $\rho$ 相应的表示为 $\mathfrak{g}$。

(i) 如果$a$是$\mathfrak{g}$的幂零元，且$\rho (a)$局部幂零，

$$
\rho (e^{ada}b) =e^{\rho(a)}\rho (b)e^{-\rho(a)}
$$

对于所有$b\in \mathfrak{g}$。

(ii) 如果$\mathfrak{g}^{\alpha}$和$\mathfrak{g}^{-\alpha}$的元素的$\rho$下的$\alpha \in R$和像局部幂零，则V的权的集合在反射$s_{\alpha}$下是稳定的。

对于 (i) 中的假设，对于所有 $n\geq 0$，我们有$\rho$((ad $a$)$^nb$) $=$ (ad $\rho (a)$)$^n\rho (b)$，因而$\rho (e^{ada}b) =e^{ad\rho(a)}\rho (b)$。另一方面，

$$
e^{ad\rho(a)}\rho (b) =e^{\rho(a)}\rho (b)e^{-\rho(a)}
$$

是第 1 章的断言 (ii)。 VII, §3, no. 1、引理 1。

我们现在在(ii)中采用假设。让$\theta_{\alpha}=e^{adX_{\alpha}}e^{adX_{-\alpha}}e^{adX_{\alpha}}$。通过 (i)，存在 $S\in \mathbf{G}\mathbf{L}(V)$，使得对于所有 $b\in \mathfrak{g}$ 都有 $\rho (\theta_{\alpha}b) = S\rho (b)S^{-1}$。现在$\theta_{\alpha}|\mathfrak{h}$是$s_{\alpha}($§2, no. 2的转置，引理1)。令 $\lambda$ 为 V 中的权。存在V的非零元素$x$，使得$\rho (h)x=\lambda (h)x$对于所有$h\in \mathfrak{h}$。然后

$$
\rho (h)S^{-1}x= S^{-1}\rho (^ts_{\alpha}h)x= S^{-1}\lambda (^ts_{\alpha}h)x= (s_{\alpha}\lambda )(h)S^{-1}x
$$

对于所有$h\in \mathfrak{h}$。因而，$s_{\alpha}\lambda$ 是V 中的权。

#### 命题 2 {#lie-viii-s7-prop-2 .statement tag=013B}

令V为有限维$\mathfrak{g}$模和$s\in$Aut$_0(\mathfrak{g})$。

(i) 存在$S\in \mathbf{G}\mathbf{L}(V)$，使得$(s(x))_V= Sx_VS^{-1}$对于所有$x\in \mathfrak{g}$。

(ii) 如果$s\in$ Aut$_e(\mathfrak{g})$，则可以将S选择为$\mathbf{S}\mathbf{L}(V)$的元素，从而使V的所有$\mathfrak{g}$子模块保持稳定。

断言 (ii) 由引理 1 (i) 得出。现在让 $s\in$ Aut$_0(\mathfrak{g})$ 并用 V 定义的 $\mathfrak{g}$ 的$\rho$ 表示表示。通过(ii)，表示$\rho$和$\rho \circ s$成为等价的标量之后扩张。因此它们是等价的（第 I, §3, no. 8 章，命题 13），因此存在 S。

#### 注 1 {#lie-viii-s7-n1-rem-1 .statement tag=013C}

令命题2(i)中的S满足条件，并令$\mathfrak{h}'=s(\mathfrak{h})$；从$\mathfrak{h}^*$到$\mathfrak{h}^{'*}$用$s^*$同构$\lambda  \rightarrow \lambda \circ s^{-1}$表示。很明显，

$$
S(V^{\lambda}) = V^{s^*\lambda}
$$

特别是：

#### 推论 1 {#lie-viii-s7-prop-2-cor-1 .statement tag=013D}

同构$s^*$取V相对于$\mathfrak{h}$的权到V相对于$\mathfrak{h}'$的权； 相应的权具有相同的重数。

#### 推论 2 {#lie-viii-s7-prop-2-cor-2 .statement tag=013E}

让$w\in W$。对于所有 $\lambda \in \mathfrak{h}^*$，向量子空间 $V^{\lambda}$ 和 $V^{w\lambda}$ 具有相同的维数。 V权集合在W下稳定。

事实上，$w$ 是形式 $s^*$ 和 $s\in$ Aut$_e(\mathfrak{g},\mathfrak{h}) ($§2, no. 2，Cor。的 Th。 2）。

#### 注 2 {#lie-viii-s7-n1-rem-2 .statement tag=01L8}

由科.根据第 2 条命题 1 和 §5, no. 3、注 2，相对于 $\mathfrak{g}$ 的规范嘉当子代数以及它们的多重性，谈论 V 的权是有意义的。

#### 注 3 {#lie-viii-s7-n1-rem-3 .statement tag=013F}

引理 1 (i) 和提案 2 仍然有效，具有相同的证明，即使 $\mathfrak{g}$ 不被假定为可拆分。

### 2. 有限维简单 $\mathfrak{g}$ 模块的最高权

#### 定理 1 {#lie-viii-s7-thm-1 .statement tag=013G}

一个简单的 $\mathfrak{g}$ 模是有限维的当且仅当它有最高权属于到 $P_{++}$。

我们用V表示一个简单的$\mathfrak{g}$模块，用$\mathscr{X}$表示它的权的集合。

a) 假设 V 是有限维的。那么 $\mathscr{X}$ 是有限且非空的（命题 1），极大元素 $\omega$ 也是如此。让$\alpha \in B$。然后$\omega +\alpha  \notin \mathscr{X}$，证明$\omega$是V的最高权（§6, no. 2，引理2）。另一方面，存在从$\mathfrak{s}\mathfrak{l}(2, k)$到$\mathfrak{g}$需要$H$到$H_{\alpha}$的同态；根据§1，提案 2 (i)，$\omega (H_{\alpha})$ 是整数 $\geq 0$，所以$\omega \in P_{++}$。

b) 假设V有最高权$\omega \in P_{++}$。令$\alpha \in B$和$e$为V中权$\omega$的原语元素。将$e_j=X_{-\alpha}^je$换成$j\geq 0$，

$m=\omega (H_{\alpha})\in \mathbf{N}$，N = $\sum_{j=0}^mke_j$。根据 §1, no. 2，提案 $1,X_{\alpha}e_{m+1}$ = 0。

如果 $\beta \in B$ 和 $\beta \not=\alpha$，则 $[X_{\beta}, X_{-\alpha}] = 0$，因此 $X_{\beta}e_{m+1}=X_{\beta}X_{-\alpha}^{m+1}e$ = $X_{-\alpha}^{m+1}X_{\beta}e= 0$。如果$e_{m+1}\not= 0$，我们结论认为$e_{m+1}$是原始的，这是荒谬的（§6，命题3（i））；所以$e_{m+1}= 0$。因此，通过 §1, no. 2，Cor。根据命题1，N在$H_{\alpha}, X_{\alpha}$和$X_{-\alpha}$生成的子代数$\mathfrak{s}_{\alpha}$下是稳定的。现在$\mathfrak{s}_{\alpha}$在$\mathfrak{g}$中被还原，因此V的有限维子空间在$\mathfrak{s}_{\alpha}$下稳定的和是V的$\mathfrak{g}$子模（第I, §6, no. 6章，道具1） 7);由于和非零，因此它等于V。由此可见$(X_{\alpha})_V$和$(X_{-\alpha})_V$是局部幂零的。鉴于引理 1 (ii)，$\mathscr{X}$在$s_{\alpha}$下是稳定的，这对于所有$\alpha$都成立。因此$\mathscr{X}$在W下是稳定的。现在P上W的每个轨道都满足$P_{++}$（第VI, §1, no. 10章）。另一方面，如果 $\lambda \in \mathscr{X}\cap P_{++}$，则 $\lambda =\omega -\sum_{\alpha\in B}n_{\alpha}\alpha =\sum_{\alpha\in B}n'_{\alpha}\alpha$ 以及 $n_{\alpha}\in \mathbf{N}$ 和 $n'_{\alpha}\geq 0$ 对于所有 $\alpha \in B$

（第V, §3, no. 5、引理6章）。所以$\mathscr{X}\cap P_{++}$是有限的，因此$\mathscr{X}$也是有限的。由于每个权都有有限的重数（§6, no. 1，命题 1 (ii)），V 是有限维的。

#### 推论 1 {#lie-viii-s7-thm-1-cor-1 .statement tag=013H}

如果$\lambda \in \mathfrak{h}^*$和$\lambda  \notin P_{++}$，则$\mathfrak{g}$模$E(\lambda ) ($§6, no. 3）是无限维的。

#### 推论 2 {#lie-viii-s7-thm-1-cor-2 .statement tag=013I}

$\lambda \in P_{++}$的$\mathfrak{g}$模$E(\lambda )$构成有限维简单$\mathfrak{g}$模的类代表的集合。

$\mathfrak{g}$-模$E(\lambda )$，其中$\lambda$是基本权，称为基本$\mathfrak{g}$-模； 相应的表示称为$\mathfrak{g}$的基数表示；它们是绝对不可约的（§6, no. 2，命题 3 (iv)）。

如果V是有限维$\mathfrak{g}$模且$\lambda \in P_{++}$，则型$E(\lambda )$的V的同典型分量称为最高权$\lambda$的V的同典型分量。

#### 注 1 {#lie-viii-s7-n2-rem-1 .statement tag=013J}

令 $E(\lambda ),s\in$ Aut($\mathfrak{g}$) 上的 $\mathfrak{g}$ $\lambda \in P_{++},\rho_{\lambda}$ 表示，以及 Aut(R$,B$) 上的 $s$ $\sigma$ 典范像 $($§5, no. 3，Cor.提案 5 中的 1）。那么$\rho_{\lambda}\circ s$就相当于$\rho_{\sigma \lambda}$；事实上，如果 $s\in$ Aut$_0(\mathfrak{g}),\rho_{\lambda}\circ s$ 和 $\rho_{\sigma \lambda}$ 等价于 $\rho_{\lambda}$（命题 2）；并且，如果$s$使$\mathfrak{h}$和B稳定，则$\rho_{\lambda}\circ s$是最高权$\sigma \lambda$的简单。

特别是，基本的表示被$s$排列，并且这个置换是恒等式当且仅当$s\in$Aut$_0(\mathfrak{g})$。

#### 命题 3 {#lie-viii-s7-prop-3 .statement tag=013K}

令V为有限维$\mathfrak{g}$模，$\mathscr{X}$为权的集合。令$t\in \mathbf{Z}$的$\lambda \in \mathscr{X},\alpha \in R$、I集合使得I的$\lambda +t\alpha \in \mathscr{X},p$（分别$-q$）最大的（分别最小的）元素。令$m_t$为$\lambda +t\alpha$中的重数。

(i) I = $-q, p$ 和 $q-p=\lambda (H_{\alpha})$。

(ii) 对于任何整数、$u\in 0, p+q,\lambda + (p-u)\alpha$和$\lambda + (-q+u)\alpha$，共轭低于$s_{\alpha}$和$m_{-q+u}=m_{p-u}$。

(iii) 如果$t\in \mathbf{Z}$和$t <(p-q)/2$，则$(X_{\alpha})_V$映射$V^{\lambda+t\alpha}$内射到$V^{\lambda+(t+1)\alpha}$。

(iv) 函数 $t \rightarrow m_t$ 在 $-q,(p-q)/2$ 上是递增，在$(p-q)/2, p$ 上是递减。

让$\alpha \in B$。给出V由$\mathfrak{g}$的元素$X_{\alpha}, X_{-\alpha}, H_{\alpha}$定义的$\mathfrak{s}\mathfrak{l}(2, k$)模块结构。 $V^{\lambda+p\alpha}$ 的每个非零元素都是本原的。因而，$(\lambda +p\alpha )(H_{\alpha})\geq 0$ 和 $(X_{-\alpha})^rV^{\lambda+p\alpha}\not= 0$ 为

$$
0\leq r\leq (\lambda +p\alpha )(H_{\alpha}) =\lambda (H_{\alpha}) + 2p
$$

（§1, no. 2，提案 2）。由此可见，$V^{\lambda+t\alpha}\not= 0$ 对应$p\geq t\geq p-(\lambda (H_{\alpha}) + 2p)$，因而$p+q\geq \lambda (H_{\alpha}) + 2p$。 应用这个结果到 $-\alpha$ 给出

$$
p+q\geq \lambda (H_{-\alpha}) + 2q=-\lambda (H_{\alpha}) + 2q
$$

因而 $q-p=\lambda (H_{\alpha})$ 和 $\lambda +t\alpha \in \mathscr{X}$ 对于 $p\geq t\geq  -q$，这证明了 (i)。

我们有 $s_{\alpha}(\alpha ) =-\alpha$，所有 $\mu\in \mathfrak{h}^*$ 都有 $s_{\alpha}(\mu)\in \mu+k\alpha$。由于 W 使 $\mathscr{X}$ 保持稳定（$2$ 的 Cor. 2），$,s_{\alpha}$ 使 $\{\lambda -q\alpha , \lambda -q\alpha +\alpha , . . . , \lambda +p\alpha \}$ 保持稳定，并且对于所有 $u\in k$，将 $\lambda -q\alpha +u\alpha$ 变为 $\lambda +p\alpha -u\alpha$。使用 Cor.再次根据 Prop. 2 的 2，我们看到每个整数 $u\in 0, p+q$ 都有 $m_{-q+u}=m_{p-u}$。这就证明了(ii)。

由 §1 提供，Cor.命题$2, (X_{\alpha})_V|V^{\lambda+t\alpha}$是$t <(p-q)/2$的单射。现在$(X_{\alpha})_V$映射$V^{\lambda+t\alpha}$到$V^{\lambda+(t+1)\alpha}$。因而 $m_{t+1}\geq m_t$ 对应 $t <(p-q)/2$。将 $\alpha$ 更改为 $-\alpha$，我们看到 $m_{t+1}\leq m_t$ 对应 $t >(p-q)/2$。这就证明了(iii)和(iv)。

#### 推论 1 {#lie-viii-s7-prop-3-cor-1 .statement tag=013L}

如果$\lambda \in \mathscr{X}$和$\lambda (H_{\alpha})\geq 1$，则$\lambda -\alpha \in \mathscr{X}$。如果$\lambda +\alpha \in \mathscr{X}$和$\lambda (H_{\alpha}) = 0$，则$\lambda \in \mathscr{X}$和$\lambda -\alpha \in \mathscr{X}$。

这紧随提案 3 (i) 而来。

#### 推论 2 {#lie-viii-s7-prop-3-cor-2 .statement tag=01J4}

让$\mu\in P_{++}$和$\nu \in Q_+$。如果$\mu+\nu \in \mathscr{X}$，则$\mu\in \mathscr{X}$。

写出 $\nu =\sum_{\alpha\in B}c_{\alpha}.\alpha$，其中 $c_{\alpha}\in \mathbf{N}$ 代表所有 $\alpha \in B$。推论很清楚

当$\sum_{\alpha\in B}c_{\alpha}= 0$时；假设$\sum_{\alpha\in B}c_{\alpha}>0$，并根据归纳对$\sum_{\alpha\in B}c_{\alpha}$进行论证。令$(\cdot  | \cdot )$为$\mathfrak{h}^*_{\mathbf{R}}$上的W不变非简并正对称双线性形式。那么$(\nu |\sum_{\alpha\in B}c_{\alpha}.\alpha )>0$，所以存在$\beta \in B$使得$c_{\beta}\geq 1$和

$(\nu |\beta )>0$，因而$\nu (H_{\beta})\geq 1$。从$\mu\in P_{++}$开始，得出$(\mu+\nu )(H_{\beta})\geq 1$。由科. $1,\mu+ (\nu -\beta )\in \mathscr{X}$，申请归纳假设就够了。

#### 推论 3 {#lie-viii-s7-prop-3-cor-3 .statement tag=013M}

设$v\in V$是权$\omega$的原语。令$\Sigma$为$\alpha \in B$的集合，使得$\omega (H_{\alpha}) = 0$。 $kv$线的$\mathfrak{g}$中的稳定子是与$\Sigma ($§3, no. 4、注相关的抛物线子代数$\mathfrak{p}_{\Sigma}$）。

替换V由$v$生成的$\mathfrak{g}$子模块生成，如有必要，我们可以假设V是简单的。设$\mathfrak{s}$为稳定子。我们有 $(\mathfrak{n}_+)_Vv$ = 0, $(\mathfrak{h})_Vv\subset kv$。令$\alpha \in B$ 使得$\omega (H_{\alpha}) = 0$。我们有 $\omega +\alpha  \notin \mathscr{X}$，因此有 $\omega -\alpha  \notin \mathscr{X}$（命题 3 (i)），因此有 $(\mathfrak{g}^{-\alpha})_Vv= 0$。上式证明$\mathfrak{p}_{\Sigma}\subset \mathfrak{s}$。如果$\mathfrak{p}_{\Sigma}\not=\mathfrak{s}$，则$\mathfrak{s}=\mathfrak{p}_{\Sigma'}$，其中$\Sigma '$严格来说是B的子集包含$\Sigma$。让 $\beta \in \Sigma '$ **--** $\Sigma$。然后$\mathfrak{g}^{-\beta}$稳定$kv$，从而消灭$v$。但是，从$\omega (H_{\beta})>0$开始，这个与……矛盾提案3 (iii)。 Q.E.D.

如果 P 的子集 $\mathscr{X}$ 满足以下条件，则称为 R 饱和的：对于所有 $\lambda \in \mathscr{X}$ 和所有 $\alpha \in R$，对于 0 到 $\lambda (H_{\alpha})$ 之间的所有整数 $t$，我们有 $\lambda -t\alpha \in \mathscr{X}$。从$s_{\alpha}(\lambda ) =\lambda -\lambda (H_{\alpha})\alpha$开始，我们看到P的R饱和子集在W下是稳定的。设$\mathscr{Y}\subset P$。如果对于所有 $\alpha \in R$，$\lambda +\alpha  \notin \mathscr{Y}$ 或 $\lambda -\alpha  \notin \mathscr{Y}$，则$\mathscr{Y}$ 的元素 $\lambda$ 称为$\mathscr{Y}$ 中的 R 极值。

#### 命题 4 {#lie-viii-s7-prop-4 .statement tag=013N}

令V为有限维$\mathfrak{g}$模，$d$整数$\geq 1$。 重数$\geq d$V权集合是R-饱和的。

这直接来自于第 3 条命题。

#### 命题 5 {#lie-viii-s7-prop-5 .statement tag=013O}

令V为有限维简单$\mathfrak{g}$模，$\omega$为最高权，$\mathscr{X}$为权的集合。 选择 $\mathfrak{h}^*_{\mathbf{R}}$ 上的 W 不变非简并正对称双线性形式 $(\cdot |\cdot )$，并令 $\lambda  \rightarrow  \|\lambda \|= (\lambda |\lambda )^{1/2}$ 为相应的范数。

(i) $\mathscr{X}$ 是 P 包含 $\omega$ 的最小的 R 饱和子集。

(ii) $\mathscr{X}$ 的 R 极值元素是 $\omega$ 的 W 变换。

(iii) 如果$\mu\in \mathscr{X}$，我们就有$\|\mu\| \leq  \|\omega \|$。如果，在加法，$\mu\not=\omega$，我们有$\|\mu+\rho \|<\|\omega +\rho \|$。如果 $\mu$ 不是 $\mathscr{X}$ 中的 R 极值，则 $\|\mu\|<\|\omega \|$。

(iv) 我们有$\mathscr{X}= W.(\mathscr{X}\cap P_{++})$。 $P_{++}$ 属于的元素 $\lambda$ 到 $\mathscr{X}\cap P_{++}$ 当且仅当$\omega -\lambda \in Q_+$。

(i) 令 $\mathscr{X}'$ 为 P 包含 $\omega$ 的最小的 R 饱和子集。我们有 $\mathscr{X}'\subset \mathscr{X}$（命题 4）。假设$\mathscr{X}\not=\mathscr{X}'$。令 $\lambda$ 为 $\mathscr{X}$ **--** $\mathscr{X}'$ 中的极大元素。由于$\lambda \not=\omega$，存在$\alpha \in B$使得$\lambda +\alpha \in \mathscr{X}$。按照命题 3 引入 $p$ 和 $q$。因为 $\lambda$ 在 $\mathscr{X}$ **--** $\mathscr{X}',\lambda +p\alpha \in \mathscr{X}'$ 中最大。根据命题 3 (ii)，由于 $\mathscr{X}'$ 在 W 下是稳定的，$\lambda -q\alpha \in \mathscr{X}'$ 是稳定的。因此，对于区间 $-q, p$ 内的每个整数 $u$，$\lambda +u\alpha \in \mathscr{X}'$ 都是稳定的。这与……矛盾 $\lambda  \notin \mathscr{X}'$ 并证明 (i)。

(ii) 显然$\omega$是$\mathscr{X}$的R极值元素；因此，它的 W 变换在 $\mathscr{X}$ 中也是 R 极值。令$\lambda$为$\mathscr{X}$的R极值元素；我们将证明$\lambda \in W.\omega$。由于存在$w\in W$使得$w\lambda \in P_{++}$（第VI, §1, no. 10章），我们可以假设$\lambda \in P_{++}$。设 $\alpha \in B$；引入$p$和$q$，如命题3。由于$\lambda$是R极值，$p= 0$或$q= 0$。自从

$$
q-p=\lambda (H_{\alpha})\geq 0
$$

我们不能有$p >0$。因此$p= 0$和$\lambda =\omega$。

(iii)设$\mu\in \mathscr{X}\cap P_{++}$。然后$\omega +\mu\in P_{++}$和$\omega -\mu\in Q_+($§6, no. 1，命题1)，所以$0\leq (\omega -\mu|\omega +\mu) = (\omega |\omega )-(\mu|\mu)$；因此，$(\mu|\mu)\leq (\omega |\omega )$，以及通过使用 Weyl 群将这个扩展转换为所有 $\mu\in \mathscr{X}$。如果 $\mu\in \mathscr{X}$ **--** $\{\omega \}$，

$$
(\mu+\rho |\mu+\rho ) = (\mu|\mu) + 2(\mu|\rho ) + (\rho |\rho )\leq (\omega |\omega ) + 2(\mu|\rho ) + (\rho |\rho )
$$

$$
= (\omega +\rho |\omega +\rho )-2(\omega -\mu|\rho )
$$

现在$\omega -\mu=\sum_{\alpha\in B}n_{\alpha}\alpha$和整数$n_{\alpha}\geq 0$不是所有零，所以从$(\rho |\alpha )>0$开始$(\omega -\mu|\rho )>0$对于所有$\alpha \in B$（第VI, §1, no. 10，提案29（iii））。如果$\mu$不是$\mathscr{X}$中的R极值，则存在$\alpha \in R$使得$\mu+\alpha \in \mathscr{X}$和$\mu-\alpha \in \mathscr{X}$；然后

$\|\mu\|<$ 上($\|\mu+\alpha \|,\|\mu-\alpha \|$)$\leq$ 上$_{\lambda\in\mathscr{X}}\|\lambda \|$

最后一个上界是前一个$\|\omega \|$。

(iv) 我们有第 1 章的$\mathscr{X}= W.(\mathscr{X}\cap P_{++})$。 VI, §1, no. 10。如果 $\lambda \in \mathscr{X}$，则$\omega -\lambda \in Q_+($§6, no. 1，命题 1)。如果 $\lambda \in P_{++}$ 和 $\omega -\lambda \in Q_+$，则 $\lambda \in \mathscr{X}$（第 3 条命题第 2 条）。

#### 推论{#lie-viii-s7-n2-cor-1 .statement tag=013P}

令$\mathscr{X}$为P的有限R饱和子集。存在一个有限维$\mathfrak{g}$模，其权的集合为$\mathscr{X}$。

由于$\mathscr{X}$在$W,\mathscr{X}$下稳定，因此最小的R饱和集合包含$\mathscr{X}\cap P_{++}$。根据提案 5 (i)，$\mathscr{X}$ 是集合权 $\bigoplus_{\lambda\in\mathscr{X}\cap P_{++}}E(\lambda )$。

#### 注 2 {#lie-viii-s7-n2-rem-2 .statement tag=013Q}

回想一下（第 17 条命题第 VI, §1, no. 6 章，Cor.3），存在 W 的唯一元素 $w_0$，变换 B 进入$-B$；我们有$w_0^2= 1$。并且 $-w_0$ 尊重 P 上的序关系。考虑到这一点，令 V 为有限维简单 $\mathfrak{g}$ 模，$\omega$ 为最高权。那么$w_0(\omega )$就是V中最低的权，它的重数就是1。

### 3.极小权

#### 命题 6 {#lie-viii-s7-prop-6 .statement tag=013R}

让 $\lambda \in P$ 和 $\mathscr{X}$ 最小的 R 饱和子集的 P 包含 $\lambda$。 选择范数 $\| \cdot  \|$ 如提案 5 中所示。以下条件是等效的：

(i) $\mathscr{X}= W.\lambda$；

(ii) $\mathscr{X}$ 中的所有元素具有相同的范数；

(iii) 对于所有$\alpha \in R$，我们有$\lambda (H_{\alpha})\in  \{0,1,-1\}$。

P 包含元素 $\lambda$ 满足上述条件的每个非空 R 饱和子集。

介绍一下条件：

(ii$'$) 对于所有 $\alpha \in R$ 以及对于 0 到 $\lambda (H_{\alpha})$ 之间的每个整数 $t$，

$$
\|\lambda -t\alpha \| \geq  \|\lambda \|
$$

(i) $=\Rightarrow$ (ii) $=\Rightarrow$ (ii$'$)$:$ 这很清楚。

(ii$'$)$=\Rightarrow$(iii)：假设满足条件(ii$'$)。让$\alpha \in R$。我们有 $\|\lambda \|=\|\lambda -\lambda (H_{\alpha})\alpha \|$，因此每个整数 $t$ 的 $\|\lambda -t\alpha \|<\|\lambda \|$ 严格在 0 到 $\lambda (H_{\alpha})$ 之间；因此，不可能有这样的整数，所以$|\lambda (H_{\alpha})| \leq 1$。

(iii)$=\Rightarrow$(i)：假设满足条件(iii)。设$w\in W$和$\alpha \in R$。然后$(w\lambda )(H_{\alpha}) =\lambda (H_{w^{-1}\alpha})\in  \{0,1,-1\}$；因此，如果 $t$ 是整数，介于 0 和 $(w\lambda )(H_{\alpha}),w\lambda -t\alpha$ 之间，则等于 $w\lambda$ 或 $s_{\alpha}(w\lambda )$。这证明$W.\lambda$是R饱和的，所以$\mathscr{X}= W.\lambda$。

令$\mathscr{Y}$为P的非空R饱和子集。存在最小范数的$\mathscr{Y}$元素$\lambda$。很明显，$\lambda$满足条件（ii$'$），因此最后一个断言等于命题。

#### 命题 7 {#lie-viii-s7-prop-7 .statement tag=013S}

令V为有限维简单$\mathfrak{g}$模，V的权的$\mathscr{X}$集合，以及$\mathscr{X}$的$\lambda$最高元素 （cf. 提案 5 (i)）。提案6的条件(i)、(ii)和(iii)等价于：

(iv) 对于所有$\alpha \in R$和所有$x\in \mathfrak{g}^{\alpha}$，我们有$(x_V)^2= 0$。

如果满足这些条件，则V中的所有权都有重数 1。

如果满足(i)，则$\mathscr{X}= W.\lambda$和权都具有与$\lambda$相同的重数（命题2的Cor.2），在其他字，重数1。此外，如果$w\in W$和$\alpha \in R,w\lambda +t\alpha$不能是权 V 除非 $|t| \leq 1$；因此，如果$x\in \mathfrak{g}^{\alpha}$，

$$
(x_V)^2(V^{w(\lambda)})\subset V^{w(\lambda)+2\alpha}= 0
$$

所以$(x_V)^2= 0$，证明(i)$=\Rightarrow$(iv)。

相反，假设满足(iv)。设$\alpha \in R$，并给V由$\mathfrak{g}$的元素$X_{\alpha}, X_{-\alpha}, H_{\alpha}$定义的$\mathfrak{s}\mathfrak{l}(2, k)$模块结构。 条件 (iv)，应用于$x=X_{\alpha}$，意味着$\mathfrak{s}\mathfrak{l}(2, k$)-模块V属于到$\{0,1,-1\}$的权（cf.§1, no. 2，Prop.2的Cor.）。特别是$\lambda (H_{\alpha})\in  \{0,1,-1\}$，所以 (iv) $=\Rightarrow$ (iii)。

#### 命题 8 {#lie-viii-s7-prop-8 .statement tag=013T}

假设 $\mathfrak{g}$ 很简单。用B的$\alpha_1, . . . , \alpha_l$元素表示。令$\varpi_1, . . . , \varpi_l$为相应的基本权。令 $H$ = $n_1H_{\alpha_1}+\cdots +n_lH_{\alpha_l}$ 为 $R^{\vee}$ 的最高根，且 $i\in  \{1, . . . , l\}$ 的 J 集合使得 $n_i= 1$。让 $\lambda \in P_{++}$ **--** $\{0\}$。那么第 6 条命题的条件(i)、(ii)和(iii)等价于以下条件：

(v) $\lambda (H) = 1$；

(vi) 存在$i\in J$使得$\lambda =\varpi_i$。

$P(R)/Q(R)$的非零元素代表P(R)中的$\varpi_i$、$i\in J$、形式系统。

让$\lambda =u_1\varpi_1+\cdots +u_l\varpi_l$，其中$u_1, . . . , u_l$是整数$\geq 0$，而不是全部零。然后$\lambda (H) =u_1n_1+\cdots +u_ln_l$和$n_1\geq 1, . . . , n_l\geq 1$，立即给出(v)和(vi)的等价。另一方面，$\lambda (H) =$sup$_{\alpha\in R_+}\lambda (H_{\alpha})$和$\lambda (H)>0$，因为$\lambda$是$P_{++}$的非零元素。因此

对于所有 $\alpha \in R$，条件 (v) 相当于条件 $\lambda (H_{\alpha})\in  \{0,1\}$，在第 6 条的其他字至条件 (iii) 中。

命题中的最后一个断言源自第1章。 VI, §2, no. 3，科。提案 6。

#### 定义 1 {#lie-viii-s7-def-1 .statement tag=013U}

假设 $\mathfrak{g}$ 很简单。 $(\mathfrak{g},\mathfrak{h})$的极小权是$P_{++}$ **--** $\{0\}$的元素，满足第6、7和8条的等价条件(i)、(ii)、(iii)、(iv)、(v)和(vi)。

#### 注 {#lie-viii-s7-n3-rem-1 .statement tag=013V}

假设$\mathfrak{g}$很简单。令 $\Sigma^{'\vee}$ 为仿射 Weyl 群 $W_a(R^{\vee})$ 的 Coxeter 图。回想一下，$\Sigma^{'\vee}$ 的顶点是 $W(R^{\vee})$ 的 Coxeter 图 $\Sigma^{\vee}$ 的顶点，以及补充顶点 0。 群 $A(R^{\vee})$ 在 $\Sigma^{'\vee}$ 上运行，保持 0 固定。 群 Aut($\Sigma^{'\vee}$) 与 $A(R^{\vee})/W(R^{\vee})$ 的半直接乘积与群 $\Gamma_C$（cf. 第 VI, §2, no. 3 章和第 VI, §4, no. 3）典型同构；显然（Aut $\Sigma^{'\vee}$）$(0) =\Gamma_C(0)$； $\Gamma_C(0)$ 由 0 和 $i\in J$ 的$\Sigma^{\vee}$ 相应的到$\varpi_i$ 的顶点组成（cf. 第 VI, §2 章，第 5 条命题和no. 3 的注 1）。综上所述，极小权是$\Sigma^{\vee}$顶点的基本权相应的，可以从0通过Aut($\Sigma^{'\vee}$)的元素的运算得到。

与第 80 章的记号 VI，板片I至IX，由上可知极小权如下：

型$A_l(l\geq 1):\varpi_1, . . . , \varpi_l$。

型$B_l(l\geq 2):\varpi_l$。

型$C_l(l\geq 2):\varpi_1$。

型$D_l(l\geq 3):\varpi_1, \varpi_{l-1}, \varpi_l$。

型$E_6:\varpi_1, \varpi_6$。

型$E_7:\varpi_7$。

对于型$E_8,F_4,G_2$，没有极小权。

### 4. 张量积 $\mathfrak{g}$-模块

令 $E,F$ 为$\mathfrak{g}$-模块。对于所有 $\lambda , \mu\in \mathfrak{h}^*, E^{\lambda}\otimes F^\mu\subset (E\otimes F)^{\lambda+\mu}$（第 VII, §1, no. 1 章，提案 2 (ii)）。如果 E 和 F 是有限维的，则 $E =\sum_{\lambda\in P}E^{\lambda}$

和$F =\sum_{\mu\in P}F^\mu$；因而，

$$
(E\otimes F)^{\nu}=\sum_{\lambda ,\mu\in P,\lambda+\mu=\nu}E^{\lambda}\otimes F^\mu
$$

在其他字中，配备型$P, E\otimes F$的分级是分级向量空间E和F的分级张量积。

#### 命题 9 {#lie-viii-s7-prop-9 .statement tag=013W}

令 $E,F$ 为有限维简单 $\mathfrak{g}$ 模，分别具有最高权 $\lambda , \mu$。

(i) 最高权 $\lambda +\mu$ 的$E\otimes F$ 分量是简单子模，由$(E\otimes F)^{\lambda+\mu}= E^{\lambda}\otimes F^\mu$ 生成。

(ii) $E\otimes F$ 中任意简单子模的最高权是$\leq \lambda +\mu$（cf. §9，命题 2）。

如果$\alpha , \beta \in P$并且如果$E^{\alpha}\otimes F^{\beta}\not= 0$，则$\alpha \leq \lambda$和$\beta \leq \mu$。因而，$(E\otimes F)^{\lambda+\mu}$等于$E^{\lambda}\otimes F^\mu$，因此是维数1，$\lambda +\mu$是$E\otimes F$的最高权。 $E^{\lambda}\otimes F^\mu$ 的每个非零元素都是本原的。根据§6, no. 2的命题4，最高权$\lambda +\mu$的$E\otimes F$同型成分的长度为1。

#### 注 {#lie-viii-s7-n4-rem-1 .statement tag=013X}

保留命题 9 中的记号。令C 为最高权$\lambda +\mu$ 的$E\otimes F$ 的同型成分。那么C只依赖于E和F，而不依赖于$\mathfrak{h}$和基B的选择。在其他字中，令$\mathfrak{h}'$为$(\mathfrak{g},\mathfrak{h}')$的$\mathfrak{g}, R'$根系分裂嘉当子代数，和 $R'$ 的 $B'$ 基；令$\lambda ', \mu'$为$E,F$相对于$\mathfrak{h}'$和$B'$的最高权；令$C'$为最高权$\lambda '+\mu'$的$E\otimes F$的同型成分；然后$C'= C$。事实上，为了证明这一点，我们可以通过基域的扩张来假设 $k$ 是代数封闭的。然后存在$s\in$ Aut$_e(\mathfrak{g})$，需要$\mathfrak{h}$到$\mathfrak{h}', R$到$R', B$到$B'$。令$S\in \mathbf{S}\mathbf{L}(E\otimes F)$具有no. 1命题2中的性质。那么 $S((E\otimes F)^{\lambda+\mu}) = (E\otimes F)^{\lambda'+\mu'}$ 和 S(C) = C。因此$(E\otimes F)^{\lambda'+\mu'}\subset C'\cap S(C) = C'\cap C$，所以$C'= C$。因此，对于 2 个类有限维简单 $\mathfrak{g}$ 模块，我们可以规范地关联第三个；在其他字中，我们定义了有限维简单$\mathfrak{g}$模合成律的类集合$\mathfrak{S}_{\mathfrak{g}}$。有了这个结构，$\mathfrak{S}_{\mathfrak{g}}$ 与加法幺半群 $P_{++}$ 是标准同构的。

#### 推论 1 {#lie-viii-s7-prop-9-cor-1 .statement tag=01J5}

令$(\varpi_{\alpha})_{\alpha\in B}$是相对于B的基本权族。令$\lambda =\sum_{\alpha\in B}m_{\alpha}\varpi_{\alpha}\in P_{++}$。对于所有$\alpha \in B$，让$E_{\alpha}$是最高权$\varpi_{\alpha}$的简单$\mathfrak{g}$模块。在$\mathfrak{g}$模$\bigotimes_{\alpha\in B}(\bigotimes^{m_{\alpha}}E_{\alpha})$中，最高权$\lambda$的同型成分为长度1。

这是根据归纳在 $\sum_{\alpha\in B}m_{\alpha}$ 提出的第 9 号提案得出的。

#### 推论 2 {#lie-viii-s7-prop-9-cor-2 .statement tag=013Y}

假设$k$是$\mathbf{R}$或$\mathbf{C}$或非离散完全超度量域。令 G 为李群和李代数 $\mathfrak{g}$。假设，对于 $\mathfrak{g}$ 的任何基本表示 $\rho$，存在 G 的解析线性表示 $\rho '$，使得 $\rho = L(\rho ')$。那么，对于 $\mathfrak{g}$ 的任意有限维线性表示 $\pi$，存在 G 的解析线性表示 $\pi '$，使得 $\pi = L(\pi ')$。

我们使用Cor的记号。 1. 在$X =\bigotimes_{\alpha\in B}(\bigotimes^{m_{\alpha}}E_{\alpha})$上存在G的表示$\sigma$，使得$L(\sigma )$对应到X的$\mathfrak{g}$模结构（第41条第III, §3, no. 11章，Cor.3）。令 C 为最高权 $\lambda$ 的 X 的同型组件。鉴于章。 III, §3, no. 11，第40条命题，足以证明C在$\sigma (G)$下稳定。设 $g\in G$ 和 $\varphi =$ Ad($g$)。然后 $\sigma (g)a_X\sigma (g)^{-1}= (\varphi (a))_X$ 代表所有 $a\in \mathfrak{g}$。另一方面，$\varphi$是$\mathfrak{g}$的自同构，需要$\mathfrak{h}$到$\mathfrak{h}', R$到$R'= R(\mathfrak{g},\mathfrak{h}'), B$到基$B'$$R'$，以及$\varpi_{\alpha}$到最高权 $E_{\alpha}$相对于$\mathfrak{h}'$和$B'$的$\varpi '_{\alpha}$（因为$\varphi$变换$E_{\alpha}$变成与$E_{\alpha}$同构的$\mathfrak{g}$模块）。因此，$\varphi$需要$\lambda$到$\sum m_{\alpha}\varpi '_{\alpha}$。上面注，$\sigma (g)(C) = C$。

#### 命题 10 {#lie-viii-s7-prop-10 .statement tag=013Z}

让$\lambda , \mu\in P_{++}$。让$E,F,G$是简单的$\mathfrak{g}$-模块与最高权$\lambda , \mu, \lambda +\mu$。令$\mathscr{X}$（或$\mathscr{X}',\mathscr{X}''$）为E（或$F,G$）的权中的集合。然后$\mathscr{X}''=\mathscr{X}+\mathscr{X}'$。

我们有 $E =\bigoplus_{\nu\in P}E^{\nu},F =\bigoplus_{\sigma\in P}F^{\sigma}$，所以 $E\otimes F$ 是直和

$$
(E\otimes F)^{\tau}=\sum_{\nu+\sigma=\tau}E^{\nu}\otimes F^{\sigma}
$$

根据命题 9，G 可以被识别为 $E\otimes F$ 的$\mathfrak{g}$子模，因此$\mathscr{X}''\subset \mathscr{X}+\mathscr{X}'$。 我们有$G^{\tau}= G\cap (E\otimes F)^{\tau}$，并且足以证明，对于$\nu \in \mathscr{X}$和$\sigma \in \mathscr{X}'$，我们有$G\cap (E\otimes F)^{\nu+\sigma}\not= 0$。 Let $(e_1, . . . , e_n)$ (resp. $(f_1, . . . , f_p)$) be a basis of E (resp. F) 元素中的由……组成，其中每个属于到一些$E^{\nu}$（分别为$F^{\sigma}$），并且使得$e_1\in E^{\lambda}$（分别为$f_1\in F^\mu$）。 $E\otimes F$的$e_i\otimes f_j$形式基。 假设要证明的结果是假的。 则存在对$(i, j)$，使得G的每个元素的指标$(i, j)$的坐标为零。 令 U 为 $\mathfrak{g}, U'$ 的包络代数，是 U 的$U,c$ 余积的对偶。 对于所有$u\in U$，令$x_i(u)$（或$y_j(u)$）为指标、$i$（或$j$）的$u(e_1)$（或$u(f_1)$）的坐标；设$z_{ij}(u)$为$u(e_1\otimes f_1)$的指标$(i, j)$的坐标。 然后$x_i, y_j, z_{ij}\in U'$。 现在$e_1$生成是$\mathfrak{g}$-模块E，所以$x_i\not= 0$，类似的$y_j\not= 0$。 通过 $\mathfrak{g}$-模块 $E\otimes F$ 的定义（第 1 章） I, §3, no. 2），如果$c(u) =\sum u_s\otimes u'_s$，我们有

$$
z_{ij}(u) =\sum_sx_i(u_s).y_j(u'_s) =\langle c(u), x_i\otimes y_j\rangle
$$

在其他字中，$z_{ij}$是代数$U'$中$x_i$和$y_j$的乘积。但是这个代数是整环（第II, §1, no. 5章，第10条命题），所以$z_{ij}\not= 0$。由于$u(e_1\otimes f_1)\in G$对于所有$u\in U$，这是一个矛盾。

### 5. 对偶的$\mathfrak{g}$-模块

令$E,F$为$\mathfrak{g}$-模块。回想一下（第 I, §3, no. 3 章）Hom$_k(E,F)$ 有一个规范的 $\mathfrak{g}$ 模块结构。令$\varphi$为Hom$_k(E,F)$中权$\lambda$的元素。如果$\mu\in \mathfrak{h}^*$，则$\varphi (E^\mu)\subset F^{\lambda+\mu}$（第VII, §1, no. 1章，提案2 (ii)）。因此，如果 E 和 F 是有限维的，则 Hom$_k(E,F)$ 中权 $\lambda$ 的元素是次数 $\lambda$ 在代数意义上的分级同态，第 1 章。 II, §11, no. 2，防御。 4.

#### 命题 11 {#lie-viii-s7-prop-11 .statement tag=0140}

令 E 为有限维 $\mathfrak{g}$ 模，并考虑 $\mathfrak{g}$ 模 $E^*=$ Hom$_k(E, k)$。

(i) 元素$\lambda \in P$是$E^*$的权当且仅当$-\lambda$是E的权，并且$E^*$中$\lambda$的重数等于E中$-\lambda$的重数。

(ii) 如果 E 是简单的并且有最高权 $\omega ,E^*$ 是简单的并且有最高权 $-w_0(\omega )$ (cf. no. 2, 注 2)。

将$k$视为一个平凡的$\mathfrak{g}$模块，其元素为权0。根据上面所述，权$\lambda$的$E^*$的元素从E到$k$为同态，其中如果$\mu\not=-\lambda$，则在$E^\mu$消失。这就证明了(i)。如果 E 是简单的，$E^*$ 也是简单的（I, §3, no. 3 章），并且最后一个断言是从 no. 2 的注 2 得出的。

#### 注 1 {#lie-viii-s7-n5-rem-1 .statement tag=0141}

令 $E,E^*$ 如命题 11 中那样，并且 $\sigma \in$ Aut($\mathfrak{g},\mathfrak{h}$) 使得 §5, no. 1 的记号中的$\varepsilon (\sigma ) =-w_0$（§5, no. 2，命题 2）。令 $\rho , \rho '$ 为与 $E,E^*$ 伴随的 $\mathfrak{g}$ 中的表示。那么$\rho \circ \sigma$是$\mathfrak{g}$与最高权$-w_0(\omega )$的简单表示，因此$\rho \circ \sigma$等价于$\rho '$。

#### 注 2 {#lie-viii-s7-n5-rem-2 .statement tag=0142}

假设$w_0=-1$。那么，对于任何有限维 $\mathfrak{g}$-模 E，E 与 $E^*$ 同构的。回想一下，如果 $\mathfrak{g}$ 很简单，则在以下情况下使用 $w_0=-1$：型 $A_1,B_l(l\geq 2), C_l(l\geq 2), D_l(l$ 的 $\mathfrak{g}$ 甚至 $\geq 4), E_7,E_8,F_4,G_2$（第 VI 章，板）。

#### 引理 2 {#lie-viii-s7-lem-2 .statement tag=0143}

让$h^0=\sum_{\alpha\in R_+}H_{\alpha}$。然后是$h^0=\sum_{\alpha\in B}a_{\alpha}H_{\alpha}$，其中$a_{\alpha}$是整数$\geq 1$。令 $(b_{\alpha})_{\alpha\in B},(c_{\alpha})_{\alpha\in B}$ 为标量族，使得 $b_{\alpha}c_{\alpha}=a_{\alpha}$ 对于所有 $\alpha \in B$。把$x=\sum_{\alpha\in B}b_{\alpha}X_{\alpha}, y=\sum_{\alpha\in B}c_{\alpha}X_{-\alpha}$。存在同态 $\varphi$

从$\mathfrak{s}\mathfrak{l}(2, k)$到$\mathfrak{g}$，这样$\varphi (H) =h^0, \varphi (X_+) =x, \varphi (X_-) =y$。

$a_{\alpha}$ 是整数 $\geq 1$ 的事实源于$(H_{\alpha})_{\alpha\in B}$ 是根系 $(H_{\alpha})_{\alpha\in B}$ 中的基（cf. 第 VI, §1, no. 5、注 5）。我们有：

$$
\alpha (h^0) = 2 \tag{1}
$$

对于所有$\alpha \in B$（第VI, §1, no. 10章，第29号提案的Cor.），所以

$$
[h^0, x] =\sum_{\alpha\in B}b_{\alpha}\alpha (h^0)X_{\alpha}= 2x \tag{2}
$$

$$
[h^0, y] =\sum_{\alpha\in B}c_{\alpha}(-\alpha (h^0))X_{-\alpha}=-2y \tag{3}
$$

另一方面，

$$
[x, y] =\sum_{\alpha ,\beta\in B}b_{\alpha}c_{\beta}[X_{\alpha}, X_{-\beta}] =\sum_{\alpha\in B}b_{\alpha}c_{\alpha}[X_{\alpha}, X_{-\alpha}] =-\sum_{\alpha\in B}a_{\alpha}H_{\alpha}=-h^0 \tag{4}
$$

因此存在同态$\varphi$。

#### 命题 12 {#lie-viii-s7-prop-12 .statement tag=0144}

设E是E上的有限维简单$\mathfrak{g}$模，$\omega$其最高权，以及E上$\mathfrak{g}$不变双线性形式的$\mathscr{B}$向量空间。令$m$为整数$\sum_{\alpha\in R_+}\omega (H_{\alpha})$，因而$m/2$为和 $\omega$ 相对于 B 的坐标（第 VI, §1, no. 10 章，Prop. 29 的 Cor.）。令 $w_0$ 为 W 的元素，使得 $w_0(B) =-B$。

(i) 如果$w_0(\omega )\not=-\omega$，则$\mathscr{B}= 0$。

(ii) 假设$w_0(\omega ) =-\omega$。那么 $\mathscr{B}$ 是维数 1，并且 $\mathscr{B}$ 的每个非零元素都是非简并的。如果 $m$ 是偶数（或奇数），则 $\mathscr{B}$ 的每个元素都是对称的（或交错的）。

a) 令$\Phi \in \mathscr{B}$。从E到$E^*$定义的映射$\varphi$，对于$x, y\in E$，通过$\varphi (x)(y) =$$\Phi (x, y)$是$\mathfrak{g}$模块的同态。如果$\Phi \not= 0$，则$\varphi \not= 0$，因此根据舒尔的引理，$\varphi$ 是同构，因而$\Phi$ 是非简并的。因而，$\mathfrak{g}$-模块E与$\mathfrak{g}$-模块$E^*$同构的，因而$w_0(\omega ) =-\omega$。由此我们证明了(i)。

b) 从现在开始假设$w_0(\omega)=-\omega$。则 E 同构于 $E^*$。 向量空间 $\mathscr B$ 同构于 $\operatorname{Hom}_{\mathfrak g}(E,E^*)$，因此也同构于 $\operatorname{Hom}_{\mathfrak g}(E,E)$，后者是维数 1（§6, no. 1，命题 1 (iii)）。因而$\dim \mathscr B=1$。 $\mathscr B$ 的每个非零元素 $\Phi$ 都不会被 a) 退化。将 $\Phi_1(x,y)=\Phi(y,x)$ 替换为 $x,y\in E$。由上可知，存在$\lambda\in k$，使得所有$x,y\in E$都有$\Phi_1(x,y)=\lambda\Phi(x,y)$。然后$\Phi(y,x)=\lambda\Phi(x,y)=\lambda^2\Phi(y,x)$，所以$\lambda^2=1$和$\lambda=\pm1$。因而，$\Phi$ 要么是对称的，要么是交错的。

c) 第 1 章如果 $\lambda+\mu\ne0$，则VII, §1, no. 3、第 9 (v) 条命题、$E^\lambda$ 和$E^\mu$ 相对于 $\Phi$ 正交。由于$\Phi$是非简并的，因而$E^\omega,E^{-\omega}$与$\Phi$不正交。

d) 存在从$\mathfrak{sl}(2,k)$到$\mathfrak g$的子代数的同态$\varphi$，需要$H$
$$
\sum_{\alpha\in R_+}H_\alpha
$$
（引理2）。通过这个同态将 E 视为一个 $\mathfrak{sl}(2,k)$ 模块。那么$E^\lambda$的元素就是权$\lambda\left(\sum_{\alpha\in R_+}H_\alpha\right)$。如果$\lambda\in P$满足$E^\lambda\ne0$和$\lambda\ne\omega,\lambda\ne-\omega$，则$-\omega<\lambda<\omega$，所以
$$
-m=-\omega\left(\sum_{\alpha\in R_+}H_\alpha\right)<\lambda\left(\sum_{\alpha\in R_+}H_\alpha\right)<\omega\left(\sum_{\alpha\in R_+}H_\alpha\right)=m.
$$
设G为$\mathfrak{sl}(2,k)$模E的型V$(m)$的同型分量。由上可知，G为长度1和包含$E^\omega,E^{-\omega}$。根据c)，$\Phi$到G的限制非零。通过§1, no. 3，注 3，$\pi$是偶数或奇数，因为限制是对称的或交错的。鉴于b)，这完成了证明。

#### 定义 2 {#lie-viii-s7-def-2 .statement tag=01J6}

如果 E 上存在非简并对称（或交错的）双线性形式在 $\rho$ 下不变，则 $\mathfrak g$ 的有限维不可约表示 $\rho$ 被称为正交（或辛）。

### 6.表示环

令 $\mathfrak a$ 为有限维李代数。令$\mathscr F_{\mathfrak a}$（或$\mathscr G_{\mathfrak a}$）为有限维（或有限维简单）$\mathfrak a$-模的类的集合。让 $\mathscr R(\mathfrak a)$ 成为免费的阿贝尔的群 $\mathbf Z^{(\mathscr G_{\mathfrak a})}$。对于任何有限维简单 $\mathfrak a$-模 E，用 $[E]$ 表示其类。设 F 为有限维 $\mathfrak a$ 模；让
$$
(F_n,F_{n-1},\ldots,F_0)
$$
成为 F 的 Jordan-Hölder 级数； 元素
$$
\sum_{i=1}^{n}[F_i/F_{i-1}]
$$
$\mathscr R(\mathfrak a)$ 仅取决于 F，而不取决于 Jordan-Hölder 级数的选择；我们用$[F]$表示。如果
$$
0\longrightarrow F'\longrightarrow F\longrightarrow F''\longrightarrow0
$$
是有限维$\mathfrak a$模的正合序列，则$[F]=[F']+[F'']$。

设 F 为有限维半单 $\mathfrak{a}$ 模；对于所有$E\in \mathfrak{S}_{\mathfrak{a}}$，令$n_E$为型E的F同型成分的长度；那么 [F] = $\sum_{E\in\mathfrak{S}_{\mathfrak{a}}}n_E.E$。如果 $F,F'$ 是有限维半单 $\mathfrak{a}$ 模，并且如果 [F] = $[F']$，则 F 和 $F'$ 同构的。

#### 引理 3 {#lie-viii-s7-lem-3 .statement tag=0145}

设G为阿贝尔的群相加，且$\varphi :\mathscr{F}_{\mathfrak{a}}\rightarrow G$映射；通过滥用记号，我们用任何有限维$\mathfrak{a}$模F的类的$\varphi$下的$\varphi (F)$像表示。假设，对于任何正合序列

$$
0\longrightarrow F'\longrightarrow F\longrightarrow F''\longrightarrow 0
$$

有限维 $\mathfrak{a}$ 模块，我们有 $\varphi (F) =\varphi (F') +\varphi (F'')$。那么，对于每个有限维 $\mathfrak{a}$-模 F，存在唯一同态 $\theta :\mathscr{R}(\mathfrak{a})\rightarrow G$，使得$\theta ([F]) =\varphi (F)$。

从$\mathscr{R}(\mathfrak{a})$到G存在唯一同态$\theta$，使得对于每个有限维简单$\mathfrak{a}$-模E有$\theta ([E]) =\varphi (E)$。设F是有限维$\mathfrak{a}$-模，并且$(F_n,F_{n-1}, . . . ,F_0)$是F的Jordan-Hölder级数；如果$n >0$，我们有，到$n$的归纳，

$$
\theta ([F]) =\sum_{i=1}^n\theta ([F_i/F_{i-1}]) =\sum_{i=1}^n\varphi (F_i/F_{i-1}) =\varphi (F)
$$

如果 $n= 0$ 则 [F] = 0 所以$\theta ([F]) = 0$；另一方面，通过考虑正合序列$0\longrightarrow 0\longrightarrow 0\longrightarrow 0\longrightarrow 0$，我们看到$\varphi (0) = 0$。

#### 例 {#lie-viii-s7-n6-exa-1 .statement tag=0146}

取$G =\mathbf{Z}$和$\varphi (F) =$dim F。从$\mathscr{R}(\mathfrak{a})$到$\mathbf{Z}$的相应的同态用dim表示。令$c$为维数1的平凡$\mathfrak{a}$模的类，并令$\psi$为从$\mathbf{Z}$到$\mathscr{R}(\mathfrak{a})$的同态$n \rightarrow nc$。就是直接的

暗淡$\circ \psi =$ ID$_{\mathbf{Z}}$，

这样$\mathscr{R}(\mathfrak{a})$就是Ker dim和$\mathbf{Z}c$的直和。

#### 引理 4 {#lie-viii-s7-lem-4 .statement tag=0147}

在加法群$\mathscr{R}(\mathfrak{a})$上存在加法上唯一的乘法分配性，使得$[E][F] = [E\otimes F]$对于所有有限维$\mathfrak{a}$-模E、F。这样，$\mathscr{R}(\mathfrak{a})$被赋予交换环的结构。 维数 1 的平凡$\mathfrak{a}$模的类是这个环的单位元。

唯一性很清楚。 $\mathscr{R}(\mathfrak{a}) =\mathbf{Z}^{(\mathfrak{S}_{\mathfrak{a}})}$ 上存在可交换的乘法，它在加法上可分配，因此 $[E][F] = [E\otimes F]$ 对于所有 $E,F\in \mathfrak{S}_{\mathfrak{a}}$。令$E_1,E_2$为有限维$\mathfrak{a}$模，$l_1$和$l_2$为它们的长度；我们在$l_1+l_2$上通过归纳显示$[E_1][E_2] = [E_1\otimes E_2]$。如果$l_1+l_2\leq 2$，这很清楚。另一方面，令$F_1$为$E_1$的子模，与0和$E_1$不同。然后

$[F_1][E_2] = [F_1\otimes E_2]$ 和$[E_1/F_1][E_2] = [(E_1/F_1)\otimes E_2]$ 归纳假设。另一方面，$(E_1\otimes E_2)/(F_1\otimes E_2)$与$(E_1/F_1)\otimes E_2$同构的。因此

$$
[E_1][E_2] = ([E_1/F_1] + [F_1]).[E_2] = [(E_1/F_1)\otimes E_2] + [F_1\otimes E_2] = [E_1\otimes E_2]
$$

这证明了我们的断言。紧接着，上面定义的乘法是结合律，因此$\mathscr{R}(\mathfrak{a})$有结构或交换环。最后，很明显，维数 1 的平凡$\mathfrak{a}$模的类是这个环的单位元。

#### 引理 5 {#lie-viii-s7-lem-5 .statement tag=0148}

存在环$\mathscr{R}(\mathfrak{a})$的唯一对合自同构$X \rightarrow X^*$，使得$[E]^*= [E^*]$对于每个有限维$\mathfrak{a}$-模E。

唯一性很清楚。到引理 3 时，存在从加法群 $\mathscr{R}(\mathfrak{a})$ 到自身的同态 $X \rightarrow X^*$，使得对于每个有限维 $\mathfrak{a}$-模 E 都有 $[E]^*= [E^*]$。我们有 $(X^*)^*= X$，所以这个同态是内合的。它是环 $\mathscr{R}(\mathfrak{a})$ 的自同构，因为对于所有有限维 $\mathfrak{a}$ 模 E 和 F，$(E\otimes F)^*$ 与 $E^*\otimes F^*$ 同构的。

令$U(\mathfrak{a})$为$\mathfrak{a}, U(\mathfrak{a})^*$向量空间对偶$U(\mathfrak{a})$的包络代数。回想一下（第II, §1, no. 5章）$U(\mathfrak{a})$定义在$U(\mathfrak{a})^*$上的余代数结构是可交换的、结合的代数结构与单位元。对于任何有限维$\mathfrak{a}$-模E，从$U(\mathfrak{a})$到$k$的映射$u \rightarrow$Tr($u_E$)是$U(\mathfrak{a})^*$的元素$\tau_E$。如果$0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0$是有限维$\mathfrak{a}$模的正合序列，则$\tau_E=\tau_{E'}+\tau_{E''}$。因而，通过引理 3，存在唯一同态，我们用Tr表示，从加法群$\mathscr{R}(\mathfrak{a})$到群$U(\mathfrak{a})^*$，使得对于每个有限维$\mathfrak{a}$-模E，Tr[E]$=\tau_E$。如果$k$表示维数 1 的平凡 $\mathfrak{a}$ 模，很容易检查 Tr[$k]$ 是 $U(\mathfrak{a})^*$ 的单位元。最后，令 E 和 F 为有限维 $\mathfrak{a}$ 模。令$u\in U(\mathfrak{a})$且$c$为余积除以$U(\mathfrak{a})$。通过U模块$E\otimes F$（第I, §3, no. 2章）的定义，如果$c(u) =\sum_iu_i\otimes u'_i$，

$$
u_{E\otimes F}=\sum_i(u_i)_E\otimes (u'_i)_F
$$

因而

$\tau_{E\otimes F}(u) =\sum_i$Tr($u_i$)$_E$Tr($u'_i$)$_F=\sum_i\tau_E(u_i)\tau_F(u'_i)$

$$
= (\tau_E\otimes \tau_F)(c(u))
$$

这意味着$\tau_E\tau_F=\tau_{E\otimes F}$。因而，Tr$:\mathscr{R}(\mathfrak{a})\rightarrow U(\mathfrak{a})^*$ 是环中的同态。

令$\mathfrak{a}_1$和$\mathfrak{a}_2$为李代数，从$\mathfrak{a}_1$到$\mathfrak{a}_2$为$f$同态。每个有限维$\mathfrak{a}_2$模E定义通过$f$和$\mathfrak{a}_1$模，因此$\mathscr{R}(\mathfrak{a}_2)$和$\mathscr{R}(\mathfrak{a}_1)$的元素我们暂时用$[E]_2$和$[E]_1$表示。通过引理 3，存在唯一同态，用$\mathscr{R}(f)$表示，从群$\mathscr{R}(\mathfrak{a}_2)$到群$\mathscr{R}(\mathfrak{a}_1)$，使得$\mathscr{R}(f)[E]_2=[E]_1$对于每个有限维$\mathfrak{a}_2$-模E。此外，$\mathscr{R}(f)$是同态 / 环。如果 U(f) 是从 U($\mathfrak{a}_1$) 到 U($\mathfrak{a}_2$) 延伸 $f$ 的同态，则以下图表是可交换的

$$
\begin{array}{ccc}
\mathscr{R}(\mathfrak{a}_2) & \xrightarrow{\mathscr{R}(f)} & \mathscr{R}(\mathfrak{a}_1)\\
\Big\downarrow\scriptstyle{\operatorname{Tr}} & & \Big\downarrow\scriptstyle{\operatorname{Tr}}\\
U(\mathfrak{a}_2)^* & \xrightarrow{t_{U(f)}} & U(\mathfrak{a}_1)^*.
\end{array}
$$

接下来我们将 $\mathfrak{a}$ 视为可分割的半单李代数 $\mathfrak{g}$。 环$\mathscr{R}(\mathfrak{g})$称为$\mathfrak{g}$的*表示环*。对于所有$\lambda\in P_{++}$，我们用最高权$\lambda$的简单$\mathfrak{g}$模块E($\lambda$)的$[\lambda]$类表示。

### 7. 特征标 $\mathfrak{g}$-模块

令 $\Delta$ 为可加写成的可交换幺半群，且幺半群 $\Delta$ 的 $\mathbf{Z}[\Delta]=\mathbf{Z}^{(\Delta)}$ 代数在 $\mathbf{Z}$ 上（代数，第 III, §2, no. 6 章）。用$\mathbf{Z}[\Delta]$的$(e^\lambda)_{\lambda\in\Delta}$典范基表示。对于所有 $\lambda,\mu\in\Delta$，我们有 $e^{\lambda+\mu}=e^\lambda e^\mu$。如果0是$\Delta$的中性元素，那么$e^0$就是$\mathbf{Z}[\Delta]$的单位元；用1表示。

令 E 为域 $\kappa$ 的 $\Delta$ 分级向量空间，并令 $(E^\lambda)_{\lambda\in\Delta}$ 为其分级。如果每个$E^\lambda$都是有限维的，则E的*特征标*（用ch(E)表示）是$\mathbf{Z}^{\Delta}$的元素$(\dim E^\lambda)_{\lambda\in\Delta}$。如果 E 本身是有限维的，

$$
\operatorname{ch}(E)=\sum_{\lambda\in\Delta}(\dim E^\lambda)e^\lambda\in\mathbf{Z}[\Delta].
\tag{5}
$$

令 E′、E、E″ 为 $\Delta$ 分级向量空间，使得 E′${}^\lambda$、E${}^\lambda$、E″${}^\lambda$ 为 $\kappa$ 上的有限维，并且 $0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow0$ 正合序列的分级同态次数 0. 就是直接的

$$
\operatorname{ch}(E)=\operatorname{ch}(E')+\operatorname{ch}(E'').
\tag{6}
$$

特别是，如果 F$_1$、F$_2$ 是 $\Delta$ 分级向量空间，使得 F$_1^\lambda$ 和 F$_2^\lambda$ 是 $\kappa$ 上的有限维，则

$$
\operatorname{ch}(F_1\oplus F_2)=\operatorname{ch}(F_1)+\operatorname{ch}(F_2).
\tag{7}
$$

如果 F$_1$ 和 F$_2$ 是有限维的，我们也有

$$
\operatorname{ch}(F_1\otimes F_2)=\operatorname{ch}(F_1)\mathbin{.}\operatorname{ch}(F_2).
\tag{8}
$$

#### 例 {#lie-viii-s7-n7-exa-1 .statement tag=01JX}

假设$\Delta=\mathbf{N}$。设 T 为不定式。从代数$\mathbf{Z}[\mathbf{N}]$到代数$\mathbf{Z}[T]$存在一个唯一的同构，对于所有$n\in\mathbf{N}$需要$e^n$到$T^n$。对于任何有限维 $\mathbf{N}$ 分级向量空间 E，$\mathbf{Z}[T]$ 中 ch(E) 的像是 E 的庞加莱多项式（第 V, §5, no. 1 章）。

设 E 是一个 $\mathfrak{g}$ 模，使得 $E =\sum_{\lambda\in\mathfrak{h}^*}E^{\lambda}$ 且每个 $E^{\lambda}$ 是

有限维。我们知道$(E^{\lambda})_{\lambda\in\mathfrak{h}^*}$是向量空间E的分级。接下来我们将为E的特征标保留记号ch(E)，被视为$\mathfrak{h}^*$分级的向量空间。因此，特征标 ch(E) 是$\mathbf{Z}^{\mathfrak{h}^*}$ 的元素。如果 E 是有限维的，则 ch(E) $\in \mathbf{Z}[P]$。通过公式 (6) 和 no. 6 的引理 3，对于任何有限维 $\mathfrak{g}$-模 E，存在从群 $\mathscr{R}(\mathfrak{g})$ 到 $\mathbf{Z}[P]$ 的唯一同态，将 E 带到 ch(E)；这个同态将由ch表示。 关系(8)表明ch是从环$\mathscr{R}(\mathfrak{g})$到环$\mathbf{Z}[P]$的同态。

#### 注 {#lie-viii-s7-n7-rem-1 .statement tag=0149}

P 定义的每个元素都是维数1的简单$\mathfrak{h}$模，因此同态从群$\mathbf{Z}[P]$到群$\mathscr{R}(\mathfrak{h})$，即环的单同态。复合的就是直接的

$$
\mathscr{R}(\mathfrak{g})\longrightarrow \mathbf{Z}[P]\longrightarrow \mathscr{R}(\mathfrak{h})
$$

同态由$\mathfrak{h}$ 的典范嵌入定义为$\mathfrak{g}$ (no. 6)。

Weyl 群 W 在群 P 上按自同构运行，因此在 $\mathbf{Z}^P$ 上运行。对于所有$\lambda \in P$和所有$w\in W$，我们有$we^{\lambda}=e^{w\lambda}$。令 $\mathbf{Z}[P]^W$ 为 $\mathbf{Z}[P]$ 由……组成的子环元素在 W 下不变。

#### 引理 6 {#lie-viii-s7-lem-6 .statement tag=014A}

如果 $\lambda \in P_{++}$，则 ch[$\lambda ]\in \mathbf{Z}[P]^W$。 ch[$\lambda ]$（第 VI, §3, no. 2，定义 1）的唯一最大值项是 $e^{\lambda}$。

第一个断言源自 no. 1，Cor。提案 2 中的第 2 条，以及提案 1 (ii) §6, no. 1 中的第二条。

#### 定理 2 {#lie-viii-s7-thm-2 .statement tag=014B}

(i) 令 $(\varpi_{\alpha})_{\alpha\in B}$ 为基本权相对于 B 的族。令 $(T_{\alpha})_{\alpha\in B}$ 为不定族。从$\mathbf{Z}[(T_{\alpha})_{\alpha\in B}]$到$\mathscr{R}(\mathfrak{g})$的映射$f \rightarrow f(([\varpi_{\alpha}])_{\alpha\in B})$是环的同构。

(ii) 同态从$\mathscr{R}(\mathfrak{g})$到$\mathbf{Z}[P]$诱导同构从环$\mathscr{R}(\mathfrak{g})$到环$\mathbf{Z}[P]^W$。

(iii) 令 E 为有限维 $\mathfrak{g}$ 模。如果 ch $E =\sum_{\lambda\in P_{++}}m_{\lambda}$ch[$\lambda ]$，最高权 $\lambda$ 的 E 的同型成分有长度 $m_{\lambda}$。

家族$([\lambda ])_{\lambda\in P_{++}}$是$\mathbf{Z}$模块$\mathscr{R}(\mathfrak{g})$的基，家族(ch[$\lambda ]$)$_{\lambda\in P_{++}}$是$\mathbf{Z}$模块$\mathbf{Z}[P]^W$的基（引理6，以及第1章）。 VI, §3, no. 4，提案 3）。这就证明了(ii)和(iii)。 断言 (i) 源自 (ii)、引理 6 和第 1 章。 VI, §3, no. 4，周四。 1.

#### 推论{#lie-viii-s7-n7-cor-1 .statement tag=014C}

令$E,E'$为有限维$\mathfrak{g}$模。那么 E 同构于 $E'$ 当且仅当 ch E = ch $E'$。

这是从 Th 得出的。 2 (ii) 并且$E,E'$ 是半单。

### 习题 {#lie-viii-s7-exercises}

考虑的所有 $\mathfrak{g}$ 模块（练习 14 和 15 中的模块除外）均假设为有限维。

§ 7](exercises/s7/)参见[习题。
