---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 4
section_title: Tensor products of algebras
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 460-484, 626-627
pdf_pages: 0484-0508, 0650-0651
extraction: ocr
subsections:
    - "no": 1
      title: TENSOR PRODUCT OF A FINITE FAMILY OF ALGEBRAS
      page: 460
      pdf_page: 484
    - "no": 2
      title: UNIVERSAL CHARACTERIZATION OF TENSOR PRODUCTS OF ALGEBRAS
      page: 463
      pdf_page: 487
    - "no": 3
      title: MODULES AND MULTIMODULES OVER TENSOR PRODUCTS OF ALGEBRAS
      page: 465
      pdf_page: 489
    - "no": 4
      title: TENSOR PRODUCT OF ALGEBRAS OVER A FIELD
      page: 468
      pdf_page: 492
    - "no": 5
      title: TENSOR PRODUCT OF AN INFINITE FAMILY OF ALGEBRAS
      page: 470
      pdf_page: 494
    - "no": 6
      title: COMMUTATION LEMMAS
      page: 472
      pdf_page: 496
    - "no": 7
      title: TENSOR PRODUCT OF GRADED ALGEBRAS RELATIVE TO COMMUTATION FACTORS
      page: 474
      pdf_page: 498
    - "no": 8
      title: TENSOR PRODUCT OF GRADED ALGEBRAS OF THE SAME TYPES
      page: 480
      pdf_page: 504
    - "no": 9
      title: ANTICOMMUTATIVE ALGEBRAS AND ALTERNATING ALGEBRAS
      page: 482
      pdf_page: 506
statements: 43
exercises: 2
content_sha256: aec2dc96f9a432987b2e1c8246cc1a75cdba73cb523b5c8551059dd17aeac1a1
translated_from: content/en/alg/III/04_s4_tensor_products_of_algebras.md
source_content_sha256: 104babe43ca0f7b29fb3d06064b2db49850bf4ce36b16bfb4fc025a8d61a1f77
translation_model: gpt-5.4
translation_run: translate-vi-b55d44b5
glossary_version: 34
glossary_terms_sha256: c2c9b0460c4cd91ead64d23156ce206914b3ed2519c096f28919ae8209178687
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. TÍCH TENXƠ CỦA CÁC ĐẠI SỐ

Từ § 4 đến § 8 kể cả, A ký hiệu một vành giao hoán, và, trừ khi có nói khác, các đại số được xét được giả thiết là kết hợp và có đơn vị và các đồng cấu đại số được giả thiết là có đơn vị.

### 1. TÍCH TENXƠ CỦA MỘT HỌ HỮU HẠN CÁC ĐẠI SỐ

A luôn ký hiệu một vành giao hoán có phần tử đơn vị. Cho (E_i)_{i \in I} là một họ hữu hạn các đại số trên A và đặt E = \bigotimes_{i \in I} E_i là A-môđun tích tenxơ của các A-môđun E_i (II, § 3, no. 9). Ta sẽ định nghĩa một cấu trúc đại số trên A trên E. Cho m_i: E_i \otimes_A E_i \to E_i là ánh xạ A-tuyến tính xác định phép nhân trên E_i (§ 1, no. 3). Xét ánh xạ A-tuyến tính

$$
m' = \bigotimes_{i \in I} m_i: \bigotimes_{i \in I} (E_i \otimes_A E_i) \to \bigotimes_{i \in I} E_i = E;
$$

ánh xạ hợp thành

$$
\left( \bigotimes_{i \in I} E_i \right) \otimes_A \left( \bigotimes_{i \in I} E_i \right) \xrightarrow{\tau} \bigotimes_{i \in I} (E_i \otimes_A E_i) \xrightarrow{m'} \bigotimes_{i \in I} E_i
$$

trong đó $\tau$ là đẳng cấu kết hợp (II, § 3, no. 9) là một ánh xạ A-tuyến tính $m : E \otimes_A E \to E$; ta sẽ thấy rằng $m$ xác định một cấu trúc đại số (kết hợp và có đơn vị) trên $E$. Thật vậy, khi thực hiện tường minh phép nhân do $m$ xác định, ta thu được công thức

(1)
$$
\left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) = \bigotimes_{i \in I} (x_i y_i) \quad \text{với } x_i, y_i \text{ trong } E_i \text{ và } i \in I.
$$

Do đó đã thấy ngay, bởi tính tuyến tính, rằng nếu $e_i$ là phần tử đơn vị của $E_i$, thì $e = \bigotimes_{i \in I} e_i$ là phần tử đơn vị của $E$. Mặt khác, tính kết hợp của mỗi E_i suy ra quan hệ

$$
\left( \left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) \right) \left( \bigotimes_{i \in I} z_i \right) = \bigotimes_{i \in I} (x_i y_i z_i) = \left( \bigotimes_{i \in I} x_i \right) \left( \left( \bigotimes_{i \in I} y_i \right) \left( \bigotimes_{i \in I} z_i \right) \right)
$$

do đó, bởi tính tuyến tính, có quan hệ $x(yz) = (xy)z$ với mọi $x, y, z$ trong $E$.

#### Định nghĩa 1 {#alg-iii-s4-def-1 .statement}

*Cho một họ* $(E_i)_{i \in I}$ *các đại số trên* $A$, *tích tenxơ của họ này*, ký hiệu bởi $\bigotimes_{i \in I} E_i$ (hoặc, khi $I$ là khoảng $\{1, n\}$ của $\mathbf{N}$, $E_1 \otimes_A E_2 \otimes \cdots \otimes_A E_n$, hoặc đơn giản là $E_1 \otimes E_2 \otimes \cdots \otimes E_n$) *là đại số thu được bằng cách trang bị cho tích tenxơ của các* $A$*-môđun* $E_i$ *phép nhân được xác định bởi* (1).

Quan hệ (1) cho thấy rằng tích tenxơ $\bigotimes_{i \in I} E_i^0$ của các đại số *đối* của các E_i là đại số đối của $\bigotimes_{i \in I} E_i$; đặc biệt, nếu các E_i là *giao hoán* thì $\bigotimes_{i \in I} E_i$ cũng vậy.

Cho $(E_i)_{i \in I}$ và $(F_i)_{i \in I}$ là hai họ các đại số trên $A$ có cùng tập hợp chỉ số hữu hạn $I$. Với mỗi $i \in I$, cho $f_i : E_i \to F_i$ là một đồng cấu đại số trên $A$. Khi đó ánh xạ A-tuyến tính

$$
f = \bigotimes_{i \in I} f_i : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} F_i
$$

là một *đồng cấu đại số trên A*, như suy ra từ (1).

Với mọi phân hoạch $(I_j)_{j \in J}$ của $I$, các đẳng cấu kết hợp

$$
\bigotimes_{j \in J} \left( \bigotimes_{i \in I_j} E_i \right) \to \bigotimes_{i \in I} E_i
$$

(II, § 3, no. 9) cũng là các đẳng cấu *đại số*, như suy ra từ (1) và các định nghĩa của chúng.

Khi $I$ là khoảng $[1, n]$ của $\mathbf{N}$ và tất cả các đại số E_i đều bằng cùng một đại số $E$, đại số tích tenxơ $\bigotimes_{i \in I} E_i$ cũng được ký hiệu bởi $E^{\otimes n}$.

Trong phần còn lại của số này, ta sẽ chỉ giới hạn sự chú ý vào các tính chất của tích tenxơ của hai đại số, dành cho người đọc việc mở rộng chúng sang các tích tenxơ của những họ hữu hạn tùy ý.

Cho $E, F$ là hai $A$-đại số; nếu $a$ (resp. $b$) là một iđêan trái của $E$ (resp. $F$), ảnh chính tắc $\operatorname{Im}(a \otimes b)$ của $a \otimes_A b$ trong $E \otimes_A F$ là một iđêan trái của $E \otimes_A F$; có các kết quả tương tự khi thay "iđêan trái" bằng "iđêan phải" hoặc "iđêan hai phía". Hơn nữa:

#### Mệnh đề 1 {#alg-iii-s4-prop-1 .statement}

*Cho $E, F$ là hai $A$-đại số và $a$ (resp. $b$) là một iđêan hai phía của $E$ (resp. $F$). Khi đó đẳng cấu $A$-môđun chính tắc*

$$
(E/a) \otimes (E/b) \to (E \otimes F)/(\operatorname{Im}(a \otimes F) + \operatorname{Im}(E \otimes b))
$$

(II, § 3, no. 6, Hệ quả 1 của Mệnh đề 6) *là một đẳng cấu đại số*.

Điều này suy ra từ (1) và định nghĩa đã cho ở *loc. cit*.

#### Hệ quả 1 {#alg-iii-s4-prop-1-cor-1 .statement}

*Cho $E$ là một $A$-đại số và $a$ là một iđêan của $A$. Khi đó $A$-môđun $aE$ là một iđêan hai phía của $E$ và đẳng cấu $(A/a)$-môđun chính tắc*

$$
(A/a) \otimes_A E \to E/aE
$$

*là một đẳng cấu $(A/a)$-đại số*.

#### Hệ quả 2 {#alg-iii-s4-prop-1-cor-2 .statement}

*Nếu $a, b$ là hai iđêan của $A$, thì $(A/a) \otimes_A (A/b)$ đẳng cấu chính tắc với $A/(a + b)$*.

#### Hệ quả 3 {#alg-iii-s4-prop-1-cor-3 .statement}

*Cho $E, F$ là hai $A$-đại số và $a$ là một iđêan của $A$ được chứa trong linh hóa tử của $F$. Khi đó $(A/a)$-đại số $E \otimes_A F$ đẳng cấu chính tắc với $(E/aE) \otimes_{A/a} F$*.

#### Mệnh đề 2 {#alg-iii-s4-prop-2 .statement}

*Cho $(E_\lambda)_{\lambda \in L}$ và $(F_\mu)_{\mu \in M}$ là hai họ $A$-đại số. Ánh xạ chính tắc* (II, § 3, no. 7)

$$
\left( \bigoplus_{\lambda \in L} E_\lambda \right) \otimes_A \left( \bigoplus_{\mu \in M} F_\mu \right) \to \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$

*là một đẳng cấu đại số*.

Điều này suy ra ngay lập tức từ II, § 3, no. 7, Mệnh đề 7 và định nghĩa của phép nhân trên $E \otimes F$.

#### Mệnh đề 3 {#alg-iii-s4-prop-3 .statement}

*Cho $A, B$ là hai vành giao hoán, $\varphi : A \to B$ là một đồng cấu vành và $E, F$ là hai $A$-đại số. Khi đó đẳng cấu $B$-môđun chính tắc*

$$
\varphi^*(E) \otimes_B \varphi^*(F) \to \varphi^*(E \otimes_A F)
$$

(II, § 5, no. 1, Mệnh đề 3) *là một đẳng cấu $B$-đại số*.

#### Mệnh đề 4 {#alg-iii-s4-prop-4 .statement}

Cho $A, B$ là hai vành giao hoán, $\rho : A \to B$ là một đồng cấu vành, $E$ là một $A$-đại số và $F$ là một $B$-đại số. Khi đó đẳng cấu $A$-môđun chính tắc

$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E))
$$

(II, § 5, no. 2, Mệnh đề 6) là một đẳng cấu đại số $A$.

Các phép kiểm tra là tầm thường do § 1, no. 5.

Đặc biệt, cấu trúc đại số $A$ trên $B \otimes_A E$, thu được bằng cách hạn chế vành vô hướng $B$ xuống $A$, trùng với cấu trúc của đại số $B \otimes_A E$, tích tenxơ của các đại số $A$ $B$ và $E$.

Cuối cùng, nếu $(A_i, \phi_{ji})$ là một hệ trực tiếp các vành giao hoán, $(E_i, f_{ji})$ và $(F_i, g_{ji})$ là hai hệ trực tiếp các đại số $A_i$ ($§ 1$, no. 6) và $A = \lim \rightarrow A_i$, thì đẳng cấu môđun $A$ chính tắc

$$
\lim \rightarrow (E_i \otimes_{A_i} F_i) \to (\lim \rightarrow E_i) \otimes_A (\lim \rightarrow F_i)
$$

(II, § 6, no. 3, Mệnh đề 7) cũng là một đẳng cấu đại số $A$, như suy ra từ các định nghĩa.

