---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 0
section_title: Hardy Fields. (H) Functions
appendix: true
lang: vi
source: fvr-i-vii
pdf_pages: 0262-0273, 0278-0282
extraction: ocr
subsections:
    - "no": 1
      title: HARDY FIELDS
      page: 0
      pdf_page: 262
    - "no": 2
      title: EXTENSION OF A HARDY FIELD
      page: 0
      pdf_page: 263
    - "no": 3
      title: COMPARISON OF FUNCTIONS IN A HARDY FIELD
      page: 0
      pdf_page: 265
    - "no": 4
      title: (H) FUNCTIONS
      page: 0
      pdf_page: 267
    - "no": 5
      title: EXPONENTIALS AND ITERATED LOGARITHMS
      page: 0
      pdf_page: 268
    - "no": 6
      title: INVERSE FUNCTION OF AN (H) FUNCTION
      page: 0
      pdf_page: 270
statements: 21
exercises: 15
content_sha256: d443428924b062e186cff045b5a775b937232c7f4f21129535592ad2662ab0c5
translated_from: content/en/fvr/V/A_a_hardy_fields_h_functions.md
source_content_sha256: 211cef728f92b9ed4d60cc34a4d1f0d68ce047104889cba432f95522f59df089
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-75b0505f
glossary_version: 34
glossary_terms_sha256: 57c466909efbf824c118ff8bf50e8919a7383444363ab860edb720c5485f54fa
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# Các trường Hardy. Các hàm (H)

### 1. CÁC TRƯỜNG HARDY

Cho $\mathfrak{F}$ là cơ sở lọc trên $\mathbf{R}$ được tạo bởi các khoảng dạng $[x_0, +\infty[$. Nhắc lại rằng ta đã định nghĩa một quan hệ tương đương $R_\infty$ trên tập hợp $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ các hàm thực được xác định trên các tập hợp thuộc $\mathfrak{F}$: “tồn tại một tập hợp $M \in \mathfrak{F}$ sao cho $f(x) = g(x)$ trên $M$” (V, p. 211), và tập thương $\mathcal{H}(\mathfrak{F}, \mathbf{R})/R_\infty$ được trang bị cấu trúc của một *vành* có phần tử đơn vị.

#### Định nghĩa 1 {#fvr-v-a0-def-1 .statement}

*Cho một tập con $\mathfrak{K}$ của $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, ta nói rằng $\mathfrak{K}/R_\infty$ (ảnh chính tắc của $\mathfrak{K}$ trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})/R_\infty$) là một trường Hardy nếu $\mathfrak{K}$ thỏa mãn các điều kiện sau:

1. $\mathfrak{K}/R_\infty$ is a subfield of the ring $\mathcal{H}(\mathfrak{F}, \mathbf{R})/R_\infty$.
2. *Every function in $\mathfrak{K}$ is continuous and differentiable on an interval $[a, +\infty[$ (depending on the function), and the class with respect to $R_\infty$ of its derivative belongs to $\mathfrak{K}/R_\infty$.*

Giả thiết rằng $\mathfrak{K}/R_\infty$ là một *trường* tương đương với các điều kiện sau: nếu $f \in \mathfrak{K}$ và $g \in \mathfrak{K}$ thì $f + g$ và $fg$ bằng các hàm thuộc $\mathfrak{K}$ trên một tập hợp nào đó trong $\mathfrak{F}$; hơn nữa, nếu $f$ không đồng nhất bằng không trên một tập hợp thuộc $\mathfrak{F}$ thì tồn tại một tập hợp $M$ trong $\mathfrak{F}$ mà trên đó $f$ *không triệt tiêu*, và $1/f$ bằng một hàm của $\mathfrak{K}$ trên $M$; theo điều kiện 2', luôn có thể giả sử rằng $M$ được chọn sao cho $f$ *liên tục* trên $M$, và do đó *có dấu không đổi* trên khoảng này.

Do một sự lạm dụng ngôn ngữ, nếu $\mathfrak{K}$ sao cho $\mathfrak{K}/R_\infty$ là một trường Hardy thì trong phần tiếp theo ta sẽ nói rằng chính $\mathfrak{K}$ là một *trường Hardy*.

#### Ví dụ 1 {#fvr-v-a0-n1-exa-1 .statement}

Mọi trường Hardy đều chứa trường các *hằng hữu tỉ* (trường nhỏ nhất có đặc số 0, *xem Alg.*, V, §1), trường này có thể đồng nhất với trường $\mathbf{Q}$; hơn nữa, vì hai hằng số không thể đồng dư theo môđun $R_\infty$ trừ khi chúng bằng nhau, nên $\mathbf{Q}/R_\infty$ đồng nhất với $\mathbf{Q}$. Các *hằng thực* cũng tạo thành một trường Hardy, trường này có thể đồng nhất với $\mathbf{R}$.

#### Ví dụ 2 {#fvr-v-a0-n1-exa-2 .statement}

Một ví dụ rất quan trọng của trường Hardy là *tập hợp các hàm hữu tỉ với hệ số thực*, mà do một sự lạm dụng ngôn ngữ ta sẽ ký hiệu là $\mathbf{R}(x)$; nếu $f(x) = p(x)/q(x)$ là một hàm hữu tỉ với hệ số thực, không đồng nhất bằng không, thì nó liên tục, khả vi, và $\neq 0$ trên một khoảng $[a, +\infty[$, trong đó $a$ lớn hơn nghiêm ngặt nghiệm thực lớn nhất của các đa thức $p(x)$ và $q(x)$; do đó mọi phần tử của $\mathbf{R}(x)/R_\infty$ khác 0 đều khả nghịch. Ta lại chú ý rằng hai hàm hữu tỉ không thể đồng dư theo môđun $\mathbf{R}_\infty$ trừ khi chúng bằng nhau, nên $\mathbf{R}(x)/\mathbf{R}_\infty$ lại có thể được đồng nhất với $\mathbf{R}(x)$.

### 2. MỞ RỘNG MỘT TRƯỜNG HARDY

Cho một trường Hardy $\mathfrak{K}$, ta sẽ thấy cách có thể tạo thành các trường Hardy mới $\mathfrak{K}' \supset \mathfrak{K}$ sao cho $\mathfrak{K}'/\mathbf{R}_\infty$ thu được bằng cách *kết nạp* (theo nghĩa đại số của thuật ngữ này, *xem Alg.*, V. §2) các phần tử mới, có một dạng mà ta sẽ làm rõ, vào $\mathfrak{K}/\mathbf{R}_\infty$.

#### Bổ đề 1 {#fvr-v-a0-lem-1 .statement}

*Cho* $a(x), b(x)$ *là hai hàm thực liên tục không thay đổi dấu trên một khoảng* $[x_0, +\infty[$. *Nếu, trên khoảng này, hàm* $y(x)$ *là liên tục và khả vi, và thỏa mãn đẳng thức*

$$
y' = ay + b
$$

(1)

*thì tồn tại một khoảng* $[x_1, +\infty[$ *trên đó* $y$ *không thay đổi dấu.*

Thật vậy, đặt $z(x) = y(x) \exp \left( - \int_{x_0}^x a(t) \, dt \right)$ (*xem IV*, p. 183); khi đó, theo (1), $z'(x) = b(x) \exp \left( - \int_{x_0}^x a(t) \, dt \right)$. Nếu $b(x) \geqslant 0$ với $x \geqslant x_0$ thì $z$ là tăng trên khoảng này, do đó hoặc là $< 0$ trên toàn bộ khoảng này, hoặc là không trên một khoảng $[x_1, +\infty[$, hoặc ngược lại là $> 0$ trên một khoảng $[x_1, +\infty[$; vì $y$ có cùng dấu với $z$ nên mệnh đề được chứng minh trong trường hợp này. Lập luận tương tự nếu $b(x) \leqslant 0$ với $x \geqslant x_0$.

#### Nhận xét {#fvr-v-a0-n2-rem-1 .statement}

Tính chất rất sơ cấp này không mở rộng cho các phương trình vi phân tuyến tính cấp $> 1$; ví dụ, hàm $y = \sin x$ thỏa mãn $y'' + y = 0$, nhưng thay đổi dấu trên mọi lân cận của $+\infty$.

#### Bổ đề 2 {#fvr-v-a0-lem-2 .statement}

*Cho* $a(x)$ *và* $b(x)$ *là hai hàm thuộc một trường Hardy cho trước* $\mathfrak{K}$ *và* $y(x)$ *là một hàm thỏa mãn đẳng thức* (1) *trên một khoảng* $[x_0, +\infty[$ *trên đó* $a$ *và* $b$ *được xác định và liên tục*. *Nếu* $p(u)$ *là một đa thức theo* $u$ *có các hệ số là các hàm của* $x$ *thuộc* $\mathfrak{K}$, *được xác định và khả vi trên* $[x_0, +\infty[$, *thì tồn tại một khoảng* $[x_1, +\infty[$ *trên đó hàm* $p(y)$ *không thay đổi dấu.*

Mệnh đề là tầm thường nếu $p(u)$ có các hệ số đồng nhất bằng không trên $[x_0, +\infty[$, hoặc nếu $p(u)$ có bậc 0 theo $u$, vì mọi hàm trong $\mathfrak{K}$ đều có dấu hằng trên một khoảng $[x_1, +\infty[$. Giả sử rằng $p(u)$ có bậc $n > 0$; hệ số đầu $c$ của $p(u)$ khi đó là $\neq 0$ trên một khoảng $[\alpha, +\infty[$; do đó ta có thể viết $p(u) = c(u^n + c_1 u^{n-1} + \cdots + c_n)$ trong đó $c, c_1, c_2, \ldots, c_n$ là các *hàm* thuộc $\mathfrak{K}$ và khả vi trên $[\alpha, +\infty[$; vì vậy chỉ cần chứng minh bổ đề cho $c = 1$. Ta lập luận bằng quy nạp theo $n$; ta có

$$
\frac{d}{dx} (p(y)) = (ay + b)(ny^{n-1} + (n-1)c_1 y^{n-2} + \cdots + c_{n-1})
$$
$$
+ c'_1 y^{n-1} + \cdots + c'_n = na\ p(y) + q(y)
$$

trong đó $q(u)$ là một đa thức bậc $\leq n - 1$, với các hệ số trong $\mathfrak{K}$. Theo giả thiết các hàm $na(x)$ và $q(y(x))$ không thay đổi dấu trên một khoảng $[ \beta, +\infty[$; do đó bổ đề là một hệ quả của bổ đề 1.

#### Định lý 1 {#fvr-v-a0-thm-1 .statement}

*Cho $a(x)$ và $b(x)$ là hai hàm thuộc một trường Hardy đã cho $\mathfrak{K}$ và $y(x)$ là một hàm thỏa mãn (1) trên một khoảng $[ x_0, +\infty[$. Khi $r(u) = p(u)/q(u)$ chạy qua tập hợp các phân thức hữu tỉ theo $u$ với các hệ số trong $\mathfrak{K}$ sao cho $q(y)$ không đồng nhất bằng không trên một lân cận của $+\infty$ thì tập hợp $\mathfrak{K}(y)$ các hàm $r(y)$ tạo thành một trường Hardy.*

Thật vậy, theo bổ đề 2, tồn tại một khoảng $[ x_1, +\infty[$ trên đó $r(y)$ được xác định, liên tục và không thay đổi dấu, từ đó suy ra ngay lập tức rằng $\mathfrak{K}(y)/\mathbf{R}_\infty$ là một trường; hơn nữa, vì

$$
\frac{d}{dx}(r(y)) = r'(y)y' = r'(y)(ay + b)
$$

(trong đó $r'(y) = (p'(y)q(y) - p(y)q'(y))/(q(y))^2$ được xác định theo giả thiết trên một lân cận của $+\infty$), đạo hàm của mọi hàm trong $\mathfrak{K}(y)$ thuộc $\mathfrak{K}(y)$, điều này chứng minh rằng $\mathfrak{K}(y)$ thỏa mãn các điều kiện của định nghĩa 1 của V, p. 247.

Rõ ràng rằng $\mathfrak{K}(y)/\mathbf{R}_\infty$ thu được bằng phép *nối* đại số vào $\mathfrak{K}/\mathbf{R}_\infty$ của lớp của $y$ modulo $\mathbf{R}_\infty$. Một lần nữa người ta nói rằng $\mathfrak{K}(y)$ thu được bằng cách *nối* $y$ vào $\mathfrak{K}$.

#### Hệ quả 1 {#fvr-v-a0-thm-1-cor-1 .statement}

*Nếu $y$ là một hàm trong $\mathfrak{K}$, không đồng nhất bằng không trên một lân cận của $+\infty$, thì $\mathfrak{K}(\log|y|)$ là một trường Hardy.*

Thật vậy, $(\log|y|)' = y'/y$ bằng một hàm trong $\mathfrak{K}$ trên một khoảng $[ x_0, +\infty[$.

HỆ QUẢ 2 *Nếu $y$ là một hàm bất kỳ trong $\mathfrak{K}$, thì $\mathfrak{K}(e^y)$ là một trường Hardy.*

Thật vậy, $(e^y)' = e^y y'$, và $y'$ bằng một hàm trong $\mathfrak{K}$ trên một khoảng $[ x_0, +\infty[$.

HỆ QUẢ 3 *Nếu $\mathfrak{K}$ chứa các hằng số thực, và nếu $y$ là một hàm trong $\mathfrak{K}$, không đồng nhất bằng không trên một lân cận của $+\infty$, thì $\mathfrak{K}(|y|^{\alpha})$ là một trường Hardy với mọi số thực $\alpha$.*

Thật vậy, $\frac{d}{dx}(|y|^{\alpha}) = |y|^{\alpha} (\alpha y'/y)$, và $\alpha y'/y$ bằng một hàm trong $\mathfrak{K}$ trên một khoảng $[ x_0, +\infty[$.

Cuối cùng, ta chú ý rằng nếu $y$ là *nguyên thủy* của một hàm bất kỳ trong $\mathfrak{K}$ thì $\mathfrak{K}(y)$ lại là một trường Hardy.

### 3. SO SÁNH CÁC HÀM TRONG MỘT TRƯỜNG HARDY

#### Mệnh đề 1 {#fvr-v-a0-prop-1 .statement}

*Hai hàm trong cùng một trường Hardy là so sánh được theo mọi cấp* (V, p. 232).

Thật vậy, nếu $f$ thuộc một trường Hardy $\mathcal{K}$, thì với mọi số nguyên $n > 0$ tồn tại một khoảng $[x_0, +\infty[$ trên đó $f$ khả vi $n$ lần, đạo hàm cấp $n^{th}$ của nó bằng một hàm trong $\mathcal{K}$ trên khoảng này. Do đó chỉ cần chứng minh rằng hai hàm bất kỳ $f, g$ của $\mathcal{K}$ là *so sánh được*. Điều này hiển nhiên nếu một trong các hàm là đồng nhất không trên một lân cận của $+\infty$; vì vậy ta có thể giới hạn vào trường hợp cả hai đều dương ngặt trên một lân cận của $+\infty$. Nhưng khi đó, với mọi số thực $t$, $f - tg$ bằng một hàm trong $\mathcal{K}$ trên một lân cận của $+\infty$, nên có dấu không đổi trên một lân cận của $+\infty$, điều này chứng minh mệnh đề (V, p. 217, mệnh đề 9).

Từ mệnh đề này suy ra ngay rằng, nếu một trường Hardy $\mathcal{K}$ chứa các hằng thực (như ta luôn giả sử trong phần tiếp theo), và nếu $f$ và $g$ là hai hàm tùy ý trong $\mathcal{K}$ thì hai trong các hàm $e^f, e^g, \log |f|, \log |g|, |f|^{\alpha}, |g|^{\alpha}$ ($\alpha$ là một số thực tùy ý), $\int_a f, \int_a g$ ($a$ là một số thực bất kỳ trong một khoảng $[x_0, +\infty[$ nơi $f$ và $g$ bị chặn) là *so sánh được* (khi chúng được xác định); thật vậy, hai trong các hàm này thuộc về một trường Hardy cho trước thu được bằng cách lần lượt ghép thêm chúng vào $\mathcal{K}$.

Tương tự, mọi hàm $f(x)$ trong một trường Hardy $\mathcal{K}$ đều so sánh được với $x$, vì $x$ và $f(x)$ thuộc về trường Hardy thu được bằng cách ghép thêm $x$ vào $\mathcal{K}$. Do đó suy ra (đặc biệt) rằng $f$ so sánh được theo mọi cấp với mọi lũy thừa $x^{\alpha}$, cũng như với $\log x$ và với $e^x$.

Cũng thấy rằng nếu $f$ và $g$ thuộc cùng một trường Hardy $\mathcal{K}$, nếu $g(x) > 0$ trên một khoảng $[x_0, +\infty[$, và nếu $g(x)$ tiến tới 0 hoặc tới $+\infty$ khi $x$ tiến tới $+\infty$, thì *cấp* của $f$ đối với $g$ (V, p. 219) luôn được xác định.

Mệnh đề 8 của V, p. 233, do đó áp dụng được cho mọi hàm $f$ trong một trường Hardy, và chứng minh rằng:

1' nếu $f$ có cấp $+\infty$ đối với $x$ thì $\int_a^x f(t)\,dt \sim (f(x))^2/f'(x)$.

2' nếu $f$ có cấp $\mu > -1$ đối với $x$ thì $\int_a^x f(t)\,dt \sim \frac{1}{\mu+1} x f(x)$.

3' nếu $f$ có cấp $\mu < -1$ đối với $x$ thì $\int_a^{+\infty} f(t)\,dt \sim -\frac{1}{\mu+1} x f(x)$.

4' nếu $f$ có cấp $-\infty$ đối với $x$ thì $\int_a^{+\infty} f(t)\,dt \sim -(f(x))^2/f'(x)$.

Hơn nữa, ta có mệnh đề sau:

#### Mệnh đề 2 {#fvr-v-a0-prop-2 .statement}

Cho $f$ là một hàm thuộc một trường Hardy $\mathcal{K}$.

1 Nếu $f$ có cấp vô hạn đối với $x$, thì, với mọi số nguyên $n > 0$,
$$
f^{(n)}(x) \sim \frac{(f'(x))^n}{(f(x))^{n-1}}.
$$
(2)

2° Nếu $f$ có cấp hữu hạn $\mu$ đối với $x$ thì, với mọi $n > 0$,
$$
f^{(n)}(x) \sim \mu(\mu - 1) \ldots (\mu - n + 1) \frac{f(x)}{x^n}
$$
$$
\sim \frac{(\mu - 1) \ldots (\mu - n + 1)}{\mu^{n-1}} \frac{(f'(x))^n}{(f(x))^{n-1}}
$$
(3)
trừ khi $\mu$ là một số nguyên $\geqslant 0$ và $n > \mu$.

1 Nếu $f$ có cấp vô hạn đối với $x$ thì có $\log |f| \gg \log x$, do đó, vì $\log |f|$ và $\log x$ so sánh được tới mọi cấp, $f'/f \gg 1/x$. Đặt $g = f'/f$; vì $g$ bằng một hàm trong $\mathcal{K}$ trên một lân cận của $+\infty$ ta suy ra từ $1/g \ll x$, rằng $g'/g^2 \ll 1$, và do đó $g'/g \ll g = f'/f$, hay một cách khác $fg' \ll gf'$. Từ quan hệ $f' = fg$ ta suy ra bằng cách lấy đạo hàm rằng
$$
f'' = fg' + gf' \sim gf'
$$
hay một cách khác $f''/f' \sim f'/f$. Lập luận tương tự, áp dụng cho $f^{(n)}$ thay cho $f$, cho thấy, bằng quy nạp theo $n$, rằng $f^{(n)}/f^{(n-1)} \sim f'/f$; do đó quan hệ (2).

2 Nếu $f$ có cấp hữu hạn $\mu$ đối với $x$, và nếu $\mu \neq 0$, ta có $\log |f| \sim \mu \log x$, do đó, khi lấy đạo hàm, $f'(x) \sim \mu \frac{f(x)}{x}$; suy ra rằng $f'$ có cấp $\mu - 1$ đối với $x$, điều này cho phép áp dụng cùng một lập luận bằng quy nạp theo $n$ chừng nào $\mu \neq n$, do đó có công thức (3) khi $\mu$ không phải là một số nguyên $\geqslant 0$ và $< n$.

Khi $f$ có cấp nguyên $p \geqslant 0$ đối với $x$ ta có thể viết $f(x) = x^p f_1(x)$, trong đó $f_1$ có cấp 0 đối với $x$. Theo mệnh đề 2 ta có
$$
f^{(p)} \sim p! f_1.
$$
Để tính các đạo hàm có cấp $n > p$ ta có thể chỉ xét trường hợp $p = 0$. Khi đó ta có $\log |f| \ll \log x$, do đó $f'(x)/f(x) \ll 1/x$, nói cách khác $x f'(x) \ll f(x)$; nếu $f$ không tương đương với một hằng $k \neq 0$ thì, khi lấy đạo hàm của quan hệ này (V, p. 232, mệnh đề 7), ta có $x f''(x) + f'(x) \ll f'(x)$, điều này suy ra $x f''(x) \sim -f'(x)$. Tính đến công thức này, bằng quy nạp theo $n$ ta thấy rằng $f^{(n)}$ có cấp $\leqslant -n$ đối với $x$, và rằng
$$
f^{(n)} \sim (-1)^{n+1} (n-1)! \frac{f'(x)}{x^{n-1}}.
$$
(4)

Nếu $f$ tương đương với một hằng $k \neq 0$ thì ta có $f(x) = k + f_2(x)$ với $f_2 \ll 1$, và quy về việc khảo sát các đạo hàm của $f_2$.

### 4. (H) HÀM

#### Mệnh đề 3 {#fvr-v-a0-prop-3 .statement}

*Nếu $\mathcal{K}_0$ là một trường Hardy thì tồn tại một trường Hardy $\mathcal{K}$ chứa $\mathcal{K}_0$ và sao cho, đối với mọi hàm $z \in \mathcal{K}$, không đồng nhất bằng không trên một lân cận của $+\infty$, cả $e^z$ và $\log |z|$ đều thuộc $\mathcal{K}$.*

Ký hiệu $\mathcal{K}$ là tập hợp các hàm $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$ có các tính chất sau: với mỗi hàm $f \in \mathcal{K}$ có một số hữu hạn các trường Hardy $\mathcal{K}_1, \mathcal{K}_2, \ldots, \mathcal{K}_n$ (số $n$ và các trường $\mathcal{K}_i$ phụ thuộc vào $f$) sao cho $f \in \mathcal{K}_n$ và, với $0 \leq i \leq n-1$, ta có $\mathcal{K}_{i+1} = \mathcal{K}_i(u_{i+1})$ trong đó $u_{i+1}$ bằng hoặc là $e^{z_i}$ hoặc là $\log |z_i|$ với $z_i$ thuộc $\mathcal{K}_i$ và không triệt tiêu đồng nhất trên một lân cận của $+\infty$. Người ta nói rằng $u_1, u_2, \ldots, u_n$ tạo thành một *dãy định nghĩa* cho trường $\mathcal{K}_n$ và cho hàm $f$; cùng một hàm dĩ nhiên có thể nhận nhiều dãy định nghĩa.

Theo định nghĩa 1 của V, p. 247, mọi hàm $f \in \mathcal{K}$, không đồng nhất bằng không trên một lân cận của $+\infty$, có dấu hằng và khả vi trên một khoảng $[x_0, +\infty[$; nếu $f \in \mathcal{K}_n$, thì $1/f$ và $f'$ bằng các hàm thuộc $\mathcal{K}_n$, do đó bằng các hàm thuộc $\mathcal{K}$, trên một lân cận của $+\infty$. Để thấy rằng $\mathcal{K}$ là một trường Hardy, chỉ cần chứng minh rằng nếu $f$ và $g$ là hai hàm thuộc $\mathcal{K}$ thì $f - g$ và $fg$ bằng các hàm thuộc $\mathcal{K}$ trên một lân cận của $+\infty$. Bây giờ cho $u_1, u_2, \ldots, u_m$ là một dãy định nghĩa của $f$, và $v_1, v_2, \ldots, v_n$ là một dãy định nghĩa của $g$. Dãy $u_1, u_2, \ldots, u_m, v_1, v_2, \ldots, v_n$ thu được bằng cách ghép các dãy $(u_i)$ và $(v_i)$ lại là một dãy định nghĩa của một trường Hardy $\mathcal{K}_{m+n}$ và trường này chứa $f$ và $g$, do đó $f - g$ và $fg$ bằng các hàm thuộc $\mathcal{K}_{m+n}$ trên một lân cận của $+\infty$.

Người ta nói rằng trường Hardy $\mathcal{K}$ được định nghĩa trong chứng minh của mệnh đề 3 là phép (H) *mở rộng* của trường Hardy $\mathcal{K}_0$.

Nếu $\mathcal{K}'$ là một trường Hardy khác có các tính chất đã nêu trong mệnh đề 3, thì từ phép dựng của $\mathcal{K}$ suy ra rằng $\mathcal{K}/\mathbf{R}_\sim$ được *chứa* trong $\mathcal{K}'/\mathbf{R}_\sim$. Do lạm dụng ngôn ngữ, người ta nói rằng phép mở rộng (H) của trường Hardy $\mathcal{K}_0$ là trường Hardy $\mathcal{K}$ *nhỏ nhất* có các tính chất này.

#### Định nghĩa 2 {#fvr-v-a0-def-2 .statement}

*Trường các hàm (H) được gọi là phép (H) mở rộng của trường Hardy $\mathbf{R}(x)$ gồm các hàm hữu tỉ với các hệ số thực. Mọi hàm thuộc phép mở rộng này được gọi là một hàm (H).*

Theo định nghĩa này, nếu $f$ là một hàm (H), không đồng nhất bằng không trên một lân cận của $+\infty$, thì $e^f$ và $\log |f|$ cũng là các hàm (H). Nói chung hơn, nếu $g$ là một hàm (H) thứ hai, và $u_1, u_2, \ldots, u_n$ là một dãy định nghĩa đối với $g$, và nếu $f(x)$ tiến tới $+\infty$ cùng với $x$, ta thấy bằng quy nạp theo $n$ rằng các hàm hợp $u_1 \circ f, u_2 \circ f, \ldots, u_n \circ f$ và $g \circ f$ là các hàm (H).

### 5. HÀM MŨ VÀ LÔGARIT LẶP

Ta đã định nghĩa (V, p. 229) các *lôgarit lặp* $l_n(x)$ bởi các điều kiện $l_0(x) = x, l_n(x) = \log(l_{n-1}(x))$ với $n \geq 1$. Tương tự, ta định nghĩa các *hàm mũ lặp* $e_n(x)$ bởi các điều kiện $e_0(x) = x, e_n(x) = \exp(e_{n-1}(x))$ với $n \geq 1$. Ngay lập tức, bằng quy nạp theo $n$, ta có rằng $l_n(x)$ là hàm nghịch đảo của $e_n(x)$, được xác định với $x > e_{n-1}(0)$, và rằng $e_m(e_n(x)) = e_{m+n}(x), l_m(l_n(x)) = l_{m+n}(x)$. Theo các hệ thức $\log x \ll x^\mu \ll e^x$ với mọi $\mu > 0$, ta có, với $n \geq 1$,

$$
l_n(x) \ll (l_{n-1}(x))^\mu \quad \text{với mọi } \mu > 0 \tag{5}
$$

$$
e_{n-1}(x^{1+\beta}) \ll e_n(x^{1+\delta}) \ll e_n((1-\gamma)x) \ll (e_n(x))^\mu
$$
$$
\ll e_n((1+\alpha)x) \ll e_n(x^{1+\beta}) \tag{6}
$$

với mọi $\mu > 0, \alpha > 0, \beta > 0, 0 < \gamma < 1, 0 < \delta < 1$, các số này là tùy ý nếu không có điều kiện nào khác (*xem* V, p. 218, Mệnh đề 11).

Ta đã thấy (V, p. 229) rằng, với $n \geq 1$, ta có

$$
\frac{d}{dx}(l_n(x)) = \prod_{i=0}^{n-1} \frac{1}{l_i(x)}. \tag{7}
$$

Tương tự với $n \geq 1$

$$
\frac{d}{dx}(e_n(x)) = \prod_{i=1}^n e_i(x). \tag{8}
$$

do đó, theo Mệnh đề 8 của V, p. 233, với mọi $\mu > 0$

$$
\int_a^x e_n(t^\mu) \, dt \sim \frac{x}{\mu} e_n(x^\mu) \prod_{i=0}^{n-1} \frac{1}{e_i(x^\mu)} \tag{9}
$$

$$
\int_x^{+\infty} \frac{dt}{e_n(t^\mu)} \sim \frac{x}{\mu} \prod_{i=0}^n \frac{1}{e_i(x^\mu)}. \tag{10}
$$

Có thể chứng minh rằng nếu $f$ là một hàm (H) *bất kỳ* sao cho $f \gg 1$ thì tồn tại hai số nguyên $m$ và $n$ sao cho

$$
l_m(x) \ll f(x) \ll e_n(x)
$$

(V, p. 263, bài tập 1 và p. 264, bài tập 5). Mặt khác, ta có thể định nghĩa các hàm tăng $g(x)$ (không còn là các hàm (H)) sao cho $g(x) \gg e_n(x)$ với *mọi* $n > 0$, hoặc $1 \ll g(x) \ll l_m(x)$ với *mọi* $m > 0$ (V, p. 265, bài tập 8, 9 và 10).

Với sự trợ giúp của các lôgarit lặp, ta sẽ chỉ ra rằng có thể định nghĩa một *thang so sánh* $\mathcal{E}$ (đối với $x$ tiến tới $+\infty$) gồm các hàm (H), dương $> 0$ trên một lân cận của $+\infty$ và thỏa mãn các điều kiện sau:

$a)$ tích của hai hàm bất kỳ trong $\mathcal{E}$ thuộc về $\mathcal{E}$;

$b)$ $f^\mu \in \mathcal{E}$ với mọi hàm $f \in \mathcal{E}$ và mọi số thực $\mu$;

c) với mọi hàm $f \in \mathcal{E}$, $\log f$ là một tổ hợp tuyến tính của một số hữu hạn các hàm trong $\mathcal{E}$;
d) với mọi hàm $f \in \mathcal{E}$, ngoài hằng 1, $e^f$ tương đương với một hàm trong $\mathcal{E}$.

Trước hết ta xét tập hợp $\mathcal{E}_0$ các hàm có dạng $\prod_{m=0}^{\infty} (l_m(x))^{\alpha_m}$, trong đó các $\alpha_m$ là các số thực, bằng không trừ ra với một số hữu hạn chỉ số $m$; hiển nhiên, từ (5) (V, p. 253) suy ra rằng các hàm này tạo thành một *thang so sánh* thỏa mãn các điều kiện $a), b)$ và $c)$. Bây giờ ta định nghĩa, bằng quy nạp theo $n$, tập hợp $\mathcal{E}_n$ (với $n \geqslant 1$) được tạo bởi hằng 1 và bởi các hàm có dạng $\exp \left( \sum_{k=1}^p a_k f_k \right)$, trong đó $p$ là một số nguyên tùy ý $> 0$, các hàm $f_k$ ($1 \leqslant k \leqslant p$) là các hàm trong $\mathcal{E}_{n-1}$ sao cho $f_1 \gg f_2 \gg \cdots \gg f_p \gg 1$, và các $a_k$ là các số thực $\neq 0$; ta chứng minh bằng quy nạp rằng $\mathcal{E}_n$ là một *thang so sánh* thỏa mãn $a), b)$ và $c)$ và chứa $\mathcal{E}_{n-1}$. Trước hết, quan hệ $\mathcal{E}_{n-1} \subset \mathcal{E}_n$ đúng với $n = 1$, vì logarit của mọi hàm không hằng trong $\mathcal{E}_0$ có dạng $\sum_{k=1}^p a_k f_k$, trong đó các $f_k$ là các logarit lặp, và do đó $\gg 1$; mặt khác, nếu $\mathcal{E}_{n-2} \subset \mathcal{E}_{n-1}$ thì từ định nghĩa của $\mathcal{E}_n$ suy ra $\mathcal{E}_{n-1} \subset \mathcal{E}_n$; định nghĩa này hơn nữa cho thấy rằng $\mathcal{E}_n$ thỏa mãn $a), b)$ và $c)$. Còn lại cần thấy rằng $\mathcal{E}_n$ là một thang so sánh: vì thương của hai hàm trong $\mathcal{E}_n$ lại thuộc về $\mathcal{E}_n$ nên chỉ cần chứng minh rằng mọi hàm $f$ của $\mathcal{E}_n$, ngoài hằng 1, không thể tương đương với một hằng $\neq 0$. Bây giờ ta có $\log f = \sum_{k=1}^p a_k f_k \sim a_1 f_1$ theo phép dựng, và vì $f_1 \gg 1$, $\log f$ tiến tới $\pm \infty$, do đó $f$ tiến tới 0 hoặc tới $+\infty$ khi $x$ tiến tới $+\infty$.

Nếu $\mathcal{E}$ là *hợp* của các $\mathcal{E}_n$ với $n \geqslant 0$, thì $\mathcal{E}$ là một thang so sánh, vì hai hàm trong $\mathcal{E}$ thuộc cùng một thang $\mathcal{E}_n$; vì cùng lý do đó, $\mathcal{E}$ thỏa mãn $a)$, và rõ ràng nó cũng thỏa mãn $b)$ và $c)$. Cuối cùng, nếu $f \in \mathcal{E}$ thì tồn tại một $n$ sao cho $f \in \mathcal{E}_n$; nếu $f$ không phải là hằng 1 thì $f(x)$ tiến tới 0 hoặc tới $+\infty$ khi $x$ tiến tới $+\infty$; trong trường hợp thứ nhất $e^f \sim 1$ và trong trường hợp thứ hai, $e^f$ thuộc $\mathcal{E}_{n+1}$ theo định nghĩa, và do đó thuộc $\mathcal{E}$.

#### Nhận xét {#fvr-v-a0-n5-rem-1 .statement}

Mặc dù có tính hữu dụng thực tiễn của thang $\mathcal{E}$ mà ta vừa định nghĩa, thật dễ dàng đưa ra các ví dụ về các hàm (H) *không có phần chính* đối với $\mathcal{E}$. Thật vậy, nếu $f$ là một hàm (H) sao cho $f \sim a g$, trong đó $a$ là một hằng số $> 0$ và $g \in \mathcal{E}$, thì $\log f - \log g - \log a$ tiến tới 0 cùng với $1/x$, do đó $\log f$ thừa nhận, đối với $\mathcal{E}$, một khai triển tiệm cận có *phần dư tiến tới 0*, theo tính chất $c)$. Bây giờ, nếu xét chẳng hạn hàm (H) $f(x) = e_2 \left( x + \frac{1}{x} \right)$ thì ta có $\log f(x) = \exp \left( x + \frac{1}{x} \right)$, do đó các khai triển tiệm cận của $\log f$ đối với $\mathcal{E}$ có dạng

$$
\log f(x) = e^x + \frac{e^x}{x} + \frac{1}{2!} \frac{e^x}{x^2} + \cdots + \frac{1}{n!} \frac{e^x}{x^n} + o \left( \frac{e^x}{x^n} \right) \quad (n \text{ một số nguyên } > 0).
$$

Rõ ràng phần dư trong khai triển này tương đương với $\frac{1}{(n+1)!} \frac{e^x}{x^{n+1}}$, nên không tiến tới 0. Vì vậy $f$ không có phần chính đối với $\mathcal{E}$.

Nếu $f$ là một hàm (H), thì $f$ là đơn điệu và liên tục trên một khoảng $[x_0, +\infty[$, do đó hàm ngược $\varphi$ của hạn chế của $f$ trên khoảng này là đơn điệu và liên tục trên một lân cận của điểm $a = \lim_{x \to +\infty} f(x)$; nhưng, nếu $a$ bằng $+\infty$ (resp. $-\infty$, hữu hạn), ta có thể chỉ ra rằng $\varphi(y)$ (resp. $\varphi(-y)$, $\varphi \left( a + \frac{1}{y} \right)$ hoặc $\varphi \left( a - \frac{1}{y} \right)$) nói chung không bằng một hàm (H) trên một lân cận của $+\infty$. Tuy nhiên ta sẽ thấy rằng trong một số trường hợp quan trọng có thể thu được một hàm (H) tương đương với $\varphi(y)$ (resp. $\varphi(-y)$, $\varphi \left( a + \frac{1}{y} \right)$, $\varphi \left( a - \frac{1}{y} \right)$) và đôi khi thậm chí một khai triển tiệm cận của hàm này đối với thang $\mathcal{E}$ được định nghĩa trong V, p. 254.

Ta sẽ sử dụng mệnh đề sau:

#### Mệnh đề 4 {#fvr-v-a0-prop-4 .statement}

Cho $p$ và $q$ là hai hàm (H) dương ngặt trên một khoảng $[x_0, +\infty[$.

1° Nếu $q \ll p/p'$ thì có $p(x + q(x)) \sim p(x)$.
2° Nếu cả $q \ll p/p'$ và $q(x) \ll x$ thì có $p(x - q(x)) \sim p(x)$.

Hai phần của mệnh đề này là hiển nhiên nếu $p \sim k$ (hằng $\neq 0$); do đó có thể giả sử rằng $p(x) \ll 1$ (nếu không thì áp dụng lập luận cho $1/p$). Khi đó suy ra $p'(x) \ll 1$.

1° Có thể viết $p(x + q(x)) = p(x) + q(x)p'(x + \theta q(x))$ với $0 \leq \theta \leq 1$ (I, p. 14, hệ quả). Vì $|p'(x)|$ tiến tới 0 khi $x$ tiến tới $+\infty$, và bằng một hàm (H) trên một lân cận của $+\infty$, nên nó giảm trên một khoảng $[x_1, +\infty[$, do đó, với $x \geq x_1$, ta có $|p'(x + \theta q(x))| \leq |p'(x)|$; vì $qp' \ll p$ nên có $p(x + q(x)) \sim p(x)$.

2° Điều kiện $q(x) \ll x$ đảm bảo rằng $x - q(x)$ tiến tới $+\infty$ cùng với $x$. Một lần nữa ta có $p(x - q(x)) = p(x) - q(x)p'(x - \theta p(x))$ với $0 \leq \theta \leq 1$. Cùng lập luận như trong phần thứ nhất của chứng minh cho thấy rằng, với $x$ đủ lớn, $|p'(x - \theta q(x))| \leq |p'(x - q(x))|$. Nó quy về việc chứng minh rằng $q(x) \frac{p'(x - q(x))}{p(x - q(x))}$ tiến tới 0 khi $x$ tiến tới $+\infty$. Mệnh đề đúng nếu $p'/p \gg 1$ vì khi đó $|p'/p|$ là một hàm (H), tăng khi $x$ đủ lớn; do đó $q(x) \frac{|p'(x - q(x))|}{|p(x - q(x))|} \leq q(x) \frac{|p'(x)|}{|p(x)|}$, và $qp' \ll p$ theo giả thiết. Nó cũng đúng nếu $p'/p \sim k$ ($k$ hằng $\neq 0$), vì khi đó

$$
\frac{p'(x - q(x))}{p(x - q(x))} \sim \frac{p'(x)}{p(x)}
$$

vì $x - q(x)$ tiến tới $+\infty$. Chỉ còn phải xét trường hợp $p'/p \ll 1$. Trước hết giả sử rằng $p(x)$ có cấp *hữu hạn* đối với $x$, và do đó (V, p. 232, prop. 7) $p'(x)/p(x) \ll 1/x$. Khi đó ta có
$$
\frac{p'(x-q(x))}{p(x-q(x))} = \frac{1}{x-q(x)} O_1(1),
$$
do đó
$$
q(x) \frac{p'(x-q(x))}{p(x-q(x))} = \frac{q(x)}{x} \left( 1 - \frac{q(x)}{x} \right)^{-1} O_1(1) = \frac{q(x)}{x} O_2(1),
$$
và ta thấy trong trường hợp này mệnh đề đúng chỉ *với giả thiết duy nhất* rằng $q(x) \ll x$. Cuối cùng ta xét trường hợp $1/x \ll p'(x)/p(x) \ll 1$; hàm $r = p'/p$ khi đó có cấp hữu hạn đối với $x$; vì, theo nhận xét trước đó, mệnh đề 4 của V, p. 255, áp dụng được cho một hàm như vậy, ta có $p'(x-q(x))/p(x-q(x)) \sim p'(x)/p(x)$, và giả thiết $qp' \ll p$ cho phép ta hoàn thành chứng minh.

#### Nhận xét {#fvr-v-a0-n6-rem-3 .statement}

Các điều kiện đặt ra cho $q(x)$ có thể không được cải thiện, như các ví dụ sau đây cho thấy:

a)
$$
p(x) = e^x, \quad q(x) = 1 = \frac{p(x)}{p'(x)}, \quad p(x+q(x)) = ep(x)
$$

b)
$$
p(x) = \log x, \quad q(x) = x - \log x \ll \frac{p(x)}{p'(x)} = x \log x,
$$
$$
p(x-q(x)) = \log \log x \ll p(x).
$$

Trước hết ta sẽ nghiên cứu các hàm nghịch đảo của các hàm (H) thuộc một loại đặc biệt:

#### Mệnh đề 5 {#fvr-v-a0-prop-5 .statement}

*Cho g là một hàm* (H) *không tương đương với một hằng $\neq 0$, và sao cho* $g(x) \ll x$, *và cho* $u(x)$ *là hàm nghịch đảo của* $x - g(x)$, *được xác định trên một lân cận của* $+\infty$. *Cho* $(u_n)$ *là dãy các hàm được xác định, bằng quy nạp theo* $n$, *bởi các điều kiện* $u_0(x) = x$, $u_n(x) = x + g(u_{n-1}(x))$ *với* $n \geqslant 1$; *khi đó* $u_n \gg 1$ *và*
$$
u(x) - u_n(x) \sim g(x)(g'(x))^n.
$$ (11)

Đặt $y = u(x)$, $y_n = u_n(x)$; khi đó $x = y - g(y)$, $y_0 = x$ và $y_n = x + g(y_{n+1})$. Trước hết ta suy ra rằng $x/y = 1 - \frac{g(y)}{y}$; vì $y$ tiến tới $+\infty$ cùng với $x$, giả thiết $g(x) \ll x$ cho thấy rằng $y = u(x) \sim x = y_0$; hơn nữa,
$$
y - x = g(y) = g(x) + (y - x)g'(z)
$$
trong đó $z$ thuộc khoảng có hai đầu mút là $x, y$; khi $x$ tiến tới $+\infty$ thì $z$ cũng vậy, và vì $g(x) \ll x$, $g' \ll 1$, do đó $g'(z)$ tiến tới 0, và do đó
$$
y - x = g(x) + o(y - x)
$$

do đó
$$
u(x) - x \sim g(x).
$$
(12)

Thứ hai, ta chứng minh, bằng quy nạp theo $n$, rằng khi $x$ tiến tới $+\infty$ thì có $u_n \gg 1$, và
$$
u(x) - u_n(x) \ll u(x) - u_{n-1}(x).
$$
(13)

Thật vậy, $y - y_n = g(y) - g(y_{n-1}) = (y - y_{n-1})g'(z_{n-1})$, trong đó $z_{n-1}$ thuộc khoảng có hai đầu mút là $y$ và $y_{n-1}$; theo giả thiết quy nạp $z_{n-1}$ tiến tới $+\infty$ cùng với $x$, và do đó $g'(z_{n-1})$ tiến tới 0, điều này chứng minh (13). Từ quan hệ này và từ (12) ta suy ra rằng $u(x) - u_n(x) \ll u(x) - x \sim g(x) \ll x \sim u(x)$, do đó $u_n(x) \sim u(x)$ và do đó $u_n \gg 1$. Cuối cùng, quan hệ $u(x) - u_n(x) \ll u(x) - x$ cũng có thể được viết là $(u(x) - x) - (u_n(x) - x) \ll u(x) - x$, do đó
$$
u_n(x) - x \sim u(x) - x \sim g(x).
$$
(14)

Để chứng minh (11), trước hết nhận xét rằng nếu $t(x)$ là một hàm sao cho $t(x) - x \sim g(x)$, thì ta có $g'(t(x)) \sim g'(x)$. Thật vậy, với mọi $\varepsilon > 0$, khi $x$ đủ lớn thì $g'$ đơn điệu, do đó $g'(t(x))$ nằm giữa $g'(x + (1 + \varepsilon)g(x))$ và $g'(x + (1 - \varepsilon)g(x))$. Mệnh đề 4 của V, p. 255, chỉ ra rằng $g'(t(x)) \sim g'(x)$, với điều kiện đã thiết lập quan hệ $g \ll g'/g''$. Bây giờ, nếu $g$ có cấp vô hạn đối với $x$ thì ta có (V, p. 251, mệnh đề 2) $g''/g' \sim g'/g$, và, vì $g' \ll 1, g \ll g/g' \sim g'/g''$; nếu $g$ có cấp hữu hạn $\mu$ đối với $x$ thì nhất thiết có $\mu \leq 1$; nếu $\mu < 1$, vì $g$ không tương đương với một hằng số $\neq 0$, các công thức (3) và (4) (V, p. 251) chỉ ra rằng $g''/g' \sim k/x$ ($k$ hằng $\neq 0$), do đó lại có $g \ll g'/g''$; cuối cùng, nếu $\mu = 1$ thì $g'$ có cấp 0 đối với $x$, nên $g''/g' \ll 1/x$, và do đó lại có $g \ll g'/g''$.

Điều này đã được chứng minh, vì $z_{n-1}$ nằm giữa $y$ và $y_n$, từ (14) suy ra rằng $z_{n-1} - x \sim g(x)$, do đó $g'(z_{n-1}) \sim g'(x)$ theo kết quả trên; vậy
$$
y - y_n \sim (y - y_{n-1})g'(x),
$$
do đó ta thu được (11) bằng quy nạp theo $n$.

#### Nhận xét 1 {#fvr-v-a0-n6-rem-1 .statement}

Nếu $g$ có cấp $< 1$ đối với $x$, hàm $u(x) - u_n(x)$ tiến về 0 theo $x$ một khi $n$ đủ lớn. Thật vậy, trong trường hợp đối, ta sẽ có ${gg''}^n \gg 1$ với mọi $n$, do đó $g$ sẽ có cấp vô hạn đối với $1/g'$; nói cách khác, ta sẽ có $\log|g| \gg \log|g'|$, do đó, khi lấy đạo hàm, $g'/g \gg g''/g'$. Nhưng nếu $g$ có cấp $\mu < 1$ đối với $x$ thì ta có $g'/g \sim g''/g'$ khi $\mu = -\infty, \frac{g'}{g} \sim \frac{\mu}{\mu - 1} \frac{g''}{g'}$ khi $\mu \neq 0$, và cuối cùng $g'/g \ll g''/g'$ khi $\mu = 0$ (V, p. 251, n 3).

Trái lại, nếu $g$ có cấp 1 đối với $x$ thì có thể có ${gg''}^n \gg 1$ với mọi số nguyên $n > 0$, như ví dụ $g(x) = x/\log x$ chỉ ra.

#### Nhận xét 2 {#fvr-v-a0-n6-rem-2 .statement}

Khi $g(x)$ là một hàm (H) tương đương với một hằng $k \neq 0$ ta có $g(x) = k + g_1(x)$, với $g_1 \ll 1$; hàm $u_1(x) = u(x) - k$ là nghịch đảo của hàm $x - g_1(x + k)$, và ta được đưa trở lại trường hợp đã xét trong prop. 5 của V, p. 256.

Để có một khai triển tiệm cận cho hàm $u$ thì chỉ cần có một khai triển như vậy cho hàm $u_n$: nếu $g$ thừa nhận một khai triển tiệm cận đối với thang đang xét thì do đó ta được dẫn đến (theo định nghĩa của các hàm (H)) các bài toán đã khảo sát trong V, p. 223 đến 227.

Trường hợp tổng quát nhất, như sau đây, quy về trường hợp đã xét trong prop. 5 của V, p. 256: hàm $y = u(x)$ được giả sử thỏa mãn quan hệ
$$
\varphi(x) = \psi(y) - g(y)
$$
trong đó $\varphi$ là một hàm (H), $\psi$ là một hàm (H) sao cho $\psi \gg 1$ và sao cho hàm nghịch đảo $\theta$ của $\psi$ cũng là một hàm (H), và $g$ là một hàm (H) sao cho $g \ll \psi$. Bây giờ cho $v(x)$ là hàm nghịch đảo của $x - g(\theta(x))$; ta có $u = \theta \circ v \circ \varphi$, và $g(\theta(x)) \ll x$; nếu biết một khai triển tiệm cận của $v$ nhờ prop. 5 của V, p. 256, thì khi đó ta có thể suy ra một khai triển tiệm cận của $u$ như trong V, p. 223 đến 227.

#### Ví dụ 1 {#fvr-v-a0-n6-exa-1 .statement}

Ta tìm một khai triển tiệm cận cho hàm nghịch đảo $v(x)$ của $x^5 + x$ (khi $x$ tiến tới $+\infty$); đặt $x^5 = t$ ta được dẫn đến việc tìm một khai triển của hàm nghịch đảo $u(t)$ của $t + t^{1/5}$ (khi $t$ tiến tới $+\infty$), nghĩa là áp dụng prop. 5 của V, p. 256, cho trường hợp $g(t) = -t^{1/5}$. Chẳng hạn, ta tính, $u_2(t)$; ta có
$$
u_2(t) = t - \left( t - t^{1/5} \right)^{1/5} = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{2}{25} t^{-7/5} + o_1\left( t^{-7/5} \right).
$$
Hơn nữa, theo (11) (V, p. 256)
$$
u(t) - u_2(t) \sim -\frac{1}{25} t^{-7/5}
$$
do đó
$$
u(t) = t - t^{1/5} + \frac{1}{5} t^{-3/5} + \frac{1}{25} t^{-7/5} + o_2\left( t^{-7/5} \right)
$$
và ta suy ra khai triển
$$
v(x) = u(x)^{1/5} = x^{1/5} - \frac{1}{5} x^{-3/5} - \frac{1}{25} x^{-7/5} + o_3\left( x^{-7/5} \right)
$$
cần tìm.

#### Ví dụ 2 {#fvr-v-a0-n6-exa-2 .statement}

Ta tìm một khai triển tiệm cận cho hàm nghịch đảo của hàm $x / \log x$; từ đẳng thức $x = y / \log y$, trong đó $y = v(x)$, ta suy ra $\log x = \log y - \log \log y$; đặt $z = \log y, t = \log x$, ta có $t = z - \log z$, và ta được dẫn đến việc khai triển hàm nghịch đảo $u(t)$ của $t - \log t$; chẳng hạn, ta có
$$
u_2(t) = t + \log(t + \log t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + o_1\left( \frac{\log t}{t^2} \right)
$$
và hơn nữa, theo (11) (V, p. 256)
$$
u(t) - u_2(t) \sim \frac{\log t}{t^2}
$$
do đó
$$
u(t) = t + \log t + \frac{\log t}{t} - \frac{(\log t)^2}{2t^2} + \frac{\log t}{t^2} + o_2\left( \frac{\log t}{t^2} \right)
$$
và khi trở lại bài toán ban đầu ta thu được khai triển tiệm cận
$$
v(x) = x \log x + x \log \log x + x \frac{\log \log x}{\log x} + o\left( x \frac{\log \log x}{\log x} \right).
$$

#### Nhận xét {#fvr-v-a0-n6-rem-4 .statement}

Chú ý rằng hai hàm (H) tương đương có thể có các hàm nghịch đảo không tương đương, như ví dụ của hai hàm $\log x$ và $1 + \log x$ chỉ ra.

### Bài tập {#fvr-v-a0-exercises}

Xem các [bài tập cho Phụ lục 0](exercises/a0/).
