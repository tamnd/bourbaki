---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 5
section_title: Real-valued functions
lang: vi
source: top-i-iv
pdf_pages: 0353-0365, 0395-0399
extraction: ocr
subsections:
    - "no": 1
      title: REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 353
    - "no": 2
      title: REAL-VALUED FUNCTIONS DEFINED ON A FILTERED SET
      page: 0
      pdf_page: 354
    - "no": 3
      title: LIMITS ON THE RIGHT AND ON THE LEFT OF A FUNCTION OF A REAL VARIABLE
      page: 0
      pdf_page: 355
    - "no": 4
      title: BOUNDS OF A REAL-VALUED FUNCTION
      page: 0
      pdf_page: 356
    - "no": 5
      title: ENVELOPES OF A FAMILY OF REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 358
    - "no": 6
      title: UPPER LIMIT AND LOWER LIMIT OF A REAL-VALUED FUNCTION WITH RESPECT TO A FILTER
      page: 0
      pdf_page: 359
    - "no": 7
      title: ALGEBRAIC OPERATIONS ON REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 362
statements: 30
exercises: 18
content_sha256: 8a67347bcfaa3a526f966d71c19149978cf07be3d947c9d65b10dfb393a61b2a
translated_from: content/en/top/IV/05_s5_real_valued_functions.md
source_content_sha256: f33e039db67c9eaf9660a5f3b5638d6a045e91c9c90c9d92661a758c61127e21
translation_model: gpt-5.4
translation_run: translate-vi-92820145
glossary_version: 34
glossary_terms_sha256: 28db7e1889d5976228a267c90c9adfb65cad49f2e9b43aa469606376848facf1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. CÁC HÀM THỰC

### 1. CÁC HÀM THỰC

#### Định nghĩa 1 {#top-iv-s5-def-1 .statement}

Một ánh xạ của một tập hợp $X$ vào đường thẳng thực được gọi là một hàm thực (hay hàm thực) xác định trên $X$.

Theo một sự lạm dụng ngôn ngữ tương tự như đã nói ở § 4, no. 2, các ánh xạ của $X$ vào $\overline{\mathbf{R}}$ cũng sẽ được gọi là các hàm thực xác định trên $X$ trong tiết này và tiết sau. Các ánh xạ của $X$ vào $\mathbf{R}$ sẽ được gọi là các hàm thực hữu hạn.

Nếu $f$ và $g$ là hai hàm thực xác định trên $X$, thì theo định nghĩa, quan hệ $f \leq g$ tương đương với “$f(x) \leq g(x)$ với mọi $x \in X$;” quan hệ này là một thứ tự trên tập hợp $\overline{\mathbf{R}}^X$ của mọi hàm thực trên $X$. Tập hợp $\overline{\mathbf{R}},^X$ được sắp thứ tự bởi quan hệ này là một dàn; thật vậy, nếu $f$ và $g$ là hai hàm thực bất kỳ, thì hàm $h$ được xác định bởi $h(x) = \sup (f(x), g(x))$ với mọi $x \in X$ là nhỏ nhất trong các hàm thực trên $X$ vừa $\geq f$ vừa $\geq g$; phù hợp với ký hiệu tổng quát, ta ký hiệu hàm này (là cận trên nhỏ nhất của $f$ và $g$ trong $\overline{\mathbf{R}}^X$) bởi $\sup (f, g)$. Tương tự, hàm mà giá trị tại mỗi $x \in X$ là $\inf (f(x), g(x))$ được ký hiệu bởi $\inf (f, g)$.

Chú ý rằng $\sup (f, g)$ là hợp thành của ánh xạ
$$
(u, v) \to \sup (u, v)
$$
từ $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ vào $\overline{\mathbf{R}}$ và ánh xạ $x \to (f(x), g(x))$ từ $X$ vào $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$. Tương tự đối với $\inf (f, g)$.

Một hàm thực $f$ xác định trên một tập hợp $X$ được gọi là *bị chặn trên* (tương ứng, *bị chặn dưới*) trong $X$, nếu $f(X)$ là một tập con của $A'' = [-\infty, +\infty]$ và bị chặn trên (tương ứng, nếu $f(X)$ là một tập con của $A' = ]-\infty, +\infty]$ và bị chặn dưới). $f$ được gọi là *bị chặn* trong $X$ nếu nó bị chặn cả trên lẫn dưới, nghĩa là nếu $f(X)$ là một tập con bị chặn của $\mathbf{R}$.

Do đó mọi hàm bị chặn đều *hữu hạn*. Đảo lại là sai, như được chỉ ra bởi hàm $1/x$ trên $\mathbf{R}_+^* = ]0, +\infty[$.

### 2. HÀM THỰC XÁC ĐỊNH TRÊN MỘT TẬP HỢP ĐƯỢC LỌC

#### Mệnh đề 1 {#top-iv-s5-prop-1 .statement}

*Cho $f$ và $g$ là hai hàm thực xác định trên một tập hợp $X$ được lọc bởi một bộ lọc $\mathfrak{F}$. Nếu $\lim_{\mathfrak{F}} f$ và $\lim_{\mathfrak{F}} g$ tồn tại, và nếu, với mỗi tập con $A \in \mathfrak{F}$, tồn tại $x \in A$ sao cho $f(x) \leq g(x)$, thì ta có $\lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g$.*

Để chứng minh kết quả này, ta sẽ chứng minh mệnh đề tương đương sau:

#### Mệnh đề 2 {#top-iv-s5-prop-2 .statement}

*Cho $f$ và $g$ là hai hàm thực xác định trên một tập hợp $X$ được lọc bởi một bộ lọc $\mathfrak{F}$. Nếu $\lim_{\mathfrak{F}} f$ và $\lim_{\mathfrak{F}} g$ tồn tại, và nếu $\lim_{\mathfrak{F}} f > \lim_{\mathfrak{F}} g$, thì tồn tại một tập hợp $A \in \mathfrak{F}$ sao cho $f(x) > g(x)$ với mọi $x \in A$.*

Cho $a = \lim_{\mathfrak{F}} f$, $b = \lim_{\mathfrak{F}} g$ và $c$ sao cho $b < c < a$. Khoảng $]c, +\infty]$ của $\overline{\mathbf{R}}$ (tương ứng $]-\infty, c[$) là một lân cận của $a$ (tương ứng của $b$); do đó tồn tại một tập hợp $M \in \mathfrak{F}$ (tương ứng một tập hợp $N \in \mathfrak{F}$) sao cho $f(x) > c$ với mọi $x \in M$ [tương ứng $g(x) < c$ với mọi $x \in N$]. Tập hợp $A = M \cap N$ thuộc $\mathfrak{F}$, và ta có $f(x) > c > g(x)$ với mọi $x \in A$.

