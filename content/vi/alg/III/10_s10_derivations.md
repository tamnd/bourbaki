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
book_pages: 550-574, 645-646
pdf_pages: 0574-0598, 0669-0670
extraction: ocr
subsections:
    - "no": 1
      title: COMMUTATION FACTORS
      page: 550
      pdf_page: 574
    - "no": 2
      title: GENERAL DEFINITION OF DERIVATIONS
      page: 551
      pdf_page: 575
    - "no": 3
      title: EXAMPLES OF DERIVATIONS
      page: 553
      pdf_page: 577
    - "no": 4
      title: COMPOSITION OF DERIVATIONS
      page: 554
      pdf_page: 578
    - "no": 5
      title: DERIVATIONS OF AN ALGEBRA A INTO AN A-MODULE
      page: 557
      pdf_page: 581
    - "no": 6
      title: DERIVATIONS OF AN ALGEBRA
      page: 559
      pdf_page: 583
    - "no": 7
      title: Functorial Properties
      page: 560
      pdf_page: 584
    - "no": 8
      title: RELATIONS BETWEEN DERIVATIONS AND ALGEBRA HOMOMORPHISMS
      page: 561
      pdf_page: 585
    - "no": 9
      title: EXTENSION OF DERIVATIONS
      page: 562
      pdf_page: 586
    - "no": 10
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; NON-COMMUTATIVE CASE
      page: 567
      pdf_page: 591
    - "no": 11
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; COMMUTATIVE CASE
      page: 568
      pdf_page: 592
    - "no": 12
      title: FUNCTIORIAL PROPERTIES OF K-DIFFERENTIALS
      page: 570
      pdf_page: 594
statements: 41
exercises: 5
content_sha256: caec8df37fb2b5032ecee144d8f81b7c96d138b63883d4c58fd411f51c150999
translated_from: content/en/alg/III/10_s10_derivations.md
source_content_sha256: 321a0214d9f86881e7cc2493bc5c6c5f347dd080ee2ae7987600113edd176f01
translation_model: gpt-5.4
translation_run: translate-vi-6a225208
glossary_version: 34
glossary_terms_sha256: 2dbe9224324fb992191eac5e3b5f1517ca8fca87901836fac70d5198967c2f53
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. ĐẠO HÀM

Trong đoạn này, và trừ khi có nói rõ ngược lại, các đại số được xét không được giả thiết là kết hợp cũng không nhất thiết có phần tử đơn vị; K ký hiệu một vành giao hoán.

### 1. NHÂN TỬ GIAO HOÁN

Khi trong đoạn này chúng ta nói về các phân bậc mà không nói rõ, ta sẽ luôn hiểu là các phân bậc kiểu $\Delta$, trong đó $\Delta$ là một nhóm giao hoán viết theo lối cộng. Trong đoạn này, một nhân tử giao hoán trên $\Delta$ với giá trị trong $\mathbf{Z}$ được gọi là một nhân tử giao hoán trên $\Delta$ (§ 4, no. 7, Định nghĩa 6). Do đó, một nhân tử giao hoán trên $\Delta$ được đồng nhất với một ánh xạ $\varepsilon : (\alpha, \beta) \mapsto \varepsilon_{\alpha \beta} = \varepsilon(\alpha, \beta)$ từ $\Delta \times \Delta$ vào nhóm nhân $\{-1, 1\}$ sao cho với $\alpha, \alpha', \beta, \beta'$ thuộc $\Delta$,

$$
\begin{cases}
\varepsilon(\alpha + \alpha', \beta) = \varepsilon(\alpha, \beta)\varepsilon(\alpha', \beta) \\
\varepsilon(\alpha, \beta + \beta') = \varepsilon(\alpha, \beta)\varepsilon(\alpha, \beta') \\
\varepsilon(\beta, \alpha) = \varepsilon(\alpha, \beta).
\end{cases}
$$

(1)

Suy ra rằng $\varepsilon(2\alpha, \beta) = \varepsilon(\alpha, 2\beta) = 1$.

Khi $\Delta = \mathbf{Z}$, mọi nhân tử giao hoán $\varepsilon$ được xác định bởi việc cho $\varepsilon(1, 1)$; do đó chỉ có *hai* nhân tử như vậy, nhân tử thứ nhất được xác định bởi

(2)
$$
\varepsilon(p, q) = 1 \quad \text{với } p, q \text{ trong } \mathbf{Z}
$$
và nhân tử thứ hai bởi
(3)
$$
\varepsilon(p, q) = (-1)^{pq} \quad \text{với } p, q \text{ trong } \mathbf{Z}.
$$

### 2. ĐỊNH NGHĨA TỔNG QUÁT CỦA CÁC ĐẠO HÀM

