---
book: int
book_title: Integration
chapter: II
chapter_title: RIESZ SPACES
section: 2
section_title: Linear forms on a Riesz space
lang: vi
source: int-i-vi
book_pages: INT II.19-INT II.21
pdf_pages: 0033-0039, 0043-0045
extraction: ocr
subsections:
    - "no": 1
      title: Positive linear forms on a Riesz space
      page: 9
      pdf_page: 33
    - "no": 2
      title: Relatively bounded linear forms
      page: 10
      pdf_page: 34
statements: 13
exercises: 9
content_sha256: 1e25f2ce84e070d2124701f33c7a9fc9469590c1c86df4251da2348de38a8b71
translated_from: content/en/int/II/02_s2_linear_forms_on_a_riesz_space.md
source_content_sha256: f261078ae1db1a985db1c8cbda6a7a6f980a9e5c399f533b3b3eabf7b1f185bd
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-90bd1f49
glossary_version: 34
glossary_terms_sha256: bc36d137f16dca754c0bdcf62e80edae04b09c5015b3fd409dd24bb8bb1d29f0
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC DẠNG TUYẾN TÍNH TRÊN MỘT KHÔNG GIAN RIESZ

### 1. Các dạng tuyến tính dương trên một không gian Riesz

Ta nhắc lại định nghĩa sau (TVS, II, §2, No. 5):

#### Định nghĩa 1 {#int-ii-s2-def-1 .statement}

Cho một không gian vectơ có thứ tự E, một dạng tuyến tính L trên E được gọi là dương nếu $L(x) \geq 0$ với mọi $x \geq 0$ trong E.

Vì $L(y) - L(x) = L(y - x)$, nên nói rằng quan hệ $x \leq y$ kéo theo $L(x) \leq L(y)$ cũng là tương đương, hay nói cách khác $L$ là một hàm tăng trên E.

#### Ví dụ 1 {#int-ii-s2-n1-exa-1 .statement}

Cho A là một tập hợp bất kỳ, E là một không gian con tuyến tính của không gian $\mathbf{R}^A$ gồm tất cả các hàm giá trị thực xác định trên A. Với mọi phần tử $a \in A$, ánh xạ $x \mapsto x(a)$ là một dạng tuyến tính dương trên E.

#### Ví dụ 2 {#int-ii-s2-n1-exa-2 .statement}

Cho $I = [a, b]$ là một khoảng compact của $\mathbf{R}$, E là không gian Riesz được tạo bởi các hàm giá trị thực điều hòa trên I (FRV, II, §1, No. 3); ánh xạ $x \mapsto \int_a^b x(t) \, dt$ là một dạng tuyến tính dương trên E.

#### Ví dụ 3 {#int-ii-s2-n1-exa-3 .statement}

Cho F là một tập hợp bất kỳ, $\mathcal{U}$ là một siêu lọc trên F (GT, I, §6, No. 4), E là không gian Riesz $\mathscr{B}(F)$ của các hàm giá trị thực bị chặn trên F. Với mọi $x \in E$, $\lim_{\mathcal{U}} x(t)$ tồn tại, bởi vì $x(\mathcal{U})$ là một cơ sở của một siêu lọc trên tập compact tương đối $x(F)$, do đó là hội tụ. Hơn nữa, nếu $x \geq 0$ thì $\lim_{\mathcal{U}} x(t) \geq 0$ theo nguyên lý mở rộng của các bất đẳng thức; ánh xạ $x \mapsto \lim_{\mathcal{U}} x$ do đó là một dạng tuyến tính dương trên E. Nếu $\mathcal{U}$ được lấy là siêu lọc tạo bởi các tập chứa một phần tử $a \in F$, ta thu được lại dạng tuyến tính dương $x \mapsto x(a)$ (Ví dụ 1).

#### Mệnh đề 1 {#int-ii-s2-prop-1 .statement}

Cho E là một không gian vectơ có thứ tự, L là một ánh xạ của E vào $\mathbf{R}$ sao cho $L(x + y) = L(x) + L(y)$ và sao cho quan hệ $x \geq 0$ kéo theo $L(x) \geq 0$; khi đó $L(\lambda x) = \lambda L(x)$ với mọi vô hướng $\lambda$ và mọi $x \geq 0$.

