---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 5
section_title: Symmetric tensors and polynomial mappings
lang: vi
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
statements: 36
exercises: 16
content_sha256: 273cbbbac0f6c1b6ed8269fa1faaa142c8df29d1035eed05417b5e3cb464ac91
translated_from: content/en/alg/IV/05_s5_symmetric_tensors_and_polynomial.md
source_content_sha256: 6da98969b53ee5df6cf503b3f80c244de4578e27ef1ee1edd5bf16c915b72321
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4, gpt-5.4-mini
translation_run: translate-vi-dfe81d24
glossary_version: 34
glossary_terms_sha256: 2b166281331bcc6a7ef1a2e13cd3fda05fe55a8e45dd52e7afb5c389c897f2ce
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. TENXƠ ĐỐI XỨNG VÀ CÁC ÁNH XẠ ĐA THỨC

### 1. Vết tương đối

Cho H là một nhóm và M là một A[H]-môđun trái $^{(1)}$. Ta sẽ ký hiệu $M^H$ là tập hợp tất cả các $m \in M$ sao cho $hm = m$ với mọi $h \in H$ $^{(2)}$; đây là một A-môđun con của M.

Cho G là một nhóm con của H, khi đó $M^G$ là một A-môđun con của M chứa $M^H$.

Cho $m \in M^G$, $h \in H$, nếu $x = hG$ là lớp ghép trái của h modulo G, thì ta có $xm = hGm = \{hm\}$. Do lạm dụng ký hiệu, phần tử $hm$ của M sẽ được viết là xm. Nếu $h' \in H$, ta có

(1)
$$
h'(xm) = (h'x) m .
$$

Từ đây về sau giả sử rằng G có chỉ số hữu hạn trong H. Khi đó

(2)
$$
\sum_{x \in H/G} xm \in M^H .
$$

Thật vậy, với $h' \in H$, theo (1), ta có

$$
h' \left( \sum_{x \in H/G} xm \right) = \sum_{x \in H/G} (h'x) m = \sum_{y \in H/G} ym .
$$

(1) Ta ký hiệu A[H] là đại số nhóm của H (III, p. 446).
(2) Cần chú ý không nhầm ký hiệu này với ký hiệu được đưa vào trong việc nghiên cứu các tích của các tập hợp (*Lý thuyết tập hợp*, II, p. 102).

#### Định nghĩa 1 {#alg-iv-s5-def-1 .statement}

— Nếu G *là* nhóm con có chỉ số hữu hạn trong H, ta ký hiệu $\mathrm{Tr}_{H/G}$ là ánh xạ từ $M^G$ vào $M^H$ được xác định bởi

$$
\mathrm{Tr}_{H/G} m = \sum_{x \in H/G} x m .
$$

Ánh xạ này là một đồng cấu của A-môđun $M^G$ vào A-môđun $M^H$.

#### Mệnh đề 1 {#alg-iv-s5-prop-1 .statement}

— (i) Cho $m \in M^G$ và $h \in H$. Khi đó $hm \in M^{hGh^{-1}}$ và

$$
\mathrm{Tr}_{H/hGh^{-1}}(hm) = \mathrm{Tr}_{H/G} m .
$$

(ii) Cho F là một nhóm con của G có chỉ số hữu hạn trong G, và cho $m \in M^F$, khi đó

$$
\mathrm{Tr}_{H/G}(\mathrm{Tr}_{G/F} m) = \mathrm{Tr}_{H/F} m
$$

(iii) *Nếu* $m \in M^H$, thì $\mathrm{Tr}_{H/G} m = (H : G) \cdot m$.

(i) Cho $h \in H$. Với $h' \in H$ và $m \in M$, đặt $\varphi(h') = hh'h^{-1}$ và $\psi(m) = hm$. Ta có $\varphi(h') \psi(m) = \psi(h'm)$; bằng phép chuyển cấu trúc ta suy ra rằng nếu $m \in M^G$, thì $hm \in M^{hGh^{-1}}$ và

$$
\mathrm{Tr}_{H/hGh^{-1}}(hm) = \psi(\mathrm{Tr}_{H/G}(m)) .
$$

Vì $\mathrm{Tr}_{H/G}(m) \in M^H$, điều này chứng minh (i).

(ii) Cho $m \in M^F$ và cho $(g_\alpha)_\alpha \in_A$ là một hệ các đại diện của các lớp ghép trái của G modulo F, và $(h_\beta)_\beta \in_B$ là một hệ các đại diện của các lớp ghép trái của H modulo G. Khi đó $(h_\beta g_\alpha)_{(\beta,\alpha) \in B \times A}$ là một hệ các đại diện của các lớp ghép trái của H modulo F. do đó

$$
\begin{align*}
\mathrm{Tr}_{H/G}(\mathrm{Tr}_{G/F} m) &= \sum_{\beta \in B} h_\beta \left( \sum_{\alpha \in A} g_\alpha m \right) \\
&= \sum_{(\beta,\alpha) \in B \times A} (h_\beta g_\alpha) m = \mathrm{Tr}_{H/F} m .
\end{align*}
$$

(iii) Mệnh đề này là hiển nhiên.

### 2. Định nghĩa các tenxơ đối xứng

Cho M là một A-môđun. Ta nhắc lại (III, p. 501) rằng $\mathfrak{S}_n$ tác động bên trái trên A-môđun $T^n(M)$, theo cách sao cho

$$
\sigma(x_1 \otimes x_2 \otimes \ldots \otimes x_n) = x_{\sigma^{-1}(1)} \otimes x_{\sigma^{-1}(2)} \otimes \ldots \otimes x_{\sigma^{-1}(n)}
$$

với mọi $x_1, \ldots, x_n \in M$ và $\sigma \in \mathfrak{S}_n$. Các phần tử $z \in T^n(M)$ sao cho $\sigma \cdot z = z$ với mọi $\sigma \in \mathfrak{S}_n$ được gọi là các tenxơ đối xứng cấp n; chúng tạo thành một A-môđun con của $T^n(M)$ được ký hiệu bởi $\mathbf{TS}^n(M)$; ta có $\mathbf{TS}^0(M) = A, \mathbf{TS}^1(M) = M$. Ta sẽ đặt

TS(M) = $\bigoplus_{n=0}^{\infty} TS^n(M)$; đây là một môđun con A-phân bậc của $\mathbf{T}(M)$. Với mọi $z \in T^n(M)$, phần tử $\sum_{\sigma \in S_n} \sigma . z$ thuộc $TS^n(M)$; ta ký hiệu nó bởi $s . z$ và gọi nó là phép đối xứng hóa của $z$. Ánh xạ $s : z \mapsto s . z$ là một đồng cấu của A-môđun $T^n(M)$ vào A-môđun $TS^n(M)$. Nếu $z \in TS^n(M)$, thì $s . z = n! \ z$.

### 3. Tích đối với các tenxơ đối xứng

Cho $p, q \in \mathbf{N}$ và cho $S_{p|q}$ là nhóm con của $S_{p+q}$ gồm tất cả các hoán vị $\sigma \in S_{p-q}$ giữ ổn định các khoảng $(1, p)$ và $(p+1, p+q)$ của $\mathbf{N}$. Nếu $\sigma \in S_p$ và $\sigma' \in S_q$, ta có thể định nghĩa một phần tử $\sigma''$ của $S_{p|q}$ bằng cách đặt $\sigma''(n) = \sigma(n)$ với $1 \leq n \leq p$ và $\sigma''(p+n) = p + \sigma'(n)$ với $1 \leq n \leq q$; ánh xạ $(\sigma, \sigma') \mapsto \sigma''$ là một đẳng cấu từ $S_p \times S_q$ lên $S_{p|q}$.

Cho $z \in TS^p(M)$, $z' \in TS^q(M)$, khi đó phần tử $z \otimes z'$ của $T^{p+q}(M)$ là bất biến dưới $S_{p|q}$; do đó ta có thể định nghĩa phần tử $\operatorname{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')$ của $TS^{p+q}(M)$. Ta trang bị cho $TS(M)$ phép nhân A-song tuyến tính $(y, y') \mapsto yy'$ sao cho với $p, q \in \mathbf{N}$, $z \in TS^p(M)$, $z' \in TS^q(M)$ ta có

$$
zz' = \operatorname{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')
$$

Nếu $y \in TS(M)$ và $y' \in TS(M)$, ta gọi $yy'$ là tích đối xứng của $y$ và $y'$. Họ $(TS^p(M))_p$, , là một phân bậc kiểu $\mathbf{N}$ của đại số $TS(M)$, và phần tử đơn vị của $\mathbf{T}(M)$ là một phần tử đơn vị của $TS(M)$.

Cho $S_{p,q}$ là tập hợp các $\sigma \in S_{p+q}$ sao cho

$$
\begin{align*}
&\sigma(1) < \sigma(2) < \ldots < \sigma(p) \\
&\sigma(p+1) < \sigma(p+2) < \ldots < \sigma(p+q).
\end{align*}
$$

Ánh xạ $(\sigma, \tau) \mapsto \sigma \tau$ từ $S_{p,q} \times S_{p|q}$ vào $S_{p+q}$ là song ánh (I, p. 60, Ví dụ 2); do đó nếu $z \in TS^p(M)$ và $z' \in TS^q(M)$, ta có

$$
zz' = \sum_{\sigma \in S_{p,q}} \sigma(z \otimes z')
$$

