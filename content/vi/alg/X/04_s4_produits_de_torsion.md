---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 4
section_title: Produits de torsion
lang: vi
source: alg-x-fr
book_pages: A X.61-A X.81, A X.184-A X.186
pdf_pages: 0067-0087, 0190-0192
extraction: ocr
subsections:
    - "no": 1
      title: Produit tensoriel de deux complexes
      page: 61
      pdf_page: 67
    - "no": 2
      title: Produits tensoriels et homotopie
      page: 64
      pdf_page: 70
    - "no": 3
      title: Produit tensoriel par un complexe plat borné à droite
      page: 66
      pdf_page: 72
    - "no": 4
      title: Définition et premières propriétés du produit de torsion
      page: 67
      pdf_page: 73
    - "no": 5
      title: Les homomorphismes de liaison et les suites exactes
      page: 71
      pdf_page: 77
    - "no": 6
      title: Modules plats et produits de torsion
      page: 74
      pdf_page: 80
    - "no": 7
      title: ' **Formule de Künneth**'
      page: 76
      pdf_page: 82
    - "no": 8
      title: Complexes bornés et plats sur un anneau noethérien
      page: 79
      pdf_page: 85
    - "no": 9
      title: Généralisation aux complexes de multimodules
      page: 80
      pdf_page: 86
statements: 39
exercises: 9
content_sha256: 289e038ff5c0105b1eca66c91897f10ed6b2b2ab059286647381a2251c8ff78c
translated_from: content/en-mt/alg/X/04_s4_produits_de_torsion.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 7cd64a7ad3c3af38edd96851d0e24b924bbb8ef9af1e92be9cdb84f739041489
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5-mini
translation_run: translate-vi-577277fa
glossary_version: 34
glossary_terms_sha256: df898024851cef759224c0328296135e89aac7d29a936011bd046358b91c2ede
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. Tích xoắn

*Trong các mục 4 đến 8, ta ký hiệu $k$ là một vành giao hoán, và $A$ là một đại số kết hợp có đơn vị trên $k$. Vai trò của $k$ là phụ trợ; ta chủ yếu xét ba trường hợp đặc biệt sau:*

a) ta xét một vành tùy ý $A$, đặt $k=\mathbf{Z}$ và trang bị cho $A$ cấu trúc tự nhiên của một $\mathbf{Z}$-đại số,

b) ta xét một vành tùy ý $A$, lấy tâm của $A$ làm $k$,

c) ta xét một vành giao hoán $A$ và lấy $k=A$.

### 1. Tích tenxơ của hai phức

Cho $(C,d)$ là một phức của các môđun phải $A$ và $(C',d')$ là một phức của các môđun trái $A$.

Ta trang bị cho môđun $k$ $C\otimes_A C'$ phép phân bậc sao cho

$$
(C\otimes_A C')_n=\sum_{p+q=n}(C_p\otimes C'_q)
$$

và gọi $D$ là tự đồng cấu $k$-tuyến tính duy nhất bậc $(-1)$ của $C\otimes_A C'$ sao cho

