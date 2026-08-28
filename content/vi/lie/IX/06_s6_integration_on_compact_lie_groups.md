---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 6
section_title: Integration on compact Lie groups
lang: vi
source: lie-vii-ix
book_pages: 333-346, 409-414
pdf_pages: 0340-0353, 0416-0421
extraction: native
subsections:
    - "no": 1
      title: PRODUCT OF ALTERNATING MULTILINEAR FORMS
      page: 333
      pdf_page: 340
    - "no": 2
      title: INTEGRATION FORMULA OF H. WEYL
      page: 334
      pdf_page: 341
    - "no": 3
      title: INTEGRATION ON LIE ALGEBRAS
      page: 339
      pdf_page: 346
    - "no": 4
      title: INTEGRATION OF SECTIONS OF A VECTOR BUNDLE
      page: 341
      pdf_page: 348
    - "no": 5
      title: INVARIANT DIFFERENTIAL FORMS
      page: 344
      pdf_page: 351
statements: 25
exercises: 13
content_sha256: 185874cefc5ee2b589419ee7445951bb5d29059f2237e9b5484b5208867e328a
translated_from: content/en/lie/IX/06_s6_integration_on_compact_lie_groups.md
source_content_sha256: 746c6186434593ae87ea52347a193f0e294cca0a933dcfbfbd4549276c4b772c
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5.4-mini
translation_run: translate-vi-fbf2713e
glossary_version: 34
glossary_terms_sha256: f58490ec4e4518adbcb69ff1f08702f419fa55de0298af8ab9f9cb09cc0a734e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. TÍCH PHÂN TRÊN CÁC NHÓM LIE COMPACT

Ta giữ lại các ký hiệu của §4; đặt $w(G) =$ Card(W$_G(T)$). Ký hiệu $dg$ (tương ứng $dt$) là độ đo Haar trên G (tương ứng T) có khối lượng toàn phần bằng 1, và $n$ (tương ứng $r$) là chiều của G (tương ứng T).

### 1. TÍCH CỦA CÁC DẠNG ĐA TUYẾN TÍNH THAY PHIÊN

Cho A là một vành giao hoán và M là một A-môđun. Với mỗi số nguyên $r\geq 0$, ký hiệu Alt$^r(M)$ là A-môđun của các dạng $r$-tuyến tính thay phiên trên M; nó có thể được đồng nhất với đối ngẫu của A-môđun $\wedge \wedge^r(M) ($Algebra, Chap. III, §7, no. 4, Prop. 7). Cho $u\in$ Alt$^s(M)$ và $v\in$ Alt$^r(M)$; nhắc lại (Algebra, Chap. III, §11, no. 2, Ví dụ 3) rằng tích thay phiên của $u$ và $v$ là phần tử $u\wedge v\in$ Alt$^{s+r}(M)$ được xác định bởi

$$
(u\wedge v)(x_1, . . . , x_{s+r}) =\sum_{\sigma\in\mathfrak{S}_{s,r}}\varepsilon_{\sigma}u(x_{\sigma(1)}, . . . , x_{\sigma(s)})v(x_{\sigma(s+1)}, . . . , x_{\sigma(s+r)})
$$

trong đó $\mathfrak{S}_{s,r}$ là tập con của nhóm đối xứng $\mathfrak{S}_{s+r}$ gồm các phép thế mà các hạn chế của chúng lên $1, s$ và $s+ 1, s+r$ là tăng.

Bây giờ cho

0 $\longrightarrow M'\longrightarrow^i$ M $\longrightarrow^pM''\longrightarrow$ 0

là một dãy khớp các A-môđun tự do, có các hạng lần lượt là $r, r+s$ và $s$.

#### Bổ đề 1 {#lie-ix-s6-lem-1 .statement tag=01EX}

Tồn tại một ánh xạ A-song tuyến tính từ Alt$^s(M'')\times$ Alt$^r(M')$ vào Alt$^{s+r}(M)$, được ký hiệu bởi $(u, v) \rightarrow u\cap v$, và được đặc trưng bởi một trong hai tính chất sau:

a) Ký hiệu $u_1\in$ Alt$^s(M)$ là dạng $(x_1, . . . , x_s) \rightarrow u(p(x_1), . . . , p(x_s))$, và cho $v_1\in$ Alt$^r(M)$ là một dạng sao cho $v_1(i(x'_1), . . . , i(x'_r)) =v(x'_1, . . . , x'_r)$ với $x'_1, . . . , x'_r$ trong $M'$; khi đó $u\cap v=u_1\wedge v_1$.

b) Với mọi $x_1, . . . , x_s$ trong M và $x'_1, . . . , x'_r$ trong $M'$,

$$
(u\cap v)(x_1, . . . , x_s, i(x'_1), . . . , i(x'_r)) =u(p(x_1), . . . , p(x_s))v(x'_1, . . . , x'_r) \tag{1}
$$

Ánh xạ $\varphi :$ Alt$^s(M'')\otimes_A$Alt$^r(M')\rightarrow$ Alt$^{s+r}(M)$ sao cho $\varphi (u\otimes v) =u\cap v$ là một đẳng cấu của các A-môđun tự do hạng một.

Sự tồn tại của một dạng $v_1$ thỏa mãn điều kiện a) suy ra từ sự kiện rằng $\wedge \wedge^r(i)$ cảm sinh một đẳng cấu từ $\wedge \wedge^r(M')$ lên một môđun con hạng tử trực tiếp của $\wedge \wedge^r(M) ($Algebra, Chap. III, §7, no. 2). Cho $v_1$ là một dạng như vậy; đặt $u\cap v=u_1\wedge v_1$. Công thức (1) khi đó được thỏa mãn, vì nếu đặt $i(x'_k) =x_{s+k}$ với $1\leq k\leq r$, thì phần tử duy nhất $\sigma$ của $\mathfrak{S}_{s,r}$ sao cho $p(x_{\sigma(i)})\not= 0$ với $1\leq i\leq s$ là phép hoán vị đơn vị. Mặt khác, công thức (1) xác định $u\cap v$ một cách duy nhất: thật vậy, gọi $(e'_1, . . . , e'_r)$ là một cơ sở của $M', (f''_1, . . . , f''_s)$ là một cơ sở của $M''$, và $f_1, . . . , f_s$ là các phần tử của M sao cho $p(f_i) =f''_i$ với $1\leq i\leq s$. Khi đó $(f_1, . . . , f_s, i(e'_1), . . . , i(e'_r))$ là một cơ sở của M (Algebra, Chap. II, §1, no. 11, Prop. 21), và công thức (1) có thể được viết

$$
(u\cap v)(f_1, . . . , f_s, i(e'_1), . . . , i(e'_r)) =u(f''_1, . . . , f''_s)v(e'_1, . . . , e'_r) \tag{2}
$$

nhưng một phần tử của Alt$^{s+r}(M)$ được xác định bởi giá trị của nó trên một cơ sở.

Từ điều đã nêu trước đó suy ra rằng mỗi điều kiện a) và b) xác định tích $u\cap v$ một cách duy nhất; rõ ràng tích này là song tuyến tính. Cuối cùng, khẳng định cuối cùng của bổ đề suy ra từ công thức (2).

### 2. CÔNG THỨC TÍCH PHÂN CỦA H. WEYL

Cho $e$ là phần tử đơn vị của G và $\overline{e}$ là lớp của nó trong $G/T$. Đồng nhất không gian tiếp xúc của G tại $e$ với $\mathfrak{g}$, không gian tiếp xúc của T tại $e$ với $\mathfrak{t}$ và không gian tiếp xúc của $G/T$ tại $\overline{e}$ với $\mathfrak{g}/\mathfrak{t}$. Ký hiệu bằng $(u, v) \rightarrow u\cap v$ ánh xạ song tuyến tính trên $\mathbf{R}$

