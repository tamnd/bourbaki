---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 2
section_title: ASYMPTOTIC EXPANSIONS
lang: vi
source: fvr-i-vii
pdf_pages: 0235-0242
extraction: ocr
subsections:
    - "no": 1
      title: SCALES OF COMPARISON
      page: 0
      pdf_page: 235
    - "no": 2
      title: PRINCIPAL PARTS AND ASYMPTOTIC EXPANSIONS
      page: 0
      pdf_page: 236
    - "no": 3
      title: SUMS AND PRODUCTS OF ASYMPTOTIC EXPANSIONS
      page: 0
      pdf_page: 238
    - "no": 4
      title: COMPOSITION OF ASYMPTOTIC EXPANSIONS
      page: 0
      pdf_page: 239
    - "no": 5
      title: ASYMPTOTIC EXPANSIONS WITH VARIABLE COEFFICIENTS
      page: 0
      pdf_page: 241
statements: 12
exercises: 0
content_sha256: 681123887075c4ca35c4426e4c50dd4c48c1c27e5710a4dee028f183e8c4eaf1
translated_from: content/en/fvr/V/02_s2_asymptotic_expansions.md
source_content_sha256: b37ae9ead916beb8ee26900f2ecf0229caf81e067950a00605a7b4ef490a7455
translation_model: gpt-5.4
translation_run: translate-vi-bc8cfeda
glossary_version: 34
glossary_terms_sha256: e4c73ec18e159841a7b1c9632bc02c0a1a9a2b49d69faa2003de64a2e645652b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. KHAI TRIỂN TIỆM CẬN

### 1. THANG SO SÁNH

Cho E là một tập hợp được lọc bởi một bộ lọc có cơ sở $\mathfrak{F}$, và K là một trường định giá không rời rạc (thường nhất là $K = \mathbf{R}$ hoặc $K = \mathbf{C}$). Trên tập hợp các hàm trong $\mathcal{H}(\mathfrak{F}, K)$ không tương đương với 0 modulo $R_\infty$ (nghĩa là, những hàm mà trong mọi tập hợp thuộc $\mathfrak{F}$ đều có ít nhất một điểm tại đó hàm không triệt tiêu), quan hệ " $f \ll g$ or $f = g$" là một quan hệ thứ tự.

#### Định nghĩa 1 {#fvr-v-s2-def-1 .statement}

*Người ta nói rằng một tập con $\mathcal{E}$ của $\mathcal{H}(\mathfrak{F}, K)$, gồm các hàm không tương đương với 0 modulo $R_\infty$, là một thang so sánh khi $\mathcal{E}$ được sắp thứ tự toàn phần bởi quan hệ " $f \ll g$ or $f = g$".*

Nói cách khác, nếu $f$ và $g$ là các hàm trong $\mathcal{E}$ thì một (và chỉ một) trong các quan hệ $f \ll g$, $g \ll f$, $f = g$ luôn đúng. Suy ra rằng trên $\mathcal{E}$, *quan hệ* $f \asymp g$ (và *a fortiori* $|f| \sim a\,|g|$, trong đó $a$ là một số $> 0$) *kéo theo* $f = g$.

Mọi tập con của một thang so sánh rõ ràng cũng là một thang so sánh.

#### Ví dụ 1 {#fvr-v-s2-n1-exa-1 .statement}

Với $x$ thực và tiến tới $+\infty$ thì tập hợp các hàm $x^\alpha$ ($\alpha$ là một số thực tùy ý) là một thang so sánh. Điều tương tự cũng đúng đối với các hàm $(x-a)^\alpha$ khi $\mathfrak{F}$ là tập hợp các khoảng mở có đầu mút trái là $a$.

#### Ví dụ 2 {#fvr-v-s2-n1-exa-2 .statement}

Với $z$ phức và tiến tới $\infty$ thì tập hợp các hàm $z^n$ ($n$ là một số nguyên) là một thang so sánh; các hàm $(z-a)^n$ cũng vậy khi $\mathfrak{F}$ là vết trên phần bù của điểm $a \in \mathbf{C}$ của bộ lọc các lân cận của điểm này.

#### Ví dụ 3 {#fvr-v-s2-n1-exa-3 .statement}

Cho F là một không gian chuẩn; họ các hàm $\|x-\mathbf{a}\|^\alpha$ ($\alpha$ là một số thực tùy ý) là một thang so sánh khi $\mathfrak{F}$ là vết trên phần bù của $\mathbf{a}$ của bộ lọc các lân cận của điểm này. Chú ý rằng nếu $p$ và $q$ là hai chuẩn phân biệt trên F, thì hợp của hai thang so sánh $(p(x-\mathbf{a}))^\alpha$ và $(q(x-\mathbf{a}))^\alpha$ nói chung không phải là một thang so sánh.

#### Ví dụ 4 {#fvr-v-s2-n1-exa-4 .statement}

