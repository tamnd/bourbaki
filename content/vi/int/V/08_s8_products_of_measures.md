---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 8
section_title: Products of measures
lang: vi
source: int-i-vi
book_pages: INT V.114-INT V.122
pdf_pages: 0334-0349, 0369-0377
extraction: ocr
subsections:
    - "no": 1
      title: Interpretation of the product measure as an integral of measures
      page: 79
      pdf_page: 334
    - "no": 2
      title: Functions measurable with respect to a product of two measures
      page: 81
      pdf_page: 336
    - "no": 3
      title: Integration of positive functions
      page: 83
      pdf_page: 338
    - "no": 4
      title: Integration of functions with values in a Banach space
      page: 87
      pdf_page: 342
    - "no": 5
      title: Operations on the product of two measures
      page: 89
      pdf_page: 344
    - "no": 6
      title: Integration with respect to a finite product of measures
      page: 91
      pdf_page: 346
    - "no": 7
      title: 'Application: Measure of the Euclidean ball in $\mathbf{R}^n$'
      page: 93
      pdf_page: 348
statements: 31
exercises: 21
content_sha256: bf5c4f5835cc811a56d68f620f1cfe79e97df7ca016b57f9c715b449d9c4ee4e
translated_from: content/en/int/V/08_s8_products_of_measures.md
source_content_sha256: f32ac9b0595976df24efb98f8ebc133115fe2afd869695655c5382ac45e70518
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-646eb530
glossary_version: 34
glossary_terms_sha256: f96ed2ceef8e2640566befcf15e4c6631969ce5c2cbb0775578569347d8e2860
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. TÍCH CỦA CÁC ĐỘ ĐO

### 1. Giải thích độ đo tích như một tích phân các độ đo

Trong suốt tiết này, T và T' ký hiệu hai không gian địa phương compact, $\mu$ là một độ đo dương trên T, $\mu'$ là một độ đo dương trên T', và $\nu = \mu \otimes \mu'$ là độ đo tích trên $X = T \times T'$ (Ch. III, §4, No. 1).

Với mọi $t \in T$, ánh xạ $t' \mapsto (t, t')$ từ T' vào X là liên tục và thực sự. Gọi $\lambda'_t$ là ảnh của $\mu'$ qua ánh xạ này; $\lambda'_t$ là một độ đo dương trên X, và nếu $f \in \mathcal{K}(X)$ thì, ký hiệu bởi $f_t$ ánh xạ riêng phần $t' \mapsto f(t, t')$, ta có

$$
\int f \, d\lambda'_t = \int f_t \, d\mu',
$$

điều này cũng được biểu diễn bởi quan hệ $\lambda'_t = \varepsilon_t \otimes \mu'$.

Hơn nữa, ánh xạ $t \mapsto \lambda'_t(f)$ là liên tục, có giá compact (Ch. III, §4, No. 1, Bổ đề 2), do đó ánh xạ $t \mapsto \lambda'_t$ từ T vào $\mathcal{M}(X)$ là liên tục mờ (và, *a fortiori*, $\mu$-đo được mờ); do đó, họ các độ đo $t \mapsto \lambda'_t$ là $\mu$-thích hợp ($\S 3$, No. 1, Mệnh đề 2a)). Tích phân của $f$ đối với độ đo $\int \lambda'_t \, d\mu(t)$ theo định nghĩa là

$$
\int \langle f, \lambda'_t \rangle \, d\mu(t) = \int d\mu(t) \int f_t(t') \, d\mu'(t') = \int f(t, t') \, d\nu(t, t')
$$

(Ch. III, §4, No. 1, Định lý 2); do đó $\nu = \int \lambda'_t \, d\mu(t)$.

Tương tự, với mọi phần tử $t' \in T'$, gọi $\lambda_{t'}$ là ảnh của $\mu$ qua ánh xạ $t \mapsto (t, t')$ từ T vào X. Ánh xạ $t' \mapsto \lambda_{t'}$ là $\mu'$-thích hợp và liên tục mờ, và $\nu = \int \lambda_{t'} \, d\mu'(t')$. Ta sẽ cần các bổ đề sau:

#### Bổ đề 1 {#int-v-s8-lem-1 .statement}

*Với mọi hàm số $f \geqslant 0$ xác định trên X,*

$$
\int^* f_t \, d\mu' = \int^* f \, d\lambda'_t.
$$

Vì $t' \mapsto (t, t')$ là một ánh xạ liên tục và thực sự, điều này suy ra từ Mệnh đề 2 của §4, No. 2.

#### Bổ đề 2 {#int-v-s8-lem-2 .statement}

Cho $f$ là một ánh xạ từ $X$ vào một không gian tôpô. Để $f$ là $\lambda'_t$-đo được, điều kiện cần và đủ là $f_t$ là $\mu'$-đo được.
Đây là một hệ quả của Mệnh đề 3 của §6, No. 2.

#### Bổ đề 3 {#int-v-s8-lem-3 .statement}

Cho $f$ là một hàm xác định trên $X$, nhận giá trị trong $\overline{\mathbf{R}}$ hoặc trong một không gian Banach. Để $f$ là $\lambda'_t$-khả tích, điều kiện cần và đủ là $f_t$ là $\mu'$-khả tích, và khi đó

$$
\int f_t \, d\mu' = \int f \, d\lambda'_t .
$$

Điều này suy ra từ Định lý 2 của §4, No. 4, khi xét đến việc $t' \mapsto (t, t')$ là liên tục và thực sự.

#### Nhận xét {#int-v-s8-n1-rem-1 .statement}

Bổ đề 1,2,3 có thể được chứng minh rất đơn giản mà không cần dùng đến các kết quả của §§4 và 6, bằng một lập luận trực tiếp. Chẳng hạn, quan hệ (2) là hiển nhiên theo định nghĩa nếu $f \in \mathcal{K}(T \times T')$. Nếu $f$ là nửa liên tục dưới trên $X = T \times T'$, chỉ cần nhận xét rằng $t' \mapsto f_t(t')$ là bao trên của các hàm $t' \mapsto g_t(t') = g(t, t')$, trong đó $g$ chạy qua tập hợp các hàm thuộc $\mathcal{K}(X)$ sao cho $0 \leq g \leq f$. Cuối cùng, với $f$ tùy ý, ta nhận thấy rằng nếu $h \geq f$ là nửa liên tục dưới trên $X$, thì $t' \mapsto h(t, t')$ là nửa liên tục dưới trên $T'$; và ngược lại, nếu $t' \mapsto u(t')$ là nửa liên tục dưới trên $T'$ và sao cho $u(t') \geq f(t, t')$ với mọi $t' \in T'$, thì hàm $h$ sao cho $h(t, t') = u(t')$, $h(t_1, t') = +\infty$ với $t_1 \neq t'$, là nửa liên tục dưới trên $X$ và thỏa mãn $h \geq f$. Một khi Bổ đề 1 được chứng minh, từ đó suy ra rằng tập hợp $(T - \{t\}) \times T'$ là $\lambda'_t$-không đáng kể, và khi đó rất dễ chứng minh các Bổ đề 2 và 3.

