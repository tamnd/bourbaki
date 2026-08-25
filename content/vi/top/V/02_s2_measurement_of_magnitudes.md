---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 2
section_title: Measurement of magnitudes
lang: vi
source: top-v-x
pdf_pages: 0018-0023, 0031-0031
extraction: ocr
statements: 5
exercises: 2
content_sha256: a086dd4dc7a5ff21d42133d5c8f51c9f647cae8e2a5a438c391dd08588dd18e4
translated_from: content/en/top/V/02_s2_measurement_of_magnitudes.md
source_content_sha256: f069c591d5864c6d5318ca3b67c20ab746c5526dd0f4324b46149dcbc086d510
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-66c878af
glossary_version: 34
glossary_terms_sha256: 325ed56f45d6f29c30307de75a29e7278fdef6f30c094e7493eb7ec0ba61ccde
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. ĐO LƯỜNG CÁC ĐẠI LƯỢNG

Chúng ta đã thấy (xem ghi chú lịch sử cho Chương IV) rằng bài toán đo các đại lượng là nguồn gốc của khái niệm số thực; chính xác hơn, các kiểu đại lượng khác nhau mà người ta dần dần nghiên cứu, vì những mục đích thực tiễn hoặc lý thuyết, thoạt đầu được xem xét tách biệt với nhau, và khả năng đo mọi kiểu đại lượng bằng cùng một hệ số đã xuất hiện như một sự kiện thực nghiệm từ lâu trước khi người Hy Lạp nảy ra ý tưởng táo bạo về việc đưa ra một chứng minh chặt chẽ. Trong lý thuyết tiên đề mà họ xây dựng, khái niệm đại lượng liên quan đến một luật hợp thành ("phép cộng" các đại lượng cùng kiểu) và một quan hệ thứ tự (quan hệ "A nhỏ hơn B", được gọi là quan hệ so sánh các đại lượng). Trong phần sau, chúng ta sẽ xét cùng bài toán đó, nghĩa là chúng ta sẽ khảo sát các điều kiện phải đặt lên một luật hợp thành nội và một quan hệ thứ tự trên một tập hợp E để nó đẳng cấu với một tập con E' của R, được trang bị cấu trúc cảm sinh bởi phép cộng và quan hệ $\leq$ trong R. Vì chúng ta sẽ không giả thiết tiên nghiệm rằng luật hợp thành đã cho trên E là giao hoán, nên chúng ta sẽ dùng ký hiệu nhân; nhưng ngoài điều này ra, chúng ta hầu như không rời khỏi các lập luận cổ điển.

Cho E là một tập hợp được sắp thứ tự tuyến tính bởi một quan hệ thứ tự viết là $x \leq y$, và giả sử E có một phần tử nhỏ nhất $\omega$. Cho I là một tập con của E sao cho $\omega \in I$, và sao cho các quan hệ $x \in I$ và $y \leq x$ kéo theo $y \in I$; giả sử thêm rằng ta được cho một luật hợp thành $(x, y) \to xy$ trên E, với tích $xy$ được xác định cho mọi cặp phần tử của I ($xy$ thuộc E, nhưng không nhất thiết thuộc I). Hơn nữa, ta đưa ra các giả thiết sau:

(GR_I) $\omega$ là phần tử đơn vị [$\omega x = x \omega = x$ với mọi $x \in I$] và luật hợp thành là kết hợp [theo nghĩa sau: với mọi $x \in I, y \in I, z \in I, xy \in I$ và $yz \in I$, ta có $x(yz) = (xy)z$].

(GR_{II}) Quan hệ $x < y$ giữa các phần tử của I kéo theo, với mọi $z \in I$, các quan hệ $xz < yz$ và $zx < zy$.

(GR_{III}) Tập các phần tử $> \omega$ trong I không rỗng và không có phần tử nhỏ nhất; và với mọi phần tử $x, y$ của I sao cho $x < y$, tồn tại $z > \omega$ sao cho $xz \leq y$.

