---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 3
section_title: Factorial domains
lang: vi
source: ac-i-vii
book_pages: 502-512
pdf_pages: 0520-0530
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF FACTORIAL DOMAINS
      page: 502
      pdf_page: 520
    - "no": 2
      title: CHARACTERIZATIONS OF FACTORIAL DOMAINS
      page: 502
      pdf_page: 520
    - "no": 3
      title: DECOMPOSITION INTO EXTREMAL ELEMENTS
      page: 504
      pdf_page: 522
    - "no": 4
      title: RINGS OF FRACTIONS OF A FACTORIAL DOMAIN
      page: 505
      pdf_page: 523
    - "no": 5
      title: POLYNOMIAL RINGS OVER A FACTORIAL DOMAIN
      page: 505
      pdf_page: 523
    - "no": 6
      title: FACTORIAL DOMAINS AND ZARISKI RINGS
      page: 506
      pdf_page: 524
    - "no": 7
      title: PRELIMINARIES ON AUTOMORPHISMS OF RINGS OF FORMAL POWER SERIES
      page: 506
      pdf_page: 524
    - "no": 8
      title: THE PREPARATION THEOREM
      page: 507
      pdf_page: 525
    - "no": 9
      title: FACTORIALITY OF RINGS OF FORMAL POWER SERIES
      page: 511
      pdf_page: 529
statements: 19
exercises: 0
content_sha256: 2ebdd44893f2057bd4f5a54122a80abf135d3cf031db1074974a6ce130f827a2
translated_from: content/en/ac/VII/03_s3_factorial_domains.md
source_content_sha256: 24b2404392ec37a498e3b069e48cd23f3c3de2b03e46d826d86d894e0aa6aa9e
translation_model: gpt-5.4
translation_run: translate-vi-d91a6f09
glossary_version: 34
glossary_terms_sha256: b0243daad0909dbaba4dbefdc13a0a245f291808aca40260af31dbcae74d87aa
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. MIỀN FACTORIAL

### 1. ĐỊNH NGHĨA MIỀN FACTORIAL

#### Định nghĩa 1 {#ac-vii-s3-def-1 .statement}

Một miền Krull mà mọi iđêan ước của nó đều là chính được gọi là một miền factorial (hay miền phân tích duy nhất).

Nói cách khác, nhóm các lớp ước (§ 1, no. 2) thu về 0.

Ví dụ
(1) Mọi miền iđêan chính đều là factorial (và, xin nhắc lại, đều là miền Dedekind). Đảo lại, mọi miền Dedekind factorial đều là một miền iđêan chính theo § 2, no. 2, Định lý 1 (c).
(2) Đặc biệt, nếu K là một trường, thì các vành K[X] và K[[X]] là các miền factorial (xem Định lý 2 và Mệnh đề 8 dưới đây để có các tổng quát hóa).
(3) \* Vành địa phương của một điểm đơn của một đa tạp đại số là một miền factorial. Vành các mầm hàm giải tích tại gốc tọa độ của $\mathbf{C}^n$ là một miền factorial. \*

### 2. CÁC ĐẶC TRƯNG CỦA MIỀN FACTORIAL

Cho một vành $A$, ta cần xét điều kiện sau:

(M) Mọi họ không rỗng các iđêan chính nguyên của $A$ đều có một phần tử cực đại.

#### Định lý 1 {#ac-vii-s3-thm-1 .statement}

Cho $A$ là một miền nguyên. Các điều kiện sau là tương đương:
(a) $A$ là factorial;
(b) nhóm có thứ tự của các iđêan chính phân thức khác không của $A$ là một tổng trực tiếp của các nhóm đẳng cấu với $\mathbf{Z}$ (được sắp thứ tự bởi thứ tự tích);
(c) điều kiện (M) được thỏa mãn và giao của hai iđêan chính của $A$ là một iđêan chính;
(d) điều kiện (M) được thỏa mãn và, với mọi phần tử cực biên $p$ của $A$, iđêan $Ap$ là nguyên tố;
(e) $A$ là một miền Krull và mọi iđêan nguyên tố có chiều cao 1 đều là chính.

Ta sẽ ký hiệu bởi K trường phân thức của A và bởi $\mathcal{P}^*$ (hay $\mathcal{P}^*(A)$) nhóm có thứ tự của các iđêan chính phân thức khác không của A. Chứng minh sẽ được thực hiện bằng cách chứng minh các kéo theo sau:

(a) ⇔ (b) ⇔ (c) ⇔ (d) ⇔ (e)

Ta chứng minh rằng (a) kéo theo (b); nếu A là factorial, $\mathcal{P}^*$ đẳng cấu với nhóm các ước của A và do đó với một tổng trực tiếp của các nhóm $\mathbf{Z}$ ($§ 1$, no. 3, Định lý 2).

Bây giờ lưu ý rằng quan hệ "giao của hai iđêan chính nguyên của A là một iđêan chính" có nghĩa là mọi cặp có thứ tự các phần tử của A đều có một bội chung nhỏ nhất, nghĩa là $\mathcal{P}^*$ là một nhóm có thứ tự dàn (Đại số, Chương VI, $§ 1$, no. 9, Mệnh đề 8). Vì vậy, việc (b) kéo theo (c) (và thậm chí là tương đương với nó) suy ra từ Đại số, Chương VI, $§ 1$, no. 13, Định lý 2. Việc (c) kéo theo (d) suy ra từ Đại số, Chương VI, $§ 1$, no. 13, Mệnh đề 14 (DIV).

