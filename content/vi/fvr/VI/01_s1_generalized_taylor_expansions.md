---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 1
section_title: GENERALIZED TAYLOR EXPANSIONS
lang: vi
source: fvr-i-vii
pdf_pages: 0284-0298, 0306-0307
extraction: ocr
subsections:
    - "no": 1
      title: COMPOSITION OPERATORS ON AN ALGEBRA OF POLYNOMIALS
      page: 0
      pdf_page: 284
    - "no": 2
      title: APPELL POLYNOMIALS ATTACHED TO A COMPOSITION OPERATOR
      page: 0
      pdf_page: 287
    - "no": 3
      title: GENERATING SERIES FOR THE APPELL POLYNOMIALS
      page: 0
      pdf_page: 289
    - "no": 4
      title: BERNOULLI POLYNOMIALS
      page: 0
      pdf_page: 290
    - "no": 5
      title: COMPOSITION OPERATORS ON FUNCTIONS OF A REAL VARIABLE
      page: 0
      pdf_page: 292
    - "no": 6
      title: INDICATRIX OF A COMPOSITION OPERATOR
      page: 0
      pdf_page: 293
    - "no": 7
      title: THE EULER-MACLAURIN SUMMATION FORMULA
      page: 0
      pdf_page: 297
statements: 20
exercises: 3
content_sha256: 8a2a439e6a11a7a14e383f452713ea08c693091c88c285cf3a39bf7c3a371e31
translated_from: content/en/fvr/VI/01_s1_generalized_taylor_expansions.md
source_content_sha256: 0001fab43420fc721b2091717a772409bf8d8ed8a052f67cffccc1674b37f714
translation_model: gpt-5.4
translation_run: translate-vi-0556b9c2
glossary_version: 34
glossary_terms_sha256: 9815db109c3a798cf5dde634676f5c75b3c9dfdfa7ccf46626b618b12907bea3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. KHAI TRIỂN TAYLOR TỔNG QUÁT

### 1. CÁC TOÁN TỬ HỢP THÀNH TRÊN MỘT ĐẠI SỐ ĐA THỨC

Cho K là một trường giao hoán có đặc số 0, và K[X] là đại số các đa thức theo một ẩn trên K (Đại số, IV. 1); trong suốt tiết này, bởi một toán tử trên K[X] ta sẽ hiểu là một ánh xạ tuyến tính U của không gian vectơ K[X] (trên K) vào chính nó; vì các đơn thức $X^n \ (n \geqslant 0)$ tạo thành một cơ sở của không gian này, U được xác định bởi các đa thức $U(X^n)$; cụ thể, nếu $f(X) = \sum_{k=0}^\infty \lambda_k X^k$ với $\lambda_k \in K$, thì
$$
U(f) = \sum_{k=0}^\infty \lambda_k U(X^k).
$$
Nếu G là một đại số giao hoán trên K, có phần tử đơn vị, thì G-môđun G[X] thu được bằng cách mở rộng trường vô hướng K của không gian vectơ K[X] thành G; mọi toán tử U trên K[X] mở rộng theo một cách duy nhất thành một ánh xạ tuyến tính từ G-môđun G[X] vào chính nó, mà ta lại ký hiệu là U (Đại số, II, p. 278); với mỗi phần tử $g(X) = \sum_{k=0}^\infty \gamma_k X^k$, trong đó $\gamma_k \in G$, ta có $U(g) = \sum_{k=0}^\infty \gamma_k U(X^k)$.

Xét riêng trường hợp G = K[Y]; khi đó G[X] là vành K[X,Y] các đa thức theo hai ẩn trên K; để tránh nhầm lẫn, ta ký hiệu phần mở rộng của U lên G[X] bởi $U_X$. Do đó, với mọi đa thức $g(X, Y) = \sum_{k=0}^\infty \gamma_k(Y) X^k$ trong đó $\gamma_k(Y) \in K[Y]$ ta có $U_X(g) = \sum_{k=0}^\infty \gamma_k(Y) U(X^k)$. Vì $U_X$ là tuyến tính, ta thấy rằng nếu viết $g(X, Y) = \sum_{h=0}^\infty \beta_h(X) Y^h$ thì ta cũng có $U_X(g) = \sum_{h=0}^\infty U(\beta_h) Y^h$.

Dưới đẳng cấu chính tắc từ K[X] lên K[Y] gắn Y với X, toán tử U chuyển thành một toán tử trên K[Y], mà để tránh nhầm lẫn, ta sẽ ký hiệu là $U_Y$, sao cho $U_Y(f(Y))$ là đa thức thu được bằng cách thay thế X bởi Y trong đa thức $U(f(X)) = U_X(f(X))$. Đến lượt mình, toán tử $U_Y$ này có thể được mở rộng thành một toán tử (vẫn ký hiệu là $U_Y$) trên K[X,Y]: nếu $g(X, Y) = \sum_{h=0}^\infty \beta_h(X) Y^h$ thì
$$
U_Y(g(X, Y)) = \sum_{h=0}^\infty \beta_h(X) U_Y(Y^h).
$$

Như một ví dụ về các sự mở rộng này, ta dẫn ra toán tử đạo hàm D trên K[X] (Alg., IV. 6), cho các toán tử đạo hàm riêng D_X và D_Y trên K[X,Y].

Với mọi đa thức $f \in K[X]$ ta ký hiệu bởi $T_Y(f)$ đa thức $f(X + Y)$ trong K[X,Y]; ánh xạ $T_Y$ là một ánh xạ K-tuyến tính từ K[X] vào K[X,Y], gọi là một toán tử tịnh tiến.

#### Định nghĩa 1 {#fvr-vi-s1-def-1 .statement}

*Ta nói rằng một toán tử U trên K[X] là một toán tử hợp thành nếu nó giao hoán với toán tử tịnh tiến, nghĩa là, nếu $U_X T_Y = T_Y U$.*

Nói cách khác, nếu $f$ là một đa thức tùy ý trong K[X], và nếu $g = U(f)$, thì phải có $g(X + Y) = U_X(f(X + Y))$.