#### Mệnh đề 2 {#alg-iv-s5-prop-2 .statement}

— (i) Đại số trên A $TS(M)$ là kết hợp, giao hoán và có đơn vị.

(ii) Cho $p_1, \ldots, p_n$ là các số nguyên $> 0$, và cho $S_{p_1| \ldots |p_n}$ là tập hợp tất cả các $\sigma \in S_{p_1+\cdots+p_n}$ giữ ổn định các khoảng sau đây của $\mathbf{N}$:

$$
(1, p_1), (p_1+1, p_1+p_2), \ldots, (p_1+\cdots+p_{n-1}+1, p_1+\cdots+p_n).
$$

Cho $z_1 \in \mathbf{TS}^{p_1}(M) , \ldots , z_n \in \mathbf{TS}^{p_n}(M)$, khi đó

$$
z_1 z_2 \ldots z_n = \operatorname{Tr}_{\mathfrak{S}_{p_1 + \cdots + p_n}/\mathfrak{S}_{p_1}| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n) .
$$

Đặc biệt, nếu $x_1, \ldots, x_r \in M$, ta có $x_1 \ldots x_r = s(x_1 \otimes \ldots \otimes x_r)$.

Mệnh đề (ii) là hiển nhiên khi $n = 1$. Giả sử rằng quan hệ

$$
z_2 \ldots z_n = \operatorname{Tr}_{\mathfrak{S}_{p_2 + \cdots + p_n}/\mathfrak{S}_{p_2}| \cdots | p_n} (z_2 \otimes \ldots \otimes z_n)
$$

đã được chứng minh, và đồng nhất $\mathfrak{S}_{p_2 + \cdots + p_n}$ với nhóm con của $\mathfrak{S}_{p_1 + \cdots + p_n}$ gồm tất cả các hoán vị mà hạn chế trên $(1, p_1)$ là đồng nhất. Khi đó

$$
\operatorname{Tr}_{\mathfrak{S}_{p_1}|p_2+\cdots+p_n/\mathfrak{S}_{p_1}|p_2| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_r) =
$$
$$
= z_1 \otimes \operatorname{Tr}_{\mathfrak{S}_{p_2+\cdots+p_n}/\mathfrak{S}_{p_2}| \cdots | p_n} (z_2 \otimes \ldots \otimes z_r) = z_1 \otimes (z_2 \ldots z_n) .
$$

Do đó ta có

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

theo Mệnh đề 1, (ii) của IV, p. 42. Vậy (ii) được thiết lập.

Đặc biệt,

$$
z_1 (z_2 z_3) = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1}|p_2|p_3} (z_1 \otimes z_2 \otimes z_3) ,
$$

và tương tự, ta chứng minh rằng

$$
(z_1 z_2) z_3 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1}|p_2|p_3} (z_1 \otimes z_2 \otimes z_3) .
$$

Do đó đại số $\mathbf{TS}(M)$ là kết hợp.

Gọi $o$ là phần tử của $\mathfrak{S}_{p_1+p_2}$ sao cho

$$
\begin{align*}
\sigma(1) &= p_2 + 1, \; \sigma(2) = p_2 + 2, \; \ldots, \; \sigma(p_1) = p_2 + p_1 , \\
\sigma(p_1 + 1) &= 1, \; \sigma(p_1 + 2) = 2, \; \ldots, \; \sigma(p_1 + p_2) = p_2 .
\end{align*}
$$

Khi đó

$$
z_2 z_1 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_2}|p_1} (z_2 \otimes z_1)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\sigma \mathfrak{S}_{p_1}|p_2 \sigma^{-1}\sigma} (z_1 \otimes z_2)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_1}|p_2} (z_1 \otimes z_2) \quad \text{theo Mệnh đề 1, (i)}
$$
$$
= z_1 z_2 .
$$

Do đó đại số $\mathbf{TS}(M)$ là giao hoán.

Cần lưu ý rằng đơn ánh chính tắc của $\mathbf{TS}(M)$ vào $\mathbf{T}(M)$ nói chung không phải là một đồng cấu đại số. Tệ hơn nữa, $\mathbf{TS}(M)$ nói chung không ổn định đối với phép nhân của $\mathbf{T}(M)$.

### 4. Lũy thừa chia

Cho $x \in M$ và $k \in \mathbf{N}$. Hiển nhiên $x, \otimes x_2 \otimes \ldots \otimes x_k$, trong đó
$$
x_1 = x_2 = \cdots = x_k = x ,
$$
là một phần tử của $\mathbf{TS}^k(M)$.

#### Định nghĩa 2 {#alg-iv-s5-def-2 .statement}

*Nếu* $x \in M$, *phần tử* $x \otimes x \otimes \ldots \otimes x$ *của* $\mathbf{TS}^k(M)$ *được ký hiệu là* $\gamma_k(x)$.

#### Mệnh đề 3 {#alg-iv-s5-prop-3 .statement}

(i) *Nếu* $x \in M$, *lũy thừa bậc p của* $x$, *tính trong* $\mathbf{TS}(M)$, *bằng* $p! \; \gamma_p(x)$.
(ii) *Cho* $x,, \ldots, x, \in M$; *khi đó*
$$
\gamma_p(x_1 + x_2 + \cdots + x_n) = \sum_{p_1 + p_2 + \cdots + p_n = p} \gamma_{p_1}(x_1) \; \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) .
$$
(iii) *Cho* $x,, \ldots, x_n \in M$, *cho* $p_1, \ldots, p$, *là các số nguyên* $\geqslant 0$ *và* $p = p_1 + \ldots + p_n$. *Cho* $E$ *là tập hợp các ánh xạ* $\varphi$ *từ* $\{1, \ldots, p\}$ *vào* $(1, \ldots, n)$ *sao cho*
$$
\operatorname{Card} \varphi^{-1}(1) = p_1, \ldots, \operatorname{Card} \varphi^{-1}(n) = p_n .
$$
*Khi đó*
$$
\gamma_{p_1}(x_1) \; \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) = \sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes \ldots \otimes x_{\varphi(p)} .
$$
(iv) *Cho* $x \in M$ *và cho* $q, r$ *là các số nguyên* $\geqslant 0$. *Khi đó*
$$
\gamma_q(x) \; \gamma_r(x) = \frac{(q + r)!}{q! \; r!} \; \gamma_{q + r}(x) .
$$
(v) *Cho* $x_1, \ldots, x, \in M$, *và với* $H \subset (1, \ldots, n)$ *đặt* $x_H = \sum_{i \in H} x_i$, *khi đó*
$$
(-1)^n x_1 x_2 \ldots x_n = \sum_{H \subset \{1, \ldots, n\}} (-1)^{\operatorname{Card} H} \gamma_n(x_H) .
$$

Mệnh đề (i) suy ra ngay từ Mệnh đề 2 (ii).

Hãy chứng minh (ii); bằng một quy nạp theo n, ta thấy rằng chỉ cần xét trường hợp $n = 2$. Khi đó ta có

$$
\gamma_p(x_1 + x_2) = (x_1 + x_2) \otimes (x_1 + x_2) \otimes ... \otimes (x_1 + x_2) \quad @\text{thừa số})
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

Để chứng minh (iii), đặt $S_{p_1, ..., p_n}$ là tập hợp các hoán vị của $(1, p_1 + ... + p_n)$ mà các hạn chế của chúng trên các khoảng
$$(1, p_1), (p_1 + 1, p_1 + p_2), ..., (p_1 + ... + p_{n-1} + 1, p_1 + ... + p_n)$$
là tăng. Theo I, p. 60, ví dụ 2 và Mệnh đề 2, (ii) ta có
$$
\gamma_{p_1}(x_1) \gamma_{p_2}(x_2) ... \gamma_{p_n}(x_n) = \sum_{\rho \in S_{p_1, p_2, ..., p_n}} \rho(x_1 \otimes x_1 \otimes ... \otimes x_1 \otimes x_2 \otimes x_2 \otimes ... \otimes x_2 \otimes ... \otimes x_n \otimes x_n \otimes ... \otimes x_n)
$$
(với $p_i$ thừa số $x_i$) và tổng này bằng
$$
\sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes ... \otimes x_{\varphi(p)}.
$$

Trong (iii), đặt $n = 2, x_1 = x_2 = x, p_1 = q$ và $p_2 = r$, khi đó ta thu được (iv) (I, loc. cit.).

