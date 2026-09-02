---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 10
section_title: Matrices
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 338-363, 417-424
pdf_pages: 0362-0387, 0441-0448
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF MATRICES
      page: 338
      pdf_page: 362
    - "no": 2
      title: MATRICES OVER A COMMUTATIVE GROUP
      page: 339
      pdf_page: 363
    - "no": 3
      title: MATRICES OVER A RING
      page: 341
      pdf_page: 365
    - "no": 4
      title: MATRICES AND LINEAR MAPPINGS
      page: 342
      pdf_page: 366
    - "no": 5
      title: BLOCK PRODUCTS
      page: 346
      pdf_page: 370
    - "no": 6
      title: MATRIX OF A SEMI-LINEAR MAPPING
      page: 347
      pdf_page: 371
    - "no": 7
      title: SQUARE MATRICES
      page: 349
      pdf_page: 373
    - "no": 8
      title: CHANGE OF BASES
      page: 352
      pdf_page: 376
    - "no": 9
      title: EQUIVALENT MATRICES; SIMILAR MATRICES
      page: 354
      pdf_page: 378
    - "no": 10
      title: TENSOR PRODUCT OF MATRICES OVER A COMMUTATIVE RING
      page: 356
      pdf_page: 380
    - "no": 11
      title: TRACE OF A MATRIX
      page: 358
      pdf_page: 382
    - "no": 12
      title: MATRICES OVER A FIELD
      page: 359
      pdf_page: 383
    - "no": 13
      title: EQUIVALENCE OF MATRICES OVER A FIELD
      page: 360
      pdf_page: 384
statements: 35
exercises: 12
content_sha256: b2a835f74562463b9a308557929977108ddbeec80e8e899ef145967342056a76
translated_from: content/en/alg/II/10_s10_matrices.md
source_content_sha256: a47679ba1ab8c0e078a09ebdfca77031eefe61db8ddab4faffc08a0fa8c19aa5
translation_model: gpt-5.4
translation_run: translate-vi-5f9ccca3
glossary_version: 34
glossary_terms_sha256: ae97e21d0a8a6f190faca6ef4cc5787d3cc1c91f9f653f7181508772415344a9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. MA TRẬN

### 1. ĐỊNH NGHĨA MA TRẬN

#### Định nghĩa 1 {#alg-ii-s10-def-1 .statement}

Cho $I, K, H$ là ba tập hợp; một ma trận kiểu $(I, K)$ với các phần tử trong $H$ (hoặc một ma trận kiểu $(I, K)$ trên $H$) là một họ bất kỳ $M = (m_{i\kappa})_{(i, \kappa) \in I \times K}$ gồm các phần tử của $H$ mà tập hợp chỉ số là tích $I \times K$. Với mọi $i \in I$, họ $(m_{i\kappa})_{\kappa \in K}$ được gọi là hàng của $M$ có chỉ số $i$; với mọi $\kappa \in K$, họ $(m_{i\kappa})_{i \in I}$ được gọi là cột của $M$ có chỉ số $\kappa$.

Nếu $I$ (resp. $K$) là hữu hạn, thì $M$ được gọi là ma trận có một số hữu hạn hàng (resp. cột). Tập hợp các ma trận kiểu $(I, K)$ trên $H$ được đồng nhất với tích $HI^{I \times K}$.

Các tên gọi "hàng" và "cột" xuất phát từ sự kiện là, trong trường hợp $I$ và $K$ là các khoảng $[1, p], [1, q]$ của $\mathbf{N}$, các phần tử của ma trận được hình dung như được sắp xếp thành một bảng chữ nhật gồm $p$ hàng (xếp theo phương ngang) và $q$ cột (xếp theo phương dọc):

$$
\begin{pmatrix}
m_{11} & m_{12} & \cdots & m_{1q} \\
m_{21} & m_{22} & \cdots & m_{2q} \\
\cdots & \cdots & \cdots & \cdots \\
m_{p1} & m_{p2} & \cdots & m_{pq}
\end{pmatrix}
$$

Khi $p$ và $q$ là những số nguyên cho tường minh đủ nhỏ để việc đó là khả thi, thì theo quy ước bảng trên là một ký hiệu thực sự biểu thị ma trận đang xét; ký hiệu này cho phép ta khỏi dùng các chỉ số, với sự hiểu ngầm rằng các chỉ số của một phần tử được xác định bởi vị trí của nó trong bảng; chẳng hạn, khi ta nói về ma trận

$$
\begin{pmatrix}
a & b & c \\
d & e & f
\end{pmatrix}
$$

thì ta có ý nói ma trận $(m_{ij})_{1 \leq i < 2, 1 \leq j < 3}$ sao cho

$$
m_{11} = a,\ m_{12} = b,\ m_{13} = c,\ m_{21} = d,\ m_{22} = e,\ m_{23} = f.
$$

Thay cho ma trận kiểu $([1, p], [1, q])$, ta cũng nói ma trận kiểu $(p, q)$, hoặc ma trận có $p$ hàng và $q$ cột, nếu không gây nhầm lẫn; tập hợp các ma trận kiểu $(p, q)$ trên $H$ đôi khi được ký hiệu bởi $\mathbf{M}_{p, q}(H)$.

Mọi ma trận trên $H$ mà một trong các tập hợp chỉ số $I, K$ là rỗng đều đồng nhất với họ rỗng các phần tử của $H$; nó cũng được gọi là ma trận rỗng. Khi $I = \{i_0\}$ (resp. $K = \{k_0\}$) là một tập hợp gồm một phần tử duy nhất, thì $M$ được gọi là ma trận hàng (resp. ma trận cột) và khi đó có thể bỏ chỉ số hàng (resp. cột) trong ký hiệu; khi $I$ và $K$ đều là các tập hợp có một phần tử, một ma trận kiểu $(I, K)$ thường được đồng nhất với phần tử duy nhất trong ma trận này.

Một họ con $M' = (m_{\iota \kappa})_{(\iota, \kappa) \in J \times L}$ của một ma trận $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$, mà tập hợp chỉ số là tích của một tập con $J$ của $I$ và một tập con $L$ của $K$, được gọi là một *ma trận con* của ma trận $M$; ta nói rằng nó thu được bằng cách *bỏ đi* trong $M$ các hàng có chỉ số $\iota \notin J$ và các cột có chỉ số $\kappa \notin L$; ngược lại, ta nói rằng $M$ thu được bằng cách *viền thêm* vào $M'$ các hàng có chỉ số $\iota \notin J$ và các cột có chỉ số $\kappa \notin L$.

#### Định nghĩa 2 {#alg-ii-s10-def-2 .statement}

