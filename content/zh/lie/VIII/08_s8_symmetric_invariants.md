---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 8
section_title: Symmetric invariants
lang: zh
source: lie-vii-ix
book_pages: 141-151, 250-253
pdf_pages: 0149-0159, 0258-0261
extraction: native+ocr
subsections:
    - "no": 1
      title: EXPONENTIAL OF A LINEAR FORM
      page: 141
      pdf_page: 149
    - "no": 2
      title: INJECTION OF $\boldsymbol{k}$[P] INTO S($\mathfrak{h}$)$^*$
      page: 142
      pdf_page: 150
    - "no": 3
      title: INVARIANT POLYNOMIAL FUNCTIONS
      page: 143
      pdf_page: 151
    - "no": 4
      title: PROPERTIES OF Aut0
      page: 148
      pdf_page: 156
    - "no": 5
      title: CENTRE OF THE ENVELOPING ALGEBRA
      page: 148
      pdf_page: 156
statements: 24
exercises: 18
content_sha256: 9e779ae659dad594f2cd4d1f35309a78b10ef04f2a11d69b21d5c99a38ccccac
translated_from: content/en/lie/VIII/08_s8_symmetric_invariants.md
translation_method: google
source_content_sha256: 732d0bf5cbdb060a54cdf12410d56095982532b83bb7ad565c69e521edffa36a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 8cfff6a381a1afb1894a0a516c40f7644ddbc139025b4cbf6a68b50579438fe0
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 8。 对称不变量

在本段中，我们用 $(\mathfrak{g},\mathfrak{h})$ 分裂的半单李代数表示，用 R 表示根系，用 W 表示 Weyl 群，用 P 表示权的群。

### 1. 线性形式的指数

令V为有限维向量空间，$\mathbf{S}(V)$其对称代数。 $\mathbf{S}(V)$ 定义在 $\mathbf{S}(V)^*$ 上的余代数结构代数结构（代数，第 III, §11，第 579 至 582 页）。 向量空间 $\mathbf{S}(V)^*$ 可以与 $\prod_{m\geq 0}\mathbf{S}^m(V)^*$ 规范地识别，$\mathbf{S}^m(V)^*$ 可以

