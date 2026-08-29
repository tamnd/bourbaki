---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 2
section_title: Metric spaces and metrizable spaces
lang: vi
source: top-v-x
pdf_pages: 0153-0166, 0232-0241
extraction: ocr
subsections:
    - "no": 1
      title: METRICS AND METRIC SPACES
      page: 0
      pdf_page: 153
    - "no": 2
      title: STRUCTURE OF A METRIC SPACE
      page: 0
      pdf_page: 154
    - "no": 3
      title: OSCILLATION OF A FUNCTION
      page: 0
      pdf_page: 157
    - "no": 4
      title: METRIZABLE UNIFORM SPACES
      page: 0
      pdf_page: 157
    - "no": 5
      title: METRIZABLE TOPOLOGICAL SPACES
      page: 0
      pdf_page: 158
    - "no": 6
      title: USE OF COUNTABLE SEQUENCES
      page: 0
      pdf_page: 159
    - "no": 7
      title: SEMI-CONTINUOUS FUNCTIONS ON A METRIZABLE SPACE
      page: 0
      pdf_page: 161
    - "no": 8
      title: METRIZABLE SPACES OF COUNTABLE TYPE
      page: 0
      pdf_page: 161
    - "no": 9
      title: COMPACT METRIC SPACES; COMPACT METRIZABLE SPACES
      page: 0
      pdf_page: 163
    - "no": 10
      title: QUOTIENT SPACES OF METRIZABLE SPACES
      page: 0
      pdf_page: 165
statements: 32
exercises: 9
content_sha256: 0a2079a4030086f98d0a98c613173101c4aa8daf175bfc7546106d5f0459f69b
translated_from: content/en/top/IX/02_s2_metric_spaces_and_metrizable_spaces.md
source_content_sha256: 251e0a701a7a4479cdf6534f4d5644531e477de5a2f33457b6f0c1971ce81b63
translation_model: gpt-5-6, gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-4b6cb0bf
glossary_version: 34
glossary_terms_sha256: 962880fc7954ecfa486279c37bea8384d590ed16a2accdd4a012cc35597b2af0
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. KHÔNG GIAN MÊTRIC VÀ CÁC KHÔNG GIAN MÊTRIC HÓA

### 1. CÁC MÊTRIC VÀ KHÔNG GIAN MÊTRIC

#### Định nghĩa 1 {#top-ix-s2-def-1 .statement}

*Một mêtric trên một tập hợp* $X$ *là một giả mêtric hữu hạn* $d$ *trên* $X$ *sao cho quan hệ* $d(x, y) = 0$ *suy ra* $x = y$. *Một không gian mêtric là một tập hợp* $X$ *được trang bị cấu trúc được xác định bởi một mêtric đã cho trên* $X$.

Một không gian mêtric $X$ luôn được xem là mang cấu trúc đều và tôpô được xác định bởi mêtric đã cho trên $X$.

#### Ví dụ 1 {#top-ix-s2-n1-exa-1 .statement}

Khoảng cách Euclid $d(x, y)$ (Chương VI, § 2, no. 1) là một mêtric trên không gian số thực $n$-chiều $\mathbf{R}^n$; các hàm sau cũng vậy

$$
\sup_{1 \leq i \leq n} |x_i - y_i| \quad \text{và} \quad \sum_{i=1}^n |x_i - y_i|.
$$

Tất cả các mêtric này là *tương đương* ($\S$ 1, no. 2).

#### Ví dụ 2 {#top-ix-s2-n1-exa-2 .statement}

Trên mọi tập hợp $X$, giả mêtric $d$, được xác định bởi các quan hệ $d(x, x) = 0$ và $d(x, y) = 1$ nếu $x \neq y$, là một mêtric. Cấu trúc đều mà nó xác định trên $X$ là cấu trúc đều *rời rạc*.

Ta có một định nghĩa tương đương với Định nghĩa 1 nếu nói rằng một mêtric là một giả mêtric *hữu hạn* sao cho cấu trúc đều được xác định bởi giả mêtric này là *Hausdorff*; một giả mêtric hữu hạn tương đương với một mêtric do đó là một mêtric.

Các không gian đều được xác định bởi *một giả mêtric duy nhất* (mà ta có thể giả sử là *hữu hạn*) có thể quy về các không gian mêtric khi giả mêtric không phải là một mêtric. Cho $f$ là một giả mêtric như vậy trên một tập hợp $X$, và cho $\mathcal{U}$ là cấu trúc đều được xác định bởi $f$; $\mathcal{U}$ không là Hausdorff, và giao của các lân cận của $\mathcal{U}$ là tập con của $X \times X$ được xác định bởi quan hệ tương đương $f(x, y) = 0$. Gọi $R$ là quan hệ này. Nếu $x \equiv x' \pmod{R}$, thì theo bất đẳng thức tam giác ta có

