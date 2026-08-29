---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 1
section_title: Krull domains
lang: vi
source: ac-i-vii
book_pages: 475-493, 545-555
pdf_pages: 0493-0511, 0563-0573
extraction: ocr
subsections:
    - "no": 1
      title: DMSORIAL IDEALS OF AN INTEGRAL DOMAIN
      page: 475
      pdf_page: 493
    - "no": 2
      title: THE MONOID STRUCTURE ON D(A)
      page: 478
      pdf_page: 496
    - "no": 3
      title: KRULL DOMAINS
      page: 480
      pdf_page: 498
    - "no": 4
      title: ESSENTIAL VALUATIONS OF A KRULL DOMAIN
      page: 482
      pdf_page: 500
    - "no": 5
      title: APPROXIMATION FOR ESSENTIAL VALUATIONS
      page: 484
      pdf_page: 502
    - "no": 6
      title: PRIME IDEALS OF HEIGHT 1 IN A KRULL DOMAIN
      page: 485
      pdf_page: 503
    - "no": 7
      title: 'APPLICATION: NEW CHARACTERIZATIONS OF DISCRETE VALUATION RINGS'
      page: 487
      pdf_page: 505
    - "no": 8
      title: THE INTEGRAL CLOSURE OF A KRULL DOMAIN IN A FINITE EXTENSION OF ITS FIELD OF FRACTIONS
      page: 487
      pdf_page: 505
    - "no": 9
      title: POLYNOMIAL RINGS OVER A KRULL DOMAIN
      page: 488
      pdf_page: 506
    - "no": 10
      title: DIVISOR CLASSES IN KRULL DOMAINS
      page: 489
      pdf_page: 507
statements: 41
exercises: 32
content_sha256: 1e14e67718807d0948922e5233e9366c7029cc0b6fd6e335cb7d997840112ba6
translated_from: content/en/ac/VII/01_s1_krull_domains.md
source_content_sha256: 9bef6d28f362c12836cf4563473a98aa78f886c75e3bc526c03329214a3be918
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-c35f3b28
glossary_version: 34
glossary_terms_sha256: f1e546aaac359d9f99cb7412ca9171980a20decd9856913e587865b58bffb2ab
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. CÁC MIỀN KRULL

### 1. CÁC IĐÊAN PHÂN THỨC CỦA MỘT MIỀN NGUYÊN

#### Định nghĩa 1 {#ac-vii-s1-def-1 .statement}

Cho $A$ là một miền nguyên và $K$ là trường các phân thức của nó. Mọi A-môđun con $a$ của $K$ sao cho tồn tại một phần tử $d \neq 0$ trong $A$ mà $da \subset A$ được gọi là một iđêan phân thức $\mathfrak{d}$ của $A$ (hoặc của $K$, do lạm dụng ngôn ngữ).

Mọi A-môđun con sinh hữu hạn $a$ của $K$ đều là một iđêan phân thức: thật vậy, nếu $(a_i)_{1 \leq i \leq n}$ là một hệ sinh của $a$, ta có thể viết $a_i = b_i/d_i$, trong đó $b_i \in A$, $d_i \in A$ và $d, \neq 0$; nếu $d = d_1 \ldots d_n$, rõ ràng $da \subset A$. Đặc biệt, các A-môđun con đơn sinh của $K$ là các iđêan phân thức (nhắc lại rằng chúng đã được gọi là các iđêan chính phân thức trong Đại số, Chương VI, § 1, no. 5). Nếu $A$ là Noether, mọi iđêan phân thức là một A-môđun sinh hữu hạn. Mọi A-môđun con của một iđêan phân thức của $A$ là một iđêan phân thức. Mọi iđêan của $A$ là một iđêan phân thức; để tránh nhầm lẫn, các iđêan này cũng được gọi là các iđêan nguyên của $A$.

Ta ký hiệu bởi $I(A)$ tập hợp các iđêan phân thức khác không của $A$. Cho hai phần tử $a, b$ của $I(A)$, ta sẽ viết $a \prec b$ (hoặc $b \succ a$) cho quan hệ "mọi iđêan chính phân thức chứa $a$ cũng chứa $b$"; rõ ràng quan hệ này là một tiền thứ tự trên $I(A)$. Gọi $R$ là quan hệ tương đương liên kết "$a \prec b$ và $b \prec a$" (Lý thuyết tập hợp, Chương III, § 1, no. 2) và $D(A)$ là tập thương $I(A)/R$; ta sẽ nói rằng các phần tử của $D(A)$ là các ước của $A$ và, với mọi iđêan phân thức $a \in I(A)$, ta sẽ ký hiệu bởi $\operatorname{div} a$ (hoặc $\operatorname{div}, a$) ảnh chính tắc của $a$ trong $D(A)$ và ta sẽ nói rằng $\operatorname{div} a$ là ước $\mathfrak{d}$ của $a$; nếu $a = Ax$ là một iđêan chính phân thức, ta viết div(x) thay cho div(Ax) và div(x) được gọi là ước của x; các phần tử của D(A) có dạng div(x) được gọi là các ước chính. Bằng cách lấy thương, tiền thứ tự $\prec$ trên I(A) xác định trên D(A) một thứ tự mà ta sẽ ký hiệu bởi $\leqslant$.

Với mọi $a \in I(A)$, theo giả thiết tồn tại một $d \neq 0$ nào đó trong A sao cho $a \subset Ad - 1$; giao $\tilde{a}$ của các iđêan chính phân chứa a do đó là một phần tử của I(A). Hiển nhiên quan hệ $a \prec b$ tương đương với quan hệ $\tilde{a} \supset 6$; do đó quan hệ $a \supset b$ kéo theo $a \prec b$. Để hai phần tử $a, b$ của I(A) tương đương modulo R, điều kiện cần và đủ là $\tilde{a} = 6$.

#### Định nghĩa 2 {#ac-vii-s1-def-2 .statement}

*Mỗi phần tử a của I(A) sao cho $a = \tilde{a}$ được gọi là một iđêan phân kiểu chia của A.*

Nói cách khác, một iđêan phân kiểu chia chỉ là một giao khác không của một họ không rỗng các iđêan chính phân. Mọi giao khác không của các iđêan phân kiểu chia là một iđêan phân kiểu chia. Nếu a là kiểu chia, thì ax cũng vậy với mọi $x \in K^*$, ánh xạ $b \mapsto bx$ là một song ánh của tập hợp các iđêan chính phân lên chính nó. Với mọi $a \in I(A)$, 6 là iđêan phân kiểu chia nhỏ nhất chứa a và tương đương với a modulo R. Hơn nữa, nếu $b$ là một iđêan phân kiểu chia tương đương với a modulo R, thì $\tilde{a} = 6 = b$. Do đó 5 là iđêan phân kiểu chia duy nhất $b$ sao cho div $a =$ div $b$ (nói cách khác, hạn chế của ánh xạ $a \mapsto$ div $a$ lên tập hợp các iđêan phân kiểu chia là đơn ánh).

Cho a và b là hai iđêan phân của K. Nhắc lại (Chương I, § 2, no. 10) rằng $b : a$ ký hiệu tập hợp các $x \in K$ sao cho $xa \subset b$; đây hiển nhiên là một A-môđun; nếu $b \in I(A)$ và $a \in I(A)$, thì $b : a \in I(A)$; vì nếu $d$ là một phần tử khác không của A sao cho $db \subset A$ và $da \subset A$ và $a$ là một phần tử khác không của $A \cap a$, thì $da(b : a) \subset A$; mặt khác, nếu $b \neq 0$ thuộc về $b$, thì $bda \subset b$, do đó $bd \in b : a$ và $b : a \neq 0$.

Định nghĩa của $b : a$ cũng có thể được viết:

$$
(1) \quad b : a = \bigcap_{x \in a, x \neq 0} b x^{-1}.
$$

#### Mệnh đề 1 {#ac-vii-s1-prop-1 .statement}

(a) *Nếu b là một iđêan kiểu chia và $a \in I(A)$, $b : a$ là kiểu chia.*

(b) *Cho a, b thuộc I(A). Để div $a =$ div $b$, điều kiện cần và đủ là $A : a = A : b$.*

(c) *Với mọi $a \in I(A)$, $6 = A : (A : a)$.*

Khẳng định (a) suy ra ngay lập tức từ công thức (1) vì, nếu $b$ là kiểu chia, thì $b x^{-1}$ cũng là kiểu chia với mọi $x \neq 0$.

Để chứng minh (b), ký hiệu $P(a)$ là tập hợp các iđêan chính phân chứa a; quan hệ $Ax \in P(a)$ tương đương với $x^{-1} a \subset A$ và do đó tương đương với $x^{-1} \in A : a$. Vì quan hệ div $a =$ div $b$ theo định nghĩa tương đương với $P(a) = P(b)$, nó cũng tương đương với $A : a = A : b$.

Cuối cùng, vì $a(A : a) \subset A, a \subset A : (A : a)$. Thay thế $a$ bởi $A : a$ trong công thức này, ta thấy rằng $A : a \subset A : (A : (A : a))$; mặt khác, quan hệ $a \subset A : (A : a)$ kéo theo
$$
A : a \supset A : (A : (A : a)).
$$
Do đó $A : a = A : (A : (A : a))$ và suy ra từ (b) rằng $\operatorname{div} a = \operatorname{div}(A : (A : a))$
Vì $A : (A : a)$ là chia được theo (a), chắc chắn $6 = A : (A : a)$, điều này chứng minh (c).

#### Nhận xét {#ac-vii-s1-n1-rem-1 .statement}

Trong quá trình chứng minh ở trên, ta đã chứng minh rằng $A : a = A : (A : (A : a))$ đối với mọi iđêan $a \in I(A)$, đây là một trường hợp đặc biệt của *Lý thuyết tập hợp*, Chương 111, § 1, no. 5, Mệnh đề 2.

#### Mệnh đề 2 {#ac-vii-s1-prop-2 .statement}

(i) *Trong $D(A)$ mọi tập hợp khác rỗng bị chặn trên đều có một cận trên nhỏ nhất. Chính xác hơn, nếu $(a_i)$ là một họ khác rỗng các phần tử của $I(A)$ bị chặn trên, thì*
$$
\sup(\operatorname{div} a_i) = \operatorname{div}\left( \bigcap_i 5_i \right).
$$
(ii) *Trong $D(A)$ mọi tập hợp khác rỗng bị chặn dưới đều có một cận dưới lớn nhất. Chính xác hơn, nếu $(a_i)$ là một họ khác rỗng các phần tử của $I(A)$ bị chặn dưới, thì*
$$
\inf(\operatorname{div} a_i) = \operatorname{div}\left( \sum_i a_i \right).
$$
(iii) *Tập hợp $D(A)$ là một dàn.*

