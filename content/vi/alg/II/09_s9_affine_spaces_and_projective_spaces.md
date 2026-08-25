---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 9
section_title: Affine spaces and projective spaces
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0349-0361, 0434-0441
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AFFINE SPACES
      page: 0
      pdf_page: 349
    - "no": 2
      title: BARYCENTRIC CALCULUS
      page: 0
      pdf_page: 350
    - "no": 3
      title: AFFINE LINEAR VARIETIES
      page: 0
      pdf_page: 351
    - "no": 4
      title: AFFINE LINEAR MAPPINGS
      page: 0
      pdf_page: 353
    - "no": 5
      title: DEFINITION OF PROJECTIVE SPACES
      page: 0
      pdf_page: 355
    - "no": 6
      title: HOMOGENEOUS COORDINATES
      page: 0
      pdf_page: 355
    - "no": 7
      title: PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 356
    - "no": 8
      title: PROJECTIVE COMPLETION OF AN AFFINE SPACE
      page: 0
      pdf_page: 357
    - "no": 9
      title: EXTENSION OF RATIONAL FUNCTIONS
      page: 0
      pdf_page: 358
    - "no": 10
      title: PROJECTIVE LINEAR MAPPINGS
      page: 0
      pdf_page: 359
    - "no": 11
      title: PROJECTIVE SPACE STRUCTURE
      page: 0
      pdf_page: 361
statements: 12
exercises: 6
content_sha256: 52e572fe5a884b5a9f261bca524626851a8fe46b620eceef422c3867ecfb2b8b
translated_from: content/en/alg/II/09_s9_affine_spaces_and_projective_spaces.md
source_content_sha256: e3465293943c05dcb209132b84aeaca7762277abbf514e5ef69a8e26ea9f9804
translation_model: gpt-5.4-mini
translation_run: translate-vi-57309ea3
glossary_version: 34
glossary_terms_sha256: 8525c8eb162f10d53ba5038655ac122c3844e7ca7a4f34c0f9dad833e8daeb46
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. KHÔNG GIAN AFFINE VÀ KHÔNG GIAN XẠ ẢNH

### 1. ĐỊNH NGHĨA VỀ KHÔNG GIAN AFFINE

#### Định nghĩa 1 {#alg-ii-s9-def-1 .statement}

*Cho một không gian vectơ trái (resp. phải) T trên một trường K, một không gian affine gắn với T là bất kỳ không gian thuần nhất E của nhóm cộng T* (I, § 5, no. 5) *sao cho 0 là toán tử duy nhất trong T giữ bất biến mọi phần tử của E* (nghĩa là, T *tác động trung thành và bắc cầu trên E*). *Trong các điều kiện này, T được gọi là không gian tịnh tiến của E và các phần tử của nó được gọi là các phép tịnh tiến của E* (hay *các vectơ tự do của E*).

Trong phần tiếp theo, ta sẽ chỉ xét trường hợp T là một không gian vectơ trái trên K. Chiều (trên K) của không gian vectơ tịnh tiến T của một không gian affine được gọi là *chiều* của E (trên K) và được ký hiệu bởi dim E hoặc $ \dim_K E $. Một không gian affine có chiều một (resp. hai) được gọi là một *đường thẳng affine* (resp. một *mặt phẳng affine*). Các phần tử của một không gian affine cũng được gọi là *điểm*.

Dưới các điều kiện của Định nghĩa 1, với $ t \in T $ và $ a \in E $ ta sẽ ký hiệu bởi $ t + a $ hoặc $ a + t $ ảnh của điểm a dưới t. Khi đó các quan hệ

$$
s + (t + a) = (s + t) + a, \quad 0 + a = a
$$

đúng với $ s \in T, t \in T, a \in E $. Ánh xạ $ x \mapsto x + t $ là một song ánh của E lên chính nó, và ta đồng nhất nó với t. Định nghĩa 1 hơn nữa suy ra rằng, với mọi $ a \in E $, ánh xạ $ t \mapsto t + a $ là một *song ánh* của T lên E. Nói cách khác, cho hai điểm $ a, b $ của E, tồn tại một và chỉ một phép tịnh tiến t sao cho $ b = t + a $; ta sẽ ký hiệu phép tịnh tiến này bởi $ b - a $; khi đó các công thức

$$
a - a = 0, \quad a - b = -(b - a), \quad b = (b - a) + a
$$
$$
(c - b) + (b - a) = c - a
$$

đúng với $ a \in E, b \in E, c \in E $. Nếu bốn điểm $ a, b, a', b' $ của E sao cho $ b - a = b' - a' $, thì công thức

