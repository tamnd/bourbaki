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
pdf_pages: 0484-0508, 0650-0651
extraction: ocr
subsections:
    - "no": 1
      title: TENSOR PRODUCT OF A FINITE FAMILY OF ALGEBRAS
      page: 0
      pdf_page: 484
    - "no": 2
      title: UNIVERSAL CHARACTERIZATION OF TENSOR PRODUCTS OF ALGEBRAS
      page: 0
      pdf_page: 487
    - "no": 3
      title: MODULES AND MULTIMODULES OVER TENSOR PRODUCTS OF ALGEBRAS
      page: 0
      pdf_page: 489
    - "no": 4
      title: TENSOR PRODUCT OF ALGEBRAS OVER A FIELD
      page: 0
      pdf_page: 492
    - "no": 5
      title: TENSOR PRODUCT OF AN INFINITE FAMILY OF ALGEBRAS
      page: 0
      pdf_page: 494
    - "no": 6
      title: COMMUTATION LEMMAS
      page: 0
      pdf_page: 496
    - "no": 7
      title: TENSOR PRODUCT OF GRADED ALGEBRAS RELATIVE TO COMMUTATION FACTORS
      page: 0
      pdf_page: 498
    - "no": 8
      title: TENSOR PRODUCT OF GRADED ALGEBRAS OF THE SAME TYPES
      page: 0
      pdf_page: 504
    - "no": 9
      title: ANTICOMMUTATIVE ALGEBRAS AND ALTERNATING ALGEBRAS
      page: 0
      pdf_page: 506
statements: 43
exercises: 2
content_sha256: 3fc3231b230cd48877e058771d91d85fedeca843bc4d17b397a631b27c21e3b5
translated_from: content/en/alg/III/04_s4_tensor_products_of_algebras.md
source_content_sha256: 49f95c708f427e2fa95fa3af1f1ba7efb0d6fbfdf94099d282881d1313bbff03
translation_model: gpt-5.4-mini
translation_run: translate-vi-b55d44b5
glossary_version: 34
glossary_terms_sha256: c2c9b0460c4cd91ead64d23156ce206914b3ed2519c096f28919ae8209178687
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. TÍCH TENXƠ CỦA CÁC ĐẠI SỐ

Từ § 4 đến § 8 kể cả, A ký hiệu một vành giao hoán và, trừ khi có nói khác, các đại số được xét được giả thiết là kết hợp và có đơn vị, và các đồng cấu đại số được giả thiết là có đơn vị.

### 1. TÍCH TENXƠ CỦA MỘT HỌ HỮU HẠN CÁC ĐẠI SỐ

A luôn luôn ký hiệu một vành giao hoán có phần tử đơn vị. Cho $(E_i)_{i \in I}$ là một họ hữu hạn các A-đại số và cho $E = \bigotimes_{i \in I} E_i$ là tích tenxơ môđun của các A-môđun $E_i$ (II, § 3, no. 9). Ta sẽ định nghĩa một cấu trúc A-đại số trên $E$. Cho $m_i: E_i \otimes_A E_i \to E_i$ là ánh xạ A-tuyến tính định nghĩa phép nhân trên $E_i$ (§ 1, no. 3). Xét ánh xạ A-tuyến tính

$$
m' = \bigotimes_{i \in I} m_i: \bigotimes_{i \in I} (E_i \otimes_A E_i) \to \bigotimes_{i \in I} E_i = E;
$$

ánh xạ hợp thành

$$
\left( \bigotimes_{i \in I} E_i \right) \otimes_A \left( \bigotimes_{i \in I} E_i \right) \xrightarrow{\tau} \bigotimes_{i \in I} (E_i \otimes_A E_i) \xrightarrow{m'} \bigotimes_{i \in I} E_i
$$

trong đó $\tau$ là đẳng cấu tính kết hợp (II, § 3, no. 9) là một ánh xạ A-tuyến tính $m : E \otimes_A E \to E$; ta sẽ thấy rằng $m$ định nghĩa một cấu trúc đại số (kết hợp và có đơn vị) trên $E$. Thật vậy, khi thực hiện tường minh phép nhân do $m$ định nghĩa, ta thu được công thức

(1)
$$
\left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) = \bigotimes_{i \in I} (x_i y_i) \quad \text{cho } x_i, y_i \text{ trong } E_i \text{ và } i \in I.
$$

Do đó, nhờ tính tuyến tính, ta thấy ngay rằng nếu $e_i$ là phần tử đơn vị của $E_i$, $e = \bigotimes_{i \in I} e_i$ là phần tử đơn vị của $E$. Mặt khác, tính kết hợp của từng $E_i$ kéo theo quan hệ

$$
\left( \left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) \right) \left( \bigotimes_{i \in I} z_i \right) = \bigotimes_{i \in I} (x_i y_i z_i) = \left( \bigotimes_{i \in I} x_i \right) \left( \left( \bigotimes_{i \in I} y_i \right) \left( \bigotimes_{i \in I} z_i \right) \right)
$$

do đó, nhờ tính tuyến tính, ta được quan hệ $x(yz) = (xy)z$ với mọi $x, y, z$ trong $E$.

#### Định nghĩa 1 {#alg-iii-s4-def-1 .statement}

*Cho một họ* $(E_i)_{i \in I}$ *các đại số trên* $A$, *tích tenxơ của họ này*, được ký hiệu bởi $\bigotimes_{i \in I} E_i$ (hoặc, khi $I$ là khoảng $\{1, n\}$ của $\mathbf{N}$, $E_1 \otimes_A E_2 \otimes \cdots \otimes_A E_n$, hoặc đơn giản là $E_1 \otimes E_2 \otimes \cdots \otimes E_n$) *là đại số thu được bằng cách cho tích tenxơ của các* $A$*-môđun* $E_i$ *phép nhân được định nghĩa bởi* (1).

Quan hệ (1) cho thấy tích tenxơ $\bigotimes_{i \in I} E_i^0$ của các đại số *đối* của các $E_i$ là đại số đối của $\bigotimes_{i \in I} E_i$; nói riêng, nếu các $E_i$ *giao hoán*, thì $\bigotimes_{i \in I} E_i$ cũng giao hoán.

Cho $(E_i)_{i \in I}$ và $(F_i)_{i \in I}$ là hai họ các $A$-đại số với cùng một tập chỉ số hữu hạn $I$. Với mỗi $i \in I$, cho $f_i : E_i \to F_i$ là một đồng cấu A-đại số. Khi đó ánh xạ A-tuyến tính

$$
f = \bigotimes_{i \in I} f_i : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} F_i
$$

là một *đồng cấu A-đại số*, suy ra từ (1).

Với mọi phân hoạch $(I_j)_{j \in J}$ của $I$, các đẳng cấu tính kết hợp

$$
\bigotimes_{j \in J} \left( \bigotimes_{i \in I_j} E_i \right) \to \bigotimes_{i \in I} E_i
$$

(II, § 3, no. 9) cũng là các đẳng cấu *đại số*, suy ra từ (1) và các định nghĩa của chúng.

Khi $I$ là khoảng $[1, n]$ của $\mathbf{N}$ và tất cả các đại số $E_i$ đều bằng cùng một đại số $E$, thì đại số tích tenxơ $\bigotimes_{i \in I} E_i$ cũng được ký hiệu là $E^{\otimes n}$.

Trong phần còn lại của số này, chúng ta sẽ giới hạn sự chú ý vào các tính chất của tích tenxơ của hai đại số, và để cho người đọc nhiệm vụ mở rộng chúng sang các tích tenxơ của các họ hữu hạn tùy ý.

Cho $E, F$ là hai $A$-đại số; nếu $a$ (resp. $b$) là một iđêan trái của $E$ (resp. $F$), thì ảnh chính tắc $\operatorname{Im}(a \otimes b)$ của $a \otimes_A b$ trong $E \otimes_A F$ là một iđêan trái của $E \otimes_A F$; có các kết quả tương tự khi "left ideal" được thay bằng "right ideal" hoặc "two-sided ideal". Hơn nữa:

#### Mệnh đề 1 {#alg-iii-s4-prop-1 .statement}

*Cho $E, F$ là hai $A$-đại số và $a$ (resp. $b$) một iđêan hai phía của $E$ (resp. $F$). Khi đó đẳng cấu chính tắc của $A$-môđun*

$$
(E/a) \otimes (E/b) \to (E \otimes F)/(\operatorname{Im}(a \otimes F) + \operatorname{Im}(E \otimes b))
$$

*(II, § 3, no. 6, Corollary 1 to Proposition 6) là một đẳng cấu đại số*.

Điều này suy ra từ (1) và định nghĩa cho trong *loc. cit*.

#### Hệ quả 1 {#alg-iii-s4-prop-1-cor-1 .statement}

*Cho $E$ là một $A$-đại số và $a$ một iđêan của $A$. Khi đó $A$-môđun $aE$ là một iđêan hai phía của $E$ và đẳng cấu chính tắc của $(A/a)$-môđun*

$$
(A/a) \otimes_A E \to E/aE
$$

*là một đẳng cấu đại số của* $(A/a)$*.

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

Điều này suy ra ngay lập tức từ II, § 3, no. 7, Proposition 7 và định nghĩa của phép nhân trên $E \otimes F$.

#### Mệnh đề 3 {#alg-iii-s4-prop-3 .statement}

*Cho $A, B$ là hai vành giao hoán, $\varphi : A \to B$ một đồng cấu vành và $E, F$ là hai $A$-đại số. Khi đó đẳng cấu chính tắc của $B$-môđun*

$$
\varphi^*(E) \otimes_B \varphi^*(F) \to \varphi^*(E \otimes_A F)
$$

*(II, § 5, no. 1, Proposition 3) là một đẳng cấu đại số của $B$-đại số*.

#### Mệnh đề 4 {#alg-iii-s4-prop-4 .statement}

Cho $A, B$ là hai vành giao hoán, $\rho : A \to B$ một đồng cấu vành, $E$ một $A$-đại số và $F$ một $B$-đại số. Khi đó đẳng cấu chính tắc của $A$-môđun

$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E))
$$

(II, § 5, no. 2, Mệnh đề 6) là một đẳng cấu đại số $A$.

Các phép kiểm tra là tầm thường nhờ § 1, no. 5.

Đặc biệt, cấu trúc $A$-đại số trên $B \otimes_A E$, thu được bằng cách hạn chế vành $B$ của các vô hướng xuống $A$, trùng với cấu trúc của đại số $B \otimes_A E$, tích tenxơ của các $A$-đại số $B$ và $E$.

Cuối cùng, nếu $(A_i, \phi_{ji})$ là một hệ trực tiếp của các vành giao hoán, $(E_i, f_{ji})$ và $(F_i, g_{ji})$ là hai hệ trực tiếp của các $A_i$-đại số ($\S 1$, no. 6) và $A = \lim \rightarrow A_i$, thì đẳng cấu môđun $A$ chính tắc

$$
\lim \rightarrow (E_i \otimes_{A_i} F_i) \to (\lim \rightarrow E_i) \otimes_A (\lim \rightarrow F_i)
$$

(II, § 6, no. 3, Mệnh đề 7) cũng là một đẳng cấu đại số $A$, như suy ra từ các định nghĩa.

Các ví dụ về tích tenxơ của các đại số. (1) Cho $A$ là một vành giao hoán và $M, N$ là hai $A$-môđun; ánh xạ chính tắc

$$
\text{End}_A(M) \otimes_A \text{End}_A(N) \to \text{End}_A(M \otimes_A N)
$$

(II, § 4, no. 4) là một đồng cấu đại số $A$, như suy ra từ II, § 3, no. 2, công thức (5). Khi $M$ hoặc $N$ là một $A$-môđun xạ ảnh sinh hữu hạn, ta biết rằng đồng cấu này là song ánh (II, § 4, no. 4, Mệnh đề 4). Đặc biệt, ta thu lại được định nghĩa của tích tenxơ của hai ma trận vuông.