Cho $(a_i)$ là một họ khác rỗng các phần tử của $I(A)$ bị chặn trên. Nói rằng một iđêan chia được $b$ chặn trên họ này có nghĩa là nó được chứa trong mọi $a_i$, tức là $b$ được chứa trong $\bigcap_i 6_i$. Do đó $\bigcap_i a_i \neq (0)$ và $\bigcap_i 6_i$, vì vậy là một iđêan chia được, điều này chứng minh (i).

Bây giờ cho $(6_i)$ là một họ khác rỗng các phần tử của $I(A)$ bị chặn dưới. Nói rằng một iđêan chia được $b$ chặn dưới họ này có nghĩa là nó chứa mọi $a_i$, tức là (vì $b$ là chia được) nó chứa mọi $a_i$, hoặc cũng có nghĩa là $b \supset \sum_i a_i$. Điều này chứng minh (ii).

Cuối cùng, để chứng minh (iii) chỉ cần theo (i) và (ii) chứng minh rằng, nếu $a, b$ thuộc $I(A)$, tập hợp $\{a, b\}$ bị chặn cả trên lẫn dưới trong $I(A)$; bây giờ nó bị chặn trên bởi $a \cap b$ (phân biệt với $(0)$). Nó bị chặn dưới bởi $a + b$, vì $a + b \in I(A)$: nếu $d$ và $d'$ là các phần tử khác không của $A$ sao cho $da \subset A$ và $d'b \subset A$, thì $dd'(a + b) \subset A$.

#### Hệ quả {#ac-vii-s1-n1-cor-1 .statement}

*Nếu $x, y$ và $x + y$ thuộc $K^*$, thì $\operatorname{div}(x + y) \geq \inf(\operatorname{div}(x), \operatorname{div}(y))$.*

$A(x + y) \subset Ax + Ay$ và do đó $\operatorname{div}(x + y) \geq \operatorname{div}(Ax + Ay)$.

### 2. CẤU TRÚC MONÔĐ TRÊN D(A)

#### Mệnh đề 3 {#ac-vii-s1-prop-3 .statement}

Cho $a, a', b, b'$ là các phần tử của $I(A)$. Các quan hệ $a > a'$ và $b > b'$ kéo theo $ab > a'b'$.

Ta có thể hạn chế sự chú ý của mình vào trường hợp $b = b'$. Khi đó cho $Ax$ là một iđêan chính phân thức chứa $a'b$; với mọi phần tử khác không $y$ của $b$, $Ax \supset a'y$ và do đó $Axy^{-1} \supset a'$, do đó $Axy^{-1} \supset a$ và $Ax \supset ay$. Thay đổi $y$, ta thấy rằng $Ax \supset ab$, do đó $ab > a'b$.

Suy ra từ Mệnh đề 3 rằng phép nhân trên $I(A)$ xác định, bằng cách chuyển qua thương, một luật hợp thành trên $D(A)$ hiển nhiên kết hợp và giao hoán. Nó được viết theo phép cộng để ta có thể viết:

$$
\text{div}(ab) = \text{div } a + \text{div } b,
$$

với $a, b$ thuộc $I(A)$. Rõ ràng $\text{div}(1)$ là một phần tử đơn vị đối với phép cộng này; phần tử này được ký hiệu là 0. Mệnh đề 3 còn chứng minh rằng cấu trúc thứ tự trên $D(A)$ là *tương thích* với phép cộng này (*Algebra*, Chương VI, § 1, no. 1) và, chính xác hơn (no. 1, Mệnh đề 2 (ii)):

$$
\inf(\text{div } a + \text{div } b, \text{div } a + \text{div } c) = \inf(\text{div}(ab), \text{div}(ac)) = \text{div}(ab + ac)
= \text{div}(a(b + c)) = \text{div} a + \text{div}(b + c) = \text{div} a + \inf(\text{div } b, \text{div } c).
$$

Đối với một iđêan phân thức $a \neq 0$ sao cho $\text{div } a \geq 0$ trong $D(A)$, điều kiện cần và đủ là $a \subset A$ (nói cách khác, $a$ là một iđêan *nguyên* của $A$).

Đối với hai phần tử $x, y$ của $K^*$, quan hệ $\text{div}(x) = \text{div}(y)$ tương đương với $Ax = Ay$; tập hợp các ước chính của $A$ với quan hệ thứ tự và luật nửa nhóm cảm sinh bởi luật trên $D(A)$ là một *nhóm có thứ tự* đẳng cấu chính tắc với nhóm nhân của các iđêan chính phân thức được sắp thứ tự bởi quan hệ thứ tự đối với bao hàm (*Algebra*, Chương VI, § 1, no. 5). Quan hệ $S$ giữa hai phần tử $P, Q$ của $D(A)$:

"tồn tại $x \in K^*$ sao cho $P = Q + \text{div}(x)$"

do đó là một quan hệ tương đương vì quan hệ $P = Q + \text{div}(x)$ tương đương với $Q = P + \text{div}(x^{-1})$; nếu $P$ và $Q$ đồng dư theo môđun $S$, chúng được gọi là các ước tương đương của $A$. Hơn nữa, rõ ràng quan hệ $S$ tương thích với luật của nửa nhóm $D(A)$ và do đó nửa nhóm sau xác định, bằng cách lấy thương, một cấu trúc nửa nhóm trên $D(A)/S$; nửa nhóm này được gọi là *nửa nhóm lớp ước của A*.

#### Mệnh đề 4 {#ac-vii-s1-prop-4 .statement}

Cho $a, b$ là hai iđêan phân thức chia của $A$. Các tính chất sau là tương đương:
(a) $\text{div } a$ và $\text{div } b$ là các ước tương đương;
(b) tồn tại $x \in K^*$ sao cho $b = xa$.

Nếu $\operatorname{div} b = \operatorname{div} a + \operatorname{div}(x)$ với một số $x \in K^*$, thì $\operatorname{div} b = \operatorname{div}(xa)$ và, vì $b$ và $xa$ là các iđêan chia được, ta có $b = xa$, điều này chứng minh mệnh đề.

Cho $a$ là một iđêan phân số khả nghịch (Chương II, § 5, no. 6); khi đó $a = A : (A : a)$ (*loc. cit.*, Mệnh đề 10) và do đó $a$ là *chia được* (no. 1, Mệnh đề 1). Nhóm $J(A)$ của các iđêan phân số khả nghịch do đó được đồng nhất với một nhóm con của monôit $D(A)$ và ảnh chính tắc của $J(A)$ trong $D(A)/S$ với nhóm các lớp của các $A$-môđun *xạ ảnh* có *hạng* 1 (Chương II, § 5, no. 7, Hệ quả 2 của Mệnh đề 12 và *Nhận xét* 1).

#### Định lý 1 {#ac-vii-s1-thm-1 .statement}

*Cho $A$ là một miền nguyên. Để monôit $D(A)$ của các ước của $A$ là một nhóm, điều kiện cần và đủ là $A$ được đóng nguyên hoàn toàn.*

Giả sử rằng $D(A)$ là một nhóm. Cho $x \in K$; giả sử rằng $A[x]$ được chứa trong một môđun con $A$-sinh hữu hạn của $K$. Khi đó ta đã thấy (no. 1) rằng $a = A[x]$ là một phần tử của $I(A)$. Khi đó $xa \subset a$ và do đó $\operatorname{div}(x) + \operatorname{div} a \geq \operatorname{div} a$. Vì $D(A)$ là một nhóm có thứ tự, ta kết luận rằng $\operatorname{div}(x) \geq 0$, do đó $x \in A$. Vậy $A$ là đóng nguyên hoàn toàn (Chương V, § 1, số **4**, Định nghĩa 5).

Ngược lại, giả sử rằng $A$ được đóng nguyên hoàn toàn. Cho $a$ là một iđêan chia được. Ta sẽ chứng minh rằng $\operatorname{div} a + \operatorname{div}(A : a) = 0$, điều này sẽ chứng minh rằng $D(A)$ là một nhóm. Vì $a(A : a) \subset A$, chỉ cần (no. 1) kiểm tra rằng mọi iđêan chính phân số $Ax^{-1}$ chứa $a(A : a)$ cũng chứa $A$. Bây giờ, với $y \in K^*$, quan hệ $Ay \supset a$ kéo theo $y^{-1} \in A : a$, do đó $y^{-1}a \subset a(A : a) \subset Ax^{-1}$ và vì thế $xa \subset Ay$. Vì $a$ là chia được, ta suy ra rằng $xa \subset a$, do đó $x^n a \subset a$ với mọi $n \in \mathbf{N}$. Tồn tại các phần tử $x_0, x_1$ của $K^*$ sao cho $Ax_0 \subset a \subset Ax_1$; do đó $x^n x_0 \in Ax_1$, và vì thế $x^n \in Ax_1 x_0^{-1}$. Vì $A$ được đóng nguyên hoàn toàn, $x \in A$, nghĩa là $Ax^{-1} \supset A$, điều này hoàn tất chứng minh.

Chú ý rằng, nếu $A$ được đóng nguyên hoàn toàn (và thậm chí Noether), một iđêan chia được của $A$ không nhất thiết khả nghịch, nói cách khác, nói chung $J(A) \neq D(A)$ (Bài tập 2 và § 3, no. 2, Mệnh đề 1).

#### Hệ quả {#ac-vii-s1-n2-cor-1 .statement}

*Cho $A$ là một miền nguyên đóng hoàn toàn và $a$ là một iđêan phân thức chia được của $A$. Khi đó, với mọi iđêan phân thức $b \neq 0$ của $A$, $\operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b$*

Theo công thức (1) của no. 1:

$$
\operatorname{div}(a : b) = \operatorname{div}\left( \bigcap_{y \in b, y \neq 0} y^{-1}a \right) = \sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1}a)
$$

có tính đến Mệnh đề 2 và sự kiện rằng các iđêan phân thức $y^{-1}a$ là chia được. Nhưng vì $D(A)$ là một nhóm có thứ tự (*Đại số*, Chương VI, § 1, no. 8):

