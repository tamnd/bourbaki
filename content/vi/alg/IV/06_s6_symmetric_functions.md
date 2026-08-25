---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 6
section_title: Symmetric functions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.98-A IV.105
pdf_pages: 0070-0095, 0107-0114
extraction: ocr
subsections:
    - "no": 1
      title: Symmetric polynomials
      page: 61
      pdf_page: 70
    - "no": 2
      title: Symmetric rational fractions
      page: 67
      pdf_page: 76
    - "no": 3
      title: Symmetric formal power series
      page: 67
      pdf_page: 76
    - "no": 4
      title: Sums of powers
      page: 70
      pdf_page: 79
    - "no": 5
      title: Symmetric functions in the roots of a polynomial
      page: 72
      pdf_page: 81
    - "no": 6
      title: The resultant
      page: 75
      pdf_page: 84
    - "no": 7
      title: The discriminant
      page: 81
      pdf_page: 90
statements: 43
exercises: 12
content_sha256: c5967631d4b873f6621a264fcd7bd519740785457f8ecaaf6d701cbd38dcdc83
translated_from: content/en/alg/IV/06_s6_symmetric_functions.md
source_content_sha256: c0d6d98ff4015c3c6fee324330e8258f97161700ae1a515e8b9b28fc72039a2d
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-fa2660c6
glossary_version: 34
glossary_terms_sha256: 9e09c9270d0e1d860b0a905a48ba1a28d78e9141956b460ebd62a5335a350d71
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. HÀM ĐỐI XỨNG

### 1. Đa thức đối xứng

Cho $n$ là một số nguyên dương. Với mọi phép hoán vị $\sigma \in \mathfrak{S}_n$, ký hiệu $\varphi_\sigma$ là tự đẳng cấu của đại số trên A $A[X_1, \ldots, X_n]$ biến $X_i$ thành $X_{\sigma(i)}$ với $1 \leq i \leq n$. Rõ ràng ánh xạ $\sigma \mapsto \varphi_\sigma$ là một đồng cấu của $\mathfrak{S}_n$ vào nhóm các tự đẳng cấu của $A[X_1, \ldots, X_n]$. Ta đặt $\sigma f = \varphi_\sigma(f)$ với $\sigma \in \mathfrak{S}_n$ và $f \in A[X_1, \ldots, X_n]$. Đa thức f được gọi là đối xứng nếu $\sigma f = f$ với mọi $\sigma \in \mathfrak{S}_n$ ; các đa thức đối xứng lập thành một đại số con có đơn vị phân bậc của $A[X_1, \ldots, X_n]$ ; trong phần này, ta sẽ ký hiệu đại số đó bởi $A[X_1, \ldots, X_n]^{\mathrm{sym}}$.
Với mỗi số nguyên dương k, ta ký hiệu $\mathfrak{P}_k$ là tập hợp các tập con gồm k phần tử của tập hợp $\{1, 2, \ldots, n\}$ và đặt

(1)
$$
s_k = \sum_{H \in \mathfrak{P}_k} \prod_{i \in H} X_i .
$$

Khi muốn chỉ rõ số nguyên n, ta sẽ viết $s_{k,n}$ thay cho $s_k$. Đặc biệt, ta có

$$
\begin{aligned}
s_0 &= 1 \\
s_1 &= \sum_{1 \leq i \leq n} X_i \\
s_2 &= \sum_{1 \leq i < j \leq n} X_i X_j \\
&\ \ \cdots \cdots \cdots \cdots \cdots \\
s_n &= X_1 \ldots X_n
\end{aligned}
$$

và $s_k = 0$ với $k > n$. Rõ ràng $s_k$ là một đa thức đối xứng thuần nhất bậc k ; ta gọi nó là đa thức đối xứng sơ cấp bậc k.
Trong vành $A[X_1, \ldots, X_n, U, V]$ ta có quan hệ

(2)
$$
\prod_{i=1}^{n} (U + V X_i) = \sum_{k=0}^{n} U^{n-k} V^k s_k ;
$$

bằng những phép thế thích hợp, ta suy ra các quan hệ

(3)
$$
\prod_{i=1}^{n} (1 + T X_i) = \sum_{k=0}^{n} s_k T^k ,
$$

(4)
$$
\prod_{i=1}^{n} (\mathbf{X} - \mathbf{X}_i) = \sum_{k=0}^{n} (-1)^{n-k} s_{n-k} \mathbf{X}^k .
$$

#### Định lý 1 {#alg-iv-s6-thm-1 .statement}

— Đặt $E = A[\mathbf{X}_1, \ldots, \mathbf{X}_n]$ và $S = A[\mathbf{X}_1, \ldots, \mathbf{X}_n]^{\text{sym}}$.

a) Đại số trên $A$ $S$ của các đa thức đối xứng được sinh bởi $s_1, \ldots, s_n$.

b) Các phần tử $s_1, \ldots, s_n$ của $E$ độc lập đại số trên $A$ (IV, p. 4).

c) Họ các đơn thức $X^v = X_1^{v(1)} \ldots X_n^{v(n)}$ sao cho $0 \leq v(i) < i$ với $1 \leq i \leq n$ là một cơ sở của môđun $S$- $E$. Đặc biệt, $E$ là một môđun $S$ tự do có hạng $n!$.

Ta sẽ chứng minh định lý bằng quy nạp theo $n$, trường hợp $n = 0$ là tầm thường. Đặt $B = A[X,]$ và ký hiệu $s_k'$ là đa thức đối xứng sơ cấp bậc $k$ theo $X_1, \ldots, X_{-1}$; do đó ta có $B[X_1, \ldots, X_{-1}] = A[X_1, \ldots, X_n]$. Nếu thay $n$ bởi $n-1$ và $A$ bởi $B$ trong mệnh đề của Th. 1, ta có thể phát biểu giả thiết quy nạp như sau:

(A) $B$-đại số $S'$ của các đa thức $f \in A[\mathbf{X}_1, \ldots, \mathbf{X}_n]$ bất biến dưới mọi hoán vị của $X,, \ldots, X_{-1}$ được sinh bởi $s_1', \ldots, s_{n-1}'$.

(B) Các phần tử $s_1', \ldots, s_{n-1}'$ của $E$ độc lập đại số trên $B$.

(C) Họ các đơn thức $X_1^{v(1)} \ldots X_{n-1}^{v(n-1)}$ sao cho $0 \leq v(i) < i$ với $1 \leq i \leq n-1$ là một cơ sở của $S'$-môđun $E$.

Ta có hệ thức hiển nhiên

(5)
$$
s_k = s_k' + s_{k-1}' X_n \quad (1 \leq k \leq n-1),
$$
từ đó ta suy ra bằng quy nạp theo $k$

(6)
$$
s_k' = (-1)^k X_n^k + \sum_{i=1}^k (-1)^{k-i} s_i X_n^{k-i} \quad (1 \leq k \leq n-1).
$$

Ta có $S \subset S'$, do đó $s_1, \ldots, s_n$ thuộc $S'$; theo (A) và công thức (6) $B$-đại số $S'$ vì thế được sinh bởi $s_1, \ldots, s_{n-1}'$.

Theo (B) tồn tại một tự đồng cấu $\mu$ của $B$-đại số $S'$ sao cho

(7)
$$
u(s_k') = (-1)^k X_n^k + \sum_{i=1}^k (-1)^{k-i} s_i' X_n^{k-i} \quad (1 \leq k \leq n-1).
$$

Theo (5), ta có $u(s_k) = u(s_k') + u(s_{k-1}') X_n$, do đó $u(s_k) = s_k'$ bằng một tính toán dễ dàng. Cho $P \in B[Y_1, \ldots, Y_{-1}]$; khi đó từ $P(s_1, \ldots, s_{n-1}) = 0$ ta suy ra
$$
0 = u(P(s_1, \ldots, s_{n-1})) = P(s_1', \ldots, s_{n-1}'),
$$
do đó $P = 0$ theo (B). Suy ra rằng $B$-đại số $S'$ được sinh bởi các phần tử độc lập đại số $s_1, \ldots, s_{n-1}$. Tính chất này có thể được phát biểu lại như sau:
(D) $A$-đại số $S'$ được sinh bởi các phần tử độc lập đại số $s_1, \ldots, s_{n-1}, X_n$.

Vì thế ta có thể đồng nhất S' với vành đa thức $C[X_n]$, trong đó $C$ là đại số con trên $A$ của $E$ được sinh bởi $s_1, ..., s_{n-1}$.

Để chứng minh a), cho $f \in S$ là một đa thức đối xứng thuần nhất bậc $m$. Ta có $f \in S' = C[X_n]$, nên tồn tại một phần tử $g = P(s_1, ..., s_{n-1})$ của C, thuần nhất bậc $m$ theo $X_1, ..., X_n$, sao cho $f - g$ chia được cho $X_n$. Vì $f - g$ là đối xứng, mỗi số hạng của nó cũng chia được cho $X_1, ..., X_{n-1}$, do đó $f - g$ chia được cho $s_n = X_1 ... X_n$. Nói cách khác, tồn tại $h \in S$ sao cho $f = g + hs_n$, do đó $\deg h < m$. Bằng quy nạp theo $m$ suy ra rằng $f$ thuộc

$$
C[s_n]_E = A[s_1, ..., s_{n-1}, s_n]_E .
$$

Vậy ta đã chứng minh rằng $A$-đại số S được sinh bởi $s_1, ..., s_n$.

Tiếp theo ta chứng minh b). Nếu thay $X$ cho $X$ trong (4), ta được

$$
(-1)^{n+1}s_n = X_n^n + \sum_{k=1}^{n-1} (-1)^{n-k} s_{n-k} X_n^k ;
$$

nói cách khác, $(-1)^{n+1}s_n$ là một đa thức đơn khởi theo $X$, có bậc $n$ và các hệ số thuộc $C$. Theo IV, p. 11, ta có tính chất sau:
(E) Đồng cấu đại số $\varphi$ của $C[T]$ vào $C[X_n] = S'$ biến T thành $s_n$ là đơn ánh, và $S'$ là một môđun tự do trên ảnh của $\varphi$, với cơ sở $(1, X_n, ..., X_n^{n-1})$.

Các phần tử $s_1, ..., s_{n-1}$ của $C$ độc lập đại số trên A, theo (D); do đó tính đơn ánh của $\varphi$ có nghĩa là $s_1, ..., s_{n-1}, s_n$ độc lập đại số trên A, do đó b).

Để chứng minh c), ảnh của $\varphi$ bằng $C[s_n]_E = S$, do đó theo (E), $S'$ là một môđun tự do trên S với cơ sở $(1, X_1, ..., X_n^{n-1})$. Bây giờ mệnh đề c) suy ra từ giả thiết quy nạp (C) và Mệnh đề 25 của II, p. 222. Điều này hoàn tất chứng minh.

Cho $f$ là một đa thức đối xứng theo $X_1, ..., X_n$, thuần nhất bậc $m$. Theo Định lý 1 (IV, p. 62), tồn tại một đa thức $Q \in A[Y_1, ..., Y_n]$ sao cho $f = Q(s_1, ..., s_n)$. Chứng minh trên cung cấp một phương tiện tính toán tường minh $Q$, bằng quy nạp kép theo $n$ và $m$. Thật vậy, như đã thấy, tồn tại một đa thức $P \in A[Y_1, ..., Y_{n-1}]$ và một đa thức h đối xứng theo $X_1, ..., X_n$, thuần nhất bậc $m-n$, sao cho

$$
f = P(s_1, ..., s_{n-1}) + s_n h .
$$

Với mọi đa thức $u \in A[X_1, ..., X_n]$, ta đặt

