---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 9
section_title: Complexes de Koszul
lang: vi
source: alg-x-fr
book_pages: A X.147-A X.168, A X.206-A X.216
pdf_pages: 0153-0174, 0212-0222
extraction: ocr
subsections:
    - "no": 1
      title: Les complexes $\mathbf{K}(u)$, $\mathbf{K}.(u, C)$, $\mathbf{K}^*(u, C)$
      page: 147
      pdf_page: 153
    - "no": 2
      title: Fonctorialité
      page: 150
      pdf_page: 156
    - "no": 3
      title: 'Exemple 1 : le complexe $S(L) \otimes_A \Lambda(L)$'
      page: 151
      pdf_page: 157
    - "no": 4
      title: 'Exemple 2 : le cas d’un module libre'
      page: 153
      pdf_page: 159
    - "no": 5
      title: 'Exemple 3 : le cas $L = A$'
      page: 156
      pdf_page: 162
    - "no": 6
      title: Familles complètement sécantes
      page: 157
      pdf_page: 163
    - "no": 7
      title: Un critère pour les suites complètement sécante
      page: 159
      pdf_page: 165
    - "no": 8
      title: 'Démonstration du théorème 1 : première partie'
      page: 161
      pdf_page: 167
    - "no": 9
      title: 'Démonstration du théorème 1 : deuxième partie'
      page: 163
      pdf_page: 169
    - "no": 10
      title: Classe d’extensions associée à une suite régulière
      page: 165
      pdf_page: 171
statements: 35
exercises: 10
content_sha256: ed1304e6db2314c2ae8eedb4ce30088be617c24666b5ce7897387096857e1bbe
translated_from: content/en-mt/alg/X/09_s9_complexes_de_koszul.md
source_lang: en-mt
translation_method: machine
source_content_sha256: d4957bb3ac1fc8e376a572314bfd00cbabab87776df84d39b3e13113c9574cf0
translation_model: gpt-5.4
translation_run: translate-vi-e14adcd1
glossary_version: 34
glossary_terms_sha256: ad0a09c2cfaec71469e5f1699122149fa889d2e2d9debc8b3d92c6d9dd9090f3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. CÁC PHỨC KOSZUL

Trong đoạn này, mọi vành được xét đều giao hoán.

### 1. Các phức $\mathbf{K}(u)$, $\mathbf{K}.(u, C)$, $\mathbf{K}^*(u, C)$

Cho $A$ là một vành, $L$ một $A$-môđun, $u : L \to A$ một dạng tuyến tính, và $\Lambda(L)$ là đại số ngoài của $A$-môđun $L$. Với $x \in \Lambda(L)$, ký hiệu bởi $d_u(x)$ tích trong $x \cdot u$ (III, p. 161, ví dụ). Theo nơi đã dẫn, p. 162, công thức (60), ta có

$$
(1)\quad d_u(e_1 \wedge \ldots \wedge e_n) = \sum_{i=1}^n (-1)^{i+1} u(e_i) \; e_1 \wedge \ldots \wedge e_{i-1} \wedge e_{i+1} \wedge \ldots \wedge e_n
$$

với $e_1, \ldots, e_n$ trong $L$. Theo III, p. 164 và 165, ánh xạ $d_u : \Lambda(L) \to \Lambda(L)$ là một phép phản vi phân bậc $(-1)$ và có bình phương bằng không. Đó là phép phản vi phân duy nhất của $A$-đại số $\Lambda(L)$ mở rộng $u : \Lambda^1(L) \to \Lambda^0(L)$.

#### Định nghĩa 1 {#alg-x-s9-def-1 .statement}

Phức $(\Lambda(L), d_u)$ được ký hiệu bởi $\mathbf{K}^A(u)$ hoặc $\mathbf{K}(u)$.

Cần chú ý rằng $\mathbf{K}_n(u) = \Lambda^n(L) = \mathbf{K}^{-n}(u)$. Rõ ràng $\mathbf{K}(u)$ bằng không ở bên phải và $H_0(\mathbf{K}(u)) = \mathrm{Coker}\,(u) = A/q$ trong đó $q$ là iđêan $u(L)$ của $A$.

Với mọi phức các $A$-môđun $C$, đặt

$$
\begin{aligned}
\mathbf{K}^A(u, C) &= C \otimes_A \mathbf{K}^A(u), \\
H^A(u, C) &= H(C \otimes_A \mathbf{K}^A(u)) \\
H_r^A(u, C) &= H_r(C \otimes_A \mathbf{K}^A(u)),
\end{aligned}
$$
$$
\begin{aligned}
\mathbf{K}^*_A(u, C) &= \mathrm{Homgr}_A(\mathbf{K}^A(u), C), \\
H^*_A(u, C) &= H(\mathrm{Homgr}_A(\mathbf{K}^A(u), C)), \\
H^r_A(u, C) &= H^r(\mathrm{Homgr}_A(\mathbf{K}^A(u), C)).
\end{aligned}
$$

Do đó có các đồng cấu chính tắc của các $A$-môđun (X, p. 62 và p. 82)

$$
\begin{aligned}
\gamma_0 : H_0(C) \otimes_A A/q &\to H^A_0(u, C), \\
\lambda^0 : H^0_A(u, C) &\to \mathrm{Hom}_A(A/q, H^0(C)).
\end{aligned}
$$

#### Bổ đề 1 {#alg-x-s9-lem-1 .statement}

Nếu phức $C$ bằng không ở bên phải (tương ứng ở bên trái), thì $\mathbf{K}^A(u, C)$ (tương ứng $\mathbf{K}^*_A(u, c)$) bằng không ở bên phải (tương ứng ở bên trái), và $\gamma_0$ (tương ứng $\lambda^0$) là song ánh.

Điều này suy ra từ X, p. 62, mệnh đề 1 và p. 82, mệnh đề 1.

#### Mệnh đề 1 {#alg-x-s9-prop-1 .statement}

Cho $x \in L$; ký hiệu bởi $R_x : y \mapsto x \wedge y$ phép nhân trái bởi $x$ trong đại số $\Lambda(L)$. Khi đó $d_u \circ R_x + R_x \circ d_u = u(x) \cdot 1_{\Lambda(L)} = u(x)_{\Lambda(L)}$.

Thật vậy $(d_u \circ R_x + R_x \circ d_u)(y) = d_u(x \wedge y) + x \wedge d_u(y)$; vì $d_u$ là một phép phản vi phân, $d_u(x \wedge y) + x \wedge d_u(y) = d_u(x) \wedge y = u(x) \cdot y$.

#### Hệ quả 1 {#alg-x-s9-prop-1-cor-1 .statement}

Nếu $u$ là toàn ánh, $K(u)$ đồng luân với không (X, p. 34) cũng như $K^A(u, C)$ và $K_A^*(u, C)$ với mọi phức $C$.

Thật vậy, tồn tại $x \in L$ sao cho $u(x) = 1$. Khi đó $K(u)$ đồng luân với không theo mệnh đề 1, và do đó $K^A(u, C)$ (X, p. 64, mệnh đề 3) và $K_A^*(u, C)$ (X, p. 83, mệnh đề 3) cũng vậy.

#### Hệ quả 2 {#alg-x-s9-prop-1-cor-2 .statement}

Cho $C$ là một phức, Ann (C) là linh hóa tử của nó. Khi đó $q + \mathrm{Ann}(C)$ linh hóa $H^A(u, C)$ và $H_A^*(u, C)$.

Với mọi $\lambda \in q$, phép vị tự $\lambda_{K(u)}$ đồng luân với không theo mệnh đề, do đó $1_C \otimes \lambda_{K(u)}$ và Homgr ($\lambda_{K(u)}, 1_C$) cũng vậy theo X, p. 64, mệnh đề 3 và X, p. 83, mệnh đề 3; suy ra $\lambda$ linh hóa $H(u, C)$ và $H^*(u, C)$. Nếu $\lambda \in \mathrm{Ann}(C)$, thì $1_{K(u)} \otimes \lambda_C$ và Homgr ($1_{K(u)}, \lambda_C$) bằng không.

Giả sử $L$ xạ ảnh (tương ứng, $K(u)$ không chu trình ở các bậc > 0). Khi đó phức $\Lambda(L)$ là xạ ảnh theo III, p. 87, hệ quả 2 (tương ứng, là một giải của $A/q$); do đó theo X, p. 102 (tương ứng, p. 100), với mọi $A$-môđun $M$, ta có các đồng cấu

(2) $H_r^A(u, M) \to \mathrm{Tor}_r^A(A/q, M)$, $\mathrm{Ext}_A^r(A/q, M) \to H_r^A(u, M)$
tương ứng.
(3) $\mathrm{Tor}_r^A(A/q, M) \to H_r^A(u, M)$, $H_r(u, M) \to \mathrm{Ext}_A^r(A/q, M)$.

Nếu $L$ là xạ ảnh và $K(u)$ không chu trình ở các bậc > 0, thì các đồng cấu (2) và (3) ở trên là song ánh và đối ứng nhau (X, p. 102, mệnh đề 1).

#### Mệnh đề 2 {#alg-x-s9-prop-2 .statement}

Cho $(L_i)_{i \in I}$ là một họ các $A$-môđun, trong đó tập hợp $I$ là hữu hạn và được sắp thứ tự toàn phần. Cho $u$ là một dạng tuyến tính trên $\bigoplus_{i \in I} L_i$, $u_i$ là hạn chế của nó lên $L_i$.

Đẳng cấu chính tắc của các $A$-đại số (III, p. 84)

$$
g : \bigotimes_{i \in I} \Lambda(L_i) \to \Lambda(\bigoplus_{i \in I} L_i)
$$

là một đẳng cấu của phức $\bigotimes_{i \in I} K(u_i)$ (X, p. 63) lên phức $K(u)$.

Thật vậy, theo X, p. 64, nhận xét 4, vi phân $D$ của phức $\bigotimes_{i \in I} K(u_i)$ là một phản đạo hàm; các phản đạo hàm $d_u$ và $g \circ D \circ g^{-1}$ của $\Lambda(\bigoplus L_i)$ trùng nhau trên $\bigoplus L_i$ với ánh xạ $x \mapsto u(x).1$ từ $\bigoplus L_i$ vào $\Lambda(\bigoplus L_i)$, do đó bằng nhau (III, p. 128, hệ quả).

Cho $C$ và $C'$ là hai phức các $A$-môđun. Ta có (X, p. 63 và p. 99) các đẳng cấu chính tắc của các phức

$$
C \otimes_A (C' \otimes_A K(u)) \to (C \otimes_A C') \otimes_A K(u)
$$
$$
\mathrm{Homgr}_A(C', \mathrm{Homgr}_A(K(u), C)) \to \mathrm{Homgr}_A(C' \otimes_A K(u), C),
$$

nghĩa là, các *đẳng cấu*