可以用V上对称$m$线性形式的空间进行规范地识别。 $V^*=\mathbf{S}^1(V)^*$的典范嵌入从代数$\mathbf{S}(V^*)$到代数$\mathbf{S}(V)^*$进入$\mathbf{S}(V)^*$定义单同态，其中像是$\mathbf{S}(V)^{*gr}=\sum_{m\geq 0}\mathbf{S}^m(V)^*($代数， III, §11, no. 5，提案 8）。我们认同

代数$\mathbf{S}(V^*)$和$\mathbf{S}(V)^{*gr}$通过这个同态；我们还在V上进行了认同$\mathbf{S}(V^*)$和代数或多项式函数（第VII章，附录I，no. 1）。

元素 $(u_m)\in \prod_{m\geq 0}\mathbf{S}^m(V)^*$ 使得 $u_0= 0$ 形式的理想 J

$\mathbf{S}(V)^*$；我们给$\mathbf{S}(V)^*$ J-adic 拓扑（交换代数，第III, §2, no. 5章），其中$\mathbf{S}(V)^*$是完备的，而$\mathbf{S}(V^*)$在$\mathbf{S}(V)^*$中是稠密的。如果$(e^*_i)_{1\leq i\leq n}$是$V^*$的基，并且如果$T_1, . . . ,T_n$不确定，则从$k[T_1, . . . ,T_n]$到$\mathbf{S}(V^*)$需要$T_i$到$e^*_i(1\leq i\leq n)$的同态是代数的同构，并且扩展从代数$k[[T_1, . . . ,T_n]]$到代数$\mathbf{S}(V)^*$连续同构。

为了所有$\lambda \in V^*$，为了家人$\lambda^n/n$！可在 $\mathbf{S}(V)^*$ 中求和。它的和称为$\lambda$的指数，记为exp($\lambda$)（符合II, §6, no. 1章节）。设 $x_1, . . . , x_n\in V$；我们有

$\langle$exp $\lambda , x_1. . . x_n\rangle =n1$！$\langle \lambda^n, x_1. . . x_n\rangle =\langle \lambda , x_1\rangle . . .\langle \lambda , x_n\rangle$

作者：代数，第 1 章III, §11, no. 5、公式 (29)。紧接着，exp($\lambda$)是唯一同态，从代数$\mathbf{S}(V)$到$k$即扩展$\lambda$。

对于所有$\lambda , \mu\in V^*$（第II, §6, no. 1、注），我们有exp($\lambda +\mu$) $=$ exp($\lambda$) exp($\mu$)。 Thus, the map exp$: V^*\rightarrow \mathbf{S}(V)^*$ is a homomorphism from the additive group $V^*$ to the multiplicative group of invertible elements of $\mathbf{S}(V)^*$. 族 (exp $\lambda$ )$_{\lambda\in V^*}$ 是第向量空间 $\mathbf{S}(V)^*($代数中的一个自由家庭。 V, §7, no. 3，Th。 1）。

#### 引理 1 {#lie-viii-s8-lem-1 .statement tag=0154}

令$\Pi$为$V^*$的子群，生成向量空间$V^*$，以及$m$整数$\geq 0$。然后 pr$_m$(exp $\Pi$ ) 生成向量空间 $\mathbf{S}^m(V^*)$。

代数，第 1 章I, §8, no. 2，第 2 条，$V^*$ 的 $m$ 元素中的任意乘积是形式 $x^m$ 的元素的 $k$ 线性组合，其中 $x\in \Pi$。但是$x^m=m$！ pr$_m$(exp $x$)。 Q.E.D.

截至结构迁移、V定义自同构、代数$\mathbf{S}(V)$及$\mathbf{S}(V)^*$每自同构；这给出了$\mathbf{S}(V)$和$\mathbf{S}(V)^*$上的$\mathbf{G}\mathbf{L}(V)$的线性表示。

### 2. 单射 OF $\boldsymbol{k}$[P] 进入 S($\mathfrak{h}$)$^*$

从P到$\mathbf{S}(\mathfrak{h})^*$的映射$p \rightarrow$exp$p$是同态从加法群P到$\mathbf{S}(\mathfrak{h})^*$配备了乘法结构（no. 1）。因而，存在从幺半群 P 的代数 $k[P]$ 到代数 $\mathbf{S}(\mathfrak{h})^*$ 的唯一同态 $\psi$，使得

$\psi (e^{\lambda}) =$exp($\lambda$)$(\lambda \in P)$

（在§7, no. 7中的记号）。按不。 $1,\psi$ 是单射的。截至结构的迁移，所有 $\lambda \in P$ 和所有 $w\in W$ 为 $\psi (w(e^{\lambda})) =w(\psi (e^{\lambda}))$。因而，如果$k[P]^W$（或$\mathbf{S}(\mathfrak{h})^{*W}$）表示$k[P]$（或$\mathbf{S}(\mathfrak{h})^*$）的元素或集合在W下不变，我们有$\psi (k[P]^W)\subset \mathbf{S}(\mathfrak{h})^{*W}$。

#### 命题 1 {#lie-viii-s8-prop-1 .statement tag=0155}

令$S^m(\mathfrak{h}^*)^W$为W下$S^m(\mathfrak{h}^*)$的元素的集合不变。则pr$_m(\psi (k[P]^W)) =\mathbf{S}^m(\mathfrak{h}^*)^W$。

由上可知，pr$_m(\psi (k[P]^W))\subset \mathbf{S}^m(\mathfrak{h}^*)^W$。 $\mathbf{S}^m(\mathfrak{h}^*)$ 的每个元素都是元素形式的 $k$ 线性组合

pr$_m$(exp $\lambda$)$=$(pr$_m\circ \psi$)$(e^{\lambda})$

其中 $\lambda \in P$ (引理 1)。因而$\mathbf{S}^m(\mathfrak{h}^*)^W$的每个元素都是形式的元素的线性组合

$\sum_{w\in W}w$((pr$_m\circ \psi$)$(e^{\lambda})$)$=$(pr$_m\circ \psi$)$(\sum_{w\in W}w(e^{\lambda}))$,

其中每个属于到pr$_m(\psi (k[P]^W))$。

#### 命题 2 {#lie-viii-s8-prop-2 .statement tag=0156}

令 E 为有限维 $\mathfrak{g}$ 模。令$U(\mathfrak{h}) =\mathbf{S}(\mathfrak{h})$为$\mathfrak{h}$的包络代数。如果$u\in U(\mathfrak{h})$，那么

Tr($u_E$)$=\langle \psi$(ch $E$)$, u\rangle$。

将$u=h_1. . . h_m$与$h_1, . . . , h_m\in \mathfrak{h}$处理即可。对于所有$\lambda \in P$，让$d_{\lambda}=$变暗$E^{\lambda}$。然后 ch $E =\sum_{\lambda}d_{\lambda}e^{\lambda}$，所以 $\psi$(ch $E$) $=\sum_{\lambda}d_{\lambda}$ exp($\lambda$ ) 因而

$$
\langle \psi(\mathrm{ch}\,E),u\rangle
 = \sum_{\lambda} d_\lambda\langle\exp\lambda,h_1\ldots h_m\rangle
$$
$$
= \sum_{\lambda} d_\lambda\lambda(h_1)\ldots\lambda(h_m)\qquad\text{(no. 1)}
$$
$$
= \mathrm{Tr}\,u_E.
$$

#### 推论 1 {#lie-viii-s8-prop-2-cor-1 .statement tag=01J7}

— 令 $\mathrm{U}(\mathfrak g)$ 为 $\mathfrak g$ 的包络代数。让同态
$$
\zeta:\mathrm{U}(\mathfrak g)^*\longrightarrow\mathrm{U}(\mathfrak h)^*=\mathrm{S}(\mathfrak h)^*
$$
是典范嵌入中的转置
$$
\mathrm{U}(\mathfrak h)\longrightarrow\mathrm{U}(\mathfrak g).
$$
以下图表通勤
$$
\begin{array}{ccccc}
\mathscr{R}(\mathfrak g)&\xrightarrow{\mathrm{ch}}&\mathbf{Z}[P]\\
\Big\downarrow{\scriptstyle\mathrm{Tr}}&&\Big\downarrow{\scriptstyle\psi}\\
\mathrm{U}(\mathfrak g)^*&\xrightarrow{\zeta}&\mathrm{S}(\mathfrak h)^*
\end{array}
$$

这只是提案 2 的重新表述。

#### 推论 2 {#lie-viii-s8-prop-2-cor-2 .statement tag=01J8}

— 设 $m$ 为整数 $\geqslant 0$。 $\mathrm{S}^m(\mathfrak h^*)^W$的每个元素都是形式$x\mapsto\mathrm{Tr}(\rho(x)^m)$的$\mathfrak h$上多项式函数的线性组合，其中$\rho$是$\mathfrak g$的有限维线性表示。

根据第 1 号提案，$\mathrm{S}^m(\mathfrak h^*)^W=(\mathrm{pr}_m\circ\psi)(k[P]^W)$。现在$\mathbf{Z}[P]^W=\mathrm{ch}\,\mathscr{R}(\mathfrak g)$（§7, no. 7，Th.2（ii））。因而，由章。 VI, §3, no. 4、引理 3、$\psi(k[P]^W)$ 是$\psi(\mathrm{ch}\,\mathscr{R}(\mathfrak g))=\zeta(\mathrm{Tr}\,\mathscr{R}(\mathfrak g))$ 生成的$\mathrm{S}(\mathfrak h)^*$ 的$k$-向量子空间。因而，$\mathrm{S}^m(\mathfrak h^*)^W$是由$(\mathrm{pr}_m\circ\zeta\circ\mathrm{Tr})(\mathscr{R}(\mathfrak g))$生成的$\mathrm{S}^m(\mathfrak h^*)$的向量子空间。但是，如果 $\rho$ 是 $\mathfrak g$ 的有限维线性表示，

$$
((\mathrm{pr}_m\circ\zeta\circ\mathrm{Tr})(\rho))(x)
=\left\langle(\zeta\circ\mathrm{Tr})(\rho),\frac{x^m}{m!}\right\rangle
=\frac{1}{m!}\mathrm{Tr}(\rho(x)^m)
$$

对于所有$x\in\mathfrak h$。

### 3. 不变多项式函数

令 $\mathfrak a$ 为有限维李代数。按照no. 1的约定，我们在$\mathfrak a$上进行认同代数$\mathrm{S}(\mathfrak a^*)$、代数$\mathrm{S}(\mathfrak a)^{*gr}$、多项式函数的代数。对于所有$a\in\mathfrak a$，令$\theta(a)$为$\mathrm{S}(\mathfrak a)$的推导，使得$\theta(a)x=[a,x]$对于所有$x\in\mathfrak a$。我们知道（第I, §3, no. 2章）$\theta$是$\mathrm{S}(\mathfrak a)$上$\mathfrak a$的表示。设$\theta^*(\mathfrak a)$为${}^t\theta(a)$到$\mathrm{S}(\mathfrak a^*)$中的限制。那么$\theta^*$就是$\mathfrak a$的表示。如果$f\in\mathrm{S}^n(\mathfrak a^*)$，则$\theta^*(a)f\in\mathrm{S}^n(\mathfrak a^*)$，对于$x_1,\ldots,x_n\in\mathfrak a$，

$$
(\theta^*(a)f)(x_1,\ldots,x_n)
=-\sum_{1\leqslant i\leqslant n}
f(x_1,\ldots,x_{i-1},[a,x_i],x_{i+1},\ldots,x_n).
\tag{1}
$$

从(1)我们很容易推断出$\theta^*(a)$是$\mathbf{S}(\mathfrak{a}^*)$的推导。 $\mathbf{S}(\mathfrak{a})$（或$\mathbf{S}(\mathfrak{a}^*)$）的元素在$\mathfrak{a}$的表示$\theta$（或$\theta^*$）下保持不变，称为$\mathbf{S}(\mathfrak{a})$（或$\mathbf{S}(\mathfrak{a}^*)$）的不变量元素。

#### 引理 2 {#lie-viii-s8-lem-2 .statement tag=0157}

令$\rho$为$\mathfrak{a}$的有限维线性表示，以及$m$整数$\geq 0$。 $\mathfrak{a}$ 上的函数 $x \rightarrow$ Tr($\rho (x)^m$) 是不变量多项式函数。

将 $g(x_1, . . . , x_m) =$ Tr($\rho (x_1). . . \rho (x_m)$) 替换为 $x_1, . . . , x_m\in \mathfrak{a}$。如果$x\in \mathfrak{a}$，我们有

$$
-(\theta^*(x)g)(x_1, . . . , x_m)
$$

$=\sum_{1\leq i\leq m}$Tr($\rho (x_1). . . \rho (x_{i-1})[\rho (x), \rho (x_i)]\rho (x_{i+1}). . . \rho (x_m)$)

= Tr($\rho (x)\rho (x_1). . . \rho (x_m)$)$-$ Tr($\rho (x_1). . . \rho (x_m)\rho (x)$)$= 0$,

所以$\theta^*(x)g= 0$。令 $h$ 为由下式定义的对称多重线性形式

$h(x_1, . . . , x_m) =m1$！ $\sum g(x_{\sigma(1)}, . . . , x_{\sigma(m)})$。

$\sigma \in \mathfrak{S}_m$

对于所有$x\in \mathfrak{a}$，我们有$\theta^*(x)h= 0$和Tr($\rho (x)^m$)$=h(x, . . . , x)$，因此有引理。

#### 引理 3 {#lie-viii-s8-lem-3 .statement tag=0158}

令 E 为有限维 $\mathfrak{g}$ 模，且为 $x\in E$。那么$x$是$\mathfrak{g}$模块E的不变量元素当且仅当对于$\mathfrak{g}$的每个幂零元$a$有(exp $a_E$)$.x=x$。

条件显然是必要的。假设现在已经满足了。设$a$为$\mathfrak{g}$的幂零元。存在整数$n$使得$a^n_E= 0$。对于所有$t\in k$，我们有

0 = exp($ta_E$)$.x-x=ta_Ex+$ 2!$1t^2a^2_Ex+\cdots +(n-1$ 1)! $t^{n-1}a^{n-1}_Ex$,

所以$a_Ex= 0$。但李代数$\mathfrak{g}$是由它的幂零元生成的（§4, no. 1，命题1）。因此 $x$ 是 $\mathfrak{g}$ 模 E 的不变量元素。

对于任何$\xi \in \mathbf{G}\mathbf{L}(\mathfrak{g})$，令$\mathbf{S}(\xi )$为$\mathbf{S}(\mathfrak{g})$的自同构，扩展$\xi$，以及$\mathbf{S}^*(\xi )$限制到$\mathbf{S}(\xi )$的同余自同构的$\mathbf{S}(\mathfrak{g}^*)$。那么$\mathbf{S}$和$\mathbf{S}^*$就是$\mathbf{G}\mathbf{L}(\mathfrak{g})$的表示。如果$a$是$\mathfrak{g},\theta (a)$的幂零元在$\mathbf{S}(\mathfrak{g})$和$\mathbf{S}$(exp ad$a$)$=$exp$\theta (a)$上局部幂幂，所以

$\mathbf{S}^*$（exp广告$a$）$=$exp$\theta^*(a)$。 (2)

#### 命题 3 {#lie-viii-s8-prop-3 .statement tag=0159}

令$f$在$\mathfrak{g}$上为多项式函数。以下条件是等效的：

(i) $f\circ s=f$ 对于所有 $s\in$ Aut$_e(\mathfrak{g})$；

(ii) $f\circ s=f$ 对于所有 $s\in$ Aut$_0(\mathfrak{g})$；

(iii) $f$ 是不变的。

(i) 和 (iii) 的等价由公式 (2) 和引理 3 得出。由此得出，(iii) 通过基域的扩张蕴含 (ii)。 (ii) $=\Rightarrow$ (i) 的含义是明确的。

注仔细观察，如果$f$ 满足$3,f$ 的条件，则在 Aut($\mathfrak{g}$) 下一般不不变（练习 1 和 2）。

#### 定理 1 {#lie-viii-s8-thm-1 .statement tag=015A}

令$I(\mathfrak{g}^*)$为$\mathfrak{g}$上不变多项式函数的代数。设$i:\mathbf{S}(\mathfrak{g}^*)\rightarrow \mathbf{S}(\mathfrak{h}^*)$为限制同态。

(i) 映射$i|I(\mathfrak{g}^*)$是从代数$I(\mathfrak{g}^*)$到代数$\mathbf{S}(\mathfrak{h}^*)^W$的同构。

(ii) 对于任何整数$n\geq 0$，令$I^n(\mathfrak{g}^*)$为次数$n$的$I(\mathfrak{g}^*)$的齐次元素的集合。那么$I^n(\mathfrak{g}^*)$是形式$x \rightarrow$Tr($\rho (x)^n$)的$\mathfrak{g}$上函数的线性组合集合，其中$\rho$是$\mathfrak{g}$的有限维线性表示。

(iii) 设 $l=$ rk($\mathfrak{g}$)。 $I(\mathfrak{g}^*)$存在$l$代数独立齐次元素即生成代数$I(\mathfrak{g}^*)$。

a) 设$f\in I(\mathfrak{g}^*)$和$w\in W$。存在 $s\in$ Aut$_e(\mathfrak{g},\mathfrak{h})$ 使得$s|\mathfrak{h}=w($§2, no. 2，Cor。的 Th。 2）。由于$f$在$s$下是不变的（命题$3$）$,i(f)$在$w$下是不变的。因此$i(I(\mathfrak{g}^*))\subset \mathbf{S}(\mathfrak{h}^*)^W$。

b) 我们证明，如果$f\in I(\mathfrak{g}^*)$ 满足$i(f) = 0$，则$f= 0$。如有必要，扩展基域，我们可以假设$k$是代数封闭的。根据提案，对于所有 $s\in$ Aut$_e(\mathfrak{g})$，$3,f$ 在 $s(\mathfrak{h})$ 上消失。因此，$f$在$\mathfrak{g}$的每个嘉当子代数（第VII, §3, no. 2，第1章）消失，特别是在$\mathfrak{g}$的正则元素的集合。但是对于 Zariski 拓扑（第 VII, §2, no. 2 章）来说，这个集合密集于 $\mathfrak{g}$。

c) 设$n$为整数$\geq 0$。令$L^n$为$\mathfrak{g}$上形式$x \rightarrow$函数线性组合集合Tr($\rho (x)^n$)，其中$\rho$是$\mathfrak{g}$的有限维线性表示。 引理$2, L^n\subset I^n(\mathfrak{g}^*)$。因此