$$
f(x, y) \leq f(x, x') + f(x', y) = f(x', y)
$$

và tương tự $f(x', y) \leq f(x, y)$, do đó $f(x, y) = f(x', y)$; nói cách khác, $f$ là một hàm *tương thích* (theo $x$ và $y$) với quan hệ tương đương $R$ (*Lý thuyết tập hợp*, R, § 5, no. 7). Gọi $\overline{f}$ là hàm được cảm sinh bởi $f$ trên tập thương; $\overline{f}$ được xác định trên $(X/R) \times (X/R)$, và nếu $x$ và $y$ là hai điểm bất kỳ của $X$ và nếu $\dot{x}$ và $\dot{y}$ lần lượt chỉ các lớp tương đương (mod $R$) của $x$ và $y$, thì ta có $\overline{f}(\dot{x}, \dot{y}) = f(x, y)$. Suy ra ngay lập tức rằng $\overline{f}$ là một *mêtric* trên $X/R$; nó được gọi là mêtric *liên kết* với giả mêtric $f$; hơn nữa, cấu trúc đều mà nó xác định trên $X/R$ chính xác là cấu trúc đều Hausdorff *liên kết* với $\mathcal{U}$ bởi định nghĩa của cấu trúc đều này (Chương II, § 3, no. 8, Nhận xét). Như vậy, bằng cách chuyển qua một không gian thương thích hợp, cấu trúc đều được xác định bởi một giả mêtric duy nhất có thể quy về cấu trúc của một không gian mêtric.

Mệnh đề 1 của § 1, no. 3 xác định cấu trúc của *phép hoàn thiện* của một không gian mêtric:

#### Mệnh đề 1 {#top-ix-s2-prop-1 .statement}

*Cho $X$ là một không gian mêtric và $d$ là mêtric của nó. Nếu $\hat{X}$ là mêtric hoàn chỉnh của $X$ (đối với cấu trúc đều được xác định bởi $d$), thì hàm $d$ có thể được mở rộng bằng tính liên tục lên $\hat{X} \times \hat{X}$; hàm mở rộng $\overline{d}$ là một mêtric trên $\hat{X}$, và cấu trúc đều của $\hat{X}$ trùng với cấu trúc đều được xác định bởi mêtric $\overline{d}$.*

Mệnh đề 1 của § 1, no. 3 cho thấy rằng $\overline{d}$ là một giả mêtric hữu hạn trên $\hat{X}$, và cấu trúc đều được xác định bởi $\overline{d}$ trên $\hat{X}$ là cấu trúc đều thu được bằng phép hoàn chỉnh hóa; vì cấu trúc đều sau này là Hausdorff, nên $\overline{d}$ là một *mêtric*. Mỗi khi ta xét mêtric hoàn chỉnh của một không gian mêtric $X$ như một không gian mêtric, luôn phải hiểu rằng mêtric trên $\hat{X}$ là mêtric thu được bằng cách mở rộng mêtric trên $X$ bằng tính liên tục.

### 2. CẤU TRÚC CỦA MỘT KHÔNG GIAN MÊTRIC

Cho $X$ và $X'$ là hai không gian mêtric, $d$ là mêtric trên $X$, $d'$ là mêtric trên $X'$. Phù hợp với các định nghĩa tổng quát (*Lý thuyết tập hợp*, R, § 8, no. 5), một ánh xạ một-một $f$ từ $X$ lên $X'$ là một *đẳng cấu* của cấu trúc không gian mêtric của $X$ lên cấu trúc của $X'$ nếu

$$(1)$$
$$
d(x, y) = d'(f(x), f(y))
$$

với mọi $x \in X$ và mọi $y \in X$.

Chú ý rằng nếu $f$ là một ánh xạ từ $X$ lên $X'$ thỏa mãn đẳng thức (1), thì $f$ tất phải *song ánh* và do đó là một đẳng cấu từ $X$ lên $X'$; một đẳng cấu như vậy cũng được gọi là một *đẳng cự* (hay một ánh xạ *đẳng cự*) từ $X$ lên $X'$.

Một đẳng cự từ X lên X' dĩ nhiên là một đẳng cấu của cấu trúc đều (tương ứng tôpô) của X lên cấu trúc đều (tương ứng tôpô) của X'; các mệnh đề đảo của những mệnh đề này là sai, như được chỉ ra bởi sự tồn tại của các mêtric tương đương phân biệt (§ 1, no. 2).

Cho X là một không gian mêtric, d là mêtric trên X. Với mỗi a > 0, gọi V_a là tập con của X × X gồm mọi cặp (x, y) sao cho d(x, y) < a, và gọi W_a là tập con của X × X gồm mọi cặp (x, y) sao cho d(x, y) ≤ a. Khi a chạy qua tập hợp mọi số thực > 0 (hoặc chỉ cần một dãy số > 0 hội tụ về 0), các tập V_a (tương ứng W_a) tạo thành một hệ cơ bản các lân cận mở (tương ứng đóng) của cấu trúc đều của X, do tính liên tục của d (§ 1, no. 3). Ta có $\overline{V}_a \subset W_a$, nhưng hai tập này không nhất thiết trùng nhau.

Tương tự như trường hợp khoảng cách Euclid trên $\mathbf{R}^n$, tập $V_a(x)$ [tương ứng $W_a(x)$] được gọi là quả cầu mở (tương ứng quả cầu đóng) tâm x bán kính a; nó là một tập mở (tương ứng đóng) trong X. Cũng vậy, tập hợp mọi $y \in X$ sao cho $d(x, y) = a$ được gọi là mặt cầu tâm x bán kính a; nó là một tập đóng. Từ những điều đã nói, các quả cầu mở (tương ứng đóng) tâm x bán kính a tạo thành một hệ cơ bản các lân cận của x khi a chạy qua tập hợp mọi số thực > 0, hoặc một dãy số > 0 hội tụ về 0.

Người đọc cần thận trọng đừng cho rằng các quả cầu và mặt cầu trong một không gian mêtric tùy ý có cùng các tính chất như các quả cầu và mặt cầu Euclid được nghiên cứu trong Chương VI, § 2. Chẳng hạn, bao đóng của một quả cầu mở không nhất thiết là quả cầu đóng có cùng tâm và bán kính; biên của một quả cầu đóng không nhất thiết là mặt cầu có cùng tâm và bán kính; một quả cầu mở (hay đóng) không nhất thiết liên thông; và một mặt cầu có thể rỗng (xem Bài tập 4).

Cho A và B là hai tập con không rỗng tùy ý của một không gian mêtric X. Số
$$
d(A, B) = \inf_{x \in A, y \in B} d(x, y)
$$
được gọi là khoảng cách giữa các tập A và B. Đặc biệt, ta ký hiệu bởi $d(x, A)$ khoảng cách giữa tập $\{x\}$ và tập A; đó được gọi là khoảng cách từ điểm x đến tập A. Như vậy
$$
d(x, A) = \inf_{y \in A} d(x, y)
$$
do đó
$$
d(A, B) = \inf_{x \in A} d(x, B)
$$
(Chương IV, § 5, no. 4, Mệnh đề 9).

#### Nhận xét {#top-ix-s2-n2-rem-1 .statement}

Nếu $d(x, A) = a$, có thể xảy ra trường hợp không có điểm nào của A mà khoảng cách đến x bằng a. Tuy nhiên, tình huống này không bao giờ xảy ra nếu A compắc, vì khi đó định lý Weierstrass (Chương IV, § 6, no. 1, Định lý 1) cho thấy rằng tồn tại $y \in A$ sao cho $d(x, A) = d(x, y)$.

#### Mệnh đề 2 {#top-ix-s2-prop-2 .statement}

*Các mệnh đề* $d(x, A) = 0$ *và* $x \in \overline{A}$ *là tương đương*.

Vì $d(x, A) = 0$ biểu thị sự kiện rằng quả cầu $V_a(x)$ gặp $A$ với mọi giá trị của $a > 0$; và điều này tương đương với $x \in \overline{A}$.

#### Mệnh đề 3 {#top-ix-s2-prop-3 .statement}

*Hàm* $d(x, A)$ *là liên tục đều trên* $X$.

Cho $x$ và $y$ là hai điểm tùy ý của $X$; khi đó với mọi $\varepsilon > 0$ cho trước tồn tại $z \in A$ sao cho $d(y, z) \leq d(y, A) + \varepsilon$, và do đó
$$
d(x, z) \leq d(x, y) + d(y, z) \leq d(x, y) + d(y, A) + \varepsilon
$$
theo bất đẳng thức tam giác.

*A fortiori* $d(x, A) \leq d(x, y) + d(y, A) + \varepsilon$, và vì $\varepsilon$ là tùy ý nên suy ra $d(x, A) \leq d(x, y) + d(y, A)$. Tương tự ta có
$$
d(y, A) \leq d(x, y) + d(x, A),
$$
sao cho
$$
|d(x, A) - d(y, A)| \leq d(x, y),
$$
do đó kết quả được suy ra.

#### Nhận xét {#top-ix-s2-n2-rem-2 .statement}

Ta có thể có $d(A, B) = 0$ đối với hai tập con $A, B$ của $X$ sao cho $\overline{A} \cap \overline{B} = \varnothing$, với điều kiện rằng không tập con nào trong hai tập con là một điểm đơn. Ví dụ, trên đường thẳng thực $\mathbf{R}$, tập hợp các số nguyên $> 0$ và tập hợp các điểm của dãy $(n + 1/2^n)_{n \geq 1}$ là hai tập hợp đóng rời nhau mà khoảng cách giữa chúng là không.

Tuy nhiên, nếu $A$ là *compact* và $B$ là *đóng*, quan hệ $d(A, B) = 0$ kéo theo $A \cap B \neq \varnothing$, vì nhờ quan hệ
$$
d(A, B) = \inf_{x \in A} d(x, B)
$$
suy ra từ Mệnh đề 3 và định lý Weierstrass rằng tồn tại $x_0 \in A$ sao cho $d(x_0, B) = d(A, B) = 0$ và do đó (Mệnh đề 2) $x_0 \in B$.

*Đường kính* của một tập con khác rỗng $A$ của $X$ là số (hữu hạn hoặc bằng $+\infty$)
$$
\delta(A) = \sup_{x \in A, y \in A} d(x, y).
$$

Khái niệm về một "tập hợp W_a-nhỏ" (Chương II, § 3, no. 1) đồng nhất với khái niệm về một tập hợp có đường kính $\leq a$. Một tập hợp khác rỗng $A$ gồm một điểm duy nhất khi và chỉ khi $\delta(A) = 0$.

Một tập con $A$ của $X$ là *bị chặn* (đối với metric $d$) nếu đường kính của nó là *hữu hạn*; tương đương, nếu với mỗi điểm $x_0 \in X$, $A$ được chứa trong một quả cầu có tâm $x_0$. Mọi tập con của một tập hợp bị chặn đều bị chặn, và hợp của một họ hữu hạn các tập hợp bị chặn là một tập hợp bị chặn.

Chú ý rằng một tập con của $X$ có thể bị chặn đối với một metric $d$ nhưng không bị chặn đối với một metric tương đương với $d$ (xem § 1, no. 2).

### 3. DAO ĐỘNG CỦA MỘT HÀM

Liên quan đến khái niệm đường kính là khái niệm dao động của một hàm $f$, được định nghĩa trên một tập hợp tùy ý $X$ và nhận các giá trị của nó trong một không gian metric $X'$; nếu $A$ là một tập con khác rỗng tùy ý của $X$, đường kính $\delta(f(A))$ được gọi là dao động của $f$ trong $A$.

Nếu hơn nữa $X$ là một tập con của một không gian tôpô $Y$, và nếu $x \in \overline{X}$, số
$$
\omega(x; f) = \inf \delta(f(V \cap X))
$$
(khi $V$ chạy qua lọc lân cận của $x$ trong $Y$) được gọi là độ dao động của $f$ tại $x \in \overline{X}$.

#### Mệnh đề 4 {#top-ix-s2-prop-4 .statement}

*Độ dao động $\omega(x; f)$ của một hàm tùy ý $f$, được xác định trên một tập con $X$ của một không gian tôpô $Y$ và nhận giá trị trong một không gian mêtric $X'$, là nửa liên tục trên trên $\overline{X}$.*

Cho $a$ là một điểm bất kỳ của $\overline{X}$; khi đó với mỗi $k > \omega(a; f)$ tồn tại một lân cận mở $V$ của $a$ sao cho $\delta(f(V \cap X)) \leq k$; với mỗi $x \in V \cap \overline{X}$, $V$ là một lân cận của $x$ và do đó
$$
\omega(x; f) \leq \delta(f(V \cap X)) \leq k,
$$
điều này chứng tỏ rằng $\omega$ là nửa liên tục trên tại điểm $a$.

Để có $\omega(x; f) = 0$ tại một điểm $x \in \overline{X}$ thì điều kiện cần và đủ là với mỗi $\varepsilon > 0$ tồn tại một lân cận $V$ của $x$ sao cho $f(V \cap X)$ được chứa trong một hình cầu bán kính $\varepsilon$; nếu $x \in X$, điều kiện này biểu thị sự kiện rằng $f$ liên tục tại điểm $x$ (đối với $X$); nếu $x \in \overline{X} \cap \mathbf{C}X$, ảnh qua $f$ của vết trên $X$ của lọc lân cận của $x$ trong $Y$ là một cơ sở lọc Cauchy trên $X'$; đặc biệt:

#### Mệnh đề 5 {#top-ix-s2-prop-5 .statement}

*Một hàm $f$ được xác định trên một tập con $X$ của một không gian tôpô $Y$, nhận giá trị trong một không gian mêtric đầy đủ $X'$. Khi đó $f$ có giới hạn tương đối với $X$ tại một điểm $x \in \overline{X}$ khi và chỉ khi độ dao động của $f$ tại $x$ bằng không.*

### 4. CÁC KHÔNG GIAN ĐỒNG ĐỀU METRIC HÓA ĐƯỢC

#### Định nghĩa 2 {#top-ix-s2-def-2 .statement}

*Một mêtric trên một tập hợp $X$ được gọi là tương thích với một cấu trúc đồng đều $U$ trên $X$ nếu cấu trúc đồng đều được xác định bởi mêtric trùng với $U$.
Một cấu trúc đồng đều trên một tập hợp $X$ được gọi là metric hóa được nếu có một mêtric trên $X$ tương thích với cấu trúc đồng đều này. Một không gian đồng đều được gọi là metric hóa được nếu cấu trúc đồng đều của nó là metric hóa được.*

Các mêtric phân biệt có thể tương thích với cùng một cấu trúc đồng đều; khi đó chúng là *tương đương* (§ 1, no. 2, Định nghĩa 2).

#### Định lý 1 {#top-ix-s2-thm-1 .statement}

*Một cấu trúc đồng đều là metric hóa được khi và chỉ khi nó Hausdorff và lọc các lân cận của cấu trúc đồng đều có một cơ sở đếm được.*

Điều kiện là *cần thiết*, vì (với ký hiệu của no. 2) các lân cận $V_{1/n} (n \geq 1)$ tạo thành một cơ sở của lọc các lân cận của cấu trúc đồng đều của một không gian mêtric.

Điều kiện là *đủ*, vì, nếu nó được thỏa mãn, cấu trúc đồng đều đang xét được xác định bởi một giả mêtric duy nhất, theo Mệnh đề 2 của § 1, no. 4; vì cấu trúc đồng đều là Hausdorff, giả mêtric này là một mêtric.

#### Hệ quả 1 {#top-ix-s2-thm-1-cor-1 .statement}

*Một cấu trúc đồng đều Hausdorff được xác định bởi một họ đếm được các giả mêtric là metric hóa được.*

Vì nếu $(f_n)$ là một dãy các giả metric xác định một cấu trúc như vậy, lọc các lân cận được sinh bởi họ đếm được các tập $\overline{f}_n^1([0, 1/m])$, trong đó $m$ và $n$ lần lượt chạy qua tập các số nguyên $> 0$.

#### Hệ quả 2 {#top-ix-s2-thm-1-cor-2 .statement}

*Mọi tích đếm được của các không gian đồng nhất mêtric hóa được đều mêtric hóa được.*

Vì một không gian như vậy là Hausdorff và cấu trúc đồng nhất của nó có một hệ cơ sở đếm được các lân cận (Chương II, § 2, no. 6).

### 5. KHÔNG GIAN TÔPÔ MÊTRIC HÓA ĐƯỢC

#### Định nghĩa 3 {#top-ix-s2-def-3 .statement}

*Một mêtric trên một tập $X$ được gọi là tương thích với một tôpô $\mathcal{T}$ trên $X$ nếu tôpô được xác định bởi mêtric này trùng với $\mathcal{T}$. Một không gian tôpô được gọi là mêtric hóa được nếu tồn tại một mêtric trên $X$ tương thích với tôpô của $X$.*

Hai mêtric trên một tập $X$ đều tương thích với cùng một tôpô $\mathcal{T}$ có thể *không tương đương*.

Không gian con $\mathbf{R}_+^*$ của $\mathbf{R}$ cung cấp một ví dụ về điều này. Cả cấu trúc đồng nhất cảm sinh bởi cấu trúc đồng nhất cộng tính của $\mathbf{R}$ và cấu trúc đồng nhất cảm sinh bởi cấu trúc đồng nhất nhân của $\mathbf{R}_+^*$ đều mêtric hóa được và tương thích với tôpô của $\mathbf{R}_+^*$; nhưng chúng không so sánh được.

Ta cũng nhận xét rằng có thể tồn tại các cấu trúc đồng nhất *không mêtric hóa được* tương thích với tôpô của một không gian tôpô *mêtric hóa được* (Bài tập 7).

Ở đây ta sẽ chỉ xét các điều kiện *cần* để một không gian tôpô mêtric hóa được (về một điều kiện cần và đủ, xem § 4, Bài tập 22). Trước hết, một không gian không thể mêtric hóa được trừ khi nó hoàn toàn chính quy (thật vậy, ta sẽ thấy, trong § 4, no. 1, Mệnh đề 2, rằng một không gian mêtric hóa được nhất thiết là "chuẩn tắc", đây là một điều kiện mạnh hơn). Mặt khác, Định lý 1 chỉ ra rằng:

#### Mệnh đề 6 {#top-ix-s2-prop-6 .statement}

Mỗi điểm của một không gian mêtric hóa được có một hệ cơ bản đếm được các lân cận.

Tổng quát hơn:

#### Mệnh đề 7 {#top-ix-s2-prop-7 .statement}

Trong một không gian mêtric hóa được, mỗi tập đóng là giao của một họ đếm được các tập mở, và mỗi tập mở là hợp của một họ đếm được các tập đóng.

Cho $d$ là một mêtric tương thích với tôpô của một không gian mêtric hóa được $X$. Nếu $A$ là một tập con đóng của $X$, nó là giao của các tập mở $V_{1/n}(A)$ [tập hợp tất cả các $x \in X$ sao cho $d(x, A) < 1/n$; xem Mệnh đề 2]. Phần thứ hai của mệnh đề suy ra bằng cách lấy các phần bù.

#### Nhận xét 1 {#top-ix-s2-n5-rem-1 .statement}

Các điều kiện cần này không đủ (xem Bài tập 13).
2) Có những không gian trong đó mỗi điểm có một hệ cơ bản đếm được các lân cận nhưng trong đó tồn tại các tập đóng không phải là giao đếm được của các tập mở (Bài tập 15); các không gian như vậy không mêtric hóa được.

