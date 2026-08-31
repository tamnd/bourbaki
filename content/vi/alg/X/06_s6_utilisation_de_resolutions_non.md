---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 6
section_title: Utilisation de résolutions non canoniques
lang: vi
source: alg-x-fr
book_pages: A X.100-A X.113, A X.189-A X.197
pdf_pages: 0106-0119, 0195-0203
extraction: ocr
subsections:
    - "no": 1
      title: Calcul des modules $\mathrm{Tor}^A(P, M)$ et $\mathrm{Ext}_A(M, N)$
      page: 100
      pdf_page: 106
    - "no": 2
      title: Calcul des applications $\mathrm{Tor}^A(g, f)$ et $\mathrm{Ext}_A(f, h)$
      page: 103
      pdf_page: 109
    - "no": 3
      title: Calcul des homomorphismes de liaison
      page: 104
      pdf_page: 110
    - "no": 4
      title: Finitude des modules d’extensions et de torsion
      page: 107
      pdf_page: 113
    - "no": 5
      title: Les homomorphismes $\operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to \operatorname{Tor}^{B}(P,N \otimes_{A} Q)$ et $\operatorname{Ext}_{B}(M,N) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q)$
      page: 108
      pdf_page: 114
    - "no": 6
      title: Les homomorphismes $\mathrm{Tor}^B(P, N \otimes_A Q) \to \mathrm{Tor}^A(P \otimes_B N, Q)$ et $\mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)) \to \mathrm{Ext}_B(N \otimes_A Q, M)$
      page: 109
      pdf_page: 115
    - "no": 7
      title: Les homomorphismes $B \otimes_A \mathrm{Tor}^A(E, F) \to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)$ et $B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F)$
      page: 110
      pdf_page: 116
    - "no": 8
      title: 'Application : homologie et cohomologie des groupes'
      page: 111
      pdf_page: 117
statements: 30
exercises: 18
content_sha256: 3ed9447f2ce6951e07cc25d42a19253c98384d756f11ba6d9d9697d2f7b8caca
translated_from: content/en-mt/alg/X/06_s6_utilisation_de_resolutions_non.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 0c26e4c195513eda20c41eed9f564bfc5605c3675b50f3a3af22c634208610bd
translation_model: gpt-5.4
translation_run: translate-vi-8e05e0c5
glossary_version: 34
glossary_terms_sha256: 6d7acf620f2c5062863d530760ccd18ecf15594d5efb01c9307eda3d9dfbbd7c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. SỬ DỤNG CÁC PHÂN GIẢI KHÔNG CHÍNH TẮC

Ta giữ lại các quy ước của § 4.

### 1. Tính các môđun $\mathrm{Tor}^A(P, M)$ và $\mathrm{Ext}_A(M, N)$

Cho $M, N$ là các $A$-môđun trái, $P$ là một $A$-môđun phải. Hơn nữa, cho $a : R \to M$ là một phân giải trái của $M$, $b : S \to P$ là một phân giải trái của $P$ và $c : N \to E$ là một phân giải phải của $N$.

Theo $X$, p. 49, mệnh đề 3 và 3 bis, tồn tại các cấu xạ phức $\alpha : L(M) \to R$, $\beta : L(P) \to S$, $\gamma : E \to I(N)$ sao cho $a \circ \alpha = p_M$, $b \circ \beta = p_P$, $\gamma \circ C = e_N$, và các lớp đồng luân của $\alpha, \beta, \gamma$ chỉ phụ thuộc vào các phân giải đã cho. Theo $X$, p. 64, mệnh đề 3 và $X$, p. 84, mệnh đề 3, các lớp đồng luân của các cấu xạ

$$
\beta \otimes \alpha : L(P) \otimes_A L(M) \to S \otimes_A R,
$$
$$
\mathrm{Homgr}_A(\alpha, \gamma) : \mathrm{Homgr}_A(R, E) \to \mathrm{Homgr}_A(L(M), I(N))
$$

chỉ phụ thuộc vào các phân giải đã cho, do đó khi chuyển qua đồng điều ta được các $k$-đồng cấu phân bậc bậc 0

$$
\psi(S, R) : \mathrm{Tor}^A(P, M) \to H(S \otimes_A R),
$$
$$
\varphi(R, E) : H(\mathrm{Homgr}_A(R, E)) \to \mathrm{Ext}_A(M, N),
$$

độc lập với lựa chọn của $\alpha, \beta, \gamma$.

Ví dụ, lấy đối với $a, b, c$ các ánh xạ đồng nhất của tương ứng $M, P, N$, ta thu được các đồng cấu $\psi(P, M) : \mathrm{Tor}^A(P, M) \to P \otimes_A M$ và $\varphi(M, N) : \mathrm{Hom}_A(M, N) \to \mathrm{Ext}_A(M, N)$ được đưa vào trong $X$, p. 68, nhận xét 2) và $X$, p. 87, nhận xét 2).

#### Định lý 1 {#alg-x-s6-thm-1 .statement}

a) Nếu một trong hai phân giải $R$ hoặc $S$ là phẳng, thì $\psi(S, R)$ là một đẳng cấu của các $k$-môđun phân bậc.

b) Nếu $R$ là xạ ảnh hoặc nếu $E$ là đơn ánh, thì $\varphi(R, E)$ là một đẳng cấu của các $k$-môđun phân bậc.

a) Chẳng hạn giả sử $\mathbf R$ phẳng, và chọn $\alpha$ và $\beta$ như trên. Đồng cấu $\beta\otimes\alpha$ là hợp thành của các cấu xạ

$$
L(P)\otimes_A L(M)\xrightarrow{1_{L(P)}\otimes\alpha}L(P)\otimes_A\mathbf R\xrightarrow{\beta\otimes1_{\mathbf R}}S\otimes_A\mathbf R.
$$

Vì $L(P)$ (tương ứng $\mathbf R$) là phẳng và $\alpha$ (tương ứng $\beta$) là một đồng cấu, nên $1_{L(P)}\otimes\alpha$ (tương ứng $\beta\otimes1_{\mathbf R}$) cũng là một đồng cấu, theo mệnh đề 4 của X, p. 67. Vậy $\beta\otimes\alpha$ là một đồng cấu và $\psi(S,R)=H(\beta\otimes\alpha)$ là song ánh.

b) Ta lập luận tương tự, dùng mệnh đề 4 của X, p. 86.

#### Hệ quả {#alg-x-s6-n1-cor-1 .statement}

Nếu $R$ là một phân giải phẳng của $M$, đồng cấu

$$
\psi(P,R):\operatorname{Tor}^A(P,M)\longrightarrow H(P\otimes_A R)
$$

là song ánh. Nếu $R$ là một phân giải xạ ảnh của $M$, đồng cấu

$$
\varphi(R,N):H(\operatorname{Homgr}_A(R,N))\longrightarrow \operatorname{Ext}_A(M,N)
$$

là song ánh. Nếu $E$ là một phân giải đơn ánh của $N$, thì đồng cấu

$$
\varphi(M,E):H(\operatorname{Homgr}_A(M,E))\longrightarrow \operatorname{Ext}_A(M,N)
$$

là song ánh.

#### Nhận xét {#alg-x-s6-n1-rem-1 .statement}