Quan hệ (3) cho phép ký hiệu hai vế của nó bằng $\int f(t, t') \, d\mu'(t')$ mà không có nguy cơ nhầm lẫn. Các kết quả tương tự hiển nhiên đúng đối với các độ đo $\lambda_{t'} = \mu \otimes \varepsilon_{t'}$.

Thay vì các ký hiệu

$$
\int^* f(t, t') \, d\nu(t, t'), \quad \int^\bullet f(t, t') \, d\nu(t, t'), \quad \int f(t, t') \, d\nu(t, t'),
$$

ta sẽ dùng các ký hiệu

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t'), \quad \iint^\bullet f(t, t') \, d\mu(t) \, d\mu'(t'), \quad \iint f(t, t') \, d\mu(t) \, d\mu'(t'),
$$

phù hợp với các ký hiệu đã được chấp nhận trong Ch. III, §4, No. 1.

Cách hiểu độ đo $\nu$ như một tích phân $\int \lambda'_t \, d\mu(t)$ sẽ cho phép chúng ta chuyển các kết quả của §3 sang ngôn ngữ của các độ đo tích. Mặt khác, độ đo $\lambda'_t$ được mang bởi $\{t\} \times T' = \overline{\mathrm{pr}}_1^{-1}(t)$, do đó tích phân này xác định một phân tích của $\nu$ thành các lát, liên quan đến phép chiếu $\mathrm{pr}_1$ của $T \times T'$ lên $T$ (§6, No. 6). Trước khi đưa ra danh sách các kết quả thu được như vậy, đây là một tính chất hữu ích:

#### Mệnh đề 1 {#int-v-s8-prop-1 .statement}

— Cho $(\mu_\alpha)_{\alpha \in A}$ (tương ứng $(\mu'_\beta)_{\beta \in B}$) là một họ các độ đo dương tổng được trên T (tương ứng trên T'), với tổng được ký hiệu bởi $\mu$ (tương ứng bởi $\mu'$). Khi đó họ $(\mu_\alpha \otimes \mu'_\beta)_{(\alpha, \beta) \in A \times B}$ là tổng được trên $T \times T'$, và

$$
\mu \times \mu' = \sum_{(\alpha, \beta) \in A \times B} \mu_\alpha \otimes \mu'_\beta.
$$

Các tính chất này là hiển nhiên khi A và B là hữu hạn. Suy ra rằng nếu $A'$ (tương ứng $B'$) là một tập con hữu hạn của A (tương ứng của B), thì

$$
\sum_{(\alpha, \beta) \in A' \times B'} \mu_\alpha \otimes \mu'_\beta \leq \mu \otimes \mu'.
$$

Do đó họ $(\mu_\alpha \otimes \mu'_\beta)$ là tổng được. Để chỉ ra rằng hai vế của (4) bằng nhau, chỉ cần chứng minh rằng vế thứ hai thỏa mãn tính chất đặc trưng của các độ đo tích (Ch. III, §4, No. 1, Định lý 1), điều này được chỉ ra bởi phép tính sau.

Cho $f$ là một phần tử của $\mathcal{K}_+(T)$, $f'$ là một phần tử của $\mathcal{K}_+(T')$; nhắc lại rằng $f \otimes f'$ ký hiệu hàm $(t, t') \mapsto f(t)f'(t')$ trên $T \times T'$, thuộc $\mathcal{K}_+(T \times T')$ (A, II, §7, No. 7). Khi đó, theo định nghĩa của các độ đo tích,

$$
\sum_{(\alpha, \beta) \in A \times B} \langle \mu_\alpha \otimes \mu'_\beta, f \otimes f' \rangle = \sum_{(\alpha, \beta) \in A \times B} (\langle \mu_\alpha, f \rangle \langle \mu'_\beta, f' \rangle)
= \left( \sum_{\alpha \in A} \langle \mu_\alpha, f \rangle \right) \left( \sum_{\beta \in B} \langle \mu'_\beta, f' \rangle \right)
= \langle \mu, f \rangle \langle \mu', f' \rangle
= \langle \mu \otimes \mu', f \otimes f' \rangle.
$$

### 2. Các hàm đo được đối với một tích của hai độ đo

#### Mệnh đề 2 {#int-v-s8-prop-2 .statement}

— Cho $f$ là một hàm $\nu$-đo được xác định trên $T \times T'$, với các giá trị trong một không gian tôpô G, và cho M là tập hợp các $t \in T$ sao cho ánh xạ $t' \mapsto f(t, t')$ không $\mu'$-đo được.

a) Nếu $f$ là hằng trên phần bù của một tập con $\nu$-được điều hòa của $T \times T'$, thì M là $\mu$-không đáng kể.

b) Nếu $\mu'$ được điều hòa, thì M là $\mu$-không đáng kể.

Mệnh đề a) suy ra từ Mệnh đề 4b) của §3, No. 2 và các nhận xét của No. 1. Để xử lý b), chú ý rằng $\mu'$ là tổng của một dãy $\mu'_n$ các độ đo bị chặn (§2, No. 3, Mệnh đề 4); $f$ là đo được đối với $\mu \otimes \mu'_n \leq \nu$, và tập hợp $M$ là hợp của các tập hợp $M_n$ liên kết với các độ đo $\mu'_n$ (\S 2, No. 2, Mệnh đề 2). Do đó ta quy về trường hợp $\mu'$ bị chặn, điều này suy ra từ Mệnh đề 4c) của \S 3, No. 2.

Mệnh đề này mở rộng ngay lập tức đến các độ đo phức (Ch. III, \S 4, No. 2, Mệnh đề 3).

#### Hệ quả {#int-v-s8-n2-cor-1 .statement}

— *Cho A là một tập con $\nu$-đo được của $T \times T'$, và cho M là tập hợp các $t \in T$ sao cho tiết diện $A(t)$ của A tại t không $\mu'$-đo được.*

a) *Nếu A là $\nu$-được điều hòa, thì M là $\mu$-không đáng kể.*

b) *Nếu phép chiếu của A trên $T'$ là $\mu'$-được điều hòa, thì M là $\mu$-không đáng kể địa phương.*

Mệnh đề a) suy ra ngay lập tức từ Mệnh đề 2. Để chứng minh b), ký hiệu B là một tập hợp, hợp của một dãy các tập mở $\mu'$-tích phân được trong $T'$, chứa phép chiếu của A trên $T'$, và ký hiệu $\mu'_1$ là độ đo được điều hòa $\varphi_B \cdot \mu'$; vì A là đo được đối với $\mu \otimes \mu'_1 \leq \mu \otimes \mu'$, Mệnh đề 2 suy ra rằng $A(t)$ là $\mu'_1$-đo được, ngoại trừ các $t$ tạo thành một tập hợp $\mu$-không đáng kể địa phương. Nhưng vì $A(t) \subset B$, việc nói rằng $A(t)$ là $\mu'_1$-đo được tương đương với việc nói rằng $A(t)$ là $\mu'$-đo được (\S 5, No. 3, Hệ quả của Mệnh đề 4).

#### Mệnh đề 3 {#int-v-s8-prop-3 .statement}