Khi $x$ thực tiến tới $+\infty$, họ $\mathcal{E}$ các hàm có dạng $\exp(p(x))$, trong đó $p$ chạy qua tập hợp các *đa thức không có hằng số* (với hệ số thực), là một thang so sánh: chỉ cần nhận xét rằng thương của hai hàm trong $\mathcal{E}$ lại thuộc $\mathcal{E}$, và một hàm $\exp(p(x))$ ắt phải tiến tới 0 hoặc $+\infty$ nếu $p \neq 0$; quả thật, $p(x) \sim \alpha x^n$ với $n > 0$ và $\alpha \neq 0$; nếu $\alpha > 0$ thì $p(x) > \frac{1}{2} \alpha x^n$ với $x$ đủ lớn; nếu $\alpha < 0$ thì $p(x) < \frac{1}{2} \alpha x^n$ với $x$ đủ lớn; trong trường hợp thứ nhất $\exp(p(x))$ tiến tới $+\infty$, trong trường hợp thứ hai tiến tới 0.

#### Ví dụ 5 {#fvr-v-s2-n1-exa-5 .statement}

Khi $x$ thực tiến tới $+\infty$, tập hợp $\mathcal{E}$ các hàm dạng $x^\alpha (\log x)^\beta$ (được xác định với $x > 1$), trong đó $\alpha$ và $\beta$ là các số thực tùy ý, là một thang so sánh. Thật vậy, ở đây nữa thương của hai hàm trong $\mathcal{E}$ là một hàm trong $\mathcal{E}$; chỉ cần chỉ ra rằng nếu $\alpha$ và $\beta$ không đồng thời bằng không thì $x^\alpha (\log x)^\beta$ tiến tới 0 hoặc $+\infty$; điều này là hiển nhiên nếu $\alpha = 0, \beta \neq 0$; nếu $\alpha > 0$ thì ta có $(\log x)^{-\beta} \ll x^\alpha$, và nếu $\alpha < 0$ thì ta có $(\log x)^\beta \ll x^{-\alpha}$ với mọi $\beta$, do đó mệnh đề.

