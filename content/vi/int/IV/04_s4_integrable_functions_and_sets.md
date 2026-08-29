---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 4
section_title: Integrable functions and sets
lang: vi
source: int-i-vi
book_pages: INT IV.32-INT IV.59, INT IV.120-INT IV.127
pdf_pages: 0139-0166, 0227-0234
extraction: ocr
subsections:
    - "no": 1
      title: Extension of the integral
      page: 32
      pdf_page: 139
    - "no": 2
      title: Properties of the integral
      page: 34
      pdf_page: 141
    - "no": 3
      title: Passage to the limit in integrals
      page: 36
      pdf_page: 143
    - "no": 4
      title: Characterizations of integrable numerical functions
      page: 37
      pdf_page: 144
    - "no": 5
      title: Integrable sets
      page: 41
      pdf_page: 148
    - "no": 6
      title: Criteria for the integrability of a set
      page: 43
      pdf_page: 150
    - "no": 7
      title: Characterization of bounded measures
      page: 46
      pdf_page: 153
    - "no": 8
      title: Integration with respect to a measure with compact support
      page: 47
      pdf_page: 154
    - "no": 9
      title: Clans and additive set functions
      page: 50
      pdf_page: 157
    - "no": 10
      title: Approximation of continuous functions by step functions
      page: 52
      pdf_page: 159
    - "no": 11
      title: Extension of a measure defined on a family of sets
      page: 53
      pdf_page: 160
statements: 63
exercises: 23
content_sha256: 189965e66749ee96b2cce7d7dabbe37cdbee928d2cab22deb65f7b7ecbb01cbe
translated_from: content/en/int/IV/04_s4_integrable_functions_and_sets.md
source_content_sha256: 04515fb1fa953c06cc0b2f25528b8c99e5a79b5ad3a2d7ec3b4743f52081eec4
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-20725f8a
glossary_version: 34
glossary_terms_sha256: b623f2ebae90893d493cc0bc6d47e20a69a90e40f8f2071f3859e4af7367687e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CÁC HÀM KHẢ TÍCH VÀ CÁC TẬP HỢP

### 1. Mở rộng của nguyên hàm

Từ định nghĩa của không gian $\mathcal{L}_F^p$ suy ra rằng không gian con $\mathcal{K}_F$ của các hàm liên tục có giá compact là *trù mật* trong $\mathcal{L}_F^p$ (§ 3, No. 4, Định nghĩa 2). Mọi hàm tuyến tính liên tục (đối với tôpô hội tụ trung bình cấp $p$), xác định trên $\mathcal{K}_F$ và nhận các giá trị của nó trong một không gian vectơ tôpô Hausdorff *đầy đủ* $G$, do đó có thể được *mở rộng bằng tính liên tục* một cách duy nhất, thành một hàm tuyến tính liên tục xác định trên $\mathcal{L}_F^p$ với các giá trị trong $G$ (GT, II, § 3, No. 6, Định lý 2 và III, § 3, No. 1, Mệnh đề 3).

Bây giờ, đối với mọi hàm liên tục $f$ có giá compact, nhận các giá trị trong không gian Banach $F$, ta đã định nghĩa (trong Ch. III, § 3, No. 1) *nguyên* $\mu(f) = \int f \, d\mu$ đối với $\mu$, là một phần tử của $F$, và ta đã chứng minh (Ch. III, § 3, No. 2, Mệnh đề 6) bất đẳng thức

$$
\left| \int f \, d\mu \right| \leqslant \int |f| \, d|\mu| = N_1(f).
$$

Bất đẳng thức này chứng minh rằng ánh xạ tuyến tính $f \mapsto \int f \, d\mu$ từ $\mathcal{K}_F$ vào $F$ là liên tục đối với tôpô hội tụ trung bình trong $\mathcal{K}_F$. Do đó nó có thể được mở rộng bằng tính liên tục đến toàn bộ không gian $\mathcal{L}_F^1$, và ta có thể đưa ra định nghĩa sau:

#### Định nghĩa 1 {#int-iv-s4-def-1 .statement}

*Các hàm thuộc $\mathcal{L}_F^1(X, \mu)$ được gọi là khả tích đối với độ đo $\mu$* (hoặc, một lần nữa, được gọi là $\mu$-khả tích). *Nguyên (đối với $\mu$) của hàm khả tích $f$ theo định nghĩa là giá trị tại $f$ của mở rộng bằng tính liên tục lên $\mathcal{L}_F^1$ của ánh xạ tuyến tính $g \mapsto \int g\, d\mu$ từ $\mathcal{H}_F$ vào $F$; nó lại được ký hiệu là $\mu(f)$ hoặc $\int f\, d\mu$, hoặc $\int f(x)\, d\mu(x)$ hoặc $\int f\mu$, hoặc $\int f(x)\mu(x)$.

#### Ví dụ {#int-iv-s4-n1-exa-1 .statement}

— Cho $X$ là một không gian *rời rạc*, $\mu$ là một độ đo trên $X$, và đặt $\alpha(x) = \mu(\varphi_{\{x\}})$ đối với mọi $x \in X$. Khi đó các hàm trong $\mathcal{F}_F^1$ là *khả tích*, nói cách khác $\mathcal{L}_F^1 = \mathcal{F}_F^1$; hơn nữa, đối với mọi hàm $f \in \mathcal{L}_F^1$,

$$
\int f\, d\mu = \sum_{x \in X} \alpha(x)f(x).
$$

Thật vậy, cho $f \in \mathcal{F}_F^1$; ta có $|\mu|^*(|f|) = \sum_{x \in X} |\alpha(x)| \cdot |f(x)| < +\infty$ (§ 1, No. 3, *Ví dụ*); với mọi $\varepsilon > 0$, tồn tại một tập con hữu hạn $M$ của $X$ sao cho

$$
\sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon.
$$

Hàm $g$ bằng $f$ tại các điểm $x \in M$ nơi $|f|$ là hữu hạn, và bằng 0 ở các nơi khác, thuộc về $\mathcal{H}(X; F)$ và, theo các quy ước đã được đưa ra,

$$
|\mu|^*(|f - g|) \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon,
$$

điều này chứng minh rằng $f \in \mathcal{L}_F^1$. Mặt khác,

$$
\left| \mu(g) - \sum_{x \in X} \alpha(x)f(x) \right| \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon,
$$

do đó có mệnh đề thứ hai.

Nói cách khác, các hàm $\mu$-khả tích $f$ là những hàm sao cho họ $(\alpha(x)f(x))_{x \in X}$ là *khả tổng tuyệt đối* (GT, IX, §3, No. 6), và nguyên $\int f\, d\mu$ là tổng của họ này.

Vì $\mu(f)$ là liên tục trên $\mathcal{L}_F^1$ theo định nghĩa, và vì nó nhận các giá trị trong một không gian Hausdorff, ta có $\mu(f) = 0$ đối với mọi hàm thuộc bao đóng của 0 trong $\mathcal{L}_F^1$, tức là *không đáng kể*; nếu $f$ và $g$ là hai hàm khả tích *tương đương*, thì $\mu(f) = \mu(g)$. Nói cách khác, giá trị của $\mu(f)$ chỉ phụ thuộc vào lớp $\tilde{f}$ của hàm khả tích $f$; nó lại được ký hiệu là $\mu(\tilde{f})$, và ánh xạ $\tilde{f} \mapsto \mu(\tilde{f})$ là một ánh xạ tuyến tính liên tục của $L^1_F$ vào $F$. Nếu một hàm $f$, có giá trị trong $F$ và được xác định gần khắp nơi trong $X$, tương đương với một hàm khả tích, ta lại nói rằng $f$ là *khả tích* và viết $\int f\, d\mu = \mu(\tilde{f})$; người ta cũng định nghĩa tương tự một hàm khả tích có giá trị trong $\overline{\mathbf{R}}$, được xác định và hữu hạn gần khắp nơi, cũng như nguyên của nó.

### 2. Các tính chất của nguyên

#### Mệnh đề 1 {#int-iv-s4-prop-1 .statement}

*Với mọi hàm số dương khả tích theo $\mu$ $f$,*

$$
\int f\, d|\mu| = \int^* f\, d|\mu| = N_1(f) \geqslant 0.
$$

Thật vậy, $\int f\, d|\mu|$ và $N_1(f)$ là liên tục trên $\mathcal{L}^1$ và bằng nhau đối với mọi hàm liên tục $f \geqslant 0$ có giá đỡ compact; mặt khác, mọi hàm $f \geqslant 0$ trong $\mathcal{L}^1$ là giới hạn (theo nghĩa hội tụ theo trung bình) của một dãy các hàm liên tục $\geqslant 0$ có giá đỡ compact (§ 3, No. 5, Mệnh đề 11); do đó mệnh đề.

#### Hệ quả 1 {#int-iv-s4-prop-1-cor-1 .statement}

*Với mọi hàm khả tích $f \in \mathcal{L}^1_F$, $|f|$ là khả tích và*

$$
\int |f|\, d|\mu| = \int^* |f|\, d|\mu| = N_1(f).
$$

Chúng ta sẽ thường xuyên dùng Mệnh đề 1 và Hệ quả 1 của nó, khi thay $\int^* f\, d|\mu|$ hoặc $N_1(f)$ bằng $\int f\, d|\mu|$ khi xét một hàm khả tích $\geqslant 0$. Chẳng hạn, để hai hàm khả tích $f, g$ là *tương đương*, điều kiện cần và đủ là $\int |f - g|\, d|\mu| = 0$.

Ta nhắc lại rằng, để một hàm $f$ thuộc $\mathcal{L}^p_F$, điều kiện cần và đủ là hàm $|f|^{p-1} \cdot f$ thuộc $\mathcal{L}^1_F$ (§ 3, No. 8, Hệ quả 1 của ĐL. 7), tức là nó khả tích; đó là lý do của thuật ngữ 'hàm khả tích lũy thừa bậc $p$'. Hơn nữa:

#### Hệ quả 2 {#int-iv-s4-prop-1-cor-2 .statement}

*Với mọi hàm $f \in \mathcal{L}^p_F$, hàm số $|f|^p$ là khả tích và*

$$
N_p(f) = \left( \int |f|^p\, d|\mu| \right)^{1/p}.
$$

Điều này suy ra ngay từ việc $|f|$ thuộc $\mathcal{L}^p$ (§ 3, No. 5, Mệnh đề 11) và công thức (2).

#### Mệnh đề 2 {#int-iv-s4-prop-2 .statement}

— Với mọi hàm khả tích $f$,

$$
\left| \int f \, d\mu \right| \leq \int |f| \, d|\mu|.
$$

Điều này suy ra ngay từ bất đẳng thức (1) bằng cách lấy giới hạn, có xét đến (3) và tính liên tục của $N_1(f)$ trên $\mathcal{L}_F^1$.

#### Định lý 1 {#int-iv-s4-thm-1 .statement}

— Cho $F$ và $G$ là hai không gian Banach, $u$ là một ánh xạ tuyến tính liên tục của $F$ vào $G$. Với mọi hàm khả tích $f$ nhận giá trị trong $F$, $u \circ f$ là khả tích và

$$
\int u(f(x)) \, d\mu(x) = u \left( \int f(x) \, d\mu(x) \right).
$$

Ta đã biết rằng $u \circ f$ là khả tích (§ 3, No. 5, Định lý 4); quan hệ (6), vì đúng với mọi $f \in \mathcal{H}_F$, được mở rộng cho mọi hàm khả tích $f$ bởi nguyên lý mở rộng các đẳng thức: thật vậy, $f \mapsto u \circ f$ là liên tục đối với tôpô hội tụ theo trung bình, như suy ra từ bất đẳng thức $N_1(u \circ f) \leq \|u\| \cdot N_1(f)$.

#### Hệ quả 1 {#int-iv-s4-thm-1-cor-1 .statement}

— Cho $a'$ là một dạng tuyến tính liên tục trên $F$. Nếu $f$ là một hàm khả tích với giá trị trong $F$, thì hàm số vô hướng $\langle f, a' \rangle$ là khả tích và

$$
\int \langle f(x), a' \rangle \, d\mu(x) = \left\langle \int f(x) \, d\mu(x), a' \right\rangle.
$$

Ta sẽ thấy ở Ch. VI, § 1, Bài tập 7, 11 và 12 rằng có thể tồn tại các hàm $f$, với giá trị trong một không gian Banach vô hạn chiều $F$, sao cho $\langle f, a' \rangle$ khả tích với mọi dạng tuyến tính liên tục $a'$ trên $F$, mà $f$ không khả tích.

#### Hệ quả 2 {#int-iv-s4-thm-1-cor-2 .statement}

— Nếu các $a_k$ ($1 \leq k \leq n$) là các vectơ trong $F$ và các $f_k$ ($1 \leq k \leq n$) là các hàm số vô hướng khả tích, thì hàm $f = \sum_{k=1}^n a_k f_k$ là khả tích và

$$
\int \left( \sum_{k=1}^n a_k f_k \right) d\mu = \sum_{k=1}^n a_k \int f_k \, d\mu.
$$

### 3. Chuyển sang giới hạn trong các tích phân

#### Mệnh đề 3 {#int-iv-s4-prop-3 .statement}

— Cho $\mathcal{B}$ là một cơ sở lọc trên $\mathcal{L}_F^1$. Giả sử tồn tại một tập compact $K \subset X$ sao cho, với mọi tập $M \in \mathcal{B}$, mọi hàm $f \in M$ đều có giá trong $K$. Trong những điều kiện này, nếu $\mathcal{B}$ hội tụ đều trên $X$ đến $f_0$, thì hàm $f_0$ khả tích và

$$
\int f_0 \, d\mu = \lim_{\mathcal{B}} \int f \, d\mu .
$$

Thật vậy, $\mathcal{B}$ hội tụ theo trung bình đến $f_0$ (§ 3, No. 3, Mệnh đề 4).

#### Mệnh đề 4 {#int-iv-s4-prop-4 .statement}

