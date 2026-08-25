---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 1
section_title: COMPARISON OF FUNCTIONS ON A FILTERED SET
lang: vi
source: fvr-i-vii
pdf_pages: 0226-0235, 0274-0274
extraction: ocr
subsections:
    - "no": 1
      title: 'COMPARISON RELATIONS: I. WEAK RELATIONS'
      page: 0
      pdf_page: 226
    - "no": 2
      title: 'COMPARISON RELATIONS: II. STRONG RELATIONS'
      page: 0
      pdf_page: 229
    - "no": 3
      title: CHANGE OF VARIABLE
      page: 0
      pdf_page: 232
    - "no": 4
      title: COMPARISON RELATIONS BETWEEN STRICTLY POSITIVE FUNCTIONS
      page: 0
      pdf_page: 232
    - "no": 5
      title: NOTATION
      page: 0
      pdf_page: 234
statements: 38
exercises: 3
content_sha256: 6e0979e46483b296b2ed97466cb240d9b675187146d09a24612bf7eeab71d549
translated_from: content/en/fvr/V/01_s1_comparison_of_functions_on_a_filtered.md
source_content_sha256: f90de3067099cf19260303b9de7511a8e7908cc1fc7dbeb7ba244aa4277da258
translation_model: gpt-5.4-mini
translation_run: translate-vi-52b281be
glossary_version: 34
glossary_terms_sha256: e2166aa281835d373989defad866b9926986958ccb1b53f54f1b032fed6a74bd
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. SO SÁNH CÁC HÀM TRÊN MỘT TẬP HỢP ĐƯỢC LỌC

Cho E là một tập hợp được lọc bởi một bộ lọc có cơ sở $\mathfrak{F}$ (*Gen. Top.*, I, p. 58); trong chương này ta sẽ xét các hàm có miền xác định là một tập con của E thuộc cơ sở của bộ lọc $\mathfrak{F}$ (tập con tùy thuộc vào hàm) và nhận giá trị либо trong trường số thực $\mathbf{R}$, hoặc, nói chung hơn, trong một không gian vectơ định chuẩn trên một trường có giá trị (*Gen. Top.*, IX, p. 170).

Trong các ứng dụng, E thường sẽ là một không gian con của không gian thực $\mathbf{R}^n$, hoặc đường thẳng mở rộng $\overline{\mathbf{R}}$, và $\mathfrak{F}$ sẽ là vết trên E của bộ lọc các lân cận của một điểm đóng của E, hoặc là bộ lọc các phần bù của các tập hợp tương đối compact của E ("các lân cận của điểm ở vô cực").

Nói chung, sẽ không đủ chỉ biết rằng một hàm như vậy tiến tới một giới hạn đã cho theo $\mathfrak{F}$ để có thể xử lý mọi bài toán về "chuyển qua giới hạn theo $\mathfrak{F}$" đối với các biểu thức được tạo từ hàm này.

Chẳng hạn, khi biến thực x tiến tới $+\infty$ thì ba hàm $x$, $x^2$ và $\sqrt{x}$ đều tiến tới $+\infty$, nhưng, trong các biểu thức

$$
(x+1)^2 - x^2, \quad (x+1) - x, \quad \sqrt{x+1} - \sqrt{x},
$$

biểu thức thứ nhất tiến tới $+\infty$, biểu thức thứ hai tiến tới 1, biểu thức thứ ba tiến tới 0.

Vì thế, điều quan trọng không chỉ là biết giá trị giới hạn của một hàm theo $\mathfrak{F}$ (khi giới hạn này tồn tại) mà còn là "cách thức" hàm tiến tới giới hạn của nó; nói cách khác, ta đi đến việc phân loại tập hợp các hàm cùng tiến tới một giới hạn.

### 1. CÁC QUAN HỆ SO SÁNH: I. CÁC QUAN HỆ YẾU

Trong phần sau ta ký hiệu V là một không gian vectơ định chuẩn trên một trường có giá trị K, và $\mathcal{H}(\mathfrak{F}, V)$ là tập hợp các hàm nhận giá trị trong V, mỗi hàm đều được xác định trên một tập con của E thuộc cơ sở của bộ lọc $\mathfrak{F}$. Những quan hệ mà ta sẽ định nghĩa giữa các hàm như vậy có một tính chất *địa phương* tương đối với bộ lọc có cơ sở $\mathfrak{F}$: hãy làm rõ ý ta muốn nói là gì. Nếu f và g là hai hàm trong $\mathcal{H}(\mathfrak{F}, V)$, hãy nhớ rằng quan hệ "có một tập $Z \in \mathfrak{F}$ sao cho f và g được xác định và bằng nhau trên Z" là một *quan hệ tương đương $R_\infty$ trên $\mathcal{H}(\mathfrak{F}, V)$ (*Gen. Top.*, I, p. 66). Vì thế, ta sẽ nói rằng một quan hệ S liên quan đến một hàm $f$ của $\mathcal{H}(\mathfrak{F}, V)$ là có tính chất *địa phương* (theo $\mathfrak{F}$) đối với f, nếu nó *tương thích* (với f) với quan hệ tương đương $R_\infty$ (*Set Theory*, II, p. 117); ta biết rằng nếu $\tilde{f}$ là *mầm* của f theo $\mathfrak{F}$, tức là lớp tương đương của f modulo $R_\infty$ (một phần tử của tập thương $\mathcal{H}_\infty(\mathfrak{F}, V) = \mathcal{H}(\mathfrak{F}, V)/R_\infty$), thì từ S, bằng cách chuyển qua tập thương, ta có thể suy ra một quan hệ giữa $\tilde{f}$ và các đối số khác của S, và ngược lại, mọi quan hệ như vậy đều xác định một quan hệ có tính chất địa phương đối với f.

#### Ví dụ {#fvr-v-s1-n1-exa-5 .statement}

Nếu $f$ và $g$ là hai hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, quan hệ "có một $X \in \mathfrak{F}$ sao cho $f$ và $g$ được xác định trên $X$ và $f(t) \leq g(t)$ với mọi $t \in X$" là có tính chất địa phương đối với $f$ và $g$. Ta ký hiệu $\tilde{f} \leq \tilde{g}$ quan hệ thu được bằng cách chuyển qua tập thương (đối với $f$ và $g$); ta nhận xét rằng nếu $\tilde{f} \leq \tilde{g}$ thì tồn tại một hàm $f_1 \in \tilde{f}$ và một hàm $g_1 \in \tilde{g}$, được xác định trên *toàn bộ* E, sao cho $f_1(t) \leq g_1(t)$ với mọi $t \in E$.

