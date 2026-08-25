---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 7
section_title: Infinite sums and products of real numbers
lang: vi
source: top-i-iv
pdf_pages: 0369-0378, 0403-0407
extraction: ocr
subsections:
    - "no": 1
      title: FAMILIES OF POSITIVE FINITE NUMBERS SUMMABLE IN $\mathbf{R}$
      page: 0
      pdf_page: 370
    - "no": 2
      title: FAMILIES OF FINITE NUMBERS OF ARBITRARY SIGN SUMMABLE IN $\mathbf{R}$
      page: 0
      pdf_page: 372
    - "no": 3
      title: PRODUCT OF TWO INFINITE SUMS
      page: 0
      pdf_page: 373
    - "no": 4
      title: FAMILIES MULTIPLIABLE IN $\mathbf{R}^*$
      page: 0
      pdf_page: 373
    - "no": 5
      title: SUMMABLE FAMILIES AND MULTIPLIABLE FAMILIES IN $\overline{\mathbf{R}}$
      page: 0
      pdf_page: 375
    - "no": 6
      title: INFINITE SERIES AND INFINITE PRODUCTS OF REAL NUMBERS
      page: 0
      pdf_page: 376
statements: 20
exercises: 22
content_sha256: d03aa8ee0c2eccf74d6bb7652e3961dde8faf9d4ec008cbb5f917bd4b1510dfc
translated_from: content/en/top/IV/07_s7_infinite_sums_and_products_of_real.md
source_content_sha256: 53fa6856b0ed9b2e76f1e361c0d82aa4411cc7ecfa0b354e495808655f7944b3
translation_model: gpt-5.4
translation_run: translate-vi-e536aaea
glossary_version: 34
glossary_terms_sha256: cbb5cbaf477cfc082a976afe7cc41b6ce6c667a2c5d45160eba9db048177c1a6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 7. TỔNG VÀ TÍCH VÔ HẠN CỦA CÁC SỐ THỰC

Vì mọi điểm của $\mathbf{R}$ đều có một hệ cơ bản lân cận *đếm được* (§ 1, no. 4, Hệ quả của Mệnh đề 3), suy ra rằng một họ $(x_t)$ các số thực *hữu hạn* chỉ là khả tổng trong $\mathbf{R}$ nếu tập hợp các chỉ số t sao cho $x_t \neq 0$ là *đếm được* (Chương III, § 5, no. 2, Hệ quả của Mệnh đề 1). Do đó việc nghiên cứu các họ khả tổng trong $\mathbf{R}$ về cơ bản được quy về việc nghiên cứu các *dãy* khả tổng. Tuy nhiên, về sau chúng ta sẽ phải xét các họ không đếm được $(x_t)$ các số thực hữu hạn, mà các số hạng là các hàm của một tham số $t$; có thể xảy ra là họ này khả tổng với mọi $t$, nhưng tập hợp (đếm được) các chỉ số $i$ sao cho $x_i \neq 0$ lại phụ thuộc vào $t$. Vì lý do đó, trong phần sau chúng ta sẽ không đặt giả thiết nào về lũy thừa của tập hợp chỉ số.

### 1. CÁC HỌ SỐ HỮU HẠN DƯƠNG KHẢ TỔNG TRONG $\mathbf{R}$

#### Định lý 1 {#top-iv-s7-thm-1 .statement}

*Một họ* $(x_i)$ *các số thực hữu hạn* $\geqslant 0$ *là khả tổng trong* $\mathbf{R}$ *khi và chỉ khi tập hợp các tổng riêng phần hữu hạn của họ bị chặn trên trong* $\mathbf{R}$. *Khi đó, cận trên bé nhất của tập hợp này là tổng của họ* $(x_i)$.

Với mỗi tập con hữu hạn $H$ của tập chỉ số $I$, đặt $s_H = \sum_{i \in H} x_i$; vì các $x_i$ đều $\geqslant 0$, quan hệ $H \subset H'$ kéo theo $s_H \leqslant s_{H'}$. Nói cách khác, ánh xạ $H \to s_H$ là một hàm *tăng* trên tập có hướng $\mathfrak{F}(I)$ các tập con hữu hạn của $I$; do đó (\$ 5, no. 2, Hệ quả của Định lý 2) nó có một giới hạn hữu hạn khi và chỉ khi nó *bị chặn trên*.

#### Nhận xét {#top-iv-s7-n1-rem-1 .statement}