Các ví dụ về tích tenxơ của các đại số. (1) Cho $A$ là một vành giao hoán và $M, N$ là hai $A$-môđun; ánh xạ chính tắc

$$
\text{End}_A(M) \otimes_A \text{End}_A(N) \to \text{End}_A(M \otimes_A N)
$$

(II, § 4, no. 4) là một đồng cấu đại số $A$, như suy ra từ II, § 3, no. 2, công thức (5). Khi $M$ hoặc $N$ là một $A$-môđun xạ ảnh sinh hữu hạn, ta biết rằng đồng cấu này là song ánh (II, § 4, no. 4, Mệnh đề 4). Đặc biệt, ta thu lại định nghĩa của tích tenxơ của hai ma trận vuông.

(2) Cho $S, T$ là hai monoid và $A^{(S)}$ và $A^{(T)}$ là các đại số của các monoid $S$ và $T$ trên vành $A$ (III, § 2, no. 6); khi đó có một đẳng cấu đại số $A$ chính tắc

$$
A^{(S)} \otimes_A A^{(T)} \to A^{(S \times T)}.
$$

Các phần tử $e_s \otimes e_t$ (tương ứng $e_{(s,t)}$), trong đó $s$ chạy qua $S$ và $t$ chạy qua $T$, tạo thành một cơ sở của $A^{(S)} \otimes_A A^{(T)}$ theo II, § 3, no. 7, Hệ quả 2 của Mệnh đề 7 (tương ứng của $A^{(S \times T)}$); đẳng cấu cần tìm thu được bằng cách ánh xạ $e_s \otimes e_t$ thành $e_{(s,t)}$ và từ các định nghĩa suy ra rằng đây thực sự là một đẳng cấu đại số.

### 2. ĐẶC TRƯNG HÓA PHỔ QUÁT CỦA TÍCH TENXƠ CÁC ĐẠI SỐ

#### Mệnh đề 5 {#alg-iii-s4-prop-5 .statement}

Cho $(E_i)_{i \in I}$ là một họ hữu hạn các đại số $A$ và, với mỗi $i \in I$, ký hiệu $e_i$ là phần tử đơn vị của $E_i$. Với mỗi $i \in I$, ký hiệu $u_i : E_i \to E = \bigotimes_{i \in I} E_i$ là ánh xạ tuyến tính $A$ được xác định bởi

$$
u_i(x_i) = \bigotimes_j x'_j \quad \text{với } x'_i = x_i \text{ và } x'_j = e_j \text{ với } j \neq i.
$$

(i) *Các $u_i$ là các đẳng cấu $\mathbf{A}$-đại số; hơn nữa, với $i \neq j$, các phần tử $u_i(x_i)$ và $u_j(x_j)$ là hoán vị được trong $\mathbf{E}$ với mọi $x_i \in \mathbf{E}_i$ và $x_j \in \mathbf{E}_j$, và $\mathbf{E}$ được sinh bởi hợp của các đại số con $u_i(\mathbf{E}_i)$.

(ii) *Cho $\mathbf{F}$ là một $\mathbf{A}$-đại số và, với mọi $i \in \mathbf{I}$, cho $v_i : \mathbf{E}_i \to \mathbf{F}$ là một đồng cấu $\mathbf{A}$-đại số, trong đó các $v_i$ sao cho, với $i \neq j$, $v_i(x_i)$ và $v_j(x_j)$ là hoán vị được trong $\mathbf{F}$ với mọi $x_i \in \mathbf{E}_i$ và $x_j \in \mathbf{E}_j$. Khi đó tồn tại một và chỉ một đồng cấu $\mathbf{A}$-đại số $w : \mathbf{E} \to \mathbf{F}$ sao cho*

$$
v_i = w \circ u_i \quad \text{với mọi } i \in \mathbf{I}.
$$

(i) Ánh xạ $u_i$ là một đồng cấu đại số theo định nghĩa của phép nhân trên $\mathbf{E}$. Nếu $i \neq j$, $x_i \in \mathbf{E}_i, x_j \in \mathbf{E}_j$, thì

$$
u_i(x_i) = \bigotimes_k x'_k \quad \text{sao cho } x'_i = x_i, x'_k = e_k \text{ với } k \neq i,
$$
$$
u_j(x_j) = \bigotimes_k x''_k \quad \text{sao cho } x''_j = x_j, x''_k = e_k \text{ với } k \neq j.
$$

Rõ ràng $x'_k x''_k = x''_k x'_k$ với mọi $k \in \mathbf{I}$ và do đó $u_i(x_i)$ và $u_j(x_j)$ giao hoán trong $\mathbf{E}$ theo công thức (1) (no. 1) định nghĩa phép nhân trong $\mathbf{E}$. Khẳng định cuối cùng suy ra từ quan hệ $\bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i)$.

(ii) Với mỗi $i \in \mathbf{I}$, cho $x_i$ là một phần tử của $\mathbf{E}_i$. Khi đó tích $\prod_{i \in \mathbf{I}} v_i(x_i)$ được xác định trong $\mathbf{F}$ độc lập với mọi thứ tự trên $\mathbf{I}$ vì đại số $\mathbf{F}$ là kết hợp và các phần tử $v_i(x_i)$ là hoán vị được từng đôi một. Ánh xạ $(x_i)_{i \in \mathbf{I}} \to \prod_{i \in \mathbf{I}} v_i(x_i)$ từ $\prod_{i \in \mathbf{I}} \mathbf{E}_i$ vào $\mathbf{F}$ hiển nhiên là $\mathbf{A}$-tuyến tính nhiều biến và do đó tồn tại một và chỉ một ánh xạ $\mathbf{A}$-tuyến tính $w : \mathbf{E} \to \mathbf{F}$ sao cho

$$
w\left( \bigotimes_i x_i \right) = \prod_i v_i(x_i).
$$

Bây giờ, đồng cấu đại số trên $\mathbf{A}$ cần tìm $w : \mathbf{E} \to \mathbf{F}$ phải thỏa mãn (5), điều này suy ra từ (4) và thực tế là $\bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i)$. Điều này chứng minh tính duy nhất của $w$; còn phải chứng tỏ rằng ánh xạ $\mathbf{A}$-tuyến tính $w$ được xác định bởi (5) là một đồng cấu đại số trên $\mathbf{A}$ và thỏa mãn (4). Việc $w$ thỏa mãn (4) là hiển nhiên: chỉ cần áp dụng (5) cho trường hợp $x_j = e_j$ với $j \neq i$ và ta được $w(u_i(x_i)) = v_i(x_i)$. Cuối cùng, $w$ là một đồng cấu đại số, vì

$$
w\left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) = w\left( \bigotimes_i (x_i y_i) \right) = \prod_i v_i(x_i y_i)
$$
$$
= \prod_i (v_i(x_i) v_i(y_i)) = \left( \prod_i v_i(x_i) \right) \cdot \left( \prod_i v_i(y_i) \right)
$$

vì $v_i(x_i)$ giao hoán với $v_j(y_j)$ khi $j \neq i$; do đó

$$
w w \left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) = w \left( \bigotimes_i x_i \right) . w \left( \bigotimes_i y_i \right)
$$

điều này, theo tính tuyến tính, hoàn tất chứng minh.

Cặp có thứ tự gồm E và ánh xạ chính tắc $\phi : (x_i) \mapsto \bigotimes_i x_i$ từ $\prod_i E_i$ vào E là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1), trong đó $\Sigma$ là loài cấu trúc đại số trên A, các cấu xạ là các đồng cấu đại số trên A và các ánh xạ-$\alpha$ là các ánh xạ $\prod_i u_i$ từ $\prod_i E_i$ vào một đại số trên A sao cho các $u_i$ là các đồng cấu đại số trên A và $u_i(x_i)$ và $u_j(x_j)$ giao hoán với nhau khi $i \neq j$, với mọi $x_i \in E_i$ và $x_j \in E_j$.

#### Hệ quả {#alg-iii-s4-n2-cor-1 .statement}

*Cho* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *là hai họ hữu hạn các đại số trên A và, với mọi* $i \in I$, *cho* $f_i : E_i \to F_i$ *là một đồng cấu đại số. Nếu* $u_i : E_i \to \bigotimes_{j \in I} E_j, v_i : F_i \to \bigotimes_{j \in I} F_j$ *là các đồng cấu chính tắc, thì ánh xạ* $f = \bigotimes_i f_i$ *(xem no. 1)* *là đồng cấu đại số trên A duy nhất sao cho* $f \circ u_i = v_i \circ f_i$ *với mọi* $i \in I$.

Chỉ cần chú ý rằng các đồng cấu $g_i = v_i \circ f_i$ có tính chất là $g_i(x_i) = v_i(f_i(x_i))$ và $g_j(x_j) = v_j(f_j(x_j))$ giao hoán với nhau khi $i \neq j$, $x_i \in E_i$ và $x_j \in E_j$; rồi áp dụng Mệnh đề 5.

Khi, trong Mệnh đề 5, đại số F được giả sử là *giao hoán*, giả thiết rằng $v_i(x_i)$ và $v_j(x_j)$ hoán vị được với nhau khi $i \neq j$ tự động được thỏa mãn. Do đó, *khi F giao hoán*, có một song ánh chính tắc

$$
\text{Hom}_{A\text{-alg.}} \left( \bigotimes_i E_i, F \right) \to \prod_i \text{Hom}_{A\text{-alg.}} (E_i, F),
$$

cụ thể là song ánh gán cho mỗi đồng cấu $w$ từ $\bigotimes_i E_i$ vào F họ các $w \circ u_i$.

Chú ý rằng nếu E là một đại số giao hoán trên A, thì cấu trúc vành của $E \otimes_A F$ cũng chính là cấu trúc vành của $F_{(E)}$ (§ 1, no. 5).

### 3. MÔĐUN VÀ ĐA MÔĐUN TRÊN CÁC TÍCH TENXƠ CỦA ĐẠI SỐ

#### Định nghĩa 2 {#alg-iii-s4-def-2 .statement}

*Cho E là một đại số trên A (có đơn vị). Một E-môđun trái (tương ứng, phải) là một môđun trái (tương ứng, phải) trên vành nền của E.*

Trừ khi có nói rõ ngược lại, mọi môđun và đa môđun được xét trong no. này đều là môđun trái và đa môđun trái.

Nếu M là một E-môđun, thì đồng cấu $\eta : A \to E$ (§ 1, no. 4) xác định trên M một cấu trúc A-môđun, được gọi là cấu trúc nền của cấu trúc E-môđun trên M; với $\alpha \in A, s \in E, x \in M$,

$$
\alpha(sx) = s(\alpha x) = (\alpha s)x,
$$

do đó với mọi $s \in E$, phép vị tự $h_s : x \mapsto sx$ của M là một tự đồng cấu của cấu trúc A-môđun nền. Ngược lại, việc cho một cấu trúc E-môđun trên M tương đương với việc cho một cấu trúc A-môđun trên M và một đồng cấu đại số trên A $s \mapsto h_s$ từ E vào $\mathrm{End}_A(M)$.

#### Định nghĩa 3 {#alg-iii-s4-def-3 .statement}

*Cho E và F là hai đại số trên A (có đơn vị) và M là một tập hợp được trang bị một cấu trúc E-môđun và một cấu trúc F-môđun. M được gọi là một song môđun (trái) trên các đại số E và F nếu:*

(1) *M là một song môđun trên các vành nền của E và F* (II, § 1, no. 14);
(2) *hai cấu trúc A-môđun nền của các cấu trúc E-môđun và F-môđun trên M là đồng nhất*.

Điều kiện sau cùng này nói rằng nếu e và $e'$ lần lượt là các phần tử đơn vị của E và F, thì