Ngay lập tức suy ra từ định nghĩa này rằng với mọi đa thức $f(X) \in K[X]$ ta có, theo ký hiệu trên,

$$
U_X(f(X + Y)) = U_Y(f(X + Y)).
$$

(1)

#### Ví dụ 1 {#fvr-vi-s1-n1-exa-1 .statement}

Với mọi $\lambda \in K$ toán tử gán cho mỗi đa thức $f(X)$ đa thức $f(X + \lambda)$ là một toán tử hợp thành.
2) Đạo hàm D trên K[X] là một toán tử hợp thành (*xem* mệnh đề 1).

#### Nhận xét {#fvr-vi-s1-n1-rem-1 .statement}

Vì K là một trường vô hạn nên toán tử U trên K[X] là một toán tử hợp thành khi và chỉ khi với mọi đa thức $f \in K[X]$ và mọi phần tử $\alpha \in K$ ta có, đặt $g = U(f)$, rằng $g(X + \alpha) = U(f(X + \alpha))$. (Alg., IV. 16, hệ quả).

Rõ ràng mọi tổ hợp tuyến tính của các toán tử hợp thành, với các hệ số trong K, đều là một toán tử hợp thành; điều tương tự cũng đúng đối với hợp thành của hai toán tử hợp thành. Nói cách khác, các toán tử hợp thành tạo thành một đại số con $\Gamma$ của đại số các nội cấu của không gian vectơ K[X].

#### Mệnh đề 1 {#fvr-vi-s1-prop-1 .statement}

*Điều kiện cần và đủ để một toán tử U trên K[X] là một toán tử hợp thành là nó giao hoán với đạo hàm D trên K[X].*

Thật vậy, công thức Taylor cho thấy rằng với mọi đa thức $f \in K[X]$ ta có

$$
U_X(f(X + Y)) = U_X \left( \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k f(X) \right) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k U(D^k f(X));
$$

nếu đặt $g = U(f)$ thì ta có

$$
g(X + Y) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k g(X) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k (U(f(X)));
$$

để U là một toán tử hợp thành, khi đó phải có $UD^k = D^k U$ với mọi số nguyên $k \geq 1$, và đặc biệt $UD = DU$. Ngược lại, nếu quan hệ này đúng, thì nó kéo theo $UD^k = D^k U$ với mọi số nguyên $k \geq 1$, bằng quy nạp theo $k$; khi đó công thức Taylor cho thấy rằng $g(X + Y) = U_X(f(X + Y))$.

Với mọi đa thức $f \in K[X, Y]$ ta ký hiệu bởi $U_0(f)$ số hạng *độc lập với* X trong đa thức $U_X(f)$; đặc biệt, nếu $f \in K[X]$, thì $U_0(f)$ là *số hạng hằng* trong $U(f)$, và $U_0$ là một *dạng tuyến tính* trên $K[X]$. Với mọi đa thức $f \in K[X]$ đặt $g = U(f)$; theo Định nghĩa 1 của VI, p. 270

$$
g(X + Y) = U_X(f(X + Y)) = U_X \left( \sum_{k=0}^{\infty} \frac{1}{k!} X^k D^k f(Y) \right) = \sum_{k=0}^{\infty} \frac{1}{k!} U(X^k) D^k f(Y)
$$

và nếu, trong công thức này, thay X bằng 0, ta thu được

$$
g(Y) = \sum_{k=0}^{\infty} \frac{1}{k!} U_0(X^k) D^k f(Y).
$$

Do đó ta thấy rằng

$$
U(f(X)) = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k f(X) \tag{2}
$$

trong đó $\mu_k$ *là số hạng hằng trong đa thức* $U(X^k)$.

Công thức này cho thấy rằng các $\mu_k$ xác định toán tử hợp thành $U$ một cách hoàn toàn; ngược lại, nếu $(\mu_n)$ là một dãy *tùy ý* các phần tử của K thì công thức (2) xác định một toán tử $U$ mà rõ ràng giao hoán với D, nên theo (VI, p. 270, prop. 1) là một toán tử hợp thành. Từ đây về sau, ta sẽ viết (2) dưới dạng

$$
U = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k. \tag{3}
$$

Công thức này có thể được giải thích bằng ngôn ngữ tôpô như sau: nếu ta xét tôpô rời rạc trên $K[X]$, và tôpô hội tụ *đơn* trên đại số $\mathrm{End}(K[X])$ các nội cấu của $K[X]$ (*Gen. Top.*, X, p. 277), thì chuỗi có số hạng tổng quát $\frac{1}{k!} \mu_k D^k$ hội tụ giao hoán trong $\mathrm{End}(K[X])$ và có tổng là $U$ (*Gen. Top.*, III, p. 269).

Công thức (3) cho thấy rằng với mọi *chuỗi hình thức* $u(S) = \sum_{k=0}^{\infty} \alpha_k S^k$ theo một ẩn trên K (*Alg.*, IV. 41), ta có thể gắn với nó toán tử hợp thành $U = \sum_{k=0}^{\infty} \alpha_k D^k$, mà về sau ta sẽ ký hiệu là $u(D)$. Nhận xét này có thể được làm sáng tỏ theo cách sau:

#### Định lý 1 {#fvr-vi-s1-thm-1 .statement}

*Ánh xạ gán cho mỗi chuỗi hình thức* $u(S) = \sum_{k=0}^{\infty} \alpha_k S^k$ *theo một ẩn trên* K *toán tử hợp thành* $u(D) = \sum_{k=0}^{\infty} \alpha_k D^k$ *trên* $K[X]$ *là một đẳng cấu của đại số* $K[[S]]$ *các chuỗi hình thức lên đại số* $\Gamma$ *các toán tử hợp thành.*

Người ta kiểm tra ngay lập tức rằng ánh xạ này là một đồng cấu. Còn phải thấy rằng nó là đơn ánh, nói cách khác, rằng quan hệ $\sum_{k=0}^{\infty} \alpha_k D^k = 0$ kéo theo $\alpha_k = 0$ với mọi $k$; mà $h! \alpha_h$ là số hạng hằng trong đa thức thu được bằng cách áp dụng $\sum_{k=0}^{\infty} \alpha_k D^k$ cho $X^h$, do đó định lý.

