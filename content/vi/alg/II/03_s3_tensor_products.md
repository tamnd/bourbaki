---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 3
section_title: Tensor products
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 243-266, 395-396
pdf_pages: 0267-0290, 0419-0420
extraction: ocr
subsections:
    - "no": 1
      title: TENSOR PRODUCT OF TWO MODULES
      page: 243
      pdf_page: 267
    - "no": 2
      title: TENSOR PRODUCT OF TWO LINEAR MAPPINGS
      page: 245
      pdf_page: 269
    - "no": 3
      title: CHANGE OF RING
      page: 246
      pdf_page: 270
    - "no": 4
      title: OPERATORS ON A TENSOR PRODUCT; TENSOR PRODUCTS AS MULTIMODULES
      page: 247
      pdf_page: 271
    - "no": 5
      title: TENSOR PRODUCT OF TWO MODULES OVER A COMMUTATIVE RING
      page: 249
      pdf_page: 273
    - "no": 6
      title: PROPERTIES OF $E \otimes_A F$ RELATIVE TO EXACT SEQUENCES
      page: 251
      pdf_page: 275
    - "no": 7
      title: TENSOR PRODUCTS OF PRODUCTS AND DIRECT SUMS
      page: 254
      pdf_page: 278
    - "no": 8
      title: ASSOCIATIVITY OF THE TENSOR PRODUCT
      page: 258
      pdf_page: 282
    - "no": 9
      title: TENSOR PRODUCT OF FAMILIES OF MULTIMODULES
      page: 259
      pdf_page: 283
statements: 30
exercises: 4
content_sha256: 2f7994ba3abc8dc06da3e00228b14105741f784f5e5fd0c6ae8018935e30acfa
translated_from: content/en/alg/II/03_s3_tensor_products.md
source_content_sha256: 1eba95005f4ce917b7b3a9ff9847bb4bbfb2a404c0a595664fe6a6f3d7426913
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-3b7fa4e4
glossary_version: 34
glossary_terms_sha256: 206940ad5368833c7e9354b54361b5abd826f6c5f29e3c7e0f7f46cdf1d16711
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. TÍCH TENXƠ

### 1. TÍCH TENXƠ CỦA HAI MÔĐUN

Cho $G_1, G_2$ là hai $\mathbf{Z}$-môđun; một ánh xạ $u$ từ tập hợp $G = G_1 \times G_2$ vào một $\mathbf{Z}$-môđun được gọi là song cộng tính (hay $\mathbf{Z}$-song tuyến tính) nếu $u(x_1, x_2)$ là "cộng tính đối với $x_1$ và đối với $x_2$"; nói chính xác, điều này có nghĩa là, với $x_1, y_1$ trong $G_1$, $x_2, y_2$ trong $G_2$,

$$
u(x_1 + y_1, x_2) = u(x_1, x_2) + u(y_1, x_2)
$$
$$
u(x_1, x_2 + y_2) = u(x_1, x_2) + u(x_1, y_2).
$$

Chú ý rằng điều này đặc biệt kéo theo $u(0, x_2) = u(x_1, 0) = 0$ với mọi $x_1 \in G_1, x_2 \in G_2$.

Cho A là một vành, E là một A-môđun phải và F là một A-môđun trái. Ta sẽ xét bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1) trong đó $\Sigma$ là loài cấu trúc $\mathbf{Z}$-môđun (khi đó các cấu xạ là các ánh xạ $\mathbf{Z}$-tuyến tính, nói cách khác, các đồng cấu nhóm cộng) và các ánh xạ $\alpha$ là các ánh xạ $f$ từ $E \times F$ vào một $\mathbf{Z}$-môđun G vừa là $\mathbf{Z}$-song tuyến tính vừa còn thỏa mãn, với mọi $x \in E, y \in F$ và $\lambda \in A$

$$(1)$$
$$
f(x \lambda, y) = f(x, \lambda y).
$$

Ta chứng minh rằng bài toán này có nghiệm. Để làm điều đó ta xét $\mathbf{Z}$-môđun $C = \mathbf{Z}^{(E \times F)}$ của các tổ hợp tuyến tính hình thức của các phần tử của $E \times F$ với hệ số trong $\mathbf{Z}$ (§ 1, no. 11), một cơ sở của nó có thể được xem là gồm các cặp có thứ tự $(x, y)$, trong đó $x \in E$ và $y \in F$. Cho D là môđun con-$\mathbf{Z}$ của C sinh bởi các phần tử thuộc một trong các kiểu sau:

$$(2)$$
$$
\begin{cases}
(x_1 + x_2, y) - (x_1, y) - (x_2, y) \\
(x, y_1 + y_2) - (x, y_1) - (x, y_2) \\
(x \lambda, y) - (x, \lambda y)
\end{cases}
$$

trong đó $x, x_1, x_2$ thuộc $E$, $y, y_1, y_2$ thuộc $F$ và $\lambda$ thuộc $A$.

#### Định nghĩa 1 {#alg-ii-s3-def-1 .statement}

*Tích tenxơ của A-môđun phải E và A-môđun trái F*, ký hiệu là $E \otimes_A F$ hoặc $E \otimes_A F$ (hoặc đơn giản là $E \otimes F$ nếu không sợ nhầm lẫn) *là thương $\mathbf{Z}$-môđun* $C/D$ (thương của $\mathbf{Z}$-môđun C gồm các tổ hợp tuyến tính hình thức của các phần tử của $E \times F$ với các hệ số trong $\mathbf{Z}$, theo môđun con $D$ sinh bởi các phần tử thuộc một trong các kiểu (2)). *Với $x \in E$ và $y \in F$, phần tử của $E \otimes_A F$ là ảnh chính tắc của phần tử $(x, y)$ của $C = \mathbf{Z}^{(E \times F)}$ được ký hiệu bởi $x \otimes y$ và được gọi là tích tenxơ của $x$ và $y$.

Ánh xạ $(x, y) \mapsto x \otimes y$ từ $E \times F$ vào $E \otimes_A F$ được gọi là *chính tắc*. Đó là một ánh xạ $\mathbf{Z}$-song tuyến tính thỏa mãn các điều kiện (1).

Ta chứng minh rằng tích tenxơ $E \otimes_A F$ và ánh xạ chính tắc ở trên tạo thành một nghiệm của bài toán ánh xạ phổ quát đã nêu trước đó. Chính xác hơn:

#### Mệnh đề 1 {#alg-ii-s3-prop-1 .statement}

(a) *Cho $g$ là một ánh xạ $\mathbf{Z}$-tuyến tính từ $E \otimes_A F$ vào một $\mathbf{Z}$-môđun $G$. Ánh xạ $(x, y) \mapsto f(x, y) = g(x \otimes y)$ từ $E \times F$ vào $G$ là $\mathbf{Z}$-song tuyến tính và thỏa mãn các điều kiện (1).*

(b) *Ngược lại, cho $f$ là một ánh xạ $\mathbf{Z}$-song tuyến tính từ $E \times F$ vào một $\mathbf{Z}$-môđun $G$ thỏa mãn các điều kiện (1). Khi đó tồn tại duy nhất một ánh xạ $\mathbf{Z}$-tuyến tính $g$ từ $E \otimes_A F$ vào $G$ sao cho $f(x, y) = g(x \otimes y)$ với $x \in E, y \in F$.*

Nếu $\phi$ ký hiệu ánh xạ chính tắc từ $E \times F$ vào $E \otimes_A F$, thì $f = g \circ \phi$; do đó suy ra (a). Để chỉ ra (b), ta chú ý rằng, theo ký hiệu của Định nghĩa 1, $f$ kéo dài thành một ánh xạ $\mathbf{Z}$-tuyến tính $\bar{f}$ từ $C$ vào $G$ (§ 1, no. 11, Mệnh đề 17). Do các hệ thức (1), $\bar{f}$ bằng không trên mọi phần tử của $C$ thuộc một trong các kiểu (2), và vì thế trên $D$. Vậy nên tồn tại một ánh xạ $\mathbf{Z}$-tuyến tính $g$ từ $C/D = E \otimes_A F$ vào $G$ sao cho $\bar{f} = g \circ \psi$, trong đó $\psi : C \to C/D$ là đồng cấu chính tắc (§ 1, no. 8, *Nhận xét*). Tính duy nhất của $g$ là ngay lập tức vì $E \otimes_A F$ được sinh, như một $\mathbf{Z}$-môđun, bởi các phần tử có dạng $x \otimes y$.

Mệnh đề 1 xác định một *đẳng cấu chính tắc* từ $\mathbf{Z}$-môđun các ánh xạ $\mathbf{Z}$-song tuyến tính $f$ từ $E \times F$ vào $G$, thỏa mãn các điều kiện (1), lên $\mathbf{Z}$-môđun $\mathrm{Hom}_{\mathbf{Z}}(E \otimes_A F, G)$.

Khi $A = \mathbf{Z}$, các điều kiện (1) tự động được thỏa mãn đối với *mọi* ánh xạ $\mathbf{Z}$-song tuyến tính $f$ và môđun con $D$ của $C$ đã được sinh bởi các phần tử thuộc hai kiểu đầu tiên trong (2).

Bây giờ nếu trở lại trường hợp tổng quát và $E'$ và $F'$ lần lượt ký hiệu các $\mathbf{Z}$-môđun nền của $E$ và $F$, thì nhận xét trên và Định nghĩa 1 chỉ ra ngay lập tức rằng $\mathbf{Z}$-môđun $E \otimes_A F$ có thể được đồng nhất một cách chính tắc với *thương* của $\mathbf{Z}$-môđun $E' \otimes_{\mathbf{Z}} F'$ bởi môđun con-$\mathbf{Z}$ sinh bởi các phần tử có dạng $(x \lambda) \otimes y - x \otimes (\lambda y)$, trong đó $x$ chạy qua $E$, $y$ chạy qua $F$ và $\lambda$ chạy qua $A$.

#### Hệ quả 1 {#alg-ii-s3-prop-1-cor-1 .statement}

*Cho $H$ là một $\mathbf{Z}$-môđun và $h : E \times F \to H$ là một ánh xạ $\mathbf{Z}$-song tuyến tính thỏa mãn các điều kiện (1) và sao cho $H$ được sinh bởi $h(E \times F)$. Giả sử rằng với mọi $\mathbf{Z}$-môđun $G$ và mọi ánh xạ $\mathbf{Z}$-song tuyến tính $f$ từ $E \times F$ vào $G$ thỏa mãn (1)* tồn tại một ánh xạ $\mathbf{Z}$-tuyến tính $g : H \to G$ sao cho $f = g \circ h$. Khi đó, nếu $\phi$ ký hiệu ánh xạ chính tắc từ $E \times F$ vào $E \otimes_A F$, thì tồn tại một và chỉ một đẳng cấu $\theta$ từ $E \otimes_A F$ lên $H$ sao cho $h = \theta \circ \phi$.

Giả thiết rằng $h(E \times F)$ sinh ra $H$ kéo theo tính duy nhất của $g$; khi đó hệ quả này chỉ là tính chất duy nhất tổng quát của một nghiệm của một bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1).

#### Hệ quả 2 {#alg-ii-s3-prop-1-cor-2 .statement}

*Cho* $E^0$ (resp. $F^0$) *ký hiệu môđun* $E$ (resp. $F$) *được xét như một môđun trái (resp. phải) trên vành đối* $A^0$; *khi đó tồn tại một và chỉ một* $\mathbf{Z}$*-môđun đẳng cấu* $\sigma : E \otimes_A F \to F^0 \otimes_{A^0} E^0$ *sao cho* $\sigma(x \otimes y) = y \otimes x$ *với* $x \in E$ *và* $y \in F$ ("tính giao hoán" của các tích tenxơ).

Theo định nghĩa của các cấu trúc $A^0$-môđun trên $E^0$ và $F^0$, ánh xạ $(x, y) \mapsto y \otimes x$ từ $E \times F$ vào $F^0 \otimes_{A^0} E^0$ là $\mathbf{Z}$-song tuyến tính và thỏa mãn các điều kiện (1), do đó tồn tại duy nhất ánh xạ $\mathbf{Z}$-tuyến tính $\sigma$. Tương tự, xác định được một ánh xạ $\mathbf{Z}$-tuyến tính $\tau : F^0 \otimes_{A^0} E^0 \to E \otimes_A F$ sao cho $\tau(y \otimes x) = x \otimes y$ và rõ ràng $\sigma$ và $\tau$ là các đẳng cấu nghịch đảo của nhau.

#### Nhận xét {#alg-ii-s3-n1-rem-1 .statement}

Tích tenxơ của các môđun khác không có thể bằng không: ví dụ, lấy hai $\mathbf{Z}$-môđun $E = \mathbf{Z}/2\mathbf{Z}$ và $F = \mathbf{Z}/3\mathbf{Z}$, ta có $2x = 0$ và $3y = 0$ với mọi $x \in E$ và $y \in F$; do đó, trong $E \otimes_{\mathbf{Z}} F$,
$$
x \otimes y = 3(x \otimes y) - 2(x \otimes y) = x \otimes (3y) - (2x) \otimes y = 0
$$
với mọi $x$ và $y$ (xem no. 6, Hệ quả 4 của Mệnh đề 6).

### 2. TÍCH TENXƠ CỦA HAI ÁNH XẠ TUYẾN TÍNH

