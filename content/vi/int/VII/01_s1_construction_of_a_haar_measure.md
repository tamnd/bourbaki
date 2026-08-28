---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 1
section_title: Construction of a Haar measure
lang: vi
source: int-vii-ix
pdf_pages: 0007-0032, 0084-0093
extraction: ocr
subsections:
    - "no": 1
      title: Definitions and notations
      page: 0
      pdf_page: 7
    - "no": 2
      title: The existence and uniqueness theorem
      page: 6
      pdf_page: 12
    - "no": 3
      title: Modulus
      page: 10
      pdf_page: 16
    - "no": 4
      title: Modulus of an automorphism
      page: 13
      pdf_page: 19
    - "no": 5
      title: Haar measure of a product
      page: 14
      pdf_page: 20
    - "no": 6
      title: Haar measure of an inverse limit*
      page: 15
      pdf_page: 21
    - "no": 7
      title: Local definition of a Haar measure
      page: 18
      pdf_page: 24
    - "no": 8
      title: Relatively invariant measures
      page: 19
      pdf_page: 25
    - "no": 9
      title: Quasi-invariant measures
      page: 20
      pdf_page: 26
    - "no": 10
      title: Locally compact fields
      page: 21
      pdf_page: 27
    - "no": 11
      title: Finite-dimensional algebras over a locally compact field
      page: 25
      pdf_page: 31
statements: 42
exercises: 23
content_sha256: f3abda162ae4f2167c2a8015e1e5e74aec3f352555bc97a7fc7601d61c84078c
translated_from: content/en/int/VII/01_s1_construction_of_a_haar_measure.md
source_content_sha256: 419ab91b51b52ce173f1a3d494e9786a6b3f625f788e1e4f59833324cd27ed0e
translation_model: gpt-5.4-mini
translation_run: translate-vi-ae8ef630
glossary_version: 34
glossary_terms_sha256: b7ba7d4b6c2d35ce9fe598e3a4a2273b7e4300a95a7789709398e6bdbb4680c2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. XÂY DỰNG MỘT ĐỘ ĐO HAAR

### 1. Các định nghĩa và ký hiệu

Cho $G$ là một nhóm tôpô tác động liên tục bên trái (GT, III, §2, No. 4) trên một không gian compact địa phương $X$; với $s \in G$ và $x \in X$, đặt $sx$ là biến đổi của $x$ bởi $s$. Kí hiệu $\gamma_X(s)$, hay $\gamma(s)$, là phép đồng phôi của $X$ lên $X$ được xác định bởi

(1)
$$
\gamma(s)x = sx.
$$

Ta có

(2)
$$
\gamma(st) = \gamma(s)\gamma(t).
$$

Nếu $f$ là một hàm xác định trên $X$, thì $\gamma(s)f$ được xác định bằng phép chuyển cấu trúc, tức là bởi công thức $(\gamma(s)f)(\gamma(s)x) = f(x)$; nói cách khác,

(3)
$$
(\gamma(s)f)(x) = f(s^{-1}x).
$$

Nếu $\mu$ là một độ đo xác định trên $X$, thì $\gamma(s)\mu$ cũng được xác định bằng phép chuyển cấu trúc, dẫn đến

(4)
$$
\langle f, \gamma(s)\mu \rangle = \langle \gamma(s^{-1})f, \mu \rangle \quad \text{với } f \in \mathcal{K}(X).
$$

Nói cách khác,

(5)
$$
\int_X f(x) d(\gamma(s)\mu)(x) = \int_X f(sx) d\mu(x).
$$

Nếu $A$ là một tập hợp khả tích theo $(\gamma(s)\mu)$, thì $s^{-1}A$ khả tích theo $\mu$ và

(6)
$$
(\gamma(s)\mu)(A) = \mu(s^{-1}A).
$$

Độ đo $\gamma(s)\mu$ cũng có thể được định nghĩa là *ảnh* của $\mu$ qua $\gamma(s)$.

Thay vì viết $d(\gamma(s)\mu)(x)$, đôi khi người ta thấy tiện viết $d\mu(s^{-1}x)$; khi đó công thức (5) có dạng sau:

$$
\int_X f(x) d\mu(s^{-1}x) = \int_X f(sx) d\mu(x);
$$

biểu thức ở bên phải khi đó có thể được suy ra từ biểu thức ở bên trái bằng cách 'thay $x$ bằng $sx$.'

#### Định nghĩa 1 {#int-vii-s1-def-1 .statement}

*Cho $\mu$ là một độ đo trên $X$.*
a) $\mu$ *được gọi là* **bất biến dưới $G$** *nếu* $\gamma(s)\mu = \mu$ *với mọi* $s \in G$.
b) $\mu$ *được gọi là* **tương đối bất biến dưới $G$** *nếu* $\gamma(s)\mu$ *tỉ lệ với* $\mu$ *với mọi* $s \in G$.
c) $\mu$ *được gọi là* **gần bất biến dưới $G$** *nếu* $\gamma(s)\mu$ *tương đương với* $\mu$ *với mọi* $s \in G$.

#### Nhận xét {#int-vii-s1-n1-rem-1 .statement}

— 1) Giả sử $\mu$ bất biến. Khi đó $|\mu|$, $\mathcal{R}(\mu)$, $\mathcal{I}(\mu)$ đều bất biến. Nếu $\mu$ thực, thì $\mu^+$ và $\mu^-$ đều bất biến.
2) Giả sử $\mu$ tương đối bất biến và khác không. Với mọi $s \in G$, tồn tại duy nhất một số phức $\chi(s)$ sao cho

(7)
$$
\gamma(s)\mu = \chi(s)^{-1}\mu,
$$

và hàm $\chi$ trên $G$ là một biểu diễn của $G$ trong $\mathbf{C}^*$, gọi là *nhân tử* của $\mu$. Công thức (5) khi đó cho

$$
(8) \quad \int_X f(sx)\, d\mu(x) = \chi(s)^{-1} \int_X f(x)\, d\mu(x),
$$

và công thức (6) cho

$$
(9) \quad \mu(sA) = \chi(s) \mu(A).
$$

Với các quy ước đã đặt ở trên, (7) cũng có thể viết

$$
(10) \quad d\mu(sx) = \chi(s)\, d\mu(x).
$$

3) Vì $|\gamma(s)\mu| = \gamma(s)(|\mu|)$, nói rằng $\mu$ là gần bất biến tức là nói rằng $|\mu|$ là gần bất biến.

Nếu $\mu$ là gần bất biến và $\mu'$ là một độ đo khác trên $X$ tương đương với $\mu$, thì $\gamma(s)\mu'$ tương đương với $\gamma(s)\mu$, do đó tương đương với $\mu$, do đó tương đương với $\mu'$, và vì vậy $\mu'$ là gần bất biến. Nói rằng $\mu$ là gần bất biến dưới $G$ vì thế có nghĩa là *lớp* của $\mu$ là bất biến dưới $G$.

Để $\mu$ là gần bất biến, điều kiện cần và đủ là tập hợp các tập con địa phương $\mu$-không đáng kể của $X$ bất biến dưới $G$ (Ch. V, §5, No. 5, Th. 2), hoặc cũng là rằng, với mọi tập con compact $K$ của $X$ mà $\mu$-không đáng kể và với mọi $s \in G$, $sK$ là $\mu$-không đáng kể (*loc. cit.*, *Nhận xét*).

Nếu $\mu$ là gần bất biến, thì giá đỡ của $\mu$ bất biến dưới $G$. Đặc biệt nếu $G$ là *bắc cầu* trong $X$ (A, I, §5, No. 5, Def. 6), thì giá đỡ này hoặc rỗng (nếu $\mu = 0$) hoặc bằng $X$ (nếu $\mu \neq 0$).

#### Bổ đề 1 {#int-vii-s1-lem-1 .statement}

— *Cho $X, Y, Z$ là ba không gian tôpô, với $Y$ địa phương compact. Cho $(x, y) \mapsto xy$ là một ánh xạ liên tục của $X \times Y$ vào $Z$, xác định một ánh xạ $x \mapsto u_x$ của $X$ vào $\mathcal{F}(Y; Z)$ bởi quan hệ $u_x(y) = xy$. Cho $f$ là một hàm liên tục trên $Z$ lấy giá trị trong $\mathbf{R}$ hoặc trong một không gian Banach, S là giá đỡ của $f$, và $\mu$ là một độ đo trên $Y$. Giả sử rằng với mọi $x_0 \in X$, tồn tại một lân cận $V$ của $x_0$ trong $X$ sao cho $\bigcup_{x \in V} u_x^{-1}(S)$ tương đối compact trong $Y$. Khi đó:
a) với mọi $x \in X$, $f \circ u_x$ liên tục trên $Y$, với giá đỡ compact;
b) ánh xạ $x \mapsto \int_Y f(xy)\, d\mu(y)$, được xác định bởi a), là liên tục trên $X$.

Mệnh đề a) hiển nhiên. Ta chứng minh b). Vì tính liên tục là một tính chất địa phương, ta có thể rút gọn về trường hợp $\bigcup_{x \in X} u_x^{-1}(S)$ được chứa trong một tập con compact $Y'$ của $Y$. Vì hàm $(x, y) \mapsto f(xy)$ liên tục trên $X \times Y$, $f \circ u_x$ tiến tới $f \circ u_{x_0}$ đều trên $Y'$ khi $x$ tiến tới $x_0$

(GT, X, §3, No. 4, Th. 3), do đó $\mu(f \circ u_x)$ tiến tới $\mu(f \circ u_{x_0})$. Do đó bổ đề.*

Bây giờ ta trở lại các ký hiệu trước.

#### Mệnh đề 1 {#int-vii-s1-prop-1 .statement}

— *Giả sử rằng G là địa phương compact. Cho $\mu$ là một độ đo bất biến tương đối khác không trên X. Khi đó nhân tử $\chi$ của nó là một hàm liên tục trên G.*

Thật vậy, cho $f \in \mathcal{K}(X)$, S là giá đỡ của $f$, $s_0$ là một điểm của G, và V là một lân cận compact của $s_0$ trong G; khi đó, tập hợp

$$
\bigcup_{s \in V} \gamma(s)^{-1}(S) = V^{-1}S
$$

là compact trong X; bởi Bổ đề 1 và công thức (8), $\chi(s^{-1}) \langle \mu, f \rangle$ phụ thuộc liên tục vào $s$; nếu chọn $f$ sao cho $\langle \mu, f \rangle \neq 0$, ta thấy rằng $\chi$ liên tục.*

Bây giờ cho G là một nhóm tôpô tác động liên tục bên phải trên một không gian địa phương compact X; với $s \in G$ và $x \in X$, ta gọi $xs$ là phép biến đổi của $x$ bởi $s$. Ta ký hiệu $\delta_X(s)$, hay $\delta(s)$, là đồng phôi của X được xác định bởi

