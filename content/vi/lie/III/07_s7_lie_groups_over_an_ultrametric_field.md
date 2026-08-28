---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 7
section_title: Lie groups over an ultrametric field
lang: vi
source: lie-i-iii
pdf_pages: 0344-0355, 0409-0413
extraction: ocr
subsections:
    - "no": 1
      title: PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS
      page: 0
      pdf_page: 345
    - "no": 2
      title: EXPONENTIAL MAPPINGS
      page: 0
      pdf_page: 346
    - "no": 3
      title: STANDARD GROUPS†
      page: 0
      pdf_page: 346
    - "no": 4
      title: FILTRATION OF STANDARD GROUPS
      page: 0
      pdf_page: 348
    - "no": 5
      title: POWERS IN STANDARD GROUPS
      page: 0
      pdf_page: 349
    - "no": 6
      title: LOGARITHMIC MAPPING
      page: 0
      pdf_page: 351
statements: 26
exercises: 10
content_sha256: d2160344699d1c7f7c55cce0254246881d03bf4bcda0816116a4cc3b859296cc
translated_from: content/en/lie/III/07_s7_lie_groups_over_an_ultrametric_field.md
source_content_sha256: 99933437c8c4d2e2f5fcf1297f50f16501e540051b440dd1d8a6c64abe8c68f7
translation_model: gpt-5-mini, gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-a6d5466a
glossary_version: 34
glossary_terms_sha256: 3d955f029a5b6c5bffbc8fb48b4a3f22a18862b17cd2c9a719f88c3e6bc0f45c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. CÁC NHÓM LIE TRÊN MỘT TRƯỜNG ULTRAMETRIC

Trong đoạn này, trường định giá $K$ được giả thiết là ultrametric và có đặc số 0. Ký hiệu $A$ là vành định giá của $K$, $m$ là iđêan cực đại của $A$ và $p$ là đặc số của trường thặng dư $A/m$. Nếu $K$ compact địa phương, thì $p \neq 0$ (*Đại số giao hoán*, Chương VI, \S 9, Định lý 1).

### 1. TỪ CÁC ĐẠI SỐ LIE ĐẾN CÁC NHÓM LIE

#### Mệnh đề 1 {#lie-iii-s7-prop-1 .statement}

Cho G là một mầm nhóm Lie với phần tử đơn vị e. Tồn tại một hệ cơ bản các lân cận mở của e trong G gồm các nhóm con Lie của G.

Trang bị cho L(G) một chuẩn tương thích với tôpô của nó và sao cho $\| [x, y] \| \leq \| x \| \| y \|$ với mọi x, y trong L(G). Gọi G_1 là nhóm Lie được xác định bởi L(G). Theo § 4, no. 2, Định lý 2, G và G_1 là đẳng cấu địa phương. Khi đó chỉ cần áp dụng § 4, no. 2, Bổ đề 3 (iii).

#### Định lý 1 {#lie-iii-s7-thm-1 .statement}

Cho L là một đại số Lie đầy đủ khả chuẩn. Tồn tại một nhóm Lie G sao cho L(G) đẳng cấu với L. Hai nhóm như vậy là đẳng cấu địa phương.

Mệnh đề đầu tiên đã được chứng minh trong § 4, no. 2, Bổ đề 3. Mệnh đề thứ hai là một trường hợp riêng của § 4, no. 2, Định lý 2.

#### Định lý 2 {#lie-iii-s7-thm-2 .statement}

Cho G là một nhóm Lie và h là một đại số con Lie của L(G) nhận một phần bù tôpô. Tồn tại một nhóm con Lie H của G sao cho L(H) = h. Nếu H_1 và H_2 là các nhóm con Lie của G sao cho L(H_1) = L(H_2) = h, thì H_1 \cap H_2 là mở trong H_1 và H_2.

Mệnh đề đầu tiên suy ra từ Mệnh đề 1 và § 4, no. 2, Định lý 3. Mệnh đề thứ hai là một trường hợp riêng của § 4, no. 2, Định lý 3.

#### Định lý 3 {#lie-iii-s7-thm-3 .statement}

Cho G và H là các nhóm Lie và h là một cấu xạ liên tục của L(G) vào L(H).

(i) Tồn tại một nhóm con mở G' của G và một cấu xạ nhóm Lie $\phi$ của G' vào H sao cho $h = L(\phi)$.

(ii) Cho G_1, G_2 là các nhóm con mở của G và $\phi_i$ là một cấu xạ của G_i vào H sao cho $h = L(\phi_i)$. Khi đó $\phi_1$ và $\phi_2$ trùng nhau trên một nhóm con mở của G.

Theo Mệnh đề 1, điều này suy ra từ § 4, no. 1, Định lý 1.

#### Mệnh đề 2 {#lie-iii-s7-prop-2 .statement}

Cho G là một nhóm Lie và h là một đại số con Lie của L(G) nhận một phần bù tôpô. Các điều kiện sau là tương đương:

(i) Tồn tại một nhóm con mở G' của G và một nhóm con Lie chuẩn H của G' sao cho L(H) = h.

(ii) h là một iđêan của L(H).

