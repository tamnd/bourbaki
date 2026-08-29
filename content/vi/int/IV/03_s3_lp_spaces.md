---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 3
section_title: LP spaces
lang: vi
source: int-i-vi
book_pages: INT IV.18-INT IV.32, INT IV.120
pdf_pages: 0125-0139, 0227-0227
extraction: ocr
subsections:
    - "no": 1
      title: Minkowski’s inequality
      page: 18
      pdf_page: 125
    - "no": 2
      title: The semi-norms $N_p$
      page: 19
      pdf_page: 126
    - "no": 3
      title: The spaces $\mathcal{F}_F^p$
      page: 20
      pdf_page: 127
    - "no": 4
      title: $p$-th power integrable functions
      page: 23
      pdf_page: 130
    - "no": 5
      title: Properties of $p$-th power integrable functions
      page: 25
      pdf_page: 132
    - "no": 6
      title: Directed sets in $L^p$ and increasing sequences in $\mathcal{L}^p$
      page: 27
      pdf_page: 134
    - "no": 7
      title: Lebesgue’s theorem
      page: 30
      pdf_page: 137
    - "no": 8
      title: Relations between the spaces $\mathcal{L}_F^p$ ($1 \leq p < +\infty$)
      page: 31
      pdf_page: 138
statements: 43
exercises: 3
content_sha256: 4a57a98e507e96be2e7a08932445fa343c566b842907c923e06bff4a2163a1a4
translated_from: content/en/int/IV/03_s3_lp_spaces.md
source_content_sha256: 990c6868635eb8d33252eba948d26e29837eae81e092411c1ee46078be262311
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-4243370b
glossary_version: 34
glossary_terms_sha256: 664180aaefdf1893b8bedf8fcf079ecfc2b6113b74ad04f036c126498e73063c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC KHÔNG GIAN L$^p$

### 1. Bất đẳng thức Minkowski

Cho X là một không gian địa phương compact, $\mu$ là một độ đo trên X. Trong tập hợp các hàm số dương (hữu hạn hoặc không) xác định trên X, hàm $|\mu|^*(f)$ là dương, thuần nhất dương, tăng và lồi ($§ 1$, No. 3, Props. 10, 11 và 12).

#### Mệnh đề 1 {#int-iv-s3-prop-1 .statement}

— Với mọi số thực $p \geqslant 1$ và mọi cặp hàm dương $f, g$ (hữu hạn hoặc không) xác định trên X,

$$
(|\mu|^*((f + g)^p))^{1/p} \leqslant (|\mu|^*(f^p))^{1/p} + (|\mu|^*(g^p))^{1/p}
$$

(bất đẳng thức Minkowski).

Bất đẳng thức (1) là hiển nhiên khi một trong các số hạng của vế thứ hai bằng $+\infty$. Trong trường hợp ngược lại, $f$ và $g$ hữu hạn hầu khắp nơi ($§ 2$, No. 3, Prop. 7). Nếu $f_1$ và $g_1$ là các hàm dương hữu hạn tương đương lần lượt với $f$ và $g$, thì $f_1^p, g_1^p$ và $(f_1 + g_1)^p$ lần lượt tương đương với $f^p, g^p$ và $(f + g)^p$, và vì các hàm dương tương đương có cùng tích phân trên ($§ 2$, No. 3, Prop. 6), ta quy về việc chứng minh bất đẳng thức (1) trong trường hợp $f$ và $g$ hữu hạn khắp nơi; nhưng trong trường hợp này bất đẳng thức là một trường hợp riêng của bất đẳng thức Minkowski tổng quát đã được chứng minh trong Ch. I, No. 2, Prop. 3.

Ta cũng sẽ có dịp sử dụng bất đẳng thức sơ cấp sau đây: nếu $p \geqslant 1$ thì, với mọi số $a \geqslant 0,\ b \geqslant 0$,

$$
a^p + b^p \leqslant (a + b)^p .
$$

Bất đẳng thức là hiển nhiên nếu $a = b = 0$ hoặc nếu một trong hai số $a, b$ bằng $+\infty$; nếu $a, b$ hữu hạn và $a + b > 0$, nó có thể viết thành

$$
\left( \frac{a}{a + b} \right)^p + \left( \frac{b}{a + b} \right)^p \leqslant 1 ,
$$

điều này suy ra từ

$$
\left( \frac{a}{a + b} \right)^p \leqslant \frac{a}{a + b} , \quad \left( \frac{b}{a + b} \right)^p \leqslant \frac{b}{a + b} \quad \text{và} \quad \frac{a}{a + b} + \frac{b}{a + b} = 1 .
$$

### 2. Các nửa chuẩn $N_p$

Trong toàn bộ phần sau, $F$ ký hiệu một không gian vectơ *đầy đủ có chuẩn* (nghĩa là một không gian Banach) trên trường $\mathbf{R}$ hoặc trường $\mathbf{C}$; *chuẩn* của một phần tử $z \in F$ được ký hiệu là $|z|$. Cho một ánh xạ $f$ của một tập hợp $A$ vào $F$, ta viết $|f|$ để chỉ ánh xạ $x \mapsto |f(x)|$ của $A$ vào $\mathbf{R}_+$ (cần lưu ý rằng $|f|$ là một *hàm số*, chứ không phải một *số*).

#### Định nghĩa 1 {#int-iv-s3-def-1 .statement}

*Cho $X$ là một không gian địa phương compact, $\mu$ là một độ đo trên $X$. Với mọi ánh xạ $f$ của $X$ vào một không gian Banach $F$, và với mọi số $p$ sao cho $1 \leq p < +\infty$, ta ký hiệu $N_p(f, \mu)$, hoặc đơn giản là $N_p(f)$, là số dương* $(\int^* |f|^p d|\mu|)^{1/p}$.

Chú ý rằng số $N_p(f)$ có thể bằng $+\infty$.

#### Mệnh đề 2 {#int-iv-s3-prop-2 .statement}

*Giả sử $f$ và $g$ là hai ánh xạ từ $X$ vào $F$, và $\alpha$ là một vô hướng bất kỳ $\neq 0$, khi đó, với $1 \leq p < +\infty$,

(3) $$
N_p(\alpha f) = |\alpha| N_p(f)
$$
(4) $$
N_p(f + g) \leq N_p(f) + N_p(g).
$$

Thật vậy, quan hệ (3) suy ra ngay lập tức từ Định nghĩa 1 và sự kiện rằng $|\mu|^*$ là thuần nhất dương; mặt khác, vì $|f + g| \leq |f| + |g|$, bất đẳng thức (4) suy ra từ bất đẳng thức Minkowski (1) và sự kiện rằng $|\mu|^*$ là tăng.

Ta mở rộng Định nghĩa 1 sang trường hợp các hàm số, *hữu hạn hoặc không*, xác định trên $X$, bằng cách một lần nữa đặt

$$
N_p(f) = \left( \int^* |f|^p d|\mu| \right)^{1/p}
$$

đối với một hàm như vậy $f$. Ta thấy ngay lập tức rằng các quan hệ (3) và (4) cũng đúng đối với các hàm này khi $f + g$ được xác định trên $X$ và $\alpha \neq 0$. Hơn nữa:

#### Định lý 1 (định lý lồi đếm được) {#int-iv-s3-thm-1 .statement}

— *Cho $(f_n)$ là một dãy các hàm $\geq 0$ (hữu hạn hoặc không) xác định trên $X$. Với $1 \leq p < +\infty$,

(5) $$
N_p \left( \sum_{n=1}^\infty f_n \right) \leq \sum_{n=1}^\infty N_p(f_n).
$$