$$
(\alpha e)x = (\alpha e')x \quad \text{với } \alpha \in A, x \in M;
$$

khi đó $\alpha x$ được dùng để ký hiệu giá trị chung của hai vế.

Cũng có thể nói rằng việc cho trên M một cấu trúc song môđun trên E và F là tương đương với việc cho một cấu trúc A-môđun trên M và thêm vào đó hai đồng cấu đại số trên A $s \mapsto h'_s$ từ E vào $\mathrm{End}_A(M)$ và $t \mapsto h''_t$ từ F vào $\mathrm{End}_A(M)$ sao cho $h'_s h''_t = h''_t h'_s$ với mọi $s \in E$ và $t \in F$. Do đó (no. 2, Mệnh đề 5) một đồng cấu đại số trên A $u \mapsto h_u$ từ $E \otimes_A F$ vào $\mathrm{End}_A(M)$ được dẫn xuất một cách chính tắc sao cho $h_{s \otimes t} = h'_s h''_t = h''_t h'_s$ với $s \in E$ và $t \in F$. Nói cách khác, một cấu trúc $(E \otimes_A F)$-môđun do đó được định nghĩa trên M, được gọi là liên kết với cấu trúc song môđun đã cho trên E và F và theo đó

$$
(s \otimes t).x = s(tx) = t(sx) \quad \text{với } s \in E, t \in F \text{ và } x \in M.
$$

Các cấu trúc E-môđun và F-môđun đã cho trên M có thể được dẫn xuất từ cấu trúc $(E \otimes_A F)$-môđun này bằng cách hạn chế vành các vô hướng, tương ứng với hai đồng cấu chính tắc $E \to E \otimes_A F$ và $F \to E \otimes_A F$.

Ngược lại, nếu một cấu trúc $(E \otimes_A F)$-môđun được cho trên M, nhờ các đồng cấu chính tắc $E \to E \otimes_A F$ và $F \to E \otimes_A F$ ta được một cấu trúc E-môđun và một cấu trúc F-môđun trên M và ngay lập tức thấy rằng M là một *song môđun* trên các đại số E và F với hai cấu trúc ấy và rằng cấu trúc $(E \otimes_A F)$-môđun đã cho là liên kết với cấu trúc song môđun này.

Như vậy một sự tương ứng một-một đã được thiết lập giữa các $(E \otimes_A F)$-môđun và các song môđun trên các đại số E và F. Rõ ràng mọi môđun con song của M đều là một môđun con đối với cấu trúc $(E \otimes_A F)$-môđun liên kết và ngược lại. Có các kết quả tương tự đối với các thương, tích, tổng trực tiếp và các giới hạn nghịch đảo và trực tiếp. Sau cùng, nếu $M'$ là một song môđun khác trên các đại số E và F và $f : M \to M'$ là một đồng cấu song môđun, thì $f$ cũng là một đồng cấu $(E \otimes_A F)$-môđun và ngược lại.

Hiển nhiên cũng có các mệnh đề tương ứng đối với các cấu trúc song môđun phải, hoặc chẳng hạn khi có một cấu trúc E-môđun trái và một cấu trúc F-môđun phải; trong trường hợp này ta nói đến một $(E, F)$-song môđun và việc cho một cấu trúc như vậy tương đương với việc cho một cấu trúc song môđun trái trên E và $F^o$.

#### Ví dụ {#alg-iii-s4-n3-exa-1 .statement}

(1) Cho B là một đại số trên A; vành B có một cách chính tắc một cấu trúc (B, B)-song môđun (II, § 1, no. 14, Ví dụ 1) và, nếu e là phần tử đơn vị của B, thì $(\alpha e)x = x(\alpha e) = \alpha x$ với mọi $x \in B$ và mọi $\alpha \in A$; vì vậy B có thể được xem như một song môđun trái trên các đại số B và $B^o$ (đối của B); do đó có một cấu trúc $(B \otimes_A B^o)$-môđun liên kết với cấu trúc (B, B)-song môđun trên B sao cho, với $b, x$ và $b'$ trong B,

$$
(b \otimes b').x = bx b'
$$

vế phải là tích trong vành B.

(2) Cho E và F là hai đại số trên A, $e, e'$ là các phần tử đơn vị tương ứng của chúng, M là một E-môđun và N là một F-môđun; các cấu trúc môđun này xác định trên M một cấu trúc song môđun trên các vành A và E và trên N một cấu trúc song môđun trên các vành A và F; từ đó do đó dẫn xuất được một cấu trúc song môđun trên các vành E và F trên tích tenxơ $M \otimes_A N$, được định nghĩa bởi

$$
x.(m \otimes n) = (x.m) \otimes n, \quad y.(m \otimes n) = m \otimes (y.n)
$$

với $x \in E, y \in F, m \in M, n \in N$ (II, § 3, no. 4); cũng thấy rằng các điều kiện (8) được thỏa mãn và vì thế cấu trúc song môđun trên đây liên kết với một cấu trúc $(E \otimes_A F)$-môđun trên $M \otimes_A N$, sao cho

$$
(x \otimes y).(m \otimes n) = (x.m) \otimes (y.n)
$$

với $x \in E, y \in F, m \in M, n \in N$.

Đặc biệt, lấy $M = E_s, E_s \otimes_A N$ có một cách chính tắc một cấu trúc môđun trên $(E \otimes_A F)$; mặt khác, $E \otimes_A N$ được đồng nhất một cách chính tắc với $E \otimes_A (F_d \otimes_F N) = (E \otimes_A F) \otimes_F N$, trong đó $E \otimes_A F$ được xét với cấu trúc F-môđun phải được định nghĩa bởi đồng cấu chính tắc $v : F \to E \otimes_A F$; với $x, x'$ trong E, $y \in F, n \in N$, $x' \otimes n$ do đó được đồng nhất với $(x' \otimes e') \otimes n$ và $(x \otimes y).(x' \otimes n') = (xx') \otimes (y.n)$ với $((xx') \otimes y) \otimes n$. Môđun trên $(E \otimes_A F)$ là $E_s \otimes_A N$ do đó được đồng nhất với môđun trên $(E \otimes_A F)$ dẫn xuất từ N bằng cách mở rộng vô hướng lên $E \otimes_A F$ nhờ đồng cấu $v$ (II, § 5, no. 1). Ánh xạ chính tắc $n \mapsto e \otimes n$ từ N vào $E_s \otimes_A N$ được đồng nhất với ánh xạ chính tắc $n \mapsto (e \otimes e') \otimes n$ từ N vào $(E \otimes_A F) \otimes_F N$; điều này được biết là một F-đồng cấu.

Với cùng ký hiệu ấy, cho P là một môđun phải trên $(E \otimes_A F)$; khi đó có một đẳng cấu Z-môđun chính tắc

(11) $$ P \otimes_{E \otimes_A F} (E_s \otimes_A N) \to P \otimes_F N $$

trong đó ở vế phải P được xét như một F-môđun phải nhờ đồng cấu chính tắc $v$. Thật vậy, P được đồng nhất một cách chính tắc với $P \otimes_{E \otimes_A F} (E \otimes_A F)$ và $(E \otimes_A F) \otimes_F N$ với $E \otimes_A (F \otimes_F N)$ và do đó với $E \otimes_A N$, điều này thiết lập đẳng cấu đã phát biểu (II, § 3, no. 8, Mệnh đề 8 and II, § 3, no. 4, mệnh đề 4).

Tất cả những điều trên đều mở rộng được cho các *đa môđun* (II, § 1, no. 14).

### 4. TÍCH TENXƠ CỦA CÁC ĐẠI SỐ TRÊN MỘT TRƯỜNG

Cho K là một *trường* giao hoán và E, F là hai đại số trên K mà các phần tử đơn vị tương ứng $e, e'$ là *khác không*. Khi đó các đồng cấu $\eta_E : K \to E$ và $\eta_F : K \to F$ (§ 1, no. 3) là đơn ánh, cho phép ta đồng nhất K với một trường con của E (tương ứng của F). Các đồng cấu chính tắc $u : E \to E \otimes_K F$ và $v : F \to E \otimes_K F$, được định nghĩa bởi $u(x) = x \otimes e'$ và $v(y) = e \otimes y$ là *đơn ánh* (II, § 7, no. 9, Proposition 19) và cho phép ta đồng nhất E và F với các *đại số con* của $E \otimes_K F$, cả hai đều có phần tử đơn vị là phần tử đơn vị $e \otimes e'$ của $E \otimes_K F$. Trong $E \otimes_K F, E \cap F = K$ (II, § 7, no. 9, Proposition 19).

Nếu E' và F' lần lượt là các đại số con của E và F, thì đồng cấu chính tắc $E' \otimes_K F' \to E \otimes_K F$ là đơn ánh và cho phép ta đồng nhất $E' \otimes_K F'$ với đại số con của $E \otimes_K F$ được sinh bởi $E' \cup F'$ (II, § 7, no. 7, Proposition 14).

#### Mệnh đề 6 {#alg-iii-s4-prop-6 .statement}

*Cho E, F là hai đại số khác không trên một trường giao hoán, K, C (tương ứng D) là một đại số con của E (tương ứng của F) và C' (tương ứng D') là tập trung hóa tử của C trong E (tương ứng của D trong F). Khi đó tập trung hóa tử của C \otimes_K D trong E \otimes_K F là C' \otimes_K D'.*

Tất cả quy về việc kiểm tra rằng một phần tử $z = \sum_i x_i \otimes y_i$ của tập trung hóa tử của $C \otimes_K D$ ($x_i \in F, y_i \in F$) thuộc $C' \otimes_K D'$; ta biết rằng

$$
C' \otimes_K D' = (C' \otimes_K F) \cap (E \otimes_K D')
$$

(II, § 7, no. 7, Hệ quả to Proposition 14). Có thể giả thiết các $y_i$ độc lập tuyến tính trên K; với mọi $x \in C$, tất yếu có $(x \otimes e')z = z(x \otimes e')$, tức là $\sum_i (xx_i - x_ix) \otimes y_i = 0$, do đó $xx_i = x_ix$ với mọi $i$ (II, § 3, no. 7, Hệ quả 1 to Proposition 7); vì thế tất yếu $x_i \in C'$ với mọi $i$ và do đó $z \in C' \otimes_K F$; tương tự có thể chứng minh rằng $z \in E \otimes_K D'$, do đó có mệnh đề.

#### Hệ quả {#alg-iii-s4-n4-cor-1 .statement}

*Nếu Z và Z' là các tâm tương ứng của E và F, thì tâm của E \otimes_K F là Z \otimes_K Z'*.

Cho E và F là hai đại số con của một đại số G trên một trường giao hoán K; giả sử rằng mọi phần tử của E đều giao hoán với mọi phần tử của F. Khi đó các đơn ánh chính tắc $i : E \to G, j : F \to G$ xác định một đồng cấu chính tắc $h = i \otimes j : E \otimes_K F \to G$ (no. 2, Mệnh đề 5) sao cho
$$
(i \otimes j)(x \otimes y) = xy \quad \text{với } x \in E, y \in F.
$$

#### Định nghĩa 4 {#alg-iii-s4-def-4 .statement}

*Cho một đại số G trên một trường giao hoán K, hai đại số con E, F của G được gọi là độc lập tuyến tính trên K nếu chúng thỏa mãn các điều kiện sau:*
(1) *mọi phần tử của E đều giao hoán với mọi phần tử của F;*
(2) *đồng cấu chính tắc của $E \otimes_K F$ vào G là đơn ánh.*

#### Mệnh đề 7 {#alg-iii-s4-prop-7 .statement}

*Cho G là một đại số trên một trường giao hoán K và E, F là hai đại số con của G sao cho mọi phần tử của E đều giao hoán với mọi phần tử của F. Để E và F độc lập tuyến tính trên K, điều kiện cần và đủ là tồn tại một cơ sở của E trên K là một tập con tự do của G đối với cấu trúc F-môđun phải trên G. Khi đó:*
(i) *đồng cấu chính tắc $h : E \otimes_K F \to G$ là một đẳng cấu từ $E \otimes_K F$ lên đại số con của G sinh bởi $E \cup F$;*
(ii) $E \cap F = K;$
(iii) *mọi tập con tự do của E (tương ứng, F) trên K là một tập con tự do của G với cấu trúc F-môđun phải hoặc trái của nó (tương ứng, E-môđun).*

Điều kiện của mệnh đề hiển nhiên là cần thiết, vì mọi cơ sở của E trên K đều là một cơ sở của $E \otimes_K F$ với cấu trúc F-môđun phải của nó (II, § 3, no. 7, Hệ quả 1 của Mệnh đề 7). Để thấy rằng điều kiện là đủ, chú ý rằng ảnh H của $E \otimes_K F$ dưới h là tập các tổng $\sum_i x_i y_i = \sum_i y_i x_i$ trong G, với $x_i \in E$ và $y_i \in F$; do đó nếu $(a_\lambda)$ là một cơ sở của E trên K thì H cũng là môđun con của F-môđun G (phải hoặc trái) sinh bởi $(a_\lambda)$. Vậy điều kiện của mệnh đề có nghĩa là tồn tại một cơ sở $(a_\lambda)$ của E đồng thời cũng là một cơ sở của F-môđun H; suy ra h là đơn ánh. Mệnh đề (iii) suy ra từ việc mọi tập con tự do của E đều được chứa trong một cơ sở của E (II, § 7, no. 1, Định lý 2).

#### Hệ quả 1 {#alg-iii-s4-prop-7-cor-1 .statement}

*Để đồng cấu chính tắc của $E \otimes_K F$ vào G là song ánh, điều kiện cần và đủ là tồn tại một cơ sở của E trên K đồng thời là một cơ sở của F-môđun G (phải hoặc trái).*

#### Hệ quả 2 {#alg-iii-s4-prop-7-cor-2 .statement}

*Cho E, F là hai đại số con của G, có hạng hữu hạn trên K và sao cho mọi phần tử của E đều giao hoán với mọi phần tử của F. Để E và F độc lập tuyến tính trên K, điều kiện cần và đủ là đại số con H của G sinh bởi $E \cup F$ thỏa mãn*
$$
[H : K] = [E : K] \cdot [F : K].
$$
Điều này nói rằng hạng trên K của đồng cấu chính tắc toàn ánh h : E \otimes_K F \to H bằng hạng của E \otimes_K F trên K, điều này tương đương với việc nói rằng đồng cấu này là song ánh (II, § 7, No. 4, Mệnh đề 9).

### 5. TÍCH TENXƠ CỦA MỘT HỌ VÔ HẠN CÁC ĐẠI SỐ

Cho A là một vành giao hoán và $(E_i)_{i \in I}$ là một họ tùy ý các A-đại số (có đơn vị). Với mọi tập con hữu hạn J của I, ký hiệu E_J là tích tenxơ $\bigotimes_{i \in J} E_i$ của các đại số E_i có chỉ số $i \in J$; ký hiệu $e_i$ là phần tử đơn vị của E_i và $e_J = \bigotimes_{i \in J} e_i$ là phần tử đơn vị của E_J; ký hiệu $f_{J,i}$ là đồng cấu chính tắc $E_i \to E_J$ với $i \in J$ (no. 2, Mệnh đề 5). Nếu J, J' là hai tập con hữu hạn của I sao cho $J \subset J'$, thì một đồng cấu $f_{J'J} : E_J \to E_{J'}$ được dẫn xuất một cách chính tắc (no. 2, Mệnh đề 5), bởi điều kiện $f_{J'J} \circ f_{J,i} = f_{J',i}$ với mọi $i \in J$. Hơn nữa tính duy nhất của $f_{J'J}$ suy ra rằng nếu J, J', J'' là ba tập con hữu hạn của I sao cho $J \subset J' \subset J''$, thì $f_{J''J} = f_{J''J'} \circ f_{J'J}$. Nói cách khác, $(E_J, f_{J'J})$ là một hệ trực tiếp các A-đại số mà tập chỉ số là tập có hướng phải $\mathcal{F}(I)$ của các tập con hữu hạn của I.