*Nhận xét.* 1) Cho $V_i$ ($1 \leq i \leq n$) là $n$ không gian vectơ định chuẩn trên K, và $\varphi$ là một hàm được xác định trên $V_1 \times V_2 \times \cdots \times V_n$, nhận giá trị trong V; khi chuyển qua thương theo $R_\infty$ thì hàm $\varphi$ xác định một ánh xạ từ
$$
\mathcal{H}_\infty(\mathfrak{F}, V_1) \times \cdots \times \mathcal{H}_\infty(\mathfrak{F}, V_n)
$$
vào $\mathcal{H}_\infty(\mathfrak{F}, V)$, mà người ta thường ký hiệu là $\varphi(\tilde{f}_1, \ldots, \tilde{f}_n)$ (*Gen. Top.*, I, p. 67). Chẳng hạn, lấy $\varphi$ là các ánh xạ $(x, y) \mapsto x + y$ và $x \mapsto x\lambda$ ($\lambda \in K$), do đó, với bất kỳ hai mầm $\tilde{f}, \tilde{g}$ trong $\mathcal{H}_\infty(\mathfrak{F}, V)$, ta định nghĩa các phần tử $\tilde{f} + \tilde{g}$ và $\tilde{f}\lambda$, và người ta kiểm tra ngay rằng các luật hợp thành $(\tilde{f}, \tilde{g}) \mapsto \tilde{f} + \tilde{g}$ và $(\lambda, \tilde{f}) \mapsto \tilde{f}\lambda$ xác định trên $\mathcal{H}_\infty(\mathfrak{F}, V)$ một cấu trúc *không gian vectơ* trên trường K; trong không gian này $\tilde{O}$ là lớp gồm các hàm bằng 0 trên một tập trong $\mathfrak{F}$, và $-\tilde{f}$ là lớp gồm các hàm bằng $-f$ trên một tập trong $\mathfrak{F}$. Cũng theo cách ấy, nếu V là một *đại số* trên K, người ta xác định trên $\mathcal{H}_\infty(\mathfrak{F}, V)$ một luật hợp thành nội bộ thứ hai $(\tilde{f}, \tilde{g}) \mapsto \tilde{f}\tilde{g}$ bằng cách lấy $\varphi(x, y) = xy$; cùng với hai luật trước, điều này xác định trên $\mathcal{H}_\infty(\mathfrak{F}, V)$ một cấu trúc *đại số* trên K; nếu V có một phần tử đơn vị e thì $\mathcal{H}_\infty(\mathfrak{F}, V)$ có phần tử đơn vị là lớp $\tilde{e}$ gồm các hàm bằng e trên một tập nào đó trong $\mathfrak{F}$; để $\tilde{f}$ *khả nghịch* trong $\mathcal{H}_\infty(\mathfrak{F}, V)$ thì cần và đủ rằng với một $f \in \tilde{f}$ nào đó, tồn tại một $Z \in \mathfrak{F}$ sao cho $f(t)$ khả nghịch trong V với mọi $t \in Z$ (trong trường hợp ấy điều kiện này được mọi hàm trong lớp $\tilde{f}$ thỏa mãn).

2) Với cùng ký hiệu, cho $\psi$ là một ánh xạ của một tập con của $\prod_{i=1}^n V_i$ vào V; ta ký hiệu bởi $\psi(f_1, f_2, \ldots, f_n)$ hàm bằng $\psi(f_1(t), f_2(t), \ldots, f_n(t))$ tại mọi điểm $t \in E$ nơi các $f_i(t)$ được xác định và nơi điểm $(f_i(t))$ thuộc tập mà trên đó $\psi$ được xác định $^1$. Chẳng hạn, $f + g$ là hàm bằng $f(t) + g(t)$ tại mọi điểm $t \in E$ nơi cả $f$ lẫn $g$ đều được xác định. Hãy chú ý rằng ánh xạ $(f, g) \mapsto f + g$ *không phải là một luật nhóm* trên $\mathcal{H}(\mathfrak{F}, V)$, vì nếu $f$ không được xác định trên toàn bộ E thì không có hàm $g \in \mathcal{H}(\mathfrak{F}, V)$ sao cho $f + g = 0$.

#### Định nghĩa 1 {#fvr-v-s1-def-1 .statement}

*Cho hai hàm thực* $f, g$ *thuộc* $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, *đều* $\geq 0$ *trên một tập hợp trong* $\mathfrak{F}$, *ta nói rằng* $f$ *bị trội bởi* $g$, *hoặc rằng* $g$ *trội* $f$ *(theo* $\mathfrak{F}$*), và viết* $f \preceq g$ *hoặc* $g \succeq f$, *nếu có một tập hợp* $X \in \mathfrak{F}$ *và một số* $k > 0$ *sao cho* $f(t) \leq k\ g(t)$ *với mọi* $t \in X$ *(nói cách khác, nếu tồn tại một* $k > 0$ *sao cho* $\tilde{f} \leq k\ \tilde{g}$)

$^1$ *Đặc biệt, trong toàn bộ phần sau, với một hàm* $f$ *trong* $\mathcal{H}(\mathfrak{F}, V)$ *ta sẽ ký hiệu bởi* $\|f\|$ *hàm* $t \mapsto \|f(t)\|$ *thuộc* $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ *và được xác định trên cùng tập hợp như* $f$: *chúng tôi đặc biệt lưu ý rằng trong chương này* $\|f\|$ *là một* *hàm* *chứ không phải một* *số*.

Cho hai không gian vectơ chuẩn hoá $V_1, V_2$, và hai hàm $f_1, f_2$ thuộc $\mathcal{H}(\mathfrak{F}, V_1)$ và $\mathcal{H}(\mathfrak{F}, V_2)$ tương ứng, người ta nói rằng $f_1$ bị trội bởi $f_2$ (theo $\mathfrak{F}$), và viết $f_1 \preccurlyeq f_2$ hoặc $f_2 \succeq f_1$, nếu $\|f_1\| \preccurlyeq \|f_2\|$.