Hệ quả 2 của Định lý 1, no. 4, chỉ ra rằng một tích đếm được của các không gian tôpô mêtric hóa được là mêtric hóa được. Ngoài ra, tổng $X$ (Chương I, § 2, no. 4) của một họ tùy ý $(X_i)_{i \in I}$ các không gian mêtric hóa được cũng mêtric hóa được. Vì nếu $d_i$ là một mêtric tương thích với tôpô của $X_i$ đối với mỗi $i \in I$, ta có thể giả sử rằng $d_i$ bị chặn và đường kính của $X_i$ là $\leq 1$; khi đó ta có thể định nghĩa một khoảng cách $d$ tương thích với tôpô của $X$ bằng cách đặt $d(x, y) = d_i(x, y)$ nếu $x$ và $y$ đều thuộc cùng một $X_i$, và $d(x, y) = 1$ nếu không.

### 6. SỬ DỤNG CÁC DÃY ĐẾM ĐƯỢC

Mệnh đề 6 là nguồn gốc của vai trò do các dãy đếm được của các điểm đóng trong lý thuyết các không gian mêtric hóa được; đối với nhiều vấn đề, chúng có thể được dùng thuận lợi thay cho các lọc. Điều này là vì các lọc lân cận của các điểm của một không gian mêtric hóa được (và do đó cả các lọc hội tụ) được xác định bởi các dãy hội tụ của các điểm của không gian: vì lọc lân cận của một điểm có một cơ sở đếm được, nó là giao của các lọc sơ cấp mịn hơn nó (Chương I, § 6, no. 8, Mệnh đề 11), tức là, của các lọc sơ cấp liên kết với các dãy hội tụ đến điểm đang xét.