Cho $(H_\lambda)$ là một họ các tập con hữu hạn của $I$ sao cho, với mỗi tập con hữu hạn $H$ của $I$, tồn tại một chỉ số $\lambda$ sao cho $H \subset H_\lambda$; khi đó $(x_i)$ là khả tổng nếu và chỉ nếu họ các $s_{H_\lambda}$ bị *chặn trên* trong $\mathbf{R}$. Đặc biệt, cho $(x_n)$ là một dãy các số thực hữu hạn $\geqslant 0$, và với mỗi số nguyên $n$ đặt $s_n = \sum_{p=0}^n x_p$; khi đó dãy $(x_n)$ là khả tổng trong $\mathbf{R}$ nếu và chỉ nếu, đối với *một dãy* các số nguyên tăng ngặt $(n_k)$, dãy bộ phận $(s_{n_k})$ bị *chặn trên* trong $\mathbf{R}$.

*Ví dụ.* 1) Với mỗi số $q$ sao cho $0 \leqslant q < 1$, dãy $(q^n)$ ("cấp số nhân có công bội $q$") là khả tổng trong $\mathbf{R}$, vì
$$
s_n = \frac{1 - q^{n+1}}{1 - q} \leqslant \frac{1}{1 - q}
$$
tổng của dãy này là $\lim_{n \to \infty} s_n = \frac{1}{1 - q}$.

2) Cho $a$ và $b$ là hai số sao cho $0 \leqslant a < 1$ và $0 \leqslant b < 1$; khi đó họ $(a^m b^n)_{(m, n) \in \mathbf{N} \times \mathbf{N}}$ là cộng được trong $\mathbf{R}$. Thật vậy, mỗi tập con hữu hạn của $\mathbf{N} \times \mathbf{N}$ được chứa trong một tập con dạng $[0, p] \times [0, p]$, và ta có
$$
\sum_{m=0}^p \sum_{n=0}^p a^m b^n = \left( \sum_{m=0}^p a^m \right) \left( \sum_{n=0}^p b^n \right) = \frac{1 - a^{p+1}}{1 - a} \cdot \frac{1 - b^{p+1}}{1 - b} \leqslant \frac{1}{(1 - a)(1 - b)}.
$$

3) Với mỗi số nguyên $p > 1$, dãy $(n^{-p})$ ($n > 0$) là cộng được, vì
$$
s_{2^n + 1} - s_{2^n} = \sum_{k=1}^{2^n} (2^n + k)^{-p} < 2^n \cdot (2^n)^{-p}
$$
và do đó, bằng cách cộng các bất đẳng thức này,
$$
s_{2^n} < \frac{1}{1 - 2^{1-p}}.
$$

4) Dãy $(1/n)$ ($n > 0$) không khả tổng trong $\mathbf{R}$, vì
$$
s_{2^{n+1}} - s_{2^n} = \sum_{k=1}^{2^n} \frac{1}{2^n + k} > \frac{2^n}{2^{n+1}} = \frac{1}{2}
$$
và do đó, cộng các bất đẳng thức này lại với nhau,
$$
s_{2^n} > n/2
$$
nên tiêu chuẩn của Định lý 1 không được thỏa mãn.

5) Cho $(I_n)$ là một dãy các khoảng mở không rỗng đôi một rời nhau, tất cả đều được chứa trong một khoảng có độ dài hữu hạn $l$. Tổng các độ dài của một số hữu hạn khoảng thuộc họ này là $\leq l$ ($\S 1$, no. 5) và do đó họ các độ dài của các $I_n$ là khả tổng trong $\mathbf{R}$, và tổng của nó là $\leq l$.

#### Định lý 2 (Nguyên lý so sánh) {#top-iv-s7-thm-2 .statement}

*Cho* $(x_i)_{i \in I}$ *và* $(y_i)_{i \in I}$ *là hai họ các số thực hữu hạn* $\geq 0$, *sao cho* $x_i \leq y_i$ *với mọi* $i$. *Nếu* $(y_i)$ *là khả tổng trong* $\mathbf{R}$ *thì* $(x_i)$ *cũng vậy, và ta có* $\sum_i x_i \leq \sum_i y_i$; *nếu thêm nữa tồn tại một chỉ số* $x$ *sao cho* $x_x < y_x$, *thì* $\sum_i x_i < \sum_i y_i$.

