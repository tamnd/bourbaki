---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 3
section_title: Disintegration of measures
lang: vi
source: int-i-vi
book_pages: INT VI.40-INT VI.51, INT VI.69-INT VI.71
pdf_pages: 0431-0442, 0460-0462
extraction: ocr
subsections:
    - "no": 1
      title: Disintegration of a measure $\mu$ relative to a $\mu$-proper mapping
      page: 40
      pdf_page: 431
    - "no": 2
      title: Pseudo-image measures
      page: 44
      pdf_page: 435
    - "no": 3
      title: Disintegration of a measure $\mu$ relative to a pseudo-image of $\mu$
      page: 45
      pdf_page: 436
    - "no": 4
      title: Measurable equivalence relations
      page: 46
      pdf_page: 437
    - "no": 5
      title: Disintegration of a measure by a measurable equivalence relation
      page: 50
      pdf_page: 441
statements: 16
exercises: 12
content_sha256: 56798dc47dd81cf53b56a86323ba48cbe3ad59b0d050ec9749d442d8a38f3235
translated_from: content/en/int/VI/03_s3_disintegration_of_measures.md
source_content_sha256: 8879ed2dcbac290dcceecb297da3c70b77ffea9c231d05f50a9508eb784557f9
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-71f41523
glossary_version: 34
glossary_terms_sha256: c1f37c7855bbf50652ab0fdaa3b2d6f7f8870f88a22a72c368672a62372e62d2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. PHÂN RÃ CỦA CÁC ĐO LƯỜNG

### 1. Phân rã của một đo lường $\mu$ đối với một ánh xạ $\mu$-thực sự

Cho T là một không gian compact địa phương có một cơ sở đếm được (nói cách khác, một không gian Polish compact địa phương (GT, IX, §6, No. 1). Ta biết rằng đối với mọi đo lường dương trên T, các khái niệm nguyên và nguyên cốt yếu trùng nhau (Ch. V, §1, No. 3, Hệ quả của Mệnh đề 9). Mặt khác, ta có các tính chất sau:

#### Bổ đề 1 {#int-vi-s3-lem-1 .statement}

*Nếu Y là một không gian compact địa phương có một cơ sở đếm được, không gian $\mathcal{H}(Y)$ chứa một tập con trù mật đếm được. Chính xác hơn, tồn tại trong $\mathcal{H}(Y)$ một tập con đếm được S gồm các hàm $\geq 0$, sao cho, đối với mọi hàm $f \geq 0$ của $\mathcal{H}(Y)$, tồn tại một dãy các hàm $f_n \in S$ ($n \geq 0$) hội tụ đều đến $f$ và sao cho $f_n \leq f_0$ với mọi $n \geq 0$.*

Vì Y là hợp của một dãy tăng $(U_n)$ các tập mở tương đối compact sao cho $\overline{U}_n \subset U_{n+1}$ với mọi $n$ (GT, I, §9, No. 9, Mệnh đề 15); không gian $\mathcal{H}(Y)$ là hợp của dãy tăng các không gian Banach $\mathcal{H}(Y, \overline{U}_n)$, và mỗi không gian sau cùng này được biết là tách được (GT, Ch. X, §3, No. 3, Định lý 1). Cho $S'_n$ là một tập con trù mật đếm được trong $\mathcal{H}(Y, \overline{U}_n)$, $S_n$ là tập hợp các hàm $\varphi^+$ đối với $\varphi \in S'_n$, và $u_n$ là một hàm trong $\mathcal{H}(Y, \overline{U}_{n+1})$, có các giá trị trong $[0, 1]$ và bằng 1 trên $U_n$. Ta lấy cho S hợp của các $S_n$ và tập hợp các $m u_n$ với $m$ và $n$ là các số nguyên $\geq 0$. Đối với mọi hàm $f \geq 0$ của $\mathcal{H}(Y)$, $f$ có giá chứa được trong một trong các $U_n$, do đó là giới hạn đều của một dãy các hàm $f_p \in S_n$ ($p \geq 1$). Các hàm $f_p$ này bị chặn đều bởi một số nguyên dương $m$, và chỉ cần lấy $f_0 = m u_n$.*

#### Bổ đề 2 {#int-vi-s3-lem-2 .statement}

*Nếu T là một không gian compact địa phương với một cơ sở đếm được, thì không gian Banach $\mathcal{K}(Y)$ gồm các hàm số liên tục tiến về 0 tại điểm vô hạn là tách được.*

Bổ đề này không gì khác hơn là Hệ quả của Định lý 1 của GT, X, §3, No. 3. Ta có thể nhận xét rằng nó cũng suy ra từ Bổ đề 1 và sự kiện rằng tôpô của sự hội tụ đều trên $\mathcal{K}(Y)$ thô hơn tôpô giới hạn trực tiếp của các tôpô của các không gian con $\mathcal{K}(Y, \overline{U}_n)$.

#### Bổ đề 3 {#int-vi-s3-lem-3 .statement}

— *Cho T và X là hai không gian compact địa phương có các cơ sở đếm được, $\mu$ là một đo lường dương trên T, và $t \mapsto \lambda_t$ ($t \in T$) là một họ các đo lường dương trên X. Nếu ánh xạ $t \mapsto \lambda_t$ là $\mu$-nguyên theo vô hướng (đối với tôpô $\sigma(\mathcal{M}(X), \mathcal{K}(X))$), thì họ $t \mapsto \lambda_t$ là $\mu$-thích hợp ($§ 1$, No. 1, Ví dụ).*

Vì, Bổ đề 1, áp dụng cho $\mathcal{K}(X)$, chỉ ra rằng ánh xạ $t \mapsto \lambda_t$ là đo được theo nghĩa mơ hồ đối với $\mu$ ($§ 1$, No. 5, Mệnh đề 13).

#### Định lý 1 {#int-vi-s3-thm-1 .statement}

*Cho T và B là hai không gian compact địa phương có các cơ sở đếm được, $\mu$ là một độ đo dương trên T, p là một ánh xạ $\mu$-thực sự (Ch. V, §6, No. 1, Định nghĩa 1) của T vào B, và $\nu = p(\mu)$ là ảnh của $\mu$ qua p. Khi đó tồn tại một họ $\nu$-thích hợp ($§ 1$, No. 1, Ví dụ) $b \mapsto \lambda_b$ ($b \in B$) các độ đo dương trên T, có các tính chất sau:

a) $\| \lambda_b \| = 1$ với mọi $b \in p(T)$;