(2) Cho $S, T$ là hai monoid và $A^{(S)}$ và $A^{(T)}$ là các đại số của các monoid $S$ và $T$ trên vành $A$ (III, § 2, no. 6); khi đó có một đẳng cấu đại số $A$ chính tắc

$$
A^{(S)} \otimes_A A^{(T)} \to A^{(S \times T)}.
$$

Các phần tử $e_s \otimes e_t$ (tương ứng $e_{(s,t)}$), với $s$ chạy qua $S$ và $t$ chạy qua $T$, tạo thành một cơ sở của $A^{(S)} \otimes_A A^{(T)}$ nhờ II, § 3, no. 7, Hệ quả 2 của Mệnh đề 7 (tương ứng của $A^{(S \times T)}$; đẳng cấu mong muốn thu được bằng cách gửi $e_s \otimes e_t$ tới $e_{(s,t)}$ và từ các định nghĩa suy ra rằng đây thật sự là một đẳng cấu đại số.

### 2. ĐẶC TRƯNG HÓA PHỔ QUÁT CỦA TÍCH TENXƠ CỦA CÁC ĐẠI SỐ

#### Mệnh đề 5 {#alg-iii-s4-prop-5 .statement}

Cho $(E_i)_{i \in I}$ là một họ hữu hạn các $A$-đại số và, với mỗi $i \in I$, cho $e_i$ là phần tử đơn vị của $E_i$. Với mỗi $i \in I$, cho $u_i : E_i \to E = \bigotimes_{i \in I} E_i$ là ánh xạ tuyến tính trên $A$ được xác định bởi

$$
u_i(x_i) = \bigotimes_j x'_j \quad \text{with } x'_i = x_i \text{ and } x'_j = e_j \text{ for } j \neq i.
$$

(i) *Các $u_i$ là các đẳng cấu đại số trên $\mathbf{A}$; hơn nữa, với $i \neq j$, các phần tử $u_i(x_i)$ và $u_j(x_j)$ giao hoán trong $\mathbf{E}$ với mọi $x_i \in \mathbf{E}_i$ và $x_j \in \mathbf{E}_j$ và $\mathbf{E}$ được sinh bởi hợp của các đại số con $u_i(\mathbf{E}_i)$.*

(ii) *Cho $\mathbf{F}$ là một $\mathbf{A}$-đại số và, với mọi $i \in \mathbf{I}$, cho $v_i : \mathbf{E}_i \to \mathbf{F}$ là một đồng cấu đại số trên $\mathbf{A}$, trong đó các $v_i$ thỏa mãn rằng, với $i \neq j$, $v_i(x_i)$ và $v_j(x_j)$ giao hoán trong $\mathbf{F}$ với mọi $x_i \in \mathbf{E}_i$ và $x_j \in \mathbf{E}_j$. Khi đó tồn tại một và chỉ một đồng cấu đại số trên $\mathbf{A}$ $w : \mathbf{E} \to \mathbf{F}$ sao cho*

$$
v_i = w \circ u_i \quad \text{for all } i \in \mathbf{I}.
$$

(i) Ánh xạ $u_i$ là một đồng cấu đại số theo định nghĩa của phép nhân trên $\mathbf{E}$. Nếu $i \neq j$, $x_i \in \mathbf{E}_i, x_j \in \mathbf{E}_j$, thì

$$
u_i(x_i) = \bigotimes_k x'_k \quad \text{với } x'_i = x_i, x'_k = e_k \text{ với } k \neq i,
$$
$$
u_j(x_j) = \bigotimes_k x''_k \quad \text{với } x''_j = x_j, x''_k = e_k \text{ với } k \neq j.
$$

Rõ ràng $x'_k x''_k = x''_k x'_k$ với mọi $k \in \mathbf{I}$ và do đó $u_i(x_i)$ và $u_j(x_j)$ giao hoán trong $\mathbf{E}$ theo công thức (1) (no. 1) định nghĩa phép nhân trong $\mathbf{E}$. Khẳng định cuối cùng suy ra từ quan hệ $\bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i)$.

(ii) Với mỗi $i \in \mathbf{I}$, cho $x_i$ là một phần tử của $\mathbf{E}_i$. Khi đó tích $\prod_{i \in \mathbf{I}} v_i(x_i)$ được xác định trong $\mathbf{F}$ độc lập với mọi thứ tự trên $\mathbf{I}$ vì đại số $\mathbf{F}$ là kết hợp và các phần tử $v_i(x_i)$ giao hoán từng đôi một. Ánh xạ $(x_i)_{i \in \mathbf{I}} \to \prod_{i \in \mathbf{I}} v_i(x_i)$ từ $\prod_{i \in \mathbf{I}} \mathbf{E}_i$ vào $\mathbf{F}$ hiển nhiên là $\mathbf{A}$-đa tuyến tính và do đó tồn tại một và chỉ một ánh xạ $\mathbf{A}$-tuyến tính $w : \mathbf{E} \to \mathbf{F}$ sao cho

$$
w\left( \bigotimes_i x_i \right) = \prod_i v_i(x_i).
$$

Bây giờ, đồng cấu đại số trên A $w : \mathbf{E} \to \mathbf{F}$ cần thỏa mãn (5), điều này suy ra từ (4) và thực tế là $\bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i)$. Điều này chứng minh tính duy nhất của $w$; còn lại phải chứng minh rằng ánh xạ $\mathbf{A}$-tuyến tính $w$ được xác định bởi (5) là một đồng cấu đại số trên A và thỏa mãn (4). Việc $w$ thỏa mãn (4) là hiển nhiên: chỉ cần áp dụng (5) cho trường hợp $x_j = e_j$ với $j \neq i$ và ta thu được $w(u_i(x_i)) = v_i(x_i)$. Cuối cùng, $w$ là một đồng cấu đại số, vì

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

điều này, nhờ tính tuyến tính, hoàn tất chứng minh.

Cặp có thứ tự gồm E và ánh xạ chính tắc $\phi : (x_i) \mapsto \bigotimes_i x_i$ của $\prod_i E_i$ vào E là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1) trong đó $\Sigma$ là loài của cấu trúc đại số trên A, các đồng cấu là các đồng cấu đại số trên A và các ánh xạ $\alpha$ là các ánh xạ $\prod_i u_i$ của $\prod_i E_i$ vào một đại số trên A sao cho các $u_i$ là các đồng cấu đại số trên A và $u_i(x_i)$ và $u_j(x_j)$ giao hoán với nhau khi $i \neq j$, với mọi $x_i \in E_i$ và $x_j \in E_j$.

#### Hệ quả {#alg-iii-s4-n2-cor-1 .statement}

*Cho* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *là hai họ hữu hạn các A-đại số và, với mọi* $i \in I$, *cho* $f_i : E_i \to F_i$ *là một đồng cấu đại số. Nếu* $u_i : E_i \to \bigotimes_{j \in I} E_j, v_i : F_i \to \bigotimes_{j \in I} F_j$ *là các đồng cấu chính tắc, thì ánh xạ* $f = \bigotimes_i f_i$ *(xem no. 1)* *là đồng cấu đại số trên A duy nhất sao cho* $f \circ u_i = v_i \circ f_i$ *với mọi* $i \in I$.

Chỉ cần lưu ý rằng các đồng cấu $g_i = v_i \circ f_i$ thỏa mãn $g_i(x_i) = v_i(f_i(x_i))$ và $g_j(x_j) = v_j(f_j(x_j))$ giao hoán với nhau khi $i \neq j$, $x_i \in E_i$ và $x_j \in E_j$; rồi áp dụng Mệnh đề 5.

Khi, trong Mệnh đề 5, đại số F được giả thiết là *giao hoán*, thì giả thiết rằng $v_i(x_i)$ và $v_j(x_j)$ có thể hoán vị với nhau khi $i \neq j$ được tự động thỏa mãn. Do đó, *khi F giao hoán*, có một song ánh chính tắc

$$
\text{Hom}_{A\text{-đại số.}} \left( \bigotimes_i E_i, F \right) \to \prod_i \text{Hom}_{A\text{-đại số.}} (E_i, F),
$$

nghĩa là song ánh gán cho mỗi đồng cấu $w$ của $\bigotimes_i E_i$ vào F họ các $w \circ u_i$.

Chú ý rằng nếu E là một A-đại số giao hoán, thì cấu trúc vành của $E \otimes_A F$ cũng chính là cấu trúc vành của $F_{(E)}$ (\S 1, no. 5).

### 3. MÔĐUN VÀ ĐA MÔĐUN TRÊN TÍCH TENXƠ CỦA CÁC ĐẠI SỐ

#### Định nghĩa 2 {#alg-iii-s4-def-2 .statement}

*Cho E là một A-đại số (có đơn vị). Một E-môđun trái (tương ứng phải) là một môđun trái (tương ứng phải) trên vành nền của E.*

Trừ khi có nói rõ khác, mọi môđun và đa môđun xét trong số này đều là môđun và đa môđun trái.

Nếu M là một E-môđun, thì đồng cấu $\eta : A \to E$ (\S 1, no. 4) xác định trên M một cấu trúc A-môđun, gọi là cấu trúc nền của cấu trúc E-môđun trên M; với $\alpha \in A, s \in E, x \in M$,

$$
\alpha(sx) = s(\alpha x) = (\alpha s)x,
$$

do đó với mọi $s \in E$, phép vị tự $h_s : x \mapsto sx$ của M là một tự đồng cấu của cấu trúc A-môđun nền. Ngược lại, cho một cấu trúc E-môđun trên M tương đương với cho một cấu trúc A-môđun trên M và một đồng cấu đại số trên A $s \mapsto h_s$ của E vào $\mathrm{End}_A(M)$.

#### Định nghĩa 3 {#alg-iii-s4-def-3 .statement}

*Cho E và F là hai A-đại số (có đơn vị) và M là một tập hợp mang một cấu trúc E-môđun và một cấu trúc F-môđun. M được gọi là một song môđun (trái) trên các đại số E và F nếu:*

(1) *M là một song môđun trên các vành nền của E và F* (II, § 1, no. 14);
(2) *hai cấu trúc A-môđun nền tương ứng với các cấu trúc E-môđun và F-môđun trên M là như nhau*.

Điều kiện sau nói rằng nếu e và $e'$ lần lượt là các phần tử đơn vị của E và F, thì