— *Cho f là một ánh xạ từ T vào một không gian tôpô F. Nếu f là $\mu$-đo được, thì ánh xạ $(t, t') \mapsto f(t)$ là $\nu$-đo được. Ngược lại, nếu $\mu' \neq 0$, và nếu ánh xạ này là $\nu$-đo được, thì hàm f là $\mu$-đo được.*

Mệnh đề đầu tiên suy ra từ Hệ quả 1 của Mệnh đề 10 của \S 6, No. 6. Giả sử rằng $\mu' \neq 0$, ký hiệu $\mu'_1$ là một độ đo khác không có giá compact bị chặn trên bởi $\mu'$, ký hiệu $\nu_1$ là độ đo $\mu \otimes \mu'_1$, và đặt $a = \| \mu'_1 \|$. Khi đó phép chiếu $\mathrm{pr}_1$ của $T \times T'$ lên T là $\nu_1$-thực sự, và độ đo ảnh $\mathrm{pr}_1(\nu_1)$ bằng $a \mu$ (\S 6, No. 6, Mệnh đề 10). Nếu $(t, t') \mapsto f(t)$ là $\nu$-đo được, thì nó cũng $\nu_1$-đo được, do đó $f$ đo được đối với độ đo $a \mu$ (\S 6, No. 2, Mệnh đề 3), do đó có kết quả vì $a \neq 0$.

Mệnh đề trên mở rộng ngay lập tức sang các độ đo phức (Ch. III, \S 4, No. 2, Mệnh đề 3), cũng như các hệ quả sau đây.

#### Hệ quả 1 {#int-v-s8-prop-3-cor-1 .statement}

— *Cho F, F' và G là ba không gian tôpô, và cho u là một ánh xạ liên tục từ $F \times F'$ vào G. Cho f (resp. $f'$) là một hàm xác định trên T (resp. $T'$), nhận giá trị trong F (resp. $F'$) và đo được đối với $\mu$ (resp. $\mu'$). Khi đó hàm $(t, t') \mapsto u(f(t), f'(t'))$ đo được đối với $\mu \otimes \mu'$.*

Các ánh xạ $(t, t') \mapsto f(t)$, $(t, t') \mapsto f'(t')$ là $\nu$-đo được theo Mệnh đề 3, nên điều này suy ra từ Định lý 1 của Ch. IV, \S 5, No. 3.

#### Hệ quả 2 {#int-v-s8-prop-3-cor-2 .statement}

— *Nếu $A \subset T$ và $A' \subset T'$ là đo được (lần lượt đối với $\mu$ và $\mu'$), thì $A \times A'$ đo được đối với $\mu \otimes \mu'$.*
Điều này suy ra ngay lập tức từ Hệ quả 1.

#### Hệ quả 3 {#int-v-s8-prop-3-cor-3 .statement}

— *Xét hai hàm số dương (resp. nhận giá trị phức) $f$ xác định trên $T$ và $f'$ xác định trên $T'$. Nếu các hàm này lần lượt đo được đối với $\mu$ và $\mu'$, thì hàm*

$$
f \otimes f' : (t, t') \mapsto f(t)f'(t')
$$

*đo được đối với $\mu \otimes \mu'$.*

Trường hợp các hàm phức, hoặc các hàm thực hữu hạn, là một hệ quả ngay lập tức của Hệ quả 1. Để xét trường hợp các hàm số dương, với mỗi số nguyên $n \geqslant 0$ ta đặt $f_n = \inf(f, n)$, $f'_n = \inf(f', n)$, và ta có (với quy ước thông thường $0 \cdot (+\infty) = 0$) $f \otimes f' = \sup_n (f_n \otimes f'_n)$, do đó có kết quả.

#### Mệnh đề 4 {#int-v-s8-prop-4 .statement}

— *Cho $A$ là một tập con của $T$. Nếu $A$ là địa phương $\mu$-không đáng kể, thì $A \times T'$ là địa phương $\nu$-không đáng kể. Ngược lại, nếu $A \times T'$ là địa phương $\nu$-không đáng kể và nếu $\mu' \neq 0$, thì $A$ là địa phương $\mu$-không đáng kể.*

Mệnh đề đầu tiên suy ra từ Hệ quả 1 của Mệnh đề 10 của §6, No. 6. Để thiết lập mệnh đề thứ hai, ta lấy lại các ký hiệu trong chứng minh của Mệnh đề 3; $A \times T' = \mathrm{pr}_1^{-1}(A)$ là địa phương không đáng kể đối với độ đo $\nu_1$, do đó $A$ là địa phương không đáng kể đối với $a\mu$ (\S6, No. 2, Hệ quả của Mệnh đề 2), do đó có kết quả vì $a \neq 0$.

Mệnh đề trên lập tức mở rộng đến tích của hai độ đo phức (Ch. III, §4, No. 2, Mệnh đề 3), cũng như hệ quả sau đây.

#### Hệ quả {#int-v-s8-n2-cor-2 .statement}

— *Nếu độ đo $\mu$ (resp. $\mu'$) tập trung trên $M$ (resp. $M'$), thì $\mu \otimes \mu'$ tập trung trên $M \times M'$.*

Thật vậy, $(T \times T') - (M \times M')$ là hợp của các tập hợp $(T - M) \times T'$ và $T \times (T' - M')$, là các tập hợp địa phương không đáng kể đối với $\mu \times \mu'$ theo Mệnh đề 4.

### 3. Tích phân các hàm dương

Nhắc lại rằng ta đã quy ước định nghĩa tích $0 \cdot (+\infty)$ bằng 0. Quy ước này đặc biệt dẫn đến hệ quả sau: nếu $f$ là một hàm số $\geqslant 0$ được xác định trên một không gian địa phương compact được trang bị một độ đo dương $\lambda$, thì $\lambda^*(af) = a \cdot \lambda^*(f)$ với mọi hằng $a$ sao cho $0 \leqslant a \leqslant +\infty$. Điều này hiển nhiên nếu $a = 0$; nếu $a = +\infty$, thì $\lambda^*(af) = a \cdot \lambda^*(f) = 0$ hoặc $\lambda^*(af) = a \cdot \lambda^*(f) = +\infty$ tùy theo $f$ là $\lambda$-không đáng kể hay không; cuối cùng, nếu $0 < a < +\infty$, ta biết rằng $\lambda^*(af) = a \cdot \lambda^*(f)$.

#### Mệnh đề 5 {#int-v-s8-prop-5 .statement}

— Cho $f$ là một hàm số $\geqslant 0$, nửa liên tục dưới trên $T \times T'$. Khi đó, hàm

$$
t \mapsto \int^* f(t, t') \, d\mu'(t')
$$

là nửa liên tục dưới trên $T$, và

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') \, d\mu'(t').
$$

Đây là một hệ quả của Mệnh đề 2 của §3, No. 1, có tính đến Bổ đề 1 của No. 1.

#### Hệ quả 1 {#int-v-s8-prop-5-cor-1 .statement}

— Cho $f$ (resp. $f'$) là một hàm nửa liên tục dưới $\geqslant 0$ được xác định trên $T$ (resp. $T'$); hàm $f \otimes f' : (t, t') \mapsto f(t)f'(t')$ khi đó là nửa liên tục dưới trên $T \times T'$, và

$$
\iint^* f(t)f'(t') \, d\mu(t) \, d\mu'(t') = \left( \int^* f(t) \, d\mu(t) \right) \left( \int^* f'(t') \, d\mu'(t') \right).
$$

