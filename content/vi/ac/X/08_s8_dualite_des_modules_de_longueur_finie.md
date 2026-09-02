---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 8
section_title: Dualité des modules de longueur finie
lang: vi
source: ac-x-fr
pdf_pages: 0104-0123, 0172-0174
extraction: ocr
subsections:
    - "no": 1
      title: Modules injectifs indécomposables
      page: 0
      pdf_page: 104
    - "no": 2
      title: Structure des modules injectifs indécomposables
      page: 0
      pdf_page: 105
    - "no": 3
      title: Dualité de Matlis
      page: 110
      pdf_page: 109
    - "no": 4
      title: Dualité des modules de longueur finie
      page: 114
      pdf_page: 113
    - "no": 5
      title: Foncteurs dualisants
      page: 115
      pdf_page: 114
    - "no": 6
      title: Changement d’anneaux ; dualité de Macaulay
      page: 119
      pdf_page: 118
    - "no": 7
      title: Dualité des modules d’extensions et des produits de torsion
      page: 0
      pdf_page: 119
statements: 31
exercises: 10
content_sha256: a5815fe78bda7489723bd12f34c6f96bf25a792382006be0570b4a597d3139fd
translated_from: content/en-mt/ac/X/08_s8_dualite_des_modules_de_longueur_finie.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 51e31816b68f96681968fe09fb5cad0e0228d14a3641b0e6b586d1cd7ea00744
translation_model: gpt-5.4
translation_run: translate-vi-be263a49
glossary_version: 34
glossary_terms_sha256: 3b85e7d2cffb62713acc7d48ca09ef12d335bc3e12019232a07b7e995183a24d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. ĐỐI NGẪU CỦA CÁC MÔĐUN CÓ ĐỘ DÀI HỮU HẠN

### 1. Các môđun đơn ánh không phân tích được

Cho $A$ là một vành. Quan hệ "$I$ là một lớp các $A$-môđun đơn ánh không phân tích được" là xác định tập (A, X, p. 21, Hệ quả 1); ta ký hiệu bởi $\mathscr{J}(A)$ tập hợp các lớp các $A$-môđun đơn ánh không phân tích được.

#### Mệnh đề 1 {#ac-x-s8-prop-1 .statement}

Cho $A$ là một vành Noether. Với mọi iđêan nguyên tố $\mathfrak{p}$ của $A$, gọi $e_{\mathfrak{p}} : A/\mathfrak{p} \to I(\mathfrak{p})$ là một bao đơn ánh của $A/\mathfrak{p}$ (A, X, § 1, No. 9).

a) Các $A$-môđun $I(\mathfrak{p})$ là không phân tích được.

b) Cho $I$ là một $A$-môđun đơn ánh không phân tích được; tập hợp $\mathrm{Ass}(I)$ chỉ gồm một phần tử duy nhất.

c) Ánh xạ $\mathfrak{p} \mapsto \mathrm{cl}(I(\mathfrak{p}))$ là một song ánh từ $\mathrm{Spec}(A)$ lên $\mathscr{J}(A)$. Song ánh ngược gắn với một phần tử $I$ của $\mathscr{J}(A)$ phần tử duy nhất của $\mathrm{Ass}(I)$.

Cho $\mathfrak{p} \in \mathrm{Spec}(A)$; ta hãy chứng minh rằng môđun $I(\mathfrak{p})$ là không phân tích được. Theo A, X, p. 21, Hệ quả 2, chỉ cần chứng minh rằng nếu $a$ và $b$ là các iđêan của $A$ chứa $\mathfrak{p}$ và phân biệt với $\mathfrak{p}$, thì iđêan $a \cap b$ phân biệt với $\mathfrak{p}$; mà nếu $a$ là một phần tử của $a - \mathfrak{p}$ và $b$ là một phần tử của $b - \mathfrak{p}$, thì tích $ab$ thuộc $(a \cap b) - \mathfrak{p}$.

Cho $I$ là một $A$-môđun đơn ánh không phân tích được, và cho $\mathfrak{p}, \mathfrak{q}$ là các phần tử của $\mathrm{Ass}(I)$. Khi đó $I$ chứa một môđun con $M$ đẳng cấu với $A/\mathfrak{p}$ và một môđun con $N$ đẳng cấu với $A/\mathfrak{q}$. Ta có $M \cap N \neq 0$ (A, X, p. 21, Mệnh đề 14); với mọi phần tử khác không $x$ của $M \cap N$, ta có $\mathfrak{p} = \mathrm{Ann} x = \mathfrak{q}$. Vì $\mathrm{Ass}(I)$ không rỗng (IV, § 1, No. 1, Hệ quả 1 của Mệnh đề 2), nên nó chỉ gồm một phần tử duy nhất $\mathfrak{p}(I)$.

Như vậy ta đã xác định hai ánh xạ $\mathfrak{p} \mapsto \mathrm{cl}(I(\mathfrak{p}))$ từ $\mathrm{Spec}(A)$ vào $\mathscr{J}(A)$ và $I \mapsto \mathfrak{p}(I)$ từ $\mathscr{J}(A)$ vào $\mathrm{Spec}(A)$; hãy chứng minh rằng hai ánh xạ này là hai song ánh nghịch đảo của nhau. Cho $\mathfrak{p} \in \mathrm{Spec}(A)$; khi đó $\mathfrak{p}$ thuộc $\mathrm{Ass}(I(\mathfrak{p}))$, và vì thế là phần tử duy nhất của $\mathrm{Ass}(I(\mathfrak{p}))$. Cho $I$ là một $A$-môđun đơn ánh không phân tích được, và $\mathfrak{p}$ là phần tử duy nhất của $\mathrm{Ass}(I)$; khi đó $I$ là một bao đơn ánh của $A/\mathfrak{p}$ (A, X, p. 21, Mệnh đề 14). Điều này hoàn tất chứng minh của mệnh đề.

#### Nhận xét 1 {#ac-x-s8-n1-rem-1 .statement}

Cho $I$ là một $A$-môđun đơn ánh không phân tích được, và cho $\mathfrak{p}$ là phần tử duy nhất của $\mathrm{Ass}(I)$; theo Mệnh đề 1, $I$ chứa một môđun con đẳng cấu với $A/\mathfrak{p}$ mà nó là bao đơn ánh. Nói chung một môđun con như thế không duy nhất, như thấy được khi lấy $A = \mathbf{Z}$, $\mathfrak{p} = 0$, $I = \mathbf{Q}$.

Với mỗi iđêan nguyên tố $\mathfrak{p}$ của $A$, ta hãy chọn như trên một bao đơn ánh $(I(\mathfrak{p}), e_{\mathfrak{p}})$ của $A/\mathfrak{p}$. Theo A, X, p. 22, Định lý 3, ta có:

#### Định lý 1 {#ac-x-s8-thm-1 .statement}

Cho $A$ là một vành Noether. Với mọi $A$-môđun đơn ánh $I$, tồn tại một và chỉ một họ các lực lượng $(a_{\mathfrak{p}})_{\mathfrak{p} \in \mathrm{Spec}(A)}$ sao cho $I$ đẳng cấu với $\bigoplus_{\mathfrak{p}} I(\mathfrak{p})^{(a_{\mathfrak{p}})}$.

#### Nhận xét 2 {#ac-x-s8-n1-rem-2 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun, $e : M \to I$ là một bao đơn ánh của $M$. *Tập hợp Ass(M) bằng Ass(I)*: thật vậy, bao hàm $Ass(M) \subset Ass(I)$ là hiển nhiên. Mặt khác, nếu $p$ là một phần tử của $Ass(I)$, thì $I$ chứa một môđun con $N$ đẳng cấu với $A/p$; vì $A$-môđun $e^{-1}(N)$ là khác không, nên ta có $Ass(e^{-1}(N)) = \{p\}$ (IV, § 1, No. 1, Mệnh đề 1). Điều này chứng minh rằng $p$ liên kết với $e^{-1}(N)$, do đó với $M$, do đó mệnh đề của ta.

Giữ lại các ký hiệu của định lý, và giả sử thêm rằng $Ass(M)$ là hữu hạn. Với mọi $q \in Ass(M)$, gọi $Q_q$ là giao với $M$ của $\bigoplus_{p \in Ass(M) - \{q\}} I(p)^{(a_p)}$. Khi đó $(Q_q)_{q \in Ass(M)}$ *là một phân tích nguyên sơ tối giản của 0 trong M* (IV, § 2, No. 3, Def. 3). Thật vậy $\cap Q_q = 0$; vì $M/Q_q$ được đồng nhất với một môđun con khác không của $I(q)^{(a_q)}$, ta có $Ass(M/Q_q) = \{q\}$, và chỉ cần áp dụng Mệnh đề 4 của *loc. cit*.

#### Ví dụ {#ac-x-s8-n1-exa-1 .statement}

Cho $A$ là một miền iđêan chính, và gọi $K$ là trường phân thức của nó. Các $A$-môđun nội xạ là các $A$-môđun chia được (A, X, p. 17, Hệ quả 2). $A$-môđun $K$ là một bao nội xạ của $A$ (A, X, p. 20, Ví dụ 1). Gọi $p$ là một phần tử cực đại của $A$, và $p$ là iđêan (cực đại) $Ap$; gọi $e : A/p \longrightarrow K/A_p$ là đồng cấu ánh xạ lớp của một phần tử $a \in A$ vào lớp của $a/p$. Ta sẽ chứng minh rằng $(K/A_p, e)$ *là một bao nội xạ của $A/p$*. Đồng cấu $e$ là đơn ánh. $A$-môđun $K/A_p$ là một thương của một môđun chia được, nên là chia được. Gọi $x$ là một phần tử khác không của $K/A_p$; nó là lớp của một phần tử $a/p^n$ của $K$, với $a \in A - \{0\}$ và $n \geqslant 1$ (A, VII, p. 10, định lý 2). Khi đó $p^{n-1}x = e(a)$, nên $e^{-1}(Ax) \neq 0$, điều này chứng minh mệnh đề của ta.

Khi đó từ định lý 1 suy ra rằng *mọi $A$-môđun chia được đều là một tổng trực tiếp của các $A$-môđun đẳng cấu với $K$ hoặc với $K/A_p$ với $p$ là một iđêan cực đại (chính) của $A$*.

### 2. Cấu trúc của các môđun nội xạ không phân tích được

#### Bổ đề 1 {#ac-x-s8-lem-1 .statement}

Cho $A$ là một vành, $a$ là một iđêan của $A$, và $I$ là một $A$-môđun. Với mọi số nguyên $n \geqslant 0$, gọi $I_n$ là môđun con của $I$ gồm các phần tử bị triệt tiêu bởi $a^n$.

a) *Giả sử rằng $A$-môđun $I$ là nội xạ. Khi đó $A/a^n$-môđun $I_n$ là nội xạ với mọi $n \geqslant 0$*.

b) *Giả sử rằng vành $A$ là Noether, và rằng với mọi $n \geqslant 0$ thì $A/a^n$-môđun $I_n$ là đơn ánh. Khi đó hợp của các $I_n$ là một A-môđun đơn ánh*.

a) $A/a^n$-môđun $I_n$ đẳng cấu với $\operatorname{Hom}_A(A/a^n, I)$, môđun này là đơn ánh (A, X, p. 18, Mệnh đề 11).