$$
(\alpha e)x = (\alpha e')x \quad \text{for } \alpha \in A, x \in M;
$$

sau đó $\alpha x$ được dùng để ký hiệu giá trị chung của hai vế.

Cũng có thể nói rằng, việc cho trên M một cấu trúc song môđun trên E và F tương đương với việc cho một cấu trúc A-môđun trên M và đồng thời hai đồng cấu đại số trên A $s \mapsto h'_s$ của E vào $\mathrm{End}_A(M)$ và $t \mapsto h''_t$ của F vào $\mathrm{End}_A(M)$ sao cho $h'_s h''_t = h''_t h'_s$ với mọi $s \in E$ và $t \in F$. Do đó (no. 2, Mệnh đề 5) một đồng cấu đại số trên A $u \mapsto h_u$ của $E \otimes_A F$ vào $\mathrm{End}_A(M)$ được dẫn xuất một cách chính tắc sao cho $h_{s \otimes t} = h'_s h''_t = h''_t h'_s$ với $s \in E$ và $t \in F$. Nói cách khác, như thế một cấu trúc môđun $(E \otimes_A F)$ được định nghĩa trên M, và cấu trúc này được nói là liên kết với cấu trúc song môđun đã cho trên E và F, dưới đó

$$
(s \otimes t).x = s(tx) = t(sx) \quad \text{for } s \in E, t \in F \text{ and } x \in M.
$$

Các cấu trúc E-môđun và F-môđun đã cho trên M có thể được dẫn xuất từ cấu trúc môđun $(E \otimes_A F)$ này bằng cách hạn chế vành vô hướng, tương ứng với hai đồng cấu chính tắc $E \to E \otimes_A F$ và $F \to E \otimes_A F$.

Ngược lại, nếu một cấu trúc môđun $(E \otimes_A F)$ được cho trên M, thì nhờ các đồng cấu chính tắc $E \to E \otimes_A F$ và $F \to E \otimes_A F$ ta được một cấu trúc E-môđun và một cấu trúc F-môđun trên M và hiển nhiên rằng M là một *song môđun* trên các đại số E và F với hai cấu trúc này và cấu trúc môđun $(E \otimes_A F)$ đã cho được liên kết với cấu trúc song môđun này.

Như vậy một sự tương ứng một-một đã được thiết lập giữa các môđun $(E \otimes_A F)$ và các song môđun trên các đại số E và F. Rõ ràng mọi môđun con song của M đều là một môđun con đối với cấu trúc môđun $(E \otimes_A F)$ liên kết, và ngược lại. Có các kết quả tương tự cho thương, tích, tổng trực tiếp và giới hạn nghịch và trực tiếp. Cuối cùng, nếu $M'$ là một song môđun khác trên các đại số E và F và $f : M \to M'$ là một đồng cấu song môđun, thì $f$ cũng là một đồng cấu môđun $(E \otimes_A F)$ và ngược lại.

Hiển nhiên có các mệnh đề tương ứng đối với các cấu trúc song môđun phải, hoặc khi chẳng hạn có một cấu trúc E-môđun trái và một cấu trúc F-môđun phải; trong trường hợp này ta nói về một $(E, F)$-song môđun và việc được cho một cấu trúc như vậy tương đương với việc được cho một cấu trúc song môđun trái trên E và $F^o$.

#### Ví dụ {#alg-iii-s4-n3-exa-1 .statement}

(1) Cho B là một A-đại số; vành B có một cách chính tắc một cấu trúc song môđun $(B, B)$ (II, § 1, no. 14, Ví dụ 1) và, nếu e là phần tử đơn vị của B, thì $(\alpha e)x = x(\alpha e) = \alpha x$ với mọi $x \in B$ và mọi $\alpha \in A$; do đó có thể xem B như một song môđun trái trên các đại số B và $B^o$ (đối của B); vì vậy với cấu trúc song môđun trên $(B, B)$ của B có liên kết một cấu trúc môđun $(B \otimes_A B^o )$ sao cho, với $b, x$ và $b'$ trong B,

$$
(b \otimes b').x = bx b'
$$

vế phải là tích trong vành B.

(2) Cho E và F là hai A-đại số, $e, e'$ là các phần tử đơn vị tương ứng của chúng, M là một E-môđun và N là một F-môđun; các cấu trúc môđun này xác định trên M một cấu trúc song môđun trên các vành A và E và trên N một cấu trúc song môđun trên các vành A và F; từ đó do đó suy ra một cấu trúc song môđun trên các vành E và F trên tích tenxơ $M \otimes_A N$, được định nghĩa bởi

$$
x.(m \otimes n) = (x.m) \otimes n, \quad y.(m \otimes n) = m \otimes (y.n)
$$

với $x \in E, y \in F, m \in M, n \in N$ (II, § 3, no. 4); cũng thấy rằng các điều kiện (8) được thỏa mãn và do đó cấu trúc song môđun ở trên liên kết với một cấu trúc môđun $(E \otimes_A F)$ trên $M \otimes_A N$, sao cho

$$
(x \otimes y).(m \otimes n) = (x.m) \otimes (y.n)
$$

với $x \in E, y \in F, m \in M, n \in N$.

Đặc biệt, khi lấy $M = E_s, E_s \otimes_A N$ thì $E_s \otimes_A N$ có một cấu trúc môđun $(E \otimes_A F)$ một cách chính tắc; mặt khác, $E \otimes_A N$ được đồng nhất một cách chính tắc với $E \otimes_A (F_d \otimes_F N) = (E \otimes_A F) \otimes_F N$, trong đó $E \otimes_A F$ được xem như có cấu trúc môđun phải trên F được định bởi đồng cấu chính tắc $v : F \to E \otimes_A F$; với $x, x'$ trong E, $y \in F, n \in N$, do đó $x' \otimes n$ được đồng nhất với $(x' \otimes e') \otimes n$ và $(x \otimes y).(x' \otimes n') = (xx') \otimes (y.n)$ với $((xx') \otimes y) \otimes n$. Môđun $(E \otimes_A F)$-môđun $E_s \otimes_A N$ do đó được đồng nhất với môđun $(E \otimes_A F)$-môđun dẫn xuất từ N bằng cách mở rộng các vô hướng lên $E \otimes_A F$ nhờ đồng cấu $v$ (II, § 5, no. 1). Ánh xạ chính tắc $n \mapsto e \otimes n$ của N vào $E_s \otimes_A N$ được đồng nhất với ánh xạ chính tắc $n \mapsto (e \otimes e') \otimes n$ của N vào $(E \otimes_A F) \otimes_F N$; điều này được biết là một đồng cấu F.

Với cùng ký hiệu, cho P là một môđun phải trên $(E \otimes_A F)$; khi đó có một đẳng cấu Z-môđun chính tắc

(11) $$ P \otimes_{E \otimes_A F} (E_s \otimes_A N) \to P \otimes_F N $$

trong đó ở vế phải P được xem như một môđun phải trên F nhờ đồng cấu chính tắc $v$. Quả vậy, P được đồng nhất một cách chính tắc với $P \otimes_{E \otimes_A F} (E \otimes_A F)$ và $(E \otimes_A F) \otimes_F N$ với $E \otimes_A (F \otimes_F N)$ và do đó với $E \otimes_A N$, điều này thiết lập đẳng cấu đã nêu (II, § 3, no. 8, Mệnh đề 8 và II, § 3, no. 4, mệnh đề 4).

Tất cả những điều trên mở rộng cho *multimôđun* (II, § 1, no. 14).

### 4. TÍCH TENXƠ CỦA CÁC ĐẠI SỐ TRÊN MỘT TRƯỜNG

Cho K là một *trường* giao hoán và E, F là hai đại số trên K mà các phần tử đơn vị tương ứng $e, e'$ đều *khác 0*. Khi đó các đồng cấu $\eta_E : K \to E$ và $\eta_F : K \to F$ (§ 1, no. 3) là các đơn ánh cho phép đồng nhất K với một trường con của E (resp. F). Các đồng cấu chính tắc $u : E \to E \otimes_K F$ và $v : F \to E \otimes_K F$, được định bởi $u(x) = x \otimes e'$ và $v(y) = e \otimes y$ là *đơn ánh* (II, § 7, no. 9, Mệnh đề 19) và cho phép đồng nhất E và F với các *đại số con* của $E \otimes_K F$, cả hai đều có làm phần tử đơn vị là phần tử đơn vị $e \otimes e'$ của $E \otimes_K F$. Trong $E \otimes_K F, E \cap F = K$ (II, § 7, no. 9, Mệnh đề 19).

Nếu E' và F' là các đại số con của E và F tương ứng, thì đồng cấu chính tắc $E' \otimes_K F' \to E \otimes_K F$ là đơn ánh và cho phép đồng nhất $E' \otimes_K F'$ với đại số con của $E \otimes_K F$ sinh bởi $E' \cup F'$ (II, § 7, no. 7, Mệnh đề 14).

#### Mệnh đề 6 {#alg-iii-s4-prop-6 .statement}

*Cho E, F là hai đại số khác 0 trên một trường giao hoán, K, C (resp. D) là một đại số con của E (resp. F) và C' (resp. D') là tập trung hóa của C trong E (resp. D trong F). Khi đó tập trung hóa của C \otimes_K D trong E \otimes_K F là C' \otimes_K D'.*

Tất cả quy về việc kiểm tra rằng một phần tử $z = \sum_i x_i \otimes y_i$ của tập trung hóa của $C \otimes_K D$ ($x_i \in F, y_i \in F$) thuộc $C' \otimes_K D'$; ta biết rằng

$$
C' \otimes_K D' = (C' \otimes_K F) \cap (E \otimes_K D')
$$

(II, § 7, no. 7, Hệ quả của Mệnh đề 14). Các $y_i$ có thể được giả sử là độc lập tuyến tính trên K; với mọi $x \in C$, tất yếu $(x \otimes e')z = z(x \otimes e')$, tức là $\sum_i (xx_i - x_ix) \otimes y_i = 0$, do đó $xx_i = x_ix$ với mọi $i$ (II, § 3, no. 7, Hệ quả 1 của Mệnh đề 7); suy ra tất yếu $x_i \in C'$ với mọi $i$ và do đó $z \in C' \otimes_K F$; cũng có thể chứng minh tương tự rằng $z \in E \otimes_K D'$, suy ra mệnh đề.

#### Hệ quả {#alg-iii-s4-n4-cor-1 .statement}

*Nếu Z và Z' lần lượt là các tâm của E và F, thì tâm của E \otimes_K F là Z \otimes_K Z'*

Cho E và F là hai đại số con của một đại số G trên một trường giao hoán K; giả sử mọi phần tử của E đều giao hoán với mọi phần tử của F. Khi đó các đơn ánh chính tắc $i : E \to G, j : F \to G$ định nghĩa một đồng cấu chính tắc $h = i \otimes j : E \otimes_K F \to G$ (no. 2, Mệnh đề 5) sao cho
$$
(i \otimes j)(x \otimes y) = xy \quad \text{cho } x \in E, y \in F.
$$

#### Định nghĩa 4 {#alg-iii-s4-def-4 .statement}

*Cho một đại số G trên một trường giao hoán K, hai đại số con E, F của G được gọi là tách tuyến tính trên K nếu chúng thỏa mãn các điều kiện sau:*
(1) *mọi phần tử của E giao hoán với mọi phần tử của F;*
(2) *đồng cấu chính tắc từ $E \otimes_K F$ vào G là đơn ánh.*

#### Mệnh đề 7 {#alg-iii-s4-prop-7 .statement}

*Cho G là một đại số trên một trường giao hoán K và E, F là hai đại số con của G sao cho mọi phần tử của E giao hoán với mọi phần tử của F. Để E và F tách tuyến tính trên K, cần và đủ rằng tồn tại một cơ sở của E trên K là một tập con tự do của G đối với cấu trúc môđun phải F trên G. Khi đó:*
(i) *đồng cấu chính tắc $h : E \otimes_K F \to G$ là một đẳng cấu từ $E \otimes_K F$ lên đại số con của G sinh bởi $E \cup F$;*
(ii) $E \cap F = K;$
(iii) *mọi tập con tự do của E (resp. F) trên K là một tập con tự do của G với cấu trúc môđun phải F (resp. môđun trái E) của nó.*

Điều kiện của mệnh đề hiển nhiên là cần, vì mọi cơ sở của E trên K đều là một cơ sở của $E \otimes_K F$ với cấu trúc môđun phải F của nó (II, § 3, no. 7, Hệ quả 1 của Mệnh đề 7). Để thấy điều kiện ấy là đủ, xét ảnh H của $E \otimes_K F$ qua h; đó là tập các tổng $\sum_i x_i y_i = \sum_i y_i x_i$ trong G, với $x_i \in E$ và $y_i \in F$; nếu $(a_\lambda)$ là một cơ sở của E trên K, thì H do đó cũng là môđun con của môđun phải hoặc trái F của G, được sinh bởi $(a_\lambda)$. Điều kiện của mệnh đề vì thế có nghĩa là tồn tại một cơ sở $(a_\lambda)$ của E đồng thời là một cơ sở của F-môđun H; suy ra h là đơn ánh. Mệnh đề (iii) suy ra từ sự kiện rằng mọi tập con tự do của E đều được chứa trong một cơ sở của E (II, § 7, no. 1, Định lý 2).

#### Hệ quả 1 {#alg-iii-s4-prop-7-cor-1 .statement}

*Để đồng cấu chính tắc từ $E \otimes_K F$ vào G là song ánh, cần và đủ rằng tồn tại một cơ sở của E trên K là một cơ sở của F-môđun phải hay trái G.*

#### Hệ quả 2 {#alg-iii-s4-prop-7-cor-2 .statement}

*Cho E, F là hai đại số con của G, có hạng hữu hạn trên K và sao cho mọi phần tử của E giao hoán với mọi phần tử của F. Để E và F tách tuyến tính trên K, cần và đủ rằng đại số con H của G được sinh bởi $E \cup F$ thỏa mãn*
$$
[H : K] = [E : K] \cdot [F : K].
$$
Điều này nói rằng hạng trên K của đồng cấu chính tắc toàn ánh h : E \otimes_K F \to H bằng hạng của E \otimes_K F trên K, điều đó tương đương với việc nói rằng đồng cấu này là song ánh (II, § 7, No. 4, Mệnh đề 9).

### 5. TÍCH TENXƠ CỦA MỘT HỌ VÔ HẠN CÁC ĐẠI SỐ

Cho A là một vành giao hoán và $(E_i)_{i \in I}$ là một họ tùy ý các A-đại số (có đơn vị). Với mọi tập con hữu hạn J của I, kí hiệu $E_J$ là tích tenxơ $\bigotimes_{i \in J} E_i$ của các đại số E_i có chỉ số $i \in J$; kí hiệu $e_i$ là phần tử đơn vị của E_i và $e_J = \bigotimes_{i \in J} e_i$ là phần tử đơn vị của E_J; kí hiệu $f_{J,i}$ là đồng cấu chính tắc $E_i \to E_J$ với $i \in J$ (no. 2, Mệnh đề 5). Nếu J, J' là hai tập con hữu hạn của I sao cho $J \subset J'$, thì một đồng cấu $f_{J'J} : E_J \to E_{J'}$ được suy ra một cách chính tắc (no. 2, Mệnh đề 5), bởi điều kiện $f_{J'J} \circ f_{J,i} = f_{J',i}$ với mọi $i \in J$. Hơn nữa tính duy nhất của $f_{J'J}$ suy ra rằng nếu J, J', J'' là ba tập con hữu hạn của I sao cho $J \subset J' \subset J''$, thì $f_{J''J} = f_{J''J'} \circ f_{J'J}$. Nói cách khác, $(E_J, f_{J'J})$ là một hệ trực tiếp các A-đại số có tập chỉ số là tập có hướng phải $\mathcal{F}(I)$ của các tập con hữu hạn của I.

