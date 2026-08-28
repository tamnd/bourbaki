---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 4
section_title: Convolution of measures and functions
lang: vi
source: int-vii-ix
book_pages: INT VIII.24-INT VIII.45, INT VIII.65-INT VIII.73
pdf_pages: 0124-0145, 0165-0173
extraction: ocr
subsections:
    - "no": 1
      title: Convolution of a measure and a function
      page: 24
      pdf_page: 124
    - "no": 2
      title: Examples of convolvable measures and functions
      page: 28
      pdf_page: 128
    - "no": 3
      title: Convolution and transposition
      page: 34
      pdf_page: 134
    - "no": 4
      title: Convolution of a measure and a function on a group
      page: 37
      pdf_page: 137
    - "no": 5
      title: Convolution of functions on a group
      page: 38
      pdf_page: 138
    - "no": 6
      title: Applications
      page: 42
      pdf_page: 142
    - "no": 7
      title: Regularization
      page: 44
      pdf_page: 144
statements: 38
exercises: 28
content_sha256: aaddfaf1028a4f72ac725f6e2e2f8e41125dabb15f4c66690e545c9b6a2dd6f4
translated_from: content/en/int/VIII/04_s4_convolution_of_measures_and_functions.md
source_content_sha256: 4bdfd45d074b8fb1fc45bbdbf705e28e2b73e20a27681320842f9ce58bd4d2d5
translation_model: gpt-5.4, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-22bd618f
glossary_version: 34
glossary_terms_sha256: 32f48de064fb22f42346f49d5c701d11be08c5aa8a570486ee8e1440dfd03d52
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. TÍCH CHẬP CỦA CÁC ĐỘ ĐO VÀ CÁC HÀM

### 1. Tích chập của một độ đo và một hàm

Cho X là một không gian địa phương compact, trên đó một nhóm địa phương compact G tác động liên tục ở bên trái. Cho $\beta$ là một độ đo dương trên X, tựa-bất biến dưới G. Cho $\chi$ là một hàm $> 0$ trên $G \times X$, đo được đối với mọi độ đo trên $G \times X$, và sao cho, với mọi $s \in G$, $\chi(s^{-1}, \cdot)$ là một mật độ của $\gamma(s)\beta$ đối với $\beta$:

$$
(1) \qquad \gamma(s)\beta = \chi(s^{-1}, \cdot) \cdot \beta,
$$

điều này, với các quy ước của Ch. VII, §1, No. 1, có thể viết:

$$
(1') \qquad d\beta(sx) = \chi(s, x) \, d\beta(x).
$$

Các dữ kiện này sẽ được giữ cố định trong Nos. 1, 2, 3 (ngoại lệ là Nhận xét 2 của No. 2).

Nhắc lại (§2, No. 5) rằng nếu $\chi$ liên tục và $\beta$ có giá là $X$, thì $\chi$ là một nhân tử.

Cho $f$ là một hàm phức địa phương $\beta$-khả tích trên $X$, và cho $\mu$ là một độ đo trên $G$. Với mọi $s \in G$, độ đo $\gamma(s)(f \cdot \beta)$ có cơ sở là $\beta$ vì $\beta$ là tựa-bất biến. Do đó, nếu $\mu$ và $f \cdot \beta$ chập được, thì $\mu * (f \cdot \beta)$ có cơ sở là $\beta$ (§3, No. 2, Prop. 10).

#### Định nghĩa 1 {#int-viii-s4-def-1 .statement}

*Nếu $\mu$ và $f \cdot \beta$ chập được, thì nói rằng $\mu$ và $f$ chập được đối với $\beta$. Mọi mật độ của $\mu * (f \cdot \beta)$ đối với $\beta$ được gọi là một tích chập của $\mu$ và $f$ đối với $\beta$ và được ký hiệu là $\mu *_{\beta} f$.*

Người ta bỏ $\beta$ đi khi không thể có sự lẫn lộn nào. Tích chập của nhiều độ đo trên $G$ và một hàm trên $X$ được định nghĩa một cách tương tự.

Các tích chập khác nhau của $\mu$ và $f$ bằng nhau địa phương $\beta$-hầu khắp nơi. Nếu $\beta$ có giá là $X$ và nếu tồn tại một tích chập của $\mu$ và $f$ là liên tục, thì tích chập này được xác định duy nhất; khi đó nó được gọi là *tích chập* của $\mu$ và $f$ đối với $\beta$.

Cho $s \in G$ và cho $f$ là một hàm phức địa phương $\beta$-khả tích trên $X$. Khi đó $\varepsilon_s$ và $f$ chập được, và

$$
\varepsilon_s * (f \cdot \beta) = \gamma(s)(f \cdot \beta) = (\gamma(s)f) \cdot (\gamma(s)\beta) = (\gamma(s)f) \cdot \chi(s^{-1}, \cdot) \cdot \beta,
$$

do đó

$$
(2) \qquad (\varepsilon_s * f)(x) = \chi(s^{-1}, x) f(s^{-1}x) = (\gamma_{\chi}(s)f)(x)
$$

địa phương $\beta$-hầu khắp mọi nơi.

#### Bổ đề 1 {#int-viii-s4-lem-1 .statement}

*Cho $\mu$ là một độ đo trên $G$. Khi đó $\chi$ là địa phương $(\mu \otimes \beta)$-khả tích, và ảnh của $\mu \otimes \beta$ dưới phép đồng phôi $(s, x) \mapsto (s, s^{-1}x)$ từ $G \times X$ lên $G \times X$ là $\chi \cdot (\mu \otimes \beta)$.*

Ta có thể giả sử rằng $\mu \geqslant 0$. Cho $F \in \mathcal{K}_+(\mathbf{G} \times \mathbf{X})$. Khi đó
$$
\iint F(s, s^{-1}x) d\mu(s) d\beta(x) = \int d\mu(s) \int F(s, s^{-1}x) d\beta(x)
$$
$$
= \int d\mu(s) \int F(s, x) d(\gamma(s^{-1})\beta)(x) = \int d\mu(s) \int F(s, x)\chi(s, x) d\beta(x).
$$

Bây giờ, hàm $(s, x) \mapsto F(s, x)\chi(s, x)$ có giá compact và là $(\mu \otimes \beta)$-đo được. Theo Ch. V, §8, No. 3, Prop. 7, đẳng thức trên chứng minh rằng hàm này là $(\mu \otimes \beta)$-khả tích và rằng
$$
\iint F(s, s^{-1}x) d\mu(s) d\beta(x) = \iint F(s, x)\chi(s, x) d\mu(s) d\beta(x).
$$
Điều này đồng thời chứng minh cả hai khẳng định của Bổ đề 1.

#### Mệnh đề 1 {#int-viii-s4-prop-1 .statement}

*Cho $\mu$ là một độ đo trên $\mathbf{G}$, $f$ là một hàm phức địa phương $\beta$-khả tích trên $\mathbf{X}$. Giả sử rằng hàm $s \mapsto f(s^{-1}x)\chi(s^{-1}, x)$ là khả tích thiết yếu theo $\mu$ trừ ra trên một tập các giá trị của $x$ không đáng kể địa phương đối với $\beta$, và rằng hàm $x \mapsto \int |f(s^{-1}x)|\chi(s^{-1}, x) d|\mu|(s)$, được xác định địa phương hầu khắp nơi đối với $\beta$, là địa phương $\beta$-khả tích. Khi đó $\mu$ và $f$ chập được với nhau.*

Ta có thể giả sử rằng $f \geqslant 0$ và $\mu \geqslant 0$. Cho $h \in \mathcal{K}_+(\mathbf{X})$. Ta phải chứng minh rằng hàm $(s, x) \mapsto h(sx)$ là khả tích thiết yếu đối với $\mu \otimes (f \cdot \beta) = (1 \otimes f) \cdot (\mu \otimes \beta)$ (Ch. V, §8, No. 5, Prop. 10), tức là $\iint^\bullet h(sx)f(x)\varphi_K(s) d\mu(s) d\beta(x) < +\infty$ (Ch. V, §5, No. 3, Prop. 3); rõ ràng chỉ cần chứng minh rằng tồn tại một $a > 0$ sao cho với mọi tập con compact $K$ của $\mathbf{G}$,
$$
\iint^\bullet h(sx)f(x)\varphi_K(s) d\mu(s) d\beta(x) \leqslant a.
$$
Theo Bổ đề 1,
$$
\iint^\bullet h(sx)f(x)\varphi_K(s) d\mu(s) d\beta(x)
$$
$$
= \iint^* h(x)f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x) d\mu(s) d\beta(x).
$$
Bây giờ, hàm $(s, x) \mapsto h(x)f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x)$ là $(\mu \otimes \beta)$-đo được (Bổ đề 1) và có giá compact. Do đó biểu thức trên bằng (Ch. V, §8, No. 3, Prop. 7)
$$
\int^* h(x) d\beta(x) \int^* f(s^{-1}x)\varphi_K(s)\chi(s^{-1}, x) d\mu(s)
$$
$$
\leqslant (\sup h) \int^* d\beta(x) \int^* f(s^{-1}x)\chi(s^{-1}, x) d\mu(s),
$$

trong đó S ký hiệu giá của h. Do đó suy ra mệnh đề.

#### Mệnh đề 2 {#int-viii-s4-prop-2 .statement}

— Cho $\mu$ là một độ đo trên G, f là một hàm phức địa phương $\beta$-khả tích trên X. Giả sử rằng một trong các điều kiện sau được thỏa mãn:
(i) f và $\chi$ liên tục;
(ii) G tác động một cách đúng trên X và f bằng không trên phần bù của một hợp đếm được các tập compact;
(iii) $\mu$ được mang bởi một hợp đếm được các tập compact.
Nếu $\mu$ và f chập được với nhau, thì hàm $s \mapsto f(s^{-1}x)\chi(s^{-1}, x)$ là khả tích thiết yếu theo $\mu$ trừ ra trên một tập các giá trị của x không đáng kể địa phương đối với $\beta$, và ta có, địa phương $\beta$-hầu khắp mọi nơi,