Giả thiết suy ra rằng,
$$
\sum_{i \in H} x_i \leq \sum_{i \in H} y_i,
$$
với mọi tập con hữu hạn $H$ của $I$, và phần thứ nhất của định lý được suy ra từ điều này; bất đẳng thức liên hệ các tổng được suy ra từ nguyên lý mở rộng các bất đẳng thức ($\S 5$, no. 2, Định lý 1). Nếu $x_x < y_x$, thì
$$
\sum_i x_i = x_x + \sum_{i \neq x} x_i < y_x + \sum_{i \neq x} y_i = \sum_i y_i.
$$

Định lý này cung cấp tiêu chuẩn được dùng thông dụng nhất để quyết định một dãy $(x_n)$ các số thực $\geq 0$ có tổng được trong $\mathbf{R}$ hay không: ta cố *so sánh* dãy đã cho với một dãy đơn giản hơn $(y_n)$ mà ta đã biết nó có tổng được hay không. Nếu tồn tại một số hữu hạn $a > 0$ sao cho $x_n \leq a y_n$ với mọi $n$ kể từ một điểm nào đó trở đi, và nếu $(y_n)$ có tổng được, thì $(x_n)$ có tổng được; còn nếu tồn tại một số hữu hạn $b > 0$ sao cho $x_n \geq b y_n$ với mọi $n$ kể từ một điểm nào đó trở đi, và nếu $(y_n)$ không có tổng trong $\mathbf{R}$, thì $(x_n)$ không có tổng trong $\mathbf{R}$. Ta sẽ thấy trong một tập sau cách thu được những dãy so sánh như thế trong các trường hợp xuất hiện thường gặp nhất.

#### Ví dụ 1 {#top-iv-s7-n1-exa-1 .statement}

Cho $a$ là một số thực hữu hạn $> 0$, và xét dãy $\left( \frac{a^n}{n!} \right)$; gọi $n_0$ là số nguyên nhỏ nhất sao cho $a < n_0$. Khi đó với mỗi $n \geq n_0$ ta có
$$
\frac{a^n}{n!} \leq \frac{a^{n_0}}{n_0!} \cdot \left( \frac{a}{n_0} \right)^{n-n_0};
$$
vì $q = \frac{a}{n_0} < 1$, dãy $(q^{n-n_0})$ là hội tụ tuyệt đối, và do đó dãy $\left( \frac{a^n}{n!} \right)$ cũng vậy.

#### Ví dụ 2 {#top-iv-s7-n1-exa-2 .statement}

Cho $(a_n)$ là một dãy khả tổng gồm các số dương. Vì
$$
\lim_{n \to \infty} a_n = 0,
$$
nên tồn tại một số nguyên $n_0$ sao cho $a_n \leq 1$ mỗi khi $n \geq n_0$. Do đó, với mỗi $n \geq n_0$ ta có $a_n^2 \leq a_n$, và vì thế dãy $(a_n^2)$ là khả tổng trong $\mathbf{R}$. Dãy $(a_n^p)$ cũng vậy với mỗi số nguyên $p > 1$.

#### Ví dụ 3 {#top-iv-s7-n1-exa-3 .statement}

Cho $a$ và $b$ là hai số $< 1$; khi đó
$$
\frac{1}{a^m + b^n} \leq \frac{1}{2(\sqrt{a})^m (\sqrt{b})^n}
$$
và do đó họ $\left( \frac{1}{a^m + b^n} \right)$ là khả tổng trong $\mathbf{R}$.

#### Hệ quả {#top-iv-s7-n1-cor-1 .statement}

*Cho* $(x_i)_{i \in I}$ *là một họ khả tổng các số hữu hạn* $\geq 0$ *trong* $\mathbf{R}$. *Nếu* $H$ *là một tập con tùy ý của* $I$, *ta có*
$$
\sum_{i \in H} x_i \leq \sum_{i \in I} x_i,
$$
*và đẳng thức chỉ đúng nếu* $x_i = 0$ *với mọi* $i \in \complement H$.

### 2. HỌ CÁC SỐ HỮU HẠN CÓ DẤU TÙY Ý KHẢ TỔNG TRONG $\mathbf{R}$

#### Định lý 3 {#top-iv-s7-thm-3 .statement}

*Cho* $(x_i)_{i \in I}$ *là một họ các số thực hữu hạn; khi đó các mệnh đề sau là tương đương*:

a) *Họ* $(x_i)$ *là khả tổng trong* $\mathbf{R}$.
b) *Họ* $(|x_i|)$ *là khả tổng trong* $\mathbf{R}$.
c) *Tập hợp các tổng riêng hữu hạn của họ* $(x_i)$ *bị chặn trong* $\mathbf{R}$.

Đặt $I_1$ *là tập hợp mọi* $i \in I$ *sao cho* $x_i \geq 0$, *và* $I_2$ *là tập hợp mọi* $i \in I$ *sao cho* $x_i < 0$. *Họ* $(x_i)_{i \in I}$ *[resp. $(|x_i|)_{i \in I}$] *là khả tổng khi và chỉ khi mỗi họ* $(x_i)_{i \in I_1}$ *và* $(x_i)_{i \in I_2}$ *[resp. $(|x_i|)_{i \in I_1}$ and $(|x_i|)_{i \in I_2}$] *đều khả tổng* (Chương III, § 5, no. 3, Mệnh đề 2 and 3). *Bây giờ, nói rằng* $(x_i)_{i \in I_1}$ *khả tổng, hay nói rằng* $(|x_i|)_{i \in I_1}$ *khả tổng, hay nói rằng tập hợp các tổng bộ phận hữu hạn của họ* $(x_i)_{i \in I_1}$ bị chặn (no. 1, Định lý 1), *thì cũng là một*; và điều tương tự cũng đúng khi thay $I_1$ bằng $I_2$. Định lý được suy ra ngay lập tức.

Định lý 3 cho thấy rằng tính khả tổng trong $\mathbf{R}$ của một họ các số thực hữu hạn chỉ phụ thuộc vào tính khả tổng của họ các giá trị tuyệt đối của chúng.

Nhắc lại (Chương III, § 5, no. 5, Mệnh đề 6) rằng nếu $(x_i)$ và $(y_i)$ là hai họ khả tổng của các số thực hữu hạn, thì họ $(x_i + y_i)$ là khả tổng và $\sum (x_i + y_i) = \sum x_i + \sum y_i$. Hơn nữa, nếu $(x_i)$ là một họ khả tổng của các số thực hữu hạn và $a$ là một số thực hữu hạn bất kỳ, thì họ $(ax_i)$ khả tổng trong $\mathbf{R}$, và ta có $\sum ax_i = a \cdot \sum x_i$.

### 3. TÍCH CỦA HAI TỔNG VÔ HẠN

#### Mệnh đề 1 {#top-iv-s7-prop-1 .statement}

*Nếu các họ* $(x_\lambda)_{\lambda \in L}$ *và* $(y_\mu)_{\mu \in M}$ *các số thực hữu hạn là khả tổng trong* $\mathbf{R}$, *thì họ* $(x_\lambda y_\mu)_{(\lambda, \mu) \in L \times M}$ *cũng vậy và ta có*

(1)
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = (\sum_{\lambda \in L} x_\lambda) (\sum_{\mu \in M} y_\mu).
$$

Mọi tập con hữu hạn của $L \times M$ đều được chứa trong một tập con hữu hạn dạng $H \times K$, trong đó $H$ là một tập con hữu hạn của $L$ và $K$ là một tập con hữu hạn của $M$. Theo giả thiết, tồn tại một số $a > 0$ sao cho $\sum_{\lambda \in H} |x_\lambda| \leq a$ và $\sum_{\mu \in K} |y_\mu| \leq a$ với mọi tập con hữu hạn $H$ và $K$ của $L$ và $M$ tương ứng; do đó
$$
\sum_{(\lambda, \mu) \in H \times K} |x_\lambda y_\mu| = (\sum_{\lambda \in H} |x_\lambda|) (\sum_{\mu \in K} |y_\mu|) \leq a^2,
$$
và điều này cho thấy họ $(x_\lambda y_\mu)$ là khả tổng trong $\mathbf{R}$, theo Định lý 1 và 3. Theo tính kết hợp, ta có thể viết [Chương III, § 5, no. 3, công thức (2)]
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = \sum_{\lambda \in L} (\sum_{\mu \in M} x_\lambda y_\mu) = \sum_{\lambda \in L} x_\lambda (\sum_{\mu \in M} y_\mu) = (\sum_{\lambda \in L} x_\lambda) (\sum_{\mu \in M} y_\mu);
$$
do đó có kết quả phải chứng minh.

### 4. CÁC HỌ NHÂN ĐƯỢC TRONG $\mathbf{R}^*$

