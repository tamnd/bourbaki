---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 4
section_title: Nilpotent Lie algebras
lang: vi
source: lie-i-iii
pdf_pages: 0056-0060, 0109-0116
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF NILPOTENT LIE ALGEBRAS
      page: 0
      pdf_page: 56
    - "no": 2
      title: ENGEL'S THEOREM
      page: 0
      pdf_page: 57
    - "no": 3
      title: THE LARGEST NILPOTENCY IDEAL OF A REPRESENTATION
      page: 0
      pdf_page: 58
    - "no": 4
      title: THE LARGEST NILPOTENT IDEAL OF A LIE ALGEBRA
      page: 0
      pdf_page: 60
    - "no": 5
      title: EXTENSION OF THE BASE FIELD
      page: 0
      pdf_page: 60
statements: 18
exercises: 27
content_sha256: 7815680b8318036c3ec4a4c8ac843d327461e829f8cd8f36969f5036eecb902f
translated_from: content/en/lie/I/04_s4_nilpotent_lie_algebras.md
source_content_sha256: 48ab9b1787343e1f86d71a8b0614a97c02bf7d85a80b47fd455f6abb64aa840b
translation_model: gpt-5.4
translation_run: translate-vi-c10151d9
glossary_version: 34
glossary_terms_sha256: da79895154eb47a1bf4236050c40c9f03be60dad60c7a0d00cd97c3619968c8a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. ĐẠI SỐ LIE LŨY LINH

*Nhắc lại rằng từ nay về sau $K$ kí hiệu một trường giao hoán. Trong phần còn lại của chương, các đại số Lie được giả thiết là hữu hạn chiều trên $K$.*

### 1. ĐỊNH NGHĨA ĐẠI SỐ LIE LŨY LINH

#### Định nghĩa 1 {#lie-i-s4-def-1 .statement}

*Một đại số Lie $g$ được gọi là lũy linh nếu tồn tại một dãy hữu hạn giảm các iđêan $(g_i)_{1 \leq i \leq p}$ của $g$ với $g_0 = g, g_p = \{0\}$, sao cho* $[g, g_i] \subset g_{i+1}$ *với* $0 \leq i < p$.

Một đại số Lie giao hoán là lũy linh.

#### Mệnh đề 1 {#lie-i-s4-prop-1 .statement}

*Cho $g$ là một đại số Lie. Các điều kiện sau là tương đương:*
(a) $g$ *là lũy linh;*
(b) $\mathcal{C}^k g = \{0\}$ *với* $k$ *đủ lớn*;
(c) $\mathcal{C}_k g = g$ *với* $k$ *đủ lớn*;
(d) *tồn tại một số nguyên* $k$ *sao cho* $\operatorname{ad} x_1 \circ \operatorname{ad} x_2 \circ \cdots \circ \operatorname{ad} x_k = 0$ *với mọi phần tử* $x_1, x_2, \ldots, x_k$ *của* $g$;
(e) *tồn tại một dãy giảm các iđêan* $(g_i)_{0 \leq i \leq n}$ *của* $g$ *với* $g_0 = g, g_n = \{0\}$, *sao cho* $[g, g_i] \subset g_{i+1}$ *và* $\dim g_i / g_{i+1} = 1$ *với* $0 \leq i < n$.

Nếu $\mathcal{C}^k g = \{0\}$ (resp. $\mathcal{C}_k g = g$), rõ ràng dãy $\mathcal{C}^1 g, \ldots, \mathcal{C}^k g$ (resp. $\mathcal{C}_k g, \mathcal{C}_{k-1} g, \ldots, \mathcal{C}_0 g$) có các tính chất của Định nghĩa 1 và do đó $g$ là lũy linh. Ngược lại, giả sử rằng tồn tại một dãy $(g_i)_{0 \leq i \leq p}$ có các tính chất của Định nghĩa 1. Ta thấy bằng quy nạp theo $n$ rằng $g_i \supset \mathcal{C}^{i+1} g$ và $g_{p-i} \subset \mathcal{C}_i g$. Do đó $\mathcal{C}^{p+1} g = \{0\}$ và $\mathcal{C}_p g = g$. Như vậy ta đã chứng minh rằng các điều kiện (a), (b) và (c) là tương đương. Mặt khác, $\mathcal{C}^1 g$ là tập hợp các tổ hợp tuyến tính của các phần tử có dạng