$$
(\mu *_{\beta} f)(x) = \int_G f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) = \int_G (\gamma_{\chi}(s)f)(x)\, d\mu(s).
$$

Cho $h \in \mathcal{H}(X)$. Vì $\mu$ và f có thể lấy tích chập, hàm $(s, x) \mapsto h(sx)f(x)$ về bản chất là $(\mu \otimes \beta)$-khả tích. Theo Bổ đề 1, hàm $(s, x) \mapsto h(x)f(s^{-1}x)\chi(s^{-1}, x)$ về bản chất là $(\mu \otimes \beta)$-khả tích. Theo giả thiết (i) hoặc (ii) của mệnh đề, do đó suy ra hàm này là $(\mu \otimes \beta)$-khả tích; vì, trong trường hợp thứ nhất, nó liên tục và ta áp dụng Mệnh đề 3 của Ch. V, §1, No. 1, còn trong trường hợp thứ hai, nó bằng không ngoài một hợp đếm được các tập compact, và ta áp dụng Mệnh đề 7, 2) của No. 2, loc. cit. Theo định lý Lebesgue–Fubini,

$$
\iint h(sx)\, d\mu(s)\, d(f \cdot \beta)(x) = \iint h(x)f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s)\, d\beta(x)
= \int h(x)\, d\beta(x) \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s),
$$

hàm $x \mapsto g(x) = \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s)$ hơn nữa khả tích địa phương theo $\beta$. Do đó ta thấy rằng

$$
\langle h, \mu * (f \cdot \beta) \rangle = \langle h, g \cdot \beta \rangle,
$$

do đó $g = \mu *_{\beta} f$.

Bây giờ giả sử rằng $\mu$ được mang bởi hợp S của một dãy các tập compact. Hàm

$$
(s, x) \mapsto h(x)f(s^{-1}x)\chi(s^{-1}, x)\varphi_S(s)
$$

về bản chất là $(\mu \otimes \beta)$-khả tích, và bằng không ngoài một hợp đếm được các tập compact, do đó là $(\mu \otimes \beta)$-khả tích. Vì $\mu = \varphi_S \cdot \mu$, lập luận kết thúc như trên.

#### Nhận xét {#int-viii-s4-n1-rem-1 .statement}

Giả thiết (iii) của Mệnh đề 2 đặc biệt được thỏa mãn khi $\mu$ bị chặn. Thật vậy, với mọi $n > 0$, khi đó tồn tại một tập con compact $K_n$ của $G$ sao cho
$$
|\mu|(G - K_n) \leq \frac{1}{n}
$$
(Ch. IV, §4, No. 7), và $\mu$ được mang bởi hợp của các $K_n$. Tổng quát hơn, cho $\rho$ là một hàm hữu hạn nửa liên tục dưới $> 0$ trên $G$ sao cho $\rho(st) \leq \rho(s)\rho(t)$; nếu $\mu \in \mathcal{M}^\rho$, thì giả thiết (iii) được thỏa mãn; vì $\rho \cdot \mu$ bị chặn, và $\mu$ được mang bởi cùng các tập con như $\rho \cdot \mu$, bởi vì, trên mỗi tập con compact của $G$, $\rho$ bị chặn dưới bởi một hằng số $> 0$.

### 2. Ví dụ về các độ đo và hàm có thể lấy tích chập

Trong Mệnh đề 3 và 4, $\mathcal{C}'(G)$ và $\mathcal{M}(G)$ được trang bị tôpô hội tụ compact trong $\mathcal{C}(G)$ và $\mathcal{K}(G)$, tương ứng.

#### Mệnh đề 3 {#int-viii-s4-prop-3 .statement}

— Giả sử $\chi$ liên tục. Cho $\mu \in \mathcal{C}'(G)$, $f \in \mathcal{C}(X)$. Khi đó:
(i) $\mu$ và $f$ có thể lấy tích chập đối với $\beta$.
(ii) Công thức (3) của No. 1 xác định, với mọi $x \in X$, một tích chập $\mu *_{\beta} f$ liên tục và chính là phần tử $\gamma_\chi(\mu)f$ được xác định bởi biểu diễn liên tục $\gamma_\chi$ của $G$ trong $\mathcal{C}(X)$; hơn nữa, ánh xạ $(\mu, f) \mapsto \mu *_{\beta} f$ là liên tục giả đối với các tập con đều liên tục của $\mathcal{C}'(G)$ và các tập compact của $\mathcal{C}(X)$.
(iii) Nếu thêm $f \in \mathcal{K}(X)$, thì tích $\mu *_{\beta} f$ ở (ii) thuộc $\mathcal{K}(X)$ và ánh xạ $(\mu, f) \mapsto \mu *_{\beta} f$ là liên tục giả đối với các tập con đều liên tục của $\mathcal{C}'(G)$ và các tập compact của $\mathcal{K}(X)$.

Ta biết rằng $\mu$ và $f$ là nhân chập được (§3, No. 2, Prop. 8 (i)). Mặt khác, với các ký hiệu của §2, ta có
$$
\gamma_\chi(\mu)f = \int (\gamma_\chi(s)f)d\mu(s) \in \mathcal{C}(X)
$$
vì $\mathcal{C}(X)$ là đầy đủ. Đặc biệt, với mọi $x \in X$,
$$
(\gamma_\chi(\mu)f)(x) = \int (\gamma_\chi(s)f)(x)\,d\mu(s).
$$
Điều này, kết hợp với Prop. 2 (i), và §2, No. 6, chứng minh (ii). Cuối cùng, nếu $f \in \mathcal{K}(X)$ thì $\mu * (f \cdot \beta)$ có giá đỡ compact (§3, No. 2, Prop. 9), do đó $\mu *_{\beta} f \in \mathcal{K}(X)$. Thật vậy, xét biểu diễn liên tục $U$ của $G$ trong phần hoàn thành $\mathcal{K}(X)^{\sim}$ thu được bằng cách mở rộng theo tính liên tục các toán tử liên tục $\gamma_\chi(s)$ trong $\mathcal{K}(X)$ (\S 2, No. 1, *Nhận xét 3*). Gọi $S$ là giá đỡ của $\mu$. Các hàm $\gamma_\chi(s)f$, với $s \in S$, có giá đỡ được chứa trong một tập compact cố định $K$. Tập hợp $\mathcal{K}(X, K)$ là một không gian con tuyến tính đầy đủ của $\mathcal{K}(X)$. Do đó $U(\mu)f \in \mathcal{K}(X)$. Như trước đây ta thấy rằng $U(\mu)f = \mu *^\beta f$, và (iii) lại suy ra từ \S 2, No. 6.

#### Mệnh đề 4 {#int-viii-s4-prop-4 .statement}

*Giả sử rằng G tác động đúng trong X và rằng $\chi$ là liên tục. Cho $\mu \in \mathcal{M}(G)$ và $f \in \mathcal{K}(X)$.*

(i) $\mu$ và $f$ là nhân chập được đối với $\beta$.

(ii) *Công thức (3) của No. 1 xác định với mọi $x \in X$ một tích nhân chập $\mu *^\beta f$ là liên tục.*

(iii) *Ánh xạ $(\mu, f) \mapsto \mu *^\beta f$ từ $\mathcal{M}(G) \times \mathcal{K}(X)$ vào $\mathcal{C}(X)$ là nửa liên tục đều đối với các tập con bị chặn của $\mathcal{M}(G)$ và các tập con compact của $\mathcal{K}(X)$ được chứa trong một không gian con $\mathcal{K}(X, L)$ nào đó (trong đó $L$ là một tập compact biến thiên của $X$).*

Ta biết rằng $\mu$ và $f$ là nhân chập được (\S 3, No. 2, Prop. 8 (ii)), và rõ ràng rằng các tích phân xuất hiện trong (3) tồn tại với mọi $x \in X$. Gọi $K$ và $L$ là hai tập con compact của $X$. Tồn tại một tập con compact $H$ của $G$ sao cho các quan hệ $x \in K$ và $s^{-1}x \in L$ kéo theo $s \in H$; lấy $\varphi \in \mathcal{K}_+(G)$ với $\varphi(s) = 1$ với $s \in H$. Khi đó, với $f \in \mathcal{K}(X, L)$ và $x \in K$,

$$
\int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) = \int f(s^{-1}x)\chi(s^{-1}, x)\varphi(s)\, d\mu(s)
= ((\varphi \cdot \mu) *^\beta f)(x).
$$

Do đó $\int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s)$ là một hàm liên tục của $x$ và xác định một tích chập $\mu *^\beta f \in \mathcal{C}(X)$. Hơn nữa, ánh xạ $\mu \mapsto \varphi \cdot \mu$ của $\mathcal{M}(G)$ vào $\mathcal{C}'(G)$ là liên tục đối với các tôpô hội tụ compact. Mệnh đề 3 (iii) do đó suy ra rằng ánh xạ $(\mu, f) \mapsto \mu *^\beta f$ của $\mathcal{M}(G) \times \mathcal{K}(X, L)$ vào $\mathcal{C}(X)$ là, với mọi tập con compact $L$ của $X$, nửa liên tục đối với các tập con compact của $\mathcal{K}(X, L)$. Đặc biệt, ánh xạ $(\mu, f) \mapsto \mu *^\beta f$ của $\mathcal{M}(G) \times \mathcal{K}(X)$ vào $\mathcal{C}(X)$ là liên tục riêng. Vì $\mathcal{K}(X)$ là không gian thùng, ánh xạ này là nửa liên tục đối với các tập con bị chặn của $\mathcal{M}(G)$ (TVS, III, \S 5, No. 3, Mệnh đề 6).

#### Nhận xét 1 {#int-viii-s4-n2-rem-1 .statement}