b) $\lambda_b$ tập trung trên tập hợp $\overline{p}^{-1}(b)$ (Ch. V, §5, No. 7, Định nghĩa 4) với mọi $b \in B$; đặc biệt, $\lambda_b = 0$ với $b \notin p(T)$;

c) $\mu = \int \lambda_b d\nu(b)$.

Hơn nữa, nếu $b \mapsto \lambda'_b$ ($b \in B$) là một họ $\nu$-thích hợp thứ hai các độ đo dương trên T có các tính chất b) và c), thì $\lambda'_b = \lambda_b$ hầu khắp nơi trong B đối với độ đo $\nu$.

1) *Tính duy nhất.* Với mọi hàm $f \in \mathcal{K}(B)$, $f \circ p$ là $\mu$-khả tích vì p là $\mu$-thực sự (Ch. V, §6, No. 2, Định lý 1); với mọi hàm $g \in \mathcal{K}(T)$, hàm $t \mapsto g(t)f(p(t))$ do đó là $\mu$-khả tích. Suy ra (Ch. V, §3, No. 3, Định lý 1) rằng với hầu hết mọi $b \in B$, hàm $t \mapsto g(t)f(p(t))$ là $\lambda_b$-khả tích và

$$
\int g(t)f(p(t)) d\mu(t) = \int d\nu(b) \int g(t)f(p(t)) d\lambda_b(t).
$$

Nhưng vì $\lambda_b$ tập trung trên $\overline{p}^{-1}(b)$, ta có, với mọi $b \in B$, $f(p(t)) = f(b)$ hầu khắp nơi đối với $\lambda_b$, do đó vế thứ hai của (1) bằng $\int f(b)\langle g, \lambda_b \rangle d\nu(b)$. Công thức tương tự đối với $\lambda'_b$ cũng đúng; do đó $\int f(b)\langle g, \lambda_b \rangle d\nu(b) = \int f(b)\langle g, \lambda'_b \rangle d\nu(b)$ với mọi $f \in \mathcal{K}(B)$ và $g \in \mathcal{K}(T)$. Nói cách khác, hai ánh xạ $b \mapsto \lambda_b$ và $b \mapsto \lambda'_b$ của B vào $\mathcal{M}(T)$ bằng nhau vô hướng hầu khắp nơi địa phương đối với $\nu$, do đó bằng nhau hầu khắp nơi đối với $\nu$ (Bổ đề 1 và §1, No. 1, Nhận xét 2).

2) *Định nghĩa tạm thời của họ* $b \mapsto \lambda_b$. Với mọi hàm $f \in \mathcal{L}^1(\nu)$, $f \circ p$ là $\mu$-khả tích (Ch. V, §6, No. 2, Định lý 1), do đó $(f \circ p) \cdot \mu$ là một độ đo bị chặn trên T, và

$$
\|(f \circ p) \cdot \mu\| = \int |f \circ p| \, d\mu = \int |f| \, d\nu = N_1(f)
$$

(Ch. IV, §4, No. 7, Prop. 12; Ch. V, §5, No. 3, Th. 1 và §6, No. 2, Th. 1). Suy ra rằng $(f \circ p) \cdot \mu$ chỉ phụ thuộc vào lớp $\tilde{f}$ của $f$ trong $L^1(\nu)$ và rằng $\tilde{f} \mapsto (f \circ p) \cdot \mu$ là một ánh xạ tuyến tính *đẳng cự* từ $L^1(\nu)$ vào không gian Banach $\mathcal{M}^1(T)$ của các độ đo bị chặn trên T, đối ngẫu mạnh của không gian Banach $\mathcal{K}(T)$, là tách được (Bổ đề 2). Theo định lý Dunford–Pettis (§2, No. 5, Hệ quả 2 của Th. 1), tồn tại một ánh xạ $b \mapsto \lambda_b$ của B vào quả cầu đơn vị của $\mathcal{M}^1(T)$, đo được vô hướng theo $\nu$ (đối với tôpô $\sigma(\mathcal{M}^1(T), \overline{\mathcal{K}(T)})$) và sao cho, với mọi hàm $f \in \mathcal{L}^1(\nu)$,

$$
(f \circ p) \cdot \mu = \int f(b) \lambda_b \, d\nu(b),
$$

cũng có thể được viết, với mọi hàm $g \in \overline{\mathcal{K}(T)}$

$$
\int g(t) f(p(t)) \, d\mu(t) = \int f(b) \, d\nu(b) \int g(t) \, d\lambda_b(t).
$$

Nếu $f \geq 0$ và $g \geq 0$, vế thứ nhất của (3) là $\geq 0$, điều này chứng minh rằng với mọi hàm $g \geq 0$ trong $\mathcal{K}(T)$, độ đo $(\int g(t) \, d\lambda_b(t)) \cdot \nu$ là $\geq 0$, do đó $\int g(t) \, d\lambda_b(t) \geq 0$ ngoại trừ với $b$ thuộc một tập hợp $\nu$-không đáng kể $N(g)$ (Ch. V, §5, No. 3, Hệ quả 3 của Prop. 3). Bây giờ, tồn tại một dãy trù mật $(g_n)$ trong không gian $\mathcal{K}_+(T)$ của các hàm $\geq 0$ của $\mathcal{K}(T)$ (Bổ đề 1). Hợp N của các $N(g_n)$ là $\nu$-không đáng kể và, với $b \notin N$, ta có $\int g_n(t) \, d\lambda_b(t) \geq 0$ với mọi $n$, do đó $\int g(t) \, d\lambda_b(t) \geq 0$ với mọi hàm $g \in \mathcal{K}_+(T)$, nói cách khác $\lambda_b \geq 0$.

Vì vậy, ta có thể thay thế $\lambda_b$ bởi 0 với mọi $b \in N$ mà không làm thay đổi tính đúng đắn của (3); do đó ta có thể giả sử rằng sự thay đổi này đã được thực hiện, sao cho $\lambda_b \geq 0$ với mọi $b \in B$.

3) *Mở rộng của công thức* (3).