Việc (d) kéo theo (b) suy ra từ Đại số, Chương VI, $§ 1$, no. 13, Định lý 2 áp dụng cho nhóm $\mathcal{S}^*$.

Ta chứng minh rằng (b) kéo theo (e). Nếu (b) đúng, có một đẳng cấu từ $\mathcal{P}^*$ lên $\mathbf{Z}^{(l)}$; gọi $(v_i(x))_{i \in I}$ là phần tử của $\mathbf{Z}^{(l)}$ tương ứng với iđêan $Ax$ ($x \in K^*$). Ngay lập tức thấy rằng mỗi $v_i$ là một định giá rời rạc trên K, rằng A là giao của các vành của các $v_i$ và rằng, với $x \in K^*$, $v_i(x) = 0$ trừ ra đối với một số hữu hạn chỉ số $i$; do đó A là một miền Krull. Mặt khác, gọi q là một iđêan nguyên tố của A có chiều cao 1; nó chứa một phần tử khác không a mà tất yếu là không khả nghịch và do đó cũng (theo định nghĩa của một iđêan nguyên tố) là một trong các phần tử cực biên của A; vì $Ap$ là nguyên tố và khác không, $q = Ap$, điều này chứng minh rằng q là chính.

Sau cùng ta chứng minh rằng (e) kéo theo (a). Gọi a là một iđêan ước của A. Tồn tại các iđêan nguyên tố $p_i$ của A có chiều cao 1 sao cho $\operatorname{div} a = \sum_i n_i \operatorname{div} p_i$ trong đó $n_i \in \mathbf{Z}$. Nếu (e) đúng, $p_i$ có dạng $Ap_i$, do đó $\operatorname{div} a = \operatorname{div} \left( \prod_i Ap_i^{n_i} \right)$ và vì thế $a = \prod_i Ap_i^{n_i}$ vì a là iđêan ước.

#### Mệnh đề 1 {#ac-vii-s3-prop-1 .statement}

*Nếu A là một miền Krull. Nếu mọi iđêan ước của A đều khả nghịch, thì, với mọi iđêan cực đại m của A, $A_m$ là factorial. Đảo lại là đúng nếu còn giả thiết thêm rằng mọi iđêan ước của A đều sinh hữu hạn (đặc biệt nếu A là Noether).*

Giả sử rằng mọi iđêan ước của $A$ đều khả nghịch; vì $A_{,,}$ là một miền Krull ($§ 1$, no. 4, Mệnh đề 6), mọi iđêan ước $a$ của $A_{,,}$ đều là giao của hai iđêan phân thức chính ($§ 1$, no. 5, Hệ quả 2 của Mệnh đề 9); do đó $a = bA_m$, trong đó $b$ là một iđêan ước của $A$ (Chương II, $§ 2$, no. 4); vì $b$ khả nghịch theo giả thiết, ta suy ra từ Chương II, $§ 5$, no. 6, Định lý 4 rằng $a$ là chính và vì thế $A_{,,}$ là một miền phân tích duy nhất (no. 1, Định nghĩa 1). Ngược lại, nếu mọi $A_{,,}$ đều là các miền phân tích duy nhất và $c$ là một iđêan ước sinh hữu hạn của $A$, thì $cA_m$ là một iđêan ước của $A_{,,}$, như suy ra từ $§ 1$, no. 5, Hệ quả 2 của Mệnh đề 9 và Chương II, $§ 2$, no. 4; theo giả thiết $cA_m$ là chính và do đó suy ra từ Chương 11, $§ 5$, no. 6, Định lý 4 rằng $c$ khả nghịch.

### 3. PHÂN TÍCH THÀNH CÁC PHẦN TỬ CỰC BIÊN

Cho $A$ là một miền nguyên, $K$ là trường phân thức của nó và $U$ là nhóm nhân các phần tử khả nghịch của $A$. Nhắc lại (Đại số, Chương VI, $§ 1$, no. 5) rằng có một đẳng cấu chính tắc từ $K^*/U$ lên nhóm $\mathcal{P}^*$ các iđêan chính phân thức khác không của $A$. Khi đó điều kiện (b) của Định lý 1 có thể được diễn đạt như sau:

#### Mệnh đề 2 {#ac-vii-s3-prop-2 .statement}

*Cho $A$ là một miền nguyên. Điều kiện cần và đủ để $A$ là phân tích duy nhất là tồn tại một tập con $P$ của $A$ sao cho mọi $a \in A - \{0\}$ đều có thể viết duy nhất dưới dạng $a = u \prod_{p \in P} p^{n(p)}$, trong đó $u \in U$ và các $n(p)$ là những số nguyên dương bằng không trừ một số hữu hạn phần tử.*

Nếu $P$ thỏa mãn điều kiện này thì rõ ràng mọi phần tử của nó đều là *cực biên* và mọi phần tử cực biên của $A$ đều liên kết với một phần tử duy nhất của $P$. Nhắc lại rằng khi đó $P$ được gọi là một *hệ đại diện các phần tử cực biên* của $A$ (Đại số, Chương VII, $§ 1$, no. 3, Định nghĩa 2).

