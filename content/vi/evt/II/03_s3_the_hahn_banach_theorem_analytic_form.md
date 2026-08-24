---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 3
section_title: The Hahn-Banach Theorem (analytic form)
lang: vi
source: evt-i-v
book_pages: TVS II.21-TVS II.23, TVS II.72-TVS II.74
pdf_pages: 0058-0060, 0109-0111
extraction: ocr
subsections:
    - "no": 1
      title: Extension of positive linear forms
      page: 21
      pdf_page: 58
    - "no": 2
      title: The Hahn-Banach theorem (analytic form)
      page: 22
      pdf_page: 59
statements: 6
exercises: 8
content_sha256: d364a428f37194a61dbe7525627f7f06269652d08299bc08ad6b8eca483f08a8
translated_from: content/en/evt/II/03_s3_the_hahn_banach_theorem_analytic_form.md
source_content_sha256: 0aea7a7a7c11a906853b8b153e32f9152738a2304edacc86af18cebd51c10233
translation_model: gpt-5.4, gpt-5-6
translation_run: translate-vi-4a007b50
glossary_version: 34
glossary_terms_sha256: 7cf957e2a97579ae99596d4ae6ee3089d99021bb09bc909ad70eb4b9db4f6c69
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ĐỊNH LÝ HAHN-BANACH (DẠNG GIẢI TÍCH)

### 1. Mở rộng các dạng tuyến tính dương

#### Mệnh đề 1 {#evt-ii-s3-prop-1 .statement}