(1')
$$
\delta(s)x = xs^{-1}.
$$

Ta có

(2')
$$
\delta(st) = \delta(s)\delta(t).
$$

Bằng phép chuyển cấu trúc, ta định nghĩa tác động của $\delta(s)$ lên các hàm và các độ đo trên X:

(3')
$$
(\delta(s)f)(x) = f(xs)
$$
(4')
$$
\langle f, \delta(s)\mu \rangle = \langle \delta(s^{-1})f, \mu \rangle
$$
(5')
$$
\int_X f(x) d(\delta(s)\mu)(x) = \int_X f(xs^{-1}) d\mu(x)
$$
(6')
$$
(\delta(s)\mu)(A) = \mu(As).
$$

Chúng ta đồng ý viết $d\mu(xs)$ thay cho $d(\delta(s)\mu)(x)$, và (5') khi đó có dạng

$$
\int_X f(x) d\mu(xs) = \int_X f(xs^{-1}) d\mu(x).
$$

Người ta định nghĩa theo một cách tương tự các độ đo trên X bất biến, tương đối bất biến và quasi-bất biến dưới G. Nếu $\mu$ là tương đối bất biến, thì nhân tử $\chi$ của nó được định nghĩa bởi các công thức

$$
(7') \quad \delta(s)\mu = \chi(s)\mu
$$
$$
(8') \quad \int_X f(xs)\,d\mu(x) = \chi(s)^{-1} \int_X f(x)\,d\mu(x)
$$
$$
(9') \quad \mu(As) = \chi(s)\mu(A)
$$
$$
(10') \quad d\mu(xs) = \chi(s)\,d\mu(x).
$$

Nếu xem nhóm $G^0$ đối của G tác động trên X bởi $(x,s) \mapsto xs$, thì $\mu$ là tương đối bất biến dưới $G^0$ với cùng nhân tử $\chi$.

Cuối cùng, cho G là một nhóm locally compact. Nó tác động lên chính nó bởi các phép tịnh tiến trái và phải, theo các công thức $\gamma(s)x = sx$, $\delta(s)x = xs^{-1}$. Khi đó

$$
(11) \quad \gamma(s)\delta(t) = \delta(t)\gamma(s).
$$

Mọi điều nói trên đều áp dụng ở đây, do đó ta có trên G các khái niệm về các độ đo *bất biến trái*, *bất biến phải*, *tương đối bất biến trái*, *tương đối bất biến phải*, *quasi-bất biến trái*, *quasi-bất biến phải* (tuy nhiên, xem Nos. 8 và 9).

Ánh xạ $x \mapsto x^{-1}$ là một homeomorphism của G lên G. Với mọi hàm $f$ trên G, ta định nghĩa hàm $\check{f}$ trên G bởi

$$
(12) \quad \check{f}(x) = f(x^{-1}).
$$

Với mọi độ đo $\mu$ trên G, ta định nghĩa độ đo $\check{\mu}$ bởi

$$
(13) \quad \check{\mu}(f) = \mu(\check{f}) \quad \text{cho } f \in \mathcal{K}(G).
$$

Nói cách khác,

$$
(14) \quad \int_G f(x)\,d\check{\mu}(x) = \int_G f(x^{-1})\,d\mu(x).
$$

Nếu A là một tập khả tích theo $\check{\mu}$, thì $A^{-1}$ khả tích theo $\mu$ và

$$
(15) \quad \check{\mu}(A) = \mu(A^{-1}).
$$

Chúng ta đồng ý viết $d\mu(x^{-1})$ thay cho $d\check{\mu}(x)$, và (14) khi đó có dạng

$$
\int_G f(x)\, d\mu(x^{-1}) = \int_G f(x^{-1})\, d\mu(x).
$$

### 2. Định lý tồn tại và duy nhất

#### Định nghĩa 2 {#int-vii-s1-def-2 .statement}

*Cho G là một nhóm locally compact. Một độ đo dương khác không trên G mà bất biến trái (resp. phải) được gọi là một độ đo Haar trái (resp. phải) trên G.*

#### Định lý 1 {#int-vii-s1-thm-1 .statement}

*Trên mọi nhóm locally compact, tồn tại một độ đo Haar trái (resp. phải), và, cho đến một thừa số hằng, chỉ có một.*

A) *Tồn tại.* — Đặt $\mathcal{K}(G) = \mathcal{K}$, $\mathcal{K}_+(G) = \mathcal{K}_+$, $\mathcal{K}_+^* = \mathcal{K}_+ - \{0\}$. Nếu C là một tập con compact của G, ta ký hiệu bởi $\mathcal{K}_+^*(C)$ tập các $f \in \mathcal{K}_+^*$ có giá đỡ trong C. Với $f \in \mathcal{K}$ và $g \in \mathcal{K}_+^*$, tồn tại các số $c_1, \ldots, c_n \geq 0$ và các phần tử $s_1, \ldots, s_n$ của G sao cho $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$: quả vậy, tồn tại một tập mở khác rỗng U trong G sao cho $\inf_{s \in U} g(s) > 0$, và giá đỡ của $f$ có thể được phủ bởi một số hữu hạn các ảnh tịnh tiến trái của U. Cho $(f : g)$ là cận dưới đúng của các số $\sum_{i=1}^n c_i$ đối với mọi hệ $(c_1, \ldots, c_n, s_1, \ldots, s_n)$ các số $\geq 0$ và các phần tử của G sao cho $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$. Khi đó:

(i) $(\gamma(s)f : g) = (f : g)$ với $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$, $s \in G$;
(ii) $(\lambda f : g) = \lambda(f : g)$ với $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$, $\lambda \geq 0$;
(iii) $((f + f') : g) \leq (f : g) + (f' : g)$ với $f \in \mathcal{K}$, $f' \in \mathcal{K}$, $g \in \mathcal{K}_+^*$;
(iv) $(f : g) \geq (\sup f)/(\sup g)$ với $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$;
(v) $(f : h) \leq (f : g)(g : h)$ với $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$, $h \in \mathcal{K}_+^*$;
(vi) $0 < \frac{1}{(f_0 : f)} \leq \frac{(f : g)}{(f_0 : g)} \leq (f : f_0)$ với $f, f_0, g$ trong $\mathcal{K}_+^*$;
(vii) cho $f, f', h$ thuộc $\mathcal{K}_+$ với $h(s) \geq 1$ trên hỗ trợ của $f + f'$, và cho $\varepsilon > 0$; tồn tại một lân cận compact V của e sao cho, với mọi $g \in \mathcal{K}_+^*(V)$,

$$
(f : g) + (f' : g) \leq ((f + f') : g) + \varepsilon(h : g).
$$

Các tính chất (i), (ii), (iii) là hiển nhiên. Cho $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$; nếu $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ với $c_i \geq 0$, thì $\sup f \leq \sum_{i=1}^n c_i g(s_i^{-1}s)$ với một số s \in G, do đó $\sup f \leq (\sum_{i=1}^n c_i) \sup g$, suy ra (iv). Bây giờ chứng minh (v); cho $f \in \mathcal{K}$, $g, h$ trong $\mathcal{K}_+^*$; nếu $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ và $g \leq \sum_{j=1}^p d_j \gamma(t_j)h$ ($c_i \geq 0, d_j \geq 0, s_i, t_j$ trong $G$), thì $f \leq \sum_{i,j} c_i d_j \gamma(s_i t_j)h$, do đó $(f : h) \leq \sum_{i,j} c_i d_j = (\sum_i c_i)(\sum_j d_j)$; vậy $(f : h) \leq (f : g)(g : h)$. Áp dụng (v) cho $f_0, f, g$ một mặt và cho $f, f_0, g$ mặt khác, suy ra (vi). Cuối cùng, cho $f, f', h$ thuộc $\mathcal{K}_+$ với $h(s) \geq 1$ trên giá đỡ của $f + f'$, và cho $\varepsilon > 0$. Đặt $F = f + f' + \frac{1}{2} \varepsilon h$; các hàm $\varphi, \varphi'$, trùng nhau lần lượt với $f/F$ và $f'/F$ trên giá đỡ của $f + f'$ và bằng không ở ngoài đó, thuộc $\mathcal{K}_+$; với mọi $\eta > 0$, tồn tại một lân cận compact $V$ của $e$ sao cho $|\varphi(s) - \varphi(t)| \leq \eta$ và $|\varphi'(s) - \varphi'(t)| \leq \eta$ khi $s^{-1} t \in V$. Khi đó cho $g \in \mathcal{K}_+^*(V)$; với mọi $s \in G$,

$$
\varphi \cdot \gamma(s)g \leq (\varphi(s) + \eta) \cdot \gamma(s)g;
$$

vì điều này hiển nhiên tại các điểm mà $\gamma(s)g$ bằng không, do đó ở ngoài $sV$; và trên $sV$, $\varphi \leq \varphi(s) + \eta$; tương tự, $\varphi' \cdot \gamma(s)g \leq (\varphi'(s) + \eta) \cdot \gamma(s)g$. Nói như vậy, cho $c_1, \ldots, c_n$ là các số $\geq 0$ và $s_1, \ldots, s_n$ là các phần tử của $G$ sao cho $F \leq \sum_{i=1}^n c_i \gamma(s_i)g$; khi đó

$$
f = \varphi F \leq \sum_{i=1}^n c_i \varphi \cdot \gamma(s_i)g \leq \sum_{i=1}^n c_i (\varphi(s_i) + \eta) \cdot \gamma(s_i)g
$$

và tương tự cho $f'$; do đó

$$
(f : g) + (f' : g) \leq \sum_{i=1}^n c_i (\varphi(s_i) + \varphi'(s_i) + 2\eta) \leq (1 + 2\eta) \sum_{i=1}^n c_i
$$

vì $\varphi + \varphi' \leq 1$. Áp dụng định nghĩa của $F$, rồi đến (ii), (iii) và (v), suy ra rằng

$$
(f : g) + (f' : g) \leq (1 + 2\eta)(F : g) \leq
$$
$$
(1 + 2\eta)[((f + f') : g) + \frac{1}{2}\varepsilon(h : g)] \leq
$$
$$
(((f + f') : g) + \frac{1}{2}\varepsilon(h : g) + 2\eta((f + f') : h)(h : g) + \varepsilon\eta(h : g)
$$

và, nếu $\eta$ đã được chọn sao cho $\eta[2((f + f') : h) + \varepsilon] \leq \frac{1}{2}\varepsilon$, thì suy ra (vii).

Khi $\mathcal{K}_+^*(V)$ chạy qua tập hợp các lân cận compact của e, thì các $\mathcal{K}_+^*(V)$ tạo thành một cơ sở của một bộ lọc $\mathcal{B}$ trên $\mathcal{K}_+^*$. Cho $\mathcal{F}$ là một siêu bộ lọc trên $\mathcal{K}_+^*$ mịn hơn $\mathcal{B}$. Mặt khác, hãy cố định $f_0 \in \mathcal{K}_+^*$ và hãy đặt, với $f \in \mathcal{K}_+^*$ và $g \in \mathcal{K}_+^*$,

$$
I_g(f) = \frac{(f : g)}{(f_0 : g)}.
$$

Theo (vi), $\lim_{g,\mathcal{F}} I_g(f) = I(f)$ tồn tại trong không gian compact $[1/(f_0 : f), (f : f_0)]$.

Theo (iii), $I(f + f') \leq I(f) + I(f')$. Theo (vii), $I(f) + I(f') \leq I(f + f') + \varepsilon I(h)$ với mọi $\varepsilon > 0$ miễn là $h$ là $\geq 1$ trên giá của $f + f'$; suy ra $I(f + f') = I(f) + I(f')$. Theo Ch. II, §2, No. 1, ĐL. 2, I có thể được mở rộng thành một dạng tuyến tính trên $\mathcal{K}$; dạng tuyến tính này là một độ đo dương khác không trên G, bất biến trái theo (i); đó là độ đo Haar trái cần tìm. Chuyển qua nhóm đối, từ đó suy ra sự tồn tại của một độ đo Haar phải.

B) *Tính duy nhất.* — Cho $\mu$ là một độ đo Haar trái, $\nu$ là một độ đo Haar phải. Khi đó $\check{\nu}$ là một độ đo Haar trái. Ta sẽ chứng minh rằng $\mu$ và $\check{\nu}$ tỉ lệ với nhau. Điều này sẽ chứng tỏ rằng bất kỳ hai độ đo Haar trái nào cũng thật vậy tỉ lệ với nhau.

Cho $f \in \mathcal{K}$ sao cho $\mu(f) \neq 0$. Theo Bổ đề 1, hàm $D_f$ được xác định trên G bởi công thức

$$
D_f(s) = \mu(f)^{-1} \int f(t^{-1}s) d\nu(t)
$$

là liên tục trên G. Cho $g \in \mathcal{K}$. Hàm $(s, t) \mapsto f(s)g(ts)$ liên tục và có giá compact trong $G \times G$. Theo Ch. III, §4, No. 1, ĐL. 2,

$$
\begin{align*}
\mu(f)\nu(g) &= \left( \int f(s) d\mu(s) \right) \left( \int g(t) d\nu(t) \right) \\
&= \int d\mu(s) \int f(s)g(ts) d\nu(t) = \int d\nu(t) \int f(s)g(ts) d\mu(s) \\
&= \int d\nu(t) \int f(t^{-1}s)g(s) d\mu(s) \\
&= \int g(s) \left[ \int f(t^{-1}s) d\nu(t) \right] d\mu(s) = \mu(g \cdot \mu(f) D_f),
\end{align*}
$$

do đó

$$
\nu(g) = \mu(D_f \cdot g).
$$

Điều này trước hết chứng minh rằng $D_f$ không phụ thuộc vào $f$. Thật vậy, nếu $f' \in \mathcal{K}$ sao cho $\mu(f') \neq 0$, thì $D_f \cdot \mu = D_{f'} \cdot \mu$, do đó $D_f = D_{f'}$ gần như khắp nơi địa phương đối với $\mu$, nên khắp nơi, vì $D_f$ và $D_{f'}$ là liên tục và giá đỡ của $\mu$ là $G$. Vì thế ta có thể viết $D_f = D$. Công thức (16) cho

$$
\mu(f)D(e) = \check{\nu}(f).
$$

Công thức (19) có thể được mở rộng theo tính tuyến tính cho các hàm $f \in \mathcal{K}$ sao cho $\mu(f) = 0$. Ta có $D(e) \neq 0$ vì $\check{\nu} \neq 0$. Điều này quả thực thiết lập tính tỉ lệ của $\mu$ và $\check{\nu}$.

#### Hệ quả {#int-vii-s1-n2-cor-1 .statement}

— *Mọi độ đo bất biến trái* (resp. *bất biến phải*) *trên* $G$ *đều tỉ lệ với một độ đo Haar trái* (resp. *phải*).

#### Ví dụ {#int-vii-s1-n2-exa-1 .statement}

— 1) Trên nhóm cộng $\mathbf{R}$, độ đo Lebesgue $dx$ là một độ đo Haar (Ch. III, §1, No. 3, *Ví dụ*).

2) Với mọi hàm $f \in \mathcal{K}(\mathbf{R}_+^*)$, ta có (FRV, II, §1, công thức (12))

$$
\int_0^{+\infty} \frac{f(x)}{x} dx = \int_0^{+\infty} \frac{f(tx)}{tx} t dx = \int_0^{+\infty} \frac{f(tx)}{x} dx
$$

với mọi $t > 0$; độ đo $x^{-1} dx$ như vậy là một độ đo Haar trên nhóm nhân $\mathbf{R}_+^*$.

3) Lấy xuyến $T = \mathbf{R}/\mathbf{Z}$ làm $G$. Cho $\varphi$ là ánh xạ chính tắc của $\mathbf{R}$ lên $T$. Với $f \in \mathcal{K}(T)$, hàm $f \circ \varphi$ liên tục và tuần hoàn với chu kỳ 1 trên $\mathbf{R}$, và tích phân

$$
I(f) = \int_a^{a+1} f(\varphi(x)) dx
$$

không phụ thuộc vào lựa chọn $a \in \mathbf{R}$; hiển nhiên nó bất biến dưới phép tịnh tiến; do đó nó xác định một độ đo Haar trên $T$. Nhờ phép chuyển cấu trúc, suy ra từ đó rằng $I(f) = \int_a^{a+1} f(e^{2\pi i t}) dt$ là một độ đo Haar trên nhóm nhân $U$ của các số phức có giá trị tuyệt đối bằng 1 (GT, VIII, §2, No. 1).

#### Mệnh đề 2 {#int-vii-s1-prop-2 .statement}

— *Cho* $G$ *là một nhóm địa phương compact*, $\mu$ *là một độ đo Haar trái hoặc phải trên* $G$. *Để* $G$ *rời rạc, điều kiện cần và đủ là* $\mu(\{e\}) > 0$. *Để* $G$ *compact, điều kiện cần và đủ là* $\mu^*(G) < +\infty$.

Các điều kiện là hiển nhiên cần thiết. Ta chứng minh tính đủ của chúng. Cho $V$ là một lân cận compact của $e$. Nếu $\mu(\{e\}) > 0$, thì $V$ là một tập hợp hữu hạn vì $\mu(V) < +\infty$; do $G$ là Hausdorff, nên $G$ rời rạc. Giả sử $\mu^*(G) < +\infty$ và $\mu$ chẳng hạn bất biến trái. Xét tập hợp $\mathcal{E}$ gồm các tập hợp con hữu hạn $\{s_1, \ldots, s_n\}$ của $G$ sao cho $s_i V \cap s_j V = \varnothing$ với $i \neq j$; khi đó

$$
n \mu(V) = \mu(s_1 V \cup \ldots \cup s_n V) \leq \mu^*(G),
$$

do đó $n \leq \mu^*(G)/\mu(V)$. Vì vậy ta có thể chọn trong $\mathcal{E}$ một phần tử cực đại $\{s_1, \ldots, s_n\}$. Khi đó, với mọi $s \in G$, tồn tại một $i$ sao cho $s V \cap s_i V \neq \varnothing$, tức là sao cho $s \in s_i V V^{-1}$. Vậy $G$ là hợp của các tập hợp compact $s_i V V^{-1}$, nên compact.

### 3. Môđun

Cho $\mu$ là một độ đo Haar trái trên $G$. Với mọi $s \in G$, $\delta(s)\mu$ cũng bất biến trái (No. 1, công thức (11)), do đó (Định lý 1) tồn tại một số duy nhất $\Delta_G(s) > 0$ sao cho $\delta(s)\mu = \Delta_G(s)\mu$. Nhờ Định lý 1, số $\Delta_G(s)$ không phụ thuộc vào lựa chọn của $\mu$.

#### Định nghĩa 3 {#int-vii-s1-def-3 .statement}

*Hàm $\Delta_G$ trên $G$ được gọi là môđun (hay hàm môđun) của $G$. Nếu $\Delta_G = 1$, thì nhóm $G$ được gọi là đơn môđula.*

Cũng có thể nói rằng $\mu$ là tương đối bất biến phải với nhân tử $\Delta_G$. Do đó $\Delta_G$ là một *biểu diễn liên tục của $G$ trong $\mathbf{R}_+^*$* (No. 1, Mệnh đề 1).

#### Nhận xét {#int-vii-s1-n3-rem-1 .statement}

— Nếu $\varphi$ là một đẳng cấu của $G$ lên một nhóm địa phương compact $G'$, thì $\Delta_{G'} \circ \varphi = \Delta_G$. Đặc biệt:
1) Vì $x \mapsto x^{-1}$ là một đẳng cấu của $G$ lên nhóm đối $G^0$, ta có $\Delta_{G^0} = \Delta_G^{-1}$.
2) Nếu $\varphi$ là một tự đẳng cấu của $G$, thì $\Delta_G \circ \varphi = \Delta_G$.

Cho $s \in G$. Khi đó:

$$
\delta(s)(\Delta_G^{-1} \cdot \mu) = (\delta(s)\Delta_G^{-1}) \cdot (\delta(s)\mu) = (\Delta_G(s)^{-1}\Delta_G^{-1}) \cdot (\Delta_G(s)\mu) = \Delta_G^{-1} \cdot \mu,
$$

do đó $\Delta_G^{-1} \cdot \mu = \mu'$ là một độ đo Haar phải. Từ đó, suy ra rằng $\gamma(s)\mu' = (\gamma(s)\Delta_G^{-1}) \cdot \mu = \Delta_G(s)(\Delta_G^{-1} \cdot \mu) = \Delta_G(s)\mu'$, do đó, với mọi độ đo Haar phải $\nu$, ta có $\gamma(s)\nu = \Delta_G(s)\nu$. Vì $\dot{\mu}$ là một độ đo Haar phải, $\dot{\mu} = a \Delta_G^{-1} \cdot \mu$ với một hằng số $a > 0$; suy ra rằng

$$
\mu = a(\Delta_G^{-1} \cdot \mu)^{\vee} = a \Delta_G \cdot \dot{\mu} = a^2 \mu,
$$

do đó $a = 1$ và cuối cùng $\dot{\mu} = \Delta_G^{-1} \cdot \mu$. Ta thấy tương tự rằng $\dot{\nu} = \Delta_G \cdot \nu$.

Do đó ta có các kết quả sau:

Bảng công thức. — Cho G là một nhóm địa phương compact, $\Delta$ là môđun của nó, $\mu$ là một độ đo Haar trái, và $\nu$ là một độ đo Haar phải.

1) Ta có

$$
\gamma(s)\mu = \mu \quad \delta(s)\mu = \Delta(s)\mu \quad \check{\mu} = \Delta^{-1} \cdot \mu .
$$

Nếu $f$ là khả tích theo $\mu$ trên G, thì các phép tịnh tiến trái và phải của $f$ là khả tích theo $\mu$, và

$$
\int f(sx)\, d\mu(x) = \int f(x)\, d\mu(x)
$$
(21)
$$
\int f(xs)\, d\mu(x) = \Delta(s)^{-1} \int f(x)\, d\mu(x) .
$$

Hơn nữa, $\check{f}$ khả tích đối với $\Delta^{-1} \cdot \mu$ và

$$
\int f(x^{-1})\Delta(x)^{-1}\, d\mu(x) = \int f(x)\, d\mu(x) .
$$
(22)

Nếu A là một tập con khả tích theo $\mu$ của G, thì sA và As là khả tích theo $\mu$ và

$$
\mu(sA) = \mu(A) \qquad \mu(As) = \Delta(s)\mu(A) .
$$
(23)

2) Ta có

$$
\delta(s)\nu = \nu \quad \gamma(s)\nu = \Delta(s)\nu \quad \check{\nu} = \Delta \cdot \nu .
$$

Nếu $f$ là khả tích theo $\nu$ trên G, thì các phép tịnh tiến trái và phải của $f$ là khả tích theo $\nu$ và

$$
\int f(xs)\, d\nu(x) = \int f(x)\, d\nu(x)
$$
(25)
$$
\int f(xs)\, d\nu(x) = \Delta(s) \int f(x)\, d\nu(x) .
$$

Hơn nữa, $\check{f}$ khả tích đối với $\Delta \cdot \nu$ và

$$
\int f(x^{-1})\Delta(x)\, d\nu(x) = \int f(x)\, d\nu(x) .
$$
(26)

Nếu A là một tập con khả tích theo $\nu$ của G, thì sA và As là khả tích theo $\nu$ và

$$
\nu(As) = \nu(A) \qquad \nu(sA) = \Delta(s)^{-1} \nu(A) .
$$
(27)

3) $\nu$ tỉ lệ với $\Delta^{-1} \cdot \mu$, và $\mu$ tỉ lệ với $\Delta \cdot \nu$.

4) Giả sử G là *đơn môđula*. Cho $\mu$ là một độ đo Haar trên G. Khi đó:

$$
\gamma(s)\mu = \delta(s)\mu = \dot{\mu} = \mu .
$$

Nếu $f$ là một hàm $\mu$-khả tích trên G, thì các phép tịnh tiến trái và phải của $f$ đều $\mu$-khả tích, cũng như $\check{f}$, và

$$
\int f(sx)\,d\mu(x) = \int f(xs)\,d\mu(x) = \int f(x^{-1})\,d\mu(x) = \int f(x)\,d\mu(x) .
$$

Nếu A là một tập con $\mu$-khả tích của G, thì sA, As và $A^{-1}$ đều $\mu$-khả tích và

$$
\mu(sA) = \mu(As) = \mu(A^{-1}) = \mu(A) .
$$

Các tính chất tương tự đúng đối với tích phân cốt yếu.

#### Mệnh đề 3 {#int-vii-s1-prop-3 .statement}

*Nếu trong G tồn tại một lân cận compact V của e bất biến dưới các tự đẳng cấu trong, thì G là đơn môđula.*

Thật vậy, cho $\mu$ là một độ đo Haar trái trên G. Với mọi $s \in G$,

$$
\mu(V) = \mu(s^{-1}Vs) = \Delta_G(s)\mu(V) ,
$$

suy ra $\Delta_G(s) = 1$ vì $0 < \mu(V) < +\infty$.

Từ đó, suy ra ngay:

#### Hệ quả {#int-vii-s1-n3-cor-1 .statement}

*Nếu G là rời rạc, hoặc compact, hoặc giao hoán, thì G là đơn môđula.*

Điều này hơn nữa là tầm thường khi G *giao hoán*. Chú ý thêm rằng nếu G *rời rạc*, thì độ đo trên G sao cho mỗi điểm có khối lượng 1 hiển nhiên là một độ đo Haar trái và phải trên G, gọi là độ đo Haar *chuẩn hóa* trên G. Nếu G *compact*, thì tồn tại một và chỉ một độ đo Haar trên G sao cho $\mu(G) = 1$; nó được gọi là độ đo Haar *chuẩn hóa* của G. Hai quy ước trên không phù hợp với nhau khi G vừa rời rạc vừa compact, tức là hữu hạn; trong trường hợp này ta sẽ luôn nói tường minh ý nghĩa của độ đo Haar chuẩn hóa.

Các nhóm con và các nhóm thương của một nhóm đơn môđula không phải luôn luôn đơn môđula (\S 2, Bài tập 5). Tuy nhiên, xem Mệnh đề 10 của \S 2, Mục 7.

*Sau này ta sẽ thấy rằng các nhóm Lie liên thông nửa đơn hoặc lũy linh là đơn môđula.*

### 4. Môđun của một tự đẳng cấu

Cho G là một nhóm địa phương compact, $\varphi$ là một tự đẳng cấu của G, và $\mu$ là một độ đo Haar trái trên G. Hiển nhiên $\varphi^{-1}(\mu)$ cũng là một độ đo Haar trái trên G. Do đó tồn tại (Mục 2, Định lý 1) một và chỉ một số $a > 0$ sao cho $\varphi^{-1}(\mu) = a \mu$. Theo Mục 2, Định lý 1, số này không phụ thuộc vào lựa chọn của $\mu$. Chú ý rằng nếu ta bắt đầu với một độ đo Haar phải, chẳng hạn $\Delta_G^{-1} \cdot \mu$ (Mục 3), thì cũng sẽ thu được cùng một vô hướng $a$: vì, do $\varphi^{-1}$ để bất biến $\Delta_G$ (Mục 3, Chú ý), ta có $\varphi^{-1}(\Delta_G^{-1} \cdot \mu) = \Delta_G^{-1} \cdot \varphi^{-1}(\mu) = a \Delta_G^{-1} \cdot \mu$.

#### Định nghĩa 4 {#int-vii-s1-def-4 .statement}

*Số $a > 0$ sao cho $\varphi^{-1}(\mu) = a \mu$ được gọi là môđun của tự đẳng cấu $\varphi$ và được ký hiệu $\operatorname{mod}_G \varphi$ hoặc đơn giản là $\operatorname{mod} \varphi$. \*

Nếu $f$ là một hàm $\mu$-khả tích trên G, thì

$$
\int f(\varphi^{-1}(x)) d\mu(x) = (\operatorname{mod} \varphi) \int f(x) d\mu(x).
$$

Nếu A là một tập con $\mu$-khả tích của G, thì

$$
\mu(\varphi(A)) = (\operatorname{mod} \varphi) \mu(A).
$$

Đặc biệt, với $s \in G$, đặt $i_s$ là tự đẳng cấu trong $x \mapsto s^{-1} x s$. Khi đó $i_s^{-1} = \delta(s) \gamma(s)$, do đó

$$
i_s^{-1}(\mu) = \delta(s) \mu = \Delta_G(s) \mu,
$$

do đó

$$
\operatorname{mod} i_s = \Delta_G(s).
$$

Nếu G hoặc rời rạc hoặc compact, thì độ đo Haar chuẩn hóa của nó được mọi tự đẳng cấu $\varphi$ của G biến thành chính nó, như ta thấy ngay bằng phép chuyển cấu trúc. Vì vậy *một tự đẳng cấu của một nhóm rời rạc hoặc compact có môđun bằng 1*.

#### Mệnh đề 4 {#int-vii-s1-prop-4 .statement}

*Cho G là một nhóm địa phương compact, $\Gamma$ là một nhóm tôpô, và $\gamma \mapsto u_\gamma$ là một đồng cấu từ $\Gamma$ vào nhóm $\mathcal{G}$ các tự đẳng cấu của G, sao cho $(\gamma, x) \mapsto u_\gamma(x)$ là một ánh xạ liên tục từ $\Gamma \times G$ vào G. Khi đó, ánh xạ $\gamma \mapsto \operatorname{mod}(u_\gamma)$ là một biểu diễn liên tục của $\Gamma$ trong $\mathbf{R}_+^*$. \*

Đây hiển nhiên là một biểu diễn (đại số) của $\Gamma$ trong $\mathbf{R}_+^*$; chỉ cần chứng minh tính liên tục của nó. Cho $f \in \mathcal{K}(G)$ và gọi S là giá đỡ của nó.*

Cho $\gamma_0 \in \Gamma$ và cho $U$ là một láng giềng tương đối compact của $u_{\gamma_0}^{-1}(S)$. Ánh xạ $\gamma \mapsto u_\gamma$ là một ánh xạ liên tục từ $\Gamma$ vào $\mathcal{G}$ được trang bị tôpô hội tụ compact (GT, X, §3, No. 4, Th. 3); do đó $u_\gamma^{-1}(S) \subset U$ với $\gamma$ đủ gần $\gamma_0$. Bổ đề 1 của No. 1 khi đó chứng minh rằng $\int f(u_\gamma(x)) d\mu(x)$ (trong đó $\mu$ ký hiệu một độ đo Haar trái của $G$) phụ thuộc liên tục vào $\gamma$; do đó mệnh đề.

### 5. Độ đo Haar của một tích

#### Mệnh đề 5 {#int-vii-s1-prop-5 .statement}

— *Cho* $(G_\iota)_{\iota \in I}$ *là một họ các nhóm địa phương compact*. *Với mọi* $\iota \in I$ *gọi* $\mu_\iota$ *là một độ đo Haar trái (resp. phải) trên* $G_\iota$. *Giả sử tồn tại một tập con hữu hạn* $J$ *của* $I$ *sao cho, với mọi* $\iota \in I - J$, $G_\iota$ *là compact và* $\mu_\iota(G_\iota) = 1$. *Khi đó độ đo tích* $\bigotimes_{\iota \in I} \mu_\iota$ *là một độ đo Haar trái (resp. phải) trên* $G = \prod_{\iota \in I} G_\iota$. *Nếu* $x = (x_\iota) \in G$ *thì*
$$
\Delta_G(x) = \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota).
$$
Đối với mọi tập con hữu hạn $J$ của $I$, $\bigotimes_{\iota \in J} \mu_\iota$ là một độ đo Haar trái (resp. phải) trên $\prod_{\iota \in J} G_\iota$, như suy ra ngay lập tức từ các định nghĩa. Do đó $\bigotimes_{\iota \in I} \mu_\iota$ là một độ đo Haar trái (resp. phải) trên $G$ (Ch. III, §4, No. 6, Prop. 9). Mặt khác, nếu các $\mu_\iota$ là các độ đo Haar trái thì
$$
\delta(x) \left( \bigotimes_{\iota \in I} \mu_\iota \right) = \bigotimes_{\iota \in I} \delta(x_\iota) \mu_\iota = \bigotimes_{\iota \in I} (\Delta_{G_\iota}(x_\iota) \mu_\iota) = \left( \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota) \right) \bigotimes_{\iota \in I} \mu_\iota,
$$
suy ra $\Delta_G(x) = \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota)$.

#### Ví dụ {#int-vii-s1-n5-exa-1 .statement}

— 1) Độ đo Lebesgue trên $\mathbf{R}^n$ là một độ đo Haar của nhóm cộng $\mathbf{R}^n$.

2) Ánh xạ $(r, u) \mapsto ru$ là một đẳng cấu từ $\mathbf{R}_+^* \times \mathbf{U}$ lên $\mathbf{C}^*$ (GT, VIII, §1, No. 3). Nếu $\mathbf{C}^*$ được đồng nhất với $\mathbf{R}_+^* \times \mathbf{U}$ nhờ đẳng cấu này, và nếu $du$ ký hiệu một độ đo Haar trên $\mathbf{U}$, thì $r^{-1} dr du$ là một độ đo Haar trên $\mathbf{C}^*$ theo Ví dụ 2 của No. 2. Mặt khác, song ánh $\theta \mapsto e^{2i\pi \theta}$ của $[0, 1[$ lên $\mathbf{U}$ biến độ đo Lebesgue $d\theta$ trên $[0, 1[$ thành một độ đo Haar trên $\mathbf{U}$ theo Ví dụ 3 của No. 2. Suy ra rằng nếu $f \in \mathcal{H}(\mathbf{C}^*)$, thì tích phân
$$
\int_0^{+\infty} \int_0^1 f(re^{2i\pi \theta}) r^{-1} dr\, d\theta
$$
xác định một độ đo Haar trên $\mathbf{C}^*$.

### 6. Độ đo Haar của một giới hạn ngược*

Khi đó, giới hạn ngược của hệ ngược $(G_\alpha, \varphi_{\beta \alpha})$ có thể được đồng nhất với G, và ánh xạ chính tắc của giới hạn ngược này vào $G_\alpha$ được đồng nhất với $\varphi_\alpha$ (GT, III, §7, No. 3, Mệnh đề 2). Các ánh xạ $\varphi_\alpha$ và $\varphi_{\beta \alpha}$ là riêng (*loc. cit.*, §4, No. 1, Hệ quả 2 của Mệnh đề 1). Các giả thiết này được giữ cố định trong suốt tiểu mục này.

\* Bổ đề 2. — a) *Cho $f \in \mathcal{K}_+(G)$, S là một tập con compact của G chứa giá đỡ $f$, U là một lân cận mở của S trong G, và $\varepsilon > 0$. Tồn tại một $\alpha \in A$ và một hàm $g \in \mathcal{K}_+(G)$, bằng không ở ngoài U và hằng trên các lớp kề của $K_\alpha$, sao cho $|f - g| \leq \varepsilon$.

b) *Cho $\mu$ và $\mu'$ là hai độ đo trên G sao cho $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ với mọi $\alpha \in A$. Khi đó $\mu = \mu'$.

Tồn tại một $\alpha_1 \in A$ sao cho $K_{\alpha_1} S \cap K_{\alpha_1}(G - U) = \emptyset$ (GT, II, §4, No. 3, Mệnh đề 4). Sau khi nới rộng S và thu hẹp U, do đó ta có thể giả sử rằng S và U là các hợp của các lớp kề của $K_{\alpha_1}$. Xét các hàm số thực liên tục $h$ trên S có tính chất sau: tồn tại một $\alpha \geq \alpha_1$ sao cho $h$ hằng trên các lớp kề của $K_\alpha$. Các hàm này tạo thành một đại số con của $\mathcal{K}(S)$ (vì $(K_\alpha)$ là một họ giảm có hướng) chứa các hằng số và phân biệt các điểm của S: thật vậy, cho $x, y$ là hai điểm phân biệt của S; vì giao của các $K_\alpha$ là $\{e\}$, tồn tại một $\alpha \geq \alpha_1$ sao cho $\varphi_\alpha(x) \neq \varphi_\alpha(y)$, rồi một hàm số thực liên tục $u$ trên $\varphi_\alpha(S)$ sao cho $u(\varphi_\alpha(x)) \neq u(\varphi_\alpha(y))$. Theo định lý Stone–Weierstrass, tồn tại một $\alpha \geq \alpha_1$ và một hàm liên tục $h \geq 0$ trên S, hằng trên các lớp kề của $K_\alpha$, sao cho $|f - h| \leq \frac{\varepsilon}{2}$ trên S. Với mọi $t \in \mathbf{R}$, đặt $\delta(t) = \left( t - \frac{\varepsilon}{2} \right)^+$, và đặt $h' = \delta \circ h$. Khi đó $h'$ là một hàm $\geq 0$, liên tục trên S, hằng trên các lớp kề của $K_\alpha$, và $|h - h'| \leq \frac{\varepsilon}{2}$ trên S, do đó $|f - h'| \leq \varepsilon$ trên S. Mặt khác, $h'(x) = 0$ nếu x thuộc biên của S trong G, vì khi đó $h(x) \leq \frac{\varepsilon}{2}$. Nếu mở rộng $h'$ bằng 0 trên phần bù của S, ta thu được một hàm $g$ thỏa các yêu cầu, do đó chứng minh a).

Giả sử $\mu, \mu'$ là hai độ đo trên G sao cho $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ với mọi $\alpha \in A$. Cho $v \in \mathcal{K}(G)$ là một hàm hằng trên các lớp kề của $K_\alpha$ với một $\alpha \in A$ nào đó, để ta có thể viết $v = w \circ \varphi_\alpha$ với $w \in \mathcal{K}(G_\alpha)$; khi đó

\* Xem Ch. III, §4, No. 5.

$$
\mu(v) = (\varphi_\alpha(\mu))(w) = (\varphi_\alpha(\mu'))(w) = \mu'(v); \text{ suy ra } \mu = \mu' \text{ theo a)}.
$$

#### Mệnh đề 6 {#int-vii-s1-prop-6 .statement}

*Với mọi* $\alpha \in A$, *hãy cho* $\mu_\alpha$ *là một độ đo dương trên* $G_\alpha$. *Giả sử rằng* $\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta$ *khi* $\alpha \geq \beta$. *Khi đó, tồn tại một và chỉ một độ đo dương* $\mu$ *trên* $G$ *sao cho* $\varphi_\alpha(\mu) = \mu_\alpha$ *với mọi* $\alpha \in A$.

Tính duy nhất suy ra ngay từ Bổ đề 2 b). Hãy chứng minh sự tồn tại của $\mu$. Cho $V$ là không gian vectơ các hàm thuộc $\mathcal{K}(G)$ và hằng trên các lớp kề của một $K_\alpha$ nào đó ($\alpha$ có thể phụ thuộc vào hàm). Từ Bổ đề 2 a) suy ra rằng $V$ thỏa điều kiện (P) của Ch. III, §1, No. 7, Mệnh đề 9: thật vậy, cho $K$ là một tập compact trong $G$ và chọn $f \in \mathcal{K}_+(G)$ sao cho $f(x) > 0$ với mọi $x \in K$; cho $a > 0$ là giá trị nhỏ nhất của $f$ trên $K$; theo Bổ đề 2 a), tồn tại một hàm $g \in V \cap \mathcal{K}_+(G)$ sao cho $|f - g| \leq a/2$, do đó $g(x) > 0$ với mọi $x \in K$, và điều kiện (P) được thỏa mãn. Cho $f \in V$. Tồn tại một $\alpha \in A$ sao cho $f$ hằng trên các lớp kề của $K_\alpha$. Bằng cách chuyển sang thương, $f$ xác định một hàm $f_\alpha \in \mathcal{K}(G_\alpha)$. Số $\mu(f) = \mu_\alpha(f_\alpha)$ không phụ thuộc vào lựa chọn $\alpha$: thật vậy, cho $\beta$ là bất kỳ chỉ số nào sao cho $f$ hằng trên các lớp kề của $K_\beta$; cho $\gamma \in A$ sao cho $\gamma \geq \alpha, \gamma \geq \beta$; khi đó $f$ xác định các hàm $f_\beta \in \mathcal{K}(G_\beta)$, $f_\gamma \in \mathcal{K}(G_\gamma)$ sao cho $f = f_\beta \circ \varphi_\beta = f_\gamma \circ \varphi_\gamma$; khi đó $f_\alpha \circ \varphi_{\alpha\gamma} = f_\gamma$, do đó $\mu_\gamma(f_\gamma) = (\varphi_{\alpha\gamma}(\mu_\gamma))(f_\alpha) = \mu_\alpha(f_\alpha)$, và tương tự $\mu_\gamma(f_\gamma) = \mu_\beta(f_\beta)$, suy ra mệnh đề đã nêu. Điều đó đã được thiết lập, hiển nhiên $\mu$ là một dạng tuyến tính trên $V$ và $\mu(f) \geq 0$ khi $f \geq 0$. Theo Mệnh đề 9 của Ch. III, §1, No. 7, $\mu$ có thể được mở rộng thành một độ đo dương trên $G$, mà ta lại ký hiệu là $\mu$. Ta có $\varphi_\alpha(\mu) = \mu_\alpha$ với mọi $\alpha \in A$ theo chính phép dựng của $\mu$.

#### Định nghĩa 5 {#int-vii-s1-def-5 .statement}

*Độ đo* $\mu$ *được gọi là giới hạn ngược (hoặc giới hạn xạ ảnh) của các* $\mu_\alpha$.

#### Mệnh đề 7 {#int-vii-s1-prop-7 .statement}

*Ta giữ các ký hiệu của Mệnh đề 6. Nếu mỗi* $\mu_\alpha$ *là một độ đo Haar trái (resp. phải) trên* $G_\alpha$, *thì* $\mu$ *là một độ đo Haar trái (resp. phải) trên* $G$.

Giả sử, chẳng hạn, rằng các $\mu_\alpha$ là các độ đo Haar trái. Cho $s \in G$. Với mọi $x \in G$,

$$
(\varphi_\alpha \circ \gamma(s))(x) = \varphi_\alpha(sx) = \varphi_\alpha(s)\varphi_\alpha(x) = (\gamma(\varphi_\alpha(s)) \circ \varphi_\alpha)(x);
$$

therefore $\varphi_\alpha(\gamma(s)\mu) = \gamma(\varphi_\alpha(s))\mu_\alpha = \mu_\alpha$. Do đó $\gamma(s)\mu = \mu$ theo Bổ đề 2 b), suy ra $\mu$ là một độ đo Haar trái.

