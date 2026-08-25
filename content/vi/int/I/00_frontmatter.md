---
book: int
book_title: Integration
chapter: I
chapter_title: INEQUALITIES OF CONVEXITY
section: 0
section_title: INEQUALITIES OF CONVEXITY
kind: front
lang: vi
source: int-i-vi
pdf_pages: 0016-0022
extraction: ocr
subsections:
    - "no": 1
      title: The fundamental inequality of convexity
      page: 0
      pdf_page: 16
    - "no": 3
      title: The semi-norms $N_p$
      page: 4
      pdf_page: 19
statements: 0
exercises: 0
content_sha256: e8e38b2c8caeca17303484bb14d4ccbf008eab5ca8fc3e5f2b6af8474115f31a
translated_from: content/en/int/I/00_frontmatter.md
source_content_sha256: 7903e043f4340792f2eced78a10f941d410ff38a9f8de464278d8f409206e188
translation_model: gpt-5.4
translation_run: translate-vi-5c520436
glossary_version: 34
glossary_terms_sha256: 0b3e9453f817374457d15d0c3f8a62ee799a3cd6974668db277c68f8da1180ff
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## CHƯƠNG I

# Các bất đẳng thức về tính lồi

### 1. Bất đẳng thức cơ bản về tính lồi

Cho X là một tập hợp; trong không gian vectơ $\mathbf{R}^X$ của mọi hàm số hữu hạn$^1$ xác định trên X, gọi P là tập hợp của mọi hàm nhận giá trị thực dương trên X. Mặt khác, cho $M$ là một hàm số,$^2$ hữu hạn hoặc không, nhận các giá trị $\geqslant 0$, xác định trên P, sao cho:

$1^\circ$ $M(0) = 0$, và $M$ là thuần nhất dương, nghĩa là $M(\lambda f) = \lambda M(f)$ với mọi số thực $\lambda > 0$.$^3$

$2^\circ$ $M$ tăng trên P, nói cách khác quan hệ $f \leqslant g$ kéo theo $M(f) \leqslant M(g)$.

$3^\circ$ $M$ lồi trong P, nói cách khác (TVS, II, §2, No. 8) thỏa mãn quan hệ $M(f + g) \leqslant M(f) + M(g)$.

*Ví dụ.* — Giả sử X là một tập hợp hữu hạn, chẳng hạn khoảng $[1, n]$ của $\mathbf{N}$; ký hiệu bởi $x_i$ ($1 \leqslant i \leqslant n$) các tọa độ của một vectơ $\mathbf{x} \in \mathbf{R}^n$, các hàm
$$
M_1(\mathbf{x}) = \sum_{i=1}^n x_i \quad \text{và} \quad M_\infty(\mathbf{x}) = \sup_{1 \leqslant i \leqslant n} x_i
$$
thỏa mãn các điều kiện trước trong tập hợp P của các vectơ $\mathbf{x}$ có các tọa độ $\geqslant 0$.

*Nhận xét.* — Cho S là một nón lồi nhọn được chứa trong P (nghĩa là, một tập hợp sao cho $S + S \subset S$ và $\lambda S \subset S$ với $\lambda \geqslant 0$; xem TVS, II, §2, No. 4); cho $M$ là một hàm số (hữu hạn hay không) nhận giá trị $\geqslant 0$, được định nghĩa trên S và thỏa mãn trong S các điều kiện trên $1^\circ, 2^\circ$ và $3^\circ$. Khi đó $M$ có thể được mở rộng ra toàn bộ tập hợp P, sao cho hàm mở rộng (mà ta lại ký hiệu là $M$) thỏa mãn cùng những điều kiện ấy: chỉ cần, với mọi hàm $f \in P$, đặt $M(f) = +\infty$ nếu không tồn tại hàm nào $g \in S$ sao cho $f \leqslant g$, và $M(f) = \inf_{g \in S, f \leqslant g} M(g)$ trong trường hợp ngược lại. Thủ tục này sẽ được áp dụng trong Ch. IV, §1 để định nghĩa *tích phân trên* của một hàm dương.

\footnotetext{
$^1$ Fonction numérique finie—một hàm nhận giá trị trong $\mathbf{R}$—cũng có thể được dịch là "hàm thực" (xem GT, IV, §5, No. 1).
$^2$ Fonction numérique—"hàm số"—chỉ một hàm nhận giá trị trong $\overline{\mathbf{R}}$ (TG, IV, §5, No. 1). Cụm từ "hữu hạn hay không" đôi khi cũng được thêm vào để nhắc rằng hàm có thể nhận các giá trị vô hạn.
$^3$ Nhắc lại rằng trong $\overline{\mathbf{R}}$, các tích như $0 \cdot (+\infty)$ không được xác định (GT, IV, §4, No. 3).
}