*Ma trận chuyển vị của một ma trận* $M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times K}$, *ký hiệu bởi* $^tM$, *là ma trận* $(m'_{\kappa \iota})_{(\kappa, \iota) \in K \times I}$ *trên* $H$ *xác định bởi* $m'_{\kappa \iota} = m_{\iota \kappa}$ *với mọi* $(\iota, \kappa) \in K \times L$.

Từ định nghĩa này suy ra rằng ma trận chuyển vị của một ma trận kiểu $(I, K)$ là một ma trận kiểu $(K, I)$ và rằng

(1)
$$
^t(^tM) = M.
$$

### 2. MA TRẬN TRÊN MỘT NHÓM GIAO HOÁN

Cho $G$ là một nhóm giao hoán (được viết theo ký pháp cộng). Tập hợp các ma trận trên $G$, với các tập hợp chỉ số đã cho $I, K$, có một cấu trúc *nhóm giao hoán* vì đó là tập hợp các ánh xạ từ $I \times K$ vào $G$; nhóm này được viết theo ký pháp cộng, sao cho nếu $M = (m_{\iota \kappa})$ và $M' = (m'_{\iota \kappa})$ là hai phần tử của nó, thì
$$
M + M' = (m_{\iota \kappa} + m'_{\iota \kappa});
$$
vì vậy phần tử đơn vị của nhóm này là ma trận mà mọi phần tử đều *không* (gọi là *ma trận không*). Rõ ràng
(2)
$$
^t(M + M') = ^tM + ^tM'.
$$

Như vậy tổng của hai ma trận chỉ được xác định nếu các tập hợp chỉ số của các hàng và các cột là *cùng một* cho hai ma trận.

Cho $H', H''$ là hai tập hợp, $G$ một nhóm giao hoán (được viết theo ký pháp cộng) và $f : (h', h'') \mapsto h'h''$ một ánh xạ từ $H' \times H''$ vào $G$. Với hai ma trận
$$
M' = (m'_{ik})_{(i, k) \in I \times K}, \quad M'' = (m''_{kl})_{(k, l) \in K \times L}
$$
trên $H'$ và $H''$ tương ứng sao cho tập hợp chỉ số $K$ của các cột của $M'$ là *hữu hạn* và bằng tập hợp chỉ số của các hàng của $M''$, thì *tích của* $M'$ và $M''$ *qua* $f$, ký hiệu bởi $M'M''$ hoặc $f(M', M'')$, là ma trận
(3)
$$
\left( \sum_{k \in K} m'_{ik} m''_{kl} \right)_{(i, l) \in I \times L}
$$
trên $G$.

Định nghĩa trên giả thiết rằng tập hợp chỉ số của các cột của $M'$ bằng tập hợp chỉ số của các hàng của $M''$; đặc biệt tích $M''M'$ *không có nghĩa nếu* $I \neq L$. Trong công thức (3) các phần tử của *cùng một* hàng của $M'$ xuất hiện được nhân ở bên phải bởi các phần tử của *cùng một* cột của $M''$; phép nhân ấy được gọi là thực hiện "hàng nhân cột".

Cho $f^0$ là ánh xạ $(h'', h') \mapsto h'h''$ từ $H'' \times H'$ vào $G$; từ các định nghĩa suy ra ngay lập tức rằng
$$
t(M'M'') = tM''.tM'
$$
trong đó tích ở vế trái (tương ứng, vế phải) được tính qua $f$ (tương ứng, qua $f^0$).

Khi $H'$ và $H''$ bản thân chúng là các nhóm giao hoán (viết theo phép cộng) và $f$ là $\mathbf{Z}$-*song tuyến tính* (§ 3, no. 1), các công thức phân phối
$$
\begin{cases}
(M' + N')M'' = M'M'' + N'M'' \\
M'(M'' + N'') = M'M'' + M'N''
\end{cases}
$$
được kiểm tra ngay lập tức, với điều kiện các tập hợp chỉ số sao cho các tổng và tích xuất hiện đều được định nghĩa.

Bây giờ cho $H_1, H_2, H_3, H_{12}, H_{23}$ và $H$ là các nhóm giao hoán (viết theo phép cộng), $f_{12}:H_1 \times H_2 \to H_{12}, f_{23}:H_2 \times H_3 \to H_{23}$ là các ánh xạ và
$$
f_3:H_{12} \times H_3 \to H, \quad f_1:H_1 \times H_{23} \to H
$$
là các ánh xạ $\mathbf{Z}$-song tuyến tính; giả sử thêm rằng, với mọi $x_i \in H_i \ (i = 1, 2, 3)$
$$
f_3(f_{12}(x_1, x_2), x_3) = f_1(x_1, f_{23}(x_2, x_3))
$$
(điều này cũng có thể được viết như trên thành $(x_1 x_2)x_3 = x_1(x_2 x_3)$); khi đó, nếu $M' = (m'_{rs}), M'' = (m''_{st}), M''' = (m'''_{tu})$ lần lượt là các ma trận trên $H_1, H_2, H_3$,
$$
(M'M'')M''' = M'(M''M'''')
$$
khi các tích ở hai vế (được tính tương ứng qua $f_{12}, f_3, f_{23}$ và $f_1$) được định nghĩa; thật vậy,
$$
\sum_t \left( \sum_s m'_{rs} m''_{st} \right) m'''_{tu} = \sum_t \sum_s (m'_{rs} m''_{st}) m'''_{tu} = \sum_s \sum_t m'_{rs} (m''_{st} m'''_{tu})
$$
$$
= \sum_s m'_{rs} \left( \sum_t m''_{st} m'''_{tu} \right)
$$
do các giả thiết đã nêu.

Hai vế của (6) cũng được ký hiệu bởi $M'M''M'''$. Những quy ước tương tự được đặt ra cho các tích có hơn ba thừa số.

#### Nhận xét {#alg-ii-s10-n2-rem-1 .statement}

Các công thức trên mở rộng được cho một tình huống tổng quát hơn. Cụ thể:

(a) Giả sử $H = \bigcup_{(\iota, \kappa) \in I \times K} G_{\iota \kappa}$ trong đó mỗi $G_{\iota \kappa}$ là một nhóm giao hoán viết theo phép cộng; khi đó tổng $M + M'$ có thể được định nghĩa khi, với mỗi cặp có thứ tự $(\iota, \kappa)$, ta có $m_{\iota \kappa} \in G_{\iota \kappa}$ và $m'_{\iota \kappa} \in G_{\iota \kappa}$.

(b) Cho I, K, L là ba tập hợp với K được giả thiết là hữu hạn và cho $H' = \bigcup_{(i, k) \in I \times K} H'_{ik}$, $H'' = \bigcup_{(k, l) \in K \times L} H''_{kl}$, $H = \bigcup_{(i, l) \in I \times L} H_{il}$ là ba tập hợp; giả sử rằng mỗi $H_{il}$ là một nhóm giao hoán viết theo phép cộng và với mỗi bộ ba $(i, k, l)$ đặt
$$
f_{ikl}: H'_{ik} \times H''_{kl} \to H_{il}
$$
là một ánh xạ. Khi đó nếu $M' = (m'_{ik})_{(i, k) \in I \times K}$, $M'' = (m''_{kl})_{(k, l) \in K \times L}$ là các ma trận sao cho $m'_{ik} \in H'_{ik}$ và $m''_{kl} \in H''_{kl}$ với mọi $i, k, l$ thì ta có thể định nghĩa tích $M'M''$ qua các $f_{ikl}$. Chúng tôi để cho người đọc việc viết ra và chứng minh các công thức tương tự với (4), (5) và (6).

### 3. MA TRẬN TRÊN MỘT VÀNH

Các ma trận quan trọng nhất trong Toán học là các ma trận trên một vành A. Khi đó tập hợp $A^{I \times K}$ các ma trận trên A tương ứng với các tập hợp chỉ số I, K có một cách chính tắc một cấu trúc song môđun (A, A) (§ 1, no. 14).

Với mỗi cặp có thứ tự $(i, k) \in I \times K$, cho $E_{ik}$ là ma trận $(a_{jl})$ sao cho $a_{ik} = 1$ và $a_{jl} = 0$ với $(j, l) \neq (i, k)$; các $E_{ik}$ được gọi là các đơn vị ma trận trong tập hợp các ma trận $A^{I \times K}$; nếu I và K là hữu hạn, chúng tạo thành cơ sở chính tắc của tập hợp này đối với cấu trúc A-môđun trái hoặc phải của nó (§ 1, no. 11). Rõ ràng
$$
tE_{ik} = E_{ki}.
$$

Trừ khi có nói khác, tích $M'M''$ của hai ma trận trên A (được giả thiết là xác định) sẽ luôn luôn được hiểu là lấy đối với phép nhân $(x, y) \mapsto xy$ trong A (hay, như người ta cũng nói, sẽ được "tính trong A"). Khi đó ta có (no. 2) các công thức tính kết hợp và tính phân phối

(7)
$$(XY)Z = X(YZ)$$

(8)
$$
\begin{cases}
X(Y + Z) = XY + XZ \\
(X + Y)Z = XZ + YZ
\end{cases}
$$
đối với ba ma trận X, Y, Z trên A, mỗi khi các tổng và tích xuất hiện trong các công thức này được xác định.

Đặc biệt, nếu $E_{ik}$ (tương ứng, $E'_{kl}, E''_{il}$) là các đơn vị ma trận trong $A^{I \times K}$ (tương ứng, $A^{K \times L}, A^{I \times L}$), với $I = \{1, p\}, K = \{1, q\}, L = \{1, r\}$, ta thu được các công thức
$$
\begin{cases}
E_{ik}E'_{jl} = 0 & \text{nếu } k \neq j \\
E_{ik}E'_{kl} = E''_{il}.
\end{cases}
$$

Gọi $A^0$ là vành đối của A và gọi $a * b \ (= ba)$ là tích của a và b trong $A^0$; khi đó, với hai ma trận X, Y trên A mà tích của chúng được xác định,
$$(10)$$
$$
t(XX) = tY * tX
$$

trong đó ở vế phải $^tY$ và $^tX$ được xét như các ma trận có phần tử trong $\mathbf{A}^0$; khi $\mathbf{A}$ là *giao hoán*, thì

$$(11)$$
$$
^t(XY) = ^tY.^tX
$$

#### Mệnh đề 1 {#alg-ii-s10-prop-1 .statement}

*Cho $\mathbf{A}, \mathbf{B}$ là hai vành và $M = (m_{ik})_{(i,k) \in I \times K}$ và*
$$
M' = (m'_{ik})_{(i,k) \in I \times K}
$$
*là hai ma trận với các tập chỉ số hữu hạn trên một* $(\mathbf{A}, \mathbf{B})$*-song môđun* $G$. *Giả sử rằng đối với mọi đơn vị ma trận* $L = (a_i)_{i \in I}$ *chỉ có một hàng và có các phần tử trong* $\mathbf{A}$ *và mọi đơn vị ma trận* $C = (b_k)_{k \in K}$ *chỉ có một cột và có các phần tử trong* $\mathbf{B}$, $L.M.C = L.M'.C$ (*các tích được tính qua các luật ngoài của* $(\mathbf{A}, \mathbf{B})$*-môđun* $G$); *khi đó* $M = M'$.

Nếu lấy $L$ là đơn vị ma trận $(a_s)$ với $a_i = 1, a_s = 0$ đối với $s \neq i$, và $C$ là đơn vị ma trận $(b_t)$ với $b_k = 1, b_t = 0$ đối với $t \neq k$, thì các tích $L.M.C$ và $L.M'.C$ là các ma trận chỉ có một phần tử, lần lượt bằng $m_{ik}$ và $m'_{ik}$.

Cho $\mathbf{A}, \mathbf{B}$ là hai vành và $\sigma : \mathbf{A} \to \mathbf{B}$ là một đồng cấu.

Với mọi ma trận $M = (m_{ik})$ trên $\mathbf{A}$, ta sẽ ký hiệu bởi $\sigma(M)$ ma trận $(\sigma(m_{ik}))$ trên $\mathbf{B}$; rõ ràng $\sigma(aM) = \sigma(a)\sigma(M)$, $\sigma(Ma) = \sigma(M)\sigma(a)$ với $a \in \mathbf{A}$, và cả $\sigma(^tM) = (^t(\sigma(M)))$ và

$$(12)$$
$$
\begin{cases}
\sigma(M + M') = \sigma(M) + \sigma(M') \\
\sigma(MM') = \sigma(M)\sigma(M')
\end{cases}
$$
*nếu các phép toán đang xét được xác định, các tích ở vế trái và vế phải của (12) lần lượt được tính trong* $\mathbf{A}$ *và* $\mathbf{B}$ *.* Khi $\sigma$ được ký hiệu bởi $x \mapsto x^\sigma$, ta viết $M^\sigma$ thay cho $\sigma(M)$.

Xét riêng một *phản tự đồng cấu* $\sigma$ của $\mathbf{A}$, nghĩa là một đồng cấu từ $\mathbf{A}$ vào vành đối $\mathbf{A}^0$, hoặc một ánh xạ từ $\mathbf{A}$ vào chính nó sao cho
$$
\sigma(a + a') = \sigma(a) + \sigma(a'), \qquad \sigma(aa') = \sigma(a')\sigma(a)
$$
*đối với mọi* $a, a'$ *trong* $\mathbf{A}$; khi đó, với hai ma trận $M, M'$ trên $\mathbf{A}$ mà tích $MM'$ của chúng được xác định,
$$(13)$$
$$
\sigma(MM') = (^t(\sigma(^tM')).\sigma(^tM))
$$
*các tích ở hai vế được tính trong* $\mathbf{A}$; *điều này suy ra ngay lập tức từ (10) và (12).*

### 4. MA TRẬN VÀ ÁNH XẠ TUYẾN TÍNH

Cho $\mathbf{A}$ là một vành và $E$ là một $\mathbf{A}$*-môđun* *(phải hoặc trái)* có một cơ sở $(e_i)_{i \in I}$. Với mọi phần tử $x \in E$, *ma trận của* $x$ *đối với cơ sở* $(e_i)$, được ký hiệu bởi $M(x)$ hoặc $\mathbf{x}$ (hoặc đôi khi đơn giản là $x$ khi không thể có sự lẫn lộn), là *ma trận cột* gồm các thành phần $x_i \ (i \in I)$ của $x$ đối với $(e_i)$ (§ 1, no. 11); trong các phép tính, đôi khi sẽ thuận tiện, để nhớ rằng chỉ số $i$ là một chỉ số hàng, ghép thêm vào nó một chỉ số cột chỉ nhận một giá trị và viết ma trận $M(x)$ dưới dạng $(x_{i0})$.

Bây giờ ta xét hai A-môđun (trái hoặc phải) E và F với các cơ sở $(e_i)_{i \in I}$ và $(f_k)_{k \in K}$ tương ứng; gọi $(f_k^*)$ là họ các dạng tọa độ tương ứng với $(f_k)$. Với một ánh xạ tuyến tính $u$ từ E vào F, ta sẽ định nghĩa *ma trận của u đối với các cơ sở* $(e_i), (f_k)$ trong mỗi trường hợp sau đây:

(D) E và F là các A-môđun phải, $u$ là A-tuyến tính.
(G) E và F là các A-môđun trái, $u$ là A-tuyến tính.

Trong phần sau, ta sẽ gắn chữ (D) (tương ứng (G)) vào các công thức áp dụng cho các môđun phải (tương ứng trái).

#### Định nghĩa 3 {#alg-ii-s10-def-3 .statement}

*Trong mỗi một trong hai trường hợp trên, ma trận của u đối với các cơ sở* $(e_i), (f_k)$ *là ma trận* $M(u) = (u_{ki})_{(k, i) \in K \times I}$ *sao cho*

$$
u_{ki} = f_k^*(u(e_i))
$$

*được viết tương ứng là*

(14 D)
$$
u_{ki} = \langle f_k^*, u(e_i) \rangle
$$
(14 G)
$$
u_{ki} = \langle u(e_i), f_k^* \rangle.
$$

*Cột* của $M(u)$ có chỉ số $i$ do đó bằng $M(u(e_i))$.

Rõ ràng nếu $u, v$ là hai ánh xạ tuyến tính từ E vào F và $M(u), M(v)$ là các ma trận của chúng đối với cùng những cơ sở ấy, thì

$$
M(u + v) = M(u) + M(v)
$$
và
$$
M(\gamma u) = \gamma M(u)
$$
với mọi phần tử $\gamma$ của *tâm* $\Gamma$ của A. Nói cách khác, một khi các cơ sở $(e_i), (f_k)$ đã được cố định, ánh xạ $u \mapsto M(u)$ là một *đẳng cấu môđun trên $\Gamma$* của $\mathrm{Hom}_A(E, F)$ lên một tập con của tập hợp $A^{K \times I}$, bằng $A^{K \times I}$ nếu K là *hữu hạn*.

#### Mệnh đề 2 {#alg-ii-s10-prop-2 .statement}

*Giả sử I và K là hữu hạn. Với mọi phần tử* $x \in E$, *ma trận* $M(u(x))$ *đối với cơ sở* $(f_k)$ *được cho bởi công thức*

(17 D)
$$
M(u(x)) = M(u) . M(x)
$$
(17 G)
$$
{}^t M(u(x)) = {}^t M(x) . {}^t M(u).
$$

