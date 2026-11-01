---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 1
section_title: Primary decomposition of linear representations
lang: zh
source: lie-vii-ix
book_pages: 1-12, 51-55
pdf_pages: 0011-0022, 0060-0064
extraction: native
subsections:
    - "no": 1
      title: DECOMPOSITION OF A FAMILY OF ENDOMORPHISMS
      page: 1
      pdf_page: 11
    - "no": 2
      title: THE CASE OF A LINEAR FAMILY OF ENDOMORPHISMS
      page: 6
      pdf_page: 16
    - "no": 3
      title: DECOMPOSITION OF REPRESENTATIONS OF A NILPOTENT LIE ALGEBRA
      page: 8
      pdf_page: 18
    - "no": 4
      title: DECOMPOSITION OF A LIE ALGEBRA RELATIVE TO AN AUTOMORPHISM
      page: 11
      pdf_page: 21
    - "no": 5
      title: INVARIANTS OF A SEMI-SIMPLE LIE ALGEBRA RELATIVE TO A SEMI-SIMPLE ACTION
      page: 11
      pdf_page: 21
statements: 25
exercises: 11
content_sha256: d1e4793707fa06b48afd90732d41d53749051e6113e964ace111531913bc17b4
translated_from: content/en/lie/VII/01_s1_primary_decomposition_of_linear.md
translation_method: google
source_content_sha256: 6d999a4f63ad71547f9729f56137320e39f7832c9c6c88d90de525d543eda5ce
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: f0c88b27d98a9743730582f745cdf25f86e0aad293b5437dd5d28f9e4bd285dc
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。 初等分解 / 线性表示

### 1. 分解自同态家庭

设V为向量空间，S集合，以及从S到End(V)的$r$映射。用从 S 到 $k$ 的映射的 P 集合表示。如果$\lambda \in P$，则用$v\in V$的$V_{\lambda}(S)$（或$V^{\lambda}(S)$）集合表示，使得对于所有$s\in S,r(s)v=\lambda (s)v$（或$n$足够大，分别用$(r(s)-\lambda (s))^nv= 0$）。 集合$V_{\lambda}(S)$和$V^{\lambda}(S)$是V和$V_{\lambda}(S)\subset V^{\lambda}(S)$的向量子空间。我们说$V_{\lambda}(S)$是V相对于$\lambda$（和$r$）的本征空间，$V^{\lambda}(S)$是V相对于$\lambda$（和$r$）的主子空间，并且$V^0(S)$是V的零空间（相对于$r$）。如果$V^{\lambda}(S)\not= 0$，我们说$\lambda$是V中S的权。

特别地，如果S约化到单个元素$s, P$可以用$k$来识别；我们使用记号$V_{\lambda(s)}(s)$和$V^{\lambda(s)}(s)$，或$V_{\lambda(s)}(r(s))$和$V^{\lambda(s)}(r(s))$，而不是$V_{\lambda}(\{s\}), V^{\lambda}(\{s\})$；我们谈论本征空间、初级子空间和 $r(s)$ 的零空间； $V_{\lambda(s)}(s)$的元素$v$称为$r(s)$的特征向量，并且，如果$v\not= 0,\lambda (s)$称为相应的特征值（cf.代数，第VII, §5章）。

对于所有 $\lambda \in P$，以下关系为直接的：

$$
V^{\lambda}(S) =\bigcap_{s\in S}V^{\lambda(s)}(s) \tag{1}
$$

$$
V_{\lambda}(S) =\bigcap_{s\in S}V_{\lambda(s)}(s) \tag{2}
$$

设$k'$为$k$中的扩张。从 End(V) 到 End($V\otimes_kk'$) 的规范映射通过合成和 $r$ 给出映射 $r': S\rightarrow$ End($V\otimes_kk'$)。类似地，从S到$k$定义的每个映射$\lambda$规范地映射，也用$\lambda$表示，从S到$k'$。有了这些记号，我们就有了以下命题：

#### 命题 1 {#lie-vii-s1-prop-1 .statement tag=00SJ}

对于所有$\lambda \in P$，