Alt$^{n-r}(\mathfrak{g}/\mathfrak{t})\times$ Alt$^r(\mathfrak{t})\rightarrow$ Alt$^n(\mathfrak{g})$

được định nghĩa trong số 1.

Nhắc lại (Chap. III, §3, no. 13, Prop. 50) rằng ánh xạ $\omega  \rightarrow \omega (e)$ là một đẳng cấu từ không gian các dạng vi phân bất biến trái bậc $n$ (tương ứng $r$) trên G (tương ứng T) lên không gian Alt$^n(\mathfrak{g})$ (tương ứng Alt$^r(\mathfrak{t})$). Hơn nữa, nhận xét rằng, vì mọi nhóm con compact liên thông của $\mathbf{R}^*$ đều thu gọn về phần tử đơn vị, det Ad $g= 1$ với mọi $g\in G$, nên các dạng vi phân bất biến trái bậc $n$ trên G cũng bất biến phải và bất biến dưới các tự đẳng cấu nội (Chap. III, §3, no. 16, Cor. of Prop. 54): từ nay ta sẽ chỉ đơn giản nói đến các dạng vi phân bất biến G.

Tương tự, từ Chap. III, §3, no. 16, Prop. 56 và điều đã nêu trước đó suy ra rằng ánh xạ $\omega  \rightarrow \omega (\overline{e})$ là một đẳng cấu từ không gian các dạng vi phân bất biến G bậc $n-r$ trên $G/T$ lên không gian Alt$^{n-r}(\mathfrak{g}/\mathfrak{t})$.

Nếu $\omega_{G/T}$ là một dạng vi phân bất biến bởi G có bậc $n-r$ trên $G/T$, và $\omega_T$ là một dạng vi phân bất biến có bậc $r$ trên T, ký hiệu $\omega_{G/T}\cap \omega_T$ là dạng vi phân bất biến duy nhất có bậc $n$ trên G sao cho

$$
(\omega_{G/T}\cap \omega_T)(e) =\omega_{G/T}(\overline{e})\cap \omega_T(e)
$$

Cuối cùng, nhắc lại rằng $f: (G/T)\times T\rightarrow G$ ký hiệu cấu xạ giữa các đa tạp cảm sinh bởi ánh xạ $(g, t) \rightarrow gtg^{-1}$ từ $G\times T$ vào G bằng cách chuyển qua thương (§5, no. 4). Nếu $\alpha$ và $\beta$ lần lượt là các dạng vi phân trên $G/T$ và T, ký hiệu đơn giản $\alpha \wedge \beta$ là dạng pr$^*_1\alpha \wedge$ pr$^*_2\beta$ trên $(G/T)\times T$.

Với $t\in T$, ký hiệu Ad$_{\mathfrak{g}/\mathfrak{t}}(t)$ là tự đồng cấu của $\mathfrak{g}/\mathfrak{t}$ cảm sinh bởi Ad $t$ bằng cách chuyển qua thương. Đặt

$\delta_G(t) =$ det(Ad$_{\mathfrak{g}/\mathfrak{t}}(t)-1$) $=\prod_{\alpha\in R(G,T)}(t^{\alpha}-1)$. (3)

Cho $x\in \mathfrak{t}$ và $\alpha \in R(G,T)$; ký hiệu $\widehat{\alpha}$ là phần tử $(2\pi i)^{-1}\delta (\alpha )$ của $\mathfrak{t}^*$, sao cho

((exp $x$)$^{\alpha}-$ 1)((exp $x$)$^{-\alpha}-1$) $= (e^{2\pi i\widehat{\alpha}(x)}-1)(e^{-2\pi i\widehat{\alpha}(x)}-1) = 4$ sin$^2\pi \widehat{\alpha}(x)$.

Nếu $R_+(G,T)$ ký hiệu tập hợp các nghiệm dương của $R(G,T)$ tương ứng với một cơ sở B, ta có

$\delta_G$(exp $x$) $=\prod_{\alpha\in R_+(G,T)}4$ sin$^2\pi \widehat{\alpha}(x)$,

do đó, đặc biệt, $\delta_G(t)>0$ với mọi $t\in T_r$. Ta cũng nhận xét rằng $\delta_G(t) =\delta_G(t^{-1})$ với $t\in T$.

#### Mệnh đề 1 {#lie-ix-s6-prop-1 .statement tag=01EY}

Cho $\omega_G, \omega_{G/T}$ và $\omega_T$ là các dạng vi phân bất biến trên $G,G/T$ và T, tương ứng, có các bậc tương ứng $n, n-r$ và $r$. Nếu $\omega_G=$ $\omega_{G/T}\cap \omega_T$, thì

$$
f^*(\omega_G) =\omega_{G/T}\wedge \delta_G\omega_T
$$

Rõ ràng ta có thể giả sử rằng $\omega_{G/T}$ và $\omega_T$ là khác không; khi đó dạng vi phân $(u, t) \rightarrow \omega_{G/T}(u)\wedge \omega_T(t)$ trên $(G/T)\times T$ có bậc $n$ và khác không tại mọi nơi; do đó tồn tại một hàm số $\delta$ trên $(G/T)\times T$ sao cho

$$
f^*(\omega_G)(u, t) =\delta (u, t)\omega_{G/T}(u)\wedge \omega_T(t)
$$

Bây giờ nhận xét rằng, với $h\in G,u\in G/T,t\in$ T, ta có $f(h.u, t) =$ (Int $h$)$f(u, t)$; vì $\omega_G$ bất biến dưới các tự đẳng cấu nội, suy ra ngay lập tức rằng $\delta (h.u, t) =\delta (u, t)$, do đó $\delta (u, t) =\delta (\overline{e}, t)$.

Ký hiệu $p:\mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{t}$ là ánh xạ thương và $\varphi :\mathfrak{g}/\mathfrak{t}\rightarrow \mathfrak{g}$ là ánh xạ được định nghĩa bởi

$\varphi (p(X)) =$ (Ad $t^{-1}$)$X-X$ với $X\in \mathfrak{g}$; hãy nhớ (§5, no. 4, Bổ đề 4) rằng ánh xạ tiếp xúc

$$
T_{(e,t)}(f) : T_e(G/T)\times T_t(T)\rightarrow T_t(G)
$$

biến $(z, tH)$ thành $t(\varphi (z) +H)$ với $z\in \mathfrak{g}/\mathfrak{t}, H\in \mathfrak{t}$.

Cho $z_1, . . . , z_{n-r}$ là các phần tử của $\mathfrak{g}/\mathfrak{t},H_1, . . . , H_r$ là các phần tử của $\mathfrak{t}$. Khi đó

$$
f^*\omega_G(\overline{e}, t)(z_1, . . . , z_{n-r}, tH_1, . . . , tH_r)
$$

$=\omega_G(t)(t\varphi (z_1), . . . , t\varphi (z_{n-r}), tH_1, . . . , tH_r)$ theo phép tính của $T_{(\overline{e},t)}(f)$

$=\omega_G(e)(\varphi (z_1), . . . , \varphi (z_{n-r}), H_1, . . . , H_r)$ vì $\omega_G$ là bất biến

$=\omega_{G/T}(\overline{e})(p\varphi (z_1), . . . , p\varphi (z_{n-r})).\omega_T(e)(H_1, . . . , H_r)$ (no$.1$, Bổ đề 1)

= det($p\varphi$ )$\omega_{G/T}(\overline{e})(z_1, . . . , z_{n-r}).\omega_T(e)(H_1, . . . , H_r)$

$$
=\delta_G(t)\omega_{G/T}(\overline{e})(z_1, . . . , z_{n-r}).\omega_T(t)(tH_1, . . . , tH_r)
$$

vì $\omega_T$ là bất biến

