---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 4
section_title: Approximation of continuous real-valued functions
lang: vi
source: top-v-x
pdf_pages: 0314-0323, 0343-0352
extraction: ocr
subsections:
    - "no": 1
      title: APPROXIMATION OF CONTINUOUS FUNCTIONS BY FUNCTIONS BELONGING TO A LATTICE
      page: 0
      pdf_page: 314
    - "no": 2
      title: APPROXIMATION OF CONTINUOUS FUNCTIONS BY POLYNOMIALS
      page: 0
      pdf_page: 317
    - "no": 3
      title: 'APPLICATION : APPROXIMATION OF CONTINUOUS REAL-VALUED FUNCTIONS DEFINED ON A PRODUCT OF COMPACT SPACES'
      page: 0
      pdf_page: 320
    - "no": 4
      title: APPROXIMATION OF CONTINUOUS MAPPINGS OF A COMPACT SPACE INTO A NORMED SPACE
      page: 0
      pdf_page: 320
statements: 18
exercises: 5
content_sha256: 6a29a79e399c2496aaed5c1c4d00902d6fbe49af851d9a0e3b16aaec88223fe4
translated_from: content/en/top/X/04_s4_approximation_of_continuous_real_valued.md
source_content_sha256: 352337cc126af02c15ffde78bc5a2610b483c38d6be644a79f5231184afe7314
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-9e661c89
glossary_version: 34
glossary_terms_sha256: bf41ba61b119a2c31b03586584e16c841da8cb3093b82bec44b675965c029fc2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. XẤP XỈ CÁC HÀM GIÁ TRỊ THỰC LIÊN TỤC

### 1. XẤP XỈ CÁC HÀM LIÊN TỤC BỞI CÁC HÀM THUỘC VÀO MỘT DÀN

Trong mục này ta sẽ nghiên cứu tập hợp $\mathcal{C} = C(X; \mathbf{R})$ các hàm giá trị thực liên tục (*) xác định trên một không gian *compact* $X$, và ta sẽ luôn giả sử rằng $\mathcal{C}$ được trang bị tôpô của *sự hội tụ đều*. Từ § 3, no. 2 ta biết rằng tôpô này được xác định bởi chuẩn

$$
||f|| = \sup_{x \in X} |f(x)|
$$

và rằng chuẩn này tương thích với cấu trúc đại số $\mathbf{R}$ của $\mathcal{C}$. Với chuẩn này và cấu trúc đại số này, $\mathcal{C}$ là một *đại số định chuẩn đầy đủ* trên $\mathbf{R}$ ($§ 1$, no. 6, Định lý 2, Hệ quả 1).

(*) Các hàm giá trị thực được xét trong mục này luôn được giả sử là *hữu hạn*.

Nếu $H$ là một tập con của $\mathcal{C}$, ta sẽ nói rằng một hàm giá trị thực liên tục $f$ trên $X$ có thể được xấp xỉ đều bởi các hàm của $H$ nếu $f$ thuộc bao đóng của $H$ trong không gian $\mathcal{C}$, tức là nếu, với mỗi $\varepsilon > 0$, tồn tại một hàm $g \in H$ sao cho $|f(x) - g(x)| \leq \varepsilon$ với mọi $x \in X$. Nói rằng mọi hàm giá trị thực liên tục trên $X$ có thể được xấp xỉ đều bởi các hàm của $H$ do đó có nghĩa là $H$ là trù mật trong $\mathcal{C}$.

Trên tập hợp $\mathcal{C}$, quan hệ $f \leq g$ [có nghĩa là $f(x) \leq g(x)$ với mọi $x \in X$] là một quan hệ thứ tự, đối với quan hệ này $\mathcal{C}$ là một dàn. Rõ ràng ta có $|||u| - |v||| \leq ||u - v||$, và do đó $u \to |u|$ là một ánh xạ liên tục đều của $\mathcal{C}$ vào chính nó. Suy ra rằng

$$
(u, v) \to \sup (u, v) = \frac{1}{2}(u + v + |u - v|)
$$

và

$$
(u, v) \to \inf (u, v) = \frac{1}{2}(u + v - |u - v|)
$$

là liên tục đều trên $\mathcal{C} \times \mathcal{C}$.