Điều kiện (GR_{II}) kéo theo rằng các bất đẳng thức giữa các phần tử của I có thể được nhân từng vế: $x < y$ và $x' < y'$ kéo theo $xx' < yy'$ (vì $xx' < yx'$ và $yx' < yy'$). Cụ thể, ta có $y < yx$ với mọi $x > \omega$ ($x \in I, y \in I$).

Cho một dãy hữu hạn $(x_i)_{1 \leq i \leq p}$ gồm các phần tử của I, ta có thể định nghĩa bằng quy nạp theo $p$ tích của dãy này $\prod_{i=1}^p x_i$ là bằng $\left( \prod_{i=1}^{p-1} x_i \right) x_p$, với điều kiện tích $\prod_{i=1}^{p-1} x_i$ được định nghĩa và thuộc I: do đó, nếu $\prod_{i=1}^p x_i$ được định nghĩa, thì mỗi tích $\prod_{i=1}^q x_i$ đều được định nghĩa và thuộc I, với $2 \leq q \leq p - 1$. Cho tất cả các $x_i$ bằng cùng một phần tử $x \in I$, ta thấy đặc biệt rằng nếu $x^p$ được định nghĩa, thì $x^q$ được định nghĩa và thuộc I với $2 \leq q \leq p - 1$. Theo quy ước, ta định nghĩa $x^0$ bằng $\omega$, với mọi $x \in I$. Theo (GR$_\text{II}$), nếu $x > \omega$, ta có $\omega < x^q < x^p$ với $1 \leq q \leq p - 1$ nếu $x^p$ được định nghĩa; nếu $x < y$ và $y^p$ được định nghĩa, thì ta thấy (bằng quy nạp theo $p$) rằng $x^p$ được định nghĩa và $x^p < y^p$. Mặt khác, điều kiện tính kết hợp (GR$_\text{I}$) suy ra bằng quy nạp theo $n$ rằng, nếu $x^{m+n}$ được định nghĩa, thì $x^m x^n$ cũng được định nghĩa, và $x^{m+n} = x^m x^n$. Ngược lại, theo (GR$_\text{I}$) và (GR$_\text{II}$), nếu $x^m x^n$ được định nghĩa và thuộc I, thì $x^{m+n}$ được định nghĩa và ta có $x^{m+n} = x^m x^n$; điều này lại được chứng minh bằng quy nạp theo $n$, vì ta có $x^{n-1} \leq x^n$, do đó $x^m x^{n-1}$ được định nghĩa và thuộc I; theo giả thiết, $x^m x^{n-1} = x^{m+n-1} \in I$, suy ra $(x^{m+n-1})x = x^{m+n}$ được định nghĩa và bằng $x^m x^n$ theo kết quả trước. Tương tự, bằng quy nạp theo $n$, ta chứng minh rằng, nếu $x^{mn}$ được định nghĩa, thì $(x^m)^n$ được định nghĩa và $x^{mn} = (x^m)^n$; và ngược lại, nếu $(x^m)^n$ được định nghĩa và thuộc I, thì $x^{mn}$ được định nghĩa và bằng $(x^m)^n$.

Cuối cùng, tiên đề (GR$_\text{III}$) kéo theo rằng, với mọi $x \in I$ sao cho $x > \omega$, tồn tại $y > \omega$ sao cho $y^2 \leq x$. Thật vậy, nếu $x > \omega$ thì tồn tại $z > \omega$ sao cho $z < x$, và khi đó $t > \omega$ sao cho $zt \leq x$; lấy $y$ là phần tử nhỏ hơn trong hai phần tử $z, t$. Bằng quy nạp theo $n$, ta suy ra rằng tồn tại $u > \omega$ sao cho $u^{2^n} \leq x$.

Bây giờ ta đưa vào giả thiết sau:

(GR$_\text{IV}$) ("Tiên đề Archimedes"). *Với mọi* $x \in I$ *và* $y \in I$ *sao cho* $x > \omega$, *tồn tại một số nguyên* $n > 0$ *sao cho* $x^n$ *được xác định và* $x^n > y$.

Nếu ta lấy E là một tập hợp các số thực $\geq 0$ chứa 0 và các số $> 0$ nhỏ tùy ý, I là giao của E với một khoảng của R có 0 là điểm đầu mút bên trái và chứa ít nhất một số khác, luật hợp thành là phép cộng các phần tử của I, và nếu ta giả thiết rằng $x + y \in E$ mỗi khi $x \in I$ và $y \in I$ thì rõ ràng các tiên đề (GR$_\text{I}$), (GR$_\text{II}$), (GR$_\text{III}$) và (GR$_\text{IV}$) được thỏa mãn (*).

(*) Trong các tập hợp "độ lớn" xuất hiện trong các khoa học thực nghiệm, các tiên đề (GR$_\text{I}$) và (GR$_\text{II}$) nói chung có khả năng được kiểm chứng bằng thực nghiệm, ít nhất là một cách xấp xỉ. Mặt khác, tiên đề (GR$_\text{III}$), tiên đề đặt ra sự tồn tại của các độ lớn "nhỏ tùy ý", rõ ràng không thể được thiết lập theo cùng cách; nó là một giả thiết thuần túy *a priori*. Đối với tiên đề (GR$_\text{IV}$), nó có thể được xem như một "ngoại suy" của một sự kiện có thể được kiểm chứng bằng thực nghiệm đối với các độ lớn không "quá nhỏ".

Ngược lại:

#### Mệnh đề 1 {#top-v-s2-prop-1 .statement}

Cho E là một tập hợp có thứ tự tuyến tính với một phần tử nhỏ nhất ω; cho I là một tập con của E sao cho ω ∈ I và sao cho các quan hệ x ∈ I, y ≤ x kéo theo y ∈ I; cho (x, y) → xy là một luật hợp thành trên E, được xác định với x ∈ I và y ∈ I. Khi đó, nếu các tiên đề (GR_I), (GR_{II}), (GR_{III}) và (GR_{IV}) được thỏa mãn, tồn tại một ánh xạ tăng ngặt f từ I vào tập hợp R_+ các số thực ≥ 0, sao cho

$$
f(xy) = f(x) + f(y)
$$

mỗi khi x ∈ I, y ∈ I và xy ∈ I; hơn nữa, giao của f(I) với mọi khoảng [0, f(b)] của R là trù mật trong khoảng này, trong đó b chỉ một phần tử bất kỳ của I.

Với hai phần tử bất kỳ x, y của I sao cho y ≠ ω, ta ký hiệu (x : y) là số nguyên lớn nhất n ≥ 0 sao cho y^n được xác định và ≤ x (*); số nguyên này tồn tại theo (GR_{IV}); nếu (x : y) = p, thì y^{p+1} được xác định và > x. Nếu x ∈ I, y ∈ I và xy ∈ I, ta có

(I)
$$
(x : z) + (y : z) \leq (xy : z) \leq (x : z) + (y : z) + 1.
$$

Thật vậy, cho (x : z) = p, (y : z) = q; khi đó ta có z^p ≤ x, z^q ≤ y; vì xy ∈ I, z^p z^q được xác định và thuộc I, do đó z^{p+q} được xác định và z^{p+q} = z^p z^q ≤ xy; hơn nữa, nếu z^{p+q+2} được xác định, ta có z^{p+q+2} > xy vì z^{p+1} > x và z^{q+1} > y.

Tiếp theo ta thiết lập các bất đẳng thức

(2)
$$
\begin{cases}
(x : y) (y : z) \leq (x : z), \\
((x : y) + 1) ((y : z) + 1) \geq (x : z) + 1.
\end{cases}
$$

