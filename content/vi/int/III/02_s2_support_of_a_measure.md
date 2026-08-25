---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 2
section_title: Support of a measure
lang: vi
source: int-i-vi
book_pages: INT III.23-INT III.32, INT III.59
pdf_pages: 0068-0077, 0104-0104
extraction: ocr
subsections:
    - "no": 1
      title: Restriction of a measure to an open set. Definition of a measure by means of local data
      page: 23
      pdf_page: 68
    - "no": 2
      title: Support of a measure
      page: 25
      pdf_page: 70
    - "no": 3
      title: Characterization of the support of a measure
      page: 27
      pdf_page: 72
    - "no": 4
      title: Point measures. Measures with finite support
      page: 29
      pdf_page: 74
    - "no": 5
      title: Discrete measures
      page: 31
      pdf_page: 76
statements: 26
exercises: 5
content_sha256: e1e19c5e078b767489bd930878b27fee21549c1b017474a7918650ae465a2dfc
translated_from: content/en/int/III/02_s2_support_of_a_measure.md
source_content_sha256: 742b186e2510b4cb080d732e55d0627d911b41a8ad1e76045df65adb4c5281c3
translation_model: gpt-5.4
translation_run: translate-vi-8186ee89
glossary_version: 34
glossary_terms_sha256: e5fa5acd67fe57c5b9ae1a870352440fd2be411d509633e6514203f29607cc5a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. GIÁ CỦA MỘT ĐỘ ĐO

### 1. Hạn chế của một độ đo trên một tập mở. Định nghĩa một độ đo bằng dữ kiện địa phương

Cho X là một không gian compact địa phương, Y là một tập hợp mở trong X. Không gian con Y của X là compact địa phương, và mọi hàm liên tục nhận giá trị trong một không gian vectơ tôpô E, được xác định trên Y và có giá compact, đều có thể được mở rộng bằng tính liên tục ra toàn bộ X, bằng cách cho nó giá trị 0 trên $\mathbf{C}Y$; do đó có thể đồng nhất theo cách này không gian $\mathcal{K}(Y;E)$ với không gian con tuyến tính của $\mathcal{K}(X;E)$ gồm các hàm liên tục có giá compact *được chứa trong* Y. Nếu $\mu$ là một độ đo trên X, thì hiển nhiên hạn chế của $\mu$ lên $\mathcal{K}(Y;\mathbf{C})$ là một độ đo trên Y, được gọi là *hạn chế* của $\mu$ lên không gian con mở Y, hoặc độ đo *cảm sinh* trên Y bởi $\mu$, và được ký hiệu là $\mu|Y$. Các hạn chế lên Y của $|\mu|$, $\mathcal{R}\mu$ và $\mathcal{I}\mu$ lần lượt là $|\mu|Y|$, $\mathcal{R}(\mu|Y)$ và $\mathcal{I}(\mu|Y)$, theo §1, Nos. 5 and 6. Nếu $\mu$ là thực thì các hạn chế của $\mu^+$ và $\mu^-$ lên Y lần lượt là $(\mu|Y)^+$ và $(\mu|Y)^-$, theo công thức (8) của §1, No. 5.

Ta thấy ngay lập tức rằng nếu Y và Z là hai tập mở trong X sao cho $Y \supset Z$, và nếu $\mu|Y$ và $\mu|Z$ là các hạn chế của $\mu$ lên Y và Z, thì $\mu|Z$ cũng là hạn chế của $\mu|Y$ lên không gian con mở Z của không gian compact địa phương Y.

Trong Ch. IV, §5, No. 7, chúng tôi sẽ tổng quát hóa định nghĩa này cho trường hợp Y là một không gian con compact địa phương của X.

Chú ý rằng một số đo trên Y *không nhất thiết* là hạn chế của một số đo nào đó trên X (xem Ch. V, §7, No. 2, Mệnh đề 3).