Như một trường hợp riêng của Mệnh đề 1, ta có định lý sau:

#### Định lý 1 (Nguyên lý mở rộng các bất đẳng thức) {#top-iv-s5-thm-1 .statement}

*Cho $f$ và $g$ là hai hàm số thực, xác định trên một tập hợp $X$ được lọc bởi một bộ lọc $\mathfrak{F}$. Nếu $\lim_{\mathfrak{F}} f$ và $\lim_{\mathfrak{F}} g$ tồn tại, và nếu $f \leq g$, thì $\lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g$.*

#### Nhận xét {#top-iv-s5-n2-rem-1 .statement}

Nếu riêng ta có $f(x) < g(x)$ với mọi $x \in X$ (hoặc chỉ với mọi điểm của một tập hợp thuộc bộ lọc $\overline{\mathbf{R}}$) thì theo Định lý 1, ta suy ra được rằng $\lim_{\mathfrak{F}} f \leq \lim_{\mathfrak{F}} g$; *nhưng không thể suy ra bất đẳng thức ngặt* $\lim_{\mathfrak{F}} f < \lim_{\mathfrak{F}} g$. Ví dụ, nếu lấy $X$ là tập hợp $\mathbf{N}$ các số tự nhiên, được lọc bởi bộ lọc Fréchet, và nếu $f(n) = 0$ và $g(n) = 1/n$, thì $f(n) < g(n)$ với mọi $n$, nhưng $\lim_{n \to \infty} f(n) = \lim_{n \to \infty} f(n) = 0$. Như vậy ta *mất tính ngặt* khi chuyển sang giới hạn trong một bất đẳng thức *ngặt*.

Giả sử chẳng hạn $f$ là tăng, và đặt $a = \sup f(A)$. Nếu $a = -\infty$, định lý là tầm thường. Nếu $a > -\infty$, thì với mỗi $b < a$ tồn tại $x \in A$ sao cho $b < f(x) \leq a$; do đó, nếu $S_x$ là tiết diện của $A$ tương đối với $x$ (tức là tập hợp mọi $y \geq x$, xem Chương I, § 6, no. 3), thì $f(S_x)$ được chứa trong lân cận $]b, +\infty]$ của $a$, và định lý suy ra. Chứng minh là tương tự nếu $f$ là giảm.

#### Hệ quả {#top-iv-s5-n2-cor-1 .statement}

Một hàm tăng (tương ứng, giảm) nhận giá trị thực, được xác định trên một tập con có hướng $A$ của một tập hợp có thứ tự $X$, có một giới hạn hữu hạn đối với $A$ khi và chỉ khi nó bị chặn trên (tương ứng, bị chặn dưới) trong $A$.

Nếu ta áp dụng Định lý 2 cho trường hợp $A = X = \mathbf{N}$ (được sắp thứ tự bởi quan hệ $\leq$), ta có mệnh đề sau:

#### Mệnh đề 3 {#top-iv-s5-prop-3 .statement}

Mọi dãy đơn điệu các số thực đều có một giới hạn trong $\overline{\mathbf{R}}$.
Đặc biệt, mọi dãy tăng (tương ứng, giảm) gồm các số hữu hạn đều hội tụ đến một số thực hữu hạn nếu nó bị chặn trên (tương ứng, bị chặn dưới), và hội tụ đến $+\infty$ (tương ứng, $-\infty$) trong trường hợp ngược lại. Ví dụ, dãy các số nguyên dương hội tụ đến $+\infty$.

Sự kiện này là nguồn gốc của ký hiệu $\lim_{n \to \infty} u_n$ để chỉ giới hạn của một dãy (Chương I, § 7, no. 3).

Tương tự, mọi dãy tăng ngặt các số nguyên $(p_n)$ đều hội tụ đến $+\infty$; thật vậy, ta thấy bằng quy nạp rằng $p_n \geq p_0 + n$ với mọi $n$.

### 3. GIỚI HẠN BÊN PHẢI VÀ BÊN TRÁI CỦA MỘT HÀM CỦA BIẾN THỰC