MỆNH ĐỀ I. Cho $X$ là một không gian compact và cho $H$ là một tập hợp các hàm giá trị thực liên tục xác định trên $X$. Cho $f$ là một hàm giá trị thực liên tục trên $X$ sao cho với mỗi $x \in X$ tồn tại một hàm $u_x \in H$ sao cho $u_x(x) > f(x)$ [tương ứng. $u_x(x) < f(x)$]. Khi đó tồn tại một số hữu hạn các hàm $u_{x_i} = f_i \in H$ ($1 \leq i \leq n$) sao cho, nếu $v = \sup(f_1, f_2, \ldots, f_n)$ [tương ứng. $w = \inf(f_1, f_2, \ldots, f_n)$], ta có $v(x) > f(x)$ [tương ứng. $w(x) < f(x)$] với mọi $x \in X$.

Với mỗi $x \in X$, cho $G_x$ là tập mở gồm tất cả các $z \in X$ sao cho $u_x(z) > f(z)$ [tương ứng $u_x(z) < f(z)$]. Vì $x \in G_x$ theo giả thiết, nên $X$ là hợp của các tập hợp $G_x$ khi $x$ chạy qua $X$. Vì $X$ compact nên tồn tại một số hữu hạn điểm $x_i$ ($1 \leq i \leq n$) sao cho các $G_{x_i}$ phủ $X$, và hiển nhiên rằng các hàm $f_i = u_{x_i}$ thỏa mãn các điều kiện của mệnh đề.

ĐỊNH LÝ I (Dini). Cho $X$ là một không gian compact, và cho $H$ là một tập hợp các hàm thực liên tục trên $X$ có hướng đối với quan hệ $\leq$ (tương ứng $\geq$). Nếu bao trên (tương ứng bao dưới) $f$ của $H$ là hữu hạn và liên tục trên $X$, thì $f$ có thể được xấp xỉ đều bởi các hàm thuộc $H$ (hay tương đương, bộ lọc tiết diện của $H$ hội tụ đều đến $f$ trong $X$).

Với mọi $\varepsilon > 0$, với mỗi $x \in X$ tồn tại một hàm $u_x \in H$ sao cho $u_x(x) > f(x) - \varepsilon$. Theo Mệnh đề I và sự kiện $H$ có hướng đối với quan hệ $\leq$, tồn tại $g \in H$ sao cho $g(x) > f(x) - \varepsilon$ với mọi $x \in X$; mặt khác, theo định nghĩa ta có $g(x) \leq f(x)$, và do đó định lý được chứng minh.

#### Hệ quả {#top-x-s4-n1-cor-1 .statement}

Cho $(u_n)$ là một dãy tăng (tương ứng giảm) các hàm thực liên tục trên $X$. Nếu bao trên (tương ứng bao dưới) $f$ của dãy $(u_n)$ là hữu hạn và liên tục trên $X$, thì dãy $(u_n)$ hội tụ đều đến $f$ trong $X$.

Hiển nhiên là kết luận của Định lý 1 không còn nhất thiết đúng nếu $X$ không còn được giả thiết là compact, như được chỉ ra bởi ví dụ về dãy giảm của các hàm $x/(n + x)$ trong $\mathbf{R}_+$.

#### Mệnh đề 2 {#top-x-s4-prop-2 .statement}

Cho $X$ là một không gian compact, và cho $H$ là một tập hợp các hàm liên tục nhận giá trị thực trên $X$ sao cho, với bất kỳ hai hàm $u \in H, v \in H$ nào, các hàm $\sup(u, v)$ và $\inf(u, v)$ đều thuộc $H$. Khi đó một hàm liên tục nhận giá trị thực $f$ trên $X$ có thể được xấp xỉ đều bởi các hàm thuộc $H$ khi và chỉ khi, với mỗi số thực $\varepsilon > 0$ và mỗi cặp $x, y$ điểm của $X$, tồn tại một hàm $u_{x, y} \in H$ sao cho $|f(x) - u_{x, y}(x)| < \varepsilon$ và $|f(y) - u_{x, y}(y)| < \varepsilon$.

