---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 1
section_title: Diagrams and exact sequences
lang: vi
source: ac-i-vii
book_pages: 1-9, 39-40
pdf_pages: 0021-0029, 0059-0060
extraction: ocr
subsections:
    - "no": 1
      title: DIAGRAMS
      page: 1
      pdf_page: 21
    - "no": 2
      title: COMMUTATIVE DIAGRAMS
      page: 2
      pdf_page: 22
    - "no": 3
      title: EXACT SEQUENCES
      page: 3
      pdf_page: 23
    - "no": 4
      title: THE SNAKE DIAGRAM
      page: 4
      pdf_page: 24
statements: 7
exercises: 7
content_sha256: 6fd48ebb7f8b38cf7171a07caff2a5ef71e9d335863bf0351db2b6aa189e9054
translated_from: content/en/ac/I/01_s1_diagrams_and_exact_sequences.md
source_content_sha256: 6790203cdd252786a633208363d3c57f4b6c7b2af0a1176438dd8ea954363ad2
translation_model: gpt-5.4-mini
translation_run: translate-vi-3b304503
glossary_version: 34
glossary_terms_sha256: d629aabd137e081a5a3bc47e97faa043696a878045415ef1b25323e63e3fbc55
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. BIỂU ĐỒ VÀ DÃY KHỚP

### 1. BIỂU ĐỒ

Chẳng hạn, cho $A, B, C, D, E$ là năm tập hợp và cho $f$ là một ánh xạ từ $A$ đến $B$, $g$ một ánh xạ từ $B$ đến $C$, $h$ một ánh xạ từ $D$ đến $E$, $u$ một ánh xạ từ $B$ đến $D$ và $v$ một ánh xạ từ $C$ đến $E$. Để tóm tắt một tình huống như vậy, ta thường dùng các biểu đồ; chẳng hạn, tình huống trên được tóm tắt bằng biểu đồ sau

(*) Ngoại trừ § 4, các kết quả của chương này chỉ phụ thuộc vào các Quyển I đến VI.

biểu đồ (Lý thuyết tập hợp, Chương II, § 3, no. 4)

$$
\begin{array}{ccc}
A & \xrightarrow{f} & B \\
& & \downarrow u \\
& & D \\
& & \downarrow v \\
& & E \\
& & \xrightarrow{h}
\end{array}
$$

(1)

Trong một biểu đồ như vậy, nhóm ký hiệu $A \xrightarrow{f} B$ biểu thị một cách sơ lược sự kiện rằng $f$ là một ánh xạ từ $A$ đến $B$. Khi không có sự mơ hồ nào về $f$, ta bỏ chữ $f$ và chỉ viết $A \to B$.

Khi $A, B, C, D, E$ là các nhóm (tương ứng các nhóm giao hoán) và $f, g, h, u, v$ là các đồng cấu nhóm, biểu đồ (1) được gọi, viết tắt, là một biểu đồ các nhóm (tương ứng các nhóm giao hoán).

Về nguyên tắc, một biểu đồ không phải là một đối tượng toán học, mà chỉ là một hình vẽ được thiết kế để làm dễ việc đọc một lập luận. Trong thực hành, các biểu đồ thường được dùng như những ký hiệu viết tắt để tránh phải nêu tên tất cả các tập hợp và các ánh xạ đang xét; do đó ta nói "Xét biểu đồ (1)" thay vì nói "Cho A, B, C, D, E là năm tập hợp ... và $v$ là một ánh xạ từ C đến E"; xem chẳng hạn phát biểu của Mệnh đề 2 ở no. 4.

### 2. BIỂU ĐỒ GIAO HOÁN

Xét, chẳng hạn, biểu đồ sau:

$$
\begin{array}{ccccccc}
A & \xrightarrow{f} & B & \xrightarrow{g} & C & \xrightarrow{h} & D \\
a \downarrow & & b \downarrow & & c \downarrow & & d \downarrow \\
A' & \xrightarrow{f'} & B' & \xrightarrow{g'} & C' & \xrightarrow{h'} & D'
\end{array}
$$