Cho $A$ là một tập con không rỗng của $\overline{\mathbf{R}}$ và cho $a \neq -\infty$ là một điểm của $\overline{\mathbf{R}}$ nằm trong bao đóng của tập hợp $B = A \cap [-\infty, a[$. Tập hợp $B$ là có hướng đối với quan hệ $\leq$, và bộ lọc tiết diện của nó $\mathfrak{F}$ cũng chính là vết trên $B$ của bộ lọc các lân cận của $a$ trong $\overline{\mathbf{R}}$.

(*) Mệnh đề này ngầm giả thiết rằng thứ tự trong $X$ được viết là $x \leq y$. Nếu quan hệ này được viết là $x(\sigma) y$, trong đó $(\sigma)$ là một dấu hoặc một nhóm dấu đặc trưng cho quan hệ đang xét, thì từ "có hướng" trong mệnh đề phải được thay bằng "có hướng đối với $(\sigma)$".

#### Định nghĩa 2 {#top-iv-s5-def-2 .statement}

*Cho f là một hàm xác định trên một tập con không rỗng A của $\overline{\mathbf{R}}$, nhận giá trị trong một không gian tôpô X. Một giới hạn của f đối với bộ lọc $\mathfrak{F}$, nếu tồn tại, được gọi là giới hạn bên trái của f tại điểm a, tương đối với A, và được ký hiệu là*
$$
\lim_{x \to a,\ x < a,\ x \in A} f(x),
$$
*hoặc $f(a-)$, nếu X là Hausdorff.*

Tương tự, nếu $a$ thuộc bao đóng của tập $A \cap ]a, + \infty]$, thì ta định nghĩa một *giới hạn bên phải* (nếu tồn tại) của $f$ tại điểm $a$, và ký hiệu nó bởi
$$
\lim_{x \to a,\ x > a,\ x \in A} f(x),
$$
*hoặc $f(a+)$, nếu X là Hausdorff.*

Mệnh đề sau là một hệ quả ngay lập tức của Định lý 2:

#### Mệnh đề 4 {#top-iv-s5-prop-4 .statement}

