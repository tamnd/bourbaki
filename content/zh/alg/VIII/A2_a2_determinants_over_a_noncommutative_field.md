---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 2
section_title: Determinants over a Noncommutative Field
appendix: true
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.447-A VIII.460
pdf_pages: 0464-0477
extraction: native
subsections:
    - "no": 1
      title: A Generalization of Alternating Multilinear Forms
      page: 447
      pdf_page: 464
    - "no": 2
      title: A Uniqueness Theorem
      page: 448
      pdf_page: 465
    - "no": 3
      title: Determinant of an Automorphism
      page: 452
      pdf_page: 469
    - "no": 4
      title: Determinant of a Square Matrix
      page: 452
      pdf_page: 469
    - "no": 5
      title: The Unimodular Group
      page: 455
      pdf_page: 472
statements: 18
exercises: 4
content_sha256: 0226d6606dde26e328c295b9a60cbead7c818364825aa5aad9af7081c739d39c
translated_from: content/en/alg/VIII/A2_a2_determinants_over_a_noncommutative_field.md
translation_method: google
source_content_sha256: a1a346c55a436d2ed8247c3e3a5bc5302eaac2c7930a98ff5617acbf65dc1b0e
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 441cc7fb2bb2d30e38f944776e03cead7241b2e38549bfb49a6c417e34d224f4
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 附录 2 个超过非交换域的决定因素

在这个附录中，D是域，$D^*_{ab}$是D的乘法群$D^*$除以它的导出群的商（I, §6, No. 2，p. 70）。 群 $D^*_{ab}$ 是可交换的，如果域 D 是可交换的，$D^*_{ab}$ 可以与 $D^*$ 等价。我们用$\pi$表示从$D^*$到$D^*_{ab}$的典范同态。

### 1. 推广 / 交替多重线性形式

令 V 为右向量空间超过域 D，即有限维 $n\geqslant 0$。我们用V的基的B(V)集合和映射$\omega$的Ω(V)集合从B(V)到$D^*_{ab}$表示满足以下两个条件：

a) 如果 $\lambda_1, . . . , \lambda_n$ 是 $D^*$ 的元素，那么我们有

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) =\pi (\lambda_1\cdots \lambda_n)\omega (v_1, . . . , v_n) \tag{1}
$$

对于 V 中的每基 $(v_1, . . . , v_n)$。

b) 如果$i$和$j$是区间$[1, n]$中的两个不同整数，那么我们有

$$
\omega (v_1, . . . , v_{i-1}, v_i+v_j, v_{i+1}, . . . , v_n) =\omega (v_1, . . . , v_n) \tag{2}
$$

每基 $(v_1, . . . , v_n)$ 共 V。

设 $\omega$ 为 Ω(V) 的元素。令$(v_1, . . . , v_n)$为区间$[1, n-1]$中V和$i$整数的基；到性质 b)，我们有

$$
\omega (v_1, . . . , v_i, v_{i+1}, . . . , v_n) =\omega (v_1, . . . , v_i+v_{i+1}, v_{i+1}, . . . , v_n)
$$

$$
=\omega (v_1, . . . , v_i+v_{i+1}, v_{i+1}-(v_i+v_{i+1}), . . . , v_n)
$$

$$
=\omega (v_1, . . . , v_i+v_{i+1},-v_i, . . . , v_n)
$$

$$
=\omega (v_1, . . . ,(v_i+v_{i+1})-v_i,-v_i, . . . , v_n)
$$

因此

$$
\omega (v_1, . . . , v_i, v_{i+1}, . . . , v_n) =\pi (-1)\omega (v_1, . . . , v_{i+1}, v_i, . . . , v_n) \tag{3}
$$

由于对称群$\mathfrak{S}_n$是由间隔$[1, n]$（I, §5, No. 7，p. 63，命题9）的两个连续元素转置生成的，公式（3）推广为

$$
\omega (v_{\sigma(1)}, . . . , v_{\sigma(n)}) =\pi (\varepsilon (\sigma ))\omega (v_1, . . . , v_n) \tag{4}
$$

其中$\sigma$属于到$\mathfrak{S}_n$和$\varepsilon (\sigma )$是它的签名（I, §5, No. 7，p. 64）。

公式 (2) 概括如下。首先，对于$D^*$中的每个$\lambda$，我们有

$$
\omega (v_1, . . . , v_n) =\pi (\lambda )\omega (v_1, . . . , v_i\lambda^{-1}, . . . , v_n)
$$

$$
=\pi (\lambda )\omega (v_1, . . . , v_i\lambda^{-1}+v_j, . . . , v_n)
$$

$$
=\omega (v_1, . . . ,(v_i\lambda^{-1}+v_j)\lambda , . . . , v_n)
$$

也就是说，

$$
\omega (v_1, . . . , v_n) =\omega (v_1, . . . , v_i+v_j\lambda , . . . , v_n) \tag{5}
$$

由直接的归纳，我们推出

