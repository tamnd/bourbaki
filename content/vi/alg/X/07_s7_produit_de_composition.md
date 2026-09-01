---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 7
section_title: Produit de composition
lang: vi
source: alg-x-fr
book_pages: A X.113-A X.134, A X.197-A X.202
pdf_pages: 0119-0140, 0203-0208
extraction: ocr
subsections:
    - "no": 1
      title: L’homomorphisme $\mathrm{Ext}_A(N, P) \otimes \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)$
      page: 113
      pdf_page: 119
    - "no": 2
      title: Les sept calculs du produit de composition
      page: 115
      pdf_page: 121
    - "no": 3
      title: La classe associée à une suite exacte
      page: 116
      pdf_page: 122
    - "no": 4
      title: Propriétés de la classe associée à une suite exacte
      page: 118
      pdf_page: 124
    - "no": 5
      title: Relation entre suites exactes et éléments de $\mathrm{Ext}_A(M, N)$
      page: 121
      pdf_page: 127
    - "no": 6
      title: Produit de composition et homomorphismes de liaison des modules d’extensions
      page: 125
      pdf_page: 131
    - "no": 7
      title: L’homomorphisme $\mathrm{Ext}_A(P, Q) \otimes \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M)$
      page: 128
      pdf_page: 134
    - "no": 8
      title: Produits de composition et homomorphismes de liaison des produits de torsion
      page: 130
      pdf_page: 136
    - "no": 9
      title: Calcul des produits de composition par décalage de résolutions
      page: 132
      pdf_page: 138
statements: 34
exercises: 11
content_sha256: 33005800920543ba2074c61ec8d28c20154ea3a1d8b04d6d311bfc41e9c62b38
translated_from: content/en-mt/alg/X/07_s7_produit_de_composition.md
source_lang: en-mt
translation_method: machine
source_content_sha256: d8c8eb99f6650920ba4deb364722d8d7f501be8f487b2644b5e098c334c1068e
translation_model: gpt-5.4
translation_run: translate-vi-d15958aa
glossary_version: 34
glossary_terms_sha256: 85f06722cacde9b306f6830f9f544dc1cd929271561fc4fc2d6e152bbce959e5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. TÍCH HỢP THÀNH

*Ta theo các quy ước tổng quát của §4.*

### 1. Đồng cấu $\mathrm{Ext}_A(N, P) \otimes \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)$

Cho $M$ và $N$ là hai $A$-môđun trái. Xét các đồng cấu $p_M : L(M) \to M$, $e_M : M \to I(M)$, và $e_M \circ p_M : L(M) \to I(M)$; theo Mệnh đề 4 của X, p. 86, từ đó ta suy ra một đồng cấu *song ánh*

$$
a_{M,N} = H(\mathrm{Homgr}_A(e_M \circ p_M, 1)) : H(\mathrm{Homgr}_A(I(M), I(N))) \to \mathrm{Ext}_A(M, N) .
$$

Nhắc lại thêm rằng (X, p. 82) $H^n(\mathrm{Homgr}_A(I(M), I(N)))$ là tập hợp các lớp đồng luân của các cấu xạ bậc-tăng từ phức $I(M)$ đến phức $I(N)$. Chẳng hạn, nếu $f \in \mathrm{Hom}_A(M, N)$, thì lớp đồng luân của $I(f)$ được $a_{M,N}$ gửi đến $f$.

Nếu $P$ là một $A$-môđun trái thứ ba, thì theo X, p. 99, ta có một $k$-đồng cấu chính tắc

$$
H(\mathrm{Homgr}_A(I(N), I(P))) \otimes_k H(\mathrm{Homgr}_A(I(M), I(N))) \to H(\mathrm{Homgr}_A(I(M), I(P)))
$$

từ đó ta suy ra, bằng phép chuyển qua các đẳng cấu $a_{N,P}$, $a_{M,N}$, $a_{M,P}$, một $k$-đồng cấu (gọi là *đồng cấu hợp thành*):

$$
c_{M,N,P}: \mathrm{Ext}_A(N, P) \otimes_k \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)
$$

Đồng cấu này tương ứng với một *ánh xạ song tuyến tính*

(1)

$$
\mathrm{Ext}_A(N, P) \times \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)
$$

ánh xạ này phân tích thành các thành phần thuần nhất

(2)

$$
\mathrm{Ext}_A^i(N, P) \times \mathrm{Ext}_A^j(M, N) \to \mathrm{Ext}_A^{i+j}(M, P)
$$

Nếu $u \in \mathrm{Ext}_A(N, P)$, $v \in \mathrm{Ext}_A(M, N)$, thì ảnh của $(u, v)$ qua (1) được gọi là *tích hợp thành của $u$ và $v$* và được ký hiệu là $u \circ v$. Nếu $g$ (ứng với $f$) là một cấu xạ bậc-tăng bậc $j$ (ứng với $i$) từ $I(M)$ đến $I(N)$ (ứng với từ $I(N)$ đến $I(P)$), có lớp đồng luân là $\bar{g}$ (ứng với $\bar{f}$), thì tích hợp thành $a_{N,P}(\bar{f}) \circ a_{M,N}(\bar{g})$ là ảnh qua $a_{M,P}$ của lớp đồng luân của cấu xạ $f \circ g$ từ $I(M)$ đến $I(P)$.

#### Ví dụ 1 {#alg-x-s7-n1-exa-1 .statement}

Nếu $u \in \mathrm{Hom}_A(N, P)$, $v \in \mathrm{Hom}_A(M, N)$, thì $u \circ v$ là hợp thành của $u$ và $v$.

#### Ví dụ 2 {#alg-x-s7-n1-exa-2 .statement}

Nếu $u \in \mathrm{Hom}_A(N, P)$, $v \in \mathrm{Ext}_A(M, N)$, thì

$$
u \circ v = \mathrm{Ext}_A(l_M, u)(v) \in \mathrm{Ext}_A(M, P):
$$

tương tự, nếu $u \in \mathrm{Ext}_A(N, P)$, $v \in \mathrm{Hom}_A(M, N)$, thì

$$
u \circ v = \mathrm{Ext}_A(v, l_P)(u) \in \mathrm{Ext}_A(M, P).
$$

Điều này suy ra từ các định nghĩa và các nhận xét ở X. p. 88.

Nếu $Q, M, N, P$ là bốn $A$-môđun trái, và nếu

$$
u \in \mathrm{Ext}_A(N, P), \quad v \in \mathrm{Ext}_A(M, N), \quad w \in \mathrm{Ext}_A(Q, M),
$$

thì $(u \circ v) \circ w = u \circ (v \circ w)$: tích hợp thành là *kết hợp*; do đó từ đây ta sẽ ký hiệu hợp thành của nhiều phần tử mà không dùng dấu ngoặc. Đặc biệt, theo Ví dụ 2:

#### Ví dụ 3 {#alg-x-s7-n1-exa-3 .statement}

Cho $M, N, M', N'$ là bốn $A$-môđun trái. Nếu $u \in \mathrm{Ext}_A(M, N)$, $f \in \mathrm{Hom}_A(M', M)$, $g \in \mathrm{Hom}_A(N, N')$, thì

(3)

$$
\mathrm{Ext}_A(f, g)(u) = g \circ u \circ f \in \mathrm{Ext}_A(M', N').
$$

Điều này cho một chứng minh mới về tính song tuyến tính theo $k$ của ánh xạ $(f, g) \to \mathrm{Ext}_A(f, g)$ (X, p. 88, Mệnh đề 6).

### 2. Bảy cách tính tích hợp thành

Cho $M$, $M'$ và $M''$ là ba $A$-môđun trái, $a : R \to M$, $a' : R' \to M'$ và $a'' : R'' \to M''$ là các phân giải xạ ảnh, $c : M \to E$, $c' : M' \to E'$ và $c'' : M'' \to E''$ là các phân giải đơn ánh. Từ X, p. 100, Định lý 1 và p. 103, Mệnh đề 2, suy ra rằng biểu đồ :