MỆNH ĐỀ 1. — Cho $\varphi(t_1, t_2, \ldots, t_n)$ là một hàm số hữu hạn, được xác định và liên tục với $t_i \geq 0$ ($1 \leq i \leq n$), sao cho:
$1^\circ$ các hệ thức $t_i > 0$ ($1 \leq i \leq n$) kéo theo $\varphi(t_1, t_2, \ldots, t_n) > 0$;
$2^\circ$ hàm $\varphi$ là thuần nhất dương;
$3^\circ$ tập hợp $K \subset \mathbf{R}^n$ được xác định bởi các hệ thức $t_i \geq 0$ ($1 \leq i \leq n$), $\varphi(t_1, t_2, \ldots, t_n) \geq 1$ là lồi.
Trong các điều kiện đó, nếu $f_1, f_2, \ldots, f_n$ là $n$ hàm hữu hạn $\geq 0$ xác định trên $X$, sao cho $M(f_i) < +\infty$ với $1 \leq i \leq n$, thì

$$
M(\varphi(f_1, f_2, \ldots, f_n)) \leq \varphi(M(f_1), M(f_2), \ldots, M(f_n)).
$$

Ta biết, nhờ định lý Hahn-Banach (TVS, II, §5), rằng $K$ là giao của $n$ nửa không gian $t_i \geq 0$ ($1 \leq i \leq n$) và một họ các nửa không gian đóng $(U_\iota)_{\iota \in I}$, trong đó $U_\iota$ được xác định bởi một quan hệ có dạng

$$
\alpha_{\iota 1} t_1 + \alpha_{\iota 2} t_2 + \cdots + \alpha_{\iota n} t_n - \beta_\iota \geq 0,
$$

trong đó các $\alpha_{\iota k}$ không đồng thời bằng không. Theo giả thiết, nếu $t = (t_i)$ sao cho $t_i > 0$ với $1 \leq i \leq n$, thì $\varphi(t_1, \ldots, t_n) > 0$, do đó tồn tại một $\lambda_0 > 0$ sao cho quan hệ $\lambda \geq \lambda_0$ kéo theo $\lambda t \in K$; điều này cho thấy rằng, với mỗi $\iota \in I$, các quan hệ $t_i \geq 0$ ($1 \leq i \leq n$) kéo theo $\alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \geq 0$ và vì thế $\alpha_{\iota k} \geq 0$ với $1 \leq k \leq n$; khi đó hiển nhiên là $K$ cũng là giao của các nửa không gian $t_i \geq 0$ ($1 \leq i \leq n$) và các $U_\iota$ sao cho $\beta_\iota \geq 0$; hơn nữa, vì gốc tọa độ không thuộc $K$, nên tồn tại ít nhất một chỉ số $\iota$ sao cho $\beta_\iota > 0$.

Bây giờ gọi $C$ là nón lồi trong $\mathbf{R}^{n+1}$ được xác định bởi các hệ thức $t_i \geq 0$ ($1 \leq i \leq n+1$), $t_{n+1} \leq \varphi(t_1, t_2, \ldots, t_n)$ (bao đóng của nón lồi sinh trong $\mathbf{R}^{n+1}$ bởi tập hợp lồi $K \times \{1\}$); ngay lập tức thấy rằng $C$ cũng được xác định bởi các hệ thức $t_i \geq 0$ ($1 \leq i \leq n+1$) và

$$
\beta_\iota t_{n+1} \leq \alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \quad (\iota \in I, \ \beta_\iota \geq 0).
$$

Do đó, với mọi $x \in X$, ta có

$$
\beta_\iota \varphi(f_1(x), \ldots, f_n(x)) \leq \alpha_{\iota 1} f_1(x) + \cdots + \alpha_{\iota n} f_n(x)
$$

với mọi $\iota \in I$. Với mọi chỉ số $\iota$ sao cho $\beta_\iota > 0$, suy ra từ (4) và các giả thiết về $M$ rằng $M(\varphi(f_1, f_2, \ldots, f_n))$ là hữu hạn và

