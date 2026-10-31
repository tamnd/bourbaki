---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 5
section_title: Symmetric tensors and polynomial mappings
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.41-A IV.61, A IV.91-A IV.98
pdf_pages: 0050-0070, 0100-0107
extraction: ocr
subsections:
    - "no": 1
      title: Relative traces
      page: 41
      pdf_page: 50
    - "no": 2
      title: Definition of symmetric tensors
      page: 42
      pdf_page: 51
    - "no": 3
      title: Product for symmetric tensors
      page: 43
      pdf_page: 52
    - "no": 4
      title: Divided powers
      page: 45
      pdf_page: 54
    - "no": 5
      title: Symmetric tensors over a free module
      page: 47
      pdf_page: 56
    - "no": 6
      title: The functor TS
      page: 48
      pdf_page: 57
    - "no": 7
      title: Coproduct for symmetric tensors
      page: 50
      pdf_page: 59
    - "no": 8
      title: Relations between TS(M) and S(M)
      page: 52
      pdf_page: 61
    - "no": 9
      title: Homogeneous polynomial mappings
      page: 54
      pdf_page: 63
    - "no": 10
      title: Polynomial mappings
      page: 57
      pdf_page: 66
    - "no": 11
      title: Relations between $\mathbf{S}(M^*)$, TS(M)*gr and Pol(M, A)
      page: 59
      pdf_page: 68
statements: 41
exercises: 16
errata:
    - says: For each $w \in \Omega$ let $u_\omega = \sum_{b \in \omega} b$
      read: For each $\omega \in \Omega$ let $u_\omega = \sum_{b \in \omega} b$
      why: Omega is B/H and its elements are orbits, written omega everywhere else in Lemma 1 on page 56, including in the subscript and under the sum of this very sentence. The quantifier alone is set roman.
    - says: put $\omega' = w - \{v_\omega\}$ and $B' = \bigcup_{\omega \in \Omega} w'$
      read: put $\omega' = \omega - \{v_\omega\}$ and $B' = \bigcup_{\omega \in \Omega} \omega'$
      why: The thing omega' is obtained from is the orbit omega, named round twice earlier in the same clause of (ii), and the union is over the omega' just defined. Page 56 sets both of these two as roman w.
    - says: we have $u_\omega \in U^H$ for all $w \in \Omega$
      read: we have $u_\omega \in U^H$ for all $\omega \in \Omega$
      why: The proof on page 56 sets the subscript of u round and the quantifier of the same letter roman, in one clause.
content_sha256: a79e9abad81b6bc8311ccff916d08fdf9417b4ff290e664c86139a3591a67135
translated_from: content/en/alg/IV/05_s5_symmetric_tensors_and_polynomial.md
translation_method: google
source_content_sha256: 0718f77b4c960447aa7b0aaceb1e4b634413b342ee6a1fdee7d6efa83b9be82a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 8de4763142dfdc93500ca0c5e1a40af6a57dd42e5e67194c0c538df9809e288b
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 5。对称张量和多项式映射

### 1. 相对痕迹

设 H 为群，M 为左 A[H]-模 $^{(1)}$。我们用所有$m \in M$中的$M^H$集合表示，使得$hm = m$代表所有$h \in H$$^{(2)}$；这是M的子A模块。

设G是H的子群，则$M^G$是M包含$M^H$的子A模。

给定$m \in M^G$，$h \in H$，如果$x = hG$是h模G的左陪集，那么我们有$xm = hGm = \{hm\}$。通过滥用M的记号元素$hm$将被写成xm。如果$h' \in H$，我们有

(1)
$$
h'(xm) = (h'x) m .
$$

假设从现在起 G 在 H 中具有有限指标。则

(2)
$$
\sum_{x \in H/G} xm \in M^H .
$$

因为，给定 $h' \in H$，我们根据 (1) 有，

$$
h' \left( \sum_{x \in H/G} xm \right) = \sum_{x \in H/G} (h'x) m = \sum_{y \in H/G} ym .
$$

(1) 我们用 H (III, p. 446) 的 A[H] 群代数表示。
（2）注意不要将记号与集合的乘积研究中介绍的相混淆（*集合理论*，II，p. 102）。

#### 定义 1 {#alg-iv-s5-def-1 .statement tag=06CT}

— 如果 G *是 H 中有限指标的*，我们将 $M^G$ 的 $\mathrm{Tr}_{H/G}$ 映射表示为 $M^H$ 定义为

$$
\mathrm{Tr}_{H/G} m = \sum_{x \in H/G} x m .
$$

这个映射是A-模$M^G$到A-模$M^H$的同态。

#### 命题 1 {#alg-iv-s5-prop-1 .statement tag=06CU}

— (i) 设 $m \in M^G$ 和 $h \in H$。然后 $hm \in M^{hGh^{-1}}$ 和

$$
\mathrm{Tr}_{H/hGh^{-1}}(hm) = \mathrm{Tr}_{H/G} m .
$$

(ii) 设 F 为 G 中有限指标的 G 子群，并令 $m \in M^F$，则

$$
\mathrm{Tr}_{H/G}(\mathrm{Tr}_{G/F} m) = \mathrm{Tr}_{H/F} m
$$

(iii) *如果* $m \in M^H$，则$\mathrm{Tr}_{H/G} m = (H : G) \cdot m$。

(i) 设 $h \in H$。对于$h' \in H$和$m \in M$，让我们输入$\varphi(h') = hh'h^{-1}$和$\psi(m) = hm$。我们有$\varphi(h') \psi(m) = \psi(h'm)$；通过转移结构，我们推断出如果$m \in M^G$，则$hm \in M^{hGh^{-1}}$并且

$$
\mathrm{Tr}_{H/hGh^{-1}}(hm) = \psi(\mathrm{Tr}_{H/G}(m)) .
$$

从$\mathrm{Tr}_{H/G}(m) \in M^H$开始，这证明了(i)。

(ii) 设$m \in M^F$和$(g_\alpha)_\alpha \in_A$为G mod F的左陪集的代表系统，以及H mod G的左陪集的代表$(h_\beta)_\beta \in_B$系统。则$(h_\beta g_\alpha)_{(\beta,\alpha) \in B \times A}$为H mod F的左陪集的代表系统。

$$
\begin{align*}
\mathrm{Tr}_{H/G}(\mathrm{Tr}_{G/F} m) &= \sum_{\beta \in B} h_\beta \left( \sum_{\alpha \in A} g_\alpha m \right) \\
&= \sum_{(\beta,\alpha) \in B \times A} (h_\beta g_\alpha) m = \mathrm{Tr}_{H/F} m .
\end{align*}
$$

(iii) 这个断言是显而易见的。

### 2. 定义对称张量

令 M 为A-模。我们记得 (III, p. 501) $\mathfrak{S}_n$ 在 A-模 $T^n(M)$ 的左侧进行运算，这样

$$
\sigma(x_1 \otimes x_2 \otimes \ldots \otimes x_n) = x_{\sigma^{-1}(1)} \otimes x_{\sigma^{-1}(2)} \otimes \ldots \otimes x_{\sigma^{-1}(n)}
$$

对于任意 $x_1, \ldots, x_n \in M$ 和 $\sigma \in \mathfrak{S}_n$。 元素 $z \in T^n(M)$，使得所有$\sigma \in \mathfrak{S}_n$的$\sigma \cdot z = z$被称为阶 n 的对称张量；它们是形式$T^n(M)$的子A模块，用$\mathbf{TS}^n(M)$表示；我们有$\mathbf{TS}^0(M) = A, \mathbf{TS}^1(M) = M$。我们将把

TS(M) = $\bigoplus_{n=0}^{\infty} TS^n(M)$;这是$\mathbf{T}(M)$的分级子A模块。对于每个 $z \in T^n(M)$ 元素 $\sum_{\sigma \in S_n} \sigma . z$ 属于到 $TS^n(M)$；我们用 $s . z$ 表示它，并将其称为 $z$ 的对称化。 映射 $s : z \mapsto s . z$ 是 A-模 $T^n(M)$ 中的同态变成 A-模 $TS^n(M)$。如果$z \in TS^n(M)$，则$s . z = n! \ z$。

### 3. 乘积对称张量

令$p, q \in \mathbf{N}$和$S_{p|q}$为所有置换$\sigma \in S_{p-q}$中的$S_{p+q}$由……组成中的子群，这使得$\mathbf{N}$的区间$(1, p)$和$(p+1, p+q)$保持稳定。如果$\sigma \in S_p$和$\sigma' \in S_q$，我们可以将$S_{p|q}$的定义元素$\sigma''$通过将$\sigma''(n) = \sigma(n)$放入$1 \leq n \leq p$并将$\sigma''(p+n) = p + \sigma'(n)$放入$1 \leq n \leq q$； 映射 $(\sigma, \sigma') \mapsto \sigma''$ 是 $S_p \times S_q$ 的同构到 $S_{p|q}$。

设$z \in TS^p(M)$，$z' \in TS^q(M)$，则$T^{p+q}(M)$的元素$z \otimes z'$在$S_{p|q}$下不变；因此我们可以得到定义元素 $\operatorname{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')$ 或 $TS^{p+q}(M)$。我们将为$TS(M)$配备A双线性乘法$(y, y') \mapsto yy'$，这样对于$p, q \in \mathbf{N}$，$z \in TS^p(M)$，$z' \in TS^q(M)$我们有

$$
zz' = \operatorname{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')
$$

如果$y \in TS(M)$和$y' \in TS(M)$，我们称$yy'$为$y$和$y'$的对称乘积。族$(TS^p(M))_p$，是代数$TS(M)$的型$\mathbf{N}$毕业，$\mathbf{T}(M)$的单位元是$TS(M)$的单位元毕业。

令 $S_{p,q}$ 为 $\sigma \in S_{p+q}$ 中的集合，使得

$$
\begin{align*}
&\sigma(1) < \sigma(2) < \ldots < \sigma(p) \\
&\sigma(p+1) < \sigma(p+2) < \ldots < \sigma(p+q).
\end{align*}
$$

$S_{p,q} \times S_{p|q}$到$S_{p+q}$的映射$(\sigma, \tau) \mapsto \sigma \tau$是双射（I，p. 60，例2）；因此，如果 $z \in TS^p(M)$ 和 $z' \in TS^q(M)$，我们有

$$
zz' = \sum_{\sigma \in S_{p,q}} \sigma(z \otimes z')
$$

