---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 3
section_title: Actions
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0048-0053, 0153-0156
extraction: ocr
subsections:
    - "no": 1
      title: ACTIONS
      page: 0
      pdf_page: 48
    - "no": 2
      title: SUBSETS STABLE UNDER AN ACTION. INDUCED ACTION
      page: 0
      pdf_page: 50
    - "no": 3
      title: QUOTIENT ACTION
      page: 0
      pdf_page: 50
    - "no": 4
      title: DISTRIBUTIVITY
      page: 0
      pdf_page: 51
    - "no": 5
      title: DISTRIBUTIVITY OF ONE INTERNAL LAW WITH RESPECT TO ANOTHER
      page: 0
      pdf_page: 53
statements: 14
exercises: 10
content_sha256: 60e949b59dfe8bf7320894e0f25856ce91966881cdcf03d01363f22addfbe1a4
translated_from: content/en/alg/I/03_s3_actions.md
source_content_sha256: d48d339714b4363c7ef630231fb716b1f37eb05a2eed63a58d2f5e403a576337
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-3445099e
glossary_version: 34
glossary_terms_sha256: 69f7688280454dd44bd59e0ed0d42285500de22bc7f0b953e24157e66662d813
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC TÁC ĐỘNG

### 1. CÁC TÁC ĐỘNG

#### Định nghĩa 1 {#alg-i-s3-def-1 .statement}

*Cho $ \Omega $ và E là hai tập hợp. Một ánh xạ của $ \Omega $ vào tập hợp $ E^E $ các ánh xạ của E vào chính nó được gọi là một tác động của $ \Omega $ trên E.*

Cho $ \alpha \mapsto f_\alpha $ là một tác động của $ \Omega $ trên E. Ánh xạ $ (\alpha, x) \mapsto f_\alpha(x) $ (tương ứng. $ (x, \alpha) \mapsto f_\alpha(x) $) được gọi là *luật tác động trái* (tương ứng. *phải*) *của $ \Omega $ trên E*† *liên kết với tác động đã cho của $ \Omega $ trên E*. Cho một ánh xạ $ g $ của $ \Omega \times E $ (tương ứng. $ E \times \Omega $) vào E, tồn tại duy nhất một tác động $ \alpha \mapsto f_\alpha $ của $ \Omega $ trên E sao cho luật tác động trái (tương ứng. phải) liên kết là $ g $ (*Lý thuyết tập hợp*, II, § 5, no. 2, Mệnh đề 3).

Trong chương này, để rút gọn cách viết, ta sẽ nói "luật tác động"

† Hoặc đôi khi là *phép toán ngoài của hợp thành* trên E với $ \Omega $ là tập hợp tác động.

thay cho "luật tác động trái". Phần tử $ f_\alpha(x) $ của E (với $ \alpha \in \Omega $ và $ x \in E $) đôi khi được gọi là *biến đổi* của $ x $ dưới tác động của $ \alpha $ hoặc *hợp thành* của $ \alpha $ và $ x $. Nó thường được ký hiệu bằng ký hiệu nhân trái (tương ứng. phải) $ \alpha . x $ (tương ứng. $ x . \alpha $), dấu chấm có thể được bỏ đi; khi đó hợp thành của $ \alpha $ và $ x $ được gọi là *tích* của $ \alpha $ và $ x $ (tương ứng. $ x $ và $ \alpha $). Ký hiệu lũy thừa $ x^\alpha $ cũng được dùng. Trong các lập luận của các đoạn sau, nói chung ta sẽ dùng ký hiệu $ \alpha \perp x $. Các phần tử của $ \Omega $ thường được gọi là *toán tử*.

#### Ví dụ {#alg-i-s3-n1-exa-1 .statement}

(1) Cho E là một nửa magma kết hợp được viết theo phép nhân. Ánh xạ liên kết với một số nguyên dương ngặt $ n $ ánh xạ $ x \mapsto x^n $ của E vào chính nó là một tác động của $ \mathbf{N}^* $ trên E. Nếu E là một nhóm, ánh xạ liên kết với một số nguyên hữu tỉ $ a $ ánh xạ $ x \mapsto x^a $ của E vào E là một tác động của $ \mathbf{Z} $ trên E.

