---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 14
section_title: Opérateurs différentiels
lang: vi
source: var-fr
pdf_pages: 0162-0173
extraction: ocr
subsections:
    - "no": 1
      title: Opérateurs différentiels
      page: 0
      pdf_page: 162
    - "no": 2
      title: Symboles
      page: 0
      pdf_page: 166
    - "no": 3
      title: Transposition
      page: 0
      pdf_page: 169
    - "no": 4
      title: Exemples
      page: 0
      pdf_page: 172
statements: 2
exercises: 0
content_sha256: 49d62faf8a62896ba40f633416bd1a6df0c969ab6a34c77313b4b4b7b2b78af7
translated_from: content/en-mt/var/2/14_s14_operateurs_differentiels.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 5c066a3a7c489633b6dc0c6772b855625588fe75961eda95b9df4cb8b5ca50c8
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-abfa588b
glossary_version: 34
glossary_terms_sha256: 4881bba15c985362244afdb7530587226e11d793745b6b96cfd2463c7e909b39
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 14. Toán tử vi phân

Trong đoạn này, X ký hiệu một đa tạp hữu hạn chiều địa phương lớp $C^r$, trong đó $r \in \mathbf{N}_k$; E và F ký hiệu hai bó vectơ hạng hữu hạn lớp $C^r$ và có cơ sở X.

Mọi đa tạp và bó vectơ được xét đều được giả thiết là hữu hạn chiều địa phương.

### 14.1. Toán tử vi phân

### 14.1.1. Cho k là một số nguyên sao cho $0 \leq k \leq r$, và cho $P^k(E)$ là bó các jet của các tiết diện của E cấp k (12.6.1). Đặt

$$
D^k(E,F)=\mathscr{L}(P^k(E);F).
$$

Đây là một bó vectơ có cơ sở X và lớp $C^{r-k}$. Một tiết diện của bó này trên một tập mở U của X được đồng nhất với một ánh xạ

$$
D:P^k(E)|U\longrightarrow F|U
$$

giao hoán với phép chiếu lên U và tuyến tính trên mỗi thớ; một tiết diện như vậy được gọi là một toán tử vi phân trên U, kiểu $E \rightarrow F$, và cấp $\leq k$. Cho $h \in \mathbf{N}_k \cup \{0\}$, với $0 \leq h \leq r-k$. Ta ký hiệu $\mathscr{D}^{k,h}_U(E,F)$ là tập hợp các toán tử vi phân trên U, kiểu $E \rightarrow F$ và cấp $\leq k$, có lớp $C^h$ (xét như các tiết diện của $D^k(E,F)$, hoặc như các cấu xạ từ $P^k(E)|U$ vào $F|U$, thì hai cách này là tương đương). Nếu $M=D^k(E,F)$, ta có $\mathscr{D}^{k,h}_U(E,F)=\mathscr{F}^h_M(U)$; đây là một môđun trên $\mathscr{C}^h(U)$, cf. 7.4.1.

Nếu $0 \leq k' \leq k$, cấu xạ $r^{k,k'}:P^k(E)\longrightarrow P^{k'}(E)$ (cf. 12.6.6) xác định một đơn ánh từ $D^{k'}(E,F)$ vào $D^k(E,F)$; do đó mọi toán tử vi phân cấp $\leq k'$ đều được đồng nhất với một toán tử vi phân cấp $\leq k$. Một toán tử vi phân cấp $\leq k$ mà không có cấp $\leq k-1$ đôi khi được gọi là có cấp k. Nếu $h \in \mathbf{N}_k \cup \{0\}$ và $h \leq r-k$, và nếu U là một tập mở của X, ta có:

$$
0 \subset \mathscr{D}^{0,h}_U(E,F) \subset \mathscr{D}^{1,h}_U(E,F) \subset \cdots \subset \mathscr{D}^{k,h}_U(E,F).
$$

Nếu $r=\infty$ hoặc $\omega$, ta ký hiệu $\mathscr{D}^{\omega,h}_U(E,F)$ là hợp của các $\mathscr{D}^{k,h}_U(E,F)$ với $k \geq 0$; một phần tử của hợp này được gọi là một toán tử vi phân trên U có cấp bị chặn (kiểu $E \rightarrow F$, lớp $C^h$) hoặc đôi khi đơn giản là một toán tử vi phân trên U.

### 14.1.2. (« Các toán tử cấp không »). Ta có $P^0(E)=E$ (12.5.1) và $D^0(E,F)=\mathscr{L}(E;F)$. Nếu U là mở trong X, và nếu $h \in \mathbf{N}_k \cup \{0\}$ và $h \leq r$, một phần tử của $\mathscr{D}^{0,h}_U(E,F)$ là một cấu xạ lớp $C^h$ từ $E|U$ vào $F|U$.

