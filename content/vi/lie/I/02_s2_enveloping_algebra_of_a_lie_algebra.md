---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 2
section_title: Enveloping algebra of a Lie algebra
lang: vi
source: lie-i-iii
book_pages: 12-25, 83-85
pdf_pages: 0030-0043, 0101-0103
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE ENVELOPING ALGEBRA
      page: 12
      pdf_page: 30
    - "no": 2
      title: ENVELOPING ALGEBRA OF A PRODUCT OF LIE ALGEBRAS
      page: 13
      pdf_page: 31
    - "no": 3
      title: ENVELOPING ALGEBRA OF A LIE SUBALGEBRA
      page: 14
      pdf_page: 32
    - "no": 4
      title: ENVELOPING ALGEBRA OF THE OPPOSITE LIE ALGEBRA
      page: 15
      pdf_page: 33
    - "no": 5
      title: SYMMETRIC ALGEBRA OF A MODULE
      page: 16
      pdf_page: 34
    - "no": 6
      title: FILTRATION OF THE ENVELOPING ALGEBRA
      page: 17
      pdf_page: 35
    - "no": 7
      title: THE POINCARÉ–BIRKHOFF–WITT THEOREM
      page: 18
      pdf_page: 36
    - "no": 8
      title: EXTENSION OF DERIVATIONS
      page: 23
      pdf_page: 41
    - "no": 9
      title: EXTENSION OF THE BASE RING
      page: 25
      pdf_page: 43
statements: 22
exercises: 10
content_sha256: e9d1fd242912964f7949543e89447a8144dd5be846fb7c9faa70c09b8e7f6b24
translated_from: content/en/lie/I/02_s2_enveloping_algebra_of_a_lie_algebra.md
source_content_sha256: 70815c8f0c59caa459ae983d4d4afb3ca7aaff673e5632c3fd9b6438da4a9e5f
translation_model: gpt-5-6-mini, gpt-5.4, gpt-5-6, gpt-5-mini
translation_run: translate-vi-a4a762ec
glossary_version: 34
glossary_terms_sha256: 33acec4e7425ff9b17aa9ae8dafa5f452f1958ab5cb98b89a5d6bbde10d68d59
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ĐẠI SỐ BAO CỦA MỘT ĐẠI SỐ Lie

### 1. ĐỊNH NGHĨA ĐẠI SỐ BAO

Cho $g$ là một đại số Lie trên $K$. Đối với mọi đại số kết hợp có phần tử đơn vị $L$ trên $K$, một ánh xạ $\alpha$ của $g$ vào $L$ là một ánh xạ tuyến tính trên $K$ $\sigma$ của $g$ vào $L$ sao cho
$$
\sigma([x, y]) = \sigma(x)\sigma(y) - \sigma(y)\sigma(x) \quad (x, y \text{ trong } g)
$$
(nói cách khác là một đồng cấu của $g$ vào đại số Lie liên kết với $L$).

Nếu $L'$ là một đại số kết hợp khác có phần tử đơn vị trên $K$ và $\tau$ là một đồng cấu của $L$ vào $L'$ biến 1 thành 1, thì $\tau \circ \sigma$ là một ánh xạ $\alpha$ của $g$ vào $L'$. Ta sẽ tìm một đại số kết hợp có phần tử đơn vị và một ánh xạ $\alpha$ của $g$ vào đại số này có tính phổ quát (Lý thuyết tập hợp, Chương IV, § 3, no. 1).

#### Định nghĩa 1 {#lie-i-s2-def-1 .statement}

*Cho $g$ là một đại số Lie trên $K$, $T$ là đại số tenxơ của $K$-môđun $g$ và $J$ là iđêan hai phía của $T$ sinh bởi các tenxơ $x \otimes y - y \otimes x - [x, y]$ trong đó $x \in g, y \in g$. Đại số kết hợp $U = T/J$ được gọi là đại số bao của $g$. Hạn chế vào $g$ của ánh xạ chính tắc của $T$ lên $U$ được gọi là ánh xạ chính tắc của $g$ vào $U$.*

Cho $T_+$ là iđêan hai phía của $T$ gồm các tensor mà thành phần có cấp 0 là không. Cho $T_0 = K.1$ là tập hợp các phần tử của $T$ có cấp 0. Cho $U_+$ và $U_0$ là các ảnh chính tắc của $T_+$ và $T_0$ trong $U$. Vì $J \subset T_+$, phân tích thành tổng trực tiếp $T = T_0 + T_+$ kéo theo một phân tích thành tổng trực tiếp $U = U_0 + U_+$. Đại số $U$ do đó có một phần tử đơn vị phân biệt với 0 và $U_0 = K.1$. Với mọi $x \in U$, thành phần của $x$ trong $U_0$ được gọi là *số hạng hằng* của $x$. Các phần tử có số hạng hằng bằng không tạo thành một iđêan hai phía của $U$, cụ thể là iđêan hai phía $U^+$ sinh bởi ảnh chính tắc của $g$ trong $U$.

Đại số kết hợp $U$ được sinh bởi 1 và ảnh chính tắc của $g$ trong $U$.

Nếu $x \in g$ và $y \in g$, $x \otimes y - y \otimes x$ và $[x, y]$ là đồng dư trong $T$ theo môđun $J$; do đó, nếu $\sigma_0$ ký hiệu ánh xạ chính tắc của $g$ vào $U$,

$$
\sigma_0(x)\sigma_0(y) - \sigma_0(y)\sigma_0(x) = \sigma_0([x, y])
$$

trong $U$. Nói cách khác, $\sigma_0$ là một ánh xạ $\alpha$ của $g$ vào $U$.

#### Mệnh đề 1 {#lie-i-s2-prop-1 .statement}

*Cho $\sigma$ là một ánh xạ $\alpha$ của $g$ vào đại số kết hợp $L$ có phần tử đơn vị. Tồn tại một và chỉ một đồng cấu $\tau$ của $U$ vào $L$, biến 1 thành 1, sao cho $\sigma = \tau \circ \sigma_0$, trong đó $\sigma_0$ ký hiệu ánh xạ chính tắc của $g$ vào $U$.*

Cho $\tau'$ là đồng cấu duy nhất của $T$ vào $L$ mở rộng $\sigma$ và biến 1 thành 1. Khi đó, với $x, y$ trong $g$,

$$
\tau'(x \otimes y - y \otimes x - [x, y]) = \sigma(x)\sigma(y) - \sigma(y)\sigma(x) - \sigma([x, x]) = 0;
$$

do đó $\tau'$ bằng không trên $J$ và xác định, khi chuyển qua thương, một đồng cấu $\tau$ của $U$ vào $L$, ánh xạ 1 vào 1, sao cho $\sigma = \tau \circ \sigma_0$. Tính duy nhất của $\tau$ là ngay lập tức vì $\sigma_0(g)$ và 1 sinh đại số $U$.

Cho $g'$ là một đại số Lie khác trên $K$, $U'$ là đại số bao của nó và $\sigma'_0$ là ánh xạ chính tắc của $g'$ vào $U'$. Cho $\phi$ là một đồng cấu của $g$ vào $g'$. Khi đó $\sigma'_0 \circ \phi$ là một ánh xạ $\alpha$ của $g$ vào $U'$; do đó tồn tại một và chỉ một đồng cấu $\tilde{\phi}$ của $U$ vào $U'$ ánh xạ 1 vào 1 và sao cho biểu đồ

$$
\begin{array}{ccc}
g & \xrightarrow{\phi} & g' \\
\downarrow \sigma_0 & & \downarrow \sigma'_0 \\
U & \xleftarrow{\tilde{\phi}} & U'
\end{array}
$$