b) Gọi $J$ là hợp của các $I_n$, $b$ là một iđêan của $A$ và $f : b \to J$ là một A-đồng cấu. Theo (A, X, p. 16, Mệnh đề 10), cần chứng minh rằng tồn tại một phần tử $x$ của $J$ sao cho ta có $f(b) = bx$ với mọi $b \in b$. Vì $b$ là kiểu hữu hạn, tồn tại một số nguyên $n$ sao cho ta có $f(b) \subset I_n$, nghĩa là $f(a^n b) = 0$. Theo Hệ quả 2 của Mệnh đề 1 của III, § 3, No. 1, tồn tại một số nguyên $m \geqslant n$ sao cho $a^m \cap b \subset a^n b$, do đó $f(a^m \cap b) = 0$. Khi đó $f$ cảm sinh một ánh xạ tuyến tính $A/a^m$ của $b/(a^m \cap b)$ vào $I_m$; vì $A/a^m$-môđun $I_m$ là đơn ánh, tồn tại một phần tử $x$ của $I_m$ sao cho ta có $f(b) = bx$ với mọi $b \in b$, do đó b).

Cho $\alpha$ là một iđêan của $A$; trong phần sau, ta quy ước đặt $\alpha^n = A$ với mọi số nguyên $n \leq 0$. Cho $E$ là một $A$-môđun. Với mỗi $n \in \mathbf{Z}$, ký hiệu $E_n$ là môđun con của $E$ gồm các phần tử bị triệt tiêu bởi $\alpha^n$; gọi $\mathrm{gr}^\alpha(E)$ là $A$-môđun phân bậc kiểu $\mathbf{Z}$ sao cho $\mathrm{gr}^\alpha(E)_m = E_{-m+1}/E_{-m}$ với mọi số nguyên $m$. Môđun $\mathrm{gr}^\alpha(E)_m$ bằng không với $m \geq 1$, và $\mathrm{gr}^\alpha(E)_0$ được đồng nhất với $E_1$. Ký hiệu $\mathrm{gr}(A)$ là vành phân bậc liên kết với $A$ đối với lọc $\alpha$-adic: ta có $\mathrm{gr}(A)_n = \alpha^n/\alpha^{n+1}$ với mọi $n \in \mathbf{Z}$. Cho $n$ và $m$ là các số nguyên. Chuyển qua các thương từ ánh xạ song tuyến tính $(a, x) \mapsto ax$ của $\alpha^n \times E_{-m+1}$ vào $E_{-m-n+1}$, ta suy ra được một ánh xạ $A/\alpha$-song tuyến tính

$$
\alpha_{n,m} : \mathrm{gr}(A)_n \times \mathrm{gr}^\alpha(E)_m \longrightarrow \mathrm{gr}^\alpha(E)_{n+m},
$$

ánh xạ này xác định trên $\mathrm{gr}^\alpha(E)$ một cấu trúc $\mathrm{gr}(A)$-môđun phân bậc. Với mỗi $n \in \mathbf{Z}$, từ ánh xạ $A/\alpha$-song tuyến tính $\alpha_{n,-n} : \mathrm{gr}(A)_n \times \mathrm{gr}^\alpha(E)_{-n} \longrightarrow E_1$ ta suy ra được một ánh xạ $A/\alpha$-tuyến tính $\beta_{E,n} : \mathrm{gr}^\alpha(E)_{-n} \longrightarrow \mathrm{Hom}_{A/\alpha}(\mathrm{gr}(A)_n, E_1)$; các ánh xạ $\beta_{E,n}$ là các thành phần của một đồng cấu các $A/\alpha$-môđun phân bậc, gọi là *chính tắc*,

$$
\beta_E : \mathrm{gr}^\alpha(E) \longrightarrow \mathrm{Hom}_{\mathrm{gr}_{A/\alpha}}(\mathrm{gr}(A), E_1).
$$

Với $a \in \mathrm{gr}(A)$, $x \in \mathrm{gr}^\alpha(E)$, theo định nghĩa $\beta_E(x)(a)$ là thành phần trong $\mathrm{gr}^\alpha(E)_0 = E_1$ của phần tử $ax$ của $\mathrm{gr}^\alpha(E)$. Suy ra rằng $\beta_E$ là $\mathrm{gr}(A)$-tuyến tính khi ta trang bị cho $\mathrm{Hom}_{\mathrm{gr}_{A/\alpha}}(\mathrm{gr}(A), E_1)$ cấu trúc $\mathrm{gr}(A)$-môđun được xác định bởi công thức $(bf)(a) = f(ab)$ với $a, b$ trong $\mathrm{gr}(A)$ và $f$ trong $\mathrm{Hom}_{\mathrm{gr}_{A/\alpha}}(\mathrm{gr}(A), E_1)$.

#### Mệnh đề 2 {#ac-x-s8-prop-2 .statement}

*Cho $A$ là một vành Noether, $\alpha$ là một iđêan của $A$, $E$ là một $A$-môđun và $M$ là một môđun con-$A$ của $E$ bị triệt tiêu bởi $\alpha$. Các điều kiện sau là tương đương:*
    (i) *$E$ là một bao đơn ánh của $M$* ;
    (ii) *$E_1$ là một bao đơn ánh của $M$ như $A/\alpha$-môđun, môđun $E$ là hợp của các $E_n$ và ánh xạ chính tắc $\beta_E$ là song ánh*.

Giả sử điều kiện (i) được thỏa mãn. $E_1$ là một $A/\alpha$-môđun đơn ánh (Bổ đề 1, a)), và chứa $M$; vì mọi môđun con-$\Lambda/\alpha$ của $E_1$ đều là một môđun con-$A$ của $E$, nên $E_1$ là một bao đơn ánh của $M$ như $\Lambda/\alpha$-môđun. Theo Bổ đề 1, hợp của các $E_n$ là một môđun con-$A$ đơn ánh của $E$ chứa $M$, do đó bằng $E$. Vì $E$ là đơn ánh, với mọi $n \geq 0$ ta có một dãy khớp

$$
0 \to \mathrm{Hom}_A(A/\alpha^n, E) \longrightarrow \mathrm{Hom}_A(A/\alpha^{n+1}, E) \longrightarrow \mathrm{Hom}_A(\alpha^n/\alpha^{n+1}, E) \to 0;
$$

vì $\mathrm{Hom}_A(A/\alpha^m, E)$ được đồng nhất với $E_m$ với mọi $m$ và đơn ánh chính tắc của $\mathrm{Hom}_A(\alpha^n/\alpha^{n+1}, E_1)$ vào $\mathrm{Hom}_A(\alpha^n/\alpha^{n+1}, E)$ là song ánh, suy ra đồng cấu chính tắc $\beta_E$ là song ánh, do đó có (ii).

Giả sử (ii) được thỏa mãn. Gọi $e : M \to I$ là một bao đơn ánh của $M$. Vì $I$ là đơn ánh, tồn tại một ánh xạ tuyến tính $A$-tuyến tính $\varphi : E \to I$ kéo dài $e$. Nhưng $\varphi$ ánh xạ $E_n$ vào $I_n$ với mọi $n$, do đó cảm sinh các đồng cấu gr^{a}(\varphi) : \operatorname{gr}^{a}(E) \to \operatorname{gr}^{a}(I) \text{ và } \varphi_1 : E_1 \to I_1 \text{ làm cho biểu đồ giao hoán}

$$
\begin{array}{ccc}
\operatorname{gr}^{a}(E) & \xrightarrow{\beta_E} & \operatorname{Homgr}_{A/\alpha}(\operatorname{gr}(A), E_1) \\
\downarrow \operatorname{gr}^{a}(\varphi) & & \downarrow \operatorname{Homgr}(1, \varphi_1) \\
\operatorname{gr}^{a}(I) & \xrightarrow{\beta_I} & \operatorname{Homgr}_{A/\alpha}(\operatorname{gr}(A), I_1)
\end{array}
$$

Vì $E_1$ và $I_1$ là các bao đơn ánh của $A/\alpha$-môđun $M$, nên đồng cấu $\varphi_1$ là song ánh; vì $\beta_E$ và $\beta_I$ là song ánh, suy ra $\operatorname{gr}^{a}(\varphi)$ là song ánh. Điều này kéo theo, bằng quy nạp theo $n$, rằng $\varphi$ cảm sinh một song ánh từ $E_n$ lên $I_n$ với mọi $n \geq 1$; do đó $\varphi$ là song ánh, điều này kéo theo (i).

#### Bổ đề 2 {#ac-x-s8-lem-2 .statement}

*Cho $A$ là một vành, $\alpha$ là một iđêan hữu hạn sinh của $A$, và $M$ là một $A$-môđun mà mỗi phần tử đều bị triệt tiêu bởi một lũy thừa của $\alpha$. Ký hiệu $\widehat{A}$ là bổ sung tách của $A$ đối với tôpô $\alpha$-adic.*

a) *Tồn tại trên $M$ một cấu trúc $\widehat{A}$-môđun duy nhất, mở rộng cấu trúc $A$-môđun đã cho.*

b) *Các môđun con-$\widehat{A}$ của $M$ là các môđun con-$A$ của nó, và ta có $\operatorname{Hom}_A(M, P) = \operatorname{Hom}_{\widehat{A}}(M, P)$ với mọi $\widehat{A}$-môđun $P$.

a) Ta đồng nhất $\widehat{A}$ với giới hạn xạ ảnh của các vành $A/\alpha^n$, và trang bị cho $M$ tôpô rời rạc. Cho $a = (a_n)$ là một phần tử của $\widehat{A}$, và $x$ là một phần tử của $M$. Vì $x$ bị triệt tiêu bởi một lũy thừa của $\alpha$, dãy $(a_n x)$ là dừng; gọi $ax$ là giới hạn của nó. Ánh xạ $(a, x) \mapsto ax$ xác định trên $M$ một cấu trúc $\widehat{A}$-môđun mở rộng cấu trúc $A$-môđun đã cho.

Ngược lại, giả sử đã cho một cấu trúc như vậy trên $M$; cho $a = (a_n)$ là một phần tử của $\widehat{A}$, $x$ là một phần tử của $M$ và $m$ là một số nguyên sao cho $\alpha^m x = 0$. Với mọi số nguyên $n$, $a - a_n$ thuộc $\alpha^n$, mà bằng $\alpha^n \widehat{A}$ (III, § 2, n° 12, cor. 2 of prop. 16); do đó ta có $ax = a_n x$ với $n \geq m$, do đó có mệnh đề về tính duy nhất.

b) Suy ra từ điều trước đó rằng ta có $Ax = \widehat{A}x$ với mọi $x \in M$; do đó các môđun con theo $\widehat{A}$ của $M$ chính là các môđun con theo $A$ của nó. Cuối cùng, cho $u$ là một đồng cấu $A$-tuyến tính từ $M$ vào một $\widehat{A}$-môđun $P$. Gọi $a = (a_n)$ là một phần tử của $\widehat{A}$, $x$ là một phần tử của $M$, và $m$ là một số nguyên sao cho $\alpha^m x = 0$; ta có $\alpha^m u(x) = 0$. Vì $a - a_m$ thuộc $\alpha^m \widehat{A}$, ta có

$$
u(ax) = u(a_m x) = a_m u(x) = au(x),
$$

nên $u$ là $\widehat{A}$-tuyến tính.

#### Mệnh đề 3 {#ac-x-s8-prop-3 .statement}

*Cho $A$ là một vành Noether, $p$ là một iđêan nguyên tố của $A$, và $e : A/p \to I$ là một bao nội xạ của $A$-môđun $A/p$. Với mỗi số nguyên $n \geq 0$, ký hiệu $I_n$ là môđun con của $I$ gồm các phần tử bị triệt tiêu bởi $p^n$.*