#### 命题 2 {#alg-iv-s5-prop-2 .statement tag=06CV}

— (i) A-代数 $TS(M)$ 是结合律、交换律和单位律。

(ii) 令$p_1, \ldots, p_n$为整数$> 0$，并令$S_{p_1| \ldots |p_n}$为所有$\sigma \in S_{p_1+\cdots+p_n}$中的集合，使$\mathbf{N}$的下列区间保持稳定：

$$
(1, p_1), (p_1+1, p_1+p_2), \ldots, (p_1+\cdots+p_{n-1}+1, p_1+\cdots+p_n).
$$

令$z_1 \in \mathbf{TS}^{p_1}(M) , \ldots , z_n \in \mathbf{TS}^{p_n}(M)$，则

$$
z_1 z_2 \ldots z_n = \operatorname{Tr}_{\mathfrak{S}_{p_1 + \cdots + p_n}/\mathfrak{S}_{p_1}| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n) .
$$

特别是如果$x_1, \ldots, x_r \in M$，我们有$x_1 \ldots x_r = s(x_1 \otimes \ldots \otimes x_r)$。

断言 (ii) 对于$n = 1$ 是明确的。假设关系

$$
z_2 \ldots z_n = \operatorname{Tr}_{\mathfrak{S}_{p_2 + \cdots + p_n}/\mathfrak{S}_{p_2}| \cdots | p_n} (z_2 \otimes \ldots \otimes z_n)
$$

已经证明了，让我们把所有置换中限制到$(1, p_1)$的认同$\mathfrak{S}_{p_2 + \cdots + p_n}$和$\mathfrak{S}_{p_1 + \cdots + p_n}$由……组成的子群恒等式。然后

$$
\operatorname{Tr}_{\mathfrak{S}_{p_1}|p_2+\cdots+p_n/\mathfrak{S}_{p_1}|p_2| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_r) =
$$
$$
= z_1 \otimes \operatorname{Tr}_{\mathfrak{S}_{p_2+\cdots+p_n}/\mathfrak{S}_{p_2}| \cdots | p_n} (z_2 \otimes \ldots \otimes z_r) = z_1 \otimes (z_2 \ldots z_n) .
$$

因此我们有

$$
z_1 z_2 \ldots z_r = z_1 (z_2 \ldots z_r) =
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+\cdots+p_n}/\mathfrak{S}_{p_1}|p_2-\cdots+p_n} (z_1 \otimes (z_2 \ldots z_n))
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+\cdots+p_n}/\mathfrak{S}_{p_1}|p_2+\cdots+p_n} (\operatorname{Tr}_{\mathfrak{S}_{p_1}|p_2+\cdots+p_n/\mathfrak{S}_{p_1}|p_2| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n))
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1-\cdots+p_n}/\mathfrak{S}_{p_1}| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n)
$$

根据第 1 号提案，IV 的 (ii)，p. 42。从而(ii)成立。

特别是，

$$
z_1 (z_2 z_3) = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1}|p_2|p_3} (z_1 \otimes z_2 \otimes z_3) ,
$$

以同样的方式我们表明

$$
(z_1 z_2) z_3 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1}|p_2|p_3} (z_1 \otimes z_2 \otimes z_3) .
$$

因此代数 $\mathbf{TS}(M)$ 是结合律。

令 $o$ 为 $\mathfrak{S}_{p_1+p_2}$ 的元素，使得

$$
\begin{align*}
\sigma(1) &= p_2 + 1, \; \sigma(2) = p_2 + 2, \; \ldots, \; \sigma(p_1) = p_2 + p_1 , \\
\sigma(p_1 + 1) &= 1, \; \sigma(p_1 + 2) = 2, \; \ldots, \; \sigma(p_1 + p_2) = p_2 .
\end{align*}
$$

然后

$$
z_2 z_1 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_2}|p_1} (z_2 \otimes z_1)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\sigma \mathfrak{S}_{p_1}|p_2 \sigma^{-1}\sigma} (z_1 \otimes z_2)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_1}|p_2} (z_1 \otimes z_2) \quad \text{by Prop 1, (i)}
$$
$$
= z_1 z_2 .
$$

因此代数 $\mathbf{TS}(M)$ 是可交换的。

需要注意的是，$\mathbf{T}(M)$中的$\mathbf{TS}(M)$中的典范嵌入不是一般的代数同态。更糟糕的是，$\mathbf{TS}(M)$ 在乘法或 $\mathbf{T}(M)$ 下通常不稳定。

### 4.分幂

让$x \in M$和$k \in \mathbf{N}$。显然$x, \otimes x_2 \otimes \ldots \otimes x_k$，其中
$$
x_1 = x_2 = \cdots = x_k = x ,
$$
是元素 / $\mathbf{TS}^k(M)$。

#### 定义 2 {#alg-iv-s5-def-2 .statement tag=06CW}

*如果*$x \in M$，*元素*$x \otimes x \otimes \ldots \otimes x$*的*$\mathbf{TS}^k(M)$*由*$\gamma_k(x)$表示。

#### 命题 3 {#alg-iv-s5-prop-3 .statement tag=06CX}

(i) *如果* $x \in M$，*$x$ 的第幂，*计算在* $\mathbf{TS}(M)$，*等于* $p! \; \gamma_p(x)$。
(ii) *设* $x_1, \ldots, x_n \in M$； *然后*
$$
\gamma_p(x_1 + x_2 + \cdots + x_n) = \sum_{p_1 + p_2 + \cdots + p_n = p} \gamma_{p_1}(x_1) \; \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) .
$$
(iii) *设*$x_1, \ldots, x_n \in M$，*设*$p_1, \ldots, p_n$*为整数*$\geqslant 0$*和*$p = p_1 + \ldots + p_n$。 *让*$E$*成为映射*$\varphi$*的集合*$\{1, \ldots, p\}$*进入*$(1, \ldots, n)$*这样*
$$
\operatorname{Card} \varphi^{-1}(1) = p_1, \ldots, \operatorname{Card} \varphi^{-1}(n) = p_n .
$$
*然后*
$$
\gamma_{p_1}(x_1) \; \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) = \sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes \ldots \otimes x_{\varphi(p)} .
$$
(iv) *令* $x \in M$ *且令* $q, r$ *为整数* $\geqslant 0$。 *然后*
$$
\gamma_q(x) \; \gamma_r(x) = \frac{(q + r)!}{q! \; r!} \; \gamma_{q + r}(x) .
$$
(v) *让* $x_1, \ldots, x, \in M$，*并为* $H \subset (1, \ldots, n)$ *放入* $x_H = \sum_{i \in H} x_i$，*然后*
$$
(-1)^n x_1 x_2 \ldots x_n = \sum_{H \subset \{1, \ldots, n\}} (-1)^{\operatorname{Card} H} \gamma_n(x_H) .
$$

