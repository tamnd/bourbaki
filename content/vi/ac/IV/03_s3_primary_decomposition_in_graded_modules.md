---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 3
section_title: Primary decomposition in graded modules
lang: vi
source: ac-i-vii
book_pages: 283-285, 301
pdf_pages: 0303-0305, 0321-0321
extraction: ocr
subsections:
    - "no": 1
      title: PRIME IDEALS ASSOCIATED WITH A GRADED MODULE
      page: 283
      pdf_page: 303
    - "no": 2
      title: PRIMARY SUBMODULES CORRESPONDING TO GRADED PRIME IDEALS
      page: 284
      pdf_page: 304
    - "no": 3
      title: PRIMARY DECOMPOSITION IN GRADED MODULES
      page: 285
      pdf_page: 305
statements: 6
exercises: 3
content_sha256: 037baafad936f1794febc3d2a8adb5d27a6957bc321afb046cd6ecd0c6b7494b
translated_from: content/en/ac/IV/03_s3_primary_decomposition_in_graded_modules.md
source_content_sha256: 55183dce28d121c14a65bc1ae9b8a1e4c9902f11e7b2707081227fe1fa054024
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-5035aace
glossary_version: 34
glossary_terms_sha256: 14ceb431a973a8da769290b04ffbb35f77aa74ef7f2cac2481af0c0aac7be12d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. PHÂN TÍCH NGUYÊN SƠ TRONG CÁC MÔĐUN PHÂN BẬC

### 1. CÁC IĐÊAN NGUYÊN TỐ LIÊN KẾT VỚI MỘT MÔĐUN PHÂN BẬC

#### Mệnh đề 1 {#ac-iv-s3-prop-1 .statement}

Cho $A$ là một nhóm giao hoán xoắn tự do, $A$ là một vành phân bậc kiểu $A$ và $M$ là một $A$-môđun phân bậc kiểu $A$. Mọi iđêan nguyên tố liên kết với $M$ đều phân bậc và là linh hóa tử của một phần tử thuần nhất của $M$.

Ta biết rằng $A$ có thể được trang bị một cấu trúc cấp toàn phần tương thích với cấu trúc nhóm của nó (Đại số, Chương II, § 11, no. 4, Bổ đề 2). Cho $p$ là một iđêan nguyên tố liên kết với $M$, là linh hóa tử của một phần tử $x \in M$, và cho $(x_i)_{i \in \Delta}$ là họ các thành phần thuần nhất của $x$; cho $i(1) < i(2) < \cdots < i(r)$ là các giá trị của $i$ sao cho $x_i \neq 0$. Xét một phần tử $a \in p$ và cho $(a_i)_{i \in \Delta}$ là họ các thành phần thuần nhất của nó; ta sẽ chứng minh rằng $a, \in p$ với mọi $i \in A$, điều này sẽ cho thấy rằng $p$ là một iđêan phân bậc.

Ta lập luận bằng quy nạp theo số các chỉ số $i$ sao cho $a, \neq 0$. Mệnh đề của ta là hiển nhiên nếu số này bằng 0; nếu không, cho $m$ là lớn nhất trong các chỉ số $i$ sao cho $a, \neq 0$; nếu ta chứng minh được rằng $a, \in p$, giả thiết quy nạp áp dụng cho $a - a,$ sẽ cho kết luận. Bây giờ, $ax = 0$; với mọi $j \in A$, sử dụng sự kiện rằng thành phần thuần nhất bậc $m + j$ của $ax$ bằng 0, ta thu được
$$
\sum_{i \in \Delta} a_{m-i} x_{j+i} = 0;
$$
ta kết luận rằng $a_m x_j$ là một tổ hợp tuyến tính của các $x_i$ có các chỉ số $i > j$. Đặc biệt do đó $a_m x_{i(r)} = 0$, do đó, bằng quy nạp giảm theo $n < r$, $a_m^{r-n+1} x_{i(n)} = 0$. Khi đó $a_m^r x = 0$, do đó $a_m^r \in p$ và, vì $p$ là nguyên tố, $a, \in p$.

Ta chứng minh rằng $p$ là linh hóa tử của một phần tử thuần nhất của $M$. Ta viết $b_n = \operatorname{Ann}(x_{i(n)})$ với $1 \leq n \leq r$. Với mọi phần tử thuần nhất $b$ của $p$ và mọi $n$, thành phần thuần nhất của $bx$ có bậc $i(n) + \deg(b)$ là $bx_{i(n)}$, do đó $bx_{i(n)} = 0$ và vì thế $b \in 6$; vì $p$ được sinh bởi các phần tử thuần nhất của nó, $p \subset 6$. Mặt khác, rõ ràng $\bigcap_{n=1}^r 6_n \subset \operatorname{Ann}(x) = p$; vì $p$ là nguyên tố, tồn tại một $n$ sao cho $b_n \subset p$ (Chương 11, § 1, no. 1, Mệnh đề 1), do đó $b_n = P = \operatorname{Ann}(x_{i(n)})$, điều này hoàn thành chứng minh.

