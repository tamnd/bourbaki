---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 4
section_title: Exponentials and logarithms
lang: vi
source: top-v-x
pdf_pages: 0025-0029, 0034-0034
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF $a^x$ AND $\log_a x$
      page: 0
      pdf_page: 25
    - "no": 2
      title: BEHAVIOUR OF THE FUNCTIONS $a^x$ AND $\log_a x$
      page: 0
      pdf_page: 27
    - "no": 3
      title: MULTIPLIABLE FAMILIES OF NUMBERS $> 0$
      page: 0
      pdf_page: 28
statements: 1
exercises: 2
content_sha256: e1c199832feb5479cd6daba497bffab3faee58865c4bfbf276cb1827a0eb6b6e
translated_from: content/en/top/V/04_s4_exponentials_and_logarithms.md
source_content_sha256: 253a1c01cd6f9c44097f66ce6edc145a7650e56bfa06ec21ab22bc689a764fbb
translation_model: gpt-5-6-mini
translation_run: translate-vi-04d8dc68
glossary_version: 34
glossary_terms_sha256: c3f1bea702149026bc087488c268b12d862e72e1e8d248fa14531f79295432d8
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. HÀM MŨ VÀ LOGARIT

### 1. ĐỊNH NGHĨA CỦA $a^x$ VÀ $\log_a x$

#### Định lý 1 {#top-v-s4-thm-1 .statement}

*Nhóm nhân* $\mathbf{R}_+^*$ *của các số thực* $> 0$ *là một nhóm tôpô đẳng cấu với nhóm cộng* $\mathbf{R}$ *của các số thực*.