là giao hoán. Đồng cấu này ánh xạ các phần tử của $U$ có số hạng hằng bằng không vào các phần tử của $U'$ có số hạng hằng bằng không. Nếu $g''$ là một đại số Lie khác trên $K$ và $\phi'$ là một đồng cấu của $g'$ vào $g''$, thì $(\phi' \circ \phi)^{\sim} = \tilde{\phi}' \circ \tilde{\phi}$.

### 2. ĐẠI SỐ BAO CỦA MỘT TÍCH CỦA CÁC ĐẠI SỐ LIE

Cho $g_1, g_2$ là hai đại số Lie trên $K$, $U_i$ là đại số bao của $g_i$ và $\sigma_i$ là ánh xạ chính tắc của $g_i$ vào $U_i$ ($i = 1, 2$). Cho $g = g_1 \times g_2, U$ là đại số bao của nó và $\sigma$ là ánh xạ chính tắc của $g$ vào $U$. Các phép nhúng chính tắc của $g_1$ và $g_2$ vào $g$ xác định các đồng cấu chính tắc của $U_1$ và $U_2$ vào $U$, các ảnh của chúng giao hoán và do đó một đồng cấu $\phi$ của đại số $U_1 \otimes_K U_2$ vào đại số $U$, ánh xạ 1 vào 1.

#### Mệnh đề 2 {#lie-i-s2-prop-2 .statement}

*Đồng cấu $\phi$ là một đẳng cấu đại số*

Ánh xạ $\sigma': (x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)$ ($x_1 \in g_1, x_2 \in g_2$) là một ánh xạ $\alpha$ của $g$ vào $U_1 \otimes_K U_2$ và do đó tồn tại (no. 1, Mệnh đề 1) một đồng cấu duy nhất $\tau$ của $U$ vào $U_1 \otimes_K U_2$ biến 1 thành 1, sao cho:

$$(1)$$
$$
\sigma' = \tau \circ \sigma.
$$

Bây giờ $\phi \circ \tau \circ \sigma = \phi \circ \sigma' = \sigma$ và $\tau \circ \phi \circ \sigma' = \tau \circ \sigma = \sigma'$, do đó $\phi \circ \tau$ và $\tau \circ \phi$ lần lượt là các ánh xạ đồng nhất của $U$ và $U_1 \otimes_K U_2$. Do đó có mệnh đề.

$U_1 \otimes_K U_2$ được đồng nhất với $U$ qua đẳng cấu $\phi$. Khi đó ánh xạ chính tắc của $g$ vào $U$ được đồng nhất theo (1) với ánh xạ:
$$
(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2).
$$

Tương tự, nếu $g_1, \ldots, g_n$ là các đại số Lie trên $K$ với các đại số bao $U_1, \ldots, U_n$, thì đại số bao $U$ của $g_1 \times \cdots \times g_n$ được đồng nhất một cách chính tắc với $U_1 \otimes_K \cdots \otimes_K U_n$ và ánh xạ chính tắc của $g_1 \times \cdots \times g_n$ vào $U$ được đồng nhất với ánh xạ:
$$
(x_1, \ldots, x_n) \mapsto \sigma_1(x_1) \otimes 1 \otimes \cdots \otimes 1 + \cdots + 1 \otimes \cdots \otimes 1 \otimes \sigma_n(x_n)
$$
($\sigma_i$ ký hiệu ánh xạ chính tắc của $g_i$ vào $U_i$).

### 3. ĐẠI SỐ BAO CỦA MỘT ĐẠI SỐ CON LIE

Cho $g$ là một đại số Lie trên $K$, $h$ là một đại số con của $g$ và $\sigma, \sigma'$ là các ánh xạ chính tắc của $g, h$ vào các đại số bao của chúng $U, V$. Khi đó đơn ánh chính tắc $i$ của $h$ vào $g$ xác định một đồng cấu $\tilde{i}$, được gọi là *chính tắc*, của $V$ vào $U$ sao cho $\sigma \circ i = \tilde{i} \circ \sigma'$. Đại số $\tilde{i}(V)$ được sinh bởi 1 và $\sigma(h)$. Ta sẽ thấy (no. 7, Hệ quả của Định lý 5) rằng $\tilde{i}$ là đơn ánh trong những trường hợp quan trọng.

