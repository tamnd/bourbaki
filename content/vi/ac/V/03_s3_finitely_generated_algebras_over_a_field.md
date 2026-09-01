---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 3
section_title: Finitely generated algebras over a field
lang: vi
source: ac-i-vii
book_pages: 344-354, 370-373
pdf_pages: 0363-0373, 0389-0392
extraction: ocr
subsections:
    - "no": 1
      title: THE NORMALIZATION LEMMA
      page: 344
      pdf_page: 363
    - "no": 2
      title: THE INTEGRAL CLOSURE OF A FINITELY GENERATED ALGEBRA OVER A FIELD
      page: 348
      pdf_page: 367
    - "no": 3
      title: THE NULLSTELLENSATZ
      page: 349
      pdf_page: 368
    - "no": 4
      title: JACOBSON RINGS
      page: 351
      pdf_page: 370
statements: 17
exercises: 9
content_sha256: b1823c80c65157c4faf9c37cd1773ee8158b09f9415e35fcca609d7717edd3ac
translated_from: content/en/ac/V/03_s3_finitely_generated_algebras_over_a_field.md
source_content_sha256: badf2bc4cb748da842f275e255d9318b86b98b0069385cfdb864427619fa9e85
translation_model: gpt-5.4
translation_run: translate-vi-2b45e66a
glossary_version: 34
glossary_terms_sha256: c7a78462acf4483ec1b49b4f6ba900530daabe93a672f97265bccf3ef7a6f44d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC ĐẠI SỐ SINH HỮU HẠN TRÊN MỘT TRƯỜNG

### 1. BỔ ĐỀ CHUẨN HÓA

Trong số này và số tiếp theo, k ký hiệu một trường giao hoán.

#### Định lý 1 (Bổ đề chuẩn hóa) {#ac-v-s3-thm-1 .statement}

Cho A là một đại số trên k sinh hữu hạn và cho $a_1 \subset a_2 \subset \ldots \subset a_p$ là một dãy hữu hạn tăng các iđêan của A sao cho $p \geq 1$ và $a_p \neq A$. Tồn tại một dãy hữu hạn $(x_i)_{1 \leq i \leq n}$ các phần tử của A, độc lập đại số trên k (Chương III, § 1, no. 1), sao cho:
(a) A là nguyên trên vành $B = k[x_1, \ldots, x_n]$.
(b) Với mọi j sao cho $1 \leq j \leq p$, tồn tại một dãy tăng $(h(j))_{j \leq j \leq p}$ các số nguyên sao cho với mọi j, iđêan $a_j \cap B$ của B được sinh bởi $x_1, \ldots, x_{h(j)}$.

Trước hết chú ý rằng chỉ cần chứng minh định lý trong trường hợp A là một đại số đa thức $k[Y_1, \ldots, Y_m]$. Thật vậy, trong trường hợp tổng quát, A đẳng cấu với một thương của một đại số như thế A' bởi một iđêan $a'_0$; gọi $a'_j$ là ảnh ngược của $a_j$ trong A' và gọi $x'_i$ ($1 \leq i \leq r$) là các phần tử của A' thỏa mãn các điều kiện của mệnh đề đối với vành A' và dãy tăng các iđêan $a'_0 \subset a'_1 \subset \ldots \subset a'_p$. Khi đó các ảnh $x_i$ của các $x'_i$ trong A với $i > h(0)$ thỏa mãn các điều kiện cần có; điều này hiển nhiên đối với điều kiện (b), còn đối với điều kiện (a) thì điều này suy ra từ § 1, no. 1, Mệnh đề 2; sau cùng, nếu các $x_i(h(0) + 1 \leq i \leq r)$ không độc lập đại số trên k, thì sẽ tồn tại một đa thức khác không

$$
Q \in k[X_{h(0)+1}, \ldots, X_r]
$$

trong đó các $Q_j$ là các đa thức trong $k[Y_1, \ldots, Y_m]$; vì $a_p \neq 0$ là khả nghịch trong $k$, (4) chắc chắn là một phương trình phụ thuộc nguyên với các hệ số trong B, do đó có mệnh đề của chúng ta.

Trường phân thức $k(Y_1, \ldots, Y_r)$ của A vì thế là đại số trên trường phân thức $k(x_1, \ldots, x_m)$ của B, điều này chứng minh (Đại số, Chương V, § 5, no. 3, Định lý 4) rằng các $x_i$ ($1 \leq i \leq m$) là độc lập đại số. Hơn nữa, $a \cap B = Bx_1$; với mọi phần tử $z \in a, \cap B$ có thể viết $z = x_1 z'$ trong đó $z' \in A \cap k(x_1, \ldots, x_r)$; nhưng $A \cap k(x_1, \ldots, x_r) = k[x_1, \ldots, x_m] = B$ vì B đóng nguyên ($\S$ 1, no. 3, Hệ quả 2 của Mệnh đề 13); do đó $z' \in B$, điều này hoàn tất chứng minh các tính chất (a) và (b) trong trường hợp này.

