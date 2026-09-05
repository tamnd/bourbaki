---
book: top
book_title: General Topology
chapter: VI
chapter_title: Real number spaces and projective spaces
section: 1
section_title: Real number space R^n
lang: vi
source: top-v-x
pdf_pages: 0037-0044, 0061-0064
extraction: ocr
subsections:
    - "no": 1
      title: THE TOPOLOGY OF $\mathbf{R}^n$
      page: 0
      pdf_page: 37
    - "no": 2
      title: THE ADDITIVE GROUP $\mathbf{R}^n$
      page: 0
      pdf_page: 38
    - "no": 3
      title: THE VECTOR SPACE $\mathbf{R}^n$
      page: 0
      pdf_page: 39
    - "no": 4
      title: AFFINE LINEAR VARIETIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 40
    - "no": 5
      title: TOPOLOGY OF VECTOR SPACES AND ALGEBRAS OVER THE FIELD $\mathbf{R}$
      page: 0
      pdf_page: 42
    - "no": 6
      title: TOPOLOGY OF MATRIX SPACES OVER $\mathbf{R}$
      page: 0
      pdf_page: 43
statements: 11
exercises: 13
content_sha256: f2e03243eb163f78b121700338d37fc662751a9d266e6c96a7a57f719990bfa4
translated_from: content/en/top/VI/01_s1_real_number_space_r_n.md
source_content_sha256: 4f407f3681e8c98681264a9fe4f2c17ccb92d164b832d84999ebc3cac3052ef4
translation_model: gpt-5.4-mini
translation_run: translate-vi-1054ba35
glossary_version: 34
glossary_terms_sha256: 4b9c6feb3b0d5a236f7454967ff45166f331db93754664cbc8c8999c8c5573b7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. KHÔNG GIAN SỐ THỰC $\mathbf{R}^n$

### 1. TÔPÔ CỦA $\mathbf{R}^n$

#### Định nghĩa 1 {#top-vi-s1-def-1 .statement}

*Tích tôpô của n không gian đồng nhất với đường thẳng thực được gọi là không gian số thực n chiều, và được ký hiệu bởi $\mathbf{R}^n$. \*

#### Nhận xét {#top-vi-s1-n1-rem-1 .statement}

Không gian $\mathbf{R}^0$ gồm một điểm.

Từ *Lý thuyết tập hợp*, Chương III, § 6, no. 3, Định lý 2, Hệ quả I, ta biết rằng, nếu E là một tập vô hạn, thì $E^n$ đẳng lực với E với mọi số nguyên $n > 0$; do đó, nếu $n > 0$, thì $\mathbf{R}^n$ đẳng lực với $\mathbf{R}$, tức là $\mathbf{R}^n$ *có lực lượng của liên tục* (xem các Bài tập 1 và 2).

#### Định nghĩa 2 {#top-vi-s1-def-2 .statement}

*Mọi tập con của $\mathbf{R}^n$ là tích của n khoảng mở (tương ứng đóng) của $\mathbf{R}$ được gọi là một hộp mở (tương ứng đóng) trong $\mathbf{R}^n$. [Với $n = 2$ thì nó được gọi là một hình chữ nhật mở (tương ứng đóng).]*

Các hộp mở trong $\mathbf{R}^n$ tạo thành một *cơ sở* của tôpô của $\mathbf{R}^n$ (Chương I, § 4, no. 1); các hộp mở chứa một điểm $x = (x_i)_{1 \leq i \leq n}$ của $\mathbf{R}^n$ tạo thành một hệ cơ bản các lân cận của $x$, và các hộp đóng của $\mathbf{R}^n$ mà $x$ là một điểm trong cũng vậy.

Mọi hộp mở khác rỗng trong $\mathbf{R}^n$ đều *đồng phôi* với $\mathbf{R}^n$ (Chương IV, § 4, no. 1, Mệnh đề 1).

Suy ra rằng, khi $n \geq 1$, mọi tập mở khác rỗng trong $\mathbf{R}^n$ đều có lực lượng của liên tục.

