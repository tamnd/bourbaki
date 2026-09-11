---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 6
section_title: Absolute values
lang: vi
source: ac-i-vii
book_pages: 403-411, 459-460
pdf_pages: 0421-0429, 0477-0478
extraction: ocr
subsections:
    - "no": 1
      title: PRELIMINARIES ON ABSOLUTE VALUES
      page: 403
      pdf_page: 421
    - "no": 2
      title: ULTRAMETRIC ABSOLUTE VALUES
      page: 405
      pdf_page: 423
    - "no": 3
      title: ABSOLUTE VALUES ON Q
      page: 406
      pdf_page: 424
    - "no": 4
      title: STRUCTURE OF FIELDS WITH A NON-ULTRAMETRIC ABSOLUTE VALUE
      page: 407
      pdf_page: 425
statements: 10
exercises: 2
content_sha256: 52c4b38007c5b4d588021006c3ae64946a27bedee8c392f5ce8827456b88eb64
translated_from: content/en/ac/VI/06_s6_absolute_values.md
source_content_sha256: 0ba346951e7ec856945465325b2f054546b3b1d4334f235bfc11d9776cf48c78
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-81ca19be
glossary_version: 34
glossary_terms_sha256: ca75bd806d266ccf168059ea107da6614cea81ad10c29dc37230d1b8ff35f774
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 6. GIÁ TRỊ TUYỆT ĐỐI

### 1. NHỮNG ĐIỀU SƠ BỘ VỀ CÁC GIÁ TRỊ TUYỆT ĐỐI

Cho $K$ là một trường (giao hoán hoặc không). Nhắc lại (Tôpô đại cương, Chương IX, § 3, no. 2, Định nghĩa 2) rằng một giá trị tuyệt đối trên $K$ là một ánh xạ bất kỳ $f$ từ $K$ vào $\mathbf{R}_+$ thỏa mãn các tiên đề sau:

(VA,) Quan hệ $f(x) = 0$ tương đương với $x = 0$.
(VAII) $f(xy) = f(x)f(y)$ với mọi $x, y$ thuộc $K$.
(VAIll) $f(x + y) \leq f(x) + f(y)$ với mọi $x, y$ thuộc $K$.

Suy ra từ (VA,) và (VAII) rằng $f(1) = 1, f(-1) = 1$ và
$$
f(x^{-1}) = \frac{1}{f(x)}
$$
với $x \neq 0$.

Đối với một ánh xạ $f$ từ $K$ vào $\mathbf{R}$, và một số thực $A > 0$, ký hiệu $(\mathrm{U}_A)$ là quan hệ
$$
f(x + y) \leq A \cdot \sup(f(x), f(y)) \quad \text{với mọi } x, y \text{ thuộc } K.
$$

Ta sẽ ký hiệu bởi $\mathscr{V}(K)$ tập hợp các ánh xạ $f$ từ $K$ vào $\mathbf{R}_+$ thỏa mãn (VAI) và (VAII) và với chúng tồn tại một $A > 0$ (phụ thuộc vào $f$) sao cho $(\mathrm{U}_A)$ đúng.

Chú ý rằng nếu f $\in \mathscr{V}(K)$, thì, đặt $x = 1, y = 0$ trong $(\mathrm{U}_A)$,
$$
1 = f(1) \leq A \cdot \sup(f(1), f(0)) = A.
$$

#### Mệnh đề 1 {#ac-vi-s6-prop-1 .statement}

Đối với một ánh xạ $f$ từ $K$ vào $\mathbf{R}$, thỏa mãn (VA,) và (VAII) để thuộc $\mathscr{V}(K)$, điều kiện cần và đủ là $f(1 + x)$ bị chặn trong tập hợp các $x \in K$ sao cho $f(x) \leq 1$.

Nếu $f$ thỏa mãn $(\mathbf{U}_A)$, thì $f(1 + x) \leq A$ nếu $f(x) \leq 1$. Ngược lại, giả sử rằng $f(x + 1) \leq A$ đối với các $x \in K$ sao cho $f(x) \leq 1$ (điều này kéo theo rằng $A \geq f(1) = 1$); khi đó, nếu $x = 0$ hoặc $y = 0$, điều kiện $(\mathbf{U}_A)$ được thỏa mãn; nếu ngược lại $x \neq 0$ và $y \neq 0$, ta có thể giả sử chẳng hạn rằng $f(y) \leq f(x)$, do đó, theo $(\mathbf{VA}_s)$, $f(yx^{-1}) \leq 1$ và vì vậy $f(1 + yx^{-1}) \leq A$, điều này cho, theo $(\mathbf{VA}_{II})$, $f(x + y)f(x)^{-1} \leq A$; do đó