$(V\otimes_kk')^{\lambda}(S) = V^{\lambda}(S)\otimes_kk'$ 和 $(V\otimes_kk')_{\lambda}(S) = V_{\lambda}(S)\otimes_kk'$。

令$(a_i)$为$k$向量空间$k'$的基。如果$v\in V\otimes_kk',v$可以用形式$\sum v_i\otimes a_i$唯一地表达，其中$(v_i)$是元素和V的有限支持族。对于所有$s\in S$，

$$
(r'(s)-\lambda (s))^n(v) =\sum(r(s)-\lambda (s))^nv_i\otimes a_i
$$

由此可见

$v\in (V\otimes_kk')^{\lambda}(S)\Leftarrow \Rightarrow v_i\in V^{\lambda}(S)$ 对于所有$i$，

$v\in (V\otimes_kk')_{\lambda}(S)\Leftarrow \Rightarrow v_i\in V_{\lambda}(S)$ 对于所有$i$，

这意味着命题。

#### 命题 2 {#lie-vii-s1-prop-2 .statement tag=00SK}

令$V,V',W$为向量空间。令 $r$ : S $\rightarrow$ End(V)、$r': S\rightarrow$ End(V$'$) 和 $q: S\rightarrow$ End(W) 为映射。

(i) 令 $f: V\rightarrow W$ 为线性映射，使得 $q(s)f(v) =f(r(s)v)$ 对于 $s\in S$ 和 $v\in V$。然后，将所有 $\lambda \in P,f$ 映射 $V^{\lambda}(S)$（分别为 $V_{\lambda}(S)$）转换为 $W^{\lambda}(S)$（分别为 $W_{\lambda}(S)$）。

(ii) 设 $B : V\times V'\rightarrow W$ 为双线性映射，使得

$$
q(s)B(v, v') = B(r(s)v, v') + B(v, r'(s)v')
$$

$s\in S,v\in V,v'\in V'$。然后，对于所有 $\lambda , \mu\in P$，B 映射 $V^{\lambda}(S)\times {V'}^\mu(S)$（分别为 $V_{\lambda}(S)\times V'_\mu(S)$）变为 $W^{\lambda+\mu}(S)$（分别为 $W_{\lambda+\mu}(S)$）。

(iii) 设 $B : V\times V'\rightarrow W$ 为双线性映射，使得

$$
q(s)B(v, v') = B(r(s)v, r'(s)v')
$$

$s\in S,v\in V,v'\in V'$。然后，对于所有 $\lambda , \mu\in P$，B 映射 $V^{\lambda}(S)\times {V'}^\mu(S)$（分别为 $V_{\lambda}(S)\times V'_\mu(S)$）变为 $W^{\lambda \mu}(S)$（分别为 $W_{\lambda \mu}(S)$）。

在情况(i)中，$(q(s)-\lambda (s))^nf(v) =f((r(s)-\lambda (s))^nv)$对应$s\in S$和$v\in V$，因此得出结论。在情况(ii)中，

$$
(q(s)-\lambda (s)-\mu(s))B(v, v') = B((r(s)-\lambda (s))v, v') + B(v,(r'(s)-\mu(s))v')
$$

对于 $s\in S,v\in V,v'\in V'$，因此在 $n$ 上获得归纳

$$
'(n)''
$$

$(q(s)-\lambda (s)-\mu(s))^nB(v, v) =\sum B((r(s)-\lambda (s))^iv,(r(s)-\mu(s))^jv)$。

$$
i
$$

$i+j=n$

(ii) 中的断言紧随其后。在情况(iii)中，$(q(s)-\lambda (s)\mu(s))B(v, v') = B((r(s)-\lambda (s))v, r'(s)v')+B(\lambda (s)v,(r'(s)-\mu(s))v')$对应$s\in S,v\in V,v'\in V'$，因此归纳在$n$

$$
(q(s)-\lambda (s)\mu(s))^nB(v, v')
$$

= $\sum(n)B(\lambda (s)^j(r(s)-\lambda (s))^iv, r'(s)^i(r'(s)-\mu(s))^jv')$。

$$
i
$$

$i+j=n$

(iii) 中的断言紧随其后。

#### 命题 3 {#lie-vii-s1-prop-3 .statement tag=00SL}

和 $\sum_{\lambda\in P}V^{\lambda}(S)$ 是直达。 和 $\sum_{\lambda\in P}V_{\lambda}(S)$ 是直达。

第二个断言是第一个的推论；因此足以证明这一点。我们区分几种情况。

$a) S$ 是空的。 断言是微不足道的。

$b) S$ 减少为单个元素 $s$。令 $\lambda_0, \lambda_1, . . . , \lambda_n$ 不同于 $k$ 的元素。对于$i= 0,1, . . . , n$，设$v_i\in V^{\lambda_i}(s)$并假设$v_0=v_1+\cdots +v_n$。只需证明 $v_0$ = 0。对于 $i= 0, . . . , n$，存在整数 $q_i>$ 0，使得 $(r(s)-\lambda_i)^{q_i}v_i$ = 0。考虑多项式 $P(X) =\prod_{i\geq 1}(X-\lambda_i)^{q_i}$ 和 $Q(X) = (X-\lambda_0)^{q_0}$。我们有 $Q(r(s))v_0= 0$，并且

$P(r(s))v_0=\sum_{i=1}^nP(r(s))v_i= 0$。由于 P 和 Q 互质，Bezout 恒等式证明 $v_0= 0$。

$c) S$ 是有限且非空的。我们通过归纳对S的基数进行争论。设$s\in S$和$S'= S$**--** $\{s\}$。令$(v_{\lambda})_{\lambda\in P}$是元素和V的有限支持族，使得$\sum_{\lambda\in P}v_{\lambda}= 0$和$v_{\lambda}\in V^{\lambda}(S)$。让$\lambda_0\in P$。令$P'$为$\lambda \in P$的集合，使得$\lambda |S'=\lambda_0|S'$。将归纳假设应用于$S'$，我们就有$\sum_{\lambda\in P'}v_{\lambda}= 0$。如果$\lambda , \mu$不同于元素或$P',\lambda (s)\not=\mu(s)$。

由于和 $\sum_{\alpha\in k}V^{\alpha}(s)$ 是 b) 的直达，并且由于 $v_{\lambda}\in V^{\lambda(s)}(s),v_{\lambda}= 0$ 对于所有 $\lambda \in P'$，特别是 $v_{\lambda_0}= 0$，我们必须证明这一点。

d) 一般情况。令$(v_{\lambda})_{\lambda\in P}$是元素和V的有限支持族，使得$\sum_{\lambda\in P}v_{\lambda}= 0$和$v_{\lambda}\in V^{\lambda}(S)$。令$P'$为$\lambda \in P$的有限集合，使得$v_{\lambda}\not= 0$，并让$S'$为S的有限子集，使得条件$\lambda \in P'$，$\mu\in P',\lambda |S'=\mu|S'$暗示$\lambda =\mu$。我们有$v_{\lambda}\in V^{\lambda|S'}(S')$； 应用的 c)，我们看到$v_{\lambda}= 0$对应$\lambda \in P'$，从而完成了证明。

回想一下，如果 $x\in$ End(V)，我们用 ad $x$ 映射 $y \rightarrow xy-yx= [x, y]$ 表示从 End(V) 到自身。

#### 引理 1 {#lie-vii-s1-lem-1 .statement tag=00SM}

让$x, y\in$结束(V)。

(i) 假设 V 是有限维的。那么$x$可三角化当且仅当$V =\sum_{a\in k}V^a(x)$。

(ii) 如果存在整数$n$使得(ad$x$)$^ny= 0$，则每个$V^a(x)$在$y$下稳定。

(iii) 假设 V 是有限维的。如果 $V =\sum_{a\in k}V^a(x)$ 并且如果每个

$V^a(x)$在$y$下稳定，存在整数$n$使得(ad$x$)$^ny= 0$。

部分 (i) 源自代数，第 1 章。 VII, §5, no. 2，提案 3。

令 E = End(V)。令 B 为从 $E\times V$ 到 V 的双线性映射 $(u, v) \rightarrow u(v)$。通过广告$x$的定义，

$x(B(u, v)) =B(u, x(v)) +$ B((广告$x$)$(u), v$)

$x\in E,u\in E,v\in V$。让$x$通过ad$x$对E进行操作。根据提案 2 (ii)，$B(E^0(x),V^a(x))\subset V^a(x)$ 适用于所有 $a\in k$。如果(ad $x$)$^ny= 0$，则$y\in E^0(x)$，所以$y(V^a(x))\subset V^a(x)$，这就证明了(ii)。

为了证明(iii)，我们可以将替换V乘以$V^a(x)$，并将$x$（或$y$）乘以限制到$V^a(x)$。 替换 $x$乘以$x-a$，我们可以假设$x$是幂零的。然后，(ad $x$)$^{2 dim V-1}= 0$（第I, §4, no. 2章），证明了(iii)。

#### 注 {#lie-vii-s1-n1-rem-1 .statement tag=00SN}

该论证证明，如果 V 是有限维的，并且存在整数 $n$ 使得 (ad $x$)$^ny= 0$，则 (ad $x$)$^{2 dim V-1}y= 0$。

在续集中，我们可以说映射 $r: S\rightarrow$ End(V) 满足条件 (AC)（“几乎可交换”），如果：

(AC) 对于 S 的元素的每一个对 $(s, s')$，都存在整数 $n$，使得

（广告$r(s)$）$^nr(s') = 0$。

#### 定理 1 {#lie-vii-s1-thm-1 .statement tag=00SO}

假设 V 是有限维的。以下条件是等效的：

(i) 满足条件 (AC)，并且对于所有$s\in S,r(s)$ 是可三角化的。

(ii) 对于所有 $\lambda \in P$，$V^{\lambda}(S)$ 在 $r(S)$ 和 $V =\sum_{\lambda\in P}V^{\lambda}(S)$ 下是稳定的。

如果$V =\sum_{\lambda\in P}V^{\lambda}$(S)，则$V =\sum_{a\in k}V^a(s)$对于所有$s\in S$，并且它由

引理 1 (ii) 意味着 (i)。假设满足条件(i)。 引理 1 和公式 (1) 意味着每个$V^{\lambda}(S)$ 在$r(S)$ 下是稳定的。还有待证明$V =\sum_{\lambda\in P}V^{\lambda}(S)$。我们在昏暗的V上争论归纳。我们区分两种情况。

a) 对于所有 $s\in S,r(s)$ 都有一个特征值 $\lambda (s)$。然后$V = V^{\lambda}(S)$。

b) 存在$s\in S$使得$r(s)$至少有两个不同的特征值。那么 $a\in k$ 的 V 就是 $V^a(s)$ 的直和，而所有 $a$ 的暗淡 $V^a(s)<$ 暗淡 V。每个$V^a(s)$在$r$(S)下是稳定的，应用归纳假设就足够了。

#### 推论 1 {#lie-vii-s1-thm-1-cor-1 .statement tag=00SP}

假设V是有限维的并且满足条件(AC)。令 $k'$ 为 $k$ 的扩张。假设对于所有 $s\in S$，自同态 $r(s)\otimes 1$ 或 $V\otimes_kk'$ 都是可三角化的。令$P'$为从S到$k'$的映射中的集合。然后$V\otimes_kk'=\sum_{\lambda'\in P'}(V\otimes_kk')^{\lambda'}(S)$。

令$r': S\rightarrow$End(V$\otimes_kk'$)为由$r$定义的映射。如果 $s_1, s_2\in S$，则存在整数 $n$，使得 (ad $r(s_1)$)$^nr(s_2) = 0$，因此 (ad $r'(s_1)$)$^nr'(s_2) = 0$。现在应用 Th 就足够了。 1.

#### 推论 2 {#lie-vii-s1-thm-1-cor-2 .statement tag=00SQ}

假设V是有限维的并且满足条件(AC)。用$V^+(S)$向量子空间$\sum_{s\in S}((\bigcap_{i\geq 1}r(s)^iV)$表示。然后：

(i) $V^0(S)$和$V^+(S)$在$r(S)$下稳定；

(ii) $V = V^0(S)\oplus V^+(S)$；

(iii) V的每向量子空间W，在$r(S)$下稳定，并且$W^0(S) = 0$包含在$V^+(S)$中；

（四）$\sum_{s\in S}r(s)V^+(S) = V^+(S)$。

此外，$V^+(S)$是V中唯一具有性质(i)和(ii)的向量子空间。对于 $k,(V\otimes_kk')^+(S) = V^+(S)\otimes_kk'$ 中的任意扩张 $k'$。

最后一个断言是直接的。因此，考虑到命题 1，在证明中，我们可以假设 $k$ 是代数封闭的。由 Th. 1、V = $\sum_{\lambda\in P}V^{\lambda}$(S)，且$V^{\lambda}(S)$在$r(S)$下稳定。若$s\in S$，则特征

$r(s)|V^{\lambda}(S)$的多项式为$(X-\lambda (s))^{dim V^{\lambda}(S)}$；由此可见 $\bigcap_{i\geq 1}r(s)^iV^{\lambda}(s)$

如果$\lambda (s) = 0$，则为零；如果$\lambda (s)\not= 0$，则等于$V^{\lambda}(S)$；因此，

$$
V^+(S) =\sum_{\lambda\in P,\lambda\not=0}V^{\lambda}(S) \tag{3}
$$

从而证明 (i)、(ii) 和 (iv)。如果W是V的向量子空间在$r$(S)下稳定，则$W =\sum_{\lambda\in P}W^{\lambda}(S)$和$W^{\lambda}(S) = W\cap V^{\lambda}(S)$。如果$W^0(S) = 0$，我们看到$W\subset V^+$(S)，这证明了(iii)。

令 $V'$ 为 V 的向量子空间在 $r(S)$ 下稳定，使得 $V'\cap V^0(S) = 0$。然后 ${V'}^0(S) = 0$，所以 $V'\subset V^+(S)$ 由 (iii) 得到。如果，在加法、$V = V^0(S) + V'$中，我们看到$V'= V^+(S)$。 Q.E.D.

我们将有时称为V的$(V^0(S),V^+(S))$Fitting 分解，或映射$r: S\rightarrow$End(V)。如果 S 约化到单个元素 $s$，我们写 $V^+(s)$ 或 $V^+(r(s))$ 而不是 $V^+(\{s\})$。我们知道 $V = V^0(s)\oplus V^+(s), V^0(s)$ 和 $V^+(s)$ 在 $r(s),r(s)|V^0(s)$ 幂零且 $r(s)|V^+(s)$ 是双射的情况下是稳定的。

#### 推论 3 {#lie-vii-s1-thm-1-cor-3 .statement tag=00SR}

令V和$V'$为有限维向量空间，并令$r: S\rightarrow$End(V)和$r': S\rightarrow$End(V$'$)为映射满足条件(AC)。令 $f: V\rightarrow V'$ 为满射线性映射，使得 $f(r(s)v) =r'(s)f(v)$ 对于 $s\in S$ 和 $v\in V$。然后 $f(V^{\lambda}{(S)) = V'}^{\lambda}(S)$ 代表所有 $\lambda \in P$。

鉴于命题 1，我们被简化为 $k$ 是代数闭的情况。我们有 $V =\bigoplus_{\lambda\in P}V^{\lambda}$(S)、$V'=\bigoplus_{\lambda\in P}{V'}^{\lambda}(S)$ Th。 1、和$V'=f(V) =$$\sum_{\lambda\in P}f(V^{\lambda}(S))$。最后，根据命题 2 (i)，$f(V^{\lambda}(S))\subset {V'}^{\lambda}(S)$，因此得出推论。

#### 命题 4 {#lie-vii-s1-prop-4 .statement tag=00SS}

假设 $k$ 是完美的。令V为End(V)$,u_s, u_n$半单的有限维向量空间、$u$元素和$u($代数的幂零分量，第1章。 VII, §5, no. 8）。

(i) 对于所有$\lambda \in k,V^{\lambda}(u) = V^{\lambda}(u_s) = V_{\lambda}(u_s)$。

(ii) 如果V有代数结构，并且如果$u$是V$,u_s$中的推导，并且$u_n$是V中的推导。

(iii) 如果V有代数结构，并且如果$u$是V的自同构，则$u_s$和$1 +u^{-1}_su_n$是V的自同构。

根据命题 1，我们可以假设 $k$ 是代数闭的，所以

$$
V =\sum_{\lambda\in k}V^{\lambda}(u)
$$

$u|V^{\lambda}(u)$的半单分量是位似，$V^{\lambda}(u)$中的比率为$\lambda$。这就证明了(i)。

假设从现在开始V有代数结构。让$x\in V^{\lambda}(u)$，$y\in V^\mu(u)$。

如果$u$是V的推导，则$xy\in V^{\lambda+\mu}(u)$（命题2（ii）），所以

$$
u_s(xy) = (\lambda +\mu)(xy) = (\lambda x)y+x(\mu y) = (u_sx)y+x(u_sy)
$$

这证明$u_s$是V的推导。那么$u_n=u-u_s$就是V的推导。

如果$u$是V的自同构，则Ker($u_s$)$= V^0(u) = 0$，所以$u_s$是双射的。另一方面，$xy\in V^{\lambda \mu}(u)$（命题 2 (iii)），所以

$$
u_s(xy) = (\lambda \mu)(xy) = (\lambda x)(\mu y) =u_s(x).u_s(y)
$$

这就证明$u_s$是V的自同构；但事实也是如此

$$
1 +u^{-1}_su_n=u^{-1}_su
$$

### 2. 自同态线性族的情况

现在假设 S 具有向量空间结构，映射 $r: S\rightarrow$ End(V) 是线性的，V 和 S 是有限维的。

#### 命题 5 {#lie-vii-s1-prop-5 .statement tag=00ST}

假设满足条件(AC)，并令$\lambda : S\rightarrow k$使得$V^{\lambda}(S)\not= 0$。如果 $k$ 的特征为 0，则映射 $\lambda$ 是线性的。如果$k$具有特征$p\not= 0$，则存在$p$除暗$V^{\lambda}(S)$的幂$q$，以及次数$q$的齐次多项式函数$P : S\rightarrow k$，使得$\lambda (s)^q= P(s)$对于所有$s\in S$。

由于$V^{\lambda}(S)$在$r(S)$（no. 1的引理 1和公式（1））下稳定，我们可以假设$V = V^{\lambda}(S)$。让$n=$变暗V。因此，对于$s\in S$，

德特（X$-r(s)$）$= (X-\lambda (s))^n$。

另一方面，行列式展开表明

检测（X$-r(s)$）$= X^n+a_1(s)X^{n-1}+\cdots +a_i(s)X^{n-i}+\cdots$

其中$a_i: S\rightarrow k$是次数$i$的齐次多项式函数。写出$n=qm$，其中$q$是$k$和$(q, m) = 1$的特征指数的幂。然后$(X-\lambda (s))^n= (X^q-\lambda (s)^q)^m$；因此$-m\lambda (s)^q=a_q(s)$，这意味着结果。

#### 命题 6 {#lie-vii-s1-prop-6 .statement tag=00SU}

假设$k$是无限的并且满足条件(AC)。设$k'$为$k$中的扩张。把$V'= V\otimes_kk',S'= S\otimes_kk'$。令$r': S'\rightarrow$End(V$'$)为从$r$通过标量扩张获得的映射。然后

$$
V^0(S)\otimes_kk'{= V'}^0{(S) = V'}^0(S')
$$

第一个等式源自命题1。为了证明第二个，我们可以假设$V = V^0(S)$，因此$V'{= V'}^0(S)$。设 $(s_1, . . . , s_m)$ 为 S 的基，且 $(e_1, . . . , e_n)$ 基为 V。存在多项式 $P_{ij}(X_1, . . . ,X_m)$ 使得

$$
r'(a_1s_1+\cdots +a_ms_m)^ne_j=\sum_{i=1}^nP_{ij}(a_1, . . . , a_m)e_i
$$

对于 $1\leq j\leq n$ 和 $a_1, . . . , a_m\in k'$。 假设、$r'(s)^n= 0$适用于所有$s\in S$，其他字$P_{ij}(a_1, . . . , a_m) = 0$适用于$1\leq i, j\leq n$和$a_1, . . . , a_m\in k$。由于 $k$ 是无限的，$P_{ij}= 0$。因而，$r'(S')$的每个元素都是幂零的，$V'{= V'}^0(S')$。

#### 命题 7 {#lie-vii-s1-prop-7 .statement tag=00SV}

假设$k$是无限的并且满足条件(AC)。令$\widetilde{S}$为$s\in S$的集合，使得$V^0(s) = V^0(S)$。如果$s\in S$，则令$P(s)$为由$r(s)$定义的$V/V^0(S)$的自同态的行列式（no. 1，Th.1的Cor.2(i)）。

(i) 函数 $s \rightarrow P(s)$ 是 S 上的多项式。我们有 $\widetilde{S} =\{s\in S|P(s)\not= 0\}$；这是 Zariski 拓扑中 S 的开子集（App. 1）。

(ii) $\widetilde{S}$非空，并且$V^+(s) = V^+(S)$对于所有$s\in \widetilde{S}$。

$s \rightarrow P(s)$ 是多项式这一事实是由 $r$ 的线性性得出的。如果$s\in S, V^0(s)\supset V^0$(S)，则等式当且仅当$r(s)$定义自同构为$V/V^0$(S)，因而(i)。

现在令 $k'$ 为 $k$ 的代数闭包，并引入 $V',S', r'$，如命题 6 中所示。通过多项式恒等式 (ad $r(s_1)$)$^{2 dim V-1}r(s_2) = 0$ 的延拓，注 $S'$ 满足条件 (AC)有效期为$s_1, s_2\in S$（no. 1、注）。 应用Th.1，我们推导出分解

$$
V'{= V'}^0(S')\oplus \sum_{i=1}^m{V'}^{\lambda_i}(S')
$$

$\lambda_i\not= 0$ 为 $1\leq i\leq m$。对于$1\leq i\leq m$，在$S'$和整数$q_i$上存在多项式函数$P_i$非零，使得$\lambda^{q_i}_i= P_i$（命题5）。由于$k$是无限的，因此存在$s\in S$使得$(P_1. . .P_m)(s)\not= 0$，cf.代数，第1章。 IV, §2, no. 3，科。命题 9 的 2。然后 $\lambda_i(s)\not= 0$ 对于所有 $i$，因而 ${V'}^0(S'{) = V'}^0(s)$，因而 $V^0(S) = V^0(s)$（命题 6），这表明 $\widetilde{S}\not=\emptyset$。如果$s\in \widetilde{S}$，$V^+(S)$在$r(s)$下是稳定的，并且是V中$V^0(s)$的补集，这一事实意味着$V^+(S) = V^+(s)$（Th.1的Cor.2）。

### 3. 分解表示幂零李代数

设 $\mathfrak{h}$ 为李代数，M 为 $\mathfrak{h}$ 模。 对于从$\mathfrak{h}$到$k$的任何映射$\lambda$，我们已经在M的no. 1向量子空间$M^{\lambda}(\mathfrak{h})$和$M_{\lambda}(\mathfrak{h})$中定义。 特别是，如果$\mathfrak{g}$是李代数包含$\mathfrak{h}$和子代数，如果$x\in \mathfrak{g}$，我们经常会使用记号$\mathfrak{g}^{\lambda}(\mathfrak{h})$和$\mathfrak{g}_{\lambda}(\mathfrak{h})$；然后可以理解，$\mathfrak{h}$通过伴随表示和$_{\mathfrak{g}}$对$\mathfrak{g}$进行运算。

#### 命题 8 {#lie-vii-s1-prop-8 .statement tag=00SW}

设$\mathfrak{h}$为李代数，$L,M,N\mathfrak{h}$为模块。从$\mathfrak{h}$到$k$用映射的P集合表示。

(i) 和 $\sum_{\lambda\in P}L^{\lambda}(P)$ 是直接的。

(ii) 如果$f: L\rightarrow M$是$\mathfrak{h}$模块中的同态，则$f(L^{\lambda}(\mathfrak{h}))\subset M^{\lambda}(\mathfrak{h})$适用于所有$\lambda \in P$。

(iii) 如果$f: L\times M\rightarrow N$是双线性$\mathfrak{h}$不变量映射，

$$
f(L^{\lambda}(\mathfrak{h})\times M^\mu(\mathfrak{h}))\subset N^{\lambda+\mu}(\mathfrak{h})
$$

对于所有$\lambda , \mu\in P$。

这是从 Props 得出的。 2和3。

#### 命题 9 {#lie-vii-s1-prop-9 .statement tag=00SX}

设 $\mathfrak{h}$ 为幂零李代数，M 为有限维 $\mathfrak{h}$ 模。从$\mathfrak{h}$到$k$用映射的P集合表示。

(i) 每个$M^{\lambda}(\mathfrak{h})$都是M的$\mathfrak{h}$子模。如果$x_M$对于所有$x\in \mathfrak{h}$可三角化，则$M =\sum_{\lambda\in P}M^{\lambda}(\mathfrak{h})$。

(ii) 如果$k$是无限的，则存在$x\in \mathfrak{h}$使得$M^0(x) = M^0(\mathfrak{h})$。

(iii) 如果$k$的特征为0，并且如果$\lambda \in P$使得$M^{\lambda}(\mathfrak{h})\not= 0$，则$\lambda$是$\mathfrak{h}$上的线性形式，在$[\mathfrak{h},\mathfrak{h}]$和$M_{\lambda}(\mathfrak{h})\not= 0$上消失。

(iv) 如果$f: M\rightarrow N$是有限维$\mathfrak{h}$模的满同态，则$f(M^{\lambda}(\mathfrak{h})) = N^{\lambda}(\mathfrak{h})$对于所有$\lambda \in P$。

(v) 如果 N 是有限维 $\mathfrak{h}$ 模，并且 B 双线性形式在 $\mathfrak{h}$ 下的 $M\times N$ 上不变量，则 $M^{\lambda}(\mathfrak{h})$ 和 $N^\mu(\mathfrak{h})$ 相对于 B 正交（如果$\lambda +\mu\not= 0$）。此外，如果 B 是非简并的，那么对于所有 $\lambda \in P$，其限制到 $M^{\lambda}(\mathfrak{h})\times N^{-\lambda}(\mathfrak{h})$ 也是非简并的。

部分 (i) 由no. 1、引理 1 和 Th 得出。 1. 部分 (ii) 源自no. 2，第 7 条命题。 部分 (iv) 源自no. 1，第 7 条命题。 3 Th。 1. 我们证明(iii)。我们可以假设$M = M^{\lambda}(\mathfrak{h})$。然后，对于所有 $x\in \mathfrak{h},\lambda (x) =$ (dim $M$)$^{-1}$Tr($x_M$);这证明了 $\lambda$ 是线性的（这也是从命题 5 得出的）并且 $\lambda$ 在 $[\mathfrak{h},\mathfrak{h}]$ 上消失。考虑映射 $\rho :\mathfrak{h}\rightarrow$ End$_k(M)$ 定义为

$$
\rho (x) =x_M-\lambda (x)1_M
$$

由上可知，这是M上$\mathfrak{h}$的表示，并且$\rho (x)$对于所有$x\in \mathfrak{h}$来说是幂幂的。根据恩格尔的定理（第I, §4, no. 2，第1章），M中存在$m\not= 0$，使得$\rho (x)m= 0$对于所有$x\in \mathfrak{h}$，因此$m\in M_{\lambda}(\mathfrak{h})$。

(v) 的第一个断言源自命题 2 (ii) no. 1。为了证明第二个，我们可以假设$k$根据no. 1的命题1是代数封闭的；然后从第一个和$M =\sum_{\lambda}M^{\lambda}(\mathfrak{h}), N =\sum_{\lambda}N^{\lambda}(\mathfrak{h})$，cf. (i) 的事实得出结论。

#### 注 {#lie-vii-s1-n3-rem-1 .statement tag=00SY}

假设$k$是完美的并且具有特征2。设$\mathfrak{h}=\mathfrak{s}\mathfrak{l}(2, k)$，并且

$$
_2(ab)
$$

令 M 为$\mathfrak{h}$-模$k$（对于$\mathfrak{h}$的恒等式映射）。如果 $x=$ 是

$$
ca
$$

$\mathfrak{h}$的任意元素，用$\lambda (x)$表示唯一的$\lambda \in k$，使得$\lambda^2=a^2+bc$。计算立即表明$M = M^{\lambda}(\mathfrak{h})$；另一方面，$M_{\lambda}(\mathfrak{h}) = 0$和$\lambda$既不是线性的，也不是$[\mathfrak{h},\mathfrak{h}]$上的零，甚至虽然$\mathfrak{h}$也是幂零的。

#### 推论 {#lie-vii-s1-n3-cor-1 .statement tag=00SZ}

令 $\mathfrak{h}$ 为幂零李代数，且 M 为有限维 $\mathfrak{h}$ 模，使得 $M^0(\mathfrak{h}) = 0$。令 $f:\mathfrak{h}\rightarrow M$ 为线性映射，使得

$f([x, y]) =x.f(y)-y.f(x)$ 换$x, y\in \mathfrak{h}$。

存在 $a\in M$，使得 $f(x) =x.a$ 对于所有 $x\in \mathfrak{h}$。

让$N = M\times k$。让$\mathfrak{h}$在N上运行公式

$$
x.(m, \lambda ) = (x.m-\lambda f(x),0)
$$

$f$满足的恒等式意味着N是一个$\mathfrak{h}$模（第I, §1, no. 8，例2）。从N到$k$的映射$(m, \lambda ) \rightarrow \lambda$是从N到平凡的$\mathfrak{h}$-模块$k$的同态。根据提案 9 (iv)，可以得出形式 $(a,1)$ 与 $a\in M$ 的$N^0(\mathfrak{h})$ 包含元素。鉴于M上的假设，

$$
(M\times 0)\cap N^0(\mathfrak{h}) = 0
$$

所以 $N^0(\mathfrak{h})$ 是维数 1，因此被 $\mathfrak{h}$ 湮灭。因此，$x.a-f(x) = 0$对于所有$x\in \mathfrak{h}$，这证明了推论。

#### 命题 10 {#lie-vii-s1-prop-10 .statement tag=00T0}

令$\mathfrak{g}$为李代数，$\mathfrak{h}$是$\mathfrak{g}$的幂零子代数。用从$\mathfrak{h}$到$k$的映射的P集合来表示。

(i) 对于$\lambda , \mu\in P$、$[\mathfrak{g}^{\lambda}(\mathfrak{h}),\mathfrak{g}^\mu(\mathfrak{h})]\subset \mathfrak{g}^{\lambda+\mu}(\mathfrak{h})$；特别是，$\mathfrak{g}^0(\mathfrak{h})$是$\mathfrak{g}$包含$\mathfrak{h}$的谎言子代数，并且$\mathfrak{g}^{\lambda}(\mathfrak{h})$在广告$\mathfrak{g}^0(\mathfrak{h})$下是稳定的。此外，$\mathfrak{g}^0(\mathfrak{h})$是$\mathfrak{g}$中自己的标准化器。

(ii) 如果 M 是 $\mathfrak{g}$ 模，$\mathfrak{g}^{\lambda}(\mathfrak{h})M^\mu(\mathfrak{h})\subset M^{\lambda+\mu}(\mathfrak{h})$ 代表 $\lambda , \mu\in P$；特别是，每个$M^{\lambda}(\mathfrak{h})$都是一个$\mathfrak{g}^0(\mathfrak{h})$模块。

(iii) 如果 B 在 $\mathfrak{g}$ 上是双线性形式，则$\mathfrak{h},\mathfrak{g}^{\lambda}(\mathfrak{h})$ 和 $\mathfrak{g}^\mu(\mathfrak{h})$ 不变量相对于$\lambda +\mu\not= 0$ 的 B 正交。假设 B 是非简并的。那么，对于所有$\lambda \in P$，B到$\mathfrak{g}^{\lambda}(\mathfrak{h})\times \mathfrak{g}^{-\lambda}(\mathfrak{h})$的限制都是非简并的；特别是，B 到 $\mathfrak{g}^0(\mathfrak{h})\times \mathfrak{g}^0(\mathfrak{h})$ 的限制是非简并的。

(iv) 假设$k$的特征为0。那么，如果$x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$和$\lambda \not= 0$，则$x$幂零的。

根据雅可比恒等式，映射$(x, y) \rightarrow [x, y]$从$\mathfrak{g}\times \mathfrak{g}$到$\mathfrak{g}$是$\mathfrak{g}$不变的，因此$\mathfrak{h}$是不变的。因此，(i) 的第一个部分由命题 2 (ii) 得出。 部分 (ii) 类似地证明。

如果 $x$ 属于为 $\mathfrak{g}$ 中 $\mathfrak{g}^0(\mathfrak{h})$ 的归一化器，则 (ad $y$)$.x=-[x, y]\in \mathfrak{g}^0(\mathfrak{h})$ 对于所有 $y\in \mathfrak{h}$，因此 (ad $y$)$^n.x= 0$ 对于 $n$ 足够大。这就证明了$x\in \mathfrak{g}^0(\mathfrak{h})$。 断言 (i) 现已完全证明。

断言 (iii) 源自提案 9 (v)。

为了证明(iv)，我们可以假设$k$是代数封闭的。让$x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$，与$\lambda \not= 0$。对于所有$\mu\in P$和任何整数$n\geq 0$，（广告$x$）$^n\mathfrak{g}^\mu(\mathfrak{h})\subset \mathfrak{g}^{\mu+n\lambda}(\mathfrak{h})$；令$P_1$为$\mu\in P$的有限集合，使得$\mathfrak{g}^\mu(\mathfrak{h})\not= 0$；如果 $k$ 的特征为 0，$\lambda \not= 0, (P_1+n\lambda )\cap P_1=\emptyset$ 的特征为 $n$ 足够大，则 (ad $x$)$^n= 0$。

#### 引理 2 {#lie-vii-s1-lem-2 .statement tag=00T1}

假设$k$的特征为0。令$\mathfrak{g}$比$k$为半单李代数，B为$\mathfrak{g}$的$\mathfrak{g},\mathfrak{m}$子代数的杀戮形式。假设满足以下条件：

1) B 到 $\mathfrak{m}$ 的限制是非简并的；