Cho $A$ là một vành, $E, E'$ là hai $A$-môđun phải, $F, F'$ là hai $A$-môđun trái và $u : E \to E'$ và $v : F \to F'$ là hai ánh xạ tuyến tính $A$. Dễ dàng kiểm tra rằng ánh xạ
$$
(x, y) \mapsto u(x) \otimes v(y)
$$
từ $E \times F$ vào $E' \oplus_A F'$ là $\mathbf{Z}$-song tuyến tính và thỏa mãn các điều kiện (1) của no. 1. Do đó theo Mệnh đề 1 của no. 1 tồn tại một và chỉ một ánh xạ tuyến tính $\mathbf{Z}$ $w : E \otimes_A F \to E' \otimes_A F'$ sao cho
$$
w(x \otimes y) = u(x) \otimes v(y)
$$
với $x \in E, y \in F$. Ánh xạ này được ký hiệu là $u \otimes v$ (khi không thể có sự lẫn lộn) và được gọi là *tích tenxơ* của các ánh xạ tuyến tính $u$ và $v$.

Từ (3) suy ra ngay lập tức rằng $(u, v) \mapsto u \otimes v$ là một ánh xạ $\mathbf{Z}\text{-song tuyến tính}$ gọi là *chính tắc*
$$
\operatorname{Hom}_A(E, E') \times \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, E' \otimes_A F').
$$

Theo Mệnh đề 1 của no. 1, tương ứng với nó có một ánh xạ tuyến tính $\mathbf{Z}$ gọi là chính tắc

(4) $$
\operatorname{Hom}_A(E, E') \otimes_{\mathbf{Z}} \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, E' \otimes_A F')
$$
ánh xạ này gắn với mọi phần tử $u \otimes v$ của tích tenxơ ánh xạ tuyến tính $u \otimes v : E \otimes_A F \to E' \otimes_A F'$. Chú ý rằng ánh xạ chính tắc (4) *không nhất thiết là đơn ánh cũng không nhất thiết là toàn ánh*. Vì vậy ký hiệu $u \otimes v$ có thể gây ra sự lẫn lộn và ngữ cảnh sẽ cần chỉ rõ nó ký hiệu một phần tử của tích tenxơ hay một ánh xạ tuyến tính.

Hơn nữa, cho $E''$ là một $A$-môđun phải, $F''$ là một $A$-môđun trái và $u' : E' \to E''$, $v' : F' \to F''$ là các ánh xạ tuyến tính $A$; từ (3) suy ra rằng
(5)
$$
(u' \circ u) \otimes (v' \circ v) = (u' \otimes v') \circ (u \otimes v).
$$

### 3. THAY ĐỔI VÀNH

#### Mệnh đề 2 {#alg-ii-s3-prop-2 .statement}

*Cho $A, B$ là hai vành, $\rho : B \to A$ là một đồng cấu vành và $E$ (resp. $F$) là một $A$-môđun phải (resp. trái). Khi đó tồn tại một và chỉ một ánh xạ tuyến tính $\mathbf{Z}$*
(6)
$$
\phi : \rho_*(E) \otimes_B \rho_*(F) \to E \otimes_A F
$$
\* sao cho, với mọi $x \in E$ và $y \in F$, ảnh qua $\phi$ của phần tử $x \otimes y$ của $\rho_*(E) \otimes_B \rho_*(F)$ là phần tử $x \otimes y$ của $E \otimes_A F$; ánh xạ tuyến tính $\mathbf{Z}$ này là toàn ánh.*

Ta xét ánh xạ $(x, y) \mapsto x \otimes y$ từ $\rho_*(E) \times \rho_*(F)$ vào $E \otimes_A F$; nó là $\mathbf{Z}$-song tuyến tính và, với mọi $\beta \in B$, theo định nghĩa ta có $(x \rho(\beta)) \otimes y = x \otimes (\rho(\beta)y)$, do đó các điều kiện (1) của no. 1 được thỏa mãn, do đó có sự tồn tại và tính duy nhất của $\phi$ (no. 1, Mệnh đề 1). Mệnh đề sau cùng suy ra từ việc các phần tử $x \otimes y$ sinh $\mathbf{Z}$-môđun $E \otimes_A F$.

Ánh xạ (6) được gọi là *chính tắc*.

#### Hệ quả {#alg-ii-s3-n3-cor-1 .statement}

*Cho $\mathfrak{J}$ là một iđêan hai phía của $A$ sao cho $\mathfrak{J}$ được chứa trong linh hóa tử của $E$ và trong linh hóa tử của $F$, để $E$ (tương ứng, $F$) có một cấu trúc môđun trái (tương ứng, phải) chính tắc trên $(A/\mathfrak{J})$* ($§ 1$, no. 12). *Khi đó đồng cấu chính tắc* (6)
$$
\phi : E \otimes_A F \to E \otimes_{A/\mathfrak{J}} F
$$
*tương ứng với đồng cấu chính tắc $\rho : A \to A/\mathfrak{J}$ là đồng nhất.*

Với mọi $\bar{\alpha} \in A/\mathfrak{J}$, mọi $x \in E$ và mọi $y \in F$, ta có $x \bar{\alpha} = x \alpha$ (tương ứng, $\bar{\alpha} y = \alpha y$) với mọi $\alpha$ sao cho $\rho(\alpha) = \bar{\alpha}$. Nếu $C = \mathbf{Z}^{(E \times F)}$, thì môđun con của $C$ sinh bởi các phần tử $(x \alpha, y) - (x, \alpha y)$ khi đó bằng môđun con sinh bởi các phần tử $(x \bar{\alpha}, y) - (x, \bar{\alpha} y)$.

Với các giả thiết và ký hiệu của Mệnh đề 2, cho $E'$ là một $B$-môđun phải, $F'$ là một $B$-môđun trái và xét hai ánh xạ *nửa tuyến tính* $u : E' \to E$, $v:F' \to F$ đối với đồng cấu $\rho : B \to A$; $u$ (tương ứng, $v$) có thể được xem như một ánh xạ $B$-tuyến tính $E' \to \rho_*(E)$ (tương ứng, $F' \to \rho_*(F')$), do đó một ánh xạ $\mathbf{Z}$-tuyến tính $w : E' \otimes_B F' \to \rho_*(E) \otimes_B \rho_*(F)$ sao cho $w(x' \otimes y') = u(x') \otimes v(y')$ với $x' \in E',\ y' \in F'$; hợp thành ánh xạ chính tắc (6) với ánh xạ này, do đó thu được một ánh xạ $\mathbf{Z}$-tuyến tính $w' : E' \otimes_B F' \to E \otimes_A F$ sao cho $w'(x' \otimes y') = u(x') \otimes v(y')$ với $x' \in E',\ y' \in F'$; đó là ánh xạ thường sẽ được ký hiệu bởi $u \otimes v$ nếu không thể có sự lẫn lộn nào. Rõ ràng $(u, v) \mapsto u \otimes v$ là một ánh xạ $\mathbf{Z}$-song tuyến tính

$$
\operatorname{Hom}_B(E', \rho_*(E)) \times \operatorname{Hom}_B(F', \rho_*(F)) \to \operatorname{Hom}_\mathbf{Z}(E' \otimes_B F', E \otimes_A F).
$$

Hơn nữa, nếu $C$ là một vành thứ ba, $\sigma : C \to B$ là một đồng cấu, $E''$ là một $C$-môđun phải, $F''$ là một $C$-môđun trái, $u' : E'' \to E'$ và $v' : F'' \to F'$ là các ánh xạ nửa tuyến tính đối với $\sigma$, thì

$$
(u \circ u') \otimes (v \circ v') = (u \otimes v) \circ (u' \otimes v').
$$

### 4. TOÁN TỬ TRÊN MỘT TÍCH TENXƠ; CÁC TÍCH TENXƠ NHƯ NHỮNG ĐA MÔĐUN

Với các giả thiết và ký hiệu của no. 1, với mọi tự đồng cấu $u$ (resp. $v$) của $A$-môđun $E$ (resp. $F$), $u \otimes 1_F$ (resp. $1_E \otimes v$) là một tự đồng cấu của $\mathbf{Z}$-môđun $E \otimes_A F$; ngay lập tức suy ra từ (5) (no. 2) rằng ánh xạ $u \mapsto u \otimes 1_F$ (resp. $v \mapsto 1_E \otimes v$) là một *đồng cấu vành*

$$
\operatorname{End}_A(E) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)
$$

(resp. $\operatorname{End}_A(F) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$); hơn nữa,

$$
(u \otimes 1_F) \circ (1_E \otimes v) = (1_E \otimes v) \circ (u \otimes 1_F) = u \otimes v
$$

và do đó (§ 1, no. 14) $E \otimes_A F$ có một cấu trúc *song môđun trái* chính tắc đối với các vành $\operatorname{End}_A(E)$ và $\operatorname{End}_A(F)$.

Như vậy, giả sử trên $E$ cho một cấu trúc đa môđun $((B'_i); A, (C'_j))$ và trên $F$ một cấu trúc đa môđun $(A, (B''_h); (C''_{k_c}))$ (§ 1, no. 14); điều đó cũng tương đương với việc cho các đồng cấu vành $B'_i \to \operatorname{End}_A(E)$, $C'_j{}^0 \to \operatorname{End}_A(E)$ có các ảnh giao hoán từng đôi một, và các đồng cấu vành $B''_h \to \operatorname{End}_A(F)$, $C''_{k_c}{}^0 \to \operatorname{End}_A(F)$ có các ảnh giao hoán từng đôi một. Nếu hợp thành các đồng cấu này tương ứng với các đồng cấu chính tắc $\operatorname{End}_A(E) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$ và $\operatorname{End}_A(F) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$ đã định nghĩa ở trên, thì thấy được (có tính đến (7)) rằng các đồng cấu vành

$$
\begin{align*}
B'_i &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F), & C'_j{}^0 &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F) \\
B''_h &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F), & C''_{k_c}{}^0 &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F)
\end{align*}
$$

được xác định với các ảnh *giao hoán từng đôi một*; nói cách khác, trên $E \otimes_A F$ đã được xác định một cấu trúc đa môđun $((B'_i), (B''_h); (C'_j), (C''_{k_c}))$; chính đa môđun này cũng được gọi là *tích tenxơ* (tương đối với $A$) *của*

đa môđun $((B'_i); A, (C'_j))$ E và đa môđun $(A, (B''_h); (C''_k))$ F. Đa môđun này là nghiệm của một bài toán ánh xạ phổ quát tương tự như bài toán đã xét trong no. 1; nói chính xác:

#### Mệnh đề 3 {#alg-ii-s3-prop-3 .statement}

Cho G là một đa môđun $((B'_i), (B''_h); (C'_j), (C''_k))$.

(a) Cho g là một ánh xạ tuyến tính của đa môđun E $\otimes_A$ F vào G. Ánh xạ $f : (x, y) \mapsto g(x \otimes y)$ từ E $\times$ F vào G là $\mathbf{Z}$-song tuyến tính và thỏa mãn các hệ thức (1) của no. 1 và các điều kiện