$$
u'(X_1, ..., X_{n-1}) = u(X_1, ..., X_{n-1}, 0)
$$

Khi đó $s'_1, ..., s'_{n-1}$ là các đa thức đối xứng sơ cấp theo $X_1, ..., X_{n-1}$ và công thức (8) cho

$$
f' = P(s'_1, ..., s'_{n-1})
$$

Do đó, việc xác định $P$ được quy về một phép tính các đa thức đối xứng theo $n - 1$ bất định, còn $h$ thu được từ (8).

Ta minh họa phương pháp bằng hai ví dụ.

**Ví dụ. — 1)** Cho $n = 3$ và

$$
f = X_1^2(X_2 + X_3) + X_2^2(X_3 + X_1) + X_3^2(X_1 + X_2).
$$

Ta có

$$
f' = X_1^2X_2 + X_1X_2^2 = X_1X_2(X_1 + X_2) = s'_1s'_2.
$$

Đặt $g = f - s_1s_2$; ta có

$$
g = f - (X_1 + X_2 + X_3)(X_1X_2 + X_1X_3 + X_2X_3) = -3X_1X_2X_3,
$$

do đó cuối cùng

$$
f = s_1s_2 - 3s_3.
$$

2) Lại cho $n = 3$ và đặt $p = X_1^3 + X_2^3 + X_3^3$.
Ta có $p(X_1, 0, 0) = X_1^3 = s_1(X_1, 0, 0)^3$. Đặt $q = p - s_1^3$, ta được

$$
q = -3f - 6X_1X_2X_3 = -3s_1s_2 + 3s_3
$$

và cuối cùng

$$
p = s_1^3 - 3s_1s_2 + 3s_3.
$$

Cho $S_1, ..., S_n$ là các bất định. Ta trang bị cho đại số đa thức $A[S_1, ..., S_n]$ phép phân bậc kiểu $N$ trong đó $S_k$ có trọng số $k$ với $1 \leq k \leq n$ (IV, p. 3), và ta trang bị cho $A[X_1, ..., X_n]$ phép phân bậc thông thường. Với $1 \leq k \leq n$ đa thức đối xứng sơ cấp $s_{k,n}$ theo $X_1, ..., X_n$ là thuần nhất bậc $k$. Theo Định lý 1 (IV, p. 62) ánh xạ $g \mapsto g(s_{1,n}, ..., s_{n,n})$ do đó là một đẳng cấu của các đại số phân bậc

$$
\varphi_n : A[S_1, ..., S_n] \to A[X_1, ..., X_n]^{\text{sym}}
$$

Cho $m$ là một số nguyên sao cho $0 \leq m \leq n$. Với mọi số nguyên $k$ sao cho $1 \leq k \leq m$ ta có

$$
s_{k,m}(X_1, ..., X_m) = s_{k,n}(X_1, ..., X_m, 0, ..., 0)
$$

theo định nghĩa (IV, p. 61, công thức (1)) của $s_k$. Do đó biểu đồ

$$
\begin{array}{ccc}
A[S_1, ..., S_m] & \xrightarrow{j} & A[S_1, ..., S_n] \\
\varphi_m \downarrow & & \varphi_n \downarrow \\
A[X_1, ..., X_m]^{\text{sym}} & \xleftarrow{p} & A[X_1, ..., X_n]^{\text{sym}}
\end{array}
$$

(trong đó j là phép nhúng chính tắc và $p$ là đồng cấu
$$
g \mapsto g (X_1, \ldots, X_m, 0, \ldots, 0)
$$
là giao hoán.

#### Mệnh đề 1 {#alg-iv-s6-prop-1 .statement}

*Với mọi cặp số nguyên dương k, n, gọi $S_k^{(n)}$ là A-môđun gồm tất cả các đa thức đối xứng theo $X_1, \ldots, X_n$, thuần nhất bậc k. Nếu số nguyên m thỏa mãn $0 \leq k \leq m \leq n$, thì ánh xạ $f \mapsto f (X_1, \ldots, X_m, 0, \ldots, 0)$ là một đẳng cấu của $S_k^{(n)}$ lên $S_k^{(m)}$.*

Do tính giao hoán của biểu đồ (10), chỉ cần chứng minh rằng mọi đa thức đẳng áp trọng số k trong $S_1, \ldots, S_n$ chỉ phụ thuộc vào $S_1, \ldots, S_m$ dưới các giả thiết $0 \leq k \leq m \leq n$. Bây giờ trọng số của một đơn thức $S_1^{\alpha(1)} \cdots S_n^{\alpha(n)}$ bằng số nguyên $\alpha(1) + 2\alpha(2) + \ldots + n\alpha(n)$; vì các số nguyên $\alpha(1), \ldots, \alpha(n)$ là dương, quan hệ
$$
\alpha(1) + 2\alpha(2) + \cdots + n\alpha(n) = k \leq n
$$
suy ra $\alpha(j) = 0$ với $k < j \leq n$, do đó có khẳng định.

#### Ví dụ 3 {#alg-iv-s6-n1-exa-3 .statement}

Theo ví dụ 2 của IV, p. 64 và Mệnh đề 1 ở trên ta có do đó
$$
\sum_{i=1}^n X_i^3 = s_{1,n}^3 - 3s_{1,n}s_{2,n} + 3s_{3,n}
$$
với mọi số nguyên $n \geq 3$. Tính giao hoán của biểu đồ (10) hơn nữa cho các công thức
$$
X_1^3 + X_2^3 = s_{1,2}^3 - 3s_{1,2}s_{2,2},
$$
$$
X_1^3 = s_{1,1}^3.
$$

#### Nhận xét {#alg-iv-s6-n1-rem-1 .statement}

— Cho n và k là hai số nguyên dương. Ta ký hiệu $\Delta_{k,n}$ là tập hợp các phần tử có độ dài k trong $N^n$ và hơn nữa trang bị cho $A$, , quan hệ thứ tự, ký hiệu là $a \leq \beta$, cảm sinh bởi quan hệ thứ tự từ điển trên $N^n$ (*Lý thuyết tập hợp*, III, p. 157), và định nghĩa một tác động của nhóm $\mathfrak{S}_n$ trên $N^n$ bởi $(\sigma a)(i) = a(\sigma^{-1}(i))$ với $\sigma \in \mathfrak{S}_n, a \in N^n$ và $l \leq i \leq n$. Hơn nữa, ta ký hiệu $D_k$ là tập hợp các phần tử $a = (\alpha(1), \ldots, \alpha(k))$ của $\mathbf{N}^k$ sao cho
$$
\alpha(1) \geq \alpha(2) \geq \cdots \geq \alpha(k), \quad \alpha(1) + \cdots + \alpha(k) = k.
$$

Giả sử $k \leq n$ và đồng nhất $\mathbf{N}^k$ với một tập con của $N^n$ bằng ánh xạ $(a(1), \ldots, a(k)) \mapsto (a(1), \ldots, a(k), 0, \ldots, 0)$. Khi đó $D_k$ gồm các phần tử $a$ của $\Delta_{k,n}$ sao cho $\sigma a \leq a$ với mọi $\sigma \in \mathfrak{S}_n$. Suy ra rằng mọi quỹ đạo của nhóm $\mathfrak{S}_n$ trong $A$, , đều chứa một phần tử duy nhất của $D_k$. Với mọi $a \in D_k$ gọi $O(a)$ là quỹ đạo của $a$ trong $\Delta_{k,n}$ dưới phép toán của $\mathfrak{S}_n$; đặt
$$
M(\alpha) = \sum_{\beta \in O(\alpha)} X^\beta.
$$

Từ Bổ đề 1 của IV, p. 47, suy ra rằng họ $(\mathbf{M}(\alpha))_{\alpha \in D_k}$ là một cơ sở của A-môđun $S_k^{(n)}$.

Với mỗi $\alpha \in D_k$ đặt

$$
(12)\quad S(\alpha) = \prod_{i=1}^k s_i^{\alpha(i) - \alpha(i+1)} \quad \text{(với quy ước rằng } a\ (k+1) = 0 \text{)} ;
$$

vì ta có $\sum_{i=1}^k i \cdot (a(i) - a(i+1)) = \sum_{i=1}^k a(i) = k$, đa thức đối xứng $S(\alpha)$ là thuần nhất có bậc $k$. Từ Định lý 1 (IV, p. 62) suy ra trực tiếp rằng họ $(S(\alpha))_{\alpha \in D_k}$ là một cơ sở của A-môđun $S_k^{(n)}$.

Cho $\alpha, \beta$ thuộc $D_k$, và gọi $c_{\alpha\beta}$ là hệ số của đơn thức $X^\beta$ trong đa thức $S(\alpha)$ được định nghĩa bởi (12) trong trường hợp $A = \mathbf{Z}$ và $k = n$. Đây là một số nguyên dương, *độc lập với vành A và số nguyên n*. Theo công thức (9) (IV, p. 64) ta có

$$
(13)\quad S(\alpha) = \sum_{\beta \in D_k} c_{\alpha\beta} \cdot \mathbf{M}(\beta) \quad (\alpha \in D_k) .
$$

Có thể chứng minh được (xem IV, p. 101, Bài tập 13) rằng ma trận $C = (c_{\alpha\beta})_{\alpha,\beta \in D_k}$ có tính chất $c_{\alpha\alpha} = 1$ và $c_{\alpha\beta} = 0$ với $\alpha < \beta$; khái quát hóa thuật ngữ được đưa vào trong II, p. 351, ta sẽ nói rằng $C$ thuộc nhóm tam giác toàn phần dưới. Điều tương tự cũng đúng đối với ma trận D nghịch đảo của C. Các giá trị của các ma trận C và D khi $2 \leq k \leq 5$, được cho trong bảng (IV, p. 103-105).

Giả sử bây giờ $n < k$ và đồng nhất $N^n$ với một tập con của $N^k$ bằng ánh xạ $(a(1), \ldots, a(n)) \mapsto (a(1), \ldots, a(n), 0, \ldots, 0)$. Với mỗi $a$ trong $D_k \cap N^n$ ta lại ký hiệu $O(\alpha)$ là quỹ đạo của $a$ trong $\Delta_{k,n}$ dưới phép toán của $\mathfrak{S}_n$ và định nghĩa $\mathbf{M}(\alpha)$ bởi (11). Hơn nữa ta định nghĩa $S(\alpha)$ bởi (12), khi đó các họ $(\mathbf{M}(a))_{a \in D_k \cap N^n}$ và $(S(a))_{a \in D_k \cap N^n}$ là các cơ sở của A-môđun $S_k^{(n)}$. Theo công thức (9) của IV, p. 64, ta có một công thức tương tự (13) trong đó $D_k$ được thay bởi $D_k \cap N^n$, với cùng các số nguyên $c_{\alpha\beta}$.

#### Ví dụ 4 {#alg-iv-s6-n1-exa-4 .statement}

Theo Ví dụ 3 của IV, p. 65, ta có

$$
\mathbf{M}(3,0,0) = S(3,0,0) - 3S(2,1,0) + 3S(1,1,1)
$$

cho mọi số nguyên $n \geq 3$, và do đó

$$
\mathbf{M}(3,0) = S(3,0) - 3S(2,1)
$$

đối với $n = 2$.

### 2. Phân thức hữu tỉ đối xứng

Cho $K$ là một trường giao hoán và $X_1, X_2, \ldots, X_n$ là các phần tử bất định. Với mọi $\sigma \in S_n$, ta đã định nghĩa trong No. 1 (IV, p. 61) một tự đẳng cấu $\varphi_\sigma$ của $K[X_1, X_2, \ldots, X_n]$. Tự đẳng cấu này có một mở rộng duy nhất $\psi_\sigma$ tới trường $K(X_1, \ldots, X_n)$, và $\sigma \mapsto \psi_\sigma$ là một đơn cấu của $S_n$ vào nhóm tự đẳng cấu của $K(X_1, \ldots, X_n)$. Với mỗi $f \in K(X_1, \ldots, X_n)$, ta có $(\psi_\sigma f)(X_1, \ldots, X_n) = f(X_{\sigma(1)}, \ldots, X_{\sigma(n)})$. Các phân thức hữu tỉ $f$ sao cho $\psi_\sigma(f) = f$ với mọi $\sigma \in S_n$ được gọi là các phân thức hữu tỉ đối xứng. Tập hợp tất cả các phân thức hữu tỉ đối xứng theo $X_1, \ldots, X_n$ là một trường con của $K(X_1, \ldots, X_n)$.

#### Mệnh đề 2 {#alg-iv-s6-prop-2 .statement}

— *Trường các phân thức hữu tỉ đối xứng theo $X_1, \ldots, X_n$ là trường các phân thức của vành các đa thức đối xứng theo $X_1, \ldots, X_n$.*.

Cho $f \in K(X_1, \ldots, X_n)$ là một phân thức hữu tỉ đối xứng, và cho $u_1, v_1$ là hai phần tử của $K[X_1, \ldots, X_n]$ sao cho $f = \frac{u_1}{v_1}$. Đặt $v = \prod_{\sigma \in S_n} \psi_\sigma(v_1) \in K[X_1, \ldots, X_n]$ và $u = fv \in K[X_1, \ldots, X_n]$; khi đó $v$ đối xứng, do đó $u$ đối xứng, vì $f$ đối xứng, và $f = \frac{u}{v}$, do đó có kết quả.

#### Hệ quả {#alg-iv-s6-n2-cor-1 .statement}

— *Cho $s_1, s_2, \ldots, s_n$ là các đa thức đối xứng sơ cấp theo $X_1, \ldots, X_n$. Với mọi phân thức hữu tỉ $g \in K(S_1, S_2, \ldots, S_n)$, dãy $(s_1, s_2, \ldots, s_n)$ có thể thế vào $g$ và ánh xạ $g \mapsto g(s_1, s_2, \ldots, s_n)$ là một đẳng cấu của $K(S_1, S_2, \ldots, S_n)$ lên trường các phân thức hữu tỉ đối xứng theo $X_1, \ldots, X_n$.*

Điều này suy ra từ Mệnh đề 2 và Định lý 1 của IV, p. 62.

### 3. Chuỗi lũy thừa hình thức đối xứng

Cho $I$ là một tập hợp, $X = (X_i)_{i \in I}$ là một họ các ẩn thức và $A[[X]]$ là đại số các chuỗi lũy thừa hình thức theo các $X_i$. Với mọi phép hoán vị $a \in S_I$ tồn tại duy nhất một tự đẳng cấu liên tục $\varphi_a$ của đại số $A[[X]]$ gửi $X_i$ đến $X_{a(i)}$ với mỗi $i \in I$ (IV, p. 28, Mệnh đề 4); hiển nhiên $\sigma \mapsto \varphi_\sigma$ là một đồng cấu của $S_I$ vào nhóm các tự đẳng cấu liên tục của đại số $A[[X]]$. Cho $f \in A[[X]]$ là một chuỗi lũy thừa hình thức; ta đặt $af = \varphi_a(f)$ và ta sẽ nói rằng chuỗi lũy thừa hình thức $f$ là đối xứng nếu $\sigma f = f$ với mỗi $\sigma \in S_I$. Các chuỗi lũy thừa hình thức đối xứng tạo thành một đại số con đóng của $A[[X]]$ được ký hiệu bởi $A[[X]]^{\text{sym}}$ và được trang bị tôpô cảm sinh bởi tôpô của $A[[X]]$.

Cho $T$ là một ẩn thức. Trong vành các chuỗi lũy thừa hình thức $A[[X, T]]$ họ $(X_i T)_{i \in I}$ là cộng được, do đó họ $(1 + X_i T)_{i \in I}$ là nhân được (IV, p. 27, Mệnh đề 2); hơn nữa ta có

$$
\prod_{i \in I} (1 + X_i T) = 1 + \sum_{k \geq 1} s_k T^k,
$$

trong đó chuỗi lũy thừa hình thức $s_k \in A[[X]]$ được định nghĩa bởi

$$
s_k = \sum_{H \in \mathcal{P}_k} \left( \prod_{i \in H} X_i \right) \quad (k \geq 1)
$$

(ta ký hiệu $\mathcal{P}_k$ là tập hợp tất cả các tập con gồm k phần tử của I). Đặc biệt ta có $s_1 = \sum_{i \in I} X_i$. Khi I là hữu hạn với n phần tử ta có $s_k = 0$ với $k > n$; chính xác hơn, khi $I = \{1, \ldots, n\}$ thì chuỗi lũy thừa hình thức $s_k$ chẳng gì khác hơn đa thức đối xứng sơ cấp bậc k theo $X_1, \ldots, X_n$.

Cho $S = (S_k)_{k \geq 1}$ là một dãy các ẩn thức. Vì chuỗi lũy thừa hình thức $s_k$ có bậc $\geq k$, và thuộc $A[[X]]^{\text{sym}}$, nên các điều kiện a) và b) của Mệnh đề 4 ở IV, p. 28 được thỏa mãn với $E = A[[X]]^{\text{sym}}$; do đó tồn tại duy nhất một đồng cấu đại số trên A liên tục