$$
[x_1, [x_2, \ldots, [x_{i-2}, [x_{i-1}, x_i]] \ldots]]
$$

trong đó $x_1, x_2, \ldots, x_i$ chạy qua $g$. Do đó các điều kiện (b) và (d) là tương đương. Cuối cùng, nếu tồn tại một dãy $(g_i)_{0 \leq i \leq p}$ các iđêan có các tính chất của

Định nghĩa 1, thì tồn tại một dãy giảm $(\mathfrak{h}_i)_{0 \leq i \leq n}$ các không gian con vectơ của $g$ có số chiều $n, n-1, n-2, \ldots, 0$ và một dãy chỉ số
$$
i_0 < i_1 < \cdots < i_p
$$
với $g_0 = \mathfrak{h}_{i_0}, g_1 = \mathfrak{h}_{i_1}, \ldots, g_p = \mathfrak{h}_{i_p}$; khi đó, vì $[g, \mathfrak{h}_{i_k}] \subset \mathfrak{h}_{i_{k+1}}$ nên các $\mathfrak{h}_i$ là các iđêan và $[g, \mathfrak{h}_i] \subset \mathfrak{h}_{i+1}$ với mọi $i$. Do đó các điều kiện (a) và (e) là tương đương.

#### Hệ quả 1 {#lie-i-s4-prop-1-cor-1 .statement}

*Tâm của một đại số Lie lũy linh khác không là khác không.*

#### Hệ quả 2 {#lie-i-s4-prop-1-cor-2 .statement}

*Dạng Killing của một đại số Lie lũy linh là không.*
Với mọi $x$ và $y$ trong một đại số Lie lũy linh, $\operatorname{ad} x \circ \operatorname{ad} y$ là lũy linh và do đó có vết bằng không.

#### Mệnh đề 2 {#lie-i-s4-prop-2 .statement}

*Các đại số con, các đại số thương và các mở rộng trung tâm của một đại số Lie lũy linh đều là lũy linh. Một tích hữu hạn các đại số Lie lũy linh là một đại số Lie lũy linh.*
Cho $g$ là một đại số Lie, $g'$ là một đại số con của $g$, $\mathfrak{h}$ là một iđêan của $g$, $\mathfrak{k} = g/\mathfrak{h}$ và $\phi$ là ánh xạ chính tắc từ $g$ lên $\mathfrak{k}$. Nếu $g$ là lũy linh, thì $\mathcal{C}^k g = \{0\}$ với một số nguyên $k$, do đó $\mathcal{C}^k g' \subset \mathcal{C}^k g = \{0\}$ và $\mathcal{C}^k \mathfrak{k} = \phi(\mathcal{C}^k g) = \{0\}$, và vì thế $g'$ và $\mathfrak{k}$ đều lũy linh. Nếu $\mathfrak{k}$ lũy linh và $\mathfrak{h}$ được chứa trong tâm của $g$, thì $\mathcal{C}^k \mathfrak{k} = \{0\}$ với một số nguyên $k$, do đó $\mathcal{C}^k g \subset \mathfrak{h}$ và vì vậy $\mathcal{C}^{k+1} g \subset [\mathfrak{h}, g] = \{0\}$, nên $g$ là lũy linh. Sau cùng, mệnh đề liên quan đến các tích suy ra chẳng hạn từ mệnh đề (a) $\Leftrightarrow$ (d) của Mệnh đề 1.

Định nghĩa 1 và Mệnh đề 2 cho thấy rằng các đại số Lie lũy linh chính xác là các đại số thu được từ các đại số Lie giao hoán bằng một dãy các mở rộng trung tâm.

#### Mệnh đề 3 {#lie-i-s4-prop-3 .statement}

