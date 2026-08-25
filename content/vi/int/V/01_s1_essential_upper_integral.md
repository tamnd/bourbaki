---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 1
section_title: Essential upper integral
lang: vi
source: int-i-vi
book_pages: INT V.2-INT V.11
pdf_pages: 0257-0266, 0349-0350
extraction: ocr
subsections:
    - "no": 1
      title: Definition of the essential upper integral
      page: 2
      pdf_page: 257
    - "no": 2
      title: Moderated functions and measures
      page: 4
      pdf_page: 259
    - "no": 3
      title: Essentially integrable functions
      page: 7
      pdf_page: 262
    - "no": 4
      title: A property special to the essential upper integral
      page: 10
      pdf_page: 265
statements: 22
exercises: 6
content_sha256: 8fadbee72ac73da411d425d18cf914ac1c96f9d172664d599af61a546e7003d7
translated_from: content/en/int/V/01_s1_essential_upper_integral.md
source_content_sha256: 9adb07a62fadd6e5f8620bda6421cb8411520345e999c2b98de2982037c52e39
translation_model: gpt-5-6-mini
translation_run: translate-vi-ba13410c
glossary_version: 34
glossary_terms_sha256: c3fec433a58fded12a0a71ed749b2e25e56e481e13ccfddc80c76c48de99fb85
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. TÍCH PHÂN TRÊN CỐT YẾU

### 1. Định nghĩa của tích phân trên cốt yếu

#### Định nghĩa 1 {#int-v-s1-def-1 .statement}

Với mọi hàm $f \in \mathcal{F}_+(T)$, ta gọi tích phân trên cốt yếu của $f$ đối với $\mu$, và ký hiệu là $\mu^\bullet(f)$, là supremum, hữu hạn hoặc không, của tập hợp các số $\mu^*(f \varphi_K)$, trong đó $K$ chạy trên tập hợp các tập con compact của $T$. Với mọi tập con $A$ của $T$, ta đặt $\mu^\bullet(A) = \mu^\bullet(\varphi_A)$.

Các ký hiệu $\int^\bullet f d\mu$, $\int^\bullet f(t) d\mu(t)$, $\int^\bullet f \mu$ cũng được sử dụng.
Vì $f \varphi_K \leq f$ với mọi tập con compact $K$ của $T$, ta có

$$
\int^\bullet f d\mu \leq \int^* f d\mu .
$$

Có thể xảy ra $\mu^\bullet(f) \neq \mu^*(f)$; thật vậy, điều kiện $\mu^*(f) = 0$ có nghĩa là $f$ là không đáng kể, trong khi điều kiện $\mu^\bullet(f) = 0$ có nghĩa là $f$ là không đáng kể địa phương (Ch. IV, §5, No. 2, Mệnh đề 5), và có thể tồn tại các tập không đáng kể địa phương nhưng không không đáng kể (Ch. IV, §1, Bài tập 5).

Ánh xạ $\mu^\bullet$ từ $\mathcal{F}_+(T)$ vào $\overline{\mathbf{R}}$ trùng với $\mu$ trên $\mathcal{K}_+(T)$. Suy ra rằng hai độ đo $\mu_1$ và $\mu_2$ sao cho $\mu_1^\bullet = \mu_2^\bullet$ là bằng nhau.

#### Mệnh đề 1 {#int-v-s1-prop-1 .statement}

a) Nếu $f$ và $g$ là hai hàm số $\geq 0$ bằng nhau hầu khắp nơi địa phương, thì $\mu^\bullet(f) = \mu^\bullet(g)$.
b) Nếu $f$ và $g$ là hai hàm số $\geq 0$ sao cho $f \leq g$, thì $\mu^\bullet(f) \leq \mu^\bullet(g)$.
c) Nếu $f$ là một hàm số $\geq 0$, và $\alpha$ là một số $\geq 0$, thì $\mu^\bullet(\alpha f) = \alpha \mu^\bullet(f)$.
d) Nếu $f$ và $g$ là hai hàm số $\geq 0$, thì $\mu^\bullet(f + g) \leq \mu^\bullet(f) + \mu^\bullet(g)$.
e) Nếu $(f_n)_{n \in \mathbf{N}}$ là một dãy tăng các hàm số $\geq 0$, và nếu $f = \lim_{n \to \infty} f_n$, thì $\mu^\bullet(f) = \lim_{n \to \infty} \mu^\bullet(f_n)$.

Các tính chất a), b), c), d) suy ra ngay lập tức từ các tính chất tương ứng của tích phân trên: a) từ Mệnh đề 6 của Ch. IV, §2, No. 3 và Mệnh đề 5 của Ch. IV, §5, No. 2; b), c), d) từ các Mệnh đề 10, 11, 12 của Ch. IV, §1, No. 3. Để thiết lập e), ký hiệu $\mathfrak{K}$ là tập hợp các tập con compact của $T$; theo Định lý 3 của Ch. IV, §1, No. 3, ta có