$$
\omega (v_1, . . . , v_n) =\omega (v_1, . . . , v_i+w, . . . , v_n) \tag{6}
$$

对于 $j$ 的向量 $v_j$ 中的每个线性组合 $w=\sum_{j\not=i}v_j\lambda_j$ 与间隔 $[1, n]$ 中的$i$ 不同。

### 2. 唯一性定理

在这个小节中，对于任何严格的正整数$m$，任何$[1, m]$中的整数$i$，以及$V^m$中的任何序列$(v_1, . . . , v_m)$，我们将$(v_1, . . . ,\widehat{v}_i, . . . , v_m)$写为序列$(v_1, . . . , v_{i-1}, v_{i+1}, . . . , v_m)$在$V^{m-1}$。

#### 命题 1 {#alg-viii-a2-prop-1 .statement tag=00Q1}

设W为V中的超平面，$e$为V-W中的向量。令$\varphi$为Ω(W)的元素。存在 Ω(V) 的唯一元素 $\omega$ 使得我们有

$$
\omega (w_1, . . . , w_{n-1}, e) =\varphi (w_1, . . . , w_{n-1}) \tag{7}
$$

每基 $(w_1, . . . , w_{n-1})$ W。

A) $\omega :$ 的唯一性令 $\omega$ 为 Ω(V) 的元素。令$(v_1, . . . , v_n)$为V的基，令$\mu_1, . . . , \mu_n$为$e$在此基中的坐标。用整数的 I 集合表示从 1 到 $n$（含），使得 $\mu_i\not= 0$；它不是空的。设$i$为I中的元素。 序列$(v_1, . . . ,\widehat{v}_i, . . . , v_n, e)$是V的基，并且由于$e-v_i\mu_i$是序列$(v_1, . . . ,\widehat{v}_i, . . . , v_n)$的线性组合，所以公式(6)意味着

$$
\omega (v_1, . . . ,\widehat{v}_i, . . . , v_n, v_i\mu_i) =\omega (v_1, . . . ,\widehat{v}_i, . . . , v_n, e) \tag{8}
$$

从公式 (1) 和 (3) 可以看出，等式的左侧等于 $\pi (-1)^{n-i}\pi (\mu_i)\omega (v_1, . . . , v_n)$。用V的$p$投影算子和像W和核$eD$表示。 向量$v_j-p(v_j)$与$e$成正比，重复应用公式(6)可知公式(8)的右边等于$\omega (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n), e)$。

由此可见，如果 $\omega$ 满足关系 (7)，那么我们有

$$
\omega (v_1, . . . , v_n) =\pi (-1)^{n-i}\pi (\mu_i)^{-1}\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n)) \tag{9}
$$

对于I中的每个$i$，这证明唯一性等于$\omega$。

B) $\omega :$ 的构造令$(v_1, . . . , v_n)$ 为V 的基；我们定义$\mu_1, . . . , \mu_n$和I如上所述。对于I中的每个$i$，假设$\mu_i\not= 0$意味着序列$(v_1, . . . ,\widehat{v}_i, . . . , v_n, e)$生成空间V，所以序列$(p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n))$生成空间$W =p(V)$。在其他字中，最后一个序列是W的基，并且

$$
t_i=\pi (-1)^{n-i}\pi (\mu_i)^{-1}\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n)) \tag{10}
$$

定义元素共$D^*_{ab}$。

令$i$和$j$为I中的两个元素，使得$i < j$；让我们证明等式$t_i=t_j$。通过定义，向量$v_i\mu_i+v_j\mu_j-e$是$k$的向量$p(v_k)$中的线性组合，与$i$和$j$不同。因而，对于$k$，$p(v_i)\mu_i+p(v_j)\mu_j$ 是向量 $p(v_k)$ 的线性组合，与$i$ 和$j$ 不同。到公式 (6)，我们有

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . ,p(\widehat{v}_j), . . . , p(v_n), p(v_i)\mu_i)
$$

$$
=\varphi (p(v_1), . . . ,p(\widehat{v}_i), . . . ,p(\widehat{v}_j), . . . , p(v_n),-p(v_j)\mu_j)
$$

由应用公式 (1) 和 (3)，我们推出

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_j), . . . , p(v_n))\pi (\mu_i)\pi (-1)^{n-i-1}
$$

$$
=\varphi (p(v_1), . . . ,\widehat{p}(v_i), . . . , p(v_n))\pi (-\mu_j)\pi (-1)^{n-j}
$$

因而$t_i=t_j$。

证明了这一点，我们将I中$i$的$t_i$的公共的值视为定义$\omega (v_1, . . . , v_n)$。因此，我们从 B(V) 到$D^*_{ab}$构造了映射$\omega$，满足关系(9)。设$(w_1, . . . , w_{n-1})$为W的基；如果我们对$1\leqslant i\leqslant n-1$和$v_n=e$进行集合$v_i=w_i$，那么我们就有$I =\{n\}$和$\mu_n= 1$。此外，对于$1\leqslant i\leqslant n-1$，我们还有$p(v_i) =w_i$，而公式$\omega (w_1, . . . , w_{n-1}, e) =\varphi (w_1, . . . , w_{n-1})$是（9）的一个特例。