Quan hệ $f_1 \preccurlyeq f_2$ rõ ràng có đặc trưng địa phương theo $f_1$ và $f_2$; do đó nó tương đương với quan hệ $\tilde{f}_1 \preccurlyeq \tilde{f}_2$ thu được khi chuyển qua thương. Khi $f$ và $g$ là các hàm thực, cần cẩn thận để không nhầm lẫn các quan hệ $\tilde{f} \preccurlyeq \tilde{g}$ và $\tilde{f} \leq \tilde{g}$.

Chú ý rằng với mọi vô hướng $\lambda \neq 0$ quan hệ $f_1 \preccurlyeq f_2 \lambda$ *tương đương với* $f_1 \preccurlyeq f_2$. Nếu $f_1 \preccurlyeq f_2$ thì tồn tại một tập hợp $X \in \mathfrak{F}$ sao cho $f_1(x) = 0$ với mọi điểm $x \in X$ mà ở đó $f_2(x) = 0$.

*Ví dụ.* 1) Quan hệ $f \preccurlyeq 1$ có nghĩa là $f$ *bị chặn* trên một tập hợp của $\mathfrak{F}$.

2) Với mọi hàm $f$ của $\mathcal{H}(\mathfrak{F}, V)$, và với mọi vô hướng $\lambda \neq 0$, ta có $f \preccurlyeq f \lambda$.
3) Khi $x$ tiến tới $+\infty$ thì $\sin^2 x \preccurlyeq \sin x$.
4) Khi $(x, y)$ tiến tới $(0, 0)$ trong $\mathbf{R}^2$ thì có
$$
xy \preccurlyeq x^2 + y^2.
$$

Các mệnh đề sau là những hệ quả ngay lập tức của đn. 1:

#### Mệnh đề 1 {#fvr-v-s1-prop-1 .statement}

*Nếu* $f, g, h$ *là ba hàm trong* $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ *thì các quan hệ* $f \preccurlyeq g$ *và* $g \preccurlyeq h$ *suy ra* $f \preccurlyeq h$.

#### Mệnh đề 2 {#fvr-v-s1-prop-2 .statement}

*Cho* $f_1, f_2$ *là hai hàm trong* $\mathcal{H}(\mathfrak{F}, V)$ *và* $g$ *là một hàm trong* $\mathcal{H}(\mathfrak{F}, \mathbf{R})$. *Các quan hệ* $f_1 \preccurlyeq g$ *và* $f_2 \preccurlyeq g$ *suy ra* $f_1 + f_2 \preccurlyeq g$.

Tiếp theo:

#### Mệnh đề 3 {#fvr-v-s1-prop-3 .statement}

*Cho* $V_1, V_2, V$ *là ba không gian chuẩn trên cùng một trường có định giá, và* $(x, y) \mapsto [x.y]$ *là một ánh xạ song tuyến tính từ* $V_1 \times V_2$ *vào* $V$. *Nếu* $f_1$ *và* $f_2$ *là các hàm trong* $\mathcal{H}(\mathfrak{F}, V_1)$ *và* $\mathcal{H}(\mathfrak{F}, V_2)$ *tương ứng, và* $g_1, g_2$ *là hai hàm trong* $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ *sao cho* $f_1 \preccurlyeq g_1$ *và* $f_2 \preccurlyeq g_2$ *thì* $[f_1.f_2] \preccurlyeq g_1 g_2$.

Thật vậy (*Gen. Top.*, IX, p. 173, đl. 1) tồn tại một số $a > 0$ sao cho
$$
|[f_1.f_2]| \leq a \|f_1\| \|f_2\|.
$$

#### Hệ quả {#fvr-v-s1-n1-cor-1 .statement}

*Nếu* $V$ *là một đại số chuẩn*, *nếu* $f_1, f_2$ *là hai hàm trong* $\mathcal{H}(\mathfrak{F}, V)$, *và* $g_1, g_2$ *là hai hàm trong* $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, *thì các quan hệ* $f_1 \preccurlyeq g_1, f_2 \preccurlyeq g_2$ *suy ra* $f_1 f_2 \preccurlyeq g_1 g_2$.

Quan hệ $f \preccurlyeq g$ giữa các hàm trong $\mathcal{H}(\mathfrak{F}, V)$ là *bắc cầu* theo mđ. 1; vì nó là *phản xạ* nên quan hệ "*f \preccurlyeq g and g \preccurlyeq f*" là một *quan hệ tương đương* trên $\mathcal{H}(\mathfrak{F}, V)$ (*Lý thuyết tập hợp*, II, p. 113).

#### Định nghĩa 2 {#fvr-v-s1-def-2 .statement}

*Cho hai hàm* $f, g$ *của* $\mathcal{H}(\mathfrak{F}, V)$ *ta nói rằng* $f$ *và* $g$ *là tương tự (theo* $\mathfrak{F}$*), và viết* $f \simeq g$, *nếu* $f \preccurlyeq g$ *và* $g \preccurlyeq f$.

Với mọi vô hướng $\lambda \neq 0$ quan hệ $f \simeq g$ tương đương với $f \simeq g \lambda$. Nó suy ra sự tồn tại của một tập $X \in \mathfrak{F}$ sao cho tập con của $X$ gồm các điểm mà ở đó $f(x) = 0$ trùng với tập con của $X$ gồm các điểm mà ở đó $g(x) = 0$.

#### Ví dụ 1 {#fvr-v-s1-n1-exa-1 .statement}

Với một hàm thực $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$ quan hệ $f \simeq 1$ có nghĩa là có hai số $a > 0,\ b > 0$ sao cho $a \leq |f(x)| \leq b$ trên một tập trong $\mathfrak{F}$, hay rằng hàm số $\log |f|$ bị chặn trên một tập trong $\mathfrak{F}$: khi đó người ta nói rằng $f$ *bị chặn theo lôgarit* trên một tập trong $\mathfrak{F}$.

#### Ví dụ 2 {#fvr-v-s1-n1-exa-2 .statement}