$$
\begin{cases}
f(\mu'_i x, y) = \mu'_i f(x, y), & f(x v'_j, y) = f(x, y) v'_j \\
f(x, \mu''_h y) = \mu''_h f(x, y), & f(x, y v''_k) = f(x, y) v''_k
\end{cases}
$$

với mọi $x \in E, y \in F, \mu'_i \in B'_i, v'_j \in C'_j, \mu''_h \in B''_h, v''_k \in C''_k, i, j, h, k$ tùy ý.

(b) Ngược lại, cho f là một ánh xạ $\mathbf{Z}$-song tuyến tính từ E $\times$ F vào G thỏa mãn các điều kiện (1) (no. 1) và (8). Khi đó tồn tại một và chỉ một ánh xạ tuyến tính g của đa môđun E $\otimes_A$ F vào đa môđun G sao cho $f(x, y) = g(x \otimes y)$ với $x \in E, y \in F$.

Mệnh đề (a) suy ra ngay lập tức từ định nghĩa của cấu trúc đa môđun trên E $\otimes_A$ F, vì chẳng hạn $(x \otimes y)v'_j = (xv'_j) \otimes y$. Để chứng minh (b), trước hết chú ý rằng Mệnh đề 1 của no. 1 cho sự tồn tại và tính duy nhất của một ánh xạ $\mathbf{Z}$-tuyến tính g sao cho $g(x \otimes y) = f(x, y)$ với $x \in E, y \in F$; điều duy nhất cần làm là kiểm tra rằng g là tuyến tính đối với các cấu trúc đa môđun. Vì các phần tử $x \otimes y$ sinh $\mathbf{Z}$-môđun E $\otimes_A$ F, chỉ cần kiểm tra các hệ thức $g(\mu'(x \otimes y)) = \mu'_i g(x \otimes y)$ và các hệ thức tương tự; nhưng điều này suy ra ngay lập tức từ công thức $g(x \otimes y) = f(x, y)$ và các hệ thức (8).

#### Chú giải {#alg-ii-s3-n4-sch-1 .statement}

Một phần tử của E $\otimes_A$ F nói chung có thể được viết theo nhiều cách dưới dạng $\sum_i (x_i \otimes y_i)$, trong đó $x_i \in E$ và $y_i \in F$; nhưng để định nghĩa một ánh xạ tuyến tính g của đa môđun E $\otimes_A$ F vào một đa môđun G, không cần phải kiểm tra rằng, nếu $\sum_i (x_i \otimes y_i) = \sum_j (x'_j \otimes y'_j)$, thì $\sum_i g(x_i \otimes y_i) = \sum_j g(x'_j \otimes y'_j)$; chỉ cần cho trước $g(x \otimes y)$ với $x \in E$ và $y \in F$ và kiểm tra rằng $(x, y) \mapsto g(x \otimes y)$ là $\mathbf{Z}$-song tuyến tính và thỏa mãn các điều kiện (1) (no. 1) và (8).

Cho E' là một đa môđun ((B'_i), A, (C'_j)), F' là một đa môđun (A, (B''_h); (C''_k)) và $u : E \to E', v : F \to F'$ là các ánh xạ tuyến tính của các đa môđun; ngay lập tức suy ra từ các định nghĩa (no. 2) rằng $u \otimes v$ là một ánh xạ tuyến tính của đa môđun E $\otimes_A$ F vào đa môđun E' $\otimes_A$ F'.

Vẫn ký hiệu E là một A-môđun phải, ký hiệu $_sA_d$ là vành A được xét như một (A, A)-song môđun (§ 1, no. 14, Ví dụ 1); theo điều trên, tích tenxơ E $\otimes_A (_sA_d)$ có một cấu trúc A-môđun phải chính tắc sao cho $(x \otimes \lambda)\mu = x \otimes (\lambda \mu)$ với $x \in E, \lambda \in A, \mu \in A$. Ánh xạ $(x, \lambda) \mapsto x \lambda$ từ E $\times (_sA_d)$ vào E là $\mathbf{Z}$-song tuyến tính và thỏa mãn các điều kiện (1) (no. 1) và (8) (trong đó, ở điều kiện sau, các $B'_i, C'_j$ và $B''_h$ không có mặt và họ $(C''_k)$ thu về A); do đó (Mệnh đề 3), tồn tại một ánh xạ A-tuyến tính $g$ (gọi là chính tắc) từ $E \otimes_A (sA_d)$ vào $E$ sao cho $g(x \otimes \lambda) = x\lambda$ với $x \in E, \lambda \in A$.

#### Mệnh đề 4 {#alg-ii-s3-prop-4 .statement}

*Nếu $E$ là một A-môđun phải, thì ánh xạ $h : x \mapsto x \otimes 1$ từ $E$ vào $E \otimes_A (sA_d)$ là một đẳng cấu A-môđun phải, mà đẳng cấu nghịch đảo $g$ của nó thỏa mãn $g(x \otimes \lambda) = x\lambda$ với $x \in E, \lambda \in A$.*

Nếu $g$ là ánh xạ chính tắc, thì $g \circ h$ là ánh xạ đồng nhất $1_E$ và $h \circ g$ trùng với ánh xạ đồng nhất của $E \otimes_A (sA_d)$ lên chính nó đối với các phần tử có dạng $x \otimes y$, là các phần tử sinh ra $\mathbf{Z}$-môđun sau; do đó có kết luận.

Ta sẽ thường viết $E \otimes_A A$ thay cho $E \otimes_A (sA_d)$ và sẽ thường đồng nhất $E \otimes_A A$ với $E$ nhờ các đẳng cấu chính tắc ở trên. Lưu ý rằng, nếu $E$ còn có một cấu trúc $B$-môđun (trái hoặc phải) tương thích với cấu trúc $A$-môđun phải của nó, thì $g$ và $h$ cũng là các đẳng cấu đối với các cấu trúc $B$-môđun trên $E$ và $E \otimes_A A$ (và do đó là các đẳng cấu đa môđun).

Bây giờ cho $F$ là một $A$-môđun trái; khi đó $(sA_d) \otimes_A F$ (cũng được ký hiệu bởi $A \otimes_A F$) có một cấu trúc $A$-môđun trái chính tắc và, như trong Mệnh đề 4, ta định nghĩa một đẳng cấu chính tắc từ $A \otimes_A F$ lên $F$ biến $\lambda \otimes x$ thành $\lambda x$, và đẳng cấu nghịch đảo của nó là $x \mapsto 1 \otimes x$.

Đặc biệt, tồn tại một đẳng cấu chính tắc của song môđun $(A, A)$ $(sA_d) \otimes_A (sA_d)$ lên $sA_d$ biến $\lambda \otimes \mu$ thành $\lambda \mu$.

### 5. TÍCH TENXƠ CỦA HAI MÔĐUN TRÊN MỘT VÀNH GIAO HOÁN

Cho $C$ là một vành *giao hoán*; với mọi $C$-môđun $E$, cấu trúc môđun trên $E$ là *tương thích với chính nó* (§ 1, no. 14). Nếu $E$ và $F$ là hai $C$-môđun, thì các nhận xét của no. 4 cho phép ta định nghĩa *hai* cấu trúc $C$-môđun trên tích tenxơ $E \otimes_C F$, lần lượt sao cho $\gamma(x \otimes y) = (\gamma x) \otimes y$ và sao cho $\gamma(x \otimes y) = x \otimes (\gamma y)$; nhưng vì, theo Định nghĩa 1 của no. 1, trong trường hợp này $(\gamma x) \otimes y = x \otimes (\gamma y)$, nên hai cấu trúc ấy *trùng nhau*. Từ nay về sau, khi nói về $E \otimes_C F$ như một $C$-*môđun*, ta sẽ hiểu là với cấu trúc được định nghĩa như vậy, trừ khi có nói rõ ngược lại. Đẳng cấu chính tắc

$$
\sigma : F \otimes_C E \to E \otimes_C F
$$

(no. 1, Hệ quả 2 của Mệnh đề 1) khi đó là một đẳng cấu $C$-môđun.

Theo định nghĩa này, nếu $(a_\lambda)_{\lambda \in L}$ (resp. $(b_\mu)_{\mu \in M}$) là một *hệ sinh* của $C$-môđun $E$ (resp. $F$), thì $(a_\lambda \otimes b_\mu)$ là một *hệ sinh* của $C$-môđun $E \otimes_C F$; đặc biệt, nếu $E$ và $F$ là các $C$-môđun *sinh hữu hạn*, thì $E \otimes_C F$ cũng vậy.

Với mọi C-môđun $G$, các ánh xạ $\mathbf{Z}$-song tuyến tính $f$ của $E \times F$ vào $G$ sao cho

$$
f(\gamma x, y) = f(x, \gamma y) = \gamma f(x, y) \quad \text{với } x \in E, y \in F, \gamma \in C
$$

khi đó được gọi là C-song tuyến tính và tạo thành một C-môđun ký hiệu bởi $\mathcal{L}_2(E, F; G)$; Mệnh đề 3 (no. 4) xác định một đẳng cấu C-môđun chính tắc (x. § 1, no. 14, Nhận xét 1).

$$
\mathcal{L}_2(E, F; G) \to \mathrm{Hom}_C(E \otimes_C F, G).
$$

Cho E', F' là hai C-môđun và $u : E \to E'$, $v : F \to F'$ là hai ánh xạ C-tuyến tính; khi đó (no. 4) $u \otimes v$ là một ánh xạ C-tuyến tính của $E \otimes_C F$ vào $E' \otimes_C F'$. Hơn nữa, ngay lập tức thấy rằng $(u, v) \mapsto u \otimes v$ là một ánh xạ C-song tuyến tính của $\mathrm{Hom}_C(E, E') \times \mathrm{Hom}_C(F, F')$ vào $\mathrm{Hom}_C(E \otimes_C F, E' \otimes_C F')$; do đó tương ứng với nó một cách chính tắc có một ánh xạ C-tuyến tính, gọi là chính tắc:

$$
\mathrm{Hom}_C(E, E') \otimes_C \mathrm{Hom}_C(F, F') \to \mathrm{Hom}_C(E \otimes_C F, E' \otimes_C F')
$$

ánh xạ này gán cho mọi phần tử $u \otimes v$ của tích tenxơ

$$
\mathrm{Hom}_C(E, E') \otimes_C \mathrm{Hom}_C(F, F')
$$

ánh xạ tuyến tính $u \otimes v$. Chú ý rằng ánh xạ chính tắc (11) *không nhất thiết là đơn ánh cũng không toàn ánh* (§ 4, Bài tập 2).

#### Nhận xét {#alg-ii-s3-n5-rem-1 .statement}

(1) Cho A, B là hai vành giao hoán, $\rho : B \to A$ là một đồng cấu vành và E và F là hai A-môđun; khi đó ánh xạ chính tắc (6) của no. 3 là một ánh xạ B-tuyến tính

$$
\rho_*(E) \otimes \rho_*(F) \to \rho_*(E \otimes_A F).
$$

(2) Điều đã nói trong no. này có thể được tổng quát hóa cho trường hợp sau: cho E là một A-môđun phải, F là một A-môđun trái, C là một vành giao hoán và $\rho : C \to A$ là một đồng cấu của C vào A sao cho $\rho(C)$ được chứa trong tâm của A (x. III, § 1, no. 3). Khi đó ta có thể xét các C-môđun $\rho_*(E)$ và $\rho_*(F)$ và giả thiết trên $\rho$ kéo theo rằng các cấu trúc C-môđun này tương thích tương ứng với các cấu trúc A-môđun trên E và F (§ 1, no. 14). Tích tenxơ $E \otimes_A F$ do đó (nhờ no. 4) được cho hai cấu trúc C-môđun sao cho $\gamma(x \otimes y) = (x \rho(\gamma)) \otimes y$ và

$$
\gamma(x \otimes y) = x \otimes (\rho(\gamma)y)
$$

tương ứng với $\gamma \in C$, $x \in E$, $y \in F$ và Định nghĩa 1 (no. 1) cũng cho thấy rằng hai cấu trúc này là đồng nhất. Nếu E' (resp. F') là một A-môđun phải (resp. trái) và $u : E \to E'$, $v : F \to F'$ là hai ánh xạ A-tuyến tính, thì $u \otimes v : E \otimes_A F \to E' \otimes_A F'$ là C-tuyến tính đối với các cấu trúc C-môđun vừa được định nghĩa; ánh xạ $(u, v) \mapsto u \otimes v$:

$$
\mathrm{Hom}_A(E, E') \times \mathrm{Hom}_A(F, F') \to \mathrm{Hom}_C(E \otimes_A F, E' \otimes_A F')
$$

là C-song tuyến tính (đối với các cấu trúc C-môđun trên $\mathrm{Hom}_A(E, E')$ và $\mathrm{Hom}_A(F, F')$) được định nghĩa ở § 1, no. 14, *Nhận xét* 1), do đó ta cũng suy ra một ánh xạ *C-tuyến tính*, gọi là *chính tắc*