Đặt $f = \sum_{n=1}^\infty f_n$; $f$ là bao trên của dãy tăng các hàm $g_n = \sum_{k=1}^n f_k$; định nghĩa của $N_p(f)$, và Định lý 3 của §1, No. 3, cho thấy rằng $N_p(f) = \sup_n N_p(g_n)$. Nhưng $N_p(g_n) \leq \sum_{k=1}^n N_p(f_k)$ theo Mệnh đề 1, do đó bất đẳng thức (5).

#### Mệnh đề 3 {#int-iv-s3-prop-3 .statement}

*Nếu f và g là hai ánh xạ tương đương từ X vào một không gian Banach F, thì $N_p(f - g) = 0$ với $1 \leq p < +\infty$; ngược lại, nếu $N_p(f - g) = 0$ với một giá trị $p \geq 1$ thì f và g tương đương.*

Mệnh đề suy ra ngay lập tức từ Định lý 1 của §2, No. 3.

Nếu f và g là hai ánh xạ tương đương từ X vào F, thì $N_p(f) = N_p(g)$ với mọi $p \geq 1$ (§ 2, No. 3, Mệnh đề 6); do đó, $N_p(f)$ chỉ phụ thuộc vào lớp $\tilde{f}$ của f, và ta đặt, theo định nghĩa, $N_p(\tilde{f}) = N_p(f)$. Vì các lớp các ánh xạ từ X vào F tạo thành một không gian vectơ (§ 2, No. 4), các quan hệ (3) và (4) cũng có thể được viết

$$
(6) \quad N_p(\alpha \tilde{f}) = |\alpha| N_p(\tilde{f})
$$
$$
(7) \quad N_p(\tilde{f} + \tilde{g}) \leq N_p(\tilde{f}) + N_p(\tilde{g}).
$$

Ta định nghĩa tương tự $N_p(\tilde{f})$ cho mọi lớp các hàm số tương đương (hữu hạn hoặc không).

Khi đó ta có thể định nghĩa $N_p(f)$ cho một hàm có giá trị trong F (tương ứng trong $\overline{\mathbf{R}}$) được xác định hầu khắp nơi trong X, bằng cách đặt $N_p(f) = N_p(\tilde{f})$; khi đó hiển nhiên rằng các quan hệ (3) và (4) lại đúng (giả sử $\alpha \neq 0$ và $f + g$ được xác định hầu khắp nơi, trong trường hợp các hàm số, hữu hạn hoặc không).

Nếu $0 < p < 1$, ta lại đặt $N_p(f) = (\int^* |f|^p d|\mu|)^{1/p}$, nhưng các bất đẳng thức (4) và (5) không còn đúng nữa (xem Ch. I, Bài tập 6 và Ch. IV, §6, Bài tập 13).

### 3. Các không gian $\mathcal{F}_F^p$

Cho F là một không gian Banach, $\mathcal{F}(X; F)$ (hoặc đơn giản là $\mathcal{F}_F$) là không gian vectơ của tất cả các ánh xạ từ X vào F. Với $1 \leq p < +\infty$ ta sẽ ký hiệu bởi $\mathcal{F}^p(X, \mu; F)$ hoặc $\mathcal{F}_F^p(X, \mu)$, hoặc đơn giản là $\mathcal{F}_F^p(\mu)$, hoặc $\mathcal{F}_F^p$ (nếu không thể xảy ra nhầm lẫn), tập hợp các ánh xạ f từ X vào F sao cho $N_p(f) < +\infty$ (ta viết $\mathcal{F}^p$ thay cho $\mathcal{F}_R^p$). Rõ ràng là $\mathcal{F}_F^p(|\mu|) = \mathcal{F}_F^p(\mu)$. Suy ra ngay từ Mệnh đề 2 của No. 2 rằng $\mathcal{F}_F^p$ là một *không gian con tuyến tính* của $\mathcal{F}_F$ và rằng $N_p(f)$ là một *bán chuẩn* trên không gian này. Ta sẽ luôn giả thiết (trừ khi có nói rõ ngược lại) rằng $\mathcal{F}_F^p$ được trang bị tôpô xác định bởi bán chuẩn này; ta sẽ nói rằng tôpô này là *tôpô hội tụ trung bình cấp p* (với $p = 1$, ta gọi đơn giản là *tôpô hội tụ trung bình*; với $p = 2$, người ta cũng nói «tôpô hội tụ theo trung bình bình phương»). Ta sẽ nói rằng một lọc $\mathcal{G}$ trên $\mathcal{F}_F^p$ (tương ứng một dãy $(f_n)$ các phần tử của $\mathcal{F}_\mathbf{F}^p$) hội tụ đến f theo tôpô này *hội tụ trung bình cấp* $p$ đến f; điều này có nghĩa là, do đó, $N_p(g - f)$ tiến tới 0 đối với $\mathcal{G}$ (tương ứng $N_p(f_n - f)$ tiến tới 0 khi n tiến tới vô hạn).

Thuật ngữ này được mở rộng ngay lập tức đến trường hợp các hàm $f_n$ và hàm $f$ chỉ được xác định hầu khắp nơi (hoặc có các giá trị trong $\overline{\mathbf{R}}$, và được xác định và hữu hạn hầu khắp nơi).

Chú ý rằng không gian lồi địa phương $\mathcal{F}_\mathbf{F}^p$ nói chung *không Hausdorff*; bao đóng của 0 trong không gian này là không gian con tuyến tính $\mathcal{N}_\mathbf{F}$ của các ánh xạ *không đáng kể* từ X vào F (No. 2, Mệnh đề 3).

#### Nhận xét {#int-iv-s3-n3-rem-1 .statement}

— Cho F là một không gian Banach *trên trường* $\mathbf{C}$ các số phức; khi đó, với mọi hàm $f \in \mathcal{F}_\mathbf{F}^p$ và mọi số phức $\alpha$, $\alpha f$ thuộc về $\mathcal{F}_\mathbf{F}^p$ và $N_p(\alpha f) = |\alpha| N_p(f)$; nói cách khác, $\mathcal{F}_\mathbf{F}^p$ cũng là một không gian vectơ trên $\mathbf{C}$, và $N_p(f)$ là một bán chuẩn trên không gian vectơ phức này (TVS, II, §1).

#### Mệnh đề 4 {#int-iv-s3-prop-4 .statement}

*Cho $\mathcal{B}$ là một cơ sở lọc trên $\mathcal{F}_\mathbf{F}^p$. Giả sử tồn tại một tập compact $K \subset X$ sao cho, với mọi tập hợp $M \in \mathcal{B}$, tất cả các ánh xạ $f \in M$ đều có giá được chứa trong K. Dưới các điều kiện này, nếu $\mathcal{B}$ hội tụ đều trên X đến $f_0$, thì $f_0$ thuộc về $\mathcal{F}_\mathbf{F}^p$ và $\mathcal{B}$ hội tụ trung bình cấp $p$ đến $f_0$.*

Điều này tương đương với việc nói rằng, trên tập hợp các ánh xạ $f \in \mathcal{F}_\mathbf{F}^p$ có giá được chứa trong một tập compact cố định, tôpô hội tụ đều là *mịn hơn* tôpô hội tụ trung bình cấp $p$.

Do đó, cho $h$ là một ánh xạ liên tục của X vào $[0,1]$, có giá compact, bằng 1 trên K (Ch. III, §1, No. 2, Bổ đề 1). Với mọi $\varepsilon > 0$, tồn tại một $M \in \mathcal{B}$ sao cho, với mọi ánh xạ $f \in M$, $|f(x) - f_0(x)| \leq \varepsilon h(x)$ với mọi $x \in X$. Từ đó, suy ra rằng $N_p(f - f_0) \leq \varepsilon N_p(h)$, do đó có mệnh đề.