(4) $$
C \otimes_A K^A(u, C') \to K^A(u, C \otimes_A C')
$$

(5) $$
\operatorname{Homgr}_A(C', K^i_A(u, C)) \to \operatorname{Homgr}_A(K^A(u, C'), C)
$$

Trong (4) và (5), lấy $C' = K(u')$, trong đó $u' : L' \to A$ là một dạng tuyến tính trên một $A$-môđun $L'$, và chú ý rằng $K^A(u, K(u'))$ mà theo định nghĩa bằng $K(u') \otimes_A K(u)$ được đồng nhất, theo Mệnh đề 2, với $K(u' \oplus u)$ trong đó $u' \oplus u : L' \oplus L \to A$ là dạng tuyến tính $(x', x) \mapsto u'(x') + u(x)$. Khi đó ta thu được các đẳng cấu của các phức

(6) $$
K^A(u' \oplus u, C) \to K^A(u, K^A(u', C))
$$

(7) $$
K^i_A(u', K^i_A(u, C)) \to K^i_A(u' \oplus u, C)
$$

Chuyển qua đồng điều, ta suy ra các đẳng cấu của các $A$-môđun

$$
H^A_r(u' \oplus u, C) \to H^A_r(u, K^A(u', C)) , \qquad r \in \mathbf{Z} ,
$$
$$
H^r_A(u', K^i_A(u, C)) \to H^r_A(u' \oplus u, C) , \qquad r \in \mathbf{Z} .
$$

Sau cùng, chú ý rằng đồng cấu suy ra từ tích trong đại số $\Lambda(L)$

$$
m : K^A(u) \otimes_A K^A(u) \to K^A(u)
$$

là một cấu xạ của *các phức* (vì $d_u$ là một phản đạo hàm). Giả sử rằng $L$ là *tự do hạng n* và hợp thành với cấu xạ của các phức $K^A(u) \to \Lambda^n L(-n)$ là đồng nhất thức ở bậc $n$, ta suy ra một cấu xạ của các phức

$$
\chi : K^A(u) \otimes_A K^A(u) \to \Lambda^n L(-n) ;
$$

với cấu xạ này tương ứng một cách chính tắc, theo X, p. 99, Prop. 12, một cấu xạ của các phức

$$
\varphi : K^A(u) \to \operatorname{Homgr}_A(K^A(u), \Lambda^n L(-n))
$$

mà là *song ánh* (III, p. 87, công thức (20)). Với mọi phức $C$, ta suy ra một đẳng cấu hợp thành

$$
K^A(u, C) = C \otimes_A K^A(u) \xrightarrow{1 \otimes \varphi} C \otimes \operatorname{Homgr}_A(K^A(u), \Lambda^n L(-n)) \to \\
\to \operatorname{Homgr}_A(K^A(u), C \otimes_A \Lambda^n L(-n)) = K^i_A(u, C \otimes_A \Lambda^n L(-n)) .
$$

Chuyển qua đồng điều, do đó ta có các đẳng cấu *chính tắc*

(8) $$
H^A_r(u, C) \to H^{n-r}_A(u, C \otimes_A \Lambda^n L) , \qquad r \in \mathbf{Z} .
$$

*Nhận xét. — 1)* \* Điều trên vẫn đúng khi $L$ là xạ ảnh hạng $n$. \*

2) Vì $L$ là tự do hạng $n$, $\Lambda^n L$ đẳng cấu với $A$, và ta có các đẳng cấu không chính tắc $H^A_r(u,C)\to H^{n-r}_A(u,C)$.

### 2. Tính hàm tử

Cho $f:C\to C'$ là một cấu xạ của các phức. Ta ký hiệu

$$
K^A(u,f):K^A(u,C)\to K^A(u,C'),
$$

$$
K_A(u,f):K_A(u,C)\to K_A(u,C'),
$$

các cấu xạ của các phức $f\otimes 1_{K(u)}$ và $\operatorname{Hom}_{A}(1_{K(u)},f)$.

Ta ký hiệu bởi $H^A(u,f):H^A(u,C)\to H^A(u,C')$, $H_A(u,f):H_A(u,C)\to H_A(u,C')$,
$H^A_r(u,f):H^A_r(u,C)\to H^A_r(u,C')$, $H^A_r(u,f):H^A_r(u,C)\to H^A_r(u,C')$ các cấu xạ cảm sinh trong đồng điều. Ánh xạ $f\mapsto K^A(u,f)$ là tuyến tính; nếu $g:C'\to C''$ là một cấu xạ khác của các phức, ta có $K^A(u,g\circ f)=K^A(u,g)\circ K^A(u,f)$; tương tự đối với $K_A$, $H^A$, $H_A$, $H^A_r$, $H^A_r$.

Cho $0\to C'\xrightarrow{f}C\xrightarrow{g}C''\to0$ là một dãy khớp của các phức.

a) Giả sử $L$ là phẳng; khi đó $\Lambda(L)$ là phẳng (X, p. 15, Hệ quả). Dãy

$$
0\to K^A(u,C')\xrightarrow{K^A(u,f)}K^A(u,C)\xrightarrow{K^A(u,g)}K^A(u,C'')\to0
$$

khi đó là khớp, và sinh ra (X, p. 30) một dãy khớp của đồng điều

$$
\cdots\to H^A_n(u,C')\xrightarrow{H_n(u,f)}H^A_n(u,C)
\xrightarrow{H_n(u,g)}H^A_n(u,C'')
\xrightarrow{\partial_n}H^A_{n-1}(u,C')\to\cdots .
$$

b) Giả sử $L$ là xạ ảnh; khi đó $\Lambda(L)$ là xạ ảnh. Dãy

$$
0\to K_A(u,C')\xrightarrow{K_A(u,f)}K_A(u,C)
\xrightarrow{K_A(u,g)}K_A(u,C'')\to0
$$

khi đó là khớp, và sinh ra một dãy khớp của đồng điều

$$
\cdots\to H^n_A(u,C')\xrightarrow{H^n(u,f)}H^n_A(u,C)
\xrightarrow{H^n(u,g)}H^n_A(u,C'')
\xrightarrow{\delta^n}H^{n+1}_A(u,C')\to\cdots .
$$

Cho $\rho:A\to A'$ là một đồng cấu vành, $L'$ là $A'$-môđun $A'\otimes_A L$, $u':L'\to A'$ là dạng tuyến tính $1\otimes u$. Đồng cấu chính tắc song ánh (III, p. 83, Prop. 8)

$$
\psi:\Lambda_{A'}(A'\otimes_A L)\to A'\otimes_A\Lambda_A(L)
$$

là một đẳng cấu của các phức $A'$-môđun. Suy ra rằng:

1) với mọi phức $A'$-môđun $C'$, có một đẳng cấu của các phức $A$-môđun

$$
K^{A'}_{A}(u',C')\to K^A_A(u,C'),
$$

hợp thành bởi biểu đồ

$$
C' \otimes_{A'} (\Lambda_A(A' \otimes_A L)) \xrightarrow{1_C \otimes \psi} C' \otimes_{A'} A' \otimes_A \Lambda_A(L) \to C' \otimes_A \Lambda_A(L)
$$

trong đó $\varphi$ là song ánh chính tắc (III, p. 85, Prop. 14);

2) với mọi phức $A$-môđun $C$, có một *đẳng cấu* của các phức $A'$-môđun

$$
K^A(u, A' \otimes_A C) \to A' \otimes_A K^A(u, C),
$$

do đó có các đồng cấu $A'$-môđun

$$
A' \otimes_A H_n^A(u, C) \to H_n^{A'}(u', A' \otimes_A C),
$$

là song ánh khi $A'$ là *phẳng* trên $A$ (X, p. 66, Cor. 2).

Cho $L'$ là một $A$-môđun, $u' : L' \to A$ là một dạng tuyến tính, $f : L \to L'$ là một $A$-đồng cấu sao cho $u' \circ f = u$. Từ III, p. 161, công thức (55), suy ra đồng cấu $\Lambda(f) : \Lambda(L) \to \Lambda(L')$ thỏa mãn $d_u \circ \Lambda(f) = \Lambda(f) \circ d_{u'}$, do đó xác định một *cấu xạ của các phức* $\Lambda(u) : K^A(u) \to K^A(u')$. Nếu $C$ là một $A$-phức, suy ra có các cấu xạ của các phức

$1_C \otimes \Lambda(u) : K^A(u, C) \to K^A(u', C)$ và $\mathrm{Homgr}(\Lambda(u), 1_C) : K_A^*(u', C) \to K_A^*(u, C)$.

Nếu $f$ là song ánh, thì tất cả các cấu xạ này đều là các đẳng cấu.

### 3. Ví dụ 1: phức $S(L) \otimes_A \Lambda(L)$

Cho $A$ là một vành, $L$ là một $A$-môđun, $S(L)$ là đại số đối xứng của nó, $S(L) \otimes_A L$ là $S(L)$-môđun thu được bằng mở rộng vô hướng, $u : S(L) \otimes_A L \to S(L)$ là dạng tuyến tính sao cho $u(s \otimes x) = sx$ với $s \in S(L), x \in L$. Bởi đẳng cấu chính tắc của các $S(L)$-môđun (III, p. 83, Prop. 8)

$$
\Lambda_{S(L)}(S(L) \otimes_A L) \to S(L) \otimes_A \Lambda(L),
$$

vi phân của phức $K^{S(L)}(u)$ được chuyển thành ánh xạ

$$
d : S(L) \otimes_A \Lambda(L) \to S(L) \otimes_A \Lambda(L)
$$

sao cho, với $x_1, ..., x_p, y_1, ..., y_q$ trong $L$, ta có

$$
\begin{align}
(9) \quad d((x_1 ... x_p) \otimes (y_1 \wedge ... \wedge y_q)) \\
&= \sum_{i=1}^q (-1)^{i+1} y_i x_1 ... x_p \otimes (y_1 \wedge ... \wedge y_{i-1} \wedge y_{i+1} \wedge ... \wedge y_q).
\end{align}
$$

Chú ý rằng $d$ biến $S^p(L) \otimes \Lambda^q(L)$ thành $S^{p+1}(L) \otimes \Lambda^{q-1}(L)$, do đó *phức các $A$-môđun* $S(L) \otimes \Lambda(L)$ phân tích thành tổng trực tiếp của các phức được mô tả bởi các biểu đồ sau:

$$
(\mathcal{E}_n) : 0 \to S^0 L \otimes_A \Lambda^n L \to S^1 L \otimes_A \Lambda^{n-1} L \to ... \to S^n L \otimes_A \Lambda^0 L \to 0, \quad n \in \mathbf{N}.
$$

Nếu A-môđun L là tổng trực tiếp của một họ hữu hạn $(L_i)_{i \in I}$ trong đó I được sắp thứ tự toàn phần, song ánh chính tắc

$$
\bigotimes_{i \in I} (\mathbf{S}(L_i) \otimes_A \Lambda(L_i)) \to \mathbf{S}(L) \otimes_A \Lambda(L)
$$

là một đẳng cấu của các phức A-môđun (điều này suy ra từ mệnh đề 2 của X, p. 148 hoặc từ công thức (9) ở trên).

#### Mệnh đề 3 {#alg-x-s9-prop-3 .statement}

*Nếu A-môđun L là phẳng, các dãy $(\mathcal{E}_n)$ ở trên là khớp với $n > 0$.*

*a)* Trước hết ta nhận thấy rằng, nếu $p_L$ là đồng cấu hợp thành

$$
\mathbf{S}(L) \otimes \Lambda(L) \xrightarrow{\alpha} \mathbf{S}^0(L) \otimes \Lambda^0(L) \xrightarrow{\beta} A,
$$

trong đó $\alpha$ là tích tenxơ của các phép chiếu chính tắc và $\beta$ là đẳng cấu chính tắc, thì chỉ còn phải chứng minh rằng $H(p_L)$ là *song ánh*.

*b)* Nếu $L = 0$ hoặc nếu $L = A$, mệnh đề là hiển nhiên.

*c)* Giả sử L là tự do hạng hữu hạn; viết nó thành tổng trực tiếp $L_1 \oplus ... \oplus L_n$ của các A-môđun tự do hạng 1. Theo nhận xét đứng trước mệnh đề, phức $\mathbf{S}(L) \otimes \Lambda(L)$ đẳng cấu với tích tenxơ của $n$ phức *tự do* $\mathbf{S}(L_i) \otimes \Lambda(L_i)$ mà đồng điều của chúng là *tự do* theo *b)*. Theo X, p. 79, hệ quả 4, đồng cấu chính tắc

$$
\gamma : \bigoplus_{i=1}^n H(\mathbf{S}(L_i) \otimes \Lambda(L_i)) \to H(\mathbf{S}(L) \otimes \Lambda(L))
$$

là song ánh. Theo *b)*, $H(p_{L_i})$ là song ánh với mọi $i$. Vì $\bigotimes_{i=1}^n H(p_{L_i}) = H(p_L) \circ \gamma$,