Chẳng hạn, ta kiểm tra (17 G). Đặt $x = \sum_i x_{i0} e_i, \quad u(x) = \sum_k y_{k0} f_k$ với $x_{i0} \in A, \ y_{k0} \in A$; khi đó $u(x) = u\left( \sum_i x_{i0} e_i \right) = \sum_i x_{i0} u(e_i) = \sum_{i, k} x_{i0} u_{ki} f_k$; do đó y_{k0} = \sum_i x_{i0} u_{ki}. Để đưa hai chỉ số $i$ lại cạnh nhau, ta xét các ma trận chuyển vị ${}^t M(x) = (x'_{0i})$, trong đó $x'_{0i} = x_{i0}$ và
$$
{}^t M(u) = (u'_{ik}),
$$
trong đó $u'_{ik} = u_{ki}$; khi đó $y_{k0} = \sum_i x'_{0i} u'_{ik}$ và vế phải là phần tử có chỉ số $k$ của ma trận một hàng ${}^t M(x) \cdot {}^t M(u)$, do đó có (17 G).

Khi A là giao hoán, (17 G) quy về (17 D) bởi công thức (4) của no. 2.

#### Hệ quả {#alg-ii-s10-n4-cor-1 .statement}

*Cho E, F, G là ba môđun phải (resp. trái) trên một vành A, $(e_i)_{i \in I}$, $(f_k)_{k \in K}$, $(g_l)_{l \in L}$ các cơ sở hữu hạn tương ứng của E, F, G, $u : E \to F$, $v : F \to G$ là hai ánh xạ tuyến tính, $M(u)$ là ma trận của u đối với các cơ sở $(e_i)$, $(f_k)$, $M(v)$ là ma trận của v đối với các cơ sở $(f_k)$, $(g_l)$ và $M(v \circ u)$ là ma trận của $v \circ u$ đối với các cơ sở $(e_i)$, $(g_l)$; khi đó*

(18 D)
$$
M(v \circ u) = M(v) M(u)
$$
(18 G)
$$
{}^t M(v \circ u) = {}^t M(u) {}^t M(v).
$$

Chẳng hạn, ta chứng minh (18 G). Với mọi $x \in E$, theo (17 G):
$$
{}^t M(x) \cdot {}^t M(v \circ u) = {}^t M(v(u(x))) = {}^t M(u(x)) \cdot {}^t M(v) = {}^t M(x) \cdot {}^t M(u) \cdot {}^t M(v)
$$
do tính kết hợp; khi đó hệ quả suy ra từ no. 3, Mệnh đề 1 vì ma trận một hàng ${}^t M(x)$ là tùy ý.

*Nhận xét (1)*. Công thức (17 D) có thể được xem như một trường hợp riêng của (18 D). Thật vậy, với mỗi $x \in E$ tương ứng một cách chính tắc ánh xạ tuyến tính $\theta_x : A_d \to E$ ánh xạ mỗi $\alpha \in A$ tới $x \alpha$ (§ 2, no. 1). Ngay lập tức thấy rằng ma trận $M(\theta_x)$ đối với cơ sở 1 của $A_d$ và cơ sở $(e_i)$ của E chính là ma trận $M(x)$; tương tự $M(\theta_{u(x)}) = M(u(x))$ và vì thế công thức (17 D) có thể được xem như một cách diễn đạt của quan hệ
$$
\theta_{u(x)} = u \circ \theta_x.
$$

#### Mệnh đề 3 {#alg-ii-s10-prop-3 .statement}

*Cho E, F là hai A-môđun phải (tương ứng trái) và $(e_i)_{i \in I}$, $(f_k)_{k \in K}$ là các cơ sở hữu hạn của E và F tương ứng. Với mọi ánh xạ tuyến tính u từ E vào F, gọi $M(u)$ là ma trận của u đối với các cơ sở $(e_i)$ và $(f_k)$. Khi đó ma trận của ${}^t u : F^* \to E^*$ đối với các cơ sở đối ngẫu $(f_k^*)$ và $(e_i^*)$ bằng ${}^t M(u)$.*

E được đồng nhất một cách chính tắc với đối ngẫu kép của nó $E^{**}$ và $(e_i)$ với cơ sở đối ngẫu của $(e_i^*)$; khi đó (chẳng hạn giả sử E và F là các môđun phải)
$$
\langle {}^t u(f_k^*), e_i \rangle = \langle f_k^*, u(e_i) \rangle,
$$
do đó có mệnh đề.

#### Nhận xét {#alg-ii-s10-n4-rem-1 .statement}

(2) Cho E và F là hai A-môđun trái với các cơ sở $(e_i)_{i \in I}$ và $(f_k)_{k \in K}$ tương ứng. Với mọi ánh xạ A-tuyến tính $u : E \to F$, theo (14 G), $u(e_i) = \sum_k u_{ki} f_k$; các hệ thức này cũng có thể được giải thích bằng cách nói rằng ma trận cột $(u(e_i))_{i \in I}$ với các phần tử trong F bằng tích $^tM(u) \cdot (f_k)$, trong đó $(f_k)_{k \in K}$ được coi như một ma trận cột với các phần tử trong F và tích được tính đối với ánh xạ $A \times F \to F$ xác định luật tác động trên A-môđun F (no. 2).

(3) Cho A, B là hai vành giao hoán và $\sigma : A \to B$ là một đồng cấu vành. Theo ký hiệu của Mệnh đề 3, $(e_i \otimes 1)$ và $(f_k \otimes 1)$ là các cơ sở tương ứng của $E_{(B)} = E \otimes_A B$ và $F_{(B)} = F \otimes_A B$ (§ 5, no. 1, Mệnh đề 4); hơn nữa, nếu $(e_i^*)$ và $(f_k^*)$ lần lượt là các cơ sở đối ngẫu của $(e_i)$ và $(f_k)$, thì $(e_i^* \otimes 1)$ và $(f_k^* \otimes 1)$ lần lượt là các cơ sở đối ngẫu của $(e_i \otimes 1)$ và $(f_k \otimes 1)$ (§ 5, no. 4). Với mọi ánh xạ A-tuyến tính $u : E \to F$, gọi $M(u)$ và $M(u \otimes 1)$ là ma trận của $u$ đối với $(e_i)$ và $(f_k)$, và ma trận của ánh xạ B-tuyến tính $u \otimes 1$ đối với $(e_i \otimes 1)$ và $(f_k \otimes 1)$. Từ § 5, no. 4, công thức (20) suy ra rằng
$$
M(u \otimes 1) = \sigma(M(u)).
$$

Xét một hệ gồm một số hữu hạn phương trình tuyến tính vô hướng phải với một số hữu hạn ẩn số
$$
\sum_{i \in I} a_{kt} x_i = b_k \quad (k \in K)
$$
trong đó $a_{kt}, x_i, b_k$ thuộc A.

Cho $(e_i)_{i \in I}, (f_k)_{k \in K}$ là các cơ sở chính tắc của $E = A_d^I$ và $F = A_d^K$; hệ (19) tương đương với phương trình $u(x) = b$, trong đó $x = \sum_i e_i x_i$, $b = \sum_k f_k b_k$ và $u : E \to F$ là ánh xạ tuyến tính sao cho ma trận $M(u)$ đối với các cơ sở $(e_i)$ và $(f_k)$ bằng $A = (a_{kt})_{(k, i) \in K \times L}$. Ma trận này được gọi là ma trận của hệ phương trình tuyến tính (19). Nhắc lại rằng (§ 2, no. 8, Nhận xét 2 và 3), khi viết $c_i = \sum_k f_k a_{kt}$, hệ (19) tương đương với phương trình vectơ duy nhất
$$
\sum_i c_i x_i = b,
$$
và vì $c_i$ là cột có chỉ số $i$ trong ma trận $A$, ta thấy rằng nói hệ (19) có nghiệm tức là nói rằng ma trận $b = (b_{k0})$ chỉ có một cột là một tổ hợp tuyến tính của các cột của ma trận $A$.

Chúng tôi để người đọc tự phát biểu các định nghĩa và các nhận xét tương tự đối với các hệ phương trình tuyến tính trái.

### 5. TÍCH KHỐI

Các định nghĩa của no. 4 có thể được tổng quát hóa như sau. Cho E là một A-môđun (phải hoặc trái), là tổng trực tiếp của một họ $(E_i)_{i \in I}$ các môđun con. Với mọi $x \in E$, viết $x = \sum_{i \in I} x_i$ với $x_i \in E_i$ với mọi $i \in I$; ta sẽ nói rằng ma trận cột $M(x) = (x_i)_{i \in I}$ với các phần tử trong E là *ma trận của x đối với phân tích $(E_i)_{i \in I}$ của E thành tổng trực tiếp*.

Cho F là một A-môđun khác (E và F hoặc đều là A-môđun phải, hoặc đều là A-môđun trái) và giả sử rằng F là tổng trực tiếp của một họ $(F_k)_{k \in K}$ các môđun con. Với mọi $u \in \mathrm{Hom}(E, F)$ và mọi $x_i \in E_i$, viết $u(x_i) = \sum_k u_{ki}(x_i)$ với $u_{ki}(x_i) \in F_k$ với mọi $k \in K$; khi đó $u_{ki} \in \mathrm{Hom}(E_i, F_k)$; ta sẽ nói rằng ma trận $M(u) = (u_{ki})_{(k, i) \in K \times I}$ kiểu $(K, I)$ với các phần tử trong tập hợp H là tổng của các $\mathrm{Hom}(E_i, F_k)$ là *ma trận của u đối với các phân tích $(E_i)$ và $(F_k)$ của E và F thành các tổng trực tiếp*.

Với các định nghĩa này, hiển nhiên là nếu $u, v$ là hai ánh xạ A-tuyến tính từ E vào F thì, đối với các ma trận lấy theo cùng những phân tích thành tổng trực tiếp,

$$
M(u + v) = M(u) + M(v), \qquad M(\gamma u) = \gamma M(u)
$$

với mọi phần tử $\gamma$ của tâm của A (no. 2, *Nhận xét*).

Hơn nữa, định nghĩa của các $u_{ki}$ cho thấy rằng, nếu K là hữu hạn, ta có thể viết

$$
M(u(x)) = M(u) . M(x)
$$

trong đó $M(u(x))$ là ma trận của $u(x)$ đối với phân tích $(F_k)$, tích ở vế phải của (22) được tính đối với các ánh xạ $(t, z) \mapsto t(z)$ từ $\mathrm{Hom}(E_i, F_k) \times E_i$ vào $F_k$ (no. 2, *Nhận xét*).

Cho G là một A-môđun thứ ba, là tổng trực tiếp của một họ $(G_l)_{l \in L}$ các môđun con, sao cho với mọi ánh xạ A-tuyến tính $v : F \to G$ tương ứng một ma trận $M(v) = (v_{lk})$ đối với các phân tích $(F_k)$ và $(G_l)$. Nếu I, K và L là *hữu hạn*, thì

$$
M(v \circ u) = M(v) . M(u)
$$

trong đó vế trái là ma trận $(w_{li})$ của $w = v \circ u$ đối với phân tích $(E_i)$ và $(G_l)$ và tích ở vế trái được tính cho các ánh xạ $(t, s) \mapsto t \circ s$ từ $\mathrm{Hom}(F_k, G_l) \times \mathrm{Hom}(E_i, F_k)$ vào $\mathrm{Hom}(E_i, G_l)$ (no. 2, *Nhận xét*). Đây chỉ là công thức (32) của § 1, no. 8, được biểu thị theo ma trận.

Sau cùng, nếu I và K được giả sử là hữu hạn, thì $E^*$ (tương ứng $F^*$) được đồng nhất một cách chính tắc với tổng trực tiếp của các môđun $E_i^*$ (tương ứng $F_k^*$) (§ 2, no. 6, Mệnh đề 10). Khi đó kiểm tra ngay lập tức được rằng ma trận của $^t u$ đối với các phân tích $(F_k^*)$ và $(E_i^*)$ chính là $(^t u_{ki})_{(k, i) \in K \times I}$.

Bây giờ giả sử rằng I và K là hữu hạn và hơn nữa mỗi $E_i$ (tương ứng $F_k$) đều thừa nhận một cơ sở hữu hạn. Điều đó tương đương với việc nói rằng E (tương ứng F) thừa nhận một cơ sở $(e_r)_{r \in R}$ (tương ứng $(f_s)_{s \in S}$) và rằng R (tương ứng S) thừa nhận một phân hoạch $(R_i)_{i \in I}$ (tương ứng $(S_k)_{k \in K}$) sao cho với mọi $i \in I$ (tương ứng $k \in K$), $(e_r)_{r \in R_i}$ là một cơ sở của $E_i$ (tương ứng $(f_s)_{s \in S_k}$ là một cơ sở của $F_k$). Khi đó, nếu X = M(u) là ma trận của u đối với các cơ sở $(e_r)_{r \in R}$ và $(f_s)_{s \in S}$, thì ma trận $X_{kt} = M(u_{kt})$ đối với các cơ sở $(e_r)_{r \in R_i}$ và $(f_s)_{s \in S_k}$ chính là ma trận con của X thu được bằng cách bỏ các hàng có chỉ số $s \notin S_k$ và các cột có chỉ số $r \notin R_i$. Do đó ta định nghĩa một sự tương ứng một-một

$$
X \mapsto (X_{kt})_{(k, t) \in K \times I}
$$

giữa tập hợp các ma trận kiểu (S, R) với các phần tử trong A và tập hợp các ma trận của các ma trận $(X_{kt})_{(k, t) \in K \times I}$ kiểu K \times I, trong đó mỗi $X_{kt}$ là một ma trận trên A kiểu (S_k, R_i). Giả sử thêm rằng G thừa nhận một cơ sở hữu hạn $(g_t)_{t \in T}$ và rằng T = $(T_l)_{l \in L}$ là một phân hoạch của T sao cho, với mỗi $l \in L$, $(g_t)_{t \in T_l}$ là một cơ sở của $G_l$; gọi Y = M(v) là ma trận của v đối với các cơ sở $(f_s)_{s \in S}$ và $(g_t)_{t \in T}$, $Y_{lk} = M(v_{lk})$ là ma trận của $v_{lk}$ đối với các cơ sở $(f_s)_{s \in S_k}$ và $(g_t)_{t \in T_l}$, Z = M(w) là ma trận của $w = v \circ u$ đối với các cơ sở $(e_r)_{r \in R}$ và $(g_t)_{t \in T}$ và $Z_{li} = M(w_{li})$ là ma trận của $w_{li}$ đối với các cơ sở $(e_r)_{r \in R_i}$ và $(g_t)_{t \in T_l}$; khi đó suy ra từ (23) rằng các ma trận con $Z_{li}$ của Z = YX được cho bởi

$$
Z_{li} = \sum_k Y_{lk} X_{kt}
$$

nói cách khác, sự tương ứng một-một (24) biến tích thành tích khi mọi tích được xét đều xác định (các tích của ma trận của các ma trận được định nghĩa theo nghĩa của no. 2, Nhận xét); khi các ma trận con $Z_{li}$ của tích YX được tính như vậy, người ta nói rằng tích này được thực hiện "theo khối".

Tên gọi này xuất phát từ việc, khi I = {1, p} và K = {1, q}, bảng biểu diễn ma trận X được hình dung là được chia thành các "khối" tạo thành một "bảng ma trận"

$$
\begin{pmatrix}
X_{11} & X_{12} & \ldots & X_{1p} \\
X_{21} & X_{22} & \ldots & X_{2p} \\
\ldots & \ldots & \ldots & \ldots \\
X_{q1} & X_{q2} & \ldots & X_{qp}
\end{pmatrix}
$$

được xem như một ký hiệu biểu thị X khi p và q là các số nguyên cụ thể đủ nhỏ để điều này là khả thi.

### 6. MA TRẬN CỦA MỘT ÁNH XẠ NỬA TUYẾN TÍNH

Cho A, B là hai vành, $\sigma : A \to B$ là một đồng cấu từ A vào B, E là một A-môđun phải (tương ứng trái) có cơ sở $(e_i)_{i \in I}$ và F là một B-môđun phải (tương ứng trái) có cơ sở $(f_k)_{k \in K}$. Cho $u : E \to F$ là một ánh xạ *nửa tuyến tính* đối với $\sigma$ và $u(e_i) = \sum_{k \in K} f_k u_{ki}$ (tương ứng $u(e_i) = \sum_{k \in K} u_{ki} f_k$), trong đó các $u_{ki}$ do đó là các phần tử của B; theo định nghĩa, ma trận $M(u) = (u_{ki})$ kiểu $K \times I$ cũng được gọi là *ma trận của u đối với các cơ sở* $(e_i)$ và $(f_k)$. Bằng cùng phép tính như trong Mệnh đề 2 của no. 4, kiểm tra ngay lập tức được rằng với mọi $x \in E$, nếu I và K là *hữu hạn*,

(26 D)
$$
M(u(x)) = M(u) \cdot \sigma(M(x))
$$
(tương ứng

(26 G)
$$
{}^t M(u(x)) = \sigma({}^t M(x)) \cdot {}^t M(u)).
$$

Cho C là một vành thứ ba, $\tau : B \to C$ là một đồng cấu, G là một C-môđun phải (tương ứng trái) có cơ sở $(g_l)_{l \in L}$ và $v$ là một ánh xạ nửa tuyến tính từ F vào G đối với $\tau$; nếu $M(v)$ là ma trận của $v$ đối với $(f_k)$ và $(g_l)$ và $M(v \circ u)$ là ma trận của $v \circ u$ đối với $(e_i)$ và $(g_l)$, thì nếu I, K và L là hữu hạn,

(27 D)
$$
M(v \circ u) = M(v) \cdot \tau(M(u))
$$
(tương ứng

(27 G)
$$
{}^t M(v \circ u) = \tau({}^t M(u)) \cdot {}^t M(v)).
$$

Để chứng minh chẳng hạn (27 D), nhận thấy rằng với mọi $x \in E$, theo (26 D),
$$
M(v \circ u) \cdot \tau(\sigma(M(x))) = M(v(u(x)))
$$
$$
= M(v) \cdot \tau(M(u(x))) = M(v) \cdot \tau(M(u)) \cdot \tau(\sigma(M(x))),
$$
do đó có (27 D) theo Mệnh đề 1 của no. 3.

Sau cùng giả sử rằng $\sigma : A \to B$ là một *đẳng cấu*; khi đó nhắc lại rằng ${}^t u : F^* \to E^*$ là một ánh xạ nửa tuyến tính đối với $\sigma^{-1}$ (§ 2, no. 5); khi I và K là hữu hạn, ma trận của ${}^t u$ đối với các cơ sở đối ngẫu $(f_k^*)$ và $(e_i^*)$ được cho bởi

(28)
$$
M({}^t u) = \sigma^{-1}({}^t M(u))
$$

vì, theo định nghĩa, giả sử chẳng hạn E và F là các môđun phải,
$$
\langle {}^t u(f_k^*), e_i \rangle^\sigma = \langle f_k^*, u(e_i) \rangle
$$
khi $\sigma$ được ký hiệu bởi $x \mapsto x^\sigma$.

#### Nhận xét {#alg-ii-s10-n6-rem-1 .statement}

Cho A là một vành và $\sigma$ là một *phản tự đồng cấu* của A (no. 3); xét hai tình huống sau:

(GD) E là một A-môđun trái, F là một A-môđun phải và $u$ là một ánh xạ tuyến tính trên $\mathbf{Z}$ từ E vào F sao cho $u(ax) = u(x)\sigma(a)$ với $a \in A,\ x \in E$; nói cách khác, $u$ là một ánh xạ *nửa tuyến tính* tương đối với $\sigma$ từ A$^0$-môđun phải E vào A-môđun phải F.

(DG) E là một A-môđun phải, F là một A-môđun trái và $u$ là một ánh xạ tuyến tính trên $\mathbf{Z}$ từ E vào F sao cho $u(xa) = \sigma(a)u(x)$ với $a \in A,\ x \in E$; nói cách khác, $u$ là một ánh xạ *nửa tuyến tính* tương đối với $\sigma$ từ A$^0$-môđun trái E vào A-môđun trái F.

Trong hai trường hợp, ma trận $M(u)$ của $u$ đối với các cơ sở của E và F có các phần tử thuộc A; nếu các cơ sở này là hữu hạn, thì, với mọi $x \in E$, ta có các công thức tương ứng

(17 GD) $$
M(u(x)) = M(u) . \sigma(M(x))
$$
(17 DG) $$
{}^t M(u(x)) = \sigma({}^t M(x)) . {}^t M(u),
$$
các tích ở hai vế được tính *trong* A. Điều này suy ra ngay lập tức từ (26 D) và (26 G) tương ứng.

### 7. MA TRẬN VUÔNG

#### Định nghĩa 4 {#alg-ii-s10-def-4 .statement}

*Một ma trận mà các hàng và các cột có cùng tập hợp chỉ số được gọi là ma trận vuông.*

Một ma trận vuông có $n$ hàng và $n$ cột được gọi là một *ma trận cấp* $n$.

#### Nhận xét {#alg-ii-s10-n7-rem-1 .statement}

Cần lưu ý rằng một ma trận mà các tập hợp chỉ số của các hàng và các cột có *cùng lực lượng* nhưng *không đồng nhất*, thì không được xem là một ma trận vuông; đặc biệt, tích của hai ma trận như vậy trên một vành *không được định nghĩa*.

Rõ ràng phép cộng và phép nhân các ma trận vuông trên A với một tập hợp hữu hạn làm tập hợp chỉ số của các hàng và các cột xác định trên tập hợp các ma trận ấy một cấu trúc *vành* do các công thức (7), (8) và (9) (no. 3); ma trận $(\delta_{ij})$, trong đó $\delta_{ij}$ là chỉ số Kronecker (với $i \in I, j \in I$), là phần tử đơn vị của vành này và được ký hiệu là $I_n$ hoặc $l_n$ khi I có $n$ phần tử. Khi $I = \{1, n\}$, vành các ma trận được xác định như vậy được ký hiệu đơn giản là $\mathbf{M}_n(A)$; nhóm các phần tử khả nghịch của $\mathbf{M}_n(A)$ được ký hiệu là $\mathbf{GL}_n(A)$ hoặc $\mathbf{GL}(n, A)$.

Để một ma trận vuông $U = (a_{ij})$ cấp $n$ trên A khả nghịch phải (tương ứng, trái), điều kiện cần và đủ là, với mọi hệ $(b_i)_{1 \leq i \leq n}$ các phần tử của A, hệ $n$ phương trình với $n$ ẩn

$$
\sum_{j=1}^n a_{ij} x_j = b_i \quad (1 \leq i \leq n)
$$

(tương ứng, $\sum_{j=1}^n x_j a_{ji} = b_i$)

có *một nghiệm* $(x_i)$ trong A.

Cho I là một tập hợp chỉ số hữu hạn, A là một vành và E là một A-môđun phải (tương ứng, trái) có cơ sở $(e_i)_{i \in I}$. Với mọi *tự đồng cấu* $u$ của E, ma trận $M(u)$ của $u$ đối với *hai cơ sở đồng nhất với* $(e_i)$ là một ma trận vuông; nói gọn hơn, nó được gọi là ma trận của $u$ *đối với cơ sở* $(e_i)$.

Giả sử rằng $I = \{1, n\}$. Ánh xạ $u \mapsto M(u)$ (tương ứng, $u \mapsto {}^t M(u)$) là một *đẳng cấu* từ vành $\mathrm{End}_A(E)$ lên $\mathbf{M}_n(A)$ (tương ứng, lên vành đối của $\mathbf{M}_n(A)$, như suy ra từ các công thức (18 D) (tương ứng, 18 G)) (no. 4). Các phần tử khả nghịch của vành $\mathbf{M}_n(\mathbf{A})$ gọi là *ma trận khả nghịch*, tương ứng qua ánh xạ $u \mapsto M(u)$ (tương ứng, $u \mapsto {}^t M(u)$) với các *tự đẳng cấu* của E; do đó nhóm $\mathbf{GL}(n, \mathbf{A})$ được đồng nhất một cách chính tắc với nhóm $\mathbf{GL}(\mathbf{A}_d^n)$.

Nếu $u$ là một tự đẳng cấu của E, thì *phản biến* của nó $\check{u}$ là một tự đẳng cấu của A-môđun trái (resp. phải) $E^*$, sao cho $\check{u} = ({}^t u)^{-1} = {}^t (u^{-1})$ (§ 2, no. 5, Định nghĩa 6); nếu $M(\check{u})$ là ma trận của $\check{u}$ đối với cơ sở đối ngẫu $(e_i^*)$, thì, theo Mệnh đề 3 (no. 4),

$$
M(\check{u}) = ({}^t M(u))^{-1} = {}^t M(u^{-1}).
$$

Do đó với mọi ma trận khả nghịch $X$, suy ra ${}^t (X^{-1}) = ({}^t X)^{-1}$; ma trận này cũng được ký hiệu là ${}^t X^{-1}$ và được gọi là *phản biến* của ma trận $X$.

Cho $\sigma$ là một *tự đẳng cấu* của vành $\mathbf{A}$; với mọi ánh xạ *nửa tuyến tính* $u : E \to E$ đối với $\sigma$, ma trận $M(u)$ của ánh xạ này đối với một cơ sở $(e_i)$ của E cũng là một ma trận vuông. Từ (27 D) (no. 6) suy ra ngay lập tức rằng, nếu $u$ là song ánh, thì

$$
M(u^{-1}) = (\sigma^{-1}(M(u)))^{-1}.
$$

Cho E là một A-môđun là *tổng trực tiếp* của một họ hữu hạn $(E_i)_{i \in I}$ các môđun con; với mọi tự đồng cấu $u$ của E, ma trận $M(u) = (u_{ki})$ của $u$ đối với hai phân tích của E trùng với $(E_i)$ (no. 5) là một *ma trận vuông các ánh xạ tuyến tính*. Để có $u(E_i) \subset E_i$ với mọi $i \in I$, điều kiện cần và đủ là $u_{ki} = 0$ với $k \neq i$. Khi $I = \{1, n\}$, các quan hệ

$$
u(E_i) \subset E_i + E_{i+1} + \cdots + E_n \qquad (1 \leq i \leq n)
$$

là tương đương với các quan hệ $u_{ki} = 0$ với $k < i$.

*Các ví dụ về ma trận vuông.* I. *Ma trận đường chéo*. Trong một ma trận vuông

$$
M = (m_{\iota \kappa})_{(\iota, \kappa) \in I \times I},
$$

các phần tử mà hai chỉ số của chúng bằng nhau được gọi là *các phần tử đường chéo* và họ $(m_{\iota \iota})_{\iota \in I}$ được gọi là *đường chéo* của $M$; một ma trận vuông $M = (m_{\iota \kappa})$ trên một vành, mà các phần tử khác các phần tử đường chéo đều bằng không, được gọi là một *ma trận đường chéo*. Với mọi họ $(a_\iota)_{\iota \in I}$ các phần tử của một vành $\mathbf{A}$, ma trận đường chéo $(m_{\iota \kappa})$ sao cho $m_{\iota \iota} = a_\iota$ với mọi $\iota \in I$ được ký hiệu là $\operatorname{diag}(a_\iota)_{\iota \in I}$ (hoặc $\operatorname{diag}(a_1, a_2, \ldots, a_n)$ khi $I = \{1, n\}$). Trong tập hợp $\mathbf{M}_n(\mathbf{A})$ các ma trận vuông cấp $n$ trên $\mathbf{A}$, ma trận đơn vị $I_n$ là một ma trận đường chéo và mọi bội $a I_n = I_n a$ của ma trận này bởi một vô hướng $a$ cũng vậy (ma trận đường chéo (gọi là *vô hướng*) mà mọi phần tử đường chéo của nó đều bằng $a$).

Với mọi họ $(d_i)_{1 \leq i \leq n}$ các phần tử của $\mathbf{A}$ và mọi ma trận $X = (x_{ij})$ kiểu $(n, q)$ (resp. $(p, n)$) trên $\mathbf{A}$, viết $D = \operatorname{diag}(d_i)$,

$$
\begin{cases}
DX = (d_i x_{ij}) \\
XD = (x_{ij} d_j).
\end{cases}
$$

Đặc biệt, đối với hai ma trận đường chéo cấp $n$,

$$
\text{diag}(a_i) + \text{diag}(b_i) = \text{diag}(a_i + b_i)
$$
(31)
$$
\text{diag}(a_i) \cdot \text{diag}(b_i) = \text{diag}(a_i b_i).
$$

Do đó các ma trận đường chéo tạo thành một vành con của $\mathbf{M}_n(\mathbf{A})$ đẳng cấu với vành tích $\mathbf{A}^n$; các ma trận vô hướng tạo thành một vành con đẳng cấu với $\mathbf{A}$.

II. *Ma trận hoán vị; ma trận đơn thức.* Cho $\pi$ là một *phép hoán vị* bất kỳ của một tập hợp hữu hạn $\mathbf{I}$ và cho $(e_i)_{i \in \mathbf{I}}$ là cơ sở chính tắc của $\mathbf{A}$-môđun $\mathbf{E} = \mathbf{A}_d^\mathbf{I}$; tồn tại một và chỉ một tự đồng cấu $u_\pi$ của $\mathbf{E}$ sao cho, với mọi $i \in \mathbf{I}$, $u_\pi(e_i) = e_{\pi(i)}$ (§ 1, no. 11, Hệ quả 3 của Mệnh đề 17). Với mọi $i \in \mathbf{I}$, cột chỉ số $i$ trong ma trận $M(u_\pi)$ đối với cơ sở $(e_i)$ có mọi phần tử bằng không trừ phần tử ở hàng chỉ số $\pi(i)$, phần tử này bằng 1. Theo một cách nói lạm dụng, $M(u_\pi)$ được gọi là *ma trận của phép hoán vị* $\pi$. Ngay lập tức thấy rằng với hai phép hoán vị bất kỳ $\sigma, \tau$ của $\mathbf{I}$, $u_{\sigma \tau} = u_\sigma \circ u_\tau$ và đối với phép hoán vị đồng nhất $\varepsilon$, $u_\varepsilon$ là đồng nhất; do đó ánh xạ $\pi \mapsto M(u_\pi)$ là một *đẳng cấu* của nhóm đối xứng $\mathfrak{S}_\mathbf{I}$ lên nhóm các ma trận hoán vị.

Mỗi hàng và mỗi cột của một ma trận hoán vị chỉ chứa một phần tử duy nhất $\neq 0$. Một ma trận vuông hữu hạn $R$ trên một vành khác không $\mathbf{A}$, có tính chất này, được gọi là một *ma trận đơn thức*; gọi $r_i$ là phần tử duy nhất $\neq 0$ trong cột của $R$ có chỉ số $i$ và gọi $\pi(i)$ là chỉ số của hàng nơi phần tử này nằm; rõ ràng $\pi$ là một phép hoán vị của tập hợp chỉ số $\mathbf{I}$ và $R = M(u_\pi)D$, trong đó $D = \text{diag}(r_i)$.

III. *Ma trận tam giác.* Trong vành $\mathbf{M}_n(\mathbf{A})$ các ma trận vuông cấp $n$ trên một vành $\mathbf{A}$, mọi ma trận $(a_{ij})$ sao cho $a_{ij} = 0$ với $i > j$ (tương ứng $i < j$) được gọi là một *ma trận tam giác trên* (tương ứng *dưới*); cũng nói rằng một ma trận như vậy *chỉ có các số không ở dưới* (tương ứng *ở trên*) *đường chéo của nó*. Ngay lập tức chứng minh được rằng các ma trận tam giác trên (tương ứng dưới) tạo thành một vành con $S$ (tương ứng $T$) của $\mathbf{M}_n(\mathbf{A})$, và $S \cap T$ hiển nhiên là vành các ma trận đường chéo.

Tập hợp $S'$ (tương ứng $T'$) các ma trận trong $S$ (tương ứng $T$) mà các phần tử đường chéo là *khả nghịch* là một *nhóm* nhân các ma trận, gọi là *nhóm tam giác toàn phần* *trên* (tương ứng *dưới*), điều này suy ra ngay lập tức từ § 1, no. 11, *Nhận xét* 5. Tập hợp $S_1$ (tương ứng $T_1$) các ma trận trong $S$ (tương ứng $T$) mà các phần tử đường chéo đều bằng 1 là một *nhóm con* của nhóm trên, gọi là *nhóm tam giác ngặt* *trên* (tương ứng *dưới*), và mọi ma trận $M \in S'$ (tương ứng $M \in T'$) có đường chéo là $(d_i)$ đều có thể viết dưới dạng $M = DM_1 = M'_1D$, trong đó $D = \text{diag}(d_i)$ và $M_1$ và $M'_1$ là các ma trận thuộc $S_1$ (tương ứng $T_1$).