Cho $G$ (resp. $G'$) là tập hợp các hàm $g \in \mathcal{K}_+(T)$ (resp. $g' \in \mathcal{K}_+(T')$) sao cho $g \leqslant f$ (resp. $g' \leqslant f'$); khi đó

$$
f \otimes f' = \sup_{g \in G,\ g' \in G'} g \otimes g'.
$$

Vì các hàm $g \otimes g'$ thuộc $\mathcal{K}_+(T \times T')$, nên $f \otimes f'$ thực sự là nửa liên tục dưới, và (6) suy ra ngay từ Mệnh đề 5 (hoặc trực tiếp bằng cách lấy giới hạn trong công thức trước đó).

#### Hệ quả 2 {#int-v-s8-prop-5-cor-2 .statement}

— Cho $A$ là một tập con $\mu$-vừa phải của $T$, và $A'$ là một tập con $\mu'$-vừa phải của $T'$; khi đó $A \times A'$ là $\nu$-vừa phải trong $T \times T'$.

Theo định nghĩa của tập vừa phải (§1, No. 2, Mệnh đề 5), chỉ cần chứng minh rằng nếu $B$ là một tập mở khả tích trong $T$, và $B'$ là một tập mở khả tích trong $T'$, thì tập mở $B \times B'$ là khả tích. Điều này suy ra ngay từ Hệ quả 1.

#### Hệ quả 3 {#int-v-s8-prop-5-cor-3 .statement}

— Cho $A$ là một tập con $\mu$-không đáng kể của $T$, và cho $B'$ là một tập con $\mu'$-vừa phải của $T'$; khi đó $A \times B'$ là $\nu$-không đáng kể.

Thật vậy, $A \times B'$ là $\nu$-không đáng kể địa phương (Mệnh đề 4) và $\nu$-vừa phải (Hệ quả 2), do đó nó là $\nu$-không đáng kể (§1, No. 2, Hệ quả 1 của Mệnh đề 7).

Hệ quả 2 và 3 có thể được mở rộng cho tích của hai độ đo phức, bằng cách áp dụng mệnh đề đó cho các biến phân toàn phần của chúng (Chương III, §4, No. 2, Mệnh đề 3).

#### Mệnh đề 6 {#int-v-s8-prop-6 .statement}

— Cho $f$ là một hàm số $\geqslant 0$ xác định trên $T \times T'$. Khi đó

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') \geqslant \int^* d\mu(t) \int^* f(t, t') d\mu'(t').
$$

Điều này suy ra từ Mệnh đề 3 của §3, No. 2, có lưu ý đến (2).

#### Mệnh đề 7 {#int-v-s8-prop-7 .statement}

— Cho $f$ là một hàm số dương $\nu$-đo được xác định trên $T \times T'$.

a) *Nếu $f$ là $\nu$-vừa phải, thì các hàm* $t \mapsto \int^* f(t, t') d\mu'(t')$, $t' \mapsto \int^* f(t, t') d\mu(t)$ *là đo được và vừa phải đối với $\mu$ và $\mu'$, tương ứng, và*

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'(t')
$$
(7)
$$
= \int^* d\mu'(t') \int^* f(t, t') d\mu(t).
$$

b) *Nếu độ đo $\mu'$ là vừa phải, thì hàm* $t \mapsto \int^* f(t, t') d\mu'(t')$ *là $\mu$-đo được, và*

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'(t').
$$
(8)

Mệnh đề a), cũng như mệnh đề b) khi $\mu'$ bị chặn, là những hệ quả của Mệnh đề 5 của §3, No. 2. Để xét trường hợp $\mu'$ vừa phải, ta biểu diễn $\mu'$ thành một tổng $\sum_{n \in \mathbf{N}} \mu'_n$ của một dãy các độ đo bị chặn (\S2, No. 3, Mệnh đề 4). Khi đó hàm $t \mapsto \int^* f(t, t') d\mu'_n(t')$ là $\mu$-đo được, và
$$
\iint^* f(t, t') d\mu(t) d\mu'_n(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'_n(t').
$$
Nhưng $\mu \otimes \mu' = \sum_{n \in \mathbf{N}} (\mu \otimes \mu'_n)$ (Mệnh đề 1); khi đó mệnh đề b) thu được bằng cách lấy tổng theo $n$ (\S2, No. 2, Mệnh đề 1).

#### Hệ quả 1 {#int-v-s8-prop-7-cor-1 .statement}

— Cho $H$ là một tập con của $T \times T'$, và cho $A$ là tập hợp các $t \in T$ sao cho tiết diện $H(t)$ của $H$ tại $t$ không $\mu'$-không đáng kể.

a) *Nếu $H$ là $\nu$-không đáng kể thì $A$ là $\mu$-không đáng kể.*

b) *Nếu $H$ là địa phương $\nu$-không đáng kể và $\mu'$ là điều hòa, thì $A$ là địa phương $\mu$-không đáng kể.*

Tính chất a) suy ra ngay lập tức từ Mệnh đề 7 (hoặc từ Mệnh đề 6). Dưới các giả thiết của b), nói rằng $H(t)$ là địa phương μ′-không đáng kể cũng như nói rằng nó là μ′-không đáng kể là tương đương, vì μ′ là điều hòa (§1, No. 2, Mệnh đề 7). Do đó tính chất b) suy ra từ công thức (8).

Hệ quả này suy ra ngay lập tức, bằng cách chuyển sang các giá trị tuyệt đối, cho tích của hai độ đo phức. Điều tương tự cũng đúng đối với hệ quả sau:

#### Hệ quả 2 {#int-v-s8-prop-7-cor-2 .statement}

— *Nếu một tập hợp* $A \subset T \times T'$ *là ν-khả tích, thì tiết diện* $A(t)$ *của* $A$ *tại* $t$ *là μ′-khả tích với hầu khắp mọi* $t \in T$, *hàm* $t \mapsto \mu'(A(t))$ *là μ-khả tích, và*

$$
\nu(A) = \int \mu'(A(t))\, d\mu(t).
$$

#### Mệnh đề 8 {#int-v-s8-prop-8 .statement}

— *Với mỗi cặp hàm số* $f \geq 0$, $f' \geq 0$ *xác định lần lượt trên* $T$ *và* $T'$, *ta có*

$$
\iint^\bullet f(t)f'(t')\, d\mu(t)\, d\mu'(t') = \left( \int^\bullet f(t)\, d\mu(t) \right) \left( \int^\bullet f'(t')\, d\mu'(t') \right).
$$

Ta bắt đầu bằng cách xét trường hợp $\mu$ và $\mu'$ là các độ đo *có giá compact*; khi đó $\mu \otimes \mu'$ cũng có tính chất này, và tất cả các ký hiệu $\int^\bullet$, $\iint^\bullet$ có thể được thay bằng các tích phân trên. Theo Mệnh đề 6,