Cuối cùng, (v) suy ra từ Mệnh đề 2, (ii) và Mệnh đề 2 của I, p. 100, áp dụng cho các phần tử $x_i$ của vành $\mathbf{T}(M)$.

#### Nhận xét 1 {#alg-iv-s5-n4-rem-1 .statement}

Cho $(x_i)_{i \in I}$ là một họ các phần tử của M. Với mỗi $\nu \in \mathbf{N}^{(1)}$ đặt
$$
x_\nu = \prod_{i \in I} \gamma_{\nu_i}(x_i).
$$
Nếu $(\lambda_i) \in \mathbf{A}^{(1)}$ và $p \in \mathbf{N}$, thì theo Mệnh đề 3 (ii), ta có
$$
\gamma_p \left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{\nu \in \mathbf{N}^{(1)}, |\nu| = p} \lambda^\nu x_\nu.
$$
(6)

#### Nhận xét 2 {#alg-iv-s5-n4-rem-2 .statement}

Cho $\mathcal{M}$ là tập hợp các ánh xạ từ $(1, p)$ vào I. Ta định nghĩa một ánh xạ $\rho \mapsto \rho^*$ từ $\mathcal{M}$ vào $\mathbf{N}^{(1)}$ bằng cách đặt
$$
\rho^*(i) = \operatorname{Card} \rho^{-1}(i)
$$

Đối với hai phần tử $\rho_1, \rho_2$ của $\mathcal{M}$, điều kiện $\rho_1^* = \rho_2^*$ là cần và đủ để tồn tại $\sigma \in \mathfrak{S}_p$ sao cho $\rho_2 = \rho_1 \circ \sigma$ (I, p. 95). Theo Mệnh đề 3 (iii), với $|\nu| = p$, ta có

$$
x_\nu = \sum_{\rho \in \mathcal{M}, \rho^* = \nu} x_{\rho(1)} \otimes x_{\rho(2)} \otimes \ldots \otimes x_{\rho(p)}
$$

### 5. Tenxơ đối xứng trên một môđun tự do

#### Mệnh đề 4 {#alg-iv-s5-prop-4 .statement}

— Cho $M$ là tự do và $(e_i)_{i \in I}$ là một cơ sở của $M$.

(i) Với $\nu \in \mathbf{N}^{(I)}$, đặt $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$. Khi đó $(e,)_{\nu \in \mathbf{N}^{(I)}}$ là một cơ sở của $A$-môđun $TS(M)$. Đặc biệt, đại số $\mathbf{TS}(M)$ được sinh bởi họ các phần tử $\gamma_k(x)$ với $k \in N$ và $x \in M$.

(ii) Với mỗi $p \in N$, $\mathbf{TS}^p(M)$ là một nhân tử trực tiếp của $A$-môđun $\mathbf{T}^p(M)$.

Ta dùng ký hiệu của Nhận xét 2 ở trên. Họ $(e_{\rho(1)} \otimes \ldots \otimes e_{\rho(p)})_{\rho \in \mathcal{M}}$ là một cơ sở của $\mathbf{T}^p(M)$. Do đó Mệnh đề 4 suy ra từ công thức (7) và bổ đề sau đây, áp dụng với $H = \mathfrak{S}_p$ và $U = \mathbf{T}^p(M)$.

#### Bổ đề 1 {#alg-iv-s5-lem-1 .statement}

Cho $H$ là một nhóm hữu hạn và $U$ là một $A[H]$-môđun trái. Giả sử $A$-môđun $U$ có một cơ sở $B$ ổn định dưới các phép toán của $H$ trong $U$, và đặt $\Omega = B/H$. Với mỗi $w \in \Omega$, đặt $u_w = \sum_{b \in w} b$; khi đó

(i) $(u_w)_{w \in \Omega}$ là một cơ sở của $A$-môđun $U^H$.

(ii) Với mỗi $\omega \in \Omega$, lấy $v$, là một điểm của $\omega$; đặt $\omega' = w - \{v_\omega\}$ và $B' = \bigcup_{\omega \in \Omega} w'$, khi đó $B'$ là một cơ sở của một không gian con bổ sung cho $U^H$ trong $U$.