*Nếu A là một tập con của $\overline{\mathbf{R}}$ và $a \neq -\infty$ là một điểm thuộc bao đóng của giao $A \cap [-\infty, a[$, thì mọi hàm thực đơn điệu f xác định trên A đều có một giới hạn bên trái $f(a-)$ tại a, đối với A.*

### 4. CẬN CỦA MỘT HÀM THỰC

#### Định nghĩa 3 {#top-iv-s5-def-3 .statement}

*Cho f là một hàm thực xác định trên một tập hợp X, và A là một tập con không rỗng của X. Khi đó cận trên nhỏ nhất (tương ứng, cận dưới lớn nhất) của tập $f(A)$ trong $\overline{\mathbf{R}}$ được gọi là cận trên nhỏ nhất (tương ứng, cận dưới lớn nhất) của f trên A, và được ký hiệu bởi*
$$
\sup_{x \in A} f(x) \quad \text{[resp. } \inf_{x \in A} f(x) \text{]}.
$$

Đặc biệt, nếu A là một tập con không rỗng của $\overline{\mathbf{R}}$, thì
$$(1)$$
$$
\sup A = \sup_{x \in A} x.
$$
Thường thuận tiện hơn khi dùng ký hiệu ở vế phải để chỉ cận trên nhỏ nhất của A.

Số $a = \sup_{x \in A} f(x)$ được đặc trưng bởi hai tính chất sau:
(i) Với mọi $x \in A, f(x) \leq a$.
(ii) Với mọi $b < a$, tồn tại $x \in A$ sao cho $b < f(x) \leq a$.

Các số $\sup_{x \in A} f(x)$ và $\inf_{x \in A} f(x)$ thuộc *bao đóng* của $f(A)$ trong $\overline{\mathbf{R}}$. Ta có $\inf_{x \in A} f(x) \leq \sup_{x \in A} f(x)$; và hai số này *bằng nhau* khi và chỉ khi $f$ là *hằng* trên A.

Một hàm nhận giá trị thực, xác định trên một tập hợp X, được gọi là *bị chặn trên* (tương ứng, *bị chặn dưới*) trong một tập con không rỗng A của X khi và chỉ khi $\sup_{x \in A} f(x) < + \infty$ [tương ứng, $\inf_{x \in A} f(x) > -\infty$]. $f$ *bị chặn* trong A khi và chỉ khi $|f|$ bị chặn trên trong A, do đó khi và chỉ khi $\sup_{x \in A} |f(x)| < + \infty$.

Ta có

$$
\inf_{x \in A} f(x) = -\sup_{x \in A} (-f(x)).
$$

Quan hệ này quy tất cả các tính chất của cận dưới lớn nhất về các tính chất của cận trên bé nhất; vì thế nói chung ta sẽ chỉ nói đến cái sau.

#### Mệnh đề 5 {#top-iv-s5-prop-5 .statement}

*Cho $f$ là một hàm thực định nghĩa trên một tập hợp $X$. Trên tập hợp $\mathcal{F}(X)$ gồm mọi tập con hữu hạn của $X$, có hướng đối với quan hệ $\subset$, hàm thực $H \to \sup_{x \in H} f(x)$ là tăng, hàm thực $H \to \inf_{x \in H} f(x)$ là giảm, và ta có*

$$
\begin{cases}
\sup_{x \in A} f(x) = \lim_{H \in \mathcal{F}(X)} (\sup_{x \in H} f(x)), \\
\inf_{x \in A} f(x) = \lim_{H \in \mathcal{F}(X)} (\inf_{x \in H} f(x)).
\end{cases}
$$

Đặt $\varphi(H) = \sup_{x \in H} f(x)$. Rõ ràng $\varphi$ tăng, và do đó có một giới hạn $a$ (no. 2, Định lý 2); và vì $\varphi(H) \leq \sup_{x \in A} f(x)$ với mọi $H$, ta có $a \leq \sup_{x \in A} f(x)$ (no. 2, Định lý 1). Nếu ta có $a < \sup_{x \in A} f(x)$, thì sẽ tồn tại $x_0 \in X$ sao cho $a < f(x_0)$; nhưng điều này là mâu thuẫn vì $\varphi(H) \geq f(x_0)$ mỗi khi $x_0 \in H$.

Đặc biệt, theo (1), nếu $A$ là một tập con không rỗng bất kỳ của $\overline{\mathbf{R}}$, ta có

$$
\sup A = \lim_{H \in \mathcal{F}(A)} (\sup_{x \in H} x).
$$

#### Mệnh đề 6 {#top-iv-s5-prop-6 .statement}

*Cho $f$ và $g$ là hai hàm thực xác định trên $X$. Nếu $f(x) \leq g(x)$ tại mọi điểm $x$ của một tập con không rỗng $A$ của $X$, thì ta có*

$$
\begin{cases}
\sup_{x \in A} f(x) \leq \sup_{x \in A} g(x), \\
\inf_{x \in A} f(x) \leq \inf_{x \in A} g(x).
\end{cases}
$$

#### Mệnh đề 7 {#top-iv-s5-prop-7 .statement}

*Cho $f$ là một hàm thực xác định trên $X$. Nếu $A$ và $B$ là hai tập con không rỗng của $X$ sao cho $A \subset B$, thì*

$$
\sup_{x \in A} f(x) \leq \sup_{x \in B} f(x).
$$

#### Mệnh đề 8 {#top-iv-s5-prop-8 .statement}

*Cho $f$ là một hàm nhận giá trị thực được xác định trên $X$, và cho $(A_i)_{i \in I}$ là một họ không rỗng các tập con không rỗng của $X$; khi đó*

$$
\sup_{x \in \bigcup_{i \in I} A_i} f(x) = \sup_{i \in I} (\sup_{x \in A_i} f(x)).
$$

Cho $f$ là một hàm nhận giá trị thực được xác định trên một tập hợp tích $X_1 \times X_2$. Nếu $A_2$ là một tập con không rỗng của $X_2$ thì ta sẽ ký hiệu bởi $\sup_{x_1 \in A_2} f(x_1, x_2)$ cận trên bé nhất trên $A_2$ của hàm nhận giá trị thực $x_2 \to f(x_1, x_2)$ được xác định trên $X_2$. Từ Mệnh đề 8 ta suy ra đặc biệt:

#### Mệnh đề 9 {#top-iv-s5-prop-9 .statement}

*Cho $f$ là một hàm thực-valued được xác định trên một tập hợp tích $X_1 \times X_2$. Nếu $A_1, A_2$ lần lượt là các tập hợp con không rỗng bất kỳ của $X_1, X_2$, thì*

$$
\sup_{(x_1, x_2) \in A_1 \times A_2} f(x_1, x_2) = \sup_{x_1 \in A_1} (\sup_{x_2 \in A_2} f(x_1, x_2)) = \sup_{x_2 \in A_2} (\sup_{x_1 \in A_1} f(x_1, x_2)).
$$

### 5. BAO CỦA MỘT HỌ CÁC HÀM THỰC-VALUED

#### Định nghĩa 4 {#top-iv-s5-def-4 .statement}

*Cho $(f_i)_{i \in I}$ là một họ các hàm thực xác định trên một tập hợp $X$. Hàm thực trên $X$ mà giá trị tại mỗi điểm $x \in X$ là $\sup_{i \in I} (f_i(x))$ [tương ứng là $\inf_{i \in I} (f_i(x))$] được gọi là bao trên (tương ứng, bao dưới) của họ $(f_i)$, và được ký hiệu bởi $\sup_{i \in I} f_i$ hoặc $\sup_i f_i$ (tương ứng $\inf_{i \in I} f_i$ hoặc $\inf_i f_i$).

Như vậy, bao trên của họ $(f_i)$ là cận trên bé nhất của họ này trong dàn $\overline{\mathbf{R}}$ các hàm thực xác định trên $X$, và điều đó biện minh cho ký hiệu $\sup_{i \in I} f_i$.

Hơn nữa, nếu ta trang bị cho $\overline{\mathbf{R}}^X$ tôpô là tích của các tôpô trên các nhân tử của nó (tất cả đều đồng nhất với $\overline{\mathbf{R}}$), thì ta có mệnh đề sau:

#### Mệnh đề 10 {#top-iv-s5-prop-10 .statement}

*Trong không gian tích $\overline{\mathbf{R}}^X$, bao trên $\sup_{i \in I} f_i$ của một họ các hàm thực $(f_i)_{i \in I}$ là giới hạn, đối với tập có hướng $\mathcal{F}(I)$ các tập con hữu hạn của $I$, của ánh xạ $H \to \sup_{i \in H} f_i$ [ánh xạ này gán cho mỗi tập con hữu hạn $H$ của $I$ bao trên của họ con hữu hạn $(f_i)_{i \in H}$].

Điều này suy ra ngay lập tức từ Mệnh đề 5 của no. 4 và từ Chương I, § 7, no. 6, Hệ quả 1 của Mệnh đề 10.

Vì vậy ta có thể viết

$$
\sup_{i \in I} f_i = \lim_{H \in \mathcal{F}(I)} (\sup_{i \in H} f_i).
$$

#### Định nghĩa 5 {#top-iv-s5-def-5 .statement}

*Một họ $(f_i)_{i \in I}$ các hàm nhận giá trị thực xác định trên một tập hợp $X$ được gọi là bị chặn đều trên (resp. bị chặn đều dưới) trong $X$, nếu tồn tại một số hữu hạn $a$ sao cho $f_i(x) \leq a$ [resp. $f_i(x) \geq a$] với mọi $x \in X$ và mọi $i \in I$. Họ $(f_i)$ được gọi là bị chặn đều trong $X$ nếu nó bị chặn đều trên và bị chặn đều dưới trong $X$.

Do đó $(f_i)$ bị chặn trên đều trong $X$ khi và chỉ khi bao trên của họ này bị chặn trên trong $X$. $(f_i)$ bị chặn đều trong $X$ khi và chỉ khi bao trên của họ $(|f_i|)$ bị chặn trên trong $X$ [tức là khi và chỉ khi tồn tại một số thực hữu hạn $a \geq 0$ sao cho $|f_i(x)| \leq a$ với mọi $x \in X$ và mọi $i \in I$].

### 6. GIỚI HẠN TRÊN VÀ GIỚI HẠN DƯỚI CỦA MỘT HÀM SỐ THỰC ĐỐI VỚI MỘT BỘ LỌC

Cho $f$ là một hàm thực xác định trên một tập hợp $X$ được lọc bởi một bộ lọc $\mathcal{G}$. $\mathcal{G}$ là một tập có hướng đối với quan hệ $\supseteq$ (Chương I, § 6). Với mỗi $M \in \mathcal{G}$ xét số thực $\sup_{x \in M} f(x)$: ta có một hàm $M \to \sup_{x \in M} f(x)$ từ $\mathcal{G}$ vào $\overline{\mathbf{R}}$, là một hàm giảm trên $\mathcal{G}$, theo Mệnh đề 7 của no. 4. Do đó, theo Định lý 2 của no. 2, nó có một giới hạn đối với tập có hướng $\mathcal{G}$.

#### Định nghĩa 6 {#top-iv-s5-def-6 .statement}

*Giới hạn của hàm thực* $M \to \sup_{x \in M} f(x)$ *đối với tập có hướng* $\mathcal{G}$ *được gọi là giới hạn trên của* $f$ *đối với bộ lọc* $\mathcal{G}$, *và được ký hiệu là* $\lim \sup_{\mathcal{G}} f$, *hoặc* $\lim \sup_{x, \mathcal{G}} f(x)$.

*Giới hạn dưới* của $f$ đối với bộ lọc $\mathcal{G}$ được định nghĩa tương tự, và được ký hiệu là $\lim \inf_{\mathcal{G}} f$ hoặc $\lim \inf_{x, \mathcal{G}} f(x)$. Như vậy ta có

$$
\begin{cases}
\lim \sup_{\mathcal{G}} f = \lim_{M \in \mathcal{G}} (\sup_{x \in M} f(x)), \\
\lim \inf_{\mathcal{G}} f = \lim_{M \in \mathcal{G}} (\inf_{x \in M} f(x)).
\end{cases}
$$

(10)

Thường bộ lọc $\mathcal{G}$ được lược bỏ khỏi ký hiệu, và ta viết đơn giản $\lim \sup f$ hoặc $\lim \sup_{x} f(x)$, hoặc $\lim \sup f(x)$ khi không có nguy cơ nhầm lẫn.

Từ các công thức (10) và Định lý 1 ta có

$$
\inf_{x \in X} f(x) \leq \lim \inf_{\mathcal{G}} f \leq \lim \sup_{\mathcal{G}} f \leq \sup_{x \in X} f(x).
$$

(11)

Theo Định lý 2 của no. 2, ta cũng có thể viết

$$
\begin{cases}
\lim \sup_{\mathcal{G}} f = \inf_{M \in \mathcal{G}} (\sup_{x \in M} f(x)), \\
\lim \inf_{\mathcal{G}} f = \sup_{M \in \mathcal{G}} (\inf_{x \in M} f(x)).
\end{cases}
$$

(12)

Ta cũng có thể thay thế bộ lọc $\mathcal{G}$, ở các vế phải của các công thức (10) và (12), bằng bất kỳ *cơ sở* nào $\mathcal{B}$ của $\mathcal{G}$.

Từ (2) và (10),

$$
\lim \inf_{\mathcal{G}} f = -\lim \sup_{\mathcal{G}} (-f)
$$

và do đó ta chỉ cần xét giới hạn trên.

#### Định lý 3 {#top-iv-s5-thm-3 .statement}

*Giới hạn trên của một hàm giá trị thực $f$ đối với một bộ lọc $\mathcal{G}$ bằng giá trị giới hạn lớn nhất của $f$ đối với $\mathcal{G}$.*

Cho $b$ là một điểm tụ của $f$ đối với $\mathcal{G}$. Với mỗi $M \in \mathcal{G}$, $b$ nằm trong bao đóng của $f(M)$, do đó $b \leq \sup_{x \in M} f(x)$, và vì thế, theo (12),
$b \leq \lim \sup_{\mathcal{G}} f = a.$

Mặt khác, cho $V$ là một lân cận mở bất kỳ của $a$ trong $\overline{\mathbf{R}}$. Khi đó tồn tại một tập $M_0$ trong $\mathcal{G}$ sao cho, với mỗi $M \in \mathcal{G}$ được chứa trong $M_0$, ta có $\sup_{x \in M} f(x) \in V$; vì $V$ là mở nên suy ra $f(M)$ cắt $V$, và do đó $a$ là một *điểm tụ* của $f$ đối với $\mathcal{G}$, và chứng minh đã hoàn tất.

#### Hệ quả 1 {#top-iv-s5-thm-3-cor-1 .statement}

*Để $\lim \sup_{\mathcal{G}} f = \lim \inf_{\mathcal{G}} f$, điều kiện cần và đủ là $f$ có giới hạn đối với bộ lọc $\mathcal{G}$, và khi đó*
$$
\lim_{\mathcal{G}} f = \lim \sup_{\mathcal{G}} f = \lim \inf_{\mathcal{G}} f.
$$
Thật vậy, vì $\overline{\mathbf{R}}$ là compact, cơ sở bộ lọc $f(\mathcal{G})$ có một điểm giới hạn khi và chỉ khi nó chỉ có một điểm tụ (Chương I, § 9, no. 1, Hệ quả của Định lý 1).

#### Hệ quả 2 {#top-iv-s5-thm-3-cor-2 .statement}

*Nếu $\mathcal{H}$ là một bộ lọc mịn hơn $\mathcal{G}$, thì ta có*
$$
\lim \inf_{\mathcal{G}} f \leq \lim \inf_{\mathcal{H}} f \leq \lim \sup_{\mathcal{H}} f \leq \lim \sup_{\mathcal{G}} f.
$$
Mọi điểm tụ của $f$ đối với $\mathcal{H}$ cũng là một điểm tụ của $f$ đối với $\mathcal{G}$ (Chương I, § 7, no. 3).
Đặc biệt, nếu $\lim_{\mathcal{G}} f$ tồn tại, thì
$$
\lim \inf_{\mathcal{G}} f \leq \lim_{\mathcal{G}} f \leq \lim \sup_{\mathcal{G}} f.
$$

#### Hệ quả 3 {#top-iv-s5-thm-3-cor-3 .statement}

*Cho $A$ là một tập hợp của bộ lọc $\mathcal{G}$, $\mathcal{G}_A$ là bộ lọc cảm sinh trên $A$ bởi $\mathcal{G}$, và $f_A$ là hạn chế của $f$ lên $A$; khi đó*
$$
\lim \sup_{\mathcal{G}_A} f_A = \lim \sup_{\mathcal{G}} f.
$$
Mọi điểm tụ của cơ sở bộ lọc $f(\mathcal{G})$ đều là một điểm tụ của cơ sở bộ lọc $f_A(\mathcal{G}_A)$, và ngược lại.

Vì lý do này, nếu $f$ chỉ được xác định trên một tập con $A$ của $X$ thuộc $\mathcal{G}$, thì ta sẽ thường viết $\limsup_{\mathcal{G}} f$ thay cho $\limsup_{\mathcal{G}_A} f_A$, do lạm dụng ngôn ngữ.

#### Mệnh đề 11 {#top-iv-s5-prop-11 .statement}

Cho $f$ và $g$ là hai hàm số thực xác định trên một tập lọc $X$. Khi đó quan hệ $f \leq g$ kéo theo

$$
\begin{cases}
\limsup f \leq \limsup g, \\
\liminf f \leq \liminf g.
\end{cases}
$$

Đây là một hệ quả ngay lập tức của các quan hệ (12).

Khi $X$ là một không gian tôpô và $\mathcal{G}$ là bộ lọc lân cận của một điểm $a$ của $X$, ta viết $\limsup_{x \to a} f(x)$ [resp. $\liminf_{x \to a} f(x)$] thay cho $\limsup_{\mathcal{G}} f$ [resp. $\liminf_{\mathcal{G}} f$]; rõ ràng ta có

$$
\liminf_{x \to a} f(x) \leq f(a) \leq \limsup_{x \to a} f(x).
$$

Nói chung hơn, nếu $X$ là một không gian con của một không gian tôpô $Y$, và nếu $\mathcal{G}$ là vết trên $X$ của bộ lọc lân cận của một điểm $a \in \overline{X}$, ta viết $\limsup_{x \to a, x \in X} f(x)$ [tương ứng, $\liminf_{x \to a, x \in X} f(x)$] thay cho $\limsup_{\mathcal{G}} f$ [tương ứng, $\liminf_{\mathcal{G}} f$] ; $\limsup$ được gọi là giới hạn trên của $f(x)$ khi $x$ tiến tới $a$ mà vẫn thuộc $X$. Nếu $X$ là phần bù của $\{a\}$ thì trong các ký hiệu này ta viết "x \neq a" thay cho "x \in X".

Nếu $A$ là một tập con của $X$ sao cho $a \in \overline{A}$, thì (Hệ quả 2 của Định lý 3)

$$
\liminf_{x \to a, x \in X} f(x) \leq \liminf_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in X} f(x).
$$

Nếu $V$ là một lân cận của $a$ trong $Y$, ta có (Hệ quả 3 của Định lý 3)

$$
\limsup_{x \to a, x \in V \cap X} f(x) = \limsup_{x \to a, x \in X} f(x).
$$

Vì thế các khái niệm giới hạn trên và giới hạn dưới tại một điểm của một không gian tôpô, cũng như khái niệm giới hạn, đều có đặc trưng địa phương.

Cuối cùng, nếu $\mathcal{G}$ là bộ lọc Fréchet trên $\mathbf{N}$, thì giới hạn trên (tương ứng, giới hạn dưới), đối với $\mathcal{G}$, của ánh xạ $n \to u_n$ từ $\mathbf{N}$ vào $\overline{\mathbf{R}}$ được ký hiệu bởi $\limsup_{n \to \infty} u_n$ (tương ứng, $\liminf_{n \to \infty} u_n$) và được gọi là giới hạn trên (tương ứng, giới hạn dưới) của dãy các số thực $u_n$.

Vậy quan hệ $\limsup_{n \to \infty} u_n = a \in \mathbf{R}$ tương đương với điều sau đây: với mọi $\varepsilon > 0$ tồn tại một số nguyên $n_0$ sao cho, với mọi $n \geq n_0$ ta có $u_n \leq a + \varepsilon$, và với vô hạn giá trị của $n$ ta có $u_n \geq a - \varepsilon$. Định nghĩa của giới hạn trên của một dãy có thể được phát biểu tương tự khi giá trị của nó là $+\infty$ hoặc $-\infty$.

Cho một dãy $(f_n)$ các hàm thực xác định trên một tập hợp $X$, ta ký hiệu bởi $\limsup_{n \to \infty} f_n$ (resp. $\liminf_{n \to \infty} f_n$) hàm thực có giá trị tại mọi điểm $x \in X$ là $\limsup_{n \to \infty} f_n(x)$ [resp. $\liminf_{n \to \infty} f_n(x)$]. Từ (10) và (12) ta suy ra
$$
\begin{cases}
\limsup_{n \to \infty} f_n = \inf_{n \in \mathbf{N}} (\sup_{m \geq n} f_m) = \lim_{n \to \infty} (\sup_{m \geq n} f_m), \\
\liminf_{n \to \infty} f_n = \sup_{n \in \mathbf{N}} (\inf_{m \geq n} f_m) = \lim_{n \to \infty} (\inf_{m \geq n} f_m),
\end{cases}
$$
các giới hạn được lấy trong *không gian tích* $\overline{\mathbf{R}}^X$. Dãy $(f_n)$ có một *giới hạn* trong $\overline{\mathbf{R}}^X$ khi và chỉ khi $\limsup_{n \to \infty} f_n = \liminf_{n \to \infty} f_n$ (Hệ quả 1 của Định lý 3, và Chương I, § 7, no. 6, Hệ quả 1 của Mệnh đề 10).

### 7. CÁC PHÉP TOÁN ĐẠI SỐ TRÊN CÁC HÀM THỰC

Cho $f$ và $g$ là hai hàm thực xác định trên một tập hợp $X$; nếu tổng $f(x) + g(x)$ [resp. tích $f(x)g(x)$] được xác định với mọi $x \in X$, thì ta ký hiệu bởi $f + g$ (resp. $fg$) hàm thực
$$
x \mapsto f(x) + g(x) \quad \text{[resp. } x \mapsto f(x)g(x)].
$$
Tương tự, nếu $1/f(x)$ được xác định với mọi $x \in X$, thì $1/f$ ký hiệu hàm $x \mapsto 1/f(x)$.

Vậy hàm cuối cùng này được xác định miễn là $f$ không nhận giá trị 0; khi $f$ nhận các giá trị trong khoảng $[0, +\infty]$ (resp. trong $[-\infty, 0]$) $1/f(x)$ được xem là xác định khắp nơi bằng cách đặt $1/0 = +\infty$ (resp. $1/0 = -\infty$); trong trường hợp này hàm $1/f$ được xác định.

Giả sử rằng $X$ được lọc bởi một bộ lọc $\mathcal{F}$, và rằng $\lim_{\mathcal{F}} f$ và $\lim_{\mathcal{F}} g$ tồn tại. Nếu một mặt hàm $f + g$ (tương ứng $fg$, $1/g$) được xác định, và nếu mặt khác biểu thức $\lim_{\mathcal{F}} f + \lim_{\mathcal{F}} g$ (tương ứng $\lim_{\mathcal{F}} f \cdot \lim_{\mathcal{F}} g$, $1/\lim_{\mathcal{F}} f$) có nghĩa, thì $\lim_{\mathcal{F}} (f + g)$ [tương ứng $\lim_{\mathcal{F}} fg$, $\lim_{\mathcal{F}} (1/f)$] tồn tại và bằng biểu thức ấy do tính liên tục của hàm $x + y$ (tương ứng $xy$, $1/x$) tại các điểm mà nó được xác định.

#### Mệnh đề 12 {#top-iv-s5-prop-12 .statement}

*Cho $f$ và $g$ là hai hàm thực được xác định trên một tập hợp $X$, và cho $A$ là một tập con không rỗng của $X$.*

(i) *Ta có*
$$
\begin{align*}
&\sup_{x \in A} (f(x) + g(x)) \leq \sup_{x \in A} f(x) + \sup_{x \in A} g(x), \\
&\sup_{x \in A} f(x) + \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x) + g(x)),
\end{align*}
$$
*mỗi khi hai vế của các bất đẳng thức này đều được xác định.*