Mặt khác, khái niệm một dãy hội tụ không thích nghi với việc nghiên cứu các không gian tôpô trong đó có những điểm mà lọc lân cận không có cơ sở đếm được. Đặc biệt, có thể xây dựng các không gian tôpô Hausdorff không rời rạc trong đó, tại mỗi điểm $x$, giao của mọi họ đếm được các lân cận của $x$ lại là một lân cận của $x$(*); trong một không gian như vậy các dãy hội tụ duy nhất là những dãy mà tất cả các số hạng đều bằng nhau kể từ một chỉ số nào đó trở đi.

Làm ví dụ về việc sử dụng các dãy đếm được, ta đưa ra các mệnh đề sau:

#### Mệnh đề 8 {#top-ix-s2-prop-8 .statement}

*Trong một không gian mêtric hóa được* $X$, *một điểm* $x$ *nằm trong bao đóng của một tập con khác rỗng* $A$ *của* $X$ *khi và chỉ khi tồn tại một dãy các điểm của* $A$ *hội tụ đến* $x$.

Chúng ta đã biết, từ Chương I, § 7, no. 3, rằng điều kiện là *đủ*. Để thấy rằng nó là *cần*, xét một hệ cơ bản đếm được $(V_n)$ các lân cận của $x$ sao cho $V_{n+1} \subset V_n$ với mỗi $n$. Nếu $x$ nằm trong bao đóng của $A$ thì mỗi $V_n$ giao với $A$, và nếu $x_n$ nằm trong $V_n \cap A$, dãy $(x_n)$ hội tụ tới $x$(**).