2) 如果$x\in \mathfrak{m}$、半单以及$x$的幂零分量$^1$位于$\mathfrak{g}$、属于至$\mathfrak{m}$。

然后$\mathfrak{m}$在$\mathfrak{g}$中被还原（第I, § 6, no. 6章）。

由章。 I, §6, no. 4，命题$5d),\mathfrak{m}$ 是还原性的。令 $\mathfrak{c}$ 为 $\mathfrak{m}$ 中的中心。如果$x\in \mathfrak{c}$幂零，则$x= 0$；事实上，对于所有 $y\in \mathfrak{m}$、ad $x$ 和 ad $y$ 通勤，它们的合成、ad $x\circ$、ad $y$ 是幂零的，而 $B(x, y) = 0$，因而 $x= 0$。现在让 $x$ 为 $\mathfrak{c}$ 的任意元素；设$s$和$n$为其半单和幂零分量。我们有$n\in \mathfrak{m}$。由于 ad $n$ 是形式 P(ad $x$)，其中 P 是没有常数项的多项式，(ad $n$)$.\mathfrak{m}= 0$ 等等 $n\in \mathfrak{c}$，然后通过上面的 $n= 0$。因此广告$x$是半单。因而，$\mathfrak{g}$的伴随表示的限制到$\mathfrak{m}$是半单（第I, §6, no. 5，第$4b$）$)$。