$$
\begin{array}{cccccc}
H(\mathrm{Homgr}_A(M, E')) & \longrightarrow & H(\mathrm{Homgr}_A(R, E')) & \longrightarrow & H(\mathrm{Homgr}_A(R, M')) \\
\uparrow & & \downarrow & & \uparrow \\
H(\mathrm{Homgr}_A(E, E')) & \xrightarrow{\varphi(E, E')} & \mathrm{Ext}_A(M, M') & \xleftarrow{\varphi(R, R')} & H(\mathrm{Homgr}_A(R, R')) \\
& \swarrow_{\varphi(M, E')} & & \searrow^{\varphi(R, M')} & \\
& & H(\mathrm{Homgr}_A(R, E')) & &
\end{array}
$$

trong đó các mũi tên không ghi nhãn được suy ra một cách chính tắc từ $c, a, c', a'$, là giao hoán, và mọi mũi tên đều là các đẳng cấu, điều này cho năm mô tả của $\mathrm{Ext}_A(M, M')$. Tương tự, ta thu được năm mô tả của $\mathrm{Ext}_A(M', M'')$, và cũng năm mô tả của $\mathrm{Ext}_A(M, M'')$.

Bây giờ xét bảy đồng cấu hợp thành

$$
H(\mathrm{Homgr}_A(C', C'')) \otimes_k H(\mathrm{Homgr}_A(C, C')) \to H(\mathrm{Homgr}_A(C, C''))
$$

trong đó lần lượt lấy cho $(C, C', C'')$ bảy bộ ba $(R, R', R''), (R, R', M''), (R, R', E''), (R, M', E''), (R, E', E''), (M, E', E''), (E, E', E'')$.

![Biểu đồ của bảy cách tính tích hợp thành](https://i.imgur.com/3Q5z5QG.png)

Hình 1.

Đồng nhất $H(\mathrm{Homgr}_A(C, C'))$ với $\mathrm{Ext}(M, M')$ nhờ đẳng cấu trên, và tương tự đối với $H(\mathrm{Homgr}_A(C', C''))$ và $H(\mathrm{Homgr}_A(C, C''))$, ta thu được *bảy đồng cấu*

$$
\mathrm{Ext}_A(M', M'') \otimes_k \mathrm{Ext}_A(M, M') \to \mathrm{Ext}_A(M, M'')
$$

Bảy đồng cấu này trùng nhau, và độc lập với lựa chọn các phân giải. Đặc biệt, chúng trùng với đồng cấu đã được định nghĩa ở No. 2, qua bộ ba $(I(M), I(M'), I(M''))$. Quả vậy, điều này suy ra từ việc diễn giải các môđun H(Homgr $(C, C')$) như môđun các lớp đồng luân của các cấu xạ phức từ C vào C’, và từ sự kiện rằng nếu trong một biểu đồ các phức

$$
\begin{array}{ccccc}
C & \xrightarrow{\ f\ } & C' & \xrightarrow{\ g\ } & C''\\
\downarrow\scriptstyle{\alpha} & & \downarrow\scriptstyle{\alpha'} & & \downarrow\scriptstyle{\alpha''}\\
C_1 & \xrightarrow{\ f_1\ } & C'_1 & \xrightarrow{\ g_1\ } & C''_1
\end{array}
$$

$\alpha'' \circ g$ đồng luân với $g_1 \circ \alpha'$ và $\alpha' \circ f$ đồng luân với $f_1 \circ \alpha$, thì $\alpha'' \circ g \circ f$ đồng luân với $g_1 \circ f_1 \circ \alpha$ (X, p. 33, Mệnh đề 4 và Hệ quả).

Trong phần sau, tùy trường hợp ta sẽ dùng cách này hay cách khác trong bảy cách xây dựng trước đây của các đồng cấu hợp thành.

### 3. Lớp liên kết với một dãy khớp

#### Mệnh đề 1 {#alg-x-s7-prop-1 .statement}

Cho $(C,d)$ và $(C',d')$ là hai phức các $A$-môđun trái và $n,p,q$ là ba số nguyên sao cho $p \geq q$. Với $p \geq i \geq q-1$, cho $f_i:C_i\longrightarrow C'_{i+n+1}$ là một đồng cấu các $A$-môđun sao cho $f_p\circ d=0$, $f_i\circ d=d'\circ f_{i+1}$ với $p>i\geq q-1$, và $d'\circ f_{q-1}=0$ (xem hình 2).

$$
\begin{array}{ccccccccccccc}
C_{p+1}&\xrightarrow{\ d\ }&C_p&\xrightarrow{\ d\ }&C_{p-1}&\xrightarrow{\ d\ }&\cdots&\xrightarrow{\ d\ }&C_q&\xrightarrow{\ d\ }&C_{q-1}&\xrightarrow{\ d\ }&C_{q-2}\\
0\downarrow&&\downarrow f_p&&\downarrow f_{p-1}&&&&\downarrow f_q&&\downarrow f_{q-1}&&\downarrow 0\\
C'_{p+n+2}&\xrightarrow{\ d'\ }&C'_{p+n+1}&\xrightarrow{\ d'\ }&C'_{p+n}&\xrightarrow{\ d'\ }&\cdots&\xrightarrow{\ d'\ }&C'_{q+n+1}&\xrightarrow{\ d'\ }&C'_{q+n}&\xrightarrow{\ d'\ }&C'_{q+n-1}
\end{array}
$$

Hình 2.

Đặt $\alpha=f_{p-1}\circ d=d'\circ f_p$, $\beta=f_{q-1}\circ d=d'\circ f_q$, và gọi $a$ (resp. $b$) là đồng cấu phân bậc $A$ bậc $n$ từ $C$ vào $C'$ mà thành phần song thuần nhất khác không duy nhất là $\alpha$ (resp. $\beta$). Khi đó ta có $a\in Z_n(\operatorname{Homgr}_A(C,C'))$, $b\in Z_n(\operatorname{Homgr}_A(C,C'))$ và

$$
a-(-1)^{(n+1)(p-q)}b\in B_n(\operatorname{Homgr}_A(C,C')).
$$

Ta có $d'\circ\alpha=d'\circ f_{p-1}\circ d=0$, $\alpha\circ d=f_{p-1}\circ d\circ d=0$, nên

$$
a\in Z_n(\operatorname{Homgr}_A(C,C')) ;
$$

Tương tự $b\in Z_n(\operatorname{Homgr}_A(C,C'))$. Đặt $\varepsilon=(-1)^{n+1}$. Ta có, trong phức $\operatorname{Homgr}_A(C,C')$ các hệ thức

$$
Df_{p-1}=d'\circ f_{p-1}-\varepsilon f_{p-1}\circ d=f_{p-2}\circ d-\varepsilon\alpha
$$

$$
Df_i=d'\circ f_i-\varepsilon f_i\circ d=f_{i-1}\circ d-\varepsilon f_{i+1}\circ d\qquad (p-1>i>q)
$$

$$
Df_q=d'\circ f_q-\varepsilon f_q\circ d=\beta-\varepsilon f_q\circ d .
$$

do đó

$$
\sum_{i=1}^{p-q} \varepsilon^i Df_{p-i} = \varepsilon^{p-q} \beta - \alpha,
$$

điều này chứng minh bổ đề.

Xét hai A-môđun trái M và N và một dãy khớp các A-môđun

(4)
$$
0 \to N \to R_n \to R_{n-1} \to \ldots \to R_1 \to M \to 0.
$$

Theo mệnh đề 3 và 3 bis của X, p. 49, tồn tại một biểu đồ giao hoán:

(5)

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{e_N} & I^0(N) & \longrightarrow & \ldots & \longrightarrow & I^{n-1}(N) & \xrightarrow{\delta^{n-1}} & I^n(N) & \xrightarrow{\delta^n} & I^{n+1}(N) \\
& & \uparrow & & \uparrow & & & & \uparrow & & \uparrow & & \uparrow \\
0 & \longrightarrow & N & \longrightarrow & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & \uparrow & & \uparrow & & & & \uparrow & & \uparrow & & \uparrow \\
L_{n+1}(M) & \xrightarrow{d_{n+1}} & L_n(M) & \xrightarrow{d_n} & L_{n-1}(M) & \longrightarrow & \ldots & \xrightarrow{d_1} & L_0(M) & \xrightarrow{p_M} & M & \longrightarrow & 0.
\end{array}
$$

Xét hai phần tử $b$ và $a$ của $\mathrm{Homgr}_A(L(M), I(N))$ mà các thành phần song thuần nhất khác không duy nhất là

$$
b^n = e_N \circ u_n : L_n(M) \to I^0(N) \quad \text{và} \quad a^n = v^n \circ p_M : L_0(M) \to I^n(N)
$$

tương ứng.

#### Mệnh đề 2 {#alg-x-s7-prop-2 .statement}

*Ta có* $a, b \in Z^n(\mathrm{Homgr}_A(L(M), I(N)))$. *Hơn nữa*, các lớp $\overline{a}$ và $\overline{b}$ của $a$ và $b$ trong $H^n(\mathrm{Homgr}_A(L(M), I(N))) = \mathrm{Ext}_A^n(M, N)$ chỉ phụ thuộc vào dãy khớp (4) và bằng nhau.

Theo mệnh đề 1, áp dụng cho hai hàng ngoài cùng của (5) và cho các mũi tên thẳng đứng hợp thành, với $p = n, q = 0$, ta có $a, b \in Z^n(\mathrm{Homgr}_A(I(M), L(N)))$ và

$$
a - b = a - (-1)^{(n+1)n} b \in B^n(\mathrm{Homgr}_A(L(M), I(N))) .
$$

Vì $a$ (resp. $b$) độc lập với lựa chọn của $u$ (resp. $v$), phần tử $\overline{a} = \overline{b}$ của $\mathrm{Ext}_A^n(M, N)$ độc lập với lựa chọn các cấu xạ $u$ và $v$, do đó suy ra mệnh đề.

#### Định nghĩa 1 {#alg-x-s7-def-1 .statement}

*Ta gọi lớp liên kết với dãy khớp* (4) *là phần tử* $\theta$ *của* $\mathrm{Ext}_A^n(M, N)$ *được xác định bởi* $\theta = (-1)^{n(n+1)/2} \overline{a} = (-1)^{n(n+1)/2} \overline{b}$.

#### Nhận xét 1 {#alg-x-s7-n3-rem-1 .statement}

Cho (P, p) là một phân giải xạ ảnh của M. Theo X, p. 49. mệnh đề 3, tồn tại một biểu đồ giao hoán

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \longrightarrow & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & \uparrow & & \uparrow & & & & \uparrow & & \uparrow & & \uparrow \\
P_n & \longrightarrow & P_{n-1} & \longrightarrow & \ldots & \longrightarrow & P_0 & \xrightarrow{p} & M & \longrightarrow & 0.
\end{array}
$$

Với các ký hiệu của § 6, θ là ảnh dưới φ(P, N) của lớp đồng luân của cấu xạ P → N xác định bởi (−1)^{n(n+1)/2} \tilde{u}_n. Tương tự, nếu (e, E) là một phân giải đơn ánh của N, thì tồn tại một biểu đồ giao hoán

$$
\begin{array}{cccccccccccc}
0 & \longrightarrow & N & \longrightarrow & E^0 & \longrightarrow & \ldots \longrightarrow & E^{n-1} & \longrightarrow & E^n \\
& & ^{1_N}\uparrow & & ^{\tilde{v}^0}\uparrow & & & ^{\tilde{v}^{n-1}}\uparrow & & ^{\tilde{v}^n}\uparrow \\
0 & \longrightarrow & N & \longrightarrow & R_n & \longrightarrow & \ldots \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 .
\end{array}
$$

và θ là ảnh dưới φ(M, E) của lớp đồng luân của cấu xạ M → E xác định bởi (−1)^{n(n+1)/2} v^n. Điều này suy ra từ phép dựng của θ và các định nghĩa của φ(P, N) và φ(M, E).

#### Nhận xét 2 {#alg-x-s7-n3-rem-2 .statement}

Khi $n = 0$, dãy khớp (4) có dạng $0 \to N \xrightarrow{f} M \to 0$, và lớp liên kết là $f^{-1} \in \mathrm{Hom}_A(M, N) = \mathrm{Ext}^0_A(M, N)$.

### 4. Các tính chất của lớp liên kết với một dãy khớp

#### Mệnh đề 3 {#alg-x-s7-prop-3 .statement}

Cho

(6)
$$
0 \to P \to S_m \to S_{m-1} \to \ldots \to S_1 \xrightarrow{\lambda} N \to 0
$$
(7)
$$
0 \to N \twoheadrightarrow R_n \to R_{n-1} \to \ldots \to R_1 \to M \to 0
$$
là hai dãy khớp của các A-môđun trái, với các lớp tương ứng θ ∈ Ext^m_A(N, P) và θ' ∈ Ext^n_A(M, N). Lớp trong Ext^{m+n}_A(M, P) liên kết với dãy khớp (8)
$$
0 \to P \to S_m \to \ldots \to S_1 \xrightarrow{\mu \circ \lambda} R_n \to \ldots \to R_1 \to M \to 0
$$
là tích hợp thành θ ∘ θ'.

Chọn các biểu đồ giao hoán

$$
\begin{array}{cccccccccccc}
0 & \longrightarrow & P & \longrightarrow & I^0(P) & \longrightarrow & \ldots \longrightarrow & I^{m-1}(P) & \xrightarrow{\delta_P^{m-1}} & I^m(P) \\
& & ^{l_P}\uparrow & & ^{w^0}\uparrow & & & ^{w^{m-1}}\uparrow & & ^{w^m}\uparrow \\
0 & \longrightarrow & P & \longrightarrow & S_m & \longrightarrow & \ldots \longrightarrow & S_1 & \xrightarrow{\lambda} & N & \longrightarrow & 0 ,
\end{array}
$$
$$
\begin{array}{cccccccccccc}
0 & \longrightarrow & N & \xrightarrow{e_N} & I^0(N) & \longrightarrow & \ldots \longrightarrow & I^{n-1}(N) & \longrightarrow & I^n(N) \\
& & ^{1_N}\uparrow & & ^{v^0}\uparrow & & & ^{v^{n-1}}\uparrow & & ^{v^n}\uparrow \\
0 & \longrightarrow & N & \xrightarrow{\mu} & R_n & \longrightarrow & \ldots \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 .
\end{array}
$$

Vì $I^m(P)$ là nội xạ, tồn tại một đồng cấu $h^0 \colon I^0(N) \rightarrow I^m(P)$ sao cho $w^m = h^0 \circ e_N$; theo X, p. 49, Proposition 3 bis, $h^0$ mở rộng thành một cấu xạ của các phức $h \colon I(N) \rightarrow I(P)\, (-m)$. Do đó $w^m = h^0 \circ e_N = h^0 \circ v^0 \circ \mu$, suy ra
$$
\delta_I^{m-1} \circ w^{m-1} = w^m \circ \lambda = h^0 \circ v^0 \circ (\mu \circ \lambda),
$$

và biểu đồ sau là giao hoán:

$$
\begin{array}{ccccccccccccccccccc}
0&\longrightarrow&P&\longrightarrow&I^0(P)&\longrightarrow&\cdots&\longrightarrow&I^{m-1}(P)&\longrightarrow&I^m(P)&\longrightarrow&I^{m+1}(P)&\longrightarrow&\cdots&\longrightarrow&I^{m+n}(P)\\
&&\uparrow^{i_P}&&\uparrow^{w^0}&&&&\uparrow^{w^{m-1}}&&\uparrow^{t^0}&&\uparrow^{t^1}&&&&\uparrow^{t^n}\\
0&\longrightarrow&P&\longrightarrow&S_m&\longrightarrow&\cdots&\longrightarrow&S_1&\xrightarrow[\mu\circ\lambda]{}&R_n&\longrightarrow&R_{n-1}&\longrightarrow&\cdots&\longrightarrow&M&\longrightarrow&0
\end{array}
$$

trong đó $t^0=h^0\circ v^0$, $t^1=(-1)^m h^1\circ v^1$, $\ldots$, $t^i=(-1)^{mi}h^i\circ v^i$, $\ldots$, $t^n=(-1)^{mn}h^n\circ v^n$.

Lớp $\theta$ liên kết với (6) là lớp của $(-1)^{m(m+1)/2}w^m\in\operatorname{Homgr}_A^m(N,I(P))$, tương ứng qua đẳng cấu $\alpha_{N,P}$ với lớp của $(-1)^{m(m+1)/2}h\in\operatorname{Homgr}_A^m(I(N),I(P))$; lớp $\theta'$ liên kết với (7) là lớp của $(-1)^{n(n+1)/2}v^n\in\operatorname{Homgr}^n(M,I(N))$, lớp liên kết với (8) là lớp của $(-1)^{(m+n)(m+n+1)/2}t^n\in\operatorname{Homgr}^{m+n}(M,I(P))$, do đó suy ra kết luận, theo định nghĩa của tích hợp thành (X, p. 114) và công thức

$$
m(m+1)/2+n(n+1)/2=(m+n)(m+n+1)/2-mn.
$$

4. - Xét một biểu đồ giao hoán các $A$-môđun với các hàng là dãy khớp

$$
\begin{array}{ccccccccccccccc}
0&\longrightarrow&N&\longrightarrow&R_n&\longrightarrow&R_{n-1}&\longrightarrow&\cdots&\longrightarrow&R_1&\longrightarrow&M&\longrightarrow&0\\
&&\downarrow^{g}&&\downarrow&&\downarrow&&&&\downarrow&&\downarrow^{f}&&\\
0&\longrightarrow&N'&\longrightarrow&R'_n&\longrightarrow&R'_{n-1}&\longrightarrow&\cdots&\longrightarrow&R'_1&\longrightarrow&M'&\longrightarrow&0.
\end{array}
$$

Gọi $\theta$ (resp. $\theta'$) là lớp của hàng thứ nhất (resp. hàng thứ hai) trong

$$
\operatorname{Ext}_A^n(M,N)\quad\text{(tương ứng }\operatorname{Ext}_A^n(M',N')\text{)}.
$$

Trong $\operatorname{Ext}_A^n(M,N')$, ta có $\theta'\circ f=g\circ\theta$.

Thật vậy, xét một biểu đồ giao hoán

$$
\begin{array}{ccccccccccccc}
L_n(M)&\xrightarrow{d_n}&L_{n-1}(M)&\longrightarrow&\cdots&\longrightarrow&L_0(M)&\xrightarrow{p_M}&M&\longrightarrow&0\\
\downarrow^{u_n}&&\downarrow&&&&\downarrow&&\downarrow^{1}\\
0&\longrightarrow&N&\longrightarrow&R_n&\longrightarrow&\cdots&\longrightarrow&R_1&\longrightarrow&M&\longrightarrow&0\\
&&\downarrow^{g}&&\downarrow&&&&\downarrow&&\downarrow^{f}\\
0&\longrightarrow&N'&\longrightarrow&R'_n&\longrightarrow&\cdots&\longrightarrow&R'_1&\longrightarrow&M'&\longrightarrow&0\\
&&\downarrow&&\downarrow&&&&\downarrow&&\downarrow^{v^n}\\
0&\longrightarrow&N'&\xrightarrow{\epsilon_{N'}}&I^0(N')&\xrightarrow{\delta^0}&\cdots&\longrightarrow&I^{n-1}(N')&\xrightarrow{\delta^{n-1}}&I^n(N')
\end{array}
$$

Theo định nghĩa, $\theta'\circ f$ là lớp của $(-1)^{n(n+1)/2}v^n\circ f\circ p_M\in\operatorname{Homgr}^n(L(M),I(N'))$, còn $g\circ\theta$ là lớp của $(-1)^{n(n+1)/2}\epsilon_{N'}\circ g\circ u_n$. Theo Bổ đề 1, áp dụng cho hai hàng biên của biểu đồ, hai lớp này bằng nhau.

#### Hệ quả 1 {#alg-x-s7-prop-3-cor-1 .statement}

Xét một biểu đồ giao hoán với các hàng khớp

$$
\begin{array}{cccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & \cdots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
\downarrow & & \downarrow & & \downarrow & & & \downarrow & & \downarrow & & \downarrow \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & \cdots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0 ;
\end{array}
$$

hai hàng của biểu đồ có cùng lớp liên kết trong $\mathrm{Ext}_A^n(M, N)$.

#### Hệ quả 2 {#alg-x-s7-prop-3-cor-2 .statement}

Cho

$$
0 \to N \xrightarrow{f_{n-1}} R_n \xrightarrow{f_n} R_{n-1} \to \cdots \xrightarrow{f_2} R_1 \xrightarrow{f_1} M \to 0
$$

là một dãy khớp, $\theta \in \mathrm{Ext}_A^n(M, N)$ là lớp liên kết của nó, $a_1, \ldots, a_{n+1}$ là các phần tử khả nghịch của $k$. Lớp liên kết của dãy khớp

$$
0 \to N \xrightarrow{a_{n+1} f_{n+1}} R_n \xrightarrow{a_n f_n} R_{n-1} \to \cdots \xrightarrow{a_2 f_2} R_1 \xrightarrow{a_1 f_1} M \to 0
$$

là $(a_1^{-1}\, a_2^{-1}\, \ldots\, a_{n+1}^{-1})\ \theta$.

Thật vậy, có một biểu đồ giao hoán

$$
\begin{array}{ccccccccccccccc}
0 & \rightarrow & N & \xrightarrow{a_{n+1} f_{n+1}} & R_n & \rightarrow & \cdots & \rightarrow & R_2 & \xrightarrow{a_2 f_2} & R_1 & \xrightarrow{a_1 f_1} & M & \rightarrow & 0 \\
& & \downarrow a_1 \ldots a_{n+1} & & \downarrow a_1 \ldots a_n & & & \downarrow a_1 a_2 & & \downarrow a_1 & & \downarrow 1 \\
0 & \rightarrow & N & \xrightarrow{f_{n+1}} & R_n & \rightarrow & \cdots & \rightarrow & R_2 & \xrightarrow{f_2} & R_1 & \xrightarrow{f_1} & M & \rightarrow & 0 .
\end{array}
$$

và ta áp dụng mệnh đề.

#### Hệ quả 3 {#alg-x-s7-prop-3-cor-3 .statement}

Cho $0 \to N \xrightarrow{f_{n-1}} R_n \xrightarrow{f_n} \cdots \to R_1 \xrightarrow{f_1} M \to 0$ là một dãy khớp, $\theta$ lớp của nó trong $\mathrm{Ext}_A^n(M, N)$, $u \colon M' \to M$ và $v \colon N \to N'$ là các đồng cấu của $A$-môđun.

a) Phần tử $v \circ \theta$ của $\mathrm{Ext}_A^n(M, N')$ bằng lớp của dãy khớp

$$
0 \to N' \xrightarrow{f_{n'+1}} R'_n \xrightarrow{f_{n'}} R_{n-1} \xrightarrow{f_{n-1}} \cdots \to R_1 \to M \to 0 ,
$$

trong đó $R'_n$ là $A$-môđun thương của $R_n \oplus N'$ theo môđun con gồm các cặp $(f_{n+1}(x), -v(x))$ với $x \in N$, và trong đó $f_{n'+1}'$ (tương ứng $f_{n'}'$) được suy ra từ đơn ánh chính tắc (tương ứng từ $(f_n, 0)$) bằng cách chuyển qua thương.

b) Phần tử $\theta \circ u$ của $\mathrm{Ext}_A^n(M', N)$ là lớp của dãy khớp

$$
0 \to N \to R_n \to \cdots \to R_2 \xrightarrow{f_2''} R'_1 \xrightarrow{f_1''} M' \to 0 ,
$$

trong đó $R'_1$ là tích thớ $R_1 \times_M M'$, nghĩa là (I, p. 44) môđun con của $R_1 \times M'$ gồm các cặp $(x, y)$ sao cho $f_1(x) = u(y)$, và trong đó $f_2''$ (tương ứng $f_1''$) được suy ra từ $(f_2, 0)$ (tương ứng từ phép chiếu thứ hai).

Chẳng hạn, ta hãy chứng minh $a$. Cho $z$ là một phần tử của $R'_n$ sao cho $f'_n(z) = 0$; nếu $z$ là lớp của một cặp $(x, y)$, với $x \in R_n$, $y \in N'$, thì ta có $f_n(x) = 0$, nên tồn tại một phần tử $t \in N$ sao cho $x = f_{n+1}(t)$. Khi đó ta có $z = f'_{n+1}(y + v(t))$, điều này chứng minh rằng $\mathrm{Ker}\ f'_n = \mathrm{Im}\ f'_{n+1}$. Tính đơn ánh của $f'_{n+1}$ suy ra từ tính đơn ánh của $f_{n+1}$.

Cho $j : R_n \to R'_n$ là đồng cấu suy ra từ đơn ánh chính tắc; ta có một biểu đồ giao hoán của các dãy khớp:

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{f_{n+1}} & R_n & \xrightarrow{f_n} & R_{n-1} & \longrightarrow & \ldots & \longrightarrow & M & \longrightarrow & 0 \\
& & \downarrow v & & \downarrow j & & \downarrow 1 & & & & \downarrow 1 & & \\
0 & \longrightarrow & N' & \xrightarrow{f'_{n+1}} & R'_n & \xrightarrow{f'_n} & R'_{n-1} & \longrightarrow & \ldots & \longrightarrow & M & \longrightarrow & 0 ;
\end{array}
$$

mệnh đề $a$ khi đó suy ra từ mệnh đề.

Chứng minh của $b$ là tương tự.

#### Nhận xét {#alg-x-s7-n4-rem-1 .statement}

Cho $\theta \in \mathrm{Ext}^n_A(M, N)$, tương ứng $\theta' \in \mathrm{Ext}^n_A(M', N')$, là lớp của một dãy khớp

$$
0 \to N \xrightarrow{f_{n+1}} R_n \to \ldots \to R_1 \xrightarrow{f_1} M \to 0,
$$
tương ứng $0 \to N' \xrightarrow{f'_{n+1}} R'_n \to \ldots \to R'_1 \xrightarrow{f'_1} M' \to 0.$

Cho $i_N,\ i_{N'}$, là các đơn ánh chính tắc của $N$ và $N'$ vào $N \oplus N'$, $q_M,\ q_{M'}$, là các phép chiếu của $M \oplus M'$ lên $M$ và $M'$. Xét đồng cấu

$$
m = \mathrm{Ext}\,(q_M,\ i_N) \oplus \mathrm{Ext}\,(q_{M'},\ i_{N'})
$$

từ $\mathrm{Ext}_A(M, N) \oplus \mathrm{Ext}_A(M', N')$ vào $\mathrm{Ext}_A(M \oplus M', N \oplus N')$. *Phần tử*

$$
m(\theta, \theta') = i_N \circ \theta \circ q_M + i_{N'} \circ \theta' \circ q_{M'}
$$

*là lớp của dãy khớp*

$$
0 \to N \oplus N' \xrightarrow{f_{n-1} \oplus f'_{n-1}} R_n \oplus R'_n \to \ldots \to R_1 \oplus R'_1 \xrightarrow{f_1 \oplus f'_1} M \oplus M' \to 0 .
$$

Thật vậy, nếu ký hiệu lớp này là $\theta''$, thì từ mệnh đề 4 suy ra rằng ta có

$$
\theta'' \circ i_M = i_N \circ \theta = m(\theta, \theta') \circ i_M \quad \text{and} \quad \theta'' \circ i_{M'} = i_{N'} \circ \theta = m(\theta, \theta') \circ i_{M'} ;
$$

theo X, p. 89, mệnh đề 7, điều đó kéo theo $\theta'' = m(\theta, \theta')$.

### 5. Quan hệ giữa các dãy khớp và các phần tử của $\mathrm{Ext}_A(M, N)$

#### Định lý 1 {#alg-x-s7-thm-1 .statement}

*Cho $n$ là một số nguyên $\geqslant 1$, $M$ và $N$ là hai $A$-môđun.*

a) *Mọi phần tử của $\mathrm{Ext}^n_A(M, N)$ đều là lớp của một dãy khớp* (X, p. 117, định nghĩa 1).

b) *Cho* $0 \to N \xrightarrow{f_{n+1}} R_n \xrightarrow{f_n} \ldots \to R_1 \xrightarrow{f_1} M \to 0$ và $0 \to N \xrightarrow{f_{n+1}} R'_n \xrightarrow{f_n} \ldots \to R'_1 \xrightarrow{f_1} M \to 0$

là các dãy khớp, $\theta$ và $\theta'$ là các lớp liên kết. Các điều kiện sau là tương đương:

(i) $\theta = \theta'$;

(ii) tồn tại một biểu đồ giao hoán với các hàng khớp:

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{f_{n+1}} & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \xrightarrow{f_1} & M & \longrightarrow & 0 \\
& & 1_N \uparrow & & \uparrow & & & & \uparrow & & 1_M \uparrow \\
0 & \longrightarrow & N & \longrightarrow & R''_n & \longrightarrow & \ldots & \longrightarrow & R''_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & 1_N \downarrow & & \downarrow & & & & \downarrow & & 1_M \downarrow \\
0 & \longrightarrow & N & \xrightarrow{f'_{n+1}} & R'_n & \longrightarrow & \ldots & \longrightarrow & R'_1 & \xrightarrow{f'_1} & M & \longrightarrow & 0 ;
\end{array}
$$

(iii) tồn tại một biểu đồ giao hoán với các hàng khớp:

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{f_{n+1}} & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \xrightarrow{f_1} & M & \longrightarrow & 0 \\
& & 1_N \downarrow & & \downarrow & & & & \downarrow & & 1_M \downarrow \\
0 & \longrightarrow & N & \longrightarrow & R''_n & \longrightarrow & \ldots & \longrightarrow & R''_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & 1_N \uparrow & & \uparrow & & & & \uparrow & & 1_M \uparrow \\
0 & \longrightarrow & N & \xrightarrow{f'_{n+1}} & R'_n & \longrightarrow & \ldots & \longrightarrow & R'_1 & \xrightarrow{f'_1} & M & \longrightarrow & 0 .
\end{array}
$$

Ta hãy chứng minh $a$. Cho $\alpha \in \mathrm{Ext}_A^n(M, N)$, và cho $P$ là một phân giải xạ ảnh của $M$. Cho $a : P(n) \to N$ là một cấu xạ phức biểu diễn $\alpha$; thành phần khác không duy nhất của nó là một $A$-đồng cấu $u : P_n \to N$ thỏa mãn $u \circ d_{n+1} = 0$, nên phân tích thành $u = \overline{u} \circ \delta_n$, trong đó $\delta_n : P_n \to Z_{n-1}$ là ánh xạ cảm sinh bởi $d_n$ (ta đặt $Z_{n-1} = \mathrm{Im}\, d_n$) và $\overline{u}$ là một $A$-đồng cấu từ $Z_{n-1}$ vào $N$. Theo Nhận xét 1, p. 117, lớp $\theta \in \mathrm{Ext}_A^n(M, Z_{n-1})$ của dãy khớp

$$
0 \to Z_{n-1} \to P_{n-1} \to \ldots \to P_0 \to M \to 0
$$

bằng lớp đồng luân của cấu xạ $(-1)^{n(n+1)/2} \delta_n$. Do đó ta có

$$
\alpha = (-1)^{n(n+1)/2} \overline{u} \circ \theta ,
$$

điều này cho phép, theo Hệ quả 3, p. 120, biểu diễn $\alpha$ như lớp của một dãy khớp.

Ta hãy chứng minh $b$. Từ Hệ quả 1 của X, p. 120 suy ra rằng (ii) $\Rightarrow$ (i) và (iii) $\Rightarrow$ (i). Giả sử rằng (i) được thỏa mãn, và cho $P$ là một phân giải xạ ảnh của $M$. Khi đó tồn tại một biểu đồ giao hoán

$$
\begin{array}{cccccccccccccc}
0 & \rightarrow & N & \xrightarrow{f_{n+1}} & R_n & \rightarrow & R_{n-1} & \rightarrow & \ldots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & u_n \uparrow & & u_{n-1} \uparrow & & u_{n-2} \uparrow & & & & & & 1_M \uparrow \\
& & P_n & \xrightarrow{d_n} & P_{n-1} & \rightarrow & P_{n-2} & \rightarrow & \ldots \rightarrow & P_0 & \rightarrow & M & \rightarrow & 0 \\
& & u'_n \downarrow & & u'_{n-1} \downarrow & & u'_{n-2} \downarrow & & & & & & 1_M \downarrow \\
0 & \rightarrow & N & \xrightarrow{f'_{n+1}} & R'_n & \rightarrow & R'_{n-1} & \rightarrow & \ldots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0 .
\end{array}
$$

Các cấu xạ từ $P(n)$ vào $N$ được xác định bởi $u_n$ và $u'_n$ là đồng luân, vì cả hai đều thuộc lớp $(-1)^{n(n+1)/2} \theta$, nên $u'_n - u_n$ có dạng $w \circ d_n$, trong đó $w : P_{n-1} \to N$ là một $A$-đồng cấu. Thay $u'_{n-1}$ bởi $u'_{n-1} - f'_{n+1} \circ w$ và $u'_n$ bởi $u_n$, ta rút gọn về trường hợp $u_n = u'_n$. Điều này cho phép xây dựng một biểu đồ giao hoán mới với các hàng khớp:

$$
\begin{array}{cccccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & R_{n-1} & \rightarrow & \ldots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \uparrow & & v \uparrow & & u_{n-2} \uparrow & & & & & & 1_M \uparrow \\
0 & \rightarrow & N & \rightarrow & N' & \rightarrow & P_{n-2} & \rightarrow & \ldots \rightarrow & P_0 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \downarrow & & v' \downarrow & & u'_{n-2} \downarrow & & & & & & 1_M \downarrow \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & R'_{n-1} & \rightarrow & \ldots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0
\end{array}
$$

trong đó $N'$ là thương của $P_{n-1} \oplus N$ bởi môđun con tạo thành bởi các cặp $(d_n(x), -u_n(x))$ với $x \in P_n$, và trong đó $v$ (resp. $v'$) được xác định bằng cách chuyển qua thương từ ánh xạ $u_{n-1} \oplus f_{n+1}$ (resp. $u'_{n-1} \oplus f'_{n+1}$). Vậy điều kiện (ii) được thỏa mãn.

Lại giả sử rằng điều kiện (i) được thỏa mãn, và gọi $E$ là một giải nhập của $N$. Tồn tại một biểu đồ giao hoán

$$
\begin{array}{cccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & \ldots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \downarrow & & v_0 \downarrow & & & & & & & \\
0 & \rightarrow & N' & \rightarrow & E^0 & \xrightarrow{\delta^0} & \ldots \rightarrow & E^{n-1} & \xrightarrow{\delta^{n-1}} & E^n \\
& & 1_N \uparrow & & v'_0 \uparrow & & & & & & & \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & \ldots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0
\end{array}
$$

và như trên ta chứng minh rằng có thể giả sử $v'_n = v_n$. Khi đó ta có một biểu đồ giao hoán với các hàng khớp

$$
\begin{array}{cccccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & \ldots \rightarrow & R_2 & \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \downarrow & & \downarrow & & & & & & & & 1_M \downarrow \\
0 & \rightarrow & N & \rightarrow & E^0 & \rightarrow & \ldots \rightarrow & E^{n-2} & \rightarrow & M' & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \uparrow & & \uparrow & & & & & & & & 1_M \uparrow \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & \ldots \rightarrow & R'_2 & \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0
\end{array}
$$

với $M' = M \times_{\mathbf{R}_1} E_{n-1}$ (xem X, p. 120, hệ quả 3, b)). Vậy điều kiện (iii) được thỏa mãn, điều này hoàn tất chứng minh định lý.

#### Nhận xét 1 {#alg-x-s7-n5-rem-1 .statement}

Nếu vành $A$ là Noether, và nếu các $A$-môđun $M$ và $N$ là hữu hạn kiểu, thì từ chứng minh của a) suy ra rằng mọi phần tử của $\mathrm{Ext}_A^n(M, N)$ là lớp liên kết với một dãy khớp $0 \to N \to R_n \to \ldots \to R_1 \to M \to 0$ trong đó các $R_i$ là hữu hạn kiểu.

#### Hệ quả {#alg-x-s7-n5-cor-1 .statement}

*Cho* $0 \to N \xrightarrow{f} R \xrightarrow{g} M \to 0$ *và* $0 \to N \xrightarrow{f'} R' \xrightarrow{g'} M \to 0$ *là hai dãy khớp*, $\theta$ *và* $\theta'$ *các lớp liên kết của chúng trong* $\mathrm{Ext}^1(M, N)$. *Để có* $\theta = \theta'$*, điều kiện cần và đủ là tồn tại một* A-đồng cấu $h : R \to R'$ *làm cho biểu đồ*

$$
\begin{array}{ccc}
& & R \\
N & \xrightarrow{f} & R \\
& \downarrow h & \downarrow g \\
& & M \\
& \xrightarrow{f'} & R' \\
& & \xrightarrow{g'}
\end{array}
$$

*giao hoán. Một đồng cấu như vậy tất yếu là một đẳng cấu.*

Điều kiện ấy là đủ theo hệ quả 1 của mệnh đề 4. Nếu $\theta = \theta'$, tồn tại một biểu đồ giao hoán với các hàng khớp:

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & N & \longrightarrow & R & \longrightarrow & M & \longrightarrow & 0 \\
& & ^{1_N} & & ^{h'} & & ^{1_M} & & \\
0 & \longrightarrow & N & \longrightarrow & R'' & \longrightarrow & M & \longrightarrow & 0 \\
& & ^{1_N} & & ^{h''} & & ^{1_M} & & \\
0 & \longrightarrow & N & \longrightarrow & R' & \longrightarrow & M & \longrightarrow & 0 .
\end{array}
$$

Các đồng cấu $h'$ và $h''$ là các đẳng cấu theo X, p. 7, hệ quả 3, và $h = h'' \circ {h'}^{-1}$ trả lời câu hỏi. Khẳng định cuối cùng suy ra từ *loc. cit.*

#### Nhận xét 2 {#alg-x-s7-n5-rem-2 .statement}

Định lý 1 cho một mô tả của $\mathrm{Ext}_A^n(M, N)$ như một tập hợp các lớp tương đương của các dãy khớp; thật dễ mô tả luật nhóm thu được trên tập hợp này bằng phép chuyển cấu trúc. Thật vậy, gọi $\theta$ (tương ứng, $\theta'$) là lớp của một dãy khớp $0 \to N \xrightarrow{f_{n+1}} R_n \xrightarrow{f_n} \ldots \to R_1 \to M \to 0$ (tương ứng, $0 \to N \xrightarrow{f'_{n+1}} R'_n \xrightarrow{f'_n} \ldots \to R'_1 \to M \to 0$). Gọi $\Delta : M \to M \oplus M$ và $\nabla : N \oplus N \to N$ là các ánh xạ $A$-tuyến tính được xác định bởi $\Delta(x) = (x, x)$ với $x \in M$ và $\nabla(y, z) = y + z$ với $y, z \in N$. Xét ánh xạ

$$
m : \mathrm{Ext}_A(M, N) \oplus \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M \oplus M, N \oplus N)
$$

được định nghĩa trong *nhận xét*, p. 121. Với các ký hiệu của *loc. cit.*, ta có $\nabla \circ i_N = 1_N$ và $q_M \circ \Delta = 1_M$, và do đó $\theta + \theta' = \nabla \circ m(\theta, \theta') \circ \Delta$. Tính đến *loc. cit.* và hệ quả 3, p. 120, điều này cho một dãy khớp thuộc lớp $\theta+\theta'$: chẳng hạn, nếu $n \geq 2$, có thể lấy dãy

$$
0\longrightarrow \mathbf{N}\longrightarrow R_n''\longrightarrow R_{n-1}\oplus R'_{n-1}\xrightarrow{\,f_{n-1}\oplus f'_{n-1}\,}\cdots\longrightarrow R_2\oplus R'_2\longrightarrow R'_1\longrightarrow M\longrightarrow0
$$

trong đó $R_n''$ là thương của $R_n\oplus R'_n$ theo môđun con tạo bởi các cặp

$$
\left(f_{n+1}(x),-f'_{n+1}(x)\right)\quad\text{với }x\in\mathbf{N},
$$

và trong đó $R''_1=R_1\times_M R'_1$.

### 6. Tích Hợp thành và các Đồng cấu Nối kết của các Môđun Mở rộng

#### Mệnh đề 5 {#alg-x-s7-prop-5 .statement}

Cho

$$(\mathcal{E})\qquad 0\longrightarrow M'\xrightarrow{\,f\,}M\xrightarrow{\,g\,}M''\longrightarrow0$$

là một dãy khớp của các môđun trái trên $A$, $\theta\in\operatorname{Ext}^1_A(M'',M')$ là lớp liên kết, $N$ là một môđun trái trên $A$, $n$ là một số nguyên.

a) Đồng cấu nối kết $\delta^n(N,\mathcal{E}):\operatorname{Ext}^n_A(N,M'')\longrightarrow\operatorname{Ext}^{n+1}_A(N,M')$ là tích hợp thành $\alpha\mapsto\theta\circ\alpha$ với $\theta$.

#### Hệ quả 1 {#alg-x-s7-prop-5-cor-1 .statement}

a) *Đồng cấu nối kết* $\mathrm{Hom}_A(M'', M'') \to \mathrm{Ext}_A^1(M'', M')$ *gửi* $1_{M''}$ *lên* $\theta$.

b) *Đồng cấu nối kết* $\mathrm{Hom}_A(M', M') \to \mathrm{Ext}_A^1(M'', M')$ *gửi* $1_{M'}$ *lên* $-\theta$.

#### Hệ quả 2 {#alg-x-s7-prop-5-cor-2 .statement}

*Xét hai dãy khớp ngắn của các môđun trái trên A*

$$
\begin{align*}
0 &\to M' \to M \to M'' \to 0 \\
0 &\to N' \to N \to N'' \to 0 .
\end{align*}
$$

*Khi đó các đồng cấu nối kết hợp thành*

$$
\operatorname{Ext}_A^n(M',N'') \to \operatorname{Ext}_A^{n+1}(M'',N'') \to \operatorname{Ext}_A^{n+2}(M'',N')
$$

*và*

$$
\operatorname{Ext}_A^n(M',N'') \to \operatorname{Ext}_A^{n+1}(M',N') \to \operatorname{Ext}_A^{n+2}(M'',N')
$$

*là đối nhau.*

Thật vậy, gọi $\theta_1$, $\theta_2$ là các lớp liên kết với các dãy khớp đã cho, và gọi $\alpha \in \operatorname{Ext}_A^n(M', M'')$. Các ảnh của $\alpha$ lần lượt là

$$
\theta_2 \circ \bigl((-1)^{n+1} \alpha \circ \theta_1\bigr) \quad \text{và} \quad (\theta_2 \circ \alpha) \circ \bigl((-1)^{n+2} \theta_1\bigr).
$$

Xét một dãy khớp ngắn của các môđun trái trên A

$$
(\mathcal{S}) \qquad 0 \to N \to R_n \xrightarrow{f_n} R_{n-1} \xrightarrow{f_{n-1}} \cdots \to R_1 \xrightarrow{f_1} M \to 0
$$

và đặt $K_0=M$, $K_i=\operatorname{Ker}f_i$, $i=1,\ldots,n-1$, $K_n=N$. Khi đó ta có các dãy khớp

$$
(9)\qquad 0\to K_i\to R_i\to K_{i-1}\to0,\qquad 1\leq i\leq n,
$$

mà với mỗi môđun trái trên $A$ là $P$, liên kết với chúng là các đồng cấu nối kết

$$
\operatorname{Ext}_A^m(P,K_{i-1})\to\operatorname{Ext}_A^{m+1}(P,K_i),
$$

$$
\operatorname{Ext}_A^m(K_i,P)\to\operatorname{Ext}_A^{m+1}(K_{i-1},P),
$$

do đó, bằng hợp thành của các *đồng cấu nối kết lặp*, liên kết với $(\mathcal{S})$

$$
\delta^m(P,\mathcal{S}):\operatorname{Ext}_A^m(P,M)\to\operatorname{Ext}_A^{m+n}(P,N)
$$

$$
\delta^m(\mathcal{S},P):\operatorname{Ext}_A^m(N,P)\to\operatorname{Ext}_A^{m+n}(M,P).
$$

#### Hệ quả 3 {#alg-x-s7-prop-5-cor-3 .statement}

Nếu $\theta\in\operatorname{Ext}_A^n(M,N)$ là lớp của dãy khớp $(\mathcal{S})$, ta có

$$
\delta^m(P,\mathcal{S})(\alpha)=\theta\circ\alpha,\qquad
\delta^m(\mathcal{S},P)(\beta)=(-1)^{mn+n(n+1)/2}\beta\circ\theta.
$$

Nếu $\theta_i\in\operatorname{Ext}_A^1(K_{i-1},K_i)$ là lớp liên kết với dãy khớp (9), thì theo Mệnh đề 5 ta có

$$
\delta^m(P,\mathcal{S})(\alpha)=\theta_n\circ\cdots\circ\theta_2\circ\theta_1\circ\alpha
$$

$$
\delta^m(\mathcal{S},P)(\beta)=(-1)^{(m+1)+\cdots+(m+n)}\beta\circ\theta_n\circ\cdots\circ\theta_1.
$$

Hơn nữa, theo Mệnh đề 3 (X, p. 118), ta có $\theta=\theta_n\circ\cdots\circ\theta_1$. Hệ quả suy ra ngay lập tức từ điều này, và từ quan hệ (E, III, p. 44)

$$
(m+1)+\cdots+(m+n)=mn+n(n+1)/2.
$$

#### Hệ quả 4 {#alg-x-s7-prop-5-cor-4 .statement}

Nếu mỗi môđun $R_i,\ i = 1, ..., n,$ là đơn ánh (resp. xạ ảnh), thì ánh xạ $\alpha \mapsto \theta \circ \alpha$ (resp. $\alpha \mapsto \alpha \circ \theta$) từ $\mathrm{Ext}_A^m(P, M)$ vào $\mathrm{Ext}_A^{m+n}(P, N)$ (resp. từ $\mathrm{Ext}_A^m(N, P)$ vào $\mathrm{Ext}_A^{m+n}(M, P)$) là song ánh với mọi $A$-môđun $P$ và mọi số nguyên $m > 0$.

Thật vậy, điều này suy ra từ Hệ quả 3 và các dãy khớp

$$
\mathrm{Ext}_A^{m+i-1}(P, R_i) \to \mathrm{Ext}_A^{m+i-1}(P, K_{i-1}) \to \mathrm{Ext}_A^{m+i}(P, K_i) \to \mathrm{Ext}_A^{m+i}(P, R_i)
$$
(resp. $\mathrm{Ext}_A^{m+i-1}(R_i, P) \to \mathrm{Ext}_A^{m+i-1}(K_i, P) \to \mathrm{Ext}_A^{m+i}(K_{i-1}, P) \to \mathrm{Ext}_A^{m+i}(R_i, P)$),
mà các hạng ở hai đầu bằng không theo giả thiết.

#### Nhận xét {#alg-x-s7-n6-rem-1 .statement}

Các định nghĩa và các mệnh đề từ No. 3 đến No. 6 áp dụng cho các $A$-môđun phải, được xét như các môđun trái trên vành đối $A^\circ$ của $A$.

### 7. Đồng cấu $\mathrm{Ext}_A(P, Q) \otimes \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M)$

Cho $M$ là một $A$-môđun trái, $P$ và $Q$ là hai $A$-môđun phải. Xét đồng cấu $\mathrm{Homgr}_A(L(P), L(Q)) \otimes_k (L(P) \otimes_A L(M)) \to L(Q) \otimes_A L(M)$ gán cho $f \otimes (x \otimes y)$ phần tử $f(x) \otimes y$. Theo X, p. 99, đó là một cấu xạ của các phức. Từ đó ta suy ra một ánh xạ tuyến tính phân bậc bậc 0 trên $k$

$$
H(\mathrm{Homgr}_A(L(P), L(Q))) \otimes_k \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M)
$$

rồi, nhờ đẳng cấu $\varphi(L(P), L(Q))$ của § 6 (X, p. 100, Định lý 1), một ánh xạ tuyến tính phân bậc bậc 0 trên $k$

(10)
$$
\mathrm{Ext}_A(P, Q) \otimes_k \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M),
$$
tương ứng với các ánh xạ song tuyến tính trên $k$

(11)
$$
c_{P, Q; M}: \mathrm{Ext}_A^n(P, Q) \times \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-n}^A(Q, M);
$$
Ảnh của cặp $(\alpha, \gamma)$ dưới $c_{P, Q; M}$ được gọi là tích hợp thành của $\alpha$ và $\gamma$ và được ký hiệu bởi $\alpha \circ \gamma$.

Theo phép dựng, $\alpha \circ \gamma$ thu được như sau: ta biểu diễn $\alpha$ bởi một cấu xạ của các phức $f : L(P) \to L(Q)(-n)$, $\gamma$ bởi một phần tử $z \in Z_m(L(P) \otimes_A L(M))$, và $\alpha \otimes \gamma$ là lớp của phần tử

$$
(f \otimes 1)(z) \in Z_m(L(Q)(-n) \otimes_A L(M)) = Z_{m-n}(L(Q) \otimes_A L(M)).
$$

Ví dụ, nếu $\alpha \in \mathrm{Hom}_A(P, Q)$, thì $\alpha \circ \gamma = \mathrm{Tor}(\alpha, 1)(\gamma)$.

#### Nhận xét 1 {#alg-x-s7-n7-rem-1 .statement}

Nếu ta dùng các đẳng cấu $\psi$ của X, p. 69, thì cũng có thể định nghĩa tích hợp thành bằng biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Ext}_A^n(P, Q) \times \mathrm{Tor}_m^A(P, M) & \xrightarrow{c_{P,Q;M}} & \mathrm{Tor}_{m-n}^A(Q, M) \\
\bar{a}_{P,Q} \times \psi_{P(M)} \downarrow & & \downarrow \psi_{Q(M)} \\
H^n(\mathrm{Homgr}_A(L(P), L(Q))) \times H_m(L(P) \otimes_A M) & \longrightarrow & H_{m-n}(L(Q) \otimes_A M);
\end{array}
$$

nói cách khác, biểu diễn $\alpha$ bởi một cấu xạ $f$ từ $L(P)$ đến $L(Q) (-n)$, $\gamma$ bởi một chu trình $x \in L_m(P) \otimes_A M$, và $\alpha \circ \gamma$ là lớp của chu trình

$$
(f_m \otimes 1_M)(x) \in L_{m-n}(Q) \otimes_A M.
$$

#### Nhận xét 2 {#alg-x-s7-n7-rem-2 .statement}

Ta cũng có thể dùng các giải quyết $l(P)$ và $l(Q)$.

Tương tự, nếu $N$ là một $A$-môđun trái thứ hai, ta định nghĩa một tích hợp thành $(\mu, \gamma) \mapsto \mu \circ \gamma$ được ký hiệu là

$$
c_{P:M,N}: \mathrm{Ext}_A^r(M, N) \times \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-r}^A(P, N)
$$

bởi biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Ext}_A^r(M, N) \times \mathrm{Tor}_m^A(P, M) & \xrightarrow{c_{P:M,N}} & \mathrm{Tor}_{m-r}^A(P, N) \\
1 \times \sigma_{P,M,r} \downarrow & & \downarrow \sigma_{P,N,m-r} \\
\mathrm{Ext}_A^r(M^\circ, N^\circ) \times \mathrm{Tor}_m^{A^\circ}(M^\circ, P^\circ) & \xrightarrow{c_{M^\circ,N^\circ,P^\circ}} & \mathrm{Tor}_{m-r}^{A^\circ}(N^\circ, P^\circ)
\end{array}
$$

trong đó $\sigma$ ký hiệu các đẳng cấu giao hoán (X, p. 71).

Nếu $\mu \in \mathrm{Ext}_A^r(M, N)$ là lớp của cấu xạ $g : L(M) \to L(N) (-r)$, và nếu $\gamma \in \mathrm{Tor}_m^A(P, M)$ là lớp của chu trình $z = \sum z_{ij}$, trong đó $z_{ij} \in L_i(P) \otimes_A L_j(M)$, thì do đó $\mu \circ \gamma$ là lớp của chu trình $\sum (-1)^{ir} (1 \otimes g)(z_{ij})$.

Ta cũng có thể biểu diễn $\gamma$ bởi một chu trình $y \in P \otimes L_m(M)$, và $\mu \circ \gamma$ là lớp của chu trình $(1 \otimes g)(y) \in P \otimes L_{m-r}(M)$.

#### Mệnh đề 6 {#alg-x-s7-prop-6 .statement}

Cho $K, M, N$ là các $A$-môđun trái, $P, Q, R$ là các $A$-môđun phải,
$\alpha \in \mathrm{Ext}_A^n(P, Q)$, $\beta \in \mathrm{Ext}_A^p(Q, R)$, $\lambda \in \mathrm{Ext}_A^r(K, M)$, $\mu \in \mathrm{Ext}_A^s(M, N)$, $\gamma \in \mathrm{Tor}_m^A(P, K)$.
Khi đó
(13) $$ (\beta \circ \alpha) \circ \gamma = \beta \circ (\alpha \circ \gamma) \quad \text{trong} \quad \mathrm{Tor}_{m-p-n}^A(R, K), $$
(14) $$ (\mu \circ \lambda) \circ \gamma = \mu \circ (\lambda \circ \gamma) \quad \text{trong} \quad \mathrm{Tor}_{n-r-s}^A(P, N), $$
(15) $$ \alpha \circ (\lambda \circ \gamma) = (-1)^{nr} \lambda \circ (\alpha \circ \gamma) \quad \text{trong} \quad \mathrm{Tor}_{m-p-r}^A(Q, M). $$

Các công thức (13) và (14) theo ngay lập tức từ các định nghĩa. Hãy chứng minh (15).
Cho $z = \sum z_{ij}$, $z_{ij} \in L_i(P) \otimes L_j(K)$ là một chu trình biểu diễn $\gamma$, $f : L(P) \to L(Q) (-n)$ và $g : L(K) \to L(M) (-r)$ là các cấu xạ biểu diễn $\alpha$ và $\lambda$. Khi đó $\lambda \circ (\alpha \circ \gamma)$ là lớp của $\sum (-1)^{(i-n)r} (f \otimes g)(z_{ij})$ và $\alpha \circ (\lambda \circ \gamma)$ là lớp của

$$
\sum (-1)^{ir} (f \otimes g)(z_{ij}), \quad \text{do đó (15)}.
$$

### 8. Các tích hợp thành và các đồng cấu nối của các tích xoắn

#### Mệnh đề 7 {#alg-x-s7-prop-7 .statement}

a) Cho

(ε)
$$
0 \to P' \xrightarrow{f} P \xrightarrow{g} P'' \to 0
$$
là một dãy khớp của các $A$-môđun phải, $\theta \in \mathrm{Ext}_A^1(P'', P')$ là lớp liên kết, $M$ là một $A$-môđun trái. Đồng cấu nối
$$
\delta_n(\mathcal{E}, M) : \mathrm{Tor}_n^A(P'', M) \to \mathrm{Tor}_{n-1}^A(P', M) \text{ là ánh xạ } \gamma \mapsto \theta \circ \gamma .
$$

b) Let

(ε₁)
$$
0 \to M' \to M \to M'' \to 0
$$
là một dãy khớp của các $A$-môđun trái, $\theta_1 \in \mathrm{Ext}_A^1(M'', M')$ lớp liên kết, $P$ một $A$-môđun phải. Đồng cấu nối
$$
\delta_n(P, \mathcal{E}_1) : \mathrm{Tor}_n^A(P, M'') \to \mathrm{Tor}_{n-1}^A(P, M') \text{ là ánh xạ } \gamma \mapsto \theta_1 \circ \gamma .
$$
Cho $\gamma \in \mathrm{Tor}_n^A(P'', M)$ là lớp của một chu trình $z'' \in \dot{Z}_n(L(P'') \otimes_A L(M))$, và
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & P' & \xrightarrow{f} & P & \xrightarrow{g} & P'' & \longrightarrow & 0 \\
& & \uparrow u_1 & & \uparrow u_0 & & \uparrow 1 & & \\
L_1(P'') & \xrightarrow{d_1} & L_0(P'') & \xrightarrow{p_0''} & P'' & \longrightarrow & 0
\end{array}
$$
là một biểu đồ giao hoán. Ta sẽ ký hiệu bởi $p' : L(P') \to P'$ và $p'' : L(P'') \to P''$ các cấu xạ chính tắc của phức. Theo định nghĩa, $\delta(\gamma) \in \mathrm{Tor}_{n-1}^A(P', M)$ thu được như sau: ta chọn $x \in P \otimes L_n(M)$ sao cho $(g \otimes 1)(x) = (p'' \otimes 1)(z'')$ và $\delta(\gamma)$ là lớp của các chu trình $z' \in Z_{n-1}(L(P') \otimes L(M))$ sao cho
$$
(f \otimes 1)(p' \otimes 1)(z') = (1 \otimes d_n)(x) .
$$
Với $0 \leq i \leq n$, gọi $z''_i$ là thành phần của $z''$ trong $L_i(P'') \otimes L_{n-i}(M)$; ta có
$$
0 = Dz'' = \sum_i (d_i \otimes 1 + (-1)^i \otimes d_{n-i})(z''_i) ,
$$
do đó $(d_i \otimes 1)(z''_i) = (-1)^i \otimes d_{n-i+1}(z''_{i-1})$ và đặc biệt
$$
(d_1 \otimes 1)(z''_1) = -1 \otimes d_n(z''_0) .
$$
Khi đó ta chọn $x = (u_0 \otimes 1)(z''_0)$: thật vậy ta có
$$
(g \otimes 1)(x) = (p_0'' \otimes 1)(z''_0) = (p'' \otimes 1)(z'') .
$$
Vì
$$
(1 \otimes d_n)(x) = (u_0 \otimes 1)(1 \otimes d_n)(z''_0) = - (u_0 \otimes 1)(d_1 \otimes 1)(z''_1)
= - (f \otimes 1)(u_1 \otimes 1)(z''_1) ,
$$

suy ra $\delta(\gamma)$ là lớp của các chu trình $z' \in Z_{n-1}(L(P') \otimes_A L(M))$ sao cho $(p' \otimes 1)(z') = - (u_1 \otimes 1)(z''_1)$. Nhưng, theo định nghĩa, lớp $\theta$ tương ứng qua đẳng cấu $\mathrm{Ext}_A^1(P'', P') \to H^1(\mathrm{Homgr}_A(L(P''), P'))$ với lớp của cấu xạ $f : L(P'')(1) \to P'$ được xác định bởi $- u_1$, và tích $\theta \circ \gamma$ là lớp của các chu trình
$$
\overline{z}' \in Z_{n-1}(L(P') \otimes_A L(M)) \quad \text{sao cho} \quad (p \otimes 1)(\overline{z}') = f(z'') = - (u_1 \otimes 1)(z''_1),
$$
điều này hoàn tất chứng minh của a). Mệnh đề b) suy ra từ a) nhờ các đẳng cấu giao hoán.