$$
=\delta_G(t)(\omega_{G/T}\wedge \omega_T)(\overline{e}, t)(z_1, . . . , z_{n-r}, tH_1, . . . , tH_r)
$$

do đó $f^*\omega_G(\overline{e}, t) =\delta_G(t)(\omega_{G/T}\wedge \omega_T)(\overline{e}, t)$; vậy $\delta (\overline{e}, t) =\delta_G(t)$, suy ra mệnh đề.

Gán cho các đa tạp $G,T$ và $G/T$ các định hướng được xác định lần lượt bởi các dạng $\omega_G, \omega_T$ và $\omega_{G/T}$. Các dạng này định nghĩa các độ đo bất biến trên $G,T$ và $G/T$ (Chap. III, §3, no. 16, Props. 55 and 56), cũng được ký hiệu bởi $\omega_G, \omega_T$ và $\omega_{G/T}$.

#### Bổ đề 2 {#lie-ix-s6-lem-2 .statement tag=01EZ}

Nếu $\omega_G=\omega_{G/T}\cap \omega_T$, thì

$$
\int_G\omega_G=\int_{G/T}\omega_{G/T}.\int_T\omega_T
$$

Ký hiệu $\pi$ là cấu xạ chính tắc từ G đến $G/T$. Cho $g\in G$, và cho $t_1, . . . , t_{n-r}$ là các phần tử của $T_{\pi(g)}(G/T)$. Đồng nhất thớ $\pi^{-1}(\pi (g)) =gT$ với T bằng phép tịnh tiến $\gamma (g)$. Quan hệ $\omega_G=\omega_{G/T}\cap \omega_T$ bây giờ suy ra đẳng thức (Differentiable and Analytic Manifolds, Results, 11.4.5):

$$
\omega_G\llcorner (t_1, . . . , t_{n-r}) = (\omega_{G/T}(t_1, . . . , t_{n-r}))\omega_T
$$

Do đó $\int_{\pi}\omega_G=(\int_T\omega_T)\omega_{G/T}($Đa tạp khả vi và giải tích, Kết quả, 11.4.6), và

$$
\int_G\omega_G=\int_{G/}\int_{T\pi}\omega_G=\int_T\omega_T.\int_{G/T}\omega_{G/T}
$$

(Đa tạp khả vi và giải tích, Kết quả, 11.4.8).

#### Bổ đề 3 {#lie-ix-s6-lem-3 .statement tag=01F0}

Ảnh ngược trên $(G/T)\times T_r$ của độ đo $dg$ trên $G_r$ qua phép đồng phôi cục bộ $f_r($Tích phân, Chương V, §6, no. 6) là độ đo $\mu\otimes \delta_Gdt$, trong đó $\mu$ là độ đo G-bất biến duy nhất trên $G/T$ có tổng khối lượng 1.

Chọn một dạng vi phân bất biến $\omega_T$ (resp. $\omega_{G/T}$) trên T (resp. $G/T$) có bậc tối đa, sao cho độ đo do $\omega_T$ (resp. $\omega_{G/T}$) xác định bằng $dt$ (resp. $\mu$). Đặt $\omega_G=\omega_{G/T}\cap \omega_T$. Bổ đề 2 suy ra rằng độ đo do $\omega_G$ xác định bằng $dg$. Cho U là một tập con mở của $(G/T)\times T_r$ sao cho $f_r$ xác định một đẳng cấu từ U lên một tập con mở V của $G_r$. Cho $\varphi$ là một hàm liên tục có giá compact trong V; cũng ký hiệu bằng $\varphi$ phần mở rộng của $\varphi$ đến $G_r$ bằng 0 ngoài V. Ta có

$$
\int_V\varphi  dg=\int_V\varphi  \omega_G=\int_U(\varphi \circ f_r)f_r^*(\omega_G)
$$

$=\int_U(\varphi \circ f_r)\omega_{G/T}\wedge \delta_G\omega_T$ (Mệnh đề$.1$)

$$
=\int_U(\varphi \circ f_r)d\mu.\delta_Gdt
$$

suy ra bổ đề.

#### Định lý 1 (H. Weyl) {#lie-ix-s6-thm-1 .statement tag=01F1}

Độ đo $dg$ trên G là ảnh qua ánh xạ $(g, t) \rightarrow gtg^{-1}$ từ $G\times T$ vào G của độ đo $dg\otimes \frac{1}{w(G)}\delta_Gdt$, trong đó

$\delta_G(t) =$ det(Ad$_{\mathfrak{g}/\mathfrak{t}}(t)-1$) $=\prod_{\alpha\in R(G,T)}(t^{\alpha}-1)$.

Tương đương (Tích phân, Chương V, §6, no. 3, Mệnh đề $4$)$,dg$ là ảnh qua ánh xạ $f: (G/T)\times T\rightarrow G$ của độ đo $\mu\otimes \frac{1}{w(G)}\delta_Gdt$.

Ta chứng minh khẳng định cuối cùng. Từ §5, no. 1 và Đa tạp khả vi và giải tích, Kết quả$, 10.1.3c)$ suy ra rằng G**--** $G_r$ là tập không đáng kể trong G và T **--** $T_r$ là tập không đáng kể trong T. Hơn nữa, ánh xạ $f_r$ làm cho $(G/T)\times T_r$ thành một phủ chính của $G_r$, với nhóm W (§5, no. 4, Mệnh đề $4b$)$)$. Định lý bây giờ suy ra từ Bổ đề 3 và Tích phân, Chương V, §6, no. 6, Mệnh đề 11.

#### Hệ quả 1 {#lie-ix-s6-thm-1-cor-1 .statement tag=01F2}

(i) Cho $\varphi$ là một hàm khả tích trên G với giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$. Với hầu hết $t\in T$, hàm $g \rightarrow \varphi (gtg^{-1})$ trên G là khả tích đối với $dg$. Hàm $t \rightarrow \delta_G(t)\int_G\varphi (gtg^{-1})dg$ là khả tích trên T, và ta có

$$
\int_G\varphi (g)dg=\frac{1}{w(G)}\int_T(\int_G\varphi (gtg^{-1})dg)\delta_G(t)dt \tag{4}
$$

(“công thức tích phân của Hermann Weyl”).

(ii) Cho $\varphi$ là một hàm đo được dương trên G. Với hầu hết mọi $t\in T$, hàm $g \rightarrow \varphi (gtg^{-1})$ trên G là đo được. Hàm $t \rightarrow \int_G^*\varphi (gtg^{-1})dg$ trên T là đo được, và ta có

$$
\int_G^*\varphi (g)dg=\frac{1}{w(G)}\int_T^*(\int_G^*\varphi (gtg^{-1})dg)\delta_G(t)dt \tag{5}
$$

Vì ánh xạ $f$ cảm sinh bởi phép chuyển qua thương từ ánh xạ $(g, t) \rightarrow gtg^{-1}$ từ $G\times T\rightarrow G$, nên chỉ cần áp dụng Integration, Chap. V, §5, 6, 8 và Integration, Chap. VII, §2.

#### Hệ quả 2 {#lie-ix-s6-thm-1-cor-2 .statement tag=01F3}

Cho $\varphi$ là một hàm trung tâm trên G (nghĩa là, sao cho $\varphi (gh) =$ $\varphi (hg)$ với mọi $g$ và $h$ trong G) với các giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$.

a$)\varphi$ đo được khi và chỉ khi hạn chế của nó lên T là đo được.

b$)\varphi$ khả tích khi và chỉ khi hàm $(\varphi |T)\delta_G$ khả tích trên T, và trong trường hợp đó ta có

$$
\int_G\varphi (g)dg=\frac{1}{w(G)}\int_T\varphi (t)\delta_G(t)dt \tag{6}
$$