断言(i) 立即由提案 2 (ii) 得出。

让我们证明(ii)；通过 n 上的归纳，我们看到考虑$n = 2$的情况就足够了。然后我们有

$$
\gamma_p(x_1 + x_2) = (x_1 + x_2) \otimes (x_1 + x_2) \otimes ... \otimes (x_1 + x_2) \quad @\text{factors})
$$
$$
= \sum_{p_1 + p_2 = p} \sum_{\sigma \in S_{p_1, p_2}} \sigma(x_1 \otimes x_1 \otimes ... \otimes x_1 \otimes x_2 \otimes x_2 \otimes ... \otimes x_2)
$$
$$
= \sum_{p_1 + p_2 = p} \sum_{\sigma \in S_{p_1, p_2}} \sigma(\gamma_{p_1}(x_1) \otimes \gamma_{p_2}(x_2))
$$
$$
= \sum_{p_1 + p_2 = p} \gamma_{p_1}(x_1) \gamma_{p_2}(x_2).
$$

为了证明 (iii)，令 $S_{p_1, ..., p_n}$ 为 $(1, p_1 + ... + p_n)$ 的置换的集合，其限制为区间
$$(1, p_1), (p_1 + 1, p_1 + p_2), ..., (p_1 + ... + p_{n-1} + 1, p_1 + ... + p_n)$$
是递增。根据 I、p. 60、例 2 和命题 2，(ii) 我们有
$$
\gamma_{p_1}(x_1) \gamma_{p_2}(x_2) ... \gamma_{p_n}(x_n) = \sum_{\rho \in S_{p_1, p_2, ..., p_n}} \rho(x_1 \otimes x_1 \otimes ... \otimes x_1 \otimes x_2 \otimes x_2 \otimes ... \otimes x_2 \otimes ... \otimes x_n \otimes x_n \otimes ... \otimes x_n)
$$
（$p_i$ 因子 $x_i$）并且这个和等于
$$
\sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes ... \otimes x_{\varphi(p)}.
$$

在(iii)中，让我们输入$n = 2, x_1 = x_2 = x, p_1 = q$和$p_2 = r$，然后我们得到(iv)（I，loc.cit.）。

最后 (v) 源自第 2、(ii) 条和 I p. 100 的第 2 条提案，应用于环 $\mathbf{T}(M)$ 的元素 $x_i$。

#### 注 1 {#alg-iv-s5-n4-rem-1 .statement tag=06CY}

令 $(x_i)_{i \in I}$ 为 M 的元素的家族。对于每个 $\nu \in \mathbf{N}^{(I)}$ 放置
$$
x_\nu = \prod_{i \in I} \gamma_{\nu_i}(x_i).
$$
如果 $(\lambda_i) \in \mathbf{A}^{(1)}$ 和 $p \in \mathbf{N}$，那么根据命题 3 (ii)，我们有，
$$
\gamma_p \left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{\nu \in \mathbf{N}^{(I)}, |\nu| = p} \lambda^\nu x_\nu.
$$
(6)

#### 注 2 {#alg-iv-s5-n4-rem-2 .statement tag=06CZ}

设$\mathscr{M}$为$(1, p)$映射集合代入I。我们将$\mathscr{M}$定义映射$\rho \mapsto \rho^*$代入$\mathbf{N}^{(I)}$
$$
\rho^*(i) = \operatorname{Card} \rho^{-1}(i)
$$

对于$\mathscr{M}$到满足$\rho_1^* = \rho_2^*$的两个元素$\rho_1, \rho_2$来说，存在$\sigma \in \mathfrak{S}_p$使得$\rho_2 = \rho_1 \circ \sigma$(I，p. 95)是充分必要的。根据提案 3 (iii)，对于 $|\nu| = p$，我们有：

$$
x_\nu = \sum_{\rho \in \mathscr{M}, \rho^* = \nu} x_{\rho(1)} \otimes x_{\rho(2)} \otimes \ldots \otimes x_{\rho(p)}
$$

### 5. 对称张量超过自由模

#### 命题 4 {#alg-iv-s5-prop-4 .statement tag=06D0}

— 让 $M$ 自由，并且 $(e_i)_{i \in I}$ 基为 $M$。

(i) 对于$\nu \in \mathbf{N}^{(I)}$，设$e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$。那么$(e_\nu)_{\nu \in \mathbf{N}^{(I)}}$就是$A$模块$TS(M)$的基。特别是代数$\mathbf{TS}(M)$是由元素$\gamma_k(x)$族为$k \in N$和$x \in M$生成的。

(ii) 对于每个$p \in N$，$\mathbf{TS}^p(M)$ 是$A$-模块$\mathbf{T}^p(M)$ 的直因子。

让我们使用上面的注 2 中的记号。家庭$(e_{\rho(1)} \otimes \ldots \otimes e_{\rho(p)})_{\rho \in \mathscr{M}}$是$\mathbf{T}^p(M)$的基。因此，第 4 条提案源自公式 (7) 和随后的引理，并与$H = \mathfrak{S}_p$ 和 $U = \mathbf{T}^p(M)$ 一起应用。

#### 引理 1 {#alg-iv-s5-lem-1 .statement tag=06D1}

令$H$为有限群，且$U$为左$A[H]$模。假设$A$-模块$U$有基$B$，在$U$中的$H$的运算下是稳定的，并放入$\Omega = B/H$。对于每个 $w \in \Omega$ 让 $u_\omega = \sum_{b \in \omega} b$；然后

(i) $(u_\omega)_{\omega \in \Omega}$ 是$A$-模块$U^H$ 的基。

(ii) 对于每个$\omega \in \Omega$，令$v$为$\omega$的点；把$\omega' = w - \{v_\omega\}$和$B' = \bigcup_{\omega \in \Omega} w'$放在一起，那么$B'$就是$U$中$U^H$的补充子空间的基。