Nếu tồn tại G' và H với các tính chất của (i), thì L(G') = L(G) và L(H) là một iđêan của L(G') theo § 3, no. 12, Mệnh đề 47.

Giả sử rằng h là một iđêan của L(G). Tồn tại một nhóm Lie F sao cho L(F) = L(G)/h (Định lý 1). Gọi h là cấu xạ chính tắc của L(G) lên L(F). Theo Định lý 3 (i), tồn tại một nhóm con mở G' của G và một cấu xạ nhóm Lie $\phi$ của G' vào F sao cho $L(\phi) = h$. Theo § 3, no. 8, hạt nhân H của $\phi$ là một nhóm con Lie của G' và $L(H) = \mathrm{Ker}\ L(\phi) = \mathrm{Ker}\ h = h$. Cuối cùng, H là chuẩn trong G' vì $H = \mathrm{Ker}\ \phi$.

### 2. CÁC ÁNH XẠ MŨ

#### Mệnh đề 3 {#lie-iii-s7-prop-3 .statement}

Cho G là một nhóm Lie. Tồn tại một ánh xạ mũ $\phi$ của G với các tính chất sau:
(i) $\phi$ được xác định trên một nhóm con mở U của nhóm cộng tính $L(G)$;
(ii) $\phi(U)$ là một nhóm con mở của G và $\phi$ là một đẳng cấu của đa tạp giải tích U lên đa tạp giải tích $\phi(U)$;
(iii) $\phi(nx) = \phi(x)^n$ với mọi $x \in U$ và mọi $n \in \mathbf{Z}$.

Trang bị cho $L(G)$ một chuẩn tương thích với tôpô của nó và sao cho $\| [x, y] \| \leq \| x \| \| y \|$ đối với $x, y$ trong $L(G)$. Gọi $G_1$ là nhóm Lie được xác định bởi $L(G)$. Gọi $\psi = \mathrm{Id}_{G_1}$, đây là một ánh xạ mũ của $G_1$. Với mọi $\mu > 0$, gọi $L_\mu$ là tập hợp các $x \in L(G)$ sao cho $\| x \| < \mu$. Khi $\mu$ đủ nhỏ, $L_\mu$ là một nhóm con mở của nhóm cộng tính $L(G)$, $\psi(L_\mu)$ là một nhóm con mở của $G_1$ (\S 4, no. 2, Bổ đề 3), $\psi|L_\mu$ là một đẳng cấu của các đa tạp giải tích của $L_\mu$ lên $\psi(L_\mu)$ và $\psi(nx) = \psi(x)^n$ với mọi $x \in L_\mu$ và mọi $n \in \mathbf{Z}$. Các $L_\mu$ tạo thành một hệ cơ bản các lân cận của 0 trong $L(G)$. Theo Định lý 1, tồn tại $\mu$ và một nhóm con mở $G'$ của G sao cho $\psi(L_\mu)$ và $G'$ đẳng cấu, do đó có mệnh đề.

#### Mệnh đề 4 {#lie-iii-s7-prop-4 .statement}

Cho G là một nhóm Lie và $\phi$ là một ánh xạ mũ đơn ánh của G. Giả sử rằng $p > 0$. Với mọi $x, y$ trong $L(G)$,

(1)
$$
x + y = \lim_{n \to +\infty} p^{-n} \phi^{-1}(\phi(p^n x) \phi(p^n y))
$$
(2)
$$
[x, y] = \lim_{n \to +\infty} p^{-2n} \phi^{-1}(\phi(p^n x) \phi(p^n y) \phi(-p^n x) \phi(-p^n y)).
$$

Đây là các trường hợp đặc biệt của Mệnh đề 4 của \S 4, no. 3.

### 3. CÁC NHÓM CHUẨN†

Nếu $S(X_1, X_2, \ldots, X_n)$ là một chuỗi lũy thừa hình thức với các hệ số trong $A$, thì, với mọi $x_1, \ldots, x_r$ trong m, chuỗi $S(x_1, x_2, \ldots, x_r)$ là hội tụ. Chính xác hơn, $m \times m \times \cdots \times m$ được chứa trong miền hội tụ tuyệt đối của $S$ (Các đa tạp khả vi và giải tích, R, 4.1.3).

#### Định nghĩa 1 {#lie-iii-s7-def-1 .statement}

Cho r là một số nguyên $\geq 0$. Một nhóm chuẩn chiều r trên K là một nhóm Lie G có các tính chất sau:
(i) đa tạp giải tích cơ sở của G là $m \times m \times \cdots \times m$ (r thừa số);
(ii) tồn tại một chuỗi lũy thừa hình thức F trong 2r biến với các hệ số trong $A^r$, không có số hạng hằng, sao cho $x.y = F(x, y)$ với mọi $x, y$ trong G.

Khi đó $0.0 = 0$ và do đó phần tử đơn vị của G là gốc của $m \times m \cdots \times m$.

† Các kết quả của các số 3 và 4 cùng với các chứng minh của chúng vẫn đúng khi đặc số của K là $> 0$.

L(G) sẽ được đồng nhất với K'. Theo § 5, công thức (13), các hằng cấu trúc của L(G) đối với cơ sở chính tắc thuộc về A. Trong cùng một chứng minh, ta sẽ cần xét các phần tử của m × ... × m, lúc này như các phần tử của G, lúc khác như các phần tử của L(G).

#### Ví dụ {#lie-iii-s7-n3-exa-1 .statement}

Cho G = 1 + M_n(m), là một tập con mở của M_n(K). Nếu x ∈ G, thì det x ∈ 1 + m và do đó G ⊂ GL(n, K). Rõ ràng GG ⊂ G. Nếu x = 1 + y với y ∈ M_n(m), phép tính nghịch đảo của một ma trận chứng minh trước hết rằng x^{-1} ∈ M_n(A); nếu ta viết x^{-1} = 1 + y', thì y + y' + yy' = 0, do đó y' ∈ M_n(m) và vì thế x^{-1} ∈ G. Vậy G là một nhóm con mở của GL(n, K). Ta đồng nhất G với m^{n^2} nhờ ánh xạ (\delta_{ij} + y_{ij}) ↦ (y_{ij}). Rõ ràng G là một nhóm chuẩn.

#### Định lý 4 {#lie-iii-s7-thm-4 .statement}

Cho G là một nhóm Lie hữu hạn chiều. Tồn tại một nhóm con mở của G đẳng cấu với một nhóm chuẩn.

Bằng cách thay G bởi một nhóm đẳng cấu với một nhóm con mở của G, bài toán được quy về trường hợp G là một tập con mở của K', với phần tử đơn vị 0 và trong đó các tọa độ của tích x.y và nghịch đảo x^{[-1]} được cho bởi các công thức

(3) $$(x.y)_i = x_i + y_i + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha \beta i} x^\alpha y^\beta \quad (i = 1, 2, \ldots, r)$$