Từ nay trở đi, ta giả sử các $K_\alpha$ không những compact, mà còn mở trong $G$. Khi đó các $G_\alpha$ là rời rạc và, với $\beta \geq \alpha$, $K_\alpha/K_\beta$ là một nhóm compact và rời rạc, do đó là hữu hạn. Nhóm $G$ là đơn môđula (Mệnh đề 3).

#### Mệnh đề 8 {#int-vii-s1-prop-8 .statement}

a) *Cho* $\mu$ *và* $\mu'$ *là hai độ đo dương trên* $G$ *sao cho, với mọi* $\alpha$ *và với mọi lớp ghép* $C$ *của* $K_\alpha$, $\mu(C) = \mu'(C)$. *Khi đó* $\mu = \mu'$.

b) *Cố định một* $\alpha_0 \in A$. *Với mọi* $\alpha \geq \alpha_0$ *gọi* $n_\alpha$ *là số phần tử của nhóm hữu hạn* $K_{\alpha_0}/K_\alpha$. *Tồn tại một và chỉ một độ đo dương* $\mu$ *trên* $G$ *sao cho, với mọi* $\alpha \geq \alpha_0$, *mỗi lớp ghép của* $K_\alpha$ *đều có độ đo* $n_\alpha^{-1}$. *Hơn nữa, $\mu$ là một độ đo Haar trên* $G$, *sao cho* $\mu(K_{\alpha_0}) = 1$.