Cho (x : y) = p và (y : z) = q; khi đó y^p ≤ x và z^q ≤ y, do đó (z^q)^p được xác định và ≤ x; vì vậy nó thuộc I; do đó z^{pq} được xác định và ta có z^{pq} = (z^q)^p ≤ x, từ đó suy ra bất đẳng thức thứ nhất. Mặt khác, nếu z^{(p+1)(q+1)} được xác định, ta có z^{(p+1)(q+1)} > x, vì y^{p+1} > x và z^{q+1} > y; do đó có bất đẳng thức thứ hai.

Gọi $\tilde{\mathcal{X}}$ là lọc các đoạn của tập hợp có thứ tự gồm các phần tử > ω trong I, đối với quan hệ ≥; các khoảng ]ω, z[, trong đó z chạy qua tập hợp tất cả các phần tử > ω, tạo thành một cơ sở của $\tilde{\mathcal{X}}$. Cho hai phần tử a và x của I sao cho a > ω, ta sẽ chỉ ra rằng tỉ số $\frac{(x : z)}{(a : z)}$, được xác định với z ≤ a và là một số hữu tỉ > 0,

(*) Khi E = I là tập hợp các số nguyên tự nhiên, luật hợp thành là phép cộng, (x : y) là phần nguyên của x/y.

là một hàm của $z$ có một *giới hạn* đối với $\mathfrak{F}$. Điều này là hiển nhiên nếu $x = \omega$, vì khi đó $(x : z) = 0$ với mọi $z$. Nếu $x > \omega$, ta sẽ chứng minh rằng ảnh $\mathcal{G}$ của $\mathfrak{F}$ qua ánh xạ $z \to \frac{(x : z)}{(a : z)}$ (hạn chế vào tập hợp các $z > \omega$ sao cho $\leq x$ và $\leq a$) là một cơ sở lọc Cauchy cho cấu trúc đều của nhóm *nhân* $\mathbf{R}_+^*$, và do đó hội tụ đến một số thực $> 0$. Trước hết chú ý rằng, cho $u > \omega$, $(u : z)$ có giới hạn $+\infty$ đối với $\mathfrak{F}$: vì tồn tại $z > \omega$ sao cho $z^{2^n} \leq u$, do đó $(u : z) \geq 2^n > n$. Bây giờ lấy tùy ý một số $\varepsilon > 0$; tồn tại $t > \omega$ sao cho $(x : t) \geq 1 / \varepsilon$ và $(a : t) \geq 1 / \varepsilon$. Xét bất đẳng thức kép

$$
\frac{(x : t)}{(a : t) + 1} \cdot \frac{(t : z)}{(t : z) + 1} \leq \frac{(x : z)}{(a : z)} \leq \frac{(x : t) + 1}{(a : t)} \cdot \frac{(t : z) + 1}{(t : z)},
$$

suy ra ngay lập tức từ các bất đẳng thức (2). Tồn tại $z_0 > \omega$ sao cho $z \leq z_0$ kéo theo $(t : z) \geq 1 / \varepsilon$, do đó

$$
\frac{1}{(1 + \varepsilon)^2} \frac{(x : t)}{(a : t)} \leq \frac{(x : z)}{(a : z)} \leq (1 + \varepsilon)^2 \frac{(x : t)}{(a : t)},
$$

điều này chứng tỏ rằng $\mathcal{G}$ là một cơ sở lọc Cauchy cho cấu trúc đều nhân.

Cố định một lần và mãi mãi phần tử $a > \omega$ ("đơn vị đo") và với mỗi $x \in I$ đặt

$$
f(x) = \lim_{z \in \mathfrak{F}} \frac{(x : z)}{(a : z)}.
$$

Từ những gì đã được chứng minh, ta có $f(\omega) = 0$, $f(x) > 0$ với $x > \omega$, và $f(a) = 1$. Nếu ta chia bất đẳng thức (1) cho $(a : z)$ và chuyển qua giới hạn đối với $\mathfrak{F}$, ta thấy rằng

$$
f(xy) = f(x) + f(y)
$$

với mọi $x \in I, y \in I$ và $xy \in I$. Tương tự, quan hệ $x \leq y$ kéo theo $(x : z) \leq (y : z)$, do đó bằng cách chia cho $(a : z)$ và chuyển qua giới hạn ta có $f(x) \leq f(y)$, nên $f$ là *tăng* trên $I$. Ta suy ra rằng $f$ là *tăng ngặt* trên $I$; vì nếu $x < y$, tồn tại $z > \omega$ sao cho $xz \leq y$, do đó $f(xz) \leq f(y)$; và vì $xz \in I$,

$$
f(x) + f(z) = f(xz) \leq f(y);
$$

nhưng $f(z) > 0$, do đó thực sự $f(x) < f(y)$.

Cuối cùng, nếu $b \in I$, giao của $f(I)$ và khoảng $[0, f(b)]$ của $\mathbf{R}$ là trù mật trong khoảng này. Thật vậy, nếu $n$ là một số nguyên bất kỳ $> 0$, tồn tại $x > \omega$ sao cho $f(x) \leq 2^{-n}$ (lấy $x$ sao cho $x^{2^n} \leq a$); nếu $p$ là số nguyên nhỏ nhất sao cho $x^{p+1} > b$, ta có $(p+1)f(x) > f(b)$ và $qf(x) \leq f(b)$ với $1 \leq q \leq p$; do đó mọi khoảng được chứa trong $[0, f(b)]$ và có độ dài $> 2^{-n}$ chứa ít nhất một điểm có dạng $qf(x) = f(x^q) \in f(I)$. Chứng minh của Mệnh đề 1 do đó hoàn tất.

#### Nhận xét 1 {#top-v-s2-rem-1 .statement}

Các hệ thức $x \in I, y \in I, xy \in I, yx \in I$ kéo theo
$$
f(xy) = f(x) + f(y) = f(yx),
$$
và do đó $yx = xy$ vì $f$ là tăng ngặt; nói cách khác, luật cảm sinh bởi luật hợp thành của $E$ trên một khoảng $[0, b]$ được chọn thích hợp (chẳng hạn, sao cho $b^2 \leq a$) là *giao hoán*.

#### Nhận xét 2 {#top-v-s2-rem-2 .statement}

Mọi ánh xạ $g$ của $I$ vào $\mathbf{R}_+$ thỏa mãn cùng các điều kiện như $f$ đều có dạng $x \to \lambda f(x)$ trong đó $\lambda > 0$. Thật vậy, nếu $\lambda = g(a) > 0$, các hệ thức $z^p \leq x \leq z^{p+1}, z^q \leq a \leq z^{q+1}$ kéo theo, theo giả thiết,
$$
pg(z) \leq g(x) \leq (p+1)g(z), \qquad qg(z) \leq g(a) \leq (q+1)g(z),
$$
do đó
$$
\lambda \frac{(x : z)}{(q : z) + 1} \leq g(x) \leq \lambda \frac{(x : z) + 1}{(q : z)},
$$
và do đó, chuyển qua giới hạn đối với $\tilde{x}$, ta có $g(x) = \lambda f(x)$.

Ta hãy tìm các điều kiện dưới đó $f(I)$ là một *khoảng* của $\mathbf{R}_+$. Rõ ràng hai điều kiện sau đây là cần thiết:

(GR_{IIIa}) *Tập hợp các phần tử $> \omega$ trong $I$ là không rỗng và không có phần tử nhỏ nhất, và với mọi hai phần tử $x, y$ của $I$ sao cho $x < y$, tồn tại $z \in I$ sao cho $xz = y$* ("phép trừ" các đại lượng).

(GR_{IVa}) *Mọi dãy tăng các phần tử của $I$, được chặn trên bởi một phần tử của $I$ đều có một cận trên nhỏ nhất trong $I$*.

Ta sẽ chỉ ra rằng các điều kiện này cũng đủ, và hơn nữa chúng cho phép ta loại bỏ tiên đề (GR_{IV}) (tiên đề Archimedes). Cụ thể hơn, ta sẽ chứng minh mệnh đề sau:

#### Mệnh đề 2 {#top-v-s2-prop-2 .statement}

*Nếu một tập hợp có thứ tự tuyến tính $E$ và một tập con $I$ của $E$ thỏa mãn các tiên đề (GR_I), (GR_{II}), (GR_{IIIa}) và (GR_{IVa}), thì tồn tại một ánh xạ tăng ngặt $f$ của $I$ lên một khoảng của $\mathbf{R}$, với $0$ là điểm đầu bên trái của nó, sao cho $f(\omega) = 0$ và $f(xy) = f(x) + f(y)$ bất cứ khi nào $x, y$ và $xy$ thuộc $I$.*

Trước hết ta chứng minh rằng tiên đề (GR_{IV}) được thỏa mãn. Ta lập luận bằng phản chứng: giả sử tồn tại $x, y \in I$ sao cho $x > \omega$, $x^n$ được xác định và $x^n \leq y$ với mọi số nguyên $n > 0$. Dãy tăng $(x^n)$ có một cận trên nhỏ nhất $b \in I$ theo (GR$_{\text{IV}_a}$). Vì $x < b$, tồn tại $c \in I$ sao cho $xc = b$ theo (GR$_{\text{III}_a}$), và ta có $c < b$ vì $x > \omega$. Bây giờ, với mọi $n$, ta có $x^{n+1} \leq b = xc$, do đó $x^n \leq c$ theo (GR$_{\text{II}}$) : cận trên $b$ của các $x^n$ do đó $\leq c$, đây là một mâu thuẫn.

Do đó chúng ta ở vào vị trí áp dụng Mệnh đề 1. Còn phải chứng minh rằng, nếu $\gamma = f(c)$ ($c > \omega$) là một phần tử bất kỳ của $f(I)$, và nếu $\beta$ là một số thực bất kỳ sao cho $0 < \beta < \gamma$, thì tồn tại $b \in I$ sao cho $f(b) = \beta$ (Chương IV, § 2, no. 4, Mệnh đề 1). Vì giao của $f(I)$ và $[0, \gamma]$ là trù mật trong $[0, \gamma]$, nên tồn tại một dãy tăng $(x_n)$ gồm các phần tử của $I$ sao cho $f(x_n)$ có $\beta$ làm giới hạn. Gọi $b$ là cận trên của dãy $(x_n)$ trong $I$; ta có $f(b) \geq f(x_n)$ với mọi $n$, do đó $f(b) \geq \beta$; nhưng $f(b) > \beta$ là không thể, bởi vì nếu không thì sẽ tồn tại $y \in I$ sao cho $\beta < f(y) < f(b)$, và vì $\beta$ là cận trên của dãy $(f(x_n))$, ta sẽ có $f(x_n) < f(y) < f(b)$ với mọi $n$, do đó $x_n < y < b$ với mọi $n$, điều này là vô lý. Vậy $f(b) = \beta$, và do đó Mệnh đề 2 được chứng minh.

#### Nhận xét {#top-v-s2-n0-rem-3 .statement}

Khi $I = E$, ảnh $f(I) = f(E)$ là toàn bộ $\mathbf{R}_+$, bởi vì nếu $b > \omega$, thì $b^n$ được xác định với mọi $n$, và do đó $n \cdot f(b)$ thuộc về $f(E)$ với mọi $n$; điều này suy ra rằng $f(E)$ không bị chặn trên, bởi vì $f(b) > 0$.

### Bài tập {#top-v-s2-exercises}

Xem các [bài tập của § 2](exercises/s2/).