— Cho E là một không gian vectơ tiền thứ tự và V là một không gian con vectơ của E sao cho mọi phần tử của E đều bị chặn trên bởi một phần tử của V. Với một dạng tuyến tính f trên V, dương đối với cấu trúc không gian vectơ tiền thứ tự của V (cảm sinh bởi cấu trúc của E), tồn tại một tập hợp không rỗng $ S_f $ các dạng tuyến tính dương trên E, mỗi dạng là một mở rộng của f. Nếu $ h \in S_f $ thì các giá trị $ h(a) $ với $ a \in E $ nằm trong khoảng $ [\alpha', \alpha''] $, trong đó

$$
\alpha' = \sup_{z \in V, z \leq a} f(z), \quad \alpha'' = \inf_{y \in V, y \geq a} f(y).
$$

I. Trường hợp riêng.

Trước hết giả sử rằng $ E = V + \mathbf{R}a $. Vì mệnh đề là tầm thường nếu $ a \in V $, ta chỉ xét trường hợp $ a \notin V $. Các giả thiết đối với V kéo theo rằng tập hợp $ A'' $ các $ y \in V $ sao cho $ a \leq y $ là không rỗng; tương tự, tập hợp $ A' $ các $ z \in V $ sao cho $ -z \geq -a $ (\emph{tức là} $ z \leq a $) là không rỗng. Với $ y \in A'' $ và $ z \in A' $, ta có $ z \leq a \leq y $, và do đó theo giả thiết $ f(z) \leq f(y) $. Vậy $ \alpha', \alpha'' $ là hữu hạn và $ \alpha' \leq \alpha'' $. Mọi dạng tuyến tính $ f_1 $ trên E mở rộng $ f $ đều được xác định hoàn toàn bởi $ f_1(a) $ và với mọi $ \lambda \in \mathbf{R} $ và mọi $ x \in V $, ta có

$$
f_1(x + \lambda a) = f(x) + \lambda f_1(a).
$$

Do đó $ f_1 $ là dương khi và chỉ khi các hệ thức

$$
x \in V, \quad \lambda \in \mathbf{R}, \quad x + \lambda a \geq 0
$$

suy ra

$$
f(x) + \lambda f_1(a) \geq 0.
$$

Vì $ f(\mu x) = \mu f(x) $ và các quan hệ $ x \geq 0 $ và $ \mu x \geq 0 $ là tương đương đối với $ \mu > 0 $, nên chỉ cần chỉ ra rằng (2) kéo theo (3) trong các trường hợp riêng $ \lambda = 0, \lambda = 1 $ và $ \lambda = -1 $. Với $ \lambda = 0 $, việc (2) kéo theo (3) suy ra từ giả thiết rằng $ f $ là dương. Với $ \lambda = 1 $, nói rằng (2) kéo theo (3) có nghĩa là với $ -x \in A' $, ta có $ f_1(a) \geq f(-x) $, \emph{tức là} $ f_1(a) \geq \alpha' $; với $ \lambda = -1 $, (2) kéo theo (3) có nghĩa là với $ x \in A'' $, ta có $ f(x) \geq f_1(a) $, \emph{tức là} $ f_1(a) \leq \alpha'' $. Vậy mệnh đề được chứng minh trong trường hợp này.

II. Trường hợp tổng quát.

Cho $ \mathfrak{F} $ là tập hợp các cặp $(W, g)$ trong đó $W$ là một không gian con vectơ của $E$ chứa $V$ và $g$ là một dạng tuyến tính dương trên $W$ là một mở rộng của $f$. Ta sắp thứ tự $ \mathfrak{F} $ bằng cách đặt $(W, g) \leq (W', g')$ nếu $W \subset W'$ và nếu $g'$ là một mở rộng của $g$. Rõ ràng $ \mathfrak{F} $ là quy nạp và theo đl. 2 của S, III, § 2.4, tồn tại một phần tử cực đại $(W_0, g_0)$. Giả sử $W_0 \neq E$. Khi đó tồn tại một vectơ $b \notin W_0$, và, nếu đặt $W_1 = W_0 + \mathbf{R}b$, trường hợp riêng ở trên cho thấy rằng tồn tại một dạng tuyến tính dương trên $W_1$ là một mở rộng của $g_0$; điều này mâu thuẫn với giả thiết rằng $(W_0, g_0)$ là cực đại. Vậy $W_0 = E$, và phần thứ nhất của mệnh đề được chứng minh. Khi $a \in V$, mệnh đề thứ hai hiển nhiên đúng với $\alpha' = \alpha'' = f(a)$; nếu, trái lại, $a \notin V$ và đặt $V_1 = V + \mathbf{R}a$, thì mệnh đề thứ hai suy ra từ trường hợp riêng I của chứng minh.

#### Hệ quả {#evt-ii-s3-n1-cor-1 .statement}

Trong một không gian vectơ tôpô $E$ với một cấu trúc tiền thứ tự tương thích, cho $P$ là tập hợp các phần tử $\geq 0$ trong $E$. Cho $V$ là một không gian con vectơ của $E$ chứa ít nhất một điểm trong $x_0$ của $P$. Khi đó mọi dạng tuyến tính dương trên $V$ đều có thể được mở rộng thành một dạng tuyến tính dương trên $E$.

Theo mệnh đề 1, chỉ cần chứng tỏ rằng với mọi $x \in E$, tồn tại $x' \in V$ sao cho $x' - x \in P$. Bây giờ lấy $U$ là một lân cận của $0$ trong $E$ sao cho $x_0 + U \subset P$. Khi đó $x + x_0 + U \subset x + P$, và do đó tồn tại $\varepsilon$ sao cho $0 < \varepsilon < 1$ và điểm $y = x_0 + (1 - \varepsilon)x$ thuộc $x + P$; khi đó mọi điểm có dạng $x + \lambda(y - x)$ đều thuộc $x + P$ với $\lambda > 0$. Nếu lấy $\lambda = 1/\varepsilon$, thì $x + \lambda(y - x) = \lambda x_0 \in V$, từ đó suy ra kết luận.

Kết luận của hệ quả không nhất thiết còn đúng nếu không giả thiết rằng $V$ chứa một điểm trong của $P$, ngay cả khi $E$ có số chiều hữu hạn và khi $P \cap V$ chứa các điểm trong đối với $V$ (II, p. 91, bài tập 25, b)).

### 2. Định lý Hahn-Banach (dạng giải tích)

#### Định lý 1 (Hahn-Banach) {#evt-ii-s3-thm-1 .statement}

Cho $p$ là một hàm dưới tuyến tính trên một không gian vectơ $E$. Cho $V$ là một không gian con vectơ của $E$ và $f$ là một dạng tuyến tính trên $V$ sao cho, với mọi $y \in V$, ta có $f(y) \leq p(y)$. Khi đó tồn tại một dạng tuyến tính $h$ trên $E$ là một mở rộng của $f$ và sao cho $h(x) \leq p(x)$ với $x \in E$.