*Cho $g$ là một đại số Lie lũy linh và $\mathfrak{h}$ là một đại số con của $g$ phân biệt với $g$. Chuẩn hóa tử của $\mathfrak{h}$ trong $g$ phân biệt với $\mathfrak{h}$.*
Cho $k$ là số nguyên lớn nhất sao cho $\mathcal{C}^k g + \mathfrak{h} \neq \mathfrak{h}$. Khi đó
$$
[\mathcal{C}^k g + \mathfrak{h}, \mathfrak{h}] \subset \mathcal{C}^{k+1} g + \mathfrak{h} \subset \mathfrak{h}
$$
và do đó chuẩn hóa tử của $\mathfrak{h}$ trong $g$ chứa $\mathcal{C}^k g + \mathfrak{h}$.

### 2. ĐỊNH LÝ ENGEL

#### Bổ đề 1 {#lie-i-s4-lem-1 .statement}

*Cho $V$ là một không gian vectơ trên $\mathbf{K}$. Nếu $x$ là một tự đồng cấu lũy linh của $V$, thì ánh xạ $y \mapsto [x, y]$ của $\mathcal{L}(V)$ vào $\mathcal{L}(V)$ là lũy linh.*
Nếu $f$ ký hiệu ánh xạ này, thì $f^m(y)$ là một tổng các hạng tử có dạng $\pm x^i y x^j$ với $i + j = m$. Nếu $x^k = 0$, thì $f^{2k-1}(y) = 0$ với mọi $y$.

#### Định lý 1 (Engel) {#lie-i-s4-thm-1 .statement}

*Cho $V$ là một không gian vectơ trên $\mathbf{K}$ và $g$ là một đại số con hữu hạn chiều của $\mathfrak{gl}(V)$ mà các phần tử của nó là các nội cấu lũy linh của $V$. Nếu $V \neq \{0\}$, tồn tại $u \neq 0$ trong $V$ sao cho $x.u = 0$ với mọi $x \in g$.*

Chứng minh được tiến hành bằng quy nạp theo chiều $n$ của $g$. Định lý là hiển nhiên nếu $n = 0$. Giả sử nó đúng đối với các đại số có chiều $< n$.

Cho $h$ là một đại số Lie con của $g$ có chiều $m < n$. Nếu $x \in h$, thì $\mathrm{ad}_g x$ biến $h$ vào chính nó và khi chuyển qua thương xác định một tự đồng cấu $\sigma(x)$ của không gian $g/h$. Theo Bổ đề 1, $\mathrm{ad}_g x$ là lũy linh và do đó $\sigma(x)$ là lũy linh. Theo giả thiết quy nạp, tồn tại một phần tử khác không của $g/h$ bị mọi $\sigma(x),\ x \in h$, triệt tiêu. Suy ra $h$ là một iđêan trong một đại số con nào đó có số chiều $(m+1)$ của $g$.

Ta kết luận (bằng cách lặp bắt đầu từ $h = \{0\}$) rằng $g$ có một iđêan $h$ chiều $n-1$. Lấy $a \in g,\ a \notin h$. Ta lại dùng giả thiết quy nạp: các $u \in V$ sao cho $x.u = 0$ với mọi $x \in h$ tạo thành một không gian con vectơ khác không U của V. Không gian con này ổn định dưới tác dụng của $a$ (§ 3, no. 5, Mệnh đề 5). Vì $a$ là một tự đồng cấu lũy linh của V, tồn tại một phần tử khác không của U bị triệt tiêu bởi $a$ và do đó bởi mọi phần tử của $g$.

#### Hệ quả 1 {#lie-i-s4-thm-1-cor-1 .statement}

*Để một đại số Lie g là lũy linh, điều kiện cần và đủ là, với mọi $x \in g$, $\mathrm{ad}\ x$ là lũy linh.*

Điều kiện này là cần thiết (Mệnh đề 1). Giả sử rằng tính đủ của nó đã được chứng minh đối với các đại số Lie chiều $< n$ ($n \neq 0$). Cho $g$ là một đại số Lie $n$-chiều sao cho, với mọi $x \in g$, $\mathrm{ad}\ x$ là lũy linh. Định lý 1, áp dụng cho tập hợp các $\mathrm{ad}\ x\ (x \in g)$, chứng minh rằng tâm $c$ của $g$ là khác không. Khi đó $g$ là một mở rộng trung tâm của đại số Lie $g/c$, đại số này là lũy linh theo giả thiết quy nạp của chúng ta. Chứng minh được hoàn tất bằng cách áp dụng Mệnh đề 2.