Điều kiện ấy hiển nhiên là cần thiết; ta hãy chứng minh rằng nó là đủ. Với mỗi $\varepsilon > 0$, ta sẽ chứng minh rằng có một hàm $g \in H$ sao cho $|f(z) - g(z)| < \varepsilon$ với mọi $z \in X$. Cho $x$ là một điểm bất kỳ của $X$, và cho $H_x$ là tập hợp tất cả các hàm $u \in H$ sao cho $u(x) < f(x) + \varepsilon$. Theo giả thiết, với mỗi $y \in X$, hàm $u_{x, y}$ thuộc $H_x$ và ta có $u_{x, y}(y) > f(y) - \varepsilon$. Do đó, theo Mệnh đề 1, tồn tại một số hữu hạn các hàm của $H_x$ mà bao trên của chúng là $v_x$ sao cho $v_x(z) > f(z) - \varepsilon$ với mọi $z \in X$; mặt khác, ta có $v_x(x) < f(x) + \varepsilon$ theo định nghĩa của $H_x$; cuối cùng, $v_x \in H$ theo giả thiết. Vì vậy Mệnh đề 1 cho thấy rằng tồn tại một số hữu hạn các hàm $v_{x_i}$ mà bao dưới của chúng là $g$ sao cho $g(z) < f(z) + \varepsilon$ với mọi $z \in X$; nhưng vì ta có $v_{x_i}(z) > f(z) - \varepsilon$ với mọi $z \in X$ và với mọi chỉ số $i$, nên ta cũng có $g(z) > f(z) - \varepsilon$ với mọi $z \in X$. Vì $g \in H$ theo giả thiết, chứng minh kết thúc.

#### Nhận xét {#top-x-s4-n1-rem-1 .statement}

Khi tập $H$ thỏa mãn các điều kiện của Mệnh đề 2, nó là một dàn đối với thứ tự $f \leq g$. Nhưng cần lưu ý rằng một tập con $H$ của $C$ có thể là một dàn đối với thứ tự này mà không nhất thiết là cận trên nhỏ nhất (tương ứng, cận dưới lớn nhất) trong $H$ của hai hàm $u, v$ thuộc $H$ lại trùng với cận trên nhỏ nhất (tương ứng, cận dưới lớn nhất) của chúng trong $C$. \* Một ví dụ là các ánh xạ lồi của một khoảng compact của $\mathbf{R}$ vào $\mathbf{R}$. \*

#### Hệ quả {#top-x-s4-n1-cor-2 .statement}

Giả sử rằng $H$ được xác định sao cho, hễ $u \in H$ và $v \in H$ thì ta có $\sup(u, v) \in H$ và $\inf(u, v) \in H$; đồng thời sao cho, cho trước bất kỳ hai điểm phân biệt $x, y$ của $X$ và bất kỳ hai số thực $\alpha, \beta$, tồn tại một hàm $g \in H$ sao cho $g(x) = \alpha$ và $g(y) = \beta$. Khi đó mọi hàm giá trị thực liên tục trên $X$ đều có thể được xấp xỉ đều bởi các hàm thuộc $H$.

#### Định nghĩa 1 {#top-x-s4-def-1 .statement}

*Nếu X là bất kỳ một tập hợp nào, một tập H các ánh xạ của X vào một tập Y được gọi là phân biệt các phần tử của một tập con A của X (hay là một tập phân biệt cho các phần tử của A) nếu, với bất kỳ hai phần tử phân biệt x, y nào của A, tồn tại một hàm f ∈ H sao cho f(x) ≠ f(y).*

Chẳng hạn, nếu X là một không gian hoàn toàn chính quy (Chương IX, § 1, no. 5) thì tập tất cả các ánh xạ liên tục của X vào [0, 1] phân biệt các điểm của X.

#### Định lý 2 (Stone) {#top-x-s4-thm-2 .statement}

*Cho X là một không gian compact, và cho H là một không gian con vectơ của $\mathcal{C}(X; \mathbf{R})$ sao cho 1) các hàm hằng thuộc H; 2) nếu $u \in H$ thì $|u| \in H$; 3) H phân biệt các điểm của X. Khi đó mọi hàm giá trị thực liên tục trên X đều có thể được xấp xỉ đều bởi các hàm của H.*

Chỉ cần chứng minh rằng H thỏa các điều kiện của Hệ quả của Mệnh đề 2. Theo giả thiết, nếu $u \in H$ và $v \in H$, ta có

$$
\sup (u, v) = \frac{1}{2} (u + v + |u - v|) \in H
$$
và
$$
\inf (u, v) = \frac{1}{2} (u + v - |u - v|) \in H.
$$