我们现在必须证明 $\omega$ 属于到 Ω(V)。

C)公式的证明 (1)：令$\lambda_1, . . . , \lambda_n$为$D^*$的元素，且$(v_1, . . . , v_n)$为V的基。我们定义$\mu_1, . . . , \mu_n$和I如上所述。 选择 $i$ I。由于我们有 $e=\sum^n_{j=1}(v_j\lambda_j)(\lambda^{-1}_j\mu_j)$，公式 (9) 意味着

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) \tag{11}
$$

$$
=\pi (-1)^{n-i}\pi (\lambda^{-1}_i\mu_i)^{-1}\varphi (p(v_1)\lambda_1, . . . ,\widehat{p(v_i)\lambda_i}, . . . , p(v_n)\lambda_n)
$$

但我们有 $\pi (\lambda^{-1}_i\mu_i)^{-1}=\pi (\mu_i)^{-1}\pi (\lambda_i)$ 并且

$$
\varphi (p(v_1)\lambda_1, . . . ,\widehat{p(v_i)\lambda_i}, . . . , p(v_n)\lambda_n)
$$

$$
=\varphi (p(v_1), . . . ,\widehat{p(v_i)}, . . . , p(v_n))\pi (\lambda_1. . .\widehat{\lambda}_i. . . \lambda_n)
$$

比较公式 (9) 和 (11) 得到所需的关系

$$
\omega (v_1\lambda_1, . . . , v_n\lambda_n) =\omega (v_1, . . . , v_n)\pi (\lambda_1. . . \lambda_n)
$$

D) 公式证明 (2): 设$(v_1, . . . , v_n)$为V的基，且$i, j$为区间$[1, n]$中的两个不同整数；我们定义$\mu_1, . . . , \mu_n$为之前。考虑$v'_i=v_i+v_j$和$v'_k=v_k$对$k\not=i$定义的V的基$(v'_1, . . . , v'_n)$，让我们介绍$e$相对于这个基的坐标$\mu'_1, . . . , \mu'_n$；他们满足$\mu'_j=\mu_j-\mu_i$和$\mu'_k=\mu_k$$k\not=j$。我们集合$t=\omega (v_1, . . . , v_n)$和$t'=\omega (v'_1, . . . , v'_n)$。我们必须证明认为$t$和$t'$是相等的。

让我们首先注，通过$\omega$的定义，我们有

$$
t=\pi (-1)^{n-k}\pi (\mu_k)^{-1}\varphi (p(v_1), . . . ,\widehat{p(v_k)}, . . . , p(v_n)) \tag{12}
$$

$$
t'=\pi (-1)^{n-k}\pi (\mu'_k)^{-1}\varphi (p(v'_1), . . . ,\widehat{p(v'_k)}, . . . , p(v'_n)) \tag{13}
$$

对于每个$k$，使得$\mu_k$和$\mu'_k$是非零的。

a) 如果$\mu_i\not=0$，则序列、$(p(v_1), . . . ,\widehat{p(v_k)}, . . . , p(v_n))$和$(p(v'_1), . . . ,\widehat{p(v'_k)}, . . . , p(v'_n))$相等，并且我们有$\mu_i$ = $\mu'_i$，因此$t=t'$。

b) 如果存在与$i$和$j$不同的指标$k$使得$\mu_k\not= 0$，那么对于$l\not=i$和$p(v'_i) =p(v_i) +p(v_j)$我们有$p(v'_l) =p(v_l)$。 元素$p(v_i)$和$p(v_j)$均为属于至序列$(p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n))$。从 $\varphi$ 属于到 Ω(W)，公式 (2) of VIII、p. 447 适用；它给了

$$
\varphi (p(v_1), . . . ,p(\widehat{v}_k), . . . , p(v_n)) =\varphi (p(v'_1), . . . ,p(\widehat{v}'_k), . . . , p(v'_n))
$$

但我们还有 $\mu_k=\mu'_k$，因此也有 $t=t'$。

c) 当唯一的指标$k$使得$\mu_k\not= 0$是$j$时，仍然需要检查这种情况。然后我们就有$\mu'_j=\mu_j,e=v_j\mu_j$和$p(v_j) = 0$。 集合$k=j$在公式（12）和（13）中。由于序列 $(p(v_1), . . . ,p(\widehat{v}_j), . . . , p(v_n))$ 和 $(p(v'_1), . . . ,p(\widehat{v}'_j), . . . , p(v'_n))$ 相等，因此我们有 $t=t'$。

#### 推论 1 {#alg-viii-a2-prop-1-cor-1 .statement tag=00Q2}