$$
H(p_L) \text{ là song ánh}.
$$

*d)* Trong trường hợp tổng quát, L là giới hạn quy nạp của một hệ quy nạp lọc $(L_i)_{i \in I}$ gồm các môđun tự do hạng hữu hạn (X, p. 14, định lý 1). Vì đồng cấu chính tắc song ánh

$$
\varprojlim \mathbf{S}(L_i) \otimes \Lambda(L_i) \to \mathbf{S}(L) \otimes \Lambda(L)
$$

là một đẳng cấu của các phức, mệnh đề suy ra từ X, p. 28, mệnh đề 1.

#### Nhận xét 1 {#alg-x-s9-n3-rem-1 .statement}

Ta sẽ thấy ở dưới (X, p. 158, ví dụ) một chứng minh khác của phần *c)* ở trên.

#### Nhận xét 2 {#alg-x-s9-n3-rem-2 .statement}

Nếu A là một $\mathbf{Q}$-đại số, kết luận của mệnh đề 3 vẫn đúng mà không cần giả thiết nào trên L (*cf.* X, p. 206, bài tập 1).

#### Nhận xét 3 {#alg-x-s9-n3-rem-3 .statement}

Cho G là một nhóm và $\rho : G \to \mathbf{GL}(L)$ một biểu diễn tuyến tính của G trong một A-môđun phẳng L. Khi đó các $(\mathcal{E}_n)$ là các dãy khớp của các biểu diễn tuyến tính. Giả sử L xạ ảnh sinh hữu hạn, và ký hiệu $R_A(G)$ là vành biểu diễn của G trong các A-môđun xạ ảnh sinh hữu hạn. Từ mệnh đề 3 suy ra rằng trong R_A(G) ta có các hệ thức

$$
\sum_{i=0}^{n} (-1)^i [\mathbf{S}^i(L)] [\Lambda^{n-i}(L)] = 0 , \quad n > 0 .
$$

Nếu ta xét các chuỗi hình thức

$$
s(T) = \sum_{i=0}^{\infty} [\mathbf{S}^i(L)] T^i \in R_A(G)[[T]] ,
$$
$$
\lambda(T) = \sum_{i=0}^{\infty} [\Lambda^i(L)] T^i \in R_A(G)[[T]] ,
$$

thì các hệ thức (10) được viết thành

$$
s(T) \lambda(-T) = 1_* .
$$

### 4. Ví dụ 2 : trường hợp của một môđun tự do

Cho k là một vành, M một k-môđun, I một tập hợp và p một số nguyên $\geqslant 0$. Một ánh xạ $m : I^p \to M$ được gọi là *phản xứng* nếu nó thỏa mãn hai điều kiện sau:

a) với mọi phép hoán vị $\sigma \in S_p$ và mọi dãy $(\alpha_1, ..., \alpha_p) \in I^p$, ta có

$$
m(\alpha_{\sigma(1)}, ..., \alpha_{\sigma(p)}) = \varepsilon_{\sigma} m(\alpha_1, ..., \alpha_p) ,
$$

b) với mọi dãy $(\alpha_1, ..., \alpha_p) \in I^p$ sao cho hai trong các chỉ số $\alpha_1, ..., \alpha_p$ bằng nhau, ta có $m(\alpha_1, ..., \alpha_p) = 0$.
(Trong trường hợp I là một k-môđun và m là đa tuyến tính, ta thu lại khái niệm được đưa vào ở III, p. 80.)

*Giả sử I hữu hạn* và ký hiệu $C_I^p(M)$ là k-môđun các ánh xạ phản xứng từ $I^p$ vào M.

Cho $L_0$ là một k-môđun, $(e_i)_{i \in I}$ một họ các phần tử của $L_0$; ta định nghĩa hai ánh xạ k-tuyến tính

$$
g : \mathrm{Hom}_k (\Lambda^p L_0, M) \to C_I^p(M)
$$
$$
h : C_I^p(M) \to M \otimes_k \Lambda^p L_0
$$

như sau: nếu $f \in \mathrm{Hom}_k (\Lambda^p L_0, M)$, ta đặt

$$
g(f)(\alpha_1, ..., \alpha_p) = f(e_{\alpha_1} \wedge ... \wedge e_{\alpha_p}) ;
$$

cho $m \in C_I^p(M)$, định nghĩa $h(m) \in M \otimes_k \Lambda^p L_0$. Với mọi phần tử $(\alpha_1, ..., \alpha_p)$ của $I^p$, phần tử $m(\alpha_1, ..., \alpha_p) \otimes (e_{\alpha_1} \wedge ... \wedge e_{\alpha_p})$ của $\Lambda^p L_0 \otimes_k M$ bằng không nếu $\mathrm{Card}\{ \alpha_1, ..., \alpha_p \} < p$ và độc lập với thứ tự của các chỉ số $\alpha_1, ..., \alpha_p$ nếu
$$
\mathrm{Card}\{ \alpha_1, ..., \alpha_p \} = p .
$$
Nó chỉ phụ thuộc vào tập con $J = (\alpha_1, ..., \alpha_p)$ của $I$; ký hiệu nó bởi $h_J(m)$; ta có $h_J(m) = 0$ nếu $\mathrm{Card}(J) < p$; khi đó ta đặt:
$$
h(m) = \sum_J h_J(m) ,
$$
trong đó $J$ chạy qua các tập con của $I$ có $p$ phần tử.

#### Bổ đề 2 {#alg-x-s9-lem-2 .statement}

*Nếu K-môđun $L_0$ là tự do với cơ sở $(e_i)_{i \in I}$, thì các ánh xạ K-tuyến tính g và h là song ánh.*
Điều này suy ra từ III, p. 79, đ. l. 1.

Cho $M$ là một $k$-môđun, và cho $x = (x_i)_{i \in I}$ là một họ các $k$-endomorphism của $M$, từng đôi một giao hoán. Xét vành đa thức $A = k[(X_i)_{i \in I}]$ và trang bị cho $M$ cấu trúc của một $A$-môđun sao cho $P(X_i) m = P(x_i) m$ với $P \in A$ và $m \in M$. Hơn nữa, cho $L$ là $A$-môđun tự do $A^I$, $(e_i)_{i \in I}$ là cơ sở chính tắc của nó và $u : L \to A$ là dạng tuyến tính ánh xạ $e_i$ lên $X_i$ với mọi $i \in I$. Xét các phức của các $k$-môđun $K_A^*(u, M)$ và $K_A^*(u, M)$; ta có các *đẳng cấu chính tắc*
$$
K_A^p(u, M) = \mathrm{Hom}_A(\Lambda_A^p(A^I), M) \to \mathrm{Hom}_k(\Lambda_k^p(k^I), M) ,
$$
$$
M \otimes_k \Lambda_k^p(k^I) \to M \otimes_A \Lambda_A^p(A^I) = K_A^p(u, M) ;
$$
do đó, bằng hợp thành với các đẳng cấu $g$ và $h$, các *đẳng cấu của các $k$-môđun*
$$
\theta^p : K_A^p(u, M) \to C_I^p(M) ,
$$
$$
\theta_p : C_I^p(M) \to K_A^p(u, M) .
$$
Ta ký hiệu bởi
$$
\partial^p : C_I^p(M) \to C_I^{p+1}(M) ,
$$
$$
\partial_p : C_I^p(M) \to C_I^{p-1}(M) ,
$$
các đồng cấu $k$ thu được bằng cách chuyển các vi phân của $K_A^*(u, M)$ và $K_A^*(u, M)$ qua các đẳng cấu $\theta$. Chẳng hạn, ta có:
(12) $$
(\partial^p m)(\alpha_1, ..., \alpha_{p+1}) = \sum_{j=1}^{p+1} (-1)^{j+1} x_{\alpha_j} m(\alpha_1, ..., \alpha_{j-1}, \alpha_{j+1}, ..., \alpha_{p+1}) .
$$
Phức được tạo thành bởi các $C_I^p(M)$ và các $\partial^p$ (resp. các $\partial_p$) được ký hiệu là $K^*(x, M)$ (resp. $K.(x, M)$) và được gọi là *phức Koszul tăng (resp. giảm)* liên kết với môđun M và dãy các endomorphism $(x_1, ..., x_n)$. Vì thế ta có các đẳng cấu của các phức của các $k$-môđun

$$
\theta^*: K_A^*(u, M) \to K^*(x, M),
$$
$$
\theta_*: K_*(x, M) \to K_A^*(u, M).
$$

#### Nhận xét {#alg-x-s9-n4-rem-1 .statement}