— Cho $(f_n)$ là một dãy tăng (tương ứng giảm) các hàm số vô hướng khả tích. Để hàm bao trên (tương ứng bao dưới) $f$ của dãy khả tích, cần và đủ rằng $\sup_n \int f_n \, d|\mu| < +\infty$ (tương ứng $\inf_n \int f_n \, d|\mu| > -\infty$), trong trường hợp đó

$$
\int f \, d\mu = \lim_{n \to \infty} \int f_n \, d\mu .
$$

Chúng tôi chỉ xét một dãy tăng. Dãy $g_n = f_n + f_1^-$ là tăng và gồm các hàm khả tích $\geqslant 0$; vì hàm bao trên của nó là $g = f + f_1^-$, mệnh đề suy ra từ Định lý 5 của § 3, No. 6.

#### Định lý 2 {#int-iv-s4-thm-2 .statement}

==========

— Cho $A$ là một tập chỉ số, được lọc bởi một bộ lọc $\mathfrak{F}$ có một cơ sở đếm được. Cho $(f_\alpha)_{\alpha \in A}$ là một họ các hàm khả tích mà, đối với bộ lọc $\mathfrak{F}$, hội tụ từng điểm hầu khắp nơi đến một hàm số $f$; nếu tồn tại một hàm số $g \geqslant 0$ sao cho $\int^* g \, d|\mu| < +\infty$ và sao cho $|f_\alpha(x)| \leqslant g(x)$ hầu khắp nơi trên $X$ với mỗi $\alpha \in A$, thì hàm số $f$ khả tích và

$$
\int f \, d\mu = \lim_{\mathfrak{F}} \int f_\alpha \, d\mu .
$$

Định lý suy ra từ định lý của Lebesgue (§ 3, No. 7, Hệ quả của Định lý 6) vì, dưới các điều kiện của phát biểu, $f_\alpha$ hội tụ theo trung bình đến $f$ đối với $\mathfrak{F}$.

#### Hệ quả 1 {#int-iv-s4-thm-2-cor-1 .statement}

— Cho $\Omega$ là một không gian tôpô, $t_0$ là một điểm của $\Omega$ thừa nhận một hệ cơ bản đếm được các lân cận, $f$ là một ánh xạ của $X \times \Omega$ vào $F$ có các tính chất sau:
a) với mọi $t \in \Omega$, hàm số $x \mapsto f(x, t)$ là khả tích;
b) với mọi $x \in X$, hàm số $t \mapsto f(x, t)$ liên tục tại $t_0$;

c) tồn tại một lân cận U của $t_0$ và một hàm số g \geqslant 0 xác định trên X, sao cho $\int^* g d|\mu| < +\infty$ và $|\mathbf{f}(x,t)| \leqslant g(x)$ với mọi $x \in X$ và $t \in U$.

Dưới các điều kiện này, ánh xạ $t \mapsto \int \mathbf{f}(x,t) d\mu(x)$ của $\Omega$ vào $F$ là liên tục tại điểm $t_0$.

#### Hệ quả 2 {#int-iv-s4-thm-2-cor-2 .statement}

— Cho $(\mathbf{f}_n)$ là một dãy các hàm khả tích sao cho chuỗi có số hạng tổng quát $\mathbf{f}_n(x)$ hội tụ hầu khắp nơi; nếu tồn tại một hàm số $g \geqslant 0$ sao cho $\int^* g d|\mu| < +\infty$ và sao cho, với mọi số nguyên $n$, $\left| \sum_{k=1}^n \mathbf{f}_k(x) \right| \leqslant g(x)$ hầu khắp nơi, thì tổng $\mathbf{f}(x)$ (được xác định hầu khắp nơi) của chuỗi có số hạng tổng quát $\mathbf{f}_n(x)$ là khả tích và

$$
\int \mathbf{f} d\mu = \sum_{n=1}^\infty \int \mathbf{f}_n d\mu
$$

('phép tích phân từng số hạng của một chuỗi').

### 4. Các đặc trưng của các hàm số khả tích

#### Mệnh đề 5 {#int-iv-s4-prop-5 .statement}

— Để một hàm số $f \geqslant 0$ (hữu hạn hoặc không), nửa liên tục dưới trên X, khả tích, điều kiện cần và đủ là $\int^* f d|\mu| < +\infty$.

Mọi việc quy về chứng minh rằng điều kiện ấy là đủ. Định nghĩa của $|\mu|^*(f)$ (§ 1, No. 1, Định nghĩa 1) cho thấy rằng, với mọi $\varepsilon > 0$, tồn tại một hàm liên tục $g \geqslant 0$, có giá compact, sao cho $g \leqslant f$ và $|\mu|^*(f) \leqslant |\mu|(g) + \varepsilon$. Nhưng $f - g$ là nửa liên tục dưới và $\geqslant 0$, do đó (§ 1, No. 1, Định lý 2)

$$
|\mu|^*(f) = |\mu|(g) + |\mu|^*(f - g),
$$

nói cách khác $N_1(f - g) = |\mu|^*(f - g) = |\mu|^*(f) - |\mu|(g) \leqslant \varepsilon$, điều đó chứng tỏ rằng $f$ khả tích (§ 3, No. 4, Mệnh đề 7).

#### Hệ quả 1 {#int-iv-s4-prop-5-cor-1 .statement}

— Để một hàm số hữu hạn $f \geqslant 0$, nửa liên tục trên X, khả tích, điều kiện cần và đủ là $\int^* f d|\mu| < +\infty$.

==========

Vì, nếu $|\mu|^*(f) < +\infty$, thì tồn tại một hàm nửa liên tục dưới $h$ sao cho $f \leqslant h$ và $|\mu|^*(h) < +\infty$; $h - f$ được xác định ở mọi nơi và nửa liên tục dưới, và $|\mu|^*(h - f) \leqslant |\mu|^*(h) < +\infty$; do đó $h - f$ khả tích, và vì $f(x) = h(x) - (h(x) - f(x))$ hầu khắp nơi, nên $f$ khả tích.

#### Hệ quả 2 {#int-iv-s4-prop-5-cor-2 .statement}

— Cho $\mathbf{H}$ là một tập khác rỗng, có hướng đối với quan hệ $\leqslant$ (resp. $\geqslant$), gồm các hàm số trị số nửa liên tục dưới (resp. nửa liên tục trên) và khả tích; nếu

$$
\sup_{f \in \mathbf{H}} \int f \, d|\mu| < +\infty \quad \text{(resp. } \inf_{f \in \mathbf{H}} \int f \, d|\mu| > -\infty \text{)},
$$

thì bao trên (resp. bao dưới) $g$ của $\mathbf{H}$ là khả tích,

$$
\int g \, d\mu = \lim_{f \in \mathbf{H}} \int f \, d\mu,
$$

và $\int g \, d|\mu| = \sup_{f \in \mathbf{H}} \int f \, d|\mu|$ (resp. $\int g \, d|\mu| = \inf_{f \in \mathbf{H}} \int f \, d|\mu|$).

Ta có thể giới hạn ở trường hợp các hàm nửa liên tục dưới; khi $f$ chạy qua $\mathbf{H}$, các hàm $f^+$ (resp. $f^-$) khi đó tạo thành một tập có hướng đối với $\leqslant$ (resp. $\geqslant$) của các hàm nửa liên tục dưới (resp. nửa liên tục trên) $\geqslant 0$; bao trên (resp. bao dưới) của các $f^+$ (resp. $f^-$), với $f \in \mathbf{H}$, bằng $g^+$ (resp. $g^-$). Mặt khác, ta có thể thay thế $\mathbf{H}$ bằng một trong các đoạn của nó (đoạn này đồng cuối với nó), gồm các $f \in \mathbf{H}$ thỏa $\geqslant f_0$, với một hàm $f_0 \in \mathbf{H}$ nào đó; khi đó $\int f^+ \, d|\mu| \leqslant \int f \, d|\mu| + \int f_0^- \, d|\mu|$; do đó ta thấy rằng ta quy về việc chứng minh hai mệnh đề của hệ quả trong trường hợp $\mathbf{H}$ gồm các hàm dương. Nếu $\mathbf{H}$ có hướng đối với $\leqslant$ và gồm các hàm nửa liên tục dưới $\geqslant 0$, thì ta biết (§ 1, No. 1, Th. 1) rằng

$$
|\mu|^*(g) = \sup_{f \in \mathbf{H}} |\mu|^*(f) = \sup_{f \in \mathbf{H}} \int f \, d|\mu| < +\infty,
$$

do đó $g$, vốn nửa liên tục dưới, là khả tích theo Mệnh đề 5; ta có $\int g \, d|\mu| = \lim_{f \in \mathbf{H}} \int f \, d|\mu|$ và, vì $f \leqslant g$, $\lim_{f \in \mathbf{H}} N_1(g - f) = 0$, điều này cho thấy $f$ hội tụ theo nghĩa trung bình tới $g$ đối với $\mathbf{H}$, và do đó chứng minh hệ quả trong trường hợp này. Nếu $\mathbf{H}$ là tập có hướng theo $\geqslant$ và gồm các hàm số khả tích nửa liên tục trên $f$ sao cho $0 \leqslant f \leqslant f_1$ với $f_1 \in \mathbf{H}$, thì tồn tại một hàm số khả tích nửa liên tục dưới $h$ sao cho $f_1 \leqslant h$; ta có thể viết $f = h - f'$, trong đó $f'(x) = h(x) - f(x)$ khi $f(x) < +\infty$, và $f'(x) = 0$ trong trường hợp khác. Rõ ràng các $f'$ tạo thành một tập có hướng, theo $\leqslant$, gồm các hàm số khả tích nửa liên tục dưới $\geqslant 0$, với

$$
\int f' \, d|\mu| \leqslant \int h \, d|\mu| < +\infty;
$$

ta có thể áp dụng cho chúng điều đã được chứng minh ở trên; nếu $g'$ là bao trên của các $f'$, thì $h$ và $g'$ đều hữu hạn hầu khắp nơi, do đó $h - g'$ được xác định hầu khắp nơi và bằng $g$ hầu khắp nơi; từ đó, các kết luận của hệ quả suy ra ngay trong trường hợp này.

#### Hệ quả 3 {#int-iv-s4-prop-5-cor-3 .statement}

— Cho $f$ là một hàm số thực bị chặn, nửa liên tục trên trên $X$ và có giá compact. Khi đó, ánh xạ $\mu \mapsto \int f\, d\mu$ là nửa liên tục trên trên $\mathcal{M}_+(X)$ đối với tôpô vague.

Nếu $h$ là một hàm thuộc $\mathcal{K}_+(X)$ sao cho $|f| \leq h$ (Chương III, §1, No. 2, Bổ đề 1) thì $0 \leq f + h \leq 2h$, và vì $f + h$ là nửa liên tục trên, suy ra từ Hệ quả 1 rằng $f$ là $\mu$-khả tích với mọi độ đo $\mu$ trên $X$. Hơn nữa, $\mu(f) = \mu(h) - \mu(h - f)$ và $h - f$ là một hàm nửa liên tục dưới $\geq 0$. Vì ánh xạ $\mu \mapsto \mu(h - f)$ là nửa liên tục dưới trên $\mathcal{M}_+(X)$ đối với tôpô vague (§1, No. 1, Mệnh đề 4), điều này chứng minh hệ quả.

#### Định lý 3 {#int-iv-s4-thm-3 .statement}

— Để một hàm số thực $f \geq 0$ là khả tích, điều kiện cần và đủ là, với mọi $\varepsilon > 0$, tồn tại một hàm nửa liên tục trên $g \geq 0$, nhận giá trị hữu hạn và có giá compact, và một hàm khả tích nửa liên tục dưới $h$, sao cho $g \leq f \leq h$ và $\int (h - g)\, d|\mu| \leq \varepsilon$.

Điều kiện này là đủ theo một tiêu chuẩn tổng quát về tính khả tích (§3, No. 4, Mệnh đề 8), Mệnh đề 5 và Hệ quả 1 của nó. Ta hãy chứng minh rằng điều kiện này là cần thiết. Nếu $f \geq 0$ là khả tích thì, với mọi $\varepsilon > 0$, tồn tại một hàm $u \geq 0$, liên tục và có giá compact, sao cho $N_1(f - u) \leq \varepsilon/4$. Theo định nghĩa của $N_1$, điều đó suy ra rằng tồn tại một hàm nửa liên tục dưới $v \geq 0$ sao cho $|\mu|^*(v) \leq \varepsilon/2$ và $|f - u| \leq v$. Do đó, $-v(x) \leq f(x) - u(x) \leq v(x)$ với mọi $x \in X$, và vì $u(x)$ hữu hạn mọi nơi, suy ra $(u(x) - v(x))^+ \leq f(x) \leq u(x) + v(x)$ với mọi $x \in X$. Hai hàm $g = (u - v)^+$ và $h = u + v$ thỏa mãn các yêu cầu.

#### Hệ quả {#int-iv-s4-n4-cor-1 .statement}

— Với mọi hàm khả tích (tương ứng khả tích và $\geq 0$) $f$, tồn tại một dãy tăng $(g_n)$ gồm các hàm nửa liên tục trên khả tích (tương ứng khả tích, có giá trị hữu hạn $\geq 0$, và có giá compact), và một dãy giảm $(h_n)$ gồm các hàm khả tích nửa liên tục dưới, sao cho:
$1^\circ$ $g_n(x) \leq f(x) \leq h_n(x)$ với mọi $x \in X$ và mọi số nguyên $n$;
$2^\circ$ $f(x)$ bằng hầu khắp nơi với bao dưới $h$ của dãy $(h_n)$ và với bao trên $g$ của dãy $(g_n)$;
$3^\circ$ $\int f\, d\mu = \lim_{n \to \infty} \int g_n\, d\mu = \lim_{n \to \infty} \int h_n\, d\mu$.

Trước hết giả sử $f \geq 0$. Theo Định lý 3, với mọi $n$, tồn tại một hàm nửa liên tục dưới khả tích $v_n$, và một hàm nửa liên tục trên $u_n \geq 0$ có giá trị hữu hạn và có giá compact, sao cho