— Dưới các giả thiết của Mệnh đề 4, ánh xạ $\mu \mapsto \mu *^\beta f$ của $\mathcal{M}_+(G)$ vào $\mathcal{C}(X)$ là liên tục khi $\mathcal{M}_+(G)$ được trang bị tôpô *mơ hồ*, với mọi $f \in \mathcal{K}(X)$. Thật vậy, cho $K$ là một tập compact con của $X$, $S$ là giá đỡ (compact) của $f$; vì $G$ tác động đúng trong $X$, tập hợp các $s \in G$ sao cho tồn tại một $x \in K$ với $s^{-1}x \in S$ là một tập compact con $L$ của $G$ (GT, III, \S 4, No. 5, Th. 1). Cho $\varepsilon$ là một số $> 0$, $\varphi$ là một hàm trong $\mathcal{K}_+(G)$ bằng 1 trên tập compact $L$, $\mu_0$ là một phần tử của $\mathcal{M}_+(G)$; tập hợp $W_0$ các độ đo $\mu \in \mathcal{M}_+(G)$ sao cho
$$
\left| \int \varphi(s)\, d\mu(s) - \int \varphi(s)\, d\mu_0(s) \right| \leq \varepsilon
$$
là một lân cận của $\mu_0$ trong $\mathcal{M}_+(G)$. Mặt khác, hàm $(s, x) \mapsto f(s^{-1}x)\chi(s^{-1}, x)$ là liên tục đều trên $L \times K$, do đó tồn tại một số hữu hạn các điểm $x_i \in K$ ($1 \leq i \leq n$) sao cho với mọi $x \in K$, tồn tại một $i$ mà
$$
|f(s^{-1}x)\chi(s^{-1}, x) - f(s^{-1}x_i)\chi(s^{-1}, x_i)| \leq \varepsilon
$$
với mọi $s \in L$. Vì $\mu(L) \leq \int \varphi(s)\, d\mu_0(s) + \varepsilon$ với mọi $\mu \in W_0$, nên cũng có
$$
\begin{align*}
\left| \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) - \int f(s^{-1}x_i)\chi(s^{-1}, x_i)\, d\mu(s) \right| \\
\leq \varepsilon \left( \int \varphi(s)\, d\mu_0(s) + \varepsilon \right)
\end{align*}
$$
với mọi $x$ thỏa mãn bất đẳng thức trước đó và mọi $\mu \in W_0$. Bây giờ cho $W$ là lân cận của $\mu_0$ trong $\mathcal{M}_+(G)$ tạo bởi các độ đo $\mu \in W_0$ sao cho
$$
\left| \int f(s^{-1}x_i)\chi(s^{-1}, x_i)\, d\mu(s) - \int f(s^{-1}x_i)\chi(s^{-1}, x_i)\, d\mu_0(s) \right| \leq \varepsilon
$$
với $1 \leq i \leq n$. Rõ ràng là với mọi độ đo $\mu \in W$ và mọi $x \in K$,
$$
\begin{align*}
\left| \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu(s) - \int f(s^{-1}x)\chi(s^{-1}, x)\, d\mu_0(s) \right| \\
\leq \varepsilon \left( 2 \int \varphi(s)\, d\mu_0(s) + 2\varepsilon + 1 \right),
\end{align*}
$$
và vì $\varepsilon$ là tùy ý, điều này chứng minh mệnh đề của chúng ta.

#### Mệnh đề 5 {#int-viii-s4-prop-5 .statement}

*Giả sử $\chi$ là một nhân tử liên tục và mỗi hàm $\chi(s, \cdot)$ bị chặn.*
(i) *Hàm $s \mapsto \rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$ trên $G$ là nửa liên tục dưới $> 0$ và thỏa mãn $\rho(st) \leq \rho(s)\rho(t)$ với mọi $s, t$ thuộc $G$.*
(ii) *Cho $\mu \in \mathcal{M}^\rho(G)$ và $f \in L^\infty(X, \beta)$.*¹ *Khi đó $\mu$ và $f$ là nhân chập được với nhau và $\mu *^\beta f$ được cho địa phương hầu khắp nơi bởi công thức (3) của No. 1. Ta có $\mu *^\beta f \in L^\infty(X, \beta)$, và $\| \mu *^\beta f \|_\infty \leq \| \mu \|_\rho \| f \|_\infty$.*

¹Đối với một hàm $f$, biểu thức "$f \in L^\infty(X, \beta)$" là một sự lạm dụng ký hiệu, biểu thị rằng, tùy theo ngữ cảnh, ký hiệu $f$ được hiểu hoặc như một hàm hoặc như lớp tương đương của một hàm. Đặc biệt, ký hiệu $\mu *^\beta f$ có thể chỉ hoặc một hàm được xác định địa phương $\beta$-hầu khắp nơi, hoặc lớp tương đương của một hàm như vậy đối với quan hệ đẳng thức địa phương $\beta$-hầu khắp nơi.

(iii) *Nếu hơn nữa, $f \in \mathcal{C}^\infty(X)$ (resp. $\overline{\mathcal{K}(X)}$), thì công thức (3) của No. 1 xác định với mọi $x$ một tích nhân chập $\mu *^\beta f$ thuộc $\mathcal{C}^\infty(X)$ (resp. $\mathcal{K}(X)$).*

(iv) *Nếu $f \in \mathcal{K}(X)$, thì tích nhân chập $\mu *^\beta f$ được xác định bởi (3) chính là phần tử $\gamma_\chi(\mu)f$ được xác định bởi biểu diễn liên tục $\gamma_\chi$ của $G$ trong $\overline{\mathcal{K}(X)}$.

Đẳng thức $\chi(st, x) = \chi(s, tx)\chi(t, x)$ kéo theo ngay rằng $\rho(st) \leq \rho(s)\rho(t)$. Mặt khác, $\rho$ là nửa liên tục dưới, vì nó là bao trên của các hàm liên tục.

Cho $\mu \in \mathcal{M}^\rho(G)$. Theo Mệnh đề 1 của No. 1, $\mu$ và 1 là nhân chập được với nhau; Mệnh đề 2 (i) chỉ ra rằng $(|\mu| *^\beta 1)(x) \leq \int_G \rho(s) d|\mu|(s)$ địa phương $\beta$-hầu khắp nơi. Do đó, nếu $f$ là $\beta$-đo được và $|f| \leq 1$, thì $\mu$ và $f$ là nhân chập được với nhau và $N_\infty(\mu *^\beta f) \leq \int \rho(s) d|\mu|(s)$. Hơn nữa, $\mu *^\beta f$ được cho địa phương hầu khắp nơi bởi công thức (3) của No. 1, vì điều kiện (iii) của Mệnh đề 2 của No. 1 được thỏa mãn. Điều này suy ra (ii).

Giả sử $f$ liên tục và bị chặn bởi 1 về giá trị tuyệt đối. Rõ ràng là các tích phân xuất hiện trong (3) tồn tại với mọi $x \in X$. Ta chứng minh rằng chúng phụ thuộc liên tục vào $x$. Ta có thể giả sử $\mu \geq 0$. Cho $x_0 \in X$ và $\varepsilon > 0$. Cho $K$ là một tập con compact của $G$ sao cho $\int_{G - K} \rho(s) d\mu(s) \leq \varepsilon$. Tồn tại một lân cận $V$ của $x_0$ trong $X$ sao cho $x \in V$ kéo theo

$$
|f(s^{-1}x)\chi(s^{-1}, x) - f(s^{-1}x_0)\chi(s^{-1}, x_0)| \leq \varepsilon / \mu(K)
$$

với $s \in K$. Khi đó, với $x \in V$,

$$
\left| \int f(s^{-1}x)\chi(s^{-1}, x) d\mu(s) - \int f(s^{-1}x_0)\chi(s^{-1}, x_0) d\mu(s) \right|
$$
$$
\leq 2 \int_{G - K} \rho(s) d\mu(s) + \int_K \frac{\varepsilon}{\mu(K)} d\mu(s) \leq 3\varepsilon,
$$

do đó mệnh đề của chúng ta. Giả sử thêm rằng $f \in \overline{\mathcal{K}(X)}$. Cho $H$ là một tập con compact của $X$ sao cho $|f(y)| \leq \varepsilon$ với $y \notin H$. Cho $x \notin KH$. Khi đó $s^{-1}x \notin H$ với $s \in K$, do đó

$$
\left| \int_G f(s^{-1}x)\chi(s^{-1}, x) d\mu(s) \right| \leq \int_{G - K} \rho(s) d\mu(s) + \int_K \varepsilon \rho(s) d\mu(s)
$$
$$
\leq \varepsilon \left( 1 + \int_G \rho(s) d\mu(s) \right),
$$

điều này hoàn tất chứng minh của (iii).

Cuối cùng, nếu $f \in \mathcal{K}(X)$ thì, vì $\varepsilon_x \in \mathcal{M}^1(X)$ với mọi $x \in X$, ta có

$$
(\gamma_\chi(\mu)f)(x) = \int (\gamma_\chi(s)f)(x) d\mu(s),
$$

do đó $\gamma_\chi(\mu)f$ là tích chập $\mu *^\beta f$ được định nghĩa bởi (3).

#### Mệnh đề 6 {#int-viii-s4-prop-6 .statement}

*Giả sử $\chi$ là một nhân tử liên tục và mỗi hàm $\chi(s, \cdot)$ bị chặn. Đặt $\rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$. Cho $p$ và $q$ là hai số mũ liên hợp ($1 \leq p < +\infty$). Cho $\mu \in \mathcal{M}^{\rho^{1/q}}(G)$ và $f \in L^p(X, \beta)^2$ Khi đó:
(i) $\mu$ và $f$ là lấy tích chập được;
(ii) tích chập $\mu *^\beta f$ được cho địa phương $\beta$-hầu khắp nơi bởi công thức (3), và bằng địa phương $\beta$-hầu khắp nơi với một hàm $g \in L^p(X, \beta)$ sao cho $\|g\|_p \leq \|\mu\|_{\rho^{1/q}} \|f\|_p$;
(iii) $g$ bằng phần tử $\gamma_\chi(\mu)f$ được xác định bởi biểu diễn liên tục $\gamma_\chi$ của $G$ trong $L^p(X, \beta)$.*

