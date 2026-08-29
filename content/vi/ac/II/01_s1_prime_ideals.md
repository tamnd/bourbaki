---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 1
section_title: Prime ideals
lang: vi
source: ac-i-vii
book_pages: 51-55, 121-123
pdf_pages: 0071-0075, 0141-0143
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF PRIME IDEALS
      page: 51
      pdf_page: 71
    - "no": 2
      title: RELATIVELY PRIME IDEALS
      page: 53
      pdf_page: 73
statements: 9
exercises: 11
content_sha256: 870dc5a3798adb1453d440d2364ee590175ade40b80ceed2f603ca9546e8c942
translated_from: content/en/ac/II/01_s1_prime_ideals.md
source_content_sha256: 1b5bfd8804f03cc3ee0ccdadad5a967b6ee8842cca8b6471ecb23b5ec4046120
translation_model: gpt-5-6-mini
translation_run: translate-vi-70377c07
glossary_version: 34
glossary_terms_sha256: dc1afa28aec385d914c28eca6243ff65e26827f9b4aad7478dc28310411c1145
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. IĐÊAN NGUYÊN TỐ

### 1. ĐỊNH NGHĨA CỦA IĐÊAN NGUYÊN TỐ

#### Định nghĩa 1 {#ac-ii-s1-def-1 .statement}

Một iđêan $p$ của một vành $A$ được gọi là nguyên tố nếu vành $A/p$ là một miền nguyên.

Theo định nghĩa này, một iđêan $p$ của một vành $A$ là nguyên tố nếu hai điều kiện sau đây được thỏa mãn:
(1) $p \neq A$;
(2) nếu $x, y$ là hai phần tử của $A$ sao cho $x \notin p$ và $y \notin p$, thì $xy \notin p$.

Các điều kiện này cũng có thể được phát biểu bằng cách nói rằng tích của mọi họ hữu hạn các phần tử của $\mathfrak{g}p$ thuộc về $\mathfrak{g}p$, vì áp dụng điều kiện này cho tập rỗng cho ta $1 \notin p$.

Một iđêan cực đại $m$ của $A$ là nguyên tố vì $A/m$ là một trường; do đó suy ra từ định lý Krull (Đại số, Chương I, § 8, no. 7, Định lý 2) rằng mọi iđêan của

(*) Ngoại trừ các mệnh đề được đặt giữa hai dấu sao: \* ... *, các kết quả của chương này chỉ phụ thuộc vào các Quyển I đến VI và Chương I, §§ 1–3 của Quyển này.

A *khác với* $\mathbf{A}$ được chứa trong ít nhất một iđêan nguyên tố. Đặc biệt, để các iđêan nguyên tố tồn tại trong một vành $\mathbf{A}$, điều kiện cần và đủ là $\mathbf{A}$ không bị rút gọn về 0.

Cho $f : \mathbf{A} \to \mathbf{B}$ là một đồng cấu vành và $q$ là một iđêan của $\mathbf{B}$. Đặt $p = f^{-1}(q)$; đồng cấu $\overline{f} : \mathbf{A}/p \to \mathbf{B}/q$ dẫn xuất từ $f$ bằng cách lấy thương là đơn ánh. Giả sử $q$ là nguyên tố; vì vành $\mathbf{B}/q$ là một miền nguyên, nên $\mathbf{A}/p$ cũng vậy, do nó đẳng cấu với một vành con của $\mathbf{B}/q$; do đó iđêan $p = f^{-1}(q)$ là nguyên tố. Đặc biệt, giả sử $\mathbf{A}$ là một vành con của $\mathbf{B}$; với mọi iđêan $q$ của $\mathbf{B}$, $q \cap \mathbf{A}$ là một iđêan nguyên tố $\mathbf{A}$. Nếu $f$ là toàn ánh, $\overline{f}$ là một đẳng cấu; các điều kiện "p là nguyên tố" và "$q$ là nguyên tố" khi đó là tương đương. Do đó, nếu $p$ và $a$ là các iđêan của $\mathbf{A}$ sao cho $a \subset p$, một điều kiện cần và đủ để $p$ là nguyên tố là $p/a$ là nguyên tố trong $\mathbf{A}/a$.

#### Mệnh đề 1 {#ac-ii-s1-prop-1 .statement}