$$
\tag{1}
D(x\otimes x')=dx\otimes x'+(-1)^p x\otimes d'x',
\qquad x\in C_p,\ y\in C'_q,\ p,\ q\in\mathbf{Z}.
$$

Ta có $D\circ D=0$ vì, với các ký hiệu của (1)

$$
D^2(x\otimes x')=ddx\otimes x'+(-1)^{p-1}dx\otimes d'x'+(-1)^pdx\otimes d'x'-x\otimes d'd'x'.
$$

Phức của các môđun $k$ $(C\otimes_A C',D)$ được gọi là *phức tích tenxơ* của các phức $(C,d)$ và $(C',d')$.

#### Nhận xét 1 {#alg-x-s4-n1-rem-1 .statement}

Khi $C'$ thu gọn thành $C'_0=M$, thì $(C\otimes_A C')_n=C_n\otimes_A M$ và $D=d\otimes 1_M$; ví dụ $C\otimes_A A_s$ được đồng nhất một cách tự nhiên với $C$. Tương tự, khi $C$ thu gọn thành $C_0=P$, thì $(C\otimes_A C')_n=P\otimes_A C'_n$ và $D=1_P\otimes d$.

#### Nhận xét 2 {#alg-x-s4-n1-rem-2 .statement}

Với mọi số nguyên $r$, ta có $(C\otimes_A C')(r)=C(r)\otimes_A C'$, nhưng nói chung $(C\otimes_A C')(r)$ và $C\otimes_A C'(r)$ không có cùng vi phân.

Cho $p, q$ là hai số nguyên, $x \in Z_p(C), x' \in Z_q(C')$; khi đó phần tử $x \otimes x'$ của $C_p \otimes C'_q$ thuộc về $Z_{p+q}(C \otimes C')$ theo (1); hơn nữa, nếu $y \in C_{p+1}, y' \in C'_{q+1}$, ta có
$$
(x + dy) \otimes (x' + d'y') = x \otimes x' + D(y \otimes x' + (-1)^p (x + dy) \otimes y');
$$
bằng cách chuyển qua các thương, ta suy ra một ánh xạ $k$-tuyến tính, được gọi là chính tắc
$$
\gamma_{p,q}(C, C') : H_p(C) \otimes_A H_q(C') \to H_{p+q}(C \otimes_A C');
$$
nếu ta trang bị cho $H(C) \otimes_A H(C')$ phép phân bậc sao cho
$$
(H(C) \otimes H(C'))_n = \sum_{p+q=n} H_p(C) \otimes_A H_q(C'),
$$
các $\gamma_{p,q}$ định nghĩa một ánh xạ $k$-tuyến tính phân bậc bậc 0
$$
\gamma(C, C') : H(C) \otimes_A H(C') \to H(C \otimes_A C').
$$
Mệnh đề 6 của II, p. 59, có thể được phát biểu lại như sau:

#### Mệnh đề 1 {#alg-x-s4-prop-1 .statement}

*Nếu các phức $C$ và $C'$ bằng không ở bên phải, thì $C \otimes_A C'$ bằng không ở bên phải và ánh xạ tuyến tính trên $k$ chính tắc*
$$
\gamma_{0,0}(C, C') : H_0(C) \otimes_A H_0(C') \to H_0(C \otimes_A C')
$$
*là song ánh*.

Cho $u : (C, d) \to (C_1, d_1)$ là một cấu xạ của các phức của các $A$-môđun phải và $u' : (C', d') \to (C'_1, d'_1)$ là một cấu xạ của các phức của các $A$-môđun trái; khi đó $u \otimes u' : C \otimes_A C' \to C_1 \otimes_A C'_1$ là một cấu xạ của các phức của các $k$-môđun; thật vậy, nó là phân bậc bậc 0, và nếu ký hiệu $D$ và $D_1$ là các vi phân của $C \otimes C'$ và $C_1 \otimes C'_1$, ta có với $p, q \in \mathbf{Z}, x \in C_p, x' \in C'_q$,
$$
(u \otimes u') (D(x \otimes x')) = u(dx) \otimes u'(x') + (-1)^p u(x) \otimes u'(d'x') =
= d_1 u(x) \otimes u'(x') + (-1)^p u(x) \otimes d'_1 u'(x') = D_1(u(x) \otimes u(x')) .
$$
Ngoài ra biểu đồ sau là giao hoán :
$$
\begin{array}{ccc}
H(C) \otimes_A H(C') & \xrightarrow{\gamma(C, C')} & H(C \otimes_A C') \\
H(u) \otimes H(u') \downarrow & & \downarrow H(u \otimes u') \\
H(C_1) \otimes_A H(C'_1) & \xrightarrow{\gamma(C_1, C'_1)} & H(C_1 \otimes_A C'_1)
\end{array}
$$

Gọi $A^\circ$ là $k$-đại số đối của $A$, $C^\circ$ (tương ứng ${C'}^\circ$) là phức $C$ (tương ứng $C'$) được xem như một phức của các $A^\circ$-môđun trái (tương ứng phải). Ký hiệu bởi
$$
\sigma(C, C') : C \otimes_A C' \to {C'}^\circ \otimes_{A^\circ} C^\circ
$$
ánh xạ tuyến tính trên $k$ phân bậc duy nhất bậc 0 sao cho, với $x \in C_p, x' \in C'_q, p, q \in \mathbf{Z}$, ta có
$$
\sigma(C, C') (x \otimes x') = (-1)^{pq} x' \otimes x .
$$

#### Mệnh đề 2 {#alg-x-s4-prop-2 .statement}

Ánh xạ $\sigma(C, C') : C \otimes_A C' \to {C'}^\circ \otimes_A C^\circ$ là một đẳng cấu của các phức của $k$-môđun, mà đẳng cấu ngược là $\sigma({C'}^\circ, C^\circ)$.

Vì các ánh xạ $\sigma(C, C')$ và $\sigma({C'}^\circ, C^\circ)$ ngược nhau, chỉ cần chứng minh rằng $\sigma(C, C')$ là một cấu xạ của các phức. Bây giờ, với
$$
x \in C_p = C_p^\circ, \quad x' \in C'_q = C_{q'}^\circ, \quad p, q \in \mathbf{Z},
$$
ta có, ký hiệu $D'$ là vi phân của $C' \otimes_{A^\circ} C$,
$$
\begin{align*}
\sigma(C, C') \circ D(x \otimes x') &= \sigma(C, C') (dx \otimes x' + (-1)^p x \otimes d'x') = \\
&= (-1)^{(p+1)q} x' \otimes dx + (-1)^{p+p(q+1)} d'x' \otimes x = (-1)^{pq} d'x' \otimes x + (-1)^{pq+q} x' \otimes dx \\
&= (-1)^{pq} D'(x' \otimes x) = D^\circ \circ \sigma(C, C') (x \otimes x');
\end{align*}
$$
điều này cho $\sigma(C, C') \circ D = D^\circ \circ \sigma(C, C')$, do đó thu được mệnh đề cần tìm.

Đẳng cấu $\sigma(C, C') : C \otimes_A C' \to {C'}^\circ \otimes_A C^\circ$ được gọi là *đẳng cấu giao hoán* của tích tenxơ của các phức $C$ và $C'$.

Nếu $u : C \to C_1$ và $v : C' \to C'_1$ là hai cấu xạ của các phức như trên, ta có một biểu đồ giao hoán :

$$
\begin{array}{ccc}
C \otimes_A C' & \xrightarrow{\sigma(C, C')} & {C'}^\circ \otimes_A C^\circ \\
u \otimes u' \downarrow & & \downarrow u' \otimes u \\
C_1 \otimes_A C'_1 & \xrightarrow{\sigma(C_1, C'_1)} & C'_1{}^\circ \otimes_A C_1^\circ.
\end{array}
$$

Giả sử ở cuối số này rằng vành $A$ là *giao hoán* (*xem* No. 9 cho trường hợp tổng quát).

Cho $C, C', C''$ là ba phức của các $A$-môđun; đồng cấu chính tắc của các $A$-môđun (III, p. 64)
$$
\varphi : (C \otimes_A C') \otimes_A C'' \to C \otimes_A (C' \otimes_A C'')
$$
là một *đẳng cấu của các phức*, như được kiểm chứng ngay lập tức bằng cách sử dụng các định nghĩa.

Nói chung hơn, cho $(C^{(i)}, d^{(i)})_{i \in I}$ là một *họ các phức* của các $A$-môđun, trong đó tập hợp $I$ là *hữu hạn và được sắp thứ tự toàn phần*; ta sẽ đồng nhất $I$ với khoảng $[1, r]$ của $\mathbf{N}$ để đơn giản hóa ký hiệu. Ta trang bị cho $A$-môđun $C = \bigotimes_{i=1}^r C^{(i)}$ cấu trúc phân bậc sao cho
$$
C_n = \sum_{p_1 + p_2 + \cdots + p_r = n} (C^{(1)})_{p_1} \otimes (C^{(2)})_{p_2} \otimes \cdots \otimes (C^{(r)})_{p_r},
$$
và định nghĩa một tự đồng cấu $A$ phân bậc bậc $(-1)$ của $C$ bởi
$$
D(x_1 \otimes \ldots \otimes x_r) = \sum_{j=1}^r (-1)^{p_1 + \cdots + p_{j-1}} x_1 \otimes \ldots \otimes x_{j-1} \otimes d_j x_j \otimes x_{j+1} \otimes \ldots \otimes x_r
$$
trong đó $x_i \in (C^{(i)})_{p_i}$ với $i = 1, \ldots, n$. Khi đó $(C, D)$ là một phức của các $A$-môđun được gọi là phức tích tenxơ của họ $(C_i, d_i)$. Với mọi dãy tăng ngặt $r_0, ..., r_k$ của $[0, r]$ sao cho $r_0 = 0,\ r_k = r$, đẳng cấu chính tắc của tính kết hợp

$$
\bigotimes_{j=0}^{k-1} \left( \bigotimes_{i=r_j+1}^{r_{j+1}} C^{(i)} \right) \to \bigotimes_{i=1}^r C^{(i)}
$$

là một đẳng cấu của các phức.

Ta định nghĩa như trên một đồng cấu $A$ phân bậc bậc 0

$$
\gamma((C^{(i)})) : \bigotimes_{i \in I} H(C^{(i)}) \to H \left( \bigotimes_{i \in I} C^{(i)} \right)
$$

#### Nhận xét 3 {#alg-x-s4-n1-rem-3 .statement}

Có thể định nghĩa tích tenxơ của một họ hữu hạn các phức mà không trang bị cho tập hợp chỉ số một thứ tự toàn phần (X, p. 185, Bài tập 3).

#### Nhận xét 4 {#alg-x-s4-n1-rem-4 .statement}

Giả sử mỗi $C^{(i)}$ được trang bị một cấu trúc đại số phân bậc tương thích với cấu trúc phân bậc của nó và sao cho các $d^{(i)}$ là các phản đạo hàm (III, p. 117). Khi đó ta trang bị $\bigotimes_{i \in I} C^{(i)}$ cấu trúc đại số tích tenxơ phân bậc trái của các cấu trúc đã cho (III, p. 49). Khi đó $D$ là một phản đạo hàm. Thật vậy, sử dụng tính kết hợp của tích tenxơ, ta có thể giả sử rằng $I = \{1, 2\}$; khi đó cho $p_1,\ q_1,\ p_2,\ q_2 \in \mathbf{Z},\ x_1 \in (C^{(1)})_{p_1},\ y_1 \in (C^{(1)})_{q_1},\ x_2 \in (C^{(2)})_{p_2},\ y_2 \in (C^{(2)})_{q_2}$; ta có

$$
(D(x_1 \otimes x_2))(y_1 \otimes y_2) + (-1)^{p_1+p_2} (x_1 \otimes x_2)(D(y_1 \otimes y_2)) =
$$
$$
= (dx_1 \otimes x_2 + (-1)^{p_1} x_1 \otimes dx_2)(y_1 \otimes y_2) +
$$
$$
+ (-1)^{p_1+p_2} (x_1 \otimes x_2)(dy_1 \otimes y_2 + (-1)^{q_1} y_1 \otimes dy_2) =
$$
$$
= (-1)^{p_2 q_1} (dx_1) y_1 \otimes x_2 y_2 + (-1)^{p_1+(p_2-1)q_1} x_1 y_1 \otimes (dx_2) y_2 +
$$
$$
+ (-1)^{p_1+p_2+p_2(q_1-1)} x_1 dy_1 \otimes x_2 y_2 + (-1)^{p_1+p_2+q_1+p_2 q_1} x_1 y_1 \otimes x_2 dy_2
$$
$$
= (-1)^{p_2 q_1} [(dx_1) y_1 + (-1)^{p_1} x_1 dy_1] \otimes x_2 y_2 +
$$
$$
+ (-1)^{p_1+q_1+p_2 q_1} x_1 y_1 \otimes ((dx_2) y_2 + (-1)^{p_2} x_2 dy_2)
$$
$$
= (-1)^{p_2 q_1} [d(x_1 y_1) \otimes x_2 y_2 + (-1)^{p_1+q_1} x_1 y_1 \otimes d(x_2 y_2)]
$$
$$
= (-1)^{p_2 q_1} D(x_1 y_1 \otimes x_2 y_2) = D((x_1 \otimes x_2)(y_1 \otimes y_2)).
$$

### 2. Tích tenxơ và đồng luân

#### Mệnh đề 3 {#alg-x-s4-prop-3 .statement}

Cho $C,\ C_1$ là hai phức của các $A$-môđun phải, $C',\ C'_1$ là hai phức của các $A$-môđun trái, và $u : C \to C_1,\ v : C \to C_1,\ u' : C' \to C'_1,\ v' : C' \to C'_1$ là các xạ của các phức.

a) Nếu $u$ và $u'$ lần lượt đồng luân với $v$ và $v'$, thì hai xạ $u \otimes u'$ và $v \otimes v'$ từ $C \otimes_A C'$ đến $C_1 \otimes_A C'_1$ là đồng luân.

b) Nếu $u$ và $u'$ là các tương đương đồng luân, thì $u \otimes u'$ là một tương đương đồng luân.

c) Nếu $C$ hoặc $C'$ đồng luân với không, thì $C \otimes_A C'$ đồng luân với không.

Gọi bằng cùng một chữ cái $d$ các vi phân của các phức $C,\ C_1,\ C',\ C'_1$ và bằng $D$ các vi phân của các phức $C \otimes_A C'$ và $C_1 \otimes_A C'_1$.

Nếu $u$ (tương ứng $u'$) đồng luân với $v$ (tương ứng $v'$), thì tồn tại một đồng cấu phân bậc bậc 1 $s:C\to C_1$ (tương ứng $s':C'\to C'_1$) sao cho

$$
(2)\qquad u-v=ds+sd\qquad\text{(resp. }u'-v'=ds'+s'd\text{)}.
$$

Gọi $S:C\otimes_A C'\to C_1\otimes_A C'_1$ là đồng cấu phân bậc duy nhất bậc 1 sao cho, với $x\in C_p,\ y\in C'_q,\ p,q\in\mathbf Z$, ta có

$$
(3)\qquad S(x\otimes y)=s(x)\otimes u'(y)+(-1)^p v(x)\otimes s'(y).
$$

Khi đó, với các ký hiệu trước đó:

$$
\begin{aligned}
(DS+SD)(x\otimes y)&=D(sx\otimes u'y)+(-1)^pD(vx\otimes s'y)+S(dx\otimes y)\\
&\quad+(-1)^pS(x\otimes dy)=\\
&=dsx\otimes u'y+(-1)^{p+1}sx\otimes du'y+(-1)^pdvx\otimes s'y+vx\otimes ds'y\\
&\quad+sdx\otimes u'y+(-1)^{p-1}vdx\otimes s'y+(-1)^psx\otimes u'dy+vx\otimes s'dy\\
&=(ds+sd)(x)\otimes u'y+vx\otimes(ds'+s'd)(y)\\
&=(ux-vx)\otimes u'y+vx\otimes(u'y-v'y)=ux\otimes u'y-vx\otimes v'y.
\end{aligned}
$$

Điều này cho $DS+SD=u\otimes u'-v\otimes v'$, do đó a).

Ta chứng minh b). Nếu $u$ và $u'$ là các tương đương đồng luân, thì tồn tại các đồng cấu của các phức $\alpha:C_1\to C$ và $\alpha':C'_1\to C'$ sao cho $u\circ\alpha,\ \alpha\circ u',\ \alpha'\circ u'$ lần lượt đồng luân với $\mathrm{Id}_{C_1},\ \mathrm{Id}_C,\ \mathrm{Id}_{C'_1},\ \mathrm{Id}_{C'}$. Khi đó $(u\otimes u')\circ(\alpha\otimes\alpha')$, bằng $(u\circ\alpha)\otimes(u'\circ\alpha')$, là đồng luân theo a) với $\mathrm{Id}_{C_1}\otimes\mathrm{Id}_{C'_1}=\mathrm{Id}_{C_1\otimes C'_1}$, trong khi $(\alpha\otimes\alpha')\circ(u\otimes u')$ đồng luân với $\mathrm{Id}_{C\otimes C'}$, do đó b). Cuối cùng, c) suy ra từ b) áp dụng vào trường hợp $C_1$ hoặc $C'_1$ là không.

#### Hệ quả 1 {#alg-x-s4-prop-3-cor-1 .statement}

Cho $C'$ là một phức tách của các $A$-môđun trái sao cho $H(C')$ là phẳng. Với mọi phức $C$ của các $A$-môđun phải, ánh xạ chính tắc