#### Mệnh đề 5 {#int-iv-s3-prop-5 .statement}

*Không gian lồi địa phương $\mathcal{F}_\mathbf{F}^p$ là đầy đủ.*

Vì không gian Hausdorff liên kết với $\mathcal{F}_\mathbf{F}^p$ là một không gian chuẩn, chỉ cần chứng minh rằng mọi *dãy Cauchy* $(f_n)$ trong $\mathcal{F}_\mathbf{F}^p$ đều có một giới hạn đối với tôpô hội tụ theo trung bình cấp $p$ (GT, IX, §2, No. 6, Mệnh đề 9). Theo giả thiết, với mọi $\varepsilon > 0$ tồn tại một số nguyên $m_0$ sao cho các quan hệ $m \geq m_0,\ n \geq m_0$ kéo theo $N_p(f_n - f_m) \leq \varepsilon$. Do đó, có thể định nghĩa, bằng quy nạp theo $k$, một dãy tăng ngặt $(n_k)$ các số nguyên $\geq 0$ sao cho $N_p(f_{n_{k+1}} - f_{n_k}) \leq 2^{-k}$. Nếu ta chứng minh rằng chuỗi với số hạng tổng quát $g_k = f_{n_{k+1}} - f_{n_k}$ ($k \geq 1$) là *hội tụ theo trung bình cấp* $p$, thì nó sẽ có một tổng $g \in \mathcal{F}_\mathbf{F}^p$, và $f = g + f_{n_1}$ sẽ là giới hạn của dãy $(f_{n_k})$ trong $\mathcal{F}_\mathbf{F}^p$; khi đó $f$ sẽ là một điểm tụ của dãy $(f_n)$; vì dãy này là một dãy Cauchy, nó sẽ có $f$ làm giới hạn, và Mệnh đề 5 sẽ được chứng minh (GT, II, §3, No. 2, Hệ quả 2 của Mệnh đề 5).

Mệnh đề 5 do đó là một hệ quả của mệnh đề sau:

#### Mệnh đề 6 {#int-iv-s3-prop-6 .statement}

*Cho $(f_n)$ là một dãy các hàm trong $\mathcal{F}_\mathbf{F}^p$ sao cho $\sum_{n=1}^\infty N_p(f_n) < +\infty$. Với các điều kiện này, chuỗi có số hạng tổng quát $f_n(x) \in \mathbf{F}$ là hội tụ tuyệt đối hầu khắp nơi trong $X$. Đặt $f(x) = \sum_{n=1}^\infty f_n(x)$ tại các điểm mà chuỗi hội tụ, và $f(x) = 0$ ở các điểm khác, hàm $f$ thuộc về $\mathcal{F}_\mathbf{F}^p$ và là tổng của chuỗi có số hạng tổng quát $f_n$ (đối với tôpô hội tụ theo trung bình cấp $p$); chính xác hơn, với mọi $n \geqslant 0$,

$$
N_p \left( f - \sum_{k=1}^n f_k \right) \leqslant \sum_{k=n+1}^\infty N_p(f_k).
$$

Xét hàm dương (hữu hạn hoặc không) $g(x) = \sum_{n=1}^\infty |f_n(x)|$. Theo định lý lồi đếm được (No. 2, Định lý 1),

$$
N_p(g) \leqslant \sum_{n=1}^\infty N_p(f_n) < +\infty;
$$

do đó $g$ hữu hạn hầu khắp nơi (§ 2, No. 3, Mệnh đề 7), điều đó có nghĩa là chuỗi có số hạng tổng quát $f_n(x)$ hội tụ tuyệt đối hầu khắp nơi. Vì $\mathbf{F}$ là đầy đủ, chuỗi này hội tụ hầu khắp nơi và, với mọi $x \in X$, $|f(x)| \leqslant \sum_{n=1}^\infty |f_n(x)| = g(x)$, do đó

$$
N_p(f) \leqslant N_p(g) \leqslant \sum_{n=1}^\infty N_p(f_n) < +\infty,
$$

điều này chứng minh rằng $f$ thuộc về $\mathcal{F}_\mathbf{F}^p$. Mặt khác, với mọi số nguyên $n$,

$$
|f(x) - \sum_{k=1}^n f_k(x)| \leqslant \sum_{k=n+1}^\infty |f_k(x)|
$$

gần khắp nơi, do đó $N_p \left( f - \sum_{k=1}^n f_k \right) \leqslant \sum_{k=n+1}^\infty N_p(f_k)$. Theo giả thiết, chuỗi có số hạng tổng quát $N_p(f_n)$ là hội tụ; do đó, với mọi $\varepsilon > 0$, tồn tại một số nguyên $n$ sao cho $\sum_{k=n+1}^{\infty} N_p(f_k) \leq \varepsilon$, và bất đẳng thức (8) chứng minh rằng $f$ là tổng của chuỗi có số hạng tổng quát $f_n$, đối với tôpô hội tụ theo trung bình cấp $p$.

Các Mệnh đề 5 và 6 do đó đã được chứng minh hoàn toàn.

### 4. Các hàm khả tích lũy thừa $p$

Không gian vectơ $\mathcal{H}(X; F)$ (mà ta sẽ ký hiệu đơn giản là $\mathcal{H}_F$ nếu không sợ nhầm lẫn), gồm các hàm liên tục từ $X$ vào $F$ với giá compact, hiển nhiên là một không gian con của mỗi không gian vectơ $\mathcal{F}_F^p$.

#### Định nghĩa 2 {#int-iv-s3-def-2 .statement}

*Cho một không gian compact địa phương* $X$, *một độ đo* $\mu$ *trên* $X$, *và một không gian Banach* $F$, *ta ký hiệu bởi* $\mathcal{L}_F^p(X, \mu)$ *(hoặc đơn giản là* $\mathcal{L}_F^p(\mu)$, *hoặc* $\mathcal{L}_F^p$) *bao đóng, trong không gian lồi địa phương* $\mathcal{F}_F^p(X, \mu)$, *của không gian vectơ* $\mathcal{H}(X; F)$ *của các ánh xạ liên tục của* $X$ *vào* $F$ *với giá compact.* *Ta ký hiệu bởi* $L_F^p(X, \mu)$ *(hoặc* $L_F^p(\mu)$, *hoặc* $L_F^p$) *không gian* Hausdorff *(chuẩn hóa)* *liên kết với* $\mathcal{L}_F^p(X, \mu)$. *Các hàm thuộc* $\mathcal{L}_F^p$ *được gọi là các hàm khả tích lũy thừa* $p$* (*).

Hiển nhiên $\mathcal{L}_F^p(X, |\mu|) = \mathcal{L}_F^p(X, \mu)$ và $L_F^p(X, |\mu|) = L_F^p(X, \mu)$.

Ta sẽ viết $\mathcal{L}^p$ và $L^p$ thay cho $\mathcal{L}_R^p$ và $L_R^p$ (hoặc cho $\mathcal{L}_C^p$ và $L_C^p$ khi điều này không gây nhầm lẫn). Nếu $F$ là một không gian Banach *phức*, $\mathcal{L}_F^p$ và $L_F^p$ được trang bị cấu trúc của một không gian vectơ tôpô trên trường $\mathbf{C}$ (No. 3, *Nhận xét*).