Tiếp tục giả sử rằng $A$ là phân tích duy nhất. Ta đã thấy (no. 2, Định lý 1) rằng nhóm $\mathcal{P}^*$ là một dàn. Do đó ta có thể áp dụng các kết quả của Đại số, Chương VI, $§ 1$, nos. 9 và 13. Đặc biệt, mọi phần tử của $K^*$ đều có thể được viết theo một cách về bản chất là duy nhất dưới dạng một *phân thức bất khả quy*. Hai phần tử bất kỳ $a, b$ của $K^*$ có một ước chung lớn nhất và một bội chung nhỏ nhất; nếu $a = u \prod_{p \in P} p^{n(p)}$ và
$$
b = u' \prod_{p \in P} p^{m(p)}
$$
là các phân tích của $a$ và $b$ thành tích các phần tử cực biên, thì:
$$
\text{(1)} \quad \text{ƯCLN}(a, b) = w \prod_{p \in P} p^{\inf(m(p), n(p))}
$$
$$
\text{(2)} \quad \text{BCNN}(a, b) = w' \prod_{p \in P} p^{\sup(m(p), n(p))}
$$

trong đó $w, w'$ thuộc U. Đặc biệt, ta thu lại các kết quả của Đại số, Chương VIII, § 1, no. 3.

Với mọi $p \in P$, ánh xạ $a \mapsto n(p)$ là một định giá rời rạc $v_p$ trên K mà vành của nó hiển nhiên là $A_{A_p}$. Từ Định lý 1(e) suy ra rằng các $v_p$ chính là các định giá cốt yếu của A và các iđêan $Ap$ ($p \in P$) chính là các iđêan nguyên tố của A có chiều cao 1.

### 4. VÀNH PHÂN THỨC CỦA MỘT MIỀN GIAI THỪA

#### Mệnh đề 3 {#ac-vii-s3-prop-3 .statement}

*Cho A là một miền Krull và S là một tập con nhân của A không chứa 0.*

(i) *Nếu A là giai thừa thì $S^{-1}A$ là giai thừa.*
(ii) *Nếu S được sinh bởi một họ các phần tử $p_i$ sao cho các iđêan chính $Ap_i$ là nguyên tố và $S^{-1}A$ là giai thừa, thì A là giai thừa.*

Điều này suy ra ngay lập tức từ Định nghĩa 1 của no. 1 và § 1, no. 10, Mệnh đề 17.

### 5. VÀNH ĐA THỨC TRÊN MỘT MIỀN GIAI THỪA

Cho A là một miền giai thừa, K là trường phân thức của nó và $f$ là một phần tử khác không của $K[X]$; một phần tử c của $K^*$ sẽ được gọi là một *nội dung* của $f$ nếu nó là một ước chung lớn nhất của các hệ số của $f$. Cho $\nu$ là một định giá trên K cốt yếu đối với A và $\bar{\nu}$ là mở rộng chính tắc của nó lên $K[X]$ (được định nghĩa bởi $\bar{\nu}\left(\sum a_i X^i\right) = \inf \nu(a_i)$; xem Chương VI, § 10, no. 1, Mệnh đề 2); khi đó $\bar{\nu}(f) = \nu(c)$.

#### Bổ đề 1 (Gauss) {#ac-vii-s3-lem-1 .statement}

*Cho $f, f'$ là các phần tử khác không của $K[X]$ và c, $c'$ là các nội dung của $f, f'$. Khi đó $cc'$ là một nội dung của $ff'$.*

Cho d là một nội dung của $ff'$. Với mọi định giá $\nu$ trên K cốt yếu đối với A, cho $\bar{\nu}$ ký hiệu mở rộng chính tắc của nó lên $K[X]$. Khi đó
$$
\nu(d) = \bar{\nu}(ff') = \bar{\nu}(f) + \bar{\nu}(f') = \nu(c) + \nu(c') = \nu(cc').
$$
Do đó $cc'd^{-1}$ là một phần tử khả nghịch của A.

#### Định lý 2 {#ac-vii-s3-thm-2 .statement}

*Cho A là một miền giai thừa, K là trường phân thức của nó, $(p_\lambda)$ là một hệ đại diện các phần tử cực biên của A và $(P_\lambda)$ là một hệ đại diện các đa thức bất khả quy của $K[X]$, mỗi $P_\lambda$ có 1 làm nội dung. Khi đó:*
(i) *$A[X]$ là một miền giai thừa;*
(ii) *tập hợp các $p_\lambda$ và $P_\lambda$ là một hệ đại diện các phần tử cực biên của A[X].*

Cho $f$ là một phần tử khác không của $A[X]$. Trong vành $K[X]$, $f$ có thể được phân tích duy nhất dưới dạng:
$$
f = a \prod_\lambda P_\lambda^{n(\lambda)} \quad (a \in K^*, n(\lambda) \geq 0).
$$

Bổ đề 1 chứng minh rằng $a$ là một nội dung của $f$. Do đó $a \in A$. Vì $A$ là giai thừa, $a$ có thể được phân tích duy nhất dưới dạng:

$$
a = u \prod p_i^{m(i)} \quad (u \text{ khả nghịch trong } A,\ m(i) \geqslant 0).
$$