$$
b' = (b' - b) + (b - a) + a = (b' - a') + (a' - a) + a
$$

và tính giao hoán của phép cộng trong T cho thấy rằng $ b' - b = a' - a $.

Cho một điểm $ a \in E $, ánh xạ $ x \mapsto x - a $ là một song ánh của $ E $ lên $ T $; khi E được đồng nhất với T qua ánh xạ này, ta nói rằng E được xem như không gian vectơ thu được *bằng cách lấy $ a $ làm gốc* trong $ E $. Ngược lại, mọi không gian vectơ T đều có một cách chính tắc cấu trúc của một không gian affine gắn với T, cụ thể là cấu trúc không gian thuần nhất tương ứng với nhóm con $ \{0\} $ của T (I, § 5, no. 6).

#### Nhận xét {#alg-ii-s9-n1-rem-1 .statement}

Các định nghĩa của số này và một số kết quả sau đây mở rộng ngay lập tức sang trường hợp, thay vì một không gian vectơ $ T $, ta xét một *nhóm giao hoán có toán tử* tùy ý $ T $.

### 2. PHÉP TÍNH TRỌNG TÂM

#### Mệnh đề 1 {#alg-ii-s9-prop-1 .statement}

*Cho* $ (x_i)_{i \in I} $ *là một họ các điểm trong một không gian affine* E *và* $ (\lambda_i)_{i \in L} $ *là một họ các phần tử của* K *có giá hữu hạn sao cho* $ \sum_{i \in I} \lambda_i = 1 $ *(*resp. $ \sum_{i \in I} \lambda_i = 0 $*). *Nếu* $ a $ *là một điểm bất kỳ của* E, *điểm* $ x \in E $ *được xác định bởi*
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*(resp. vectơ tự do* $ \sum_{i \in I} \lambda_i (x_i - a) $) *không phụ thuộc vào điểm được xét.*

Nếu $ a' $ là một điểm khác của E, thì
$$
\sum_i \lambda_i (x_i - a') = \sum_i \lambda_i ((x_i - a) + (a - a')) = \sum_i \lambda_i (x - a) + \left( \sum_i \lambda_i \right) (a - a').
$$
Nếu $ \sum_i \lambda_i = 1 $, thì $ \sum_i \lambda_i (x_i - a) = (x - a) + (a - a') = x - a' $; nếu $ \sum_i \lambda_i = 0 $, thì $ \sum_i \lambda_i (x - a') = \sum_i \lambda_i (x - a) $; do đó mệnh đề.

Dưới các điều kiện của Mệnh đề 1, điểm $ x $ được xác định bởi
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*(resp. vectơ tự do* $ \sum_{i \in I} \lambda_i (x_i - a) $) *được ký hiệu bởi* $ \sum_{i \in I} \lambda_i x_i $.

Do đó, nói riêng, ký hiệu $ b - a $ được đưa vào ở no. 1 được khôi phục. Khi $ \sum_i \lambda_i = 1 $, điểm $ x = \sum_i \lambda_i x_i $ được gọi là *trọng tâm của các điểm* $ x_i $ *với các khối lượng* $ \lambda_i $.

Cho $ m $ điểm $ a_1, \ldots, a_m $ của $ E $, mà số $ m $ không là bội của đặc số của $ K $ (V, § 1), điểm $ g = \sum_{i=1}^m \frac{1}{m} a_i $ được gọi (theo một cách nói không chặt chẽ) là *trọng tâm của các điểm* $a_i$ ($1 \leq i \leq m$) (với $m = 2$, ta nói "trung điểm" thay vì "trọng tâm"); nó được đặc trưng bởi hệ thức
$$
\sum_{i=1}^m (a_i - g) = 0.
$$

### 3. CÁC DẠNG TUYẾN TÍNH AFFINE

#### Định nghĩa 2 {#alg-ii-s9-def-2 .statement}

*Cho một không gian affine* $E$, *một tập con* $V$ *của* $E$ *được gọi là một dạng tuyến tính affine* (hay đơn giản là một *dạng tuyến tính* hoặc một *tập con affine* của $E$) *nếu, với mọi họ* $(x_i)_{i \in I}$ *các điểm của* $V$ *và mọi họ* $(\lambda_i)_{i \in I}$ *các phần tử của* $K$ *có giá hữu hạn sao cho* $\sum_{i \in I} \lambda_i = 1$, *trọng tâm* $\sum_{i \in I} \lambda_i x_i$ *thuộc* $V$.

Cũng tương đương khi nói rằng điều kiện của Định nghĩa 2 đúng với mọi *họ hữu hạn* các điểm của $V$.

Tập rỗng là một dạng tuyến tính; mọi giao của các dạng tuyến tính đều là một dạng tuyến tính.

Cho $V$ là một tập con không rỗng của $E$ và $a$ là một điểm của $V$; hệ thức
$$
x - a = \sum_{i=1}^n \lambda_i (x_i - a)
$$
có nghĩa là $x$ là một trọng tâm $\sum_{i=1}^n \lambda_i x_i + \left(1 - \sum_{i=1}^n \lambda_i\right)a$ của họ gồm các $x_i$ và $a$. Do đó:

#### Mệnh đề 2 {#alg-ii-s9-prop-2 .statement}

*Để một tập con không rỗng* $V$ *của một không gian affine* $E$ *là một dạng tuyến tính, điều kiện cần và đủ là* $V$ *là một không gian con vectơ đối với cấu trúc không gian vectơ trên* $E$ *thu được bằng cách lấy một điểm của* $V$ *làm gốc.*

Đặc biệt, các dạng tuyến tính affine không rỗng của một không gian vectơ $T$ (được xem như một không gian affine) chỉ là các *tịnh tiến* của các không gian con vectơ của $T$; do đó các không gian con vectơ của $T$ là những dạng tuyến tính chứa 0.

Cho $V$ là một đa tạp tuyến tính không rỗng của không gian afin $E$; tập các vectơ tự do $x - y$, với $x$ và $y$ chạy qua $V$, là một không gian con vectơ $D$ của không gian tịnh tiến $T$ của $E$ được gọi là *phương* của $V$: vì, nếu $a \in V$, thì
$$
x - y = (x - a) - (y - a)
$$
và mệnh đề của ta suy ra từ Mệnh đề 2. Hiển nhiên $D$ tác động trung thành và bắc cầu lên $V$, do đó $V$ một cách chính tắc có cấu trúc của một *không gian afin gắn với* $D$. Theo *chiều* của đa tạp afin $V$, ta hiểu là chiều của $V$ với cấu trúc không gian afin này, tức là chiều của không gian vectơ $D$. Các đa tạp tuyến tính có chiều 0 là các điểm của $E$; các đa tạp có chiều 1 (tương ứng 2) được gọi là *đường thẳng* (tương ứng *mặt phẳng*) của $E$.

Mọi vectơ $ \neq 0 $ thuộc phương của một đường thẳng được gọi là một *vectơ phương* của đường thẳng này; các thành phần của nó đối với một cơ sở của T tạo thành cái gọi là một hệ *tham số phương* của đường thẳng nói trên.

*Đồng chiều* của một đa tạp tuyến tính V trong E là đồng chiều của phương D của nó trong T; một đa tạp tuyến tính có đồng chiều 1 trong E được gọi là một (afin) *siêu phẳng* của E.

Hai đa tạp tuyến tính có cùng phương được gọi là *song song*; nói rằng một đa tạp là dẫn xuất từ đa tạp kia bằng phép tịnh tiến cũng là như nhau. Nếu V là một đa tạp tuyến tính trong T (xem như một không gian afin), thì phương của nó là đa tạp tuyến tính song song với V và chứa 0.

#### Mệnh đề 3 {#alg-ii-s9-prop-3 .statement}

*Cho một họ* $(a_i)_{i \in I}$ *gồm các điểm của một không gian afin* E, *tập* V *các trọng tâm* $\sum_{i \in I} \lambda_i a_i$ *((\lambda_i) có giá hữu hạn, $\sum_{i \in I} \lambda_i = 1$) là một đa tạp tuyến tính của* E.

Nếu họ $(a_i)$ là rỗng, thì $V = \varnothing$ do điều kiện $\sum_i \lambda_i = 1$. Vì vậy có thể giả sử rằng họ $(a_i)$ không rỗng và trong trường hợp này mệnh đề là hiển nhiên, khi lấy một trong các $a_i$ làm gốc trong E.

Đa tạp V hiển nhiên là đa tạp tuyến tính nhỏ nhất chứa các $a_i$; nó được nói là *sinh* bởi họ $(a_i)$ và họ này được gọi là một *hệ sinh* của V.

Trong ký hiệu của Mệnh đề 3, giả sử họ $(a_i)$ là không rỗng, để biểu thức của mọi điểm $x \in V$ dưới dạng $x = \sum_i \lambda_i a_i$ là *duy nhất*, thì cần và đủ rằng, ký hiệu một chỉ số tùy ý của I bởi $\kappa$, họ các vectơ $a_i - a_\kappa$, với i chạy qua tập các chỉ số $\neq \kappa$, là tự do trong T. Khi đó họ $(a_v)_{v \in I}$ của các điểm của E được nói là *độc lập afin* (hoặc các phần tử của nó tạo thành một *hệ độc lập afin*, hoặc là *độc lập afin*) và rằng $\lambda_i$ là *tọa độ barycentric* của $x$ có chỉ số i đối với họ độc lập afin $(a_i)$.

Một họ $(a_i)_{i \in I}$ các điểm của E không độc lập afin được nói là *có quan hệ afin*.

#### Mệnh đề 4 {#alg-ii-s9-prop-4 .statement}

*Để một họ không rỗng* $(a_i)_{i \in I}$ *các điểm trong một không gian afin* E *là có quan hệ afin, thì cần và đủ rằng tồn tại một họ* $(\lambda_i)_{i \in I}$ *các phần tử không đồng thời bằng không trong* K, *có giá hữu hạn, sao cho* $\sum_{i \in I} \lambda_i = 0$ *và* $\sum_{i \in I} \lambda_i a_i = 0$.

Cho một chỉ số $\kappa \in I$, nói rằng họ các vectơ $(a_i - a_\kappa)$, với i chạy qua tập các chỉ số $\neq \kappa$, là có quan hệ trong T, nghĩa là tồn tại một họ các vô hướng $(\lambda_i)_{i \neq \kappa}$ không đồng thời bằng không sao cho $\sum_{i \neq \kappa} \lambda_i (a_i - a_\kappa) = 0$, điều này cũng có thể viết là $\sum_{i \in I} \lambda_i a_i = 0$, với $\lambda_\kappa = -\sum_{i \neq \kappa} \lambda_i$, nói cách khác $\sum_{i \in I} \lambda_i = 0$.

#### Mệnh đề 5 {#alg-ii-s9-prop-5 .statement}

==========

Với một họ không rỗng $(a_i)_{i \in I}$ các điểm của một không gian afin $E$, để nó là tự do afin, điều kiện cần và đủ là, với mọi chỉ số $\kappa \in I$, $a_\kappa$ không thuộc đa tạp tuyến tính được sinh bởi các $a_i$ có chỉ số $\neq \kappa$.

Mệnh đề hiển nhiên nếu $I$ chỉ có một phần tử duy nhất. Ngược lại, lấy làm gốc trong $E$ một trong các $a_i$ có chỉ số $\neq \kappa$, thì mệnh đề suy ra từ § 7, no. 1, Nhận xét.

### 4. ÁNH XẠ TUYẾN TÍNH AFFINE

#### Định nghĩa 3 {#alg-ii-s9-def-3 .statement}

Cho hai không gian afin $E, E'$ gắn với hai không gian vectơ $T, T'$ trên cùng một trường $K$, một ánh xạ $u$ của $E$ vào $E'$ được gọi là một ánh xạ tuyến tính affine (hay một ánh xạ affine) nếu, với mọi họ $(x_i)_{i \in I}$ các điểm của $E$ và mọi họ $(\lambda_i)_{i \in I}$ sao cho $\sum_{i \in I} \lambda_i = 1$,

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i).
$$

(3)

#### Mệnh đề 6 {#alg-ii-s9-prop-6 .statement}

Cho $u$ là một ánh xạ affine của $E$ vào $E'$. Có một và chỉ một ánh xạ tuyến tính $v$ của $T$ vào $T'$ sao cho

$$
u(x + t) = u(x) + v(t)
$$

với mọi $x \in E, t \in T$.

Cho $a$ là một điểm bất kỳ của $E$. Ánh xạ

$$
t \mapsto u(a + t) - u(a)
$$

là một ánh xạ tuyến tính $v_a$ của $T$ vào $T'$, vì ta có thể viết

$$
a + \lambda t = \lambda (a + t) + (1 - \lambda)a \\
a + s + t = (a + s) + (a + t) - a
$$

và từ (3) suy ra rằng $v_a(\lambda t) = \lambda v_a(t)$ và $v_a(s + t) = v_a(s) + v_a(t)$. Hơn nữa, nếu $b$ là một điểm khác của $E$, thì $v_a = v_b$; vì quan hệ

$$
(a + t) - a + b = b + t
$$

suy ra

$$
u(a + t) - u(a) + u(b) = u(b + t)
$$

tức là $u(a + t) - u(a) = u(b + t) - u(b)$. Do đó tồn tại $v$; tính duy nhất là ngay lập tức.

$v$ được gọi là ánh xạ tuyến tính của $T$ vào $T'$ liên kết với $u$. Ngược lại, với mọi ánh xạ tuyến tính $v$ của $T$ vào $T'$ và mọi cặp có thứ tự các điểm $a \in E, a' \in E'$, dễ dàng kiểm tra ngay lập tức rằng

$$
x \mapsto a' + v(x - a)
$$

là một ánh xạ affine của $E$ vào $E'$ mà ánh xạ tuyến tính liên kết là $v$. Nói rằng $u$ là một ánh xạ affine của $E$ vào $E'$ do đó cũng có nghĩa là, nếu lấy một điểm bất kỳ $a$ trong $E$ và điểm $u(a)$ trong $E'$ làm các gốc, thì $u$ là một ánh xạ tuyến tính đối với hai không gian vectơ thu được như vậy.

Cho $E''$ là một không gian afin thứ ba, $T''$ là không gian tịnh tiến của nó, $u'$ là một ánh xạ affine của $E'$ vào $E''$ và $v'$ là ánh xạ tuyến tính của $T'$ vào $T''$ liên kết với $u'$. Rõ ràng $u' o u$ là một ánh xạ affine của $E$ vào $E''$; hơn nữa, với $a \in E$ và $t \in T$,
$$
u'(u(a + t)) = u'(u(a) + v(t)) = u'(u(a)) + v'(v(t))
$$
và do đó $v' o v$ là ánh xạ tuyến tính của $T$ vào $T''$ liên kết với $u' o u$. Để một ánh xạ affine $u$ là song ánh, điều kiện cần và đủ là ánh xạ tuyến tính liên kết $v$ cũng như vậy, và khi đó $u^{-1}$ là một ánh xạ affine mà ánh xạ tuyến tính liên kết là $v^{-1}$.

Đặc biệt, các song ánh affine của $E$ lên chính nó tạo thành một nhóm $G$, gọi là nhóm affine của $E$. Ánh xạ gán với $u \in G$ ánh xạ tuyến tính $v$ liên kết với $u$ là, theo trên, một đồng cấu của $G$ lên nhóm tuyến tính $\mathbf{GL}(T)$. Nếu $u$ là một phép tịnh tiến, thì $v$ là phần tử đơn vị và ngược lại. Do đó, hạt nhân của đồng cấu trên là nhóm tịnh tiến $T$ của $E$, vì thế là một nhóm con chuẩn tắc của $G$.

Nếu $u \in G$, tự đẳng cấu $t \mapsto utu^{-1}$ của $T$ (trong đó $t$ được đồng nhất với phép tịnh tiến $x \mapsto x + t$) là ánh xạ tuyến tính $v$ liên kết với $u$. Với $x \in E$ và $t \in T$, theo định nghĩa
$$
x + utu^{-1} = u(u^{-1}(x) + t) = u(u^{-1}(x)) + v(t) = x + v(t)
$$
và do đó $utu^{-1} = v(t)$.

Cho $a \in E$ và $G_a$ là nhóm con của $G$ gồm các $u \in G$ sao cho $u(a) = a$. Nếu đồng nhất $E$ với $T$ bằng cách lấy $a$ làm gốc, thì $G_a$ được đồng nhất với $\mathbf{GL}(T)$. Mỗi $u \in G$ có thể được biểu diễn duy nhất dưới dạng $u = t_1u_1$ (hoặc dưới dạng $u = u_2t_2$), trong đó $u_1, u_2$ thuộc $G_a$ và $t_1, t_2$ thuộc $T$: thật vậy, viết $t_1 = u(a) - a$, $u^{-1}t_1 \in G_a$, do đó có $u_1$ và $t_1$; sự tồn tại của $u_2$ và $t_2$ thu được tương tự. Tính duy nhất theo từ thực tế rằng $G_a \cap T$ chỉ còn phần tử đơn vị của $G$. Hơn nữa
$$
t_1u_1 = u_1(u_1^{-1}t_1u_1)
$$
do đó $u_2 = u_1$, $t_2 = u_1^{-1}t_1u_1$. Sau cùng, các ánh xạ tuyến tính liên kết với $u$ và $u_1$ là như nhau và do đó, nếu như trên $G_a$ được đồng nhất với $\mathbf{GL}(T)$, thì $u_1$ là ánh xạ tuyến tính từ $T$ vào chính nó liên kết với $u$. Vì thế thấy rằng $G$ là tích nửa trực tiếp của $G_a$ bởi $T$ (I, § 6, no. 1).

### 5. Định nghĩa các không gian xạ ảnh

#### Định nghĩa 4 {#alg-ii-s9-def-4 .statement}

Cho E, E' là hai không gian afin trên K. Ảnh trực tiếp (resp. ảnh nghịch đảo) của một không gian con afin của E (resp. E') dưới một ánh xạ afin u của E vào E' là một không gian con afin của E' (resp. E); hạng của u theo định nghĩa là chiều của u(E); nó bằng hạng của ánh xạ tuyến tính liên kết với u. Nếu V, V' là các không gian con afin cùng chiều hữu hạn m trong E, E' tương ứng, thì tồn tại một ánh xạ afin $ u $ của $ E $ vào $ E' $ sao cho $ u(V) = V' $: lấy làm gốc trong $ E $ và $ E' $ lần lượt các điểm của $ V $ và $ V' $, rồi lấy trong $ E $ (resp. $ E' $) một cơ sở mà $ m $ vectơ đầu tiên tạo thành một cơ sở của $ V $ (resp. $ V' $), mệnh đề suy ra ngay từ § 1, no. 11, Hệ quả 3 của Mệnh đề 17.

Vì trường $ K $ có một cách chính tắc cấu trúc không gian vectơ trái (có chiều 1) trên $ K $, nên nó có thể được xem như một không gian afin có chiều 1. Một ánh xạ afin của một không gian afin $ D $ (trên $ K $) vào không gian afin $ K $ cũng được gọi là một *hàm tuyến tính afin* (hoặc một *hàm afin*). Nếu một điểm $ a $ được lấy làm gốc trong $ E $, thì mọi hàm afin trên $ E $ khi đó có thể được viết duy nhất dưới dạng $ x \mapsto \alpha + v(x) $, trong đó $ \alpha \in K $ và $ v $ là một dạng tuyến tính trên không gian vectơ $ E $ thu được như vậy; vì thế các hàm afin trên $ E $ tạo thành một *không gian vectơ phải trên* $ K $ có chiều $ 1 + \dim E $. Nếu $ u $ là một hàm afin không hằng trên $ E $ và $ \lambda \in K $, thì tập các $ x \in E $ thỏa mãn phương trình $ u(x) = \lambda $ là một siêu phẳng; ngược lại, với mỗi siêu phẳng $ H $ trong $ E $, tồn tại một hàm afin $ u_0 $ trên $ E $ sao cho $ H = u_0^{-1}(0) $ và mọi hàm afin $ u $ sao cho $ H = u^{-1}(0) $ đều có dạng $ u_0 \mu $, với $ \mu \in K $ (\S 7, no. 5, Mệnh đề 11). Nếu $ u $ là một hàm afin trên $ E $, thì các siêu phẳng có phương trình $ u(x) = \alpha $ và $ u(x) = \beta $ là song song.

*Cho một không gian vectơ trái (resp. phải)* $ V $ *trên một trường* $ K $, *không gian xạ ảnh trái (resp. phải) dẫn xuất từ* $ V $, *được ký hiệu bởi* $ \mathbf{P}(V) $, *là thương của phần bù* $ V - \{0\} $ *của* $ \{0\} $ *trong* $ V $ *theo quan hệ tương đương* $ \Delta(V) $ *"tồn tại* $ \lambda \neq 0 $ *trong* $ K $ *sao cho* $ y = \lambda x $ *(resp.* $ y = x \lambda$ )  *giữa* $ x $ *và* $ y $ *trong* $ V - \{0\} $.

Khi $ V = K_s^{n+1} $, ta cũng viết $ \mathbf{P}_n(K) $ thay cho $ \mathbf{P}(K_s^{n+1}) $ và $ \Delta_n(K) $ thay cho $ \Delta(V) $.

Định nghĩa 4 cũng có thể được phát biểu bằng cách nói rằng $ \mathbf{P}(V) $ là tập hợp các đường thẳng (đi qua 0) trong $ V $ với gốc bị bỏ đi; do đó $ \mathbf{P}(V) $ được đồng nhất một cách chính tắc với tập hợp các đường thẳng (đi qua 0) trong $ V $. Các phần tử của một không gian xạ ảnh được gọi là *các điểm* của không gian đó.

Khi $ V $ có chiều $ n $, số nguyên $ n - 1 $ được gọi là *chiều* của không gian xạ ảnh $ \mathbf{P}(V) $ nếu $ n $ hữu hạn, và là lực lượng $ n $ trong trường hợp ngược lại; lực lượng này được ký hiệu bởi $ \dim_K \mathbf{P}(V) $ hoặc $ \dim \mathbf{P}(V) $. Vậy một không gian xạ ảnh có chiều $ -1 $ là rỗng và một không gian xạ ảnh có chiều 0 là một điểm duy nhất. Một không gian xạ ảnh có chiều 1 (resp. 2) được gọi là một *đường thẳng xạ ảnh* (resp. *mặt phẳng xạ ảnh*).

Từ đây trở đi, ta sẽ chỉ xét các không gian xạ ảnh trái.

### 6. TỌA ĐỘ THUẦN NHẤT

Cho $ V $ là một không gian vectơ hữu hạn chiều $ n + 1 $ trên $ K $, $ \mathbf{P}(V) $ là không gian xạ ảnh có chiều $ n $ dẫn xuất từ $ V $ và $ (e_i)_{0 \leq i \leq n} $ là một cơ sở của $ V $. Ký hiệu $ \pi $ là ánh xạ chính tắc của $ V - \{0\} $ lên tập thương $ \mathbf{P}(V) $. Với mỗi điểm $ x = \sum_{i=0}^{n} \xi_i e_i $ của $ V - \{0\} $, $ (\xi_0, \xi_1, \ldots, \xi_n) $ được gọi là một *hệ tọa độ thuần nhất* của điểm $ \pi(x) $ đối với cơ sở $ (e_i) $ của $ V $. Vì vậy, mọi hệ $ (\xi_i) $ gồm $ n + 1 $ phần tử *không đồng thời bằng không* của $ K $ đều là một hệ tọa độ thuần nhất của một điểm của $ P(V) $ đối với $ (e_i) $; để hai hệ như thế $ (\xi_i) $, $ (\xi'_i) $ là các hệ tọa độ thuần nhất của cùng một điểm của $ P(V) $ đối với cùng một cơ sở $ (e_i) $, thì điều kiện cần và đủ là tồn tại một phần tử $ \lambda \neq 0 $ của $ K $ sao cho $ \xi'_i = \lambda \xi_i $ với $ 0 \leq i \leq n $.

Định nghĩa này được tổng quát hóa ngay lập tức cho trường hợp $ V $ là vô hạn chiều.

Cho một cơ sở khác $ (\tilde{e}_i) $ của $ V $ sao cho $ e_i = \sum_{j=0}^{n} \alpha_{ij} \tilde{e}_j $ ($ 0 \leq i \leq n $) và một hệ $ (\xi_i) $ tọa độ thuần nhất của $ \pi(x) $ đối với cơ sở $ (e_i) $, để một hệ $ (\bar{\xi}_i) $ gồm $ n + 1 $ phần tử của $ K $ là một hệ tọa độ thuần nhất của $ \pi(x) $ đối với cơ sở $ (\tilde{e}_i) $, điều kiện cần và đủ là tồn tại $ \lambda \neq 0 $ trong $ K $ sao cho

$$
\lambda \bar{\xi}_i = \sum_{j=0}^{n} \xi_j \alpha_{ji} \quad \text{for } 0 \leq i \leq n.
$$

Đặc biệt, nếu $ e_i = \gamma_i \tilde{e}_i $ với $ \gamma_i \neq 0 $ ($ 0 \leq i \leq n $), thì $ \bar{\xi}_i = \mu \xi_i \gamma_i $ với $ \mu \neq 0 $.

### 7. CÁC ĐA TẠP TUYẾN TÍNH XẠ ẢNH

Cho $ W $ là một không gian con vectơ của một không gian vectơ $ V $; ảnh chính tắc của $ W - \{0\} $ trong không gian xạ ảnh $ P(V) $ dẫn xuất từ $ V $ được gọi là một *đa tạp tuyến tính xạ ảnh* (hoặc đơn giản là một *đa tạp tuyến tính* khi không sợ nhầm lẫn); vì quan hệ tương đương $ \Delta(W) $ trên $ W - \{0\} $ là cảm sinh bởi quan hệ $ \Delta(V) $, đa tạp tuyến tính xạ ảnh là ảnh của $ W - \{0\} $ trong $ P(V) $ có thể được đồng nhất với không gian xạ ảnh $ P(W) $ dẫn xuất từ $ W $ và do đó ta có thể nói về chiều của một đa tạp như vậy. Trong một không gian xạ ảnh $ P(V) $, ảnh chính tắc của một siêu phẳng (bỏ gốc) của $ V $ là một đa tạp tuyến tính được gọi là *siêu phẳng xạ ảnh* (hoặc đơn giản là *siêu phẳng*); nếu $ P(V) $ hữu hạn chiều $ n $ thì các siêu phẳng trong $ P(V) $ là các đa tạp tuyến tính có chiều $ n - 1 $.

Mọi mệnh đề về các không gian con vectơ của một không gian vectơ đều chuyển sang một mệnh đề về các đa tạp tuyến tính xạ ảnh. Chẳng hạn, nếu một không gian xạ ảnh $ P(V) $ có số chiều hữu hạn $ n $ và $ (e_i)_{0 \leq i \leq n} $ là một cơ sở của $ V $, thì mọi đa tạp tuyến tính $ L \subset P(V) $ có chiều $ r $ đều có thể được xác định bởi một hệ gồm $ n - r $ phương trình tuyến tính thuần nhất

$$
\sum_{i=0}^{n} \xi_i \alpha_{ij} = 0 \qquad (1 \leq j \leq n - r)
$$

giữa các tọa độ thuần nhất $ \xi_i $ ($ 0 \leq i \leq n $) của một điểm của $ \mathbf{P}(V) $ đối với cơ sở $ (e_i) $, trong đó các vế trái của (4) là các dạng tuyến tính độc lập trên V. Đặc biệt, một siêu phẳng xạ ảnh được xác định bởi một phương trình tuyến tính thuần nhất duy nhất với các hệ số không phải đều bằng không. Ngược lại, các điểm của $ \mathbf{P}(V) $ thỏa mãn một hệ tùy ý các phương trình tuyến tính thuần nhất theo các $ \xi_i $ tạo thành một đa tạp tuyến tính L; nếu hệ xét đến gồm $ k \leq n + 1 $ phương trình, thì L có chiều $ \geq n - k $.

Mọi giao của các đa tạp tuyến tính của $ \mathbf{P}(V) $ đều là một đa tạp tuyến tính; với mọi tập con A của $ \mathbf{P}(V) $, tồn tại một đa tạp tuyến tính nhỏ nhất L chứa A; nó được gọi là đa tạp tuyến tính *sinh bởi* A và A được gọi là một *hệ sinh* của L.

Nếu W là không gian con vectơ của V được sinh bởi $ \pi^{-1}(A) $, thì $ L = \mathbf{P}(W) $.

Nếu L và M là bất kỳ hai đa tạp tuyến tính nào trong $ \mathbf{P}(V) $ và N là đa tạp được sinh bởi $ L \cup M $, thì (\$ 7, no. 3, Hệ quả 3 của Mệnh đề 4)

$$
\text{dim } L + \text{dim } M = \text{dim}(L \cap M) + \text{dim } N.
$$

Đặc biệt, nếu $ \mathbf{P}(V) $ hữu hạn chiều và $ \text{dim } L + \text{dim } M \geq \text{dim } \mathbf{P}(V) $, thì từ (5) suy ra $ L \cap M $ không rỗng.

Cho $ (x_i), (y_i) $ là hai họ điểm trong không gian vectơ V với cùng một tập chỉ số, sao cho $ y_i = \lambda_i x_i $, với $ \lambda_i \neq 0 $ đối với mọi $ i $. Nếu họ $ (x_i) $ là tự do, thì họ $ (y_i) $ cũng tự do, và ngược lại; khi đó nói rằng họ điểm $ \pi(x_i) $ của $ \mathbf{P}(V) $ là *tự do xạ ảnh* (hoặc đơn giản là *tự do*). Điều đó tương đương với việc nói rằng với mọi chỉ số $ \kappa $, điểm $ \pi(x_\kappa) $ không thuộc vào đa tạp tuyến tính do các $ \pi(x_i) $ với $ i \neq \kappa $ sinh ra. Một họ điểm của $ \mathbf{P}(V) $ không tự do xạ ảnh được gọi là *liên quan xạ ảnh* (hoặc đơn giản là *liên quan*).

Để một họ $ (x_i) $ các điểm của $ V - \{0\} $ sao cho họ $ (\pi(x_i)) $ là tự do xạ ảnh và sinh ra $ \mathbf{P}(V) $, thì điều kiện cần và đủ là $ (x_i) $ là một cơ sở của V. Nếu $ \mathbf{P}(V) $ có chiều $ n $ thì số phần tử trong một họ như vậy do đó là $ n + 1 $. Chú ý rằng việc cho một họ như vậy $ (\pi(x_i)) $ trong $ \mathbf{P}(V) $ không xác định (ngay cả đến một thừa số trái) các tọa độ thuần nhất của một điểm cho trước của $ \mathbf{P}(V) $ đối với một cơ sở $ (y_i) $ của V sao cho $ \pi(y_i) = \pi(x_i) $ với mọi $ i $ (xem no. 6).

### 8. PHÉP HOÀN THIỆN XẠ ẢNH CỦA MỘT KHÔNG GIAN AFFINE

Cho V là một không gian vectơ (trái) trên một trường K và xét không gian vectơ $ K_s \times V $ trên K; không gian xạ ảnh $ \mathbf{P}(K_s \times V) $ được gọi là không gian xạ ảnh *liên kết chính tắc* với không gian vectơ V. Nếu V có chiều $ n $, thì $ \mathbf{P}(K_s \times V) $ cũng có cùng chiều $ n $. Xét trong $ K_s \times V $ siêu phẳng affine $ V_1 = \{1\} \times V $, có phương (no. 3) là không gian con $ V_0 = \{0\} \times V $; nếu một đường thẳng (chuyển qua 0) của $ K_s \times V $ không được chứa trong $ V_0 $, thì nó chứa một điểm $ (\alpha, x) $ với $ \alpha \neq 0 $ và $ x \in V $, do đó nó cũng chứa điểm $ \alpha^{-1}(\alpha, x) = (1, \alpha^{-1}x) $ của $ V_1 $; điều ngược lại là hiển nhiên và thấy rằng có một tương ứng một-một giữa các điểm của $ V_1 $ và các đường thẳng (chuyển qua 0) của $ K_s \times V $ không được chứa trong $ V_0 $, mỗi đường thẳng sau cắt $ V_1 $ tại đúng một điểm. Suy ra rằng ánh xạ $ x \mapsto \phi(x) = \pi(1, x) $ là một đơn ánh (gọi là chính tắc) từ $ V $ vào không gian xạ ảnh $ P(K_s \times V) $; $ V $ thường được đồng nhất với ảnh của nó qua đơn ánh này. Phần bù của $ \phi(V) $ trong $ P(K_s \times V) $ là siêu phẳng xạ ảnh $ P(V_0) $ được gọi là siêu phẳng ở vô cực của $ P(K_s \times V) $ (hay của $ V $, theo lối nói quen); các điểm của nó cũng được gọi là "các điểm ở vô cực" của $ P(K_s \times V) $ (hay của $ V $). Nếu $ (a_i) $ là một cơ sở của $ V $ và trong $ K_s \times V $ lấy cơ sở gồm các phần tử $ e_i = (0, a_i) $ và phần tử $ e_\omega = (1, 0) $, thì các điểm ở vô cực trong $ P(K_s \times V) $ là những điểm có tọa độ thuần nhất chỉ số $ \omega $ bằng 0.

Cho $ M $ là một đa tạp tuyến tính afin trong $ V $ (no. 3) và $ D $ là phương của nó; ảnh chính tắc $ \phi(M) $ của $ M $ trong $ P(K_s \times V) $ được chứa trong ảnh chính tắc $ \overline{M} = \pi(M_2) $ của không gian con $ M_2 $ của $ K_s \times V $ sinh bởi đa tạp afin $ M_1 = \{1\} \times M $ của $ K_s \times V $. Chính xác hơn, nếu $ (a_i) $ là một hệ tự do afin của $ M $ sinh $ M $, thì các phần tử $ (1, a_i) $ lập thành một cơ sở của $ M_2 $ và do đó $ \overline{M} $ chỉ là đa tạp tuyến tính xạ ảnh sinh bởi $ \phi(M) $; nếu $ M $ hữu hạn chiều, thì $ \overline{M} $ có cùng chiều với $ M $. Phần bù của $ \phi(M) $ trong $ \overline{M} $ là giao của $ \overline{M} $ với siêu phẳng ở vô cực và bằng ảnh chính tắc $ \pi(M_0) $, trong đó $ M_0 = \{0\} \times D $.

Ngược lại, cho $ N $ là một đa tạp tuyến tính xạ ảnh không được chứa trong siêu phẳng ở vô cực và đặt $ R = \pi^{-1}(N) $; $ R \cap V_1 $ là một đa tạp tuyến tính afin của $ K \times V $ có dạng $ \{1\} \times M $, trong đó $ M $ là một đa tạp tuyến tính afin của $ V $ và ta thấy ngay rằng $ N $ là đa tạp tuyến tính afin $ \overline{M} $ sinh bởi $ \phi(M) $.

Vì vậy có một sự tương ứng một-một giữa các đa tạp tuyến tính afin của $ V $ và các đa tạp tuyến tính xạ ảnh của $ P(K_s \times V) $ không được chứa trong siêu phẳng ở vô cực; để hai đa tạp tuyến tính afin của $ V $ song song với nhau, điều cần và đủ là các đa tạp tuyến tính xạ ảnh do chúng sinh ra có cùng giao với siêu phẳng ở vô cực (điều này đôi khi được nói bằng cách rằng hai đa tạp tuyến tính afin nói trên có cùng các điểm ở vô cực).

### 9. MỞ RỘNG CÁC HÀM HỮU TỈ

Nếu áp dụng các kết quả của no. 8 cho không gian vectơ $ V = K_s $ có chiều 1, ta thấy tồn tại một đơn ánh chính tắc $ \phi $ từ $ K_s $ vào đường thẳng xạ ảnh $ P_1(K) = P(K_s \times K_s) $; với mọi $ \xi \in K $, $ \phi(\xi) $ là điểm có tọa độ thuần nhất $ (1, \xi) $ đối với cơ sở chính tắc (\$ 1, no. 11) của $ K_s \times K_s $. Phần bù của $ \phi(K) $ trong $ P_1(K) $ chỉ gồm một điểm duy nhất có tọa độ thuần nhất $ (0, 1) $ đối với cơ sở nói trên; nó được gọi là "điểm ở vô cực". $ P_1(K) $ cũng còn được gọi là trường xạ ảnh liên kết với $ K $ và được ký hiệu bởi $ \tilde{K} $, điểm ở vô cực trong $ \tilde{K} $ được ký hiệu bởi $ \infty $.

*Xét riêng trường hợp $ K $ là một trường giao hoán và cho f \in K(X) là một hàm hữu tỉ trên một ẩn với hệ số trong K (IV, § 4); nếu $ f \neq 0 $, ta có một biểu diễn duy nhất $ f = \alpha p/q $, trong đó $ \alpha \in K^* $ và $ p $ cùng $ q $ là hai đa thức đơn thức nguyên tố cùng nhau (VII, § 1); gọi $ m $ và $ n $ là các bậc tương ứng của chúng và đặt $ r = \sup(m, n) $. Ta viết
$$
p_1(T, X) = T^r p(X/T), \qquad q_1(T, X) = T^r q(X/T);
$$
$ p_1 $ và $ q_1 $ là hai đa thức thuần nhất bậc $ r $ trên $ K $ sao cho $ p(X) = p_1(1, X) $, $ q(X) = q_1(1, X) $. Do đó, với mọi phần tử $ \xi \in K $ không là một nghiệm của $ q(X) $, $ f(\xi) = \alpha p(\xi)/q(\xi) $ được xác định và ta có thể viết
$$
f(\xi) = \alpha p_1(1, \xi)/q_1(1, \xi) = \alpha p_1(\lambda, \lambda \xi)/q_1(\lambda, \lambda \xi)
$$
với mọi $ \lambda \neq 0 $ trong $ K $. Khi đó xét ánh xạ
$$
(\eta, \xi) \mapsto (q_1(\eta, \xi), p_1(\eta, \xi))
$$
từ $ K^2 $ vào chính nó; nó tương thích với quan hệ tương đương $ \Delta(K^2) $ và vì thế xác định, khi chuyển sang các thương, một ánh xạ $ \tilde{f} $ của $ \tilde{K} $ vào chính nó, trùng với $ \xi \mapsto f(\xi) $ tại các điểm mà hàm hữu tỉ này được xác định; người ta nói, theo lối nói lạm dụng, rằng $ \tilde{f} $ là mở rộng chính tắc của $ f $ lên $ \tilde{K} $.

Chẳng hạn, nếu $ f = 1/X $, thì $ \tilde{f}(0) = \infty $ và $ \tilde{f}(\infty) = 0 $; nếu
$$
f = (aX + b)/(cX + d)
$$
với $ ad - bc \neq 0 $, thì $ \tilde{f}(-d/c) = \infty $, $ \tilde{f}(\infty) = a/c $ nếu $ c \neq 0 $, $ \tilde{f}(\infty) = \infty $ nếu $ c = 0 $. Nếu $ f = a_0 X^n + \cdots + a_n $ là một đa thức bậc $ n > 0 $, thì $ \tilde{f}(\infty) = \infty $*

### 10. CÁC ÁNH XẠ TUYẾN TÍNH XẠ ẢNH

Cho $ V, V' $ là hai không gian vectơ trái trên một trường $ K $, $ f $ là một ánh xạ tuyến tính của $ V $ vào $ V' $ và $ N = \overline{f}(0) $ là hạt nhân của nó. Hiển nhiên rằng ảnh của một đường thẳng (đi qua $0$) trong $ V $ không được chứa trong $ N $ qua $ f $ là một đường thẳng (đi qua $0$) trong $ V' $; do đó, khi đi sang các thương, $ f $ xác định một ánh xạ $ g $ của $ P(V) - P(N) $ vào $ P(V') $. Một ánh xạ như vậy được gọi là một ánh xạ xạ ảnh tuyến tính (hay, nói ngắn gọn, một ánh xạ xạ ảnh); mặc dù nó được xác định trên $ P(V) - P(N) $ chứ không phải trên $ P(V) $ (khi $ N \neq \{0\} $), ta sẽ nói một cách lạm dụng ngôn ngữ rằng $ g $ là một ánh xạ xạ ảnh của $ P(V) $ vào $ P(V') $. Đa tạp xạ ảnh tuyến tính $ P(N) $, nơi $ g $ không được xác định, được gọi là tâm của $ g $.

Chú ý rằng, khi $ g $ được xác định trên toàn bộ $ P(V) $ (tức là khi $ N = \{0\} $), $ g $ là một đơn ánh của $ P(V) $ vào $ P(V') $.

Khi các cơ sở $ (a_\lambda)_{\lambda \in L}, (b_\mu)_{\mu \in M} $ được cho trong $ V $ và $ V' $ tương ứng, một ánh xạ xạ ảnh của $ P(V) $ vào $ P(V') $ gửi một điểm của $ P(V) $ có các tọa độ thuần nhất $ \xi_\lambda $ ($ \lambda \in L $) tới một điểm của $ \mathbf{P}(V') $ có một hệ tọa độ thuần nhất $ \eta_\mu $ ($ \mu \in M $) có dạng

$$
\eta_\mu = \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} \quad (\alpha_{\lambda \mu} \in K).
$$

Tâm của $ g $ là đa tạp tuyến tính được xác định bởi các phương trình

$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} = 0 \quad (\mu \in M).
$$

Nếu $ C $ là tâm của $ g $ và $ M $ là một đa tạp tuyến tính của $ \mathbf{P}(V) $, thì ảnh của $ M - (M \cap C) $ qua $ g $ là một đa tạp tuyến tính của $ \mathbf{P}(V') $ được ký hiệu (một cách lạm dụng ngôn ngữ) bởi $ g(M) $. Khi đó

$$
\dim g(M) + \dim(M \cap C) + 1 = \dim M
$$

(\S 7, no. 4, công thức (12)). Nếu $ M' $ là một đa tạp tuyến tính của $ \mathbf{P}(V') $, $ g^{-1}(M') \cup C $ là một đa tạp tuyến tính của $ \mathbf{P}(V) $ và

$$
\dim(g^{-1}(M') \cup C) = \dim C + \dim(M' \cap g(\mathbf{P}(V))) + 1.
$$

Người ta nói, một cách lạm dụng ngôn ngữ, rằng $ g^{-1}(M') \cup C $ là *ảnh ngược* của $ M' $ qua $ g $.

As the values taken by a linear mapping on a basis $ (e_i) $ of $ V $ can be chosen arbitrarily in $ V' $, it is seen that there exists a projective linear mapping of $ \mathbf{P}(V) $ into $ \mathbf{P}(V') $ taking *các giá trị tùy ý* at the points $ \pi(e_i) $. But (even when $ g $ is everywhere defined) giving $ g(\pi(e_i)) $ does not determine $ g $ uniquely (Bài tập 10).

The composition of two projective mappings which are bijections is a projective mapping; so is the inverse mapping of such a bijection. The bijective projective mappings of a projective space $ \mathbf{P}(V) $ onto itself thus form a group, called the *nhóm xạ ảnh* of $ \mathbf{P}(V) $ and denoted by $ \mathbf{PGL}(V) $; we write $ \mathbf{PGL}_n(K) $ or $ \mathbf{PGL}(n, K) $ instead of $ \mathbf{PGL}(K^n_s) $.

#### Nhận xét {#alg-ii-s9-n10-rem-1 .statement}

In a projective space $ \mathbf{P}(V) $ over a field $ K $, let $ H = \mathbf{P}(W) $ be a hyperplane. There exists a bijective linear mapping $ f $ of $ V $ onto $ K_s \times W $ such that $ f(W) = W $; let $ g $ be the projective mapping obtained from $ f $ by passing to the quotients. It has been seen (no. 8) that the complement of $ \mathbf{P}(W) $ in $ \mathbf{P}(K_s \times W) $ can be identified with an affine space whose translation space is $ W $. When $ \mathbf{P}(V) $ is identified with $ \mathbf{P}(K_s \times W) $ by means of $ g $, it is said that $ H $ *đã được lấy làm siêu phẳng ở vô cực* in $ \mathbf{P}(V) $; the complement of $ H $ in $ \mathbf{P}(V) $ is then identified with an affine space whose translation space is $ W $.

### 11. CẤU TRÚC KHÔNG GIAN XẠ ẢNH

Given a set E and a field K, a (left) projective space structure on E with respect to the field K is defined by giving a non-empty set $ \Phi $ of bijections of subsets of the projective space $ \mathbf{P}(K_s^{(E)}) $ onto E satisfying the following axioms:

$$(\mathrm{EP}_I)$$ *Tập xác định của mọi ánh xạ $ f \in \Phi $ là một đa tạp tuyến tính của $ \mathbf{P}(K_s^{(E)}) $.*

$$(\mathrm{EP}_{II})$$ *Với mọi cặp có thứ tự các phần tử $ f, g $ của $ \Phi $ được xác định tương ứng trên các đa tạp tuyến tính $ \mathbf{P}(V) $ và $ \mathbf{P}(W) $, song ánh $ h = g^{-1} \circ f $ của $ \mathbf{P}(V) $ lên $ \mathbf{P}(W) $ là một ánh xạ xạ ảnh.*

$$(\mathrm{EP}_{III})$$ *Ngược lại, nếu $ f \in \Phi $ được xác định trên đa tạp tuyến tính $ \mathbf{P}(V) $ và $ h $ là một ánh xạ xạ ảnh song ánh của $ \mathbf{P}(V) $ lên một đa tạp tuyến tính $ \mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)}) $, thì $ f \circ h^{-1} \in \Phi $.*

