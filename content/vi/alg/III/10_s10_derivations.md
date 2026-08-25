---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 10
section_title: Derivations
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0574-0598, 0669-0670
extraction: ocr
subsections:
    - "no": 1
      title: COMMUTATION FACTORS
      page: 0
      pdf_page: 574
    - "no": 2
      title: GENERAL DEFINITION OF DERIVATIONS
      page: 0
      pdf_page: 575
    - "no": 3
      title: EXAMPLES OF DERIVATIONS
      page: 0
      pdf_page: 577
    - "no": 4
      title: COMPOSITION OF DERIVATIONS
      page: 0
      pdf_page: 578
    - "no": 5
      title: DERIVATIONS OF AN ALGEBRA A INTO AN A-MODULE
      page: 0
      pdf_page: 581
    - "no": 6
      title: DERIVATIONS OF AN ALGEBRA
      page: 0
      pdf_page: 583
    - "no": 7
      title: Functorial Properties
      page: 0
      pdf_page: 584
    - "no": 8
      title: RELATIONS BETWEEN DERIVATIONS AND ALGEBRA HOMOMORPHISMS
      page: 0
      pdf_page: 585
    - "no": 9
      title: EXTENSION OF DERIVATIONS
      page: 0
      pdf_page: 586
    - "no": 10
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; NON-COMMUTATIVE CASE
      page: 0
      pdf_page: 591
    - "no": 11
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; COMMUTATIVE CASE
      page: 0
      pdf_page: 592
    - "no": 12
      title: FUNCTIORIAL PROPERTIES OF K-DIFFERENTIALS
      page: 0
      pdf_page: 594
statements: 41
exercises: 5
content_sha256: bf144adb8ffae9888bbd467e461e3172df43e563b22c1c60cd6b7f5c218cd671
translated_from: content/en/alg/III/10_s10_derivations.md
source_content_sha256: 16a1c152f622a064eb59a1f7fd58156eb456421b2fbffd3bc85193e30f63bc79
translation_model: gpt-5.4-mini
translation_run: translate-vi-6a225208
glossary_version: 34
glossary_terms_sha256: 2dbe9224324fb992191eac5e3b5f1517ca8fca87901836fac70d5198967c2f53
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. ĐẠO HÀM

Trong đoạn này, và trừ khi có nói khác, các đại số được xét không được giả sử là kết hợp cũng không nhất thiết có phần tử đơn vị; K ký hiệu một vành giao hoán.

### 1. CÁC NHÂN TỬ GIAO HOÁN

Khi trong đoạn này ta nói về các phân bậc mà không nói rõ chúng, ta luôn hiểu là các phân bậc kiểu $\Delta$, trong đó $\Delta$ là một nhóm giao hoán viết theo phép cộng. Trong đoạn này, một nhân tử giao hoán trên $\Delta$ với giá trị trong $\mathbf{Z}$ được gọi là một nhân tử giao hoán trên $\Delta$ (§ 4, no. 7, Định nghĩa 6). Do đó, một nhân tử giao hoán trên $\Delta$ được đồng nhất với một ánh xạ $\varepsilon : (\alpha, \beta) \mapsto \varepsilon_{\alpha \beta} = \varepsilon(\alpha, \beta)$ của $\Delta \times \Delta$ vào nhóm nhân $\{-1, 1\}$ sao cho với $\alpha, \alpha', \beta, \beta'$ trong $\Delta$,

$$
\begin{cases}
\varepsilon(\alpha + \alpha', \beta) = \varepsilon(\alpha, \beta)\varepsilon(\alpha', \beta) \\
\varepsilon(\alpha, \beta + \beta') = \varepsilon(\alpha, \beta)\varepsilon(\alpha, \beta') \\
\varepsilon(\beta, \alpha) = \varepsilon(\alpha, \beta).
\end{cases}
$$

(1)

Suy ra rằng $\varepsilon(2\alpha, \beta) = \varepsilon(\alpha, 2\beta) = 1$.

Khi $\Delta = \mathbf{Z}$, mọi nhân tử giao hoán $\varepsilon$ đều được xác định bởi việc cho $\varepsilon(1, 1)$; vì vậy chỉ có *hai* nhân tử như thế, nhân tử thứ nhất được xác định bởi

(2)
$$
\varepsilon(p, q) = 1 \quad \text{for } p, q \text{ in } \mathbf{Z}
$$
và nhân tử thứ hai bởi
(3)
$$
\varepsilon(p, q) = (-1)^{pq} \quad \text{for } p, q \text{ in } \mathbf{Z}.
$$

### 2. ĐỊNH NGHĨA TỔNG QUÁT VỀ ĐẠO HÀM