$$
\sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1}a) = \sup_{y \in b, y \neq 0} (\operatorname{div} a - \operatorname{div}(y)) \\
= \operatorname{div} a - \inf_{y \in b, y \neq 0} \operatorname{div}(y) = \operatorname{div} a - \operatorname{div} b.
$$

### 3. MIỀN KRULL

#### Định nghĩa 3 {#ac-vii-s1-def-3 .statement}

Một miền nguyên $A$ được gọi là một miền Krull nếu tồn tại một họ $(v_i)_{i \in I}$ các định giá trên trường phân thức $K$ của $A$ với các tính chất sau:
(AK,) các định giá $v_i$ là rời rạc;
(AK,,) giao của các vành & $v_i$ là $A$;
(AK,,,) với mọi $x \in K^*$, tập hợp các chỉ số $t \in I$ sao cho $v_t(x) \neq 0$ là hữu hạn.

Hiển nhiên chỉ cần kiểm tra điều kiện (AK$_{III}$) đối với các phần tử $x$ của $A - (0)$.

Ví dụ
(1) Mọi vành định giá rời rạc đều là một miền Krull.
(2) Nói chung hơn, mọi miền iđêan chính $A$ đều là một miền Krull. Thật vậy, cho $(p_i)_{i \in I}$ là một hệ đại diện các phần tử cực biên của $A$ và $v_i$ là định giá trên trường phân thức của $A$ được xác định bởi $p_i$ (Chương VI, § 3, no. 3, Ví dụ 4). Ta thấy ngay lập tức rằng họ $(v_i)_{i \in I}$ thỏa mãn các tính chất (AK$_I$), (AK$_II$) và (AK$_{III}$).
(3) Cho $F$ là một trường và $(R_i)_{1 \leq i \leq n}$ là một họ hữu hạn các vành con của $F$ mà đều là các miền Krull. Khi đó giao của chúng $S = \bigcap_{j=1}^n R_j$, là một miền Krull. Với $1 \leq j \leq n$, cho $(v_{j,t})_{t \in I_j}$ là một họ các định giá trên trường phân thức của $R_j$, thỏa mãn (AK$_I$), (AK$_{II}$), (AK$_{III}$) (ở đó $A$ được thay bằng $R_j$). Ký hiệu $w_{j,t}$ là hạn chế của $v_{j,t}$ lên trường phân thức của $S$. Khi đó họ $(v_{j,t})_{1 \leq j \leq n, t \in I_j}$ hiển nhiên thỏa mãn (AK$_{II}$) (ở đó $A$ được thay bằng $S$) và cả (AK$_{III}$) vì tập hợp các chỉ số$j$ là hữu hạn. Các định giá $w_{j,t}$ hoặc là rời rạc, hoặc là không chính quy. Chỉ giữ lại những định giá nào là rời rạc, ta thu được một họ hiển nhiên thỏa mãn (AK$_I$), (AK$_{II}$) và (AK$_{,,}$) (ở đó $A$ được thay bằng $S$). Do đó chắc chắn $S$ là một miền Krull.
(4) Đặc biệt, nếu $A$ là một miền Krull và $K'$ là một trường con của trường phân thức $K$ của $A$, thì $K' \cap A$ là một miền Krull.

#### Định lý 2 {#ac-vii-s1-thm-2 .statement}

Cho $A$ là một miền nguyên. Để $A$ là một miền Krull, điều kiện cần và đủ là hai điều kiện sau được thỏa mãn:
(a) $A$ là nguyên đóng hoàn toàn;
(b) mọi họ không rỗng các iđêan nguyên divisorial của $A$ đều thừa nhận một phần tử cực đại (đối với quan hệ $\subset$).
Hơn nữa, nếu $P(A)$ là tập hợp các phần tử cực biên của $D(A)$, thì $P(A)$ là một cơ sở của $\mathbf{Z}$-môđun $D(A)$ và các phần tử dương của $D(A)$ là các tổ hợp tuyến tính của các phần tử của $P(A)$ với các hệ số $\geq 0$.

Cho $A$ là một miền Krull. Nó là hoàn toàn đóng nguyên (Chương VI, § 4, no. 5, Hệ quả của Mệnh đề 9). Cho $(v_i)_{i \in I}$ là một họ các định giá trên trường các phân thức $K$ của $A$ thỏa mãn (AK$_I$), (AK$_{II}$) và (AK$_{III}$). Có thể giả sử rằng các $v_i$ được chuẩn hóa (Chương VI, § 3, no. 6, Định nghĩa 3). Với mọi $a \in I(A)$, ta sẽ viết:

$$
v_t(a) = \sup_{a \subset Ax} (v_t(x));
$$

khi đó $v_t(a) \in \mathbf{Z}$, vì, nếu $a$ là một phần tử khác không của $a$, quan hệ $Ax \supset Aa$ kéo theo rằng $v_t(x) \leq v_t(a)$ (theo (AK$_{III}$)), điều này chứng tỏ rằng họ các $v_t(x)$ ($a \subset Ax$) bị chặn trên. Ta thiết lập các tính chất sau:

(1) *Cho $a$ là một iđêan phân thức chia được; để $y \in a$, điều kiện cần và đủ là $v_t(y) \geq v_t(a)$ với mọi $t \in I$.*

Vì $a$ là chia được, quan hệ $y \in a$ tương đương với quan hệ ““$a \subset Ax$ kéo theo $y \in Ax$”. Bây giờ, theo (AK,,), quan hệ $y \in Ax$ tương đương với “$v_t(y) \geq v_t(x)$ với mọi $t \in I$”. Do đó có (1).

(2) *Cho $a$ và $b$ là hai iđêan phân thức chia được của $A$; để $a \subset b$, điều kiện cần và đủ là $v_t(a) \geq v_t(b)$ với mọi $t \in I$.*

Điều này suy ra ngay lập tức từ tính chất (1).

(3) *Nếu $x \in K^*$, thì $v_t(Ax) = v_t(x)$.*

Nếu $Ay \supset Ax$, thì $v_t(y) \leq v_t(x)$ theo (AK,,) và giá trị cực tiểu của $v_t(y)$ đạt được tại $y = x$.

(4) *Với mọi $a \in I(A)$, các chỉ số $t \in I$ sao cho $v_t(a) \neq 0$ là hữu hạn về số lượng.*

Tồn tại $x, y$ trong $K^*$ sao cho $Ax \subset a \subset Ay$. Theo các tính chất (2) và (3), $v_t(x) \geq v_t(a) \geq v_t(y)$ với mọi $t \in I$. Khi đó chỉ cần áp dụng (AK$_{III}$).

Do đó ta đã chứng minh bổ đề sau:

#### Bổ đề 1 {#ac-vii-s1-lem-1 .statement}

*Nếu $A$ là một miền Krull và $(v_t)_t$, là một họ các định giá chuẩn hóa trên $K$ thỏa mãn (AK, ), (AK,,) và (AK$_{III}$), ánh xạ $a \mapsto (v_t(a))_{t \in I}$ là một ánh xạ đơn ánh giảm từ tập hợp các iđêan nguyên chia được của $A$ (có thứ tự bởi $\subset$) vào tập hợp các phần tử dương & nhóm có thứ tự là tổng trực tiếp $\mathbf{Z}^{(I)}$.*

Với điều này, mọi tập hợp không rỗng các phần tử dương của $\mathbf{Z}^{(I)}$ đều có một phần tử cực tiểu (*Đại số*, Chương VI, § 1, no. 13, Định lý 2). Do đó $A$ chắc chắn thỏa mãn tính chất (b) của mệnh đề.

Ngược lại, cho $A$ là một miền nguyên thỏa mãn các tính chất (a) và (b) của mệnh đề. Vì $A$ là nguyên đóng hoàn toàn, $D(A)$ là một nhóm có thứ tự (no. 2, Định lý 1). Nhóm này là một dàn (no. 1, Mệnh đề 2). Theo điều kiện (b) của mệnh đề, mọi họ không rỗng các phần tử dương của $D(A)$ đều có một phần tử cực tiểu. Gọi $P(A)$ là tập hợp các phần tử cực biên của $D(A)$. Khi đó (*Đại số*, Chương VI, § 1, no. 13, Định lý 2) $P(A)$ là một cơ sở của $\mathbf{Z}$-môđun $D(A)$ và các phần tử dương của $D(A)$ là các tổ hợp tuyến tính với các hệ số nguyên dương của các phần tử của $P(A)$.

Do đó, với $x \in K^*$, các số nguyên hữu tỉ $v_P(x)$ được xác định (với $P \in P(A)$) bằng cách viết:

$$
\text{div}(x) = \sum_{P \in P(A)} v_P(x) \cdot P.
$$

Ta cũng viết $v_P(0) = +\infty$.

Từ các hệ thức

$$
\text{div}(xy) = \text{div}(x) + \text{div}(y)
$$

và

$$
\text{div}(x + y) \geq \inf(\text{div}(x), \text{div}(y)),
$$

với $x, y$ và $x + y$ thuộc $K^*$, ta suy ra rằng các $v_P$ là những *định giá rời rạc* trên $K$. Để có $x \in A$, điều kiện cần và đủ là $\text{div}(x) \geq 0$, nghĩa là $v_P(x) \geq 0$ với mọi $P \in P(A)$. Do đó các $v_P$ thỏa mãn các điều kiện (AK$_1$) và (AK$_{11}$), và hiển nhiên cũng thỏa mãn (AK$_{III}$).

#### Hệ quả {#ac-vii-s1-n3-cor-1 .statement}

*Điều kiện cần và đủ để một vành Noether là một miền Krull là nó là một miền nguyên đóng.*

Một miền Noether nguyên đóng là nguyên đóng hoàn toàn (Chương V, § 1, no. 4).

Có những miền Krull không Noether, chẳng hạn vành đa thức $K[X_n]_{n \in \mathbf{N}}$ trên một trường $K$ theo một vô hạn các ẩn số (xem Bài tập 8).

### 4. CÁC ĐỊNH GIÁ CỐT YẾU CỦA MỘT MIỀN KRULL

Cho $A$ là một miền Krull và $K$ là trường phân thức của nó. Các định giá được xác định bởi công thức (4) của no. 3 (với $x \in K^*$) được gọi là các *định giá cốt yếu* của $K$ (*hoặc* của $A$).