Vì $\mathbf{R}_+^* = ]0, +\infty[$ là một khoảng mở của $\mathbf{R}$ nên do đó *đồng phôi* với $\mathbf{R}$ (chương IV, § 4, no. 1, Mệnh đề 1). Theo Định lý 2 của § 3, do đó nó là một nhóm tôpô *đẳng cấu* với $\mathbf{R}$.

Theo Hệ quả của Mệnh đề 5 của § 1, no. 3, với mọi số $a > 0$ tồn tại duy nhất một đồng cấu liên tục $f_a$ của $\mathbf{R}$ vào $\mathbf{R}_+^*$ sao cho $f_a(1) = a$. Do đó, với mọi $x \in \mathbf{R}$ và mọi $y \in \mathbf{R}$ ta có

$$
f_a(x + y) = f_a(x) f_a(y), \qquad f_a(-x) = \frac{1}{f_a(x)},
$$

và do đó, đặc biệt, với mọi $n \in \mathbf{Z}$,

$$
f_a(n) = a^n.
$$

Vì lý do này, ta ký hiệu $f_a(x)$ bởi $a^x$ với mọi $x \in \mathbf{R}$; các hàm $a^x$ (với mọi giá trị của $a > 0$) được gọi là *các hàm mũ*. Ta có $1^x = 1$ với mọi $x \in \mathbf{R}$; nếu $a \neq 1$, $x \to a^x$ là một *đẳng cấu* của nhóm $\mathbf{R}$ lên nhóm $\mathbf{R}_+^*$.

Nếu $a \neq 1$, đẳng cấu của $\mathbf{R}_+^*$ lên $\mathbf{R}$ là nghịch đảo của $x \to a^x$ được gọi là *logarit cơ số* $a$, và giá trị của nó tại $x \in \mathbf{R}_+^*$ được ký hiệu bởi $\log_a x$. Như vậy, với ký hiệu này, ta có

(1) $$
a^{x+y} = a^x a^y \qquad (x \in \mathbf{R}, y \in \mathbf{R}, a > 0);
$$
(2) $$
a^{-x} = \frac{1}{a^x} \qquad (x \in \mathbf{R}, a > 0);
$$
(3) $$
\log_a 1 = 0, \quad \log_a a = 1 \qquad (a > 0, a \neq 1);
$$
(4) $$
\log_a (xy) = \log_a x + \log_a y \qquad (x > 0, y > 0);
$$
(5) $$
\log_a \left( \frac{1}{x} \right) = -\log_a x \qquad (x > 0);
$$
(6) $$
a^{\log_a x} = x \qquad (x > 0);
$$
(7) $$
\log_a a^x = x \qquad (x \in \mathbf{R}).
$$

Theo Mệnh đề 5 của § 1, no. 3, mọi đồng cấu liên tục của $\mathbf{R}$ vào $\mathbf{R}_+^*$ đều có dạng $y \to a^{xy}$, trong đó $x \in \mathbf{R}$; vì giá trị của nó khi $y = 1$ là $a^x$, nên đồng nhất ta có

(8) $$
(a^x)^y = a^{xy} \qquad (x \in \mathbf{R}, \ y \in \mathbf{R}, \ a > 0),
$$
hay, thay đổi ký hiệu,

(9) $$
x^y = a^{y \cdot \log_a x} \qquad (x > 0, y \in \mathbf{R}, a > 0, a \neq 1).
$$

Công thức (8) cho thấy rằng, với mọi số nguyên $n > 0$, ta có $(a^{1/n})^n = a$, điều này biện minh cho ký hiệu $a^{1/n}$ được đưa vào để chỉ *nghiệm bậc $n$* $\sqrt[n]{a}$, được định nghĩa trong chương IV, § 3, no. 3.

Các công thức (7) và (9) cho thấy rằng

(10) $$
\log_a (x^y) = y \log_a x \qquad (x > 0, y \in \mathbf{R}),
$$
hay, thay đổi ký hiệu,

(11) $$
\log_a x = \log_a b \cdot \log_b x \qquad (x > 0, a > 0, b > 0, a \neq 1, b \neq 1),
$$
đó là công thức về "thay đổi cơ số".

Cuối cùng, ta hãy thu được tất cả các *đồng cấu liên tục* của nhóm tôpô $\mathbf{R}^*$ vào chính nó; nếu $g$ là một đồng cấu liên tục như vậy,

$$
\log\_a (g(a^x))
$$

là một đồng cấu liên tục của $\mathbf{R}$ vào $\mathbf{R}$, do đó (§ 1, no. 3, Mệnh đề 5) tồn tại $\alpha \in \mathbf{R}$ sao cho $\log_a (g(a^x)) = \alpha x$ với mọi $x \in \mathbf{R}$; suy ra, theo (8), $g(x) = x^\alpha$ với mọi $x > 0$. Do đó ta có đồng nhất thức

(12) $$
(xy)^\alpha = x^\alpha y^\alpha \text{ for all } x > 0, y > 0 \text{ and } \alpha \in \mathbf{R}.
$$

Do công thức (4) biến mọi phép nhân thành một phép cộng (phép toán duy nhất mà hệ ghi số thông thường thích nghi tốt), logarit từ lâu đã là một công cụ không thể thiếu trong các phép tính số (xem Ghi chú lịch sử của chương này).

Khi được dùng cho mục đích này, cơ sở được chọn là $a = 10$; và có những bảng cho các giá trị của hàm $\log_{10} x$ (với một độ chính xác nhất định). Trong giải tích, người ta dẫn đến việc chọn một cơ sở khác (ký hiệu là $e$) sao cho $\lim_{x \to 1, x \neq 1} \frac{\log_e x}{(x - 1)} = 1$ (xem Bài tập 1).

### 2. HÀNH VI CỦA CÁC HÀM $a^x$ VÀ $\log_a x$

Theo Định lý 5 của Chương IV, § 2, no. 6, nếu $a \neq 1$, $x \to a^x$ là một ánh xạ đơn điệu nghiêm ngặt của $\mathbf{R}$ lên khoảng $\mathbf{R}_+^* = ]0, + \infty[$. Nếu $a > 1$, ta có $a^1 = a \geq 1 = a^0$, do đó $a^x$ là hàm tăng ngặt; hơn nữa, vì $\mathbf{R}_+^*$ không bị chặn trên, $a^x$ không bị chặn trên trong $\mathbf{R}$, nên

$$
\lim_{x \to +\infty} a^x = +\infty \quad (a > 1)
$$

và, theo (2),

$$
\lim_{x \to -\infty} a^x = 0 \quad (a > 1).
$$

Mặt khác, nếu $a < 1$, hàm $a^x$ là hàm giảm, tiến tới 0 khi $x$ tiến tới $+\infty$, và tiến tới $+\infty$ khi $x$ tiến tới $-\infty$ (Hình 1).

![Đồ thị biểu diễn y = a^x (a > 1) và y = a^x (a < 1)](https://i.imgur.com/1.png)

Hình 1.

![Đồ thị biểu diễn y = log\_a x (a > 1) và y = log\_a x (a < 1)](https://i.imgur.com/2.png)

Hình 2.

Từ các tính chất này và từ (12), ta suy ra rằng nếu $0 < a < b$, thì $a^x < b^x$ với $x > 0$, và $a^x > b^x$ với $x < 0$; vì $\left(\frac{b}{a}\right)^x > 1$ nếu $x > 0$, và $\left(\frac{b}{a}\right)^x < 1$ nếu $x < 0$.

Hành vi của $\log_a x$ trong $\mathbf{R}_+^*$ được suy ra từ hành vi của $a^x$ trong $\mathbf{R}$; nếu $a > 1$, hàm $\log_a x$ tăng ngặt, tiến tới $-\infty$ khi $x$ tiến tới $0$, và tiến tới $+\infty$ khi $x$ tiến tới $+\infty$; nếu $a < 1$, hàm $\log_a x$ giảm nghiêm ngặt, tiến tới $+\infty$ khi $x$ tiến tới $0$, và tiến tới $-\infty$ khi $x$ tiến tới $+\infty$ (Hình 2).

Hàm $a^x$ (tương ứng, $\log_a x$), được xét như một hàm xác định trên một tập con của đường thẳng mở rộng $\overline{\mathbf{R}}$ và nhận giá trị trong $\overline{\mathbf{R}}$, có thể được *mở rộng bằng tính liên tục* tới $\overline{\mathbf{R}}$ (tương ứng, tới khoảng $[0, +\infty]$ của $\overline{\mathbf{R}}$) bằng cách gán cho nó các giá trị giới hạn tại các điểm $+\infty$ và $-\infty$ (tương ứng, $0$ và $+\infty$).

Nói chung, công thức (9) cho thấy hàm $x^y$ liên tục trên không gian con $\mathbf{R}_+^* \times \mathbf{R}$ của $\overline{\mathbf{R}}^2$ và tiến tới một giới hạn khi $(x, y)$ tiến tới bất kỳ điểm $(a, b)$ nào của $\overline{\mathbf{R}}^2$ nằm trong bao đóng của $\mathbf{R}_+^* \times \mathbf{R}$, ngoại trừ các điểm $(0, 0)$, $(+\infty, 0)$, $(1, +\infty)$, $(1, -\infty)$. Do đó, ta có thể mở rộng $x^y$ bằng tính liên tục tới những điểm của $\overline{\mathbf{R}}^2$ tại đó giới hạn tồn tại; theo nguyên lý mở rộng các đồng nhất thức (chương I, § 8, no. 1, Mệnh đề 2, Hệ quả 1), các công thức (1), (4) và (8) vẫn đúng bất cứ khi nào cả hai vế đều có nghĩa.

Chú ý rằng việc mở rộng $x^y$ bằng tính liên tục không cho phép ta thu được công thức $0^0 = 1$.

Cũng chú ý rằng định nghĩa hàm mũ cho phép ta mở rộng tới $\mathbf{R}$ hàm $n \to a^n$ được xác định trên $\mathbf{Z}$, với mọi $a > 0$; nhưng bằng cách này ta không thu được bất kỳ mở rộng nào của hàm này khi $a < 0$; một mở rộng "tự nhiên" của hàm này chỉ có thể được định nghĩa theo lý thuyết các hàm giải tích.

### 3. HỌ CÁC SỐ $> 0$ CÓ THỂ NHÂN

Đẳng cấu của các nhóm tôpô $\mathbf{R}$ và $\mathbf{R}_+^*$ cho thấy ngay lập tức rằng để một họ $(x_i)$ gồm các số thực hữu hạn $> 0$ là *có thể nhân được* (chương IV, § 7, no. 4) thì điều kiện cần và đủ là họ $(\log_a x_i)$ phải *khả tổng* ($a$ là bất kỳ số nào $> 0$ và $\neq 1$); và ta có

$$
\prod_i x_i = a^{\sum \log_a x_i}.
$$

Tương tự, một tích vô hạn được xác định bởi một dãy $(1 + u_n)$ gồm các số hữu hạn $> 0$ là *hội tụ* (chương IV, § 7, no. 6) khi và chỉ khi chuỗi mà số hạng tổng quát là $\log_a (1 + u_n)$ hội tụ, và khi đó ta có

$$
\prod_{n=0}^{\infty} (1 + u_n) = a^{S_{n=0}^{\infty} \log_a (1 + u_n)}.
$$

Việc nghiên cứu các tích vô hạn của các số thực $> 0$ do đó được quy về việc nghiên cứu các chuỗi vô hạn của các số thực mà các số hạng xuất hiện dưới dạng các lôgarit; sau này chúng ta sẽ thấy các tổng có dạng này có thể được nghiên cứu dễ dàng như thế nào bằng các tính chất vi phân của lôgarit.

### Bài tập {#top-v-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