#### Định nghĩa 5 {#alg-iii-s4-def-5 .statement}

*Giới hạn trực tiếp E của hệ trực tiếp* $(E_J, f_{J'J})$ *được gọi là tích tenxơ của họ các A-đại số* $(E_i)_{i \in I}$.

Nếu I hữu hạn, thì E được đồng nhất với $\bigotimes_{i \in I} E_i$. Do lạm dụng ký hiệu, E cũng được ký hiệu bởi $\bigotimes_{i \in I} E_i$ ngay cả khi I là vô hạn.

Với mọi tập con hữu hạn J của I, kí hiệu $f_J$ là đồng cấu chính tắc $\bigotimes_{i \in J} E_i \to \bigotimes_{i \in I} E_i$ (viết $f_i$ thay cho $f_{\{i\}}$); nếu e là phần tử đơn vị của $\bigotimes_{i \in I} E_i$, thì $f_J(e_J) = e$ với mọi $J \in \mathcal{F}(I)$. Hiển nhiên rằng nếu tất cả các đại số E_i đều giao hoán, thì $\bigotimes_{i \in I} E_i$ cũng giao hoán.

#### Mệnh đề 8 {#alg-iii-s4-prop-8 .statement}

(i) *Các đồng cấu* $f_i : E_i \to E = \bigotimes_{k \in I} E_k$ *thỏa mãn rằng với hai chỉ số* i, j *sao cho* $i \neq j$, $f_i(x_i)$ *và* $f_j(x_j)$ *giao hoán trong* E *với mọi* $x_i \in E_i$ *và* $x_j \in E_j$; *hơn nữa,* E *được sinh bởi hợp của các đại số con* $f_i(E_i)$.

(ii) *Cho F là một đại số trên A và, với mọi* $i \in I$, *cho* $u_i : E_i \to F$ *là một đồng cấu đại số trên A sao cho, với* $i \neq j$, $u_i(x_i)$ *và* $u_j(x_j)$ *giao hoán trong* F *với mọi* $x_i \in E_i$ *và* $x_j \in E_j$. *Khi đó tồn tại duy nhất một đồng cấu đại số trên A* $u : E \to F$ *sao cho* $u_i = u \circ f_i$ *với mọi* $i \in I$.

(i) Vì, với mọi tập con hữu hạn J của I, $f_i = f_J \circ f_{J,i}$, khẳng định thứ nhất trong (i) suy ra từ no. 2, Mệnh đề 5, lấy J chứa i và j; khẳng định thứ hai cũng suy ra từ no. 2, Mệnh đề 5, xét đến sự kiện rằng E là hợp của các $f_J(E_J)$ khi J chạy qua $\mathcal{F}(I)$.

(ii) Với mọi tập con hữu hạn J của I, suy ra từ no. 2, Mệnh đề 5 rằng tồn tại duy nhất một đồng cấu $u_J : E_J \to F$ sao cho $u_J \circ f_{J,i} = u_i$ với mọi $i \in J$; suy ngay từ tính duy nhất này rằng, với $J \subset J'$, $u_J = u_{J'} \circ f_{J'J}$; nói cách khác, các $u_J$ tạo thành một *hệ trực tiếp* các đồng cấu. Đặt $u = \lim \to u_J : E \to F$; khi đó theo định nghĩa $u_J = u \circ f_J$ với mọi tập con hữu hạn $J$ của $I$ và đặc biệt $u_i = u \circ f_i$ với mọi $i \in I$; tính duy nhất của $u$ suy ra từ các hệ thức này và từ việc các $f_i(E_i)$ sinh ra đại số $E$.

#### Hệ quả {#alg-iii-s4-n5-cor-1 .statement}

*Cho* $(E_i)_{i \in I},\ (E'_i)_{i \in I}$ *là hai họ các* $A$*-đại số có cùng một tập chỉ số và, với mọi* $i \in I$, *cho* $u_i : E_i \to E'_i$ *là một đồng cấu đại số. Khi đó tồn tại duy nhất một* $A$*-đồng cấu đại số* $u : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} E'_i$ *sao cho, với mọi* $i \in I$, *biểu đồ*

$$
\begin{array}{ccc}
E_i & \xrightarrow{u_i} & E'_i \\
| & & | \\
\bigotimes_{i \in I} E_i & \xrightarrow{u} & \bigotimes_{i \in I} E'_i
\end{array}
$$

*là giao hoán*, $f_i$ *và* $f'_i$ *ký hiệu các đồng cấu chính tắc*.

Chỉ cần áp dụng Mệnh đề 8 cho đồng cấu $f'_i \circ u_i$.

Đồng cấu $u$ được xác định trong Hệ quả của Mệnh đề 8 được ký hiệu bởi $\bigotimes_{i \in I} u_i$. Nếu $J$ là bất kỳ tập con nào của $I$, có thể áp dụng Mệnh đề 8 cho họ $(f_i)_{i \in J}$ các đồng cấu chính tắc $f_i : E_i \to \bigotimes_{i \in I} E_i = E$; thu được một đồng cấu chính tắc $E_J \to E$ cũng được ký hiệu bởi $f_J$ và, khi $J$ là *hữu hạn*, trùng với đồng cấu được ký hiệu như vậy ở trên.

Bây giờ cho $(x_i)_{i \in I}$ là một phần tử của $\prod_{i \in I} E_i$ sao cho họ $(x_i - e_i)_{i \in I}$ có *giá hữu hạn* $H$. Hiển nhiên rằng, nếu $J$ và $J'$ là hai tập con hữu hạn của $I$ chứa $H$, thì

$$
f_J((x_i)_{i \in J}) = f_{J'}((x_i)_{i \in J'}).
$$

### 6. CÁC BỔ ĐỀ GIAO HOÁN

Giá trị chung của các $f_J((x_i)_{i \in J})$ đối với các tập con hữu hạn $J \supset H$ của $I$ được ký hiệu là $\bigotimes_{i \in I} x_i$.

#### Mệnh đề 9 {#alg-iii-s4-prop-9 .statement}

*Cho* $(E_i)_{i \in I}$ *là một họ các* $A$*-đại số và với mỗi* $i \in I$ *cho* $B_i$ *là một cơ sở của* $E_i$ *sao cho phần tử đơn vị* $e_i$ *thuộc* $B_i$. *Cho* $B$ *là tập hợp các phần tử có dạng* $\bigotimes_{i \in I} x_i$, *trong đó* $(x_i)$ *chạy qua tập hợp các phần tử của* $\prod_{i \in I} B_i$ *sao cho họ* $(x_i - e_i)$ *có giá hữu hạn*. *Khi đó* $B$ *là một cơ sở của đại số* $\bigotimes_{i \in I} E_i$ *và cơ sở này chứa phần tử đơn vị* $e$.

Với mọi tập con hữu hạn $J$ của $I$, cho $B_J$ là cơ sở của $E_J = \bigotimes_{i \in J} E_i$ tích tenxơ của các cơ sở $B_i$ với $i \in J$ (II, § 3, no. 9). Từ các định nghĩa suy ra ngay rằng $B$ là hợp của các $f_J(B_J)$ khi $J$ chạy qua $\mathcal{F}(I)$ và rằng $f_{J',J}(B_J) \subset B_{J'}$ khi $J \subset J'$; do đó $(B_J)$ là một hệ trực tiếp các tập con của các $E_J$ và $B = \lim \rightarrow B_J$; kết luận sau đó suy ra từ II, § 6, no. 2, Hệ quả của Mệnh đề 5.

Cơ sở $B$ cũng được gọi là *tích tenxơ* của các cơ sở $B_i$ với $i \in I$; khi các điều kiện của Mệnh đề 9 được thỏa mãn, các đồng cấu chính tắc $f_J : E_J \to E = \bigotimes_{i \in I} E_i$ là *đơn ánh* đối với mọi tập con $J$ của $I$, vì nếu $B_J$ là cơ sở của $E_J$ là tích tenxơ của các $B_i$ với $i \in J$, thì ngay lập tức kiểm tra được rằng hạn chế của $f_J$ lên $B_J$ là đơn ánh và ánh xạ $B_J$ lên một tập con của $B$.

*Cho* $A$ *là một vành giao hoán, $E$ là một* $A$*-đại số, $(x_i)_{1 \leq i \leq n}$ là một dãy hữu hạn các phần tử của* $E$, $(\lambda_i)_{1 \leq i \leq n}$ *là một dãy hữu hạn các phần tử của* $A$ *và* $y$ *là một phần tử của* $E$; *giả sử rằng*
$$
x_i y = \lambda_i y x_i \quad \text{cho } 1 \leq i \leq n.
$$
*Khi đó*
$$
(x_1 x_2 \ldots x_n) y = (\lambda_1 \lambda_2 \ldots \lambda_n) y (x_1 x_2 \ldots x_n).
$$

Vì bổ đề là tầm thường khi $n = 1$, ta chứng minh bằng quy nạp theo $n \geq 2$. Bây giờ
$$
(x_1 x_2 \ldots x_n) y = (x_1 \ldots x_{n-1})(x_n y)
= (x_1 \ldots x_{n-1})(\lambda_n y x_n) = \lambda_n ((x_1 \ldots x_{n-1}) y) x_n,
$$
mà, theo giả thiết quy nạp, bằng
$$
\lambda_n (\lambda_1 \ldots \lambda_{n-1}) y (x_1 \ldots x_{n-1}) x_n = (\lambda_1 \ldots \lambda_{n-1} \lambda_n) y (x_1 \ldots x_{n-1} x_n),
$$
do đó bổ đề.

#### Bổ đề 2 {#alg-iii-s4-lem-2 .statement}

*Cho $A$ là một vành giao hoán, $E$ là một $A$-đại số và $(x_i)_{1 \leq i \leq n}$ và $(y_i)_{1 \leq i \leq n}$ là hai dãy hữu hạn gồm $n$ phần tử của $E$; giả sử rằng với $1 \leq j \leq i \leq n$,*
$$
x_i y_j = \lambda_{ij} y_j x_i \quad \text{với } \lambda_{ij} \in A.
$$
*Khi đó*
$$
(x_1 x_2 \ldots x_n)(y_1 y_2 \ldots y_n) = \left( \prod_{i > j} \lambda_{ij} \right) (x_1 y_1)(x_2 y_2) \ldots (x_n y_n).
$$

Vì bổ đề là tầm thường khi $n = 1$, ta lại chứng minh bằng quy nạp theo $n$ với $n \geq 2$. Nhờ Bổ đề 1,
$$
(x_1 \ldots x_n)(y_1 \ldots y_n) = x_1 (x_2 \ldots x_n) y_1 (y_2 \ldots y_n)
= \left( \prod_{i > 1} \lambda_{i1} \right) (x_1 y_1)(x_2 \ldots x_n)(y_2 \ldots y_n)
$$
và khi đó chỉ cần áp dụng giả thiết quy nạp để suy ra (16).

Với mọi họ $\lambda = (\lambda_{ij})$ các phần tử của $\mathbf{A}$, với $1 \leq j < i \leq n$, và với mọi phép hoán vị $\sigma \in \mathfrak{S}_n$, ta đặt

$$
\varepsilon_\sigma(\lambda) = \prod_{i > j,\ \sigma^{-1}(i) < \sigma^{-1}(j)} \lambda_{ij} = \prod_{i < j,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)}.
$$