(13) $\operatorname{Hom}_A(E, E') \otimes_C \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_C(E \otimes_A F, E' \otimes_A F')$.

(3) Cho A là một miền nguyên và K là trường phân thức của nó. Nếu E và F là hai không gian vectơ K, ánh xạ chính tắc

$$
(E_{[A]}) \otimes_A (F_{[A]}) \to E \otimes_K F
$$

(no. 3 và § 1, no. 13) là *song ánh*. Chỉ cần (no. 4) chứng minh rằng nếu $f$ là một ánh xạ *A-song tuyến tính* của $E \times F$ vào một không gian vectơ K G, thì $f$ cũng là *K-song tuyến tính*. Thật vậy, với mọi $\alpha \neq 0$ trong A.

$$
\alpha f(\alpha^{-1}x, y) = f(x, y) = \alpha f(x, \alpha^{-1}y)
$$
do đó
$$
f(\alpha^{-1}x, y) = f(x, \alpha^{-1}y) = \alpha^{-1}f(x, y)
$$
vì G là một không gian vectơ K.

### 6. CÁC TÍNH CHẤT CỦA $E \otimes_A F$ ĐỐI VỚI CÁC DÃY KHỚP

#### Mệnh đề 5 {#alg-ii-s3-prop-5 .statement}

*Cho* E, E', E'' *là các* A-*môđun phải*, F *là một* A-*môđun trái* và

(14)

$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \to 0
$$

*là một dãy khớp các ánh xạ tuyến tính.* *Viết* $\bar{u} = u \otimes 1_F, \bar{v} = v \otimes 1_F,$ *thì dãy*

(15)

$$
E' \otimes_A F \xrightarrow{\bar{u}} E \otimes_A F \xrightarrow{\bar{v}} E'' \otimes_A F \to 0
$$

*các* $\mathbf{Z}$-*đồng cấu* *là khớp*.

Chiếu theo no. 2, công thức (5), $\bar{v} \circ \bar{u} = (v \circ u) \otimes 1_F = 0$; ảnh $H = \bar{u}(E' \otimes F)$ được chứa trong hạt nhân $L = \operatorname{Ker}(\bar{v})$; bằng cách chuyển qua thương, do đó ta suy ra từ $\bar{v}$ một ánh xạ $\mathbf{Z}$-tuyến tính $f$ từ đối hạt nhân $M = (E \otimes F)/H$ của $\bar{u}$ vào $E'' \otimes F$; cần phải chứng minh rằng $f$ là *song ánh* và vì thế sẽ đủ để định nghĩa một ánh xạ $\mathbf{Z}$-tuyến tính $g : E'' \otimes F \to M$ sao cho $g \circ f$ và $f \circ g$ là các ánh xạ đồng nhất.

Cho $x'' \in E''$, $y \in F$; theo giả thiết tồn tại $x \in E$ sao cho $v(x) = x''$. Ta chỉ ra rằng, nếu $x_1, x_2$ là hai phần tử của E sao cho $v(x_1) = v(x_2) = x''$ và $\phi : E \otimes F \to M$ là ánh xạ chính tắc, thì $\phi(x_1 \otimes y) = \phi(x_2 \otimes y)$. Chỉ cần chứng minh rằng nếu $v(x) = 0$ thì $\phi(x \otimes y) = 0$, điều này suy ra từ sự kiện rằng $x = u(x')$ với $x' \in E'$, do đó $x \otimes y = u(x') \otimes y = \bar{u}(x' \otimes y) \in H$. Nếu $(x'', y)$ được ánh xạ tới giá trị duy nhất $\phi(x \otimes y)$ với mọi $x \in E$ sao cho $v(x) = x''$, thì một ánh xạ từ $E'' \times F$ vào M được định nghĩa; ánh xạ này là $\mathbf{Z}$-song tuyến tính và thỏa mãn các điều kiện (1) (no. 1), vì $v(x \lambda) = x'' \lambda$ và $(x \lambda) \otimes y = x \otimes (\lambda y)$ với $x \in E$; do đó có một ánh xạ $\mathbf{Z}$-tuyến tính $g$ từ $E'' \otimes F$ vào M sao cho $g(x'' \otimes y) = \phi(x \otimes y)$ với $y \in F, x \in E$ và $x'' = v(x)$. Định nghĩa này còn chứng minh rằng $f \circ g$ trùng với ánh xạ đồng nhất trên các phần tử của

E'' \otimes F có dạng x'' \otimes y và do đó f \circ g là ánh xạ đồng nhất của E'' \otimes F; mặt khác, với x \in E và y \in F, $f(\phi(x \otimes y)) = v(x) \otimes y$ theo định nghĩa, do đó $g(f(\phi(x \otimes y))) = \phi(x \otimes y)$ và, vì các phần tử có dạng \phi(x \otimes y) sinh ra M, $g \circ f$ là ánh xạ đồng nhất của M.

#### Hệ quả {#alg-ii-s3-n6-cor-1 .statement}

*Cho F, F', F'' là các A-môđun trái, E là một A-môđun phải và*
$$
\begin{array}{ccccc}
F' & \xrightarrow{s} & F & \xrightarrow{t} & F'' \longrightarrow 0
\end{array}
$$
*(16)*
*là một dãy khớp các ánh xạ tuyến tính. Đặt \bar{s} = l_E \otimes s, \bar{t} = l_E \otimes t, dãy các \mathbf{Z}-đồng cấu*
$$
\begin{array}{cccccc}
E \otimes_A F' & \xrightarrow{\bar{s}} & E \otimes_A F & \xrightarrow{\bar{t}} & E \otimes_A F'' & \longrightarrow 0
\end{array}
$$
*(17)*
*là khớp.*

Khi E (tương ứng F) được xét như một A^0-môđun trái (tương ứng phải), F \otimes_{A^0} E được đồng nhất với E \otimes_A F và có các sự đồng nhất tương tự cho F' \otimes_{A^0} E và F'' \otimes_{A^0} E (no. 1, Hệ quả 2 của Mệnh đề 1); khi đó hệ quả suy ra ngay lập tức từ Mệnh đề 5.

#### Nhận xét {#alg-ii-s3-n6-rem-1 .statement}

Chú ý rằng nói chung, nếu E' là một môđun con của một A-môđun phải E và j : E' \to E là đơn ánh chính tắc, thì ánh xạ chính tắc
$$
j \otimes 1_F : E' \otimes F \to E \otimes F
$$
*không nhất thiết là đơn ánh.* Nói cách khác, đối với một dãy khớp
$$
\begin{array}{ccccccc}
0 & \longrightarrow & E' & \xrightarrow{u} & E & \xrightarrow{v} & E'' \longrightarrow 0
\end{array}
$$
*(18)*
nói chung không thể kết luận rằng dãy
$$
\begin{array}{ccccccc}
0 & \longrightarrow & E' \otimes F & \xrightarrow{u} & E \otimes F & \xrightarrow{v} & E'' \otimes F \longrightarrow 0
\end{array}
$$
*(19)*
*là khớp.*

Lấy chẳng hạn A = \mathbf{Z}, E = \mathbf{Z}, E' = 2\mathbf{Z}, F = \mathbf{Z}/2\mathbf{Z}. Vì E' đẳng cấu với E, E' \otimes F đẳng cấu với E \otimes F mà bản thân nó lại đẳng cấu với F (no. 4, Mệnh đề 4). Nhưng với mọi x' = 2x \in E' (trong đó x \in E) và mọi y \in F, j(x') \otimes y = (2x) \otimes y = x \otimes (2y) = 0, vì 2y = 0, và ảnh chính tắc của E' \otimes F trong E \otimes F thu về 0.

Nói cách khác, phải cẩn thận phân biệt, với một môđun con E' của E và một phần tử x \in E', giữa phần tử x \otimes y "được tính trong E' \otimes F'" và phần tử x \otimes y "được tính trong E \otimes F" (nói cách khác, phần tử j(x) \otimes y).

Sau này ta sẽ nghiên cứu, dưới tên gọi các môđun phẳng, các môđun F sao cho dãy (19) là khớp với mọi dãy khớp (18) (*Đại số giao hoán*, I, § 2).

#### Mệnh đề 6 {#alg-ii-s3-prop-6 .statement}

*Cho hai dãy khớp (14) và (16), đồng cấu v \otimes t : E \otimes_A F \to E'' \otimes_A F'' là toàn ánh và hạt nhân của nó bằng*
$$
\operatorname{Im}(u \otimes 1_F) + \operatorname{Im}(l_E \otimes s)
$$

Bây giờ $v \otimes t = (v \otimes 1_{F''}) \circ (1_E \otimes t)$ (no. 2, công thức (5)) và do đó $v \otimes t$ là toàn ánh, vì nó là hợp thành của hai đồng cấu toàn ánh theo Mệnh đề 5 và Hệ quả của nó. Mặt khác, để $z \in E \otimes F$ thuộc hạt nhân của $v \otimes t$, điều kiện cần và đủ là $(1_E \otimes t)(z)$ thuộc hạt nhân của $v \otimes 1_{F''}$, tức là, chiếu theo (15), thuộc ảnh của

$$
u \otimes 1_{F''}: E' \otimes F'' \to E \otimes F''.
$$

Nhưng vì đồng cấu $t: F \to F''$ là toàn ánh, nên

$$
1_{E'} \otimes t: E' \otimes F \to E' \otimes F''
$$

cũng toàn ánh theo Hệ quả của Mệnh đề 5, do đó điều kiện trên z quy về sự tồn tại của một $a \in E' \otimes F$ sao cho

$$
(l_E \otimes t)(z) = (u \otimes t)(a).
$$

Cho $b = z - (u \otimes 1_F)(a)$; khi đó $(l_E \otimes t)(b) = 0$, và theo (17), $b$ thuộc ảnh của $l_E \otimes s$, điều đó chứng minh mệnh đề.

Nói cách khác:

#### Hệ quả 1 {#alg-ii-s3-prop-6-cor-1 .statement}

*Cho $E'$ là một môđun con của một A-môđun phải $E$, $F'$ là một môđun con của một A-môđun trái $F$ và $\operatorname{Im}(E' \otimes_A F)$ và $\operatorname{Im}(E \otimes_A F')$ là các $\mathbf{Z}$-môđun con của $E \otimes_A F$, là các ảnh tương ứng của các ánh xạ chính tắc $E' \otimes_A F \to E \otimes_A F$,

$$
E \otimes_A F' \to E \otimes_A F.
$$

Khi đó có một đẳng cấu $\mathbf{Z}$-môđun chính tắc*

$$(20)\quad \pi : (E/E') \otimes_A (F/F') \to (E \otimes_A F)/(\operatorname{Im}(E' \otimes_A F) + \operatorname{Im}(E \otimes_A F'))$$

*sao cho, với $\xi \in E/E'$, $\eta \in F$, $\pi(\xi \otimes \eta)$ là lớp của mọi phần tử $x \otimes y \in E \otimes_A F$ sao cho $x \in \xi$ và $y \in \eta$.

Chú ý rằng khi $E$ là một $((B'_i); A, (C'_j))$-đa môđun, $F$ là một $(A, (B''_h); (C''_k))$-đa môđun và $E'$ và $F'$ lần lượt là các *đa môđun con* của $E$ và $F$, thì đẳng cấu (20) là một đẳng cấu đối với các cấu trúc $((B'_i), (B''_h); (C'_j), (C''_k))$-đa môđun của hai vế (no. 3).

#### Hệ quả 2 {#alg-ii-s3-prop-6-cor-2 .statement}

*Cho $a$ là một iđêan phải của $A$, $F$ là một A-môđun trái và $aF$ là $\mathbf{Z}$-môđun con của $F$ sinh bởi các phần tử dạng $\lambda x$, trong đó $\lambda \in a$ và $x \in F$. Khi đó có một đẳng cấu $\mathbf{Z}$-môđun chính tắc*

$$(21)\quad \pi : (A/a) \otimes_A F \to F/aF$$

*sao cho, với mọi $\bar{\lambda} \in A/a$ và mọi $x \in F$, $\pi(\bar{\lambda} \otimes x)$ là lớp mod. $aF$ của $\lambda x$, trong đó $\lambda \in \bar{\lambda}$.

Đặc biệt, với $A = \mathbf{Z}$, ta thấy rằng với mọi số nguyên $n$ và mọi $\mathbf{Z}$-môđun $F$, $(\mathbf{Z}/n\mathbf{Z}) \otimes_{\mathbf{Z}} F$ được đồng nhất một cách chính tắc với $\mathbf{Z}$-môđun thương $F/nF$.

#### Hệ quả 3 {#alg-ii-s3-prop-6-cor-3 .statement}

Cho $A$ là một vành giao hoán, $a$ là một iđêan của $A$ và $E$ và $F$ là hai $A$-môđun sao cho $a$ được chứa trong linh hóa tử của $F$. Khi đó các $(A/a)$-môđun $E \otimes_A F$ và $(E/aE) \otimes_{A/a} F$ đẳng cấu chính tắc.

$F$ và $E \otimes_A F$ bị triệt tiêu bởi $a$ và do đó có các cấu trúc $(A/a)$-môđun chính tắc ($§ 1$, no. 12) và nếu ta viết $E' = aE$, thì $\operatorname{Im}(E' \otimes_A F) = 0$; khi đó có một đẳng cấu chính tắc (20) từ $E \otimes_A F$ lên $(E/aE) \otimes_A F$ và môđun sau này tự nó đồng nhất với $(E/aE) \otimes_{A/a} F$ (no. 3, Hệ quả của Mệnh đề 2).

#### Hệ quả 4 {#alg-ii-s3-prop-6-cor-4 .statement}

Cho $a, b$ là hai iđêan trong một vành giao hoán $C$; khi đó $C$-môđun $(C/a) \otimes_C (C/b)$ đẳng cấu chính tắc với $C(a + b)$.

### 7. TÍCH TENXƠ CỦA CÁC TÍCH VÀ CÁC TỔNG TRỰC TIẾP

Cho $(E_\lambda)_{\lambda \in L}$ là một họ các $A$-môđun phải, $(F_\mu)_{\mu \in M}$ là một họ các $A$-môđun trái và xét các môđun tích $C = \prod_{\lambda \in L} E_\lambda, D = \prod_{\mu \in M} F_\mu$. Ánh xạ $((x_\lambda), (y_\mu)) \mapsto (x_\lambda \otimes y_\mu)$ từ $C \times D$ vào $\mathbf{Z}$-môđun tích
$$
\prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$
là song tuyến tính trên $\mathbf{Z}$ và hiển nhiên thỏa mãn các điều kiện (1) (no. 1). Vì vậy tồn tại (no. 1, Mệnh đề 1) một ánh xạ tuyến tính trên $\mathbf{Z}$, gọi là chính tắc,
$$
f : \left( \prod_{\lambda \in L} E_\lambda \right) \otimes_A \left( \prod_{\mu \in M} F_\mu \right) \to \prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$
sao cho $f((x_\lambda) \otimes (y_\mu)) = (x_\lambda \otimes y_\mu)$.

Khi $C = R^L, D = S^M, R$ (resp. $S$) là một $A$-môđun phải (resp. trái), ánh xạ chính tắc (22) gắn với mọi tích tenxơ $u \otimes v$, trong đó $u$ là một ánh xạ từ $L$ vào $R$ và $v$ là một ánh xạ từ $M$ vào $S$, ánh xạ $(\lambda, \mu) \mapsto u(\lambda) \otimes v(\mu)$ từ $L \times M$ vào $R \otimes_A S$; ngay cả trong trường hợp này ánh xạ chính tắc (22) nói chung cũng không đơn ánh cũng không toàn ánh (Bài tập 3; xem Hệ quả 3 của Mệnh đề 7).

Khi các $E_\lambda$ là các đa môđun $((B'_i); A, (C'_j))$ và các $F_\mu$ là các đa môđun $(A, (B''_h); (C''_{k_c}))$, đồng cấu (22) cũng là một đồng cấu đối với các cấu trúc đa môđun $((B'_i), (B''_h); (C'_j), (C''_{k_c}))$ của hai vế.

Xét bây giờ môđun con $E = \bigoplus_{\lambda \in L} E_\lambda$ (resp. $\bigoplus_{\mu \in M} F_\mu$) của $C$ (resp. $D$); các đơn cấu chính tắc $E \to C, F \to D$ xác định một cách chính tắc một ánh xạ $\mathbf{Z}$-tuyến tính $E \otimes_A F \to C \otimes_A D$ mà khi hợp thành với ánh xạ (22) cho một ánh xạ $\mathbf{Z}$-tuyến tính $g$ từ $E \otimes_A F$ vào $\prod_{\lambda, \mu} (E_\lambda \otimes_A F_\mu)$ sao cho
$$
g((x_\lambda) \otimes (y_\mu)) = (x_\lambda \otimes y_\mu);
$$

hơn nữa, vì các họ $(x_\lambda)$ và $(y_\mu)$ có giá hữu hạn nên $(x_\lambda \otimes y_\mu)$ cũng vậy và do đó cuối cùng $g$ là một đồng cấu chính tắc

$$
g : \left( \bigoplus_{\lambda \in L} E_\lambda \right) \otimes_A \left( \bigoplus_{\mu \in M} F_\mu \right) \to \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu),
$$

là một đồng cấu đa môđun trong cùng các điều kiện như (22).

#### Mệnh đề 7 {#alg-ii-s3-prop-7 .statement}

*Ánh xạ chính tắc (23) là song ánh.*

Để chứng minh điều này, chỉ cần định nghĩa một ánh xạ $\mathbf{Z}$-tuyến tính $h$ từ tổng trực tiếp $G = \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)$ vào $E \otimes_A F$ sao cho $g \circ h$ và $h \circ g$ là các ánh xạ đồng nhất. Nhưng để định nghĩa một ánh xạ $\mathbf{Z}$-tuyến tính từ $G$ vào $E \otimes_A F$, chỉ cần (§ 1, no. 6, Mệnh đề 6) định nghĩa một ánh xạ $\mathbf{Z}$-tuyến tính

