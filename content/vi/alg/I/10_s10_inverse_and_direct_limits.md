---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 10
section_title: Inverse and direct limits
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0142-0147, 0203-0203
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE SYSTEMS OF MAGMAS
      page: 0
      pdf_page: 142
    - "no": 2
      title: INVERSE LIMITS OF ACTIONS
      page: 0
      pdf_page: 143
    - "no": 3
      title: DIRECT SYSTEMS OF MAGMAS
      page: 0
      pdf_page: 144
    - "no": 4
      title: DIRECT LIMIT OF ACTIONS
      page: 0
      pdf_page: 147
statements: 5
exercises: 2
content_sha256: 166433e603af117f388405115cafa8b4f181adc3f9c3d2a1c29954ddfdeda621
translated_from: content/en/alg/I/10_s10_inverse_and_direct_limits.md
source_content_sha256: b08bffa16dc436eeac0e17dcfce948125f5417d3d262e5a26fd8ffccc2df44ff
translation_model: gpt-5-6-mini
translation_run: translate-vi-37f286f0
glossary_version: 34
glossary_terms_sha256: 854e0a2c3527a98f006454f52da1bd4c688f406c47cfee2c311ffe31fd8f691d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. GIỚI HẠN NGƯỢC VÀ GIỚI HẠN TRỰC TIẾP

Trong toàn bộ đoạn này, tôi ký hiệu một tập tiền thứ tự không rỗng bởi $ I $, và $ \alpha \leq \beta $ là quan hệ tiền thứ tự trên I. Khái niệm hệ ngược (tương ứng hệ trực tiếp) của các tập hợp đối với tập chỉ số I được định nghĩa trong *Lý thuyết tập hợp*, III, § 7, no. 1 (tương ứng *Lý thuyết tập hợp*, III, § 7, no. 5, dưới giả thiết rằng I có hướng phải).

### 1. CÁC HỆ NGƯỢC CỦA CÁC MAGMA

#### Định nghĩa 1 {#alg-i-s10-def-1 .statement}

*Một hệ ngược của các magma đối với tập chỉ số I là một hệ ngược của các tập hợp* $ (\mathbf{E}_\alpha, f_{\alpha\beta}) $ *đối với I, mỗi* $ \mathbf{E}_\alpha $ *có một cấu trúc magma và mỗi* $ f_{\alpha\beta} $ *là một đồng cấu magma.*

Cho $ (\mathbf{E}_\alpha, f_{\alpha\beta}) $ là một hệ ngược của các magma mà các luật được viết theo phép nhân. Tập giới hạn ngược $ E = \lim_{\leftarrow} \mathbf{E}_\alpha $ là một tập con của magma tích $ \prod_{\alpha \in I} \mathbf{E}_\alpha $ gồm các họ $ (x_\alpha)_{\alpha \in I} $ sao cho $ x_\alpha = f_{\alpha\beta}(x_\beta) $ với $ \alpha \leq \beta $. Nếu $ (x_\alpha) $ và $ (y_\alpha) $ thuộc E, thì với $ \alpha \leq \beta $, $ x_\alpha = f_{\alpha\beta}(x_\beta) $ và $ y_\alpha = f_{\alpha\beta}(y_\beta) $, do đó $ x_\alpha y_\alpha = f_{\alpha\beta}(x_\beta) f_{\alpha\beta}(y_\beta) = f_{\alpha\beta}(x_\beta y_\beta) $; do đó E là một magma con của $ \prod_{\alpha \in I} \mathbf{E}_\alpha $. E sẽ được trang bị luật cảm sinh bởi luật trên $ \prod_{\alpha \in I} \mathbf{E}_\alpha $; magma thu được được gọi là

† Ta tránh thuật ngữ hiện hành trong đó dương có nghĩa là $ > 0 $.

magma giới hạn ngược của các magma $ E_\alpha $. Nó có tính chất phổ quát sau:

(a) Với mọi $ \alpha \in I $, ánh xạ chính tắc $ f_\alpha $ của $ E $ vào $ E_\alpha $ là một đồng cấu magma từ $ E $ vào $ E_\alpha $. $ f_\alpha = f_{\alpha \beta} \circ f_\beta $ với $ \alpha \leq \beta $.

(b) Giả sử một magma $ F $ được cho và các đồng cấu $ u_\alpha : F \to E_\alpha $ sao cho $ u_\alpha = f_{\alpha \beta} \circ u_\beta $ với $ \alpha \leq \beta $. Có duy nhất một đồng cấu $ u : F \to E $ sao cho $ u_\alpha = f_\alpha \circ u $ với mọi $ \alpha \in I $ (cụ thể là $ x \mapsto u(x) = (u_\alpha(x))_{\alpha \in I} $).

Nếu các magma $ E_\alpha $ là kết hợp (tương ứng giao hoán), thì E cũng vậy. Giả sử mỗi magma $ E_\alpha $ thừa nhận một phần tử đơn vị $ e_\alpha $ và các đồng cấu $ f_{\alpha \beta} $ là có đơn vị. Khi đó $ e = (e_\alpha)_{\alpha \in I} $ thuộc E vì $ e_\alpha = f_{\alpha \beta}(e_\beta) $ với $ \alpha \leq \beta $ và nó là một phần tử đơn vị của magma $ E $; với ký hiệu trên, các đồng cấu $ f_\alpha $ là có đơn vị và nếu các $ u_\alpha $ là có đơn vị thì $ u $ là có đơn vị. Hơn nữa, một phần tử $ x = (x_\alpha)_{\alpha \in I} $ của E là khả nghịch khi và chỉ khi mỗi $ x_\alpha $ là khả nghịch trong magma tương ứng $ E_\alpha $ và $ x^{-1} = (x_\alpha^{-1})_{\alpha \in I} $; điều này suy ra từ công thức $ f_{\alpha \beta}(x_\beta^{-1}) = f_{\alpha \beta}(x_\beta)^{-1} = x_\alpha^{-1} $ với $ \alpha \leq \beta $.

Từ các nhận xét này có thể suy ra rằng nếu các magma $ E_\alpha $ là các nửa nhóm có đơn vị (tương ứng nhóm) và các $ f_{\alpha \beta} $ là các đồng cấu nửa nhóm có đơn vị, thì magma $ E $ là một nửa nhóm có đơn vị (tương ứng một nhóm). Trong trường hợp này ta nói đến một hệ ngược của các nửa nhóm có đơn vị (tương ứng nhóm). Tính chất phổ quát chuyển ngay sang trường hợp này.

Để người đọc tự định nghĩa một hệ ngược các vành $ (E_\alpha, f_{\alpha \beta}) $ và kiểm chứng rằng $ E = \lim \leftarrow E_\alpha $ là một vành con của vành tích $ \prod_{\alpha \in I} E_\alpha $, được gọi là vành giới hạn ngược của các vành $ E_\alpha $; có thể kiểm chứng rằng tính chất phổ quát mở rộng đến trường hợp này.

Cho $ \mathfrak{C} = (E_\alpha, f_{\alpha \beta}) $ và $ \mathfrak{C}' = (E'_\alpha, f'_{\alpha \beta}) $ là hai hệ ngược của các magma (tương ứng là nửa nhóm, nhóm, vành) đối với cùng một tập chỉ số. Một đồng cấu từ $ \mathfrak{C} $ vào $ \mathfrak{C}' $ là một hệ ngược $ (u_\alpha)_{\alpha \in I} $ của các ánh xạ $ u_\alpha : E_\alpha \to E'_\alpha $ sao cho mỗi $ u_\alpha $ là một đồng cấu. Trong các điều kiện này, ánh xạ $ u = \lim \leftarrow u_\alpha $ từ $ \lim \leftarrow E_\alpha $ vào $ \lim \leftarrow E'_\alpha $ là một đồng cấu (xem Lý thuyết tập hợp , III, § 7, no. 2).

### 2. GIỚI HẠN NGƯỢC CỦA CÁC TÁC ĐỘNG