#### Hệ quả {#fvr-vi-s1-n1-cor-1 .statement}

*Đại số $\Gamma$ các toán tử hợp thành trong $K[X]$ là giao hoán.*

#### Ví dụ {#fvr-vi-s1-n1-exa-2 .statement}

Nếu $U$ là toán tử gán cho mỗi đa thức $f(X)$ đa thức $f(X + \lambda)$ (trong đó $\lambda \in K$), thì ta có $U_0(X^k) = \lambda^k$, và do đó $U = \sum_{k=0}^{\infty} \frac{1}{k!} (\lambda D)^k$. Theo phép loại suy với khai triển chuỗi của $e^{\lambda}$ (III, p. 105), ta viết $e^S$ hoặc $\exp(S)$ cho chuỗi hình thức $\sum_{n=0}^{\infty} \frac{1}{n!} S^n$ trong vành $K[[S]]$; vì thế có thể viết $U = e^{\lambda D}$. Thay thế trường $K$ bằng trường phân thức hữu tỉ $K(Y)$ trong lập luận này, ta cũng thấy tương tự rằng *toán tử tịnh tiến* $T_Y$ có thể được viết dưới dạng $e^{YD}$.

Hơn nữa, trong vành $K[[S, T]]$ của các chuỗi hình thức theo hai ẩn bất định trên $K$ ta có

$$
(\exp S)(\exp T) = \sum_{p,q} \frac{S^p}{p!} \frac{T^q}{q!}
$$
$$
= \sum_{n=0}^{\infty} \frac{1}{n!} \left( \binom{n}{0} S^n + \binom{n}{1} S^{n-1} T + \cdots + \binom{n}{n} T^n \right)
$$
$$
= \exp(S + T)
$$

và đặc biệt
$$
(\exp S)(\exp(-S)) = 1
$$
điều này biện minh cho ký hiệu mà chúng ta đã đưa vào.

#### Chú giải {#fvr-vi-s1-n1-sch-1 .statement}

Đẳng cấu của đại số $K[[S]]$ các chuỗi hình thức với đại số $\Gamma$ các toán tử hợp thành trên $K[X]$ đôi khi cho phép chứng minh các mệnh đề về chuỗi hình thức một cách đơn giản nhất bằng cách chứng minh chúng cho các toán tử hợp thành tương ứng (*cf.* VI, p. 274, prop. 6).

### 2. CÁC ĐA THỨC APPELL GẮN VỚI MỘT TOÁN TỬ HỢP THÀNH

Cho một toán tử hợp thành $U = \sum_{k=0}^{\infty} \alpha_k D^k \neq 0$ và gọi $p$ là số nguyên nhỏ nhất trong các số nguyên $k$ sao cho $\alpha_k \neq 0$; ta sẽ nói rằng $p$ là *cấp* của toán tử $U$.

#### Mệnh đề 2 {#fvr-vi-s1-prop-2 .statement}

Mọi toán tử hợp thành cấp 0 đều khả nghịch trong đại số $\Gamma$ các toán tử hợp thành trên $\mathbf{K}[X]$.

Thật vậy, một chuỗi hình thức $\sum_{k=0}^{\infty} \alpha_k S^k$ sao cho $\alpha_0 \neq 0$ là khả nghịch trong vành $\mathbf{K}[[S]]$ (Alg., IV. 41); do đó mệnh đề suy ra từ đ.l. 1 của VI, p. 271.

#### Mệnh đề 3 {#fvr-vi-s1-prop-3 .statement}

Cho $U$ là một toán tử hợp thành cấp $p$; khi đó $U(f) = 0$ với mọi đa thức $f$ bậc $< p$; với mọi đa thức $f \neq 0$ bậc $n \geq p$, $U(f)$ là một đa thức $\neq 0$ bậc $n - p$.

Đây là một hệ quả ngay lập tức của công thức (2) ở VI, p. 271 và của định nghĩa cấp của $U$.

Rõ ràng là mọi toán tử $U$ cấp $p$ đều có thể được viết theo một cách duy nhất dưới dạng $U = D^p V = V D^p$, trong đó $V$ là một toán tử cấp 0 (và do đó khả nghịch).

#### Định nghĩa 2 {#fvr-vi-s1-def-2 .statement}

Cho $U = D^p V$ là một toán tử hợp thành cấp $p$ trên $\mathbf{K}[X]$. Đa thức $u_n(X) = V^{-1}(X^n)$ được gọi là đa thức Appell chỉ số $n$ gắn với toán tử $U$.

Nếu $V^{-1} = \sum_{k=0}^{\infty} \frac{1}{k!} \beta_k D^k$ (với $\beta_0 \neq 0$) thì do đó ta có
$$
u_n(X) = \sum_{k=0}^{n} \binom{n}{k} \beta_k X^{n-k}.
$$
(6)

Ta kiểm tra rằng $u_n$ là một đa thức bậc $n$ (mệnh đề 3); hơn nữa
$$
u_n(0) = \beta_n.
$$

#### Mệnh đề 4 {#fvr-vi-s1-prop-4 .statement}

Các đa thức Appell gắn với $U$ thỏa mãn các hệ thức
$$
\frac{d u_n}{d X} = n \, u_{n-1}
$$
(7)
$$
u_n(X + Y) = \sum_{k=0}^{n} \binom{n}{k} u_{n-k}(X) Y^k
$$
(8)
$$
U(u_n(X)) = \frac{n!}{(n-p)!} X^{n-p}.
$$
(9)

Thực ra, các công thức này lần lượt tương đương với các hệ thức sau (có lưu ý đến định nghĩa 2):

$$
DV^{-1} = V^{-1}D \tag{10}
$$
$$
(\exp(YD_X))V_X^{-1} = V_X^{-1}\exp(YD_X) \tag{11}
$$
$$
UV^{-1} = D^p. \tag{12}
$$

#### Mệnh đề 5 {#fvr-vi-s1-prop-5 .statement}

*Với mọi đa thức $f \in K[X]$ và mọi toán tử hợp thành cấp $p$ ta có*