Cho $\mu$ và $\mu'$ là hai độ đo dương trên $G$ thỏa mãn điều kiện a). Các điểm của nhóm rời rạc $G_\alpha$ khi đó có cùng độ đo đối với $\varphi_\alpha(\mu)$ và $\varphi_\alpha(\mu')$, do đó $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$, và điều này đúng với mọi $\alpha$. Vậy $\mu = \mu'$ (Bổ đề 2 b)).

Chứng minh b). Với mọi $\alpha \geq \alpha_0$, gọi $\mu_\alpha$ là độ đo Haar của nhóm rời rạc $G_\alpha$ sao cho mỗi điểm đều có độ đo $n_\alpha^{-1}$. Cho $\alpha, \beta$ sao cho $\alpha \geq \beta \geq \alpha_0$. Khi đó $K_\beta/K_\alpha$ có $n_\alpha/n_\beta$ phần tử. Do đó $\varphi_{\beta\alpha}(\mu_\alpha)$ là độ đo trên $G_\beta$ sao cho mỗi điểm đều có độ đo $n_\alpha^{-1} \cdot \frac{n_\alpha}{n_\beta} = n_\beta^{-1}$; nói cách khác, $\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta$. Khi đó chỉ cần áp dụng các Mệnh đề 6 và 7.