$$
\lim_{n \to \infty} \mu^\bullet(f_n) = \sup_{n \in \mathbf{N}} \sup_{K \in \mathfrak{K}} \mu^*(f_n \varphi_K) = \sup_{K \in \mathfrak{K}} \sup_{n \in \mathbf{N}} \mu^*(f_n \varphi_K)
= \sup_{K \in \mathfrak{K}} \mu^*(f \varphi_K) = \mu^\bullet(f) .
$$

Đẳng thức xảy ra trong quan hệ d) nếu $f$ và $g$ là đo được, theo Hệ quả 4 của Định lý 5, Ch. IV, §5, No. 6. Nói chung hơn, ta có kết quả sau:

#### Mệnh đề 2 {#int-v-s1-prop-2 .statement}

*Cho $f, g, h$ là ba phần tử của $\mathcal{F}_+$; nếu $g$ và $h$ đo được, thì*

$$
\int^\bullet f(g + h)\, d\mu = \int^\bullet fg\, d\mu + \int^\bullet fh\, d\mu.
$$

Ta ngay lập tức quy về việc chứng minh công thức tương tự đối với tích phân trên. Vì $f(g + h) = fg + fh$ (với quy ước rằng $0 \cdot (+\infty) = 0$), ta có

$$
\int^* f(g + h)\, d\mu \leq \int^* fg\, d\mu + \int^* fh\, d\mu;
$$

còn phải thiết lập bất đẳng thức ngược lại. Cho $u$ là một hàm nửa liên tục dưới sao cho $u \geq f(g + h)$. Đặt $v = \frac{u}{g + h}$ trên tập hợp mà $g + h > 0$, và $v = +\infty$ trên tập hợp mà $g + h = 0$; khi đó $v \geq f$ và $u \geq v(g + h)$, do đó

$$
\int^* v(g + h)\, d\mu \leq \int^* u\, d\mu
$$

và do đó, $v$ đo được (Ch. IV, §5, No. 6, Hệ quả 4 của Định lý 5),

$$
\int^* fg\, d\mu + \int^* fh\, d\mu \leq \int^* vg\, d\mu + \int^* vh\, d\mu \\
= \int^* v(g + h)\, d\mu \leq \int^* u\, d\mu,
$$

điều này suy ra bất đẳng thức cần chứng minh vì $u$ là tùy ý.

#### Hệ quả {#int-v-s1-n1-cor-1 .statement}

*Cho $f$ là một hàm $\geq 0$, $(g_n)$ là một dãy các hàm đo được $\geq 0$; khi đó $\int^\bullet f \left( \sum_n g_n \right) d\mu = \sum_n \left( \int^\bullet f g_n\, d\mu \right)$.

Đối với trường hợp một dãy hữu hạn, đây là một hệ quả ngay lập tức của Mệnh đề 2. Trường hợp một dãy vô hạn có thể được suy ra từ điều này bằng cách dùng Mệnh đề 1, e).

#### Mệnh đề 3 {#int-v-s1-prop-3 .statement}

*Với mọi số hữu hạn $\alpha \geq 0$ và mọi cặp độ đo $\mu, \nu$ trên $\mathbf{T}$,

$$
(\alpha \mu)^\bullet = \alpha \mu^\bullet \\
(\mu + \nu)^\bullet = \mu^\bullet + \nu^\bullet.
$$

Hơn nữa, quan hệ $\mu \leq \nu$ suy ra $\mu^\bullet \leq \nu^\bullet$.*

Chứng minh là ngay lập tức từ mệnh đề tương tự trong Ch. IV (§1, No. 3, Mệnh đề 15).

#### Mệnh đề 4 {#int-v-s1-prop-4 .statement}

— *Với mọi hàm số* $f \geqslant 0$ *nửa liên tục dưới trên* $T$, $\mu^\bullet(f) = \mu^*(f)$.

Vì, cho $g$ là một hàm trong $\mathcal{K}_+(T)$ sao cho $g \leqslant f$. Nếu $K$ là giá (compact) của $g$, thì $\mu(g) \leqslant \mu^*(f \varphi_K) \leqslant \mu^\bullet(f)$. Từ đó, theo định nghĩa của tích phân trên, ta có $\mu^*(f) \leqslant \mu^\bullet(f)$, do đó $\mu^*(f) = \mu^\bullet(f)$ (công thức (1)).

### 2. Các hàm điều hòa và các độ đo

#### Mệnh đề 5 {#int-v-s1-prop-5 .statement}