Hợp của tập hợp tất cả các $u_w$ (với $\omega \in \Omega$) và của $B'$ là một cơ sở của $U$. Nếu $U' = \sum_{\omega \in \Omega} Au$, và $U'' = \sum_{b \in B'} Ab$, do đó ta có $U = U' \oplus U''$. Mặt khác, ta có $u_w \in U^H$ với mọi $w \in \Omega$, nên $U' \subset U^H$. Cuối cùng, cho $(\alpha_b)_{b \in B}$ là một họ các phần tử của $A$ có giá hữu hạn và đặt $x = \sum_{b \in B} \alpha_b b$. Nếu $x \in U^H$, thì $\alpha_{hb} = \alpha_b^H$ với mọi $b \in B$ và mọi $h \in H$, nên $x \in U'$, và suy ra $U' = u^H$.

#### Mệnh đề 5 {#alg-iv-s5-prop-5 .statement}

— Cho $M$ là một A-môđun tự do, $k$ một số nguyên $\geq 0$, $P$ A-môđun con của $\mathbf{TS}^k(M)$ được sinh bởi $\gamma_k(M)$. Giả sử $A$ là một miền nguyên vô hạn. Khi đó với mỗi $z \in \mathbf{TS}^k(M)$ tồn tại $a \in A - \{0\}$ sao cho $az \in P$.

Gọi $K$ là trường phân thức của $A$. Ta đồng nhất $\mathbf{TS}^k(M)$ với một A-môđun con của không gian vectơ K $V = \mathbf{TS}^k(M) \otimes_A K$ (Mệnh đề 4, và II, p. 314). Ta phải chỉ ra rằng không gian vectơ K này được sinh bởi $\gamma_k(M)$, tức là, mọi dạng tuyến tính K $f$ trên V thỏa mãn $f(\gamma_k(M)) = 0$ đều bằng không. Cho $(e_i)_{i \in I}$ là một cơ sở của M, và định nghĩa các $e_\nu$ như trong Mệnh đề 4. Với mọi $(\alpha_i) \in A^{(I)}$ ta có, khi lưu ý đến (6),

$$
0 = f \left( \gamma_k \left( \sum_{i \in I} \alpha_i e_I \right) \right) = \sum_{\nu \in N^{(I)}, |\nu| = k} \alpha^\nu f(e_\nu).
$$

Theo Hệ quả 2 của IV, p. 18 suy ra $f(e_v) = 0$ với mọi $v \in N^{(I)}$, do đó $f = 0$.

### 6. Hàm tử TS

Cho M, N là các A-môđun và u một đồng cấu từ M vào N; hiển nhiên là $T(u)(TS(M)) \subset TS(N)$. Ánh xạ từ TS(M) vào TS(N) thu được từ T(u) được ký hiệu là TS(u). Dễ dàng kiểm tra rằng đó là một đồng cấu có đơn vị của các đại số phân bậc và ta có TS(u) $(\gamma_p(x)) = \gamma_p(u(x))$ với mọi $x \in M$ và mỗi số nguyên $p \geq 0$. Nếu $v : N \to P$ là một đồng cấu các A-môđun, ta có

$$
TS(v \circ u) = TS(v) \circ TS(u).
$$

Theo định nghĩa của TS(u), biểu đồ

$$
\begin{array}{cccc}
M & \longrightarrow & TS(M) \longrightarrow T(M) \\
u \downarrow & & \downarrow TS(u) & \downarrow T(u) \\
N & \longrightarrow & TS(N) \longrightarrow T(N)
\end{array}
$$

là giao hoán, trong đó các mũi tên ngang biểu thị các đơn ánh chính tắc.

Nếu M là một nhân tử trực tiếp của N và i : M \to N là đơn ánh chính tắc, thì TS(i) là một đơn cấu của TS(M) lên một nhân tử trực tiếp R của TS(N), nhờ đó ta thường đồng nhất TS(M) và R. Điều đó được chứng minh như đối với đại số tenxơ (III, p. 487).

Giả sử M là tổng trực tiếp của một họ $(M_\lambda)_{\lambda \in L}$ các môđun con. Các đơn ánh chính tắc $TS(M_\lambda) \to TS(M)$ xác định một đồng cấu có đơn vị của các đại số phân bậc, được gọi là chính tắc:

$$
\bigotimes_{\lambda \in L} TS(M_\lambda) \to TS(M)
$$

Cho $\lambda_1, \lambda_2, \ldots, \lambda_n$ là các phần tử từng đôi một phân biệt của L và cho $x_1 \in M_{\lambda_1}, \ldots, x_n \in M_{\lambda_n}$. Theo Mệnh đề 3, (ii) của IV, p. 45 ta có

$$
h \left( \sum_{p_1 + \cdots + p_n = p} \gamma_{p_1}(x_1) \otimes \cdots \otimes \gamma_{p_n}(x_n) \right) = \gamma_p(x_1 + \cdots + x_n).
$$

Cho $N$ là một $A$-môđun là tổng trực tiếp của một họ $(N_\lambda)_\lambda$ các môđun con. Với mọi $\lambda \in L$, cho $u_\lambda$ là một đồng cấu từ $M_\lambda$ vào $N_\lambda$. Cho $u$ là đồng cấu từ $M$ vào $N$ được xác định bởi các $u_\lambda$. Khi đó biểu đồ

$$
\begin{array}{ccc}
\otimes \mathbf{TS}(M_\lambda) & \xrightarrow{h} & \mathbf{TS}(M) \\
\downarrow & & \downarrow \mathbf{TS}(u) \\
\otimes \mathbf{TS}(u_\lambda) & & \\
\downarrow & & \\
\otimes \mathbf{TS}(N_\lambda) & \xrightarrow{h'} & \mathbf{TS}(N)
\end{array}
$$

giao hoán, trong đó $h$ và $h'$ là các đồng cấu chính tắc. Thật vậy, nếu $z \in TS(M_\lambda)$ và nếu $i_\lambda$ (resp. $j_\lambda$) ký hiệu đơn ánh chính tắc của $M_\lambda$ vào $M$ (resp. $N$, vào $N$), thì ta có

$$
\mathbf{TS}(u)(h(z)) = \mathbf{TS}(u) \circ \mathbf{TS}(i_\lambda)(z) = \mathbf{TS}(u \circ i_\lambda)(z) =
$$
$$
= \mathbf{TS}(j_\lambda \circ u_\lambda)(z) = \mathbf{TS}(j_\lambda) \circ \mathbf{TS}(u_\lambda)(z) = h'(\mathbf{TS}(u_\lambda)(z)) .
$$

#### Mệnh đề 6 {#alg-iv-s5-prop-6 .statement}

— *Cho $M$ là một $A$-môđun là tổng trực tiếp của một họ $(M_\lambda)_\lambda$ các môđun con. Nếu mỗi $M_\lambda$ là một môđun tự do, thì đồng cấu chính tắc từ $\otimes_{\lambda \in L} \mathbf{TS}(M_\lambda)$ vào $\mathbf{TS}(M)$ là một đẳng cấu.*

Cho $(e_{i,\lambda})_{i, I_\lambda}$ là một cơ sở của $M_\lambda$. Với $\nu \in \mathbf{N}^{(I_\lambda)}$, đặt $e_{\nu,\lambda} = \prod_{i \in I_\lambda} \gamma_{\nu(i)}(e_{i,\lambda})$. Các $e_{\nu,\lambda}$ với $\nu \in \mathbf{N}^{(I_\lambda)}$ lập thành một cơ sở của $TS(M_\lambda)$ (IV, p. 47, Mệnh đề 4 (i)) và $e_{0,\lambda}$ là phần tử khả nghịch của $\mathbf{TS}(M_\lambda)$. Do đó các phần tử

$$
\otimes_{\lambda \in L} e_{\nu_{\lambda,\lambda}}
$$

với $\nu_\lambda \in \mathbf{N}^{(I_\lambda)}$ và $\nu_\lambda = 0$ trừ một số hữu hạn chỉ số, lập thành một cơ sở của $\otimes_A TS(M_\lambda)$. Ảnh của phần tử (9) qua đồng cấu chính tắc của mệnh đề là $\prod_{\lambda \in L} e_{\nu_{\lambda,\lambda}}$. Nếu ký hiệu $(e_i)_i$ là hợp rời nhau của các họ $(e_{i,\lambda})_{i, I_\lambda}$, thì các phần tử trên chính xác là $\prod_{i \in I} \gamma_{\nu(i)}(e_i)$, trong đó $\nu \in \mathbf{N}^{(I)}$, và do đó chúng lập thành một cơ sở của $\mathbf{TS}(M)$. Điều này chứng minh mệnh đề.

Dưới các điều kiện của Mệnh đề 6, đẳng cấu nghịch đảo $\mathbf{TS}(M) \to \otimes_{\lambda} \mathbf{TS}(M_\lambda)$ cũng được gọi là *chính tắc*. Thường xuyên $\mathbf{TS}(M)$ được đồng nhất với $\otimes_{\lambda} TS(M_\lambda)$ bằng đẳng cấu này. Cần lưu ý rằng nếu $z \in TS(M_\lambda)$ và $z' \in \mathbf{TS}(M_{\mu})$ với $\lambda \neq \mu$, thì phần tử của $\mathbf{TS}(M)$ mà ta được dẫn đến để ký hiệu là $z \otimes z'$ không phải là tích tenxơ của $z$ và $z'$ trong $\mathbf{T}(M)$ mà là tích đối xứng của $z$ và $z'$.

#### Mệnh đề 7 {#alg-iv-s5-prop-7 .statement}

*Cho $M$ là một $A$-môđun, $u$ là ánh xạ $(x, y) \mapsto x + y$ của $M \oplus M$ vào $M$ và $f$ là ánh xạ hợp*

$$
\mathbf{TS}(M) \otimes \mathbf{TS}(M) \xrightarrow{h} \mathbf{TS}(M \oplus M) \xrightarrow{\mathbf{TS}(u)} \mathbf{TS}(M)
$$

*trong đó $h$ là đồng cấu chính tắc. Nếu $z, z' \in \mathbf{TS}(M)$, thì $f(z \otimes z') = zz'$.*

Vì $i$ là ánh xạ $x \mapsto (x, 0)$ của $M$ vào $M \oplus M$. Ta có $u \circ i = \mathrm{Id}_M$, do đó $\mathbf{TS}(u) \circ \mathbf{TS}(i) = \mathrm{Id}_{\mathbf{TS}(M)}$; vì thế

$$
f(z \otimes 1) = \mathbf{TS}(u)(h(z \otimes 1)) = \mathbf{TS}(u)(\mathbf{TS}(i)(z)) = z .
$$

Tương tự $f(1 \otimes z') = z'$, do đó $f(z \otimes z') = f(z \otimes 1) f(1 \otimes z') = zz'$.

### 7. Đồng tích cho các tenxơ đối xứng

Cho $M$ là một $A$-môđun *tự do*, và $\Delta_M = A$ là đồng cấu đường chéo $x \mapsto (x, x)$ của $M$ vào $M \oplus M$. Cho $c_M = c$ là đồng cấu có đơn vị của các đại số $A$ phân bậc hợp thành bởi các đồng cấu :

$$
\mathbf{TS}(M) \xrightarrow{\mathbf{TS}(\Delta)} \mathbf{TS}(M \oplus M) \xrightarrow{\sigma} \mathbf{TS}(M) \otimes \mathbf{TS}(M)
$$

trong đó $\sigma$ là đẳng cấu chính tắc. Được trang bị $c$, $\mathbf{TS}(M)$ là một đối đại số $A$ phân bậc.

Với mọi $x \in M$ và mỗi số nguyên $p \geq 0$ ta có $\mathbf{TS}(A)(\gamma_p(x)) = \gamma_p((x, x))$, do đó theo (8),

$$
c(\gamma_p(x)) = \sum_{r+s=p} \gamma_r(x) \otimes \gamma_s(x).
$$

Đặc biệt

$$
c(x) = x \otimes 1 + 1 \otimes x .
$$

Cho $(x_i)_{i \in I}$ là một họ các phần tử của $M$, và với $\nu \in \mathbf{N}^{(I)}$ đặt $x_\nu = \prod_{i \in I} \gamma_{\nu_i}(x_i)$.

Khi đó

$$
c(x_\nu) = \sum_{\rho + \sigma = \nu} x_\rho \otimes x_\sigma .
$$

Điều này suy ra từ *(10)* vì $c$ là một đồng cấu đại số.

#### Mệnh đề 8 {#alg-iv-s5-prop-8 .statement}

— Cho M là một A-môđun tự do, khi đó với các cấu trúc đại số và đối đại số của nó, TS (M) là một song đại số phân bậc giao hoán và đối giao hoán. Đồng đơn vị là ánh xạ A-tuyến tính $\varepsilon : TS(M) \to TS^0(M) = A$ bằng không trên $TS^p(M)$ với $p > 0$ và sao cho $\varepsilon(1) = 1$.

Ta biết rằng A-đại số $TS(M)$ là kết hợp, giao hoán và có đơn vị. Mặt khác, đồng tích theo phép dựng là một đồng cấu của các đại số phân bậc; bây giờ việc đối đại số $TS(M)$ là đối kết hợp và đối giao hoán suy ra bằng một phép tính dễ dàng từ Công thức (10). Ánh xạ $\varepsilon$ từ $TS(M)$ vào A là một đồng cấu của các đại số phân bậc sao cho $\varepsilon(l) = l$. Cuối cùng với mọi $x \in M$ ta có $\varepsilon(\gamma_p(x)) = 0$ nếu $p > 0$, $\varepsilon(\gamma_0(x)) = l$; nếu lưu ý đến (lo), điều này cho thấy rằng $(F \otimes 1) \circ c = (l \otimes E) \circ c = \mathrm{Id}_{TS(M)}$; do đó $E$ là đồng đơn vị của $TS(M)$.

#### Mệnh đề 9 {#alg-iv-s5-prop-9 .statement}

— Cho M và N là các A-môđun tự do và u là một A-đồng cấu từ M vào N; khi đó $\mathbf{TS}(u)$ là một đồng cấu song đại số.

Thật vậy ta có $\Delta_N \circ u = (u,u) \circ \Delta_M$, do đó biểu đồ

$$
\begin{array}{ccccccccc}
\mathbf{TS}(M) & \xrightarrow{\mathbf{TS}(\Delta_M)} & \mathbf{TS}(M \oplus M) & \xrightarrow{\sigma} & \mathbf{TS}(M) \otimes \mathbf{TS}(M) \\
\downarrow \mathbf{TS}(u) & & \downarrow \mathbf{TS}(u,u) & & \downarrow \mathbf{TS}(u) \otimes \mathbf{TS}(u) \\
\mathbf{TS}(N) & \xrightarrow{\mathbf{TS}(\Delta_N)} & \mathbf{TS}(N \oplus N) & \xrightarrow{\tau} & \mathbf{TS}(N) \otimes \mathbf{TS}(N),
\end{array}
$$

trong đó $\sigma$ và $\tau$ là các đẳng cấu chính tắc, là giao hoán (IV, p. 49). Vậy $c_N \circ \mathbf{TS}(u) = (\mathbf{TS}(u) \otimes \mathbf{TS}(u)) \circ c_M$.

#### Mệnh đề 10 {#alg-iv-s5-prop-10 .statement}

— Cho M là một A-môđun tự do, khi đó các phần tử nguyên thủy (III, p. 602) của song đại số $\mathbf{TS}(M)$ là các phần tử của M.

Cho $(e_i)_{i \in I}$ là một cơ sở của M, và với $v \in \mathbf{N}^{(I)}$ đặt $e_v = \prod_{i \in I} \gamma_{v_i}(e_i)$. Cho $z = \sum_{v \in \mathbf{N}^{(I)}} \lambda_v e_v$ là một phần tử của $\mathbf{TS}(M)$, khi đó theo (12) ta có

$$
c(z) = \sum_v \lambda_v \sum_{\rho, \sigma \in \mathbf{N}^{(I)}, \rho + \sigma = v} e_\rho \otimes e_\sigma = \sum_{\rho, \sigma} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma
$$

do đó

$$
c(z) - 1 \otimes z - z \otimes 1 = \sum_{\rho \neq 0, \sigma \neq 0} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma - \lambda_0 e_0 \otimes e_0
$$

và vì thế

z nguyên thủy $\Leftrightarrow \lambda_{\rho + \sigma} = 0$ khi $\rho \neq 0$ và $\sigma \neq 0$ và $\lambda_0 = 0$
$\Leftrightarrow \lambda_v = 0$ khi $|v| \neq 1$
$\Leftrightarrow z \in M$.

### 8. Các quan hệ giữa TS(M) và S(M)

Đơn ánh chính tắc từ M vào TS(M) mở rộng một cách duy nhất thành một đồng cấu đại số từ T(M) vào TS(M) (III, p. 485, Prop. 1). Theo Mệnh đề 2, (ii) của IV, p. 43, đồng cấu này là các toán tử đối xứng hóa. Vì đại số TS(M) là giao hoán nên tồn tại (III, p. 497) một và chỉ một đồng cấu đại số $\varphi_M$, gọi là chính tắc, từ đại số S(M) vào đại số TS(M) sao cho biểu đồ

$$
\begin{array}{ccc}
T(M) & \xrightarrow{\rho} & S(M) \\
& & \searrow s \\
& & TS(M)
\end{array}
$$

trong đó $\rho$ ký hiệu đồng cấu chính tắc từ T(M) lên S(M), là giao hoán. Ta có $\varphi_M(S^p(M)) \subset TS^p(M)$ với mọi $p \in \mathbf{N}$.

Mặt khác, bằng cách hợp thành đơn ánh chính tắc i của TS(M) vào T(M) với đồng cấu chính tắc $\rho$ từ T(M) lên S(M), ta thu được một đồng cấu của các A-môđun phân bậc $\psi_M$, gọi là chính tắc. Biểu đồ

$$
\begin{array}{ccc}
TS(M) & \xrightarrow{\psi_M} & S(M) \\
& & \downarrow \rho \\
& & T(M)
\end{array}
$$

là giao hoán.

Nếu $u : M \to N$ là một đồng cấu của các A-môđun, thì biểu đồ

$$
\begin{array}{ccccccccc}
S(M) & \xrightarrow{\varphi_M} & TS(M) & \xrightarrow{\psi_M} & S(M) \\
| & & | & & | \\
S(N) & \xrightarrow{\varphi_N} & TS(N) & \xrightarrow{\psi_N} & S(N)
\end{array}
$$

là giao hoán, như dễ dàng kiểm tra được.

Nếu M là tổng trực tiếp của các môđun $M_\lambda$, thì biểu đồ (14)

$$
\begin{array}{ccc}
\otimes S(M_\lambda) & \xrightarrow{\otimes \varphi_{M_\lambda}} & \otimes TS(M_\lambda) \\
\downarrow f & & \downarrow g \\
S(M) & \xrightarrow{\varphi_M} & TS(M),
\end{array}
$$

trong đó $f$ và $g$ là các đồng cấu chính tắc, là giao hoán. Thật vậy, $g \circ \otimes \varphi_{M_\lambda}$ và $\varphi_M \circ f$ là các đồng cấu đại số trùng nhau trên $M_\lambda$ với mọi $\lambda$.

#### Mệnh đề 11 {#alg-iv-s5-prop-11 .statement}

— *Nếu $M$ là tự do, thì $\varphi_M$ là một cấu xạ của các song đại số phân bậc.*

Dùng tính giao hoán của các biểu đồ (13) và (14), ta được biểu đồ giao hoán

$$
\begin{array}{ccccccccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \oplus M) & \xrightarrow{h} & S(M) \otimes S(M) \\
\downarrow \varphi_M & & \downarrow \varphi_{M \oplus M} & & \downarrow \varphi_M \otimes \varphi_M \\
TS(M) & \xrightarrow{TS(\Delta)} & TS(M \oplus M) & \xrightarrow{k} & TS(M) \otimes TS(M),
\end{array}
$$

trong đó $\Delta$ là đồng cấu đường chéo và $h, k$ là các đồng cấu chính tắc. Mệnh đề suy ra từ điều này.

#### Mệnh đề 12 {#alg-iv-s5-prop-12 .statement}

— (i) *Nếu $u \in S^n(M)$, thì $\psi_M(\varphi_M(u)) = n!u$.*

(ii) *Nếu $v \in TS^n(M)$ thì $\varphi_M(\psi_M(v)) = n!v$.*

Cho $x_1, \ldots, x_n \in M$ và gọi $u$ là tích $x_1 \ldots x_n$ tính trong $S(M)$. Khi đó $\varphi_M(u)$ là tích $x_1 \ldots x_n$ tính trong $TS(M)$, nghĩa là

$$
\sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)}.
$$