Ví dụ, lấy Y là khoảng mở ]0,1[ của $X = \mathbf{R}$; ánh xạ

$$
f \mapsto \int_0^1 \frac{f(x)}{x} dx
$$

là một số đo trên $Y$, vì mọi hàm trong $\mathcal{K}(Y; \mathbf{C})$ đều bằng không trên một lân cận của 0 trong $\mathbf{R}$. Tuy nhiên, số đo này không thể được mở rộng thành một số đo trên $\mathbf{R}$ vì, trong trường hợp ngược lại, hạn chế của nó lên tập hợp các hàm $f \in \mathcal{K}(Y; \mathbf{C})$ sao cho $\|f\| \leq 1$ sẽ bị chặn; nhưng điều này là sai.

Tuy nhiên, ta có mệnh đề sau:

#### Mệnh đề 1 {#int-iii-s2-prop-1 .statement}

*Cho* $(Y_\alpha)_{\alpha \in A}$ *là một phủ mở của* $X$ *và giả sử trên mỗi không gian con* $Y_\alpha$, *đã cho một độ đo* $\mu_\alpha$, *sao cho với mọi cặp* $(\alpha, \beta)$, *các hạn chế của* $\mu_\alpha$ *và* $\mu_\beta$ *trên* $Y_\alpha \cap Y_\beta$ *là đồng nhất. Trong các điều kiện đó, tồn tại một và chỉ một độ đo* $\mu$ *trên* $X$ *mà hạn chế của nó trên* $Y_\alpha$ *bằng* $\mu_\alpha$ *với mọi chỉ số* $\alpha$.

Trước hết hãy chỉ ra rằng mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$ đều có thể viết dưới dạng một tổng hữu hạn $f = \sum_i f_i$ trong đó, với mỗi hàm $f_i \in \mathcal{K}(X; \mathbf{C})$, tồn tại một chỉ số $\alpha_i$ sao cho $\operatorname{Supp}(f_i) \subset Y_{\alpha_i}$. Nếu $K = \operatorname{Supp}(f)$, thì tồn tại một số hữu hạn chỉ số $\alpha_i$ ($1 \leq i \leq n$) sao cho các $Y_{\alpha_i}$ lập thành một phủ của $K$; gọi $h_i$ ($1 \leq i \leq n$) là các ánh xạ liên tục từ $X$ vào $[0, 1]$ sao cho giá của $h_i$ là compact và được chứa trong $Y_{\alpha_i}$ với $1 \leq i \leq n$, và sao cho $\sum_{i=1}^n h_i(x) = 1$ trên $K$ (\S 1, No. 2, Bổ đề 1); các hàm $f_i = f h_i$ thỏa mãn các yêu cầu. Điều này trước hết cho thấy rằng nếu tồn tại một độ đo $\mu$ thỏa mãn các yêu cầu thì nó là *duy nhất*, bởi vì với mọi tổng hữu hạn $f = \sum_{i=1}^n f_i$, trong đó $f_i \in \mathcal{K}(Y_{\alpha_i}; \mathbf{C})$, tất yếu có $\mu(f) = \sum_{i=1}^n \mu_{\alpha_i}(f_i)$. Hơn nữa, ta sẽ chứng minh được sự tồn tại của một dạng tuyến tính $\mu$ trên $\mathcal{K}(X; \mathbf{C})$ mà hạn chế của nó trên mỗi không gian con $\mathcal{K}(Y_\alpha; \mathbf{C})$ là $\mu_\alpha$, miễn là ta chứng minh được tính chất sau đây: nếu $(g_i)_{1 \leq i \leq m}$ và $(h_j)_{1 \leq j \leq n}$ là hai dãy hữu hạn các hàm trong $\mathcal{K}(X; \mathbf{C})$ sao cho $g_i \in \mathcal{K}(Y_{\alpha_i}; \mathbf{C})$ với $1 \leq i \leq m$, $h_j \in \mathcal{K}(Y_{\beta_j}; \mathbf{C})$ với $1 \leq j \leq n$ và
$$
\sum_{i=1}^m g_i(x) = \sum_{j=1}^n h_j(x) = 1
$$
trên $K$, thì
$$
\sum_{i=1}^m \mu_{\alpha_i}(f g_i) = \sum_{j=1}^n \mu_{\beta_j}(f h_j).
$$
Bây giờ,
$$
f g_i = \sum_{j=1}^n f g_i h_j,
$$

do đó
$$
\sum_{i=1}^{m} \mu_{\alpha_i}(f g_i) = \sum_{i=1}^{m} \sum_{j=1}^{n} \mu_{\alpha_i}(f g_i h_j).
$$
Tương tự,
$$
\sum_{j=1}^{n} \mu_{\beta_j}(f h_j) = \sum_{j=1}^{n} \sum_{i=1}^{m} \mu_{\beta_j}(f g_i h_j).
$$
Nhưng vì giá đỡ của $f g_i h_j$ được chứa trong $Y_{\alpha_i} \cap Y_{\beta_j}$, ta có $\mu_{\alpha_i}(f g_i h_j) = \mu_{\beta_j}(f g_i h_j)$, điều này thiết lập mệnh đề của chúng ta.

Còn lại là thấy rằng $\mu$ là một độ đo trên $X$; nay, mọi điểm của $X$ đều thừa nhận một lân cận compắc được chứa trong một trong các $Y_\alpha$; do đó kết luận suy ra ngay từ định nghĩa của $\mu$ và từ Mệnh đề 6 của §1, No. 3.

**Hệ quả (Nguyên lý địa phương hóa).** — *Cho $\mu$ và $\nu$ là hai độ đo trên $X$, và cho $(Y_\alpha)$ là một họ các tập mở của $X$ sao cho, với mọi $\alpha$, các hạn chế trên $Y_\alpha$ của $\mu$ và $\nu$ là bằng nhau; khi đó các hạn chế của $\mu$ và $\nu$ trên $Y = \bigcup_\alpha Y_\alpha$ là bằng nhau.*

### 2. Giá của một độ đo

Cho $\mu$ là một độ đo trên một không gian địa phương compact $X$, và gọi $\mathcal{G}$ là tập hợp các tập mở $U \subset X$ sao cho hạn chế của $\mu$ lên $U$ là không; suy ra ngay từ nguyên lý địa phương hóa (No. 1, Hệ quả của Mệnh đề 1) rằng nếu $U_0$ là hợp của các tập $U \in \mathcal{G}$, thì chính $U_0$ cũng thuộc $\mathcal{G}$ và do đó là lớn nhất trong các tập thuộc $\mathcal{G}$.

#### Định nghĩa 1 {#int-iii-s2-def-1 .statement}

*Nếu $\mu$ là một độ đo trên một không gian địa phương compact $X$, người ta định nghĩa giá đỡ của $\mu$, ký hiệu là $\operatorname{Supp}(\mu)$, là tập hợp đóng bù với tập hợp lớn nhất trong các tập hợp mở của $X$ mà trên đó hạn chế của $\mu$ bằng không.*

Nói rằng một điểm $x \in X$ không thuộc giá đỡ của $\mu$ có nghĩa là tồn tại một lân cận mở $V$ của $x$ sao cho hạn chế của $\mu$ trên $V$ bằng không; vì thế, nói rằng $x$ thuộc giá đỡ của $\mu$ có nghĩa là với *mọi* lân cận $V$ của $x$, tồn tại một hàm $f \in \mathcal{K}(X; \mathbf{C})$, có giá đỡ được chứa trong $V$, sao cho $\mu(f) \neq 0$.

#### Ví dụ {#int-iii-s2-n2-exa-1 .statement}

— 1) Để một độ đo trên $X$ là *không*, điều kiện cần và đủ là giá mang của nó *rỗng*.
2) Giá mang của độ đo Lebesgue trên $\mathbf{R}$ là toàn bộ đường thẳng $\mathbf{R}$; vì nó khác rỗng và bất biến dưới mọi phép tịnh tiến.