— *Cho* $A$ *là một tập con của* $T$; *các tính chất sau là tương đương*:
a) *Tập hợp* $A$ *được chứa trong hợp của một dãy các tập mở* $\mu$*-nguyên*.
b) *Tập hợp* $A$ *được chứa trong hợp của một dãy các tập hợp* $\mu$*-nguyên*.
c) *Tập hợp* $A$ *được chứa trong hợp của một dãy các tập compact và một tập* $\mu$*-không đáng kể*.

Hiển nhiên là mỗi tính chất a) và c) suy ra b). Ngược lại, b) suy ra a) vì mọi tập hợp có độ đo ngoài hữu hạn đều được chứa trong một tập mở nguyên (Ch. IV, §1, No. 4, Mệnh đề 19), và b) suy ra c) vì mọi tập hợp nguyên là hợp của một dãy các tập compact và một tập không đáng kể (Ch. IV, §4, No. 6, Hệ quả 2 của Định lý 4).

#### Định nghĩa 2 {#int-v-s1-def-2 .statement}

— *Một tập con của* $T$ *được gọi là* $\mu$*-điều hòa nếu nó thỏa mãn các điều kiện tương đương của Mệnh đề 5*. *Một hàm xác định trên* $T$, *có giá trị trong một không gian vectơ hoặc trong* $\overline{\mathbf{R}}$, *được gọi là* $\mu$*-điều hòa nếu nó bằng không trên phần bù của một tập con* $\mu$*-điều hòa của* $T$. *Độ đo* $\mu$ *được gọi là điều hòa nếu* $T$ *là một tập* $\mu$*-điều hòa*.

Nếu $\mu$ là một độ đo điều hòa, thì mọi hàm trên $T$ đều là $\mu$-điều hòa và mọi tập con của $T$ đều là $\mu$-điều hòa.

#### Nhận xét {#int-v-s1-n2-rem-1 .statement}

— 1) Nếu $\theta$ là một độ đo phức trên $T$, ta nói rằng một hàm $f$ là $\theta$-điều hòa (tương ứng rằng $\theta$ là điều hòa) nếu $f$ là $|\theta|$-điều hòa (tương ứng nếu $|\theta|$ là điều hòa).
2) Mọi độ đo bị chặn đều là điều hòa; nếu $T$ là một hợp đếm được của các tập compact, thì mọi độ đo trên $T$ đều là điều hòa.
3) Cho $(f_n)$ là một dãy các hàm $\mu$-điều hòa với các giá trị trong $\overline{\mathbf{R}}$. Với mỗi $n$, cho $U_n$ là một tập mở là một hợp đếm được của các tập mở có độ đo ngoài hữu hạn, sao cho $f_n$ bằng không bên ngoài $U_n$. Khi đó hàm $s = \sum_{n \in \mathbf{N}} |f_n|$ bằng không bên ngoài $\bigcup_{n \in \mathbf{N}} U_n$; do đó nó là $\mu$-điều hòa, và điều tương tự cũng đúng với mọi hàm $f$ sao cho $|f| \leq s$. Điều này áp dụng đặc biệt cho các hàm $\liminf_{n \to \infty} f_n$, $\limsup_{n \to \infty} f_n$ và $\sum_{n \in \mathbf{N}} f_n$ (nếu tổng được xác định).

4) Một hàm bằng hầu khắp nơi với một hàm điều hòa thì là điều hòa.

#### Mệnh đề 6 {#int-v-s1-prop-6 .statement}

— *Cho $f$ là một hàm số dương xác định trên $T$ là $\mu$-đo được và $\mu$-điều hòa. Khi đó tồn tại một dãy $(h_n)_{n \in \mathbf{N}}$ các phần tử của $\mathcal{F}_+(T)$, có tổng bằng $f$, có các tính chất sau:*

1) *Hàm $h_0$ là $\mu$-không đáng kể.*
2) *Với mọi $n \geq 1$, tồn tại một tập compact $K_n$ sao cho $h_n$ bằng không bên ngoài $K_n$, và sao cho hạn chế của $h_n$ lên $K_n$ là hữu hạn và liên tục.*

Giả sử rằng $f$ là tổng của một dãy $(f_n)$ các hàm đo được dương, mỗi hàm trong đó có tính chất trong mệnh đề; rõ ràng rằng $f$ cũng có tính chất đó. Đặt
$$
f_n = \inf(f, n+1) - \inf(f, n)
$$
với mọi $n \in \mathbf{N}$; vì $f$ bằng tổng của dãy $(f_n)$, nên do đó chỉ cần thiết lập mệnh đề với giả thiết rằng $f$ là điều hòa và *bị chặn*. Khi đó ký hiệu $A$ là tập hợp các $t \in T$ sao cho $f(t) > 0$; $A$ là đo được và điều hòa, do đó tồn tại một dãy $(A_n)$ các tập hợp nguyên rời nhau từng đôi một sao cho $A = \bigcup_n A_n$. Ta được rút gọn về việc chứng minh mệnh đề cho các hàm $f \varphi_{A_n}$; nói cách khác, ta có thể giả sử rằng $f$ bị chặn và bằng không bên ngoài một tập hợp nguyên $I$. Nhưng $I$ là hợp của một tập hợp không đáng kể $N$ và một dãy $(L_n)$ các tập hợp compact rời nhau từng đôi một (Ch. IV, §4, No. 6, Hệ quả 2 của Định lý 4). Do đó ta được rút gọn về việc xét trường hợp $f$ bị chặn và bằng không bên ngoài một tập hợp compact $L$.