所有$u_\omega$（对于$\omega \in \Omega$）的集合和$B'$的并是$U$的基。如果 $U' = \sum_{\omega \in \Omega} Au$ 和 $U'' = \sum_{b \in B'} Ab$，则我们有 $U = U' \oplus U''$。另一方面，对于所有$w \in \Omega$，我们都有$u_\omega \in U^H$，因此$U' \subset U^H$。最后，令$(\alpha_b)_{b \in B}$成为$A$与有限支撑的元素的族，并令$x = \sum_{b \in B} \alpha_b b$。如果$x \in U^H$，则$\alpha_{hb} = \alpha_b^H$适用于所有$b \in B$和所有$h \in H$，因此$x \in U'$，并且随之而来的是$U' = u^H$。

#### 命题 5 {#alg-iv-s5-prop-5 .statement tag=06D2}

— 令$M$为自由的$A$模块，$k$整数$\geq 0$，$P$由$\gamma_k(M)$生成的$\mathbf{TS}^k(M)$的子$A$模块。假设$A$是无限的整环。那么对于每个$z \in \mathbf{TS}^k(M)$，都存在$a \in A - \{0\}$，使得$az \in P$。

设$K$为$A$的分数中的域。我们认同$\mathbf{TS}^k(M)$具有向量K空间$V = \mathbf{TS}^k(M) \otimes_A K$的子A模块（第4条，以及II，p. 314）。我们必须证明这个向量 K-空间是由$\gamma_k(M)$生成的，也就是说，V 满足 $f(\gamma_k(M)) = 0$上的每个K线性形式$f$都是零。令 $(e_i)_{i \in I}$ 为 M 的基，定义为 e，如命题 4 中所示。对于任何 $(\alpha_i) \in A^{(I)}$，考虑到 (6)，我们有：

$$
0 = f \left( \gamma_k \left( \sum_{i \in I} \alpha_i e_I \right) \right) = \sum_{\nu \in N^{(I)}, |\nu| = k} \alpha^\nu f(e_\nu).
$$

由科. IV 的 2，p. 18 由此得出，$f(e_\nu) = 0$ 对于所有 $\nu \in N^{(I)}$、从而 $f = 0$。

### 6. 函子 TS

令M、N为M到N的A-模且u同态；很明显$T(u)(TS(M)) \subset TS(N)$。从T(u)获得的TS(M)到TS(N)的映射记为TS(u)。很容易验证这是分级代数的统一同态，并且我们对所有 $x \in M$ 和每个整数 $p \geq 0$ 都有 TS(u) $(\gamma_p(x)) = \gamma_p(u(x))$。如果$v : N \to P$是同态/A-模，我们有

$$
TS(v \circ u) = TS(v) \circ TS(u).
$$

TS(u) 定义，图表

$$
\begin{array}{cccc}
M & \longrightarrow & TS(M) \longrightarrow T(M) \\
u \downarrow & & \downarrow TS(u) & \downarrow T(u) \\
N & \longrightarrow & TS(N) \longrightarrow T(N)
\end{array}
$$

是可交换的，其中水平箭头表示典范嵌入。

如果 M 是 N 的直因子并且 i : M \to N 是典范嵌入，则 TS(i) 是 TS(M) 的单同态到 TS(N) 的直因子 R，通过它我们通常可以认同 TS(M) 和 R。对于张量代数证明了这一点（三、p. 487）。

假设M是子模家庭$(M_\lambda)_{\lambda \in L}$的直和。 典范嵌入 $TS(M_\lambda) \to TS(M)$ 定义分级代数的单位同态 h，称为规范：

$$
\bigotimes_{\lambda \in L} TS(M_\lambda) \to TS(M)
$$

令$\lambda_1, \lambda_2, \ldots, \lambda_n$与L成对不同的元素，并令$x_1 \in M_{\lambda_1}, \ldots, x_n \in M_{\lambda_n}$。根据第 3 条命题 IV 的 (ii)，p. 45，我们有

$$
h \left( \sum_{p_1 + \cdots + p_n = p} \gamma_{p_1}(x_1) \otimes \cdots \otimes \gamma_{p_n}(x_n) \right) = \gamma_p(x_1 + \cdots + x_n).
$$

令$N$为$A$模块，它是$(N_\lambda)_\lambda$族、子模族的直和。对于每个$\lambda \in L$，令$u_\lambda$为$M_\lambda$到$N_\lambda$的同态。令$u$为$M$的同态进入由$u_\lambda$定义的$N$。然后图表

$$
\begin{array}{ccc}
\otimes \mathbf{TS}(M_\lambda) & \xrightarrow{h} & \mathbf{TS}(M) \\
\downarrow & & \downarrow \mathbf{TS}(u) \\
\otimes \mathbf{TS}(u_\lambda) & & \\
\downarrow & & \\
\otimes \mathbf{TS}(N_\lambda) & \xrightarrow{h'} & \mathbf{TS}(N)
\end{array}
$$

通勤，其中$h$和$h'$是典范同态。对于如果 $z \in TS(M_\lambda)$ 且 $i_\lambda$（或 $j_\lambda$）表示 $M_\lambda$ 的典范嵌入到 $M$（或$N$，到 $N$），那么我们有

$$
\mathbf{TS}(u)(h(z)) = \mathbf{TS}(u) \circ \mathbf{TS}(i_\lambda)(z) = \mathbf{TS}(u \circ i_\lambda)(z) =
$$
$$
= \mathbf{TS}(j_\lambda \circ u_\lambda)(z) = \mathbf{TS}(j_\lambda) \circ \mathbf{TS}(u_\lambda)(z) = h'(\mathbf{TS}(u_\lambda)(z)) .
$$

#### 命题 6 {#alg-iv-s5-prop-6 .statement tag=06D3}

— *让$M$是一个$A$模块，它是$(M_\lambda)_\lambda$家族的直和，子模。如果每个$M_\lambda$是自由模，那么$\otimes_{\lambda \in L} \mathbf{TS}(M_\lambda)$到$\mathbf{TS}(M)$的典范同态就是同构。*

令 $(e_{i,\lambda})_{i, I_\lambda}$ 为 $M_\lambda$ 中的基。对于$\nu \in \mathbf{N}^{(I_\lambda)}$，输入$e_{\nu,\lambda} = \prod_{i \in I_\lambda} \gamma_{\nu(i)}(e_{i,\lambda})$。 $TS(M_\lambda)$（IV，p. 47，命题 4 (i)）和$e_{0,\lambda}$的$\nu \in \mathbf{N}^{(I_\lambda)}$ 形式基的$e_{\nu,\lambda}$是$\mathbf{TS}(M_\lambda)$的单位元素。因此元素

$$
\otimes_{\lambda \in L} e_{\nu_{\lambda,\lambda}}
$$

其中 $\nu_\lambda \in \mathbf{N}^{(I_\lambda)}$ 和 $\nu_\lambda = 0$，除了指标的有限数、形式基 $\otimes_A TS(M_\lambda)$。 元素(9)中的像在命题的典范同态下是$\prod_{\lambda \in L} e_{\nu_{\lambda,\lambda}}$。如果我们用$(e_{i,\lambda})_{i, I_\lambda}$家族的$(e_i)_i$、不相交的并来表示，那么上面的元素正是$\prod_{i \in I} \gamma_{\nu(i)}(e_i)$，其中$\nu \in \mathbf{N}^{(I)}$，因此它们构成$\mathbf{TS}(M)$的基。这就证明了命题。

根据第6号提案的条件，逆同构$\mathbf{TS}(M) \to \otimes_{\lambda} \mathbf{TS}(M_\lambda)$也称为*规范*。通常，$\mathbf{TS}(M)$ 通过此同构与$\otimes_{\lambda} TS(M_\lambda)$ 进行识别。需要注意的是，如果$z \in TS(M_\lambda)$和$z' \in \mathbf{TS}(M_{\mu})$与$\lambda \neq \mu$，那么$\mathbf{TS}(M)$的元素（因此我们用$z \otimes z'$表示）不是$\mathbf{T}(M)$中的$z$和$z'$的张量积，而是对称的$z$ 和 $z'$ 中的乘积。

#### 命题 7 {#alg-iv-s5-prop-7 .statement tag=06D4}

*令$M$为$A$模，将$M \oplus M$的$u$映射$(x, y) \mapsto x + y$分解为$M$和$f$复合映射*

$$
\mathbf{TS}(M) \otimes \mathbf{TS}(M) \xrightarrow{h} \mathbf{TS}(M \oplus M) \xrightarrow{\mathbf{TS}(u)} \mathbf{TS}(M)
$$

*其中 $h$ 是典范同态。如果$z, z' \in \mathbf{TS}(M)$，则$f(z \otimes z') = zz'$。*

让$i$是$M$的映射$x \mapsto (x, 0)$到$M \oplus M$。我们有$u \circ i = \mathrm{Id}_M$，因此$\mathbf{TS}(u) \circ \mathbf{TS}(i) = \mathrm{Id}_{\mathbf{TS}(M)}$；因此

$$
f(z \otimes 1) = \mathbf{TS}(u)(h(z \otimes 1)) = \mathbf{TS}(u)(\mathbf{TS}(i)(z)) = z .
$$

同样$f(1 \otimes z') = z'$、从而$f(z \otimes z') = f(z \otimes 1) f(1 \otimes z') = zz'$。

### 7. 余积对称张量

令 $M$ 为*自由* $A$ 模块，并且 $\Delta_M = A$ $M$ 的对角线同态 $x \mapsto (x, x)$ 进入$M \oplus M$。令 $c_M = c$ 为由同态组成的分级 $A$-代数的单位同态：

$$
\mathbf{TS}(M) \xrightarrow{\mathbf{TS}(\Delta)} \mathbf{TS}(M \oplus M) \xrightarrow{\sigma} \mathbf{TS}(M) \otimes \mathbf{TS}(M)
$$

其中 $\sigma$ 是典范同构。配备$c$，$\mathbf{TS}(M)$是分级的$A$-代数。

对于所有 $x \in M$ 和每个整数 $p \geq 0$，我们有 $\mathbf{TS}(A)(\gamma_p(x)) = \gamma_p((x, x))$，因此根据 (8)，

$$
c(\gamma_p(x)) = \sum_{r+s=p} \gamma_r(x) \otimes \gamma_s(x).
$$

特别是

$$
c(x) = x \otimes 1 + 1 \otimes x .
$$

让$(x_i)_{i \in I}$是元素和$M$的一个家族，对于$\nu \in \mathbf{N}^{(I)}$来说，放入$x_\nu = \prod_{i \in I} \gamma_{\nu_i}(x_i)$。

然后

$$
c(x_\nu) = \sum_{\rho + \sigma = \nu} x_\rho \otimes x_\sigma .
$$

这是从*(10)*得出的，因为$c$是代数同态。

#### 命题 8 {#alg-iv-s5-prop-8 .statement tag=06D5}

— 令 M 为自由A-模，则以其代数和余代数结构，TS (M) 是分级交换和共交换大数。 余单位是 A-线性映射 $\varepsilon : TS(M) \to TS^0(M) = A$，对于 $p > 0$，$TS^p(M)$ 是零，因此$\varepsilon(1) = 1$。

我们知道A-代数$TS(M)$是结合律、交换律和单位律。另一方面，余积是按构造同态分级的代数；现在，余代数 $TS(M)$ 是共结合和共交换的，可以通过公式 (10) 进行简单计算。 A 中 $TS(M)$ 的映射 $\varepsilon$ 是分级代数的同态，使得 $\varepsilon(l) = l$。最后，对于每个$x \in M$，如果$p > 0$，$\varepsilon(\gamma_0(x)) = l$，我们有$\varepsilon(\gamma_p(x)) = 0$；如果我们记住（lo），这表明 $(F \otimes 1) \circ c = (l \otimes E) \circ c = \mathrm{Id}_{TS(M)}$；因此$E$是$TS(M)$的余单位。

#### 命题 9 {#alg-iv-s5-prop-9 .statement tag=06D6}

— 设 M 和 N 为自由A-模，u 为 M 到 N 的 A 同态；那么$\mathbf{TS}(u)$是一个大数同态。

因为我们有$\Delta_N \circ u = (u,u) \circ \Delta_M$，因此图表

$$
\begin{array}{ccccccccc}
\mathbf{TS}(M) & \xrightarrow{\mathbf{TS}(\Delta_M)} & \mathbf{TS}(M \oplus M) & \xrightarrow{\sigma} & \mathbf{TS}(M) \otimes \mathbf{TS}(M) \\
\downarrow \mathbf{TS}(u) & & \downarrow \mathbf{TS}(u,u) & & \downarrow \mathbf{TS}(u) \otimes \mathbf{TS}(u) \\
\mathbf{TS}(N) & \xrightarrow{\mathbf{TS}(\Delta_N)} & \mathbf{TS}(N \oplus N) & \xrightarrow{\tau} & \mathbf{TS}(N) \otimes \mathbf{TS}(N),
\end{array}
$$

其中 $\sigma$ 和 $\tau$ 是典范同构，是可交换的 (IV, p. 49)。因此$c_N \circ \mathbf{TS}(u) = (\mathbf{TS}(u) \otimes \mathbf{TS}(u)) \circ c_M$。

#### 命题 10 {#alg-iv-s5-prop-10 .statement tag=06D7}

— 令 M 为自由A-模，则大数$\mathbf{TS}(M)$ 的原语元素 (III, p. 602) 为 M 的元素。

令 $(e_i)_{i \in I}$ 为 M 的基，对于 $\nu \in \mathbf{N}^{(I)}$ 则设置 $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$。设$z = \sum_{\nu \in \mathbf{N}^{(I)}} \lambda_\nu e_\nu$为$\mathbf{TS}(M)$的元素，则由(12)可得

$$
c(z) = \sum_\nu \lambda_\nu \sum_{\rho, \sigma \in \mathbf{N}^{(I)}, \rho + \sigma = \nu} e_\rho \otimes e_\sigma = \sum_{\rho, \sigma} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma
$$

因此

$$
c(z) - 1 \otimes z - z \otimes 1 = \sum_{\rho \neq 0, \sigma \neq 0} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma - \lambda_0 e_0 \otimes e_0
$$

所以

zprimitive $\Leftrightarrow \lambda_{\rho + \sigma} = 0$ 当 $\rho \neq 0$ 和 $\sigma \neq 0$ 和 $\lambda_0 = 0$ 时
$\Leftrightarrow \lambda_\nu = 0$ 当 $|\nu| \neq 1$
$\Leftrightarrow z \in M$。

### 8. TS(M) 和 S(M) 之间的关系

The canonical injection of M in TS(M) extends in a unique fashion to an algebra homomorphism of T(M) into TS(M) (III, p. 485, Prop. 1). 根据IV的命题2(ii)，p. 43，这个同态就是对称化算子。 由于代数 TS(M) 是可交换的，因此存在 (III, p. 497) 一个且仅有一个代数同态 $\varphi_M$（称为规范），将代数 S(M) 转换为代数 TS(M)，使得图表

$$
\begin{array}{ccc}
T(M) & \xrightarrow{\rho} & S(M) \\
& & \searrow s \\
& & TS(M)
\end{array}
$$

其中$\rho$表示T(M)到S(M)的典范同态，是可交换的。我们对所有 $p \in \mathbf{N}$ 都有 $\varphi_M(S^p(M)) \subset TS^p(M)$。

另一方面，通过将 TS(M) 的典范嵌入 i 组合成 T(M)，并将 T(M) 的典范同态 $\rho$ 组合到 S(M) 上，我们得到分级 A-模的同态 $\psi_M$，称为规范。 图表

$$
\begin{array}{ccc}
TS(M) & \xrightarrow{\psi_M} & S(M) \\
& & \downarrow \rho \\
& & T(M)
\end{array}
$$

是可交换的。

如果$u : M \to N$是A-模的同态，则图表

$$
\begin{array}{ccccccccc}
S(M) & \xrightarrow{\varphi_M} & TS(M) & \xrightarrow{\psi_M} & S(M) \\
| & & | & & | \\
S(N) & \xrightarrow{\varphi_N} & TS(N) & \xrightarrow{\psi_N} & S(N)
\end{array}
$$

是可交换的，很容易验证。

如果 M 是模 $M_\lambda$ 中的直和，则图表 (14)

$$
\begin{array}{ccc}
\otimes S(M_\lambda) & \xrightarrow{\otimes \varphi_{M_\lambda}} & \otimes TS(M_\lambda) \\
\downarrow f & & \downarrow g \\
S(M) & \xrightarrow{\varphi_M} & TS(M),
\end{array}
$$

其中$f$和$g$是典范同态，是可交换的。对于$g \circ \otimes \varphi_{M_\lambda}$和$\varphi_M \circ f$来说，代数同态是代数同态，对于每个$\lambda$，$M_\lambda$是重合。

#### 命题 11 {#alg-iv-s5-prop-11 .statement tag=06D8}

— *如果 $M$ 是免费的，那么 $\varphi_M$ 是分级 bigebras 的态射。*

利用图表 (13) 和 (14) 的交换律，我们得到交换律图表

$$
\begin{array}{ccccccccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \oplus M) & \xrightarrow{h} & S(M) \otimes S(M) \\
\downarrow \varphi_M & & \downarrow \varphi_{M \oplus M} & & \downarrow \varphi_M \otimes \varphi_M \\
TS(M) & \xrightarrow{TS(\Delta)} & TS(M \oplus M) & \xrightarrow{k} & TS(M) \otimes TS(M),
\end{array}
$$

其中$\Delta$是对角线同态，$h, k$是典范同态。由此得出命题。

#### 命题 12 {#alg-iv-s5-prop-12 .statement tag=06D9}

— (i) *如果 $u \in S^n(M)$，则 $\psi_M(\varphi_M(u)) = n!u$。*

(ii) *如果$v \in TS^n(M)$则$\varphi_M(\psi_M(v)) = n!v$。*

令$x_1, \ldots, x_n \in M$和$u$为在$S(M)$中计算出的乘积$x_1 \ldots x_n$。那么$\varphi_M(u)$就是$TS(M)$计算出来的乘积$x_1 \ldots x_n$，即

$$
\sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)}.
$$

