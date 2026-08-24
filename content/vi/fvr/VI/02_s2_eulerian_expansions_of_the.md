---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 2
section_title: EULERIAN EXPANSIONS OF THE TRIGONOMETRIC FUNCTIONS AND BERNOULLI NUMBERS
lang: vi
source: fvr-i-vii
pdf_pages: 0298-0303, 0307-0311
extraction: ocr
subsections:
    - "no": 1
      title: EULERIAN EXPANSION OF $ \cot z $
      page: 0
      pdf_page: 298
    - "no": 2
      title: EULERIAN EXPANSION OF $ \sin z $
      page: 0
      pdf_page: 301
    - "no": 3
      title: APPLICATION TO THE BERNOULLI NUMBERS
      page: 0
      pdf_page: 302
statements: 5
exercises: 1
content_sha256: 2622a21b2a42daa8fb9cbfd138a6197d5ea43e452c0153b0663993d5193defe2
translated_from: content/en/fvr/VI/02_s2_eulerian_expansions_of_the.md
source_content_sha256: 0dad261156c428389028cbfb5e9f6e4e1b2a32c74de3d12c098e8bfd126ac99b
translation_model: gpt-5.4, copied
translation_run: translate-vi-4168b8cf
glossary_version: 34
glossary_terms_sha256: 26051e8153a4f2954abe1e8ace9f99eaff9fbf4a01f6fe0ba28af2099dd56d5f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. KHAI TRIỂN EULER CỦA CÁC HÀM LƯỢNG GIÁC VÀ CÁC SỐ BERNOULLI

### 1. KHAI TRIỂN EULER CỦA $ \cot z $

Theo công thức (20) của VI, p. 275, các số $b_n / n!$ là các hệ số trong khai triển của $S/(e^S - 1)$ thành một chuỗi *hình thức*; trong tiết này chúng ta sẽ chỉ ra rằng hàm $z/(e^z - 1)$ bằng tổng của một chuỗi nguyên chỉnh tuyệt đối hội tụ trên một lân cận của 0 trong $\mathbf{C}$; từ bổ đề ở VI, p. 280 sẽ suy ra rằng các hệ số của chuỗi này là các số $b_n / n!$, từ đó chúng ta sẽ suy ra các ước lượng đối với các số Bernoulli $b_n$.

Trước hết ta chú ý rằng

$$
\frac{z}{e^z - 1} = - \frac{z}{2} + \frac{z}{2} \frac{e^z + 1}{e^z - 1} = - \frac{z}{2} + \frac{iz}{2} \cot \frac{iz}{2}.
$$ (1)

Dưới đây ta sẽ thu được một khai triển thành chuỗi của $\cot z$, đúng với mọi $z$ không phải là bội số nguyên của $\pi$.

#### Mệnh đề 1 {#fvr-vi-s2-prop-1 .statement}

*Với mọi số phức* $z$ *và mọi số nguyên* $n$ *ta có*

$$
\sin nz = 2^{n-1} \sin z \sin \left(z + \frac{\pi}{n}\right) \sin \left(z + \frac{2\pi}{n}\right) \ldots \sin \left(z + \frac{(n-1)\pi}{n}\right).
$$ (2)

Thật vậy, ta có thể viết

$$
\sin nz = \frac{e^{niz} - e^{-niz}}{2i} = \frac{e^{-niz}(e^{2niz} - 1)}{2i}
= \frac{e^{-niz}(e^{2iz} - 1)(e^{2iz} - e^{-2i\pi/n}) \ldots (e^{2iz} - e^{-2(n-1)i\pi/n})}{2i}
= A \sin z \sin \left( z + \frac{\pi}{n} \right) \sin \left( z + \frac{2\pi}{n} \right) \ldots \sin \left( z + \frac{(n-1)\pi}{n} \right)
$$

trong đó
$$
A = (2i)^{n-1} e^{-\frac{i\pi}{n}(1+2+\ldots+(n-1))} = (2i)^{n-1} e^{-i(n-1)\frac{\pi}{2}} = 2^{n-1}.
$$

#### Hệ quả 1 {#fvr-vi-s2-prop-1-cor-1 .statement}

*Với mọi số nguyên n, ta có*
$$
\sin \frac{\pi}{n} \sin \frac{2\pi}{n} \ldots \sin \frac{(n-1)\pi}{n} = \frac{n}{2^{n-1}}.
$$
(3)