Gọi $\mathcal{K}$ là tập hợp các tập con compact $K$ của $T$ sao cho $f|K$ liên tục; vì $\mathcal{K}$ là $\mu$-trù mật (Ch. IV, §5, No. 10, Mệnh đề 15), $L$ là hợp của một tập hợp không đáng kể $N$ và một dãy $(K_n)_{n \geq 1}$ các phần tử rời nhau từng đôi một của $\mathcal{K}$ (Ch. IV, §5, No. 8, Định nghĩa 6). Các hàm $h_0 = f \varphi_N$, $h_n = f \varphi_{K_n}$ với $n \geq 1$ khi đó thỏa mãn các điều kiện của mệnh đề.

Mệnh đề sau đây cho phép rút gọn việc nghiên cứu tích phân trên về việc nghiên cứu tích phân trên cốt yếu.

#### Mệnh đề 7 {#int-v-s1-prop-7 .statement}

— *Cho $f$ là một phần tử của $\mathcal{F}_+(T)$.*
1) *Nếu hàm $f$ không $\mu$-điều hòa, thì $\mu^*(f) = +\infty$.*
2) *Nếu hàm $f$ là $\mu$-điều hòa, thì $\mu^*(f) = \mu^*(f)$.*
3) *Nếu $\mu^*(f) < +\infty$ thì tồn tại một tập con $\mu$-điều hòa $A$, là hợp của một dãy các tập con compact của $T$, sao cho $f = f \varphi_A$ hầu khắp nơi địa phương.*

Mệnh đề thứ nhất suy ra ngay lập tức từ Bổ đề 1 của Ch. IV, §5, No. 6. Để thiết lập mệnh đề thứ hai, ký hiệu $A$ là một tập con điều hòa sao cho f bằng không bên ngoài A; A là hợp của một tập hợp không đáng kể $A_0$ và một dãy $(A_n)_{n \geq 1}$ các tập hợp compact, mà ta có thể giả sử là tăng. Khi đó hàm $f$ hầu khắp nơi bằng bao trên của các hàm $f \varphi_{A_n}$ ($n \geq 1$), do đó (Ch. IV, §1, No. 3, Định lý 3 và §2, No. 3, Mệnh đề 6)

$$
\mu^*(f) = \lim_{n \to \infty} \mu^*(f \varphi_{A_n}) \leq \mu^\bullet(f),
$$

do đó có đẳng thức $\mu^*(f) = \mu^\bullet(f)$ theo công thức (1). Cuối cùng, giả sử rằng $\mu^\bullet(f) < +\infty$; tồn tại một dãy tăng $(A_n)$ các tập hợp compact sao cho

$$
\mu^\bullet(f) = \sup_n \mu^*(f \varphi_{A_n}).
$$

Đặt $A = \bigcup_n A_n$; thành phần thứ hai bằng $\mu^*(f \varphi_A)$ (Ch. IV, §1, No. 3, Th. 3), nghĩa là bằng $\mu^\bullet(f \varphi_A)$ (theo Mệnh đề 1, hoặc theo 2) ở trên). Vì $\mu^\bullet(f) = \mu^\bullet(f \varphi_A) + \mu^\bullet(f \varphi_{\mathbf{C}_A})$ (Mệnh đề 2), ta có $\mu^\bullet(f \varphi_{\mathbf{C}_A}) = 0$, từ đó suy ra 3).

#### Hệ quả 1 {#int-v-s1-prop-7-cor-1 .statement}

*Để f là không đáng kể, điều kiện cần và đủ là nó không đáng kể địa phương và bị điều hòa.*

#### Hệ quả 2 {#int-v-s1-prop-7-cor-2 .statement}

*Nếu $\mu$ là một độ đo bị điều hòa (đặc biệt nếu $\mu$ bị chặn, hoặc nếu T là đếm được tại vô hạn), thì $\mu^* = \mu^\bullet$.*

#### Mệnh đề 8 {#int-v-s1-prop-8 .statement}

a) *Cho H là một tập hợp các hàm $\geq 0$, nửa liên tục dưới, có hướng đối với quan hệ $\leq$; khi đó*

$$
\mu^\bullet \left( \sup_{h \in H} h \right) = \sup_{h \in H} \mu^\bullet(h).
$$