Giả sử đã cho hai hệ ngược của các tập hợp $ (\Omega_\alpha, \phi_{\alpha \beta}) $ và $ (E_\alpha, f_{\alpha \beta}) $ đối với cùng một tập chỉ số $ I $. Giả sử rằng với mọi $ \alpha \in I $ đã cho một tác động của $ \Omega_\alpha $ lên $ E_\alpha $ sao cho

(1)
$$
f_{\alpha \beta}(\omega_\beta x_\beta) = \phi_{\alpha \beta}(\omega_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$
cho $ \alpha \leq \beta, x_\beta \in E_\beta, \omega_\beta \in \Omega_\beta $. Khi đó họ các tác động được xét được gọi là một hệ ngược của các tác động. Đặt $ \Omega = \lim \leftarrow \Omega_\alpha $ và $ E = \lim \leftarrow E_\alpha $; nếu $ x = (x_\alpha)_{\alpha \in I} $ thuộc $ E $ và $ \omega = (\omega_\alpha)_{\alpha \in I} $ thuộc $ \Omega $, thì $ \omega . x = (\omega_\alpha . x_\alpha)_{\alpha \in I} $ thuộc E theo (1). Như vậy một tác động của $ \Omega $ lên E được định nghĩa, gọi là *giới hạn ngược của các tác động của $ \Omega_\alpha $ lên $ E_\alpha $*.

Điều trên đặc biệt áp dụng trong trường hợp các $ \Omega_\alpha $ là các nửa nhóm và mỗi tác động của $ \Omega_\alpha $ lên $ E_\alpha $ là một phép toán. Khi đó giới hạn ngược của các phép toán này là một phép toán của nửa nhóm trên E.

Để người đọc tự định nghĩa giới hạn ngược của một hệ ngược các nhóm có toán tử và kiểm chứng rằng giới hạn này là một nhóm có toán tử.

### 3. CÁC HỆ TRỰC TIẾP CỦA CÁC MAGMA

Trong số này và các số tiếp theo ta giả sử rằng I là *có hướng phải*.

#### Định nghĩa 2 {#alg-i-s10-def-2 .statement}

*Một hệ trực tiếp của các magma đối với tập chỉ số I là một hệ trực tiếp của các tập hợp* $ (E_\alpha, f_{\beta\alpha}) $ *đối với I, mỗi* $ E_\alpha $ *có một cấu trúc magma và mỗi* $ f_{\beta\alpha} $ *là một đồng cấu magma.*

Cho $ (E_\alpha, f_{\beta\alpha}) $ là một hệ trực tiếp của các magma. E sẽ ký hiệu tập giới hạn trực tiếp $ \lim_{\longrightarrow} E_\alpha $ và $ f_\alpha $ là ánh xạ chính tắc của $ E_\alpha $ vào E. Nhắc lại rằng

(2)
$$
f_\beta \circ f_{\beta\alpha} = f_\alpha \quad \text{cho } \alpha \leq \beta,
$$

(3)
$$
E = \bigcup_{\alpha \in I} f_\alpha(E_\alpha).
$$

Theo (2), cũng có

(4)
$$
f_\alpha(E_\alpha) \subset f_\beta(E_\beta) \quad \text{cho } \alpha \leq \beta.
$$

Nếu $ x_\alpha, y_\alpha \in E_\alpha $ là sao cho $ f_\alpha(x_\alpha) = f_\alpha(y_\alpha) $, tồn tại một $ \beta \geq \alpha $ sao cho $ f_{\beta\alpha}(x_\alpha) = f_{\beta\alpha}(y_\alpha) $.

#### Mệnh đề 1 {#alg-i-s10-prop-1 .statement}

*Trên E tồn tại duy nhất một cấu trúc magma sao cho các ánh xạ* $ f_\alpha : E_\alpha \to E $ *là các đồng cấu. Nếu các magma* $ E_\alpha $ *là kết hợp (tương ứng giao hoán), thì E cũng vậy. Nếu các magma* $ E_\alpha $ *và đồng cấu* $ f_{\beta\alpha} $ *là có đơn vị, thì magma* E *và các đồng cấu* $ f_\alpha $ *cũng vậy.*

Các magma $ E_\alpha $ sẽ được viết theo phép nhân.

Cho $ x, y $ thuộc E. Tồn tại $ \alpha $ thuộc I và $ x_\alpha, y_\alpha $ thuộc $ E_\alpha $ sao cho $ x = f_\alpha(x_\alpha) $ và $ y = f_\alpha(y_\alpha) $. Nếu tồn tại một cấu trúc magma trên E mà $ f_\alpha $ là một đồng cấu, thì $ x.y = f_\alpha(x_\alpha y_\alpha) $, do đó có *tính duy nhất* của cấu trúc magma này.

Để chứng minh sự tồn tại, ta phải chứng minh rằng với $ \alpha, \beta $ thuộc I, $ x_\alpha, y_\alpha $ thuộc $ E_\alpha $ và $ x'_\beta, y'_\beta $ thuộc $ E_\beta $, các hệ thức

(5)
$$
f_\alpha(x_\alpha) = f_\beta(x'_\beta), \qquad f_\alpha(y_\alpha) = f_\beta(y'_\beta)
$$
suy ra $ f_\alpha(x_\alpha y_\alpha) = f_\beta(x'_\beta y'_\beta) $. Với $ \gamma \geq \alpha $ và $ \gamma \geq \beta $, đặt $ x_\gamma = f_{\gamma\alpha}(x_\alpha) $, $ y_\gamma = f_{\gamma \alpha}(y_\alpha), x'_\gamma = f_{\gamma \beta}(x'_\beta), y'_\gamma = f_{\gamma \beta}(y'_\beta) $. Theo định nghĩa của giới hạn trực tiếp, tồn tại $ \gamma $ thuộc $ I $ sao cho $ \gamma \geq \alpha, \gamma \geq \beta, x_\gamma = x'_\gamma, y_\gamma = y'_\gamma $. Khi đó
$$
f_\alpha(x_\alpha y_\alpha) = f_\gamma(f_{\gamma \alpha}(x_\alpha y_\alpha)) = f_\gamma(x_\gamma y_\gamma) = f_\gamma(x'_\gamma y'_\gamma) = f_\gamma(f_{\gamma \beta}(x'_\beta y'_\beta)) \\
= f_\beta(x'_\beta y'_\beta).
$$
Giả sử các magma $ E_\alpha $ là kết hợp. Cho $ x, y, z $ thuộc $ E $. Tồn tại $ \alpha \in I $ và các phần tử $ x_\alpha, y_\alpha, z_\alpha $ thuộc $ E_\alpha $ sao cho
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha), \quad z = f_\alpha(z_\alpha).
$$
Khi đó $ xy = f_\alpha(x_\alpha y_\alpha) $, do đó $ (xy)z = f_\alpha((x_\alpha y_\alpha)z_\alpha) $; tương tự
$$
x(yz) = f_\alpha(x_\alpha(y_\alpha z_\alpha)),
$$
do đó $ (xy)z = x(yz) $ với $ (x_\alpha y_\alpha)z_\alpha = x_\alpha(y_\alpha z_\alpha) $. Trường hợp các magma giao hoán được xử lý tương tự.