Chỉ cần chia cả hai vế của (2) cho $\sin z$ rồi cho $z$ tiến tới 0.

#### Hệ quả 2 {#fvr-vi-s2-prop-1-cor-2 .statement}

*Với mọi số nguyên lẻ $n = 2m + 1$, và mọi số phức $z$ sao cho $nz$ không là một bội nguyên của $\pi$, ta có*
$$
\cot nz = (-1)^m \cot z \cot \left( z + \frac{\pi}{n} \right) \ldots \cot \left( z + \frac{(n-1)\pi}{n} \right).
$$
(4)

Thật vậy, $\sin n \left( z + \frac{\pi}{2} \right) = \sin \left( nz + \frac{\pi}{2} + m\pi \right) = (-1)^m \cos nz$, do đó, thay thế $z$ bởi $z + \frac{\pi}{2}$ trong (2),

$$
\cos nz = (-1)^m 2^{n-1} \cos z \cos \left( z + \frac{\pi}{n} \right) \ldots \cos \left( z + \frac{(n-1)\pi}{n} \right)
$$
(5)

và các công thức (2) và (5) cho (4) bằng cách chia từng số hạng khi $\sin nz \neq 0$.

Trong tất cả những gì tiếp theo, ta sẽ luôn giả thiết rằng $n = 2m + 1$ là một số nguyên lẻ; công thức (4) cũng có thể được viết thành

$$
\cot nz = (-1)^m \prod_{k=-m}^{m} \cot \left( z - \frac{k\pi}{n} \right).
$$

hoặc, ta có

$$
\cot \left( z - \frac{k\pi}{n} \right) = \frac{1 + \tan z \tan \frac{k\pi}{n}}{\tan z - \tan \frac{k\pi}{n}}
$$

khi tan z hữu hạn; do đó cot $ nz $ là một hàm hữu tỉ theo $ u = \tan z $, mà tử số có bậc $ n - 1 $, và mẫu số, có bậc $ n $, có $ n $ nghiệm đơn $ \tan k\pi / n $; phân tích thành các phân thức đơn cho

$$
\cot nz = \sum_{k=-m}^{m} \frac{A_k}{u - \tan \frac{k\pi}{n}}
$$

trong đó

$$
A_k = \lim_{z \to k\pi/n} \cot nz \left( \tan z - \tan \frac{k\pi}{n} \right) = \lim_{z \to k\pi/n} \frac{\cos nz}{\sin nz} \frac{\sin \left( z - \frac{k\pi}{n} \right)}{\cos z \cos \frac{k\pi}{n}}
$$
$$
= \lim_{h \to 0} \frac{\cos nh}{\cos \frac{k\pi}{n} \cos \left( h + \frac{k\pi}{n} \right)} \frac{\sin h}{\sin nh} = \frac{1}{n \cos^2 \frac{k\pi}{n}}
$$

do đó, khi tách riêng số hạng trong (6) tương ứng với $ k = 0 $ và gộp các số hạng tương ứng với các giá trị đối của $ k $, rồi thay thế $ z $ bởi $ z/n $,

$$
\cot z = \frac{1}{n \tan \frac{z}{n}} + \sum_{k=1}^{m} \frac{2n \tan \frac{z}{n}}{\cos^2 \frac{k\pi}{n} \left( n \tan \frac{z}{n} \right)^2 - \left( n \sin \frac{k\pi}{n} \right)^2}
$$

đúng với mọi số phức $ z $ không là một bội nguyên của $ \pi/2 $. Ta có thể viết công thức này dưới dạng

$$
\cot z = \frac{1}{n \tan \frac{z}{n}} + \sum_{k=1}^{\infty} v_k(n, z)
$$

với $ v_k(n, z) = 0 $ đối với $ k > m $ và

$$
v_k(n, z) = \frac{2n \tan \frac{z}{n}}{\cos^2 \frac{k\pi}{n} \left( n \tan \frac{z}{n} \right)^2 - \left( n \sin \frac{k\pi}{n} \right)^2}
$$