$$
\gamma(C,C'):H(C)\otimes_AH(C')\longrightarrow H(C\otimes_A C')
$$

là song ánh.

Theo X, p. 35, def. 6, tồn tại một tương đương đồng luân $u':C'\to H(C')$. Theo mệnh đề 3, $1_C\otimes u':C\otimes_A C'\to C\otimes_AH(C')$ là một tương đương đồng luân; vì

$$
H(1_C\otimes u')\circ\gamma(C,C')=\gamma(C,H(C'))\circ(1_C\otimes H(u')),
$$

và $H(1_C\otimes u')$ và $H(u')$ là song ánh, chỉ cần chứng minh rằng $\gamma(C,H(C'))$ là song ánh, và ta quy về trường hợp $C'$ phẳng và có vi phân không. Trong trường hợp này, các dãy khớp chính tắc

$$
\mathrm{(I)}\qquad 0\longrightarrow Z(C)\xrightarrow{i}C\xrightarrow{\partial}B(C)\longrightarrow0
$$

$$
\mathrm{(II)}\qquad 0\longrightarrow B(C)\xrightarrow{j}Z(C)\xrightarrow{\pi}H(C)\longrightarrow0
$$

cho các dãy khớp:

$$
0 \longrightarrow Z(C) \otimes_A C' \xrightarrow{i\otimes 1} C \otimes_A C' \xrightarrow{\delta\otimes 1} B(C) \otimes_A C' \longrightarrow 0
$$

$$
0 \longrightarrow B(C) \otimes_A C' \xrightarrow{j\otimes 1} Z(C) \otimes_A C' \xrightarrow{\pi\otimes 1} H(C) \otimes_A C' \longrightarrow 0.
$$

Vì $d=i\circ j\circ\delta$, ta có $D=d\otimes 1_{C'}=(i\otimes 1)\circ(j\otimes 1)\circ(\delta\otimes 1)$, điều này chỉ ra rằng các ánh xạ chính tắc $Z(C)\otimes_A C'\to Z(C\otimes_A C')$ và $B(C)\otimes_A C'\to B(C\otimes_A C')$ là song ánh, do đó $\gamma(C,C')$ cũng vậy bằng cách chuyển qua thương.

#### Hệ quả 2 {#alg-x-s4-prop-3-cor-2 .statement}

Cho $\mathbf N$ là một $A$-môđun trái phẳng. Với mọi phức $C$ của các $A$-môđun phải, các đồng cấu chính tắc

$$
\gamma_n(C,\mathbf N): H_n(C)\otimes_A \mathbf N \longrightarrow H_n(C\otimes_A \mathbf N)
$$

là song ánh.

#### Hệ quả 3 {#alg-x-s4-prop-3-cor-3 .statement}

Cho $C'$ là một phức của các $A$-môđun trái sao cho $B(C')$ và $H(C')$ là xạ ảnh. Với mọi phức $C$ của các $A$-môđun phải, ánh xạ $\gamma(C,C')$ là song ánh.

Thật vậy, $C'$ là tách (X, p. 35, ví dụ 4) và $H(C')$ là xạ ảnh; do đó ta có thể áp dụng hệ quả 1.

#### Nhận xét 1 {#alg-x-s4-n2-rem-1 .statement}

Sử dụng các đẳng cấu giao hoán, từ các hệ quả 1, 2 và 3 ta suy ra các mệnh đề tương tự thu được bằng cách hoán đổi vai trò của hai đối số của các tích tenxơ.

#### Nhận xét 2 {#alg-x-s4-n2-rem-2 .statement}

Ta sẽ thấy dưới đây (X, p. 79, Hệ quả 4) rằng kết luận của Hệ quả 1 cũng đúng khi giả sử $C'$ và $H(C')$ phẳng và $C'$ bị chặn về phía phải.

### 3. Tích tenxơ bởi một phức phẳng bị chặn về phía phải

#### Bổ đề 1 {#alg-x-s4-lem-1 .statement}

Cho C là một phức của các $A$-môđun phải và E là một phức của các $A$-môđun trái. Ta giả sử rằng $H(C)=0$ và rằng E là phẳng và bị chặn về phía phải. Khi đó $H(C\otimes_A E)=0$.

Với $k\in\mathbf Z$, gọi $T^{(k)}$ là phức con của $C\otimes_A E$ sao cho

$$
T_n^{(k)}=\sum_{\substack{p+q=n\\q\leq k}} C_p\otimes_A E_q\ ;
$$

khi đó $T^{(k-1)}\subset T^{(k)}$ và ta có một dãy khớp các phức

$$
0\longrightarrow T^{(k-1)}\xrightarrow{i_k}T^{(k)}\xrightarrow{\pi}C\otimes_A E_k(-k)\longrightarrow 0
$$

trong đó $i_k$ là đơn ánh chính tắc và $\pi$ chiếu tổng trực tiếp trước đó lên nhân tử của nó $C_{n-k}\otimes_A E_k=(C\otimes_A E_k(-k))_n$. Theo Hệ quả 2 ở trên, ta có $H(C\otimes_A E_k(-k))=0$, do đó $i_k$ là một đồng cấu. Ta có $T^{(k)}=0$ với $k$ đủ nhỏ, vì E bị chặn về phía phải, do đó $H(T^{(k)})=0$ với mọi $k$ theo quy nạp trên $k$. Cuối cùng, cấu xạ chính tắc $\underset{\longrightarrow}{\lim}\,T^{(k)}\to C\otimes_A E$ hiển nhiên là một đẳng cấu, do đó $H(C\otimes_A E)=0$ (X, p. 28, Mệnh đề 1).

#### Bổ đề 2 {#alg-x-s4-lem-2 .statement}

Nếu $u:C\to C'$ là một cấu xạ của các phức của $A$-môđun phải và E là một phức của các $A$-môđun trái, thì các phức $\operatorname{Con}(u)\otimes_A E$ và $\operatorname{Con}(u\otimes 1_E)$ là đẳng cấu.

Theo định nghĩa, $\operatorname{Con}(u)\otimes_A E$ là môđun phân bậc $(C'(-1)\oplus C)\otimes_A E$ được trang bị vi phân $D$ sao cho, với $x\in C_p$, $y'\in C'(-1)_p=C'_{p-1}$, $z\in E_q$, ta có

(4)
$$
D(y',x)\otimes z=(-dy',dx-u(y'))\otimes z+(-1)^p(y',x)\otimes dz,
$$

trong khi $\operatorname{Con}(u\otimes 1_E)$ là môđun phân bậc $(C'\otimes_A E)(-1)\oplus(C\otimes_A E)$ được trang bị vi phân $D_1$ sao cho, với $x\in C_p$, $y'\in C'_{p-1}$, $z\in E_q$, ta có

$$
D_1(y'\otimes z,x\otimes z)=(-dy'\otimes z-(-1)^{p-1}y'\otimes dz,dx\otimes z+(-1)^p x\otimes dz-u(y')\otimes z)
$$

$$
=(-dy'\otimes z,(dx-u(y'))\otimes z)+(-1)^p(y'\otimes dz,x\otimes dz),
$$

do đó có mệnh đề.

#### Mệnh đề 4 {#alg-x-s4-prop-4 .statement}

Cho $u:C\to C'$ là một đẳng cấu đồng điều của các phức của $A$-môđun phải và E là một phức của các $A$-môđun trái, phẳng và bị chặn về phía phải. Khi đó

$$
u\otimes 1_E:C\otimes_A E\to C'\otimes_A E
$$

là một đẳng cấu đồng điều của các phức của $k$-môđun.

Thật vậy, theo X, p. 38, Hệ quả, $u$ (tương ứng $u\otimes 1_E$) là một đẳng cấu đồng điều khi và chỉ khi $H(\operatorname{Con}(u))=0$ (tương ứng $H(\operatorname{Con}(u\otimes 1_E))=0$). Kết luận suy ra từ các Bổ đề 1 và 2.

#### Nhận xét {#alg-x-s4-n3-rem-1 .statement}

Sử dụng các đẳng cấu giao hoán, từ các mệnh đề trước đó ta suy ra các mệnh đề tương tự thu được bằng cách hoán đổi vai trò của hai đối số của các tích tenxơ.

### 4. Định nghĩa và các tính chất đầu tiên của tích xoắn

Với mọi A-môđun $E$, ta ký hiệu bởi $p_E:L(E)\to E$ phân giải tự do chính tắc của $E$ (X, p. 50).

#### Định nghĩa 1 {#alg-x-s4-def-1 .statement}

Cho $M$ là một A-môđun phải và $N$ là một A-môđun trái. Ta gọi tích xoắn của $M$ và $N$ là môđun $k$ phân bậc

(4)
$$
\operatorname{Tor}^A(M,N)=H(L(M)\otimes_A L(N)).
$$

Các thành phần thuần nhất của $\operatorname{Tor}^A(M,N)$ được ký hiệu

(5)
$$
\operatorname{Tor}^A_n(M,N)=H_n(L(M)\otimes_A L(N)).
$$

Vì $L(M)$ và $L(N)$ bằng không ở bên phải, ta có

(6)
$$
\operatorname{Tor}_n^A(M, N) = 0 \quad \text{cho } n < 0 .
$$

#### Nhận xét 1 {#alg-x-s4-n4-rem-1 .statement}

Ta sẽ thấy dưới đây (X, p. 107, Mệnh đề 6) các tính chất hữu hạn của các môđun $\operatorname{Tor}^A(M, N)$. Chẳng hạn, nếu $A$ là giao hoán Noether và nếu $M$ và $N$ là các $A$-môđun kiểu hữu hạn, thì mọi $A$-môđun $\operatorname{Tor}_n^A(M, N)$ đều là kiểu hữu hạn.

Cho $f : M \to M'$ là một đồng cấu của các $A$-môđun phải và $g : N \to N'$ là một đồng cấu của các $A$-môđun trái. Ta định nghĩa $\operatorname{Tor}^A(f, g) = H(L(f) \otimes_A L(g))$; đây là một đồng cấu của các môđun $k$ phân bậc

$$
\operatorname{Tor}^A(f, g) : \operatorname{Tor}^A(M, N) \to \operatorname{Tor}^A(M', N')
$$

mà các thành phần thuần nhất của nó được ký hiệu

$$
\operatorname{Tor}_n^A(f, g) : \operatorname{Tor}_n^A(M, N) \to \operatorname{Tor}_n^A(M', N') .
$$

Theo Mệnh đề 1 của X, p. 62, đồng cấu chính tắc

$$
\gamma_{0,0} : H_0(L(M)) \otimes_A H_0(L(N)) \to H_0(L(M) \otimes_A L(N))
$$

là song ánh; sử dụng các đẳng cấu $M \to H_0(L(M))$ và $N \to H_0(L(N))$, ta suy ra từ đó một đẳng cấu, được gọi là *chính tắc*

(7)
$$
\gamma_{M,N} : M \otimes_A N \to \operatorname{Tor}_0^A(M, N) .
$$

Ta sẽ luôn đồng nhất $\operatorname{Tor}_0^A(M, N)$ với $M \otimes_A N$ qua đẳng cấu này. Do đó ánh xạ tuyến tính $k$ $\operatorname{Tor}_0^A(f, g)$ được đồng nhất với $f \otimes g$.

#### Nhận xét 2 {#alg-x-s4-n4-rem-2 .statement}

Cấu xạ phức $p_M \otimes p_N : L(M) \otimes_A L(N) \to M \otimes_A N$ cảm sinh trên đồng điều bậc 0 đẳng cấu

$$
\gamma_{M,N}^{-1} : \operatorname{Tor}_0^A(M, N) \to M \otimes_A N
$$

nghịch đảo của $\gamma_{M,N}$.

Ta có $L(1_M) = 1_{L(M)}$, $L(1_N) = 1_{L(N)}$, do đó bằng cách chuyển qua đồng điều:

(8)
$$
\operatorname{Tor}^A(1_M, 1_N) = 1_{\operatorname{Tor}^A(M, N)} .
$$

Nếu $f' : M' \to M''$ (tương ứng $g' : N' \to N''$) là một đồng cấu của các $A$-môđun phải (tương ứng trái), ta có $L(g' \circ g) = L(g') \circ L(g)$ và $L(f' \circ f) = L(f') \circ L(f)$, do đó

(9)
$$
\operatorname{Tor}^A(f' \circ f, g' \circ g) = \operatorname{Tor}^A(f', g') \circ \operatorname{Tor}^A(f, g) .
$$

Xét các cấu xạ của các phức $k$

$$
L(M) \otimes_A N \xleftarrow{1 \otimes p_N} L(M) \otimes_A L(N) \xrightarrow{p_M \otimes 1} M \otimes_A L(N)
$$

và các đồng cấu $k$ mà chúng cảm sinh trong đồng điều:

$$
H(L(M) \otimes_A N) \xleftarrow{\psi_M(N)} \mathrm{Tor}^A(M, N) \xrightarrow{\overline{\psi}_N(M)} H(M \otimes_A L(N)) ;
$$

theo Mệnh đề 4 của X, p. 67, $1 \otimes p_N$ và $p_M \otimes 1$ là các cấu xạ đồng điều. Do đó:

**Mệnh đề 5. — Các đồng cấu $k$**

$$
\begin{aligned}
& \psi_M(N) : \mathrm{Tor}^A(M, N) \to H(L(M) \otimes_A N) \\
& \overline{\psi}_N(M) : \mathrm{Tor}^A(M, N) \to H(M \otimes_A L(N))
\end{aligned}
$$

là *song ánh*.

**Hệ quả. — Nếu $M$ hoặc $N$ là phẳng, $\mathrm{Tor}_i^A(M, N) = 0$ với $i \geqslant 0$.**

Giả sử $N$ (resp. $M$) là phẳng. Khi đó $p_M \otimes 1 : L(M) \otimes_A N \to M \otimes_A N$ (resp. $1 \otimes p_N : M \otimes_A L(N) \to M \otimes_A N$) là một cấu xạ đồng luân (X, p. 67, Mệnh đề 4), do đó $H_i(L(M) \otimes_A N)$ (resp. $H_i(M \otimes_A L(N))$) triệt tiêu với $i > 0$.

*Nhận xét 3. — Nếu $g : N \to N'$ là một đồng cấu của các môđun trái A, thì*

$$
(1_{L(M)} \otimes g) \circ (1_{L(M)} \otimes 1_N) = (1_{L(M)} \otimes 1_N) \circ (1_{L(M)} \otimes L(g)) ,
$$

do đó biểu đồ

$$
\begin{array}{ccc}
\mathrm{Tor}^A(M, N) & \xrightarrow{\psi_{M(N)}} & H(L(M) \otimes_A N) \\
\mathrm{Tor}^A(1, g) \downarrow & & \downarrow H(1 \otimes g) \\
\mathrm{Tor}^A(M, N') & \xrightarrow{\psi_{M(N')}} & H(L(M) \otimes_A N')
\end{array}
$$

là giao hoán.

Tương tự, nếu $f : M \to M'$ là một đồng cấu của các môđun phải A, ta có một biểu đồ giao hoán :

$$
\begin{array}{ccc}
\mathrm{Tor}^A(M, N) & \xrightarrow{\overline{\psi}_{N(M)}} & H(M \otimes_A L(N)) \\
\mathrm{Tor}^A(f, 1) \downarrow & & \downarrow H(f \otimes 1) \\
\mathrm{Tor}^A(M', N) & \xrightarrow{\overline{\psi}_{N(M')}} & H(M' \otimes_A L(N)) .
\end{array}
$$

**Mệnh đề 6. — Ánh xạ** $(f, g) \mapsto \mathrm{Tor}^A(f, g) :$

$$
\mathrm{Hom}_A(M, M') \times \mathrm{Hom}_A(N, N') \to \mathrm{Hom}_k(\mathrm{Tor}^A(M, N), \mathrm{Tor}^A(M', N'))
$$

*là $k$-song tuyến tính.*

Cho $f \in \mathrm{Hom}_A(M, M')$, $g_1, g_2 \in \mathrm{Hom}_A(N, N')$, $\lambda_1, \lambda_2 \in k$. Khi đó các cấu xạ

$$
\lambda_1(L(f) \otimes g_1) + \lambda_2(L(f) \otimes g_2) \quad \text{và} \quad L(f) \otimes (\lambda_1 g_1 + \lambda_2 g_2)
$$

từ $L(M) \otimes_A N$ vào $L(M) \otimes_A N'$ trùng nhau; theo mệnh đề 5 và Nhận xét 3, do đó ta có

(10) $$
\mathrm{Tor}^A(f, \lambda_1 g_1 + \lambda_2 g_2) = \lambda_1 \mathrm{Tor}^A(f, g_1) + \lambda_2 \mathrm{Tor}^A(f, g_2).
$$

Ta lập luận tương tự đối với ánh xạ $f \mapsto \mathrm{Tor}^A(f, g)$.

#### Hệ quả {#alg-x-s4-n4-cor-1 .statement}

*Cho $\lambda \in k$. Nếu $\lambda$ triệt tiêu $M$ hoặc $N$, thì nó triệt tiêu $\mathrm{Tor}^A(M, N)$.*

Thật vậy, $\lambda . 1_{\mathrm{Tor}(M, N)} = \mathrm{Tor}(\lambda . 1_M, 1_N) = \mathrm{Tor}(1_M, \lambda . 1_N)$.

#### Mệnh đề 7 {#alg-x-s4-prop-7 .statement}

*Cho I và J là hai tập hợp, $(M_\alpha)_{\alpha \in I}$ là một họ các môđun phải A, $(N_\beta)_{\beta \in J}$ là một họ các môđun trái A. Đồng cấu*

$$
\bigoplus_{\alpha \in I, \beta \in J} \mathrm{Tor}^A(M_\alpha, N_\beta) \to \mathrm{Tor}^A\left( \bigoplus_{\alpha \in I} M_\alpha, \bigoplus_{\beta \in J} N_\beta \right)
$$

*được suy ra từ các đồng cấu chính tắc* $M_\alpha \to \bigoplus M_\alpha$ *và* $N_\beta \to \bigoplus N_\beta$ *là song ánh*.

Chỉ cần chứng minh rằng với mọi môđun phải $M$ (resp. mọi môđun trái $N$), đồng cấu chính tắc

$$
\bigoplus_{\beta \in J} \mathrm{Tor}^A(M, N_\beta) \to \mathrm{Tor}^A(M, \bigoplus_{\beta \in J} N_\beta)
$$

(resp. $\bigoplus_{\alpha \in I} \mathrm{Tor}^A(M_\alpha, N) \to \mathrm{Tor}^A(\bigoplus_{\alpha \in I} M_\alpha, N)$) là song ánh. Bây giờ điều này suy ra từ điều trước, từ Mệnh đề 1 của X, p. 28, và từ các đẳng cấu chính tắc :

$$
\bigoplus_{\beta} (L(M) \otimes_A N_\beta) \to L(M) \otimes_A (\bigoplus_{\beta} N_\beta),
$$

$$
\bigoplus_{\alpha} (M_\alpha \otimes_A L(N)) \to (\bigoplus_{\alpha} M_\alpha) \otimes_A L(N).
$$

Một lập luận tương tự cho :

#### Mệnh đề 8 {#alg-x-s4-prop-8 .statement}

*Cho I (resp. J) là một tập tiền thứ tự lọc phải, (($M_\alpha$, $u_{\alpha', \alpha}$) (resp. (($N_\beta$, $v_{\beta', \beta}$))) là một hệ quy nạp các môđun phải A (resp. trái) tương ứng với I (resp. J). Đồng cấu của các môđun k phân bậc*