(2) Cho E là một nửa magma với luật được ký hiệu bởi $ \top $. Ánh xạ liên kết với $ x \in E $ ánh xạ $ A \mapsto x \top A $ của tập hợp các tập con của E vào chính nó là một tác động của E trên $ \mathcal{P}(E) $.

(3) Cho E là một tập hợp. Ánh xạ đồng nhất của $ E^E $ là một tác động của $ E^E $ trên E, được gọi là *tác động chính tắc*. Luật tác động tương ứng là ánh xạ $ (f, x) \mapsto f(x) $ của $ E^E \times E $ vào E.

(4) Cho $ (\Omega_i)_{i \in I} $ là một họ các tập hợp. Với mọi $ i \in I $, cho $ f_i : \Omega_i \to E^E $ là một tác động của $ \Omega_i $ trên E. Cho $ \Omega $ là tổng của các $ \Omega_i $ (*Lý thuyết tập hợp*, II, § 4, no. 8). Ánh xạ $ f $ của $ \Omega $ lên $ E^E $, mở rộng các $ f_i $, là một tác động của $ \Omega $ trên E. Điều này cho phép ta rút gọn việc nghiên cứu một họ các tác động về việc nghiên cứu một tác động duy nhất.

(5) Cho một tác động của $ \Omega $ lên E với luật được ký hiệu bởi $ \perp $, một tập con $ \Xi $ của $ \Omega $ và một tập con X của E, $ \Xi \perp X $ ký hiệu tập hợp các $ \alpha \perp x $ với $ \alpha \in \Xi $ và $ x \in X $; khi $ \Xi $ gồm một phần tử duy nhất $ \alpha $, nói chung ta viết $ \alpha \perp X $ thay cho $ \{\alpha\} \perp X $. Ánh xạ gắn với $ \alpha \in \Omega $ ánh xạ $ X \mapsto \alpha \perp X $ là một tác động của $ \Omega $ lên $ \mathcal{P}(E) $, được gọi là *dẫn xuất* từ tác động đã cho bằng cách mở rộng lên tập hợp các tập con.

(6) Cho $ \alpha \mapsto f_\alpha $ là một tác động của $ \Omega $ lên E. Cho g là một ánh xạ từ $ \Omega' $ vào $ \Omega $. Khi đó ánh xạ $ \beta \mapsto f_{g(\beta)} $ là một tác động của $ \Omega' $ lên E.

(7) Cho $ f : E \times E \to E $ là một luật hợp thành trên một tập hợp E. Ánh xạ $ \gamma : x \mapsto \gamma_x $ (tương ứng. $ \delta : x \mapsto \delta_x $) (\S 2, no. 2) gắn với phần tử $ x \in E $ phép tịnh tiến trái (tương ứng. phải) bởi $ x $ là một tác động của E lên chính nó; nó được gọi là *tác động* *trái* (tương ứng. *phải*) của E lên chính nó *dẫn xuất* từ luật đã cho. Khi $ f $ là giao hoán, hai tác động này trùng nhau.

Luật của tác động trái (tương ứng. phải) liên kết với $ \gamma $ là $ f $ (tương ứng. luật đối của $ f $). Luật của tác động phải (tương ứng. trái) liên kết với $ \delta $ là $ f $ (tương ứng. luật đối của $ f $).

Cho $ \Omega, E, F $ là các tập hợp, $ \alpha \mapsto f_\alpha $ là một tác động của $ \Omega $ lên E và $ \alpha \mapsto g_\alpha $ là một tác động của $ \Omega $ lên F. Một $ \Omega $-*cấu xạ từ E vào F*, hay *ánh xạ từ E vào F tương thích với tác động của $ \Omega $*, là một ánh xạ $ h $ từ E vào F sao cho

$$
g_\alpha(h(x)) = h(f_\alpha(x))
$$

với mọi $ \alpha \in \Omega $ và $ x \in E $. Hợp thành của hai cấu xạ $ \Omega $ là một cấu xạ $ \Omega $.