因此$\psi_M(\varphi_M(u))$等于$S(M)$计算出的$\sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \ldots x_{\sigma(n)}$，即

$$
n! x_1 \ldots x_n = n!u.
$$

令$v = \sum_{i=1}^p x_1^i \otimes x_2^i \otimes \ldots \otimes x_n^i$为$TS^n(M)$的元素，其中$x_j^i$属于到$M$；那么$\psi_M(v)$等于$S(M)$、从而计算出的$\sum_{i=1}^p x_1^i x_2^i \ldots x_n^i$

$$
\varphi_M(\psi_M(v)) = \sum_{i=1}^p s(x_1^i \otimes x_2^i \otimes \ldots \otimes x_n^i) = s(v) = n!v.
$$

#### 推论 1 {#alg-iv-s5-prop-12-cor-1 .statement tag=06DA}

— *如果$\mathbf{A}$是$\mathbf{Q}$代数，则$S(M)$到$TS(M)$的典范同态是代数同构。而且如果$M$是免费的，那么它就是分级bigebras的同构。*

#### 推论 2 {#alg-iv-s5-prop-12-cor-2 .statement tag=06DB}

— *如果$A$是$\mathbf{Q}$代数，则模$TS^n(M)$由$TS(M)$中$M$的元素的第n个幂生成。
这是从 Cor 得出的。 1 和 $S(M)$* 的相应的性质（III、p. 498）。

