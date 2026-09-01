---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 1
section_title: Finitely generated graded algebras
lang: vi
source: ac-i-vii
book_pages: 155-162, 232-233
pdf_pages: 0175-0182, 0252-0253
extraction: ocr
subsections:
    - "no": 1
      title: SYSTEMS OF GENERATORS OF A COMMUTATIVE ALGEBRA
      page: 155
      pdf_page: 175
    - "no": 2
      title: Criteria of Finiteness for Graded Rings
      page: 156
      pdf_page: 176
    - "no": 3
      title: PROPERTIES OF THE RING $A^{(d)}$
      page: 157
      pdf_page: 177
    - "no": 4
      title: GRADED PRIME IDEALS
      page: 160
      pdf_page: 180
statements: 13
exercises: 3
content_sha256: 15f8cd9e1594a60f1a1ad01ad3f76deda9bb9795e70852d02b09b26a70da971b
translated_from: content/en/ac/III/01_s1_finitely_generated_graded_algebras.md
source_content_sha256: f5a839fc9eb2de4a6348015dd8cd693291996b095c75da79331ecfb76c8dfc47
translation_model: gpt-5.4
translation_run: translate-vi-78d3ca82
glossary_version: 34
glossary_terms_sha256: bf1d69339648eb617cc610fc547fbfe8af6efff88c28668ace904fc7cded5e19
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. ĐẠI SỐ PHÂN BẬC SINH HỮU HẠN

### 1. CÁC HỆ SINH CỦA MỘT ĐẠI SỐ GIAO HOÁN

Cho $\mathbf{A}$ là một vành giao hoán và $\mathbf{B}$ là một $\mathbf{A}$-đại số giao hoán. Nhắc lại (Đại số, Chương IV, § 2, no. 1) rằng nếu $x = (x_i)_{i \in I}$ là một họ các phần tử của $\mathbf{B}$, thì ánh xạ $f \mapsto f(x)$ từ đại số đa thức $\mathbf{A}[X_i]_{i \in I}$ vào $\mathbf{B}$ là một đồng cấu của $\mathbf{A}[X_i]_{i \in I}$ lên đại số con của $\mathbf{B}$ sinh bởi các $x_i$, có hạt nhân $a$ là iđêan các đa thức $f$ sao cho $f(x) = 0$, được gọi là *iđêan các quan hệ đại số (với hệ số trong $\mathbf{A}$) giữa các $x_i$*.

#### Định nghĩa 1 {#ac-iii-s1-def-1 .statement}

*Trong một đại số giao hoán $\mathbf{B}$ trên một vành giao hoán $\mathbf{A}$, một họ $(x_i)_{i \in I}$ các phần tử của $\mathbf{B}$ được gọi là tự do đại số trên $\mathbf{A}$ (hoặc các $x_i$ được gọi là độc lập đại số trên $\mathbf{A}$) nếu iđêan các quan hệ đại số giữa các $x_i$, với hệ số trong $\mathbf{A}$, thu về 0. Một họ $(x_i)$ không tự do đại số trên $\mathbf{A}$ cũng được gọi là liên hệ đại số (hoặc các phần tử của nó cũng được gọi là phụ thuộc đại số trên $\mathbf{A}$).*

Định nghĩa này khái quát hoá định nghĩa đã cho trong Đại số, Chương V, § 5, no. 1, Định nghĩa 1 đối với các họ phần tử của một trường giao hoán.

(*) Trừ ở § 5, nơi sử dụng các kết quả của Chương I, § 4 và do đó của đại số đồng điều, trong chương này không dùng đến sách nào khác ngoài các Quyển I đến VI và các Chương I và II của quyển này.

Nói rằng một họ $(x_i)_{i \in I}$ là tự do đại số trên $A$ tương đương với nói rằng các đơn thức $\prod_i x_i^{n_i}$ theo các $x$, là *độc lập tuyến tính* trên $A$; đặc biệt các $x_i$ khi đó độc lập tuyến tính trên $A$.

#### Định nghĩa 2 {#ac-iii-s1-def-2 .statement}

*Một đại số giao hoán* $B$ *trên một vành giao hoán* $A$ *được gọi là sinh hữu hạn nếu nó được sinh bởi một họ hữu hạn phần tử.*