Ngược lại, cho B là một $k$-đại số, L là một B-môđun tự do với cơ sở $(e_i)_{i \in I}$, và M là một B-môđun. Việc cho một dạng tuyến tính $u : L \to B$ tương đương với việc cho một họ $x = (x_i)_{i \in I}$ các phần tử của B, theo quan hệ $x_i = u(e_i)$. Khi đó phức nền của các $k$-môđun của $K_B^*(u, M)$ (resp. $K^B(u, M)$) được đồng nhất, bởi đẳng cấu $\theta^*$ (resp. $\theta_*$), với phức Koszul $K^*(x, M)$ (resp. $K_*(x, M)$). Chẳng hạn $K^B(u)$ được đồng nhất với $K^*(x, B)$.

Các ký hiệu $H_*(x, M)$, $H_*(x, M)$, v.v., được đưa vào như trong No. 1 (X, p. 147), và mọi kết quả của Nos. 1 và 2 đều áp dụng được với những thay đổi thích hợp, môđun $A^I$ là tự do. Chẳng hạn ta có các đẳng cấu

$$
H_0(x, M) \to M/(x) M
$$
$$
H^0(x, M) \to \operatorname{Hom}_A(A/(x), M),
$$

trong đó $(x)$ ký hiệu iđêan $\sum A x_i$ của A. Chẳng hạn nữa, nếu $K_*(x, A)$ là vô chu trình ở các bậc $> 0$, ta có các đẳng cấu

$$
H_r(x, M) \to \operatorname{Tor}_r^A(k, M),
$$
$$
\operatorname{Ext}_A^r(k, M) \to H^r(x, M).
$$

Sau cùng, giả sử rằng I là (hữu hạn và) được sắp thứ tự toàn phần, chẳng hạn $I = \{ 1, ..., n \}$; đồng nhất $\Lambda^n(A^I)$ với A nhờ phần tử cơ sở $e_1 \wedge ... \wedge e_n$ và chuyển đẳng cấu $K_p^A(u, M) \to K_A^{n-p}(u, M)$ của X, p. 149. Khi đó nó trở thành, nhờ phép chuyển bởi $(\theta_p)$ và $(\theta^{n-p})$, đẳng cấu

$$
C_1^p(M) \to C_1^{n-p}(M)
$$

gắn với $m \in C_1^p(M)$ phần tử $\tilde{m}$ của $C_1^{n-p}(M)$ sao cho

$$
m(\alpha_1, ..., \alpha_p) = \tilde{m}(\beta_1, ..., \beta_{n-p})
$$

nếu $(\alpha_1, ..., \alpha_p, \beta_1, ..., \beta_{n-p})$ là một phép hoán vị *chẵn* của $\{ 1, ..., n \}$. Ta cũng nhận xét rằng khi $I = \{ 1, ..., n \}$, ta có thể đồng nhất $C_1^p(M)$ với tập hợp các họ $m(\alpha_1, ..., \alpha_p)$ các phần tử của M trong đó $\alpha_1 < \alpha_2 < ... < \alpha_p$; công thức (12) vẫn đúng, cũng như quan hệ (13).

#### Ví dụ {#alg-x-s9-n4-exa-1 .statement}

Lấy $M = k[T_1, ..., T_n]$; phức Koszul $K (\partial/\partial T, M)$ liên kết với dãy các nội cấu $(\partial/\partial T_1, ..., \partial/\partial T_n)$ được đồng nhất với phức de Rham của $k[x_1, ..., x_n]$ trên $k$ (X, p. 44): với $m \in C_{\{1,...,n\}}^p(M)$, ta gắn dạng vi phân

$$
\omega(m) = \sum_{\alpha_1 < ... < \alpha_p} m(\alpha_1, ..., \alpha_p)\ dx_{\alpha_1} \wedge ... \wedge dx_{\alpha_p},
$$

xem công thức (12) và Ví dụ 1, p. 44.

### 5. Ví dụ 3 : trường hợp $L = A$

Nếu $L = A$, đặt $u(1) = x \in A$. Khi đó phức $K(u)$ có độ dài 1, ta có $K_0(u) = K_1(u) = A$ và $d_1(a) = xa$, do đó với mọi A-môđun $M$, $K_0(u, M)$, $K_1(u, M)$, $K^0(u, M)$ và $K^1(u, M)$ được đồng nhất với $M$, các vi phân

$$
d_1 : K_1(u, M) \to K_0(u, M) \quad \text{and} \quad d^0 : K^0(u, M) \to K^1(u, M)
$$

là $m \mapsto xm$. Vậy ta có các đẳng cấu

$$
H_0(x, M) \to A/xA \otimes_A M \leftarrow H^1(x, M),
$$
$$
H_1(x, M) \to \mathrm{Hom}_A(A/xA, M) \leftarrow H^0(x, M).
$$

#### Bổ đề 3 {#alg-x-s9-lem-3 .statement}

Cho $K$ là một phức sao cho $K_i = 0$ với $i \neq 0, 1$, và cho $C$ là một phức và $p$ là một số nguyên.

a) Nếu $K$ là phẳng, thì với mọi $p \in \mathbf{N}$, có một dãy khớp

$$
0 \to H_0(K \otimes_A H_p(C)) \to H_p(K \otimes_A C) \to H_1(K \otimes_A H_{p-1}(C)) \to 0.
$$

b) Nếu $K$ là xạ ảnh, thì với mọi $p \in \mathbf{N}$, ta có một dãy khớp

$$
0 \to H^1(\mathrm{Homgr}_A(K, H^{p-1}(C))) \to H^p(\mathrm{Homgr}_A(K, C))
$$
$$
\to H^0(\mathrm{Homgr}_A(K, H^p(C))) \to 0.
$$

Ta hãy chứng minh a), chứng minh của b) là tương tự. Với mọi $i$, ký hiệu bởi $K_{(i)}$ phức $K_i(-i)$. Ta có một dãy khớp các phức, tách như một dãy các $A$-môđun

$$
0 \to K_{(0)} \xrightarrow{\alpha} K \xrightarrow{\beta} K_{(1)} \to 0;
$$

dãy

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & K_{(0)} \otimes_A C & \xrightarrow{\alpha \otimes 1} & K \otimes_A C & \xrightarrow{\beta \otimes 1} & K_{(1)} \otimes_A C & \longrightarrow & 0
\end{array}
$$

là khớp, và do $K$ phẳng, các đồng cấu

$$
\gamma_{0,p}(K_{(0)}, C) : K_{(0)} \otimes_A H_p(C) \to H_p(K_{(0)} \otimes_A C)
$$
$$
\gamma_{1,p-1}(K_{(1)}, C) : K_{(1)} \otimes_A H_{p-1}(C) \to H_p(K_{(1)} \otimes_A C)
$$

là song ánh (X, p. 66, hệ quả 2). Ta hãy tính đồng cấu nối $\partial(\alpha \otimes 1,\beta \otimes 1)$; theo định nghĩa, nó ánh xạ lớp của chu trình $\sum a_i \otimes b_i$ lên lớp của $\sum d a_i \otimes b_i$, điều đó có nghĩa là

$$
\partial(\alpha \otimes 1,\beta \otimes 1)\circ\gamma(K_{(1)},\mathbf C)=\gamma(K_{(0)},\mathbf C)\circ(d_K\otimes 1).
$$

Do đó dãy đồng điều khớp liên kết với (14) có dạng

$$
K_1\otimes H_p(\mathbf C)\xrightarrow{d_k\otimes 1}K_0\otimes H_p(\mathbf C)\longrightarrow H_p(K\otimes\mathbf C)
$$

$$
\hspace{7cm}\longrightarrow K_1\otimes H_{p-1}(\mathbf C)\xrightarrow{d_k\otimes 1}K_0\otimes H_{p-1}(\mathbf C),
$$

do đó suy ra a).

Áp dụng Bổ đề 3, a) cho phức $K(u)$, và dùng các đẳng cấu giao hoán, ta thu được:

#### Mệnh đề 4 {#alg-x-s9-prop-4 .statement}

*Với mọi phức $C$, có các dãy khớp .*

$$
0\longrightarrow A/xA\otimes_A H_p(C)\longrightarrow H_p(x,C)\longrightarrow \operatorname{Hom}_A(A/xA,H_{p-1}(C))\longrightarrow 0.
$$

#### Hệ quả 1 {#alg-x-s9-prop-4-cor-1 .statement}

*Để có $H_p(x,C)=0$, điều kiện cần và đủ là phép vị tự tỉ số $x$ trong $H_p(C)$ là toàn ánh và phép vị tự tỉ số $x$ trong $H_{p-1}(C)$ là đơn ánh.*

#### Hệ quả 2 {#alg-x-s9-prop-4-cor-2 .statement}

*Cho $x=(x_1,\ldots,x_n)$ là một dãy các phần tử của $A$, $M$ là một $A$-môđun, $x'$ là dãy $(x_1,\ldots,x_{n-1})$. Ta có các dãy khớp*

$$
0\longrightarrow A/x_nA\otimes_A H_p(x',M)\longrightarrow H_p(x,M)\longrightarrow \operatorname{Hom}_A(A/x_nA,H_{p-1}(x',M))\longrightarrow 0.
$$

#### Hệ quả 3 {#alg-x-s9-prop-4-cor-3 .statement}

*Để $H_i(x,M)$ bằng không với mọi $i>0$, điều kiện cần và đủ là phép vị tự tỉ số $x_n$ trong $H_i(x',M)$ là song ánh với $i>0$, và phép vị tự tỉ số $x_n$ trong $M/(x')M$ là đơn ánh.*

### 6. Các họ hoàn toàn cắt ngang

Cho $A$ là một vành, $M$ là một $A$-môđun, $x=(x_i)_{i\in I}$ là một họ các phần tử của $A$.

#### Định nghĩa 2 {#alg-x-s9-def-2 .statement}

*Họ $x$ được gọi là hoàn toàn cắt ngang đối với $M$ nếu ta có $H_i(x,M)=0$ với $i>0$.*

Nếu $I$ là hữu hạn, thì điều đó tương đương (X, p. 150) với việc có $H^i(x,M)=0$ với $i<\operatorname{Card}(I)$.

Mệnh đề sau cho phép đưa ra các ví dụ về các họ hoàn toàn cắt ngang.

#### Mệnh đề 5 {#alg-x-s9-prop-5 .statement}

*Cho $x=(x_1,\ldots,x_n)$ là một dãy các phần tử của $A$. Nếu với $i=1,\ldots,n$, phép vị tự tỉ số $x_i$ trong $A$-môđun $M/(x_1M+\cdots+x_{i-1}M)$ là đơn ánh, thì dãy $x$ là hoàn toàn cắt đối với $M$.*

Một dãy thỏa mãn các điều kiện của mệnh đề được gọi là chính quy đối với M, hay M-chính quy. Ta sẽ chú ý rằng tính chất này nói chung phụ thuộc vào thứ tự của các $x_i$; chẳng hạn dãy $(1, 0)$ luôn luôn là M-chính quy, trong khi dãy $(0, 1)$ chỉ như vậy nếu M là không. Mặt khác, việc một dãy là hoàn toàn cắt không phụ thuộc vào thứ tự của các số hạng.