$$
\iint^* f(t)f'(t')\, d\mu(t)\, d\mu'(t') \geq \int^* d\mu(t) \int^* f(t)f'(t')\, d\mu'(t')
$$
$$
= \left( \int^* f(t)\, d\mu(t) \right) \left( \int^* f'(t')\, d\mu'(t') \right).
$$

Để thiết lập bất đẳng thức ngược lại, ta chọn một hàm $h \geq f$ (resp. $h' \geq f'$), là bao dưới của một dãy $(h_n)$ (resp. $(h'_n)$) các hàm nửa liên tục dưới, sao cho

$$
\int^* h(t)\, d\mu(t) = \int^* f(t)\, d\mu(t)
$$

(resp. $\int^* h'(t')\, d\mu'(t') = \int^* f'(t')\, d\mu'(t')$); sự tồn tại của các hàm như vậy suy ra ngay lập tức từ định nghĩa tích phân trên (Ch. IV, §1, No. 3, Def. 3) và định lý Lebesgue. Áp dụng Mệnh đề 7 cho hàm đo được $h \otimes h'$, ta có

$$
\iint^* f(t)f'(t')\, d\mu(t)\, d\mu'(t') \leq \iint^* h(t)h'(t')\, d\mu(t)\, d\mu'(t')
$$
$$
= \left( \int^* h(t)\, d\mu(t) \right) \left( \int^* h'(t')\, d\mu'(t') \right)
$$
$$
= \left( \int^* f(t)\, d\mu(t) \right) \left( \int^* f'(t')\, d\mu'(t') \right),
$$

đó chính là bất đẳng thức cần tìm. Do đó mệnh đề được chứng minh khi $\mu$ và $\mu'$ là các độ đo có giá compact. Để xét trường hợp tổng quát, chỉ cần biểu diễn $\mu$ (resp. $\mu'$) dưới dạng tổng của một họ $(\mu_\alpha)_{\alpha \in A}$ (resp. $(\mu'_\beta)_{\beta \in B}$) các độ đo có giá compact (\S 2, No. 3, Mệnh đề 4), viết công thức (10) cho mỗi độ đo $\mu_\alpha \otimes \mu'_\beta$, rồi lấy tổng theo $(\alpha, \beta)$, có tính đến Mệnh đề 1 (\S 2, No. 2, Mệnh đề 1).

#### Hệ quả 1 {#int-v-s8-prop-8-cor-1 .statement}

*Với các ký hiệu như trong Mệnh đề 8,*

$$
\iint^* f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int^* f(t)\,d\mu(t) \right) \left( \int^* f'(t')\,d\mu'(t') \right)
$$

*trừ trường hợp có thể xảy ra khi một trong các thừa số của vế thứ hai bằng 0 và thừa số kia bằng $+\infty$.*

Khi hai thừa số của vế thứ hai là hữu hạn, các hàm $f$ và $f'$ là vừa phải (\S 1, No. 2, Prop. 7), do đó hàm $f \otimes f'$ là vừa phải (Cor. 2 of Prop. 5); vì thế đẳng thức trên quy về công thức (10) (\S 1, No. 2, Prop. 7). Khi một trong các thừa số của vế thứ hai có giá trị $+\infty$ và thừa số kia khác không, thì vế thứ hai có giá trị $+\infty$, và đẳng thức trên suy ra từ Prop. 6.

#### Hệ quả 2 {#int-v-s8-prop-8-cor-2 .statement}

*Cho $f$ và $f'$ là hai hàm nhận giá trị trong $\mathbf{C}$ hoặc trong $\overline{\mathbf{R}}$, được xác định tương ứng trên $T$ và $T'$, và khả tích cốt yếu (tương ứng, khả tích) đối với các độ đo $\mu$ và $\mu'$, tương ứng. Khi đó hàm $f \otimes f'$ là khả tích cốt yếu (tương ứng, khả tích) đối với độ đo $\mu \otimes \mu'$, và*

$$
\iint f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int f(t)\,d\mu(t) \right) \left( \int f'(t')\,d\mu'(t') \right).
$$

Khi $f$ và $f'$ dương, $f \otimes f'$ là đo được theo Cor. 3 of Prop. 3, và mệnh đề suy ra từ công thức (10) (tương ứng, (11)) và tiêu chuẩn khả tích cốt yếu (\S 1, No. 3, Prop. 9) (tương ứng, tiêu chuẩn khả tích của Ch. IV, \S 5, No. 6, Th. 5). Trường hợp tổng quát khi đó suy ra ngay lập tức.

Hệ quả 2 mở rộng ngay cho tích của hai độ đo phức.

### 4. Tích phân các hàm nhận giá trị trong một không gian Banach

#### Định lý 1 (Lebesgue–Fubini) {#int-v-s8-thm-1 .statement}

— *Cho $f$ là một hàm được xác định trên $T \times T'$, nhận giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$; gọi $N$ là tập hợp các $t \in T$ sao cho hàm $t' \mapsto f(t,t')$ không $\mu'$-khả tích.

a) Giả sử rằng $f$ là $\nu$-khả tích; khi đó $N$ là $\mu$-không đáng kể, hàm $t \mapsto \int f(t,t')\,d\mu'(t')$ (được xác định với $t \notin N$) là $\mu$-khả tích, và*

$$
\iint f(t,t')\,d\mu(t)\,d\mu'(t') = \int d\mu(t) \int f(t,t')\,d\mu'(t').
$$

b) *Giả sử rằng $f$ là khả tích cốt yếu đối với $\nu$, và độ đo $\mu'$ là vừa phải; khi đó $N$ là địa phương $\mu$-không đáng kể, hàm $t \mapsto \int f(t, t')\, d\mu'(t')$ (được xác định với $t \notin N$) là khả tích cốt yếu đối với $\mu$, và (13) đúng.*

Mệnh đề a) suy ra ngay từ Th. 1 of §3, No. 3. Để thiết lập b), ký hiệu $g$ là một hàm $\nu$-khả tích bằng $f$ địa phương hầu khắp nơi, và $H$ là tập hợp các $(t, t')$ sao cho $f(t, t') \neq g(t, t')$. Theo Cor. 1 of Prop. 7, tiết diện $H(t)$ là $\mu'$-không đáng kể, trừ phi $t \in T$ thuộc một tập địa phương $\mu$-không đáng kể. Khi đó kết quả liên quan đến $f$ có thể suy ra từ mệnh đề a) áp dụng cho $g$.

#### Chú giải {#int-v-s8-n4-sch-1 .statement}

— *Cho $f$ là một hàm được xác định trên $T \times T'$, nhận giá trị trong $\overline{\mathbf{R}}$ hoặc trong một không gian Banach, là $\nu$-đo được và $\nu$-vừa phải. Đối với ba tích phân*