#### Ví dụ {#int-vii-s1-n6-exa-1 .statement}

— Cho $\mathbf{Q}_p$ là trường $p$-adic, tức là sự hoàn thành của $\mathbf{Q}$ theo giá trị tuyệt đối $p$-adic $|x|_p = p^{-v_p(x)}$ (GT, IX, §3, No. 2, *Ví dụ 3*). Các phần tử của $\mathbf{Q}_p$ được gọi là *các số* *$p$-adic*. Ta ký hiệu tiếp tục bởi $|x|_p$ phần mở rộng liên tục của giá trị tuyệt đối $p$-adic lên $\mathbf{Q}_p$. Ta có

$$
|x + y|_p \leq \sup(|x|_p, |y|_p)
$$

với $x, y$ trong $\mathbf{Q}$ (*loc. cit.*), do đó với $x, y$ trong $\mathbf{Q}_p$; hơn nữa, nếu $|y|_p < |x|_p$ thì $|x + y|_p = |x|_p$, vì $|x|_p = |(x + y) - y|_p \leq \sup(|x + y|_p, |y|_p)$. Nếu $(x_n)$ là một dãy các điểm của $\mathbf{Q}_p$ tiến tới $x \in \mathbf{Q}_p^*$, thì $|x - x_n|_p < |x|_p$ và $|x - x_n|_p < |x_n|_p$ với $n$ đủ lớn, do đó $|x|_p = |x_n|_p$. Điều này chứng tỏ rằng, với mọi $x \in \mathbf{Q}_p^*$, $|x|_p$ là một lũy thừa của $p$.