Ta hãy chứng minh mệnh đề bằng quy nạp theo $n$, trường hợp $n = 0$ là ngay lập tức. Đặt $x' = (x_1, ..., x_{n-1})$; nếu dãy $x$ là M-chính quy, thì dãy $x'$ là M-chính quy và phép nhân bởi $x_n$ trong $M/(x')M$ là đơn ánh; theo giả thiết quy nạp, ta có $H_i(x', M) = 0$ với $i > 0$; khi đó suy ra từ hệ quả 3 của X, p. 157, rằng $H_i(x, M) = 0$ với $i > 0$.

#### Ví dụ {#alg-x-s9-n6-exa-1 .statement}

Cho $k$ là một vành; lấy $A = k[X_1, ..., X_n]$ và $x = (X_1, ..., X_n)$. Dãy $x$ là A-chính quy và mệnh đề lại cho tính không chu trình ở các bậc $> 0$ của phức $S_k(k^n) \otimes_k \Lambda_k(k^n)$ (xem X, p. 152, mệnh đề 3).
Tương tự, trong vành các chuỗi hình thức $\hat{A} = k[[X_1, ..., X_n]]$, dãy $(X_1, ..., X_n)$ là $\hat{A}$-chính quy, do đó hoàn toàn cắt đối với $\hat{A}$.

#### Mệnh đề 6 {#alg-x-s9-prop-6 .statement}

a) Nếu $\sum_{i \in I} x_i A = A$, họ $(x_i)_{i \in I}$ là hoàn toàn cắt đối với M.
b) Cho $x = (x_1, ..., x_n)$ là một dãy các phần tử của A. Cho $(a_{ij}) \in \mathrm{GL}_n(A)$; đặt
$$
y_i = \sum_j a_{ij} x_j.
$$
Nếu dãy $x$ là hoàn toàn cắt đối với M, thì dãy $(y_1, ..., y_n)$ cũng vậy.
c) Cho $k_1, ..., k_n$ là các số nguyên $\geqslant 1$; để dãy $(x_1^{k_1}, ..., x_n^{k_n})$ là hoàn toàn cắt đối với M, điều kiện cần và đủ là dãy $x$ là hoàn toàn cắt đối với M.
Mệnh đề a) suy ra từ hệ quả 1, p. 148.
Ta hãy chứng minh b). Cho $f : A^n \to A^n$ là đẳng cấu được xác định bởi ma trận $^t(a_{ij})$; suy ra từ X, p. 151, rằng $1_M \otimes \Lambda(f)$ là một đẳng cấu của phức $K.(y, M)$ lên phức $K.(x, M)$, do đó b).
Để chứng minh c), hiển nhiên chỉ cần chứng minh rằng nếu $k$ là một số nguyên $\geqslant 1$, thì dãy $(x_1, ..., x_{n-1}, x_n^k)$ là hoàn toàn cắt đối với M khi và chỉ khi dãy $x$ cũng có tính chất đó. Đặt $x' = (x_1, ..., x_{n-1})$; theo hệ quả 3, p. 157, điều kiện thứ nhất (tương ứng điều kiện thứ hai) có nghĩa là phép vị tự tỉ số $x_n^k$ (tương ứng $x_n$) là song ánh trong $H_i(x', M)$ với $i \geqslant 1$ và đơn ánh trong $M/(x')M$. Hai điều kiện này rõ ràng là tương đương, do đó c).

#### Nhận xét 1 {#alg-x-s9-n6-rem-1 .statement}

Mệnh đề tương tự như c) đối với các dãy chính quy là đúng (X, p. 207, bài tập 5).

#### Mệnh đề 7 {#alg-x-s9-prop-7 .statement}

a) Cho N là một A-môđun phẳng. Nếu họ x là hoàn toàn cắt đối với M, thì nó cũng vậy đối với $M \otimes_A N$.

b) Cho $0 \to M' \to M \to M'' \to 0$ là một dãy khớp các $A$-môđun. Nếu họ $x$ là hoàn toàn cắt ngang đối với $M'$ và đối với $M''$, thì nó cũng như vậy đối với $M$.

Phức $K.(x, M \otimes_A N)$ theo định nghĩa đẳng cấu với $K.(x, M) \otimes_A N$; vì $N$ phẳng, từ đó suy ra một đẳng cấu $H.(x, M) \otimes_A N \to H.(x, M \otimes_A N)$ (X, p. 66, hệ quả 2), do đó a).

Vì phức $K.(x)$ là phẳng, ta có một dãy khớp các phức

$$
0 \to K.(x, M') \to K.(x, M) \to K.(x, M'') \to 0 ;
$$

mệnh đề b) suy ra từ dãy đồng điều khớp liên kết.

#### Nhận xét 2 {#alg-x-s9-n6-rem-2 .statement}

Các mệnh đề tương tự với a) và b) đối với các dãy chính quy là ngay lập tức.

#### Nhận xét 3 {#alg-x-s9-n6-rem-3 .statement}

Nếu họ $x$ là hoàn toàn cắt ngang đối với $A$, phức $K.(x, A)$ xác định một phân giải tự do của $A$-môđun $A/x$, với $x = \sum_{i \in I} x_i A$; do đó với mọi số nguyên $i \geqslant 0$ và với mọi $A$-môđun $M$ có các đẳng cấu

$$
\text{Ext}_A^{n-i}(A/x, M) \to H^{n-i}(x, M) \to H_i(x, M) \to \operatorname{Tor}_i^A(A/x, M) .
$$

#### Nhận xét 4 {#alg-x-s9-n6-rem-4 .statement}

Ta nói rằng dãy $x = (x_1, ..., x_n)$ là $M$-đối chính quy nếu (ký hiệu bởi $(x_i)_M$ phép vị tự tỉ số $x_i$ trong $M$) phép vị tự tỉ số $x_i$ trong môđun

$$
\operatorname{Ker}(x_1)_M \cap ... \cap \operatorname{Ker}(x_{i-1})_M
$$

là toàn ánh với $i = 1, ..., n$. *Khi đó ta có* $H_i(x, M) = 0$ với $i < n$: điều này được chứng minh theo cùng cách như ở mệnh đề 5.

Lấy chẳng hạn $A = k[D_1, ..., D_n]$, trong đó $k$ là một $\mathbf{Q}$-đại số, và $M = k[T_1, ..., T_n]$, được trang bị cấu trúc môđun trên $A$ sao cho $D_i P = \partial P / \partial T_i$ với mọi $P \in M$ ($1 \leqslant i \leqslant n$). Ta kiểm tra ngay lập tức rằng dãy $(D_1, ..., D_n)$ là $M$-đối chính quy; có xét đến ví dụ p. 155, suy ra rằng *phức de Rham của* $k[T_1, ..., T_n]$ *trên* $k$ *là acyclic ở các bậc* $> 0$.

### 7. Một tiêu chuẩn cho các dãy hoàn toàn cắt ngang

Cho $A$ là một vành, $M$ một $A$-môđun, $x$ một iđêan của $A$. *Tôpô* *$x$-adic* trên $M$ được định nghĩa là tôpô tương thích với cấu trúc nhóm của $M$ mà trong đó tập hợp các môđun con $x^r M$ ($r \geqslant 0$) là một hệ cơ bản các lân cận của không (TG, III, p. 5, ví dụ). Tôpô này là tách biệt khi và chỉ khi

$$
\bigcap_{r \geqslant 0} x^r = 0 .
$$

Giả sử bây giờ iđêan $x$ được sinh bởi một dãy $x = (x_1, ..., x_n)$ các phần tử của A. Xét A-môđun phân bậc $\bigoplus_{r \geq 0} x^r M$ và A-đồng cấu phân bậc bậc 0

$$
a_M^x : A[X_1, ..., X_n] \otimes_A M \to \bigoplus_{r \geq 0} x^r M
$$

sao cho $a_M^x(P \otimes m) = P(x_1, ..., x_n) m$ nếu P là một đa thức thuần nhất theo $X_1, ..., X_n$ và $m \in M$. Gọi $\mathfrak{d}$ là iđêan của $A[X_1, ..., X_n]$ sinh bởi các phần tử $(x_i X_j - x_j X_i)$ với $1 \leq i < j \leq n$. Ta có $P(x_1, ..., x_n) = 0$ nếu $P \in \mathfrak{d}$, nên $a_M^x$ cho, bằng cách chuyển qua thương, một A-đồng cấu phân bậc bậc 0

$$
\alpha_M^x : (A[X_1, ..., X_n]/\mathfrak{d}) \otimes_A M \to \bigoplus_{r \geq 0} x^r M .
$$

Bằng tích tenxơ với $A/x$, từ $\alpha_M^x$ ta suy ra một A-đồng cấu phân bậc bậc 0

$$
\beta_M^x : (A/x)[X_1, ..., X_n] \otimes_A M \to \bigoplus_{r \geq 0} (x^r M/x^{r+1} M) .
$$

Các đồng cấu $a_M^x, \alpha_M^x$ và $\beta_M^x$ đều toàn ánh.

#### Định lý 1 {#alg-x-s9-thm-1 .statement}

Xét các điều kiện sau:
(i) Dãy $x$ là M-chính quy (X, p. 158).
(ii) Dãy $x$ hoàn toàn cát tuyến đối với M (X, p. 157, định nghĩa 2).
(iii) Ta có $H_1(x, M) = 0$.
(iv) Đồng cấu $\alpha_M^x : (A[X_1, ..., X_n]/\mathfrak{d}) \otimes_A M \to \bigoplus_{r \geq 0} x^r M$ là song ánh.
(v) Đồng cấu $\beta_M^x : (A/x)[X_1, ..., X_n] \otimes_A M \to \bigoplus_{r \geq 0} (x^r M/x^{r+1} M)$ là song ánh.

Khi đó ta có các kéo theo (i) $\Rightarrow$ (ii) $\Rightarrow$ (iii) $\Leftrightarrow$ (iv) $\Rightarrow$ (v). Nếu với $1 \leq i \leq n$, A-môđun $M/(x_1 M + \cdots + x_{i-1} M)$ là tách đối với tôpô $x$-adic, thì các điều kiện từ (i) đến (v) là tương đương.

Định lý sẽ được chứng minh trong các No 8 và 9.

*HỆ QUẢ 1. — Nếu A là Noether, nếu A-môđun M là kiểu hữu hạn và nếu các $x_i$ thuộc căn của A, thì các điều kiện từ (i) đến (v) của định lý là tương đương.
Thật vậy, trên mỗi môđun $M/(x_1 M + \cdots + x_{i-1} M)$ tôpô $x$-adic là tách (AC III, § 3, No. 3, mệnh đề 6).

#### Hệ quả 2 {#alg-x-s9-thm-1-cor-2 .statement}