#### Hệ quả 2 {#lie-i-s4-thm-1-cor-2 .statement}

*Cho g là một đại số Lie và h là một iđêan của g. Giả sử rằng $g/h$ là lũy linh và rằng, với mọi $x \in g$, hạn chế của $\mathrm{ad}\ x$ trên h là lũy linh. Khi đó g là lũy linh.*

Cho $x \in g$. Vì $g/h$ là lũy linh, tồn tại một số nguyên $k$ sao cho $(\mathrm{ad}\ x)^k(g) \subset h$. Theo giả thiết tồn tại một số nguyên $k'$ sao cho $(\mathrm{ad}\ x)^{k'}(h) = \{0\}$. Do đó $(\mathrm{ad}\ x)^{k+k'}(g) = \{0\}$. Vậy Hệ quả 2 là một hệ quả của Hệ quả 1.

#### Hệ quả 3 {#lie-i-s4-thm-1-cor-3 .statement}

*Cho V là một không gian vectơ và g là một đại số con hữu hạn chiều của $\mathfrak{gl}(V)$ mà các phần tử của nó là những nội đồng cấu lũy linh của V. Khi đó g là một đại số Lie lũy linh.*

Điều này suy ra ngay lập tức từ Bổ đề 1 và Hệ quả 1.

#### Ví dụ {#lie-i-s4-n2-exa-1 .statement}

Đại số $\mathfrak{n}(n, K)$ (§ 1, no. 2, Ví dụ 2 (3)) là lũy linh.

### 3. IĐÊAN LŨY LINH LỚN NHẤT CỦA MỘT BIỂU DIỄN

#### Bổ đề 2 {#lie-i-s4-lem-2 .statement}

*Cho g là một đại số Lie, a là một iđêan của g và M là một g-môđun đơn. Nếu, với mọi $x \in a,\ x_M$ là lũy linh, thì $x_M = 0$ với mọi $x \in a$.*

Cho N là không gian con của M gồm các $m \in M$ sao cho $x_M.m = 0$ với mọi $x \in a$. Theo Định lý 1, $N \neq \{0\}$. Mặt khác, với mọi $y \in g$, N ổn định dưới $y_M$ (§ 3, no. 5, Mệnh đề 5). Do đó $N = M$, điều này chứng minh bổ đề.

#### Bổ đề 3 {#lie-i-s4-lem-3 .statement}

*Cho g là một đại số Lie, a là một iđêan của g, M là một g-môđun có số chiều hữu hạn trên*

K và $(M_i)_{0 \leq i \leq n}$ là một chuỗi Jordan-Hölder của $g$-môđun $M$. Các điều kiện sau là tương đương:

(a) với mọi $x \in a$, $x_M$ là lũy linh;
(b) với mọi $x \in a$, $x_M$ thuộc căn Jacobson của đại số kết hợp $A$ sinh bởi 1 và các $y_M$ với $y \in g$;
(c) với mọi $x \in a$,
$$
x_M(M_0) \subset M_1, x_M(M_1) \subset M_2, \ldots, x_M(M_{n-1}) \subset M_n.
$$

Nếu các điều kiện này được thỏa mãn, $a$ trực giao với $g$ đối với dạng song tuyến tính liên kết với $g$-môđun $M$.

(b) $\Rightarrow$ (a): vì $A$ là hữu hạn chiều trên $K$, căn Jacobson của $A$ là một iđêan lũy linh (*Đại số*, Chương VIII, § 6, no. 4, Định lý 3) và do đó mọi phần tử của căn này đều lũy linh.

(a) $\Rightarrow$ (c): mỗi $Q_i = M_i/M_{i+1}$ ($0 \leq i < n$) là một $g$-môđun đơn. Với mọi $x \in a$, tự đồng cấu $x_{Q_i}$ (được dẫn xuất từ $x_M$ bằng cách hạn chế vào $M_i$ và chuyển qua thương) là lũy linh nếu điều kiện (a) được thỏa mãn và do đó bằng không theo Bổ đề 2; nói cách khác, $x_M(M_i) \subset M_{i+1}$.

(c) $\Rightarrow$ (b): giả sử điều kiện (c) được thỏa mãn; lấy $x \in a$ và $z \in A$. Khi đó $z(M_i) \subset M_i$ ($0 \leq i < n$) và do đó $(zx_M)^n(M) = \{0\}$; vì thế $Ax_M$ là một iđêan trái lũy linh của $A$ và do đó được chứa trong căn Jacobson của $A$ (*Đại số*, Chương VIII, § 6, no. 3, Hệ quả 3 của Định lý 1).

Cuối cùng, giả sử các điều kiện (a), (b) và (c) được thỏa mãn. Lấy $x \in a$ và $y \in g$. Ta vừa thấy rằng $y_M x_M$ là lũy linh và do đó $\operatorname{Tr}(y_M x_M) = 0$, điều này chứng minh khẳng định cuối cùng của bổ đề.

#### Mệnh đề 4 {#lie-i-s4-prop-4 .statement}

Cho $g$ là một đại số Lie, $M$ là một $g$-môđun có số chiều hữu hạn trên $K$ và $A$ là đại số kết hợp được sinh bởi 1 và tập hợp các $x_M$ ($x \in g$).

(a) Các iđêan $a$ của $g$ sao cho $x_M$ là lũy linh với mọi $x \in a$ đều được chứa trong một iđêan trong số đó, $n$.

(b) Iđêan $n$ là tập hợp các $x \in g$ sao cho $x_M$ thuộc căn Jacobson của $A$.

(c) Cho $(M_i)_{0 \leq i \leq n}$ là một chuỗi Jordan-Hölder của $g$-môđun $M$; khi đó $n$ cũng là tập hợp các $x \in g$ sao cho $(x)_{M_i/M_{i+1}} = 0$ với mọi $i$.

(d) $n$ trực giao với $g$ đối với dạng song tuyến tính liên kết với $\varphi$.

Tập hợp các $x \in g$ sao cho $x_M$ thuộc căn Jacobson của $A$ hiển nhiên là một iđêan của $g$. Khi đó mệnh đề suy ra ngay lập tức từ Bổ đề 3.

#### Định nghĩa 2 {#lie-i-s4-def-2 .statement}

Iđêan $n$ của Mệnh đề 4 được gọi là iđêan lũy linh lớn nhất đối với $g$-môđun $M$ hoặc iđêan lũy linh lớn nhất của biểu diễn tương ứng.

Rõ ràng $n$ chứa hạt nhân của biểu diễn này. Nó bằng hạt nhân ấy khi $M$ là nửa đơn (Mệnh đề 4 (c)), nhưng nói chung thì không. Cần chú ý rằng một phần tử $x$ của $g$ sao cho $x_M$ là lũy linh không nhất thiết thuộc $n$.

Ta cũng chú ý rằng một trường hợp riêng của Bổ đề 3 ngay lập tức cho kết quả sau:

#### Mệnh đề 5 {#lie-i-s4-prop-5 .statement}

Cho $V$ là một không gian vectơ có số chiều hữu hạn $n$ trên $K$ và $g$ là một đại số Lie con của $gl(V)$ mà các phần tử của nó là những nội cấu lũy linh của $V$. Khi đó tồn tại một dãy giảm các không gian vectơ con $V_0, V_1, \ldots, V_n$ của $V$, có các chiều $n, n-1, \ldots, 0$, sao cho $x(V_i) \subset V_{i+1}$ với mọi $x \in g$ và $i = 0, 1, \ldots, n-1$.

### 4. IĐÊAN LŨY LINH LỚN NHẤT CỦA MỘT ĐẠI SỐ LIE

Cho $g$ là một đại số Lie và $a$ là một iđêan của $g$. Để $a$ là lũy linh, điều kiện cần và đủ là, với mọi $x \in a$, $\operatorname{ad}_g x$ là lũy linh; điều kiện này hiển nhiên là đủ và là cần, vì nếu $a$ là lũy linh và $x \in a$, thì $\operatorname{ad}_a x$ là lũy linh và $\operatorname{ad}_g x$ ánh xạ $g$ vào $a$, do đó $\operatorname{ad}_g x$ là lũy linh. Khi đó Mệnh đề 4 áp dụng cho biểu diễn kề của $g$ cho kết quả sau:

#### Mệnh đề 6 {#lie-i-s4-prop-6 .statement}

Cho $g$ là một đại số Lie và $E$ là đại số con kết hợp của $\mathcal{L}(g)$ được sinh bởi 1 và các $\operatorname{ad}_g x$ ($x \in g$). Gọi $R$ là căn Jacobson của $E$.
(a) Tập hợp $n$ gồm các $y \in g$ sao cho $\operatorname{ad}_g y \in R$ là iđêan lũy linh lớn nhất của $g$.
(b) Nó trực giao với $g$ đối với dạng Killing.

Cần lưu ý rằng $g/n$ có thể có các iđêan lũy linh khác không.

### 5. MỞ RỘNG TRƯỜNG CƠ SỞ

Cho $g$ là một đại số Lie trên $K$, $K_1$ là một mở rộng của $K$ và $g' = g_{(K_1)}$. Vì $\mathcal{C}^k g' = (\mathcal{C}^k g)_{(K_1)}$, $g$ là lũy linh nếu và chỉ nếu $g'$ là lũy linh.

Cho $M$ là một $g$-môđun có số chiều hữu hạn trên $K$, $n$ là iđêan lũy linh lớn nhất đối với $M$ và $M' = M_{(K_1)}$. Cho $(M_i)_{0 \leq i \leq n}$ là một chuỗi Jordan-Hölder của $g$-môđun $M$. Khi đó $x_M(M_i) \subset M_{i+1}$ với mọi $i$ và mọi $x \in n$, do đó

$$
x'_{M'}((M_i)_{(K_1)}) \subset (M_{i+1})_{(K_1)}
$$