Mặt khác, cho x và y là bất kỳ hai điểm phân biệt nào của X, và cho α, β là bất kỳ hai số thực nào. Theo giả thiết, tồn tại một hàm $h \in H$ sao cho $h(x) \neq h(y)$: chẳng hạn $h(x) = \gamma$ và $h(y) = \delta$. Vì các hàm hằng thuộc H, hàm
$$
g(z) = \alpha + (\beta - \alpha) \frac{h(z) - \gamma}{\delta - \gamma}
$$
thuộc H và thỏa $g(x) = \alpha$ và $g(y) = \beta$.

### 2. XẤP XỈ CÁC HÀM LIÊN TỤC BẰNG ĐA THỨC

Cho một tập H các hàm giá trị thực được xác định trên một tập X, ta nói rằng một hàm giá trị thực được xác định trên X là một đa thức (hoặc một đa thức không có số hạng tự do) với hệ số thực, theo các hàm của H, nếu nó có dạng $x \to g(f_1(x), f_2(x), \ldots, f_n(x))$ trong đó g là một đa thức (hoặc một đa thức không có số hạng tự do) theo n ẩn thức (n tùy ý) với hệ số thực, và các $f_i$ ($1 \leq i \leq n$) thuộc H.

#### Định lý 3 (Weierstrass-Stone) {#top-x-s4-thm-3 .statement}

*Cho X là một không gian compact và cho H là một tập các hàm giá trị thực liên tục trên X phân biệt các điểm của X. Khi đó mọi hàm giá trị thực liên tục trên X đều có thể được xấp xỉ đều bởi các đa thức (với hệ số thực) theo các hàm của H.*

Một mệnh đề tương đương của định lý là *bất kỳ đại số con nào của $\mathcal{C}(X; \mathbf{R})$ chứa các hàm hằng và phân biệt các điểm của X đều trù mật trong $\mathcal{C}(X; \mathbf{R})$*.

Cho $H_0$ là tập tất cả các đa thức theo các hàm của H, và cho $\overline{H}_0$ là bao đóng của $H_0$ trong $\mathcal{C}$. Nếu g là một đa thức bất kỳ theo n biến với hệ số thực, thì $(u_1, u_2, \ldots, u_n) \to g(u_1, u_2, \ldots, u_n)$ là một ánh xạ liên tục của $\mathcal{C}^n$ vào $\mathcal{C}$, ánh xạ $H_0^n$ vào $H_0$, và do đó ánh xạ $\overline{H}_0^n$ vào $\overline{H}_0$ (Chương I, § 2, no. 1, Định lý 1). Đặc biệt, $\overline{H}_0$ là một không gian con vectơ của $\mathcal{C}$ và hiển nhiên thỏa điều kiện thứ nhất và thứ ba của Định lý 2; ta sẽ chứng minh rằng nó cũng thỏa điều kiện thứ hai, và điều này sẽ chứng minh rằng $\overline{H}_0 = \mathcal{C}$.

Vì mọi hàm $u \in \overline{H}_0$ đều bị chặn trên X, nên đủ để chứng minh bổ đề sau:

#### Bổ đề 1 {#top-x-s4-lem-1 .statement}

*Với mỗi số thực $\varepsilon > 0$ và mỗi khoảng compact $I \subset \mathbf{R}$ tồn tại một đa thức p(t) không có số hạng tự do sao cho $|p(t) - |t|| \leq \varepsilon$ với mọi $t \in I$.*

Đủ để chứng minh bổ đề cho một khoảng có dạng $I = [-a, +a]$ và do đó, thay $t$ bằng $at$, cho khoảng $I = [-1, +1]$. Vì $|t| = \sqrt{t^2}$, Bổ đề 1 là hệ quả của kết quả sau:

#### Bổ đề 2 {#top-x-s4-lem-2 .statement}

*Gọi $(P_n)$ là dãy các đa thức không có số hạng hằng được xác định bởi*
$$
(1) \quad p_0(t) = 0, \quad p_{n+1}(t) = p_n(t) + \frac{1}{2} (t - (p_n(t))^2), \qquad n \geq 0.
$$
*Trong khoảng $[0, 1]$, dãy $(p_n)$ tăng và hội tụ đều đến $\sqrt{t}$.*