Hãy chú ý rằng, khi $\mathbf{A} = \mathbf{Z}$ và $\lambda_{ij} = -1$ đối với mọi cặp có thứ tự $(i, j)$ sao cho $1 \leq j < i \leq n$, thì $\varepsilon_\sigma(\lambda)$ chỉ là dấu $\varepsilon_\sigma$ của phép hoán vị $\sigma$ (I, § 5, no. 7).

#### Bổ đề 3 {#alg-iii-s4-lem-3 .statement}

*Cho $\mathbf{A}$ là một vành giao hoán, $\mathbf{E}$ là một $\mathbf{A}$-đại số, $(x_i)_{1 \leq i \leq n}$ là một dãy hữu hạn các phần tử của $\mathbf{E}$ và giả sử rằng, với mọi cặp có thứ tự $(i, j)$ của các số nguyên sao cho $1 \leq j < i \leq n$,*

$$
x_i x_j = \lambda_{ij} x_j x_i \quad \text{với } \lambda_{ij} \in \mathbf{A}.
$$

*Khi đó, với mọi phép hoán vị $\sigma \in \mathfrak{S}_n$,*

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \varepsilon_\sigma(\lambda) x_1 x_2 \cdots x_n.
$$

Bổ đề là tầm thường khi $n = 1$ và $n = 2$; ta chứng minh bằng quy nạp theo $n$ với $n \geq 3$. Nếu $\sigma(n) = n$, quan hệ (19) suy ra từ giả thiết quy nạp. Giả sử do đó rằng $\sigma(n) = k, k \neq n$, và hãy để $\tau$ là phép hoán vị của $\{1, n\}$ được xác định bởi

$$
\begin{cases}
\tau(i) = i & \text{với } i < k \\
\tau(i) = i + 1 & \text{với } k \leq i < n \\
\tau(n) = k.
\end{cases}
$$

### 7. TÍCH TENXƠ CỦA CÁC ĐẠI SỐ PHÂN BẬC ĐỐI VỚI CÁC HỆ SỐ GIAO HOÁN

#### Định nghĩa 6 {#alg-iii-s4-def-6 .statement}

*Cho* $(\Delta_i)_{i \in I}$ *là một họ hữu hạn các vị nhóm giao hoán viết theo phép cộng. Một hệ các hệ số giao hoán trên các* $\Delta_i$ *với giá trị trong một vành giao hoán* $\mathbf{A}$ *là một hệ các ánh xạ* $\varepsilon_{ij}: \Delta_i \times \Delta_j \to \mathbf{A}$, *trong đó* $i \in I$, $j \in I$, $i \neq j$ *thỏa mãn các điều kiện sau*:

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

*với mọi* $\alpha_i, \alpha'_i$ *trong* $\Delta_i$, $\beta_j, \beta'_j$ *trong* $\Delta_j$.

Nếu I được cho một thứ tự toàn phần và các $\Delta_i$ là các nhóm, thì một hệ các hệ số giao hoán được xác định trên các $\Delta_i$ bằng cách, với mỗi cặp có thứ tự $(i, j)$ sao cho $i < j$, lấy một ánh xạ $\mathbf{Z}$-*song tuyến tính* tùy ý của $\Delta_i \times \Delta_j$ vào $\mathbf{Z}$-*môđun* (*nhân*) $\mathbf{A}^*$ của các phần tử *khả nghịch* của vành $\mathbf{A}$ và rồi viết

$$
\varepsilon_{ji}(\beta_j, \alpha_i) = (\varepsilon_{ij}(\alpha_i, \beta_j))^{-1}
$$

cho $i < j$.

Chú ý rằng, vì các $\varepsilon_{ij}(\alpha_i, \beta_j)$ đều khả nghịch,

$$
\varepsilon_{ij}(0, \beta_j) = \varepsilon_{ij}(\alpha_i, 0) = 1,
$$

nhờ (22) và (23).

#### Ví dụ {#alg-iii-s4-n7-exa-1 .statement}

(1) Hệ *tầm thường* các hệ số giao hoán gồm các $\varepsilon_{ij}$ sao cho $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ đối với mọi $i, j$, $\alpha_i \in \Delta_i$, $\beta_j \in \Delta_j$.

Let $\pi = \tau^{-1} \circ \sigma$; the permutation $\pi$ leaves $n$ fixed; now $\sigma = \tau \circ \pi$ and therefore, writing $y_i = x_{\tau(i)},\ y_{\pi(i)} = x_{\sigma(i)}$. If $i \neq n$ and $j \neq n$, the relations $\pi(i) > \pi(j)$ and $\sigma(i) > \sigma(j)$ are equivalent (since $\tau$ is a strictly increasing mapping of $\{1, n-1\}$ into $\{1, n\}$). For $i \neq n, j \neq n$ and $\sigma(i) > \sigma(j)$,

$$
y_{\pi(i)} y_{\pi(j)} = x_{\sigma(i)} x_{\sigma(j)} = \lambda_{\sigma(i),\ \sigma(j)} x_{\sigma(j)} x_{\sigma(i)} = \lambda_{\sigma(i),\ \sigma(j)} y_{\pi(j)} y_{\pi(i)}
$$

do đó, theo giả thiết quy nạp (dùng thực tế rằng $\pi(n) = n$):

$$
y_{\pi(1)} y_{\pi(2)} \cdots y_{\pi(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) y_1 y_2 \cdots y_n
$$

tức là

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) x_{\tau(1)} \cdots x_{\tau(n)}.
$$

Khi đó

$$
x_{\tau(1)} \cdots x_{\tau(n)} = x_1 \cdots x_{k-1} x_{k+1} \cdots x_n x_k
$$

và điều này, theo Bổ đề 1, bằng

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

điều này hoàn tất chứng minh của Bổ đề 3.

==========

(2) Nếu ta lấy $\mathbf{A} = \mathbf{Z}$ và $\Delta_i = \mathbf{Z}$ với mọi $i \in I$, thì thu được một hệ các nhân tử giao hoán bằng cách lấy $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$. Chú ý rằng số này chỉ phụ thuộc vào tính chẵn lẻ của $\alpha_i$ và $\beta_j$ và do đó các $\varepsilon_{ij}$ có thể được xem như là các nhân tử giao hoán khi một số $\Delta_i$ bằng $\mathbf{Z}/2\mathbf{Z}$ và các $\Delta_i$ khác bằng $\mathbf{Z}$.

Hai ví dụ này là những trường hợp thường gặp nhất trong các ứng dụng.

#### Mệnh đề 10 {#alg-iii-s4-prop-10 .statement}

Cho $\mathbf{A}$ là một vành giao hoán và $(\Delta_i)_{i \in I}$ là một họ hữu hạn các monoid giao hoán viết theo phép cộng; với mỗi $i \in I$ cho $E_i$ là một $\mathbf{A}$-đại số phân bậc kiểu $\Delta_i$. Sau cùng, cho $(\varepsilon_{ij})$ là một hệ các nhân tử giao hoán trên các $\Delta_i$ lấy giá trị trong $\mathbf{A}$. Khi đó tồn tại một $\mathbf{A}$-đại số phân bậc $E$ kiểu $\Delta = \prod_{i \in I} \Delta_i$ và với mỗi $i \in I$ một đồng cấu đại số $h_i : E_i \to E$, có các tính chất sau:

(i) *Nếu $\phi_i : \Delta_i \to \Delta$ là đồng cấu chính tắc, thì $h_i$ là một đồng cấu phân bậc* (II, § 11, no. 2), nói cách khác, $h_i(E_i^{\alpha_i}) \subset E^{\phi_i(\alpha_i)}$, trong đó $(E_i^{\alpha_i})$ và $(E^{\alpha})$ ký hiệu các phân bậc tương ứng trên $E_i$ và $E$.

(ii) *Nếu $i \neq j$ và $x_i$ (resp. $x_j$) là một phần tử thuần nhất của $E_i$ (resp. $E_j$) có bậc $\alpha_i \in \Delta_i$ (resp. $\beta_j \in \Delta_j$), thì*

$$
h_i(x_i) h_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) h_j(x_j) h_i(x_i).
$$

(iii) *Với mọi $\mathbf{A}$-đại số $F$ và mọi hệ các đồng cấu $f_i : E_i \to F$ thỏa mãn các điều kiện*

$$
f_i(x_i) f_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) f_j(x_j) f_i(x_i),
$$

*trong đó $i, j, x_i, x_j, \alpha_i, \beta_j$ như trong (ii), thì tồn tại một và chỉ một đồng cấu đại số $f : E \to F$ sao cho $f_i = f \circ h_i$ với mọi $i \in I$. Hơn nữa môđun nền của $E$ là tích tenxơ $\bigotimes_{i \in I} E_i$.*

Xét $\mathbf{A}\text{-module}$ $E = \bigotimes_{i \in I} E_i$; nó được đồng nhất với tổng trực tiếp của các môđun con $E^{\alpha}$, trong đó, với mỗi $\alpha = (\alpha_i) \in \Delta$, ta viết $E^{\alpha} = \bigotimes_{i \in I} E_i^{\alpha_i}$; do đó các $E^{\alpha}$ tạo thành một phân bậc kiểu $\Delta$ trên $\mathbf{A}$-môđun $E$. Ta sẽ định nghĩa trên $E$ một *cấu trúc đại số trên $\mathbf{A}$ có phân bậc* kiểu $\Delta$. Để làm điều đó, hãy cho $I$ được trang bị một thứ tự toàn phần; với mọi cặp có thứ tự các phần tử $\alpha = (\alpha_i), \beta = (\beta_i)$ của $\Delta$, trước hết ta phải định nghĩa một ánh xạ $\mathbf{A}$-song tuyến tính từ $E^{\alpha} \times E^{\beta}$ vào $E^{\alpha + \beta}$, hoặc tương đương một ánh xạ $\mathbf{A}$-tuyến tính $m_{\alpha \beta}$ từ $E^{\alpha} \otimes_{\mathbf{A}} E^{\beta}$ vào $E^{\alpha + \beta}$. Ta sẽ định nghĩa $m_{\alpha \beta}$ bởi điều kiện