Xét một vành giao hoán $K$, sáu $K$-môđun phân bậc kiểu $\Delta : A, A', A'', B, B', B''$, và ba ánh xạ $K$-tuyến tính
$$
\mu : A \times A' \to A'', \qquad \lambda_1 : B \times A' \to B'', \qquad \lambda_2 : A \times B' \to B''
$$
sao cho các ánh xạ $K$-tuyến tính tương ứng
$$
A \otimes_K A' \to A'', \qquad B \otimes_K A' \to B'', \qquad A \otimes_K B' \to B''
$$
là *phân bậc bậc* 0. Ảnh $\mu(a, a')$ với $a \in A, a' \in A'$ được ký hiệu đơn giản là $a.a'$ hoặc thậm chí $aa'$, và tương tự đối với hai ánh xạ song tuyến tính kia. Do đó, *bậc* của $a.a'$ là *tổng* các bậc của $a$ và $a'$.

#### Định nghĩa 1 {#alg-iii-s10-def-1 .statement}

*Với các dữ kiện trên và một nhân tử giao hoán $\varepsilon$ trên $\Delta \times \Delta$, một $\varepsilon$-đạo hàm (hay đạo hàm $(K, \varepsilon)$) bậc $\delta \in \Delta$ từ $(A, A', A'')$ vào $(B, B', B'')$ là một bộ ba ánh xạ $K$-tuyến tính phân bậc bậc $\delta$:*
$$
d : A \to B, \qquad d' : A' \to B', \qquad d'' : A'' \to B''
$$
*thoả mãn rằng, với mọi phần tử thuần nhất $a \in A$ và mọi phần tử $a' \in A'$*
(4)
$$
d''(a.a') = (da).a' + \varepsilon_{\delta, \deg(a)}a.(d'a').
$$

Hiển nhiên chỉ cần, nhờ tính tuyến tính, kiểm tra quan hệ (4) khi $a$ và $a'$ chạy trong các hệ sinh tương ứng của $A$ và $A'$.

Thường khi đó tiện ký hiệu ba ánh xạ $d, d', d''$ bằng cùng một chữ $d$ (điều này có thể được biện minh bằng cách cũng ký hiệu bởi $d$ ánh xạ $K$-tuyến tính phân bậc bậc $\delta$)

$$
(a, a', a'') \mapsto (da, d'a', d''a'')
$$

của $A \oplus A' \oplus A''$ vào $B \oplus B' \oplus B''$). Khi đó quan hệ (4) có thể được viết đơn giản hơn
$$
d(a.a') = (da).a' + \varepsilon_{\delta,\deg(a)} a.(da').
$$
Các $\varepsilon$-đạo hàm của $(A, A', A'')$ vào $(B, B', B'')$ có bậc *cho trước* tạo thành một môđun con của K-môđun các ánh xạ tuyến tính phân bậc
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
Khi $\varepsilon(\alpha, \beta) = 1$ với mọi $\alpha, \beta$ trong $\Delta$, thay cho $\varepsilon$-đạo hàm ta nói đơn giản là *đạo hàm* (hoặc *K-đạo hàm*). Các đạo hàm tạo thành một môđun con của
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
Khi $\Delta = \mathbf{Z}$ và $\varepsilon(p.q) = (-1)^{pq}$, mọi $\varepsilon$-đạo hàm có bậc *chẵn* đều là một đạo hàm; mọi $\varepsilon$-đạo hàm có bậc *lẻ* thường được gọi là một *phản đạo hàm* (hoặc *K-phản đạo hàm*); do đó một phản đạo hàm $d$ thỏa mãn
$$
d(a.a') = (da).a' + (-1)^{\deg(a)} a.(da')
$$
đối với một phần tử *thuần nhất* $a \in A$.

#### Nhận xét {#alg-iii-s10-n2-rem-1 .statement}

(1) Khái niệm *đạo hàm* có thể được định nghĩa cho các môđun không phân bậc bằng cách quy ước cho các môđun này phân bậc tầm thường.

(2) Nếu chỉ xét các $\varepsilon$-đạo hàm có bậc $\delta$ cho trước, thì nhân tử giao hoán $\varepsilon$ có thể được loại bỏ như sau: ánh xạ song tuyến tính $\lambda_2 : A \times B' \to B''$ được sửa đổi bằng cách thay thế nó bằng ánh xạ song tuyến tính $\lambda'_2 : A \times B' \to B''$ sao cho, với mọi $a$ *thuần nhất* trong $A$ và mọi $b' \in B'$,
$$
\lambda'_2(a, b') = \varepsilon_{\delta, \deg(a)} \lambda_2(a, b').
$$
Khi đó $d$ là một đạo hàm đối với các ánh xạ song tuyến tính $\mu, \lambda_1, \lambda'_2$.

Định nghĩa tổng quát về các $\varepsilon$-đạo hàm đã cho ở trên được dùng đặc biệt trong hai trường hợp:

*Trường hợp (I)*: $A = B, A' = B', A'' = B''$ và ba ánh xạ song tuyến tính $\mu, \lambda_1, \lambda_2$ bằng *cùng một* ánh xạ.

*Trường hợp (II)*: $A = A' = A'', B = B' = B''$, sao cho (đối với $\mu$) $A$ là một *đại số phân bậc* và hai ánh xạ K-song tuyến tính.
$$
\lambda_1 : B \times A \to B, \quad \lambda_2 : A \times B \to B
$$
có tính chất là các ánh xạ K-tuyến tính tương ứng $B \otimes_K A \to B, A \otimes_K B \to B$ là phân bậc bậc 0. Khi đó một $\varepsilon$-đạo hàm bậc $\delta$ của $A$ vào $B$ là một ánh xạ K-tuyến tính phân bậc $d : A \to B$ bậc $\delta$, sao cho với mọi $x$ thuần nhất trong $A$ và mọi $y \in A$, ta có quan hệ
$$
d(xy) = (dx)y + \varepsilon_{\delta, \deg(a)} x(dy).
$$

Hãy xét riêng, trong trường hợp (II), trường hợp A là một đại số kết hợp có đơn vị trên K và $\lambda_1$ và $\lambda_2$ là các luật ngoài của một song môđun (A, A) (§ 4, no. 3, Định nghĩa 3). Điều này đúng đặc biệt khi A và B là hai đại số kết hợp có đơn vị trên K, đã cho một đồng cấu có đơn vị của các đại số K phân bậc $\rho : A \to B$, và xét trên B một cấu trúc song môđun (A, A) được định nghĩa bởi hai luật ngoài

$$
\lambda_1 : (b, a) \mapsto b \rho(a), \qquad \lambda_2 : (a, b) \mapsto \rho(a)b
$$

với $a \in A, b \in B$.

Các trường hợp (I) và (II) có điểm chung sau đây: xét một đại số trên K phân bậc A, lấy $B = A$, hai ánh xạ (7) đều là phép nhân trên A. Khi đó ta nói đến một $\varepsilon$-đạo hàm (hay (K, $\varepsilon$)-đạo hàm) của đại số phân bậc A: đó là một ánh xạ K-tuyến tính phân bậc từ A vào chính nó, bậc $\delta$, thỏa mãn (8) với mọi $x$ thuần nhất trong A và mọi $y \in A$. Đặc biệt, nếu A là một vành phân bậc, được xét như một đại số trên $\mathbf{Z}$ (kết hợp), thì ta nói đến $\varepsilon$-đạo hàm của vành A.

Cho A là một đại số trên K có đơn vị, giao hoán và kết hợp, và B là một A-môđun; khi ta nói đến một đạo hàm từ A vào B, điều đó luôn được hiểu là đối với cấu trúc song môđun trên B dẫn xuất từ cấu trúc A-môđun của nó; khi đó công thức

$$
d(xy) = x(dy) + y(dx) \quad \text{với} \quad x \in A, y \in A
$$

đúng với một đạo hàm như vậy $d : A \to B$.

### 3. VÍ DỤ VỀ CÁC ĐẠO HÀM

#### Ví dụ 1 {#alg-iii-s10-n3-exa-1 .statement}

Cho A là một đại số trên $\mathbf{R}$ các ánh xạ khả vi từ $\mathbf{R}$ vào $\mathbf{R}$ và $x_0$ là một điểm của $\mathbf{R}$; $\mathbf{R}$ có thể được xét như một A-môđun với phép toán ngoài $(f, a) \mapsto f(x_0)a$. Khi đó ánh xạ $f \mapsto Df(x_0)$ là một đạo hàm, vì (Functions of a Real Variable, I, § 1, no. 3)

$$
(D(fg))(x_0) = (Df(x_0))g(x_0) + f(x_0)(Dg(x_0)).*
$$

#### Ví dụ 2 {#alg-iii-s10-n3-exa-2 .statement}

Cho X là một đa tạp khả vi lớp $C^\infty$ và A là đại số trên $\mathbf{R}$ phân bậc các dạng vi phân trên X. Ánh xạ gán cho mỗi dạng vi phân $\omega$ trên X vi phân ngoài $d\omega$ của nó là một phản đạo hàm bậc +1 (Differentiable and Analytic Manifolds, R, § 8).*

#### Ví dụ 3 {#alg-iii-s10-n3-exa-3 .statement}

Cho A là một đại số trên K kết hợp. Với mọi $a \in A$, ánh xạ $x \mapsto ax - xa$ là một đạo hàm của đại số A (xem no. 6).

#### Ví dụ 4 {#alg-iii-s10-n3-exa-4 .statement}

Cho M là một K-môđun và A là đại số ngoài $\bigwedge(M^*)$ với phân bậc thông thường của nó (§ 7, no. 1). *Sẽ thấy ở § 11, no. 9 rằng, với mọi $x \in M$, tích trong bên phải $i(x)$ là một phản đạo hàm của A bậc $-1$.*

#### Ví dụ 5 {#alg-iii-s10-n3-exa-5 .statement}

Trở lại tình huống tổng quát của Định nghĩa 1 ở no. 2, cho $\overline{K}$ là một vành giao hoán khác và $\rho : K \to \overline{K}$ là một đồng cấu vành; ký hiệu $\overline{A}, \overline{A}', \overline{A}'', \overline{B}, \overline{B}', \overline{B}''$ lần lượt là các $\overline{K}$-môđun phân bậc thu được từ $A, A', A'', B, B', B''$ bằng cách mở rộng vành vô hướng lên $\overline{K}$ (II, § 11, no. 5); từ $\mu, \lambda_1$ và $\lambda_2$ ta suy ra các ánh xạ $\overline{K}$-song tuyến tính
$$
\bar{\mu} : \overline{A} \times \overline{A}' \to \overline{A}'', \quad \bar{\lambda}_1 : \overline{B} \times \overline{A}' \to \overline{B}'', \quad \bar{\lambda}_2 : \overline{A} \times \overline{B}' \to \overline{B}''
$$
bằng cách xét các tích tenxơ theo $l_{\overline{K}}$ của các ánh xạ K-tuyến tính tương ứng với $\mu, \lambda_1$ và $\lambda_2$ (II, § 5, no. 1). Khi đó, nếu $d$ là một $\varepsilon$-đạo hàm bậc $\delta$ của $(A, A', A'')$ vào $(B, B', B'')$, thì ánh xạ $\bar{d} = d \otimes l_{\overline{K}}$ từ $\overline{A} \oplus \overline{A}' \oplus \overline{A}''$ vào $\overline{B} \oplus \overline{B}' \oplus \overline{B}''$ là một $\varepsilon$-đạo hàm bậc $\delta$ của $(\overline{A}, \overline{A}', \overline{A}'')$ vào $(\overline{B}, \overline{B}', \overline{B}'')$.

#### Ví dụ 6 {#alg-iii-s10-n3-exa-6 .statement}

Cho $A$ là một đại số $K$ phân bậc kiểu $\mathbf{Z}$$;$ một ánh xạ $K$-tuyến tính phân bậc bậc 0, $d : A \to A$, được định nghĩa bằng cách đặt, với $x_n \in A_n (n \in \mathbf{Z})$, $d(x_n) = nx_n$. Ánh xạ này là một đạo hàm của $A$, vì, với $x_p \in A_p, x_q \in A_q$,
$$
d(x_p x_q) = (p + q)x_p x_q = d(x_p)x_q + x_p d(x_q).
$$

### 4. HỢP THÀNH CÁC ĐẠO HÀM

Trong số này, ta giả sử rằng trường hợp (I) của no. 2 được thỏa mãn, nghĩa là $A, A', A''$ là ba $K$-môđun phân bậc kiểu $\Delta$ và rằng ta được cho một ánh xạ $K$-song tuyến tính $\mu : A \times A' \to A''$ tương ứng với một ánh xạ $K$-tuyến tính phân bậc bậc 0, $A \otimes_K A' \to A''$. Các nội đồng cấu phân bậc $f$ của $A \oplus A' \oplus A''$ sao cho $f(A) \subset A, f(A') \subset A'$ và $f(A'') \subset A''$ tạo thành một đại số con phân bậc của đại số kết hợp phân bậc $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ (§ 3, no. 1, Ví dụ 2). Đặc biệt, hai $\varepsilon$-đạo hàm của $(A, A', A'')$ có thể được hợp thành, nhưng không nên nghĩ rằng hợp thành của hai $\varepsilon$-đạo hàm là một $\varepsilon$-đạo hàm.

Trên mọi đại số phân bậc $B$ kiểu $\Delta$, ta định nghĩa ngoặc $\varepsilon$ (hay đơn giản là ngoặc khi $\varepsilon = 1$) của hai phần tử thuần nhất $u, v$, bằng công thức (10)
$$
[u, v]_\varepsilon = uv - \varepsilon_{\deg u, \deg v} vu \text{ (ký hiệu đơn giản là } [u, v] \text{ nếu } \varepsilon = 1).
$$
Mở rộng ánh xạ này bằng tính tuyến tính, ta thu được một ánh xạ $K$-song tuyến tính $(u, v) \mapsto [u, v]_\varepsilon$ từ $B \times B$ vào $B$. Khi đó, với $u$ và $v$ thuần nhất trong $B$
$$
[v, u]_\varepsilon = -\varepsilon_{\deg u, \deg v}[u, v]_\varepsilon.
$$
Áp dụng định nghĩa này cho đại số phân bậc $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$, như vậy ngoặc $\varepsilon$ của hai nội đồng cấu phân bậc được định nghĩa.

#### Mệnh đề 1 {#alg-iii-s10-prop-1 .statement}

*Cho $d_1, d_2$ là hai $\varepsilon$-đạo hàm của $(A, A', A'')$ có các bậc tương ứng $\delta_1, \delta_2$. Khi đó ngoặc $\varepsilon$*
$$
[d_1, d_2]_\varepsilon = d_1 \circ d_2 - \varepsilon_{\delta_1, \delta_2} d_2 \circ d_1
$$
*là một $\varepsilon$-đạo hàm bậc $\delta_1 + \delta_2$. Hơn nữa, nếu $d$ là một $\varepsilon$-đạo hàm của $(A, A', A'')$ bậc $\delta$ và nếu $\varepsilon_{\delta, \delta} = -1$, thì $d^2 = d \circ d$ là một đạo hàm.*

Giả sử $x \in A$ là thuần nhất bậc $\xi$; với mọi $y \in A'$,
$$
d_1(d_2(xy)) = ((d_1 d_2)(x))y + \varepsilon_{\delta_1, \delta_2 + \xi}(d_2 x)(d_1 y)
+ \varepsilon_{\delta_2, \xi}(d_1 x)(d_2 y) + \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
$$
có tính đến các công thức (1) của no. 1. Đổi vai trò của $d_1$ và $d_2$, ta lại thu được, sau các phép rút gọn dùng (1) (no. 1),
$$
(d_1 d_2)(xy) - \varepsilon_{\delta_1, \delta_2}(d_2 d_1)(xy) = ((d_1 d_2)(x))y - \varepsilon_{\delta_1, \delta_2}((d_2 d_1)(x))y
+ \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
- \varepsilon_{\delta_1, \delta_2} \varepsilon_{\delta_1 + \delta_2, \xi} x((d_2 d_1)(y))
$$
nghĩa là, viết $d = [d_1, d_2]_\varepsilon$ và $\delta = \delta_1 + \delta_2$,
$$
d(xy) = (dx)y + \varepsilon_{\delta, \xi} x(dy)
$$
điều này chứng minh rằng $d$ là một $\varepsilon$-đạo hàm.

Mặt khác, nếu trong (11), ta đặt $d_1 = d_2 = d$, $\delta_1 = \delta_2 = \delta$ và $\varepsilon_{\delta, \delta} = -1$, thì ta thu được, vì khi đó $\varepsilon_{\delta, \delta + \xi} = -\varepsilon_{\delta, \xi}$ theo (1),
$$
d^2(xy) = (d^2 x)y + \varepsilon_{2\delta, \xi} x(d^2 y)
$$
và vì $\varepsilon_{2\delta, \xi} = 1$ nên ta thấy $d^2$ là một đạo hàm.

#### Hệ quả {#alg-iii-s10-n4-cor-1 .statement}

*Giả sử rằng $\Delta = \mathbf{Z}$. Khi đó:*
(i) *Bình phương của một phản đạo hàm là một đạo hàm.*
(ii) *Ngoặc của hai đạo hàm là một đạo hàm.*
(iii) *Ngoặc của một phản đạo hàm và một đạo hàm bậc chẵn là một phản đạo hàm.*
(iv) *Nếu $d_1$ và $d_2$ là các phản đạo hàm, thì $d_1 d_2 + d_2 d_1$ là một đạo hàm.*

Dưới các giả thiết ở đầu số này, bây giờ xét một dãy hữu hạn $D = (d_i)_{1 \leq i \leq n}$ gồm các *đạo hàm hoán vị từng đôi một* của $(A, A', A'')$. Với mọi đa thức $P(X_1, \ldots, X_n)$ trong đại số $K[X_1, \ldots, X_n]$, phần tử $P(d_1, \ldots, d_n)$ của $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ khi đó được xác định (§ 2, no. 9); ký hiệu rút gọn của nó là $P(D)$.

#### Mệnh đề 2 {#alg-iii-s10-prop-2 .statement}

*Với các giả thiết và ký hiệu trên đây, xét 2n ẩn số $T_1, \ldots, T_n, T'_1, \ldots, T'_n$ và với mọi đa thức $F \in K[X_1, \ldots, X_n]$ viết $F(T) = F(T_1, \ldots, T_n), F(T') = F(T'_1, \ldots, T'_n)$ và*
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

Ta đưa vào $n$ ẩn số khác $T_1'', \ldots, T_n''$ và xét đại số đa thức $K[T_1, \ldots, T_n, T_1', \ldots, T_n', T_1'', \ldots, T_n''] = B$; mặt khác ta xét $K$-môđun $M$ gồm các ánh xạ song tuyến tính từ $A \times A'$ vào $A''$; một cấu trúc B-môđun được xác định trên $M$ bằng cách viết, với mọi ánh xạ $K$-song tuyến tính $f \in M$ và $1 \leq i \leq n$,

$$
\begin{cases}
(T_i f)(a, a') = f(d_i a, a') \\
(T_i' f)(a, a') = f(a, d_i a') \\
(T_i'' f)(a, a') = d_i(f(a, a'))
\end{cases}
$$

Vì các $d_i$ hoán vị với nhau từng đôi một, ta thấy rằng, với mọi đa thức $F \in K[X_1, \ldots, X_n]$, $(F(T)f)(a, a') = f(F(D)a, a')$,

$$
(F(T')f)(a, a') = f(a, F(D)a')
$$

và $(F(T'')f) = F(D)(f(a, a'))$. Do đó, để chứng minh (12), chỉ cần chỉ ra rằng

$$
(P(T'') - \sum_i Q_i(T)R_i(T')).\mu = 0
$$

hoặc cũng có $(P(T'') - P(T + T')).\mu = 0$ trong B-môđun $M$. Bây giờ, giả thiết rằng các $d_i$ là các đạo hàm cũng có thể được diễn đạt bằng cách nói rằng, với $1 \leq i \leq n$,

$$
(T_i'' - T_i - T_i').\mu = 0
$$

trong B-môđun $M$. Khi xét lần lượt các đa thức

$P(T_1'', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2'', \ldots, T_n'')$
$P(T_1 + T_1', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2 + T_2', \ldots, T_n'')$
$\ldots$
$P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n'') - P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n + T_n')$

người ta thấy rằng hiệu $P(T'') - P(T + T')$ có thể được viết dưới dạng

$$
\sum_{i=1}^n (T_i'' - T_i - T_i') G_i(T, T', T'')
$$

trong đó các $G_i$ là những phần tử của $B$. Do đó, quan hệ (14) là một hệ quả ngay lập tức của các quan hệ (15).

#### Hệ quả (công thức Leibniz) {#alg-iii-s10-n4-cor-2 .statement}

*Cho $d_i$ ($1 \leq i \leq n$) là $n$ đạo hàm của $(A, A', A'')$ hoán vị được với nhau. Với mọi $\alpha = (\alpha_1, \ldots, \alpha_n) \in \mathbf{N}^n$, ta viết*

$$
d^\alpha = d_1^{\alpha_1} d_2^{\alpha_2} \ldots d_n^{\alpha_n}.
$$

Khi đó, với $x \in \mathbf{A}$ và $y \in \mathbf{A}'$,

$$
d^\alpha(xy) = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) d^\beta(x)d^\gamma(y)
$$

trong đó ta đã viết (theo ký hiệu được đưa vào ở đầu chương)

$$
((\beta, \gamma)) = (\beta + \gamma)!/(\beta! \gamma!).
$$

Điều này suy ra ngay lập tức từ công thức đa thức Newton (I, § 8, no. 2)

$$
(T + T')^\alpha = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) T^\beta {T'}^\gamma
$$

và Mệnh đề 2.

### 5. CÁC ĐẠO HÀM CỦA MỘT ĐẠI SỐ A VÀO MỘT A-MÔĐUN

Trong số này, ta giả sử rằng Trường hợp (II) của no. 2 được thỏa mãn. Khi đó có một K-đại số phân bậc A và một K-môđun phân bậc E và cũng có hai ánh xạ K-tuyến tính bậc 0

$$
E \otimes_K A \to E, \quad A \otimes_K E \to E
$$

được ký hiệu bởi

$$
x \otimes a \mapsto x.a \quad \text{và} \quad a \otimes x \mapsto a.x \quad \text{cho } a \in A \text{ và } x \in E.
$$

#### Mệnh đề 3 {#alg-iii-s10-prop-3 .statement}

Cho $d : A \to E$ là một $\varepsilon$-đạo hàm bậc $\delta$. Khi đó $\mathrm{Ker}(d)$ là một đại số con phân bậc của A; nếu A có một phần tử đơn vị, thì phần tử ấy thuộc $\mathrm{Ker}(d)$.

Rõ ràng $\mathrm{Ker}(d)$ là một K-môđun con phân bậc của A; hơn nữa, quan hệ (8) của no. 2 cho thấy rằng, nếu $x$ và $y$ là hai phần tử thuần nhất thuộc $\mathrm{Ker}(d)$, thì $d(xy) = 0$ và do đó $xy \in \mathrm{Ker}(d)$. Sau cùng, nếu A có một phần tử đơn vị 1 (bậc 0, xem § 3, no. 1), thì quan hệ (8) của no. 2, trong đó $x$ và $y$ được thay bởi 1, cho $d(1) = d(1) + d(1)$ và do đó $d(1) = 0$.

#### Hệ quả {#alg-iii-s10-n5-cor-1 .statement}

Cho $d_1$ và $d_2$ là hai $\varepsilon$-đạo hàm từ A đến E cùng bậc $\delta$. Nếu $d_1$ và $d_2$ nhận cùng giá trị tại mỗi phần tử của một hệ sinh của đại số A, thì $d_1 = d_2$.

$d_1 - d_2$ là một $\varepsilon$-đạo hàm bậc $\delta$, vì vậy $\mathrm{Ker}(d_1 - d_2)$ là một đại số con của A chứa một hệ sinh của A và do đó bằng A.

#### Mệnh đề 4 {#alg-iii-s10-prop-4 .statement}

Cho $d : A \to E$ là một $\varepsilon$-đạo hàm bậc $\delta$. Giả sử rằng A có một phần tử đơn vị 1 và cho $x$ là một phần tử thuần nhất của A có một nghịch đảo $x^{-1}$ trong A. Khi đó

$$
d(x^{-1}) = -\varepsilon_{\delta, \deg(x)} x^{-1}((dx)x^{-1}) = -\varepsilon_{\delta, \deg(x)} (x^{-1}(dx))x^{-1}.
$$

Ta có $d(xx^{-1}) = d(1) = 0$ (Mệnh đề 3), do đó
$$
(dx)x^{-1} + \varepsilon_{\delta, \deg(x)} x(d(x^{-1})) = 0
$$
điều này chứng minh công thức thứ nhất của (19). Mặt khác, $x^{-1}$ là thuần nhất bậc $-\deg(x)$ và $\varepsilon_{\delta, \deg(x)} = \varepsilon_{\delta, -\deg(x)}$ theo các công thức (1) của no. 1; viết $d(x^{-1}x) = 0$, ta thu được công thức thứ hai của (19) một cách tương tự.

#### Mệnh đề 5 {#alg-iii-s10-prop-5 .statement}

*Giả sử rằng $\mathbf{A}$ là một miền nguyên và $\mathbf{L}$ là trường phân thức của nó. Mọi đạo hàm của $\mathbf{A}$ vào một không gian vectơ $\mathbf{E}$ trên $\mathbf{L}$ (được coi như một $\mathbf{A}$-môđun) đều có thể được mở rộng duy nhất thành một đạo hàm của $\mathbf{L}$ vào $\mathbf{E}$.*

Cho $d$ là một đạo hàm của $\mathbf{A}$ vào $\mathbf{E}$ và $\bar{d}$ là một đạo hàm của $\mathbf{L}$ vào $\mathbf{E}$ mở rộng $d$; khi đó, với $u \in \mathbf{A}, v \in \mathbf{A}, v \neq 0$, tất yếu, theo (19),
$$
\bar{d}(u/v) = v^{-1}du - uv^{-2}dv
$$
điều này chứng minh tính duy nhất của $\bar{d}$. Ngược lại, ta chỉ ra rằng $\bar{d}$ có thể được xác định bởi công thức (20); trước hết phải kiểm tra rằng nếu $u/v = u'/v'$ thì giá trị của vế phải của (20) không thay đổi khi thay $u$ bằng $u'$ và $v$ bằng $v'$. Thật vậy, $uv' = vu'$, nên $v'(du) + u(dv') = v(du') + u'(dv)$ và do đó $v'(du - uv^{-1}dv) = v(du' - u'{v'}^{-1}dv')$, vì $uv'v^{-1} = u'$ và $u'{v'}^{-1}v = u$. Như vậy đã xác định được một ánh xạ $\bar{d}: \mathbf{L} \to \mathbf{E}$ mở rộng $d$; kiểm tra ngay lập tức được rằng nó là $\mathbf{K}$-tuyến tính và là một đạo hàm.

#### Mệnh đề 6 {#alg-iii-s10-prop-6 .statement}

*Giả sử rằng $\mathbf{A}$ là một $\mathbf{K}$-đại số phân bậc kết hợp có đơn vị và $\mathbf{E}$ là một song môđun phân bậc $(\mathbf{A}, \mathbf{A})$. Nếu $d : \mathbf{A} \to \mathbf{E}$ là một $\varepsilon$-đạo hàm bậc $\delta$, thì với mọi dãy hữu hạn $(x_i)_{1 \leq i \leq n}$ gồm các phần tử thuần nhất của $\mathbf{A}$, có các bậc tương ứng $\xi_i$ ($1 \leq i \leq n$),
$$
d(x_1 x_2 \ldots x_n) = \sum_{i=1}^n \varepsilon_{\delta, \xi_1 + \cdots + \xi_{i-1}} x_1 \cdots x_{i-1} (dx_i) x_{i+1} \cdots x_n.
$$
Công thức (21) là tầm thường đối với $n = 0$ và được chứng minh bằng quy nạp theo $n$, có tính đến (4) (no. 2).

#### Hệ quả {#alg-iii-s10-n5-cor-2 .statement}

*Giả sử rằng $\mathbf{A}$ là một đại số giao hoán kết hợp có đơn vị và $\mathbf{E}$ là một $\mathbf{A}$-môđun. Nếu $d : \mathbf{A} \to \mathbf{E}$ là một đạo hàm, thì, với mọi số nguyên $n \geq 0$,
$$
d(x^n) = nx^{n-1}(dx) \quad \text{với mọi } x \in \mathbf{A}.
$$
Chỉ cần cho $\mathbf{A}$ phân bậc tầm thường và áp dụng (21) với mọi $x_i$ đều bằng $x$.

Ta trở lại trường hợp tổng quát của một $\varepsilon$-đạo hàm $d : \mathbf{A} \to \mathbf{E}$ bậc $\delta$. Ký hiệu $Z_\delta$ là tập hợp các $a \in \mathbf{A}$ sao cho với mọi thành phần thuần nhất $a_\alpha$ của $a$ có bậc $\alpha$, với mọi $x$ thuần nhất trong $\mathbf{E}$,
$$
xa_\alpha = \varepsilon_{\alpha, \deg(x)} a_\alpha x.
$$

Nếu $A$ là một đại số phân bậc kết hợp có đơn vị và $E$ là một song môđun phân bậc $(A, A)$ thì theo định nghĩa này suy ra ngay lập tức rằng $Z_\varepsilon$ là một *đại số con phân bậc* của $A$ chứa phần tử đơn vị.

#### Mệnh đề 7 {#alg-iii-s10-prop-7 .statement}

*Giả sử rằng $A$ là một đại số phân bậc kết hợp có đơn vị và $E$ là một song môđun phân bậc $(A, A)$. Cho $d : A \to E$ là một $\varepsilon$-đạo hàm bậc $\delta$ và $a$ là một phần tử thuần nhất của $Z_\varepsilon$ có bậc $\alpha$. Khi đó ánh xạ $x \mapsto a(dx)$ là một $\varepsilon$-đạo hàm bậc $\delta + \alpha$.*

Ta viết $d'(x) = a(dx)$; với $x$ thuần nhất bậc $\xi$ trong $A$ và $y \in A$, theo (23) và (1) (no. 1),

$$
d'(xy) = a((dx)y) + \varepsilon_{\delta, \xi} a(x(dy)) = (a(dx))y + \varepsilon_{\delta+\alpha, \xi}(xa)(dy)
= (d'x)y + \varepsilon_{\delta+\alpha, \xi} x(d'y).
$$

Mệnh đề 7 nói rằng K-môđun các $\varepsilon$-đạo hàm của $A$ vào $E$ là một *$Z_\varepsilon$-môđun phân bậc* kiểu $\Delta$.

### 6. CÁC ĐẠO HÀM CỦA MỘT ĐẠI SỐ

Cho $A$ là một đại số trên K phân bậc; với mỗi phần tử *thuần nhất* $a \in A$, ký hiệu $\mathrm{ad}_\varepsilon(a)$, hoặc đơn giản là $\mathrm{ad}(a)$ nếu không thể có nhầm lẫn, là ánh xạ K-tuyến tính từ $A$ vào $A$

$$
x \mapsto [a, x]_\varepsilon
$$
(no. 4, công thức (10)) *phân bậc bậc* $\deg a$.

#### Mệnh đề 8 {#alg-iii-s10-prop-8 .statement}

*Cho $A$ là một đại số trên K phân bậc.*

(i) *Với mọi $\varepsilon$*-đạo hàm $d : A \to A$ và mọi phần tử thuần nhất $a$ của $A$,

$$(24)$$
$$
[d, \mathrm{ad}_\varepsilon(a)]_\varepsilon = \mathrm{ad}_\varepsilon(da).
$$

(ii) *Nếu đại số $A$ là kết hợp, thì $\mathrm{ad}_\varepsilon(a)$ là một $\varepsilon$*-đạo hàm của $A$ bậc $\deg(a)$.

(i) Giả sử $d$ có bậc $\delta$, đặt $\alpha = \deg a$ và viết $f = [d, \mathrm{ad}_\varepsilon(a)]_\varepsilon$. Với mọi phần tử thuần nhất $x \in A$ bậc $\xi$, theo (1) (no. 1), ta có

$$
f(x) = d(ax - \varepsilon(\alpha, \xi) xa) - \varepsilon_{\delta, \alpha}(a(dx)) - \varepsilon_{\alpha, \delta+\xi}(dx)a \\
= (da)x + \varepsilon_{\delta, \alpha} a(dx) - \varepsilon_{\alpha, \xi}(dx)a - \varepsilon_{\delta+\alpha, \xi} x(da) \\
- \varepsilon_{\delta, \alpha} a(dx) + \varepsilon_{\alpha, \xi}(dx)a \\
= (da)x - \varepsilon_{\delta+\alpha, \xi} x(da) = [da, x]_\varepsilon.
$$

(ii) Với mọi $x$ thuần nhất bậc $\xi$ và mọi $y$ thuần nhất bậc $\eta$ trong $A$,

$$
\mathrm{ad}_\varepsilon(a)(xy) = a(xy) - \varepsilon_{\alpha, \xi+\eta}(xy)a \\
= (ax - \varepsilon_{\alpha, \xi} xa)y + \varepsilon_{\alpha, \xi} x(ay - \varepsilon_{\alpha, \eta} ya) \\
= \mathrm{ad}_\varepsilon(a)(x).y + \varepsilon_{\alpha, \xi} x.\mathrm{ad}_\varepsilon(a)(y)
$$
có tính đến (1) và tính kết hợp của $A$.

Khi $A$ là kết hợp, $\mathrm{ad}_\varepsilon(a)$ được gọi là *đạo hàm $\varepsilon$-nội* của $A$ xác định bởi $a$.

#### Hệ quả {#alg-iii-s10-n6-cor-1 .statement}

*Cho $A$ là một đại số phân bậc kết hợp. Với hai phần tử thuần nhất $a, b$ của $A$,*
$$
[\mathrm{ad}_\varepsilon(a), \mathrm{ad}_\varepsilon(b)]_\varepsilon = \mathrm{ad}_\varepsilon([a, b]_\varepsilon).
$$
(25)

Chỉ cần thay thế $d$ bởi $\mathrm{ad}_\varepsilon(a)$ và $\mathrm{ad}_\varepsilon(a)$ bởi $\mathrm{ad}_\varepsilon(b)$ trong (24).

Nếu $\deg a = \alpha, \deg b = \beta$, công thức (25) tương đương với quan hệ sau đây đối với mọi phần tử thuần nhất $c \in A$ bậc $\gamma$
$$
\varepsilon_{\alpha, \gamma}[a, [b, c]_\varepsilon]_\varepsilon + \varepsilon_{\beta, \alpha}[b, [c, a]_\varepsilon]_\varepsilon + \varepsilon_{\gamma, \beta}[c, [a, b]_\varepsilon]_\varepsilon = 0
$$
được gọi là *đồng nhất thức Jacobi*.

### 7. Các Tính Chất Hàm Tử

*Trong số này, mọi đại số đều được giả sử là kết hợp và có đơn vị và mọi đồng cấu đại số đều được giả sử là có đơn vị.*

#### Mệnh đề 9 {#alg-iii-s10-prop-9 .statement}

*Cho $A, B$ là hai $K$-đại số phân bậc, $E$ là một $(A, A)$-song môđun và $F$ là một $(B, B)$-song môđun phân bậc; giả sử $\rho : A \to B$ là một đồng cấu đại số phân bậc và $\theta : E \to F$ là một $A$-đồng cấu phân bậc của các $A$-song môđun (đối với $\rho$), bậc 0. Khi đó:*

*(i)* *Với mọi $\varepsilon$-đạo hàm $d' : B \to F$, $d' \circ \rho : A \to \rho^*(F)$ là một $\varepsilon$-đạo hàm cùng bậc.*
*(ii)* *Với mọi $\varepsilon$-đạo hàm $d : A \to E$, $\theta \circ d : A \to \rho^*(F)$ là một $\varepsilon$-đạo hàm cùng bậc.*

Hai mệnh đề này suy ra ngay lập tức từ các hệ thức
$$
d'(\rho(xy)) = d'(\rho(x)\rho(y)) = d'(\rho(x))\rho(y) + \varepsilon_{\delta', \xi}\rho(x)d'(\rho(y))
$$
$$
\theta(d(xy)) = \theta((dx)y + \varepsilon_{\delta, \xi}x(dy)) = \theta(dx)\rho(y) + \varepsilon_{\delta, \xi}\rho(x)\theta(dy)
$$
với $x \in A$ thuần nhất bậc $\xi$ và $y \in A$, $\delta$ và $\delta'$ chỉ các bậc tương ứng của $d$ và $d'$.

#### Hệ quả {#alg-iii-s10-n7-cor-1 .statement}

*Cho $S$ là một hệ sinh của đại số $A$. Để có $d' \circ \rho = \theta \circ d$, điều kiện cần và đủ là $d'(\rho(x)) = \theta(d(x))$ với mọi $x \in S$.*

Đây là một hệ quả ngay lập tức của Mệnh đề 9 và no. 5, Hệ quả của Mệnh đề 3.

Trong các điều kiện của Mệnh đề 9, ta biết rằng $B$ có (thông qua $\rho$) một cấu trúc song môđun $(A, A)$ (II, § 1, no. 14, *Ví dụ 1*).

#### Mệnh đề 10 {#alg-iii-s10-prop-10 .statement}

*Trong các điều kiện của Mệnh đề 9, để một $\varepsilon$-đạo hàm $d' : B \to F$ là $A$-tuyến tính đối với các cấu trúc A-môđun trái (tương ứng phải) trên $B$ và $\rho^*(F)$, điều kiện cần và đủ là $d'$ bằng không trên đại số con $\rho(A)$ của $B$.*

Ta thực hiện chứng minh cho các cấu trúc A-môđun trái. Với $a \in A, b \in B$,
$$
d'(\rho(a)b) = d'(\rho(a))b + \rho(a)d'b
$$
và do đó nếu $d' \circ \rho = 0$, thì $d'$ là tuyến tính đối với các cấu trúc A-môđun trái trên B và $\rho^*(F)$. Ngược lại, nếu đúng như vậy, thì đặc biệt
$$
d'(\rho(a)) = d'(\rho(a).1) = \rho(a)d'(1) = 0
$$
(no. 5, Mệnh đề 3).

Đặc biệt, ký hiệu $D_K(B, F)$ là K-môđun các đạo hàm từ B vào F (no. 2); những đạo hàm trong số đó là A-tuyến tính, nói cách khác những đạo hàm bằng không trên $\rho(A)$, tạo thành một môđun con trên K của $D_K(B, F)$, ký hiệu là $D_{A,\rho}(B, F)$ hoặc đơn giản là $D_A(B, F)$ ($D_K(B, F) = D_{K,\phi}(B, F)$ một cách hiển nhiên, trong đó $\phi : K \to B$ là đồng cấu xác định cấu trúc đại số trên K của B).

Bây giờ cho A, B, C là ba đại số trên K phân bậc, $\rho : A \to B, \sigma : B \to C$ là hai đồng cấu đại số phân bậc và G là một song môđun $(C, C)$ phân bậc; nếu $D_A(B, G)$, $D_B(C, G)$ và $D_A(C, G)$ chỉ các K-môđun tương ứng $D_{A,\rho}(B, \sigma_*(G))$, $D_{B,\sigma}(C, G)$ và $D_{A,\sigma \circ \rho}(C, G)$, thì $D_B(C, G)$ rõ ràng là một môđun con trên K của $D_A(C, G)$ vì $\sigma(\rho(A)) \subset \sigma(B)$.

#### Mệnh đề 11 {#alg-iii-s10-prop-11 .statement}

*Trong các điều kiện trên, có một dãy khớp các K-đồng cấu*
$$
0 \to D_B(C, G) \xrightarrow{u} D_A(C, G) \xrightarrow{v} D_A(B, G)
$$
*trong đó u là đơn ánh chính tắc và v là đồng cấu $d \mapsto d \circ \sigma$* (Mệnh đề 9).

Hạt nhân của v là tập hợp các đạo hàm $d : C \to G$ sao cho $d(\sigma(b)) = 0$ với mọi $b \in B$, điều này chính xác là ảnh của u.

### 8. QUAN HỆ GIỮA CÁC ĐẠO HÀM VÀ CÁC ĐỒNG CẤU ĐẠI SỐ

Trong số này, ta lại giả sử rằng *Trường hợp (II)* của no. 2 được thỏa mãn và đại số trên K phân bậc A không được giả thiết là kết hợp. Cho một phần tử $\delta \in \Delta$, xét K-môđun phân bậc E($\delta$) (II, § 11, no. 2) sao cho
$$
(E(\delta))_\mu = E_{\mu+\delta}
$$
với mọi $\mu \in \Delta$. Ta định nghĩa trên K-môđun phân bậc $A \oplus E(\delta)$ một cấu trúc *đại số trên K phân bậc* bằng cách đặt, với mọi phần tử thuần nhất $a \in A$ và các phần tử tùy ý $a' \in A, x, x'$ trong $E(\delta)$
$$
(a, x)(a', x') = (aa', x.a' + \varepsilon_{\delta, \deg(a)} a.x');
$$
việc kiểm tra rằng phép nhân này xác định một cấu trúc vành phân bậc là ngay lập tức.

Phép chiếu $p : (a, x) \mapsto a$ được gọi là phép tăng cường của đại số $A \oplus E(\delta)$ và là một đồng cấu đại số phân bậc. Các ánh xạ K-tuyến tính phân bậc $g : A \to A \oplus E(\delta)$ bậc 0 sao cho hợp thành

$$
A \xrightarrow{g} A \oplus E(\delta) \xrightarrow{p} A
$$

là đồng nhất ánh xạ $1_A$ là các ánh xạ có dạng $x \mapsto (x, f(x))$, trong đó $f : A \to E$ là một ánh xạ K-tuyến tính phân bậc bậc $\delta$.

#### Mệnh đề 12 {#alg-iii-s10-prop-12 .statement}

*Điều kiện cần và đủ để một ánh xạ K-tuyến tính phân bậc $f : A \to E$ bậc $\delta$ là một $\varepsilon$-đạo hàm là ánh xạ $x \mapsto (x, f(x))$ từ A vào $A \oplus E(\delta)$ là một đồng cấu đại số trên K phân bậc.*

Dùng thực tế rằng với $x$ thuần nhất trong $A$ và $y \in A$

$$
(xy, f(xy)) = (x, f(x)).(y, f(y)),
$$

ta thu được, có tính đến (28), quan hệ tương đương

$$
f(xy) = f(x).y + \varepsilon_{\delta, \deg(x)} x.f(y),
$$

do đó có mệnh đề.

#### Mệnh đề 13 {#alg-iii-s10-prop-13 .statement}

*Điều kiện cần và đủ để đại số $A \oplus E(\delta)$ là kết hợp và có đơn vị là $A$ kết hợp và có đơn vị, và các ánh xạ $(a, x) \mapsto a.x$ và $(a, x) \mapsto x.a$ xác định trên $E$ một cấu trúc song môđun $(A, A)$; khi đó phần tử đơn vị của $A \oplus E(\delta)$ là $(1, 0)$.*

Nếu một phần tử $(u, m) \in A \oplus E(\delta)$ được viết là phần tử đơn vị của đại số này, thì ngay lập tức thấy rằng $u$ phải là phần tử đơn vị của $A$; viết $(u, m).(0, x) = (0, x).(u, m) = (0, x)$, ta thu được $u.x = x.u = x$ với $x \in E$ và, viết $(u, m).(u, 0) = (u, 0).(u, m) = (u, 0)$, ta thu được $m = 0$. Việc $A$ là kết hợp khi $A \oplus E(\delta)$ kết hợp suy ra từ तथ्य rằng phép tăng cường là một đồng cấu toàn ánh. Điều kiện $(x.a').a'' = x.(a'.a'')$ khi đó tương đương với $((0, x)(a', 0))(a'', 0) = (0, x)((a', 0)(a'', 0))$ và tương tự điều kiện $a.(a'.x) = (a.a').x$ tương đương với

$$
(a, 0)((a', 0)(0, x)) = ((a, 0)(a', 0))(0, x);
$$

cuối cùng điều kiện $a.(x.a') = (a.x).a'$ tương đương với

$$
(a, 0)((0, x)(a', 0)) = ((a, 0)(0, x))(a', 0).
$$

### 9. MỞ RỘNG CÁC ĐẠO HÀM

#### Mệnh đề 14 {#alg-iii-s10-prop-14 .statement}

*Cho $A$ là một vành giao hoán, $M$ là một $A$-môđun, $B$ là $A$-đại số $T(M)$ (resp. $S(M)$, resp. $\Lambda(M)$) và $E$ là một $(B, B)$-song môđun. Cho $d_0 : A \to E$ là một đạo hàm của vành $\mathbf{A}$ vào $\mathbf{A}$-môđun $\mathbf{E}$ và $d_1 : M \to \mathbf{E}$ là một đồng cấu nhóm cộng sao cho, với mọi $a \in \mathbf{A}$ và mọi $x \in M$,

$$
(29) \quad d_1(ax) = ad_1(x) + d_0(a) \cdot x,
$$

và thêm nữa, khi $B = S(M)$,

$$
(30) \quad x \cdot d_1(y) + d_1(x) \cdot y = y \cdot d_1(x) + d_1(y) \cdot x
$$

với mọi $x, y$ trong $M$, và, khi $B = \bigwedge(M)$,

$$
(31) \quad x \cdot d_1(x) + d_1(x) \cdot x = 0
$$

với mọi $x \in M$. Khi đó tồn tại duy nhất một đạo hàm $d$ của $B$ (được xét như một $\mathbf{Z}$-đại số) vào $(B, B)$-song môđun $\mathbf{E}$ sao cho $d|_{\mathbf{A}} = d_0$ và $d|_{M} = d_1$.

Ta đặt trên $\mathbf{Z}$-môđun $B \oplus \mathbf{E}$ cấu trúc $\mathbf{Z}$-đại số kết hợp được xác định bởi

$$
(b, t)(b', t') = (bb', bt' + tb')
$$

mà có $(1, 0)$ làm phần tử đơn vị (no. 8, Mệnh đề 13). Dưới đơn ánh chính tắc $t \mapsto (0, t)$, $\mathbf{E}$ được đồng nhất với một iđêan hai phía của $B \oplus \mathbf{E}$ sao cho $\mathbf{E}^2 = \{0\}$. Mặt khác, ánh xạ $h_0 : B \oplus \mathbf{E}$ xác định bởi $h_0(a) = (a, d_0(a))$ là một đồng cấu vành có đơn vị (no. 8, Mệnh đề 12); qua ánh xạ này, $B \oplus \mathbf{E}$ khi đó trở thành một $\mathbf{A}$-đại số. Hơn nữa, nếu với mọi $x \in M$, ta viết $h_1(x) = (x, d_1(x))$, thì từ định nghĩa của $h_0$ và (29) suy ra rằng $h_1(ax) = h_0(a)h_1(x)$; nói cách khác, $h_1$ là một ánh xạ $\mathbf{A}$-tuyến tính từ $M$ vào $B \oplus \mathbf{E}$. Khi đó tồn tại một và chỉ một đồng cấu đại số $\mathbf{A}$, $h : B \to B \oplus \mathbf{E}$ sao cho $h|_M = h_1$ (và tất yếu $h|_{\mathbf{A}} = h_0$): thật vậy, nếu $B = T(M)$, điều này suy ra từ $§ 5$, no. 1, Mệnh đề 1; nếu $B = S(M)$, điều kiện (30) cho thấy rằng $h(x)h(y) = h(y)h(x)$ với mọi $x, y$ trong $M$ và kết luận suy ra từ $§ 6$, no. 1, Mệnh đề 2; sau cùng nếu $B = \bigwedge(M)$, điều kiện (31) cho thấy rằng $(h(x))^2 = 0$ với mọi $x \in M$, vì $x \wedge x = 0$ và kết luận suy ra từ $§ 7$, no. 1, Mệnh đề 1. Đồng cấu $h$ có tính chất là hợp thành $p \circ h : B \to B$ với phép tăng cường $\rho : B \oplus \mathbf{E} \to B$ là đồng nhất $l_B$, vì $p \circ h$ và $l_B$ trùng nhau theo định nghĩa trên các phần tử của $\mathbf{A}$ và các phần tử của $M$ và tập hợp các phần tử ấy là một hệ sinh của $B$. Do đó ta có thể viết $h(b) = (b, d(b))$ với mọi $b \in B$ và ánh xạ $b \mapsto d(b)$ từ $B$ vào $\mathbf{E}$ là một đạo hàm có các tính chất đã yêu cầu, theo Mệnh đề 12 của no. 8.

#### Hệ quả {#alg-iii-s10-n9-cor-1 .statement}

*Cho $M$ là một K-môđun phân bậc kiểu $\Delta$; các K-đại số $T(M)$, $S(M)$ và $\bigwedge(M)$ được cho các phân bậc tương ứng kiểu $\Delta' = \Delta \times \mathbf{Z}$ ($§ 5$, no. 5, Proposition 7, $§ 6$, no. 6, Proposition 10 và $§ 7$, no. 7, Proposition 11). Mặt khác $M$ được cho phân bậc kiểu $\Delta'$ sao cho $M_{\alpha, 1} = M_{\alpha}$ với mọi $\alpha \in \Delta$ và $M_{\alpha, n} = \{0\}$ với $\alpha \in \Delta$ và $n \neq 1$. Cho $\varepsilon'$ là một nhân tử giao hoán trên $\Delta'$.*

(i) Cho E là một $\mathbf{T}(M)$-song môđun phân bậc (trái và phải) kiểu $\Delta'$; với mọi $\delta \in \Delta$ và mọi số nguyên $n \in \mathbf{Z}$, mọi ánh xạ K-tuyến tính phân bậc $f : M \to E$ bậc $\delta_1' = (\delta, n)$ đều có thể được mở rộng duy nhất thành một $\varepsilon'$-đạo hàm $d : \mathbf{T}(M) \to E$ bậc $\delta'$.

(ii) Cho E là một $S(M)$-môđun phân bậc kiểu $\Delta'$; điều kiện cần và đủ để một ánh xạ K-tuyến tính phân bậc $f : M \to E$ bậc $\delta'$ có thể được mở rộng thành một $\varepsilon'$-đạo hàm $d : S(M) \to E$ bậc $\delta'$ là, với mọi cặp có thứ tự $(x, y)$ gồm các phần tử thuần nhất của M,

$$
x . f(y) + \varepsilon_{\delta', (\deg(y), 1)} y . f(x) = y . f(x) + \varepsilon_{\delta', (\deg(x), 1)} x . f(y).
$$

$\varepsilon'$-đạo hàm d khi đó là duy nhất.

(iii) Cho E là một $\Lambda(M)$-song môđun phân bậc (trái và phải) kiểu $\Delta'$; điều kiện cần và đủ để một ánh xạ K-tuyến tính phân bậc $f : M \to E$ bậc $\delta'$ có thể được mở rộng thành một $\varepsilon'$-đạo hàm

$$
d : \Lambda(M) \to E
$$

bậc $\delta'$ là, với mọi phần tử thuần nhất x của M,

$$
x . f(x) + \varepsilon_{\delta', (\deg(x), 1)} f(x) . x = 0.
$$

$\varepsilon'$-đạo hàm d khi đó là duy nhất.

Nhận xét 2 của no. 2 được áp dụng với một trong các luật B-môđun ngoài trên E (với B bằng $\mathbf{T}(M)$, $S(M)$ hoặc $\Lambda(M)$) được sửa đổi; luật ngoài được sửa đổi như vậy vẫn là, theo (1) (no. 1), một luật B-môđun và luật B-môđun do đó thu được trên E vẫn tương thích với cấu trúc B-môđun kia. Khi đó chỉ cần áp dụng Mệnh đề 14 với $A = K$ và $d_0 = 0$.

Ví dụ (1). Trong việc áp dụng Mệnh đề 14 hãy chú ý rằng nếu $d_0 = 0$ thì điều kiện (29) đơn giản chỉ có nghĩa là $d_1$ là A-tuyến tính. Đặc biệt, nếu ta lấy $E = B$ và cấu trúc song môđun (B, B) dẫn xuất từ cấu trúc vành trên B, thì các điều kiện (30) và (31) tự động được thỏa mãn khi lấy $d_1$ là hợp thành của một tự đồng cấu s của M với đơn ánh chính tắc $M \to B$; điều này là hiển nhiên đối với (30) vì $S(M)$ là giao hoán, còn đối với (31) thì điều này suy ra từ thực tế là x và $s(x)$ có bậc 1 trong $\Lambda(M)$. Do đó thấy rằng mọi tự đồng cấu s của M đều có thể được mở rộng duy nhất thành một đạo hàm $D_s$ của $\mathbf{T}(M)$ (resp. $S(M)$, resp. $\Lambda(M)$), có bậc 0. Hơn nữa, với hai tự đồng cấu s, t của M,

$$
[D_s, D_t] = D_{[s, t]}
$$

vì hai vế đều là các đạo hàm của $\mathbf{T}(M)$ (resp. $S(M)$, resp. $\Lambda(M)$) trùng với $[s, t]$ trên M.

Biểu thức của $D_s$ thu được bằng cách dùng công thức (21) của no. 5, công thức này lần lượt cho, với $x_1, x_2, \ldots, x_n$ trong $M$,

$$
\begin{cases}
D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n) \\
\phantom{D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n)} = \sum_{i=1}^n x_1 \otimes \cdots \otimes x_{i-1} \otimes s(x_i) \otimes x_{i+1} \otimes \cdots \otimes x_n \\
D_s(x_1 x_2 \ldots x_n) = \sum_{i=1}^n x_1 \ldots x_{i-1} s(x_i) x_{i+1} \ldots x_n \\
D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \\
\phantom{D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n)} = \sum_{i=1}^n x_1 \wedge \cdots \wedge x_{i-1} \wedge s(x_i) \wedge x_{i+1} \wedge \cdots \wedge x_n.
\end{cases}
$$

Trong trường hợp của đại số $\Lambda(M)$, có cách giải thích sau đây về $D_s$:

#### Mệnh đề 15 {#alg-iii-s10-prop-15 .statement}

*Nếu $M$ là một K-môđun tự do hạng hữu hạn $n$, thì với mọi tự đồng cấu $s$ của $M$, hạn chế của đạo hàm $D_s$ lên $\Lambda^n(M)$ là phép vị tự có tỷ số $\operatorname{Tr}(s)$.*

Lấy $(e_j)_{1 \leq j \leq n}$ là một cơ sở của $M$ và đặt $e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$. Nếu
$$
s(e_j) = \sum_{k=1}^n \alpha_{jk} e_k,
$$
thì công thức thứ ba trong (36) cho
$$
D_s(e) = \sum_{i=1}^n e_1 \wedge \cdots \wedge e_{i-1} \wedge s(e_i) \wedge e_{i+1} \wedge \cdots \wedge e_n = \left( \sum_{j=1}^n \alpha_{jj} \right) e.
$$

*Ví dụ (2).* Trong Hệ quả của Mệnh đề 14, phần (iii), lấy $\Delta = \{0\}$, khi đó phân bậc trên $\Lambda(M)$ là phân bậc thông thường kiểu $\mathbf{Z}$; mặt khác lấy $\varepsilon(p, q) = (-1)^{pq}$. Khi đó, với mọi dạng tuyến tính $x^* \in M^*$ trên $M$, $x \mapsto \langle x, x^* \rangle$ là một ánh xạ K-tuyến tính phân bậc bậc $-1$ từ $M$ vào $\Lambda(M)$ thỏa mãn quan hệ (34); khi đó tồn tại một *phản đạo hàm* $i(x^*)$ của $\Lambda(M)$, bậc $-1$, sao cho (nhờ công thức (21) của no. 5)
$$
i(x^*)(x_1 \wedge \cdots \wedge x_n)
= \sum_{i=1}^n (-1)^{i-1} \langle x_i, x^* \rangle x_1 \wedge \cdots \wedge x_{i-1} \wedge x_{i+1} \wedge \cdots \wedge x_n
$$
và đây là một trường hợp riêng của tích nội sẽ được định nghĩa trong § 11, no. 9, công thức (68).

#### Mệnh đề 16 {#alg-iii-s10-prop-16 .statement}

*Cho $A$ là một K-đại số giao hoán, $M_i$ ($1 \leq i \leq n$) và $P$ là các A-môđun và $H$ là A-môđun các ánh xạ A-đa tuyến tính của $M_1 \times M_2 \times \cdots \times M_n$* vào P. Giả sử cho một K-đạo hàm $d_0 : A \to A$ của đại số A, với mỗi i, một ánh xạ K-tuyến tính $d_i : M_i \to M_i$ và một ánh xạ K-tuyến tính $D : P \to P$, sao cho, với $1 \leq i \leq n$, $(d_0, d_i, d_i)$ là một K-đạo hàm của $(A, M_i, M_i)$ vào chính nó và $(d_0, D, D)$ là một K-đạo hàm của $(A, P, P)$ vào chính nó. Khi đó tồn tại một ánh xạ K-tuyến tính $D' : H \to H$ sao cho $(d_0, D', D')$ là một K-đạo hàm của $(A, H, H)$ vào chính nó và

(37) $D(f(x_1, \ldots, x_n))$

$$
= (D'f)(x_1, \ldots, x_n) + \sum_{i=1}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$

với mọi $x_i \in M_i$ với $1 \leq i \leq n$ và $f \in H$.

Ta chỉ ra rằng với $f \in H$, ánh xạ $D'f$ của $M_1 \times M_2 \times \cdots \times M_n$ vào P được xác định bởi (37) là A-đa tuyến tính. Với $a \in A$,

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

và $d_1(ax_1) = (d_0a)x_1 + a.d_1x_1$, suy ra

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

điều này chứng minh mệnh đề.

#### Ví dụ {#alg-iii-s10-n9-exa-1 .statement}

(3) Áp dụng Mệnh đề 16 cho trường hợp $n = 1$, $M_1 = M$, $P = A$, khi đó $H = M^*$, đối ngẫu của M, và thấy rằng từ một K-đạo hàm $(d_0, d, d')$ của $(A, M, M)$ suy ra một K-đạo hàm $(d_0, d^*, d^*)$ của $(A, M^*, M^*)$ sao cho

(38) $d_0\langle m, m^*\rangle = \langle dm, m^*\rangle + \langle m, d^*m^*\rangle$

với $m \in M$ và $m^* \in M^*$. Khi đó ánh xạ K-tuyến tính của $M \oplus M^*$ vào chính nó mà bằng $d$ trên $M$ và bằng $d^*$ trên $M^*$ thỏa mãn điều kiện (29) và do đó có một đạo hàm $K$ $D$ của $K$-đại số $T(M \oplus M^*)$, mà hạn chế thành $d_0$ trên $A$, thành $d$ trên $M$ và thành $d^*$ trên $M^*$. Hạn chế $d_J^I$ của $D$ lên A-môđun con $T_J^I(M)$ của $T(M \oplus M^*)$ ($§ 5$, no. 6) là một tự đồng cấu $K$ của $T_J^I(M)$ sao cho $(d_0, d_J^I, d_J^I)$ là một đạo hàm $K$ của $(A, T_J^I(M), T_J^I(M))$. Hơn nữa, với $i \in I, j \in J$, nếu ta viết $I' = I - \{i\}, J' = J - \{j\}$, thì ngay lập tức kiểm tra được rằng đối với phép co $c_j^i$ ($§ 5$, no. 6)

$$
c_j^i(d_J^I(z)) = d_{J'}^{I'}(c_j^i(z)) \quad \text{với mọi } z \in T_J^I(M).
$$

(4) Cho $M_i$ ($1 \leq i \leq 3$) là ba A-môđun và, với mỗi $i$, giả sử rằng $(d_0, d_i, d_i)$ là một đạo hàm của $(A, M_i, M_i)$; lại áp dụng Mệnh đề 16 cho $n = 1$, ta dẫn xuất được, với mỗi cặp có thứ tự $(i, j)$, một đạo hàm $(d_0, d_{ij}, d_{ij})$ của $(A, H_{ij}, H_{ij})$, trong đó $H_{ij} = \operatorname{Hom}_A(M_i, M_j)$. Với ký hiệu này, với $u \in \operatorname{Hom}_A(M_1, M_2)$ và $v \in \operatorname{Hom}_A(M_2, M_3)$,

$$
d_{13}(v \circ u) = (d_{23}v) \circ u + v \circ (d_{12}u)
$$
như được kiểm tra ngay lập tức từ các định nghĩa.

### 10. BÀI TOÁN PHỔ QUÁT ĐỐI VỚI CÁC ĐẠO HÀM; TRƯỜNG HỢP KHÔNG GIAO HOÁN

Trong toàn bộ phần còn lại của $§ 10$ mọi đại số đều được giả sử là kết hợp và có đơn vị và mọi đồng cấu đại số đều được giả sử là có đơn vị.

Cho $A$ là một $K$-đại số; tích tenxơ $A \otimes_K A$ có một cách chính tắc một cấu trúc song môđun $(A, A)$, dưới đó

$$
x . (u \otimes v) . y = (xu) \otimes (vy)
$$
với mọi $x, y, u, v$ trong $A$ ($§ 4$, no. 3, Ví dụ 2). Ánh xạ $K$-tuyến tính $m : A \otimes_K A \to A$ tương ứng với phép nhân trong $A$ (và do đó thỏa mãn $m(x \otimes y) = xy$) là một đồng cấu song môđun $(A, A)$; vì vậy hạt nhân $I$ của nó là một môđun con song của $A \otimes_K A$.

#### Bổ đề 1 {#alg-iii-s10-lem-1 .statement}

*Ánh xạ $\delta_A : x \mapsto x \otimes 1 - 1 \otimes x$ là một đạo hàm $K$ của $A$ vào $I$ và $I$ được sinh, như một A-môđun trái, bởi ảnh của $\delta_A$.*

Mệnh đề thứ nhất suy ra từ việc

$$
(xy) \otimes 1 - 1 \otimes (xy) = (x \otimes 1 - 1 \otimes x) . y + x . (y \otimes 1 - 1 \otimes y)
$$
theo (40). Mặt khác, nếu phần tử $\sum_i x_i \otimes y_i$ (với $x_i, y_i$ trong $A$) thuộc $I$, thì theo định nghĩa $\sum_i x_i y_i = 0$ và do đó

$$
\sum_i (x_i \otimes y_i) = \sum_i x_i (1 \otimes y_i - y_i \otimes 1)
$$
theo (40), điều này hoàn thành chứng minh của bổ đề.

#### Mệnh đề 17 {#alg-iii-s10-prop-17 .statement}

*Đạo hàm* $\delta_A$ *có tính chất phổ quát sau*: với mọi song môđun $(A, A)$ $E$ và mọi đạo hàm $K$ $d : A \to E$, tồn tại một và chỉ một đồng cấu song môđun $(A, A)$ $f : I \to E$ sao cho $d = f \circ \delta_A$.

Trước hết hãy chú ý rằng, với mọi đồng cấu song môđun $(A, A)$ $f : I \to E$, $f \circ \delta_A$ là một đạo hàm (no. 7, Mệnh đề 9). Ngược lại, cho $d : A \to E$ là một đạo hàm K; trước hết ta chứng minh rằng nếu tồn tại một đồng cấu song môđun $(A, A)$ $f : I \to E$ sao cho $d = f \circ \delta_A$, thì $f$ *được xác định duy nhất* bởi điều kiện này vì định nghĩa của $\delta_A$ cho

$$
f(x \otimes 1 - 1 \otimes x) = dx
$$

và mệnh đề của ta suy ra từ việc ảnh của $\delta_A$ đã sinh ra I như một A-môđun trái (Bổ đề 1): do đó tất yếu có

$$
f\left( \sum_i x_i \otimes y_i \right) = \sum_i x_i \cdot f(1 \otimes y_i - y_i \otimes 1) = -\sum_i x_i \cdot dy_i.
$$

Ngược lại, vì ánh xạ $(x, y) \mapsto -x \cdot dy$ từ $A \times A$ vào $E$ là $K$-song tuyến tính, nên tồn tại một và chỉ một ánh xạ $K$-tuyến tính $g : A \otimes_K A \to E$ sao cho $g(x \otimes y) = -x \cdot dy$; chỉ cần kiểm tra rằng hạn chế $f$ của $g$ lên $I$ là A-tuyến tính đối với các cấu trúc A-môđun trái và phải. Mệnh đề thứ nhất là hiển nhiên vì $(xx') \cdot dy = x \cdot (x' \cdot dy)$; để chứng minh mệnh đề thứ hai, hãy chú ý rằng, nếu $\sum_i x_i \otimes y_i \in I$ và $x \in A$, thì

$$
\sum_i x_i \cdot d(y_i x) = \sum_i x_i \cdot dy_i \cdot x + \sum_i (x_i y_i) \cdot dx
$$

nhưng vì $\sum_i x_i y_i = 0$ theo định nghĩa của $I$, điều này hoàn tất chứng minh.

Như vậy ta đã xác định một *đẳng cấu* *chính tắc* của các $K$-môđun $f \mapsto f \circ \delta_A$

$$
\operatorname{Hom}_{(A, A)}(I, E) \to D_K(A, E)
$$

trong đó vế trái là $K$-môđun các đồng cấu song môđun $(A, A)$ từ $A$ vào $E$.

### 11. BÀI TOÁN PHỔ QUÁT ĐỐI VỚI CÁC ĐẠO HÀM; TRƯỜNG HỢP GIAO HOÁN

Bây giờ giả sử rằng $A$ là một $K$-đại số *giao hoán* và $E$ là một $A$-*môđun*; $E$ có thể được xét như một song môđun $(A, A)$ mà hai luật ngoài của nó trùng với luật môđun $A$ đã cho. Mặt khác, cấu trúc song môđun $(A, A)$ trên $A \otimes_K A$ trùng với cấu trúc môđun $(A \otimes_K A)$ của nó xuất phát từ cấu trúc *vành giao hoán* trên $A \otimes_K A$, vì trong trường hợp này, với $x, y, u, v$ thuộc $A$,

$$
x \cdot (u \otimes v) \cdot y = (xu) \otimes (vy) = (xu) \otimes (yv) = (x \otimes y)(u \otimes v).
$$

Do đó hạt nhân $\mathfrak{J}$ của $m$ trong trường hợp này là một *iđêan* của vành $A \otimes_K A$ và, vì $m : A \otimes_K A \to A$ là toàn ánh, $(A \otimes_K A)/\mathfrak{J}$ đẳng cấu với $A$; nếu cũng xét $E$ như một môđun $(A \otimes_K A)$ посредством $m$ (nói cách khác là môđun $(A \otimes_K A)$ $m_*(E)$), thì các đồng cấu *song môđun* $(A, A)$ $\mathfrak{J} \to E$ được đồng nhất với các đồng cấu *môđun* $(A \otimes_K A)$ $\mathfrak{J} \to E$ (§ 4, no. 3), nói cách khác có một đẳng cấu chính tắc của các $K$-môđun.

$$
\operatorname{Hom}_{(A, A)}(\mathfrak{J}, E) \to \operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E).
$$

Mặt khác, $\mathfrak{J}E = \{0\}$, vì các phần tử $1 \otimes x - x \otimes 1$ sinh ra $\mathfrak{J}$ như một môđun $(A \otimes_K A)$ (no. 10, Bổ đề 1) và, với mọi $z \in E$,

$$
(1 \otimes x - x \otimes 1)z = 0
$$

theo định nghĩa của cấu trúc môđun $(A \otimes_K A)$ trên $E$. Vì $\mathfrak{J}$ được chứa trong linh hóa tử của môđun $(A \otimes_K A)$ $E$ và cấu trúc môđun $((A \otimes_K A)/\mathfrak{J})$ trên $E$ theo định nghĩa chính là cấu trúc môđun $A$ ban đầu đã cho trên $E$, nên, có tính đến đẳng cấu chính tắc của

$$
\mathfrak{J} \otimes_K ((A \otimes_K A)/\mathfrak{J})
$$

lên $\mathfrak{J}/\mathfrak{J}^2$ (§ 4, no. 1, Hệ quả 1 của Mệnh đề 1), có một đẳng cấu chính tắc của các $K$-môđun

$$
\operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E) \to \operatorname{Hom}_A(\mathfrak{J}/\mathfrak{J}^2, E).
$$

Có tính đến Mệnh đề 17 của no. 10, ta thấy rằng ta đã chứng minh mệnh đề sau:

#### Mệnh đề 18 {#alg-iii-s10-prop-18 .statement}

*Cho $A$ là một $K$-đại số giao hoán và $\mathfrak{J}$ là iđêan bằng hạt nhân của đồng cấu chính tắc toàn ánh $m : A \otimes_K A \to A$, sao cho $A$ đẳng cấu với $(A \otimes_K A)/\mathfrak{J}$ và $\mathfrak{J}/\mathfrak{J}^2$ một cách chính tắc có cấu trúc $A$-môđun. Gọi $d_{A/K} : A \to I/I^2$ là ánh xạ $K$-tuyến tính gán cho mỗi $x \in A$ lớp của $x \otimes 1 - 1 \otimes x$ modulo $\mathfrak{J}^2$. Ánh xạ $d_{A/K}$ là một $K$-đạo hàm và, với mọi $A$-môđun $E$ và mọi $K$-đạo hàm $D : A \to E$, tồn tại một và chỉ một ánh xạ $A$-tuyến tính $g : \mathfrak{J}/\mathfrak{J}^2 \to E$ sao cho $D = g \circ d_{A/K}$.*

#### Ví dụ {#alg-iii-s10-n11-exa-1 .statement}

Cho M là một K-môđun; từ Mệnh đề 14 của no. 9 suy ra rằng với mọi S(M)-môđun E, ánh xạ D ↦ D | M xác định một đẳng cấu S(M)-môđun từ D_K(S(M), E) lên Hom_K(M, E); mặt khác, vì E là một S(M)-môđun, Hom_K(M, E) đẳng cấu chính tắc với

$$
\operatorname{Hom}_{S(M)}(M \otimes_K S(M), E),
$$

mọi đồng cấu K của M vào E đều được biểu diễn duy nhất dưới dạng $x \mapsto h(x \otimes 1)$, trong đó

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E)
$$

(II, § 5, no. 1). Gọi D_0 là $K$-đạo hàm $S(M) \to M \otimes_K S(M)$ mà hạn chế của nó trên M là đồng cấu chính tắc $x \mapsto x \otimes 1$; do đó mọi $K$-đạo hàm D : S(M) → E đều có thể được viết một cách duy nhất dưới dạng $h \circ D_0$ với

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E).
$$

Do tính duy nhất của một nghiệm của một bài toán ánh xạ phổ quát, suy ra tồn tại một đẳng cấu S(M)-môđun duy nhất

$$
\omega : M \otimes_K S(M) \to \Omega_K(S(M))
$$

sao cho $D_0 \circ \omega = d_{S(M)/K}$; nói cách khác, với mọi $x \in M$, $\omega(x \otimes 1) = dx$.

Đặc biệt, *nếu M là một K-môđun tự do với cơ sở* $(e_\lambda)_{\lambda \in L}$, thì $\Omega_K(S(M))$ *là một S(M)-môđun tự do có cơ sở là tập hợp các vi phân* $de_\lambda$. Xét riêng trường hợp $L = \{1, n\}$, khi đó S(M) được đồng nhất với đại số đa thức $K[X_1, \ldots, X_n]$ (§ 6, no. 6); với mọi đa thức $P \in K[X_1, \ldots, X_n]$, ta có thể viết một cách duy nhất

$$
dP = \sum_{i=1}^n D_i P . dX_i
$$

với $D_i P \in K[X_1, \ldots, X_n]$ và, theo điều trên, các ánh xạ $P \mapsto D_i P$ là các *K-đạo hàm* của $K[X_1, \ldots, X_n]$ tương ứng với các dạng tọa độ trên $\Omega_K(S(M))$ đối với cơ sở $(dX_i)$; ta cũng viết $\frac{\partial P}{\partial X_i}$ thay cho $D_i P$ và gọi đó là *đạo hàm riêng* của P theo $X_i$.

### 12. CÁC TÍNH CHẤT HÀM TỬ CỦA VI PHÂN K

#### Mệnh đề 19 {#alg-iii-s10-prop-19 .statement}

*Cho*

$$
\begin{array}{ccc}
K & \xrightarrow{\rho} & K' \\
\downarrow \eta & & \downarrow \eta' \\
A & \xrightarrow{u} & A'
\end{array}
$$

*là một biểu đồ giao hoán các đồng cấu vành giao hoán*, $\eta$ (tương ứng $\eta'$) *biến*

A (tương ứng $A'$) thành một $K$-đại số (tương ứng một $K'$-đại số). Tồn tại một và chỉ một ánh xạ $A$-tuyến tính $v : \Omega_K(A) \to \Omega_{K'}(A')$ làm cho biểu đồ

$$
\begin{array}{ccc}
A & \xrightarrow{u} & A' \\
d_{A/K} \downarrow & & d_{A'/K'} \downarrow \\
\Omega_K(A) & \xrightarrow{v} & \Omega_{K'}(A')
\end{array}
$$

giao hoán.

$d_{A'/K'} \circ u$ là một $K$-đạo hàm của $A$ nhận giá trị trong $A$-môđun $\Omega_{K'}(A')$; khi đó sự tồn tại và tính duy nhất của $v$ suy ra từ Mệnh đề 18 ở no. 11.

Ánh xạ $v$ của Mệnh đề 19 sẽ được ký hiệu là $\Omega(u)$; nếu có một biểu đồ giao hoán các đồng cấu vành giao hoán

$$
\begin{array}{cccccc}
K & \xrightarrow{\sigma} & K' & \xrightarrow{\sigma'} & K'' \\
\eta \downarrow & & \eta' \downarrow & & \eta'' \downarrow \\
A & \xrightarrow{u} & A' & \xrightarrow{u'} & A''
\end{array}
$$

thì suy ra ngay lập tức từ tính duy nhất của Mệnh đề 19 rằng

$$
\Omega(u' \circ u) = \Omega(u') \circ \Omega(u).
$$

Vì $\Omega_{K'}(A')$ là một $A'$-môđun, từ $\Omega(u)$ ta suy ra một cách chính tắc một ánh xạ $A'$-tuyến tính

$$(41)$$
$$
\Omega_0(u) : \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

sao cho $\Omega(u)$ là hợp thành của $\Omega_0(u)$ và đồng cấu chính tắc $i_A : \Omega_K(A) \to \Omega_K(A) \otimes_A A'$. Với mọi $A'$-môđun $E'$, có một biểu đồ giao hoán

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

Do trong biểu đồ (42) các mũi tên thẳng đứng là song ánh, điều đó quy về việc chứng minh rằng, với mọi $A'$-môđun $E'$, đồng cấu $C(u): D \mapsto D \circ u$ trong biểu đồ (42) là song ánh (II, § 2, no. 1, Định lý 1). Bây giờ $\mathrm{Hom}(u, 1_{E'}): \mathrm{Hom}_{K'}(A \otimes_K K', E') \to \mathrm{Hom}_K(A, E')$ là một đẳng cấu (II, § 5, no. 1, Mệnh đề 1) và $C(u)$ là hạn chế của nó lên $D_{K'}(A', E')$ và do đó là đơn ánh; hơn nữa, nếu $f: A' \to E'$ là một ánh xạ $K'$-tuyến tính sao cho

$$
f \circ u: A \to E'
$$

là một $K$-đạo hàm, thì suy ra ngay lập tức từ việc $f$ là $K'$-tuyến tính và việc $f((x \otimes 1)(y \otimes 1)) = (y \otimes 1)f(x \otimes 1) + (x \otimes 1)f(y \otimes 1)$ với $x, y$ trong $A$, rằng $f$ là một $K'$-*đạo hàm*, vì các phần tử $x \otimes 1$ với $x \in A$ lập thành một hệ sinh của $K'$-môđun $A'$; điều này hoàn tất chứng minh rằng $C(u)$ là song ánh.

Từ nay về sau ta chỉ giới hạn sự chú ý vào trường hợp $\rho: K \to K'$ là *ánh xạ đồng nhất* của $K$; do đó mọi đồng cấu đại số $K$ $u: A \to B$ đều được ánh xạ thành một ánh xạ $B$-tuyến tính

$$
\Omega_0(u): \Omega_K(A) \otimes_K B \to \Omega_K(B).
$$

Mặt khác, ta có thể xét $B$-môđun các $A$-*vi phân* $\Omega_A(B)$ vì $B$ là một $A$-đại số thông qua $u$; đạo hàm chính tắc $d_{B/A}: B \to \Omega_A(B)$ vì thế *a fortiori* là một $K$-đạo hàm, nên nó phân tích duy nhất thành

$$
B \xrightarrow{d_{B/K}} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B)
$$

trong đó $\Omega_u$ là một ánh xạ $B$-tuyến tính (no. 11, Mệnh đề 18). Với mọi $B$-môđun $E$, có một biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Hom}_B(\Omega_A(B), E) & \xrightarrow{\mathrm{Hom}(\Omega_u, 1_E)} & \mathrm{Hom}_B(\Omega_K(B), E) \\
\downarrow \phi_{A,B} & & \downarrow \phi_{K,B} \\
D_A(B, E) & \xrightarrow{j_u} & D_K(B, E)
\end{array}
$$

trong đó $j_u$ là đơn ánh chính tắc (no. 7); điều này suy ra ngay lập tức từ Mệnh đề 18 của no. 11.

#### Mệnh đề 21 {#alg-iii-s10-prop-21 .statement}

*Dãy các ánh xạ $B$-tuyến tính*

$$
\Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B) \to 0
$$

*là khớp.*

Điều này quy về việc kiểm tra rằng, với mọi B-môđun E, dãy

$$
0 \to \operatorname{Hom}_B(\Omega_A(B), E) \xrightarrow{\operatorname{Hom}(\Omega_u, 1_E)} \operatorname{Hom}_B(\Omega_K(B), E) \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_E)} \operatorname{Hom}_B(\Omega_K(A) \otimes_A B, E)
$$

là khớp (II, § 2, no. 1, Định lý 1); nhưng do trong các biểu đồ giao hoán (42) và (44) các mũi tên thẳng đứng là các đẳng cấu, chỉ cần chỉ ra rằng dãy

$$
0 \longrightarrow D_A(B, E) \xrightarrow{j_u} D_K(B, E) \xrightarrow{C(u)} D_K(A, E)
$$

là khớp, mà đó chính là Mệnh đề 11 của no. 7.

Bây giờ ta xét trường hợp đồng cấu đại số trên K $u : A \to B$ là toàn ánh; nếu $\mathfrak{J}$ là hạt nhân của nó, thì B khi đó đẳng cấu với $A/\mathfrak{J}$. Ta xét hạn chế $d|_{\mathfrak{J}} : \mathfrak{J} \to \Omega_K(A)$ của đạo hàm chính tắc $d = d_{A/K}$ và ánh xạ A-tuyến tính hợp thành

$$
d' : \mathfrak{J} \xrightarrow{d|_{\mathfrak{J}}} \Omega_K(A) \xrightarrow{i_A} \Omega_K(A) \otimes_A B.
$$

Khi đó $d'(\mathfrak{J}^2) = 0$, vì, với $x, y$ trong $\mathfrak{J}$,

$$
d'(xy) = d(xy) \otimes 1 = (x.dy + y.dx) \otimes 1 = dy \otimes u(x) + dx \otimes u(y) = 0
$$

vì $u(x) = u(y) = 0$. Do đó ta suy ra từ $d'$, bằng cách chuyển qua thương, một ánh xạ A-tuyến tính

$$
\bar{d} : \mathfrak{J}/\mathfrak{J}^2 \to \Omega_K(A) \otimes_A B
$$

và vì $\mathfrak{J}$ triệt tiêu A-môđun $\mathfrak{J}/\mathfrak{J}^2$, nên $\bar{d}$ là một ánh xạ B-tuyến tính.

#### Mệnh đề 22 {#alg-iii-s10-prop-22 .statement}

*Cho $\mathfrak{J}$ là một iđêan của đại số giao hoán trên K A, $B = A/\mathfrak{J}$ và $u : A \to B$ là đồng cấu chính tắc. Khi đó dãy các ánh xạ B-tuyến tính*

$$
\mathfrak{J}/\mathfrak{J}^2 \xrightarrow{\bar{d}} \Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \to 0
$$

*là khớp.*

Chú ý rằng $\Omega_K(A) \otimes_A B$ được đồng nhất với $\Omega_K(A)/\mathfrak{J}\Omega_K(A)$ và ảnh của $\bar{d}$ là ảnh của $d(\mathfrak{J})$ trong môđun thương này; do đó thương của $\Omega_K(A) \otimes_A B$ bởi $\operatorname{Im}(\bar{d})$ được đồng nhất với thương $\Omega_K(A)/N$, trong đó N là môđun con-A sinh bởi $\mathfrak{J}\Omega_K(A)$ và $d(\mathfrak{J})$. Hơn nữa, ánh xạ hợp thành

$$
A \xrightarrow{d_{A/K}} \Omega_K(A) \longrightarrow \Omega_K(A)/N
$$

là một $K$-đạo hàm (no. 7, Mệnh đề 9) và, vì nó bằng không trên $\mathfrak{J}$ theo định nghĩa của N, nên nó xác định, khi chuyển qua thương, một $K$-đạo hàm $D_0 : B \to \Omega_K(A)/N$.

Có tính đến tính duy nhất của nghiệm của một bài toán ánh xạ phổ quát, điều này quy về việc chứng minh rằng, với mọi B-môđun E và mọi K-đạo hàm D: B → E, tồn tại duy nhất một ánh xạ B-tuyến tính g: Ω_K(A)/N → E sao cho D = g ∘ D_0. Nhưng ánh xạ hợp thành D ∘ u: A → E là một K-đạo hàm (no. 7, Mệnh đề 9) và vì thế tồn tại một và chỉ một ánh xạ A-tuyến tính f: Ω_K(A) → E sao cho f ∘ d_{A/K} = D ∘ u. Quan hệ này đã cho thấy rằng f bằng không trên d(Σ); đồng thời ΣE = {0} vì E là một B-môđun, nên f bằng không trên ΣΩ_K(A); do đó f bằng không trên N và xác định, khi chuyển qua thương, một ánh xạ B-tuyến tính g: Ω_K(A)/N → E sao cho g ∘ D_0 = D; tính duy nhất của g suy ra từ tính duy nhất của f.

Không được nghĩ rằng, ngay cả nếu u: A → B là một đơn cấu, Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) cũng là đơn ánh (Bài tập 5). Tuy nhiên ta có mệnh đề sau:

#### Mệnh đề 23 {#alg-iii-s10-prop-23 .statement}

Cho A là một đại số nguyên trên K, B là trường các phân thức của nó và u: A → B là đơn ánh chính tắc. Khi đó Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) là một đẳng cấu.

Dùng तथ्य rằng trong biểu đồ (42) các mũi tên thẳng đứng là song ánh, điều này quy về việc chứng minh rằng, với mọi không gian vectơ E trên B, ánh xạ C(u): D_K(B, E) → D_K(A, E) là song ánh. Nhưng điều này suy ra từ तथ्य rằng mọi K-đạo hàm từ A vào E đều có thể được mở rộng duy nhất thành một K-đạo hàm từ B vào E (no. 5, Mệnh đề 5).

### Bài tập {#alg-iii-s10-exercises}

Xem [bài tập của § 10](exercises/s10/).