Do đó có sự tồn tại và tính duy nhất của phân tích:

$$
f = u \prod p_i^{m(i)} \bigcap_{\lambda} p_{\lambda}^{n(\lambda)}.
$$

Chú ý rằng định lý này chứng minh rằng mọi phần tử của $A$ thừa nhận *cùng một* phân tích thành các phần tử cực biên trong $A$ và $A[X]$. Vì vậy, ước chung lớn nhất của một họ các phần tử của $A$ là như nhau trong $A$ và trong $A[X]$.

Ta cũng có thể sử dụng Mệnh đề 18 của § 1, no. 10 để chỉ ra rằng $A[X]$ *là* một miền giai thừa khi và chỉ khi $A$ là một miền giai thừa.

#### Hệ quả {#ac-vii-s3-n5-cor-1 .statement}

*Nếu $A$ là một miền giai thừa thì miền $A[X_1, \ldots, X_n]$ là giai thừa.*

Lập luận bằng quy nạp theo $n$.

Hệ quả này có thể được mở rộng cho trường hợp một họ vô hạn các ẩn số (xem Bài tập 2).

### 6. MIỀN GIAI THỪA VÀ VÀNH ZARISKI

#### Mệnh đề 4 {#ac-vii-s3-prop-4 .statement}

*Nếu $A$ là một vành Zariski và $\hat{A}$ là vành hoàn thành của nó. Nếu $\hat{A}$ là một miền phân tích duy nhất, thì $A$ là một miền phân tích duy nhất.*

Điều này suy ra từ no. 1, Định nghĩa 1 và § 1, no. 10, Mệnh đề 16.

#### Hệ quả {#ac-vii-s3-n6-cor-1 .statement}

*Nếu vành hoàn thành của một vành địa phương Noether $A$ là một miền phân tích duy nhất, thì $A$ là một miền phân tích duy nhất.*

### 7. CÁC ĐIỀU CHUẨN BỊ VỀ TỰ ĐỒNG CẤU CỦA CÁC VÀNH CHUỖI LŨY THỪA HÌNH THỨC

#### Bổ đề 2 {#ac-vii-s3-lem-2 .statement}

*Cho $f(X_1, X_2, \ldots, X_n)$ là một chuỗi lũy thừa hình thức $\neq 0$ với hệ số trong một vành $E$. Tồn tại các số nguyên $u(i) \geqslant 1$ ($1 \leqslant i \leqslant n - 1$) sao cho*

$$
f(T^{u(1)}, \ldots, T^{u(n-1)}, T) \neq 0.
$$

Giả sử các số nguyên $u(i) \geqslant 1$ ($1 \leqslant i \leqslant k - 1$) được xác định sao cho $f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_k, \ldots, X_n) \neq 0$. Ta sẽ xác định một số nguyên $u(k) \geqslant 1$ sao cho

$$
f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_n^{u(k)}, X_{k+1}, \ldots, X_n) \neq 0.
$$

Khi đó bổ đề sẽ được chứng minh bằng quy nạp.

Nhận thấy rằng chuỗi $f(X_n^{u(1)}, \ldots, X_n^{u(k-1)}, X_k, \ldots, X)$ có thể được xem như một chuỗi theo $X_k$ và $X_n$ với hệ số trong $E[[X_{k+1}, \ldots, X_{n-1}]]$. Vì thế ta thấy rằng chỉ cần thiết lập bổ đề cho $n = 2$.

Vậy đặt
$$
f = \sum_{i,j} e_{ij} X^i Y^j \in E[[X, Y]]
$$
trong đó $f \neq 0$. Gọi $G \subset \mathbf{N} \times \mathbf{N}$ là tập hợp khác rỗng các cặp có thứ tự $(i, j)$ sao cho $e_{ij} \neq 0$. Trang bị cho $\mathbf{N} \times \mathbf{N}$ thứ tự từ điển. Gọi $(c, d)$ là phần tử bé nhất của $G$. Chọn một số nguyên $p > d$. Trong khai triển của
$$
f(T^p, T) = \sum_{(i, j) \in G} e_{ij} T^{ip + j}
$$
ta tìm các số hạng bậc $cp + d$. Nếu $ip + j = cp + d, i \geq c + 1$ là không thể, vì điều đó sẽ cho
$$
ip + j \geq (c + 1)p + j \geq (c + 1)p > cp + d;
$$
$i < c$ cũng không thể, vì $(c, d)$ là phần tử bé nhất của $G$; do đó $i = c$ và khi đó $j = d$. Vậy số hạng bậc $cp + d$ trong $f(T^p, T)$ là $e_{cd} T^{cp + d}$. Vì $e_{cd} \neq 0, f(T^p, T) \neq 0$. Do đó bổ đề được chứng minh.

Trong vành $E[[X_1, \ldots, X]]$, gọi $a$ là iđêan của các chuỗi lũy thừa hình thức không có số hạng hằng. Nếu $w_1, \ldots, w_n$ là các phần tử của $a$, nhắc lại rằng ánh xạ $f(X_1, \ldots, X,) \mapsto f(w_1, \ldots, w,)$ là tự đồng cấu duy nhất $s$ của vành $E[[X_1, \ldots, X_n]]$ sao cho $s(X_i) = w_i$ với $1 \leq i \leq n$ (Chương III, § 4, no. 5, Mệnh đề 6).