Ta có
$$
\int^* \|\gamma_\chi(s)f\|_p d|\mu|(s) \leq \left( \int^* \rho(s)^{1/q} d|\mu|(s) \right) \|f\|_p < +\infty
$$
theo §2, No. 5, công thức (5). Mặt khác, ánh xạ $s \mapsto \gamma_\chi(s)f$ của $G$ vào $L^p(X, \beta)$ là liên tục (§2, No. 5, Mệnh đề 9). Do đó ánh xạ này là $\mu$-khả tích. Đặt
$$
g = \int_G (\gamma_\chi(s)f) d\mu(s) \in L^p(X, \beta).
$$
Ta có $\|g\|_p \leq (\int \rho^{1/q}(s) d|\mu|(s)) \|f\|_p$. Áp dụng các nhận xét trước cho $|f|$, ta thấy rằng ánh xạ $s \mapsto \varepsilon_s * |f|$ của $G$ vào $L^p(X, \beta)$ là $\mu$-khả tích, do đó, với mọi $h \in \mathcal{H}(X)$, ánh xạ $s \mapsto \langle h, \varepsilon_s * (|f| \cdot \beta) \rangle$ là $\mu$-khả tích. Mệnh đề 7 của §1, No. 5 khi đó chứng minh rằng $\mu$ và $f \cdot \beta$ là chập được. Hơn nữa,
$$
\int_X g(x)h(x) d\beta(x) = \int_G d\mu(s) \int_X (\gamma_\chi(s)f)(x)h(x) d\beta(x)
= \int_G \langle h, \varepsilon_s * (f \cdot \beta) \rangle d\mu(s),
$$
và tích phân cuối cùng này bằng $\langle h, \mu * (f \cdot \beta) \rangle$ theo Mệnh đề 7 của §1, No. 5. Vì vậy ta thấy rằng $g$ là một tích chập của $\mu$ và $f$. Tích chập này được cho địa phương $\beta$-hầu khắp nơi bởi (3), theo Mệnh đề 2 và *Nhận xét* theo sau nó.

2Đối với một hàm $f$, biểu thức " $f \in L^p(X, \beta)$ " là một lạm dụng ký hiệu, có nghĩa là, tùy theo ngữ cảnh, ký hiệu $f$ được hiểu hoặc là một hàm được xác định $\beta$-hầu khắp nơi, hoặc là lớp tương đương của một hàm như vậy đối với quan hệ đẳng thức $\beta$-hầu khắp nơi. Như vậy $f \in L^p$ có thể biểu diễn hoặc $f \in \mathcal{L}^p$ hoặc $\dot{f} \in L^p$.

Do một lạm dụng ký hiệu, thường một trong các hàm $g$ của mệnh đề được ký hiệu là $\mu *^\beta f$, điều này cho phép viết

$$
\| \mu *^\beta f \|_p \leq \| \mu \|_{\rho^{1/q}} \| f \|_p .
$$

Nếu $X$ là đếm được tại vô cùng, kiểu ký hiệu này hơn nữa hoàn toàn được biện minh.

#### Hệ quả {#int-viii-s4-n2-cor-1 .statement}

*Dưới các giả thiết của Mệnh đề 6, ánh xạ* $(\mu, f) \mapsto \mu *^\beta f$ *xác định trên* $L^p(X, \beta)$ *cấu trúc của một môđun trái trên* $\mathcal{M}^{\rho^{1/q}}(G)$ $(1 \leq p \leq +\infty)$.

Điều này suy ra từ các Mệnh đề 5 và 6 và tính kết hợp của tích chập.

#### Nhận xét 2 {#int-viii-s4-n2-rem-2 .statement}

— Cho $X$ là một không gian compact địa phương trên đó một nhóm compact địa phương $G$ tác động liên tục bên phải bởi $(x, s) \mapsto xs$. Cho $\beta$ là một độ đo dương trên $X$. Cho $\chi$ là một hàm $> 0$ trên $G \times X$, đo được đối với mọi độ đo trên $G \times X$, sao cho $\delta(s)\beta = \chi(s, \cdot) \cdot \beta$ với mọi $s \in G$. Cho $f$ là một hàm khả tích địa phương theo $\beta$ trên $X$ và cho $\mu$ là một độ đo trên $G$. Nếu $f \cdot \beta$ và $\mu$ là khả tích chập được (đối với ánh xạ $(x, s) \mapsto xs$ của $X \times G$ vào $X$), thì $(f \cdot \beta) * \mu$ có cơ sở $\beta$. Khi đó ta nói rằng $f$ và $\mu$ là khả tích chập được tương đối với $\beta$; mọi mật độ của $(f \cdot \beta) * \mu$ đối với $\beta$ được gọi là một tích chập của $f$ và $\mu$ tương đối với $\beta$, và được ký hiệu $f *^\beta \mu$ hoặc đơn giản là $f * \mu$.

Cho $G^0$ là nhóm đối của $G$. Bởi $(s, x) \mapsto xs$, $G^0$ tác động liên tục bên trái trong $X$. Nói rằng $f$ và $\mu$ là khả tích chập được theo nghĩa trên tương đương với nói rằng $\mu$ và $f$ là khả tích chập được đối với $G^0$ tác động bên trái trong $X$; và các tích chập $f *^\beta \mu$ không gì khác hơn là các tích chập $\mu *^\beta f$ đối với $G^0$ tác động bên trái trong $X$. Mặt khác, với $s \in G^0$ ta có $\gamma(s)\beta = \chi(s^{-1}, \cdot) \cdot \beta$. Các kết quả của Số 1 và 2 khi đó có thể được chuyển ngay lập tức thành các kết quả liên quan đến các tích $f *^\beta \mu$. Đặc biệt:

1) Nếu $s \in G$ và $f$ là khả tích địa phương theo $\beta$, thì $f$ và $\varepsilon_s$ là khả tích chập được và

$$
(f * \varepsilon_s)(x) = \chi(s^{-1}, x)f(xs^{-1}) .
$$

2) Nếu $f$ và $\mu$ là tích chập được với nhau và nếu một trong các điều kiện (i), (ii), (iii) của Mệnh đề 2 được thỏa mãn, thì $f *^\beta \mu$ được cho địa phương $\beta$-hầu khắp nơi bởi

$$
(f *^\beta \mu)(x) = \int_G f(xs^{-1})\chi(s^{-1}, x)\, d\mu(s) .
$$

Ta để lại cho người đọc nhiệm vụ chuyển dịch các mệnh đề khác. Lưu ý rằng nếu $\chi$ liên tục và $\beta$ có giá đỡ $X$, thì

$$
\chi(ts, x) = \chi(s, xt)\chi(t, x) \quad (x \in X; \ s, t \text{ trong } G) .
$$

### 3. Tích chập và chuyển vị

Ta quay lại các giả thiết và ký hiệu ở đầu No. 1, nhưng giả sử thêm rằng $\beta$ là *bất biến tương đối với nhân tử* $\chi$; do đó $\chi$ là một hàm liên tục trên $G$.

#### Mệnh đề 7 {#int-viii-s4-prop-7 .statement}

*Cho $f$ là một hàm khả tích $\beta$-địa phương trên $X$, $\nu$ là một độ đo trên $X$, và $\mu$ là một độ đo trên $G$. Giả sử rằng:*
(i) $\mu$ và $f$ là tích chập được với nhau và công thức (3) của No. 1 xác định địa phương $\beta$-hầu khắp nơi một tích chập $\mu *_{\beta} f$.
(ii) $\chi \cdot \check{\mu}$ và $\nu$ là tích chập được với nhau.
(iii) *Hàm* $g(s, x) = f(s^{-1}x)\chi(s^{-1})$ *là* $(\mu \otimes \nu)$*-khả tích.*
*Khi đó* $f$ *là khả tích bản chất đối với* $(\chi \cdot \check{\mu}) * \nu$, *hàm* $\mu *_{\beta} f$ *xác định bởi (3) là* $\nu$*-khả tích, và*

$$
\nu(\mu *_{\beta} f) = ((\chi \cdot \check{\mu}) * \nu)(f).
$$

Vì $g(s, x)$ khả tích đối với $\mu \otimes \nu$, hàm $f(sx)$ là khả tích bản chất đối với $(\chi \cdot \check{\mu}) \otimes \nu$ và $f$ là khả tích bản chất đối với $(\chi \cdot \check{\mu}) * \nu$. Theo định lý Lebesgue–Fubini, $\mu *_{\beta} f = \int g(s, x) d\mu(s)$ là $\nu$-khả tích và

$$
\begin{align*}
\nu(\mu *_{\beta} f) &= \iint f(s^{-1}x)\chi(s^{-1}) d\mu(s) d\nu(x) \\
&= \iint f(sx)\chi(s) d\check{\mu}(s) d\nu(x) = ((\chi \cdot \check{\mu}) * \nu)(f).
\end{align*}
$$

#### Ví dụ {#int-viii-s4-n3-exa-1 .statement}

— 1) Có thể lấy $f \in \mathcal{C}(X)$, $\nu \in \mathcal{C}'(X)$ và $\mu \in \mathcal{C}'(G)$ theo Mệnh đề 3, và Hệ quả của Mệnh đề 5 của §1, No. 4. Công thức (7) khi đó có nghĩa là tự đồng cấu $\nu \mapsto (\chi \cdot \check{\mu}) * \nu$ của $\mathcal{C}'(X)$ là *chuyển vị* của tự đồng cấu $f \mapsto \mu * f$ của $\mathcal{C}(X)$.

2) Có thể lấy $f \in \mathcal{K}(X)$, $\nu \in \mathcal{M}(X)$ và $\mu \in \mathcal{C}'(G)$ theo Mệnh đề 3, Mệnh đề 8 của §3, No. 2, và nhận xét rằng giá đỡ của hàm liên tục $g(s, x)$ giao với giá đỡ của $\mu \otimes \nu$ trong một tập compact. Công thức (7) khi đó có nghĩa là tự đồng cấu $\nu \mapsto (\chi \cdot \check{\mu}) * \nu$ của $\mathcal{M}(X)$ là *chuyển vị* của tự đồng cấu $f \mapsto \mu * f$ của $\mathcal{K}(X)$.

3) Nếu $G$ tác động đúng trên $X$, ta có thể lấy $f \in \mathcal{K}(X)$, $\nu \in \mathcal{C}'(X)$ và $\mu \in \mathcal{M}(G)$ theo Mệnh đề 4, Mệnh đề 8 của §3, No. 2, và cùng nhận xét như trong *Ví dụ 2*.