IV. *Ma trận chéo và ma trận tam giác của các ma trận.* Cho $(I_k)_{1 \leq k \leq p}$ là một phân hoạch của tập hợp hữu hạn $\mathbf{I}$; mọi ma trận bình phương trên một vành $\mathbf{A}$ có tập chỉ số là $\mathbf{I}$ đều có thể viết dưới dạng một *ma trận bình phương của các ma trận* tương ứng với cùng phân hoạch $(\mathbf{I}_k)$ của tập chỉ số của các hàng và tập chỉ số của các cột (no. 5)

$$
(32)
\begin{pmatrix}
X_{11} & X_{12} & \ldots & X_{1p} \\
X_{21} & X_{22} & \ldots & X_{2p} \\
\ldots & \ldots & \ldots & \ldots \\
X_{p1} & X_{p2} & \ldots & X_{pp}
\end{pmatrix}
$$

trong đó mỗi $X_{kk}$ là một ma trận bình phương có $\mathbf{I}_k$ làm tập chỉ số của các hàng và các cột.

Với ký hiệu này, (32) sẽ được gọi là một ma trận chéo (tương ứng tam giác trên, tương ứng tam giác dưới) của các ma trận nếu mọi ma trận $X_{ij}$ sao cho $i \neq j$ (tương ứng $i > j$, tương ứng $i < j$) đều bằng không. Cách hiểu các tự đồng cấu $u$ mà ma trận của nó là một ma trận chéo, tương ứng tam giác, của các ma trận đã được thấy trước đó, bằng cách xét ma trận tương ứng $M(u)$ của các ánh xạ tuyến tính. Các ma trận tam giác dưới (tương ứng tam giác trên, chéo) của các ma trận ứng với một phân hoạch $(\mathbf{I}_k)$ đã cho của I lập thành các vành con của vành các ma trận $\mathbf{A}^{I \times I}$. Đặc biệt, vành các ma trận chéo của các ma trận đối với phân hoạch $(\mathbf{I}_k)$ là đẳng cấu với tích $\prod_{k=1}^p \operatorname{End}_\mathbf{A}(E_k)$.