Do đó $\psi_M(\varphi_M(u))$ bằng $\sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \ldots x_{\sigma(n)}$ tính trong $S(M)$, nghĩa là

$$
n! x_1 \ldots x_n = n!u.
$$

Cho $v = \sum_{i=1}^p x_1^i \otimes x_2^i \otimes \ldots \otimes x_n^i$ là một phần tử của $TS^n(M)$, trong đó các $x_j^i$ thuộc $M$; khi đó $\psi_M(v)$ bằng $\sum_{i=1}^p x_1^i x_2^i \ldots x_n^i$ tính trong $S(M)$, do đó

$$
\varphi_M(\psi_M(v)) = \sum_{i=1}^p s(x_1^i \otimes x_2^i \otimes \ldots \otimes x_n^i) = s(v) = n!v.
$$

#### Hệ quả 1 {#alg-iv-s5-prop-12-cor-1 .statement}

— *Nếu $\mathbf{A}$ là một $\mathbf{Q}$-đại số, thì đồng cấu chính tắc từ $S(M)$ vào $TS(M)$ là một đẳng cấu đại số. Hơn nữa, nếu $M$ là tự do, thì đó là một đẳng cấu của các song đại số phân bậc.*

#### Hệ quả 2 {#alg-iv-s5-prop-12-cor-2 .statement}