Từ Mệnh đề 8 ta suy ra:

#### Mệnh đề 9 {#top-ix-s2-prop-9 .statement}

*Một không gian metric* $X$ *là đầy đủ khi và chỉ khi mọi dãy Cauchy trong* $X$ *là hội tụ*.

Gọi $\hat{X}$ là phần đầy đủ của $X$. Nếu có một điểm $x \in \hat{X}$ không thuộc $X$, thì tồn tại một dãy $(x_n)$ các điểm của $X$ hội tụ tới $x$, và đây là một dãy Cauchy không hội tụ trong $X$.

#### Mệnh đề 10 {#top-ix-s2-prop-10 .statement}

*Cho* $X$ *là một không gian khả mêtric và cho* $f$ *là một ánh xạ từ* $X$ *vào một không gian tôpô* $X'$. *Khi đó* $f$ *liên tục tại một điểm* $x \in X$ *khi và chỉ khi, bất cứ khi nào* $(x_n)$ *là một dãy các điểm của* $X$ *hội tụ tới* $x$, *dãy* $(f(x_n))$ *hội tụ tới* $f(x)$ *trong* $X'$.

Điều kiện là cần, từ Chương I, § 7, no. 4, Mệnh đề 9, Hệ quả 1. Để chứng minh rằng nó là đủ, xét lọc $\mathcal{B}'$ các lân cận của $f(a)$ trong $X'$; giả thiết kéo theo rằng $\overline{f}^{-1}(\mathcal{B}')$ thô hơn mọi lọc sơ cấp liên kết với một dãy hội tụ tới $a$, nghĩa là mọi lọc sơ cấp hội tụ tới $a$; nhưng

(*) Xem chẳng hạn, J. Dieudonné, Notes de Tératopologie (I), Revue scientifique (Revue rose), 1939, p. 39.
(**) Mệnh đề này vẫn có thể đúng trong một số không gian trong đó ít nhất một điểm không có bất kỳ hệ cơ bản đếm được nào các lân cận; ví dụ, không gian thu được bằng cách compact hóa một không gian rời rạc không đếm được bằng cách thêm vào một điểm ở vô cực (Chương I, § 9, no. 8, Định lý 4).

giao của các lọc này là lọc lân cận của $a$ (Chương I, § 6, no. 8, Mệnh đề 11). Do đó có kết quả.

Chú ý rằng các Mệnh đề 8 và 10 đúng trong mọi không gian $X$ trong đó mỗi điểm có một hệ cơ bản đếm được các lân cận.

### 7. HÀM BÁN LIÊN TỤC TRÊN MỘT KHÔNG GIAN KHẢ MÊTRIC

#### Mệnh đề 11 {#top-ix-s2-prop-11 .statement}

*Cho $X$ là một không gian khả mêtric và cho* $f$ *là một hàm nửa liên tục dưới trên* $X$ *nhận các giá trị của nó trong một khoảng đóng* $[a, b]$ *của* $\overline{\mathbf{R}}$. *Khi đó* $f$ *là bao trên của một dãy tăng các hàm liên tục trên* $X$ *nhận các giá trị của chúng trong* $[a, b]$.*

Bằng phép chuyển cấu trúc, ta có thể giả sử rằng $a = 0$ và $b = 1$.

(i) Trước hết, giả sử rằng $f = \varphi_A$, trong đó $A$ là một tập mở của $X$. Khi đó hàm $g_n$ được xác định bởi $g_n(x) = n \inf (d(x, X - A), 1/n)$ là liên tục và $\geq 0$ trên $X$; ngoài ra $g_n(x) = f(x)$ khi $x \in X - A$ và khi
$$
d(x, X - A) \geq 1/n.
$$
Do đó, ngay lập tức, $f = \sup_n (g_n)$.

(ii) Trong trường hợp tổng quát, với mỗi số nguyên $n \geq 1$, xét dãy giảm hữu hạn các tập mở
$$
A_k = f^{-1}\left( \left[ \frac{k}{n}, +\infty \right[ \right) \quad (0 \leq k \leq n - 1);
$$
hàm $g_n = \frac{1}{n} \sum_{k=1}^{n-1} \varphi_{A_k}$ là nửa liên tục dưới, và ta có $0 \leq f(x) - g_n(x) \leq 1/n$ với mọi $n$; do đó $f$ là bao trên của dãy $(g_n)$. Mặt khác, $g_n$ là một tổ hợp tuyến tính với các hệ số dương của một số hữu hạn các hàm đặc trưng của các tập mở và do đó là bao trên của một dãy đếm được $(h_{mn})_{m \geq 0}$ gồm các hàm liên tục $\geq 0$, theo (i); do đó $f = \sup_{m,n} h_{mn}$. Nếu đặt
$$
f_n = \sup_{p \leq n, q \leq n} h_{pq},
$$
ta thấy rằng dãy $(f_n)$ là một dãy tăng các hàm liên tục $\geq 0$, có $f$ làm bao trên, và không nhận giá trị 1, vì $g_n \leq n - 1/n$.

### 8. KHÔNG GIAN METRIZƠ KIỂU ĐẾM ĐƯỢC

#### Định nghĩa 4 {#top-ix-s2-def-4 .statement}

*Một không gian mêtric được gọi là kiểu đếm được (hoặc tách được) nếu tôpô của nó có một cơ sở đếm được.*

Rõ ràng mọi không gian con của một không gian mêtric kiểu đếm được lại là không gian kiểu đếm được. Định nghĩa về cơ sở của tôpô của một không gian tích (Chương I, § 4, no. 1) và Hệ quả 2 của Định lý 1 của no. 4 cho thấy tích của một họ đếm được các không gian mêtric kiểu đếm được là một không gian mêtric kiểu đếm được. Tương tự, tổng của một họ đếm được các không gian mêtric kiểu đếm được là một không gian mêtric kiểu đếm được (no. 5).

#### Mệnh đề 12 {#top-ix-s2-prop-12 .statement}

*Nếu X là một không gian tôpô mêtric, các mệnh đề sau là tương đương*:

a) *X là kiểu đếm được*.
b) *X có một tập con trù mật đếm được*.
c) *X đẳng cấu tôpô với một không gian con của khối $\mathbf{I}^{\mathbf{N}}$, trong đó $\mathbf{I}$ là khoảng $[0, 1]$ trong $\mathbf{R}$.*