$$
\varphi_I : A[[S]] \to A[[X]]^{\text{sym}}
$$

sao cho $\varphi_I(S_k) = s_k$ với mỗi số nguyên $k \geq 1$.

**Định lý 2. — a)** *Nếu I là một tập hữu hạn có n phần tử, thì $\varphi_I$ cảm sinh một đẳng cấu song liên tục của $A[[S_1, \ldots, S_n]]$ lên $A[[X]]^{\text{sym}}$*.

*b)* *Nếu I là vô hạn, $\varphi_I$ là một đẳng cấu song liên tục của $A[[S]]$ lên $A[[X]]^{\text{sym}}$*.

Trong trường hợp a), ta đặt $B = A[[S_1, \ldots, S_n]]$ và trang bị cho đại số này tôpô cảm sinh bởi tôpô của $A[[S]]$; ta cũng ký hiệu bởi $\psi_I$ hạn chế của $\varphi_I$ trên B. Trong trường hợp b), ta đặt $B = A[[S]]$ và $\psi_I = \varphi_I$. Ta sẽ trang bị cho đại số đa thức $A[S]$ phân bậc kiểu N sao cho $S_k$ có trọng số k với mỗi số nguyên $k \geq 1$.

**Bổ đề 1. — Cho $J$ là một tập con hữu hạn của $I$, $r$ là một số nguyên sao cho Card $J \geq r$ và $f$ là một chuỗi lũy thừa hình thức đối xứng thuần nhất bậc $r$ trong các $X_i$ ($i \in I$). Cho $\bar{f}$ là chuỗi lũy thừa hình thức thu được bằng cách thay $0$ vào $X_i$ đối với mỗi $i$ trong $I - J$. Nếu $\bar{f} = 0$, thì ta có $f = 0$.**

Đặt $f = \sum_{|\alpha| = r} a_\alpha X^\alpha$ (trong đó $|\alpha|$ là độ dài $\sum_{i \in I} \alpha_i$ của đa chỉ số $a = (\alpha_i)_{i \in I}$). Nếu $a$ là một đa chỉ số có độ dài $r$, và $J'$ là tập hỗ trợ của $a$ (tập các $i \in I$ sao cho $\alpha_i \neq 0$), thì Card $J' \leq r$, do đó tồn tại một phép hoán vị $\sigma \in S_I$ sao cho $\sigma(J') \subset J$. Đặt $\beta_i = \alpha_{\sigma^{-1}(i)}$ với mọi $i \in I$, khi đó đơn thức $X^\beta = \prod_{i \in I} X_{\sigma(i)}^{\alpha_i}$ chỉ phụ thuộc vào các ẩn $X_j$ ($j \in J$), do đó theo giả thiết $\overline{f} = 0$ thì $a_\beta = 0$. Vì $f$ đối xứng, ta có $a_\alpha = a_\beta$ và vì $\alpha$ tùy ý, suy ra $f = 0$.

#### Bổ đề 2 {#alg-iv-s6-lem-2 .statement}

*Cho $f$ là một chuỗi lũy thừa hình thức đối xứng bậc $r$ trong các $X_i (i \in I)$. Tồn tại duy nhất một đa thức $P \in B \cap A[S]$, đồng trọng có trọng số $r$, sao cho $f = \psi_1(P)$.*

Trường hợp $I$ hữu hạn suy ra từ Định lý 1 (IV, p. 62).

Giả sử rằng $I$ là vô hạn và chọn một tập con hữu hạn $J$ của $I$, chứa $r$ phần tử. Chúng ta giữ ký hiệu của Bổ đề 1; ta nhận xét rằng mọi đa thức đồng trọng có trọng số $r$ trong các $S_n \ (n \geq 1)$ chỉ phụ thuộc vào $S_1, \ldots, S_r$ và rằng $\overline{s}_1, \ldots, \overline{s}_r$ là các đa thức đối xứng sơ cấp trong $r$ ẩn $X_j \ (j \in J)$. Nếu $P$ là một đa thức đồng trọng có trọng số $r$ trong các $S_n$ và $h = f - \psi_1(P)$, thì $\overline{h} = \overline{f} - P(\overline{s}_1, \ldots, S_r)$ và Bổ đề 1 cho thấy quan hệ $f = \psi_1(P)$ tương đương với $\overline{f} = P(\overline{s}_1, \ldots, \overline{s}_r)$. Theo Định lý 1 (IV, p. 62) tồn tại duy nhất một đa thức $P \in A[S]$, đồng trọng có trọng số $r$ và sao cho $\overline{f} = P(\overline{s}_1, \ldots, \overline{s}_r)$, do đó suy ra kết quả.

#### Bổ đề 3 {#alg-iv-s6-lem-3 .statement}

*Với mỗi số nguyên $m \geq 0$, cho $c_m$ là iđêan của đại số $A[[X]]^{sym}$ gồm tất cả các chuỗi lũy thừa hình thức đối xứng có cấp $\geq m$. Dãy $(c_m)_{m \geq 0}$ là một hệ cơ sở các lân cận của $0$ trong $A[[X]]^{sym}$.*

Bổ đề hiển nhiên đúng khi $I$ là hữu hạn, do đó ta giả sử rằng $I$ là vô hạn. Với mỗi tập con hữu hạn $J$ của $I$, gồm $m$ phần tử, ký hiệu $\tilde{J}$ là tập các phần tử của $N^{(1)}$ có độ dài $< m$ và có giá trong $J$. Ngoài ra, ký hiệu $a_J'$ là tập các chuỗi lũy thừa hình thức không chứa số hạng nào $aX^\alpha$ với $a \in \tilde{J}$. Vì $\tilde{J}$ là một tập con hữu hạn của $N^{(1)}$ và mọi tập con hữu hạn của $N^{(1)}$ đều được chứa trong một tập có dạng $\tilde{J}$, họ $(a_J')$ là một cơ sở các lân cận của $0$ trong $A[[X]]$ (IV, p. 26). Khi đó Bổ đề 1 suy ra quan hệ $a_J' \cap A[[X]]^{sym} = c_m$ với mọi tập con $J$ có $m$ phần tử, và điều này chứng minh Bổ đề 3.

