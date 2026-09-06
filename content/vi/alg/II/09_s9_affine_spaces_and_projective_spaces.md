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
book_pages: 325-337, 410-417
pdf_pages: 0349-0361, 0434-0441
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AFFINE SPACES
      page: 325
      pdf_page: 349
    - "no": 2
      title: BARYCENTRIC CALCULUS
      page: 326
      pdf_page: 350
    - "no": 3
      title: AFFINE LINEAR VARIETIES
      page: 327
      pdf_page: 351
    - "no": 4
      title: AFFINE LINEAR MAPPINGS
      page: 329
      pdf_page: 353
    - "no": 5
      title: DEFINITION OF PROJECTIVE SPACES
      page: 331
      pdf_page: 355
    - "no": 6
      title: HOMOGENEOUS COORDINATES
      page: 331
      pdf_page: 355
    - "no": 7
      title: PROJECTIVE LINEAR VARIETIES
      page: 332
      pdf_page: 356
    - "no": 8
      title: PROJECTIVE COMPLETION OF AN AFFINE SPACE
      page: 333
      pdf_page: 357
    - "no": 9
      title: EXTENSION OF RATIONAL FUNCTIONS
      page: 334
      pdf_page: 358
    - "no": 10
      title: PROJECTIVE LINEAR MAPPINGS
      page: 335
      pdf_page: 359
    - "no": 11
      title: PROJECTIVE SPACE STRUCTURE
      page: 337
      pdf_page: 361
statements: 12
exercises: 6
content_sha256: 4a5fba84198ededc1f6e56ee7ac90c955c414c2b5f6a5681e0134d31193f0a53
translated_from: content/en/alg/II/09_s9_affine_spaces_and_projective_spaces.md
source_content_sha256: 6d5414948dceab419cbfb016f0d02a94213bdb1f5a7f8c8b4975a8a4bd8908c9
translation_model: gpt-5.4
translation_run: translate-vi-57309ea3
glossary_version: 34
glossary_terms_sha256: 8525c8eb162f10d53ba5038655ac122c3844e7ca7a4f34c0f9dad833e8daeb46
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. KHÔNG GIAN AFIN VÀ KHÔNG GIAN XẠ ẢNH

### 1. ĐỊNH NGHĨA KHÔNG GIAN AFIN

#### Định nghĩa 1 {#alg-ii-s9-def-1 .statement}

*Cho một không gian vectơ trái (tương ứng phải) T trên một trường K, một không gian afin gắn với T là mọi không gian thuần nhất E của nhóm cộng T* (I, § 5, no. 5) *sao cho 0 là toán tử duy nhất trong T để bất biến mọi phần tử của E* (nghĩa là, T *tác động trung thành và bắc cầu trên E*). *Trong các điều kiện đó, T được gọi là không gian tịnh tiến của E và các phần tử của nó được gọi là các phép tịnh tiến của E* (hoặc *các vectơ tự do của E*).

Trong phần sau, chúng tôi sẽ chỉ giới hạn sự chú ý vào trường hợp T là một không gian vectơ trái trên K. Chiều (trên K) của không gian vectơ tịnh tiến T của một không gian afin E được gọi là *chiều* của E (trên K) và được ký hiệu là dim E hoặc $\dim_K E$. Một không gian afin chiều một (tương ứng hai) được gọi là một *đường thẳng afin* (tương ứng một *mặt phẳng afin*). Các phần tử của một không gian afin cũng được gọi là *điểm*.

Trong các điều kiện của Định nghĩa 1, với $t \in T$ và $a \in E$ chúng tôi sẽ ký hiệu bởi $t + a$ hoặc $a + t$ biến đổi của điểm a dưới t. Khi đó các hệ thức

$$
s + (t + a) = (s + t) + a, \quad 0 + a = a
$$

đúng với $s \in T, t \in T, a \in E$. Ánh xạ $x \mapsto x + t$ là một song ánh của E lên chính nó, mà ta đồng nhất với t. Định nghĩa 1 hơn nữa kéo theo rằng, với mọi $a \in E$, ánh xạ $t \mapsto t + a$ là một *song ánh* từ T lên E. Nói cách khác, cho hai điểm $a, b$ của E, tồn tại một và chỉ một phép tịnh tiến t sao cho $b = t + a$; chúng tôi sẽ ký hiệu phép tịnh tiến này bởi $b - a$; khi đó các công thức

$$
a - a = 0, \quad a - b = -(b - a), \quad b = (b - a) + a
$$
$$
(c - b) + (b - a) = c - a
$$

đúng với $a \in E, b \in E, c \in E$. Nếu bốn điểm $a, b, a', b'$ của E sao cho $b - a = b' - a'$, thì công thức