$$
i(L^n)\subset i(I^n(\mathfrak{g}^*))\subset \mathbf{S}^n(\mathfrak{h}^*)^W
$$

由科. $2,\mathbf{S}^n(\mathfrak{h}^*)^W\subset i(L^n)$ 提案第 2 条。因此 $i(I^n(\mathfrak{g}^*)) =\mathbf{S}^n(\mathfrak{h}^*)^W$ 证明了 (i)，$i(L^n) =i(I^n(\mathfrak{g}^*))$ 证明了 b) $L^n= I^n(\mathfrak{g}^*)$。从而证明(ii)。

d) 断言 (iii) 由 (i) 和第 1 章得出。 V, §5, no. 3，周四。 3.

#### 推论 1 {#lie-viii-s8-thm-1-cor-1 .statement tag=015B}

假设 $\mathfrak{g}$ 很简单。令 $m_1, . . . , m_l$ 为 $\mathfrak{g}$ 的 Weyl 群的指数。存在 $I(\mathfrak{g}^*)$ 的元素 $P_1, . . . ,P_l$，齐次次数

$$
m_1+ 1, . . . , m_l+ 1
$$

它们在代数上是独立的且生成代数 $I(\mathfrak{g}^*)$。

这是从 Th 得出的。 2(i)和章。 V, §6, no. 2，提案 3。