Ký hiệu $p: G/T\times T\rightarrow T$ là phép chiếu thứ hai. Ta có $\varphi \circ f$ = $(\varphi |T)\circ p$; hơn nữa, ảnh dưới $p$ của độ đo $\mu\otimes \frac{1}{w(G)}\delta_Gdt$ là $\frac{1}{w(G)}\delta_Gdt$. Hệ quả bây giờ suy ra từ Định lý 1 ở trên và Định lý 1 của Integration, Chap. V, §6, no. 2, áp dụng cho hai ánh xạ thực sự $f$ và $p$.

#### Hệ quả 3 {#lie-ix-s6-thm-1-cor-3 .statement tag=01F4}

Cho H là một nhóm con đóng liên thông của G chứa T, $\mathfrak{h}$ là đại số Lie của nó, và $dh$ là độ đo Haar trên H có khối lượng toàn phần bằng 1. Cho $\varphi$ là một hàm trung tâm khả tích trên G, với các giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$. Khi đó hàm $h \rightarrow \varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1$) là khả tích và trung tâm trên H và ta có

$\int_G\varphi (g)dg=\frac{w(H)}{w(G)}\int_H\varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1$)$dh$. (7)

Thật vậy, hàm $h \rightarrow \varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1$) là một hàm trung tâm trên H mà hạn chế của nó lên T là hàm $t \rightarrow \varphi (t)\delta_G(t)\delta_H(t)^{-1}$. Do đó, hệ quả suy ra từ Hệ quả 2 áp dụng cho G và H.

#### Nhận xét 1 {#lie-ix-s6-n2-rem-1 .statement tag=01F5}

Nếu ta lấy $\varphi = 1$ trong Hệ quả 3, ta thu được

$\int_H$ det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1$)$dh=w(G)/w(H)$ (8)

và đặc biệt

$$
\int_T\delta_G(t)dt=w(G) \tag{9}
$$

#### Nhận xét 2 {#lie-ix-s6-n2-rem-2 .statement tag=01F6}

Cho $\nu$ là độ đo trên thương $T/W$ được xác định bởi

$$
\int_{T/W}\psi (\tau )d\nu (\tau ) =\frac{1}{w(G)}\int_T\psi (\pi (t))\delta_G(t)dt
$$

trong đó $\pi$ biểu thị phép chiếu chính tắc của T lên $T/W$. Hệ quả 2 có nghĩa là phép đồng phôi $T/W\rightarrow G/$Int(G) (§2, no. 5, Hệ quả 1 của Mệnh đề 5) chuyển độ đo $\nu$ thành ảnh của độ đo $dg$ dưới phép chiếu chính tắc $G\rightarrow G/$Int(G).

#### Nhận xét 3 {#lie-ix-s6-n2-rem-3 .statement tag=01F7}

Giả sử rằng G liên thông đơn. Cho A là một alcôv của $\mathfrak{t}$, và $dx$ là độ đo Haar trên $\mathfrak{t}$ sao cho $\int_Adx= 1$. Khi đó độ đo $\nu$ cũng có thể thu được bằng cách chuyển độ đo $\frac{1}{w(G)}\prod_{\alpha\in R_+(G,T)}4$ sin$^2\pi \widehat{\alpha}(x)dx$ trên $\overline{A}$ bởi

phép đồng phôi $\overline{A}\rightarrow T/W ($§5, no. 2, Hệ quả 1 của Mệnh đề 2).

#### Ví dụ {#lie-ix-s6-n2-exa-1 .statement tag=01F8}

Cho G là nhóm $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ và T là nhóm con của các ma trận đường chéo (§3, no. 6); đồng nhất $\mathfrak{t}$ với $\mathbf{R}$ bằng lựa chọn cơ sở $\{iH\}$ của $\mathfrak{t}($loc. cit.). Đặt $A = 0, \pi$; đó là một alcove của $\mathfrak{t}$. Khoảng $A = 0, \pi$ có thể được đồng nhất với không gian các lớp liên hợp của G, phần tử $\theta$ của

$(e^{i\theta}$ 0 $)$

$\overline{A}$ tương ứng với lớp liên hợp của $-_{i\theta}$ . Cho $d\theta$ là độ đo Lebesgue

0 $e$

trên $0, \pi$; suy ra từ điều trên rằng ảnh trên $\overline{A}$ của độ đo Haar trên G là độ đo $\frac{2}{\pi}$ sin$^2\theta  d\theta$.

### 3. TÍCH PHÂN TRÊN ĐẠI SỐ LIE

#### Mệnh đề 2 {#lie-ix-s6-prop-2 .statement tag=01F9}

Cho H là một nhóm Lie (thực) có chiều $m,\mathfrak{h}$ là đại số Lie của nó. Cho $\omega_H$ là một dạng vi phân bất biến phải bậc $m$ trên H, và cho $\omega_{\mathfrak{h}}$ là dạng vi phân bất biến theo phép tịnh tiến trên $\mathfrak{h}$, bậc $m$, trùng với $\omega_H(e)$ tại gốc. Ta có

(exp$_H$)$^*\omega_H=\lambda_{\mathfrak{h}}\omega_{\mathfrak{h}}$ (10)

trong đó $\lambda_{\mathfrak{h}}$ là hàm bất biến theo Ad(H) trên $\mathfrak{h}$ sao cho

$\lambda_{\mathfrak{h}}(x) =$ det $\sum(p+$ 1)!1 (ad $x$)$^p$ với $x\in \mathfrak{h}$.

$p\geq 0$

Cho $x, x_1, . . . , x_m$ là các phần tử của $\mathfrak{h}$. Ta có

(exp$^*\omega_H$)$_x(x_1, . . . , x_m) = (\omega_H$(exp $x$))$(T_x$(exp)($x_1$)$, . . . ,T_x$(exp)($x_m$)). Ký hiệu $\varpi (x) :\mathfrak{h}\rightarrow \mathfrak{h}$ là vi phân phải của ánh xạ mũ tại $x$ (Chap. III, §3, no. 17, Def. 8); theo định nghĩa,

$T_x$(exp)($y$).(exp $x$)$^{-1}=\varpi (x).y$ với mọi $y\in \mathfrak{h}$.

Vì dạng $\omega_H$ bất biến phải, ta thu được

$(\omega_H$(exp $x$))$(T_x$(exp)($x_1$)$, . . . ,T_x$(exp)($x_m$))

$=\omega_H(e)(\varpi (x).x_1, . . . , \varpi (x).x_m) =$ (det $\varpi (x)$)$\omega_{\mathfrak{h}}(x_1, . . . , x_m)$;

do đó, exp$^*\omega_H=\lambda_{\mathfrak{h}}\omega_{\mathfrak{h}}$, với $\lambda_{\mathfrak{h}}(x) =$ det $\varpi (x) =$ det$\frac{exp ad x-1}{ad x}$ (Chương III, §6, no. 4, Mệnh đề 12).

Cho $h\in H$; vì Ad $h$ là một tự đẳng cấu của $\mathfrak{h}$, ta có

ad ((Ad $h$)$(x)$) $=$ Ad $h\circ$ Ad$x\circ$ (Ad $h$)$^{-1}$,

nên $\lambda_{\mathfrak{h}}$((Ad $h$)$(x)$) $=\lambda_{\mathfrak{h}}(x)$. Do đó, hàm $\lambda_{\mathfrak{h}}$ là bất biến dưới Ad(H); điều này hoàn tất chứng minh của mệnh đề.

#### Nhận xét {#lie-ix-s6-n3-rem-1 .statement tag=01FA}

Xét hàm $\lambda_{\mathfrak{g}}$ liên kết với một nhóm Lie compact G; xét theo §2, no. 1, Định lý 1, để tính $\lambda_{\mathfrak{g}}$ chỉ cần biết các giá trị của nó trên $\mathfrak{t}$. Nhưng, với $x\in \mathfrak{t}$, tự đồng cấu ad $x$ của $\mathfrak{g}$ là nửa đơn, và có các trị riêng 0 (với bội số $r$) và, với mọi $\alpha \in R(G,T),\delta (\alpha )(x)$ (với bội no. 1). Suy ra ngay lập tức rằng