### 9.齐次多项式映射

#### 命题 13 {#alg-iv-s5-prop-13 .statement tag=06DC}

— *令$M$和$N$为$A$模块，$q$整数$\geqslant 0$，以及$M$的$f$映射为$N$。假设$M$是免费的，那么以下条件是等价的：
(i) 存在$M^q$到$N$的$q$线性映射$g$，使得$f(x) = g(x, x, \ldots, x)$对于所有$x \in M$。
(ii) 存在$TS^q(M)$到$N$的线性映射$h$，使得$f(x) = h(\gamma_q(x))$对于所有$x \in M$。
(iii) 存在$M$的基$(e_i)_{i \in I}$和$N$的元素族$(u_\nu)_{\nu \in N^{(I)}, |\nu| = q}$使得
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{\nu \in N^{(I)}, |\nu| = q} \lambda^\nu u_\nu
$$
对于所有$(\lambda_i) \in A^{(I)}$。
(iv) 对于 $M$ 的每个基 $(e_i)_{i \in I}$，都存在一个$(u_\nu)_{\nu \in N^{(I)}, |\nu| = q}$ 元素 $N$ 族，使得
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{\nu \in N^{(I)}, |\nu| = q} \lambda^\nu u_\nu
$$
对于所有$(\lambda_i) \in A^{(I)}$。
(i) $\Rightarrow$ (ii)：设 $g$ 满足 (i)，则$T^q(M)$中存在线性映射$g'$进入$N$，使得对于任何$x, \ldots, x, \in M$都有$g(x_1, x_2, \ldots, x_q) = g'(x_1 \otimes x_2 \otimes \ldots \otimes x)$。然后
$$
f(x) = g(x, x, \ldots, x) = g'(x \otimes x \otimes \ldots \otimes x) = g'(\gamma_q(x));
$$
在写出 $h = g'|TS^q(M)$ 时，我们看到条件 (ii) 成立。
(ii)$\Rightarrow$(i)和(iv)：令(ii)的$h$满足条件。根据命题 4，(ii)(IV，p. 47)，存在$T^q(M)$的线性映射$g'$进入$N$，使得$h = g'|TS^q(M)$。令$g$为$M$到$N$与$g'$相关的$q$线性映射，那么对于任何$x \in M$我们有
$$
f(x) = h(\gamma_q(x)) = g'(x \otimes x \otimes \ldots \otimes x) = g(x, x, \ldots, x),
$$

从而（一）。另一方面，如果 $(e_i)_{i \in I}$ 是 M 的基，则通过公式 (6) (IV, p. 46)

$$
f \left( \sum_i \lambda_i e_i \right) = h \left( \gamma_q \left( \sum_i \lambda_i e_i \right) \right) = h \left( \sum_{|\nu|=q} \lambda^\nu e_\nu \right)
$$

关于写作$e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$；因此我们有

$$
f \left( \sum_i \lambda_i e_i \right) = \sum_{|\nu|=q} \lambda^\nu h(e_\nu).
$$

(iv) $\Rightarrow$ (iii) 很清楚。
(iii) $\Rightarrow$ (ii) ：给定 (iii) 的 $(e_i), (u_\nu)$ 满足条件，让我们写出 $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$ 并回想一下 $(e_\nu)_{|\nu|=q}$ 是 $\mathrm{TS}^q(M)$ 的基。令h为$\mathrm{TS}^q(M)$的同态到由$h(e_\nu) = u_\nu$定义的N中；那么对于 M 中的每个 $x = \sum_i \lambda_i e_i$ 我们有

$$
f(x) = f \left( \sum_i \lambda_i e_i \right) = \sum_{|\nu|=q} \lambda^\nu u_\nu = h \left( \sum_{|\nu|=q} \lambda^\nu e_\nu \right) = h(\gamma_q(x))
$$

#### 定义 3 {#alg-iv-s5-def-3 .statement tag=06DD}

— 令 M 和 N 为 A-模且 q 整数 $\geq 0$。假设M是*自由*，并用M的映射的$\mathrm{Pol}_A^q(M, N)$或简称$\mathrm{Pol}^q(M, N)$集合表示为命题13的N满足条件。$\mathrm{Pol}^q(M, N)$的元素称为M的次数q齐次多项式映射进入N。

提案 13 (i) 定义同态或 A-模 ：

$$
\mathscr{L}_q(M, ..., M; N) \to \mathrm{Pol}^q(M, N).
$$

提案 13 (ii) 定义同态 A-模

$$
\mathrm{Hom}_A(\mathbf{TS}^q(M), N) \to \mathrm{Pol}^q(M, N).
$$

这些同态被称为规范的。它们是主观的。

#### 例 1 {#alg-iv-s5-n9-exa-1 .statement tag=06DE}

M 到 N 的次数 1 的齐次多项式映射是 M 到 N 的 A-线性映射。

#### 例 2 {#alg-iv-s5-n9-exa-2 .statement tag=06DF}

令$(N_i)_{i \in I}$是A-模、$f_i$映射到$N_i, i \in I$的族，以及$f : M \to \prod_{i \in I} N_i$映射和组件$f_i$。要使 f 为次数 q 中的齐次多项式映射，每个 $f_i$ 为次数 q 中的齐次多项式映射是充分必要的。

#### 例 3 {#alg-iv-s5-n9-exa-3 .statement tag=06DG}

令 $(M_j)_{j \in J}$ 为自由A-模的有限族，$u : \prod_{j \in J} M_j \to N$ 为多线性映射；那么 u 是次数 $\mathrm{Card}(J)$ 的多项式。

#### 例 4 {#alg-iv-s5-n9-exa-4 .statement tag=06DH}

令$(X_i)_{i \in I}$为不定式族，$N$为$A$模，$u \in N[(X_i)_{i \in I}]$为次数$q$的齐次多项式。 $A^{(I)}$的映射$(x_i)_{i \in I} \mapsto u((x_i)_{i \in I})$到$N$是次数$q$的齐次多项式映射：这可以通过第13条命题的条件(iii)立即看出。如果$I$是有限的，则每齐次多项式映射 $A^{(I)} = A'$的次数$q$变成$N$就是形式。

#### 例 5 {#alg-iv-s5-n9-exa-5 .statement tag=06DI}

$A^{(N)}$映射$(x_i)_{i \in N} \mapsto x_0^2 + x_1^2 + \ldots + x_n^2 + \ldots$入$A$是次数2的齐次多项式映射。如果$A = 2/22$，则重合和线性映射$(x_i)_{i \in I} \mapsto x_0 + x_1 + \ldots + x_n + \ldots$