#### Hệ quả {#ac-iv-s3-n1-cor-1 .statement}

Với mọi iđêan nguyên tố $p$ (tất yếu là phân bậc) liên kết với một $A$-môđun phân bậc $M$, tồn tại một chỉ số $k \in A$ sao cho $A$-môđun phân bậc $(A/p)(k)$ nhận được từ $A$-môđun phân bậc $A/p$ bằng cách làm giảm các bậc đi $k$ (Đại số, Chương II, § 11, no. 2) là đẳng cấu với một môđun con phân bậc của $M$.

Với ký hiệu của chứng minh Mệnh đề 1, xét đồng cấu nhận được, bằng cách lấy thương, từ đồng cấu $a \mapsto ax_{i(n)}$ của $A$ vào $M$; đồng cấu sau là một đồng cấu phân bậc có bậc $i(n)$ và do đó nó cho, khi lấy thương, một đồng cấu phân bậc song ánh có bậc $i(n)$ từ $A/p$ lên một môđun con phân bậc của $M$.

#### Mệnh đề 2 {#ac-iv-s3-prop-2 .statement}

*Cho $A$ là một nhóm giao hoán không xoắn, $A$ là một vành Noether phân bậc kiểu $A$ và $M$ là một $A$-môđun phân bậc sinh hữu hạn kiểu $A$. Tồn tại một chuỗi hợp thành $(\mathbf{M}_i)_{0 \leq i \leq n}$ gồm các môđun con phân bậc của $M$ sao cho với $0 \leq i \leq n - 1$ môđun phân bậc $\mathbf{M}_i / \mathbf{M}_{i+1}$ là đẳng cấu với một môđun phân bậc dịch chuyển $(A/p_i)(k_i)$, trong đó $p_i$ là một iđêan nguyên tố phân bậc của $A$ và $k_i \in A$.*

Chỉ cần lần lại lập luận của § 1, no. 4, Định lý 1, trong dịp này lấy $\mathcal{G}$ là tập hợp các môđun con phân bậc của $M$ có một chuỗi hợp thành với các tính chất của mệnh đề; ta kết luận bằng cách sử dụng Hệ quả của Mệnh đề 1.

### 2. CÁC MÔĐUN CON NGUYÊN SƠ TƯƠNG ỨNG VỚI CÁC IĐÊAN NGUYÊN TỐ PHÂN BẬC

#### Mệnh đề 3 {#ac-iv-s3-prop-3 .statement}

*Cho $A$ là một nhóm giao hoán không xoắn, $A$ là một vành Noether phân bậc kiểu $A$, $p$ là một iđêan phân bậc của $A$ và $M$ là một $A$-môđun phân bậc kiểu $A$ không rút gọn về $0$. Giả sử rằng với mọi phần tử thuần nhất $a$ của $p$, phép vị tự tỉ số $a$ trên $M$ là gần lũy linh và với mọi phần tử thuần nhất $b$ của $A - p$, phép vị tự tỉ số $b$ trên $M$ là đơn ánh. Khi đó $p$ là nguyên tố và môđun con $\{0\}$ của $M$ là $p$-nguyên sơ.*

Chỉ cần chứng minh rằng $\operatorname{Ass}(M) = \{p\}$ (§ 2, no. 1, Mệnh đề 1). Cho $q$ là một iđêan nguyên tố liên kết với $M$; nó là một iđêan phân bậc và là linh hóa tử của một phần tử thuần nhất $x \neq 0$ của $M$ (no. 1, Mệnh đề 1). Với mọi phần tử thuần nhất $a$ của $q$, $ax = 0$ và do đó phép vị tự tỉ số $a$ trên $M$ không là đơn ánh, do đó $a \in p$. Ngược lại, cho $b$ là một phần tử thuần nhất của $p$; tồn tại một số nguyên $n > 0$ sao cho $b^n x = 0$, do đó $b^n \in \operatorname{Ann}(x) = q$ và, vì $q$ là nguyên tố, $b \in q$. Vì $p$ và $q$ được sinh bởi các phần tử thuần nhất tương ứng của chúng, $p = q$, điều này chứng minh rằng $\operatorname{Ass}(M) \subset \{p\}$. Vì $M \neq \{0\}, \operatorname{Ass}(M) \# \varnothing$ (§ 1, no. 1, Hệ quả 1 của Mệnh đề 2), do đó $\operatorname{Ass}(M) = \{p\}$.

#### Mệnh đề 4 {#ac-iv-s3-prop-4 .statement}

*Cho $A$ là một nhóm giao hoán không xoắn, $A$ là một vành Noether phân bậc kiểu $A$ và $M$ là một $A$-môđun phân bậc kiểu $A$. Cho $p$ là một iđêan nguyên tố của $A$ và $N$, một môđun con của $M$ là $p$-nguyên sơ đối với $M$.