$$
f(x + y) \leq Af(x) \leq A \sup(f(x), f(y)).
$$

Nếu $f$ là một giá trị tuyệt đối trên $K$, thì $f(n.1) \leq n$ theo quy nạp trên số nguyên $n > 0$ bắt đầu từ $(\mathbf{VA}_{III})$; ngược lại:

#### Mệnh đề 2 {#ac-vi-s6-prop-2 .statement}

*Cho $f$ là một ánh xạ từ $K$ vào $\mathbf{R}_+$ thuộc $\mathcal{V}(K)$; nếu tồn tại $C > 0$ sao cho $f(n.1) \leq C$ với mọi số nguyên $n > 0$, thì $f$ là một giá trị tuyệt đối trên $K$.*

Theo quy nạp trên $r > 0$, ta suy ra từ $(\mathbf{U}_A)$ quan hệ

$$(1)$$
$$
f(x_1 + x_2 + \cdots + x_{2^r}) \leq A^r \sup_{1 \leq i \leq 2^r} f(x_i)
$$

với mọi họ $(x_i)$ gồm $2^r$ phần tử của $K$. Ta đặt $n = 2^r - 1$; với mọi $x \in K$, ta suy ra từ (1)

$$
(f(1 + x))^n = f((1 + x)^n) = f\left( \sum_{i=0}^n \binom{n}{i} x^i \right) \leq A^r \sup \left( f\left( \binom{n}{i} \right) (f(x))^i \right)
$$
$$
\leq CA^r \sum_{i=0}^n \binom{n}{i} (f(x))^i = CA^r (1 + f(x))^n
$$

do $f\left( \binom{n}{i} \right) \leq C \binom{n}{i}$; do đó
$$
f(1 + x) \leq C^{1/n} A^{r/n} (1 + f(x)).
$$

Cho $r$ tiến tới $+\infty$, ta thu được $f(1 + x) \leq 1 + f(x)$ với mọi $x \in K$; áp dụng bất đẳng thức này với $x$ được thay bởi $xy^{-1}$ (trong đó $y \neq 0$) và tính đến $(\mathbf{VA}_{II})$, ta thu được quan hệ $(\mathbf{VA}_{III})$, điều này chứng minh mệnh đề.

#### Hệ quả 1 {#ac-vi-s6-prop-2-cor-1 .statement}

*Để một ánh xạ $f$ từ $K$ vào $\mathbf{R}_+$ là một giá trị tuyệt đối, điều kiện cần và đủ là nó thỏa mãn các điều kiện $(\mathbf{VA}_I)$, $(\mathbf{VA}_{II})$ và $(\mathbf{U}_2)$.*

Điều kiện này là cần, vì $(\mathbf{VA}_{II})$ suy ra
$$
f(x + y) \leq f(x) + f(y) \leq 2 \sup(f(x), f(y)).
$$

Ngược lại, giả sử $f$ thỏa mãn $(\mathbf{VA}_I)$, $(\mathbf{VA}_s)$ và $(\mathbf{U}_2)$; với mọi số nguyên $n > 0$, gọi $r$ là số nguyên nhỏ nhất sao cho $2^r \geq n$; nếu trong (1) $A$ được thay bởi 2, các $x_i$ có chỉ số $i \leq n$ được thay bởi 1 và các $x_i$ có chỉ số $i > n$ được thay bởi 0, ta thu được
$$
f(n.1) \leq 2^r < 2n;
$$
khi đó Mệnh đề 2 có thể được áp dụng với $C = 2$ và do đó $f$ là một giá trị tuyệt đối.

#### Hệ quả 2 {#ac-vi-s6-prop-2-cor-2 .statement}

Đối với một ánh xạ $f$ của $K$ vào $\mathbf{R}_+$ thuộc $\mathcal{V}(K)$, điều kiện cần và đủ là nó có dạng $g^t$, trong đó $t > 0$ và $g$ là một giá trị tuyệt đối trên $K$.

Nói rằng $f$ thỏa mãn $(\mathbf{U}_A)$ tương đương với việc nói rằng $f^s$ thỏa mãn $(\mathbf{U}_{A^s})$; vì tồn tại $s > 0$ sao cho $A^s \leq 2$, Hệ quả 1 cho thấy rằng với giá trị $s$ như vậy, $f^s$ là một giá trị tuyệt đối.

### 2. CÁC GIÁ TRỊ TUYỆT ĐỐI SIÊU MÊTRIC

Một ánh xạ $f$ của $K$ vào $\mathbf{R}_+$ được gọi là một giá trị tuyệt đối siêu mêtric nếu nó thỏa mãn các điều kiện $(\mathrm{VA}_I)$, $(\mathrm{VA}_{II})$ và $(\mathrm{U},)$ (điều này hiển nhiên suy ra rằng $f$ là một giá trị tuyệt đối).