$$
u_n \leq f \leq v_n \quad \text{và} \quad \int (v_n - u_n)\, d|\mu| \leq 1/n;
$$

đặt $g_n = \sup(u_1, u_2, \ldots, u_n)$ và $h_n = \inf(v_1, v_2, \ldots, v_n)$, các dãy $(g_n)$ và $(h_n)$ thỏa mãn các yêu cầu. Thật vậy, vì $g \leq f$, nên $g$ khả tích theo Mệnh đề 4 của No. 3, và vì
$$
\int (f - g_n) d|\mu| \leq \int (v_n - u_n) d|\mu| \leq 1/n
$$
ta có
$$
\int (f - g) d|\mu| = \lim_{n \to \infty} \int (f - g_n) d|\mu| = 0
$$
(No. 3, Mệnh đề 4), điều đó chứng tỏ rằng $f$ và $g$ tương đương. Ta lập luận tương tự cho dãy $(h_n)$.

Nếu $f$ không dương, ta có thể áp dụng điều trên cho $f^+$ và $f^-$, do đó có hai dãy tăng $(g'_n), (g''_n)$ gồm các hàm khả tích nửa liên tục trên, và hai dãy giảm $(h'_n), (h''_n)$ gồm các hàm khả tích nửa liên tục dưới, sao cho: $1^\circ \ g'_n \leq f^+ \leq h'_n,\ g''_n \leq -f^- \leq h''_n;$
$2^\circ \ f^+$ (resp. $-f^-$) bằng gần khắp nơi bao trên của $g'_n$ và bao dưới của $h'_n$ (resp. bao trên của $g''_n$ và bao dưới của $h''_n$); và $3^\circ$:
$$
\int f^+ d\mu = \lim_{n \to \infty} \int g'_n d\mu = \lim_{n \to \infty} \int h'_n d\mu,
$$
$$
-\int f^- d\mu = \lim_{n \to \infty} \int g''_n d\mu = \lim_{n \to \infty} \int h''_n d\mu.
$$
Hơn nữa, ta có thể giả sử rằng các $g'_n$ và các $h''_n$ đều hữu hạn khắp nơi; khi đó hiển nhiên các dãy $g_n = g'_n + g''_n$ và $h_n = h'_n + h''_n$ thỏa mãn các yêu cầu.

#### Ví dụ {#int-iv-s4-n4-exa-1 .statement}

Đối với mọi độ đo dương $\mu$ trên $\mathbf{R}$, mọi *hàm bậc thang* có giá compact đều khả tích theo $\mu$; vì hàm đặc trưng của một khoảng mở (resp. đóng) là nửa liên tục dưới (resp. nửa liên tục trên), và mọi hàm bậc thang đều là một tổ hợp tuyến tính của các hàm đặc trưng như thế. Suy ra rằng nếu $\mathbf{f}$ là một *hàm chỉnh* trên $\mathbf{R}$ có giá compact (FRV, II, §1, No. 3), thì $\mathbf{f}$ khả tích, vì nó là giới hạn đều của một dãy các hàm bậc thang $\mathbf{g}_n$ có giá được chứa trong một tập compact cố định (No. 3, Mệnh đề 3); hơn nữa, $\int \mathbf{f}\, d\mu = \lim_{n \to \infty} \int \mathbf{g}_n\, d\mu$.

Nếu, nói riêng, lấy $\mu$ là độ đo Lebesgue, ta thấy rằng đối với mọi hàm chỉnh $\mathbf{f}$ có giá compact, tích phân $\int \mathbf{f}\, d\mu$ bằng tích phân $\int_{-\infty}^{+\infty} \mathbf{f}(x)\, dx$ được định nghĩa trong FRV, II, §2, No. 1.

#### Nhận xét 1 {#int-iv-s4-n4-rem-1 .statement}

Cho $\mathbf{f}$ là một hàm chỉnh trên $\mathbf{R}$ khả tích đối với độ đo Lebesgue $\mu$; khi đó $|\mathbf{f}|$ cũng khả tích (No. 2, Hệ quả 1 của Mệnh đề 1), và, đặt $I_n = [-n, n]$, $|\mathbf{f}|$ là bao trên của dãy tăng các hàm chỉnh $|\mathbf{f}| \varphi_{I_n}$, do đó $\int |\mathbf{f}|\, d\mu = \lim_{n \to \infty} \int_{-n}^{n} |\mathbf{f}(x)|\, dx$ theo Định lý 2 của No. 3; vì thế, tích phân $\int_{-\infty}^{+\infty} f(x) dx$ là *hội tụ tuyệt đối* (FRV, II, §2, No. 3). Hơn nữa, $\int f\, d\mu = \int_{-\infty}^{+\infty} f(x) dx$ theo Định lý 2 của No. 3. Ngược lại, giả sử rằng $\int_{-\infty}^{+\infty} f(x) dx$ hội tụ tuyệt đối; một lần nữa, theo Định lý 2 của No. 3, $\int f\, d\mu = \int_{-\infty}^{+\infty} f(x) dx$. Lưu ý rằng nếu tích phân $\int_{-\infty}^{+\infty} f(x) dx$ hội tụ nhưng không hội tụ tuyệt đối; thì $f$ *không khả tích* đối với độ đo Lebesgue.

#### Nhận xét 2 {#int-iv-s4-n4-rem-2 .statement}

Áp dụng cho độ đo Lebesgue và cho các hàm chỉnh, Mệnh đề 3 của No. 3 cho lại định lý về chuyển qua giới hạn đối với các tích phân của các hàm chỉnh trên một khoảng compact (FRV, II, §3, No. 1, Mệnh đề 1); đối với *các dãy* (hay đối với các bộ lọc có một cơ sở đếm được) các hàm chỉnh, Định lý 2 của No. 3 cải thiện rất nhiều mệnh đề này vì, đối với các hàm chỉnh bị chặn đều trên một khoảng compact, nó thay thế hội tụ *từng điểm* cho hội tụ *đều* (cf. §5, No. 4, Định lý 2). Tuy nhiên, về sự chuyển qua giới hạn đối với các tích phân *hội tụ tuyệt đối* của các hàm chỉnh trên một khoảng không compact, ta nhận xét rằng các điều kiện của Định lý 2 của No. 3 kéo theo rằng các tích phân đang xét là *hội tụ đều* (theo nghĩa được định nghĩa trong FRV, II, §3, No. 2), và do đó không cải thiện các điều kiện hội tụ được cho trong Sách IV (*loc. cit.*) ngoại trừ phần liên quan đến sự hội tụ của các hàm $f_\alpha$ trên mọi khoảng compact. Cuối cùng, các điều kiện chuyển qua giới hạn được cho đối với các tích phân của các hàm chỉnh *không hội tụ tuyệt đối* vẫn nằm ngoài lý thuyết được phát triển trong chương này.

### 5. Các tập hợp khả tích

#### Định nghĩa 2 {#int-iv-s4-def-2 .statement}

*Một tập con* $A$ *của một không gian compact địa phương* $X$ *được gọi là khả tích đối với một độ đo* $\mu$ *trên* $X$ *(hay là* $\mu$*-khả tích)* *nếu hàm đặc trưng* $\varphi_A$ *của* $A$ *là khả tích.* *Số hữu hạn* $\mu(A) = \int \varphi_A\, d\mu$ *được gọi là độ đo của* $A$.

Đối với mọi tập khả tích $A$, $|\mu|(A) = |\mu|^*(A)$ (No. 2, Mệnh đề 1); để một tập là *không đáng kể*, điều kiện cần và đủ là nó có *độ đo bằng không đối với* $|\mu|$.

#### Mệnh đề 6 {#int-iv-s4-prop-6 .statement}

*Hợp của một họ hữu hạn* $(A_i)_{1 \leq i \leq n}$ *gồm các tập khả tích là khả tích,* và

$$
|\mu| \left( \bigcup_{i=1}^n A_i \right) \leq \sum_{i=1}^n |\mu|(A_i).
$$

*Hơn nữa, nếu* $A_i$ *từng đôi một rời nhau, thì*

$$
\mu \left( \bigcup_{i=1}^n A_i \right) = \sum_{i=1}^n \mu(A_i).
$$

Vì, nếu $A = \bigcup_{i=1}^n A_i$ thì $\varphi_A = \sup \varphi_{A_i}$, do đó (§ 3, No. 5, Hệ quả của Mệnh đề 12) nếu các $A_i$ khả tích thì $A$ cũng vậy; quan hệ (13) là một trường hợp riêng của quan hệ tương tự đối với các độ đo ngoài (§ 1, No. 4, Mệnh đề 18), khi xét tới quan hệ $|\mu|(A) = |\mu|^*(A)$; cuối cùng, nếu các $A_i$ từng đôi một rời nhau, thì $\varphi_A = \sum_{i=1}^n \varphi_{A_i}$, suy ra (14).

#### Mệnh đề 7 {#int-iv-s4-prop-7 .statement}

1° *Nếu A và B là hai tập khả tích sao cho $B \subset A$, thì tập $C = A - B$ khả tích và*

$$
\mu(C) = \mu(A) - \mu(B).
$$

2° *Giao của một họ đếm được các tập khả tích là khả tích.*

Phần thứ nhất suy ra từ việc $\varphi_C = \varphi_A - \varphi_B$. Mặt khác, nếu $(A_n)$ là một dãy các tập khả tích và $A$ là giao của nó, thì $\varphi_A = \inf_n \varphi_{A_n}$, do đó $A$ khả tích (No. 3, Mệnh đề 4).

#### Hệ quả {#int-iv-s4-n5-cor-1 .statement}

*Nếu $(A_n)$ là một dãy giảm các tập khả tích, thì* $\mu(\bigcap_n A_n) = \lim_{n \to \infty} \mu(A_n)$.

Vì, nếu $A = \bigcap_n A_n$ thì $\varphi_A$ là bao dưới của dãy giảm $(\varphi_{A_n})$ (No. 3, Mệnh đề 4).

#### Mệnh đề 8 {#int-iv-s4-prop-8 .statement}

*Cho $(A_n)$ là một dãy tăng các tập khả tích; để hợp $A = \bigcup_n A_n$ khả tích, điều kiện cần và đủ là* $\sup_n |\mu|(A_n) < +\infty$, *trong trường hợp đó,*

$$
\mu(A) = \lim_{n \to \infty} \mu(A_n).
$$

Vì, các $\varphi_{A_n}$ tạo thành một dãy tăng các hàm khả tích, và $\varphi_A = \sup_n \varphi_{A_n}$; do đó, mệnh đề suy ra từ Mệnh đề 4 của No. 3.

#### Hệ quả {#int-iv-s4-n5-cor-2 .statement}

*Cho $(A_n)$ là một dãy các tập khả tích sao cho* $\sum_{n=1}^\infty |\mu|(A_n) < +\infty$; *hợp* $A = \bigcup_n A_n$ *khả tích, và*

$$
|\mu| \left( \bigcup_n A_n \right) \leq \sum_{n=1}^\infty |\mu|(A_n).
$$

Vì, $\varphi_A = \sup_n \varphi_{A_n}$ và

$$
|\mu|^*(A) \leq \sum_{n=1}^\infty |\mu|^*(A_n) = \sum_{n=1}^\infty |\mu|(A_n) < +\infty
$$

(§ 1, No. 4, Mệnh đề 18); do đó A khả tích (§ 3, No. 6, Hệ quả 2 của Định lý 5) và, vì $|\mu|(A) = |\mu|^*(A)$, ta quả thật có (17).

#### Mệnh đề 9 {#int-iv-s4-prop-9 .statement}

— Cho $(A_n)$ là một dãy các tập khả tích từng đôi một rời nhau sao cho $\sum_{n=1}^\infty |\mu|(A_n) < +\infty$; khi đó

$$
\mu\left(\bigcup_n A_n\right) = \sum_{n=1}^\infty \mu(A_n).
$$

Vì, nếu $A = \bigcup_n A_n$ thì $\varphi_A = \sum_{n=1}^\infty \varphi_{A_n}$, và mệnh đề suy ra từ (17) và Hệ quả 2 của Định lý 2 của No. 3.

Quan hệ (18) cũng được diễn đạt bằng cách nói rằng độ đo $\mu$ cộng tính hoàn toàn trên tập các tập con khả tích của X.

### 6. Các tiêu chuẩn cho tính khả tích của một tập hợp

#### Mệnh đề 10 {#int-iv-s4-prop-10 .statement}

— Để một tập $A$ mở (tương ứng, đóng) trong X khả tích, điều kiện cần và đủ là $|\mu|^*(A) < +\infty$.

Vì khi đó $\varphi_A$ nửa liên tục dưới (tương ứng, nửa liên tục trên), mệnh đề suy ra từ Mệnh đề 5 của No. 4 và Hệ quả 1 của nó.

#### Hệ quả 1 {#int-iv-s4-prop-10-cor-1 .statement}

— Mọi tập compact đều khả tích; mọi tập mở tương đối compact đều khả tích.

#### Hệ quả 2 {#int-iv-s4-prop-10-cor-2 .statement}

— Với mọi độ đo dương $\mu$ trên X, $A \mapsto \mu^*(A)$ là một dung lượng trên X (xem GT, IX, §6, No. 9, Ví dụ).

#### Ví dụ {#int-iv-s4-n6-exa-1 .statement}