$$
m_{\alpha \beta} \left( \left( \bigotimes_{i \in I} x_i \right) \otimes \left( \bigotimes_{i \in I} y_i \right) \right) = \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)
$$

với $x_i \in E_i^{\alpha_i}, y_i \in E_i^{\alpha_i}$, trong đó

$$
\varepsilon(\alpha, \beta) = \prod_{i > j} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

Vế phải của (27) hiển nhiên thuộc $E^{\alpha + \beta}$ và ánh xạ $(x_1, \ldots, x_n, y_1, \ldots, y_n) \mapsto \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)$ là $\mathbf{A}$-đa tuyến tính trên tích của các $E_i^{\alpha_i}$ và các $E_i^{\beta_i}$ ($1 \leq i \leq n$). Khi đó cần phải chứng minh rằng phép nhân được định nghĩa như vậy trên E là kết hợp; bây giờ, nếu $\gamma = (\gamma_i)$ là một phần tử thứ ba của $\Delta$ và $z_i \in E_i^{\gamma_i'}$ với $1 \leq i \leq n$, thì

$$
\left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) \left( \bigotimes_i z_i \right) = \varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) \bigotimes_i (x_i y_i z_i)
$$

$$
\left( \bigotimes_i x_i \right) \left( \left( \bigotimes_i y_i \right) \left( \bigotimes_i z_i \right) \right) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma) \bigotimes_i (x_i y_i z_i)
$$

và điều đó quy về việc kiểm tra đẳng thức

$$
\varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma).
$$

Nhưng đẳng thức sau suy ra ngay lập tức từ các quan hệ

$$
\varepsilon(\alpha + \beta, \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\beta, \gamma)
$$
$$
\varepsilon(\alpha, \beta + \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\alpha, \gamma)
$$

mà chính chúng là những hệ quả ngay lập tức của định nghĩa (28) và (22) và (23).

Nếu, với mọi $i \in I$, $e_i$ ký hiệu phần tử đơn vị của $E_i$, ta biết rằng $e_i$ là thuần nhất bậc 0 (\S 3, no. 1), do đó $e = \bigotimes_{i \in I} e_i$ là thuần nhất bậc 0 và suy ra từ (27), (28) và các quan hệ

$$
\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1
$$

rằng $e$ là phần tử đơn vị của $E$, điều đó hoàn tất việc định nghĩa trên $E$ cấu trúc đại số trên $\mathbf{A}$ có phân bậc mong muốn. Khi đó đặt $h_i(x_i) = x_i \otimes \bigotimes_{j \neq i} e_j$; để kiểm tra rằng $h_i(x_i x_i') = h_i(x_i) h_i(x_i')$ với $x_i, x_i'$ trong $E_i$, ta chỉ cần xét trường hợp $x_i$ và $x_i'$ thuần nhất và khi đó quan hệ này suy ra ngay lập tức từ (27) và các quan hệ $\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1$; các quan hệ ấy và (24) cũng chứng minh rằng các $h_i$ thỏa mãn các điều kiện (i) và (ii) của mệnh đề và rằng

$$
\bigotimes_{i \in I} x_i = \prod_{i \in I} h_i(x_i)
$$

trong đó vế phải là tích của dãy có thứ tự $(h_i(x_i))_{i \in I}$ trong E với thứ tự toàn phần đã cho trên I (I, \S 1, no. 2) (chỉ cần lập luận bằng quy nạp theo số các $x_i$ (giả sử thuần nhất) khác với các $e_i$).

Còn phải chứng minh điều kiện (iii); chú ý rằng ánh xạ

$$
(x_i)_{i \in I} \mapsto \prod_{i \in I} f_i(x_i),
$$

trong đó vế phải là tích của dãy có thứ tự $(f_i(x_i))_{i \in I}$ với thứ tự toàn phần đã cho trên $I$, là A-đa tuyến tính. Khi đó tồn tại duy nhất một ánh xạ A-tuyến tính $f : E \to F$ sao cho

$$
f\left( \bigotimes_{i \in I} x_i \right) = \prod_{i \in I} f_i(x_i).
$$

Rõ ràng $f(e)$ là phần tử đơn vị của $F$ và $f \circ h_i = f_i$; để kiểm tra rằng $f$ là một đồng cấu đại số, hay nói cách khác là $f(x)f(y) = f(xy)$ với $x, y$ trong $E$, ta có thể, nhờ tính tuyến tính, chỉ xét trường hợp $x = \bigotimes_{i \in I} x_i$ và $y = \bigotimes_{i \in I} y_i$, trong đó $x_i$ (tương ứng $y_i$) là thuần nhất bậc $\alpha_i$ (tương ứng $\beta_i$) với mọi $i \in I$. Quan hệ cần kiểm tra khi đó, theo (27), quy về

$$
\left( \prod_{i \in I} f_i(x_i) \right) \left( \prod_{i \in I} f_i(y_i) \right) = \varepsilon(\alpha, \beta) \prod_{i \in I} (f_i(x_i) f_i(y_i)).
$$

Nhưng, xét đến các quan hệ (26), đây là hệ quả của Bổ đề 2 ở no. 6.

Rõ ràng đại số $E$ và ánh xạ chính tắc $\psi : \bigotimes_{i \in I} E_i \to E$ tạo thành một nghiệm của *vấn đề ánh xạ phổ quát* (*Lý thuyết tập hợp*, IV, § 3, no. 1), trong đó $\Sigma$ là loài của cấu trúc A-đại số và các $\alpha$-ánh xạ $\prod_i f_i$ từ $\prod_i E_i$ đến một A-đại số, thỏa mãn các điều kiện (26).

Với một thứ tự toàn phần cố định trên $I$, đại số phân bậc $E$ được định nghĩa trong chứng minh của Mệnh đề 10 sẽ được gọi là *tích tenxơ $\varepsilon$-phân bậc kiểu* $\Delta$ của họ $(E_i)_{i \in I}$ các đại số phân bậc kiểu $\Delta_i$ và sẽ được ký hiệu bởi $^{\varepsilon} \bigotimes_{i \in I} E_i$ (nếu không thể có nhầm lẫn về thứ tự trên $I$); tương tự, đồng cấu $f : E \to F$ được định nghĩa trong chứng minh của Mệnh đề 10 sẽ được ký hiệu bởi $^{\varepsilon} \bigotimes_{i \in I} f_i$. Các đồng cấu $h_i$ được gọi là *chính tắc*. Ta cũng viết $^{\varepsilon} G^{\otimes n}$ khi $I = \{1, n\}$ và mọi $E_i$ đều bằng cùng một đại số $G$.

#### Nhận xét {#alg-iii-s4-n7-rem-1 .statement}

(1) Ta thu được tích tenxơ của các đại số được định nghĩa ở no. 1 (với thêm phân bậc là tích tenxơ của các phân bậc của các thừa số) bằng cách lấy $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ với mọi $i, j, \alpha_i$ và $\beta_j$.

(2) Giả sử mọi $\Delta_i$ đều bằng $\mathbf{Z}$ và viết $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$; khi đó tích tenxơ $\varepsilon$-phân bậc $^{\varepsilon} \bigotimes_{i \in I} E_i$ tương ứng với hệ số giao hoán này được gọi là tích tenxơ *lệch* của các đại số phân bậc $E_i$ kiểu $\mathbf{Z}$ và được ký hiệu bởi $^{\varepsilon} \bigotimes_{i \in I} E_i$ (hoặc $E \ ^{\varepsilon} \otimes_A F$ cho hai đại số, hoặc $^{\varepsilon} G^{\otimes n}$ thay cho $^{\varepsilon} G^{\otimes n}$).

#### Hệ quả 1 {#alg-iii-s4-prop-10-cor-1 .statement}

Theo ký hiệu của Mệnh đề 10, giả sử thêm rằng F là một đại số trên A phân bậc kiểu $\Delta$ và rằng mỗi $f_i$ là một đồng cấu đại số phân bậc tương ứng với $\phi_i : \Delta_i \to \Delta$; khi đó $f = \varepsilon \bigotimes_i f_i$ là một đồng cấu đại số phân bậc.

Điều này suy ra ngay lập tức từ định nghĩa của $f$ và thực tế rằng
$$
\sum_{i \in I} \phi_i(\alpha_i) = (\alpha_i)
$$
theo định nghĩa của các $\phi_i$.

Vì vậy thấy rằng $(E, \psi)$ cũng là một nghiệm của một bài toán ánh xạ phổ quát khác, trong đó lần này $\Sigma$ là loài cấu trúc *đại số trên A phân bậc* *kiểu* $\Delta$, các đồng cấu là các đồng cấu đại số phân bậc kiểu $\Delta$ và các ánh xạ $\alpha$ là các ánh xạ $\prod_i f_i$, trong đó, ngoài các điều kiện (26), còn giả thiết rằng $f_i$ là một đồng cấu đại số phân bậc tương ứng với $\phi_i$.

#### Hệ quả 2 {#alg-iii-s4-prop-10-cor-2 .statement}

*Cho* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *là hai họ hữu hạn của* A*-đại số, với* $E_i$ *và* $F_i$ *phân bậc kiểu* $\Delta_i$ *với mọi* $i \in I$. *Với mỗi* $i \in I$, *cho* $g_i : E_i \to F_i$ *là một đồng cấu đại số phân bậc kiểu* $\Delta_i$. *Khi đó, nếu* $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i$ *và* $h'_i : F_i \to \varepsilon \bigotimes_{i \in I} F_i$ *là các đồng cấu chính tắc, thì tồn tại một và chỉ một đồng cấu của các* A*-đại số phân bậc kiểu* $\Delta$, $g : \varepsilon \bigotimes_{i \in I} E_i \to \varepsilon \bigotimes_{i \in I} F_i$ *sao cho* $g \circ h_i = h'_i \circ g_i$ *với mọi* $i \in I$. *Hơn nữa, nếu mỗi* $g_i$ *là song ánh, thì* $g$ *cũng song ánh.*

Chỉ cần áp dụng Hệ quả 1 cho $f_i = h'_i \circ g_i$, lưu ý rằng khi đó các điều kiện (26) suy ra từ các hệ thức (25) áp dụng cho các $h'_i$.

Đồng cấu được định nghĩa trong Hệ quả 2 cũng được ký hiệu bởi $\varepsilon \bigotimes_i g_i$ (nếu không thể gây nhầm lẫn); nếu, với mỗi $i \in I$, $G_i$ là một đại số trên A phân bậc thứ ba kiểu $\Delta_i$ và $g'_i : F_i \to G_i$ là một đồng cấu đại số phân bậc, thì
$$
\left( \varepsilon \bigotimes_i g'_i \right) \circ \left( \varepsilon \bigotimes_i g_i \right) = \varepsilon \bigotimes_i (g'_i \circ g_i),
$$
như suy ra ngay lập tức từ (30).

Trong trường hợp một tích tenxơ lệch của các đại số phân bậc kiểu $\mathbf{Z}$, ta viết $\varepsilon \bigotimes_i f_i$ thay cho $\varepsilon \bigotimes_i f_i$ đối với các đồng cấu $f_i : E_i \to F_i$ của các đại số phân bậc kiểu $\mathbf{Z}$; khi $I = \{1, 2\}$, đồng cấu này cũng được ký hiệu bởi $f_1 \varepsilon \otimes f_2$; khi $I = \{1, n\}$ và mọi $E_i$ (resp. $F_i$) đều bằng nhau và mọi $f_i$ đều bằng cùng một đồng cấu $f$, ta viết $\varepsilon f^{\otimes n}$.

#### Nhận xét {#alg-iii-s4-n7-rem-2 .statement}

Trong chứng minh của Mệnh đề 10, đã dùng một thứ tự toàn phần trên $I$ để định nghĩa một *cấu trúc đại số* trên tích tenxơ $\bigotimes_{i \in I} E_i$ của các A-môđun