Ta đã nhận xét trong quá trình chứng minh Định lý 2 rằng các định giá $v_P$ thỏa mãn các tính chất (AK$_1$), (AK$_2$) và (AK$_{III}$) của Định nghĩa 3. Hơn nữa, các định giá rời rạc $v_P$ này là *được chuẩn hóa*: với mọi ước cực biên $P \in P(A)$, ta có $P < 2P$ và vì thế, nếu $a$ và $b$ là các iđêan ước tương ứng với $P$ và $2P$, thì $a \supseteq b$ và $a \neq b$; với $x \in a - b$, $\text{div}(x) \geq P$ và $\text{div}(x) \not\geq 2P$, do đó $v_P(x) = 1$, điều này chứng minh mệnh đề của ta.

#### Mệnh đề 5 {#ac-vii-s1-prop-5 .statement}

*Cho $A$ là một miền Krull, $K$ là trường phân thức của nó và $(v_P)_{P \in P(A)}$ là họ các định giá cốt yếu của nó. Cho $(n_P)_{P \in P(A)}$ là một họ các số nguyên, bằng không trừ đối với một số hữu hạn chỉ số. Khi đó tập hợp các $x \in K$ sao cho $v_P(x) \geq n_P$ với mọi $P \in P(A)$ là iđêan ước $a$ của $A$ sao cho $\text{div } a = \sum_{P \in P(A)} n_P \cdot P$.*

Cho $x \in K^*$. Để có $x \in a$, điều cần và đủ là $Ax \subset a$, do đó là $\text{div}(x) \geq \text{div } a$ và vì thế, theo (4), là $v_P(x) \geq n_P$ với mọi $P \in P(A)$.

#### Mệnh đề 6 {#ac-vii-s1-prop-6 .statement}

Cho $A$ là một miền Krull, $K$ là trường phân thức của nó, $(v_t)_{t \in I}$ là một họ các định giá trên $K$ có các tính chất của Định nghĩa 3 và $A$, vành của các $v_t$. Cho $S$ là một tập con nhân của $A$ không chứa $0$ và $J$ là tập hợp các chỉ số $t \in I$ sao cho $v_t$ bằng không trên $S$. Khi đó $S^{-1}A = \bigcap_{t \in J} A_t$; đặc biệt $S^{-1}A$ là một miền Krull.