#### 推论 2 {#lie-viii-s8-thm-1-cor-2 .statement tag=015C}

设B为R的基，$R_+$（或$R_-$）集合为$(\mathfrak{g},\mathfrak{h})$相对于B$,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha}$的正（或负）根，$\mathbf{S}(\mathfrak{h})$$\mathfrak{h}$的对称代数，J为理想$\mathbf{S}(\mathfrak{g})$ 由$\mathfrak{n}_+\cup \mathfrak{n}_-$ 生成。

（一）$\mathbf{S}(\mathfrak{g}) =\mathbf{S}(\mathfrak{h})\oplus J$。

(ii) 设$j$为同态，从代数$\mathbf{S}(\mathfrak{g})$到代数$\mathbf{S}(\mathfrak{h})$，由$\mathbf{S}(\mathfrak{g})$的前一个分解定义。令$I(\mathfrak{g})$为$\mathbf{S}(\mathfrak{g})$的不变式元素的集合。设$\mathbf{S}(\mathfrak{h})^W$为W的运算下不变的$\mathbf{S}(\mathfrak{h})$元素集合。则$j|I(\mathfrak{g})$从$I(\mathfrak{g})$到$\mathbf{S}(\mathfrak{h})^W$为同构。

断言 (i) 很清楚。杀戮形式定义同构从向量空间$\mathfrak{g}^*$到向量空间$\mathfrak{g}$，其中扩展到同构$\xi$来自$\mathfrak{g}$模块$\mathbf{S}(\mathfrak{g}^*)$ 到$\mathfrak{g}$-模块$\mathbf{S}(\mathfrak{g})$。我们有$\xi (I(\mathfrak{g}^*)) = I(\mathfrak{g})$。 $\mathfrak{h}$相对于杀戮形式的正交补集是$\mathfrak{n}_++\mathfrak{n}_-($§2, no. 2，命题1)。如果我们将认同$\mathfrak{h}^*$与$\mathfrak{n}_++\mathfrak{n}_-$在$\mathfrak{g}^*$中的正交补集，则$\xi (\mathfrak{h}^*) =\mathfrak{h}$，所以$\xi (\mathbf{S}(\mathfrak{h}^*)) =\mathbf{S}(\mathfrak{h})$和$\xi (\mathbf{S}(\mathfrak{h}^*)^W) =\mathbf{S}(\mathfrak{h})^W$。最后，$\xi^{-1}(J)$是$\mathfrak{g}$上的多项式函数的集合，在$\mathfrak{h}$上消失。这就证明了Th的$\xi$变换同态$i$。 1 入 Cor 的同态 $j$。 2. 因此断言 (ii) 由 Th 推出。 1（一）。