Một *khối lập phương* mở (tương ứng *đóng*) của $\mathbf{R}^n$ là một hộp mở (tương ứng đóng) là tích của n *khoảng bị chặn có cùng độ dài* [với $n = 2$, nó được gọi là một hình vuông mở (tương ứng đóng)]; độ dài chung của các khoảng này được gọi là cạnh (hay độ dài cạnh) của khối lập phương. Các khối lập phương mở

$$
K_m = \prod_{1 \leq i \leq n} \left[ x_i - \frac{1}{m}, x_i + \frac{1}{m} \right]
$$

tạo thành một hệ cơ bản đếm được các lân cận của điểm $x = (x_i)$, khi $m$ chạy qua tập tất cả các số nguyên $> 0$ hoặc qua bất kỳ dãy số nguyên nào tăng tới vô cùng.

Mọi hộp mở (hay đóng) trong $\mathbf{R}^n$ đều liên thông (Chương I, § 11, no. 4, Mệnh đề 8); nói riêng, $\mathbf{R}^n$ liên thông và liên thông địa phương.

Nếu $A$ là một tập mở khác rỗng trong $\mathbf{R}^n$, thì các thành phần của nó do đó là các tập mở (Chương I, § 11, no. 6, Mệnh đề 11); và tập các thành phần này là đếm được, vì $\mathbf{R}^n$ có một tập con trù mật đếm được (chẳng hạn $\mathbf{Q}^n$).

Xét xem dưới những điều kiện nào một tập con $A$ của $\mathbf{R}^n$ sẽ compact tương đối. Theo định lý Tychonoff (Chương I, § 9, no. 5, Định lý 3) thì điều kiện cần và đủ là các phép chiếu của $A$ lên các thừa số của $\mathbf{R}^n$ phải compact tương đối; theo định lý Borel-Lebesgue (Chương IV, § 2, no. 2, Định lý 2) điều này tương đương với việc nói rằng các phép chiếu ấy là các tập con bị chặn của $\mathbf{R}$. Ta nói rằng một tập con $A$ của $\mathbf{R}^n$ là bị chặn nếu mọi phép chiếu của nó đều là các tập con bị chặn của $\mathbf{R}$; do đó ta đã chứng minh:

#### Mệnh đề 1 {#top-vi-s1-prop-1 .statement}

Một tập con $A$ của $\mathbf{R}^n$ compact tương đối khi và chỉ khi nó bị chặn.

#### Hệ quả {#top-vi-s1-n1-cor-1 .statement}

Không gian $\mathbf{R}^n$ là compact địa phương, nhưng không compact nếu $n \geq 1$.

### 2. NHÓM CỘNG $\mathbf{R}^n$

Tập $\mathbf{R}^n$, được trang bị cấu trúc nhóm là tích của các cấu trúc nhóm cộng của n thừa số của $\mathbf{R}^n$, là một nhóm Abel; ta dùng ký hiệu cộng, nên tổng của $x = (x_i)$ và $y = (y_i)$ là $x + y = (x_i + y_i)$. Tôpô của không gian số tương thích với cấu trúc nhóm này; được trang bị hai cấu trúc ấy, $\mathbf{R}^n$ là một nhóm tôpô gọi là *nhóm cộng của không gian số thực n chiều*. Nếu $n = 0$, ta quy ước rằng $\mathbf{R}^0$ ký hiệu một nhóm chỉ gồm phần tử đơn vị.

Cấu trúc đều của nhóm này, gọi là *cấu trúc đều cộng tính* của $\mathbf{R}^n$, là tích của các cấu trúc đều của các thừa số của $\mathbf{R}^n$ (Chương III, § 3, no. 2). Nếu, với mỗi số nguyên $p > 0$, $V_p$ ký hiệu tập hợp các cặp $(x, y)$ của $\mathbf{R}^n$ sao cho $\max_{1 \leq i \leq n} |x_i - y_i| \leq 1/p$, thì các tập hợp $V_p$ tạo thành một *cơ bản*

### 3. KHÔNG GIAN VECTƠ $\mathbf{R}^n$