#### Định nghĩa 5 {#alg-iii-s4-def-5 .statement}

*Giới hạn trực tiếp E của hệ trực tiếp* $(E_J, f_{J'J})$ *được gọi là tích tenxơ của họ các A-đại số* $(E_i)_{i \in I}$.

Nếu I là hữu hạn, E được đồng nhất với $\bigotimes_{i \in I} E_i$. Theo một lạm dụng ký hiệu, E cũng được ký hiệu bởi $\bigotimes_{i \in I} E_i$ ngay cả khi I là vô hạn.

Với mọi tập con hữu hạn J của I, ký hiệu $f_J$ là đồng cấu chính tắc $\bigotimes_{i \in J} E_i \to \bigotimes_{i \in I} E_i$ (viết $f_i$ thay cho $f_{\{i\}}$); nếu e là phần tử đơn vị của $\bigotimes_{i \in I} E_i$, thì $f_J(e_J) = e$ với mọi $J \in \mathcal{F}(I)$. Ngay lập tức thấy rằng nếu mọi đại số E_i đều giao hoán, thì $\bigotimes_{i \in I} E_i$ cũng giao hoán.

#### Mệnh đề 8 {#alg-iii-s4-prop-8 .statement}

(i) *Các đồng cấu* $f_i : E_i \to E = \bigotimes_{k \in I} E_k$ *có tính chất sau: với hai chỉ số* i, j *sao cho* $i \neq j$, $f_i(x_i)$ *và* $f_j(x_j)$ *giao hoán trong* E *với mọi* $x_i \in E_i$ *và* $x_j \in E_j$; *hơn nữa,* E *được sinh bởi hợp của các đại số con* $f_i(E_i)$.

(ii) *Cho F là một đại số trên A và, với mọi* $i \in I$, *cho* $u_i : E_i \to F$ *là một đồng cấu đại số trên A sao cho, với* $i \neq j$, $u_i(x_i)$ *và* $u_j(x_j)$ *giao hoán trong* F *với mọi* $x_i \in E_i$ *và* $x_j \in E_j$. *Khi đó tồn tại một và chỉ một đồng cấu đại số trên A* $u : E \to F$ *sao cho* $u_i = u \circ f_i$ *với mọi* $i \in I$.

(i) Vì, với mọi tập con hữu hạn J của I, $f_i = f_J \circ f_{J,i}$, mệnh đề đầu tiên trong (i) suy ra từ No. 2, Mệnh đề 5, khi lấy J chứa i và j; mệnh đề thứ hai cũng suy ra từ No. 2, Mệnh đề 5, có tính đến sự kiện rằng E là hợp của các $f_J(E_J)$ khi J chạy qua $\mathcal{F}(I)$.

(ii) Với mọi tập con hữu hạn J của I, suy ra từ No. 2, Mệnh đề 5 rằng tồn tại một đồng cấu duy nhất $u_J : E_J \to F$ sao cho $u_J \circ f_{J,i} = u_i$ với mọi $i \in J$; ngay lập tức suy ra từ tính duy nhất này rằng, với $J \subset J'$, $u_J = u_{J'} \circ f_{J'J}$; nói cách khác, các $u_J$ tạo thành một *hệ trực tiếp* các đồng cấu. Đặt $u = \lim \to u_J : E \to F$; khi đó theo định nghĩa ta có $u_J = u \circ f_J$ với mọi tập con hữu hạn $J$ của $I$ và đặc biệt $u_i = u \circ f_i$ với mọi $i \in I$; tính duy nhất của $u$ suy ra từ các hệ thức này và từ sự kiện rằng các $f_i(E_i)$ sinh đại số $E$.

#### Hệ quả {#alg-iii-s4-n5-cor-1 .statement}

*Cho* $(E_i)_{i \in I},\ (E'_i)_{i \in I}$ *là hai họ* $A$*-đại số có cùng tập hợp chỉ số và, với mọi* $i \in I$, *cho* $u_i : E_i \to E'_i$ *là một đồng cấu đại số. Khi đó tồn tại một và chỉ một đồng cấu đại số trên* $A$ $u : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} E'_i$ *sao cho, với mọi* $i \in I$, *biểu đồ*

$$
\begin{array}{ccc}
E_i & \xrightarrow{u_i} & E'_i \\
| & & | \\
\bigotimes_{i \in I} E_i & \xrightarrow{u} & \bigotimes_{i \in I} E'_i
\end{array}
$$

*là giao hoán*, $f_i$ *và* $f'_i$ *ký hiệu các đồng cấu chính tắc*.

Chỉ cần áp dụng Mệnh đề 8 cho đồng cấu $f'_i \circ u_i$.

Đồng cấu $u$ được định nghĩa trong Hệ quả của Mệnh đề 8 được ký hiệu là $\bigotimes_{i \in I} u_i$. Nếu $J$ là một tập con bất kỳ của $I$, có thể áp dụng Mệnh đề 8 cho họ $(f_i)_{i \in J}$ các đồng cấu chính tắc $f_i : E_i \to \bigotimes_{i \in I} E_i = E$; từ đó dẫn xuất một đồng cấu chính tắc $E_J \to E$ cũng được ký hiệu là $f_J$ và, khi $J$ là *hữu hạn*, thì trùng với đồng cấu đã được ký hiệu như vậy ở trên.

Bây giờ cho $(x_i)_{i \in I}$ là một phần tử của $\prod_{i \in I} E_i$ sao cho họ $(x_i - e_i)_{i \in I}$ có *giá hữu hạn* $H$. Ngay lập tức thấy rằng, nếu $J$ và $J'$ là hai tập con hữu hạn của $I$ chứa $H$, thì

$$
f_J((x_i)_{i \in J}) = f_{J'}((x_i)_{i \in J'}).
$$

Giá trị chung của các $f_J((x_i)_{i \in J})$ đối với các tập con hữu hạn $J \supset H$ của $I$ được ký hiệu là $\bigotimes_{i \in I} x_i$.

#### Mệnh đề 9 {#alg-iii-s4-prop-9 .statement}

*Cho* $(E_i)_{i \in I}$ *là một họ các* $A$*-đại số và với mỗi* $i \in I$ *cho* $B_i$ *là một cơ sở của* $E_i$ *sao cho phần tử đơn vị* $e_i$ *thuộc về* $B_i$. *Gọi* $B$ *là tập hợp các phần tử có dạng* $\bigotimes_{i \in I} x_i$, *trong đó* $(x_i)$ *chạy qua tập hợp các phần tử của* $\prod_{i \in I} B_i$ *sao cho họ* $(x_i - e_i)$ *có giá hữu hạn*. *Khi đó* $B$ *là một cơ sở của đại số* $\bigotimes_{i \in I} E_i$ *và cơ sở này chứa phần tử đơn vị* $e$.

Với mọi tập con hữu hạn $J$ của $I$, gọi $B_J$ là cơ sở của $E_J = \bigotimes_{i \in J} E_i$, là tích tenxơ của các cơ sở $B_i$ với $i \in J$ (II, § 3, no. 9). Ngay từ các định nghĩa suy ra rằng $B$ là hợp của các $f_J(B_J)$ khi $J$ chạy qua $\mathcal{F}(I)$ và rằng $f_{J',J}(B_J) \subset B_{J'}$ khi $J \subset J'$; do đó $(B_J)$ là một hệ trực tiếp các tập con của các $E_J$ và $B = \lim \rightarrow B_J$; kết luận khi đó suy ra từ II, § 6, no. 2, Hệ quả của Mệnh đề 5.

Cơ sở $B$ cũng được gọi là *tích tenxơ* của các cơ sở $B_i$ với $i \in I$; khi các điều kiện của Mệnh đề 9 được thỏa mãn, các đồng cấu chính tắc $f_J : E_J \to E = \bigotimes_{i \in I} E_i$ là *đơn ánh* với mọi tập con $J$ của $I$, vì nếu $B_J$ là cơ sở của $E_J$, là tích tenxơ của các $B_i$ với $i \in J$, thì kiểm tra ngay lập tức được rằng hạn chế của $f_J$ lên $B_J$ là đơn ánh và ánh xạ $B_J$ lên một tập con của $B$.

### 6. CÁC BỔ ĐỀ GIAO HOÁN

#### Bổ đề 1 {#alg-iii-s4-lem-1 .statement}

*Cho $A$ là một vành giao hoán, $E$ là một $A$-đại số, $(x_i)_{1 \leq i \leq n}$ là một dãy hữu hạn các phần tử của $E$, $(\lambda_i)_{1 \leq i \leq n}$ là một dãy hữu hạn các phần tử của $A$ và $y$ là một phần tử của $E$; giả sử rằng*
$$
x_i y = \lambda_i y x_i \quad \text{với } 1 \leq i \leq n.
$$
*Khi đó*
$$
(x_1 x_2 \ldots x_n) y = (\lambda_1 \lambda_2 \ldots \lambda_n) y (x_1 x_2 \ldots x_n).
$$

Bổ đề là tầm thường với $n = 1$, ta lập luận bằng quy nạp theo $n \geq 2$. Bây giờ
$$
(x_1 x_2 \ldots x_n) y = (x_1 \ldots x_{n-1})(x_n y)
= (x_1 \ldots x_{n-1})(\lambda_n y x_n) = \lambda_n ((x_1 \ldots x_{n-1}) y) x_n,
$$
mà, theo giả thiết quy nạp, bằng
$$
\lambda_n (\lambda_1 \ldots \lambda_{n-1}) y (x_1 \ldots x_{n-1}) x_n = (\lambda_1 \ldots \lambda_{n-1} \lambda_n) y (x_1 \ldots x_{n-1} x_n),
$$
do đó suy ra bổ đề.

#### Bổ đề 2 {#alg-iii-s4-lem-2 .statement}

*Cho $A$ là một vành giao hoán, $E$ là một $A$-đại số và $(x_i)_{1 \leq i \leq n}$ và $(y_i)_{1 \leq i \leq n}$ là hai dãy hữu hạn gồm $n$ phần tử của $E$; giả sử rằng với $1 \leq j \leq i \leq n$,*
$$
x_i y_j = \lambda_{ij} y_j x_i \quad \text{với } \lambda_{ij} \in A.
$$
*Khi đó*
$$
(x_1 x_2 \ldots x_n)(y_1 y_2 \ldots y_n) = \left( \prod_{i > j} \lambda_{ij} \right) (x_1 y_1)(x_2 y_2) \ldots (x_n y_n).
$$

Bổ đề là tầm thường với $n = 1$, ta lại lập luận bằng quy nạp theo $n$ với $n \geq 2$. Theo bổ đề 1,
$$
(x_1 \ldots x_n)(y_1 \ldots y_n) = x_1 (x_2 \ldots x_n) y_1 (y_2 \ldots y_n)
= \left( \prod_{i > 1} \lambda_{i1} \right) (x_1 y_1)(x_2 \ldots x_n)(y_2 \ldots y_n)
$$
và khi đó chỉ cần áp dụng giả thiết quy nạp để thu được (16).

Với mọi họ $\lambda = (\lambda_{ij})$ gồm các phần tử của $\mathbf{A}$, với $1 \leq j < i \leq n$, và với mọi phép hoán vị $\sigma \in \mathfrak{S}_n$, ta viết

$$
\varepsilon_\sigma(\lambda) = \prod_{i > j,\ \sigma^{-1}(i) < \sigma^{-1}(j)} \lambda_{ij} = \prod_{i < j,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)}.
$$