令$(e_1, . . . , e_n)$为V之基，且$t$元素为$D^*_{ab}$。存在 Ω(V) 的唯一元素 $\omega$，使得 $\omega (e_1, . . . , e_n) =t$。

让我们用归纳在$n$上证明这个推论。如果$n= 0$，那么V中唯一的基是空的，所以断言为真。现在假设$n\geqslant 1$；表示由$e_1, . . . , e_{n-1}$生成的V的W子空间。到命题 1，存在从 Ω(V) 到 Ω(W) 满足的双射 Λ

$$
(\Lambda (\omega ))(w_1, . . . , w_{n-1}) =\omega (w_1, . . . , w_{n-1}, e_n)
$$

对于 W 的每基 $(w_1, . . . , w_{n-1})$ 和 Ω(V) 中的每 $\omega$。到归纳假设时，存在 Ω(W) 的唯一元素 $\varphi$，使得 $\varphi (e_1, . . . , e_{n-1}) =t$。 关系 $\omega (e_1, . . . , e_n) =t$，对于 Ω(V) 中的 $\omega$，相当于 $\Lambda (\omega ) =\varphi$。推论 1 如下。

#### 推论 2 {#alg-viii-a2-prop-1-cor-2 .statement tag=00Q3}

令$\omega$和$\omega '$为Ω(V)的两个元素。存在$D^*_{ab}$的唯一元素$t$使得$\omega '=t\omega$。

#### 注 {#alg-viii-a2-n2-rem-1 .statement tag=00Q4}

假设域 D 是可交换的。到定义时，B(V) 是子集 / $V^n$。显然，非零的交错的$n$的限制到B(V)-线性形式$f: V^n\rightarrow D$属于到Ω(V)。此外，如果$(e_1, . . . , e_n)$是V的基并且$t$是D的非零元素，则存在唯一的交错的$n$线性形式$f$使得$f(e_1, . . . , e_n) =t$(III, §7, No. 4， p. 511 和 III, §7, No. 8、p. 518）。根据推论 1，集合 Ω(V) 由非零的交错的 $n$ 的线性形式限制到 B(V) 组成。

### 3. 自同构的行列式

我们首先假设域 D 是可交换的。鉴于上面的注，V的自同构$u$的行列式是唯一元素 det $u$ of $D^*$，这样我们有

(14)$\omega (u(v_1), . . . , u(v_n)) =$（不含$u$）$\omega (v_1, . . . , v_n)$

对于V的每个基$(v_1, . . . , v_n)$和Ω(V)的每个元素$\omega$。

让我们回到 D 不再可交换的情况。

#### 命题 2 {#alg-viii-a2-prop-2 .statement tag=00Q5}

a) 设$u$为V中的自同构。 $D^*_{ab}$存在唯一元素，记为det$u$，称为$u$的行列式，这样我们有

(15)$\omega (u(v_1), . . . , u(v_n)) =$（不含$u$）$\omega (v_1, . . . , v_n)$

对于V的每个基$(v_1, . . . , v_n)$和Ω(V)中的每个$\omega$。

b) 映射 $u\mapsto$ 从 $\mathbf{G}\mathbf{L}(V)$ 到 $D^*_{ab}$ 的 $u$ 为群同态。

设 $\omega_0$ 为 Ω(V) 的元素。 映射$(v_1, . . . , v_n)\mapsto$$\omega_0(u(v_1), . . . , u(v_n))$从B(V)到$D^*_{ab}$属于到Ω(V)。根据VIII、p. 451的推论2，存在$D^*_{ab}$的唯一元素$t$，使得我们有

$$
\omega_0(u(v_1), . . . , u(v_n)) =t\omega_0(v_1, . . . , v_n)
$$

对于 B(V) 中的 $(v_1, . . . , v_n)$。如果 $\omega$ 是 Ω(V) 的另一个元素，则存在 $D^*_{ab}$ 的元素 $s$，使得

$$
\omega (v_1, . . . , v_n) =s\omega_0(v_1, . . . , v_n)
$$

对于 V 中的每基 $(v_1, . . . , v_n)$（前述）。我们立即推导出关系

$$
\omega (u(v_1), . . . , u(v_n)) =t\omega (v_1, . . . , v_n)
$$

这证明了a）； 断言 b) 是 a) 的直接的推论。

### 4. 平方矩阵的行列式

令$n$为正整数。让我们将上述应用于右向量空间$D^n_d$超过域D； $D^n_d$ 中的元素被视为具有 $n$ 行和一个列的矩阵。令$(\varepsilon_1, . . . , \varepsilon_n)$为$D^n_d$中的典范基。根据VIII、p. 451的推论2，存在$\Omega (D^n_d)$的唯一元素$\omega_0$使得$\omega_0(\varepsilon_1, . . . , \varepsilon_n) = 1$。如果A是$\mathbf{G}\mathbf{L}_n$(D)的元素，那么它的$D^n_d$的列$a_1, . . . , a_n$形式基； $D^*_{ab}$的元素$\omega_0(a_1, . . . , a_n)$称为A的行列式，记为det(A)。由于 $1\leqslant i\leqslant n$ 有 $a_i=A\varepsilon_i$，因此 A 的行列式就是自同构 $x\mapsto Ax$ 和 $D^n_d$ 的行列式。特别地，如果域 D 是可交换的，则重合的行列式与III, §8, No. 3、p. 524 中定义的行列式相同。