Điều đó tương đương với nói rằng $B$ đẳng cấu với một $A$-đại số có dạng $A[X_1, \ldots, X_n]/a$ (trong đó các $X_i$ là các bất định thức và $a$ là một iđêan của vành đa thức $A[X_1, \ldots, X_n]$).

Nếu $A$-đại số $B$ là một *$A$-môđun sinh hữu hạn*, thì hiển nhiên nó là một $A$-đại số sinh hữu hạn; đảo lại là sai như ví dụ các đại số đa thức cho thấy (xem Chương V).

Nếu $B$ là một $A$-đại số sinh hữu hạn và $A'$ là một $A$-đại số giao hoán bất kỳ, thì $B_{(A')} = B \otimes_A A'$ là một $A'$-đại số sinh hữu hạn, vì nếu $(x_i)_{i \in I}$ là một hệ sinh của $A$-đại số $B$, thì rõ ràng các $x, \otimes 1$ tạo thành một hệ sinh của $A$-đại số $B_{(A')}$.

Nếu $B$ là một $A$-đại số sinh hữu hạn và $C$ là một $B$-đại số sinh hữu hạn, thì $C$ là một $A$-đại số sinh hữu hạn; vì từ các định nghĩa suy ra ngay lập tức rằng nếu $(b_\lambda)_{\lambda \in L}$ là một hệ sinh của $A$-đại số $B$ và $(c_\mu)_{\mu \in M}$ là một hệ sinh của $B$-đại số $C$, thì mọi phần tử của $C$ đều bằng một đa thức, với các hệ số trong $A$, theo các $b_\lambda$ và các $c_\mu$.

### 2. Các tiêu chuẩn hữu hạn đối với các vành phân bậc

*Trong số này và số tiếp theo, mọi phân bậc được xét đến (Đại số, Chương II, § 11) đều được giả sử là kiểu* $\mathbf{Z}$. *Nếu* $A$ *(tương ứng M)* *là một vành phân bậc* (tương ứng *môđun phân bậc*), $A_i$ (tương ứng $M_i$) *sẽ kí hiệu tập hợp các phần tử thuần nhất bậc* $i$ *trong* $A$ *(tương ứng M)*.

*Nếu* $A_i = \{0\}$ *(tương ứng $M_i = \{0\}$) với* $i < 0$, $A$ *(tương ứng M)* *sẽ, để viết gọn, được gọi là một vành phân bậc* (tương ứng *môđun*) *có các bậc dương*.

#### Mệnh đề 1 {#ac-iii-s1-prop-1 .statement}

*Cho* $A = \bigoplus_{i \in \mathbf{Z}} A_i$ *là một vành giao hoán phân bậc có các bậc dương, m là iđêan phân bậc* $\bigoplus_{i \geq 1} A_i$ *và* $(x_\lambda)_{\lambda \in L}$ *là một họ các phần tử thuần nhất của* $A$ *có bậc* $\geq 1$. *Các điều kiện sau là tương đương*:

(a) *Iđêan của* $A$ *do họ* $(x_\lambda)$ *sinh ra bằng* $m$.

(b) *Họ* $(x_\lambda)$ *là một hệ sinh của* $A$*-đại số* $A$.

(c) *Với mọi* $i \geq 0$, *thì* $A$*-môđun* $A_i$ *được sinh bởi các phần tử có dạng* $\prod_\lambda x_\lambda^{n_\lambda}$ *mà có bậc* $i$ *trong* $A$*.

Rõ ràng các điều kiện (b) và (c) là tương đương. Nếu chúng đúng, mọi phần tử của m đều có dạng $f((x_i))$ trong đó $f$ là một đa thức của $A_0[X_\lambda]_{\lambda \in L}$ không có số hạng hằng; khi đó $m = \sum_{\lambda \in L} A x_\lambda$, điều này chứng tỏ rằng (c) kéo theo (a). Ngược lại, giả sử rằng điều kiện (a) đúng. Gọi $A' = A_0[x_\lambda]_{\lambda \in L}$ là đại số con-A, của A được sinh bởi họ $(x_\lambda)$ và hãy chỉ ra rằng $A' = A$. Để làm điều này, chỉ cần chỉ ra rằng $A_i \subset A$ với mọi $i \geq 0$. Ta tiến hành bằng quy nạp theo $i$, tính chất là hiển nhiên đối với $i = 0$. Bây giờ lấy $y \in A$, với $i \geq 1$. Vì $y \in m$, tồn tại một họ $(a_\lambda)_{\lambda \in L}$ các phần tử của A có giá hữu hạn sao cho $y = \sum_\lambda a_\lambda x_\lambda$ và ta có thể giả sử rằng mỗi $a_\lambda$ là thuần nhất bậc $i - \deg(x_\lambda)$ (nếu cần thì thay thế nó bằng thành phần thuần nhất bậc đó của nó); vì $\deg(x_\lambda) > 0$, giả thiết quy nạp cho thấy rằng $a_\lambda \in A'$ với mọi $\lambda \in L$, do đó $y \in A'$ và $A_i \subset A'$, điều này chứng tỏ rằng (a) kéo theo (b).

#### Hệ quả {#ac-iii-s1-n2-cor-1 .statement}

*Cho* $A = \bigoplus_{i \in \mathbf{Z}} A_i$, *là một vành giao hoán phân bậc với các bậc dương* và $m$ *là iđêan phân bậc*, $\bigoplus_{i \geq 1} A_i$.

(i) *Các điều kiện sau là tương đương*:
(a) *Iđêan* $m$ *là một A-môđun hữu hạn sinh*.
(b) *Vành* $A$ *là một A,-môđun hữu hạn sinh*.

(ii) *Giả sử rằng các điều kiện trong (i) được thỏa mãn và cho* $M = \bigoplus_{i \in \mathbf{Z}} M_i$ *là một A-môđun phân bậc hữu hạn sinh. Khi đó, với mọi* $i \in \mathbf{Z}$, $M_i$ *là một A,-môđun hữu hạn và tồn tại* $i_0$ *sao cho* $M_i = \{0\}$ *với* $i < i_0$.

(i) Nếu một họ $(y_\mu)$ các phần tử của A là một hệ sinh của A-môđun m (resp. của A,-môđun A), thì họ gồm các thành phần thuần nhất của các $y_\mu$ cũng vậy; khi đó tính tương đương của các điều kiện (a) và (b) suy ra từ Mệnh đề 1.

(ii) Ta có thể giả sử rằng A được sinh (như một A,-đại số) bởi các phần tử thuần nhất $a_i$ ($1 < i < r$) bậc $> 1$ và M được sinh (như một A-môđun) bởi các phần tử thuần nhất $x_j$ ($1 < j < s$); gọi $h_i = \deg(a_i), k_j = \deg(x_j)$. Rõ ràng M, gồm các tổ hợp tuyến tính với hệ số trong $A_0$ của các phần tử $a_1^{\alpha_1} a_2^{\alpha_2} \ldots a_r^{\alpha_r} x_j$ sao cho các $\alpha_i$ là các số nguyên $\geq 0$ thỏa mãn quan hệ $k_j + \sum_{i=1}^r \alpha_i h_i = n$; với mỗi $n$ chỉ có một số hữu hạn các họ $(\alpha_i)_{1 \leq i \leq r}$ thỏa mãn các điều kiện đó, vì $h_i \geq 1$ với mọi $i$; ta kết luận rằng $M_n$ là một A,-môđun hữu hạn sinh và hơn nữa hiển nhiên $M_n = \{0\}$ khi $n < \inf(k_j)$.

### 3. CÁC TÍNH CHẤT CỦA VÀNH $A^{(d)}$

Cho $A = \bigoplus_{i \in \mathbf{Z}} A_i$, là một vành phân bậc và $M = \bigoplus_{i \in \mathbf{Z}} M_i$ là một A-môđun phân bậc; với mọi cặp có thứ tự các số nguyên $(d, k)$ sao cho $d \geqslant 1$ và $0 \leqslant k \leqslant d - 1$, đặt

$$
A^{(d)} = \bigoplus_{i \in \mathbf{Z}} A_{id}, \quad M^{(d, k)} = \bigoplus_{i \in \mathbf{Z}} M_{id + k}.
$$

Rõ ràng $A^{(d)}$ là một vành con phân bậc của $A$ và $M^{(d, k)}$ là một $A^{(d)}$-môđun phân bậc; hơn nữa, nếu $N$ là một môđun con phân bậc của $M$, thì $N^{(d, k)}$ là một môđun con phân bậc dưới-$A^{(d)}$ của $M^{(d, k)}$. Ta sẽ viết $M^{(d)}$ thay cho $M^{(d, 0)}$; với mỗi $d \geqslant 1$, $M$ là tổng trực tiếp của các $A^{(d)}$-môđun $M^{(d, k)}$ $(0 \leqslant k \leqslant d - 1)$.

#### Mệnh đề 2 {#ac-iii-s1-prop-2 .statement}

*Cho $A = \bigoplus_{i \in \mathbf{Z}} A_i$ là một vành giao hoán phân bậc với các bậc dương và $M = \bigoplus_{i \in \mathbf{Z}} M_i$ là một $A$-môđun phân bậc. Giả sử rằng $A$ là một $A_0$-đại số sinh hữu hạn và $M$ là một $A$-môđun sinh hữu hạn. Khi đó, với mọi cặp có thứ tự $(d, k)$ các số nguyên sao cho $d \geqslant 1, 0 \leqslant k \leqslant d - 1)$:*

(i) $A^{(d)}$ là một $A$-môđun sinh hữu hạn.
(ii) $M^{(d, k)}$ là một $A^{(d)}$-môđun sinh hữu hạn.

Ta hãy chỉ ra rằng $A$ là một *$A^{(d)}$-môđun sinh hữu hạn*. Cho $(a_i)_{1 \leqslant i \leqslant s}$ là một hệ sinh của $A$-đại số $A$ gồm các phần tử thuần nhất. Các phần tử của $A$ (hữu hạn về số lượng) có dạng $a_1^{\alpha_1} a_2^{\alpha_2} \ldots a_s^{\alpha_s}$ sao cho $0 \leqslant \alpha_i \leqslant d$ với $1 \leqslant i \leqslant s$ tạo thành một hệ sinh của $A$ như một $A^{(d)}$-môđun; với mọi hệ số nguyên $n_i \geqslant 0$ $(1 \leqslant i \leqslant s)$, tồn tại các số nguyên dương $q_i, r_i$ sao cho $n_i = q_i d + r_i$ với $r_i < d$ $(1 \leqslant i \leqslant s)$; khi đó

$$
a_1^{n_1} a_2^{n_2} \ldots a_s^{n_s} = (a_1 \ldots a_s^{q_s})^d (a_1^{r_1} \ldots a_s^{r_s})
$$

điều này chứng minh mệnh đề của ta, vì mọi phần tử thuần nhất $x \in A$ đều thỏa $x^d \in A^{(d)}$. Khi đó, nếu $M$ là một $A$-môđun sinh hữu hạn, thì nó cũng là một $A^{(d)}$-môđun sinh hữu hạn; vì $M$ là tổng *trực tiếp* của các $M^{(d, k)}$ $(0 < k < d - 1)$, nên mỗi $M^{(d, k)}$ là một $A^{(d)}$-môđun sinh hữu hạn, điều này chứng minh (ii).

Áp dụng điều trên cho A-môđun phân bậc $m = \bigoplus_{i \geqslant 1} A_i$, môđun này sinh hữu hạn theo Hệ quả của Mệnh đề 1 ở no. 2; ta thấy rằng $m^{(d)}$ là một $A^{(d)}$-môđun sinh hữu hạn; do đó (no. 2, Hệ quả của Mệnh đề 1) $A^{(d)}$ là một A-đại số sinh hữu hạn.

#### Bổ đề 1 {#ac-iii-s1-lem-1 .statement}

*Cho $A$ là một vành giao hoán phân bậc sao cho $A = A_0[A_1]$, $M$ là một A-môđun phân bậc và $(y_\lambda)_{\lambda \in L}$ là một hệ các phần tử sinh thuần nhất của $M$ sao cho $\deg(y_\lambda) \leqslant n_0$ với mọi $\lambda \in L$. Khi đó, với mọi $n \geqslant n_0$ và mọi $k \geqslant 0$, $M_{n+k} = A_k \cdot M_n$.*

Cho $n \geqslant n_0$ và $x \in M_n$. Vì các $y_\lambda$ sinh $M$, tồn tại một họ $(a_\lambda)_{\lambda \in L}$ các phần tử của $A$ có giá hữu hạn sao cho $x = \sum_\lambda a_\lambda y_\lambda$; hơn nữa ta có thể giả sử mỗi $a_\lambda$ là thuần nhất và có bậc $n + 1 - \deg(y_\lambda)$ (nếu cần thì thay thế nó bằng thành phần thuần nhất ở bậc đó). Vì

$A = A_0[A_1]$ và $\deg(a_\lambda) > 0$, mỗi $a_\lambda$ là một tổng các phần tử dạng $bb'$ với $b \in A_0, b' \in A$, do đó $x \in A_1 M_n$. Khi đó $M_{n+1} = A_1 M_n$, do đó $M_{n+k} = A_k M_n$ bằng quy nạp theo $k$.

#### Bổ đề 2 {#ac-iii-s1-lem-2 .statement}

*Cho $A$ là một vành giao hoán phân bậc sao cho $A = A_0[A_1]$ và cho $S = \bigoplus_{i \geq 0} S_i$, là một A-đại số giao hoán phân bậc với các bậc dương, đồng thời là một A-môđun sinh hữu hạn. Khi đó tồn tại một số nguyên $n_0 \geq 0$ sao cho:*

(i) *Với $n \geq n_0$ và $k \geq 0$, $S_{n+k} = S_k \cdot S_n$.*
(ii) *Với $d \geq n_0$, $S^{(d)} = S_0[S_d]$.*

Theo Bổ đề 1 tồn tại một số nguyên $n_0 \geq 0$ sao cho, với $n \geq n_0$ và $k \geq 0$, $S_{n+k} = A_k S_n$, do đó a fortiori $S_{n+k} = S_k S_n$, điều này thiết lập (i). Khi đó, với $d \geq n_0$ và $m > 0$, $S_{m d} = (S_d)^m$ như suy ra bằng quy nạp theo $m$ khi áp dụng (i); điều này thiết lập (ii).

#### Mệnh đề 3 {#ac-iii-s1-prop-3 .statement}

*Cho $R = \bigoplus_{i \geq 0} R_i$, là một vành giao hoán phân bậc với các bậc dương, là một $R_0$-đại số sinh hữu hạn. Tồn tại một số nguyên $e \geq 1$ sao cho $R^{(me)} = R_0[R_{me}]$ với mọi $m \geq 1$.*

Cho $(x_j)_{1 \leq j \leq s}$ là một hệ sinh thuần nhất của $R_0$-đại số $R$, có các bậc $\geq 1$. Đặt $h_j = \deg(x_j)$, lấy $q$ là một bội chung của các $h_j$ và viết $q_j = q/h_j$ với $1 \leq j \leq s$; khi đó các phần tử $x_j^{q_j}$ đều có bậc $q$. Gọi $B$ là đại số con-$R_0$ của $R$ sinh bởi các $x_j^{q_j}$; đó là một đại số con phân bậc của $R$ và $B_i = 0$ nếu $i$ không là bội của $q$. Gọi $A$ (tương ứng $S$) là vành phân bậc có vành nền là $B$ (tương ứng $R^{(q)}$) và có phân bậc gồm các $A_i = B_{iq}$ (tương ứng $S_i = R_{iq}$). Khi đó $A = A_0[A_1]$ theo định nghĩa của $B$. Xét các phần tử của $R$ (hữu hạn về số lượng) có dạng $x_1^{\alpha_1} x_2^{\alpha_2} \ldots x_s^{\alpha_s}$, trong đó $0 \leq \alpha_j \leq q_j$ và $\alpha_1 h_1 + \ldots + \alpha_s h_s \equiv 0$ (mod. $q$); ta sẽ chứng minh rằng chúng sinh $R^{(q)}$-môđun $B$. Chỉ cần chứng minh rằng mọi phần tử của $R^{(q)}$ có dạng $x_1^{n_1} x_2^{n_2} \ldots x_s^{n_s}$ là một tổ hợp tuyến tính trên $B$ của các phần tử ở trên. Thật vậy, tồn tại các số nguyên dương $k_j, r_j$ sao cho $n_j = k_j q_j + r_j$ với $r_j < q_j$ ($1 \leq j \leq s$); khi đó

$$
x_1^{n_1} x_2^{n_2} \ldots x_s^{n_s} = (x_1^{q_1})^{k_1} \ldots (x_s^{q_s})^{k_s} \cdot (x_1^{r_1} \ldots x_s^{r_s})
$$

và theo giả thiết $\sum_{j=1}^s n_j h_j \equiv 0$ (mod. $q$), do đó $\sum_{j=1}^s r_j h_j \equiv 0$ (mod. $q$); vì các $x_j^{q_j}$ thuộc $B$ theo định nghĩa, điều này chứng minh mệnh đề của ta. Vì $S$ là một $A$-môđun sinh hữu hạn, có thể áp dụng Bổ đề 2: tồn tại $n_0$ sao cho với $d > n_0$, $S^{(d)} = S_0[S_d]$ và do đó $R^{(qd)} = R_0[R_{qd}]$ với $d \geq n_0$. Mệnh đề được suy ra với $e = q n_0$.

### 4. IĐÊAN NGUYÊN TỐ PHÂN BẬC

Cho $A = \bigoplus_{i \geq 0} A_i$ là một vành giao hoán phân bậc với các bậc *dương* và $m$ là iđêan phân bậc $\bigoplus_{i \geq 1} A_i$; ta sẽ gọi hai iđêan phân bậc $a = \bigoplus_{i \geq 0} a_i, b = \bigoplus_{i \geq 0} b_i$ của $A$ là *tương đương* nếu tồn tại một số nguyên $n_0$ sao cho $a_n = b_n$ với $n \geq n_0$ (rõ ràng đó là một quan hệ tương đương). Một iđêan phân bậc được gọi là *cốt yếu* nếu nó không tương đương với $m$.

#### Mệnh đề 4 {#ac-iii-s1-prop-4 .statement}

*Cho $p = \bigoplus_{i \geq 0} p_i$ là một iđêan phân bậc của $A$; để $p$ là nguyên tố, điều kiện cần và đủ là, nếu $x \in A, \ y \in A,$ thỏa mãn $x \notin p$ và $y \notin p,$ thì $xy \notin p$.*

Điều kiện này hiển nhiên là cần thiết. Ngược lại, nếu nó được thỏa mãn, thì trong vành phân bậc $A/p = \bigoplus_{i \geq 0} A_i/p_i$ tích của hai phần tử thuần nhất $\neq 0$ là $\neq 0$ và do đó $A/p$ là một miền nguyên (*Algebra*, Chương II, § 11, no. 4, Mệnh đề 7).

#### Mệnh đề 5 {#ac-iii-s1-prop-5 .statement}

*Cho $a = \bigoplus_{i \geq 0} a_i$ là một iđêan phân bậc của $A$ và $n_0$ là một số nguyên $> 0$. Để tồn tại một iđêan nguyên tố phân bậc $p = \bigoplus_{i \geq 0} p_i$ sao cho $p_{n_0} = a,$ với $n \geq n_0,$ điều kiện cần và đủ là, đối với mọi cặp phần tử thuần nhất $x, y$ có bậc $\geq n_0,$ hệ thức $xy \in a$ kéo theo '"$x \in a$ hoặc $y \in a$". Nếu tồn tại $n \geq n_0$ sao cho $a_n \neq A_n,$ thì iđêan nguyên tố thỏa mãn các điều kiện trên là duy nhất.*

Điều kiện của mệnh đề hiển nhiên là cần thiết. Nếu $a_n = A_n$ với mọi $n \geq n_0,$ thì hiển nhiên mọi iđêan nguyên tố chứa $m$ đều là một nghiệm của bài toán; do đó có thể có nhiều iđêan nguyên tố giải bài toán; tuy nhiên, hai iđêan bất kỳ trong số đó hiển nhiên là tương đương. Vậy giả sử tồn tại một phần tử thuần nhất $a \in A_d$ (với $d \geq n_0$) không thuộc $a_d$. Gọi $p$ là tập hợp các $x \in A$ sao cho $ax \in a$. Rõ ràng $p$ là một iđêan của $A$; vì các thành phần thuần nhất của $ax$ là các tích với $a$ của các thành phần thuần nhất của $x$ và $a$ là một iđêan phân bậc, nên $p$ là một iđêan phân bậc; hơn nữa, $1 \notin p$ và do đó $p \neq A$. Để chứng minh rằng $p$ là nguyên tố, chỉ cần chỉ ra rằng, nếu $x \in A, \ y \in A,$ thỏa mãn $x \notin p$ và $y \notin p,$ thì $xy \notin p$ (Mệnh đề 4). Khi đó $ax \notin a_{m+d}, ay \notin a_{n+d},$ do đó theo giả thiết

$$
a^2xy \notin a_{m+n+2d};
$$

ta kết luận rằng $axy \notin a_{m+n+d}$ vì $xy \notin p$. Cuối cùng, nếu $n \geq n_0$ và $x \in A_n,$ thì các điều kiện $x \in a,$ và $ax \in a_{n+d}$ là tương đương theo giả thiết, và do đó $p \cap A_n = a_n$, điều này hoàn tất chứng minh về sự tồn tại của iđêan nguyên tố phân bậc $p$ giải quyết bài toán. Nếu thêm nữa $p'$ là một iđêan nguyên tố phân bậc khác của $A$ sao cho $p' \cap A_n = a_n$ với $n \geq n_0,$ thì $a \notin p'$ và $ax \in p'$ với mọi $x \in p,$ do đó $p \subset p'$ vì $p'$ là nguyên tố. Mặt khác, nếu $x$ là một phần tử thuần nhất bậc $n \geq 0$ của $p',$ thì $ax$ là thuần nhất bậc $n + d \geq n_0$ và vì thế thuộc $p' \cap A_{n+d} = a_{n+d}$, do đó theo định nghĩa ta có $x \in p$, điều này cho thấy $p' \subset p$ và cuối cùng $p' = p$.

#### Mệnh đề 6 {#ac-iii-s1-prop-6 .statement}

*Cho d là một số nguyên $\geq 1$.*

(i) *Với mọi iđêan phân bậc cốt yếu p của A, $p \cap A^{(d)}$ là một iđêan nguyên tố phân bậc cốt yếu của $A^{(d)}$.*

(ii) *Ngược lại, với mọi iđêan nguyên tố phân bậc cốt yếu $p'$ của $A^{(d)}$, tồn tại một iđêan nguyên tố phân bậc duy nhất (tất yếu là cốt yếu) $p$ của A sao cho $p \cap A^{(d)} = p'$.*

(i) Nếu $a \in A_k$ không thuộc $p_k$, thì $a^{kd}$ không thuộc $p_{kd}$ và do đó $p \cap A^{(d)}$ là cốt yếu.

(ii) Với mọi $n \geq 0$, tập $p \cap A$ phải bằng tập $a_n$ các $x \in A$ sao cho $x^d \in p'$. Hãy chỉ ra rằng $a = \bigoplus_{n \geq 0} a_n$ là một iđêan nguyên tố phân bậc; vì $a_n = p'_n$ khi $n$ là một bội của $d$, do $p'$ là nguyên tố, điều này sẽ chứng minh tính duy nhất của $p$. Thật vậy, nếu $x \in a_n$, $y \in a_m$, thì $(x - y)^{2d}$ là tổng của các hạng tử mà mỗi hạng tử là một tích của $x^d$ hoặc $y^d$ với một phần tử thuần nhất bậc $nd$ và do đó $(x - y)^{2d} \in p'$, và vì $p'$ là nguyên tố, $(x - y)^d \in p'$ và bởi vậy $a_n$ là một nhóm con của $A$. Vì $p'$ là một iđêan của $A^{(d)}$, $a$ là một iđêan phân bậc của $A$; cuối cùng, quan hệ $(xy)^d \in p'$ suy ra $x^d \in p'$ hoặc $y^d \in p'$, điều này hoàn tất chứng minh theo Mệnh đề 4.

Cho $A$ là một vành giao hoán phân bậc với các bậc dương và $p$ là một iđêan nguyên tố phân bậc cốt yếu của $A$. Tập $S$ các phần tử *thuần nhất* của $A$ không thuộc $p$ là tập nhân tính và do đó vành phân thức $S^{-1}A$ được phân bậc một cách chính tắc (Chương II, § 2, no. 9) (chú ý rằng nói chung trong phân bậc này sẽ có các phần tử thuần nhất $\neq 0$ có bậc âm). Ta sẽ ký hiệu bởi $A_{(p)}$ vành con của $S^{-1}A$ gồm các phần tử thuần nhất bậc 0, nói cách khác là tập các phân thức $x/s$, trong đó $x$ và $s$ là các phần tử thuần nhất cùng bậc trong $A$ và $s \notin p$. Tương tự, với mọi $A$-môđun phân bậc $M$, $S^{-1}M$ được phân bậc một cách chính tắc (*loc. cit.*) và ta sẽ ký hiệu bởi $M_{(p)}$ nhóm con các phần tử thuần nhất bậc 0, hiển nhiên là một $A_{(p)}$-môđun.

#### Mệnh đề 7 {#ac-iii-s1-prop-7 .statement}

*Cho $p$ là một iđêan nguyên tố phân bậc của $A$, $d$ là một số nguyên $\geq 1$ và $p'$ là iđêan nguyên tố phân bậc $p \cap A^{(d)}$ của $A^{(d)}$; với mọi $A$-môđun phân bậc $M$, đồng cấu $(M^{(d)})_{(p')} \to M_{(p)}$ dẫn xuất từ đơn ánh chính tắc $M^{(d)} \to M$ là song ánh.*

