---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 4
section_title: APPLICATION TO SERIES WITH POSITIVE TERMS
lang: vi
source: fvr-i-vii
pdf_pages: 0251-0261, 0276-0278
extraction: ocr
subsections:
    - "no": 1
      title: CONVERGENCE CRITERIA FOR SERIES WITH POSITIVE TERMS
      page: 0
      pdf_page: 251
    - "no": 2
      title: ASYMPTOTIC EXPANSION OF THE PARTIAL SUMS OF A SERIES
      page: 0
      pdf_page: 253
    - "no": 3
      title: ASYMPTOTIC EXPANSION OF THE PARTIAL PRODUCTS OF AN INFINITE PRODUCT
      page: 0
      pdf_page: 258
    - "no": 4
      title: 'APPLICATION: CONVERGENCE CRITERIA OF THE SECOND KIND FOR SERIES WITH POSITIVE TERMS'
      page: 0
      pdf_page: 259
statements: 13
exercises: 3
content_sha256: d7a920a824bbcbe300cdb6034689d19515fa3e59e9beccfaa3d56832a909f21a
translated_from: content/en/fvr/V/04_s4_application_to_series_with_positive.md
source_content_sha256: 87c97f97a2aa2a2c80dd6cc88cc89ee66ad2600b9dca489982bfd1a6b369472c
translation_model: gpt-5.4
translation_run: translate-vi-2cce6ac7
glossary_version: 34
glossary_terms_sha256: 82a29aac261f742f7b6de3ab47c4bf45ee26741c3a11bd2a0303273d80c2cc9e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. ỨNG DỤNG VÀO CÁC CHUỖI CÓ CÁC SỐ HẠNG DƯƠNG

### 1. CÁC TIÊU CHUẨN HỘI TỤ ĐỐI VỚI CÁC CHUỖI CÓ CÁC SỐ HẠNG DƯƠNG