$$
\lim_{\longrightarrow (\alpha, \beta) \in I \times J} \mathrm{Tor}^A(M_\alpha, N_\beta) \to \mathrm{Tor}^A\left( \lim_{\longrightarrow \alpha \in I} M_\alpha, \lim_{\longrightarrow \beta \in J} N_\beta \right),
$$

*được suy ra từ các đồng cấu A chính tắc* $M_\alpha \to \lim_{\longrightarrow} M_\alpha$ *và* $N_\beta \to \lim_{\longrightarrow} N_\beta$, *là song ánh*.

Đặc biệt, lấy $J = I$ và nhận xét rằng $(\alpha, \alpha), \alpha \in I$, tạo thành một tập con đồng cuối của $I \times I$, ta thu được :

#### Hệ quả {#alg-x-s4-n4-cor-2 .statement}

Cho I là một tập tiền thứ tự lọc phải, $(M_i, u_{ji})$ (resp. $(N_i, v_{ji})$) là một hệ quy nạp các môđun phải $A$ (resp. trái) tương ứng với I. Đồng cấu của các môđun $k$ phân bậc

$$
\lim_{\longrightarrow i \in I} \operatorname{Tor}^A(M_i, N_i) \to \operatorname{Tor}^A\left(\lim_{\longrightarrow i \in I} M_i, \lim_{\longrightarrow i \in I} N_i\right),
$$