Giả sử A là một vành phân bậc với các bậc dương, M là một A-môđun phân bậc bị chặn dưới, và các $x_i$ là những phần tử thuần nhất bậc > 0 của A. Khi đó các điều kiện từ (i) đến (v) của định lý là tương đương.
Thật vậy, tôpô $x$-adic là tách đối với mọi A-môđun phân bậc N bị chặn dưới, vì nếu $N_n = 0$ với $n < n_0$ thì ta có $x^a N \subset \sum_{j \geq n_0 + a} N_j$ với mọi $a \geq 0$.

#### Hệ quả 3 {#alg-x-s9-thm-1-cor-3 .statement}

Giả sử các môđun $M/(x_1M+\cdots+x_{i-1}M)$ là tách đối với tôpô $\mathfrak{x}$-adic $(1\leq i\leq n)$ ; gọi p là một số nguyên nằm giữa $1$ và $n$. Để dãy $\mathfrak{x}$ hoàn toàn cát tuyến đối với $M$, điều kiện cần và đủ là dãy $(x_1,\ldots,x_p)$ hoàn toàn cát tuyến đối với $M$ và dãy $(x_{p+1},\ldots,x_n)$ hoàn toàn cát tuyến đối với $M/(x_1M+\cdots+x_pM)$.

Thật vậy hệ quả là hiển nhiên nếu trong phát biểu người ta thay “các dãy hoàn toàn cát tuyến” bằng “các dãy chính quy”; nhưng ở đây hai khái niệm này trùng nhau theo định lý.

#### Nhận xét {#alg-x-s9-n7-rem-1 .statement}

Cho $\mathfrak{x}=(x_1,\ldots,x_n)$ là một dãy các phần tử của $A$ sao cho $H_1(\mathfrak{x},A)=0$; khi đó hạt nhân của đồng cấu toàn ánh $u:A^n\to\mathfrak{x}$ sao cho
$$
u\left(\sum a_i e_i\right)=\sum a_i x_i
$$
được sinh bởi các phần tử $X_j e_i-X_i e_j$; do đó, $A$-đại số $A[X_1,\ldots,X_n]/\mathfrak{d}$ đẳng cấu với đại số đối xứng $S_A(\mathfrak{x})$ (III, p. 69, mệnh đề 4). Vì thế từ Định lý 1 suy ra rằng đồng cấu đại số
$$
S_A(\mathfrak{x})\longrightarrow\bigoplus_n \mathfrak{x}^n
$$
cảm sinh bởi đơn ánh chính tắc của $\mathfrak{x}$ vào $\bigoplus_n\mathfrak{x}^n$ là một đẳng cấu. Điều tương tự cũng đúng cho đồng cấu
$$
S_A(\mathfrak{x}/\mathfrak{x}^2)\longrightarrow\bigoplus_n\mathfrak{x}^n/\mathfrak{x}^{n+1}.
$$

### 8. Chứng minh Định lý 1: phần đầu

Hệ quả (i) $\Rightarrow$ (ii) đã được chứng minh (X, p. 157, mệnh đề 5). Hệ quả (ii) $\Rightarrow$ (iii) là hiển nhiên; điều tương tự cũng đúng cho (iv) $\Rightarrow$ (v), vì $\beta_M^x$ được đồng nhất với $\alpha_M^x\otimes 1_{A/\mathfrak{x}}$.

Để chứng minh rằng (iv) suy ra (iii), xét đồng cấu $(\alpha_M^x)_1$ cảm sinh trên các thành phần bậc 1. Gọi $E$ là A-môđun phân bậc $A[X_1,\ldots,X_n]$; A-môđun $E_1$ là tự do với cơ sở $X_1,\ldots,X_n$ và $\mathfrak{d}_1$ là A-môđun con của $E_1$ sinh bởi các phần tử $(x_iX_j-x_jX_i)$ với $1\leq i<j\leq n$. Do đó $((E/\mathfrak{d})\otimes_A M)_1$ được đồng nhất với $K_1(\mathfrak{x},M)/B_1(K_\bullet(\mathfrak{x},M))$, đồng cấu $(\alpha_M^x)_1$ được đồng nhất với ánh xạ từ $K_1(\mathfrak{x},M)/B_1(K_\bullet(\mathfrak{x},M))$ vào $B_0(K_\bullet(\mathfrak{x},M))$ cảm sinh bởi $d_1$. Như vậy việc triệt tiêu của $H_1(\mathfrak{x},M)$ tương đương với tính đơn ánh của $(\alpha_M^x)_1$, do đó suy ra (iv) $\Rightarrow$ (iii).

Để chứng minh rằng (iii) suy ra (iv), ta sẽ dùng bổ đề sau:

#### Bổ đề 4 {#alg-x-s9-lem-4 .statement}

Cho $A_0$ là vành $\mathbf{Z}[T_1,\ldots,T_n]$, và cho $u:A_0[X_1,\ldots,X_n]\to A_0[U]$ là đồng cấu của các $A_0$-đại số sao cho $u(X_i)=T_iU$. Hạt nhân của $u$ là iđêan $\mathfrak{d}_0$ của $A_0[X_1,\ldots,X_n]$ sinh bởi các phần tử $(T_iX_j-T_jX_i)$ với $1\leq i<j\leq n$. Nếu $t$ là iđêan của $A_0$ sinh bởi $(T_1,\ldots,T_n)$, thì $u$ cảm sinh một đẳng cấu
$$
\bar{u}:A_0[X_1,\ldots,X_n]/\mathfrak{d}_0\longrightarrow\bigoplus_{r\geq0}t^r.
$$

Hiển nhiên chỉ cần chứng minh mệnh đề thứ nhất. Với mọi dãy số nguyên tự nhiên $\alpha=(\alpha_1,\ldots,\alpha_n)$ và mọi số nguyên $k\in[0,n]$, ký hiệu $P_{\alpha,k}$ là đơn thức
$$
T_1^{\alpha_1}\cdots T_k^{\alpha_k}X_{k+1}^{\alpha_{k+1}}\cdots X_n^{\alpha_n};
$$

gọi $N$ là môđun con trên $\mathbf{Z}$ của $A_0[X_1, ..., X_n]$ sinh bởi các $P_{\alpha, k}$ với $\alpha \in \mathbf{N}^n$ và $0 \leq k \leq n$. Ta sẽ chứng minh rằng hạn chế của $u$ trên $N$ là đơn ánh và $A_0[X_1, ..., X_n] = \mathfrak{d}_0 + N$; vì ta có $\mathfrak{d}_0 \subset \mathrm{Ker}\,u$, điều này sẽ kéo theo bổ đề.

Hãy nhận xét rằng $N$ được sinh bởi tập hợp $S$ gồm $P_{0,0} = 1$ và những $P_{\alpha, k}$ mà với chúng $\alpha_k \neq 0$. Để chứng minh tính đơn ánh của hạn chế của $u$ trên $N$, chỉ cần chỉ ra rằng hai phần tử phân biệt của $S$ có ảnh bởi $u$ là các đơn thức phân biệt trong $A_0[U]$. Bây giờ ta có $u(P_{\alpha, k}) = T^\alpha U^{\sum \alpha_i}_{i \geq k}$, nên đẳng thức $u(P_{\alpha, k}) = u(P_{\alpha', k'})$ kéo theo $\alpha = \alpha'$ và $\sum_{i \geq k} \alpha_i = \sum_{i \geq k'} \alpha_i$. Giả sử rằng $P_{\alpha, k}$ và $P_{\alpha', k'}$ thuộc $S$. Nếu $\alpha = 0$, thì ta có $k = k' = 0$; nếu $\alpha \neq 0$, ta thu được $k = k'$ vì $\alpha_k$ và $\alpha_{k'}$ khác không, do đó có kết quả.

Chứng minh rằng mọi đơn thức $T^\alpha X^\beta \in A_0[X_1, ..., X_n]$ đều đồng dư môđun $\mathfrak{d}_0$ với một $P_{\eta, k}$. Với mọi dãy $\lambda \in \mathbf{N}^n$, ta sẽ ký hiệu bởi $i(\lambda)$ (tương ứng $j(\lambda)$) số nguyên nhỏ nhất (tương ứng lớn nhất) $k \in [1, n]$ sao cho $\lambda_k \neq 0$. Trong các đơn thức $T^\gamma X^\delta$ đồng dư với $T^\alpha X^\beta$ môđun $\mathfrak{d}_0$, chọn một đơn thức sao cho số nguyên hữu tỉ $j(\gamma) - i(\delta)$ là cực tiểu; ta sẽ chứng minh rằng khi đó ta có $j(\gamma) - i(\delta) < 0$. Giả sử rằng $j(\gamma) \geq i(\delta)$; đặt $j = j(\gamma), i = i(\delta)$, và $\varepsilon = \inf (\gamma_j, \delta_i)$. Vì $(T_j^\varepsilon X_i^\varepsilon - T_i^\varepsilon X_j^\varepsilon)$ chia được cho $(T_j X_i - T_i X_j)$, và do đó thuộc $\mathfrak{d}_0$, nên ta thấy rằng $T^\gamma X^\delta$ đồng dư môđun $\mathfrak{d}_0$ với $T^{\gamma'} X^{\delta'}$, trong đó $\gamma'_i = \gamma_i + \varepsilon, \gamma'_j = \gamma_j - \varepsilon, \gamma'_k = \gamma_k$ với $k \neq i, j$, và $\delta'_i = \delta_i - \varepsilon, \delta'_j = \delta_j + \varepsilon, \delta'_k = \delta_k$ với $k \neq i, j$. Vì $\gamma'_j$ hoặc $\delta'_i$ bằng không, nên ta có $j(\gamma') - i(\delta') < j(\gamma) - i(\delta)$, điều này mâu thuẫn với đặc trưng cực tiểu của $j(\gamma) - i(\delta)$.

Do đó ta có $j(\gamma) < i(\delta)$, suy ra $T^\gamma X^\delta \in N$, điều này hoàn tất chứng minh của bổ đề.

Ta hãy chứng minh rằng (iii) kéo theo (iv). Xét vành $A_0 = \mathbf{Z}[T_1, ..., T_n]$ và iđêan t của $A_0$ sinh bởi $T_1, ..., T_n$. Trang bị cho $M$ cấu trúc A_0-môđun sao cho $T_i m = x_i m$ với $m \in M, 1 \leq i \leq n$. Theo X, p. 155, $H_i(x, M)$ được đồng nhất một cách chính tắc với $H_i(T, M)$.

Vì dãy $T$ là chính quy đối với $A_0$, nên từ phép kéo theo (i) $\Rightarrow$ (ii) suy ra rằng phức $K.(T, A_0)$ xác định một phân giải tự do của $A_0$-môđun $A_0/t$. Ta nhận xét rằng môđun sau được đồng nhất với $\mathbf{Z}$, được trang bị cấu trúc $A_0$-môđun sao cho $T_i \mathbf{Z} = 0$ với $1 \leq i \leq n$. Như vậy điều kiện (iii) tương đương với $\mathrm{Tor}_1^{A_0}(M, \mathbf{Z}) = 0$.

Ta sẽ chứng minh rằng (iii) kéo theo $\mathrm{Tor}_1^{A_0}(M, A_0/t^r) = 0$ với mọi $r \geq 1$. Điều này thu được từ điều đi trước đối với $r = 1$. Trong trường hợp tổng quát, xét dãy khớp

$$
0 \to t^r/t^{r+1} \to A_0/t^{r+1} \to A_0/t^r \to 0,
$$

A-môđun $t^r/t^{r+1}$ đẳng cấu với một tích hữu hạn của các bản sao của $\mathbf{Z}$; do đó ta có $\mathrm{Tor}_1^{A_0}(M, t^r/t^{r+1}) = 0$. Suy ra, bằng quy nạp theo $r$, rằng

$$
\mathrm{Tor}_1^{A_0}(M, A_0/t^r) = 0 \quad \text{với mọi } r,
$$

Dãy khớp (16) do đó, sau khi lấy tích tenxơ với $M$, cho một dãy khớp

$$
0 \to (t^r/t^{r+1}) \otimes_{A_0} M \to M/x^{r+1} M \to M/x^r M \to 0
$$

từ đó suy ra một đẳng cấu của $(t'/{t'}^{r+1}) \otimes_{A_0} M$ lên $x' M/{x'}^{r+1} M$. Khi xét dãy khớp $0 \to {t'}^{r+1} \to t' \to t'/{t'}^{r+1} \to 0$, khi đó lại thấy, bằng quy nạp theo $r$, rằng ánh xạ $m_r : t' \otimes_{A_0} M \to x' M$, cảm sinh bởi phép toán của $A_0$ trong $M$, là một đẳng cấu.