a) $A$-môđun $I$ là hợp của các $I_n$. Đơn ánh $\Lambda / \mathfrak{p} \to I_1$ mở rộng thành một đẳng cấu từ $\kappa(\mathfrak{p})$ lên $I_1$; hãy đồng nhất $\kappa(\mathfrak{p})$ với $I_1$ qua đẳng cấu này. Với mỗi số nguyên $n \geqslant 0$, cấu trúc $\Lambda / \mathfrak{p}$-môđun của $I_{n+1}/I_n$ thu được bằng cách hạn chế vô hướng từ một cấu trúc không gian vectơ $\kappa(\mathfrak{p})$ duy nhất; đồng cấu chính tắc $\beta_{I,-n}: I_{n+1}/I_n \longrightarrow \mathrm{Hom}_{\Lambda/\mathfrak{p}}(\mathfrak{p}^n/\mathfrak{p}^{n+1}, \kappa(\mathfrak{p}))$ là một đẳng cấu của các không gian vectơ $\kappa(\mathfrak{p})$ hữu hạn chiều.

b) Tồn tại một cấu trúc $\widehat{A_p}$-môđun duy nhất trên $I$ cảm sinh cấu trúc $A$-môđun của nó. Đồng cấu chính tắc $\widehat{A_p} \longrightarrow \mathrm{End}_A(I)$ là song ánh.

Theo A, X, p. 20, Ví dụ 1, $A/\mathfrak{p}$-môđun $\kappa(\mathfrak{p})$ là một bao nội xạ của $A/\mathfrak{p}$. Do đó suy ra từ Mệnh đề 2 rằng $I_1$ được đồng nhất với $\kappa(\mathfrak{p})$, rằng $I$ là hợp của các $I_m$, và rằng với mỗi số nguyên $n \geqslant 0$, $\beta_{I,-n}$ là một đẳng cấu của các $A/\mathfrak{p}$-môđun. Với mọi phần tử khác không $a$ của $A/\mathfrak{p}$, phép vị tự tỉ số $a$ là khả nghịch trong $\mathrm{Hom}_{A/\mathfrak{p}}(\mathfrak{p}^n/\mathfrak{p}^{n+1}, \kappa(\mathfrak{p}))$, nên cũng khả nghịch trong $I_{n+1}/I_n$, điều này hoàn tất chứng minh của a).

Cho $s \in A - \mathfrak{p}$. Vì phép vị tự $s_{A/\mathfrak{p}}$ là đơn ánh, vết của $\mathrm{Ker}\, s_I$ trên $A/\mathfrak{p}$ bằng không, do đó suy ra phép vị tự $s_I$ là đơn ánh. Khi đó $s_I$ là một môđun con hạng tử trực tiếp của $I$ (A, X, p. 19, Hệ quả 4), nên bằng $I$ vì $I$ không phân tích được (No. 1, Mệnh đề 1), thành thử phép vị tự $s_I$ là song ánh. Vì vậy tồn tại duy nhất một cấu trúc $A_p$-môđun trên $I$ cảm sinh cấu trúc $A$-môđun của nó; cấu trúc này được mở rộng duy nhất thành một cấu trúc $\widehat{A_p}$-môđun (Bổ đề 2).

Với mỗi số nguyên $n$, từ đồng cấu vành chính tắc $\Lambda_p \longrightarrow \mathrm{End}_A(I)$ ta suy ra một ánh xạ $A$-tuyến tính $\alpha_n : A_p/\mathfrak{p}^n A_p \longrightarrow \mathrm{Hom}_A(I_n, I)$. Xét biểu đồ giao hoán có các hàng khớp

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & \mathfrak{p}^n A_p/\mathfrak{p}^{n+1} A_p & \longrightarrow & A_p/\mathfrak{p}^{n+1} A_p & \longrightarrow & A_p/\mathfrak{p}^n A_p & \longrightarrow & 0 \\
& & \downarrow \alpha'_{n+1} & & \downarrow \alpha_{n+1} & & \downarrow \alpha_n & & \\
0 & \longrightarrow & \mathrm{Hom}_A(I_{n+1}/I_n, I_1) & \longrightarrow & \mathrm{Hom}_A(I_{n+1}, I) & \longrightarrow & \mathrm{Hom}_A(I_n, I) & \longrightarrow & 0
\end{array}
$$

trong đó $\alpha'_{n+1}$ là đồng cấu cảm sinh bởi $\alpha_{n+1}$. Xét ánh xạ song tuyến tính chính tắc trên $\kappa(\mathfrak{p})$

$$
\alpha_{n,-n} : \mathfrak{p}^n A_p/\mathfrak{p}^{n+1} A_p \times I_{n+1}/I_n \longrightarrow I_1
$$

(công thức (1)). Ánh xạ tuyến tính $I_{n+1}/I_n \longrightarrow \mathrm{Hom}_{\kappa(\mathfrak{p})}(\mathfrak{p}^n A_p/\mathfrak{p}^{n+1} A_p, I_1)$ liên kết với nó ở bên trái được đồng nhất với $\beta_{I,-n}$, và ánh xạ liên kết với nó ở bên phải là $\alpha'_{n+1}$. Vì $\beta_{I,-n}$ là song ánh theo a), điều tương tự cũng đúng với $\alpha'_{n+1}$; khi đó từ biểu đồ trên, bằng quy nạp theo $n$, suy ra $\alpha_n$ là một đẳng cấu với mọi $n$. Vì $I$ là hợp của các $I_n$, ánh xạ chính tắc $\mathrm{End}_A(I) \to \varprojlim \mathrm{Hom}_A(I_n, I)$ là song ánh; do đó đồng cấu vành $\widehat{A_p} \to \mathrm{End}_A(I)$, được đồng nhất với giới hạn xạ ảnh của các ánh xạ $\alpha_n$, là song ánh.

#### Nhận xét {#ac-x-s8-n2-rem-1 .statement}

Suy ra từ chứng minh trước rằng linh hóa tử của $I_n$ trong $\widehat{A_p}$ (resp. trong $A_p$) là $\mathfrak{p}^n \widehat{A_p}$ (resp. $\mathfrak{p}^n A_p$). Do đó linh hóa tử của A-môđun $I_n$ là ảnh ngược trong $A$ của iđêan $\mathfrak{p}^n A_p$, đôi khi được ký hiệu bởi $\mathfrak{p}^{(n)}$ và được gọi là lũy thừa ký hiệu thứ $n$ của iđêan nguyên tố $\mathfrak{p}$.

#### Hệ quả {#ac-x-s8-n2-cor-1 .statement}

Cho J là một A-môđun đơn ánh sao cho Ass_A(J) = {p}.

a) Ánh xạ chính tắc J → A_p ⊗_A J là song ánh.

b) Ký hiệu E là A/p-môđun Hom_A(A/p, J). Trên E tồn tại duy nhất một cấu trúc không gian vectơ trên κ(p) kéo dài cấu trúc A/p-môđun của nó; A-môđun J đẳng cấu với I([E:κ(p)]).

Thật vậy, J đẳng cấu với một A-môđun I^{(c)}, trong đó c là một lực lượng thích hợp (No. 1, th. 1). Hệ quả suy ra từ mệnh đề khi J = I, và trường hợp tổng quát được suy ra từ đó ngay lập tức.

### 3. Đối ngẫu Matlis

Trong No. này, ta giả sử rằng vành A là địa phương Noether.

#### Định nghĩa {#ac-x-s8-n3-def-1 .statement}

Ta nói rằng một A-môđun I là một Matlis A-môđun nếu nó là đơn ánh, nếu m_A là iđêan nguyên tố liên kết duy nhất của nó, và nếu không gian vectơ trên κ_A Hom_A(κ_A, I) có chiều bằng 1.

Cho e : κ_A → I là một bao đơn ánh của κ_A (A, X, p. 20, th. 2). A-môđun I là một môđun Matlis, và mọi môđun Matlis đều đẳng cấu với I (No. 2, cor. of prop. 3). Nếu A là một vành định giá rời rạc, với trường phân thức K, thì A-môđun K/A là một môđun Matlis (No. 1, example). Nếu A là một vành địa phương Artin, thì A-môđun A là một môđun Matlis khi và chỉ khi A là một vành Gorenstein (§ 3, No. 7, lemma 1).

Cho I là một Matlis A-môđun. Với mọi số nguyên n ≥ 0, ký hiệu I_n là môđun con-A của I gồm các phần tử bị triệt tiêu bởi m_A^n. Theo mệnh đề 2 của No. 2, A-môđun I là hợp của các I_n, A-môđun I_1 có độ dài 1 (nghĩa là đẳng cấu với κ_A) và A-môđun I là một bao đơn ánh của I_1; hơn nữa, đồng cấu chính tắc của các gr(A)-môđun phân bậc

$$
\beta : \operatorname{gr}^{m_A}(I) \longrightarrow \operatorname{Hom}_{\kappa_A}(\operatorname{gr}(A), I_1)
$$

là một đẳng cấu. Theo mệnh đề 3 của No. 2, cấu trúc A-môđun của I kéo dài thành một cấu trúc $\widehat{A}$-môđun duy nhất, và đồng cấu chính tắc $\widehat{A} \to \operatorname{End}_A(I)$ là song ánh.

#### Bổ đề 3 {#ac-x-s8-lem-3 .statement}

Cho I là một Matlis A-môđun. Khi đó:

a) I là một Matlis $\widehat{A}$-môđun;
b) A-môđun I là Artin và là một đối sinh (A, X, p. 18, def. 3).

Vì A-môđun I là đơn ánh, nên A/m_A^n-môđun I_n là đơn ánh với mỗi n (No. 2, lemma 1, a)). Vì I_n là tập các phần tử của I bị triệt tiêu bởi m_A^n, nên $\widehat{A}$-môđun I là đơn ánh (lemma 1, b)). Nó không phân tích được trên $\widehat{A}$ vì nó đã như vậy trên A; do nó chứa môđun con-$\widehat{A}$ I_1 đẳng cấu với $\kappa_A$, ta có $m_{\widehat{A}} \in \operatorname{Ass}_{\widehat{A}}(I)$, nên $\operatorname{Ass}_{\widehat{A}}(I) = \{ m_{\widehat{A}} \}$ (prop. 1), do đó suy ra a).

Bây giờ ta chứng minh rằng I là Artin. Với mỗi môđun con-A M của I, ta gắn cho nó iđêan phân bậc $a_M$ của gr(A) được định nghĩa như sau: một phần tử của gr(A)_n thuộc về $(\mathfrak{a}_M)_n$ nếu nó bị triệt tiêu bởi mọi dạng tuyến tính $\beta(x)$, trong đó $x$ chạy qua $((M \cap I_{n+1}) + I_n)/I_n$. Cho $M$ và $N$ là các môđun con của $I$ sao cho $N \subset M$; khi đó $\mathfrak{a}_M \subset \mathfrak{a}_N$. Giả sử $\mathfrak{a}_M = \mathfrak{a}_N$; ta có $(M \cap I_{n+1}) + I_n = (N \cap I_{n+1}) + I_n$ với mọi $n$ vì $\beta$ là một đẳng cấu. Bằng quy nạp theo $n$ ta suy ra từ đó rằng $M \cap I_{n+1} = N \cap I_{n+1}$ với mọi $n$, do đó cuối cùng $M = N$.