$$
\lambda_{\mathfrak{g}}(x) =\prod\frac{e^{\delta(\alpha)(x)} - 1}{\delta(\alpha)(x)}=\frac{\delta_{\mathfrak{g}}(x)}{\pi_{\mathfrak{g}}(x)} \tag{11}
$$

$\alpha \in R(G,T)$

với $\delta_{\mathfrak{g}}(x) =\delta_G$(exp $x$) và $\pi_{\mathfrak{g}}(x) =\prod_{\alpha\in R(G,T)}\delta (\alpha )(x) =$ det ad$_{\mathfrak{g}/\mathfrak{t}}(x)$.

Cho $\omega_{G/T}$ là một dạng vi phân bất biến bậc $n-r$ trên $G/T$ và $\omega_{\mathfrak{t}}$ là một dạng vi phân bất biến qua tịnh tiến bậc $r$ trên $\mathfrak{t}$. Theo ký hiệu ở số 1, ký hiệu $\omega_{G/T}\cap \omega_{\mathfrak{t}}$ dạng vi phân bất biến qua tịnh tiến duy nhất $\omega_{\mathfrak{g}}$ bậc $n$ trên $\mathfrak{g}$ sao cho $\omega_{\mathfrak{g}}(0) =\omega_{G/T}(\overline{e})\cap \omega_{\mathfrak{t}}(0)$.

Cuối cùng, ký hiệu $\psi : (G/T)\times \mathfrak{t}\rightarrow \mathfrak{g}$ là cấu xạ của các đa tạp cảm sinh bởi ánh xạ $(g, x) \rightarrow$ (Ad $g$)$(x)$ từ $G\times \mathfrak{t}$ đến $\mathfrak{g}$ bằng cách qua thương.

#### Mệnh đề 3 {#lie-ix-s6-prop-3 .statement tag=01FB}

Cho $\omega_{\mathfrak{g}},\omega_{\mathfrak{t}},\omega_{G/T}$ lần lượt là các dạng vi phân bất biến trên $\mathfrak{g},\mathfrak{t}$, $G/T$, có các bậc tương ứng $n, r, n-r$. Nếu $\omega_{\mathfrak{g}}=\omega_{G/T}\cap \omega_{\mathfrak{t}}$, ta có

$$
\psi^*\omega_{\mathfrak{g}}=\omega_{G/T}\wedge \pi_{\mathfrak{g}}\omega_{\mathfrak{t}}
$$

trong đó $\pi_{\mathfrak{g}}$ là hàm trên $\mathfrak{t}$ được xác định bởi $\pi_{\mathfrak{g}}(x) =\prod_{\alpha\in R(G,T)}\delta (\alpha )(x)$.

Ký hiệu $\omega_G$ (resp. $\omega_T$) là dạng vi phân bất biến bậc lớn nhất trên G (resp. T) trùng với $\omega_{\mathfrak{g}}$ (resp. $\omega_{\mathfrak{t}}$) tại gốc. Xét biểu đồ giao hoán

$$
(G/T)\times \mathfrak{t}\longrightarrow^{\psi}\mathfrak{g}
$$

(Id,exp$_T$) exp$_G$.

$(G/T)\times T\longrightarrow^f$ G

Nhờ Mệnh đề 1 của no. 2 và hệ thức exp$^*_T\omega_T=\omega_{\mathfrak{t}}$, ta suy ra đẳng thức

$\psi^*$exp$^*_G\omega_G=\omega_{G/T}\wedge \delta_{\mathfrak{g}}\omega_{\mathfrak{t}}$.

Theo Mệnh đề $2,\psi^*$exp$^*_G\omega_G= (\psi^*\lambda_{\mathfrak{g}})\psi^*\omega_{\mathfrak{g}}$. Vì hàm $\lambda_{\mathfrak{g}}$ bất biến dưới Ad(G), ta có $(\psi^*\lambda_{\mathfrak{g}})(\overline{g}, x) =\lambda_{\mathfrak{g}}(x) =\frac{\delta_{\mathfrak{g}}(x)}{\pi_{\mathfrak{g}}(x)}$ với $\overline{g}\in G/T, x\in \mathfrak{t}$.

Suy ra các dạng $\psi^*\omega_G(\overline{g}, x)$ và $\omega_{G/T}(\overline{g})\wedge \pi_{\mathfrak{g}}(x)\omega_{\mathfrak{t}}(x)$ trùng nhau tại những điểm mà $\delta_{\mathfrak{g}}(x)$ khác không, tức là trên tập con mở trù mật $(G/T)\times \mathfrak{t}_r$; do đó chúng bằng nhau, suy ra mệnh đề.

Chọn các dạng vi phân bất biến $\omega_G$ trên G và $\omega_T$ trên T, có bậc lớn nhất, sao cho $|\omega_G|=dg$ và $|\omega_T|=dt$; ký hiệu $\omega_{\mathfrak{g}}$ (resp. $\omega_{\mathfrak{t}}$) là dạng vi phân bất biến qua phép tịnh tiến trên $\mathfrak{g}$ (resp. $\mathfrak{t}$) trùng với $\omega_G(e)$ (resp. $\omega_T(e)$) tại gốc, và $dz$ (resp. $dx$) là độ đo Haar $|\omega_{\mathfrak{g}}|$ (resp. $|\omega_{\mathfrak{t}}|$). Lập luận như ở no. 2, với những sửa đổi thích hợp, cho ta mệnh đề sau:

#### Mệnh đề 4 {#lie-ix-s6-prop-4 .statement tag=01FC}

Độ đo $dz$ trên $\mathfrak{g}$ là ảnh của độ đo $dg\otimes \frac{1}{w(G)}\pi_{\mathfrak{g}}dx$ qua ánh xạ riêng $(g, x) \rightarrow$ (Ad $g$)$(x)$ từ $G\times \mathfrak{t}$ đến $\mathfrak{g}$.

Chúng tôi để cho độc giả phát biểu và chứng minh các kết quả tương tự của Hệ quả 1 đến 3 và các Nhận xét 1 đến 3 của no. 2. Ví dụ, cho $\varphi$ là một hàm khả tích trên $\mathfrak{g}$ (nhận giá trị trong một không gian Banach hoặc $\overline{\mathbf{R}}$); khi đó

$\int_{\mathfrak{g}}\varphi (z)dz=\frac{1}{w(G)}\int_{\mathfrak{t}}(\int_G\varphi$((Ad $g$)$x$)$dg)\pi_{\mathfrak{g}}(x)dx$, (12)

và, nói riêng, nếu $\varphi$ bất biến dưới Ad(G),

$$
\int_{\mathfrak{g}}\varphi (z)dz=\frac{1}{w(G)}\int_{\mathfrak{t}}\varphi (x)\pi_{\mathfrak{g}}(x)dx \tag{13}
$$

### 4. TÍCH PHÂN CÁC TIẾT DIỆN CỦA MỘT BÓ VECTƠ

Trong số này và số tiếp theo, ta ký hiệu X là một đa tạp thực lớp $C^r$ $(1\leq r\leq  \infty )$, địa phương có số chiều hữu hạn.

Cho Y là một đa tạp lớp $C^r$. Nếu $r <\infty$, xét ánh xạ $f \rightarrow$ $j^r(f)$ từ $\mathscr{C}^r(X; Y)$ đến $\mathscr{C}(X; J^r(X,Y)) ($Differentiable and Analytic Manifolds, Results, 12.3.7). Ảnh ngược qua ánh xạ này của tôpô hội tụ compact trên $\mathscr{C}(X; J^r(X,Y))$ được gọi là tôpô hội tụ compact $C^r$ trên $\mathscr{C}^r(X; Y)$; nó là cận trên của các tôpô hội tụ đều $C^r$ trên K (Differentiable and Analytic Manifolds, Results, 12.3.10), trong đó K chạy qua tập các tập con compact của X.

