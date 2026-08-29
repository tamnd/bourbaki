---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 3
section_title: Integrals of continuous vector-valued functions
lang: vi
source: int-i-vi
book_pages: INT III.32-INT III.40, INT III.60
pdf_pages: 0077-0085, 0105-0105
extraction: ocr
subsections:
    - "no": 1
      title: Definition of the integral of a vector-valued function
      page: 32
      pdf_page: 77
    - "no": 2
      title: Properties of the vectorial integral
      page: 34
      pdf_page: 79
    - "no": 3
      title: Criteria for the integral to belong to $E$
      page: 37
      pdf_page: 82
    - "no": 4
      title: Continuity properties of the integral
      page: 39
      pdf_page: 84
statements: 17
exercises: 4
content_sha256: 17e80f91040900ffe68a640ebbd75480c381d3b92d3710071c42e88ceb91f776
translated_from: content/en/int/III/03_s3_integrals_of_continuous_vector_valued.md
source_content_sha256: 08e80431efbc022e93acec00bafa9892334f63e19b825a718a5f6da8a6173417
translation_model: gpt-5.4
translation_run: translate-vi-f3da66a2
glossary_version: 34
glossary_terms_sha256: 7172cbb25a42069bb745a07ffdc7e47667e8797448130f8b50df0f3f731d59f1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. TÍCH PHÂN CỦA CÁC HÀM LIÊN TỤC NHẬN GIÁ TRỊ VECTƠ