b) *Cho H là một tập hợp các hàm $\geq 0$, nửa liên tục trên, có hướng đối với quan hệ $\geq$; nếu tồn tại trong H một hàm $h_0$ sao cho $\mu^\bullet(h_0) < +\infty$, thì*

$$
\mu^\bullet \left( \inf_{h \in H} h \right) = \inf_{h \in H} \mu^\bullet(h).
$$

Mệnh đề a) là, theo Mệnh đề 4, sự lặp lại của Định lý 1 của Ch. IV, §1, No. 1. Để thiết lập b), đặt $\eta = \inf_{h \in H} h$, và cho $a$ là một số $> 0$. Tồn tại một tập compact K sao cho (Ch. IV, §4, No. 4, Hệ quả 1 của Mệnh đề 5):

$$
\mu^\bullet(h_0) - a \leq \mu^*(h_0 \varphi_K) = \mu(h_0 \varphi_K) \leq \mu^\bullet(h_0).
$$

Các hàm $h\varphi_K$, trong đó h chạy trên H, tạo thành một tập hợp các hàm nửa liên tục trên, có hướng đối với quan hệ $\geqslant$, chứa một hàm khả tích. Do đó (Ch. IV, §4, No. 4, Hệ quả 2 của Mệnh đề 5):

$$
\mu^*(\eta\varphi_K) = \inf_{h \in H} \mu^*(h\varphi_K).
$$

Nhưng (Ch. IV, §4, No. 4, Hệ quả 1 của Mệnh đề 5) $\mu^\bullet(h_0\varphi_{C_K}) \leqslant a$, do đó $\mu^\bullet(h\varphi_{C_K}) \leqslant a$ đối với mọi hàm $h \in H$ sao cho $h \leqslant h_0$. Vì vậy, cuối cùng:

$$
\mu^\bullet(\eta) \geqslant \mu^*(\eta\varphi_K) = \inf_{h \in H} \mu^*(h\varphi_K) \geqslant \inf_{h \in H} \mu^\bullet(h) - a.
$$

Bất đẳng thức $\mu^\bullet(\eta) \leqslant \inf_{h \in H} \mu^\bullet(h)$ là hiển nhiên, và $a$ là tùy ý, nên mệnh đề được chứng minh.

### 3. Các hàm khả tích thiết yếu

Cho $F$ là một không gian Banach thực; nhắc lại rằng các phần tử của các không gian $\mathcal{F}_F^p$ (Ch. IV, §3, No. 3) và $\mathcal{L}_F^p$ (Ch. IV, §3, No. 4, Định nghĩa 2) là các hàm $\mu$-bị điều hòa (Ch. IV, §5, No. 6, Bổ đề 1); với $\mathcal{N}_F$ vẫn ký hiệu không gian các ánh xạ không đáng kể của $T$ vào $F$, ta sẽ đưa vào không gian $\mathcal{N}_F^\infty$ các ánh xạ không đáng kể địa phương của $T$ vào $F$.

#### Bổ đề {#int-v-s1-n3-lem-1 .statement}

*Cho $g$ và $g'$ là hai ánh xạ $\mu$-bị điều hòa với các giá trị trong $F$; nếu $g$ và $g'$ bằng địa phương hầu khắp nơi với cùng một hàm $f$, thì $g = g'$ hầu khắp nơi.*

Thật vậy, cho $D$ là tập hợp các $t \in T$ sao cho $g(t) \neq g'(t)$; $D$ là không đáng kể địa phương và bị điều hòa, do đó không đáng kể (Hệ quả 1 của Mệnh đề 7).

Ta sẽ ký hiệu bởi $\overline{\mathcal{F}}_F^p(T, \mu)$ (hoặc đơn giản là $\overline{\mathcal{F}}_F^p(\mu)$, $\overline{\mathcal{F}}_F^p$, nếu không thể có sự nhầm lẫn) tập hợp các ánh xạ $f$ của $T$ vào $F$, sao cho tồn tại một hàm $g \in \mathcal{F}_F^p$ bằng $f$ hầu khắp nơi một cách địa phương. Vì số $N_p(g)$ chỉ phụ thuộc vào $f$ theo Bổ đề, ta sẽ viết $\overline{N}_p(f) = N_p(g)$. Hàm $\overline{N}_p$ hiển nhiên là một nửa chuẩn trên $\overline{\mathcal{F}}_F^p$, và ta sẽ luôn giả sử rằng $\overline{\mathcal{F}}_F^p$ được trang bị tôpô xác định bởi $\overline{N}_p$. Bao đóng của 0 đối với tôpô này là không gian $\mathcal{N}_F^\infty$; các hệ thức $\overline{\mathcal{F}}_F^p = \mathcal{F}_F^p + \mathcal{N}_F^\infty$, $\mathcal{N}_F^\infty \cap \mathcal{F}_F^p = \mathcal{N}_F$ (Bổ đề) chỉ ra rằng không gian chuẩn hóa $\overline{\mathcal{F}}_F^p / \mathcal{N}_F^\infty$ có thể được đồng nhất một cách chính tắc với $\mathcal{F}_F^p / \mathcal{N}_F$, là đầy đủ (Ch. IV, §3, No. 3, Mệnh đề 5); do đó $\overline{\mathcal{F}}_F^p$ tự nó là đầy đủ.