Chú ý rằng, khi $\mathbf{A} = \mathbf{Z}$ và $\lambda_{ij} = -1$ với mọi cặp có thứ tự $(i, j)$ sao cho $1 \leq j < i \leq n$, $\varepsilon_\sigma(\lambda)$ chỉ đơn giản là dấu $\varepsilon_\sigma$ của phép hoán vị $\sigma$ (I, § 5, no. 7).

#### Bổ đề 3 {#alg-iii-s4-lem-3 .statement}

*Cho $\mathbf{A}$ là một vành giao hoán, $\mathbf{E}$ là một $\mathbf{A}$-đại số, $(x_i)_{1 \leq i \leq n}$ là một dãy hữu hạn các phần tử của $\mathbf{E}$ và giả sử rằng, với mọi cặp có thứ tự $(i, j)$ của các số nguyên sao cho $1 \leq j < i \leq n$,*

$$
x_i x_j = \lambda_{ij} x_j x_i \quad \text{với } \lambda_{ij} \in \mathbf{A}.
$$

*Khi đó, với mọi phép hoán vị $\sigma \in \mathfrak{S}_n$,*

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \varepsilon_\sigma(\lambda) x_1 x_2 \cdots x_n.
$$

Bổ đề là tầm thường với $n = 1$ và $n = 2$; ta tiến hành bằng quy nạp theo $n$ với $n \geq 3$. Nếu $\sigma(n) = n$, hệ thức (19) suy ra từ giả thiết quy nạp. Vậy giả sử rằng $\sigma(n) = k, k \neq n$, và gọi $\tau$ là phép hoán vị của $\{1, n\}$ được xác định bởi

$$
\begin{cases}
\tau(i) = i & \text{với } i < k \\
\tau(i) = i + 1 & \text{với } k \leq i < n \\
\tau(n) = k.
\end{cases}
$$

Đặt $\pi = \tau^{-1} \circ \sigma$; phép hoán vị $\pi$ để cố định $n$; khi đó $\sigma = \tau \circ \pi$ và do đó, viết $y_i = x_{\tau(i)},\ y_{\pi(i)} = x_{\sigma(i)}$. Nếu $i \neq n$ và $j \neq n$, các hệ thức $\pi(i) > \pi(j)$ và $\sigma(i) > \sigma(j)$ là tương đương (vì $\tau$ là một ánh xạ tăng ngặt của $\{1, n-1\}$ vào $\{1, n\}$). Với $i \neq n, j \neq n$ và $\sigma(i) > \sigma(j)$,

$$
y_{\pi(i)} y_{\pi(j)} = x_{\sigma(i)} x_{\sigma(j)} = \lambda_{\sigma(i),\ \sigma(j)} x_{\sigma(j)} x_{\sigma(i)} = \lambda_{\sigma(i),\ \sigma(j)} y_{\pi(j)} y_{\pi(i)}
$$

do đó, theo giả thiết quy nạp (dùng sự kiện rằng $\pi(n) = n$):

$$
y_{\pi(1)} y_{\pi(2)} \cdots y_{\pi(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) y_1 y_2 \cdots y_n
$$

nghĩa là

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) x_{\tau(1)} \cdots x_{\tau(n)}.
$$

Bây giờ

$$
x_{\tau(1)} \cdots x_{\tau(n)} = x_1 \cdots x_{k-1} x_{k+1} \cdots x_n x_k
$$

và biểu thức này, theo Bổ đề 1, bằng

$$
\left( \prod_{j > k} \lambda_{jk} \right) x_1 \cdots x_n = \left( \prod_{\sigma(i) > \sigma(n)} \lambda_{\sigma(i),\ \sigma(n)} \right) x_1 \cdots x_n.
$$

Sau cùng, (20) và (21) cho

$$
x_{\sigma(1)} \cdots x_{\sigma(n)} = \alpha \cdot x_1 \cdots x_n
$$

với

$$
\alpha = \left( \prod_{i < j < n, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} \right) \cdot \left( \prod_{i < n, \sigma(i) > \sigma(n)} \lambda_{\sigma(i), \sigma(n)} \right)
$$
$$
= \prod_{i < j, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} = \varepsilon_\sigma(\lambda)
$$

điều này hoàn tất chứng minh Bổ đề 3.

### 7. TÍCH TENXƠ CỦA CÁC ĐẠI SỐ PHÂN BẬC ĐỐI VỚI CÁC NHÂN TỬ GIAO HOÁN

#### Định nghĩa 6 {#alg-iii-s4-def-6 .statement}

*Cho* $(\Delta_i)_{i \in I}$ *là một họ hữu hạn các monoid giao hoán viết theo phép cộng. Một hệ các nhân tử giao hoán trên các* $\Delta_i$ *với giá trị trong một vành giao hoán* $\mathbf{A}$ *là một hệ các ánh xạ* $\varepsilon_{ij}: \Delta_i \times \Delta_j \to \mathbf{A}$, *trong đó* $i \in I$, $j \in I$, $i \neq j$ *thỏa mãn các điều kiện sau*:

(22)
$$
\varepsilon_{ij}(\alpha_i + \alpha'_i, \beta_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha'_i, \beta_j)
$$
(23)
$$
\varepsilon_{ij}(\alpha_i, \beta_j + \beta'_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha_i, \beta'_j)
$$
(24)
$$
\varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ji}(\beta_j, \alpha_i) = 1,
$$

*đối với mọi* $\alpha_i, \alpha'_i$ *trong* $\Delta_i$, $\beta_j, \beta'_j$ *trong* $\Delta_j$.

Nếu I được cho một thứ tự toàn phần và các $\Delta_i$ là các nhóm, thì một hệ các nhân tử giao hoán được xác định trên các $\Delta_i$ bằng cách lấy, với mọi cặp có thứ tự $(i, j)$ sao cho $i < j$, một ánh xạ $\mathbf{Z}$-*song tuyến tính* tùy ý từ $\Delta_i \times \Delta_j$ vào $\mathbf{Z}$-môđun (*nhân*) $\mathbf{A}^*$ gồm các phần tử *khả nghịch* của vành $\mathbf{A}$ rồi viết

$$
\varepsilon_{ji}(\beta_j, \alpha_i) = (\varepsilon_{ij}(\alpha_i, \beta_j))^{-1}
$$

với $i < j$.

Chú ý rằng, vì các $\varepsilon_{ij}(\alpha_i, \beta_j)$ là khả nghịch,

$$
\varepsilon_{ij}(0, \beta_j) = \varepsilon_{ij}(\alpha_i, 0) = 1,
$$

theo (22) và (23).

#### Ví dụ {#alg-iii-s4-n7-exa-1 .statement}

(1) Hệ các nhân tử giao hoán *tầm thường* là hệ gồm các $\varepsilon_{ij}$ sao cho $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ với mọi $i, j$, $\alpha_i \in \Delta_i$, $\beta_j \in \Delta_j$.

(2) Nếu lấy $\mathbf{A} = \mathbf{Z}$ và $\Delta_i = \mathbf{Z}$ với mọi $i \in I$, thì thu được một hệ các nhân tử giao hoán bằng cách lấy $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$. Chú ý rằng số này chỉ phụ thuộc vào tính chẵn lẻ của $\alpha_i$ và $\beta_j$, và do đó các $\varepsilon_{ij}$ có thể được coi là các nhân tử giao hoán khi một số $\Delta_i$ bằng $\mathbf{Z}/2\mathbf{Z}$ và các $\Delta_i$ khác bằng $\mathbf{Z}$.

Hai ví dụ này là những trường hợp thường gặp nhất trong các ứng dụng.

#### Mệnh đề 10 {#alg-iii-s4-prop-10 .statement}

Cho $\mathbf{A}$ là một vành giao hoán và $(\Delta_i)_{i \in I}$ là một họ hữu hạn các monoid giao hoán viết theo phép cộng; với mỗi $i \in I$, cho $E_i$ là một $\mathbf{A}$-đại số phân bậc kiểu $\Delta_i$. Sau hết, cho $(\varepsilon_{ij})$ là một hệ các nhân tử giao hoán trên các $\Delta_i$ với giá trị trong $\mathbf{A}$. Khi đó tồn tại một $\mathbf{A}$-đại số phân bậc $E$ kiểu $\Delta = \prod_{i \in I} \Delta_i$ và, với mỗi $i \in I$, một đồng cấu đại số $h_i : E_i \to E$, có các tính chất sau:

(i) *Nếu $\phi_i : \Delta_i \to \Delta$ là đồng cấu chính tắc, thì $h_i$ là một đồng cấu phân bậc* (II, § 11, no. 2), nói cách khác, $h_i(E_i^{\alpha_i}) \subset E^{\phi_i(\alpha_i)}$, trong đó $(E_i^{\alpha_i})$ và $(E^{\alpha})$ chỉ các phân bậc tương ứng trên $E_i$ và $E$.

(ii) *Nếu $i \neq j$ và $x_i$ (resp. $x_j$) là một phần tử thuần nhất của $E_i$ (resp. $E_j$) bậc $\alpha_i \in \Delta_i$ (resp. $\beta_j \in \Delta_j$), thì*

$$
h_i(x_i) h_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) h_j(x_j) h_i(x_i).
$$

(iii) *Với mọi $\mathbf{A}$-đại số $F$ và mọi hệ các đồng cấu $f_i : E_i \to F$ thỏa mãn các điều kiện*

$$
f_i(x_i) f_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) f_j(x_j) f_i(x_i),
$$

*trong đó $i, j, x_i, x_j, \alpha_i, \beta_j$ như trong (ii), thì tồn tại một và chỉ một đồng cấu đại số $f : E \to F$ sao cho $f_i = f \circ h_i$ với mọi $i \in I$. Hơn nữa, $\mathbf{A}$-môđun nền của $E$ là tích tenxơ $\bigotimes_{i \in I} E_i$.*