Ta lấy $w_1 = X_1 + X_n^{u(1)}, \ldots, w_{n-1} = X_{n-1} + X_n^{u(n-1)}, w_n = X_n$, trong đó các $u(i)$ là những số nguyên $\geq 1$. Gọi $s'$ là tự đồng cấu của $E[[X_1, \ldots, X_n]]$ biến $X_1$ thành $X_1 - X_n^{u(1)}, \ldots, X_{n-1}$ thành $X_{n-1} - X_n^{u(n-1)}$ và $X_n$ thành $X_n$. Khi đó $s'(s(X_i)) = X_i$ với $1 \leq i \leq n$ và do đó $s' \circ s$ là tự đẳng cấu đồng nhất; tương tự đối với $s \circ s'$. Vậy $s$ là một *tự đẳng cấu*.

#### Bổ đề 3 {#ac-vii-s3-lem-3 .statement}

*Cho $f$ là một phần tử khác không của $E[[X_1, \ldots, X_n]]$. Tồn tại những số nguyên $u(i) \geq 1 (1 \leq i \leq n-1)$ sao cho tự đẳng cấu $s$ của $E$ được xác định bởi*
$$
s(X_i) = X_i + X_n^{u(i)} \quad (1 \leq i \leq n-1)
$$
*và $s(X_n) = X_n$, biến $f$ thành một phần tử $g$ sao cho $g(0, \ldots, 0, X,) \neq 0$.*

$g(0, \ldots, 0, X,) = f(X_n^{u(1)}, \ldots, X_n^{u(n-1)}, X,)$. Vì thế Bổ đề 3 là một hệ quả của Bổ đề 2.

### 8. ĐỊNH LÝ CHUẨN BỊ

Trong số này, A sẽ chỉ một vành *địa phương*, $m$ iđêan cực đại của nó và $k = A/m$ trường thặng dư của nó. Giả sử rằng A là *Hausdorff và đầy đủ* đối với tôpô $m$-adic. Đặt $B = A[[X]]$; đó là một vành địa phương mà iđêan cực đại $\mathfrak{n}$ của nó được sinh bởi $m$ và $X$; với tôpô $\mathfrak{A}$-adic, B là Hausdorff và đầy đủ (Chương III, § 2, no. 6, Mệnh đề 6).

Với mọi chuỗi lũy thừa hình thức
$$
f = \sum_{i=0}^{\infty} a_i X^i \in B,
$$
ta viết
$$
\tilde{f} = \sum_{i=0}^{\infty} \bar{a}_i X^i \in k[[X]],
$$
trong đó $\bar{a}_i$ chỉ ảnh chính tắc của $a_i$ trong $k$. Chuỗi $\tilde{f}$ sẽ được gọi là *chuỗi rút gọn* của f; nếu $\tilde{f} \neq 0$, cấp của $\tilde{f}$ (nghĩa là số nguyên nhỏ nhất $s$ sao cho $a_s \notin m$) sẽ được gọi là *cấp rút gọn* của f.

#### Mệnh đề 5 {#ac-vii-s3-prop-5 .statement}

*Cho $f \in B$ là một chuỗi mà chuỗi rút gọn của nó khác không. Gọi $s$ là cấp rút gọn của nó và $M$ là A-môđun con của $B$ có cơ sở $\{1, X, \ldots, X^{s-1}\}$. Khi đó $B$ là tổng trực tiếp của $M$ và $f$ không là một ước của không trong $B$.*

(a) Ta chứng minh rằng $f \mid B \cap M = (0)$. Giả sử có một quan hệ:
$$
\left( \sum_{i=0}^{\infty} b_i X^i \right) f = r_0 + r_1 X + \cdots + r_{s-1} X^{s-1} \qquad (b_i \in A, r_j \in A).
$$
Ta chứng minh rằng các $b_i$ (và do đó các $r_j$) đều bằng không, điều này đặc biệt sẽ chứng minh rằng $f$ không phải là một ước của không trong $B$. Vì $A$ là Hausdorff, chỉ cần chứng minh rằng $b_i \in m^n$ với mọi $i \geq 0$ và mọi $n \geq 0$. Điều đó hiển nhiên với $n = 0$. Ta sẽ lập luận bằng quy nạp kép: ta sẽ giả sử rằng $b_i \in m^{n-1}$ với mọi $i$ và $b_i \in m^n$ với $i < k$, rồi chứng minh rằng điều này kéo theo $b_k \in m^n$. Để làm điều đó, ta viết $f = \sum_{i=1}^{\infty} a_i X^i$ và so sánh các hệ số của $X^{s+k}$ trong (3); khi đó:
$$
(b_0 a_{s+k} + \cdots + b_{k-1} a_{s+1}) + b_k a_s + (b_{k+1} a_{s-1} + \cdots + b_{k+s} a_0) = 0.
$$
Các số hạng trong ngoặc thứ nhất thuộc $m^n$ vì $b_i \in m^n$ với $i < k$; tương tự đối với các số hạng trong ngoặc thứ hai, vì $b_i \in m^{n-1}$ với mọi $i$ và $a_i \in m$ với $i \leq s-1$. Do đó $b_k a_s \in m^n$ và, vì $a_s$ là một phần tử khả nghịch của $A$, $b_k \in m^n$.