*Trong suốt tiết này, X ký hiệu một không gian địa phương compact, E một không gian lồi địa phương trên $\mathbf{R}$ hoặc $\mathbf{C}$. Ta ký hiệu bởi $E'$ đối ngẫu của E (không gian các dạng tuyến tính liên tục trên E) và bởi ${E'}^*$ đối ngẫu đại số của $E'$ (không gian mọi dạng tuyến tính trên $E'$); với $z \in E$, $z' \in E'$, ${z'}^* \in {E'}^*$, ta viết $\langle z, z' \rangle = z'(z)$, $\langle {z'}^*, z' \rangle = {z'}^*(z')$.

Nhắc lại rằng nếu E là Hausdorff, thì E có thể được đồng nhất với một không gian con tuyến tính của ${E'}^*$ bằng cách đồng nhất một phần tử $z \in E$ với dạng tuyến tính $z' \mapsto \langle z, z' \rangle$ trên $E'$, và rằng ${E'}^*$, được trang bị tôpô yếu $\sigma({E'}^*, E')$, có thể được đồng nhất một cách chính tắc với đầy đủ hóa của E được trang bị tôpô làm yếu $\sigma(E, E')$.

### 1. Định nghĩa của tích phân của một hàm nhận giá trị vectơ

Nhắc lại rằng một ánh xạ f từ X vào E được gọi là *liên tục yếu* nếu, với mọi $z' \in E'$, ánh xạ $x \mapsto \langle f(x), z' \rangle$ từ X vào $\mathbf{C}$ (nói cách khác ánh xạ $z' \circ f$, cũng được ký hiệu là $\langle f, z' \rangle$) là liên tục. Ta sẽ nói rằng một ánh xạ f từ X vào E là *có giá vô hướng với giá đỡ compact* nếu, với mọi $z' \in E'$, ánh xạ $x \mapsto \langle f(x), z' \rangle$ có giá đỡ compact. Ta ký hiệu bởi $\widetilde{\mathcal{K}}(X; E)$ không gian các ánh xạ từ X vào E mà *liên tục yếu và có giá vô hướng với giá đỡ compact*; hiển nhiên là $\widetilde{\mathcal{K}}(X; E) \supset \mathcal{K}(X; E)$, nhưng hai không gian này không nhất thiết trùng nhau (xem *Ví dụ* 2 dưới đây); tuy nhiên, chúng bằng nhau khi E hữu hạn chiều.

Chú ý rằng trong định nghĩa của một hàm liên tục yếu (tương ứng, có giá vô hướng với giá đỡ compact), tôpô của E chỉ can thiệp thông qua đối ngẫu $E'$ của E; do đó, tập hợp các hàm ấy không thay đổi khi tôpô của E được thay bằng bất kỳ tôpô lồi địa phương nào mà đối ngẫu vẫn là như nhau.

Nếu E và F là hai không gian vectơ đối ngẫu với nhau, ta lưu ý rằng nói một ánh xạ từ X vào E là *liên tục* đối với $\sigma(E, F)$ hay nói rằng nó là *liên tục yếu* là cùng một nghĩa.

Cho $f$ là một ánh xạ từ $X$ vào $E$, liên tục yếu và có giá vô hướng với giá đỡ compact, và cho $\mu$ là một độ đo trên $X$; với mọi $z' \in E'$ ta có $z' \circ f \in \mathcal{K}(X)$; đặt

$$
\varphi(z') = \int \langle f(x), z' \rangle d\mu(x) = \mu(z' \circ f).
$$

Hiển nhiên $\varphi$ là một dạng tuyến tính trên $E'$, do đó là *một phần tử của ${E'}^*$*.

#### Định nghĩa 1 {#int-iii-s3-def-1 .statement}

*Với mọi hàm $f \in \widetilde{\mathcal{K}}(X;E)$, ta gọi là tích phân của $f$ đối với $\mu$, và ký hiệu bởi $\int f d\mu$ hoặc $\int f(x) d\mu(x)$, hoặc $\int f \mu$, hoặc $\int f(x)\mu(x)$, phần tử của ${E'}^*$ được xác định bởi*

$$
\left\langle \int f d\mu, z' \right\rangle = \int \langle f, z' \rangle d\mu \quad \text{for all } z' \in E'.
$$

Ta lưu ý rằng ngay cả khi $E$ là *Hausdorff* và $f \in \mathcal{K}(X;E)$, *không nhất thiết có* $\int f d\mu \in E$ (Bài tập 1; xem No. 3).

#### Ví dụ {#int-iii-s3-n1-exa-1 .statement}

— 1) Giả sử rằng $E$ là *hữu hạn chiều* trên $\mathbf{C}$ và Hausdorff, để nếu $(e_i)_{1 \leq i \leq n}$ là một cơ sở của $E$ thì ánh xạ

$$
(\xi_1, \ldots \xi_n) \mapsto \sum_{i=1}^n \xi_i e_i
$$

là một *đẳng cấu* từ $\mathbf{C}^n$ lên $E$. Khi đó ta biết rằng mọi dạng tuyến tính trên $E$ đều liên tục, nói cách khác $E'$ đồng nhất với đối ngẫu đại số $E^*$ của $E$, và ${E'}^*$ có thể được đồng nhất với $E$ một cách chính tắc. Gọi $(e'_i)_{1 \leq i \leq n}$ là cơ sở của $E'$ đối ngẫu với $(e_i)$; để một ánh xạ $f$ từ $X$ vào $E$ là liên tục yếu và có giá vô hướng với giá đỡ compact, điều kiện cần và đủ là các hàm $f_i = e'_i \circ f$ liên tục và có giá đỡ compact; khi đó ta có $f(x) = \sum_{i=1}^n f_i(x) e_i$ với mọi $x \in X$, và

$$
\int f d\mu = \sum_{i=1}^n \mu(f_i) e_i.
$$

2) Lấy $E$ là không gian $\mathcal{M}(X; \mathbf{C})$ các độ đo trên $X$, được trang bị tôpô *mơ hồ* (§ 1, No. 9); khi đó đối ngẫu $E'$ của $E$ có thể được đồng nhất một cách chính tắc với không gian $\mathcal{K}(X; \mathbf{C})$ (TVS, II, § 6, No. 2, Prop. 3). Ánh xạ $x \mapsto \varepsilon_x$ từ $X$ vào $E$ là *liên tục* (§ 1, No. 9, Prop. 13), nhưng giá đỡ của nó không compact nếu $X$ không compact; tuy nhiên, nó *có giá đỡ compact về mặt vô hướng*, vì với mọi hàm $f \in E'$ thì hàm $x \mapsto \langle \varepsilon_x, f \rangle = f(x)$ theo định nghĩa có giá đỡ compact. Hơn nữa,

$$
\int \langle \varepsilon_x, f \rangle d\mu = \int f(x) d\mu(x) = \langle \mu, f \rangle
$$

với mọi hàm $f \in \mathcal{K}(X; \mathbf{C}) = E'$, điều này chứng tỏ rằng

$$
\int \varepsilon_x d\mu(x) = \mu
$$

với mọi độ đo $\mu$ trên $X$.

3) Nếu $E$ là Hausdorff thì, với mọi điểm $y \in X$ và mọi hàm $f \in \widetilde{\mathcal{K}}(X; E)$, ta có