#### Mệnh đề 3 {#ac-vi-s6-prop-3 .statement}

Cho $f$ là một ánh xạ của $K$ vào $\mathbf{R}_+$. Các tính chất sau là tương đương:
(a) $f$ là một giá trị tuyệt đối siêu mêtric.
(b) Tồn tại một định giá $v$ trên $K$ với các giá trị trong $\mathbf{R}$ và một số thực $a$ sao cho $0 < a < 1$ và $f = a''$.
(c) $f$ thuộc $\mathcal{V}(K)$ và $f(n.1) \leq 1$ với mọi số nguyên $n > 0$.
(d) Với mọi $s > 0$, $f^s$ là một giá trị tuyệt đối.

Với mọi số thực $c$ sao cho $0 < c < 1$, ánh xạ $t \mapsto c^t$ là một đẳng cấu của nhóm có thứ tự $\mathbf{R}$ (với thứ tự đối với thứ tự thông thường) lên nhóm có thứ tự $\mathbf{R}_+^*$; điều này chỉ ra sự tương đương của (a) và (b). Rõ ràng (a) suy ra (c); (c) suy ra (d), vì ta suy ra từ (c) rằng
$$
(f(n.1))^s \leq 1 \leq n
$$
với mọi số nguyên $n > 0$ và Mệnh đề 2 của no. 1 chỉ ra rằng $f''$ là một giá trị tuyệt đối. Cuối cùng (d) suy ra (a): vì iff" là một giá trị tuyệt đối, nó thỏa mãn $(\mathbf{U}_2)$ và do đó $f$ thỏa mãn $(\mathbf{U}_{2^{1/s}})$ với mọi $s > 0$ và vì vậy cũng thỏa mãn $(\mathbf{U}_1)$, khi cho $s$ tiến tới $+\infty$.

#### Hệ quả {#ac-vi-s6-n2-cor-1 .statement}

Nếu $K$ là một trường (không nhất thiết giao hoán) có đặc số $p > 0$, mọi hàm trên $\mathcal{V}(K)$ đều là một giá trị tuyệt đối siêu mêtric.

Mọi phần tử khác không $z = n.1$ ($n$ một số nguyên $> 0$) thuộc trường con nguyên tố $\mathbf{F}_p$ của $K$ và do đó thỏa mãn quan hệ $z^{p-1} = 1$, điều này suy ra $f(z) = 1$ và ta có thể áp dụng Mệnh đề 3 (c).

Cho một số thực $c$ sao cho $0 < c < 1$, các công thức
$$
f(x) = c^{v(x)}, \quad v(x) = \log, f(x)
$$
do đó thiết lập một sự tương ứng một-một giữa các giá trị tuyệt đối ultramêtric trên $K$ và các định giá trên $K$ có giá trị thực. Định giá không đúng tương ứng với giá trị tuyệt đối không đúng (Tôpô Đại cương, Chương IX, § 3, no. 2). Cho $v_1, v_2$ là hai định giá trên $K$ có giá trị thực và $f_1, f_2$ là các giá trị tuyệt đối tương ứng; để $v_1$ và $v_2$ tương đương, điều kiện cần và đủ là $f_1$ và $f_2$ tương đương: nói rằng $v_1$ và $v_2$ tương đương tương đương với việc nói rằng các quan hệ $v_1(x) \geq 0$ và $v_2(x) \geq 0$ tương đương hoặc cũng vậy rằng các quan hệ $f_1(x) \leq 1$ và $f_2(x) \leq 1$ tương đương; do đó chỉ cần áp dụng Mệnh đề 5 của *Tôpô Đại cương*, Chương IX, § 3, no. 2. Ngoài ra (*loc. cit.*) để các tôpô xác định trên K bởi $f_1$ và $f_2$ là đồng nhất, điều kiện cần và đủ là $f_1$ và $f_2$ tương đương.

### 3. CÁC GIÁ TRỊ TUYỆT ĐỐI TRÊN Q

#### Mệnh đề 4 {#ac-vi-s6-prop-4 .statement}

*Cho $f$ là một ánh xạ từ $\mathbf{Q}$ vào $\mathbf{R}_+$ thuộc $\mathcal{V}(\mathbf{Q})$. Khi đó:*

(i) *Hoặc $f$ là giá trị tuyệt đối không đúng trên $\mathbf{Q}$.*

(ii) *Hoặc tồn tại một số thực $a$ và một số nguyên tố $p$ sao cho $0 < a < 1$ và $f = a^{v_p}$, trong đó $v_p$ là định giá $p$-adi.*