*Cho $\mathbf{A}$ là một vành, $a_1, a_2, \ldots, a_n$ là các iđêan của $\mathbf{A}$ và $p$ là một iđêan nguyên tố của $\mathbf{A}$. Nếu $p$ chứa tích $a_1 a_2 \ldots a_n$, thì nó chứa ít nhất một trong các $a_i$.*

Giả sử trên thực tế rằng $p$ không chứa một phần tử nào trong các $a_i$. Với $1 \leq i \leq n$, khi đó tồn tại một phần tử $s_i \in a_i \cap p$; khi đó $s = s_1 s_2 \ldots s_n$ được chứa trong $a_1 a_2 \ldots a_n$, và không được chứa trong $p$, điều này là vô lý.

#### Hệ quả {#ac-ii-s1-n1-cor-1 .statement}

*Cho $m$ là một iđêan cực đại của $\mathbf{A}$; với mọi số nguyên $n > 0$, iđêan nguyên tố duy nhất chứa $m^n$ là $m$.*

Một iđêan như vậy $p$ phải chứa $m$ theo Mệnh đề 1 được áp dụng cho $a_i = m$ với $1 \leq i \leq n$; vì $m$ là cực đại, $p = m$.

#### Mệnh đề 2 {#ac-ii-s1-prop-2 .statement}

*Cho $\mathbf{A}$ là một vành, $a$ là một tập hợp khác rỗng của $\mathbf{A}$ đóng đối với phép cộng và phép nhân và $(p_i)_{i \in I}$ là một họ hữu hạn khác rỗng các iđêan của $\mathbf{A}$. Giả sử rằng $a$ được chứa trong hợp của các $p_i$ và nhiều nhất hai trong các $p_i$ không nguyên tố. Khi đó $a$ được chứa trong một trong các $p_i$.*

Ta lập luận bằng quy nạp theo $n = \mathrm{Card}(I)$; mệnh đề là tầm thường nếu $n = 1$. Giả sử $n \geq 2$; nếu tồn tại một chỉ số $j$ sao cho $a \cap p_j \subset \bigcup_{i \neq j} p_i$, tập hợp $a$, là hợp của các $a \cap p_i$ với $i \in I$, được chứa trong $\bigcup_{i \neq j} p_i$ và do đó được chứa trong một trong các $p_i$ theo giả thiết quy nạp. Giả sử khi đó không tồn tại chỉ số như vậy; với mọi $j \in I$, lấy $y_j$ là một phần tử của $a \cap p_j$ không thuộc bất kỳ $p_i$ nào với $i \neq j$. Lấy $k$ là một phần tử của $I$ được chọn sao cho $p_k$ là nguyên tố nếu $n > 2$ và được chọn tùy ý nếu $n = 2$; đặt $z = y_k + \prod_{i \neq k} y_i$. Khi đó $z \in a$, vì $a$ đóng đối với phép cộng và phép nhân; nếu $j \neq k$, $\prod_{i \neq k} y_i$ thuộc $p_j$, nhưng $y_k \notin p_j$, do đó $z \notin p_j$. Mặt khác, $\prod_{i \neq k} y_i$ không thuộc $p_k$, vì không có thừa số nào $y_i \ (i \neq k)$ thuộc nó và $p_k$ là nguyên tố nếu $n - 1 > 1$; vì $y_k \in p_k$, $z$ không thuộc $p_k$ và mệnh đề được chứng minh.

### 2. CÁC IĐÊAN NGUYÊN TỐ CÙNG NHAU

Cho $A$ là một vành; hai iđêan $a, b$ của $A$ được gọi là *nguyên tố cùng nhau* nếu $a + b = A$. Để điều này đúng, điều kiện cần và đủ là $a + b$ không được chứa trong bất kỳ iđêan nguyên tố nào (*Algebra*, chương I, § 8, no. 7, định lý 2), nói cách khác, không có iđêan nguyên tố nào chứa cả $a$ và $b$. Hai iđêan cực đại phân biệt là nguyên tố cùng nhau.

Nếu $A$ là một *miền iđêan chính* (*Algebra*, chương VII, § 1), để hai phần tử $a, b$ của $A$ nguyên tố cùng nhau, điều kiện cần và đủ, theo đồng nhất thức Bezout (*loc. cit.*, no. 2, định lý 1), là các iđêan $Aa$ và $Ab$ nguyên tố cùng nhau.