Khi $r$ = $\infty$, ta gọi tôpô hội tụ compact $C^{\infty}$ trên $\mathscr{C}^{\infty}(X; Y)$ là cận trên của các tôpô hội tụ compact $C^k$, nói cách khác là tôpô thô nhất sao cho các nhúng chính tắc $\mathscr{C}^{\infty}(X; Y)\rightarrow \mathscr{C}^k(X; Y)$ là liên tục đối với $0\leq k <\infty$.

Cho E là một bó vectơ thực với cơ sở X, thuộc lớp $C^r$, và cho $\mathscr{S}^r(X; E)$ là không gian vectơ các tiết diện của E thuộc lớp $C^r$. Trong số này ta trang bị cho $\mathscr{S}^r(X; E)$ tôpô cảm sinh bởi tôpô hội tụ compact $C^r$ trên $\mathscr{C}^r(X; E)$, cũng gọi là tôpô hội tụ compact $C^r$; nó biến $\mathscr{S}^r(X; E)$ thành một không gian vectơ tôpô lồi địa phương, tách rời và đầy đủ (xem Differentiable and Analytic Manifolds, Results, 15.3.1 và Spectral Theories, in preparation).

Bây giờ cho H là một nhóm Lie, $m: H\times X\rightarrow X$ là một luật tác động trái thuộc lớp $C^r$; đặt $hx=m(h, x)$ với $h\in H, x\in X$. Cho E là một bó H-vectơ với cơ sở X, thuộc lớp $C^r$ (Chap. III, §1, no. 8, Def. 4). Với $s\in \mathscr{S}^r(X; E)$ và $h\in H$, ký hiệu $^hs$ là tiết diện $x \rightarrow h.s(h^{-1}x)$ của E; ánh xạ $(h, s) \rightarrow^hs$ là một luật tác động của H lên không gian $\mathscr{S}^r(X; E)$.

#### Bổ đề 4 {#lie-ix-s6-lem-4 .statement tag=01FD}

Luật tác động $H\times \mathscr{S}^r(X; E)\rightarrow \mathscr{S}^r(X; E)$ là liên tục.

Xét theo định nghĩa của tôpô của $\mathscr{S}^r(X; E)$ và General Topology, Chap. X, §3, no. 4, Định lý 3, đủ để chứng minh rằng với mọi số nguyên $k\leq r$, ánh xạ $f: H\times X\times \mathscr{S}^k(X; E)\rightarrow J^k(X; E)$ sao cho $f(h, x, s) =j_x^k(^hs)$ là liên tục. Với $h\in H$, ký hiệu $\tau_h$ (tương ứng $\theta_h$) là tự đẳng cấu $x \rightarrow hx$ của X (tương ứng của E). Định nghĩa các ánh xạ

$$
f_1:H\times X\rightarrow J^k(X,X)
$$

$$
f_2:H\times E\rightarrow J^k(E,E)
$$

$$
g:H\times X\times \mathscr{S}^k(X; E)\rightarrow J^k(X,E)
$$

bởi $f_1(h, x) =j^k_x(\tau_h), f_2(h, v) =j_v^k(\theta_h), g(h, x, s) =j_{hx}^k(s)$. Ta có

$$
f(h, x, s) =f_2(h, s(h^{-1}x))\circ g(h^{-1}, x, s)\circ f_1(h^{-1}, x)
$$

và do đó, theo Differentiable and Analytic Manifolds, Results, 12.3.6, đủ để chứng minh rằng $f_1, f_2$ và $g$ là liên tục.

Bây giờ $g$ là ánh xạ hợp thành

$$
H\times X\times \mathscr{S}^k(X; E)-------\longrightarrow^{(m,Id)}X\times \mathscr{S}^k(X; E)
$$

$$
-------\longrightarrow^{(Id,j^k)}X\times \mathscr{C}(X; J^k(X,E))\longrightarrow^{\varepsilon}J^k(X,E)
$$

với $\varepsilon (x, u) =u(x)$; vì $\varepsilon$ liên tục (General Topology, Chap. X, §3, no. 4, Hệ quả 1 của Định lý $3$), nên $g$ liên tục.

Cho $(h_0, x_0)\in H\times X$; ta sẽ chứng minh rằng $f_1$ liên tục tại $(h_0, x_0)$. Tồn tại các biểu đồ $(U, \psi ,F)$ và $(V, \chi ,F')$ của X và một tập con mở $\Omega$ của H sao cho $x_0\in U, h_0\in \Omega$ và $m(\Omega \times U)\subset V$. Dùng biểu thức của $J^k(X,X)$ trong các biểu đồ này, ta quy về việc chứng minh, với $1\leq l\leq k$, tính liên tục tại $(h_0, x_0)$ của ánh xạ $(h, x) \rightarrow \Delta^l_x(\tau_h)$ từ $\Omega \times U$ đến $P_l(F; F')$, với $\Delta^l_x(\tau_h)(v) =$ $\frac{1}{l!}D^l\tau_h(x).v$ đối với $v\in F ($Differentiable and Analytic Manifolds, Results, 12.2). Nhưng $D^l\tau_h(x)$ chỉ đơn giản là đạo hàm riêng bậc $l$ của $m(h, x)$ theo $x$, vốn liên tục theo giả thiết; do đó, $f_1$ liên tục. Chứng minh rằng $f_2$ liên tục là tương tự, do đó suy ra bổ đề.

#### Mệnh đề 5 {#lie-ix-s6-prop-5 .statement tag=01FE}

Giả sử nhóm H là compact và ký hiệu $dh$ là độ đo Haar trên H có tổng khối lượng bằng 1. Cho $s$ là một tiết diện của E lớp $C^r$. Ký hiệu $s^{\sharp}$ là tích phân vectơ $\int_H^hs dh$. Khi đó $s^{\sharp}$ là một tiết diện của E lớp $C^r$, bất biến dưới H; với $x\in X$, ta có $s^{\sharp}(x) =\int_Hhs(h^{-1}x)dh\in E_x$. Tự đồng cấu $s \rightarrow s^{\sharp}$ của $\mathscr{S}^r(X; E)$ là một phép chiếu lên không gian con các tiết diện bất biến dưới H.

Xét ánh xạ $h \rightarrow^hs$ từ H đến $\mathscr{S}^r(X; E)$; nó liên tục theo Bổ đề 4. Vì không gian $\mathscr{S}^r(X; E)$ tách biệt và đầy đủ, nên tích phân $s^{\sharp}=$ $\int_H^hs dh$ thuộc $\mathscr{S}^r(X; E)$ (Integration, Chương III, §3, no. 3, Hệ quả 2). Vì ánh xạ tuyến tính $s \rightarrow s(x)$ từ $\mathscr{S}^r(X; E)$ đến $E_x$ là liên tục, ta có $s^{\sharp}(x) =$ $\int_H^hs(x)dh$ với mọi $x\in X$. Rõ ràng $s^{\sharp}$ bất biến dưới H; nếu $s$ là một tiết diện bất biến dưới H, ta có $s^{\sharp}=s$, do đó khẳng định cuối cùng.

#### Hệ quả 1 {#lie-ix-s6-prop-5-cor-1 .statement tag=01FF}

Cho F là một không gian Banach, $\rho : H\rightarrow \mathbf{G}\mathbf{L}(F)$ là một biểu diễn tuyến tính giải tích, $f\in \mathscr{C}^r(X; F)$. Với $x\in X$, đặt

$$
f^{\sharp}(x) =\int_H\rho (h).f(h^{-1}x)dh
$$

