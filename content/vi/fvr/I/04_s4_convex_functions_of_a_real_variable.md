---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 4
section_title: CONVEX FUNCTIONS OF A REAL VARIABLE
lang: vi
source: fvr-i-vii
pdf_pages: 0038-0048, 0060-0064
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A CONVEX FUNCTION
      page: 0
      pdf_page: 39
    - "no": 2
      title: FAMILIES OF CONVEX FUNCTIONS
      page: 0
      pdf_page: 42
    - "no": 3
      title: CONTINUITY AND DIFFERENTIABILITY OF CONVEX FUNCTIONS
      page: 0
      pdf_page: 42
    - "no": 4
      title: CRITERIA FOR CONVEXITY
      page: 0
      pdf_page: 45
statements: 21
exercises: 10
content_sha256: 27f70da6f0afe4eb5afa2ceef4ad82fae3ee56e2eb658f5adee5d5cf1e6fafe0
translated_from: content/en/fvr/I/04_s4_convex_functions_of_a_real_variable.md
source_content_sha256: 7ce62adb175e316461e0076f49e0da867be5dc77b36f37f3c179a2545bb96dd9
translation_model: gpt-5.4
translation_run: translate-vi-a606d333
glossary_version: 34
glossary_terms_sha256: 0c5757d239d406ae4cda45b0660308d901e0952337a3832bbcfb520509d0d59e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. HÀM LỒI CỦA MỘT BIẾN THỰC

Cho $H$ là một tập con của $\mathbf{R}$. $f$ là một hàm thực hữu hạn xác định trên $H$, và gọi $G$ là *đồ thị* hay tập đại diện của hàm $f$ trong $\mathbf{R} \times \mathbf{R} = \mathbf{R}^2$, tức là tập hợp các điểm $M_x = (x, f(x))$, khi $x$ chạy qua $H$. Thật tiện khi nói rằng một điểm $(a, b)$ của $\mathbf{R}^2$ sao cho $a \in H$ nằm *trên* (hoặc *strictly above*, *dưới*, *strictly below*) $G$ nếu ta có $b \geq f(a)$ (hoặc $b > f(a)$, $b \leq f(a)$, $b < f(a)$). Nếu $A = (a, a')$ và $B = (b, b')$ là hai điểm của $\mathbf{R}^2$ thì ta ký hiệu bởi $AB$ đoạn đóng có các đầu mút là $A$ và $B$; nếu $a < b$ thì $AB$ là đồ thị của hàm tuyến tính $a' + \frac{b' - a'}{b - a} (x - a)$ xác định trên $[a, b]$; ta ký hiệu hệ số góc $\frac{b' - a'}{b - a}$ của đoạn này bởi $p(AB)$, và sẽ dùng bổ đề sau đây, mà việc kiểm tra là ngay lập tức:

#### Bổ đề {#fvr-i-s4-n0-lem-1 .statement}

*Cho $A = (a, a')$, $B = (b, b')$, $C = (c, c')$ là ba điểm trong $\mathbf{R}^2$ sao cho $a < b < c$. Các mệnh đề sau là tương đương:*

a) *B ở dưới AC;*
b) *C nằm phía trên đường thẳng đi qua A và B;*
c) *A nằm phía trên đường thẳng đi qua B và C;*
d) $p(AB) \leq p(AC)$;
e) $p(AC) \leq p(BC)$.

Bổ đề vẫn còn đúng khi thay "phía trên" (resp. "phía dưới") bằng "phía trên hẳn" (resp. "phía dưới hẳn") và dấu $\leq$ bằng < (hình 1).

![Đồ thị biểu diễn các điểm A, B, C, và các đoạn được ghi nhãn với các giá trị x a, b, c](../images/fig_1.png)

Hình 1

### 1. ĐỊNH NGHĨA CỦA MỘT HÀM LỒI

#### Định nghĩa 1 {#fvr-i-s4-def-1 .statement}

Ta nói rằng một hàm số $f$ hữu hạn, xác định trên một khoảng $I \subset \mathbf{R}$, là lồi trên $I$ nếu, bất kể các điểm $x, x'$ của $I$, ($x < x'$), mọi điểm $M_z$ của đồ thị $G$ của $f$ sao cho $x \leq z \leq x'$ đều nằm dưới đoạn thẳng $M_xM_{x'}$ (hay, điều đó cũng tương đương, nếu mọi điểm của đoạn thẳng này đều nằm trên $G$) (hình 2).