#### 命题 4 {#lie-viii-s8-prop-4 .statement tag=015D}

令$\mathfrak{a}$为半单李代数，$l$为秩。令I（分别$I'$）为$\mathbf{S}(\mathfrak{a}^*)$（分别$\mathbf{S}(\mathfrak{a})$）元素的集合，在表示下由$\mathfrak{a}$的伴随物表示诱导不变。令Z为$\mathfrak{a}$的包络代数的中心。

(i) I和$I'$是超越次数$l$的分级多项式代数（第V, §5, no. 1章）。

(ii) Z 同构于 $k$ 上$l$ 不定式多项式的代数。

$\mathfrak{a}$ 诱导的包络代数的规范过滤是 Z 的过滤。 I, §2, no. 7，周四。 1 和 p. 25，gr Z 与 $I'$ 同构的。鉴于交换代数，第 1 章。 III, §2, no. 9，第 10 条命题，因此 (i) $=\Rightarrow$ (ii)。

另一方面，Th. 1 及其 Cor。 2 证明只要 $\mathfrak{a}$ 是分裂的，(i) 就为真。一般情况约化鉴于以下引理：

#### 引理 4 {#lie-viii-s8-lem-4 .statement tag=01JY}

$^2$ 设$A =\bigoplus_{n\geq 0}A^n$ 为$k$-代数，$k'$ 扩张 $k$ 和$A'= A\otimes_kk'$。假设$A'$是$k'$的分级多项式代数。那么 A 是 $k$ 上的分级多项式代数。