Biểu đồ các $k$-môđun

$$
\begin{array}{ccc}
\operatorname{Tor}^A(P,M)&\xrightarrow{\psi(S,R)}&H(S\otimes_A R)\\
\downarrow{\sigma_{P,M}}&&\downarrow{H(\sigma(S,R))}\\
\operatorname{Tor}^{A^\circ}(M^\circ,P^\circ)&\xrightarrow{\psi(R^\circ,S^\circ)}&H(R^\circ\otimes_{A^\circ}S^\circ),
\end{array}
$$

trong đó $\sigma_{P,M}$ và $\sigma(S,R)$ là các *đẳng cấu giao hoán* (X, p. 71 và 63), là giao hoán: thật vậy, nó thu được bằng cách chuyển qua đồng điều từ biểu đồ giao hoán các phức

$$
\begin{array}{ccc}
L(P)\otimes_A L(M)&\xrightarrow{\beta\otimes\alpha}&S\otimes_A R\\
\downarrow{\sigma(L(P),L(M))}&&\downarrow{\sigma(S,R)}\\
L(M^\circ)\otimes_{A^\circ}L(P^\circ)&\xrightarrow{\alpha\otimes\beta}&R^\circ\otimes_{A^\circ}S^\circ
\end{array}
$$

("các cấu xạ $\psi$ tương thích với các đẳng cấu giao hoán").

Tương tự, cho $a_1:R_1\to M$, $b_1:S_1\to P$, $c_1:N\to E_1$ là các cấu xạ của phức, trong đó $R_1$ và $S_1$ là xạ ảnh và phải không, còn $E_1$ là đơn ánh và trái không. Theo X, p. 49, mệnh đề 3 và 3 bis, tồn tại các cấu xạ của phức

$$
\alpha_1:R_1\to L(M),\qquad \beta_1:S_1\to L(P),\qquad \gamma_1:I(N)\to E_1
$$

sao cho $p_M \circ \alpha_1 = a_1, p_P \circ \beta_1 = b_1, \gamma_1 \circ e_N = c_1$, do đó có các cấu xạ của phức

$$
\beta_1 \otimes \alpha_1 : S_1 \otimes_A R_1 \to L(P) \otimes_A L(M),
$$

$$
\operatorname{Homgr}_A (\alpha_1, \gamma_1) : \operatorname{Homgr}_A (L(M), l(N)) \to \operatorname{Homgr}_A (R_1, E_1),
$$

và, bằng cách chuyển qua đồng điều, các *ánh xạ phân bậc k-tuyến tính bậc* 0:

$$
\psi'(S_1, R_1) : H(S_1 \otimes_A R_1) \to \operatorname{Tor}^A (P, M)
$$
$$
\varphi'(R_1, E_1) : \operatorname{Ext}_A (M, N) \to H(\operatorname{Homgr}_A (R_1, E_1))
$$

mà, như trên, ta kiểm tra được là độc lập với lựa chọn $\alpha_1, \beta_1, \gamma_1$.

#### Mệnh đề 1 {#alg-x-s6-prop-1 .statement}

*Nếu* $a_1, b_1, c_1$ *là các đồng cấu đồng điều,* $\psi'(S_1, R_1)$ *và* $\varphi'(R_1, E_1)$ *lần lượt là các song ánh nghịch đảo của các song ánh* $\psi(S_1, R_1)$ *và* $\varphi(R_1, E_1)$.

Thật vậy, $f = (\beta \otimes \alpha) \circ (\beta_1 \otimes \alpha_1)$ là một cấu xạ từ phức $S_1 \otimes_A R_1$ vào chính nó, và ta có $(h_1 \circ \alpha_1) \circ f = f$. Theo X, p. 49, mệnh đề 3 và 3 *bis*, $f$ là một đồng luân đẳng cấu, do đó $H(f) = 1$ và

$$
\psi(S_1, R_1) \circ \psi'(B_1, R_1) = H(\beta \otimes \alpha) \circ H(\beta_1 \otimes \alpha_1) = H(f) = 1;
$$

tương tự $\psi'(S_1, R_1) \circ \psi(S_1, R_1) = 1$. Ta lập luận tương tự cho các ánh xạ $\varphi$ và $\varphi'$.

#### Ví dụ 1 {#alg-x-s6-n1-exa-1 .statement}

Cho $a$ là một phần tử của $A$ sao cho ánh xạ $\varphi : x \mapsto xa$ từ $A$ vào chính nó là đơn ánh (*"* $a$ không là một ước của không phải *"*). Dùng phân giải

$$
0 \to A_s \xrightarrow{\varphi} A_s \to A/Aa \to 0
$$

ta thấy rằng với mọi $A$-môđun phải $M$, ta có

$$
\operatorname{Tor}_i^A (M, A/Aa) = 0 \quad \text{với } i > 1
$$

và $k$-môđun $\operatorname{Tor}_1^A (M, A/Aa)$ đẳng cấu với $\operatorname{Ker} (a_M)$.

Tương tự, với mọi $A$-môđun trái $M$, ta có

$$
\operatorname{Ext}_A^i (A/Aa, M) = 0 \quad \text{với } i > 1
$$

và $k$-môđun $\operatorname{Ext}_A^1 (A/Aa, M)$ đẳng cấu với $M/aM$.

#### Ví dụ 2 {#alg-x-s6-n1-exa-2 .statement}

Giả sử rằng $A$ là một miền nguyên; cho $K$ là trường phân thức của $A$ và $M$ là một $A$-môđun. Dùng phân giải phẳng

$$
0 \to A \to K \to K/A \to 0
$$

(X, p. 9, *ví dụ* 5), ta thấy rằng $\operatorname{Tor}_i^A (K/A, M) = 0$ với $i > 1$; hơn nữa, theo II, p. 116, prop. 26, (ii), $A$-môđun $\operatorname{Tor}_1^A (K, A, M)$ đẳng cấu với môđun con xoắn của $M$.

#### Ví dụ 3 {#alg-x-s6-n1-exa-3 .statement}

Giả sử rằng $A$ là một vành địa phương Noether, ký hiệu $m$ là iđêan cực đại của nó, và đặt $\kappa = A/m$. Cho $M$ là một $A$-môđun sinh hữu hạn và $P$ là một phân giải xạ ảnh cực tiểu của $M$ (X, p. 54). Với mọi $n \geqslant 0$, các không gian vectơ trên $\kappa$ $\mathrm{Tor}_n^A(\kappa, M)$ và $\mathrm{Ext}_A^n(M, \kappa)$ đều hữu hạn chiều, có chiều bằng hạng của $A$-môđun tự do $P_n$; thực vậy, các phức $\kappa \otimes_A P$ và $\mathrm{Homgr}_A(P, \kappa)$ có vi phân bằng không.

### 2. Tính các ánh xạ $\mathrm{Tor}^A(g, f)$ và $\mathrm{Ext}_A(f, h)$

Cho $f : M \to M', h : N' \to N$ là các đồng cấu của các $A$-môđun trái, $g : P \to P'$ là một đồng cấu của các $A$-môđun phải, $a : R \to M, a' : R' \to M'$, $b : S \to P, b' : S' \to P'$, tương ứng là các phân giải trái của $M, M', P, P'$, $c : N \to E, c' : N' \to E'$ là các phân giải phải của $N$ và $N'$, $\tilde{f} : R \to R', \tilde{g} : S \to S', \tilde{h} : E' \to E$ là các cấu xạ của các phức sao cho