Hiển nhiên rằng mọi hàm trong $\mathcal{F}_F^p$ tương đương với một hàm trong $\mathcal{L}_F^p$ thì thuộc $\mathcal{L}_F^p$. Một hàm có giá trị trong $F$ và *được xác định hầu khắp nơi* trong $X$ lại được gọi là *khả tích lũy thừa $p$* nếu nó tương đương với một hàm trong $\mathcal{L}_F^p$; tương tự, một hàm có giá trị trong $\overline{\mathbf{R}}$, được xác định và hữu hạn hầu khắp nơi trong $X$, được gọi là *khả tích lũy thừa $p$* nếu nó tương đương với một hàm trong $\mathcal{L}^p$.

Các hàm trong $\mathcal{L}_F^p$ (tương ứng trong $\mathcal{L}^p$) do đó là các *hàm khả tích theo lũy thừa thứ $p$* *được xác định trên toàn bộ* $X$ (tương ứng được xác định và hữu hạn trên toàn bộ $X$). Trong tiết diện này và tiết diện tiếp theo, phần lớn các mệnh đề đã chứng minh đối với các hàm trong $\mathcal{L}_F^p$ (tương ứng $\mathcal{L}^p$) có thể ngay lập tức mở rộng cho các *hàm khả tích theo lũy thừa thứ $p$* không được xác định khắp nơi (tương ứng không được xác định và hữu hạn khắp nơi); thông thường chúng ta sẽ để cho độc giả nhiệm vụ phát biểu và chứng minh các kết quả này.

(*) Sự biện minh cho thuật ngữ này sẽ được đưa ra trong §4, No. 2.

#### Nhận xét 1 {#int-iv-s3-n4-rem-1 .statement}

Như đã được chỉ ra (§2, No. 5), các hàm khả tích theo lũy thừa $p$ với giá trị trong $\mathbf{F}$ nói chung không tạo thành một không gian vectơ.
2) Nói chung, không gian $\mathcal{F}_\mathbf{F}^p$ phân biệt với không gian con của nó $\mathcal{L}_\mathbf{F}^p$ (§4, Exer. 8).

Định nghĩa 2 ngay lập tức cho tiêu chuẩn sau:

#### Mệnh đề 7 {#int-iv-s3-prop-7 .statement}

Để một hàm $\mathbf{f}$ thuộc $\mathcal{L}_\mathbf{F}^p$, điều kiện cần và đủ là, với mọi $\varepsilon > 0$, tồn tại một hàm liên tục $g$ có giá compact sao cho $N_p(\mathbf{f} - g) \leq \varepsilon$.

Nói cách khác, các hàm trong $\mathcal{L}_\mathbf{F}^p$ là các giới hạn của các dãy hàm liên tục có giá compact, đối với tôpô hội tụ theo trung bình cấp $p$.

#### Mệnh đề 8 {#int-iv-s3-prop-8 .statement}

Cho $f$ là một hàm số (hữu hạn hoặc không) được xác định hầu khắp nơi; nếu, với mọi $\varepsilon > 0$, tồn tại hai hàm khả tích theo lũy thừa $p$ $g, h$ sao cho $g \leq f \leq h$ hầu khắp nơi và $N_p(h - g) \leq \varepsilon$, thì $f$ là khả tích theo lũy thừa $p$.

Thật vậy, $f$ là hữu hạn hầu khắp nơi và $N_p(f - g) \leq N_p(h - g) \leq \varepsilon$; Mệnh đề 7 do đó cho thấy rằng $f$ là khả tích theo lũy thừa $p$.

Vì, theo định nghĩa, $\mathcal{L}_\mathbf{F}^p$ là một không gian con đóng của $\mathcal{F}_\mathbf{F}^p$, và vì không gian sau là đầy đủ (No. 3, Mệnh đề 5), ta có kết quả sau (GT, II, §3, No. 4, Mệnh đề 8):

#### Định lý 2 {#int-iv-s3-thm-2 .statement}

Không gian $\mathcal{L}_\mathbf{F}^p$ là đầy đủ; không gian $L_\mathbf{F}^p$ là một không gian Banach.

Trong không gian $L_\mathbf{F}^p$, chuẩn $N_p(\tilde{\mathbf{f}})$ của một lớp lại được ký hiệu là $\| \tilde{\mathbf{f}} \|_p$.

Định lý 2 có thể được làm sắc hơn như sau:

#### Định lý 3 {#int-iv-s3-thm-3 .statement}

Cho $(\mathbf{f}_n)$ là một dãy Cauchy trong không gian $\mathcal{L}_\mathbf{F}^p$; tồn tại một dãy con $(\mathbf{f}_{n_k})$ của $(\mathbf{f}_n)$ có các tính chất sau:
1° chuỗi với số hạng tổng quát $N_p(\mathbf{f}_{n_{k+1}} - \mathbf{f}_{n_k})$ là hội tụ;
2° chuỗi với số hạng tổng quát $\mathbf{f}_{n_{k+1}}(x) - \mathbf{f}_{n_k}(x)$ là hội tụ tuyệt đối hầu khắp nơi;
3° nếu $\mathbf{f}$ là một hàm được xác định trên $X$ và bằng hầu khắp nơi với giới hạn của dãy $(\mathbf{f}_{n_k}(x))$, thì $\mathbf{f}$ thuộc $\mathcal{L}_\mathbf{F}^p$ và dãy $(\mathbf{f}_n)$ hội tụ theo trung bình cấp $p$ đến $\mathbf{f}$;
4° tồn tại một hàm nửa liên tục dưới $g \geq 0$ sao cho $N_p(g) < +\infty$ và sao cho, với mọi $k$, $|\mathbf{f}_{n_k}(x)| \leq g(x)$ với mọi $x \in X$.

Như trong chứng minh của Mệnh đề 5 của No. 3, chỉ cần định nghĩa dãy $(n_k)$ bằng quy nạp, sao cho $N_p(\mathbf{f}_{n_{k+1}} - \mathbf{f}_{n_k}) \leq 2^{-k}$; các phần 2° và 3° khi đó suy ra từ Mệnh đề 6 của No. 3 và sự kiện rằng $\mathcal{L}_\mathbf{F}^p$ là đóng trong $\mathcal{F}_\mathbf{F}^p$. Mặt khác, nếu $h(x)$ là tổng của chuỗi có số hạng tổng quát $|\mathbf{f}_{n_{k+1}}(x) - \mathbf{f}_{n_k}(x)|$, Định lý 1 của No. 2 cho thấy rằng $N_p(h) < +\infty$; do đó, theo định nghĩa của $|\mu|^*$, tồn tại một hàm nửa liên tục dưới $g \geq h + |\mathbf{f}_{n_1}|$ sao cho $N_p(g) < +\infty$, điều này hoàn tất chứng minh.

#### Hệ quả 1 {#int-iv-s3-thm-3-cor-1 .statement}

— *Nếu một dãy Cauchy* $(f_n)$ *trong không gian* $\mathcal{L}_F^p$ *là sao cho dãy* $(f_n(x))$ *hội tụ hầu khắp nơi đến* $f(x)$*, thì* $f$ *là khả tích theo lũy thừa p và dãy* $(f_n)$ *hội tụ theo trung bình cấp* $p$ *đến* $f$.

Thật vậy, tồn tại một dãy con $(f_{n_k})$ của $(f_n)$ sao cho $(f_{n_k}(x))$ hội tụ hầu khắp nơi đến $g(x)$, trong đó $g$ là một hàm trong $\mathcal{L}_F^p$ sao cho $(f_n)$ hội tụ theo trung bình cấp $p$ đến $g$. Các giả thiết do đó kéo theo rằng $f(x) = g(x)$ hầu khắp nơi, do đó có hệ quả.