我们有${A'}^0=k'$，所以$A^0=k$。输入$A_+=\bigoplus_{n\geq 1}A^n$和$P = A_+/A^2_+$。那么P是一个分级的向量空间，并且有一个分级的线性映射$f: P\rightarrow A_+$

$^2$ 在引理 4、5 和 $6,k$ 中可以是任何（可交换的）域。 次数零，使得与规范投影$A_+\rightarrow P$的复合体是P上的恒等式。给出$\mathbf{S}(P)$由P的恒等式引起的分级结构（代数，第III，p. 506）。 $k$-代数$g:\mathbf{S}(P)\rightarrow A$的同态，扩展$f$（代数，第III，p. 497）是次数0的分级同态； 直接的归纳在次数上表明 $g$ 是满射。

#### 引理 5 {#lie-viii-s8-lem-5 .statement tag=015E}

当且仅当 P 是有限维且 $g$ 是双射时，A 是分级多项式代数。

如果 P 是有限维的，则 $\mathbf{S}(P)$ 显然是分级多项式代数，如果 $g$ 是双射的话，A 也是有限维的。相反，假设 A 由次数 $d_1, . . . , d_m$ 的代数独立齐次元素 $x_1, . . . , x_m$ 生成。设P中$\overline{x}_i$为$x_i$像。P的$\overline{x}_i$形式基为直接的；由于$\overline{x}_i$是次数$d_i$，所以$\mathbf{S}(P)$和A同构；特别是，对所有 $n$ 都调暗 $\mathbf{S}(P)^n=$ 调暗 $A^n$。由于 $g$ 是满射，因此它必然是双射。

引理 4 现在是直接的。事实上，引理 5，应用于$k'$代数$A'$，表明$g\otimes 1 :\mathbf{S}(P)\otimes k'\rightarrow A\otimes k'$是双射的，因此$g$也是双射的。

#### 命题 5 {#lie-viii-s8-prop-5 .statement tag=015F}

我们保留命题4的记号，并用$\mathfrak{p}$表示由次数$\geq 1$的I齐次元素生成的$\mathbf{S}(\mathfrak{a}^*)$理想。让$x\in \mathfrak{a}$。那么 $x$ 是幂零的当且仅当 $f(x) = 0$ 对于所有 $x\in \mathfrak{p}.^3$

如有必要，扩展基域，我们可以假设$\mathfrak{a}=\mathfrak{g}$是可拆分的。假设$x$幂零。对于 $\mathfrak{g}$ 的任何有限维线性表示 $\rho$ 和任何整数 $n\geq 1$，我们有 Tr($\rho (x)^n$) $= 0$，因此 $f(x) = 0$ 对于次数 $\geq 1$ 的所有齐次 $f\in I(\mathfrak{g}^*)$ (Th. 1 (ii))，因此对于所有 $f\in \mathfrak{p}$ 都是 $f(x) = 0$。相反，如果 $f(x) = 0$ 对于所有 $f\in \mathfrak{p}$，则 Tr((ad $x$)$^n$) $= 0$ 对于所有 $n\geq 1$ (Th. 1 (ii))，因此 $x$ 是幂零的。

#### 注 1 {#lie-viii-s8-n3-rem-1 .statement tag=01L5}

\*设$P_1, . . . ,P_l$是I的代数独立齐次元素，即生成代数I。那么$(P_1, . . . ,P_l)$是一个$\mathbf{S}(\mathfrak{a}^*)$-正则序列（第V, §5, no. 5章）。事实上，如果有必要的话，扩展基域，我们可以假设$\mathfrak{a}=\mathfrak{g}$是可分割的。现在让 N = dim $\mathfrak{g}$，并让

$$
(Q_1, . . . ,Q_{N-l})
$$

是$\mathfrak{g}^*$中$\mathfrak{h}$的正交补集基。令$\mathfrak{m}$为$P_1, . . . ,P_l,Q_1, . . . ,Q_{N-l}$生成的$\mathbf{S}(\mathfrak{g}^*)$的理想。那么$\mathbf{S}(\mathfrak{g}^*)\mathfrak{m}$同构于$\mathbf{S}(\mathfrak{h}^*)/J$，其中J是由$i(P_1), . . . , i(P_l)$生成的$\mathbf{S}(\mathfrak{h}^*)$的理想。由 Th. 1 和章。 V, §5, no. 2，周四。 $2,\mathbf{S}(\mathfrak{h}^*)/J$ 是有限维向量空间，因此 $\mathbf{S}(\mathfrak{g}^*)/\mathfrak{m}$ 也是有限维。根据交换代数的结果，$(P_1, . . . ,P_l,Q_1, . . . ,Q_{N-l})$是$\mathbf{S}(\mathfrak{g}^*$)-正则序列，更不必说也是$(P_1, . . . ,P_l)$。

$^3$ 可以显示 (B. KOSTANT, 李群表示 on 多项式环,

Amer. J. Math., Vol. LXXXV (1963), pp. 327-404, Th. 10 and 15) that $\mathfrak{p}$ is a

$\mathbf{S}(\mathfrak{a}^*)$ 的素理想且 $\mathbf{S}(\mathfrak{a}^*)/\mathfrak{p}$ 是全闭的。

#### 注 2 {#lie-viii-s8-n3-rem-2 .statement tag=01L6}

代数 $\mathbf{S}(\mathfrak{a}^*)$ 是超过 I 的分级自由模。事实上，这是从第 4 条、注 1 和第 1 章得出的。 V, §5, no. 5, 引理 5.\*

### 4. PROPERTIES OF Aut0

#### 引理 6 {#lie-viii-s8-lem-6 .statement tag=015G}

令V为有限维向量空间，V的自同构的G有限群，以及V的$v$和$v'$元素，使得$v'\notin Gv$。 V 上存在 G 不变量多项式函数 $f$，使得 $f(v')\not=f(v)$。

事实上，对于每个$s\in G$，V上都存在多项式函数$g_s$，在$v$处等于1，在$sv'$处等于0。那么函数 $g= 1-\prod_{s\in G}g_s$ 等于 0

$v$ 和 $Gv'$ 上的 1。 多项式函数 $f=\prod_{t\in g}t.g$ 是 G 不变量，在 $v$ 等于 0，在 $v'$ 等于 1。

#### 命题 6 {#lie-viii-s8-prop-6 .statement tag=015H}

令$\mathfrak{a}$为半单李代数且$s\in$Aut($\mathfrak{a}$)。以下条件是等效的：

(i)$s\in$自动$_0(\mathfrak{a})$；

(ii) 对于 $\mathfrak{a}$ 上的任何不变量多项式函数 $f$，我们有 $f\circ s=f$。

通过在必要时扩展标量，我们可以假设 $k$ 是代数封闭的。蕴涵 (i) $=\Rightarrow$ (ii) 由命题 3 得出。我们假设条件 (ii) 满足并证明 (i)。鉴于第 3 号提案和 §5, no. 3，Cor.根据命题 5 的 1，我们可以假设 $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) 和 $s$ 使 Weyl 室 C 保持稳定。让$x\in C\cap \mathfrak{h}_{\mathbf{Q}}$。我们有$sx\in C$。如果$g$是$\mathfrak{h}$上的W不变量多项式函数，我们有$g(x) =g(sx)$（Th.1（i））。到引理 6，得出$sx\in Wx$。从$sx\in C$开始，我们有$x=sx$（第V, §3, no. 3章，第2章）。然后是$s|\mathfrak{h}=$ Id$_{\mathfrak{h}}$，以及$s\in$ Aut$_0(\mathfrak{g},\mathfrak{h}) ($§5, no. 2，提案 4）。

#### 推论{#lie-viii-s8-n4-cor-1 .statement tag=015I}

群 Aut$_0(\mathfrak{a})$ 在 Zariski 拓扑的 Aut($\mathfrak{a}$) 开放和关闭。

命题 6 表明 Aut$_0(\mathfrak{a})$ 是封闭的。令 $\overline{k}$ 为 $k$ 的代数闭包。 群 Aut($\mathfrak{a}\otimes \overline{k}$)$/$Aut$_0(\mathfrak{a}\otimes \overline{k})$ 是有限的（§5, no. 3，第 5 条命题第 1 条）； 更不必说, 群 Aut($\mathfrak{a}$)$/$Aut$_0(\mathfrak{a})$ 是有限的。由于 Aut($\mathfrak{a}$) 中 Aut($\mathfrak{a}$) 的陪集是闭集，因此 Aut$_0(\mathfrak{a})$ 在 Aut($\mathfrak{a}$) 中是开集。

### 5. 中心封套代数

在这个数中，我们选择基R的B。让$R_+$是相对于B的正根的集合。让$\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$和代数的$\delta$自同构 $\mathbf{S}(\mathfrak{h})$需要每个$x\in \mathfrak{h}$到$x-\rho (x)$，因此多项式函数$p$在$\mathfrak{h}^*$到函数$\lambda  \rightarrow p(\lambda -\rho )$。

#### 定理 2 {#lie-viii-s8-thm-2 .statement tag=015J}

设U为$\mathfrak{g}$的包络代数，Z为中心，$V\subset U$为$\mathfrak{h}($的包络代数，与$\mathbf{S}(\mathfrak{h}))$、$U^0$为V在U中的交换子， $\varphi$ *Harish-Chandra 同态* (§6, no. 4) 相对于$B$从$U^0$到$V$。

设$S(\mathfrak h)^W$为$S(\mathfrak h)$元素集合在$W$作用下不变。那么$(\delta\circ\varphi)|_Z$是从$Z$到$S(\mathfrak h)^W$的同构，独立于$B$的选择。

a) 令$P_{++}$为$R$、$w\in W$、$\lambda\in P_{++}$、$\mu=w\lambda$的主导权的集合。那么 $Z(\mu-\rho)$ 同构于 $Z(\lambda-\rho)$ 的子模（§6, no. 3，第 6 条命题的 Cor.2），并且 $\varphi(u)(\lambda-\rho)=\varphi(u)(\mu-\rho)$ 同构于所有 $u\in Z$（§6, no. 4，第 7 条命题）。因而，多项式函数$(\delta\circ\varphi)(u)$和$(\delta\circ\varphi)(u)\circ w$在$\mathfrak h^*$重合在$P_{++}$。但是，在 Zariski 拓扑中，$P_{++}$ 在 $\mathfrak h^*$ 中是“密集”的：这可以通过基本权 $\varpi_\alpha$ 的基由……组成识别 $\mathfrak h^*$ 与 $k^B$ 来看出，并通过*代数* 第 9 章应用提案 9 IV, §2, no. 3。因而

$$
(\delta\circ\varphi)(u)=(\delta\circ\varphi)(u)\circ w,
$$

这就证明了$(\delta\circ\varphi)(Z)\subset S(\mathfrak h)^W$。

b) 令$\eta$为同构，从$I(\mathfrak g)$到$S(\mathfrak h)^W$，在no. 3中定义。 2 Th。 1. 考虑从$\mathfrak g$-模块$U$到$\mathfrak g$-模块$S(\mathfrak g)$（第I, §2, no. 8章）的典范同构，并令$\theta$为其限制到$Z$。然后$\theta(Z)=I(\mathfrak g)$。令$z$为$Z$的元素，并在$U$中过滤$\leqslant f$。