3) Trên khoảng $X = [0,1]$ của $\mathbf{R}$, xét một tập con trù mật đếm được, được sắp thành một dãy $(a_n)$, và gọi $\mu$ là độ đo được xác định bằng cách đặt khối lượng $2^{-n}$ tại điểm $a_n$ với mọi $n \geq 0$ (\$1, No. 3, Ví dụ I). Giá của $\mu$ là toàn bộ $X$; thật vậy, cho $x$ là một điểm bất kỳ của $X$, $V$ là một lân cận của $x$, và $f$ là một hàm thực liên tục $\geq 0$ trên $X$, bằng 1 tại điểm $x$, mà giá được chứa trong $V$ (\$1, No. 2, Bổ đề 1); tập hợp các $y \in V$ sao cho $f(y) > 0$ là mở trong $X$, vì thế chứa một điểm $a_n$, do đó $\mu(f) \geq f(a_n)2^{-n} > 0$.

#### Mệnh đề 2 {#int-iii-s2-prop-2 .statement}

*Giá của một độ đo $\mu$ trùng với giá của độ đo $|\mu|$; nếu $\mu$ là thực, thì giá của nó là hợp của các giá của các độ đo $\mu^+$ và $\mu^-$.*

Thật vậy, nếu hạn chế của $\mu$ trên một tập mở $U$ là không, thì hạn chế của $|\mu|$ cũng vậy (tương ứng của $\mu^+$ và $\mu^-$ khi $\mu$ là thực), và ngược lại.

Chú ý rằng các giá của $\mu^+$ và $\mu^-$ có thể khác rỗng và *trùng nhau* (xem Ch. V, § 5, Exer. 5).

#### Mệnh đề 3 {#int-iii-s2-prop-3 .statement}

*Nếu $\mu$ và $\nu$ là hai độ đo trên một không gian compact địa phương $X$ sao cho $|\mu| \leq |\nu|$, thì $\mathrm{Supp}(\mu) \subset \mathrm{Supp}(\nu)$.*

Thật vậy, nếu hạn chế của $\nu$ trên một tập mở bằng không, thì hạn chế của $\mu$ cũng vậy.

#### Mệnh đề 4 {#int-iii-s2-prop-4 .statement}

*Giá của tổng của hai độ đo được chứa trong hợp các giá của chúng.*

Thật vậy, nếu các hạn chế của hai độ đo trên một tập mở đều bằng không, thì điều tương tự cũng đúng với hạn chế của tổng của chúng.

Nếu $\mu$ và $\nu$ là hai độ đo *dương*, thì giá của $\lambda = \mu + \nu$ là *bằng* hợp của các giá của $\mu$ và $\nu$; thật vậy, nếu $x_0$ là một điểm của hợp ấy và $V$ là một lân cận bất kỳ của $x_0$, thì tồn tại một hàm liên tục $f \geq 0$ có giá được chứa trong $V$ và sao cho một trong hai số $\mu(f)$, $\nu(f)$ là $> 0$; *a fortiori*, $\lambda(f) = \mu(f) + \nu(f) > 0$.

#### Mệnh đề 5 {#int-iii-s2-prop-5 .statement}