Đặt $B = \bigcap_{t \in J} A_t$. Khi đó $S^{-1} \subset B$ và $A \subset B$ và vì thế $S^{-1}A \subset B$. Ngược lại, cho $x \in B$. Gọi $J'$ là tập hợp hữu hạn các chỉ số $t$ sao cho $v_t(x) < 0$. Nếu $t \in J'$, thì $x \notin A_t$, do đó $t \notin J$ và vì thế tồn tại $s_t \in S$ sao cho $v_t(s_t) > 0$. Cho $n(t)$ là một số nguyên $> 0$ sao cho $v_t(s_t^{n(t)}x) \geq 0$; đặt $s = \prod_{t \in J'} s_t^{n(t)}$. Khi đó $v_t(sx) \geq 0$ với mọi $t \in I$ và vì thế $sx \in A$ và $x \in S^{-1}A$. Vậy $B = S^{-1}A$.

#### Hệ quả 1 {#ac-vii-s1-prop-6-cor-1 .statement}

Cho $P$ là một ước cực biên của $A$ và $p$ là iđêan ước tương ứng. Khi đó $p$ là nguyên tố, vành của $v_P$ là $A$, và trường thặng dư của $v_P$ được đồng nhất với trường phân thức của $A/p$.

Đặt $S = A - p$. Theo Mệnh đề 5, $v_P$ bằng không trên $S$ và $> 0$ trên $p$. Do đó $p$ là giao của $A$ và iđêan của $v_P$ nên là nguyên tố. Mặt khác, với mọi ước cực biên $Q \neq P$, ta có $Q \not\subset P$ và do đó iđêan ước $q$ tương ứng với $Q$ không được chứa trong $p$; vì thế $q \cap S \neq \varnothing$ và suy ra, theo Mệnh đề 5, $v_Q$ không bằng không trên $S$. Như vậy, hệ quả suy ra từ Mệnh đề 6 và Chương II, § 3, no. 1, Mệnh đề 3.

#### Hệ quả 2 {#ac-vii-s1-prop-6-cor-2 .statement}

Cho $A$ là một miền Krull, $K$ là trường phân thức của nó và $(v_t)_{t \in I}$ là một họ các định giá có các tính chất của Định nghĩa 3. Khi đó mọi định giá cốt yếu của $A$ đều tương đương với một trong các $v_t$.

Cho $P$ là một ước cực biên của $A$ và $p$ là iđêan ước tương ứng. Theo Hệ quả 1, Mệnh đề 5, Bổ đề 1 và mệnh đề (1) trong chứng minh của Định lý 2, no. 3, tồn tại $t \in I$ sao cho vành $A_t$ của $v_t$ chứa vành $A$ của $v_P$. Vì $v_t$ và $v_P$ có chiều cao 1, nên chúng tương đương với nhau (Chương VI, § 4, no. 5, Mệnh đề 6).

#### Mệnh đề 7 {#ac-vii-s1-prop-7 .statement}

Cho $A$ là một miền Krull, $(v_P)_{P \in P(A)}$ là họ các định giá cốt yếu của nó và $a \in I(A)$. Khi đó hệ số của $P$ trong $\operatorname{div} a$ là $\inf_{y \in a} (v_P(y))$. Nếu $p$ là iđêan nguyên tố ước tương ứng với ước cực biên $P$, thì $aA_p = \tilde{a}A_p$.

Vì $a = \sum_{y \in a} Ax$, Mệnh đề 2 (b) (no. 1) cho thấy rằng $\operatorname{div}(a) = \inf_{x \in a} (\operatorname{div}(Ax))$, do đó có mệnh đề thứ nhất của chúng ta. Mệnh đề thứ hai suy ra ngay lập tức, vì $\operatorname{div} \tilde{a} = \operatorname{div} a$ và $A_p$ là vành của định giá rời rạc $v_P$.

#### Mệnh đề 8 {#ac-vii-s1-prop-8 .statement}

Cho $A$ là một miền Noether đóng nguyên.
(a) Cho $P$ là một ước cực biên của $A$ và $p$ là iđêan nguyên tố ước tương ứng;

với $n \in \mathbf{N}$, đặt $p^{(n)} = p^n A_p \cap A$; khi đó $p^{(n)}$ là tập hợp các $x \in A$ sao cho $v_p(x) \geq n$ và là một iđêan nguyên sơ theo $p$.

(b) Cho $a$ là một iđêan nguyên ước, $n_1 P_1 + \ldots + n_r P_r$ là ước của $a$ (các $P_i$ là những ước cực biên phân biệt) và $p_i$ là iđêan nguyên tố ước tương ứng với $P_i$. Khi đó $a = \bigcap_{i=1}^r p_i^{(n_i)}$ là phân tích nguyên sơ thu gọn duy nhất của $a$ và các $p_i$ không bị nhúng.

Theo Hệ quả 1 của Mệnh đề 6, quan hệ $x \in p^n A_p = (pA_p)^n$ tương đương với $v_p(x) \geq n$; mặt khác, vì $A_p$ là một vành định giá rời rạc, $(pA_p)^n$ là nguyên sơ theo $(pA_p)$ (Chương IV, § 2, no. 1, Ví dụ 4) và do đó $p^{(n)}$ là nguyên sơ theo $p$ (Chương IV, § 2, no. 1, Mệnh đề 3); điều này chứng tỏ (a). Mệnh đề 5 hiển nhiên cho thấy rằng $a = \bigcap_{i=1}^r p_i^{(n_i)}$. Vì $p_i \not\subset p_j$ khi $i \neq j$ nên phân tích nguyên sơ này là thu gọn: Thật vậy, nếu $p_i^{(n_i)} \supset \bigcap_{j \neq i} p_j^{(n_j)} \supset \prod_{j \neq i} p_j^{(n_j)}$, thì $p_i$ sẽ chứa một trong các $p_j$ với $j \neq i$ (Chương II, § 1, no. 1, Mệnh đề 1). Tính duy nhất suy ra từ Chương IV, § 2, no. 3, Mệnh đề 5.

### 5. XẤP XỈ ĐỐI VỚI CÁC ĐỊNH GIÁ CỐT YẾU

Vì các định giá cốt yếu của một miền Krull là rời rạc và được chuẩn hóa, không có hai định giá nào trong chúng là tương đương và do đó chúng độc lập (Chương VI, § 7, no. 2). Bởi vậy có thể áp dụng Hệ quả 2 của định lý xấp xỉ (loc. cit., Định lý 1) cho chúng: cho các $n_i \in \mathbf{Z}$ và các định giá cốt yếu $v_i$ hữu hạn về số lượng và phân biệt, tồn tại $x \in K$ sao cho $v_i(x) = n_i$ với mọi $i$. Nhưng ở đây có một kết quả chính xác hơn:

#### Mệnh đề 9 {#ac-vii-s1-prop-9 .statement}

Cho $v_1, \ldots, v_r$ là những định giá cốt yếu phân biệt của một miền Krull $A$ và $n_1, \ldots, n_r$ là các số nguyên hữu tỉ. Tồn tại một phần tử $x$ của trường phân thức $K$ của $A$ sao cho $v_i(x) = n_i$ với $1 \leq i \leq r$ và $v(x) \geq 0$ đối với mọi định giá cốt yếu $v$ của $A$ khác $v_1, \ldots, v_r$.

Cho $p_1, \ldots, p_r$ là các iđêan chia được của $A$ tương ứng với các định giá $v_1, \ldots, v_r$. Tồn tại $y \in K$ sao cho $v_i(y) = n_i$ với $1 \leq i \leq r$ (Chương VI, § 7, no. 2, Hệ quả 1 của Định lý 1). Các định giá cốt yếu $w_1, \ldots, w_s$ của $A$ phân biệt với các $v_i$ mà với chúng số nguyên $w_j(y) = -m_j$ là $< 0$ chỉ có hữu hạn; gọi $q_1, \ldots, q_s$ là các iđêan tương ứng. Không tồn tại quan hệ bao hàm nào giữa $p_1, \ldots, p_r, q_1, \ldots, q_s$ vì các iđêan này tương ứng với các ước cực biên và các iđêan này là nguyên tố (Hệ quả 1 của Mệnh đề 6). Do đó iđêan nguyên $a = q_1^{m_1} \ldots q_s^{m_s}$ không được chứa trong iđêan nào trong các $p_i$ (Chương 11, § 1, no. 1, Mệnh đề 1) và vì vậy không được chứa trong hợp của chúng (loc. cit., Mệnh đề 2). Vậy tồn tại $z \in a$ sao cho $z \notin p_i$ với $1 \leq i \leq r$; khi đó $v_1(z) = \cdots = v_r(z) = 0$ và $w_j(z) \geq m_j$ với $1 \leq j \leq s$; do đó phần tử $x = yz$ giải bài toán.

#### Hệ quả 1 {#ac-vii-s1-prop-9-cor-1 .statement}

Cho $\mathbf{A}$ là một miền Krull, $\mathbf{K}$ trường phân thức của nó và $\mathbf{a}, \mathbf{b}$ và $c$ là ba iđêan phân thức chia được của $\mathbf{A}$ sao cho $\mathbf{a} \subset \mathbf{b}$. Tồn tại $x \in \mathbf{K}$ sao cho $\mathbf{a} = \mathbf{b} \cap x\mathbf{c}$.

Cho $(v_t)_{t \in I}$ là họ các định giá cốt yếu của $\mathbf{A}$ và cho $(m,)$ (tương ứng $(n_t), (p_t)$) là họ các số nguyên hữu tỉ (bằng không trừ ra với một số hữu hạn chỉ số) sao cho $\mathbf{a}$ (tương ứng $\mathbf{b}, c$) là tập hợp các $x \in \mathbf{K}$ mà với chúng $v(x_t) \geq m$, (tương ứng $n_t, p_t$) với mọi $t \in I$ (Mệnh đề 5, no. 4). Tập hợp $\mathbf{J}$ các $t \in I$ sao cho $m_t > n_t$ là hữu hạn. Vì $p_t = m_t = 0$ trừ ra với một số hữu hạn chỉ số, Mệnh đề 9 cho thấy rằng tồn tại $x \in \mathbf{K}^*$ sao cho $v_t(x^{-1}) + m_t = p_t$ với $t \in \mathbf{J}$ và
$$
v_t(x^{-1}) + m_t \geq p_t
$$
với $t \in I - \mathbf{J}$. Khi đó, với mọi $t \in I$, $m_t = \sup(n_t, v_t(x) + p_t)$. Do đó $\mathbf{a} = \mathbf{b} \cap x\mathbf{c}$.

#### Hệ quả 2 {#ac-vii-s1-prop-9-cor-2 .statement}

Cho $\mathbf{A}$ là một miền Krull. Để một iđêan phân thức $\mathbf{a}$ của $\mathbf{A}$ là chia được, điều kiện cần và đủ là nó là giao của hai iđêan chính phân thức.

Tính đủ là hiển nhiên (no. 1, Định nghĩa 2). Tính cần suy ra từ Hệ quả 1: lấy $b$ và $c$ là các iđêan chính sao cho $b \supseteq a$.

### 6. CÁC IĐÊAN NGUYÊN TỐ CÓ CHIỀU CAO 1 TRONG MỘT MIỀN KRULL

#### Định nghĩa 4 {#ac-vii-s1-def-4 .statement}

Cho $\mathbf{A}$ là một miền nguyên. Một iđêan nguyên tố $\mathfrak{p}$ của $\mathbf{A}$ được gọi là có chiều cao 1 nếu nó là cực tiểu trong các iđêan nguyên tố khác không của $\mathbf{A}$.

Ta cũng sẽ nói rằng iđêan $(0)$ có chiều cao 0; do đó, theo định nghĩa, một iđêan nguyên tố có chiều cao $\leq 1$ thì bằng $(0)$ hoặc có chiều cao 1.

Dưới đây ta sẽ định nghĩa, theo một cách tổng quát, chiều cao của một iđêan nguyên tố.

#### Định lý 3 {#ac-vii-s1-thm-3 .statement}

Cho $\mathbf{A}$ là một miền Krull và $\mathfrak{p}$ là một iđêan nguyên của $\mathbf{A}$. Để $\mathfrak{p}$ là iđêan ước tương ứng với một ước cực biên, điều kiện cần và đủ là $\mathfrak{p}$ là một iđêan nguyên tố có chiều cao 1.

Nếu $\mathfrak{p}$ là iđêan ước tương ứng với một ước cực biên, ta biết (no. 4, Hệ quả 1 của Mệnh đề 6) rằng $\mathfrak{p}$ là nguyên tố và rằng $\mathbf{A}_\mathfrak{p}$ là một vành định giá rời rạc; vì $\mathbf{A}_\mathfrak{p}$ không có iđêan nguyên tố nào khác ngoài $(0)$ và $\mathfrak{p}\mathbf{A}_\mathfrak{p}$, nên $(0)$ và $\mathfrak{p}$ là các iđêan nguyên tố duy nhất của $\mathbf{A}$ được chứa trong $\mathfrak{p}$ (Chương II, § 3, no. 1, Mệnh đề 3); do đó $\mathfrak{p}$ có chiều cao 1. Ngược lại, trước hết ta sẽ chỉ ra rằng mọi iđêan nguyên tố $\mathfrak{p} \neq (0)$ của $\mathbf{A}$ đều chứa một iđêan nguyên tố ước $\mathfrak{q}$ tương ứng với một ước cực biên: thật vậy, vì $\mathbf{A}_\mathfrak{p} \neq K$, $\mathbf{A}_\mathfrak{p}$ là giao của một họ không rỗng $(\mathbf{A}_t)$ các vành định giá cốt yếu (no. 4, Mệnh đề 6); mỗi $\mathbf{A}_t$ có dạng $\mathbf{A}_{\mathfrak{q}_t}$ (no. 4, Hệ quả 1 của Mệnh đề 6) và từ $\mathbf{A}_\mathfrak{p} \subset \mathbf{A}_{\mathfrak{q}_t}$ ta suy ra rằng $\mathfrak{q}_t \subset \mathfrak{p}$. Vậy nếu $\mathfrak{p}$ có chiều cao 1, thì $\mathfrak{p} = \mathfrak{q}$, điều đó cho thấy rằng $\mathfrak{p}$ là iđêan ước tương ứng với một ước cực biên.

#### Hệ quả 1 {#ac-vii-s1-thm-3-cor-1 .statement}

Trong một miền Krull, mọi iđêan nguyên tố khác không m đều chứa một iđêan nguyên tố có chiều cao 1. Nếu m không có chiều cao 1, thì div m = 0 và A : m = A.

Mệnh đề thứ nhất đã được thấy trong quá trình chứng minh Định lý 3. Nếu m không có chiều cao 1 và p là một iđêan nguyên tố có chiều cao 1 được chứa trong m, thì p ⊂ m̃ và p ≠ m̃; vì div p là cực biên, tất yếu div m = div m̃ = 0; do đó div(A : m) = 0 và, vì A : m là ước (no. 1, Mệnh đề 1), A : m = A.

#### Hệ quả 2 {#ac-vii-s1-thm-3-cor-2 .statement}

Cho A là một miền Krull, K là trường phân thức của nó, v là một định giá trên K dương trên A và p là tập hợp các x ∈ A sao cho v(x) > 0. Nếu iđêan nguyên tố p có chiều cao 1, thì v tương đương với một định giá cốt yếu của A.

Cho B là vành của v và m là iđêan của nó. Khi đó m ∩ A = p và do đó A, ⊂ B. Bây giờ A,, là một vành định giá rời rạc (Định lý 3 và Hệ quả 1 của Mệnh đề 6). Vì p ≠ (0), B ≠ K và do đó B = A, (Chương VI, § 4, no. 5, Mệnh đề 6).

#### Định lý 4 {#ac-vii-s1-thm-4 .statement}

Cho A là một miền nguyên và M là tập hợp các iđêan nguyên tố của nó có chiều cao 1. Để A là một miền Krull, điều kiện cần và đủ là các Tính chất sau được thỏa mãn:
(i) Với mọi p ∈ M, A, là một vành định giá rời rạc.
(ii) A là giao của các A_p với p ∈ M.
(iii) Với mọi x ≠ 0 trong A, chỉ tồn tại một số hữu hạn iđêan p ∈ M sao cho x ∈ p.
Hơn nữa, các định giá tương ứng với các A_p với p ∈ M là các định giá cốt yếu của A.

Các điều kiện ấy hiển nhiên là đủ. Tính cần thiết của chúng suy ra ngay lập tức từ Định lý 3 của no. 4, Hệ quả I của Mệnh đề 6 và thực tế là các định giá cốt yếu của A thỏa mãn các điều kiện của Định nghĩa 3 của no. 3.

#### Mệnh đề 10 {#ac-vii-s1-prop-10 .statement}

Cho A là một miền Noether nguyên đóng và a là một iđêan nguyên của A. Các điều kiện sau là tương đương:
(a) a là ước;
(b) các iđêan nguyên tố liên kết với A/a có chiều cao 1.

Nhắc lại rằng, nếu a = $\bigcap^n q_i$ là một phân tích nguyên sơ thu gọn của a và p_i ký hiệu iđêan nguyên tố tương ứng với q_i, thì các iđêan nguyên tố liên kết với A/a chính là các p_i (Chương IV, § 2, no. 3, Mệnh đề 4). Khi đó việc (a) suy ra (b) suy ra từ Mệnh đề 8 của no. 4. Ngược lại, nếu, theo ký hiệu trên, các p_i có chiều cao 1, thì A_{p_i} là một vành định giá rời rạc (Định lý 4); mà, q_i = q_i A_{p_i} ∩ A (Chương IV, § 2, no. 1, Mệnh đề 3); ký hiệu v_i là định giá cốt yếu tương ứng với p_i, do đó tồn tại một số nguyên n_i sao cho q_i là tập hợp các x ∈ A sao cho v_i(x) ≥ n_i; điều này cho thấy rằng các q_i là ước (no. 4, Mệnh đề 5), do đó a cũng vậy.

### 7. ÁP DỤNG: NHỮNG ĐẶC TRƯNG MỚI CỦA CÁC VÀNH ĐỊNH GIÁ RỜI RẠC

#### Mệnh đề 11 {#ac-vii-s1-prop-11 .statement}

Cho $\mathbf{A}$ là một miền Krull địa phương (đặc biệt là một miền Noether địa phương nguyên đóng) và $m$ là iđêan cực đại của nó. Các điều kiện sau là tương đương:
(a) $\mathbf{A}$ là vành định giá rời rạc;
(b) $m$ là khả nghịch;
(c) $\mathbf{A}:m \neq \mathbf{A}$;
(d) $m$ là ước;
(e) $m$ là iđêan nguyên tố khác không duy nhất của $\mathbf{A}$.

Vì mọi iđêan khác không của một vành định giá rời rạc đều là chính (Chương VI, § 3, no. 6, Mệnh đề 9), nên nó khả nghịch và do đó (a) kéo theo (b). Nếu $m$ khả nghịch, thì nghịch đảo của nó là $\mathbf{A}:m$ (Chương II, § 5, no. 6, Mệnh đề 10) và do đó $\mathbf{A}:m \neq \mathbf{A}$; vì thế (b) kéo theo (c). Nếu $\mathbf{A}:m \neq \mathbf{A}$, thì $\mathbf{A}:(\mathbf{A}:m) \neq \mathbf{A}$; mà $m \subset \mathbf{A}:(\mathbf{A}:m)$; do đó $m = \mathbf{A}:(\mathbf{A}:m)$ vì $m$ là cực đại, nên $m$ là ước tính được (no. 1, Mệnh đề 1 (c)); do đó (c) kéo theo (d). Việc (d) kéo theo (e) suy ra từ Định lý 3 của no. 6. Cuối cùng, nếu $m$ là iđêan nguyên tố khác không duy nhất của $\mathbf{A}$, thì nó có chiều cao 1 và do đó $\mathbf{A}_m$ là một vành định giá rời rạc (no. 6, Định lý 4); vì $\mathbf{A}$ là địa phương, nên $\mathbf{A}_m = \mathbf{A}$, điều này chỉ ra rằng (e) kéo theo (a).

### 8. BAO ĐÓNG NGUYÊN CỦA MỘT MIỀN KRULL TRONG MỘT MỞ RỘNG HỮU HẠN CỦA TRƯỜNG PHÂN THỨC CỦA NÓ

#### Mệnh đề 12 {#ac-vii-s1-prop-12 .statement}

Cho $\mathbf{A}$ là một miền Krull, $K$ trường phân thức của nó, $K'$ là một mở rộng hữu hạn của $K$ và $\mathbf{A}'$ là bao đóng nguyên của $\mathbf{A}$ trong $K'$. Khi đó $\mathbf{A}'$ là một miền Krull. Các định giá cốt yếu của $\mathbf{A}'$ là các định giá rời rạc được chuẩn hóa trên $K'$ tương đương với các mở rộng của các định giá cốt yếu của $\mathbf{A}$.

Gọi $(v_i)_{i \in I}$ là họ các mở rộng lên $K'$ của các định giá cốt yếu của $\mathbf{A}$. Vì bậc $n = [K':K]$ là hữu hạn, nên các $v_i$ là các định giá rời rạc trên $K'$ (Chương VI, § 8, no. 1, Hệ quả 3 của Mệnh đề 1). Gọi $B_i$ là vành của $v_i$; khi đó $\mathbf{A}' \subset \bigcap_{L \in I} B_i$ (Chương VI, § 1, no. 3, Định lý 3). Ngược lại, mọi phần tử $x$ của $\bigcap_{i \in I} B_i$ đều nguyên trên mỗi vành định giá cốt yếu của $\mathbf{A}$ (Chương VI, § 1, no. 3, Hệ quả 3 của Định lý 3); do đó các hệ số của đa thức tối tiểu của $x$ trên $K$ thuộc $\mathbf{A}$ (Chương V, § 1, no. 3, Hệ quả của Mệnh đề 11), nên $x \in \mathbf{A}'$; vậy $\mathbf{A}' = \bigcap_{i \in I} B_i$. Bây giờ, gọi $x$ là một phần tử khác không của $\mathbf{A}'$; nó thỏa mãn một phương trình có dạng $x^s + a_{s-1}x^{s-1} + \ldots + a_0 = 0$