### 8. THAY ĐỔI CƠ SỞ

#### Mệnh đề 4 {#alg-ii-s10-prop-4 .statement}

*Cho E là một A-môđun phải có cơ sở hữu hạn $(e_i)_{1 \leq i \leq n}$ gồm n phần tử. Để một họ gồm n phần tử $e'_i = \sum_{j=1}^n e_j a_{ji} (1 \leq i \leq n)$ là một cơ sở của E, điều kiện cần và đủ là ma trận bình phương $P = (a_{ji})$ cấp n khả nghịch.*

$P$ chính là ma trận, đối với cơ sở $(e_i)$, của tự đồng cấu $u$ của E được xác định bởi $u(e_i) = e'_i (1 \leq i \leq n)$. Bây giờ, để $u$ là một tự đẳng cấu của E, điều kiện cần và đủ là họ $(u(e_i))$ là một cơ sở của E (§ 1, no. 11, Hệ quả 3 của Mệnh đề 17); do đó suy ra mệnh đề.

Ma trận khả nghịch $P$ được gọi là *ma trận chuyển từ cơ sở* $(e_i)$ *sang cơ sở* $(e'_i)$. Nó cũng có thể được hiểu là ma trận của ánh xạ đồng nhất $l_E$ đối với các cơ sở $(e'_i)$ và $(e_i)$ (*theo thứ tự đó*); khi đó rõ ràng ma trận chuyển *từ cơ sở* $(e'_i)$ *sang cơ sở* $(e_i)$ là *nghịch đảo* $P^{-1}$ của $P$.

#### Mệnh đề 5 {#alg-ii-s10-prop-5 .statement}

*Cho $(e_i), (e'_i)$ là hai cơ sở gồm n phần tử của E và P là ma trận chuyển từ $(e_i)$ sang $(e'_i)$. Nếu $(e_i^*)$ và $({e'_i}^*)$ là các cơ sở đối ngẫu tương ứng của $(e_i)$ và $(e'_i)$, thì ma trận chuyển từ $(e_i^*)$ sang $({e'_i}^*)$ là phản biến $^tP^{-1}$ của P.*

Chuyển vị của ánh xạ đồng nhất $l_E$ là ánh xạ đồng nhất $l_{E^*}$; theo Mệnh đề 3, no. 4, ma trận của $l_{E^*}$ đối với các cơ sở $({e'_i}^*)$ và $(e_i^*)$ (theo thứ tự đó) là chuyển vị của ma trận của $l_E$ đối với các cơ sở $(e_i)$ và $(e'_i)$ (theo thứ tự đó), tức là chuyển vị của $P^{-1}$.

#### Mệnh đề 6 {#alg-ii-s10-prop-6 .statement}

*Cho E và F là hai A-môđun phải, $(e_i)$ và $(e'_i)$ là hai cơ sở của E* gồm $n$ phần tử, $(f_j)$ và $(f'_j)$ là hai cơ sở của $F$ gồm $m$ phần tử, $P$ là ma trận chuyển từ $(e_i)$ sang $(e'_i)$ và $Q$ là ma trận chuyển từ $(f_j)$ sang $(f'_j)$. Với mọi ánh xạ tuyến tính $u$ từ $E$ vào $F$, gọi $M(u)$ là ma trận của $u$ đối với các cơ sở $(e_i)$ và $(f_j)$ và $M'(u)$ là ma trận của $u$ đối với các cơ sở $(e'_i)$ và $(f'_j)$; khi đó*

$$
M'(u) = Q^{-1} M(u) P.
$$

Ta có thể viết $u = l_F \circ u \circ l_E$. Công thức (33) suy ra ngay lập tức từ no. 4, Hệ quả của Mệnh đề 2 khi lấy ma trận của $l_E$ đối với $(e'_i)$ và $(e_i)$, ma trận của $u$ đối với $(e_i)$ và $(f_i)$ và ma trận của $l_F$ đối với $(f_i)$ và $(f'_j)$.

#### Hệ quả 1 {#alg-ii-s10-prop-6-cor-1 .statement}

*Nếu $u$ là một tự đồng cấu của $E$ và $M(u)$ và $M'(u)$ là các ma trận của nó đối với các cơ sở $(e_i)$ và $(e'_i)$ tương ứng, thì*

$$
M'(u) = P^{-1} M(u) P.
$$

#### Hệ quả 2 {#alg-ii-s10-prop-6-cor-2 .statement}

*Nếu $M(x)$ và $M'(x)$ là các ma trận một cột của cùng phần tử $x \in E$ đối với các cơ sở $(e_i)$ và $(e'_i)$ tương ứng, thì*

$$
M(x) = P . M'(x).
$$

Đây là một trường hợp riêng của Mệnh đề 6, áp dụng cho ánh xạ $\theta_x : a \mapsto xa$ từ $A_d$ đến $E$ (no. 4, *Nhận xét 1*).

Công thức (35) tương đương với

$$
x_i = \sum_{j=1}^n a_{ij} x'_j \quad (1 \leq i \leq n)
$$

đối với các phần tử $x_i$ và $x'_i$ của các ma trận $M(x)$ và $M'(x)$ tương ứng. Các công thức (36 D) được gọi là *các công thức thay đổi tọa độ*. Hãy lưu ý rằng chúng biểu thị các thành phần của $x$ đối với cơ sở "cũ" $(e_i)$ như những hàm của các thành phần của $x$ đối với cơ sở "mới" $(e'_i)$ và các phần tử của $P$, nghĩa là các thành phần của cơ sở "mới" đối với cơ sở "cũ".

#### Nhận xét {#alg-ii-s10-n8-rem-1 .statement}

(1) Bây giờ ta bắt đầu với một $A$-môđun trái $E$ có hai cơ sở $(e_i), (e'_i)$, mỗi cơ sở có $n$ phần tử; nếu ta viết $e'_i = \sum_{j=1}^n a_{ji} e_i$, thì $P = (a_{ji})$ cũng được gọi là *ma trận chuyển qua* từ $(e_i)$ đến $(e'_i)$; nó cũng là ma trận của tự đẳng cấu của $E$ sao cho $u(e_i) = e'_i$, đối với cơ sở $(e_i)$, và cũng là ma trận của $l_E$ đối với các cơ sở $(e'_i)$ và $(e_i)$ *theo thứ tự đó*. Khi đó các kết quả trên vẫn đúng, chỉ với những sửa đổi sau đây: các công thức (33 D) đến (36 D) lần lượt được thay bằng

$$
\begin{align*}
(33\text{ G}) &\quad {}^t M'(u) = {}^t P . {}^t M(u) . {}^t Q^{-1} \\
(34\text{ G}) &\quad {}^t M'(u) = {}^t P . {}^t M(u) . {}^t P^{-1} \\
(35\text{ G}) &\quad {}^t M(u) = {}^t M'(u) . {}^t P.
\end{align*}
$$

ĐẠI SỐ TUYẾN TÍNH

(36 G)
$$
x_i = \sum_{j=1}^n x_j' a_{ij} \quad (1 \leq i \leq n).
$$

(2) Dưới các giả thiết của Mệnh đề 4, xét một phần tử $x^* \in \mathbf{E}^*$; vì ma trận chuyển qua từ $(e_i^*)$ đến $(e_{i'}^*)$ là $tP^{-1}$ (Mệnh đề 5), nên đối với các ma trận $M(x^*)$ và $M'(x^*)$ của $x^*$ đối với hai cơ sở này tương ứng,

$$
tM(x^*) = tM'(x^*) . P^{-1}
$$

hay cũng là

(37 D)
$$
tM'(x^*) = tM(x^*) . P
$$

điều này tương đương với hệ phương trình

(38 D)
$$
x_{i'}^* = \sum_{j=1}^n x_j^* a_{ji} \quad (1 \leq i \leq n)
$$

đối với các phần tử $(x_i^*)$ và $(x_{i'}^*)$ của các ma trận $M(x^*)$ và $M'(x^*)$. Các công thức tương ứng đối với một A-môđun trái E là

(37 G)
$$
M'(x^*) = tP . M(x^*)
$$

(38 G)
$$
x_{i'}^* = \sum_{j=1}^n a_{ji} x_j^* \quad (1 \leq i \leq n).
$$

(3) Cho A, B là hai vành, $\sigma : A \to B$ là một đồng cấu của A vào B, E là một A-môđun phải (tương ứng, trái), $(e_i)$, $(e_i')$ là hai cơ sở có $n$ phần tử của E, F là một B-môđun phải (tương ứng, trái), $(f_j)$, $(f_j')$ là hai cơ sở có $m$ phần tử của F, và P (tương ứng, Q) là ma trận chuyển từ $(e_i)$ sang $(e_i')$ (tương ứng, từ $(f_j)$ sang $(f_j')$).

Với mọi ánh xạ nửa tuyến tính $u : E \to F$, đối với $\sigma$, gọi $M(u)$ là ma trận của $u$ đối với $(e_i)$ và $(f_j)$ và $M'(u)$ là ma trận của nó đối với $(e_i')$ và $(f_j')$. Khi đó

(39 D)
$$
M'(u) = Q^{-1} M(u) \sigma(P)
$$
(tương ứng,
(39 G)
$$
tM'(u) = \sigma(tP) . tM(u) . tQ^{-1}.
$$

Chứng minh giống như chứng minh của (33 D) và (33 G), lần này dùng các công thức (27 D) và (27 G) (no. 6).

### 9. MA TRẬN TƯƠNG ĐƯƠNG; MA TRẬN TƯƠNG TỰ

#### Định nghĩa 5 {#alg-ii-s10-def-5 .statement}

*Hai ma trận* $X, X'$ *có m hàng và n cột trên một vành được gọi là tương đương nếu tồn tại một ma trận bình phương khả nghịch* $P$ *cấp m và một ma trận bình phương khả nghịch* $Q$ *cấp n sao cho*

(40)
$$
X' = PXQ.
$$

Rõ ràng quan hệ "X và X' tương đương" là một quan hệ tương đương (Lý thuyết tập hợp, II, § 6, no. 1) trên tập hợp $A^{mn}$ các ma trận kiểu $(m, n)$ trên A, điều đó biện minh cho thuật ngữ này.

Với định nghĩa này, Mệnh đề 6 của no. 8 có thể được phát biểu bằng cách nói rằng khi thay đổi các cơ sở trong hai A-môđun phải E, F (có các cơ sở hữu hạn), thì ma trận của một ánh xạ tuyến tính $u : E \to F$ đối với các cơ sở mới là tương đương với ma trận của $u$ đối với các cơ sở cũ.

Ngược lại, nếu quan hệ (40) được thỏa mãn và $u : A_d^n \to A_d^m$ là một ánh xạ tuyến tính có ma trận là $X$ đối với các cơ sở chính tắc tương ứng $(e_i)$ và $(f_j)$ của $A_d^n$ và $A_d^m$, thì $X'$ là ma trận của $u$ đối với các cơ sở $(e'_i)$ và $(f'_j)$ sao cho $Q$ là ma trận chuyển từ $(e_i)$ sang $(e'_i)$ và $P^{-1}$ là ma trận chuyển từ $(f_j)$ sang $(f'_j)$.

Ví dụ về các ma trận tương đương. (1) Hai ma trận $X = (x_{ij})$ và $X' = (x'_{ij})$ có $m$ hàng và $n$ cột "chỉ khác nhau về thứ tự các hàng của chúng" nếu tồn tại một phép hoán vị $\sigma$ của khoảng $[1, m]$ của $\mathbf{N}$ sao cho với mọi cặp có thứ tự các chỉ số $(i, j)$, $x'_{ij} = x_{\sigma(i), j}$ (ta cũng nói rằng $X'$ thu được bằng cách thực hiện phép hoán vị $\sigma^{-1}$ trên các hàng của $X$). Khi đó các ma trận $X$ và $X'$ là tương đương, vì $X' = PX$, trong đó $P$ là ma trận của phép hoán vị $\sigma^{-1}$ (xem no. 7, Ví dụ II).

Tương tự, ta nói $X$ và $X'$ chỉ khác nhau về thứ tự các cột của chúng nếu tồn tại một phép hoán vị $\tau$ của $[1, n]$ sao cho $x'_{ij} = x_{i, \tau(j)}$ với mọi cặp có thứ tự các chỉ số $(i, j)$, $X$ và $X'$ cũng tương đương, vì $X' = XQ$ trong đó $Q$ là ma trận của phép hoán vị $\tau$.

Chú ý rằng theo ký hiệu ở trên, $P$ là ma trận chuyển từ một cơ sở $(f_j)_{1 \leq j \leq m}$ sang cơ sở $(f_{\sigma^{-1}(j)})_{1 \leq j \leq m}$ và $Q$ là ma trận chuyển từ một cơ sở $(e_i)_{1 \leq i \leq n}$ sang cơ sở $(e_{\tau(i)})_{1 \leq i \leq n}$.

(2) Cho $j, k$ là các phần tử phân biệt của $[1, n]$ và cho $a \in A$.

Giả sử rằng với $1 \leq i \leq m$, $x'_{ij} = x_{ij} + x_{ik}a$ và $x'_{il} = x_{il}$ đối với $j \neq l$ và $1 \leq i \leq m$; khi đó ta nói $X'$ được dẫn xuất từ $X$ bằng cách cộng vào cột của $X$ có chỉ số $j$ cột có chỉ số $k$ được nhân bên phải với $a$. Trong trường hợp này $X$ và $X'$ cũng tương đương: thật vậy, nếu $Q = I_n + aE_{kj}$ (một ma trận tam giác khả nghịch, như đã thấy ở no. 7), thì $X' = XQ$.

Tương tự, cho $h, i$ là hai phần tử phân biệt của $[1, m]$ và $a$ là một phần tử của $A$; nếu $X'$ được dẫn xuất từ $X$ bằng cách cộng vào hàng của $X$ có chỉ số $i$ hàng có chỉ số $h$ sau khi nhân bên trái với $a$, thì $X$ và $X'$ tương đương, vì $X' = PX$, trong đó $P = I_m + aE_{ih}$.

(3) Cuối cùng, nếu, với một chỉ số $j$ cho trước, $x'_{ij} = x_{ij}c$ với $1 \leq i \leq m$, trong đó $c$ là khả nghịch, và $x'_{il} = x_{il}$ với $1 \leq i \leq m$ và $l \neq j$, thì $X$ và $X'$ tương đương; vì $X' = XQ$, trong đó $Q$ là ma trận $\operatorname{diag}(a_k)$ với $a_j = c$, $a_k = 1$ với $k \neq j$. Khi đó, ta nói rằng $X'$ được dẫn xuất từ $X$ bằng cách nhân bên phải cột của $X$ có chỉ số $j$ với $a$.

Tương tự, nếu $X'$ được dẫn xuất từ $X'$ bằng cách nhân bên trái hàng của $X$ có chỉ số $i$ với một phần tử khả nghịch $c \in A$, thì $X'$ và $X$ tương đương, vì $X' = PX$ trong đó $P$ là ma trận $\operatorname{diag}(b_h)$ với $b_i = c$, $b_h = 1$ với $h \neq i$.

#### Định nghĩa 6 {#alg-ii-s10-def-6 .statement}

*Hai ma trận vuông X, X' cấp n trên một vành A được gọi là đồng dạng nếu tồn tại một ma trận vuông khả nghịch P cấp n sao cho*

$$(41)$$
$$X' = PXP^{-1}$$

Rõ ràng quan hệ "X và X' là đồng dạng" là một *quan hệ tương đương* trên $M_n(A)$, nghĩa là X và X' được biến đổi thành nhau bởi một *tự đẳng cấu trong* của vành này.

Với định nghĩa này, Hệ quả 1 của Mệnh đề 6 ở no. 8 có thể được phát biểu bằng cách nói rằng khi thay đổi cơ sở của một A-môđun E (có một cơ sở hữu hạn), thì ma trận của một tự đồng cấu u đối với cơ sở mới là *đồng dạng* với ma trận của u đối với cơ sở cũ.

#### Nhận xét {#alg-ii-s10-n9-rem-1 .statement}

(1) Hai ma trận vuông chỉ khác nhau ở thứ tự các hàng của chúng (hoặc thứ tự các cột của chúng) thì tương đương, nhưng nói chung *không đồng dạng*. Một ma trận đồng dạng với một ma trận vuông $X = (x_{ij})$ có thể thu được bằng cách thực hiện *cùng một phép hoán vị* $\sigma^{-1}$ trên các hàng và các cột, nghĩa là bằng cách xét ma trận $X' = (x'_{ij})$, trong đó $x'_{ij} = x_{\sigma(i), \sigma(j)}$ với mọi cặp có thứ tự các chỉ số; vì nếu X là ma trận của một tự đồng cấu u của $A^n_d$ đối với một cơ sở $(e_i)_{1 \leq i \leq n}$, thì $X'$ là ma trận của u đối với cơ sở $(e_{\sigma(i)})_{1 \leq i \leq n}$.

(2) Cho X và $X'$ là hai ma trận vuông cấp n có thể viết dưới dạng các ma trận đường chéo của các ma trận vuông (no. 7, Ví dụ IV):

$$
X = \begin{pmatrix}
X_1 & 0 & \ldots & 0 \\
0 & X_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X_p
\end{pmatrix}
\qquad
X' = \begin{pmatrix}
X'_1 & 0 & \ldots & 0 \\
0 & X'_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X'_p
\end{pmatrix}
$$

ứng với *cùng* một phân hoạch của tập hợp chỉ số $[1, n]$ đối với X và $X'$. Nếu, với $1 \leq i \leq p$, $X_i$ và $X'_i$ là tương đương (tương ứng, đồng dạng), thì X và $X'$ là tương đương (tương ứng, đồng dạng): thật vậy, nếu $X'_i = P_i X_i Q_i$ với $1 \leq i \leq p$, thì $X' = PXQ$ trong đó

$$
P = \begin{pmatrix}
P_1 & 0 & \ldots & 0 \\
0 & P_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & P_p
\end{pmatrix}
\qquad
Q = \begin{pmatrix}
Q_1 & 0 & \ldots & 0 \\
0 & Q_2 & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & Q_p
\end{pmatrix}
$$

như suy ra từ việc tính tích "khối" (no. 6). Hơn nữa, nếu $Q_i = P_i^{-1}$ với mọi i, thì $Q = P^{-1}$.

### 10. TÍCH TENXƠ CỦA CÁC MA TRẬN TRÊN MỘT VÀNH GIAO HOÁN

Cho C là một vành giao hoán, E, F, U, V là bốn C-môđun và $\phi : E \to U$, $\psi : F \to V$ là hai ánh xạ C-tuyến tính. Giả sử rằng E, F, U, V lần lượt có các cơ sở hữu hạn $(e_\lambda)_{\lambda \in L}, (f_\mu)_{\mu \in M}, (u_\rho)_{\rho \in R}, (v_\sigma)_{\sigma \in S}$; gọi $A = (a_{\rho \lambda})$ là ma trận của $\phi$ đối với $(e_\lambda)$ và $(u_\rho)$, $B = (b_{\sigma \mu})$ là ma trận của $\psi$ đối với $(f_\mu)$ và $(v_\sigma)$. Với mọi cặp có thứ tự $(\lambda, \mu) \in L \times M = N$, đặt $g_{\lambda \mu} = e_\lambda \otimes f_\mu$; với mọi cặp có thứ tự $(\rho, \sigma) \in R \times S = T$ đặt $w_{\rho \sigma} = u_\rho \otimes v_\sigma$; khi đó các $g_{\lambda \mu}$ tạo thành một cơ sở của $E \otimes F$ và các $w_{\rho \sigma}$ một cơ sở của $U \otimes V$ (§ 3, no. 6, Hệ quả 2 của Mệnh đề 7). *Tích tenxơ* của $A$ với $B$, ký hiệu bởi $A \otimes B$, là ma trận $X = (x_{\tau v})_{(\tau, v) \in T \times N}$ mà các phần tử được cho bởi

$$
x_{(\rho, \sigma), (\lambda, \mu)} = a_{\rho \lambda} b_{\sigma \mu}.
$$

Khi đó $A \otimes B$ là *ma trận của* $\phi \otimes \psi$ *đối với các cơ sở* $(g_{\lambda \mu})$ *và* $(w_{\rho \sigma})$. Theo định nghĩa (§ 3, no. 2, công thức (3))

$$
\begin{align*}
(\phi \otimes \psi)(g_{\lambda \mu}) &= (\phi \otimes \psi)(e_\lambda \otimes f_\mu) = \phi(e_\lambda) \otimes \psi(f_\mu) \\
&= \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} (u_\rho \otimes v_\sigma) = \sum_{\rho, \sigma} a_{\rho \lambda} b_{\sigma \mu} w_{\rho \sigma}.
\end{align*}
$$

Định nghĩa (42) của các phần tử của $A \otimes B$ cho thấy rằng ma trận này tương ứng song ánh với ma trận các ma trận $(a_{\rho \lambda} B)_{(\rho, \lambda) \in R \times L}$ và cả ma trận $(A b_{\sigma \mu})_{(\sigma, \mu) \in S \times M}$ (no. 5).

Việc $(\phi, \psi) \mapsto \phi \otimes \psi$ là một ánh xạ C-song tuyến tính và công thức (9) của § 3, no. 5, có thể được biểu thị bằng các đồng nhất thức

$$
\begin{align*}
(A \otimes (B_1 + B_2)) &= A \otimes B_1 + A \otimes B_2 \\
((A_1 + A_2) \otimes B) &= A_1 \otimes B + A_2 \otimes B
\end{align*}
$$
(43)

$$(cA) \otimes B = A \otimes (cB) = c(A \otimes B) \quad \text{với } c \in \mathbf{C}$$
(44)

$$(A_1 \otimes B_1)(A_2 \otimes B_2) = (A_1 A_2) \otimes (B_1 B_2)$$
(45)

khi các phép toán xuất hiện đều được xác định. Ma trận chuyển vị của một tích tenxơ của các ma trận được cho bởi

$$(A \otimes B)^t = (A^t) \otimes (B^t).$$
(46)

Nếu $A$ và $B$ là các ma trận vuông khả nghịch trên $\mathbf{C}$, thì $A \otimes B$ là khả nghịch và

$$(A \otimes B)^{-1} = (A^{-1}) \otimes (B^{-1}).$$
(47)

Cho $(e'_\lambda)_{\lambda \in L}$ là một cơ sở khác của $E$ và $(f'_\mu)_{\mu \in M}$ một cơ sở khác của $F$; nếu $P$ là ma trận chuyển từ cơ sở $(e_\lambda)$ sang cơ sở $(e'_\lambda)$ và $Q$ là ma trận chuyển từ cơ sở $(f_\mu)$ sang cơ sở $(f'_\mu)$, thì ma trận chuyển từ cơ sở $(e_\lambda \otimes f_\mu)$ sang cơ sở $(e'_\lambda \otimes f'_\mu)$ là $P \otimes Q$. Nếu $A'$ *tương đương* (resp. *đồng dạng*) với $A$ và $B'$ *tương đương* (resp. *đồng dạng*) với $B$, thì $A' \otimes B'$ *tương đương* (resp. *đồng dạng*) với $A \otimes B$.

Định nghĩa tích tenxơ của các ma trận có thể được tổng quát hóa một cách hiển nhiên cho một số hữu hạn tùy ý các ma trận trên $\mathbf{C}$; đặc biệt ta có công thức kết hợp

$$
\left( \bigotimes_{i \in I_1} X_i \right) \otimes \left( \bigotimes_{i \in I_2} X_i \right) = \bigotimes_{i \in I} X_i
$$

đối với mọi *phân hoạch* $(I_1, I_2)$ của tập hợp chỉ số hữu hạn $I$.

### 11. VẾT CỦA MỘT MA TRẬN

Cho $C$ là một vành *giao hoán*; với mọi ma trận bình phương $X = (x_{ij})$ trên $C$ ứng với tập hợp chỉ số hữu hạn $I$, *vết* của $X$ là phần tử

$$
\operatorname{Tr}(X) = \sum_{i \in I} x_{ii}.
$$

Cho $E$ là một $C$-môđun thừa nhận một cơ sở hữu hạn $(e_i)_{i \in I}$; với mọi tự đồng cấu $u$ của $E$,

$$
\operatorname{Tr}(u) = \operatorname{Tr}(M(u))
$$

trong đó $M(u)$ là ma trận của $u$ đối với cơ sở $(e_i)$; điều này suy ra ngay lập tức từ § 4, no. 3, công thức (17), khi công thức này được áp dụng cho tự đồng cấu $x \mapsto \langle x, e_i^*\rangle e_j$ (trong đó $e_i^*$ là cơ sở đối ngẫu của $(e_i)$); từ đó ta chuyển sang trường hợp tổng quát nhờ tính tuyến tính. Công thức (49) cho thấy rằng

$$
\operatorname{Tr}(u) = \sum_i \langle u(e_i), e_i^* \rangle
$$

đối với mọi cơ sở $(e_i)$ của $E$ (xem § 4, no. 3, công thức (17)).

Nếu $X$ là một ma trận kiểu $(m, n)$ trên $C$ và $Y$ là một ma trận kiểu $(n, m)$ trên $C$, thì

$$
\operatorname{Tr}(XY) = \operatorname{Tr}(YX)
$$

như suy ra từ điều trên và Mệnh đề 3 của § 4, no. 3; (52) cũng có thể thu được trực tiếp, vì nếu $X = (x_{ij}), Y = (y_{ji})$ ($1 \leq i \leq m, 1 \leq j \leq n$), thì

$$
\operatorname{Tr}(XY) = \sum_{i,j} x_{ij} y_{ji}
$$

theo (49). Hơn nữa công thức sau cùng chứng minh:

#### Mệnh đề 7 {#alg-ii-s10-prop-7 .statement}

*Cho $C$ là một vành giao hoán và với mỗi ma trận $P \in \mathbf{M}_n(C)$, ký hiệu $f_P$ là dạng tuyến tính $X \mapsto \operatorname{Tr}(PX)$ trên $\mathbf{M}_n(C)$; ánh xạ $P \mapsto f_P$ là một song ánh $C$-tuyến tính từ $\mathbf{M}_n(C)$ lên đối ngẫu của nó.*

#### Mệnh đề 8 {#alg-ii-s10-prop-8 .statement}

*Nếu $g$ là một dạng tuyến tính trên $C$-môđun $\mathbf{M}_n(C)$ sao cho $g(XY) = g(YX)$ với mọi ma trận $X, Y$ trong $\mathbf{M}_n(C)$, thì tồn tại một và chỉ một vô hướng $c \in C$ sao cho $g(X) = c \cdot \operatorname{Tr}(X)$ với mọi ma trận $X \in \mathbf{M}_n(C)$.*

Vì mệnh đề là tầm thường đối với $n = 1$, ta có thể chỉ xét trường hợp $n \geqslant 2$. Lấy $X = E_{ij},\ Y = E_{jk}$ với $i \neq k$, ta được $g(E_{ik}) = 0$; rồi lấy $X = E_{ij},\ Y = E_{ji}$ với $i \neq j$, ta thấy $g(E_{ii}) = g(E_{jj})$; mệnh đề suy ra ngay lập tức vì các $E_{ij}$ lập thành một cơ sở của $\mathbf{M}_n(\mathbf{C})$.

### 12. MA TRẬN TRÊN MỘT TRƯỜNG

Các ma trận hữu hạn có $m$ hàng và $n$ cột trên một trường $K$ tương ứng song ánh với các ánh xạ tuyến tính từ không gian vectơ phải $E = K_d^n$ vào không gian vectơ phải $K_d^m$ khi các ma trận của các ánh xạ ấy được lấy đối với các cơ sở chính tắc của $E$ và $F$. Theo định nghĩa, *hạng* của một ma trận như thế $X$ là hạng của ánh xạ tuyến tính $u : E \to F$ tương ứng với nó; vì số này theo định nghĩa là chiều của không gian con $u(E)$ của $F$, nên cũng tương đương như vậy (khi đồng nhất các cột của $X$ với các ảnh qua $u$ của cơ sở chính tắc của $E$) khi đưa ra định nghĩa sau:

#### Định nghĩa 7 {#alg-ii-s10-def-7 .statement}

*Cho một ma trận $X$ có $m$ hàng và $n$ cột trên một trường $K$, chiều của không gian con của $K_d^m$ sinh bởi $n$ cột của $X$ được gọi là hạng của $X$ đối với $K$ và được ký hiệu là $\operatorname{rg}(X)$.*

Cũng có thể nói rằng hạng của $X$ là *số lớn nhất các cột độc lập tuyến tính của $X$* (xem như các phần tử của $K_d^m$). Hiển nhiên $\operatorname{rg}(X) \leqslant \inf(m, n)$; với mọi ma trận con $Y$ của $X$, $\operatorname{rg}(Y) \leqslant \operatorname{rg}(X)$.

Nếu $E$ và $F$ là hai không gian vectơ hữu hạn chiều trên $K$ và $u$ là một ánh xạ tuyến tính từ $E$ vào $F$, thì hạng của ma trận $M(u)$ đối với hai cơ sở bất kỳ bằng hạng của $u$.

#### Mệnh đề 9 {#alg-ii-s10-prop-9 .statement}

*Nếu các phần tử của một ma trận $X$ có $m$ hàng và $n$ cột thuộc một trường con $K_0$ của một trường $K$, thì hạng của $X$ đối với $K_0$ bằng hạng của $X$ đối với $K$.*

Cho $F_0$ là không gian vectơ phải $K_0$ sinh bởi cơ sở chính tắc của không gian vectơ phải $K$ $E = K_d^m$; theo giả thiết các cột của $X$ thuộc $E_0$. Gọi $V_0$ (resp. $V$) là không gian con vectơ trên-$K_0$ của $F_0$ (resp. không gian con vectơ trên-$K$ của $E$) sinh bởi các cột ấy. Khi đó $V = V_0 \otimes_{K_0} K$ (§ 8, no. 2, Mệnh đề 2) và do đó $\dim_K V = \dim_{K_0} V_0$.

#### Mệnh đề 10 {#alg-ii-s10-prop-10 .statement}

*Hạng của một ma trận $X$ trên một trường $K$ bằng hạng của ma trận chuyển vị của nó ${}^t X$ trên trường đối $K^0$.*

Theo ký hiệu đã đưa vào trước Định nghĩa 7, hạng của $u$ bằng hạng của ${}^t u$ (§ 7, no. 5, Mệnh đề 10) và vì thế mệnh đề suy ra từ no. 4, Mệnh đề 3.

Như vậy ta thấy rằng hạng của $X$ cũng có thể được định nghĩa là *số lớn nhất các hàng độc lập tuyến tính của $X$* (coi chúng như những phần tử của không gian vectơ trái $K$ $K_s^n$).

Các ma trận vuông cấp $n$ trên một trường $K$ tương ứng song ánh với các nội cấu của $E = K_d^n$ và tạo thành một vành đẳng cấu với vành

End$_{\mathbf{K}}$ (E) (no. 7); tương ứng với các tự đẳng cấu của E là các ma trận vuông khả nghịch.

#### Mệnh đề 11 {#alg-ii-s10-prop-11 .statement}

*Cho X là một ma trận vuông cấp n trên một trường K. Các tính chất sau là tương đương:*

(a) *X khả nghịch trong $\mathbf{M}_n(\mathbf{K})$.*
(b) *X khả nghịch phải trong $\mathbf{M}_n(\mathbf{K})$.*
(c) *X khả nghịch trái trong $\mathbf{M}_n(\mathbf{K})$.*
(d) *X có hạng n.*

Đây chỉ là bản dịch của § 7, no. 4, Hệ quả của Mệnh đề 9.

#### Mệnh đề 12 {#alg-ii-s10-prop-12 .statement}

*Để một hệ gồm m phương trình tuyến tính với n ẩn*

$$
\sum_{j=1}^n a_{ij} x_j = b_i \quad (1 \leq i \leq m)
$$

*trên một trường K có ít nhất một nghiệm, điều kiện cần và đủ là ma trận $A = (a_{ij})$ của hệ và ma trận B, thu được bằng cách ghép thêm vào A một cột thứ $(n+1)$ bằng $(b_i)$, là các ma trận có cùng hạng.*

Ta đã thấy (no. 4) rằng sự tồn tại của một nghiệm của (54) tương đương với việc cột $(b_i)$ là một tổ hợp tuyến tính của các cột của $A$ và vì thế mệnh đề suy ra từ § 7, no. 3, Hệ quả 4 của Mệnh đề 4.

Chú ý rằng điều kiện của Mệnh đề 12 luôn được thỏa mãn khi $m = n$ và $A$ khả nghịch, nghĩa là có hạng $n$ (Mệnh đề 11). Khi đó, nếu $x$ và $b$ lần lượt chỉ các ma trận một cột $(x_i)$ và $(b_i)$, thì hệ (54) tương đương với $A.x = b$ và nghiệm duy nhất của nó là $x = A^{-1}.b$.

### 13. TƯƠNG ĐƯƠNG CỦA CÁC MA TRẬN TRÊN MỘT TRƯỜNG

#### Mệnh đề 13 {#alg-ii-s10-prop-13 .statement}

*Cho E, F là hai không gian vectơ hữu hạn chiều trên một trường K. Nếu $u : E \to F$ là một ánh xạ tuyến tính có hạng r, thì tồn tại các cơ sở của E và F sao cho, đối với các cơ sở ấy,*

$$
M(u) = \begin{pmatrix} I_r & 0 \\ 0 & 0 \end{pmatrix}.
$$

*Mọi ma trận kiểu $(m, n)$ trên K và có hạng r đều tương đương với một ma trận dạng (55).*

Mệnh đề thứ hai hiển nhiên tương đương với mệnh đề thứ nhất. Để chứng minh mệnh đề sau, đặt $\dim E = n$, $\dim F = m$. Hạt nhân $N = u^{-1}(0)$ có chiều $n - r$ (§ 7, no. 4, công thức (11)); gọi V là một không gian con bù của N trong E và $(e_i)_{1 \leq i \leq n}$ là một cơ sở của E sao cho $(e_i)_{1 \leq i \leq r}$ là một cơ sở của V và $(e_i)_{r+1 \leq i \leq n}$ là một cơ sở của N. Khi đó các $u(e_j)$ $(1 \leq j \leq r)$ lập thành một cơ sở của $u(E)$; do đó tồn tại một cơ sở $(f_j)_{1 \leq j \leq m}$ của F sao cho $f_j = u(e_j)$ với $1 \leq j \leq r$ (§ 7, no. 1, Định lý 2) và rõ ràng, đối với các cơ sở $(e_i)$ và $(f_j)$, ma trận $M(u)$ được cho bởi (55).

#### Hệ quả {#alg-ii-s10-n13-cor-1 .statement}

*Điều kiện cần và đủ để hai ma trận trên một trường, cùng kiểu $(m, n)$, tương đương với nhau là chúng có cùng hạng.*

Bây giờ ta sẽ tìm lại Mệnh đề 13 bằng một phương pháp khác tường minh hơn. Với mọi vành $A$, mọi $\lambda \in A$, mọi số nguyên $m > 1$ và mọi cặp có thứ tự gồm hai số nguyên *phân biệt* $i, j$ trong $[1, m]$, ta viết

$$
B_{ij}(\lambda) = I_m + \lambda E_{ij}
$$

là một ma trận khả nghịch cấp $m$ theo no. 8.

#### Bổ đề 1 {#alg-ii-s10-lem-1 .statement}

*Cho $X = (\xi_{ij})$ là một ma trận kiểu $(m, n)$ trên một vành $A$. Giả sử rằng $m \geqslant 2$ và tồn tại một phần tử $\xi_{i1}$ trong cột thứ nhất của $X$ khả nghịch trong $A$. Khi đó tồn tại hai ma trận vuông khả nghịch $P \in \mathbf{M}_m(A)$, $Q \in \mathbf{M}_n(A)$ và một ma trận $Y$ kiểu $(m - 1, n - 1)$ trên $A$ sao cho $P$ (tương ứng $Q$) là một tích các ma trận dạng $B_{ij}(\lambda)$ cấp $m$ (tương ứng $n$) và*

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 \\
0 & & & \\
\vdots & & Y & \\
0 & & &
\end{pmatrix}.
$$

Ma trận $B_{ij}(\lambda)X$ thu được bằng cách cộng vào hàng của $X$ có chỉ số $i$ hàng có chỉ số $j$ được nhân bên trái với $\lambda$ (no. 9, *Ví dụ 2*); nếu $\xi_{i1}$ khả nghịch, thì tồn tại $\lambda \in A$ sao cho, đối với ma trận $X' = B_{1i}(\lambda)X = (\xi'_{kl})$, ta có $\xi'_{11} = 1$; nhân $X'$ ở bên trái với các ma trận $B_{k1}(\mu_k)$ cấp $m$ được chọn thích hợp (với $1 \leq k \leq m$), ta thu được một ma trận $X'' = (\xi''_{kl})$ sao cho $\xi''_{j1} = 1$, $\xi''_{k1} = 0$ với $k \neq 1$. Sau đó nhân liên tiếp ma trận thu được *ở bên phải* với các ma trận $B_{1j}(v_j)$ cấp $n$ thích hợp $(2 \leq j \leq n)$ và ta thu được một ma trận có dạng (57).

#### Mệnh đề 14 {#alg-ii-s10-prop-14 .statement}

*Cho $X$ là một ma trận kiểu $(m, n)$ trên một trường $K$. Nếu $X$ có hạng $r$, thì tồn tại hai ma trận vuông khả nghịch $P \in \mathbf{M}_m(K)$, $Q \in M_n(K)$ sao cho $P$ (tương ứng $Q$) là một tích của các ma trận cấp $m$ (tương ứng $n$) có dạng $B_{ij}(\lambda)$ và*

$$
PXQ = \begin{pmatrix}
1 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & \delta_r & 0 & \cdots & 0 \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0 \\
\cdots & \cdots & \cdots & \cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & 0 & 0 & \cdots & 0
\end{pmatrix}
$$

(một ma trận $(\eta_{ij})$ mà mọi phần tử đều bằng không trừ các $\eta_{li}$ với $1 \leq i \leq r$, với $\eta_{li} = 1$ đối với $1 \leq i \leq r - 1$, $\eta_{rr} = \delta_r \neq 0$). *Nếu $r \neq m$ hoặc $r \neq n$, cũng có thể giả sử rằng $\delta_r = 1$.

Mệnh đề là hiển nhiên nếu $X = 0$; vậy giả sử $X \neq 0$. Nếu $m = n = 1$ thì mệnh đề là hiển nhiên (với $P = I_m$, $Q = I_n$, $\delta_1 \neq 0$ tùy ý). Nếu $n = 1$, $m \geq 2$, ta có thể áp dụng Bổ đề 1 (vì $X \neq 0$), bổ đề này cho dạng mong muốn (58) với $r = 1$, $\delta_r = 1$. Ta lập luận bằng quy nạp theo $n > 1$; tồn tại một phần tử $\xi_{ij} \neq 0$ trong $X$; nếu $j = 1$, có thể áp dụng Bổ đề 1 và quy bài toán về trường hợp $X$ có dạng (57). Khi đó giả thiết quy nạp áp dụng được cho $Y$ và do đó tồn tại các ma trận khả nghịch

$$
P' \in \mathbf{M}_{m-1}(\mathbf{K}), \quad Q' \in \mathbf{M}_{n-1}(\mathbf{K})
$$

là các tích của các ma trận có dạng $B_{ij}(\lambda)$ cấp $m - 1$ (resp. $n - 1$), sao cho $P'YQ'$ có dạng (58). Nhưng nếu, chẳng hạn, $B_{ij}(\lambda)$ thuộc $\mathbf{M}_{m-1}(\mathbf{K})$, thì

$$
\begin{pmatrix}
1 & 0 \\
0 & B_{ij}(\lambda)
\end{pmatrix} = B_{i+1,\ j+1}(\lambda);
$$

khi đó công thức (58) suy ra từ công thức về tích khối bằng cách viết

$$
P = \begin{pmatrix} 1 & 0 \\ 0 & P' \end{pmatrix} \text{ và } Q = \begin{pmatrix} 1 & 0 \\ 0 & Q' \end{pmatrix}.
$$

Sau cùng, nếu $j \neq 1$, thì chỉ cần xét ma trận $XB_{j1}(1)$ để quy về trường hợp trên.

Mệnh đề 14 suy ra lại Mệnh đề 13 ngay lập tức.

#### Hệ quả 1 {#alg-ii-s10-prop-14-cor-1 .statement}

*Nếu $X$ là một ma trận vuông khả nghịch cấp $n$ trên một trường $\mathbf{K}$, thì tồn tại ba ma trận khả nghịch $P, Q, D$ cấp $n$ sao cho $X = PDQ$, trong đó $P$ và $Q$ là các tích của các ma trận có dạng $B_{ij}(\lambda)$ và $D$ là một ma trận đường chéo có dạng*

$$
D = \operatorname{diag}(1, 1, \ldots, \delta),
$$

*ở đây $\delta \neq 0$ (xem Bài tập 13).*

#### Hệ quả 2 {#alg-ii-s10-prop-14-cor-2 .statement}

*Với mọi trường $\mathbf{K}$, nhóm các ma trận khả nghịch $\mathbf{GL}(n, \mathbf{K})$ được sinh bởi các ma trận hoán vị (no. 7, Ví dụ 2), các ma trận đường chéo $\operatorname{diag}(a, 1, \ldots, 1)$ ($a \neq 0$ trong $\mathbf{K}$) và các ma trận $B_{12}(\lambda)$ ($\lambda \in \mathbf{K}$).*

Ta đã thấy (no. 9) rằng tích bên phải (resp. bên trái) của một ma trận với ma trận của một phép đổi chỗ thích hợp sẽ đổi chỗ hai cột bất kỳ (resp. hai hàng bất kỳ). Khi đó ma trận $\operatorname{diag}(1, \ldots, 1, a)$ bằng tích của $\operatorname{diag}(a, 1, \ldots, 1)$ với các ma trận hoán vị, và mọi ma trận $B_{ij}(\lambda)$ đều bằng tích của $B_{12}(\lambda)$ với các ma trận hoán vị, do đó có hệ quả.

#### Nhận xét {#alg-ii-s10-n13-rem-1 .statement}

(1) Trong Chương III, ta sẽ thấy rằng, nếu $m = n = r$ và $K$ là *giao hoán*, thì với mọi cách chọn $P$ và $Q$ thỏa mãn các điều kiện của Mệnh đề 14, phần tử $\delta_r$ luôn luôn như nhau và bằng *định thức* của $X$ (III, § 8, no. 6).

(2) Lập luận của Mệnh đề 14, được sửa đổi nhẹ, cho thấy rằng tồn tại một ma trận hoán vị $R$ sao cho (với cùng các điều kiện trên $P$)

$$
PX R = \begin{pmatrix} I_r & N \\ 0 & 0 \end{pmatrix}
$$

nếu $m = n = r$ không đúng, và

$$
PX R = \operatorname{diag}(1, \ldots, 1, \delta)
$$

trong trường hợp ngược lại. Cũng lưu ý rằng phương pháp chứng minh cho một sự xác định tường minh các ma trận $P, Q, R$ khi $X$ được cho tường minh.

### Bài tập {#alg-ii-s10-exercises}

Xem [bài tập của § 10](exercises/s10/).