Cuối cùng, giả sử mỗi magma $ E_\alpha $ có một phần tử đơn vị $ e_\alpha $ và $ f_{\beta \alpha}(e_\alpha) = e_\beta $ với $ \alpha \leq \beta $. Với $ \alpha, \beta $ thuộc $ I $, tồn tại $ \gamma $ thuộc $ I $ sao cho $ \gamma \geq \alpha $ và $ \gamma \geq \beta $, do đó
$$
f_\alpha(e_\alpha) = f_\gamma(f_{\gamma \alpha}(e_\alpha)) = f_\gamma(e_\gamma) = f_\gamma(f_{\gamma \beta}(e_\beta)) = f_\beta(e_\beta)
$$
và do đó tồn tại một phần tử $ e $ trong $ E $ sao cho $ f_\alpha(e_\alpha) = e $ với mọi $ \alpha \in I $. Cho $ x $ thuộc $ E $; chọn $ \alpha \in I $ và $ x_\alpha \in E_\alpha $ sao cho $ x = f_\alpha(x_\alpha) $. Khi đó
$$
ex = f_\alpha(e_\alpha) \cdot f_\alpha(x_\alpha) = f_\alpha(e_\alpha \cdot x_\alpha) = f_\alpha(x_\alpha) = x
$$
và tương tự $ x \cdot e = x $, do đó $ e $ là phần tử đơn vị của $ E $.