Như vậy, cho $M_0 \supset M_1 \supset \ldots \supset M_n \supset \ldots$ là một dãy giảm các môđun con-A của $I$; dãy tăng $\mathfrak{a}_{M_0} \subset \mathfrak{a}_{M_1} \subset \ldots$ là dừng, vì $\mathrm{gr}(A)$ là một $\kappa_A$-đại số sinh hữu hạn. Do đó dãy $(M_i)_{i \geq 0}$ là dừng, điều này kéo theo rằng A-môđun $I$ là Artin. Cuối cùng, A-môđun $I$ là một đối sinh theo A, X, p. 18, prop. 12.

Cho $M$ là một A-môđun. Nhắc lại (A, VIII, § 4, No. 6) rằng đế của $M$ là tổng của các môđun con đơn của $M$, tức là tập các phần tử của $M$ bị triệt tiêu bởi $m_A$; nó là một không gian vectơ trên $\kappa_A$, đẳng cấu chính tắc với $\mathrm{Hom}_A(\kappa_A, M)$.

#### Bổ đề 4 {#ac-x-s8-lem-4 .statement}

*Cho I là một Matlis A-môđun và M là một $\Lambda$-môđun. Các điều kiện sau là tương đương :*

(i) $M$ là Artin;
(ii) mọi phần tử của $M$ đều bị triệt tiêu bởi một lũy thừa của $m_A$, và đế của $M$ có số chiều hữu hạn trên $\kappa_\Lambda$;
(iii) tồn tại một số nguyên $n \geq 0$ và một ánh xạ A-tuyến tính đơn ánh từ $M$ vào $I^n$.

*Khi các điều kiện này được thỏa mãn, mọi bao nội xạ của $M$ đều đẳng cấu với $I^s$, trong đó $s$ là số chiều trên $\kappa_A$ của đế của $M$.*

(iii) $\Rightarrow$ (i): điều này hiển nhiên vì A-môđun $I$ là Artin (Bổ đề 3).

(i) $\Rightarrow$ (ii): giả sử rằng $M$ là Artin. Lấy $x \in M$; dãy giảm các môđun con $m_A^n x$ của $M$ là dừng. Gọi $n$ là một số nguyên sao cho $m_A^{n+1} x = m_A^n x$; bổ đề Nakayama suy ra rằng $m_A^n x = 0$. Mặt khác, đế của $M$ là Artin như một A-môđun, do đó cũng là Artin như một $\kappa_A$-không gian vectơ, nghĩa là nó có số chiều hữu hạn.

(ii) $\Rightarrow$ (iii): giả sử điều kiện (ii) được thỏa mãn; gọi $e : M \to J$ là một bao nội xạ của $M$. Ta có $\mathrm{Ass}(M) \subset \{m_A\}$, do đó $\mathrm{Ass}(J) \subset \{m_A\}$ (No. 1, Nhận xét 2), và $J$ đẳng cấu với $I^{(c)}$ với một lực lượng $c$ (No. 1, Định lý 1). Gọi $x$ là một phần tử khác không của $J$ bị triệt tiêu bởi $m_A$; vì A-môđun $Ax$ là đơn và giao của nó với $e(M)$ không phải chỉ là 0, nên $x$ thuộc $e(M)$. Vậy $e$ gây ra một đẳng cấu từ đế của $M$ lên đế của $J$; do đó đế của $M$ có số chiều bằng $c$, điều này chứng minh (iii) cũng như khẳng định cuối cùng.

#### Bổ đề 5 {#ac-x-s8-lem-5 .statement}

*Mọi $\widehat{\Lambda}$-môđun Artin đều là Artin như một $\Lambda$-môđun.*

Cho $M$ là một $\widehat{\Lambda}$-môđun Artin; mọi phần tử của $M$ đều bị triệt tiêu bởi một lũy thừa của $m_{\widehat{\Lambda}}$, nên cũng bị triệt tiêu bởi một lũy thừa của $m_A$. Theo Bổ đề 2 của No. 2, các môđun con-A của $M$ chính là các môđun con-$\widehat{\Lambda}$ của nó, do đó $M$ là Artin như một A-môđun.

Bây giờ ta cố định một Matlis $A$-môđun I. Với mọi $A$-môđun $M$, ta ký hiệu bởi $D_A(M)$ là $\widehat{A}$-môđun
$$
D_A(M) = \operatorname{Hom}_A(M, I)
$$
$\widehat{A}$-môđun $D_A(A)$ được đồng nhất một cách chính tắc với $I$, $\widehat{A}$-môđun $D_A(I)$ với $\widehat{A}$ ($n^\circ 2$, mệnh đề 3), và $\widehat{A}$-môđun $D_A(\kappa_A)$ với $I_1$ (*loc. cit.*).

Với mọi ánh xạ tuyến tính $A$ $f : M \to N$, ta sẽ ký hiệu bởi
$$
D_A(f) : D_A(N) \to D_A(M)
$$
ánh xạ tuyến tính $\widehat{A}$ $\operatorname{Hom}_A(f, 1_I)$. Vì $A$-môđun $I$ là đơn ánh, dãy $(D_A(g), D_A(f))$ là khớp với mọi dãy khớp $(f, g)$ các ánh xạ tuyến tính $A$.

Ta sẽ áp dụng các định nghĩa này cho vành $\widehat{A}$ được trang bị môđun Matlis I (bổ đề 3, a)) ; với mọi $\widehat{A}$-môđun $P$, $D_{\widehat{A}}(P)$ do đó là môđun con $\widehat{A}$ $\operatorname{Hom}_{\widehat{A}}(P, I)$ của $D_A(P)$. Nói rằng $P$ là Artin như một $A$-môđun hay như một $\widehat{A}$-môđun là như nhau (bổ đề 5) ; nếu đúng như vậy, ta có $D_{\widehat{A}}(P) = D_A(P)$ (*loc. cit.*).

Cho $M$ là một $A$-môđun. Với $m \in M$, ánh xạ $f \mapsto f(m)$ từ $D_A(M)$ vào $I$ là $\widehat{A}$-tuyến tính ; ta ký hiệu nó bởi $\alpha_M(m)$. Như vậy ta xác định được một đồng cấu $A$-tuyến tính
$$
\alpha_M : M \longrightarrow D_{\widehat{A}}(D_A(M))
$$
Ta ký hiệu bởi $\widehat{\alpha}_M : \widehat{A} \otimes_A M \longrightarrow D_{\widehat{A}}(D_A(M))$ ánh xạ tuyến tính $\widehat{A}$ suy ra từ $\alpha_M$.

#### Định lý 2 {#ac-x-s8-thm-2 .statement}

*Cho $M$ là một $A$-môđun.*

a) *Để $M$ là Artin, điều kiện cần và đủ là $\widehat{A}$-môđun $D_A(M)$ là hữu hạn kiểu. Khi đó, đồng cấu $\alpha_M$ là song ánh.*

b) *Để $M$ là kiểu hữu hạn, điều kiện cần và đủ là $D_A(M)$ là Artin (như một $A$-môđun hoặc như một $\widehat{A}$-môđun). Trong trường hợp này đồng cấu $\widehat{\alpha}_M$ là một đẳng cấu.*

c) *Để $M$ có độ dài hữu hạn, điều kiện cần và đủ là $D_A(M)$ có độ dài hữu hạn (như một $A$-môđun hoặc như một $\widehat{A}$-môđun). Trong trường hợp này $\alpha_M$ là một đẳng cấu từ $M$ lên $D_A(D_A(M))$, và ta có $\operatorname{long}_A(D_A(M)) = \operatorname{long}_A(M)$.*

Trước hết ta sẽ chứng minh rằng đồng cấu $\alpha_M$ là đơn ánh với mọi $A$-môđun $M$. Gọi $m$ là một phần tử khác không của $M$; linh hóa tử của nó được chứa trong $m_A$. Do đó tồn tại một $A$-đồng cấu toàn ánh của $Am$ lên $\kappa_A$, và vì thế một đồng cấu khác không của $Am$ vào $I$. Vì $I$ là nội xạ, đồng cấu này kéo dài thành một đồng cấu $f : M \to I$ sao cho $f(m) \neq 0$. Điều này chứng minh tính đơn ánh của $\alpha_M$.

Giả sử $A$-môđun $M$ là Artin. Theo bổ đề 4, tồn tại một số nguyên $r$ và một ánh xạ tuyến tính $A$-đơn ánh $f : M \to I^r$. Khi đó đồng cấu $D_A(f) : D_A(I^r) \to D_A(M)$ là toàn ánh; vì $D_A(I^r)$ được đồng nhất với $\widehat{A}^r$, điều này chứng minh rằng $\widehat{A}$-môđun $D_A(M)$ là kiểu hữu hạn. Tương tự, nếu $M$ là kiểu hữu hạn, thì tồn tại một số nguyên $n$ và một đồng cấu toàn ánh $u : A^n \to M$; đồng cấu $D_A(u) : D_A(M) \to I^n$ là đơn ánh, do đó $D_A(M)$ là Artin (như một $A$-môđun hoặc như một $\widehat{A}$-môđun).

Giả sử $M$ là Artin. Tồn tại một số nguyên $r$ và một ánh xạ tuyến tính $A$-đơn ánh $f : M \to I^r$; vì $I$ là Artin (bổ đề 3), nên $A$-môđun $\operatorname{Coker}(f)$ cũng vậy, và ta có thể tìm được một số nguyên $s$ và một dãy khớp các $A$-môđun

$$
0 \to M \xrightarrow{f} I^r \xrightarrow{g} I^s .
$$

Từ đó suy ra một biểu đồ giao hoán với các hàng khớp

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & M & \xrightarrow{f} & I^r & \xrightarrow{g} & I^s \\
& & \downarrow{\alpha_M} & & \downarrow{\alpha_{I^r}} & & \downarrow{\alpha_{I^s}} \\
0 & \to & D_{\widehat{A}}(D_A(M)) & \xrightarrow{D_{\widehat{A}}(D_A(f))} & D_{\widehat{A}}(D_A(I^r)) & \xrightarrow{D_{\widehat{A}}(D_A(g))} & D_{\widehat{A}}(D_A(I^s)) .
\end{array}
$$

$\widehat{A}$-môđun $D_{\widehat{A}}(D_A(I))$ được đồng nhất với $I$ và $\alpha_I$ với ánh xạ đồng nhất; do đó $\alpha_{I^r}$ và $\alpha_{I^s}$ là song ánh, và tương tự $\alpha_M$ cũng vậy (A, X, p. 7, Hệ quả 3).

Nếu A-môđun $M$ sinh hữu hạn, tồn tại các số nguyên $m$ và $n$ và một dãy khớp các A-môđun

$$
A^m \longrightarrow A^n \longrightarrow M \to 0 ;
$$

từ đó suy ra một biểu đồ giao hoán với các hàng khớp

$$
\begin{array}{ccccccccc}
\widehat{A}^m & \longrightarrow & \widehat{A}^n & \longrightarrow & \widehat{A} \otimes_A M & \longrightarrow & 0 \\
\downarrow{\widehat{\alpha}_{A^m}} & & \downarrow{\widehat{\alpha}_{A^n}} & & \downarrow{\widehat{\alpha}_M} & & \\
\widehat{A}^m & \longrightarrow & \widehat{A}^n & \longrightarrow & D_A(D_A(M)) & \to & 0 .
\end{array}
$$

Vì $\widehat{\alpha}_A$ bằng $1_{\widehat{A}}$, suy ra $\widehat{\alpha}_M$ là một đẳng cấu.