đối với $ 1 \leq k \leq m $. Ta sẽ thấy rằng với mọi $ z $ được chứa trong một tập con compắc K của $ \mathbf{C} $, không chứa một bội nguyên nào của $ \pi $, và với mọi $ n $ lẻ đủ lớn, chuỗi có số hạng tổng quát $ v_k(n, z) $ là hội tụ chuẩn tắc. Thật vậy, khi $ n $ tiến tới $ +\infty $, $ \tan \frac{z}{n} $ tiến tới $ \frac{z}{n} $ đều trên K, nên tồn tại một số $ M > 0 $ sao cho $ \left| n \tan \frac{z}{n} \right| \leq M $ với mọi $ m $ đủ lớn và mọi $ z \in K $. Mặt khác, với $ 0 \leq x \leq \pi/2 $ ta có $ \sin x / x \geq 1 - \frac{x^2}{6} \geq \frac{1}{2} $, nên với $ 1 \leq k \leq m $ ta có $ n \sin \frac{k\pi}{n} \geq k\pi/2 $; do đó, khi $ m $ đủ lớn, với mọi số nguyên $ k $ sao cho t $ k\pi /2 > M $ ta có $ |v_k(n, z)| \leq \frac{8M}{k^2 \pi^2 - 4M^2} $, điều đó chứng minh mệnh đề của ta. Với $ k $ lẻ, $ v_k(n, z) $ tiến tới $ \frac{2z}{z^2 - k^2 \pi^2} $ (đều trên K) khi $ n $ tiến tới $ +\infty $. Do đó:

#### Định lý 1 {#fvr-vi-s2-thm-1 .statement}

*Với mọi số phức $ z $ không phải là bội nguyên của $ \pi $ ta có*

$$
\cot z = \frac{1}{z} + \sum_{n=1}^{\infty} \frac{2z}{z^2 - n^2 \pi^2}
$$

*(chuỗi ở phải hội tụ chuẩn tắc trên mọi tập con compắc $ K \subset \mathbf{C} $ chứa bất kỳ bội số nguyên nào của $ \pi $ (khai triển Euler của $ \cot z $).)*

### 2. KHAI TRIỂN EULER CỦA $ \sin z $

Với mọi số nguyên *lẻ* $ n = 2m + 1 $ và mọi số phức $ z $, công thức (2) của VI, p. 283, có thể viết thành

$$
\sin nz = (-1)^m 2^{n-1} \prod_{k=-m}^{m} \sin \left( z - \frac{k\pi}{n} \right)
$$
$$
= (-1)^m 2^{n-1} \sin z \prod_{k=1}^{m} \sin \left( z - \frac{k\pi}{n} \right) \sin \left( z + \frac{k\pi}{n} \right).
$$

Mặt khác, ta có $ \sin \left( z - \frac{k\pi}{n} \right) \sin \left( z + \frac{k\pi}{n} \right) = \sin^2 z - \sin^2 \frac{k\pi}{n} $, và, theo (3) (VI, 284), $ \prod_{k=1}^{m} \sin^2 \frac{k\pi}{n} = \frac{n}{2^{n-1}} $, do đó, khi thay thế $ z $ bởi $ z/n $,

$$
\sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} \left( 1 - \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}} \right).
$$

Ta có thể viết công thức này dưới dạng $ \sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} (1 - w_k(n, z)) $, với $ w_k(n, z) = 0 $ nếu $ k > m $ và $ w_k(n, z) = \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}} $ đối với $ 1 \leq k \leq m $. Ta sẽ thấy rằng với mọi $ z $ được chứa trong một tập con compắc $ K $ của $ \mathbf{C} $, và với $ n $ lẻ, chuỗi có số hạng tổng quát $ (n, z) $ là *hội tụ chuẩn tắc*. Thật vậy, khi $ n $ tiến tới $ +\infty $, $ n \sin \frac{z}{n} $ hội tụ đều trên $ K $, nên tồn tại một số $ M > 0 $ sao cho $ \left| n \sin \frac{z}{n} \right| \leq M $ với mọi số nguyên $ n $ và mọi $ z \in K $. Hơn nữa, trong chứng minh của đl. 1 của VI, p. 286, ta đã thấy rằng với $1 \leq k \leq m$ ta có $n \sin \frac{k \pi}{n} \geq \frac{k \pi}{2}$; do đó với mọi số nguyên $k$ sao cho $k \pi / 2 \geq M$ ta có $|w_k(n, z)| \leq 4M^2 / k^2 \pi^2$, điều này chứng minh mệnh đề của ta. Vì, với mọi $k$ cố định, $w_k(n, z)$ tiến tới (đều trên K) $z^2 / k^2 \pi^2$ khi $n$ tiến tới $+\infty$, ta thấy rằng:

#### Định lý 2 {#fvr-vi-s2-thm-2 .statement}

Với mọi số phức $z$ ta có

$$
\sin z = z \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2 \pi^2} \right)
$$

tích vô hạn ở vế phải hội tụ tuyệt đối và đều trên mọi tập con compắc của $\mathbf{C}$ (khai triển Euler của $\sin z$).

### 3. ỨNG DỤNG CHO CÁC SỐ BERNOULLI

Định lý 1 của VI, p. 286, cho thấy rằng, với $0 \leq x < \pi$, chuỗi có số hạng tổng quát

$$
\frac{2x}{n^2 \pi^2 - x^2} \geq 0
$$

là hội tụ. Mặt khác, ta có thể viết, với mọi số phức $z$ sao cho $|z| < \pi$,

$$
\frac{2z}{n^2 \pi^2 - z^2} = \frac{2z}{n^2 \pi^2} \sum_{k=0}^{\infty} \frac{z^{2k}}{n^{2k} \pi^{2k}}
$$

chuỗi ở vế phải hội tụ tuyệt đối. Từ đó ta sẽ suy ra rằng chuỗi "kép"

$$
\sum_{n=1}^{\infty} \sum_{k=1}^{\infty} \frac{-2z^{2k-1}}{n^{2k} \pi^{2k}}
$$

hội tụ tuyệt đối trong đĩa mở $|z| < \pi$, hội tụ chuẩn trên mọi tập compact được chứa trong đĩa này, và có tổng bằng $\cot z - \frac{1}{z}$. Thật vậy, với $|z| \leq a < \pi$ giá trị tuyệt đối của số hạng tổng quát của (11) nhiều nhất bằng $2a^{2k-1} / n^{2k} \pi^{2k}$, và tổng của bất kỳ số hữu hạn nào các số hạng $2a^{2k-1} / n^{2k} \pi^{2k}$ đều nhỏ hơn số hữu hạn $\sum_{n=1}^{\infty} \frac{2a}{n^2 \pi^2 - a^2}$; lấy tổng trước theo $k$, rồi theo $n$, ta thấy rằng tổng của chuỗi (11) bằng $\sum_{n=1}^{\infty} \frac{2z}{z^2 - n^2 \pi^2}$, điều đó chứng minh mệnh đề của chúng ta.

Bây giờ nếu ta lấy tổng chuỗi (11) trước theo $n$ rồi theo $k$ thì thu được đẳng thức (với $|z| < \pi$)

$$
\cot z - \frac{1}{z} = -2 \sum_{k=1}^{\infty} \frac{S_{2k}}{\pi^{2k}} z^{2k-1}
$$

trong đó ta đặt $S_k = \sum_{n=1}^{\infty} \frac{1}{n^k}$. Theo (1) (VI, p. 283) do đó ta có, với $|z| < 2\pi$ từ đó ta thu được công thức

$$
b_{2n} = (-1)^{n-1} (2n)! \frac{2 S_{2n}}{(2\pi)^{2n}} \quad \text{với } n \geq 1,
$$

một công thức đặc biệt cho thấy rằng các số $ S_{2n}/\pi^{2n} $ là *hữu tỉ*. Rõ ràng $ S_{k+1} \leq S_k $ nên, với mọi số nguyên $ k \geq 2 $, ta có $ S_k \leq S_2 = \pi^2/6 \leq 2 $; từ (14) suy ra các bất đẳng thức sau đối với các số Bernoulli

$$
\frac{2 (2n)!}{(2\pi)^{2n}} \leq |b_{2n}| \leq 4 \frac{(2n)!}{(2\pi)^{2n}} \quad \text{với } n \geq 1.
$$

Từ các bất đẳng thức này người ta có thể suy ra một ước lượng đối với đa thức Bernoulli

$$
B_n(x) = \sum_{k=0}^n \binom{n}{k} b_k x^{n-k}; \text{ đặc biệt, với } 0 \leq x \leq 1 \text{ ta có}
$$

$$
|B_n(x)| \leq 4 \sum_{k=0}^n \binom{n}{k} \frac{k!}{(2\pi)^k} = 4 \frac{n!}{(2\pi)^n} \sum_{k=0}^n \frac{(2\pi)^k}{k!} \leq 4 e^{2\pi} \frac{n!}{(2\pi)^n}.
$$