Vì $\mathbf{R}$ là một trường, ta có thể định nghĩa trên $\mathbf{R}^n$ một cấu trúc không gian vectơ trên trường $\mathbf{R}$, tích $t x$ của một vô hướng $t \in \mathbf{R}$ và một điểm (hoặc vectơ) $x = (x_i)$ của $\mathbf{R}^n$ là điểm $(t x_i)$. Chú ý rằng phép vị tự $(t, x) \to t x$ là liên tục trên $\mathbf{R} \times \mathbf{R}^n$. Nếu $e_i$ ký hiệu vectơ của $\mathbf{R}^n$ có tất cả các tọa độ đều bằng không, trừ tọa độ có chỉ số $i$, bằng 1, thì các $e_i$ tạo thành một cơ sở của không gian vectơ $\mathbf{R}^n$, gọi là cơ sở chính tắc của không gian này. Mọi vectơ $x = (x_i) \in \mathbf{R}^n$ đều có thể viết $x = \sum_{i=1}^n x_i e_i$, và quan hệ $\sum_{i=1}^n t_i e_i = 0$ suy ra $t_i = 0$ với $1 \leq i \leq n$.

Không gian vectơ $\mathbf{R}^n$ do đó có chiều $n$ trên trường $\mathbf{R}$, theo nghĩa của đại số (Đại số, Chương II, § 7, no. 2); do đó có tên là không gian số thực $n$ chiều.

Cho $f$ là một ánh xạ afin của không gian vectơ $\mathbf{R}^n$ vào không gian vectơ $\mathbf{R}^m$ ($m$ và $n$ là các số nguyên > 0). Nếu ta đặt $g(x) = f(x) - f(0)$, thì $g$ là một ánh xạ tuyến tính của $\mathbf{R}^n$ vào $\mathbf{R}^m$. Cho $a_{ij}$ ($1 \leq j \leq m$) là các tọa độ của $g(e_i)$ trong $\mathbf{R}^m$ và cho $b_j$ ($1 \leq j \leq m$) là các tọa độ của $f(0)$; nếu $x_i$ ($1 \leq i \leq n$) là tọa độ thứ $i$ của $x \in \mathbf{R}^n$ và nếu $y_j$ là tọa độ thứ $j$ của $y = f(x)$, ta có

$$
y_j = \sum_{i=1}^n a_{ij} x_i + b_j \quad (1 \leq j \leq m).
$$

Vì mỗi đa thức tuyến tính trong $x_1, x_2, \ldots, x_n$ là liên tục đều trên $\mathbf{R}^n$, suy ra mọi ánh xạ afin của $\mathbf{R}^n$ vào $\mathbf{R}^m$ đều liên tục đều trên $\mathbf{R}^n$ (Chương II, § 2, no. 6, Mệnh đề 7).

Đặc biệt, ta biết rằng mọi ánh xạ afin của $\mathbf{R}^n$ lên chính nó đều song ánh và nghịch đảo của nó lại là một ánh xạ afin; do đó mọi ánh xạ afin của $\mathbf{R}^n$ lên chính nó đều là một homeomorphisme (và là một tự đẳng cấu của cấu trúc đều của $\mathbf{R}^n$).

Cho $(a_i)_{1 \leq i \leq n}$ là một hệ tự do gồm $n$ vectơ của $\mathbf{R}^n$ [nói cách khác là một cơ sở của không gian vectơ $\mathbf{R}^n$]; nếu $b$ là một điểm bất kỳ của $\mathbf{R}^n$, thì tập P gồm các điểm $x = b + \sum_{i=1}^{n} u_i a_i$ sao cho $-1 \leq u_i \leq 1$ với $1 \leq i \leq n$ là một lân cận compact của $b$; vì tồn tại một ánh xạ afin song ánh $f$ của $\mathbf{R}^n$ lên chính nó sao cho $f(b) = 0, f(b + a_i) = e_i$ với $1 \leq i \leq n$; và $f(P)$ là hình lập phương, tức là tích của $n$ khoảng $[ -1, +1 ]$ trong $n$ không gian nhân tử. $P$ được gọi là hình hộp song song đóng có tâm $b$ và các vectơ cơ sở $a_i$. Phần trong của $P$ gồm các điểm $b + \sum_{i=1}^{n} u_i a_i$ sao cho $-1 < u_i < 1$ với $1 \leq i \leq n$; nó được gọi là hình hộp song song mở có tâm $b$ và các vectơ cơ sở $a_i$.