Còn phải chứng minh đẳng thức $\operatorname{long}_A(M) = \operatorname{long}_A(D_A(M))$ khi $M$ có độ dài hữu hạn. Ta có thể giả sử $M \neq 0$; khi đó tồn tại một dãy khớp

$$
0 \to \kappa_A \longrightarrow M \longrightarrow N \to 0 ,
$$

do đó suy ra một dãy khớp

$$
0 \to D_A(N) \longrightarrow D_A(M) \longrightarrow D_A(\kappa_A) \to 0 .
$$

Ta có $\operatorname{long}_A(M) = \operatorname{long}_A(N) + 1$ và

$$
\operatorname{long}_A(D_A(M)) = \operatorname{long}_A(D_A(N)) + \operatorname{long}_A(D_A(\kappa_A)) = \operatorname{long}_A(D_A(N)) + 1 ;
$$

kết luận bằng quy nạp theo số nguyên $\operatorname{long}_A(M)$.

#### Nhận xét {#ac-x-s8-n3-rem-1 .statement}

Giả sử vành $A$ là Artin. Ta có $\operatorname{long}_A(I) = \operatorname{long}_A(D_A(A)) = \operatorname{long}(A)$ (Định lý 2, c)). Cho $M$ là một A-môđun sinh hữu hạn; nó thừa nhận một bao nội xạ đẳng cấu với $I^s$, trong đó $s$ là chiều của đế của $M$ (Bổ đề 4). Do đó ta có $\operatorname{long}_A(M) \leq s \operatorname{long}(A)$; để có đẳng thức, điều kiện cần và đủ là $M$ nội xạ. Đặc biệt, để A-môđun $A$ là nội xạ, điều kiện cần và đủ là đế của nó có chiều 1; như vậy ta thu được lại Bổ đề 1 của § 3, No. 7.

### 4. Đối ngẫu của các môđun có độ dài hữu hạn

Cho $A$ là một vành Noether; ký hiệu $\Omega$ là tập hợp các iđêan cực đại của nó. Mở rộng định nghĩa đã cho ở số trước, ta sẽ nói rằng một A-môđun $J$ là một A-môđun Matlis nếu nó nội xạ, nếu các iđêan nguyên tố liên kết của nó là các iđêan cực đại của $A$, và nếu với mọi iđêan cực đại $m$ của $A$ thì không gian vectơ $A/m$ $\operatorname{Hom}_A(A/m, J)$ có chiều 1. Với mỗi $m \in \Omega$, hãy chọn một bao nội xạ $\kappa(m) \to I(m)$ của A-môđun $\kappa(m)$; A-môđun $\bigoplus_{m \in \Omega} I(m)$ là một môđun Matlis, và mọi A-môđun Matlis đều đẳng cấu với nó (No. 1, Định lý 1).

Nhắc lại (VIII, § 1, No. 5) rằng người ta ký hiệu bởi $Z_0(A)$ $\mathbf{Z}$-môđun $\mathbf{Z}^{(\Omega)}$ và bởi $\varepsilon : Z_0(A) \to \mathbf{Z}$ dạng tuyến tính ánh xạ mỗi phần tử của cơ sở $\Omega$ thành 1. Nếu $M$ là một $A$-môđun có độ dài hữu hạn, thì $A_m$-môđun $M_m$ có độ dài hữu hạn với mọi $m \in \Omega$, và bằng không trừ ra với một số hữu hạn iđêan $m \in \Omega$. Ta đặt

$$
z_0(M) = \sum_{m \in \Omega} \operatorname{long}_{A_m}(M_m)[m] \text{ trong } Z_0(A) ;
$$

ta có $\operatorname{long}_A(M) = \varepsilon(z_0(M))$ (*loc. cit.*, ví dụ 3). Ngược lại, một $A$-môđun $N$ sao cho $\operatorname{long}_{A_m}(N_m)$ là hữu hạn với mọi $m \in \Omega$, và bằng không ngoài một tập con hữu hạn $I$ của $\Omega$, thì có độ dài hữu hạn: thật vậy, $N$ đẳng cấu với một môđun con của $\bigoplus_{m \in I} N_m$ (II, § 3, No. 3, hệ quả 2 của định lý 1), và ta có $\operatorname{long}_{A_m}(N_m) = \operatorname{long}_A(N_m)$ vì mọi $A_m$-môđun đơn đều đẳng cấu với $\kappa(m)$, do đó đơn như một $A$-môđun.

Cho $J$ là một $A$-môđun Matlis. Với mọi $A$-môđun $M$, ta sẽ ký hiệu bởi $D_A(M)$, hoặc đơn giản bởi $D(M)$, $A$-môđun $\operatorname{Hom}_A(M, J)$. Cho $\alpha_M$ là đồng cấu từ $M$ vào $D(D(M))$ được xác định bởi $\alpha_M(m)(f) = f(m)$ với $m \in M,\ f \in D(M)$.

#### Mệnh đề 4 {#ac-x-s8-prop-4 .statement}

Điều kiện cần và đủ để A-môđun M có độ dài hữu hạn là D(M) có độ dài hữu hạn. Khi đó ta có $z_0(D(M)) = z_0(M)$, $\operatorname{long}_A(M) = \operatorname{long}_A D(M)$, $\operatorname{Ann}_A(M) = \operatorname{Ann}_A(D(M))$, và ánh xạ A-tuyến tính $\alpha_M$ là song ánh.

Với mọi $m \in \Omega$, $A_m$-môđun $D(M)_m$ được đồng nhất với $\operatorname{Hom}_{A_m}(M_m, J_m)$ (II, § 2, No. 7, mệnh đề 19); khi đó mệnh đề đầu tiên của mệnh đề suy ra từ định lý 2, c) và từ đặc trưng hóa của các môđun có độ dài hữu hạn đã cho ở trên. Từ đây giả sử M có độ dài hữu hạn; ta có $\operatorname{long}_{A_m}(D(M)_m) = \operatorname{long}_{A_m}(M_m)$ với mọi $m \in \Omega$ (*loc. cit.*), do đó $z_0(D(M)) = z_0(M)$ và $\operatorname{long}_A(D(M)) = \operatorname{long}_A(M)$. Hơn nữa ánh xạ $(\alpha_M)_m : M_m \to D(D(M))_m$ được đồng nhất với đồng cấu chính tắc $\alpha_{M_m}$, là song ánh (*loc. cit.*); do đó $\alpha_M$ là song ánh.

Với mọi $a \in A$ ta có $D(a_M) = a_{D(M)}$ và do đó $\operatorname{Ann}_A(M) \subset \operatorname{Ann}_A(D(M))$. Áp dụng điều này cho A-môđun D(M), ta suy ra bao hàm đối, do đó có đẳng thức $\operatorname{Ann}_A(M) = \operatorname{Ann}_A(D(M))$.

#### Ví dụ {#ac-x-s8-n4-exa-1 .statement}

Cho A là một miền iđêan chính, K là trường phân thức của nó. *A-môđun K/A là một môđun Matlis*: thật vậy, ánh xạ chính tắc từ K/A vào $\prod_{m \in \Omega} K/A_m$ cảm sinh một đẳng cấu từ K/A lên $\bigoplus_{m \in \Omega} K/A_m$ (A, VII, p. 10, đl. 2); khi đó mệnh đề suy ra từ No. 1, ví dụ 1. Hơn nữa, trong A, VII, § 4, No. 9, ta đã chứng minh rằng ánh xạ $\alpha_M$ là song ánh đối với mọi A-môđun M có độ dài hữu hạn khi vành A là chính.

### 5. Các hàm tử đối ngẫu hóa

Trong số này, cho $A$ là một vành địa phương Noether cố định. Giả sử cho
a) với mọi $A$-môđun $M$ có độ dài hữu hạn, một $A$-môđun $T(M)$ ;
b) với mọi ánh xạ A-tuyến tính $f : M \to N$ giữa các $A$-môđun có độ dài hữu hạn, một ánh xạ A-tuyến tính $T(f) : T(N) \to T(M)$,
sao cho các điều kiện sau được thỏa mãn:
FD 1) Các ánh xạ $f \mapsto T(f)$ là A-tuyến tính.
FD 2) Với mọi $A$-môđun $M$ có độ dài hữu hạn, ta có $T(1_M) = 1_{T(M)}$.
FD 3) Với mọi biểu đồ $M \xrightarrow{f} N \xrightarrow{g} P$ gồm các $A$-môđun có độ dài hữu hạn và các ánh xạ A-tuyến tính, ta có $T(g \circ f) = T(f) \circ T(g)$.
FD 4) Với mọi dãy khớp $M' \xrightarrow{u} M \xrightarrow{v} M''$ gồm các $A$-môđun có độ dài hữu hạn, dãy $T(M'') \xrightarrow{T(v)} T(M) \xrightarrow{T(u)} T(M')$ là khớp.
FD 5) $A$-môđun $T(\kappa_A)$ có độ dài 1.

Từ FD 1) và FD 2), suy ra $T(a_M) = a T(1_M) = a 1_{T(M)} = a_{T(M)}$ với mọi $a \in A$. Lấy $M = \{0\}$, ta được $0_{T(M)} = 1_{T(M)}$, do đó $T(\{0\}) = \{0\}$. Từ điều này và từ FD 4) suy ra rằng với mọi ánh xạ tuyến tính đơn ánh (tương ứng, toàn ánh) giữa các $A$-môđun có độ dài hữu hạn, ánh xạ $T(f)$ là toàn ánh (tương ứng, đơn ánh).

Cho $M$ là một $A$-môđun có độ dài hữu hạn. Khi đó $T(M)$ có độ dài hữu hạn và ta có $\operatorname{long}_A(T(M)) = \operatorname{long}_A(M)$: điều này thực ra suy ra từ FD 4) và FD 5) và từ việc mọi môđun có độ dài hữu hạn đều nhận một chuỗi hợp thành mà các thương của nó đẳng cấu với $\kappa_A$.

Cho $M$ là một $A$-môđun có độ dài hữu hạn, và $(e_\lambda)_{\lambda \in L}$ là một họ trực giao các phép chiếu của $M$; theo FD 3), $(T(e_\lambda))_{\lambda \in L}$ là một họ trực giao các phép chiếu của $T(M)$. Bởi vậy, nếu $M$ là tổng trực tiếp của một họ các môđun con $(M_\lambda)_{\lambda \in L}$, và nếu $p_\lambda$ ký hiệu phép chiếu của $M$ lên $M_\lambda$, thì đồng cấu
$$
\sum_{\lambda \in L} T(p_\lambda) : \bigoplus_{\lambda \in L} T(M_\lambda) \longrightarrow T(M)
$$
là một đẳng cấu.

#### Ví dụ 1 {#ac-x-s8-n5-exa-1 .statement}

Cho $J$ là một $A$-môđun Matlis. Đặt $T(M) = \operatorname{Hom}_A(M, J)$ với mọi $A$-môđun $M$ có độ dài hữu hạn và $T(f) = \operatorname{Hom}_A(f, 1_J)$ với mọi ánh xạ A-tuyến tính $f$ giữa các $A$-môđun có độ dài hữu hạn. Khi đó các điều kiện FD 1) đến FD 5) được thỏa mãn. Ta sẽ thấy dưới đây (đl. 3) rằng mọi phép dựng thỏa mãn các điều kiện FD 1) đến FD 5) đều thu được theo cách này.

#### Ví dụ 2 {#ac-x-s8-n5-exa-2 .statement}