Xét $\mathbf{A}\text{-module}$ $E = \bigotimes_{i \in I} E_i$; nó được đồng nhất với tổng trực tiếp của các môđun con $E^{\alpha}$, trong đó, với mỗi $\alpha = (\alpha_i) \in \Delta$, ta viết $E^{\alpha} = \bigotimes_{i \in I} E_i^{\alpha_i}$; do đó các $E^{\alpha}$ tạo thành một phân bậc kiểu $\Delta$ trên $\mathbf{A}$-môđun $E$. Ta sẽ định nghĩa trên $E$ một cấu trúc *đại số $\mathbf{A}$ phân bậc* kiểu $\Delta$. Để làm điều đó, cho $I$ một thứ tự toàn phần; với mọi cặp có thứ tự các phần tử $\alpha = (\alpha_i), \beta = (\beta_i)$ của $\Delta$, trước hết ta phải định nghĩa một ánh xạ $\mathbf{A}$-song tuyến tính từ $E^{\alpha} \times E^{\beta}$ vào $E^{\alpha + \beta}$, hay tương đương một ánh xạ $\mathbf{A}$-tuyến tính $m_{\alpha \beta}$ từ $E^{\alpha} \otimes_{\mathbf{A}} E^{\beta}$ vào $E^{\alpha + \beta}$. Ta sẽ định nghĩa $m_{\alpha \beta}$ bởi điều kiện

$$
m_{\alpha \beta} \left( \left( \bigotimes_{i \in I} x_i \right) \otimes \left( \bigotimes_{i \in I} y_i \right) \right) = \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)
$$

với $x_i \in E_i^{\alpha_i}, y_i \in E_i^{\alpha_i}$, trong đó

$$
\varepsilon(\alpha, \beta) = \prod_{i > j} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

Vế phải của (27) hiển nhiên thuộc $E^{\alpha + \beta}$ và ánh xạ $(x_1, \ldots, x_n, y_1, \ldots, y_n) \mapsto \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)$ là $\mathbf{A}$-đa tuyến tính theo tích của các $E_i^{\alpha_i}$ và các $E_i^{\beta_i}$ ($1 \leq i \leq n$). Sau đó phải chứng minh rằng phép nhân được định nghĩa như vậy trên E là kết hợp; bây giờ, nếu $\gamma = (\gamma_i)$ là một phần tử thứ ba của $\Delta$ và $z_i \in E_i^{\gamma_i'}$ với $1 \leq i \leq n$, thì

$$
\left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) \left( \bigotimes_i z_i \right) = \varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) \bigotimes_i (x_i y_i z_i)
$$

$$
\left( \bigotimes_i x_i \right) \left( \left( \bigotimes_i y_i \right) \left( \bigotimes_i z_i \right) \right) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma) \bigotimes_i (x_i y_i z_i)
$$

và điều đó quy về việc kiểm tra đồng nhất thức

$$
\varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma).
$$

Nhưng điều sau này suy ra ngay lập tức từ các quan hệ

$$
\varepsilon(\alpha + \beta, \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\beta, \gamma)
$$
$$
\varepsilon(\alpha, \beta + \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\alpha, \gamma)
$$

mà bản thân chúng là những hệ quả ngay lập tức của định nghĩa (28) và của (22) và (23).

Nếu, với mọi $i \in I$, $e_i$ ký hiệu phần tử đơn vị của $E_i$, ta biết rằng $e_i$ là thuần nhất bậc 0 (§ 3, no. 1), do đó $e = \bigotimes_{i \in I} e_i$ là thuần nhất bậc 0 và suy ra từ (27), (28) và các quan hệ

$$
\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1
$$

rằng $e$ là phần tử đơn vị của $E$, điều này hoàn tất việc định nghĩa trên $E$ cấu trúc đại số A phân bậc mong muốn. Sau đó đặt $h_i(x_i) = x_i \otimes \bigotimes_{j \neq i} e_j$; để kiểm tra rằng $h_i(x_i x_i') = h_i(x_i) h_i(x_i')$ với $x_i, x_i'$ trong $E_i$, có thể chỉ cần xét trường hợp $x_i$ và $x_i'$ là thuần nhất và khi đó quan hệ này suy ra ngay lập tức từ (27) và các quan hệ $\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1$; các quan hệ ấy và (24) cũng chứng minh rằng các $h_i$ thỏa mãn các điều kiện (i) và (ii) của mệnh đề và rằng

$$
\bigotimes_{i \in I} x_i = \prod_{i \in I} h_i(x_i)
$$

trong đó vế phải là tích của dãy có thứ tự $(h_i(x_i))_{i \in I}$ trong E với thứ tự toàn phần đã cho trên I (I, § 1, no. 2) (chỉ cần lập luận bằng quy nạp theo số các $x_i$ (được giả thiết là thuần nhất) khác với các $e_i$).

Còn phải chứng minh điều kiện (iii); chú ý rằng ánh xạ

$$
(x_i)_{i \in I} \mapsto \prod_{i \in I} f_i(x_i),
$$

trong đó vế phải là tích của dãy có thứ tự $(f_i(x_i))_{i \in I}$ với thứ tự toàn phần đã cho trên $I$, là A-đa tuyến tính. Khi đó tồn tại một và chỉ một ánh xạ A-tuyến tính $f : E \to F$ sao cho

$$
f\left( \bigotimes_{i \in I} x_i \right) = \prod_{i \in I} f_i(x_i).
$$

Rõ ràng $f(e)$ là phần tử đơn vị của $F$ và $f \circ h_i = f_i$; để kiểm tra rằng $f$ là một đồng cấu đại số, nói cách khác rằng $f(x)f(y) = f(xy)$ với $x, y$ trong $E$, do tính tuyến tính, có thể chỉ cần xét trường hợp $x = \bigotimes_{i \in I} x_i$ và $y = \bigotimes_{i \in I} y_i$, trong đó $x_i$ (tương ứng $y_i$) thuần nhất bậc $\alpha_i$ (tương ứng $\beta_i$) với mọi $i \in I$. Khi đó quan hệ phải kiểm tra, theo (27), được quy về

$$
\left( \prod_{i \in I} f_i(x_i) \right) \left( \prod_{i \in I} f_i(y_i) \right) = \varepsilon(\alpha, \beta) \prod_{i \in I} (f_i(x_i) f_i(y_i)).
$$

Nhưng, có tính đến các quan hệ (26), điều này là một hệ quả của Bổ đề 2 của no. 6.

Rõ ràng đại số $E$ và ánh xạ chính tắc $\psi : \bigotimes_{i \in I} E_i \to E$ tạo thành một nghiệm của *bài toán ánh xạ phổ quát* (*Set Theory*, IV, § 3, no. 1), trong đó $\Sigma$ là loài cấu trúc đại số trên A và các $\alpha$-ánh xạ $\prod_i f_i$ từ $\prod_i E_i$ đến một đại số trên A, thỏa mãn các điều kiện (26).

Với một thứ tự toàn phần cố định trên $I$, đại số phân bậc $E$ được định nghĩa trong chứng minh của Mệnh đề 10 sẽ được gọi là một *tích tenxơ $\varepsilon$ phân bậc kiểu* $\Delta$ của họ $(E_i)_{i \in I}$ các đại số phân bậc kiểu $\Delta_i$ và sẽ được ký hiệu bởi $^{\varepsilon} \bigotimes_{i \in I} E_i$ (nếu không thể có nhầm lẫn về thứ tự trên $I$); tương tự, đồng cấu $f : E \to F$ được định nghĩa trong chứng minh của Mệnh đề 10 sẽ được ký hiệu bởi $^{\varepsilon} \bigotimes_{i \in I} f_i$. Các đồng cấu $h_i$ được gọi là *chính tắc*. Ta cũng viết $^{\varepsilon} G^{\otimes n}$ khi $I = \{1, n\}$ và mọi $E_i$ đều bằng cùng một đại số $G$.

#### Nhận xét {#alg-iii-s4-n7-rem-1 .statement}

(1) Ta thu được tích tenxơ các đại số được định nghĩa ở no. 1 (hơn nữa với phân bậc là tích tenxơ của các phân bậc của các thừa số của nó) bằng cách lấy $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ với mọi $i, j, \alpha_i$ và $\beta_j$.

(2) Giả sử rằng mọi $\Delta_i$ đều bằng $\mathbf{Z}$ và đặt $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$; khi đó tích tenxơ $\varepsilon$ $^{\varepsilon} \bigotimes_{i \in I} E_i$ tương ứng với hệ các yếu tố giao hoán này được gọi là tích tenxơ *lệch* của các đại số phân bậc $E_i$ kiểu $\mathbf{Z}$ và được ký hiệu bởi $^{\varepsilon} \bigotimes_{i \in I} E_i$ (hoặc $E \ ^{\varepsilon} \otimes_A F$ đối với hai đại số, hoặc $^{\varepsilon} G^{\otimes n}$ thay cho $^{\varepsilon} G^{\otimes n}$).

#### Hệ quả 1 {#alg-iii-s4-prop-10-cor-1 .statement}

Theo ký hiệu của Mệnh đề 10, giả sử thêm rằng F là một đại số trên A phân bậc kiểu $\Delta$ và mỗi $f_i$ là một đồng cấu đại số phân bậc đối với $\phi_i : \Delta_i \to \Delta$; khi đó $f = \varepsilon \bigotimes_i f_i$ là một đồng cấu đại số phân bậc.

Điều này suy ra ngay lập tức từ định nghĩa của $f$ và từ sự kiện là
$$
\sum_{i \in I} \phi_i(\alpha_i) = (\alpha_i)
$$
theo định nghĩa của các $\phi_i$.

Do đó ta thấy rằng $(E, \psi)$ cũng là một nghiệm của một bài toán ánh xạ phổ quát khác, trong đó lần này $\Sigma$ là loài các cấu trúc *đại số trên A phân bậc* *kiểu* $\Delta$, các cấu xạ là các đồng cấu đại số phân bậc kiểu $\Delta$ và các ánh xạ $\alpha$ là các ánh xạ $\prod_i f_i$, trong đó, ngoài các điều kiện (26), còn giả sử rằng $f_i$ là một đồng cấu đại số phân bậc đối với $\phi_i$.

#### Hệ quả 2 {#alg-iii-s4-prop-10-cor-2 .statement}

*Cho* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *là hai họ hữu hạn các* A*-đại số, với* $E_i$ *và* $F_i$ *đều phân bậc kiểu* $\Delta_i$ *với mọi* $i \in I$. *Với mỗi* $i \in I$, *cho* $g_i : E_i \to F_i$ *là một đồng cấu đại số phân bậc kiểu* $\Delta_i$. *Khi đó, nếu* $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i$ *và* $h'_i : F_i \to \varepsilon \bigotimes_{i \in I} F_i$ *là các đồng cấu chính tắc, thì tồn tại một và chỉ một đồng cấu các* A*-đại số phân bậc kiểu* $\Delta$, $g : \varepsilon \bigotimes_{i \in I} E_i \to \varepsilon \bigotimes_{i \in I} F_i$ *sao cho* $g \circ h_i = h'_i \circ g_i$ *với mọi* $i \in I$. *Ngoài ra, nếu mỗi* $g_i$ *là song ánh, thì* $g$ *cũng vậy*.

Chỉ cần áp dụng Hệ quả 1 cho $f_i = h'_i \circ g_i$, lưu ý rằng khi đó các điều kiện (26) suy ra từ các hệ thức (25) áp dụng cho các $h'_i$.

Đồng cấu được định nghĩa trong Hệ quả 2 cũng được ký hiệu bởi $\varepsilon \bigotimes_i g_i$ (nếu không thể xảy ra nhầm lẫn); nếu, với mỗi $i \in I$, $G_i$ là một A-đại số phân bậc thứ ba kiểu $\Delta_i$ và $g'_i : F_i \to G_i$ là một đồng cấu đại số phân bậc, thì
$$
\left( \varepsilon \bigotimes_i g'_i \right) \circ \left( \varepsilon \bigotimes_i g_i \right) = \varepsilon \bigotimes_i (g'_i \circ g_i),
$$
như suy ra ngay lập tức từ (30).

Trong trường hợp tích tenxơ *xiên* của các đại số phân bậc kiểu $\mathbf{Z}$, ta viết $\varepsilon \bigotimes_i f_i$ thay cho $\varepsilon \bigotimes_i f_i$ đối với các đồng cấu $f_i : E_i \to F_i$ của các đại số phân bậc kiểu $\mathbf{Z}$; khi $I = \{1, 2\}$, đồng cấu này cũng được ký hiệu bởi $f_1 \varepsilon \otimes f_2$; khi $I = \{1, n\}$ và mọi $E_i$ (tương ứng mọi $F_i$) đều bằng nhau và mọi $f_i$ đều bằng cùng một đồng cấu $f$, ta viết $\varepsilon f^{\otimes n}$.