$$
a' \circ \tilde{f} = f \circ a, \quad b' \circ \tilde{g} = g \circ b, \quad \tilde{h} \circ c' = c \circ h .
$$

#### Mệnh đề 2 {#alg-x-s6-prop-2 .statement}

*Hai biểu đồ sau là giao hoán*:

$$
\begin{array}{ccc}
\mathrm{Tor}^A(P, M) & \xrightarrow{\psi(S, R)} & \mathrm{H}(S \otimes_A R) \\
\mathrm{Tor}^A(g, f) \downarrow & & \downarrow \mathrm{H}(\tilde{g} \otimes \tilde{f}) \\
\mathrm{Tor}^A(P', M') & \xrightarrow{\psi(S', R')} & \mathrm{H}(S' \otimes_A R') ,
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{H}(\mathrm{Homgr}_A(R', E')) & \xrightarrow{\varphi(R', E')} & \mathrm{Ext}_A(M', N') \\
\mathrm{H}(\mathrm{Homgr}_A(\tilde{f}, \tilde{h})) \downarrow & & \downarrow \mathrm{Ext}_A(f, h) \\
\mathrm{H}(\mathrm{Homgr}_A(R, E)) & \xrightarrow{\varphi(R, E)} & \mathrm{Ext}_A(M, N) .
\end{array}
$$

Cho $\alpha : L(M) \to R, \alpha' : L(M') \to R', \gamma : L(P) \to S, \gamma' : L(P') \to S'$ là các cấu xạ của các phức sao cho

$$
a \circ \alpha = p_M, \quad a' \circ \alpha' = p_{M'}, \quad b \circ \gamma = p_P, \quad b' \circ \gamma' = p_{P'} .
$$

Theo định nghĩa, $\mathrm{H}(\tilde{g} \otimes \tilde{f}) \circ \psi(S, R)$ bằng

$$
\mathrm{H}(\tilde{g} \otimes \tilde{f}) \circ \mathrm{H}(\gamma \otimes \alpha) = \mathrm{H}((\tilde{g} \circ \gamma) \otimes (\tilde{f} \circ \alpha)) ,
$$

trong khi $\psi(S', R') \circ \mathrm{Tor}^A(g, f)$ bằng

$$
\mathrm{H}(\gamma' \otimes \alpha') \circ \mathrm{H}(L(g) \otimes L(f)) = \mathrm{H}((\gamma' \circ L(g)) \otimes (\alpha' \circ L(f))) .
$$

Mặt khác, $\alpha' \circ L(f)$ và $\tilde{f} \circ \alpha$ là hai cấu xạ từ $L(M)$ vào $R'$ sao cho $a' \circ (\alpha' \circ L(f)) = p_{M'} \circ L(f) = f \circ p_M = f \circ a \circ \alpha = a' \circ (\tilde{f} \circ \alpha)$. Theo X, p. 49, prop. 3, $\alpha' \circ L(f)$ và $\tilde{f} \circ \alpha$ đồng luân; tương tự $\gamma' \circ L(g)$ và $\tilde{g} \circ \gamma$ đồng luân, và do đó $(\gamma' \circ L(g)) \otimes (\alpha' \circ L(f))$ và $(\tilde{g} \circ \gamma) \otimes (\tilde{f} \circ \alpha)$ cũng đồng luân theo prop. 3 của X, p. 64. Vậy nên

$$
H(\tilde{g} \otimes \tilde{f}) \circ \psi(S, R) = H((\tilde{g} \circ \gamma) \otimes (\tilde{f} \circ \alpha)) = H((\gamma' \circ L(g)) \otimes (\alpha' \circ L(f)))
$$
$$
= \psi(S', R') \circ \mathrm{Tor}^A(g, f) .
$$

Ta lập luận tương tự đối với biểu đồ thứ hai.

#### Nhận xét {#alg-x-s6-n2-rem-1 .statement}

Tương tự, xét các biểu đồ giao hoán của các cấu xạ của các phức

$$
\begin{array}{ccc}
R_1 & \xrightarrow{a_1} & M \\
\tilde{f} \downarrow & & \downarrow f \\
R'_1 & \xrightarrow{a'_1} & M'
\end{array}
$$
$$
\begin{array}{ccc}
S_1 & \xrightarrow{b_1} & P \\
\tilde{g} \downarrow & & g \downarrow \\
S'_1 & \xrightarrow{b'_1} & P'
\end{array}
$$
$$
\begin{array}{ccc}
N' & \xrightarrow{c'_1} & E' \\
h \downarrow & & \tilde{h} \downarrow \\
N & \xrightarrow{c_1} & E_1
\end{array}
$$

trong đó các phức $R_1, R'_1, S_1, S'_1$ là xạ ảnh và không ở bên phải, và các phức $E_1, E'_1$ là đơn ánh và không ở bên trái. Khi đó

$$
\mathrm{Tor}^A(g, f) \circ \psi'(S_1, R_1) = \psi'(S'_1, R'_1) \circ H(\tilde{g} \otimes \tilde{f})
$$
$$
\varphi'(R_1, E_1) \circ \mathrm{Ext}_A(f, h) = H(\mathrm{Homgr}_A(\tilde{f}, \tilde{h})) \circ \varphi'(R'_1, E'_1)
$$

như được chứng minh tương tự như mệnh đề 2.

### 3. Tính toán các đồng cấu nối kết

Xét một biểu đồ giao hoán

(1)
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & R' & \xrightarrow{\tilde{u}} & R & \xrightarrow{\tilde{v}} & R'' & \longrightarrow & 0 \\
& & a' \downarrow & & a \downarrow & & a'' \downarrow & & \\
0 & \longrightarrow & M' & \xrightarrow{u} & M & \xrightarrow{v} & M'' & \longrightarrow & 0
\end{array}
$$

(2)

trong đó hàng thứ nhất (1) là một dãy khớp của các phức các A-môđun trái, hàng thứ hai (2) là một dãy khớp các A-môđun trái, và các mũi tên thẳng đứng là các phân giải trái.

#### Mệnh đề 3 {#alg-x-s6-prop-3 .statement}

a) Cho $P$ là một A-môđun, $b : S \to P$ là một phân giải trái của $P$; giả sử rằng dãy các phức các k-môđun

(3)
$$
0 \to S \otimes_A R' \xrightarrow{1_S \otimes \tilde{u}} S \otimes_A R \xrightarrow{1_S \otimes \tilde{v}} S \otimes_A R'' \to 0
$$

là khớp. Khi đó biểu đồ sau là giao hoán:

$$
\begin{array}{ccc}
\operatorname{Tor}^{A}(P,M'')&\xrightarrow{\partial(P,(2))}&\operatorname{Tor}^{A}(P,M')\\
\Big\downarrow\vcenter{\rlap{$\psi(S,R'')$}}&&\Big\downarrow\vcenter{\rlap{$\psi(S,R')$}}\\
H(S\otimes_A R'')&\xrightarrow{\partial(3)}&H(S\otimes_A R').
\end{array}
$$

b) Cho $N$ là một A-môđun trái, $c:N\to E$ là một phân giải phải của $N$; giả sử rằng dãy các phức các $k$-môđun

(4)

$$
0\longrightarrow \operatorname{Homgr}_A(R'',E)
\xrightarrow{\operatorname{Homgr}_A(\tilde{\imath},1)}
\operatorname{Homgr}_A(R,E)
\xrightarrow{\operatorname{Homgr}_A(\tilde{u},1)}
\operatorname{Homgr}'_A(R',E)\longrightarrow 0
$$

là khớp. Khi đó biểu đồ sau là giao hoán:

$$
\begin{array}{ccc}
H(\operatorname{Homgr}_A(R',E))
&\xrightarrow{\delta((4))}
&H(\operatorname{Homgr}_A(R'',E))
\\
\Big\downarrow\vcenter{\rlap{$\varphi(R',E)$}}
&&
\Big\downarrow\vcenter{\rlap{$\varphi(R'',E)$}}
\\
\operatorname{Ext}_A(M',N)
&\xrightarrow{\partial((2),N)}
&\operatorname{Ext}_A(M'',N).
\end{array}
$$

Chẳng hạn, ta hãy chứng minh a). Cho $\beta:L(P)\to S$ là một cấu xạ các phức sao cho
$t\circ\beta=p_P$; xét biểu đồ các k-phức

$$
\begin{array}{ccccccccc}
0&\longrightarrow&S\otimes_A R'&\xrightarrow{1\otimes\tilde{u}}&S\otimes_A R&\xrightarrow{1\otimes\tilde{v}}&S\otimes_A R''&\longrightarrow&0\\
&&\Big\uparrow\vcenter{\rlap{$\beta\otimes1_R$}}&&\Big\uparrow\vcenter{\rlap{$\beta\otimes1_R$}}&&\Big\uparrow\vcenter{\rlap{$\beta\otimes1_{R'}$}}&&\\
0&\longrightarrow&L(P)\otimes_A R'&\xrightarrow{1\otimes\tilde{u}}&L(P)\otimes_A R&\xrightarrow{1\otimes\tilde{v}}&L(P)\otimes_A R''&\longrightarrow&0\\
&&\Big\downarrow\vcenter{\rlap{$1\otimes a'$}}&&\Big\downarrow\vcenter{\rlap{$1\otimes a$}}&&\Big\downarrow\vcenter{\rlap{$1\otimes a''$}}&&\\
0&\longrightarrow&L(P)\otimes_A M'&\xrightarrow{1\otimes u}&L(P)\otimes_A M&\xrightarrow{1\otimes v}&L(P)\otimes_A M''&\longrightarrow&0.
\end{array}
$$

Đây là một biểu đồ giao hoán với các hàng khớp (do giả thiết đối với hàng thứ nhất, và do việc $L(P)$ là phẳng đối với hai hàng còn lại). Do đó ta có một biểu đồ giao hoán (X, p. 31, mệnh đề 2, và X, p. 72, định nghĩa 2)

$$
\begin{array}{ccc}
H(S\otimes_A R'')&\xrightarrow{\partial(3)}&H(S\otimes_A R')\\
\Big\uparrow\vcenter{\rlap{$H(\beta\otimes1)$}}&&\Big\uparrow\vcenter{\rlap{$H(\beta\otimes1)$}}\\
H(L(P)\otimes_A R'')&\longrightarrow&H(L(P)\otimes_A R')\\
\Big\downarrow\vcenter{\rlap{$H(1\otimes a'')$}}&&\Big\downarrow\vcenter{\rlap{$H(1\otimes a')$}}\\
H(L(P)\otimes_A M'')&\longrightarrow&H(L(P)\otimes_A M')\\
\Big\uparrow\vcenter{\rlap{$\psi_P(M'')$}}&&\Big\uparrow\vcenter{\rlap{$\psi_P(M')$}}\\
\operatorname{Tor}(P,M'')&\xrightarrow{\partial(P,(2))}&\operatorname{Tor}(P,M').
\end{array}
$$

Theo X, p. 67, mệnh đề 4, H(1 ⊗ a'') và H(1 ⊗ a') là song ánh; mặt khác, theo định nghĩa của các đồng cấu ψ, ta có H(β ⊗ 1) ◦ ψ(L(P), R'') = ψ(S, R'') và H(1 ⊗ a'') ◦ ψ(L(P), R'') = ψ(L(P), M'') = ψ_p(M''), do đó

$$
ψ(S, R'') = H(β ⊗ 1) ◦ H(1 ⊗ a'')^{-1} ◦ ψ_p(M'');
$$

tương tự, $ψ(S, R') = H(β ⊗ 1) ◦ H(1 ⊗ a')^{-1} ◦ ψ_p(M')$, và mệnh đề cần chứng minh $\partial((3)) ◦ ψ(S, R'') = ψ(S, R') ◦ \partial(P, (2))$ suy ra từ tính giao hoán của biểu đồ trên.

#### Nhận xét 1 {#alg-x-s6-n3-rem-1 .statement}

Dùng các đẳng cấu giao hoán, suy ra từ a) mệnh đề tương tự thu được bằng cách đổi vai trò của hai đối số của tích tenxơ.

#### Nhận xét 2 {#alg-x-s6-n3-rem-2 .statement}

Với các ký hiệu của a), giả sử hoặc S là phẳng, hoặc R, R', R'' là phẳng; khi đó một mặt dãy (3) là khớp (X, p. 72, hệ quả 2) và có thể áp dụng mệnh đề 3; mặt khác $ψ(S, R')$ là song ánh (định lý 1), do đó

$$
\partial(P, (2)) = ψ(S, R')^{-1} ◦ \partial((3)) ◦ ψ(S, R'').
$$

#### Nhận xét 3 {#alg-x-s6-n3-rem-3 .statement}

Với các ký hiệu của b), giả sử hoặc E là đơn ánh, hoặc R, R', R'' là xạ ảnh; khi đó một mặt dãy (4) là khớp (X, p. 83, mệnh đề 2) và có thể áp dụng mệnh đề 3; mặt khác, $φ(R', E)$ là song ánh (định lý 1) ; do đó

$$
δ((2), N) = φ(R'', E) ◦ \partial((4)) ◦ φ(R', E)^{-1}.
$$

Bây giờ xét một biểu đồ giao hoán

(5)
$$
\begin{array}{ccccccccc}
0 & \rightarrow & N' & \xrightarrow{r} & N & \xrightarrow{s} & N'' & \rightarrow & 0 \\
   &           & c'   &         &   &         & c''   &         &
\end{array}
$$

(6)
$$
\begin{array}{ccccccccc}
0 & \rightarrow & E' & \xrightarrow{\tilde{r}} & E & \xrightarrow{\tilde{s}} & E'' & \rightarrow & 0
\end{array}
$$

trong đó hàng thứ nhất (5) là một dãy khớp các A-môđun trái, hàng thứ hai (6) là một dãy khớp các phức của các A-môđun trái, và trong đó các mũi tên thẳng đứng là các phân giải phải. Lập luận như trong Mệnh đề 3, ta chứng minh mệnh đề sau:

#### Mệnh đề 4 {#alg-x-s6-prop-4 .statement}

Cho M là một A-môđun trái, $a : R \to M$ là một phân giải trái của M sao cho dãy

(7)
$$
0 \rightarrow \mathrm{Homgr}_A(R, E') \xrightarrow{\mathrm{Homgr}(\tilde{s}, 1)} \mathrm{Homgr}_A(R, E) \xrightarrow{\mathrm{Homgr}(\tilde{r}, 1)} \mathrm{Homgr}_A(R, E'') \rightarrow 0
$$

là khớp. Khi đó biểu đồ sau là giao hoán.

$$
\begin{array}{ccc}
\mathrm{H}(\mathrm{Homgr}_A(R, E'')) & \xrightarrow{\partial((7))} & \mathrm{H}(\mathrm{Homgr}_A(R, E')) \\
\varphi(R, E'') \downarrow & & \downarrow \varphi(R, E') \\
\mathrm{Ext}_A(M, N'') & \xrightarrow{\delta(M, (5))} & \mathrm{Ext}_A(M, N')
\end{array}
$$

#### Nhận xét 4 {#alg-x-s6-n3-rem-4 .statement}

Nếu R là xạ ảnh hoặc nếu E, E', E'' là đơn ánh, thì dãy (7) là khớp ($\lambda$, p. 83, Mệnh đề 2); hơn nữa, $\varphi(R, E'')$ là song ánh (Định lý 1); do đó

$$
\delta(M, (5)) = \varphi(R, E') \circ \partial((7)) \circ \varphi(R, E'')^{-1}.
$$

#### Nhận xét 5 {#alg-x-s6-n3-rem-5 .statement}

Chúng tôi để bạn đọc phát biểu và chứng minh các mệnh đề tương tự với các Mệnh đề 3 và 4 và liên quan đến các đồng cấu $\psi_1$ và $\varphi_1$.

### 4. Tính hữu hạn của các môđun mở rộng và xoắn

Cho M là một A-môđun trái, I là một tập tiền thứ tự lọc, $(N_i, u_{ji})$ là một hệ quy nạp các A-môđun trái đối với I, $N = \lim N_i$ là giới hạn quy nạp của nó, $u_i : N_i \to N,\ i \in I$, là ánh xạ chính tắc. Khi đó $(\mathrm{Ext}_A(M, N_i), \mathrm{Ext}_A(l_M, u_{ji}))$ là một hệ quy nạp các $k$-môđun và $(\mathrm{Ext}_A(l_M, u_i))$ là một hệ quy nạp các ánh xạ, mà giới hạn quy nạp là một đồng cấu của các $k$-môđun phân bậc, gọi là *chính tắc*

$$
\lim_{i \in I} \mathrm{Ext}_A(M, N_i) \to \mathrm{Ext}_A(M, \lim_{i \in I} N_i).
$$

#### Mệnh đề 5 {#alg-x-s6-prop-5 .statement}

*Nếu A là Noether trái và nếu M là một A-môđun hữu hạn sinh, thì đồng cấu chính tắc (8) là song ánh.*

Thật vậy, theo (X, p. 53, Mệnh đề 6), gọi $p : L \to M$ là một phân giải tự do của M sao cho $L_n$ là kiểu hữu hạn với mỗi $n$. Cấu xạ chính tắc của các $k$-phức

$$
u : \lim \mathrm{Homgr}_A(L, N_i) \to \mathrm{Homgr}_A(L, \lim N_i)
$$

là song ánh, do đó đồng cấu

$$
\lim \mathrm{H}(\mathrm{Homgr}_A(L, N_i)) \to \mathrm{H}(\mathrm{Homgr}_A(L, \lim N_i))
$$

suy ra từ các đồng cấu $\mathrm{H}(\mathrm{Homgr}(l, u_i))$ cũng vậy (X, p. 28, Mệnh đề 1). Sau đó ta kết luận nhờ Mệnh đề 2 (X, p. 103) và Định lý 1 (X, p. 100).

#### Mệnh đề 6 {#alg-x-s6-prop-6 .statement}

*Cho B là một vành và N là một song môđun (A, B), là một B-môđun Noether (resp. có độ dài hữu hạn).

a) Giả sử A Noether phải và cho M là một A-môđun phải hữu hạn sinh. Khi đó các B-môđun (X, p. 81) $\mathrm{Tor}_n^A(M, N)$ là Noether (resp. có độ dài hữu hạn).

b) Giả sử A Noether trái và cho M là một A-môđun trái hữu hạn sinh. Khi đó các B-môđun (X, p. 98) $\mathrm{Ext}_A^n(M, N)$ là Noether (resp. có độ dài hữu hạn).*

Chọn một phân giải tự do $p : L \to M$ sao cho mỗi A-môđun $L_n$ là kiểu hữu hạn (X, p. 53, Mệnh đề 6), và gọi C là phức các B-môđun $L \otimes_A N$ trong trường hợp $a$, $\mathrm{Homgr}_A(L, N)$ trong trường hợp $b$. Mỗi B-môđun $C_n$ đẳng cấu với một tích của một số hữu hạn bản sao của N, nên là Noether (resp. có độ dài hữu hạn); vì vậy điều tương tự cũng đúng đối với các môđun $\mathrm{H}_n(C)$. Nhưng, theo X, p. 100, Định lý 1, các môđun này đẳng cấu với các $\mathrm{Tor}_n^A(M, N)$ trong trường hợp $a$, với các $\mathrm{Ext}_A^{-n}(M, N)$ trong trường hợp $b$.

#### Hệ quả {#alg-x-s6-n4-cor-1 .statement}

Cho $\rho : A \to B$ là một đồng cấu của các vành giao hoán Noether, $M$ là một $A$-môđun hữu hạn sinh, $N$ là một $B$-môđun. Nếu $N$ là một $B$-môđun hữu hạn sinh (resp. có độ dài hữu hạn), thì điều tương tự cũng đúng đối với các $B$-môđun $\operatorname{Tor}^{A}_{n}(M,N)$ và $\operatorname{Ext}^{n}_{A}(M,N)$.

### 5. Các đồng cấu $\operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to \operatorname{Tor}^{B}(P,N \otimes_{A} Q)$ và $\operatorname{Ext}_{B}(M,N) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q)$

Cho $B$ là một vành, $N$ là một song môđun $(B,A)$, $M$ là một $B$-môđun trái, $P$ là một
$B$-môđun phải, $Q$ là một $A$-môđun trái.
Theo X, p. 62, ta có một đồng cấu

$$
\gamma_{1} : H(L(P) \otimes_{B} N) \otimes_{A} Q \to H(L(P) \otimes_{B} N \otimes_{A} Q) \,;
$$

hơn nữa (X, p. 69, Mệnh đề 5), ta có các đẳng cấu

$$
\psi_{1}(N) : \operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to H(L(P) \otimes_{B} N) \otimes_{A} Q \,,
$$

$$
\psi_{1}(N \otimes_{A} Q) : \operatorname{Tor}^{B}(P,N \otimes_{A} Q) \to H(L(P) \otimes_{B} N \otimes_{A} Q) \,.
$$

Đồng cấu phân bậc bậc 0, gọi là *chính tắc*

(9)

$$
\operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to \operatorname{Tor}^{B}(P,N \otimes_{A} Q)
$$

được định nghĩa là hợp thành $\psi_{P}(N \otimes_{A} Q)^{-1} \circ \gamma_{1} \circ (\psi_{P}(N) \otimes 1_{Q})$.

Tương tự, từ cấu xạ chính tắc của các phức

$$
\alpha : \operatorname{Homgr}_{B}(L(M),N) \otimes_{A} Q \to \operatorname{Homgr}_{B}(L(M),N \otimes_{A} Q)
$$

suy ra một đồng cấu $H(\alpha)$; ta có đồng cấu chính tắc (X, p. 62)

$$
\gamma_{2} : H(\operatorname{Homgr}_{B}(L(M),N)) \otimes_{A} Q \to H(\operatorname{Homgr}_{B}(L(M),N \otimes_{A} Q)) \,,
$$

và các đẳng cấu (X, p. 88, mệnh đề 5)

$$
\varphi_{M}(N) : H(\operatorname{Homgr}_{B}(L(M),N)) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N) \otimes_{A} Q \,,
$$

$$
\varphi_{M}(N \otimes_{A} Q) : H(\operatorname{Homgr}_{B}(L(M),N \otimes_{A} Q)) \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q) \,.
$$

Đồng cấu phân bậc bậc 0, gọi là *chính tắc*

(10)

$$
\operatorname{Ext}_{B}(M,N) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q)
$$

được định nghĩa là hợp thành

$$
\varphi_{M}(N \otimes_{A} Q) \circ H(\alpha) \circ (\varphi_{M}(N) \otimes 1_{Q})^{-1} \,.
$$

#### Mệnh đề 7 {#alg-x-s6-prop-7 .statement}

a) Nếu $A$-môđun $Q$ là phẳng thì đồng cấu (9) là song ánh.
b) Nếu $A$-môđun $Q$ là xạ ảnh sinh hữu hạn thì đồng cấu (10) là song ánh.

c) Nếu $A$-môđun $Q$ là phẳng, vành $B$ là Noether và $B$-môđun $M$ sinh hữu hạn thì đồng cấu (10) là song ánh.

a) Nếu $Q$ là phẳng thì $\gamma_1$ là song ánh ($X$, p. 66, hệ quả 2).

b) Nếu $Q$ là xạ ảnh sinh hữu hạn thì nó phẳng, do đó $\gamma_2$ là song ánh, và hơn nữa $\alpha$ là song ánh (II, p. 75, mệnh đề 2, a)).

c) Dưới các giả thiết của c), $\gamma_2$ là song ánh vì $Q$ phẳng. Hơn nữa ($X$, p. 53, mệnh đề 6), tồn tại một phân giải $L$ của $M$ sao cho mỗi $L_n$ là tự do sinh hữu hạn; gọi $u : L(M) \to L$ là một đồng luân cấu xạ ($X$, p. 49, hệ quả của mệnh đề 3); trong biểu đồ giao hoán,

$$
\begin{array}{ccc}
\mathrm{Homgr}_B(L(M), N) \otimes_A Q & \xrightarrow{\alpha} & \mathrm{Homgr}_B(L(M), N \otimes_A Q) \\
\uparrow & & \uparrow \\
\mathrm{Homgr}_B(L, N) \otimes_A Q & \xrightarrow{\bar{\alpha}} & \mathrm{Homgr}_B(L, N \otimes_A Q).
\end{array}
$$

các mũi tên thẳng đứng suy ra từ $u$ là các đồng luân cấu xạ ($X$, p. 64, mệnh đề 3 và p. 83, mệnh đề 3) và $\bar{\alpha}$ là song ánh (II, p. 75, mệnh đề 2 (ii)); do đó $H(\alpha)$ là song ánh, và đồng cấu (10) là song ánh.

### 6. Các đồng cấu $\mathrm{Tor}^B(P, N \otimes_A Q) \to \mathrm{Tor}^A(P \otimes_B N, Q)$ và $\mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)) \to \mathrm{Ext}_B(N \otimes_A Q, M)$

Giữ các ký hiệu trước đây, và giả sử rằng $N$ phẳng trên $A$. Khi đó cấu xạ $N \otimes_A L(Q) \xrightarrow{1 \otimes p_Q} N \otimes_A Q$ là một đồng điều cấu xạ ($X$, p. 67, mệnh đề 4), do đó có các đồng cấu

$$
\psi(P, N \otimes_A L(Q)) : \mathrm{Tor}^B(P, N \otimes_A Q) \to H(P \otimes_B N \otimes_A L(Q))
$$
$$
\varphi(N \otimes_A L(Q), M) : H(\mathrm{Homgr}_B(N \otimes_A L(Q), M)) \to \mathrm{Ext}_B(N \otimes_A Q, M).
$$

Khi đó dùng các *đẳng cấu*

$$
\overline{\psi}_Q(P \otimes_B N) : \mathrm{Tor}^A(P \otimes_B N, Q) \to H(P \otimes_B N \otimes_A L(Q)),
$$
$$
\beta : \mathrm{Homgr}_A(L(Q), \mathrm{Hom}_B(N, M)) \to \mathrm{Homgr}_B(N \otimes_A L(Q), M),
$$
$$
\varphi_Q(\mathrm{Hom}_B(N, M)) : H(\mathrm{Homgr}_A(L(Q), \mathrm{Hom}_B(N, M))) \to \mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)),
$$

ta suy ra từ chúng các đồng cấu phân bậc bậc 0 gọi là *chính tắc*:

(11) $$ \mathrm{Tor}^B(P, N \otimes_A Q) \to \mathrm{Tor}^A(P \otimes_B N, Q) $$
(12) $$ \mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)) \to \mathrm{Ext}_B(N \otimes_A Q, M). $$

#### Mệnh đề 8 {#alg-x-s6-prop-8 .statement}

*a)* Nếu $N$ phẳng trên $A$ và trên $B$ thì đồng cấu (11) là song ánh.

*b)* Nếu $N$ phẳng trên $A$ và xạ ảnh trên $B$ thì đồng cấu (12) là song ánh.

Thật vậy $N \otimes_A L(Q)$ đẳng cấu với một tổng trực tiếp các bản sao của $N$, do đó là một $B$-môđun phẳng (resp. xạ ảnh) khi $B$-môđun $N$ là phẳng (resp. xạ ảnh); khi đó áp dụng Định lý 1 (X, p. 100).

### 7. Các đồng cấu $B \otimes_A \mathrm{Tor}^A(E, F) \to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)$ và $B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F)$

Trong số này, ta giả sử rằng $A$ là *giao hoán*; cho một đồng cấu vành $\rho : A \to B$ sao cho $\rho(A)$ được chứa trong tâm của $B$ và hai $A$-môđun $E$ và $F$. Có một đẳng cấu chính tắc của các phức $A$-môđun

$$
u : B \otimes_A (L(E) \otimes_A L(F)) \to (L(E) \otimes_A B) \otimes_B (B \otimes_A L(F));
$$

mặt khác, vì $L(E) \otimes_A B$ và $B \otimes_A L(F)$ là các $B$-phức *tự do*, nên có một đồng cấu chính tắc của các $A$-môđun phân bậc (X, p. 102)

$$
\psi'(L(E) \otimes_A B, B \otimes_A L(F)) : H((L(E) \otimes_A B) \otimes_B (B \otimes_A L(F)))
$$
$$
\to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)
$$

sau hết, có một đồng cấu (X, p. 62)

$$
\gamma : B \otimes_A \mathrm{Tor}^A(E, F) \to H(B \otimes_A L(E) \otimes_A L(F)).
$$

Đồng cấu *chính tắc* của các $B$-môđun phân bậc

(13)
$$
B \otimes_A \mathrm{Tor}^A(E, F) \to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)
$$

được định nghĩa là hợp thành $\psi'(L(E) \otimes_A B, B \otimes_A L(F)) \circ H(u) \circ \gamma$.

#### Mệnh đề 9 {#alg-x-s6-prop-9 .statement}

*Nếu $B$ phẳng trên $A$, thì đồng cấu (13) là song ánh.*
Thật vậy $\psi'(L(E) \otimes_A B, B \otimes_A L(F))$ là song ánh (X, p. 102, prop. 1) và $\gamma$ là song ánh (X, p. 66, hệ quả 2).

Giả sử $B$ *phẳng* trên $A$. Thay $E$ cho $Q$, $B$ cho $N$ và $B \otimes_A F$ cho $M$ trong đồng cấu (12), ta thu được một đồng cấu

$$
\mathrm{Ext}_A(E, B \otimes_A F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F)
$$

đồng cấu này là song ánh theo Mệnh đề 8. Thay $E$ cho $M$, $F$ cho $N$, $A$ cho $B$, $B$ cho $Q$, trong đồng cấu (10), và đổi chỗ các thừa số trong các tích tenxơ, ta thu được một đồng cấu của các $B$-môđun

$$
B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_A(E, B \otimes_A F),
$$

do đó, bằng hợp thành, một đồng cấu gọi là *chính tắc*

(14)
$$
B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F).
$$

#### Mệnh đề 10 {#alg-x-s6-prop-10 .statement}

Đồng cấu (14) là song ánh trong các trường hợp sau:
a) B là một A-môđun xạ ảnh sinh hữu hạn;
b) B là một A-môđun phẳng, A là Noether, và E là một A-môđun hữu hạn sinh.
Điều này suy ra từ Mệnh đề 7 (X, p. 108).

### 8. Ứng dụng: đồng điều và đối đồng điều của nhóm

Cho G là một nhóm, $\mathbf{Z}^{(G)}$ đại số của nó trên $\mathbf{Z}$ (III, p. 19). Nhắc lại (x. III, p. 20, ví dụ) rằng nếu M là một nhóm giao hoán, thì việc cho một tác động của G trên M (nghĩa là một đồng cấu $\tau : G \to \mathrm{Aut}(M)$), hay một cấu trúc môđun trái trên $\mathbf{Z}^{(G)}$ cho nhóm cộng M, là như nhau. Đặc biệt, ta sẽ coi nhóm $\mathbf{Z}$ như một môđun trái trên $\mathbf{Z}^{(G)}$ bằng cách trang bị cho nó tác động tầm thường.

#### Định nghĩa 1 {#alg-x-s6-def-1 .statement}

Cho M là một $\mathbf{Z}^{(G)}$-môđun trái (tương ứng phải), $n$ là một số nguyên $\geqslant 0$. Nhóm $\mathrm{Ext}_{\mathbf{Z}^{(G)}}^n(\mathbf{Z}, M)$ (tương ứng $\mathrm{Tor}_n^{\mathbf{Z}^{(G)}}(M, \mathbf{Z})$) được ký hiệu bởi $H^n(G, M)$ (tương ứng $H_n(G, M)$) và được gọi là nhóm đối đồng điều thứ $n$ (tương ứng nhóm đồng điều) của G với hệ số trong M.

Phân giải tiêu chuẩn (X, p. 58) $B(\mathbf{Z}^{(G)}, \mathbf{Z})$ là một phân giải tự do của $\mathbf{Z}^{(G)}$-môđun $\mathbf{Z}$; suy ra rằng các nhóm $H^n(G, M)$ (tương ứng $H_n(G, M)$) được đồng nhất với các nhóm đồng điều của phức:

$$
\mathrm{Hom}_{\mathbf{Z}^{(G)}}(B(\mathbf{Z}^{(G)}, \mathbf{Z}), M) \quad (\text{resp. } M \otimes_{\mathbf{Z}^{(G)}} B(\mathbf{Z}^{(G)}, \mathbf{Z})) .
$$

Dùng đẳng cấu chính tắc của $(\mathbf{Z}^{(G)})^{\otimes n}$ lên $\mathbf{Z}^{(G^n)}$ (III, p. 36) và các tính chất của mở rộng vô hướng (II, p. 82), ta suy ra rằng $H^n(G, M)$ đẳng cấu chính tắc với nhóm đồng điều bậc tăng $n$ của phức $C(G, M)$ được xác định như sau: $C^n(G, M) = 0$ với $n < 0$; với $n \geqslant 0$, $C^n(G, M)$ là $\mathbf{Z}$-môđun các ánh xạ từ $G^n$ vào M; với $n \geqslant 0$, vi phân $d^n : C^n(G, M) \to C^{n+1}(G, M)$ được cho bởi

$$
(d^n f)(g_0, ..., g_n) = g_0 \cdot f(g_1, ..., g_n) + \sum_{i=0}^{n-1} (-1)^{i+1} f(g_0, ..., g_i g_{i+1}, ..., g_n)
$$
$$
+ (-1)^{n+1} f(g_0, ..., g_{n-1})
$$

với mọi $f$ trong $C^n(G, M)$ và $g_0, ..., g_n$ trong G.

Tương tự, $H_n(G, M)$ được đồng nhất với nhóm đồng điều bậc $n$ của phức $C'(G, M)$, trong đó $C'_n(G, M) = M \otimes_{\mathbf{Z}} \mathbf{Z}^{(G^n)}$ với $n \geqslant 0$, $C'_n(G, M) = 0$ với $n < 0$, vi phân $d_n : C'_n(G, M) \to C'_{n-1}(G, M)$ được xác định bởi:

$$
d_n(m \otimes e_{g_1, ..., g_n}) = m \cdot g_1 \otimes e_{g_2, ..., g_n} + \sum_{i=1}^{n-1} (-1)^i m \otimes e_{g_1, ..., g_i g_{i+1}, ..., g_n}
$$
$$
+ (-1)^n m \otimes e_{g_1, ..., g_{n-1}}
$$

với mọi $n \geqslant 1$, $m$ trong M và $g_1, ..., g_n$ trong G.

#### Ví dụ 1 {#alg-x-s6-n8-exa-1 .statement}

Từ định nghĩa suy ra trực tiếp rằng $H^0(G, M)$ đẳng cấu với môđun con các phần tử của $M$ bất biến dưới tác động của $G$, và $H_0(G, M)$ đẳng cấu với môđun thương của $M$ theo môđun con sinh bởi các phần tử $m.g-m$ với $m\in M$, $g\in G$.

#### Ví dụ 2 {#alg-x-s6-n8-exa-2 .statement}

Từ điều trên suy ra rằng $H^1(G, M)$ đẳng cấu với $\mathbf{Z}$-môđun $Z^1(G, M)/B^1(G, M)$, trong đó $Z^1(G, M)$ là $\mathbf{Z}$-môđun các ánh xạ $f$ từ $G$ vào $M$ thỏa mãn:

$$
f(g_1,g_2)=g_1.f(g_2)+f(g_1)\quad\text{với mọi }g_1,g_2\text{ trong }G,
$$

và $B^1(G, M)$ là môđun con trên $\mathbf{Z}$ của $Z^1(G, M)$ gồm các $f$ sao cho tồn tại một phần tử $m$ của $M$ thỏa mãn:

$$
f(g)=g.m-m\quad\text{với mọi }g\in G.
$$

Đôi khi người ta nói rằng $Z^1(G, M)$ là $\mathbf{Z}$-môđun của các đồng cấu chéo từ $G$ vào $M$, và $B^1(G, M)$ là môđun con của các đồng cấu chéo chính.

Ký hiệu bởi $\iota:G\to \operatorname{Aut}(M)$ đồng cấu suy ra từ tác động của $G$; xét tích nửa trực tiếp ngoài $M\times_{\iota}G$ và mở rộng $\xi_{\iota}:M\times_{\iota}G\to G$ (I, p. 64). Cho $e:G\to M\times_{\iota}G$ là một ánh xạ sao cho $\rho\circ e=1_G$; ta có $e=(f,1_G)$, trong đó $f\in C^1(G,M)$. Để $e$ là một đồng cấu (nghĩa là, một tiết diện của mở rộng $\xi_{\iota}$), điều kiện cần và đủ là $f\in Z^1(G,M)$. Để hai tiết diện của $\xi_{\iota}$ liên hợp với nhau bởi một phần tử của $i(M)$, điều kiện cần và đủ là các đồng cấu chéo tương ứng có cùng lớp trong $H^1(G,M)$.

Khi $G$ tác động tầm thường trên $M$, ta có $B^1(G,M)=0$ và $H^1(G,M)$ đẳng cấu với $\mathbf{Z}$-môđun các đồng cấu nhóm từ $G$ vào $M$.

#### Ví dụ 3 {#alg-x-s6-n8-exa-3 .statement}

Tương tự, $H^2(G,M)$ đẳng cấu với $\mathbf{Z}$-môđun $Z^2(G,M)/B^2(G,M)$, trong đó $Z^2(G,M)$ là $\mathbf{Z}$-môđun các ánh xạ $f$ từ $G\times G$ vào $M$, thỏa mãn:

$$
g_1.f(g_2,g_3)-f(g_1g_2,g_3)+f(g_1,g_2g_3)-f(g_1,g_2)=0
$$

với mọi $g_1,g_2,g_3$ trong $G$, và $B^2(G,M)$ là môđun con trên $\mathbf{Z}$ của $Z^2(G,M)$ gồm các $f$ sao cho tồn tại một ánh xạ $h$ từ $G$ vào $M$ thỏa mãn:

$$
f(g_1,g_2)=g_1.h(g_2)-h(g_1g_2)+h(g_1)
$$

với mọi $g_1,g_2$ trong $G$.

Như vậy ta thu lại định nghĩa của nhóm $H^2(G,M)$ đã cho trong VIII, App. II; đặc biệt, tồn tại một đẳng cấu chính tắc từ $H^2(G,M)$ lên nhóm các lớp mở rộng của $G$ bởi $M$ (loc. cit.).

#### Ví dụ 4 {#alg-x-s6-n8-exa-4 .statement}

Cho $M$ là một $\mathbf{Z}$-môđun, được xét như một $\mathbf{Z}^{(G)}$-môđun phải bằng cách cho $G$ tác động tầm thường. Nhóm $H_1(G,M)$ đẳng cấu với thương của $M\otimes_{\mathbf{Z}}\mathbf{Z}^{(G)}$ bởi môđun con-$\mathbf{Z}$ sinh bởi các phần tử $m\otimes(e_{g_1g_2}-e_{g_1}-e_{g_2})$ với $m$ trong $M$, $g_1,g_2$ trong $G$; suy ra dễ dàng rằng $H_1(G,M)$ đẳng cấu với $M\otimes_{\mathbf{Z}}(G/(G,G))$.

Kí hiệu $\sigma$ là phản tự đẳng cấu của $\mathbf{Z}^{(G)}$ được định nghĩa bởi $\sigma(e_g) = e_{g^{-1}}$ với $g \in G$. Mọi $\mathbf{Z}^{(G)}$-môđun trái đều có thể được xét như một $\mathbf{Z}^{(G)}$-môđun phải nhờ $\sigma$, và ngược lại. Điều này cho phép, chẳng hạn, định nghĩa các nhóm $H_q(G, M)$ đối với một $\mathbf{Z}^{(G)}$-môđun trái $M$, bằng cách đặt $H_q(G, M) = H_q(G, \sigma_*(M)) = \mathrm{Tor}_q^{\mathbf{Z}^{(G)}}(\mathbf{Z}, M)$.

#### Bổ đề 1 {#alg-x-s6-lem-1 .statement}

*Cho $M$ là một $\mathbf{Z}$-môđun; kí hiệu $M^G$ là nhóm $\mathrm{Hom}_{\mathbf{Z}}(\mathbf{Z}^{(G)}, M)$ được trang bị cấu trúc tự nhiên của $\mathbf{Z}^{(G)}$-môđun trái. Khi đó:*

$$
H^i(G, M^G) = 0 \quad \text{với} \quad i \geqslant 1 .
$$

Thật vậy, từ Mệnh đề 8, b) (X, p. 109), áp dụng với $A = N = \mathbf{Z}^{(G)}$ và $B = Q = \mathbf{Z}$, suy ra có một đẳng cấu chính tắc:

$$
\mathrm{Ext}_{\mathbf{Z}^{(G)}}(\mathbf{Z}, M^G) \to \mathrm{Ext}_{\mathbf{Z}}(\mathbf{Z}, M)
$$

do đó có bổ đề.

#### Mệnh đề 11 {#alg-x-s6-prop-11 .statement}

*Cho $L$ là một mở rộng Galois bậc hữu hạn của một trường giao hoán $K$, với nhóm Galois $G$.
a) *Ta có* $H^i(G, L) = 0$ *với* $i \geqslant 1$.
b) *Ta có* $H^1(G, L^*) = 0$.
c) *Nhóm* $H^2(G, L^*)$ *đẳng cấu chính tắc với nhóm* $\mathrm{Br}(K, L)$ *(VIII, § 13)*.

Định lý cơ sở chuẩn tắc (V, §10, No. 9, Định lý 6) cho thấy rằng $L$ đẳng cấu, với tư cách là một $\mathbf{Z}^{(G)}$-môđun, với $K^G = \mathrm{Hom}_{\mathbf{Z}}(\mathbf{Z}^{(G)}, K)$; khi đó mệnh đề a) suy ra từ Bổ đề 1. Theo Ví dụ 2, mệnh đề b) suy ra từ V, §10, No. 5, Hệ quả 1 của Mệnh đề 9: sau cùng, mệnh đề c) đã được chứng minh trong VIII, §13.

## BÀI TẬP {#alg-x-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