$$
f^{(p)}(X + Y) = \sum_{k=0}^{\infty} \frac{1}{k!} U \left( f^{(k)}(X) \right) u_k(Y) \tag{13}
$$
*(khai triển Taylor suy rộng)*.

Thật vậy, nếu đặt $U = D^p V = V D^p$ thì ta có (VI, p. 270, công thức (1))

$$
V_X^{-1}(f(X + Y)) = V_Y^{-1}(f(X + Y)) = \sum_{k=0}^{\infty} \frac{1}{k!} f^{(k)}(X) u_k(Y) \tag{14}
$$
công thức Taylor và theo Định nghĩa 2 của VI, p. 273; chỉ cần áp dụng toán tử $U$ cho số hạng thứ nhất và số hạng cuối của công thức (14) để thu được (13).

### 3. CHUỖI SINH CỦA CÁC ĐA THỨC APPELL

Cho E là vành các *chuỗi hình thức* theo một phần tử bất định S, với các hệ số trong vành đa thức $K[X]$ (*Alg.*, IV. 41); nói cách khác, vành các chuỗi hình thức $g(X, S) = \sum_{n=0}^{\infty} \alpha_n(X) S^n$ trong đó các $\alpha_n$ thuộc $K[X]$. Với mọi toán tử $U$ trên $K[X]$ ta xác định một ánh xạ $U_X$ từ E vào chính nó bằng cách đặt $U_X(g(X, S)) = \sum_{n=0}^{\infty} U(\alpha_n) S^n$. Rõ ràng E là một môđun trên vành $K[[S]]$ các chuỗi hình thức theo S với hệ số trong $K$; do tính tuyến tính của $U$ trên $K[X]$, ta kiểm tra ngay lập tức được rằng với mọi phần tử $\theta \in K[[S]]$ và mọi $g \in E$ ta có $U_X(\theta g) = \theta U_X(g)$; nói cách khác, $U_X$ là một ánh xạ tuyến tính của môđun E vào chính nó.

#### Mệnh đề 6 {#fvr-vi-s1-prop-6 .statement}

*Cho $U = D^p V = u(D)$ là một toán tử hợp thành cấp $p$ trên $K[X]$, trong đó $u(S)$ là một chuỗi lũy thừa hình thức cấp $p$ trong $K[[S]]$. Khi đó*

$$
U_X \left( \exp(XS) \right) = u(S) \exp(XS) \tag{15}
$$
$$
\frac{S^p}{u(S)} \exp(XS) = \sum_{n=0}^{\infty} \frac{1}{n!} u_n(X) S^n \tag{16}
$$
*n là đa thức Appell chỉ số n gắn với U*.

Theo chú giải của định lý 1 (VI, p. 271), để thiết lập (15), chỉ cần chỉ ra rằng với mọi đa thức $f(Y) \in K[Y]$ ta có

$$
U_X \left( \exp(XD_Y)(f(Y)) \right) = u(D_Y)(\exp(XD_Y)(f(Y))).
$$

Bây giờ số hạng thứ nhất trong (17) là $U_X(f(X + Y))$, và, vì $U = u(D)$, số hạng thứ hai trong (17) là $U_Y(f(X + Y))$, nên đồng nhất thức (17) được quy về (1) (VI, p. 270).

Bây giờ chỉ còn áp dụng (15) cho toán tử hợp thành $V^{-1} = D^p / u(D)$ để thu được (16), vì theo định nghĩa ta có

$$
V^{-1}(\exp(XS)) = \sum_{n=0}^{\infty} \frac{1}{n!} u_n(X) S^n.
$$

Chú ý rằng (16) cũng có thể thu được bằng cách nhân các chuỗi hình thức $S^p / u(S)$ và $\exp(XS)$, có tính đến (6).

Người ta nói rằng chuỗi hình thức (16) là chuỗi sinh của các đa thức Appell gắn với $U$.

### 4. ĐA THỨC BERNOULLI

Xét toán tử hợp thành $U$ được xác định bởi

$$
U(f(X)) = f(X + 1) - f(X);
$$

ta có thể viết $U = e^D - 1$ (VI, p. 270, Ví dụ 1); đây là một toán tử cấp 1, và nếu đặt $U = DV$ thì ta có $V^{-1} = \frac{D}{e^D - 1}$. Đa thức Appell bậc $n$ tương ứng với toán tử $U$ được gọi là đa thức Bernoulli bậc $n$ và được ký hiệu là $B_n(X)$; nếu đặt $b_n = B_n(0)$ thì ta có các công thức

$$
B_n(X) = \sum_{k=0}^{n} \binom{n}{k} b_{n-k} X^k
$$
(18)

$$
\frac{S \, e^{XS}}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} B_n(X) S^n
$$
(19)

và đặc biệt

$$
\frac{S}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} b_n S^n
$$
(20)

Các công thức (7) và (9) của VI, p. 273, cho, đối với các đa thức Bernoulli, các quan hệ

$$
\frac{dB_n}{dX} = n B_{n-1}(X)
$$
(21)

$$
B_n(X + 1) - B_n(X) = n X^{n-1}.
$$
(22)

Đặc biệt, ta có $B_n(1) - B_n(0) = 0$ với $n > 1$, điều này, có kể đến (18), cho quan hệ quy nạp

$$
\sum_{m=0}^{n-1} \binom{n}{m} b_m = 0 \quad \text{(với } n > 1)
$$

quan hệ này cho phép tính các $b_n$ từng bước. Các số này rõ ràng là *hữu tỉ*; vì ta có thể viết

$$
\frac{S}{e^S - 1} = -\frac{S}{2} + \frac{S}{2} \frac{e^S + 1}{e^S - 1}
$$

và vì (VI, p. 272, công thức (5))

$$
\frac{e^{-S} + 1}{e^{-S} - 1} = -\frac{e^S + 1}{e^S - 1}
$$

nên ta thấy rằng trong chuỗi hình thức của $\frac{S}{2} \frac{e^S + 1}{e^S - 1}$ tất cả các hạng tử bậc *lẻ* đều có hệ số không; do đó ta có