Cho $ \Omega, \Xi, E, F $ là các tập hợp, $ \alpha \mapsto f_\alpha $ là một tác động của $ \Omega $ trên $ E $, $ \beta \mapsto g_\beta $ là một tác động của $ \Xi $ trên $ F $ và $ \phi $ là một ánh xạ của $ \Omega $ vào $ \Omega' $. Một $ \phi $-cấu xạ của $ E $ vào $ F $ là một ánh xạ $ h $ của $ E $ vào $ F $ sao cho
$$
g_{\phi(\alpha)}(h(x)) = h(f_\alpha(x))
$$
với mọi $ \alpha \in \Omega $ và $ x \in E $.

### 2. CÁC TẬP CON ỔN ĐỊNH DƯỚI MỘT TÁC ĐỘNG. TÁC ĐỘNG CẢM SINH

#### Định nghĩa 2 {#alg-i-s3-def-2 .statement}

*Một tập con $ A $ của một tập hợp $ E $ được gọi là ổn định dưới một tác động $ \alpha \mapsto f_\alpha $ của $ \Omega $ trên $ E $ nếu $ f_\alpha(A) \subset A $ với mọi $ \alpha \in \Omega $. Một phần tử $ x $ của $ E $ được gọi là bất biến dưới một phần tử $ \alpha $ của $ \Omega $ nếu $ f_\alpha(x) = x $.*

Giao của một họ các tập con ổn định của $ E $ dưới một tác động đã cho là ổn định. Do đó tồn tại một tập con ổn định nhỏ nhất của $ E $ chứa một tập con $ X $ đã cho của $ E $; nó được gọi là được *sinh* bởi $ X $; nó gồm các phần tử $ (f_{\alpha_1} \circ f_{\alpha_2} \circ \cdots \circ f_{\alpha_n})(x) $, trong đó $ x \in X, n \geq 0, \alpha_i \in \Omega $ với mọi $ i $.

#### Nhận xét {#alg-i-s3-n2-rem-1 .statement}

Cho $ E $ là một magma với luật được ký hiệu bởi $ \tau $. Cần lưu ý rằng một tập con $ A $ của $ E $ ổn định dưới tác động trái của $ E $ trên chính nó không nhất thiết ổn định dưới tác động phải của $ E $ trên chính nó; một tập con $ A $ của $ E $ ổn định dưới tác động trái (tương ứng phải) của $ E $ trên chính nó thì ổn định dưới luật trên $ E $, nhưng điều đảo lại nói chung không đúng. Chính xác hơn, $ A $ ổn định dưới luật trên $ E $ khi và chỉ khi $ A \tau A \subset A $ trong khi $ A $ ổn định dưới tác động trái (tương ứng phải) của $ E $ trên chính nó khi và chỉ khi $ E \tau A \subset A $ (tương ứng $ A \tau E \subset A $).

#### Ví dụ {#alg-i-s3-n2-exa-1 .statement}

Lấy magma $ E $ là tập $ \mathbf{N} $ với phép nhân. Tập $ \{1\} $ là ổn định đối với luật nội tại của $ \mathbf{N} $, nhưng tập con ổn định đối với tác động của $ \mathbf{N} $ trên chính nó sinh bởi $ \{1\} $ là toàn bộ $ \mathbf{N} $.

#### Định nghĩa 3 {#alg-i-s3-def-3 .statement}

*Cho $ \alpha \mapsto f_\alpha $ là một tác động của $ \Omega $ trên $ E $ và $ A $ là một tập con ổn định của $ E $. Ánh xạ gắn với một phần tử $ \alpha \in \Omega $ hạn chế của $ f_\alpha $ lên $ A $ (được xem như một ánh xạ từ $ A $ vào chính nó) là một tác động của $ \Omega $ trên $ A $ được gọi là cảm sinh bởi tác động đã cho.*

### 3. TÁC ĐỘNG THƯƠNG

#### Định nghĩa 4 {#alg-i-s3-def-4 .statement}