Trong nhóm nhân $\mathbf{R}^*$ của các số thực khác không hữu hạn, một họ $(x_i)_{i \in I}$ chỉ có thể khả nhân nếu $\lim x_i = 1$ đối với bộ lọc các phần bù của các tập con hữu hạn của $I$ (Chương III, § 5, no. 2, Mệnh đề 1). Đặc biệt chỉ có thể có một số *hữu hạn* chỉ số $i$ sao cho $x_i < 0$. Vì vậy ta có thể chỉ cần xét các họ $x_i$ mà mọi số hạng đều dương ngặt; khi đó thuận tiện là đặt $x_i = 1 + u_i$, trong đó các $u_i$ thỏa mãn các bất đẳng thức $-1 < u_i < +\infty$ với mọi $i$. Vì mỗi điểm của $\mathbf{R}^*$ có một hệ cơ bản đếm được các lân cận, tập hợp các chỉ số $i$ sao cho $u_i \neq 0$ là đếm được, nếu họ $(1 + u_i)$ là khả nhân trong $\mathbf{R}^*$.

#### Định lý 4 {#top-iv-s7-thm-4 .statement}

*Họ* $(1 + u_i)$ *là khả nhân trong* $\mathbf{R}^*$ *khi và chỉ khi họ* $(u_i)$ *là khả tổng trong* $\mathbf{R}$.
**Bổ đề.** (i) *Nếu* $(a_i)_{1 \leq i \leq p}$ *là một dãy hữu hạn các số* $> 0$, *thì*
$$
\prod_{i=1}^p (1 + a_i) \geq 1 + \sum_{i=1}^p a_i.
$$
(ii) *Nếu thêm nữa* $a_i < 1$ *với mọi* $i$, *thì*
$$
\prod_{i=1}^p (1 - a_i) \geq 1 - \sum_{i=1}^p a_i.
$$

Các bất đẳng thức này là hiển nhiên nếu $p = 1$, và được chứng minh bằng quy nạp theo $p$. Nếu
$$
\prod_{i=1}^{p-1} (1 + a_i) \geq 1 + \sum_{i=1}^{p-1} a_i,
$$
ta có
$$
\prod_{i=1}^p (1 + a_i) \geq (1 + a_p) \left( 1 + \sum_{i=1}^{p-1} a_i \right) = 1 + \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 + \sum_{i=1}^p a_i.
$$
Tương tự, nếu
$$
\prod_{i=1}^{p-1} (1 - a_i) \geq 1 - \sum_{i=1}^{p-1} a_i,
$$
ta có
$$
\prod_{i=1}^p (1 - a_i) \geq (1 - a_p) \left( 1 - \sum_{i=1}^{p-1} a_i \right) = 1 - \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 - \sum_{i=1}^p a_i.
$$

Sau khi đã chứng minh bổ đề, ta nhận thấy rằng nếu họ $(1 + u_i)$ là khả nhân thì các họ $(1 + u_i^+)$ và $(1 - u_i^-)$ cũng vậy, vì $\mathbf{R}^*$ là một nhóm đầy đủ (Chương III, § 5, no. 3, Mệnh đề 2); và ngược lại, nếu các họ $(1 + u_i^+)$ và $(1 - u_i^-)$ là khả nhân, thì $(1 + u_i)$ cũng vậy (Chương III, § 5, no. 3, Mệnh đề 3). Do đó ta chỉ cần xét các trường hợp trong đó mọi $u_i$ đều $\geq 0$ và trong đó chúng đều $\geq 0$.

Trước hết giả sử rằng $u_i \geq 0$ với mọi $i$. Nếu họ $(1 + u_i)$ là khả nhân được, thì với mỗi $\varepsilon > 0$ tồn tại một tập con hữu hạn $J$ của tập chỉ số trong $I$ sao cho, với mỗi tập con hữu hạn $H$ của $I$ rời nhau với $J$, ta có $1 \leq \prod_{i \in H} (1 + u_i) \leq 1 + \varepsilon$; theo (2) suy ra rằng $\sum_{i \in H} u_i \leq \varepsilon$, điều này cho thấy rằng $(u_i)$ là khả tổng trong $\mathbf{R}$ theo tiêu chuẩn Cauchy (Chương III, § 5, no. 2, Định lý 1).