với mọi $i$ và mọi $x' \in n_{(K_1)}$; do đó $x'_{M'}$ là lũy linh với $x' \in n_{(K_1)}$ nên $n_{(K_1)}$ được chứa trong iđêan lũy linh lớn nhất $n'$ của $M'$. Bây giờ ta sẽ thấy rằng, *nếu $K_1$ tách được trên $K$, thì $n' = n_{(K_1)}$*. Gọi $E$ là $K$-đại số kết hợp sinh bởi 1 và các $x_M$ ($x \in g$), $E'$ là $K$-đại số kết hợp sinh bởi 1 và các $x_{M'}$ ($x' \in g'$), còn $R$ và $R'$ là các căn Jacobson của $E$ và $E'$. Đại số $E'$ được đồng nhất một cách chính tắc với $E_{(K_1)}$. Khi đó $R' = R_{(K_1)}$ (*Đại số*, Chương VIII, § 7, no. 2, Hệ quả 2 (c) của Mệnh đề 3). Bây giờ lấy $y' \in n'$ và viết

$$
y' = \sum_{i=1}^n \lambda_i y_i,
$$

trong đó các $y_i$ thuộc $g$ và các $\lambda_i \in K_1$ độc lập tuyến tính trên $K$. Khi đó $y'_{M'} = \sum_{i=1}^n \lambda_i (y_i)_{M'}$ và $y'_{M'} \in R' = R_{(K_1)}$. Suy ra $(y_i)_M \in R$ và do đó $y_i \in n$ với mọi $i$. Kéo theo $y' \in n_{(K_1)}$, do đó $n' \subset n_{(K_1)}$.

Đặc biệt, nếu $K_1$ tách được trên $K$, thì iđêan lũy linh lớn nhất của $g_{(K_1)}$ được dẫn xuất từ iđêan đó của $g$ bằng cách mở rộng trường cơ sở từ $K$ đến $K_1$.

### Bài tập {#lie-i-s4-exercises}

Các quy ước của § 4 vẫn có hiệu lực trừ khi có nói khác.

Xem [các bài tập của § 4](exercises/s4/).