Xét một vành giao hoán $K$, sáu môđun phân bậc $K$ kiểu $\Delta : A, A', A'', B, B', B''$, và ba ánh xạ tuyến tính của $K$
$$
\mu : A \times A' \to A'', \qquad \lambda_1 : B \times A' \to B'', \qquad \lambda_2 : A \times B' \to B''
$$
sao cho các ánh xạ tuyến tính của $K$ tương ứng
$$
A \otimes_K A' \to A'', \qquad B \otimes_K A' \to B'', \qquad A \otimes_K B' \to B''
$$
đều là *phân bậc bậc 0*. Ảnh $\mu(a, a')$ với $a \in A, a' \in A'$ được ký hiệu đơn giản là $a.a'$ hay thậm chí $aa'$, và tương tự cho hai ánh xạ song tuyến tính kia. Do đó, *bậc* của $a.a'$ là *tổng* các bậc của $a$ và $a'$.

#### Định nghĩa 1 {#alg-iii-s10-def-1 .statement}

*Cho những dữ kiện trên và một nhân tử giao hoán $\varepsilon$ trên $\Delta \times \Delta$, một $\varepsilon$-đạo hàm (hay $(K, \varepsilon)$-đạo hàm) bậc $\delta \in \Delta$ của $(A, A', A'')$ vào $(B, B', B'')$ là một bộ ba các ánh xạ tuyến tính phân bậc của $K$ bậc $\delta$:*
$$
d : A \to B, \qquad d' : A' \to B', \qquad d'' : A'' \to B''
$$
*sao cho, với mọi phần tử thuần nhất $a \in A$ và mọi phần tử $a' \in A'$*
(4)
$$
d''(a.a') = (da).a' + \varepsilon_{\delta, \deg(a)}a.(d'a').
$$

Rõ ràng, do tính tuyến tính, chỉ cần kiểm tra quan hệ (4) khi $a$ và $a'$ chạy qua các hệ sinh tương ứng của $A$ và $A'$.

Thường tiện hơn khi ký hiệu ba ánh xạ $d, d', d''$ bằng cùng một chữ $d$ (điều này có thể được biện minh bằng cách cũng ký hiệu bằng $d$ ánh xạ tuyến tính phân bậc của $K$ bậc $\delta$)

$$
(a, a', a'') \mapsto (da, d'a', d''a'')
$$

của $A \oplus A' \oplus A''$ vào $B \oplus B' \oplus B''$). Quan hệ (4) khi đó có thể được viết đơn giản hơn
$$
d(a.a') = (da).a' + \varepsilon_{\delta,\deg(a)} a.(da').
$$
Các $\varepsilon$-đạo hàm của $(A, A', A'')$ vào $(B, B', B'')$ có *bậc* cho trước tạo thành một K-môđun con của K-môđun các ánh xạ tuyến tính phân bậc
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
Khi $\varepsilon(\alpha, \beta) = 1$ với mọi $\alpha, \beta$ trong $\Delta$, ta chỉ gọi là *đạo hàm* (hoặc *K-đạo hàm*) thay cho $\varepsilon$-đạo hàm. Các đạo hàm tạo thành một K-môđun con của
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
Khi $\Delta = \mathbf{Z}$ và $\varepsilon(p.q) = (-1)^{pq}$, mọi $\varepsilon$-đạo hàm có bậc *chẵn* đều là một đạo hàm; mọi $\varepsilon$-đạo hàm có bậc *lẻ* thường được gọi là một *phản đạo hàm* (hoặc *K-phản đạo hàm*); do đó một phản đạo hàm $d$ thỏa mãn
$$
d(a.a') = (da).a' + (-1)^{\deg(a)} a.(da')
$$
với một phần tử *thuần nhất* $a \in A$.

#### Nhận xét {#alg-iii-s10-n2-rem-1 .statement}

(1) Khái niệm *đạo hàm* có thể được định nghĩa cho các môđun không phân bậc bằng cách quy ước cho các môđun này sự phân bậc tầm thường.

(2) Nếu chỉ xét các $\varepsilon$-đạo hàm có bậc $\delta$ cho trước, thì nhân tử giao hoán $\varepsilon$ có thể được bỏ đi như sau: ánh xạ song tuyến tính $\lambda_2 : A \times B' \to B''$ được sửa bằng cách thay nó bởi ánh xạ song tuyến tính $\lambda'_2 : A \times B' \to B''$ sao cho, với mọi $a$ *thuần nhất* trong $A$ và mọi $b' \in B'$,
$$
\lambda'_2(a, b') = \varepsilon_{\delta, \deg(a)} \lambda_2(a, b').
$$
Khi đó $d$ là một đạo hàm đối với các ánh xạ song tuyến tính $\mu, \lambda_1, \lambda'_2$.

Định nghĩa tổng quát của các $\varepsilon$-đạo hàm đã cho ở trên đặc biệt được dùng trong hai trường hợp:

*Trường hợp (I)*: $A = B, A' = B', A'' = B''$ và ba ánh xạ song tuyến tính $\mu, \lambda_1, \lambda_2$ đều bằng cùng một ánh xạ.

*Trường hợp (II)*: $A = A' = A'', B = B' = B''$, sao cho (đối với $\mu$) $A$ là một *đại số phân bậc* và hai ánh xạ song tuyến tính K.
$$
\lambda_1 : B \times A \to B, \quad \lambda_2 : A \times B \to B
$$
thỏa mãn rằng các ánh xạ K-tuyến tính tương ứng $B \otimes_K A \to B, A \otimes_K B \to B$ là phân bậc bậc 0. Một $\varepsilon$-đạo hàm bậc $\delta$ của $A$ vào $B$ khi đó là một ánh xạ K-tuyến tính phân bậc $d : A \to B$ có bậc $\delta$, sao cho với mọi $x$ thuần nhất trong $A$ và mọi $y \in A$, ta có quan hệ
$$
d(xy) = (dx)y + \varepsilon_{\delta, \deg(a)} x(dy).
$$

Xét riêng trong trường hợp (II) trường hợp A là một đại số K kết hợp có đơn vị và $\lambda_1$ và $\lambda_2$ là các luật ngoài của một song môđun $(A, A)$ (\S 4, no. 3, Định nghĩa 3). Điều này đúng, đáng chú ý là khi A và B là hai đại số K kết hợp có đơn vị, một đồng cấu có đơn vị của các đại số K phân bậc $\rho : A \to B$ được cho và một cấu trúc song môđun $(A, A)$ được xét trên B được xác định bởi hai luật ngoài

$$
\lambda_1 : (b, a) \mapsto b \rho(a), \qquad \lambda_2 : (a, b) \mapsto \rho(a)b
$$

với $a \in A, b \in B$.

Các trường hợp (I) và (II) có chung trường hợp sau đây: xét một đại số K phân bậc A, lấy $B = A$, cả hai ánh xạ (7) đều là phép nhân trên A. Khi đó ta nói về một $\varepsilon$-đạo hàm (hoặc (K, $\varepsilon$)-đạo hàm) của đại số phân bậc A: đó là một ánh xạ K-tuyến tính phân bậc của A vào chính nó, có bậc $\delta$, thỏa mãn (8) với mọi $x$ thuần nhất trong A và mọi $y \in A$. Đặc biệt, nếu A là một vành phân bậc, xét như một (kết hợp) $\mathbf{Z}$-đại số, ta nói về $\varepsilon$-đạo hàm của vành A.

Cho A là một đại số K có đơn vị, giao hoán, kết hợp và B là một A-môđun; khi nói đến một đạo hàm của A vào B, luôn hiểu rằng ta nói với cấu trúc song môđun A trên B được dẫn xuất từ cấu trúc A-môđun của nó; khi đó công thức

$$
d(xy) = x(dy) + y(dx) \quad \text{cho} \quad x \in A, y \in A
$$

đúng đối với một đạo hàm $d : A \to B$ như thế.

### 3. CÁC VÍ DỤ VỀ ĐẠO HÀM

#### Ví dụ 1 {#alg-iii-s10-n3-exa-1 .statement}

Cho A là một $\mathbf{R}$-đại số các ánh xạ khả vi từ $\mathbf{R}$ vào $\mathbf{R}$ và cho $x_0$ là một điểm của $\mathbf{R}$; $\mathbf{R}$ có thể được xem như một A-môđun với phép toán ngoài $(f, a) \mapsto f(x_0)a$. Khi đó ánh xạ $f \mapsto Df(x_0)$ là một đạo hàm, vì (Functions of a Real Variable, I, \S 1, no. 3)

$$
(D(fg))(x_0) = (Df(x_0))g(x_0) + f(x_0)(Dg(x_0)).*
$$

#### Ví dụ 2 {#alg-iii-s10-n3-exa-2 .statement}

Cho X là một đa tạp khả vi lớp $C^\infty$ và cho A là đại số $\mathbf{R}$ phân bậc của các dạng vi phân trên X. Ánh xạ gán cho mỗi dạng vi phân $\omega$ trên X vi phân ngoài $d\omega$ của nó là một phản đạo hàm có bậc +1 (Differentiable and Analytic Manifolds, R, \S 8).*

#### Ví dụ 3 {#alg-iii-s10-n3-exa-3 .statement}

Cho A là một đại số K kết hợp. Với mọi $a \in A$, ánh xạ $x \mapsto ax - xa$ là một đạo hàm của đại số A (xem no. 6).

#### Ví dụ 4 {#alg-iii-s10-n3-exa-4 .statement}

Cho M là một K-môđun và A là đại số ngoài $\bigwedge(M^*)$ với cách phân bậc thông thường của nó (\S 7, no. 1). *Sẽ thấy ở \S 11, no. 9 rằng, với mọi $x \in M$, tích trong phải $i(x)$ là một phản đạo hàm của A có bậc $-1$.*

#### Ví dụ 5 {#alg-iii-s10-n3-exa-5 .statement}

Quay lại tình huống tổng quát của Định nghĩa 1 của no. 2, cho $\overline{K}$ là một vành giao hoán khác và $\rho : K \to \overline{K}$ là một đồng cấu vành; ký hiệu $\overline{A}, \overline{A}', \overline{A}'', \overline{B}, \overline{B}', \overline{B}''$ là các môđun phân bậc $\overline{K}$ thu được tương ứng từ $A, A', A'', B, B', B''$ bằng cách mở rộng vành vô hướng lên $\overline{K}$ (II, § 11, no. 5); ta thu được từ $\mu, \lambda_1$ và $\lambda_2$ các ánh xạ $\overline{K}$-song tuyến tính
$$
\bar{\mu} : \overline{A} \times \overline{A}' \to \overline{A}'', \quad \bar{\lambda}_1 : \overline{B} \times \overline{A}' \to \overline{B}'', \quad \bar{\lambda}_2 : \overline{A} \times \overline{B}' \to \overline{B}''
$$
bằng cách xét các tích tenxơ với $l_{\overline{K}}$ của các ánh xạ K-tuyến tính tương ứng ứng với $\mu, \lambda_1$ và $\lambda_2$ (II, § 5, no. 1). Khi đó, nếu $d$ là một $\varepsilon$-đạo hàm có bậc $\delta$ của $(A, A', A'')$ vào $(B, B', B'')$, thì ánh xạ $\bar{d} = d \otimes l_{\overline{K}}$ của $\overline{A} \oplus \overline{A}' \oplus \overline{A}''$ vào $\overline{B} \oplus \overline{B}' \oplus \overline{B}''$ là một $\varepsilon$-đạo hàm có bậc $\delta$ của $(\overline{A}, \overline{A}', \overline{A}'')$ vào $(\overline{B}, \overline{B}', \overline{B}'')$.

#### Ví dụ 6 {#alg-iii-s10-n3-exa-6 .statement}

Cho $A$ là một đại số $K$ phân bậc kiểu $\mathbf{Z}$; một ánh xạ tuyến tính $K$ phân bậc có bậc 0, $d : A \to A$, được định nghĩa bằng cách lấy, với $x_n \in A_n (n \in \mathbf{Z})$, $d(x_n) = nx_n$. Ánh xạ này là một đạo hàm của $A$, vì, với $x_p \in A_p, x_q \in A_q$,
$$
d(x_p x_q) = (p + q)x_p x_q = d(x_p)x_q + x_p d(x_q).
$$

### 4. HỢP THÀNH CÁC ĐẠO HÀM

Ta giả sử trong số này rằng trường hợp (I) của no. 2 đúng, tức là $A, A', A''$ là ba môđun $K$ phân bậc kiểu $\Delta$ và rằng ta được cho một ánh xạ song tuyến tính $K$ $\mu : A \times A' \to A''$ tương ứng với một ánh xạ tuyến tính $K$ phân bậc có bậc 0, $A \otimes_K A' \to A''$. Các tự đồng cấu phân bậc $f$ của $A \oplus A' \oplus A''$ sao cho $f(A) \subset A, f(A') \subset A'$ và $f(A'') \subset A''$ tạo thành một đại số con phân bậc của đại số kết hợp phân bậc $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ (\S 3, no. 1, Ví dụ 2). Đặc biệt, hai $\varepsilon$-đạo hàm của $(A, A', A'')$ có thể được hợp thành, nhưng không nên nghĩ rằng hợp thành của hai $\varepsilon$-đạo hàm là một $\varepsilon$-đạo hàm.

Trên mọi đại số phân bậc $B$ kiểu $\Delta$ đều được định nghĩa ngoặc $\varepsilon$ (hay đơn giản là ngoặc khi $\varepsilon = 1$) của hai phần tử thuần nhất $u, v$, theo công thức (10)
$$
[u, v]_\varepsilon = uv - \varepsilon_{\deg u, \deg v} vu \text{ (được ký hiệu đơn giản bởi } [u, v] \text{ nếu } \varepsilon = 1).
$$
Bằng cách mở rộng ánh xạ này theo tính tuyến tính, ta thu được một ánh xạ song tuyến tính $K$ $(u, v) \mapsto [u, v]_\varepsilon$ từ $B \times B$ vào $B$. Khi đó, với $u$ và $v$ thuần nhất trong $B$
$$
[v, u]_\varepsilon = -\varepsilon_{\deg u, \deg v}[u, v]_\varepsilon.
$$
Áp dụng định nghĩa này cho đại số phân bậc $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$, ta do đó định nghĩa được ngoặc $\varepsilon$ của hai tự đồng cấu phân bậc.

#### Mệnh đề 1 {#alg-iii-s10-prop-1 .statement}

*Cho $d_1, d_2$ là hai $\varepsilon$-đạo hàm của $(A, A', A'')$ có các bậc tương ứng $\delta_1, \delta_2$. Khi đó, ngoặc $\varepsilon$*
$$
[d_1, d_2]_\varepsilon = d_1 \circ d_2 - \varepsilon_{\delta_1, \delta_2} d_2 \circ d_1
$$
*là một $\varepsilon$-đạo hàm bậc $\delta_1 + \delta_2$. Hơn nữa, nếu $d$ là một $\varepsilon$-đạo hàm của $(A, A', A'')$ có bậc $\delta$ và nếu $\varepsilon_{\delta, \delta} = -1$, thì $d^2 = d \circ d$ là một đạo hàm.*

Giả sử $x \in A$ là thuần nhất bậc $\xi$; với mọi $y \in A'$,
$$
d_1(d_2(xy)) = ((d_1 d_2)(x))y + \varepsilon_{\delta_1, \delta_2 + \xi}(d_2 x)(d_1 y)
+ \varepsilon_{\delta_2, \xi}(d_1 x)(d_2 y) + \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
$$
theo các công thức (1) của no. 1. Đổi vai trò của $d_1$ và $d_2$, ta được, sau khi rút gọn lại dùng (1) (no. 1),
$$
(d_1 d_2)(xy) - \varepsilon_{\delta_1, \delta_2}(d_2 d_1)(xy) = ((d_1 d_2)(x))y - \varepsilon_{\delta_1, \delta_2}((d_2 d_1)(x))y
+ \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
- \varepsilon_{\delta_1, \delta_2} \varepsilon_{\delta_1 + \delta_2, \xi} x((d_2 d_1)(y))
$$
tức là, viết $d = [d_1, d_2]_\varepsilon$ và $\delta = \delta_1 + \delta_2$,
$$
d(xy) = (dx)y + \varepsilon_{\delta, \xi} x(dy)
$$
điều đó chứng tỏ rằng $d$ là một $\varepsilon$-đạo hàm.

Mặt khác, nếu, trong (11), ta lấy $d_1 = d_2 = d$, $\delta_1 = \delta_2 = \delta$ và $\varepsilon_{\delta, \delta} = -1$, ta thu được, vì khi đó $\varepsilon_{\delta, \delta + \xi} = -\varepsilon_{\delta, \xi}$ theo (1),
$$
d^2(xy) = (d^2 x)y + \varepsilon_{2\delta, \xi} x(d^2 y)
$$
và như $\varepsilon_{2\delta, \xi} = 1$ thì thấy rằng $d^2$ là một đạo hàm.

#### Hệ quả {#alg-iii-s10-n4-cor-1 .statement}

*Giả sử rằng $\Delta = \mathbf{Z}$. Khi đó:*
(i) *Bình phương của một phản đạo hàm là một đạo hàm.*
(ii) *Ngoặc của hai đạo hàm là một đạo hàm.*
(iii) *Ngoặc của một phản đạo hàm và một đạo hàm có bậc chẵn là một phản đạo hàm.*
(iv) *Nếu $d_1$ và $d_2$ là các phản đạo hàm, thì $d_1 d_2 + d_2 d_1$ là một đạo hàm.*

Dưới các giả thiết ở đầu số này, xét bây giờ một dãy hữu hạn $D = (d_i)_{1 \leq i \leq n}$ gồm các *đạo hàm từng đôi một giao hoán* của $(A, A', A'')$. Với mọi đa thức $P(X_1, \ldots, X_n)$ trong đại số $K[X_1, \ldots, X_n]$, phần tử $P(d_1, \ldots, d_n)$ của $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ khi đó được xác định (\S 2, no. 9); ký hiệu tắt của nó là $P(D)$.

#### Mệnh đề 2 {#alg-iii-s10-prop-2 .statement}

*Với các giả thiết và ký hiệu trên, xét 2n biến vô định $T_1, \ldots, T_n, T'_1, \ldots, T'_n$ và với mọi đa thức $F \in K[X_1, \ldots, X_n]$ viết $F(T) = F(T_1, \ldots, T_n), F(T') = F(T'_1, \ldots, T'_n)$ và*
$$
F(T + T') = F(T_1 + T'_1, \ldots, T_n + T'_n).
$$
*Giả sử rằng*
$$
P(T + T') = \sum_i Q_i(T) R_i(T')
$$
*trong đó các $Q_i$ và $R_i$ thuộc $K[X_1, \ldots, X_n]$. Khi đó, với mọi $x \in A$ và $y \in A'$,*
$$
P(D)(xy) = \sum_i (Q_i(D)x)(R_i(D)y).
$$

Ta đưa thêm $n$ biến vô định khác $T_1'', \ldots, T_n''$ và xét đại số đa thức $K[T_1, \ldots, T_n, T_1', \ldots, T_n', T_1'', \ldots, T_n''] = B$; mặt khác ta xét $K$-môđun $M$ của các ánh xạ song tuyến tính từ $A \times A'$ vào $A''$; một cấu trúc $B$-môđun được xác định trên $M$ bằng cách viết, với mọi ánh xạ song tuyến tính trên $K$ $f \in M$ và $1 \leq i \leq n$,

$$
\begin{cases}
(T_i f)(a, a') = f(d_i a, a') \\
(T_i' f)(a, a') = f(a, d_i a') \\
(T_i'' f)(a, a') = d_i(f(a, a'))
\end{cases}
$$

Vì các $d_i$ giao hoán từng đôi một, thấy rằng, với mọi đa thức $F \in K[X_1, \ldots, X_n]$, $(F(T)f)(a, a') = f(F(D)a, a')$,

$$
(F(T')f)(a, a') = f(a, F(D)a')
$$

và $(F(T'')f) = F(D)(f(a, a'))$. Do đó, để chứng minh (12) chỉ cần chỉ ra rằng

$$
(P(T'') - \sum_i Q_i(T)R_i(T')).\mu = 0
$$

hoặc cũng $(P(T'') - P(T + T')).\mu = 0$ trong $B$-môđun $M$. Bây giờ, giả thiết rằng các $d_i$ là các đạo hàm cũng có thể được diễn đạt bằng cách nói rằng, với $1 \leq i \leq n$,

$$
(T_i'' - T_i - T_i').\mu = 0
$$

trong $B$-môđun $M$. Bằng cách xét lần lượt các đa thức

$P(T_1'', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2'', \ldots, T_n'')$
$P(T_1 + T_1', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2 + T_2', \ldots, T_n'')$
$\ldots$
$P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n'') - P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n + T_n')$

ta thấy rằng hiệu $P(T'') - P(T + T')$ có thể được viết dưới dạng

$$
\sum_{i=1}^n (T_i'' - T_i - T_i') G_i(T, T', T'')
$$

trong đó các $G_i$ là các phần tử của $B$. Do đó quan hệ (14) là một hệ quả ngay lập tức của các quan hệ (15).

#### Hệ quả (công thức Leibniz) {#alg-iii-s10-n4-cor-2 .statement}

*Cho $d_i$ ($1 \leq i \leq n$) là $n$ đạo hàm của $(A, A', A'')$ đôi một giao hoán với nhau. Với mọi $\alpha = (\alpha_1, \ldots, \alpha_n) \in \mathbf{N}^n$, ta viết*

$$
d^\alpha = d_1^{\alpha_1} d_2^{\alpha_2} \ldots d_n^{\alpha_n}.
$$

Khi đó, với $x \in \mathbf{A}$ và $y \in \mathbf{A}'$,

$$
d^\alpha(xy) = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) d^\beta(x)d^\gamma(y)
$$

trong đó ta đã viết (trong ký hiệu được đưa vào ở đầu chương)

$$
((\beta, \gamma)) = (\beta + \gamma)!/(\beta! \gamma!).
$$

Điều này suy ra ngay lập tức từ công thức đa thức (I, § 8, no. 2)

$$
(T + T')^\alpha = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) T^\beta {T'}^\gamma
$$

và Mệnh đề 2.

### 5. ĐẠO HÀM CỦA MỘT ĐẠI SỐ A VÀO MỘT A-MÔĐUN

Trong số này, ta giả sử rằng Trường hợp (II) của no. 2 đúng. Khi đó có một đại số K phân bậc A và một K-môđun phân bậc E, đồng thời có hai ánh xạ K-tuyến tính bậc 0

$$
E \otimes_K A \to E, \quad A \otimes_K E \to E
$$

được ký hiệu bởi

$$
x \otimes a \mapsto x.a \quad \text{và} \quad a \otimes x \mapsto a.x \quad \text{cho } a \in A \text{ và } x \in E.
$$

#### Mệnh đề 3 {#alg-iii-s10-prop-3 .statement}

Cho $d : A \to E$ là một $\varepsilon$-đạo hàm bậc $\delta$. Khi đó $\mathrm{Ker}(d)$ là một đại số con phân bậc của A; nếu A có phần tử đơn vị, thì nó thuộc $\mathrm{Ker}(d)$.

Rõ ràng $\mathrm{Ker}(d)$ là một K-môđun con phân bậc của A; hơn nữa, quan hệ (8) của no. 2 cho thấy rằng, nếu $x$ và $y$ là hai phần tử thuần nhất thuộc $\mathrm{Ker}(d)$, thì $d(xy) = 0$ và do đó $xy \in \mathrm{Ker}(d)$. Cuối cùng, nếu A có phần tử đơn vị 1 (của bậc 0, xem § 3, no. 1), thì quan hệ (8) của no. 2, khi thay $x$ và $y$ bởi 1, cho $d(1) = d(1) + d(1)$ và do đó $d(1) = 0$.

#### Hệ quả {#alg-iii-s10-n5-cor-1 .statement}

Cho $d_1$ và $d_2$ là hai $\varepsilon$-đạo hàm từ A đến E cùng bậc $\delta$. Nếu $d_1$ và $d_2$ nhận cùng giá trị tại mỗi phần tử của một hệ sinh của đại số A, thì $d_1 = d_2$.

$d_1 - d_2$ là một $\varepsilon$-đạo hàm bậc $\delta$, do đó $\mathrm{Ker}(d_1 - d_2)$ là một đại số con của A chứa một hệ sinh của A và vì thế bằng A.

#### Mệnh đề 4 {#alg-iii-s10-prop-4 .statement}

Cho $d : A \to E$ là một $\varepsilon$-đạo hàm bậc $\delta$. Giả sử A có phần tử đơn vị 1 và cho $x$ là một phần tử thuần nhất của A có nghịch đảo $x^{-1}$ trong A. Khi đó

$$
d(x^{-1}) = -\varepsilon_{\delta, \deg(x)} x^{-1}((dx)x^{-1}) = -\varepsilon_{\delta, \deg(x)} (x^{-1}(dx))x^{-1}.
$$

Ta có $d(xx^{-1}) = d(1) = 0$ (Mệnh đề 3), do đó
$$
(dx)x^{-1} + \varepsilon_{\delta, \deg(x)} x(d(x^{-1})) = 0
$$
điều này chứng minh công thức thứ nhất của (19). Mặt khác, $x^{-1}$ là thuần nhất bậc $-\deg(x)$ và $\varepsilon_{\delta, \deg(x)} = \varepsilon_{\delta, -\deg(x)}$ theo các công thức (1) của no. 1; viết $d(x^{-1}x) = 0$, ta thu được công thức thứ hai của (19) tương tự.

#### Mệnh đề 5 {#alg-iii-s10-prop-5 .statement}

*Giả sử $\mathbf{A}$ là một miền nguyên và đặt $\mathbf{L}$ là trường phân thức của nó. Mọi đạo hàm của $\mathbf{A}$ vào một không gian vectơ $\mathbf{E}$ trên $\mathbf{L}$ (xem như một $\mathbf{A}$-môđun) đều có thể được mở rộng duy nhất thành một đạo hàm của $\mathbf{L}$ vào $\mathbf{E}$.*

Gọi $d$ là một đạo hàm của $\mathbf{A}$ vào $\mathbf{E}$ và $\bar{d}$ là một đạo hàm của $\mathbf{L}$ vào $\mathbf{E}$ mở rộng $d$; khi đó, với $u \in \mathbf{A}, v \in \mathbf{A}, v \neq 0$, tất nhiên, nhờ (19),
$$
\bar{d}(u/v) = v^{-1}du - uv^{-2}dv
$$
điều này chứng tỏ tính duy nhất của $\bar{d}$. Ngược lại, ta chỉ ra rằng $\bar{d}$ có thể được xác định bởi công thức (20); trước hết cần kiểm tra rằng nếu $u/v = u'/v'$ thì giá trị của vế phải của (20) không thay đổi khi $u$ được thay bằng $u'$ và $v$ bằng $v'$. Bây giờ, $uv' = vu'$, do đó $v'(du) + u(dv') = v(du') + u'(dv)$ và vì thế $v'(du - uv^{-1}dv) = v(du' - u'{v'}^{-1}dv')$, vì $uv'v^{-1} = u'$ và $u'{v'}^{-1}v = u$. Vì vậy đã xác định được một ánh xạ $\bar{d}: \mathbf{L} \to \mathbf{E}$ mở rộng $d$; ngay lập tức kiểm tra được rằng nó là $\mathbf{K}$-tuyến tính và là một đạo hàm.

#### Mệnh đề 6 {#alg-iii-s10-prop-6 .statement}

*Giả sử $\mathbf{A}$ là một đại số phân bậc kết hợp có đơn vị $\mathbf{K}$ và $\mathbf{E}$ là một song môđun phân bậc $(\mathbf{A}, \mathbf{A})$. Nếu $d : \mathbf{A} \to \mathbf{E}$ là một $\varepsilon$-đạo hàm bậc $\delta$, thì, với mọi dãy hữu hạn $(x_i)_{1 \leq i \leq n}$ gồm các phần tử thuần nhất của $\mathbf{A}$, có các bậc tương ứng $\xi_i$ ($1 \leq i \leq n$),
$$
d(x_1 x_2 \ldots x_n) = \sum_{i=1}^n \varepsilon_{\delta, \xi_1 + \cdots + \xi_{i-1}} x_1 \cdots x_{i-1} (dx_i) x_{i+1} \cdots x_n.
$$
Công thức (21) là tầm thường khi $n = 0$ và được chứng minh bằng quy nạp theo $n$, có xét đến (4) (no. 2).

#### Hệ quả {#alg-iii-s10-n5-cor-2 .statement}

*Giả sử $\mathbf{A}$ là một đại số giao hoán kết hợp có đơn vị và $\mathbf{E}$ là một $\mathbf{A}$-môđun. Nếu $d : \mathbf{A} \to \mathbf{E}$ là một đạo hàm, thì, với mọi số nguyên $n \geq 0$,
$$
d(x^n) = nx^{n-1}(dx) \quad \text{với mọi } x \in \mathbf{A}.
$$
Chỉ cần cho $\mathbf{A}$ phân bậc tầm thường và áp dụng (21) với mọi $x_i$ đều bằng $x$.

Ta trở lại trường hợp tổng quát của một $\varepsilon$-đạo hàm $d : \mathbf{A} \to \mathbf{E}$ có bậc $\delta$. Kí hiệu $Z_\delta$ là tập hợp các $a \in \mathbf{A}$ sao cho với mọi thành phần thuần nhất $a_\alpha$ của $a$ có bậc $\alpha$, với mọi $x$ thuần nhất trong $\mathbf{E}$,
$$
xa_\alpha = \varepsilon_{\alpha, \deg(x)} a_\alpha x.
$$

Nếu $A$ là một đại số phân bậc kết hợp có đơn vị và $E$ là một $(A, A)$-song môđun phân bậc thì từ định nghĩa này suy ra ngay rằng $Z_\varepsilon$ là một *đại số con phân bậc* của $A$ chứa phần tử đơn vị.

#### Mệnh đề 7 {#alg-iii-s10-prop-7 .statement}

*Giả sử $A$ là một đại số phân bậc kết hợp có đơn vị và $E$ là một $(A, A)$-song môđun phân bậc. Cho $d : A \to E$ là một $\varepsilon$-đạo hàm có bậc $\delta$ và $a$ là một phần tử thuần nhất của $Z_\varepsilon$ có bậc $\alpha$. Khi đó ánh xạ $x \mapsto a(dx)$ là một $\varepsilon$-đạo hàm có bậc $\delta + \alpha$.*

Ta viết $d'(x) = a(dx)$; với $x$ thuần nhất có bậc $\xi$ trong $A$ và $y \in A$, nhờ (23) và (1) (no. 1),

$$
d'(xy) = a((dx)y) + \varepsilon_{\delta, \xi} a(x(dy)) = (a(dx))y + \varepsilon_{\delta+\alpha, \xi}(xa)(dy)
= (d'x)y + \varepsilon_{\delta+\alpha, \xi} x(d'y).
$$

Mệnh đề 7 nói rằng K-môđun các $\varepsilon$-đạo hàm của $A$ vào $E$ là một *môđun $Z_\varepsilon$ phân bậc* kiểu $\Delta$.

### 6. ĐẠO HÀM CỦA MỘT ĐẠI SỐ

Cho $A$ là một đại số K phân bậc; với mọi phần tử *thuần nhất* $a \in A$, kí hiệu $\mathrm{ad}_\varepsilon(a)$, hay đơn giản $\mathrm{ad}(a)$ nếu không thể có nhầm lẫn, ánh xạ K-tuyến tính của $A$ vào $A$

$$
x \mapsto [a, x]_\varepsilon
$$
(no. 4, công thức (10)) là *phân bậc có bậc* $\deg a$.

#### Mệnh đề 8 {#alg-iii-s10-prop-8 .statement}

*Cho $A$ là một đại số K phân bậc.*

(i) *Với mọi $\varepsilon$-đạo hàm $d : A \to A$ và mọi phần tử thuần nhất $a$ của $A$,*

$$(24)$$
$$
[d, \mathrm{ad}_\varepsilon(a)]_\varepsilon = \mathrm{ad}_\varepsilon(da).
$$

(ii) *Nếu đại số $A$ là kết hợp, thì $\mathrm{ad}_\varepsilon(a)$ là một $\varepsilon$-đạo hàm của $A$ có bậc $\deg(a)$. \*

(i) Giả sử $d$ có bậc $\delta$, đặt $\alpha = \deg a$ và viết $f = [d, \mathrm{ad}_\varepsilon(a)]_\varepsilon$. Với mọi phần tử thuần nhất $x \in A$ có bậc $\xi$, ta có, theo (1) (mục 1),

$$
f(x) = d(ax - \varepsilon(\alpha, \xi) xa) - \varepsilon_{\delta, \alpha}(a(dx)) - \varepsilon_{\alpha, \delta+\xi}(dx)a \\
= (da)x + \varepsilon_{\delta, \alpha} a(dx) - \varepsilon_{\alpha, \xi}(dx)a - \varepsilon_{\delta+\alpha, \xi} x(da) \\
- \varepsilon_{\delta, \alpha} a(dx) + \varepsilon_{\alpha, \xi}(dx)a \\
= (da)x - \varepsilon_{\delta+\alpha, \xi} x(da) = [da, x]_\varepsilon.
$$

(ii) Với mọi $x$ thuần nhất có bậc $\xi$ và mọi $y$ thuần nhất có bậc $\eta$ trong $A$,

$$
\mathrm{ad}_\varepsilon(a)(xy) = a(xy) - \varepsilon_{\alpha, \xi+\eta}(xy)a \\
= (ax - \varepsilon_{\alpha, \xi} xa)y + \varepsilon_{\alpha, \xi} x(ay - \varepsilon_{\alpha, \eta} ya) \\
= \mathrm{ad}_\varepsilon(a)(x).y + \varepsilon_{\alpha, \xi} x.\mathrm{ad}_\varepsilon(a)(y)
$$
xét đến (1) và tính kết hợp của $A$.

Khi $A$ là kết hợp, $\mathrm{ad}_\varepsilon(a)$ được gọi là *$\varepsilon$-đạo hàm nội* của $A$ xác định bởi $a$.

#### Hệ quả {#alg-iii-s10-n6-cor-1 .statement}

*Cho $A$ là một đại số phân bậc kết hợp. Với hai phần tử thuần nhất $a, b$ của $A$,*
$$
[\mathrm{ad}_\varepsilon(a), \mathrm{ad}_\varepsilon(b)]_\varepsilon = \mathrm{ad}_\varepsilon([a, b]_\varepsilon).
$$
(25)

Chỉ cần thay $d$ bởi $\mathrm{ad}_\varepsilon(a)$ và $\mathrm{ad}_\varepsilon(a)$ bởi $\mathrm{ad}_\varepsilon(b)$ trong (24).

Nếu $\deg a = \alpha, \deg b = \beta$, công thức (25) tương đương với quan hệ sau đây đối với mọi phần tử thuần nhất $c \in A$ có bậc $\gamma$
$$
\varepsilon_{\alpha, \gamma}[a, [b, c]_\varepsilon]_\varepsilon + \varepsilon_{\beta, \alpha}[b, [c, a]_\varepsilon]_\varepsilon + \varepsilon_{\gamma, \beta}[c, [a, b]_\varepsilon]_\varepsilon = 0
$$
được gọi là *đẳng thức Jacobi*.

### 7. Tính chất hàm tử

*Trong mục này, mọi đại số đều được giả thiết là kết hợp và có đơn vị và mọi đồng cấu đại số đều được giả thiết là có đơn vị.*

#### Mệnh đề 9 {#alg-iii-s10-prop-9 .statement}

*Cho $A, B$ là hai $K$-đại số phân bậc, $E$ là một $(A, A)$-song môđun và $F$ là một $(B, B)$-song môđun phân bậc; cho $\rho : A \to B$ là một đồng cấu đại số phân bậc và $\theta : E \to F$ là một đồng cấu $A$-môđun của $A$-song môđun phân bậc (tương đối với $\rho$), có bậc 0. Khi đó:*

*(i)* *Với mọi $\varepsilon$-đạo hàm $d' : B \to F$, $d' \circ \rho : A \to \rho^*(F)$ là một $\varepsilon$-đạo hàm cùng bậc.*
*(ii)* *Với mọi $\varepsilon$-đạo hàm $d : A \to E$, $\theta \circ d : A \to \rho^*(F)$ là một $\varepsilon$-đạo hàm cùng bậc.*

Hai khẳng định này suy ra ngay lập tức từ các hệ thức
$$
d'(\rho(xy)) = d'(\rho(x)\rho(y)) = d'(\rho(x))\rho(y) + \varepsilon_{\delta', \xi}\rho(x)d'(\rho(y))
$$
$$
\theta(d(xy)) = \theta((dx)y + \varepsilon_{\delta, \xi}x(dy)) = \theta(dx)\rho(y) + \varepsilon_{\delta, \xi}\rho(x)\theta(dy)
$$
với $x \in A$ thuần nhất bậc $\xi$ và $y \in A$, $\delta$ và $\delta'$ ký hiệu các bậc tương ứng của $d$ và $d'$.

#### Hệ quả {#alg-iii-s10-n7-cor-1 .statement}

*Cho $S$ là một hệ sinh của đại số $A$. Để $d' \circ \rho = \theta \circ d$, điều kiện cần và đủ là $d'(\rho(x)) = \theta(d(x))$ với mọi $x \in S$. \*

Đây là một hệ quả ngay lập tức của Mệnh đề 9 và no. 5, Hệ quả của Mệnh đề 3.

Dưới các điều kiện của Mệnh đề 9, ta biết rằng $B$ có (qua $\rho$) một cấu trúc song môđun $(A, A)$ (II, § 1, no. 14, *Ví dụ 1*).

#### Mệnh đề 10 {#alg-iii-s10-prop-10 .statement}

*Dưới các điều kiện của Mệnh đề 9, để một $\varepsilon$-đạo hàm $d' : B \to F$ là $A$-tuyến tính đối với các cấu trúc $A$-môđun trái (tương ứng phải) trên $B$ và $\rho^*(F)$, điều kiện cần và đủ là $d'$ bằng không trên đại số con $\rho(A)$ của $B$. \*

Chúng ta chứng minh cho các cấu trúc A-môđun trái. Với $a \in A, b \in B$,
$$
d'(\rho(a)b) = d'(\rho(a))b + \rho(a)d'b
$$
và do đó nếu $d' \circ \rho = 0$, thì $d'$ là tuyến tính đối với các cấu trúc A-môđun trái trên B và $\rho^*(F)$. Ngược lại, nếu điều này đúng, thì đặc biệt
$$
d'(\rho(a)) = d'(\rho(a).1) = \rho(a)d'(1) = 0
$$
(no. 5, Mệnh đề 3).

Đặc biệt, ký hiệu $D_K(B, F)$ là K-môđun các đạo hàm của B vào F (no. 2); những đạo hàm trong đó là A-tuyến tính, nói cách khác những đạo hàm triệt tiêu trên $\rho(A)$, tạo thành một K-môđun con của $D_K(B, F)$, ký hiệu là $D_{A,\rho}(B, F)$ hay đơn giản là $D_A(B, F)$ (hiển nhiên $D_K(B, F) = D_{K,\phi}(B, F)$, trong đó $\phi : K \to B$ là đồng cấu xác định cấu trúc đại số trên K của B).

Bây giờ cho A, B, C là ba đại số trên K phân bậc, $\rho : A \to B, \sigma : B \to C$ là hai đồng cấu đại số phân bậc và G là một song môđun phân bậc $(C, C)$; nếu $D_A(B, G)$, $D_B(C, G)$ và $D_A(C, G)$ lần lượt ký hiệu các K-môđun $D_{A,\rho}(B, \sigma_*(G))$, $D_{B,\sigma}(C, G)$ và $D_{A,\sigma \circ \rho}(C, G)$, thì $D_B(C, G)$ rõ ràng là một K-môđun con của $D_A(C, G)$ vì $\sigma(\rho(A)) \subset \sigma(B)$.

#### Mệnh đề 11 {#alg-iii-s10-prop-11 .statement}

*Dưới các điều kiện trên, tồn tại một dãy khớp các K-đồng cấu*
$$
0 \to D_B(C, G) \xrightarrow{u} D_A(C, G) \xrightarrow{v} D_A(B, G)
$$
*trong đó u là đơn ánh chính tắc và v là đồng cấu $d \mapsto d \circ \sigma$* (Mệnh đề 9).

==========

### 8. QUAN HỆ GIỮA CÁC ĐẠO HÀM VÀ CÁC ĐỒNG CẤU ĐẠI SỐ

Ta lại giả sử trong mục này rằng *Trường hợp (II)* của no. 2 đúng và đại số trên K phân bậc A không được giả thiết là kết hợp. Cho một phần tử $\delta \in \Delta$, xét K-môđun phân bậc E($\delta$) (II, § 11, no. 2) sao cho
$$
(E(\delta))_\mu = E_{\mu+\delta}
$$
với mọi $\mu \in \Delta$. Ta định nghĩa trên K-môđun phân bậc $A \oplus E(\delta)$ một *cấu trúc đại số trên K phân bậc* bằng cách đặt, với mọi phần tử thuần nhất $a \in A$ và các phần tử tùy ý $a' \in A, x, x'$ trong $E(\delta)$
$$
(a, x)(a', x') = (aa', x.a' + \varepsilon_{\delta, \deg(a)} a.x');
$$
việc kiểm tra rằng phép nhân này xác định một cấu trúc vành phân bậc là ngay lập tức.

Phép chiếu $p : (a, x) \mapsto a$ được gọi là phép tăng cường của đại số $A \oplus E(\delta)$ và là một đồng cấu đại số phân bậc. Các ánh xạ K-tuyến tính phân bậc $g : A \to A \oplus E(\delta)$ có bậc 0 sao cho hợp thành

$$
A \xrightarrow{g} A \oplus E(\delta) \xrightarrow{p} A
$$

là đồng nhất $1_A$ chính là các ánh xạ có dạng $x \mapsto (x, f(x))$, trong đó $f : A \to E$ là một ánh xạ K-tuyến tính phân bậc bậc $\delta$.

#### Mệnh đề 12 {#alg-iii-s10-prop-12 .statement}

*Để một ánh xạ K-tuyến tính $f : A \to E$ bậc $\delta$ là một $\varepsilon$-đạo hàm, cần và đủ là ánh xạ $x \mapsto (x, f(x))$ của A vào $A \oplus E(\delta)$ là một đồng cấu đại số trên K phân bậc.*

Dùng thực tế rằng với $x$ thuần nhất trong A và $y \in A$

$$
(xy, f(xy)) = (x, f(x)).(y, f(y)),
$$

ta được, xét đến (28), quan hệ tương đương

$$
f(xy) = f(x).y + \varepsilon_{\delta, \deg(x)} x.f(y),
$$

do đó mệnh đề.

#### Mệnh đề 13 {#alg-iii-s10-prop-13 .statement}

*Để đại số $A \oplus E(\delta)$ kết hợp và có đơn vị, cần và đủ là A kết hợp và có đơn vị, và các ánh xạ $(a, x) \mapsto a.x$ và $(a, x) \mapsto x.a$ định nghĩa trên $E$ một cấu trúc song môđun $(A, A)$; khi đó phần tử đơn vị của $A \oplus E(\delta)$ là $(1, 0)$.*

Nếu một phần tử $(u, m) \in A \oplus E(\delta)$ được viết như là phần tử đơn vị của đại số này, thì ngay lập tức thấy rằng $u$ phải là phần tử đơn vị của A; viết $(u, m).(0, x) = (0, x).(u, m) = (0, x)$, ta được $u.x = x.u = x$ với $x \in E$ và, viết $(u, m).(u, 0) = (u, 0).(u, m) = (u, 0)$, ta được $m = 0$. Việc A kết hợp khi $A \oplus E(\delta)$ kết hợp suy ra từ thực tế rằng phép tăng cường là một đồng cấu toàn ánh. Điều kiện $(x.a').a'' = x.(a'.a'')$ khi đó tương đương với $((0, x)(a', 0))(a'', 0) = (0, x)((a', 0)(a'', 0))$ và tương tự điều kiện $a.(a'.x) = (a.a').x$ tương đương với

$$
(a, 0)((a', 0)(0, x)) = ((a, 0)(a', 0))(0, x);
$$

cuối cùng điều kiện $a.(x.a') = (a.x).a'$ tương đương với

$$
(a, 0)((0, x)(a', 0)) = ((a, 0)(0, x))(a', 0).
$$

### 9. MỞ RỘNG CÁC ĐẠO HÀM

#### Mệnh đề 14 {#alg-iii-s10-prop-14 .statement}

*Cho $A$ là một vành giao hoán, $M$ là một $A$-môđun, $B$ là $A$-đại số $T(M)$ (tương ứng $S(M)$, tương ứng $\Lambda(M)$) và $E$ là một $(B, B)$-song môđun. Cho $d_0 : A \to E$ là một đạo hàm của vành $\mathbf{A}$ vào $\mathbf{A}$-môđun $\mathbf{E}$ và $d_1 : M \to \mathbf{E}$ là một đồng cấu nhóm cộng sao cho, với mọi $a \in \mathbf{A}$ và mọi $x \in M$,*

$$
(29) \quad d_1(ax) = ad_1(x) + d_0(a) \cdot x,
$$

*và thêm nữa, khi $B = S(M)$,*

$$
(30) \quad x \cdot d_1(y) + d_1(x) \cdot y = y \cdot d_1(x) + d_1(y) \cdot x
$$

*với mọi $x, y$ trong $M$, và, khi $B = \bigwedge(M)$,*

$$
(31) \quad x \cdot d_1(x) + d_1(x) \cdot x = 0
$$

*với mọi $x \in M$. Khi đó tồn tại một và chỉ một đạo hàm $d$ của $B$ (xét như một $\mathbf{Z}$-đại số) vào song môđun $(B, B)$ $\mathbf{E}$ sao cho $d|_{\mathbf{A}} = d_0$ và $d|_{M} = d_1$.*

Trên $\mathbf{Z}$-môđun $B \oplus \mathbf{E}$ ta đặt cấu trúc $\mathbf{Z}$-đại số kết hợp được xác định bởi

$$
(b, t)(b', t') = (bb', bt' + tb')
$$

which has $(1, 0)$ as unit element (no. 8, Mệnh đề 13). Qua đơn ánh chính tắc $t \mapsto (0, t)$, $\mathbf{E}$ được đồng nhất với một iđêan hai phía của $B \oplus \mathbf{E}$ sao cho $\mathbf{E}^2 = \{0\}$. Mặt khác, ánh xạ $h_0 : B \oplus \mathbf{E}$ được định nghĩa bởi $h_0(a) = (a, d_0(a))$ là một đồng cấu vành có đơn vị (no. 8, Mệnh đề 12); dưới ánh xạ này, $B \oplus \mathbf{E}$ khi đó trở thành một $\mathbf{A}$-đại số. Hơn nữa, nếu, với mọi $x \in M$, ta viết $h_1(x) = (x, d_1(x))$, thì từ định nghĩa của $h_0$ và (29) suy ra $h_1(ax) = h_0(a)h_1(x)$; nói cách khác $h_1$ là một ánh xạ tuyến tính $\mathbf{A}$ của $M$ vào $B \oplus \mathbf{E}$. Khi đó tồn tại một và chỉ một đồng cấu đại số $\mathbf{A}$, $h : B \to B \oplus \mathbf{E}$ sao cho $h|_M = h_1$ (và tất nhiên $h|_{\mathbf{A}} = h_0$): vì, nếu $B = T(M)$, điều này suy ra từ $\S 5$, no. 1, Mệnh đề 1; nếu $B = S(M)$, điều kiện (30) cho thấy rằng $h(x)h(y) = h(y)h(x)$ với mọi $x, y$ trong $M$ và kết luận suy ra từ $\S 6$, no. 1, Mệnh đề 2; cuối cùng nếu $B = \bigwedge(M)$, điều kiện (31) cho thấy rằng $(h(x))^2 = 0$ với mọi $x \in M$, vì $x \wedge x = 0$ và kết luận suy ra từ $\S 7$, no. 1, Mệnh đề 1. Đồng cấu $h$ có tính chất rằng phép hợp thành $p \circ h : B \to B$ với phép tăng cường $\rho : B \oplus \mathbf{E} \to B$ là đồng nhất $l_B$, vì $p \circ h$ và $l_B$ trùng nhau theo định nghĩa trên các phần tử của $\mathbf{A}$ và các phần tử của $M$ và tập hợp các phần tử ấy là một hệ sinh của $B$. Do đó ta có thể viết $h(b) = (b, d(b))$ với mọi $b \in B$ và ánh xạ $b \mapsto d(b)$ của $B$ vào $\mathbf{E}$ là một đạo hàm có các tính chất yêu cầu, theo Mệnh đề 12 của no. 8.

#### Hệ quả {#alg-iii-s10-n9-cor-1 .statement}

*Cho $M$ là một $K$-môđun phân bậc kiểu $\Delta$; các $K$-đại số $T(M)$, $S(M)$ và $\bigwedge(M)$ được cho các cách phân bậc tương ứng kiểu $\Delta' = \Delta \times \mathbf{Z}$ ($\S 5$, no. 5, Mệnh đề 7, $\S 6$, no. 6, Mệnh đề 10 và $\S 7$, no. 7, Mệnh đề 11). Mặt khác $M$ được cho cách phân bậc kiểu $\Delta'$ sao cho $M_{\alpha, 1} = M_{\alpha}$ với mọi $\alpha \in \Delta$ và $M_{\alpha, n} = \{0\}$ với $\alpha \in \Delta$ và $n \neq 1$. Cho $\varepsilon'$ là một hệ số giao hoán trên $\Delta'$.*

(i) Cho E là một $\mathbf{T}(M)$-song môđun phân bậc (trái và phải) kiểu $\Delta'$; với mọi $\delta \in \Delta$ và mọi số nguyên $n \in \mathbf{Z}$, mọi ánh xạ K-tuyến tính phân bậc $f : M \to E$ có bậc $\delta_1' = (\delta, n)$ đều có thể được mở rộng duy nhất thành một $\varepsilon'$-đạo hàm $d : \mathbf{T}(M) \to E$ có bậc $\delta'$.

(ii) Cho E là một môđun phân bậc $S(M)$ kiểu $\Delta'$; để một ánh xạ K-tuyến tính phân bậc $f : M \to E$ có bậc $\delta'$ có thể được mở rộng thành một $\varepsilon'$-đạo hàm $d : S(M) \to E$ có bậc $\delta'$, điều kiện cần và đủ là, với mọi cặp có thứ tự $(x, y)$ của các phần tử thuần nhất của M,

$$
x . f(y) + \varepsilon_{\delta', (\deg(y), 1)} y . f(x) = y . f(x) + \varepsilon_{\delta', (\deg(x), 1)} x . f(y).
$$

Khi đó, $\varepsilon'$-đạo hàm d là duy nhất.

(iii) Cho E là một $\Lambda(M)$-song môđun phân bậc (trái và phải) kiểu $\Delta'$; với một ánh xạ K-tuyến tính phân bậc $f : M \to E$ có bậc $\delta'$ có thể được mở rộng thành một $\varepsilon'$-đạo hàm

$$
d : \Lambda(M) \to E
$$

có bậc $\delta'$, điều kiện cần và đủ là, với mọi phần tử thuần nhất x của M,

$$
x . f(x) + \varepsilon_{\delta', (\deg(x), 1)} f(x) . x = 0.
$$

Khi đó, $\varepsilon'$-đạo hàm d là duy nhất.

Nhận xét 2 của no. 2 được áp dụng với một trong các luật môđun ngoài B trên E (với B bằng $\mathbf{T}(M)$, $S(M)$ hoặc $\Lambda(M)$) được sửa đổi; luật ngoài đã sửa đổi như vậy vẫn, theo (1) (no. 1), là một luật môđun B và luật môđun B thu được trên E vẫn tương thích với cấu trúc môđun B còn lại. Khi đó chỉ cần áp dụng Mệnh đề 14 với $A = K$ và $d_0 = 0$.

Example (1). Trong việc áp dụng Mệnh đề 14 hãy chú ý rằng nếu $d_0 = 0$ thì điều kiện (29) chỉ có nghĩa đơn giản là $d_1$ là A-tuyến tính. Nếu ta lấy riêng $E = B$ và cấu trúc song môđun (B, B) dẫn xuất từ cấu trúc vành trên B, thì các điều kiện (30) và (31) tự động được thỏa mãn khi $d_1$ được lấy là hợp thành của một tự đồng cấu s của M và đơn ánh chính tắc $M \to B$; điều này hiển nhiên đối với (30) vì $S(M)$ là giao hoán và đối với (31) điều này suy ra từ sự kiện rằng x và $s(x)$ có bậc 1 trong $\Lambda(M)$. Do đó thấy rằng mọi tự đồng cấu s của M đều có thể được mở rộng duy nhất thành một đạo hàm $D_s$ của $\mathbf{T}(M)$ (resp. $S(M)$, resp. $\Lambda(M)$), có bậc 0. Hơn nữa, với hai tự đồng cấu s, t của M,

$$
[D_s, D_t] = D_{[s, t]}
$$

vì cả hai vế đều là các đạo hàm của $\mathbf{T}(M)$ (resp. $S(M)$, resp. $\Lambda(M)$) và đều bằng $[s, t]$ trên M.

Biểu thức của $D_s$ thu được bằng cách dùng công thức (21) của no. 5, công thức này cho lần lượt, với $x_1, x_2, \ldots, x_n$ trong $M$,

$$
\begin{cases}
D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n) \\
\phantom{D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n)} = \sum_{i=1}^n x_1 \otimes \cdots \otimes x_{i-1} \otimes s(x_i) \otimes x_{i+1} \otimes \cdots \otimes x_n \\
D_s(x_1 x_2 \ldots x_n) = \sum_{i=1}^n x_1 \ldots x_{i-1} s(x_i) x_{i+1} \ldots x_n \\
D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \\
\phantom{D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n)} = \sum_{i=1}^n x_1 \wedge \cdots \wedge x_{i-1} \wedge s(x_i) \wedge x_{i+1} \wedge \cdots \wedge x_n.
\end{cases}
$$

Trong trường hợp của đại số $\Lambda(M)$, có sự diễn giải sau của $D_s$:

#### Mệnh đề 15 {#alg-iii-s10-prop-15 .statement}

*Nếu $M$ là một $K$-môđun tự do có hạng hữu hạn $n$, thì, với mọi tự đồng cấu $s$ của $M$, hạn chế lên $\Lambda^n(M)$ của đạo hàm $D_s$ là phép vị tự có tỉ số $\operatorname{Tr}(s)$. \*

Cho $(e_j)_{1 \leq j \leq n}$ là một cơ sở của $M$ và viết $e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$. Nếu
$$
s(e_j) = \sum_{k=1}^n \alpha_{jk} e_k,
$$
công thức thứ ba trong (36) cho
$$
D_s(e) = \sum_{i=1}^n e_1 \wedge \cdots \wedge e_{i-1} \wedge s(e_i) \wedge e_{i+1} \wedge \cdots \wedge e_n = \left( \sum_{j=1}^n \alpha_{jj} \right) e.
$$

*Ví dụ (2).* Trong Hệ quả của Mệnh đề 14, phần (iii), lấy $\Delta = \{0\}$, khi đó phân bậc trên $\Lambda(M)$ là phân bậc thông thường kiểu $\mathbf{Z}$; mặt khác lấy $\varepsilon(p, q) = (-1)^{pq}$. Khi đó, với mọi dạng tuyến tính $x^* \in M^*$ trên $M$, $x \mapsto \langle x, x^* \rangle$ là một ánh xạ $K$-tuyến tính phân bậc có bậc $-1$ từ $M$ vào $\Lambda(M)$ thỏa mãn quan hệ (34); khi đó tồn tại một *phản đạo hàm* $i(x^*)$ của $\Lambda(M)$, có bậc $-1$, sao cho (theo công thức (21) của no. 5)
$$
i(x^*)(x_1 \wedge \cdots \wedge x_n)
= \sum_{i=1}^n (-1)^{i-1} \langle x_i, x^* \rangle x_1 \wedge \cdots \wedge x_{i-1} \wedge x_{i+1} \wedge \cdots \wedge x_n
$$
và đây là một trường hợp riêng của tích nội sẽ được định nghĩa ở § 11, no. 9, công thức (68).

#### Mệnh đề 16 {#alg-iii-s10-prop-16 .statement}

*Cho $A$ là một $K$-đại số giao hoán, $M_i$ ($1 \leq i \leq n$) và $P$ là các $A$-môđun và $H$ là $A$-môđun của các ánh xạ $A$-đa tuyến tính từ $M_1 \times M_2 \times \cdots \times M_n$* vào P. Giả sử rằng đã cho một $K$-đạo hàm $d_0 : A \to A$ của đại số A, với mỗi i, một ánh xạ $K$-tuyến tính $d_i : M_i \to M_i$ và một ánh xạ $K$-tuyến tính $D : P \to P$, sao cho, với $1 \leq i \leq n$, $(d_0, d_i, d_i)$ là một $K$-đạo hàm của $(A, M_i, M_i)$ vào chính nó và $(d_0, D, D)$ là một $K$-đạo hàm của $(A, P, P)$ vào chính nó. Khi đó tồn tại một ánh xạ $K$-tuyến tính $D' : H \to H$ sao cho $(d_0, D', D')$ là một $K$-đạo hàm của $(A, H, H)$ vào chính nó và

(37) $D(f(x_1, \ldots, x_n))$

$$
= (D'f)(x_1, \ldots, x_n) + \sum_{i=1}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$

với mọi $x_i \in M_i$ với $1 \leq i \leq n$ và $f \in H$.

Ta chứng minh rằng với $f \in H$, ánh xạ $D'f$ của $M_1 \times M_2 \times \cdots \times M_n$ vào P được xác định bởi (37) là A-đa tuyến tính. Với $a \in A$,

$$
(D'f)(ax_1, x_2, \ldots, x_n) = D(af(x_1, \ldots, x_n)) - f(d_1(ax_1), x_2, \ldots, x_n)
$$
$$
-a \sum_{i=2}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$

và theo giả thiết

$$
D(af(x_1, \ldots, x_n)) = (d_0a)f(x_1, \ldots, x_n) + aD(f(x_1, \ldots, x_n))
$$

và $d_1(ax_1) = (d_0a)x_1 + a.d_1x_1$, điều này cho

$$
(D'f)(ax_1, x_2, \ldots, x_n) = a.(D'f)(x_1, \ldots, x_n)
$$

và tính tuyến tính theo từng $x_i$ được chứng minh tương tự. Mặt khác,

$$
(D'(af))(x_1, \ldots, x_n) = D(af(x_1, \ldots, x_n))
$$
$$
- \sum_{i=1}^n af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n)) + aD(f(x_1, \ldots, x_n))
$$
$$
- \sum_{i=1}^n af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n) + a(D'f)(x_1, \ldots, x_n)
$$

nói cách khác

$$
D'(af) = (d_0a)f + a(D'f)
$$

điều đó chứng minh mệnh đề.

#### Ví dụ {#alg-iii-s10-n9-exa-1 .statement}

(3) Áp dụng Mệnh đề 16 cho trường hợp $n = 1$, $M_1 = M$, $P = A$, thì $H = M^*$, là đối ngẫu của M, và thấy rằng đối với một $K$-đạo hàm $(d_0, d, d')$ của $(A, M, M)$ suy ra một $K$-đạo hàm $(d_0, d^*, d^*)$ của $(A, M^*, M^*)$ sao cho

(38) $d_0\langle m, m^*\rangle = \langle dm, m^*\rangle + \langle m, d^*m^*\rangle$

cho $m \in M$ và $m^* \in M^*$. Ánh xạ K-tuyến tính của $M \oplus M^*$ vào chính nó mà bằng $d$ trên $M$ và bằng $d^*$ trên $M^*$ khi đó thỏa mãn điều kiện (29) và do đó tồn tại một $K$-đạo hàm $D$ của $A$-đại số $T(M \oplus M^*)$, mà trên $A$ là $d_0$, trên $M$ là $d$ và trên $M^*$ là $d^*$. Hạn chế $d_J^I$ của $D$ lên môđun con $A$ $T_J^I(M)$ của $T(M \oplus M^*)$ ($\S 5$, no. 6) là một $K$-tự đồng cấu của $T_J^I(M)$ sao cho $(d_0, d_J^I, d_J^I)$ là một $K$-đạo hàm của $(A, T_J^I(M), T_J^I(M))$. Hơn nữa, với $i \in I, j \in J$, nếu đặt $I' = I - \{i\}, J' = J - \{j\}$, thì ngay lập tức kiểm tra được rằng đối với phép co $c_j^i$ ($\S 5$, no. 6)

$$
c_j^i(d_J^I(z)) = d_{J'}^{I'}(c_j^i(z)) \quad \text{với mọi } z \in T_J^I(M).
$$

(4) Cho $M_i$ ($1 \leq i \leq 3$) là ba $A$-môđun và, với mỗi $i$, giả sử rằng $(d_0, d_i, d_i)$ là một đạo hàm của $(A, M_i, M_i)$; áp dụng lại Mệnh đề 16 với $n = 1$, một đạo hàm $(d_0, d_{ij}, d_{ij})$ của $(A, H_{ij}, H_{ij})$, trong đó $H_{ij} = \operatorname{Hom}_A(M_i, M_j)$, được suy ra cho mỗi cặp có thứ tự $(i, j)$. Với ký hiệu này, đối với $u \in \operatorname{Hom}_A(M_1, M_2)$ và $v \in \operatorname{Hom}_A(M_2, M_3)$,

$$
d_{13}(v \circ u) = (d_{23}v) \circ u + v \circ (d_{12}u)
$$
như dễ dàng kiểm tra từ các định nghĩa.

### 10. BÀI TOÁN PHỔ QUÁT CHO CÁC ĐẠO HÀM; TRƯỜNG HỢP KHÔNG GIAO HOÁN

Trong phần còn lại của $\S 10$ mọi đại số đều được giả sử là kết hợp và có đơn vị và mọi đồng cấu đại số đều được giả sử là có đơn vị.

Cho $A$ là một $K$-đại số; tích tenxơ $A \otimes_K A$ có một cấu trúc song môđun $(A, A)$ một cách chính tắc dưới đó

$$
x . (u \otimes v) . y = (xu) \otimes (vy)
$$
với mọi $x, y, u, v$ trong $A$ ($\S 4$, no. 3, Ví dụ 2). Ánh xạ $K$-tuyến tính $m : A \otimes_K A \to A$ tương ứng với phép nhân trong $A$ (và do đó sao cho $m(x \otimes y) = xy$) là một đồng cấu $(A, A)$-song môđun; hạt nhân của nó $I$ do đó là một môđun con song của $A \otimes_K A$.

#### Bổ đề 1 {#alg-iii-s10-lem-1 .statement}

*Ánh xạ $\delta_A : x \mapsto x \otimes 1 - 1 \otimes x$ là một $K$-đạo hàm của $A$ vào $I$ và $I$ được sinh, với tư cách là một môđun trái $A$, bởi ảnh của $\delta_A$.*

Mệnh đề thứ nhất suy ra từ đẳng thức

$$
(xy) \otimes 1 - 1 \otimes (xy) = (x \otimes 1 - 1 \otimes x) . y + x . (y \otimes 1 - 1 \otimes y)
$$
theo (40). Mặt khác, nếu phần tử $\sum_i x_i \otimes y_i$ (với $x_i, y_i$ trong $A$) thuộc $I$, thì theo định nghĩa $\sum_i x_i y_i = 0$ và do đó

$$
\sum_i (x_i \otimes y_i) = \sum_i x_i (1 \otimes y_i - y_i \otimes 1)
$$
theo (40), điều này hoàn tất chứng minh của bổ đề.

#### Mệnh đề 17 {#alg-iii-s10-prop-17 .statement}

*Đạo hàm* $\delta_A$ *có tính chất phổ quát sau*: với mọi $(A, A)$-song môđun $E$ và mọi $K$-đạo hàm $d : A \to E$, tồn tại một và chỉ một đồng cấu $(A, A)$-song môđun $f : I \to E$ sao cho $d = f \circ \delta_A$.

Trước hết lưu ý rằng, với mọi đồng cấu $(A, A)$-song môđun $f : I \to E$, $f \circ \delta_A$ là một đạo hàm (no. 7, Mệnh đề 9). Ngược lại, cho $d : A \to E$ là một $K$-đạo hàm; khi đó trước hết ta chứng minh rằng nếu tồn tại một đồng cấu $(A, A)$-song môđun $f : I \to E$ sao cho $d = f \circ \delta_A$, thì $f$ được *xác định duy nhất* bởi điều kiện này vì định nghĩa của $\delta_A$ cho ta

$$
f(x \otimes 1 - 1 \otimes x) = dx
$$

và mệnh đề của chúng ta suy ra từ việc ảnh của $\delta_A$ đã sinh ra $I$ như một môđun trái $A$ (Bổ đề 1): do đó tất yếu

$$
f\left( \sum_i x_i \otimes y_i \right) = \sum_i x_i \cdot f(1 \otimes y_i - y_i \otimes 1) = -\sum_i x_i \cdot dy_i.
$$

Ngược lại, vì ánh xạ $(x, y) \mapsto -x \cdot dy$ của $A \times A$ vào $E$ là $K$-song tuyến tính, nên tồn tại một và chỉ một ánh xạ $K$-tuyến tính $g : A \otimes_K A \to E$ sao cho $g(x \otimes y) = -x \cdot dy$; chỉ cần kiểm tra rằng hạn chế $f$ của $g$ lên $I$ là $A$-tuyến tính đối với cấu trúc môđun trái và phải trên $A$. Mệnh đề thứ nhất hiển nhiên vì $(xx') \cdot dy = x \cdot (x' \cdot dy)$; để chứng minh mệnh đề thứ hai, hãy lưu ý rằng, nếu $\sum_i x_i \otimes y_i \in I$ và $x \in A$, thì

$$
\sum_i x_i \cdot d(y_i x) = \sum_i x_i \cdot dy_i \cdot x + \sum_i (x_i y_i) \cdot dx
$$

nhưng vì $\sum_i x_i y_i = 0$ theo định nghĩa của $I$, điều này hoàn tất chứng minh.

Do đó ta đã định nghĩa một đẳng cấu $K$-môđun chính tắc $f \mapsto f \circ \delta_A$

$$
\operatorname{Hom}_{(A, A)}(I, E) \to D_K(A, E)
$$

vế trái là môđun $K$ của các đồng cấu song môđun $(A, A)$ từ $A$ vào $E$.

### 11. BÀI TOÁN PHỔ QUÁT VỀ CÁC PHÉP ĐẠO HÀM; TRƯỜNG HỢP GIAO HOÁN

Giả sử bây giờ $A$ là một đại số giao hoán trên $K$ và $E$ là một $A$-môđun; $E$ có thể được xét như một song môđun $(A, A)$ mà hai luật ngoài của nó trùng với luật $A$-môđun đã cho. Mặt khác cấu trúc song môđun $(A, A)$ trên $A \otimes_K A$ trùng với cấu trúc $(A \otimes_K A)$-môđun của nó xuất phát từ cấu trúc *vành giao hoán* trên $A \otimes_K A$, vì trong trường hợp này, với $x, y, u, v$ trong $A$,

$$
x \cdot (u \otimes v) \cdot y = (xu) \otimes (vy) = (xu) \otimes (yv) = (x \otimes y)(u \otimes v).
$$

Hạt nhân $\mathfrak{J}$ của $m$ do đó trong trường hợp này là một *iđêan* của vành $A \otimes_K A$ và, vì $m : A \otimes_K A \to A$ là toàn ánh, $(A \otimes_K A)/\mathfrak{J}$ đẳng cấu với $A$; nếu $E$ cũng được xét như một $(A \otimes_K A)$-môđun bởi $m$ (nói cách khác môđun $(A \otimes_K A)$-môđun $m_*(E)$), thì các đồng cấu *song môđun* $(A, A)$ $\mathfrak{J} \to E$ được đồng nhất với các đồng cấu *môđun* $(A \otimes_K A)$ $\mathfrak{J} \to E$ (\S 4, no. 3), nói cách khác có một đẳng cấu $K$-môđun chính tắc.

$$
\operatorname{Hom}_{(A, A)}(\mathfrak{J}, E) \to \operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E).
$$

Mặt khác, $\mathfrak{J}E = \{0\}$, vì các phần tử $1 \otimes x - x \otimes 1$ sinh ra $\mathfrak{J}$ như một $(A \otimes_K A)$-môđun (no. 10, Bổ đề 1) và, với mọi $z \in E$,

$$
(1 \otimes x - x \otimes 1)z = 0
$$

theo định nghĩa của cấu trúc $(A \otimes_K A)$-môđun trên $E$. Vì $\mathfrak{J}$ được chứa trong linh hóa tử của môđun $(A \otimes_K A)$-môđun $E$ và cấu trúc môđun $((A \otimes_K A)/\mathfrak{J})$-môđun trên $E$ theo định nghĩa chỉ là cấu trúc $A$-môđun ban đầu đã cho trên $E$, xét đến đẳng cấu chính tắc của

$$
\mathfrak{J} \otimes_K ((A \otimes_K A)/\mathfrak{J})
$$

onto $\mathfrak{J}/\mathfrak{J}^2$ (\S 4, no. 1, Hệ quả 1 của Mệnh đề 1), ta được một đẳng cấu $K$-môđun chính tắc

$$
\operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E) \to \operatorname{Hom}_A(\mathfrak{J}/\mathfrak{J}^2, E).
$$

Xét đến Mệnh đề 17 của no. 10, thấy rằng ta đã chứng minh mệnh đề sau:

#### Mệnh đề 18 {#alg-iii-s10-prop-18 .statement}

*Cho $A$ là một $K$-đại số giao hoán và $\mathfrak{J}$ là iđêan là hạt nhân của đồng cấu chính tắc toàn ánh $m : A \otimes_K A \to A$, do đó $A$ đẳng cấu với $(A \otimes_K A)/\mathfrak{J}$ và $\mathfrak{J}/\mathfrak{J}^2$ có một cấu trúc $A$-môđun một cách chính tắc. Cho $d_{A/K} : A \to I/I^2$ là ánh xạ $K$-tuyến tính gán cho mỗi $x \in A$ lớp của $x \otimes 1 - 1 \otimes x$ modulo $\mathfrak{J}^2$. Ánh xạ $d_{A/K}$ là một $K$-đạo hàm và, với mọi $A$-môđun $E$ và mọi $K$-đạo hàm $D : A \to E$, tồn tại duy nhất một ánh xạ $A$-tuyến tính $g : \mathfrak{J}/\mathfrak{J}^2 \to E$ sao cho $D = g \circ d_{A/K}$.*

#### Ví dụ {#alg-iii-s10-n11-exa-1 .statement}

Cho $M$ là một $K$-môđun; suy ra từ Mệnh đề 14 của no. 9 rằng đối với mọi $S(M)$-môđun $E$, ánh xạ $D \mapsto D | M$ xác định một đẳng cấu $S(M)$-môđun từ $D_K(S(M), E)$ lên $\operatorname{Hom}_K(M, E)$; mặt khác, vì $E$ là một $S(M)$-môđun, $\operatorname{Hom}_K(M, E)$ đẳng cấu chính tắc với

$$
\operatorname{Hom}_{S(M)}(M \otimes_K S(M), E),
$$

mọi đồng cấu $K$ từ $M$ vào $E$ đều biểu diễn duy nhất dưới dạng $x \mapsto h(x \otimes 1)$, với

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E)
$$

(II, § 5, no. 1). Cho $D_0$ là $K$-đạo hàm $S(M) \to M \otimes_K S(M)$ có hạn chế trên $M$ là đồng cấu chính tắc $x \mapsto x \otimes 1$; do đó mọi $K$-đạo hàm $D : S(M) → E$ đều có thể được viết duy nhất dưới dạng $h \circ D_0$ với

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E).
$$

Nhờ tính duy nhất của nghiệm của một bài toán ánh xạ phổ quát, thấy rằng tồn tại duy nhất một đẳng cấu $S(M)$-môđun

$$
\omega : M \otimes_K S(M) \to \Omega_K(S(M))
$$

sao cho $D_0 \circ \omega = d_{S(M)/K}$; nói cách khác, với mọi $x \in M$, $\omega(x \otimes 1) = dx$.

Đặc biệt, *nếu $M$ là một $K$-môđun tự do với cơ sở* $(e_\lambda)_{\lambda \in L}$, $\Omega_K(S(M))$ *là một $S(M)$-môđun tự do với cơ sở là tập hợp các vi phân* $de_\lambda$. Xét riêng trường hợp $L = \{1, n\}$, do đó S(M) được đồng nhất với đại số đa thức $K[X_1, \ldots, X_n]$ (\S 6, no. 6); với mọi đa thức $P \in K[X_1, \ldots, X_n]$, ta có thể viết duy nhất

$$
dP = \sum_{i=1}^n D_i P . dX_i
$$

với $D_i P \in K[X_1, \ldots, X_n]$ và, nhờ trên đây, các ánh xạ $P \mapsto D_i P$ là các *k-đạo hàm* của $K[X_1, \ldots, X_n]$ tương ứng với các dạng tọa độ trên $\Omega_K(S(M))$ đối với cơ sở $(dX_i)$; ta cũng viết $\frac{\partial P}{\partial X_i}$ thay cho $D_i P$ và đó được gọi là *đạo hàm riêng* của P theo $X_i$.

### 12. CÁC TÍNH CHẤT HÀM TỰ CỦA K-VI PHÂN

#### Mệnh đề 19 {#alg-iii-s10-prop-19 .statement}

*Cho*

$$
\begin{array}{ccc}
K & \xrightarrow{\rho} & K' \\
\downarrow \eta & & \downarrow \eta' \\
A & \xrightarrow{u} & A'
\end{array}
$$

*là một biểu đồ giao hoán các đồng cấu vành giao hoán*, $\eta$ (tương ứng $\eta'$) *làm cho*

A (tương ứng $A'$) trở thành một $K$-đại số (tương ứng $K'$-đại số). Tồn tại duy nhất một ánh xạ $A$-tuyến tính $v : \Omega_K(A) \to \Omega_{K'}(A')$ làm cho biểu đồ sau giao hoán

$$
\begin{array}{ccc}
A & \xrightarrow{u} & A' \\
d_{A/K} \downarrow & & d_{A'/K'} \downarrow \\
\Omega_K(A) & \xrightarrow{v} & \Omega_{K'}(A')
\end{array}
$$

$d_{A'/K'} \circ u$ là một $K$-đạo hàm của $A$ với giá trị trong $A$-môđun $\Omega_{K'}(A')$; sự tồn tại và tính duy nhất của $v$ khi đó suy ra từ Mệnh đề 18 của no. 11.

Ánh xạ $v$ của Mệnh đề 19 sẽ được ký hiệu bởi $\Omega(u)$; nếu có một biểu đồ giao hoán của các đồng cấu vành giao hoán

$$
\begin{array}{cccccc}
K & \xrightarrow{\sigma} & K' & \xrightarrow{\sigma'} & K'' \\
\eta \downarrow & & \eta' \downarrow & & \eta'' \downarrow \\
A & \xrightarrow{u} & A' & \xrightarrow{u'} & A''
\end{array}
$$

thì từ tính duy nhất của Mệnh đề 19 suy ra ngay lập tức rằng

$$
\Omega(u' \circ u) = \Omega(u') \circ \Omega(u).
$$

Vì $\Omega_{K'}(A')$ là một $A'$-môđun, từ $\Omega(u)$ ta suy ra một cách chính tắc một ánh xạ $A'$-tuyến tính

$$(41)$$
$$
\Omega_0(u) : \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

sao cho $\Omega(u)$ là hợp thành của $\Omega_0(u)$ và đồng cấu chính tắc $i_A : \Omega_K(A) \to \Omega_K(A) \otimes_A A'$. Với mọi $A'$-môđun $E'$, ta có một biểu đồ giao hoán

$$
\begin{array}{ccc}
\operatorname{Hom}_{A'}(\Omega_{K'}(A'), E') & \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_{E'})} & \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \\
\phi_{A'} \downarrow & & \phi_A \circ r_A \downarrow \\
D_{K'}(A', E') & \xrightarrow{C(u)} & D_K(A, E)
\end{array}
$$

trong đó $C(u)$ là ánh xạ $D \mapsto D \circ u$ (no. 7, Mệnh đề 9) và $r_A$ là đẳng cấu chính tắc

$$
\operatorname{Hom}(i_A, 1_{E'}) : \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \to \operatorname{Hom}_A(\Omega_K(A), E');
$$

điều này suy ra ngay lập tức từ Mệnh đề 19 và định nghĩa của các đẳng cấu $\phi_A$ và $\phi_{A'}$.

#### Mệnh đề 20 {#alg-iii-s10-prop-20 .statement}

*Giả sử rằng $A' = A \otimes_K K'$, với $\eta': K' \to A'$ và $u: A \to A'$ là các đồng cấu chính tắc. Khi đó ánh xạ $A'$-tuyến tính*

$$
\Omega_0(u): \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

*là một đẳng cấu.*

Do các mũi tên thẳng đứng trong biểu đồ (42) là song ánh, ta quy về việc chứng minh rằng, với mọi $A'$-môđun $E'$, đồng cấu $C(u): D \mapsto D \circ u$ trong biểu đồ (42) là song ánh (II, § 2, no. 1, Định lý 1). Bây giờ $\mathrm{Hom}(u, 1_{E'}): \mathrm{Hom}_{K'}(A \otimes_K K', E') \to \mathrm{Hom}_K(A, E')$ là một đẳng cấu (II, § 5, no. 1, Mệnh đề 1) và $C(u)$ là hạn chế của nó lên $D_{K'}(A', E')$ nên là đơn ánh; hơn nữa, nếu $f: A' \to E'$ là một ánh xạ $K'$-tuyến tính sao cho

$$
f \circ u: A \to E'
$$

là một $K$-đạo hàm, thì từ việc $f$ là $K'$-tuyến tính và từ đẳng thức $f((x \otimes 1)(y \otimes 1)) = (y \otimes 1)f(x \otimes 1) + (x \otimes 1)f(y \otimes 1)$ với $x, y$ trong $A$, suy ra ngay lập tức rằng $f$ là một $K'$-*đạo hàm*, các phần tử $x \otimes 1$ với $x \in A$ tạo thành một hệ sinh của K'-môđun $A'$; điều này hoàn tất chứng minh rằng $C(u)$ là song ánh.

Từ nay về sau ta chỉ xét trường hợp $\rho: K \to K'$ là *ánh xạ đồng nhất* của $K$; do đó mọi đồng cấu đại số $K$ $u: A \to B$ đều được gán với một ánh xạ $B$-tuyến tính

$$
\Omega_0(u): \Omega_K(A) \otimes_K B \to \Omega_K(B).
$$

Mặt khác, ta có thể xét B-môđun của các A-vi phân $\Omega_A(B)$ vì $B$ là một A-đại số nhờ $u$; đạo hàm chính tắc $d_{B/A}: B \to \Omega_A(B)$ là *a fortiori* một K-đạo hàm, nên nó phân tích duy nhất qua

$$
B \xrightarrow{d_{B/K}} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B)
$$

trong đó $\Omega_u$ là một ánh xạ B-tuyến tính (no. 11, Mệnh đề 18). Với mọi B-môđun $E$, có một biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Hom}_B(\Omega_A(B), E) & \xrightarrow{\mathrm{Hom}(\Omega_u, 1_E)} & \mathrm{Hom}_B(\Omega_K(B), E) \\
\downarrow \phi_{A,B} & & \downarrow \phi_{K,B} \\
D_A(B, E) & \xrightarrow{j_u} & D_K(B, E)
\end{array}
$$

trong đó $j_u$ là đơn ánh chính tắc (no. 7); điều này suy ra ngay từ Mệnh đề 18 của no. 11.

#### Mệnh đề 21 {#alg-iii-s10-prop-21 .statement}

*Dãy các ánh xạ B-tuyến tính*

$$
\Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B) \to 0
$$

*là khớp.*

Điều này quy về việc kiểm tra rằng, với mọi B-môđun E, dãy

$$
0 \to \operatorname{Hom}_B(\Omega_A(B), E) \xrightarrow{\operatorname{Hom}(\Omega_u, 1_E)} \operatorname{Hom}_B(\Omega_K(B), E) \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_E)} \operatorname{Hom}_B(\Omega_K(A) \otimes_A B, E)
$$

là khớp (II, § 2, no. 1, Định lý 1); nhưng nhờ thực tế là trong các biểu đồ giao hoán (42) và (44) các mũi tên dọc là đẳng cấu, chỉ cần chứng minh rằng dãy

$$
0 \longrightarrow D_A(B, E) \xrightarrow{j_u} D_K(B, E) \xrightarrow{C(u)} D_K(A, E)
$$

là khớp, và điều đó chính là Mệnh đề 11 của no. 7.

Ta xét bây giờ trường hợp đồng cấu đại số trên K $u : A \to B$ là toàn ánh; nếu $\mathfrak{J}$ là hạt nhân của nó, thì khi đó B đẳng cấu với $A/\mathfrak{J}$. Ta xét hạn chế $d|_{\mathfrak{J}} : \mathfrak{J} \to \Omega_K(A)$ của đạo hàm chính tắc $d = d_{A/K}$ và ánh xạ A-tuyến tính hợp thành

$$
d' : \mathfrak{J} \xrightarrow{d|_{\mathfrak{J}}} \Omega_K(A) \xrightarrow{i_A} \Omega_K(A) \otimes_A B.
$$

Khi đó $d'(\mathfrak{J}^2) = 0$, vì, với $x, y$ trong $\mathfrak{J}$,

$$
d'(xy) = d(xy) \otimes 1 = (x.dy + y.dx) \otimes 1 = dy \otimes u(x) + dx \otimes u(y) = 0
$$

vì $u(x) = u(y) = 0$. Do đó từ $d'$, khi chuyển qua thương, ta thu được một ánh xạ A-tuyến tính

$$
\bar{d} : \mathfrak{J}/\mathfrak{J}^2 \to \Omega_K(A) \otimes_A B
$$

và vì $\mathfrak{J}$ triệt tiêu A-môđun $\mathfrak{J}/\mathfrak{J}^2$, nên $\bar{d}$ là một ánh xạ B-tuyến tính.

#### Mệnh đề 22 {#alg-iii-s10-prop-22 .statement}

*Cho $\mathfrak{J}$ là một iđêan của đại số giao hoán trên K A, $B = A/\mathfrak{J}$ và $u : A \to B$ là đồng cấu chính tắc. Dãy các ánh xạ B-tuyến tính*

$$
\mathfrak{J}/\mathfrak{J}^2 \xrightarrow{\bar{d}} \Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \to 0
$$

*là khớp.*

Chú ý rằng $\Omega_K(A) \otimes_A B$ được đồng nhất với $\Omega_K(A)/\mathfrak{J}\Omega_K(A)$ và ảnh của $\bar{d}$ là ảnh của $d(\mathfrak{J})$ trong môđun thương này; do đó thương của $\Omega_K(A) \otimes_A B$ bởi $\operatorname{Im}(\bar{d})$ được đồng nhất với thương $\Omega_K(A)/N$, trong đó N là A-môđun con sinh bởi $\mathfrak{J}\Omega_K(A)$ và $d(\mathfrak{J})$. Hơn nữa, ánh xạ hợp thành

$$
A \xrightarrow{d_{A/K}} \Omega_K(A) \longrightarrow \Omega_K(A)/N
$$

là một K-đạo hàm (no. 7, Mệnh đề 9) và, vì nó bằng 0 trên $\mathfrak{J}$ theo định nghĩa của N, nó xác định, khi chuyển qua thương, một K-đạo hàm $D_0 : B \to \Omega_K(A)/N$.

Xét đến tính duy nhất của nghiệm của một bài toán ánh xạ phổ quát, điều này quy về việc chứng minh rằng, với mọi B-môđun E và mọi K-đạo hàm D: B → E, tồn tại một và chỉ một ánh xạ B-tuyến tính g: Ω_K(A)/N → E sao cho D = g ∘ D_0. Nhưng ánh xạ hợp thành D ∘ u: A → E là một K-đạo hàm (no. 7, Mệnh đề 9), và do đó tồn tại một và chỉ một ánh xạ A-tuyến tính f: Ω_K(A) → E sao cho f ∘ d_{A/K} = D ∘ u. Quan hệ này đã cho thấy rằng f bằng 0 trên d(Σ); vì cũng có ΣE = {0} do E là một B-môđun, f bằng 0 trên ΣΩ_K(A); do đó f bằng 0 trên N và xác định, khi chuyển qua thương, một ánh xạ B-tuyến tính g: Ω_K(A)/N → E sao cho g ∘ D_0 = D; tính duy nhất của g suy ra từ tính duy nhất của f.

Không nên cho rằng, dù u: A → B là một đồng cấu đơn ánh, Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) là đơn ánh (Bài tập 5). Tuy nhiên ta có mệnh đề sau:

#### Mệnh đề 23 {#alg-iii-s10-prop-23 .statement}

Cho A là một đại số nguyên trên K, B là trường phân thức của nó và u: A → B là đơn ánh chính tắc. Khi đó Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) là một đẳng cấu.

Dùng thực tế rằng trong biểu đồ (42) các mũi tên dọc là song ánh, điều này quy về việc chứng minh rằng, với mọi không gian vectơ E trên B, ánh xạ C(u): D_K(B, E) → D_K(A, E) là song ánh. Nhưng điều này suy ra từ thực tế là mọi K-đạo hàm của A vào E đều có thể được mở rộng duy nhất thành một K-đạo hàm của B vào E (no. 5, Mệnh đề 5).

### Bài tập {#alg-iii-s10-exercises}

Xem [các bài tập cho § 10](exercises/s10/).