(b) Ta chứng minh rằng $f \mid B + M = B$. Ta viết
$$
g = a_s + a_{s+1} X + a_{s+2} X^2 + \cdots;
$$
nó là một phần tử khả nghịch của $B$. Khi đó
$$
f - X^s g = a_0 + a_1 X + \cdots + a_{s-1} X^{s-1};
$$
vậy nếu ta viết $fg^{-1} - X^s = (f - X^s g) g^{-1} = -h$, thì các hệ số của $h$ thuộc $m$. Sau đó lấy $r$ là một phần tử của $B$. Bằng quy nạp theo $n$ ta định nghĩa một dãy $(q^{(n)})$ các phần tử của B: ta lấy $q^{(0)}$ là chuỗi duy nhất thỏa mãn:
$$
r \equiv X^s q^{(0)} \pmod{M};
$$
viết $h = \sum_{i=0}^m h_i X^i$ và $q^{(n)} = \sum_{i=0}^\infty q_i^{(n)} X^i$, các $q_i^{(n)}$ được định nghĩa bởi:
$$
q_i^{(n)} = \sum_{j=0}^{i+s} h_j q_{i+s-j}^{(n-1)}
$$
Từ (6) suy ra ngay lập tức rằng:
$$
X^s q^{(n)} \equiv h q^{(n-1)} \pmod{M}.
$$
Vì $h_j \in m$ với mọi $j$, từ (6) cũng suy ra, bằng quy nạp theo $n$, rằng $q_i^{(n)} \in m^n$ với mọi $i$ và mọi $n$. Vì A là đầy đủ, suy ra rằng chuỗi
$$
q^{(0)} + q^{(1)} + \ldots + q^{(n)} + \ldots
$$
hội tụ đến một phần tử $q$ của B. Theo (5) và (7),
$$
X^s(q^{(0)} + q^{(1)} + \ldots + q^{(n)}) \equiv r + h(q^{(0)} + \ldots + q^{(n-1)}) \pmod{M}.
$$
Vì M là đóng, ở giới hạn (8) cho $r \equiv (X^s - h)q \pmod{M}$, tức là
$$
r \in fg^{-1}q + M \subset fB + M.
$$
Ta cũng có thể dùng các kết quả của Chương III, § 2 để chứng minh quan hệ $B = fB + M$ (xem Bài tập 12). Phương pháp được theo ở đây có ưu điểm là áp dụng được cho các chuỗi hội tụ.

#### Hệ quả {#ac-vii-s3-n8-cor-1 .statement}

*Với các giả thiết và ký hiệu của Mệnh đề 5, giả sử rằng $s \geq 1$, sao cho $f \in Bm + BX$. Khi đó đồng cấu A-môđun $h$ từ $B' = A[[T]]$ vào $B = A[[X]]$ sao cho $h(T) = f$ (Chương III, § 2, no. 9, Mệnh đề 11 (a)) xác định trên B một cấu trúc $B'$-môđun tự do nhận $\{1, X, \ldots, X^{s-1}\}$ làm cơ sở. Đặc biệt $h$ là đơn ánh.*

Cho $B'$-môđun B được trang bị lọc (T)-adic, gồm các $f^n B$ với $n \geq 0$ (Chương 111, § 2, no. 1). Khi đó $B/fB$ là một môđun tự do trên vành $A = B'/TB'$ và các ảnh của $X^i$ ($0 \leq i \leq s-1$) trong A-môđun này tạo thành một cơ sở của nó (Mệnh đề 5); hơn nữa vì $f$ không là một ước của không trong B (Mệnh đề 5), $Bf^n/Bf^{n+1}$ cũng là một $(B'/TB')$-môđun tự do hạng s, nên điều kiện (GR) của Chương 111, § 2, no. 8 được thỏa mãn (thay thế A bởi B' và M bởi B). Mặt khác, vì B' là Hausdorff và đầy đủ đối với lọc (T)-adic và gr(B) là một gr(B')-môđun sinh hữu hạn theo điều trên, trước hết suy ra (Chương III, § 2, no. 9, Hệ quả 1 của Mệnh đề 12) rằng B là một B' môđun sinh hữu hạn. Mệnh đề thứ nhất của hệ quả khi đó suy ra từ Chương III, § 2, no. 9, Mệnh đề 13. Mệnh đề thứ hai suy ra ngay lập tức từ đó.

#### Định nghĩa 2 {#ac-vii-s3-def-2 .statement}

*Một đa thức* $F \in \mathbf{A}[X]$ *được gọi là phân biệt nếu nó có dạng*
$$
F = X^s + a_{s-1} X^{s-1} + \cdots + a_0,
$$
*trong đó* $a_i \in \mathfrak{m}$ *với* $0 \leq i \leq s - 1$.

Chú ý rằng tích của hai đa thức phân biệt là một đa thức phân biệt.

#### Mệnh đề 6 (Định lý chuẩn bị) {#ac-vii-s3-prop-6 .statement}