Ngược lại, giả sử rằng $(u_i)$ là khả tổng trong $\mathbf{R}$. Với mỗi $\varepsilon$ sao cho $0 < \varepsilon < 1$, tồn tại một tập con hữu hạn $J$ của $I$ sao cho, với mỗi tập con hữu hạn $H$ của $I$ rời nhau với $J$, ta có $0 \leq \sum_{i \in H} u_i \leq \varepsilon$. Do (3), vì thế ta có $\prod_{i \in H} (1 - u_i) \geq 1 - \varepsilon$; nhưng vì $1 + u \leq \frac{1}{1 - u}$ với mọi số $u$ sao cho $0 \leq u < 1$, suy ra rằng

$$
1 \leq \prod_{i \in H} (1 + u_i) \leq \frac{1}{1 - \varepsilon},
$$

và điều này cho thấy rằng $(1 + u_i)$ là khả nhân được (tiêu chuẩn Cauchy).

Chứng minh là tương tự khi tất cả các $u_i$ đều $\leq 0$. Để chứng tỏ rằng $(u_i)$ là khả tổng nếu $(1 + u_i)$ là khả nhân được, dùng công thức (2) và bất đẳng thức $1 - u \leq \frac{1}{1 + u}$ ($0 \leq u < 1$); để chứng tỏ rằng $(1 + u_i)$ là khả nhân được nếu $(u_i)$ là khả tổng, dùng công thức (3).

Trong Chương V (§ 4), việc nghiên cứu tôpô của nhóm $\mathbf{R}^*$ sẽ cho phép ta đưa ra một tiêu chuẩn khác cho tính khả nhân được của một họ trong $\mathbf{R}^*$ với sự trợ giúp của hàm lôgarit; trong một tập sau, chúng tôi sẽ thiết lập tính tương đương của tiêu chuẩn này với tiêu chuẩn ở trên, bằng cách dùng các tính chất vi phân của lôgarit.

### 5. CÁC HỌ KHẢ TỔNG VÀ CÁC HỌ KHẢ NHÂN ĐƯỢC TRONG $\overline{\mathbf{R}}$

Trên khoảng $[0, + \infty]$ của $\overline{\mathbf{R}}$, phép cộng là một luật hợp thành kết hợp và giao hoán (§ 4, no. 3); do đó khái niệm một họ *khả tổng* các số trong khoảng này được xác định (Chương III, § 5, no. 1, Nhận xét 3).

#### Mệnh đề 2 {#top-iv-s7-prop-2 .statement}

*Mọi họ* $(x_i)$ *gồm các số thực* $\geq 0$ *đều khả tổng trong* $\overline{\mathbf{R}}$.

Vì ánh xạ $H \to s_H$ của tập có hướng $\mathfrak{F}(I)$ vào $\overline{\mathbf{R}}$ là *tăng*; do đó (§ 5, no. 2, Định lý 2) có một giới hạn.

Cùng lập luận ấy cho thấy rằng mọi họ số thực $\leq 0$ đều khả tổng trong $\overline{\mathbf{R}}$.

Tương tự, phép nhân là một luật hợp thành kết hợp và giao hoán trên mỗi khoảng $[0, 1]$ và $[1, + \infty]$ của $\overline{\mathbf{R}}$, và do đó khái niệm về một họ khả nhân được xác định trên mỗi khoảng ấy.

#### Mệnh đề 3 {#top-iv-s7-prop-3 .statement}

Mọi họ $(1 + u_i)$ [resp. $(1 - u_i)$] các số $\geq 1$ (resp. $\geq 0$ và $\leq 1$) đều khả tích trong $\overline{\mathbf{R}}$.

Chứng minh giống như đối với Mệnh đề 2.

#### Hệ quả {#top-iv-s7-n5-cor-1 .statement}

Tích $\prod (1 + u_i)$ [resp. $\prod (1 - u_i)$] của các số $\geq 1$ (resp. $> 0$ và $\leq 1$) bằng $+ \infty$ (resp. 0) khi và chỉ khi $\sum u_i = + \infty$.

Thật vậy, nếu $\sum u_i$ là hữu hạn thì $\prod (1 + u_i)$ và $\prod (1 - u_i)$ đều thuộc $\mathbf{R}^*$, và ngược lại (no. 4, Định lý 4).

#### Nhận xét {#top-iv-s7-n5-rem-1 .statement}