Từ các nhận xét trên, rõ ràng c) kéo theo a); a) kéo theo b), vì nếu $(U_n)$ là một cơ sở đếm được của tôpô của X và $a_n$ là một điểm của $U_n$, thì các $a_n$ tạo thành một tập con trù mật của X. Cuối cùng, ta chứng minh rằng b) kéo theo c). Gọi $(a_n)$ là một dãy đếm được trù mật các điểm của X, và với mỗi $x \in X$ đặt $\varphi(x)$ là điểm $(d(x, a_n))_{n \in \mathbf{N}}$ của $\mathbf{I}^{\mathbf{N}}$ ($d$ là một metric tương thích với tôpô của X, đối với metric này đường kính của X là $\leq 1$). Ta sẽ chứng minh rằng $\varphi$ là một phép đồng phôi của X lên một không gian con của $\mathbf{I}^{\mathbf{N}}$. Thật vậy, $\varphi$ liên tục, vì mỗi hàm $x \to d(x, a_n)$ đều liên tục; và $\varphi$ đơn ánh, vì mỗi điểm của X là giới hạn của một dãy con nào đó của $(a_n)$ (Mệnh đề 8). Cho B là một quả cầu có tâm $x_0$ và bán kính $r$ trong X, và cho $n$ là một số nguyên sao cho

$$
d(x_0, a_n) < \frac{1}{3} r.
$$

Ảnh qua $\varphi$ của tập W gồm các điểm $x \in X$ sao cho

$$
|d(x_0, a_n) - d(x, a_n)| < \frac{1}{3} r
$$

theo định nghĩa là một lân cận của $\varphi(x_0)$ trong $\varphi(X)$. Nhưng với mỗi $x \in W$ ta có $d(x, a_n) < d(x_0, a_n) + \frac{1}{3} r < \frac{2}{3} r$, do đó

$$
d(x, x_0) \leq d(x_0, a_n) + d(x, a_n) < r,
$$

điều đó cho thấy W là một lân cận của $x_0$ được chứa trong B, và do đó $\varphi$ là một đồng phôi của X lên $\varphi(X)$.

Chú ý rằng đối với một không gian tôpô tùy ý X, tính chất b) không nhất thiết kéo theo sự tồn tại của một cơ sở đếm được, ngay cả khi X compact và mọi điểm của X đều có một hệ cơ bản đếm được các lân cận (Bài tập 13; xem Chương I, § 1, Bài tập 7).

#### Mệnh đề 13 {#top-ix-s2-prop-13 .statement}

*Cho X là một không gian tôpô có một cơ sở đếm được $(U_n)$; khi đó với mỗi phủ mở $(V_i)_{i \in I}$ của X, tồn tại một tập con đếm được J của I sao cho $(V_i)_{i \in J}$ là một phủ của X.*

Gọi H là tập con của N gồm các chỉ số n sao cho U_n được chứa trong ít nhất một trong các $V_i$; dãy (U_n)_{n \in H} là một phủ của X, vì mọi điểm $x \in X$ đều thuộc một $V_i$ nào đó, và vì $V_i$ là mở, nên tồn tại một chỉ số n sao cho $x \in U_n \subset V_i$. Do đó tồn tại một ánh xạ $\psi$ từ H vào I sao cho $U_n \subset V_{\psi(n)}$ với mỗi $n \in H$; lấy J = $\psi(H)$, là một tập đếm được, thì mệnh đề được chứng minh.

### 9. KHÔNG GIAN METRIC COMPACT; KHÔNG GIAN COMPACT KHẢ MÉTRIC HÓA

Tiêu chuẩn tiền compact của một không gian đều (Chương II, § 4, no. 2, Định lý 3) dẫn đến mệnh đề sau đối với các không gian metric:

#### Mệnh đề 14 {#top-ix-s2-prop-14 .statement}

*Một không gian metric X là tiền compact khi và chỉ khi, với mỗi $\varepsilon > 0$, tồn tại một phủ hữu hạn của X bởi các tập hợp có đường kính $\leq \varepsilon$.*

Nếu thêm giả thiết rằng X là *đầy đủ* thì ta có một tiêu chuẩn về *tính compact* của các không gian metric.

Từ Mệnh đề 14 ta thu được một tiêu chuẩn *tôpô* về tính compact, áp dụng được cho các không gian khả métric hóa:

#### Mệnh đề 15 {#top-ix-s2-prop-15 .statement}

*Một không gian tôpô khả métric hóa X là compact khi và chỉ khi mọi dãy vô hạn các điểm của X đều có một điểm tụ trong X.*

Tiên đề (C) của Chương I, § 9, no. 1 cho thấy điều kiện đó là *cần*. Để chứng minh tính *đủ*, gọi d là một metric tương thích với tôpô của X. Trước hết ta chứng minh rằng không gian metric X được xác định như vậy là *đầy đủ*: mọi dãy Cauchy trong X đều có một điểm tụ và do đó hội tụ (Chương II, § 3, no. 2, Mệnh đề 5, Hệ quả 2); vì thế X là đầy đủ, theo Mệnh đề 9. Tiếp theo ta sẽ chứng minh rằng X là *tiền compact*; nếu không phải vậy thì theo Mệnh đề 14 sẽ tồn tại một số thực $\alpha > 0$ sao cho X không thể được phủ bởi một số hữu hạn tập con của X có đường kính $\leq \alpha$. Khi đó ta có thể định nghĩa bằng quy nạp theo n một dãy vô hạn $(x_n)$ các điểm của X bởi điều kiện $d(x_p, x_n) > \frac{1}{2} \alpha$ với mọi $p < n$; và một dãy như thế không thể có điểm tụ, vì mọi quả cầu bán kính $< \frac{1}{2} \alpha$ chứa nhiều nhất một điểm của dãy.

#### Hệ quả {#top-ix-s2-n9-cor-1 .statement}

*Một tập con A của một không gian tôpô khả métric hóa X là compact tương đối khi và chỉ khi mọi dãy vô hạn các điểm của A đều có một điểm tụ trong X.*

