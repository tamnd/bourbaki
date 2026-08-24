---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 3
section_title: BOUNDS FOR THE REMAINDER IN THE EULER-MACLAURIN SUMMATION FORMULA
lang: vi
source: fvr-i-vii
pdf_pages: 0303-0305, 0311-0312
extraction: ocr
subsections:
    - "no": 1
      title: BOUNDS FOR THE REMAINDER IN THE EULER-MACLAURIN SUMMATION FORMULA
      page: 0
      pdf_page: 303
    - "no": 2
      title: APPLICATION TO ASYMPTOTIC EXPANSIONS
      page: 0
      pdf_page: 304
statements: 0
exercises: 3
content_sha256: 42932e06e15d96f6dfb654d10ddeae8f055b77294ad52303e9e0d39bffb3ae2b
translated_from: content/en/fvr/VI/03_s3_bounds_for_the_remainder_in_the_euler.md
source_content_sha256: 103ec5ec6513283f6c6e9909a63a827d7480ecb776856e9ab7fb3eb96b37fc76
translation_model: gpt-5.4
translation_run: translate-vi-46a3c5b4
glossary_version: 34
glossary_terms_sha256: 45547f5d059046b844365c0649be04c8614e632c609588fdc41f3b3eac6c09bf
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CHẶN CHO PHẦN DƯ TRONG CÔNG THỨC CỘNG EULER-MACLAURIN

### 1. CHẶN CHO PHẦN DƯ TRONG CÔNG THỨC CỘNG EULER-MACLAURIN

Ước lượng thu được ở (16) cho các đa thức Bernoulli trên khoảng $[0, 1]$ cho phép ta ước lượng dễ dàng phần dư $ T_p(x, n) $ trong công thức cộng Euler-Maclaurin (VI, p. 282, công thức (39)):

$$
\left\{
\begin{array}{l}
f(x) + f(x+1) + \cdots + f(x+n) \\
\phantom{=} = \int_x^{x+n+1} f(t)\,dt - \frac{1}{2} (f(x+n+1) - f(x)) \\
\phantom{=} \phantom{=} + \sum_{k=1}^p \frac{b_{2k}}{(2k)!} (f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x)) + T_p(x, n).
\end{array}
\right.
$$

Thật vậy, ta có (VI, p. 283, công thức (41))

$$
T_p(x, n) = -\frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1-s) f^{(2p+1)}(x+s)\,ds
$$

trong đó $ \overline{B}_{2p+1}(t) $ là hàm tuần hoàn chu kỳ 1, bằng $ B_{2p+1}(t) $ trên khoảng $[0, 1[$. Công thức (16) của VI, p. 288, cho thấy rằng

$$
|\overline{B}_{2p+1}(t)| \leq 4e^{2\pi} \frac{(2p+1)!}{(2\pi)^{2p+1}}
$$
(3)

với mọi $ t \in \mathbf{R} $, và áp dụng công thức giá trị trung bình ta được ước lượng

$$
|T_p(x, n)| \leq \frac{4e^{2\pi}}{(2\pi)^{2p+1}} \int_x^{x+n+1} |f^{(2p+1)}(t)| \, dt
$$
(4)

cho $ T_p(x, n) $.

### 2. ÁP DỤNG CHO CÁC KHAI TRIỂN TIỆM CẬN

Công thức Euler-Maclaurin cho phép đưa ra một lời giải đầy đủ hơn (trong những trường hợp quan trọng nhất) cho bài toán được xét trong V, p. 238 đến 242, tức là bài toán tìm một khai triển tiệm cận của tổng riêng phần $ s_n = \sum_{m=0}^n g(m) $ (tương ứng, của số dư $ r_n = \sum_{m=n+1}^\infty g(m) $), trong đó $ g $ là một hàm vô hướng, $ > 0 $, đơn điệu, xác định trên $ [0, +\infty[ $.

Chúng tôi sẽ tự giới hạn vào trường hợp $ g $ là một hàm (H) (V, p. 252), cấp 0 đối với $ e^x $; nói cách khác, ta có quan hệ $ g' \ll g $; từ quan hệ này suy ra $ g^{(k+1)} \ll g^{(k)} $ với mọi số nguyên $ k > 0 $ sao cho không có đạo hàm nào $ g^{(h)} $ cấp $ h \leq k $ tương đương với một hằng (V, p. 232, mệnh đề 7). Cho $ p $ là một số nguyên sao cho không có đạo hàm nào $ g^{(h)} $ cấp $ h \leq 2p $ tương đương với một hằng. Trước hết giả sử rằng chuỗi có số hạng tổng quát $ g(n) $ có tổng vô hạn, và phân biệt nhiều trường hợp:

1. $ |g^{(2p-1)}(n)| $ tends to $ +\infty $ with $ n $; we have the same, by the hypothesis, for $ |g^{(2k-1)}(n)| $ for $ 1 \leq k \leq p $; further, since $ g^{(2p+1)} $ is monotone on a neighbourhood of $ +\infty $, the formula (4) of VI, p. 289, gives $ T_p(0, n) = O(g^{(2p)}(n+1)) = o(g^{(2p-1)}(n+1)) $; the Euler-Maclaurin formula, applied for $ x = 0 $, shows that

$$
s_n = \sum_{m=0}^n g(m) = \int_0^{n+1} g(t) \, dt - \frac{1}{2} g(n+1)
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} g^{(2k-1)}(n+1) + o(g^{(2p-1)}(n+1))
$$

mỗi hạng của tổng này đều là không đáng kể so với hạng đứng trước; khi khai triển từng hạng của chúng theo một thang so sánh $ \mathcal{E} $ thì khi đó ta sẽ có một khai triển tiệm cận của $ s_n $.

2' Bây giờ giả sử rằng với một chỉ số $ q $ sao cho $ 1 \leq q \leq p $ ta có $ |g^{(2q-1)}(n)| $ tiến tới $ +\infty $ khi $ n $ tăng, nhưng $ g^{(2k-1)}(n) $ tiến tới 0 đối với $ k > q $. Vì $ g^{(2p+1)} $ là đơn điệu trên một lân cận của $ +\infty $ nên tích phân $ \int_0^\infty |g^{(2p+1)}(u)| \, du $ hội tụ, và khi đó có thể viết

= $ \sum_{m=0}^{n} g(m) = \int_0^{n+1} g(t)\,dt - \frac{1}{2}g(n+1) + \sum_{k=1}^{q} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + C $
$$
+ \sum_{k=q+1}^{p} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + o\left(g^{(2p-1)}(n+1)\right)
$$
C là một hằng: thật vậy
$$
\int_{n+1}^{\infty} |g^{(2p+1)}(u)|\,du = O\left(g^{(2p)}(n+1)\right) = o\left(g^{(2p-1)}(n+1)\right).
$$
Công thức tương tự vẫn đúng khi chính $ g(n) $ tiến tới 0. Cuối cùng, khi số hạng tổng quát $ g(n) $ của chuỗi hội tụ, ta có, đối với số dư $ r_n = \sum_{m=n+1}^{\infty} g(m) $, khai triển
$$
= \sum_{m=n+1}^{\infty} g(m) = \int_{n+1}^{\infty} g(t)\,dt + \frac{1}{2}\,g(n+1)
$$
$$
- \sum_{k=1}^{p} \frac{b_{2k}}{(2k)!}\,g^{(2k-1)}(n+1) + o\left(g^{(2p-1)}(n+1)\right).
$$

### Bài tập {#fvr-vi-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