Cho $V$ là một không gian định chuẩn trên một trường có định giá không rời rạc $K$, và cho $f(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n$ là một đa thức theo biến $x \in K$, với các hệ số trong $V$, sao cho $a_0 \neq 0$. Với mọi vectơ $b \neq 0$ ta có $f(x) \simeq b x^n$ khi $|x|$ tiến tới $+\infty$.

#### Ví dụ 3 {#fvr-v-s1-n1-exa-3 .statement}

Ta đã thấy rằng $\sin^2 x \preccurlyeq \sin x$ khi $x$ tiến tới $+\infty$, nhưng *ta không có* $\sin^2 x \simeq \sin x$, mặc dù các hàm này triệt tiêu tại cùng các điểm.

#### Ví dụ 4 {#fvr-v-s1-n1-exa-4 .statement}

Ta có $x^2 + xy + y^2 \simeq x^2 + y^2$ khi $(x,\ y)$ tiến tới $(0,\ 0)$ trong $\mathbf{R}^2$, nhưng *không* $xy \simeq x^2 + y^2$.

Suy ra ngay từ mệnh đề 3 của V, p. 213, rằng nếu $f_1,\ f_2,\ g_1,\ g_2$ là các hàm trong $\mathcal{H}(\mathfrak{F}, K)$ ($K$ là bất kỳ trường có định giá nào) thì các quan hệ $f_1 \simeq g_1$ và $f_2 \simeq g_2$ suy ra $f_1 f_2 \simeq g_1 g_2$.

Ta nhận xét rằng ngược lại các quan hệ $f_1 \simeq g_1$ và $f_2 \simeq g_2$ *không suy ra rằng* $f_1 + f_2 \simeq g_1 + g_2$, như được chỉ ra bởi ví dụ $f_1(x) = g_1(x) = x^2,\ f_2(x) = -(x^2 + x),\ g_2(x) = -(x^2 - 1)$, khi biến thực $x$ tiến tới $+\infty$.

Các quan hệ so sánh $f \preccurlyeq g,\ f \simeq g$ được gọi là *yếu*. Ta nói rằng hai hàm $f,\ g$ từ $\mathcal{H}(\mathfrak{F}, V)$ là *so sánh được yếu* nếu chúng thỏa mãn một trong các quan hệ $f \preccurlyeq g,\ g \preccurlyeq f$.

#### Nhận xét 1 {#fvr-v-s1-n1-rem-1 .statement}

Hai hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ không nhất thiết so sánh được yếu, như được chỉ ra bởi ví dụ về các hàm 1 và $x \sin x$ khi $x$ tiến tới $+\infty$.

#### Nhận xét 2 {#fvr-v-s1-n1-rem-2 .statement}

Đặt $R_0$ là quan hệ $f \simeq g$ trên $\mathcal{H}(\mathfrak{F}, V)$, và đặt $\mathcal{H}_0(\mathfrak{F}, V)$ là tập thương $\mathcal{H}(\mathfrak{F}, V)/R_0$; chú ý rằng quan hệ $R$ *suy ra* $R_0$. Chuyển qua tập thương, quan hệ $f \preccurlyeq g$ cho, theo mệnh đề 1 của V, p. 213, một *quan hệ thứ tự* trên $\mathcal{H}_0(\mathfrak{F}, V)$ (*Lý thuyết tập hợp*, III, p. 134); ví dụ trước cho thấy rằng $\mathcal{H}_0(\mathfrak{F}, V)$ *không được sắp thứ tự toàn phần* bởi quan hệ này.

### 2. CÁC QUAN HỆ SO SÁNH: II. CÁC QUAN HỆ MẠNH

#### Định nghĩa 3 {#fvr-v-s1-def-3 .statement}

*Cho hai hàm thực* $f,\ g$ *thuộc* $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, *mà đều* $\geq 0$ *trên một tập trong* $\mathfrak{F}$, *ta nói rằng* $f$ *không đáng kể so với* $g$, *hay rằng* $g$ *trội hơn* $f$ *(theo* $\mathfrak{F}$), *và viết* $f \ll g$ *hoặc* $g \gg f$ *nếu, với mọi* $\varepsilon > 0$, *tồn tại một tập* $X \in \mathfrak{F}$ *sao cho* $f(t) \leq \varepsilon g(t)$ *với mọi* $t \in X$.

*Cho hai không gian định chuẩn* $V_1,\ V_2$ *và hai hàm* $f_1,\ f_2$ *lần lượt thuộc* $\mathcal{H}(\mathfrak{F}, V_1)$ *và* $\mathcal{H}(\mathfrak{F}, V_2)$, *ta nói rằng* $f_1$ *không đáng kể so với* $f_2$ *(theo* $\mathfrak{F}$), *và viết* $f_1 \ll f_2$ *hoặc* $f_2 \gg f_1$, *nếu* $\|f_1\| \ll \|f_2\|$.

Với mọi vô hướng $\lambda \neq 0$, quan hệ $f_1 \ll f_2 \lambda$ *tương đương* với $f_1 \ll f_2$. Quan hệ $f_1 \ll f_2$ suy ra $f_1 \preccurlyeq f_2$ nhưng không tương đương với nó.

Chú ý rằng quan hệ $f_1 \preccurlyeq f_2$ hoàn toàn không suy ra quan hệ "f_1 \ll f_2 \text{ hoặc } f_1 \asymp f_2 \text{": ta có } \sin x \preccurlyeq 1 \text{ khi } x \text{ tiến tới } +\infty, \text{ nhưng không quan hệ nào trong hai quan hệ } \sin x \ll 1 \text{ hoặc } \sin x \asymp 1 \text{ là đúng.}"

*Ví dụ.* 1) Quan hệ $f \ll 1$ có nghĩa là $f$ *tiến tới 0 theo* $\mathfrak{F}$.

2) Khi $\alpha$ và $\beta$ là hai số thực sao cho $\alpha < \beta$ ta có $x^\alpha \ll x^\beta$ khi $x$ tiến tới $+\infty$. Tương tự, khi $m$ và $n$ là hai số nguyên sao cho $m < n$ ta có $z^m \ll z^n$ khi số phức $z$ tiến tới $\infty$.

3) Khi $x$ tiến tới $+\infty$ ta có $x^n \ll e^x$ với mọi số nguyên $n$ (III, p. 105).