Khi đó $f^{\sharp}$ là một cấu xạ lớp $C^r$ từ X đến F, tương thích với các tác động của H; với $x\in X$, ta có (với $\tau_h$ ký hiệu tự đẳng cấu $x \rightarrow hx$ của X)

$$
d_xf^{\sharp}=\int_H(\rho (h)\circ d_{h^{-1}x}f\circ T_x(\tau_{h^{-1}}))dh\in \mathscr{L}(T_x(X); F) \tag{14}
$$

Mệnh đề thứ nhất suy ra từ mệnh đề được áp dụng cho bó $X\times$ F, được trang bị bởi luật của phép toán $(h; (x, f)) \rightarrow (hx, \rho (h).f)$. Mệnh đề thứ hai suy ra từ Integration, Chương III, §3, no. 2, Mệnh đề 2, bằng cách áp dụng lên nguyên vectơ $f^{\sharp}$ đồng cấu $d_x:\mathscr{C}^r(X; F)\rightarrow \mathscr{L}(T_x(X); F)$ vốn liên tục theo định nghĩa của tôpô hội tụ compact $C^r$.

#### Hệ quả 2 {#lie-ix-s6-prop-5-cor-2 .statement tag=01FG}

Cho F là một không gian Banach, $f\in \mathscr{C}^r(X; F)$; đặt

$$
f^{\sharp}(x) =\int_Hf(hx)dh
$$

với $x\in X$. Hàm $f^{\sharp}$ thuộc lớp $C^r$, và $f^{\sharp}(hx) =f^{\sharp}(x)$ với $x\in X$, $h\in H$.

#### Hệ quả 3 {#lie-ix-s6-prop-5-cor-3 .statement tag=01FH}

Cho F là một không gian Banach, $p$ là một số nguyên $\geq 0,^k\Omega^p(X; F)$ là không gian các dạng vi phân bậc $p$ trên X, với giá trị trong F, và thuộc lớp $C^k(2\leq k+ 1\leq r)$. Với $\omega \in^k\Omega^p(X; F)$, đặt $\omega^{\sharp}=\int_H\tau_h^*\omega  dh$. Khi đó ánh xạ $\omega  \rightarrow \omega^{\sharp}$ là một phép chiếu trên $^k\Omega^p(X; F)$ có ảnh là không gian các dạng bất biến theo H. Ta có $d(\omega^{\sharp}) = (d\omega )^{\sharp}$ với mọi $\omega \in^k\Omega^p(X; F)$.

Mệnh đề thứ nhất suy ra từ mệnh đề được áp dụng cho bó vectơ H Alt$^p(T(X); F)$ (Chương III, §1, no. 8, Ví dụ). Để chứng minh mệnh đề thứ hai, chỉ cần, xét theo Integration, Chương III, §3, no. 2, Mệnh đề 2, chứng minh rằng ánh xạ $d:^k\Omega^p(X; F)\rightarrow^{k-1}\Omega^{p+1}(X; F)$ là liên tục khi không gian thứ nhất (tương ứng thứ hai) được trang bị tôpô hội tụ compact $C^k$ (tương ứng $C^{k-1}$). Nhưng điều này suy ra ngay lập tức từ định nghĩa của các tôpô này bằng các nửa chuẩn (Spectral Theories, in preparation) và thực tế là $d$ là một toán tử vi phân bậc $\leq 1 ($Differentiable and Analytic Manifolds, Results, 14.4.2).

### 5. CÁC DẠNG VI PHÂN BẤT BIẾN

Cho X là một đa tạp thực hữu hạn địa phương chiều thuộc lớp $C^{\infty}$, và cho $(g, x) \rightarrow gx$ là một luật của phép toán trái thuộc lớp $C^{\infty}$ của một nhóm Lie compact liên thông G trên X. Với $g\in G$, ký hiệu $\tau_g$ là tự đẳng cấu $x \rightarrow gx$ của X. Ký hiệu $\Omega (X)$ là đại số các dạng vi phân thực thuộc lớp $C^{\infty}$ trên X (Differentiable and Analytic Manifolds, Results, 8.3.1).

Với mọi phần tử $\xi$ của $\mathfrak{g}$, ký hiệu $D_{\xi}$ là trường vectơ tương ứng trên X (Chương III, §3, no. 5) và $\theta (\xi ), i(\xi )$ là các toán tử tương ứng trên $\Omega$(X), do đó ta có các công thức (Differentiable and Analytic Manifolds, Results, 8.4.5 and 8.4.7)

$$
\theta (\xi )\omega =d(i(\xi )\omega ) +i(\xi )d\omega \tag{15}
$$

$$
d_**
$$

$$
(\tau_{expt\xi}\omega ) =\tau_{expt\xi}(\theta (\xi )\omega ) \tag{16}
$$

$$
dt
$$

Một dạng vi phân $\omega \in \Omega (X)$ là bất biến nếu $\tau_g^*\omega =\omega$ với mọi $g\in G$; theo công thức (16), điều này tương đương với $\theta (\xi )\omega = 0$ với mọi $\xi \in \mathfrak{g}$. Ký hiệu $\Omega (X)^G$ là không gian các dạng vi phân bất biến trên X; nếu $\omega \in \Omega (X)^G$, ta có $d\omega \in \Omega (X)^G$, nên $\Omega (X)^G$ là một dưới phức của phức $(\Omega (X), d)$.

#### Định lý 2 {#lie-ix-s6-thm-2 .statement tag=01FI}

Phép đơn ánh chính tắc $\iota :\Omega (X)^G\rightarrow \Omega (X)$ là một đồng luân tương đương của các phức (Algèbre, Chap. X, p. 33, déf. 5); ánh xạ $\omega  \rightarrow \omega^{\sharp}=\int_G\tau_g^*\omega  dg$ là một đồng luân tương đương, nghịch đảo của nó tới sai khác đồng luân. Đặc biệt, ánh xạ $H(\iota ) : H(\Omega (X)^G)\rightarrow H(\Omega (X))$ là song ánh.

Theo Hệ quả 3 của no. 4, ánh xạ $\omega  \rightarrow \omega^{\sharp}$ là một cấu xạ của phức từ $\Omega (X)$ đến $\Omega (X)^G$ cảm sinh đồng nhất trên dưới phức $\Omega (X)^G$; do đó, để chứng minh định lý chỉ cần xây dựng một đồng cấu $s:\Omega (X)\rightarrow \Omega$(X), phân bậc bậc $-1$, sao cho

$\omega^{\sharp}-\omega = (d\circ s+s\circ d)(\omega )$ cho mọi $\omega \in \Omega (X)$. (17)

Theo Bổ đề 1 của phần Tích phân, Chương IX, §2, no. 4 và Nhận xét 1 của §2, no. 2, tồn tại một độ đo dương $d\xi$ trên $\mathfrak{g}$ có giá compact mà ảnh của nó qua ánh xạ mũ bằng $dg$. Với $\omega \in \Omega$(X), đặt

$$
s(\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(i(\xi )\omega ).d\xi \}dt
$$

ta phải chứng minh rằng công thức (17) được thỏa mãn. Như trong chứng minh của Hệ quả 1 (no. 4), ta kiểm tra công thức

$$
ds(\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*d(i(\xi )\omega ).d\xi \}dt
$$

Bây giờ ta suy ra từ các công thức (15) và (16) các đẳng thức

$$
ds(\omega ) +s(d\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(d(i(\xi )\omega ) +i(\xi )d\omega ).d\xi \}dt
$$

$$
=\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(\theta (\xi )\omega ).d\xi \}dt
$$

$$
=\int_{\mathfrak{g}}\{\int_0^1\frac{d}{dt}(\tau_{expt\xi}^*\omega )dt\}d\xi
$$

$$
=\int_{\mathfrak{g}}(\tau_{exp\xi}^*\omega -\omega )d\xi
$$