(iii) *Hoặc tồn tại $s > 0$ sao cho $f(x) = |x|^s$ với mọi $x \in \mathbf{Q}$.*

*Trong trường hợp (iii) để $f$ là một giá trị tuyệt đối trên $\mathbf{Q}$, điều kiện cần và đủ là $0 < s \leq 1$.*

Trước hết, giả sử rằng $f(n) \leq 1$ với mọi số nguyên $n > 0$. Theo Mệnh đề 3 của no. 2 tồn tại một số thực $b$ và một định giá $v$ trên $\mathbf{Q}$ sao cho $0 < b < 1$ và $f = b^v$. Bây giờ, ta biết (§ 3, no. 4, *Ví dụ 4*) rằng các định giá duy nhất trên $\mathbf{Q}$ là (tới tương đương) định giá không đúng và các định giá $p$-adi $v_p$; do đó ta có hoặc trường hợp (i) hoặc trường hợp (ii).

Giả sử từ nay rằng tồn tại một số nguyên $h > 0$ sao cho $f(h) > 1$; theo no. 1, Hệ quả 2 của Mệnh đề 2, tồn tại một số $\rho > 0$ sao cho $f^\rho$ là một giá trị tuyệt đối; ta viết

$$
g(x) = \rho \log(f(x))/\log|x|
$$

với mọi số hữu tỉ $x \neq 0$. Cho $a, b$ là hai số nguyên $\geq 2$; với mỗi số nguyên $n \geq 2$ ký hiệu $q(n)$ là phần nguyên của $n \log a/\log b$, nói cách khác là số nguyên nhỏ nhất $m$ sao cho $a^n < b^{m+1}$; do đó khai triển của $a^n$ theo cơ số $b$ là

$$
a^n = c_0 + c_1 b + \ldots + c_{q(n)} b^{q(n)}
$$

trong đó $0 \leq c_i < b$ với $0 \leq i \leq q(n)$. Vì $f^\rho$ là một giá trị tuyệt đối, $f^\rho(c_i) \leq c_i \leq b$ và do đó từ (2) suy ra rằng

$$
(f(a))^{n\rho} = (f(a^n))^\rho \leq b(1 + (f(b))^\rho + \ldots + (f(b))^{q(n)\rho})
$$
$$
\leq b(q(n) + 1)(\sup(1, (f(b))^\rho))^{q(n)}.
$$

Lấy logarit hai vế của bất đẳng thức này và chia cho $n \log a$, ta được

$$
g(a) \leq \frac{\log b}{n \log a} + \frac{\log(q(n) + 1)}{q(n)} \cdot \frac{q(n)}{n \log a} + \frac{\sup(0, \rho \log f(b))}{\log a} \cdot \frac{q(n)}{n}.
$$

Chú ý rằng khi $n$ tiến tới $+\infty$, $q(n)/n$ tiến tới $\log a/\log b$; do đó $q(n)$ tiến tới $+\infty$ và

$$
\log(q(n) + 1)/q(n)
$$

tiến tới 0 (Hàm của một Biến Thực, Chương III, § 2, no. 1). Lấy giới hạn trong (3), ta được

(4) $$
g(a) \leq \frac{\sup(0, \rho \log f(b))}{\log b} = \sup(0, g(b)).
$$

Nhưng $f(h) > 1$, do đó $g(h) > 0$; nếu thay $a$ bởi $h$ trong (4), ta được $\sup(0, g(b)) > 0$ và do đó

$$
\sup(0, g(b)) = g(b).
$$

Sau đó, với mọi số nguyên $a, b$ lớn hơn hoặc bằng 2, $g(a) \leq g(b)$ và do đó $g(a) = g(b)$, bằng cách hoán đổi vai trò của $a$ và $b$. Nói cách khác, tồn tại một hằng $\lambda$ sao cho $g(a) = A$ với mọi số nguyên $a \geq 2$; nếu ta viết $s = \lambda / \rho$, thì $f(a) = |a|^s$ với mọi số nguyên $a \geq 2$. Vì $f(xy) = f(x)f(y)$ và $f(-x) = f(x)$, nên $f(x) = |x|^s$ với mọi $x \in Q$. Cuối cùng, nếu $0 < s \leq 1$, ta biết rằng $x \mapsto |x|^s$ là một giá trị tuyệt đối (Tôpô đại cương, chương IX, § 3, no. 2); ngược lại, nếu $s$ là sao cho $x \mapsto |x|^s$ là một giá trị tuyệt đối trên $Q$, thì $(1 + 1)^s \leq 1^s + 1^s$, nghĩa là $2^s \leq 2$, do đó $s \leq 1$.