$$
\beta_\iota M(\varphi(f_1, f_2, \ldots, f_n)) \leq \alpha_{\iota 1} M(f_1) + \alpha_{\iota 2} M(f_2) + \cdots + \alpha_{\iota n} M(f_n),
$$

và quan hệ này cũng được kiểm tra một cách hiển nhiên nếu $\beta_\iota = 0$. Do đó ta thấy rằng điểm có các tọa độ

$$
M(f_1), M(f_2), \ldots, M(f_n), \quad M(\varphi(f_1, f_2, \ldots, f_n))
$$

thuộc $C$, điều này chứng minh mệnh đề.

2. The inequalities of Hölder and Minkowski

Trong số này và số tiếp theo, $X$ và $P$ có cùng nghĩa như trong No. 1, và $M$ ký hiệu một hàm xác định trên $P$ thỏa mãn các điều kiện được liệt kê trong No. 1.

MỆNH ĐỀ 2. — *Cho $\alpha$ và $\beta$ là hai số sao cho $0 < \alpha < 1$, $0 < \beta < 1$, $\alpha + \beta = 1$. Nếu $f$ và $g$ là hai hàm hữu hạn $\geq 0$ xác định trên $X$, và nếu $M(f)$ và $M(g)$ là hữu hạn, thì*

$$
M(f^\alpha g^\beta) \leq (M(f))^\alpha (M(g))^\beta
$$

(*bất đẳng thức Hölder*).

Theo Mệnh đề 1, tất cả quy về việc chứng minh rằng, trong $\mathbf{R}^2$, tập hợp được xác định bởi các quan hệ $t_1 \geq 0$, $t_2 \geq 0$, $t_1^\alpha t_2^\beta \geq 1$ là lồi, hay cũng vậy (FRV, I, §4, No. 1, Định nghĩa 1) rằng hàm $u(t) = t^{-\alpha/\beta}$ là lồi với $0 < t < +\infty$. Bây giờ, đặt $r = \alpha/\beta$, ta có $D^2 u(t) = r(r+1)t^{-r-2}$ và, vì $r > 0$, $D^2 u(t) > 0$ trên $]0, +\infty[$, điều này chứng minh mệnh đề (FRV, I, §4, No. 4, Hệ quả của Mệnh đề 8).

HỆ QUẢ. — *Cho $\alpha_i$ ($1 \leq i \leq n$) là $n$ số $\geq 0$ sao cho*
$$
\sum_{i=1}^n \alpha_i = 1,
$$
*và cho $f_i$ ($1 \leq i \leq n$) là $n$ hàm số $\geq 0$ xác định trên $X$, sao cho $M(f_i)$ là hữu hạn với $1 \leq i \leq n$. Trong các điều kiện ấy,*

$$
M(f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}) \leq (M(f_1))^{\alpha_1} (M(f_2))^{\alpha_2} \cdots (M(f_n))^{\alpha_n}.
$$

Ta có thể chỉ xét trường hợp $\alpha_i > 0$ với mọi $i$. Chỉ cần lập luận bằng quy nạp theo $n$, bằng cách áp dụng bất đẳng thức (5) cho các số $\alpha = \alpha_1$ và $\beta = \sum_{i=2}^n \alpha_i$, và cho các hàm $f = f_1$, $g = (f_2^{\alpha_2} f_3^{\alpha_3} \cdots f_n^{\alpha_n})^{1/\beta}$.

MỆNH ĐỀ 3. — *Cho $p$ là một số thực $\geq 1$. Nếu $f$ và $g$ là hai hàm hữu hạn $\geq 0$ xác định trên $X$, thì*

$$
\left( M((f+g)^p) \right)^{1/p} \leq \left( M(f^p) \right)^{1/p} + \left( M(g^p) \right)^{1/p}
$$

(*bất đẳng thức Minkowski*).

Ta có thể chỉ xét trường hợp $M(f^p)$ và $M(g^p)$ là hữu hạn. Theo Mệnh đề 1, ta được quy về việc chứng minh rằng tập hợp trong $\mathbf{R}^2$ được xác định bởi các quan hệ $t_1 \geq 0,\ t_2 \geq 0,\ t_1^{1/p} + t_2^{1/p} \geq 1$ là lồi, hay cũng chính là hàm $u(t) = (1 - t^{1/p})^p$ là lồi với $0 \leq t \leq 1$. Thật vậy,

$$
D^2 u(t) = \left(1 - \frac{1}{p}\right)t^{1/p-2}(1-t^{1/p})^{p-2} \geq 0
$$