$$
\iint f(t, t')\, d\mu(t)\, d\mu'(t'), \quad \int d\mu(t) \int f(t, t')\, d\mu'(t'), \quad \int d\mu'(t') \int f(t, t')\, d\mu(t)
$$

*tồn tại và bằng nhau, điều kiện cần và đủ là một trong hai số*

$$
\int^* d\mu(t) \int^* |f(t, t')|\, d\mu'(t'), \quad \int^* d\mu'(t') \int^* |f(t, t')|\, d\mu(t)
$$

*là hữu hạn.*

Đây là một hệ quả ngay lập tức của Định lý 1, Mệnh đề 7 và tiêu chuẩn khả tích (Ch. IV, §5, No. 6, Định lý 5).

#### Nhận xét {#int-v-s8-n4-rem-1 .statement}

— 1) Khi độ đo $\mu'$ không ôn hòa, có thể xảy ra trường hợp $f$ là khả tích thiết yếu theo $\nu$ và hàm $t' \mapsto f(t, t')$ lại không khả tích thiết yếu theo $\mu'$ với bất kỳ giá trị nào của $t \in T$ (§3, Exer. 4).

2) Cho $\mu$ và $\mu'$ là hai độ đo phức, và đặt $\nu = \mu \otimes \mu'$. Nếu $f$ là khả tích theo $\nu$ (nói cách khác, khả tích theo $|\nu|$), thì áp dụng định lý cho các độ đo $|\mu|$ và $|\mu'|$, mà tích của chúng là $|\nu|$ (Ch. III, §4, No. 2, Mệnh đề 3), suy ra rằng $t' \mapsto f(t, t')$ là khả tích theo $\mu'$ với $\mu$-hầu khắp mọi $t$. Từ đó suy ra, bằng cách phân tích các độ đo $\mu$ và $\mu'$ thành một tổ hợp tuyến tính của các độ đo dương, rằng mệnh đề ở a) mở rộng được cho các độ đo phức. Ta cũng có thể lập luận tương tự cho b).

#### Mệnh đề 9 {#int-v-s8-prop-9 .statement}

*Cho $F$, $F'$ và $G$ là ba không gian Banach, và cho $(x, y) \mapsto [x \cdot y]$ là một ánh xạ song tuyến tính liên tục từ $F \times F'$ vào $G$. Cho $f$ (tương ứng $f'$) là một hàm xác định trên $T$ (tương ứng $T'$) nhận giá trị trong $F$ (tương ứng $F'$) và khả tích thiết yếu theo $\mu$ (tương ứng $\mu'$). Đặt $g$ là hàm $(t, t') \mapsto [f(t) \cdot f'(t')]$; khi đó $g$ khả tích thiết yếu theo $\mu \otimes \mu'$, và*

$$
\iint [f(t) \cdot f'(t')] \, d\mu(t)\, d\mu'(t') = \left[ \left( \int f\, d\mu(t) \right) \cdot \left( \int f'(t')\, d\mu'(t') \right) \right].
$$

*Nếu hơn nữa $f$ và $f'$ khả tích, thì $g$ khả tích.*

Hàm $(t, t') \mapsto [\mathbf{f}(t) \cdot \mathbf{f}'(t')]$ là $(\mu \otimes \mu')$-đo được theo Hệ quả 1 của Mệnh đề 3. Mặt khác, nếu $b$ ký hiệu chuẩn của ánh xạ song tuyến tính $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x} \cdot \mathbf{y}]$, thì

$$
\iint^\bullet |[\mathbf{f}(t) \cdot \mathbf{f}'(t')]| d\mu(t) d\mu'(t') \leq b \iint^\bullet |\mathbf{f}(t)| \cdot |\mathbf{f}'(t')| d\mu(t) d\mu'(t')
$$
$$
= b \left( \int^\bullet |\mathbf{f}(t)| d\mu(t) \right) \left( \int^\bullet |\mathbf{f}'(t')| d\mu'(t') \right)
$$

theo Mệnh đề 8. Điều này cho thấy rằng $[\mathbf{f}(t) \cdot \mathbf{f}'(t')]$ là khả tích thiết yếu đối với $\mu \otimes \mu'$ (\S 1, No. 3, Mệnh đề 9). Giả sử rằng $\mathbf{f}$ và $\mathbf{f}'$ khả tích: khi đó $\mathbf{f}$ và $\mathbf{f}'$ là điều hòa, và $\mathbf{g}$ là điều hòa (Hệ quả 2 của Mệnh đề 5), do đó khả tích (\S 1, No. 3, Hệ quả của Mệnh đề 9). Trong trường hợp này công thức (14) suy ra từ định lý Lebesgue–Fubini và tính tuyến tính của tích phân (Ch. IV, \S 4, No. 2, Định lý 1). Để hoàn tất việc xét trường hợp $\mathbf{f}$ và $\mathbf{f}'$ là khả tích thiết yếu, khi đó áp dụng (14) cho hai hàm khả tích $\mathbf{f}_1$ và $\mathbf{f}_1'$, bằng với $\mathbf{f}$ và $\mathbf{f}'$ hầu khắp nơi địa phương, khi nhận thấy rằng $[\mathbf{f} \cdot \mathbf{f}'] = [\mathbf{f}_1 \cdot \mathbf{f}_1']$ hầu khắp nơi địa phương trong $T \times T'$ (Mệnh đề 4).

Kết quả này mở rộng cho tích của các độ đo phức.

### 5. Các phép toán trên tích của hai độ đo

#### Mệnh đề 10 {#int-v-s8-prop-10 .statement}

— Cho $g$ (resp. $g'$) là một hàm phức (hoặc một hàm nhận giá trị trong $\overline{\mathbf{R}}$) xác định trên $T$ (resp. $T'$).
a) Nếu $g$ (resp. $g'$) khả tích địa phương đối với $\mu$ (resp. $\mu'$), thì hàm $g \otimes g': (t, t') \mapsto g(t)g'(t')$ khả tích địa phương đối với $\nu = \mu \otimes \mu'$, và

$$
(g \cdot \mu) \otimes (g' \cdot \mu') = (g \otimes g') \cdot (\mu \otimes \mu').
$$

b) Ngược lại, nếu $g \otimes g'$ khả tích địa phương theo $\nu$, và nếu $g'$ không $\mu'$-không đáng kể địa phương, thì $g$ khả tích địa phương theo $\mu$.