trong đó $a_i \in \mathbf{A}$ và $a_s \neq 0$; nếu $v_i(x) > 0$, thì $v_i(a_0) > 0$; mà các định giá cốt yếu $v$ của $\mathbf{A}$ sao cho $v(a_0) > 0$ chỉ hữu hạn về số lượng và các định giá trên $K'$ mở rộng một định giá đã cho trên $K$ cũng chỉ hữu hạn về số lượng (Chương VI, § 8, no. 3, Định lý 1); do đó $v_i(x) = 0$ trừ ra đối với một số hữu hạn chỉ số $i \in I$. Vậy đã chứng minh được rằng $\mathbf{A}'$ là một miền Krull (no. 3, Định nghĩa 3).

Còn phải chỉ ra rằng các $v_i$ tương đương với các định giá cốt yếu của $A'$ (no. 4, Hệ quả 2 của Mệnh đề 6), nghĩa là (no. 6, Hệ quả 2 của Định lý 3) iđêan nguyên tố $p_i$, gồm các $x \in A'$ sao cho $v_i(x) > 0$, có chiều cao 1. Nếu không phải như vậy, sẽ tồn tại một iđêan nguyên tố $q$ của $A'$ sao cho $(0) \subset q \subset p_i$ và phân biệt với $(0)$ và $p_i$; khi đó $(0) \subset q \cap A \subset p_i \cap A$ và $q \cap A$ sẽ phân biệt với $(0)$ và $p_i \cap A$ (Chương V, §2, no. 1, Hệ quả 1 của Mệnh đề 1); do đó iđêan nguyên tố $p_i \cap A$ sẽ không có chiều cao 1, điều này mâu thuẫn với việc nó tương ứng với một định giá cốt yếu của $A$.

#### Hệ quả {#ac-vii-s1-n8-cor-1 .statement}

*Cho $p$ (resp. $p'$) là một iđêan nguyên tố của $A$ (resp. $A'$) có chiều cao 1, và $v$ (resp. $u'$) là định giá cốt yếu của $A$ (resp. $A'$) tương ứng với nó. Để $p'$ nằm trên $p$, điều kiện cần và đủ là hạn chế của $v'$ trên $K$ tương đương với $v$.*

Định giá $v'$ tương đương với mở rộng của một định giá cốt yếu $w$ của $A$ (Mệnh đề 12). Đặt $q = p' \cap A$, đó là một iđêan nguyên tố của $A$ có chiều cao 1. Để hạn chế của $v'$ trên $K$ tương đương với $v$, điều kiện cần và đủ là $w = v$ và do đó $q = p$.

### 9. CÁC VÀNH ĐA THỨC TRÊN MỘT MIỀN KRULL

#### Mệnh đề 13 {#ac-vii-s1-prop-13 .statement}

*Cho $A$ là một miền Krull và $X_1, X_n, \ldots, X_n$ là các ẩn. Vành $A[X_1, \ldots, X_n]$ là một miền Krull.*

Lập luận bằng quy nạp theo $n$, chỉ cần chỉ ra rằng, nếu $X$ là một ẩn, thì $A[X]$ là một miền Krull. Gọi $K$ là trường phân thức của $A$. Trường phân thức của $A[X]$ là $K(X)$. Gọi $I$ là tập hợp các đa thức đơn nhất trong $K[X]$ bất khả quy trên $K$; với mọi $f \in I$, gọi $v_f$ là định giá trên $K(X)$ được xác định bởi $f$ (Chương VI, §3, no. 3, Ví dụ 4). Mặt khác, với mọi định giá cốt yếu $w$ của $A$, gọi $w$ là mở rộng của $w$ lên $K(X)$ được xác định bởi

$$
\bar{w}\left( \sum_j a_j X^j \right) = \inf_j (w(a_j))
$$

với $\sum_j a_j X^j \in K[X]$ (Chương VI, §10, no. 1, Bổ đề 1). Rõ ràng các $u$, và các $\bar{w}$ là rời rạc và được chuẩn hoá và, với mọi $u \in K[X]$, $v_f(u) = 0$ (tương ứng $\bar{w}(u) = 0$) trừ ra đối với một số hữu hạn định giá $v_f$ (tương ứng $\bar{w}$).

Do đó, để chứng minh mệnh đề, chỉ cần chỉ ra rằng $A[X]$ là giao của các vành của các định giá $v_f$ và $\bar{w}$. Mà giao của các vành của các định giá $v_f$ là $K[X]$. Mặt khác, với $\sum_j a_j X^j \in K[X]$, quan hệ $\bar{w}\left( \sum_j a_j X^j \right) \geq 0$ tương đương với " $w(a_j) \geq 0$ với mọi $j$"; do đó quan hệ " $\bar{w}\left( \sum_j a_j X^j \right) \geq 0$ với mọi định giá $\bar{w}'$" tương đương với " $w(a_j) \geq 0$ với mọi $j$ và mọi định giá cốt yếu $w$ của $A$." Điều này chứng minh mệnh đề của chúng ta.

#### Nhận xét {#ac-vii-s1-n9-rem-1 .statement}

