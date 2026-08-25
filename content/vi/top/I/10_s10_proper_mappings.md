---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 10
section_title: Proper mappings
lang: vi
source: top-i-iv
pdf_pages: 0103-0113, 0156-0161
extraction: ocr
subsections:
    - "no": 1
      title: PROPER MAPPINGS
      page: 0
      pdf_page: 103
    - "no": 2
      title: CHARACTERIZATION OF PROPER MAPPINGS BY COMPACTNESS PROPERTIES
      page: 0
      pdf_page: 107
    - "no": 3
      title: PROPER MAPPINGS INTO LOCALLY COMPACT SPACES
      page: 0
      pdf_page: 110
    - "no": 4
      title: QUOTIENT SPACES OF COMPACT SPACES AND LOCALLY COMPACT SPACES
      page: 0
      pdf_page: 111
statements: 30
exercises: 20
content_sha256: b58ddae76ab4d9629ee0b452f9a7ac0648d8395a6e3377df225f6bc9cdf3c6e1
translated_from: content/en/top/I/10_s10_proper_mappings.md
source_content_sha256: dbc7fb11c2caffb7665f50d824927c81bc19d0007face4b58efe12f172f6eb6d
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-ad2f2242
glossary_version: 34
glossary_terms_sha256: 7e9fcbaaaa277b8e2319816361192488f950ee59298e5de4e6ad988037900f5e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 10. ÁNH XẠ THỰC SỰ

*Trong tiết này, ta ký hiệu bởi $ \iota_X $ ánh xạ đồng nhất của một tập hợp $ X $ lên chính nó.*

### 1. ÁNH XẠ THỰC SỰ

Nếu $ f : X \to Y $ và $ f' : X' \to Y' $ là hai ánh xạ *liên tục đóng*, tích $ f \times f' : X \times X' \to Y \times Y' $ không nhất thiết là một ánh xạ đóng, ngay cả khi $ f $ có dạng $ \iota_X $.

#### Ví dụ {#top-i-s10-n1-exa-1 .statement}

Mọi ánh xạ hằng vào một không gian Hausdorff đều đóng. Nhưng nếu $ f $ là ánh xạ hằng $ Q \to 0 $, thì $ f \times \iota_Q $ là ánh xạ $ (x, y) \to (0, y) $ của $ Q^2 $ vào $ Q^2 $, do đó nó là phép chiếu thứ hai và không đóng (\S 4, no. 2, Nhận xét 1).

#### Định nghĩa 1 {#top-i-s10-def-1 .statement}

*Cho $ f $ là một ánh xạ của một không gian tôpô $ X $ vào một không gian tôpô $ Y $. Ta nói $ f $ là thực sự nếu $ f $ liên tục và nếu ánh xạ $ f \times \iota_Z : X \times Z \to Y \times Z $ là đóng, với mọi không gian tôpô $ Z $.*

Ta sẽ đưa ra các đặc trưng khác của các ánh xạ thực sự trong no. 2 và 3.

Nếu trong Định nghĩa 1 ta lấy không gian $ Z $ gồm một điểm duy nhất, ta thấy rằng:

#### Mệnh đề 1 {#top-i-s10-prop-1 .statement}

*Mọi ánh xạ thực sự đều đóng.*

#### Mệnh đề 2 {#top-i-s10-prop-2 .statement}

*Cho $ f : X \to Y $ là một đơn ánh liên tục. Khi đó ba mệnh đề sau là tương đương:*
a) $ f $ là thực sự.
b) $ f $ là đóng.
c) $ f $ là một đồng phôi của $ X $ lên một tập con đóng của $ Y $.