Nếu $S$ là tập hợp các phần tử thuần nhất của $A$ không thuộc $p$ và $S' = S \cap A^{(d)}$, thì đồng cấu chính tắc $\phi : {S'}^{-1}M^{(d)} \to S^{-1}M$ là một đồng cấu thuần nhất bậc 0 và nó đơn ánh, vì nếu $x \in M_{nd}$ thỏa mãn $sx = 0$ với $s \in A_n, s \notin p$, thì cũng có $s^dx = 0$ và $s^d \in A_{md}, s^d \notin p'$. Còn phải chứng minh rằng ảnh qua $\phi$ của $(M^{(d)})_{(p')}$ là toàn bộ $M_{(p)}$; nhưng nếu $x \in M_n, s \in A_n$ và $s \notin p$, thì cũng có $x/s = (xs^{d-1})/s^d$ với $xs^{d-1} \in A_{nd}, s^d \in A_n$ và $s^d \notin p'$, do đó có mệnh đề của chúng ta.

#### Mệnh đề 8 {#ac-iii-s1-prop-8 .statement}

*Cho $m = \bigoplus_{i \geq 1} A_i$; cho $(p^{(k)})_{1 \leq k \leq s}$ là một họ hữu hạn các iđêan nguyên tố phân bậc* của $A$ và một iđêan phân bậc $\mathfrak{a} \subset A$ sao cho $\mathfrak{a} \cap m \not\subset p^{(k)}$ với mọi $k$; khi đó tồn tại một phần tử thuần nhất $z \in \mathfrak{a} \cap m$ không thuộc bất kỳ $p^{(k)}$ nào.