Cho $\mathbf{Z}_p$ là bao đóng của $\mathbf{Z}$ trong $\mathbf{Q}_p$; đây là một vành con của $\mathbf{Q}_p$; các phần tử của nó được gọi là các số nguyên *$p$*-*adic*. Ta có $|x|_p \leq 1$ với mọi $x \in \mathbf{Z}_p$. Ngược lại, cho $x$ là một phần tử của $\mathbf{Q}_p$ sao cho $|x|_p \leq 1$, và hãy chứng minh rằng $x \in \mathbf{Z}_p$; tồn tại một dãy $(x_n)$ các phần tử của $\mathbf{Q}$ tiến tới $x$, và $|x_n|_p \leq 1$ với $n$ đủ lớn theo điều đã thấy ở trên; chỉ cần chứng minh rằng $x_n$ thuộc $\mathbf{Z}_p$ với $n$ đủ lớn; nói cách khác, ta quy về trường hợp $x \in \mathbf{Q}$; khi đó $x = a/b$ với $b$ nguyên tố cùng nhau với $p$; với mọi số nguyên $n > 0$, tồn tại $b'_n \in \mathbf{Z}$ và $h_n \in \mathbf{Z}$ sao cho $bb'_n + h_n p^n = 1$, do đó $x = \frac{abb'_n + ah_n p^n}{b} = ab'_n + \frac{ah_n p^n}{b}$ và $|x - ab'_n|_p \leq p^{-n}$, vì vậy $ab'_n$ tiến tới $x$.

Từ đây suy ra rằng quả cầu đóng có tâm 0 và bán kính $p^{-n}$, trùng với quả cầu mở có tâm 0 và bán kính $p^{-n+1}$, là $p^n \mathbf{Z}_p$. Không gian tôpô $\mathbf{Q}_p$ do đó không chiều, suy ra hoàn toàn rời rạc (GT, IX, §6, No. 4).

Chúng ta hãy ցույց ra rằng các số nguyên $0, 1, \ldots, p^n - 1$ tạo thành một hệ đại diện của $\mathbf{Z}_p$ theo modulo $p^n \mathbf{Z}_p$. Trước hết, $|k - k'|_p > p^{-n}$ đối với hai số nguyên như thế $k$ và $k'$, do đó các lớp modulo $p^n \mathbf{Z}_p$ của các số nguyên này là phân biệt. Mặt khác, cho $x \in \mathbf{Z}_p$; tồn tại một $k \in \mathbf{Z}$ sao cho $|x - k|_p \leq p^{-n}$; cộng thêm vào $k$ một bội thích hợp của $p^n$, ta có thể giả sử rằng $k \in [0, p^n - 1]$, và $x$ đồng dư với $k$ modulo $p^n \mathbf{Z}_p$. Suy ra khẳng định của chúng ta. Điều đó cho thấy $\mathbf{Z}_p / p^n \mathbf{Z}_p$ đẳng cấu chính tắc với $\mathbf{Z}/p^n \mathbf{Z}$. Hơn nữa, ta thấy rằng $\mathbf{Z}_p$ là tiền compact, nên *compact* vì nó đầy đủ. Vì $\mathbf{Z}_p$ là một nhóm con mở của $\mathbf{Q}_p$, nên $\mathbf{Q}_p$ là *địa phương compact*. Tôpô của $\mathbf{Q}_p$ có một cơ sở đếm được (GT, IX, §2, No. 9, Hệ quả của Mệnh đề 16). Nhóm cộng $\mathbf{Q}_p$ có thể được đồng nhất với giới hạn ngược của các nhóm rời rạc $\mathbf{Q}_p / p^n \mathbf{Z}_p$.

Tồn tại một và chỉ một độ đo Haar $\alpha$ trên nhóm cộng $\mathbf{Q}_p$ sao cho $\alpha(\mathbf{Z}_p) = 1$; nó được gọi là *độ đo Haar chuẩn hóa* trên $\mathbf{Q}_p$. Vì $\mathbf{Z}_p$ là hợp của $p^n$ lớp kề rời nhau của $p^n \mathbf{Z}_p$ ($n$ là một số nguyên $\geq 0$), ta có $\alpha(p^n \mathbf{Z}_p) = p^{-n}$; tương tự $\alpha(p^{-n} \mathbf{Z}_p) = p^n$, do đó, cuối cùng, $\alpha(p^n \mathbf{Z}_p) = p^{-n}$ với mọi $n \in \mathbf{Z}$. Theo Mệnh đề 8 b), $\alpha$ là độ đo dương duy nhất trên $\mathbf{Q}_p$ sao cho mọi lớp kề của $p^n \mathbf{Z}_p$ ($n$ là một số nguyên $\geq 0$) đều có độ đo $p^{-n}$.

Hạn chế của $\alpha$ lên $\mathbf{Z}_p$ hiển nhiên là một độ đo Haar trên $\mathbf{Z}_p$.

### 7. Định nghĩa địa phương của một độ đo Haar

#### Mệnh đề 9 {#int-vii-s1-prop-9 .statement}

*Cho G là một nhóm địa phương compact, V là một tập con mở của G, và $\mu$ là một độ đo dương khác không trên V thỏa mãn tính chất sau: nếu U là một tập con mở của V và nếu s \in G sao cho sU \subset V, thì ảnh của độ đo $\mu_U$ cảm sinh bởi $\mu$ trên U, qua đồng phôi $x \mapsto sx$ của U lên sU, là $\mu_{sU}$. Khi đó, tồn tại một và chỉ một độ đo Haar trái $\alpha$ trên G cảm sinh $\mu$ trên V.*

Với mọi $s \in G$, cho $\mu_s$ là ảnh của $\mu$ qua phép đồng phôi $x \mapsto sx$ từ V lên sV. Hạn chế của $\mu_s$ lên $V \cap sV$ là ảnh của $\mu_{s^{-1}V \cap V}$ qua phép hạn chế của $x \mapsto sx$ lên $s^{-1}V \cap V$; theo giả thiết, ảnh này là $\mu_{V \cap sV}$. Bằng phép tịnh tiến, suy ra từ đó rằng $\mu_s$ và $\mu_t$ có cùng hạn chế lên $sV \cap tV$ với mọi $s, t$. Do đó, theo Mệnh đề 1 của Ch. III, §2, No. 1, tồn tại một độ đo $\alpha$ trên G cảm sinh $\mu_s$ trên sV với mọi $s$. Rõ ràng $\alpha$ là độ đo Haar trái duy nhất trên G cảm sinh $\mu$ trên V.

#### Hệ quả {#int-vii-s1-n7-cor-1 .statement}

*Cho G, G' là hai nhóm compact địa phương, V (tương ứng V') là một lân cận mở của phần tử trung hòa của G (tương ứng G'), và $\varphi$ là một đẳng cấu địa phương của G' với G (GT, III, §1, No. 3, Def. 2) được xác định trên V', sao cho $\varphi(V') = V$. Cho $\alpha'$ là một độ đo Haar trái trên G', và $\alpha'_V$, là hạn chế của nó lên $V'$. Khi đó $\varphi(\alpha'_{V'})$ là hạn chế lên $V$ của một độ đo Haar trái duy nhất $\alpha$ trên $G$.*

Cho $V_1$ là một lân cận mở của $e$ trong $G$ sao cho $V_1 V_1^{-1} \subset V$. Cho $\mu$ là hạn chế của $\varphi(\alpha'_{V'})$ lên $V_1$. Cho $U$ là một tập con mở của $V_1$ và cho $s \in G$ sao cho $sU \subset V_1$. Khi đó $s \in V_1 V_1^{-1} \subset V$, do đó $s = \varphi(s')$ với một $s' \in V'$. Cho $x \in U$. Khi đó $x = \varphi(x')$ với một $x' \in V'$, do đó $sx = \varphi(s')\varphi(x') = \varphi(s'x')$ vì $sx \in sU \subset V$. Vì các phép tịnh tiến trái trong $G'$ bảo toàn $\alpha'$, suy ra $V_1$ và $\mu$ thỏa mãn các điều kiện của Mệnh đề 9. Cho $\alpha$ là độ đo Haar trái trên $G$ cảm sinh $\mu$ trên $V_1$. Với mọi $t \in V$, tồn tại một lân cận mở $W$ của $e$ trong $V_1$ sao cho $tW \subset V$. Khi đó hạn chế của $\varphi(\alpha'_{V'})$ lên $tW$ có thể được suy ra bằng phép tịnh tiến từ hạn chế của $\mu$ lên $W$, do đó là hạn chế của $\alpha$ lên $tW$. Vì thế $\varphi(\alpha'_{V'})$ là hạn chế của $\alpha$ lên $V$.

Người ta nói rằng $\alpha$ *được suy ra từ* $\alpha'$ *nhờ đẳng cấu địa phương* $\varphi$.

#### Ví dụ {#int-vii-s1-n7-exa-1 .statement}

— Độ đo Haar trên $T$ thu được ở No. 2, *Ví dụ 3* có thể được suy ra từ độ đo Lebesgue trên $R$ nhờ một đẳng cấu địa phương của $R$ với $T$.

### 8. Các độ đo bất biến tương đối

#### Mệnh đề 10 {#int-vii-s1-prop-10 .statement}

*Cho $G$ là một nhóm locally compact, $\mu$ là một độ đo trái bất biến tương đối trên $G$ với nhân tử $\chi$. Nếu $\chi_1$ là một biểu diễn liên tục của $G$ trong $\mathbf{C}^*$, thì độ đo $\chi_1 \cdot \mu$ là trái bất biến tương đối với nhân tử $\chi_1 \chi$.*

Vì,

$$
\gamma(s)(\chi_1 \cdot \mu) = (\gamma(s)\chi_1) \cdot (\gamma(s)\mu) = (\chi_1(s^{-1})\chi_1) \cdot (\chi(s)^{-1}\mu)
= (\chi_1 \chi)(s)^{-1}(\chi_1 \cdot \mu).
$$

#### Hệ quả 1 {#int-vii-s1-prop-10-cor-1 .statement}

*Cho $\mu$ là một độ đo Haar trái trên $G$. Để một độ đo không bằng không $\nu$ trên $G$ là bất biến tương đối trái, điều kiện cần và đủ là nó có dạng $a \chi \cdot \mu$, trong đó $a \in \mathbf{C}^*$ và $\chi$ là một biểu diễn liên tục của $G$ trong $\mathbf{C}^*$; khi đó nhân tử của nó là $\chi$. \*

Điều kiện này là đủ (Mệnh đề 10). Mặt khác, nếu $\nu$ là một độ đo bất biến tương đối trái không bằng không với nhân tử $\chi$, thì $\chi^{-1} \cdot \nu$ là bất biến trái (Mệnh đề 10), do đó có dạng $a \mu$ với $a \in \mathbf{C}^*$ (No. 2, hệ quả của Định lý 1).

#### Hệ quả 2 {#int-vii-s1-prop-10-cor-2 .statement}

*Mọi độ đo bất biến tương đối trái đều là bất biến tương đối phải.*

Thật vậy, với các ký hiệu của Hệ quả 1,

$$
\delta(s)(\chi \cdot \mu) = (\delta(s)\chi) \cdot (\delta(s)\mu) = (\chi(s)\chi) \cdot (\Delta_G(s)\mu)
= (\chi \Delta_G)(s)(\chi \cdot \mu).
$$

Do Hệ quả 2, từ nay về sau ta sẽ nói về *các độ đo bất biến tương đối trên* G, không cần chỉ rõ thêm. Các độ đo bất biến tương đối, như các trường hợp riêng, bao gồm các độ đo Haar trái và các độ đo Haar phải. Cho một độ đo bất biến tương đối $\nu$ trên G, ta thuận tiện phân biệt giữa *nhân tử trái* $\chi$ và *nhân tử phải* $\chi'$, được xác định bởi $\gamma(s)\nu = \chi(s)^{-1}\nu$, $\delta(s)\nu = \chi'(s)\nu$. Theo (34), các nhân tử này thỏa mãn quan hệ

$$
\chi' = \chi \Delta_G.
$$

Vẫn ký hiệu $\mu$ là một độ đo Haar trái, ta có

$$
\nu' = (\chi \cdot \mu)' = \dot{\chi} \cdot \dot{\mu} = (\chi^{-1} \Delta_G^{-1}) \cdot \mu,
$$

do đó $\nu'$ là bất biến tương đối với nhân tử trái $\chi^{-1} \Delta_G^{-1}$ và nhân tử phải $\chi^{-1}$.

Các khái niệm về hàm không đáng kể, hàm không đáng kể địa phương, hàm khả đo và hàm khả tích địa phương là như nhau đối với mọi độ đo bất biến tương đối.

### 9. Các độ đo nửa bất biến

#### Mệnh đề 11 {#int-vii-s1-prop-11 .statement}

*Cho G là một nhóm địa phương compact, $\mu$ là một độ đo Haar trái trên G. Để một độ đo $\nu \neq 0$ trên G là nửa bất biến trái, điều kiện cần và đủ là $\nu$ tương đương với $\mu$. \*