Ta vừa thấy rằng a) kéo theo b). Vì quan hệ tương đương $ f(x) = f(x') $ là quan hệ đẳng thức, không gian thương của $ X $ đối với quan hệ này có thể được đồng nhất với $ X $; do đó b) kéo theo c) theo lý do của § 5, no. 2, Mệnh đề 3. Cuối cùng, nếu c) được thỏa mãn thì $ f \times \iota_Z $ là một đồng phôi của $ X \times Z $ lên một không gian con đóng của $ Y \times Z $ và vì thế là một ánh xạ đóng; do đó c) kéo theo a).

#### Mệnh đề 3 {#top-i-s10-prop-3 .statement}

*Cho $ f : X \to Y $ là một ánh xạ liên tục. Nếu $ T $ là một tập con bất kỳ của $ Y $, gọi $ f_T $ là ánh xạ $ \overline{f}^{-1}(T) \to T $ trùng với $ f $ trên $ \overline{f}^{-1}(T) $.*

a) *Nếu $ f $ là thực sự thì $ f_T $ cũng là thực sự.*
b) *Cho $ (T(i))_{i \in I} $ là một họ các tập con của $ Y $ mà các phần trong của chúng phủ $ Y $, hoặc là một phủ đóng hữu hạn địa phương của $ Y $; khi đó nếu mỗi ánh xạ $ f_{T(i)} $ là thực sự thì $ f $ cũng là thực sự.*

Cho $ Z $ là một không gian tôpô. Nếu $ T $ là một tập con bất kỳ của $ Y $, ta có
$$
f_T \times \iota_Z = (f \times \iota_Z)_{T \times Z};
$$
nếu $ f $ là thực sự, thì $ f \times \iota_Z $ là đóng, do đó $ (f \times \iota_Z)_{T \times Z} $ cũng vậy [§ 5, no. 1, Mệnh đề 2 a)], do đó a) được chứng minh. Nếu bây giờ $ (T(i))_{i \in I} $ thỏa mãn một trong hai điều kiện đã nêu trong b), thì phủ $ (T(i) \times Z)_{i \in I} $ của $ Y \times Z $ có cùng tính chất đó; nếu $ f_{T(i)} $ là thực sự thì các ánh xạ
$$
(f \times \iota_Z)_{T(i) \times Z}
$$
là đóng, do đó $ f \times \iota_Z $ là đóng [§ 5, no. 1, Mệnh đề 2 b)]. Điều này hoàn thành chứng minh.

#### Mệnh đề 4 {#top-i-s10-prop-4 .statement}

*Cho $ I $ là một tập hợp hữu hạn và với mỗi $ i \in I $ cho $ f_i : X_i \to Y_i $ là một ánh xạ liên tục. Cho $ X = \prod_{i \in I} X_i, \ Y = \prod_{i \in I} Y_i, $ và cho $ f : X \to Y $* là ánh xạ tích $ (x_i) \to (f_i(x_i)) $. Khi đó:
a) *Nếu mỗi $ f_i $ là thực sự, thì $ f $ là thực sự.*
b) *Nếu $ f $ là thực sự và nếu các $ X_i $ là không rỗng, thì mỗi $ f_i $ là thực sự.*

(Trong no. 2, Định lý 1, Hệ quả 3, ta sẽ thấy rằng mệnh đề này mở rộng đến các tích vô hạn.)

Bằng quy nạp, chỉ cần xét trường hợp $ I = \{1, 2\} $.
a) Giả sử rằng $ f_1, f_2 $ là thực sự, và cho $ Z $ là một không gian tôpô; $ f_1 \times f_2 \times \iota_Z $ là hợp thành của $ \iota_{Y_1} \times f_2 \times \iota_Z $ và
$$
f_1 \times \iota_{X_2} \times \iota_Z;
$$
hai ánh xạ này là đóng theo giả thiết, do đó $ f_1 \times f_2 \times \iota_Z $ cũng là đóng [\S 5, no. 1, Mệnh đề 1 a)], do đó $ f_1 \times f_2 $ là thực sự.