Nếu $h$ là một iđêan của $g$, iđêan trái của $U$ sinh bởi $\sigma(h)$ trùng với iđêan phải sinh bởi $\sigma(h)$, nói cách khác nó là một iđêan hai phía $R$. Điều này suy ra vì, với $x \in h$ và $x' \in g$,
$$
\sigma(x)\sigma(x') = \sigma(x')\sigma(x) + \sigma([x, x'])
$$
và $[x, x'] \in h$.

#### Mệnh đề 3 {#lie-i-s2-prop-3 .statement}

*Cho $h$ là một iđêan của $g$, $p$ là đồng cấu chính tắc của $g$ lên $g/h$ và $W$ là đại số bao của $g/h$. Đồng cấu:*
$$
\tilde{p}: U \to W
$$
*được xác định một cách chính tắc bởi $p$ là toàn ánh và hạt nhân của nó là iđêan $R$ của $U$ sinh bởi $\sigma(h)$.*

Cho $\sigma''$ là ánh xạ chính tắc của $g/\mathfrak{h}$ vào W. Biểu đồ giao hoán:

$$
\begin{array}{ccc}
\mathfrak{h} & \xrightarrow{i} & g \\
\downarrow \sigma' & & \downarrow \sigma \\
V & \xrightarrow{\iota} & U
\end{array}
$$
$$
\begin{array}{ccc}
g & \xrightarrow{p} & g/\mathfrak{h} \\
\downarrow \sigma & & \downarrow \sigma'' \\
U & \xrightarrow{\tilde{p}} & W
\end{array}
$$

chứng minh rằng $\tilde{p}$ bằng không trên $\sigma(\mathfrak{h})$ và do đó trên R. Gọi $\psi$ là đồng cấu chính tắc của U lên U/R. Có một đồng cấu $\phi$ của U/R

$$
\begin{array}{ccc}
g & \xrightarrow{p} & g/\mathfrak{h} \\
\downarrow \sigma & & \downarrow \sigma'' \\
U & \xrightarrow{\psi} & U/R
\end{array}
$$
$$
\begin{array}{ccc}
U/R & \xleftarrow{\phi'} & W \\
& \uparrow \theta & \\
& \uparrow \phi & \\
U/R & \xrightarrow{\phi} & W
\end{array}
$$

vào W sao cho $\tilde{p} = \phi \circ \psi$. Ánh xạ $\psi \circ \sigma$ của g vào U/R là một ánh xạ $\alpha$ và bằng không trên $\mathfrak{h}$, do đó xác định một ánh xạ $\alpha$ $\theta$ của $g/\mathfrak{h}$ vào U/R sao cho $\theta \circ p = \psi \circ \sigma$. Khi đó $\phi \circ \theta \circ p = \phi \circ \psi \circ \sigma = \sigma'' \circ p$. Suy ra $\phi \circ \theta = \sigma''$. Có một và chỉ một đồng cấu $\phi'$ của W vào U/R (no. 1, Mệnh đề 1) biến 1 thành 1 và sao cho $\theta = \phi' \circ \sigma''$. Khi đó $\phi' \circ \phi \circ \theta = \phi' \circ \sigma'' = \theta$ và $\phi \circ \phi' \circ \sigma'' = \phi \circ \theta = \sigma''$, và do đó $\phi' \circ \phi$ và $\phi \circ \phi'$ lần lượt là các ánh xạ đồng nhất của U/R và W. Điều này hoàn tất chứng minh.

U/R được đồng nhất với W dưới đẳng cấu $\phi$. Khi đó ánh xạ chính tắc $\sigma''$ của $g/\mathfrak{h}$ vào W được đồng nhất với $\theta$, tức là với ánh xạ của $g/\mathfrak{h}$ vào U/R dẫn xuất từ $\sigma$ bằng cách lấy thương.

### 4. ĐẠI SỐ BAO CỦA ĐẠI SỐ LIE ĐỐI

Cho $g$ là một đại số Lie trên K, $g^0$ là đại số Lie đối và $\sigma$ và $\sigma_0$ là các ánh xạ chính tắc của $g$ và $g^0$ vào các đại số bao quanh của chúng U và V. Khi đó $\sigma$ là một ánh xạ $\alpha$ của $g^0$ vào đại số kết hợp $U^0$ đối với đại số kết hợp U. Do đó tồn tại duy nhất một đồng cấu $\phi$ từ V vào $U^0$ biến 1 thành 1 và sao cho $\sigma = \phi \circ \sigma_0$.

#### Mệnh đề 4 {#lie-i-s2-prop-4 .statement}

*Đồng cấu $\phi$ là một đẳng cấu từ V lên $U^0$.*

Tồn tại một đồng cấu $\phi'$ từ U vào $V^0$ biến 1 thành 1 và sao cho $\sigma_0 = \phi' \circ \sigma$. Có thể xem $\phi'$ như một đồng cấu từ $U^0$ vào V. Khi đó $\sigma_0 = \phi' \circ \phi \circ \sigma_0$ và $\sigma = \phi \circ \phi' \circ \sigma$ và do đó $\phi' \circ \phi$ và $\phi \circ \phi'$ là các ánh xạ đồng nhất của V và U. Do đó có mệnh đề.

V được đồng nhất với $U^0$ theo đẳng cấu $\phi$. Khi đó $\sigma_0$ được đồng nhất với $\sigma$.

Với sự đồng nhất này, đẳng cấu $\theta : x \mapsto -x$ của $g$ lên $g^0$ xác định một đẳng cấu $\tilde{\theta}$ của U lên $V = U^0$. Đẳng cấu này có thể được xem như một phản tự đẳng cấu của U. Nó được gọi là phản tự đẳng cấu chính của U. Nếu $x_1, \ldots, x_n$ thuộc $g$, thì:

$$
(2) \quad \tilde{\theta}(\sigma(x_1) \ldots \sigma(x_n)) = \tilde{\theta}(\sigma(x_n)) \ldots \tilde{\theta}(\sigma(x_1)) = (-\sigma(x_n)) \ldots (-\sigma(x_1))
$$
$$
= (-1)^n \sigma(x_n) \ldots \sigma(x_1).
$$

### 5. ĐẠI SỐ ĐỐI XỨNG CỦA MỘT MÔĐUN

Cho V là một K-môđun. V có thể được xem theo một cách duy nhất như một đại số Lie giao hoán. Đại số bao quanh của V khi đó có thể thu được như sau: cho T là đại số tenxơ của V; cho I là iđêan hai phía của T sinh bởi các tenxơ $x \otimes y - y \otimes x$ ($x \in V, y \in V$); khi đó lập đại số $S = T/I$.

Nhắc lại (*Algebra*, Chương III, § 6) rằng S được gọi là đại số đối xứng của V, ta tóm tắt ngắn gọn các tính chất cần dùng trong chương này, mà các chứng minh của chúng là ngay lập tức. Cho $T^n$ là tập hợp các tenxơ thuần nhất cấp n trong T. Khi đó $I = (I \cap T^2) + (I \cap T^3) + \cdots$ và do đó S là tổng trực tiếp của các ảnh chính tắc $S^n$ của các $T^n$. Các phần tử của $S^n$ được gọi là thuần nhất bậc n. $S^0 = K.1, S^1$ được đồng nhất với V và $S^n S^p \subset S^{n+p}$. Đại số S được sinh bởi 1 và $S^1 = V$. Rõ ràng hai phần tử bất kỳ của $S^1$ đều hoán vị được và do đó S là giao hoán. Nếu V là một K-môđun tự do với cơ sở $(x_\lambda)_{\lambda \in \Lambda}$, đồng cấu chính tắc f của đại số đa thức $K[X_\lambda]_{\lambda \in \Lambda}$ lên S biến 1 thành 1 và $X_\lambda$ thành $x_\lambda$ với mọi $\lambda \in \Lambda$ là một đẳng cấu: vì theo tính chất phổ quát của S (no. 1, Mệnh đề 1) tồn tại một đồng cấu g của S vào $K[X_\lambda]_{\lambda \in \Lambda}$ biến 1 thành 1 và $x_\lambda$ thành $X_\lambda$ với mọi $\lambda \in \Lambda$ và f và g là các đồng cấu nghịch đảo của nhau.

Cho ${S'}^n \subset T^n$ là tập hợp các tenxơ đối xứng thuần nhất cấp n (*Algebra*, Chương III, § 5, no. 1, Định nghĩa 2). Nếu K là một trường có đặc số 0, thì ${S'}^n$ và $I \cap T^n$ bù nhau trong $T^n$. Thật vậy, lấy $(x_\lambda)_{\lambda \in \Lambda}$ là một cơ sở của V. Ta trang bị cho $\Lambda$ một thứ tự toàn phần (*Set Theory*, Chương III, § 2, no. 3, Định lý 1). Gọi $\Lambda_n$ là tập hợp các dãy tăng gồm n phần tử của $\Lambda$. Với $M = (\lambda_1, \ldots, \lambda_n) \in \Lambda_n$, đặt

$$
y_M = \frac{1}{n!} \sum_{\sigma \in S_n} x_{\lambda_{\sigma(n)}} \otimes \cdots \otimes x_{\lambda_{\sigma(n)}}.
$$

Các $y_M$ với $M \in \Lambda_n$ lập thành một hệ sinh của K-không gian vectơ ${S'}^n$. Mặt khác, các ảnh chính tắc của chúng trong $S^n$ cấu thành, theo đoạn trên, một cơ sở của $S^n$. Do đó $(y_M)_{M \in \Lambda_n}$ là một cơ sở của một không gian con bù của $I \cap T^n$ trong $T^n$ (*Algebra*, Chương II, § 1, no. 6, Mệnh đề 4), điều này chứng minh mệnh đề của ta.

Vì thế, khi K là một trường có đặc số 0, hạn chế lên ${S'}^n$ của ánh xạ chính tắc $T^n \to S^n$ là một đẳng cấu từ không gian ${S'}^n$ lên không gian $S^n$ và do đó có một đẳng cấu nghịch đảo. Các đẳng cấu nghịch đảo thu được như vậy với mỗi n xác định một đẳng cấu chính tắc từ không gian S lên không gian

$$
S' = \sum_{n \geq 0} {S'}^n \text{ các tenxơ đối xứng}.
$$

### 6. PHÂN BẬC CỦA ĐẠI SỐ BAO

Cho $g$ là một đại số Lie trên $K$ và $T$ là đại số tenxơ của K-môđun $g$. Gọi $T^n$ là môđun con của $T$ gồm các tenxơ thuần nhất cấp $n$ và $T_n = \sum_{i \leq n} T^i$. Khi đó $T_n \subset T_{n+1}$, $T_0 = K.1$, $T_{-1} = \{0\}$ và $T_n T_p \subset T_{n+p}$.

Gọi $U_n$ là ảnh chính tắc của $T_n$ trong đại số bao $U$ của $g$. Khi đó $U_n \subset U_{n+1}$, $U_0 = K.1$, $U_{-1} = \{0\}$ và $U_n U_p \subset U_{n+p}$; vì thế $U$ có thể được mô tả như một đại số *được lọc bởi* các $U_n$ (*Commutative Algebra*, Chương III, § 2, no. 1); các phần tử của $U_n$ sẽ được gọi là *có bậc lọc* $\leq n$.

Cho $G^n$ là $K$-môđun $U_n / U_{n-1}$ và cho $G$ là $K$-môđun là tổng trực tiếp của các $G^n$. Phép nhân trên $U$ xác định, khi lấy các thương, một ánh xạ song tuyến tính từ $G^n \times G^m$ vào $G^{n+m}$ và do đó một ánh xạ song tuyến tính từ $G \times G$ vào $G$, ánh xạ này kết hợp. Vì vậy $G$ được trang bị một cấu trúc đại số $K$ kết hợp. Khi đó $G^n G^m \subset G^{n+m}$. Các phần tử của $G^n$ được gọi là có *bậc* $n$. Đại số phân bậc thu được như vậy chính là đại số phân bậc liên kết với đại số lọc $U$ (*Đại số giao hoán*, Chương III, § 2, no. 3).

Cho $\phi_n$ là hợp thành của các ánh xạ tuyến tính $K$ chính tắc

$$
T^n \to U_n \to G^n.
$$

Vì $T^n$ là bổ sung cho $T_{n-1}$ trong $T_n$, $\phi_n$ là toàn ánh. Các $\phi_n$ xác định một ánh xạ tuyến tính $K$ $\phi$ từ $\sum_n T^n = T$ lên $\sum_n G^n = G$.

#### Mệnh đề 5 {#lie-i-s2-prop-5 .statement}

*Ánh xạ $\phi$ từ $T$ lên $G$ là một đồng cấu đại số biến 1 thành 1 và bằng không trên iđêan hai phía sinh bởi các tenxơ $x \otimes y - y \otimes x$ ($x \in g, y \in g$).*

Nếu $t \in T^n$ và $t' \in T^p$, thì $\phi(t)\phi(t') = \phi(tt')$ theo định nghĩa của phép nhân trên $G$. Do đó $\phi$ là một đồng cấu đại số và rõ ràng $\phi(1) = 1$. Nếu $x, y$ thuộc $g$, thì $x \otimes y - y \otimes x \in T^2$ và ảnh chính tắc của phần tử này trong $U_2$ bằng ảnh của $[x, y]$ và do đó thuộc $U_1$. Vì vậy $\phi(x \otimes y - y \otimes x) = 0$, điều này chứng minh mệnh đề.

Cho $S$ là đại số đối xứng của $K$-môđun $g$ và $\tau$ là đồng cấu chính tắc từ $T$ lên $S$. Mệnh đề 5 chứng minh rằng tồn tại một đồng cấu duy nhất $\omega$, được gọi là *chính tắc*, từ đại số $S$ lên đại số $G$, biến 1 thành 1, sao cho $\phi = \omega \circ \tau$. Ta có $\omega(S^n) = \phi(T^n) = G^n$. Gọi $\tau_n$ là hạn chế của $\tau$ lên $T^n$, $\omega_n$ là hạn chế của $\omega$ lên $S^n$, $\psi_n$ là ánh xạ chính tắc từ $T^n$ vào $U_n$ và $\theta_n$ là ánh xạ chính tắc từ $U_n$ lên $G^n$. Định nghĩa của $\omega_n$ chứng minh rằng biểu đồ sau đây là giao hoán:

$$
\begin{array}{ccccc}
T^n & \xrightarrow{\psi_n} & U_n & \xrightarrow{\theta_n} & G^n \\
& \searrow & & \swarrow & \\
& & S^n & \xrightarrow{\omega_n} &
\end{array}
$$

#### Mệnh đề 6 {#lie-i-s2-prop-6 .statement}

*Nếu K là Noether và g là một môđun hữu hạn sinh, thì vành U là Noether phải và trái.*

S là một đại số sinh hữu hạn trên K và do đó là một vành Noether (*Đại số giao hoán*, Chương III, § 2, no. 10, Hệ quả 3 của Định lý 2). Vì thế G, đẳng cấu với một vành thương của S, là Noether. Vì thế U là Noether phải và trái (*Đại số giao hoán*, Chương III, § 2, no. 10, *Nhận xét 2*).

#### Hệ quả {#lie-i-s2-n6-cor-1 .statement}

*Giả sử rằng K là một trường và g là hữu hạn chiều trên K. Gọi I₁, ..., Iₘ là các iđêan phải (tương ứng là trái) có đối chiều hữu hạn trong U. Khi đó iđêan tích I₁I₂...Iₘ có đối chiều hữu hạn.*

Bằng quy nạp theo m, chỉ cần xét trường hợp, chẳng hạn, của hai iđêan phải. U-môđun phải I₁ được sinh bởi một số hữu hạn phần tử u₁, ..., uₚ (Mệnh đề 6). Gọi v₁, ..., vₐ là các phần tử của U sao cho các lớp của chúng theo môđun I₂ sinh không gian vectơ U/I₂. Khi đó các ảnh chính tắc trong I₁/I₁I₂ của các uᵢvⱼ sinh không gian vectơ I₁/I₁I₂, do đó không gian này là hữu hạn chiều. Vì thế dim_K(U/I₁I₂) = dim_K(U/I₁) + dim_K(I₁/I₁I₂) < +∞.

#### Nhận xét {#lie-i-s2-n6-rem-1 .statement}

Cho g' là một đại số Lie khác trên vành K, U' là đại số bao của nó, U'_n là tập các phần tử của U' có cấp lọc $\leq n$ và U^n (tương ứng là U'^n) là tập các ảnh chính tắc trong U (tương ứng là U') của các tenxơ đối xứng thuần nhất của g (tương ứng là g') bậc n. Gọi $\eta$ là một đồng cấu từ g vào g' và $\tilde{\eta}$ là đồng cấu tương ứng từ U vào U'. Khi đó

$$
\tilde{\eta}(U_n) \subset U'_n, \quad \tilde{\eta}(U^n) \subset {U'}^n.
$$

Đặc biệt, phản tự đẳng cấu chính của U để ổn định U_n và U^n. Ánh xạ K-tuyến tính từ $T^n$ lên chính nó biến

$$
x_1 \otimes x_2 \otimes \cdots \otimes x_n \quad \text{thành} \quad x_n \otimes x_{n-1} \otimes \cdots \otimes x_1
$$

với mọi $x_1, ..., x_n$ trong g là một toán tử đối xứng và do đó để bất động các tenxơ đối xứng thuần nhất bậc n. Vì thế phản tự đẳng cấu chính của U cảm sinh trên mỗi U^n phép vị tự với tỉ số $(-1)^n$.

### 7. ĐỊNH LÝ POINCARÉ–BIRKHOFF–WITT

#### Định lý 1 {#lie-i-s2-thm-1 .statement}

*Cho g là một đại số Lie trên K, U là đại số bao của nó, G là đại số phân bậc liên kết với đại số lọc U và S là đại số đối xứng của $K$-môđun g. Nếu g là một K-môđun tự do, thì đồng cấu chính tắc $\omega : S \to G$ là một đẳng cấu.*

Gọi $(x_\lambda)_{\lambda \in \Lambda}$ là một cơ sở của $K$-môđun g; ta trang bị cho $\Lambda$ một thứ tự toàn phần (*Lý thuyết tập hợp*, Chương III, § 2, no. 3, Định lý 1). Gọi P là đại số đa thức $K[z_\lambda]_{\lambda \in \Lambda}$ theo các ẩn $z_\lambda$ tương ứng một-một với các $x_\lambda$. Với mọi dãy $M = (\lambda_1, \lambda_2, ..., \lambda_n)$ gồm các phần tử của $\Lambda$, gọi $z_M$ là đơn thức $z_{\lambda_1}z_{\lambda_2}...z_{\lambda_n}$ và $x_M$ là tenxơ $x_{\lambda_1} \otimes x_{\lambda_2} \otimes \cdots \otimes x_{\lambda_n}$.

Các $z_M$, với M tăng, tạo thành một cơ sở của K-môđun P (ta quy ước rằng $\varnothing$ là một dãy tăng và $z_\varnothing = 1$). Gọi $P_p$ là môđun con các đa thức bậc $\leq p$. Trước hết ta sẽ chứng minh một số bổ đề. (Để viết gọn, ta viết $\lambda \leq M$ nếu $\lambda \leq \mu$ với mọi chỉ số $\mu$ của dãy M.)

#### Bổ đề 1 {#lie-i-s2-lem-1 .statement}

*Với mọi số nguyên $p \geq 0$, tồn tại một đồng cấu duy nhất $f_p$ từ K-môđun $g \otimes_K P_p$ vào K-môđun P thỏa mãn các điều kiện sau:*
$$
\begin{align*}
(A_p) \quad & f_p(x_\lambda \otimes z_M) = z_\lambda z_M \quad \text{với } \lambda \leq M, z_M \in P_p; \\
(B_p) \quad & f_p(x_\lambda \otimes z_M) - z_\lambda z_M \in P_q \quad \text{với } z_M \in P_q, q \leq p; \\
(C_p) \quad & f_p(x_\lambda \otimes f_p(x_\mu \otimes z_N)) = f_p(x_\mu \otimes f_p(x_\lambda \otimes z_N)) + f_p([x_\lambda, x_\mu] \otimes z_N)
\end{align*}
$$
*với $z_N \in P_{p-1}$. (Các hạng xuất hiện trong (C_p) là có nghĩa theo (B_p).)*

Hơn nữa, hạn chế của $f_p$ lên $g \otimes P_{p-1}$ trùng với $f_{p-1}$.

Khẳng định cuối cùng suy ra từ các khẳng định khác vì hạn chế của $f_p$ trên $g \otimes_K P_{p-1}$ thỏa mãn các điều kiện (A_{p-1}), (B_{p-1}) và (C_{p-1}). Ta sẽ chứng minh sự tồn tại và tính duy nhất của $f_p$ bằng quy nạp theo $p$. Với $p = 0$, điều kiện (A_0) cho $f_0(x_\lambda \otimes 1) = z_\lambda$ và các điều kiện (B_0) và (C_0) khi đó hiển nhiên được thỏa mãn. Giả sử bây giờ rằng sự tồn tại và tính duy nhất của $f_{p-1}$ đã được chứng minh. Ta chứng minh rằng $f_{p-1}$ có một mở rộng duy nhất $f_p$ lên $g \otimes_K P_p$ thỏa mãn các điều kiện (A_p), (B_p) và (C_p).

Ta phải định nghĩa $f_p(x_\lambda \otimes z_M)$ đối với một dãy tăng M gồm $p$ phần tử.

Nếu $\lambda \leq M$, giá trị này được cho bởi điều kiện (A_p). Ngược lại, M có thể được viết duy nhất dưới dạng ($\mu, N$), trong đó $\mu < \lambda, \mu \leq N$. Khi đó
$$
z_M = z_\mu z_N = f_{p-1}(x_\mu \otimes z_N)
$$
theo (A_{p-1}), do đó vế trái của (C_p) là $f_p(x_\lambda \otimes z_M)$. Bây giờ vế phải của (C_p) đã được định nghĩa: vì (B_{p-1}) cho phép ta viết:
$$
f_p(x_\lambda \otimes z_N) = f_{p-1}(x_\lambda \otimes z_N) = z_\lambda z_N + w
$$
trong đó $w \in P_{p-1}$; do đó vế phải của (C_p) trở thành:
$$
z_\lambda z_\mu z_N + f_{p-1}(x_\mu \otimes w) + f_{p-1}([x_\lambda, x_\mu] \otimes z_N).
$$

Như vậy $f_p$ được xác định duy nhất và hiển nhiên thỏa mãn các điều kiện (A_p) và (B_p). Điều kiện (C_p) được thỏa mãn nếu $\mu < \lambda, \mu \leq N$. Vì $[x_\mu, x_\lambda] = -[x_\lambda, x_\mu]$, điều kiện (C_p) cũng được thỏa mãn đối với $\lambda < \mu, \lambda \leq N$. Vì (C_p) được thỏa mãn hiển nhiên đối với $\lambda = \mu$, nên (C_p) do đó được thỏa mãn nếu $\lambda \leq N$ hoặc $\mu \leq N$. Nếu không có bất kỳ bất đẳng thức nào trong các bất đẳng thức này đúng, $N = (\nu, Q)$, trong đó $\nu \leq Q, \nu < \lambda, \nu < \mu$. Từ nay viết tắt $f_p(x \otimes z) = xz$ với $x \in g$ và $z \in P_p$, ta có theo giả thiết quy nạp:
$$
x_\mu z_N = x_\mu(x_\nu z_Q) = x_\nu(x_\mu z_Q) + [x_\mu, x_\nu]z_Q.
$$

Bây giờ $z_\mu z_Q$ có dạng $z_\mu z_Q + w$, trong đó $w \in P_{p-2}$. (C_p) có thể được áp dụng cho $x_\lambda(x_\nu(z_\mu z_Q))$, vì $\nu \leq Q$ và $\nu < \mu$, và cho $x_\lambda(x_\nu w)$ theo giả thiết quy nạp, và do đó cho $x_\lambda(x_\nu(x_\mu z_Q))$. Suy ra:
$$
x_\lambda(x_\mu z_N) = x_\nu(x_\lambda(x_\mu z_Q)) + [x_\lambda, x_\nu](x_\mu z_Q) + [x_\mu, x_\nu](x_\lambda z_Q)
+ [x_\lambda, [x_\mu, x_\nu]]z_Q.
$$

Đổi chỗ $\lambda$ và $\mu$ rồi lấy hiệu:

$$
x_{\lambda}(x_{\mu}z_{N}) - x_{\mu}(x_{\lambda}z_{N}) = x_{v}(x_{\lambda}(x_{\mu}z_{Q}) - x_{\mu}(x_{\lambda}z_{Q}))
+ [x_{\lambda}, [x_{\mu}, x_{v}]]z_{Q} - [x_{\mu}, [x_{\lambda}, x_{v}]]z_{Q}
= x_{v}([x_{\lambda}, x_{\mu}]z_{Q}) + [x_{\lambda}, [x_{\mu}, x_{v}]]z_{Q} + [x_{\mu}, [x_{v}, x_{\lambda}]]z_{Q}
= [x_{\lambda}, x_{\mu}](x_{v}z_{Q}) + ([x_{v}, [x_{\lambda}, x_{\mu}]]
+ [x_{\lambda}, [x_{\mu}, x_{v}]] + [x_{\mu}, [x_{v}, x_{\lambda}]])z_{Q}
$$

và do đó theo đồng nhất thức Jacobi

$$
x_{\lambda}(x_{\mu}z_{N}) - x_{\mu}(x_{\lambda}z_{N}) = [x_{\lambda}, x_{\mu}]z_{N}
$$

điều này hoàn thành chứng minh của Bổ đề 1.

#### Bổ đề 2 {#lie-i-s2-lem-2 .statement}

*Có một ánh xạ $\alpha$ $\sigma$ của $g$ vào $\mathcal{L}_{K}(P)$ sao cho:*

(1) $\sigma(x_{\lambda})z_{M} = z_{\lambda}z_{M}$ đối với $\lambda \leq M$;
(2) $\sigma(x_{\lambda})z_{M} \equiv z_{\lambda}z_{M}$ (mod. $P_{p}$) nếu $M$ có $p$ phần tử.

Theo Bổ đề 1 tồn tại một đồng cấu $f$ của K-môđun $g \otimes_{K} P_{p}$ vào $P$ thỏa mãn, với mọi $p$, các điều kiện (A$_{p}$), (B$_{p}$), (C$_{p}$) (trong đó $f_{p}$ được thay bởi $f$). Đồng cấu này xác định một đồng cấu $\sigma$ của K-môđun $g$ vào K-môđun $\mathcal{L}_{K}(P)$ và $\sigma$ là một ánh xạ $\alpha$ do điều kiện (C$_{p}$). Cuối cùng, $\sigma$ thỏa mãn các tính chất (1) và (2) của bổ đề do các điều kiện (A$_{p}$) và (B$_{p}$).

#### Bổ đề 3 {#lie-i-s2-lem-3 .statement}

*Cho $t$ là một tenxơ trong $T_{n} \cap J$. Thành phần thuần nhất $t_{n}$ của $t$ có cấp $n$ nằm trong hạt nhân $I$ của đồng cấu chính tắc $T \to S$.*

Ta viết $t_{n}$ dưới dạng $\sum_{i=1}^{r} x_{M_{i}}$, trong đó các $M_{i}$ là các dãy gồm $n$ phần tử của $\Lambda$. Ánh xạ $\sigma$ mở rộng thành một đồng cấu của đại số $T$ vào đại số $\mathcal{L}_{K}(P)$ (mà ta cũng sẽ ký hiệu là $\sigma$), bằng không trên $J$. Theo Bổ đề 2, $\sigma(t) . 1$ là một đa thức mà các số hạng có bậc cao nhất là $\sum_{i=1}^{r} z_{M_{i}}$. Vì $t \in J$, nên $\sigma(t) = 0$ và do đó $\sum_{i=1}^{r} z_{M_{i}} = 0$ trong $P$. Bây giờ $P$ được đồng nhất một cách chính tắc với $S$, vì $g$ có cơ sở $(x_{\lambda})$. Vì thế ảnh chính tắc của $t_{n}$ trong $S$ là không, tức là $t_{n} \in I$.

Bây giờ ta có thể chứng minh Định lý 1. Cần chứng minh rằng đồng cấu chính tắc của $S$ lên $G$ là đơn ánh. Nói cách khác, nếu $t \in T^{n}$ và $\psi$ ký hiệu đồng cấu chính tắc của $T$ lên $U$, thì cần chỉ ra rằng điều kiện $\psi(t) \in U_{n-1}$ kéo theo $t \in I$. Mà $\psi(t) \in U_{n-1}$ có nghĩa là tồn tại một tenxơ $t' \in T_{n-1}$ sao cho $t - t' \in J$. Tenxơ $t - t'$ nhận $t$ làm thành phần thuần nhất cấp $n$ và do đó $t \in I$ theo Bổ đề 3.

#### Hệ quả 1 {#lie-i-s2-lem-3-cor-1 .statement}

*Giả sử rằng $g$ là một $K$-môđun tự do. Cho $W$ là một K-môđun con của $T^{n}$.*

*Nếu, theo ký hiệu của biểu đồ* (3), *hạn chế của* $\tau_n$ *trên* $W$ *là một đẳng cấu từ* $W$ *lên* $S^n$, *thì hạn chế của* $\psi_n$ *trên* $W$ *là một đẳng cấu từ* $W$ *lên một phần bù của* $U_{n-1}$ *trong* $U_n$.

Hạn chế trên $W$ của $\omega_n \circ \tau_n$ là một song ánh từ $W$ lên $G^n$; hạn chế $\theta_n \circ \psi_n$ trên $W$ cũng vậy. Do đó suy ra hệ quả.

#### Hệ quả 2 {#lie-i-s2-lem-3-cor-2 .statement}

*Nếu $g$ là một K-môđun tự do, thì ánh xạ chính tắc từ $g$ vào đại số bao của nó là đơn ánh.*

Điều này suy ra từ Hệ quả 1 khi lấy $W = T^1$.

Khi $g$ là một K-môđun tự do (đặc biệt khi K là một trường), $g$ được đồng nhất với một môđun con của $U$ qua ánh xạ chính tắc từ $g$ vào $U$. Quy ước này được chấp nhận kể từ hệ quả sau đây.

#### Hệ quả 3 {#lie-i-s2-lem-3-cor-3 .statement}

*Nếu $g$ có một cơ sở được sắp thứ tự toàn phần $(x_\lambda)_{\lambda \in \Lambda}$, thì các phần tử $x_{\lambda_1} x_{\lambda_2} \ldots x_{\lambda_n}$ của đại số bao $U$, trong đó $(\lambda_1, \ldots, \lambda_n)$ là một dãy hữu hạn tăng tùy ý gồm các phần tử của $\Lambda$, tạo thành một cơ sở của K-môđun $U$.*

Cho $\Lambda_n$ là tập hợp các dãy tăng gồm $n$ phần tử của $\Lambda$. Với $M = (\lambda_1, \ldots, \lambda_n) \in \Lambda_n$, đặt $y_M = x_{\lambda_1} \otimes x_{\lambda_2} \otimes \cdots \otimes x_{\lambda_n}$. Cho $W$ là môđun con của $T^n$ có cơ sở là $(y_M)_{M \in \Lambda_n}$. Hệ quả 1 cho thấy rằng hạn chế của $\psi_n$ lên $W$ là một đẳng cấu từ $W$ lên một phần bù của $U_{n-1}$ trong $U_n$. Nhưng

$$
\psi_n(y_M) = x_{\lambda_1} x_{\lambda_2} \ldots x_{\lambda_n},
$$

do đó có hệ quả.

#### Hệ quả 4 {#lie-i-s2-lem-3-cor-4 .statement}

*Cho ${S'}^n \subset T^n$ là tập hợp các tensor đối xứng thuần nhất cấp n. Giả sử rằng K là một trường có đặc số 0. Khi đó ánh xạ hợp thành của các ánh xạ chính tắc*

$$
S^n \to {S'}^n \to U_n
$$

*là một đẳng cấu từ không gian vectơ $S^n$ lên một phần bù của $U_{n-1}$ trong $U_n$.*

Điều này suy ra từ Hệ quả 1 khi lấy $W = {S'}^n$.

Từ nay giả sử rằng K là một trường có đặc số 0. Cho $\eta_n$ là ánh xạ từ $S^n$ vào $U_n$ vừa được định nghĩa. Đặt $U^n = \eta_n(S^n)$. Không gian vectơ $U$ là tổng trực tiếp của các $U^n$. Các $\eta_n$ xác định một đẳng cấu $\eta$ từ không gian vectơ $S = \sum_n S^n$ lên không gian vectơ $U = \sum_n U^n$, gọi là *đẳng cấu chính tắc từ S lên U*; đây *không* phải là một đẳng cấu đại số. Ta có biểu đồ giao hoán:

$$
\begin{array}{ccccc}
& & U^n & & \\
& \nearrow \psi_n & \uparrow \eta_n & \searrow \theta_n & \\
{S'}^n & & & & G^n \\
& \searrow \tau_n & & \nearrow \omega_n & \\
& & S^n & &
\end{array}
$$

trong đó mỗi mũi tên biểu diễn một đẳng cấu không gian vectơ. Nếu $x_1, x_2, \ldots, x_n$ thuộc $g$, thì $\eta_n$ biến tích $x_1 x_2 \ldots x_n$, tính trong $S$, thành phần tử

$$
\frac{1}{n!} \sum_{\sigma \in S_n} x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)}
$$

tính trong $U$.

#### Hệ quả 5 {#lie-i-s2-lem-3-cor-5 .statement}

*Cho $h$ là một đại số con của đại số Lie $g$ và $U'$ là đại số bao của nó. Giả sử rằng các K-môđun $h$ và $g/h$ là tự do (chẳng hạn nếu $K$ là một trường). Cho $(x_\alpha)_{\alpha \in L}$ là một cơ sở của $h$ và $(y_\beta)_{\beta \in M}$ là một họ phần tử của $g$ mà các ảnh chính tắc của chúng trong $g/h$ lập thành một cơ sở của $g/h$.

(a) *Đồng cấu chính tắc từ $U'$ vào $U$ là đơn ánh.*

(b) *Nếu $M$ được sắp thứ tự toàn phần, thì các phần tử $y_{\beta_1} \ldots y_{\beta_q}$, với $\beta_1 \leq \cdots \leq \beta_q$, lập thành một cơ sở của $U$ khi xem nó như một môđun trái hoặc phải trên $U'$.*

Ta cho $L \cup M$ một thứ tự toàn phần sao cho mọi phần tử của $L$ đều nhỏ hơn mọi phần tử của $M$. Các phần tử $x_{\alpha_1} x_{\alpha_2} \ldots x_{\alpha_p}$ được tính trong $U'$ (trong đó $\alpha_1 \leq \cdots \leq \alpha_p$) tạo thành một cơ sở của $U'$ (Hệ quả 3). Các phần tử

$$
x_{\alpha_1} \ldots x_{\alpha_p} y_{\beta_1} \ldots y_{\beta_q}
$$

được tính trong $U$ (trong đó $\alpha_1 \leq \cdots \leq \alpha_p \leq \beta_1 \leq \cdots \leq \beta_q$) tương tự tạo thành một cơ sở của $U$. Do đó đồng cấu chính tắc của $U'$ vào $U$ ánh xạ các phần tử của một cơ sở của $U'$ thành các phần tử độc lập tuyến tính của $U$ và vì vậy là đơn ánh. Hơn nữa, ta thấy rằng các $y_{\beta_1} \ldots y_{\beta_q}$ (trong đó $\beta_1 \leq \cdots \leq \beta_q$) tạo thành một cơ sở của $U$ được xét như một $U'$-môđun trái. Sắp thứ tự $L \cup M$ sao cho mọi phần tử của $M$ đều nhỏ hơn mọi phần tử của $L$, ta thấy tương tự rằng các $y_{\beta_1} \ldots y_{\beta_q}$ (trong đó $\beta_1 \leq \cdots \leq \beta_q$) tạo thành một cơ sở của $U$ được xét như một $U'$-môđun phải.

Trong các điều kiện của Hệ quả 5, $U'$ được đồng nhất với đại số con của $U$ sinh bởi $h$ nhờ đồng cấu chính tắc của $U'$ vào $U$.

#### Hệ quả 6 {#lie-i-s2-lem-3-cor-6 .statement}

*Giả sử rằng $K$-môđun $g$ là tổng trực tiếp của các đại số con $g_1, g_2, \ldots, g_n$ và mỗi $g_i$ là một $K$-môđun tự do. Gọi $U_i$ là đại số bao phủ của $g_i$ ($1 \leq i \leq n$). Gọi $\phi$ là ánh xạ tuyến tính $K$ của $K$-môđun $U_1 \otimes_K \cdots \otimes_K U_n$ vào $U$ được xác định bởi ánh xạ đa tuyến tính $(u_1, \ldots, u_n) \mapsto u_1 \ldots u_n$ của $U_1 \times \cdots \times U_n$ vào $U$. Khi đó $\phi$ là một đẳng cấu $K$-môđun.*

Cho $(x^i_{\lambda})_{\lambda \in L_i}$ là một cơ sở của $g_i$. Ta sắp thứ tự toàn phần $L_1 \cup \cdots \cup L_n$ sao cho mọi phần tử của $L_i$ đều lớn hơn mọi phần tử của $L_j$ đối với $i \geq j$. Khi đó các phần tử:

$$
(x^1_{\lambda_1} x^1_{\lambda_2} \ldots x^1_{\lambda_p}) \otimes \cdots \otimes (x^n_{v_1} x^n_{v_2} \ldots x^n_{v_q}),
$$

trong đó $\lambda_1 \leq \lambda_2 \leq \cdots \leq \lambda_p \leq \cdots \leq v_1 \leq v_2 \leq \cdots \leq v_q$, tạo thành một cơ sở của $U_1 \otimes_K \cdots \otimes_K U_n$. Chúng được $\phi$ ánh xạ thành các phần tử:

$$
x^1_{\lambda_1} x^1_{\lambda_2} \ldots x^1_{\lambda_p} \ldots x^n_{v_1} x^n_{v_2} \ldots x^n_{v_q}
$$

which lập thành một cơ sở của $U$. Do đó hệ quả.

#### Hệ quả 7 {#lie-i-s2-lem-3-cor-7 .statement}

*Nếu K là một miền nguyên và g là một K-môđun tự do, đại số U không có các ước của không.*

G đẳng cấu với một đại số đa thức trên K (Định lý 1) và do đó là một miền nguyên (*Đại số*, Chương IV, § 1, no. 4, Định lý 1). Do đó hệ quả (*Đại số giao hoán*, Chương III, § 2, no. 3, Mệnh đề 1).

### 8. MỞ RỘNG CÁC ĐẠO HÀM

#### Bổ đề 4 {#lie-i-s2-lem-4 .statement}

*Cho V là một K-môđun và T là đại số tenxơ của V. Cho u là một tự đồng cấu của V. Tồn tại duy nhất một đạo hàm của T mở rộng u. Đạo hàm này giao hoán với các toán tử đối xứng trên T.*

Cho F = V × V × ... × V (n thừa số). Ánh xạ
$$
(x_1, \ldots, x_n) \mapsto ux_1 \otimes x_2 \otimes \cdots \otimes x_n \\
+ x_1 \otimes ux_2 \otimes \cdots \otimes x_n + \cdots + x_1 \otimes x_2 \otimes \cdots \otimes ux_n
$$
của F vào $\bigotimes^n V$ là đa tuyến tính. Do đó tồn tại một tự đồng cấu $u_n$ của $\bigotimes^n V$ sao cho:
$$
u_n(x_1 \otimes \cdots \otimes x_n) = ux_1 \otimes \cdots \otimes x_n + \cdots + x_1 \otimes \cdots \otimes ux_n
$$
với mọi $x_1, \ldots, x_n$ trong V. Khi đó $u_1 = u$. Gọi v là tự đồng cấu của K-môđun T trùng với $u_n$ trên mỗi $T^n = \bigotimes^n V$ và bằng không trên $T^0 = K.1$. Ta chứng minh rằng v là một đạo hàm của T. Nếu $x_1, \ldots, x_n, y_1, \ldots, y_p$ là các phần tử của V, thì
$$
v((x_1 \otimes \cdots \otimes x_n) \otimes (y_1 \otimes \cdots \otimes y_p)) \\
= \sum_{i=1}^n x_1 \otimes \cdots \otimes x_{i-1} \otimes ux_i \otimes x_{i+1} \otimes \cdots \otimes x_n \otimes y_1 \otimes \cdots \otimes y_p \\
+ \sum_{j=1}^p x_1 \otimes \cdots \otimes x_n \otimes y_1 \otimes \cdots \otimes y_{j-1} \otimes uy_j \otimes y_{j+1} \otimes \cdots \otimes y_p \\
= v(x_1 \otimes \cdots \otimes x_n) \otimes (y_1 \otimes \cdots \otimes y_p) + (x_1 \otimes \cdots \otimes x_n) \otimes v(y_1 \otimes \cdots \otimes y_p).
$$
Theo tính tuyến tính, suy ra v là một đạo hàm. Tính duy nhất của v là hiển nhiên. Cuối cùng, rõ ràng $u_n$ giao hoán với tất cả các toán tử đối xứng trên $\bigotimes^n V$, do đó có khẳng định cuối cùng.

#### Mệnh đề 7 {#lie-i-s2-prop-7 .statement}

*Cho g là một đại số Lie, U là đại số bao quanh của nó, σ là ánh xạ chính tắc của g vào U và D là một đạo hàm của g.*
(a) *Tồn tại duy nhất một đạo hàm $D_U$ của U sao cho $\sigma \circ D = D_U \circ \sigma$ (nghĩa là sao cho $D_U$ mở rộng D, khi g có thể được đồng nhất với một môđun con của U dưới σ).*
(b) $D_U$ giữ ổn định $U_n$ và tập hợp $U^n$ gồm các ảnh trong U của các tenxơ đối xứng thuần nhất cấp n trên g.

(c) $D_U$ giao hoán với phản tự đồng cấu chính tắc của $U$.

(d) *Nếu $D$ là đạo hàm nội của $g$ được xác định bởi một phần tử $x$ của $g$, $D_U$ là đạo hàm nội của $U$ được xác định bởi $\sigma(x)$.*

Gọi $D_T$ là đạo hàm của đại số tenxơ $T$ của $g$ mở rộng $D$ (Bổ đề 4). Iđêan hai phía $J$ của $T$ sinh bởi

$$
x \otimes y - y \otimes x - [x, y]
$$

$(x, y$ trong $g$) là ổn định dưới $D_T$. Vì:

$$
D_T(x \otimes y - y \otimes x - [x, y]) = Dx \otimes y - y \otimes Dx - [Dx, y]
$$
$$
+ x \otimes Dy - Dy \otimes x - [x, Dy].
$$

Khi chuyển qua thương, $D_T$ xác định một đạo hàm $D_U$ của $U$ sao cho $\sigma \circ D = D_U \circ \sigma$. Tính duy nhất của $D_U$ là ngay lập tức vì 1 và $\sigma(g)$ sinh đại số $U$. Khẳng định (b) là hiển nhiên. Gọi $A$ là phản tự đồng cấu chính tắc của $U$. Bây giờ chứng minh (c). Nếu $x_1, \ldots, x_n$ thuộc $g$, thì

$$
D_U A(\sigma(x_1) \ldots \sigma(x_n)) = D_U((-1)^n \sigma(x_n) \ldots \sigma(x_1))
$$
$$
= (-1)^n \sum_{i=1}^n \sigma(x_n) \ldots D_U(\sigma(x_i)) \ldots \sigma(x_1)
$$
$$
= (-1)^n \sum_{i=1}^n \sigma(x_n) \ldots \sigma(Dx_i) \ldots \sigma(x_1)
$$
$$
= A \left( \sum_{i=1}^n \sigma(x_1) \ldots \sigma(Dx_i) \ldots \sigma(x_n) \right)
$$
$$
= AD_U(\sigma(x_1) \ldots \sigma(x_n)).
$$

Sau cùng, cho $x \in g$. Gọi $\Delta$ là đạo hàm nội $y \mapsto \sigma(x)y - y\sigma(x)$ của $U$ (*Algebra*, Chapter IV, § 4, no. 3, *Example 2*). Khi đó, với $x' \in g$,

$$
(\Delta \circ \sigma)(x') = \sigma(x)\sigma(x') - \sigma(x')\sigma(x) = \sigma([x, x']) = (\sigma \circ \mathrm{ad}\, x)(x'),
$$

do đó $\Delta \circ \sigma = \sigma \circ \mathrm{ad}\, x$. Điều này hoàn tất chứng minh.

Áp dụng Mệnh đề 7 cho trường hợp một đại số Lie giao hoán, ta thấy rằng mọi tự đồng cấu $u$ của một $K$-môđun đều có thể được mở rộng một cách duy nhất thành một đạo hàm của đại số đối xứng của môđun này; đạo hàm này được dẫn xuất, khi chuyển qua thương, từ đạo hàm của đại số tenxơ mở rộng $u$.

Ta lại lấy một đại số Lie $g$ trên $K$ và gọi $D$ là một đạo hàm của $g$. Ta dùng các ký hiệu đã có trước đó $T, S, U, G$. Gọi $D_T, D_S$ là các đạo hàm của $T, S$ mở rộng $D$ và gọi $D_U$ là đạo hàm duy nhất của $U$ sao cho $\sigma \circ D = D_U \circ \sigma$. Vì $D_U$ giữ ổn định các $U_n$, nên $D_U$ xác định, khi lấy thương, một đạo hàm $D_G$ của $G$. Vì $D_U$ và $D_S$ được dẫn xuất từ $D_T$ khi chuyển qua thương, biểu đồ giao hoán (3) chứng tỏ rằng $D_G$ cũng có thể được dẫn xuất từ $D_S$ bởi đồng cấu $\omega$ được định nghĩa trong no. 6. Hơn nữa, nếu $K$ là một trường có đặc số 0, các đẳng cấu của biểu đồ (4) biến các hạn chế của $D_T, D_S, D_U, D_G$ trên ${S'}^n, S^n, U^n, G^n$ thành nhau. Vậy nên đẳng cấu chính tắc của $S$ lên $U$ biến $D_S$ thành $D_U$.

### 9. MỞ RỘNG VÀNH CƠ SỞ

Cho $g$ là một đại số Lie trên $K$, $T$ là đại số tenxơ của nó, $J$ là iđêan hai phía của $T$ sinh bởi các $x \otimes y - y \otimes x - [x, y]$ ($x, y$ trong $g$) và $U = T/J$. Cho $K_1$ là một vành giao hoán có phần tử đơn vị và $\sigma$ là một đồng cấu của $K$ vào $K_1$ biến 1 thành 1. Khi đó đại số tenxơ của $g_{(K_1)}$ được đồng nhất một cách chính tắc với $T_{(K_1)}$. Gọi $J'$ là iđêan hai phía của $T_{(K_1)}$ sinh bởi các

$$
x' \otimes y' - y' \otimes x' - [x', y']
$$

($x', y'$ trong $g_{(K_1)}$). Rõ ràng ảnh chính tắc của $J_{(K_1)}$ trong $T_{(K_1)}$ được chứa trong $J'$. Để thấy rằng nó bằng $J'$, chỉ cần chứng minh rằng, nếu $x'$ và $y'$ là hai phần tử của $g_{(K_1)}$, $x' \otimes y' - y' \otimes x' - [x', y']$ thuộc vào ảnh này. Khi đó

$$
x' = \sum_i x_i \otimes \lambda_i, y' = \sum_j y_j \otimes \mu_j \quad (x_i, y_j \text{ trong } g, \lambda_i, \mu_j \text{ trong } K_1);
$$

do đó

$$
x' \otimes y' - y' \otimes x' - [x', y'] = \sum_{i,j} (x_i \otimes y_j - y_j \otimes x_i - [x_i, y_j]) \otimes \lambda_i \mu_j
$$

điều này chứng minh mệnh đề của chúng ta. Sau đó có thể thấy rằng $U_{(K_1)} = (T/J)_{(K_1)}$ được đồng nhất một cách chính tắc với $T_{(K_1)}/J'$: *đại số bao của $g_{(K_1)}$ được đồng nhất một cách chính tắc với $U_{(K_1)}$* và ánh xạ chính tắc của $g_{(K_1)}$ vào đại số bao của nó được đồng nhất với $\sigma \otimes 1$ (trong đó $\sigma$ ký hiệu ánh xạ chính tắc của $g$ vào $U$).

### Bài tập {#lie-i-s2-exercises}

Xem các [bài tập của § 2](exercises/s2/).