suy ra từ các $A$-đồng cấu chính tắc $M_i \to \lim_{\longrightarrow} M_i$ và $N_j \to \lim_{\longrightarrow} N_j$ là song ánh.

#### 5. Liên kết các đồng cấu và các dãy khớp

Cho $M$ là một $A$-môđun phải, $N$ là một $A$-môđun trái, $A^\circ$ là vành đối của $A$, $M^\circ$ là $A^\circ$-môđun trái cơ sở trên $M$, $N^\circ$ là $A^\circ$-môđun phải cơ sở trên $N$. Ta có $L(M^\circ ) = L(M)^\circ $ và $L(N^\circ ) = L(N)^\circ $, do đó có một đẳng cấu giao hoán (X, p. 63, prop. 2)

$$
\sigma(L(M), L(N)) : L(M) \otimes_A L(N) \to L(N^\circ) \otimes_{A^\circ} L(M^\circ).
$$

Chuyển qua đồng điều, $\sigma(L(M), L(N))$ sinh ra một đẳng cấu phân bậc bậc 0 $\sigma_{M,N} : \operatorname{Tor}^A(M, N) \to \operatorname{Tor}^{A^\circ}(N^\circ, M^\circ)$ được gọi là *đẳng cấu giao hoán của các tích xoắn*.

Ta chú ý rằng $\sigma_{N^\circ, M^\circ} \circ \sigma_{M,N} = \mathrm{Id}_{\operatorname{Tor}(M,N)}$ và rằng $\sigma_{M,N}$ cảm sinh trên các thành phần bậc 0 đồng cấu giao hoán của tích tenxơ. Mặt khác, nếu $f : M \to M'$ và $g : N \to N'$ là các đồng cấu của các $A$-môđun, thì

$$
\operatorname{Tor}^{A^\circ}(g, f) \circ \sigma_{M,N} = \sigma_{M', N'} \circ \operatorname{Tor}^A(f, g).
$$

#### Định nghĩa 2 {#alg-x-s4-def-2 .statement}

Cho $M$ là một $A$-môđun phải. Ta nhắc lại rằng với mọi $A$-môđun trái $N$, một đẳng cấu

$$
\psi_M(N) : \operatorname{Tor}^A(M, N) \to H(L(M) \otimes_A N)
$$

đã được định nghĩa trong tiết diện trước (X, p. 69, prop. 5). Cho

$$(\mathcal{E})$$
$$
0 \to N' \xrightarrow{u} N \xrightarrow{v} N'' \to 0
$$

là một dãy khớp của các $A$-môđun trái; khi đó dãy các phức $k$

$$(\mathcal{ME})$$
$$
0 \longrightarrow L(M) \otimes_A N' \xrightarrow{1 \otimes u} L(M) \otimes_A N \xrightarrow{1 \otimes v} L(M) \otimes_A N'' \longrightarrow 0
$$

là khớp (X, p. 66, Bổ đề 1); ký hiệu bởi