Cho E là một tập hợp, $ (V_\lambda)_{\lambda \in L} $ là một họ các không gian vectơ trên K và giả sử, với mỗi $ \lambda \in L $, cho trước một song ánh $ f_\lambda $ từ $ \mathbf{P}(V_\lambda) $ lên E sao cho, với mọi cặp có thứ tự của các chỉ số $ \lambda, \mu $, $ f_\lambda^{-1} \circ f_\mu $ là một *ánh xạ xạ ảnh* từ $ \mathbf{P}(V_\mu) $ lên $ \mathbf{P}(V_\lambda) $. Khi đó ta có thể định nghĩa trên E một cấu trúc không gian xạ ảnh đối với K như sau: cho $ (e_i)_{i \in I} $ là một cơ sở của một không gian $ V_\lambda $ và viết $ a_i = f_\lambda(\pi(e_i)) $; cho $ b_i $ là phần tử có chỉ số $ a_i $ trong cơ sở chính tắc của $ K_s^{(E)} $ (\S 1, no. 11). Quan hệ $ i \neq \kappa $ kéo theo $ b_i \neq b_\kappa $ vì giả thiết rằng $ f_\lambda $ là song ánh; do đó các $ b_i $ lập thành một cơ sở của một không gian con vectơ $ W_0 $ của $ K_s^{(E)} $ và vì vậy tồn tại một ánh xạ xạ ảnh song ánh $ h $ từ $ \mathbf{P}(W_0) $ lên $ \mathbf{P}(V_\lambda) $ sao cho $ h(\pi(b_i)) = \pi(e_i) $ với mọi $ i \in I $. Nếu lấy $ \Phi $ là tập hợp tất cả các ánh xạ xạ ảnh song ánh $ f_\lambda \circ h \circ g^{-1} $, trong đó $ g $ chạy qua tập hợp tất cả các ánh xạ xạ ảnh song ánh $ \mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)}) $, thì ngay lập tức kiểm tra được rằng $ \Phi $ thỏa các tiên đề (EP_I), (EP_{II}) và (EP_{III}). Hơn nữa, ngay lập tức thấy rằng $ \Phi $ không phụ thuộc vào việc chọn chỉ số $ \lambda \in L $, cũng không phụ thuộc vào việc chọn cơ sở $ (e_i) $ trong $ V_\lambda $, cũng không phụ thuộc vào việc chọn $ h $.