(A2) **Trường hợp tổng quát ($p = 1$).**
Ta lập luận bằng quy nạp theo $m$, trường hợp $m = 0$ là tầm thường. Hiển nhiên ta có thể giả sử rằng $a_i \neq 0$ (nếu không thì ta có thể lấy $x_i = Y$, với $1 \leq i \leq m$ và $h(1) = 0$). Cho $x_1$ là một phần tử khác không của $a_i$; theo (A1) tồn tại $t_2, \ldots, t_m$ sao cho $x_1, t_2, \ldots, t$, độc lập đại số trên $k$, $A$ là nguyên trên $C = k[x_1, t_2, \ldots, t_m]$ và $x_1 A \cap C = x_1 C$. Theo giả thiết quy nạp tồn tại các phần tử $x_2, \ldots, x_m$ của $k[t_2, \ldots, t_m]$ và một số nguyên $h$ sao cho $k[t_2, \ldots, t_m]$ là nguyên trên $B' = k[x_2, \ldots, x_m]$, $x_2, \ldots, x_m$ độc lập đại số trên $k$ và iđêan $a_i \cap B'$ được sinh bởi $x_2, \ldots, x_h$. Khi đó $C$ là nguyên trên $B = k[x_1, x_2, \ldots, x_m]$ ($\S$ 1, no. 1, Hệ quả của Mệnh đề 5 ) và do đó $A$ cũng vậy ($\S$ 1, no. 1, Mệnh đề 6 ); cùng một lập luận như trong trường hợp (A1) cho thấy rằng $x_1, \ldots, x_m$ độc lập đại số trên $k$; sau cùng, vì $x_1 \in a_i$, và $B = B'[x_1], a_i \cap B = Bx, + (a_i \cap B')$ và, vì $a_i \cap B'$ được sinh (trong $B'$) bởi $x_2, \ldots, x_h, a_i \cap B$ được sinh (trong $B$) bởi $x_1, x_2, \ldots, x_h$.

(B) **Đoạn từ $p - 1$ trở lên.**
Cho $t_1, \ldots, t_r$, là các phần tử của $A$ thỏa mãn các điều kiện của định lý đối với dãy tăng các iđêan $a_1 \subset \ldots \subset a_{p-1}$ và đặt $r = h(p - 1)$. Theo (A2), tồn tại các phần tử $x_{r+1}, \ldots, x_s$ của $k[t_{r+1}, \ldots, t_m]$ và một số nguyên s sao cho
$$
C = k[t_{r+1}, \ldots, t_m]
$$
là nguyên trên $B' = k[x_{r+1}, \ldots, x_m]$, $x_{r+1}, \ldots, x_s$ độc lập đại số trên $k$ và iđêan $a_p \cap B'$ được sinh bởi $x_{r+1}, \ldots, x_s$. Viết $x_i = t_i$ với $i \leq r$ thì họ $(x_i)_{1 \leq i \leq m}$ thu được giải quyết bài toán với $h(p) = s$.
Vì $A$ là nguyên trên $C[t_1, \ldots, t_r] = C[x_1, \ldots, x_r]$ và do đó cũng nguyên trên $B = k[x_1, \ldots, x_m] = B'[x_1, \ldots, x_r]$ vì $C$ là nguyên trên $B'$ ($\S$ 1, no. 1, Hệ quả của Mệnh đề 5 và Mệnh đề 6); có thể chỉ ra như trong trường hợp (A1) rằng các $x_i$ độc lập đại số trên $k$. Mặt khác, với $j \leq p - 1$, iđêan
$$
a_j \cap k[x_1, \ldots, x_r, t_{r+1}, \ldots, t_m]
$$
theo giả thiết là tập hợp các đa thức theo $x_1, \ldots, x_r, t_{r+1}, \ldots, t_m$ mà mọi đơn thức của chúng đều chứa một trong các phần tử $x_1, \ldots, x_{h(j)}$; vì $x_{r+1}, \ldots, x_m$ là các đa thức theo $t_{r+1}, \ldots, t$, với các hệ số trong $k$, nên ngay lập tức thấy rằng một đa thức theo $x_1, \ldots, x_r, x_{r+1}, \ldots, x_s$ (với các hệ số trong $k$) chỉ có thể thuộc $a_j$ nếu mọi đơn thức của nó đều chứa một trong các phần tử $x_1, \ldots, x_{h(j)}$. Sau cùng, vì $x_1, \ldots, x_r$ thuộc $a_{p-1}$, và do đó cũng thuộc $a_p$, nên $a_p \cap B'[x_1, \ldots, x_r]$ gồm các đa thức theo $x_1, \ldots, x_r$ với hệ số trong $B'$ mà số hạng hằng thuộc $a_p \cap B'$; vậy iđêan này được sinh bởi $x_1, \ldots, x_r, x_{r+1}, \ldots, x_t$.

#### Hệ quả 1 {#ac-v-s3-thm-1-cor-1 .statement}

Cho $A$ là một miền nguyên và $B$ là một $A$-đại số sinh hữu hạn chứa $A$ như một vành con. Khi đó tồn tại một phần tử $s \neq 0$ của $A$ và một đại số con $B'$ của $B$ đẳng cấu với một đại số đa thức $A[Y_1, \ldots, Y_n]$ sao cho $B[s^{-1}]$ (Chương II, § 2, no. 1) là nguyên trên $B'[s^{-1}]$.