*Cho $ \alpha \mapsto f_\alpha $ là một tác động của một tập hợp $ \Omega $ trên một tập hợp $ E $. Một quan hệ tương đương $ R $ trên $ E $ được gọi là tương thích với tác động đã cho nếu, với mọi phần tử $ x $ và $ y $ của $ E $ sao cho $ x \equiv y \pmod{R} $ và mọi $ \alpha \in \Omega, f_\alpha(x) \equiv f_\alpha(y) \pmod{R} $. Ánh xạ gắn với một phần tử $ \alpha \in \Omega $ ánh xạ của $ E/R $ vào chính nó dẫn xuất từ $ f_\alpha $ bằng cách chuyển qua các thương là một tác động của $ \Omega $ trên $ E/R $ được gọi là thương của tác động của $ \Omega $ trên $ E $.*

Cho $ E $ là một magma và $ R $ là một quan hệ tương đương trên $ E $. $ R $ được gọi là *trái* (tương ứng *phải*) *tương thích* với luật trên $ E $ nếu nó tương thích với tác động trái (tương ứng

phải) của E trên chính nó dẫn xuất từ luật trên E. Để R tương thích với luật trên E thì điều kiện cần và đủ là nó tương thích trái và phải với luật trên E.

Chúng ta để cho độc giả phát biểu và chứng minh các mệnh đề tương tự của các Mệnh đề 6, 7 và 8 của § 1, no. 6.

### 4. TÍNH PHÂN PHỐI

#### Định nghĩa 5 {#alg-i-s3-def-5 .statement}

Cho $ E_1, \ldots, E_n $ và F là các tập hợp và u là một ánh xạ từ $ E_1 \times \cdots \times E_n $ vào F. Cho $ i \in \{1, n\} $. Giả sử $ E_i $ và F được cho các cấu trúc của magma. u được gọi là phân phối đối với biến chỉ số i nếu ánh xạ bộ phận

$$
x_i \mapsto u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n)
$$

là một đồng cấu của $ E_i $ vào F đối với mọi $ a_j $ cố định trong $ E_j $ và $ j \neq i $.

Nếu $ \top $ ký hiệu các luật nội tại trên $ E_i $ và F, tính phân phối của u được cho bởi các đẳng thức