Vì chỉ có một số hữu hạn đơn thức có một trọng số đã cho trong các $S_k$, nên mọi chuỗi lũy thừa hình thức $f \in B$ có thể được viết theo một cách duy nhất dưới dạng $f = \sum_{r \geq 0} P_r$, trong đó $P_r$ là một đa thức đẳng trọng của trọng số $r$ trong $B \cap A[S]$. Với mỗi số nguyên $m \geq 0$ cho $b_m$ là iđêan của $B$ gồm tất cả các chuỗi lũy thừa hình thức thuộc dạng trên sao cho $P_r = 0$ với $0 \leq r < m$. Dãy $(b_m)_{m \geq 0}$ là một cơ sở các lân cận của $0$ trong $B$.

Với ký hiệu trên, $\psi_1(P_r)$ là một chuỗi lũy thừa hình thức đối xứng trong các $X_i$, thuần nhất bậc $r$, và do đó đây là thành phần thuần nhất bậc $r$ của $\psi_1(f)$. Bổ đề 2 chỉ ra rằng $\psi_1$ là một đồng cấu đại số từ $B$ lên $A[[X]]^{sym}$, ánh xạ $b_m$ vào $c_m$ với mỗi số nguyên $m \geq 0$; khi đó Bổ đề 3 chỉ ra rằng $\psi_1$ là song liên tục, và điều này hoàn tất chứng minh Định lý 2.

### 4. Tổng các lũy thừa

Ta lại viết $X = (X_i)_{i \in I}$ cho một họ các bất định. Các chuỗi lũy thừa hình thức đối xứng $s_k$ được định nghĩa như trước bởi

$$
s_k = \sum_{H \in \mathfrak{P}_k} \prod_{i \in H} X_i \quad (k \geq 1),
$$

trong đó $\mathfrak{P}_k$ là tập hợp tất cả các tập con có k phần tử của $I$. Ta cũng viết

$$
p_k = \sum_{i \in I} X_i^k \quad (k \geq 1)
$$

Đây là một chuỗi lũy thừa hình thức đối xứng, thuần nhất bậc k.

**Bổ đề 4 (« Các hệ thức Newton »).** — *Với mọi số nguyên $d \geq 1$ ta có*

$$
p_d = \sum_{k=1}^{d-1} (-1)^{k-1} s_k p_{d-k} + (-1)^{d+1} d s_d
$$

Định nghĩa một đạo hàm liên tục $A$ trên $\mathbf{A}[[\mathbf{X}]]$ bởi $A(u) = \sum_{n \geq 0} n u_n$, trong đó với mọi $u$ trong $\mathbf{A}[[\mathbf{X}]]$, $u_n$ là thành phần thuần nhất bậc $n$ của $u$. Theo (16) và Mệnh đề 2 của *IV*, p. 27 ta có

$$
1 + \sum_{k \geq 1} s_k = \prod_{i \in I} (1 + X_i)
$$

Theo Mệnh đề 9 của *IV*, p. 34 suy ra

$$
\left( \sum_{k \geq 1} k s_k \right) \cdot \left( 1 + \sum_{k \geq 1} s_k \right)^{-1} = \sum_{i \in I} \Delta(X_i)/(1 + X_i).
$$

Ta có $A(X_i) = X_i$ và $X_i/(1 + X_i) = \sum_{k \geq 1} (-1)^k \ X_i^k$. Vế phải của (20) do đó bằng $\sum_{k \geq 1} (-1)^{k-1} p_k$. Suy ra theo (20) ta có

$$
\sum_{k \geq 1} k s_k = \left( 1 + \sum_{k \geq 1} s_k \right) \cdot \left( \sum_{k \geq 1} (-1)^{k-1} p_k \right)
$$

và nay Bổ đề 4 suy ra từ việc so sánh các thành phần thuần nhất bậc d.

#### Nhận xét {#alg-iv-s6-n4-rem-1 .statement}

— Với ký hiệu của chứng minh trên, ta có

$$
\Delta u = \sum_{i \in I} X_i \cdot D_i(u)
$$

(IV, p. 33, Hệ quả 1). Nói cách khác, *quan hệ Euler (IV, p. 8, Mệnh đề 6)* được mở rộng sang các chuỗi lũy thừa hình thức : nếu $u \in A[X]$ là thuần nhất bậc $n$, thì

(21)
$$
n \cdot u = \sum_{i \in I} X_i \cdot D_i(u) .
$$

Khi I hữu hạn, gồm $n$ phần tử, ta có $s_k = 0$ với $k > n$. Khi đó các hệ thức Newton có thể viết

$$
\begin{aligned}
p_2 &= s_1 p_1 - 2 s_2 \\
p_3 &= s_1 p_2 - s_2 p_1 + 3 s_3 \\
&\ \ \cdots \cdots \cdots \cdots \cdots \cdots \cdots \\
p_{n-1} &= s_1 p_{n-2} - s_2 p_{n-3} + \cdots + (-1)^{n-1} s_{n-2} p_1 + (-1)^n (n-1) s_{n-1} \\
p_n &= s_1 p_{n-1} - s_2 p_{n-2} + \cdots + (-1)^n s_{n-1} p_1 + (-1)^{n+1} n s_n
\end{aligned}
$$

và

(22)
$$
p_k = s_1 p_{k-1} - s_2 p_{k-2} + \cdots + (-1)^{n+1} s_n p_{k-n} \quad (\text{với } k > n) .
$$

N $n$ quan hệ đầu tiên ở trên đúng với mọi $I$ ; chẳng hạn ta có

$$
p_1 = s_1 , \quad p_2 = s_1^2 - 2 s_2 , \quad p_3 = s_1^3 - 3 s_1 s_2 + 3 s_3 .
$$

Tổng quát hơn, cho $S = (S_n)_{n \geq 1}$ là một họ các ẩn. Định nghĩa các đa thức $P_d \in \mathbf{Z}[S_1, \ldots, S_d]$ theo quy nạp bởi $P_1 = S_1$ và

$$
P_d = \sum_{k=1}^{d-1} (-1)^{k-1} S_k P_{d-k} + (-1)^{d+1} d S_d \quad (d \geq 2) .
$$

Khi đó ta có các « công thức phổ quát » $p_d = P_d(s_1, \ldots, s_d)$ đúng trên mọi vành A và mọi họ X các ẩn.
Cho $P = (P_k)_{k \geq 1}$ là một dãy các ẩn. Vì $p_k$ thuần nhất bậc k trong $A[[X]]$, tồn tại duy nhất một đồng cấu đại số trên A liên tục

$$
\lambda_I : A[[P]] \to A[[X]]^{\mathrm{sym}}
$$

sao cho $\lambda_I(P_k) = p_k$ với mọi số nguyên $k \geq 1$ *(IV, p. 28)*. Nếu gán cho $P_k$ trọng số k, thì $\lambda_I$ biến một đa thức đẳng trọng có trọng số $n$ trong các $P_k$ thành một chuỗi lũy thừa hình thức thuần nhất bậc $n$ trong các $X_i$.

#### Mệnh đề 3 {#alg-iv-s6-prop-3 .statement}

— *a) Nếu I là một tập hữu hạn có n phần tử và $n! \cdot 1$ khả nghịch trong A, thì $\lambda_I$ cảm sinh một đẳng cấu hai liên tục từ $A[[P_1, \ldots, P_n]]$ lên $A[[X]]^{\mathrm{sym}}$.*
*b) Nếu I là vô hạn và A là một Q-đại số, thì $\lambda_I$ cảm sinh một đẳng cấu hai liên tục từ $A[[P]]$ lên $A[[X]]^{\mathrm{sym}}$.*
Ta sẽ chỉ xét trường hợp *a)*, còn trường hợp *b)* thì khá tương tự.

Theo Định lý 2 (IV, p. 68) ta có thể đồng nhất $\mathbf{A}[[\mathbf{X}]]^{\text{sym}}$ với đại số các chuỗi lũy thừa hình thức $\mathbf{A}[[S_1, \ldots, S_n]]$, với $S_k$ tương ứng với $s_k$. Theo Bổ đề 4 của *IV*, p. 70, tồn tại các chuỗi lũy thừa hình thức $g_1, \ldots, g_s$ có cấp $\geq 2$ trong các ẩn $s_1, \ldots, s_n$ sao cho

$$
p_k = (-1)^{k+1} k s_k + g_k(s_1, \ldots, s_s) \quad (1 \leq k \leq n).
$$

Vì $k! . 1$ là khả nghịch trong $\mathbf{A}$, Bổ đề 2 của IV, p. 35 chứng minh sự tồn tại của một tự đẳng cấu $T$ của $\mathbf{A}$-đại số tôpô $\mathbf{A}[[\mathbf{X}]]^{\text{sym}}$ biến $s_k$ thành $p_k$ với $l \leq k \leq n$. Khi đó Mệnh đề 3, $a)$ là một hệ quả ngay lập tức.

#### Hệ quả {#alg-iv-s6-n4-cor-1 .statement}

— *Cho $\xi_1, \ldots, \xi_n, \eta_1, \ldots, \eta_n$ là các phần tử của $\mathbf{A}$ và giả sử rằng $\mathbf{A}$ là một miền nguyên.*

$a)$ *Nếu $s_k(\xi_1, \ldots, \xi_n) = s_k(\eta_1, \ldots, \eta_n)$ với $1 \leq k \leq n$, thì tồn tại một phép hoán vị $\sigma \in \mathfrak{S}_n$ sao cho $\eta_i = \xi_{\sigma(i)}$ với $1 \leq i \leq n$.*

$b)$ *Giả sử rằng $n! . 1 \neq 0$ trong $\mathbf{A}$ và*

$$
\xi_1^k + \cdots + \xi_n^k = \eta_1^k + \cdots + \eta_n^k
$$

với $1 \leq k \leq n$. *Khi đó tồn tại một phép hoán vị $\sigma \in \mathfrak{S}_n$ sao cho $\eta_i = \xi_{\sigma(i)}$ với $1 \leq i \leq n$.*

Dưới các giả thiết $a)$ ta có $\prod_{i=1}^n (X - \xi_i) = \prod_{i=1}^n (X - \eta_i)$. Nếu ta thay $\eta_n$ vào $X$, ta thấy rằng $\prod_{i=1}^n (\eta_n - \xi_i) = 0$ và vì $\mathbf{A}$ là một miền nguyên, tồn tại một số nguyên $\sigma(n)$ sao cho $l \ s \ \sigma(n) \leq n$ và $\eta_n = \xi_{\sigma(n)}$. Bây giờ mệnh đề $a)$ suy ra dễ dàng bằng quy nạp vì $\mathbf{A}[X]$ là một miền nguyên.

Dưới các giả thiết của $b)$, theo Mệnh đề 3 tồn tại các đa thức $\Pi_1, \ldots, \Pi_n$ theo $n$ bất định, với các hệ số trong trường các phân thức của $\mathbf{A}$ sao cho $s_k = \Pi_k(p_1, \ldots, p_n)$ với $1 \leq k \leq n$. Khi đó quan hệ (23) suy ra

$$
s_k(\xi_1, \ldots, \xi_n) = s_k(\eta_1, \ldots, \eta_n)
$$

với $1 \leq k \leq n$ và do đó $b)$ suy ra từ $a)$.

### 5. Các hàm đối xứng trong các nghiệm của một đa thức

Xét một đa thức đơn khởi bậc $n$, với các hệ số trong $\mathbf{A}$:

$$
f = X^n + a_1 X^{n-1} + \cdots + a_{n-1} X + a_n.
$$