*Giá của hạn chế của một độ đo $\mu$ lên một tập mở $U$ là vết trên $U$ của giá của $\mu$.*

Mệnh đề là hiển nhiên từ các định nghĩa.

#### Mệnh đề 6 {#int-iii-s2-prop-6 .statement}

*Tập hợp các độ đo trên một không gian compact địa phương $X$, mà giá của chúng được chứa trong một tập đóng $F$, là một không gian con tuyến tính đóng theo tôpô mờ của $\mathcal{M}(X; \mathbf{C})$.*

Thật vậy, đó là giao của các siêu phẳng đóng theo tôpô mờ có phương trình $\mu(f) = 0$, trong đó $f$ chạy qua tập hợp các hàm trong $\mathcal{H}(X; \mathbf{C})$ mà giá của chúng không giao với $F$.

Giả sử $X$ *không compact*: với một bộ lọc $\Phi$ trên không gian $\mathcal{M}(X; \mathbf{C})$ các độ đo trên $X$, ta sẽ nói rằng giá của một độ đo $\mu$ *lùi ra vô hạn dọc theo* $\Phi$ nếu, với mọi tập con compact $K$ của $X$, tồn tại một tập $M \in \Phi$ sao cho $\mathrm{Supp}(\mu) \cap K = \varnothing$ đối với mọi độ đo $\mu \in M$.

#### Mệnh đề 7 {#int-iii-s2-prop-7 .statement}

— *Nếu $\Phi$ là một bộ lọc trên $\mathcal{M}(X; \mathbf{C})$ sao cho giá của $\mu$ lùi ra vô hạn dọc theo $\Phi$, thì $\mu$ hội tụ mơ hồ đến 0 theo $\Phi$.*

Cho $f$ là một hàm bất kỳ trong $\mathcal{K}(X; \mathbf{C})$ và $K$ là giá của nó. Theo giả thiết, tồn tại một tập hợp $M \in \Phi$ sao cho với mọi độ đo $\mu \in M$, $\operatorname{Supp}(\mu) \cap K = \varnothing$; suy ra $\mu(f) = 0$ với mọi $\mu \in M$, điều này chứng minh mệnh đề.

### 3. Đặc trưng hóa của giá của một độ đo

Theo định nghĩa, nếu giá của một hàm $f \in \mathcal{K}(X; \mathbf{C})$ *không giao* giá của một độ đo $\mu$, thì $\mu(f) = 0$; nhưng kết quả chính xác hơn sau đây là đúng:

#### Mệnh đề 8 {#int-iii-s2-prop-8 .statement}

— *Cho $\mu$ là một độ đo trên một không gian compact địa phương $X$. Với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$ bằng không trên $\operatorname{Supp}(\mu)$, ta có $\mu(f) = 0$.*

Đặt $K = \operatorname{Supp}(f)$, $S = \operatorname{Supp}(\mu)$. Cho một số $\varepsilon > 0$, gọi $V$ là tập hợp các $x \in X$ sao cho $|f(x)| < \varepsilon$; $V$ là một tập mở chứa $S$ theo giả thiết, do đó $CS$ là một lân cận của tập compact $CV$. Suy ra tồn tại một ánh xạ liên tục $h$ từ $X$ vào $[0, 1]$, bằng 1 trên $CV$ và có giá được chứa trong $CS$ (\S 1, No. 2, Bổ đề 1). Vì giá của $fh$ không giao với $S$ nên $\mu(fh) = 0$. Mặt khác, $f = fh$ trên $K \cap CV$, và $|fh| \leq |f|$ trên $X$, do đó $|f - fh| \leq 2\varepsilon$ trên $X$, bởi lựa chọn $V$. Cuối cùng, nhận thấy rằng tồn tại một số $M_K$ sao cho $|\mu(g)| \leq M_K \|g\|$ với mọi hàm $g \in \mathcal{K}(X; \mathbf{C})$ mà giá của nó được chứa trong $K$; vì giá của $f - fh$ được chứa trong $K$, nên $|\mu(f - fh)| \leq 2M_K \varepsilon$ và do đó $|\mu(f)| = |\mu(f - fh)| \leq 2M_K \varepsilon$; vì $\varepsilon$ là tùy ý, $\mu(f) = 0$.

#### Hệ quả 1 {#int-iii-s2-prop-8-cor-1 .statement}

— *Nếu hai hàm $f, g$ trong $\mathcal{K}(X; \mathbf{C})$ bằng nhau trên $\operatorname{Supp}(\mu)$, thì $\mu(f) = \mu(g)$.*

#### Hệ quả 2 {#int-iii-s2-prop-8-cor-2 .statement}

— *Cho $\mu$ là một độ đo dương trên $X$; nếu $f \in \mathcal{K}(X; \mathbf{C})$ sao cho $f(x) \geq 0$ trên $\operatorname{Supp}(\mu)$, thì $\mu(f) \geq 0$.*

Quả vậy, $f = |f|$ trên $\operatorname{Supp}(\mu)$, do đó $\mu(f) = \mu(|f|) \geq 0$ theo Hệ quả 1.