$$
=\omega^{\sharp}-\omega
$$

suy ra ĐL. 2.

Ta áp dụng định lý trong trường hợp X = G, với tác động của G bởi các phép tịnh tiến trái. Nhắc lại (Chương III, §3, no. 13, Mệnh đề 50) rằng gán cho một dạng vi phân trên G giá trị của nó tại phần tử đơn vị cho một đẳng cấu từ $\Omega (G)^G$ đến đại số phân bậc Alt($\mathfrak{g}$) của các dạng đa tuyến tính phản xứng trên $\mathfrak{g}$. Đồng nhất $\Omega (G)^G$ với Alt($\mathfrak{g}$) nhờ đẳng cấu này. Khi đó toán tử $d$ được cho bởi công thức (Chương III, §3, no. 14, Mệnh đề 51)

$$
d\omega (a_1, . . . , a_{p+1})
$$

$$
=\sum_{i<j}(-1)^{i+j}\omega ([a_i, a_j], a_1, . . . , a_{i-1}, a_{i+1}, . . . , a_{j-1}, a_{j+1}, . . . , a_{p+1})
$$

đối với $\omega$ trong Alt$^p(\mathfrak{g})$ và $a_1, . . . , a_{p+1}$ trong $\mathfrak{g}$.

Với $\xi \in \mathfrak{g}$, ký hiệu $L_{\xi}$ là trường vectơ trái bất biến tương ứng (được định nghĩa nhờ tác động của G lên chính nó bởi các phép tịnh tiến phải, xem Chương III, §3, no. 6). Các toán tử $\theta (L_{\xi}), i(L_{\xi})$ giao hoán với tác động của G trên $\Omega (G)$ được định nghĩa bởi phép tịnh tiến trái, và do đó cảm sinh các toán tử $\theta (\xi ), i(\xi )$ trên $\Omega (G)^G$; với các đồng nhất trước đó, chúng được biểu diễn bởi các công thức (Differentiable and Analytic Manifolds, Results, 8.3.2 and 8.4.2)

$$
(\theta (\xi )\omega )(a_1, . . . , a_p) =-\sum_i\omega (a_1, . . . , a_{i-1},[\xi , a_i], a_{i+1}, . . . , a_p)
$$

$$
(i(\xi )\omega )(a_1, . . . , a_{p-1}) =\omega (\xi , a_1, . . . , a_{p-1})
$$

đối với $\omega$ trong Alt$^p(\mathfrak{g})$ và $a_1, . . . , a_p$ trong $\mathfrak{g}$.

Dưới phức $^G\Omega (G)^G$ của các dạng bất biến kép (Chương III, §3, no. 13) có thể đồng nhất với dưới phức Alt($\mathfrak{g}$)$^G$ của các dạng đa tuyến tính phản xứng trên $\mathfrak{g}$ bất biến dưới biểu diễn liên hợp (tức là sao cho $\theta (\xi )\omega = 0$ với mọi $\xi \in \mathfrak{g}$). Do đó, ta có một biểu đồ giao hoán của các phức

$$
^G\Omega (G)^G\longrightarrow \Omega (G)^G\longrightarrow \Omega (G)
$$

(18)

Alt($\mathfrak{g}$)$^G\longrightarrow$ Alt($\mathfrak{g}$)

trong đó các mũi tên ngang là các phép nhúng chính tắc, và các mũi tên dọc là các đẳng cấu cảm sinh bởi ánh xạ $\omega  \rightarrow \omega (e)$.

#### Hệ quả 1 {#lie-ix-s6-thm-2-cor-1 .statement tag=01FJ}

a) Trong biểu đồ (18), mọi cấu xạ đều là các homotopism.

b) Cho $\omega \in$ Alt($\mathfrak{g}$). Khi đó $\omega$ thuộc Alt($\mathfrak{g}$)$^G$ khi và chỉ khi $d\omega = 0$ và $d(i(\xi )\omega ) = 0$ với mọi $\xi \in \mathfrak{g}$. Toán tử vi phân của phức Alt($\mathfrak{g}$)$^G$ bằng 0.

c) Không gian vectơ phân bậc $H(\Omega (G))$ đẳng cấu với Alt($\mathfrak{g}$)$^G$.

Định lý, áp dụng cho tác động của G lên G bởi các phép tịnh tiến trái (tương ứng, cho tác động $((g, h);x) \rightarrow gxh^{-1}$ của $G\times G$ lên G) suy ra rằng đơn ánh chính tắc $\Omega (G)^G\rightarrow \Omega (G)$ (tương ứng, $^G\Omega (G)^G\rightarrow \Omega (G)$) là một tương đương đồng luân; theo Algèbre, Chap. X, p. 34, Cor., suy ra mệnh đề a).

Ta chứng minh b). Theo Prop. 51 của Chap. III, §3, no. 14, ta có $d\alpha =-d\alpha$, tức là $d\alpha = 0$, với mọi dạng vi phân $\alpha$ trên G vừa bất biến trái vừa bất biến phải. Do đó, nếu $\omega \in$ Alt($\mathfrak{g}$)$^G$, thì $d\omega = 0$, và do đó $d(i(\xi )\omega ) =$ $\theta (\xi )\omega -i(\xi )d\omega = 0$. Ngược lại, nếu $d\omega = 0$ và $d(i(\xi )d\omega ) = 0$, thì $\theta (\xi )\omega = 0$.

Mệnh đề c) suy ra từ a) và b).

#### Nhận xét {#lie-ix-s6-n5-rem-1 .statement tag=01FK}

Xét các phức con $Z(\Omega (G))$ và $B(\Omega (G))$ của $\Omega (G) ($Algèbre, Chap. X, p. 25). Từ công thức cho vi phân của tích của hai dạng (Differentiable and Analytic Manifolds, Results, 8.3.5) suy ra rằng $Z(\Omega (G))$ là một đại số con của $\Omega (G)$ và $B(\Omega (G))$ là một iđêan của $Z(\Omega (G))$; do đó, tích ngoài cảm sinh một cấu trúc đại số phân bậc trên $H(\Omega (G))$. Kết quả trên nay cho một đẳng cấu của các đại số phân bậc $H(\Omega (G))\rightarrow$ Alt($\mathfrak{g}$)$^G$.

Cho H là một nhóm con đóng của G; ta áp dụng Th. 2 cho $X = G/H$. Theo Chap. III, §1, no. 8, Cor. 1 của Prop. 17, các dạng vi phân bất biến theo G trên $G/H$ có thể được đồng nhất với các phần tử bất biến theo H của Alt(T$_e(G/H)$), tức là với các phần tử của Alt($\mathfrak{g}$) bất biến theo H và bị triệt tiêu bởi các toán tử $i(\xi )$ với mọi $\xi \in L(H)$. Do đó:

#### Hệ quả 2 {#lie-ix-s6-thm-2-cor-2 .statement tag=01FL}

Cho H là một nhóm con đóng của G.

a) Đơn ánh chính tắc $\Omega (G/H)^G\rightarrow \Omega (G/H)$ là một tương đương đồng luân.

b) Phức $\Omega (G/H)^G$ có thể được đồng nhất với phức con của Alt($\mathfrak{g}$) gồm các phần tử $\omega$ của Alt($\mathfrak{g}$) bất biến dưới biểu diễn kề của H và sao cho $i(\xi )\omega = 0$ với mọi $\xi \in L(H)$. Nếu, hơn nữa, H liên thông, thì phức con này gồm các $\omega \in$ Alt($\mathfrak{g}$) sao cho $\theta (\xi )\omega = 0$ và $i(\xi )\omega = 0$ với mọi $\xi \in L(H)$.

### Bài tập {#lie-ix-s6-exercises}

Xem [bài tập cho § 6](exercises/s6/).