Tương tự, ta sẽ ký hiệu bởi $\overline{\mathcal{L}}_F^p(T, \mu)$ (hoặc $\overline{\mathcal{L}}_F^p(\mu)$, hoặc $\overline{\mathcal{L}}_F^p$) không gian con $\mathcal{L}_F^p + \mathcal{N}_F^\infty$ của $\overline{\mathcal{F}}_F^p$; ta cũng có thể đặc trưng $\overline{\mathcal{L}}_F^p$ như là không gian con của $\overline{\mathcal{F}}_F^p$ được cấu thành bởi các ánh xạ *đo được* (Ch. IV, §5, No. 6, Định lý 5).

Không gian chuẩn hóa $\overline{\mathcal{L}}_F^p / \mathcal{N}_F^\infty$ có thể được đồng nhất một cách chính tắc với $L_F^p$; do đó $\overline{\mathcal{L}}_F^p$ là đầy đủ. Các phần tử của nó được gọi là *các hàm khả tích thiết yếu lũy thừa p*, thuật ngữ này được biện minh bởi mệnh đề sau:

#### Mệnh đề 9 {#int-v-s1-prop-9 .statement}

*Đối với một ánh xạ f của T vào F thuộc $\overline{\mathcal{F}}_F^p$ (tương ứng thuộc $\overline{\mathcal{L}}_F^p$), điều kiện cần và đủ là* (tương ứng *rằng f đo được và rằng*)

$$
\mu^\bullet(|f|^p) < +\infty .
$$

*Khi đó ta có* $\overline{N}_p(f) = (\mu^\bullet(|f|^p))^{1/p}$.

Ta rõ ràng có thể giới hạn vào mệnh đề liên quan đến $\overline{\mathcal{F}}_F^p$. Nếu f thuộc $\overline{\mathcal{F}}_F^p$, gọi g là một hàm thuộc $\mathcal{F}_F^p$ bằng f hầu khắp nơi một cách địa phương; khi đó $|f|^p = |g|^p$ hầu khắp nơi một cách địa phương, do đó

$$
\mu^\bullet(|f|^p) = \mu^\bullet(|g|^p) = \mu^*(|g|^p) < +\infty
$$

(Mệnh đề 1, a) và Mệnh đề 7), và mặt khác, theo định nghĩa của $\overline{N}_p$,

$$
\overline{N}_p(f) = N_p(g) = (\mu^*(|g|^p))^{1/p} .
$$

Ngược lại, giả sử rằng $\mu^\bullet(|f|^p) < +\infty$; khi đó tồn tại một tập hợp điều hòa A sao cho f bằng không hầu khắp nơi một cách địa phương trong T − A (Mệnh đề 7). Hàm $f \varphi_A$, bằng f hầu khắp nơi một cách địa phương, thỏa mãn $N_p(f \varphi_A) = \overline{N}_p(f) < +\infty$, do đó nó thuộc về $\mathcal{F}_F^p$, và $f \in \overline{\mathcal{F}}_F^p$.

#### Hệ quả {#int-v-s1-n3-cor-1 .statement}

*Để f thuộc $\mathcal{L}_F^p$, điều kiện cần và đủ là f thuộc $\overline{\mathcal{L}}_F^p$ và là điều hòa.*

#### Định nghĩa 3 {#int-v-s1-def-3 .statement}

*Các phần tử của $\overline{\mathcal{L}}_F^1$ được gọi là các hàm khả tích thiết yếu với giá trị trong F. Khi hợp thành ánh xạ $\tilde{f} \mapsto \mu(f)$ của $L_F^1$ vào F với ánh xạ chính tắc của $\overline{\mathcal{L}}_F^1$ lên $L_F^1$, ta thu được một ánh xạ tuyến tính liên tục của $\overline{\mathcal{L}}_F^1$ vào F mở rộng ánh xạ $f \mapsto \int f d\mu$ của $\mathcal{L}_F^1$ vào F. Một lần nữa ký hiệu $\int f d\mu$ hoặc $\mu(f)$ là giá trị của ánh xạ này đối với $f \in \overline{\mathcal{L}}_F^1$, và phần tử này được gọi là nguyên của f đối với $\mu$.*