#### Hệ quả 3 {#int-iii-s2-prop-8-cor-3 .statement}

— *Giả sử $\mu$ là một độ đo bị chặn trên $X$; nếu $f \in \mathcal{K}(X; \mathbf{C})$ sao cho $|f(x)| \leq a$ trên $\operatorname{Supp}(\mu)$, thì $|\mu(f)| \leq a \|\mu\|$.*

Thật vậy, $\operatorname{Supp}(|\mu|) = \operatorname{Supp}(\mu)$, và nếu $h$ là một ánh xạ liên tục từ $X$ vào $[0, 1]$, bằng 1 trên $\operatorname{Supp}(f)$ và có giá compact, thì $|f(x)| \leq ah(x)$ trên $\operatorname{Supp}(\mu)$, do đó

$$
|\mu|(|f|) \leq a|\mu|(h) \leq a\|\mu\|
$$

theo Hệ quả 2; khi đó kết luận suy ra từ công thức (13) của \S 1, No. 6.

#### Mệnh đề 9 {#int-iii-s2-prop-9 .statement}

— Cho $\mu$ là một độ đo dương trên $X$; nếu $f$ là một hàm trong $\mathcal{K}_+(X)$ sao cho $\mu(f) = 0$, thì $f$ bằng không trên $\mathrm{Supp}(\mu)$.

Cho $x$ là một điểm của $X$ sao cho $f(x) > 0$; hãy chỉ ra rằng $x$ không thuộc $\mathrm{Supp}(\mu)$. Thật vậy, tồn tại một lân cận compắc $V$ của $x$ và một số $a > 0$ sao cho $f(y) \geq a$ trên $V$. Nếu $g$ là một hàm liên tục bất kỳ $\geq 0$ với giá đỡ được chứa trong $V$, hãy chỉ ra rằng $\mu(g) = 0$; thật vậy, nếu đặt $b = \|g\|$ thì $g \leq bf/a$, do đó $\mu(g) \leq b\mu(f)/a = 0$.

#### Mệnh đề 10 {#int-iii-s2-prop-10 .statement}

— Cho $\mu$ là một độ đo trên một không gian compact địa phương $X$; với mọi hàm $g \in \mathcal{C}(X; \mathbf{C})$, giá của độ đo $g \cdot \mu$ là bao đóng $T$ của tập hợp các điểm $x \in \mathrm{Supp}(\mu)$ sao cho $g(x) \neq 0$.

Đặt $S = \mathrm{Supp}(\mu)$; lấy $x_0$ là một điểm không thuộc $T$; tồn tại một lân cận mở $V$ của $x_0$ sao cho tại mọi điểm của $V \cap S$, $g$ bằng không; nếu $f \in \mathcal{K}(X; \mathbf{C})$ có giá được chứa trong $V$, thì $fg$ bằng không trên $S$, do đó (Mệnh đề 8) $\mu(gf) = 0$; nói cách khác, hạn chế của $g \cdot \mu$ trên $V$ bằng không.

Ngược lại, giả sử rằng hạn chế của $g \cdot \mu$ trên một lân cận mở $W$ của một điểm $x_0 \in X$ là không, hãy chứng minh rằng không tồn tại điểm nào của $W \cap S$ tại đó $g$ là $\neq 0$. Thật vậy, nếu có một điểm như vậy $y$, thì sẽ tồn tại một lân cận compact $U$ của $y$, được chứa trong $W$, sao cho tại mọi điểm $x$ của nó ta có $g(x) \neq 0$; nhưng khi đó mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$ với giá được chứa trong $U$ đều có thể được viết dưới dạng $f = gh$, trong đó $h \in \mathcal{K}(X; \mathbf{C})$ có giá được chứa trong $U \subset W$; do đó suy ra $\mu(f) = \mu(gh) = 0$, trái với giả thiết $y \in S$.

Chú ý rằng $T$ được chứa trong giao của giá $S$ của $\mu$ và giá của $g$, nhưng không nhất thiết bằng giao này. Ví dụ, nếu $X = \mathbf{R}$, $\mu$ là độ đo Dirac tại điểm 0, và $g(x) = x$, thì $g \cdot \mu = 0$ mặc dù giao của các giá của $g$ và $\mu$ thu về điểm 0, do đó là khác rỗng.

#### Hệ quả {#int-iii-s2-n3-cor-1 .statement}

— Để độ đo $g \cdot \mu$ bằng không, điều kiện cần và đủ là $g$ bằng không trên giá của $\mu$.

#### Mệnh đề 11 {#int-iii-s2-prop-11 .statement}

— Mọi độ đo có giá compact đều bị chặn.

Thật vậy, $|\mu|$ cũng là một độ đo có giá compact, do đó ta có thể chỉ xét trường hợp $\mu \geq 0$; nếu $h$ là một ánh xạ liên tục từ $X$ vào $[0, 1]$, có giá compact và bằng 1 trên $\mathrm{Supp}(\mu)$, thì với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$ ta có $|f(x)| \leq \|f\| h(x)$ trên $\mathrm{Supp}(\mu)$, do đó (Hệ quả 2 của Mệnh đề 8) $\mu(|f|) \leq \mu(h)\|f\|$, điều này chứng minh mệnh đề (\S 1, No. 8).