Magma $ E $ được gọi là *giới hạn trực tiếp của các magma* $ E_\alpha $.

#### Mệnh đề 2 {#alg-i-s10-prop-2 .statement}

*Cho* $ (E_\alpha, f_{\beta \alpha}) $ *là một hệ trực tiếp của các magma và cho* $ E $ *là giới hạn trực tiếp của nó với* $ f_\alpha : E_\alpha \to E $ *là các đồng cấu chính tắc. Giả sử một magma* $ F $ *và các đồng cấu* $ u_\alpha : E_\alpha \to F $ *được cho sao cho* $ u_\alpha = u_\beta \circ f_{\beta \alpha} $ *đối với* $ \alpha \leq \beta $. *Tồn tại một và chỉ một đồng cấu* $ u : E \to F $ *sao cho* $ u_\alpha = u \circ f_\alpha $ *với mọi* $ \alpha \in I $. *Nếu các magma* $ E_\alpha $ *và* $ F $ *cũng như các đồng cấu* $ f_{\beta \alpha} $ *và* $ u_\alpha $ *đều có đơn vị, thì đồng cấu* $ u $ *có đơn vị.*

Ta biết (*Lý thuyết tập hợp*, III, § 7, no. 6, Mệnh đề 6) rằng tồn tại một và chỉ một ánh xạ $ u : E \to F $ sao cho $ u_\alpha = u \circ f_\alpha $ với mọi $ \alpha \in I $. Ta kiểm tra rằng $ u $ là một đồng cấu: cho $ x, y $ là các phần tử của $ E $, $ \alpha $ thuộc $ I $ và $ x_\alpha, y_\alpha $ thuộc $ E_\alpha $ sao cho $ x = f_\alpha(x_\alpha) $ và $ y = f_\alpha(y_\alpha) $. Khi đó $ xy = f_\alpha(x_\alpha y_\alpha) $, do đó
$$
u(xy) = u(f_\alpha(x_\alpha y_\alpha)) = u_\alpha(x_\alpha y_\alpha) = u_\alpha(x_\alpha)u_\alpha(y_\alpha) \\
= u(f_\alpha(u_\alpha))u(f_\alpha(y_\alpha)) = u(x)u(y).
$$
Bây giờ ta xét trường hợp có đơn vị và ký hiệu $ e_\alpha $ là phần tử đơn vị của $ E_\alpha $, $ e $ là phần tử đơn vị của $ E $ và $ e' $ là phần tử đơn vị của $ F $. Chọn $ \alpha \in I $, khi đó $ e = f_\alpha(e_\alpha) $, do đó
$$
u(e) = u(f_\alpha(e_\alpha)) = u_\alpha(e_\alpha) = e'
$$
vì $ u_\alpha $ có đơn vị. Suy ra $ u $ có đơn vị.

Tương tự như khái niệm hệ trực tiếp của các magma, ta có thể xây dựng khái niệm hệ trực tiếp của các nửa nhóm hoặc nhóm. Mệnh đề 1 chỉ ra rằng magma E là giới hạn của một hệ trực tiếp của các nửa nhóm $(E_\alpha, f_{\beta\alpha})_{\alpha, \beta \in I}$ là một nửa nhóm. Ta chứng minh rằng E là một nhóm nếu các $E_\alpha$ là các nhóm: cho $x \in E, \alpha \in I$ và $x_\alpha \in E_\alpha$ sao cho $x = f_\alpha(x_\alpha)$; phần tử $y = f_\alpha(x_\alpha^{-1})$ của E là phần tử nghịch đảo của x (\S 2, no. 3). Tính chất phổ quát của Mệnh đề 2 được chuyển ngay lập tức sang trường hợp của một hệ trực tiếp của các nửa nhóm hoặc nhóm.