— *Nếu $A$ là một $\mathbf{Q}$-đại số thì môđun $TS^n(M)$ được sinh bởi các lũy thừa bậc n của các phần tử của $M$ trong $TS(M)$.
Điều này suy ra từ Hệ quả 1 và tính chất tương ứng của $S(M)$* (III, p. 498).

### 9. Ánh xạ đa thức thuần nhất

#### Mệnh đề 13 {#alg-iv-s5-prop-13 .statement}

— *Cho $M$ và $N$ là các $A$-môđun, $q$ là một số nguyên $\geqslant 0$, và $f$ là một ánh xạ từ $M$ vào $N$. Giả sử rằng $M$ là tự do, khi đó các điều kiện sau là tương đương:
(i) Tồn tại một ánh xạ $q$-tuyến tính $g$ từ $M^q$ vào $N$ sao cho $f(x) = g(x, x, \ldots, x)$ với mọi $x \in M$.
(ii) Tồn tại một ánh xạ tuyến tính $h$ từ $TS^q(M)$ vào $N$ sao cho $f(x) = h(\gamma_q(x))$ với mọi $x \in M$.
(iii) Tồn tại một cơ sở $(e_i)_{i \in I}$ của $M$ và một họ $(u_v)_{v \in N^{(1)}, |v| = q}$ các phần tử của $N$ sao cho
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{v \in N^{(1)}, |v| = q} \lambda^v u_v
$$
với mọi $(\lambda_i) \in A^{(1)}$.
(iv) Với mỗi cơ sở $(e_i)_{i \in I}$ của $M$ tồn tại một họ $(u_v)_{v \in N^{(1)}, |v| = q}$ các phần tử của $N$ sao cho
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{v \in N^{(1)}, |v| = q} \lambda^v u_v
$$
với mọi $(\lambda_i) \in A^{(1)}$.
(i) $\Rightarrow$ (ii): giả sử $g$ thỏa mãn (i), khi đó tồn tại một ánh xạ tuyến tính $g'$ từ $T^q(M)$ vào $N$ sao cho $g(x_1, x_2, \ldots, x_q) = g'(x_1 \otimes x_2 \otimes \ldots \otimes x)$ với mọi $x, \ldots, x, \in M$. Khi đó
$$
f(x) = g(x, x, \ldots, x) = g'(x \otimes x \otimes \ldots \otimes x) = g'(\gamma_q(x));
$$
và khi viết $h = g'|TS^q(M)$ ta thấy rằng điều kiện (ii) được thỏa mãn.
(ii) $\Rightarrow$ (i) và (iv): giả sử $h$ thỏa mãn các điều kiện của (ii). Theo Mệnh đề 4, (ii) (IV, p. 47) tồn tại một ánh xạ tuyến tính $g'$ từ $T^q(M)$ vào $N$ sao cho $h = g'|TS^q(M)$. Gọi $g$ là ánh xạ $q$-tuyến tính từ $M$ vào $N$ liên kết với $g'$, khi đó với mọi $x \in M$ ta có
$$
f(x) = h(\gamma_q(x)) = g'(x \otimes x \otimes \ldots \otimes x) = g(x, x, \ldots, x),
$$

do đó có (i). Mặt khác, nếu $(e_i)_{i \in I}$ là một cơ sở của M, thì theo công thức (6) (IV, p. 46) ta có

$$
f \left( \sum_i \lambda_i e_i \right) = h \left( \gamma_q \left( \sum_i \lambda_i e_i \right) \right) = h \left( \sum_{|\nu|=q} \lambda^\nu e_\nu \right)
$$

khi viết $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$; do đó ta có

$$
f \left( \sum_i \lambda_i e_i \right) = \sum_{|\nu|=q} \lambda^\nu h(e_\nu).
$$

(iv) $\Rightarrow$ (iii) là hiển nhiên.
(iii) $\Rightarrow$ (ii): cho $(e_i), (u,)$ thỏa mãn các điều kiện của (iii), đặt $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$ và nhắc lại rằng $(e_\nu)_{|\nu|=q}$ là một cơ sở của $\mathrm{TS}^q(M)$. Gọi h là đồng cấu từ $\mathrm{TS}^q(M)$ vào N được xác định bởi $h(e_\nu) = u_\nu$; khi đó với mỗi $x = \sum_i \lambda_i e_i$ trong M ta có

$$
f(x) = f \left( \sum_i \lambda_i e_i \right) = \sum_{|\nu|=q} \lambda^\nu u_\nu = h \left( \sum_{|\nu|=q} \lambda^\nu e_\nu \right) = h(\gamma_q(x))
$$

#### Định nghĩa 3 {#alg-iv-s5-def-3 .statement}

— Cho M và N là các A-môđun và q là một số nguyên $\geq 0$. Giả sử rằng M là *tự do*, và ký hiệu bởi $\mathrm{Pol}_A^q(M, N)$ hoặc đơn giản là $\mathrm{Pol}^q(M, N)$ tập hợp các ánh xạ từ M vào N thỏa mãn các điều kiện của Mệnh đề 13. Các phần tử của $\mathrm{Pol}^q(M, N)$ được gọi là các ánh xạ đa thức thuần nhất bậc q từ M vào N.

Mệnh đề 13 (i) xác định một đồng cấu của các A-môđun:

$$
\mathcal{L}_q(M, ..., M; N) \to \mathrm{Pol}^q(M, N).
$$

Mệnh đề 13 (ii) xác định một đồng cấu của các A-môđun

$$
\mathrm{Hom}_A(\mathbf{TS}^q(M), N) \to \mathrm{Pol}^q(M, N).
$$

Các đồng cấu này được gọi là chính tắc. Chúng toàn ánh.

#### Ví dụ 1 {#alg-iv-s5-n9-exa-1 .statement}

Các ánh xạ đa thức thuần nhất bậc 1 từ M vào N là các ánh xạ A-tuyến tính từ M vào N.
2) Cho $(N_i)_{i \in I}$ là một họ các A-môđun, $f_i$ là một ánh xạ từ M vào $N_i, i \in I$, và $f : M \to \prod_{i \in I} N_i$ là ánh xạ có các thành phần là $f_i$. Để f là một ánh xạ đa thức thuần nhất bậc q thì điều kiện cần và đủ là mỗi $f_i$ đều là một ánh xạ đa thức thuần nhất bậc q.
3) Cho $(M_j)_{j \in J}$ là một họ hữu hạn các A-môđun tự do và $u : \prod_{j \in J} M_j \to N$ là một ánh xạ đa tuyến tính; khi đó u là đa thức bậc $\mathrm{Card}(J)$.

4) Cho $(X_i)_{i \in I}$ là một họ các ẩn, $N$ là một $A$-môđun và $u \in N[(X_i)_{i \in I}]$ là một đa thức thuần nhất bậc $q$. Ánh xạ $(x_i)_{i \in I} \mapsto u((x_i)_{i \in I})$ từ $A^{(I)}$ vào $N$ là một ánh xạ đa thức thuần nhất bậc $q$: điều này thấy ngay từ điều kiện (iii) của Mệnh đề 13. Nếu $I$ là hữu hạn, mọi ánh xạ đa thức thuần nhất bậc $q$ từ $A^{(I)} = A'$ vào $N$ đều có dạng đó.

5) Ánh xạ $(x_i)_{i \in N} \mapsto x_0^2 + x_1^2 + \ldots + x_n^2 + \ldots$ từ $A^{(N)}$ vào $A$ là một ánh xạ đa thức thuần nhất bậc 2. Nếu $A = 2/22$, nó trùng với ánh xạ tuyến tính $(x_i)_{i \in I} \mapsto x_0 + x_1 + \ldots + x_n + \ldots$

6) Cho $f \in \mathrm{Pol}_A^q(M, N)$, cho $B$ là một vành giao hoán, $\rho$ là một đồng cấu từ $B$ vào $A$ và $M'$ và $N'$ là các $B$-môđun dẫn xuất từ $M$ và $N$ bằng $\rho$. Giả sử rằng $M'$ là tự do; khi đó $f \in \mathrm{Pol}_B^q(M', N')$: điều này suy ra ngay từ điều kiện (i) của Mệnh đề 13.

#### Mệnh đề 14 {#alg-iv-s5-prop-14 .statement}

— Cho $M, N, P$ là các $A$-môđun, $q$ và $r$ là các số nguyên $\geqslant 0$, và giả sử rằng $M$ và $N$ tự do. Nếu $f \in \mathrm{Pol}^q(M, N)$, $f' \in \mathrm{Pol}^r(N, P)$, thì $f' \circ f \in \mathrm{Pol}^{qr}(M, P)$.

Tồn tại một ánh xạ $q$-tuyến tính $g$ của $M^q$ vào $N$ và một ánh xạ $r$-tuyến tính $g'$ của $N^r$ vào $P$ sao cho