Cho $C$ là một phức nội xạ của các $A$-môđun và $d$ là một số nguyên sao cho $H^i(\operatorname{Homgr}_A(\kappa_A, C))$ bằng không với $i \neq d$ và có độ dài 1 với $i = d$. Với mọi $A$-môđun $M$ có độ dài hữu hạn, ta có $H^i(\operatorname{Homgr}_A(M, C)) = 0$ với $i \neq d$; thực vậy, hãy lập luận bằng quy nạp theo độ dài của $M$, được giả sử $> 0$; tồn tại một dãy khớp các $A$-môđun $0 \to \kappa_A \to M \to N \to 0$, dãy này suy ra một dãy khớp các phức
$$
0 \to \operatorname{Homgr}_A(N, C) \longrightarrow \operatorname{Homgr}_A(M, C) \longrightarrow \operatorname{Homgr}_A(\kappa_A, C) \longrightarrow 0
$$
và kết luận suy ra từ giả thiết quy nạp áp dụng cho $N$.

Đặt $T(M) = H^d(\operatorname{Homgr}_A(M, C))$ với mọi $A$-môđun $M$ có độ dài hữu hạn, và $T(f) = H^d(\operatorname{Homgr}_A(f, 1_C))$ với mọi ánh xạ tuyến tính $A$-tuyến tính $f$ giữa các $A$-môđun có độ dài hữu hạn; các điều kiện FD 1) đến FD 5) được thỏa mãn.

#### Ví dụ 3 {#ac-x-s8-n5-exa-3 .statement}

Cho $\Omega$ là một $A$-môđun và $d$ là một số nguyên $\geqslant 0$ sao cho $\operatorname{Ext}_A^i(\kappa_A, \Omega)$ bằng không với $i \neq d$ và có độ dài 1 với $i = d$. Đặt $T(M) = \operatorname{Ext}_A^d(M, \Omega)$ với mọi $A$-môđun $M$ có độ dài hữu hạn và $T(f) = \operatorname{Ext}_A^d(f, 1_\Omega)$ với mọi ánh xạ tuyến tính $A$-tuyến tính $f$ giữa các $A$-môđun có độ dài hữu hạn. Khi đó $\operatorname{Ext}_A^i(M, \Omega) = 0$ với mọi $A$-môđun $M$ có độ dài hữu hạn và mọi $i \neq d$, và các điều kiện FD 1) đến FD 5) được thỏa mãn: thực vậy, chỉ cần áp dụng ví dụ trước trong trường hợp $C$ là phân giải nội xạ chính tắc của $\Omega$.

#### Ví dụ 4 {#ac-x-s8-n5-exa-4 .statement}

Nếu $A$ là một vành Gorenstein, chẳng hạn một vành chính quy, thì có thể áp dụng Ví dụ 3 bằng cách lấy $\Omega = A$ và $d = \dim(A)$ (§ 3, No. 7, Mệnh đề 11).

Với mọi số nguyên $n \geqslant 0$, đặt $I_n = T(A/\mathfrak{m}_A^n)$. Với $m \geqslant n$, ký hiệu $p_{mn} : A/\mathfrak{m}_A^m \longrightarrow A/\mathfrak{m}_A^n$ là toàn cấu chính tắc và $i_{mn} : T(A/\mathfrak{m}_A^n) \longrightarrow T(A/\mathfrak{m}_A^m)$ là ánh xạ $A$-tuyến tính $T(p_{mn})$. Nó là đơn ánh theo FD 4), và ta có $i_{mn} \circ i_{np} = i_{mp}$ với $m \geqslant n \geqslant p$ theo FD 3). Gọi $I = \varprojlim T(A/\mathfrak{m}_A^n)$ là $A$-môđun giới hạn quy nạp của hệ $((I_n), (i_{mn}))$. Với $n \geqslant 0$, ánh xạ chính tắc $I_n \to I$ là đơn ánh; ta đồng nhất $I_n$ với ảnh của nó trong $I$, để $I$ là hợp tăng của các $I_n$.

Cho M là một A-môđun có độ dài hữu hạn, và n là một số nguyên $\geqslant 0$ sao cho $m_A^n M = 0$. Với $x \in M$, ký hiệu $\varphi_{M,x}^n$ là ánh xạ A-tuyến tính từ $A/m_A^n$ vào M gửi lớp của 1 tới x. Ánh xạ $T(\varphi_{M,x}^n) : T(M) \to I_n$ là A-tuyến tính, và ta có $T(\varphi_{M,a x}^n) = a T(\varphi_{M,x}^n)$ với $a \in A$ theo FD 1). Do đó ánh xạ $(x, u) \mapsto T(\varphi_{M,x}^n)(u)$ từ $M \times T(M)$ vào I là A-song tuyến tính. Nó không phụ thuộc vào lựa chọn số nguyên n: thật vậy, với mọi số nguyên $q \geqslant n$ và mọi phần tử x của M, ta có $\varphi_{M,x}^q = \varphi_{M,x}^n \circ p_{q n}$, do đó theo FD 3) $T(\varphi_{M,x}^q) = i_{q n} \circ T(\varphi_{M,x}^n)$. Ta suy ra một ánh xạ A-tuyến tính
$$
\theta_M : T(M) \longrightarrow \operatorname{Hom}_A(M, I)
$$
thỏa mãn $\theta_M(u)(x) = T(\varphi_{M,x})(u)$ với $u \in T(M),\ x \in M$.

#### Định lý 3 {#ac-x-s8-thm-3 .statement}

a) A-môđun I là một môđun Matlis. Với mọi số nguyên $m \geqslant 0$, $I_m$ là A-môđun con của I gồm các phần tử bị triệt tiêu bởi $m_A^m$.

b) Với mọi A-môđun M có độ dài hữu hạn, ánh xạ A-tuyến tính $\theta_M : T(M) \to \operatorname{Hom}_A(M, I)$ là song ánh.

c) Với mọi ánh xạ A-tuyến tính $f : M \to N$ giữa các A-môđun có độ dài hữu hạn, ta có $\theta_M \circ T(f) = \operatorname{Hom}_A(f, 1_I) \circ \theta_N$.

Ta chứng minh c). Cho n là một số nguyên và M, N là các A-môđun có độ dài hữu hạn bị triệt tiêu bởi $m_A^n$. Cho $f : M \to N$ là một ánh xạ A-tuyến tính. Với $u$ trong $T(N)$ và x trong M, theo FD 3) ta có
$$
\begin{align*}
\theta_M(T(f)(u))(x) &= T(\varphi_{M,x}^n)(T(f)(u)) = T(f \circ \varphi_{M,x}^n)(u) \\
&= T(\varphi_{N,f(x)}^n)(u) = \theta_N(u)(f(x)) = (\theta_N(u) \circ f)(x) .
\end{align*}
$$
Điều này chứng minh c).

Ta chứng minh b). Trước hết xét trường hợp riêng $M = A/m_A^n$. Khi đó $T(M)$ bằng $I_n$ theo định nghĩa. Nếu $a$ là một phần tử của A, có lớp $\bar{a}$ trong M, ta có $\varphi_{M,\bar{a}}^n = a 1_M$, do đó $T(\varphi_{M,\bar{a}}^n) = a 1_{I_n}$; vì thế $\theta_M : I_n \to \operatorname{Hom}_A(A/m_A^n, I)$ là đẳng cấu chính tắc gửi một phần tử $x$ của $I_n$ tới ánh xạ $\bar{a} \mapsto a x$. Điều này chứng minh b) trong trường hợp này.

Bây giờ giả sử đã cho một dãy khớp
$$
P \xrightarrow{u} N \xrightarrow{v} M \to 0
$$
gồm các A-môđun có độ dài hữu hạn bị triệt tiêu bởi $m_A^n$. Xét biểu đồ
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & T(M) & \xrightarrow{T(v)} & T(N) & \xrightarrow{T(u)} & T(P) \\
   &                & \downarrow{\theta_M} &           & \downarrow{\theta_N} &           & \downarrow{\theta_P} \\
0 & \longrightarrow & \operatorname{Hom}_A(M, I) & \xrightarrow{\operatorname{Hom}(v, 1)} & \operatorname{Hom}_A(N, I) & \xrightarrow{\operatorname{Hom}(u, 1)} & \operatorname{Hom}_A(P, I)
\end{array}
$$

nó là giao hoán theo phần đầu của chứng minh, và các hàng của nó là khớp theo FD 4). Ta suy ra rằng $\theta_M$ là song ánh nếu $\theta_P$ và $\theta_N$ là như vậy. Áp dụng điều này cho một biểu diễn
$$
(A/\mathfrak{m}_A^n)^r \longrightarrow (A/\mathfrak{m}_A^n)^s \longrightarrow M \longrightarrow 0
$$
của $A/\mathfrak{m}_A^n$-môđun $M$, ta suy ra rằng $\theta_M$ là song ánh đối với mọi $A$-môđun có độ dài hữu hạn bị triệt tiêu bởi $\mathfrak{m}_A^n$, do đó b).

Hãy chứng minh a). Từ điều vừa nói ở trên áp dụng cho $A$-môđun $A/\mathfrak{m}_A^n$ suy ra rằng $I_n$ là tập hợp các phần tử của $I$ bị triệt tiêu bởi $\mathfrak{m}_A^n$. Theo FD 5) thì $A$-môđun $I_1 = T(\kappa_A)$ đẳng cấu với $\kappa_A$; theo Mệnh đề 2 của No. 2, với chúng ta chỉ cần chứng minh rằng, với mọi số nguyên $n \geqslant 0$, ánh xạ A-tuyến tính chính tắc
$$
\beta : I_{n+1}/I_n \longrightarrow \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)
$$
là song ánh. Bây giờ từ dãy khớp
$$
0 \longrightarrow \mathfrak{m}_A^n/\mathfrak{m}_A^{n+1} \xrightarrow{u} A/\mathfrak{m}_A^{n+1} \xrightarrow{p_{n+1,n}} A/\mathfrak{m}_A^n \longrightarrow 0,
$$
người ta suy ra một dãy khớp
$$
0 \longrightarrow I_n \xrightarrow{i_{n+1,n}} I_{n+1} \xrightarrow{T(u)} T(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}) \longrightarrow 0.
$$
Bằng cách hợp thành $T(u)$ với $\theta_{\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}}$, do đó ta thu được một đồng cấu toàn ánh
$$
\gamma : I_{n+1} \longrightarrow \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)
$$
có hạt nhân là $I_n$. Theo c), $\gamma$ là hợp thành của các ánh xạ $\theta_{I_{n+1}} : I_{n+1} \to \mathrm{Hom}_A(A/\mathfrak{m}_A^{n+1}, I)$ và $\mathrm{Hom}(u, 1) : \mathrm{Hom}_A(A/\mathfrak{m}_A^{n+1}, I) \to \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)$; vì $\theta_{I_{n+1}}$ là ánh xạ tuyến tính liên kết với phép nhân $A/\mathfrak{m}_A^{n+1} \times I_{n+1} \to I$, nên đẳng cấu $I_{n+1}/I_n \to \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)$ suy ra từ $\gamma$ trùng với $\beta$, điều này hoàn tất chứng minh.

#### Ví dụ 5 {#ac-x-s8-n5-exa-5 .statement}