4) Trong $\mathbf{R}^2$ ta có, khi $(x, y)$ tiến tới $(0, 0)$,
$$
x^2 + y^2 \ll |x| + |y|.
$$

Các mệnh đề sau có thể được suy ra ngay lập tức từ định nghĩa 3:

#### Mệnh đề 4 {#fvr-v-s1-prop-4 .statement}

*Nếu $f, g, h$ là ba hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ thì các quan hệ $f \preccurlyeq g$ và $g \ll h$ (resp. $f \ll g$ và $g \preccurlyeq h$) suy ra $f \ll h$. \*

#### Mệnh đề 5 {#fvr-v-s1-prop-5 .statement}

*Cho $f_1, f_2$ là hai hàm trong $\mathcal{H}(\mathfrak{F}, V)$ và $g$ là một hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$. Khi đó các quan hệ $f_1 \ll g$ và $f_2 \ll g$ suy ra $f_1 + f_2 \ll g$. \*

Hơn nữa, lập luận tương tự như trong mệnh đề 3 của V, p. 213 cho thấy rằng:

#### Mệnh đề 6 {#fvr-v-s1-prop-6 .statement}

*Với ký hiệu của mệnh đề 3, các quan hệ $f_1 \ll g_1$ và $f_2 \preccurlyeq g_2$ (resp. $f_1 \preccurlyeq g_1$ và $f_2 \ll g_2$) suy ra $[f_1.f_2] \ll g_1g_2$. \*

Mệnh đề 4 cho thấy quan hệ $f \ll g$ giữa các hàm trong $\mathcal{H}(\mathfrak{F}, V)$ là *bắc cầu*; nhưng *nó không phản xạ*: nói chính xác hơn, quan hệ $f \ll f$ suy ra rằng $f$ *triệt tiêu trên một tập hợp trong $\mathfrak{F}$* (nói cách khác, $f$ tương đương với 0 modulo $R_\infty$); thật vậy, với một $\varepsilon$ sao cho $0 < \varepsilon < 1$ tồn tại một $X \in \mathfrak{F}$ sao cho $\|f(x)\| \leq \varepsilon \|f(x)\|$ với mọi $x \in X$, điều này chỉ có thể xảy ra nếu $f(x) = 0$ với mọi $x \in X$. Suy ra quan hệ "f \ll g và g \ll f" là bắc cầu và đối xứng, nhưng không phản xạ: do đó nó không phải là một quan hệ tương đương (nó suy ra rằng tồn tại một tập hợp $X \in \mathfrak{F}$ sao cho $f(x) = g(x) = 0$ với mọi $x \in X$).

#### Mệnh đề 7 {#fvr-v-s1-prop-7 .statement}

*Nếu $f$ và $g$ là hai hàm trong $\mathcal{H}(\mathfrak{F}, V)$ thì quan hệ $f - g \ll f$ tương đương với $f - g \ll g$. \*

Thật vậy, $f - g \ll f$ suy ra rằng với mọi $\varepsilon > 0$ tồn tại một $X \in \mathfrak{F}$ sao cho $\|f(x) - g(x)\| \leq \varepsilon \|f(x)\|$ với mọi $x \in X$. Nhưng khi đó $(1 - \varepsilon) \|f(x)\| \leq \|g(x)\|$, và do đó $f \preccurlyeq g$, suy ra (V, p. 215, mệnh đề 4) $f - g \ll g$.

#### Hệ quả {#fvr-v-s1-n2-cor-1 .statement}

*Quan hệ $f - g \ll f$ là một quan hệ tương đương trên $\mathcal{H}(\mathfrak{F}, V)$. \*

Thật vậy, nếu $f - g \ll f$ và $g - h \ll g$ thì $f - g \ll g$, do đó (V, p. 215, mệnh đề 5) $f - h \ll g$, và do đó, vì $g \preceq f$, ta có $f - h \ll f$, điều này cho thấy quan hệ này là bắc cầu; nó đối xứng theo mệnh đề 7, và rõ ràng là phản xạ, suy ra hệ quả.

#### Định nghĩa 4 {#fvr-v-s1-def-4 .statement}

*Cho hai hàm* $f, g$ *của* $\mathcal{H}(\mathfrak{F}, V)$ *người ta nói rằng* $f$ *và* $g$ *tương đương (theo* $\mathfrak{F}$), *và viết* $f \sim g$, *nếu* $f - g \ll f$.

Quan hệ $f \sim g$ suy ra $f \asymp g$ nhưng không tương đương với nó.

#### Ví dụ 1 {#fvr-v-s1-n2-exa-1 .statement}

Nếu $a$ là một hàm hằng, $\neq 0$ trên $E$, thì quan hệ $f \sim a$ có nghĩa là $f$ *tiến tới* $a$ *theo* $\mathfrak{F}$.

#### Ví dụ 2 {#fvr-v-s1-n2-exa-2 .statement}