$\alpha)$ Với mọi hàm $f \in \mathcal{L}^1(\nu)$, suy ra từ (3) rằng ánh xạ $b \mapsto \lambda_b$ của B vào $\mathcal{M}(T)$ là khả tích vô hướng đối với độ đo $|f \cdot \nu|$ và tôpô $\sigma(\mathcal{M}(T), \mathcal{K}(T))$, do đó (Bổ đề 3) họ $b \mapsto \lambda_b$ là $|f \cdot \nu|$-*thích hợp*. Bây giờ cho $g$ là một hàm số được xác định trên T, khả tích đối với độ đo $|(f \circ p) \cdot \mu|$, nghĩa là (Ch. V, §5, No. 3, Th. 1), sao cho $t \mapsto g(t)f((p(t)))$ là $\mu$-khả tích; khi đó suy ra từ (2), từ Th. 1 của Ch. V, §3, No. 3 và từ Th. 1 của Ch. V, §5, No. 3 rằng, với hầu hết mọi $b \in B$, $g$ khả tích đối với $\lambda_b$, rằng hàm (được xác định hầu khắp nơi) $b \mapsto \int g(t)\, d\lambda_b(t)$ là khả tích đối với $|f \cdot \nu|$, và rằng công thức (3) lại đúng.

$\beta)$ Với mọi hàm $g \in \overline{\mathcal{K}(T)}$, suy ra từ (3), áp dụng cho $f \in \mathcal{K}(B)$, rằng ánh xạ $p$ là thực sự đối với độ đo $|g \cdot \mu|$ (Ch. V, §6, No. 1, Định nghĩa 1) và ảnh qua $p$ của độ đo $g \cdot \mu$ là độ đo có mật độ $b \mapsto \int g(t)\, d\lambda_b(t)$ đối với $\nu$. Nếu khi đó lấy $f$ là một hàm sao cho $f \circ p$ là khả tích đối với độ đo $|g \cdot \mu|$, tức là sao cho $t \mapsto g(t)f(p(t))$ là $\mu$-khả tích (Ch. V, §5, No. 3, Định lý 1), thì công thức (3) lại đúng (Ch. V, §6, No. 2, Định lý 1).

4) *Các tính chất của họ* $b \mapsto \lambda_b$. Theo tính chất $\beta)$, ta có thể áp dụng công thức (3) bằng cách lấy $f = 1,\ g \in \mathcal{K}(T)$; điều này chứng tỏ rằng $b \mapsto \lambda_b$ là khả tích vô hướng theo $\nu$ (đối với tôpô $\sigma(\mathcal{M}(T), \mathcal{K}(T))$), do đó là $\nu$-*thích hợp* (Bổ đề 3), và rằng $\mu = \int \lambda_b\, d\nu(b)$.

Bây giờ cho $\psi$ là bất kỳ hàm nào trong $\mathcal{K}(B)$; các điều kiện của tính chất $\alpha)$ được thỏa mãn bằng cách lấy $f \in \mathcal{K}(B)$ và $g = \psi \circ p$, vì hàm $\psi(p(t))f(p(t))$ là $\mu$-khả tích do $f\psi$ thuộc $\mathcal{K}(B)$ và $p$ là $\mu$-thực sự. Khi đó $\psi \circ p$ là $\lambda_b$-khả tích với hầu hết mọi $b \in B$, và

$$
\int f(p(t))\psi(p(t))\, d\mu(t) = \int f(b)\, d\nu(b) \int \psi(p(t))\, d\lambda_b(t);
$$

nhưng vế thứ nhất theo định nghĩa là $\int f(b)\psi(b)\, d\nu(b)$. Do đó ta thấy rằng với mọi hàm $\psi \in \mathcal{K}(B)$, độ đo $\psi \cdot \nu$ và độ đo có mật độ $b \mapsto \int \psi(p(t))\, d\lambda_b(t)$ là trùng nhau. Do đó (Ch. V, §5, No. 3, Hệ quả 2 của Mệnh đề 3) tồn tại một tập hợp bỏ qua được theo $\nu$ $N'(\psi)$ sao cho, với mọi $b \notin N'(\psi)$, hàm $\psi \circ p$ là $\lambda_b$-khả tích và $\psi(b) = \int \psi(p(t))\, d\lambda_b(t)$.

Cho $S$ là một tập con đếm được của $\mathcal{K}(B)$ thỏa mãn các tính chất đã nêu trong Bổ đề 1 (với $Y = B$), và cho $N'$ là tập không đáng kể theo $\nu$ là hợp của các $N'(\psi)$ với $\psi \in S$. Mọi hàm $\psi \geq 0$ của $\mathcal{K}(B)$ đều là giới hạn đều của một dãy $(\psi_n)$ gồm các phần tử của S với $\psi_n \leq \psi_0$. Do đó, với $b \notin N'$, định lý Lebesgue cho thấy, một mặt, rằng $\psi \circ p$ là khả tích theo $\lambda_b$, nói cách khác là $p$ là $\lambda_b$-thực sự, và mặt khác rằng $\psi(b) = \int \psi(p(t))\, d\lambda_b(t)$. Nói cách khác, các ánh xạ $b \mapsto \varepsilon_b$ và $b \mapsto p(\lambda_b)$ của B vào $\mathcal{M}(B)$ (ánh xạ sau được xác định hầu khắp nơi) là bằng nhau hầu khắp nơi theo vô hướng đối với $\nu$ (và đối với tôpô $\sigma(\mathcal{M}(B), \mathcal{K}(B))$); suy ra rằng các ánh xạ này bằng nhau hầu khắp nơi đối với $\nu$ (Bổ đề 1 và §1, No. 1, *Nhận xét* 2). Cuối cùng, nếu $p(\lambda_b) = \varepsilon_b$, thì tập $B - \{b\}$ là $\varepsilon_b$-không đáng kể, do đó tập $T - \bar{p}^{-1}(B)$ là $\lambda_b$-không đáng kể (Ch. V, §6, No. 2, Hệ quả 2 của Mệnh đề 2), nói cách khác $\lambda_b$ tập trung trên $\overline{p}^{-1}(b)$; và, mặt khác, $\| \lambda_b \| = \int d\lambda_b = \int d((p(\lambda_b))) = \| \varepsilon_b \| = 1$ (Ch. V, §6, No. 2, Định lý 1).