### Bài tập {#fvr-vi-s2-exercises}

Thiết lập các công thức

$$
\tan z = \sum_{n=1}^{\infty} (-1)^{n-1} 2^{2n} (2^{2n} - 1) b_{2n} \frac{z^{2n-1}}{(2n)!}
$$

$$
\frac{1}{\sin z} = \frac{1}{z} + \sum_{n=1}^{\infty} (-1)^{n-1} 2 (2^{2n-1} - 1) b_{2n} \frac{z^{2n-1}}{(2n)!}
$$

ở đây các chuỗi ở các vế phải hội tụ tuyệt đối, chuỗi thứ nhất với $ |z| < \frac{\pi}{2} $ và chuỗi thứ hai với $ |z| < \pi $ (biểu thị $ \tan z $ và $ 1/\sin 2z $ dưới dạng các tổ hợp tuyến tính của $ \cot z $ và $ \cot 2z $). Suy ra rằng các số $ \frac{2^{2n}(2^{2n} - 1)}{2n} b_{2n} $ là các số nguyên. (Dùng bổ đề sau: trong hai chuỗi hội tụ tuyệt đối $ \sum_{n=0}^{\infty} \alpha_n \frac{z^n}{n!} $, $ \sum_{n=0}^{\infty} \beta_n \frac{z^n}{n!} $ các hệ số $ \alpha_n $ và $ \beta_n $ là các số nguyên, thì, trong tích của chúng viết dưới dạng $ \sum_{n=0}^{\infty} \gamma_n \frac{z^n}{n!} $, các $ \gamma_n $ là các số nguyên.)

Chứng minh công thức

$$
(n-1)B_n(X) = n(X-1)B_{n-1}(X) - \sum_{k=0}^{n} \binom{n}{k} b_k B_{n-k}(X)
$$

lấy đạo hàm chuỗi $ S e^{SX}/(e^S - 1) $ theo S). Suy ra công thức

$$
(2n+1)b_{2n} = - \sum_{k=1}^{n-1} \binom{2n}{2k} b_{2k} b_{2n-2k}
$$

đối với các số Bernoulli.

Hãy chứng minh rằng, với mọi số nguyên $ p > 1 $,

$$
B_n \left( \frac{x}{p} \right) + B_n \left( \frac{x+1}{p} \right) + \cdots + B_n \left( \frac{x+p-1}{p} \right) = \frac{1}{p^{n-1}} B_n(X).
$$

4) a) Chứng minh hệ thức
$$
B_n(1 - X) = (-1)^n B_n(X)
$$
(dùng việc $ b_{2n-1} = 0 $ với $ n > 1 $, và hệ thức
$$
B_n(1 - X) - B_n(-X) = (-1)^n n X^{n-1}.
$$)

b) Hãy chứng minh rằng
$$
B_n \left( \frac{1}{2} \right) = b_n \left( \frac{1}{2^n} - 1 \right)
$$
(dùng bài tập 3).

c) Chứng minh rằng, với $ n $ chẵn, $ B_n(X) $ có hai nghiệm trong khoảng $[0, 1]$ của $ \mathbf{R} $, và rằng với $ n $ lẻ $ > 1 $, $ B_n(X) $ có một nghiệm đơn tại các điểm $ 0, \frac{1}{2} $ và $ 1 $ và không triệt tiêu tại điểm nào khác của $[0, 1]$ (dùng $ b $) và quan hệ $ B'_n = n \tilde{B}_{n-1} $).

d) Suy ra từ c) rằng, với $ n $ chẵn, giá trị lớn nhất của $ |B_n(x)| $ trên khoảng $[0, 1]$ là $ |b_n| $, và với $ n $ lẻ, nếu $ a_n $ là giá trị lớn nhất của $ |B_n(x)| $ trên $[0, 1]$, thì
$$
\frac{4}{n+1} |b_{n+1}| \left( 1 - \frac{1}{2^n} \right) \leq a_n \leq \frac{1}{2} n |b_{n-1}|
$$
(dùng định lý giá trị trung bình).

5) Nếu đặt $ S_n(x) = \frac{1}{n+1} (B_{n-1}(x) - B_{n+1}(0)) $ thì, với mọi số nguyên $ a > 0 $, ta có
$$
S_n(a) = 1^n + 2^n + \cdots + (a-1)^n.
$$