令V为有限维$n$在域D上的右向量空间，并令$(e_1, . . . , e_n)$为V的基。如果$u$是V的自同构，并且A是$u$的矩阵，相对于基$(e_1, . . . , e_n)$，那么我们有det($u$)$=$det(A)。

我们用（$E_{ij}$）表示$\mathbf{M}_n(D)$（II, §10, No. 3，p. 341）的矩阵单位家族。对于 D 中的每个元素 $\lambda$ 和 $[1, n]$ 中不同整数的每个对 $(i, j)$，我们集合 (II, §10, No. 13, p. 361)

$$
B_{ij}(\lambda ) =I_n+\lambda E_{ij}
$$

它是 $\mathbf{G}\mathbf{L}_n(D)$ 中的元素。如果$\lambda_1, . . . , \lambda_n$是$D^*$的元素，则对角矩阵 diag($\lambda_1, . . . , \lambda_n$)也属于到$\mathbf{G}\mathbf{L}_n(D)$。

#### 命题 3 {#alg-viii-a2-prop-3 .statement tag=00Q6}

映射 det 是从$\mathbf{G}\mathbf{L}_n(D)$到$D^*_{ab}$的唯一同态，满足关系

（16）det（$B_{ij}(1)$）$= 1$

对于 $i\not=j$ 和

(17) det(诊断($\lambda_1, . . . , \lambda_n$)) $=\pi (\lambda_1\cdots \lambda_n)$,

$\lambda_1, . . . , \lambda_n\in D^*$

设 A 为 $\mathbf{G}\mathbf{L}_n(D)$ 的元素，$a_1, . . . , a_n$ 为其列。我们有

检测（A）$=\omega_0(a_1, . . . , a_n)$。

现在，矩阵 A diag($\lambda_1, . . . , \lambda_n$) 的列为 $a_1\lambda_1, . . . , a_n\lambda_n$，因此矩阵 AB$_{ij}(1)$ 的$a_1, . . . , a_j+a_i, a_{j+1}, . . . , a_n$。由于$\omega_0$是$\Omega (D^n_d)$的唯一元素使得$\omega_0(\varepsilon_1, . . . , \varepsilon_n) = 1$，我们看到行列式是满足关系的唯一映射$\varphi :\mathbf{G}\mathbf{L}_n(D)\rightarrow D^*_{ab}$

(18) $\varphi ($A 诊断($\lambda_1, . . . , \lambda_n$)) $=\varphi ($A$)\pi (\lambda_1\cdots \lambda_n)$,

(19) $\varphi ($AB$_{ij}(1)) =\varphi ($A) $i\not=j$，

$$
\varphi (I_n) = 1 \tag{20}
$$

这首先证明行列式映射满足关系（16）和（17）。我们已经知道这个映射是从$\mathbf{G}\mathbf{L}_n(D)$到$D^*_{ab}$的同态。相反，如果 $\varphi$ 是从 $\mathbf{G}\mathbf{L}_n(D)$ 到 $D^*_{ab}$ 的同态，使得 $\varphi (B_{ij}(1)) = 1$ 对于 $i\not=j$ 和 $\varphi$(diag($\lambda_1, . . . , \lambda_n$)) $=\pi (\lambda_1\cdots \lambda_n)$，则 $\varphi$ 满足关系 (18) 到 (20)，因此等于 det。

#### 例 1 {#alg-viii-a2-n4-exa-1 .statement tag=00Q7}

列 / 矩阵 $B_{ij}(\lambda )$ 是 $\varepsilon_1, . . . , \varepsilon_j$ + $\varepsilon_i\lambda , \varepsilon_{i+1}, . . . , \varepsilon_n$。到VIII、p. 448的公式(5)，我们有

（21）det（$B_{ij}(\lambda )$）$= 1$。

#### 例 2 {#alg-viii-a2-n4-exa-2 .statement tag=00Q8}

令$\sigma$为$\mathbf{N}$中区间$[1, n]$的置换，签名为$\varepsilon (\sigma )$。令M$(\sigma )$为置换$\sigma$（II, §10, No. 7，p. 351）中的矩阵。 矩阵 M$(\sigma )$ 中的列为 $\varepsilon_{\sigma(1)}, . . . , \varepsilon_{\sigma(n)}$。 应用公式 (4) of VIII, p. 448，因此有

（22）det（M$(\sigma )$）$=\pi (\varepsilon (\sigma ))$。

#### 例 3 {#alg-viii-a2-n4-exa-3 .statement tag=00Q9}