E_i. Nếu thứ tự trên I bị thay đổi, sẽ phát sinh một cấu trúc nhân khác trên $\bigotimes_{i \in I} E_i$, nhưng đại số mới thu được như vậy là *đẳng cấu* chính tắc với đại số ở trên, vì cả hai đều là nghiệm của cùng một bài toán ánh xạ phổ quát. Chẳng hạn, khi $I = \{1, 2\}$, đẳng cấu chính tắc của đại số $E_1 \overset{\varepsilon}{\otimes}_A E_2$ lên đại số $E_2 \overset{\varepsilon}{\otimes}_A E_1$ gửi $x_1 \otimes x_2$ thành $\varepsilon_{2,1}(\alpha, \beta)x_2 \otimes x_1$, trong đó $x_1$ thuần nhất bậc $\alpha$ và $x_2$ thuần nhất bậc $\beta$.

Cho J là một tập con của I và, với mỗi $i \in J$, xét đồng cấu chính tắc $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i = E$. Nhờ các quan hệ (25), một đồng cấu chính tắc $h : E' = \varepsilon \bigotimes_{i \in J} E_i \to E$ được suy ra một cách chính tắc (theo Mệnh đề 10) từ các đồng cấu này, sao cho, với mọi $i \in J$, $h'_i = h \circ h_i$, trong đó $h'_i$ là đồng cấu chính tắc $E_i \to E'$. Lấy thứ tự toàn phần trên J cảm sinh bởi thứ tự đã chọn trên I, ta được

$$
h\left( \bigotimes_{i \in J} x_i \right) = \prod_{i \in I} h_i(x_i) = \bigotimes_{i \in I} x'_i
$$

trong đó số hạng ở giữa là tích của *dãy có thứ tự* $(h_i(x_i))_{i \in J}$ và trong số hạng bên phải, $x'_i = x_i$ với $i \in J$, $x'_i = e_i$ với $i \notin J$.

#### Mệnh đề 11 {#alg-iii-s4-prop-11 .statement}

("tính kết hợp" của tích tenxơ $\varepsilon$). *Trong ký hiệu của Mệnh đề 10, cho* $(J_\lambda)_{\lambda \in L}$ *là một phân hoạch của I và viết* $\Delta'_\lambda = \prod_{i \in J_\lambda} \Delta_i$ *với mọi* $\lambda \in L$. *Cho* $E'_\lambda$ *là một tích tenxơ $\varepsilon$ phân bậc kiểu* $\Delta'_\lambda$ *của họ* $(E_i)_{i \in J_\lambda}$ *với một thứ tự toàn phần nào đó được chọn trên* $J_\lambda$. *Mặt khác, với* $\lambda, \mu$ *trong* $L$ *và* $\lambda \neq \mu$, *ta viết, với* $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$, $\beta'_\mu = (\beta_j)_{j \in J_\mu}$,

$$
\varepsilon'_{\lambda \mu}(\alpha'_\lambda, \beta'_\mu) = \prod_{i \in J_\lambda, j \in J_\mu} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

*Khi đó* $(\varepsilon'_{\lambda \mu})$ *là một hệ các hệ số giao hoán trên các* $\Delta'_\lambda$ *với giá trị trong* $A$ *và tồn tại một và chỉ một đồng cấu của các đại số phân bậc kiểu* $\Delta$, $v : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$, *sao cho*

$$
v\left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*với mọi* $(x_i) \in \prod_{i \in I} E_i$, *miễn là lấy thứ tự toàn phần trên I sao cho nó cảm sinh trên mỗi* $J_\lambda$ *thứ tự toàn phần đã chọn, và sao cho, với* $\lambda < \mu$ *trong* $L$, $i \in J_\lambda$ *và* $j \in J_\mu$, $i < j$.

Việc $\varepsilon'_{\lambda \mu}$ tạo thành một hệ các hệ số giao hoán là tầm thường. Cho $h_{i,\lambda} : E_i \to E'_\lambda$, $h'_\lambda : E'_\lambda \to \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$ *là các đồng cấu chính tắc* (với $\lambda \in L$, $i \in J_\lambda$) *và đặt* $h''_i = h'_\lambda \circ h_{i,\lambda}$; *do tính duy nhất của* nghiệm của một bài toán ánh xạ phổ quát, chỉ cần chứng minh rằng $\varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$ và các $h''_i$ thỏa mãn các điều kiện của Mệnh đề 10. Nay, với mọi $\lambda \in L$, cho $f'_\lambda : E'_\lambda \to F$ là đồng cấu đại số duy nhất sao cho $f'_\lambda \circ h_{i,\lambda} = f_i$ với mọi $i \in J_\lambda$. Ta chứng minh rằng, với $\lambda \neq \mu$, $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}, \beta'_\mu = (\beta_j)_{j \in J_\mu}$,