#### Mệnh đề 8 {#int-viii-s4-prop-8 .statement}

*Cho $f$ và $g$ là hai hàm địa phương $\beta$-khả tích vành trên $X$ và cho $\mu \in \mathcal{M}(G)$. Giả sử rằng:*

(i) $\mu$ và $f$ là nhân được với nhau và công thức (3) của No. 1 xác định địa phương hầu khắp nơi theo $\beta$ một tích chập $\mu *_{\beta} f$.

(ii) $\chi \cdot \check{\mu}$ và $g$ là nhân được với nhau và công thức (3) của No. 1 (với $\mu$ được thay bởi $\chi \cdot \check{\mu}$ và $f$ bởi $g$) xác định địa phương hầu khắp nơi theo $\beta$ một tích chập $(\chi \cdot \check{\mu}) *_{\beta} g$.

(iii) Tồn tại một hàm $\psi$ trên $G$, bằng địa phương hầu khắp nơi theo $\mu$ với 1, sao cho hàm

$$
h(s, x) = g(x) f(s^{-1} x) \chi(s^{-1}) \psi(s)
$$

là $(\mu \otimes \beta)$-khả tích.

Khi đó các hàm $g(x)((\mu *_{\beta} f)(x))$ và $f(x)(((\chi \cdot \check{\mu}) *_{\beta} g)(x))$ là khả tích theo $\beta$ một cách bản chất, và

$$
(8) \quad \int f(x)(((\chi \cdot \check{\mu}) *_{\beta} g)(x)) d\beta(x) = \int g(x)((\mu *_{\beta} f)(x)) d\beta(x).
$$

Thật vậy, theo (iii) và định lý Lebesgue–Fubini, hàm

$$
x \mapsto g(x) \int f(s^{-1} x) \chi(s^{-1}) \psi(s) d\mu(s)
$$

là khả tích theo $\beta$, và

$$
\begin{align*}
\mathrm{I} &= \iint f(s^{-1} x) g(x) \chi(s^{-1}) \psi(s) d\mu(s) d\beta(x) \\
&= \int g(x) d\beta(x) \int f(s^{-1} x) \chi(s^{-1}) \psi(s) d\mu(s).
\end{align*}
$$

Nhưng $\psi \cdot \mu = \mu$, do đó

$$
\int f(s^{-1} x) \chi(s^{-1}) \psi(s) d\mu(s) = (\mu *_{\beta} f)(x)
$$

địa phương hầu khắp nơi theo $\beta$. Điều này chứng minh rằng hàm

$$
x \mapsto g(x)((\mu *_{\beta} f)(x))
$$

là khả tích theo $\beta$ một cách bản chất và rằng

$$
\mathrm{I} = \int g(x)((\mu *_{\beta} f)(x)) d\beta(x).
$$

Mặt khác, Bổ đề 1 chỉ ra rằng hàm

$$(s, x) \mapsto g(sx)f(x)\chi(s^{-1})\psi(s)$$

là khả tích đối với $(\chi \cdot \mu) \otimes \beta$. Do đó hàm $(s, x) \mapsto g(s^{-1}x)f(x)\psi(s^{-1})$ là khả tích đối với $\check{\mu} \otimes \check{\beta}$, và

$$
\begin{align*}
\mathrm{I} &= \iint g(s^{-1}x)f(x)\psi(s^{-1})\, d\check{\mu}(s)\, d\beta(x) \\
&= \int f(x)\, d\beta(x) \int g(s^{-1}x)\psi(s^{-1})\, d\check{\mu}(s).
\end{align*}
$$

Nhưng $\check{\psi} \cdot \check{\mu} = \check{\mu}$ và do đó $\int g(s^{-1}x)\psi(s^{-1})\, d\check{\mu}(s) = ((\chi \cdot \check{\mu}) *^\beta g)(x)$ địa phương hầu khắp nơi theo $\beta$. Điều này chứng minh rằng hàm

$$x \mapsto f(x)(((\chi \cdot \check{\mu}) *^\beta g)(x))$$

là khả tích theo $\beta$ một cách bản chất và rằng

$$\mathrm{I} = \int f(x)(((\chi \cdot \check{\mu}) *^\beta g)(x))\, d\beta(x).$$

Điều này chứng minh mệnh đề.

#### Ví dụ {#int-viii-s4-n3-exa-2 .statement}

— 4) Có thể lấy $f \in \mathcal{C}(X)$, $g \in \mathcal{K}(X)$ và $\mu \in \mathcal{C}'(G)$ (với $\psi = 1$).

5) Nếu G tác động đúng trên X, có thể lấy $f \in \mathcal{K}(X)$, $g \in \mathcal{K}(X)$ và $\mu \in \mathcal{M}(G)$ (với $\psi = 1$).

6) Có thể lấy $f \in \mathbf{L}^p(X, \beta)$, $g \in \mathbf{L}^q(X, \beta)$ và $\mu \in \mathcal{M}^\rho(G)$, trong đó $1 \leq p < +\infty$, $\frac{1}{p} + \frac{1}{q} = 1$, $\rho = \chi^{-1/q}$. Các điều kiện (i) và (ii) được thỏa mãn theo các Mệnh đề 5 và 6. Ta hãy chứng minh (iii). Ta đã thấy rằng $\mu$ được mang bởi một tập S là hợp đếm được của các tập compact. Hãy lấy $\psi$ là hàm đặc số của S. Hàm $h$ là $(\mu \otimes \beta)$-đo được: thật vậy, hàm $(s, x) \mapsto g(x)\chi(s^{-1})\psi(s)$ là như vậy, cũng như hàm $(s, x) \mapsto f(s^{-1}x)$ theo Bổ đề 1. Hơn nữa, vì $g$ bằng không bên ngoài một hợp đếm được của các tập $\beta$-khả tích, $h$ bằng không bên ngoài một hợp đếm được của các tập $(\mu \otimes \beta)$-khả tích. Do đó ta có (Ch. V, §8, No. 3, Mệnh đề 7):

$$
\begin{align*}
\mathrm{J} &= \iint^* |g(x)f(s^{-1}x)|\chi(s^{-1})\psi(s)\, d|\mu|(s)\, d\beta(x) \\
&= \int^* |g(x)|\, d\beta(x) \int^* |f(s^{-1}x)|\chi(s^{-1})\psi(s)\, d|\mu|(s).
\end{align*}
$$

Nhưng vì $g$ (tương ứng $\psi$) bằng không bên ngoài một hợp đếm được của các tập khả tích, các tích phân trên của số hạng thứ hai trong (9) bằng các tích phân trên cốt yếu (Ch. V, §1, No. 2, Mệnh đề 7). Bây giờ (Ch. V, §5, No. 3, Mệnh đề 3)

$$
\int^\bullet |f(s^{-1}x)| \chi(s^{-1}) \psi(s) d|\mu|(s) = \int^\bullet |f(s^{-1}x)| \chi(s^{-1}) d|\mu|(s)
$$

vì $\mu = \psi \cdot \mu$. Theo Mệnh đề 6, tích phân cuối cùng này là hữu hạn và bằng $(|\mu| *^\beta |f|)(x)$ địa phương hầu khắp nơi theo $\beta$. Do đó

$$
J = \int^\bullet |g(x)|(|\mu| *^\beta |f|)(x) d\beta(x),
$$

và J là hữu hạn vì $g \in L^q$ và $|\mu| *^\beta |f| \in L^p$ (Mệnh đề 6). Do đó h là $(\mu \otimes \beta)$-khả tích.

Công thức (8) khi đó có nghĩa là tự đồng cấu $g \mapsto (\chi \cdot \check{\mu}) * g$ của $L^q(X, \beta)$ là, đối với $\mu \in \mathcal{M}^\rho(G)$, chuyển vị của tự đồng cấu $f \mapsto \mu * f$ của $L^p(X, \beta)$.

### 4. Tích chập của một độ đo và một hàm trên một nhóm

Cho G là một nhóm compact địa phương. Trong suốt các Số 4 và 5, ta cố định một độ đo dương tương đối bất biến $\beta \neq 0$ trên G; gọi $\chi$ và $\chi'$ là các nhân trái và phải của nó (nhớ rằng $\chi' = \chi \Delta_G$). Nếu $\mu$ là một độ đo trên G và $f$ là một hàm phức $\beta$-khả tích địa phương trên G, tính khả tích chập của $\mu$ và $f$ và các tích $\mu * f$ (tương ứng tính khả tích chập của $f$ và $\mu$ và các tích $f * \mu$) có thể được định nghĩa bằng cách xem G tác động lên chính nó ở bên trái (tương ứng ở bên phải) bởi các phép tịnh tiến. Ta hãy làm rõ trong tình huống này một số kết quả trước đó:

1) Cho $\mu$ là một độ đo trên G, $f$ là một hàm phức $\beta$-khả tích địa phương trên G. Giả sử một trong các điều kiện sau được thỏa mãn:
   (i) $f$ liên tục;
   (ii) $f$ bằng không trên phần bù của một hợp đếm được các tập compact;
   (iii) $\mu$ được mang bởi một hợp đếm được các tập compact.
Nếu $\mu$ và $f$ khả tích chập được thì, địa phương hầu khắp nơi theo $\beta$,

$$
(\mu * f)(x) = \int_G f(s^{-1}x) \chi(s^{-1}) d\mu(s).
$$

Nếu $f$ và $\mu$ khả tích chập được thì, địa phương hầu khắp nơi theo $\beta$,

$$
(f * \mu)(x) = \int_G f(xs^{-1}) \chi'(s^{-1}) d\mu(s).
$$

2) Cho $p$ và $q$ là hai số mũ liên hợp ($1 \leq p \leq +\infty$). Nếu $\mu \in \mathcal{M}^{\chi^{-1/q}}(G)$ và $f \in L^p(G, \beta)$, thì $\mu$ và $f$ liên tục xoắn được, và $\mu * f$ bằng địa phương $\beta$-hầu khắp nơi với một hàm thuộc $L^p(G, \beta)$; ta có (với sự lạm dụng ký hiệu đã được ghi nhận)