Các định giá $v_f$ và $\bar{w}$ được đưa vào trong chứng minh của Mệnh đề 13 là các định giá cốt yếu của $A[X]$. Với chúng tôi, chỉ cần chỉ ra rằng, nếu $V$ là tập hợp các định giá $v_f$ ($f$ bất khả quy) và $\bar{w}$ (w cốt yếu), thì với mọi $v' \in V$, tồn tại một phần tử $g \in K(X)$ không thuộc $A[X]$ và sao cho $v''(g) \geq 0$ đối với mọi định giá $v'' \in V$ phân biệt với $v'$; điều này sẽ chứng minh rằng $V - \{v'\}$ không thỏa mãn (AK$_{II}$), và do đó kết luận sẽ suy ra từ no. 4, Hệ quả 2 của Mệnh đề 6. Trước hết giả sử rằng $v'$ có dạng $\bar{w}$: khi đó ta có thể lấy $g$ là một phần tử $b \in K$ sao cho $w(b) < 0, w'(b) \geq 0$ đối với các định giá cốt yếu $w'$ của $A$ phân biệt với $w$, vì khi ấy $v_f(b) = 0$ với mọi đa thức đơn khởi bất khả quy $f$ trong $K[X]$; sự tồn tại của một phần tử $b$ thỏa mãn các điều kiện trên suy ra từ no. 5, Mệnh đề 9. Thứ hai, giả sử rằng $v'$ có dạng $v_f$ với một đa thức đơn khởi bất khả quy $f \in K[X]$ bậc $m$; khi đó ta có thể lấy $g = a/f$ với $a \in A$. Thật vậy, $v_h(g) \geq 0$ đối với mọi đa thức đơn khởi bất khả quy $h \neq f$ trong $K[X]$; còn lại là chọn $a \in A$ sao cho, với mọi định giá cốt yếu $w$ của $A$, $w(a)$ ít nhất bằng cận dưới lớn nhất của các phần tử $w(c_i)$, trong đó các $c_i$ là các hệ số của $f$ ($1 \leq i \leq m$); mà sự tồn tại của một $a \in A$ như vậy suy ra từ (AK$_{III}$) và no. 5, Mệnh đề 9.

Ta cũng có thể nói (no. 6, Định lý 4) rằng các iđêan nguyên tố của $A[X]$ có chiều cao 1 là:
(1) các iđêan nguyên tố có dạng $pA[X]$, trong đó $p$ là một iđêan nguyên tố của $A$ có chiều cao 1;
(2) các iđêan nguyên tố có dạng $m \cap A[X]$, trong đó $m$ là một iđêan nguyên tố (tất yếu là chính) của $K[X]$.

Các iđêan loại sau được đặc trưng bởi tính chất là giao của chúng với $A$ thu về 0.

### 10. CÁC LỚP ƯỚC TRONG CÁC MIỀN KRULL

Cho $A$ là một miền Krull. Nhắc lại rằng nhóm các ước $D(A)$ của $A$ là nhóm giao hoán tự do sinh bởi tập $P(A)$ các phần tử cực biên của nó (no. 3, Định lý 2) và rằng $P(A)$ được đồng nhất với tập các iđêan nguyên tố của $A$ có chiều cao 1 (no. 6); với $p \in P(A)$ ta sẽ ký hiệu bởi $v_p$ định giá cốt yếu chuẩn hóa tương ứng với $p$ (no. 4); nhắc lại rằng vành của $v_p$ là $A_p$ (no. 4, Hệ quả 1 của Mệnh đề 6). Ta sẽ ký hiệu bởi $F(A)$ nhóm con của $D(A)$ gồm các ước chính và bởi $C(A) = D(A)/F(A)$ nhóm lớp ước của $A$ (no. 2).

#### Mệnh đề 14 {#ac-vii-s1-prop-14 .statement}

Cho $A$ là một miền Krull và $B$ là một miền Krull chứa $A$. Giả sử rằng điều kiện sau được thỏa mãn:

(PDE) Với mọi iđêan nguyên tố $\mathfrak{P}$ của $B$ có chiều cao 1, iđêan nguyên tố $\mathfrak{P} \cap A$ bằng không hoặc có chiều cao 1.

Với $p \in P(A)$ các $\mathfrak{P} \in P(B)$ sao cho $\mathfrak{P} \cap A = p$ là hữu hạn về số lượng; ta viết

$$
i(p) = \sum_{\mathfrak{P} \in P(B), \mathfrak{P} \cap A = p} e(\mathfrak{P}/p)\mathfrak{P},
$$

trong đó $e(\mathfrak{P}/\mathfrak{p})$ ký hiệu chỉ số *phân nhánh* của $v_{\mathfrak{p}}$ trên $v_{\mathfrak{p}}$ (Chương VI, § 8, no. 1). *Khi đó i xác định, bởi* tính tuyến tính, một *đồng cấu* tăng $i$ từ $D(A)$ vào $D(B)$, có các tính chất sau:

(a) *với mọi phần tử khác không x của trường phân thức của A*,

$$
i(\operatorname{div}_A(x)) = \operatorname{div}_B(x);
$$

(b) *với mọi D, D' trong D(A)*,

$$
i(\sup(D, D')) = \sup(i(D), i(D'));
$$

Cho $\mathfrak{p} \in P(A)$; xét một phần tử khác không $a$ của $\mathfrak{p}$; các $\mathfrak{P} \in P(B)$ chứa $a$ là hữu hạn về số lượng (no. 6, Định lý 4); *a fortiori* các $\mathfrak{P} \in P(B)$ sao cho $\mathfrak{P} \cap A = \mathfrak{p}$ là hữu hạn về số lượng.

Bây giờ ta chứng minh (a). Do tính cộng tính, có thể giả thiết rằng $x \in A^* = A - \{0\}$.

Theo định nghĩa, $\operatorname{div}_B(x) = \sum_{\mathfrak{P} \in P(B)} v_{\mathfrak{p}}(x) \cdot \mathfrak{P}$. Với mọi $\mathfrak{P} \in P(B)$ sao cho $v_{\mathfrak{p}}(x) > 0$, $\mathfrak{P} \cap A$ là khác không (vì $x \in \mathfrak{P}$) và do đó có chiều cao 1 theo (PDE); đặt $\mathfrak{p} = \mathfrak{P} \cap A$, theo định nghĩa của chỉ số phân nhánh, $v_{\mathfrak{p}}(x) = e(\mathfrak{P}/\mathfrak{p}) v_{\mathfrak{p}}(x)$ (vì $v_{\mathfrak{p}}$ và $v_{\mathfrak{P}}$ là chuẩn hóa). Vì $\operatorname{div}_A(x) = \sum_{\mathfrak{p} \in P(A)} v_{\mathfrak{p}}(x) \cdot \mathfrak{p}$, và $i(q) = 0$ với mọi $q \in P(A)$ không có dạng $\mathfrak{Q} \cap A$ trong đó $\mathfrak{Q} \in P(B)$, ta suy ra (a).

Để chứng minh (b) ta viết

$$
D = \sum_{\mathfrak{p} \in P(A)} n(\mathfrak{p}) \cdot \mathfrak{p} \quad \text{and} \quad D' = \sum_{\mathfrak{p} \in P(A)} n'(\mathfrak{p}) \cdot \mathfrak{p};
$$

hệ số của $\mathfrak{p}$ trong $\sup(D, D')$ là $\sup(n(\mathfrak{p}), n'(\mathfrak{p}))$. Cho $\mathfrak{P}$ là một phần tử của $P(B)$. Nếu $\mathfrak{P} \cap A = (0)$, các hệ số của $\mathfrak{P}$ trong $i(D)$ và $i(D')$ và do đó cả trong $\sup(i(D), i(D'))$ đều bằng không; vậy hệ số của $\mathfrak{P}$ trong $i(\sup(D, D'))$ bằng không. Nếu $\mathfrak{P} \cap A \neq (0)$, đó là một iđêan nguyên tố $\mathfrak{p}$ có chiều cao 1 (theo (PDE)); viết $e = e(\mathfrak{P}/\mathfrak{p})$, thì các hệ số của $\mathfrak{P}$ trong $i(D)$, $i(D')$ và $i(\sup(D, D'))$ lần lượt là $en(\mathfrak{p}), en'(\mathfrak{p})$ và $e \cdot \sup(n(\mathfrak{p}), n'(\mathfrak{p}))$; hệ số của $\mathfrak{P}$ trong $\sup(i(D), i(D'))$ là

$$
\sup(e \cdot n(\mathfrak{p}), e \cdot n'(\mathfrak{p})) = e \cdot \sup(n(\mathfrak{p}), n'(\mathfrak{p})).
$$

Điều này chứng minh (b).

Dưới các giả thiết của Mệnh đề 14, từ (a) suy ra rằng i xác định, bằng cách lấy thương, một đồng cấu $\bar{i}$, gọi là chính tắc, từ $C(A)$ đến $C(B)$, mà chúng tôi cũng sẽ đôi khi viết là $i$, do lạm dụng ký hiệu.

Điều kiện (PDE) được thỏa mãn trong hai trường hợp sau đây:

(1) B là nguyên trên A; trong trường hợp này, *để iđêan nguyên tố* $\mathfrak{P}$ của B *có chiều cao* 1, *điều kiện cần và đủ là* $\mathfrak{p} = \mathfrak{P} \cap A$ có chiều cao 1. Thật vậy, (0) là iđêan nguyên tố duy nhất của B nằm trên iđêan (0) của A (Chương V, § 2, no. 1, Hệ quả I của Mệnh đề 1); nếu $\mathfrak{P}$ có chiều cao 1, thì $\mathfrak{p} \neq 0$; nếu $\mathfrak{p}$ không có chiều cao 1, sẽ tồn tại một iđêan nguyên tố $\mathfrak{p}'$ của A phân biệt với (0) và $\mathfrak{p}$ và sao cho 0 ⊂ p' ⊂ p; nhưng khi đó, vì B là một miền nguyên và A là một miền nguyên đóng nguyên, sẽ tồn tại một iđêan nguyên tố $\mathfrak{p}'$ của B sao cho $\mathfrak{p}' \cap A = p'$ và $\mathfrak{p}' \subset \mathfrak{p}$ (Chương V, § 2, no. 4, Định lý 3), trái với giả thiết. Ngược lại, nếu p có chiều cao 1, thì không thể tồn tại iđêan nguyên tố nào $\mathfrak{p}'$ của B phân biệt với 0 và $\mathfrak{p}$ và sao cho $0 \subset \mathfrak{p}' \subset \mathfrak{p}$, nếu không thì $0 \subset \mathfrak{p}' \cap A \subset p$ và $\mathfrak{p}' \cap A$ sẽ phân biệt với 0 và p theo Chương V, § 2, no. 1, Hệ quả 1 của Mệnh đề 1.

(2) B là một A-môđun phẳng. Chính xác hơn:

#### Mệnh đề 15 {#ac-vii-s1-prop-15 .statement}

Cho A và B là các miền Krull sao cho B chứa A và là một A-môđun phẳng. Khi đó:
(a) điều kiện (PDE) của Mệnh đề 14 được thỏa mãn;
(b) với mọi iđêan phân thức $a \in A$, Ba là iđêan phân thức của B tương ứng với ước $i(\operatorname{div}_A(a))$.

Để chứng minh (a), giả sử tồn tại một iđêan nguyên tố $\mathfrak{p}$ của B có chiều cao 1 sao cho $\mathfrak{p} \cap A$ không phải là 0 cũng không có chiều cao 1. Lấy một phần tử $x \neq 0$ trong $\mathfrak{p} \cap A$. Các iđêan $p_i$ của A có chiều cao 1 mà chứa x chỉ có hữu hạn, và không iđêan nào chứa $\mathfrak{p} \cap A$; do đó tồn tại một phần tử y của $\mathfrak{p} \cap A$ sao cho $y \notin p_i$ với mọi $i$ (Chương II, § 2, no. 1, Mệnh đề 2). Khi đó $\operatorname{div}_A(x)$ và $\operatorname{div}_A(y)$ là các phần tử nguyên tố cùng nhau của nhóm có thứ tự P(A), vì thế $\sup(\operatorname{div}_A(x), \operatorname{div}_A(y)) = \operatorname{div}_A(x) + \operatorname{div}_A(y) = \operatorname{div}_A(xy)$; vì các iđêan $Ax \cap Ay$ và $Axy$ là divisoriel, ta suy ra $Ax \cap Ay = Axy$. Vì B là một A-môđun phẳng, $Bx \cap By = Bxy$ (Chương I, § 2, no. 6, Mệnh đề 6). Điều này kéo theo $\sup(v_{\mathfrak{p}}(x), v_{\mathfrak{p}}(y)) = v_{\mathfrak{p}}(xy) = v_{\mathfrak{p}}(x) + v_{\mathfrak{p}}(y)$, điều này mâu thuẫn với các bất đẳng thức $v_{\mathfrak{p}}(x) > 0, v_{\mathfrak{p}}(y) > 0$ (đúng vì x và y thuộc $\mathfrak{p}$). Vậy (a) được chứng minh bằng phản chứng.

Bây giờ ta chứng minh (b). Nếu $a$ là một iđêan divisoriel của A, thì nó là giao của hai iđêan chính phân thức (no. 5, Hệ quả 2 của Mệnh đề 9), chẳng hạn

$$
a = d^{-1}(Aa \cap Ab)
$$

trong đó $a, b,$ d thuộc $A^*$; vì B phẳng trên A, $Ba = d^{-1}(Ba \cap Bb)$ (Chương I, § 2, no. 6, Mệnh đề 6), điều này cho thấy Ba là divisoriel. Điều này cũng cho thấy rằng $\operatorname{div}_B(Ba) = \sup(\operatorname{div}_B(a), \operatorname{div}_B(b)) - \operatorname{div}_B(d)$; dùng Mệnh đề 14 (a) và (b), ta thấy rằng

$$
\begin{align*}
\operatorname{div}_B(Ba) &= \sup(i(\operatorname{div}_A(a)), i(\operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) \\
&= i(\sup(\operatorname{div}_A(a), \operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) \\
&= i(\operatorname{div}_A(Aa \cap Ab)) - i(\operatorname{div}_A(d)) \\
&= i(\operatorname{div}_A(d^{-1}(Aa \cap Ab))) = i(\operatorname{div}_A(a)).
\end{align*}
$$

#### Hệ quả {#ac-vii-s1-n10-cor-1 .statement}

Cho A là một miền Krull địa phương và B là một vành định giá rời rạc sao cho B trội hơn A và là một A-môđun phẳng. Khi đó A là một trường hoặc một vành định giá rời rạc.

Gọi $\mathfrak{m}$ là iđêan cực đại của B. Theo (PDE), $\mathfrak{m} \cap A$ bằng không hoặc có chiều cao 1. Vì theo giả thiết nó là iđêan cực đại của A, mệnh đề của ta suy ra từ Mệnh đề 11 của no. 7.

#### Nhận xét {#ac-vii-s1-n10-rem-1 .statement}

Trong trường hợp thứ nhất của hai trường hợp trên, ánh xạ $i : D(A) \to D(B)$ là đơn ánh: vì các phần tử của $P(B)$ lập thành một cơ sở của $D(B)$ và hai iđêan phân biệt của $P(A)$ không thể là các vết trên A của cùng một iđêan của $P(B)$, nên chỉ cần kiểm tra rằng $i(p) \neq 0$ với mọi $p \in P(A)$; mà điều này suy ra từ Chương V, § 2, no. 1, Định lý 1. Tương tự, ta cũng thấy rằng, nếu B là một A-môđun phẳng trung thành, thì $i$ là đơn ánh (Chương II, § 2, no. 5, Hệ quả 4 của Mệnh đề 11).

Trong phần tiếp theo, chúng tôi đề nghị nghiên cứu đồng cấu chính tắc $\tilde{i}$ từ $C(A)$ đến $C(B)$ đối với một số cặp có thứ tự các miền Krull A, B.

#### Mệnh đề 16 {#ac-vii-s1-prop-16 .statement}

Cho A là một vành Zariski sao cho hoàn thành của nó $\hat{A}$ là một miền Krull. Khi đó A là một miền Krull và đồng cấu chính tắc $\tilde{i}$ từ $C(A)$ đến $C(\hat{A})$ (được xác định vì A là một A-môđun phẳng; xem Chương III, § 3, no. 4, Định lý 3) là đơn ánh.

Vì A là một miền nguyên và $A \subset \hat{A}$, A là một miền nguyên. Gọi L là trường phân thức của $\hat{A}$ và K $\subset$ L là trường phân thức của A. Vì $A = \hat{A} \cap K$ (Chương III, § 3, no. 5, Hệ quả 4 của Mệnh đề 9), A là một miền Krull (no. 3, Ví dụ 4). Việc $\tilde{i} : C(A) \to C(\hat{A})$ là đơn ánh suy ra từ Mệnh đề 15 (b) và sự kiện rằng, nếu $b \hat{A}$ là chính, thì b là chính (Chương III, § 3, no. 5, Hệ quả 3 của Mệnh đề 9).

Bây giờ cho A là một miền Krull và S là một tập con nhân của A không chứa 0. Nhóm $D(A)$ (tương ứng $D(S^{-1}A)$) là nhóm giao hoán tự do có cơ sở là tập hợp các $\operatorname{div}(p)$ (tương ứng các $\operatorname{div}(S^{-1}p)$), trong đó p chạy qua tập hợp các iđêan nguyên tố của A có chiều cao 1 (tương ứng tập hợp các iđêan nguyên tố của A có chiều cao 1 sao cho $p \cap S = \varnothing$) (no. 4, Mệnh đề 6) và, nếu $p \cap S = \varnothing$, thì $i(\operatorname{div}(p)) = \operatorname{div}(S^{-1}p)$. Do đó $D(S^{-1}A)$ được đồng nhất với thừa số trực tiếp của $D(A)$ sinh bởi các phần tử $\operatorname{div}(p)$ sao cho $p \cap S = \varnothing$ và có phần bù là nhóm con giao hoán tự do của $D(A)$ có cơ sở là tập hợp các $\operatorname{div}(p)$ sao cho $p \cap S \neq \varnothing$; chúng ta sẽ ký hiệu phần bù này bởi G. Vì $i : D(A) \to D(S^{-1}A)$ là toàn ánh, nên $i : C(A) \to C(S^{-1}A)$ cũng vậy; và:

$$
G/(G \cap F(A)) = (G + F(A))/F(A) = \operatorname{Ker}(\tilde{i});
$$

vì nếu một phần tử của $D(S^{-1}A)$ bằng $\operatorname{div}_{S^{-1}A}(x/s)$, với $x \in A$ và $s \in S$, thì nó là ảnh qua $i$ của ước chính $\operatorname{div}_A(x)$ (Mệnh đề 14).

Bây giờ giả sử rằng S được sinh bởi một họ các phần tử $(p_i)_{i \in I}$ của A sao cho các iđêan chính $Ap_i$ đều là nguyên tố. Khi đó, nếu $p$ là một iđêan nguyên tố của A có chiều cao 1 sao cho $p \cap S \neq \varnothing$, thì $p$ chứa một tích các lũy thừa của các $p_i$, và do đó chứa một trong các $p_i$, giả sử là $p_\alpha$; vì $Ap_\alpha$ khác không và là nguyên tố và $p$ có chiều cao 1, suy ra $p = Ap_\alpha$. Vậy, theo ký hiệu ở trên, $G \subset F(A)$ và (5) cho thấy hạt nhân của $\bar{i}$ bằng không. Do đó chúng ta đã chứng minh kết quả sau đây:

#### Mệnh đề 17 {#ac-vii-s1-prop-17 .statement}

*Cho $A$ là một miền Krull và $S$ là một tập con nhân của $A$ không chứa $0$. Khi đó đồng cấu chính tắc $\bar{i}$ từ $C(A)$ tới $C(S^{-1}A)$ là toàn ánh. Nếu thêm nữa $S$ được sinh bởi một họ các phần tử $p_i$ sao cho các iđêan chính $Ap_i$ đều là nguyên tố, thì $\bar{i}$ là song ánh.*

Như một áp dụng thứ hai của công thức (5), xét tình huống sau: cho $R$ là một miền Krull; lấy $A$ là vành đa thức $A = R[X]$ (no. 9, Mệnh đề 13) và $S$ là tập hợp $R - (0)$ các đa thức hằng khác không của $A$. Các iđêan nguyên tố $p$ của $A$ có chiều cao 1 sao cho $p \cap S \neq \varnothing$ là những iđêan có dạng $p_0A$, trong đó $p_0$ là một iđêan nguyên tố của $R$ có chiều cao 1 (no. 9, *Nhận xét*). Do đó, theo ký hiệu đã đưa vào ở trên, $G$ được đồng nhất với $D(R)$ bằng cách đồng nhất $\mathrm{div}_A(p_0A)$ với $\mathrm{div}_R(p_0)$. Mặt khác $G \cap F(A)$ được đồng nhất với $F(R)$: thật vậy, nếu một iđêan $a$ của $R$ sinh ra một iđêan chính $a_0A = f(X)A$ trong $A = R[X]$, thì $f(0) \in a_0A$ vì $a_0A$ là một iđêan phân bậc của vành $A$ (được phân bậc theo bậc thông thường của các đa thức) và do đó $f(0) \in a$; hơn nữa, với $a \in a_0A$, ta có $a = f(X)g(X)$ với $g(X) \in R$, do đó, khi so sánh các hạng tử bậc 0, $a = f(0)g(0)$; suy ra $a$ là iđêan chính của $R$ sinh bởi $f(0)$. Cuối cùng, ký hiệu $K$ là trường phân thức của $R$, $S^{-1}A$ được đồng nhất với vành đa thức $K[X]$, là một miền iđêan chính; do đó $C(S^{-1}A) = (0)$. Vậy, theo (5), $C(A) = \mathrm{Ker}(\bar{i})$ được đồng nhất với $C(R)$ và chúng ta đã chứng minh kết quả sau:

#### Mệnh đề 18 {#ac-vii-s1-prop-18 .statement}

*Cho $R$ là một miền Krull và $A$ là vành đa thức $R[X]$. Đồng cấu chính tắc từ $C(R)$ vào $C(R[X])$ là song ánh.*

### Bài tập {#ac-vii-s1-exercises}

Xem [bài tập của § 1](exercises/s1/).