![Đồ thị biểu diễn các điểm M_x, M_z, M_{x'}, và đường cong G](../images/fig_2.png)

Hình 2

Tính đến biểu diễn tham số của một đoạn thẳng (Gen. Top., VI, p. 35), điều kiện để $f$ lồi trên I là có bất đẳng thức

$$
f(\lambda x + (1 - \lambda)x') \leq \lambda f(x) + (1 - \lambda)f(x')
$$

đối với mỗi cặp điểm $(x, x')$ của I và mọi $\lambda \in [0, 1]$.

Định nghĩa 1 tương đương với điều sau đây: *tập hợp các điểm của $\mathbf{R}^2$ nằm phía trên đồ thị G của $f$ là lồi*. Thật vậy, điều kiện này rõ ràng là đủ để $f$ lồi trên I; nó cũng là cần thiết, vì nếu $f$ lồi trên I, và nếu $(x, y), (x', y')$ là hai điểm nằm phía trên G, thì ta có $y \geq f(x),\ y' \geq f(x')$, từ đó, với $0 \leq \lambda \leq 1$,

$$
\lambda y + (1 - \lambda)y' \geq \lambda f(x) + (1 - \lambda)f(x') \geq f(\lambda x + (1 - \lambda)x')
$$

theo (1), điều đó cho thấy rằng mọi điểm của đoạn thẳng có các đầu mút là $(x, y)$ và $(x', y')$ đều nằm phía trên G.

#### Nhận xét {#fvr-i-s4-n1-rem-1 .statement}

Ta cũng thấy theo cùng một cách rằng tập hợp các điểm nằm *nghiêm ngặt phía trên* G là lồi. Ngược lại, nếu tập hợp này là lồi thì ta có

$$
\lambda y + (1 - \lambda)y' > f(\lambda x + (1 - \lambda)x')
$$

với $0 \leq \lambda \leq 1$ và $y > f(x),\ y' > f(x')$; khi cho y tiến tới $f(x)$ và $y'$ tiến tới $f(x')$ trong công thức này thì suy ra $f$ là lồi.

#### Ví dụ 1 {#fvr-i-s4-n1-exa-1 .statement}

Mọi hàm afin tuyến tính (thực) $ax + b$ đều lồi trên $\mathbf{R}$.
2) Hàm $x^2$ lồi trên $\mathbf{R}$, vì ta có

$$
\lambda x^2 + (1 - \lambda)(x')^2 - \left( \lambda x + (1 - \lambda)x' \right)^2 = \lambda(1 - \lambda)(x - x')^2 \geq 0
$$

với $0 \leq \lambda \leq 1$.
3) Hàm $|x|$ lồi trên $\mathbf{R}$, vì

$$
|\lambda x + (1 - \lambda)x'| \leq \lambda |x| + (1 - \lambda)|x'|
$$

với $0 \leq \lambda \leq 1$.

Hiển nhiên là nếu $f$ lồi trên I, thì hạn chế của nó trên mọi khoảng $J \subset I$ đều lồi trên J.

Cho $f$ là một hàm lồi trên I, và $x, x'$ là hai điểm của I sao cho $x < x'$; nếu $z \in I$ là *ở ngoài* $[x, x']$ thì $M_z$ nằm *phía trên* đường thẳng D nối $M_x$ và $M_{x'}$; đây là một hệ quả ngay lập tức của bổ đề.

Từ đó suy ra rằng nếu $z$ là một điểm sao cho $x < z < x'$ và sao cho $M_z$ nằm *trên* đoạn thẳng $M_x M_{x'}$, thì, với *mọi điểm khác* $z'$ sao cho $x < z' < x'$, điểm $M_{z'}$ cũng nằm *trên* đoạn thẳng $M_x M_{x'}$, vì từ điều trên suy ra rằng $M_{z'}$ đồng thời vừa ở trên vừa ở dưới đoạn thẳng này; nói cách khác, khi đó $f$ bằng một hàm *tuyến tính afin* trên $[x, x']$.

#### Định nghĩa 2 {#fvr-i-s4-def-2 .statement}

*Ta nói rằng một hàm thực hữu hạn $f$ xác định trên một khoảng $I \subset \mathbf{R}$ là lồi nghiêm ngặt trên I nếu, với mọi điểm $x, x'$ của I ($x < x'$), mọi điểm $M_z$ của đồ thị G của $f$ sao cho $x < z < x'$ đều nằm hẳn bên dưới đoạn $M_x M_{x'}$ (hay, cũng tương đương như vậy, nếu mọi điểm của đoạn ấy, trừ các đầu mút, đều nằm hẳn bên trên G).*