với $0 < t \leq 1$, do đó suy ra mệnh đề.

### 3. Các nửa chuẩn $N_p$

Cho $p$ là một số thực $\geq 1$ và gọi $\mathcal{F}^p(X, M)$ là tập hợp các hàm số hữu hạn $f$ xác định trên $X$ sao cho $M(|f|^p)$ là *hữu hạn*. Hiển nhiên là nếu $g$ là một hàm thuộc $\mathcal{F}^p(X, M)$ và nếu $|f| \leq |g|$, thì $f$ cũng thuộc $\mathcal{F}^p(X, M)$; nhận xét này và bất đẳng thức Minkowski cho thấy tổng của hai hàm trong $\mathcal{F}^p(X, M)$ cũng thuộc tập hợp này; có tính đến việc $M$ là thuần nhất dương, do đó ta thấy rằng $\mathcal{F}^p(X, M)$ là một *không gian con tuyến tính* của không gian $\mathbf{R}^X$ gồm mọi hàm số hữu hạn xác định trên $X$.

Với mọi số $p > 0$ và mọi hàm số hữu hạn $f$ xác định trên $X$, đặt

$$
N_p(f) = \left(M(|f|^p)\right)^{1/p};
$$

khi đó $N_p(\lambda f) = |\lambda| N_p(f)$ với mọi vô hướng $\lambda$; hơn nữa, nếu $p \geq 1$ thì, theo (7),

$$
N_p(f+g) \leq N_p(f) + N_p(g),
$$

điều đó chứng tỏ rằng $N_p$ là một *nửa chuẩn* trên không gian vectơ $\mathcal{F}^p(X, M)$ (TVS, II, §1).

**Mệnh đề 4.** — *Cho $p$ và $q$ là hai số thực $> 0$ và đặt $1/r = 1/p + 1/q$. Với mọi hàm số hữu hạn $f, g$ xác định trên $X$,*

$$
N_r(fg) \leq N_p(f) N_q(g)
$$

*miễn là $N_p(f)$ và $N_q(g)$ là hữu hạn.*

Thật vậy, quan hệ (9) có thể được viết thành

$$
M(|f|^r |g|^r) \leq (M(|f|^p))^{r/p} (M(|g|^q))^{r/q},
$$

đó không là gì khác ngoài bất đẳng thức Hölder (5) áp dụng cho các số $\alpha = r/p$ và $\beta = r/q$ và cho các hàm số $|f|^p$ và $|g|^q$.

HỆ QUẢ. — *Giả sử rằng* $M(1) = 1$; *khi đó, đối với mọi hàm số hữu hạn* $f$ *xác định trên* $X$, *ánh xạ* $p \mapsto N_p(f)$ *là tăng trên* $]0, +\infty[$.

Áp dụng bất đẳng thức (9) cho trường hợp $g = 1$, ta thấy rằng $N_r(f) \leq N_p(f)$ với mọi $q > 0$; vì số $r$ được xác định bởi $1/r = 1/p + 1/q$ chạy qua tập hợp các số sao cho $0 < r < p$ khi $q$ chạy qua tập hợp các số $> 0$, hệ quả được chứng minh.

MỆNH ĐỀ 5. — *Với mọi hàm số hữu hạn* $f$ *xác định trên* $X$, *tập hợp* $I$ *các giá trị của* $1/p$ ($p > 0$) *sao cho* $N_p(f)$ *hữu hạn hoặc là rỗng hoặc là một khoảng; nếu* $I$ *không quy về một điểm, thì ánh xạ* $\alpha \mapsto \log N_{1/\alpha}(f)$ *hoặc lồi trên* $I$ *hoặc bằng* $-\infty$ *trên phần trong của* $I$.

Cho $r$ và $s$ là hai số phân biệt $> 0$ sao cho $1/r$ và $1/s$ thuộc $I$; tất cả quy về việc chứng minh rằng nếu

$$
\frac{1}{p} = \frac{t}{r} + \frac{1-t}{s},
$$

với $0 < t < 1$, thì

$$
\log N_p(f) \leq t \cdot \log N_r(f) + (1-t) \log N_s(f),
$$

hay, cũng tương đương như vậy,

$$
N_p(f) \leq (N_r(f))^t (N_s(f))^{1-t},
$$

một quan hệ mà theo định nghĩa của $N_p$ có thể viết thành

$$
M(|f|^p) \leq (M(|f|^r))^{tp/r} (M(|f|^s))^{(1-t)p/s}.
$$

Đặt $\alpha = tp/r$, ta có $1-\alpha = (1-t)p/s$ theo quan hệ xác định $p$ như một hàm của $t, r, s$; do đó $p = \alpha r + (1-\alpha)s$. Bất đẳng thức Hölder khi đó cho

$$
M(|f|^{r\alpha}|f|^{s(1-\alpha)}) \leq (M(|f|^r))^{\alpha} (M(|f|^s))^{1-\alpha},
$$

mà chính là bất đẳng thức (12).

Bài tập

1) Với các giả thiết của No. 1, hãy chứng minh rằng tập hợp các hàm bị chặn trên X sao cho $M(|f|)$ là hữu hạn là một đại số con A của $\mathbf{R}^X$, và tập hợp các hàm bị chặn trên X sao cho $M(|f|) = 0$ là một iđêan trong A. Nếu, hơn nữa, $M(1)$ là hữu hạn, hãy chứng minh rằng ánh xạ $f \mapsto M(f)$ là liên tục khi A được trang bị tôpô của sự hội tụ đều trên X.