Để chứng minh Bổ đề 2, chỉ cần chỉ ra rằng, với mọi $t \in [0, 1]$, ta có
$$
(2) \qquad 0 \leq \sqrt{t} - p_n(t) \leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}},
$$
vì (2) suy ra $0 \leq \sqrt{t} - p_n(t) \leq 2/n$.

Ta chứng minh (2) bằng quy nạp theo $n$. Điều này đúng với $n = 0$. Nếu $n \geq 0$ thì từ giả thiết quy nạp (2) suy ra $0 \leq \sqrt{t} - p_n(t) \leq \sqrt{t}$, do đó $0 \leq p_n(t) \leq \sqrt{t}$, và vì vậy từ (1) ta có
$$
\sqrt{t} - p_{n+1}(t) = (\sqrt{t} - p_n(t)) (1 - \frac{1}{2} (\sqrt{t} + p_n(t))),
$$
suy ra $\sqrt{t} - p_{n+1}(t) \geq 0$, và từ (2)
$$
\begin{align*}
\sqrt{t} - p_{n+1}(t) &\leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2} \right) \\
&\leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2 + (n+1) \sqrt{t}} \right) \\
&= \frac{2 \sqrt{t}}{2 + (n+1) \sqrt{t}}.
\end{align*}
$$
Q.E.D.

Nếu $X$ không compact, kết luận của Định lý 3 không nhất thiết đúng. Chẳng hạn, một hàm thực liên tục trên $\mathbf{R}$ bị chặn và không hằng không thể được xấp xỉ đều trong $\mathbf{R}$ bởi các đa thức (xem Bài tập 6).

#### Mệnh đề 3 {#top-x-s4-prop-3 .statement}

*Gọi* $(K_i)_{i \in I}$ *là một họ các khoảng compact của* $\mathbf{R}$, $K = \prod_{i \in I} K_i$ *là tích của chúng*, và gọi $X$ *là một không gian con compact của* $K$. *Khi đó mọi hàm thực liên tục trên* $X$ *đều có thể được xấp xỉ đều bởi các đa thức theo các tọa độ* $x_i = \mathrm{pr}_i x$.

Vì nếu $x = (x_i)$ và $y = (y_i)$ là hai điểm phân biệt của $X$, thì tồn tại ít nhất một chỉ số $i$ sao cho $x_i \neq y_i$; do đó họ các hàm liên tục $\mathrm{pr}_i$ thỏa mãn các điều kiện của Định lý 3.

#### Mệnh đề 4 {#top-x-s4-prop-4 .statement}

*Gọi* $X$ *là một không gian compact, gọi* $A$ *là một không gian con đóng của* $X$, *và gọi* $H$ *là một tập hợp các hàm thực liên tục trên* $X$ *phân biệt các điểm của* $C_A$ *và sao cho* $A$ *là giao của các tập hợp* $\overline{u}^{-1}(0)$ *khi* $u$ *chạy qua* $H$. *Khi đó mọi hàm thực liên tục trên* $X$ *bằng không trên* $A$ *có thể được xấp xỉ đều bởi các đa thức không có số hạng hằng theo các hàm của* $H$.

Xét trước hết trường hợp riêng trong đó $A$ gồm một điểm duy nhất $x_0$. Khi đó các giả thiết suy ra rằng $H$ phân biệt các điểm của $X$; thật vậy, nếu $x \neq x_0$, thì theo giả thiết có một hàm $u \in H$ sao cho $u(x) \neq 0 = u(x_0)$. Do đó, với mỗi $\varepsilon > 0$ và mỗi hàm thực liên tục $f$ trên $X$ sao cho $f(x_0) = 0$, tồn tại (Định lý 3) một đa thức $g$ theo các hàm của $H$ sao cho $|f(x) - g(x)| \leq \varepsilon$ với mọi $x \in X$. Đặc biệt $|g(x_0)| \leq \varepsilon$, nên

$$
|f(x) - (g(x) - g(x_0))| \leq 2\varepsilon
$$

với mọi $x \in X$; và vì $g(x) - g(x_0)$ là một đa thức theo các hàm của $H$ không có hạng tự do, kết quả được thiết lập trong trường hợp này.