Vì $L(-x) = -L(x)$ ($L$ là một biểu diễn của nhóm cộng E trong $\mathbf{R}$), ta có thể tự giới hạn vào trường hợp $\lambda \geq 0$. Với mọi số nguyên $n \geq 0$, ta có $L(nx) = nL(x)$, do đó $L((1/n)x) = (1/n)L(x)$ và do đó $L(rx) = rL(x)$ với mọi số hữu tỉ $r \geq 0$. Mặt khác, $L$ tăng trong E; nếu $r$ và $r'$ là các số hữu tỉ sao cho $r \leq \lambda \leq r'$, thì suy ra $rL(x) \leq L(\lambda x) \leq r'L(x)$; vì $rL(x)$ và $r'L(x)$ sai khác với $\lambda L(x)$ nhỏ tùy ý, ta có $L(\lambda x) = \lambda L(x)$.

#### Mệnh đề 2 {#int-ii-s2-prop-2 .statement}

Cho E là một không gian vectơ thực, C là một nón lồi có đỉnh 0 trong E sao cho $E = C - C$, và $x \mapsto M(x)$ là một ánh xạ từ C vào $\mathbf{R}$ sao cho $M(\lambda x + \mu y) = \lambda M(x) + \mu M(y)$ với mọi $x \in C$, $y \in C$, $\lambda \geq 0$, $\mu \geq 0$. Khi đó, tồn tại duy nhất một dạng tuyến tính L mở rộng M lên E.

Theo giả thiết, mọi $z \in E$ có thể được viết $z = y - x$, trong đó $x, y$ thuộc C; hơn nữa, nếu cũng có $z = y' - x'$ với $x' \in C$, $y' \in C$, thì

$M(y) - M(x) = M(y') - M(x')$; vì, từ quan hệ $y - x = y' - x'$ ta suy ra $y + x' = x + y'$, do đó $M(y) + M(x') = M(x) + M(y')$. Ta ký hiệu $L(z)$ là giá trị chung của $M(y) - M(x)$ đối với mọi biểu thức của $z$ dưới dạng hiệu $y - x$ của hai phần tử của $C$; ta kiểm tra ngay lập tức rằng $L$ là một dạng tuyến tính trên $E$ mở rộng $M$; tính duy nhất của $L$ suy ra từ sự kiện $C$ sinh ra không gian $E$.

#### Mệnh đề 3 {#int-ii-s2-prop-3 .statement}

*Cho $E$ là một không gian vectơ có hướng có thứ tự, $P$ là tập hợp các phần tử $\geqslant 0$ của $E$, và $x \mapsto M(x)$ là một ánh xạ của $P$ vào $\mathbf{R}$, với các giá trị $\geqslant 0$, sao cho $M(x + y) = M(x) + M(y)$ với mọi $x, y$ trong $P$. Khi đó, tồn tại một và chỉ một dạng tuyến tính dương $L$ mở rộng $M$ đến $E$.*

Vì $E = P - P$, cùng lập luận như trong Mệnh đề 2 chứng minh, trước hết, sự tồn tại và tính duy nhất của một ánh xạ *cộng tính* $L$ của $E$ vào $\mathbf{R}$ mở rộng $M$. Mệnh đề 1 sau đó chỉ ra rằng $L(\lambda x) = \lambda L(x)$ với mọi $\lambda \geqslant 0$ và mọi $x \in P$, từ đó ngay lập tức suy ra rằng $L$ là một dạng tuyến tính.

### 2. Các dạng tuyến tính bị chặn tương đối

Cho $E$ là một không gian vectơ có thứ tự có hướng. Gọi $Q$ là tập hợp các dạng tuyến tính *dương* trên $E$; đó là một tập con của đối ngẫu đại số $E^*$ của $E$ (không gian của mọi dạng tuyến tính trên $E$). Ngay lập tức thấy rằng $Q + Q \subset Q$ và $\lambda Q \subset Q$ với mọi vô hướng $\lambda > 0$ (nói cách khác, $Q$ là một *nón lồi* trong $E^*$). Hơn nữa, $Q \cap (-Q) = \{0\}$, vì nếu $L$ và $-L$ đều là các dạng tuyến tính dương, thì $L(x) \geqslant 0$ và $L(x) \leqslant 0$ với mọi $x \geqslant 0$, do đó $L(x) = 0$ với mọi $x \geqslant 0$ và vì thế $L = 0$ (No. 1, Prop. 3). Như vậy tập $Q$ xác định trên $E^*$ một *quan hệ thứ tự* $L \leqslant M$, tương đương với « $M - L$ là một dạng tuyến tính dương trên $E$ », hay cũng tương đương với « với mọi $x \geqslant 0$, $L(x) \leqslant M(x)$ »; các phần tử $\geqslant 0$ của $E^*$ đối với cấu trúc thứ tự này là các dạng tuyến tính dương (điều này biện minh cho thuật ngữ đã được đưa vào). Gọi $\Omega$ là không gian con tuyến tính của $E^*$ sinh bởi $Q$, nghĩa là tập hợp các dạng tuyến tính trên $E$ là *hiệu của hai dạng tuyến tính dương*; chúng ta sẽ đưa ra một đặc trưng hóa khác của các phần tử của $\Omega$ khi $E$ là một không gian Riesz.