Cho $V$ là một không gian chuẩn trên một trường định giá không rời rạc $K$, và cho $f(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n$ là một đa thức theo biến $x \in K$, với các hệ số trong $V$, sao cho $a_0 \neq 0$. Khi đó $f(x) \sim a_0 x^n$ khi $|x|$ tiến tới $+\infty$.

#### Ví dụ 3 {#fvr-v-s1-n2-exa-3 .statement}

Khi số thực $x$ tiến tới $+\infty$ ta có $\left( 1 + \frac{1}{x} \right) \sin x \sim \sin x$.

#### Ví dụ 4 {#fvr-v-s1-n2-exa-4 .statement}

Khi biến phức $z$ tiến tới 0 ta có $e^z - 1 \sim z$. Nói chung hơn, nếu $V$ là một không gian chuẩn trên một trường định giá $K$, và $f$ là một hàm được xác định trên một lân cận của $x_0 \in K$, với giá trị trong $V$, và có đạo hàm $f'(x_0) \neq 0$ tại điểm $x_0$, thì, khi $x$ tiến tới $x_0$, ta có $f(x) - f(x_0) \sim f'(x_0)(x - x_0)$ (I, p. 3, định nghĩa 1).

#### Ví dụ 5 {#fvr-v-s1-n2-exa-5 .statement}

Khi $(x, y)$ tiến tới $(0, 0)$ trong $\mathbf{R}^2$ ta có
$$
\sqrt{\sin^2 x + \sin^2 y} \sim \sqrt{x^2 + y^2}.
$$

#### Ví dụ 6 {#fvr-v-s1-n2-exa-6 .statement}

Cho $f(x, y)$ là một đa thức với hệ số thực theo hai biến thực $x, y$, không có số hạng tự do. Nếu, khi $x$ tiến tới 0 mà vẫn $> 0$, có một hàm $\varphi(x)$, liên tục trên một khoảng $[0, a]$, và sao cho $\varphi(0) = 0$ và $f(x, \varphi(x)) = 0$ với $0 \leq x \leq a$, ta có thể chứng minh rằng tồn tại một số hữu tỉ $r$ và một số thực $\lambda \neq 0$ sao cho $\varphi(x) \sim \lambda x^r$ (V, p. 259, exerc. 3).

#### Ví dụ 7 {#fvr-v-s1-n2-exa-7 .statement}

Với mọi $x > 0$ đặt $\pi(x)$ là số các số nguyên tố $\leq x$; người ta đã chứng minh rằng $\pi(x) \sim x / \log x$ $^2$ khi $x$ tiến tới $+\infty$.

#### Nhận xét {#fvr-v-s1-n2-rem-3 .statement}

Chú ý rằng quan hệ $f \sim g$ hoàn toàn không suy ra rằng hiệu $f - g$ tiến tới 0 dọc theo $\mathfrak{F}$; hiệu này thậm chí có thể *không bị chặn*, như được chỉ ra bởi ví dụ $x^2 + x \sim x^2$ khi $x$ tiến tới $+\infty$.

#### Mệnh đề 8 {#fvr-v-s1-prop-8 .statement}

*Cho* $K$ *là một trường định giá và* $f_1, f_2, g_1, g_2$ *là bốn hàm trong* $\mathcal{H}(\mathfrak{F}, K)$; *khi đó các quan hệ* $f_1 \sim g_1$ *và* $f_2 \sim g_2$ *suy ra* $f_1 f_2 \sim g_1 g_2$.

Thật vậy, ta có $f_1 f_2 - g_1 g_2 = f_1 (f_2 - g_2) + (f_1 - g_1) g_2$; vì $f_1 \preceq g_1$, $f_1 - g_1 \ll g_1$ và $f_2 - g_2 \ll g_2$, ta có $f_1 f_2 - g_1 g_2 \ll g_1 g_2$ (V, p. 215, prop. 5 and 6).

Trái lại, ta đã cho một ví dụ ở V, p. 214 trong đó có $f_1 = g_1$, $f_2 \sim g_2$ mà quan hệ $f_1 + f_2 \asymp g_1 + g_2$ không đúng (nên đương nhiên cũng không có
$$
f_1 + f_2 \sim g_1 + g_2).
$$
2 Xem, chẳng hạn, A. E. INGHAM, *The distribution of prime numbers* (Cambridge Tracts, n 30), Cambridge University Press, 1932.

Các quan hệ so sánh $f \ll g, f \sim g$ được gọi là các quan hệ mạnh. Hai hàm $f, g$ từ $\mathcal{H}(\mathfrak{F}, V)$ được gọi là tương đẳng được so sánh (hoặc tương đẳng mạnh nếu muốn tránh mọi nhầm lẫn có thể xảy ra) nếu chúng thỏa mãn một trong ba quan hệ: $f \ll g, f \gg g$, hoặc "tồn tại một $\lambda \neq 0$ sao cho $f \sim g\lambda$".

#### Nhận xét 1 {#fvr-v-s1-n2-rem-1 .statement}

Hai hàm có thể yếu tương đẳng mà không mạnh tương đẳng, chẳng hạn các hàm 1 và $\sin x$ khi $x$ tiến tới $+\infty$.

#### Nhận xét 2 {#fvr-v-s1-n2-rem-2 .statement}

Trong các định nghĩa của các quan hệ so sánh $f_1 \preccurlyeq f_2$ và $f_1 \ll f_2$ các chuẩn trên các không gian $V_1, V_2$ mà $f_1$ và $f_2$ lần lượt nhận giá trị, chỉ được xét một cách hình thức; trên thực tế chỉ các tôpô trên $V_1$ và $V_2$ được xét, vì các quan hệ $f_1 \preccurlyeq f_2$ và $f_1 \ll f_2$ được thay bởi các quan hệ tương đương khi thay chuẩn trên $V_1$ hoặc $V_2$ bằng một chuẩn tương đương (\emph{Gen. Top.}, IX, p. 170, def. 7).

### 3. THAY ĐỔI BIẾN SỐ

Let $\varphi$ be a map from the set $E'$ into $E$ such that $\varphi^{-1}(\mathfrak{F})$ is a filter base on $E'$. Rõ ràng là nếu $f_1, f_2$ lần lượt là các hàm trong $\mathcal{H}(\mathfrak{F}, V_1)$ và $\mathcal{H}(\mathfrak{F}, V_2)$, thì $f_1 \circ \varphi, f_2 \circ \varphi$ lần lượt thuộc $\mathcal{H}(\varphi^{-1}(\mathfrak{F}), V_1)$ và $\mathcal{H}(\varphi^{-1}(\mathfrak{F}), V_2)$, và quan hệ $f_1 \preccurlyeq f_2$ (resp. $f_1 \ll f_2$) tương đương với $f_1 \circ \varphi \preccurlyeq f_2 \circ \varphi$ (resp. $f_1 \circ \varphi \ll f_2 \circ \varphi$).

### 4. CÁC QUAN HỆ SO SÁNH GIỮA CÁC HÀM DƯƠNG NGẶT

Let $g$ be a function in $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ which is strictly positive on a set in $\mathfrak{F}$. Các quan hệ so sánh có chứa $g$ có thể được phát biểu theo một cách khác: quan hệ $f \preccurlyeq g$ tương đương với nói rằng $\|f\|/g$ (which is defined on a set in $\mathfrak{F}$) bị chặn trên trên một tập hợp trong $\mathfrak{F}$; quan hệ $f \ll g$ tương đương với nói rằng $\|f\|/g$ tiến tới 0 dọc theo $\mathfrak{F}$. If $f$ is a function in $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ quan hệ $f \asymp g$ có nghĩa là $f/g$ bị chặn theo lôgarit trên một tập hợp trong $\mathfrak{F}$, và quan hệ $f \sim g$ rằng $f/g$ tiến tới 1 dọc theo $\mathfrak{F}$. If $f$ is a function in $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ and positive on a set in $\mathfrak{F}$, nói rằng $f$ và $g$ là so sánh được suy ra rằng $f/g$ tiến tới một giới hạn (hữu hạn hoặc bằng $+\infty$) dọc theo $\mathfrak{F}$.

#### Mệnh đề 9 {#fvr-v-s1-prop-9 .statement}

Cho $f$ và $g$ là hai hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, dương ngặt trên một tập hợp trong $\mathfrak{F}$. Để $f$ và $g$ là so sánh được thì cần và đủ là với mọi số $t \geqslant 0$, trừ nhiều nhất một ngoại lệ, hàm $f - tg$ có dấu không đổi $^3$ trên một tập hợp trong $\mathfrak{F}$.

Điều kiện là cần thiết. Thật vậy, nếu $f \ll g$ thì ta có $f - tg \sim -tg$ trừ trường hợp $t = 0$, do đó $f - tg$ là âm ngặt trên một tập hợp thuộc $\mathfrak{F}$, trừ trường hợp $t = 0$; nếu $f \gg g$ thì $f - tg$ là dương ngặt trên một tập hợp thuộc $\mathfrak{F}$ với mọi $t$; cuối cùng, nếu $f \sim kg$ ($k$ hằng $> 0$), thì $f - t g \sim (k - t)g$ trừ trường hợp $t = k$, do đó, trừ có lẽ trường hợp $t = k$, $f - t g$ có dấu của $k - t$ trên một tập hợp thuộc $\mathfrak{F}$.

Điều kiện là đủ. Thật vậy, giả sử rằng tỉ số $f/g$ có hai điểm tụ phân biệt $\alpha < \beta$ theo $\mathfrak{F}$. Khi đó, với *mọi* số $t$ sao cho $\alpha < t < \beta$ tồn tại trong *mọi* tập hợp $X \in \mathfrak{F}$ hai điểm $x_1, x_2$ sao cho $f(x_1)/g(x_1) < t$ và $f(x_2)/g(x_2) > t$; do đó $f(x) - t g(x)$ không có dấu hằng trên $X$; ta đã đi đến một kết luận không tương thích với giả thiết. Suy ra rằng $f/g$ chỉ có thể có *một* giá trị tụ (hữu hạn hoặc vô hạn) theo bộ lọc có cơ sở là $\mathfrak{F}$, và do đó, (*Gen. Top.*, I, p. 85, hệ quả) có giá trị này làm *giới hạn* của nó theo $\mathfrak{F}$.

#### Mệnh đề 10 {#fvr-v-s1-prop-10 .statement}

*Cho $f$ và $g$ là hai hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ dương ngặt trên một tập hợp thuộc $\mathfrak{F}$; với mọi $\alpha$ thực và $\neq 0$ thì quan hệ $f \asymp g$ (resp. $f \sim g$) tương đương với $f^\alpha \asymp g^\alpha$ (resp. $f^\alpha \sim g^\alpha$); nếu $\alpha > 0$ thì quan hệ $f \preccurlyeq g$ (resp. $f \ll g$) tương đương với $f^\alpha \preccurlyeq g^\alpha$ (resp. $f^\alpha \ll g^\alpha$); nếu $\alpha < 0$ thì nó tương đương với $f^\alpha \succcurlyeq g^\alpha$ (resp. $f^\alpha \succ g^\alpha$).*

Các chứng minh là ngay lập tức.

Một nhận thấy rằng trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ tập hợp $I'$ các hàm dương ngặt trên một tập trong $\mathfrak{F}$ là như vậy rằng $\Gamma/\mathbf{R}_\infty$ là một *nhóm nhân* $\Gamma_\infty$ trong $\mathcal{H}_\infty(\mathfrak{F}, \mathbf{R})$; $\Gamma/\mathbf{R}_0$ trùng với nhóm thương của $\Gamma_\infty$ bởi nhóm con các lớp (mod. $\mathbf{R}_\infty$) của các hàm bị chặn logarit trong $\Gamma$; trên $\Gamma/\mathbf{R}_0$ quan hệ thứ tự suy ra từ quan hệ $f \preccurlyeq g$ khi đi qua thương là *tương thích* với cấu trúc nhóm của $\Gamma/\mathbf{R}_0$ và do đó biến nó thành một nhóm có thứ tự.

#### Mệnh đề 11 {#fvr-v-s1-prop-11 .statement}

*Cho $g$ là một hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ sao cho $\lim_{\mathfrak{F}} g = +\infty$; quan hệ $f \ll g$ kéo theo $e^f \ll e^g$; quan hệ $f \sim g$ kéo theo $\log f \sim \log g$.*

Thật vậy, nếu $f \ll g$ thì $f - g = g \left( \frac{f}{g} - 1 \right)$ tiến tới $-\infty$ theo $\mathfrak{F}$. Tương tự, nếu $f \sim g$ ta có $\log f = \log g + \log \frac{f}{g}$, nên $\log f - \log g$ tiến tới 0, và tương tự cho $\frac{\log f}{\log g} - 1 = \frac{\log f - \log g}{\log g}$.

Mặt khác, lưu ý rằng quan hệ $f \sim g$ *không kéo theo* $e^f \sim e^g$, cũng không kéo theo ngay cả $e^f \asymp e^g$, như được cho thấy bởi ví dụ trong đó $f(x) = x^2, \ g(x) = x^3 + x$ khi $x$ tiến tới $+\infty$; tương tự, quan hệ $f \ll g$ *không kéo theo* $\log f \ll \log g$, như được cho thấy bởi ví dụ $f(x) = x, \ g(x) = x^2$ khi $x$ tiến tới $+\infty$.

#### Định nghĩa 5 {#fvr-v-s1-def-5 .statement}

*Cho $g$ là một hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$, dương ngặt trên một tập trong $\mathfrak{F}$, và sao cho $\lim_{\mathfrak{F}} g = 0$ hoặc $\lim_{\mathfrak{F}} g = +\infty$. Người ta nói rằng một hàm $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$ có cấp $\rho$ (hữu hạn hoặc vô hạn) tương đối với $g$ nếu $\lim_{\mathfrak{F}} \log(|f|)/\log g = \rho$.*

Lưu ý rằng nếu $f$ có cấp $\rho$ tương đối với $g$ thì $f$ có cấp $-\rho$ tương đối với $1/g$; do đó chỉ cần xét trường hợp $g(x)$ tiến tới $+\infty$ theo $\mathfrak{F}$.

#### Mệnh đề 12 {#fvr-v-s1-prop-12 .statement}

Cho g là một hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ sao cho $\lim_{\mathfrak{F}} g = +\infty$; cho f là một hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$.

a) Để f có cấp $+\infty$ đối với g thì cần và đủ là $f \gg g^\alpha$ với mọi $\alpha \geq 0$.