5) *Sự biến đổi của họ* $b \mapsto \lambda_b$. Như vậy ta đã định nghĩa một họ $\nu$-thích hợp $b \mapsto \lambda_b$ các độ đo $\geqslant 0$ trên T, thỏa mãn điều kiện c) của mệnh đề và sao cho, với hầu hết mọi $b \in B$, $p$ là $\lambda_b$-thực sự, và $\lambda_b$ tập trung trên $\overline{p}^{-1}(b)$ và có chuẩn 1. Gọi $N''$ là tập không đáng kể theo $\nu$ gồm các điểm $b \in B$ tại đó một trong ba tính chất cuối cùng không được thỏa mãn; khi đó ta có thể sửa đổi $\lambda_b$ theo cách sau. Nếu $b \in B - p(T)$, đặt $\lambda_b = 0$; nếu $b \in p(T) \cap N''$, đặt $\lambda_b = \varepsilon_{\xi(b)}$, trong đó $\xi(b)$ là một điểm bất kỳ của $\overline{p}^{-1}(b)$. Vì $B - p(T)$ là tập không đáng kể theo $\nu$ (Ch. V, §6, No. 2, Hệ quả 3 của Mệnh đề 2), ta chỉ mới sửa đổi $\lambda_b$ tại các điểm của một tập không đáng kể, do đó họ $b \mapsto \lambda_b$ vẫn là $\nu$-thích hợp và có tính chất c); hơn nữa, nó nay thỏa mãn a) và b), điều đó hoàn tất chứng minh.

Mọi họ $\nu$-thích hợp $b \mapsto \lambda_b$ các độ đo dương trên T, có các tính chất b) và c) của Định lý 1, được gọi là một *phân rã* của độ đo $\mu$, tương ứng với ánh xạ $p$ $\mu$-thực sự.

### 2. Các độ đo ảnh giả

#### Định nghĩa 1 {#int-vi-s3-def-1 .statement}

*Cho T và B là hai không gian compact địa phương, $\mu$ là một độ đo dương trên T, và p là một ánh xạ $\mu$-khả đo được của T vào B. Một độ đo dương $\nu$ trên B được gọi là một độ đo ảnh giả của $\mu$ dưới p nếu nó thỏa mãn điều kiện sau: để một tập con N của B là địa phương $\nu$-không đáng kể, cần và đủ là $\overline{p}^{-1}(N)$ địa phương $\mu$-không đáng kể.*

#### Ví dụ {#int-vi-s3-n2-exa-1 .statement}

— 1) Nếu $p$ là $\mu$-thực sự và $\nu = p(\mu)$, thì $\nu$ là một độ đo ảnh giả của $\mu$ dưới $p$ (Ch. V, §6, No. 2, Hệ quả 2 của Mệnh đề 2).

2) Cho $B'$ là một không gian compact địa phương, $\nu'$ là một độ đo dương trên $B'$; lấy T là không gian $B \times B'$ và $\mu$ là độ đo $\nu \otimes \nu'$; nếu $p$ là phép chiếu của T lên B, thì $\nu$ là một độ đo ảnh giả của $\mu$ dưới $p$ (Ch. V, §8, No. 2, Mệnh đề 4 và No. 3, Hệ quả 1 của Mệnh đề 7).

Chú ý rằng nếu $\nu$ là một độ đo ảnh giả của $\mu$ dưới $p$, thì $\nu$ được mang bởi $p(T)$.

Nếu $\nu$ là một ảnh giả của $\mu$ dưới $p$, thì tập các độ đo là ảnh giả của $\mu$ dưới $p$ là lớp các độ đo dương tương đương với $\nu$, và mọi độ đo dương tương đương với $\mu$ đều thừa nhận cùng các độ đo ảnh giả dưới $p$. Lớp của $\nu$ được gọi là *lớp ảnh giả* của lớp của $\mu$ dưới $p$.

#### Mệnh đề 1 {#int-vi-s3-prop-1 .statement}

— *Cho T là một không gian compact địa phương đếm được ở vô cùng, $\mu$ là một độ đo dương trên T, và $p$ là một ánh xạ $\mu$-khả đo được của T vào một không gian compact địa phương B. Khi đó tồn tại một độ đo ảnh giả của $\mu$ dưới $p$.*

Vì tồn tại một độ đo *bị chặn* $\mu'$ trên T tương đương với $\mu$ (Ch. V, §5, No. 6, Mệnh đề 11); khi đó $p$ là $\mu'$-thực sự.

### 3. Sự phân rã của một độ đo $\mu$ theo một ảnh giả của $\mu$

#### Định lý 2 {#int-vi-s3-thm-2 .statement}

==========

— *Cho T và B là hai không gian compact địa phương có cơ sở đếm được, $\mu$ là một độ đo dương trên T, $p$ là một ánh xạ $\mu$-đo được từ T vào B, và $\nu$ là một độ đo giả-ảnh của $\mu$ theo $p$. Khi đó tồn tại một họ $\nu$-thích hợp $b \mapsto \lambda_b$ ($b \in B$) các độ đo dương trên T, có các tính chất sau:
a) $\lambda_b \neq 0$ với $b \in p(T)$;
b) $\lambda_b$ tập trung trên tập hợp $\overline{p^{-1}}(b)$ với mọi $b \in B$; đặc biệt, $\lambda_b = 0$ với $b \notin p(T)$;
c) $\mu = \int \lambda_b \, d\nu(b)$.

Hơn nữa, nếu $\nu' = r \cdot \nu$ là một độ đo giả-ảnh thứ hai của $\mu$ theo $p$, và nếu $b \mapsto \lambda'_b$ là một họ $\nu'$-thích hợp các độ đo dương trên T có các tính chất b) và c) đối với $\nu'$, thì $\lambda_b = r(b)\lambda'_b$ hầu khắp nơi trong B (*đối với $\nu$ hoặc $\nu'$*).

Tồn tại một hàm số liên tục và hữu hạn $f$ xác định trên T, sao cho $f(t) > 0$ với mọi $t \in T$ và sao cho $\mu'' = f \cdot \mu$ bị chặn (Ch. V, §5, No. 6, Mệnh đề 11). Gọi $\nu'' = p(\mu'')$, nó tương đương với $\nu$, và viết $\nu'' = g \cdot \nu$, với $g$ hữu hạn và $\nu$-khả tích địa phương; hơn nữa có thể giả sử rằng $g(b) > 0$ với mọi $b \in B$ (Ch. V, §5, No. 6, Mệnh đề 10). Định lý 1 của No. 1, áp dụng cho $\mu''$ và $\nu''$, chỉ ra rằng tồn tại một họ $\nu''$-thích hợp $b \mapsto \lambda''_b$ ($b \in B$) các độ đo dương trên T, sao cho:

1) $\| \lambda''_b \| = 1$ với $b \in p(T)$;
2) $\lambda''_b$ tập trung trên $\overline{p^{-1}}(b)$ với mọi $b \in B$;
3) $\mu'' = \int \lambda''_b \, d\nu''(b)$.

Với mỗi $b \in B$, ta định nghĩa một độ đo dương $\lambda_b$ trên T bởi công thức $\lambda_b = (1/f) \cdot (g(b)\lambda''_b)$. Hiển nhiên rằng họ $b \mapsto \lambda_b$ có các tính chất a) và b) của mệnh đề. Mặt khác, với mọi hàm $h \in \mathcal{K}(T)$, $h/f$ thuộc $\mathcal{K}(T)$, do đó

$$
\int h(t) \, d\mu(t) = \int (h(t)/f(t)) \, d\mu''(t) = \int d\nu''(b) \int (h(t)/f(t)) \, d\lambda''_b(t).
$$

Nhưng vì hàm $b \mapsto \int (h(t)/f(t)) \, d\lambda''_b(t)$ là $\nu''$-khả tích, hàm $b \mapsto g(b) \int (h(t)/f(t)) \, d\lambda''_b(t)$ là $\nu$-khả tích (Ch. V, §5, No. 3, Định lý 1).*

Theo định nghĩa của $\lambda_b$, hàm này là $b \mapsto \int h(t) d\lambda_b(t)$, do đó (*loc. cit.*) $\int h(t) d\mu(t) = \int d\nu(b) \int h(t) d\lambda_b(t)$, điều này chứng minh rằng $\mu = \int \lambda_b d\nu(b)$.

Để thiết lập phần thứ hai của mệnh đề, ta nhận xét rằng có thể giả sử rằng $r(b) > 0$ với mọi $b \in B$ (Ch. V, §5, No. 6, Prop. 10); đặt $\lambda'''_b = f \cdot \left( (r(b)/g(b)) \lambda'_b \right)$; ta chỉ ra, như trên, rằng với mọi hàm $h \in \mathcal{K}(T)$, quan hệ

$$
\int h(t) d\mu(t) = \int d\nu'(b) \int h(t) d\lambda'_b(t)
$$

suy ra

$$
\int h(t) d\mu(t) = \int d\nu''(b) \int (h(t)/f(t)) d\lambda'''_b(t) .
$$