#### Hệ quả 1 {#alg-x-s7-prop-7-cor-1 .statement}

*Cho* $0 \to P' \to P \to P'' \to 0$ *là một dãy khớp của các* $A$-*môđun phải*, $0 \to M' \to M \to M'' \to 0$ *là một dãy khớp của các* $A$-*môđun trái*. *Khi đó các hợp thành của các đồng cấu nối*
$$
\mathrm{Tor}_n^A(P'', M'') \to \mathrm{Tor}_{n-1}^A(P'', M') \to \mathrm{Tor}_{n-2}^A(P', M')
$$
*và*
$$
\mathrm{Tor}_n^A(P'', M'') \to \mathrm{Tor}_{n-1}^A(P', M'') \to \mathrm{Tor}_{n-2}^A(P', M')
$$
*là đối nhau*.

Thật vậy, nếu $\theta$ và $\theta_1$ là các lớp liên kết với các dãy khớp đã cho, và nếu $\gamma \in \mathrm{Tor}_n^A(P'', M'')$, thì các ảnh của $\gamma$ lần lượt là $\theta \circ (\theta_1 \circ \gamma)$ và $\theta_1 \circ (\theta \circ \gamma)$, do đó đối nhau theo mệnh đề 6.

Ta nhắc lại các ký hiệu của X, p. 127 và xét dãy $(\mathscr{S})$ các $A$-môđun trái cùng các đồng cấu nối liên kết với các dãy khớp (9)
$$
\mathrm{Tor}_m^A(P, K_{i-1}) \to \mathrm{Tor}_{m-1}^A(P, K_i);
$$
ta suy ra từ đó, bằng hợp thành của các *đồng cấu nối lặp*
$$
\hat{\partial}_m(P, \mathscr{S}) : \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-n}^A(P, N).
$$
Khi đó theo mệnh đề 7 và mệnh đề 3 của X, p. 118 :

#### Hệ quả 2 {#alg-x-s7-prop-7-cor-2 .statement}

Nếu $\theta \in \mathrm{Ext}_A^n(M, N)$ là lớp liên kết với dãy khớp $(\mathscr{S})$, ta có $\hat{\partial}_m(P, \mathscr{S})(\alpha) = \theta \circ \alpha$ với mọi $\alpha \in \mathrm{Tor}_m^A(P, M)$.

#### Hệ quả 3 {#alg-x-s7-prop-7-cor-3 .statement}

Nếu tất cả các môđun $R_i$, $i = 1, ..., n$, đều phẳng, thì ánh xạ $\alpha \mapsto \theta \circ \alpha$ từ $\mathrm{Tor}_{m+n}^A(P, M)$ vào $\mathrm{Tor}_m^A(P, N)$ là song ánh đối với mọi A-môđun phải $P$ và mọi số nguyên $m > 0$.

Điều này suy ra từ Hệ quả 2 và các dãy khớp

$$
\mathrm{Tor}_{m+n-i+1}^A(P, R_i) \to \mathrm{Tor}_{m+n-i+1}^A(P, K_{i-1}) \xrightarrow{\hat{\partial}} \mathrm{Tor}_{m+n-i}^A(P, K_i) \to \mathrm{Tor}_{m+n-i}^A(P, R_i)
$$

trong đó các hạng ở hai đầu bằng không theo giả thiết.

Tương tự, nếu

$$(\mathcal{S}_1)$$
$$0 \to Q \to S_n \to S_{n-1} \to \ldots \to S_1 \to P \to 0$$

là một dãy khớp các A-môđun phải, và $M$ là một A-môđun trái, ta định nghĩa các *đồng cấu nối lặp*

$$\partial^m(\mathcal{S}_1, M) : \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-n}^A(Q, M)$$