假设$n\geqslant 1$。对于形式 Δ = diag($d_1, . . . , d_n$) 的每个可逆对角矩阵，我们有 Δ$B_{ij}(\lambda$)Δ$^{-1}=B_{ij}(d_i\lambda d^{-1}_j)$。设 A 为 $\mathbf{G}\mathbf{L}_n(D)$ 的元素。由II, §10, No. 13、p. 362的推论1和前面的公式，$\mathbf{G}\mathbf{L}_n(D)$中存在矩阵 P和Δ，使得A = PΔ，则P为形式$B_{ij}(\lambda )$的矩阵的乘积，且Δ为对角矩阵 / 形式诊断 (1$, . . . ,1, d$)。我们有 det(P) = 1 × 例 1，因而 det(A) = det(Δ) $=\pi (d)$ × 命题 3。

#### 例 4 {#alg-viii-a2-n4-exa-4 .statement tag=00QA}

令$D'$为域，并令$u$为从D到$D'$的同态。当经过为商时，$u$定义群同态$u_{ab}$从$D^*_{ab}$到$D^{'*}_{ab}$。令$u_n$为从$\mathbf{G}\mathbf{L}_n(D)$到$\mathbf{G}\mathbf{L}_n(D')$的同态，即变换矩阵A$= (a_{ij})$到矩阵$(u(a_{ij}))$。 公式

(23) det($u_n($A)) $=u_{ab}$(det(A))

对于 $A\in \mathbf{G}\mathbf{L}_n(D)$ 来说，紧接着是例 3。

#### 例 5 {#alg-viii-a2-n4-exa-5 .statement tag=00QB}

我们有 $\mathbf{G}\mathbf{L}_1(D) = D^*$，命题 3 表明我们在 $\mathbf{G}\mathbf{L}_1(D)$ 中有 $a$ 的 det($a$) $=\pi (a)$。

#### 例 6 {#alg-viii-a2-n4-exa-6 .statement tag=00QC}

假设$n= 2$。令$A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$为$\mathbf{G}\mathbf{L}_2(D)$的元素。 D 的元素 $a$ 和$c$ 不都是零。我们将明确给出 A 的行列式。

如果 $a$ 不是零，那么我们有

（24）$A = \begin{pmatrix} 1 & 0 \\ ca^{-1} & 1 \end{pmatrix}\begin{pmatrix} a & 0 \\ 0 & d-ca^{-1}b \end{pmatrix}\begin{pmatrix} 1 & a^{-1}b \\ 0 & 1 \end{pmatrix}$。

因而，$ad-aca^{-1}b\not= 0$ 和

（25）检测（A）$=\pi (ad-aca^{-1}b)$。

b) 如果 $a$ 是零，那么我们有 $c\not= 0$ 并且

(26)$A = \begin{pmatrix} 0 & b \\ c & d \end{pmatrix} = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}\begin{pmatrix} c & d \\ 0 & b \end{pmatrix}$。

因而，通过 a) 和例 2，我们有 $cb\not= 0$ 和

（27）检测（A）$=\pi (-cb)$。

#### 例 7 {#alg-viii-a2-n4-exa-7 .statement tag=00QD}

令$D^o$与D的域相反。从$\mathbf{M}_n(D)$到$\mathbf{M}_n(D^o)$的映射$A\mapsto^tA$满足$^t($AB$) =^tB^tA$。因而，对于$\mathbf{G}\mathbf{L}_n$(D)中的每个矩阵 A，转置的矩阵$^tA$在$\mathbf{M}_n(D^o)$中可逆，但在$\mathbf{M}_n(D)$中不一定可逆。由例 3可知，如果属于到$\mathbf{G}\mathbf{L}_n$(D)，则$\mathbf{G}\mathbf{L}_n(D)$的元素A和$\mathbf{G}\mathbf{L}_n(D^o)$的$^tA$具有相同的行列式。另一方面，即使矩阵$^tA$属于到$\mathbf{G}\mathbf{L}_n$(D)，其在GL$_n(D)$中的行列式也不一定等于A的行列式(cf.例6)。

#### 注 1 {#alg-viii-a2-n4-rem-1 .statement tag=00QE}

令 V 为右向量空间超过域 D，即有限维 $n$。我们将对偶空间 $V^*=$ Hom$_D(V,D)$ 视为 D 的对偶域 $D^o$ 上的右向量空间。令 $u$ 为 V 的自同构，并令 $^tu$ 为自同构 $V^*$ 即 $u$ 中的转置。如果对于V的基$(e_1, . . . , e_n)$，$u$由$\mathbf{M}_n(D)$中的矩阵A表示，则自同构$^tu$关于$\mathbf{M}_n(D^o)$中的矩阵$^tA$表示$V^*$ 的基 $(e^*_1, . . . , e^*_n)$ 对偶$(e_1, . . . , e_n)$（II, §10, No. 4、p. 344、命题 3）。到例 7 时，$^tu$ 的行列式等于 $u$ 的行列式。

