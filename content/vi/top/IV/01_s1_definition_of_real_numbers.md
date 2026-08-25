---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 1
section_title: Definition of real numbers
lang: vi
source: top-i-iv
pdf_pages: 0335-0340, 0384-0387
extraction: ocr
subsections:
    - "no": 1
      title: THE ORDERED GROUP OF RATIONAL NUMBERS
      page: 0
      pdf_page: 335
    - "no": 2
      title: THE RATIONAL LINE
      page: 0
      pdf_page: 336
    - "no": 3
      title: THE REAL LINE AND REAL NUMBERS
      page: 0
      pdf_page: 337
    - "no": 4
      title: PROPERTIES OF INTERVALS IN $\mathbf{R}$
      page: 0
      pdf_page: 338
    - "no": 5
      title: LENGTH OF AN INTERVAL
      page: 0
      pdf_page: 339
    - "no": 6
      title: ADDITIVE UNIFORMITY OF $\mathbf{R}$
      page: 0
      pdf_page: 340
statements: 10
exercises: 4
content_sha256: 16b315d18984e89283b27af103bc3c7c4c494faeaaec6f69d4af419e4cbd0fee
translated_from: content/en/top/IV/01_s1_definition_of_real_numbers.md
source_content_sha256: 3e464a20dbba1b7e5ca5492e42ca53c9282c0ce314d92b39f60176990dba0c1b
translation_model: gpt-5-6-mini
translation_run: translate-vi-b5f2ec1a
glossary_version: 34
glossary_terms_sha256: d7ea9d92bbdf5c18e82a53822a06340585efbcc1820528842476cb547a43cc44
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. ĐỊNH NGHĨA CÁC SỐ THỰC

### 1. NHÓM CÓ THỨ TỰ CỦA CÁC SỐ HỮU TỈ

Ta đã định nghĩa quan hệ thứ tự $x \leq y$ trên tập $\mathbf{Q}$ các số hữu tỉ; ta đã thấy rằng quan hệ thứ tự này làm cho $\mathbf{Q}$ là một tập *có thứ tự tuyến tính*, và nó *tương thích* với cấu trúc *nhóm cộng* của $\mathbf{Q}$, nghĩa là với mỗi $z \in \mathbf{Q}$ quan hệ $x \leq y$ tương đương với $x + z \leq y + z$ (tức là, *quan hệ thứ tự là bất biến qua các phép tịnh tiến*). Ta nhắc lại ký hiệu (được sử dụng trong mọi nhóm có thứ tự tuyến tính)

$$
x^+ = \sup (x, 0), \\
x^- = \sup (-x, 0) = (-x)^+, \\
|x| = \sup (x, -x);
$$

$|x|$ được gọi là *giá trị tuyệt đối* của $x$, và ta có

$$
x = x^+ - x^-, \qquad |x| = x^+ + x^-
$$

và *bất đẳng thức tam giác*

(1)
$$
|x + y| \leq |x| + |y|,
$$
cùng với bất đẳng thức
(2)
$$
||x| - |y|| \leq |x - y|
$$
là một hệ quả ngay lập tức của (1); hơn nữa
(3)
$$
|x^+ - y^+| \leq |x - y|.
$$

Các quan hệ $x \geq 0,\ x = x^+,\ x^- = 0,\ |x| = x$ (tương ứng. $x \leq 0,\ x = -x^-,\ x^+ = 0,\ |x| = -x$) là *tương đương*. Quan hệ $|x| = 0$ tương đương với $x = 0$; nếu $a \geq 0$, quan hệ $|x| \leq a$ tương đương với $-a \leq x \leq a$, và quan hệ $|x| \geq a$ tương đương với "$x \geq a$ hoặc $x \leq -a$". Với mọi $x, y$ trong $\mathbf{Q}$, ta có

(4)
$$
\sup (x, y) + z = \sup (x + z, y + z),
$$
(5)
$$
\inf (x, y) = - \sup (-x, -y),
$$

và, như các trường hợp riêng,

(6)
$$
\sup (x, y) = x + (y - x)^+ = x + (x - y)^-,
$$
(7)
$$
\inf (x, y) = x - (y - x)^- = x - (x - y)^+.
$$

Cuối cùng, gọi $\mathbf{Q}_+$ là tập hợp các số hữu tỉ $\geq 0$; khi đó ta có