#### Nhận xét {#alg-iii-s4-n7-rem-2 .statement}

Trong chứng minh của Mệnh đề 10, một thứ tự toàn phần trên $I$ đã được dùng để định nghĩa một cấu trúc *đại số* trên tích tenxơ $\bigotimes_{i \in I} E_i$ của các A-môđun

E_i. Nếu thứ tự trên I bị thay đổi, thì một cấu trúc nhân khác xuất hiện trên $\bigotimes_{i \in I} E_i$, nhưng đại số mới nhận được như vậy là *đẳng cấu* một cách chính tắc với đại số ở trên, vì cả hai đều là nghiệm của cùng một bài toán ánh xạ phổ quát. Chẳng hạn, khi $I = \{1, 2\}$, đẳng cấu chính tắc của đại số $E_1 \overset{\varepsilon}{\otimes}_A E_2$ lên đại số $E_2 \overset{\varepsilon}{\otimes}_A E_1$ biến $x_1 \otimes x_2$ thành $\varepsilon_{2,1}(\alpha, \beta)x_2 \otimes x_1$, trong đó $x_1$ là thuần nhất bậc $\alpha$ và $x_2$ thuần nhất bậc $\beta$.

Cho J là một tập con của I và, với mỗi $i \in J$, xét đồng cấu chính tắc $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i = E$. Nhờ các hệ thức (25), một đồng cấu chính tắc $h : E' = \varepsilon \bigotimes_{i \in J} E_i \to E$ được dẫn xuất một cách chính tắc (theo Mệnh đề 10) từ các đồng cấu này, sao cho, với mọi $i \in J$, $h'_i = h \circ h_i$, trong đó $h'_i$ là đồng cấu chính tắc $E_i \to E'$. Lấy trên J thứ tự toàn phần cảm sinh bởi thứ tự đã chọn trên I, ta được

$$
h\left( \bigotimes_{i \in J} x_i \right) = \prod_{i \in I} h_i(x_i) = \bigotimes_{i \in I} x'_i
$$

trong đó số hạng ở giữa là tích của *dãy có thứ tự* $(h_i(x_i))_{i \in J}$ và trong số hạng bên phải, $x'_i = x_i$ với $i \in J$, $x'_i = e_i$ với $i \notin J$.

#### Mệnh đề 11 {#alg-iii-s4-prop-11 .statement}

("tính kết hợp" của tenxơ $\varepsilon$-tích). *Theo ký hiệu của Mệnh đề 10, giả sử* $(J_\lambda)_{\lambda \in L}$ *là một phân hoạch của I và đặt* $\Delta'_\lambda = \prod_{i \in J_\lambda} \Delta_i$ *với mọi* $\lambda \in L$. *Giả sử* $E'_\lambda$ *là một tenxơ $\varepsilon$-tích phân bậc kiểu* $\Delta'_\lambda$ *của họ* $(E_i)_{i \in J_\lambda}$ *ứng với một thứ tự toàn phần nào đó được chọn trên* $J_\lambda$. *Mặt khác, với* $\lambda, \mu$ *trong* $L$ *và* $\lambda \neq \mu$, *ta đặt, với* $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$, $\beta'_\mu = (\beta_j)_{j \in J_\mu}$,

$$
\varepsilon'_{\lambda \mu}(\alpha'_\lambda, \beta'_\mu) = \prod_{i \in J_\lambda, j \in J_\mu} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

*Khi đó* $(\varepsilon'_{\lambda \mu})$ *là một hệ các nhân tử giao hoán trên các* $\Delta'_\lambda$ *nhận giá trị trong* $A$ *và tồn tại duy nhất một đồng cấu các đại số phân bậc kiểu* $\Delta$, $v : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$, *sao cho*

$$
v\left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*với mọi* $(x_i) \in \prod_{i \in I} E_i$, *miễn là trên I lấy thứ tự toàn phần cảm sinh trên mỗi* $J_\lambda$ *đúng bằng thứ tự toàn phần đã chọn, và sao cho, với* $\lambda < \mu$ *trong* $L$, $i \in J_\lambda$ *và* $j \in J_\mu$, $i < j$.

Việc các $\varepsilon'_{\lambda \mu}$ tạo thành một hệ các nhân tử giao hoán là tầm thường. Cho $h_{i,\lambda} : E_i \to E'_\lambda$, $h'_\lambda : E'_\lambda \to \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$ *là các đồng cấu chính tắc* (với $\lambda \in L$, $i \in J_\lambda$) *và viết* $h''_i = h'_\lambda \circ h_{i,\lambda}$; *khi đó, do tính duy nhất của* nghiệm của một bài toán ánh xạ phổ quát, chỉ cần chứng minh rằng $\varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$ và các $h''_i$ thỏa mãn các điều kiện của Mệnh đề 10. Bây giờ, với mọi $\lambda \in L$, cho $f'_\lambda : E'_\lambda \to F$ là đồng cấu đại số duy nhất sao cho $f'_\lambda \circ h_{i,\lambda} = f_i$ với mọi $i \in J_\lambda$. Ta chứng minh rằng, với $\lambda \neq \mu$, $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}, \beta'_\mu = (\beta_j)_{j \in J_\mu}$,