Gọi d là một metric tương thích với tôpô của X. Ta sẽ chứng minh rằng không gian $\overline{A}$ là compact, bằng cách áp dụng tiêu chuẩn của Mệnh đề 15. Gọi $(x_n)$ là một dãy các điểm của $\overline{A}$; khi đó với mỗi chỉ số n tồn tại $y_n \in A$ sao cho $d(x_n, y_n) < 1/n$; dãy $(y_n)$ theo giả thiết có một điểm tụ $a \in X$, và a cũng là một điểm tụ của dãy $x_i$, vì nếu $y_m$ nằm trong quả cầu tâm a bán kính $1/n$, với một $m > n$, thì $x_m$ nằm trong quả cầu tâm a bán kính $2/n$.

Cần nhận xét rằng Mệnh đề 15 không phải là một hệ quả của sự tồn tại của một hệ cơ bản đếm được các lân cận tại mỗi điểm của $X$; có những ví dụ về các không gian không khả métric hóa, không compact mà trong đó mọi điểm đều có một hệ cơ bản đếm được các lân cận và mọi dãy vô hạn các điểm đều có một điểm tụ (Bài tập 15).

#### Mệnh đề 16 {#top-ix-s2-prop-16 .statement}

*Một không gian compact $X$ là khả métric hóa khi và chỉ khi tôpô của nó có một cơ sở đếm được.*

Điều kiện đó là *cần*. Theo Mệnh đề 14, với mỗi số nguyên $n \geq 1$ tồn tại một tập con hữu hạn $A_n$ của $X$ sao cho khoảng cách từ $A_n$ đến mọi điểm của $X$ là $\leq 1/n$; do đó tập hợp đếm được $A = \bigcup_n A_n$ là trù mật trong $X$, và kết quả suy ra từ Mệnh đề 12 của no. 8.

Điều kiện đó là *đủ*. Gọi $(U_n)$ là một cơ sở đếm được của tôpô trên $X$. Mọi lân cận của một điểm trên đường chéo $\Delta$ của $X \times X$ do đó đều chứa một lân cận có dạng $U_n \times U_n$; áp dụng tiên đề Borel-Lebesgue cho tập con compact $\Delta$ của $X \times X$, suy ra rằng mọi lân cận của $\Delta$ đều chứa một hợp hữu hạn các tập hợp có dạng $U_n \setminus U_n$, là một lân cận của $\Delta$. Do đó các lân cận của $\Delta$ là những hợp hữu hạn của các tập hợp có dạng $U_n \times U_n$ tạo thành một hệ cơ bản các entourage của cấu trúc đều trên $X$ (Chương II, § 4, no. 1, Định lý 1), và vì thế kết quả suy ra từ Định lý 1 của no. 4.

#### Hệ quả {#top-ix-s2-n9-cor-2 .statement}

*Cho $X$ là một không gian compact địa phương và gọi $X'$ là không gian compact thu được bằng cách thêm vào $X$ một điểm ở vô cùng $\omega$ (Chương I, § 9, no. 8). Khi đó các mệnh đề sau là tương đương:*

a) *Tôpô của $X$ có một cơ sở đếm được.*
b) $X'$ *có thể mêtric hóa được.*
c) $X$ *có thể mêtric hóa được và $\sigma$-compact.*

$a \Longrightarrow b$: Cho $U_n$ là một cơ sở đếm được của tôpô của $X$. Mỗi lân cận của một điểm $x \in X$ chứa một lân cận compact của $x$, đến lượt nó chứa một lân cận của $x$ bằng một $U_n$ nào đó. Do đó, các $U_n$ tương đối compact tạo thành một cơ sở của tôpô của $X$, và vì vậy ta có thể giả sử rằng tất cả các $U_n$ đều tương đối compact. Do đó, $X$ là hợp đếm được của các tập compact $\overline{U}_n$, tức là $\sigma$-compact; điều này suy ra rằng trong $X'$ điểm $\omega$ có một hệ cơ bản đếm được $V_n$ gồm các lân cận mở (Chương I, § 9, no. 9, Mệnh đề 15, Hệ quả 2). Do đó mỗi lân cận của một điểm $y \in X'$ chứa hoặc một trong các $U_n$, hoặc một trong các $V_n$, vốn là một lân cận của $y$, và do đó các $U_n$ và các $V_n$ tạo thành một cơ sở đếm được của tôpô của $X'$. Suy ra $X'$ có thể mêtric hóa được, theo Mệnh đề 16.

b) $\Longrightarrow c)$: Nếu $X'$ có thể mêtric hóa được, thì $\omega$ có một hệ cơ bản đếm được các lân cận, và do đó $X$ là $\sigma$-compact theo Chương I, § 9, no. 9, Mệnh đề 15, Hệ quả 2.

c) $\Longrightarrow a)$: Theo giả thiết, có một dãy tăng $(V_n)$ gồm các tập mở tương đối compact phủ $X$ và thỏa mãn $\overline{V}_n \subset V_{n+1}$ (Chương I, § 9, no. 9, Mệnh đề 15). Không gian con $\overline{V}_n$ compact và có thể mêtric hóa được, do đó có một cơ sở đếm được (Mệnh đề 16), và vì vậy $V_n$ cũng có một cơ sở đếm được. Cho $(U_{mn})_{m \geq 1}$ là một cơ sở của tôpô của $V_n$. Với mỗi $x \in X$ và mỗi lân cận $W$ của $x$, tồn tại $n$ sao cho $x \in V_n$, do đó tồn tại $m$ sao cho $x \in U_{mn} \subset V_n \cap W$. Suy ra các tập $U_{mn}$ ($m \geq 1, n \geq 1$) tạo thành một cơ sở của tôpô của $X$.

### 10. CÁC KHÔNG GIAN THƯƠNG CỦA CÁC KHÔNG GIAN CÓ THỂ MÊTRIC HÓA ĐƯỢC

Nếu $X$ là một không gian có thể mêtric hóa được và $R$ là một quan hệ tương đương trên $X$, không gian thương $X/R$ không nhất thiết có thể mêtric hóa được (ngay cả khi $X$ là compact địa phương \* và $X/R$ là chuẩn tắc *). Tuy nhiên:

#### Mệnh đề 17 {#top-ix-s2-prop-17 .statement}

Mọi không gian thương Hausdorff của một không gian compact có thể mêtric hóa được đều compact và có thể mêtric hóa được.

Tương đương, nếu $f$ là một ánh xạ liên tục từ một không gian compact mêtric $X$ vào một không gian Hausdorff $X'$, thì $f(X)$ là một không gian con mêtric của $X'$ (Chương I, § 9, no. 4, Định lý 2, Hệ quả 4).