$$
h_{\lambda \mu} : E_\lambda \otimes_A F_\mu \to E \otimes_A F
$$

cho mọi cặp có thứ tự $(\lambda, \mu)$, và ta lấy $h_{\lambda \mu} = i_\lambda \otimes j_\mu$, trong đó $i_\lambda : E_\lambda \to E$ và $j_\mu : F_\mu \to F$ là các đơn cấu chính tắc. Khi đó rõ ràng $h \circ g$ trùng với ánh xạ đồng nhất trên các phần tử dạng $\left( \sum_\lambda x_\lambda \right) \otimes \left( \sum_\mu y_\mu \right)$ sinh ra $\mathbf{Z}$-môđun $E \otimes_A F$; tương tự, $g \circ h$ trùng với ánh xạ đồng nhất trên các phần tử dạng $\sum_{\lambda, \mu} (x_\lambda \otimes y_\mu)$ sinh ra $\mathbf{Z}$-môđun $G$, vì với mỗi cặp có thứ tự $(\lambda, \mu)$, các tích

$$
x_\lambda \otimes y_\mu \quad (x_\lambda \in E_\lambda, y_\mu \in F_\mu)
$$

sinh ra $\mathbf{Z}$-môđun $E_\lambda \otimes_A F_\mu$. Do đó suy ra mệnh đề.

Cho $u_\lambda : E_\lambda \to E'_\lambda$, $v_\mu : F_\mu \to F'_\mu$ là các đồng cấu $A$; rõ ràng biểu đồ

$$
\begin{array}{ccc}
\left( \bigoplus_\lambda E_\lambda \right) \otimes_A \left( \bigoplus_\mu F_\mu \right) & \longrightarrow & \bigoplus_{\lambda, \mu} (E_\lambda \otimes_A (F_\mu)) \\
(\bigoplus u_\lambda) \otimes (\bigoplus v_\mu) \downarrow & & \downarrow (\bigoplus (u_\lambda \otimes v_\mu)) \\
\left( \bigoplus_\lambda E'_\lambda \right) \otimes_A \left( \bigoplus_\mu F'_\mu \right) & \longrightarrow & \bigoplus_{\lambda, \mu} (E'_\lambda \otimes_A F'_\mu)
\end{array}
$$

là giao hoán.

#### Hệ quả 1 {#alg-ii-s3-prop-7-cor-1 .statement}

*Nếu $A$-môđun trái $F$ thừa nhận một cơ sở $(b_\mu)_{\mu \in M}$, thì mọi phần tử của $E \otimes_A F$ có thể được viết duy nhất dưới dạng $\sum_\mu (x_\mu \otimes b_\mu)$, trong đó $x_\mu \in E$ và họ $(x_\mu)$ có giá hữu hạn. $\mathbf{Z}$-môđun $E \otimes_A F$ đẳng cấu với $E^{(M)}$ được xét như một $\mathbf{Z}$-môđun.*

Cơ sở $(b_\mu)$ xác định một đẳng cấu của $F$ lên $\bigoplus_{\mu \in M} Ab_\mu$, do đó theo Mệnh đề 7 có một đẳng cấu $E \otimes_A F \to \bigoplus_{\mu \in M} (E \otimes_A Ab_\mu)$; vì ξ ↦ ξb_μ là một đẳng cấu của A_s lên Ab_μ, nên x ↦ x ⊗ b_μ là một đẳng cấu của E lên E ⊗_A (Ab_μ) theo Mệnh đề 4 của no. 4, do đó suy ra hệ quả.

Nếu E là một đa môđun $((B'_i); A, (C'_j))$, thì đẳng cấu chính tắc E ⊗_A F → E^{(M)} là một đẳng cấu đa môđun $((B'_i); (C'_j))$.

Đặc biệt, nếu E cũng có một cơ sở (a_λ)_{λ ∈ L}, thì mọi z ∈ E ⊗_A F đều có thể được viết dưới dạng $\sum_{λ, μ} (a_λ ξ_{λμ}) ⊗ b_μ$ theo một và chỉ một cách, trong đó các ξ_{λμ} thuộc A (và tạo thành một họ có giá hữu hạn); ánh xạ $z ↦ (\xi_{λμ})_{(λ, μ) ∈ L × M}$ là một đẳng cấu của E ⊗_A F lên A^{(L × M)} đối với các cấu trúc $\mathbf{Z}$-môđun (và thậm chí cả các cấu trúc môđun trên tâm của A). Cụ thể hơn:

#### Hệ quả 2 {#alg-ii-s3-prop-7-cor-2 .statement}

*Nếu E và F là hai môđun tự do trên một vành giao hoán C và (a_λ) (resp. (b_μ)) là một cơ sở của C-môđun E (resp. F), thì (a_λ ⊗ b_μ) là một cơ sở của C-môđun E ⊗_C F.*

Do lạm dụng ngôn ngữ, cơ sở (a_λ ⊗ b_μ) đôi khi được gọi là *tích tenxơ* của các cơ sở (a_λ) và (b_μ).

*Nhận xét (1)*. Cho E là một A-môđun phải tự do, F là một A-môđun trái tự do, (a_λ)_{λ ∈ L} một cơ sở của E và (b_μ)_{μ ∈ M} một cơ sở của F. Mọi phần tử z ∈ E ⊗_A F đều có thể được viết duy nhất dưới dạng $\sum_λ a_λ ⊗ y_λ$, trong đó y_λ ∈ F, và cũng được viết duy nhất dưới dạng $\sum_μ x_μ ⊗ b_μ$, trong đó x_μ ∈ E. Nếu ta viết $y_λ = \sum_μ η_{λμ} b_μ$, $x_μ = \sum_λ a_λ ξ_{λμ}$, trong đó các ξ_{λμ} và η_{λμ} thuộc A, thì $ξ_{λμ} = η_{λμ}$ với mọi (λ, μ), vì

$$
\sum_λ \left( a_λ ⊗ \left( \sum_μ η_{λμ} b_μ \right) \right) = \sum_{λ, μ} ((a_λ η_{λμ}) ⊗ b_μ) = \sum_μ \left( \left( \sum_λ a_λ η_{λμ} \right) ⊗ b_μ \right).
$$

#### Hệ quả 3 {#alg-ii-s3-prop-7-cor-3 .statement}

*Cho (E_λ)_{λ ∈ L} là một họ các A-môđun phải và F là một A-môđun trái tự do (resp. tự do sinh hữu hạn). Khi đó ánh xạ chính tắc (22)

$$
\left( \prod_{λ ∈ L} E_λ \right) ⊗_A F → \prod_{λ ∈ L} (E_λ ⊗_A F)
$$

là đơn ánh (resp. song ánh).

Nếu (b_μ) là một cơ sở của F, mọi phần tử của $\left( \prod_{λ ∈ L} E_λ \right) ⊗_A F$ có thể được viết duy nhất dưới dạng $z = \sum_μ ((x_λ^{(μ)}) ⊗ b_μ)$ (Hệ quả 1); nói rằng ảnh chính tắc của nó bằng không có nghĩa là, với mọi λ ∈ L, $\sum_μ (x_λ^{(μ)} ⊗ b_μ) = 0$, do đó $x_λ^{(μ)} = 0$ với mọi λ ∈ L và mọi μ (Hệ quả 1) và vì thế $z = 0$.

Việc chứng minh rằng ánh xạ chính tắc là song ánh khi F có một cơ sở hữu hạn được quy ngay lập tức, theo Mệnh đề 7, về trường hợp

F = A_s; nhưng khi đó hai vế được đồng nhất một cách chính tắc với $\prod_{\lambda \in L} E_\lambda$ (no. 4, Mệnh đề 4) và sau các sự đồng nhất này ánh xạ chính tắc (22) trở thành đồng nhất ánh xạ.

#### Hệ quả 4 {#alg-ii-s3-prop-7-cor-4 .statement}

*Cho A là một vành không có ước của không, E là một A-môđun phải tự do và F là một A-môđun trái tự do. Khi đó quan hệ x $\otimes$ y = 0 trong E $\otimes_A$ F kéo theo x = 0 hoặc y = 0.*