Trong mục này, bởi một *chuỗi có các số hạng dương* ta sẽ hiểu (do một sự lạm dụng ngôn ngữ) một chuỗi $ (u_n) $ các số hạng thực sao cho $ u_n \geq 0 $ *kể từ một* giá trị nào đó của n. Mọi điều chúng ta sẽ nói về các chuỗi như vậy đều mở rộng ngay lập tức, bằng cách thay đổi dấu, cho các chuỗi mà mọi số hạng đều $ \leq 0 $ kể từ một giá trị nào đó. Ta đã thấy (II, p. 64, Ví dụ 3) rằng với mọi dãy $ (\mathbf{u}_n)_{n \geq 1} $ các điểm của một không gian định chuẩn E, có thể gắn với nó một hàm bậc thang $ \mathbf{u} $ xác định trên $[1, +\infty[$ bởi các điều kiện $ \mathbf{u}(x) = \mathbf{u}_n $ với $ n \leq x < n+1 $: khi đó chuỗi $ (\mathbf{u}_n) $ hội tụ khi và chỉ khi tích phân $ \int_1^{+\infty} \mathbf{u}(t)\,dt $ hội tụ.

Cho $ (u_n) $ và $ (v_n) $ là hai chuỗi có các số hạng dương, và $ u $ và $ v $ là các hàm bậc thang liên kết: quan hệ $ u_n \leq v_n $ với $ n \geq n_0 $ là tương đương với $ u(x) \leq v(x) $ với $ x \geq n_0 $. Do đó mỗi quan hệ trong các quan hệ $ u_n \preccurlyeq v_n, u_n \ll v_n, u_n \sim v_n $ là tương đương lần lượt với $ u(x) \preccurlyeq v(x), u(x) \ll v(x) $ và $ u(x) \sim v(x) $; nhận xét này cho phép chúng ta dịch các mệnh đề 1 (V, p. 228) và 6 (V, p. 230) như sau:

#### Mệnh đề 1 {#fvr-v-s4-prop-1 .statement}

*Cho* $ (u_n) $ *và* $ (v_n) $ *là hai chuỗi có các số hạng dương. Nếu* $ u_n \preccurlyeq v_n $ *và nếu chuỗi* $ (v_n) $ *hội tụ, thì* $ (u_n) $ *hội tụ; nếu* $ u_n \succ v_n $ *và nếu* $ \sum_{n=1}^{\infty} v_n = +\infty $, *thì* $ \sum_{n=1}^{\infty} u_n = +\infty $.

#### Mệnh đề 2 {#fvr-v-s4-prop-2 .statement}

*Cho* $ (u_n) $ *và* $ (v_n) $ *là hai chuỗi có các số hạng dương*:
1. *Nếu chuỗi* $ (v_n) $ *hội tụ thì quan hệ* $ u_n \ll v_n $ *(tương ứng* $ u_n \sim v_n $) *suy ra* $ \sum_{p=n}^{\infty} u_p \ll \sum_{p=n}^{\infty} v_p $ *(tương ứng* $ \sum_{p=n}^{\infty} u_p \sim \sum_{p=n}^{\infty} v_p $).
2. *Nếu* $ \sum_{n=1}^{\infty} v_n = +\infty $ *thì quan hệ* $ u_n \ll v_n $ *(tương ứng* $ u_n \sim v_n $) *suy ra* $ \sum_{p=1}^{n} u_p \ll \sum_{p=1}^{n} v_p $ *(tương ứng* $ \sum_{p=1}^{n} u_p \sim \sum_{p=1}^{n} v_p $).

Ta thu được các tiêu chuẩn hội tụ tiện lợi bằng cách lấy, đối với chuỗi so sánh $ (v_n) $ trong mệnh đề 1, một chuỗi có các số hạng dạng $ v_n = f(n) $, trong đó $ f $ là một hàm $ \geq 0 $ được xác định với mọi số thực $ x > x_0 $ và giảm trên khoảng $[x_0, +\infty[$; thực vậy:

#### Mệnh đề 3 (tiêu chuẩn Cauchy-Maclaurin) {#fvr-v-s4-prop-3 .statement}

*Nếu* $ f $ *là một hàm* $ \geq 0 $ *và giảm trên* $[x_0, +\infty[$, *thì chuỗi có số hạng tổng quát* $ v_n = f(n) $ *hội tụ khi và chỉ khi tích phân* $ \int_{x_0}^{+\infty} f(t)\,dt $ *hội tụ*.

Để chứng minh điều này, chỉ cần chú ý rằng nếu $ v $ là hàm bậc thang liên kết với chuỗi $ (v_n) $ thì $ v(x+1) \leq f(x) \leq v(x) $ với mọi $ x \geq x_0 $ vì $ f $ giảm; do đó mệnh đề là một hệ quả của nguyên lý so sánh (II, p. 66, mệnh đề 3).

Vì các hàm xuất hiện trong các tiêu chuẩn hội tụ lôgarit đối với tích phân (V, p. 229, mệnh đề 2, 3 và 4) là giảm trên một khoảng $[x_0, +\infty[$, áp dụng mệnh đề 1 và 3 của V, p. 237, cho ta các tiêu chuẩn sau:

#### Mệnh đề 4 ("tiêu chuẩn lôgarit cấp 0") {#fvr-v-s4-prop-4 .statement}

Cho $(u_n)$ là một chuỗi có các số hạng dương; nếu $u_n \preccurlyeq n^\mu$ với một $\mu < -1$ thì chuỗi $(u_n)$ hội tụ; nếu $u_n \succcurlyeq n^\mu$ với một $\mu \geq -1$ thì chuỗi $(u_n)$ có tổng vô hạn.

#### Mệnh đề 5 ("tiêu chuẩn lôgarit cấp $p$") {#fvr-v-s4-prop-5 .statement}

Cho $(u_n)$ là một chuỗi có các số hạng dương. Nếu $u_n \preccurlyeq \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)(l_p(n))^\mu}$ với một $\mu > 1$ thì chuỗi $(u_n)$ hội tụ; nếu $u_n \succcurlyeq \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)(l_p(n))^\mu}$ với một $\mu \leq 1$ thì chuỗi $(u_n)$ có tổng vô hạn.

Nếu $0 \leq q < 1$ thì có $q^n \preccurlyeq n^{-\mu}$ với mọi $\mu > 0$; áp dụng lại tiêu chuẩn lôgarit cấp 0 chứng minh được sự hội tụ của chuỗi hình học $\sum_{n=0}^\infty q^n$ khi $|q| < 1$ (Gen. Top., IV, p. 364). Nếu áp dụng mệnh đề 1 với $v_n = q^n$ thì thu được một tiêu chuẩn có thể phát biểu dưới dạng sau ("tiêu chuẩn Cauchy"): *Cho $(u_n)$ là một chuỗi có các số hạng dương; nếu $\limsup_{n \to \infty}(u_n)^{1/n} < 1$ thì chuỗi $(u_n)$ hội tụ; nếu $\limsup_{n \to \infty}(u_n)^{1/n} > 1$ thì chuỗi $(u_n)$ có tổng vô hạn.* Thật vậy, nếu $\limsup_{n \to \infty}(u_n)^{1/n} = a < 1$ thì $u_n \preccurlyeq q^n$ với mọi $q$ sao cho $a < q < 1$. Mặt khác, nếu $\limsup_{n \to \infty}(u_n)^{1/n} = a > 1$ thì $u_n \succcurlyeq q^n > 1$ với vô hạn nhiều giá trị của $n$, với mọi $q$ sao cho $1 < q < a$; vì $u_n$ không tiến tới 0 nên ta có $\sum_{n=1}^\infty u_n = +\infty$.

Tiêu chuẩn này rất hữu ích trong lý thuyết các *chuỗi nguyên*, mà chúng ta sẽ nghiên cứu về sau; nhưng ngay cả như vậy nó cũng không cho phép quyết định sự hội tụ của chuỗi $(1/n^\alpha)$; nói cách khác, phạm vi áp dụng của nó hạn chế hơn nhiều so với các tiêu chuẩn lôgarit.

### 2. KHAI TRIỂN TIỆM CẬN CỦA CÁC TỔNG RIÊNG CỦA MỘT CHUỖI

Với $x$ thực tiến tới $+\infty$ hãy gọi $\mathcal{E}$ là một thang so sánh gồm các hàm, mỗi hàm được xác định trên một *khoảng toàn phần* $[x_0, +\infty[$ (phụ thuộc vào hàm) và $\geq 0$ trên khoảng này. Cho $(\mathbf{u}_n)$ là một chuỗi mà các số hạng thuộc một không gian định chuẩn đầy đủ $\mathbf{E}$, sao cho $\mathbf{u}_n$ có một khai triển tiệm cận đến cấp chính xác $g_\alpha$ đối với thang $\mathcal{E}'$ gồm các hạn chế lên $\mathbf{N}$ của các hàm trong $\mathcal{E}$:

$$
\mathbf{u}_n = \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda g_\lambda(n) + \mathbf{r}_\alpha(n).
$$

Giả sử rằng mọi tổng riêng phần $\sum_{m=1}^n g(m)$, trong đó $g \in \mathcal{E}$, đều có một khai triển tiệm cận đối với $\mathcal{E}'$. Khi đó có thể thu được một khai triển tiệm cận của các $s_n = \sum_{m=1}^n \mathbf{u}_m$ đối với $\mathcal{E}'$; ở đây nữa ta phân biệt hai trường hợp:

1° $ \sum_{n=1}^{\infty} g_{\alpha}(n) = +\infty $. Khi đó (V, p. 237, mệnh đề 2) ta có $ \sum_{m=1}^{n} r_{\alpha}(m) \ll \sum_{m=1}^{n} g_{\alpha}(m) $:
theo giả thiết, có thể thu được một khai triển tiệm cận của
$$
\sum_{\lambda \leq \alpha} a_{\lambda} \left( \sum_{m=1}^{n} g(m) \right)
$$
(V, p. 222) đến một độ chính xác nào đó $ g_{\sigma} $; nếu $ c g_{\sigma}(n) $ là phần chính của $ \sum_{m=1}^{n} g_{\alpha}(m) $, thì ta sẽ có một khai triển tiệm cận của $ s_{n} $ đến độ chính xác $ g_{\min(\rho,\sigma)} $.

2° $ \sum_{n=1}^{\infty} g_{\alpha}(n) $ hội tụ; khi đó gọi $ \beta $ là nhỏ nhất trong các chỉ số $ \lambda \leq \alpha $ sao cho $ a_{\lambda} \neq 0 $ và sao cho $ \sum_{n=1}^{\infty} g_{\lambda}(n) $ hội tụ; khi đó chuỗi
$$
C = \sum_{n=1}^{\infty} \left( u_{n} - \sum_{\lambda < \beta} a_{\lambda} g_{\lambda}(n) \right)
$$
hội tụ tuyệt đối, và có thể viết
$$
s_{n} = \sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right) - \sum_{m=n+1}^{\infty} r_{\alpha}(m).
$$
Hơn nữa, $ \sum_{m=n+1}^{\infty} r_{\alpha}(m) \ll \sum_{m=n+1}^{\infty} g_{\alpha}(m) $; nếu $ c g_{\sigma}(n) $ là phần chính của $ \sum_{m=n+1}^{\infty} g_{\alpha}(m) $,
và nếu ta có một khai triển tiệm cận của
$$
\sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right)
$$
với độ chính xác $ g_{\rho} $ thì do đó suy ra được một khai triển tiệm cận của $ s_{n} $ với độ chính xác $ g_{\min(\rho,\sigma)} $.

Do đó ta được dẫn tới trường hợp riêng của các chuỗi $ (g(n)) $ trong đó $ g \in \mathcal{E} $. Ta sẽ thấy rằng, với những điều kiện nào đó, có thể thu được ngay một phần chính của $ s_{n} = \sum_{m=1}^{n} g(m) $ (khi $ \sum_{n=1}^{\infty} g(n) = +\infty $) hoặc của $ r_{n} = \sum_{m=n+1}^{\infty} g(m) $ (khi $ \sum_{n=1}^{n} g(n) < +\infty $).

#### Mệnh đề 6 {#fvr-v-s4-prop-6 .statement}

*Cho g là một hàm thực, > 0 và đơn điệu, xác định trên một khoảng [x_0, +\infty[ (trong đó x_0 \leq 1 ), và sao cho log g và x so sánh được cấp 1.*

1° *Nếu g có cấp vô hạn đối với e*, ta có

$$
s_n = \sum_{m=1}^n g(m) \sim g(n) \qquad \text{nếu} \quad \sum_{n=1}^\infty g(n) = +\infty; \tag{1}
$$

$$
r_n = \sum_{m=n+1}^\infty g(m) \sim g(n+1) \qquad \text{nếu} \quad \sum_{n=1}^\infty g(n) < +\infty. \tag{2}
$$

2° *Nếu g có cấp hữu hạn $ \mu $ đối với $ e^x $ thì ta có*

$$
s_n = \sum_{m=1}^n g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_{\lambda_0}^n g(t) \, dt \qquad \text{nếu} \quad \sum_{n=1}^\infty g(n) = +\infty; \tag{3}
$$

$$
r_n = \sum_{m=n+1}^\infty g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_n^\infty g(t) \, dt \qquad \text{nếu} \quad \sum_{n=1}^\infty g(n) < +\infty \tag{4}
$$

(số $ \frac{\mu}{1 - e^{-\mu}} $ được thay bằng 1 trong (3) và (4) khi $ \mu = 0 $).

1° Nếu g có cấp $ +\infty $ đối với $ e^x $ thì ta có $ \log g \gg x $ do đó $ g'/g \gg 1 $, hay $ g' \gg g $, theo giả thiết; bởi vậy g tăng và tiến tới $ +\infty $ cùng với $ x $, do đó $ \sum_{n=1}^\infty g(n) = +\infty $. Nếu $ u $ là hàm bậc thang liên kết với chuỗi $ (g(n)) $ (V, p. 237), thì ta có $ u(x) \leq g(x) $ kể từ một giá trị nào đó của $ x $, nên $ u \ll g $ và do đó

$$
s_{n-1} = \int_1^n u(t) \, dt \ll \int_1^n g(t) \, dt \ll \int_1^n g'(t) \, dt \sim g(n);
$$

vì $ s_n = s_{n-1} + g(n) $ nên ta có $ s_n \sim g(n) $. Chứng minh là tương tự khi g có cấp $ -\infty $ đối với $ e^x $; do đó ta thu được công thức (2).

2° Nếu g có cấp hữu hạn $ \mu $ đối với $ e^x $ thì có thể viết $ g(x) = e^{\mu x} h(x) $ trong đó h có cấp 0 đối với $ e^x $; hơn nữa, theo giả thiết, $ \log g \sim \mu x $ với $ \mu \neq 0 $ ($ \log g \ll x $ với $ \mu = 0 $) suy ra $ h' \ll h $. Trước hết giả sử rằng $ \sum_{n=1}^\infty g(n) = +\infty $ (điều này suy ra $ \mu \geq 0 $; mệnh đề đảo lại luôn đúng nếu $ \mu > 0 $, vì khi đó $ g(x) $ tiến tới $ +\infty $ cùng với $ x $); hãy tính phần chính của $ \int_{n-1}^n g(t) \, dt $. Có thể viết

$$
\int_{n-1}^n g(t) \, dt = \int_{n-1}^n e^{\mu t} h(t) \, dt
$$
$$
= h(n) \int_{n-1}^n e^{\mu t} \, dt + \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt
$$
$$
= \frac{1 - e^{-\mu}}{\mu} g(n) + \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt.
$$

Bây giờ, quan hệ $ h' \ll h $ kéo theo rằng với mọi $ \varepsilon > 0 $ tồn tại một $ n_0 $ sao cho quan hệ $ x \geq n_0 $ kéo theo $ |h'(x)/h(x)| \leq \varepsilon $; từ định lý giá trị trung bình suy ra rằng $ -\varepsilon \leq \log |h(t)/h(n)| \leq \varepsilon $, với $ n-1 \leq t \leq n $, nếu $ n \geq n_0 $, do đó

$$
|h(t) - h(n)| \leq (e^\varepsilon - 1)h(n)
$$

và do đó

$$
\left| \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt \right| \leq (e^\varepsilon - 1)e^{\mu n}h(n) = (e^\varepsilon - 1)g(n)
$$

vì $ e^{\mu t} $ tăng. Vì $ e^\varepsilon - 1 $ trở nên nhỏ tùy ý cùng với $ \varepsilon $ nên ta thấy rằng có thể viết

$$
\int_{n-1}^n g(t) \, dt = \frac{1 - e^{-\mu}}{\mu} g(n) + o(g(n))
$$

$ \left( \frac{1 - e^{-\mu}}{\mu} \text{ được thay bởi } 1 \text{ khi } \mu = 0 \right) $. Mệnh đề khi đó là hệ quả của mệnh đề 2 của V, p. 237. Ta lập luận tương tự khi $ \sum_{n=1}^\infty g(n) $ hữu hạn.

Bằng cách áp dụng mệnh đề 6 của V, p. 239 nhiều lần, khi đó đôi khi có thể thu được một *khai triển tiệm cận* cho $ s_n = \sum_{m=1}^n g(m) $. Trước hết giả sử rằng $ g $ có cấp $ +\infty $ đối với $ e^\lambda $; với mọi giá trị *cố định* của $ p $ ta có thể viết, theo mệnh đề 6,

$$
s_n = g(n) + g(n-1) + \cdots + g(n-p) + o(g(n-p))
$$

và chỉ cần khai triển (đối với $ \mathcal{E}' $) mỗi hàm trong các hàm $ g(n-k) $ ($ 0 \leq k \leq p $), bằng cách giới hạn độ chính xác của các khai triển tới phần chính của $ g(n-p) $, để thu được một khai triển của $ s_n $.

#### Ví dụ {#fvr-v-s4-n2-exa-1 .statement}

Cho $ g(x) = x^\lambda = \exp(\lambda \log x) $, có cấp $ +\infty $ đối với $ e^\lambda $. Lấy $ p = 2 $ ta có

$$
(n-1)\log(n-1) = (n-1)\log n - 1 + \frac{1}{2n} + o\left( \frac{1}{n} \right)
$$

do đó (V, p. 225)

$$
(n-1)^{n-1} = \frac{1}{e} n^{n-1} + \frac{1}{2e} n^{n-2} + o_1\left( n^{n-2} \right)
$$

và tương tự

$$
(n-2)^{n-2} = \frac{1}{e^2} n^{n-2} + o_2\left( n^{n-2} \right);
$$

do đó

$$
s_n = n^n + \frac{1}{e} n^{n-1} + \left( \frac{1}{2e} + \frac{1}{e^2} \right) n^{n-2} + o_3\left( n^{n-2} \right).
$$

Ta làm tương tự (đối với $ r_n $) khi $ g $ có cấp $ -\infty $ đối với $ e^\lambda $.

Bây giờ nếu $ g $ có cấp hữu hạn $ \mu $ đối với $ e^x $, và nếu, chẳng hạn, $ \sum_{n=1}^\infty g(n) = +\infty $, ta có thể viết
$$
s_n = \frac{\mu}{1 - e^{-\mu}} \int_1^n g(t)\, dt + \sum_{m=1}^n f_1(m)
$$
trong đó $ f_1(n) = g(n) - \frac{\mu}{1 - e^{-\mu}} \int_1^n g(t)\, dt \ll g(n) $ theo mệnh đề 6 của V, p. 239. Nếu ta có một phần chính $ c g_1(n) $ của $ f_1(n) $ đối với $ \mathcal{E}' $, và nếu ta lại có thể áp dụng mệnh đề 6 cho hàm $ g_1 $ thì ta sẽ thu được một nguyên hàm tương đương với $ \sum_{m=1}^n f_1(m) $ nếu $ \sum_{n=1}^\infty g_1(n) = +\infty $, và tương đương với $ \sum_{m=n+1}^\infty f_1(m) $ trong trường hợp đối (trong trường hợp sau, ta viết $ \sum_{m=1}^n f_1(m) = C - \sum_{m=n+1}^\infty f_1(m) $, với $ C = \sum_{n=1}^\infty f_1(n) $).

Từng bước một, do đó rốt cuộc có thể thu được một biểu thức của $ s_n $ dưới dạng tổng của một số nhất định nguyên hàm, mỗi nguyên hàm đều không đáng kể đối với nguyên hàm đứng trước, của một số hạng còn lại không đáng kể đối với nguyên hàm cuối cùng đã viết, và cuối cùng là một hằng số (trường hợp số hạng dư tiến tới 0). Khi đó còn phải khai triển mỗi nguyên hàm thu được theo $ \mathcal{E}' $ (x. V, p. 235).

#### Ví dụ {#fvr-v-s4-n2-exa-2 .statement}

Cho $ g(n) = \frac{1}{n} $; khi đó
$$
s_n = \sum_{m=1}^n \frac{1}{m} \sim \int_1^n \frac{dt}{t} = \log n
$$
rồi
$$
\frac{1}{n} - (\log n - \log(n-1)) \sim -\frac{1}{2n^2}
$$
do đó
$$
s_n = \log n + \gamma + \frac{1}{2n} + o\left(\frac{1}{n}\right).
$$
Hằng số $ \gamma $ xuất hiện trong công thức này giữ một vai trò quan trọng trong Giải tích (x. chap. VI và VII); nó được gọi là *hằng số Euler*; ta có
$$
\gamma = 0.577\,215\,664\ldots
$$
chính xác đến $ 1/10^9 $.

Ta sẽ thấy ở VI, p. 288, công thức *cầu tích Euler-Maclaurin* cho một khai triển tiệm cận đến cấp *tùy ý* đối với $ s_n $ (hoặc đối với $ r_n $) trong những trường hợp quan trọng nhất như thế nào.

### 3. KHAI TRIỂN TIỆM CẬN CỦA CÁC TÍCH TỪNG PHẦN CỦA MỘT TÍCH VÔ HẠN

Ta biết (Gen. Top., V. p. 22 và 23) rằng để tích vô hạn với nhân tử tổng quát $ 1 + u_n $ ($ u_n > -1 $) hội tụ (ứng với hội tụ giao hoán), điều kiện cần và đủ là chuỗi có số hạng tổng quát $ \log(1 + u_n) $ hội tụ (ứng với hội tụ giao hoán), và khi đó ta có quan hệ

$$
\log \prod_{n=1}^{\infty} (1 + u_n) = \sum_{n=1}^{\infty} \log(1 + u_n).
$$

Khi tích vô hạn hội tụ thì ta biết rằng $ u_n $ tiến tới 0; do đó $ \log(1 + u_n) \sim u_n $; bây giờ ta biết rằng để một chuỗi số thực hội tụ giao hoán thì điều kiện cần và đủ là nó hội tụ tuyệt đối (Gen. Top., IV, p. 372, mệnh đề 5); do mệnh đề 1, như vậy ta thu lại được sự kiện rằng tích có nhân tử tổng quát $ 1 + u_n $ hội tụ giao hoán khi và chỉ khi chuỗi có số hạng tổng quát $ u_n $ hội tụ tuyệt đối (Gen. Top., IV, p. 368, định lý 4).

Một lập luận tương tự áp dụng cho một tích vô hạn có nhân tử tổng quát là một số phức $ 1 + u_n $ ($ u_n \neq -1 $). Thật vậy, để một tích như thế hội tụ giao hoán thì điều kiện cần và đủ (Gen. Top., VIII, p. 115, mệnh đề 2) là tích vô hạn có nhân tử tổng quát $ |1 + u_n| $ cũng như vậy, và thêm nữa, nếu $ \theta_n $ là biên độ của $ 1 + u_n $ (lấy giữa $ -\pi $ và $ +\pi $), thì chuỗi các $ \theta_n $ phải hội tụ giao hoán. Vì $ u_n $ tiến tới 0, $ \log(1 + u_n) $ được xác định kể từ một giá trị nào đó của $ n $ (III, p. 100) và ta có

$$
\log(1 + u_n) = \log |1 + u_n| + i \theta_n;
$$

do đó, để tích có nhân tử tổng quát $ 1 + u_n $ là hội tụ giao hoán thì điều kiện cần và đủ là chuỗi có số hạng tổng quát $ |\log(1 + u_n)| $ hội tụ tuyệt đối (Top. Gen., VII, p. 84, th. 1); mà $ \log(1 + u_n) \sim u_n $ (I, p. 18, prop. 5), nên lại thu được điều kiện rằng chuỗi có số hạng tổng quát $ u_n $ phải hội tụ tuyệt đối (Top. Gen., VIII, p. 116, th. 1).

Quan hệ giữa tích vô hạn và các chuỗi số thực đôi khi cho phép thu được một khai triển tiệm cận của tích riêng phần $ p_n = \prod_{k=1}^{n} (1 + u_k) $; chỉ cần có một khai triển tiệm cận của tổng riêng phần $ s_n = \sum_{k=1}^{n} \log(1 + u_k) $, rồi khai triển $ p_n = \exp(s_n) $; như vậy ta lại quay về hai bài toán đã xét trước đây (V, p. 238 và p. 226).

*Ví dụ: công thức Stirling.* Ta hãy tìm một khai triển tiệm cận của $ n! $; điều này dẫn ta đến việc khai triển $ s_n = \sum_{p=1}^{n} \log p $, rồi sau đó $ \exp(s_n) $. Phương pháp ở n 2 lần lượt cho

$$
s_n = \sum_{p=1}^{n} \log p \sim \int_{1}^{n} \log t \, dt = n \log n - n + 1
$$

khi đó
$$
\log n - \int_{n-1}^{n} \log t \, dt = \log n - (n \log n - (n-1) \log(n-1) - 1) \sim \frac{1}{2n}
$$
do đó
$$
s_n = n \log n - n + \frac{1}{2} \log n + o(\log n).
$$
Khi đó
$$
\log n - \int_{n-1}^{n} \log t \, dt - \frac{1}{2} (\log n - \log(n-1)) \sim -\frac{1}{12n^2}
$$
do đó
$$
s_n = n \log n - n + \frac{1}{2} \log n + k + \frac{1}{12n} + o_1 \left( \frac{1}{n} \right) \quad (k \text{ hằng})
$$
và cuối cùng suy ra được (V, p. 226)
$$
n! = e^k \, n^{n+1/2} \, e^{-n} \left( 1 + \frac{1}{12n} + o_2 \left( \frac{1}{n} \right) \right). \tag{5}
$$
Ta sẽ chứng minh trong VII, p. 322, rằng $ e^k = \sqrt{2\pi} $. Công thức (5) (với giá trị này của $ k $) được gọi là *công thức Stirling*. Theo cùng cách đó, với mọi số thực $ a $ không là một số nguyên $ > 0 $, ta chứng minh được rằng
$$
(a+1)(a+2)\ldots(a+n) \sim K(a) \, n^{n+a+\frac{1}{2}} \, e^{-n}. \tag{6}
$$
Ta cũng sẽ xác định hàm $ K(a) $ (VII, p. 18). Từ các công thức (5) và (6) đặc biệt suy ra rằng
$$
\binom{a}{n} \sim (-1)^n \varphi(a) \, n^{-a-1} \tag{7}
$$
với mọi số thực $ a $ không là một số nguyên $ > 0 $, trong đó $ \varphi(a) $ là một hàm của $ a $ sẽ được nêu rõ trong VII, p. 322.

### 4. ỨNG DỤNG: CÁC TIÊU CHUẨN HỘI TỤ LOẠI THỨ HAI CHO CÁC CHUỖI VỚI CÁC HẠNG DƯƠNG

Khá thường gặp những chuỗi $ (u_n) $ mà từ một chỗ nào đó trở đi có $ u_n > 0 $, và $ u_{n+1}/u_n $ có một khai triển tiệm cận dễ xác định. Đối với những chuỗi như vậy, thật thuận tiện khi có các tiêu chuẩn (gọi là *các tiêu chuẩn loại thứ hai*) cho phép xác định chuỗi có hội tụ hay không chỉ từ dạng của $ u_{n+1}/u_n $. Sau đây là một tiêu chuẩn như vậy:

#### Mệnh đề 7 ("tiêu chuẩn Raabe") {#fvr-v-s4-prop-7 .statement}

*Cho $ (u_n) $ là một chuỗi mà từ một chỗ nào đó trở đi các hạng đều $ > 0 $. Nếu, kể từ một chỉ số nào đó, $ u_{n+1}/u_n \leqslant 1 - \frac{\alpha}{n} $ với một $ \alpha > 1 $, thì chuỗi $ (u_n) $ hội tụ; nếu, từ một chỗ nào đó trở đi, $ u_{n+1}/u_n \geqslant 1 - \frac{1}{n} $, thì chuỗi $ (u_n) $ có tổng vô hạn.*

Thật vậy, nếu $ u_{n+1}/u_n \leqslant 1 - \frac{\alpha}{n} $ với $ \alpha > 1 $, với mọi $ n \geqslant n_0 $, thì ta có $ u_n \preccurlyeq p_n = \prod_{k=n_0}^{n} \left( 1 - \frac{\alpha}{k} \right) $. Bây giờ, $ \log \left( 1 - \frac{\alpha}{n} \right) = -\frac{\alpha}{n} - \frac{\alpha^2}{2n^2} + o \left( \frac{1}{n^2} \right) $, do đó $ \log p_n = $ $-\alpha \log n + k + o(1/n)$ ($k$ hằng), và $p_n \sim e^k \frac{1}{n^\alpha}$; vì $\alpha > 1$ nên tiêu chuẩn lôgarit cấp 0 cho phép kết thúc.

Mặt khác, nếu $u_{n+1}/u_n \geq 1 - \frac{1}{n}$ kể từ một điểm nào đó, thì phép tính tương tự chứng minh rằng $u_n \geq \frac{1}{n}$, do đó có mệnh đề.

Cũng có thể chứng minh theo cùng cách, bằng cách dùng các tiêu chuẩn lôgarit cấp $> 0$, tiêu chuẩn sau đây loại thứ hai:

#### Mệnh đề 8 {#fvr-v-s4-prop-8 .statement}

*Cho $(u_n)$ là một chuỗi có các số hạng $> 0$ kể từ một điểm nào đó. Nếu, kể từ một điểm nào đó, ta có*

$$
\frac{u_{n+1}}{u_n} \leq 1 - \frac{1}{n} - \frac{1}{nl_1(n)} - \ldots - \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)} - \frac{\alpha}{nl_1(n)l_2(n)\ldots l_p(n)}
$$

*nếu với một $\alpha > 1$ nào đó, thì chuỗi $(u_n)$ hội tụ; nếu, kể từ một điểm nào đó trở đi, ta có*

$$
\frac{u_{n+1}}{u_n} \geq 1 - \frac{1}{n} - \frac{1}{nl_1(n)} - \ldots - \frac{1}{nl_1(n)l_2(n)\ldots l_p(n)}
$$

*thì chuỗi $(u_n)$ có tổng vô hạn.*

#### Ví dụ {#fvr-v-s4-n4-exa-1 .statement}

Xét *chuỗi siêu bội*, có số hạng tổng quát

$$
u_n = \frac{\alpha(\alpha+1)\ldots(\alpha+n-1)\,\beta(\beta+1)\ldots(\beta+n-1)}{1.2\ldots n.\gamma(\gamma+1)\ldots(\gamma+n-1)}
$$

trong đó $\alpha, \beta, \gamma$ là các số thực tùy ý, không là các số nguyên $\leq 0$: hiển nhiên là $u_n$ thì $> 0$ kể từ một giai đoạn nào đó, hoặc $< 0$ kể từ một giai đoạn nào đó trở đi. Ta có

$$
\begin{align*}
\frac{u_{n+1}}{u_n} &= \frac{(\alpha+n)(\beta+n)}{(n+1)(\gamma+n)} \\
&= \left(1 + \frac{\alpha+\beta}{n} + \frac{\alpha\beta}{n^2}\right) \left(1 + \frac{\gamma+1}{n} + \frac{\gamma}{n^2}\right)^{-1} \\
&= 1 + \frac{\alpha+\beta-\gamma-1}{n} \\
&\quad + \frac{\alpha\beta-(\alpha+\beta)(\gamma+1)+\gamma^2+\gamma+1}{n^2} + o\left(\frac{1}{n^2}\right).
\end{align*}
$$

Tiêu chuẩn Raabe cho thấy rằng chuỗi hội tụ khi $\alpha + \beta < \gamma$, và có tổng vô hạn khi $\alpha + \beta > \gamma$; khi $\alpha + \beta = \gamma$ thì chuỗi cũng có tổng vô hạn, như được chỉ ra bởi mệnh đề 8.

#### Nhận xét 1 {#fvr-v-s4-n4-rem-1 .statement}

Như một trường hợp riêng của tiêu chuẩn của Raabe, ta thấy rằng nếu $\limsup_{n \to \infty} u_{n+1}/u_n < 1$ thì chuỗi $(u_n)$ hội tụ; còn nếu $\liminf_{n \to \infty} u_{n+1}/u_n > 1$ thì chuỗi $(u_n)$ có tổng vô hạn (*tiêu chuẩn của d'Alembert*).

#### Nhận xét 2 {#fvr-v-s4-n4-rem-2 .statement}

Các tiêu chuẩn loại thứ hai chỉ có thể được áp dụng cho những chuỗi mà số hạng tổng quát biến thiên theo một cách rất chính quy khi $n$ tiến tới $+\infty$; nói cách khác, phạm vi áp dụng của chúng hạn chế hơn nhiều so với các tiêu chuẩn lôgarit, và sẽ là một sai lầm nếu cố dùng chúng vượt ra ngoài những trường hợp đặc biệt mà chúng đặc biệt thích hợp. Chẳng hạn, đối với chuỗi $(u_n)$ xác định bởi $u_{2m} = 2^{-m}$, $u_{2m+1} = 3^{-m}$ ta có $u_{2m+1}/u_{2m} = \left(\frac{2}{3}\right)^m$, $u_{2m+2}/u_{2m+1} = \frac{1}{2} \left(\frac{3}{2}\right)^m$; tỉ số thứ nhất trong các tỉ số này tiến tới 0 và tỉ số thứ hai tiến tới $+\infty$ khi $m$ tăng vô hạn, nên không tiêu chuẩn nào thuộc loại thứ hai có thể áp dụng được; tuy nhiên, vì $u_n \preccurlyeq 2^{-n/2}$, nên ngay lập tức suy ra rằng chuỗi hội tụ.

Ngay cả khi $u_{n+1}/u_n$ có một biểu thức đơn giản, việc đánh giá trực tiếp một phần chính của $u_n$ thường dẫn đến kết quả nhanh chẳng kém các tiêu chuẩn loại thứ hai. Chẳng hạn, đối với chuỗi hypergeometric, công thức Stirling cho thấy ngay lập tức rằng $u_n \sim a n^{\alpha + \beta - \gamma - 1}$, trong đó $a$ là một hằng $\neq 0$, và khi đó tiêu chuẩn logarithm cấp 0 là áp dụng được.

### Bài tập {#fvr-v-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