$$
\| \mu * f \|_p \leq \| \mu \|_{\chi^{-1/q}} \| f \|_p .
$$

Nếu $\mu \in \mathcal{M}^{{\chi'}^{-1/q}}(G)$ và $f \in L^p(G, \beta)$, thì $f$ và $\mu$ liên tục xoắn được, và $f * \mu$ bằng địa phương $\beta$-hầu khắp nơi với một hàm thuộc $L^p(G, \beta)$; ta có $\| f * \mu \|_p \leq \| \mu \|_{{\chi'}^{-1/q}} \| f \|_p$.

3) Các ánh xạ $(\mu, f) \mapsto \mu * f , (f, \mu) \mapsto f * \mu$ xác định trên $L^p(G, \beta)$ các cấu trúc của một môđun trái trên $\mathcal{M}^{\chi^{-1/q}}(G)$ và một môđun phải trên $\mathcal{M}^{{\chi'}^{-1/q}}(G)$. Hai phép toán ngoài trên $L^p(G, \beta)$ hoán vị được do tính kết hợp của phép xoắn.

4) Nếu $\mu * f$ liên tục và được cho tại mọi điểm bởi (10), thì

$$
(\mu * f)(e) = \int f(s^{-1}) \chi(s^{-1}) d\mu(s) .
$$

Nếu $f * \mu$ liên tục và được cho tại mọi điểm bởi (11), thì

$$
(f * \mu)(e) = \int f(s^{-1}) \chi'(s^{-1}) d\mu(s) .
$$

### 5. Phép xoắn của các hàm trên một nhóm

Ta giữ các ký hiệu $G, \beta, \chi, \chi'$ của No. 4.

Nhắc lại rằng nếu $f$ là một hàm phức trên $G$, tính chất khả tích địa phương theo $\beta$ là độc lập với lựa chọn $\beta$. Gọi $\mathcal{L}(G)$ là tập hợp các hàm có tính chất này. Nếu $f \in \mathcal{L}(G) , g \in \mathcal{L}(G)$, quan hệ

« $f \cdot \beta$ và $g \cdot \beta$ là liên tục xoắn được »

không phụ thuộc vào lựa chọn $\beta$ (\S 3, No. 1, Prop. 6). Khi đó ta sẽ nói rằng $f$ và $g$ là *có thể lấy tích chập*. Theo No. 1, $(f \cdot \beta) * (g \cdot \beta)$ có dạng $h \cdot \beta$ với $h \in \mathcal{L}(G)$, $h$ được xác định sai khác bởi các tập hợp địa phương $\beta$-không đáng kể. Ta sẽ viết $h = f *^{\beta} g$ và ta sẽ nói rằng $h$ là một *tích chập* của $f$ và $g$ đối với $\beta$. (Người ta bỏ qua $\beta$ khi không thể có nhầm lẫn.) Nếu $\beta$ được thay bởi $\psi \cdot \beta$, $\psi$ là một biểu diễn liên tục của $G$ trong $\mathbf{R}_+^*$, thì $h$ không thay đổi (\S 3, No. 1, Prop. 6); nếu $\beta$ được thay bởi $a \beta$ ($a \in \mathbf{R}_+^*$), thì $h$ được thay bởi $ah$. Tích chập của một số hàm trên $G$ được định nghĩa theo cách tương tự.

Nếu một trong các tích chập của $f$ và $g$ là liên tục, nó được xác định duy nhất vì giá của $\beta$ là $G$. Khi đó nó được gọi là *tích chập* của $f$ và $g$ đối với $\beta$.

Rõ ràng rằng

$$
f *_{\beta}^{\beta} g = (f \cdot \beta) *_{\beta}^{\beta} g = f *_{\beta}^{\beta} (g \cdot \beta).
$$

#### Mệnh đề 9 {#int-viii-s4-prop-9 .statement}

*Cho $f, g$ thuộc $\mathcal{L}(G)$. Giả sử rằng hàm $s \mapsto g(s^{-1}x)f(s)\chi(s^{-1})$ là khả tích $\beta$ theo nghĩa thiết yếu ngoại trừ một tập hợp địa phương $\beta$-không đáng kể các giá trị của $x$, và rằng hàm*

$$
x \mapsto \int |g(s^{-1}x)f(s)|\chi(s^{-1})\, d\beta(s),
$$

*được xác định địa phương $\beta$-hầu khắp nơi, là khả tích $\beta$ địa phương. Khi đó $f$ và $g$ có thể lấy tích chập.*

Điều này suy ra từ Mệnh đề 1 của No. 1.

#### Mệnh đề 10 {#int-viii-s4-prop-10 .statement}

*Cho $f, g$ thuộc $\mathcal{L}(G)$. Giả sử rằng một trong hai hàm này là liên tục hoặc bằng không trên phần bù của một hợp đếm được các tập hợp compact. Nếu $f$ và $g$ có thể lấy tích chập, thì hàm $f * g$ được cho địa phương $\beta$-hầu khắp nơi bởi*

$$
(f * g)(x) = \int_G g(s^{-1}x)f(s)\chi(s^{-1})\, d\beta(s)
= \int_G f(xs^{-1})g(s)\chi'(s^{-1})\, d\beta(s).
$$

Điều này suy ra từ Mệnh đề 2 của No. 1, và các nhận xét trong No. 4.

Đặc biệt, nếu $f * g$ là liên tục và được cho tại mọi điểm bởi (15), thì

$$
(f * g)(e) = \int g(s^{-1})f(s)\chi(s^{-1})\, d\beta(s) = \int f(s^{-1})g(s)\chi'(s^{-1})\, d\beta(s).
$$

Cụ thể hơn nữa, nếu $\beta$ là một độ đo Haar trái và phải, và nếu $f * g$ và $g * f$ là liên tục và được cho tại mọi điểm bởi (15) và công thức tương tự cho $g * f$, thì

$$
(f * g)(e) = (g * f)(e) = \int f(s)g(s^{-1})\, d\beta(s).
$$

#### Mệnh đề 11 {#int-viii-s4-prop-11 .statement}

— Cho $f, g$ thuộc $\mathcal{L}(G)$. Giả sử một trong hai hàm $f, g$ là liên tục, và một trong hai hàm $f, g$ có giá compact. Khi đó $f$ và $g$ chập được với nhau. Công thức (15) xác định với mọi $x \in G$ một tích $f * g$ liên tục. Nếu $f \in \mathcal{K}(G)$ và $g \in \mathcal{K}(G)$, thì $f * g \in \mathcal{K}(G)$.

Điều này suy ra từ các Mệnh đề 3 và 4 của No. 2.

#### Mệnh đề 12 {#int-viii-s4-prop-12 .statement}

— Cho $p$ và $q$ là hai số mũ liên hợp ($1 \leq p \leq +\infty$). Nếu $f \chi^{-1/q} \in L^1(G, \beta)$ và $g \in L^p(G, \beta)$, thì $f$ và $g$ chập được với nhau, $f * g$ bằng địa phương $\beta$-hầu khắp nơi với một hàm thuộc $L^p(G, \beta)$, và
$$
\|f * g\|_p \leq \|f \chi^{-1/q}\|_1 \|g\|_p.
$$
Nếu $f \in L^p(G, \beta)$ và $g {\chi'}^{-1/q} \in L^1(G, \beta)$, thì $f$ và $g$ chập được với nhau, $f * g$ bằng địa phương $\beta$-hầu khắp nơi với một hàm thuộc $L^p(G, \beta)$, và
$$
\|f * g\|_p \leq \|f\|_p \|g {\chi'}^{-1/q}\|_1.
$$
Điều này suy ra từ các Mệnh đề 5 và 6 của No. 2 và các nhận xét trong No. 4.

#### Mệnh đề 13 {#int-viii-s4-prop-13 .statement}

— Nếu $f \chi^{-1} \in L^1(G, \beta)$ và $g \in \overline{\mathcal{K}(G)}$, hoặc nếu $f \in \mathcal{K}(G)$ và $g {\chi'}^{-1} \in L^1(G, \beta)$, thì $f$ và $g$ chập được với nhau, và (15) xác định với mọi $x \in G$ một tích $f * g$ thuộc $\mathcal{K}(G)$.

Điều này suy ra từ Mệnh đề 5 của No. 2, và các nhận xét trong No. 4.

#### Mệnh đề 14 {#int-viii-s4-prop-14 .statement}

— Nếu $f \chi^{-1} \in L^1(G, \beta)$ và $g \in L^\infty(G, \beta)$, thì công thức (15) xác định với mọi $x \in G$ một tích $f * g$ bị chặn và liên tục đều đối với cấu trúc đều phải của $G$.

Ta đã biết rằng $f * g$ thuộc $L^\infty(G, \beta)$ (No. 2, Mệnh đề 5); hơn nữa, $(f * g)(x) = \int f(xs^{-1})g(s)\, d\nu(s)$, khi đặt $\nu = {\chi'}^{-1} \cdot \beta$; $\nu$ là một độ đo Haar phải. Do đó
$$
|(f * g)(x) - (f * g)(x')| \leq \|g\|_\infty \int |f(xs^{-1}) - f(x's^{-1})|\, d\nu(s)
$$
$$
= \|g\|_\infty \int |(f(s^{-1}) - f(x'x^{-1}s^{-1}))\, d\nu(s)
$$
và tích phân sau có thể nhỏ tùy ý với điều kiện $x'x^{-1}$ thuộc một lân cận thích hợp của $e$ (\S 2, No. 5, Mệnh đề 8).

#### Mệnh đề 15 {#int-viii-s4-prop-15 .statement}

— Cho $p$ và $q$ là hai số mũ liên hợp ($1 < p < +\infty$). Giả sử rằng $\beta$ là bất biến trái. Cho $f \in L^p(G, \beta)$, $g \in L^q(G, \check{\beta})$. Khi đó $f$ và $g$ chập được với nhau. Công thức (15) xác định, với mọi $x \in G$, một tích $f * g$ thuộc $\mathcal{K}(G)$ và thỏa mãn
$$
\|f * g\|_\infty \leq \|f\|_p \|g\|_q.
$$

Thật vậy, ta có $\dot{g} \in L^q(G, \beta)$, do đó hàm $s \mapsto g(s^{-1}x)f(s)$ là $\beta$-khả tích với mọi $x \in G$. Hơn nữa,

$$
\int |g(s^{-1}x)f(s)| d\beta(s) \leq \left( \int |f(s)|^p d\beta(s) \right)^{1/p} \left( \int |g(s^{-1}x)|^q d\beta(s) \right)^{1/q}
= \|f\|_p \left( \int |\dot{g}(x^{-1}s)|^q d\beta(s) \right)^{1/q} = \|f\|_p \|\dot{g}\|_q,
$$

do đó $f$ và $g$ chập được với nhau (Mệnh đề 9). Đồng thời cũng thấy rằng (15) xác định với mọi $x$ một tích $f * g$ sao cho

$$
|(f * g)(x)| \leq \|f\|_p \|\dot{g}\|_q.
$$

Với $f, g$ trong $\mathcal{K}(G)$, ta có $f * g \in \mathcal{K}(G)$ (Mệnh đề 11); do đó, với $f \in L^p(G, \beta)$ và $g \in L^q(G, \dot{\beta})$, tích $f * g$ do (15) cung cấp là giới hạn đều của các hàm trong $\mathcal{K}(G)$, nên thuộc $\overline{\mathcal{K}(G)}$.

#### Hệ quả {#int-viii-s4-n5-cor-1 .statement}

— Cho $f \in L^2(G, \beta)$, $g \in L^2(G, \beta)$. Khi đó $f$ và $\dot{g}$ chập được với nhau. Một trong các tích chập $f * \dot{g}$ thuộc $\overline{\mathcal{K}(G)}$ và giá trị của nó tại $e$ là $\int_G f(s)g(s) d\beta(s)$.

Chỉ cần lấy $p = q = 2$ trong Mệnh đề 15 và áp dụng (16).

Từ đây ta không còn giả thiết $\beta$ là bất biến trái nữa. Cho $\rho$ là một hàm hữu hạn nửa liên tục dưới $> 0$ trên $G$, sao cho $\rho(st) \leq \rho(s)\rho(t)$ với mọi $s, t$ trong $G$. Ta ký hiệu bởi $L^\rho(G, \beta)$ tập hợp các lớp tương đương của các hàm phức trên $G$ khả tích đối với $\rho \cdot \beta$. Nhờ ánh xạ $f \mapsto f \cdot \beta$, có thể đồng nhất $L^\rho(G, \beta)$ với tập hợp các phần tử của $\mathcal{M}^\rho(G)$ có cơ sở $\beta$ (một tập hợp độc lập với lựa chọn của $\beta$). Nếu đặt

$$
\|f\|_\rho = \int_G |f(s)| \rho(s) d\beta(s)
$$

đối với $f \in L^\rho(G, \beta)$, sự đồng nhất này tương thích với các chuẩn, do đó $L^\rho(G, \beta)$ xuất hiện như một đại số con chuẩn đầy đủ của $\mathcal{M}^\rho(G)$. Hơn nữa, nó là một iđêan hai phía của $\mathcal{M}^\rho(G)$ theo Mệnh đề 10 của §3, No. 2. (Với $\rho = 1$, ta thu được một trong các khẳng định của No. 4.) Đặc biệt, $L^1(G, \beta)$ có thể được đồng nhất với một iđêan hai phía đóng của $\mathcal{M}^1(G)$.

#### Mệnh đề 16 {#int-viii-s4-prop-16 .statement}

— Cho $U$ là một biểu diễn liên tục của $G$ trong một không gian Banach $E$. Đặt $\rho(s) = \|U(s)\|$ với mọi $s \in G$. Với mọi $f \in L^\rho(G, \beta)$, đặt $U(f) = U(f \cdot \beta)$. Khi đó $f \mapsto U(f)$ là một biểu diễn tuyến tính của đại số $L^\rho(G, \beta)$ trong $E$, sao cho $\|U(f)\| \leq \|f\|_\rho$.

Điều này suy ra từ §2, No. 6 và §3, No. 3, Mệnh đề 11.

### 6. Các áp dụng

#### Mệnh đề 17 {#int-viii-s4-prop-17 .statement}

— Cho G là một nhóm địa phương compact, A là một tập con của G, đo được và không địa phương không đáng kể đối với một độ đo Haar. Khi đó $A \cdot A^{-1}$ là một lân cận của e.

Cho $\beta$ là một độ đo Haar trái. Tồn tại một tập con compact K của G sao cho $B = A \cap K$ là khả tích và có độ đo > 0 đối với $\beta$. Hãy áp dụng Hệ quả của Mệnh đề 15 với $f = g = \varphi_B$. Hàm $F = \varphi_B * \check{\varphi}_B$ là liên tục và > 0 tại e. Vì vậy tồn tại một lân cận V của e sao cho $F(x) > 0$ với $x \in V$. Bây giờ,

$$
F(x) = \int \varphi_B(s) \varphi_B(x^{-1}s) d\beta(s) = \beta(B \cap xB).
$$

Do đó, với $x \in V$, ta có $B \cap xB \neq \emptyset$, do đó $x \in B \cdot B^{-1}$. Vậy $V \subset B \cdot B^{-1} \subset A \cdot A^{-1}$.

#### Hệ quả 1 {#int-viii-s4-prop-17-cor-1 .statement}

— Cho H là một nhóm con của G đo được đối với một độ đo Haar $\beta$. Khi đó H либо mở, либо địa phương $\beta$-không đáng kể.

Thật vậy, $H = H \cdot H^{-1}$, do đó nếu H không địa phương $\beta$-không đáng kể, thì H chứa một lân cận của e (Mệnh đề 17), nên là mở (GT, III, §2, No. 1, Hệ quả của Mệnh đề 4).

#### Hệ quả 2 {#int-viii-s4-prop-17-cor-2 .statement}

— Cho L là một tập con của G ổn định đối với phép nhân và có phần bù địa phương không đáng kể đối với một độ đo Haar $\beta$. Khi đó $L = G$.

Thật vậy, $L^{-1}$ và $L \cap L^{-1}$ có các phần bù địa phương $\beta$-không đáng kể. Mà $L \cap L^{-1}$ là một nhóm con, nên là mở (Hệ quả 1) và vì thế đóng. Do đó $G - (L \cap L^{-1})$, là tập mở và địa phương $\beta$-không đáng kể, là rỗng. Vậy $G = L \cap L^{-1}$.

#### Mệnh đề 18 {#int-viii-s4-prop-18 .statement}

— Cho G là một nhóm địa phương compact, $\Gamma$ là một tập hợp được trang bị một phép nhân $(u, v) \mapsto uv$ và một tôpô Hausdorff sao cho:
1) tôpô của $\Gamma$ là bất biến đối với các phép tịnh tiến;
2) hạn chế của phép nhân lên mọi tập con compact của $\Gamma \times \Gamma$ là liên tục.

Cho $f : G \to \Gamma$ là một ánh xạ từ G vào $\Gamma$ sao cho $f(xy) = f(x)f(y)$ với $x, y$ trong G, và đo được đối với một độ đo Haar $\beta$ trên G. Khi đó $f$ là liên tục.

Đặt $g(x) = f(x^{-1})$ với $x \in G$. Vì $f$ và $g$ là $\beta$-đo được, nên tồn tại một tập con compắc K của G không $\beta$-không đáng kể sao cho các hạn chế của $f$ và $g$ lên K là liên tục. Ánh xạ $(x, y) \mapsto f(xy^{-1}) = f(x)g(y)$ từ $K \times K$ vào $\Gamma$ là liên tục vì phép nhân của $\Gamma$ liên tục trên $f(K) \times g(K)$; bây giờ, ánh xạ này có thể được viết thành $\varphi \circ \psi$, trong đó $\psi$ là ánh xạ $(x, y) \mapsto xy^{-1}$ từ $K \times K$ lên $K \cdot K^{-1}$, và $\varphi$ là hạn chế của $f$ lên $K \cdot K^{-1}$. Gọi $R$ là quan hệ tương đương được xác định trên $K \times K$ bởi $\psi$. Ánh xạ $\psi'$ từ $(K \times K)/R$ lên $K \cdot K^{-1}$ suy ra từ $\psi$ bằng cách chuyển sang thương là liên tục, do đó $(K \times K)/R$ là Hausdorff và $\psi'$ là một đồng phôi. Vì $\varphi \circ \psi$ là liên tục, ta thấy rằng hạn chế của $f$ lên $K \cdot K^{-1}$ là liên tục. Bây giờ, $K \cdot K^{-1}$ là một lân cận của $e$ (Mệnh đề 17), do đó $f$ liên tục tại $e$. Với mọi $x_0 \in G$, $f(x_0x) = f(x_0)f(x)$, vì thế $f$ liên tục tại $x_0$ vì tôpô của $\Gamma$ là bất biến dưới các phép tịnh tiến.

#### Hệ quả 1 {#int-viii-s4-prop-18-cor-1 .statement}

*Cho $G$ là một nhóm địa phương compắc, $\beta$ là một độ đo Haar trên $G$, $E$ là một không gian lồi địa phương thùng Hausdorff, $U$ là một biểu diễn tuyến tính của $G$ trong $E$, sao cho $U(s) \in \mathcal{L}(E;E)$ với mọi $s \in G$, $\beta$-đo được khi $\mathcal{L}(E;E)$ được trang bị tôpô hội tụ từng điểm. Khi đó $U$ là một biểu diễn tuyến tính liên tục.*

Cho $\Gamma$ là nhóm các tự đẳng cấu của $E$, được trang bị tôpô hội tụ từng điểm. Tôpô này là Hausdorff và bất biến qua các phép tịnh tiến. Cho $K$ là một tập con compact của $\Gamma$. Khi đó $K$ bị chặn trong $\mathcal{L}(E;E)$ được trang bị tôpô hội tụ từng điểm, do đó là đều liên tục (TVS, III, §4, No. 2, Th. 1); vì vậy ánh xạ $(u,v) \mapsto v \circ u$ từ $K \times K$ vào $\mathcal{L}(E;E)$ là liên tục (*loc. cit.*, §5, No. 5, Hệ quả 1 của Mệnh đề 9). Do đó, với mọi $x \in E$, ánh xạ $s \mapsto U(s)x$ từ $G$ vào $E$ là liên tục (Mệnh đề 18). Vì $E$ là barreled, $U$ là liên tục (§2, No. 1, Mệnh đề 1).

#### Hệ quả 2 {#int-viii-s4-prop-18-cor-2 .statement}

*Cho $G$ là một nhóm compact địa phương, $\beta$ là một độ đo Haar trên $G$, $E$ là một không gian Banach tách được, và $U$ là một biểu diễn tuyến tính của $G$ trong $E$ sao cho $U(s) \in \mathcal{L}(E;E)$ với mọi $s \in G$. Cho $(a_m)$ là một dãy toàn phần trong $E$, và cho $(a'_n)$ là một dãy trù mật trong quả cầu đơn vị $B'$ của không gian đối ngẫu $E'$ của $E$, được trang bị tôpô yếu. Giả sử rằng các hàm $s \mapsto \langle U(s)a_m, a'_n \rangle$ trên $G$ là $\beta$-đo được. Khi đó $U$ là một biểu diễn tuyến tính liên tục.*

Trước hết, hãy chỉ ra rằng với mọi $z' \in E'$, các hàm vô hướng

$$
s \mapsto \langle U(s)a_m, z' \rangle
$$

là $\beta$-đo được; ta có thể tự hạn chế vào trường hợp $\|z'\| \leq 1$, và, vì $B'$ mêtric được đối với tôpô yếu (TVS, III, §3, No. 4, Hệ quả 2 của Mệnh đề 6), tồn tại một dãy con $(a'_{n_k})$ của $(a'_n)$ hội tụ yếu đến $z'$; hàm

$$
s \mapsto \langle U(s)a_m, z' \rangle
$$

do đó là giới hạn của một dãy các hàm $\beta$-đo được, do đó được mệnh đề của chúng ta. Suy ra rằng ánh xạ $s \mapsto U(s)a_m$ từ $G$ vào $E$ là $\beta$-đo được với mọi $m$ (Ch. IV, §5, No. 5, Mệnh đề 10). Mặt khác, tồn tại một dãy $(b_m)$ các phần tử của $E$, là những tổ hợp tuyến tính của các $a_i$, trù mật trong quả cầu đơn vị của $E$. Với mọi $s \in G$, $\|U(s)\| = \sup_m \|U(s)b_m\|$, vì vậy $s \mapsto \|U(s)\|$ là đo được. Cho $K$ là một tập con compắc của $G$ và cho $\varepsilon > 0$. Tồn tại một tập con compắc $K_0$ của $K$ sao cho $\beta(K - K_0) \leq \varepsilon$ và sao cho các hạn chế lên $K_0$ của các hàm $s \mapsto U(s)a_m$ và $s \mapsto \|U(s)\|$ là liên tục. Khi đó các $U(s)$ với $s \in K_0$ là đồng liên tục, và tôpô hội tụ điểm từng điểm cảm sinh trên $U(K_0)$ tôpô hội tụ điểm từng điểm trên tập các $a_m$ (TVS, III, §3, No. 4, Mệnh đề 5). Do đó ánh xạ $s \mapsto U(s)$ từ $K_0$ vào $\mathcal{L}_s(E; E)$ là liên tục. Khi ấy chỉ cần áp dụng Hệ quả 1.

### 7. Chính quy hóa

#### Mệnh đề 19 {#int-viii-s4-prop-19 .statement}

— *Cho $G$ là một nhóm địa phương compắc, $\beta$ là một độ đo dương tương đối bất biến $\neq 0$ trên $G$, $\mathcal{B}$ là một cơ sở của bộ lọc các lân cận của $e$ trong $G$, gồm các lân cận compắc. Với mỗi $V \in \mathcal{B}$, cho $f_V$ là một hàm liên tục $\geq 0$ trên $G$, có giá được chứa trong $V$, sao cho $\int f_V d\beta = 1$. Nếu $\mu$ là một độ đo trên $G$ thì, trong $\mathcal{M}(G)$ được trang bị tôpô hội tụ compắc trong $\mathcal{H}(G)$,

$$
\mu = \lim_V (\mu * f_V) \cdot \beta = \lim_V (f_V * \mu) \cdot \beta,
$$

giới hạn được lấy theo bộ lọc tiết diện của $\mathcal{B}$.

Đối với tôpô hội tụ compắc trong $\mathcal{C}(G)$, $f_V \cdot \beta$ hội tụ đến $\varepsilon_e$ theo bộ lọc tiết diện của $\mathcal{B}$ (\S2, No. 7, Hệ quả 1 của Bổ đề 4). Vì vậy $\mu = \lim_V \mu * (f_V \cdot \beta) = \lim_V (f_V \cdot \beta) * \mu$ trong $\mathcal{M}(G)$ được trang bị tôpô hội tụ compắc trong $\mathcal{H}(G)$ (\S3, No. 3, Hệ quả của Mệnh đề 12).

#### Nhận xét 1 {#int-viii-s4-n7-rem-1 .statement}

Như vậy ta thấy rằng mọi độ đo trên $G$ đều là giới hạn của các độ đo thừa nhận một *mật độ liên tục* đối với mọi độ đo Haar (đối với tôpô được chỉ ra trong Mệnh đề 19 và *a fortiori* đối với tôpô mơ hồ).

#### Nhận xét 2 {#int-viii-s4-n7-rem-2 .statement}

Nếu $G$ khả mêtric hóa được, thì có thể lấy $\mathcal{B}$ là một dãy $(V_n)$ các lân cận. Khi đó $\mu$ là giới hạn của dãy các độ đo $(\mu * f_{V_n}) \cdot \beta$ có mật độ liên tục. *Nếu $G$ là một nhóm Lie thực, thì có thể lấy các $f_{V_n}$ khả vi vô hạn lần; sau này ta sẽ thấy rằng khi đó các mật độ $\mu * f_{V_n}$ cũng khả vi vô hạn lần.*

#### Mệnh đề 20 {#int-viii-s4-prop-20 .statement}

— *Giữ nguyên các giả thiết và ký hiệu của Mệnh đề 19.* Cho $p \in [1, +\infty[$ và $g \in L^p(G, \beta)$. Khi đó

$$
g = \lim_V g *^\beta f_V = \lim_V f_V *^\beta g
$$

theo nghĩa của chuẩn $N_p$, giới hạn được lấy đối với bộ lọc tiết diện của $\mathcal{B}$.

Chỉ cần áp dụng Mệnh đề 6 (iii), và §2, No. 7, Hệ quả 3 của Bổ đề 4.

#### Nhận xét 3 {#int-viii-s4-n7-rem-3 .statement}

Theo Mệnh đề 15, các hàm $g * f_V$, $f_V * g$ thuộc $\mathcal{K}(G)$.

#### Hệ quả {#int-viii-s4-n7-cor-1 .statement}

— Cho $W$ là một không gian con tuyến tính đóng của $L^1(G, \beta)$. Để $W$ là một iđêan trái (tương ứng, phải) của $L^1(G, \beta)$, điều kiện cần và đủ là $W$ bất biến đối với các phép tịnh tiến trái (tương ứng, phải) của $G$.

Giả sử $W$ là một iđêan trái. Cho $s \in G$ và $g \in W$. Ta có $\varepsilon_s * g = \lim_V f_V * (\varepsilon_s * g) = \lim_V (f_V * \varepsilon_s) * g$, và $(f_V * \varepsilon_s) * g \in W$, do đó $\varepsilon_s * g \in W$, suy ra $\gamma(s)g \in W$. Ngược lại, nếu $W$ bất biến dưới các phép tịnh tiến trái, thì $\mu *^\beta g \in W$ với $\mu \in \mathcal{M}^1(G)$ và $g \in W$, do đó $W$ a fortiori là một iđêan trái của $L^1(G, \beta)$. Lập luận tương tự đối với các iđêan phải.

#### Ví dụ {#int-viii-s4-n7-exa-1 .statement}

Ta lấy $G = \mathbf{R}$. Hãy định nghĩa một hàm $F_n \in \mathcal{K}(\mathbf{R})$ bởi
$$
F_n(x) = (1 - x^2)^n \quad \text{nếu } x \in [-1, 1] \\
F_n(x) = 0 \qquad \text{nếu } x \notin [-1, 1].
$$
Đặt $A_n = \int_{-1}^{+1} F_n(x) dx$, và $G_n = A_n^{-1} F_n$. Ngay lập tức thấy rằng các độ đo $G_n(x) dx$ thỏa mãn các điều kiện của §2, No. 7, Hệ quả 1 của Bổ đề 4. Cho $\mu$ là một độ đo trên $\mathbf{R}$ mà giá của nó được chứa trong $[-1/2, 1/2]$. Khi đó
$$
(\mu * G_n)(x) = \int_{\mathbf{R}} G_n(x - y) d\mu(y)
= A_n^{-1} \int_{-1/2}^{1/2} F_n(x - y) d\mu(y).
$$
Nếu $-1/2 \leq x \leq 1/2$, thì
$$
(\mu * G_n)(x) = A_n^{-1} \int_{-1/2}^{1/2} [1 - (x - y)^2]^n d\mu(y),
$$
do đó $\mu * G_n$ trùng với một đa thức trên $[-1/2, 1/2]$. Đặc biệt, nếu $f$ là một hàm liên tục mà giá của nó được chứa trong $[-1/2, 1/2]$, thì $f * G_n$ trùng trên $[-1/2, 1/2]$ với một đa thức; hơn nữa, theo Mệnh đề 5 (iv), và §2, No. 7, Hệ quả 3 của Bổ đề 4, $f * G_n$ hội tụ đều tới $f$.
*Nếu $f$ thuộc lớp $C^r$, thì các đạo hàm $D^s(f * G_n)$ hội tụ đều tới $D^s f$ với $0 \leq s \leq r$.*

### Bài tập {#int-viii-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