Ta viết $S = A - \{0\}$ và đặt $k = S^{-1}A$ là trường phân thức của $A$; rõ ràng $S^{-1}B$ là một đại số $k$ sinh hữu hạn và, vì nó chứa $k$ theo giả thiết (Chương II, § 2, no. 4, Định lý 1), nó không bị thu về 0. Do đó theo Định lý 1 (áp dụng với top = 1 và $a_i = 0$) tồn tại một dãy hữu hạn $(x_i)_{1 \leq i \leq n}$ các phần tử của $S^{-1}B$ độc lập đại số trên $k$ và sao cho $S^{-1}B$ là nguyên trên $k[x_1, \ldots, x_n]$. Gọi $(z_j)_{1 \leq j \leq m}$ là một hệ các phần tử sinh của $B$ như một $A$-đại số; trong $S^{-1}B$ mỗi $z_j/1$ thỏa mãn một phương trình phụ thuộc nguyên

$$
(z_j/1)^{a_j} + \sum_{h < a_j} P_{hj}(x_1, \ldots, x_n)(z_j/1)^h = 0
$$

trong đó các $P_{hj}$ là những đa thức theo các $x_i$ với hệ số trong $k$. Tồn tại một phần tử $s \neq 0$ của $A$ sao cho ta có thể viết $x_i = y_i/s$ sao cho, $\in B$ với $1 \leq i \leq n$ và mọi hệ số của các $P_{hj}$ đều có dạng $c/s$ trong đó $c \in A$; sau hết, bằng cách thay thế, nếu cần, $s$ bởi một tích các phần tử của $S$, ta có thể giả sử rằng trong $B$

$$
sz_j^{a_j} + \sum_{h < a_j} Q_{hj}z_j^h = 0
$$