a) Cho $K$ và $K'$ là hai tập hợp compact của $T$ và $T'$, tương ứng; Hệ quả 2 của Mệnh đề 8 cho thấy rằng hàm $(t, t') \mapsto g(t)g'(t')\varphi_{K \times K'}(t, t')$, bằng với $(g\varphi_K) \otimes (g'\varphi_{K'})$, là $\nu$-khả tích. Do đó, $g \otimes g'$ là $\nu$-khả tích địa phương. Khi đó người ta kiểm tra ngay lập tức rằng vế thứ hai của (15) thỏa mãn tính chất đặc trưng của các độ đo tích (Ch. III, \S 4, No. 1, Định lý 1).

b) Bây giờ giả sử rằng $g \otimes g'$ là $\nu$-khả tích địa phương, và rằng $g'$ không $\mu'$-không đáng kể địa phương. Cho $\mu_1$ là một độ đo dương có giá compact sao cho $\mu_1 \leq \mu$; do $g \otimes g'$ là $(\mu_1 \otimes \mu')$-đo được, $t \mapsto g(t)g'(t')$ là $\mu_1$-đo được trừ ra một tập hợp các giá trị của $t'$ là $\mu'$-không đáng kể địa phương (Mệnh đề 2).

Vì $g'$ không bằng không địa phương $\mu'$-gần khắp nơi, từ đó ta suy ra rằng $g$ là $\mu_1$-đo được, rồi $\mu$-đo được bằng cách phân tích $\mu$ thành tổng của một họ các độ đo có giá compact (\S 2, No. 3, Prop. 4 và \S 2, No. 2, Prop. 2). Sau khi đã thiết lập điểm này, ta có thể rút gọn về trường hợp $g$ và $g'$ đều $\geqslant 0$, bằng cách thay $g$ và $g'$ lần lượt bởi các giá trị tuyệt đối của chúng nếu cần. Cho $K$ là một tập con compact bất kỳ của $T$, và cho $K'$ là một tập con compact của $T'$ sao cho $\int g' \varphi_{K'} d\mu' \neq 0$. Theo Prop. 8,

$$
\left( \int^\bullet g \varphi_K d\mu \right) \left( \int^\bullet g' \varphi_{K'} d\mu' \right) = \iiint^\bullet (g \otimes g') \varphi_{K \times K'} d\mu d\mu' < +\infty .
$$

Do đó nhân tử thứ nhất của vế thứ nhất là hữu hạn, và điều này hoàn tất chứng minh.

Mệnh đề này mở rộng sang các độ đo phức, nhờ Prop. 3 của Ch. III, \S 4, No. 2.

#### Mệnh đề 11 {#int-v-s8-prop-11 .statement}

*Cho $\pi$ (resp. $\pi'$) là một ánh xạ từ $T$ (resp. $T'$) vào một không gian compact địa phương $T_1$ (resp. $T'_1$).*

a) *Nếu $\pi$ (resp. $\pi'$) là $\mu$-thực sự (resp. $\mu'$-thực sự), thì ánh xạ $\pi \times \pi'$ là $(\mu \otimes \mu')$-thực sự và $(\pi \times \pi')(\mu \otimes \mu') = \pi(\mu) \otimes \pi'(\mu')$.*

b) *Ngược lại, nếu $\pi \times \pi'$ là $(\mu \otimes \mu')$-thực sự và $\mu' \neq 0$, thì $\pi$ là $\mu$-thực sự.*