(4) $$(x^{[-1]})_i = -x_i + \sum_{|\alpha| > 1} d_{\alpha i} x^\alpha \quad (i = 1, 2, \ldots, r)$$

trong đó các chuỗi ở vế phải là hội tụ với x, y trong G (§ 5, no. 1). Cho λ ∈ K* và luật nhóm được chuyển từ G sang G' = λG bởi phép vị tự tỉ số λ. Với x', y' trong G', tích x'.y' và nghịch đảo x'^{[-1]} được tính trong G' có các tọa độ

$$(x'.y')_i = x'_i + y'_i + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c'_{\alpha \beta i} x'^\alpha y'^\beta \quad (i = 1, 2, \ldots, r)$$

$$(x'^{[-1]})_i = -x'_i + \sum_{|\alpha| > 1} d'_{\alpha i} x'^\alpha \quad (i = 1, 2, \ldots, r)$$

trong đó

$$c'_{\alpha \beta i} = \lambda^{-|\alpha|-|\beta|+1} c_{\alpha \beta i}, \qquad d'_{\alpha i} = \lambda^{-|\alpha|+1} d_{\alpha i}.$$

Vì các chuỗi (3) và (4) là hội tụ, ta thấy rằng, với |λ| đủ lớn, với mọi α, β, i,

$$|c'_{\alpha \beta i}| \leq 1, \qquad |d'_{\alpha i}| \leq 1$$

nghĩa là c'_{\alpha \beta i} ∈ A và d'_{\alpha i} ∈ A; và mặt khác G' ⊃ m × m × ... × m. Khi đó m × m × ... × m là một nhóm con mở của G' và là một nhóm chuẩn.

### 4. LỌC CÁC NHÓM CHUẨN

Ta lại sử dụng ký hiệu của Định nghĩa 1. Ta chọn một số $a > 1$ và một định giá thực $v$ của $K$ sao cho $|x| = a^{-v(x)}$ với mọi $x \in K$ (Đại số giao hoán, Chương VI, § 6, Mệnh đề 3). Nếu $a$ là một iđêan khác không (và do đó mở) của $A$ được chứa trong $m$, ký hiệu $G(a)$ là tập hợp các phần tử của G mà các tọa độ của chúng thuộc về $a$. Nếu $\lambda \in \mathbf{R}$, ký hiệu $a_\lambda$ (tương ứng $a_\lambda^+$) là tập hợp các $x \in K$ sao cho $v(x) \geq \lambda$ (tương ứng $v(x) > \lambda$); khi đó $a_0 = A$, $a_0^+ = m$. Với $x = (x_1, \ldots, x_r) \in G$, ta sẽ viết

$$
\omega(x) = \inf(v(x_1), \ldots, v(x_r)).
$$

#### Mệnh đề 5 {#lie-iii-s7-prop-5 .statement}

Cho $G$ là một nhóm chuẩn.

(i) Nếu $a$ là một iđêan khác không của $A$ được chứa trong $m$, $G(a)$ là một nhóm con chuẩn mở của $G$.

(ii) Các $G(a_\lambda)$, với $\lambda > 0$, tạo thành một hệ cơ bản các lân cận của $e$ trong $G$.

(iii) Giả sử rằng $a_\lambda \subset a$ với $\lambda \geq \lambda_0$ và cho $G(a)/G(a_\lambda)$, với $\lambda \geq \lambda_0$, có tôpô rời rạc. Khi đó nhóm tôpô $G(a)$ là giới hạn ngược của các nhóm $G(a)/G(a_\lambda)$.

(iv) Cho $a, b$ là các iđêan khác không của $A$ được chứa trong $m$ sao cho $a \supset b \supset a^2$. Ánh xạ $x \mapsto (x_1 \bmod b, \ldots, x_r \bmod b)$ của $G(a)$ vào $(a/b) \times \cdots \times (a/b)$ xác định khi chuyển qua thương một đẳng cấu của nhóm $G(a)/G(b)$ lên nhóm cộng $(a/b) \times \cdots \times (a/b)$.

Nếu $x \in G$ và $y \in G(a)$, các tọa độ của $x$ và $x.y$ bằng nhau modulo $a$. Do đó, với $x', x''$ trong $G$ và $y', y''$ trong $G(a)$, các tọa độ của $x'.x''$ và $(x'.y').(x''.y'')$ bằng nhau modulo $a$. Điều này chứng minh (i).

(ii) là hiển nhiên.

(iii) suy ra từ các kết quả trên và Tôpô đại cương, Chương III, § 7, Mệnh đề 2.

Nếu $x \in G(a)$ và $y \in G(a)$, các tọa độ của $x.y$ đồng dư với các tọa độ của $x + y$ modulo $G(a^2)$ theo công thức (4) của § 5. Điều này chứng minh (iv).

#### Hệ quả {#lie-iii-s7-n4-cor-1 .statement}

Giả sử rằng $K$ là compact địa phương và đặt $q = \mathrm{Card}(A/m)$.

(i) Nếu $a = m^a$ và $b = m^b$ với $b \geq a \geq 1$, $G(a)/G(b)$ là một $p$-nhóm có lực lượng $q^{r(b-a)}$.

(ii) $G(a)$ là một giới hạn ngược của các $p$-nhóm.

Số phần tử của $G(a)/G(b)$ là $(\mathrm{Card}(a/b))^r$; nếu $b = a + 1$, $a/b$ là một không gian vectơ 1 chiều trên $A/m$, do đó (i) trong trường hợp này; trường hợp tổng quát suy ra bằng quy nạp theo $b - a$. Mệnh đề (ii) suy ra từ (i) và Mệnh đề 5 (iii).

#### Mệnh đề 6 {#lie-iii-s7-prop-6 .statement}

Cho $a, b, c, c'$ là các iđêan khác không của $A$ được chứa trong $m$ sao cho

$$
c' \subset c, \quad ab \subset c, \quad ab^2 \subset c', \quad a^2b \subset c'.
$$

Nếu $x \in G(a)$ và $y \in G(b)$, thì $x^{[-1]}y^{[-1]}x.y, x.y.x^{[-1]}y^{[-1]}$ và $[x,y]$ thuộc $G(c')$ và đồng dư modulo $G(c')$.

Theo § 5, no. 2, Mệnh đề 1, tồn tại $c_{\alpha\beta} \in A'$ sao cho
$$
x^{[-1]}y^{[-1]}x.y - [x,y] = \sum_{|\alpha| + |\beta| \geq 3} c_{\alpha\beta} x^\alpha y^\beta.
$$
Nếu $x = 0$ hoặc $y = 0$, thì $x^{[-1]}y^{[-1]}x.y - [x,y] = 0$; do đó $c_{0\beta} = c_{\alpha 0} = 0$.
Mặt khác, các điều kiện
$$
x \in G(a), \quad y \in G(b), \quad |\alpha| \geq 1, \quad |\beta| \geq 1, \quad |\alpha| + |\beta| \geq 3
$$
suy ra
$$
c_{\alpha\beta} x^\alpha y^\beta \in G(a^2 b + ab^2) \subset G(c')
$$
và do đó $x^{[-1]}y^{[-1]}x.y - [x,y] \in G(c')$. Tương tự, ta thấy rằng
$$
x.y.x^{[-1]}y^{[-1]} - [x,y] \in G(c').
$$
Cuối cùng, theo § 5, công thức (13), $[x,y] \in G(ab) \subset G(c)$.

#### Mệnh đề 7 {#lie-iii-s7-prop-7 .statement}

(i) *Họ* $(G(a_\lambda))$ *là một phép lọc trung tâm trên* $G$ *(Chương II, § 4, no. 4, Định nghĩa 2)*.
(ii) *Đối với* $\lambda \in \mathbf{R}_+^*$, $G(a_\lambda) = \{ x \in G | \omega(x) \geq \lambda \}$, $G(a_\lambda^+) = \{ x \in G | \omega(x) > \lambda \}$.
(ii) là hiển nhiên. Ta chứng minh (i). Rõ ràng $G(a_\lambda) = \bigcap_{\mu < \lambda} G(a_\mu)$ và $G = \bigcup_{\lambda > 0} G(a_\lambda)$.
Mặt khác, nếu $x \in G(a_\lambda)$ và $y \in G(a_\mu)$, thì
$$
x^{[-1]}y^{[-1]}x.y \in G(a_{\lambda+\mu})
$$
theo Mệnh đề 6 được áp dụng với $a = a_\lambda, b = a_\mu, c = c' = a_{\lambda+\mu}$.

Theo Chương II, § 4, no. 4, ta có thể lập nhóm $\mathrm{gr}(G)$ liên kết với nhóm $G$, với phép lọc trung tâm $(G(a_\lambda))$. Viết $G_\lambda = G(a_\lambda)/G(a_\lambda^+)$ với mọi $\lambda > 0$, ta thu được $\mathrm{gr}(G) = \bigoplus_{\lambda > 0} G_\lambda$. Nhắc lại ( *cùng chỗ đã dẫn*, Mệnh đề 1) rằng giao hoán tử trong $G$ cho phép ta định nghĩa một móc trong $\mathrm{gr}(G)$, nhờ đó $\mathrm{gr}(G)$ là một đại số Lie, như sau: nếu $\bar{x} \in G_\lambda$ và $\bar{y} \in G_\mu$, chọn một đại diện $x$ của $\bar{x}$ trong $G(a_\lambda)$ và một đại diện $y$ của $\bar{y}$ trong $G(a_\mu)$; khi đó $[\bar{x}, \bar{y}]$ là lớp của $x^{[-1]}y^{[-1]}x.y \in G(a_{\lambda+\mu})$ trong $G_{\lambda+\mu}$. Theo Mệnh đề 6, được áp dụng với $a = a_\lambda, b = a_\mu, c = a_{\lambda+\mu}, c' = a_{\lambda+\mu}^+$, ta thấy rằng $[\bar{x}, \bar{y}]$ cũng là lớp của $[x, y]$ trong $G_{\lambda+\mu}$. Vì vậy, khi $G$ được xem như một đại số con Lie của $L(G) = K^r$, được lọc bởi các $G(a_\lambda)$, đại số Lie phân bậc liên kết (Chương II, § 4, no. 3) bằng $\mathrm{gr}(G)$.

### 5. LŨY THỪA TRONG CÁC NHÓM CHUẨN

Ta giữ nguyên ký hiệu của no. 4.

#### Mệnh đề 8 {#lie-iii-s7-prop-8 .statement}

*Cho* $n \in \mathbf{Z}$ *và* $h_n$ *là ánh xạ* $x \mapsto x^n$ *của* $G$ *vào* $G$. *Cho* $a$ *là một iđêan khác không của* $A$ *được chứa trong* $m$, *sao cho* $n \notin a$. *Khi đó* $h_n|G(a)$ *là một đẳng cấu của đa tạp giải tích* $G(a)$ *lên đa tạp giải tích* $G(na)$.

Theo định nghĩa của các nhóm chuẩn, $h_n$ bằng trên toàn bộ $G$ tổng của một chuỗi nguyên với các hệ số trong $A'$. Theo § 5, công thức (4), chuỗi này có dạng
$$
h_n(x) = nx + \sum_{|\alpha| \geq 2} a_\alpha x^\alpha.
$$
Do đó, với $x \in G$,
$$
\begin{align*}
h_n(nx) &= n^2 \left( x + \sum_{|\alpha| \geq 2} a_\alpha n^{|\alpha|-2} x^\alpha \right) \\
&= n^2 S(x)
\end{align*}
$$
trong đó ta viết $S(x) = x + \sum_{|\alpha| \geq 2} a_\alpha n^{|\alpha|-2} x^\alpha$. Chuỗi này $S(x)$ xác định một ánh xạ giải tích, cũng được ký hiệu là $S$, từ $G$ vào $G$. Theo *Đại số*, Chương IV, § 6, Mệnh đề 8, tồn tại một chuỗi nguyên $S'$ trong $r$ biến với các hệ số trong $A'$ sao cho $S'(S(X)) = S(S'(X)) = X$. Do đó $S$ là một đẳng cấu của đa tạp giải tích $G$ lên chính nó và, với mọi iđêan khác không $b$ của $A$ được chứa trong $m$, $S(G(b)) \subset G(b)$, $S'(G(b)) \subset G(b)$ và do đó
$$
S(G(b)) = G(b).
$$
Vì $h_n(y) = n^2 S \left( \frac{1}{n} y \right)$ với $y \in nG$, ta thấy rằng $h_n|nG(b)$ là một đẳng cấu của đa tạp giải tích $nG(b)$ lên đa tạp giải tích $n^2 G(b)$. Nhưng, vì $n \notin a$, $|n| > |\lambda|$ với mọi $\lambda \in a$, do đó $n^{-1} a \subset m$ và do đó $a$ có dạng $nb$ trong đó $b$ là một iđêan khác không của $A$ được chứa trong $m$.

#### Hệ quả {#lie-iii-s7-n5-cor-1 .statement}

*Nếu $n$ khả nghịch trong $A$, $h_n$ là một đẳng cấu của đa tạp giải tích* $G$ *lên chính nó. Với mọi iđêan khác không* $a$ *của* $A$ *được chứa trong* $m$, $h_n(G(a)) = G(a)$. *Với mọi* $x \in G$, $\omega(x^n) = \omega(x)$.*

Điều này suy ra ngay lập tức từ Mệnh đề 8.

#### Mệnh đề 9 {#lie-iii-s7-prop-9 .statement}

*Giả sử rằng $p \neq 0$.
(i) Cho $a, b$ là các iđêan khác không của $A$ sao cho $b \subset a \subset m$. Trong nhóm $G(a)/G(b)$, mọi phần tử đều có cấp là một lũy thừa của $p$.
(ii) Giả sử rằng $v(p) = 1$. Nếu $x \in G$ sao cho $\omega(x) > \frac{1}{p-1}$, thì*
$$
\omega(x^p) = \omega(x) + 1.
$$
Theo § 5, công thức (4), với mọi $x \in G$,
$$
x^p = px + \sum_{|\alpha| \geq 2} c_\alpha x^\alpha
$$
trong đó $c_\alpha \in A'$ với mọi $\alpha$. Ngay cả khi chứng minh (i), có thể giả sử rằng $v(p) = 1$. Khi đó nếu $\omega(x) \geq 1$, suy ra rằng $\omega(x^p) \geq \omega(x) + 1$ và do đó $\omega(x^{p^n})$ tiến tới $+\infty$ khi $n$ tiến tới $+\infty$; điều này chứng minh (i). Vì $\binom{p}{i}$ chia hết cho $p$ đối với $1 \leq i \leq p - 1$, Mệnh đề 2 của § 5, no. 3, chứng minh rằng $c_\alpha \in pA'$ đối với
$$
2 \leq |\alpha| \leq p - 1
$$
và do đó
$$
\omega(c_\alpha x^\alpha) > \omega(px) = \omega(x) + 1 \quad \text{đối với } 2 \leq |\alpha| \leq p - 1.
$$
Mặt khác, nếu $|\alpha| \geq p$, $\omega(c_\alpha x^\alpha) \geq p \omega(x)$ và $p \omega(x) > \omega(x) + 1$ nếu $\omega(x) > \frac{1}{p - 1}$. Điều này chứng minh (ii).

### 6. ÁNH XẠ LÔGARIT

#### Bổ đề 1 {#lie-iii-s7-lem-1 .statement}

Giả sử rằng $p \neq 0$. Cho $G$ là một nhóm Lie, $G_1$ là một nhóm con mở của $G$ đẳng cấu với một nhóm chuẩn và $x \in G$. Các điều kiện sau là tương đương:
(i) tồn tại một lũy thừa của $x$ thuộc về $G_1$;
(ii) tồn tại một dãy ngặt tăng $(n_i)$ các số nguyên sao cho $x^{n_i}$ tiến tới $e$ khi $i$ tiến tới $+\infty$.
(ii) $\Rightarrow$ (i): hiển nhiên.
(i) $\Rightarrow$ (ii): giả sử rằng $y = x^m \in G_1$. Theo Mệnh đề 9 (i) của no. 5, $y^{p^n}$ tiến tới $e$ khi $n$ tiến tới $+\infty$, nói cách khác $x^{m p^n}$ tiến tới $e$ khi $n$ tiến tới $+\infty$.

#### Mệnh đề 10 {#lie-iii-s7-prop-10 .statement}

Giả sử rằng $p \neq 0$. Cho $G$ là một nhóm Lie hữu hạn chiều. Cho $G_f$ là tập hợp các $x \in G$ sao cho tồn tại một dãy tăng ngặt $(n_i)$ các số nguyên sao cho $x^{n_i}$ tiến tới $e$ khi $i$ tiến tới $+\infty$.
(i) $G_f$ là mở trong $G$.
(ii) Tồn tại duy nhất một ánh xạ $\psi$ của $G_f$ vào $L(G)$ có các tính chất sau:
(a) $\psi(x^n) = n \psi(x)$ với mọi $x \in G_f$ và mọi $n \in \mathbf{Z}$;
(b) tồn tại một lân cận mở $V$ của $e$ trong $G$ sao cho $\psi|V$ là ánh xạ nghịch đảo của một ánh xạ mũ đơn ánh.
(iii) Ánh xạ $\psi$ là giải tích.

Tồn tại một nhóm con mở của $G$ đẳng cấu với một nhóm chuẩn (no. 3, Định lý 4). Mệnh đề (i) suy ra khi đó từ Bổ đề 1.

Cho $U$ là một nhóm con mở của $L(G)$ và $\phi : U \to \phi(U)$ là một ánh xạ mũ của $G$ với các tính chất của Mệnh đề 3 của no. 2. Có thể giả sử rằng $U$ đủ nhỏ để $\phi(U) \subset G_f$. Cho $x \in G_f$. Tồn tại $m \in \mathbf{Z} - \{0\}$ sao cho $x^m \in \phi(U)$. Phần tử $\frac{1}{m} \phi^{-1}(x^m)$ không phụ thuộc vào việc lựa chọn $m$. Thật vậy, cho $m' \in \mathbf{Z}$ sao cho $x^{m'} \in \phi(U)$. Khi đó $x^{m m'} \in \phi(U)$ và
$$
m' \phi^{-1}(x^m) = \phi^{-1}(x^{m m'}) = m \phi^{-1}(x^{m'})
$$
do đó có mệnh đề của chúng ta. Đặt $\psi(x) = \frac{1}{m} \phi^{-1}(x^m)$. Khi đó $\psi|\phi(U) = \phi^{-1}$. Mặt khác, nếu $n \in \mathbf{Z}$, thì
$$
\psi(x^n) = \frac{1}{m} \phi^{-1}(x^{nm}) = \frac{n}{m} \phi^{-1}(x^m) = n \psi(x).
$$

Vậy $\psi$ có các tính chất (a) và (b) của mệnh đề. Trong một lân cận của $x$, $\psi$ là hợp thành của các ánh xạ $x \mapsto x^m$, $y \mapsto \phi^{-1}(y)$ và $z \mapsto \frac{1}{m} z$; do đó $\psi$ là giải tích trên $G_f$.

Cuối cùng, cho $\psi'$ là một ánh xạ từ $G_f$ vào $L(G)$ và $V'$ là một lân cận của $e$ trong $G_f$ sao cho $\psi'(x^n) = n \psi'(x)$ với $x \in G_f$ và $n \in \mathbf{Z}$ và sao cho $\psi'|V'$ là ánh xạ nghịch đảo của một ánh xạ mũ đơn ánh. Khi đó $\psi$ và $\psi'$ trùng nhau trên một lân cận $W$ của $e$. Nếu $x \in G_f$, tồn tại $n \in \mathbf{Z}$ sao cho $x^n \in W$. Khi đó
$$
n \psi'(x) = \psi'(x^n) = \psi(x^n) = n \psi(x)
$$
và do đó $\psi = \psi'$.

#### Định nghĩa 2 {#lie-iii-s7-def-2 .statement}

*Ánh xạ $\psi$ của Mệnh đề 10 được gọi là ánh xạ logarit của $G$ và được ký hiệu bởi $\log_G$ hoặc đơn giản là $\log$.*

#### Mệnh đề 11 {#lie-iii-s7-prop-11 .statement}

*Giả sử rằng $p \neq 0$. Cho $x, y$ là hai phần tử giao hoán được của $G_f$. Khi đó $xy \in G_f$ và $\log(xy) = \log x + \log y$.*

Việc $xy \in G_f$ suy ra từ Bổ đề 1. Cho $U$ là một nhóm con mở của nhóm cộng tính $L(G)$ và $\phi : U \to \phi(U)$ là một ánh xạ mũ của $G$ với các tính chất của Mệnh đề 3 của no. 2; có thể giả sử rằng $U$ đủ nhỏ để $\log|\psi(U)|$ là ánh xạ nghịch đảo của $\phi$. Với $n \in \mathbf{Z} - \{0\}$ được chọn thích hợp, $x^n \in \phi(U)$, $y^n \in \phi(U)$. Đặt $u = \log x^n$, $v = \log y^n$, do đó $x^n = \phi(u)$, $y^n = \phi(v)$. Theo công thức (2), $[u, v] = 0$. Công thức Hausdorff chứng minh khi đó rằng $\phi(\lambda(u + v)) = \phi(\lambda u) \phi(\lambda v)$ với $|\lambda|$ đủ nhỏ; do đó, với mọi số nguyên $i$ đủ lớn,
$$
\phi(p^i(u + v)) = \phi(p^i u) \phi(p^i v)
$$
nghĩa là
$$
p^i (\log x^n + \log y^n) = \log(x^{np^i} y^{np^i})
$$
hoặc
$$
np^i (\log x + \log y) = np^i \log(xy).
$$

#### Mệnh đề 12 {#lie-iii-s7-prop-12 .statement}

*Giả sử rằng $p \neq 0$. Cho $x \in G_f$. Các điều kiện sau là tương đương:
(i) $\log x = 0$;
(ii) $x$ có cấp hữu hạn trong $G$.*

Nếu tồn tại một số nguyên $n > 0$ sao cho $x^n = e$, ta suy ra
$$
n \log x = \log x^n = 0,
$$
do đó $\log x = 0$. Nếu $\log x = 0$, gọi $V$ là một lân cận của $e$ trong $G_f$ sao cho $\log|V|$ là ánh xạ nghịch đảo của một ánh xạ mũ đơn ánh. Tồn tại một số nguyên $n > 0$ sao cho $x^n \in V$; đẳng thức $\log x^n = 0$ kéo theo $x^n = e$.

#### Mệnh đề 13 {#lie-iii-s7-prop-13 .statement}

*Giả sử rằng $p \neq 0$. Nếu $G$ là compact hoặc chuẩn, thì $G_f = G$.*

Nếu G là chuẩn, chỉ cần sử dụng Bổ đề 1. Giả sử rằng G là compact. Cho $x \in G$ và V là một lân cận của e trong G. Gọi y là một điểm giới hạn của dãy $(x^n)_{n \geq 0}$. Với mọi $n > 0$, tồn tại hai số nguyên $n_1, n_2$ sao cho $n_1 \geq 2n_2 \geq n$ và $x^{n_1} \in yV, x^{n_2} \in yV$, do đó $x^{n_1 - n_2} \in V^{-1}V$ và $n_1 - n_2 \geq n$. Suy ra $x \in G_f$.

#### Hệ quả {#lie-iii-s7-n6-cor-1 .statement}

*Giả sử rằng K là compact địa phương. Khi đó $G_f$ là hợp của các nhóm con compact của G.*

Cho $x \in G$. Nếu x thuộc một nhóm con compact của G, thì $x \in G_f$ (Mệnh đề 13). Giả sử rằng $x \in G_f$. Vì K là compact địa phương, tồn tại một nhóm con mở $G_1$ của G là compact. Khi đó tồn tại một số nguyên $m > 0$ sao cho $x^m \in G_1$. Nhóm con đóng $G_2$ sinh bởi $x^m$ được chứa trong $G_1$ và do đó là compact. Khi đó x giao hoán với các phần tử của $G_2$ và vì vậy $G_2 \cup xG_2 \cup \cdots \cup x^{m-1}G_2$ là một nhóm con compact của G chứa x.

#### Ví dụ {#lie-iii-s7-n6-exa-1 .statement}

Giả sử rằng K là compact địa phương. Gọi U là tập hợp các phần tử khả nghịch của A; nó là một nhóm con mở compact của nhóm Lie $K^*$. Khi đó $U \subset (K^*)_f$ theo Mệnh đề 13; mặt khác, nếu $x \in K^*$ sao cho $x \notin U$, thì hoặc $x^n$ tiến tới 0 khi n tiến tới $+\infty$, hoặc $x^n$ tiến tới 0 khi n tiến tới $-\infty$; do đó $U = (K^*)_f$. Hàm $\log_{K^*}$ được xác định và giải tích trên U, với các giá trị trong $L(K^*) = K$, và sao cho $\log_{K^*}(xy) = \log_{K^*}(x) + \log_{K^*}(y)$ với mọi $x, y$ trong U; các phần tử x của U sao cho $\log_{K^*}(x) = 0$ là các căn đơn vị của K.

Ta lại sử dụng ký hiệu của các số 3, 4 và 5.

#### Mệnh đề 14 {#lie-iii-s7-prop-14 .statement}

*Giả sử rằng $p \neq 0$ và v được chọn sao cho $v(p) = 1$. Cho G là một nhóm chuẩn và E(X) (tương ứng L(X)) là khai triển của hàm mũ của G (tương ứng hàm lôgarit của G) thành một chuỗi nguyên quanh 0.*

(i) *Miền hội tụ tuyệt đối* (Differentiable and Analytic Manifolds, R, 4.1.3) *của E chứa tập hợp $\Delta$ gồm các $x \in G$ sao cho $\omega(x) > \frac{1}{p-1}$. Gọi $E'$ là ánh xạ được xác định trên $\Delta$ bởi chuỗi này. Khi đó $E'$ là một ánh xạ mũ của G và là một đẳng cấu của đa tạp $\Delta$ lên chính nó.*

(ii) *Miền hội tụ tuyệt đối của L chứa G. Gọi $L'$ là ánh xạ trên G được xác định bởi chuỗi này. Khi đó $L'$ là ánh xạ logarit của G và hạn chế của $L'$ lên $\Delta$ là ánh xạ nghịch đảo của $E'$.*

(iii) *Ánh xạ $E'$ là một đẳng cấu của $\Delta$, với luật Hausdorff, lên nhóm con $\Delta$ của G.*

Sử dụng ký hiệu của § 5, các số 3 và 4, $E = \sum_{m \geq 1} \frac{\psi_{m,m}}{m!}$ ($\S 5$, no. 4, Mệnh đề 3). Vì các hệ số $c_{\alpha \beta \gamma}$ thuộc A, $\| \psi_{m,m} \| \leq 1$ (Differentiable and Analytic Manifolds, R, Phụ lục) $K^r$ được giả sử có chuẩn

$$
\| (\lambda_1, \ldots, \lambda_r ) \| = \sup(|\lambda_1|, \ldots, |\lambda_r|)
$$

Theo Chương II, § 8, no. 1, Bổ đề 1, $v(m!) \leq \frac{m-1}{p-1}$. Nếu $\omega(x) > \frac{1}{p-1}$, ta thấy rằng $m \omega(x) - v(m!)$ tiến tới $+\infty$ khi m tiến tới vô hạn, do đó
$$
\left\| \frac{\psi_{m,m}}{m!} \right\| \|x\|^m \leq \frac{1}{|m!|} \|x\|^m
$$
tiến tới 0 khi m tiến tới $+\infty$ và
$$
\omega\left( \frac{\psi_{m,m}(x)}{m!} \right) > \frac{m}{p-1} - \frac{m-1}{p-1} = \frac{1}{p-1} \quad \text{cho } m \geq 1.
$$
Do đó $\Delta$ được chứa trong miền hội tụ tuyệt đối của $E$ và $E'(\Delta) \subset \Delta$. Rõ ràng $E'$ là một ánh xạ mũ.

Nếu $L_m$ là thành phần thuần nhất của $L$ có bậc m, Mệnh đề 3 của § 5, no. 4, chứng minh rằng mỗi hệ số của $L_m$ có dạng
$$
a_1 + \frac{1}{2} a_2 + \cdots + \frac{1}{m} a_m
$$
với $a_1, a_2, \ldots, a_m$ thuộc A; nhưng
$$
\inf \left( v(1), v\left( \frac{1}{2} \right), \ldots, v\left( \frac{1}{m} \right) \right) = o(\log m) \quad \text{as } m \text{ tends to } +\infty
$$
và
$$
\inf \left( v(1), v\left( \frac{1}{2} \right), \ldots, v\left( \frac{1}{m} \right) \right) \geq v\left( \frac{1}{m!} \right) \geq -\frac{m-1}{p-1}.
$$
Do đó, nếu $\omega(x) > 0$, $\|L_m\| \cdot \|x\|^m$ tiến tới 0 khi m tiến tới $+\infty$, vì vậy G được chứa trong miền hội tụ tuyệt đối của $L$. Mặt khác, nếu $\omega(x) > \frac{m}{p-1}$, thì $\omega(L_m(x)) > \frac{m}{p-1} - \frac{m-1}{p-1} = \frac{1}{p-1}$ với $m \geq 1$ và do đó $L'(\Delta) \subset \Delta$.

Vì các chuỗi lũy thừa hình thức $L(E(X))$ và $E(L(X))$ đều bằng X, no. 4.1.5 của *Differentiable and Analytic Manifolds*, R, chứng minh rằng
$$
L'(E'(x)) = E'(L'(x)) = x
$$
với $x \in \Delta$. Do đó $E'$ là một đẳng cấu của đa tạp $\Delta$ lên chính nó và đẳng cấu nghịch đảo là hạn chế của $L'$ lên $\Delta$.

$L(X^{[n]}) = nL(X)$ với $n$ là một số nguyên $> 0$ (xem § 5, no. 4). Vì $G$ được chứa trong miền hội tụ tuyệt đối của $L$ và $X^{[n]}$, do đó $L'(x^n) = nL'(x)$ với mọi $x \in G$. Quan hệ $L'|_{\Delta} = E'^{-1}$ kéo theo rằng $L'(x^n) = \log x^n$ với $n$ đủ lớn. Suy ra $L'(x) = \log x$. Như vậy ta đã chứng minh được (i) và (ii).

Gọi $H = \sum_{r,s \geq 0} H_{r,s}$ là chuỗi lũy thừa hình thức Hausdorff và $h$ là hàm Hausdorff tương ứng với $L(G)$. Miền hội tụ tuyệt đối của $\tilde{H}$ chứa $\Delta \times \Delta$ và $h$ được xác định trên $\Delta \times \Delta$ (Chương II, § 8, Mệnh đề 2). Khi đó
$$
E'(x)E'(y) = E'(h(x, y))
$$
với $x, y$ đủ gần 0 ($\S 4$, Định lý 4 (v)). Do đó, theo ký hiệu của no. 3, Định nghĩa 1, các chuỗi lũy thừa hình thức $F(E(X), E(Y))$ và $E(H(X, Y))$ bằng nhau. Cho $x, y$ là các phần tử của $\Delta$. Khi đó
$$
\sup_m \left| \frac{\psi_{m,m}}{m!} \right| (\sup \|x\|, \|y\|)^m < 1 \\
\sup_{r,s} \|H_{r,s}\| \|x\|^r \|y\|^s < |\rho|^{1/(p-1)}
$$
theo Chương II, § 8, công thức (14). Theo *Differentiable and Analytic Manifolds*, R, 4.1.5, $E'(x)E'(y)$ thu được bằng cách thế $x$ vào $X$ và $y$ vào $Y$ trong
$$
F(E(X), E(Y))
$$
và $E'(h(x, y))$ thu được bằng cách thế $x$ vào $X$ và $y$ vào $Y$ trong $E(H(X, Y))$. Do đó $E'(x)E'(y) = E'(h(x, y))$.

### Bài tập {#lie-iii-s7-exercises}

Xem [các bài tập cho § 7](exercises/s7/).