b) Để f có cấp $-\infty$ đối với g thì cần và đủ là $f \ll g^{-\alpha}$ với mọi $\alpha > 0$.

c) Để f có cấp hữu hạn bằng $\rho$ đối với g thì cần và đủ là, với mọi $\varepsilon > 0$, ta có $g^{\rho-\varepsilon} \ll f \ll g^{\rho+\varepsilon}$.

Hãy chứng minh c) chẳng hạn. Nếu cấp của f đối với g là $\rho$ thì với mọi $\varepsilon > 0$ tồn tại một tập $M \in \mathfrak{F}$ sao cho, với mọi $x \in M$, ta có

$$
\left( \rho - \frac{\varepsilon}{2} \right) \log g(x) \leq \log |f(x)| \leq \left( \rho + \frac{\varepsilon}{2} \right) \log g(x),
$$

hay $(g(x))^{\rho - \frac{\varepsilon}{2}} \leq |f(x)| \leq (g(x))^{\rho + \frac{\varepsilon}{2}}$; vì $\lim_{\mathfrak{F}} g = +\infty$ nên do đó ta có $g^{\rho-\varepsilon} \ll f \ll g^{\rho+\varepsilon}$ với mọi $\varepsilon > 0$; chiều ngược lại hiển nhiên. Chứng minh của a) và b) là tương tự.