$$
b_0 = 1, \qquad b_1 = -\frac{1}{2}, \qquad b_{2n-1} = 0 \quad \text{với } n > 1.
$$

Các số hữu tỉ $b_{2n}$ ($n \geq 1$) được gọi là các *số Bernoulli*; ta sẽ thấy (VI, p. 288) rằng $b_{2n}$ có dấu của $(-1)^{n-1}$. Công thức (23) cho, đối với các giá trị đầu tiên của $n$,

$$
\begin{align*}
b_2 &= \frac{1}{6}, & b_4 &= -\frac{1}{30}, & b_6 &= \frac{1}{42}, & b_8 &= -\frac{1}{30}, \\
b_{10} &= \frac{5}{66}, & b_{12} &= -\frac{691}{2730}, & b_{14} &= \frac{7}{6}, \\
b_{16} &= -\frac{3617}{510}, & b_{18} &= \frac{43867}{798}, & b_{20} &= -\frac{174611}{330}, & b_{22} &= \frac{854513}{138}, \\
b_{24} &= -\frac{236364091}{2730}, & b_{26} &= \frac{8553103}{6}, & b_{28} &= -\frac{23749461029}{870}.
\end{align*}
$$

Chú ý rằng các tử số 691, 3617, 43867 là nguyên tố; các phân tích thành thừa số nguyên tố của các số khác là

$$
\begin{align*}
174611 &= 283 \times 617 \\
854513 &= 11 \times 131 \times 593 \\
236364091 &= 103 \times 2294797 \\
8553103 &= 13 \times 657931 \\
23749461029 &= 7 \times 9349 \times 362903.
\end{align*}
$$

Từ đó ta suy ra các biểu thức của những đa thức Bernoulli đầu tiên

$$
\begin{align*}
B_0(X) &= 1, & B_1(X) &= X - \frac{1}{2}, & B_2(X) &= X^2 - X + \frac{1}{6}, \\
B_3(X) &= X^3 - \frac{3}{2}X^2 + \frac{1}{2}X, & B_4(X) &= X^4 - 2X^3 + X^2 - \frac{1}{30}.
\end{align*}
$$

### 5. TOÁN TỬ HỢP THÀNH TRÊN CÁC HÀM CỦA MỘT BIẾN THỰC