$$
\begin{aligned}
f(x) &= g(x, x, \ldots, x) & \text{với mọi } x \in M, \\
f'(y) &= g'(y, y, \ldots, y) & \text{với mọi } y \in N.
\end{aligned}
$$

Suy ra với mọi $x \in M$ ta có

$$
f'(f(x)) = g'(f(x), f(x), \ldots, f(x)) = g'(g(x, x, \ldots, x), \ldots, g(x, x, \ldots, x))
$$

và ánh xạ $(x_1, \ldots, x_{qr}) \mapsto g'(g(x_1, \ldots, x_q), \ldots, g(x_{q(r-1)+1}, \ldots, x_{qr}))$ của $M^{qr}$ vào $P$ là $qr$-tuyến tính.

#### Mệnh đề 15 {#alg-iv-s5-prop-15 .statement}

— Cho $M$ là một $A$-môđun tự do, $N$ là một $A$-môđun và $q$ là một số nguyên $\geqslant 0$. Ta giả sử rằng ánh xạ $y \mapsto q!y$ là một tự đẳng cấu của $N$. Cho $f \in \mathrm{Pol}^q(M, N)$, khi đó tồn tại một và chỉ một ánh xạ $q$-tuyến tính đối xứng $h$ của $M^q$ vào $M$ sao cho $f(x) = h(x, x, \ldots, x)$ với mọi $x \in M$. Với bất kỳ $x_1, \ldots, x_q \in M$ nào ta có

$$
h(x_1, x_2, \ldots, x_q) = \frac{(-1)^q}{q!} \sum_{H \subset \{1, 2, \ldots, q\}} (-1)^{\mathrm{Card}\ H} f\left( \sum_{i \in H} x_i \right).
$$

a) Tồn tại một ánh xạ $q$-tuyến tính $g$ của $M^q$ vào $N$ sao cho $f(x) = g(x, x, \ldots, x)$ với mọi $x \in M$. Ta định nghĩa một ánh xạ $q$-tuyến tính $h$ của $M$ vào $N$ bởi

$$
h(x_1, x_2, \ldots, x_q) = \frac{1}{q!} \sum_{\sigma \in S_q} g(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(q)}).
$$

Khi đó $h$ là đối xứng và $f(x) = h(x, x, \ldots, x)$ với mọi $x \in M$.

b) Cho $h$ là một ánh xạ $q$-tuyến tính đối xứng của $M^q$ vào $N$ sao cho f(x) = g(x, x, ..., x). Gọi l là ánh xạ tuyến tính của T^q(M) vào N sao cho h(x_1, ..., x_q) = l(x_1 \otimes ... \otimes x_q) với bất kỳ x_1, ..., x_q \in M. Ta có

$$
(-1)^q q! h(x_1, ..., x_q) = (-1)^q \sum_{\sigma \in S_q} h(x_{\sigma(1)}, ..., x_{\sigma(q)}) =
= (-1)^q l(s(x_1 \otimes ... \otimes x_q)) = \sum_{H \subset \{1, ..., q\}} (-1)^{\text{Card } H} l \left( \gamma_q \left( \sum_{i \in H} x_i \right) \right)
$$

theo Mệnh đề 3, (v) (IV, p. 45). Bây giờ

$$
l \left( \gamma_q \left( \sum_{i \in H} x_i \right) \right) = h \left( \sum_{i \in H} x_i, ..., \sum_{i \in H} x_i \right) = f \left( \sum_{i \in H} x_i \right)
$$

và điều này chứng minh công thức (16) và tính duy nhất của h.

#### Mệnh đề 16 {#alg-iv-s5-prop-16 .statement}

— *Cho M là một A-môđun tự do, N là một A-môđun, q là một số nguyên dương và u là đồng cấu chính tắc từ Hom ($\mathbf{TS}^q(M)$, N) vào $\mathbf{Pol}^Y(M, N)$.

(i) *Nếu A là một miền nguyên vô hạn và N không có xoắn, thì u là một đẳng cấu.*

(ii) *Nếu ánh xạ $y \mapsto q!y$ trong N là đơn ánh, thì u là một đẳng cấu.*

Trong hai trường hợp của mệnh đề này, ta phải chứng minh rằng u là đơn ánh, nghĩa là mọi ánh xạ tuyến tính f từ $\mathbf{TS}^q(M)$ vào N mà bằng không trên $\gamma_q(M)$ đều triệt tiêu.

Giả sử A là một miền nguyên vô hạn và N không có xoắn. Với mọi $z \in \mathbf{TS}^q(M)$ tồn tại $a \in A - \{0\}$ sao cho $az$ là một tổ hợp A-tuyến tính của các phần tử của y, (M) (*IV*, p. 47, Mệnh đề 5). Do đó $af(z) = f(az) = 0$, và vì thế $f(z) = 0$.

Tiếp theo giả sử ánh xạ $y \mapsto q!y$ trong N là đơn ánh; khi đó theo *IV*, p. 45, Mệnh đề 3, (v), f triệt tiêu trên s . T^q(M). Vậy nếu $z \in \mathbf{TS}^q(M)$, ta có $q!f(z) = f(sz) = 0$, và vì thế $f(z) = 0$.

#### Hệ quả {#alg-iv-s5-n9-cor-1 .statement}