Nói cách khác, ta phải có bất đẳng thức

$$
f(\lambda x + (1 - \lambda)x') < \lambda f(x) + (1 - \lambda)f(x')
$$

với mọi cặp điểm phân biệt $(x, x')$ của $I$ và mọi $\lambda$ sao cho $0 < \lambda < 1$.

Các nhận xét đứng trước đ.n. 2 cho thấy rằng để một hàm lồi $f$ là lồi chặt trên $I$ thì điều kiện cần và đủ là không có khoảng nào được chứa trong $I$ (không thu về một điểm duy nhất) sao cho hạn chế của $f$ lên khoảng này là *afin tuyến tính*.

Trong các ví dụ trên, ví dụ thứ nhất và thứ ba không lồi chặt; mặt khác, $x^2$ lồi chặt trên $\mathbf{R}$; một phép tính tương tự cho thấy rằng $1/x$ lồi chặt trên $[0, +\infty[$.

#### Mệnh đề 1 {#fvr-i-s4-prop-1 .statement}

*Cho $f$ là một hàm thực hữu hạn, lồi (resp. lồi nghiêm ngặt) trên một khoảng $I \subset \mathbf{R}$. Với mọi họ $(x_i)_{1 \leq i \leq p}$ gồm $p \geq 2$ điểm phân biệt của $I$, và mọi họ $(\lambda_i)_{1 \leq i \leq p}$ gồm $p$ số thực sao cho $0 < \lambda_i < 1$ và $\sum_{i=1}^p \lambda_i = 1$, ta có*

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i)
$$

(resp.

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i)).
$$

Vì mệnh đề (đối với các hàm lồi) quy về bất đẳng thức (1) với $p = 2$ nên ta lập luận bằng quy nạp đối với $p > 2$. Số $\mu = \sum_{i=1}^{p-1} \lambda_i$ là $> 0$; ngay lập tức thấy rằng nếu $a$ và $b$ là các giá trị nhỏ nhất và lớn nhất trong các $x_i$ thì $a \leq \frac{\sum_{i=1}^{p-1} \lambda_i x_i}{\sum_{i=1}^{p-1} \lambda_i} \leq b$; nói cách khác, điểm $x = \frac{1}{\mu} \sum_{i=1}^{p-1} \lambda_i x_i$ thuộc $I$, và giả thiết quy nạp kéo theo $\mu f(x) \leq \sum_{i=1}^{p-1} \lambda_i f(x_i)$; hơn nữa, từ (1) ta có rằng

$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) = f(\mu x + (1 - \mu)x_p) \leq \mu f(x) + (1 - \mu)f(x_p) \leq \sum_{i=1}^p \lambda_i f(x_i).
$$

Ta cũng lập luận theo cùng một cách đối với các hàm lồi nghiêm ngặt, bắt đầu từ bất đẳng thức (2).