Người đọc được để lại việc định nghĩa một hệ trực tiếp các vành. Cho $(A_\alpha, f_{\beta\alpha})$ là một hệ trực tiếp như vậy; đặt $A = \lim \overrightarrow{A_\alpha}$ và $f_\alpha : A_\alpha \to A$ là các đồng cấu chính tắc. Trên A tồn tại duy nhất một phép cộng và phép nhân (Mệnh đề 2) được đặc trưng bởi $x + y = f_\alpha(x_\alpha + y_\alpha), xy = f_\alpha(x_\alpha y_\alpha)$ với $\alpha \in I, x_\alpha, y_\alpha$ thuộc $A_\alpha$ và $x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$. Đối với phép cộng, A là một nhóm giao hoán và phép nhân là kết hợp và có đơn vị. Cuối cùng, với $x, y, z$ thuộc A, chọn $\alpha$ trong I và $x_\alpha, y_\alpha$ và $z_\alpha$ trong $A_\alpha$ sao cho
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha) \quad \text{và} \quad z = f_\alpha(z_\alpha).
$$
Khi đó
$$
(x + y) \cdot z = f_\alpha(x_\alpha + y_\alpha)f_\alpha(z_\alpha) = f_\alpha((x_\alpha + y_\alpha)z_\alpha)
= f_\alpha(x_\alpha z_\alpha + y_\alpha z_\alpha) = f_\alpha(x_\alpha z_\alpha) + f_\alpha(y_\alpha z_\alpha) = xz + yz
$$
và quan hệ $x(y + z) = xy + xz$ được chứng minh tương tự. Nói cách khác, A có cấu trúc của một vành, được đặc trưng bởi tính chất $f_\alpha$ là một đồng cấu vành với mọi $\alpha \in I$.

Vành A được gọi là giới hạn trực tiếp của các vành $A_\alpha$. Mệnh đề 2 mở rộng ngay lập tức sang trường hợp các vành.

#### Mệnh đề 3 {#alg-i-s10-prop-3 .statement}

(a) *Nếu các $A_\alpha$ khác không, thì A khác không.*
(b) *Nếu các $A_\alpha$ là các miền nguyên, thì A là một miền nguyên.*
(c) *Nếu các $A_\alpha$ là các trường, thì A là một trường.*

Gọi $0_\alpha, 1_\alpha$ lần lượt là phần tử không và phần tử khả nghịch của $A_\alpha$ và 0, 1 lần lượt là phần tử không và phần tử khả nghịch của A. Tồn tại $\alpha \in I$ sao cho $f_\alpha(0_\alpha) = 0, f_\alpha(1_\alpha) = 1$. Nếu $0 = 1$, tồn tại $\beta \geq \alpha$ sao cho $f_{\beta\alpha}(0_\alpha) = f_{\beta\alpha}(1_\alpha)$, tức là $0_\beta = 1_\beta$. Điều này chứng minh (a).

Giả sử các $A_\alpha$ là các miền nguyên. Khi đó A là giao hoán và khác không theo (a). Cho $x, y$ là các phần tử của A sao cho $xy = 0$. Tồn tại $\alpha \in I$ và $x_\alpha, y_\alpha \in A_\alpha$ sao cho $x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$. Khi đó $f_\alpha(x_\alpha y_\alpha) = xy = 0 = f_\alpha(0_\alpha)$. Do đó tồn tại $\beta \geq \alpha$ sao cho $f_{\beta\alpha}(x_\alpha y_\alpha) = f_{\beta\alpha}(0_\alpha)$. Vì $A_\beta$ là một miền nguyên, suy ra $f_{\beta\alpha}(x_\alpha) = 0_\beta$ hoặc $f_{\beta\alpha}(y_\alpha) = 0_\beta$, do đó $x = 0$ hoặc $y = 0$. Điều này chứng minh (b).