#### Hệ quả 2 {#int-iv-s3-thm-3-cor-2 .statement}

— *Cho* $\mathcal{E}$ *là một tập con trù mật của* $\mathcal{L}_F^p$. *Đối với mọi hàm* $f \in \mathcal{L}_F^p$, *tồn tại một dãy* $(g_n)$ *gồm các hàm trong* $\mathcal{E}$ *có các tính chất sau*:

1° *dãy* $(g_n)$ *hội tụ theo trung bình cấp* $p$ *đến* $f$;
2° *đối với hầu hết mọi* $x \in X$, *dãy* $(g_n(x))$ *hội tụ đến* $f(x)$.

Thật vậy, vì không gian $\mathcal{L}_F^p$ là mêtric hóa được, tồn tại một dãy Cauchy $(f_n)$ trong $\mathcal{L}_F^p$ gồm các hàm trong $\mathcal{E}$ và hội tụ theo trung bình cấp $p$ đến $f$ (GT, IX, §2, No. 6, Mệnh đề 8); chỉ cần áp dụng Định lý 3 cho dãy này.

Hệ quả 2 áp dụng đặc biệt cho trường hợp $\mathcal{E}$ được lấy là không gian $\mathcal{K}_F$ gồm các *hàm liên tục có giá compact*.

#### Nhận xét 2 {#int-iv-s3-n4-rem-2 .statement}

Một dãy Cauchy $(f_n)$ trong $\mathcal{L}_F^p$ có thể sao cho dãy $(f_n(x))$ không hội tụ *tại bất kỳ điểm nào của* $X$ (Bài tập 1).

#### Nhận xét 3 {#int-iv-s3-n4-rem-3 .statement}

Nếu $f$ thuộc về $\mathcal{L}_F^p$, không phải lúc nào cũng có thể tìm được một dãy $(f_n)$ gồm các hàm liên tục có giá compact sao cho dãy $(f_n(x))$ hội tụ *mọi nơi* trong $X$ đến một hàm bằng $f(x)$ hầu khắp nơi (§4, Bài tập 4 c)).

### 5. Các tính chất của các hàm khả tích theo lũy thừa $p$

#### Định lý 4 {#int-iv-s3-thm-4 .statement}

— *Cho* $F$ *và* $G$ *là hai không gian Banach,* $u$ *là một ánh xạ tuyến tính liên tục từ* $F$ *vào* $G$. *Đối với mọi hàm* $f \in \mathcal{L}_F^p$, *hàm hợp thành* $u \circ f$ *thuộc* $\mathcal{L}_G^p$.

Cho $f \in \mathcal{L}_F^p$; với mọi $\varepsilon > 0$, tồn tại một hàm $g \in \mathcal{K}_F$ sao cho $N_p(f - g) \leq \varepsilon$; vì $|u \circ f - u \circ g| \leq \|u\| \cdot |f - g|$, ta có

$$
N_p(u \circ f - u \circ g) \leq \|u\| \cdot N_p(f - g) \leq \varepsilon \|u\|,
$$

và vì $u \circ g$ liên tục với giá compact, định lý được chứng minh.

#### Hệ quả 1 {#int-iv-s3-thm-4-cor-1 .statement}