Đặc biệt (lấy L chỉ gồm một phần tử), mọi không gian xạ ảnh $ \mathbf{P}(V) $ dẫn xuất từ một không gian vectơ V (no. 5, Định nghĩa 4) như vậy đều có một "cấu trúc không gian xạ ảnh" được xác định rõ theo nghĩa của định nghĩa đã cho trong số này. Do đó, mọi tập hợp có cấu trúc không gian xạ ảnh có thể được gọi là một *không gian xạ ảnh*.

Với cùng ký hiệu, một *đa tạp tuyến tính* trong một không gian xạ ảnh E là một tập con M của E sao cho, với ít nhất *một* song ánh $ f \in \Phi $ xác định trên $ \mathbf{P}(V) \subset \mathbf{P}(K_s^{(E)}) $, $ f^{-1}(M) $ là một đa tạp tuyến tính trong $ \mathbf{P}(V) $ theo nghĩa của no. 7 (khi đó tính chất này đúng với *mọi* $ f \in \Phi $). Từ điều trên suy ra rằng mọi đa tạp tuyến tính trong một không gian xạ ảnh đều có một cách chính tắc cấu trúc không gian xạ ảnh.

Một không gian xạ ảnh E được gọi là *có chiều n* nếu, với mọi $ f \in \Phi $, $ f^{-1}(E) $ là một đa tạp tuyến tính có chiều n (chỉ cần điều này đúng với *một* ánh xạ $ f \in \Phi $).

### Bài tập {#alg-ii-s9-exercises}

Xem [các bài tập cho § 9](exercises/s9/).