Chú ý rằng thang so sánh cuối cùng này là một tập sắp thứ tự toàn phần (đối với quan hệ "f $\ll$ g" hoặc $f = g$") mà cấu trúc thứ tự của nó đẳng cấu với thứ tự *từ điển* trên $\mathbf{R}^2$ (*Lý thuyết tập hợp*, III, p. 157); nhắc lại rằng trong cấu trúc này quan hệ $(\alpha, \beta) < (\gamma, \delta)$ có nghĩa là "$\alpha < \gamma$, hoặc $\alpha = \gamma$ và $\beta < \delta$").

Tương tự, thang được tạo bởi các hàm $\exp(p(x))$, trong đó $p$ chạy qua tập hợp $P_0$ các đa thức không có số hạng hằng, có cấu trúc thứ tự đẳng cấu với cấu trúc thứ tự của $P_0$, trong đó quan hệ $p < q$ kéo theo rằng số hạng trội của đa thức $q - p$ có hệ số $> 0$ (*x. Alg.*, VI. 19, *Ví dụ 2*).

Cho $\varphi$ là một ánh xạ từ một tập hợp F vào E, sao cho $\varphi^{-1}(\mathfrak{F})$ là một cơ sở bộ lọc trên F. Nếu $\mathcal{E}$ là một thang so sánh trên E (đối với cơ sở bộ lọc $\mathfrak{F}$) thì các hàm $f \circ \varphi$, khi $f$ chạy qua $\mathcal{E}$, tạo thành một thang so sánh trên F (đối với cơ sở bộ lọc $\varphi^{-1}(\mathfrak{F})$).

### 2. CÁC PHẦN CHÍNH VÀ CÁC KHAI TRIỂN TIỆM CẬN

Cho $\mathcal{E}$ là một thang so sánh được tạo bởi các hàm có giá trị trong một trường được định giá không rời rạc K. Cho V là một không gian định chuẩn trên K, và cho $\mathbf{f}$ là một hàm trong $\mathcal{H}(\mathfrak{F}, V)$; nếu tồn tại một hàm $g \in \mathcal{E}$ và một phần tử $\mathbf{a} \neq 0$ của V sao cho $\mathbf{f} \sim \mathbf{a}g$, ta nói rằng $\mathbf{a}g$ là một *phần chính* của $\mathbf{f}$ đối với thang $\mathcal{E}$. Theo định nghĩa 1 của V, p. 10, $\mathbf{f}$ chỉ có thể có *một* phần chính đối với $\mathcal{E}$, vì nếu $g_1,\ g_2$ là hai hàm trong $\mathcal{E}$ và $\mathbf{a}_1,\ \mathbf{a}_2$ là hai phần tử $\neq 0$ của V, thì quan hệ $\mathbf{a}_1 g_1 \sim \mathbf{a}_2 g_2$ kéo theo $|g_1| \asymp |g_2|$ và do đó $g_1 = g_2$, do đó $(\mathbf{a}_2 - \mathbf{a}_1)g_1 \ll g_1$, và vì $g_1$ không đồng nhất bằng không trên bất kỳ tập hợp nào trong $\mathcal{E}$ nên điều này kéo theo $\mathbf{a}_2 = \mathbf{a}_1$.

Nếu $\mathbf{f}$ có một phần chính đối với một thang so sánh $\mathcal{E}$ thì nó có *cùng* phần chính đó đối với mọi thang so sánh $\mathcal{E}' \supset \mathcal{E}$.

#### Ví dụ 1 {#fvr-v-s2-n2-exa-1 .statement}

Với $x$ thực (resp. phức) tiến tới $+\infty$ (resp. $\infty$), mọi đa thức $a_0 x^n + a_1 x^{n-1} + \ldots + a_n$ với các hệ số trong V, sao cho $a_0 \neq 0$, đều có phần chính là $a_0 x^n$ đối với thang $x^n$ (hoặc bất kỳ thang nào chứa các $x^n$). Suy ra mọi phân thức hữu tỉ $\frac{a_0 x^n + \cdots + a_m}{b_0 x^n + \cdots + b_n}$ với các hệ số thực hoặc phức sao cho $a_0 b_0 \neq 0$ đều có phần chính là $\frac{a_0}{b_0} x^n$ đối với cùng thang đó.

#### Ví dụ 2 {#fvr-v-s2-n2-exa-2 .statement}

Một hàm có thể so sánh được với mọi hàm của một thang mà vẫn không có phần chính đối với thang ấy. Ví dụ, khi $x$ thực tiến tới $+\infty$, $\sqrt{x}$ không có phần chính đối với thang $x^n$ trong đó $n$ là một số nguyên hữu tỉ; $\log x$ không có phần chính đối với thang các $x^\alpha$ ($\alpha$ thực tùy ý); $\exp(\sqrt{\log x})$ và $x' = e^{x \log x}$ không có phần chính đối với thang các $x^\alpha (\log x)^\beta$, cũng không đối với thang các $\exp(p(x))$ ($p$ là một đa thức không có số hạng hằng).

Khái niệm phần chính cho phép phép tổng quát hóa rộng rãi. Giả sử rằng một hàm $f \in \mathcal{H}(\mathfrak{F}, V)$ có phần chính $a_1 g_1$ đối với một thang $\mathcal{E}$; quan hệ $f \sim a_1 g_1$ là tương đương với $f - a_1 g_1 \ll g_1$ (V, p. 216, định nghĩa 4); do đó, để khảo sát hàm $f$ chặt chẽ hơn, ta được dẫn tới việc xét hàm $f - a_1 g_1$. Nếu hàm này có một phần chính $a_2 g_2$ đối với $\mathcal{E}$ thì phải có $g_2 \ll g_1$ và $f - a_1 g_1 - a_2 g_2 \ll g_2$.

Nói chung hơn, giả sử rằng thang $\mathcal{E}$ được viết dưới dạng tham số $(g_\alpha)$ trong đó $\alpha$ chạy qua một tập hợp chỉ số $A$ được trang bị một cấu trúc được sắp thứ tự toàn phần đẳng cấu với cấu trúc có thứ tự *đối* của $\mathcal{E}$: do đó quan hệ $\alpha < \beta$ là tương đương với $g_\beta \ll g_\alpha$. Trong những hoàn cảnh này:

#### Định nghĩa 2 {#fvr-v-s2-def-2 .statement}

*Ta nói rằng một hàm* $f \in \mathcal{H}(\mathfrak{F}, V)$ *có một khai triển tiệm cận đến cấp chính xác* $g_\alpha$ *(đối với thang* $\mathcal{E}$*) *nếu tồn tại một họ* $(a_\lambda)_{\lambda \leq \alpha}$ *các phần tử của* $V$, *mà tất cả trừ một số hữu hạn đều bằng* $0$, *sao cho* $f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \ll g_\alpha$. *Ta nói rằng* $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ *là một khai triển tiệm cận của* $f$ *đến cấp chính xác* $g_\alpha$, *rằng các* $a_\lambda g_\lambda$ ($\lambda \leq \alpha$) *là các số hạng của nó, các* $a_\lambda$ *là các hệ số của nó, và hàm* $r_\alpha = f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ *là số dư của khai triển này*.

Để diễn đạt việc $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ là một khai triển tiệm cận của $f$ với độ chính xác $g_\alpha$ người ta thường hạn chế ở cách viết

$$
f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o(g_\alpha) \quad \text{(hoặc } f = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + o_k(g_\alpha)
$$

nếu có nhiều hàm trong chứng minh), theo ký hiệu của V, p. 219 và 220.

Trong hai khai triển tiệm cận (của hai hàm, phân biệt hoặc không) đối với cùng một thang $\mathcal{E}$, người ta nói rằng khai triển có độ chính xác với chỉ số lớn hơn là khai triển *chính xác hơn*.

Nếu $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ là một khai triển tiệm cận của $f$ với độ chính xác $g_\alpha$, thì với mọi $\beta < \alpha$, $\sum_{\lambda \leq \beta} a_\lambda g_\lambda$ là một khai triển tiệm cận của $f$ với độ chính xác $g_\beta$ (V, p. 215, mệnh đề 5): người ta nói rằng nó thu được bằng cách *giảm độ chính xác* của khai triển đã cho $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ của $f$ xuống $g_\beta$.

Nếu $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ và $\sum_{\lambda \leq \alpha} b_\lambda g_\lambda$ là các khai triển tiệm cận đến *cùng* độ chính xác $g_\alpha$ của hai hàm $f_1, f_2$, thì $\sum_{\lambda \leq \alpha} (a_\lambda + b_\lambda) g_\lambda$ là một khai triển tiệm cận của $f_1 + f_2$ đến độ chính xác $g_\alpha$ (V, p. 215, prop. 5); và với mọi vô hướng $c$, $\sum_{\lambda \leq \alpha} a_\lambda c g_\lambda$ là một khai triển tiệm cận của $f_1 c$ đến độ chính xác $g_\alpha$. Suy ra rằng nếu một hàm thừa nhận một khai triển tiệm cận đến độ chính xác $g_\alpha$ thì khai triển này là *duy nhất*: chỉ cần thấy rằng hàm 0 không thừa nhận một khai triển tiệm cận với độ chính xác $g_\alpha$ có các hệ số $\neq 0$. Thật vậy, nếu $0 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$, và nếu $\gamma$ là nhỏ nhất trong các chỉ số $\lambda \leq \alpha$ sao cho $a_\lambda \neq 0$, thì sẽ có $a_\gamma g_\gamma = - \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda - r_\alpha \ll g_\gamma$, điều này vô lý.

Nói rằng một hàm $f$ thừa nhận một khai triển tiệm cận đến độ chính xác $g_\alpha$, mà mọi hệ số đều bằng *không*, là tương đương với nói rằng $f \ll g_\alpha$. Nếu $f$ thừa nhận một khai triển tiệm cận $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$ đến độ chính xác $g_\alpha$ mà các hệ số không phải tất cả đều bằng không, và nếu $\gamma$ là nhỏ nhất trong các chỉ số $\lambda$ sao cho $a_\lambda \neq 0$, thì $a_\gamma g_\gamma$ là *phần chính* của $f$ đối với thang $\mathcal{E}$, vì ta có $f - a_\gamma g_\gamma = \sum_{\gamma < \lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha \ll g_\gamma$; tương tự, nếu $\mu \leq \alpha$ là một chỉ số sao cho $a_\mu \neq 0$, thì $a_\mu g_\mu$ là phần chính của $f - \sum_{\lambda < \mu} a_\lambda g_\lambda$.

Những khai triển tiệm cận quan trọng nhất trong các ứng dụng là những khai triển đối với thang của các $x^{-n}$ (tương ứng của các $z^{-n}$), trong đó $n$ là một số nguyên dương hoặc âm, khi $x$ tiến tới $+\infty$ hoặc $-\infty$ (tương ứng khi số phức $z$ tiến tới $\infty$), hoặc đối với thang của các $(x - c)^n$ (tương ứng $(z - c)^n$) khi số thực $x$ tiến tới $c$ từ phải hoặc từ trái (tương ứng khi số phức $z$ tiến tới $c$). Ta đã thấy ở I, p. 21 rằng mọi hàm vectơ của biến thực $x$ khả vi $k$ lần tại một điểm $c \in \mathbf{R}$ đều chấp nhận một khai triển Taylor cấp $k$ tại điểm này, nghĩa là, một khai triển tiệm cận với độ chính xác $(x - c)^k$ đối với thang của các $(x - c)^n$.

### 3. TỔNG VÀ TÍCH CỦA CÁC KHAI TRIỂN TIỆM CẬN

Nếu $f_1, f_2$ có các khai triển tiệm cận với độ chính xác $g_\alpha$ và $g_\beta$ tương ứng, đối với một thang so sánh $\mathcal{E}$, thì suy ra được các khai triển với độ chính xác $g_{\min(\alpha, \beta)}$ bằng cách *cắt ngắn* hai khai triển đó đến độ chính xác này; ta đã thấy ở V, p. 222 cách thu được một khai triển tiệm cận của $f_1 + f_2$ với độ chính xác $g_{\min(\alpha, \beta)}$.

Cho $V_1, V_2$ và $V$ là ba không gian định chuẩn trên trường $K$, và gọi $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}. \mathbf{y}]$ là một *ánh xạ song tuyến tính liên tục* từ $V_1 \times V_2$ vào $V$; hơn nữa, trong phần còn lại của tiết này, ta giả sử rằng thang $\mathcal{E}$ được chọn sao cho *tích* của hai hàm bất kỳ trong $\mathcal{E}$ lại vẫn thuộc $\mathcal{E}$ (điều này đúng với mọi thang so sánh được cho làm ví dụ (trong V, p. 220)).