#### 例 6 {#alg-iv-s5-n9-exa-6 .statement tag=06DJ}

令$f \in \mathrm{Pol}_A^q(M, N)$，令$B$为交换环，$B$的$\rho$同态转化为$A$和$M'$和$N'$，从$M$和$N$衍生的$B$模块，通过$\rho$。假设$M'$是免费的；那么$f \in \mathrm{Pol}_B^q(M', N')$：这立即来自于第 13 条提案的条件 (i)。

#### 命题 14 {#alg-iv-s5-prop-14 .statement tag=06DK}

— 令$M, N, P$为$A$模块，$q$和$r$整数$\geqslant 0$，并假设$M$和$N$是免费的。如果$f \in \mathrm{Pol}^q(M, N)$，$f' \in \mathrm{Pol}^r(N, P)$，则$f' \circ f \in \mathrm{Pol}^{qr}(M, P)$。

存在$M^q$到$N$的$q$线性映射$g$和$N^r$到$P$的$r$线性映射$g'$，使得

$$
\begin{aligned}
f(x) &= g(x, x, \ldots, x) & \text{for all } x \in M, \\
f'(y) &= g'(y, y, \ldots, y) & \text{for all } y \in N.
\end{aligned}
$$

因此对于每个 $x \in M$ 我们有

$$
f'(f(x)) = g'(f(x), f(x), \ldots, f(x)) = g'(g(x, x, \ldots, x), \ldots, g(x, x, \ldots, x))
$$

$M^{qr}$到$P$的映射$(x_1, \ldots, x_{qr}) \mapsto g'(g(x_1, \ldots, x_q), \ldots, g(x_{q(r-1)+1}, \ldots, x_{qr}))$是$qr$线性。

#### 命题 15 {#alg-iv-s5-prop-15 .statement tag=06DL}

— 令$M$为免费的$A$模块，$N$为$A$模块，$q$整数$\geqslant 0$。我们假设映射$y \mapsto q!y$是$N$的自同构。设$f \in \mathrm{Pol}^q(M, N)$，则存在且仅有一个对称$q$-线性映射$M^q$到$M$的$h$，使得$f(x) = h(x, x, \ldots, x)$对于所有$x \in M$。对于任意 $x_1, \ldots, x_q \in M$ 我们有

$$
h(x_1, x_2, \ldots, x_q) = \frac{(-1)^q}{q!} \sum_{H \subset \{1, 2, \ldots, q\}} (-1)^{\mathrm{Card}\ H} f\left( \sum_{i \in H} x_i \right).
$$

a) 存在$M^q$到$N$的$q$线性映射$g$，使得所有$x \in M$都有$f(x) = g(x, x, \ldots, x)$。让我们将$M$的定义$q$线性映射$h$到$N$：

$$
h(x_1, x_2, \ldots, x_q) = \frac{1}{q!} \sum_{\sigma \in S_q} g(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(q)}).
$$

那么 $h$ 是对称的，并且 $f(x) = h(x, x, \ldots, x)$ 对于所有 $x \in M$ 都是对称的。

b) 令 $h$ 为 $M^q$ 到 $N$ 的对称 $q$ 线性映射，使得 f(x) = g(x, x, ..., x)。令 l 为 N 中 T^q(M) 的线性映射，使得对于任何 M 中的 x_1, ..., x_q \h(x_1, ..., x_q) = l(x_1 \otimes ... \otimes x_q) 。我们有

$$
(-1)^q q! h(x_1, ..., x_q) = (-1)^q \sum_{\sigma \in S_q} h(x_{\sigma(1)}, ..., x_{\sigma(q)}) =
= (-1)^q l(s(x_1 \otimes ... \otimes x_q)) = \sum_{H \subset \{1, ..., q\}} (-1)^{\text{Card } H} l \left( \gamma_q \left( \sum_{i \in H} x_i \right) \right)
$$

根据第 3 号提案 (v) (IV, p. 45)。现在

$$
l \left( \gamma_q \left( \sum_{i \in H} x_i \right) \right) = h \left( \sum_{i \in H} x_i, ..., \sum_{i \in H} x_i \right) = f \left( \sum_{i \in H} x_i \right)
$$

这就证明了 h 的公式 (16) 和唯一性。

#### 命题 16 {#alg-iv-s5-prop-16 .statement tag=06DM}

— *设 M 为 Hom ($\mathbf{TS}^q(M)$, N) 的自由A-模、N A-模、q 正整数和 u 典范同态到 $\mathbf{Pol}^Y(M, N)$。

(i) *如果 A 是无限整环并且 N 是无扭转的，则 u 是同构。*

(ii) *如果 N 中的映射 $y \mapsto q!y$ 是单射，则 u 是同构。*

在命题的两种情况下，我们必须证明u是单射的，也就是说，$\mathbf{TS}^q(M)$的每一个线性映射 f进入$\gamma_q(M)$上的零，消失。

假设 A 为无限整环并且 N 无扭转。对于每个 $z \in \mathbf{TS}^q(M)$ 都存在 $a \in A - \{0\}$，使得 $az$ 是 y, (M) (*IV*, p. 47，命题 5) 的元素的 A 线性组合。因此$af(z) = f(az) = 0$，所以$f(z) = 0$。

接下来假设 N 中的映射 $y \mapsto q!y$ 是单射的，则根据 *IV*, p. 45，命题 3, (v)， f 在 s 上消失。 T^q(M)。因此，如果$z \in \mathbf{TS}^q(M)$，我们有$q!f(z) = f(sz) = 0$，所以$f(z) = 0$。

#### 推论 {#alg-iv-s5-n9-cor-1 .statement tag=06DN}