### 4. CẤU TRÚC CỦA CÁC TRƯỜNG CÓ GIÁ TRỊ TUYỆT ĐỐI KHÔNG SIÊU MÊTRIC

#### Định lý 1 (Gelfand-Mazur) {#ac-vi-s6-thm-1 .statement}

Cho $K$ là một đại số trên trường $\mathbf{R}$ với hai tính chất sau:
(1) $K$ là một trường (không nhất thiết giao hoán).
(2) Trên $K$ tồn tại một chuẩn $x \mapsto \|x\|$ tương thích với cấu trúc đại số trên $K$ (Tôpô đại cương, chương IX, § 3, no. 7, Định nghĩa 9).
Khi đó đại số $K$ đẳng cấu với một trong các đại số $\mathbf{R}, \mathbf{C}$ hoặc $\mathbf{H}$.

Nhắc lại (loc. cit.) rằng luôn có thể giả sử rằng $\|xy\| \leq \|x\| \cdot \|y\|$ với mọi $x, y$ trong $K$. Ta sẽ trang bị cho $K$ tôpô (tương thích với cấu trúc đại số) được xác định bởi chuẩn.

(A) Trường hợp thứ nhất: $K$ là giao hoán và tồn tại $j \in K$ sao cho $j^2 = -1$

Khi đó tồn tại một đẳng cấu $\sigma$ của trường $\mathbf{C}$ lên một trường con của $K$ sao cho $\sigma(\xi + i\eta) = \xi . 1 + \eta . j$ với $\xi, \eta$ trong $\mathbf{R}$. Ta sẽ chứng minh bằng phản chứng rằng $K = \sigma(\mathbf{C})$. Giả sử khi đó tồn tại $x \in K - \sigma(\mathbf{C})$; với mọi $z \in \mathbf{C}, x - \sigma(z)$ do đó là khả nghịch trong $K$; ta viết $F(z) = (x - \sigma(z))^{-1}$; vì $\sigma$ liên tục và phép nghịch đảo liên tục trên $K$ (Tôpô đại cương, chương IX, § 3, no. 7, Mệnh đề 13 áp dụng cho đại số hoàn thành của $K$), $F$ là một ánh xạ liên tục từ $\mathbf{C}$ vào $K$. Hơn nữa, ta có thể viết với $z \neq 0$

$$
F(z) = (\sigma(z))^{-1}(x(\sigma(z))^{-1} - 1)^{-1}.
$$

Nhưng, vì $(\sigma(z))^{-1} = \sigma(z^{-1})$ tiến tới 0 khi $z$ tiến tới vô cực trong $\mathbf{C}$, ta thấy rằng $F(z)$ tiến tới 0; nói cách khác, $z \mapsto \|F(z)\|$ là một hàm thực liên tục, $\geq 0$ trên $\mathbf{C}$, tiến tới 0 tại điểm vô cực và do đó có thể được xem như một hàm liên tục trên không gian compact $\tilde{C}$ thu được bằng cách ghép thêm vào $C$ một điểm vô cực. Cận trên của $\| F \|$ trên $C$ là $a$ do đó là hữu hạn và $> 0$, và tập hợp $P$ gồm các số phức $z$ sao cho $\| F(z) \| = a$ là đóng và khác rỗng (*General Topology*, Chương IV, § 6, no. 1, Định lý 1).

Cho $z \in P$; ta viết $y = x - \sigma(z)$ và cho $t$ là một số phức $\neq 0$ sao cho $\| \sigma(t) \| < \alpha^{-1}$, do đó $\| \sigma(t) \cdot y^{-1} \| < 1$ theo định nghĩa của $a$. Dãy của các $(\sigma(t) y^{-1})^n$ và dãy của các $n(\sigma(t) y^{-1})^n$ do đó tiến tới 0 trong $K$ khi $n$ tiến tới $+\infty$, vì các dãy tương ứng của các chuẩn trong $R$ cũng vậy. Mặt khác, chú ý rằng với mọi đa thức $H(T) = \prod_{k=1}^p (T - \sigma(c_k))$, trong đó các $c_k$ là các số phức phân biệt, trong trường $K(T)$ của các hàm hữu tỉ