và ta có:

#### Hệ quả 4 {#alg-x-s7-prop-7-cor-4 .statement}

Nếu $\theta_1 \in \mathrm{Ext}_A^n(P, Q)$ là lớp liên kết với dãy khớp $(\mathcal{S}_1)$, thì ta có $\partial^m(\mathcal{S}_1, M)(\alpha) = \theta_1 \circ \alpha$ với mọi $\alpha \in \mathrm{Tor}_m^A(P, M)$.

### 9. Tính các tích hợp thành bằng cách dịch chuyển các phân giải

Cho

(16)
$$0 \to M \xrightarrow{\iota} K_n \to K_{n-1} \to \ldots \to K_1 \xrightarrow{\rho} M' \to 0$$

là một dãy khớp các A-môđun trái và $\theta \in \mathrm{Ext}_A^n(M', M)$ là lớp liên kết.

Cho $a : (R, d) \to M$ là một phân giải trái của $M$; do đó có một dãy khớp

$$ \to R_k \xrightarrow{d_k} R_{k-1} \to \ldots \xrightarrow{d_1} R_0 \xrightarrow{a_0} M \to 0.$$

và, bằng cách dịch chuyển n lần (X, p. 26), một dãy khớp

(17)
$$\to R_k \xrightarrow{(-1)^n d_k} R_{k-1} \to \ldots \xrightarrow{(-1)^n d_1} R_0 \xrightarrow{(-1)^n a_0} M \to 0.$$

Ta suy ra từ (16) và (17) một dãy khớp

$$\to R_k \xrightarrow{(-1)^n d_k} R_{k-1} \to \ldots \xrightarrow{(-1)^n d_1} R_0 \xrightarrow{(-1)^n f \circ a_0} K_n \to K_{n-1} \to \ldots \to K_1 \to M' \to 0$$

do đó thu được một phân giải $R'$ của $M'$; gọi $\varphi : R' \to R(-n)$ là cấu xạ sao cho $\varphi_k = 1_{R_{k-n}}$ với $k \geq n$.

Nếu $N$ là một A-môđun trái và $P$ là một A-môđun phải, thì do đó ta có các ánh xạ

$$\mathrm{H}(1_P \otimes \varphi) : \mathrm{H}(P \otimes_A R') \to \mathrm{H}(P \otimes_A R)(-n)$$
$$\mathrm{H}(\mathrm{Homgr}_A(\varphi, 1_N)) : \mathrm{H}(\mathrm{Homgr}_A(R, N))(n) \to \mathrm{H}(\mathrm{Homgr}_A(R', N)).$$

Cho $k$ là một số nguyên.

#### Mệnh đề 8 {#alg-x-s7-prop-8 .statement}

*a)* Biểu đồ sau đây, trong đó $h_\theta(\alpha) = \theta \circ \alpha$, là giao hoán

$$
\begin{array}{ccc}
\mathrm{Tor}_{k+n}^A(P, M') & \xrightarrow{h_\theta} & \mathrm{Tor}_k^A(P, M) \\
\psi_{k+n}(P, R') \downarrow & & \downarrow \psi_k(P, R) \\
\mathrm{H}_{k+n}(P \otimes_A R') & \xrightarrow{H_{k+n}(1 \otimes \varphi)} & \mathrm{H}_k(P \otimes_A R)
\end{array}
$$

b) Biểu đồ sau đây, trong đó $\delta_\theta(\beta) = \beta \circ \theta$, là giao hoán

$$
\begin{array}{ccc}
H^k(\mathrm{Homgr}_A(R, N)) & \xrightarrow{H^{k+n}(\mathrm{Homgr}_A(\varphi, 1))} & H^{k+n}(\mathrm{Homgr}_A(R', N)) \\
\varphi^k(R, N) \downarrow & & \varphi^{k+n}(R', N) \downarrow \\
\mathrm{Ext}_A^k(M, N) & \xrightarrow{\delta_\theta} & \mathrm{Ext}_A^{k+n}(M', N).
\end{array}
$$

Cho $\alpha : L(M) \to R$ là một cấu xạ của các phức sao cho $a \circ \alpha = p_M$ và cho

$$
\begin{array}{ccccccccc}
L_n(M') & \longrightarrow & L_{n-1}(M') & \longrightarrow & \ldots & \longrightarrow & L_0(M') & \longrightarrow & M' \longrightarrow 0 \\
u_n \downarrow & & u_{n-1} \downarrow & & & & u_0 \downarrow & & 1 \downarrow \\
0 & \longrightarrow & M & \xrightarrow{f} & K_n & \longrightarrow & \ldots & \longrightarrow & K_1 \longrightarrow M' \longrightarrow 0
\end{array}
$$

một biểu đồ giao hoán, ta hãy chọn một đồng cấu $v_n : L_n(M') \to L_0(M)$ sao cho $p_M \circ v_n = (-1)^n u_n$; theo *X*, p. 47, Mệnh đề 1, a), $v_n$ mở rộng thành một cấu xạ của các phức $v : L(M') \to L(M)$ $(-n)$, và $\theta$ là ảnh, dưới đẳng cấu chính tắc $H^n(\mathrm{Homgr}_A(L(M'), L(M))) \to \mathrm{Ext}_A^n(M', M)$, của lớp của $v$ (*X*, p. 117, Nhận xét 1). Ta định nghĩa một cấu xạ của các phức $\beta : L(M') \to R'$ bởi $\beta_p = u_p$ với $p \leq n - 1$, $\beta_p = \alpha_{p-n} \circ v_p$ với $p \geq n$, và ta có

$$
\varphi \circ \beta = \alpha(-n) \circ v.
$$

Mặt khác, theo định nghĩa của các ánh xạ $\varphi$ và $\psi$, ta có

$$
\begin{aligned}
& \psi_k(P, R) = H_k(p_P \otimes \alpha), \quad \varphi^k(R, N) = H^k(\mathrm{Homgr}_A(\alpha, e_N)), \\
& \psi_{k+n}(P, R') = H_{k+n}(p_P \otimes \beta), \quad \varphi^{k+n}(R', \tilde{N}) = H^{k+n}(\mathrm{Homgr}_A(\beta, e_N)).
\end{aligned}
$$

Sau cùng, theo định nghĩa của tích hợp thành, ta có

$$
h_\theta = H(1_{L(P)} \otimes v), \quad \delta_\theta = H(\mathrm{Homgr}_A(v, 1_{L(N)})) .
$$

Do đó, ta có các đẳng thức

$$
\begin{aligned}
\psi_k(P, R) \circ h_\theta &= H_k(p_P \otimes \alpha) \circ H_k(1_{L(P)} \otimes v) = H_k(p_P \otimes (\alpha \circ v)) = H_{k+n}(p_P \otimes (\varphi \circ \beta)) \\
&= H_{k+n}(1 \otimes \varphi) \circ H_{k+n}(p_P \circ \beta) = H_{k+n}(1 \otimes \varphi) \circ \psi_{k+n}(P, R'),
\end{aligned}
$$

từ đó suy ra a); chứng minh của b) là tương tự.

#### Nhận xét {#alg-x-s7-n9-rem-1 .statement}

Nhờ các đẳng cấu giao hoán, từ a) ta suy ra một mệnh đề tương tự trong trường hợp một dãy khớp (16) các A-môđun phải.

Cho $b : M' \to E'$ là một phân giải phải của $M'$; do đó ta có một dãy khớp

$$
0 \to M' \xrightarrow{b^0} {E'}^0 \xrightarrow{\delta^0} {E'}^1 \to \ldots \to {E'}^k \xrightarrow{\delta^k} {E'}^{k+1}
$$

tương ứng với một phân giải phải $E$ của $M$; gọi $\sigma : E'(n) \to E$ là cấu xạ sao cho $\sigma^k = 1_{{E'}^{k-n}}$ với $k \geq n$. Do đó ta có các đồng cấu

$$
H(\mathrm{Homgr}_A(1_N, \sigma)) : H(\mathrm{Homgr}_A(N, E'))(n) \to H(\mathrm{Homgr}_A(N, E)) .
$$

#### Mệnh đề 9 {#alg-x-s7-prop-9 .statement}

*Biểu đồ sau đây, trong đó $\gamma_\theta(\alpha) = \theta \circ \alpha$, là giao hoán*:

$$
\begin{array}{ccc}
H^k(\mathrm{Homgr}_A(N, E')) & \xrightarrow{H^{k+n}(\mathrm{Homgr}_A(1_N, \sigma))} & H^{k+n}(\mathrm{Homgr}_A(N, E)) \\
\downarrow \varphi^k(N, E') & & \downarrow \varphi^{k+n}(N, E) \\
\mathrm{Ext}_A^k(N, M') & \xrightarrow{\gamma_\theta} & \mathrm{Ext}_A^{k+n}(N, M)
\end{array}
$$

Điều này được chứng minh theo cách tương tự như Mệnh đề 8.

## Bài tập {#alg-x-s7-exercises}
Xem [bài tập của § 7](exercises/s7/).