Bây giờ, cho $f_1, f_2$ là hai hàm thuộc $\mathcal{H}(\mathfrak{F}, V_1)$ và $\mathcal{H}(\mathfrak{F}, V_2)$ tương ứng, có các khai triển tiệm cận $f_1 = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$ và $f_2 = \sum_{\mu \leq \beta} b_\mu g_\mu + r_\beta$ với độ chính xác tương ứng là $g_\alpha$ và $g_\beta$, đối với thang $\mathcal{E}$. Giả sử thêm rằng các $a_\lambda$ không đồng thời đều bằng không và các $b_\mu$ cũng không đồng thời đều bằng không, và gọi $a_\gamma g_\gamma$ và $b_\delta g_\delta$ là các phần chính của $f_1$ và $f_2$. Theo giả thiết, có thể viết $g_\gamma g_\beta = g_\rho$ và $g_\delta g_\alpha = g_\sigma$; ta sẽ chỉ ra rằng tổng $\sum [\mathbf{a}_\lambda . \mathbf{b}_\mu] g_\lambda g_\mu$ lấy trên mọi cặp $(\lambda, \mu)$ sao cho $g_{\min(\rho, \sigma)} \ll g_\lambda g_\mu$, là một *khai triển tiệm cận của* $[f_1.f_2]$ *với độ chính xác* $g_{\min(\rho, \sigma)}$. Bây giờ hiệu giữa $[f_1.f_2]$ và tổng này là tổng của một số hữu hạn số hạng, mỗi số hạng hoặc có dạng $[\mathbf{a}_\lambda . \mathbf{b}_\mu] g_\lambda g_\mu$ với $g_\lambda g_\mu \ll g_{\min(\rho, \sigma)}$, hoặc có dạng $[\mathbf{a}_\lambda . \mathbf{r}_\beta] g_\lambda$ trong đó $\lambda \geq \gamma$, hoặc có dạng $[\mathbf{r}_\alpha . \mathbf{b}_\mu] g_\mu$ trong đó $\mu \geq \delta$; nhưng vì $[\mathbf{x}. \mathbf{y}]$ là liên tục, suy ra từ (V, p. 213, mệnh đề 3 and V, p. 215, mệnh đề 6) rằng $[\mathbf{a}_\lambda . \mathbf{r}_\beta] g_\lambda \preccurlyeq \mathbf{r}_\beta g_\lambda \ll g_\beta g_\gamma = g_\rho$ đối với $\lambda \geq \gamma$, và tương tự $[\mathbf{r}_\alpha . \mathbf{b}_\mu] g_\mu \preccurlyeq \mathbf{r}_\alpha g_\mu \ll g_\alpha g_\delta = g_\sigma$ đối với $\mu \geq \delta$, do đó mệnh đề (V, p. 215, mệnh đề 5).