Cho $(a_\lambda)$ là một cơ sở của E, $(b_\mu)$ là một cơ sở của F và đặt $x = \sum_\lambda a_\lambda \xi_\lambda, y = \sum_\mu \eta_\mu b_\mu$; khi đó $x \otimes y = \sum_{\lambda, \mu} ((a_\lambda \xi_\lambda \eta_\mu) \otimes b_\mu$ và quan hệ $x \otimes y = 0$ kéo theo $\xi_\lambda \eta_\mu = 0$ với mọi cặp chỉ số có thứ tự $(\lambda, \mu)$ (Hệ quả 1). Do đó, nếu $x \neq 0$, tức là $\xi_\lambda \neq 0$ với ít nhất một $\lambda$, thì suy ra $\eta_\mu = 0$ với mọi $\mu$, do đó $y = 0$.

#### Hệ quả 5 {#alg-ii-s3-prop-7-cor-5 .statement}

*Cho E là một A-môđun phải, F là một A-môđun trái, M là một môđun con của E và N là một môđun con của F. Nếu M là một nhân tử trực tiếp của E và N là một nhân tử trực tiếp của F, thì đồng cấu chính tắc $M \otimes_A N \to E \otimes_A F$ là đơn ánh và ảnh của $M \otimes_A N$ dưới đồng cấu này là một nhân tử trực tiếp của $\mathbf{Z}$-môđun $E \otimes_A F$.*

Điều này suy ra ngay lập tức từ Mệnh đề 7.

Chú ý rằng nếu E là một đa môđun $((B'_i); A, (C'_j))$ và F là một đa môđun $(A, (B''_h); (C''_k))$ và M và N là các nhân tử trực tiếp trong các đa môđun này, thì $M \otimes N$ là một nhân tử trực tiếp của đa môđun $((B'_i), (B''_h); (C'_j), (C''_k))$ $E \otimes F$.

#### Hệ quả 6 {#alg-ii-s3-prop-7-cor-6 .statement}

*Cho P là một A-môđun trái xạ ảnh và E, F là hai A-môđun phải. Với mọi đơn cấu $u : E \to F$, đồng cấu*
$$
u \otimes 1_P : E \otimes_A P \to F \otimes_A P
$$
*là đơn ánh.*

Tồn tại một A-môđun trái Q sao cho $L = P \oplus Q$ là tự do (§ 2, no. 2, Mệnh đề 4) và $u \otimes 1_L$ được đồng nhất (Mệnh đề 7) với
$$(u \otimes 1_P) \oplus (u \otimes 1_Q);$$
do đó chỉ cần chứng minh hệ quả trong trường hợp P là *tự do* (§ 1, no. 6, Hệ quả 1 của Mệnh đề 7). Lập luận tương tự quy bài toán về trường hợp $P = A_s$, trường hợp này suy ra ngay lập tức từ no. 4, Mệnh đề 4.

#### Hệ quả 7 {#alg-ii-s3-prop-7-cor-7 .statement}

*Cho C là một vành giao hoán. Nếu E và F là hai C-môđun xạ ảnh, thì $E \otimes_C F$ là một C-môđun xạ ảnh.*

Điều này suy ra ngay lập tức từ Hệ quả 5 và thực tế là tích tenxơ của hai C-môđun tự do là một C-môđun tự do (Hệ quả 2).

#### Nhận xét 2 {#alg-ii-s3-n7-rem-2 .statement}

Dưới các giả thiết của Mệnh đề 7, cho $E'_\lambda$ là một môđun con của $E_\lambda$, $F'_\mu$ là một môđun con của $F_\mu$ và đặt $E' = \bigoplus_{\lambda \in L} E'_\lambda$, $F' = \bigoplus_{\mu \in M} F'_\mu$. Gọi Im$(E' \otimes_A F')$ (resp. Im(E'_λ ⊗_A F'_μ)) là ảnh của E' ⊗_A F' (resp. E'_λ ⊗_A F'_μ) trong E ⊗_A F (resp. E_λ ⊗_A F_μ) dưới ánh xạ chính tắc; khi đó đẳng cấu (23) đồng nhất các môđun con-$\mathbf{Z}$

$$
\operatorname{Im}(E' \otimes_A F') \quad \text{và} \quad \bigoplus_{(\lambda, \mu) \in I \times M} \operatorname{Im}(E'_\lambda \otimes_A F'_\mu);
$$

điều này suy ra ngay lập tức từ tính giao hoán của biểu đồ

$$
\begin{array}{ccc}
\left( \bigoplus_\lambda E'_\lambda \right) \otimes_A \left( \bigoplus_\mu F'_\mu \right) & \longrightarrow & \left( \bigoplus_\lambda E_\lambda \right) \otimes_A \left( \bigoplus_\mu F_\mu \right) \\
\downarrow & & \downarrow \\
\bigoplus_{\lambda, \mu} (E'_\lambda \otimes_A F'_\mu) & \longrightarrow & \bigoplus_{\lambda, \mu} (E_\lambda \otimes_A F_\mu)
\end{array}
$$

trong đó các mũi tên thẳng đứng là các đẳng cấu chính tắc.

### 8. TÍNH KẾT HỢP CỦA TÍCH TENXƠ

#### Mệnh đề 8 {#alg-ii-s3-prop-8 .statement}

*Cho A, B là hai vành, E một A-môđun phải, F một song môđun (A, B) và G một B-môđun trái. Khi đó E ⊗_A F là một B-môđun phải, F ⊗_B G là một A-môđun trái và tồn tại một và chỉ một ánh xạ $\mathbf{Z}$-tuyến tính*

$$
\phi : (E \otimes_A F) \otimes_B G \to E \otimes_A (F \otimes_B G)
$$

*thỏa mãn* $\phi((x \otimes y) \otimes z) = x \otimes (y \otimes z)$ *với* $x \in E,\ y \in F,\ z \in G;$ hơn nữa *ánh xạ $\mathbf{Z}$-tuyến tính này là song ánh* ("tính kết hợp" của tích tenxơ).

Cấu trúc B-môđun phải trên E ⊗_A F và cấu trúc A-môđun trái trên F ⊗_B G đã được định nghĩa ở no. 4. Tính duy nhất của $\phi$ là hiển nhiên vì các phần tử $(x \otimes y) \otimes z$ sinh ra $\mathbf{Z}$-môđun $(E \otimes_A F) \otimes_B G$. Để chứng minh sự tồn tại của $\phi$, ta chú ý rằng, với mọi $z \in G,\ h_z : y \mapsto y \otimes z$ là một ánh xạ A-tuyến tính từ A-môđun trái F vào A-môđun trái F ⊗_B G. Ta viết $g_z = 1_E \otimes h_z$, do đó đây là một ánh xạ $\mathbf{Z}$-tuyến tính từ E ⊗_A F vào E ⊗_A (F ⊗_B G) và xét ánh xạ $(t, z) \mapsto g_z(t)$ từ $(E \otimes_A F \times G$ vào $E \otimes_A (F \otimes_B G)$; vì $h_{z + z'} = h_z + h_{z'}$ với $z \in G,\ z' \in G$, hiển nhiên là ánh xạ trên là $\mathbf{Z}$-song tuyến tính. Hơn nữa, ta chứng minh rằng với mọi $\mu \in B,\ g_{\mu z}(t) = g_z(t \mu)$; hiển nhiên là chỉ cần làm điều này với $t = x \otimes y$ trong đó $x \in E$ và $y \in F$; khi đó

$$
g_{\mu z}(x \otimes y) = x \otimes (y \otimes \mu z)
$$
$$
g_z((x \otimes y)\mu) = g_z(x \otimes y\mu) = x \otimes (y\mu \otimes z).
$$

Mệnh đề 1 (no. 1) khi đó chứng minh sự tồn tại của một ánh xạ $\mathbf{Z}$-tuyến tính

$$
\phi : (E \otimes_A F) \otimes_B G \to E \otimes_A (F \otimes_B G)
$$

thỏa mãn $\phi(t \otimes z) = g_z(t)$, do đó $\phi((x \otimes y) \otimes z) = x \otimes (y \otimes z)$. Tương tự, một ánh xạ $\mathbf{Z}$-tuyến tính

$$
\psi : E \otimes_A (F \otimes_B G) \to (E \otimes_A F) \otimes_B G
$$

được định nghĩa sao cho $\psi(x \otimes (y \otimes z)) = (x \otimes y) \otimes z$ và hiển nhiên $\psi \circ \phi$ và $\phi \circ \psi$ lần lượt là các ánh xạ đồng nhất của $(E \otimes_A F) \otimes_B G$ và $E \otimes_A (F \otimes_B G)$, vì chúng rút gọn thành các ánh xạ đồng nhất trên các hệ sinh của các $\mathbf{Z}$-môđun này.

Hiển nhiên là, nếu $E$ là một đa môđun $((C'_i); A, (D'_j))$, $F$ là một đa môđun $(A, (C''_h); B, (D''_k))$ và $G$ là một đa môđun $(B, (C'''_l); (D'''_m))$, thì đẳng cấu chính tắc được định nghĩa trong Mệnh đề 8 là một đẳng cấu đa môđun $((C'_i), (C''_h), (C'''_l); (D'_j), (D''_k), (D'''_m))$. Đặc biệt, nếu $C$ là một vành *giao hoán* và $E, F, G$ là ba $C$-môđun, thì có một đẳng cấu chính tắc C-môđun

$$
(E \otimes_C F) \otimes_C G \to E \otimes_C (F \otimes_C G).
$$

Ta sẽ thấy ở dưới rằng, dưới những điều kiện nào đó, định nghĩa của tích tenxơ có thể được tổng quát hóa cho một họ các đa môđun, điều này đặc biệt sẽ cho ta dưới các giả thiết của Mệnh đề 8 một $\mathbf{Z}$-môđun $E \otimes_A F \otimes_B G$, đẳng cấu chính tắc với mỗi $\mathbf{Z}$-môđun $(E \otimes_A F) \otimes_B G$ và $E \otimes_A (F \otimes_B G)$, và các môđun sau này sẽ được đồng nhất với nó.

### 9. TÍCH TENXƠ CỦA CÁC HỌ ĐA MÔĐUN

Cho $(G_\lambda)_{\lambda \in L}$ là một họ các $\mathbf{Z}$-môđun; một ánh xạ $u$ từ tập hợp $G = \prod_{\lambda \in L} G_\lambda$ vào một $\mathbf{Z}$-môđun được gọi là *đa cộng tính* (hay $\mathbf{Z}$-*đa tuyến tính*) nếu $(x_\lambda) \mapsto u((x_\lambda))$ là cộng tính đối với từng biến $x_\lambda$; nói chính xác hơn, điều này có nghĩa là, với mọi $\mu \in L$ và mọi phần tử $(a_\lambda) \in \prod_{\lambda \neq \mu} G_\lambda$, bằng cách đồng nhất một cách chính tắc $G$ với $G_\mu \times \prod_{\lambda \neq \mu} G_\lambda$,

$$
u(x_\mu + y_\mu, (a_\lambda)) = u(x_\mu, (a_\lambda)) + u(y_\mu, (a_\lambda)) \quad \text{với } x_\mu, y_\mu \text{ thuộc } G_\mu.
$$

Điều này đặc biệt suy ra rằng $u((x_\lambda)) = 0$ nếu một trong các $x_\lambda$ bằng không.

Ta cũng xét *bài toán ánh xạ phổ quát* trong đó $\Sigma$ là loài các cấu trúc $\mathbf{Z}$-môđun và các ánh xạ $\alpha$ là các ánh xạ đa cộng tính từ $G$ vào một $\mathbf{Z}$-môđun. Một nghiệm vẫn thu được bằng cách xét $\mathbf{Z}$-môđun $C = \mathbf{Z}^{(G)}$ gồm các tổ hợp tuyến tính hình thức của các phần tử của $G$ với hệ số trong $\mathbf{Z}$ và môđun con-$\mathbf{Z}$ $D$ của $C$ sinh bởi các phần tử có dạng

$$
(x_\mu + y_\mu, (z_\lambda)_{\lambda \neq \mu}) - (x_\mu, (z_\lambda)_{\lambda \neq \mu}) - (y_\mu, (z_\lambda)_{\lambda \neq \mu})
$$

trong đó $\mu \in L, x_\mu \in G_\mu, y_\mu \in G_\mu$ và các $z_\lambda \in G_\lambda$ ($\lambda \neq \mu$) là tùy ý. $\mathbf{Z}$-môđun thương $C/D$ được gọi là *tích tenxơ (trên $\mathbf{Z}$) của họ* $(G_\lambda)_{\lambda \in L}$ các $\mathbf{Z}$-*môđun* và được ký hiệu bởi $\bigotimes_{\lambda \in L} G_\lambda$; với mọi phần tử $(x_\lambda)_{\lambda \in L}$ của $G$ là một phần tử của cơ sở chính tắc của $C$, $\bigotimes_{\lambda \in L} x_\lambda$ ký hiệu ảnh chính tắc của phần tử này trong C/D. Từ các định nghĩa trên suy ra rằng ánh xạ $\phi : (x_\lambda) \mapsto \bigotimes_{\lambda \in L} x_\lambda$ từ G vào $\bigotimes_{\lambda \in L} G_\lambda$ là $\mathbf{Z}$-đa tuyến tính và rằng, với mọi ánh xạ $\mathbf{Z}$-đa tuyến tính $f$ từ G vào một $\mathbf{Z}$-môđun H, tồn tại một và chỉ một ánh xạ $\mathbf{Z}$-tuyến tính $g : \bigotimes_{\lambda \in L} G_\lambda \to H$ sao cho $f = g \circ \phi$; do đó cặp có thứ tự $\left( \bigotimes_{\lambda \in L} G_\lambda, \phi \right)$ giải quyết bài toán ánh xạ phổ quát đang xét.

Cho $(G'_\lambda)_{\lambda \in L}$ là một họ khác các $\mathbf{Z}$-môđun và, với mọi $\lambda \in L$, cho $v_\lambda : G_\lambda \to G'_\lambda$ là một ánh xạ $\mathbf{Z}$-tuyến tính (nói cách khác là một đồng cấu các nhóm giao hoán). Khi đó ánh xạ
$$
(x_\lambda) \mapsto \bigotimes_{\lambda \in L} v_\lambda(x_\lambda)
$$
từ G vào $\bigotimes_{\lambda \in L} G'_\lambda$ là $\mathbf{Z}$-đa tuyến tính và do đó xác định một cách chính tắc một ánh xạ $\mathbf{Z}$-tuyến tính từ $\bigotimes_{\lambda \in L} G_\lambda$ vào $\bigotimes_{\lambda \in L} G'_\lambda$ được ký hiệu là $\bigotimes_{\lambda \in L} v_\lambda$ và sao cho
$$
\left( \bigotimes_{\lambda \in L} v_\lambda \right) \left( \bigotimes_{\lambda \in L} x_\lambda \right) = \bigotimes_{\lambda \in L} v_\lambda(x_\lambda).
$$
Đặc biệt, xét, với một $\mu \in L$ nào đó, một tự đồng cấu $\theta$ của $G_\mu$; ta ký hiệu bởi $\tilde{\theta}$ tự đồng cấu của $\bigotimes_{\lambda \in L} G_\lambda$ bằng với $\bigotimes_{\lambda \in L} v_\lambda$ trong đó $v_\mu = \theta$ và $v_\lambda = 1_{G_\lambda}$ với $\lambda \neq \mu$.

Tiếp đó giả sử đã cho một tập hợp $\Omega$, một ánh xạ
$$
c : \omega \mapsto (\rho(\omega), \sigma(\omega))
$$
từ $\Omega$ vào $L \times L$ và, với mọi $\omega \in \Omega$, một tự đồng cấu $p_\omega$ của $G_{\rho(\omega)}$ và một tự đồng cấu $q_\omega$ của $G_{\sigma(\omega)}$; tương ứng với chúng là hai tự đồng cấu $\tilde{p}_\omega$ và $\tilde{q}_\omega$ của $P = \bigotimes_{\lambda \in L} G_\lambda$. Cho R là môđun con-$\mathbf{Z}$ của P *được sinh bởi hợp các ảnh của các tự đồng cấu* $\tilde{p}_\omega - \tilde{q}_\omega$ khi $\omega$ chạy qua $\Omega$. $\mathbf{Z}$-môđun thương $P/R$ được gọi là *tích tenxơ của họ* $(G_\lambda)_{\lambda \in L}$ *đối với* c, p, q và được ký hiệu là $\bigotimes_{(c, p, q)} G_\lambda$; hợp thành đồng cấu chính tắc $P \to P/R$ với ánh xạ $\phi : G \to \bigotimes_{\lambda \in L} G_\lambda$ được định nghĩa ở trên, ta thu được một ánh xạ $\mathbf{Z}$-đa tuyến tính $\phi_{(c, p, q)} : G \to \bigotimes_{(c, p, q)} G_\lambda$ và viết $\phi_{(c, p, q)}((x_\lambda)) = \bigotimes_{(c, p, q)} x_\lambda$ hoặc đơn giản là $\bigotimes_{(c)} x_\lambda$. Cặp có thứ tự gồm $\bigotimes_{(c, p, q)} x_\lambda$ và $\phi_{(c, p, q)}$ giải quyết *bài toán ánh xạ phổ quát* sau đây: ký hiệu bởi $\bar{p}_\omega$ (tương ứng $\bar{q}_\omega$) ánh xạ
$$
(x_{\rho(\omega)}, (x_\lambda)_{\lambda \neq \rho(\omega)}) \mapsto (p_\omega(x_{\rho(\omega)}), (x_\lambda)_{\lambda \neq \rho(\omega)})
$$
(tương ứng $(x_{\sigma(\omega)}, (x_\lambda)_{\lambda \neq \sigma(\omega)}) \mapsto (q_\omega(x_{\sigma(\omega)}), (x_\lambda)_{\lambda \neq \sigma(\omega)})$)
từ G vào chính nó. Khi đó $\Sigma$ được lấy là loài cấu trúc $\mathbf{Z}$-môđun và các ánh xạ α là các ánh xạ $\mathbf{Z}$-đa tuyến tính $u$ từ $G$ vào một $\mathbf{Z}$-môđun mà còn thỏa mãn các điều kiện

$$(26)$$
$$
u \circ \bar{p}_\omega = u \circ \bar{q}_\omega
$$

với mọi $\omega \in \Omega$. Chứng minh là hiển nhiên từ các định nghĩa trên.

Phép dựng này đặc biệt cho lại phép dựng của $E \otimes_A F$ đã được mô tả ở no. 1: trong trường hợp này ta lấy $L = \{1, 2\}$, $G_1 = E$, $G_2 = F$, $\Omega = A$; hơn nữa, với mọi $\omega \in A$, phải có $\rho(\omega) = 1$, $\sigma(\omega) = 2$, $\omega$ là tự đồng cấu $x \mapsto x\omega$ của $\mathbf{Z}$-môđun $E$ và $q_\omega$ là tự đồng cấu $y \mapsto \omega y$ của $\mathbf{Z}$-môđun $F$.

Cho $(G'_\lambda)_{\lambda \in L}$ là một họ thứ hai các $\mathbf{Z}$-môđun; vẫn giữ nguyên ánh xạ $c$, giả sử rằng với mọi $\omega \in \Omega$, đã cho một tự đồng cấu $p'_\omega$ của $G'_{\rho(\omega)}$ và một tự đồng cấu $q'_\omega$ của $G'_{\sigma(\omega)}$. Khi đó, với mọi $\lambda \in L$, cho $v_\lambda : G_\lambda \to G'_\lambda$ là một ánh xạ tuyến tính trên $\mathbf{Z}$ sao cho, với mọi $\omega \in \Omega$,

$$(27)$$
$$
v_{\rho(\omega)} \circ p_\omega = p'_\omega \circ v_{\rho(\omega)} \quad \text{và} \quad v_{\sigma(\omega)} \circ q_\omega = q'_\omega \circ v_{\sigma(\omega)}
$$

(nói cách khác, với mọi $\lambda \in L$, $v_\lambda$ là một cấu xạ đối với các luật tác động trên $G_\lambda$ (resp. $G'_\lambda$) được xác định bởi các $p_\xi$ và $q_\eta$ (resp. $p'_\xi$ và $q'_\eta$), với $\xi$ và $\eta$ sao cho $\rho(\xi) = \lambda$ và $\sigma(\eta) = \lambda$). Khi đó ánh xạ
$$
u : (x_\lambda) \mapsto \bigotimes_{(c, p', q')} v_\lambda(x_\lambda)
$$
từ $G$ vào $\bigotimes_{(c, p', q')} G'_\lambda$ là $\mathbf{Z}$-đa tuyến tính và thỏa mãn các điều kiện (26), do đó xác định một ánh xạ tuyến tính trên $\mathbf{Z}$ từ $\bigotimes_{(c, p, q)} G_\lambda$ vào $\bigotimes_{(c, p', q')} G'_\lambda$, mà ta sẽ ký hiệu đơn giản là $\bigotimes_{(c)} v_\lambda$ nếu không thể có sự nhầm lẫn.

Bây giờ ta sẽ nêu một tính chất "kết hợp" đối với các tích tenxơ tổng quát đã được định nghĩa như trên. Cho $(L_i)_{1 \leq i \leq n}$ là một phân hoạch hữu hạn của $L$; với mỗi chỉ số $i$, ký hiệu $\Omega_i$ là tập con của $\Omega$ gồm các phần tử sao cho $\rho(\omega) \in L_i$ và $\sigma(\omega) \in L_i$; rõ ràng các $\Omega_i$ rời nhau từng đôi một; đặt $\Omega' = \Omega - \left( \bigcup_i \Omega_i \right)$. Với mỗi chỉ số $i$, $c^{(i)}$ sẽ ký hiệu ánh xạ $\omega \mapsto (\rho(\omega), \sigma(\omega))$ từ $\Omega_i$ vào $L_i \times L_i$; với $\omega \in \Omega_i$, ta viết $p^{(i)}_\omega$ và $q^{(i)}_\omega$ thay cho $p_\omega$ và $q_\omega$. Khi đó với mỗi $i$ có một tích tenxơ "bộ phận"
$$
F_i = \bigotimes_{(c^{(i)}, p^{(i)}, q^{(i)})} G_\lambda.
$$

Hơn nữa ta sẽ đặt giả thiết "hoán vị được" sau đây:

(P) *Nếu $\omega \in \Omega'$, thì $p_\omega$ (resp. $q_\omega$) hoán vị với mỗi tự đồng cấu $p_\xi$ và $q_\eta$ của $G_{\rho(\omega)}$ (resp. $G_{\sigma(\omega)}$) sao cho $\xi \notin \Omega'$, $\eta \notin \Omega'$ và $\rho(\omega) = \rho(\xi) = \sigma(\eta)$ (resp. $\sigma(\omega) = \rho(\xi) = \sigma(\eta)$).*

Với mỗi $\omega \in \Omega'$, gọi $i$ là chỉ số sao cho $\rho(\omega) \in L_i$; khi đó xét họ $(v_\lambda)_{\lambda \in L_i}$ trong đó $v_{\rho(\omega)} = p_\omega$ và $v_\lambda = 1_{G_\lambda}$ với $\lambda \neq \rho(\omega)$; giả thiết (P) kéo theo rằng họ $(v_\lambda)$ thỏa mãn các điều kiện (27) (trong đó $p'$ và $p$ phải được thay bằng $p^{(i)}$, $q'$ và $q$ bằng $q^{(i)}$, $\omega$ bằng một phần tử $\xi$ chạy qua $\Omega_i$); do đó một tự đồng cấu $\bigotimes_{(c^{(i)})} v_\lambda = r_\omega$ được dẫn xuất của $\mathbf{Z}$-môđun $F_i$. Tương tự, một tự đồng cấu $s_\omega$ của $\mathbf{Z}$-môđun $F_j$ được định nghĩa từ $q_\omega$, trong đó $j$ là chỉ số sao cho $\sigma(\omega) \in L_j$; sau cùng đặt $d(\omega) = (i, j)$. Khi đó ta có thể định nghĩa *tích tenxơ* $\bigotimes_{(d, r, s)} F_i$ và ánh xạ chính tắc tương ứng

$$
\phi_{(d, r, s)} : \prod_{i=1}^n F_i \to \bigotimes_{(d, r, s)} F_i.
$$

Mặt khác, với mỗi $i$, ánh xạ chính tắc

$$
\psi_i = \phi_{(c^{(i)}, p^{(i)}, q^{(i)})} : \prod_{\lambda \in L_i} G_\lambda \to F_i;
$$

dùng tính kết hợp của tích các tập hợp, từ đó dẫn xuất một ánh xạ $\mathbf{Z}$-tuyến tính nhiều biến $\psi = \phi_{(d, r, s)} \circ (\psi_i)$ từ $G$ vào $\bigotimes_{(d, r, s)} F_i$. Ta chứng minh rằng *cặp có thứ tự* $\left( \bigotimes_{(d, r, s)} F_i, \psi \right)$ *là một nghiệm của cùng bài toán phổ quát như* $\left( \bigotimes_{(c, p, q)} G_\lambda, \phi_{(c, p, q)} \right)$, do đó sẽ suy ra sự tồn tại của một *đẳng cấu* $\mathbf{Z}$-môđun *duy nhất*

$$
\theta : \bigotimes_{(c, p, q)} G_\lambda \to \bigotimes_{(d, r, s)} F_i
$$

sao cho $\psi = \theta \circ \phi_{(c, p, q)}$ (*Lý thuyết tập hợp*, IV, § 3, no. 1).

Bằng quy nạp theo $n$, chứng minh được quy về trường hợp $n = 2$; để đơn giản ta viết $F_1 \otimes_{(d)} F_2$ và $y_1 \otimes_{(d)} y_2$ thay cho $\bigotimes_{(d, r, s)} F_i$ và $\bigotimes_{(d, r, s)} y_i$. Xét ánh xạ từ $G$ vào $F_1 \otimes_{(d)} F_2$

$$
h : (x_\lambda) \to \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \otimes_{(d)} \left( \bigotimes_{(c^{(2)})} x_\lambda \right).
$$

Nó hiển nhiên là $\mathbf{Z}$-tuyến tính nhiều biến; ta chứng minh rằng nó thỏa mãn các điều kiện (26) với mọi $\omega \in \Omega$. Điều này là hiển nhiên nếu $\omega \in \Omega_1$ hoặc $\omega \in \Omega_2$; nếu không, giả sử, để cụ thể hóa, rằng $\rho(\omega) \in L_1$ và $\sigma(\omega) \in L_2$, thì các giá trị của $h \circ \bar{p}_\omega$ và $h \circ \bar{q}_\omega$ tại $(x_\lambda)$ lần lượt là

$$
\left( r_\omega \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \right) \otimes_{(d)} \left( \bigotimes_{(c^{(2)})} x_\lambda \right) \quad \text{và} \quad \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \otimes_{(d)} \left( s_\omega \left( \bigotimes_{(c^{(2)})} x_\lambda \right) \right)
$$

mà cũng bằng nhau theo định nghĩa của $F_1 \otimes_{(d)} F_2$.

Khi đó, cho $u$ là một ánh xạ $\mathbf{Z}$-tuyến tính nhiều biến từ $G$ vào một $\mathbf{Z}$-môđun $H$, thỏa mãn các điều kiện (26); ta sẽ định nghĩa một ánh xạ $\mathbf{Z}$-tuyến tính $v : F_1 \otimes_{(d)} F_2 \to H$ sao cho $u = v \circ h$ và điều đó sẽ chứng minh mệnh đề của chúng ta (lặp lại lập luận của no. 1, Hệ quả 1 của Mệnh đề 1). Với mọi $z_2 = (x_\lambda)_{\lambda \in L_2}$ ta xét ánh xạ tuyến tính "bộ phận" từ $\prod_{\lambda \in L_1} G_\lambda$ vào $H$

$$
u(., z_2): (x_\lambda)_{\lambda \in L_1} \mapsto u((x_\lambda)_{\lambda \in L_1}, z_2) = u((x_\lambda)_{\lambda \in L}).
$$

Rõ ràng nó là $\mathbf{Z}$-tuyến tính nhiều biến và thỏa mãn các điều kiện (26) với $\omega \in \Omega_1$; do định nghĩa, vì vậy tồn tại một ánh xạ $\mathbf{Z}$-tuyến tính $y_1 \mapsto w_1(y_1, x_2)$ từ $F_1$ vào $H$ sao cho

$$
w_1\left( \bigotimes_{(c^{(1)})} x_\lambda, z_2 \right) = u((x_\lambda)_{\lambda \in L_1}, z_2)
$$

Tiếp theo ta xét ánh xạ

$$
u_2: (x_\lambda)_{\lambda \in L_2} \mapsto w_1(., (x_\lambda)_{\lambda \in L_2})
$$

của $\prod_{\lambda \in L_2} G_\lambda$ vào $\mathrm{Hom}_\mathbf{Z}(F_1, H)$; nó hiển nhiên là một ánh xạ $\mathbf{Z}$-đa tuyến tính và thỏa mãn các điều kiện (26) đối với $\omega \in \Omega_2$, nhờ giả thiết đặt trên $u$ và các quan hệ (28) và (29), đồng thời lưu ý rằng các phần tử có dạng $\bigotimes_{(c^{(1)})} x_\lambda$ sinh $\mathbf{Z}$-môđun $F_1$. Do đó có một ánh xạ $\mathbf{Z}$-tuyến tính

$$
w_2: F_2 \to \mathrm{Hom}_\mathbf{Z}(F_1, H)
$$

sao cho

$$
w_2\left( \bigotimes_{(c^{(2)})} x_\lambda \right) = u_2((x_\lambda)_{\lambda \in L_2})
$$

hay cũng là

$$
\left( w_2\left( \bigotimes_{(c^{(2)})} x_\lambda \right) \right)\left( \bigotimes_{(c^{(1)})} x_\lambda \right) = u((x_\lambda)_{\lambda \in L}).
$$

Bây giờ ta xét, với $y_1 \in F_1, y_2 \in F_2$, phần tử sau của $H$

$$
w(y_1, y_2) = (w_2(y_2))(y_1).
$$

Rõ ràng $w$ là một ánh xạ $\mathbf{Z}$-song tuyến tính từ $F_1 \times F_2$ vào $H$. Hơn nữa, ta sẽ chứng minh rằng, với mọi $\omega \in \Omega'$, (giả sử, để cố định ý tưởng, rằng $\rho(\omega) \in L_1$ và $\sigma(\omega) \in L_2$)

$$
w(r_\omega(y_1), y_2) = w(y_1, s_\omega(y_2)).
$$

Chỉ cần kiểm tra quan hệ này khi $y_1$ (tương ứng $y_2$) có dạng $\bigotimes_{(c^{(1)})} x_\lambda$ (tương ứng $\bigotimes_{(c^{(2)})} x_\lambda$), vì các phần tử ấy sinh $\mathbf{Z}$-môđun $F_1$ (tương ứng $F_2$). Nhưng theo định nghĩa, $r_\omega\left( \bigotimes_{(c^{(1)})} x_\lambda \right) = \bigotimes_{(c^{(1)})} x'_\lambda$, trong đó $x'_{\rho(\omega)} = p_\omega(x_{\rho(\omega)})$ và $x'_\lambda = x_\lambda$ với λ ≠ ρ(ω) trong L₁; tương tự s_ω\left(\bigotimes_{(c^{(2)})} x_\lambda\right) = \bigotimes_{(c^{(2)})} x''_\lambda, trong đó x''_{σ(ω)} = q_ω(x'_{σ(ω)}) và x''_\lambda = x_\lambda với λ ≠ σ(ω) trong L₂; dùng (30) và (31), khi đó quan hệ (32) suy ra từ (26). Do đó tồn tại một ánh xạ $\mathbf{Z}$-tuyến tính v từ F₁ ⊗ F₂ vào H sao cho $v(y_1 \otimes y_2) = w(y_1, y_2)$, và khi đó từ (30) và (31) suy ra rằng $v \circ h = u$.

Trường hợp đặc biệt quan trọng nhất của tích tenxơ tổng quát được định nghĩa ở trên là trường hợp sau đây: ta bắt đầu với một họ $(A_i)_{1 \leq i \leq n-1}$ các vành và một họ $(E_i)_{1 \leq i \leq n}$, trong đó $E_1$ là một môđun phải $A_1$, $E_n$ là một môđun trái $A_{n-1}$ và, với $2 \leq i \leq n-1$, $E_i$ là một song môđun $(A_{i-1}, A_i)$. Khi đó định nghĩa ở trên được áp dụng như sau: L là tập hợp $[1, n]$, $G_i = E_i$, Ω là tập hợp tổng của các $A_i$ ($1 \leq i \leq n-1$). Với $ω ∈ A_i$ ($1 \leq i \leq n-1$), lấy $ρ(ω) = i$, $σ(ω) = i + 1$, $p_ω$ là tự đồng cấu $x ↦ xω$ của $Z$-môđun $E_i$ và $q_ω$ là tự đồng cấu $y ↦ ωy$ của $Z$-môđun $E_{i+1}$; tích tenxơ tương ứng được ký hiệu là

$$
E_1 \otimes_{A_1} E_2 \otimes_{A_2} E_3 \otimes \cdots \otimes_{A_{n-2}} E_{n-1} \otimes_{A_{n-1}} E_n
$$

(một ký hiệu trong đó các $A_i$ đôi khi có thể được lược bỏ) và các phần tử $\bigotimes_{(c, p, q)} x_i$ của tích tenxơ này, với một họ $(x_i)$ sao cho $x_i ∈ E_i$ với $1 \leq i \leq n$, có thể được viết là $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ nếu không thể gây ra nhầm lẫn; một ký hiệu tương tự được dùng cho một ánh xạ tuyến tính $Z$ $\bigotimes_{(c)} v_i$. Giả thiết (P) đúng với mọi phân hoạch của $[1, n]$, vì các $E_i$ là song môđun với $2 \leq i \leq n-1$. Khi $n = 3$, như vậy ta đã định nghĩa $Z$-môđun $E \otimes_A F \otimes_B G$ được nhắc đến trong no. 8, và thu được lại Mệnh đề 8 (no. 8).

Khi mỗi $E_i$ là một môđun đa tạp (với, đối với $2 \leq i \leq n-1$, $A_{i-1}$ là một trong các vành tác động bên trái và $A_i$ là một trong các vành tác động bên phải, và các điều kiện tương tự đối với $i = 1$ và $i = n$), như trong no. 4, một cấu trúc môđun đa tạp được xác định trên $E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$ đối với tất cả các vành ngoại trừ các $A_i$ tác động trên $E_i$ ($1 \leq i \leq n$).

Đặc biệt, cho C là một vành giao hoán, $(E_i)_{1 \leq i \leq n}$ là một họ các C-môđun. Bằng cách trang bị cho $E_1$ và $E_n$ hai cấu trúc C-môđun đồng nhất với cấu trúc đã cho và cho $E_i$, với $2 \leq i \leq n-1$, ba cấu trúc C-môđun đồng nhất với cấu trúc đã cho, ta xác định trên tích tenxơ

$$
E_1 \otimes_C E_2 \otimes_C E_3 \otimes \cdots \otimes_C E_{n-1} \otimes_C E_n
$$

$n$ cấu trúc C-môđun tương thích với nhau và thực ra đồng nhất, vì với mọi $γ ∈ C$ và $(x_i) ∈ \prod_{i=1}^n E_i$, theo định nghĩa

$$
(γx_1) \otimes x_2 \otimes \cdots \otimes x_n \\
= x_1 \otimes (γx_2) \otimes \cdots \otimes x_n = \cdots = x_1 \otimes x_2 \otimes \cdots \otimes (γx_n).
$$

Khi ta nói đến tích tenxơ (34) như một C-môđun, ta sẽ luôn hiểu là với cấu trúc này, trừ khi có nói khác, và tích tenxơ (34) cũng được ký hiệu bởi $\bigotimes_{1 \leq i \leq n} E_i$ nếu không thể nảy sinh nhầm lẫn. Với mọi C-môđun G, các ánh xạ $\mathbf{Z}$-đa tuyến tính từ $\prod_{i=1}^n E_i$ vào G mà, với mọi chỉ số i, thỏa mãn quan hệ

$$
f(x_1, \ldots, x_{i-1}, \gamma x_i, x_{i+1}, \ldots, x_n) = \gamma f(x_1, \ldots, x_n)
$$

với $\gamma \in \mathbf{C}$ và $(x_i) \in \prod_i E_i$ khi đó được gọi là C-đa tuyến tính và tạo thành một C-môđun ký hiệu là $\mathcal{L}_n(E_1, \ldots, E_n; G)$; khi đó tính chất phổ quát của tích tenxơ (34) cho phép ta định nghĩa một đẳng cấu C-môđun chính tắc

$$
\mathcal{L}_n(E_1, \ldots, E_n; G) \to \operatorname{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n, G)
$$

gắn với mỗi ánh xạ C-đa tuyến tính f ánh xạ C-tuyến tính g sao cho

$$
f(x_1, \ldots, x_n) = g(x_1 \otimes x_2 \otimes \cdots \otimes x_n).
$$

Một ánh xạ C-đa tuyến tính từ $E_1 \times \cdots \times E_n$ vào $\mathbf{C}$ cũng được gọi là một dạng $n$-tuyến tính.

Cho $(F_i)_{1 \leq i \leq n}$ là một họ khác các C-môđun; với mọi hệ gồm n ánh xạ C-tuyến tính $u_i : E_i \to F_i, u_1 \otimes u_2 \otimes \cdots \otimes u_n$ (cũng được ký hiệu là $\bigotimes_{1 \leq i \leq n} u_i$) là một ánh xạ C-tuyến tính từ

$$
E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n \text{ vào } F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n.
$$

Hơn nữa, $(u_1, \ldots, u_n) \mapsto u_1 \otimes u_2 \otimes \cdots \otimes u_n$ là một ánh xạ C-đa tuyến tính từ $\prod_i \operatorname{Hom}_\mathbf{C}(E_i, F_i)$ vào

$$
\operatorname{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E \otimes \cdots \otimes_\mathbf{C} E_n, F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n).
$$

Do đó tương ứng một cách chính tắc với ánh xạ sau cùng một ánh xạ C-tuyến tính gọi là chính tắc

$$
\operatorname{Hom}_\mathbf{C}(E_1, F_1) \otimes_\mathbf{C} \operatorname{Hom}_\mathbf{C}(E_2, F_2) \otimes \cdots \otimes_\mathbf{C} \operatorname{Hom}_\mathbf{C}(E_n, F_n)
$$
$$
\to \operatorname{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n, F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n)
$$

tổng quát hóa ánh xạ được định nghĩa trong no. 5 cho $n = 2$.

Tính chất kết hợp tổng quát đã thấy trước đây có thể được chuyên biệt hóa ở đây như sau. Cho một phân hoạch $(J_k)_{1 \leq k \leq m}$ của khoảng $\{1, n\}$ của $\mathbf{N}$, và với mỗi $k$, cho $F_k$ là tích tenxơ $E_{i_1} \otimes_\mathbf{C} E_{i_2} \otimes \cdots \otimes_\mathbf{C} E_{i_r}$, trong đó $(i_1, \ldots, i_r)$ là dãy tăng ngặt các phần tử của $J_k$. Khi đó có một đẳng cấu C-môđun chính tắc (gọi là "đẳng cấu kết hợp")

$$
F_1 \otimes_C F_2 \otimes \cdots \otimes_C F_m \to E_1 \otimes_C E_2 \otimes \cdots \otimes_C E_n
$$

mà, theo ký hiệu ở trên, biến tích tenxơ

$$
y_1 \otimes y_2 \otimes \cdots \otimes y_m, \quad \text{trong đó } y_k = x_{i_1} \otimes x_{i_2} \otimes \cdots \otimes x_{i_r},
$$

thành tích tenxơ $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ (trong đó $x_i \in E_i$ với mọi $i$).

Đặc biệt, nếu $\pi$ là một phép hoán vị của $\{1, n\}$, viết $J_k = \{\pi(k)\}$ với $1 \leq k \leq n$, ta thu được một đẳng cấu chính tắc ("giao hoán")

$$
E_{\pi(1)} \otimes_C E_{\pi(2)} \otimes \cdots \otimes_C E_{\pi(n)} \to E_1 \otimes_C E_2 \otimes \cdots \otimes_C E_n
$$

biến $x_{\pi(1)} \otimes x_{\pi(2)} \otimes \cdots \otimes x_{\pi(n)}$ thành $x_1 \otimes x_2 \otimes \cdots \otimes x_n$. Ta sẽ thường đồng nhất các tích tenxơ khác nhau tương ứng với nhau qua các đẳng cấu chính tắc này.

Với $1 \leq i \leq n$, giả sử rằng $E_i$ thừa nhận một cơ sở $(b^{(i)}_{\lambda_i})_{\lambda_i \in L_i}$; bằng quy nạp theo $n$, suy ra từ no. 7, Hệ quả 2 của Mệnh đề 7 rằng họ $(b^{(1)}_{\lambda_1} \otimes b^{(2)}_{\lambda_2} \otimes \cdots \otimes b^{(n)}_{\lambda_n})$, trong đó $(\lambda_1, \ldots, \lambda_n)$ chạy qua $\prod_{1 \leq i \leq n} L_i$, là một cơ sở của $\bigoplus_{1 \leq i \leq n} E_i$, đôi khi được gọi là *tích tenxơ* của các cơ sở $(b^{(1)}_{\lambda_1})$ đang xét.

#### Nhận xét {#alg-ii-s3-n9-rem-1 .statement}

(1) Các nhận xét ở trên liên quan đến trường hợp các môđun trên một vành giao hoán được tổng quát hóa như trong no. 5, *Nhận xét* 2 khi có một tích tenxơ $E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$ trong đó các vành $A_i$ không nhất thiết giao hoán và trong đó, với mỗi $i$, có một đồng cấu $\rho_i : C \to A$ từ cùng một vành *giao hoán* $C$ sao cho: (1) $\rho_i(C)$ được chứa trong *tâm* của $A_i$; (2) với $2 \leq i \leq n - 1$, các cấu trúc $C$-môđun trên $E_i$ thu được bằng cách dùng các đồng cấu $\rho_{i-1}$ và $\rho_i$ là *trùng nhau*. Khi đó ta thu được một cấu trúc $C$-*môđun* trên $E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$ và các ánh xạ chính tắc tương tự như (13) (no. 5), mà ta để bạn đọc tự mô tả.

(2) Cho $A, B$ là hai vành, $E$ là một $A$-môđun phải, $E'$ là một $A$-môđun trái, $F$ là một $B$-môđun phải và $F'$ là một $B$-môđun trái. Khi đó các ánh xạ $\mathbf{Z}\text{-song tuyến tính}$ từ $(E \otimes_A E') \times (F \otimes_B F')$ vào một $\mathbf{Z}\text{-môđun}$ $G$ *tương ứng một-một* với các ánh xạ $\mathbf{Z}\text{-đa tuyến tính}$ $f$ từ $E \times E' \times F \times F'$ vào $G$ thỏa mãn các điều kiện

$$
\begin{cases}
f(x \lambda, x', y, y') = f(x, \lambda x', y, y') \\
f(x, x', y \mu, y') = f(x, x', y, \mu y')
\end{cases}
$$

với $\lambda \in A, \mu \in B, x \in E, x' \in E', y \in F, y' \in F'$. Các cấu tạo tổng quát đã cho trong no. này rút gọn chứng minh điều này về việc xác định một đẳng cấu chính tắc của $\mathbf{Z}\text{-môđun}$ giữa $(E \otimes_A E') \otimes_{\mathbf{Z}} (F \otimes_B F')$ và $E \otimes_A E' \otimes_{\mathbf{Z}} F \otimes_B F'$, điều này suy ra từ tính kết hợp của các tích tenxơ dạng (33).

### Bài tập {#alg-ii-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