Ta định nghĩa một $\mathbf{A}$-đại số kết hợp, giao hoán và có đơn vị $E_f$ với các phần tử sinh $x_1, \ldots, x$, và các quan hệ

$$
\sum_{i_1 < \ldots < i_k} x_{i_1} \ldots x_{i_k} = (-1)^k a_k \quad (1 \leq k \leq n).
$$

Chính xác hơn, ta có

$$
E_f = A[X_1, ..., X_n]/a
$$

trong đó iđêan $a$ được sinh bởi các đa thức $s_k + (-1)^{k+1} a_k$ với $1 \leq k \leq n$, và $x_i$ là lớp thặng dư của $X_i$ mod $a$ với $1 \leq i \in n$. Hệ thức (24) cũng tương đương với $f(X) = \prod_{i=1}^n (X - x_i)$. Khi có nguy cơ mơ hồ, ta viết $x_{1,f}, ..., x_{n,f}$ thay cho $x_1, ..., x_n$.

#### Mệnh đề 4 {#alg-iv-s6-prop-4 .statement}

*Cho B là một vành giao hoán, $\rho$ một đồng cấu của A vào B và $\xi_1, ..., 5$, là các phần tử của B. Giả sử rằng hệ thức $^\rho f(X) = \prod_{i=1}^n (X - \xi_i)$ đúng trong B[X]. Khi đó tồn tại một và chỉ một đồng cấu vành $u : E_f \to B$ sao cho $\rho(a) = u(a . 1)$ với mọi $a \in A$ và $u(x_i) = \xi_i$ với $1 \leq i \leq n$.

Ta xét B như một A-đại số kết hợp, giao hoán và có đơn vị thông qua $\rho$. Khi đó hệ thức $^\rho f(X) = \prod_{i=1}^n (X - \xi_i)$ cũng có thể được viết dưới dạng

$$
\sum_{i_1 < ... < i_k} \xi_{i_1} ... \xi_{i_k} = (-1)^k a_k . 1 \quad (1 \leq k \leq n)
$$

trong B. Vì các hệ thức (24) định nghĩa một phép trình bày của $E_f$, Mệnh đề 4 suy ra.

Mệnh đề 4 biện minh cho tên gọi « đại số phân tích phổ quát của $f$ » cho $E_f$. Hệ thức $f(X) = \prod_{i=1}^n (X - x_{i,f})$ được gọi là « phân tích phổ quát của $f$ ». Cho $\sigma \in S_n$ là một phép hoán vị ; vì $f(X) = \prod_{i=1}^n (X - x_{\sigma(i),f})$, tồn tại một tự đẳng cấu $t_\sigma$ của A-đại số $E_f$ được xác định bởi $t_\sigma(x_{i,f}) = x_{\sigma(i),f}$ với $1 \leq i \leq n$. Ta có $t_{\sigma \tau} = t_\sigma \circ t_\tau$ với $\sigma, \tau$ trong $S_n$, và do đó thu được một tác động của nhóm $\mathcal{G}$, lên A-đại số $E_f$.

#### Mệnh đề 5 {#alg-iv-s6-prop-5 .statement}

*Trong đại số phân tích phổ quát $E_f$ họ các đơn thức $x_1^{\nu(1)} ... x_n^{\nu(n)}$ sao cho $0 \leq \nu(i) < i$ với $1 \leq i \leq n$ là một cơ sở của A-môđun $E_f$. Đặc biệt $E_f$ là một A-môđun tự do hạng $n!$.

Đặt $B = A[X_1, ..., X_n]$ và $C = A[X_1, ..., X_n]^{\text{sym}}$. Theo Định lý 1 (*IV*, p. 62) ta có $C = A[s_1, ..., s_n]$ và $s_1, ..., s_n$ độc lập đại số trên A. Các đa thức không có số hạng hằng trong $s_1, ..., s_n$ tạo thành một iđêan $C^+$ trong C, bổ sung cho A và được sinh bởi $s_1, ..., s_n$. Gọi c là iđêan của C được sinh bởi $s_1 + a,, s_2 - a,, ..., s_n + (-1)^n + 'a,.$ Tồn tại một tự đẳng cấu A-đại số của C ánh xạ $s_k$ thành $s_k + (-1)^{k+1} a_k$ với $1 \leq k \leq n$, và do đó ánh xạ $C^+$ lên c ; vì thế ta có $C = A \oplus c$. Hơn nữa Định lý 1, c) của *IV*, p. 62 cho thấy rằng

$$
B = \bigoplus_{\nu \in S} CX^\nu
$$

trong đó S là tập hợp tất cả $v \in \mathbf{N}^n$ sao cho $0 \leq v(i) < i$ với $1 \leq i \leq n$. Iđêan a của B được sinh bởi c, do đó $a = Bc = \bigoplus_{v \in S} c \cdot X^v$. Vì $C = A \oplus c$, ta có
$$
B = a \oplus \bigoplus_{v \in S} AX^v,
$$
do đó theo Mệnh đề 5, vì $E_f = B/a$.

#### Hệ quả {#alg-iv-s6-n5-cor-1 .statement}

— *Đồng cấu chính tắc của A vào đại số phân tích phổ quát của đa thức đơn khởi $f \in A[X]$ là đơn ánh.*

Vì phần tử đơn vị của $E_f$ là một phần của một cơ sở của A-môđun $E_f$.

#### Mệnh đề 6 {#alg-iv-s6-prop-6 .statement}

— *Cho $f \in A[X]$ là một đa thức đơn khởi bậc n, và cho P là một đa thức đối xứng theo $X_1, ..., X_n$ với hệ số trong A. Khi đó tồn tại duy nhất một phần tử a của A có tính chất sau:
(FS) Với mọi đồng cấu vành $\rho : A \to B$ và phân tích $^0f(X) = \prod_{i=1}^n (X - \xi_i)$ trong B[X] ta có $\rho(a) = P(\xi_1, ..., \xi_n)$.*

Viết $f = X^n + \sum_{k=1}^n a_k X^{n-k}$, thì theo ĐL. 1, IV, p. 62 tồn tại một đa thức $\Pi$ theo n biến với hệ số trong A, sao cho $P = \Pi(s_1, ..., s_n)$. Đặt $a = \Pi(-a_1, a,, ..., (-1)^n a_n)$. Dưới giả thiết (FS) ta có
$$
s_k(\xi_1, ..., \xi_n) = (-1)^k \rho(a_k)
$$
do đó
$$
\begin{align*}
\rho(a) &= \Pi(-\rho(a_1), \rho(a_2), ..., (-1)^n \rho(a_n)) \\
&= \Pi(s_1(\xi_1, ..., \xi_n), ..., s_n(\xi_1, ..., \xi_n)) \\
&= P(\xi_1, ..., \xi_n) .
\end{align*}
$$

Điều này chứng minh sự tồn tại của một phần tử a thỏa mãn (FS). Tính duy nhất của a suy ra từ Hệ quả của Mệnh đề 5, vì ta có $a \cdot 1 = P(x_{1,f}, ..., x_{n,f})$ trong đại số phân tích phổ quát $E_f$.

Với ký hiệu của Mệnh đề 6, đôi khi người ta viết $a = P^*(f)$. Sau đây là một vài ví dụ.

*Ví dụ. — 1) Nếu $P = s_k$, thì $P^*(f) = (-1)^k a_k$.
\* 2) Cho g là một đa thức trong $A[X]$ và đặt
$$
P(X_1, ..., X_n) = g(X_1) ... g(X_n) .
$$
Khi đó $P^*(f)$ chính là kết thức $\operatorname{res}(f, g)$, theo Hệ quả 1 của IV, p. 80.
3) Đặt $A(X_1, ..., X_n) = \prod_{i < j} (X_i - X_j)^2$, thì $\Delta^*(f)$ chính là biệt thức của đa thức đơn khởi $f$ (IV, p. 82, công thức (46)). \*

4) Đặt $P(X_1, \ldots, X_n) = X_1^k + \ldots + X_n^k$; hơn nữa, định nghĩa đại số $E = A[X]/(f)$ và viết $x$ cho ảnh của $X$ trong $E$. Nhớ rằng A-môđun $E$ là tự do, với cơ sở $(1, x, \ldots, x^{n-1})$ (IV, p. 11, Hệ quả). Ta hãy chứng minh

$$
\text{Tr}_{E/A}(x^k) = P^*(f)
$$

Đặt $\pi_k = \text{Tr}_{E/A}(x^k)$ với mọi số nguyên $k \geq 1$. Nhớ các hệ thức Newton (IV, p. 70) ta chỉ cần thiết lập các hệ thức

$$
\begin{align*}
&\pi_k + a_1 \pi_{k-1} + \cdots + a_{k-1} \pi_1 + k a_k = 0 \quad \text{cho } 1 \leq k \leq n \\
&\pi_k + a_1 \pi_{k-1} + \cdots + a_{n-1} \pi_{k-n+1} + a_n \pi_{k-n} = 0 \quad \text{cho } k > n
\end{align*}
$$