Nếu mọi $\mathbf{a}_\lambda$ đều bằng không thì ta có $[f_1.f_2] \ll g_\alpha g_\delta$: nói cách khác, ta có một khai triển tiệm cận của $[f_1.f_2]$ với các hạng bằng không, chính xác đến $g_\alpha g_\delta$; tương tự, nếu mọi $\mathbf{a}_\lambda$ và $\mathbf{b}_\mu$ đều bằng không thì ta có một khai triển tiệm cận của $[f_1.f_2]$ với các hạng bằng không chính xác đến $g_\alpha g_\beta$.

Chúng ta sẽ áp dụng kết quả trên chủ yếu cho trường hợp V là một *đại số định chuẩn* trên K và hàm song tuyến tính $[\mathbf{x}. \mathbf{y}]$ là tích xy trong đại số này; những trường hợp quan trọng nhất là khi V bằng $\mathbf{R}$ hoặc $\mathbf{C}$.

Đặc biệt, nếu $f_i$ ($1 \leq i \leq n$) là n hàm trong $\mathcal{H}(\mathfrak{F}, K)$ mà mỗi hàm đều chấp nhận một khai triển tiệm cận đối với $\mathcal{E}$, thì ta có thể thu được một khai triển tiệm cận đối với $\mathcal{E}$ cho mọi *đa thức* $\sum_{(v_i)} \mathbf{a}_{v_1 v_2} v_n f_1^{v_1} \ldots f_n^{v_n}$ theo các $f_i$ với hệ số trong một không gian định chuẩn V; hơn nữa, các quy tắc trước cho phép xác định độ chính xác của khai triển thu được, nếu biết độ chính xác của các khai triển của các hàm $f_i$.

### 4. HỢP THÀNH CÁC KHAI TRIỂN TIỆM CẬN

Cho $f$ là một hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$ (resp. $\mathcal{H}(\mathfrak{F}, \mathbf{C})$), thừa nhận một khai triển tiệm cận đến độ chính xác $g_\alpha$ đối với một thang $\mathcal{E}$, và *có giới hạn* 0 dọc theo bộ lọc có cơ sở $\widetilde{\mathfrak{F}}$. Mặt khác, cho $\mathbf{h}$ là một hàm nhận giá trị trong một không gian chuẩn V trên $\mathbf{R}$ (resp. $\mathbf{C}$), được xác định trên một lân cận của điểm 0 trong $\mathbf{R}$ (resp. $\mathbf{C}$), và *khả vi n lần* trên lân cận này; khi đó