— *设 M 为 M 的自由A-模、N A-模、q 正整数、$h \in \mathbf{Pol}^q(M, N)$ 和 $(e_i)_i$、基。在第 16 条命题的两个案例中，存在一个独特的族$(u,$、$\mathbf{N}^{(I)}, |\cdot|$、 、 N 的元素使得 $h \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{|\nu| = q} \lambda^\nu u_\nu$ 对于所有 $(\lambda_i) \in \mathbf{A}^{(1)}$*

### 10.多项式映射

#### 定义 4 {#alg-iv-s5-def-4 .statement tag=06DO}

— *令 M 和 N 为 A-模并假设 M 是自由的。令映射(M, N)为M到N的所有映射中的A-模。映射(M, N)中的子模$\sum_{q > 0} \mathbf{Pol}_A^q(M, N)$表示为$\mathbf{Pol}_A(M, N)$或简称为$\mathbf{Pol}(M, N)$；它的元素称为M到N的多项式映射。*

令$(e_i)_{i \in I}$为M的基，并假设$l$是有限的；根据命题 13 (IV, p. 54) 映射 $f$ 将 M 代入 N 是多项式当且仅当在不定式 $X_i$ 中存在一个多项式 F，其系数在 N 中，使得

$$
f \left( \sum_{i \in I} x_i e_i \right) = F(x)
$$

对于每个家庭$x = (x_i)_{i \in I}$在$A^{(I)}$。这个性质独立于为M选择的基，并且它证明了术语“多项式映射”。

#### 命题 17 {#alg-iv-s5-prop-17 .statement tag=06DP}

— *设 M 为自由A-模，B 为结合律、交换律和单位A-代数。那么$\mathrm{Pol}_A(M, B)$是代数$\mathrm{Map}(M, B)$的子B代数。

这是从 Def 得出的。 4 和提案 13，(iv) (IV，p. 54)。

#### 命题 18 {#alg-iv-s5-prop-18 .statement tag=06DQ}

— *设 M、N、P 为 A-模，并假设 M 和 N 是自由的。如果$f \in \mathrm{Pol}(M, N)$，$g \in \mathrm{Pol}(N, P)$，则$g \circ f \in \mathrm{Pol}(M, P)$。

我们可以立即约化到存在整数q使得$g \in \mathrm{Pol}^q(N, P)$的情况；则存在 $N^q$ 到 P 的 q 线性映射 $h$，使得对于所有 $y \in N$ 都有 $g(y) = h(y, y, \ldots, y)$。将 $f$ 写为齐次多项式映射的和，因此我们可以将证明简化为映射

$$
x \mapsto h(f_1(x), f_2(x), \ldots, f_q(x))
$$

将 M 转化为 P，其中 $f_i \in \mathrm{Pol}^{q_i}(M, N)$ 是多项式。对于$i = 1, \ldots, q$，存在$M^{q_i}$到N的$q_i$线性映射$l_i$，使得$f_i(x) = l_i(x, x, \ldots, x)$对于所有$x \in M$。因此

$$
h(f_1(x), f_2(x), \ldots, f_q(x)) = h(l_1(x, \ldots, x), \ldots, l_q(x, \ldots, x)),
$$

我们的断言由此而来。

#### 引理 2 {#alg-iv-s5-lem-2 .statement tag=06DR}

— *令 N 为 A-模，n 整数 $\geq 0$ 并且*

$$
f = m_0 + m_1 X + \cdots + m_n X^n \in N[X].
$$

*假设存在$\alpha_0, \alpha_1, \ldots, \alpha_r \in A$使得$f(\alpha_0) = \cdots = f(\alpha_r) = 0$，并且使得对于N中的比率$\alpha_i - \alpha_j$的$i \neq j$位似是单射的，则$f = 0$。*

（这个引理概括了IV的Cor.，p. 16。）

引理显然适用于 $n = 0$；我们将通过$n$上的归纳来证明它。我们有

$$
f(X) = f(X) - f(\alpha_0) = \sum_{i=1}^n m_i (X^i - \alpha_0^i) = (X - \alpha_0) g(X)
$$

其中 g 是形式 $m_0' + m_1' X + \ldots + m_{n-1}' X^{n-1}$ 的 N[X] 的元素。 引理的假设意味着$g(\alpha_1) = \cdots = g(\alpha_r) = 0$，因此$g = 0$乘以归纳假设，等等$f = 0$。

#### 命题 19 {#alg-iv-s5-prop-19 .statement tag=06DS}

— *设 M 为自由A-模，N A-模，G 为 A 的无限加法子群，并假设由 G 的非零元素定义的 N 的同伦是单射的。那么 Pol(M, N) 就是 Pol$^q$(M, N) 的直和。*

令 $f_0, f_1, \ldots, f_n$ 等于 $f_i \in \mathrm{Pol}^i(M, N)$ 并假设我们有关系 $f_0 + \ldots + f_n = 0$。让$x \in M$，那么对于所有$\lambda \in G$，我们有
$$
0 = \sum_{i=0}^n f_i(\lambda x) = \sum_{i=0}^n \lambda^i f_i(x).
$$
将引理 2 应用于多项式 $\sum_{i=0}^n f_i(x) X^i$ 我们有
$$
f_0(x) = \cdots = f_n(x) = 0
$$

#### 推论{#alg-iv-s5-n10-cor-1 .statement tag=06DT}

— *假设A是无穷大整环；设 M 为自由A-模，N 为无扭转 A 模块。*

(i) *我们有$\mathrm{Pol}(M, N) = \bigoplus_{q \geq 0} \mathrm{Pol}^q(M, N)$，每个$\mathrm{Pol}^q(M, N)$可以用$\mathrm{Hom}(\mathbf{T S}^q(M), N)$规范地识别。*

(ii) *设M的$f \in \mathrm{Pol}(M, N)$和$(e_i)_i$、基。N的元素中存在一个且仅有一个族$(u_\nu)_{\nu \in N^{(I)}}$，使得$f \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{\nu \in N^{(I)}} \lambda^\nu u_\nu$对于所有$(\lambda_i) \in A^{(I)}$。*

断言 (i) 由第 16 条和第 19 号提案得出，(ii) 由 (i) 和 Cor. 得出。提案 16。

### 11. $\mathbf{S}(M^*)$、TS(M)*gr 和 Pol(M, A) 之间的关系

令 M 为自由A-模，我们将为分级对偶 TS(M)*gr 配备可交换、结合和单位分级 $^1$ 代数的结构，源自 TS(M) 的分级余数结构 (III, p. 580)。到 III 时，p. 497 存在分级 A-代数的唯一同态
$$
\theta : \mathbf{S}(M^*) \to \mathbf{TS}(M)^{*gr}
$$
归纳出 M* 的次数 1 恒等映射。

$^1$ 将 TS(M) 的次数 – k 的同态分级到 A 中，此处被视为 TS(M)*gr 的次数 k 的元素 (II, p. 377)。

#### 命题 20 {#alg-iv-s5-prop-20 .statement tag=06DU}

— *如果 A-模 M 是自由且有限生成的，则 $0$ 是分级代数的同构。*

设$(e_i)_{i \in I}$为$M$之基，且$(e_i^*)_{i \in I}$对偶基为$M^*$。对于 $\nu \in \mathbf{N}^I$ 投入

$$
e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i) \in \mathbf{TS}(M)
$$

根据第 4 条（*IV*，p. 47），家庭$(e_\nu)_\nu,_{\mathbf{N}^I}$ 是基 / $TS(M)$；设$(e_\nu^*)$是$\mathbf{TS}(M)^{*gr}$右$(e_\nu)$的基。根据 III，p. 505，Th。 1 足以证明对于任何 $\nu \in \mathbf{N}^I$ 我们有

$$
e_\nu^* = \prod_{i \in I} (e_i^*)^{\nu_i},
$$

或者对于$\rho, \sigma \in \mathbf{N}^I$，我们有$e_\rho^* \cdot e_\sigma^* = e_{\rho + \sigma}^*$；但是这个最后一个断言是从 *IV*, p. 50, 公式 (12) 得出的。

#### 注 1 {#alg-iv-s5-n11-rem-1 .statement tag=06DV}

— 以同样的方式，我们看到如果$M$是有限生成的免费$A$模块，则III中定义的分级代数$S(M)^{*gr}$，p. 593可以用$TS(M^*)$来标识。

#### 命题 21 {#alg-iv-s5-prop-21 .statement tag=06DW}

— *典范同态 / A-模* (*IV*, p. 55)

$$
u : \mathbf{TS}(M)^{*gr} \to \mathrm{Pol}_A(M, A)
$$

*是代数同态。*

让$a \in \mathbf{TS}^q(M)^*, b \in TS^r(M)^*, x \in M$；我们有

$$
u(ab)(x) = \langle ab, \gamma_{q+r}(x) \rangle = \langle a \otimes b, c(\gamma_{q+r}(x)) \rangle =
= \langle a \otimes b, \gamma_q(x) \otimes \gamma_r(x) \rangle = \langle a, \gamma_q(x) \rangle \langle b, \gamma_r(x) \rangle = u(a)(x) \cdot u(b)(x),
$$

从而结果。

#### 注 {#alg-iv-s5-n11-rem-2 .statement tag=06DX}

— 2) 复合词同态$A, = u \circ 0 : S(M^*) \to \mathrm{Pol}_A(M, A)$是代数的唯一单位同态，包括

$$
M^* = \mathrm{Pol}^1(M, A)
$$

在$\mathrm{Pol}(M, A)$。如果 $M$ 是有限生成的自由且 $A$ 是无限的整环，则 $\lambda_M$ 是双射的（第 20 条命题和第 19 条命题的修正）。特别是，如果 $A$ 是无限整环，则 $A[X_1, \ldots, X_n]$ 的典范同态 $f \mapsto \tilde{f}$ 到 $\mathrm{Pol}(A^n, A)$ (*IV*, p. 4) 就是同构。

3) 考虑余积 $c_S : S(M^*) \to S(M^* \times M^*)$ (III, p. 575, 例 6)。对于任何 $v \in S(M^*)$、$x, y \in M$，多项式映射 $\lambda_{M \times M}(c_S(v)) : M \times M \to A$ 映射 $(x, y)$ 到 $A, (v)(x + y)$。对于以这种方式定义的$S(M^*)$到$\mathrm{Map}(M \times M, A)$的两个代数同态在$M^*$上一致，由于关系

$$
(v \otimes 1 + 1 \otimes v)(x, y) = v(x + y) \quad (v \in M^*)
$$

### 习题{#alg-iv-s5-exercises}

§ 5](exercises/s5/)参见[习题。