$$
\frac{H'(T)}{H(T)} = \sum_{k=1}^p \frac{1}{T - \sigma(c_k)}
$$

Ta áp dụng công thức này cho đa thức

$$
H(T) = T^n - (\sigma(t))^n = \prod_{k=0}^{n-1} (T - \sigma(\omega_n^k t)),
$$

trong đó $\omega_n = \exp(2\pi i / n)$, và thay $T$ bằng phần tử $y \in K$, là phần tử phân biệt với tất cả các $\sigma(\omega_n^k t)$. Suy ra (trong trường giao hoán $K$) rằng

$$
\frac{ny^{n-1}}{y^n - (\sigma(t))^n} = \frac{1}{y - \sigma(t)} + \sum_{k=1}^{n-1} \frac{1}{y - \sigma(\omega_n^k t)}.
$$

Tính đến các định nghĩa của $F$ và $y$, ta thu được

$$
\begin{align}
F(z + t) + \sum_{k=1}^{n-1} F(z + \omega_n^k t) - nF(z) \\
= \frac{ny^{n-1}}{y^n - (\sigma(t))^n} - \frac{n}{y} = \frac{1}{y} \cdot \frac{n(\sigma(t) y^{-1})^n}{1 - (\sigma(t) y^{-1})^n}.
\end{align}
$$

Nhưng do sự lựa chọn của $t$ và các nhận xét đã nêu ở trên, biểu thức cuối cùng trong (7) tiến tới 0 khi $n$ tiến tới $+\infty$; do đó

$$
\| F(z + t) \| = \lim_{n \to +\infty} \| nF(z) - \sum_{k=1}^{n-1} F(z + \omega_n^k t) \|.
$$

Bây giờ, $\| F(z) \| = \alpha$ và $\| F(z + \omega_n^k t) \| \leq \alpha$ theo định nghĩa của $\alpha$, do đó

$$
\| nF(z) - \sum_{k=1}^{n-1} F(z + \omega_n^k t) \| \geq n \| F(z) \| - \sum_{k=1}^{n-1} \| F(z + \omega_n^k t) \| \geq n \alpha - (n-1)\alpha = \alpha.
$$

Do đó theo (8), cho n tiến tới $+\infty$, $\|F(z + t)\| \geq a$ và theo định nghĩa của $a$ điều này suy ra
$$
\|F(z + t)\| = \alpha,
$$
nói cách khác $z + t \in P$. Điều này chứng minh rằng tập hợp $P$ là *mở* trong $\mathbf{C}$; vì nó cũng đóng và khác rỗng và $\mathbf{C}$ liên thông, $P = \mathbf{C}$ và do đó $\|F\|$ là hằng trên $\mathbf{C}$; vì hàm này tiến tới 0 tại điểm vô hạn, $\|F(z)\| = 0$ trong $\mathbf{C}$ và đặc biệt $\|F(0)\| = \|x^{-1}\| = 0$, điều này là vô lý.

(B) *Trường hợp thứ hai; K giao hoán và* $-1$ *không là bình phương của một phần tử của K*
Gọi L là trường giao hoán thu được bằng cách ghép vào K một nghiệm j của $T^2 + 1$; L là một không gian vectơ trên K nhận $(1, j)$ làm cơ sở và L hiển nhiên là một đại số trên $\mathbf{R}$. Rõ ràng hàm $x + yj \to \|x\| + \|y\|$ là một chuẩn trên L tương thích với cấu trúc của nó như một không gian vectơ trên $\mathbf{R}$; mặt khác, với $z = x + yj, z' = x' + y'j$ trong L,
$$
\begin{align*}
\|zz'\| &= \|xx' - yy'\| + \|xy' + x'y\| \\
&\leq \|x\|.\|x'\| + \|y\|.\|y'\| + \|x\|.\|y'\| + \|x'\|.\|y\| \\
&= (\|x\| + \|y\|)(\|x'\| + \|y'\|) = \|z\|.\|z'\|.
\end{align*}
$$
Chuẩn được định nghĩa như vậy do đó tương thích với cấu trúc đại số trên R của L. Theo trường hợp (A) L là một đại số trên R đẳng cấu với $\mathbf{C}$; giờ đây đại số con trên R duy nhất của $\mathbf{C}$ phân biệt với $\mathbf{C}$ là $\mathbf{R}$ và do đó K đẳng cấu với $\mathbf{R}$.

(C) *Trường hợp thứ ba: K không giao hoán*
Gọi Z là tâm của K và x là một phần tử của K không thuộc Z; trường con $Z(x)$ của K là giao hoán và chuẩn cảm sinh bởi chuẩn trên K tương thích với cấu trúc đại số trên R của $Z(x)$; vì $Z \neq Z(x)$ và Z và $Z(x)$ là các đại số trên R đẳng cấu với $\mathbf{R}$ hoặc $\mathbf{C}$ nhờ (A) và (B), Z nhất thiết đẳng cấu với $\mathbf{R}$ và $Z(x)$ với $\mathbf{C}$. Với mọi $x \in K, Z(x)$ do đó có hạng $\leq 2$ trên Z. Bây giờ ta có bổ đề sau:

#### Bổ đề 1 {#ac-vi-s6-lem-1 .statement}

*Cho D là một trường có tâm L sao cho, với mọi $x \in D, L(x)$ là một mở rộng của L có bậc $\leq m$. Khi đó hạng của D trên L là $\leq m^2$.*

Ta hiển nhiên có thể hạn chế sự chú ý của mình vào trường hợp $D \neq L$. Khi đó tồn tại trong D một mở rộng đại số giao hoán tách được *hữu hạn* E của L có bậc $> 1$ (*Đại số*, Chương VIII, § 10, no. 3, Bổ đề 1); vì $E = L(x)$ với một x thích hợp nào đó trong E (*Đại số*, Chương V, § 7, no. 7, Mệnh đề 12 và Chương VII, § 5, no. 7), theo giả thiết $[E : L] \leq m$. Giả sử mở rộng tách được E được chọn sao cho $[E : L]$ là hữu hạn và lớn nhất có thể và xét *vành giao hoán* $E' \supset E$ của E trong D, đây là một trường có tâm E sao cho $$
[D : E'] = [E : L] \leq m
$$

(*Đại số*, Chương VIII, § 10, no. 2, Định lý 2). Nếu E $\#$ E', thì trong $\mathbf{E}'$ sẽ tồn tại một mở rộng đại số tách được hữu hạn F của $\mathbf{E}$ có bậc $> 1$ (*Đại số*, Chương VIII, § 10, no. 3, Bổ đề 1); do đó F sẽ là một mở rộng đại số tách được hữu hạn của L (*Đại số*, Chương V, § 7, no. 4, Mệnh đề 7) có bậc $> [\mathrm{E}: \mathrm{L}]$, trái với định nghĩa của E; do đó $\mathbf{E}' = \mathbf{E}$, từ đó $[\mathrm{D}: \mathrm{L}] = [\mathrm{D}: \mathrm{E}][\mathrm{E}: \mathrm{L}] \leq m^2$.

Áp dụng bổ đề này cho K với $m = 2$, ta thấy rằng K là một trường mở rộng không giao hoán của R có hạng hữu hạn và do đó đẳng cấu với trường quaternion $\mathbf{H}$ (*Đại số*, Chương VIII, § 11, no. 2, Định lý 2).

Nhận xét (1) Chúng ta sẽ đưa ra trong chương dành cho các đại số chuẩn một chứng minh ngắn hơn của Định lý Gelfand-Mazur, đúng với mọi đại số tôpô lồi địa phương Hausdorff $K$ trên R và có nguyên lý như sau: nó được quy về (như trong các trường hợp (B) và (C)) trường hợp $K$ là một đại số giao hoán trên $\mathbf{C}$; nếu $x \in \mathbf{K} - \mathbf{C}.1$, ta xét như trên ánh xạ $z \mapsto (x - z.1)^{-1}$ từ $\mathbf{C}$ vào K, liên tục và khả vi trên $\mathbf{C}$. Với mọi phần tử $x'$ của không gian đối ngẫu $\mathbf{K}'$ của không gian lồi địa phương K, $z \mapsto \langle (x - z.1)^{-1}, x' \rangle$ khi đó là một hàm nguyên bị chặn trên $\mathbf{C}$ và do đó là hằng theo Định lý Liouville, và ta kết luận như trong phần (A) của chứng minh Định lý 1 rằng điều này tất yếu dẫn đến $\langle (x - z.1)^{-1}, x' \rangle = 0$ với mọi $z \in \mathbf{C}$ và mọi $x' \in \mathbf{K}'$; Định lý Hahn-Banach cho thấy kết luận này là vô lý, vì $(x - z.1)^{-1} \neq 0$. Chú ý rằng lập luận trong phần (A) của chứng minh Định lý 1 chỉ khác với lập luận trên về hình thức, vì lập luận này chỉ là một trường hợp đặc biệt của lập luận dùng để chứng minh nguyên lý cực đại đối với các hàm giải tích, phép lấy tổng trên các căn của đơn vị và chuyển qua giới hạn tương đương với việc tính tích phân $\int_{\gamma} \frac{\mathbf{F}(z + t)}{t} dt$ dọc theo một đường tròn tâm 0 và việc sử dụng công thức Cauchy được tránh ở đây, nhờ dạng đặc biệt của hàm F.

Định lý 2 (Ostrowski). Cho K là một trường (không nhất thiết giao hoán) và f là một phần tử $\mathcal{V}(K)$ không phải là một giá trị tuyệt đối ultrametric. Khi đó tồn tại duy nhất một số thực $s > 0$ và một đẳng cấu j của K lên một trường con trù mật khắp nơi của một trong các trường $\mathbf{R}, \mathbf{C}$ hoặc $\mathbf{H}$ sao cho $f(x) = |j(x)|^s$ với mọi $x \in K$ (*). Để f là một giá trị tuyệt đối trên K, điều kiện cần và đủ là $s \leq 1$.

Theo no. 2, Hệ quả của Mệnh đề 3, K có đặc số 0 và do đó là một đại số trên $\mathbf{Q}$; với mọi $x \in \mathbf{Q}$ ta đặt $h(x) = f(x.1)$; rõ ràng $h \in \mathcal{V}(\mathbf{Q})$ và do đó Mệnh đề 4 của no. 3 có thể được áp dụng; cả trường hợp (i) lẫn (ii) của mệnh đề này đều không thể xảy ra, vì điều đó sẽ kéo theo $f(n.1) \leq 1$ với mọi số nguyên $n > 0$ và f sẽ là một giá trị tuyệt đối ultrametric theo no. 2, Mệnh đề 3. Khi đó tồn tại một số thực s > 0 sao cho h(x) = |x|^s với mọi x ∈ Q, tức là f(x.1) = |x|^s; ta đặt g = f^{1/s}. Khi đó g ∈ V(K) và g(n.1) = n với mọi số nguyên n; do đó Mệnh đề 2 của no. 1 cho thấy g là một giá trị tuyệt đối trên K.

Với x ∈ Q và y ∈ K, g(xy) = |x|g(y) và do đó g là một chuẩn trên K tương thích với cấu trúc đại số trên Q của nó (với giá trị tuyệt đối thông thường trên Q). Do đó, hoàn thành K của K là một đại số chuẩn trên Q = R (Tôpô tổng quát, Chương IX, § 3, no. 7); gọi ĝ là chuẩn trên K là mở rộng liên tục của g. Vì g là một giá trị tuyệt đối trên K, K là một trường và ĝ là một giá trị tuyệt đối trên K (Tôpô tổng quát, Chương IX, § 3, no. 3, Mệnh đề 6). Theo Định lý 1 tồn tại một đẳng cấu đại số trên Rf của K̂ lên một trong các trường R, C hoặc H và g'(x) = |j(x)| do đó là một giá trị tuyệt đối trên K̂; vì K̂ hữu hạn chiều trên R và g' và ĝ trùng nhau trên trường con R . 1 của K̂, nên g' = ĝ theo bổ đề sau:

#### Bổ đề 2 {#ac-vi-s6-lem-2 .statement}

Cho L là một trường (không nhất thiết giao hoán) và K là một trường con của L sao cho L là một không gian vectơ trái ajinite-chiều trên K. Cho g là một giá trị tuyệt đối trên L vàf là hạn chế của nó trên K. Nếu K đầy đủ và không rời rạc đối với f, thì L đầy đủ đối với g; nếu thêm vào đó g' là một giá trị tuyệt đối khác trên L có cùng hạn chếf trên K, thì g' = g.

Vì tôpô xác định bởi g là Hausdorff và tương thích với cấu trúc không gian vectơ K trái trên L, khẳng định đầu tiên suy ra từ Topological Vector Spaces, Chapter I, § 2, no. 3, Định lý 2. Hơn nữa, các tôpô trên L xác định bởi g và g' là giống nhau (loc. cit.) ; do đó tồn tại một số thực s > 0 sao cho g' = g^s (General Topology, Chapter IX, § 3, no. 2, Mệnh đề 5). Lấy x là một phần tử của K sao cho f(x) ≠ 1; phương trình g'(x) = g(x) chứng minh rằng s = 1.

Quay lại chứng minh Định lý 2, ta thấy rằng, nếu j ký hiệu hạn chế của f trên K, thì j là một đẳng cấu của K lên một trường con trù mật khắp nơi của R, C hoặc H và g(x) = |j(x)| với x ∈ K, do đó f(x) = |j(x)|^s.

Cuối cùng chú ý rằng, nếu f là một giá trị tuyệt đối trên K, thì h là một giá trị tuyệt đối trên Q và s ≤ 1 theo no. 3, Mệnh đề 4; ngược lại, nếu s ≤ 1, f = g^s là một giá trị tuyệt đối trên K vì g là một giá trị tuyệt đối (Tôpô tổng quát, Chương IX, § 3, no. 2); điều này chứng minh khẳng định cuối cùng của mệnh đề.

Các nhận xét

(2) Nếu K là một trường và một đại số chuẩn trên R, thì chuẩn không nhất thiết là một giá trị tuyệt đối trên K; chẳng hạn, ξ + iη → |ξ| + |η| là một chuẩn trên C tương thích với cấu trúc đại số trên R của nó.

(3) Để có một chứng minh trường hợp (C) của Định lý 1 không sử dụng các kết quả tổng quát của Đại số, Chương VIII, xem Bài tập 2.

### Bài tập {#ac-vi-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).