$$
\partial^{(\mathcal{ME})} : H(L(M) \otimes_A N'') \to H(L(M) \otimes_A N')
$$

đồng cấu liên kết tương ứng (X, p. 29).

Đồng cấu liên kết của các tích xoắn, tương ứng với môđun $M$ và dãy khớp $\mathcal{E}$, là đồng cấu hợp thành

$$
\partial(M, \mathcal{E}) = \psi_M(N')^{-1} \circ \partial^{(M\mathcal{E})} \circ \psi_M(N'') : \mathrm{Tor}^A(M, N'') \to \mathrm{Tor}^A(M, N')
$$

Đây là một $k$-đồng cấu phân bậc bậc $-1$, các thành phần thuần nhất của nó được ký hiệu là $\partial_n(M, \mathcal{E}) : \mathrm{Tor}_n^A(M, N'') \to \mathrm{Tor}_{n-1}^A(M, N')$.

#### Định lý 1 {#alg-x-s4-thm-1 .statement}

Dãy vô hạn về bên trái của các $k$-đồng cấu môđun

$$
\cdots \longrightarrow \mathrm{Tor}_n^A(M, N') \xrightarrow{\mathrm{Tor}_n^A(1, u)} \mathrm{Tor}_n^A(M, N) \xrightarrow{\mathrm{Tor}_n^A(1, v)} \mathrm{Tor}_n^A(M, N'')
$$
$$
\xrightarrow{\partial_n(M, \mathcal{E})} \mathrm{Tor}_{n-1}^A(M, N') \xrightarrow{\mathrm{Tor}_{n-1}^A(1, u)} \cdots \xrightarrow{\mathrm{Tor}_1^A(1, v)} \mathrm{Tor}_1^A(M, N'')
$$
$$
\xrightarrow{\hat{c}_1(M, \mathcal{E})} M \otimes_A N' \xrightarrow{1 \otimes u} M \otimes_A N \xrightarrow{1 \otimes v} M \otimes_A N'' \longrightarrow 0
$$

là khớp.

Để thấy điều này, xét biểu đồ

$$
\begin{array}{ccccccccc}
\mathrm{Tor}(M, N') & \xrightarrow{\mathrm{Tor}(1, u)} & \mathrm{Tor}(M, N) & \xrightarrow{\mathrm{Tor}(1, v)} & \mathrm{Tor}(M, N'') & \xrightarrow{\partial(M, \mathcal{E})} & \mathrm{Tor}(M, N') & \xrightarrow{\mathrm{Tor}(1, u)} & \mathrm{Tor}(M, N) \\
\psi_M(N') \downarrow & & \psi_M(N) \downarrow & & \psi_M(N'') \downarrow & & \psi_M(N') \downarrow & & \psi_M(N') \downarrow \\
H(L(M) \otimes N') & \xrightarrow{H(1 \otimes u)} & H(L(M) \otimes N) & \xrightarrow{H(1 \otimes v)} & H(L(M \otimes N'') & \xrightarrow{\partial^{(M\mathcal{ME})}} & H(L(M) \otimes N') & \xrightarrow{H(1 \otimes u)} & H(L(M) \otimes N)
\end{array}
$$

Nó giao hoán theo (X, p. 69, Nhận xét 3) và Định nghĩa 2. Hơn nữa, hàng dưới là khớp (X, p. 30, Định lý 1), và các $\psi_M$ khác nhau là các song ánh (X, p. 69, prop. 5).

#### Hệ quả 1 {#alg-x-s4-thm-1-cor-1 .statement}

Nếu $\mathrm{Tor}_1^A(M, N'') = 0$, dãy

$$
0 \longrightarrow M \otimes_A N' \xrightarrow{1 \otimes u} M \otimes_A N \xrightarrow{1 \otimes v} M \otimes_A N'' \longrightarrow 0
$$

là khớp.

#### Hệ quả 2 {#alg-x-s4-thm-1-cor-2 .statement}

Cho $0 \to C' \xrightarrow{u} C \xrightarrow{v} C'' \to 0$ là một dãy khớp của các phức các $A$-môđun trái, và cho $E$ là một phức các $A$-môđun phải. Nếu $C''$ hoặc $E$ là phẳng, dãy

$$
0 \longrightarrow E \otimes_A C' \xrightarrow{1 \otimes u} E \otimes_A C \xrightarrow{1 \otimes v} E \otimes_A C'' \longrightarrow 0
$$

là khớp.

Thật vậy, $\mathrm{Tor}_1^A(E, C'') = 0$ theo X, p. 69, Hệ quả của prop. 5.

#### Ví dụ {#alg-x-s4-n5-exa-1 .statement}

Cho $a$ là một iđêan của $A$. Dãy khớp

$$
0 \to a \to A_s \to A/a \to 0
$$

của các A-môđun trái, cho ra một dãy khớp của các tích xoắn, trong đó các số hạng Tor$_i^A$ (M, A) bằng không với $i > 0$. Từ đó suy ra các đẳng cấu

$$
\operatorname{Tor}_{i+1}^A(M, A/\alpha) \to \operatorname{Tor}_i^A(M, \alpha), \quad i > 0
$$

và một dãy khớp

$$
0 \to \operatorname{Tor}_1^A(M, A\alpha) \to M \otimes_A \alpha \to M \otimes_A A \to M \otimes A \alpha \to 0 :
$$

suy ra rằng $\operatorname{Tor}_1^A(M, A/\alpha)$ được đồng nhất với hạt nhân của đồng cấu chính tắc $M \otimes_A \alpha \to M$.

Ví dụ, lấy M là một môđun có dạng $A_d/b$, trong đó b là một iđêan phải của A, ta thu được một đẳng cấu của $\operatorname{Tor}_1^A(A/b, A/\alpha)$ lên $(\alpha \cap b)/ba$.

#### Mệnh đề 9 {#alg-x-s4-prop-9 .statement}

*Cho f : M → M$_1$ là một đồng cấu của các A-môđun phải và*

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & N' & \xrightarrow{u} & N & \xrightarrow{v} & N'' & \longrightarrow & 0 \\
& & g' \downarrow & & g \downarrow & & g'' \downarrow & & \\
0 & \longrightarrow & N'_1 & \xrightarrow{u_1} & N_1 & \xrightarrow{v_1} & N''_1 & \longrightarrow & 0
\end{array}
$$

*(E$_1$)*

*là một biểu đồ giao hoán với các hàng khớp gồm các đồng cấu của các A-môđun trái. Biểu đồ của các k-môđun*

$$
\begin{array}{ccc}
\operatorname{Tor}^A(M, N'') & \xrightarrow{\partial(M, E)} & \operatorname{Tor}^A(M, N') \\
\operatorname{Tor}^A(f, g'') \downarrow & & \operatorname{Tor}^A(f, g') \downarrow \\
\operatorname{Tor}^A(M_1, N''_1) & \xrightarrow{\partial(M_1, E_1)} & \operatorname{Tor}^A(M_1, N'_1)
\end{array}
$$

*là giao hoán.*

Điều này suy ra từ X, p. 31, mệnh đề 2, áp dụng cho biểu đồ giao hoán

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & L(M) \otimes_A N' & \xrightarrow{1 \otimes u} & L(M) \otimes_A N & \xrightarrow{1 \otimes v} & L(M) \otimes_A N'' & \longrightarrow & 0 \\
& & L(f) \otimes g' \downarrow & & L(f) \otimes g \downarrow & & L(f) \otimes g'' \downarrow & & \\
0 & \longrightarrow & L(M_1) \otimes_A N'_1 & \xrightarrow{1 \otimes u_1} & L(M_1) \otimes_A N_1 & \xrightarrow{1 \otimes v_1} & L(M_1) \otimes_A N''_1 & \longrightarrow & 0 .
\end{array}
$$

Theo cách tương tự, nếu N là một A-môđun trái và

$$(F)$$
$$
0 \to M' \xrightarrow{r} M \xrightarrow{s} M'' \to 0
$$

là một dãy khớp của các A-môđun phải, ta định nghĩa các *đồng cấu liên kết*

$$
\partial(F, N) : \operatorname{Tor}^A(M'', N) \to \operatorname{Tor}^A(M', N)
$$
$$
\partial_n(F, N) : \operatorname{Tor}_n^A(M'', N) \to \operatorname{Tor}_{n-1}^A(M', N)
$$

bởi $\partial(\mathcal F,\mathbf N)=\overline{\psi}_{\mathbf N}(M')^{-1}\circ\partial(\mathcal F^{\mathbf N})\circ\overline{\psi}_{\mathbf N}(M'')$, trong đó $\partial(\mathcal F^{\mathbf N})$ là đồng cấu liên kết của dãy khớp

$$(\mathcal F_{\mathbf N})\qquad 0\longrightarrow M'\otimes_A L(N)\longrightarrow M\otimes_A L(N)\longrightarrow M''\otimes_A L(N)\longrightarrow 0$$

suy ra từ $\mathcal F$, và ta có:

**ĐỊNH LÝ 1 bis.** — *Dãy không bị chặn về bên trái của các đồng cấu của các k-môđun*

$$\longrightarrow \operatorname{Tor}_n^A(M',N)\xrightarrow{\operatorname{Tor}_n^A(r,1)}\operatorname{Tor}_n^A(M,N)\xrightarrow{\operatorname{Tor}_n^A(s,1)}\operatorname{Tor}_n^A(M'',N)\xrightarrow{\partial_n(\mathcal F,N)}\operatorname{Tor}_{n-1}^A(M',N)$$

$$\cdots\longrightarrow \operatorname{Tor}_1^A(M'',N)\xrightarrow{\partial_1(\mathcal F,N)}M'\otimes_A N\xrightarrow{r\otimes1}M\otimes_A N\xrightarrow{s\otimes1}M''\otimes_A N\longrightarrow0$$

*là khớp.*

Ta để lại cho độc giả nhiệm vụ phát biểu và chứng minh các tính chất tương tự với các hệ quả của định lý 1 và với mệnh đề 9. Hơn nữa:

#### Mệnh đề 10 {#alg-x-s4-prop-10 .statement}

*Ta ký hiệu bởi $(\mathcal F^\circ)$ dãy khớp của các A-môđun trái*

$$0\longrightarrow M'\xrightarrow{r}M\xrightarrow{s}M''\longrightarrow0.$$

*Biểu đồ*

$$
\begin{array}{ccccc}
\operatorname{Tor}^A(M'',N)&\xrightarrow{\partial(\mathcal F,N)}&\operatorname{Tor}^A(M',N)\\
\Big\downarrow{\sigma_{M'',N}}&&\Big\downarrow{\sigma_{M',N}}\\
\operatorname{Tor}^{A^\circ}(N^\circ,{M''}^\circ)&\xrightarrow{\partial(N^\circ,\mathcal F^\circ)}&\operatorname{Tor}^{A^\circ}(N^\circ,{M'}^\circ)
\end{array}
$$

*là giao hoán.*

Thật vậy, điều này suy ra từ X, p. 31, mệnh đề 2, áp dụng cho biểu đồ giao hoán

$$
\begin{array}{ccccccccc}
0&\longrightarrow&M'\otimes_A L(N)&\xrightarrow{r\otimes1}&M\otimes_A L(N)&\xrightarrow{s\otimes1}&M''\otimes_A L(N)&\longrightarrow&0\\
&&\Big\downarrow{\sigma(M',L(N))}&&\Big\downarrow{\sigma(M,L(N))}&&\Big\downarrow{\sigma(M'',L(N))}\\
0&\longrightarrow&L(N^\circ)\otimes_{A^\circ}{M'}^\circ&\xrightarrow{1\otimes r}&L(N^\circ)\otimes_{A^\circ}M^\circ&\xrightarrow{1\otimes s}&L(N^\circ)\otimes_{A^\circ}{M''}^\circ&\longrightarrow&0 .
\end{array}
$$

Ta sẽ thấy sau này các quan hệ giao hoán khác *(xem* X, p. 131, hệ quả 1*).*

### 6. Các môđun phẳng và các tích xoắn

#### Định lý 2 {#alg-x-s4-thm-2 .statement}

*Cho E là một A-môđun phải. Các điều kiện sau là tương đương :*

(i) E *là phẳng* ;

(ii) *với mọi* A-môđun trái F, *và mọi số nguyên* $n>0$, *ta có*

$$\operatorname{Tor}_n^A(E,F)=0\,;$$

(iii) Đối với mọi $A$-môđun trái xyclic $F$ có biểu diễn hữu hạn, ta có
$$
\operatorname{Tor}_1^A(E, F) = 0 ;
$$
(iv) Đối với mọi iđêan trái $a$ của $A$ có kiểu hữu hạn, ánh xạ chính tắc $E \otimes_A a \to E$ là đơn ánh;
(v) Đối với mọi dãy khớp của các $A$-môđun phải có dạng
$$
0 \to G \xrightarrow{\nu} H \xrightarrow{w} E \to 0,
$$
và mọi $A$-môđun trái $F$, dãy
$$
0 \longrightarrow G \otimes_A F \xrightarrow{\nu \otimes 1} H \otimes_A F \xrightarrow{w \otimes 1} E \otimes_A F \longrightarrow 0
$$
là khớp.
(i) $\Rightarrow$ (ii): Đây là hệ quả của Mệnh đề 5 của X, p. 69.
(ii) $\Rightarrow$ (iii): Điều này là tầm thường.
(iii) $\Leftrightarrow$ (iv): Mọi $A$-môđun trái xyclic có biểu diễn hữu hạn đều đẳng cấu với một môđun thương $A/a$, trong đó $a$ là một iđêan trái có kiểu hữu hạn, do đó (iii) tương đương với (iv) theo X, p. 72, Ví dụ.
(iii) $\Rightarrow$ (i): Theo X, p. 8, Mệnh đề 3, X, p. 72, Định lý 1, $E$ là phẳng ngay khi $\operatorname{Tor}_1^A(E, F) = 0$ đối với mọi $A$-môđun trái $F$. Nếu (iii) được thỏa mãn, điều này xảy ra khi $F$ là xyclic và có biểu diễn hữu hạn. Theo X, p. 11, Mệnh đề 7, mọi $A$-môđun (tương ứng, mọi $A$-môđun xyclic) là giới hạn quy nạp lọc của các môđun có biểu diễn hữu hạn (tương ứng, của các môđun xyclic có biểu diễn hữu hạn); do đó, theo X, p. 70, Mệnh đề 8, chỉ cần chứng minh rằng nếu $\operatorname{Tor}_1^A(E, F) = 0$ khi $F$ là xyclic, thì điều này cũng đúng khi $F$ có kiểu hữu hạn. Vì vậy ta tiến hành quy nạp theo lực lượng của một hệ sinh $(f_1, \ldots, f_n)$ của $F$; dãy khớp
$$
0 \to Af_1 \to F \to F/Af_1 \to 0
$$
sinh ra một dãy khớp
$$
\operatorname{Tor}_1^A(E, Af_1) \to \operatorname{Tor}_1^A(E, F) \to \operatorname{Tor}_1^A(E, F/Af_1),
$$
sao cho $\operatorname{Tor}_1^A(E, F) = 0$ vì $\operatorname{Tor}_1^A(E, Af_1) = 0$ và $\operatorname{Tor}_1^A(E, F/Af_1) = 0$ theo giả thiết quy nạp.
(i) $\Rightarrow$ (v): Đây là Hệ quả 2 của Định lý 1 (X, p. 72).
(v) $\Rightarrow$ (iii): Dãy khớp (X, p. 50)
$$
0 \longrightarrow Z_0(E) \xrightarrow{i_E} L_0(E) \xrightarrow{p_E} E \longrightarrow 0
$$
sinh ra, đối với mọi $A$-môđun trái $F$, một dãy khớp
$$
0 \longrightarrow \operatorname{Tor}_1^A(E, F) \longrightarrow Z_0(E) \otimes_A F \xrightarrow{i_E \otimes 1} L_0(E) \otimes_A F \xrightarrow{p_E \otimes 1} E \otimes_A F \longrightarrow 0.
$$
Nếu (v) được thỏa mãn, ta có $\operatorname{Tor}_1^A(E, F) = 0$, do đó (iii).

#### Hệ quả 1 {#alg-x-s4-thm-2-cor-1 .statement}

Cho $0 \to E' \to E \to E'' \to 0$ là một dãy khớp của các $A$-môđun phải. Giả sử rằng $E''$ là phẳng. Khi đó $E$ phẳng khi và chỉ khi $E'$ phẳng.

Cho $F$ là một $A$-môđun trái. Vì $\operatorname{Tor}^A_i(E'', F)=0$ đối với $i=1,2$ (Định lý 2, (i) $\Rightarrow$ (ii)), ta có một dãy khớp
$$
0\longrightarrow \operatorname{Tor}^A_1(E',F)\longrightarrow \operatorname{Tor}^A_1(E,F)\longrightarrow 0
$$
do đó là mệnh đề (Định lý 2, (i) $\Leftrightarrow$ (iii)).

**Hệ quả 2. —** *Cho*
$$
0\longrightarrow E_n\longrightarrow E_{n-1}\longrightarrow\cdots\longrightarrow E_1\longrightarrow0
$$
*là một dãy khớp của các $A$-môđun phải.* *Nếu $E_i$ là phẳng đối với $i=1,\ldots,n-1$, thì $E_n$ là phẳng.*

### 7. **Công thức Künneth**

Trong tiết này, ta xét một phức $(C,d)$ các $A$-môđun phải và một phức $(C',d')$ các $A$-môđun trái. Gọi
(I)
$$
0\longrightarrow Z(C)\xrightarrow{i}C\xrightarrow{\delta}B(C)(-1)\longrightarrow0,
$$
(II)
$$
0\longrightarrow B(C)\xrightarrow{i}Z(C)\xrightarrow{p}H(C)\longrightarrow0;$$
là các dãy khớp chính tắc.

Từ $\delta$ ta suy ra một đồng cấu $k$

$$
H(\delta\otimes 1):H(C\otimes_A C')\longrightarrow H(B(C)\otimes_A C')(-1);
$$

từ (II) ta suy ra một đồng cấu nối

$$
\partial(\mathrm{II},H(C')): \operatorname{Tor}^A_1(H(C),H(C'))\longrightarrow B(C)\otimes_A H(C');
$$

nếu ta trang bị $\operatorname{Tor}^A_1(H(C),H(C'))$ với phân bậc mà thành phần thuần nhất bậc $n$ là

$$
\bigoplus_{p+q=n}\operatorname{Tor}^A_1(H_p(C),H_q(C')),
$$

thì đồng cấu nối này là phân bậc bậc 0. Ta cũng có một đồng cấu chính tắc (X, p. 62)

$$
\gamma(B(C),C'): B(C)\otimes_A H(C')\longrightarrow H(B(C)\otimes_A C').
$$

Với các ký hiệu này:

#### Định lý 3. — *Giả sử các $A$-môđun $B(C)$ và $Z(C)$ là phẳng. Tồn tại duy nhất một đồng cấu các $k$-môđun phân bậc, bậc $-1$,

$$
\alpha:H(C\otimes_A C')\longrightarrow\operatorname{Tor}^A_1(H(C),H(C'))
$$

làm cho biểu đồ sau giao hoán*

$$
\begin{array}{ccc}
H(C\otimes_A C') & \xrightarrow{\alpha} & \operatorname{Tor}^A_1(H(C),H(C'))(-1)\\
{\scriptstyle H(\delta\otimes1)}\downarrow & & \downarrow{\scriptstyle\partial(\mathrm{II},H(C'))}\\
H(B(C)\otimes_A C')(-1) & \xleftarrow{\gamma(B(C),C')} & (B(C)\otimes_A H(C'))(-1).
\end{array}
$$

Dãy các $k$-môđun phân bậc

$$
0 \longrightarrow \mathrm{H}(C) \otimes_A \mathrm{H}(C') \xrightarrow{\gamma(C,C')} \mathrm{H}(C \otimes_A C') \xrightarrow{\alpha} \mathrm{Tor}_1^A(\mathrm{H}(C), \mathrm{H}(C'))(-1) \longrightarrow 0
$$

là khớp.

Do đó, với mỗi $n$, ta có một dãy khớp

(11)
$$
\begin{array}{cccccc}
0 & \longrightarrow & \bigoplus_{p+q=n} \mathrm{H}_p(C) \otimes_A \mathrm{H}_q(C') & \xrightarrow{\gamma_n(C,C')} & \mathrm{H}_n(C \otimes_A C') \\
& & & \xrightarrow{\alpha_n} & \bigoplus_{p+q=n-1} \mathrm{Tor}_1^A(\mathrm{H}_p(C), \mathrm{H}_q(C')) & \longrightarrow 0 .
\end{array}
$$

Để đơn giản, đặt $B = B(C)$, $Z = Z(C)$, $H = H(C)$, và $H' = H(C')$.

Vì $B$ là phẳng, từ (I) ta suy ra một dãy khớp (X, p. 72, Hệ quả 2)

(12)
$$
0 \longrightarrow Z \otimes_A C' \xrightarrow{j \otimes 1} C \otimes_A C' \xrightarrow{\delta \otimes 1} (B \otimes_A C')(-1) \longrightarrow 0 .
$$

#### Bổ đề 3 {#alg-x-s4-lem-3 .statement}

Đồng cấu nối $\mathrm{H}(B \otimes_A C') \to \mathrm{H}(Z \otimes_A C')$ liên kết với dãy khớp (12) bằng $\mathrm{H}(i \otimes 1)$.

Thật vậy, cho $a \in \mathrm{H}(B \otimes_A C')$; vì $B$ là phẳng, $a$ thuộc ảnh của $B \otimes_A Z(C')$, do đó có thể viết dưới dạng $\sum_\lambda da_\lambda \otimes b_\lambda$, trong đó $a_\lambda \in C$, $b_\lambda \in C'$, và $db_\lambda = 0$. Ảnh của lớp của $a$ qua đồng cấu nối, theo định nghĩa, là lớp của $D(\sum a_\lambda \otimes b_\lambda) = \sum da_\lambda \otimes b_\lambda = (i \otimes 1)(a)$, điều này chứng minh bổ đề.

Dãy khớp đồng điều liên kết với (12) do đó là

$$
\mathrm{H}(B \otimes_A C') \xrightarrow{\mathrm{H}(i \otimes 1)} \mathrm{H}(Z \otimes_A C') \xrightarrow{\mathrm{H}(j \otimes 1)} \mathrm{H}(C \otimes_A C')
$$
$$
\xrightarrow{\mathrm{H}(\delta \otimes 1)} \mathrm{H}(B \otimes_A C')(-1) \xrightarrow{\mathrm{H}(i \otimes 1)} \mathrm{H}(Z \otimes_A C')(-1) .
$$

Mặt khác, vì $Z$ là phẳng, từ (II) ta thu được một dãy các $k$-môđun phân bậc

$$
0 \longrightarrow \operatorname{Tor}_1^A(H, H') \xrightarrow{\partial(\mathrm{II}, H')} B \otimes_A H' \xrightarrow{i \otimes 1} Z \otimes_A H' \xrightarrow{p \otimes 1} H \otimes_A H' \longrightarrow 0 ;
$$

cuối cùng, ta có các đồng cấu chính tắc của No. 1

$$
\gamma_B = \gamma(B, C') : B \otimes_A H' \to \mathrm{H}(B \otimes_A C')
$$
$$
\gamma_Z = \gamma(Z, C') : Z \otimes_A H' \to \mathrm{H}(Z \otimes_A C')
$$
$$
\gamma_C = \gamma(C, C') : H \otimes_A H' \to \mathrm{H}(C \otimes_A C') ,
$$

do đó có một biểu đồ các $k$-môđun phân bậc, với *các hàng khớp*:

$$
\begin{array}{ccccccccc}
B \otimes H' & \xrightarrow{i \otimes 1} & Z \otimes H' & \xrightarrow{p \otimes 1} & H \otimes H' & \longrightarrow & 0 \\
\downarrow \gamma_B & & \downarrow \gamma_Z & & \downarrow \gamma_C & & \\
H(B \otimes C') & \xrightarrow{H(i \otimes 1)} & H(Z \otimes C') & \xrightarrow{H(j \otimes 1)} & H(C \otimes_A C') & \xrightarrow{H(\delta \otimes 1)} & H(B \otimes C')(-1) & \xrightarrow{H(i \otimes 1)} & H(Z \otimes C')(-1)
\end{array}
$$

$$
0 \longrightarrow \operatorname{Tor}_1^A(H, H')(-1) \xrightarrow{\partial(\mathrm{II}, H')} (B \otimes H')(-1) \xrightarrow{i \otimes 1} (Z \otimes H')(-1),
$$

mà là *giao hoán theo định nghĩa của các đồng cấu $\gamma$*. Nhưng vì các phức $B$ và $Z$ là tách và phẳng, $\gamma_B$ và $\gamma_Z$ là *song ánh* (X, p. 65, Hệ quả 1). Từ đó, một mặt, ta suy ra rằng $\gamma_C$ là đơn ánh và có ảnh bằng $\operatorname{Ker} H(\delta \otimes 1)$, và mặt khác, rằng $\gamma_B \circ \partial(\mathrm{II}, H')$ là đơn ánh với ảnh bằng $\operatorname{Im} H(\delta \otimes 1)$. Định lý được suy ra ngay lập tức từ đó.

#### Hệ quả 1 {#alg-x-s4-lem-3-cor-1 .statement}

*Nếu $B(C)$ và $Z(C)$ là phẳng, thì với mọi A-môđun trái $N$ và mọi số nguyên $n$, có một dãy khớp*

(13) $$ 0 \longrightarrow H_n(C) \otimes_A N \xrightarrow{\gamma_n} H_n(C \otimes_A N) \xrightarrow{\alpha_n} \operatorname{Tor}_1^A(H_{n-1}(C), N) \longrightarrow 0 . $$

#### Hệ quả 2 {#alg-x-s4-lem-3-cor-2 .statement}

*Giả sử $B(C)$ và $B(C')$ là xạ ảnh và $Z(C)$ là phẳng. Khi đó các dãy của $k$-môđun (11) và (13) là khớp và tách.*
Điều này suy ra từ định lý và bổ đề sau:

#### Bổ đề 4 {#alg-x-s4-lem-4 .statement}

*Nếu $B(C)$ và $B(C')$ là xạ ảnh, thì đồng cấu chính tắc*
$$ \gamma(C, C') : H(C) \otimes_A H(C') \to H(C \otimes_A C') $$
*có một co rút tuyến tính theo $k$.*
Thật vậy, theo X, p. 65, *nhận xét b)*, tồn tại các đồng luân $\varphi : C \to H(C)$ và $\varphi' : C' \to H(C')$ sao cho $H(\varphi) = 1_{H(C)}$ và $H(\varphi') = 1_{H(C')}$. Trong biểu đồ giao hoán

$$
\begin{array}{ccc}
H(C) \otimes_A H(C') & \xrightarrow{\gamma(C, C')} & H(C \otimes_A C') \\
\downarrow H(\varphi) \otimes H(\varphi') & & \downarrow H(\varphi \otimes \varphi') \\
H(C) \otimes_A H(C') & \xrightarrow{\gamma(H(C), H(C'))} & H(C) \otimes_A H(C')
\end{array}
$$

$H(\varphi) \otimes H(\varphi')$ và $\gamma(H(C), H(C'))$ là đồng nhất, do đó có khẳng định.

**Hệ quả 3** (*công thức hệ số phổ quát*). — *Giả sử vành $A$ là chính. Nếu các phức $C$ và $C'$ là tự do, các dãy của A-môđun (11) là khớp và tách; nếu phức $C$ là tự do, các dãy của A-môđun (13) là khớp và tách với mọi A-môđun $N$.*
Thật vậy, $B(C), Z(C)$ và $B(C')$ là các môđun con của các môđun tự do $C, C, C'$, nên là tự do (VII, § 3, hệ quả 2 của định lý 1), và ta áp dụng hệ quả 2.

#### Hệ quả 4 (« công thức Künneth ») {#alg-x-s4-lem-4-cor-4 .statement}

Giả sử C bị chặn bên phải, C và H(C) phẳng; khi đó đồng cấu chính tắc

$$
\gamma(C, C') : H(C) \otimes_A H(C') \to H(C \otimes_A C')
$$

là song ánh.

Theo định lý, chỉ cần chứng minh rằng $B(C)$ và $Z(C)$ là phẳng. Bây giờ ta có các dãy khớp

$$
\begin{align*}
0 &\to B_n(C) \to Z_n(C) \to H_n(C) \to 0 \\
0 &\to Z_n(C) \to C_n \to B_{n-1}(C) \to 0,
\end{align*}
$$

do đó, theo X, p. 75, hệ quả 1, các kéo theo (B_{n-1}(C) là phẳng) $\Rightarrow$ (Z_n(C) là phẳng) $\Rightarrow$ (B_n(C) là phẳng) ; ta kết luận bằng cách nhận xét rằng B_n(C) = 0 với n đủ nhỏ.

#### Hệ quả 5 {#alg-x-s4-lem-4-cor-5 .statement}

Cho u : C \to C' là một đồng luân của các phức của a-môđun phải, phẳng và bị chặn bên phải. Với mọi phức E của các a-môđun trái, cấu xạ $u \otimes 1_E : C \otimes_A E \to C' \otimes_A E$ là một đồng luân.

Thật vậy, Con (u) là một phức phẳng, bị chặn bên phải và có đồng điều không; khi đó có $H(Con (u) \otimes_A E) = 0$ theo hệ quả 4, do đó $H(Con (u \otimes 1_E)) = 0$ (X, p. 67, bổ đề 2), và $u \otimes 1_E$ là một đồng luân.

### 8. Các phức bị chặn và phẳng trên một vành Noether

#### Mệnh đề 11 {#alg-x-s4-prop-11 .statement}

Giả sử A Noether trái, và cho C là một phức bị chặn và phẳng của các a-môđun trái sao cho H(C) là một a-môđun sinh hữu hạn. Cho a và b là hai số nguyên sao cho a \leq b và H_n(C) = 0 với n < a, C_n = 0 với n > b. Tồn tại một phức P của các a-môđun trái sao cho P_n là xạ ảnh và sinh hữu hạn với mỗi n, và P_n = 0 với n \notin [a, b], cùng một đồng luân u : P \to C. Hơn nữa, với mọi phức E của các a-môđun phải, đồng cấu

$$
H(1_E \otimes u) : H(E \otimes_A P) \to H(E \otimes_A C) \quad \text{là song ánh}.
$$

Theo X, p. 53, mệnh đề 7, tồn tại một phức (L, d) sao cho L_n là tự do và sinh hữu hạn với mỗi n, và không với n < a, cùng một đồng luân f : L \to C. Gọi P là phức thương L/L', trong đó L'_n = 0 với n < b, L'_n = L_n với n > b, L'_b = B_b(L). Vì C_n = 0 với n > b, f(L') = 0, nên f phân tích qua một cấu xạ của các phức u : P \to C.

$$
\begin{array}{ccccccccc}
\ldots & \longrightarrow & L_{b+1} & \xrightarrow{d_{b+1}} & L_b & \xrightarrow{d_b} & L_{b-1} & \longrightarrow & \ldots \\
& & \downarrow & & \downarrow & & \downarrow & & \\
& & 0 & \longrightarrow & P_b & \longrightarrow & P_{b-1} & \longrightarrow & \ldots \\
& & \downarrow & & \downarrow^{u_b} & & \downarrow^{u_{b-1}} & & \\
& & 0 & \longrightarrow & C_b & \longrightarrow & C_{b-1} & \longrightarrow & \ldots
\end{array}
$$

Vì $f$ là một đồng luân, ta có $H(\operatorname{Con}(f))=0$, do đó có một dãy khớp

$$
\cdots \longrightarrow L_{b+1} \xrightarrow{d_{b+1}} L_b \longrightarrow L_{b-1}\oplus C_b \longrightarrow L_{b-2}\oplus C_{b-1} \longrightarrow \cdots
$$

Khi đó có một dãy khớp

$$
0\longrightarrow P_b\longrightarrow L_{b-1}\oplus C_b\longrightarrow L_{b-2}\oplus C_{b-1}\longrightarrow\cdots.
$$

Điều này chỉ ra một mặt rằng nón của $u$ có đồng điều không, do đó $u$ là một đồng luân, mặt khác rằng môđun $P_b$ là *phẳng* (X, p. 76, hệ quả 2) ; vì $P_b$ là sinh hữu hạn như một thương của $L_{b+1}$, nó là *xạ ảnh* (X, p. 13, hệ quả). Cặp $(P,u)$ khi đó thỏa mãn điều kiện yêu cầu. Khẳng định cuối cùng suy ra từ X, p. 79, hệ quả 5.

\* **Ví dụ.** — Cho A là một vành giao hoán Noether, X là một lược đồ A-thực sự và phẳng, $\mathcal F$ là một $\mathcal C_X$-môđun thuần nhất, phẳng trên A. Tồn tại một phức bị chặn P gồm các A-môđun xạ ảnh sinh hữu hạn sao cho với mọi A-môđun M, $H(X,\mathcal F\otimes_A M)$ đẳng cấu tự nhiên với $H(P\otimes_A M)$. Thật vậy, cho $\mathcal U$ là một phủ của X bởi một số hữu hạn các tập mở affine, $\mathcal C(\mathcal U,\mathcal F)$ là phức Čech liên kết. Ta chứng minh rằng $H^i(\mathcal C(\mathcal U,\mathcal F))$ đẳng cấu với A-môđun $H^i(X,\mathcal F)$, và rằng môđun sau sinh hữu hạn; hơn nữa, với mọi A-môđun M, phức $\mathcal C(\mathcal U,\mathcal F)\otimes_A M$ đẳng cấu với $\mathcal C(\mathcal U,\mathcal F\otimes_A M)$. Áp dụng Mệnh đề 11 cho phức $\mathcal C(\mathcal U,\mathcal F)$ (là phức bị chặn), ta thu được một phức P trả lời câu hỏi.

Với mọi điểm $y$ của Spec (A), ký hiệu $\kappa(y)$ là trường thặng dư của A tại $y$, $X_y=X\otimes_A\kappa(y)$ là thớ của X trên $y$, $\mathcal F_y=\mathcal F\otimes_A\kappa(y)$, và đặt $h^p(y)=\dim_{\kappa(y)}H^p(X_y,\mathcal F_y)$ với $p\geq 0$.

Từ sự tồn tại của phức P ta dễ dàng suy ra các kết quả sau :

(i) hàm $h^p$ là nửa liên tục trên trên Spec (A) ;

(ii) hàm $\displaystyle\sum_{p\geq 0}(-1)^p h^p$ là hằng địa phương trên Spec (A). \*

### 9. Tổng quát hóa cho các phức đa môđun

Cho B và B′ là hai vành, C là một phức các song môđun (B, A), C′ là một phức các song môđun (A, B′) (X, p. 43); khi đó $(C\otimes_A C',D)$ (X, p. 61) là một phức các song môđun (B, B′) và đồng cấu chính tắc

$$
\gamma:H(C)\otimes_A H(C')\longrightarrow H(C\otimes_A C')
$$

tương thích với các cấu trúc song môđun (B, B′) của hai thành phần.

Nếu B″ là một vành thứ ba, và C″ là một phức các song môđun (B′, B″), đồng cấu chính tắc (II, p. 64, Mệnh đề 8)

$$
(C\otimes_A C')\otimes_{B'}C''\longrightarrow C\otimes_A(C'\otimes_{B'}C'')
$$

là một đẳng cấu của các phức các song môđun (B, B″).

Tổng quát hơn, ta để cho độc giả phát triển lý thuyết các tích tenxơ của các họ hữu hạn, được sắp thứ tự toàn phần, của các *phức đa môđun* theo mô hình của No. 1 (X, p. 63) và của II, pp. 65–72 (tính kết hợp, tính giao hoán, … các đẳng cấu).

Cho B và B' là hai vành, M là một song môđun (B, A), N là một song môđun (A, B') :
khi đó $L(M)\otimes_A L(N)$ là một phức các song môđun (B, B') sao cho $\operatorname{Tor}^A(M,N)$ được trang bị một cấu trúc tự nhiên của song môđun phân bậc (B, B'); trên số hạng có bậc 0, cấu trúc này trùng với cấu trúc của $M\otimes_A N$.

Nếu $\lambda\in B$, $\lambda'\in B'$, và nếu ta ký hiệu bởi $\lambda_M,\lambda_N,\lambda_T,\lambda'_T$ các tự đồng cấu vị xạ $x\mapsto\lambda x$, $y\mapsto y\lambda'$, $z\mapsto\lambda z$, $z\mapsto z\lambda'$ của $M$, $N$, $\operatorname{Tor}^A(M,N)$, $\operatorname{Tor}^A(M,N)$ tương ứng, thì

$$
\lambda_T=\operatorname{Tor}^A(\lambda_M,1_N),\qquad
\lambda'_T=\operatorname{Tor}^A(1_M,\lambda_N'),
$$

điều này cho một mô tả khác của cấu trúc song môđun của $\operatorname{Tor}^A(M,N)$.
Ta để cho độc giả tổng quát hóa các No. 5 và 7 sang trường hợp các phức đa môđun.

## BÀI TẬP {#alg-x-s4-exercises}

Xem các [bài tập cho § 4](exercises/s4/).