(8)
$$
\mathbf{Q}_+ + \mathbf{Q}_+ \subset \mathbf{Q}_+,
$$
(9)
$$
\mathbf{Q}_+ \cap (- \mathbf{Q}_+) = \{ 0 \},
$$
(10)
$$
\mathbf{Q}_+ \cup (- \mathbf{Q}_+) = \mathbf{Q}.
$$

Quan hệ $x \leq y$ *tương đương* với $y - x \in \mathbf{Q}_+$.

Ta sẽ dùng quan hệ thứ tự này để định nghĩa *một tôpô trên $\mathbf{Q}$ tương thích với cấu trúc nhóm cộng của nó*.

### 2. ĐƯỜNG THẲNG HỮU TỈ

Xét tập $\mathfrak{F}$ gồm các *khoảng mở đối xứng* $]-a, +a[$, trong đó $a$ chạy qua tập các số hữu tỉ $> 0$; ta sẽ chứng minh rằng $\mathfrak{F}$ là một *hệ cơ bản các lân cận của* $0$ trong một tôpô tương thích với cấu trúc nhóm cộng của $\mathbf{Q}$.

Nhóm $\mathbf{Q}$ là giao hoán, và tiên đề $(\mathrm{GV}'_{\mathrm{II}})$ được thỏa mãn rõ ràng; do đó chỉ cần chứng minh rằng tiên đề $(\mathrm{GV}'_{\mathrm{I}})$ cũng được thỏa mãn, nói cách khác, với mỗi $a > 0$ tồn tại $b > 0$ sao cho các điều kiện $|x| < b$ và $|y| < b$ cùng kéo theo $|x + y| < a$. Bất đẳng thức tam giác cho thấy ta có thể lấy $b = a/2$.

#### Định nghĩa 1 {#top-iv-s1-def-1 .statement}

*Đường thẳng hữu tỉ là không gian tôpô gồm tập hợp $\mathbf{Q}$ cùng với tôpô nhóm cộng mà trong đó các khoảng mở đối xứng $]-a, +a[$ $(a > 0)$ tạo thành một hệ cơ bản các lân cận của $0$.*

*Nhóm tôpô $\mathbf{Q}$ được định nghĩa như vậy được gọi là nhóm cộng của đường thẳng hữu tỉ.*

Nếu $a$ là một số hữu tỉ $> 0$, thì tồn tại một số nguyên $n > 0$ sao cho $1/n < a$; do đó các khoảng mở $]-\frac{1}{n}, +\frac{1}{n}[$ $(n = 1, 2, \ldots)$ tạo thành một hệ cơ sở các lân cận của $0$ trên đường thẳng hữu tỉ.

Ta thu được một hệ cơ sở các lân cận của mọi điểm $x \in \mathbf{Q}$ bằng cách lấy các khoảng mở $]x - a, x + a[$, trong đó $a$ chạy qua tập hợp các số hữu tỉ $> 0$ (hoặc tập hợp các số $1/n$).

Định nghĩa 1 do đó tương đương với định nghĩa đã cho trong Chương I, § 1, no. 2.

Với mỗi cặp số hữu tỉ $(a, b)$ sao cho $a < b$, tồn tại $c \in \mathbf{Q}$ sao cho $a < c < b$ [chẳng hạn $c = (a + b)/2$]; suy ra đường thẳng hữu tỉ là một không gian Hausdorff không rời rạc.

Với mỗi $a > 0$, đặt $U_a$ là tập hợp các cặp $(x, y)$ thuộc $\mathbf{Q} \times \mathbf{Q}$ sao cho $|x - y| < a$. Khi $a$ chạy qua tập hợp các số hữu tỉ $> 0$ (hoặc chỉ tập hợp các số $1/n$), các tập hợp $U_a$ tạo thành một hệ cơ sở các lân cận của uniformity của nhóm cộng $\mathbf{Q}$ của đường thẳng hữu tỉ. Các quan hệ (2) và (3) cho thấy rằng $|x|, x^+$ và $x^-$ liên tục đều trên $\mathbf{Q}$. Suy ra các hàm $\sup(x, y)$ và $\inf(x, y)$ liên tục đều trên $\mathbf{Q} \times \mathbf{Q}$.

### 3. ĐƯỜNG THẲNG THỰC VÀ CÁC SỐ THỰC

#### Định nghĩa 2 {#top-iv-s1-def-2 .statement}

Gọi $\mathbf{R}$ là nhóm tôpô là hoàn thành của nhóm cộng $\mathbf{Q}$ của đường thẳng hữu tỉ. Các phần tử của $\mathbf{R}$ được gọi là các số thực; với tư cách là một không gian tôpô, $\mathbf{R}$ được gọi là đường thẳng thực; với tư cách là một nhóm tôpô, $\mathbf{R}$ được gọi là nhóm cộng của đường thẳng thực.

Ta luôn đồng nhất $\mathbf{Q}$ với nhóm con trù mật của $\mathbf{R}$ mà nó đẳng cấu chính tắc. Theo quy ước này, mọi số hữu tỉ đều là một số thực. Mọi số thực không hữu tỉ được gọi là số vô tỉ; ta đã thấy trong Chương II, § 3, no. 3 rằng các số như vậy tồn tại (ta sẽ chứng minh điều này theo một cách khác trong § 3, no. 3 của chương này; xem thêm Bài tập 2 của § 2); do đó (Chương III, § 2, no. 1) tập hợp $\mathbf{CQ}$ các số vô tỉ là trù mật trong $\mathbf{R}$.

Ta sẽ chứng minh rằng cấu trúc thứ tự của $\mathbf{Q}$ có thể mở rộng lên $\mathbf{R}$ sao cho thứ tự mở rộng vẫn tương thích với cấu trúc nhóm cộng của $\mathbf{R}$:

#### Mệnh đề 1 {#top-iv-s1-prop-1 .statement}

Quan hệ $y - x \in \overline{\mathbf{Q}}_+$ là một quan hệ thứ tự trên $\mathbf{R}$, biến $\mathbf{R}$ thành một tập hợp có thứ tự tuyến tính; tương thích với cấu trúc nhóm cộng trên $\mathbf{R}$, và cảm sinh thứ tự $x \leq y$ trên $\mathbf{Q}$.

Ta bắt đầu bằng cách chứng minh rằng các quan hệ $y - x \in \overline{\mathbf{Q}}_+$ và $z - y \in \overline{\mathbf{Q}}_+$ kéo theo $z - x \in \overline{\mathbf{Q}}_+$. Thật vậy, hàm $x + y$ liên tục trên $\mathbf{R} \times \mathbf{R}$, và do đó theo (8) ta có $\overline{\mathbf{Q}}_+ + \overline{\mathbf{Q}}_+ \subset \overline{\mathbf{Q}}_+$ (Chương I, § 2, no. 1, Định lý 1). Tiếp theo, ta sẽ chứng minh rằng các quan hệ $y - x \in \overline{\mathbf{Q}}_+$ và $x - y \in \overline{\mathbf{Q}}_+$ kéo theo $x = y$; điều này sẽ thiết lập rằng $y - x \in \overline{\mathbf{Q}}_+$ là một

Theo (10), ta có $\overline{\mathbf{Q}}_+ \cup (-\overline{\mathbf{Q}}_+) = \mathbf{R}$, và do đó $\mathbf{R}$ là *có thứ tự tuyến tính* bởi quan hệ thứ tự $y - x \in \overline{\mathbf{Q}}_+$.

Hơn nữa, vì các quan hệ $y - x \in \overline{\mathbf{Q}}_+$ và $(y + z) - (x + z) \in \overline{\mathbf{Q}}_+$ là tương đương, quan hệ thứ tự $y - x \in \overline{\mathbf{Q}}_+$ tương thích với cấu trúc nhóm cộng của $\mathbf{R}$.

Cuối cùng, nếu $x$ và $y$ thuộc $\mathbf{Q}$ thì các quan hệ $y - x \in \overline{\mathbf{Q}}_+$ và $y - x \in \mathbf{Q}_+$ là tương đương, và do đó quan hệ $y - x \in \overline{\mathbf{Q}}_+$ cảm sinh quan hệ $x \leq y$ trên $\mathbf{Q}$. Điều này hoàn tất chứng minh.

Quan hệ $y - x \in \overline{\mathbf{Q}}_+$ lại được ký hiệu là $x \leq y$. Tập hợp $\overline{\mathbf{Q}}_+$ là tập hợp tất cả các $x \geq 0$ trong $\mathbf{R}$ và được ký hiệu là $\mathbf{R}_+$; nó là một *tập hợp đóng*. Tập hợp tất cả các $x > 0$ được ký hiệu là $\mathbf{R}_+^*$; nó là phần bù của $-\mathbf{R}_+$ và do đó là *mở* trong $\mathbf{R}$.

### 4. CÁC TÍNH CHẤT CỦA CÁC KHOẢNG TRONG $\mathbf{R}$

#### Mệnh đề 2 {#top-iv-s1-prop-2 .statement}

*Mọi khoảng đóng (tương ứng, mở) trong $\mathbf{R}$ đều là một tập hợp đóng (tương ứng, mở) trong $\mathbf{R}$.*

Các tập hợp $[a, \to[ = a + \mathbf{R}_+$ và $]\leftarrow, a] = a - \mathbf{R}_+$ thu được bằng phép tịnh tiến từ $\mathbf{R}_+$ và $-\mathbf{R}_+$ tương ứng và do đó là đóng (Chương III, § 1, no. 1); các tập hợp $]\leftarrow, a[$ và $]a, \to[,$ là các phần bù của chúng, là mở; cuối cùng, khoảng đóng $[a, b]$ (tương ứng, khoảng mở $]a, b[$) là giao của $[a, \to[$ và $]\leftarrow, b]$ (tương ứng, của $]a, \to[$ và $]\leftarrow, b[$) và do đó là một tập hợp đóng (tương ứng, mở).

Các khoảng đóng $[-a, +a]$ ($a > 0$) trong $\mathbf{R}$ do đó là các lân cận của 0. Ta hãy chứng minh rằng chúng tạo thành một *hệ cơ bản các lân cận* của 0 khi $a$ chạy qua $\mathbf{R}_+^*$. Để làm điều này, chỉ cần thiết lập mệnh đề sau:

#### Mệnh đề 3 {#top-iv-s1-prop-3 .statement}

*Khi $r$ chạy qua tập hợp các số hữu tỉ $> 0$, các khoảng $s_r = [-r, +r]$ trong $\mathbf{R}$ tạo thành một hệ cơ bản các lân cận của 0.*

Theo Mệnh đề 7 của Chương III, § 3, no. 4 ta thu được một hệ cơ sở các lân cận của 0 trong $\mathbf{R}$ bằng cách lấy các *bao đóng* trong $\mathbf{R}$ của các khoảng

S_r \cap \mathbf{Q} = [-r, +r] \textit{of} \mathbf{Q}. Chứng minh sẽ hoàn tất nếu ta chỉ ra rằng S_r là bao đóng của S_r \cap \mathbf{Q}. Bây giờ S_r là đóng trong \mathbf{R}, và do đó ta chỉ cần chứng minh rằng, nếu x là một số thực sao cho -r < x < r, thì x thuộc bao đóng của S_r \cap \mathbf{Q}. Khoảng ]-r, +r[ là một tập mở trong \mathbf{R} và vì vậy với mọi lân cận V đủ nhỏ của o trong \mathbf{R} ta có x + V \subset ]-r, +r[; nhưng vì \mathbf{Q} trù mật trong \mathbf{R}, tồn tại một số hữu tỉ r' \in x + V, sao cho -r < r' < r và do đó r' \in S_r \cap \mathbf{Q}.

#### Hệ quả {#top-iv-s1-n4-cor-1 .statement}

*Mọi điểm của đường thẳng thực đều có một hệ cơ sở đếm được các lân cận.*

#### Mệnh đề 4 {#top-iv-s1-prop-4 .statement}

*Nếu (x, y) là một cặp bất kỳ các số thực sao cho x < y, thì có một số hữu tỉ r sao cho x < r < y.*

Vì \mathbf{Q} trù mật trong \mathbf{R}, chỉ cần chỉ ra rằng ]x, y[ là không rỗng; bằng phép tịnh tiến ta có thể giả sử x = 0 và y > 0. Bây giờ \mathbf{R} là một không gian Hausdorff và do đó, theo Mệnh đề 3, tồn tại một số hữu tỉ r > 0 sao cho y \notin ]-r, +r[, và điều này kéo theo 0 < r < y.

#### Mệnh đề 5 {#top-iv-s1-prop-5 .statement}

*Cho I là một khoảng bất kỳ trong \mathbf{R}. Khi đó tôpô cảm sinh trên I bởi tôpô của \mathbf{R} được sinh bởi các khoảng mở của I (trong đó I được xem là có thứ tự tuyến tính bởi quan hệ x \leq y).*

Mọi khoảng mở của I là vết trên I của một khoảng mở của \mathbf{R}. Điều này rõ ràng đối với một khoảng bị chặn, và khoảng không bị chặn ]a, \to[ của I là vết của khoảng không bị chặn ]a, \to[ của \mathbf{R}. Do đó ta có thể giới hạn vào trường hợp I = \mathbf{R}; nhưng trong trường hợp này kết quả suy ra từ Mệnh đề 3, vì mọi lân cận của một điểm x \in \mathbf{R} chứa một khoảng mở ]x - a, x + a[.

#### Nhận xét {#top-iv-s1-n4-rem-1 .statement}

Nếu A là một tập con trù mật của \mathbf{R}, tôpô của \mathbf{R} được sinh bởi các khoảng mở có các đầu mút thuộc A. Thật vậy, nếu

$$ ]x - a, x + a[ $$

là một khoảng mở chứa x, tồn tại hai điểm y, z của A sao cho x - a < y < x và x < z < x + a; do đó ]y, z[ chứa x và được chứa trong ]x - a, x + a[. Chứng minh này còn chỉ ra rằng, hơn nữa, các khoảng đang xét tạo thành một cơ sở (Chương I, § 1, no. 3) của tôpô của \mathbf{R}. Đặc biệt, nếu lấy A = \mathbf{Q}, ta thấy rằng tôpô của \mathbf{R} có một cơ sở đếm được.

### 5. ĐỘ DÀI CỦA MỘT KHOẢNG

#### Định nghĩa 3 {#top-iv-s1-def-3 .statement}

*Độ dài của một khoảng bị chặn với các đầu mút a và b (a \leq b) được định nghĩa là b - a.*

Mọi khoảng bị chặn chứa nhiều hơn một điểm do đó có độ dài > 0. Nếu $a \leq b$, bốn khoảng $[a, b], ]a, b[, [a, b[$ và $]a, b[$ đều có cùng độ dài. Một khoảng có các đầu mút $a + c$ và $b + c$ có cùng độ dài với một khoảng có các đầu mút $a$ và $b$; nói cách khác, *độ dài của một khoảng là bất biến đối với phép tịnh tiến*.

Nếu $a \leq c \leq d \leq b$ ta có $d - c \leq b - a$. Vì vậy nếu một khoảng bị chặn $I$ được chứa trong một khoảng bị chặn $I'$, độ dài của $I$ nhỏ hơn hoặc bằng độ dài của $I'$.

Nếu $n$ khoảng mở đôi một rời nhau $I_1, I_2, \ldots, I_n$ được chứa trong khoảng $[a, b]$ ($a < b$), dễ thấy bằng quy nạp theo $n$ rằng, nếu $I_k = ]c_k, d_k[$, tồn tại một phép hoán vị $\sigma$ của các chỉ số $k$ ($1 \leq k \leq n$) sao cho $d_{\sigma(k)} \leq c_{\sigma(k+1)}$ với $1 \leq k \leq n - 1$. Suy ra ngay lập tức rằng tổng các độ dài của các khoảng $I_k$ nhiều nhất bằng độ dài của $[a, b]$, và đẳng thức xảy ra khi và chỉ khi $c_{\sigma(1)} = a, d_{\sigma(n)} = b$ và $d_{\sigma(k)} = c_{\sigma(k+1)}$ với $1 \leq k \leq n - 1$.

### 6. TÍNH ĐỒNG DẠNG CỘNG TÍNH CỦA $\mathbf{R}$

Vì nhóm $\mathbf{R}$ có thứ tự tuyến tính, các hàm $x^+, x^-$ và $|x|$ được định nghĩa trên $\mathbf{R}$ theo cùng cách như trên $\mathbf{Q}$ và thỏa mãn mọi quan hệ được liệt kê ở trên đối với $\mathbf{Q}$, đặc biệt là các quan hệ (1) đến (7). Cho $a$ là một số thực > 0 và cho $U_a$ là tập hợp tất cả các cặp $(x, y) \in \mathbf{R} \times \mathbf{R}$ sao cho $|x - y| < a$; khi $a$ chạy qua tập hợp các số thực > 0 (hoặc tập hợp các số $1/n$), các tập hợp $U_a$ tạo thành một hệ cơ sở các lân cận của tính đồng dạng của nhóm cộng tính $\mathbf{R}$ của đường thẳng thực (được gọi là *tính đồng dạng cộng tính của đường thẳng thực*).

Các hàm $|x|$, $x^+$ và $x^-$ là *liên tục đều* trên $\mathbf{R}$, và các hàm $\sup(x, y)$ và $\inf(x, y)$ là *liên tục đều* trên $\mathbf{R} \times \mathbf{R}$; do đó các hàm này trùng với các hàm thu được bằng cách mở rộng bởi tính liên tục các hàm tương ứng được định nghĩa trên $\mathbf{Q}$ và $\mathbf{Q} \times \mathbf{Q}$, tương ứng.

### Bài tập {#top-iv-s1-exercises}

Xem các [bài tập cho § 1](exercises/s1/).