(mà ta cũng sẽ gọi là « Newton's relations »). Hệ thức (27) là rõ ràng, vì vế trái là vết của

$$
x^{k-n}(x^n + a_1 x^{n-1} + \cdots + a_{n-1} x + a_n) = 0 .
$$

Giả sử rằng $1 \leq k \leq n$ và đặt

$$
y = x^k + a_1 x^{k-1} + \cdots + a_{k-1} x + a_k \cdot 1 ;
$$

gọi $M = (m_{ij})$ là ma trận của ánh xạ tuyến tính $u \mapsto yu$ trong $E$ theo cơ sở $(x')_{0,\ldots,n}$. Ta dễ dàng thu được các hệ thức

$$
\begin{align*}
&m_{ii} = a_k \quad \text{cho } 0 \leq i < n - k \\
&m_{ii} = 0 \quad \text{cho } n - k \leq i < n ,
\end{align*}
$$

do đó

$$
\text{Tr}_{E/A}(y) = \sum_{i=0}^{n-1} m_{ii} = (n-k) a_k .
$$

Hơn nữa ta có

$$
\text{Tr}_{E/A}(y) = \pi_k + a_1 \pi_{k-1} + \cdots + a_{k-1} \pi_1 + n a_k ,
$$

do đó suy ra công thức (26).

### 6. Kết thức

Trong mục này, ta giả sử cho trước hai số nguyên dương $p, q$ và hai đa thức $f, g$ trong $A[X]$ có dạng

$$
\begin{align*}
f &= t_p X^p + t_{p-1} X^{p-1} + \cdots + t_0 \\
g &= u_q X^q + u_{q-1} X^{q-1} + \cdots + u_0
\end{align*}
$$

sao cho $\deg f \leq p, \deg g \leq q$. Với mọi số nguyên $n \geq 0$ ta ký hiệu bởi $S$, môđun con $A$-của $A[X]$ gồm tất cả các đa thức có bậc $< n$; nó có họ $(X')_{0 \leq i < n}$ làm cơ sở, và do đó có hạng $n$.

Ta trang bị $S, \times S_p$ với cơ sở
$$
B_1 = ((X^{q-1}, 0), ..., (X, 0), (1, 0), (0, X^{p-1}), ..., (0, X), (0, 1))
$$
và $S_{p+q}$ với cơ sở
$$
B_2 = (X^{p+2-1}, ..., X, 1).
$$
Ta định nghĩa một ánh xạ tuyến tính $\varphi : S, \times S_p \to S_{p+q}$ bởi
$$
\varphi(u, v) = uf + vg
$$
và ta ký hiệu bởi $M(f, g, p, q)$ ma trận của $\varphi$ đối với các cơ sở $B_1$ và $B_2$. Đây là một ma trận vuông cấp $p + q$, được đánh chỉ số bởi tập hợp $\{0, 1, ..., p + q - 1\}$. Các phần tử $a_{ij}$ của nó được cho bởi các quy tắc:
a) $a_{ij} = t_{p-i+j}$ với $0 \leq j \leq q-1$,
b) $a_{ij} = u_{j-i}$ với $q \leq j \leq p + q - 1$,
trong đó $t_k$ được lấy bằng 0 nếu $k \notin (0, p)$ và $u_k = 0$ nếu $k \notin (0, q)$.

Ví dụ, khi $p = 2$ và $q = 3$, ta có ma trận
$$
\begin{pmatrix}
t_2 & 0 & 0 & u_3 & 0 \\
t_1 & t_2 & 0 & u_2 & u_3 \\
t_0 & t_1 & t_2 & u_1 & u_2 \\
0 & t_0 & t_1 & u_0 & u_1 \\
0 & 0 & t_0 & 0 & u_0
\end{pmatrix}.
$$

#### Định nghĩa 1 {#alg-iv-s6-def-1 .statement}

*Với ký hiệu trên, định thức của ma trận $M(f, g, p, q)$ được gọi là định thức resultant của cặp $(f, g)$ đối với các bậc $p$ và $q$, hoặc đơn giản là resultant của $f$ và $g$ nếu $p = \deg f$ và $q = \deg g$.*

Resultant được ký hiệu bởi $\operatorname{res}_{p,q}(f, g)$ hoặc đơn giản là $\operatorname{res}(f, g)$ khi $p = \deg f$, $q = \deg g$.

#### Ví dụ 1 {#alg-iv-s6-n6-exa-1 .statement}

Cho $\Lambda, \mu$ trong $\Lambda$, ta có các công thức
$$
\operatorname{res}_{p,0}(f, \lambda) = \lambda^p, \quad \operatorname{res}_{0,q}(\mu, g) = \mu^q
$$
$$
\operatorname{res}_{p,1}(f, \lambda) = \lambda^p t_p, \quad \operatorname{res}_{1,q}(\mu, g) = (-1)^q \mu^q u_q,
$$
mà chứng minh là ngay lập tức.

#### Ví dụ 2 {#alg-iv-s6-n6-exa-2 .statement}

Khi $p = q = 1$, ta có
$$
\operatorname{res}_{1,1}(t_1 X + t_0, u_1 X + u_0) = t_1 u_0 - t_0 u_1
$$

#### Nhận xét 1 {#alg-iv-s6-n6-rem-1 .statement}

Ma trận $M(g, f, q, p)$ nhận được từ $M(f, g, p, q)$ bằng $pq$ phép chuyển vị các cột, do đó
$$
\operatorname{res}_{q,p}(g, f) = (-1)^{pq} \operatorname{res}_{p,q}(f, g)
$$

#### Nhận xét 2 {#alg-iv-s6-n6-rem-2 .statement}

Cho $\rho : A \to B$ là một đồng cấu vành. Định nghĩa / suy ra trực tiếp công thức
$$
\operatorname{res}_{p,q}(\rho f, \rho g) = \rho(\operatorname{res}_{p,q}(f, g)) .
$$

#### Nhận xét 3 {#alg-iv-s6-n6-rem-3 .statement}

Cho $\lambda, \mu$ trong $A$, ta có
$$
\operatorname{res}_{p,q}(\lambda f, \mu g) = \lambda^q \mu^p \operatorname{res}_{p,q}(f, g) .
$$
(28)

#### Nhận xét 4 {#alg-iv-s6-n6-rem-4 .statement}

Giả sử rằng $p + q \geq 1$. Theo III, p. 532, công thức (28), ảnh của $\varphi$ chứa đa thức hằng $\operatorname{res}_{p,q}(f, g)$. Do đó tồn tại một cặp đa thức $(u, v)$, với $u \in S_q, v \in S_p$ sao cho
$$
\operatorname{res}_{p,q}(f, g) = uf + vg ,
$$
do đó
$$
\operatorname{res}_{p,q}(f, g) \in A \cap (f, g) .
$$
Cặp $(u, v)$ này là duy nhất khi $\operatorname{res}_{p,q}(f, g)$ giản ước được trong $A$: vì khi đó $\varphi$ là đơn ánh (III, p. 524, Mệnh đề 3).

#### Nhận xét 5 {#alg-iv-s6-n6-rem-5 .statement}

Giả sử rằng $p \geq q$, và cho $h \in A[X]$ là một đa thức bậc $\leq p - q$. Ta chứng minh rằng
$$
\operatorname{res}_{p,q}(f, g) = \operatorname{res}_{p,q}(f + gh, g) .
$$
(29)
Vì nếu ta viết $\omega(u, v) = (u, uh + v)$ cho $(u, v) \in S_q \times S_p$, thì $w$ là một tự đẳng cấu của $A$-môđun $S_q \times S_p$ và ta có
$$
\omega^{-1}(u, v) = (u, -uh + v) .
$$
Ma trận của $w$ đối với cơ sở $B_1$ là tam giác dưới và các phần tử trên đường chéo của nó đều bằng $l$. Mặt khác, $\varphi \circ w$ ánh xạ $(u, v)$ thành $u(f + gh) + vg$. Bây giờ công thức (29) có nghĩa là các ma trận biểu diễn $\varphi$ và $\varphi \circ w$ có cùng định thức và điều này suy ra từ quan hệ $\det w = l$.

Giả sử $f$ là đơn thức bậc $p$; đặt $E = A[X]/(f)$ và ký hiệu bởi $x$ ảnh chính tắc của $X$ trong $E$. Ta biết (IV, p. 11) rằng $E$ là một $A$-môđun tự do với cơ sở $(1, x, \ldots, x^{p-1})$. Do đó ta có thể định nghĩa chuẩn $N_{E/A}(u)$ của mọi phần tử $u$ của $E$ (III, p. 543, Định nghĩa 2).

#### Mệnh đề 7 {#alg-iv-s6-prop-7 .statement}

— *Giả sử f là đơn thức bậc p; với các ký hiệu trên ta có*¹
$$
\operatorname{res}_{p,q}(f, g) = N_{E/A}(g(x)) .
$$
(30)

¹ Kết quả thức $\operatorname{res}_{p,q}(f, g)$ do đó không phụ thuộc vào $q$ khi $f$ là đơn thức bậc $p$. Sau đó ta chỉ ký hiệu nó là $\operatorname{res}(f, g)$.

Hãy định nghĩa một ánh xạ A-tuyến tính $0$ từ $S_q \times S_p$ vào $S_{p+q}$ bởi $\theta(u, v) = uf + v$. Khi đó $0$ đưa cơ sở $B_1$ của $S_q \times S_s$ vào dãy
$$
(fX^{q-1}, \ldots, fX, f, X^{p-1}, \ldots, X, 1)
$$
các phần tử của $S_{p+q}$; do đó ma trận $M$, của $0$ theo các cơ sở $B_1, B_2$ là tam giác dưới và các phần tử đường chéo của nó đều bằng 1, suy ra $\det M = 1$.

Suy ra rằng $\theta$ là song ánh và $\operatorname{res}_{p,q}(f, g)$ bằng định thức của tự đồng cấu $\varphi' = \varphi \circ \theta^{-1}$ của $S_{p-q}$. Tường minh, ta có
$$
\varphi'(uf + v) = uf + vg
$$
với mọi cặp $(u, v)$ trong $S_q \times S_s$. Bây giờ ta có $A[X] = S_{p+q} + (f)$ và $fS_q = S_s \cap (f)$, do đó đơn ánh chính tắc của $S_{p-s}$ vào $A[X]$ xác định bằng phép đi qua thương một đẳng cấu $\gamma$ của $S_{p+q}/fS_q$ lên E. Ký hiệu $\psi$ là phép nhân với $g(x)$ trong E. Công thức (31) cho thấy rằng $\varphi'$ cảm sinh đồng nhất trên $fS_q$ và $\gamma^{-1}\psi\gamma$ trên $S_{p+q}/fS_q$. Vậy ta có $\det \varphi' = \det \psi$, do đó (30) suy ra, vì $\det \varphi' = \operatorname{res}_{p,q}(f, g)$ và $\det \psi = N_{E/A}(g(x))$, theo định nghĩa.

#### Hệ quả 1 {#alg-iv-s6-prop-7-cor-1 .statement}

— Cho $f \in A[X]$ là một đa thức đơn khởi; với mọi đa thức $g \in A[X]$ các điều kiện sau là tương đương:
(i) $\operatorname{res}(f, g)$ khả nghịch trong $A$;
(ii) tồn tại các đa thức $u, v$ trong $A[X]$ sao cho $uf + vg = 1$;
(iii) $g(x)$ khả nghịch trong đại số $A[X]/(f)$.
Sự tương đương giữa (i) và (iii) chỉ là bản dịch của Hệ quả 1, theo Định nghĩa 1 của III, p. 545 và Mệnh đề 7; sự tương đương giữa (ii) và (iii) là hiển nhiên.

#### Hệ quả 2 {#alg-iv-s6-prop-7-cor-2 .statement}

— Giả sử rằng $A$ là một trường và cho $f, g \in A[X]$, khi đó các điều kiện sau là tương đương khi $f, g$ khác 0:
(i) $\operatorname{res}(f, g) \neq 0$;
(ii) các đa thức $f$ và $g$ nguyên tố cùng nhau trong $A[X]$;
\* (iii) với mọi mở rộng L của A, các đa thức $f$ và $g$ không có nghiệm chung trong L. \*

Ta có thể rút gọn ngay về trường hợp $f$ là đơn khởi (IV, p. 77, nhận xét 3).
Sự tương đương giữa (i) và (ii) chỉ là bản dịch của Hệ quả 1, theo Định nghĩa 1 của IV, p. 12; sự tương đương giữa (ii) và (iii) chỉ là Hệ quả 7 của IV, p. 13.

#### Hệ quả 3 {#alg-iv-s6-prop-7-cor-3 .statement}

— Với mọi $\lambda \in A$ ta có
$$
\operatorname{res}_{p,1}(f, \lambda - X) = f(\lambda), \quad \operatorname{res}_{1,q}(X - \lambda, g) = g(\lambda).
$$
Khi $f(X) = X - \lambda$, đại số E bằng A và ta có $x = A$; công thức thứ hai (32) nay suy ra từ Mệnh đề 7 (IV, p. 77). Theo các nhận xét 1 và 3 (IV, p. 76, 77) ta kết luận
$$
\operatorname{res}_{p,1}(f, \lambda - X) = (-1)^p \operatorname{res}_{1,p}(\lambda - X, f) = (-1)^{p+p} \operatorname{res}_{1,p}(X - A, f) = f(A).
$$

Giả sử bây giờ rằng f và g là các đa thức đơn khởi. Ta ký hiệu F là A-đại số $A[X, Y]/(f(X), g(Y))$ và ký hiệu x (resp. y) là ảnh chính tắc của X (resp. Y) trong F.

#### Mệnh đề 8 {#alg-iv-s6-prop-8 .statement}

— Giả sử rằng f và g là đơn nhất có bậc tương ứng là p và q. Với ký hiệu trên, A-môđun F là tự do với cơ sở $(x^i y^j)_{0 \leq i < p,\ 0 \leq j < q}$ và ta có

$$
\text{res}(f, g) = N_{F/A}(x - y).
$$

Đặt $E = A[X]/(f)$ và $E' = A[Y]/(g)$. Theo II, p. 253, Hệ quả 1, đồng cấu $\sigma$ của $E @ E'$ vào F dẫn xuất từ đồng cấu chính tắc $A[X] \otimes A[Y] \to A[X, Y]$ là song ánh; điều này chứng minh mệnh đề về cơ sở của F. Bây giờ ta đồng nhất E với ảnh của nó trong F qua $\sigma$. Khi đó đồng cấu đại số E của $E[Y]/(g(Y))$ vào F biến Y thành y là một đẳng cấu.

Theo tính bắc cầu của chuẩn (III, p. 546), ta có

$$
N_{F/A}(x - y) = N_{E/A}(N_{F/E}(x - y)).
$$

Theo Mệnh đề 7 (IV, p. 77), $N_{F/E}(x - y)$ là resultant của các đa thức g(Y) và x − Y trong E[Y], do đó bằng g(x) (IV, p. 78, Hệ quả 3). Theo công thức (34) và Mệnh đề 7 (IV, p. 77), ta có

$$
N_{F/A}(x - y) = N_{E/A}(g(x)) = \text{res}(f, g)
$$

#### Mệnh đề 9 {#alg-iv-s6-prop-9 .statement}

— Cho $p_1$ và $q_1$ là các số nguyên dương và $f_1, g_1$ là các đa thức trong $A[X]$ sao cho $\deg f_1 \leq p_1, \deg g_1 \leq q_1$; khi đó ta có

$$
\text{res}_{p, q + q_1}(f, gg_1) = \text{res}_{p, q}(f, g) \cdot \text{res}_{p, q_1}(f, g_1)
$$
$$
\text{res}_{p + p_1, q}(ff_1, g) = \text{res}_{p, q}(f, g) \cdot \text{res}_{p_1, q}(f_1, g).
$$

Ta có $\text{res}_{p, q}(f, g) = (-1)^{pq} \text{res}_{q, p}(g, f)$ (IV, p. 76); vì vậy chỉ cần chứng minh (35). Tương tự, Nhận xét 3 (tại chỗ đã dẫn) cho thấy rằng nếu công thức (35) được thiết lập cho một đa thức $f$, thì nó đúng với mọi đa thức dạng Af, trong đó $A \in A$. Cuối cùng, khi f là đơn nhất có bậc p, công thức (35) suy ra từ Mệnh đề 7 (IV, p. 77) bởi công thức $N_{E/A}(ab) = N_{E/A}(a) \cdot N_{E/A}(b)$. Tóm lại ta kết luận rằng (35) đúng khi hệ số $t_p$ của $X^p$ trong f là khả nghịch.

#### Bổ đề 5 {#alg-iv-s6-lem-5 .statement}

Cho t là một phần tử của A. Tồn tại một vành giao hoán C chứa A như vành con, một vành con B của C chứa A, một phần tử $\tau$ của B khả nghịch trong C và một đồng cấu vành $p : B \to A$ sao cho $p(\tau) = t$ và hạn chế của p trên A bằng Id.

Chỉ cần lấy B là đại số $A^{(\mathbf{N})}$ của monoid $\mathbf{N}$, nghĩa là đại số đa thức $A[\tau]$ theo một biến không xác định $\tau$, lấy C là đại số $A^{(\mathbf{Z})}$ của nhóm $\mathbf{Z}$ và lấy p là đồng cấu $P \mapsto P(t)$ của $A(\tau)$ vào A.

Với ký hiệu của Bổ đề 5, trong đó ta đã lấy t = t_p, đặt
$$
F = \tau X^p + t_{p-1} X^{p-1} + \cdots + t_1 X + t_0
$$
trong B[X]. Hệ số của $X^p$ trong F là khả nghịch trong C; nếu ta xét F, g, $g_1$ như các đa thức của C[X] thì ta có
$$
\operatorname{res}_{p,q+q_1}(F, gg_1) = \operatorname{res}_{p,q}(F, g) \cdot \operatorname{res}_{p,q_1}(F, g_1)
$$
theo điều đã nói. Các resultant không thay đổi nếu ta xét F, g và $g_1$ như các đa thức trong B[X]. Vì $^\rho F = f$, $^\rho g = g$, $^\rho g_1 = g_1$, công thức (35) suy ra từ (38) và Nhận xét 2 (IV, p. 77).

#### Hệ quả 1 {#alg-iv-s6-lem-5-cor-1 .statement}

— (i) Cho $\lambda, a,, \ldots, \alpha_p$ là các phần tử của A và giả sử rằng $f(X) = \lambda (X - a,) \ldots (X - a,)$. Ta có
$$
\operatorname{res}_{p,q}(f, g) = \lambda^q g(\alpha_1) \ldots g(\alpha_p) .
$$
(ii) Cho $\mu, \beta_1, \ldots, \beta_q$ là các phần tử của A và giả sử thêm rằng $g(X) = \mu (X - \beta_1) \ldots (X - \beta_q)$. Khi đó ta có
$$
\operatorname{res}_{p,q}(f, g) = \lambda^q \mu^p \prod_{\substack{1 \leq i \leq p \\ 1 \leq j \leq q}} (\alpha_i - \beta_j) .
$$
Mệnh đề (i) suy ra trực tiếp từ các công thức (28), (32) và (36). Bây giờ Mệnh đề (ii) suy ra từ (i).

#### Hệ quả 2 {#alg-iv-s6-lem-5-cor-2 .statement}

— Với mọi số nguyên $r \geq 0$ ta có
$$
\operatorname{res}_{p,q+r}(f, g) = t_p^r \cdot \operatorname{res}_{p,q}(f, g) .
$$
Ghi nhớ Ví dụ 1 (IV, p. 76), ta chỉ cần lấy $q_1 = r, g_1 = 1$ trong (35).

Giả sử rằng f là đơn nhất, và cho $\rho : A \to B$ là một đồng cấu vành và $\xi_1, \ldots, \xi_p$ là các phần tử của B sao cho ta có phân tích
$$
^\rho f(X) = (X - \xi_1) \ldots (X - \xi_p)
$$
Theo Nhận xét 2 (IV, p. 77) và Hệ quả 1 ở trên, ta có
$$
\rho(\operatorname{res}(f, g)) = g(\xi_1) \ldots g(\xi_p)
$$
Nhận xét này áp dụng đặc biệt cho phân tích phổ quát của f (IV, p. 73) và vì khi đó $\rho$ là đơn ánh, điều này cung cấp một phương tiện để tính $\operatorname{res}(f, g)$.

#### Ví dụ 3 {#alg-iv-s6-n6-exa-3 .statement}

Ta hãy chứng minh công thức
$$
\operatorname{res}_{2,2}(aX^2 + bX + c, a'X^2 + b'X + c') =
(ac' - ca')^2 + (bc' - cb')(ba' - ab')
$$

Lập luận như đối với Mệnh đề 9 (IV, p. 79), ta thấy rằng chỉ cần chứng minh công thức khi $a$ khả nghịch. Khi đó tồn tại một phân tích có dạng

$$
aX^2 + bX + c = a(X - x)(X - y)
$$

trong $B[X]$, trong đó $B$ là một vành thích hợp chứa $A$ như vành con. Theo Hệ quả 1 ở trên, resultant cần tìm bằng

$$
R = a^2(a'x^2 + b'x + c')(a'y^2 + b'y + c') .
$$

Bây giờ ta có

$$
ax + ay = -b , \quad axy = c
$$

theo (43), do đó $(ax)^2 + (ay)^2 = b^2 - 2ac$.

Theo (44) ta có

$$
R = {a'}^2(axy)^2 + {ab'}^2(axy) + a^2{c'}^2 + a'b'(axy)(ax + ay) +
$$
$$
+ a'c'((ax)^2 + (ay)^2) + ab'c'(ax + ay)
$$
$$
= {a'}^2c^2 + {ab'}^2c + a^2{c'}^2 - a'b'cb + a'c'(b^2 - 2ac) - ab'c'b
$$
$$
= (ac' - ca')^2 + (ab' - a'b)(b'c - c'b) ,
$$

từ đó suy ra kết quả cần chứng minh.

### 7. Biệt thức

#### Định nghĩa 2 {#alg-iv-s6-def-2 .statement}

*Cho $f$ là một đa thức đơn khởi của $A[X]$ có bậc $m$, và ký hiệu $E$ là $A$-đại số $A[X]/(f)$ và $x$ là ảnh chính tắc của $X$ trong $E$. Ta định nghĩa biệt thức của $f$, ký hiệu $\operatorname{dis}(f)$, là biệt thức $D_{E/A}(1, x, \ldots, x^{m-1})$ của cơ sở $(1, x, \ldots, x^{m-1})$ của $A$-đại số $E$.*

Với mọi số nguyên dương $k$, ta viết $\rho_k = \operatorname{Tr}_{E/A}(x^k)$. Theo III, p. 549, Định nghĩa 2 tương đương với công thức

$$
\operatorname{dis}(f) = \det(p_{i+j})_{0 \leq i,j < m}
$$

*Ví dụ. — 1) Nếu $f$ là một đa thức đơn khởi có bậc 0 hoặc 1, ta có $\operatorname{dis}(f) = 1$, theo (45).
2) Cho $f(X) = X^2 + \alpha X + \beta$ là một đa thức đơn khởi có bậc 2. Các hệ thức Newton có thể được viết dưới dạng (IV, p. 75)

$$
p_0 = 2 \\
p_1 + \alpha = 0 \\
p_2 + \alpha p_1 + 2\beta = 0 ,
$$

do đó $p_1 = -a$, $p_2 = a^2 - 2p$. Suy ra rằng ta có

$$
\operatorname{dis}(f) = \det \begin{pmatrix} 2 & -\alpha \\ -a & \alpha^2 - 2p \end{pmatrix} = \alpha^2 - 4\beta
$$

Cho B là một vành giao hoán, $\rho$ là một đồng cấu từ A đến B và $\xi_1, \ldots, \xi_m$ là các phần tử của B sao cho
$$
\rho f(X) = (X - \xi_1) \cdots (X - \xi_m).
$$
Ta ký hiệu M là ma trận $(\rho(p_{i + j}))_{0 \leq i, j < m}$ và D là ma trận Van der Monde $(\xi_i^{j+1})_{0 \leq i, j < m}$. Theo Ví dụ 4 của IV, p. 75 ta có
$$
\rho(p_k) = \xi_1^k + \cdots + \xi_m^k,
$$
do đó $M = 'D . D ;$ theo III, p. 532 ta có $D = \prod_{i > j} (\xi_i - \xi_j)$ và $\det M = (\det D)^2$, nghĩa là
$$
\rho(\operatorname{dis}(f)) = \prod_{i < j} (\xi_i - \xi_j)^2
$$
Hơn nữa (bằng cách ký hiệu D là đạo hàm $\frac{d}{dX}$) ta có
$$
D(\rho f)(\xi_i) = (\xi_i - \xi_1) \cdots (\xi_i - \xi_{i-1})(\xi_i - \xi_{i+1}) \cdots (\xi_i - \xi_m)
$$
với $1 \leq i \leq m$, do đó
$$
\rho(\operatorname{dis}(f)) = (-1)^{m(m-1)/2} \prod_{i \neq j} (\xi_i - \xi_j) = (-1)^{m(m-1)/2} \prod_{i=1}^m D(\rho f)(\xi_i).
$$
Theo Hệ quả 1 của IV, p. 80 áp dụng cho phân tích phổ quát của $f$, cuối cùng ta thu được
$$
\operatorname{res}(f, Df) = \operatorname{res}(Df, f) = (-1)^{m(m-1)/2} \operatorname{dis}(f).
$$

#### Mệnh đề 10 {#alg-iv-s6-prop-10 .statement}

Cho $m \geq 1$. Tồn tại duy nhất một đa thức $A \in \mathbf{Z}[A,, \ldots, A,_j]$ với tính chất sau : với mọi vành giao hoán A và đa thức *đơn nhất* $f = X^m + \sum_{i=1}^m a_i X^{m-i}$ trong $A[X]$ ta có
$$
\operatorname{dis}(f) = \Delta(a_1, \ldots, a_m).
$$
Hơn nữa A có bậc $\leq 2m-2$ và nếu ta gán trọng số i cho $A_i$ thì A là thuần nhất theo trọng số $m(m-1)$.
a) Tính duy nhất của A : nếu A thỏa mãn (48), thì đặc biệt $A = \operatorname{dis}(F)$, trong đó F là đa thức $X^m + \sum_{i=1}^m A_i X^{m-i}$ với các hệ số trong $\mathbf{Z}[A,, \ldots, A,_j]$.
b) Sự tồn tại *của* A : cho $s_1, \ldots, s_m$ là các đa thức đối xứng sơ cấp trong các ẩn $X_1, \ldots, X_m$. Tồn tại một đa thức $A \in \mathbf{Z}[A,, \ldots, A,_j]$, thuần nhất theo trọng số $m(m-1)$, sao cho
$$
\Delta(-s_1, s_2, \ldots, (-1)^m s_m) = \prod_{i < j} (X_i - X_j)^2;
$$