#### Định nghĩa 2 {#int-ii-s2-def-2 .statement}

*Cho một không gian Riesz $E$, một dạng tuyến tính $L$ trên $E$ được gọi là bị chặn tương đối nếu, với mọi $x \geqslant 0$ trong $E$, $L$ bị chặn trên tập hợp các $y \in E$ sao cho $|y| \leqslant x$.*

#### Định lý 1 {#int-ii-s2-thm-1 .statement}

1° *Điều kiện cần và đủ để một dạng tuyến tính $L$ trên một không gian Riesz $E$ bị chặn tương đối là nó là hiệu của hai dạng tuyến tính dương.*

2° *Không gian vectơ có thứ tự $\Omega$ của các dạng tuyến tính bị chặn tương đối trên $E$ là một không gian Riesz được sắp thứ tự dàn đầy đủ.*

Nếu $L = U - V$, trong đó $U$ và $V$ là các dạng tuyến tính dương trên $E$, thì quan hệ $-x \leq y \leq x$ kéo theo

$$
-U(x) \leq U(y) \leq U(x) \quad \text{và} \quad -V(x) \leq V(y) \leq V(x),
$$

do đó ngay lập tức suy ra $|L(y)| \leq U(x) + V(x)$; vì thế $L$ bị chặn tương đối. Ngược lại, giả sử $L$ bị chặn tương đối; tất cả quy về việc chứng minh rằng tồn tại một dạng tuyến tính dương $N$ sao cho $N(x) \geq L(x)$ với mọi $x \geq 0$, bởi vì khi đó $N - L$ sẽ là một dạng tuyến tính dương.

Bây giờ, nếu một dạng tuyến tính dương $N$ có tính chất này thì, với mọi $x \geq 0$ và với $0 \leq y \leq x$, ta có $N(x) \geq N(y) \geq L(y)$, do đó $N(x) \geq \sup_{0 \leq y \leq x} L(y)$; nếu ta chứng minh rằng hàm thực

$$
x \mapsto M(x) = \sup_{0 \leq y \leq x} L(y),
$$

xác định trên tập hợp $P$ các phần tử $\geq 0$ của $E$, có thể được mở rộng thành một dạng tuyến tính dương trên $E$ (cũng được ký hiệu là $M$), thì ta sẽ chứng minh phần thứ nhất của định lý và hơn nữa sẽ chứng minh rằng $M$ là cận trên bé nhất của $0$ và $L$ trong $\Omega$. Vì $M(x) \geq 0$ trên $P$, nên mọi việc quy về việc chứng minh rằng

$$
M(x + x') = M(x) + M(x')
$$

với mọi cặp phần tử $x \geq 0,\ x' \geq 0$ của $E$ (No. 1, Mệnh đề 3). Theo định nghĩa,

$$
M(x) + M(x') = \sup_{0 \leq y \leq x} L(y) + \sup_{0 \leq y' \leq x'} L(y')
= \sup_{0 \leq y \leq x,\ 0 \leq y' \leq x'} L(y + y') \leq M(x + x').
$$

Mặt khác, với mọi $z$ sao cho $0 \leq z \leq x + x'$, ta có $x + x' = z + u$ với $u \geq 0$; theo bổ đề phân tích (§ 1, No. 1), tồn tại hai phần tử $y,\ y'$ sao cho $0 \leq y \leq x,\ 0 \leq y' \leq x'$ và sao cho $z = y + y',\ u = (x - y) + (x' - y')$; khi đó

$$
L(z) = L(y) + L(y') \leq M(x) + M(x'),
$$