14.1.3 (“Sự suy yếu của cấu trúc”). Giả sử rằng $K = \mathbf{R}$, và cho $r' \in \mathbf{N}_\mathbf{R}$ với $r' \leq r$. Gọi $X', E'$ và $F'$ lần lượt là đa tạp và các bó vectơ lớp $C^{r'}$ nhận được từ $X, E,$ và $F$ bằng cách suy yếu cấu trúc. Cho $k$ là một số nguyên sao cho $0 \leq k \leq r'$. Khi đó $P^k(E')$ là bó lớp $C^{r'-k}$ suy ra từ $P^k(E)$ bằng cách suy yếu cấu trúc, và có một kết quả tương tự đối với $D^k(E', F')$. Đặc biệt, nếu $U$ mở trong $X$, và nếu $0 \leq h \leq r - k'$, thì có $\mathscr{D}_U^{k',h}(E', F') = \mathscr{D}_U^{k,h}(E, F)$.

14.1.4. Cho $D$ là một toán tử vi phân trên $X$, kiểu $E \to F$, cấp $\leq k$ (trong đó $0 \leq k \leq r$). Cho $U$ là một tập hợp mở trong $X$, và cho $s$ là một tiết diện lớp $C^m$ của $E$ trên $U$, với $m \in \mathbf{N}_K \cup \{0\}$ và $k \leq m \leq r$. Khi đó $j^k(s)$ là một tiết diện lớp $C^{m-k}$ của $P^k(E)$ trên $U$ (12.6.1); ảnh của nó qua $D$ được ký hiệu là $D_U(s)$, hoặc $D(s)$. Nó là một tiết diện của $F|U$. Giả sử rằng $D$ thuộc lớp $C^h$, trong đó $h = m - k$. Khi đó $D_U(s)$ thuộc lớp $C^h$, và các ánh xạ
$$
D_U : \mathscr{S}_E^m(U) \to \mathscr{S}_F^h(U)
$$
thu được như vậy có các tính chất sau:

(1) $D_U$ là $K$-tuyến tính.
(2) Với mọi $s \in \mathscr{S}_E^m(U)$ và mọi tập mở $V$ của $U$, ta có $D_V(s|V) = D_U(s)|V$.
(3) Với mọi $s \in \mathscr{S}_E^m(U)$ và mọi $x \in U$ sao cho $j_x^k(s) = 0$, ta có $D_U(s)(x) = 0$.
(3') Với mọi hệ tọa độ $\xi = (\xi^1, \ldots, \xi^n)$ trong $U$ và mọi khung $s = (s_1, \ldots, s_d)$ của $E$ trên $U$ (7.4.4), tồn tại các nhát cắt $n_{i,\alpha} (1 \leq i \leq d, \alpha \in \mathbf{N}^n, |\alpha| \leq k)$ của $F$ trên $U$, thuộc lớp $C^h$ và sao cho, với mọi họ $(f_i)_{1 \leq i \leq d}$ các phần tử của $\mathscr{C}^m(U)$, ta có
$$
D_U \left( \sum_{1 \leq i \leq d} f_i . s_i \right) = \sum_{1 \leq i \leq d, |\alpha| \leq k} \Delta_\xi^\alpha(f_i) . n_{i,\alpha}, \quad \text{(cf. 13.2.6).}
$$
(4) Với mọi hàm $f \in \mathscr{C}^m(U)$ và mọi ánh xạ $\theta$ từ $\mathscr{S}_U^m(E)$ vào $\mathscr{S}_U^h(F)$, gọi $\operatorname{ad}(f)\theta$ là ánh xạ
$$
s \mapsto f . \theta(s) - \theta(f.s)
$$
từ $\mathscr{S}_U^m(E)$ vào $\mathscr{S}_U^h(F)$. Khi đó, với mọi hàm $f \in \mathscr{C}^m(U)$, tồn tại một toán tử vi phân $L$ trên $U$, kiểu $E \to F$, cấp $\leq k - 1$ và thuộc lớp $C^h$ sao cho
$$
(\operatorname{ad}(f)D_U)(s) = L_U(s) \quad \text{với mọi } s \in \mathscr{S}_U^m(E).
$$
(5) Ta có
$$
\operatorname{ad}(f_0) \ldots \operatorname{ad}(f_k) D_U = 0 \quad \text{với mọi } f_0, \ldots, f_k \text{ trong } \mathscr{C}^m(U).
$$
Nếu đặt $I = \{0, \ldots, k\}$ và $f_H = \prod_{i \in H} f_i$ với mọi tập con $H$ của $I$, thì quan hệ trước tương đương với:
$$
\sum_{H \subset I} (-1)^{\operatorname{Card}(H)} f_H . D_U(f_{I-H}.s) = 0
$$
với mọi $f_0, \ldots, f_k$ tùy ý trong $\mathscr{C}^m(U)$ và $s$ trong $\mathscr{S}_E^m(U)$.

14.1.5 ("Đặc trưng hóa các toán tử vi phân"). Cho $k, m$ và $h = m - k$ như trong 14.1.4. Với mọi tập mở $U$ của $X$, gọi $D_U$ là một ánh xạ từ $\mathscr{S}_E^m(U)$ vào $\mathscr{S}_F^h(U)$. Giả sử rằng các điều kiện 1, 2, 3 (tương ứng 1, 2, 3') của 14.1.4 được thỏa mãn đối với mọi tập con mở U của X. Khi đó tồn tại một phần tử D của $\mathscr{D}_X^{k,h}(E, F)$, và chỉ một phần tử, sao cho các $D_U$ là các ánh xạ tương ứng.$^{(1)}$ Trong phần tiếp theo, D được đồng nhất với họ các $D_U$.

Khi $m = \infty$ hoặc $\omega$, ta có $h = m$ và có thể thay thế các điều kiện (3) và (3') bằng một trong hai điều kiện (4) và (5).

14.1.6 (“Các toán tử vi phân vô hướng”). Giả sử E và F bằng bó vectơ tầm thường $K_X$. Khi đó, một toán tử vi phân kiểu $E \to F$ được gọi là toán tử vi phân *vô hướng* hoặc đơn giản là một toán tử vi phân; nếu nó có cấp $\leq k$, thì nó là một tiết diện của bó vectơ $\mathscr{L}(P^k(X); K_X) = P^k(X)^*$, *đối ngẫu* của bó vectơ $P^k(X)$; sử dụng đẳng cấu
$$
i^{-1} : P^k(X)^* \to T^{(k)}(X) \quad (\text{cf. } 13.2.5),
$$
ta thấy rằng một toán tử vi phân vô hướng có cấp $\leq k$ được đồng nhất với một *tiết diện* của bó vectơ $T^{(k)}(X)$, tức là với một *trường các phân bố điểm có cấp* $\leq k$.

Đặc biệt, lấy X là một tập con mở của $K^n$, trong đó n là một số nguyên $\geq 0$. Các trường các phân bố điểm
$$
\Delta^\alpha : x \mapsto \Delta_x^\alpha \quad (\text{cf. } 13.2.6)
$$
là các toán tử vi phân vô hướng thuộc lớp $C^\omega$. Với mọi $h \in N_K$, các $\Delta^\alpha$ với $(|\alpha| \leq k)$ tạo thành một *cơ sở* của $C^h(X)$-môđun $\mathscr{D}_X^{k,h}(K_X, K_X)$.

14.1.7 (“Các toán tử vi phân phức trên một đa tạp thực”). Giả sử $K = \mathbf{R}$ và các bó vectơ E và F được trang bị *các cấu trúc phức* (8.8.1); cho k là một số nguyên sao cho $0 \leq k \leq r$. Khi đó bó vectơ $P^k(E)$ được trang bị một cấu trúc phức (12.6.3); bó vectơ $\mathscr{L}_c(P^k(E); F)$ (7.8.5) gồm các ánh xạ tuyến tính *phức* từ $P^k(E)$ vào F là một bó vectơ con của $\mathscr{L}(P^k(E); F) = D^k(E, F)$; ta ký hiệu nó là $D_c^k(E, F)$. Một tiết diện của $D_c^k(E, F)$ được gọi là một toán tử vi phân *phức*, kiểu $E \to F$ và cấp $\leq k$. Nếu $h \in N_K$ và $h \leq r - k$, và nếu U là một tập con mở của X, ta cũng ký hiệu bằng $\mathscr{D}_U^{k,h}(E, F)_c$ không gian các tiết diện thuộc lớp $C^h$ của $D_c^k(E, F)$ trên U; nó là một không gian vectơ C. Các định nghĩa và kết quả khác của đoạn này được mở rộng tương tự cho các toán tử vi phân phức; ta dành việc phát biểu chúng cho người đọc.

14.1.8 (« Hợp thành »). Cho G là một bó vectơ lớp $C^r$ và có cơ sở X. Cho $k'$ và $k''$ là các số nguyên dương có tổng $k \leq r$, và cho $D'$ (resp. $D''$) là một toán tử vi phân trên X, kiểu $E \to F$ (resp. kiểu $F \to G$), cấp $\leq k'$ (resp. $\leq k''$). Giả sử $D' : P^{k'}(E) \to F$ có lớp $C^{h'}$, với $h' \in N_K \cup \{0\}$ và $k'' \leq h' \leq r - k'$; ánh xạ
$$
D'_* = P^{k''}(D') : P^{k''}(P^{k'}(E)) \to P^{k''}(F)
$$
có lớp $C^{h'-k''}$ (12.6.3). Gọi $\beta$ là đồng cấu chính tắc từ $P^{k}(E)$ vào $P^{k''}(P^{k'}(E))$, xem 12.6.5. Bằng cách lấy hợp thành các ánh xạ
$$
P^k(E) \xrightarrow{\beta} P^{k''}(P^{k'}(E)) \xrightarrow{D'_*} P^{k''}(F) \xrightarrow{D''} G,
$$
ta được một toán tử vi phân kiểu $E \to G$ và cấp $\leq k$. Toán tử này được gọi là *hợp thành* của $D''$ và $D'$; nó được ký hiệu bởi $D'' \circ D'$.

$^1$ Thực ra chỉ cần điều kiện (3') được thỏa mãn đối với một họ $(\xi_\lambda)$ các hệ tọa độ và một họ các cơ sở $(s_\lambda)$ mà các miền của chúng phủ X.

Nếu U là một tập con mở của X, và nếu s ∈ $\mathscr{S}_E^{k}(U)$, thì
$$
(D'' \circ D')(s) = D''(D'(s))
$$
(trong đó hai vế là các tiết diện của G trên U); điều này biện minh cho thuật ngữ và ký hiệu đã dùng.

Giả sử bây giờ rằng D'' có lớp $C^{h''}$, với $h'' \in \mathbf{N}_K \cup \{0\}$ và $h'' \leq r - k''$. Khi đó $D'' \circ D'$ có lớp $C^h$, với $h = \inf(h' - k'', h'')$.

Giả sử $E = F = G$, và $k' \leq h''$, trong trường hợp đó $D' \circ D''$ được xác định. Khi đó $D' \circ D'' - D'' \circ D'$ là một toán tử vi phân kiểu $E \to E$ và cấp $\leq k - 1$; nó được ký hiệu bởi $[D', D'']$.

14.1.9 (« Tính kết hợp »). Với ký hiệu và các giả thiết của 14.1.8, cho H là một bó vectơ lớp $C^r$ và có cơ sở X, và cho $D'''$ là một toán tử vi phân trên X, kiểu $G \to H$ và cấp $\leq k'''$, với $k' + k'' + k''' \leq r$. Giả sử rằng $D'$ có lớp $C^{h'}$, với $h' \in \mathbf{N}_K \cup \{0\}$ và $k'' + k''' \leq h' \leq r - k'$ và rằng $D''$ có lớp $C^{h''}$, với $h'' \in \mathbf{N}_K \cup \{0\}$ và $k''' \leq h'' \leq r - k''$. Khi đó các hợp thành
$$
D''' \circ (D'' \circ D') \quad \text{và} \quad (D''' \circ D'') \circ D'
$$
được xác định và bằng nhau.

14.1.10. Các ví dụ

a) Cho U là một tập con mở của X, cho $D \in \mathscr{D}_U^{k,h}(E, F)$ với $h \in \mathbf{N}_K \cup \{0\}$ và $h \leq r - k$, và cho $f \in \mathscr{C}^{h+k}(U)$ (tương ứng $f \in \mathscr{C}^h(U)$). Phép nhân với f trong E (tương ứng F) là một toán tử vi phân trên U có cấp $\leq 0$, và có kiểu $E \to E$ (tương ứng $F \to F$), xem 14.1.2. Các hợp thành $D \circ f$ và $f \circ D$ được xác định và thuộc $\mathscr{D}_U^{k,h}(E; F)$; ta đặt
$$
\operatorname{ad}(f)D = f \circ D - D \circ f \in \mathscr{D}_U^{k-1,h}(E, F),
$$
xem 14.1.4, (4). Như vậy $\mathscr{D}_U^{k,h}(E, F)$ được trang bị một cấu trúc môđun $\mathscr{C}^{h+k}(U)$ bên phải (tương ứng một cấu trúc môđun $\mathscr{C}^h(U)$ bên trái). Cấu trúc môđun bên trái trùng với cấu trúc trong 14.1.1.

b) Giả sử $r = \infty$ hoặc $r = \omega$. Các toán tử vi phân có kiểu $E \to E$ và thuộc lớp $C^r$ tạo thành một đại số kết hợp trên K với phần tử đơn vị.

c) Lấy X là một tập con mở của $K^n$. Các toán tử vi phân vô hướng $\Delta^\alpha$ (14.1.6) thỏa mãn các công thức
$$
\Delta^\alpha \circ \Delta^\beta = ((\alpha, \beta)) \Delta^{\alpha+\beta}.
$$
Chúng giao hoán với nhau. Ký hiệu $D_i$ là toán tử $\Delta^{\varepsilon_i}$ (« đạo hàm riêng thứ i »). Nếu K có đặc số 0, ta có
$$
\Delta^\alpha = \frac{1}{\alpha!} D_1^{\alpha_1} \ldots D_n^{\alpha_n}.
$$
Nếu K có đặc số $p \neq 0$, ta có $D_i^p = 0$ với mọi $i$.

14.1.11 (« Các toán tử vi phân nhiều biến »). Cho $E_1, \ldots, E_n$ là các bó vectơ thuộc lớp $C^r$ và có cơ sở X, và cho $k, k_1, \ldots, k_n$ là các số nguyên thuộc $[0, r]$. Đặt
$$
L(k_1, \ldots, k_n) = \mathscr{L}(P^{k_1}(E_1) \otimes \cdots \otimes P^{k_n}(E_n); F).
$$

Nếu $k_i \leq k$ với mọi $i$, các phép chiếu $r^{k_i, k_i} : P^k(E_i) \to P^{k_i}(E_i)$ làm cho có thể đồng nhất bó $L(k_1, \ldots, k_n)$ với một bó con của bó $L(k) = L(k, \ldots, k)$. Tồn tại một bó con nhỏ nhất $M(k)$ của $L(k)$ chứa tất cả các bó con $L(k_1, \ldots, k_n)$, với $k_1 + \cdots + k_n = k$. Một tiết diện $H$ của $M(k)$ được gọi là một toán tử $n$-vi phân (hoặc đa vi phân) kiểu $(E_1, \ldots, E_n) \to F$ và cấp $\leq k$. Nếu $s_i$ ($1 \leq i \leq n$) là một tiết diện lớp $C^m$ ($m \in \mathbf{N}_K, m \geq k$) của $E_i$ trên một tập mở $U$ của $X$, ta định nghĩa $H_U(s_1, \ldots, s_n) = H(s_1, \ldots, s_n)$ là ảnh dưới $H$ của tiết diện $j^k(s_1) \otimes \cdots \otimes j^k(s_n)$ của bó
$$
P^k(E_1) \otimes \cdots \otimes P^k(E_n).
$$
Đó là một tiết diện của $F|U$. Nếu $H$ thuộc lớp $C^h$, tiết diện này thuộc lớp $C^p$ với $p = \inf(m - k, h)$.

Khi $E_1, \ldots, E_n$ và $F$ đều bằng $K_X$, người ta nói rằng $H$ là một toán tử $n$-vi phân vô hướng (hoặc đa vi phân).

#### Ví dụ {#var-2-s14-n1-exa-1 .statement}

Cho $J$ là một tập hợp hữu hạn, và $X$ là một tập mở của $K^J$. Cho $H$ là một toán tử $n$-vi phân vô hướng cấp $\leq k$ trên $X$. Tồn tại một họ duy nhất các hàm vô hướng
$$
c(\alpha(1), \ldots, \alpha(n))_{(\alpha(1), \ldots, \alpha(n)) \in \mathbf{N}^J}, \quad \sum_{i=1}^n |\alpha(i)| \leq k
$$
trên $X$ sao cho
$$
H_X(f_1, \ldots, f_n) = \sum_{\alpha(1), \ldots, \alpha(n)} c(\alpha(1), \ldots, \alpha(n)) \Delta^{\alpha(1)}(f_1) \ldots \Delta^{\alpha(n)}(f_n)
$$
với mọi họ $(f_1, \ldots, f_n)$ các hàm thuộc lớp $C^k$ trên $X$. Để $H$ thuộc lớp $C^h$, điều kiện cần và đủ là các hàm $c(\alpha(1), \ldots, \alpha(n))$ thuộc lớp $C^h$.

### 14.2. Các ký hiệu.

14.2.1. Cho $k$ là một số nguyên dương $\leq r$. Xét dãy khớp
$$
0 \to P_k(T(X); E) \xrightarrow{i'} P^k(E) \xrightarrow{j'} P^{k-1}(E) \to 0
$$
của No. 12.6.8, trong đó $j = r^{k, k-1}$. Áp dụng hàm tử bó vectơ $M \mapsto \mathscr{L}(M; F)$ vào dãy này, ta thu được dãy khớp
$$
0 \to \mathscr{L}(P^{k-1}(E); F) \xrightarrow{j''} \mathscr{L}(P^k(E); F) \xrightarrow{\sigma_k} \mathscr{L}(P_k(T(X); E); F) \to 0
$$
có thể được viết:
$$
0 \to D^{k-1}(E, F) \xrightarrow{j''} D^k(E, F) \xrightarrow{\sigma_k} S^k(E, F) \to 0
$$
bằng cách đặt
$$
S^k(E, F) = \mathscr{L}(P_k(T(X); E); F).
$$
Đồng cấu $j' = \mathscr{L}(j; \mathrm{Id}_F)$ là phép nhúng chính tắc của $D^{k-1}(E, F)$ vào $D^k(E, F)$; đồng cấu $\sigma_k$ thì, theo định nghĩa, bằng $\mathscr{L}(i; \mathrm{Id}_F)$. Nếu $D$ là một toán tử vi phân kiểu $E \to F$ và có cấp $\leq k$, ảnh của nó qua $\sigma_k$ là một tiết diện $\sigma_k(D)$ của $S^k(E, F)$ được gọi là $k$-ký hiệu (hoặc đơn giản là ký hiệu) của $D$; ta có $\sigma_k(D) = 0$ khi và chỉ khi $D$ có cấp $\leq k-1$. Nếu $D$ có lớp $C^h$, điều tương tự cũng đúng đối với ký hiệu của nó.

14.2.2 (« Các phép đồng nhất của bó ký hiệu »). Bó $S^k(E, F) = \mathscr{L}(P_k(T(X); E); F)$ có thể được viết theo nhiều cách khác nhau. Trước hết, nếu $x \in X$, một phần tử của $P_k(T_x(X); E_x)$ được đồng nhất (13.1.2) với một phần tử của $\mathscr{L}(TS^k(T_x(X)); E_x)$. Do đó ta thu được các phép đồng nhất của các bó vectơ

$$
P_k(T(X); E) = \mathscr{L}(TS^k(T(X)); E) = (TS^k(T(X)))* \otimes E
$$

và, áp dụng hàm tử bó vectơ $M \mapsto \mathscr{L}(M; F) = M^* \otimes F$, ta thu được:

$$
S^k(E, F) = TS^k(T(X)) \otimes E^* \otimes F = TS^k(T(X)) \otimes \mathscr{L}(E; F).
$$

Biểu thức trước đó có thể được biến đổi thêm. Nếu $M$ và $N$ là hai bó vectơ, gọi $\mathrm{Sym}^k(M; N)$ là bó con của $\mathscr{L}(M, \ldots, M; N)$ tạo bởi các ánh xạ $k$-tuyến tính đối xứng. Ta có một đẳng cấu chính tắc

$$
\mathrm{Sym}^k(M; N) \to \mathrm{Sym}^k(M; K_X) \otimes N;
$$

mặt khác, đối ngẫu giữa $\otimes^k M$ và $\otimes^k M^*$ đồng nhất $\mathrm{Sym}^k(M; K_X)$ với $TS^k(M^*)$. Do đó ta thu được một phép đồng nhất

$$
\mathrm{Sym}^k(M; N) = TS^k(M^*) \otimes N.
$$

Áp dụng công thức này cho $M = T(X)^*$ và $N = \mathscr{L}(E; F)$, ta có:

$$
S^k(E, F) = TS^k(T(X)) \otimes \mathscr{L}(E; F) = \mathrm{Sym}^k(T(X)^*; \mathscr{L}(E; F)).
$$

Giả sử $K$ có đặc số 0 hoặc $> k$. Nếu $u$ là một ánh xạ $k$-tuyến tính đối xứng, gọi $\tilde{u}$ là ánh xạ đa thức

$$
x \mapsto \frac{1}{k!} u(x, \ldots, x)
$$

tương ứng với nó. Ánh xạ $u \mapsto \tilde{u}$ xác định một đẳng cấu

$$
S^k(E, F) = \mathrm{Sym}^k(T(X)^*, \mathscr{L}(E; F)) \to P_k(T(X)^*; \mathscr{L}(E; F)).
$$

Do đó, mọi phần tử $\sigma$ của $S^k(E, F)_x$, với $x \in X$, đều có thể được đồng nhất với một ánh xạ đa thức thuần nhất $\tilde{\sigma}$ bậc $k$ từ $T_x(X)^*$ vào $\mathscr{L}(E_x; F_x)$.

14.2.3 (“Tính toán ký hiệu của một toán tử vi phân”). Cho $x \in X$ và cho $D$ là một toán tử vi phân kiểu $E \to F$, cấp $\leq k$, được xác định trong một lân cận mở của $x$ và thuộc lớp $C^{r-k}$. Ta sẽ làm tường minh giá trị $\sigma_k(D)(x)$ của ký hiệu của $D$ tại $x$. Xét nó như một phần tử của $\mathrm{Sym}^k(T_x(X)^*; \mathscr{L}(E_x; F_x))$ (cf. 14.2.2). Cho $\omega_1, \ldots, \omega_k$ là các đối covectơ tại $x$ và chọn các hàm $f_1, \ldots, f_k$ thuộc lớp $C^r$ trong một lân cận mở $U$ của $x$ sao cho $d_x f_i = \omega_i$ với $i = 1, \ldots, k$. Đặt

$$
D' = (-1)^k \mathrm{ad}\,(f_k) \ldots \mathrm{ad}(f_1)D \quad (\text{cf. } 14.1.10, a).
$$

Toán tử $D'$ có cấp $\leq 0$; nó là một tiết diện của $\mathscr{L}(E; F)|U$. Giá trị của $D'$ tại $x$ là một phần tử $\lambda(\omega_1, \ldots, \omega_k)$ của $\mathscr{L}(E_x; F_x)$ chỉ phụ thuộc vào $(\omega_1, \ldots, \omega_k)$. Ánh xạ thu được $\lambda$ là đối xứng. *Nó bằng ký hiệu $\sigma_k(D)(x)$ của $D$ tại $x$*.

Giả sử rằng $K = \mathbf{R}$ hoặc $\mathbf{C}$, và ta làm tường minh $\sigma_k(D)(x)$ được xem như một ánh xạ đa thức thuần nhất bậc $k$ từ $T_x(X)^*$ vào $\mathscr{L}(E_x; F_x)$ (xem 14.2.2). Cho $\omega \in T_x(X)^*$ và $v \in E_x$; chọn một hàm $f$ thuộc lớp $C^r$ trong một lân cận mở U của x sao cho $d_x f = \omega$, và một tiết diện s thuộc lớp $C^r$ của E trong U sao cho $s(x) = v$. Tồn tại một họ $(\varphi_0, \varphi_1, \ldots, \varphi_k)$ gồm các tiết diện của F trong U, và chỉ một họ như vậy, sao cho
$$
e^{-tf} D(e^{tf}s) = \sum_{j=0}^k t^j \varphi_j \quad \text{với mọi } t \in K.
$$
Khi đó $\varphi_k(x)$ không phụ thuộc vào lựa chọn của f và s sao cho $d_x f = \omega, v(x) = s$; ánh xạ $v \mapsto \varphi_k(x)$ là một phần tử $\lambda(\omega)$ của $\mathscr{L}(E_x; F_x)$, và $\lambda$ là một ánh xạ đa thức thuần nhất bậc k từ $T_x(X)^*$ vào $\mathscr{L}(E_x; F_x)$. *Ánh xạ này bằng ký hiệu $\sigma_k(D)(x)$ của D tại x.*

14.2.4 ("Trường hợp vô hướng"). Lấy $E = F = K_X$, trong trường hợp này ta đồng nhất $D^k(E, F)$ với bó $T^{(k)}(X)$ của các phân bố điểm cấp $\leq k$, xem 14.1.6. Ta có
$$
S^k(E, F) = TS^k(T(X))
$$
và ký hiệu
$$
\sigma_k : T^{(k)}(X) \to TS^k(T(X))
$$
không gì khác ngoài hợp thành
$$
T^{(k)}(X) \to T^{(k)}(X)/T^{(k-1)}(X) \xrightarrow{i_k} TS^k(T(X)),
$$
trong đó $i_k$ là đẳng cấu được xác định trong 13.3.2.

Lấy ví dụ X là một tập con mở của $K^n$, và cho $\{e_1, \ldots, e_n\}$ là cơ sở chính tắc của $K^n$ (đồng nhất với các không gian tiếp xúc $T_x(X)$). Nếu $\alpha \in \mathbf{N}^n$ sao cho $|\alpha| \leq k$, ký hiệu của toán tử $\Delta^\alpha$ được cho bởi các công thức (xem 13.3.3):
$$
\begin{aligned}
\sigma_k(\Delta^\alpha)(x) &= 0 & \text{nếu } |\alpha| < k \\
\sigma_k(\Delta^\alpha)(x) &= \gamma_{\alpha_1}(e_1) \cdots \gamma_{\alpha_n}(e_n) & \text{nếu } |\alpha| = k,
\end{aligned}
$$
tích của các $\gamma_{\alpha_i}(e_i)$ là *tích đối xứng*, xem 13.2.6 và 13.3.3.

14.2.5 ("Ký hiệu của một hợp thành"). Các ký hiệu và giả thiết là những ký hiệu và giả thiết của 14.1.8. Hợp thành của các ánh xạ tuyến tính xác định một phép ghép cặp
$$
\mathscr{L}(F; G) \times \mathscr{L}(E; F) \to \mathscr{L}(E; G).
$$
Mặt khác, phép toán *tích đối xứng* xác định một phép ghép cặp
$$
TS^{k''}(T(X)) \times TS^{k'}(T(X)) \to TS^k(T(X)).
$$
Vì ta có
$$
\begin{aligned}
S^{k''}(F, G) &= TS^{k''}(T(X)) \otimes \mathscr{L}(F; G) \\
S^{k'}(E, F) &= TS^{k'}(T(X)) \otimes \mathscr{L}(E; F) \\
S^k(E, G) &= TS^k(T(X)) \otimes \mathscr{L}(E; G)
\end{aligned}
$$
xem 14.2.2,
ta suy ra từ đó, bằng tích tenxơ, một phép ghép cặp
(*) $$
S^{k''}(F, G) \times S^{k'}(E, F) \to S^k(E, G).
$$
Khi đó ta có công thức
$$
\sigma_k(D'' \circ D') = \sigma_{k''}(D'') \cdot \sigma_{k'}(D'),
$$

trong đó tích xuất hiện ở vế phải được xác định bởi phép ghép cặp (*) ở trên.

Bây giờ giả sử K có đặc số không, và cho $x \in X$. Ký hiệu bởi $\sigma$ (tương ứng, $\sigma', \sigma''$) ký hiệu k (tương ứng, ký hiệu $k'$ , ký hiệu $k''$) của $D'' \circ D'$ (tương ứng, $D', D''$) tại $x$. Với mọi $\omega \in T_x(X)^*$, ta có (với các ký hiệu ở cuối 14.2.2):

$$
\tilde{\sigma}(\omega) \in \mathscr{L}(E_x; G_x), \quad \tilde{\sigma}'(\omega) \in \mathscr{L}(E_x; F_x), \quad \tilde{\sigma}''(\omega) \in \mathscr{L}(F_x; G_x)
$$

và

$$
\tilde{\sigma}(\omega) = \tilde{\sigma}''(\omega) \circ \tilde{\sigma}'(\omega).
$$

**14.3. Chuyển vị**

Trong No. này, giả sử rằng X thuần túy có chiều $n$.

### 14.3. Chuyển vị

14.3.1. Cho $\Omega = \det(T(X)^*)$, xem 7.9.9; đó là một bó vectơ hạng 1 tại mỗi điểm, với cơ sở X, và thuộc lớp $C^{r-1}$. Ta có

$$
\Omega = \wedge^n T(X)^* = \mathrm{Alt}^n(T(X); K_X).
$$

Cho M là một bó vectơ với cơ sở X. Đặt

$$
\tilde{M} = \mathscr{L}(M; \Omega) = M^* \otimes \Omega.
$$

[^1]

Nếu M thuộc lớp $C^n$, với $h \in N_K \cup \{0\}$ và $h \leq r - 1$, thì điều tương tự cũng đúng đối với $\tilde{M}$. Ánh xạ chính tắc của M vào $\tilde{M} = \mathscr{L}(\mathscr{L}(M; \Omega); \Omega)$ là một đẳng cấu; nó được dùng để đồng nhất M với $\tilde{M}$.

14.3.2 ("Định nghĩa về chuyển vị"). Cho $k$ là một số nguyên dương $\leq r - 1$, và cho D là một toán tử vi phân trên X, thuộc kiểu $E \to F$, có cấp $\leq k$, và thuộc lớp $C^n$, với $h \in N_K \cup \{0\}$ và $k \leq h \leq r - k$. Khi đó tồn tại một toán tử vi phân $^tD$ trên X, thuộc kiểu $\bar{F} \to \bar{E}$ và có cấp $\leq k$, có tính chất sau:

Cho $\xi = (\xi^1, \ldots, \xi^n)$ là một hệ tọa độ trong một tập mở U của X và cho $s = (s_i)_{1 \leq i \leq e}$ (tương ứng $t = (t_j)_{1 \leq j \leq f}$) là một khung của E (tương ứng của F) trên U. Cho $(s_i^*)$ (tương ứng $(t_j^*)$) là khung của $E^*$ (tương ứng của $F^*$) sao cho $\langle s_i, s_j^* \rangle = \delta_{ij}$ (tương ứng $\langle t_i, t_j^* \rangle = \delta_{ij}$), và cho $(\tilde{s}_i)$ (tương ứng $(\tilde{t}_j)$) là khung của $\bar{E}$ (tương ứng của $\bar{F}$) trên U thu được bằng cách lập tích tenxơ của $(s_i^*)$ (tương ứng của $(t_j^*)$) với khung $\omega = d\xi^1 \wedge \cdots \wedge d\xi^n$ của $\Omega$. Cho $c_{\alpha}^{ij}$ ($1 \leq i \leq e$, $1 \leq j \leq f$, $|\alpha| \leq k$) là các hàm thuộc lớp $C^n$ trên U sao cho có

$$
D \left( \sum_i f_i s_i \right) = \sum_{i,j,\alpha} c_{\alpha}^{ij} \Delta_{\xi}^{\alpha}(f_i) \cdot t_j
$$

với các hàm tùy ý $f_i$ trong $C^{h+k}(U)$, xem 14.1.4, (3'). Khi đó có

$$
{}^tD \left( \sum_j g_j \tilde{t}_j \right) = \sum_{i,j,\alpha} (-1)^{|\alpha|} \Delta_{\xi}^{\alpha}(c_{\alpha}^{ij} g_j) \tilde{s}_i
$$

với các hàm tùy ý $g_j$ trong $C^{h+k}(U)$.

80
CÁC ĐA TẠP VI PHÂN VÀ GIẢI TÍCH § 14

Tính chất trước đó (phải được kiểm tra với mọi $\xi$, $s$ và $t$ có thể có) xác định $^{t}D$ một cách duy nhất.[^2] Toán tử $^{t}D$ được gọi là chuyển vị của D; nó thuộc lớp $C^{h-k}$. Nếu $h\geq 2k$, chuyển vị của $^{t}D$ được xác định và bằng D (có tính đến các phép đồng nhất của $\widetilde{E}$ và $\widetilde{F}$ với E và F tương ứng).

Ánh xạ $D\mapsto{}^{t}D$ là $K$-tuyến tính. Nếu $k=0$, tức là nếu $D$ là một cấu xạ từ $E$ vào $F$, $^{t}D$ là cấu xạ $\mathscr{L}(D;\operatorname{Id}_{\Omega})$ từ $\widetilde{F}$ vào $\widetilde{E}$.

Ký hiệu của $^{t}D$ được suy ra từ ký hiệu của $D$ nhờ đẳng cấu

$$
\operatorname{TS}^{k}(T(X))\otimes\mathscr{L}(E;F)\longrightarrow \operatorname{TS}^{k}(T(X))\otimes\mathscr{L}(\widetilde{F};\widetilde{E})
$$

là tích tenxơ của tự đẳng cấu $(-1)^k$ của $\operatorname{TS}^{k}(T(X))$ và đẳng cấu $u\mapsto\mathscr{L}(u;\operatorname{Id}_{\Omega})$ của $\mathscr{L}(E;F)$ lên $\mathscr{L}(\widetilde{F};\widetilde{E})$.

### 14.3.3 (“Chuyển vị của một hợp”). Với ký hiệu và các giả thiết của 14.1.8, giả sử rằng $D'$ thuộc lớp $C^{h'}$ và $D''$ thuộc lớp $C^{h''}$, với $h',h''$ thuộc $\mathbf{N}_K\cup\{0\}$, $h'\geq k'+2k''$ và $h''\geq k''+2k'$.

Khi đó các chuyển vị của $D'$, $D''$ và $D''\circ D'$ được xác định, cũng như hợp của $^{t}D'$ và $^{t}D''$, và ta có

$$
^{t}(D''\circ D')={}^{t}D'\circ{}^{t}D''.
$$

Đặc biệt, với các giả thiết và ký hiệu của 14.3.2, và $f$ là một hàm thuộc lớp $C^{h'}$ trên $X$ với $2k\leq h'$, ta có $^{t}(D\circ f)=f\circ{}^{t}D$.

#### Ví dụ {#var-2-s14-n3-exa-1 .statement}

Cho $X$ là một tập con mở của $K^n$, cho $\xi^1,\ldots,\xi^n$ là các hàm tọa độ trên $X$, và đồng nhất $\Omega$ với $K_X$ bằng khung $\omega=d\xi^1\wedge\cdots\wedge d\xi^n$. Nếu $E=F=K_X$, ta có

$$
\widetilde{E}=\widetilde{F}=\mathscr{L}(K_X;\Omega)=\mathscr{L}(K_X;K_X)=K_X,
$$

và phép toán $D\mapsto{}^{t}D$ biến các toán tử vi phân vô hướng thành các toán tử vi phân vô hướng. Ta có, chẳng hạn,

$$
{}^{t}(\Delta^\alpha)=(-1)^{|\alpha|}\Delta^\alpha\qquad\text{với mọi }\alpha\in\mathbf{N}^n.
$$

Nếu $r$ là vô hạn, phép chuyển vị là một phản tự đẳng cấu của đại số $\mathscr{D}^{\infty}_{K_X}(K_X,K_X)$.

### 14.3.4. Cho $k$ là một số nguyên dương sao cho $K$ có đặc số $0$ hoặc $>k$. Cho $\Omega_1$ là bó vectơ $\bigwedge^{n-1}T(X)^*=\mathscr{L}(T(X);K_X)$. Ký hiệu và các giả thiết là những ký hiệu và giả thiết của 14.3.2, hơn nữa cho $D'$ là một toán tử vi phân trên $X$, từ $\widetilde{F}\rightarrow\widetilde{E}$, có cấp $\leq k$; một toán tử Green cho $(D,D')$ được định nghĩa là một toán tử đa vi phân bất kỳ $G$ (cf. 14.1.11) có kiểu $(E,\widetilde{F})\rightarrow\Omega_1$, có cấp $\leq k-1$[^3] và có lớp $C^h$ (với $h\geq1$), sao cho có đồng nhất thức

(1)

$$
\langle D(u),v\rangle-\langle u,D'(v)\rangle=d(G(u,v))
$$

đối với mọi tập mở $U$ của $X$ và mọi phần tử $u\in\mathscr{S}^k_E(U)$, $v\in\mathscr{S}^k_F(U)$. Ta hãy chỉ rõ rằng, trong công thức này, $d$ ký hiệu phép vi phân ngoài (8.3.5) và $\langle D(u),v\rangle$ (tương ứng.

$\langle u, D'(v) \rangle$) ký hiệu tiết diện của $\Omega$ trên $U$ nhận được từ cặp $(D(u), v)$ (tương ứng từ cặp $(u, D'(v))$) bởi phép ghép cặp chính tắc của $F \times \tilde{F}$ (tương ứng của $E \times \tilde{E}$) vào $\Omega$. Sự tồn tại của $G$ kéo theo $D' = {}^tD$; người ta cũng nói rằng $G$ là một toán tử Green cho $D$.

14.3.5. Cho $D$ là một toán tử vi phân trên $X$, có kiểu $E \to F$, có cấp $\leq k$, có lớp $C^h$ với $h \in N_K$ và $k \leq h \leq r - k$. Tồn tại một toán tử Green có lớp $C^{h-k+1}$ cho $D$ trong mỗi trường hợp sau đây:

a) $K = \mathbf{R}$, $r = \infty$ và $X$ là paracompact.
b) $K$ có đặc số $0$ hoặc $> k$, $X$ đẳng cấu với một tập mở của một không gian $K^n$, và các bó $E$ và $F$ đẳng cấu với các bó tầm thường.
c) Toán tử $D$ có cấp $\leq 1$ (cf. 14.3.7).

14.3.6. Các giả thiết và ký hiệu của 14.3.3 được giữ nguyên. Nếu $G'$ (tương ứng $G''$) là một toán tử Green đối với $D'$ (tương ứng $D''$), tồn tại duy nhất một toán tử Green $H$ đối với $D'' \circ D'$ sao cho có

$$
H(u, v) = G''(D'(u), v) + G'(u, {}^tD''(v))
$$

đối với mọi tập mở $U$ của $X$ và các phần tử $u \in \mathscr{S}_E^k(U)$ và $v \in \mathscr{S}_{\tilde{G}}^k(U)$.

14.3.7. Ta có $S^1(E, F) = T(X) \otimes E^* \otimes F$ (xem 14.2.2). Mặt khác, tích trong phải $(\xi, \omega) \mapsto i(\xi)\omega$ (xem A, III, p. 158) xác định một đẳng cấu từ $T(X) \otimes \Omega$ lên $\Omega_1$; bằng tích tenxơ với đối ngẫu $\Omega^*$ của $\Omega$, do đó ta thu được một đẳng cấu từ $T(X)$ lên $\Omega^* \otimes \Omega_1$, do đó có các đồng nhất thức của các bó vectơ

$$
\begin{align*}
S^1(E, F) &= \Omega^* \otimes \Omega_1 \otimes E^* \otimes F = (E \otimes F^* \otimes \Omega)^* \otimes \Omega_1 \\
&= (E \otimes \tilde{F})^* \otimes \Omega_1 = \mathscr{L}(E \otimes \tilde{F}; \Omega_1).
\end{align*}
$$

Với điều này đã được thiết lập, cho $D$ là một toán tử vi phân trên $X$, kiểu $E \to F$, cấp $\leq 1$, thuộc lớp $C^h$ với $h \in N_K \cup \{0\}$ và $h \leq r - 1$. Tồn tại duy nhất một toán tử Green đối với $D$; nó có cấp $0$; nó là một cấu xạ thuộc lớp $C^h$ từ $E \otimes \tilde{F}$ vào $\Omega_1$, và nó được suy ra từ ký hiệu của $D$ bởi đồng nhất thức trước đó.

14.3.8. Giả sử $K = \mathbf{R}$, $X$ là tách và định hướng (10.2.4), và cho $A$ là một phần đóng (11.1.2) của $X$. Trang bị cho $A$ định hướng cảm sinh bởi định hướng của $X$, và cho $\partial A$ định hướng tương ứng (11.2.1). Cho $k$ là một số nguyên sao cho $2k \leq r$, $D$ là một toán tử vi phân trên $X$, kiểu $E \to F$, cấp $\leq k$ và thuộc lớp $C^k$. Cho $G$ là một toán tử Green đối với $D$. Cho $U$ là một tập mở của $X$, $u \in \mathscr{S}_E^k(U)$, $v \in \mathscr{S}_{\tilde{F}}^k(U)$ và giả sử rằng giá của $u$ và $v$ gặp $A$ trong một tập compact. Khi đó có

$$
\int_A \langle D(u), v \rangle - \int_A \langle u, {}^tD(v) \rangle = \int_{\partial A} G(u, v)
$$

(*công thức Green*). Đặc biệt, nếu $\partial A = \varnothing$, ta có

$$
\int_A \langle D(u), v \rangle = \int_A \langle u, {}^tD(v) \rangle.
$$

### 14.4. Ví dụ

Giả sử X thuần túy có số chiều hữu hạn n. Giả sử nó cũng được trang bị một cấu trúc đa tạp thuộc lớp C^{r+1} tương thích với cấu trúc đã cho thuộc lớp C^r.

14.4.1 (« Các phép biến đổi vô cùng bé »). Cho $\tau$ là một hàm tử vectơ trong chiều hữu hạn đối với các đẳng cấu, thuộc lớp C^r; giả sử rằng, đối với mọi không gian vectơ hữu hạn chiều V, $\tau(V)$ là hữu hạn chiều. Ta ký hiệu $E_{\tau}$ là bó vectơ $\tau(T(X))$; nó thuộc lớp C^r.

Cho $\xi$ là một trường vectơ thuộc lớp C^r trên X. Tồn tại một toán tử vi phân D kiểu $E_{\tau} \to E_{\tau}$ và cấp $\leq 1$ sao cho

$$
D_U(s) = \theta_{\xi}.s
$$

với mọi tập mở U của X và mọi $s \in \mathscr{S}_{E_{\tau}}(U)$, xem 8.4.3. Một toán tử vi phân D như vậy là duy nhất; ta ký hiệu nó bởi $(\theta_{\xi})_{\tau}$ hoặc đơn giản là $\theta_{\xi}$. Ký hiệu của nó là tiết diện $\xi \otimes \mathrm{Id}_{E_{\tau}}$ của bó vectơ

$$
S^1(E_{\tau}, E_{\tau}) = T(X) \otimes \mathscr{L}(E_{\tau}; E_{\tau}).
$$

Nếu V là một không gian vectơ trên K hữu hạn chiều, đặt

$$
\tilde{\tau}(V) = \mathscr{L}(\tau(V); \mathrm{Alt}^n(V; K)) = \tau(V)^* \otimes \wedge^n V^*,
$$

và nếu $u : V_1 \to V_2$ là một đẳng cấu, định nghĩa $\tilde{\tau}(u) : \tilde{\tau}(V_1) \to \tilde{\tau}(V_2)$ bằng phép chuyển cấu trúc. Do đó ta thu được một hàm tử vectơ trong chiều hữu hạn $\tilde{\tau}$. Bó $E_{\tilde{\tau}} = \tilde{\tau}(T(X))$ đồng nhất theo cách hiển nhiên với bó $(E_{\tau})^*$; chuyển vị của $(\theta_{\xi})_{\tau}$ là $-(\theta_{\xi})_{\tilde{\tau}}$ và công thức (1) của no. 14.3.4 có dạng

$$
\langle \theta_{\xi}.u, v \rangle + \langle u, \theta_{\xi}.v \rangle = d(i(\xi)(u.v)).
$$

14.4.2 (« Vi phân ngoài »). Với mọi số nguyên $p \geq 0$ đặt

$$
\Omega^p = \mathrm{Alt}^p(T(X); K_X).
$$

Tồn tại một toán tử vi phân D kiểu $\Omega^p \to \Omega^{p+1}$ và cấp $\leq 1$ sao cho

$$
D_U(\omega) = d\omega
$$

với mọi tập mở U của X và mọi $\omega \in \mathscr{S}_{\Omega^p}(U)$. Một toán tử vi phân D như vậy là duy nhất; ta ký hiệu nó bởi d (hoặc $d_p$ nếu muốn chỉ rõ số nguyên p).

Ký hiệu của nó là phần tử của $S^1(\Omega^p, \Omega^{p+1})$ được thu được như sau: trước hết ta có

$$
S^1(\Omega^p, \Omega^{p+1}) = T(X) \otimes \mathscr{L}(\Omega^p; \Omega^{p+1})
$$
$$
= \mathscr{L}(\Omega^1; \mathscr{L}(\Omega^p; \Omega^{p+1})) = \mathscr{L}(\Omega^1, \Omega^p; \Omega^{p+1}),
$$

trong đó $\mathscr{L}(\Omega^1, \Omega^p; \Omega^{p+1})$ chỉ bó các ánh xạ song tuyến tính từ $\Omega^1 \times \Omega^p$ vào $\Omega^{p+1}$. Khi đó tích ngoài $(\alpha, \beta) \mapsto \alpha \wedge \beta$ định nghĩa một tiết diện chính tắc của bó sau cùng này; tiết diện này là ký hiệu của $d_p$.

Để xác định chuyển vị của $d_p$, trước hết ta nhận xét rằng tích ngoài định nghĩa một ghép cặp $\Omega^p \times \Omega^{n-p} \to \Omega^n = \Omega$ cho phép đồng nhất $(\Omega^p)^*$ với $\Omega^{n-p}$. Ta đồng nhất $(\Omega^{p+1})^*$ với $\Omega^{n-p-1}$ theo cùng cách đó. Với các quy ước này, chuyển vị của $d_p$ là $(-1)^{p+1} d_{n-p-1}$ và toán tử Green tương ứng, kiểu

$(\Omega^p,\Omega^{n-p-1})\longrightarrow\Omega_1=\Omega^{n-1}$, đơn giản là tích ngoài (trên mỗi thớ).

### 14.4.3 (« Toán tử Laplace »).

Cho $K=\mathbf{R}$, $r=\infty$, $X=\mathbf{R}^n$, $E=F=K_X$; gọi $\xi^i$ $(1\leq i\leq n)$ là các hàm tọa độ trên $X$; đặt $D_i=\partial/\partial\xi^i$, và $L=\sum_{i=1}^n D_i^2$. Toán tử $L$ là một toán tử vi phân vô hướng có cấp $\leq 2$. Nếu ta đồng nhất $\Omega$ với $K_X$ nhờ vào khung $\omega=d\xi^1\wedge\cdots\wedge d\xi^n$, ta có $\tilde E=\tilde F=K_X$ (xem 14.3.3, ví dụ) và $\tilde L=L$.

Với $1\leq i\leq n$, đặt $\omega_i=(-1)^{i-1}d\xi^1\wedge\cdots\wedge d\xi^{i-1}\wedge d\xi^{i+1}\wedge\cdots\wedge d\xi^n$. Các $\omega_i$ lập thành một khung của $\Omega_1=\Omega^{n-1}$. Nếu $f\in\mathscr C^1(X)$, gọi $\operatorname{grad}(f)$ là tiết diện $\sum_{i=1}^n D_i(f)\omega_i$ của $\Omega_1$. Tồn tại một toán tử Green $G$ cho $L$ sao cho

$$G(u,v)=v.\operatorname{grad}(u)-u.\operatorname{grad}(v)$$

với mọi tập mở $U$ của $X$ và $u,v$ trong $\mathscr C^1(U)$.

Đặc biệt, xét $A$ là một mảnh compact của $\mathbf{R}^n$. Định hướng $\mathbf{R}^n$, trang bị cho $A$ định hướng cảm sinh bởi định hướng đó của $\mathbf{R}^n$, và cho $\partial A$ định hướng tương ứng (11.2.1). Ta có

$$\int_A(Lu).v\omega-\int_Au.(Lv)\omega=\int_{\partial A}(v.\operatorname{grad}(u)-u.\operatorname{grad}(v))$$

với $u,v$ trong $\mathscr C^1(X)$.

[^1]: Cần chú ý không nhầm $\tilde{M}$ với phủ của M được định nghĩa trong 10.2.4 và được ký hiệu cùng cách như vậy.
[^2]: Thực ra, chỉ cần kiểm tra tính chất đang xét đối với các bộ ba $(\xi^\lambda,s^\lambda,t^\lambda)$ sao cho các miền của các $\xi^\lambda$ phủ $X$.
[^3]: Khi $k=0$, quy ước rằng điều này có nghĩa là $G=0$.