Ta nói rằng một hàm thực hữu hạn $f$ là *lõm* (resp. *lõm nghiêm ngặt*) trên $I$ nếu $-f$ là lồi (resp. lồi nghiêm ngặt) trên $I$. Điều đó tương đương với việc nói rằng với mọi cặp $(x, x')$ điểm phân biệt của $I$ và mọi $\lambda$ sao cho $0 < \lambda < 1$ ta có

$$
f(\lambda x + (1 - \lambda)x') \geq \lambda f(x) + (1 - \lambda)f(x')
$$

(resp. $f(\lambda x + (1 - \lambda)x') > \lambda f(x) + (1 - \lambda)f(x')$).

### 2. HỌ CÁC HÀM LỒI

#### Mệnh đề 2 {#fvr-i-s4-prop-2 .statement}

Cho $f_i$ ($1 \leq i \leq p$) là $p$ hàm lồi trên một khoảng $I \subset \mathbf{R}$, và $c_i$ ($1 \leq i \leq p$) là $p$ số dương tùy ý; khi đó hàm $f = \sum_{i=1}^p c_i f_i$ là lồi trên $I$. Hơn nữa, nếu đối với ít nhất một chỉ số $j$ thì hàm $f_j$ là lồi chặt trên $I$, và $c_j > 0$, thì $f$ là lồi chặt trên $I$.

Điều này suy ra ngay lập tức bằng cách áp dụng bất đẳng thức (1) (tương ứng (2)) cho mỗi $f_i$, nhân bất đẳng thức đối với $f_i$ với $c_i$, rồi sau đó cộng theo từng số hạng.

#### Mệnh đề 3 {#fvr-i-s4-prop-3 .statement}

Cho $(f_\alpha)$ là một họ các hàm lồi trên một khoảng $I \subset \mathbf{R}$; nếu bao trên $g$ của họ này là hữu hạn tại mọi điểm của $I$ thì $g$ là lồi trên $I$.

Thật vậy, tập hợp các điểm $(x, y) \in \mathbf{R}^2$ nằm phía trên đồ thị của $g$ là giao của các tập hợp lồi tạo thành bởi các điểm nằm phía trên đồ thị của mỗi hàm $f_\alpha$; do đó nó là lồi.

#### Mệnh đề 4 {#fvr-i-s4-prop-4 .statement}

Cho $H$ là một tập hợp các hàm lồi trên một khoảng $I \subset \mathbf{R}$; nếu $\mathfrak{F}$ là một bộ lọc trên $H$ hội tụ từng điểm trên $I$ tới một hàm thực hữu hạn $f_0$, thì hàm này là lồi trên $I$.

Để thấy điều đó, chỉ cần chuyển sang giới hạn theo $\mathfrak{F}$ trong bất đẳng thức (1).

### 3. TÍNH LIÊN TỤC VÀ KHẢ VI CỦA CÁC HÀM LỒI

#### Mệnh đề 5 {#fvr-i-s4-prop-5 .statement}

Điều kiện cần và đủ để một hàm thực hữu hạn $f$ là lồi (tương ứng, lồi ngặt) trên một khoảng $I$ là với mọi $a \in I$, hệ số góc

$$
p(M_a M_x) = \frac{f(x) - f(a)}{x - a}
$$

là một hàm tăng (tương ứng, tăng ngặt) theo $x$ trên $I \cap \mathbf{C}\{a\}$.

Mệnh đề này là một hệ quả ngay lập tức của các định nghĩa 1 và 2 và của bổ đề ở I, p. 23.

#### Mệnh đề 6 {#fvr-i-s4-prop-6 .statement}

Cho $f$ là một hàm thực hữu hạn lồi trên một khoảng $I \subset \mathbf{R}$. Khi đó tại mọi điểm trong $a$ của $I$ hàm $f$ liên tục, có các đạo hàm phải và trái hữu hạn, và $f'_g(a) \leq f'_d(a)$.

Thật vậy, với $x \in I$ và $x > a$ hàm $x \mapsto \frac{f(x) - f(a)}{x - a}$ là tăng (mệnh đề 5) và bị chặn dưới, vì nếu $y < a$ và $y \in I$ thì ta có

$$
\frac{f(y) - f(a)}{y - a} \leq \frac{f(x) - f(a)}{x - a}
$$
(5)

theo mệnh đề 5; do đó hàm này có một giới hạn phải hữu hạn tại điểm $a$; nói cách khác, $f'_d(a)$ tồn tại và hữu hạn; hơn nữa, cho $x$ tiến tới $a$ ($x > a$) trong (5), suy ra rằng

$$
\frac{f(y) - f(a)}{y - a} \leq f'_d(a)
$$
(6)

với mọi $y < a$ thuộc I. Theo cùng một cách, ta chứng minh được rằng $f'_g(a)$ tồn tại và rằng

$$
f'_d(a) \leq \frac{f(x) - f(a)}{x - a}
$$
(7)

với $x \in I$ và $x > a$. Khi cho $x$ tiến tới $a$ ($x > a$) trong bất đẳng thức cuối cùng này, ta được $f'_g(a) \leq f'_d(a)$. Sự tồn tại của các đạo hàm trái và phải tại điểm $a$ rõ ràng bảo đảm tính liên tục của $f$ tại điểm này.

#### Hệ quả 1 {#fvr-i-s4-prop-6-cor-1 .statement}

*Nếu $f$ là một hàm lồi (tương ứng, lồi chặt) trên I; nếu $a$ và $b$ là hai điểm trong của I sao cho $a < b$ thì ta có* (hình 3)

![Một đồ thị biểu diễn một hàm lồi với các tiếp tuyến tại các điểm a và b, lần lượt được ký hiệu là M_a và M_b.](../images/fig_3.png)

Hình 3

$$
f'_d(a) \leq \frac{f(b) - f(a)}{b - a} \leq f'_g(b)
$$
(8)

(tương ứng,

$$
f'_d(a) < \frac{f(b) - f(a)}{b - a} < f'_g(b)
$$
(9)

Bất đẳng thức kép (8) suy ra từ (6) và (7) bằng một thay đổi ký hiệu đơn giản. Mặt khác, nếu $f$ lồi ngặt và $c$ sao cho $a < c < b$ thì ta có, từ (8) và mệnh đề 5,

$$
f'_d(a) \leq \frac{f(c) - f(a)}{c - a} < \frac{f(b) - f(a)}{b - a} < \frac{f(b) - f(c)}{b - c} \leq f'_g(b)
$$

từ đó suy ra (9).

#### Hệ quả 2 {#fvr-i-s4-prop-6-cor-2 .statement}

*Nếu $f$ lồi (ứng với lồi ngặt) trên I thì $f'_d$ và $f'_g$ tăng (ứng với tăng ngặt) trên phần trong của I; tập hợp các điểm của I tại đó $f$ không khả vi là đếm được, và $f'_d$ và $f'_g$ liên tục tại mọi điểm mà ở đó $f$ khả vi.*

Phần thứ nhất suy ra ngay lập tức từ (8) (ứng với (9)) và bất đẳng thức

$$
f'_g(a) \leq f'_d(a).
$$

Mặt khác, gọi E là tập hợp các điểm trong $x$ của I tại đó $f$ không khả vi (nghĩa là $f'_g(x) < f'_d(x)$). Với mỗi $x \in E$ gọi $J_x$ là khoảng mở $]f'_g(x), f'_d(x)[$; suy ra từ (8) rằng nếu $x$ và $y$ là hai điểm của E sao cho $x < y$, thì $u < v$ với mọi $u \in J_x$ và mọi $v \in J_y$; nói cách khác, khi $x$ chạy qua E thì các khoảng mở khác rỗng $J_x$ rời nhau từng đôi một; vì thế tập hợp các khoảng như vậy là đếm được, và do đó E cũng đếm được. Sau cùng, do $f'_d$ (tương ứng $f'_g$) tăng, nó có một giới hạn phải và một giới hạn trái tại mọi điểm trong $x$ của I; mệnh đề 6 của I, p. 18 khi đó cho thấy rằng giới hạn phải của $f'_d$ (tương ứng $f'_g$) tại điểm $x$ bằng $f'_d(x)$, và giới hạn trái của nó là $f'_g(x)$, từ đó suy ra phần cuối của hệ quả.