#### Mệnh đề 3 {#ac-ii-s1-prop-3 .statement}

*Cho $a$ và $b$ là hai iđêan nguyên tố cùng nhau của một vành $A$. Cho $a'$ và $b'$ là hai iđêan của $A$ sao cho mọi phần tử của $a$ (resp. $b$) có một lũy thừa thuộc $a'$ (resp. $b'$). Khi đó $a'$ và $b'$ là nguyên tố cùng nhau.*

Theo giả thiết đã cho, mọi iđêan nguyên tố chứa $a'$ đều chứa $a$ và mọi iđêan nguyên tố chứa $b'$ đều chứa $b$. Nếu một iđêan nguyên tố chứa $a'$ và $b'$, thì nó chứa $a$ và $b$, điều này là vô lý, vì $a$ và $b$ nguyên tố cùng nhau; do đó $a'$ và $b'$ nguyên tố cùng nhau.

#### Mệnh đề 4 {#ac-ii-s1-prop-4 .statement}

*Cho $a, b_1, \ldots, b_n$ là các iđêan của một vành $A$. Nếu $a$ nguyên tố cùng nhau với mỗi $b_i$ ($1 \leq i \leq n$), thì nó nguyên tố cùng nhau với $b_1 b_2 \ldots b_n$.

Cho $p$ là một iđêan nguyên tố của $A$. Nếu $p$ chứa $a$ và $b_1 b_2 \ldots b_n$ thì nó chứa một trong các $b_i$ (no. 1, Mệnh đề 1), điều này là vô lý vì $a$ và $b_i$ nguyên tố cùng nhau.

#### Mệnh đề 5 {#ac-ii-s1-prop-5 .statement}

*Cho $(a_i)_{i \in I}$ là một họ hữu hạn khác rỗng các iđêan của một vành $A$. Các tính chất sau đây là tương đương =
(a) Với $i \neq j$, $a_i$ và $a_j$ nguyên tố cùng nhau.
(b) *Đồng cấu chính tắc* $\phi : A \to \prod_{i \neq I} (A/a_i)$ (*Đại số*, Chương 11, § 1, no. 7) là toàn ánh.
*Nếu các tính chất này được thỏa mãn, giao $a$ của các $a_i$ bằng tích của chúng và đồng cấu chính tắc* $\phi : A/a \to \prod_{i \in I} (A/a_i)$ (*Đại số*, Chương II, § 1, no. 7) là song ánh.*

Ta lập luận bằng quy nạp theo $n$, số các phần tử của $I$, trường hợp $n = 1$ là tầm thường. Trước hết xét trường hợp $n = 2$. Khi đó tính tương đương của (a) và (b) suy ra từ tính chính xác của dãy

$$
0 \longrightarrow A/(a_1 \cap a_2) \xrightarrow{\psi} (A/a_1) \oplus (A/a_2) \longrightarrow A/(a_1 + a_2) \longrightarrow 0
$$

(Đại số, Chương II, § 1, no. 7, công thức (30)). Hơn nữa, tồn tại $e_1 \in a$, và $e_2 \in a_2$ sao cho $1 = e_1 + e_2$; khi đó, với mọi $x \in a = a_1 \cap a_2$, $x = xe_1 + xe_2$; nhưng theo định nghĩa $xe_1 \in a_1 a_2$ và $xe_2 \in a_1 a_2$, do đó $x \in a_1 a_2$; do đó $a \subset a_1 a_2$ và bao hàm ngược lại là hiển nhiên.

Trong trường hợp tổng quát, giả sử điều kiện (a) được thỏa mãn và lấy $k$ là một phần tử của $I$ và $b_k = \bigcap_{i \neq k} a_i$; giả thiết quy nạp suy ra $b_k = \prod_{i \in I} a_i$, và theo Mệnh đề 4, $a$, và $b$, nguyên tố cùng nhau; khi đó

$$
a = \bigcap_{i \in I} a_i = a, \quad \cap b_k = a_k b_k = \prod_{i \in I} a_i,
$$

theo phần đầu của lập luận và cũng vì lý do đó, đồng cấu chính tắc $A/a \twoheadrightarrow (A/a_k) \times (A/b_k)$ là song ánh; theo giả thiết quy nạp, đồng cấu chính tắc $A/b_k \to \prod_{i \neq k} (A/a_i)$ là song ánh và do đó đồng cấu hợp

