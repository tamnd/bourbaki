---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 1
section_title: Enveloping bigebra of a Lie algebra
lang: vi
source: lie-i-iii
pdf_pages: 0129-0140, 0196-0199
extraction: ocr
subsections:
    - "no": 1
      title: PRIMITIVE ELEMENTS OF A COGEBRA
      page: 0
      pdf_page: 129
    - "no": 2
      title: PRIMITIVE ELEMENTS OF A BIGEBRA
      page: 0
      pdf_page: 131
    - "no": 3
      title: FILTERED BIGEBRAS
      page: 0
      pdf_page: 132
    - "no": 4
      title: ENVELOPING BIGEBRA OF A LIE ALGEBRA
      page: 0
      pdf_page: 133
    - "no": 5
      title: STRUCTURE OF THE COGEBRA U(g) IN CHARACTERISTIC 0
      page: 0
      pdf_page: 134
    - "no": 6
      title: STRUCTURE OF FILTERED BIGEBRAS IN CHARACTERISTIC 0
      page: 0
      pdf_page: 137
statements: 24
exercises: 12
content_sha256: b7a53c79d9d37063fe0048878aa5803b134bd4f3e97bb151e4ce7f83d686ce51
translated_from: content/en/lie/II/01_s1_enveloping_bigebra_of_a_lie_algebra.md
source_content_sha256: 2809a9ef30dc6d5e712bfdcb8c630966d7bcdf41020c5af1ebbaf978ef021eac
translation_model: gpt-5.4
translation_run: translate-vi-696e9754
glossary_version: 34
glossary_terms_sha256: 2cd6ae3d250514a68a3a089a43d2d3b4772a311d3e3b2902368832cbfc9303dd
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐỐI ĐẠI SỐ BAO CỦA MỘT ĐẠI SỐ LIE

Trong suốt tiết này, g sẽ chỉ một đại số Lie trên K, U(g) hoặc đơn giản U đại số bao của nó (Chương I, § 2, no. 1), σ ánh xạ chính tắc của g vào U(g) (sđd.) và (U_n)_{n \geq 0} phép lọc chính tắc của U (sđd., no. 6).

### 1. CÁC PHẦN TỬ NGUYÊN THỦY CỦA MỘT ĐỐI ĐẠI SỐ

Trong suốt số này, ta xét một đối đại số E (Đại số, Chương III, § 11, no. 1) với đồng tích
$$
c : E \to E \otimes E
$$
và đồng đơn vị ε (sđd., no. 2). Nhắc lại rằng ε là một dạng tuyến tính trên K-môđun E sao cho (với sự đồng nhất chính tắc của E \otimes K và K \otimes E với E):
$$
\mathrm{Id}_E = (\varepsilon \otimes \mathrm{Id}_E) \circ c = (\mathrm{Id}_E \otimes \varepsilon) \circ c.
$$
Ký hiệu E^+ là hạt nhân của ε và lấy u là một phần tử của E sao cho
$$
c(u) = u \otimes u \quad \text{và} \quad \varepsilon(u) = 1.
$$

† Các kết quả của các Chương II và III phụ thuộc vào sáu quyển đầu, vào Nhóm Lie và đại số Lie, Chương I, vào Đại số giao hoán và vào Đa tạp khả vi và giải tích, Tóm tắt các kết quả; no. 9 của § 6 của Chương III còn phụ thuộc vào Các lý thuyết phổ, Chương I.

K-môđun E là tổng trực tiếp của $ E^+ $ và của môđun con $ K.u $ tự do với cơ sở $ u $; ký hiệu $ \pi_u : E \to E^+ $ và $ \eta_u : E \to K.u $ là các phép chiếu liên kết với sự phân tích này. Khi đó

(1)
$$
\pi_u(x) = x - \varepsilon(x).u, \qquad \eta_u(x) = \varepsilon(x).u.
$$

#### Định nghĩa 1 {#lie-ii-s1-def-1 .statement}

*Một phần tử $ x $ của $ E $ được gọi là u-nguyên thủy nếu*

(2)
$$
c(x) = x \otimes u + u \otimes x.
$$

Các phần tử $ u $-nguyên thủy của $ E $ tạo thành một môđun con của $ E $, ký hiệu là $ P_u(E) $.

#### Mệnh đề 1 {#lie-ii-s1-prop-1 .statement}

*Mọi phần tử u-nguyên thủy của $ E $ đều thuộc $ E^+ $.*
(2) kéo theo $ x = \varepsilon(x).u + \varepsilon(u).x = \varepsilon(x).u + x, $ do đó $ \varepsilon(x) = 0 $.

#### Nhận xét {#lie-ii-s1-n1-rem-1 .statement}