Cho $f$ là một hàm lồi trên I, $a$ là một điểm trong của I, và D là một đường thẳng chuyển qua điểm $M_a$, có phương trình $y - f(a) = \alpha(x - a)$. Từ các bất đẳng thức (8) suy ra rằng nếu $f'_g(a) \leq \alpha \leq f'_d(a)$ thì mọi điểm của đồ thị G đều nằm *phía trên* D, và, nếu $f$ là hàm lồi nghiêm ngặt, thì $M_a$ là điểm chung duy nhất của D và G; khi đó người ta nói rằng D là một *đường tựa* của G tại điểm $M_a$. Ngược lại, nếu G nằm phía trên D, ta có $f(x) - f(a) \geq \alpha(x - a)$ với mọi $x \in I$, từ đó suy ra $\frac{f(x) - f(a)}{x - a} \geq \alpha$ với $x > a$, và $\frac{f(x) - f(a)}{x - a} \leq \alpha$ với $x < a$; khi cho $x$ tiến tới $a$ trong các bất đẳng thức này, suy ra $f'_g(a) \leq \alpha \leq f'_d(a)$.

Đặc biệt, nếu $f$ khả vi tại điểm $a$ thì chỉ có *một và chỉ một* đường tựa của G tại điểm $M_a$, đó là *tiếp tuyến* của G tại $M_a$.