Do đó Đl. 1 của No. 1, áp dụng cho $\mu''$ và $\nu''$, suy ra rằng với hầu hết mọi $b \in B$, $\lambda'''_b = \lambda''_b$, do đó $\lambda_b = r(b)\lambda'_b$.

#### Định nghĩa 2 {#int-vi-s3-def-2 .statement}

*Cho T và B là hai không gian Polish địa phương compact. Cho một độ đo dương $\mu$ trên T, một ánh xạ đo được theo $\mu$ p của T vào B, và một độ đo ảnh giả $\nu$ của $\mu$ theo p, mỗi họ $\nu$-thích hợp $b \mapsto \lambda_b$ ($b \in B$) các độ đo dương trên T có các tính chất b) và c) của Đl. 2 được gọi là một phép phân rã của $\mu$ đối với $\nu$.*

Khi $p$ là $\mu$-thực sự và $\nu = p(\mu)$, khái niệm phân rã đối với $p$ do đó trùng với khái niệm phân rã đối với $\nu$. Dưới các giả thiết của Đl. 2, hai phép phân rã của $\mu$ đối với cùng một độ đo ảnh giả $\nu$ bằng nhau hầu khắp nơi đối với $\nu$.

#### Nhận xét {#int-vi-s3-n3-rem-1 .statement}

— Đl. 1 của Ch. V, §3, No. 4 chỉ ra (có tính đến sự kiện rằng T và B có các cơ sở đếm được) rằng với mọi hàm $f$ xác định trên T, có giá trị trong $\overline{\mathbf{R}}$ hoặc trong một không gian Banach F và $\mu$-khả tích, tập hợp các $b \in B$ sao cho $f$ không $\lambda_b$-khả tích là không đáng kể đối với $\nu$, hàm $b \mapsto \int f(t) d\lambda_b(t)$, được xác định hầu khắp nơi, là $\nu$-khả tích, và

$$
\int f(t) d\mu(t) = \int d\nu(b) \int f(t) d\lambda_b(t) .
$$

Một kết quả tương tự đúng cho các hàm khả tích vô hướng theo $\mu$, khi áp dụng Prop. 3 của §1, No. 1.

### 4. Các quan hệ tương đương đo được

Cho một không gian tôpô X và một quan hệ tương đương R trong X, ta sẽ nói rằng R là *Hausdorff* nếu không gian thương X/R là Hausdorff.

Nhắc lại (GT, I, §8, No. 3, Prop. 8) rằng khi R là một quan hệ tương đương mở, việc nói rằng đồ thị của R trong X × X là đóng là tương đương.

Cho p là một ánh xạ của X vào một không gian tôpô Hausdorff B, và cho R là quan hệ tương đương $p(x) = p(y)$ trong X; nếu K là một tập con compact của X sao cho hạn chế của p trên K là liên tục, thì quan hệ $R_K$ cảm sinh bởi R trên K là Hausdorff, bởi vì không gian thương $K / R_K$ là đồng phôi với không gian $p(K)$, là compact (GT, I, §9, No. 4, Th. 2 và Hệ quả của nó 2). Nếu T là một không gian địa phương compact, $\mu$ là một độ đo dương trên T, và p là một ánh xạ đo được theo $\mu$ của T vào một không gian tôpô Hausdorff B, thì do đó ta thấy rằng tồn tại một tập hợp $\mu$-trù mật (Ch. IV, §5, No. 8) các tập con compact K của T sao cho quan hệ $R_K$ là Hausdorff. Vì vậy ta được dẫn đến định nghĩa sau:

#### Định nghĩa 3 {#int-vi-s3-def-3 .statement}

*Cho T là một không gian địa phương compact, $\mu$ một độ đo dương trên T. Một quan hệ tương đương R trong T được gọi là $\mu$-đo được nếu tồn tại một tập hợp $\mu$-trù mật các tập con compact K của T sao cho quan hệ $R_K$ là Hausdorff.*

Nếu R là Hausdorff thì R là $\mu$-đo được, bởi vì nếu $\varphi$ là ánh xạ chính tắc của T lên không gian tôpô Hausdorff T/R, $\varphi$ liên tục và R tương đương với $\varphi(x) = \varphi(y)$. Tương tự, nếu R có tính chất là bao đóng bão hòa theo R của mọi tập con compact của T là đóng (đặc biệt, nếu R là một quan hệ tương đương đóng), thì R là $\mu$-đo được, bởi vì với mọi tập con compact K của T, quan hệ $R_K$ là đóng, do đó là Hausdorff (GT, I, §10, No. 4, Prop. 8).

Chú ý rằng nếu R là $\mu$-đo được, thì R cũng đo được đối với mọi độ đo trên T có cơ sở $\mu$.

#### Mệnh đề 2 {#int-vi-s3-prop-2 .statement}

*Cho T là một không gian địa phương compact đếm được tại vô hạn, $\mu$ là một độ đo dương trên T.

1) Đối với mọi quan hệ tương đương $\mu$-đo được R trong T, tồn tại một không gian địa phương compact B và một ánh xạ $\mu$-đo được p của T vào B sao cho R tương đương với quan hệ $p(x) = p(y)$.

2) Nếu hơn nữa T có một cơ sở đếm được, có thể giả sử rằng B có một cơ sở đếm được.*

Vì T là đếm được tại vô hạn, tồn tại một dãy tăng $(K_n)_{n \geq 1}$ các tập con compact của T sao cho T là hợp của các $K_n$ và một tập hợp $\mu$-không đáng kể N, và sao cho mỗi quan hệ $R_{K_n}$ là Hausdorff. Gọi $B_n$ là không gian thương $K_n / R_{K_n}$, là compact, và gọi $B'_n$ là không gian compact là tổng tôpô của $B_n$ và một điểm $a_n$. Gọi $q_n$ là ánh xạ chính tắc của $K_n$ lên $B_n$; ta mở rộng $q_n$ thành một ánh xạ $p_n$ của T vào $B'_n$ theo cách sau: nếu $x \in T$ tương đương mod R với một phần tử $y \in K_n$, đặt $p_n(x) = q_n(y)$; trong trường hợp ngược lại, đặt $p_n(x) = a_n$.

Gọi $B'$ là không gian tích $\prod_{n=1}^{\infty} B'_n$, là compact, và gọi $p'$ là ánh xạ $x \mapsto (p_n(x))$ của T vào B'. Ta hãy chứng minh rằng $p'$ là $\mu$-đo được: chỉ cần (Ch. IV, §5, No. 3, Th. 1) chứng minh rằng mỗi ánh xạ $p_n$ là đo được, và để làm điều này chỉ cần chứng minh rằng hạn chế của $p_n$ trên mỗi $K_m$ là đo được. Bây giờ, điều này là hiển nhiên nếu $m \leq n$; nếu ngược lại, $m > n$, gọi $K_{nm}$ là bão hòa của $K_n$ đối với $R_{K_m}$, là một tập con compact của $K_m$ (GT, I, §9, No. 4, Th. 2); vì $p_n$ là hằng trên $K_m - K_{nm}$, chỉ cần chứng minh rằng hạn chế của $p_n$ trên $K_{nm}$ là liên tục, điều này là hiển nhiên do đẳng cấu chính tắc giữa $K_{nm}/R_{K_{nm}}$ và $K_n/R_{K_n}$ (GT, I, §9, No. 4, Cor. 4 of Th. 2).

Let A là sự bão hòa của $\bigcup_n K_n$ đối với quan hệ R, và đặt $N' = T - A \subset N$. Ta sẽ thấy rằng quan hệ $p'(x) = p'(y)$ tương đương với quan hệ «$R\{x, y\}$ hoặc $(x, y) \in N' \times N'$ ». Thật vậy, nếu $R\{x, y\}$ thì $p_n(x) = p_n(y)$ với mọi $n$, do đó $p'(x) = p'(y)$; và nếu $x \in N'$, $y \in N'$ thì $p_n(x) = p_n(y) = a_n$ với mọi $n$, do đó $p'(x) = p'(y)$. Mặt khác, nếu $x$ và $y$ ở trong A và không tương đương mod R, thì tồn tại một số nguyên $n$, một phần tử $x' \in K_n$ (tương ứng $y' \in K_n$) tương đương mod R với $x$ (tương ứng $y$) sao cho $x'$ không tương đương với $y'$ mod $R_{K_n}$; do đó $p_n(x) \neq p_n(y)$, suy ra $p'(x) \neq p'(y)$. Cuối cùng, nếu $x \in N'$ và $y \in A$, thì $p_n(y) \in B_n$ với $n$ đủ lớn và $p_n(x) = a_n$ với mọi $n$, do đó $p'(x) \neq p'(y)$, điều này thiết lập mệnh đề của chúng ta.

Xét tập thương $B_0 = N'/R_{N'}$; gọi $q_0$ là ánh xạ chính tắc của $N'$ lên $B_0$, $s_0$ một tiết diện của $q_0$. Đặt $p_0(x) = s_0(q_0(x))$ với $x \in N'$ và mở rộng $p_0$ lên T bằng cách cho $p_0$ là hằng trên A, bằng một phần tử của T. Khi đó $p = (p', p_0)$ là một ánh xạ $\mu$-đo được của T vào không gian địa phương compact $B = B' \times T$; hiển nhiên nếu $x \in N'$, $y \in N'$, quan hệ $p_0(x) = p_0(y)$ suy ra $R\{x, y\}$; do đó $p$ thỏa mãn các yêu cầu. Hơn nữa, nếu T thừa nhận một cơ sở đếm được, thì mỗi không gian thương $B_n$ cũng vậy (GT, IX, §2, No. 10, Prop. 17), do đó $B'$ thừa nhận một cơ sở đếm được, suy ra $B$ cũng thế.

#### Mệnh đề 3 {#int-vi-s3-prop-3 .statement}

— *Cho T là một không gian địa phương compact Polish, $\mu$ là một độ đo dương trên T, và R là một quan hệ tương đương trong T. Các tính chất sau là tương đương:*

a) $R$ là $\mu$-đo được.

b) *Tồn tại một dãy các ánh xạ $p_n : T \to F_n$ vào các không gian tôpô Hausdorff, sao cho mỗi $p_n$ là $\mu$-đo được và sao cho quan hệ $R\{x, y\}$ tương đương với «với mọi $n$, $p_n(x) = p_n(y)$».*

c) *Tồn tại một dãy $(A_n)$ các tập hợp $\mu$-đo được, bão hòa đối với R, sao cho với mọi $x \in T$ lớp của x đối với R là giao của những $A_n$ chứa x.*

Với ký hiệu như trong phát biểu b), đặt $p(x) = (p_n(x))$; tính chất b) có nghĩa là ánh xạ $p$ từ T vào không gian tích $\prod F_n$ là đo được (Chương IV, §5, No. 3, Định lý 1) và quan hệ $R\{x, y\}$ tương đương với $p(x) = p(y)$; do đó b) suy ra a).

Tiếp theo ta hãy chứng minh rằng c) suy ra b). Giả sử c) được thỏa mãn; khi đó các hàm đặc trưng $\varphi_{A_n}$ là $\mu$-đo được, và giả thiết c) có nghĩa là quan hệ $R\{x, y\}$ tương đương với «với mọi $n$, $\varphi_{A_n}(x) = \varphi_{A_n}(y)$».

Cuối cùng, ta hãy chứng minh rằng a) suy ra c). Theo Mệnh đề 2, tồn tại một không gian compact địa phương B có một cơ sở đếm được, và một ánh xạ $\mu$-đo được $p$ của T vào B, sao cho quan hệ $R\{x, y\}$ tương đương với $p(x) = p(y)$. Hãy lấy $(U_n)$ là một cơ sở đếm được cho tôpô của B. Các tập hợp $A_n = \overline{p^{-1}(U_n)}$ là $\mu$-đo được (Chương IV, §5, No. 5, Mệnh đề 7) và bão hòa đối với R; và nếu $x, y$ là các điểm của T sao cho $p(x) \neq p(y)$, thì tồn tại một chỉ số $n$ sao cho $p(x) \in U_n$ và $p(y) \notin U_n$, nghĩa là $x \in A_n$ và $y \notin A_n$.

#### Nhận xét {#int-vi-s3-n4-rem-1 .statement}

Nếu R là một quan hệ tương đương $\mu$-đo được trong T, thì sự bão hòa đối với R của một tập con compact của T không nhất thiết $\mu$-đo được (Bài tập 5).

#### Định lý 3 {#int-vi-s3-thm-3 .statement}

— *Cho T là một không gian compact địa phương có một cơ sở đếm được, $\mu$ là một độ đo dương trên T, và R là một quan hệ tương đương $\mu$-đo được trong T. Khi đó, tồn tại một tập hợp con $\mu$-đo được S của T giao với mỗi lớp theo R tại một và chỉ một điểm (một 'tiết diện đo được' cho R).*

Ta có thể rõ ràng giả sử rằng độ đo $\mu$ bị chặn và rằng $\mu(T) \leq 1$ (Chương V, §5, No. 6, Mệnh đề 11). Ta sẽ định nghĩa một dãy $(S_n)$ các tập hợp con *Borel* (GT, IX, §6, No. 3) sao cho mỗi lớp tương đương theo R cắt hợp $S'$ của các $S_n$ nhiều nhất tại một điểm, sao cho với mọi n sự bão hòa $T_n$ của hợp các $S_p$ với chỉ số $p \leq n$ là $\mu$-đo được, và sao cho $\mu(T - T_n) \leq 1/2^n$. Do đó sự bão hòa $T'$ của $S'$ sẽ là $\mu$-đo được và $N = T - T'$ sẽ có độ đo bằng không. Nếu $S''$ là bất kỳ một tiết diện nào của N đối với quan hệ $R_N$, thì $S = S' \cup S''$ sẽ thỏa các yêu cầu, vì $S'$, là một tập Borel, là $\mu$-đo được (Chương IV, §5, No. 4, Hệ quả 3 của Định lý 2), và $S''$ có độ đo bằng không.

Theo Mệnh đề 2, $R\{x, y\}$ tương đương với quan hệ $p(x) = p(y)$, trong đó $p$ là một ánh xạ $\mu$-đo được từ T vào một không gian địa phương compact F. Giả sử các $S_k$ đã được xác định với $k \leq n$. Vì $T - T_n$ là $\mu$-đo được và có độ đo $\leq 1/2^n$, nên tồn tại một tập con compact K của $T - T_n$ sao cho $\mu(T - (T_n \cup K)) \leq 1/2^{n+1}$ và sao cho hạn chế của $p$ lên K là liên tục. Vì quan hệ cảm sinh $R_K$ là đóng và K là khả metrizable, ta biết rằng tồn tại một tập con Borel $S_{n+1}$ của K sao cho, trong K, mỗi điểm tương đương (mod R) với một và chỉ một điểm của $S_{n+1}$ (GT, IX, §6, No. 8, Định lý 4). Do đó $p(S_{n+1}) = p(K)$, là một tập compact trong F; bao đóng bão hòa của $S_{n+1}$ đối với R là ảnh ngược $\overline{p^{-1}(p(K))}$, vì thế là $\mu$-đo được (Ch. IV, §5, No. 5, Mệnh đề 7); rõ ràng tập này chứa K, do đó hợp $T_{n+1}$ của $T_n$ và $\overline{p}^{-1}(p(K))$ là $\mu$-đo được, bão hòa đối với R, và thỏa mãn $\mu(T - T_{n+1}) \leq 1/2^{n+1}$, điều này hoàn tất chứng minh.

### 5. Phân rã của một độ đo theo một quan hệ tương đương đo được

Cho T là một không gian Polish địa phương compact, $\mu$ là một độ đo dương trên T, và R là một quan hệ tương đương $\mu$-đo được trong T. Khi đó, tồn tại (No. 4, Mệnh đề 2) một không gian Polish địa phương compact B và một ánh xạ $\mu$-đo được p của T vào B, sao cho quan hệ $p(x) = p(y)$ tương đương với R$\{x, y\}$. Mọi độ đo $\nu$ là một ảnh giả của $\mu$ theo p (No. 2) sẽ được gọi là một *độ đo thương của $\mu$ theo quan hệ* R; nếu $b \mapsto \lambda_b$ là một sự phân rã của $\mu$ tương đối với độ đo $\nu$, ta sẽ nói rằng $b \mapsto \lambda_b$ là một *sự phân rã của $\mu$ theo quan hệ* R. Nhờ các tính chất của p và của các $\lambda_b$, mỗi độ đo $\lambda_b$ đều tập trung trên một lớp tương đương đối với R, và nếu $b \neq c$, thì các độ đo $\lambda_b$ và $\lambda_c$ tập trung trên các lớp phân biệt.

Không gian B, ánh xạ p và độ đo ảnh giả $\nu$ trên B nói chung có thể được chọn theo vô hạn cách khác nhau. Tuy nhiên, các sự phân rã khác nhau của $\mu$ theo R đều có thể suy ra từ một trong số chúng, như là hệ quả của định lý sau:

#### Định lý 4 {#int-vi-s3-thm-4 .statement}

*Cho T là một không gian Polish địa phương compact, $\mu$ là một độ đo dương trên T, và R là một quan hệ tương đương $\mu$-đo được trong T. Cho B, B' là hai không gian Polish địa phương compact, p, p' là hai ánh xạ $\mu$-đo được của T vào B, B' tương ứng, sao cho R$\{x, y\}$ tương đương với $p(x) = p(y)$ và với $p'(x) = p'(y)$. Cho $\nu, \nu'$ là các độ đo ảnh giả của $\mu$ theo p, p' tương ứng; cho $b \mapsto \lambda_b, b' \mapsto \lambda_{b'}$ là các sự phân rã của $\mu$ tương ứng với các độ đo $\nu, \nu'$.*

*Dưới các giả thiết này, tồn tại trong B (tương ứng B') một tập N (tương ứng N') không đáng kể đối với $\nu$ (tương ứng $\nu'$) và một song ánh f từ B - N lên B' - N', có các tính chất sau:*

a) *Ánh xạ $f$ (được định nghĩa hầu khắp trên $B$) là $\nu$-khả đo và ánh xạ nghịch đảo $f'$ của nó là $\nu'$-khả đo; mọi độ đo ảnh giả của $\nu$ (resp. $\nu'$) dưới $f$ (resp. $f'$) đều tương đương với $\nu'$ (resp. $\nu$).*

b) *Với mọi $b \in B - N$, độ đo $\lambda'_{f(b)}$ trên $T$ có dạng $r(b)\lambda_b$, trong đó $r(b) \neq 0$ và $r$ là địa phương $\nu$-tích phân.*

Để chứng minh a), ta có thể hạn chế vào trường hợp $\nu$ và $\nu'$ là các độ đo *bị chặn* (Ch. V, §5, No. 6, Mệnh đề 11). Đặt $N_0 = B - p(T)$, $N'_0 = B' - p'(T)$; ta biết rằng $N_0$ (resp. $N'_0$) là không đáng kể đối với $\nu$ (resp. $\nu'$) (No. 2). Tồn tại một song ánh f từ B - $N_0$ lên B' - $N'_0$ được xác định bởi $f(p(t)) = p'(t)$ với mọi $t \in T$; gọi $f'$ là ánh xạ nghịch đảo của $f$, sao cho $f'(p'(t)) = p(t)$. Với mọi tập con M của B, quan hệ « M là $\nu$-đo được » tương đương với « $\overline{p}^{-1}(M)$ là $\mu$-đo được », tức là với « $p'(f(M))$ là $\mu$-đo được », do đó cuối cùng tương đương với « $f(M)$ là $\nu'$-đo được » (Ch. V, §6, No. 2, Hệ quả của Mệnh đề 3). Do đó ta thấy rằng $f$ (resp. $f'$) biến mọi tập $\nu$-đo được (resp. $\nu'$-đo được) thành một tập $\nu'$-đo được (resp. $\nu$-đo được); vì B và $B'$ là khả metric và có cơ sở đếm được, suy ra $f$ và $f'$ là đo được (Ch. IV, §5, No. 5, Định lý 4). Hơn nữa, nếu $M \subset B$ là $\nu$-không đáng kể thì $\overline{p}^{-1}(M) = p'(f(M))$ là $\mu$-không đáng kể, do đó $f(M)$ là $\nu'$-không đáng kể (Ch. V, §6, No. 2, Hệ quả 2 của Mệnh đề 2); tương tự, $f'$ biến mọi tập $\nu'$-không đáng kể thành một tập $\nu$-không đáng kể. Do đó, ảnh của $\nu$ qua $f$ (được định nghĩa vì $\nu$ bị chặn, điều này suy ra rằng $f$ là $\nu$-thực sự) tương đương với $\nu'$, và ảnh của $\nu'$ qua $f'$ tương đương với $\nu$ (Ch. V, §5, No. 6, Mệnh đề 10). Còn phải chứng minh b). Nhờ Định lý 2 của No. 3, ta có thể chỉ xét trường hợp $\nu' = f(\nu)$. Vì $\mu = \int \lambda_{b'}' d\nu'(b')$, ta có, với mọi hàm $h \in \mathcal{K}(T)$,

$$
\int h(t) d\mu(t) = \int d\nu'(b') \int h(t) d\lambda_{b'}'(t) = \int d\nu(b) \int h(t) d\lambda_{f(b)}'(t)
$$

(Ch. V, §3, No. 4, Định lý 1 và §6, No. 2, Định lý 1); nói cách khác, $\mu = \int \lambda_{f(b)}' d\nu(b)$. Nhưng vì đồng thời $\mu = \int \lambda_b d\nu(b)$ và vì, với mọi $b \in B - N_0$, $\lambda_b$ và $\lambda_{f(b)}'$ được mang bởi $\overline{p}^{-1}(b)$, Định lý 2 của No. 3 suy ra rằng $\lambda_b = \lambda_{f(b)}'$ với hầu hết mọi $b \in B - N_0$, do đó với hầu hết mọi $b \in B$. Các điều kiện của Định lý 4 vì thế được thỏa mãn bằng cách lấy N là hợp của $N_0$ và tập hợp các $b \in B$ sao cho $\lambda_b \neq \lambda_{f(b)}'$.

### Bài tập {#int-vi-s3-exercises}

Xem [bài tập cho § 3](exercises/s3/).