Giả sử các $A_\alpha$ là các trường. Khi đó $A \neq \{0\}$ theo (a). Cho $x$ là một phần tử khác không của A. Tồn tại $\alpha \in I$ và $x_\alpha \in A_\alpha$ sao cho $x = f_\alpha(x_\alpha)$. Khi đó $x_\alpha \neq 0$ và $f_\alpha(x_\alpha^{-1})$ là nghịch đảo của $x$ trong A. Điều này chứng minh (c).

Cho $\mathfrak{E} = (E_\alpha, f_{\beta\alpha})$ và $\mathfrak{E}' = (E'_\alpha, f'_{\beta\alpha})$ là hai hệ trực tiếp của các magma (tương ứng là các monoid, nhóm, vành). Một đồng cấu của $ \mathfrak{E} $ vào $ \mathfrak{E}' $ là một hệ trực tiếp $ (u_\alpha)_{\alpha \in I} $ của các ánh xạ $ u_\alpha : E_\alpha \to E'_\alpha $ sao cho mỗi $ u_\alpha $ là một đồng cấu. Dưới các điều kiện này, ánh xạ $ u = \lim u_\alpha $ từ $ E = \lim E_\alpha $ đến $ E' = \lim E'_\alpha $ là một đồng cấu (xem *Lý thuyết tập hợp*, III, § 7, no. 6).

### 4. GIỚI HẠN TRỰC TIẾP CỦA CÁC TÁC ĐỘNG

Giả sử đã cho hai hệ trực tiếp của các tập hợp $ (\Omega_\alpha, \phi_{\beta \alpha}) $ và $ (E_\alpha, f_{\beta \alpha}) $ đối với cùng một tập chỉ số $ I $ và với mỗi $ \alpha \in I $ một tác động của $ \Omega_\alpha $ lên $ E_\alpha $. Giả sử rằng

$$
f_{\beta \alpha}(\omega_\alpha \cdot x_\alpha) = \phi_{\beta \alpha}(\omega_\alpha) \cdot f_{\beta \alpha}(x_\alpha)
$$

với $ \alpha \leq \beta, \omega_\alpha \in \Omega_\alpha $ và $ x_\alpha \in E_\alpha $. Khi đó họ các tác động đang xét được gọi là một *hệ trực tiếp của các tác động*. Dễ dàng kiểm tra như trong Mệnh đề 2 rằng tồn tại một tác động $ h $ của $ \Omega = \lim \Omega_\alpha $ lên $ E = \lim E_\alpha $ được mô tả như sau: cho $ \omega \in \Omega $ và $ x \in E $; chọn $ \alpha \in I $ và $ \omega_\alpha \in \Omega_\alpha, x_\alpha \in E_\alpha $ sao cho $ \omega = \phi_\alpha(\omega_\alpha) $ và $ x = f_\alpha(x_\alpha) $ ($ \phi_\alpha : \Omega_\alpha \to \Omega $ và $ f_\alpha : E_\alpha \to E $ biểu thị các ánh xạ chính tắc); khi đó $ \omega \cdot x = f_\alpha(\omega_\alpha \cdot x_\alpha) $. Tác động của $ \Omega $ lên $ E $ được gọi là *giới hạn trực tiếp của các tác động* của các $ \Omega_\alpha $ lên các $ E_\alpha $.

Nếu các $ \Omega_\alpha $ là các monoid và mỗi tác động của $ \Omega_\alpha $ lên $ E_\alpha $ là một phép toán, thì tác động giới hạn trực tiếp là một phép toán.

Người đọc được yêu cầu định nghĩa giới hạn trực tiếp của một hệ trực tiếp của các nhóm với toán tử và kiểm tra rằng giới hạn này là một nhóm với toán tử.

### Bài tập {#alg-i-s10-exercises}

Xem [các bài tập cho § 10](exercises/s10/).