— *Cho* $a'$ *là một dạng tuyến tính liên tục trên* $F$; *nếu* $f \in \mathcal{L}_F^p$, *hàm số* $x \mapsto \langle f(x), a' \rangle$ **(ký hiệu là $\langle f, a' \rangle$)* thuộc* $\mathcal{L}^p$.

#### Hệ quả 2 {#int-iv-s3-thm-4-cor-2 .statement}

— Cho n điểm $a_k$ của F ($1 \leq k \leq n$), và n hàm số $f_k$ ($1 \leq k \leq n$) thuộc $\mathcal{L}^p$, hàm $f = \sum_{k=1}^n a_k f_k$ thuộc $\mathcal{L}_F^p$.

Điều này suy ra từ sự kiện rằng ánh xạ $t \mapsto a t$ từ $\mathbf{R}$ vào F là liên tục.

#### Mệnh đề 9 {#int-iv-s3-prop-9 .statement}

— Cho F là một không gian vectơ n-chiều trên $\mathbf{R}$, và cho $(e_k)_{1 \leq k \leq n}$ là một cơ sở của F. Để một hàm $f = \sum_{k=1}^n e_k f_k$ thuộc $\mathcal{L}_F^p$, điều kiện cần và đủ là mỗi hàm số $f_k$ thuộc $\mathcal{L}^p$.

Điều này suy ra ngay từ Hệ quả 1 và 2 của Định lý 4.

#### Mệnh đề 10 {#int-iv-s3-prop-10 .statement}

— Trong không gian $\mathcal{L}_F^p$, không gian con tuyến tính tạo bởi các tổ hợp tuyến tính (hữu hạn) $\sum_k a_k f_k$, trong đó $a_k \in F$ và các $f_k$ là các hàm số liên tục có giá compact, là trù mật (đối với tôpô của sự hội tụ trung bình cấp $p$).

Tập hợp $\mathcal{K}_F$ các ánh xạ liên tục từ X vào F có giá compact, theo định nghĩa là trù mật trong $\mathcal{L}_F^p$. Mặt khác, mọi hàm $g \in \mathcal{K}_F$ có thể được xấp xỉ đều bởi các hàm có dạng $\sum_k a_k f_k$, trong đó các $f_k$ là các hàm liên tục có giá được chứa trong một lân cận compact cố định của giá của $g$ (Ch. III, §1, No. 2, Bổ đề 2); do đó (No. 3, Mệnh đề 4) $g$ thuộc bao đóng trong $\mathcal{L}_F^p$ của tập hợp các $\sum_k a_k f_k$, do đó có mệnh đề.

#### Mệnh đề 11 {#int-iv-s3-prop-11 .statement}

— Nếu một hàm $f$ thuộc $\mathcal{L}_F^p$, thì hàm $|f|$ thuộc $\mathcal{L}^p$, và ánh xạ $f \mapsto |f|$ từ $\mathcal{L}_F^p$ vào $\mathcal{L}^p$ là liên tục đều (đối với tôpô của sự hội tụ trung bình cấp $p$).

Với mọi $\varepsilon > 0$ tồn tại một hàm liên tục $g$ có giá compact, sao cho $N_p(f - g) \leq \varepsilon$; vì $||f| - |g|| \leq |f - g|$, ta có $N_p(|f| - |g|) \leq \varepsilon$, điều này chứng minh rằng $|f| \in \mathcal{L}^p$. Mặt khác, nếu $f_1, f_2$ là hai hàm trong $\mathcal{L}_F^p$ thì $N_p(|f_1| - |f_2|) \leq N_p(f_1 - f_2)$, điều này chỉ ra rằng $f \mapsto |f|$ là một ánh xạ liên tục đều.

#### Mệnh đề 12 {#int-iv-s3-prop-12 .statement}

— Để một hàm số $f$ thuộc $\mathcal{L}^p$, điều kiện cần và đủ là mỗi một trong các hàm $f^+$ và $f^-$ thuộc $\mathcal{L}^p$.

Điều kiện là đủ vì $f = f^+ - f^-$; nó là cần thiết, bởi vì nếu $f \in \mathcal{L}^p$ thì $|f| \in \mathcal{L}^p$ (Mệnh đề 11).

#### Hệ quả {#int-iv-s3-n5-cor-1 .statement}

— Bao trên (tương ứng bao dưới) của một họ hữu hạn các hàm trong $\mathcal{L}^p$ thuộc $\mathcal{L}^p$.

### 6. Các tập hợp có hướng trong $L^p$ và các dãy tăng trong $\mathcal{L}^p$

Ta đã định nghĩa (§ 2, No. 6) một quan hệ thứ tự $\tilde{f} \leq \tilde{g}$ trong tập hợp $\widetilde{\mathcal{F}}$ gồm các lớp tương đương của các hàm số được xác định và hữu hạn hầu khắp nơi trong $X$; được trang bị quan hệ thứ tự này và cấu trúc không gian vectơ của nó, $\widetilde{\mathcal{F}}$ là một *không gian Riesz*. Hệ quả của Mệnh đề 12 của No. 5 chỉ ra rằng nếu $\tilde{f}$ và $\tilde{g}$ là hai phần tử của không gian con $L^p$ của $\widetilde{\mathcal{F}}$, thì cận trên đúng $\sup(\tilde{f}, \tilde{g})$ của $\tilde{f}$ và $\tilde{g}$ trong $\widetilde{\mathcal{F}}$ (là lớp của mỗi hàm $\sup(f, g)$, trong đó $f \in \tilde{f}$ và $g \in \tilde{g}$) thuộc $L^p$; điều này đặc biệt chứng minh rằng $L^p$, được trang bị quan hệ thứ tự cảm sinh bởi quan hệ của $\widetilde{\mathcal{F}}$, là một *không gian Riesz*.

#### Mệnh đề 13 {#int-iv-s3-prop-13 .statement}

*Trong không gian Riesz $L^p$, được trang bị tôpô xác định bởi chuẩn $\| \tilde{f} \|_p$, ánh xạ $\tilde{f} \mapsto | \tilde{f} |$ là liên tục đều, và tập hợp các phần tử $\tilde{f} \geq 0$ là đóng.*

Phần thứ nhất của mệnh đề suy ra ngay từ Mệnh đề 11 của No. 5; vì tập hợp các $\tilde{f} \geq 0$ cũng là tập hợp các $\tilde{f}$ sao cho $| \tilde{f} | = f$, nó là đóng, bởi vì $\tilde{f} \mapsto | \tilde{f} |$ là một ánh xạ liên tục và $L^p$ là Hausdorff.

Do đó ta thấy rằng tôpô trên $L^p$ xác định bởi chuẩn $\| \tilde{f} \|_p$ là *tương thích* với cấu trúc không gian vectơ có thứ tự của $L^p$ (TVS, II, § 2, No. 7).

#### Mệnh đề 14 {#int-iv-s3-prop-14 .statement}

*Cho $H$ là một tập con của không gian Riesz $L^p$, gồm các lớp $\geq 0$ và có hướng đối với quan hệ $\leq$. Để $H$ có một cận trên đúng trong $L^p$, điều kiện cần và đủ là*

$$
\sup_{\tilde{f} \in H} \| \tilde{f} \|_p < +\infty.
$$

*Supremum của $H$ trong $L^p$ khi đó là giới hạn* (trong không gian Banach $L^p$) *của lọc tiết diện của $H$*.

Điều kiện này rõ ràng là cần, vì $\tilde{f} \mapsto \| \tilde{f} \|_p$ là một hàm tăng trên tập hợp các phần tử $\geq 0$ của $L^p$. Để thấy rằng nó đủ, trước hết ta nhận thấy rằng nó kéo theo ảnh của $H$ qua ánh xạ $\tilde{f} \mapsto \| \tilde{f} \|_p$ có một giới hạn trong $\mathbf{R}$, theo định lý giới hạn đơn điệu; do đó ảnh của lọc tiết diện $\mathfrak{F}$ của $H$ qua ánh xạ này là một cơ sở của một lọc Cauchy trên $\mathbf{R}$. Chứng minh sẽ hoàn tất nếu ta chỉ ra rằng bản thân $\mathfrak{F}$ là một *cơ sở của một lọc Cauchy* trên $L^p$; vì khi đó $\mathfrak{F}$ sẽ hội tụ trong $L^p$, do $L^p$ là đầy đủ (No. 4, Th. 2), và mệnh đề sẽ suy ra từ TVS, II, § 2, No. 7, Mệnh đề 18.

Để thấy rằng $\mathfrak{F}$ là một cơ sở của một lọc Cauchy, ta sẽ sử dụng bổ đề sau:

#### Bổ đề {#int-iv-s3-n6-lem-1 .statement}

Nếu $f$ và $g$ là hai hàm trong $\mathcal{L}^p$ sao cho $0 \leq f \leq g$, thì

$$
(N_p(g - f))^p \leq (N_p(g))^p - (N_p(f))^p .
$$

Khi $f$ và $g$ là liên tục với giá compact, quan hệ (9) có thể được viết

$$
\int (g - f)^p d|\mu| \leq \int g^p d|\mu| - \int f^p d|\mu|
$$

và khi đó là một hệ quả của bất đẳng thức sơ cấp $(g - f)^p \leq g^p - f^p$ (No. 1, công thức (2)). Để chuyển từ điều này sang trường hợp tổng quát, chỉ cần nhận xét rằng hai vế của (9) là các hàm liên tục trên $\mathcal{L}^p \times \mathcal{L}^p$, và mọi hàm $f \geq 0$ trong $\mathcal{L}^p$ là giới hạn (đối với sự hội tụ theo trung bình cấp $p$) của một dãy các hàm liên tục $\geq 0$ có giá compact, do tính liên tục của ánh xạ $g \mapsto |g|$ trên $\mathcal{L}^p$ (Mệnh đề 11).

Sau khi bổ đề đã được thiết lập, với mọi $\varepsilon > 0$ tồn tại theo giả thiết một $\tilde{f} \in \mathrm{H}$ sao cho, với mọi $\tilde{g} \geq \tilde{f}$ thuộc $\mathrm{H}$, ta có $(\|\tilde{g}\|_p)^p - (\|\tilde{f}\|_p)^p \leq \varepsilon$; từ đó suy ra rằng $(\|\tilde{g} - \tilde{f}\|_p)^p \leq \varepsilon$; do đó, nếu $\tilde{g}_1$ và $\tilde{g}_2$ là hai phần tử trong $\mathrm{H}$ mà $\geq \tilde{f}$, thì $\|\tilde{g}_1 - \tilde{g}_2\|_p \leq 2\varepsilon^{1/p}$, điều này chứng minh rằng $\mathfrak{F}$ là một cơ sở lọc Cauchy trên $L^p$ và hoàn tất chứng minh của Mệnh đề 14.

#### Hệ quả 1 {#int-iv-s3-prop-14-cor-1 .statement}

Nếu $\tilde{g}$ là supremum của $\mathrm{H}$ trong $L^p$, thì

$$
\|\tilde{g}\|_p = \lim_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p = \sup_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p .
$$

Điều này suy ra từ tính liên tục của chuẩn $\|\tilde{f}\|_p$ trong $L^p$, và định lý giới hạn đơn điệu.

#### Hệ quả 2 {#int-iv-s3-prop-14-cor-2 .statement}

Không gian Riesz $L^p$ là có thứ tự dàn đầy đủ.

Mọi tập có hướng $\mathrm{H}$ trong $L^p$ (đối với quan hệ $\leq$), gồm các lớp $\geq 0$ và bị chặn trên trong $L^p$, đều có một cận trên nhỏ nhất: thật vậy, nếu $\tilde{h}$ là một cận trên của $\mathrm{H}$ trong $L^p$, thì $\|\tilde{f}\|_p \leq \|\tilde{h}\|_p$ với mọi $\tilde{f} \in \mathrm{H}$, và Mệnh đề 14 áp dụng được. Điều này chứng minh hệ quả (Ch. II, §1, No. 3, Mệnh đề 1).

Các kết luận của Mệnh đề 14 không còn đúng khi chúng được phát biểu cho các hàm trong $\mathcal{L}^p$ thay vì cho các lớp của chúng. Nói chính xác hơn, nếu $M$ là một tập con của $\mathcal{L}^p$, gồm các hàm $\geq 0$, có hướng đối với quan hệ $\leq$, và sao cho $\sup_{f \in M} N_p(f) < +\infty$, *lớp của bao trên* $g$ của $M$ *không nhất thiết đồng nhất với cận trên nhỏ nhất trong* $L^p$ *của các lớp của các hàm* f \in M ; đặc biệt, g không nhất thiết khả tích theo lũy thừa p, và ngay cả khi $g \in \mathcal{L}^p$, $N_p(g)$ có thể phân biệt với $\sup_{f \in M} N_p(f)$ (xem §1, No. 3, Nhận xét 1 sau Định lý 3).

Tuy nhiên, ta có định lý sau:

#### Định lý 5 {#int-iv-s3-thm-5 .statement}

*Cho $(f_n)$ là một dãy tăng các hàm $\geqslant 0$ trong $\mathcal{L}^p$. Để bao trên $f$ của dãy này khả tích theo lũy thừa p, điều kiện cần và đủ là $\sup_n N_p(f_n) < +\infty$. Khi đó dãy $(f_n)$ hội tụ theo trung bình cấp $p$ đến $f$, và*

$$
N_p(f) = \sup_n N_p(f_n) = \lim_{n \to \infty} N_p(f_n).
$$

Điều kiện là hiển nhiên cần thiết, nên ta chỉ cần chứng minh rằng nó đủ. Bây giờ, nếu điều kiện được thỏa mãn thì Mệnh đề 14 chỉ ra rằng dãy $(\tilde{f}_n)$ là một dãy Cauchy trong $L^p$, do đó dãy $(f_n)$ là một dãy Cauchy trong $\mathcal{L}^p$; vì $f_n(x)$ tiến tới $f(x)$ với mọi $x \in X$, $f$ khả tích theo lũy thừa p và là giới hạn của dãy $(f_n)$ đối với tôpô hội tụ theo trung bình cấp $p$ (No. 4, Hệ quả 1 của Định lý 3). Do đó $N_p(f_n)$ tiến tới $N_p(f)$ vì $N_p$ là một hàm liên tục trên $\mathcal{L}^p$.

#### Hệ quả 1 {#int-iv-s3-thm-5-cor-1 .statement}

*Cho $(f_n)$ là một dãy giảm các hàm $\geqslant 0$ trong $\mathcal{L}^p$; khi đó, bao dưới $f$ của dãy thuộc về $\mathcal{L}^p$, dãy $(f_n)$ hội tụ theo trung bình cấp $p$ đến $f$, và*

$$
N_p(f) = \lim_{n \to \infty} N_p(f_n) = \inf_n N_p(f_n).
$$

Hai khẳng định đầu tiên suy ra từ Định lý 5 áp dụng cho dãy $g_n = f_1 - f_n$, là dãy tăng và bị chặn trên; phần còn lại khi đó là hiển nhiên.

#### Hệ quả 2 {#int-iv-s3-thm-5-cor-2 .statement}

*Cho $(f_n)$ là một dãy các hàm trong $\mathcal{L}^p$. Để bao trên $f$ của dãy $(f_n)$ là khả tích theo lũy thừa p, điều kiện cần và đủ là tồn tại một hàm $g \geqslant 0$ sao cho $\int^* g^p d|\mu| < +\infty$ và $f_n \leqslant g$ với mọi $n$.

Điều kiện này hiển nhiên là cần, bằng cách lấy $g = f^+$. Ngược lại, giả sử điều kiện đó được thỏa mãn, và đặt $g_n = \sup_{k \leqslant n} f_k$; dãy $(g_n)$ là tăng và gồm các hàm khả tích theo lũy thừa p (No. 5, Hệ quả của Mệnh đề 12). Dãy tăng các hàm dương $h_n = g_n + g_1^-$ thỏa mãn các điều kiện của Định lý 5, vì $N_p(h_n) \leqslant N_p(g + g_1^-) < +\infty$; bao trên của nó $\sup_n h_n$ do đó là khả tích theo lũy thừa p, và điều tương tự cũng đúng đối với $f = \sup_n h_n - g_1^-$.

#### Hệ quả 3 {#int-iv-s3-thm-5-cor-3 .statement}

— Cho $A$ là một tập hợp đếm được, $\mathfrak{F}$ là một lọc trên $A$ có một cơ sở đếm được, $(f_\alpha)_{\alpha \in A}$ là một họ các hàm $\geq 0$ trong $\mathcal{L}^p$. Giả sử rằng tồn tại một hàm $g \geq 0$ sao cho $N_p(g) < +\infty$ và $f_\alpha \leq g$ với mọi $\alpha \in A$; khi đó hàm $\limsup_{\mathfrak{F}} f_\alpha$ là khả tích theo lũy thừa p và

$$
\limsup_{\mathfrak{F}} N_p(f_\alpha) \leq N_p(\limsup_{\mathfrak{F}} f_\alpha).
$$

Cho $(A_n)$ là một cơ sở giảm của $\mathfrak{F}$ và đặt $g_n = \sup_{\alpha \in A_n} f_\alpha$; vì $A_n$ là một tập hợp đếm được, suy ra từ Hệ quả 2 rằng $g_n$ là khả tích theo lũy thừa p; mặt khác, $N_p(g_n) \geq \sup_{\alpha \in A_n} N_p(f_\alpha)$. Như vậy, $\limsup_{\mathfrak{F}} f_\alpha$ là bao dưới của dãy giảm $(g_n)$; do đó $\limsup_{\mathfrak{F}} f_\alpha$ là khả tích theo lũy thừa p theo Hệ quả 1, và

$$
N_p(\limsup_{\mathfrak{F}} f_\alpha) = N_p \left( \inf_n g_n \right) = \lim_{n \to \infty} N_p(g_n)
$$
$$
\geq \lim_{n \to \infty} \left( \sup_{\alpha \in A_n} N_p(f_\alpha) \right) = \limsup_{\mathfrak{F}} N_p(f_\alpha).
$$

### 7. Định lý của Lebesgue

#### Định lý 6 (Lebesgue) {#int-iv-s3-thm-6 .statement}

— Cho $F$ là một không gian Banach, $(f_n)$ là một dãy các hàm trong $\mathcal{L}_F^p$ sao cho: $1^\circ$ dãy $(f_n(x))$ hội tụ hầu khắp nơi đến một giới hạn $f(x) \in F$; $2^\circ$ tồn tại một hàm số $g \geq 0$ sao cho $\int^* g^p d|\mu| < +\infty$ và $|f_n(x)| \leq g(x)$ hầu khắp nơi trong $X$, với mọi số nguyên $n$. Khi đó, hàm $f$ (được xác định hầu khắp nơi) là khả tích theo lũy thừa p, và dãy $(f_n)$ hội tụ theo trung bình cấp $p$ đến $f$.

Xét dãy kép các hàm số $g_{mn} = |f_m - f_n|$, thuộc $\mathcal{L}^p$ (No. 5, Prop. 11); theo giả thiết, $\lim_{m \to \infty, n \to \infty} g_{mn}(x) = 0$ hầu khắp nơi, và mặt khác $|g_{mn}(x)| \leq 2g(x)$ hầu khắp nơi; áp dụng Hệ quả 3 của Định lý 5 của No. 6 cho dãy kép này,

$$
\limsup_{m \to \infty, n \to \infty} N_p(f_m - f_n) \leq N_p(0) = 0,
$$

và vì $N_p(f_m - f_n) \geq 0$ điều này suy ra $\lim_{m \to \infty, n \to \infty} N_p(f_m - f_n) = 0$; nói cách khác, dãy $(f_n)$ là một dãy Cauchy trong $\mathcal{L}_F^p$. Định lý do đó suy ra từ Hệ quả 1 của Định lý 3 của No. 4.

#### Hệ quả {#int-iv-s3-n7-cor-1 .statement}

— Cho $A$ là một tập hợp các chỉ số, được lọc bởi một bộ lọc $\mathfrak{F}$ có một cơ sở đếm được. Nếu $(f_\alpha)_{\alpha \in A}$ là một họ các hàm trong $\mathcal{L}_F^p$ mà, đối với bộ lọc $\mathfrak{F}$, hội tụ từng điểm hầu khắp nơi đến một hàm $f$, và nếu ngoài ra tồn tại một hàm số $g \geq 0$ sao cho $\int^* g^p d|\mu| < +\infty$ và $|f_\alpha(x)| \leq g(x)$ hầu khắp nơi trong $X$ với mỗi $\alpha \in A$, thì hàm $f$ là khả tích lũy thừa bậc $p$ và $f_\alpha$ hội tụ theo trung bình cấp $p$ đến $f$ đối với bộ lọc $\mathfrak{F}$.

Thật vậy, cho $(A_n)$ là một cơ sở đếm được giảm của $\mathfrak{F}$, và cho $\alpha_n$ là một phần tử bất kỳ của $A_n$; dãy $(f_{\alpha_n})$ hội tụ từng điểm đến $f$ hầu khắp nơi trong $X$, do đó Định lý 6 cho thấy rằng $f$ là khả tích lũy thừa bậc $p$ và rằng $\lim_{n \to \infty} N_p(f - f_{\alpha_n}) = 0$. Vì $\mathfrak{F}$ là bộ lọc giao của các bộ lọc sơ cấp liên kết với tất cả các dãy như vậy $(\alpha_n)$ (GT, I, §6, No. 8, Prop. 11), $\lim_{\mathfrak{F}} N_p(f - f_\alpha)$ tồn tại và bằng giới hạn chung 0 của tất cả các dãy $(N_p(f - f_{\alpha_n}))$.

#### Nhận xét 1 {#int-iv-s3-n7-rem-1 .statement}

Định lý 6 không còn đúng nếu giả thiết $|f_n| \leq g$ (với $N_p(g) < +\infty$) được thay bằng giả thiết yếu hơn $\sup_n N_p(f_n) < +\infty$. Chẳng hạn, giả sử $\mu$ là độ đo Lebesgue trên $\mathbf{R}$; định nghĩa các hàm liên tục $f_n$ theo cách sau: $f_n(x) = 0$ với $x \leq 0$ và với $x \geq \frac{2}{n}$, $f_n(\frac{1}{n}) = n$, $f_n$ là tuyến tính trên các khoảng $[0, \frac{1}{n}]$ và $[\frac{1}{n}, \frac{2}{n}]$. Khi đó $\lim_{n \to \infty} f_n(x) = 0$ với mọi $x \in \mathbf{R}$, nhưng $N_1(f_n) = 1$ với mọi $n$ (xem §5, Bài tập 12).

#### Nhận xét 2 {#int-iv-s3-n7-rem-2 .statement}

Hệ quả của Định lý 6 không còn đúng nếu không giả sử rằng bộ lọc $\mathfrak{F}$ có một cơ sở đếm được (xem §1, No. 3, Nhận xét 1 sau Hệ quả của Định lý 3).

### 8. Các quan hệ giữa các không gian $\mathcal{L}_F^p$ ($1 \leq p < +\infty$)

Với mọi số thực $\alpha > 0$, ánh xạ $z \mapsto |z|^{\alpha-1} \cdot z$ được xác định và liên tục trên phần bù của 0 trong $F$; hơn nữa, vì $||z|^{\alpha-1} \cdot z| = |z|^{\alpha}$, hàm này tiến tới 0 cùng với $z$ và do đó có thể được mở rộng bằng tính liên tục tới điểm 0 bằng cách gán cho nó giá trị 0 tại điểm này, ngay cả khi $\alpha < 1$.

#### Định lý 7 {#int-iv-s3-thm-7 .statement}

— Cho $p$ và $q$ là hai số thực sao cho $1 \leq p < +\infty$, $1 \leq q < +\infty$. Nếu một hàm $f$ thuộc $\mathcal{L}_F^p$ thì hàm $|f|^{(p/q)-1} \cdot f$ thuộc $\mathcal{L}_F^q$, và đảo lại.

Theo giả thiết, tồn tại một dãy $(f_n)$ các hàm liên tục có giá đỡ compact sao cho $\sum_{n=1}^\infty N_p(f_n) < +\infty$ và $f(x) = \sum_{n=1}^\infty f_n(x)$ hầu khắp nơi (No. 4, Th. 3). Đặt

$$
g_n = |f_1 + f_2 + \cdots + f_n|^{(p/q)-1} \cdot (f_1 + f_2 + \cdots + f_n);
$$

hàm $g_n$ là liên tục có giá đỡ compact; mặt khác,

$$
|g_n|^q = |f_1 + f_2 + \cdots + f_n|^p \leq \left( \sum_{n=1}^\infty |f_n| \right)^p = h^q,
$$

trong đó hàm số $h \geqslant 0$ (hữu hạn hoặc không) thỏa mãn bất đẳng thức

$$
(N_q(h))^q = \left( N_p \left( \sum_{n=1}^{\infty} |f_n| \right) \right)^p \leqslant \left( \sum_{n=1}^{\infty} N_p(f_n) \right)^p < +\infty
$$

theo định lý lồi đếm được. Hơn nữa, $g_n(x)$ tiến tới hầu khắp nơi tới $g(x) = |f(x)|^{(p/q)-1} \cdot f(x)$, do đó định lý Lebesgue chỉ ra rằng $g \in \mathcal{L}_F^q$. Điều đảo lại là ngay lập tức, vì $f = |g|^{(q/p)-1} \cdot g$.

Có thể chứng minh được rằng ánh xạ $f \mapsto |f|^{\frac{p}{q}-1} \cdot f$ là một đồng phôi từ $\mathcal{L}_F^p$ lên $\mathcal{L}_F^q$ (§ 6, Exer. 10).

#### Hệ quả 1 {#int-iv-s3-thm-7-cor-1 .statement}

— *Để một hàm $f$ thuộc $\mathcal{L}_F^p$, điều kiện cần và đủ là hàm $|f|^{p-1} \cdot f$ thuộc $\mathcal{L}_F^1$.*

#### Hệ quả 2 {#int-iv-s3-thm-7-cor-2 .statement}

— *Để một hàm số dương $f$ thuộc $\mathcal{L}^p$, điều kiện cần và đủ là $f^p$ thuộc $\mathcal{L}^1$.*

Chú ý rằng nếu $f$ là một hàm số có dấu tùy ý, sao cho $|f|^p$ thuộc $\mathcal{L}^1$, thì $f$ không nhất thiết thuộc $\mathcal{L}^p$ (xem § 4, Exer. 8).

### Bài tập {#int-iv-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