(ii) *Nếu $f(x)$ và $g(x)$ là $\geq 0$ với mỗi $x \in A$, thì*

(19)
$$
\sup_{x \in A} (f(x)g(x)) \leq \sup_{x \in A} f(x) \sup_{x \in A} g(x),
$$
(20)
$$
\sup_{x \in A} f(x) \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x)g(x))
$$
*mỗi khi hai vế của các bất đẳng thức này đều được xác định.*

(iii) *Nếu $f(x) \geq 0$ với mọi $x \in A$, thì*
(21)
$$
\sup_{x \in A} (1/f(x)) = 1/\inf_{x \in A} f(x)
$$
*(quy ước $1/0 = +\infty$).*

Cho $H$ là một tập con *hữu hạn* bất kỳ của $A$. Nếu $x_0$ là một trong những điểm của $H$ tại đó $f + g$ đạt giá trị lớn nhất của nó, thì ta có
$$
f(x_0) + g(x_0) \leq \sup_{x \in H} f(x) + \sup_{x \in H} g(x);
$$
mặt khác, nếu $x_1$ là một trong những điểm của $H$ tại đó $f$ đạt giá trị lớn nhất của nó, thì
$$
f(x_1) + g(x_1) \geq \sup_{x \in H} f(x) + \inf_{x \in H} g(x);
$$
do đó
$$
\sup_{x \in H} f(x) + \inf_{x \in H} g(x) \leq \sup_{x \in H} (f(x) + g(x)) \leq \sup_{x \in H} f(x) + \sup_{x \in H} g(x).
$$
Các bất đẳng thức (17) và (18) suy ra từ đây bằng cách áp dụng Mệnh đề 5 của no. 4 và Định lý 1 của no. 2. Chứng minh của các bất đẳng thức khác là tương tự.