Đối với độ đo Lebesgue $\mu$ trên $\mathbf{R}$, từ Mệnh đề 10 suy ra rằng mọi khoảng mở bị chặn $[a, b[$ đều khả tích và có độ đo $b - a$ (\§1, No. 2, Mệnh đề 9). Vì mọi tập chỉ gồm một điểm đều là tập không đối với độ đo Lebesgue, suy ra rằng mọi khoảng có hai đầu mút $a$ và $b$ đều có cùng độ đo $b - a$.

#### Mệnh đề 11 {#int-iv-s4-prop-11 .statement}

— Cho $\mathcal{G}$ là một tập hợp, có hướng theo quan hệ $\subset$, gồm các tập hợp mở khả tích trong $X$; để $A = \bigcup_{G \in \mathcal{G}} G$ là khả tích, cần và đủ rằng $\sup_{G \in \mathcal{G}} |\mu|(G) < +\infty$, trong trường hợp đó $\mu(A) = \lim_\mathcal{G} \mu(G)$ và $|\mu|(A) = \sup_{G \in \mathcal{G}} |\mu|(G)$.

Vì, ta biết rằng $|\mu|^*(A) = \sup_{G \in \mathcal{G}} |\mu|(G)$ (§ 1, No. 2, Mệnh đề 7); do đó mệnh đề suy ra từ Mệnh đề 10.

#### Hệ quả {#int-iv-s4-n6-cor-1 .statement}

— Cho $\mathfrak{F}$ là một tập hợp, có hướng theo quan hệ $\supset$, gồm các tập hợp đóng khả tích trong $X$; khi đó tập hợp đóng $B = \bigcap_{H \in \mathfrak{F}} H$ là khả tích, và ta có
$$
\mu(B) = \lim_{\mathfrak{F}} \mu(H) \quad \text{và} \quad |\mu|(B) = \inf_{H \in \mathfrak{F}} |\mu|(H).
$$
Vì, cho $H_0$ là một tập hợp trong $\mathfrak{F}$; vì $H_0$ khả tích, nên nó được chứa trong một tập hợp mở khả tích $U$ (§ 1, No. 4, Mệnh đề 19); các tập hợp mở $U \cap \mathbf{C}H$ lập thành một tập hợp có hướng theo quan hệ $\subset$, được chứa trong $U$, và có hợp là $U \cap \mathbf{C}B$; do đó ta được quy về Mệnh đề 11.

#### Định lý 4 {#int-iv-s4-thm-4 .statement}

— Để một tập hợp $A$ là khả tích, cần và đủ rằng, với mọi $\varepsilon > 0$, tồn tại một tập hợp mở khả tích $G$ và một tập compact $K$, sao cho $K \subset A \subset G$ và
$$
|\mu|(G - K) = |\mu|(G) - |\mu|(K) \leq \varepsilon.
$$

a) Điều kiện là *đủ*, vì điều đó có nghĩa là $\varphi_K \leq \varphi_A \leq \varphi_G$ và $\int (\varphi_G - \varphi_K) d|\mu| \leq \varepsilon$; vì $\varphi_G$ và $\varphi_K$ khả tích, nên $\varphi_A$ cũng khả tích (§ 3, No. 4, Mệnh đề 8).

b) Điều kiện là *cần*. Nếu $A$ khả tích, tồn tại một tập hợp mở $G \supset A$ sao cho $|\mu|^*(G)$ tùy ý gần với $|\mu|^*(A) = |\mu|(A)$ (§ 1, No. 4, Mệnh đề 19); vì vậy, tất cả quy về việc chứng minh rằng với mọi $\varepsilon > 0$, tồn tại một tập compact $K \subset A$ sao cho $|\mu|(A) - |\mu|(K) \leq \varepsilon$. Vì $\varphi_A$ khả tích, tồn tại một hàm $f \geq 0$, nửa liên tục trên và có giá compact $S$, sao cho $f \leq \varphi_A$ và $\int (\varphi_A - f) d|\mu| \leq \varepsilon/2$ (No. 4, Định lý 3). Cho $\delta > 0$ là một số tùy ý và cho $K$ là tập hợp các điểm $x \in X$ sao cho $f(x) \geq \delta$; $K$ là đóng và được chứa trong $S$, do đó là *compact*, và vì $f \leq \varphi_A$ nên ta có $K \subset A$. Tập hợp $B = A - K$ là khả tích, và $f \leq \varphi_K + \delta \varphi_B$, suy ra
$$
\int f d|\mu| \leq |\mu|(K) + \delta \cdot |\mu|(B) \leq |\mu|(K) + \delta \cdot |\mu|(A),
$$
và cuối cùng
$$
|\mu|(A) \leq \int f d|\mu| + \frac{\varepsilon}{2} \leq |\mu|(K) + \delta \cdot |\mu|(A) + \frac{\varepsilon}{2},
$$
điều đó hoàn tất chứng minh, vì $\delta$ là tùy ý.

#### Hệ quả 1 {#int-iv-s4-thm-4-cor-1 .statement}

— Để một tập $A$ khả tích, cần và đủ là, với mọi $\varepsilon > 0$, tồn tại một tập compact $K \subset A$ sao cho $|\mu|^*(A - K) \leq \varepsilon$. Khi đó $|\mu|(A)$ là cận trên đúng của tập các độ đo $|\mu|(K)$ của các tập compact $K \subset A$.

Điều kiện là cần thiết, vì nếu $G$ và $K$ thỏa mãn các điều kiện của Định lý 4, thì $|\mu|^*(A - K) \leq |\mu|^*(G - K) \leq \varepsilon$.

Điều kiện là đủ, vì nó nói rằng, đối với tôpô hội tụ theo trung bình, $\varphi_A$ nằm trong bao đóng của tập các hàm khả tích $\varphi_K$ ($K$ là một tập con compact tùy ý của $A$).

#### Hệ quả 2 {#int-iv-s4-thm-4-cor-2 .statement}

— Với mọi tập khả tích $A$, tồn tại:

$1^\circ$ một tập $A_1 \supset A$, là giao đếm được của các tập mở khả tích, sao cho $A_1 - A$ là không đáng kể;

$2^\circ$ một tập $A_2 \subset A$, là hợp đếm được của các tập compact rời nhau từng đôi một, sao cho $A - A_2$ là không đáng kể.

$1^\circ$ Với mọi số nguyên $n$, tồn tại một tập mở khả tích $G_n \supset A$ sao cho $|\mu|(G_n) - |\mu|(A) \leq 1/n$; nếu $A_1$ là giao của các $G_n$, thì $|\mu|(A_1) = |\mu|(A)$ (No. 5, Hệ quả của Mệnh đề 7), do đó $A_1 - A$ là không đáng kể.

$2^\circ$ Định nghĩa các tập compact $K_n$ bằng quy nạp như sau: $K_1 \subset A$ và $|\mu|(A - K_1) \leq 1$; $K_n \subset A - \bigcup_{i=1}^{n-1} K_i$ và $|\mu|(A \cap \mathbf{C}(\bigcup_{i=1}^{n-1} K_i) \cap \mathbf{C}K_n) \leq 1/n$ đối với $n > 1$ (Th. 4); nếu $A_2$ là hợp của các $K_n$, thì $|\mu|(A_2) = |\mu|(A)$ (No. 5, Mệnh đề 8), do đó $A - A_2$ là không đáng kể.

#### Hệ quả 3 {#int-iv-s4-thm-4-cor-3 .statement}

— Mọi tập có độ đo ngoài hữu hạn đều được chứa trong hợp của một tập không đáng kể và một họ đếm được các tập compact rời nhau từng đôi một sao cho tổng các độ đo của chúng là hữu hạn.

Chỉ cần áp dụng Hệ quả 2 cho một tập mở khả tích chứa tập đã cho.

#### Hệ quả 4 {#int-iv-s4-thm-4-cor-4 .statement}

— Với mọi tập mở $U$ trong $X$, $|\mu|^*(U)$ là cận trên đúng của các độ đo $|\mu|(K)$ của các tập compact $K \subset U$.

Nếu $|\mu|^*(U) < +\infty$, điều này suy ra ngay từ Th. 4. Lập luận sau cũng bao quát trường hợp $|\mu|^*(U) = +\infty$. Vì $X$ compact địa phương và $U$ mở, nên $\varphi_U$ là bao trên của tập $H$ các hàm $f \in \mathcal{K}_+$ sao cho $f \leq \varphi_U$ và $\operatorname{Supp}(f) \subset U$ (xem chứng minh của §1, No. 1, Bổ đề), và, vì $H$ có hướng đối với $\leq$, ta có $|\mu|^*(U) = \sup_{f \in H} |\mu|(f)$ theo §1, No. 1, Th. 1; khi đó hệ quả suy ra ngay từ việc nếu $f \in H$ và $K = \operatorname{Supp}(f)$, thì $f \leq \varphi_K \leq \varphi_U$.

Chú ý rằng $|\mu|^*(U)$ cũng là cận trên đúng của các số đo $|\mu|(G)$ của các tập mở tương đối compact sao cho $\overline{G} \subset U$. Thật vậy, nếu $K$ là một tập compact được chứa trong $U$ thì, với mọi $x \in K$, tồn tại một lân cận mở tương đối compact $V$ của $x$ sao cho $\overline{V} \subset U$. Phủ $K$ bởi một số hữu hạn các lân cận đó, hợp của chúng $G$ là một tập mở tương đối compact sao cho $\overline{G} \subset U$ và $K \subset G$, do đó $|\mu|(K) \leq |\mu|(G) \leq |\mu|^*(U)$.

### 7. Đặc trưng hóa các độ đo bị chặn

#### Mệnh đề 12 {#int-iv-s4-prop-12 .statement}

— Đối với một độ đo $\mu$ trên một không gian compact địa phương $X$ để là bị chặn (Ch. III, §1, No. 8), điều kiện cần và đủ là $X$ là một tập khả tích đối với $\mu$ (hay, điều tương đương là, mọi hàm hằng hữu hạn đều khả tích); trong trường hợp này,

$$
\| \mu \| = | \mu |(X) = \int d|\mu|.
$$

Thật vậy, ta đã thấy rằng $|\mu|^*(X) = \| \mu \|$ (§ 1, No. 2); do đó mệnh đề suy ra từ Mệnh đề 10 của No. 6.

Đối với mọi độ đo bị chặn $\mu$, ta lại gọi $\mu(X)$ là khối lượng toàn phần của $\mu$.

Suy ra từ ĐL. 4 của No. 6 rằng nếu $\mu$ là một độ đo bị chặn thì, với mọi $\varepsilon > 0$, tồn tại một tập compact $K$ sao cho $|\mu|(CK) \leq \varepsilon$.

#### Mệnh đề 13 {#int-iv-s4-prop-13 .statement}

— Cho $\mu$ là một độ đo bị chặn trên $X$. Cho $\mathcal{B}$ là một cơ sở lọc trên $\mathcal{L}_F^p$ có các tính chất sau:
$1^\circ$ tồn tại một tập $M \in \mathcal{B}$ sao cho các hàm $f \in M$ bị chặn đều trên $X$;
$2^\circ$ $\mathcal{B}$ hội tụ đều trên mọi tập con compact của $X$ tới một hàm $f_0$.
Dưới các điều kiện này, $f_0$ thuộc $\mathcal{L}_F^p$ và $\mathcal{B}$ hội tụ trong trung bình cấp $p$ tới $f_0$.

Trước hết ta lưu ý rằng nếu $|f(x)| \leq a$ với mọi $x \in X$ và mọi hàm $f \in M$, thì cũng có $|f_0(x)| \leq a$ với mọi $x \in X$. Khi đó, với mọi $\varepsilon > 0$ tồn tại một tập compact $K$ sao cho $|\mu|(CK) \leq \varepsilon^p$ và một tập $N \in \mathcal{B}$ sao cho, với mọi hàm $f \in N$, $|f(x) - f_0(x)| \leq \varepsilon(|\mu|(K))^{-1/p}$ với mọi $x \in K$. Bây giờ, ta có thể viết

$$
f - f_0 = (f - f_0)\varphi_K + (f - f_0)\varphi_{CK};
$$

Suy ra từ điều trên rằng nếu $f \in M \cap N$ thì $N_p((f - f_0)\varphi_K) \leq \varepsilon$ và $N_p((f - f_0)\varphi_{CK}) \leq 2a\varepsilon$, do đó $N_p(f - f_0) \leq (2a + 1)\varepsilon$, điều đó chứng minh mệnh đề.

#### Hệ quả {#int-iv-s4-n7-cor-1 .statement}

— Đối với một độ đo bị chặn $\mu$ trên $X$, mọi ánh xạ liên tục bị chặn $f$ của $X$ vào $F$ đều thuộc vào từng $\mathcal{L}_F^p$ ($1 \leq p < +\infty$).

Với mọi tập con compact $K$ của $X$, cho $M_K$ là tập hợp các ánh xạ của $X$ vào $F$ có dạng $hf$, trong đó $h$ là một ánh xạ liên tục của $X$ vào $[0, 1]$ bằng 1 trên $K$ và có giá đỡ compact. Hiển nhiên các tập hợp $M_K$ tạo thành một cơ sở lọc $\mathcal{B}$ trên $\mathcal{L}_F^p$, các hàm thuộc $M_K$ đều bị chặn đều, và $\mathcal{B}$ hội tụ đều về $f$ trên mọi tập con compact của $X$, do đó có hệ quả.

Đặc biệt, hàm $f$ khả tích và tích phân $\int f\, d\mu$ của nó là giới hạn đối với $\mathcal{B}$ của các tích phân $\int h f\, d\mu$.

Chúng ta sẽ thu được lại Hệ quả của Mệnh đề 13 như một hệ quả của một tiêu chuẩn tổng quát về tính khả tích trong §5, No. 6.

Theo ký hiệu của Ch. III, §1, No. 2, $|f| \leq \|f\| \cdot 1$ đối với mọi hàm $f \in \mathcal{C}^b(X; F)$, do đó, theo các công thức (3) và (4) của No. 2,

$$
N_p(f) \leq \|f\| \cdot N_p(1) = \|f\| \cdot \|\mu\|^{1/p}.
$$

Đặc biệt, với $p = 1$, công thức (5) của No. 2 cho

$$
\left| \int f\, d\mu \right| \leq \|f\| \cdot \|\mu\|,
$$