$$
b' = (b' - b) + (b - a) + a = (b' - a') + (a' - a) + a
$$

và tính giao hoán của phép cộng trong T cho thấy rằng $b' - b = a' - a$.

Cho một điểm $a \in E$, ánh xạ $x \mapsto x - a$ là một song ánh từ $E$ lên $T$; khi E được đồng nhất với $T$ qua ánh xạ này, ta nói rằng E được xét như không gian vectơ thu được *bằng cách lấy $a$ làm gốc* trong E. Ngược lại, mọi không gian vectơ $T$ đều có một cách chính tắc cấu trúc của một không gian afin gắn với $T$, cụ thể là cấu trúc không gian thuần nhất tương ứng với nhóm con $\{0\}$ của $T$ (I, § 5, no. 6).

#### Nhận xét {#alg-ii-s9-n1-rem-1 .statement}

Các định nghĩa của số này và một số kết quả tiếp theo được mở rộng ngay lập tức cho trường hợp trong đó, thay vì một không gian vectơ $T$, ta xét một *nhóm giao hoán có toán tử* tùy ý $T$.

### 2. PHÉP TÍNH TRỌNG TÂM

#### Mệnh đề 1 {#alg-ii-s9-prop-1 .statement}

*Cho* $(x_i)_{i \in I}$ *là một họ các điểm trong một không gian afin* $E$ *và* $(\lambda_i)_{i \in L}$ *là một họ các phần tử của* $K$ *có giá hữu hạn sao cho* $\sum_{i \in I} \lambda_i = 1$ *(*tương ứng $\sum_{i \in I} \lambda_i = 0$*). *Nếu* $a$ *là một điểm tùy ý của* $E$, *thì điểm* $x \in E$ *được xác định bởi*
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*(tương ứng vectơ tự do* $\sum_{i \in I} \lambda_i (x_i - a)$) *là độc lập với điểm được xét.*

Nếu $a'$ là một điểm khác của $E$, thì
$$
\sum_i \lambda_i (x_i - a') = \sum_i \lambda_i ((x_i - a) + (a - a')) = \sum_i \lambda_i (x - a) + \left( \sum_i \lambda_i \right) (a - a').
$$
Nếu $\sum_i \lambda_i = 1$, thì $\sum_i \lambda_i (x_i - a) = (x - a) + (a - a') = x - a'$; nếu $\sum_i \lambda_i = 0$, thì $\sum_i \lambda_i (x - a') = \sum_i \lambda_i (x - a)$; do đó có mệnh đề.

Trong các điều kiện của Mệnh đề 1, điểm $x$ được xác định bởi
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*(tương ứng vectơ tự do* $\sum_{i \in I} \lambda_i (x_i - a)$) *được ký hiệu bởi* $\sum_{i \in I} \lambda_i x_i$.

Do đó, đặc biệt, ký hiệu $b - a$ được đưa vào ở no. 1 được phục hồi. Khi $\sum_i \lambda_i = 1$, điểm $x = \sum_i \lambda_i x_i$ được gọi là *trọng tâm của các điểm* $x_i$ *ứng với các khối lượng* $\lambda_i$.

Cho $m$ điểm $a_1, \ldots, a_m$ của $E$, mà số của chúng $m$ không là bội của đặc số của $K$ (V, § 1), điểm $g = \sum_{i=1}^m \frac{1}{m} a_i$ được gọi (theo một sự lạm dụng

ngôn ngữ) là *trọng tâm của các điểm* $a_i$ ($1 \leq i \leq m$) (với $m = 2$, ta nói "trung điểm" thay cho "trọng tâm"); nó được đặc trưng bởi quan hệ
$$
\sum_{i=1}^m (a_i - g) = 0.
$$

### 3. ĐA TẠP TUYẾN TÍNH AFIN

#### Định nghĩa 2 {#alg-ii-s9-def-2 .statement}

*Cho một không gian afin* $E$, *một tập con* $V$ *của* $E$ *được gọi là một đa tạp tuyến tính afin* (hay đơn giản là một *đa tạp tuyến tính* hoặc một *tập con afin* của $E$) *nếu, với mọi họ* $(x_i)_{i \in I}$ *các điểm của* $V$ *và mọi họ* $(\lambda_i)_{i \in I}$ *các phần tử của* $K$ *có giá hữu hạn sao cho* $\sum_{i \in I} \lambda_i = 1$, *trọng tâm* $\sum_{i \in I} \lambda_i x_i$ *thuộc* $V$.

Điều đó cũng tương đương với việc nói rằng điều kiện của Định nghĩa 2 được thỏa mãn với mọi họ *hữu hạn* các điểm của $V$.

Tập rỗng là một đa tạp tuyến tính; mọi giao của các đa tạp tuyến tính là một đa tạp tuyến tính.

Cho $V$ là một tập con khác rỗng của $E$ và $a$ là một điểm của $V$; quan hệ
$$
x - a = \sum_{i=1}^n \lambda_i (x_i - a)
$$
có nghĩa là $x$ là một trọng tâm $\sum_{i=1}^n \lambda_i x_i + \left(1 - \sum_{i=1}^n \lambda_i\right)a$ của họ gồm các $x_i$ và $a$. Do đó:

#### Mệnh đề 2 {#alg-ii-s9-prop-2 .statement}

*Để một tập con khác rỗng* $V$ *của một không gian afin* $E$ *là một đa tạp tuyến tính, điều kiện cần và đủ là* $V$ *là một không gian con vectơ đối với cấu trúc không gian vectơ trên* $E$ *nhận được bằng cách lấy một điểm của* $V$ *làm gốc.*

Đặc biệt, các đa tạp tuyến tính afin khác rỗng của một không gian vectơ $T$ (được xét như một không gian afin) chính là các *bản dịch* của các không gian con vectơ của $T$; do đó các không gian con vectơ của $T$ là các đa tạp tuyến tính chứa 0.

Cho $V$ là một đa tạp tuyến tính khác rỗng của không gian afin $E$; tập hợp các vectơ tự do $x - y$, trong đó $x$ và $y$ chạy qua $V$, là một không gian con vectơ $D$ của không gian tịnh tiến $T$ của $E$ được gọi là *phương* của $V$: thật vậy, nếu $a \in V$, thì
$$
x - y = (x - a) - (y - a)
$$
và mệnh đề của chúng ta suy ra từ Mệnh đề 2. Hiển nhiên là $D$ tác động một cách trung thành và bắc cầu trên $V$, do đó $V$ có một cách chính tắc cấu trúc của một *không gian afin gắn với* $D$. *Chiều* của đa tạp afin $V$ được hiểu là chiều của $V$ với cấu trúc không gian afin này, tức là chiều của không gian vectơ $D$. Các đa tạp tuyến tính có chiều 0 là các điểm của $E$; các đa tạp có chiều 1 (resp. 2) được gọi là các *đường thẳng* (resp. *mặt phẳng*) của $E$.

Mọi vectơ $\neq 0$ thuộc phương của một đường thẳng được gọi là một *vectơ chỉ phương* của đường thẳng này; các thành phần của nó đối với một cơ sở của T tạo thành cái được gọi là một hệ *tham số chỉ phương* của đường thẳng đang xét.

*Đối chiều* của một đa tạp tuyến tính V trong E là đối chiều của phương $D$ của nó trong T; một đa tạp tuyến tính có đối chiều 1 trong E được gọi là một *siêu phẳng* (afin) của E.

Hai đa tạp tuyến tính có cùng phương được gọi là *song song*; điều đó tương đương với việc nói rằng một đa tạp được dẫn xuất từ đa tạp kia bằng phép tịnh tiến. Nếu V là một đa tạp tuyến tính trong T (được xét như một không gian afin), thì phương của nó là đa tạp tuyến tính song song với V và chứa 0.

#### Mệnh đề 3 {#alg-ii-s9-prop-3 .statement}

*Cho một họ* $(a_i)_{i \in I}$ *các điểm của một không gian afin* E, *tập hợp* V *các trọng tâm* $\sum_{i \in I} \lambda_i a_i$ *((\lambda_i) có giá hữu hạn, $\sum_{i \in I} \lambda_i = 1$) *là một đa tạp tuyến tính của* E.

Nếu họ $(a_i)$ rỗng, thì $V = \varnothing$ do điều kiện $\sum_i \lambda_i = 1$. Vì vậy có thể giả thiết họ $(a_i)$ là khác rỗng và trong trường hợp này mệnh đề là hiển nhiên, bằng cách lấy một trong các $a_i$ làm gốc trong E.

Hiển nhiên đa tạp V là đa tạp tuyến tính nhỏ nhất chứa các $a_i$; người ta nói rằng nó được *sinh* bởi họ $(a_i)$ và họ này được gọi là một *hệ sinh* của V.

Theo ký hiệu của Mệnh đề 3, giả sử họ $(a_i)$ là khác rỗng, để biểu thức của mọi điểm $x \in V$ dưới dạng $x = \sum_i \lambda_i a_i$ là *duy nhất*, điều kiện cần và đủ là, ký hiệu $\kappa$ là một chỉ số tùy ý của I, họ các vectơ $a_i - a_\kappa$, trong đó $i$ chạy qua tập hợp các chỉ số $\neq \kappa$, là tự do trong T. Khi đó người ta nói rằng họ các điểm $(a_v)_{v \in I}$ của E là *tự do afin* (hoặc các phần tử của nó tạo thành một *hệ tự do afin*, hoặc là *độc lập afin*) và rằng $\lambda_i$ là *tọa độ trọng tâm* của $x$ có chỉ số $i$ đối với họ tự do afin $(a_i)$.

Một họ $(a_i)_{i \in I}$ các điểm của E không tự do afin được gọi là *liên hệ afin*.

#### Mệnh đề 4 {#alg-ii-s9-prop-4 .statement}

*Để một họ khác rỗng* $(a_i)_{i \in I}$ *các điểm trong một không gian afin* E *là liên hệ afin, điều kiện cần và đủ là tồn tại một họ* $(\lambda_i)_{i \in I}$ *các phần tử không đồng thời bằng không trong* K, *có giá hữu hạn, sao cho* $\sum_{i \in I} \lambda_i = 0$ *và* $\sum_{i \in I} \lambda_i a_i = 0$.

Cho một chỉ số $\kappa \in I$, nói rằng họ các vectơ $(a_i - a_\kappa)$, trong đó $i$ chạy qua tập hợp các chỉ số $\neq \kappa$, là liên hệ trong T, có nghĩa là tồn tại một họ các vô hướng $(\lambda_i)_{i \neq \kappa}$ không đồng thời bằng không sao cho $\sum_{i \neq \kappa} \lambda_i (a_i - a_\kappa) = 0$, điều này cũng có thể viết là $\sum_{i \in I} \lambda_i a_i = 0$, với $\lambda_\kappa = -\sum_{i \neq \kappa} \lambda_i$, nói cách khác $\sum_{i \in I} \lambda_i = 0$.

#### Mệnh đề 5 {#alg-ii-s9-prop-5 .statement}

Để một họ không rỗng $(a_i)_{i \in I}$ các điểm của một không gian afin $E$ là afin tự do, điều kiện cần và đủ là, với mọi chỉ số $\kappa \in I$, $a_\kappa$ không thuộc đa tạp tuyến tính sinh bởi các $a_i$ có chỉ số $\neq \kappa$.

Mệnh đề là hiển nhiên nếu $I$ chỉ có một phần tử. Nếu không, lấy làm gốc trong $E$ một trong các $a_i$ có chỉ số $\neq \kappa$, mệnh đề suy ra từ § 7, no. 1, Nhận xét.

### 4. ÁNH XẠ TUYẾN TÍNH AFIN

#### Định nghĩa 3 {#alg-ii-s9-def-3 .statement}

Cho hai không gian afin $E, E'$ gắn với hai không gian vectơ $T, T'$ trên cùng trường $K$, một ánh xạ $u$ từ $E$ vào $E'$ được gọi là một ánh xạ tuyến tính afin (hay một ánh xạ afin) nếu, với mọi họ $(x_i)_{i \in I}$ các điểm của $E$ và mọi họ $(\lambda_i)_{i \in I}$ sao cho $\sum_{i \in I} \lambda_i = 1$,

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i).
$$

(3)

#### Mệnh đề 6 {#alg-ii-s9-prop-6 .statement}

Cho $u$ là một ánh xạ afin từ $E$ vào $E'$. Tồn tại một và chỉ một ánh xạ tuyến tính $v$ từ $T$ vào $T'$ sao cho

$$
u(x + t) = u(x) + v(t)
$$

với mọi $x \in E, t \in T$.

Cho $a$ là một điểm tùy ý của $E$. Ánh xạ

$$
t \mapsto u(a + t) - u(a)
$$

là một ánh xạ tuyến tính $v_a$ từ $T$ vào $T'$, vì ta có thể viết

$$
a + \lambda t = \lambda (a + t) + (1 - \lambda)a \\
a + s + t = (a + s) + (a + t) - a
$$

và suy ra từ (3) rằng $v_a(\lambda t) = \lambda v_a(t)$ và $v_a(s + t) = v_a(s) + v_a(t)$. Hơn nữa, nếu $b$ là một điểm khác của $E$, thì $v_a = v_b$; thật vậy, quan hệ

$$
(a + t) - a + b = b + t
$$

kéo theo

$$
u(a + t) - u(a) + u(b) = u(b + t)
$$

tức là $u(a + t) - u(a) = u(b + t) - u(b)$. Do đó có sự tồn tại của $v$; tính duy nhất là ngay lập tức.

$v$ được gọi là ánh xạ tuyến tính từ $T$ vào $T'$ liên kết với $u$. Ngược lại, với mọi ánh xạ tuyến tính $v$ từ $T$ vào $T'$ và mọi cặp có thứ tự các điểm $a \in E, a' \in E'$, ta kiểm tra ngay lập tức được rằng

$$
x \mapsto a' + v(x - a)
$$

là một ánh xạ afin từ E vào E' mà ánh xạ tuyến tính liên kết là v. Vì vậy, nói rằng u là một ánh xạ afin từ E vào E' còn có nghĩa là, nếu lấy một điểm tùy ý a trong E và điểm u(a) trong E' làm gốc, thì u là một ánh xạ tuyến tính đối với hai không gian vectơ nhận được như vậy.

Cho E'' là một không gian afin thứ ba, T'' là không gian tịnh tiến của nó, u' là một ánh xạ afin từ E' vào E'' và v' là ánh xạ tuyến tính từ T' vào T'' liên kết với u'. Rõ ràng u' o u là một ánh xạ afin từ E vào E''; hơn nữa, với a \in E và t \in T,
$$
u'(u(a + t)) = u'(u(a) + v(t)) = u'(u(a)) + v'(v(t))
$$
và do đó v' o v là ánh xạ tuyến tính từ T vào T'' liên kết với u' o u. Để một ánh xạ afin u là song ánh, điều kiện cần và đủ là ánh xạ tuyến tính liên kết v cũng vậy, và khi đó u^{-1} là một ánh xạ afin mà ánh xạ tuyến tính liên kết là v^{-1}.

Đặc biệt, các song ánh afin của E lên chính nó tạo thành một nhóm G, gọi là nhóm afin của E. Ánh xạ gán cho mỗi u \in G ánh xạ tuyến tính v liên kết với u, theo điều trên, là một đồng cấu từ G lên nhóm tuyến tính \mathbf{GL}(T). Nếu u là một phép tịnh tiến thì v là đồng nhất và ngược lại. Do đó, hạt nhân của đồng cấu trên là nhóm tịnh tiến T của E, vì thế là một nhóm con chuẩn tắc của G.

Nếu u \in G, tự đẳng cấu t \mapsto utu^{-1} của T (trong đó t được đồng nhất với phép tịnh tiến x \mapsto x + t) là ánh xạ tuyến tính v liên kết với u. Với x \in E và t \in T, theo định nghĩa
$$
x + utu^{-1} = u(u^{-1}(x) + t) = u(u^{-1}(x)) + v(t) = x + v(t)
$$
và do đó utu^{-1} = v(t).

Cho a \in E và G_a là nhóm con của G gồm các u \in G sao cho u(a) = a. Nếu đồng nhất E với T bằng cách lấy a làm gốc, thì G_a được đồng nhất với \mathbf{GL}(T). Mọi u \in G đều có thể biểu diễn duy nhất dưới dạng u = t_1u_1 (tương ứng dưới dạng u = u_2t_2), trong đó u_1, u_2 thuộc G_a và t_1, t_2 thuộc T: thật vậy, đặt t_1 = u(a) - a, thì u^{-1}t_1 \in G_a, do đó có sự tồn tại của u_1 và t_1; sự tồn tại của u_2 và t_2 thu được tương tự. Tính duy nhất suy ra từ việc G_a \cap T quy về phần tử đơn vị của G. Hơn nữa
$$
t_1u_1 = u_1(u_1^{-1}t_1u_1)
$$
do đó u_2 = u_1, t_2 = u_1^{-1}t_1u_1. Cuối cùng, các ánh xạ tuyến tính liên kết với u và u_1 là như nhau và do đó, nếu như trên G_a được đồng nhất với \mathbf{GL}(T), thì u_1 là ánh xạ tuyến tính từ T vào chính nó liên kết với u. Như vậy thấy rằng G là tích nửa trực tiếp của G_a bởi T (I, § 6, no. 1).

Cho $E, E'$ là hai không gian afin trên $K$. Ảnh trực tiếp (tương ứng, ảnh nghịch) của một đa tạp tuyến tính của $E$ (tương ứng, $E'$) dưới một ánh xạ afin $u$ từ $E$ vào $E'$ là một đa tạp tuyến tính của $E'$ (tương ứng, $E$); hạng của $u$ theo định nghĩa là chiều của $u(E)$; nó bằng hạng của ánh xạ tuyến tính liên kết với $u$. Nếu $V, V'$ là các đa tạp tuyến tính có cùng số chiều hữu hạn $m$ trong $E, E'$ tương ứng, thì tồn tại một ánh xạ afin $u$ từ $E$ vào $E'$ sao cho $u(V) = V'$: lấy làm gốc trong $E$ và $E'$ các điểm của $V$ và $V'$ tương ứng, rồi lấy trong $E$ (tương ứng, $E'$) một cơ sở mà $m$ vectơ đầu tiên tạo thành một cơ sở của $V$ (tương ứng, $V'$), thì mệnh đề suy ra ngay lập tức từ § 1, no. 11, Hệ quả 3 của Mệnh đề 17.

Vì trường $K$ một cách chính tắc có một cấu trúc không gian vectơ trái (chiều bằng 1) trên $K$, nên nó có thể được xem như một không gian afin chiều 1. Một ánh xạ afin từ một không gian afin $D$ (trên $K$) vào không gian afin $K$ cũng được gọi là một *hàm afin tuyến tính* (hoặc một *hàm afin*). Nếu lấy một điểm $a$ làm gốc trong $E$, thì mọi hàm afin trên $E$ khi đó có thể được viết duy nhất dưới dạng $x \mapsto \alpha + v(x)$, trong đó $\alpha \in K$ và $v$ là một dạng tuyến tính trên không gian vectơ $E$ thu được như vậy; do đó các hàm afin trên $E$ tạo thành một *không gian vectơ phải trên* $K$ có chiều $1 + \dim E$. Nếu $u$ là một hàm afin không hằng trên $E$ và $\lambda \in K$, thì tập hợp các $x \in E$ thỏa mãn phương trình $u(x) = \lambda$ là một siêu phẳng; ngược lại, với mọi siêu phẳng $H$ trong $E$, tồn tại một hàm afin $u_0$ trên $E$ sao cho $H = u_0^{-1}(0)$ và mọi hàm afin $u$ sao cho $H = u^{-1}(0)$ đều có dạng $u_0 \mu$, trong đó $\mu \in K$ (§ 7, no. 5, Mệnh đề 11). Nếu $u$ là một hàm afin trên $E$, thì các siêu phẳng có phương trình $u(x) = \alpha$ và $u(x) = \beta$ là song song.

### 5. ĐỊNH NGHĨA CỦA CÁC KHÔNG GIAN XẠ ẢNH

#### Định nghĩa 4 {#alg-ii-s9-def-4 .statement}

*Cho một không gian vectơ trái (resp. phải)* $V$ *trên một trường* $K$, *không gian xạ ảnh trái (resp. phải) dẫn xuất từ* $V$, *ký hiệu bởi* $\mathbf{P}(V)$, *là thương của phần bù* $V - \{0\}$ *của* $\{0\}$ *trong* $V$ *theo quan hệ tương đương* $\Delta(V)$ *"tồn tại* $\lambda \neq 0$ *trong* $K$ *sao cho* $y = \lambda x$ *(resp.* $y = x \lambda$ ) *giữa* $x$ *và* $y$ *trong* $V - \{0\}$.

Khi $V = K_s^{n+1}$, ta cũng viết $\mathbf{P}_n(K)$ thay cho $\mathbf{P}(K_s^{n+1})$ và $\Delta_n(K)$ thay cho $\Delta(V)$.

Định nghĩa 4 cũng có thể được phát biểu bằng cách nói rằng $\mathbf{P}(V)$ là tập hợp các đường thẳng (đi qua 0) trong $V$ sau khi bỏ gốc đi; do đó $\mathbf{P}(V)$ được đồng nhất một cách chính tắc với tập hợp các đường thẳng (đi qua 0) trong $V$. Các phần tử của một không gian xạ ảnh được gọi là các *điểm* của không gian đó.

Khi $V$ có chiều $n$, số nguyên $n - 1$ được gọi là *chiều* của không gian xạ ảnh $\mathbf{P}(V)$ nếu $n$ hữu hạn, và là lực lượng $n$ nếu không; lực lượng này được ký hiệu bởi $\dim_K \mathbf{P}(V)$ hoặc $\dim \mathbf{P}(V)$. Như vậy một không gian xạ ảnh có chiều $-1$ là rỗng và một không gian xạ ảnh có chiều 0 là một điểm duy nhất. Một không gian xạ ảnh có chiều 1 (resp. 2) được gọi là *đường thẳng xạ ảnh* (resp. *mặt phẳng xạ ảnh*).

Từ đây về sau ta sẽ chỉ xét các không gian xạ ảnh trái.

### 6. TỌA ĐỘ THUẦN NHẤT

Cho $V$ là một không gian vectơ có số chiều hữu hạn $n + 1$ trên $K$, $\mathbf{P}(V)$ là không gian xạ ảnh chiều $n$ dẫn xuất từ $V$ và $(e_i)_{0 \leq i \leq n}$ là một cơ sở của $V$. Ký hiệu $\pi$ là ánh xạ chính tắc từ $V - \{0\}$ lên tập thương $\mathbf{P}(V)$. Với mọi điểm $x = \sum_{i=0}^{n} \xi_i e_i$ của $V - \{0\}$, $(\xi_0, \xi_1, \ldots, \xi_n)$ được gọi là một *hệ tọa độ thuần nhất* của điểm $\pi(x)$ đối với cơ sở $(e_i)$ của $V$. Do đó, mọi hệ $(\xi_i)$ gồm $n + 1$ phần tử *không đồng thời bằng không* của $K$ đều là một hệ tọa độ thuần nhất của một điểm của $P(V)$ đối với $(e_i)$; để hai hệ như vậy $(\xi_i)$, $(\xi'_i)$ là những hệ tọa độ thuần nhất của cùng một điểm của $P(V)$ đối với cùng cơ sở $(e_i)$, điều kiện cần và đủ là tồn tại một phần tử $\lambda \neq 0$ của $K$ sao cho $\xi'_i = \lambda \xi_i$ với $0 \leq i \leq n$.

Định nghĩa này được tổng quát hóa ngay lập tức cho trường hợp $V$ là vô hạn chiều.

Cho một cơ sở khác $(\tilde{e}_i)$ của $V$ sao cho $e_i = \sum_{j=0}^{n} \alpha_{ij} \tilde{e}_j$ ($0 \leq i \leq n$) và một hệ $(\xi_i)$ các tọa độ thuần nhất của $\pi(x)$ đối với cơ sở $(e_i)$, để một hệ $(\bar{\xi}_i)$ gồm $n + 1$ phần tử của $K$ là một hệ tọa độ thuần nhất của $\pi(x)$ đối với cơ sở $(\tilde{e}_i)$, điều kiện cần và đủ là tồn tại $\lambda \neq 0$ trong $K$ sao cho

$$
\lambda \bar{\xi}_i = \sum_{j=0}^{n} \xi_j \alpha_{ji} \quad \text{với } 0 \leq i \leq n.
$$

Đặc biệt, nếu $e_i = \gamma_i \tilde{e}_i$ với $\gamma_i \neq 0$ ($0 \leq i \leq n$), thì $\bar{\xi}_i = \mu \xi_i \gamma_i$ trong đó $\mu \neq 0$.

### 7. ĐA TẠP TUYẾN TÍNH XẠ ẢNH

Cho $W$ là một không gian con vectơ của một không gian vectơ $V$; ảnh chính tắc của $W - \{0\}$ trong không gian xạ ảnh $P(V)$ dẫn xuất từ $V$ được gọi là một *đa tạp tuyến tính xạ ảnh* (hoặc đơn giản là một *đa tạp tuyến tính* khi không sợ nhầm lẫn); vì quan hệ tương đương $\Delta(W)$ trên $W - \{0\}$ được cảm sinh bởi quan hệ $\Delta(V)$, đa tạp tuyến tính xạ ảnh là ảnh của $W - \{0\}$ trong $P(V)$ có thể được đồng nhất với không gian xạ ảnh $P(W)$ dẫn xuất từ $W$ và do đó ta có thể nói đến chiều của một đa tạp như vậy. Trong một không gian xạ ảnh $P(V)$, ảnh chính tắc của một siêu phẳng (bỏ gốc đi) của $V$ là một đa tạp tuyến tính được gọi là một *siêu phẳng xạ ảnh* (hoặc đơn giản là một *siêu phẳng*); nếu $P(V)$ có số chiều hữu hạn $n$ thì các siêu phẳng trong $P(V)$ là các đa tạp tuyến tính có chiều $n - 1$.

Mọi mệnh đề về các không gian con vectơ của một không gian vectơ đều chuyển thành một mệnh đề về các đa tạp tuyến tính xạ ảnh. Ví dụ, nếu một không gian xạ ảnh $P(V)$ có số chiều hữu hạn $n$ và $(e_i)_{0 \leq i \leq n}$ là một cơ sở của $V$, thì mọi đa tạp tuyến tính $L \subset P(V)$ có chiều $r$ có thể được xác định bởi một hệ gồm $n - r$ phương trình tuyến tính thuần nhất

$$
\sum_{i=0}^{n} \xi_i \alpha_{ij} = 0 \qquad (1 \leq j \leq n - r)
$$

giữa các tọa độ thuần nhất $\xi_i$ ($0 \leq i \leq n$) của một điểm của $\mathbf{P}(V)$ đối với cơ sở $(e_i)$, với các vế trái của (4) là các dạng độc lập tuyến tính trên V. Đặc biệt, một siêu phẳng xạ ảnh được xác định bởi một phương trình tuyến tính thuần nhất duy nhất với các hệ số không đồng thời bằng không. Ngược lại, các điểm của $\mathbf{P}(V)$ thỏa mãn một hệ tùy ý các phương trình tuyến tính thuần nhất đối với các $\xi_i$ lập thành một đa tạp tuyến tính L; nếu hệ đang xét gồm $k \leq n + 1$ phương trình, thì L có chiều $\geq n - k$.

Mọi giao của các đa tạp tuyến tính của $\mathbf{P}(V)$ đều là một đa tạp tuyến tính; với mọi tập con A của $\mathbf{P}(V)$, tồn tại một đa tạp tuyến tính nhỏ nhất L chứa A; nó được gọi là đa tạp tuyến tính *sinh bởi* A và A được gọi là một *hệ sinh* của L.

Nếu W là không gian con vectơ của V sinh bởi $\pi^{-1}(A)$, thì $L = \mathbf{P}(W)$.

Nếu L và M là hai đa tạp tuyến tính bất kỳ trong $\mathbf{P}(V)$ và N là đa tạp sinh bởi $L \cup M$, thì (§ 7, no. 3, Hệ quả 3 của Mệnh đề 4)

$$
\text{dim } L + \text{dim } M = \text{dim}(L \cap M) + \text{dim } N.
$$

Đặc biệt, nếu $\mathbf{P}(V)$ hữu hạn chiều và $\text{dim } L + \text{dim } M \geq \text{dim } \mathbf{P}(V)$, thì từ (5) suy ra rằng $L \cap M$ khác rỗng.

Cho $(x_i), (y_i)$ là hai họ điểm trong không gian vectơ V có cùng tập hợp chỉ số, sao cho $y_i = \lambda_i x_i$, với $\lambda_i \neq 0$ với mọi $i$. Nếu họ $(x_i)$ là tự do thì họ $(y_i)$ cũng vậy, và ngược lại; khi đó ta nói rằng họ các điểm $\pi(x_i)$ của $\mathbf{P}(V)$ là *tự do xạ ảnh* (hoặc đơn giản là *tự do*). Điều này tương đương với việc nói rằng với mọi chỉ số $\kappa$, điểm $\pi(x_\kappa)$ không thuộc đa tạp tuyến tính sinh bởi các $\pi(x_i)$ với $i \neq \kappa$. Một họ điểm của $\mathbf{P}(V)$ không tự do xạ ảnh được gọi là *liên quan xạ ảnh* (hoặc đơn giản là *liên quan*).

Để một họ $(x_i)$ các điểm của $V - \{0\}$ có tính chất là họ $(\pi(x_i))$ là tự do xạ ảnh và sinh ra $\mathbf{P}(V)$, điều kiện cần và đủ là $(x_i)$ là một cơ sở của V. Do đó nếu $\mathbf{P}(V)$ có chiều $n$ thì số phần tử của một họ như vậy là $n + 1$. Chú ý rằng việc cho một họ như vậy $(\pi(x_i))$ trong $\mathbf{P}(V)$ không xác định các tọa độ thuần nhất của một điểm đã cho của $\mathbf{P}(V)$ đối với một cơ sở $(y_i)$ của V sao cho $\pi(y_i) = \pi(x_i)$ với mọi $i$ (ngay cả chỉ đến một nhân tử trái) (xem no. 6).

### 8. BÙ XẠ ẢNH CỦA MỘT KHÔNG GIAN AFIN

Cho V là một không gian vectơ (trái) trên một trường K và xét không gian vectơ $K_s \times V$ trên K; không gian xạ ảnh $\mathbf{P}(K_s \times V)$ được gọi là không gian xạ ảnh *liên kết một cách chính tắc* với không gian vectơ V. Nếu V có chiều $n$ thì $\mathbf{P}(K_s \times V)$ cũng có cùng chiều $n$. Xét trong $K_s \times V$ siêu phẳng afin $V_1 = \{1\} \times V$, mà phương của nó (no. 3) là không gian con $V_0 = \{0\} \times V$; nếu một đường thẳng (đi qua 0) của $K_s \times V$ không được chứa trong $V_0$, thì nó chứa một điểm $(\alpha, x)$ với $\alpha \neq 0$ và $x \in V$, nên nó cũng chứa điểm $\alpha^{-1}(\alpha, x) = (1, \alpha^{-1}x)$ của $V_1$; đảo lại là ngay lập tức, và ta thấy rằng có một sự tương ứng một-một giữa các điểm của $V_1$ và các đường thẳng (đi qua 0) của $K_s \times V$ không được chứa trong $V_0$, mỗi đường thẳng thuộc loại sau cắt $V_1$ tại một và chỉ một điểm. Suy ra ánh xạ $x \mapsto \phi(x) = \pi(1, x)$ là một đơn ánh (được gọi là chính tắc) từ $V$ vào không gian xạ ảnh $P(K_s \times V)$; người ta thường đồng nhất $V$ với ảnh của nó qua đơn ánh này. Phần bù của $\phi(V)$ trong $P(K_s \times V)$ là siêu phẳng xạ ảnh $P(V_0)$, được gọi là siêu phẳng ở vô cùng của $P(K_s \times V)$ (hoặc của $V$, theo một sự lạm dụng ngôn ngữ); các điểm của nó cũng được gọi là "các điểm ở vô cùng" của $P(K_s \times V)$ (hoặc của $V$). Nếu $(a_i)$ là một cơ sở của $V$ và trong $K_s \times V$ ta lấy cơ sở gồm các phần tử $e_i = (0, a_i)$ và phần tử $e_\omega = (1, 0)$, thì các điểm ở vô cùng trong $P(K_s \times V)$ là những điểm mà tọa độ thuần nhất có chỉ số $\omega$ bằng 0.

Cho $M$ là một đa tạp tuyến tính afin trong $V$ (no. 3) và $D$ là phương của nó; ảnh chính tắc $\phi(M)$ của $M$ trong $P(K_s \times V)$ được chứa trong ảnh chính tắc $\overline{M} = \pi(M_2)$ của không gian con vectơ $M_2$ của $K_s \times V$ sinh bởi đa tạp afin $M_1 = \{1\} \times M$ của $K_s \times V$. Chính xác hơn, nếu $(a_i)$ là một hệ afin tự do của $M$ sinh ra $M$, thì các phần tử $(1, a_i)$ lập thành một cơ sở của $M_2$ và do đó $\overline{M}$ chính là đa tạp tuyến tính xạ ảnh sinh bởi $\phi(M)$; nếu $M$ hữu hạn chiều, thì $\overline{M}$ có cùng chiều với $M$. Phần bù của $\phi(M)$ trong $\overline{M}$ là giao của $\overline{M}$ với siêu phẳng ở vô hạn và bằng ảnh chính tắc $\pi(M_0)$, trong đó $M_0 = \{0\} \times D$.

Ngược lại, cho $N$ là một đa tạp tuyến tính xạ ảnh không được chứa trong siêu phẳng ở vô hạn và đặt $R = \pi^{-1}(N)$; $R \cap V_1$ là một đa tạp tuyến tính afin của $K \times V$ có dạng $\{1\} \times M$, trong đó $M$ là một đa tạp tuyến tính afin của $V$, và ngay lập tức thấy rằng $N$ là đa tạp tuyến tính afin $\overline{M}$ sinh bởi $\phi(M)$.

Vì vậy có một sự tương ứng một-một giữa các đa tạp tuyến tính afin của $V$ và các đa tạp tuyến tính xạ ảnh của $P(K_s \times V)$ không được chứa trong siêu phẳng ở vô hạn; để hai đa tạp tuyến tính afin của $V$ song song với nhau, điều kiện cần và đủ là các đa tạp tuyến tính xạ ảnh mà chúng sinh ra có cùng giao với siêu phẳng ở vô hạn (điều này đôi khi được diễn đạt bằng cách nói rằng hai đa tạp tuyến tính afin đang xét có cùng các điểm ở vô hạn).

### 9. MỞ RỘNG CÁC HÀM HỮU TỈ

Nếu áp dụng các kết quả của no. 8 cho không gian vectơ $V = K_s$ có chiều bằng 1, thì thấy rằng tồn tại một đơn ánh chính tắc $\phi$ từ $K_s$ vào đường thẳng xạ ảnh $P_1(K) = P(K_s \times K_s)$; với mọi $\xi \in K$, $\phi(\xi)$ là điểm có tọa độ thuần nhất $(1, \xi)$ đối với cơ sở chính tắc (§ 1, no. 11) của $K_s \times K_s$. Phần bù của $\phi(K)$ trong $P_1(K)$ chỉ gồm một điểm duy nhất có tọa độ thuần nhất $(0, 1)$ đối với cơ sở trên; điểm đó được gọi là "điểm ở vô hạn". $P_1(K)$ cũng được gọi là trường xạ ảnh liên kết với $K$ và được ký hiệu bởi $\tilde{K}$, điểm ở vô hạn trong $\tilde{K}$ được ký hiệu bởi $\infty$.

*Xét đặc biệt trường hợp $K$ là một trường giao hoán và gọi f \in K(X) là một hàm hữu tỉ theo một ẩn trên $K$ (IV, § 4); nếu $f \neq 0$, có một biểu thức duy nhất $f = \alpha p/q$, trong đó $\alpha \in K^*$ và $p$ và $q$ là hai đa thức đơn nhất nguyên tố cùng nhau (VII, § 1); gọi $m$ và $n$ là các bậc tương ứng của chúng và đặt $r = \sup(m, n)$. Ta viết $$
p_1(T, X) = T^r p(X/T), \qquad q_1(T, X) = T^r q(X/T);
$$ $p_1$ và $q_1$ là hai đa thức thuần nhất bậc $r$ trên $K$ sao cho $p(X) = p_1(1, X)$, $q(X) = q_1(1, X)$. Do đó, với mọi phần tử $\xi \in K$ không là một không của $q(X)$, $f(\xi) = \alpha p(\xi)/q(\xi)$ được xác định và ta có thể viết $$
f(\xi) = \alpha p_1(1, \xi)/q_1(1, \xi) = \alpha p_1(\lambda, \lambda \xi)/q_1(\lambda, \lambda \xi)
$$ với mọi $\lambda \neq 0$ trong $K$. Khi đó xét ánh xạ $$
(\eta, \xi) \mapsto (q_1(\eta, \xi), p_1(\eta, \xi))
$$ từ $K^2$ vào chính nó; nó tương thích với quan hệ tương đương $\Delta(K^2)$ và do đó, khi chuyển qua các thương, xác định một ánh xạ $\tilde{f}$ từ $\tilde{K}$ vào chính nó, trùng với $\xi \mapsto f(\xi)$ tại những điểm mà hàm hữu tỉ này được xác định; người ta gọi, do lạm dụng ngôn ngữ, rằng $\tilde{f}$ là mở rộng chính tắc của $f$ lên $\tilde{K}$.

Ví dụ, nếu $f = 1/X$, thì $\tilde{f}(0) = \infty$ và $\tilde{f}(\infty) = 0$; nếu
$$
f = (aX + b)/(cX + d)
$$
với $ad - bc \neq 0$, thì $\tilde{f}(-d/c) = \infty$, $\tilde{f}(\infty) = a/c$ nếu $c \neq 0$, $\tilde{f}(\infty) = \infty$ nếu $c = 0$. Nếu $f = a_0 X^n + \cdots + a_n$ là một đa thức bậc $n > 0$, thì $\tilde{f}(\infty) = \infty$*

### 10. CÁC ÁNH XẠ TUYẾN TÍNH XẠ ẢNH

Cho $V, V'$ là hai không gian vectơ trái trên một trường $K$, $f$ là một ánh xạ tuyến tính của $V$ vào $V'$ và $N = \overline{f}(0)$ là hạt nhân của nó. Chú ý rằng ảnh dưới $f$ của một đường thẳng (đi qua 0) trong $V$ không được chứa trong $N$ là một đường thẳng (đi qua 0) trong $V'$; do đó, khi chuyển qua các thương, $f$ xác định một ánh xạ $g$ từ $P(V) - P(N)$ vào $P(V')$. Một ánh xạ như vậy được gọi là một ánh xạ tuyến tính xạ ảnh (hoặc, đơn giản, là một ánh xạ xạ ảnh); mặc dù nó được xác định trên $P(V) - P(N)$ chứ không phải trên $P(V)$ (khi $N \neq \{0\}$), theo một lối nói lạm dụng, ta sẽ nói rằng $g$ là một ánh xạ xạ ảnh của $P(V)$ vào $P(V')$. Đa tạp tuyến tính xạ ảnh $P(N)$, tại đó $g$ không được xác định, được gọi là tâm của $g$.

Chú ý rằng, khi $g$ được xác định trên toàn bộ $P(V)$ (nghĩa là khi $N = \{0\}$), $g$ là một đơn ánh từ $P(V)$ vào $P(V')$.

Khi cho các cơ sở $(a_\lambda)_{\lambda \in L}, (b_\mu)_{\mu \in M}$ lần lượt trong $V$ và $V'$, một ánh xạ xạ ảnh của $P(V)$ vào $P(V')$ biến một điểm của $P(V)$ có các tọa độ thuần nhất $\xi_\lambda$ ($\lambda \in L$) thành một điểm của $\mathbf{P}(V')$ có một hệ tọa độ thuần nhất $\eta_\mu$ ($\mu \in M$) có dạng

$$
\eta_\mu = \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} \quad (\alpha_{\lambda \mu} \in K).
$$

Tâm của $g$ là đa tạp tuyến tính được xác định bởi các phương trình

$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} = 0 \quad (\mu \in M).
$$

Nếu $C$ là tâm của $g$ và $M$ là một đa tạp tuyến tính của $\mathbf{P}(V)$, ảnh dưới $g$ của $M - (M \cap C)$ là một đa tạp tuyến tính của $\mathbf{P}(V')$ được ký hiệu (theo một lối nói lạm dụng) bởi $g(M)$. Khi đó

$$
\dim g(M) + \dim(M \cap C) + 1 = \dim M
$$

(§ 7, no. 4, công thức (12)). Nếu $M'$ là một đa tạp tuyến tính của $\mathbf{P}(V')$, $g^{-1}(M') \cup C$ là một đa tạp tuyến tính của $\mathbf{P}(V)$ và

$$
\dim(g^{-1}(M') \cup C) = \dim C + \dim(M' \cap g(\mathbf{P}(V))) + 1.
$$

Theo một lối nói lạm dụng, người ta nói rằng $g^{-1}(M') \cup C$ là *ảnh ngược* của $M'$ dưới $g$.

Vì các giá trị mà một ánh xạ tuyến tính lấy trên một cơ sở $(e_i)$ của $V$ có thể được chọn *tùy ý* trong $V'$, nên suy ra tồn tại một ánh xạ xạ ảnh của $\mathbf{P}(V)$ vào $\mathbf{P}(V')$ nhận các giá trị *tùy ý* tại các điểm $\pi(e_i)$. Nhưng (ngay cả khi $g$ được xác định khắp nơi) việc cho $g(\pi(e_i))$ không xác định $g$ một cách duy nhất (Bài tập 10).

Hợp thành của hai ánh xạ xạ ảnh là các song ánh là một ánh xạ xạ ảnh; ánh xạ nghịch đảo của một song ánh như vậy cũng thế. Do đó các ánh xạ xạ ảnh song ánh của một không gian xạ ảnh $\mathbf{P}(V)$ lên chính nó lập thành một nhóm, gọi là *nhóm xạ ảnh* của $\mathbf{P}(V)$ và ký hiệu bởi $\mathbf{PGL}(V)$; ta viết $\mathbf{PGL}_n(K)$ hoặc $\mathbf{PGL}(n, K)$ thay cho $\mathbf{PGL}(K^n_s)$.

#### Nhận xét {#alg-ii-s9-n10-rem-1 .statement}

Trong một không gian xạ ảnh $\mathbf{P}(V)$ trên một trường $K$, cho $H = \mathbf{P}(W)$ là một siêu phẳng. Tồn tại một ánh xạ tuyến tính song ánh $f$ của $V$ lên $K_s \times W$ sao cho $f(W) = W$; gọi $g$ là ánh xạ xạ ảnh thu được từ $f$ bằng cách chuyển sang thương. Đã thấy (no. 8) rằng phần bù của $\mathbf{P}(W)$ trong $\mathbf{P}(K_s \times W)$ có thể được đồng nhất với một không gian afin mà không gian tịnh tiến là $W$. Khi $\mathbf{P}(V)$ được đồng nhất với $\mathbf{P}(K_s \times W)$ nhờ $g$, người ta nói rằng $H$ *đã được lấy làm siêu phẳng ở vô tận* trong $\mathbf{P}(V)$; khi đó phần bù của $H$ trong $\mathbf{P}(V)$ được đồng nhất với một không gian afin mà không gian tịnh tiến là $W$.

### 11. CẤU TRÚC KHÔNG GIAN XẠ ẢNH

Cho một tập hợp E và một trường K, một cấu trúc không gian xạ ảnh (trái) trên E đối với trường K được định nghĩa bằng cách cho một tập hợp không rỗng $\Phi$ gồm các song ánh từ các tập con của không gian xạ ảnh $\mathbf{P}(K_s^{(E)})$ lên E, thỏa mãn các tiên đề sau đây:

$$(\mathrm{EP}_I)$$ *Tập xác định của mọi ánh xạ $f \in \Phi$ là một đa tạp tuyến tính của $\mathbf{P}(K_s^{(E)})$.*

$$(\mathrm{EP}_{II})$$ *Với mọi cặp có thứ tự các phần tử $f, g$ của $\Phi$ được xác định tương ứng trên các đa tạp tuyến tính $\mathbf{P}(V)$ và $\mathbf{P}(W)$, song ánh $h = g^{-1} \circ f$ của $\mathbf{P}(V)$ lên $\mathbf{P}(W)$ là một ánh xạ xạ ảnh.*

$$(\mathrm{EP}_{III})$$ *Ngược lại, nếu $f \in \Phi$ được xác định trên đa tạp tuyến tính $\mathbf{P}(V)$ và $h$ là một ánh xạ xạ ảnh song ánh của $\mathbf{P}(V)$ lên một đa tạp tuyến tính $\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$, thì $f \circ h^{-1} \in \Phi$.*

Cho E là một tập hợp, $(V_\lambda)_{\lambda \in L}$ là một họ các không gian vectơ trên K và giả sử với mỗi $\lambda \in L$ cho trước một song ánh $f_\lambda$ từ $\mathbf{P}(V_\lambda)$ lên E sao cho, với mọi cặp có thứ tự các chỉ số $\lambda, \mu$, $f_\lambda^{-1} \circ f_\mu$ là một *ánh xạ xạ ảnh* từ $\mathbf{P}(V_\mu)$ lên $\mathbf{P}(V_\lambda)$. Khi đó ta có thể định nghĩa trên E một cấu trúc không gian xạ ảnh đối với K như sau: lấy $(e_i)_{i \in I}$ là một cơ sở của một không gian $V_\lambda$ và đặt $a_i = f_\lambda(\pi(e_i))$; gọi $b_i$ là phần tử có chỉ số $a_i$ trong cơ sở chính tắc của $K_s^{(E)}$ (§ 1, no. 11). Quan hệ $i \neq \kappa$ kéo theo $b_i \neq b_\kappa$ do giả thiết rằng $f_\lambda$ là song ánh; do đó các $b_i$ tạo thành một cơ sở của một không gian con vectơ $W_0$ của $K_s^{(E)}$ và vì thế tồn tại một ánh xạ xạ ảnh song ánh $h$ từ $\mathbf{P}(W_0)$ lên $\mathbf{P}(V_\lambda)$ sao cho $h(\pi(b_i)) = \pi(e_i)$ với mọi $i \in I$. Nếu ký hiệu $\Phi$ là tập hợp tất cả các ánh xạ xạ ảnh song ánh $f_\lambda \circ h \circ g^{-1}$, trong đó $g$ chạy qua tập hợp tất cả các ánh xạ xạ ảnh song ánh $\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$, thì kiểm tra ngay lập tức được rằng $\Phi$ thỏa mãn các tiên đề (EP_I), (EP_{II}) và (EP_{III}). Hơn nữa, cũng ngay lập tức thấy rằng $\Phi$ không phụ thuộc vào việc lựa chọn chỉ số $\lambda \in L$, cũng không phụ thuộc vào việc lựa chọn cơ sở $(e_i)$ trong $V_\lambda$, cũng không phụ thuộc vào việc lựa chọn $h$.

Đặc biệt (khi lấy L chỉ gồm một phần tử), mọi không gian xạ ảnh $\mathbf{P}(V)$ dẫn xuất từ một không gian vectơ V (no. 5, định nghĩa 4) do đó đều có một "cấu trúc không gian xạ ảnh" được xác định rõ ràng theo nghĩa của định nghĩa đã cho trong no. này. Vì thế mọi tập hợp được trang bị một cấu trúc không gian xạ ảnh đều có thể được gọi là một *không gian xạ ảnh*.

Với cùng ký hiệu ấy, một *đa tạp tuyến tính* trong một không gian xạ ảnh E là một tập con M của E sao cho, đối với ít nhất *một* song ánh $f \in \Phi$ được xác định trên $\mathbf{P}(V) \subset \mathbf{P}(K_s^{(E)})$, $f^{-1}(M)$ là một đa tạp tuyến tính trong $\mathbf{P}(V)$ theo nghĩa của no. 7 (khi đó tính chất này đúng với *mọi* $f \in \Phi$). Từ điều trên suy ra rằng mọi đa tạp tuyến tính trong một không gian xạ ảnh đều có một cách chính tắc một cấu trúc không gian xạ ảnh.

Một không gian xạ ảnh E được gọi là *có chiều n* nếu, với mọi $f \in \Phi, f^{-1}(E)$ là một đa tạp tuyến tính có chiều n (chỉ cần điều này đúng với *một* ánh xạ $f \in \Phi$).

### Bài tập {#alg-ii-s9-exercises}

Xem [các bài tập của § 9](exercises/s9/).