Để chứng minh (iv), còn phải nhận thấy rằng biểu đồ

$$
\begin{array}{ccc}
(A_0[X_1, ..., X_n]/\mathcal{D}_0) \otimes_{A_0} M & \xrightarrow{\bar{u} \otimes 1_M} & \bigoplus_{r \geq 0} (t' \otimes_{A_0} M) \\
\downarrow e & & \downarrow \oplus m_r \\
(A[X_1, ..., X_n]/\mathcal{D}) \otimes_A M & \xrightarrow{\alpha_M^x} & \bigoplus_{r \geq 0} x' M
\end{array}
$$

trong đó $e$ là đẳng cấu chính tắc của mở rộng vô hướng (II, p. 85, mệnh đề 6), là giao hoán, và áp dụng Bổ đề 4.

### 9. Chứng minh Định lý 1: phần thứ hai

Ta আবার xét dãy khớp

(16)
$$
0 \longrightarrow t'/{t'}^{r+1} \xrightarrow{i_r} A_0/{t'}^{r+1} \xrightarrow{p_r} A_0/t' \longrightarrow 0
$$

và dãy khớp liên kết của các môđun xoắn

(18)
$$
\begin{array}{cccccc}
\mathrm{Tor}_1^{A_0}(A_0/{t'}^{r+1}, M) & \longrightarrow & \mathrm{Tor}_1^{A_0}(A_0/t', M) \\
\longrightarrow (t'/{t'}^{r+1}) \otimes_{A_0} M & \xrightarrow{i_r \otimes 1_M} & (A_0/{t'}^{r+1}) \otimes_{A_0} M & \xrightarrow{p_r \otimes 1_M} & (A_0/t') \otimes_{A_0} M & \longrightarrow 0 .
\end{array}
$$

Hạt nhân của $p_r \otimes 1_M$ được đồng nhất với $x' M/{x'}^{r+1} M$; hơn nữa $t'/{t'}^{r+1}$ bị triệt tiêu bởi các $T_i$ và được đồng nhất với thành phần thuần nhất bậc $r$ của $A_0$, sao cho đồng cấu $(t'/{t'}^{r+1}) \otimes_{A_0} M \to x' M/{x'}^{r+1} M$ suy ra từ $i_r \otimes 1_M$ được đồng nhất với thành phần thuần nhất bậc $r$ của đồng cấu $\beta_M^x$. Do đó suy ra từ dãy khớp (18) rằng điều kiện (v) tương đương với

(v') : *đồng cấu* $\mathrm{Tor}_1^{A_0}(p_r, 1_M)$ : $\mathrm{Tor}_1^{A_0}(A_0/{t'}^{r+1}, M) \to \mathrm{Tor}_1^{A_0}(A_0/t', M)$ *là toàn ánh với mọi* $r \geq 1$.

Còn lại ta phải chứng minh kéo theo (v) $\Rightarrow$ (i) khi các môđun
$$
M/(x_1 M + \cdots + x_{i-1} M)
$$
là tách biệt đối với tôpô $x$-adic ($1 \leq i \leq n$). Ký hiệu $\overline{M}$ là A-môđun $M/x_1 M$. Theo định nghĩa, dãy $x$ là chính quy đối với $M$ nếu và chỉ nếu $(x_1)_M$ là đơn ánh và dãy $x' = (x_2, ..., x_n)$ là chính quy đối với $\overline{M}$. Lập luận bằng quy nạp theo $n$, do đó chỉ cần chứng minh rằng, nếu $M$ tách biệt đối với tôpô $x$-adic và nếu $\beta_M^x$ là song ánh, thì $(x_1)_M$ là đơn ánh và $\beta_M^{x'}$ là song ánh. Bây giờ tính song ánh của $\beta_M^x$ đặc biệt hàm ý rằng phép vị tự với tỷ số $x_1$ trong $\bigoplus r x' M/{x'}^{r+1} M$ là đơn ánh, bởi thế $\mathrm{Ker}\,(x_1)_M \subset \bigcap_i x^i M$ và do đó $(x_1)_M$ là đơn ánh nếu tôpô $x$-adic trên $M$ là tách biệt.

Như vậy ta được quy về việc chứng minh rằng nếu $(x_1)_M$ là đơn ánh và nếu $M$ thỏa mãn điều kiện (v'), thì $\overline{M}$ thỏa mãn điều kiện (v') đối với dãy $x'$.

Theo giả thiết, ta có một dãy khớp
$$
0 \longrightarrow M \xrightarrow{(x_1)_M} M \longrightarrow \overline{M} \longrightarrow 0;
$$
đặt $\overline{A}_0 = A_0 / T_1 A_0,\ \overline{t} = t \overline{A}_0$. Gọi $q : L \to M$ là một phân giải tự do của $A_0$-môđun $M$; vì phép vị tự với tỷ số $T_1$ là đơn ánh trong $A_0$, nên nó là đơn ánh trong $L$, và ta có một dãy khớp các phức
$$
0 \longrightarrow L \xrightarrow{(x_1)_L} L \longrightarrow \overline{L} \longrightarrow 0
$$
với $\overline{L} = L / x_1 L$, và một biểu đồ giao hoán
$$
\begin{array}{ccc}
0 & \longrightarrow & L \xrightarrow{(x_1)_L} L \longrightarrow \overline{L} \longrightarrow 0 \\
   &                & \downarrow q        \downarrow q        \downarrow \overline{q} \\
0 & \longrightarrow & M \xrightarrow{(x_1)_M} M \longrightarrow \overline{M} \longrightarrow 0 .
\end{array}
$$