#### 注 2 {#alg-viii-a2-n4-rem-2 .statement tag=00QF}

小节 1 到 4 的结果推广到 D 为局部环（VIII、p. 459、习题 2）时的情况。

### 5. 幺模群

设$n$为正整数。我们用群同态 det$:\mathbf{G}\mathbf{L}_n(D)\rightarrow D^*_{ab}$的$\mathbf{S}\mathbf{L}_n(D)$核来表示，我们称之为幺模群或特殊线性群（cf.III, §8, No. 9，p. 537当域D是可交换的）。

#### 定理 1 {#alg-viii-a2-thm-1 .statement tag=00QG}

假设$n\geqslant 2$。

a) $\mathbf{G}\mathbf{L}_n(D)$的子群$\mathbf{S}\mathbf{L}_n(D)$由矩阵$B_{ij}(\lambda )$生成，其中$i$和$j$是不同整数在区间$[1, n]$和$\lambda$穿过D。

b) 假设 $n\geqslant 3$ 或 Card(D) $\geqslant 3$。 $\mathbf{G}\mathbf{L}_n(D)$的导出群等于$\mathbf{S}\mathbf{L}_n(D)$。

c) 假设 $n\geqslant 3$ 或 Card(D) $\geqslant 4$。 $\mathbf{S}\mathbf{L}_n(D)$的导出群等于$\mathbf{S}\mathbf{L}_n(D)$。

A) 用矩阵$B_{ij}(\lambda )$生成的$\mathbf{G}\mathbf{L}_n(D)$的T子群表示。到 VIII、p. 454 的例 1 时，我们得到 det($B_{ij}(\lambda )$) $= 1$，因此有 $T\subset \mathbf{S}\mathbf{L}_n(D)$。为了证明这两个群相等，只需 loc 的例 3 即可。引证，证明形式 diag(1$, . . . ,1, d$) 的每个矩阵以及 $\pi (d) = 1$ 属于到 T。 矩阵 diag(1$, . . . ,1, d$) 属于到像同态$U\mapsto \begin{pmatrix} I_{n-2} & 0 \\ 0 & U \end{pmatrix}$从$\mathbf{G}\mathbf{L}_2(D)$到$\mathbf{G}\mathbf{L}_n(D)$；因此，考虑$n= 2$的情况就足够了。由于$\pi$的核是$D^*$的导出群，我们可以假设$d=uvu^{-1}v^{-1}$和$u, v$在$D^*$中。然后我们的断言由等式得出

(28) $\begin{pmatrix} 1 & 0 \\ 0 & d \end{pmatrix} = \begin{pmatrix} u^{-1} & 0 \\ 0 & u \end{pmatrix}\begin{pmatrix} v^{-1} & 0 \\ 0 & v \end{pmatrix}\begin{pmatrix} vu & 0 \\ 0 & u^{-1}v^{-1} \end{pmatrix}$

和

(29) $\begin{pmatrix} s & 0 \\ 0 & s^{-1} \end{pmatrix} = \begin{pmatrix} 1 & s \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 1-s^{-1} & 1 \end{pmatrix}\begin{pmatrix} 1 & -1 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 1-s & 1 \end{pmatrix}$

$s\in D^*$。

B) 通过构造，$\mathbf{S}\mathbf{L}_n(D)$是从$\mathbf{G}\mathbf{L}_n(D)$到可交换的群的同态的核，所以它是$\mathbf{G}\mathbf{L}_n(D)$的包含导出群$(\mathbf{G}\mathbf{L}_n(D),\mathbf{G}\mathbf{L}_n(D))$。综上所述，我们有

$$
\mathbf{S}\mathbf{L}_n(D)\supset (\mathbf{G}\mathbf{L}_n(D),\mathbf{G}\mathbf{L}_n(D))\supset (\mathbf{S}\mathbf{L}_n(D),\mathbf{S}\mathbf{L}_n(D))
$$

为了证明c)，只要证明矩阵$B_{ij}(\lambda )$是$\mathbf{S}\mathbf{L}_n(D)$中的换位子即可。

假设$n\geqslant 3$。如果$i,j,k$在区间$[1, n]$中是不同整数并且$\mu, \nu$是D的元素，那么我们有

$$
B_{ij}(\mu\nu ) =B_{ik}(\mu)^{-1}B_{kj}(\nu )^{-1}B_{ik}(\mu)B_{kj}(\nu ) \tag{30}
$$

通过取$\mu= 1$和$\nu =\lambda$，我们可以看到矩阵$B_{ij}(\lambda )$是$\mathbf{S}\mathbf{L}_n(D)$的元素的换位子。

现在假设$n= 2$。设$u$和$v$为D与$u\not= 0$的元素。我们有关系