Hãy xét lại các giả thiết và ký hiệu của Ví dụ 1. Khi đó $T(A/\mathfrak{m}_A^n) = \mathrm{Hom}_A(A/\mathfrak{m}_A^n, J)$ được đồng nhất với môđun con $J_n$ của $J$ tạo bởi các phần tử bị triệt tiêu bởi $\mathfrak{m}_A^n$; bằng cách chuyển qua giới hạn quy nạp người ta thu được một đẳng cấu chính tắc từ $I$ lên $J$.

#### Ví dụ 6 {#ac-x-s8-n5-exa-6 .statement}

Hãy xét lại các giả thiết và ký hiệu của Ví dụ 3. Người ta thu được rằng $I = \varinjlim \mathrm{Ext}_A^d(A/\mathfrak{m}_A^n, \Omega)$ là một A-môđun Matlis. Với mọi $A$-môđun có độ dài hữu hạn $M$, có một A-đẳng cấu chính tắc
$$
0_M : \mathrm{Ext}_A^d(M, \Omega) \longrightarrow \mathrm{Hom}_A(M, I);
$$
hơn nữa đẳng cấu này là $\mathrm{End}_A(M)$-tuyến tính (Định lý 3, c)).

Đặc biệt, nếu vành $A$ là Gorenstein có chiều $d$, thì $A$-môđun $\varinjlim \mathrm{Ext}_A^d(A/\mathfrak{m}_A^n, A)$ là một môđun Matlis.

### 6. Thay đổi vành; đối ngẫu Macaulay

#### Mệnh đề 5 {#ac-x-s8-prop-5 .statement}

Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether, sao cho mở rộng thặng dư $\kappa_A \to \kappa_B$ cảm sinh bởi $\rho$ là bậc hữu hạn. Gọi $I_A$ là một A-môđun Matlis.

a) Ký hiệu $I_B$ là môđun con-$B$ của $\mathrm{Hom}_A(B, I_A)$ gồm các $A$-đồng cấu từ $B$ vào $I_A$ mà hạt nhân chứa một lũy thừa của $m_B$. Khi đó $I_B$ là một $B$-môđun Matlis.

b) Cho $M$ là một $B$-môđun. Ánh xạ chính tắc

$$
\alpha : \mathrm{Hom}_B(M, \mathrm{Hom}_A(B, I_A)) \longrightarrow \mathrm{Hom}_A(M, I_A)
$$

được xác định bởi $\alpha(u)(m) = u(m)(1)$ cảm sinh một $B$-đẳng cấu từ $D_B(M) = \mathrm{Hom}_B(M, I_B)$ lên môđun con-$B$ $\mathrm{Hom}_A^{cont}(M, I_A)$ của $D_A(M) = \mathrm{Hom}_A(M, I_A)$ gồm các ánh xạ $f : M \to I_A$ sao cho với mọi phần tử $m$ của $M$, tồn tại một số nguyên $n \geqslant 0$ sao cho $f(m^n_B m) = 0$.

Điều kiện trên đối với $f$ có nghĩa là $f$ liên tục khi $I_A$ được cho tôpô rời rạc và $M$ được cho tôpô mịn nhất cảm sinh trên mỗi môđun con sinh hữu hạn tôpô $m_B$-adic, điều này biện minh cho ký hiệu ấy. Tương tự, điều kiện $g \in I_B$ có nghĩa là $g$ liên tục khi $I_A$ được cho tôpô rời rạc và $B$ được cho tôpô $m_B$-adic.

Ta hãy chứng minh a). Với mọi $B$-môđun có độ dài hữu hạn $M$, ký hiệu $T(M)$ là $B$-môđun $\mathrm{Hom}_A(M, I_A)$; với mọi ánh xạ tuyến tính-$B$ $f : M \to N$ giữa các $B$-môđun có độ dài hữu hạn, ký hiệu $T(f) : T(N) \to T(M)$ là ánh xạ tuyến tính-$B$ $\mathrm{Hom}_A(f, 1_{I_A})$. Việc kiểm tra các điều kiện FD 1) đến FD 4) của No. 5 là ngay lập tức. Hơn nữa, với mọi $B$-môđun có độ dài hữu hạn $N$, ta có $\mathrm{long}_A(N_{[A]}) = \mathrm{long}_B(N) \ [\kappa_B : \kappa_A]$; vì ta có $\mathrm{long}_A(T(M)) = \mathrm{long}_A(M)$ (No. 3, đl. 2), suy ra $\mathrm{long}_B(T(M)) = \mathrm{long}_B(M)$, điều này kéo theo FD 5). Do đó ta có thể áp dụng định lý 3 của No. 5; ta có

$$
T(B/m_B^n) = \mathrm{Hom}_A(B/m_B^n, I_A),
$$

nên $B$-môđun Matlis $\varprojlim T(B/m_B^n)$ được đồng nhất với môđun con-$B$ $I_B$ của $\mathrm{Hom}_A(B, I_A)$, điều này chứng minh a).

Ta hãy chứng minh b). Ánh xạ $\alpha$ là nghịch đảo của đẳng cấu chính tắc

$$
\beta : \mathrm{Hom}_A(M, 1_A) \longrightarrow \mathrm{Hom}_B(M, \mathrm{Hom}_A(B, I_A))
$$

gắn với $v \in \mathrm{Hom}_A(M, I_A)$ ánh xạ $v'$ từ $M$ vào $\mathrm{Hom}_A(B, I_A)$ sao cho $v'(m)(b) = v(bm)$ (A, II, p. 74, mệnh đề 1). Để $v'$ nhận giá trị trong $I_B$, điều kiện cần và đủ là $v$ thuộc $\mathrm{Hom}_A^{cont}(M, I_A)$, do đó b).

#### Hệ quả {#ac-x-s8-n6-cor-1 .statement}

a) Nếu $A$-đại số $B$ là hữu hạn, thì $B$-môđun $I_B = \mathrm{Hom}_A(B, I_A)$ là một $B$-môđun Matlis.

b) Nếu $B$-môđun $M$ là Artin, thì ánh xạ $\alpha$ là một $B$-đẳng cấu từ $D_B(M)$ lên $D_A(M)$.

Mệnh đề 5 áp dụng đặc biệt khi $A$ là một trường $k$, trong trường hợp đó có thể lấy $I_A = k$, do đó $D_k(M) = \mathrm{Hom}_k^{cont}(M, k)$ ("đối ngẫu Macaulay"). Cần lưu ý rằng giả thiết $[\kappa_B : k] < +\infty$ được thỏa mãn đặc biệt khi $k$-đại số $B$ là vành địa phương tại một iđêan cực đại của một $k$-đại số kiểu hữu hạn (A, VIII, App. 3, hệ quả 1).

Đặc biệt hơn, xét một $k$-đại số $S$ phân bậc bởi $\mathbf{N}$, kiểu hữu hạn, sao cho $S_0$ là một trường, có bậc hữu hạn trên $k$. Có thể áp dụng Mệnh đề 5 cho vành địa phương $S'$ của $S$ tại iđêan cực đại $S_+ = \bigoplus_{n > 0} S_n$ hoặc, điều này tương đương, cho hoàn thành của nó $\widehat{S} = \prod_{n \geq 0} S_n$ (III, § 1, No. 3, bổ đề 2 và § 2, No. 12, ví dụ 1). Khi đó $S$-môđun $I_{\widehat{S}} = \mathrm{Hom}_k^{cont}(\widehat{S}, k)$ được đồng nhất với
$$
S^{*gr} = \bigoplus_{n \geq 0} \mathrm{Hom}_k(S_n, k)
$$
với $s \in S$ và $u \in S^{*gr}$, phần tử $su$ của $S^{*gr}$ là tích nội $s \perp u$ (A, III, p. 156 and p. 157). Lấy, chẳng hạn, $S = k[T_1, \ldots, T_d]$, do đó $\widehat{S} = k[[T_1, \ldots, T_d]]$. Gọi $(u_\alpha)_{\alpha \in \mathbf{N}^d}$ là cơ sở của không gian vectơ $k$ $S^{*gr}$ đối ngẫu với cơ sở $(T^\alpha)_{\alpha \in \mathbf{N}^d}$ của $S$. Khi đó cấu trúc của $S^{*gr}$ như một $S$-môđun được mô tả bởi các công thức (A, III, p. 167)

$$
\begin{align*}
T^\beta u_\alpha &= u_\alpha \cdot \beta & \text{nếu } \alpha \geq \beta , \\
T^\beta u_\alpha &= 0 & \text{nếu không}.
\end{align*}
$$

### 7. Đối ngẫu của các môđun mở rộng và các tích xoắn

Cho $A$ là một vành, và $P$ và $J$ là các $A$-môđun. Với mọi phức $C$ của các $A$-môđun, một đẳng cấu chính tắc của các phức đã được dựng trong A, X, p. 99, mệnh đề 12
$$
\mu : \mathrm{Homgr}_A(C \otimes_A P, J) \longrightarrow \mathrm{Homgr}_A(C, \mathrm{Hom}_A(P, J)) .
$$
Cho $M$ là một $A$-môđun, và $(C, p)$ là một phân giải xạ ảnh của $M$. Xét dãy các đồng cấu
$$
\begin{array}{ccccccccc}
\mathrm{Ext}_A(M, \mathrm{Hom}_A(P, J)) & \xrightarrow{\varphi^{-1}} & \mathrm{H}(\mathrm{Homgr}_A(C, \mathrm{Hom}_A(P, J))) & \xrightarrow{\mathrm{H}(\mu)^{-1}} & \mathrm{H}(\mathrm{Homgr}_A(C \otimes_A P, J)) \\
& \xrightarrow{u} & \mathrm{Homgr}_A(\mathrm{H}(C \otimes_A P), J) & \xrightarrow{v} & \mathrm{Homgr}_A(\mathrm{Tor}^A(M, P), J) ,
\end{array}
$$

trong đó $\varphi$ là đẳng cấu chính tắc $\varphi(C, \mathrm{Hom}_A(P, J))$ (A, X, p. 100, định lý 1), $u$ là đồng cấu chính tắc $\lambda(C \otimes_A P, J)$ (A, X, p. 82), và $v$ được suy ra từ đẳng cấu chính tắc $\psi(C, P) : \mathrm{Tor}^A(M, P) \longrightarrow \mathrm{H}(C \otimes_A P)$.

Cho $(C', p')$ là một phân giải xạ ảnh khác của $M$. Theo A, X, p. 49, Hệ quả của Mệnh đề 3, tồn tại một đồng luân phức $\alpha : C' \to C$ sao cho $p \circ \alpha = p'$. Từ A, X, p. 103, Mệnh đề 2, suy ra rằng ta có $\mathrm{H}(\alpha \otimes 1_P) \circ \psi(C', P) = \psi(C, P)$ và $\varphi(C', R) \circ \mathrm{H}(\mathrm{Homgr}(\alpha, 1_R)) = \varphi(C, R)$ với mọi A-môđun $R$. Suy ra đồng cấu phân bậc bậc 0

$$
\theta(M, P) : \mathrm{Ext}_A(M, \mathrm{Hom}_A(P, J)) \longrightarrow \mathrm{Homgr}_A(\mathrm{Tor}^A(M, P), J)
$$

là hợp thành của dãy các đồng cấu trên, độc lập với lựa chọn phân giải xạ ảnh $(C, p)$ của $M$. Theo phép dựng, nó là $\mathrm{End}_A(J)$-tuyến tính.