do đó $M(x + x') = \sup_{0 \leq z \leq x + x'} L(z) \leq M(x) + M(x')$, điều này hoàn tất chứng minh phần thứ nhất của định lý. Hơn nữa, như vậy ta đã chỉ ra rằng $\Omega$ là một *không gian Riesz* và rằng, với mọi dạng tuyến tính bị chặn tương đối $L$ trên $E$ và với mọi $x \geq 0$,

(1)
$$
L^+(x) = \sup_{0 \leq y \leq x} L(y).
$$

Còn lại là thấy rằng $\Omega$ là có thứ tự dàn đầy đủ; để làm điều này, chỉ cần chỉ ra rằng mọi tập hợp $H$ gồm các dạng tuyến tính *dương*, bị chặn trên và có hướng đối với quan hệ $\leqslant$, có một cận trên bé nhất trong $\Omega$.

Tổng quát hơn, ta có bổ đề sau:

#### Bổ đề {#int-ii-s2-n2-lem-1 .statement}

— *Cho E là một không gian vectơ có thứ tự có hướng, $E^*$ là đối ngẫu của nó, được sắp thứ tự bằng cách lấy các dạng tuyến tính dương làm các phần tử dương. Cho $(u_\alpha)$ là một họ tăng có hướng các phần tử của $E^*$. Nếu, với mọi $x \geqslant 0$ trong E, $\sup u_\alpha(x) < +\infty$, thì họ $(u_\alpha)$ có một cận trên bé nhất $u$ trong $E^*$ và, với mọi $x \geqslant 0$ trong E,

$$
u(x) = \sup_{\alpha} u_\alpha(x).
$$

Trong tập hợp P gồm mọi $x \geqslant 0$ trong E, định nghĩa ánh xạ $u$ bởi công thức (2); ngay lập tức thấy rằng $u(\lambda x) = \lambda u(x)$ với mọi $\lambda \geqslant 0$ và $x \in P$; để chứng minh bổ đề, do đó chỉ cần, theo Mệnh đề 2 của No. 1, chứng minh rằng

$$
u(x + y) = u(x) + u(y)
$$

với $x, y$ trong P. Nhưng điều này là ngay lập tức khi nhận thấy rằng $u(x) = \lim u_\alpha(x)$ đối với tập có hướng của các chỉ số (định lý giới hạn đơn điệu).

Từ công thức (1), ta suy ra ngay lập tức rằng nếu $L$ và $M$ là hai dạng tuyến tính bị chặn tương đối trên E thì, với mọi $x \geqslant 0$,

$$
\begin{cases}
\sup(L, M)(x) = \sup_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} (L(y) + M(z)) \\
\inf(L, M)(x) = \inf_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} (L(y) + M(z)).
\end{cases}
$$

Đặc biệt, nếu trong công thức thứ nhất trong các công thức này, $M$ được thay bởi $-L$, ta được

$$
|L|(x) = \sup_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} L(y - z).
$$

Bây giờ, nếu $x = y + z$, $y \geqslant 0$ và $z \geqslant 0$, thì $-x \leqslant y - z \leqslant x$; ngược lại, quan hệ $|u| \leqslant x$ kéo theo $L(u) \leqslant |L|(|u|) \leqslant |L|(x)$. Từ đó suy ra công thức

$$
|L|(x) = \sup_{|y| \leqslant x} L(y) \quad \text{với } x \geqslant 0,
$$

do đó, đặc biệt,

$$
|L(x)| \leqslant |L|(|x|)
$$

với mọi $x \in E$.

#### Mệnh đề 4 {#int-ii-s2-prop-4 .statement}

— Để hai dạng tuyến tính dương $L, M$ trên một không gian Riesz $E$ xa lạ nhau trong không gian $\Omega$, điều kiện cần và đủ là, với mọi số $\varepsilon > 0$ và mọi $x \geq 0$ trong $E$, tồn tại hai phần tử $y \geq 0, z \geq 0$ của $E$ sao cho $x = y + z$ và $L(y) + M(z) \leq \varepsilon$.

Thật vậy, theo công thức thứ hai của (3), điều kiện này biểu thị rằng $\inf(L, M) = 0$.

#### Mệnh đề 5 {#int-ii-s2-prop-5 .statement}

— Cho $L$ là một dạng tuyến tính dương trên một không gian Riesz $E$. Để một dạng tuyến tính dương $M$ trên $E$ thuộc dải sinh bởi $L$ trong $\Omega$, điều kiện cần và đủ là, với mọi $x \geq 0$ trong $E$ và mọi số $\varepsilon > 0$, tồn tại một số $\delta > 0$ sao cho các quan hệ $0 \leq y \leq x$ và $L(y) \leq \delta$ kéo theo $M(y) \leq \varepsilon$.

Trước hết, hãy chứng minh rằng điều kiện là cần thiết. Nếu $M \geq 0$ thuộc dải sinh bởi $L$ trong $\Omega$, thì (§ 1, No. 5, Hệ quả của Mệnh đề 6)

$$
M = \sup_n \left( \inf(nL, M) \right).
$$

Nếu đặt

$$
U_n = M - \inf(nL, M),
$$