Trong trường hợp tổng quát, xét quan hệ tương đương $R$ trên $X$ có các lớp là tập $A$ và các tập $\{x\}$ với $x \notin A$. Không gian thương $X/R$ là Hausdorff (Chương I, § 8, no. 6, Mệnh đề 15) và do đó compact. Gọi $\varphi : X \to X/R$ là ánh xạ chính tắc. Mỗi hàm thực liên tục $f$ trên $X$ triệt tiêu trên $A$ có thể được viết dưới dạng $f = f_1 \circ \varphi$, trong đó $f_1$ là một hàm thực liên tục trên $X/R$ và triệt tiêu tại điểm $x_0' = \varphi(A)$. Áp dụng kết quả đã được chứng minh cho không gian $X/R$ và điểm $x_0'$, ta thu được kết quả cuối cùng.

### 3. ỨNG DỤNG : XẤP XỈ CÁC HÀM THỰC LIÊN TỤC ĐƯỢC XÁC ĐỊNH TRÊN TÍCH CỦA CÁC KHÔNG GIAN COMPACT

#### Định lý 4 {#top-x-s4-thm-4 .statement}

Cho $(X_i)_{i \in I}$ là một họ các không gian compact, và cho
$$
X = \prod_{i \in I} X_i.
$$
Khi đó mọi hàm thực liên tục trên $X$ đều có thể được xấp xỉ đều bởi các tổng của một số hữu hạn các hàm có dạng
$$
(x_i) \to \prod_{\alpha \in J} u_\alpha(x_\alpha),
$$
trong đó $J$ là một tập con hữu hạn (tùy ý) của $I$ và $u_\alpha$ là một hàm thực liên tục trên $X_\alpha$ với mỗi $\alpha \in J$.

Consider the set $H$ of "hàm một biến" $(x_i) \to u_\alpha(x_\alpha)$ (bất kỳ $\alpha \in I$ nào) which are continuous on $X$. Tập hợp này phân biệt các điểm của $X$, vì nếu $x = (x_i)$ và $y = (y_i)$ là hai điểm phân biệt bất kỳ của $X$, thì tồn tại $\alpha \in I$ sao cho $x_\alpha \neq y_\alpha$ và tồn tại một hàm liên tục nhận giá trị thực $h_\alpha$ trên $X_\alpha$ sao cho $h_\alpha(x_\alpha) \neq h_\alpha(y_\alpha)$. Khi đó hàm $x \to h_\alpha(\operatorname{pr}_\alpha x)$ thuộc $H$ và nhận các giá trị khác nhau tại $x$ và $y$. Vì mọi đa thức theo các hàm của $H$ đều có dạng đã nêu trong định lý, suy ra kết quả từ Định lý 3.

Nếu không phải mọi $X_i$ đều compact, thì kết luận của Định lý 4 chưa chắc đúng (xem Bài tập 9).

### 4. Xấp xỉ các ánh xạ liên tục của một không gian compact vào một không gian có chuẩn

Cho $X$ là một không gian compact và cho $Y$ là một không gian vectơ có chuẩn trên trường $\mathbf{R}$ (Chương IX, § 3); không gian $C(X; Y)$ luôn được giả thiết mang tôpô hội tụ đều được xác định bởi chuẩn $\|u\| = \sup_{x \in X} \|u(x)\|$ ($§ 3$, no. 2).

Cho một tập $H$ gồm các hàm liên tục nhận giá trị thực xác định trên $X$, một họ hữu hạn $(u_i)_{1 \leq i \leq n}$ các hàm thuộc $H$, và một họ hữu hạn $(a_i)_{1 \leq i \leq n}$ các điểm của $Y$: khi đó ánh xạ $x \to \sum_{i=1}^n a_i u_i(x)$ của $X$ vào $Y$ là liên tục; ta ký hiệu nó là $\sum_{i=1}^n a_i u_i$, và ta nói rằng nó là một tổ hợp tuyến tính của các hàm của $H$ với hệ số trong $Y$. Ta nói rằng một ánh xạ liên tục $f : X \to Y$ có thể được xấp xỉ đều bởi các tổ hợp tuyến tính của các hàm của $H$ (với hệ số trong $Y$), nếu $f$ nằm trong bao đóng của không gian con vectơ của $C(X; Y)$ được tạo thành bởi các tổ hợp tuyến tính này.

#### Mệnh đề 5 {#top-x-s4-prop-5 .statement}