#### Hệ quả 1 {#top-iv-s5-prop-12-cor-1 .statement}

*Cho $f$ là một hàm nhận giá trị thực xác định trên $X$, và cho $k$ là một số thực. Khi đó*
(22)
$$
\sup_{x \in A} (f(x) + k) = k + \sup_{x \in A} f(x)
$$
*miễn là cả hai vế đều xác định, và, nếu $k \geq 0,$*
(23)
$$
\sup_{x \in A} (kf(x)) = k \cdot \sup_{x \in A} f(x)
$$
*miễn là cả hai vế đều xác định.*

#### Hệ quả 2 {#top-iv-s5-prop-12-cor-2 .statement}

*Cho $f_1$ và $f_2$ là hai hàm nhận giá trị thực xác định lần lượt trên các tập hợp $X_1, X_2$; khi đó nếu $A_1, A_2$ là các tập con không rỗng bất kỳ của $X_1, X_2$ tương ứng, ta có*
(24)
$$
\sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1) + f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) + \sup_{x_2 \in A_2} f_2(x_2)
$$

miễn là cả hai vế đều xác định; và nếu $f_1, f_2$ đều $\geq 0$ trong $A_1, A_2$ tương ứng thì ta có

$$
(25) \quad \sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1)f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) \sup_{x_2 \in A_2} f_2(x_2),
$$