### 4. Các độ đo điểm. Các độ đo có giá hữu hạn

#### Mệnh đề 12 {#int-iii-s2-prop-12 .statement}

— Cho $a_i$ ($1 \leq i \leq n$) là các điểm phân biệt trong một không gian compact địa phương $X$. Mọi độ đo trên $X$ mà giá của nó được chứa trong tập hợp các $a_i$ đều là một tổ hợp tuyến tính của các độ đo $\varepsilon_{a_i}$ ($1 \leq i \leq n$).

Thật vậy, một độ đo như thế $\mu$ bằng không trên mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$ thỏa mãn $n$ hệ thức $f(a_i) = 0$ (No. 3, Mệnh đề 8); vì các hệ thức này có thể được viết là $\varepsilon_{a_i}(f) = 0$, nên $\mu$ là một tổ hợp tuyến tính của các $\varepsilon_{a_i}$ (A, II, §7, No. 5, Hệ quả 1 của Định lý 7).

Đặc biệt, mọi độ đo có giá hoặc rỗng hoặc thu về một điểm duy nhất $x$ đều có dạng $\alpha \varepsilon_x$, trong đó $\alpha$ là một số phức; một độ đo như vậy được gọi là một *độ đo điểm*; do đó mọi độ đo có giá hữu hạn đều là một tổng các độ đo điểm.

#### Định lý 1 {#int-iii-s2-thm-1 .statement}

— *Mọi độ đo* $\mu$ *trên một không gian địa phương compact* $X$ *đều thuộc bao đóng mờ của không gian vectơ* $V$ *gồm các độ đo có giá là một tập hữu hạn và được chứa trong* $\mathrm{Supp}(\mu)$.

Chỉ cần chứng minh rằng $\mu$ trực giao với không gian con $V^\circ$ của $\mathcal{K}(X; \mathbf{C})$ trực giao với $V$ (TVS, II, §6, No. 3, Hệ quả 2 của Định lý 1), nghĩa là các hệ thức $\langle f, \varepsilon_a \rangle = 0$, trong đó $a$ chạy qua giá của $\mu$, kéo theo $\langle f, \mu \rangle = 0$; nhưng đó chính là Mệnh đề 8 của No. 3.

#### Hệ quả 1 {#int-iii-s2-thm-1-cor-1 .statement}

— *Mọi độ đo bị chặn* $\mu$ *trên* $X$ *đều thuộc bao đóng mờ của tập lồi* $A$ *gồm các độ đo có giá hữu hạn và được chứa trong giá của* $\mu$, *và có chuẩn* $\leq \| \mu \|$. *Hơn nữa, nếu* $\nu$ *hội tụ mờ đến* $\mu$ *trong khi vẫn thuộc* $A$, *thì* $\| \nu \|$ *hội tụ đến* $\| \mu \|$.

Để chứng minh mệnh đề thứ nhất, chỉ cần thiết lập rằng độ đo $\mu$ thuộc cực của cực $A^\circ$ của $A$ trong $\mathcal{K}(X; \mathbf{C})$ (TVS, II, §6, No. 3, Định lý 1 và §8, No. 4); điều đó có nghĩa là, với $f \in \mathcal{K}(X; \mathbf{C})$, các hệ thức $|\langle f, \varepsilon_a \rangle| \leq 1/\| \mu \|$ với mọi $a \in \mathrm{Supp}(\mu)$ kéo theo $|\langle f, \mu \rangle| \leq 1$; nhưng đây là một hệ quả của Hệ quả 3 của Mệnh đề 8 của No. 3.

Để chứng minh mệnh đề thứ hai, ta nhận thấy rằng

$$
\liminf_{\nu \to \mu, \nu \in A} \| \nu \| \geq \| \mu \|
$$

vì hàm $\nu \mapsto \| \nu \|$ là nửa liên tục dưới đối với tôpô mơ hồ (§1, No. 9, Hệ quả 4 của Mệnh đề 15), và kết luận suy ra từ sự kiện là $\| \nu \| \leq \| \mu \|$ với $\nu \in A$ theo định nghĩa.

#### Hệ quả 2 {#int-iii-s2-thm-1-cor-2 .statement}

— *Mọi độ đo bị chặn* $\mu$ *trên* $X$ *đều thuộc bao đóng mờ của tập các độ đo có giá hữu hạn và được chứa trong giá của* $\mu$ *và có chuẩn bằng* $\| \mu \|$.