b) Bây giờ giả sử $ f $ là thực sự. Cho $ F $ là một tập con đóng của $ X_2 \times Z $ và cho $ G $ là ảnh của $ F $ trong $ Y_2 \times Z $ theo ánh xạ $ f_2 \times \iota_Z $. Khi đó ảnh của $ X_1 \times F $ trong $ Y_1 \times Y_2 \times Z $ theo $ f_1 \times f_2 \times \iota_Z $ là $ f_1(X_1) \times G $. Theo giả thiết, tập này là đóng trong $ Y_1 \times Y_2 \times Z $; nếu $ X_1 \neq \emptyset $, thì $ f_1(X_1) $ không rỗng, điều này suy ra rằng $ G $ là đóng trong $ Y_2 \times Z $ (\S 4, no. 3, Hệ quả của Mệnh đề 7); do đó $ f_2 $ là thực sự. Tương tự $ f_1 $ là thực sự nếu $ X_2 \neq \emptyset $.

#### Mệnh đề 5 {#top-i-s10-prop-5 .statement}

*Cho $ f : X \to X' $ và $ g : X' \to X'' $ là hai ánh xạ liên tục.*
a) *Nếu $ f $ và $ g $ là thực sự, thì $ g \circ f $ là thực sự.*
b) *Nếu $ g \circ f $ là thực sự và $ f $ là toàn ánh, thì $ g $ là thực sự.*
c) *Nếu $ g \circ f $ là thực sự và $ g $ là đơn ánh, thì $ f $ là thực sự.*
d) *Nếu $ g \circ f $ là thực sự và $ X' $ là Hausdorff, thì $ f $ là thực sự.*

Cho $ Z $ là một không gian tôpô. Ta có
$$
(g \circ f) \times \iota_Z = (g \times \iota_Z) \circ (f \times \iota_Z);
$$
nếu $ f $ và $ g $ là thực sự, thì $ f \times \iota_Z $ và $ g \times \iota_Z $ là đóng; do đó [\S 5, no. 1, Mệnh đề 1 a)] $ (g \circ f) \times \iota_Z $ là đóng; điều này chứng minh a). Chứng minh của b) [tương ứng c)] được tiến hành theo cùng các bước, sử dụng phần b) [tương ứng c)] của Mệnh đề 1 của \S 5, no. 1, và nhận xét rằng nếu $ f $ là toàn ánh (tương ứng nếu $ g $ là đơn ánh) thì $ f \times \iota_Z $ là toàn ánh (tương ứng $ g \times \iota_Z $ là đơn ánh). Cuối cùng, để chứng minh d), xét biểu đồ giao hoán

$$
\begin{array}{ccc}
X & \overset{\varphi}{\to} & X \times X' \\
f \downarrow & & \downarrow (g \circ f) \times \iota_{X'} \\
X' & \underset{\psi}{\to} & X'' \times X'
\end{array}
$$

trong đó $ \varphi(x) = (x, f(x)) $ và $ \psi(x') = (g(x'), x') $. Ánh xạ $ \varphi $ (tương ứng $ \psi $) là một đồng phôi của $ X $ (tương ứng $ X' $) lên đồ thị của $ f $ (tương ứng ảnh phản xạ của đồ thị của $ g $) (\S 4, no. 1, Mệnh đề 1, Hệ quả 2). Hơn nữa, vì $ X' $ là Hausdorff, đồ thị $ \varphi(X) $ của $ f $ là đóng trong $ X \times X' $ (\S 8, no. 1, Mệnh đề 2, Hệ quả 2). Do đó (Mệnh đề 2) $ \varphi $ là thực sự; mặt khác Mệnh đề 4 chỉ ra rằng $ (g \circ f) \times i_{X'} $ là thực sự. Theo a) ở trên và tính giao hoán của biểu đồ (1), $ \psi \circ f $ là thực sự; nhưng $ \psi $ là đơn ánh và do đó $ f $ là thực sự theo c) ở trên.

#### Nhận xét {#top-i-s10-n1-rem-1 .statement}

Nếu $ X' $ không là Hausdorff thì có thể xảy ra rằng $ g \circ f $ là thực sự còn $ f $ thì không; chẳng hạn, lấy $ X $ và $ X'' $ gồm một điểm và $ X' $ gồm hai điểm, với tôpô thô nhất.

#### Hệ quả 1 {#top-i-s10-prop-5-cor-1 .statement}

*Nếu $ f : X \to Y $ là một ánh xạ thực sự, thì hạn chế của $ f $ lên một tập con đóng $ F $ của $ X $ là một ánh xạ thực sự của $ F $ vào $ Y $.*

Vì hạn chế này là hợp thành $ f \circ j $, trong đó $ j : F \to X $ là đơn ánh chính tắc, và là thực sự theo Mệnh đề 2.

#### Hệ quả 2 {#top-i-s10-prop-5-cor-2 .statement}

*Cho $ f : X \to Y $ là một ánh xạ thực sự, trong đó $ X $ là Hausdorff. Khi đó không gian con $ f(X) $ của $ Y $ là Hausdorff.*

Theo Mệnh đề 5 c), ta chỉ cần xét trường hợp $ f(X) = Y $. Khi đó đường chéo của $ Y \times Y $ là ảnh qua $ f \times f $ của đường chéo của $ X $, vốn đóng (\S 8, no. 1, Mệnh đề 1); $ f \times f $ là thực sự (Mệnh đề 4); do đó đường chéo của $ Y \times Y $ là đóng (Mệnh đề 1) và vì vậy $ Y $ là Hausdorff (\S 8, no. 1, Mệnh đề 1).