thì $U_n$ do đó là một dạng tuyến tính dương trên $E$ và $\inf_n U_n = 0$ trong $\Omega$; do đó (Bổ đề) $U_n(x)$ tiến tới 0 khi $n$ tiến ra vô cùng, và tồn tại một $n$ sao cho $U_n(x) \leq \varepsilon/2$. Giữ cố định một $n$ như vậy, ta có $U_n(y) \leq \varepsilon/2$ với mọi $y$ sao cho $0 \leq y \leq x$, do đó quan hệ $0 \leq y \leq x$ kéo theo

$$
M(y) \leq \frac{\varepsilon}{2} + \inf(nL, M)(y) \leq \frac{\varepsilon}{2} + nL(y);
$$

nếu $y$ sao cho $L(y) \leq \varepsilon/2n$ thì suy ra $M(y) \leq \varepsilon$, điều này thiết lập mệnh đề của chúng ta.

Bây giờ ta hãy chỉ ra rằng điều kiện đó là đủ. Với mọi dạng tuyến tính dương $M$ trên $E$, ta có thể viết $M = U + V$, trong đó $U$ thuộc dải sinh bởi $L$ trong $\Omega$ và $V$ ngoại lai đối với $L$, còn $U$ và $V$ đều dương (§ 1, No. 5, Định lý 1). Nếu $M$ thỏa mãn điều kiện của mệnh đề thì $V = M - U$ cũng thỏa mãn điều kiện ấy, vì $0 \leq V \leq M$. Từ đó ta sẽ suy ra rằng $V = 0$. Với mọi $x \geq 0$ trong $E$ và mọi số $\eta > 0$, tồn tại hai phần tử $y \geq 0, z \geq 0$ của $E$ sao cho $x = y + z$ và $L(y) + V(z) \leq \eta$ (Mệnh đề 4); cho một số tùy ý $\varepsilon > 0$, chọn $\eta \leq \varepsilon$ sao cho các hệ thức $0 \leq u \leq x$ và $L(u) \leq \eta$ kéo theo $V(u) \leq \varepsilon$; với $y$ và $z$ được xác định như trên, ta có $L(y) \leq \eta$, do đó $V(y) \leq \varepsilon$ và vì thế

$$
V(x) = V(y) + V(z) \leq \varepsilon + \eta \leq 2\varepsilon;
$$

vì $\varepsilon$ là tùy ý, ta có $V(x) = 0$ với mọi $x \geq 0$, tức là, $V = 0$.

#### Ví dụ {#int-ii-s2-n2-exa-1 .statement}

Cho E là một không gian Riesz được trang bị một tôpô lồi địa phương tương thích với cấu trúc không gian vectơ có thứ tự của nó (TVS, II, §2, No. 7). Gọi E' là đối ngẫu tôpô của E, và giả sử thêm rằng nón P gồm các phần tử $\geqslant 0$ của E là *đầy đủ đối với tôpô yếu đi* $\sigma(E, E')$. Khi đó mọi dạng tuyến tính liên tục $x' \in E'$ đều *bị chặn tương đối*, vì người ta biết (TVS, II, §6, No. 8, Hệ quả 2 của Mệnh đề 11) rằng dưới các điều kiện ấy, với mọi $x \geqslant 0$ trong E, tập các $y \in E$ sao cho $|y| \leqslant x$ là *compact* đối với $\sigma(E, E')$. Từ đó ta suy ra rằng khi đó E là *dàn đầy đủ*; thật vậy, theo ($§ 1$, No. 3, Mệnh đề 2), chỉ cần chỉ ra rằng với mọi tập hợp $H \subset E$ bị chặn trên và có hướng đối với $\leqslant$, bộ lọc tiết diện $\mathcal{F}$ của H là *hội tụ trong E đối với tôpô* $\sigma(E, E')$ (tôpô sau tương thích với cấu trúc không gian vectơ có thứ tự của E). Bằng phép tịnh tiến, ta có thể giả sử rằng $H \subset P$, và khi đó chỉ cần chỉ ra rằng $\mathcal{F}$ là một *bộ lọc Cauchy* đối với $\sigma(E, E')$, hay cũng thế, rằng mọi dạng tuyến tính liên tục $x' \in E'$ đều có một giới hạn đối với $\mathcal{F}$. Nhưng điều này suy ra ngay từ định lý giới hạn đơn điệu khi $x'$ là một dạng tuyến tính *dương*, và vì mọi dạng tuyến tính $x' \in E'$ là hiệu của hai dạng tuyến tính dương (Định lý 1) nên mệnh đề của chúng ta được chứng minh.

Bài tập

### Bài tập {#int-ii-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