$$
\begin{array}{ccc}
Z & \xrightarrow{\theta} & I(\mathfrak g)\\
\Big\downarrow{\scriptstyle\varphi} & & \Big\downarrow{\scriptstyle\eta}\\
S(\mathfrak h) & \xrightarrow{\delta} & S(\mathfrak h).
\end{array}
$$

引入§6, no. 4中的记号，并把

$$
z=
\sum_{\sum q_i+\sum m_i+\sum p_i\leqslant f}
\lambda_{(q_i),(m_i),(p_i)}
u((q_i),(m_i),(p_i)).
$$

设 $v((q_i),(m_i),(p_i))$ 为单项式
$X_{\alpha_1}^{q_1}\cdots X_{\alpha_n}^{q_n}H_1^{m_1}\cdots H_l^{m_l}X_{\alpha_1}^{p_1}\cdots X_{\alpha_n}^{p_n}$
按$S(\mathfrak g)$计算。用次数 $0,1,\ldots,d$ 的 $S(\mathfrak g)$ 的齐次分量 $S_d(\mathfrak g)$ 和表示，我们有

$$
\theta(z)\equiv
\sum_{\sum q_i+\sum m_i+\sum p_i=f}
\lambda_{(q_i),(m_i),(p_i)}v((q_i),(m_i),(p_i))
\pmod{S_{f-1}(\mathfrak g)}
$$

所以

$$
(\eta\circ\theta)(z)\equiv
\sum_{\sum m_i=f}
\lambda_{(0),(m_i),(0)}v((0),(m_i),(0))
\pmod{S_{f-1}(\mathfrak h)}
$$

因而

$$
(\eta\circ\theta)(z)\equiv\varphi(z)
\pmod{S_{f-1}(\mathfrak h)}.
\tag{3}
$$

c) 我们证明$\delta\circ\varphi:Z\longrightarrow S(\mathfrak h)^W$是双射的。 $U$ 和 $S(\mathfrak g)$ 诱导 $Z$、$I(\mathfrak g)$ 和 $S(\mathfrak h)^W$ 的规范过滤以及 $\theta$、$\eta$ 与这些过滤兼容，因此 gr($\eta \circ \theta$ ) 为同构向量空间 gr(Z) 至向量空间 gr($\mathbf{S}(\mathfrak{h})^W$)。由(3)可知gr($\varphi$)$=$gr($\eta \circ \theta$)，显然gr($\delta$)是恒等式。因此 gr($\delta \circ \varphi$ ) 是双射的，所以

$$
\delta \circ \varphi : Z\rightarrow \mathbf{S}(\mathfrak{h})^W
$$

是双射的（交换代数，第 III, §2, no. 8 章，第 1 章的 Cor. 1 和 2）。

d) 回忆一下 a) 中的记号。令 E 为最高权 $\lambda$ 的简单$\mathfrak{g}$模，$\chi$其中心特征标（§6, no. 1，定义 2）。令$\varphi '$和$\delta '$是同态，类似于相对于基$w(B)$的$\varphi$和$\delta$。 E相对于$w(B)$的最高权是$w(\lambda )$。根据第 7 号提案，§6, no. 4，

$$
\varphi (u)(\lambda ) =\chi (u) =\varphi '(u)(w\lambda )
$$

对于所有 $u\in Z$，因此，通过 a)，

$$
(\delta \circ \varphi )(u)(w\lambda +w\rho ) = (\delta \circ \varphi )(u)(\lambda +\rho ) =\varphi (u)(\lambda ) =\varphi '(u)(w\lambda )
$$

$$
= (\delta '\circ \varphi ')(u)(w\lambda +w\rho )
$$

因此，多项式函数$(\delta \circ \varphi )(u)$和$(\delta '\circ \varphi ')(u)$重合在$w(P_{++}) +w\rho$上，因此是相等的。

#### 推论 1 {#lie-viii-s8-thm-2-cor-1 .statement tag=015K}

对于所有$\lambda \in \mathfrak{h}^*$，令$\chi_{\lambda}$为从Z到$k$的同态$z \rightarrow (\varphi (z))(\lambda )$。