### 4. CÁC ĐA TẠP TUYẾN TÍNH AFIN TRONG $\mathbf{R}^n$

Cho một đa tạp tuyến tính afin $p$-chiều $V$ trong $\mathbf{R}^n$, tồn tại một ánh xạ afin $f$ của $\mathbf{R}^n$ lên chính nó biến $V$ thành một đa tạp tọa độ $p$-chiều, nghĩa là một không gian con vectơ $V'$ được sinh bởi $p$ trong các vectơ của cơ sở chính tắc $(e_i)$ của $\mathbf{R}^n$. Tồn tại một ánh xạ từ $V'$ lên $\mathbf{R}^p$ là một đẳng cấu của cấu trúc không gian vectơ và tôpô của $V'$ lên các cấu trúc tương ứng của $\mathbf{R}^p$ (hơn nữa, thường tiện lợi khi đồng nhất $\mathbf{R}^p$ với một đa tạp tọa độ như thế $V'$, chẳng hạn với không gian con vectơ được sinh bởi $e_1, e_2, \ldots, e_p$). Ngoài ra, $V'$ là một tập con đóng của $\mathbf{R}^n$ (Chương I, § 4, no. 3, Hệ quả của Mệnh đề 7); suy ra:

#### Mệnh đề 2 {#top-vi-s1-prop-2 .statement}

*Mọi đa tạp afin tuyến tính $p$-chiều trong $\mathbf{R}^n$ đều là một tập con đóng của $\mathbf{R}^n$, và đồng phôi với $\mathbf{R}^p$.*

Chính kết quả này là nguồn gốc của các tên *đường thẳng* và *mặt phẳng* được gán cho các đa tạp afin tuyến tính có *một* và *hai* chiều trong một không gian vectơ trên một vành chia tùy ý. Ta cũng nhắc lại rằng, với $n \geq 1$, các đa tạp afin tuyến tính có $n - 1$ chiều của $\mathbf{R}^n$ được gọi là *các siêu phẳng* (*loc. cit.*).

$n$ đa tạp tọa độ một chiều, tức là $n$ đường thẳng đi qua $0$ và $n$ điểm $e_i$ tương ứng, được gọi là *các trục tọa độ*. Với $n = 2$ thì trục đi qua $e_1$ đôi khi được gọi là *trục hoành* và trục đi qua $e_2$ được gọi là *trục tung*; tọa độ thứ nhất của một điểm $x \in \mathbf{R}^2$ được gọi là *hoành độ* của nó, tọa độ thứ hai là *tung độ*.

Mỗi đường thẳng $D$ đi qua một điểm $a$ đều có một biểu diễn tham số $t \to a + tb$, trong đó $t$ chạy qua $\mathbf{R}$ và $b \neq 0$; ánh xạ này là một đồng phôi từ $\mathbf{R}$ lên $D$. Vectơ $b$ được gọi là một vectơ *chỉ phương* của D, và các thành phần của nó $b_i (1 \leq i \leq n)$ được gọi là các tỉ số chỉ phương của D. Nếu $b'$ là một vectơ chỉ phương khác của D, thì tồn tại $h \neq 0$ trong $\mathbf{R}$ sao cho $b' = hb$.