— *Cho M là một A-môđun tự do, N là một A-môđun, q là một số nguyên dương, $h \in \mathbf{Pol}^q(M, N)$ và $(e_i)_i$, một cơ sở của M. Trong hai trường hợp của Mệnh đề 16, tồn tại một họ duy nhất $(u,$, $\mathbf{N}^{(1)}, |\cdot|$, , các phần tử của N sao cho $h \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{|\nu| = q} \lambda^\nu u_\nu$ với mọi $(\lambda_i) \in \mathbf{A}^{(1)}$*

### 10. Ánh xạ đa thức

#### Định nghĩa 4 {#alg-iv-s5-def-4 .statement}

— *Cho M và N là các A-môđun và giả sử rằng M là tự do. Ký hiệu Map(M, N) là A-môđun của mọi ánh xạ từ M vào N. Môđun con $\sum_{q > 0} \mathbf{Pol}_A^q(M, N)$ của Map(M, N) được ký hiệu là $\mathbf{Pol}_A(M, N)$ hoặc đơn giản là $\mathbf{Pol}(M, N)$; các phần tử của nó được gọi là các ánh xạ đa thức từ M vào N.*

Cho $(e_i)_{i \in I}$ là một cơ sở của M và giả sử rằng $l$ là hữu hạn; theo Mệnh đề 13 (IV, p. 54), một ánh xạ $f$ từ M vào N là đa thức khi và chỉ khi tồn tại một đa thức F theo các ẩn số $X_i$ với hệ số trong N sao cho

$$
f \left( \sum_{i \in I} x_i e_i \right) = F(x)
$$

với mọi họ $x = (x_i)_{i \in I}$ trong $A^{(I)}$. Tính chất này không phụ thuộc vào cơ sở được chọn của M và nó biện minh cho thuật ngữ « ánh xạ đa thức ».

#### Mệnh đề 17 {#alg-iv-s5-prop-17 .statement}

— *Cho M là một A-môđun tự do và B là một A-đại số kết hợp, giao hoán và có đơn vị. Khi đó $\mathrm{Pol}_A(M, B)$ là một đại số con trên B của đại số $\mathrm{Map}(M, B)$.

Điều này suy ra từ Định nghĩa 4 và Mệnh đề 13, (iv) (IV, p. 54).

#### Mệnh đề 18 {#alg-iv-s5-prop-18 .statement}

— *Cho M, N, P là các A-môđun, và giả sử rằng M và N là tự do. Nếu $f \in \mathrm{Pol}(M, N)$, $g \in \mathrm{Pol}(N, P)$, thì $g \circ f \in \mathrm{Pol}(M, P)$.

Ta có thể rút gọn ngay về trường hợp tồn tại một số nguyên q sao cho $g \in \mathrm{Pol}^q(N, P)$; khi đó tồn tại một ánh xạ q-tuyến tính $h$ từ $N^q$ vào P sao cho $g(y) = h(y, y, \ldots, y)$ với mọi $y \in N$. Viết $f$ thành một tổng các ánh xạ đa thức thuần nhất, như vậy ta được rút gọn về việc chứng minh rằng ánh xạ

$$
x \mapsto h(f_1(x), f_2(x), \ldots, f_q(x))
$$

từ M vào P, trong đó $f_i \in \mathrm{Pol}^{q_i}(M, N)$, là đa thức. Với $i = 1, \ldots, q$ tồn tại một ánh xạ $q_i$-tuyến tính $l_i$ từ $M^{q_i}$ vào N sao cho $f_i(x) = l_i(x, x, \ldots, x)$ với mọi $x \in M$. Do đó

$$
h(f_1(x), f_2(x), \ldots, f_q(x)) = h(l_1(x, \ldots, x), \ldots, l_q(x, \ldots, x)),
$$

từ đó mệnh đề của ta suy ra.

#### Bổ đề 2 {#alg-iv-s5-lem-2 .statement}

— *Cho N là một A-môđun, n là một số nguyên $\geq 0$ và*

$$
f = m_0 + m_1 X + \cdots + m_n X^n \in N[X].
$$

*Giả sử rằng tồn tại $\alpha_0, \alpha_1, \ldots, \alpha_r \in A$ sao cho $f(\alpha_0) = \cdots = f(\alpha_r) = 0$, và sao cho với $i \neq j$ phép vị tự có tỷ số $\alpha_i - \alpha_j$ trong N là đơn ánh, thì $f = 0$.*

(Bổ đề này tổng quát hóa Hệ quả ở IV, p. 16.)

Bổ đề rõ ràng đúng với $n = 0$; chúng ta sẽ chứng minh nó bằng quy nạp theo $n$. Ta có

$$
f(X) = f(X) - f(\alpha_0) = \sum_{i=1}^n m_i (X^i - \alpha_0^i) = (X - \alpha_0) g(X)
$$

trong đó g là một phần tử của N[X] có dạng $m_0' + m_1' X + \ldots + m_{n-1}' X^{n-1}$. Các giả thiết của bổ đề suy ra rằng $g(a,) = \cdots = g(a,) = 0$, do đó $g = 0$ theo giả thiết quy nạp, và vì thế $f = 0$.

#### Mệnh đề 19 {#alg-iv-s5-prop-19 .statement}

— *Cho M là một A-môđun tự do, N là một A-môđun, G là một nhóm con cộng tính vô hạn của A, và giả sử rằng các phép vị tự của N xác định bởi các phần tử khác không của G là đơn ánh. Khi đó Pol(M, N) là tổng trực tiếp của các Pol$^q$(M, N).*

Cho $f_0, f_1, \ldots, f_n$ sao cho $f_i \in \mathrm{Pol}^i(M, N)$ và giả sử ta có quan hệ $f_0 + \ldots + f_n = 0$. Lấy $x \in M$, khi đó với mọi $\lambda \in G$ ta có
$$
0 = \sum_{i=0}^n f_i(\lambda x) = \sum_{i=0}^n \lambda^i f_i(x).
$$
Theo Bổ đề 2, áp dụng cho đa thức $\sum_{i=0}^n f_i(x) X^i$ ta có
$$
f_0(x) = \cdots = f_n(x) = 0
$$

#### Hệ quả {#alg-iv-s5-n10-cor-1 .statement}

— *Giả sử rằng A là một miền nguyên vô hạn; cho M là một A-môđun tự do và N là một A-môđun không xoắn.*

(i) *Ta có $\mathrm{Pol}(M, N) = \bigoplus_{q \geq 0} \mathrm{Pol}^q(M, N)$ và mỗi $\mathrm{Pol}^q(M, N)$ có thể được đồng nhất một cách chính tắc với $\mathrm{Hom}(\mathbf{T S}^q(M), N)$.*

(ii) *Cho $f \in \mathrm{Pol}(M, N)$ và $(e_i)_i$, một cơ sở của M. Tồn tại một và chỉ một họ $(u_v)_{v \in N^{(1)}}$ các phần tử của N sao cho $f \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{v \in N^{(1)}} \lambda^v u_v$ với mọi $(\lambda_i) \in A^{(1)}$.*

Mệnh đề (i) suy ra từ Mệnh đề 16 và 19, còn (ii) suy ra từ (i) và Hệ quả của Mệnh đề 16.

### 11. Các quan hệ giữa $\mathbf{S}(M^*)$, TS(M)*gr và Pol(M, A)

Cho M là một A-môđun tự do, ta sẽ trang bị cho đối ngẫu phân bậc TS(M)*gr cấu trúc đại số phân bậc giao hoán, kết hợp và có đơn vị $^1$, dẫn xuất từ cấu trúc đối đại số phân bậc của TS(M) (III, p. 580). Theo III, p. 497 tồn tại một đồng cấu duy nhất của các A-đại số phân bậc
$$
\theta : \mathbf{S}(M^*) \to \mathbf{TS}(M)^{*gr}
$$
cảm sinh trong bậc 1 ánh xạ đồng nhất của M*.

$^1$ Ở đây một đồng cấu phân bậc bậc – k từ TS(M) vào A được xem như một phần tử bậc k của TS(M)*gr (II, p. 377).

#### Mệnh đề 20 {#alg-iv-s5-prop-20 .statement}

— *Nếu A-môđun M là tự do và sinh hữu hạn, thì $0$ là một đẳng cấu của các đại số phân bậc.*

Cho $(e_i)_{i \in I}$ là một cơ sở của $M$ và $(e_i^*)_{i \in I}$ là cơ sở đối ngẫu của $M^*$. Với $v \in \mathbf{N}^I$ đặt

$$
e_v = \prod_{i \in I} \gamma_{v_i}(e_i) \in \mathbf{TS}(M)
$$

Theo Mệnh đề 4 (*IV*, p. 47), họ $(e_v)_v,_{\mathbf{N}^I}$ là một cơ sở của $TS(M)$; gọi $(e_v^*)$ là cơ sở của $\mathbf{TS}(M)^{*gr}$ đối ngẫu với $(e_v)$. Theo III, p. 505, Định lý 1, chỉ cần chứng tỏ rằng với mọi $v \in \mathbf{N}^I$ ta có

$$
e_v^* = \prod_{i \in I} (e_i^*)^{v_i},
$$

hay cũng có nghĩa là với $\rho, \sigma \in \mathbf{N}^I$ ta có $e_\rho^* \cdot e_\sigma^* = e_{\rho + \sigma}^*$; nhưng mệnh đề cuối cùng này suy ra từ *IV*, p. 50, Công thức (12).

#### Nhận xét 1 {#alg-iv-s5-n11-rem-1 .statement}

— Theo cùng một cách, ta thấy rằng nếu $M$ là một $A$-môđun tự do sinh hữu hạn, thì đại số phân bậc $S(M)^{*gr}$ được định nghĩa trong III, p. 593 có thể được đồng nhất với $TS(M^*)$.

#### Mệnh đề 21 {#alg-iv-s5-prop-21 .statement}

— *Đồng cấu chính tắc của các A-môđun* (*IV*, p. 55)

$$
u : \mathbf{TS}(M)^{*gr} \to \mathrm{Pol}_A(M, A)
$$

*là một đồng cấu đại số.*

Cho $a \in \mathbf{TS}^q(M)^*, b \in TS^r(M)^*, x \in M$; ta có

$$
u(ab)(x) = \langle ab, \gamma_{q+r}(x) \rangle = \langle a \otimes b, c(\gamma_{q+r}(x)) \rangle =
= \langle a \otimes b, \gamma_q(x) \otimes \gamma_r(x) \rangle = \langle a, \gamma_q(x) \rangle \langle b, \gamma_r(x) \rangle = u(a)(x) \cdot u(b)(x),
$$

do đó có kết quả.

#### Nhận xét {#alg-iv-s5-n11-rem-2 .statement}

— 2) Đồng cấu hợp thành $A, = u \circ 0 : S(M^*) \to \mathrm{Pol}_A(M, A)$ là đồng cấu có đơn vị duy nhất của các đại số cảm sinh phép nhúng của

$$
M^* = \mathrm{Pol}^1(M, A)
$$

trong $\mathrm{Pol}(M, A)$. Nếu $M$ là tự do sinh hữu hạn và $A$ là một miền nguyên vô hạn, thì $\lambda_M$ là song ánh (Mệnh đề 20 và Hệ quả của Mệnh đề 19). Đặc biệt, nếu $A$ là một miền nguyên vô hạn, thì đồng cấu chính tắc $f \mapsto \tilde{f}$ từ $A[X_1, \ldots, X_n]$ vào $\mathrm{Pol}(A^n, A)$ (*IV*, p. 4) là một đẳng cấu.

3) Xét đồng tích $c_S : S(M^*) \to S(M^* \times M^*)$ (III, p. 575, Ví dụ 6). Với mọi $v \in S(M^*)$, $x, y \in M$, ánh xạ đa thức $\lambda_{M \times M}(c_S(v)) : M \times M \to A$ ánh xạ $(x, y)$ thành $A, (v)(x + y)$. Vì hai đồng cấu đại số của $S(M^*)$ vào $\mathrm{Map}(M \times M, A)$ được xác định theo cách này trùng nhau trên $M^*$, theo quan hệ

$$
(v \otimes 1 + 1 \otimes v)(x, y) = v(x + y) \quad (v \in M^*)
$$

### Bài tập {#alg-iv-s5-exercises}

Xem [bài tập của § 5](exercises/s5/).