mỗi khi cả hai vế đều xác định.

Đây là một hệ quả ngay lập tức của hệ quả trước đó và Mệnh đề 9 của no. 4.

Đặc biệt, nếu $A$ và $B$ là hai tập hợp con của $\overline{\mathbf{R}}$ sao cho tập hợp $A + B$ các tổng $x + y \ (x \in A, y \in B)$ được xác định, thì ta có

$$
(26) \quad \sup (A + B) = \sup A + \sup B
$$

nếu vế phải được xác định. Tương tự, nếu $A$ và $B$ là hai tập hợp con của $[0, + \infty]$, thì ta có

$$
(27) \quad \sup AB = \sup A \cdot \sup B
$$

mỗi khi cả hai vế đều xác định.

#### Mệnh đề 13 {#top-iv-s5-prop-13 .statement}

*Cho $f$ và $g$ là hai hàm số thực xác định trên một tập hợp lọc $X$.*

(i) *Ta có*

$$
(28) \quad \lim \sup (f + g) \leq \lim \sup f + \lim \sup g,
$$
$$
(29) \quad \lim \sup f + \lim \inf g \leq \lim \sup (f + g)
$$

*mỗi khi cả hai vế của các bất đẳng thức này đều xác định được.*

(ii) *Nếu $f$ và $g$ là $\geq 0$ trên $X$, ta có*