do đó ánh xạ $f \mapsto \int f\, d\mu$ liên tục trên không gian Banach $\mathcal{C}^b(X; F)$; do hạn chế của nó lên bao đóng $\mathcal{C}^0(X; F)$ của $\mathcal{K}(X; F)$ trong $\mathcal{C}^b(X; F)$, tức là lên không gian các hàm liên tục tiến tới 0 tại điểm ở vô cực (Ch. III, §1, No. 2, Prop. 3), vì thế là sự mở rộng liên tục của tích phân lên $\mathcal{C}^0(X; F)$.

### 8. Tích phân đối với một độ đo có giá đỡ compact

Cho $\mu$ là một độ đo trên $X$ có giá đỡ $S = \operatorname{Supp}(\mu)$ là compact; tập mở $X - S$ là không đáng kể (§2, No. 2, Prop. 5). Với mọi hàm $f$ nhận giá trị trong một không gian vectơ $F$ hoặc trong $\overline{\mathbf{R}}$, các hàm $f$ và $f \varphi_S$ do đó là tương đương (§2, No. 4); để $f$ là $\mu$-khả tích (khi $F$ là một không gian Banach), do đó cần và đủ rằng $f \varphi_S$ cũng vậy, trong trường hợp đó (No. 1)

$$
\int f\, d\mu = \int f \varphi_S\, d\mu.
$$

Hơn nữa, nếu $f$ bị chặn trên $S$, thì từ (20) suy ra rằng

$$
\left| \int f\, d\mu \right| \leq \|\mu\| \cdot \sup_{x \in S} |f(x)|.
$$

Đặc biệt, nếu $f$ liên tục trên $X$ thì $f$ là $\mu$-khả tích, vì $fh \in \mathcal{K}(X; F)$ đối với mọi hàm $h \in \mathcal{K}(X; \mathbf{R})$ bằng 1 trên $S$ (Ch. III, §1, No. 2, Bổ đề 1). Chính xác hơn:

#### Mệnh đề 14 {#int-iv-s4-prop-14 .statement}

— Cho X là một không gian địa phương compact, F là một không gian Banach không bằng 0; trang bị cho không gian $\mathcal{C}(X; F)$ gồm tất cả các ánh xạ liên tục từ X vào F tôpô của sự hội tụ compact. Đối với một độ đo $\mu$ trên X, điều kiện cần và đủ để ánh xạ tuyến tính $f \mapsto \int f d\mu$ của $\mathcal{K}(X; F)$ vào F có thể mở rộng thành một ánh xạ tuyến tính liên tục của $\mathcal{C}(X; F)$ vào F là $\operatorname{Supp}(\mu)$ compact; sự mở rộng như vậy là duy nhất và trùng với tích phân được định nghĩa ở No. 1.

Ta vừa thấy rằng nếu $\mu$ có hỗ trợ compact, thì tích phân $\int f d\mu$ được định nghĩa cho mọi hàm $f \in \mathcal{C}(X; F)$ và rằng ánh xạ $f \mapsto \int f d\mu$ của $\mathcal{C}(X; F)$ vào F liên tục đối với tôpô của sự hội tụ compact. Ngược lại, giả sử rằng $f \mapsto \int f d\mu$ liên tục trên $\mathcal{K}(X; F)$ đối với tôpô của sự hội tụ compact. Khi đó, có một tập compact $K \subset X$ và một số $a > 0$ sao cho $|\mu(f)| \leq a \cdot \sup_{x \in K} |f(x)|$ đối với mọi hàm $f \in \mathcal{K}(X; F)$; đặc biệt, nếu hỗ trợ của $g \in \mathcal{K}(X; F)$ không giao với K, thì $\mu(g) = 0$. Lấy $g = h a$, trong đó $a \neq 0$ là một vectơ trong F và $h \in \mathcal{K}(X; \mathbf{C})$, ta thấy rằng $\mu(h) = 0$ đối với mọi hàm $h \in \mathcal{K}(X; \mathbf{C})$ có hỗ trợ không giao với K, điều này chứng tỏ rằng $\operatorname{Supp}(\mu) \subset K$. Cuối cùng, tính duy nhất của mở rộng suy ra từ thực tế là $\mathcal{K}(X; F)$ trù mật trong $\mathcal{C}(X; F)$ đối với tôpô của sự hội tụ compact (Ch. III, §1, No. 2, Mệnh đề 4).

Mệnh đề 14 cho phép đồng nhất một độ đo trên X có hỗ trợ compact với phần mở rộng liên tục của nó đến $\mathcal{C}(X; \mathbf{C})$. Do đó, tập các độ đo trên X có hỗ trợ compact có thể được đồng nhất với đối ngẫu $\mathcal{C}'(X; \mathbf{C})$ của không gian lồi địa phương Hausdorff $\mathcal{C}(X; \mathbf{C})$. Nhắc lại rằng $\mathcal{C}(X; \mathbf{C})$ đầy đủ (GT, X, §1, No. 6, Hệ quả 3 của Định lý 2), nhưng không nhất thiết là barreled (Bài tập 17). Tuy nhiên, nếu X đếm được ở vô cực, do đó là hợp của một dãy tăng các tập compact $K_n$ sao cho $K_n \subset \overset{\circ}{K}_{n+1}$, thì tôpô của $\mathcal{C}(X; \mathbf{C})$ có thể được xác định bởi họ đếm được các nửa chuẩn $p_n(f) = \sup_{x \in K_n} |f(x)|$, do đó $\mathcal{C}(X; \mathbf{C})$ là một không gian Fréchet trong trường hợp này. Do đó, với mọi phủ $\mathcal{G}$ của $\mathcal{C}(X; \mathbf{C})$ bởi các tập bị chặn, không gian $\mathcal{C}'(X; \mathbf{C})$ khi đó là quasi-đầy đủ đối với tôpô $\mathcal{G}$ (TVS, III, §4, No. 2, Hệ quả 4 của Định lý 1).

Trước hết ta sẽ xét trên $\mathcal{C}'(X; \mathbf{C})$ tôpô của sự hội tụ compact (tôpô của sự hội tụ đều trên các tập compact của $\mathcal{C}(X; \mathbf{C})$). Nhắc lại rằng các tập con tương đối compact H của $\mathcal{C}(X; \mathbf{C})$ được đặc trưng bởi các tính chất sau (GT, X, §2, No. 5, Hệ quả 3 của Định lý 2):

$1^\circ$ H là đồng đều liên tục;

$2^\circ$ với mọi $x \in X$, tập $H(x)$ gồm các $f(x)$, khi $f$ chạy qua H, là bị chặn trong $\mathbf{C}$.

#### Mệnh đề 15 {#int-iv-s4-prop-15 .statement}

— Cho X là một không gian địa phương compact và, với mọi $x \in X$, cho $\varepsilon_x$ là độ đo Dirac tại điểm x. Ánh xạ $x \mapsto \varepsilon_x$ của X vào $\mathcal{C}'(X; \mathbf{C})$ liên tục đối với tôpô của sự hội tụ compact trên $\mathcal{C}'(X; \mathbf{C})$.

Xét một lân cận của $\varepsilon_{x_0}$ trong $\mathcal{C}'(X; \mathbf{C})$ đối với tôpô này, mà ta có thể giả sử được xác định bằng cách lấy một số $\delta > 0$, một tập con compact H của $\mathcal{C}(X; \mathbf{C})$, và xét tập các độ đo $\mu$ trên X có giá compact sao cho $|\mu(f) - \varepsilon_{x_0}(f)| \leq \delta$ với mọi hàm $f \in H$. Vì H đều liên tục, tồn tại một lân cận U của $x_0$ trong X sao cho quan hệ $f \in H$ kéo theo $|f(x) - f(x_0)| \leq \delta$ với mọi $x \in U$, điều này cũng có thể viết là $|\varepsilon_x(f) - \varepsilon_{x_0}(f)| \leq \delta$ và chứng minh mệnh đề.(*)

#### Mệnh đề 16 {#int-iv-s4-prop-16 .statement}

— Cho K là một tập con compact của X, L là không gian vectơ của các độ đo $\mu$ trên X có giá nằm trong K. Trên L, các tôpô cảm sinh bởi tôpô $\mathcal{T}$ của sự hội tụ compact trên $\mathcal{C}'(X; \mathbf{C})$ và tôpô $\mathcal{T}'$ của sự hội tụ compact chặt trên $\mathcal{M}(X; \mathbf{C})$ (Ch. III, §1, No. 10) trùng nhau.

Hiển nhiên là trên L, tôpô cảm sinh bởi $\mathcal{T}$ mịn hơn tôpô cảm sinh bởi $\mathcal{T}'$. Ngược lại, cho H là một tập con compact của $\mathcal{C}(X; \mathbf{C})$, h là một hàm trong $\mathcal{K}(X; \mathbf{C})$ bằng 1 trên K. Hiển nhiên tập H' gồm các hàm fh, khi f chạy qua H, là compact chặt trong $\mathcal{K}(X; \mathbf{C})$, và, với mọi độ đo $\mu \in L$, $\mu(f) = \mu(fh)$ với mọi hàm $f \in H$, do đó suy ra kết luận.

#### Hệ quả 1 {#int-iv-s4-prop-16-cor-1 .statement}

— Với mọi tập con compact K của X và mọi số $a > 0$, tập B gồm các độ đo $\mu$ trên X sao cho $\operatorname{Supp}(\mu) \subset K$ và $\| \mu \| \leq a$ là một tập con đều liên tục của $\mathcal{C}'(X; \mathbf{C})$ và compact đối với tôpô $\mathcal{T}$ của sự hội tụ compact.

Thật vậy, cho H là một tập con của $\mathcal{C}(X; \mathbf{C})$ gồm các hàm bị chặn đều trên K; tồn tại một số $c > 0$ sao cho $|\mu(f)| \leq c \cdot \| \mu \| \leq ac$ với mọi hàm $f \in H$ và mọi độ đo $\mu \in B$, nhờ (22); do đó $B \subset acH^\circ$ trong đối ngẫu $\mathcal{C}'(X; \mathbf{C})$ của $\mathcal{C}(X; \mathbf{C})$, điều này chứng minh tính đều liên tục của B; thực tế là B compact đối với $\mathcal{T}$ suy ra từ thực tế là, trên B, $\mathcal{T}$ và tôpô mơ hồ cảm sinh cùng một tôpô (Mệnh đề 16 và Ch. III, §1, No. 10, Mệnh đề 17) và thực tế là B compact theo tôpô mơ hồ (Ch. III, §1, No. 9, Hệ quả 2 của Mệnh đề 15 và §2, No. 2, Mệnh đề 6).

#### Hệ quả 2 {#int-iv-s4-prop-16-cor-2 .statement}

— Mọi độ đo có giá compact (resp. mọi độ đo dương có giá compact) $\mu$ đều nằm trong bao đóng của $\mathcal{C}'(X; \mathbf{C})$, đối với tôpô $\mathcal{T}$ của sự hội tụ compact, của tập các độ đo (resp.

(*) Thực ra, ánh xạ $x \mapsto \varepsilon_x$ là một đồng phôi của X vào $\mathcal{C}'(X; \mathbf{C})$ (Ch. VI, §1, No. 6, Nhận xét 1).

các độ đo dương) có giá hữu hạn và nằm trong $\operatorname{Supp}(\mu)$ và có chuẩn bằng $\| \mu \|$.

Thật vậy, trên tập B gồm các độ đo $\nu$ sao cho $\mathrm{Supp}(\nu) \subset \mathrm{Supp}(\mu)$ và $\| \nu \| \leq \| \mu \|$, tôpô cảm sinh bởi tôpô mơ hồ trùng với tôpô cảm sinh bởi $\mathcal{T}$, và do đó hệ quả suy ra từ Ch. III, §2, No. 4, Hệ quả 2 và 3 của Định lý 1.

### 9. Các họ và các hàm tập cộng tính

#### Định nghĩa 3 {#int-iv-s4-def-3 .statement}

*Một tập hợp khác rỗng $\Phi$ gồm các tập con của một tập hợp $A$ được gọi là một clan nếu tồn tại một đại số $\mathcal{A}$ (trên $\mathbf{R}$) gồm các hàm giá trị thực xác định trên $A$, sao cho các quan hệ $M \in \Phi$ và $\varphi_M \in \mathcal{A}$ là tương đương.*

#### Ví dụ {#int-iv-s4-n9-exa-1 .statement}

Nếu $\mu$ là một độ đo trên một không gian compact địa phương $X$ thì các tổ hợp tuyến tính, với hệ số thực, của các hàm đặc trưng của các tập hợp khả tích lập thành một *đại số* $\mathcal{A}$, vì, với bất kỳ hai tập hợp khả tích nào $M, N$, hàm $\varphi_M \varphi_N = \varphi_{M \cap N}$ là khả tích (No. 5, Mệnh đề 7); do đó suy ra từ Định nghĩa 2 và 3 rằng tập hợp các tập con khả tích của $X$ là một clan.

#### Mệnh đề 17 {#int-iv-s4-prop-17 .statement}

*Để một tập hợp khác rỗng $\Phi$ gồm các tập con của một tập hợp $A$ là một clan, cần và đủ là nó thỏa mãn điều kiện sau:*

(CL) *Với mọi cặp tập hợp $M, N$ thuộc $\Phi$, các tập hợp $M \cup N$ và $M \cap \mathbf{C}N$ thuộc $\Phi$.*¹

Điều kiện này là *cần thiết*, do các hệ thức

$$
\varphi_{M \cup N} = \varphi_M + \varphi_N - \varphi_M \varphi_N , \quad \varphi_{M \cap \mathbf{C}N} = \varphi_M - \varphi_M \varphi_N .
$$

Để chứng minh rằng nó *đủ*, trước hết ta nhận thấy rằng điều đó kéo theo: với bất kỳ hai tập hợp $M, N$ trong $\Phi$, $M \cap N$ thuộc $\Phi$ vì $M \cap N = M \cap \mathbf{C}(M \cap \mathbf{C}N)$. Đặt $\mathcal{E}(\Phi)$ là tập hợp các tổ hợp tuyến tính, với hệ số thực, của các hàm đặc trưng của các tập hợp của $\Phi$. Vì $\varphi_M \varphi_N = \varphi_{M \cap N}$, $\mathcal{E}(\Phi)$ là một đại số. Mọi việc quy về chứng minh rằng nếu $M$ là một tập con của $A$ sao cho $\varphi_M = \sum_i c_i \varphi_{M_i}$, trong đó các $M_i$ thuộc $\Phi$, thì $M \in \Phi$. Điều này sẽ suy ra từ bổ đề sau:

#### Bổ đề {#int-iv-s4-n9-lem-1 .statement}

*Cho $\Phi$ là một tập hợp khác rỗng các tập con của $A$ thỏa mãn tiên đề (CL). Cho một họ hữu hạn $(M_i)_{1 \leq i \leq n}$ các tập hợp trong $\Phi$, tồn tại một*

¹ Một clan $\Phi$ của các tập con của một tập hợp $A$ còn được gọi là một *vành* (hay *vành Boole*) của các tập hợp; nếu, hơn nữa, $A \in \Phi$, thì $\Phi$ được gọi là một *đại số* (hay *đại số Boole*) của các tập hợp (xem GT, I, §6, Bài tập 20 và II, §4, Bài tập 12). Một đại số Boole đóng dưới các hợp đếm được được gọi là một *tribu*, hay *$\sigma$*-*đại số* (GT, IX, §6, No. 3, Định nghĩa 3).

họ hữu hạn $(N_j)_{1 \leq j \leq m}$ các tập hợp từng đôi một rời nhau trong $\Phi$ sao cho mỗi $M_i$ là hợp của một số nào đó các $N_j$.

Thật vậy, xét $2^n - 1$ tập có dạng $\bigcap_{i=1}^n P_i$, trong đó $P_i = M_i$ với một số chỉ số $i$ nào đó, $P_i = \mathbf{C} M_i$ với các chỉ số còn lại, với ít nhất một trong các $P_i$ bằng $M_i$. Gọi $(N_j)_{1 \leq j \leq m}$ là dãy các tập này được sắp theo một thứ tự nào đó; chúng đôi một rời nhau và thuộc $\Phi$; mặt khác, mọi tập $M_k$ đều là hợp của các tập $N_j = \bigcap_{i=1}^n P_i$ tương ứng với các họ $(P_i)$ sao cho $P_k = M_k$, điều này chứng minh bổ đề.

Bổ đề đã được chứng minh, mọi hàm có dạng $\sum_{i=1}^n c_i \varphi_{M_i}$, trong đó $M_i \in \Phi$, đều có thể viết dưới dạng $\sum_{j=1}^m d_j \varphi_{N_j}$, trong đó các $N_j$ thuộc $\Phi$ và đôi một rời nhau; nếu $\varphi_M = \sum_{j=1}^m d_j \varphi_{N_j}$ thì tất yếu $d_j = 0$ hoặc $d_j = 1$ với mỗi chỉ số $j$, do đó $M$ là hợp của một số nào đó trong các $N_j$, và vì thế thuộc $\Phi$.

Mỗi họ $\Phi$ các tập con của $A$ đều chứa tập con rỗng $\varnothing$ của $A$; vì tồn tại ít nhất một tập con $M \in \Phi$, do đó $M - M = \varnothing$ thuộc $\Phi$. Cũng chú ý rằng tập các tập con của $A$ chỉ gồm tập con $\varnothing$ là một họ.

#### Định nghĩa 4 {#int-iv-s4-def-4 .statement}

*Cho một họ $\Phi$ các tập con của một tập $A$, và một không gian Banach $F$, người ta gọi* hàm bậc thang² *trên các tập của $\Phi$ (hay hàm bậc thang $\Phi$), nhận giá trị trong $F$, mọi hàm có dạng* $\sum_i a_i \varphi_{M_i}$, *trong đó các $a_i$ thuộc $F$, và các $M_i$ thuộc $\Phi$.*

Rõ ràng tập $\mathcal{E}_F(\Phi)$ các hàm bậc thang $\Phi$ nhận giá trị trong $F$ là một không gian vectơ trên $\mathbf{R}$ hoặc $\mathbf{C}$. Ta vừa thấy trong Mệnh đề 17 rằng tập $\mathcal{E}(\Phi)$ các hàm bậc thang nhận giá trị thực là một *đại số* trên $\mathbf{R}$; nó cũng là không gian con tuyến tính của $\mathbf{R}^A$ sinh bởi các hàm đặc trưng của các tập của $\Phi$.

Theo Bổ đề, mọi hàm trong $\mathcal{E}_F(\Phi)$ đều có thể viết $f = \sum_j c_j \varphi_{N_j}$, trong đó các $N_j \in \Phi$ đôi một rời nhau; từ đó suy ra rằng $|f| = \sum_j |c_j| \varphi_{N_j}$ thuộc $\mathcal{E}(\Phi)$. Đặc biệt, $\mathcal{E}(\Phi)$ là một *không gian Riesz*, vì cận trên của hai hàm trong $\mathcal{E}(\Phi)$ thuộc $\mathcal{E}(\Phi)$.

#### Nhận xét {#int-iv-s4-n9-rem-1 .statement}

— Dễ thấy rằng Định nghĩa 4 tương đương với phát biểu sau đây: một hàm bậc thang $\Phi$ với giá trị trong $F$ là một hàm $f$ chỉ nhận một số hữu hạn giá trị và sao cho, với mọi $a \neq 0$ trong $F$, tập $f(a)^{-1}$ thuộc $\Phi$.

² Hàm bậc thang, do đó ký hiệu $\mathcal{E}(\Phi)$ trong phần sau.

#### Định nghĩa 5 {#int-iv-s4-def-5 .statement}

— *Một hàm nhận giá trị thực* $\lambda$ *xác định trên một họ* $\Phi$ *gồm các tập con của một tập hợp* $A$ *được gọi là cộng tính nếu, với mọi cặp* $M, N$ *của các tập rời nhau thuộc* $\Phi$, $\lambda(M \cup N) = \lambda(M) + \lambda(N)$.

Từ định nghĩa này suy ra ngay rằng $\lambda(\varnothing) = 0$.

#### Mệnh đề 18 {#int-iv-s4-prop-18 .statement}

— *Cho* $\lambda$ *là một hàm tập hợp cộng tính xác định trên một họ* $\Phi$. *Tồn tại một và chỉ một dạng tuyến tính* (cũng ký hiệu $\lambda$) *trên không gian vectơ* $\mathcal{E}(\Phi)$ *của các hàm bậc thang* $\Phi$* nhận giá trị thực*, *sao cho* $\lambda(\varphi_M) = \lambda(M)$ *với mọi tập hợp* $M \in \Phi$; *nếu, hơn nữa,* $\lambda(M) \geqslant 0$ *với mọi* $M \in \Phi$, *thì* $\lambda$ *là một dạng tuyến tính dương trên* $\mathcal{E}(\Phi)$.

*Tính duy nhất* của dạng tuyến tính $\lambda$ là hiển nhiên, vì các hàm đặc trưng của các tập trong $\Phi$ sinh ra không gian vectơ $\mathcal{E}(\Phi)$. Để chứng minh *sự tồn tại* của $\lambda$, chỉ cần chứng minh rằng hệ thức $\sum_i c_i \varphi_{M_i} = 0$, trong đó các $M_i$ là các tập khác rỗng thuộc $\Phi$, suy ra $\sum_i c_i \lambda(M_i) = 0$.

Bây giờ, theo Bổ đề, tồn tại một họ hữu hạn $(N_j)$ gồm các tập khác rỗng đôi một rời nhau trong $\Phi$ sao cho, với mọi chỉ số $i$, $\varphi_{M_i} = \sum_j a_{ij} \varphi_{N_j}$ với $a_{ij} = 0$ hoặc $a_{ij} = 1$. Hệ thức $\sum_i c_i \varphi_{M_i} = 0$, có thể viết thành $\sum_j \left( \sum_i c_i a_{ij} \right) \varphi_{N_j} = 0$, do đó suy ra rằng $\sum_i c_i a_{ij} = 0$ với mọi chỉ số $j$. Theo Định nghĩa 5, ta có

$$
\sum_i c_i \lambda(M_i) = \sum_j \left( \sum_i c_i a_{ij} \right) \lambda(N_j) = 0,
$$

mà điều này chứng minh sự tồn tại của $\lambda$. Sau cùng, giả sử rằng $\lambda(M) \geqslant 0$ đối với mọi $M \in \Phi$; với mọi hàm $f \in \mathcal{E}(\Phi)$, ta có thể viết $f = \sum_i c_i \varphi_{M_i}$, trong đó các $M_i \in \Phi$ từng đôi một rời nhau; nếu $f \geqslant 0$, suy ra rằng $c_i \geqslant 0$ đối với mọi chỉ số $i$ sao cho $M_i$ khác rỗng, do đó $\lambda(f) = \sum_i c_i \lambda(M_i) \geqslant 0$.

### 10. Xấp xỉ các hàm liên tục bởi các hàm bậc thang

#### Mệnh đề 19 {#int-iv-s4-prop-19 .statement}

— *Cho* $X$ *là một không gian địa phương compact,* $\Phi$ *một họ các tập con của* $X$, *chứa tập hợp các tập con compact của* $X$. *Với mọi ánh xạ liên tục* $f$ *từ* $X$ *vào một không gian Banach* $F$ *(tức là, mọi hàm liên tục, giá trị thực* $f \geqslant 0$ *trên* $X$) *có giá đỡ compact* $K$, *tồn tại một dãy* $(g_n)$ *các hàm trong* $\mathcal{E}_F(\Phi)$ *có giá đỡ được chứa trong* $K$ *(tức là một dãy* $(g_n)$ *các hàm trong* $\mathcal{E}(\Phi)$ *sao cho* 0 \leqslant g_n \leqslant f *đối với mọi* n) *hội tụ đều đến* $f$ *(tức là* $f$).

Vì $f$ liên tục đều trên $K$, ta có thể phủ $K$ bởi một số hữu hạn các tập compact $M_i$ ($1 \leq i \leq m$) sao cho dao động của $f$ trên mỗi $M_i$ là $\leq 1/n$. Vì các $M_i$ và $K$ thuộc $\Phi$, tồn tại một phân hoạch của $K$ thành các tập $N_j \in \Phi$ sao cho mỗi tập $M_i \cap K$ là hợp của một số nhất định các $N_j$ (No. 9, Bổ đề). Cho $a_j$ là một phần tử của $F$ sao cho $|f(x) - a_j| \leq 1/n$ trên $N_j$. Đặt $g_n = \sum_j a_j \varphi_{N_j}$, ta có $|f - g_n| \leqslant 1/n$, do đó mệnh đề trong trường hợp này. Ta lập luận tương tự đối với một hàm liên tục giá trị thực $f$, bằng cách lấy $a_j = \inf_{x \in N_j} f(x)$ và $g_n = \sum_j a_j \varphi_{N_j}$.

#### Hệ quả 1 {#int-iv-s4-prop-19-cor-1 .statement}

*Cho $\mu$ là một độ đo trên $X$; không gian $\mathcal{E}_F(\Phi)$ trù mật trong mỗi không gian của các không gian $\mathcal{L}_F^p$ ($1 \leq p < +\infty$).*

Vì, từ Mệnh đề 19 và tiêu chuẩn hội tụ theo trung bình cho các giới hạn đều của các hàm có giá compact (§ 3, No. 3, Mệnh đề 4) suy ra rằng $\mathcal{E}_F(\Phi)$ là trù mật, đối với tôpô của sự hội tụ theo trung bình cấp $p$, trong bao đóng của không gian $\mathcal{K}_F$ gồm các hàm liên tục có giá compact, do đó suy ra hệ quả.

#### Hệ quả 2 {#int-iv-s4-prop-19-cor-2 .statement}

*Với mọi tập con đóng $S$ của $X$, mọi hàm $f \in \mathcal{K}(X, S; \mathbf{C})$ là giới hạn đều của các tổ hợp tuyến tính $\sum_i \lambda_i \varphi_{K_i}$, trong đó các $\lambda_i$ thuộc $\mathbf{C}$ và các $K_i$ là các tập con compact của $S$.*

Tập $\mathcal{A}$ gồm những tổ hợp tuyến tính như vậy là một $\mathbf{C}$-đại số. Cho $\Phi$ là tập các tập con $M$ của $X$ sao cho $\varphi_M \in \mathcal{A}$; do đó $\Phi$ là một *clan* mà mọi phần tử của nó đều là các tập con của S, chứa các tập compact của $S$, và $\mathcal{E}_C(\Phi) \subset \mathcal{A}$. Khi đó chỉ cần áp dụng Mệnh đề 19 cho không gian địa phương compact $S$ và *clan* $\Phi$.

#### Hệ quả 3 {#int-iv-s4-prop-19-cor-3 .statement}

*Nếu $\mu$ và $\nu$ là hai độ đo trên $X$ sao cho $\mu(K) = \nu(K)$ với mọi tập con compact $K$ của $X$, thì $\mu = \nu$.*

Vì, từ Hệ quả 2 và định nghĩa của một độ đo suy ra rằng, với mọi tập con compact $S$ của $X$, $\mu$ và $\nu$ nhận cùng giá trị trên $\mathcal{K}(X, S; \mathbf{C})$.

### 11. Mở rộng một độ đo xác định trên một họ các tập hợp

Cho $\Phi$ là một tập khác rỗng các tập con của một không gian địa phương compact $X$. Cho một hàm nhận giá trị thực $M \mapsto \alpha(M)$, được xác định và $\geq 0$ trên $\Phi$, ta sẽ tìm các điều kiện dưới đó tồn tại một độ đo dương $\mu$ trên $X$ sao cho các tập thuộc $\Phi$ là $\mu$-tích phân và $\mu(M) = \alpha(M)$ với mọi $M \in \Phi$. Ta sẽ giới hạn ở việc xét trường hợp tập $\Phi$ thỏa các điều kiện sau:

(PC_I) *Hợp và giao của hai tập thuộc $\Phi$ đều thuộc $\Phi$.*