$$
A/a \to (A/a_k) \times (A/b_k) \to (A/a_k) \times \prod_{i \neq k} (A/a_i) = \prod_{i \in I} (A/a_i)
$$

which is precisely $\psi$; nghĩa là, (b) được thỏa mãn. Ngược lại, giả sử rằng (b) được thỏa mãn. Ta chứng minh rằng các $a_i$ tất yếu nguyên tố cùng nhau từng đôi một. Trong trường hợp ngược lại, tồn tại một iđêan $c \neq A$ chứa $a_i$ và $a_j$, với $i \neq j$. Ta đặt $a_h' = a_h$ với $h$ không bằng $i$ hoặc $j$ và $a_i' = a_j' = c$; đồng cấu chính tắc $\phi': A \to \prod_{i \in I} (A/a_i')$ có thể được viết thành ánh xạ hợp thành

$$
A \xrightarrow{\phi} \prod_{i \in I} (A/a_i) \xrightarrow{f} \prod_{i \in I} (A/a_i')
$$

trong đó $f$ là tích của các đồng cấu chính tắc $A/a_i \to A/a_i'$; rõ ràng $\phi'$ không toàn ánh, phép chiếu của $+(A)$ lên $(A/a_i') \times (A/a_i')$ là đường chéo của tích $(A/c) \times (A/c)$, khác với tích này vì $c \neq A$. Vì $f$ là toàn ánh, điều này chỉ ra rằng $\phi$ không toàn ánh.

#### Mệnh đề 6 {#ac-ii-s1-prop-6 .statement}

*Cho $(a_i)_{i \in I}$ là một họ hữu hạn không rỗng các iđêan của một vành $A$ nguyên tố cùng nhau từng đôi một; cho $a$ là giao của các $a_i$. Với mọi $A$-môđun $M$, ánh xạ chính tắc $M \to \prod_{i \in I} (M/a_i M)$ là toàn ánh và hạt nhân của nó là $aM$.*

Rõ ràng ánh xạ chính tắc của $M$ vào $\prod_{i \in I} (M/a_i M)$ bằng không trên $aM$; khi đó, bằng cách lấy các thương, nó xác định một đồng cấu $A : M/aM \to \prod_{i \in I} (M/a_i M)$. Mặt khác, theo Mệnh đề 5, đồng cấu chính tắc
$$
\psi : A/a \to \prod_{i \in I} (A/a_i)
$$
là song ánh. Khi đó $1_M \otimes \psi : M \otimes (A/a) \to M \otimes \prod_{i \in I} (A/a_i)$ cũng là song ánh. Bây giờ $M \otimes (A/a)$ được đồng nhất với $M/aM$ và $M \otimes \prod_{i \in I} (A/a_i)$ với $\prod_{i \in I} M \otimes (A/a_i)$, mà chính nó được đồng nhất với $\prod_{i \in I} (M/a_i M)$. Người ta kiểm tra ngay lập tức rằng các phép đồng nhất ở trên biến $1_M \otimes \psi$ thành $\lambda$, do đó có mệnh đề.

#### Ví dụ {#ac-ii-s1-n2-exa-1 .statement}

Cho $K$ là một trường, $a, (1 \leq i \leq m)$ là các phần tử phân biệt của $K$ và, với mỗi $i$, cho $g_i$ là một đa thức trong $K[X]$; iđêan chính $(X - a_i) = m_i$ là cực đại trong $K[X]$, do đó, với mọi hệ $(n_i)_{1 \leq i \leq m}$ gồm $m$ số nguyên $\geq 1$, các iđêan $m_i^{n_i}$ nguyên tố cùng nhau từng đôi một. Khi đó từ Mệnh đề 5 suy ra rằng tồn tại một đa thức $f \in K[X]$ sao cho $f(X) \equiv g_i(X) \pmod{(X - a_i)^{n_i}}$ với $1 \leq i \leq m$, hiệu của hai đa thức như vậy chia hết cho $\omega(X) = \prod_{i=1}^m (X - a_i)^{n_i}$. Nếu tất cả các $n_i$ được lấy bằng 1, ta thấy bài toán được giải tường minh bởi công thức nội suy của Lagrange (*Algebra*, Chương IV, § 2, no. 4).

### Bài tập {#ac-ii-s1-exercises}

Xem các [bài tập cho § 1](exercises/s1/).