(31) $\begin{pmatrix} 1 & v-uvu \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} u & 0 \\ 0 & u^{-1} \end{pmatrix}\begin{pmatrix} 1 & -v \\ 0 & 1 \end{pmatrix}\begin{pmatrix} u^{-1} & 0 \\ 0 & u \end{pmatrix}\begin{pmatrix} 1 & v \\ 0 & 1 \end{pmatrix}$ 和

(32)$\begin{pmatrix} 1 & 0 \\ v-uvu & 1 \end{pmatrix} = \begin{pmatrix} u^{-1} & 0 \\ 0 & u \end{pmatrix}\begin{pmatrix} 1 & 0 \\ -v & 1 \end{pmatrix}\begin{pmatrix} u & 0 \\ 0 & u^{-1} \end{pmatrix}\begin{pmatrix} 1 & 0 \\ v & 1 \end{pmatrix}$。

我们有 det $\begin{pmatrix} u & 0 \\ 0 & u^{-1} \end{pmatrix}$ = 1，所以矩阵 $B_{12}(v-uvu)$ 和 $B_{21}(v-uvu)$ 是 $\mathbf{S}\mathbf{L}_n(D)$ 的元素的换位子。

假设域 D 至少有四个元素。设$\lambda$为D的元素。如果$\lambda$等于0、1或$-1$，则选择为$D-\{0,1,-1\}$中的任意元素$u$；否则，集合$u=\lambda$。在这两种情况下，$u$是D的非零元素，它与$\lambda$交换，我们有$u^2\not= 1$。 集合$v=\lambda (1-u^2)^{-1}$。我们有$uv=vu$，因此有$v-uvu=v(1-u^2) =\lambda$。然后从关系(31)和(32)得出矩阵$B_{12}(\lambda )$和$B_{21}(\lambda )$是$\mathbf{S}\mathbf{L}_n(D)$中的换位子。这样就完成了 c) 的证明。

C) 当D有三个元素时，还需要证明$\mathbf{S}\mathbf{L}_2(D)$是$\mathbf{G}\mathbf{L}_2(D)$中的导出群。由A)，群$\mathbf{S}\mathbf{L}_2(D)$由矩阵$B_{12}(1) = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}$和$B_{21}(1) = \begin{pmatrix} 1 & 0 \\ 1 & 1 \end{pmatrix}$生成，而这些矩阵是$\mathbf{G}\mathbf{L}_2(D)$的元素换位子，因为我们有$B_{21}(1) =^tB_{12}(1)$和

(33)$\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} -1 & 0 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} -1 & 0 \\ 0 & 1 \end{pmatrix}^{-1}\begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}^{-1}$。

#### 注{#alg-viii-a2-n5-rem-1 .statement tag=00QH}

如果 D 为域且有两个元素，则 $\mathbf{G}\mathbf{L}_2(D)$ 等于 $\mathbf{S}\mathbf{L}_2$(D)，并且它是阶 6 中的群，其中导出群有阶 3。如果 D 为域且三个元素，则群$\mathbf{S}\mathbf{L}_2(D)$有阶24，其导出群有阶8。假设$n\geqslant 2$；除前两种情况外，与$\mathbf{S}\mathbf{L}_n(D)$不同的$\mathbf{S}\mathbf{L}_n(D)$的每个正常子群都包含在$\mathbf{S}\mathbf{L}_n(D)$的中心$Z(\mathbf{S}\mathbf{L}_n(D))$中（II, §10、p. 421、习题13和14）。 群$\mathbf{S}\mathbf{L}_n(D)/Z(\mathbf{S}\mathbf{L}_n(D))$就很简单了。

令 V 为右向量空间超过域 D，即有限维 $n$。我们用SL(V)表示，并称V的幺模群，同态det$:\mathbf{G}\mathbf{L}(V)\rightarrow D^*_{ab}$的核。选择 V 中的基可以让人们通过 $\mathbf{S}\mathbf{L}_n(D)$ 来实现认同这个群。

We say that an automorphism $u$ of V is a transvection if there exist a vector $v$ of V and a linear form $\varphi$ on V such that $\varphi (v) = 0$ and $u(x) =x+v\varphi (x)$ for every $x$ in V. 当$n\geqslant 2,u$是横流当且仅当存在V的基相对于$u$的矩阵是形式$B_{ij}(\lambda )$。 定理1 意味着以下推论。

#### 推论{#alg-viii-a2-n5-cor-1 .statement tag=00RU}

令 V 为右向量空间超过域 D，即有限维 $n\geqslant 2$。

a) $\mathbf{G}\mathbf{L}(V)$ 的子群 $\mathbf{S}\mathbf{L}(V)$ 由横断面生成。

b) 子群$\mathbf{S}\mathbf{L}(V)$是$\mathbf{G}\mathbf{L}(V)$除非的导出群，我们有$n= 2$，D有两个元素。

c) 群$\mathbf{S}\mathbf{L}(V)$等于它的导出群除非，我们有$n= 2$，D有两个或三个元素。

### 习题{#alg-viii-a2-exercises}

参见[习题附录 2](exercises/a2/)。