Hai hàm khả tích thiết yếu bằng nhau địa phương hầu khắp có cùng nguyên. Đối với mọi hàm $f \geq 0$ hữu hạn và khả tích thiết yếu, $\int^\bullet f d\mu = \int f d\mu$. Nếu A là một tập hợp mà hàm đặc số của nó là khả tích thiết yếu, thì A được gọi là một *tập hợp $\mu$-khả tích thiết yếu*; $\int \varphi_A d\mu$ cũng được ký hiệu là $\mu(A)$ và lại được gọi là *độ đo* của A.

Nếu một hàm $f$, với các giá trị trong $F$, được xác định địa phương hầu khắp trong $T$, ta lại nói rằng $f$ là *khả tích thiết yếu* nếu nó bằng, địa phương hầu khắp, một hàm $f_1$ được xác định khắp nơi và khả tích; khi đó ta đặt
$$
\int f\, d\mu = \int f_1\, d\mu,
$$
và định nghĩa này độc lập với hàm khả tích $f_1$ được xác định khắp nơi và bằng địa phương hầu khắp với $f$ (Bổ đề). Ta định nghĩa tương tự khái niệm hàm khả tích thiết yếu đối với các hàm có giá trị trong $\overline{\mathbf{R}}$ được xác định và hữu hạn địa phương hầu khắp.

Người đọc sẽ không gặp khó khăn nào trong việc mở rộng, cho các hàm khả tích thiết yếu, các kết quả của Ch. IV, §4 đối với các hàm khả tích, bằng cách thay thế 'hầu khắp' trong các mệnh đề bằng 'địa phương hầu khắp'. Ta chú ý chẳng hạn đến bất đẳng thức
$$
\left| \int f\, d\mu \right| \leq \int |f|\, d\mu,
$$
đúng đối với mọi hàm khả tích thiết yếu có giá trị trong một không gian Banach.

#### Mệnh đề 10 {#int-v-s1-prop-10 .statement}

*Cho $\mathfrak{K}$ là một tập hợp trù mật theo $\mu$ của các tập con compact của $T$.*

a) *Nếu $f$ là một hàm số $\geq 0$, thì*
$$
\mu^\bullet(f) = \sup_{K \in \mathfrak{K}} \mu^*(f \varphi_K).
$$
b) *Nếu $f$ là một hàm khả tích thiết yếu với các giá trị trong một không gian Banach $F$, thì*
$$
\int f\, d\mu = \lim_{\mathfrak{K}} \int f \varphi_K\, d\mu,
$$
*giới hạn được lấy đối với tập hợp có hướng (đối với $\subset$) $\mathfrak{K}$.*

Để thiết lập a), chỉ cần chỉ ra rằng đối với mọi tập con compact $L$ của $T$,
$$
\int^* f \varphi_L\, d\mu = \sup_K \int^* f \varphi_K\, d\mu,
$$
trong đó $K$ chạy trên tập hợp các tập con của $L$ thuộc về $\mathfrak{K}$. Vì $L$ là hợp của một tập không đáng kể và một dãy tăng $(K_n)$ các phần tử của $\mathfrak{K}$ (Ch. IV, §5, No. 8, Prop. 12), điều này suy ra từ định lý về phép chuyển qua giới hạn trong các nguyên trên (Ch. IV, §1, No. 3, Th. 3).

Giả sử bây giờ rằng $f$ thuộc về $\mathcal{L}_F^1$; cho $\varepsilon$ là một số $> 0$, và cho $K$ là một phần tử của $\mathfrak{K}$ sao cho
$$
\int |f| \varphi_K\, d\mu \geq \int |f|\, d\mu - \varepsilon
$$

(một K như vậy tồn tại theo a)). Khi đó, đối với mọi tập compact H chứa K,

$$
\left| \int f \, d\mu - \int f \varphi_H \, d\mu \right| \leq \int |f| \varphi_{\mathbf{C}_H} \, d\mu \leq \int |f| \varphi_{\mathbf{C}_K} \, d\mu \leq \varepsilon .
$$

Mở rộng đến các không gian Banach phức và các độ đo. Cho F là một không gian Banach phức; do một sự lạm dụng ký hiệu, không gian Banach thực nằm dưới F cũng được ký hiệu là F. Khi đó không gian Banach $\overline{\mathcal{L}}_F^p(T, \mu)$ có thể được trang bị một cấu trúc không gian Banach phức tự nhiên, và cần phải nói rõ liệu người ta đang sử dụng cấu trúc thực hay cấu trúc phức của không gian này. Trong chương này, và khi không có sự nói rõ ngược lại, ta luôn hiểu đó là cấu trúc thực.