Cho $X$ là một không gian compact mêtric, và cho $R$ là một quan hệ tương đương trên $X$ sao cho $X/R$ là Hausdorff. Khi đó $X/R$ là compact (Chương I, § 9, no. 4, Định lý 2), do đó theo Mệnh đề 16 chỉ cần chỉ ra rằng tôpô của $X/R$ có một cơ sở đếm được. Để làm điều này, ta sử dụng các sự kiện rằng $R$ là đóng (Chương I, § 10, no. 4, Mệnh đề 8) và các lớp mod $R$ là compact. Gọi $\varphi$ là ánh xạ chính tắc của $X$ lên $X/R$, và gọi $(U_n)$ là một cơ sở đếm được của tôpô của $X$. Cho $z$ là một điểm bất kỳ của $X/R$ và cho $V$ là một lân cận của $z$ trong $X/R$; khi đó $\overline{\varphi}^{-1}(V)$ là một lân cận trong $X$ của tập compact $\overline{\varphi}^{-1}(z)$. Nếu $x$ là một điểm bất kỳ của $\overline{\varphi}^{-1}(z)$, thì có một tập hợp $U_n$ chứa $x$ và được chứa trong $\overline{\varphi}^{-1}(V)$, và do đó theo tiên đề Borel-Lebesgue có một phủ mở hữu hạn $(U_{n_k})_{1 \leq k \leq r}$ của $\overline{\varphi}^{-1}(z)$ sao cho, nếu $W$ ký hiệu $\bigcup_k U_{n_k}$, thì $W$ là một lân cận của $\overline{\varphi}^{-1}(z)$ được chứa trong $\overline{\varphi}^{-1}(V)$. Vì $R$ là đóng, suy ra rằng $\varphi(W)$ là một lân cận của $z$ trong $X/R$, được chứa trong $V$ (Chương I, § 5, no. 4, Mệnh đề 10). Gọi $\mathcal{B}$ là tập hợp các phần trong của các tập hợp có dạng $\varphi(W)$, trong đó $W$ chạy qua tập hợp $\mathcal{F}$ của tất cả các hợp hữu hạn của các tập hợp có dạng $U_n$; khi đó ta đã chứng minh rằng $\mathcal{B}$ là một cơ sở của tôpô của $X/R$, và vì $\mathfrak{F}$ là đếm được, nên $\mathcal{B}$ cũng vậy.

#### Mệnh đề 18 {#top-ix-s2-prop-18 .statement}

*Cho $X$ là một không gian metric đầy đủ, cho $R$ là một quan hệ tương đương mở trên $X$ sao cho $X/R$ là Hausdorff, và cho $\varphi : X \to X/R$ là ánh xạ chính tắc. Khi đó nếu $K$ là một tập con compact bất kỳ của $X/R$, thì tồn tại một tập con compact $K'$ của $X$ sao cho $\varphi(K') = K$.*

Ký hiệu $\mathcal{B}_1$ là tập hợp tất cả các quả cầu mở bán kính $1/2$ trong $X$. Khi $B$ chạy qua $\mathcal{B}_1$, các tập hợp $\varphi(B)$ tạo thành một phủ mở của $K$, và do đó tồn tại một số hữu hạn điểm $x_1, \ldots, x_m$ của $X$ sao cho các ảnh qua $\varphi$ của các quả cầu mở bán kính $1/2$ và tâm $x_i$ ($1 \leq i \leq m$) tạo thành một phủ mở của $K$. Đặt $H_1 = \{ x_1, \ldots, x_m \}$ và giả sử rằng ta đã xác định được một tập hợp hữu hạn $H_i$, với $1 < i \leq n$, sao cho:

(i) $H_i \subset H_{i+1}$ và mỗi điểm của $H_{i+1}$ cách $H_i$ một khoảng cách $< 1/2^i$, với $1 \leq i \leq n - 1$;

(ii) các ảnh qua $\varphi$ của các quả cầu mở bán kính $1/2^i$, có tâm tại các điểm của $H_i$, tạo thành một phủ mở của $K$, với $1 \leq i \leq n$.

Cho $\mathcal{B}_{n+1}$ là tập hợp tất cả các quả cầu mở bán kính $1/2^{n+1}$ có tâm $x$ sao cho $d(x, H_n) < 1/2^n$ ($d$ là mêtric trên $X$). Các tính chất của $H_n$ cho thấy rằng các tập hợp $\varphi(B)$, với $B \in \mathcal{B}_{n+1}$, tạo thành một phủ mở của $K$; do đó tồn tại một tập hợp hữu hạn $L_{n+1} \subset X$ sao cho ảnh qua $\varphi$ của các quả cầu mở bán kính $1/2^{n+1}$ có tâm thuộc $L_{n+1}$ tạo thành một phủ mở của $K$. Lấy $H_{n+1} = H_n \cup L_{n+1}$, ta thấy rằng ta có thể định nghĩa quy nạp một dãy vô hạn $(H_n)$ gồm các tập con hữu hạn của $X$ có các tính chất (i) và (ii) ở trên. Đặt $H = \bigcup_n H_n$, và ta hãy chứng minh rằng $H$ là *tiền compact*. Với mỗi $p > 0$ và mỗi điểm $z_{n+p} \in H_{n+p}$, tồn tại một dãy các điểm $z_{n+i} \in H_{n+i}$ ($0 \leq i \leq p - 1$) sao cho

$$
d(z_{n+i}, z_{n+i+1}) < 1/2^{n+i} \quad \text{với } 0 \leq i \leq p - 1;
$$

suy ra rằng $d(z_n, z_{n+p}) \leq \sum_{i=0}^{p-1} 1/2^{n+i} \leq 1/2^{n-1}$, và do đó $d(y, H_n) \leq 1/2^{n-1}$ với mọi $y \in H$, điều này chứng minh khẳng định của ta. Vì $X$ là đầy đủ, $\overline{H}$ là compact, do đó $\varphi(\overline{H})$ là compact. Tiếp theo, ta hãy chứng minh rằng $K \subset \varphi(\overline{H})$. Nếu $z \in K$, thì theo định nghĩa $d(\overline{H}_n, \overline{\varphi}(z)) \leq 1/2^n$ với mọi $n$, và vì thế $d(\overline{H}, \overline{\varphi}(z)) = 0$; nhưng $\overline{\varphi}(z)$ là đóng và $\overline{H}$ là compact, nên điều này kéo theo $\overline{H} \cap \overline{\varphi}(z) \neq \emptyset$ (no. 2, Nhận xét sau Mệnh đề 3); do đó khẳng định được chứng minh. Vậy nếu $K' = \overline{H} \cap \overline{\varphi}(K)$, thì $K'$ là đóng trong $\overline{H}$ và do đó compact, và từ những gì đã được chứng minh ta có $\varphi(K') = K$.

Q.E.D.

### Bài tập {#top-ix-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