Định lý về tính kết hợp (Chương III, § 5, no. 3, Định lý 2) vẫn đúng khi thay G bằng $\overline{\mathbf{R}}$ và giả thiết rằng các $x_i$ đều $\geq 0$. Điều này hiển nhiên nếu $\sum_{i \in I} x_i$ là hữu hạn. Ngược lại, giả sử rằng $\sum_{i \in I} x_i = + \infty$. Khi đó với mỗi $a > 0$ hữu hạn, tồn tại một tập con hữu hạn H của I sao cho $\sum_{i \in H} x_i \geq a$. Gọi K là một tập con hữu hạn của L sao cho $H \subset \bigcup_{\lambda \in K} I_\lambda$; khi đó vì $s_\lambda \geq \sum_{i \in I_\lambda \cap H} x_i$ với mọi $\lambda \in K$, ta có
$$
\sum_{\lambda \in K} s_\lambda \geq \sum_{i \in H} x_i \geq a,
$$
điều này cho thấy rằng $\sum_{\lambda \in L} s_\lambda = + \infty$. Chúng tôi để người đọc phát biểu mệnh đề tương tự cho các họ nhân được của các số trong $[0, 1]$ hoặc trong $[1, + \infty]$.

### 6. CHUỖI VÔ HẠN VÀ TÍCH VÔ HẠN CỦA CÁC SỐ THỰC

Một chuỗi các số thực hữu hạn được gọi đơn giản là hội tụ nếu nó hội tụ trong $\mathbf{R}$.

#### Định nghĩa 1 {#top-iv-s7-def-1 .statement}

Một chuỗi các số thực hữu hạn được gọi là hội tụ tuyệt đối nếu chuỗi các giá trị tuyệt đối của các số hạng của nó hội tụ.

#### Mệnh đề 4 {#top-iv-s7-prop-4 .statement}

Một chuỗi các số thực hữu hạn là hội tụ giao hoán nếu và chỉ nếu nó hội tụ tuyệt đối.

Điều này suy ra từ Chương III, § 5, no. 7, Mệnh đề 9 và từ Định lý 3 của no. 2.

Nói cách khác, nếu $(u_n)$ là một dãy các số thực hữu hạn, thì nói rằng chuỗi có số hạng tổng quát là $u_n$ hội tụ giao hoán, hay hội tụ tuyệt đối, hay dãy $(u_n)$ là khả tổng trong $\mathbf{R}$, đều là như nhau. Mọi tính chất của các họ khả tổng được chứng minh trong Chương III, § 5 vì thế đều áp dụng cho các chuỗi hội tụ tuyệt đối. Đặc biệt, nếu chuỗi có số hạng tổng quát là $u_n$ hội tụ tuyệt đối, thì tổng $\sum_{n \in H} u_n$ tồn tại với mọi tập con $H$ của $\mathbf{N}$; và, nếu $(H_p)$ là một phân hoạch của $\mathbf{N}$, thì ta có
$$
\sum_{n=0}^{\infty} u_n = \sum_p \left( \sum_{n \in H_p} u_n \right)
$$
*(tính kết hợp* của các chuỗi hội tụ tuyệt đối).

Như chúng tôi đã nhận xét ở Chương III, § 5, một chuỗi số thực có thể hội tụ mà không hội tụ giao hoán, nghĩa là, không hội tụ tuyệt đối.

#### Ví dụ {#top-iv-s7-n6-exa-1 .statement}

*Chuỗi phản xứng.* Một chuỗi được xác định bởi một dãy $(u_n)$ các số thực hữu hạn được gọi là *phản xứng* nếu $u_n = (-1)^n v_n$, trong đó $v_n \geq 0$ với mọi $n$. Hãy chỉ ra rằng một điều kiện *đủ* để một chuỗi như vậy hội tụ là *dãy* $(v_n)$ *giảm và có* 0 *làm giới hạn*. Thật vậy, nếu $s_n$ ký hiệu
$$
\sum_{p=0}^{n} u_p,
$$
thì giả thiết rằng $(v_n)$ giảm kéo theo
$$
s_{2n+1} \leq s_{2n+3} \leq s_{2n+2} \leq s_{2n}
$$
với mọi $n \geq 0$. Dãy $(s_{2n})$ [tương ứng $(s_{2n+1})$] giảm và bị chặn dưới (tương ứng tăng và bị chặn trên), do đó có một giới hạn hữu hạn $a$ (tương ứng $b$), và $b \leq a$; vì
$$
a - b = \lim_{n \to \infty} (s_{2n} - s_{2n+1}) = \lim_{n \to \infty} v_{2n+1} = 0,
$$
mệnh đề được chứng minh.