Định nghĩa của đồng cấu $\theta(M, P)$ có thể được trình bày tường minh như sau. Cho $p$ là một số nguyên, $v$ là một phần tử của $\mathrm{Ext}_A^p(M, \mathrm{Hom}_A(P, J))$, $\tau$ là một phần tử của $\mathrm{Tor}_p^A(M, P)$. Với sự trợ giúp của đẳng cấu $\varphi(C, \mathrm{Hom}_A(P, J))$, $v$ được biểu diễn bởi một ánh xạ tuyến tính $u : C_p \to \mathrm{Hom}_A(P, J)$ sao cho $u \circ d_C = 0$; tương tự, với sự trợ giúp của $\psi(C, P)$, $\tau$ được biểu diễn bởi một phần tử $\sum c_\mu \otimes p_\mu$ của $C_p \otimes P$ sao cho $\sum d_C(c_\mu) \otimes p_\mu = 0$. Khi đó ta có $\theta(M, P)(v)(\tau) = \sum u(c_\mu)(p_\mu)$.

Mặt khác, cho $v : C \otimes_A \mathrm{Hom}_A(P, J) \longrightarrow \mathrm{Homgr}_A(\mathrm{Homgr}_A(C, P), J)$ là đồng cấu biến phần tử $c \otimes h$, với $c \in C_p$, $h \in \mathrm{Hom}_A(P, J)$, thành đồng cấu $u \mapsto (-1)^p h(u(c))$. Nó phân bậc bậc 0; nó là song ánh nếu mỗi môđun $C_p$ là tự do kiểu hữu hạn. Dễ dàng kiểm tra rằng đây là một cấu xạ của các phức.

Xét dãy các đồng cấu

$$
\begin{array}{cccccc}
\mathrm{Tor}^A(M, \mathrm{Hom}_A(P, J)) & \xrightarrow{\psi} & \mathrm{H}(C \otimes_A \mathrm{Hom}_A(P, J)) & \xrightarrow{\mathrm{H}(v)} & \mathrm{H}(\mathrm{Homgr}_A(\mathrm{Homgr}_A(C, P), J)) \\
& \xrightarrow{w} & \mathrm{Homgr}_A(\mathrm{H}(\mathrm{Homgr}_A(C, P)), J) & \xrightarrow{t} & \mathrm{Homgr}_A(\mathrm{Ext}_A(M, P), J)
\end{array}
$$

trong đó $\psi$ là đẳng cấu chính tắc $\psi(C, \mathrm{Hom}_A(P, J))$, $w$ là đồng cấu chính tắc $\lambda(\mathrm{Homgr}_A(C, P), J)$ (A, X, p. 82), và $t$ được suy ra từ đẳng cấu chính tắc $\varphi(C, P)$. Ta thấy như trên rằng đồng cấu hợp thành

$$
\rho(M, P) : \mathrm{Tor}^A(M, \mathrm{Hom}_A(P, J)) \longrightarrow \mathrm{Homgr}_A(\mathrm{Ext}_A(M, P), J)
$$

độc lập với lựa chọn phân giải $C$; nó là $\mathrm{End}_A(J)$-tuyến tính. Cho $p$ là một số nguyên, $\xi \in \mathrm{Tor}_p^A(M, \mathrm{Hom}_A(P, J))$, $\lambda \in \mathrm{Ext}_A^p(M, P), J)$; nếu $\xi$ được biểu diễn với sự trợ giúp của $\psi(C, \mathrm{Hom}_A(P, J))$ bởi một phần tử $\sum c_\mu \otimes u_\mu$ của $C \otimes \mathrm{Hom}_A(P, J)$ sao cho $\sum d_C(c_\mu) \otimes u_\mu = 0$, và $\lambda$ với sự trợ giúp của $\varphi(C, P)$ bởi một đồng cấu $\ell : C_p \to P$ sao cho $\ell \circ d_C = 0$, thì ta có $\rho(M, P)(\xi)(\lambda) = (-1)^p \sum u_\mu(\ell(c_\mu))$.

#### Mệnh đề 6 {#ac-x-s8-prop-6 .statement}

*Giả sử A-môđun J là nội xạ; với mọi A-môđun N, đặt $D(N) = \mathrm{Hom}_A(N, J)$.*

a) Các đồng cấu $\theta^i(M, P) : \mathrm{Ext}_A^i(M, D(P)) \longrightarrow D(\mathrm{Tor}_i^A(M, P))$ là song ánh.

b) Nếu vành $A$ là Noether và $A$-môđun $M$ thuộc kiểu hữu hạn, thì các đồng cấu $\rho_i(M, P) : \mathrm{Tor}_i^A(M, D(P)) \longrightarrow D(\mathrm{Ext}_A^i(M, P))$ là song ánh.

a) Theo phép dựng, đồng cấu $\theta(M, P)$ là song ánh ngay khi $\lambda(C \otimes_A P, J)$ là song ánh, điều này xảy ra khi $J$ là nội xạ (A, X, p. 85, Hệ quả 2).

b) Chọn phân giải $C$ sao cho mỗi môđun $C_p$ là tự do thuộc kiểu hữu hạn (A, X, p. 53, Mệnh đề 6). Khi đó đồng cấu $\nu$ là song ánh, và điều tương tự cũng đúng với $\lambda(\mathrm{Homgr}_A(C, P), J)$ vì $J$ là nội xạ; do đó $\rho(M, P)$ là song ánh.

#### Nhận xét 1 {#ac-x-s8-n7-rem-1 .statement}

Với mọi đồng cấu $f : N \to N'$ của các $A$-môđun, ký hiệu bởi $D(f) : D(N') \to D(N)$ đồng cấu $\mathrm{Hom}(f, 1_J)$. Cho $u : M \to M'$ và $v : P \to P'$ là các đồng cấu của $A$-môđun. Chọn các phân giải xạ ảnh $(C, p)$ của $M$ và $(C', p')$ của $M'$, và một cấu xạ của các phức $\tilde{u} : C \to C'$ sao cho $p' \circ \tilde{u} = u \circ p$ (A, X, p. 49, Mệnh đề 3). Biểu đồ

$$
\begin{array}{ccc}
\mathrm{Homgr}_A(C' \otimes_A P', J) & \xrightarrow{\mu'} & \mathrm{Homgr}_A(C', \mathrm{Hom}_A(P', J)) \\
\downarrow \mathrm{Hom}(\tilde{u} \otimes v, 1_J) & & \downarrow \mathrm{Hom}(\tilde{u}, \mathrm{Hom}(v, 1)) \\
\mathrm{Homgr}_A(C \otimes_A P, J) & \xrightarrow{\mu} & \mathrm{Homgr}_A(C, \mathrm{Hom}_A(P, J))
\end{array}
$$

trong đó $\mu$ và $\mu'$ là các đồng cấu chính tắc, là giao hoán; khi đó suy ra từ A, X, p. 103, Mệnh đề 2 một biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Ext}_A^i(M', D(P')) & \xrightarrow{\theta^i(M', P')} & D(\mathrm{Tor}_i^A(M', P')) \\
\downarrow \mathrm{Ext}^i(u, D(v)) & & \downarrow D(\mathrm{Tor}_i(u, v)) \\
\mathrm{Ext}_A^i(M, D(P)) & \xrightarrow{\theta^i(M, P)} & D(\mathrm{Tor}_i^A(M, P))
\end{array}
$$

Cho $w : P'' \to P$ là một đồng cấu của $A$-môđun; tương tự ta thu được một biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Tor}_i^A(M, D(P)) & \xrightarrow{\rho_i(M, P)} & D(\mathrm{Ext}_A^i(M, P)) \\
\downarrow \mathrm{Tor}_i(u, D(w)) & & \downarrow D(\mathrm{Ext}^i(u, w)) \\
\mathrm{Tor}_i^A(M', D(P'')) & \xrightarrow{\rho_i(M', P'')} & D(\mathrm{Ext}_A^i(M', P''))
\end{array}
$$

#### Nhận xét 2 {#ac-x-s8-n7-rem-2 .statement}

Cho

$$(\mathcal{E})$$
$$0 \to M' \xrightarrow{j} M \xrightarrow{q} M'' \to 0$$

là một dãy khớp của các $A$-môđun. Đồng cấu $L(q) : L(M) \to L(M'')$ cảm sinh trên các phân giải tự do chính tắc là toàn ánh, và phức $Ker\,L(q)$ xác định một phân giải xạ ảnh của $M'$. Áp dụng Mệnh đề 3 của A, X, p. 104 cho dãy khớp $0 \to Ker\,L(q) \to L(M) \to L(M'') \to 0$, ta thu được các biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Ext}_A^i(M', D(P)) & \xrightarrow{\theta^i(M', P)} & D(\mathrm{Tor}_i^A(M', P)) \\
\downarrow & & \downarrow \\
\delta^i(\mathcal{E}, D(P)) & & (-1)^{i+1}D(\partial_{i+1}(\mathcal{E}, P))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{i+1}(M'', D(P)) & \xrightarrow{\theta^{i+1}(M'', P)} & D(\mathrm{Tor}_{i+1}^A(M'', P)) \\
\downarrow & & \downarrow \\
\mathrm{Tor}_{i+1}^A(M'', D(P)) & \xrightarrow{\rho_{i+1}(M'', P)} & D(\mathrm{Ext}_A^{i+1}(M'', P)) \\
\downarrow & & \downarrow \\
\partial_{i+1}(\mathcal{E}, D(P)) & & (-1)^{i+1}D(\delta^i(\mathcal{E}, P))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Tor}_{i+1}^A(M'', D(P)) & \xrightarrow{\rho_{i+1}(M'', P)} & D(\mathrm{Ext}_A^{i+1}(M'', P)) \\
\downarrow & & \downarrow \\
\mathrm{Tor}_i^A(M', D(P)) & \xrightarrow{\rho_i(M', P)} & D(\mathrm{Ext}_A^i(M', P))
\end{array}
$$

Cho

$$(\mathcal{F})$$
$$0 \to P' \to P \to P'' \to 0$$

là một dãy khớp của các $A$-môđun; vì $A$-môđun $J$ là đơn ánh, từ đó suy ra một dãy khớp

$$(\mathcal{D}(\mathcal{F}))$$
$$0 \to D(P'') \to D(P) \to D(P') \to 0.$$

Áp dụng A, X, p. 104, Mệnh đề 3 và p. 106, Mệnh đề 4 cho các dãy khớp $(\mathcal{F})$ và $(\mathcal{D}(\mathcal{F}))$, ta cũng thu được các biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Ext}_A^i(M, D(P')) & \xrightarrow{\theta^i(M, P')} & D(\mathrm{Tor}_i^A(M, P')) \\
\downarrow & & \downarrow \\
\delta^i(M, D(\mathcal{F})) & & (-1)^{i+1}D(\partial_{i+1}(M, \mathcal{F}))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{i+1}(M, D(P'')) & \xrightarrow{\theta^{i+1}(M, P'')} & D(\mathrm{Tor}_{i+1}^A(M, P''))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Tor}_{i+1}^{\mathbf{A}}(M, D(P')) & \xrightarrow{\rho_{i+1}(M, P')} & D(\mathrm{Ext}_{\Lambda}^{i+1}(M, P')) \\
\downarrow & & \downarrow \\
\partial_{i+1}(M, D(\mathcal{F})) & & (-1)^i D(\delta^i(M, \mathcal{F}))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Tor}_{i}^{\mathbf{A}}(M, P'') & \xrightarrow{\rho_{i}(M, P'')} & D(\mathrm{Ext}_{\Lambda}^{i}(M, P''))
\end{array}
$$

## BÀI TẬP {#ac-x-s8-exercises}

Xem [các bài tập của § 8](exercises/s8/).