(i) 如果 $k$ 是代数闭的，则对于某些 $\lambda \in \mathfrak{h}^*$，从 Z 到 $k$ 的每个同态都是形式 $\chi_{\lambda}$。

(ii) 令 $\lambda , \mu\in \mathfrak{h}^*$。那么$\chi_{\lambda}=\chi_\mu$当且仅当$\mu+\rho \in W(\lambda +\rho )$。

如果$k$是代数闭的，则从$\mathbf{S}(\mathfrak{h})^W$到$k$的每个同态，从$\mathbf{S}(\mathfrak{h})$到$k($交换代数的扩展到同态，第1章。 V, §1, no. 9，第 22 号提案，以及§2, no. 1，Cor. 4 Th。 1)，从$\mathbf{S}(\mathfrak{h})$到$k$的每个同态对于某些$\lambda \in \mathfrak{h}^*$来说都是形式$f \rightarrow f(\lambda )$（第VII章，App.I，提案1）。因此，如果从 Z 到 $k$ $\chi$ 是同态，则存在 (Th. 2) $\mu\in \mathfrak{h}^*$，使得对于所有 $z\in Z$，

$$
\chi (z) = ((\delta \circ \varphi )(z))(\mu) = (\varphi (z))(\mu-\rho )
$$

因此(i)。

设$\lambda , \mu\in \mathfrak{h}^*$并假设$\chi_{\lambda}=\chi_\mu$。那么，对于所有$z\in Z$，

$$
((\delta \circ \varphi )(z))(\lambda +\rho ) = (\varphi (z))(\lambda ) =\chi_{\lambda}(z) =\chi_\mu(z) = ((\delta \circ \varphi )(z))(\mu+\rho )
$$

其他字、同态从$\mathbf{S}(\mathfrak{h})$到$k$由$\lambda +\rho$和$\mu+\rho$重合定义在$\mathbf{S}(\mathfrak{h})^W$上；因此，断言 (ii) 源自交换代数，第 1 章。 V, §2, no. 2，科。的 Th。 2.

#### 推论 2 {#lie-viii-s8-thm-2-cor-2 .statement tag=015L}

令$E,E'$为有限维简单$\mathfrak{g}$模，$\chi , \chi '$为它们的中心特征标。若$\chi =\chi '$，则E与$E'$同构的。

设$\lambda , \lambda '$为$E,E'$中的最高权。根据§6, no. 4，命题$7,\chi_{\lambda}=\chi =$$\chi '=\chi_{\lambda'}$，因此存在$w\in W$使得$\lambda '+\rho =w(\lambda +\rho )$。由于$\lambda +\rho$和$\lambda '+\rho$属于到B定义的室，我们有$w= 1$。因此，$\lambda =\lambda '$，因此是推论。

#### 命题 7 {#lie-viii-s8-prop-7 .statement tag=015M}

对于任何有限维简单$\mathfrak{g}$模的类$\gamma$，令$U_{\gamma}$为$\mathfrak{g}$模U的型$\gamma$的同型分量（对于U上$\mathfrak{g}$的伴随表示）。令$\gamma_0$为维数1的平凡$\mathfrak{g}$模的类。令$[U,U]$为由U的元素的对的括号生成的U的向量子空间。

(i) U 是 $U_{\gamma}$ 中的直和。

(ii)$U_{\gamma_0}= Z$和$\sum_{\gamma\not=\gamma_0}U_{\gamma}= [U,U]$。

(iii) 令 $u \rightarrow u^{\natural}$ 为由分解 $U = Z\oplus [U,U]$ 定义的 U 到 Z 的投影。如果$u\in U$和$v\in U$，我们有$(uv)^{\natural}= (vu)^{\natural}$。如果$u\in U$和$z\in Z$，我们有$(uz)^{\natural}=u^{\natural}z$。

(iv) 令 $\varphi$ 为 Harish-Chandra 同态。设$\lambda \in P_{++}$，并令E为最高权$\lambda$的有限维简单$\mathfrak{g}$模。对于所有 $u\in U$，我们有

暗淡 E1 Tr($u_E$) $= (\varphi (u^{\natural}))(\lambda )$。

$\mathfrak{g}$模U是有限维子模的直和。这意味着（i）。

显然$U_{\gamma_0}= Z$。令$U'$为U的向量子空间，定义伴随表示的类$\gamma$的子表示。然后$[\mathfrak{g},U'] = U'$或$[\mathfrak{g},U'] = 0$。因此，如果$\gamma \not=\gamma_0$则$[\mathfrak{g},U'] = U'$，所以$\sum_{\gamma\not=\gamma_0}U_{\gamma}\subset [U,U]$。另一方面，如果 $u\in U$ 和 $x_1, . . . , x_n\in \mathfrak{g}$，则

$$
[x_1. . . x_n, u] = (x_1. . . x_nu-x_2. . . x_nux_1)+(x_2. . . x_nux_1-x_3. . . x_nux_1x_2)
$$

$$
+\cdots + (x_nux_1. . . x_{n-1}-ux_1. . . x_n)\in [\mathfrak{g},U]
$$

因此$[U,U]\subset [\mathfrak{g},\sum_{\gamma}U_{\gamma}]=[\mathfrak{g},\sum_{\gamma\not=\gamma_0}U_{\gamma}]\subset \sum_{\gamma\not=\gamma_0}U_{\gamma}$。这就证明了(ii)。在这些条件下，(iii) 源自第 1 章。 I, §6, no. 9、引理5。

最后，让$E, \lambda$如(iv)中所示。然后

Tr($u_E$) $=$ Tr(($u^{\natural}$)$_E$) 自 $u-u^{\natural}\in [U,U]$

= Tr($\varphi (u^{\natural})(\lambda ).1$) (§$6$, 否$.4$, 提案$.7$)

=（暗淡$E$）$.\varphi (u^{\natural})(\lambda )$。

### 习题 {#lie-viii-s8-exercises}

参见[习题为 § 8](exercises/s8/)。