#### Nhận xét {#fvr-i-s4-n3-rem-1 .statement}

Nếu $f$ là một hàm lồi ngặt trên một khoảng mở I thì $f'_d$ tăng ngặt trên I, do đó có ba trường hợp có thể xảy ra, theo mệnh đề 2 của I, p. 13:
1. $f$ giảm nghiêm ngặt trên I;
2. $f$ tăng ngặt trên I;
3. tồn tại một $a \in I$ sao cho $f$ giảm nghiêm ngặt đối với $x \leq a$, và tăng ngặt đối với $x \geq a$.

Khi $f$ là lồi trên I, nhưng không lồi ngặt, thì $f$ có thể hằng trên một khoảng được chứa trong I; đặt $J = ]a, b[$ là khoảng mở lớn nhất mà trên đó $f$ hằng (nghĩa là, phần trong của khoảng mà trên đó $f'_d(x) = 0$); khi đó $f$ giảm nghiêm ngặt trên khoảng tạo bởi các điểm $x \in I$ sao cho $x \leq a$ (nếu nó tồn tại), tăng ngặt trên khoảng tạo bởi các điểm $x \in I$ sao cho $x \geq b$ (nếu nó tồn tại).

Trong mọi trường hợp, ta thấy rằng $f$ có một *giới hạn phải* tại đầu mút bên trái của $I$ (trong $\overline{\mathbf{R}}$), và một *giới hạn trái* tại đầu mút bên phải; các giới hạn này có thể là hữu hạn hoặc vô hạn (*xem* I, p. 46, bài tập 5, 6 và 7). Do lạm dụng ngôn ngữ, đôi khi người ta nói rằng hàm liên tục (với giá trị trong $\overline{\mathbf{R}}$), bằng $f$ trên phần trong của $I$, và được kéo dài bằng tính liên tục tới các đầu mút của $I$, là *lồi trên* $\overline{I}$.

### 4. CÁC TIÊU CHUẨN CỦA TÍNH LỒI

#### Mệnh đề 7 {#fvr-i-s4-prop-7 .statement}

*Cho $f$ là một hàm thực hữu hạn xác định trên một khoảng $I \subset \mathbf{R}$. Để $f$ lồi trên $I$, điều kiện cần và đủ là với mọi cặp số $a, b$ thuộc $I$ sao cho $a < b$, và với mọi số thực $\mu$, hàm $f(x) + \mu x$ đạt supremum của nó trên $[a, b]$ tại một trong hai điểm $a, b$.*

Điều kiện đó là *cần*; thật vậy, vì $\mu x$ lồi trên $\mathbf{R}$, nên hàm $f(x) + \mu x$ lồi trên $I$; do đó ta có thể quy về trường hợp $\mu = 0$. Khi đó, với
$$
x = \lambda a + (1 - \lambda) b \quad (0 \leq \lambda \leq 1),
$$
ta có
$$
f(x) \leq \lambda f(a) + (1 - \lambda) f(b) \leq \operatorname{Max}(f(a), f(b)).
$$

Điều kiện đó là *đủ*. Đặt $\mu = -\frac{f(b) - f(a)}{b - a}$ và $g(x) = f(x) + \mu x$; ta có $g(a) = g(b)$ và do đó $g(x) \leq g(a)$ với mọi $x \in [a, b]$, và có thể kiểm tra ngay lập tức rằng bất đẳng thức này tương đương với bất đẳng thức (1) khi thay $z$ bởi $a$ và $x'$ bởi $b$.

#### Mệnh đề 8 {#fvr-i-s4-prop-8 .statement}

*Để một hàm thực hữu hạn $f$ là lồi (tương ứng, lồi ngặt) trên một khoảng mở $I \subset \mathbf{R}$ thì điều kiện cần và đủ là nó liên tục trên $I$, có đạo hàm tại mọi điểm của phần bù $B$ trong $I$ của một tập con đếm được của khoảng này, và đạo hàm là tăng (tương ứng, tăng ngặt) trên $B$.*

Điều kiện là cần thiết, theo mệnh đề 6 và hệ quả 2 của nó (I, p. 27); ta hãy chỉ ra rằng nó là đủ. Vậy giả sử rằng $f'$ tăng trên $B$, và $f$ không lồi; khi đó tồn tại (I, p. 27, mệnh đề 5) ba điểm $a, b, c$ của $I$, sao cho $a < c < b$, và $\frac{f(c) - f(a)}{c - a} > \frac{f(b) - f(c)}{b - c}$; nhưng theo định lý giá trị trung bình (I, p. 14, định lý 1) ta có
$$
\frac{f(c) - f(a)}{c - a} \leq \sup_{x \in B,\ a < x < c} f'(x) \quad \text{và} \quad \frac{f(b) - f(c)}{b - c} \geq \inf_{x \in B,\ c < x < b} f'(x).
$$

Do đó ta có $\sup_{\lambda \in B,\ a < \lambda < c} f'(\lambda) > \inf_{\lambda \in B,\ c < \lambda < b} f'(\lambda)$, trái với giả thiết rằng $f'$ tăng trên $B$.

Nếu bây giờ ta giả sử rằng $f'$ tăng ngặt trên $B$, thì $f$ là lồi và không thể bằng một hàm tuyến tính afin trên bất kỳ khoảng mở nào được chứa trong $I$, vì khi đó $f'$ sẽ là hằng trên khoảng này, trái với giả thiết.

#### Hệ quả {#fvr-i-s4-n4-cor-1 .statement}

*Cho $f$ là một hàm thực hữu hạn, liên tục và khả vi hai lần trên một khoảng $I \subset \mathbf{R}$; để $f$ lồi trên $I$ thì điều kiện cần và đủ là $f''(x) \geqslant 0$ với mọi $x \in I$; để $f$ lồi nghiêm ngặt trên $I$ thì điều kiện cần và đủ là điều kiện trước được thỏa mãn và thêm nữa tập hợp các điểm $x \in I$ tại đó $f''(x) > 0$ là trù mật trong $I$.*

Điều này suy ra ngay lập tức từ mệnh đề trước, và từ hệ quả ở I, p. 14.

#### Ví dụ {#fvr-i-s4-n4-exa-1 .statement}

Trên khoảng ]$0, +\infty$ [ hàm $x^r$ ($r$ là một số thực bất kỳ) có đạo hàm bậc hai bằng $r(r-1)x^{-2}$; do đó nó là lồi nghiêm ngặt nếu $r > 1$ hoặc $r < 0$, và lõm nghiêm ngặt nếu $0 < r < 1$. \*

Để có thể phát biểu một tiêu chuẩn khác cho tính lồi, ta đưa ra định nghĩa sau đây: cho đồ thị $G$ của một hàm thực hữu hạn xác định trên một khoảng $I \subset \mathbf{R}$ và một điểm trong $a$ của $I$, ta sẽ nói rằng một đường thẳng $D$ chuyển qua $M_a = (a, f(a))$ là *ở trên một cách địa phương* (resp. *ở dưới một cách địa phương*) đối với $G$ nếu tồn tại một lân cận $V \subset I$ của $a$ sao cho mọi điểm của $D$ được chứa trong $V \times \mathbf{R}$ đều ở trên (resp. ở dưới) $G$; ta sẽ nói rằng $D$ là *nằm trên một cách địa phương* $G$ tại điểm $M_a$ nếu có một lân cận $V \subset I$ của $a$ sao cho giao của $D$ và $V \times \mathbf{R}$ trùng với giao của $G$ và $V \times \mathbf{R}$ (nói cách khác, nếu $D$ đồng thời ở trên một cách địa phương và ở dưới một cách địa phương đối với $G$).

#### Mệnh đề 9 {#fvr-i-s4-prop-9 .statement}

*Cho $f$ là một hàm thực hữu hạn nửa liên tục trên trên một khoảng mở $I \subset \mathbf{R}$. Để $f$ lồi trên $I$ thì điều kiện cần và đủ là đối với mọi điểm $M_x$ của đồ thị $G$ của $f$, mọi đường thẳng ở địa phương nằm phía trên $G$ tại điểm này đều phải ở địa phương tựa trên $G$ (tại điểm $M_x$).*

Điều kiện này là *cần*: thật vậy, nếu $f$ là lồi trên $I$ thì tại mọi điểm $M_a$ của đồ thị $G$ của $f$ đều tồn tại một *đường tựa* $\Delta$ của $G$: khi đó $\Delta$ nằm dưới $G$, nên *a fortiori* nằm dưới $G$ một cách địa phương (I, p. 29); nếu một đường thẳng $D$ nằm trên $G$ một cách địa phương tại điểm $M_a$ thì nó nằm trên $\Delta$ một cách địa phương, nên phải trùng với $\Delta$, và do đó nằm trên $G$ một cách địa phương tại điểm $M_a$.

Điều kiện đó là *đủ*. Thật vậy, giả sử nó được thỏa mãn, và giả sử rằng $f$ không lồi trên $I$; khi đó tồn tại hai điểm $a, b$ của $I$ ($a < b$) sao cho có những điểm $M_x$ của $G$ nằm chặt phía trên đoạn thẳng $M_aM_b$ (hình 4). Nói cách khác, hàm $g(x) = f(x) - f(a) - \frac{f(b) - f(a)}{b - a}(x - a)$ nhận các giá trị $> 0$ trên $[a, b]$; vì $g$ hữu hạn và nửa liên tục trên trên khoảng compắc này nên cận trên nhỏ nhất $k$ của nó trên $[a, b]$ là hữu hạn và $> 0$, và tập hợp $g^{-1}(k)$ là đóng và không rỗng (\emph{Gen. Top.}, IV, p. 361, định lý 3 và mệnh đề 1). Gọi $c$ là cận dưới lớn nhất của $g^{-1}(k)$; ta có $a < c < b$. và tại điểm $M_c$ đường thẳng D có phương trình $y = f(c) + \frac{f(b) - f(a)}{b - a}(x - c)$ nằm địa phương phía trên G; nhưng tại điểm này nó không thể địa phương nằm trên G, vì, với $a < x < c$, ta có $g(x) < k$, điều này có nghĩa là $M_x$ nằm chặt phía dưới D. Như vậy ta đã đi đến một mâu thuẫn, điều này thiết lập mệnh đề.

#### Hệ quả 1 {#fvr-i-s4-prop-9-cor-1 .statement}

*Để một hàm thực hữu hạn* $f$ *xác định trên một khoảng mở* $I \subset \mathbf{R}$ *và nửa liên tục trên trên* $I$ *là lồi trên* $I$ *thì điều kiện cần và đủ là với mọi* $x \in I$ *tồn tại một* $\varepsilon > 0$ *sao cho quan hệ* $|h| \leq \varepsilon$ *kéo theo*

$$
f(x) \leq \frac{1}{2} \left( f(x + h) + f(x - h) \right).
$$

Ta chỉ cần chứng minh rằng điều kiện ấy là *đủ*. Thật vậy, nếu tại một điểm $M_a$ của đồ thị G của $f$ một đường thẳng D ở địa phương nằm phía trên G, thì nó ở địa phương đi qua G tại điểm này; vì, trong trường hợp đối lại, chẳng hạn, một điểm $M_{a+h}$ sẽ nằm chặt dưới D, trong khi một điểm $M_{a-h}$ sẽ nằm dưới D: trung điểm của đoạn $M_{a-h}M_{a+h}$ khi đó sẽ nằm chặt trên D (hình 5), và, do giả thiết, $M_a$ *a fortiori* sẽ nằm chặt dưới D, điều này vô lý.

![Một đồ thị biểu diễn một hàm lồi với các điểm M_{a-h}, M_a, M_{a+h} và một đường tiếp tuyến ký hiệu D.](https://i.imgur.com/3Q5z5QG.png)

Hình 5

#### Hệ quả 2 {#fvr-i-s4-prop-9-cor-2 .statement}

*Cho $f$ là một hàm thực hữu hạn xác định trên một khoảng mở $I \subset \mathbf{R}$. Nếu với mọi điểm $x \in I$ đều có một khoảng mở $J_x \subset I$ chứa $x$ và sao cho hạn chế của $f$ trên $J_x$ là lồi trên $J_x$, thì $f$ là lồi trên $I$.*

Hiển nhiên là $f$ thỏa mãn tiêu chuẩn của mệnh đề 9.

### Bài tập {#fvr-i-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