(2)

Với mỗi đường đi gồm một số đoạn nào đó của biểu đồ và đi theo chiều chỉ bởi các mũi tên, ta được một ánh xạ từ tập hợp được biểu diễn bởi đầu của đoạn thứ nhất tới tập hợp được biểu diễn bởi cuối của đoạn cuối cùng, cụ thể là hợp thành của các ánh xạ được biểu diễn bởi các đoạn khác nhau đã đi qua. Với mỗi đỉnh của biểu đồ, chẳng hạn $B$, theo quy ước có một đường đi thu gọn lại thành $B$, tương ứng với ánh xạ đồng nhất 1,

Trong (2), chẳng hạn có ba đường đi bắt đầu tại $A$ và kết thúc tại $C'$; các ánh xạ tương ứng là $c \circ g \circ f, g' \circ b \circ f$ và $g' \circ f' \circ a$. Một biểu đồ được gọi là giao hoán nếu, với mọi cặp đường đi trong biểu đồ có cùng điểm đầu và điểm cuối, hai ánh xạ tương ứng bằng nhau; đặc biệt nếu điểm đầu và điểm cuối của một đường đi trùng nhau thì ánh xạ tương ứng phải là ánh xạ đồng nhất.

Để biểu đồ (2) giao hoán thì cần và đủ rằng các hệ thức
$$
f' \circ a = b \circ f, \quad g' \circ b = c \circ g, \quad h' \circ f = d \circ h;
$$
đúng; nói cách khác, cần và đủ rằng ba biểu đồ hình vuông chứa trong (2) là giao hoán. Thật vậy, các hệ thức (3) suy ra $c \circ g \circ f = g' \circ b \circ f$ vì $c \circ g = g' \circ b$, và $g' \circ b \circ f = g' \circ f' \circ a$ vì $b \circ f = f' \circ a$; do đó ba đường đi bắt đầu tại $A$ và kết thúc tại $C'$ cho cùng một ánh xạ. Có thể kiểm tra tương tự rằng bốn đường đi bắt đầu tại $A$ và kết thúc tại $D'$ (tương ứng ba đường đi bắt đầu tại $B$ và kết thúc tại $D'$) cho cùng một ánh xạ. Các hệ thức (3) có nghĩa là hai đường đi bắt đầu tại $A$ (tương ứng $B, C$) và kết thúc tại $B'$ (tương ứng $C', D'$) cho cùng một ánh xạ. Không có cặp đỉnh nào khác của (2) có thể nối với nhau bởi nhiều hơn một đường đi và do đó biểu đồ (2) là giao hoán.

Trong phần sau, chúng tôi sẽ để cho bạn đọc tự kiểm tra các kết quả tương tự đối với những kiểu biểu đồ khác.

### 3. DÃY KHỚP

Nhắc lại định nghĩa sau (Đại số, Chương II, § 1, no. 4):

#### Định nghĩa 1 {#ac-i-s1-def-1 .statement}

Cho $A$ là một vành, $F, G, H$ là ba môđun phải (tương ứng trái) trên $A$, $f$ là một đồng cấu từ $F$ đến $G$ và $g$ là một đồng cấu từ $G$ đến $H$. Cặp có thứ tự $(f, g)$ được gọi là một dãy khớp nếu $\overline{g}^{-1}(0) = f(F)$, tức là nếu hạt nhân của $g$ bằng ảnh của $f$.

Biểu đồ
$$
\begin{array}{ccc}
F & \xrightarrow{f} & G \\
& & \xrightarrow{g} \\
& & H
\end{array}
$$
cũng được gọi là một dãy khớp.

Consider tương tự một biểu đồ gồm bốn môđun và ba đồng cấu:
$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$
Biểu đồ này được gọi là khớp tại $F$ nếu biểu đồ $E \xrightarrow{f} F \xrightarrow{g} G$ là một dãy khớp; nó được gọi là khớp tại $G$ nếu $F \xrightarrow{g} G \xrightarrow{h} H$ là một dãy khớp. Nếu (5) khớp tại $F$ và $G$, thì nó được gọi là khớp, hay cũng là một dãy khớp. Các dãy khớp với bất kỳ số hạng nào cũng được định nghĩa tương tự.

Nhắc lại các kết quả sau (loc. cit.), trong đó $E, F, G$ biểu thị các A-môđun phải (tương ứng trái), các mũi tên biểu thị các đồng cấu và $0$ biểu thị một môđun thu về phần tử đơn vị của nó:

(a) Nói rằng $0 \to E \xrightarrow{f} F$ là một dãy khớp thì tương đương với nói rằng $f$ là đơn ánh.

(b) Nói rằng $E \xrightarrow{f} F \to 0$ là một dãy khớp thì tương đương với nói rằng $f$ là toàn ánh.

(c) Nói rằng $0 \to E \xrightarrow{f} F \to 0$ là một dãy khớp thì tương đương với nói rằng $f$ là song ánh, tức là $f$ là một đẳng cấu từ $E$ lên $F$.

(d) Nếu $F$ là một môđun con của $E$ và $i$ ký hiệu đơn ánh chính tắc của $F$ vào $E$ và $p$ là toàn cấu chính tắc của $E$ lên $E/F$, thì biểu đồ
$$
\begin{array}{ccccccc}
0 & \longrightarrow & F & \xrightarrow{i} & E & \xrightarrow{p} & E/F \longrightarrow 0
\end{array}
$$
là một dãy khớp.

(e) Nếu $f: E \to F$ là một đồng cấu, thì biểu đồ
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & f^{-1}(0) & \xrightarrow{i} & E & \xrightarrow{f} & F & \xrightarrow{p} & F/f(E) \longrightarrow 0
\end{array}
$$
(trong đó $i$ là đơn ánh chính tắc của $f^{-1}(0)$ vào $E$ và $p$ là phép chiếu chính tắc của $F/f(E)$) là một dãy khớp.

(f) Để biểu đồ
$$
\begin{array}{ccccc}
E & \xrightarrow{f} & F & \xrightarrow{g} & G
\end{array}
$$
là một dãy khớp, điều kiện cần và đủ là tồn tại các môđun $S$, $T$ và các đồng cấu $a : E \to S$, $b : S \to F$, $c : F \to T$ và $d : T \to G$ sao cho $f = b \circ a$, $g = d \circ c$ và ba dãy
$$
\begin{array}{ccccccccc}
E & \xrightarrow{a} & S & \longrightarrow & 0 \\
0 & \longrightarrow & S & \xrightarrow{b} & F & \xrightarrow{c} & T & \longrightarrow & 0 \\
0 & \longrightarrow & T & \xrightarrow{d} & G
\end{array}
$$
khớp.

Sau cùng, nhắc rằng nếu $f: E \to F$ là một đồng cấu A-môđun, ta đặt $\operatorname{Ker}(f) = f^{-1}(0)$, $\operatorname{Im}(f) = f(E)$, $\operatorname{Coim}(f) = E/f^{-1}(0)$ và $\operatorname{Coker}(f) = F/f(E)$. Với ký hiệu này, trong (9), có thể lấy $S = \operatorname{Im}(f) = \operatorname{Ker}(g)$ và $T = \operatorname{Im}(g)$ (đẳng cấu chính tắc với $\operatorname{Coker}(f)$).

### 4. BIỂU ĐỒ RẮN

#### Mệnh đề 1 {#ac-i-s1-prop-1 .statement}

Xét một biểu đồ giao hoán của các nhóm giao hoán:
$$
\begin{array}{ccccc}
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \xrightarrow{u'} & B' & \xrightarrow{v'} & C'
\end{array}
$$

Giả sử hai hàng của (10) là khớp. Khi đó:

(i) Nếu $c$ là đơn ánh, ta có

(11) $\operatorname{Im}(b) \cap \operatorname{Im}(u') = \operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u).$

(ii) Nếu $a$ là toàn ánh, ta có

(12) $\operatorname{Ker}(b) + \operatorname{Im}(u) = \operatorname{Ker}(v' \circ b) = \operatorname{Ker}(c \circ v).$

Ta chứng minh (i). Rõ ràng

$$
\operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u) \subset \operatorname{Im}(b) \cap \operatorname{Im}(u').
$$

Ngược lại, lấy $x \in \operatorname{Im}(b) \cap \operatorname{Im}(u')$. Tồn tại $y \in B$ sao cho $x = b(y)$. Vì $v' \circ u' = 0$, ta có $0 = v'(x) = v'(b(y)) = c(v(y))$, do đó $v(y) = 0$ vì c là đơn ánh. Vì $(u, v)$ là một dãy khớp, tồn tại $z \in A$ sao cho $y = u(z)$, do đó $x = b(u(z))$.

Ta chứng minh (ii). Vì $v \circ u = 0$ và $v' \circ u' = 0$, hiển nhiên rằng

$$
\operatorname{Ker}(b) + \operatorname{Im}(u) \subset \operatorname{Ker}(v' \circ b) = \operatorname{Ker}(c \circ v).
$$

Ngược lại, lấy $x \in \operatorname{Ker}(v' \circ b)$. Khi đó $b(x) \in \operatorname{Ker}(v')$ và tồn tại $y' \in A'$ sao cho $u'(y') = b(x)$, vì dãy $(u', v')$ khớp. Vì a là toàn ánh, tồn tại $y \in A$ sao cho $a(y) = y'$, do đó $b(x) = u'(a(y)) = b(u(y))$; suy ra $x - u(y) \in \operatorname{Ker}(b)$, điều này hoàn tất chứng minh.

#### Bổ đề 1 {#ac-i-s1-lem-1 .statement}

Xét một biểu đồ giao hoán của các nhóm giao hoán:

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
a \downarrow & & b \downarrow \\
A' & \xrightarrow{u'} & B'
\end{array}
$$

Khi đó tồn tại một và chỉ một đồng cấu $u_1 : \operatorname{Ker}(a) \to \operatorname{Ker}(b)$ và một và chỉ một đồng cấu $u_2 : \operatorname{Coker}(a) \to \operatorname{Coker}(b)$ sao cho các biểu đồ

$$
\begin{array}{ccc}
\operatorname{Ker}(a) & \xrightarrow{u_1} & \operatorname{Ker}(b) \\
i \downarrow & & j \downarrow \\
A & & B
\end{array}
$$

và

$$
\begin{array}{ccc}
A' & \xrightarrow{u'} & B' \\
p \downarrow & & q \downarrow \\
\operatorname{Coker}(a) & \xrightarrow{u_2} & \operatorname{Coker}(b)
\end{array}
$$

là giao hoán, trong đó i và j ký hiệu các đơn ánh chính tắc và p và q là các toàn ánh chính tắc.

Nếu $x \in \mathrm{Ker}(a)$, thì $a(x) = 0$ và $b(u(x)) = u'(a(x)) = 0$, suy ra $u(x) \in \mathrm{Ker}(b)$, và sự tồn tại cũng như tính duy nhất của $u_1$ là ngay lập tức. Tương tự, ta có $u'(a(A)) = b(u(A)) \subset b(B)$, rồi bằng cách lấy thương $u'$ cho một đồng cấu $u_2 : \mathrm{Coker}(a) + \mathrm{Coker}(b)$, đó là đồng cấu duy nhất sao cho (15) là giao hoán.

Bây giờ ta xét biểu đồ *giao hoán* (10) của các nhóm giao hoán; theo Bổ đề 1, nó tương ứng với một biểu đồ

$$
\begin{array}{ccccccccc}
\mathrm{Ker}(a) & \xrightarrow{u_1} & \mathrm{Ker}(b) & \xrightarrow{v_1} & \mathrm{Ker}(c) \\
i \downarrow & & j \downarrow & & k \downarrow \\
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \longrightarrow & B' & \longrightarrow & C' \\
\vdots & & \vdots & & \vdots \\
\cdots \to \mathrm{Coker}(a) & \xrightarrow{u_2} & \mathrm{Coker}(b) & \xrightarrow{v_2} & \mathrm{Coker}(c)
\end{array}
$$

trong đó $i, j, k$ là các đơn ánh chính tắc, $p, q, r$ là các toàn ánh chính tắc và $u_1, u_2$ (tương ứng $v_1, v_2$) là các đồng cấu chính tắc gắn với $u, u'$ (tương ứng $v, u'$) theo Bổ đề 1. Kiểm tra ngay rằng biểu đồ này giao hoán.

#### Mệnh đề 2 {#ac-i-s1-prop-2 .statement}

*Giả sử rằng trong biểu đồ giao hoán (10) các dãy $(u, v)$ và $(u', u')$ khớp. Khi đó:*

(i) $v_1 \circ u_1 = 0$; nếu $u'$ là đơn ánh, thì dãy $(u_1, v_1)$ khớp.
(ii) $v_2 \circ u_2 = 0$; nếu $v$ là toàn ánh, thì dãy $(u_2, v_2)$ khớp.
(iii) *Giả sử rằng $u'$ là đơn ánh và $v$ là toàn ánh. Khi đó tồn tại một và chỉ một đồng cấu $d : \mathrm{Ker}(c) \to \mathrm{Coker}(a)$ với tính chất sau: nếu $x \in \mathrm{Ker}(c)$, $y \in B$ và $t' \in A'$ thỏa mãn các quan hệ $v(y) = k(x)$ và $u'(t') = b(y)$, thì $d(x) = p(t')$. Hơn nữa dãy*

(*) $$
\begin{array}{cccccc}
\mathrm{Ker}(a) & \xrightarrow{u_1} & \mathrm{Ker}(b) & \xrightarrow{v_1} & \mathrm{Ker}(c) & \xrightarrow{d} \\
& & & & & \\
& & & & & \\
& & & & & \\
\mathrm{Coker}(a) & \xrightarrow{u_2} & \mathrm{Coker}(b) & \xrightarrow{v_2} & \mathrm{Coker}(c)
\end{array}
$$

là khớp.

Chứng minh (i). Vì $u_1$ và $v_1$ có cùng đồ thị với các phép hạn chế của $u$ và $v$ lên $\mathrm{Ker}(a)$ và $\mathrm{Ker}(b)$ tương ứng, ta có $v_1 \circ u_1 = 0$. Khi đó
$$
\mathrm{Ker}(v_1) = \mathrm{Ker}(b) \cap \mathrm{Ker}(v) = \mathrm{Ker}(b) \cap \mathrm{Im}(u) = \mathrm{Im}(j) \cap \mathrm{Im}(u).
$$
Nhưng, theo Mệnh đề 1, (i), $\mathrm{Ker}(v_1) = \mathrm{Im}(j \circ u_1) = \mathrm{Im}(u_1)$ nếu $u'$ đơn ánh.

Chứng minh (ii). Vì $u_2$ và $v_2$ thu được từ $u$ và $v$ bằng cách lấy thương, rõ ràng là $v_2 \circ u_2 = 0$. Giả sử $v$ toàn ánh; vì $q$ và $p$ toàn ánh, suy ra từ các giả thiết và Mệnh đề 1, (ii) rằng
$$
\begin{align*}
\mathrm{Ker}(v_2) &= q(\mathrm{Ker}(v_2 \circ q)) = q(\mathrm{Ker}(v') + \mathrm{Im}(b)) = q(\mathrm{Ker}(v')) = q(\mathrm{Im}(u')) \\
&= \mathrm{Im}(q \circ u') = \mathrm{Im}(u_2 \circ p) = \mathrm{Im}(u_2).
\end{align*}
$$

Sau cùng ta hãy chứng minh (iii). Với $x \in \mathrm{Ker}(c)$, tồn tại $y \in B$ sao cho $v(y) = k(x)$ vì $v$ toàn ánh; hơn nữa $v'(b(y)) = c(k(x)) = 0$ và do đó tồn tại một phần tử *duy nhất* $t' \in A'$ sao cho $u'(t') = b(y)$, vì $u'$ đơn ánh. Bây giờ ta chỉ ra rằng phần tử $p(t') \in \mathrm{Coker}(a)$ là *độc lập* với phần tử $y \in B$ sao cho $v(y) = k(x)$. Thật vậy, nếu $y' \in B$ là một phần tử khác sao cho $v(y') = k(x)$, thì $y' = y + u(z)$, với $z \in A$; ta chỉ ra rằng nếu $t'' \in A'$ sao cho $u'(t'') = b(y')$ thì $t'' = t' + a(z)$; vì
$$
u'(t' + a(z)) = u'(t') + u'(a(z)) = b(y) + b(u(z)) = b(y + u(z)) = b(y').
$$
Sau cùng, suy ra rằng $p(t'') = p(t') + p(a(z)) = p(t')$. Khi đó có thể đặt $d(x) = p(t')$ và ánh xạ $d : \mathrm{Ker}(c) \to \mathrm{Coker}(a)$ như vậy đã được định nghĩa.

Nếu bây giờ $x_1, x_2$ là các phần tử của $\mathrm{Ker}(c)$ và $x = x_1 + x_2$, ta lấy các phần tử $y_1, y_2$ của $B$ sao cho $v(y_1) = k(x_1)$ và $v(y_2) = k(x_2)$ và chọn cho $y \in B$ phần tử $y_1 + y_2$; khi đó ngay lập tức $d(x) = d(x_1) + d(x_2)$ và do đó $d$ là một *đồng cấu*.

==========

Giả sử rằng $x = v_1(x')$ với một $x' \in \mathrm{Ker}(b)$; khi đó lấy $y \in B$ là phần tử $j(x')$. Vì $b(j(x')) = 0$, suy ra $d(x) = 0$, do đó $d \circ v_1 = 0$. Ngược lại, giả sử rằng $d(x) = 0$. Trong ký hiệu trên ta có $t' = a(s)$, với $s \in A$. Trong trường hợp này ta có $b(y) = u'(t') = u'(a(s)) = b(u(s))$, hay $b(y - u(s)) = 0$. Do đó phần tử $y - u(s)$ có dạng $j(n)$, với $n \in \mathrm{Ker}(b)$, và ta có $k(x) = v(y) = v(u(s) + j(n)) = v(j(n)) = k(v_1(n))$; vì $k$ là đơn ánh, $x = v_1(n)$, điều này chứng tỏ rằng dãy (*) khớp tại $\mathrm{Ker}(c)$.

Cuối cùng, ta có (luôn luôn trong cùng ký hiệu)
$$
u_2(d(x)) = u_2(p(t')) = q(u'(t')) = q(b(y)) = 0
$$
và do đó $u_2 \circ d = 0$. Ngược lại, giả sử rằng một phần tử $w = p(t')$ của $\mathrm{Coker}(a)$ thỏa mãn $u_2(w) = u_2(p(t')) = 0$ (trong đó $t' \in A$). Khi đó $q(u'(t')) = 0$ và do đó $u'(t') = b(y)$ với một $y \in B$; vì $v'(u'(t')) = 0$, ta có $v'(b(y)) = 0$, suy ra $c(v(y)) = 0$, nói cách khác $v(y) = k(x)$ với một $x \in \mathrm{Ker}(c)$, và theo định nghĩa $w = d(x)$, điều này cho thấy rằng dãy (*) khớp tại

Coker(a). Đã thấy trong (i) rằng nó khớp tại Ker(b) và trong (ii) rằng nó khớp tại Coker(b), điều đó hoàn tất chứng minh của (iii).

#### Nhận xét {#ac-i-s1-n4-rem-1 .statement}

Nếu các nhóm của biểu đồ (10) đều là, chẳng hạn, các môđun phải trên một vành $\mathbf{A}$ và các đồng cấu là các đồng cấu A-môđun, thì dễ dàng kiểm tra rằng đồng cấu d được định nghĩa trong Mệnh đề 2, (iii) cũng là một đồng cấu A-môđun: nếu $x \in \mathrm{Ker}(c)$ và $a \in \Lambda$, và $y \in B$ sao cho $v(y) = k(x)$, thì chỉ cần lưu ý rằng $v(ya) = k(xa)$.

#### Hệ quả 1 {#ac-i-s1-prop-2-cor-1 .statement}

Giả sử rằng biểu đồ (10) giao hoán và hai hàng đều khớp. Khi đó:

(i) Nếu $u'$, a và c đơn ánh, thì b đơn ánh.
(ii) Nếu v, a và c toàn ánh, thì b toàn ánh.

Mệnh đề (i) là hệ quả của mệnh đề (i) của Mệnh đề 2: vì $\mathrm{Ker}(a) = 0$ và $\mathrm{Ker}(c) = 0$, do đó $\mathrm{Ker}(b) = 0$.

Mệnh đề (ii) là hệ quả của mệnh đề (ii) của Mệnh đề 2: vì $\mathrm{Coker}(a) = 0$ và $\mathrm{Coker}(c) = 0$, do đó $\mathrm{Coker}(b) = 0$.

#### Hệ quả 2 {#ac-i-s1-prop-2-cor-2 .statement}

Giả sử rằng biểu đồ (10) giao hoán và hai hàng đều khớp. Trong các điều kiện này:

(i) Nếu b đơn ánh và nếu a và v toàn ánh, thì c đơn ánh.
(ii) Nếu b toàn ánh và nếu c và $u'$ đơn ánh, thì a toàn ánh.

Để chứng minh (i) xét biểu đồ

$$
\begin{array}{ccccc}
u(A) & \xrightarrow{w} & B & \xrightarrow{v} & C \\
a' \downarrow & & b \downarrow & & c \downarrow \\
u'(A') & \xrightarrow{w'} & B' & \xrightarrow{v'} & C'
\end{array}
$$

trong đó $a'$ là ánh xạ có cùng đồ thị như hạn chế của b trên $u(A)$ và w và $w'$ là các đơn ánh chính tắc; rõ ràng biểu đồ này giao hoán và các hàng của nó khớp. Hơn nữa $w'$ là đơn ánh và theo giả thiết v là toàn ánh; khi đó theo Mệnh đề 2, (iii) ta có một dãy khớp

$$
0 = \mathrm{Ker}(b) \longrightarrow \mathrm{Ker}(c) \xrightarrow{d} \mathrm{Coker}(a') = 0
$$

vì b đơn ánh và $a'$ toàn ánh; suy ra $\mathrm{Ker}(c) = 0$.

Để chứng minh (ii) xét biểu đồ

$$
\begin{array}{ccccc}
A & \xrightarrow{u} & B & \xrightarrow{w} & v(B) \\
a' \downarrow & & b \downarrow & & c' \downarrow \\
A' & \xrightarrow{w'} & B' & \xrightarrow{\sigma'} & v'(B')
\end{array}
$$

trong đó lần này $c'$ là ánh xạ có cùng đồ thị như hạn chế của c trên v(B) và w và $w'$ lần lượt có cùng đồ thị như v và v'; biểu đồ này giao hoán và các hàng của nó khớp. Hơn nữa w là toàn ánh và theo giả thiết $u'$ là đơn ánh; khi đó theo Mệnh đề 2, (iii) ta có một dãy khớp

$$
0 = \operatorname{Ker}(c') \xrightarrow{d} \operatorname{Coker}(a) \longrightarrow \operatorname{Coker}(b) = 0
$$

vì b toàn ánh và c' đơn ánh; suy ra Coker (a) = 0.

### Bài tập {#ac-i-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).

==========