$$
\int f d\varepsilon_y = f(y)
$$

vì theo định nghĩa $\int \langle f, z' \rangle d\varepsilon_y = \langle f(y), z' \rangle$.

#### Nhận xét 1 {#int-iii-s3-n1-rem-1 .statement}

Nếu $E$ là một không gian lồi địa phương và $N$ là bao đóng của $\{0\}$ trong $E$, để $E_1 = E/N$ là không gian lồi địa phương Hausdorff liên kết với $E$, thì ta biết rằng các đối ngẫu $E'$ và $E'_1$ là đồng nhất; để một hàm $f$ thuộc $\widetilde{\mathcal{K}}(X; E)$, điều kiện cần và đủ là $f_1 = \pi \circ f$ (trong đó $\pi : E \to E_1$ là đồng cấu chính tắc) thuộc $\widetilde{\mathcal{K}}(X; E_1)$, và trong trường hợp đó $\int f d\mu = \int f_1 d\mu$. Do đó ta có thể chỉ giới hạn ở việc xét các không gian lồi địa phương *Hausdorff*.

#### Nhận xét 2 {#int-iii-s3-n1-rem-2 .statement}

Cho $E$ là một không gian lồi địa phương *trên* $\mathbf{C}$, và gọi $E_0$ là không gian lồi địa phương *trên* $\mathbf{R}$ nằm dưới $E$; ta biết rằng ánh xạ $z' \mapsto \Re z'$ mà với mọi dạng tuyến tính liên tục (phức) $z'$ trên $E$, tương ứng dạng tuyến tính liên tục (thực) $z \mapsto \Re \langle z, z' \rangle$ trên $E_0$, là một $\mathbf{R}$-đẳng cấu của đối ngẫu $E'$ lên đối ngẫu $E'_0$ của $E_0$ (TVS, II, §8, No. 1). Tương tự, đối ngẫu đại số $E'_0*$ của không gian vectơ thực $E'_0$ có thể được đồng nhất một cách chính tắc với không gian thực nằm dưới đối ngẫu đại số $E'*$ của $E'$. Suy ra rằng nếu $\mu$ là một *độ đo thực* và $f$ là một ánh xạ trong $\widetilde{\mathcal{K}}(X; E)$, thì công thức (1) vẫn còn đúng khi coi $f$ như nhận giá trị trong $E_0$ và các dạng song tuyến tính chính tắc xuất hiện trong hai vế lần lượt là tương đối với đối ngẫu giữa $E'_0$ và $E'_0*$ đối với vế thứ nhất và đối ngẫu giữa $E_0$ và $E'_0$ đối với vế thứ hai.

### 2. Các tính chất của tích phân vectơ

#### Mệnh đề 1 {#int-iii-s3-prop-1 .statement}

— *Ánh xạ*

$$
(f, \mu) \mapsto \int f d\mu
$$

từ $\widetilde{\mathcal{K}}(X; E) \times \mathcal{M}(X; \mathbf{C})$ vào $E'*$ *là song tuyến tính*.

Mệnh đề được suy ra ngay lập tức từ Định nghĩa 1 của No. 1.