Cho I là một khoảng trong $\mathbf{R}$ chứa khoảng $\mathbf{R}_+ = [0, +\infty[$; gọi E là một không gian vectơ trên trường $\mathbf{C}$, gồm các hàm của một biến thực nhận giá trị phức, xác định trên I. Giả sử rằng với mọi $a \geqslant 0$ và mọi hàm $f \in E$ thì hàm $x \mapsto f(x + a)$ thuộc E; hơn nữa, giả sử E chứa các hạn chế lên I của các *đa thức với hệ số phức* và các *hàm mũ* $e^{\lambda x}$, trong đó $\lambda$ là một số *phức* tùy ý. Mọi ánh xạ tuyến tính $U$ từ E vào không gian của mọi ánh xạ từ I vào trường $\mathbf{C}$ các số phức sẽ được gọi là một *toán tử* trên E; nếu $f \in E$ và $g = U(f)$ thì sẽ thuận tiện khi dùng ký hiệu

$$
g(x) = U_{\xi}^{\xi}(f(\xi))
$$

trong đó $\xi$ là một biến *giả* trong lối ký hiệu phiếm hàm của số hạng ở vế phải (*xem* II, p. 58). Với mọi $a \geqslant 0$, toán tử gán cho mỗi hàm $f \in E$ hạn chế trên I của hàm $x \mapsto f(x + a)$ được gọi là *toán tử tịnh tiến theo a*.

#### Định nghĩa 3 {#fvr-vi-s1-def-3 .statement}

*Ta nói rằng một toán tử U trên E là một toán tử hợp thành nếu, với mọi $a \geqslant 0$, nó hoán vị được với toán tử tịnh tiến theo a*.

Trong ký hiệu đã được đưa vào ở trên, định nghĩa này trở thành đẳng thức

$$
U_{x+a}^{\xi}(f(\xi)) = U_x^{\xi}(f(\xi + a))
$$

theo $x$ và $a$ ($x \in I, a \geqslant 0$). Có thể đổi vai trò của $x$ và $a$ trong đẳng thức này nếu $x \geqslant 0$, rồi đặt $a = 0$; do đó thu được, với $x \geqslant 0$,

$$
U_x^{\xi}(f(\xi)) = U_0^{\xi}(f(\xi + x))
$$

trong đó $U_0$ là *dạng tuyến tính* trên E mà với mỗi hàm $f \in E$ nó gán giá trị $g(0)$ của $g = U(f)$.

Nếu $f$ là một đa thức, ta có $f(\xi + x) = \sum_{k=0}^{\infty} \frac{1}{k!} f^{(k)}(\xi) x^k$, và công thức (26) cho thấy rằng $U(f)$ cũng là một đa thức; khi hạn chế vào tập hợp các đa thức theo $x$, với hệ số trong $\mathbf{C}$, (một tập hợp có thể đồng nhất với đại số $\mathbf{C}[X]$), thì toán tử $U$ khi đó là một toán tử hợp thành theo nghĩa của định nghĩa I của VI, p. 270, và mọi kết quả của các tiết trước đều có thể áp dụng cho nó.

Ta lại viết $u_n$ để chỉ các đa thức Appell gắn với toán tử $U$. Với khai triển Taylor suy rộng của một đa thức (VI, p. 274, công thức (13)) tương ứng một kết quả sau đây đối với các hàm tổng quát hơn:

#### Định lý 2 {#fvr-vi-s1-thm-2 .statement}

*Cho f là một hàm có đạo hàm bậc $(n + 1)^{th}$ liên tục trên I, và thuộc, cùng với mọi đạo hàm $f^{(m)}$ của nó đối với $1 \leq m \leq n$, vào E. Nếu U là một toán tử hợp thành cấp $p \leq n$ trên E thì ta có, với $x \geq 0$ và $h \geq 0$*

$$
f^{(p)}(x + h) = \sum_{m=0}^{n} \frac{1}{m!} u_m(x) U_h^\xi \left( f^{(m)}(\xi) \right) + R_n(x, h)
$$
(27)

*với*
$$
R_n(x, h) = -U_h^\xi \left( \int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta \right)
$$
(28)
*(khai triển Taylor suy rộng)*.

Xét tích phân $\int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta$, được xác định với mọi $\xi \in I$,
và áp dụng cho nó công thức tích phân từng phần cấp $n + 1$ (II, p. 59, công thức (11)); có kể đến các hệ thức
$$
u_n^{(k)} = n(n-1)\ldots(n-k+1)u_{n-k}
$$
dẫn xuất từ (7) (VI, p. 273) bằng phép truy hồi, ta thu được
$$
\int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta
$$
$$
= \sum_{m=0}^{n} \frac{1}{m!} u_m(x) f^{(m)}(\xi) - \sum_{m=0}^{n} \frac{1}{m!} u_m(\xi - h) f^{(m)}(x + h).
$$
(29)

Ta áp dụng toán tử $U$ cho hai vế của (29), được xét như các hàm của $\xi$, rồi lấy giá trị của hàm thu được ứng với giá trị $h$ của biến $\xi$; nhận thấy rằng, theo các công thức (26) (VI, p. 277) và (9) (VI, p. 272), ta có
$$
U_h^\xi (u_m(\xi - h)) = U_0^\xi (u_m(\xi)) = \begin{cases} 0 & \text{khi } m \neq p \\ p! & \text{khi } m = p \end{cases}
$$
cuối cùng ta thu được (27).

### 6. CHỈ BIỂU CỦA MỘT TOÁN TỬ HỢP THÀNH

Với cùng các giả thiết như ở số 5, công thức (26) của (VI, p. 277), áp dụng cho hàm $e^{\lambda x}$, cho
$$
U_\lambda^\xi (e^{\lambda \xi}) = U_0^\xi (e^{\lambda x} e^{\lambda \xi}) = e^{\lambda x} U_0^\xi (e^{\lambda \xi}) = u(\lambda) e^{\lambda x}
$$
(30)
khi đặt $u(\lambda) = U_0^\xi (e^{\lambda \xi})$. Người ta gọi hàm $u(\lambda)$, xác định trên $\mathbf{C}$, nhận giá trị phức, là *hàm chỉ thị* của toán tử hợp thành $U$. Chú ý rằng nếu hạn chế của $U$ lên vành $\mathbf{C}[X]$ các đa thức bằng chuỗi
$$
D^p \sum_{n=0}^{\infty} \alpha_n D^n
$$
(VI, p. 271, th. 1) (mà chúng tôi đã ký hiệu là $u(D)$ trong VI, p. 271), thì chuỗi *các số hạng phức* có số hạng tổng quát $\alpha_n \lambda^{n+p}$ *không nhất thiết hội tụ* đối với $\lambda \neq 0$, và ngay cả nếu nó hội tụ với một số giá trị của $\lambda$, tổng *không nhất thiết bằng hàm chỉ thị* $u(\lambda)$ *của U* (VI, p. 291, exerc. 2). Chúng tôi sẽ nói rằng toán tử hợp thành $U$ là *chính quy* nếu tồn tại một lân cận của 0 trong $\mathbf{C}$ sao cho chuỗi có số hạng tổng quát $\alpha_n \lambda^{n+p}$ *hội tụ tuyệt đối* và có tổng *bằng hàm chỉ thị* $u(\lambda)$ trên lân cận này$^1$. Hãy áp dụng công thức (27) của VI, p. 278, cho hàm $e^{\lambda x}$, lấy $h = 0$; vì $D^m(e^{\lambda x}) = \lambda^m e^{\lambda x}$ nên ta có $U_0^\xi \left( D^m(e^{\lambda x}) \right) = \lambda^m u(\lambda)$; do đó suy ra rằng với mọi $\lambda$ phức sao cho $u(\lambda) \neq 0$

$$
\frac{\lambda^p e^{\lambda x}}{u(\lambda)} = \sum_{m=0}^n u_m(x) \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} U_0^\xi \left( \int_0^{\xi-x} \frac{1}{n!} u_n(x+\eta) e^{\lambda(\xi-\eta)} d\eta \right)
$$

và đặc biệt, với $x = 0$

$$
\frac{\lambda^p}{u(\lambda)} = \sum_{m=0}^n \beta_m \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} U_0^\xi \left( \int_0^{\xi} \frac{1}{n!} u_n(\eta) e^{\lambda(\xi-\eta)} d\eta \right)
$$

với $\beta_m = u_m(0)$.

Nếu $U$ là một toán tử *chính quy* thì, với mọi $\lambda \in \mathbf{C}$ sao cho các chuỗi nguyên $u(\lambda) = \sum_{n=0}^\infty \alpha_n \lambda^{n+p}$ và $\sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}$ hội tụ tuyệt đối$^2$, từ công thức (16) và công thức về tích của hai chuỗi hội tụ tuyệt đối (*Gen. Top.*, VIII, p. 115, prop. 1) suy ra rằng ta có

$$
\frac{\lambda^p}{u(\lambda)} = \sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}.
$$

Tương tự, vì khai triển Taylor của $e^{\lambda x}$ hội tụ tuyệt đối với mọi $\lambda \in \mathbf{C}$ và mọi $x \in \mathbf{C}$ (III, p. 106), ta cũng có (các công thức (6) (VI, p. 273) và (16) (VI, p. 274)), với mọi giá trị đang xét và với mọi $x \in \mathbf{C}$

$$
\frac{\lambda^n e^{\lambda x}}{u(\lambda)} = \sum_{n=0}^\infty u_n(x) \frac{\lambda^n}{n!}.
$$

#### Nhận xét {#fvr-vi-s1-n6-rem-1 .statement}

Có thể dùng công thức (33) (tương ứng (34)) để tính các $\beta_n$ (tương ứng các $u_n(x)$) bằng cách dùng bổ đề sau về các chuỗi nguyên:

(1) Sau này ta sẽ nghiên cứu các chuỗi mà số hạng tổng quát có dạng $c_n z^n$ ($c_n \in \mathbf{C}, z \in \mathbf{C}$), mà người ta gọi là *chuỗi nguyên*; đặc biệt ta sẽ thấy rằng khi một chuỗi như vậy hội tụ tuyệt đối với $z = z_0$ thì nó *hội tụ chuẩn tắc* với $|z| \leq |z_0|$.
(2) Từ lý thuyết các chuỗi nguyên suy ra rằng khi một trong các chuỗi này hội tụ tuyệt đối trong một lân cận $V$ của 0, thì chuỗi kia hội tụ tuyệt đối trong một lân cận $W \subset V$ của 0.

ổ đề. **Nếu hai chuỗi nguyên** $\sum_{n=0}^{\infty} c_n \lambda^n,\ \sum_{n=0}^{\infty} d_n \lambda^n$ **hội tụ tuyệt đối với mọi** $\lambda$ **trong một lân cận của** $0$, **và nếu** $\sum_{n=0}^{\infty} c_n \lambda^n = \sum_{n=0}^{\infty} d_n \lambda^n$ **với các giá trị này của** $\lambda$, **thì** $c_n = d_n$ **với mọi số nguyên** $n \geqslant 0$.

Nếu, bằng một thủ tục nào đó, ta có thể tìm được một chuỗi nguyên hội tụ tới $\lambda^p / u(\lambda)$ trên một lân cận của $0$, thì các hệ số của chuỗi này tất yếu bằng các $\beta_n / n!$. Đó là thủ tục mà ta sẽ áp dụng trong các ví dụ sau đây.

#### Ví dụ 1 {#fvr-vi-s1-n6-exa-1 .statement}

Nếu $U$ là ánh xạ đồng nhất thì ta có $u(\lambda) = 1$ và toán tử $U$ rõ ràng là kỳ dị; vì $u_n(x) = x^n$ nên công thức (27) của VI, p. 278, có thể viết thành, đặt $\xi = \xi - \eta$

$$
f(x + h) = \sum_{n=0}^{\infty} \frac{1}{m!} f^{(m)}(h) x^m + \int_h^{x+h} f^{(n+1)}(t) \frac{(x + h - t)^n}{n!} dt
$$

nghĩa là, nó quy về công thức Taylor (II, p. 62).

#### Ví dụ 2 {#fvr-vi-s1-n6-exa-2 .statement}

Ta lấy cho $U$ toán tử hợp thành mà với mọi hàm $f$ xác định trên $\mathbf{R}_+$, gắn với nó hàm $x \mapsto f(x + 1) - f(x)$; khi đó

$$
U_{\lambda}^{\xi} (f(\xi)) = f(x + 1) - f(x);
$$

chúng ta đã thấy (VI, p. 275) rằng hạn chế của $U$ lên $\mathbf{C}[X]$ bằng $e^D - 1$. Mặt khác, vì $u(\lambda) = e^{\lambda} - 1$, toán tử $U$ là *chính quy*; chúng ta sẽ thấy (VI, p. 288) cách xác định các số Bernoulli $b_n$ bằng cách tính một khai triển của $\frac{\lambda}{e^{\lambda} - 1}$ thành một chuỗi nguyên hội tụ. Áp dụng công thức (27) của VI, p. 278 cho một nguyên hàm của một hàm $f$ có đạo hàm liên tục bậc $n^{th}$ trên $\mathbf{R}_+$, ta thu được

$$
f(x + h) = \int_h^{h+1} f(t) dt
$$
$$
+ \sum_{m=1}^n \frac{1}{m!} B_m(x) \left( f^{(m-1)}(h+1) - f^{(m-1)}(h) \right) + R_n(x, h)
$$

với

Bổ đề này là một trường hợp riêng của một kết quả tổng quát mà chúng tôi sẽ chứng minh sau; sau đây là chứng minh. Nếu một chuỗi nguyên $\sum_{n=0}^{\infty} c_n \lambda^n$ hội tụ tuyệt đối tại $\lambda = \lambda_0$ thì với mọi số nguyên $k \geqslant 0$ chuỗi $\sum_{n=0}^{\infty} c_{n+k} \lambda^n$ hội tụ chuẩn tắc với $|\lambda| \leqslant |\lambda_0|$, do đó liên tục trên đĩa này (*Gen. Top.*, X, p. 283); suy ra rằng $\sum_{n=k+1}^{\infty} c_n \lambda^n = o(\lambda^k)$ trên một lân cận của $0$. Khi đó bổ đề suy ra từ tính duy nhất của các hệ số của một khai triển tiệm cận của một hàm theo các $\lambda^n$ (V, p. 223).

$$
R_n(x, h) = - \int_0^{1-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h + 1 - \eta) d\eta \\
+ \int_0^{-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h - \eta) d\eta.
$$

(36)

#### Ví dụ 3 {#fvr-vi-s1-n6-exa-3 .statement}

Cho E là không gian vectơ các hàm $f$ xác định và liên tục trên $\mathbf{R}$, và sao cho nguyên $\int_{-\infty}^{+\infty} f(x + \xi) e^{-\xi^2/2} d\xi$ hội tụ với mọi $x \geq 0$. Toán tử U xác định bởi

$$
U_\lambda^\xi \left( f(\xi) \right) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} f(x + \xi) d\xi
$$

khi đó được xác định trên E và rõ ràng là một toán tử hợp thành. Không gian E chứa mọi hàm mũ $e^{\lambda x}$ ($\lambda$ phức tùy ý), và ta có

$$
u(\lambda) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-(\xi^2/2) + \lambda \xi} d\xi \\
= \frac{1}{\sqrt{2\pi}} e^{\lambda^2/2} \int_{-\infty}^{+\infty} e^{-(\xi - \lambda)^2/2} d\xi = e^{\lambda^2/2}
$$

(xem III, p. 120, bài tập 24, và VII, p. 313, công thức (22)). Ta có $n! \alpha_n = U_0^\xi (\xi^n) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} \xi^n d\xi$. Với mọi số nguyên $n$ ta có thể viết