*Cho* $f \in B$ *là một chuỗi mà chuỗi rút gọn của nó khác không và* $s$ *là cấp rút gọn của nó. Khi đó tồn tại một cặp có thứ tự duy nhất* $(u, F)$ *sao cho* $u$ *là một phần tử khả nghịch của* $B$, $F$ *là một đa thức phân biệt bậc* $s$ *và* $f = uF$.

Ta viết $F = X^s + G$, trong đó $G = g_0 + \cdots g_{s-1} X^{s-1}$ ($g_i \in \mathbf{A}$). Quan hệ $f = uF$ tương đương với $F = u^{-1}f$, nghĩa là với $X^s = u^{-1}f - G$. Do đó Mệnh đề 5 cho thấy tính duy nhất của $G$ và $u^{-1}$, và vì thế của $F$ và $u$. Nó cũng cho thấy rằng tồn tại $v \in B$ và một đa thức $G = g_0 + \cdots + g_{s-1} X^{s-1}$ ($g_i \in \mathbf{A}$) sao cho $X^s = v - G$; còn phải chỉ ra rằng $v$ khả nghịch trong $B$ và $g_i \in \mathfrak{m}$ với mọi $i$. Bây giờ, ký hiệu $\bar{g}_i$ là ảnh chính tắc của $g_i$ trong $k$ và $\bar{f}, \bar{v}$ là các chuỗi rút gọn của $f, g$,
$$
X^s + \bar{g}_0 + \bar{g}_1 X + \cdots + \bar{g}_{s-1} X^{s-1} = \bar{f} \bar{v};
$$
vì $\bar{f}$ có cấp $s$, nên $\bar{g}_i = 0$ với mọi $i$ và $\bar{v}$ có cấp 0, do đó $v$ là khả nghịch.

#### Mệnh đề 7 {#ac-vii-s3-prop-7 .statement}

*Cho* $F$ *là một đa thức phân biệt và* $g, h$ *là hai chuỗi lũy thừa hình thức của* $B$ *sao cho* $F = gh$. *Khi đó tồn tại một phần tử khả nghịch* $u$ *của* $B$ *sao cho* $ug$ *và* $u^{-1}h$ *là các đa thức phân biệt và* $F = (ug)(u^{-1}h)$.

Thật vậy, các chuỗi rút gọn của $g$ và $h$ đều $\neq 0$; do đó, theo Mệnh đề 6, tồn tại các phần tử khả nghịch $u, v$ của $B$ sao cho $ug$ và $vh$ là các đa thức phân biệt. Khi đó $uvF = (ug)(vh)$ là một đa thức phân biệt và $uv$ là khả nghịch. Chuyển qua các chuỗi rút gọn, thấy ngay lập tức rằng $F$ và $uvF$ có cùng cấp rút gọn, nghĩa là cùng bậc. Mệnh đề về tính duy nhất trong Mệnh đề 6 vì thế cho thấy rằng $F = uvF$, do đó $uv = 1$.

#### Hệ quả {#ac-vii-s3-n8-cor-2 .statement}

*Giả sử thêm rằng* $\mathbf{A}$ *là một miền nguyên và* $F$ *là một đa thức phân biệt bậc* $s$. *Để* $F$ *là extremal trong* $\mathbf{A}[X]$, *điều kiện cần và đủ là nó là extremal trong* $B = \mathbf{A}[[X]]$.

Giả sử $F$ không là phần tử extremal trong $\mathbf{A}[X]$, nên $F = f_1 f_2$, trong đó $f_1$ và $f_2$ là các phần tử không khả nghịch của $\mathbf{A}[X]$; tích của các hệ số đầu của $f_1$ và $f_2$ bằng 1, nên các hệ số này khả nghịch trong $\mathbf{A}$ và giả thiết kéo theo rằng $f_1$ và $f_2$ có bậc $> 0$ và $< s$; vì các đa thức rút gọn $\bar{f}_1, \bar{f}_2$ thỏa mãn $\bar{f}_1 \bar{f}_2 = X^s$, nên cả $\bar{f}_1$ lẫn $\bar{f}_2$ đều không thể khả nghịch trong $k[[X]]$, vì nếu $\bar{f}_1$ khả nghịch thì $\bar{f}_2$ sẽ có cấp $s$, điều này phi lý. *A fortiori*, cả $f_1$ lẫn $f_2$ đều không khả nghịch trong $B$ và $F$ không là phần tử extremal trong $B$.

Ngược lại, nếu F không là phần tử extremal trong $A[[X]]$, thì $F = gh$, trong đó cả g lẫn h đều không khả nghịch trong B; do đó các cấp rút gọn của chúng đều $\geq 1$; khi ấy các đa thức distinguished $ug$ và $u^{-1}h$ của Mệnh đề 7 không phải là các hằng, điều đó cho thấy F không là phần tử extremal trong $A[X]$.

### 9. TÍNH PHÂN TÍCH DUY NHẤT CỦA CÁC VÀNH CHUỖI LŨY THỪA HÌNH THỨC

#### Mệnh đề 8 {#ac-vii-s3-prop-8 .statement}

Cho C là một vành, hoặc là một trường, hoặc là một vành định giá rời rạc. Khi đó miền các chuỗi lũy thừa hình thức $C[[X_1, \ldots, X_n]]$ là phân tích duy nhất.