Cho $\theta$ là một độ đo phức; ta đặt $\overline{\mathcal{L}}_F^p(T, \theta) = \overline{\mathcal{L}}_F^p(T, |\theta|)$; nếu F là một không gian Banach phức, ta có thể đưa ra những nhận xét tương tự như trên. Đặc biệt, một hàm f nhận giá trị trong F sẽ được gọi là khả tích cốt yếu đối với $\theta$ nếu nó khả tích cốt yếu đối với $|\theta|$. Mệnh đề b) của Mệnh đề 10 khi đó mở rộng ngay cho các độ đo phức.

### 4. Một tính chất đặc biệt của tích phân trên cốt yếu

Kết quả sau đây sẽ được sử dụng thường xuyên trong phần tiếp theo. Trong mệnh đề này, không thể thay thế các tích phân trên cốt yếu bằng các tích phân trên thông thường (xem Bài tập 4).

#### Mệnh đề 11 {#int-v-s1-prop-11 .statement}

— Cho $(\lambda_\alpha)_{\alpha \in A}$ là một họ các độ đo dương trên T, có hướng theo quan hệ $\leq$ và có supremum $\lambda$ trong $\mathcal{M}(T)$. Khi đó, với mọi hàm số $f \geq 0$,

$$
\lambda^\bullet(f) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

Khi $f$ thuộc $\mathcal{K}(T)$, quan hệ này trở thành định nghĩa của supremum của một tập có hướng trong $\mathcal{M}(T)$ (Ch. II, §2, No. 2, Bổ đề). Tiếp theo, giả sử rằng $f \leq g$ với một hàm $g \in \mathcal{K}_+$ nào đó (nói cách khác, f bị chặn và bằng không ngoài một tập compact K); lấy $\alpha$ là một chỉ số sao cho $\lambda_\alpha(g) \geq \lambda(g) - \varepsilon$, trong đó $\varepsilon$ là một số $> 0$; vì độ đo $\nu = \lambda - \lambda_\alpha$ là dương, ta có $\nu^*(f) \leq \nu(g) \leq \varepsilon$, hay $\lambda_\alpha^*(f) \geq \lambda^*(f) - \varepsilon$ (Ch. IV, §1, No. 3, Mệnh đề 15). Suy ra (vì $\varepsilon$ là tùy ý) rằng vế thứ hai của (5) là $\geq$ vế thứ nhất; bất đẳng thức ngược lại là hiển nhiên, nên (5) được thiết lập trong trường hợp đặc biệt đang xét. Tiếp theo, giả sử rằng f bằng không ngoài K nhưng không nhất thiết bị chặn, và đặt $f_n = \inf(f, n)$ với mọi số nguyên $n$. Khi đó

$$
\lambda^\bullet(f) = \sup_{n \in \mathbf{N}} \lambda^\bullet(f_n) = \sup_{n \in \mathbf{N}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \sup_{n \in \mathbf{N}} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

Cuối cùng, không đặt hạn chế nào lên f, ký hiệu $\mathcal{K}$ là tập hợp các tập con compact của T, ta có
$$
\lambda^\bullet(f) = \sup_{K \in \mathcal{K}} \lambda^\bullet(f \varphi_K) = \sup_{K \in \mathcal{K}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f \varphi_K)
$$
$$
= \sup_{\alpha \in A} \sup_{K \in \mathcal{K}} \lambda_\alpha^\bullet(f \varphi_K) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

#### Hệ quả 1 {#int-v-s1-prop-11-cor-1 .statement}

*Để một tập con N của T là địa phương $\lambda$-không đáng kể, điều kiện cần và đủ là N địa phương $\lambda_\alpha$-không đáng kể với mọi $\alpha \in A$.*

#### Hệ quả 2 {#int-v-s1-prop-11-cor-2 .statement}

*Để một ánh xạ g từ T vào một không gian tôpô G là $\lambda$-đo được, điều kiện cần và đủ là nó $\lambda_\alpha$-đo được với mọi $\alpha \in A$.*

Điều kiện này hiển nhiên là cần, vì $\lambda_\alpha \leq \lambda$ với mọi $\alpha$ (Ch. IV, §1, No. 3, Mệnh đề 15). Ngược lại, giả sử rằng g là $\lambda_\alpha$-đo được với mọi $\alpha$, ký hiệu $\mathcal{K}$ là tập hợp các tập con compact K của T sao cho $g|K$ liên tục, và lấy L là một tập compact sao cho $L \cap K$ là $\lambda$-không đáng kể với mọi $K \in \mathcal{K}$. Vì tập hợp $\mathcal{K}$ là $\lambda_\alpha$-trù mật, L là $\lambda_\alpha$-không đáng kể với mọi $\alpha$ (Ch. IV, §5, No. 8, Mệnh đề 12), do đó là $\lambda$-không đáng kể (Hệ quả 1). Suy ra $\mathcal{K}$ là $\lambda$-trù mật và g là $\lambda$-đo được (Ch. IV, §5, No. 10, Mệnh đề 15).

### Bài tập {#int-v-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