Cho $X$ là một không gian compact, $Y$ là một không gian có chuẩn trên $\mathbf{R}$ và $H$ là một tập con của $\mathcal{C}(X; \mathbf{R})$. Nếu mọi hàm liên tục nhận giá trị thực trên $X$ đều có thể được xấp xỉ đều bởi các hàm của $H$, thì mọi ánh xạ liên tục $f$ của $X$ vào $Y$ đều có thể được xấp xỉ đều bởi các tổ hợp tuyến tính của các hàm của $H$ với hệ số trong $Y$.

Cho bất kỳ số thực $\varepsilon > 0$ nào, với mỗi $x \in X$ tồn tại một lân cận mở của $x$ trong đó độ dao động của $f$ không vượt quá $\varepsilon$. Do đó tồn tại một phủ mở hữu hạn $(A_i)_{1 \leq i \leq n}$ của $X$ sao cho độ dao động của $f$ trên từng $A_i$ không vượt quá $\varepsilon$. Lấy $a_i$ là một giá trị của $f$ trong $A_i$ ($1 \leq i \leq n$), và lấy $(u_i)_{1 \leq i \leq n}$ là một phân hoạch đơn vị liên tục phụ thuộc vào phủ $(A_i)$ (Chương IX, § 4, no. 4, Hệ quả của Mệnh đề 4). Cho $x$ là một điểm bất kỳ của $X$. Với mỗi chỉ số $i$ sao cho $x \notin A_i$, ta có $u_i(x) = 0$, và với mỗi chỉ số $i$ sao cho $x \in A_i$ ta có $\|f(x) - a_i\| \leq \varepsilon$; suy ra rằng

$$
\left\| f(x) - \sum_{i=1}^n a_i u_i(x) \right\| = \left\| \sum_{i=1}^n (f(x) - a_i) u_i(x) \right\| \leq \varepsilon \sum_{i=1}^n u_i(x) = \varepsilon.
$$

Mặt khác, theo giả thiết tồn tại một hàm $v_i \in H$ sao cho

$$
|u_i(x) - v_i(x)| \leq \frac{\varepsilon}{\sum_{j=1}^n \|a_j\|}
$$

với mọi $x \in X$ ($1 \leq i \leq n$); do đó ta có

$$
\left\| f(x) - \sum_{i=1}^n a_i v_i(x) \right\| \leq 2\varepsilon \quad \text{for all } x \in X,
$$

và chứng minh hoàn tất.

Từ Mệnh đề 5 suy ra rằng, ứng với mỗi mệnh đề mà ta đã chứng minh rằng một tập con $H$ nào đó của $\mathcal{C}(X; \mathbf{R})$ là trù mật, có một mệnh đề tương tự đối với các ánh xạ liên tục của $X$ vào một không gian định chuẩn $Y$ tùy ý. Ta sẽ chỉ viết tường minh mệnh đề tương ứng theo cách này với Định lý 3. Cho một tập $H$ các hàm nhận giá trị thực trên $X$, một đa thức theo các hàm của $H$, với hệ số trong $Y$, được định nghĩa là bất kỳ tổ hợp tuyến tính nào, với hệ số trong $Y$, của các tích của một họ hữu hạn (có thể rỗng) các hàm thuộc $H$. Khi đó:

#### Mệnh đề 6 {#top-x-s4-prop-6 .statement}

Cho $X$ là một không gian compact và cho $H$ là một tập các hàm liên tục nhận giá trị thực trên $X$ phân biệt các điểm của $X$. Khi đó mọi ánh xạ liên tục của $X$ vào một không gian định chuẩn $Y$ trên $\mathbf{R}$ đều có thể được xấp xỉ đều bởi các đa thức theo các hàm của $H$ với hệ số trong $Y$.

Từ đó suy ra:

#### Mệnh đề 7 {#top-x-s4-prop-7 .statement}

Cho $X$ là một không gian compact và cho $H$ là một tập các hàm liên tục nhận giá trị phức trên $X$ phân biệt các điểm của $X$. Khi đó mọi ánh xạ liên tục của $X$ vào một không gian định chuẩn $Y$ trên $\mathbf{C}$ đều có thể được xấp xỉ đều bởi các đa thức theo các hàm $f \in H$ và các liên hợp của chúng $\overline{f}$ với hệ số trong $Y$.