Nếu $ x \in E $ và $ c(x) = x' \otimes u + u \otimes x'' $, trong đó $ x', x'' $ thuộc $ E^+ $, thì $ x = \varepsilon(x').u + \varepsilon(u).x'' = x'' $; tương tự, $ x = x' $ và $ x $ là $ u $-nguyên thủy.

Với mọi $ x \in E^+ $, ta viết

(3)
$$
c_u^+(x) = c(x) - x \otimes u - u \otimes x.
$$

#### Mệnh đề 2 {#lie-ii-s1-prop-2 .statement}

*Ta có*

(4)
$$
(\pi_u \otimes \pi_u) \circ c = c_u^+ \circ \pi_u.
$$

Cho $ x $ thuộc $ E $; khi đó
$$
\begin{align*}
(\pi_u \circ \pi_u)(c(x)) &= ((1 - \eta_u) \otimes (1 - \eta_u))(c(x)) \\
&= c(x) - (1 \otimes \eta_u)(c(x)) - (\eta_u \otimes 1)(c(x)) + (\eta_u \otimes \eta_u)(c(x)).
\end{align*}
$$
Vì $ \varepsilon $ là đồng đơn vị của $ E $,
$$
(1 \otimes \eta_u)(c(x)) = x \otimes u, \qquad (\eta_u \otimes 1)(c(x)) = u \otimes x
$$
do đó
$$
(\eta_u \otimes \eta_u)(c(x)) = (\eta_u \otimes 1)((1 \otimes \eta_u)(c(x))) = \varepsilon(x).u \otimes u;
$$
từ đó ta kết luận
$$
(\pi_u \otimes \pi_u)(c(x)) = c(x) - x \otimes u - u \otimes x + \varepsilon(x).u \otimes u.
$$
Mặt khác,
$$
c_u^+(\pi_u(x)) = c(x) - x \otimes u - u \otimes x + \varepsilon(x).u \otimes u,
$$
do đó công thức (4).

Vì $ E^+ $ là một môđun con hạng tử trực tiếp của $ E $, nên $ E^+ \otimes E^+ $ có thể được đồng nhất với một môđun con hạng tử trực tiếp của $ E \otimes E $. Với sự đồng nhất này, $ \pi_u \otimes \pi_u $ là một phép chiếu của $ E \otimes E $ lên $ E^+ \otimes E^+ $. Theo công thức (4), $ c_u^+ $ ánh xạ $ E^+ $ vào $ E^+ \otimes E^+ $ và $ \pi_u $ là một cấu xạ từ đối đại số $ (E, c) $ vào đối đại số $ (E^+, c_u^+) $.

#### Mệnh đề 3 {#lie-ii-s1-prop-3 .statement}

*Nếu đối đại số* $(E, c)$ *là đối kết hợp* (resp. đối giao hoán) (*Đại số*, Chương III, § 11, no. 2), *thì đối đại số* $(E^+, c_u^+)$ *cũng vậy*.

Điều này suy ra từ bổ đề sau đây:

#### Bổ đề 1 {#lie-ii-s1-lem-1 .statement}

*Cho* $\pi : E \to E'$ *là một cấu xạ cogebras toàn ánh. Nếu* $E$ *là đối kết hợp* (resp. đối giao hoán), *thì* $E'$ *cũng vậy*.

Cho $B$ là một $K$-đại số kết hợp; ánh xạ $f \mapsto f \circ \pi$ là một đồng cấu đại số *đơn ánh* từ $\mathrm{Hom}_K(E', B)$ vào $\mathrm{Hom}_K(E, B)$. Khi đó chỉ cần áp dụng Mệnh đề 1 (resp. Mệnh đề 2) của *Đại số*, Chương III, § 11, no. 2.

### 2. CÁC PHẦN TỬ NGUYÊN THỦY CỦA MỘT SONG ĐẠI SỐ

Cho $E$ là một *song đại số* (*Đại số*, chương III, § 11, no. 4), $c$ là đồng tích của nó, $\varepsilon$ là đồng đơn vị của nó và $1$ là phần tử đơn vị của nó. Vì $\varepsilon(1) = 1$ và $c(1) = 1 \otimes 1$, các kết quả của số trước có thể được áp dụng với $u = 1$. Các phần tử 1-nguyên thủy của $E$ (no. 1, Định nghĩa 1) được gọi đơn giản là *nguyên thủy* (xem *Đại số*, chương III; § 11, no. 8), tức là các phần tử $x$ của $E$ sao cho

$$
c(x) = x \otimes 1 + 1 \otimes x.
$$

Ta viết đơn giản $\pi$, $\eta$, $P(E)$, $c^+$ thay cho $\pi_1$, $\eta_1$, $P_1(E)$, $c_1^+$.

#### Mệnh đề 4 {#lie-ii-s1-prop-4 .statement}

*Tập hợp* $P(E)$ *các phần tử nguyên thủy của* $E$ *là một đại số con Lie của* $E$.

Nếu $x, y$ thuộc $P(E)$, thì
$$
\begin{align*}
c(xy) &= c(x)c(y) = (x \otimes 1 + 1 \otimes x)(y \otimes 1 + 1 \otimes y) \\
&= xy \otimes 1 + 1 \otimes xy + x \otimes y + y \otimes x,
\end{align*}
$$
do đó
$$
c([x, y]) = [x, y] \otimes 1 + 1 \otimes [x, y].
$$

#### Mệnh đề 5 {#lie-ii-s1-prop-5 .statement}

*Cho* $f : E \to E'$ *là một cấu xạ của bigèbre. Nếu* $x$ *là một phần tử nguyên thủy của* $E$, *thì* $f(x)$ *là một phần tử nguyên thủy của* $E'$ *và hạn chế của* $f$ *trên* $P(E)$ *là một đồng cấu đại số Lie* $P(f) : P(E) \to P(E')$.

Cho $c$ (resp. $c'$) là đồng tích của $E$ (resp. $E'$). Vì $f$ là một cấu xạ cogebras nên $c' \circ f = (f \otimes f) \circ c$, do đó
$$
\begin{align*}
c'(f(x)) &= (f \otimes f)(c(x)) = (f \otimes f)(x \otimes 1 + 1 \otimes x) \\
&= f(x) \otimes 1 + 1 \otimes f(x),
\end{align*}
$$
với $x$ nguyên thủy. Vậy $f$ ánh xạ $P(E)$ vào $P(E')$ và $f([x, y]) = [f(x), f(y)]$ vì $f$ là một đồng cấu đại số.

#### Nhận xét {#lie-ii-s1-n2-rem-1 .statement}

(1) Cho $p$ là một số nguyên tố sao cho $p \cdot 1 = 0$ trong $K$. Công thức nhị thức và các đồng dư thức $\binom{p}{i} \equiv 0 \pmod{p}$ với $1 \leq i \leq p - 1$ kéo theo rằng

P(E) ổn định đối với ánh xạ $ x \mapsto x^p $.

(2) Theo định nghĩa, biểu đồ

$$
0 \longrightarrow P(E) \longrightarrow E^+ \xrightarrow{c^+} E^+ \otimes E^+
$$

là một dãy khớp. Nếu $ K' $ là một vành giao hoán và $ \rho : K \to K' $ là một đồng cấu vành, thì $ \rho^*(E) = E \otimes_K K' $ là một $ K' $-song đại số và phép bao hàm $ P(E) \to E $ xác định một đồng cấu các $ K' $-đại số Lie

$$
\alpha : P(E) \otimes_K K' \to P(E \otimes_K K').
$$

Nếu $ K' $ phẳng trên $ K $ (Đại số giao hoán, Chương I, § 2, no. 3, Định nghĩa 2), thì suy ra từ loc. cit. rằng biểu đồ

$$
0 \longrightarrow P(E) \otimes_K K' \longrightarrow E^+ \otimes_K K' \xrightarrow{c^+ \otimes_K \mathrm{Id}_{K'}} (E^+ \otimes_K K') \otimes_{K'} (E^+ \otimes_K K')
$$

là một dãy khớp, điều này kéo theo rằng $ \alpha $ là một đẳng cấu.

### 3. SONG ĐẠI SỐ LỌC

#### Định nghĩa 2 {#lie-ii-s1-def-2 .statement}

Cho $ E $ là một song đại số có đồng tích $ c $. Một bộ lọc tương thích với cấu trúc song đại số trên $ E $ là một dãy tăng $ (E_n)_{n \geq 0} $ các môđun con của $ E $ sao cho

$$
\begin{align*}
E_0 &= K.1, \quad E = \bigcup_{n \geq 0} E_n \\
E_m \cdot E_n &\subset E_{m+n} \quad \text{với } m \geq 0, n \geq 0 \\
c(E_n) &\subset \sum_{i+j=n} \operatorname{Im}(E_i \otimes E_j) \quad \text{với } n \geq 0.\dagger
\end{align*}
$$

Một song đại số có một bộ lọc tương thích với cấu trúc song đại số của nó được gọi là một song đại số lọc.

#### Ví dụ {#lie-ii-s1-n3-exa-1 .statement}

Cho $ E $ là một song đại số phân bậc (Đại số, Chương III, § 11, no. 4, Định nghĩa 3) và $ (E^n)_{n \geq 0} $ là phân bậc của nó. Ta đặt $ E_n = \sum_{i=0}^n E^i $. Dãy $ (E_n) $ là một bộ lọc tương thích với cấu trúc song đại số trên $ E $.

#### Mệnh đề 6 {#lie-ii-s1-prop-6 .statement}

Cho $ E $ là một song đại số được lọc và $ (E_n)_{n \geq 0} $ là bộ lọc của nó. Với mọi số nguyên $ n \geq 0 $, đặt $ E_n^+ = E_n \cap E^+ $. Khi đó $ E_0^+ = \{0\} $ và

$$
c^+(E_n^+) \subset \sum_{i=1}^{n-1} \operatorname{Im}(E_i^+ \otimes E_{n-1}^+) \quad \text{với } n \geq 0.\dagger
$$

Vì $ E_0 = K.1, E_0^+ = 0 $. Nếu $ x \in E_n, \pi(x) = x - \varepsilon(x).1 $ (công thức (1)), do đó $ \pi(x) \in E_n^+ $ và $ \pi(E_n) \subset E_n^+ $. Suy ra $ \pi \otimes \pi $ ánh xạ $ \operatorname{Im}(E_i \otimes E_j) $ vào

\dagger Nếu A và B là hai môđun con của E, ta ký hiệu bởi $ \operatorname{Im}(A \otimes B) $ ảnh của ánh xạ chính tắc $ A \otimes B \to E \otimes E $.

Im(E_i^+ \otimes E_j^+) \text{ với } i \geq 0, j \geq 0. \text{ Vì } c^+ = (\pi \otimes \pi) \circ c \text{ trong } E^+ \text{ (no. 1, Mệnh đề 2), theo (6)}

$$
c^+(E_n^+) \subset \sum_{i=0}^n \operatorname{Im}(E_i^+ \otimes E_{n-i}^+) = \sum_{i=1}^{n-1} \operatorname{Im}(E_i^+ \otimes E_{n-i}^+).
$$

#### Hệ quả {#lie-ii-s1-n3-cor-1 .statement}

*Các phần tử của* $ E_1^+ $ *là nguyên thủy.*
Nếu $ x \in E_1^+ $, thì $ c^+(x) = 0 $ theo (7), do đó có (5).

### 4. ĐẠI SỐ KÉP BAO BỌC CỦA MỘT ĐẠI SỐ LIE

Nhắc lại rằng $ g $ ký hiệu một đại số Lie và $ U $ ký hiệu đại số bao bọc của nó, với lọc chính tắc $ (U_n)_{n \geq 0} $.

#### Mệnh đề 7 {#lie-ii-s1-prop-7 .statement}

*Trên đại số* $ U $ *tồn tại duy nhất một đồng tích* $ c $ *biến* $ U $ *thành một song đại số sao cho các phần tử của* $ \sigma(g) $ *là nguyên thủy. Song đại số* $ (U, c) $ *là đối giao hoán; đồng đơn vị của nó là dạng tuyến tính* $ \varepsilon $ *sao cho số hạng hằng (Chương I, § 2, no. 1) của mọi phần tử* $ x $ *của* $ U $ *là* $ \varepsilon(x) . 1 $. *Lọc chính tắc* $ (U_n)_{n \geq 0} $ *của* $ U $ *tương thích với cấu trúc song đại số này.*

(a) Cho $ x \in g $; ta viết $ c_0(x) = \sigma(x) \otimes 1 + 1 \otimes \sigma(x) \in U \otimes U $. Nếu $ x, y $ thuộc $ g $, thì
$$
c_0(x)c_0(y) = (\sigma(x)\sigma(y)) \otimes 1 + 1 \otimes (\sigma(x)\sigma(y)) + \sigma(x) \otimes \sigma(y) + \sigma(y) \otimes \sigma(x),
$$
do đó
$$
[c_0(x), c_0(y)] = c_0([x, y]).
$$
Theo tính chất phổ quát của $ U $ (Chương I, § 2, no. 1, Mệnh đề 1), tồn tại một và chỉ một đồng cấu đại số có đơn vị
$$
c : U \to U \otimes U
$$
sao cho $ c(\sigma(x)) = \sigma(x) \otimes 1 + 1 \otimes \sigma(x) $ với $ x \in g $. Điều này chứng minh mệnh đề về tính duy nhất của Mệnh đề 7.

(b) *Ta chứng minh rằng* $ c $ *là đối kết hợp.* Các ánh xạ tuyến tính $ c' $ và $ c'' $ từ $ U $ vào $ U \otimes U \otimes U $ được xác định bởi
$$
c' = (c \otimes \mathrm{Id}_U) \circ c \quad \text{và} \quad c'' = (\mathrm{Id}_U \otimes c) \circ c
$$
là các đồng cấu đại số có đơn vị trùng nhau trên $ \sigma(g) $ vì, với $ a \in \sigma(g) $,
$$
c'(a) = a \otimes 1 \otimes 1 + 1 \otimes a \otimes 1 + 1 \otimes 1 \otimes a = c''(a),
$$
do đó suy ra kết quả.

(c) *Ta chỉ ra rằng* $ c $ *là đối giao hoán.* Cho $ \tau $ là tự đẳng cấu của $ U \otimes U $ sao cho $ \tau(a \otimes b) = b \otimes a $ với $ a, b $ trong $ U $. Các ánh xạ $ \tau \circ c $ và $ c $ từ $ U $ vào $ U \otimes U $ là các đồng cấu đại số có đơn vị và trùng nhau trên $ \sigma(g) $, do đó suy ra kết quả.

(d) *Ta chỉ ra rằng* $ \varepsilon $ *là một đồng đơn vị đối với* $ c $. Các ánh xạ $ (\mathrm{Id}_U \otimes \varepsilon) \circ c $ và (ε ⊗ Id_U) ∘ c, từ U vào U là các đồng cấu đại số có đơn vị và trùng với Id_U trên σ(g).

(e) Ta biết rằng U_0 = K . 1, U_n ⊂ U_{n+1}, U = ⋃_{n ≥ 0} U_n và U_n · U_m ⊂ U_{n+m} (chương I, § 2, no. 6). Cho a_1, ..., a_n thuộc σ(g). Khi đó

$$
c(a_1 ... a_n) = \prod_{i=1}^n c(a_i) = \prod_{i=1}^n (a_i ⊗ 1 + 1 ⊗ a_i)
$$
$$
= \sum_{i=0}^n \sum_{α ∈ I(i)} (a_{α(1)} ... a_{α(i)}) ⊗ (a_{α(i+1)} ... a_{α(n)}),
$$

trong đó I(i) ký hiệu tập hợp các hoán vị của {1, n} tăng trên mỗi khoảng {1, i} và {i + 1, n}. Vì U_n là K-môđun được sinh bởi các tích của nhiều nhất n phần tử của σ(g), công thức (8) suy ra rằng bộ lọc (U_n) là tương thích với cấu trúc song đại số của (U, c).

#### Định nghĩa 3 {#lie-ii-s1-def-3 .statement}

*Song đại số* (U, c) *được gọi là* song đại số bao *của đại số Lie* g.

#### Mệnh đề 8 {#lie-ii-s1-prop-8 .statement}

*Cho E là một song đại số với đồng tích ký hiệu bởi c_E và h là một đồng cấu đại số Lie của g vào P(E)* (no. 2, Mệnh đề 4). *Đồng cấu đại số có đơn vị f : U → E sao cho f(σ(x)) = h(x) với mọi x ∈ g là một cấu xạ song đại số.*

Ta chứng minh rằng (f ⊗ f) ∘ c = c_E ∘ f. Đây là hai đồng cấu đại số có đơn vị từ U vào E ⊗ E và, với a ∈ σ(g),

$$(f ⊗ f)(c(a)) = f(a) ⊗ 1 + 1 ⊗ f(a) = c_E(f(a))$$

vì f(a) ∈ P(E). Tương tự, nếu ε_E là đồng đơn vị của E thì ε_E ∘ f là một đồng cấu đại số có đơn vị U → K triệt tiêu trên σ(g) (no. 1, Mệnh đề 1) và do đó trùng với ε.

Từ các Mệnh đề 5 và 8 suy ra rằng ánh xạ f ↦ f ∘ σ xác định một sự tương ứng một-một giữa các đồng cấu song đại số U(g) → E và các đồng cấu đại số Lie g → P(E).

#### Hệ quả {#lie-ii-s1-n4-cor-1 .statement}

*Cho g_i (i = 1, 2) là một đại số Lie, U(g_i) là song đại số bao của nó và σ_i : g_i → U(g_i) là ánh xạ chính tắc. Với mọi đồng cấu đại số Lie h : g_1 → g_2, đồng cấu đại số có đơn vị U(h) : U(g_1) → U(g_2) sao cho U(h) ∘ σ_1 = σ_2 ∘ h (Chương I, § 2, no. 1) là một cấu xạ song đại số.*

### 5. CẤU TRÚC CỦA ĐỐI ĐẠI SỐ U(g) TRONG ĐẶC SỐ 0

Trong số này, K được giả thiết là một trường đặc số 0.

Gọi S(g) là đại số đối xứng của không gian vectơ g, c_S là đồng tích của nó (Đại số, Chương III, § 11, no. 1, Ví dụ 6) và η là đẳng cấu chính tắc của không gian vectơ $ S(\mathfrak{g}) $ lên không gian vectơ $ U $ (Chương I, § 2, no. 7). Nhắc lại rằng nếu $ x_1, \ldots, x_n $ thuộc $ \mathfrak{g} $, thì

$$
\eta(x_1 \ldots x_n) = \frac{1}{n!} \sum_{\tau \in \mathfrak{S}_n} \sigma(x_{\tau(1)}) \ldots \sigma(x_{\tau(n)}).
$$

Đặc biệt, với $ x \in \mathfrak{g} $ và $ n \geq 0 $,

$$
\eta(x^n) = \sigma(x)^n.
$$

Chú ý rằng theo *Đại số*, Chương III, § 6, no. 1, *Nhận xét 3*, $ \eta $ là ánh xạ tuyến tính duy nhất từ $ S(\mathfrak{g}) $ vào $ U $ thỏa mãn điều kiện (10).

#### Mệnh đề 9 {#lie-ii-s1-prop-9 .statement}

*Với mọi số nguyên $ n \geq 0 $, đặt $ U^n $ là không gian con vectơ của $ U $ sinh bởi các $ \sigma(x)^n $ với $ x \in \mathfrak{g} $.*

(a) *Dãy $ (U^n)_{n \geq 0} $ là một phân bậc của không gian vectơ $ U $ tương thích với cấu trúc đối đại số của nó.*

*Đặt trên $ U $ phân bậc $ (U^n) $.*

(b) *Ánh xạ chính tắc $ \eta : S(\mathfrak{g}) \to U $ là một đẳng cấu của các đối đại số phân bậc.*

Cho $ x \in \mathfrak{g} $ và $ n \in \mathbf{N} $. Khi đó

$$
c_S(x^n) = c_S(x)^n = (x \otimes 1 + 1 \otimes x)^n = \sum_{i=0}^n \binom{n}{i} x^i \otimes x^{n-i}
$$

vì $ c_S $ là một đồng cấu đại số. Tương tự, theo (10),

$$
c(\eta(x^n)) = c(\sigma(x)^n) = c(\sigma(x))^n = (\sigma(x) \otimes 1 + 1 \otimes \sigma(x))^n
$$
$$
= \sum_{i=0}^n \binom{n}{i} \sigma(x)^i \otimes \sigma(x)^{n-i} = \sum_{i=0}^n \binom{n}{i} \eta(x^i) \otimes \eta(x^{n-i}),
$$

do đó

$$
(\eta \otimes \eta)(c_S(x^n)) = c(\eta(x^n)).
$$

Vì các $ x^n $, với $ x \in \mathfrak{g} $ và $ n \in \mathbf{N} $, sinh không gian vectơ $ S(\mathfrak{g}) $, nên $ (\eta \otimes \eta) \circ c_S = c \circ \eta $ và $ \eta $ là một đẳng cấu đối đại số.

Mặt khác, công thức (10) cho thấy rằng $ \eta(S^n(\mathfrak{g})) = U^n $, điều này hoàn tất chứng minh của (a) và (b) nếu lưu ý rằng phân bậc của $ S(\mathfrak{g}) $ là tương thích với cấu trúc đối đại số của nó.

Phân bậc $ (U^n)_{n \geq 0} $ của $ U $ được gọi là *phân bậc chính tắc*.

#### Hệ quả {#lie-ii-s1-n5-cor-1 .statement}

*Ánh xạ chính tắc $ \sigma $ xác định một đẳng cấu của $ \mathfrak{g} $ lên đại số Lie $ P(U) $ của các phần tử nguyên thủy của $ U $.*

Vì $ c^+ $ là một đồng cấu phân bậc bậc 0,

$$
P(U) = \sum_{n \geq 1} (P(U) \cap U^n).
$$

Chỉ cần chứng minh rằng nếu $ n > 1 $ và $ a \in U^n $ là nguyên thủy, thì $ a = 0 $. Bây giờ $ a $ có thể viết thành $ \sum_i \lambda_i a_i^n $, trong đó $ \lambda_i \in K $, $ a_i \in \sigma(g) $. Theo (12), số hạng có song bậc $ (1, n-1) $ trong $ c^+(a) $ là $ n \sum_i \lambda_i a_i \otimes a_i^{n-1} $. Do đó $ \sum_i \lambda_i a_i \otimes a_i^{n-1} = 0 $. Nếu $ \mu : U \otimes U \to U $ là ánh xạ tuyến tính được xác định bởi phép nhân trên $ U $, thì
$$
a = \sum_i \lambda_i a_i^n = \mu \left( \sum_i \lambda_i a_i \otimes a_i^{n-1} \right) = 0.
$$

#### Nhận xét {#lie-ii-s1-n5-rem-1 .statement}

(1) $ U_n = \sum_{i=0}^n U^i $ (Chương I, § 2, no. 7, Hệ quả 4 của Định lý 1).

(2) Ánh xạ $ \eta $ là cấu xạ duy nhất của các đốiđại số phân bậc từ $ S(g) $ vào $ U $ sao cho $ \eta(1) = 1 $ và $ \eta(x) = \sigma(x) $ với $ x \in g $. Thật vậy, nếu $ \eta' $ là một cấu xạ thỏa mãn các điều kiện ấy, ta chứng minh bằng quy nạp theo $ n $ rằng $ \eta'(x^n) = \eta(x^n) $ với $ x \in g $ và $ n > 1 $. Vì $ c_S^+(x^n) = \sum_{i=1}^{n-1} \binom{n}{i} x^i \otimes x^{n-i} $ theo (3) và (11),
$$
(\eta \otimes \eta)(c_S^+(x^n)) = (\eta' \otimes \eta')(c_S^+(x^n))
$$
theo giả thiết quy nạp. Suy ra $ c^+(\eta(x^n)) = c^+(\eta'(x^n)) $; do đó $ \eta(x^n) - \eta'(x^n) $ là một phần tử nguyên thủy bậc $ n $ và vì thế bằng không (Hệ quả của Mệnh đề 9).

(3) Gọi $ \psi $ là đẳng cấu chính tắc của song đại số $ TS(g) $ lên song đại số $ S(g) $ (Đại số, Chương IV, § 5, Hệ quả 1 của Mệnh đề 12). Ánh xạ
$$
\eta \circ \psi : TS(g) \to U
$$
được gọi là chính tắc. Đó là cấu xạ duy nhất $ \eta' $ của các đối đại số phân bậc từ $ TS(g) $ vào $ U $ sao cho $ \eta'(1) = 1 $ và $ \eta'(x) = \sigma(x) $ với mọi $ x \in g $.

(4) Gọi $ V $ là một không gian vectơ. Các phần tử nguyên thủy của song đại số $ S(V) $ là các phần tử bậc 1. Điều này suy ra từ Hệ quả của Mệnh đề 9 áp dụng cho đại số Lie giao hoán $ V $.

Cho $ (e_i)_{i \in I} $ là một cơ sở của không gian $ K $-vectơ $ g $, trong đó tập chỉ số $ I $ được sắp thứ tự toàn phần. Với mọi $ \alpha \in \mathbf{N}^{(I)} $, ta viết
$$
e_\alpha = \prod_{i \in I} \frac{\sigma(e_i)^{\alpha(i)}}{\alpha(i)!}.
$$
Các $ e_\alpha $, với $ |\alpha| \leq n $, tạo thành một cơ sở của không gian $ K $-vectơ $ U_n $ (Chương I, § 2, no. 7, Hệ quả 3 của Định lý 1). Khi đó
$$
e_0 = 1, \quad e_{e_i} = \sigma(e_i) \quad \text{với } i \in I.
$$

Vì đại số phân bậc liên kết với đại số được lọc U là giao hoán (loc. cit., Định lý 1), với $ \alpha, \beta $ trong $ \mathbf{N}^{(\Omega)} $,

$$
e_{\alpha} \cdot e_{\beta} \equiv ((\alpha, \beta)) \cdot e_{\alpha + \beta} \mod U_{|\alpha| + |\beta| - 1}.
$$

trong đó

$$
((\alpha, \beta)) = \prod_{i \in I} \frac{(\alpha(i) + \beta(i))!}{\alpha(i)! \beta(i)!}.
$$

Mặt khác, ta có ngay lập tức

$$
\varepsilon(e_0) = 1, \quad \varepsilon(e_{\alpha}) = 0 \quad \text{với } |\alpha| \geq 1.
$$

Cuối cùng, công thức (12) kéo theo rằng, với $ \alpha \in \mathbf{N}^{(\Omega)} $,

$$
c(e_{\alpha}) = \sum_{\beta + \gamma = \alpha} e_{\beta} \otimes e_{\gamma}.
$$

Công thức này cho phép ta xác định đại số đối ngẫu $ U' = \mathrm{Hom}(U, K) $ của đối đại số U (Đại số, Chương III, § 11, no. 2). Thật vậy, gọi $ K[[X_i]]_{i \in I} $ là đại số các chuỗi lũy thừa hình thức theo các bất định $ (X_i)_{i \in I} $ (x. Đại số, Chương III, § 2, no. 11); nếu $ \lambda \in U' $, ký hiệu $ f_{\lambda} $ là chuỗi lũy thừa hình thức

$$
f_{\lambda} = \sum_{\alpha} \langle \lambda, e_{\alpha} \rangle X^{\alpha}, \quad \text{trong đó } X^{\alpha} = \prod_{i \in I} X_i^{\alpha(i)}
$$

và chỉ số tổng $ \alpha $ chạy qua $ \mathbf{N}^{(\Omega)} $.

#### Mệnh đề 10 {#lie-ii-s1-prop-10 .statement}

*Ánh xạ* $ \lambda \mapsto f_{\lambda} $ *là một đẳng cấu của đại số* $ U' $ *lên đại số các chuỗi lũy thừa hình thức* $ K[[X_i]]_{i \in I} $.

Vì $ (e_{\alpha}) $ là một cơ sở của U, ánh xạ $ \lambda \mapsto f_{\lambda} $ là K-tuyến tính và song ánh. Mặt khác, với $ \lambda, \mu $ thuộc $ U' $,

$$
\begin{align*}
f_{\lambda \mu} &= \sum_{\alpha} \langle \lambda \mu, e_{\alpha} \rangle X^{\alpha} = \sum_{\alpha} \langle \lambda \otimes \mu, c(e_{\alpha}) \rangle X^{\alpha} \\
&= \sum_{\alpha} \langle \lambda \otimes \mu, \sum_{\beta + \gamma = \alpha} e_{\beta} \otimes e_{\gamma} \rangle X^{\alpha} \tag{by (16)} \\
&= \sum_{\beta, \gamma} \langle \lambda, e_{\beta} \rangle \langle \mu, e_{\gamma} \rangle X^{\beta + \gamma} = f_{\lambda} f_{\mu},
\end{align*}
$$

điều này cho thấy rằng $ \lambda \mapsto f_{\lambda} $ là một đẳng cấu *đại số* và hoàn tất chứng minh.

### 6. CẤU TRÚC CỦA CÁC SONG ĐẠI SỐ ĐƯỢC LỌC TRONG ĐẶC SỐ 0

Trong số này, ta tiếp tục giả thiết rằng K là một *trường có đặc số 0*.

Nếu E là một song đại số, đơn ánh chính tắc $ P(E) \to E $ có thể được mở rộng thành một cấu xạ song đại số $ f_E : U(P(E)) \to E $ (no. 4, Mệnh đề 8).

#### Định lý 1 {#lie-ii-s1-thm-1 .statement}

Cho E là một đại số kép đối giao hoán.
(a) Cấu xạ đại số kép $ f_E : U(P(E)) \to E $ là đơn ánh.
(b) Nếu trên E tồn tại một bộ lọc tương thích với cấu trúc đại số kép của nó (no. 3, Định nghĩa 2), thì cấu xạ $ f_E $ là một đẳng cấu.
(Trong trường hợp (b), vì thế đại số kép E được đồng nhất với đại số kép bao trùm của đại số Lie các phần tử nguyên thủy của nó.)
Ký hiệu $ c_E $ (resp. $ \varepsilon_E $) là đồng tích (resp. đồng đơn vị) của E. Ta viết $ g = P(E) $; gọi $ (e_i)_{i \in I} $ là một cơ sở của K-không gian vectơ g, trong đó tập hợp chỉ số I được sắp thứ tự toàn phần, và gọi $ (e_\alpha)_{\alpha \in \mathbf{N}^{(1)}} $ là cơ sở được đưa vào trong số trước. Ta viết $ X_\alpha = f_E(e_\alpha) $ với $ \alpha \in \mathbf{N}^{(1)} $. Theo (15) và (16), ta có:
$$
\varepsilon_E(X_0) = 1, \quad \varepsilon_E(X_\alpha) = 0 \quad \text{với } |\alpha| \geq 1,
$$
$$
c_E(X_\alpha) = \sum_{\beta + \gamma = \alpha} X_\beta \otimes X_\gamma \quad \text{với } \alpha \in \mathbf{N}^{(1)},
$$
vì $ f_E $ là một cấu xạ đối đại số.
Ta chứng minh rằng $ f_E $ là đơn ánh. Điều này suy ra từ bổ đề sau:

#### Bổ đề 2 {#lie-ii-s1-lem-2 .statement}

Cho V là một không gian vectơ, E là một đối đại số và $ f : S(V) \to E $ là một cấu xạ đối đại số. Nếu hạn chế của f lên $ S^0(V) + S^1(V) $ là đơn ánh, thì f là đơn ánh.
Cho $ n \geq 0 $; đặt $ S_n = \sum_{i \geq n} S^i(V) $ và $ c_S $ là đồng tích của $ S(V) $ rồi chứng minh bằng quy nạp theo n rằng $ f | S_n $ là đơn ánh. Vì mệnh đề là tầm thường đối với $ n = 0 $ và $ n = 1 $, ta giả sử rằng $ n \geq 2 $ và lấy $ u \in S_n $ sao cho $ f(u) = 0 $. Khi đó
$$
0 = c_E(f(u)) = (f \otimes f)(c_S(u))
= f(u) \otimes 1 + 1 \otimes f(u) + (f \otimes f)(c_S^+(u))
= (f \otimes f)(c_S^+(u)).
$$
Vì $ c_S^+(u) \in S_{n-1} \otimes S_{n-1} $, theo (11) giả thiết quy nạp cho thấy rằng u là một phần tử nguyên thủy của $ S(V) $, do đó có bậc 1 (no. 5, Nhận xét 4) và vì thế bằng không, vì $ f | S^1(V) $ là đơn ánh.
Đặc biệt suy ra rằng họ $ (X_\alpha) $ là tự do.
Ta chứng minh rằng $ f_E $ là toàn ánh nếu E có một lọc tương thích với cấu trúc song đại số của nó. Cho $ (E_n)_{n \geq 0} $ là một lọc như vậy và đặt $ E_n^+ = E_n \cap \mathrm{Ker}(\varepsilon_E) $. Ta chứng minh bằng quy nạp theo n rằng $ E_n^+ $ được chứa trong ảnh của $ f_E $. Vì $ E = K.1 + \bigcup_{n \geq 0} E_n^+ $, điều này sẽ kéo theo tính toàn ánh của $ f_E $. Mệnh đề là tầm thường đối với $ n = 0 $ và suy ra từ Hệ quả của Mệnh đề 6 ở no. 3 đối với $ n = 1 $; từ đây giả sử rằng $ n \geq 2 $ và lấy $ x \in E_n^+ $. Theo Mệnh đề 6 ở no. 3,
$$
c_E^+(x) \in \sum_{i=1}^{n-1} E_i^+ \otimes E_{n-i}^+
$$

và theo giả thiết quy nạp tồn tại các vô hướng $ \lambda_{\alpha, \beta} $, trong đó $ \alpha, \beta $ thuộc $ \mathbf{N}^{(\Omega)} $, đều bằng không trừ một số hữu hạn, sao cho

(19)
$$
c_E^+ (x) = \sum_{\alpha, \beta \neq 0} \lambda_{\alpha, \beta} X_\alpha \otimes X_\beta.
$$

Do đó theo công thức (18)

$$
(c_E^+ \otimes \mathrm{Id}_E)(c_E^+ (x)) = \sum_{\alpha, \beta, \gamma \neq 0} \lambda_{\alpha + \beta, \gamma} X_\alpha \otimes X_\beta \otimes X_\gamma
$$
$$
(\mathrm{Id}_E \otimes c_E^+)(c_E^+ (x)) = \sum_{\alpha, \beta, \gamma \neq 0} \lambda_{\alpha, \beta + \gamma} X_\alpha \otimes X_\beta \otimes X_\gamma.
$$

Theo Mệnh đề 3 của no. 1 và tính độc lập tuyến tính của các $ X_\alpha $ suy ra rằng

(20)
$$
\lambda_{\alpha + \beta, \gamma} = \lambda_{\alpha, \beta + \gamma} \quad \text{với } \alpha, \beta, \gamma \text{ trong } \mathbf{N}^{(\Omega)} - \{0\}.
$$

Mặt khác, đồng tích $ c_E $ là đối giao hoán; cùng lập luận như trên cho

(21)
$$
\lambda_{\alpha, \beta} = \lambda_{\beta, \alpha} \quad \text{với } \alpha, \beta \text{ trong } \mathbf{N}^{(\Omega)} - \{0\}.
$$

Giả sử rằng tồn tại một họ các vô hướng $ (\mu_\alpha) $ với $ |\alpha| \geq 2 $, sao cho

(22)
$$
\mu_{\alpha + \beta} = \lambda_{\alpha, \beta} \quad \text{với } \alpha, \beta \text{ trong } \mathbf{N}^{(\Omega)} - \{0\}.
$$

Khi đó
$$
c_E^+ (x) = \sum_{\alpha, \beta \neq 0} \mu_{\alpha + \beta} X_\alpha \otimes X_\beta = \sum_{|\gamma| \geq 2} \mu_\gamma c_E^+ (X_\gamma)
$$
theo công thức (18), do đó $ y = x - \sum_{|\gamma| \geq 2} \mu_\gamma X_\gamma $ là nguyên thủy và vì thế thuộc $ P(E) \subset \mathrm{Im}(f_E) $. Suy ra
$$
x = y + \sum_{|\gamma| \geq 2} \mu_\gamma f_E(e_\gamma) \in \mathrm{Im}(f_E).
$$

Vậy chứng minh sẽ đầy đủ khi chúng ta chứng minh bổ đề sau:

#### Bổ đề 3 {#lie-ii-s1-lem-3 .statement}

*Nếu một họ các vô hướng* $ (\lambda_{\alpha, \beta}) $ *có giá hữu hạn* (với $ \alpha, \beta $ thuộc $ \mathbf{N}^{(\Omega)} - \{0\} $) *thỏa mãn các hệ thức* (20) *và* (21), *thì tồn tại một họ* $ (\mu_\alpha)_{|\alpha| \geq 2} $ *có giá hữu hạn sao cho* $ \mu_{\alpha + \beta} = \lambda_{\alpha, \beta} $ *với* $ \alpha, \beta $ *khác không*.

Chỉ cần chứng minh rằng

(23)
$$
\alpha + \beta = \gamma + \delta
$$

suy ra $ \lambda_{\alpha, \beta} = \lambda_{\gamma, \delta} $ với $ \alpha, \beta, \gamma, \delta $ khác không. Theo Bổ đề phân tích của Riesz (*Đại số*, Chương VI, § 1, no. 10, Định lý 1) tồn tại $ \pi, \rho, \sigma, \tau $ trong $ \mathbf{N}^{(\Omega)} $ sao cho
$$
\alpha = \pi + \sigma, \qquad \beta = \rho + \tau, \qquad \gamma = \pi + \rho, \qquad \delta = \sigma + \tau.
$$

Giả sử $ \pi \neq 0 $; vì $ \sigma + \beta = \rho + \delta $, quan hệ (20) suy ra
$$
\lambda_{\alpha, \beta} = \lambda_{\pi + \sigma, \beta} = \lambda_{\pi, \sigma + \beta} = \lambda_{\pi, \rho + \delta} = \lambda_{\pi + \rho, \delta} = \lambda_{\gamma, \delta}.
$$
Mặt khác nếu $ \pi = 0 $, thì $ \beta = \gamma + \tau $ và $ \delta = \alpha + \tau $, do đó
$$
\lambda_{\alpha, \beta} = \lambda_{\alpha, \gamma + \tau} = \lambda_{\alpha + \tau, \gamma} = \lambda_{\delta, \gamma}
$$
theo (20), nhưng cũng có $ \lambda_{\delta, \gamma} = \lambda_{\gamma, \delta} $ theo (21), do đó $ \lambda_{\alpha, \beta} = \lambda_{\gamma, \delta} $.

### Bài tập {#lie-ii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