Tập hợp các cặp $(x, a)$ sao cho $p(x) \leq a$ là một tập con lồi $P$ của không gian vectơ $E_1 = E \times \mathbf{R}$ (II, p. 17, mệnh đề 19), và rõ ràng nó là một nón nhọn. Gọi $V_1$ là không gian con $V \times \mathbf{R}$ của $E_1$ và $g(y, a) = -f(y) + a$ với mỗi điểm $(y, a) \in V_1$. Khi đó $g$ là một dạng tuyến tính dương đối với cấu trúc tiền thứ tự trên $V_1$ được xác định bởi $P \cap V_1$; thật vậy, nếu $(y, a) \in P \cap V_1$, thì $a \geq p(y) \geq f(y)$, do đó $g(y, a) \geq 0$. Tiếp theo, lấy $(x, a) \in E_1$; ta chứng minh rằng $(x, a)$ nhỏ hơn một điểm của $V_1$ đối với tiền thứ tự được xác định bởi $P$. Nếu $(x', a') \in V_1$ thì $(x, a) \leq (x', a')$ khi và chỉ khi $p(x' - x) \leq a' - a$, lấy $a' \geq p(-x) + a$, ta thấy rằng $(0, a')$ của $V_1$ thỏa mãn các điều kiện cần có. Do đó ta có thể áp dụng mệnh đề I của II, p. 21; tồn tại một dạng tuyến tính $u$ trên $E_1$ kéo dài $g$ và dương đối với tiền thứ tự được xác định bởi $P$. Vì thế $u(0, 1) = g(0, 1) = 1$ và $u$ có dạng $u(x, a) = -h(x) + a$, trong đó $h$ là một dạng tuyến tính trên $E$ kéo dài $f$; hơn nữa, với mọi $x \in E$ và mọi $a \geq p(x)$, ta có $h(x) \leq a$, do đó $h(x) \leq p(x)$. Q.E.D.

#### Hệ quả 1 {#evt-ii-s3-thm-1-cor-1 .statement}

— Cho $ p $ là một nửa chuẩn trên không gian vectơ $ E $. Cho $ V $ là một không gian con vectơ của $ E $ và $ f $ là một dạng tuyến tính trên $ V $ sao cho $ |f(y)| \leq p(y) $ với mọi $ y \in V $. Khi đó tồn tại một dạng tuyến tính $ h $ xác định trên $ E $ là một mở rộng của $ f $ và sao cho $ |h(x)| \leq p(x) $ với $ x \in E $.

Đối với một nửa chuẩn $ q $ và một dạng tuyến tính $ g $ trên $ E $, quan hệ $ g \leq q $ cũng chính là $ |g| \leq q $. Hệ quả suy ra từ đl. 1.

#### Hệ quả 2 {#evt-ii-s3-thm-1-cor-2 .statement}

— Cho $ p $ là một nửa chuẩn trên không gian vectơ $ E $. Với một điểm $ x_0 \in E $ đã cho, tồn tại một dạng tuyến tính $ f $ xác định trên $ E $, sao cho $ f(x_0) = p(x_0) $ và $ |f(x)| \leq p(x) $ với mọi $ x \in E $.

Áp dụng hệ quả 1 cho không gian con vectơ $ V $, sinh bởi $ x_0 $ và cho dạng tuyến tính $ \xi x_0 \mapsto \xi p(x_0) $ được xác định trên $ V $.

#### Hệ quả 3 {#evt-ii-s3-thm-1-cor-3 .statement}

— Cho $ V $ là một không gian con vectơ của không gian chuẩn $ E $ và cho $ f $ là một dạng tuyến tính liên tục trên $ V $; khi đó tồn tại một dạng tuyến tính liên tục $ h $ được xác định trên $ E $ mở rộng $ f $ và có cùng chuẩn (GT, X, § 3.2).

Áp dụng hệ quả 1, lấy $ p(x) = \|f\| \cdot \|x\| $, suy ra $ \|h\| \leq \|f\| $; nhưng rõ ràng $ \|h\| \geq \|f\| $, và hệ quả được suy ra.

Kết luận của hệ quả 3 không nhất thiết đúng đối với các ánh xạ tuyến tính liên tục từ một không gian chuẩn vào một không gian chuẩn tùy ý (IV, p. 55, bài tập 16, c) and V, p. 65, bài tập 22).

### Bài tập {#evt-ii-s3-exercises}

Xem [bài tập cho § 3](exercises/s3/).