Ta có thể giả sử rằng $\mu \neq 0$. Gọi $V$ là một lân cận mở của 0 đối với tôpô mơ hồ; với mọi $\varepsilon$ sao cho $0 < \varepsilon < 1$, theo Hệ quả 1, tồn tại một độ đo $\nu_0$ có giá là hữu hạn và được chứa trong $\mathrm{Supp}(\mu)$ và sao cho $\nu_0 - \mu \in V$ và $\| \mu \| \geq \| \nu_0 \| \geq (1 - \varepsilon) \| \mu \|$. Đặt $\nu = (\| \mu \| / \| \nu_0 \|) \nu_0$, ta có $\| \nu \| = \| \mu \|$ và $\| \nu - \nu_0 \| \leq \| \mu \|$; do đó, với $\varepsilon$ đủ nhỏ, ta có $\nu - \mu \in V + V$, do đó suy ra kết luận.

#### Hệ quả 3 {#int-iii-s2-thm-1-cor-3 .statement}

*Mọi độ đo dương bị chặn $\mu$ trên $X$ đều thuộc bao đóng mơ hồ của tập lồi các độ đo dương có giá mang hữu hạn và được chứa trong giá mang của $\mu$ và có chuẩn bằng $\| \mu \|$.*

Cùng một lập luận như trong Hệ quả 2 cho thấy rằng ta có thể chỉ cần chứng minh rằng $\mu$ thuộc bao đóng mờ của tập lồi $B$ gồm các độ đo dương có giá hữu hạn được chứa trong $\mathrm{Supp}(\mu)$ và có chuẩn $\leq \| \mu \|$. Lại nữa, chỉ cần thiết lập rằng $\mu$ thuộc tập cực của $B^\circ$, tập cực của $B$ *trong không gian* $\mathcal{K}(X; \mathbf{R})$ (TVS, II, §6, No. 3, Định lý 1); nhưng điều đó có nghĩa là với $f \in \mathcal{K}(X; \mathbf{R})$ thì các hệ thức $\langle f, \varepsilon_a \rangle \geq -1 / \| \mu \|$ với mọi $a \in \mathrm{Supp}(\mu)$ kéo theo $\langle f, \mu \rangle \geq -1$, điều này là một hệ quả của No. 3, Hệ quả 2 của Mệnh đề 8.

#### Hệ quả 4 {#int-iii-s2-thm-1-cor-4 .statement}

*Trong không gian $\mathcal{M}(X; \mathbf{C})$, tập các độ đo điểm là toàn phần đối với tôpô hội tụ compact chặt* (§1, No. 10).

Trên nón $\mathcal{M}_+(X)$, tôpô của sự hội tụ chặt chẽ compact đồng nhất với tôpô mơ hồ (§1, No. 10, Mệnh đề 18), và mọi độ đo trên $X$ đều có thể viết dưới dạng $\mu_1 - \mu_2 + i \mu_3 - i \mu_4$, trong đó các $\mu_j$ ($1 \leq j \leq 4$) là các độ đo dương; do đó kết luận suy ra từ Định lý 1.

#### Mệnh đề 13 {#int-iii-s2-prop-13 .statement}

*Cho $\mu$ là một độ đo trên một không gian địa phương compact $X$. Để một điểm $x_0$ thuộc $\mathrm{Supp}(\mu)$, điều kiện cần và đủ là độ đo điểm $\varepsilon_{x_0}$ nằm trong bao đóng mơ hồ của tập các độ đo $g \cdot \mu$, trong đó $g$ chạy qua tập các hàm liên tục có giá compact sao cho $\| g \cdot \mu \| \leq 1$.*

Điều kiện ấy hiển nhiên là đủ theo Mệnh đề 6 của No. 2. Để thấy rằng nó là cần thiết, giả sử $x_0 \in \mathrm{Supp}(\mu)$; xét một số hữu hạn các hàm $f_k$ ($1 \leq k \leq n$) trong $\mathcal{K}(X; \mathbf{C})$, và một số tùy ý $\delta > 0$; ta phải chứng minh rằng tồn tại một hàm $g \in \mathcal{K}(X; \mathbf{C})$ sao cho $\| g \cdot \mu \| \leq 1$ và sao cho
$$
|f_k(x_0) - \mu(g f_k)| \leq \delta
$$
với $1 \leq k \leq n$. Gọi $U$ là một lân cận mở tương đối compact của $x_0$ sao cho độ dao động của mỗi $f_k$ ($1 \leq k \leq n$) trên $U$ là $\leq \delta / 2$. Theo giả thiết, vì $x_0 \in \mathrm{Supp}(\mu)$, tồn tại một hàm $g_0 \in \mathcal{K}(X; \mathbf{C})$ có giá được chứa trong $U$ và sao cho $\mu(g_0) \neq 0$; độ đo $\nu = g_0 \cdot \mu$ khác không, vì với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$ bằng 1 trên $U$, ta có $\nu(f) = \mu(g_0) \neq 0$. Hơn nữa, $\nu$ bị chặn (No. 3, Mệnh đề 11);

nhân $g_0$ với một vô hướng, ta có thể giả sử rằng $\| \nu \| = 1$. Khi đó, đặt $\alpha_k = f_k(x_0)$ ta có thể viết, với $1 \leq k \leq n$ và với mọi hàm $h \in \mathcal{K}(X; \mathbf{C})$,