Chỉ cần nhận xét rằng $Y$ cũng là một không gian chuẩn trên $\mathbf{R}$ và áp dụng Mệnh đề 6 cho tập các phần thực và phần ảo của các hàm $f \in H$, dùng các công thức

$$
\Re f = \frac{1}{2} (f + \overline{f}), \quad \Im f = \frac{1}{2i} (f - \overline{f}).
$$

#### Hệ quả 1 {#top-x-s4-prop-7-cor-1 .statement}

Nếu $X$ là một tập con compact của không gian $\mathbf{C}^n$, thì mọi ánh xạ liên tục $(z_1, z_2, \ldots, z_n) \to f(z_1, z_2, \ldots, z_n)$ của $X$ vào một không gian chuẩn $Y$ trên trường $\mathbf{C}$ đều có thể được xấp xỉ đều bởi các đa thức theo $z_k$ và $\overline{z}_k$ với hệ số trong $Y$.

Sau này ta sẽ thấy rằng nói chung không thể xấp xỉ đều $f$ bởi các đa thức (với hệ số trong $Y$) chỉ theo các biến $z_k$, ngay cả khi $Y = \mathbf{C}$.

#### Hệ quả 2 {#top-x-s4-prop-7-cor-2 .statement}

Cho $X$ là một không gian địa phương compact và cho $C_0(X)$ là $\mathbf{C}$-đại số chuẩn của các ánh xạ liên tục của $X$ vào $\mathbf{C}$ tiến tới 0 ở vô cực. Cho $A$ là một đại số con của $C_0(X)$ phân biệt các điểm của $X$ và sao cho (i) $\overline{f} \in A$ mỗi khi $f \in A$, (ii) với mỗi $x \in X$, tồn tại $f \in A$ sao cho $f(x) \neq 0$. Khi đó $A$ trù mật trong $C_0(X)$.

Nếu $X'$ là không gian compact thu được bằng cách ghép thêm một điểm ở vô cực $\omega$ vào $X$, thì $C_0(X)$ có thể được đồng nhất với không gian con của $C(X; \mathbf{C})$ gồm các ánh xạ liên tục triệt tiêu tại $\omega$, với chuẩn trên $C_0(X)$ được định nghĩa bởi

$$
\|f\| = \sup_{x \in X} |f(x)| = \sup_{x \in X} |f(x)|.
$$

Nhờ Mệnh đề 7, mọi $f \in C_0(X)$ đều có thể được xấp xỉ đều bởi các đa thức với hệ số phức theo các hàm thuộc $A$; hơn nữa, vì $f(\omega) = 0$, lập luận của no. 2, Mệnh đề 4 cho thấy ta có thể giả sử các đa thức này không có số hạng hằng, và khi đó chúng thuộc $A$.

Một ứng dụng khác của Mệnh đề 7 là như sau:

#### Mệnh đề 8 {#top-x-s4-prop-8 .statement}

Cho P là tập của mọi ánh xạ liên tục tuần hoàn của $\mathbf{R}^m$ vào $\mathbf{C}$ mà nhóm chu kỳ của chúng chứa $\mathbf{Z}^m$. Khi đó mọi hàm thuộc P đều có thể được xấp xỉ đều trên $\mathbf{R}^m$ bởi các tổ hợp tuyến tính, với hệ số phức, của các hàm có dạng

$$
(x_1, x_2, \ldots, x_m) \to e(h_1 x_1 + h_2 x_2 + \cdots + h_m x_m),
$$

trong đó các $h_i$ là các số nguyên hữu tỉ (những tổ hợp tuyến tính như thế được gọi là các đa thức lượng giác trong m biến).

Ta chỉ cần nhận thấy rằng P (được trang bị tôpô của sự hội tụ đều) đẳng cấu chính tắc với không gian của mọi ánh xạ liên tục của không gian compact $\mathbf{T}^m$ vào $\mathbf{C}$ (Chương VII, § 1, no. 6), và áp dụng Mệnh đề 7 cho tập các ánh xạ của $\mathbf{T}^m$ vào $\mathbf{C}$ tương ứng với $m$ ánh xạ $(x_1, x_2, \ldots, x_m) \to e(x_i) \quad (1 \leq i \leq m)$ của $\mathbf{R}^m$ vào $\mathbf{C}$.

### Bài tập {#top-x-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