$$
\mathbf{h}(t) = c_0 + c_1 t + \cdots + c_n t^n + o(t^n)
$$

trên lân cận này (I, p. 21), do đó, trên một tập hợp thích hợp trong $\widetilde{\mathfrak{F}}$

$$
\mathbf{h} \circ f = c_0 + c_1 f + \cdots + c_n f^n + o(f^n).
$$

Ta đã thấy, trong số 3, cách lập một khai triển tiệm cận của $c_0 + c_1 f + \cdots + c_n f^n$ đến cấp chính xác $g_\rho$ được xác định bởi cấp chính xác của khai triển của $f$; hơn nữa, giả sử rằng các hệ số của khai triển tiệm cận của $f$ không đồng thời bằng không, và rằng $a_\gamma g_\gamma$ là phần chính của $f$, và đặt $g_\sigma = g_\gamma^n$; nếu $\sigma < \rho$ thì ta sẽ có một khai triển của $\mathbf{h} \circ f$ đến cấp chính xác $g_\sigma$ khi giới hạn khai triển của $\sum_{k=0}^n c_k f^k$ đến cấp chính xác này; nếu, trái lại, $\rho \leq \sigma$, thì khai triển của $\sum_{k=0}^n c_k f^k$ cũng là một khai triển của $\mathbf{h} \circ f$ đến cấp chính xác $g_\rho$.

Nếu mọi số hạng của khai triển tiệm cận của $f$ đều bằng không, và nếu $g_\alpha \ll 1$, thì $f \ll g_\alpha$ và do đó $f^k \ll g_\alpha^k \ll g_\alpha$ với mọi số nguyên $k > 0$; nếu $c_m$ là hệ số đầu tiên có chỉ số $> 0$ mà khác không (giả sử rằng các $c_k$ với chỉ số $k > 0$ không đồng thời đều bằng 0), thì $c_0$ là một khai triển tiệm cận của $h \circ f$ với độ chính xác $g_\alpha^m$.

Trong phần còn lại của tiết diện này, chúng ta sẽ tự giới hạn vào trường hợp các hàm trong $\mathcal{E}$ nhận giá trị thực và là dương ngặt trên một tập hợp thuộc $\mathfrak{F}$, và chúng ta sẽ chỉ xét các khai triển tiệm cận của các hàm trong $\mathcal{H}(\mathfrak{F}, \mathbf{R})$. Trước hết, giả sử rằng với mọi hàm $g \in \mathcal{E}$ và mọi số thực $\nu$, $g^\nu$ lại thuộc $\mathcal{E}$: điều kiện này được thỏa mãn, chẳng hạn, bởi thang của các $x^\alpha$ hoặc bởi thang của các $x^\alpha |\log x|^\beta$ ($\alpha$ và $\beta$ là các số thực tùy ý) trên một lân cận của $+\infty$ hoặc một lân cận của 0 trong $\mathbf{R}$. Tính chất này kéo theo rằng thương của hai hàm trong $\mathcal{E}$ lại thuộc $\mathcal{E}$. Như vậy, từ một khai triển tiệm cận tương đối với $\mathcal{E}$ của một hàm $f \in \mathcal{H}(\mathfrak{F}, \mathbf{R})$, đến cấp chính xác $g_\alpha$, người ta có thể suy ra một khai triển của $|f|^\nu$ với mọi số thực $\nu$. Ta hãy tự giới hạn vào trường hợp các hệ số của khai triển của $f$ không đồng thời bằng không, và ký hiệu $a_\gamma g_\gamma$ là phần chính của $f$; khi đó có thể viết $|f|^\nu = |a_\gamma|^\nu g_\gamma^\nu (1 + h)^\nu$, với
$$
h = \sum_{\gamma < \lambda \leq \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma} + o \left( \frac{g_\alpha}{g_\gamma} \right).
$$
Dưới các giả thiết của chúng ta, $\sum_{\gamma < \lambda \leq \alpha} \frac{a_\lambda}{a_\gamma} \frac{g_\lambda}{g_\gamma}$ là một khai triển tiệm cận của $h$, đến cấp chính xác $g_\alpha / g_\gamma$; vì $h$ tiến tới 0 dọc theo $\mathfrak{F}$ nên phương pháp được mô tả ở trên cho một khai triển tiệm cận của $(1 + h)^\nu$, rồi do đó một khai triển của $|f|^\nu$ sau khi nhân với $|a_\gamma|^\nu g_\gamma^\nu$.