#### Hệ quả 3 {#top-i-s10-prop-5-cor-3 .statement}

*Cho $ I $ là một tập hợp hữu hạn và với mỗi $ i \in I $, cho $ f_i : X \to Y_i $ là một ánh xạ thực sự. Nếu $ X $ là Hausdorff, thì ánh xạ $ x \mapsto (f_i(x)) $ của $ X $ vào $ \prod_{i \in I} Y_i $ là thực sự.*

Ánh xạ này là hợp thành của ánh xạ tích $ (x_i) \mapsto (f_i(x_i)) $ của $ X^I $ vào $ \prod_i Y_i $ và ánh xạ đường chéo của $ X $ vào $ X^I $; vì ánh xạ sau là thực sự (theo Mệnh đề 2 và \S 8, no. 1, Mệnh đề 1) nên kết luận suy ra từ Mệnh đề 4 và Mệnh đề 5 a).

#### Hệ quả 4 {#top-i-s10-prop-5-cor-4 .statement}

*Cho $ X $ và $ Y $ là hai không gian tôpô, $ f : X \to Y $ là một ánh xạ liên tục, $ R $ là quan hệ tương đương $ f(x) = f(y) $ trên $ X $, và*
$$
X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y
$$
*là phân tích chính tắc của $ f $.* *Khi đó để $ f $ là thực sự thì cần và đủ rằng $ p $ là thực sự, $ h $ là một phép đồng phôi và $ f(X) $ là một tập con đóng của $ Y $.*

Các điều kiện là đủ theo Mệnh đề 5 a) và Mệnh đề 2. Ngược lại, nếu $ f $ là thực sự, thì $ f $ là đóng; do đó $ f(X) $ là đóng trong $ Y $ và $ h $ là một phép đồng phôi ($ \S 5 $, no. 2, Mệnh đề 3); đồng thời $ h \circ p $ là thực sự theo Mệnh đề 5 c); do đó $ p = h^{-1} \circ (h \circ p) $ là thực sự theo Mệnh đề 5 a).

### 2. ĐẶC TRƯNG HÓA CÁC ÁNH XẠ THỰC SỰ BẰNG CÁC TÍNH CHẤT COMPACT

Trong tiểu mục này ta sẽ ký hiệu bởi $ P $ một không gian gồm một điểm duy nhất, với tôpô duy nhất của nó.

#### Bổ đề 1 {#top-i-s10-lem-1 .statement}

*Cho $ X $ là một không gian tôpô sao cho ánh xạ hằng $ X \to P $ là thực sự. Khi đó $ X $ là quasi-compact.*

(Ta sẽ thấy sau đây một chút (Định lý 1, Hệ quả 1) rằng tính chất này đặc trưng hóa các không gian quasi-compact.)