$$
f'_\lambda(x'_\lambda)f'_\mu(x'_\mu) = \varepsilon'_{\lambda\mu}(\alpha'_\lambda, \beta'_\mu)f'_\mu(x'_\mu)f'_\lambda(x'_\lambda)
$$

với $x'_\lambda \in E'_\lambda$ (resp. $x'_\mu \in E'_\mu$) thuần nhất bậc $\alpha'_\lambda$ (resp. $\beta'_\mu$); theo tính tuyến tính, chỉ cần kiểm tra điều này khi $x'_\mu = \bigotimes_{i \in J_\lambda} x_i, x'_\mu = \bigotimes_{j \in J_\mu} x_j, x_i$ (resp. $x_j$) là thuần nhất bậc $\alpha_i$ (resp. $\beta_j$) trong $E_i$ (resp. $E_j$) với $i \in J_\lambda, j \in J_\mu$. Nhưng điều này suy ra từ công thức (30) định nghĩa các $f'_\lambda$ và Bổ đề 3 của no. 6, xét đến giả thiết (26) và định nghĩa (32). Do đó tồn tại duy nhất một đồng cấu đại số $f : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to F$ sao cho $f \circ h'_\lambda = f'_\lambda$ với mọi $\lambda \in L$; suy ra $f \circ h''_i = f_i$ với mọi $i \in I$ và tính duy nhất của $f$ là tầm thường.

### 8. TÍCH TENXƠ CỦA CÁC ĐẠI SỐ PHÂN BẬC CÙNG KIỂU

Giả sử các giả thiết của no. 7, Mệnh đề 10 đều đúng, và giả sử thêm rằng mọi $\Delta_i$ đều bằng cùng một *monoid giao hoán* $\Delta_0$; khi đó ta có thể xét trên tích $\varepsilon$-tenxơ $\varepsilon \bigotimes_{i \in I} E_i$ *phân bậc toàn phần* kiểu $\Delta_0$, liên kết với phân bậc kiểu $\Delta = \Delta_0^I$ trên đại số này (II, § 11, no. 1); ta sẽ gọi $\varepsilon \bigotimes_{i \in I} E_i$, với phân bậc này, là một *tích $\varepsilon$-tenxơ phân bậc kiểu* $\Delta_0$ của họ $(E_i)_{i \in I}$ các đại số phân bậc kiểu $\Delta_0$.

Luôn giữ ký hiệu của Mệnh đề 10 của no. 7, giả sử rằng $F$ cũng là một *đại số A phân bậc kiểu* $\Delta_0$ và rằng các $f_i$ là *đồng cấu của các đại số phân bậc kiểu* $\Delta_0$. Khi đó $f : \varepsilon \bigotimes_{i \in I} E_i \to F$ cũng là một *đồng cấu của các đại số phân bậc kiểu* $\Delta_0$: vì từ công thức (30) (no. 7) suy ra rằng nếu $x_i$ thuần nhất và có bậc $\alpha_i \in \Delta_0$, thì $\bigotimes_{i \in I} x_i$ và $\prod_{i \in I} f_i(x_i)$ đều thuần nhất bậc $\sum_{i \in I} \alpha_i \in \Delta_0$.

It can therefore be said that $\varepsilon \bigotimes_{i \in I} E_i$, với tổng phân bậc kiểu $\Delta_0$, cấu thành, cùng với ánh xạ chính tắc $\psi$, một nghiệm của một bài toán ánh xạ phổ quát thứ ba, trong đó $\Sigma$ là loài của *đại số trên A phân bậc kiểu* $\Delta_0$, các đồng cấu là các đồng cấu của các đại số phân bậc kiểu $\Delta_0$ và các ánh xạ $\alpha$ là các ánh xạ $\prod_i f_i$, trong đó, ngoài các điều kiện (26) (của no. 7), giả thiết rằng mỗi $f_i$ là một đồng cấu của các đại số phân bậc kiểu $\Delta_0$.

Với mọi tập con J của I, đồng cấu chính tắc $\varepsilon \bigotimes_{i \in J} E_i \to \varepsilon \bigotimes_{i \in I} E_i$ (no. 7) thực ra là một đồng cấu của các đại số phân bậc kiểu $\Delta_0$, như suy ra ngay lập tức từ trên.

#### Mệnh đề 12 {#alg-iii-s4-prop-12 .statement}

("tính kết hợp" của tích tenxơ $\varepsilon$ của các đại số phân bậc cùng kiểu). *Với ký hiệu của Mệnh đề 10 ở no. 7, giả sử rằng mọi $\Delta_i$ đều bằng cùng một monoid $\Delta_0$; cho $(J_\lambda)_{\lambda \in L}$ là một phân hoạch của I. Với ký hiệu của Mệnh đề 11 ở no. 7, giả sử rằng vế phải của công thức (32) (no. 7) chỉ phụ thuộc vào các tổng $\alpha''_\lambda = \sum_{i \in J_\lambda} \alpha_i, \beta''_\mu = \sum_{j \in J_\mu} \beta_j$, với mọi cặp có thứ tự $(\lambda, \mu)$ của các chỉ số phân biệt, mọi $\alpha'_\lambda \in \Delta'_\lambda$ và mọi $\beta'_\mu \in \Delta'_\mu$; ký hiệu vế phải của (32) là $\varepsilon''_{\lambda \mu}(\alpha''_\lambda, \beta''_\mu)$. *Khi đó $(\varepsilon''_{\lambda \mu})$ là một hệ thừa số giao hoán trên họ $(\Delta''_\lambda)_{\lambda \in L}$, trong đó $\Delta''_\lambda = \Delta_0$ với mọi $\lambda \in L$. *Nếu $E''_\lambda$ là tích tenxơ $\varepsilon$ phân bậc kiểu $\Delta_0$ của họ $(E_i)_{i \in J_\lambda}$, thì tồn tại một và chỉ một đẳng cấu của các đại số phân bậc kiểu $\Delta_0$, $w : \varepsilon'' \bigotimes_{\lambda \in L} E''_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$, sao cho

$$
w \left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*miễn là các thứ tự toàn phần được chọn trên các $J_\lambda$ và trên I như mô tả ở no. 7, Mệnh đề 11.*

Theo giả thiết, với $\gamma, \delta$ trong $\Delta_0$, $\varepsilon''_{\lambda \mu}(\gamma, \delta) = \varepsilon_{i_0 j_0}(\gamma, \delta)$ với một $i_0 \in J_\lambda$ nào đó và một $j_0 \in J_\mu$ nào đó, như thấy bằng cách xét các phần tử $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$ và $\beta'_\mu = (\beta_j)_{j \in J_\mu}$ sao cho $\alpha_{i_0} = \gamma, \alpha_i = 0$ với $i \neq i_0$, $\beta_{j_0} = \delta, \beta_j = 0$ với $j \neq j_0$; suy ra ngay lập tức rằng các $\varepsilon''_{\lambda \mu}$ tạo thành một hệ thừa số giao hoán. Phần còn lại của chứng minh khi đó tương tự như của Mệnh đề 11 (no. 7) và để lại cho người đọc.

Chú ý rằng các giả thiết bổ sung của Mệnh đề 12 được thỏa mãn khi $\Delta_0 = \mathbf{Z}$ và rằng $(\varepsilon_{ij})$ hoặc là hệ thừa số tầm thường $(\varepsilon_{ij}(\alpha_i, \beta_j)) = 1$ với mọi $i, j$, hoặc là hệ thừa số được xác định bởi $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$; trong trường hợp sau, vế phải của công thức (32) bằng $(-1)^\gamma$, trong đó

$$
\gamma = \sum_{i \in J_\lambda, j \in J_\mu} \alpha_i \beta_j = \left( \sum_{i \in J_\lambda} \alpha_i \right) \left( \sum_{j \in J_\mu} \beta_j \right).
$$

#### Nhận xét {#alg-iii-s4-n8-rem-1 .statement}

(1) Cho I là một tập chỉ số vô hạn và $\Delta_0$ là một monoid giao hoán; cho $(\Delta_i)_{i \in I}$ ký hiệu họ sao cho $\Delta_i = \Delta_0$ với mọi $i$ và giả sử với mọi cặp có thứ tự gồm các chỉ số phân biệt $(i, j)$ của I đã cho một ánh xạ $\varepsilon_{ij} : \Delta_i \times \Delta_j \to A$ thỏa mãn các điều kiện (22), (23) và (24) (no. 7); điều này cũng sẽ được gọi là một *hệ các hệ số giao hoán trên họ* $(\Delta_i)$. Xét một họ $(E_i)_{i \in I}$ các A-đại số phân bậc kiểu $\Delta_0$; với mỗi tập con hữu hạn J của I, ký hiệu $E_J$ một *tích tenxơ $\varepsilon$ phân bậc kiểu* $\Delta_0$ của họ con $(E_i)_{i \in J}$ (với một lựa chọn tùy ý của một thứ tự toàn phần trên J). Nếu J, J' là hai tập con hữu hạn của I sao cho $J \subset J'$, một đồng cấu chính tắc của các đại số phân bậc kiểu $\Delta_0$, h_{J'J}: E_J \to E_{J'}, đã được định nghĩa ở trên và các tính chất duy nhất của những đồng cấu này cho thấy ngay lập tức rằng nếu $J \subset J' \subset J''$ là ba tập con hữu hạn của I, thì h_{J''J} = h_{J'J'} \circ h_{J'J}. Do đó có một hệ trực tiếp (E_J, h_{J'J}) của các đại số phân bậc kiểu $\Delta_0$ (\S 3, no. 3), mà tập chỉ số của nó là tập có hướng bên phải $\mathfrak{F}(I)$ của các tập con hữu hạn của I. Đại số phân bậc kiểu $\Delta_0$, giới hạn trực tiếp của hệ trực tiếp này (\S 3, no. 3), được gọi là một *tích tenxơ $\varepsilon$ phân bậc kiểu* $\Delta_0$ của họ $(E_i)_{i \in I}$; nó cũng được ký hiệu bởi $\varepsilon \bigotimes_{i \in I} E_i$. Khi mọi $\Delta_i$ đều bằng $\mathbf{Z}$ và $\varepsilon_{ij}(a_i, \beta_j) = (-1)^{\alpha_i \beta_j}$, tích tenxơ $\varepsilon \bigotimes_{i \in I} E_i$ cũng được gọi là *tích tenxơ xiên* của họ $(E_i)_{i \in I}$ và được ký hiệu bởi $g \bigotimes_{i \in I} E_i$. Chúng tôi xin để cho bạn đọc nhiệm vụ phát biểu và chứng minh mệnh đề khái quát hóa Mệnh đề 10 của no. 7 sang trường hợp I vô hạn, cũng như Mệnh đề 8 của no. 5 khái quát hóa Mệnh đề 5 của no. 2 sang trường hợp I vô hạn. Chú ý rằng A-môđun nền của $\varepsilon \bigotimes_{i \in I} E_i$ là cùng một với A-môđun nền của tích tenxơ (không phân bậc) của họ $(E_i)_{i \in I}$ các đại số không phân bậc được định nghĩa ở no. 5.

(2) Cho E là một A-đại số phân bậc kiểu $\Delta_0$ (trong đó $\Delta_0$ là một monoid giao hoán) và $\rho : A \to B$ một đồng cấu vành; sự phân bậc trên $\rho^*(E)$ (II, \S 11, no. 5) trùng với sự phân bậc trên tích tenxơ phân bậc $B \otimes_A E$, trong đó B có phân bậc tầm thường.

### 9. ĐẠI SỐ PHẢN GIAO HOÁN VÀ ĐẠI SỐ LUÂN PHIÊN

#### Định nghĩa 7 {#alg-iii-s4-def-7 .statement}

*Một A-đại số phân bậc E kiểu $\mathbf{Z}$ được gọi là phản giao hoán nếu với mọi phần tử thuần nhất khác không x, y của E*

$$
xy = (-1)^{\deg(x)\deg(y)} yx.
$$

*Đại số E được gọi là luân phiên nếu nó phản giao hoán và đồng thời $x^2 = 0$ với mọi phần tử thuần nhất $x \in E$ có bậc lẻ.*

#### Nhận xét {#alg-iii-s4-n9-rem-1 .statement}

(1) Cho $E^+$ là đại số con phân bậc của E là tổng trực tiếp của các $E_{2n}$ ($n \in \mathbf{Z}$); suy ra từ Định nghĩa 7 rằng nếu E phản giao hoán, thì $E^+$ là một *đại số con được chứa trong tâm của* E (và do đó giao hoán).

(2) Giả sử 2 không phải là một ước của 0 trong E; khi đó nếu E phản giao hoán thì E luân phiên, vì với $x \in E$ thuần nhất và có bậc lẻ, $x^2 = -x^2$ theo (36), do đó $2x^2 = 0$ và $x^2 = 0$ nhờ giả thiết.

(3) Chúng ta sẽ nghiên cứu chi tiết trong \S 7 những ví dụ quan trọng của các đại số luân phiên.

#### Bổ đề 4 {#alg-iii-s4-lem-4 .statement}

*Cho E là một đại số phân bậc kiểu $\mathbf{Z}$ và S là một tập các phần tử thuần nhất $\neq 0$; tập F các phần tử của E sao cho mọi thành phần thuần nhất $x \neq 0$ của chúng đều thỏa mãn quan hệ (36) với mọi $y \in S$ là một đại số con phân bậc của E.*

Chỉ cần nhận xét rằng: (1) nếu $x', x''$ là hai phần tử thuần nhất cùng bậc $p$, $y$ là một phần tử thuần nhất bậc $q$ và $x'y = (-1)^{pq}yx'$, $x''y = (-1)^{pq}yx''$, thì cũng có $(x' + x'')y = (-1)^{pq}y(x' + x'')$; (2) nếu $x', x''$ là hai phần tử thuần nhất có bậc tương ứng $p', p''$, $y$ là một phần tử thuần nhất bậc $q$ và $x'y = (-1)^{p'q}yx'$, $x''y = (-1)^{p''q}yx''$, thì
$$
(x'x'')y = (-1)^{(p'+p'')q}y(x'x'').
$$

#### Mệnh đề 13 {#alg-iii-s4-prop-13 .statement}

*Cho E là một A-đại số phân bậc kiểu $\mathbf{Z}$ và S là một hệ sinh của đại số E gồm các phần tử thuần nhất $\neq 0$; để E phản giao hoán (resp. phản xứng), điều kiện cần và đủ là (36) đúng với mọi $x \in S$ và $y \in S$ (resp. điều kiện này đúng và thêm nữa $x^2 = 0$ với mọi $x$ thuần nhất bậc lẻ thuộc S).*

Trước hết ta xét trường hợp các đại số phản giao hoán. Theo Bổ đề 4, đại số con F gồm các phần tử mà mọi thành phần thuần nhất $x \neq 0$ của chúng đều thỏa mãn (36) với mọi $y \in S$, chứa mọi phần tử của S và do đó $F = E$. Nếu bây giờ $F'$ cũng được hiểu là đại số con của E gồm các phần tử mà mọi thành phần thuần nhất $x \neq 0$ của chúng đều thỏa mãn (36) với mọi phần tử thuần nhất $y \neq 0$, thì từ trên suy ra $F'$ chứa mọi phần tử của S và do đó $F' = E$, điều đó hoàn thành chứng minh của mệnh đề trong trường hợp này.

Để chứng minh mệnh đề trong trường hợp các đại số phản xứng, có thể giả sử rằng E đã là phản giao hoán; khi đó ngay lập tức mọi phần tử thuần nhất bậc lẻ của E đều có dạng $\sum_i z_ix_i$, trong đó $z_i \in E^+$ và $x_i \in S$ có bậc lẻ (dùng sự kiện là $E^+$ được chứa trong tâm của E); suy ra $\left( \sum_i z_ix_i \right)^2 = \sum_i z_i^2x_i^2 + \sum_{i<j} z_i z_j (x_ix_j + x_jx_i) = 0$ vì $x_i^2 = 0$ theo giả thiết và $x_ix_j + x_jx_i = 0$ theo (36).

#### Mệnh đề 14 {#alg-iii-s4-prop-14 .statement}

*Cho E và F là hai A-đại số phân bậc kiểu $\mathbf{Z}$, đều phản giao hoán (resp. phản xứng). Khi đó tích tenxơ phản xứng $E^g \otimes_A F$ (no. 7) là một đại số phản giao hoán (resp. phản xứng).*

Một hệ sinh của $E^g \otimes_A F$ gồm các $x \otimes y$, trong đó $x$ (resp. $y$) là một phần tử thuần nhất $\neq 0$ của E (resp. F). Xét hai phần tử như vậy $x \otimes y, x' \otimes y'$, với $\deg(x) = p, \deg(y) = q, \deg(x') = p', \deg(y') = q'$, nên $x \otimes y$ có bậc $p + q$ và $x' \otimes y'$ có bậc $p' + q'$. Khi đó theo định nghĩa (no. 7, công thức (27)) và nhờ (36),
$$
\begin{align*}
(x \otimes y)(x' \otimes y') &= (-1)^{qp'}(xx') \otimes (yy') \\
(x' \otimes y')(x \otimes y) &= (-1)^{pq'}(x'x) \otimes (y'y) \\
&= (-1)^{pq'+pp'+qq'}(xx') \otimes (yy')
\end{align*}
$$
và tiêu chuẩn của Mệnh đề 13 cho thấy $E^g \otimes_A F$ là phản giao hoán vì $pq' + pp' + qq' - qp' \equiv (p + q)(p' + q')$ (mod. 2). Nếu thêm nữa E và F là phản xứng và $p + q$ là lẻ, thì một trong các số $p, q$ tất yếu là lẻ, do đó $(x \otimes y)^2 = \pm (x^2) \otimes (y^2) = 0$ và Mệnh đề 13 cho thấy $E^g \otimes_A F$ là phản xứng.

#### Hệ quả {#alg-iii-s4-n9-cor-1 .statement}

*Cho E là một A-đại số phân bậc kiểu $\mathbf{Z}$ phản giao hoán* (resp. *phản xứng*). *Khi đó với mọi đồng cấu vành $\rho : A \to B$, A-đại số phân bậc B $\rho^*(E)$ (no. 8, *Nhận xét 2*) *là phản giao hoán* (resp. *phản xứng*).

Vành B với cách phân bậc tầm thường có thể được xem như một A-đại số phản xứng và $\rho^*(E) = E^g \otimes_A B$, do đó có thể áp dụng Mệnh đề 14.

#### Nhận xét {#alg-iii-s4-n9-rem-2 .statement}

Cho E là một đại số trên A phản giao hoán phân bậc kiểu $\mathbf{Z}$. Khi đó ánh xạ A-tuyến tính của $E \otimes_A E$ vào E được xác định bởi phép nhân của E ($\S 1$, no. 3) là một đồng cấu của đại số trên A phân bậc $E^g \otimes_A E$ vào E, vì theo ký hiệu của Mệnh đề 14, trong đại số E,
$$
(xy)(x'y') = (-1)^{qp'}(xx')(yy').
$$

### Bài tập {#alg-iii-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