(i) Iđêan phân bậc lớn nhất $p'$ của $A$ được chứa trong $p$ (Đại số, Chương 11, § 11, no. 3) là nguyên tố.

(ii) Môđun con phân bậc lớn nhất $N'$ của $N$ là $p'$-nguyên sơ đối với $M$.*

Ta biết (*loc. cit.*) rằng các phần tử thuần nhất của $p'$ (tương ứng, $N'$) chính là các phần tử thuần nhất của $p$ (tương ứng, $N$). Cho $a$ là một phần tử thuần nhất của $p$; nếu $x$ là một phần tử thuần nhất của $M$, tồn tại một số nguyên $n > 0$ sao cho $a^n x \in N$; vì $a^n x$ là thuần nhất, nên $a^n x \in N'$; vì mọi $y \in M$ là tổng trực tiếp của một số hữu hạn các phần tử thuần nhất, ta kết luận rằng tồn tại một số nguyên $q > 0$ sao cho $a^q y \in N'$, do đó phép vị tự với tỉ số $a$ trong $M/N'$ là gần lũy linh.

Bây giờ xét một phần tử thuần nhất $b$ của $A - p'$; khi đó $b \notin p$ vì $b$ là thuần nhất. Cho $x$ là một phần tử của $M$ sao cho $bx \in N'$ và cho $(x_i)_{i \in \Delta}$ là họ các thành phần thuần nhất của $x$. Vì $N'$ là phân bậc, $bx_i \in N'$ với mọi $i$, do đó $bx_i \in N$ và, vì $b \notin p$, ta kết luận rằng $x_i \in N$; vì $x_i$ là thuần nhất, $x_i \in N'$, do đó $x \in N'$ và phép vị tự với tỉ số $b$ trên $M/N'$ là đơn ánh. Mệnh đề 4 khi đó suy ra từ Mệnh đề 3 áp dụng cho $p'$ và $M/N'$.

### 3. PHÂN TÍCH NGUYÊN SƠ TRONG CÁC MÔĐUN PHÂN BẬC

#### Mệnh đề 5 {#ac-iv-s3-prop-5 .statement}

Cho $A$ là một nhóm giao hoán không xoắn, $A$ là một vành Noether phân bậc kiểu $A$, $M$ là một $A$-môđun phân bậc kiểu $M$, $N$ là một môđun con phân bậc của $M$ và $N = \bigcap_{i \in I} Q_i$ là một phân tích nguyên sơ của $N$ trong $M$.

(i) Cho $Q'_i$ là môđun con phân bậc lớn nhất của $M$ được chứa trong $Q_i$. Khi đó các $Q'_i$ là nguyên sơ và $N = \bigcap_{i \in I} Q'_i$.

(ii) Nếu phân tích nguyên sơ $N = \bigcap_{i \in I} Q_i$ là rút gọn, thì phân tích nguyên sơ $N = \bigcap_{i \in I} Q'_i$ cũng là rút gọn và với mọi $i \in I$ các iđêan nguyên tố tương ứng với $Q_i$ và $Q'_i$ là bằng nhau.

(iii) Nếu $Q_i$ tương ứng với một iđêan nguyên tố $p_i$ là một phần tử cực tiểu của $\operatorname{Ass}(M/N)$, thì $Q_i$ là một môđun con phân bậc của $M$.

Ta đã thấy (no. 2, Mệnh đề 4) rằng các $Q'_i$ là nguyên sơ đối với $M$ và $N \subset Q'' \subset Q_i$, điều này chứng minh (i). Mệnh đề 4 của no. 2 cũng chỉ ra rằng iđêan nguyên tố $p'_i$ tương ứng với $Q'_i$ là iđêan phân bậc lớn nhất được chứa trong iđêan nguyên tố $p_i$ tương ứng với $Q_i$. Nếu phân tích $N = \bigcap_{i \in I} Q_i$ là rút gọn, $p_i \in \operatorname{Ass}(M/N)$ với mọi $i$ (§ 2, no. 3, Mệnh đề 4), do đó $p_i$ là một iđêan phân bậc (no. 1, Mệnh đề 1) và vì vậy $p'_i = p_i$; khi đó $\operatorname{Ass}(M/N) = \bigcup_{i \in I} \{p'_i\}$ (§ 2, no. 3, Mệnh đề 4), điều này chứng minh rằng phân tích $N = \bigcap_{i \in I} Q'_i$ là rút gọn (§ 2, no. 3, Mệnh đề 4). Cuối cùng, nếu $p_i$ là một phần tử cực tiểu của $\operatorname{Ass}(M/N)$, thì $p'_i = p_i$ vì $p_i$ là phân bậc (no. 1, Mệnh đề 1), do đó $Q'_i = Q_i$ theo § 2, no. 3, Mệnh đề 5.

### Bài tập {#ac-iv-s3-exercises}

Xem các [bài tập cho § 3](exercises/s3/).