Điều kiện đủ là hiển nhiên. Cho $\nu \neq 0$ là một độ đo nửa bất biến trái, và ta hãy chứng minh rằng $\nu$ tương đương với $\mu$. Ta có thể chỉ xét trường hợp $\nu > 0$. Cho A là một tập con compact của G. Ta sẽ chứng minh, và điều đó sẽ thiết lập mệnh đề, rằng các điều kiện $\mu(A) = 0$, $\nu(A) = 0$ là tương đương (Chương V, §5, No. 5, Định lý 2).

a) Với mọi $f \in \mathcal{K}_+(G)$, hàm $(x, y) \mapsto f(x)\varphi_A(xy)$ trên $G \times G$ là khả tích $(\nu \otimes \mu)$, vì nó là nửa liên tục trên, bị chặn, và giá đỡ của nó được chứa trong tập compact $K \times K^{-1}A$ nếu đặt $K = \operatorname{Supp} f$. Do đó, theo định lý Lebesgue–Fubini,

$$
\int d\nu(y) \int \varphi_A(xy)f(x)\,d\mu(x) = \int f(x)\,d\mu(x) \int \varphi_A(xy)\,d\nu(y).
$$

b) Giả sử $\nu(A) = 0$. Theo giả thiết, $\nu(xA) = 0$ với mọi $x \in G$, do đó vế phải của (36) bằng không. Vì thế tồn tại một tập $\nu$-không đáng kể $N_f$ sao cho, với $y \notin N_f$,

$$
(37) \quad 0 = \int \varphi_A(xy)f(x)\,d\mu(x) = \Delta_G(y)^{-1} \int \varphi_A(x)f(xy^{-1})\,d\mu(x).
$$

Cho B là một tập con compact của G sao cho $\nu(B) \neq 0$, và lấy làm $f$ một hàm trong $\mathcal{K}_+(G)$ bằng 1 trên $AB^{-1}$. Khi đó tồn tại một $y \in B$ sao cho (37) được thỏa mãn. Nhưng vì $\varphi_A(x)f(xy^{-1}) = \varphi_A(x)$ với $y \in B$, điều này chứng tỏ rằng $\mu(A) = 0$.

c) Giả sử $\mu(A) = 0$. Khi đó, với mọi $f \in \mathcal{K}_+(G)$, vế trái của (36) bằng 0, nên vế phải cũng vậy. Do đó, tồn tại một tập M địa phương $\mu$-bỏ qua được sao cho $\int \varphi_A(xy)\,d\nu(y) = 0$ với $x \notin M$. Vì $\mu \neq 0$, suy ra $\nu(xA) = 0$ với một $x \in G$, do đó $\nu(A) = 0$.

Áp dụng Mệnh đề 11 cho $G^0$, ta thấy rằng các độ đo gần bất biến phải trùng với các độ đo gần bất biến trái. Chúng được gọi đơn giản là các độ đo gần bất biến trên G.

### 10. Các trường địa phương compact

#### Định nghĩa 6 {#int-vii-s1-def-6 .statement}

— *Cho K là một trường địa phương compact*^{(1)}. *Với $a \in K^*$, người ta gọi môđun của a*, và ký hiệu bằng $\mathrm{mod}_K(a)$ hoặc đơn giản $\mathrm{mod}(a)$, *là môđun của tự đẳng cấu* $x \mapsto ax$ *của nhóm cộng* $K^+$ *nền của K; người ta đặt* $\mathrm{mod}(0) = 0$.

#### Ví dụ {#int-vii-s1-n10-exa-1 .statement}

— 1) Cho $K = \mathbf{R}$. Nếu $s > 0$ thì $s \cdot [0,1] = [0,s]$; nếu $s < 0$, $s \cdot [0,1] = [s,0]$. Do đó $\mathrm{mod}_\mathbf{R} t = |t|$ với mọi $t \in \mathbf{R}$.

2) Cho $K = \mathbf{Q}_p$. Nếu $s \in \mathbf{Q}_p^*$ sao cho $|s|_p = p^{-n}$, thì $s \mathbf{Z}_p$ là tập hợp các $x \in \mathbf{Q}_p$ sao cho $|x|_p \leq p^{-n}$; do đó, nếu $\mu$ ký hiệu độ đo Haar chuẩn hóa trên $\mathbf{Q}_p$, thì $\mu(s \mathbf{Z}_p) = p^{-n}$. Do đó $\mathrm{mod}_{\mathbf{Q}_p} t = |t|_p$ với mọi $t \in \mathbf{Q}_p$.

#### Mệnh đề 12 {#int-vii-s1-prop-12 .statement}

— *Hàm mod liên tục trên K, và* $\mathrm{mod}(ab) = \mathrm{mod}(a)\mathrm{mod}(b)$ *với mọi* $a, b$ *trong K*.

Khẳng định cuối cùng là hiển nhiên. Mệnh đề 4 của No. 4 cho thấy hàm mod liên tục tại mọi điểm của $K^*$. Chỉ còn phải chứng minh tính liên tục của nó tại 0. Điều này hiển nhiên đối với K rời rạc; vì vậy ta sẽ giả sử K không rời rạc. Cho $\alpha$ là một độ đo Haar trên $K^+$ và cho C là một tập con compact của K sao cho $\alpha(C) > 0$; với $a \in K^*$, ta có $\alpha(aC) = \mathrm{mod}(a)\alpha(C)$.

(1) Corps (A, I, §9, No. 1), cũng được dịch là "division ring" (GT, III, §6, No. 7).

Vì K không rời rạc, $\alpha(\{0\}) = 0$ (No. 2, Mệnh đề 2); do đó, với mọi $\varepsilon > 0$ tồn tại một lân cận mở U của 0 sao cho $\alpha(U) \leq \varepsilon$. Vì phép nhân trong K liên tục, $aC \subset U$ với $a$ đủ gần 0, và khi đó $\mathrm{mod}(a) \leq \varepsilon / \alpha(C)$.

#### Mệnh đề 13 {#int-vii-s1-prop-13 .statement}

— *Với mọi* $M > 0$, *cho* $V_M$ *là tập hợp các* $x \in K$ *sao cho* $\mathrm{mod}(x) \leq M$. *Nếu* K *không rời rạc, thì* $V_M$ *lập thành một hệ cơ bản các lân cận compact của* 0 *trong* K.

Các $V_M$ là các lân cận đóng của 0 theo Mệnh đề 12. Ta sẽ chứng minh rằng chúng là compact. Cho U là một lân cận compact của 0. Tồn tại một $r \neq 0$ trong K sao cho $\mathrm{mod}(r) < 1$ và $r^n \in U$ với mọi $n > 0$: quả vậy, lấy W là một lân cận của 0 sao cho $WU \subset U$; theo Mệnh đề 12, tồn tại một $r \neq 0$ trong K sao cho $\mathrm{mod}(r) < 1$ và $r \in U \cap W$; khi đó $r^2 \in WU \subset U$, và $r^n \in U$ với mọi $n > 0$ bằng quy nạp theo $n$. Ta sẽ chỉ ra rằng $V_M$ được chứa trong một hợp hữu hạn của các tập $r^{-q}U$ ($q$ là một số nguyên $\geq 0$), điều này sẽ chứng minh rằng các $V_M$ thực sự là compact. Nếu $x$ là một điểm tụ của dãy $(r^n)$, thì $\mathrm{mod}(x)$ là một điểm tụ của dãy $(\mathrm{mod}(r)^n)$, do đó $\mathrm{mod}(x) = 0$, $x = 0$; vì U là compact, suy ra (GT, I, §9, No. 1, Hệ quả của Định lý 1) rằng $\lim_{n \to \infty} r^n = 0$. Bây giờ cho $a \in V_M$. Vì dãy $(r^n a)_{n \geq 0}$ tiến tới 0, tồn tại một số nguyên nhỏ nhất $n \geq 0$ sao cho $r^n a \in U$. Nếu $n > 0$ thì $r^{n-1} a \notin U$, do đó $r^n a \in U \cap C(rU)$; bao đóng X của $U \cap C(rU)$ là compact vì U là compact, và nó không chứa 0 vì $rU$ là một lân cận của 0; do đó, trong X, $\mathrm{mod}(x)$ được chặn dưới bởi một số $m > 0$. Vậy, nếu $n > 0$, ta có $m \leq \mathrm{mod}(r^n a)$, suy ra $\mathrm{mod}(r^{-1})^n \leq M/m$. Vì $\mathrm{mod}(r^{-1}) > 1$, số nguyên $n$ chỉ có thể nhận một số hữu hạn giá trị, một số không phụ thuộc vào $a$, và điều đó hoàn tất chứng minh của mệnh đề của chúng ta.

Vì thế, do giao của các $V_M$ thu về $\{0\}$ nên các $V_M$ tạo thành một hệ cơ bản các lân cận của 0 (GT, I, §9, No. 2, Mệnh đề 1).

#### Hệ quả {#int-vii-s1-n10-cor-1 .statement}

— *Tôpô của một trường compact địa phương không rời rạc có một cơ sở đếm được.*

Quả vậy, K là hợp của các tập compact $V_1, V_2, \ldots$. Mặt khác, K là khả metric theo Mệnh đề 1 của GT, IX, §3, No. 1. Do đó tôpô của K có một cơ sở đếm được (*loc. cit.*, §2, No. 9, Hệ quả của Mệnh đề 16).

#### Mệnh đề 14 {#int-vii-s1-prop-14 .statement}

— *Cho* $\alpha$ *là một độ đo Haar trên* $K^+$. *Khi đó độ đo* $\beta = (\mathrm{mod}_K)^{-1} \cdot \alpha$ *trên* $K^*$ *là một độ đo Haar trái trên nhóm nhân* $K^*$.

Quả vậy, nếu $b \in K^*$, ánh xạ $a \mapsto b^{-1} a$ từ K vào K biến $\alpha$ thành $(\mathrm{mod}_K b) \alpha$, suy ra $(\mathrm{mod}_K)^{-1} \cdot \alpha$ thành chính nó, do đó có mệnh đề.

#### Hệ quả {#int-vii-s1-n10-cor-2 .statement}

— *Cho* f *là một hàm xác định trên* $K^*$, *với giá trị trong* $\overline{\mathbf{R}}$ *hoặc trong một không gian Banach. Để* f *là* $\beta$-*khả tích, điều kiện cần và đủ là* $(\mathrm{mod}_K)^{-1} f$ *là* $\alpha$-*khả tích, trong trường hợp đó*

$$
\int_{K^*} f(x) d\beta(x) = \int_{K^+} (\mathrm{mod}_K(x))^{-1} f(x) d\alpha(x).
$$

Điều này suy ra từ Mệnh đề 14, Hệ quả của Mệnh đề 13, và Ch. V, §5, No. 3, Định lý 1.

#### Mệnh đề 15 {#int-vii-s1-prop-15 .statement}

— *Giả sử K giao hoán. Cho u là một tự đẳng cấu của không gian vectơ E = K^n. Khi đó*

$$
\mathrm{mod}_E u = \mathrm{mod}_K(\det u).
$$

Chỉ cần kiểm tra công thức khi $u$ chạy qua một hệ sinh của $\mathbf{GL}(E)$. Bây giờ, $\mathbf{GL}(E)$ được sinh bởi các phần tử sau (A, II, §10, No. 13, Hệ quả 2 của Mệnh đề 14):
(a) Các phần tử $u_1$ có dạng

$$
(x_1, \ldots, x_n) \mapsto (x_{\sigma(1)}, \ldots, x_{\sigma(n)}),
$$

trong đó $\sigma \in \mathfrak{S}_n$;
(b) các phần tử $u_2$ có dạng

$$
(x_1, \ldots, x_n) \mapsto (ax_1, x_2, \ldots, x_n)
$$

với $a \in K^*$;
(c) các phần tử $u_3$ có dạng

$$
(x_1, \ldots, x_n) \mapsto (x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n).
$$

Nếu $f \in \mathcal{H}(E)$ thì, ký hiệu $\alpha$ là một độ đo Haar trên $K^+$,