vì vế phải là một đa thức đối xứng P, thuần nhất bậc m(m − 1) trong $Z[X_1, ..., X_m]$ (IV, p. 62, Định lý 1). Bây giờ công thức (46) có nghĩa là dis(f) = P (f ), theo ký hiệu của IV, p. 74, và (48) suy ra trực tiếp từ đó.

c) Bậc của A : quan hệ (47) và định nghĩa của định thức kết quả (IV, p. 76) suy ra công thức

$$
(-1)^{m(m-1)/2} \Delta = \det(a_{ij})_{0 \leq i,j \leq 2m-2}
$$

với các giá trị sau của $a_{ij}$

$$
\begin{align*}
a_{00} &= 1 , \quad a_{0,m-1} = m , \\
a_{ij} &= A_{i-j} & \text{với } 1 \leq i \leq 2m-2 , \quad 0 \leq j \leq m-2 \\
a_{ij} &= (j-i+1) A_{m+i-j-1} & \text{với } 1 \leq i \leq 2m-2 , \quad m-1 \leq j \leq 2m-2 .
\end{align*}
$$

$a_{0j} = 0$ nếu $j \neq 0 , \ j \neq m-1$

Trong các công thức này, ngầm hiểu rằng $A_i = 1$ và $A_i = 0$ với $i < 0$ hoặc $i > m$. Bây giờ (50) cho thấy ngay rằng A có bậc $\leq 2m-2$, như ta phải chứng minh.