Gọi $p$ là iđêan cực đại của C và $x$ là một phần tử sinh của $p$ (nếu C là một trường thì $\pi = 0$). Trang bị cho C tôpô $p$-adic, tôpô này là Hausdorff. Vì C là một vành địa phương Noether, $B = C[[X_1, \ldots, X_n]]$ là một vành địa phương Noether và đầy đủ hóa của nó là $\hat{C}[[X_1, \ldots, X_n]]$ (Chương III, §2, no. 6, Mệnh đề 6). Theo Hệ quả của Mệnh đề 4 (no. 6), chỉ cần chứng minh rằng $\hat{C}[[X_1, \ldots, X_n]]$ là phân tích duy nhất. Bây giờ, nếu C là một trường thì $\hat{C} = C$; nếu C là một vành định giá rời rạc thì $\hat{C}$ cũng có tính chất ấy (Chương VI, §5, no. 3, Mệnh đề 5). Do đó, trong phần còn lại của chứng minh, ta sẽ giả sử rằng C là đầy đủ.

Lập luận bằng quy nạp, bắt đầu từ trường hợp tầm thường $n = 0$, ta sẽ giả sử rằng đã chứng minh được $A = C[[X_1, \ldots, X_{n-1}]]$ là phân tích duy nhất. Ta sẽ đồng nhất B với $A[[X_n]]$ và ký hiệu bởi m iđêan cực đại của A (được sinh bởi $\pi, X_1, \ldots, X_{-1}$). Ta sẽ chứng minh rằng mọi phần tử khác không g của B đều là, theo một cách duy nhất về bản chất, một tích các phần tử extremal.

Cho K là trường $C/C\pi$; vì $B/B\pi$ được đồng nhất với $K[[X_1, \ldots, X_n]]$, iđêan $Bx$ là nguyên tố và $x$ là cực biên. Nếu $x \neq 0$, do đó $B_{B\pi}$ là vành của một định giá rời rạc chuẩn hóa w (Chương VI, §3, no. 6, Mệnh đề 9); bởi vậy mọi phần tử khác không g của B đều có thể viết dưới dạng $g = \pi^{w(g)} f$, trong đó $f \in B$ và f không là bội của $\pi$. Vì vậy sẽ đủ để chỉ ra rằng $f$ là một tích về cơ bản duy nhất của các phần tử cực biên. Bây giờ ảnh chính tắc của $f$ trong $K[[X_1, \ldots, X_n]]$ khác không; do đó Bổ đề 3 (no. 7) cho thấy rằng tồn tại một tự đẳng cấu của B biến $f$ thành một phần tử $f'$ sao cho các hệ số của $f'(0, \ldots, 0, X,)$ không phải tất cả đều nằm trong $Cx$; điều đó có nghĩa là các hệ số của chuỗi $f'$, được xét như một chuỗi lũy thừa hình thức theo $X,,$, không phải tất cả đều nằm trong m. Sẽ đủ để chứng minh mệnh đề của chúng ta đối với $f'$.

Trong phần sau, mọi phần tử của B sẽ được xét như các chuỗi lũy thừa hình thức theo X, với các hệ số trong A. Theo Mệnh đề 6 của no. 8 (áp dụng được vì C và do đó A là tách được và đầy đủ và chuỗi thu gọn của $f'$ là $\neq 0$), $f'$ liên kết, trong B, với một đa thức phân biệt duy nhất F. Theo Mệnh đề 7 của no. 8, mọi chuỗi chia hết $f'$ (hay, điều này tương đương, chia hết F) đều liên kết với một đa thức phân biệt chia hết F và mọi phân tích của $f'$ đều, sai khác bởi các nhân tử khả nghịch, có dạng $f' = u F_1 \cdots F_q$, trong đó $u$ là khả nghịch và các $F_i$ là các đa thức phân biệt cực biên (trong B) sao cho $F = F_1 \cdots F_q$. Theo Hệ quả của Mệnh đề 7 của no. 8, các F, cũng là cực biên trong $\mathbf{A}[X_n]$. Bây giờ, vì $\mathbf{A}$ là phân tích được duy nhất theo giả thiết quy nạp, nên $\mathbf{A}[X_n]$ cũng vậy (Định lý 2, no. 5); do đó, vì chúng là đơn nhất, các $F_i$ được xác định duy nhất bởi F (chính xác đến một phép hoán vị). Điều này chứng tỏ tính duy nhất của phân tích $f' = u F_1 \ldots F_r$; sự tồn tại của nó suy ra từ việc $B$ là Noether, điều này hoàn tất chứng minh.

Nhận xét
(1) Tồn tại các vành phân tích được duy nhất $\mathbf{A}$ sao cho vành $\mathbf{A}[[X]]$ không phân tích được duy nhất (Bài tập 8). Tuy nhiên, nếu $\mathbf{A}$ là một miền iđêan chính, thì $\mathbf{A}[[X_1, \ldots, X_n]]$ phân tích được duy nhất (Bài tập 9).
(2) \* Về sau chúng ta sẽ thấy, bằng các phương pháp đồng điều, rằng mọi vành địa phương chính quy đều phân tích được duy nhất (xem § 4, no. 7, Hệ quả 3 của Mệnh đề 16). Điều này sẽ cho một chứng minh khác, đơn giản hơn về mặt ý niệm, của Mệnh đề 8. \*