#### 命题 11 {#lie-vii-s1-prop-11 .statement tag=00T2}

假设$k$的特征为0。令$\mathfrak{g}$为半单李代数，$\mathfrak{h}$为$\mathfrak{g}$的幂零子代数。 代数$\mathfrak{g}^0(\mathfrak{h})$满足引理2的条件(1)和(2)；它在 $\mathfrak{g}$ 中是还原的。

$^1$ 作者： I, §6, no. 3，周四。 3、每个$x\in \mathfrak{g}$可以唯一地写为互通的半单元素$s$和幂零元$n$的和； 元素 $s$（分别为 $n$）被称为半单（分别为幂零） $x$ 的分量。

设$x, x'\in \mathfrak{g},s$和$s'$为它们的半单分量，$n$和$n'$为它们的幂零分量。我们有

$x'\in \mathfrak{g}^0(x)\Leftarrow \Rightarrow$（广告$s$）$(x') = 0$（提案$.4$）

$\Leftarrow \Rightarrow$（广告$x'$）$(s) = 0$

$=\Rightarrow$（广告$s'$）$(s) = 0$

$\Leftarrow \Rightarrow$（广告$s$）$(s') = 0$

$\Leftarrow \Rightarrow s'\in \mathfrak{g}^0(x)$（提案$.4$）

故$x'\in \mathfrak{g}^0(x)\Rightarrow n'\in \mathfrak{g}^0(x)$且(2)得证。 $\mathfrak{g}$的杀戮形式是非简并的，因此它的限制到$\mathfrak{g}^0(\mathfrak{h})$是非简并的（命题10（iii））。 $\mathfrak{g}^0(\mathfrak{h})$ 在 $\mathfrak{g}$ 中被还原，因此从引理 2 得出。

### 4. 李代数的分解相对于自同构

#### 命题 12 {#lie-vii-s1-prop-12 .statement tag=00T3}

令 $\mathfrak{g}$ 为李代数，$a$ 自同构 of $\mathfrak{g}$。

(i) $\lambda , \mu\in k,[\mathfrak{g}^{\lambda}(a),\mathfrak{g}^\mu(a)]\subset \mathfrak{g}^{\lambda \mu}(a)$；特别地，$\mathfrak{g}^1(a)$是$\mathfrak{g}$的子代数。

(ii) 如果 B 是 $\mathfrak{g}$ 上的对称双线性形式，则$a,\mathfrak{g}^{\lambda}(a)$ 和 $\mathfrak{g}^\mu(a)$ 相对于$\lambda \mu\not= 1$ 的 B 正交。假设 B 是非简并的。那么，如果$\lambda \not= 0$，则B到$\mathfrak{g}^{\lambda}(a)\times \mathfrak{g}^{1/\lambda}(a)$的限制是非简并的。

断言 (i) 和 (ii) 的前半部分源自应用于合成律 $\mathfrak{g}\times \mathfrak{g}\rightarrow \mathfrak{g}$ 和双线性形式 B 的命题 2 (iii)。为了证明 (ii) 的后半部分，我们可以假设 $k$ 是代数封闭的。然后$\mathfrak{g}=\bigoplus_{\nu\in k}\mathfrak{g}^{\nu}(a)$。由上可知，如果$\lambda \nu \not= 1$，则$\mathfrak{g}^{\lambda}(a)$与$\mathfrak{g}^{\nu}(a)$正交；由于 B 是非简并的，因此它的限制到 $\mathfrak{g}^{\lambda}(a)\times \mathfrak{g}^{1/\lambda}(a)$ 也是非简并的。

#### 推论{#lie-vii-s1-n4-cor-1 .statement tag=00T4}

假设$k$是特征零，$\mathfrak{g}$是半单。那么子代数$\mathfrak{g}^1(a)$满足引理2的条件(1)和(2)；它在 $\mathfrak{g}$ 中是还原的。

条件(1)源自第12号提案的部分(ii)； 条件 (2) 由no. 1 的第 4 条命题得出。

### 5. 半单李代数相对于半单作用的不变量

在这个数中，假设$k$为特征零。

#### 命题 13 {#lie-vii-s1-prop-13 .statement tag=00T5}

令$\mathfrak{g}$为半单李代数，$\mathfrak{g}$中$\mathfrak{g}$的约简$\mathfrak{a}$子代数，$\mathfrak{m}$为$\mathfrak{g}$中$\mathfrak{a}$的交换子。 子代数$\mathfrak{m}$满足no. 3的引理2的条件(1)和(2)；它在 $\mathfrak{g}$ 中是还原的。

根据第 6 章的提案。 I, §3, no. 5，应用于$\mathfrak{a}$模块$\mathfrak{g}$，我们有$\mathfrak{g}=\mathfrak{m}\oplus [\mathfrak{a},\mathfrak{g}]$。设B为$\mathfrak{g}$的杀戮形式，并设$x\in \mathfrak{a}, y\in \mathfrak{m}, z\in \mathfrak{g}$。然后，

$B([z, x], y) = B(z,[x, y]) = 0$ 自$[x, y] = 0$以来，

这表明$\mathfrak{m}$相对于B与$[\mathfrak{a},\mathfrak{g}]$正交。由于B是非简并的，并且从$\mathfrak{g}=\mathfrak{m}\oplus [\mathfrak{a},\mathfrak{g}]$开始，这意味着B到$\mathfrak{m}$的限制是非简并的；由此满足引理2的条件(1)。

现在令$x\in \mathfrak{m}$、$s$和$n$为其半单和幂零分量。广告$x$的半单组成部分是广告$s$、cf. I, §6, no. 3。由于广告 $x$ 在 $\mathfrak{a}$ 上是零，根据提案 4 (i)，广告 $s$ 也是如此。因此$s\in \mathfrak{m}$，所以$n=x-s\in \mathfrak{m}$，并且满足引理2的条件(2)。

#### 注{#lie-vii-s1-n5-rem-1 .statement tag=00T6}

$\mathfrak{g}$中$\mathfrak{m}$的交换子不一定是约化到$\mathfrak{a}$，cf.Exerc。 4.

#### 命题 14 {#lie-vii-s1-prop-14 .statement tag=00T7}

令 $\mathfrak{g}$ 为半单李代数、A 群和 $r$ 同态，从 A 到 Aut($\mathfrak{g}$)。令$\mathfrak{m}$为$\mathfrak{g}$的子代数，元素的由……组成在$r(A)$下不变。假设线性表示$r$为半单。则$\mathfrak{m}$满足no. 3的引理2的条件(1)和(2)；它在 $\mathfrak{g}$ 中被还原。

证明与前面的命题类似：

令$\mathfrak{g}^+$为由$r(a)x-x,a\in A, x\in \mathfrak{g}$生成的$\mathfrak{g}$的向量子空间。 向量空间$\mathfrak{g}'=\mathfrak{m}+\mathfrak{g}^+$在$r(A)$下稳定。设$\mathfrak{n}$是$\mathfrak{g}'$的补集，在$\mathfrak{g}$稳定在$r(A)$下。如果$x\in \mathfrak{n}, a\in A,r(a)x-x\in \mathfrak{n}\cap \mathfrak{g}^+= 0$，那么$x\in \mathfrak{m}$，然后从$\mathfrak{m}\cap \mathfrak{n}= 0$开始$x= 0$。因此，$\mathfrak{g}=\mathfrak{g}'=\mathfrak{m}+\mathfrak{g}^+$。设 B 为 $\mathfrak{g}$ 的杀戮形式，并令 $y\in \mathfrak{m}, a\in A, x\in \mathfrak{g}$。然后

$$
B(y, r(a)x-x) = B(y, r(a)x)-B(y, x)
$$

$$
= B(r(a^{-1})y, x)-B(y, x)
$$

$$
= B(y, x)-B(y, x) = 0
$$

因此$\mathfrak{m}$和$\mathfrak{g}^+$相对于B是正交的。因此B到$\mathfrak{m}$的限制是非简并的；因此，引理 2 中的条件 (1)。条件 (2) 是直接的迁移结构。

### 习题 {#lie-vii-s1-exercises}

它们上的所有李代数和模均假定为 $k$ 上的有限维；从§3开始，$k$被假定为特征零。

请参阅 § 1](exercises/s1/) 的 [习题。