a) Chứng minh rằng với mọi số nguyên $ n \geq 0 $ và mọi số nguyên $ a > 0 $ ta có $ 2 S_{2n+1}(a) \equiv 0 $ (mod. $ a $) (xét tổng $ k^{2n+1} + (a-k)^{2n+1} $).

b) Nếu $ r $ và $ s $ là hai số nguyên bất kỳ, hãy chứng minh rằng
$$
S_n(rs) \equiv s S_n(r) + n r S_{n-1}(r) S_1(s) \pmod{r^2}.
$$

c) Cho $ p $ là một số nguyên tố. Chứng tỏ rằng nếu $ n $ chia hết cho $ p-1 $ thì ta có $ S_n(p) \equiv -1 $ (mod. $ p $), và nếu $ n $ không chia hết cho $ p-1 $ thì $ S_n(p) \equiv 0 $ (mod. $ p $) (nếu $ p $ không chia hết số nguyên $ g $ thì nhận xét rằng $ S_n(p) \equiv g^n S_n(p) $ (mod. $ p $)).

6) a) Các số hữu tỉ $ b_n $ đã được xác định bởi công thức (20) của VI, p. 275, người ta ký hiệu bởi $ d_n $ mẫu số $ > 0 $ của $ b_n $ khi viết thành một phân số bất khả quy. Hãy chỉ ra rằng không có nhân tử nguyên tố nào của $ d_n $ có thể $ > n+1 $ (dùng công thức quy nạp (23) của VI, p. 276)

b) Hãy chỉ ra rằng với mọi số nguyên $ p > 0 $ và mọi số nguyên $ n > 0 $
$$
S_n(p) = b_n p + \binom{n}{1} \frac{p}{2} b_{n-1} p + \cdots + \binom{n}{r} \frac{p'}{r+1} b_{n-r} p + \cdots + \frac{p^{n+1}}{n+1}.
$$

c) Suy ra từ b) bằng đệ quy theo $ n $ rằng, với mọi số nguyên tố $ p $ mẫu số của $ S_n(p) - b_n p $ khi viết thành một phân số bất khả quy, không chia hết cho $ p $ (chú ý rằng $ p' $ không thể chia hết cho $ r+1 $).

Suy ra từ c) rằng số

$$
b_n - \sum_p \frac{S_n(p)}{p}
$$

trong đó $ p $ chạy qua tập hợp các số nguyên tố $ p \leq n + 1 $ và $ n $ là chẵn, là một số nguyên. Suy ra rằng

$$
b_{2n} + \sum_p \frac{1}{p}
$$

trong đó $ p $ chạy qua tập hợp các số nguyên tố sao cho $ p - 1 $ chia hết $ 2n $, là một số nguyên (định lý Eisenstein-von Staudt; dùng bài tập 5 c).

Ta thừa nhận rằng với mọi số nguyên $ a > 0 $ có vô hạn số nguyên tố trong tập hợp các số nguyên $ 1 + ma $ ($ m $ chạy qua tập hợp các số nguyên $ \geq 1 $; đây là một trường hợp riêng của định lý Dirichlet về các cấp số cộng).

Cho $ n $ là một số nguyên $ \geq 1 $, và cho $ s \geq 1 $ là một số nguyên sao cho $ q = 1 + (2n + 1)!s $ là nguyên tố; hãy chỉ ra rằng nếu $ p $ là một số nguyên tố sao cho $ p - 1 $ chia hết $ 2nq $ thì $ p - 1 $ phải chia hết $ 2n $ (trong trường hợp đối người ta sẽ có $ p - 1 = qd $ với $ d $ là một số nguyên, và $ p $ sẽ chia hết cho $ d + 1 $).

Suy ra từ a) rằng với mọi số nguyên $ n > 0 $ đều tồn tại vô hạn số nguyên $ m > n $ sao cho $ b_{2m} - b_{2n} $ là một số nguyên.*

Hãy chỉ ra rằng, với mọi số nguyên tố $ p > 3 $, $ S_{2n}(p^k) - p^k b_{2n} $, khi viết dưới dạng một phân số bất khả quy, có tử số chia được cho $ p^{2k} $ (lập luận như trong bài tập 6).

Nói rằng một số hữu tỉ $ r $ là một số nguyên $ p $-adic (\emph{Gen. Top.}, III, p. 322, bài tập

Xem [các bài tập cho § 2](exercises/s2/).