Vì $q$ là một đồng cấu các phức cảm sinh các đẳng cấu trong đồng điều, nên $\overline{q} : \overline{L} \to \overline{M}$ là một phân giải tự do của $\overline{A}_0$-môđun $\overline{M}$ (hệ quả 1, p. 30). Với mọi $\overline{A}_0$-môđun $P$, có một đẳng cấu chính tắc
$$
P \otimes_{A_0} L \to P \otimes_{\overline{A}_0} \overline{L},
$$
do đó khi chuyển qua đồng điều ta được một đẳng cấu
$$
\varphi_P : \mathrm{Tor}_1^{A_0}(P, M) \to \mathrm{Tor}_1^{\overline{A}_0}(P, \overline{M}) .
$$
Nếu $u : P \to P'$ là một $\overline{A}$-đồng cấu, thì
$$
\varphi_{P'} \circ \mathrm{Tor}_1^{A_0}(u, 1_M) = \mathrm{Tor}_1^{\overline{A}_0}(u, 1_M) \circ \varphi_P .
$$
Do đó, giả sử rằng điều kiện (v') được thỏa mãn đối với $M$, và hãy chứng minh rằng nó đúng với $\overline{M}$. Gọi $r$ là một số nguyên $\geqslant 1$; ta có một biểu đồ giao hoán với các hàng khớp
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & A_0 / t^r & \xrightarrow{T_1} & A_0 / t^{r+1} & \longrightarrow & \overline{A}_0 / \overline{t}^{r+1} & \longrightarrow & 0 \\
   &                  & \downarrow p_{r-1} &           & \downarrow p_r &           & \downarrow \overline{p}_r &           & \\
0 & \longrightarrow & A_0 / t^{r-1} & \xrightarrow{T_1} & A_0 / t^r & \longrightarrow & \overline{A}_0 / \overline{t}^r & \longrightarrow & 0
\end{array}
$$
từ đó suy ra một biểu đồ giao hoán với các hàng khớp
$$
\begin{array}{ccccccccccc}
\mathrm{Tor}_1^{A_0}(A_0 / t^{r+1}, M) & \longrightarrow & \mathrm{Tor}_1^{A_0}(\overline{A}_0 / \overline{t}^{r+1}, M) & \longrightarrow & M / x^r M & \xrightarrow{x_1} & M / x^{r+1} M \\
\mathrm{Tor}_1(p_{r, r'}) & \downarrow & \mathrm{Tor}_1(\overline{p}_{r, 1}) & \downarrow & & & \downarrow \\
\mathrm{Tor}_1(A_0 / t^r, M) & \longrightarrow & \mathrm{Tor}_1^{A_0}(\overline{A}_0 / \overline{t}^r, M) & \longrightarrow & M / x^{r-1} M & \xrightarrow{x_1} & M / x^r M .
\end{array}
$$
Bây giờ phép nhân với $x_1$ xác định một đơn ánh từ $M / x^r M$ vào $M / x^{r+1} M$: điều này suy ra ngay lập tức, bằng quy nạp theo $r$, từ dãy khớp
$$
0 \to x^{r-1} M / x^r M \to M / x^r M \to M / x^{r-1} M \to 0
$$

và từ tính đơn ánh của phép vị tự với tỷ số $x_1$ trong $\bigoplus_{r \geq 0} (x^r M / x^{r+1} M)$. Vì thế điều kiện (v) kéo theo rằng đồng cấu $\operatorname{Tor}_{1}^{\overline{A}_0} (\overline{p}_r, 1_M)$ là toàn ánh với mọi $r \geq 1$. Hợp thành với các đẳng cấu $(\varphi_{\overline{A}_0/\overline{t}^{r+1}})^{-1}$ và $\varphi_{\overline{A}_0/\overline{t}^r}$, ta suy ra rằng đồng cấu

$$
\operatorname{Tor}_{1}^{\overline{A}_0} (\overline{p}_r, 1_M) : \operatorname{Tor}_{1}^{\overline{A}_0} (\overline{A}_0 / \overline{t}^{r+1}, M) \to \operatorname{Tor}_{1}^{\overline{A}_0} (\overline{A}_0 / \overline{t}^r, M)
$$

là toàn ánh với $r \geq 1$, do đó có điều kiện (v') đối với $\overline{M}$. Điều này hoàn tất chứng minh định lý.

### 10. Lớp các mở rộng liên kết với một dãy chính quy

Cho $A$ là một vành, $M$ là một $A$-môđun, $x = (x_1, ..., x_n)$ là một dãy các phần tử của $A$. Ký hiệu $M_i$ là $A$-môđun $M / (x_1 M + \cdots + x_{i-1} M)$ với $i = 0, ..., n+1$, sao cho $M_0$ và $M_1$ được đồng nhất với $M$ và $M_{n+1} = M / (x) M$. Đặt

$$
\overline{x}_i : M_{i-1} \to M_i , \quad i = 1, ..., n ,
$$

đồng cấu $A$ hợp thành bởi phép vị tự của $M_{i-1}$ với tỷ số $x_i$ và phép chiếu chính tắc của $M_{i-1}$ lên $M_i$. Cuối cùng, ký hiệu bởi $p : M_n \to M / (x) M$ phép chiếu chính tắc. Biểu đồ

(19)

$$
0 \longrightarrow M \xrightarrow{\overline{x}_1} M_1 \xrightarrow{\overline{x}_2} M_2 \longrightarrow \cdots \xrightarrow{\overline{x}_n} M_n \xrightarrow{p} M / (x) M \longrightarrow 0
$$

là một dãy khớp khi và chỉ khi dãy $x$ là $M$-chính quy. Từ đây trở đi giả sử rằng dãy $x$ là chính quy đối với $M$. Phần tử $\theta_x \in \operatorname{Ext}_A^n (M / (x) M, M)$ liên kết với dãy khớp (19) cũng được nói là liên kết với dãy $M$-chính quy $x$.

Cho $i$ là một số nguyên, $1 \leq i \leq n$. Chú ý rằng dãy (19) có thể được phân tích thành hai dãy khớp

(20)

$$
0 \longrightarrow M \xrightarrow{\overline{x}_1} M_1 \xrightarrow{\overline{x}_2} M_2 \longrightarrow \cdots \xrightarrow{\overline{x}_i} M_i \longrightarrow M / (x_1 M + \cdots + x_i M) \longrightarrow 0
$$

(21)

$$
0 \longrightarrow M / (x_1 M + \cdots + x_i M) \xrightarrow{\overline{x}_{i+1}} M_{i+1} \longrightarrow \cdots \longrightarrow M_n \xrightarrow{p} M / (x) M \longrightarrow 0
$$

mà không là gì khác ngoài các dãy khớp liên kết với dãy $(x_1, ..., x_i)$, là chính quy đối với $M$, và với dãy $(x_{i+1}, ..., x_n)$, là chính quy đối với $M / (x_1 M + \cdots + x_i M)$. Ký hiệu bởi

$$
\theta_{(x_1, ..., x_i)} \in \operatorname{Ext}_A^i (M / (x_1 M + \cdots + x_i M), M)
$$
$$
\theta_{(x_{i+1}, ..., x_n)} \in \operatorname{Ext}_A^{n-i} (M / (x) M, M / (x_1 M + \cdots + x_i M)) ,
$$

các lớp mở rộng liên kết với (20) và (21), ta có, theo X, p. 118, mệnh đề 3,

(22)
$$
\theta_{(x_1, \ldots, x_n)} = \theta_{(x_1, \ldots, x_i)} \circ \theta_{(x_{i+1}, \ldots, x_n)} .
$$

Hơn nữa, theo mệnh đề 5 (X, p. 157), phức Koszul $\mathbf{K}.(x, M)$ là phi chu trình ở các bậc $\neq n$, do đó có một dãy khớp

(23)
$$
0 \longrightarrow M \xrightarrow{\partial^0} \mathbf{K}^1(x, M) \xrightarrow{\partial^1} \mathbf{K}^2(x, M) \xrightarrow{\partial^2} \cdots \longrightarrow \mathbf{K}^n(x, M) \xrightarrow{q} M/(x)M \longrightarrow 0 ,
$$
trong đó $\mathbf{K}^0(x, M)$ đã được đồng nhất với $M$ và trong đó $q$ ánh xạ mỗi phần tử $m \in \mathbf{K}^n(x, M)$ vào lớp trong $M/(x)M$ của $m(1, 2, \ldots, n) \in M$.

#### Mệnh đề 8 {#alg-x-s9-prop-8 .statement}

*Giả sử dãy x là chính quy đối với M. Phần tử của $\mathrm{Ext}_A^n(M/(x)M, M)$ liên kết với dãy khớp (23) là $(-1)^{n(n+1)/2} \theta_x$.*
Với $i = 0, 1, \ldots, n$, định nghĩa một ánh xạ A-tuyến tính
$$
a^i : \mathbf{K}^i(x, M) \to M_i = M/(x_1 M + \cdots + x_{i-1} M)
$$
như sau: nếu $m \in \mathbf{K}^i(x, M)$, thì $a^i(m)$ là lớp trong $M_i$ của phần tử $m(1, 2, \ldots, i)$ của $M$. Hiển nhiên $a^0$ là ánh xạ đồng nhất của $M$ và $p \circ a^n = q$. Hơn nữa $a^{i+1} \circ \partial^i(m)$ là ảnh trong $M_{i+1}$ của phần tử
$$
\sum_{k=1}^{i+1} (-1)^{k+1} x_k m(1, 2, \ldots, k-1, k+1, \ldots, i+1) .
$$
Vì $x_k$ triệt tiêu $M_{i+1}$ với $k = 1, \ldots, i$, nên $a^{i+1} \circ \partial^i(m)$ cũng là ảnh của
$$
(-1)^i x_{i+1} m(1, 2, \ldots, i) ,
$$
do đó
$$
a^{i+1} \circ \partial^i = (-1)^i \overline{x}_{i+1} \circ a^i .
$$
Theo X, p. 120, hệ quả 1 và 2, phần tử của $\mathrm{Ext}_A^n(M/(x)M, M)$ liên kết với (23) bằng $\prod_{i=1}^n (-1)^i \cdot \theta_x$, do đó có mệnh đề.

#### Hệ quả {#alg-x-s9-n10-cor-1 .statement}

*Giả sử hơn nữa rằng các môđun $M/(x_1 M + \cdots + x_{i-1} M)$ là tách biệt đối với tôpô (x)-adic, và cho $(a_{ij}) \in \mathrm{GL}_n(A)$. Đặt*
$$
y_i = \sum_j a_{ij} x_j \quad \text{và} \quad y = (y_1, \ldots, y_n) .
$$
*Khi đó dãy y là chính quy đối với M, và ta có $\theta_y = \det(a_{ij})^{-1} \theta_x$.*
Thật vậy, dãy y là chính quy đối với M theo Mệnh đề 6 (X, p. 158) và Định lý 1 (X, p. 160); khẳng định cuối cùng suy ra từ Mệnh đề 8, và từ Mệnh đề 4 của X, p. 119.

#### Mệnh đề 9 {#alg-x-s9-prop-9 .statement}

*Giả sử dãy x là chính quy đối với M. Nếu N là một A-môđun sao cho $(x)N = 0$, thì ta có $\mathrm{Ext}_A^i(N, M) = 0$ với $i < n$, và ánh xạ $\alpha \mapsto \theta_x \circ \alpha$* từ Hom_A (N, M/(x) M) vào Ext^n_A (N, M) (nó cũng là đồng cấu nối lặp liên kết với (19), xem X, p. 127, Hệ quả 3) là song ánh.

Còn phải chứng minh rằng đồng cấu $\psi^i : \alpha \mapsto \theta_x \circ \alpha$ từ $\mathrm{Ext}_A^{i-n}(N, M/(x) M)$ vào $\mathrm{Ext}_A^i(N, M)$ là song ánh với $i \leq n$. Ta lập luận bằng quy nạp theo $n$, mệnh đề là tầm thường với $n = 0$. Đặt $M_1 = M/x_1 M$, $x' = (x_2, ..., x_n)$, khi đó $x'$ là chính quy đối với $M_1$. Theo giả thiết quy nạp, đồng cấu

$$
\overline{\psi}^{i-1} : \alpha \mapsto \theta_{x'} \circ \alpha
$$

từ $\mathrm{Ext}_A^{i-n}(N, M/(x) M)$ vào $\mathrm{Ext}_A^{i-1}(N, M_1)$ là song ánh với $i < n$. Mặt khác, xét dãy khớp

$$
0 \longrightarrow M \xrightarrow{(x_1)_M} M \longrightarrow M_1 \longrightarrow 0 ;
$$

đồng cấu nối $\mathrm{Ext}_A^i(N, M_1) \to \mathrm{Ext}_A^{i+1}(N, M)$ liên kết với nó là $\varphi^i : \beta \mapsto \theta_{x_1} \circ \beta$ (X, p. 125, Mệnh đề 5) ;

vì ta có $\mathrm{Ext}^i(1_N, (x_1)_M) = \mathrm{Ext}^i((x_1)_N, 1_M) = 0$, nên từ dãy khớp này suy ra

$$
0 \longrightarrow \mathrm{Ext}_A^i(N, M) \longrightarrow \mathrm{Ext}_A^i(N, M_1) \xrightarrow{\varphi^i} \mathrm{Ext}_A^{i+1}(N, M) \longrightarrow 0 .
$$

Vì $\mathrm{Ext}_A^i(N, M_1) = 0$ với $i < n - 1$, nên suy ra $\mathrm{Ext}_A^{i+1}(N, M) = 0$ với $i < n - 1$, nghĩa là với $i + 1 < n$; do đó $\varphi^i$ là song ánh với $i < n$. Vì $\psi^i(\alpha) = \theta_x \circ \alpha = \theta_{x_1} \circ \theta_{x'} \circ \alpha = \varphi^{i-1} \circ \overline{\psi}^i(\alpha)$ với $\alpha \in \mathrm{Ext}_A^{i-n}(N, M/(x) M)$, nên $\psi^i$ quả thật là song ánh với $i \leq n$.

BÀI TẬP

## BÀI TẬP {#alg-x-s9-exercises}

Xem [các bài tập của § 9](exercises/s9/).