(1) $$
u(a_1, \ldots, a_{i-1}, x_i \top x'_i, a_{i+1}, a_n) \\
= u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n) \top u(a_1, \ldots, a_{i-1}, x'_i, a_{i+1}, \ldots, a_n)
$$

với $ i = 1, 2, \ldots, n, a_1 \in E_1, \ldots, a_{i-1} \in E_{i-1}, x_i \in E_i, x'_i \in E_i, a_{i+1} \in E_{i+1}, \ldots, a_n \in E_n $.

#### Ví dụ {#alg-i-s3-n4-exa-1 .statement}

Cho E là một monôit (tương ứng nhóm) được viết theo phép nhân. Ánh xạ $ (n, x) \mapsto x^n $ từ $ \mathbf{N} \times E $ (tương ứng $ \mathbf{Z} \times E $) vào E là phân phối đối với biến thứ nhất bởi đẳng thức $ x^{m+n} = x^m x^n $ (với phép cộng là luật trên $ \mathbf{N} $). Nếu E là giao hoán, ánh xạ này là phân phối đối với biến thứ hai bởi đẳng thức $ (xy)^n = x^n y^n $.

#### Mệnh đề 1 {#alg-i-s3-prop-1 .statement}

Cho $ E_1, E_2, \ldots, E_n $ và F là các nửa nhóm giao hoán được viết cộng tính và cho u là một ánh xạ từ $ E_1 \times \cdots \times E_n $ vào F, có tính phân phối đối với tất cả các biến. Với $ i = 1, 2, \ldots, n $, cho $ L_i $ là một tập hợp hữu hạn không rỗng và $ (x_{i,\lambda})_{\lambda \in L_i} $ là một họ các phần tử của $ E_i $. Đặt $ y_i = \sum_{\lambda \in L_i} x_{i,\lambda} $ với $ i = 1, 2, \ldots, n $. Khi đó

(2) $$
u(y_1, \ldots, y_n) = \sum_\alpha u(x_1, \alpha_1, \ldots, x_n, \alpha_n)
$$

tổng được lấy trên tất cả các dãy $ \alpha = (\alpha_1, \ldots, \alpha_n) $ thuộc $ L_1 \times \cdots \times L_n $.

Ta lập luận bằng quy nạp theo n, trường hợp $ n = 1 $ suy ra từ công thức (2) của § 1, no. 2. Từ cùng tham chiếu đó

(3) $$
u(y_1, \ldots, y_{n-1}, y_n) = \sum_{\alpha_n \in L_n} u(y_1, \ldots, y_{n-1}, x_n, \alpha_n)
$$

với $ y_n = \sum_{\alpha_n \in L_n} x_{n,\alpha_n} $ và ánh xạ $ z \mapsto u(y_1, \ldots, y_{n-1}, z) $ từ $ E_n $ vào $ F $ là một đồng cấu magma. Theo giả thiết quy nạp áp dụng cho các ánh xạ phân phối $ (z_1, \ldots, z_{n-1}) \mapsto u(z_1, \ldots, z_{n-1}, x_n, \alpha_n) $ từ $ E_1 \times \cdots \times E_{n-1} $ vào $ F $,

(4)
$$
u(y_1, \ldots, y_{n-1}, x_n, \alpha_n) = \sum_{\alpha_1, \ldots, \alpha_{n-1}} u(x_1, \alpha_1, \ldots, x_{n-1}, \alpha_{n-1}, x_n, \alpha_n),
$$
tổng được lấy trên các dãy $ (\alpha_1, \ldots, \alpha_{n-1}) $ thuộc $ M = L_1 \times \cdots \times L_{n-1} $. Bây giờ $ L_1 \times \cdots \times L_n = M \times L_n $; viết
$$
t_{\alpha_1, \ldots, \alpha_n} = u(x_1, \alpha_1, \ldots, x_n, \alpha_n),
$$
ta có
(5)
$$
\sum_{\alpha_1, \ldots, \alpha_n} t_{\alpha_1, \ldots, \alpha_n} = \sum_{\alpha_n} \left( \sum_{\alpha_1, \ldots, \alpha_{n-1}} t_{\alpha_1, \ldots, \alpha_{n-1}, \alpha_n} \right)
$$
theo công thức (7) của § 1, no. 5. (2) suy ra ngay lập tức từ (3), (4) và (5).

#### Nhận xét {#alg-i-s3-n4-rem-1 .statement}

Nếu $ u(a_1, \ldots, a_{i-1}, 0, a_{i+1}, \ldots, a_n) = 0 $ với $ i = 1, 2, \ldots, n $ và $ a_j \in E_j $ ($ j \neq i $), thì công thức (2) vẫn đúng cho các họ $ (x_i, \lambda)_{\lambda \in L_i} $ có giá hữu hạn.

Một trường hợp đặc biệt của Định nghĩa 5 là trường hợp trong đó $ u $ là luật tác động liên kết với tác động của một tập hợp $ \Omega $ trên một magma $ E $. Nếu $ u $ có tính phân phối đối với biến thứ hai, cũng nói rằng tác động của $ \Omega $ trên magma $ E $ là phân phối. Nói cách khác:

#### Định nghĩa 6 {#alg-i-s3-def-6 .statement}

*Một tác động* $ \alpha \mapsto f_\alpha $ *của một tập hợp* $ \Omega $ *trên một magma* $ E $ *được gọi là phân phối nếu, với mọi* $ \alpha \in \Omega $, *ánh xạ* $ f_\alpha $ *là một tự đồng cấu của magma* $ E $.

Nếu $ \top $ ký hiệu luật của magma $ E $ và $ \perp $ ký hiệu luật tác động liên kết với tác động của $ \Omega $ trên $ E $, thì tính phân phối của luật sau được biểu diễn bởi công thức
(6)
$$
\alpha \perp (x \top y) = (\alpha \perp x) \top (\alpha \perp y) \quad \text{(cho } \alpha \in \Omega \text{ và } x, y \in E\text{)}.
$$

Do lạm dụng ngôn ngữ, cũng nói rằng luật $ \perp $ là phân phối (hoặc phân phối phải) đối với luật $ \top $.

Công thức (2) của § 1, no. 2 chỉ ra rằng khi đó, với mọi dãy có thứ tự $ (x_\lambda)_{\lambda \in L} $ các phần tử của $ E $ và mọi $ \alpha \in \Omega $,
(7)
$$
\alpha \perp \left( \bigwedge_{\lambda \in L} x_\lambda \right) = \bigwedge_{\lambda \in L} (\alpha \perp x_\lambda).
$$

Nếu một tác động $ \alpha \mapsto f_\alpha $ là phân phối được và một quan hệ tương đương $ R $ trên $ E $ tương thích với luật hợp thành của $ E $ và tác động $ \alpha \mapsto f_\alpha $, thì tác động thương trên $ E/R $ là phân phối được.

Khi luật trên $ E $ được viết theo dạng nhân, ta thường dùng ký hiệu lũy thừa $ x^\alpha $ cho một luật tác động phân phối được đối với phép nhân này, sao cho tính phân phối được biểu diễn bởi đẳng thức $ (xy)^\alpha = x^\alpha y^\alpha $. Nếu luật trên E được viết theo dạng cộng, ta thường dùng ký hiệu nhân trái (tương ứng. phải) $ \alpha . x $ (tương ứng. $ x . \alpha $) cho một luật tác động phân phối được đối với phép cộng này, tính phân phối được biểu diễn bởi đẳng thức

$$
\alpha(x + y) = \alpha x + \alpha y \quad (\text{resp. } (x + y)\alpha = x\alpha + y\alpha).
$$

Ta cũng có thể xét trường hợp $ \Omega $ có một luật nội tại, ký hiệu bởi $ \overline{T} $, và luật tác động là phân phối được đối với biến thứ nhất, nghĩa là

(8)
$$
(\alpha \overline{T} \beta) \perp x = (\alpha \perp x) T (\beta \perp x)
$$
với mọi $ \alpha, \beta \in \Omega $ và $ x \in E $. Khi đó, theo công thức (2) của § 1, no. 2

(9)
$$
\left( \overline{T}_{\lambda \in L} \alpha_{\lambda} \right) \perp x = \overline{T}_{\lambda \in L} (\alpha_{\lambda} \perp x)
$$
đối với mọi dãy có thứ tự $ (\alpha_{\lambda})_{\lambda \in L} $ các phần tử của $ \Omega $ và mọi $ x \in E $.

### 5. TÍNH PHÂN PHỐI CỦA MỘT LUẬT NỘI TẠI ĐỐI VỚI MỘT LUẬT NỘI TẠI KHÁC

#### Định nghĩa 7 {#alg-i-s3-def-7 .statement}

Cho $ T $ và $ \perp $ là hai luật nội tại trên một tập hợp E. Luật $ \perp $ được gọi là phân phối được đối với luật $ T $ nếu

(10)
$$
x \perp (y T z) = (x \perp y) T (x \perp z)
$$
(11)
$$
(x T y) \perp z = (x \perp z) T (y \perp z)
$$
với mọi $ x, y, z $ trong E.

Chú ý rằng (10) và (11) là tương đương nếu luật $ \perp $ là giao hoán. Nói chung, một trong các luật được viết theo dạng cộng và luật kia theo dạng nhân; nếu phép nhân phân phối được đối với phép cộng, thì:

(12)
$$
x . (y + z) = x . y + x . z
$$
(13)
$$
(x + y) . z = x . z + y . z
$$

#### Ví dụ {#alg-i-s3-n5-exa-1 .statement}

(1) Trong tập hợp $ \mathcal{P}(E) $ các tập con của một tập hợp E, mỗi luật nội tại $ \cap $ và $ \cup $ đều phân phối được đối với chính nó và đối với luật kia. Điều này suy ra từ các công thức dạng

$$
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
$$
$$
A \cup (B \cap C) = (A \cup B) \cap (A \cup C).
$$

(2) Trong $ \mathbf{Z} $ (và nói chung, trong mọi tập sắp thứ tự toàn phần) mỗi luật sup và inf đều phân phối được đối với luật kia và đối với chính nó.

(3) Trong $ \mathbf{Z} $(*và nói chung trong mọi vành*) phép nhân phân phối được đối với phép cộng.

(4) Trong $ \mathbf{N} $ phép cộng và phép nhân phân phối được đối với các luật sup và inf.

### Bài tập {#alg-i-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