Lưu ý rằng nếu f có cấp hữu hạn $\rho$ đối với g thì $fg^{-\rho}$ có cấp 0 đối với g, và ngược lại; nếu $f_1$ (resp. $f_2$) có cấp $\rho_1$ (resp. $\rho_2$) đối với g, và nếu $\rho_1 + \rho_2$ được xác định, thì $f_1 f_2$ có cấp $\rho_1 + \rho_2$ đối với g.

#### Nhận xét 1 {#fvr-v-s1-n4-rem-1 .statement}

Hãy lưu ý rằng mặc dù f có thể có cấp hữu hạn $\rho$ đối với g, tỷ số $f/g^\rho$ vẫn có thể không tiến tới một giới hạn; chẳng hạn, mọi hàm bị chặn theo lôgarit đều có cấp 0 đối với g, nhưng có thể không có giới hạn dọc theo $\mathfrak{F}$.

#### Nhận xét 2 {#fvr-v-s1-n4-rem-2 .statement}

Một hàm xác định trên một tập thuộc $\mathfrak{F}$ có thể không có cấp xác định (hữu hạn hay không) đối với g, vì các hàm có cấp xác định đối với g đều so sánh được với mọi lũy thừa của g, nhiều nhất là một ngoại lệ. Còn f thì có thể không có tính chất này, như thấy từ ví dụ $g(x) = x,\ f(x) = 1 + x^2 \sin^2 x$ (khi x tiến tới $+\infty$). Trong ví dụ này f so sánh được với $g^\alpha$ với $\alpha < 0$ và $\alpha > 2$; nếu lấy $f(x) = e^x \sin^2 x + e^{-x} \cos^2 x$ thì f không so sánh được với bất kỳ lũy thừa nào (dương hay âm) của g.

### 5. KÝ HIỆU

Cho một hàm thực $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$ thì trong một công thức thường tiện viết $O(f)$ cho một hàm bị khống chế bởi f, và $o(f)$ cho một hàm không đáng kể đối với f. Khi, trong một chứng minh, có nhiều hàm bị cùng một hàm f khống chế (tương ứng, không đáng kể đối với f) thì ta ký hiệu chúng là $O_1(f),\ O_2(f)$, v.v. (tương ứng, $o_1(f),\ o_2(f)$, v.v.).

Nhiều tác giả viết $O(f)$ (tương ứng $o(f)$) một cách không phân biệt cho mọi hàm trong một chứng minh bị khống chế bởi f (tương ứng, không đáng kể đối với f), một lối dùng từ lạm dụng có thể gây nhầm lẫn.

Với ký hiệu này, ta có thể diễn đạt các mệnh đề 1, 2, 3 (V, p. 213) như sau: nếu $g = O_1(f)$ và $h = O(g)$ thì $h = O_2(f)$; ta có thể viết

$$
\sum_{i=1}^{n} \lambda_i O_i(f) = O_{n+1}(f) \quad (\lambda_i \text{ các vô hướng}) \tag{1}
$$
$$
O(f) \, O(g) = O(fg). \tag{2}
$$

Tương tự, mệnh đề 4 (V, p. 215) cho thấy rằng nếu $g = O_1(f)$ và $h = o(g)$ (resp. $g = o_1(f)$ và $h = O(g)$) thì $h = o_2(f)$, và các mệnh đề 5 và 6 (V, p. 5) có thể được diễn đạt dưới dạng
$$
\sum_{i=1}^{n} \lambda_i o_i(f) = o_{n+1}(f) \quad (\lambda_i \text{ các vô hướng}) \tag{3}
$$
$$
o(f) \, O(g) = o(fg). \tag{4}
$$

Quan hệ $f \sim g$ tương đương với $f = g + o(g)$. Ký hiệu $O(1)$ (resp. $o(1)$) chỉ một hàm bị chặn trên một tập hợp trong $\mathfrak{F}$ (resp. một hàm tiến tới 0 dọc theo $\mathfrak{F}$).

### Bài tập {#fvr-v-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