$$
(30) \quad \lim \sup fg \leq (\lim \sup f) (\lim \sup g),
$$
$$
(31) \quad (\lim \sup f) (\lim \inf g) \leq \lim \sup fg
$$

*mỗi khi cả hai vế của các bất đẳng thức này đều xác định được.*

(iii) *Nếu $f \geq 0$ trên $X$, thì*

$$
(32) \quad \lim \sup (1/f) = 1/(\lim \inf f)
$$

(đặt $1/0 = + \infty$).

Các hệ thức này là hệ quả của Mệnh đề 12 và các hệ thức (10)

#### Hệ quả 1 {#top-iv-s5-prop-13-cor-1 .statement}

*Cho $f$ và $g$ là hai hàm thực xác định trên một tập hợp lọc $X$. Nếu $\lim g$ tồn tại, thì*

$$
(33) \quad \lim \sup (f + g) = \lim \sup f + \lim g
$$

*khi cả hai vế đều xác định, và*

(34) $$
\lim \sup fg = (\lim \sup f) (\lim g)
$$

*khi cả hai vế đều xác định và $f$ và $g$ đều $\geqslant 0$.*

#### Hệ quả 2 {#top-iv-s5-prop-13-cor-2 .statement}

Cho $f$ và $g$ là hai hàm thực nhận giá trị thực xác định trên một tập hợp được lọc $X$. Nếu $\lim f = +\infty$ và $\lim \inf g > -\infty$ và $f + g$ được xác định, thì $\lim (f + g) = +\infty$. Nếu $\lim f = +\infty$ và $\lim \inf g > 0$ và $fg$ được xác định, thì $\lim fg = +\infty$.

### Bài tập {#top-iv-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