$$
f'_\lambda(x'_\lambda)f'_\mu(x'_\mu) = \varepsilon'_{\lambda\mu}(\alpha'_\lambda, \beta'_\mu)f'_\mu(x'_\mu)f'_\lambda(x'_\lambda)
$$

với $x'_\lambda \in E'_\lambda$ (resp. $x'_\mu \in E'_\mu$) thuần nhất bậc $\alpha'_\lambda$ (resp. $\beta'_\mu$); do tính tuyến tính, chỉ cần kiểm tra điều đó khi $x'_\mu = \bigotimes_{i \in J_\lambda} x_i, x'_\mu = \bigotimes_{j \in J_\mu} x_j, x_i$ (resp. $x_j$) là thuần nhất bậc $\alpha_i$ (resp. $\beta_j$) trong $E_i$ (resp. $E_j$) với $i \in J_\lambda, j \in J_\mu$. Nhưng điều này suy ra từ công thức (30) dùng để định nghĩa các $f'_\lambda$ và Bổ đề 3 của no. 6, có tính đến giả thiết (26) và định nghĩa (32). Do đó tồn tại một và chỉ một đồng cấu đại số $f : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to F$ sao cho $f \circ h'_\lambda = f'_\lambda$ với mọi $\lambda \in L$; do đó $f \circ h''_i = f_i$ với mọi $i \in I$ và tính duy nhất của $f$ là tầm thường.

### 8. TÍCH $\varepsilon$-TENXƠ CỦA CÁC ĐẠI SỐ PHÂN BẬC CÙNG KIỂU

Giả sử các giả thiết của no. 7, Mệnh đề 10 được thỏa mãn, và giả sử thêm rằng mọi $\Delta_i$ đều bằng *cùng một monoïde giao hoán* $\Delta_0$; khi đó ta có thể xét trên $\varepsilon$-tích tenxơ $\varepsilon \bigotimes_{i \in I} E_i$ *phân bậc toàn phần* kiểu $\Delta_0$, liên kết với phép phân bậc kiểu $\Delta = \Delta_0^I$ trên đại số này (II, § 11, no. 1); ta sẽ gọi $\varepsilon \bigotimes_{i \in I} E_i$, được trang bị phép phân bậc này, là một *$\varepsilon$-tích tenxơ phân bậc kiểu* $\Delta_0$ của họ $(E_i)_{i \in I}$ các đại số phân bậc kiểu $\Delta_0$.

Vẫn giữ ký hiệu của Mệnh đề 10 ở no. 7, giả sử rằng $F$ cũng là một *đại số trên A phân bậc kiểu* $\Delta_0$ và các $f_i$ là các *đồng cấu của các đại số phân bậc kiểu* $\Delta_0$. Khi đó $f : \varepsilon \bigotimes_{i \in I} E_i \to F$ cũng là một *đồng cấu của các đại số phân bậc kiểu* $\Delta_0$: thật vậy, từ công thức (30) (no. 7) suy ra rằng nếu $x_i$ là thuần nhất và có bậc $\alpha_i \in \Delta_0, \bigotimes_{i \in I} x_i$ và $\prod_{i \in I} f_i(x_i)$ đều thuần nhất bậc $\sum_{i \in I} \alpha_i \in \Delta_0$.

Do đó có thể nói rằng $\varepsilon \bigotimes_{i \in I} E_i$, với phân bậc toàn phần kiểu $\Delta_0$, cùng với ánh xạ chính tắc $\psi$, tạo thành một nghiệm của bài toán ánh xạ phổ quát thứ ba, trong đó $\Sigma$ là loài các *A-đại số phân bậc kiểu* $\Delta_0$, các cấu xạ là các đồng cấu của các đại số phân bậc kiểu $\Delta_0$ và các ánh xạ $\alpha$ là các ánh xạ $\prod_i f_i$, trong đó, ngoài các điều kiện (26) (của no. 7), còn giả thiết rằng mỗi $f_i$ là một đồng cấu của các đại số phân bậc kiểu $\Delta_0$.

Với mọi tập con J của I, đồng cấu chính tắc $\varepsilon \bigotimes_{i \in J} E_i \to \varepsilon \bigotimes_{i \in I} E_i$ (no. 7) thực ra là một đồng cấu của các đại số phân bậc kiểu $\Delta_0$, như suy ra ngay lập tức từ trên đây.

#### Mệnh đề 12 {#alg-iii-s4-prop-12 .statement}

("tính kết hợp" của $\varepsilon$-tích tenxơ của các đại số phân bậc cùng kiểu). *Với ký hiệu của Mệnh đề 10 của no. 7, giả sử rằng tất cả các $\Delta_i$ đều bằng cùng một monoide $\Delta_0$; gọi $(J_\lambda)_{\lambda \in L}$ là một phân hoạch của I. Với ký hiệu của Mệnh đề 11 của no. 7, giả sử rằng vế phải của công thức (32) (no. 7) chỉ phụ thuộc vào các tổng $\alpha''_\lambda = \sum_{i \in J_\lambda} \alpha_i, \beta''_\mu = \sum_{j \in J_\mu} \beta_j$, với mọi cặp có thứ tự $(\lambda, \mu)$ của các chỉ số phân biệt, mọi $\alpha'_\lambda \in \Delta'_\lambda$ và mọi $\beta'_\mu \in \Delta'_\mu$; gọi $\varepsilon''_{\lambda \mu}(\alpha''_\lambda, \beta''_\mu)$ là vế phải của (32). *Khi đó $(\varepsilon''_{\lambda \mu})$ là một hệ các nhân tử giao hoán trên họ $(\Delta''_\lambda)_{\lambda \in L}$, trong đó $\Delta''_\lambda = \Delta_0$ với mọi $\lambda \in L$. *Nếu $E''_\lambda$ là $\varepsilon$-tích tenxơ phân bậc kiểu $\Delta_0$ của họ $(E_i)_{i \in J_\lambda}$, thì tồn tại một và chỉ một đẳng cấu của các đại số phân bậc kiểu $\Delta_0$, $w : \varepsilon'' \bigotimes_{\lambda \in L} E''_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$, sao cho

$$
w \left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*với điều kiện các thứ tự toàn phần được chọn trên các $J_\lambda$ và trên I như đã mô tả trong no. 7, Mệnh đề 11.*

Theo giả thiết, với $\gamma, \delta$ trong $\Delta_0$, $\varepsilon''_{\lambda \mu}(\gamma, \delta) = \varepsilon_{i_0 j_0}(\gamma, \delta)$ với một số $i_0 \in J_\lambda$ và một số $j_0 \in J_\mu$, như thấy được khi xét các phần tử $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$ và $\beta'_\mu = (\beta_j)_{j \in J_\mu}$ sao cho $\alpha_{i_0} = \gamma, \alpha_i = 0$ nếu $i \neq i_0$, $\beta_{j_0} = \delta, \beta_j = 0$ nếu $j \neq j_0$; từ đó suy ra ngay lập tức rằng các $\varepsilon''_{\lambda \mu}$ lập thành một hệ các nhân tử giao hoán. Phần còn lại của chứng minh khi đó tương tự như chứng minh của Mệnh đề 11 (no. 7) và được để lại cho người đọc.

Chú ý rằng các giả thiết bổ sung của Mệnh đề 12 được thỏa mãn khi $\Delta_0 = \mathbf{Z}$ và rằng $(\varepsilon_{ij})$ hoặc là hệ tầm thường các nhân tử $(\varepsilon_{ij}(\alpha_i, \beta_j)) = 1$ với mọi $i, j$, hoặc là hệ các nhân tử được xác định bởi $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$; trong trường hợp sau, vế phải của công thức (32) bằng $(-1)^\gamma$, trong đó

$$
\gamma = \sum_{i \in J_\lambda, j \in J_\mu} \alpha_i \beta_j = \left( \sum_{i \in J_\lambda} \alpha_i \right) \left( \sum_{j \in J_\mu} \beta_j \right).
$$

#### Nhận xét {#alg-iii-s4-n8-rem-1 .statement}

(1) Cho I là một tập chỉ số vô hạn và $\Delta_0$ là một monoid giao hoán; ký hiệu $(\Delta_i)_{i \in I}$ là họ sao cho $\Delta_i = \Delta_0$ với mọi $i$ và giả sử rằng với mọi cặp có thứ tự các chỉ số phân biệt $(i, j)$ của I, ta được cho một ánh xạ $\varepsilon_{ij} : \Delta_i \times \Delta_j \to A$ thỏa mãn các điều kiện (22), (23) và (24) (no. 7); hệ này cũng sẽ được gọi là một *hệ các nhân tử giao hoán trên họ* $(\Delta_i)$. Xét một họ $(E_i)_{i \in I}$ các A-đại số phân bậc kiểu $\Delta_0$; với mỗi tập con hữu hạn J của I, ký hiệu $E_J$ là một *tích tenxơ phân bậc $\varepsilon$ kiểu* $\Delta_0$ của họ con $(E_i)_{i \in J}$ (với một lựa chọn tùy ý về một thứ tự toàn phần trên J). Nếu J, J' là hai tập con hữu hạn của I sao cho $J \subset J'$, thì một đồng cấu chính tắc của các đại số phân bậc kiểu $\Delta_0$, h_{J'J}: E_J \to E_{J'}, đã được định nghĩa ở trên, và các tính chất duy nhất của các đồng cấu này cho thấy ngay lập tức rằng nếu $J \subset J' \subset J''$ là ba tập con hữu hạn của I, thì h_{J''J} = h_{J'J'} \circ h_{J'J}. Do đó có một hệ trực tiếp $(E_J, h_{J'J})$ của các đại số phân bậc kiểu $\Delta_0$ (§ 3, no. 3), mà tập chỉ số là tập có hướng phải $\mathfrak{F}(I)$ của các tập con hữu hạn của I. Đại số phân bậc kiểu $\Delta_0$, *giới hạn trực tiếp* của hệ trực tiếp này (§ 3, no. 3), được gọi là một *tích tenxơ phân bậc $\varepsilon$ kiểu* $\Delta_0$ của họ $(E_i)_{i \in I}$; nó cũng được ký hiệu bởi $\varepsilon \bigotimes_{i \in I} E_i$. Khi mọi $\Delta_i$ đều bằng $\mathbf{Z}$ và $\varepsilon_{ij}(a_i, \beta_j) = (-1)^{\alpha_i \beta_j}$, tích tenxơ $\varepsilon \bigotimes_{i \in I} E_i$ cũng được gọi là tích tenxơ *lệch* của họ $(E_i)_{i \in I}$ và được ký hiệu bởi $g \bigotimes_{i \in I} E_i$. Chúng tôi để cho người đọc công việc phát biểu và chứng minh mệnh đề tổng quát hóa Mệnh đề 10 của no. 7 cho trường hợp I là vô hạn, cũng như Mệnh đề 8 của no. 5 tổng quát hóa Mệnh đề 5 của no. 2 cho trường hợp I là vô hạn. Chú ý rằng A-môđun nền của $\varepsilon \bigotimes_{i \in I} E_i$ cũng chính là A-môđun nền của tích tenxơ (không phân bậc) của họ $(E_i)_{i \in I}$ các đại số không phân bậc được định nghĩa ở no. 5.

(2) Cho E là một A-đại số phân bậc kiểu $\Delta_0$ (trong đó $\Delta_0$ là một monoid giao hoán) và $\rho : A \to B$ là một đồng cấu vành; sự phân bậc trên $\rho^*(E)$ (II, § 11, no. 5) đồng nhất với sự phân bậc trên tích tenxơ phân bậc $B \otimes_A E$, trong đó B có phân bậc tầm thường.

### 9. CÁC ĐẠI SỐ PHẢN GIAO HOÁN VÀ CÁC ĐẠI SỐ PHẢN XỨNG

#### Định nghĩa 7 {#alg-iii-s4-def-7 .statement}

*Một A-đại số phân bậc E kiểu $\mathbf{Z}$ được gọi là phản giao hoán nếu với mọi phần tử thuần nhất khác không x, y của E*

$$
xy = (-1)^{\deg(x)\deg(y)} yx.
$$

*Đại số E được gọi là phản xứng nếu nó phản giao hoán và thêm nữa $x^2 = 0$ với mọi phần tử thuần nhất $x \in E$ có bậc lẻ.*

#### Nhận xét {#alg-iii-s4-n9-rem-1 .statement}

(1) Cho $E^+$ là đại số con phân bậc của E bằng tổng trực tiếp của các $E_{2n}$ ($n \in \mathbf{Z}$); từ Định nghĩa 7 suy ra rằng nếu E phản giao hoán thì $E^+$ là một *đại số con được chứa trong tâm của* E (và do đó giao hoán).

(2) Giả sử rằng 2 không là một ước của 0 trong E; khi đó nếu E phản giao hoán thì E phản xứng, vì với $x \in E$ thuần nhất và có bậc lẻ, $x^2 = -x^2$ theo (36), do đó $2x^2 = 0$ và $x^2 = 0$ nhờ giả thiết.

(3) Chúng tôi sẽ nghiên cứu chi tiết trong § 7 những ví dụ quan trọng của các đại số phản xứng.

#### Bổ đề 4 {#alg-iii-s4-lem-4 .statement}

*Cho E là một đại số phân bậc kiểu $\mathbf{Z}$ và S là một tập hợp các phần tử thuần nhất $\neq 0$; tập F gồm các phần tử của E mà mọi thành phần thuần nhất $x \neq 0$ đều thỏa mãn quan hệ (36) với mọi $y \in S$ là một đại số con phân bậc của E.*

Chỉ cần chú ý rằng: (1) nếu $x', x''$ là hai phần tử thuần nhất cùng bậc $p$, $y$ là một phần tử thuần nhất bậc $q$ và $x'y = (-1)^{pq}yx'$, $x''y = (-1)^{pq}yx''$, thì cũng có $(x' + x'')y = (-1)^{pq}y(x' + x'')$; (2) nếu $x', x''$ là hai phần tử thuần nhất có các bậc tương ứng $p', p''$, $y$ là một phần tử thuần nhất bậc $q$ và $x'y = (-1)^{p'q}yx'$, $x''y = (-1)^{p''q}yx''$, thì
$$
(x'x'')y = (-1)^{(p'+p'')q}y(x'x'').
$$

#### Mệnh đề 13 {#alg-iii-s4-prop-13 .statement}

*Cho E là một đại số trên A phân bậc kiểu $\mathbf{Z}$ và S là một hệ sinh của đại số E gồm các phần tử thuần nhất $\neq 0$; để E là phản giao hoán (tương ứng, phản xứng), điều kiện cần và đủ là (36) đúng với mọi $x \in S$ và $y \in S$ (tương ứng, điều kiện này đúng và thêm nữa $x^2 = 0$ với mọi $x$ thuần nhất bậc lẻ thuộc S).*

Trước hết ta xét trường hợp các đại số phản giao hoán. Theo Bổ đề 4, đại số con F gồm các phần tử mà mọi thành phần thuần nhất $x \neq 0$ của chúng đều thỏa mãn (36) với mọi $y \in S$, chứa mọi phần tử của S và do đó $F = E$. Nếu bây giờ $F'$ cũng tương tự là đại số con của E gồm các phần tử mà mọi thành phần thuần nhất $x \neq 0$ của chúng đều thỏa mãn (36) với mọi phần tử thuần nhất $y \neq 0$, thì từ điều trên suy ra $F'$ chứa mọi phần tử của S và do đó $F' = E$, điều này hoàn tất chứng minh mệnh đề trong trường hợp này.

Để chứng minh mệnh đề trong trường hợp các đại số phản xứng, có thể giả sử E đã là phản giao hoán; khi đó ngay lập tức thấy rằng mọi phần tử thuần nhất bậc lẻ trong E đều có dạng $\sum_i z_ix_i$, trong đó $z_i \in E^+$ và $x_i \in S$ có bậc lẻ (dùng sự kiện rằng $E^+$ được chứa trong tâm của E); suy ra $\left( \sum_i z_ix_i \right)^2 = \sum_i z_i^2x_i^2 + \sum_{i<j} z_i z_j (x_ix_j + x_jx_i) = 0$ vì $x_i^2 = 0$ theo giả thiết và $x_ix_j + x_jx_i = 0$ theo (36).

#### Mệnh đề 14 {#alg-iii-s4-prop-14 .statement}

*Cho E và F là hai đại số trên A phân bậc kiểu $\mathbf{Z}$, cả hai đều phản giao hoán (tương ứng, phản xứng). Khi đó tích tenxơ xiên $E^g \otimes_A F$ (no. 7) là một đại số phản giao hoán (tương ứng, phản xứng).*

Một hệ sinh của $E^g \otimes_A F$ gồm các $x \otimes y$, trong đó $x$ (tương ứng, $y$) là một phần tử thuần nhất $\neq 0$ của E (tương ứng, F). Xét hai phần tử như vậy $x \otimes y, x' \otimes y'$, với $\deg(x) = p, \deg(y) = q, \deg(x') = p', \deg(y') = q'$, sao cho $x \otimes y$ có bậc $p + q$ và $x' \otimes y'$ có bậc $p' + q'$. Khi đó theo định nghĩa (no. 7, công thức (27)) và theo (36),
$$
\begin{align*}
(x \otimes y)(x' \otimes y') &= (-1)^{qp'}(xx') \otimes (yy') \\
(x' \otimes y')(x \otimes y) &= (-1)^{pq'}(x'x) \otimes (y'y) \\
&= (-1)^{pq'+pp'+qq'}(xx') \otimes (yy')
\end{align*}
$$
và tiêu chuẩn của Mệnh đề 13 cho thấy $E^g \otimes_A F$ là phản giao hoán vì $pq' + pp' + qq' - qp' \equiv (p + q)(p' + q')$ (mod. 2). Nếu thêm nữa E và F là phản xứng và $p + q$ là lẻ, thì một trong hai số $p, q$ tất yếu là lẻ, do đó $(x \otimes y)^2 = \pm (x^2) \otimes (y^2) = 0$ và Mệnh đề 13 cho thấy $E^g \otimes_A F$ là phản xứng.

#### Hệ quả {#alg-iii-s4-n9-cor-1 .statement}

*Cho E là một đại số trên A phân bậc kiểu $\mathbf{Z}$ phản giao hoán* (tương ứng, *phản xứng*). *Khi đó với mọi đồng cấu vành $\rho : A \to B$, đại số trên B phân bậc $\rho^*(E)$ (no. 8, *Nhận xét 2*) *là phản giao hoán* (tương ứng, *phản xứng*).

Vành B với phân bậc tầm thường có thể được xem như một đại số trên A phản xứng và $\rho^*(E) = E^g \otimes_A B$, do đó có thể áp dụng Mệnh đề 14.

#### Nhận xét {#alg-iii-s4-n9-rem-2 .statement}

Cho E là một đại số trên A phân bậc phản giao hoán kiểu $\mathbf{Z}$. Khi đó ánh xạ A-tuyến tính từ $E \otimes_A E$ vào E được xác định bởi phép nhân của E ($§ 1$, no. 3) là một đồng cấu từ đại số trên A phân bậc $E^g \otimes_A E$ vào E, vì, theo ký hiệu của Mệnh đề 14, trong đại số E,
$$
(xy)(x'y') = (-1)^{qp'}(xx')(yy').
$$

### Bài tập {#alg-iii-s4-exercises}

Xem [bài tập của § 4](exercises/s4/).