$$
\sum_{k=0}^n \int_{-\infty}^{+\infty} \frac{|\lambda \xi|^k}{k!} e^{-\xi^2/2} d\xi \leq 2 \int_0^{+\infty} e^{-(\xi^2/2) + |\lambda| \xi} d\xi.
$$

Vì thế chuỗi $\sum_{n=0}^{\infty} e^{-\xi^2/2} \frac{(\lambda \xi)^n}{n!}$ có thể được lấy tích phân từng số hạng trên $\mathbf{R}$ (II, p. 72, hệ quả 1), điều đó chứng minh rằng chuỗi $\sum_{n=0}^{\infty} \alpha_n \lambda^n$ hội tụ tuyệt đối với mọi $\lambda \in \mathbf{C}$, và có tổng bằng $u(\lambda) = e^{\lambda^2/2} = \sum_{n=0}^{\infty} \frac{\lambda^{2n}}{2^n n!}$; do đó toán tử $U$ là chính quy. Áp dụng bổ đề đã nhắc ở trên cho thấy rằng $\alpha_{2n} = 1/2^n n!,\ \alpha_{2n+1} = 0$ với mọi $n \geq 0$; do đó toán tử $U$ có cấp 0. Ta có

$$
\frac{1}{u(\lambda)} = e^{-\lambda^2/2} = \sum_{n=0}^{\infty} \frac{(-1)^n \lambda^{2n}}{2^n n!},
$$

chuỗi này hội tụ tuyệt đối với mọi $\lambda \in \mathbf{C}$; một lần áp dụng khác của bổ đề cho thấy rằng $\beta_{2n} = \frac{(-1)^n (2n)!}{2^n n!},\ \beta_{2n+1} = 0$; hơn nữa, chuỗi $\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x)$ hội tụ tuyệt đối với mọi $\lambda \in \mathbf{C}$ và mọi $x \in \mathbf{R}$, và ta có

$$
\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x) = \exp \left( -\frac{\lambda^2}{2} + \lambda x \right) = \exp \left( \frac{x^2}{2} \right) \exp \left( -\frac{1}{2} (\lambda - x)^2 \right).
$$

Khi áp dụng công thức Taylor cho hàm $\exp(-x^2/2)$ thì ta thu được biểu thức sau đây của các đa thức $u_n(x)$:

$$
u_n(x) = (-1)^n e^{\lambda^2/2} \frac{d^n}{dx^n} (e^{-x^2/2}).
$$

Đa thức này được gọi là *đa thức Hermite* bậc $n$, và thường được ký hiệu bởi $\mathrm{H}_n(x)$. Các công thức (7), (8) và (9) của VI, p. 273, ở đây cho

$$
\frac{d \mathrm{H}_n}{dx} = n \mathrm{H}_{n-1}(x)
$$

$$
\mathrm{H}_n(x+y) = \sum_{k=0}^n \binom{n}{k} \mathrm{H}_{n-k}(x) y^k
$$

$$
\frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} \mathrm{H}_n(x+\xi) d\xi = x^n
$$

và công thức (27) ở VI, p. 278, trở thành, với $h = 0$

$$
\sqrt{2\pi} f(x) = \sum_{m=0}^n \left( \int_{-\infty}^{+\infty} e^{\xi^2/2} f^{(m)}(\xi) d\xi \right) \frac{\mathrm{H}_m(x)}{m!}
$$
$$
- \int_{-\infty}^{+\infty} d\xi \int_0^\xi \frac{\mathrm{H}_n(x+\eta)}{n!} e^{-(\xi+\eta)^2/2} f^{(n+1)}(x+\xi-\eta) d\eta.
$$

### 7. CÔNG THỨC CỘNG EULER-MACLAURIN

Trong công thức (35) ở VI, p. 280, hãy thay thế $x$ bằng 0 và $h$ bằng $x$; vì $\mathrm{B}_m(0) = b_m$ nên suy ra từ các hệ thức (24) ở VI, p. 276 rằng với mỗi số nguyên $p > 0$ ta có thể viết

$$
f(x) = \int_x^{x+1} f(t) dt - \frac{1}{2} (f(x+1) - f(x))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(x+1) - f^{(2k-1)}(x) \right) + R_p(x)
$$
với
$$
R_p(x) = - \frac{1}{(2p+1)!} \int_0^1 \mathrm{B}_{2p+1}(t) f^{(2p+1)}(x+1-t) dt.
$$
Trong công thức này, hãy lần lượt thay thế $x$ bằng $x+1, x+2, \ldots, x+n$, và gộp các công thức thu được, từng công thức một; ta được

$$
\begin{cases}
f(x) + f(x+1) + \cdots + f(x+n) \\
= \int_x^{x+n+1} f(t) dt - \frac{1}{2} (f(x+n+1) - f(x)) \\
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x) \right) + T_p(x, n)
\end{cases}
$$
với
$$
T_p(x, n) = - \frac{1}{(2p+1)!} \int_0^1 \mathrm{B}_{2p+1}(t) \left( \sum_{k=0}^n f^{(2p+1)}(x+k+1-t) \right) dt.
$$

Số dư $T_p(x, n)$ trong công thức này có thể được viết lại theo cách sau: ký hiệu $\overline{B}_{2p+1}(t)$ là hàm *tuần hoàn* chu kỳ 1 và bằng $B_{2p+1}(t)$ trên khoảng $[0, 1[$. Khi đó

$$
\int_0^1 B_{2p+1}(t) f^{(2p+1)}(x + k + 1 - t) \, dt = \int_k^{k+1} \overline{B}_{2p+1}(1 - s) f^{(2p+1)}(x + s) \, ds
$$

và do đó

$$
T_p(x, n) = - \frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1 - s) f^{(2p+1)}(x + s) ds.
$$ (41)

Công thức (39) được gọi là *công thức tổng Euler-Maclaurin*; nó áp dụng được cho mọi hàm phức có đạo hàm bậc $(2p + 1)^{th}$ liên tục trên một khoảng $[x_0, +\infty[$, với mọi $x \geq x_0$. Ta sẽ thấy (VI, p. 288) cách ước lượng *số dư* $T_p(x, n)$ trong công thức này.

### Bài tập {#fvr-vi-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).