(PC_{II}) *Với mọi cặp gồm một tập compact K và một tập mở U trong X sao cho $K \subset U$, tồn tại một tập $M \in \Phi$ sao cho $K \subset M \subset U$.*

Chú ý rằng điều kiện (PC_{II}) suy ra rằng $\varnothing \in \Phi$, bằng cách lấy $K = U = \varnothing$. Tuy nhiên, tập $\Phi$ không nhất thiết là một *clan*; chẳng hạn, tập tất cả các tập compact của $X$ thỏa các điều kiện (PC_I) và (PC_{II}), nhưng nói chung không phải là một *clan*, vì nếu M và N là compact, thì điều đó nói chung không đúng với $M \cap \mathbf{C}N$.

Ta còn giả sử rằng hàm $\alpha$ được xác định trên $\Phi$ thỏa các điều kiện sau (hiển nhiên là cần thiết để bài toán có nghiệm):

(PM_I) *Quan hệ $M \subset N$ suy ra $\alpha(M) \leq \alpha(N)$.*
(PM_{II}) *Với mọi M và N trong $\Phi$, $\alpha(M \cup N) \leq \alpha(M) + \alpha(N)$.*
(PM_{III}) *Quan hệ $M \cap N = \varnothing$ suy ra $\alpha(M \cup N) = \alpha(M) + \alpha(N)$.*

Lấy $N = \varnothing$ trong điều kiện (PM_{III}), suy ra $\alpha(\varnothing) = 0$; điều kiện (PM_I) khi đó cho thấy $\alpha(M) \geq 0$ với mọi $M \in \Phi$.

#### Định lý 5 {#int-iv-s4-thm-5 .statement}

*Cho $\Phi$ là một tập các tập con của một không gian X địa phương compact, thỏa mãn (PC_I) và (PC_{II}), và cho $\alpha$ là một hàm nhận giá trị thực, xác định trên $\Phi$, thỏa mãn các điều kiện (PM_I), (PM_{II}) và (PM_{III}). Để tồn tại một độ đo dương $\mu$ trên X sao cho các tập của $\Phi$ là $\mu$-khả tích và $\mu(M) = \alpha(M)$ với mọi $M \in \Phi$, thì cần và đủ để $\alpha$ còn thỏa mãn thêm điều kiện sau:*

(PM_{IV}) *Với mọi $\varepsilon > 0$ và mọi $M \in \Phi$, tồn tại một tập compact $K \subset M$ và một tập mở $U \supset M$ sao cho, với mọi $N \in \Phi$ thỏa mãn quan hệ $K \subset N \subset U$, ta có $|\alpha(N) - \alpha(M)| \leq \varepsilon$.*

*Hơn nữa, nếu điều kiện (PM_{IV}) được thỏa mãn, thì độ đo $\mu$ là duy nhất; với mọi tập compact $K$, $\mu(K) = \inf_{M \in \Phi, M \supset K} \alpha(M)$; với mọi tập mở $U$, $\mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M)$. \*

Chú ý rằng điều kiện (PM_{IV}) tương đương với phép hội của hai điều kiện sau:

(PM'_{IV}) *Với mọi $\varepsilon > 0$ và mọi $M \in \Phi$, tồn tại một tập mở $U \supset M$ sao cho, với mọi $N \in \Phi$ được chứa trong $U$, $\alpha(N) \leq \alpha(M) + \varepsilon$.*
(PM''_{IV}) *Với mọi $\varepsilon > 0$ và mọi $M \in \Phi$, tồn tại một tập compact $K \subset M$ sao cho, với mọi $N \in \Phi$ chứa $K$, $\alpha(N) \geq \alpha(M) - \varepsilon$.*

Vì hiển nhiên, (PM'_{IV}) và (PM''_{IV}) suy ra (PM_{IV}). Ngược lại, chẳng hạn hãy chứng minh rằng (PM_{IV}) suy ra (PM'_{IV}): cho K là một tập compact và U là một tập mở sao cho $K \subset M \subset U$ và $|\alpha(P) - \alpha(M)| \leq \varepsilon$ với mọi $P \in \Phi$ thỏa mãn $K \subset P \subset U$. Khi đó, nếu $N \in \Phi$ và $N \subset U$, thì $M \cup N$ thuộc $\Phi$ và $K \subset M \cup N \subset U$, do đó $\alpha(M \cup N) \leq \alpha(M) + \varepsilon$ và *a fortiori* $\alpha(N) \leq \alpha(M) + \varepsilon$.

Khi tập $\Phi$, thỏa mãn (PC_I) và (PC_{II}), gồm các tập *compact*, thì điều kiện (PM''_{IV}) được thỏa mãn hiển nhiên, và khi đó (PM_{IV}) tương đương với (PM'_{IV}).

Điều kiện (PM_{IV}) là *cần*: điều này suy ra ngay từ Định lý 4 của No. 6 về sự 'xấp xỉ' của một tập khả tích bởi một tập compact và một tập mở. Để chứng minh các khẳng định khác của định lý, ta tiến hành theo nhiều bước.

1° Định nghĩa một tôpô trên $\mathfrak{P}(X)$.

Với mọi cặp $(K, U)$ gồm một tập compact $K$ và một tập mở $U$ trong $X$, ta ký hiệu $I(K, U)$ là tập hợp các tập con $M \subset X$ sao cho $K \subset M \subset U$; để $I(K, U)$ khác rỗng, cần và đủ là $K \subset U$. Nếu $(K', U')$ là một cặp thứ hai, được tạo bởi một tập compact $K'$ và một tập mở $U'$, ta có
$$
I(K, U) \cap I(K', U') = I(K \cup K', U \cap U').
$$
Cho $T$ là tôpô trên $\mathfrak{P}(X)$ được sinh bởi tập các tập con $I(K, U)$ khi $K$ chạy qua tập các tập compact của $X$, và $U$ chạy qua tập các tập mở của $X$; theo trên, các $I(K, U)$ lập thành một cơ sở cho tôpô $T$ (GT, I, §1, No. 3).

Ta thấy rằng định nghĩa của $T$ kéo theo rằng, trong $\mathfrak{P}(X)$, tập hợp các tập compact của $X$ là trù mật. Điều kiện (PC_{II}) phát biểu rằng $\Phi$ là trù mật trong $\mathfrak{P}(X)$, và điều kiện (PM_{IV}) phát biểu rằng hàm $\alpha$ liên tục trên $\Phi$ đối với tôpô cảm sinh bởi $T$. Cuối cùng, Định lý 4 của No. 6 phát biểu rằng hàm $M \mapsto \mu(M)$ liên tục trên lớp các tập $\mu$-khả tích, đối với tôpô cảm sinh bởi $T$.

2° Tính duy nhất của $\mu$.

Ta ký hiệu $\overline{\Phi}$ là tập hợp các tập con $M \subset X$ sao cho $\alpha(N)$ tiến tới một giới hạn hữu hạn khi $N$ tiến tới $M$ (đối với tôpô $T$) trong khi vẫn ở trong $\Phi$; khi đó ta chỉ có thể mở rộng $\alpha$ theo một cách thành một ánh xạ liên tục $\overline{\alpha}$ từ $\overline{\Phi}$ vào $\mathbf{R}$ (GT, I, §8, No. 5, Th. 1). Nếu tồn tại một độ đo $\mu$ thỏa mãn các yêu cầu, thì các nhận xét trên chứng minh rằng lớp $\Psi$ của các tập $\mu$-khả tích được chứa trong $\overline{\Phi}$ và rằng $\mu(M) = \overline{\alpha}(M)$ với mọi $M \in \Psi$; quan hệ này đặc biệt đúng với mọi tập compact $M$ của $X$, điều đó chứng minh tính duy nhất của $\mu$ (No. 10, Hệ quả 3 của Mệnh đề 19).

3° Mở rộng $\alpha$ đến các tập compact.

Không giả sử sự tồn tại của $\mu$, ta nay sẽ khảo sát tập $\overline{\Phi}$ và mở rộng $\overline{\alpha}$ của $\alpha$ lên $\overline{\Phi}$. Trước hết ta chứng minh rằng mọi tập compact $K$ đều thuộc $\overline{\Phi}$ và $\overline{\alpha}(K) = \inf_{P \in \Phi, P \supset K} \alpha(P)$. Đặt $a = \inf_{P \in \Phi, P \supset K} \alpha(P)$; với mọi $\varepsilon > 0$, tồn tại $M \in \Phi$ sao cho $K \subset M$ và $\alpha(M) \leq a + \varepsilon$. Theo (PM'_{IV}), tồn tại một tập mở $U \supset M$ sao cho, với mọi $N \in \Phi$ được chứa trong $U$, ta có $\alpha(N) \leq \alpha(M) + \varepsilon \leq a + 2\varepsilon$; do đó, với mọi $N \in \Phi$ sao cho $K \subset N \subset U$, ta suy ra $a \leq \alpha(N) \leq a + 2\varepsilon$, điều này, theo các định nghĩa, cho thấy $K \in \overline{\Phi}$ và $\overline{\alpha}(K) = a$.

Kết quả này lập tức chứng minh rằng nếu $K_1$ và $K_2$ là hai tập compact sao cho $K_1 \subset K_2$, thì $\overline{\alpha}(K_1) \leq \overline{\alpha}(K_2)$. Nếu $K_1$ và $K_2$ là bất kỳ hai tập compact nào, ta có $\overline{\alpha}(K_1 \cup K_2) \leq \overline{\alpha}(K_1) + \overline{\alpha}(K_2)$ theo (PM_{II}). Hơn nữa, ta sẽ thấy rằng nếu $K_1$ và $K_2$ rời nhau thì $\overline{\alpha}(K_1 \cup K_2) = \overline{\alpha}(K_1) + \overline{\alpha}(K_2)$. Thật vậy, khi đó tồn tại hai tập mở rời nhau $U_1, U_2$ sao cho $K_1 \subset U_1$, $K_2 \subset U_2$ (GT, II, §4, Mệnh đề 4). Vì thế, theo (PC_{II}), cũng tồn tại hai tập $M_1 \in \Phi$, $M_2 \in \Phi$ sao cho $K_1 \subset M_1 \subset U_1$ và $K_2 \subset M_2 \subset U_2$. Bây giờ lấy $P$ là bất kỳ tập nào của $\Phi$ chứa $K_1 \cup K_2$; hợp của hai tập $P \cap M_1$ và $P \cap M_2$ thuộc $\Phi$ theo (PC_{I}), và vì hai tập này rời nhau, áp dụng (PM_I) và (PM_{III}) suy ra

$$
\alpha(P) \geq \alpha(P \cap M_1) + \alpha(P \cap M_2) \geq \overline{\alpha}(K_1) + \overline{\alpha}(K_2),
$$

điều đó chứng minh mệnh đề của chúng ta.

**4° Mở rộng của $\alpha$ tới các tập mở.**

Ta sẽ thấy rằng, để một tập mở $U$ thuộc $\overline{\Phi}$, cần và đủ là, khi $K$ chạy qua tập các tập con compact của $U$, cận trên đúng của các số $\overline{\alpha}(K)$ là hữu hạn; hơn nữa, khi đó $\overline{\alpha}(U)$ bằng cận trên đúng này.

Cho $U$ là một tập mở thuộc $\overline{\Phi}$; với mọi $\varepsilon > 0$ tồn tại một tập compact $K \subset U$ sao cho, với mọi tập $M \in \Phi$ thỏa mãn $K \subset M \subset U$, ta có $|\overline{\alpha}(U) - \alpha(M)| \leq \varepsilon$, do đó $|\overline{\alpha}(U) - \overline{\alpha}(K)| \leq \varepsilon$; mặt khác, nếu $K'$ là bất kỳ tập compact nào được chứa trong $U$, thì $K \subset K \cup K' \subset U$, do đó $|\overline{\alpha}(U) - \overline{\alpha}(K \cup K')| \leq \varepsilon$ và vì thế $\overline{\alpha}(U) \geq \overline{\alpha}(K \cup K') - \varepsilon \geq \overline{\alpha}(K') - \varepsilon$; do đó thật vậy $\overline{\alpha}(U)$ bằng cận trên đúng của các số $\overline{\alpha}(K)$ khi $K$ chạy qua tập hợp các tập con compact của $U$.

Ngược lại, cho $U$ là một tập mở sao cho $b = \sup_{K \subset U} \overline{\alpha}(K) < +\infty$ ($K$ chạy qua tập hợp các tập con compact của $U$), và hãy chứng minh rằng $U \in \overline{\Phi}$. Với mọi $\varepsilon > 0$, tồn tại một tập compact $K \subset U$ sao cho $b - \varepsilon \leq \overline{\alpha}(K) \leq b$; theo (PM''_{IV}), với mọi tập $M \in \Phi$ sao cho $K \subset M \subset U$, tồn tại một tập compact $K' \subset M$ sao cho

$$
\alpha(M) \leq \overline{\alpha}(K') + \varepsilon \leq b + \varepsilon;
$$

do đó $b - \varepsilon \leq \alpha(M) \leq b + \varepsilon$, điều đó chứng tỏ rằng $U \in \overline{\Phi}$.

Từ đặc trưng hóa này của các tập mở $U \in \overline{\Phi}$, và của $\overline{\alpha}(U)$, trước hết suy ra rằng nếu $U_1$ và $U_2$ là hai tập mở sao cho $U_1 \subset U_2$ và $U_2 \in \overline{\Phi}$, thì $U_1 \in \overline{\Phi}$ và $\overline{\alpha}(U_1) \leq \overline{\alpha}(U_2)$. Mặt khác, nếu $U_1$ và $U_2$ là hai tập mở thuộc $\overline{\Phi}$, thì điều tương tự đúng với $U_1 \cup U_2$, và $\overline{\alpha}(U_1 \cup U_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2)$. Vì, cho $K$ là bất kỳ tập compact nào được chứa trong $U_1 \cup U_2$; với mọi điểm $x \in K$, tồn tại một lân cận compact của $x$ được chứa trong một trong hai tập $U_1$ hoặc $U_2$; do đó có thể phủ $K$ bởi một số hữu hạn các lân cận này; nếu $K_1$ (tương ứng $K_2$) là hợp của những lân cận được chứa trong $U_1$ (tương ứng $U_2$), thì $K \subset K_1 \cup K_2$, do đó

$$
\overline{\alpha}(K) \leq \overline{\alpha}(K_1 \cup K_2) \leq \overline{\alpha}(K_1) + \overline{\alpha}(K_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2),
$$

điều này thiết lập tính chất đã nêu.

**5° Các tính chất của $\overline{\Phi}$ và $\overline{\alpha}$.**

Định nghĩa của $\overline{\Phi}$ và $\overline{\alpha}$ giờ có thể được biến đổi như sau (lưu ý (PC_{II})): để $M \in \overline{\Phi}$, điều kiện cần và đủ là, với mọi $\varepsilon > 0$, tồn tại một tập compact $K$ và một tập mở $U \in \overline{\Phi}$ sao cho $K \subset M \subset U$ và $\overline{\alpha}(U) - \overline{\alpha}(K) \leq \varepsilon$; hơn nữa, $\overline{\alpha}(M)$ là *cận dưới đúng* của các $\overline{\alpha}(U)$ ứng với các tập mở $U \in \overline{\Phi}$ chứa $M$, và là *cận trên đúng* của các $\overline{\alpha}(K)$ ứng với các tập compact $K \subset M$.

Từ đó, trước hết ta suy ra rằng nếu $M_1, M_2$ và $M_1 \cup M_2$ thuộc $\overline{\Phi}$, thì $\overline{\alpha}(M_1 \cup M_2) \leq \overline{\alpha}(M_1) + \overline{\alpha}(M_2)$. Thật vậy, nếu $U_1$ và $U_2$ là hai tập mở của $\overline{\Phi}$ chứa $M_1$ và $M_2$, tương ứng, và sao cho $\overline{\alpha}(U_1) \leq \overline{\alpha}(M_1) + \varepsilon$ và $\overline{\alpha}(U_2) \leq \overline{\alpha}(M_2) + \varepsilon$, thì $U_1 \cup U_2$ thuộc $\overline{\Phi}$, chứa $M_1 \cup M_2$, và do đó

$$
\overline{\alpha}(M_1 \cup M_2) \leq \overline{\alpha}(U_1 \cup U_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2) \leq \overline{\alpha}(M_1) + \overline{\alpha}(M_2) + 2\varepsilon,
$$

do đó mệnh đề của chúng ta.

Tiếp theo, ta hãy chỉ ra rằng nếu $K$ là một tập compact và $U$ là một tập mở của $\overline{\Phi}$ sao cho $K \subset U$, thì $\overline{\alpha}(U - K) = \overline{\alpha}(U) - \overline{\alpha}(K)$. Theo điều trên, ta có $\overline{\alpha}(U) \leq \overline{\alpha}(K) + \overline{\alpha}(U - K)$. Mặt khác, với mọi tập compact $K' \subset U - K$,

$$
\overline{\alpha}(K \cup K') = \overline{\alpha}(K) + \overline{\alpha}(K') \leq \overline{\alpha}(U);
$$

vì $U - K$ là mở và thuộc $\overline{\Phi}$, nên $\overline{\alpha}(U - K)$ là cận trên đúng của các $\overline{\alpha}(K')$, điều này cho thấy rằng $\overline{\alpha}(K) + \overline{\alpha}(U - K) \leq \overline{\alpha}(U)$.

Do đó, định nghĩa của $\overline{\Phi}$ giờ có thể được phát biểu theo cách sau: để $M \in \overline{\Phi}$, điều kiện cần và đủ là, với mọi $\varepsilon > 0$, tồn tại một tập compact $K$ và một tập mở $U \in \overline{\Phi}$ sao cho $K \subset M \subset U$ và $\overline{\alpha}(U - K) \leq \varepsilon$.

Bây giờ ta có thể chứng minh rằng $\overline{\Phi}$ *là một clan* và $\overline{\alpha}$ là một *hàm tập hợp cộng tính* trên $\overline{\Phi}$. Trước hết ta chứng minh rằng nếu $M$ và $N$ thuộc $\overline{\Phi}$ thì $M \cap \mathbf{C}N$ và $M \cup N$ cũng thuộc $\overline{\Phi}$. Theo giả thiết, với mọi $\varepsilon > 0$ tồn tại hai tập compact $K, K'$ và hai tập mở $U, U'$ của $\overline{\Phi}$ sao cho

$$
K \subset M \subset U,\quad K' \subset N \subset U',\quad \overline{\alpha}(U - K) \leq \varepsilon,\quad \overline{\alpha}(U' - K') \leq \varepsilon.
$$

Tập $K'' = K \cap \mathbf{C}U'$ là compact, tập $U'' = U \cap \mathbf{C}K'$ là mở và thuộc $\overline{\Phi}$, và $K'' \subset M \cap \mathbf{C}N \subset U''$; mặt khác, $U'' - K''$ được chứa trong hợp của $U \cap \mathbf{C}K$ và $U' \cap \mathbf{C}K'$, do đó $\overline{\alpha}(U'' - K'') \leq 2\varepsilon$, điều này chứng tỏ rằng $M \cap \mathbf{C}N \in \overline{\Phi}$. Tương tự, $U_1 = U \cup U'$ là mở và thuộc $\overline{\Phi}$, $K_1 = K \cup K'$ là compact, và $K_1 \subset M \cup N \subset U_1$; mặt khác, $U_1 - K_1$ được chứa trong hợp của $U - K$ và $U' - K'$, do đó lại có $\overline{\alpha}(U_1 - K_1) \leq 2\varepsilon$, và $M \cup N$ thuộc $\overline{\Phi}$. Cuối cùng, nếu $M$ và $N$ rời nhau, thì

$$
\overline{\alpha}(K_1) = \overline{\alpha}(K) + \overline{\alpha}(K') \geq \overline{\alpha}(M) + \overline{\alpha}(N) - 2\varepsilon,
$$

do đó $\overline{\alpha}(M \cup N) \geq \overline{\alpha}(M) + \overline{\alpha}(N) - 2\varepsilon$; vì $\varepsilon$ là tùy ý, ta có $\overline{\alpha}(M \cup N) = \overline{\alpha}(M) + \overline{\alpha}(N)$.

**6° Sự tồn tại của độ đo $\mu$.**

Theo Mệnh đề 18 của No. 9, tồn tại duy nhất một dạng tuyến tính dương $\beta$ trên không gian vectơ $\mathcal{E}(\overline{\Phi})$ của các hàm bậc thang $\overline{\Phi}$, sao cho $\beta(\varphi_M) = \overline{\alpha}(M)$ với mọi $M \in \overline{\Phi}$. Với mọi tập compact $K$ của $X$, ta ký hiệu bởi $\mathcal{G}(K)$ không gian các *giới hạn đều* của các hàm của $\mathcal{E}(\overline{\Phi})$ có giá đỡ được chứa trong $K$. Vì $\beta$ là dương, $|\beta(f)| \leq \overline{\alpha}(K) \cdot \|f\|$ với mọi hàm $f \in \mathcal{E}(\overline{\Phi})$ có giá đỡ được chứa trong $K$; *hạn chế* của $\beta$ lên không gian các hàm ấy là một dạng tuyến tính *liên tục* đối với tôpô hội tụ đều; do đó nó có thể được mở rộng thành một dạng tuyến tính dương *liên tục* $\overline{\beta}_K$ trên $\mathcal{G}(K)$. Hơn nữa, nếu $K \subset K_1$, thì hạn chế của $\overline{\beta}_{K_1}$ lên $\mathcal{G}(K)$ trùng với $\overline{\beta}_K$, do đó tồn tại một dạng tuyến tính dương $\overline{\beta}$ trên hợp $\mathcal{G}$ của các $\mathcal{G}(K)$, mở rộng mỗi một trong các dạng $\overline{\beta}_K$.

Bây giờ, vì mọi tập compact đều thuộc $\overline{\Phi}$, không gian $\mathcal{H}$ của các hàm liên tục nhận giá trị thực có giá đỡ compact là một *không gian con* của $\mathcal{G}$ (No. 10, Mệnh đề 19); vì thế *hạn chế* lên $\mathcal{H}$ của dạng tuyến tính dương $\overline{\beta}$ là một *độ đo* dương $\mu$. Ta hãy chứng minh rằng với mọi tập compact $K$, $\mu(K) = \overline{\alpha}(K)$. Với mọi $\varepsilon > 0$, tồn tại một tập mở $U \in \overline{\Phi}$ sao cho $K \subset U$, $\mu(U) \leq \mu(K) + \varepsilon$ và $\overline{\alpha}(U) \leq \overline{\alpha}(K) + \varepsilon$. Cho $f$ là một ánh xạ liên tục của $X$ vào $[0, 1]$ có giá đỡ được chứa trong $U$ và sao cho $f(x) = 1$ trên $K$ (Ch. III, §1, No. 2, Bổ đề 1). Khi đó $\mu(K) \leq \mu(f) \leq \mu(U) \leq \mu(K) + \varepsilon$, và, mặt khác,

$$
\overline{\alpha}(K) = \beta(\varphi_K) \leq \overline{\beta}(f) \leq \beta(\varphi_U) = \overline{\alpha}(U) \leq \overline{\alpha}(K) + \varepsilon;
$$

vì $\mu(f) = \overline{\beta}(f)$, ta thấy rằng $|\mu(K) - \overline{\alpha}(K)| \leq \varepsilon$, và vì $\varepsilon$ là tùy ý, nên $\mu(K) = \overline{\alpha}(K)$.

Đặc trưng hóa các tập mở thuộc $\overline{\Phi}$, kết hợp với Hệ quả 4 của Định lý 4 của No. 6, khi đó cho thấy rằng các tập mở thuộc $\overline{\Phi}$ không gì khác hơn là các tập mở $\mu$-khả tích, và rằng, với một tập như vậy $U$, ta có $\mu(U) = \overline{\alpha}(U)$. Định lý 4 của No. 6 và đặc trưng hóa các tập của $\overline{\Phi}$ được cho trong 5° khi đó cho thấy rằng các tập $\mu$-khả tích là các tập của $\overline{\Phi}$ và rằng, với một tập như vậy $M$, $\mu(M) = \overline{\alpha}(M)$. Cuối cùng, việc $\mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M)$ với mọi tập mở $U$ suy ra ngay từ (PC$_{II}$) và Hệ quả 4 của Định lý 4 của No. 6.

Định lý 5 như vậy được chứng minh hoàn toàn.

#### Hệ quả {#int-iv-s4-n11-cor-1 .statement}

— *Cho X là một không gian địa phương compact với một cơ sở đếm được, $\Psi$ là tập các tập Borel của X, $\beta$ là một ánh xạ của $\Psi$ vào $[0, +\infty]$ thỏa mãn các điều kiện sau:*

(i) *Nếu* $(B_1, B_2, \ldots)$ *là một dãy các tập Borel đôi một rời nhau của X, thì* $\beta(B_1 \cup B_2 \cup \ldots) = \beta(B_1) + \beta(B_2) + \ldots$.

(ii) *Nếu B là một tập con compact của X, thì* $\beta(B) < +\infty$.

*Khi đó, tồn tại một và chỉ một độ đo dương $\mu$ trên X sao cho* $\beta(B) = \mu^*(B)$ *với mọi* $B \in \Psi$.

Cho $\Phi$ là tập các tập con compact của $X$ và cho $\alpha$ là hạn chế của $\beta$ lên $\Phi$. Các điều kiện (PC$_I$), (PC$_{II}$), (PM$_I$), (PM$_{II}$), (PM$_{III}$) và (PM$_{IV}'$) khi đó được thỏa mãn. Cho $K$ là một tập con compact của $X$, và $\varepsilon > 0$. Khi đó $K$ là giao của một dãy giảm $(U_1, U_2, \ldots)$ các tập mở tương đối compact của X (GT, IX, §2, No. 5, Mệnh đề 7). Ta có $\sum_{n=1}^{\infty} \beta(U_n - U_{n+1}) = \beta(U_1 - K) < +\infty$, do đó

$$
\beta(U_n) - \beta(K) = \beta(U_n - K) = \sum_{p=n}^{\infty} \beta(U_p - U_{p+1})
$$

tiến tới 0 khi $n$ tiến tới $\infty$. Điều đó chứng tỏ rằng điều kiện $(\mathrm{PM}'_{\mathrm{IV}})$ được thỏa mãn. Theo Định lý 5, tồn tại một độ đo dương $\mu$ trên $X$ sao cho $\mu(K) = \alpha(K)$ với mọi tập con compact $K$ của $X$. Vì mọi tập mở $U$ của $X$ đều là hợp của một dãy tăng các tập con compact, ta có $\mu^*(U) = \beta(U)$. Gọi $L$ là một tập con compact của $X$. Theo Mệnh đề 7 của No. 5, các tập con khả tích theo $\mu$ của $L$ tạo thành một bộ tộc các tập con của $L$. Do đó, nếu $B$ là một phần tử của $\Psi$ được chứa trong $L$, thì $B$ là khả tích theo $\mu$; với mọi $\varepsilon > 0$, khi đó tồn tại một tập compact $K$ và một tập mở $U$ trong $X$ sao cho $K \subset B \subset U$ và $\mu^*(U) - \mu(K) \leq \varepsilon$ (No. 6, Th. 4). Vì $\beta(U) = \mu^*(U)$ và $\beta(K) = \mu(K)$, ta thấy rằng $|\mu^*(B) - \beta(B)| \leq 2\varepsilon$. Do đó $\beta(B) = \mu^*(B)$. Cuối cùng, mọi tập Borel $C$ của $X$ đều là hợp của một dãy các tập Borel đôi một rời nhau, tương đối compact, do đó $\beta(C) = \mu^*(C)$. Tính duy nhất của $\mu$ suy ra ngay từ Th. 5.

### Bài tập {#int-iv-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