Với cùng các giả thiết trên $f$ ta có thể viết
$$
\log |f| = \log |a_\gamma g_\gamma| + \log (1 + h)
$$
và $\log (1 + h)$ có thể được khai triển, như đã nói ở trên, vì hàm $\log (1 + t)$ khả vi vô hạn trên một lân cận của 0; hơn nữa, nếu $\log g_\gamma$ thừa nhận một khai triển tiệm cận đối với $\mathcal{E}$, hoặc đối với một thang $\mathcal{E}_1 \supset \mathcal{E}$, thì bằng cách cộng hai khai triển tiệm cận ấy, ta thu được một khai triển tiệm cận của $\log |f|$.

#### Ví dụ {#fvr-v-s2-n4-exa-1 .statement}

Ta có $(1 + x)^{1/x} = \exp \left( \frac{1}{x} \log (1 + x) \right)$: khi $x$ tiến tới $+\infty$ thì $\log (1 + x) = \log x + \log \left( 1 + \frac{1}{x} \right)$, do đó khai triển tiệm cận của $\frac{1}{x} \log (1 + x)$ theo thang các $x^\alpha (\log x)^\beta$ là:
$$
\frac{1}{x} \log (1 + x) = \frac{\log x}{x} + \frac{1}{x^2} - \frac{1}{2x^3} + o_1 \left( \frac{1}{x^3} \right).
$$
Từ khai triển này, và từ khai triển Taylor
$$
e^u = 1 + u + \frac{u^2}{2} + \frac{u^3}{6} + o(u^3)
$$

trong một lân cận của $u = 0$, ta suy ra khai triển tiệm cận

$$
(1 + x)^{1/x} = 1 + \frac{\log x}{x} + \frac{1}{2} \frac{(\log x)^2}{x^2} + \frac{1}{x^2}
+ \frac{1}{6} \frac{(\log x)^3}{x^3} + \frac{\log x}{x^3} - \frac{1}{2x^3} + o_2 \left( \frac{1}{x^3} \right)
$$

theo thang $x^\alpha (\log x)^\beta$ bằng các phương pháp đã giải thích ở trên.

Giữ nguyên các giả thiết và ký hiệu, khai triển tiệm cận của $e^f$ không đặt ra vấn đề mới nào ngoại trừ khi $f \gg 1$; khi đó phải phân biệt hai trường hợp, tùy theo $g_\alpha \gg 1$ hay $g_\alpha \ll 1$. Trong trường hợp thứ nhất, việc cho một khai triển của $f$ không cho phép thu được một phần chính của $e^f$ đối với $\mathcal{E}$, vì nói chung ta không biết số dư $r_\alpha$ có tiến tới 0 hay không, tức là liệu $e^{r_\alpha}$ có tiến tới 1 hay không. Trái lại, nếu $g_\alpha \ll 1$ thì $r_\sigma \ll 1$ và do đó $e^f \sim \exp \left( \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \right)$. Có thể làm chính xác hơn kết quả này: gọi $a_\gamma g_\gamma$ là phần chính của $f$ và gọi $\delta$ là chỉ số (sao cho $\gamma < \delta \leq \alpha$) mà với nó $g_\delta = 1$; đặt $f_1 = \sum_{\lambda \leq \delta} a_\lambda g_\lambda$, $f_2 = \sum_{\delta < \lambda \leq \alpha} a_\lambda g_\lambda + r_\alpha$; ta có $f = f_1 + f_2$, nên $e^f = e^{f_1} e^{f_2}$, và phương pháp tổng quát đã được giải thích ở đầu tiểu mục này cho phép lập một khai triển tiệm cận của $e^{f_2}$ (xuất phát từ khai triển Taylor của $e^t$ tại điểm $t = 0$). Khi đó ta sẽ có một khai triển tiệm cận của $e^f$ nếu $e^{f_1} = \prod_{\lambda \leq \delta} \exp(a_\lambda g_\lambda)$ thuộc $\mathcal{E}$, hoặc thuộc một thang $\mathcal{E}_1$ chứa $\mathcal{E}$.

#### Ví dụ {#fvr-v-s2-n4-exa-2 .statement}

Ta có $x^{1/1} = \exp \left( \log x \cdot \exp \left( \frac{1}{x} \log x \right) \right)$; khi $x$ tiến tới $+\infty$ thì $\log x \ll x$, do đó khai triển tiệm cận của $\log x \cdot \exp \left( \frac{1}{x} \log x \right)$ đối với thang $x^\alpha (\log x)^\beta$ là:

$$
\log x \cdot \exp \left( \frac{1}{x} \log x \right) = \log x + \frac{(\log x)^2}{x} + \frac{1}{2} \frac{(\log x)^3}{x^2} + o \left( \frac{(\log x)^3}{x^2} \right).
$$

Mọi hạng của khai triển này, bắt đầu từ hạng thứ hai, đều tiến tới 0; từ khai triển này và từ khai triển Taylor $e^u = 1 + u + u^2/2 + o(u^2)$ trên một lân cận của $u = 0$ suy ra

$$
x^{1/1} = 1 + (\log x)^2 + \frac{1}{2} \frac{(\log x)^4}{x} + \frac{1}{2} \frac{(\log x)^3}{x} + o \left( \frac{(\log x)^3}{x} \right).
$$