$$
\int \cdots \int_{K^n} f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1) d\alpha(x_2) \ldots d\alpha(x_n)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \ldots d\alpha(x_n) \int_K f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \ldots d\alpha(x_n) \int_K f(x_1, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^n} f(x_1, \ldots, x_n) d\alpha(x_1) \ldots d\alpha(x_n),
$$

và mặt khác $\mathrm{mod}_K(\det u_3) = \mathrm{mod}_K(1) = 1$, do đó có kết quả đối với $u_3$. Nó được thiết lập theo một cách tương tự cho $u_1$ và $u_2$.

Cho K là một trường giao hoán compact địa phương, E là một không gian vectơ có số chiều hữu hạn n trên K. Nếu $\varphi$ là một đẳng cấu của không gian vectơ $K^n$ lên không gian vectơ E, thì $\varphi$ biến tôpô của $K^n$ thành một tôpô trên E làm cho E trở thành một không gian vectơ compact địa phương. Tôpô này (gọi là chính tắc) không phụ thuộc vào $\varphi$ vì mọi tự đẳng cấu của không gian vectơ $K^n$ đều song liên tục. Trừ khi có nói rõ điều ngược lại, khi chúng ta nói về E như một không gian vectơ tôpô, thì tôpô luôn được hiểu là tôpô vừa được định nghĩa. Mọi tự đẳng cấu u của không gian vectơ E đều song liên tục, do đó $\mathrm{mod}_E u$ được xác định. Mặt khác, nếu u là một tự đồng cấu không khả nghịch của E, ta đặt $\mathrm{mod}_E u = 0$. Khi đó:

#### Hệ quả 1 {#int-vii-s1-prop-15-cor-1 .statement}

— *Cho K là một trường compact địa phương giao hoán, E là một không gian vectơ hữu hạn chiều trên K, và u là một tự đồng cấu của không gian vectơ E. Khi đó* $\mathrm{mod}_E(u) = \mathrm{mod}_K(\det u)$.

Nếu u khả nghịch, điều này suy ra từ Mệnh đề 15. Nếu u không khả nghịch thì $\det u = 0$, do đó $\mathrm{mod}_K(\det u) = 0 = \mathrm{mod}_E u$.

#### Hệ quả 2 {#int-vii-s1-prop-15-cor-2 .statement}

— *Cho E là một không gian vectơ thực có số chiều hữu hạn n, $(e_1, e_2, \ldots, e_n)$ là một cơ sở của E, P là tập hợp các* $x = \sum_{i=1}^n \xi_i e_i \in E$ *sao cho* $0 \leq \xi_i \leq 1$ *với mọi i, và* $\mu$ *là độ đo Haar duy nhất trên nhóm cộng E sao cho* $\mu(P) = 1$. *Cho* $x_1, \ldots, x_n$ *là các điểm của E, S là bao lồi đóng trong E của tập hợp* $\{0, x_1, \ldots, x_n\}$. *Viết* $x_i = \sum_{j=1}^n \alpha_{ij} e_j$, *ta có*

$$
\mu(S) = \mu(\dot{S}) = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

Chúng ta sẽ đồng nhất E với $\mathbf{R}^n$ bằng đẳng cấu biến $(e_i)$ thành cơ sở chính tắc của $\mathbf{R}^n$. Khi đó $\mu$ được đồng nhất với độ đo Lebesgue $\mu_n$ trên $\mathbf{R}^n$.

Trước hết giả sử $x_i = e_i$ với mọi i. Khi đó S là tập $S_n$ gồm các $x = (\xi_i)$ trong $\mathbf{R}^n$ sao cho

$$
\xi_i \geq 0 \text{ với mọi } i \quad \text{và} \quad \xi_1 + \cdots + \xi_n \leq 1.
$$

Đặt $\mu_n(S_n) = a_n$. Cho $\lambda \in \mathbf{R}$. Đồng nhất $\mathbf{R}^n$ với $\mathbf{R}^{n-1} \times \mathbf{R}$, ta có thể xét tiết diện $C_\lambda$ của $S_n$ tại $\lambda$. Tiết diện này rỗng nếu $\lambda < 0$ hoặc $\lambda > 1$; nếu $0 \leq \lambda \leq 1$, thì $C_\lambda$ là tập hợp các $(\xi_1, \ldots, \xi_{n-1}) \in \mathbf{R}^{n-1}$ sao cho

$$
\xi_1 \geq 0, \ldots, \xi_{n-1} \geq 0, \quad \xi_1 + \cdots + \xi_{n-1} \leq 1 - \lambda,
$$

do đó có thể suy ra từ $S_{n-1}$ bằng một phép vị tự có tỉ số $1 - \lambda$, nên $\mu_{n-1}(C_\lambda) = (1 - \lambda)^{n-1} a_{n-1}$. Theo định lý Lebesgue–Fubini,

$$
a_n = \int_0^1 (1 - \lambda)^{n-1} a_{n-1} d\lambda = \frac{1}{n} a_{n-1}.
$$

Vì $a_1 = 1$, suy ra $a_n = \frac{1}{n!}$.

Ta trở lại trường hợp tổng quát của hệ quả. Cho $u$ là tự đồng cấu của $\mathbf{R}^n$ sao cho $u(e_i) = x_i$ với mọi $i$. Khi đó $u(S_n) = S$. Nếu $u$ khả nghịch, Mệnh đề 15 chứng minh rằng

$$
\mu_n(S) = \frac{1}{n!} |\det u| = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

Vì $S - \overset{\circ}{S}$ được chứa trong một số hữu hạn siêu phẳng, $\mu(\overset{\circ}{S}) = \mu(S)$. Cuối cùng, nếu $u$ không khả nghịch, thì $S$ được chứa trong một siêu phẳng, nên $\mu(S) = 0 = \det(\alpha_{ij})$.

### 11. Các đại số hữu hạn chiều trên một trường địa phương compact

Cho $K$ là một trường giao hoán, $A$ là một $K$-đại số hạng hữu hạn với phần tử đơn vị. Với mọi $a \in A$, đặt $L_a, R_a$ là các tự đồng cấu $x \mapsto ax$, $x \mapsto xa$ của không gian vectơ $A$, và đặt $N_{A/K}(a) \in K$, $N_{A^0/K}(a) \in K$ là các chuẩn của $a$ trong các biểu diễn chính quy của $A$ và đại số đối $A^0$; nhắc lại rằng $N_{A/K}(a) = \det(L_a)$, $N_{A^0/K}(a) = \det(R_a)$ (A, III, §9, No. 3). Các điều kiện sau là tương đương: $a$ khả nghịch, $L_a$ khả nghịch trong $\mathrm{Hom}_K(A, A)$, $R_a$ khả nghịch trong $\mathrm{Hom}_K(A, A)$, $N_{A/K}(a) \neq 0$, $N_{A^0/K}(a) \neq 0$. Ta ký hiệu $A^*$ là tập hợp các phần tử khả nghịch của $A$.

Giả sử trường $K$ là compact địa phương, do đó đại số $A$ cũng là compact địa phương. Khi đó $N_{A/K}$ và $N_{A^0/K}$ là các ánh xạ liên tục của $A$ vào $K$, suy ra $A^*$ là mở trong $A$. Theo Hệ quả 1 của Mệnh đề 15 của No. 10,

$$
\mathrm{mod}_A L_a = \mathrm{mod}_K N_{A/K}(a), \quad \mathrm{mod}_A R_a = \mathrm{mod}_K N_{A^0/K}(a).
$$

#### Mệnh đề 16 {#int-vii-s1-prop-16 .statement}

— *Cho $\alpha$ là một độ đo Haar của nhóm cộng của $A$. Các độ đo*

$$
(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha(a), \quad (\mathrm{mod}_K N_{A^0/K}(a))^{-1} d\alpha(a)
$$

*trên $A^*$ lần lượt là các độ đo Haar trái và phải của nhóm nhân $A^*$.*

Gọi $\alpha'$ là hạn chế của $\alpha$ lên tập mở $A^*$. Với $a \in A^*$, ta có $L_a(\alpha') = (\mathrm{mod}_K N_{A/K}(a))^{-1} \alpha'$, do đó $(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha'(a)$ là một độ đo Haar trái trên $A^*$ (No. 8, Hệ quả 1 của Mệnh đề 10). Chuyển qua đại số đối, ta thấy rằng $(\mathrm{mod}_K N_{A^0/K}(a))^{-1} d\alpha'(a)$ là một độ đo Haar phải trên $A^*$.

#### Mệnh đề 17 {#int-vii-s1-prop-17 .statement}

— *Giả sử $A$ là một trường (compact địa phương). Với mọi $a \in A$, $\mathrm{mod}_A(a) = \mathrm{mod}_K N_{A/K}(a)$.*

Đây là bản dịch của công thức thứ nhất của (38).

#### Ví dụ {#int-vii-s1-n11-exa-1 .statement}

— 1) Lấy $K = \mathbf{R}$, $A = \mathbf{C}$. Xét đến *Alg.*, chương VIII, §12, n° 2, mệnh đề 4, ta thu được $\mathrm{mod}_\mathbf{C}(z) = |z|^2$ với mọi $z \in \mathbf{C}$. (2)

2) Lấy $K = \mathbf{R}$, và lấy A là *trường quaternion* $\mathbf{H}$ (GT, VIII, §1, No. 4). Xét các phần tử sau đây của $\mathbf{M}_2(\mathbf{C})$:

$$
X_1 = \begin{pmatrix} 0 & i \\ i & 0 \end{pmatrix} \quad X_2 = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \quad X_3 = \begin{pmatrix} i & 0 \\ 0 & -i \end{pmatrix}
$$

vốn cùng với $I_2$, lập thành một cơ sở của $\mathbf{M}_2(\mathbf{C})$ trên $\mathbf{C}$. Dễ thấy rằng

$$
X_1^2 = X_2^2 = X_3^2 = -I_2, \qquad X_1 X_2 = -X_2 X_1 = X_3,
$$
$$
X_2 X_3 = -X_3 X_2 = X_1, \qquad X_3 X_1 = -X_1 X_3 = X_2.
$$

Do đó, ánh xạ $a + b i + c j + d k \mapsto a I_2 + b X_1 + c X_2 + d X_3$ có thể được mở rộng thành một $\mathbf{C}$-đẳng cấu của đại số $\mathbf{C} \otimes_\mathbf{R} \mathbf{H}$ lên đại số $\mathbf{M}_2(\mathbf{C})$. Vì $[\mathbf{H} : \mathbf{R}] = 4$, $\mathbf{C}$ là một trường trung hòa của $\mathbf{H}$ (*Alg.*, chương VIII, §10, n° 5), và chuẩn rút gọn của $q = a + b i + c j + d k \in \mathbf{H}$ là

$$
\mathrm{Nrd}(q) = \det(a I_2 + b X_1 + c X_2 + d X_3)
$$
$$
= \det \begin{pmatrix} a + i d & -c + i b \\ c + i b & a - i d \end{pmatrix} = a^2 + b^2 + c^2 + d^2 = \|q\|^2.
$$

Theo *Alg.*, chương VIII, §12, n° 3, mệnh đề 8, ta có

$$
\mathrm{N}_{\mathbf{H}/\mathbf{R}}(q) = (\mathrm{Nrd}_{\mathbf{H}/\mathbf{R}}(q))^2 = \|q\|^4.
$$

Điều này đã nói, Mệnh đề 17 cho thấy rằng

$$
\mathrm{mod}_\mathbf{H}(q) = \|q\|^4.
$$

Một nghiên cứu sâu hơn về cấu trúc của các trường compact địa phương sẽ được thực hiện trong CA, VI, §9.

(2) Điều này cũng suy ra từ Hệ quả 1 của Mệnh đề 15 và sự kiện rằng phép nhân trái bởi $z = a + i b$ có ma trận $\begin{pmatrix} a & -b \\ b & a \end{pmatrix}$ đối với cơ sở chính tắc $1, i$ của $\mathbf{C}$ trên $\mathbf{R}$.

### Bài tập {#int-vii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