trong đó các $Q_{hj}$ là những đa thức theo $y_1, \ldots, y_n$ với hệ số trong $A$; nếu ta viết $z'_j = sz_j$, thì thấy rằng, bằng cách nhân (6) với $s^{a_j-1}$, $z'_j$ là nguyên trên $B' = A[y_1, \ldots, y_n]$. Ta chứng minh rằng các $y_i$ độc lập đại số trên $A$; nếu có một quan hệ dạng $\sum_p a_p y_1^{p_1} \ldots y_n^{p_n} = 0$ trong đó $a_p \in A$ với mọi $p$, ta suy ra rằng $\sum_p a'_p x_1^{p_1} \ldots x_n^{p_n} = 0$ trong $S^{-1}B$, trong đó $a'_p = a_p s^{p_1 + \cdots + p_n}$ trong $k$; do giả thiết nên $a'_p = 0$ với mọi $p$, do đó $a_p = 0$ với mọi $p$. Hơn nữa, trong vành $B[s^{-1}]$ mỗi $z'_j/1$ là nguyên trên $B'[s^{-1}]$ (§ 1, no. 1, Mệnh đề 2) và, vì $z_j/1 = (z'_j/1)(1/s)$ trong $B[s^{-1}]$, nên thấy rằng các $z_j/1$ là nguyên trên $B'[s^{-1}]$, điều này hoàn tất chứng minh (§ 1, no. 1, Mệnh đề 4).

#### Hệ quả 2 {#ac-v-s3-thm-1-cor-2 .statement}

Cho $K$ là một trường, $A$ là một vành con của $K$ và $L$ là trường phân thức của $A$. Nếu $K$ là một $A$-đại số sinh hữu hạn, thì $[K:L]$ là hữu hạn và tồn tại $a \neq 0$ trong $A$ sao cho $L = A[a^{-1}]$.

Từ Hệ quả 1 suy ra rằng tồn tại các phần tử $x_1, \ldots, x_n$ của $K$ và một phần tử $a \neq 0$ của $A$ sao cho $x_1, \ldots, x_n$ độc lập đại số trên $A$ (và do đó trên L) và $K$ là nguyên trên vành con $A[x_1, \ldots, x_n, a^{-1}]$. Khi đó, theo §2, no.1, Bổ đề 2, $A[x_1, \ldots, x_n, a^{-1}]$ là một trường. Nhưng các phần tử khả nghịch duy nhất của một vành đa thức $C[Y_1, \ldots, Y_n]$ trên một miền nguyên C là các phần tử khả nghịch của C; áp dụng nhận xét này cho $C = A[a^{-1}]$, ta thấy tất yếu $n = 0$ và $A[a^{-1}]$ là một trường bằng L theo định nghĩa của trường này. Vì K là nguyên trên L và là một L-đại số sinh hữu hạn, nên bậc [K:L] là hữu hạn (§ 1, no. 1, Mệnh đề 4).

#### Hệ quả 3 {#ac-v-s3-thm-1-cor-3 .statement}

Cho A là một miền nguyên, B là một A-đại số sinh hữu hạn và b là một phần tử của B sao cho $zb^n \neq 0$ với mọi $z \neq 0$ trong A và mọi số nguyên $n > 0$. Gọi $\varphi : A \to B$ là đồng cấu chính tắc; tồn tại $a \neq 0$ trong A sao cho, với mọi đồng cấu f từ A vào một trường đóng đại số L thỏa mãn $f(a) \neq 0$, tồn tại một đồng cấu g từ B vào L sao cho $g(b) \neq 0$ và $f = g \circ \varphi$.

Giả thiết trên b kéo theo rằng, nếu h là đồng cấu chính tắc $x \mapsto x/1$ từ B vào $B[b^{-1}]$, thì đồng cấu $h \circ \varphi$ từ A vào $B[b^{-1}]$ là đơn ánh. Bởi Hệ quả 1, do đó tồn tại một phần tử $a \neq 0$ của A và một vành con $B'$ của $B[b^{-1}]$ sao cho $B[b^{-1}, a^{-1}]$ là nguyên trên $B'[a^{-1}]$ và $B'$ đẳng cấu với một đại số đa thức $A[Y_1, \ldots, Y_n]$. Cho f là một đồng cấu từ A vào một trường đóng đại số L sao cho $f(a) \neq 0$; tồn tại một đồng cấu từ $A[Y_1, \ldots, Y_n]$ vào L kéo dài f và do đó tồn tại một đồng cấu $f'$ từ $B'$ vào L kéo dài f. Vì $f'(a) \neq 0$ trong L, tồn tại một đồng cấu $f''$ từ $B'[a^{-1}]$ vào L sao cho

$$
f''(x/a^n) = f'(x) \cdot (f(a))^{-n}
$$

đối với mọi $x \in B'$ và mọi $n > 0$ (Chương II, §2, no. 1, Mệnh đề 1). Cuối cùng, vì $B[b^{-1}, a^{-1}]$ là nguyên trên $B'[a^{-1}]$, nên tồn tại một đồng cấu $f'''$ từ $B[b^{-1}, a^{-1}]$ đến L mở rộng $f''$ (§2, no. 1, Hệ quả 4 của Định lý 1). Nếu $j : x \mapsto x/1$ là đồng cấu chính tắc từ B đến $B[b^{-1}, a^{-1}]$, thì $g = f''' \circ j$ giải được bài toán vì $j(b)$ khả nghịch trong $B[b^{-1}, a^{-1}]$ và do đó $f'''(j(b)) \neq 0$ trong L.

Chú ý rằng, nếu trong Hệ quả 3, B được giả thiết là một miền nguyên và $A \subset B$, thì giả thiết trên b tương đương với $b \neq 0$.

### 2. BAO ĐÓNG NGUYÊN CỦA MỘT ĐẠI SỐ HỮU HẠN SINH TRÊN MỘT TRƯỜNG

#### Định lý 2 {#ac-v-s3-thm-2 .statement}

Cho A là một đại số nguyên trên k sinh hữu hạn, K trường phân thức của nó và $A'$ là bao đóng nguyên của A trong một trường K' là một mở rộng đại số hữu hạn của K. Khi đó $A'$ là một A-môđun hữu hạn sinh và một đại số trên k sinh hữu hạn.

Theo Định lý 1, tồn tại một đại số con C của A đẳng cấu với một đại số đa thức $k[X_1, \ldots, X_n]$ và sao cho A là nguyên trên C; $A'$ hiển nhiên là bao đóng nguyên của C trong K' (§ 1, no. 1, Mệnh đề 6); do đó ta có thể chỉ xét trường hợp $A = k[X_1, \ldots, X_n]$. Gọi $N$ là mở rộng quasi-Galois của $K$ (trong một bao đóng đại số của $K$) được sinh bởi $K'$, khi đó N là một mở rộng đại số hữu hạn của $K$ (Đại số, Chương V, § 6, no. 3, Hệ quả 1 của Mệnh đề 9). Chỉ cần chứng minh rằng bao đóng nguyên $B$ của $A$ trong $N$ là một $A$-môđun hữu hạn sinh, vì $A'$ là một A-môđun con của $B$ và $A$ là một vành Noether (Chương III, § 2, no. 10, Hệ quả 2 của Định lý 2). Do đó ta có thể chỉ xét trường hợp $K'$ là một mở rộng quasi-Galois của $K$. Khi đó ta biết (Đại số, Chương V, § 10, no. 9, Mệnh đề 14) rằng $K'$ là một mở rộng Galois (hữu hạn) của một mở rộng radicial (hữu hạn) $K''$ của $K$. Nếu $A''$ là bao đóng nguyên của $A$ trong $K''$, thì $A'$ là bao đóng nguyên của $A''$ trong $K'$, và chỉ cần chứng minh rằng $A''$ là một A-môđun hữu hạn sinh và $A'$ là một $A''$-môđun hữu hạn sinh. Bây giờ, nếu đã chứng minh được rằng $A''$ là một A-môđun hữu hạn sinh, thì nó là một miền Noether, nguyên đóng theo định nghĩa; việc $A$ là một $A''$-môđun hữu hạn sinh sẽ suy ra từ § 1, no. 6, Hệ quả 1 của Mệnh đề 18.

Do đó ta thấy rằng ta có thể chỉ cần xét trường hợp $A = k[X_1, \ldots, X_n]$ và $K'$ là một mở rộng thuần bất khả phân hữu hạn của $K = k(X_1, \ldots, X_r)$. Khi đó $K'$ được sinh bởi một họ hữu hạn các phần tử $(y_i)_{1 \leq i \leq m}$ và tồn tại một lũy thừa $q$ của số mũ của đặc số của $k$ sao cho $y_i^q \in k(X_1, \ldots, X_r)$. Gọi $c_j$ ($1 \leq j \leq r$) là các hệ số của tử số và mẫu số của các hàm hữu tỉ theo $X_1, \ldots, X_r$, bằng với $y_i^q$ ($1 \leq i \leq m$). Khi đó $K'$ được chứa trong mở rộng $L = k'(X_1^{q^{-1}}, \ldots, X_n^{q^{-1}})$, trong đó $k' = k(c_1^{q^{-1}}, \ldots, c_r^{q^{-1}})$ (ta đang ở trong một bao đóng đại số của $K'$) và $A$ được chứa trong bao đóng đại số $B'$ của $A$ trong $L'$. Bây giờ, $k'$ là đại số trên $k$ và do đó $C' = k'[X_1, \ldots, X_n]$ là nguyên trên $A$ ($§ 1$, no. 1, Proposition 5); vì $k'[X_1^{q^{-1}}, \ldots, X_n^{q^{-1}}]$ là nguyên đóng ($§ 1$, no. 3, Corollary 2 to Proposition 13), ta thấy rằng vành này là bao đóng nguyên của $C'$ trong $L'$ và do đó cũng là bao đóng nguyên của $A$ ($§ 1$, no. 1, Proposition 6), nói cách khác $B' = k'[X_1^{q^{-1}}, \ldots, X_n^{q^{-1}}]$. Rõ ràng $B'$ là một $C'$-môđun sinh hữu hạn ($§ 1$, no. 1, Proposition 4) và, vì $k'$ là một mở rộng hữu hạn của $k$, $C'$ là một $A$-môđun sinh hữu hạn và do đó $B'$ là một $A$-môđun sinh hữu hạn; vì $A$ là Noether và $A \subset B'$, $A'$ là một $A$-môđun sinh hữu hạn.

### 3. NULLSTELLENSATZ

#### Mệnh đề 1 {#ac-v-s3-prop-1 .statement}

Cho $A$ là một đại số sinh hữu hạn trên một trường $k$ và $L$ là bao đóng đại số của $k$.

(i) Nếu $A \neq \{0\}$, tồn tại một $k$-đồng cấu từ $A$ vào $L$.

(ii) Cho $f_1, f_2$ là hai đồng cấu $k$ từ $A$ vào $L$. Để $f_1$ và $f_2$ có cùng hạt nhân, điều kiện cần và đủ là tồn tại một tự đẳng cấu $k$ $s$ của $L$ sao cho $f_2 = s \circ f_1$.

(iii) Cho $a$ là một iđêan của $A$. Để $a$ là cực đại, điều kiện cần và đủ là nó là hạt nhân của một đồng cấu k từ $A$ vào $L$.

(iv) Để một phần tử $x$ của $A$ có tính chất $f(x) = 0$ đối với mọi đồng cấu k $f$ từ $A$ vào $L$, điều kiện cần và đủ là $x$ lũy linh.

Mệnh đề (i) suy ra từ no. 1, Hệ quả 3 của Định lý 1 áp dụng với việc thay thế $A$ bởi $k$, $B$ bởi $A$, $b$ bởi phần tử đơn vị của $B$ và $f$ bởi đơn ánh chính tắc của $k$ vào $L$.

Nếu $f$ là một đồng cấu k từ $A$ vào $L$ thì $f(A)$ là một vành con của $L$ chứa $k$; vì $L$ là một mở rộng đại số của $k$, $f(A)$ là một trường (Algebra, Chương V, § 3, no. 2, Mệnh đề 3) và, nếu $a$ là hạt nhân của f, $A/a$, đẳng cấu với $f(A)$, do đó là một trường, điều này chứng tỏ $a$ là cực đại. Ngược lại, nếu $a$ là một iđêan cực đại của $A$, thì từ (i) suy ra tồn tại một đồng cấu k từ $A/a$ vào $L$ và do đó một đồng cấu k của $A$ vào $L$ mà hạt nhân $b$ chứa $a$; nhưng vì $a$ là cực đại nên $b = a$; điều này chứng tỏ (iii).

Bây giờ chứng minh (ii). Nếu $s$ là một tự đẳng cấu trên k của $L$ sao cho $f_2 = s \circ f_1$, thì rõ ràng $f_1$ và $f_2$ có cùng hạt nhân. Ngược lại, giả sử rằng $f_1$ và $f_2$ có cùng hạt nhân; khi đó tồn tại một đẳng cấu trên k $s_0$ từ trường $f_1(A)$ lên trường $f_2(A)$ sao cho $f_2 = s_0 \circ f_1$; nhưng theo Algebra, Chương V, § 6, no. 3, Mệnh đề 7, $s_0$ mở rộng thành một tự đẳng cấu trên k của $L$ và do đó $f_2 = s \circ f_1$.

Cuối cùng, nếu $x \in A$ sao cho $x^n = 0$, thì với mọi đồng cấu trên k $f$ từ $A$ đến $L$, ta có $(f(x))^n = f(x^n) = 0$ và do đó $f(x) = 0$ vì $L$ là một trường. Ngược lại, giả sử rằng $x \in A$ không lũy linh; khi đó $A[x^{-1}]$ là một đại số trên $A$ sinh hữu hạn (và do đó là một đại số trên k sinh hữu hạn) không thu về 0 (Chương 11, § 2, no. 1, Nhận xét 3) và do đó tồn tại một đồng cấu trên k $g$ từ $A[x^{-1}]$ đến $L$ theo (i). Nếu $j : A \to A[x^{-1}]$ là đồng cấu chính tắc, thì $f = g \circ j$ là một đồng cấu trên k từ $A$ đến $L$ và $f(x)g(1/x) = g(x/1)g(1/x) = g(1) = 1$, do đó $f(x) \neq 0$.

Cho $k$ là một trường và $L$ là một trường mở rộng của $k$; một phần tử $x = (x_1, \ldots, x_n)$ của $L^n$ được gọi là một không điểm trong $L^n$ của một iđêan $c$ của vành đa thức $k[X_1, \ldots, X_n]$ nếu

$$
P(x) = P(x_1, \ldots, x_n) = 0
$$

với mọi $P \in r$.

#### Bổ đề 1 {#ac-v-s3-lem-1 .statement}

Cho $A$ là một đại số sinh hữu hạn trên một trường $k$, $(a_i)_{1 \leq i \leq n}$ là một hệ sinh của đại số này và $c$ là iđêan các quan hệ đại số giữa các $a_i$ với hệ số trong $k$ (Algebra, Chương IV, § 2, no. 1). Với mọi trường mở rộng $L$ của $k$, ánh xạ $f \mapsto (f(a_i))_{1 \leq i \leq n}$ là một song ánh từ tập hợp các đồng cấu trên k từ $A$ đến $L$ lên tập hợp các không điểm của $r$ trong $L^n$.

Tồn tại duy nhất một đồng cấu đại số trên k $h$ từ $k[X_1, \ldots, X_n]$ lên $A$ sao cho $h(X_i) = a_i$, với $1 \leq i \leq n$ và theo định nghĩa $r$ là hạt nhân của $h$. Ánh xạ f $\mapsto$ h là một song ánh từ tập các đồng cấu k từ $A$ vào $L$ lên tập các đồng cấu k từ $k[X_1, \ldots, X_n]$ vào $L$ mà bằng không trên c. Với mọi đa thức $P \in k[X_1, \ldots, X_n]$ và mọi phần tử $x = (x_1, \ldots, x_i) \in L^n$ ta viết $h_x(P) = P(x)$; khi đó ánh xạ $x \mapsto h_x$ là một song ánh từ $L^n$ lên tập các đồng cấu k từ $k[X_1, \ldots, X_n]$ vào $L$ (một đồng cấu như vậy được xác định bởi các giá trị của nó tại các $X_i$ ($1 \leq i \leq n$) ); nói rằng $h_x$ bằng không trên c có nghĩa là $x$ là một điểm không của c trong $L''$, do đó bổ đề được chứng minh.

Nếu áp dụng Mệnh đề 1 cho đại số $A = k[X_1, \ldots, X_n]/r$, trong đó c là một iđêan của $k[X_1, \ldots, X_n]$ phân biệt với toàn bộ vành, thì theo Bổ đề 1 ta thu được mệnh đề sau:

#### Mệnh đề 2 (Định lý không điểm của Hilbert) {#ac-v-s3-prop-2 .statement}

Cho k là một trường và L là một bao đóng đại số của k.

(i) Mọi iđêan $r \not\subset k[X_1, \ldots, X_n]$ không chứa 1 đều có ít nhất một điểm không trong $L^n$.

(ii) Cho $x = (x_1, \ldots, x_n), y = (y_1, \ldots, y_n)$ là hai phần tử của $L^n$; để tập các đa thức của $k[X_1, \ldots, X_n]$ bằng không tại x trùng với tập các đa thức của $k[X_1, \ldots, X_n]$ bằng không tại y, điều kiện cần và đủ là tồn tại một tự đẳng cấu k s của L sao cho $y_i = s(x_i)$ với $1 \leq i \leq n$.

(iii) Để một iđêan a của $k[X_1, \ldots, X_n]$ là cực đại, điều kiện cần và đủ là tồn tại một x trong $L^n$ sao cho a là tập các đa thức của $k[X_1, \ldots, X_n]$ bằng không tại x.

(iv) Để một đa thức Q của $k[X_1, \ldots, X_n]$ bằng không trên tập các điểm không trong $L''$ của một iđêan c của $k[X_1, \ldots, X_n]$, điều kiện cần và đủ là tồn tại một số nguyên m > 0 sao cho $Q^m \in c$.

### 4. CÁC VÀNH JACOBSON

#### Định nghĩa 1 {#ac-v-s3-def-1 .statement}

Một vành A được gọi là một vành Jacobson nếu mọi iđêan nguyên tố của A là giao của một họ các iđêan cực đại.

Ví dụ

(1) Mọi trường đều là một vành Jacobson.
(2) Vành $\mathbf{Z}$ là một vành Jacobson, iđêan nguyên tố duy nhất không cực đại là (0) là giao của các iđêan cực đại $(p)$ của $\mathbf{Z}$, trong đó $p$ chạy qua tập các số nguyên tố (xem Mệnh đề 4).
(3) Cho A là một vành Jacobson và cho a là một iđêan của A. Khi đó $A/a$ là một vành Jacobson, vì các iđêan của $A/a$ có dạng $b/a$, trong đó b là một iđêan của A chứa a, và $b/a$ là nguyên tố (tương ứng, cực đại) khi và chỉ khi b là như vậy.

#### Mệnh đề 3 {#ac-v-s3-prop-3 .statement}

Để một vành A là một vành Jacobson, điều kiện cần và đủ là, với mọi iđêan a của A, căn Jacobson của $A/a$ bằng căn nilpotent của nó (Chương II, § 2, no. 6).

Căn Jacobson (tương ứng, căn nil) của $A/a$ là giao của các iđêan cực đại (tương ứng, nguyên tố) của $A/a$ (*Đại số*, Chương VIII, § 6, no. 3, Định nghĩa 3 và *Đại số giao hoán*, Chương II, § 2, no. 6, Mệnh đề 13). Do đó điều kiện đã nêu có nghĩa là với mọi iđêan $a$ của $A$, giao của các iđêan nguyên tố chứa $a$ bằng giao của các iđêan cực đại chứa $a$. Điều kiện này hiển nhiên đúng với mọi iđêan $a$ của $A$ nếu $A$ là một vành Jacobson; ngược lại, nếu nó đúng với mọi iđêan nguyên tố của $A$, thì theo định nghĩa $A$ là một vành Jacobson.

#### Hệ quả {#ac-v-s3-n4-cor-1 .statement}

*Cho $A$ là một vành Jacobson; với mọi iđêan $a$ của $A$, căn của $a$ là giao của các iđêan cực đại của $A$ chứa $a$.*

Chỉ cần chú ý rằng $A/a$ là một vành Jacobson.

#### Mệnh đề 4 {#ac-v-s3-prop-4 .statement}

*Cho $A$ là một miền iđêan chính và $(\mathbf{p}_\lambda)_{\lambda \in L}$ là một hệ đại diện các phần tử cực biên của $A$ (*Đại số*, Chương VII, § 1, no. 3, Định nghĩa 2). Để $A$ là một vành Jacobson, điều kiện cần và đủ là $L$ vô hạn.*

Các iđêan cực đại của $A$ là các $A\mathbf{p}_\lambda$ (*loc. cit.*, no. 2, Mệnh đề 2). Nếu $L$ hữu hạn, giao của chúng là iđêan $Ax$, trong đó $x = \prod_{\lambda \in L} \mathbf{p}_\lambda$ (*ibid.*) và do đó khác $(0)$; mặt khác, nếu $L$ vô hạn, giao của các $A\mathbf{p}_\lambda$ là $(0)$$, mỗi phần tử $\neq 0$ của $A$ chỉ chia hết cho một số hữu hạn phần tử cực biên (*loc. cit.*, no. 3, Định lý 2). Khi đó mệnh đề suy ra từ sự kiện rằng $(0)$ là iđêan nguyên tố duy nhất không cực đại trong $A$ (*Đại số*, Chương VI, § 1, no. 13, Mệnh đề 14 (DIV)).

#### Mệnh đề 5 {#ac-v-s3-prop-5 .statement}

*Cho $A$ là một vành và $B$ là một $A$-đại số nguyên trên $A$. Nếu $A$ là một vành Jacobson thì $B$ cũng vậy.*

Thay thế $A$ bởi ảnh chính tắc của nó trong $B$, ta có thể giả sử rằng $A \subset B$. Cho $\mathfrak{p}'$ là một iđêan nguyên tố của $B$ và đặt $\mathfrak{p} = A \cap \mathfrak{p}'$. Theo giả thiết tồn tại một họ $(\mathfrak{m}_\lambda)_{\lambda \in L}$ các iđêan cực đại của $A$ mà giao của chúng bằng p. Với mọi $\lambda \in L$ tồn tại một iđêan cực đại $\mathfrak{m}'_\lambda$ của $B$ nằm trên $\mathfrak{m}_\lambda$ và chứa $\mathfrak{p}'$ (§ 2, no. 1, Mệnh đề 1 và Hệ quả 2 của Định lý 1). Nếu đặt $\mathfrak{q}' = \bigcap_{\lambda \in L} \mathfrak{m}'_\lambda$, thì $\mathfrak{q}' \cap A = \bigcap_{\lambda \in L} \mathfrak{m}_\lambda = \mathfrak{p}$ và $\mathfrak{q}' \supset \mathfrak{p}'$, do đó $\mathfrak{q}' = \mathfrak{p}'$ ($2$, no. 1, Hệ quả 1 của Mệnh đề 1).

#### Định lý 3 {#ac-v-s3-thm-3 .statement}

*Cho $A$ là một vành Jacobson, $B$ là một $A$-đại số sinh hữu hạn và $\varphi : A \to B$ là đồng cấu chính tắc. Khi đó:*
(i) *$B$ là một vành Jacobson.*
(ii) *Với mọi iđêan cực đại $m'$ của $B$, $m = \varphi^{-1}(m')$ là một iđêan cực đại của $A$ và $B/m'$ là một mở rộng đại số hữu hạn của $A/m$.*

Cho $\mathfrak{p}'$ là một iđêan nguyên tố của $B$ và $\mathfrak{p} = \varphi^{-1}(\mathfrak{p}')$. Cho $v$ là một phần tử $\neq 0$ của $B/\mathfrak{p}'$.

Vì $B/p'$ là một (Alp)-đại số nguyên sinh hữu hạn và đồng cấu chính tắc $\phi : A/p \to B/p'$ là đơn ánh, nên tồn tại một phần tử $u \neq 0$ của $A/p$ sao cho, với mọi đồng cấu $f$ từ $A/p$ vào một trường đóng đại số $L$ mà hạt nhân không chứa $u$, tồn tại một đồng cấu $g$ từ $B/p'$ vào $L$ mà hạt nhân không chứa $v$ và sao cho $f = g \circ \phi$ (no. 1, Hệ quả 3 của Định lý 1). Vì $A$ là một vành Jacobson, nên tồn tại một iđêan cực đại $m$ của $A$ chứa $p$ và sao cho $u \notin m/p$. Ta lấy $L$ là một bao đóng đại số của $A/m$ và $f$ là đồng cấu chính tắc $A/p \to L$; gọi

$$
g : B/p' \to L
$$

là một đồng cấu sao cho $f = g \circ \phi$ và $g(v) \neq 0$. Khi đó

$$
A/m \subset g(B/p') \subset L,
$$

do đó $g(B/p')$ là một trường con của $K$ (Đại số, Chương V, § 3, no. 2, Mệnh đề 3) và vì thế hạt nhân của $g$ là một iđêan cực đại của $B/p'$ không chứa $v$. Vậy ta thấy rằng giao của các iđêan cực đại của $B/p'$ thu về 0, điều này chứng minh rằng $B$ là một vành Jacobson. Hơn nữa, nếu $p'$ là cực đại, thì $g$ tất yếu là đơn ánh và do đó $p = m$ là cực đại; sau cùng $B/p'$ khi đó là một đại số sinh hữu hạn trên trường $A/m$ và vì thế là một mở rộng hữu hạn của $A/m$ (no. 1, Hệ quả 2 của Định lý 1).

#### Hệ quả 1 {#ac-v-s3-thm-3-cor-1 .statement}

*Mọi đại số sinh hữu hạn $A$ trên $\mathbf{Z}$ đều là một vành Jacobson; để một iđêan nguyên tố $p \subset A$ là cực đại, điều kiện cần và đủ là vành $A/p$ là hữu hạn.*

Nếu miền nguyên $A/p$ là hữu hạn, thì nó là một trường, vì, với mọi $u \neq 0$ trong $A/p$, ánh xạ $v \mapsto uv$ của $A/p$ vào chính nó là đơn ánh và do đó song ánh vì $A/p$ là hữu hạn. Ngược lại, với mọi iđêan cực đại $m$ của $A$, ảnh ngược của $m$ trong $A$ là một iđêan cực đại $(p)$ và $A/m$ là hữu hạn trên trường nguyên tố $\mathbf{Z}/(p) = \mathbf{F}_p$ theo Định lý 3.

#### Hệ quả 2 {#ac-v-s3-thm-3-cor-2 .statement}

*Cho $(P_\lambda)_{\lambda \in L}$ là một họ các đa thức trong $\mathbf{Z}[X_1, \ldots, X_n]$ và $Q$ là một đa thức trong $\mathbf{Z}[X_1, \ldots, X_n]$ sao cho, với mọi hệ các phần tử $(x_i)_{1 \leq i \leq n}$ thuộc một trường hữu hạn và thỏa mãn $P_\lambda(x_1, \ldots, x_n) = 0$ với mọi $\lambda$, thì cũng có $Q(x_1, \ldots, x_n) = 0$. Khi đó, nếu $a$ là iđêan của $\mathbf{Z}[X_1, \ldots, X_n]$ sinh bởi các $P_\lambda$, thì tồn tại một số nguyên $m > 0$ sao cho $Q^m \in a$. Hơn nữa, với mọi vành rút gọn $R$ và mọi hệ $(y_i)_{1 \leq i \leq n}$ các phần tử của $R$ sao cho $P_\lambda(y_1, \ldots, y_n) = 0$ với mọi $\lambda$, thì cũng có $Q(y_1, \ldots, y_n) = 0$.

Mệnh đề thứ hai suy ra từ mệnh đề thứ nhất vì iđêan của $\mathbf{Z}[X_1, \ldots, X_n]$ gồm các đa thức $P$ sao cho $P(y_1, \ldots, y_n) = 0$ chứa $a$. Để chứng minh mệnh đề thứ nhất, chỉ cần chú ý rằng, với mọi iđêan cực đại $m$ của $A = \mathbf{Z}[X_1, \ldots, X_n]$ chứa $a$, $A/m$ là một trường hữu hạn (Hệ quả 1) và giả thiết kéo theo rằng ảnh chính tắc của $Q$ trong $A/m$ bằng không; khi đó $Q$ thuộc giao của các iđêan cực đại của $A$ chứa $a$, giao này là căn của $a$ (Hệ quả của Mệnh đề 3).

#### Hệ quả 3 {#ac-v-s3-thm-3-cor-3 .statement}

*Cho $A$ là một vành Jacobson. Nếu tồn tại một $A$-đại số sinh hữu hạn $B$ chứa $A$ và là một trường, thì $A$ là một trường và $B$ là một mở rộng đại số của $A$.*

Chỉ cần áp dụng Định lý 3 (ii) với $m' = (0)$.

### Bài tập {#ac-v-s3-exercises}

với mọi iđêan nguyên tố $\mathfrak{p}$ của $A$ đều tồn tại một iđêan nguyên tố $\mathfrak{p}'$ của $A'$ nằm trên $\mathfrak{p}$. Lập luận bằng *phản chứng*: lấy $x \in A' \cap \mathfrak{g}A$ và đặt $a = A \cap (x^{-1}A)$, khi đó $a$ là một iđêan phân biệt với $A$. Gọi $\mathfrak{p}$ là một iđêan nguyên tố liên kết với $A/a$; khi đó iđêan thương $b = a : \mathfrak{p}$ phân biệt với $a$ (Chương IV, § 1, no. 4, Mệnh đề 9) và do đó tồn tại $y \in b$ sao cho $xy \notin A$ và
$$
xy \mathfrak{p} \subset \mathfrak{p}A' \cap A = \mathfrak{p};
$$
suy ra một mâu thuẫn.)

**93**

Xem [các bài tập của § 3](exercises/s3/).