### 5. KHAI TRIỂN TIỆM CẬN VỚI HỆ SỐ BIẾN THIÊN

Có thể tổng quát hóa khái niệm phần chính, cũng như khái niệm khai triển tiệm cận, theo cách sau. Cho $\mathcal{E}$ là một thang so sánh gồm các hàm thực (resp. phức) sao cho, đối với mỗi hàm trong số đó, tồn tại một tập hợp trong $\mathfrak{F}$ trên đó hàm *không triệt tiêu tại bất kỳ điểm nào*. Hơn nữa, cho $C$ là một tập hợp các hàm trong $\mathcal{H}(\mathfrak{F}, V)$ thỏa mãn ba điều kiện sau:

(CO₁) Với mọi hàm $a \in C$ ta có $a \preccurlyeq 1$.
(CO₂) Quan hệ $a \ll 1$ đối với một hàm $a \in C$ suy ra $a = 0$.
(CO₃) $C$ là một không gian vectơ trên $\mathbf{R}$ (tương ứng $\mathbf{C}$).

Bây giờ, cho $f$ là một hàm bất kỳ trong $\mathcal{H}(\mathfrak{F}, V)$; nếu tồn tại một hàm $g \in \mathcal{E}$ và một hàm khác không $a \in C$ sao cho $f - ag \ll g$ thì ta sẽ nói rằng $ag$ là một phần chính của $f$, đối với thang so sánh $\mathcal{E}$ và miền hệ số $C$. Nếu một phần chính như vậy tồn tại, thì nó là duy nhất: thật vậy, giả sử có hai phần chính $a_1 g_1$ và $a_2 g_2$; không thể có $g_1 \ll g_2$ vì từ (CO₁) người ta có thể suy ra rằng $a_1 g_1 \ll g_2$ và $f - a_1 g_1 \ll g_1 \ll g_2$, do đó $f \ll g_2$; nhưng khi đó cũng sẽ có $a_2 g_2 \ll g_2$ và do đó $a_2 \ll 1$ mâu thuẫn với giả thiết $a_2 \neq 0$ và (CO₂). Vậy phải có $g_1 = g_2$; từ các hệ thức $f - a_1 g_1 \ll g_1, f - a_2 g_1 \ll g_1$ suy ra rằng $(a_2 - a_1)g_1 \ll g_1$ do đó $a_2 - a_1 \ll 1$, và do đó $a_2 = a_1$, theo (CO₂) và (CO₃).

#### Ví dụ {#fvr-v-s2-n5-exa-1 .statement}

Khi $x$ thực tiến tới $+\infty$ thì các hàm tuần hoàn bị chặn trên $\mathbf{R}$, có cùng chu kỳ $\tau$, thỏa mãn các điều kiện (CO₁), (CO₂) và (CO₃): nếu $\lim_{x \to +\infty} a(x) = 0$ thì với mọi $\varepsilon > 0$ tồn tại một $x_0$ sao cho $|a(x)| \leq \varepsilon$ với mọi $x \geq x_0$; suy ra $|a(x)| \leq \varepsilon$ cũng đúng với $0 \leq x \leq \tau$, vì tồn tại một số nguyên $n$ sao cho $x + n\tau \geq x_0$, và sao cho $a(x) = a(x + n\tau)$; vì $\varepsilon$ là tùy ý nên ta có $a(x) = 0$ trên $[0, \tau]$, do đó ở mọi nơi.

Với ký hiệu của V, p. 222, ta sẽ nói rằng $\sum_{\lambda \leq \alpha} a_\lambda g_\lambda$, trong đó các $a_\lambda$ thuộc $C$ và tất cả trừ một số hữu hạn trong chúng đều bằng không, là một khai triển tiệm cận của $f$ với các hệ số trong $C$, chính xác đến $g_\alpha$, nếu $f - \sum_{\lambda \leq \alpha} a_\lambda g_\lambda \ll g_\alpha$; đối với mọi chỉ số $\mu$ sao cho $a_\mu \neq 0$ thì $a_\mu g_\mu$ là phần chính của $f - \sum_{\lambda < \mu} a_\lambda g_\lambda$, đối với $\mathcal{E}$ và $C'$, điều này chứng minh tính duy nhất của khai triển tiệm cận của $f$ (chính xác đến $g_\alpha$) khi nó tồn tại.

Các phương pháp đã cho trong n 3 (V, p. 223) để lập một khai triển tiệm cận của $f_1 + f_2$ hoặc của $[f_1 . f_2]$, xuất phát từ những khai triển tiệm cận đã biết của $f_1$ và $f_2$, lại cũng có thể được áp dụng cho các khai triển với hệ số biến, miễn là các $[a_\lambda . b_\mu]$ thuộc miền hệ số $C$ tương ứng với không gian định chuẩn $V$ hoặc chấp nhận một khai triển tiệm cận với các hệ số trong $C$.