Ta lập luận bằng quy nạp theo $n$, mệnh đề là tầm thường đối với $n = 1$. Nếu tồn tại một chỉ số $j$ sao cho $\mathfrak{a} \cap m \cap p^{(j)}$ được chứa trong một trong các $p^{(k)}$ có chỉ số $k \neq j$, thì từ giả thiết quy nạp suy ra rằng có một phần tử thuần nhất $z' \in \mathfrak{a} \cap m$ không thuộc bất kỳ $p^{(k)}$ nào với $k \neq j$ và do đó cũng không thuộc $p^{(j)}$, và phần tử này giải quyết bài toán. Vậy giả sử rằng với mọi chỉ số $j$, $\mathfrak{a} \cap m \cap p^{(j)}$ không được chứa trong bất kỳ $p^{(k)}$ nào có chỉ số $k \neq j$; do đó giả thiết quy nạp kéo theo sự tồn tại của một phần tử thuần nhất $y_j \in \mathfrak{a} \cap m \cap S_j$ không thuộc phần nào của các $S_j$ với $k \# j$; vì các $y_j$ đều có bậc $\geq 1$, ta có thể giả sử bằng cách thay thế chúng bằng các lũy thừa thích hợp (vì các $p^{(k)}$ là nguyên tố) rằng $y_1$ và $\prod_{j=2}^n y_j$ có cùng bậc. Khi đó $z = y_1 + \prod_{j=2}^n y_j$ là thuần nhất bậc $\geq 1$ và cùng một lập luận như trong Chương II, § 1, no. 1, Mệnh đề 2 cho thấy rằng $z$ giải quyết bài toán.

### Bài tập {#ac-iii-s1-exercises}

Xem các [bài tập cho § 1](exercises/s1/).