Cho $u$ là một ánh xạ tuyến tính liên tục từ $E$ vào một không gian lồi địa phương $F$; ta biết rằng chuyển vị $^t u$ là một ánh xạ tuyến tính từ đối ngẫu $F'$ của $F$ vào đối ngẫu $E'$ của $E$; ta sẽ ký hiệu bởi $^{tt} u$ ánh xạ ${E'}^* \to {F'}^*$, chuyển vị của $^t u$ (theo nghĩa đại số); khi $E$ và $F$ là Hausdorff và được đồng nhất một cách chính tắc với các không gian con của ${E'}^*$ và ${F'}^*$ tương ứng, thì $^{tt} u$ mở rộng ánh xạ $u$. Với các ký hiệu này:

#### Mệnh đề 2 {#int-iii-s3-prop-2 .statement}

— Cho $u$ là một ánh xạ tuyến tính liên tục từ $E$ vào một không gian lồi địa phương $F$; với mọi hàm $f \in \widetilde{\mathcal{K}}(X;E)$, hàm $u \circ f$ thuộc $\widetilde{\mathcal{K}}(X;F)$ và

$$
\int u(f(x))\, d\mu(x) = ^{tt} u \left( \int f(x)\, d\mu(x) \right).
$$

Với mọi dạng tuyến tính liên tục $z' \in F'$, ta có $z' \circ u \circ f = y' \circ f$ khi đặt $y' = z' \circ u = {}^t u(z') \in E'$, do đó có mệnh đề thứ nhất; hơn nữa, với mọi $z' \in F'$,

$$
\left\langle \int (u \circ f)\, d\mu, z' \right\rangle = \int \langle u \circ f, z' \rangle\, d\mu = \int \langle f, {}^t u(z') \rangle\, d\mu \\
= \left\langle \int f\, d\mu, {}^t u(z') \right\rangle = \left\langle {}^{tt} u \left( \int f\, d\mu \right), z' \right\rangle,
$$

do đó có công thức (2).

#### Mệnh đề 3 {#int-iii-s3-prop-3 .statement}

— Với mọi hàm $g \in \mathcal{C}(X;\mathbf{C})$ và mọi hàm $f \in \widetilde{\mathcal{K}}(X;E)$, hàm $gf$ thuộc $\widetilde{\mathcal{K}}(X;E)$ và

$$
\int f\, d(g \cdot \mu) = \int fg\, d\mu.
$$

Thật vậy, với mọi $z' \in E'$, $\langle gf, z' \rangle = g \langle f, z' \rangle$, do đó có mệnh đề thứ nhất; hơn nữa,

$$
\left\langle \int f\, d(g \cdot \mu), z' \right\rangle = \int \langle f, z' \rangle\, d(g \cdot \mu) = \int g \langle f, z' \rangle\, d\mu \\
= \int \langle gf, z' \rangle\, d\mu = \left\langle \int gf\, d\mu, z' \right\rangle,
$$

do đó có (3).

#### Mệnh đề 4 {#int-iii-s3-prop-4 .statement}

— Cho $\mu$ là một độ đo dương trên $X$, $S$ là giá của nó, và $f$ là một hàm trong $\widetilde{\mathcal{K}}(X;E)$. Giả sử $E$ là Hausdorff, và trang bị cho không gian ${E'}^*$ tôpô yếu $\sigma({E'}^*, E')$.

(i) *Tích phân* $\int f\, d\mu$ *thuộc bao đóng* C *trong* E'** *của nón lồi sinh bởi* f(S).

(ii) *Nếu* $\mu$ *bị chặn, thì tích phân* $\int f\, d\mu$ *thuộc tập hợp* $\| \mu \| \cdot D$, *trong đó* D *là bao lồi đóng của* f(S) *trong* E'**.

Nếu E là phức, ta trang bị cho E cấu trúc không gian vectơ *thực* nền của nó, như ta đã thấy, điều này không làm thay đổi công thức (1).

(i) Ta biết rằng C là giao của các nửa-không gian đóng trong E'** chứa f(S) và được xác định bởi các siêu phẳng đóng đi qua 0; do đó chỉ cần chứng minh rằng, với $z' \in E'$, quan hệ $\langle f(x), z' \rangle \geq 0$ với mọi $x \in S$ kéo theo

$$
\left\langle \int f\, d\mu, z' \right\rangle \geq 0;
$$

nhưng vì

$$
\left\langle \int f\, d\mu, z' \right\rangle = \int \langle f, z' \rangle\, d\mu,
$$

điều này suy ra từ §2, No. 3, Hệ quả 2 của Mệnh đề 8.

(ii) Ta biết rằng D là giao của các nửa-không gian đóng trong E'** chứa f(S); do đó chỉ cần chỉ ra rằng, với $z' \in E'$, quan hệ $\langle f(x), z' \rangle \leq a$ với mọi $x \in S$ kéo theo

$$
\left\langle \int f\, d\mu, z' \right\rangle \leq a \| \mu \|;
$$

nhưng điều này suy ra từ §2, No. 3, Hệ quả 3 của Mệnh đề 8.

#### Hệ quả {#int-iii-s3-n2-cor-1 .statement}

*Cho* $\mu$ *là một độ đo dương trên* X, $f$ *là một ánh xạ thuộc* $\mathcal{K}(X;E)$, *và* D *là bao lồi đóng của* f(X) *trong* E'**. *Tồn tại một số* $a > 0$ *sao cho* $\int f\, d\mu \in a \cdot D$.

*Nếu* $\nu$ *là một độ đo bất kỳ trên* X, *thì tồn tại các số* $a_1, a_2, a_3, a_4 > 0$ *sao cho* $\int f\, d\nu \in a_1 D - a_2 D + i a_3 D - i a_4 D$.

Trước hết giả sử $\mu$ là dương; theo giả thiết, giá K của f là compact; nếu $\nu$ là hạn chế của $\mu$ lên một lân cận mở tương đối compact của K, thì $\nu$ bị chặn và $\int f\, d\mu = \int f\, d\nu \in \| \nu \| \cdot D$ theo Mệnh đề 4, (ii). Kết quả thứ hai suy ra từ đó, vì mọi độ đo phức đều có thể viết dưới dạng $\mu_1 - \mu_2 + i \mu_3 - i \mu_4$, trong đó các $\mu_j$ là dương.

#### Mệnh đề 5 {#int-iii-s3-prop-5 .statement}

*Giả sử rằng không gian* X *là compact, và cho* f *là một ánh xạ liên tục từ* X *vào một không gian lồi địa phương Hausdorff* E. *Bao lồi đóng của* f(X) *trong* E'** *(đối với* $\sigma(E', E')$) *bằng tập hợp các vectơ* $\int f\, d\mu$ *ứng với mọi độ đo dương* $\mu$ *trên* X *có tổng khối lượng* 1.

Cho C là bao lồi đóng của $f(X)$ trong $E'**$; vì $f(X)$ là compact và $E'**$ là *đầy đủ*, C là compact. Ta đã biết (Mệnh đề 4) rằng $\int f d\mu \in C$ với mọi độ đo $\mu$ thuộc tập lồi H gồm các độ đo dương trên $X$ có tổng khối lượng bằng 1. Mặt khác, H là lồi và *compact* đối với tôpô mờ (§ 1, No. 9, Hệ quả 3 của Mệnh đề 15) và là bao đóng (đối với tôpô này) của tập lồi $H_0$ gồm các độ đo dương có khối lượng 1 và giá hữu hạn (§ 2, No. 4, Hệ quả 3 của Định lý 1). Khi đó, ảnh của $H_0$ dưới ánh xạ $\mu \mapsto \int f d\mu$ là bao lồi $C_0$ của $f(X)$ trong ${E'}^*$. Mặt khác, ánh xạ này liên tục đối với tôpô mờ trên $\mathcal{M}(X; C)$ và tôpô $\sigma({E'}^*, E')$ trên ${E'}^*$ vì $\langle \int f d\mu, z' \rangle = \int \langle f, z' \rangle d\mu$ theo định nghĩa; do đó ảnh của $H = \overline{H_0}$ là một tập lồi *compact* chứa $C_0$ và được chứa trong $C$; vì $C = \overline{C_0}$, ảnh này bằng $C$.

#### Mệnh đề 6 {#int-iii-s3-prop-6 .statement}

*Với mọi ánh xạ liên tục có giá compact $f$ từ $X$ vào một không gian lồi địa phương Hausdorff $E$, mọi nửa chuẩn liên tục $q$ trên $E$ và mọi độ đo $\mu$ trên $X$ sao cho $\int f d\mu \in E$,*

$$
q \left( \int f d\mu \right) \leq \int (q \circ f) \ d|\mu|.
$$

Cho $D$ là tập các $z \in E$ sao cho $q(z) \leq 1$; D là đóng, lồi và chứa 0, do đó $D = D^{o o}$ (TVS, II, § 6, No. 3, Hệ quả 3 của Định lý 1). Vậy chỉ cần chứng minh rằng với mọi $z' \in D^o$,

$$
\left| \left\langle \int f d\mu, z' \right\rangle \right| \leq \int (q \circ f) \ d|\mu|;
$$

vì

$$
\left\langle \int f d\mu, z' \right\rangle = \int \langle f, z' \rangle d\mu,
$$

và vì, theo định nghĩa của $D^o$,

$$
|\langle f(x), z' \rangle| \leq q(f(x))
$$

với mọi $x \in X$, bất đẳng thức cần chứng minh suy ra từ bất đẳng thức (13) của § 1, No. 6.

### 3. Các tiêu chuẩn để tích phân thuộc $E$

#### Mệnh đề 7 {#int-iii-s3-prop-7 .statement}

*Cho $E$ là một không gian lồi địa phương Hausdorff, và $f \in \mathcal{K}(X; E)$. Nếu $f(X)$ được chứa trong một tập con lồi đầy đủ $A$ của $E$, thì $\int f d\mu \in E$.*

Cho K là giá của f, tập này compact theo giả thiết. Vì f bằng không trên X − K, $f(X)$ bằng $f(K)$ hoặc $f(K) \cup \{0\}$, do đó là compact vì f liên tục và E là Hausdorff; khi đó bao lồi đóng C của $f(X)$ trong E là tiền compact (đối với cấu trúc đều do cấu trúc đều của E cảm sinh) (TVS, II, §4, No. 1, Mệnh đề 3). Nhưng vì C là một tập con đóng của không gian đầy đủ A, C là đầy đủ và do đó compact; a fortiori, C là compact đối với tôpô yếu đi σ(E, E′); nhưng vì tôpô đó được cảm sinh bởi σ(E′*, E′), C là bao lồi đóng của $f(X)$ trong E′* đối với tôpô σ(E′*, E′); vì vậy chứng minh được kết thúc nhờ Hệ quả của Mệnh đề 4 ở No. 2.

#### Hệ quả 1 {#int-iii-s3-prop-7-cor-1 .statement}

— Cho E là một không gian lồi địa phương Hausdorff; với mọi hàm f ∈ 𝒦(X; E), $\int f d\mu$ thuộc hoàn thành $\widehat{E}$ của E.

Vì các đối ngẫu của E và $\widehat{E}$ là đồng nhất, chỉ cần áp dụng Mệnh đề 7 khi xem f như nhận giá trị trong $\widehat{E}$.

#### Hệ quả 2 {#int-iii-s3-prop-7-cor-2 .statement}

— Nếu E là một không gian lồi địa phương Hausdorff quasi-đầy đủ, thì $\int f d\mu \in E$ với mọi hàm f ∈ 𝒦(X; E).

Như đã nhận xét ở đầu chứng minh của Mệnh đề 7, $f(X)$ là compact và bao lồi đóng C của nó trong E là tiền compact, do đó bị chặn; nhưng vì tập C là đóng và bị chặn, nó là đầy đủ theo giả thiết, và chỉ cần áp dụng Mệnh đề 7.

Ta sẽ thấy, trong Ch. VI, §1, No. 2, những tiêu chuẩn khác để $\int f d\mu$ thuộc E, áp dụng đặc biệt cho các hàm trong $\widetilde{\mathcal{K}}(X; E)$ chứ không chỉ cho những hàm trong $\mathcal{K}(X; E)$.

Hệ quả 2 của Mệnh đề 7 có thể được áp dụng trong hai trường hợp sau:
1° E là một không gian Banach; 2° E là đối ngẫu của một không gian lồi địa phương Hausdorff thùng G, và E được trang bị một $\mathcal{S}$-tôpô, trong đó $\mathcal{S}$ là một phủ của G bởi các tập con bị chặn (TVS, III, §4, No. 2, Hệ quả 4 của Định lý 1). Chẳng hạn, Hệ quả 2 của Mệnh đề 7 có thể được áp dụng khi E là đối ngẫu yếu của một không gian Banach, hoặc một không gian các độ đo $\mathcal{M}(Y; \mathbf{C})$ được trang bị tôpô mờ.

Nếu X = $\mathbf{R}$, $\mu$ là độ đo Lebesgue trên $\mathbf{R}$, và E là một không gian Banach, thì tích phân $\int f d\mu$ của một hàm trong $\mathcal{K}(X; E)$ không là gì khác ngoài tích phân

$$
\int_{-\infty}^{+\infty} f(x)\, dx
$$

được định nghĩa trong FRV, II, §2, No. 1; điều này suy ra từ công thức (1), và từ FRV, I, §1, No. 2, Hệ quả của Mệnh đề 2.

### 4. Các tính chất liên tục của tích phân

#### Mệnh đề 8 {#int-iii-s3-prop-8 .statement}

— Giả sử E là Hausdorff; gọi $\mu$ là một độ đo trên X. Ánh xạ $f \mapsto \int f d\mu$ từ $\mathcal{K}(X;E)$ vào $\widehat{E}$ (No. 3, Hệ quả 1 của Mệnh đề 7) là ánh xạ tuyến tính liên tục duy nhất $\Phi$ sao cho $\Phi(g \cdot a) = \mu(g) \cdot a$ với mọi vectơ $a \in E$ và mọi hàm $g \in \mathcal{K}(X;\mathbf{C})$.

Để chứng minh tính liên tục của ánh xạ $f \mapsto \int f d\mu$, chỉ cần chỉ ra rằng hạn chế của nó trên $\mathcal{K}(X,K;E)$ là liên tục với mọi tập con compắc K của X (TVS, II, §4, No. 4, Mệnh đề 5). Ta chú ý rằng nếu tôpô của E được xác định bởi một họ các nửa chuẩn $(q_\alpha)$, thì tôpô của $\mathcal{K}(X,K;E)$ được xác định bởi họ các nửa chuẩn

$$
p_\alpha(f) = \sup_{x \in K} q_\alpha(f(x)) .
$$

Bây giờ, gọi $h$ là một ánh xạ liên tục từ X vào $[0,1]$, có giá compắc và sao cho $h(x) = 1$ trên K; theo No. 2, Mệnh đề 6 ta có, với mọi hàm $f \in \mathcal{K}(X,K;E)$,

$$
q_\alpha \left( \int f d\mu \right) = q_\alpha \left( \int h f d\mu \right) \leq \int h(x) q_\alpha(f(x)) d|\mu|(x) \leq |\mu|(h) \cdot p_\alpha(f)
$$

(các $q_\alpha$ được mở rộng bằng liên tục lên $\widehat{E}$), điều này chứng minh tính liên tục của $f \mapsto \int f d\mu$. Mặt khác, với các ký hiệu của mệnh đề,

$$
\int (g(x) \cdot a) d\mu(x) = \mu(g) \cdot a
$$

do No. 1, Ví dụ 1 và Mệnh đề 2 của No. 2 áp dụng cho đơn ánh chính tắc $\mathbf{C} \cdot a \to E$. Hơn nữa, không gian con của $\mathcal{K}(X;E)$ tạo thành bởi các tổ hợp tuyến tính $\sum_i g_i \cdot a_i$, trong đó $a_i \in E$ và $g_i \in \mathcal{K}(X;\mathbf{C})$, là trù mật trong $\mathcal{K}(X;E)$ (§1, No. 2, Mệnh đề 5), điều này hoàn tất chứng minh.

#### Mệnh đề 9 {#int-iii-s3-prop-9 .statement}

— Giả sử E là Hausdorff; gọi $f$ là một ánh xạ liên tục từ X vào E có giá compắc. Khi không gian $\mathcal{M}(X;\mathbf{C})$ được trang bị tôpô hội tụ compắc chặt (§1, No. 10), ánh xạ $\mu \mapsto \int f d\mu$ từ $\mathcal{M}(X;\mathbf{C})$ vào $\widehat{E}$ là ánh xạ tuyến tính liên tục duy nhất $\Psi$ sao cho $\Psi(\varepsilon_x) = f(x)$ với mọi $x \in X$.

Với mọi $z' \in E'$,

$$
\left\langle \int f d\varepsilon_x, z' \right\rangle = \int (z' \circ f) d\varepsilon_x = z'(f(x)) = \langle f(x), z' \rangle ,
$$

do đó $\int f\, d\varepsilon_x = f(x)$. Hơn nữa, ta biết rằng tập hợp các độ đo điểm là toàn phần trong $\mathcal{M}(X; \mathbf{C})$ đối với tôpô hội tụ chặt-compact (§ 2, No. 4, Hệ quả 4 của Định lý 1). Vì vậy, tất cả quy về việc chứng minh tính liên tục của ánh xạ tuyến tính $u : \mu \mapsto \int f\, d\mu$. Để làm điều đó, xét ánh xạ tuyến tính $v : z' \mapsto \langle f, z' \rangle$ từ $E'$ vào $\mathcal{K}(X; \mathbf{C})$, và ta sẽ chỉ ra rằng ảnh qua $v$ của một tập con đồng liên tục $H$ của $E'$ được chứa trong một tập con chặt-compact của $\mathcal{K}(X; \mathbf{C})$. Thật vậy, nếu $K$ là giá của $f$, thì các hàm $\langle f, z' \rangle$ với $z' \in H$ có giá được chứa trong $K$; mặt khác, các hàm này tạo thành một tập đồng liên tục, và với mỗi $x \in X$ thì tập hợp các $z'(f(x))$ là bị chặn; do đó mệnh đề của chúng ta suy ra từ định lý Ascoli (GT, X, § 2, No. 5, Hệ quả 3 của Định lý 2). Bây giờ, từ công thức (1) của No. 1 suy ra rằng $u$ không là gì khác hơn hạn chế của chuyển vị $^t v$ lên $\mathcal{M}(X; \mathbf{C})$ (theo nghĩa đại số); vì vậy tính liên tục của nó suy ra từ điều nói trên (TVS, IV, § 1, No. 3, Mệnh đề 6).

#### Hệ quả {#int-iii-s3-n4-cor-1 .statement}

— *Với các giả thiết và ký hiệu như trong Mệnh đề 9, hạn chế của ánh xạ* $\mu \mapsto \int f\, d\mu$ *trên tập* $\mathcal{M}_+(X)$ *các độ đo dương, hoặc trên một tập con B bị chặn mơ hồ của* $\mathcal{M}(X; \mathbf{C})$, *là liên tục mơ hồ.*

Thật vậy, từ § 1, No. 10, Mệnh đề 17 và 18 suy ra rằng, trên $\mathcal{M}_+(X)$ hoặc trên $B$, tôpô cảm sinh bởi tôpô hội tụ chặt-compact cũng chính là tôpô cảm sinh bởi tôpô mơ hồ.

Tuy nhiên, ánh xạ $\mu \mapsto \int f\, d\mu$ không nhất thiết liên tục trên toàn bộ $\mathcal{M}(X; \mathbf{C})$ đối với tôpô mơ hồ (Bài tập 2).

### Bài tập {#int-iii-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).