Mệnh đề 10 cho phép ta mở rộng định nghĩa của biệt thức sang các đa thức không đơn nhất. Cho $m \geq 1$ là một số nguyên, thì tồn tại duy nhất một đa thức thuần nhất bậc $2m-2$, ký hiệu $\tilde{\Delta}$, trong $Z[A,, A,, ..., A_]$ sao cho

$$
\Delta(A_1, ..., A_r) = \tilde{\Delta}(1, A_1, ..., A_r)
$$

vì, do A có bậc $\leq 2m-2$, nên phân thức hữu tỉ

$$
A_0^{2m-2} \Delta(A_1/A_0, ..., A_m/A_0)
$$

thuộc vành con $Z[A_0, A,, ..., A_]$ của $Q(A,, A,, ..., A_)$. Nếu $A_i$ có trọng số i với $0 \leq i \leq m$, thì $\tilde{\Delta}$ là thuần nhất theo trọng số $m(m-1)$. Nếu f là một đa thức có bậc $\leq m$, chẳng hạn

$$
f = a_0 X^m + a_1 X^{m-1} + \cdots + a_{m-1} X + a_m ,
$$

thì ta đặt

$$
\operatorname{dis}_m(f) = \tilde{\Delta}(a_0, a_1, ..., a_r).
$$

Khi $m = \deg f$, ta sẽ chỉ viết dis(f) thay cho $\operatorname{dis}_m(f)$; nếu f là đa thức đơn nhất, thì dis(f) trùng với biệt thức được định nghĩa trong Định nghĩa 2, theo (48), (51) và (52).

#### Mệnh đề 11 {#alg-iv-s6-prop-11 .statement}

— Cho f trong $A[X]$ có bậc $\leq m$.

(i) *Nếu* $\rho : A \to B$ là một đồng cấu vành, ta có $\operatorname{dis}_m(\rho_f) = \rho(\operatorname{dis}_m(f))$.

(ii) Cho $\lambda, \alpha_1, ..., a_r$ là các phần tử của A. *Nếu* $f = X(X-\alpha_1) ... (X-a_r)$; thì ta có

$$
\operatorname{dis}_m(f) = \lambda^{2m-2} \prod_{i < j} (\alpha_i - \alpha_j)^2 .
$$

(iii) Cho $a_0$ là hệ số của $X^m$ trong $f$; khi đó ta có

$$
\text{res}_{m,m-1}(f, Df) = \text{res}_{m-1,m}(Df, f) = (-1)^{m(m-1)/2} a_0 \text{ dis}_m(f) .
$$

Khẳng định (i) hiển nhiên.

Vì $\tilde{\Delta}$ là thuần nhất bậc $2m - 2$, ta có

$$
\text{dis}_m(\lambda f) = \lambda^{2m-2} \text{dis}_m(f)
$$

cho mọi đa thức $f \in A[X]$ có bậc $\leq m$. Mệnh đề (ii) bây giờ suy ra từ các công thức (46) và (55).

Khi $f$ là đơn nhất có bậc $m$, ta có $a_0 = 1$ và Mệnh đề (iii) được quy về công thức (47). Ghi nhớ (55) và quan hệ

$$
\text{res}_{m,n}(\lambda f, \mu g) = \lambda^n \mu^m \text{res}_{m,n}(f, g),
$$

(IV, p. 77), ta có thể chuyển từ đó sang trường hợp $a_0$ khả nghịch trong $A$. Bây giờ trường hợp tổng quát suy ra từ Mệnh đề 11, (i) và Bổ đề 5 (IV, p. 79).

#### Hệ quả 1 {#alg-iv-s6-prop-11-cor-1 .statement}

— Cho $g \in A[X]$ và cho $n$ là một số nguyên dương sao cho $\deg g \leq n$. Ta có

$$
\text{dis}_{m+n}(fg) = \text{dis}_m(f) \cdot \text{dis}_n(g) \cdot \text{res}_{m,n}(f,g)^2 .
$$

Bằng lập luận như trước, ta quy về trường hợp $f$ và $g$ là đơn nhất có bậc tương ứng là $m$ và $n$. Bây giờ đặt $B = E_f \otimes E_g$, trong đó $E_f$ (tương ứng $E_g$) là đại số phân tích phổ quát của $f$ (tương ứng $g$) (IV, p. 73). Khi đó $A$ là một vành con của $B$, và trong $B[X]$ ta có các phân tích

$$
f = \prod_{i=1}^m (X - \alpha_i), \quad g = \prod_{j=1}^n (X - \beta_j) .
$$

Do đó ta có

$$
fg = \prod_{k=1}^{m+n} (X - \gamma_k) ,
$$

với $\gamma_i = \alpha_i$ với $1 \leq i \leq m$ và $\gamma_{m+j} = \beta_j$ với $1 \leq j \leq n$. Ta có đẳng thức hiển nhiên

$$
\prod_{k < k'} (\gamma_k - \gamma_{k'}) = \prod_{i < i'} (\alpha_i - \alpha_{i'}) \cdot \prod_{j < j'} (\beta_j - \beta_{j'}) \cdot \prod_{i,j} (\alpha_i - \beta_j)
$$

Bình phương quan hệ này ta thu được (57), theo (40) và (46).

#### Hệ quả 2 {#alg-iv-s6-prop-11-cor-2 .statement}

— Nếu $a_0$ là hệ số của $X^m$ trong $f$, ta có

$$
\text{dis}_{m+1}(f) = a_0^2 \text{dis}_m(f)
$$

Điều này suy ra từ Hệ quả 1 khi lấy $n = 1,\ g = 1$, theo công thức res,,$(f,1) = a_0$ (IV, p. 76, Ví dụ 1).

#### Hệ quả 3 {#alg-iv-s6-prop-11-cor-3 .statement}

— Cho $A$ là một trường, và cho $f$ là một đa thức không hằng trong $A[X]$. Để $f$ và $Df$ nguyên tố cùng nhau, điều kiện cần và đủ là $\mathrm{dis}(f) \neq 0$.
Điều này suy ra từ Mệnh đề 11, (iii) và Hệ quả 2 của IV, p. 78.

#### Nhận xét {#alg-iv-s6-n7-rem-1 .statement}

Một áp dụng hai lần của Hệ quả 2 ở trên cho thấy rằng ta có $\mathrm{dis}_m(f) = 0$ với mọi đa thức $f$ có bậc $\leq m - 2$.

#### Ví dụ 3 {#alg-iv-s6-n7-exa-3 .statement}

Cho $m = 2$. Theo Ví dụ2 (IV, p. 81) ta có $\Delta(A_1, A,) = A_1^2 - 4A_2$, do đó $\tilde{\Delta}(A_0, A,, A,) = A_1^2 - 4A_0A_2$. Nói cách khác, ta có
$$
\mathrm{dis}_2(a_0X^2 + a_1X + a,) = a_1^2 - 4a_0a_2 .
$$

#### Ví dụ 4 {#alg-iv-s6-n7-exa-4 .statement}

Xét đa thức
$$
F = A_0X^3 + 3A_1X^2 + 3A_2X + A,
$$
với các hệ số trong $Q[A_0, A,, A,, A_3]$. Ta có
$$
DF = 3(A_0X^2 + 2A_1X + A,) ,
$$
$$
F - 1/3X \cdot DF = A_1X^2 + 2A_2X + A_3 .
$$
Theo các công thức (54) (IV, p. 84) và (29) (IV, p. 77) ta có
$$
A_0 \cdot \mathrm{dis}_3(F) = - \mathrm{res}_{2,3}(DF, F) = - \mathrm{res}_{2,3}(DF, F - 1/3X \cdot DF)
$$
Áp dụng Hệ quả 2 của IV, p. 80 cuối cùng ta thu được
$$
\mathrm{dis}_3(F) = - 27 \mathrm{res}_{2,2}(A_0X^2 + 2A_1X + A,,\ A_1X^2 + 2A_2X + A,) .
$$
Theo Ví dụ 3 của IV, p. 80, do đó ta có
$$
\tilde{\Delta}(A_0, 3A_1, 3A_2, A_3) = - 27 (A_0A_3 - A_1A_2)^2 - 108 (A_1A_3 - A_2^2)(A_1^2 - A_0A_2) .
$$
Sau một số tính toán ta thấy rằng, nếu $f = a_0X^3 + a_1X^2 + a_2X + a_3$, ta có
$$
\mathrm{dis}_3(f) = a_1^2a_2^2 + 18a_0a_1a_2a_3 - 4a_1^3a_3 - 4a_0a_2^3 - 27a_0^2a_3^2 .
$$
Đặc biệt, ta có
$$
\mathrm{dis}(X^3 + pX + q) = - (4p^3 + 27q^2) .
$$

Bài tập

### Bài tập {#alg-iv-s6-exercises}

Xem các [bài tập cho § 6](exercises/s6/).