$$
f_k(x_0) - \nu(f_k h) = \alpha_k (1 - \nu(h)) + \nu((\alpha_k - f_k)h) .
$$

Vì $\nu$ có giá trong $U$, ta có thể đồng nhất nó với hạn chế của nó lên $U$; khi đó giả thiết $\| \nu \| = 1$ suy ra rằng tồn tại một hàm $h \in \mathcal{K}(X; \mathbf{C})$, có giá được chứa trong $U$, sao cho $\| h \| \leq 1$ và sao cho $| \alpha_k (1 - \nu(h)) | \leq \delta / 2$ với $1 \leq k \leq n$. Định nghĩa của $U$ hơn nữa cho thấy rằng $| (\alpha_k - f_k(x)) h(x) | \leq \delta / 2$ với mọi $x \in U$; vì $\| \nu \| = 1$ và $\operatorname{Supp}(\nu) \subset U$ nên do đó ta có $| \nu((\alpha_k - f_k)h) | \leq \delta / 2$ và vì thế, đặt $g = g_0 h$,

$$
| f_k(x_0) - \mu(g f_k) | \leq \delta \quad \text{với } 1 \leq k \leq n .
$$

Điều này chứng minh mệnh đề, vì $\| g \cdot \mu \| = \| (g_0 h) \cdot \mu \| \leq \| g_0 \cdot \mu \| = 1$.

#### Hệ quả {#int-iii-s2-n4-cor-1 .statement}

*Cho $\mu$ là một độ đo trên $X$. Để một độ đo $\nu$ trên $X$ thuộc bao đóng mờ của tập các độ đo $g \cdot \mu$, trong đó $g$ chạy qua $\mathcal{K}(X; \mathbf{C})$, điều kiện cần và đủ là $\operatorname{Supp}(\nu) \subset \operatorname{Supp}(\mu)$.*

Thật vậy, $\operatorname{Supp}(g \cdot \mu) \subset \operatorname{Supp}(\mu)$ theo No. 3, Mệnh đề 10; do đó giá của mọi giới hạn vague của các độ đo dạng $g \cdot \mu$ cũng được chứa trong $\operatorname{Supp}(\mu)$ (No. 2, Mệnh đề 6). Ngược lại, nếu $\operatorname{Supp}(\nu) \subset \operatorname{Supp}(\mu)$ thì $\nu$ là giới hạn vague của các độ đo có giá *hữu hạn* được chứa trong $\operatorname{Supp}(\mu)$ (Định lý 1), nên thuộc bao đóng vague của tập hợp các độ đo $g \cdot \mu$ theo Mệnh đề 13.

### 5. Các độ đo rời rạc

#### Mệnh đề 14 {#int-iii-s2-prop-14 .statement}

*Để một độ đo $\mu$ trên một không gian compact địa phương $X$ là một độ đo rời rạc (\S 1, No. 3, Ví dụ I), điều kiện cần và đủ là $\operatorname{Supp}(\mu)$ là một không gian con đóng rời rạc của $X$.*

Cho $\mu$ là một độ đo rời rạc trên $X$, được xác định bởi các khối lượng $h(x) \neq 0$ đặt tại các điểm $x$ của một không gian con rời rạc đóng $N$ của $X$; ta hãy chứng minh rằng $\operatorname{Supp}(\mu) = N$. Với mọi $a \in N$ và mọi lân cận $V$ của $a$, tồn tại một hàm $f \in \mathcal{K}(X; \mathbf{C})$ có giá được chứa trong $V$, bằng 1 tại điểm $a$ và bằng 0 tại các điểm khác của $N$, do đó $\mu(f) = h(a) \neq 0$. Mặt khác, nếu $b \notin N$ thì tồn tại một lân cận $W$ của $b$ không giao với $N$; vì vậy, với mọi hàm $g \in \mathcal{K}(X; \mathbf{C})$ có giá được chứa trong $W$, ta có $\mu(g) = 0$, điều này chứng tỏ rằng $b \notin \operatorname{Supp}(\mu)$.

Ngược lại, cho $\mu$ là một độ đo sao cho $\operatorname{Supp}(\mu)$ là một không gian con đóng rời rạc $N$ của $X$. Với mọi $a \in N$, tồn tại một lân cận mở $V_a$ của $a$ không chứa điểm nào của $N$ phân biệt với $a$; do đó hạn chế của $\mu$ lên $V_a$ là một độ đo điểm có giá $\{a\}$ (No. 2, Mệnh đề 5), nên (No. 4, Mệnh đề 12) có dạng $h(a)\varepsilon_a$, trong đó $h(a) \neq 0$. Đặt $h(x) = 0$ tại các điểm của $\mathbf{C}\mathbf{N}$, và ký hiệu bởi $\nu$ độ đo được xác định bởi các khối lượng $h(x)$, nguyên lý địa phương hóa cho thấy rằng $\nu = \mu$.

Do đó ta thấy rằng trên một không gian *rời rạc* $X$, mọi độ đo đều là *rời rạc*.

### Bài tập {#int-iii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