Tập các điểm $a + tb$, trong đó $t$ chạy qua tập các số thực $\geq 0$, được gọi là tia đóng (hay đơn giản là tia, hoặc nửa đường thẳng) có gốc $a$ và vectơ chỉ phương $b$ (hoặc với các tỉ số chỉ phương $b_i$). Nó là một tập con đóng của $\mathbf{R}^n$, đồng phôi với khoảng $[0, +\infty[$ của $\mathbf{R}$, và do đó liên thông. Đường thẳng D là hợp của hai tia có gốc $a$ và các vectơ chỉ phương lần lượt là $b$ và $-b$; hai tia này được gọi là đối nhau.

Lạm dụng ngôn ngữ, tập các điểm $a + tb$, trong đó $t$ chạy qua tập các số thực $> 0$, được gọi là tia mở có gốc $a$ và vectơ chỉ phương $b$; nó đồng phôi với khoảng ]$0, +\infty[$ (và do đó đồng phôi với $\mathbf{R}$), nhưng không mở trong $\mathbf{R}^n$ nếu $n > 1$, mặc dù nó mở trong đường thẳng chứa nó.

Một đường thẳng đi qua hai điểm phân biệt $x$ và $y$ cũng có một biểu diễn tham số $(u, v) \to ux + vy$, trong đó $(u, v)$ chạy qua tập các cặp số thực sao cho $u + v = 1$. Cho bất kỳ hai điểm $x, y$ nào (phân biệt hay không), tập các điểm $ux + uy$, trong đó $(u, v)$ chạy qua tập các cặp số thực sao cho $u \geq 0, v \geq 0$ và $u + v = 1$, được gọi là đoạn đóng (hay đơn giản là đoạn) có hai đầu mút $x, y$. Một đoạn đóng là compact và liên thông, vì nếu hai đầu mút của nó phân biệt thì nó đồng phôi với khoảng $[0, 1]$ của $\mathbf{R}$.

Nếu $x \neq y$, tập các điểm $ux + vy$ sao cho $u > 0, v > 0$ và $u + v = 1$ được gọi (một cách nói lỏng) là đoạn mở có hai đầu mút $x, y$; nó đồng phôi với khoảng mở ]$0, 1[$ (và do đó cũng đồng phôi với $\mathbf{R}$). Cuối cùng, hợp của $\{y\}$ và đoạn mở có hai đầu mút $x, y$ đôi khi được gọi là đoạn mở tại $x$ và đóng tại $y$; nó đồng phôi với khoảng $[0, 1[$. Mọi đoạn có $x$ và $y$ làm hai đầu mút đều liên thông, và bao đóng của mỗi đoạn ấy là đoạn đóng có cùng hai đầu mút.

#### Mệnh đề 3 {#top-vi-s1-prop-3 .statement}

*Cho $f(x) = f(x_1, x_2, \ldots, x_n)$ là một đa thức với hệ số thực, không đồng nhất bằng không, xác định trên $\mathbf{R}^n$. Khi đó phần bù của tập $\overline{f}(0)$ là trù mật trong $\mathbf{R}^n$.*

Cho $x$ là một điểm bất kỳ của $\mathbf{R}^n$ và cho $y \in \mathbf{R}^n$ sao cho $f(y) \neq 0$; $\varphi(t) = f(x + t(y - x))$ là một đa thức theo biến thực $t$, không đồng nhất bằng không; do đó tồn tại các giá trị của $t$ tùy ý nhỏ sao cho $\varphi(t) \neq 0$. Điều này cho thấy rằng $x$ nằm trong bao đóng của phần bù của $\overline{f}(0)$.

#### Hệ quả {#top-vi-s1-n4-cor-1 .statement}

*Phần bù của một tập tuyến tính afin có chiều $p < n$ là trù mật trong $\mathbf{R}^n$. \*

Vì mọi tập tuyến tính afin có chiều $p < n$ đều được chứa trong một siêu phẳng, nên chỉ cần chứng minh hệ quả cho một siêu phẳng; nhưng một siêu phẳng được xác định bởi một phương trình $g(x) = 0$, trong đó $g$ là một đa thức tuyến tính không đồng nhất bằng không.

#### Mệnh đề 4 {#top-vi-s1-prop-4 .statement}

*Trong $\mathbf{R}^n$ ($n \geq 1$) phần bù của mọi siêu phẳng có hai thành phần liên thông.*

Cho $g(x) = 0$ là một phương trình của một siêu phẳng $H$ trong $\mathbf{R}^n$, với $g$ là một đa thức tuyến tính. Tập $CH$ là hợp của tập $E_1$ gồm mọi điểm $x$ sao cho $g(x) > 0$ và tập $E_2$ gồm mọi điểm $x$ sao cho $g(x) < 0$. $E_1$ và $E_2$ là liên thông, vì nếu $g(x) > 0$ và $g(y) > 0$ thì ta có $g(ux + vy) = ug(x) + vg(y) > 0$ mỗi khi $u \geq 0, v \geq 0$ và $u + v = 1$; nói cách khác, đoạn thẳng có hai đầu mút $x$ và $y$ được chứa trong $E_1$. Tương tự đối với $E_2$. Mặt khác, $CH$ không liên thông, vì ảnh của nó trong $\mathbf{R}$ qua $g$ là hợp của các khoảng ]$0, +\infty$ [ và ]$-\infty, 0$ [.

Các thành phần $E_1, E_2$ của phần bù của một siêu phẳng $H$ được gọi là các *nửa không gian mở* được xác định bởi $H$.

Các bao đóng của $E_1$ và $E_2$, tức là lần lượt $E_1 \cup H$ và $E_2 \cup H$, được gọi là các *nửa không gian đóng* được xác định bởi $H$.

Nhận thấy rằng một ánh xạ afin của $\mathbf{R}^n$ lên chính nó, biến $H$ thành một siêu phẳng "tọa độ", chẳng hạn siêu phẳng có phương trình là $x_n = 0$, cũng biến các nửa không gian mở được xác định bởi $H$ thành các nửa không gian mở được xác định lần lượt bởi các quan hệ $x_n > 0$ và $x_n < 0$; các nửa không gian sau là các hộp mở và do đó *đồng phôi với* $\mathbf{R}^n$.

### 5. TÔPÔ CỦA CÁC KHÔNG GIAN VECTƠ VÀ ĐẠI SỐ TRÊN TRƯỜNG $\mathbf{R}$

Cho $E$ là một không gian vectơ có chiều $n$ trên trường $\mathbf{R}$; nếu $(a_i)_{1 \leq i \leq n}$ là một *cơ sở* của $E$, thì mỗi điểm $x \in E$ đều viết duy nhất được dưới dạng $x = \sum_{i=1}^n x_i a_i$, trong đó các $x_i$ là những số thực; do đó ánh xạ $(x_i) \to \sum_{i=1}^n x_i a_i$ là một ánh xạ tuyến tính song ánh của $\mathbf{R}^n$ lên $E$.

Nếu ta *phép chuyển* tôpô của $\mathbf{R}^n$ sang $E$ bằng ánh xạ này, thì $E$ được trang bị một tôpô tương thích với cấu trúc nhóm cộng của nó, và ánh xạ $(t, x) \to tx$ từ $\mathbf{R} \times E$ vào $E$ là liên tục đối với tôpô này. Tôpô này *không phụ thuộc vào cơ sở* được chọn trong $E$; vì nếu $(a')$ là một cơ sở khác của $E$, và nếu $x = \sum_{i=1}^n x'_i a'_i = \sum_{i=1}^n x_i a_i$, thì ánh xạ $(x_i) \to (x'_i)$ của $\mathbf{R}^n$ lên chính nó là tuyến tính và do đó là một đồng phôi.

Sự kiện này khiến người ta ngờ rằng tôpô được định nghĩa như vậy trên $E$ có thể được đặc trưng hóa mà không cần đến cơ sở của $E$. Thật vậy, về sau ta sẽ thấy rằng đây là tôpô Hausdorff *duy nhất* trên $E$ sao cho các hàm $x - y$ (trên $E \times E$) và $tx$ (trên $\mathbf{R} \times E$) liên tục.

Nếu bây giờ $A$ là một *đại số* có hạng hữu hạn $n$ trên trường $\mathbf{R}$, thì tôpô ở trên trên $A$ (xem như một không gian vectơ $n$-chiều trên $\mathbf{R}$) tương thích không những với cấu trúc nhóm cộng của $A$, mà còn với cấu trúc *vành* của nó. Đây là hệ quả của kết quả tổng quát hơn sau đây:

#### Mệnh đề 5 {#top-vi-s1-prop-5 .statement}

*Cho $E, F, G$ là ba không gian vectơ hữu hạn chiều trên trường $\mathbf{R}$. Khi đó mọi ánh xạ song tuyến tính (*) $f$ từ $E \times F$ vào $G$ đều liên tục.*

Ta có thể giả sử rằng $E = \mathbf{R}^m, F = \mathbf{R}^n, G = \mathbf{R}^p$; chỉ cần chứng minh rằng các tọa độ trong $\mathbf{R}^p$ của $f(x, y)$ là những hàm liên tục của $(x, y) \in E \times F$ (Chương I, § 4, no. 1, Mệnh đề 1). Nói cách khác, chỉ cần chứng minh rằng mọi *dạng song tuyến tính* $g$ đều liên tục trên $E \times F$; và điều này là ngay lập tức, vì $g(x, y)$ là một đa thức theo các tọa độ của $x$ và $y$.

### 6. TÔPÔ CỦA CÁC KHÔNG GIAN MA TRẬN TRÊN $\mathbf{R}$

Một ví dụ quan trọng của một không gian vectơ trên $\mathbf{R}$ là không gian $\mathbf{M}_{m,n}(\mathbf{R})$ của *các ma trận với m hàng và n cột* mà các phần tử của chúng thuộc $\mathbf{R}$; đây là một không gian có chiều $mn$ trên $\mathbf{R}$, do đó đồng phôi với $\mathbf{R}^{mn}$. Theo Mệnh đề 5 của § 5, tích $X.Y$ của hai ma trận $X \in \mathbf{M}_{m,n}(\mathbf{R}), Y \in \mathbf{M}_{n,p}(\mathbf{R})$ là một hàm liên tục của $(X, Y)$. Đặc biệt, tôpô của không gian $\mathbf{M}_n(\mathbf{R})$ các ma trận vuông cấp $n$ tương thích với cấu trúc vành trên $\mathbf{M}_n(\mathbf{R})$. Hơn nữa:

#### Mệnh đề 6 {#top-vi-s1-prop-6 .statement}

*Trong vành $\mathbf{M}_n(\mathbf{R})$, nhóm $\mathbf{GL}_n(\mathbf{R})$ của các ma trận không suy biến là một tập con mở trù mật, và tôpô cảm sinh trên tập này tương thích với cấu trúc nhóm của nó.*

(* ) Nếu $E, F, G$ là ba không gian vectơ trên một trường $K$, một ánh xạ $f$ từ $E \times F$ vào $G$ được gọi là *song tuyến tính* nếu ta có đồng nhất
$$
f(x + x', y) = f(x, y) + f(x', y), \quad f(x, y + y') = f(x, y) + f(x, y'),
$$
$$
f(\lambda x, y) = f(x, \lambda y) = \lambda f(x, y)
$$
với mọi $x, x' \in E$, mọi $y, y' \in F$ và mọi $\lambda \in K$.

Nếu $X$ là một ma trận vuông khả nghịch, các phần tử của $X^{-1}$ là các hàm hữu tỉ của các phần tử của $X$; do đó các hàm này được xác định và liên tục trong một lân cận của $X$, nên mọi ma trận $Y$ trong lân cận này đều khả nghịch, và ánh xạ $Y \to Y^{-1}$ liên tục tại điểm $X$; suy ra $\mathbf{GL}_n(\mathbf{R})$ là một tập mở trong $\mathbf{M}_n(\mathbf{R})$ và tôpô của $\mathbf{GL}_n(\mathbf{R})$ tương thích với cấu trúc nhóm của nó.

Cuối cùng, $\mathbf{GL}_n(\mathbf{R})$ là phần bù của tập hợp các ma trận vuông $X$ có định thức bằng không; vì định thức của $X$ là một đa thức theo các phần tử của $X$, Mệnh đề 3 của no. 4 cho thấy rằng $\mathbf{GL}_n(\mathbf{R})$ trù mật trong $\mathbf{M}_n(\mathbf{R})$.

### Bài tập {#top-vi-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).