a) Thật vậy, $\pi \times \pi'$ là $(\mu \times \mu')$-đo được theo Hệ quả 1 của Prop. 3 của No. 2. Mặt khác, nếu $K$ (resp. $K'$) là một tập con compact của $T_1$ (resp. $T'_1$), thì $\pi^{-1}(K)$ và ${\pi'}^{-1}(K')$ lần lượt khả tích thiết yếu đối với $\mu$ và $\mu'$, do đó $\pi^{-1}(K) \times {\pi'}^{-1}(K')$ khả tích thiết yếu đối với $\mu \otimes \mu'$ (Hệ quả 2 của Prop. 8). Điều này chứng minh rằng $\pi \times \pi'$ là $(\mu \times \mu')$-thực sự. Bây giờ đặt $\mu_1 = \pi(\mu)$, $\mu'_1 = \pi'(\mu')$, $\nu_1 = (\pi \times \pi')(\mu \otimes \mu')$; với $f \in \mathcal{K}(T_1)$ và $f' \in \mathcal{K}(T'_1)$, ta có

$$
\iint f(\pi(t)) f'(\pi'(t')) d\mu(t) d\mu'(t')
$$
$$
= \left( \int f(\pi(t)) d\mu(t) \right) \left( \int f'(\pi'(t')) d\mu'(t') \right)
$$

(Hệ quả 2 của Prop. 8), điều này chứng minh rằng $\nu_1 = \mu_1 \otimes \mu'_1$ (Ch. III, \S 4, No. 1, Th. 1).

b) Bây giờ giả sử rằng $\pi \times \pi'$ là $\mu \otimes \mu'$-thực sự và $\mu' \neq 0$. Gọi $\mu_1$ là một độ đo $\leq \mu$ có giá compact. Vì hàm $\pi \times \pi'$ đo được đối với $\mu_1 \otimes \mu'$, ánh xạ $t \mapsto (\pi(t), \pi'(t'))$ là $\mu$-đo được trừ ra đối với các $t'$ tạo thành một tập địa phương $\mu'$-không đáng kể (No. 2, Mệnh đề 2). Vì $\mu' \neq 0$, suy ra $\pi$ là $\mu_1$-đo được, và cuối cùng $\pi$ là $\mu$-đo được

(§2, No. 3, Mệnh đề 4 và §2, No. 2, Mệnh đề 2). Còn phải chứng minh rằng $\mu^\bullet(f \circ \pi) < +\infty$ với mọi hàm $f \in \mathcal{K}_+(\mathrm{T}_1)$. Nếu $\mu$ bằng không, tính chất này là hiển nhiên. Nếu $\mu$ khác không, thì $\mu \otimes \mu'$ cũng khác không, do đó $(\pi \times \pi')(\mu \otimes \mu') \neq 0$ (§6, No. 2, Hệ quả 1 của Mệnh đề 2). Theo Bổ đề 1 của Ch. III, §4, No. 1, tồn tại hai hàm $g \in \mathcal{K}_+(\mathrm{T}_1)$, $g' \in \mathcal{K}_+(\mathrm{T}'_1)$ sao cho

$$
\langle (\pi \times \pi')(\mu \otimes \mu'), g \otimes g' \rangle \neq 0.
$$

Biểu thức này bằng $\langle \mu \otimes \mu', (g \circ \pi) \otimes (g' \circ \pi') \rangle$ theo định nghĩa của độ đo ảnh, Mệnh đề 8 suy ra rằng ${\mu''}^\bullet(g' \circ \pi') \neq 0$. Khi đó ta có, theo Mệnh đề 8 và theo Mệnh đề 2 của §6, No. 2,

$$
\left( \int^\bullet (f \circ \pi) d\mu \right) \left( \int^\bullet (g' \circ \pi') d\mu' \right) = \iint^\bullet (f \circ \pi) \otimes (g' \circ \pi') d\mu d\mu'
$$
$$
= \iint^\bullet (f \otimes g') d((\pi \times \pi')(\mu \otimes \mu')) < +\infty.
$$

Vậy tích phân thứ nhất ở vế thứ nhất là hữu hạn, điều này hoàn tất chứng minh.

Kết quả này mở rộng ngay được cho tích của hai độ đo phức (áp dụng mệnh đề cho các trị tuyệt đối của chúng). Điều tương tự cũng đúng cho mệnh đề sau đây.

#### Mệnh đề 12 {#int-v-s8-prop-12 .statement}

— Cho X (tương ứng X') là một không gian con compact địa phương của T (tương ứng của T'). Khi đó độ đo cảm sinh $(\mu \otimes \mu')_{X \times X'}$ trên không gian con compact địa phương $X \times X'$ của $T \times T'$ bằng tích $\mu_X \otimes \mu'_{X'}$ của các độ đo cảm sinh trên X và X' bởi $\mu$ và $\mu'$, tương ứng.

Thật vậy, nếu $f \in \mathcal{K}(X)$ và $f' \in \mathcal{K}(X')$, thì

$$
\iint_{X \times X'} f(t)f'(t') d\mu(t) d\mu'(t') = \left( \int_X f(t) d\mu(t) \right) \left( \int_{X'} f'(t') d\mu'(t') \right)
$$

theo Hệ quả 2 của Mệnh đề 8, điều này chứng minh, theo định nghĩa của các độ đo cảm sinh (Ch. IV, §5, No. 7), rằng

$$
(\mu \otimes \mu')_{X \times X'} = \mu_X \otimes \mu'_{X'}
$$

(Ch. III, §4, No. 1, Định lý 1).

### 6. Tích phân đối với một tích hữu hạn các độ đo

Các kết quả trước có thể được mở rộng không khó khăn sang tích của một số hữu hạn độ đo. Chẳng hạn, cho $T_1, T_2, T_3$ là ba không gian compact địa phương, $\mu_i$ là một độ đo dương trên $T_i$ ($i = 1, 2, 3$), và gọi ν = μ₁ ⊗ μ₂ ⊗ μ₃ là độ đo tích trên T = T₁ × T₂ × T₃. Gọi f là một hàm ν-khả tích nhận giá trị trong $\overline{\mathbf{R}}$ hoặc trong một không gian Banach; một áp dụng thứ nhất của định lý Lebesgue–Fubini cho thấy rằng, trừ tại các điểm $(t₁, t₂) ∈ T₁ × T₂$ tạo thành một tập không đáng kể (đối với $μ₁ ⊗ μ₂$), hàm $t₃ ↦ f(t₁, t₂, t₃)$ là $μ₃$-khả tích, hàm

$$
(t₁, t₂) ↦ \int f(t₁, t₂, t₃) \, dμ₃(t₃),
$$

được xác định hầu khắp nơi trong $T₁ × T₂$, là $(μ₁ ⊗ μ₂)$-khả tích, và

$$
\iiint f(t₁, t₂, t₃) \, dν(t₁, t₂, t₃) = \iint dμ₁(t₁) \, dμ₂(t₂) \int f(t₁, t₂, t₃) \, dμ₃(t₃).
$$

Một áp dụng thứ hai của cùng định lý cho thấy rằng, với hầu hết mọi $t₁ ∈ T₁$, hàm $t₂ ↦ \int f(t₁, t₂, t₃) \, dμ₃(t₃)$ được xác định hầu khắp nơi trong $T₂$ và là $μ₂$-khả tích; hơn nữa, hàm

$$
t₁ ↦ \int dμ₂(t₂) \int f(t₁, t₂, t₃) \, dμ₃(t₃),
$$

được xác định hầu khắp nơi trong $T₁$, là $μ₁$-khả tích, và

$$
\iiint f(t₁, t₂, t₃) \, dν(t₁, t₂, t₃) = \int dμ₁(t₁) \int dμ₂(t₂) \int f(t₁, t₂, t₃) \, dμ₃(t₃).
$$

Ta chứng minh tương tự rằng, với hầu hết mọi $t₁ ∈ T₁$, hàm $(t₂, t₃) ↦ f(t₁, t₂, t₃)$ là $(μ₂ ⊗ μ₃)$-khả tích, rằng hàm

$$
t₁ ↦ \iint f(t₁, t₂, t₃) \, dμ₂(t₂) \, dμ₃(t₃),
$$

được xác định hầu khắp nơi, là $μ₁$-khả tích, và rằng

$$
\iiint f(t₁, t₂, t₃) \, dν(t₁, t₂, t₃) = \int dμ₁(t₁) \iint f(t₁, t₂, t₃) \, dμ₂(t₂) \, dμ₃(t₃).
$$

Chúng tôi để cho người đọc việc khái quát hóa theo cùng cách các kết quả khác đã được chứng minh ở trên cho tích của hai độ đo.

### 7. Ứng dụng: Độ đo của quả cầu Euclid trong $\mathbf{R}^n$

Cho $\mu$ là độ đo Lebesgue trên $\mathbf{R}$, và $\mu_n$ là độ đo Lebesgue trên $\mathbf{R}^n$, tích của $n$ thừa số đều bằng $\mu$. Ta sẽ tính độ đo $V_n = \mu_n(\mathbf{B}_n)$ của quả cầu đơn vị Euclid. Theo Hệ quả 2 của Mệnh đề 7,

$$
V_n = \int_{-1}^{+1} \mu_{n-1}(\mathbf{B}_n(z_n)) dz_n .
$$

Bây giờ, tiết diện $\mathbf{B}_n(z_n)$ là tập con của $\mathbf{R}^{n-1}$ được xác định bởi quan hệ $\sum_{i=1}^{n-1} z_i^2 \leq 1 - z_n^2$, nói cách khác, nó là biến đổi của quả cầu $\mathbf{B}_{n-1}$ bởi phép vị tự với tỷ số $\sqrt{1 - z_n^2}$. Nhưng từ Mệnh đề 11 và công thức

$$
\alpha \int_{-\infty}^{+\infty} f(\alpha x) dx = \int_{-\infty}^{+\infty} f(z) dz
$$

với $f \in \mathcal{K}(\mathbf{R})$, suy ra ngay lập tức rằng ảnh của $\mu_{n-1}$ dưới phép vị tự $\mathbf{x} \mapsto \alpha \mathbf{x}$ là độ đo $\alpha^{1-n} \mu_{n-1}$. Do đó

$$
\mu_{n-1}(\mathbf{B}_n(z_n)) = \left( \sqrt{1 - z_n^2} \right)^{n-1} V_{n-1} .
$$

Thế vào (16), và thực hiện phép đổi biến $z_n = \sin \varphi$ (với $-\frac{\pi}{2} \leq \varphi \leq \frac{\pi}{2}$), ta được

$$
V_n = V_{n-1} \int_{-\frac{\pi}{2}}^{+\frac{\pi}{2}} \cos^n \varphi d\varphi = 2 V_{n-1} \int_0^{\frac{\pi}{2}} \cos^n \varphi d\varphi .
$$

Nhưng (FRV, Ch. VII, §1, No. 3, công thức (20))

$$
\int_0^{\frac{\pi}{2}} \cos^m \varphi d\varphi = \frac{1}{2} \frac{\Gamma \left( \frac{1}{2} \right) \Gamma \left( \frac{m+1}{2} \right)}{\Gamma \left( \frac{m+2}{2} \right)}
$$

và khi thế vào hệ thức (17) và chú ý đến biểu thức của $\Gamma \left( \frac{1}{2} \right)$ (FRV, VII, §1, No. 3, công thức (21)), cuối cùng ta thu được

$$
V_n = \frac{\pi^{n/2}}{\Gamma \left( \frac{n}{2} + 1 \right)} .
$$

Bài tập

### Bài tập {#int-v-s8-exercises}

Xem [các bài tập của § 8](exercises/s8/).