2) Cho X là khoảng $[0, +\infty[$ của $\mathbf{R}$, S là nón lồi tạo bởi các hàm xác định trên X sao cho $0 \leq f(x) \leq kx$ trên X (đối với một số hữu hạn $k > 0$ phụ thuộc vào $f$). Đặt $M(f) = 0$ với $f \in S$, và $M(f) = +\infty$ với mọi hàm dương $f$ xác định trên X và không thuộc S. Hãy chỉ ra rằng $M$ thỏa mãn các điều kiện của No. 1, và rằng $M(x) = 0$, và $M(x^r) = +\infty$ với mọi số $r > 0$ khác 1.

3) Cho một ví dụ trong đó X là một tập hợp có hai phần tử, $N_p(\mathbf{x})$ là hữu hạn với mọi $p > 0$ và mọi $\mathbf{x} \in \mathbf{R}^2$, nhưng tồn tại những giá trị của $p$ sao cho ánh xạ $p \mapsto N_p(\mathbf{x})$ không khả vi tại các điểm đó.

4) Suy ra bất đẳng thức (6) từ bất đẳng thức của trung bình nhân

$$
z_1^{\alpha_1} z_2^{\alpha_2} \cdots z_n^{\alpha_n} \leq \alpha_1 z_1 + \cdots + \alpha_n z_n \quad \text{(với } \sum_{i=1}^n \alpha_i = 1 \text{)}
$$

(FRV, III, §1, No. 1, Prop. 2). (Rút gọn về trường hợp $M(f_i) = 1$ với $1 \leq i \leq n$.)

5) Cho $\alpha$ là một số thực $> 1$ và đặt $\beta = 1 - \alpha < 0$. Cho $g$ là một hàm hữu hạn, xác định trên X, sao cho $g(x) > 0$ với mọi $x \in X$ và sao cho $M(g) > 0$; hãy chứng minh rằng với mọi hàm hữu hạn $f \geq 0$ xác định trên X sao cho $M(f)$ là hữu hạn,

$$
M(f^\alpha g^\beta) \geq (M(f))^\alpha (M(g))^\beta
$$

(hãy áp dụng bất đẳng thức Hölder một cách thích hợp).

6) Suy ra bất đẳng thức Minkowski từ bất đẳng thức Hölder (hãy tìm một cận trên của $M((f+g)^{p-1})$ với sự trợ giúp của bất đẳng thức Hölder). Nếu giả thiết rằng $M(f+g) = M(f) + M(g)$ với mọi cặp hàm $f, g$ xác định và $\geq 0$ trên $X$, cũng vậy hãy suy ra từ Bài tập 5 bất đẳng thức

$$
(M((f+g)^p))^{1/p} \geq (M(f^p))^{1/p} + (M(g^p))^{1/p}
$$

trong các trường hợp sau:

a) $0 < p < 1$, $f$ và $g$ là các hàm hữu hạn $\geq 0$ xác định trên $X$, sao cho $f(x) + g(x) > 0$ với mọi $x \in X$ và sao cho $M(f^p)$ và $M(g^p)$ là hữu hạn;

b) $p < 0$, $f$ và $g$ là các hàm hữu hạn xác định trên $X$, sao cho $f(x) > 0$ và $g(x) > 0$ với mọi $x \in X$, $M(f^p)$ và $M(g^p)$ là hữu hạn, và $M((f+g)^p) > 0$.