Chẳng hạn nếu lấy $v_n = 1/n$, thì các điều kiện trên được thỏa mãn, và do đó chuỗi có số hạng tổng quát là $(-1)^n / n$ ("chuỗi điều hòa phản xứng") là hội tụ. Ta đã thấy ở no. 1 rằng chuỗi có số hạng tổng quát là $1/n$ ("chuỗi điều hòa") thì không hội tụ, và vì thế chuỗi điều hòa phản xứng không hội tụ tuyệt đối.

Ta nhắc lại (Chương III, § 5, no. 6, Mệnh đề 7) rằng, nếu $(u_n)$ và $(v_n)$ là hai chuỗi hội tụ gồm các số thực hữu hạn, thì chuỗi $(u_n + v_n)$ là hội tụ, và
$$
\sum_{n=0}^{\infty} (u_n + v_n) = \sum_{n=0}^{\infty} u_n + \sum_{n=0}^{\infty} v_n;
$$
hơn nữa, nếu chuỗi $(u_n)$ hội tụ thì chuỗi $(au_n)$ hội tụ với mọi số thực hữu hạn $a$, và $\sum_{n=0}^{\infty} au_n = a \cdot \sum_{n=0}^{\infty} u_n$.

Cuối cùng, nếu các chuỗi $(u_n)$ và $(v_n)$ hội tụ, và nếu $u_n \leq v_n$ với mọi $n$, thì ta có $\sum_{n=0}^{\infty} u_n \leq \sum_{n=0}^{\infty} v_n$ theo nguyên lý mở rộng các bất đẳng thức (\S 5, no. 2, Định lý 1).

Cần lưu ý rằng, nếu ta giả sử chuỗi $(v_n)$ hội tụ nhưng không hội tụ tuyệt đối, và nếu $|u_n| \leq |v_n|$ với mỗi $n$, thì hoàn toàn không thể suy ra rằng chuỗi $(u_n)$ hội tụ, như thấy được khi lấy $u_n = |v_n|$.

Một tích vô hạn các số thực hữu hạn khác không được gọi đơn giản là hội tụ nếu nó hội tụ trong $\mathbf{R}^*$; khi đó giá trị của nó là một số thực hữu hạn khác không.

#### Định nghĩa 2 {#top-iv-s7-def-2 .statement}

*Một tích vô hạn có nhân tử tổng quát là $1 + u_n$ được gọi là hội tụ tuyệt đối nếu tích có nhân tử tổng quát là $1 + |u_n|$ hội tụ.*

#### Mệnh đề 5 {#top-iv-s7-prop-5 .statement}

*Một tích vô hạn các số thực hữu hạn là hội tụ giao hoán khi và chỉ khi nó hội tụ tuyệt đối.*

Điều này suy ra từ Chương III, \S 5, no. 7, Mệnh đề 9, và từ Định lý 4 ở trên.

Hơn nữa, tích có nhân tử tổng quát là $1 + u_n$ là *hội tụ tuyệt đối* khi và chỉ khi chuỗi có số hạng tổng quát là $u_n$ là *hội tụ tuyệt đối*.

Một tích các số thực khác không có thể hội tụ mà không hội tụ giao hoán, nghĩa là không hội tụ tuyệt đối.

#### Ví dụ {#top-iv-s7-n6-exa-2 .statement}

Nếu ta lấy $u_{2n-1} = -1/n$ và $u_{2n} = 1/n$ với $n \geq 2$, thì tích $(1 + u_n)$ không hội tụ tuyệt đối, vì chuỗi $(u_n)$ không hội tụ tuyệt đối; nhưng vì

$$
\prod_{p=3}^{n} (1 + u_p) = \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right),
$$
và
$$
\prod_{p=3}^{2n+1} (1 + u_p) = \left(1 - \frac{1}{n+1}\right) \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right),
$$
nên suy ra từ Định lý 4 rằng tích ấy hội tụ và giá trị của nó là
$$
\prod_{n=2}^{\infty} \left(1 - \frac{1}{n^2}\right).
$$

Hơn nữa, cần nhận thấy rằng *sự hội tụ* của chuỗi có số hạng tổng quát là $u_n$ *không phải là điều kiện cần cũng không phải là điều kiện đủ* cho *sự hội tụ* của tích có nhân tử tổng quát là $1 + u_n$ (xem Bài tập 21 và 22).

### Bài tập {#top-iv-s7-exercises}

Xem [bài tập của § 7](exercises/s7/).
