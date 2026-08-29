---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 5
section_title: Modules d’extensions
lang: vi
source: alg-x-fr
book_pages: A X.81-A X.100
pdf_pages: 0087-0106, 0193-0194
extraction: ocr
subsections:
    - "no": 1
      title: ' Complexes d’homomorphismes'
      page: 81
      pdf_page: 87
    - "no": 2
      title: Complexes d’homomorphismes et homotopies
      page: 83
      pdf_page: 89
    - "no": 3
      title: Définition et premières propriétés des modules d’extensions
      page: 86
      pdf_page: 92
    - "no": 4
      title: Les homomorphismes de liaison et les suites exactes
      page: 89
      pdf_page: 95
    - "no": 5
      title: Modules projectifs, modules injectifs et modules d’extensions
      page: 93
      pdf_page: 99
    - "no": 6
      title: Formule des coefficients universels
      page: 94
      pdf_page: 100
    - "no": 7
      title: Généralisation aux complexes de multimodules ; les isomorphismes canoniques
      page: 98
      pdf_page: 104
statements: 36
exercises: 8
content_sha256: c4f270b402e8a155330b74e70a2a218bfeeac7c7cfdd475b9bf8631d8ea513d9
translated_from: content/en-mt/alg/X/05_s5_modules_d_extensions.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 2a8f00d4abc6191a2668f4c8873a54f6d7bcf2ec527b7111642fb1cc059355aa
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-dc665973
glossary_version: 34
glossary_terms_sha256: 9cb1f15b66c0b7eda0e6ca90bc1cbebfd71a60edd068488433abe6f90fe7ec61
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC MÔĐUN CỦA CÁC MỞ RỘNG

*Ta giữ lại các ký hiệu tổng quát của đoạn 4. Ta cũng quy ước rằng, trừ khi có nói rõ khác đi, tất cả các môđun được xét đều là các môđun trái, tất cả các phức được xét đều là các phức của các môđun trái.*

### 1.  Các phức của các đồng cấu

Cho $(C,d)$ và $(C',d')$ là hai phức A. Xét K-môđun phân bậc $\operatorname{Homgr}_A(C,C')$ (II, p. 174, 175): với $n\in\mathbf{Z}$, $\operatorname{Homgr}_A(C,C')_n$ là K-môđun của các ánh xạ A-tuyến tính phân bậc bậc $n$ từ $C$ vào $C'$; nói cách khác $\operatorname{Homgr}_A(C,C')$ được đồng nhất một cách chính tắc với A-môđun

$$
\bigoplus_{n\in\mathbf{Z}}\prod_{p\in\mathbf{Z}}\operatorname{Hom}_A(C_p,C'_{p+n})
=
\bigoplus_{n\in\mathbf{Z}}\prod_{p+q=n}\operatorname{Hom}_A(C_p,{C'}^q).
$$

Định nghĩa các ánh xạ K-tuyến tính

$$
D_n:\operatorname{Homgr}_A(C,C')_n\longrightarrow
\operatorname{Homgr}_A(C,C')_{n-1},\qquad n\in\mathbf{Z},
$$

bởi

(1) $$
D_n(f)=d'\circ f-(-1)^n f\circ d;
$$

ta có

$$
D_{n-1}\circ D_n(f)
=D_{n-1}\bigl(d'\circ f-(-1)^n f\circ d\bigr)
=d'\circ d'\circ f-(-1)^n d'\circ f\circ d
$$

$$
\qquad\qquad{}-(-1)^{n-1}d'\circ f\circ d-f\circ d\circ d=0.
$$

Khi đó $(\operatorname{Homgr}_A(C,C'),D)$ là một phức của các K-môđun được gọi là *phức các đồng cấu của $C$ vào $C'$*.

Chẳng hạn, Homgr_A (A, C') được đồng nhất một cách chính tắc với C'. Cũng chú ý rằng, với mọi $n \in \mathbf{Z}$, ta có $\mathrm{Homgr}_A (C, C') (n) = \mathrm{Homgr}_A (C, C'(n))$.

Các phần tử của $Z_n(\mathrm{Homgr}_A (C, C'))$ là các đồng cấu phân bậc $f$ có bậc (giảm dần) $n$ từ $C$ vào $C'$ sao cho $d' \circ f = (-1)^n f \circ d$, nghĩa là các cấu xạ của các phức từ $C$ vào $C'(n)$, hoặc tương đương từ $C(p)$ vào $C'(p+n)$ với mọi $p$ cố định. Chúng được gọi là *các cấu xạ của các phức có bậc* (giảm dần) $n$ *từ C vào C'*; nếu $f, g \in Z_n(\mathrm{Homgr}_A (C, C'))$ và $s \in \mathrm{Homgr}_A (C, C')_{n+1}$, thì điều kiện $g - f = Ds$ có nghĩa là $s$ là một đồng luân nối các cấu xạ $f$ và $g$ từ $C$ vào $C'(n)$, do đó $H_n(\mathrm{Homgr}_A (C, C'))$ *là K-môđun của các lớp đồng luân của các cấu xạ có bậc giảm dần n từ C vào C'*.

Cho $\alpha \in H_n(\mathrm{Homgr}_A (C, C'))$ và $p \in \mathbf{Z}$. Biểu diễn $\alpha$ bởi $f \in Z_n(\mathrm{Homgr}_A (C, C'))$; khi đó $f$ là một cấu xạ của các phức từ $C$ vào $C'(n)$, do đó $H_p(f)$ là một đồng cấu từ $H_p(C)$ vào $H_p(C'(n)) = H_{p+n}(C')$; vì $H_p(f)$ chỉ phụ thuộc vào lớp đồng luân $\alpha$ của $f$ (X, p. 33, prop. 3), ta suy ra một đồng cấu chính tắc của các K-môđun

$$
H_n(\mathrm{Homgr}_A (C, C')) \to \mathrm{Hom}_A (H_p(C), H_{p+n}(C')) ,
$$

do đó một *ánh xạ K-tuyến tính phân bậc bậc* 0, được gọi là *chính tắc*

$$
\lambda(C, C') : H(\mathrm{Homgr}_A (C, C')) \to \dot{\mathrm{Homgr}}_A (H(C), H(C')) .
$$

Các thành phần thuần nhất của $\lambda(C, C')$ thường được ký hiệu:

$$
\lambda^n(C, C') : H^n(\mathrm{Homgr}_A (C, C')) \to \prod_{p+q=n} \mathrm{Hom}_A (H_p(C), H^q(C')) .
$$

#### Mệnh đề 1 {#alg-x-s5-prop-1 .statement}

*Nếu C là không ở bên phải và C' là không ở bên trái, thì Homgr_A (C, C') là không ở bên trái, và ánh xạ K-tuyến tính chính tắc*

$$
\lambda^0(C, C') : H^0(\mathrm{Homgr}_A (C, C')) \to \mathrm{Hom}_A (H_0(C), H^0(C'))
$$

*là song ánh*.

Ta có các dãy khớp

$$
\begin{aligned}
&0 \longrightarrow H^0(C') \xrightarrow{i} {C'}^0 \xrightarrow{{d'}^0} {C'}^1 \\
&C_1 \xrightarrow{d_1} C_0 \xrightarrow{p} H_0(C) \longrightarrow 0 .
\end{aligned}
$$

Mặt khác $\mathrm{Homgr}_A^0 (C, C')$ được đồng nhất với $\mathrm{Hom}_A (C_0, {C'}^0)$, $Z^0(\mathrm{Homgr}_A (C, C'))$ khi đó được đồng nhất với tập hợp các $f : C_0 \to {C'}^0$ sao cho ${d'}^0 \circ f = 0, f \circ d_1 = 0$; $B^0(\mathrm{Homgr}_A (C, C'))$ là không; cuối cùng ánh xạ $\lambda^0$ gán cho lớp của $f$ modulo $\{0\}$ đồng cấu $\varphi : H_0(C) \to H^0(C')$ sao cho $f = i \circ \varphi \circ p$, do đó có mệnh đề.

Cho $u : \tilde{C} \to C$ và $u' : C' \to \tilde{C}'$ là các cấu xạ của các phức; khi đó đồng cấu chính tắc $\mathrm{Homgr}_A (u, u') : \mathrm{Homgr}_A (C, C') \to \mathrm{Homgr}_A (\tilde{C}, \tilde{C}')$, được xác định bởi $f \mapsto u' \circ f \circ u$, là một cấu xạ của các phức, như suy ra ngay lập tức từ công thức (1). Hơn nữa, biểu đồ sau là giao hoán

$$
\begin{array}{ccc}
H(\mathrm{Homgr}_A(C, C')) & \xrightarrow{\lambda(C, C')} & \mathrm{Homgr}_A(H(C), H(C')) \\
\downarrow H(\mathrm{Homgr}_A(u, u')) & & \downarrow \mathrm{Homgr}_A(H(u), H(u')) \\
H(\mathrm{Homgr}_A(\tilde{C}, \tilde{C}')) & \xrightarrow{\lambda(\tilde{C}, \tilde{C}') } & \mathrm{Homgr}_A(H(\tilde{C}), H(\tilde{C}')) .
\end{array}
$$

#### Mệnh đề 2 {#alg-x-s5-prop-2 .statement}

*a) Cho $C' \xrightarrow{u} C \xrightarrow{v} C''$ là một dãy khớp của các phức $A$, $P$ là một phức xạ ảnh, $E$ là một phức đơn ánh (X, p. 25). Khi đó các dãy*

$$
\mathrm{Homgr}_A(P, C') \xrightarrow{\mathrm{Homgr}(1,u)} \mathrm{Homgr}_A(P, C) \xrightarrow{\mathrm{Homgr}(1,v)} \mathrm{Homgr}_A(P, C'')
$$

*và*

$$
\mathrm{Homgr}_A(C'', E) \xrightarrow{\mathrm{Homgr}(v,1)} \mathrm{Homgr}_A(C, E) \xrightarrow{\mathrm{Homgr}(u,1)} \mathrm{Homgr}_A(C', E)
$$

*là các dãy khớp của các phức các $k$-môđun.*

*b) Cho $0 \to C' \xrightarrow{u} C \xrightarrow{v} C'' \to 0$ là một dãy các phức $A$ được tách như một dãy khớp của các $A$-môđun phân bậc (đây là trường hợp chẳng hạn nếu $C'$ là đơn ánh, hoặc nếu $C''$ là xạ ảnh). Khi đó với mọi phức $E$, các dãy*

$$
0 \to \mathrm{Homgr}_A(E, C') \xrightarrow{\mathrm{Homgr}(1,u)} \mathrm{Homgr}_A(E, C) \xrightarrow{\mathrm{Homgr}(1,v)} \mathrm{Homgr}_A(E, C'') \to 0
$$

$$
0 \to \mathrm{Homgr}_A(C'', E) \xrightarrow{\mathrm{Homgr}(v,1)} \mathrm{Homgr}_A(C, E) \xrightarrow{\mathrm{Homgr}(u,1)} \mathrm{Homgr}_A(C', E) \to 0
$$

*là các dãy khớp của các phức các $k$-môđun.*

Trong trường hợp *a)*, ta nhận xét rằng các dãy

$$
\mathrm{Hom}_A(P_p, C'_q) \to \mathrm{Hom}_A(P_p, C_q) \to \mathrm{Hom}_A(P_p, C''_q)
$$

*và*

$$
\mathrm{Hom}_A(C''_q, E_p) \to \mathrm{Hom}_A(C_q, E_p) \to \mathrm{Hom}_A(C'_q, E_p)
$$

là khớp với mọi $p, q \in \mathbf{Z}$, và ta áp dụng II, p. 10, prop. 5 và II, p. 13, prop. 7. Chứng minh của *b)* là tương tự.

### 2. Các phức của các đồng cấu và các đồng luân

#### Mệnh đề 3 {#alg-x-s5-prop-3 .statement}

*Cho $C, \tilde{C}, C', \tilde{C}'$ là bốn phức $A$, $u : \tilde{C} \to C, v : \tilde{C} \to C, u' : C' \to \tilde{C}'$ và $v' : C' \to \tilde{C}'$ là bốn cấu xạ của các phức.

a) Nếu $u$ và $u'$ đồng luân với $v$ và $v'$ tương ứng, thì hai cấu xạ $\mathrm{Homgr}_A(u, u')$ và $\mathrm{Homgr}_A(v, v')$ từ $\mathrm{Homgr}_A(C, C')$ đến $\mathrm{Homgr}_A(\tilde{C}, \tilde{C}')$ là đồng luân.

b) Nếu $u$ và $u'$ là các cấu xạ đồng luân, thì $\mathrm{Homgr}_A(u, u')$ là một cấu xạ đồng luân.

c) Nếu $C$ hoặc $C'$ đồng luân với không, thì $\mathrm{Homgr}_A(C, C')$ đồng luân với không.*

Ta ký hiệu bởi cùng một chữ $d$ các vi phân của các phức $C$, $C_1$, $C'$, $C'_1$, và bởi $D$ các vi phân của $\mathrm{Homgr}_A(C,C')$ và $\mathrm{Homgr}_A(C_1,C'_1)$. Nếu $u$ (tương ứng $u'$) đồng luân với $v$ (tương ứng $v'$), tồn tại một đồng cấu phân bậc bậc $1$,

$$
w:C_1\to C\qquad\text{(tương ứng }w':C'\to C'_1\text{)}
$$

sao cho

$$
\tag{2}
u-v=dw+wd\qquad\text{(tương ứng }u'-v'=dw'+w'd\text{)}
$$

Gọi $W:\mathrm{Homgr}_A(C,C')\to\mathrm{Homgr}_A(C_1,C'_1)$ là đồng cấu phân bậc bậc $1$ sao cho, với $f\in\mathrm{Homgr}_A(C,C')_n$, $n\in\mathbf{Z}$, ta có

$$
\tag{3}
W(f)=w'fu+(-1)^n v'fw.
$$

Ta có

$$
(DW+WD)(f)=D[w'fu+(-1)^n v'fw]+W[df-(-1)^nfd]
$$

$$
=dw'fu-(-1)^{n+1}w'fud+(-1)^ndv'fw+v'fwd
$$

$$
\qquad+w'dfu+(-1)^{n+1}v'dfw-(-1)^nw'fdu+v'fdw
$$

$$
=(dw'+w'd)fu+v'f(wd+dw)
$$

$$
=(u'-v')fu+v'f(u-v)=u'fu-v'fv;
$$

Điều này được viết là $DW+WD=\mathrm{Homgr}_A(u,u')-\mathrm{Homgr}_A(v,v')$, do đó a).

Ta chứng minh b). Nếu $u$ và $u'$ là các tương đương đồng luân, gọi $\alpha:C\to\widetilde C$ và $\alpha':\widetilde C'\to C'$ là các đồng cấu của các phức sao cho $u\circ\alpha$, $\alpha\circ u$, $u'\circ\alpha'$, $\alpha'\circ u'$ lần lượt đồng luân với $\mathrm{Id}_C$, $\mathrm{Id}_{\widetilde C}$, $\mathrm{Id}_{\widetilde C'}$, $\mathrm{Id}_{C'}$. Khi đó $\mathrm{Homgr}(u,u')\circ\mathrm{Homgr}(\alpha,\alpha')$, bằng với $\mathrm{Homgr}(\alpha\circ u,u'\circ\alpha')$, là đồng luân theo a) với

$$
\mathrm{Homgr}_A(\mathrm{Id}_C,\mathrm{Id}_{C'})=\mathrm{Id}_{\mathrm{Homgr}_A(C,C')};
$$

tương tự $\mathrm{Homgr}(\alpha,\alpha')\circ\mathrm{Homgr}(u,u')$ là đồng luân với $\mathrm{Id}_{\mathrm{Homgr}(\widetilde C,\widetilde C')}$, do đó b).

Cuối cùng c) được suy ra từ b) (áp dụng cho trường hợp $\widetilde C$ hoặc $\widetilde C'$ là không).

#### Hệ quả 1 {#alg-x-s5-prop-3-cor-1 .statement}

Nếu $C$ là tách và $H(C)$ xạ ảnh (tương ứng, nếu $C'$ là tách và $H_n(C')$ đơn ánh với mỗi $n$), thì đồng cấu chính tắc

$$
\lambda(C,C'):\ H(\mathrm{Homgr}_A(C,C'))\to\mathrm{Homgr}_A(H(C),H(C'))
$$

là song ánh.

Giả sử chẳng hạn $C'$ tách và $H(C')$ đơn ánh với mỗi $n$, trường hợp $C$ tách và $H(C)$ xạ ảnh được chứng minh theo một cách tương tự. Theo X, p. 35, def. 6, tồn tại một tương đương đồng luân $u':C'\to H(C')$ ; theo Mệnh đề 3, $\mathrm{Homgr}_A(1,u')$ là một tương đương đồng luân từ $\mathrm{Homgr}_A(C,C')$ lên $\mathrm{Homgr}_A(C,H(C'))$ ; vì

$$
\mathrm{Homgr}_A(1,H(u'))\circ\lambda(C,C')=\lambda(C,H(C'))\circ H(\mathrm{Homgr}_A(1,u'))
$$

và do $\mathrm{Homgr}_A(1,H(u'))$ và $H(\mathrm{Homgr}_A(1,u'))$ là song ánh, nên chỉ cần chứng minh rằng $\lambda(C, H(C'))$ là song ánh, điều này đưa ta trở lại trường hợp $C'$ là đơn ánh và có vi phân không.

Các dãy khớp chính tắc (X, p. 28)

(III) $$
0 \to B(C) \xrightarrow{i} C \xrightarrow{\delta} C/B(C) \to 0
$$
(IV) $$
0 \to H(C) \xrightarrow{j} C/B(C) \xrightarrow{\delta} B(C) \to 0
$$

cho các dãy khớp (X, p. 83, Mệnh đề 2, a))

$$
0 \to \mathrm{Homgr}_A(C/B(C), C') \xrightarrow{l'} \mathrm{Homgr}_A(C, C') \xrightarrow{l} \mathrm{Homgr}_A(B(C), C') \to 0
$$
$$
0 \to \mathrm{Homgr}_A(B(C), C') \xrightarrow{\Delta} \mathrm{Homgr}_A(C/B(C), C') \xrightarrow{j} \mathrm{Homgr}_A(H(C), C') \to 0 .
$$

Vì $d_C = i \circ \delta \circ p$, vi phân $D$ của $\mathrm{Homgr}_A(C, C')$ được cho bởi $D_n = (-1)^{n+1} P_n \circ \Delta_n \circ l_n$; khi đó ta có

$$
\mathrm{Z}(\mathrm{Homgr}_A(C, C')) = \mathrm{Ker}\,(P \circ \Delta \circ I) = \mathrm{Ker}\,I = \mathrm{Im}\,P,
$$
$$
\mathrm{B}(\mathrm{Homgr}_A(C, C')) = \mathrm{Im}\,(P \circ \Delta \circ I) = P(\mathrm{Im}\,\Delta) = P(\mathrm{Ker}\,J) ;
$$

do đó một đẳng cấu $\varphi : H(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H(C), C')$ sao cho, nếu $a \in \mathrm{Homgr}_A(C/B(C), C')$, ảnh của lớp của $P(a)$ qua $\varphi$ là $J(a)$; ta kiểm tra ngay lập tức rằng $\varphi$ trùng với đồng cấu chính tắc $\lambda$.

#### Hệ quả 2 {#alg-x-s5-prop-3-cor-2 .statement}

Giả sử rằng $B(C)$ và $H(C)$ là xạ ảnh (tương ứng, $B_n(C')$ và $H_n(C')$ là đơn ánh với mọi $n$). Khi đó $\lambda(C, C')$ là song ánh.

Thật vậy, khi đó $C$ (tương ứng, $C'$) là tách, theo X, p. 35, Ví dụ 4, và ta áp dụng Hệ quả 1.

#### Hệ quả 3 {#alg-x-s5-prop-3-cor-3 .statement}

Cho $M$ là một $A$-môđun xạ ảnh (tương ứng, một $A$-môđun đơn ánh). Với mọi phức $C$ của các $A$-môđun và mọi số nguyên $n$, đồng cấu chính tắc

$$
H^n(\mathrm{Homgr}_A(M, C)) \to \mathrm{Hom}_A(M, H^n(C))
$$

(tương ứng, $H^n(\mathrm{Homgr}_A(C, M)) \to \mathrm{Hom}_A(H_n(C), M)$) là song ánh.

#### Bổ đề 1 {#alg-x-s5-lem-1 .statement}

a) Nếu $C$ hoặc $C'$ bị chặn về phải, nếu $C$ là xạ ảnh và nếu $H(C') = 0$, thì $H(\mathrm{Homgr}_A(C, C')) = 0$.
    b) Nếu $C$ hoặc $C'$ bị chặn về trái, nếu $C'$ là đơn ánh và nếu $H(C) = 0$, thì $H(\mathrm{Homgr}_A(C, C')) = 0$.

Cho $f \in Z_n(\mathrm{Homgr}_A(C, C'))$; khi đó $f$ là một cấu xạ của các phức từ $C$ đến $C'(n)$; trong trường hợp a) (tương ứng, b)), $f_m$ triệt tiêu với $m$ đủ nhỏ (tương ứng, đủ lớn). Theo X, p. 47, Mệnh đề 1, khi đó $f$ đồng luân với không, do đó thuộc về $B_n(\mathrm{Homgr}_A(C, C'))$, điều này cho kết luận.

#### Mệnh đề 4 {#alg-x-s5-prop-4 .statement}

Cho $u : C' \to C$ là một cấu xạ của các phức, $P$ là một phức xạ ảnh, $E$ là một phức đơn ánh.

a) Nếu $P$ bị chặn bên phải, hoặc nếu $C$ và $C'$ bị chặn bên phải, thì

$$
\operatorname{Homgr}_A(1, u) : \operatorname{Homgr}_A(P, C') \to \operatorname{Homgr}_A(P, C)
$$

là một cấu xạ.

b) Nếu $E$ bị chặn bên trái, hoặc nếu $C$ và $C'$ bị chặn bên trái, thì

$$
\operatorname{Homgr}_A(u, 1) : \operatorname{Homgr}_A(C, E) \to \operatorname{Homgr}_A(C', E)
$$

là một cấu xạ.

Trước hết giả sử rằng $u$ là đơn ánh và đặt $C'' = \operatorname{Coker}\ u$. Vì $u$ là một cấu xạ, $C''$ có đồng điều không. Mặt khác, ta có các dãy khớp (Mệnh đề 2)

Bởi Bổ đề 1, $\operatorname{Homgr}_A(P, C'')$ có đồng điều không trong trường hợp $a$, $\operatorname{Homgr}_A(C'', E)$ có đồng điều không trong trường hợp $b$, do đó có kết luận.

Trong trường hợp tổng quát, tồn tại (X, p. 38, hệ quả của Mệnh đề 7) một phức $\tilde{C}'$, là bị chặn bên phải (tương ứng bị chặn bên trái) khi $C$ và $C'$ là như vậy, một cấu xạ đơn ánh $\tilde{u}: C' \to \tilde{C}'$ và một đồng luân $\beta: \tilde{C}' \to C$ sao cho $u = \beta \circ \tilde{u}$. Khi đó $\tilde{u}$ là một *cấu xạ* (X, p. 34, hệ quả của Mệnh đề 5); theo điều đã chứng minh ở trên, $\operatorname{Homgr}_A(l_P, \tilde{u})$ (tương ứng $\operatorname{Homgr}_A(\tilde{u}, l_E)$) là một cấu xạ trong trường hợp $a$ (tương ứng $b$). Hơn nữa, $\operatorname{Homgr}_A(l_P, \beta)$ (tương ứng $\operatorname{Homgr}_A(\beta, l_E)$) là một đồng luân (Mệnh đề 3); do đó, $\operatorname{Homgr}_A(l_P, u)$ (tương ứng $\operatorname{Homgr}_A(u, l_E)$) là hợp thành của hai cấu xạ, vì vậy là một cấu xạ.

### 3. Định nghĩa và các tính chất đầu tiên của các môđun mở rộng

Với mọi $A$-môđun $E$, ta ký hiệu bởi $p_E : L(E) \to E$ (tương ứng $e_E : E \to I(E)$) phép giải chính tắc tự do (tương ứng đơn ánh), cf. X, p. 50 (tương ứng p. 52).

#### Định nghĩa 1 {#alg-x-s5-def-1 .statement}

Cho $M$ và $N$ là hai $A$-môđun. Môđun các mở rộng của $N$ bởi $M$ là $k$-môđun phân bậc

$$
\text{(4)} \quad \operatorname{Ext}_A(M, N) = H(\operatorname{Homgr}_A(L(M), I(N))) .
$$

Các thành phần thuần nhất của $\operatorname{Ext}_A(M, N)$ được ký hiệu

$$
\text{(5)} \quad \operatorname{Ext}_A^n(M, N) = H^n(\operatorname{Homgr}_A(L(M), I(N))) .
$$

Vì $L(M)$ (tương ứng $I(N)$) là không về bên phải (tương ứng về bên trái), ta có

(6)
$$
\operatorname{Ext}^{n}_{A}(M,N)=0\qquad\text{cho }n<0.
$$

#### Nhận xét 1 {#alg-x-s5-n3-rem-1 .statement}

Ta sẽ thấy dưới đây (X, p. 107, Mệnh đề 6) một số tính chất hữu hạn của các môđun $\operatorname{Ext}^{n}_{A}(M,N)$. Chẳng hạn, nếu $A$ là giao hoán và Noether, và nếu $M$ và $N$ là các $A$-môđun kiểu hữu hạn, thì mỗi $A$-môđun $\operatorname{Ext}^{n}_{A}(M,N)$ là kiểu hữu hạn.

Cho $f : M' \to M$ và $g : N \to N’$ là các đồng cấu của $A$-môđun. Đặt

$$
\operatorname{Ext}_{A}(f,g)=H(\operatorname{Homgr}_{A}(L(f),I(g))) \,;
$$

đây là một đồng cấu bậc 0 của các $k$-môđun phân bậc

$$
\operatorname{Ext}_{A}(f,g):\operatorname{Ext}_{A}(M,N)\to\operatorname{Ext}_{A}(M',N')\,,
$$

các thành phần thuần nhất của nó được ký hiệu

$$
\operatorname{Ext}^{n}_{A}(f,g):\operatorname{Ext}^{n}_{A}(M,N)\to\operatorname{Ext}^{n}_{A}(M',N')\,.
$$

Theo Mệnh đề 1 của [X], p. 82, đồng cấu chính tắc

$$
\lambda^{0}(L(M),I(N)):H^{0}(\operatorname{Homgr}_{A}(L(M),I(N)))
\to\operatorname{Hom}_{A}(H_{0}(L(M)),H^{0}(I(N)))
$$

là song ánh; dùng các đẳng cấu $M\to H_{0}(L(M))$ và $H^{0}(I(N))\to N$, ta suy ra một *đẳng cấu chính tắc*

(7)
$$
\lambda_{M,N}:\operatorname{Ext}^{0}_{A}(M,N)\to\operatorname{Hom}_{A}(M,N)\,.
$$

*Ta sẽ luôn đồng nhất* $\operatorname{Ext}^{0}_{A}(M,N)$ với $\operatorname{Hom}_{A}(M,N)$ qua đẳng cấu này. Khi đó ánh xạ $k$-tuyến tính $\operatorname{Ext}_{A}(f,g)$ có thể được đồng nhất với $\operatorname{Hom}_{A}(f,g)$.

#### Nhận xét 2 {#alg-x-s5-n3-rem-2 .statement}

Cấu xạ của các phức

$$
\operatorname{Homgr}_{A}(p_{M},\epsilon_{N}):\operatorname{Hom}_{A}(M,N)\to\operatorname{Homgr}_{A}(L(M),I(N))
$$

cảm sinh trên đồng điều ở bậc 0 đẳng cấu

$$
\lambda^{-1}_{M,N}:\operatorname{Hom}_{A}(M,N)\to\operatorname{Ext}^{0}_{A}(M,N)
$$

nghịch đảo với $\lambda_{M,N}$.

Ta có $L(1_{M})=1_{L(M)}$, $I(1_{N})=1_{I(N)}$, do đó bằng cách chuyển qua đồng điều

(8)
$$
\operatorname{Ext}_{A}(1_{M},1_{N})=1_{\operatorname{Ext}_{A}(M,N)}\,.
$$

Nếu $f' : M''\to M'$ và $g' : N'\to N''$ là các đồng cấu $A$-môđun, ta có $L(f\circ f')=L(f)\circ L(f')$, $I(g'\circ g)=I(g')\circ I(g)$, và do đó...

(9)
$$
\operatorname{Ext}_{A}(f\circ f',g'\circ g)=\operatorname{Ext}_{A}(f',g')\circ\operatorname{Ext}_{A}(f,g)\,.
$$

Xét các cấu xạ của các $k$-phức
$$
\operatorname{Homgr}_A(L(M), N) \xrightarrow{\operatorname{Homgr}_A(1, e_N)} \operatorname{Homgr}_A(L(M), I(N)) \xleftarrow{\operatorname{Homgr}_A(p_M, 1)} \operatorname{Homgr}_A(M, I(N)),
$$
và các đồng cấu mà chúng cảm sinh trong đồng điều:
$$
H(\operatorname{Homgr}_A(L(M), N)) \xrightarrow{\varphi_{M(N)}} \operatorname{Ext}_A(M, N) \xleftarrow{\overline{\varphi}_{N(M)}} H(\operatorname{Homgr}_A(M, I(N))) .
$$
Theo Mệnh đề 4 của X, p. 86, $\operatorname{Homgr}_A(1, e_N)$ và $\operatorname{Homgr}_A(p_M, 1)$ là các đồng cấu đồng điều, do đó:

#### Mệnh đề 5 {#alg-x-s5-prop-5 .statement}

*Các $k$-đồng cấu*
$$
\begin{aligned}
&\varphi_M(N) : H(\operatorname{Homgr}_A(L(M), N)) \to \operatorname{Ext}_A(M, N) \\
&\text{và } \quad \overline{\varphi}_N(M) : H(\operatorname{Homgr}_A(M, I(N))) \to \operatorname{Ext}_A(M, N) \text{ là song ánh}.
\end{aligned}
$$

#### Hệ quả {#alg-x-s5-n3-cor-1 .statement}

Nếu $M$ là xạ ảnh (tương ứng, nếu $N$ là đơn ánh), thì $\operatorname{Ext}_A^i(M, N) = 0$ với $i > 0$.
Thật vậy, $\operatorname{Homgr}_A(1, e_N) : \operatorname{Hom}_A(M, N) \to \operatorname{Homgr}_A(M, I(N))$ (tương ứng, $\operatorname{Homgr}_A(p_M, 1) : \operatorname{Hom}_A(M, N) \to \operatorname{Homgr}_A(L(M), N)$) khi đó là một đồng cấu đồng điều (X, p. 86, Mệnh đề 4), suy ra kết luận.

*Các nhận xét. — 3)* Cho $g : N \to N'$ là một đồng cấu của các $A$-môđun. Khi đó
$$
\operatorname{Homgr}_A(1_{L(M)}, g) \circ \operatorname{Homgr}_A(1_{L(M)}, e_N) = \operatorname{Homgr}_A(1_{L(M)}, e_{N'}) \circ \operatorname{Homgr}_A(1_{L(M)}, I(g)),
$$
và do đó biểu đồ
$$
\begin{array}{ccc}
H(\operatorname{Homgr}_A(L(M), N)) & \xrightarrow{\varphi_{M(N)}} & \operatorname{Ext}_A(M, N) \\
\operatorname{H}(\operatorname{Homgr}_A(1_{L(M)}, g)) \downarrow & & \downarrow \operatorname{Ext}_A(1_M, g) \\
H(\operatorname{Homgr}_A(L(M), N')) & \xrightarrow{\varphi_{M(N')}} & \operatorname{Ext}_A(M, N')
\end{array}
$$
là giao hoán.

4) Tương tự, nếu $f : M' \to M$ là một đồng cấu của các $A$-môđun, biểu đồ
$$
\begin{array}{ccc}
H(\operatorname{Homgr}_A(M, I(N))) & \xrightarrow{\overline{\varphi}_{N(M)}} & \operatorname{Ext}_A(M, N) \\
\operatorname{H}(\operatorname{Homgr}_A(f, 1_{I(N)})) \downarrow & & \downarrow \operatorname{Ext}_A(f, 1_N) \\
H(\operatorname{Homgr}_A(M', I(N))) & \xrightarrow{\overline{\varphi}_{N(M')}} & \operatorname{Ext}_A(M', N)
\end{array}
$$
là giao hoán.

#### Mệnh đề 6 {#alg-x-s5-prop-6 .statement}

Ánh xạ $(f,g) \mapsto \operatorname{Ext}_A(f,g) :$
$$
\operatorname{Hom}_A(M',M)\times\operatorname{Hom}_A(N,N')\longrightarrow
\operatorname{Homgr}_k\bigl(\operatorname{Ext}_A(M,N),\operatorname{Ext}_A(M',N')\bigr)
$$
là $k$-song tuyến tính.

Cho $f\in\operatorname{Hom}_A(M',M)$, $g_1,g_2\in\operatorname{Hom}_A(N,N')$, $\lambda_1,\lambda_2\in k$. Các cấu xạ $\operatorname{Homgr}_A(L(f),\lambda_1g_1+\lambda_2g_2)$ và $\lambda_1\operatorname{Homgr}_A(L(f),g_1)+\lambda_2\operatorname{Homgr}_A(L(f),g_2)$ từ $\operatorname{Homgr}_A(L(M),N)$ đến $\operatorname{Homgr}_A(L(M),N')$ trùng nhau, do đó, theo Mệnh đề 5 và Nhận xét 3,

(10)     $\operatorname{Ext}_A(f,\lambda_1g_1+\lambda_2g_2)=\lambda_1\operatorname{Ext}_A(f,g_1)+\lambda_2\operatorname{Ext}_A(f,g_2)$.

Lập luận tương tự đối với ánh xạ $f \mapsto \operatorname{Ext}_A(f,g)$.

#### Hệ quả {#alg-x-s5-n3-cor-2 .statement}

Cho $\lambda \in k$. Nếu $\lambda$ triệt tiêu $M$ hoặc $N$, thì nó triệt tiêu $\operatorname{Ext}_A(M,N)$. Thật vậy, $\lambda \cdot 1_{\operatorname{Ext}_A(M,N)} = \operatorname{Ext}_A(\lambda 1_M, 1_N) = \operatorname{Ext}_A(1_M, \lambda 1_N)$.

#### Mệnh đề 7 {#alg-x-s5-prop-7 .statement}

Cho $I$ và $J$ là hai tập hợp, $(M_\alpha)_{\alpha\in I}$ và $(N_\beta)_{\beta\in J}$ là hai họ các $A$-môđun; đồng cấu
$$
\operatorname{Ext}_A\left(\bigoplus_{\alpha\in I}M_\alpha,\prod_{\beta\in J}N_\beta\right)
\longrightarrow
\prod_{\substack{\beta\in J,\ \alpha\in I}}
\operatorname{Ext}_A(M_\alpha,N_\beta)
$$
cảm sinh bởi các đồng cấu chính tắc $M_\alpha \to \bigoplus_{\alpha\in I} M_\alpha$ và $\prod_{\beta\in J} N_\beta \to N_\beta$ là song ánh.

Chỉ cần chứng minh rằng với mọi $A$-môđun $M$ (tương ứng $N$), các đồng cấu
$$
\operatorname{Ext}(M, \prod_\beta N_\beta) \to \prod_\beta \operatorname{Ext}(M,N_\beta)
$$
(tương ứng $\operatorname{Ext}(\bigoplus M_\alpha,N)\to\prod_\alpha\operatorname{Ext}(M_\alpha,N)$)
là song ánh. Điều này suy ra từ những gì đã được chứng minh, từ Mệnh đề 1 của X, p. 28, và các đẳng cấu chính tắc $\operatorname{Homgr}_A(L(M), \prod N_\beta) \to \prod \operatorname{Homgr}_A(L(M),N_\beta)$ và $\operatorname{Homgr}_A(\bigoplus M_\alpha, I(N)) \to \prod \operatorname{Homgr}_A(M_\alpha, I(N))$.

#### Nhận xét 5 {#alg-x-s5-n3-rem-5 .statement}

Cho $P^\circ$ và $Q^\circ$ là hai $A$-môđun phải. Ta định nghĩa $\operatorname{Ext}_A(P,Q)$ bởi

$$
\operatorname{Ext}_A(P,Q)=H(\operatorname{Homgr}_A(L(P),I(Q)))=H(\operatorname{Homgr}_{A^\circ}(L(P^\circ),I(Q^\circ)))
$$

$$
=\operatorname{Ext}_{A^\circ}(P^\circ,Q^\circ).
$$

Tất cả các định nghĩa và mệnh đề của đoạn này do đó áp dụng cho các $A$-môđun phải bằng cách xem chúng như các môđun trái trên vành $A^\circ$.

### 4. Các đồng cấu nối và các dãy khớp

Cho $M$ là một $A$-môđun. Nhắc lại rằng với mọi $A$-môđun $N$, trong số trước ta đã định nghĩa một đẳng cấu các $k$-môđun

$$
\varphi_M(N):H(\operatorname{Homgr}_A(L(M),N))\longrightarrow\operatorname{Ext}_A(M,N).
$$

Đặt

$$(\mathcal{E})\qquad 0\longrightarrow N'\xrightarrow{u}N\xrightarrow{v}N''\longrightarrow0$$

là một dãy khớp các $A$-môđun; dãy các phức $k$

$$
(\mathcal{E}) \quad 0 \longrightarrow \operatorname{Homgr}_A(L(M), N') \xrightarrow{\operatorname{Homgr}(1,u)} \operatorname{Homgr}_A(L(M), N) \\
\phantom{(M\mathcal{E})} \phantom{0} \xrightarrow{\operatorname{Homgr}(1,v)} \operatorname{Homgr}_A(L(M), N'') \longrightarrow 0
$$

là khớp ($X$, p. 83, mệnh đề 2, $a$), gọi

$$
\partial_{(M\mathcal{E})} : H(\operatorname{Homgr}_A(L(M), N'')) \to H(\operatorname{Homgr}_A(L(M), N'))
$$

là đồng cấu nối tương ứng ($X$, p. 29).

#### Định nghĩa 2 {#alg-x-s5-def-2 .statement}

*Ta gọi đồng cấu hợp thành là đồng cấu nối của các môđun mở rộng tương đối với môđun $M$ và với dãy khớp $\mathcal{E}$*

$$
\delta(M, \mathcal{E}) = \varphi_M(N') \circ \partial_{(M\mathcal{E})} \circ \varphi_M(N'')^{-1} : \operatorname{Ext}_A(M, N'') \to \operatorname{Ext}_A(M, N')
$$

Đây là một $k$-đồng cấu phân bậc có bậc tăng 1, các thành phần thuần nhất của nó được ký hiệu $\delta^n(M, \mathcal{E}) : \operatorname{Ext}_A^n(M, N'') \to \operatorname{Ext}_A^{n+1}(M, N')$.

#### Định lý 1 {#alg-x-s5-thm-1 .statement}

*Dãy phải không bị chặn của các đồng cấu các $k$-môđun*

$$
0 \longrightarrow \operatorname{Hom}_A(M, N') \xrightarrow{\operatorname{Hom}(1,u)} \operatorname{Hom}_A(M, N) \xrightarrow{\operatorname{Hom}(1,v)} \operatorname{Hom}_A(M, N'')
$$
$$
\phantom{0} \xrightarrow{\delta_{(M,\mathcal{E})}} \operatorname{Ext}_A^1(M, N') \to \cdots \xrightarrow{\delta^{n-1}(M,\mathcal{E})} \operatorname{Ext}_A^n(M, N') \xrightarrow{\operatorname{Ext}^n(1,u)} \operatorname{Ext}_A^n(M, N)
$$
$$
\phantom{0} \xrightarrow{\operatorname{Ext}^n(1,v)} \operatorname{Ext}_A^n(M, N'') \xrightarrow{\delta^n(M,\mathcal{E})} \operatorname{Ext}_A^{n+1}(M, N') \to \cdots
$$

*là khớp*.

Xét thực sự biểu đồ ở trang X.91.
Nó giao hoán theo *nhận xét* 3 của $X$, p. 88 và định nghĩa 2; hơn nữa hàng dưới là khớp ($X$, p. 30, định lý 1), và các mũi tên đứng là song ánh ($X$, p. 88, mệnh đề 5).

#### Hệ quả {#alg-x-s5-n4-cor-1 .statement}

*Nếu* $\operatorname{Ext}_A^1(M, N') = 0$, *dãy*

$$
0 \longrightarrow \operatorname{Hom}_A(M, N') \xrightarrow{\operatorname{Hom}(1,u)} \operatorname{Hom}_A(M, N) \xrightarrow{\operatorname{Hom}(1,v)} \operatorname{Hom}_A(M, N'') \longrightarrow 0
$$

*là khớp*.

#### Mệnh đề 8 {#alg-x-s5-prop-8 .statement}

*Cho* $f : M_1 \to M$ *là một đồng cấu các* $A$*-môđun* và

$$
\begin{array}{cccccccccc}
(\mathcal{E}) & 0 & \longrightarrow & N' & \xrightarrow{u} & N & \xrightarrow{v} & N'' & \longrightarrow & 0 \\
& & & g' \downarrow & & g \downarrow & & g'' \downarrow & & \\
(\mathcal{E}_1) & 0 & \longrightarrow & N'_1 & \xrightarrow{u_1} & N_1 & \xrightarrow{v_1} & N''_1 & \longrightarrow & 0
\end{array}
$$

$$
\begin{array}{ccccc}
\operatorname{Ext}(M,N') & \xrightarrow{\operatorname{Ext}(1,u)} & \operatorname{Ext}(M,N) & \xrightarrow{\operatorname{Ext}(1,v)} & \operatorname{Ext}(M,N'') \xrightarrow{\delta(M,\mathcal{G})} \operatorname{Ext}(M,N') \xrightarrow{\operatorname{Ext}(1,u)} \operatorname{Ext}(M,N)\\[6pt]
\Big\uparrow\vcenter{\rlap{$\scriptstyle\varphi_M(N')$}} && \Big\uparrow\vcenter{\rlap{$\scriptstyle\varphi_M(N)$}} && \Big\uparrow\vcenter{\rlap{$\scriptstyle\varphi_M(N'')$}} \qquad\qquad\Big\uparrow\vcenter{\rlap{$\scriptstyle\varphi_M(N')$}}\\[6pt]
H(\operatorname{Homgr}(L(M),N')) & \xrightarrow{H(\operatorname{Homgr}(1,u))} & H(\operatorname{Homgr}(L(M),N)) & \xrightarrow{H(\operatorname{Homgr}(1,v))} & H(\operatorname{Homgr}(L(M),N'')) \xrightarrow{\partial(M\mathcal{G})} H(\operatorname{Homgr}(L(M),N')) \xrightarrow{H(\operatorname{Homgr}(1,u))} H(\operatorname{Homgr}(L(M),N))
\end{array}
$$

là một biểu đồ giao hoán các $A$-môđun với các hàng khớp. Biểu đồ các $k$-môđun

$$
\begin{array}{ccc}
\mathrm{Ext}_A(M, N'') & \xrightarrow{\delta(M, \mathscr{E})} & \mathrm{Ext}_A(M, N') \\
\mathrm{Ext}(f, g'') \downarrow & & \mathrm{Ext}(f, g') \downarrow \\
\mathrm{Ext}_A(M_1, N''_1) & \xrightarrow{\delta(M, \mathscr{E}_1)} & \mathrm{Ext}_A(M_1, N'_1)
\end{array}
$$

là giao hoán.
Điều này suy ra từ X, p. 31, mệnh đề 2 áp dụng cho biểu đồ giao hoán

$$
\begin{array}{ccccccccc}
& & \mathrm{Homgr}(1, u) & & & & \mathrm{Homgr}(1, v) & & \\
0 \to \mathrm{Homgr}_A(L(M), N') & \to & \mathrm{Homgr}_A(L(M), N) & \to & \mathrm{Homgr}_A(L(M), N'') & \to & 0 \\
\mathrm{Homgr}(L(f), g') \downarrow & & \mathrm{Homgr}(L(f), g) \downarrow & & \mathrm{Homgr}(L(f), g'') \downarrow & & \\
0 \to \mathrm{Homgr}_A(L(M_1), N'_1) & \to & \mathrm{Homgr}_A(L(M_1), N_1) & \to & \mathrm{Homgr}_A(L(M_1), N''_1) & \to & 0
\end{array}
$$

Cho $N$ là một $A$-môđun, và
$$(\mathcal{F})$$
$$0 \to M' \xrightarrow{r} M \xrightarrow{s} M'' \to 0$$
là một dãy khớp của các $A$-môđun; dãy các phức
$$(\mathcal{F}_N)$$
$$0 \longrightarrow \mathrm{Homgr}_A(M'', I(N)) \xrightarrow{\mathrm{Homgr}(s, 1)} \mathrm{Homgr}_A(M, I(N))$$
$$\xrightarrow{\mathrm{Homgr}(r, 1)} \mathrm{Homgr}_A(M', I(N)) \longrightarrow 0$$
là khớp (X, p. 83, mệnh đề 2, $a$) ; đặt
$$\partial(\mathcal{F}_N) : \mathrm{H}(\mathrm{Homgr}_A(M', I(N))) \to \mathrm{H}(\mathrm{Homgr}_A(M'', I(N)))$$
là đồng cấu nối tương ứng.

#### Định nghĩa 3 {#alg-x-s5-def-3 .statement}

Ta gọi đồng cấu nối của các môđun mở rộng tương ứng với dãy khớp $(\mathcal{F})$ và với môđun $N$, là đồng cấu hợp thành
$$\delta(\mathcal{F}, N) : \overline{\varphi}_N(M'') \circ \partial(\mathcal{F}_N) \circ \overline{\varphi}_N(M')^{-1} : \mathrm{Ext}_A(M', N) \to \mathrm{Ext}_A(M'', N).$$
Nó là một $k$-đồng cấu phân bậc có bậc tăng 1, các thành phần thuần nhất của nó được ký hiệu là $\delta^n(\mathcal{F}, N) : \mathrm{Ext}_A^n(M', N) \to \mathrm{Ext}_A^{n+1}(M'', N)$.
Khi đó ta chứng minh như trên các mệnh đề sau:

#### Định lý 2 {#alg-x-s5-thm-2 .statement}

Dãy phải không bị chặn của các đồng cấu của các $k$-môđun
$$0 \longrightarrow \mathrm{Hom}_A(M'', N) \xrightarrow{\mathrm{Hom}(s, 1)} \mathrm{Hom}_A(M, N) \xrightarrow{\mathrm{Hom}(r, 1)} \mathrm{Hom}_A(M', N)$$
$$\xrightarrow{\delta^0(\mathcal{F}, N)} \mathrm{Ext}_A^1(M'', N) \to \cdots \xrightarrow{\delta^{n-1}(\mathcal{F}, N)} \mathrm{Ext}_A^n(M'', N) \xrightarrow{\mathrm{Ext}^n(s, 1)} \mathrm{Ext}_A^n(M, N)$$
$$\xrightarrow{\mathrm{Ext}^n(r, 1)} \mathrm{Ext}_A^n(M', N) \xrightarrow{\delta^n(\mathcal{F}, N)} \mathrm{Ext}_A^{n+1}(M'', N) \to \cdots$$
là khớp.

#### Hệ quả {#alg-x-s5-n4-cor-2 .statement}

Nếu $\operatorname{Ext}_A^1(M'', N) = 0$, dãy

$$
0 \longrightarrow \operatorname{Hom}_A(M'', N) \xrightarrow{\operatorname{Hom}(s, 1)} \operatorname{Hom}_A(M, N) \xrightarrow{\operatorname{Hom}(r, 1)} \operatorname{Hom}_A(M', N) \longrightarrow 0
$$

là khớp.

#### Mệnh đề 9 {#alg-x-s5-prop-9 .statement}

Cho $g : N \to N_1$ là một đồng cấu của các $A$-môđun và

$$
\begin{array}{cccccc}
(\mathcal{F}_1) & 0 \to M'_1 \xrightarrow{r_1} M_1 \xrightarrow{s_1} M''_1 \to 0 \\
& f' \downarrow & f \downarrow & f'' \downarrow \\
(\mathcal{F}) & 0 \to M' \xrightarrow{r} M \xrightarrow{s} M'' \to 0
\end{array}
$$

là một biểu đồ giao hoán của các $A$-môđun với các hàng khớp. Biểu đồ của các $k$-môđun

$$
\begin{array}{ccc}
\operatorname{Ext}_A(M', N) & \xrightarrow{\delta(\mathcal{F}, N)} & \operatorname{Ext}_A(M'', N) \\
\operatorname{Ext}_A(f', g) \downarrow & & \operatorname{Ext}_A(f'', g) \downarrow \\
\operatorname{Ext}_A(M'_1, N_1) & \xrightarrow{\delta(\mathcal{F}_1, N_1)} & \operatorname{Ext}_A(M''_1, N_1)
\end{array}
$$

là giao hoán.

### 5. Các môđun xạ ảnh, các môđun đơn ánh và các môđun mở rộng

#### Mệnh đề 10 {#alg-x-s5-prop-10 .statement}

Cho $M$ là một $A$-môđun. Các điều kiện sau là tương đương:

(i) $M$ là xạ ảnh.
(ii) $\operatorname{Ext}_A^i(M, N) = 0$ với mọi $A$-môđun $N$ và với mọi số nguyên $i > 0$.
(iii) $\operatorname{Ext}_A^1(M, N) = 0$ với mọi $A$-môđun $N$.
(iv) Tồn tại một dãy khớp

$$
0 \to K \xrightarrow{\nu} P \xrightarrow{\iota} M \to 0,
$$

trong đó $P$ là xạ ảnh, và $\operatorname{Ext}_A^1(M, K) = 0$.

(i) $\Rightarrow$ (ii) : đây là hệ quả của mệnh đề 5 của X, p. 88.
(ii) $\Rightarrow$ (iii) : điều này là tầm thường.
(iii) $\Rightarrow$ (iv) : điều này là hiển nhiên vì $M$ là thương của một môđun tự do $P$.
(iv) $\Rightarrow$ (i) : vì $\operatorname{Ext}_A^1(M, K) = 0$, ánh xạ chính tắc

$$
\operatorname{Hom}_A(M, P) \to \operatorname{Hom}_A(M, M)
$$

là toàn ánh (X, p. 90, hệ quả); do đó tồn tại một tiết diện $A$-tuyến tính của $\nu$ và $M$ đẳng cấu với một nhân tử trực tiếp của $P$, và vì vậy là xạ ảnh.

#### Mệnh đề 11 {#alg-x-s5-prop-11 .statement}

Cho $N$ là một $A$-môđun. Các điều kiện sau là tương đương:

(i) $N$ là đơn ánh.
(ii) $\operatorname{Ext}_A^i(M, N) = 0$ với mọi $A$-môđun $M$ và mọi số nguyên $i > 0$.

(iii) $\mathrm{Ext}_A^1(M, N) = 0$ với mọi $A$-môđun $M$.

(iv) Tồn tại một dãy khớp

$$
0 \to N \xrightarrow{u} I \xrightarrow{v} C \to 0,
$$

trong đó $I$ là đơn ánh và $\mathrm{Ext}_A^1(C, N) = 0$;

(v) $\mathrm{Ext}_A^1(M, N) = 0$ với mọi $A$-môđun xyclic $M$.

(i) $\Rightarrow$ (ii) : đây là hệ quả của Mệnh đề 5 của X, p. 88.

(ii) $\Rightarrow$ (iii) $\Rightarrow$ (v) : điều này là tầm thường.

(iii) $\Rightarrow$ (iv) : điều này là rõ ràng vì $N$ là một môđun con của một môđun đơn ánh (X, p. 19, Hệ quả 3).

(iv) $\Rightarrow$ (i) : vì $\mathrm{Ext}_A^1(C, N) = 0$, đồng cấu chính tắc

$$
\mathrm{Hom}_A(I, N) \to \mathrm{Hom}_A(N, N)
$$

là toàn ánh (X, p. 93, Hệ quả); do đó tồn tại một phép co rút tuyến tính trên $A$ của $u$ và $N$ đẳng cấu với một nhân tử trực tiếp của $I$, suy ra nó là đơn ánh (X, p. 16, Mệnh đề 9).

(v) $\Rightarrow$ (i) : nếu $\alpha$ là một iđêan của $A$, ta có $\mathrm{Ext}_A^1(A/\alpha, N) = 0$; ánh xạ chính tắc $\mathrm{Hom}_A(A, N) \to \mathrm{Hom}_A(\alpha, N)$ do đó là toàn ánh và $N$ là đơn ánh (X, p. 16, Mệnh đề 10).

### 6. Công thức hệ số phổ quát

Trong số này, ta xét hai phức của các $A$-môđun $(C, d)$ và $(C', d')$. Ta xét các dãy khớp chính tắc:

(I)

$$
0 \to Z(C) \xrightarrow{j} C \xrightarrow{\delta} B(C)(-1) \to 0,
$$

(II_p)

$$
0 \to B_p(C) \xrightarrow{i} Z_p(C) \xrightarrow{\rho} H_p(C) \to 0;
$$

từ $\delta$ ta suy ra một $k$-đồng cấu

$$
H(\mathrm{Homgr}(\delta, 1)) : H(Homgr_A(B(C), C'))(1) \to H(Homgr_A(C, C'));
$$

từ (II_p) ta suy ra các đồng cấu liên kết:

$$
\delta(11_p, H^q(C')) : \mathrm{Hom}_A(B_p(C), H^q(C')) \to \mathrm{Ext}_A^1(H_p(C), H^q(C')) .
$$

do đó, bằng cách chuyển qua tích, các đồng cấu của các $k$-môđun

$$
\varphi^n : \mathrm{Homgr}_A^n(B(C), H(C')) \to \prod_{p+q=n} \mathrm{Ext}_A^1(H_p(C), H^q(C'))
$$

Ta cũng có các đồng cấu chính tắc (X, p. 82)

$$
\lambda^n(B(C), C') : H^n(Homgr_A(B(C), C')) \to \mathrm{Homgr}_A^n(B(C), H(C')) .
$$

Với các ký hiệu này:

#### Định lý 3 {#alg-x-s5-thm-3 .statement}

Giả sử các $A$-môđun $B(C)$ và $Z(C)$ là xạ ảnh. Với mỗi $n$, tồn tại một đồng cấu duy nhất của các $k$-môđun

$$
\beta^n : \prod_{p+q=n-1} \mathrm{Ext}_A^1(H_p(C), H^q(C')) \to H^n(\mathrm{Homgr}_A(C, C'))
$$

làm cho biểu đồ

$$
\begin{array}{ccc}
\mathrm{Homgr}_A^{n-1}(B(C), H(C')) & \xleftarrow{\lambda^{n-1}(B(C), C')} & H^{n-1}(\mathrm{Homgr}_A(B(C), C')) \\
\downarrow \varphi^{n-1} & & \downarrow H^n(\mathrm{Homgr}(\delta, 1)) \\
\prod_{p+q=n-1} \mathrm{Ext}_A^1(H_p(C), H^q(C')) & \xrightarrow{\beta^n} & H^n(\mathrm{Homgr}_A(C, C')) .
\end{array}
$$

giao hoán.

Các dãy của các $k$-môđun phân bậc

(11) $0 \to \prod_{p+q=n-1} \mathrm{Ext}_A^1(H_p(C), H^q(C')) \xrightarrow{\beta^n} H^n(\mathrm{Homgr}_A(C, C'))$

$$
\xrightarrow{\lambda^n(C, C')} \prod_{p+q=n} \mathrm{Hom}_A(H_p(C), H^q(C')) \to 0
$$

là khớp.

#### Nhận xét {#alg-x-s5-n6-rem-1 .statement}

Người ta có thể chứng minh một mệnh đề tương tự, giả sử $B_n(C')$ và $C'/B_n(C')$ là đơn ánh với mỗi $n$.

Đặt, cho đơn giản, $B = B(C)$, $Z = Z(C)$, $H = H(C)$ và $H' = H(C')$. Vì $B$ là xạ ảnh, ta suy ra từ (1) một dãy khớp

(12) $0 \to \mathrm{Homgr}_A(B, C')(1) \xrightarrow{\mathrm{Homgr}(\delta, 1)} \mathrm{Homgr}_A(C, C')$

$$
\xrightarrow{\mathrm{Homgr}(i, 1)} \mathrm{Homgr}_A(Z, C') \to 0 .
$$

#### Bổ đề 2 {#alg-x-s5-lem-2 .statement}

Đồng cấu nối

$$
H^n(\mathrm{Homgr}_A(Z, C')) \to H^n(\mathrm{Homgr}_A(B, C'))
$$

liên kết với (12) bằng $(-1)^{n+1} H(\mathrm{Homgr}(i, 1))$.

Chứng minh. Thật vậy, cho $a \in Z^n(\mathrm{Homgr}_A(Z, C'))$; đây là một cấu xạ của các phức có bậc tăng $n$ từ $Z$ đến $C'$, do đó các giá trị của nó nằm trong $Z(C')$. Vì dãy khớp (1) là tách ($B$ là xạ ảnh), $a$ mở rộng thành một phần tử $b$ của $\mathrm{Homgr}_A^n(C, Z(C'))$. Theo định nghĩa, ảnh của lớp của $a$ qua đồng cấu nối đang xét là lớp trong $H^n(\mathrm{Homgr}_A(B, C'))$ của đồng cấu $u$ từ $B(C)$ đến $C'$ sao cho với $x \in C$, ta có

$$
u(dx) = Db(x) = d'b(x) - (-1)^n b(dx) = (-1)^{n+1} b(dx) = (-1)^{n+1} a(dx),
$$

do đó có mệnh đề.

Dãy khớp đồng điều liên kết với (12) do đó cho dãy khớp
→ H^n(\mathrm{Homgr}_A(Z, C')) \xrightarrow{\mathrm{H}(\mathrm{Homgr}(i,1))} H^n(\mathrm{Homgr}_A(B, C'))
\xrightarrow{\mathrm{H}(\mathrm{Homgr}(\delta,1))} H^{n+1}(\mathrm{Homgr}_A(C, C')) \xrightarrow{\mathrm{H}(\mathrm{Homgr}(j,1))} H^{n+1}(\mathrm{Homgr}_A(Z, C')) \to \ldots .

Hơn nữa, vì $Z$ là xạ ảnh, ta thu được từ (II_p) các dãy khớp
0 \to \mathrm{Hom}_A(H_p, H'^q) \to \mathrm{Hom}_A(Z_p, H'^q) \to \mathrm{Hom}_A(B_p, H'^q) \to \mathrm{Ext}_A^1(H_p, H'^q) \to 0 ,
do đó, bằng cách chuyển qua các tích, các dãy khớp
0 \to \mathrm{Homgr}_A^n(H, H') \to \mathrm{Homgr}_A^n(Z, H') \to \mathrm{Homgr}_A^n(B, H')
\to \prod_{p+q=n} \mathrm{Ext}_A^1(H_p, H'^q) \to 0 .
Cuối cùng, ta có các đồng cấu chính tắc của No. 1:
$$
\begin{align*}
\lambda_B &= \lambda(B, C') : \mathrm{H}(\mathrm{Homgr}_A(B, C')) \to \mathrm{Homgr}_A(B, H') , \\
\lambda_Z &= \lambda(Z, C') : \mathrm{H}(\mathrm{Homgr}_A(Z, C')) \to \mathrm{Homgr}_A(Z, H') , \\
\lambda_C &= \lambda(C, C') : \mathrm{H}(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H, H') ,
\end{align*}
$$
do đó có biểu đồ với các hàng khớp ở trang X.97.

Biểu đồ này giao hoán theo phép dựng các đồng cấu $\lambda$. Hơn nữa, vì các phức $B$ và $Z$ là tách và xạ ảnh, $\lambda_B$ và $\lambda_Z$ là song ánh ($\lambda$, p. 84, hệ quả 1). Từ đó suy ra, một mặt, $\lambda_C^n$ là toàn ánh, với hạt nhân bằng $\mathrm{Im}\ H^n(\mathrm{Homgr}(\delta, 1))$, và mặt khác, $\varphi^{n-1} \circ \lambda_B^{n-1}$ là toàn ánh, với hạt nhân bằng $\mathrm{Ker}\ H^n(\mathrm{Homgr}(\delta, 1))$. Định lý suy ra ngay lập tức từ đó.

#### Hệ quả 1 {#alg-x-s5-lem-2-cor-1 .statement}

Giả sử $B(C)$ và $Z(C)$ xạ ảnh và $B^n(C')$ đơn ánh với mỗi $n$. Khi đó các dãy khớp (11) là tách.
Điều này suy ra từ định lý và bổ đề sau:

#### Bổ đề 3 {#alg-x-s5-lem-3 .statement}

Nếu $B(C)$ là xạ ảnh và $B_n(C')$ đơn ánh với mỗi $n$, đồng cấu chính tắc $\lambda(C, C') : \mathrm{H}(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C'))$ có một tiết diện tuyến tính $k$.

Thật vậy, theo X, p. 35, các nhận xét a) và b), tồn tại các đồng luân
$$
\varphi : C \to \mathrm{H}(C) \quad \text{and} \quad \varphi' : \mathrm{H}(C') \to C'
$$
sao cho $\mathrm{H}(\varphi) = 1_{\mathrm{H}(C)}$ và $\mathrm{H}(\varphi') = 1_{\mathrm{H}(C')}$.
Trong biểu đồ giao hoán
$$
\begin{array}{ccc}
\mathrm{H}(\mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C'))) & \xrightarrow{\mathrm{H}(\mathrm{Homgr}(\varphi, \varphi'))} & \mathrm{H}(\mathrm{Homgr}_A(C, C')) \\
\lambda(\mathrm{H}(C), \mathrm{H}(C')) \downarrow & & \downarrow \lambda(C, C') \\
\mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C')) & \xrightarrow{\mathrm{Homgr}(\mathrm{H}(\varphi), \mathrm{H}(\varphi'))} & \mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C')) ,
\end{array}
$$
$\lambda(\mathrm{H}(C), \mathrm{H}(C'))$ là song ánh và $\mathrm{Homgr}(\mathrm{H}(\varphi), \mathrm{H}(\varphi'))$ là đồng nhất, do đó có mệnh đề.

$$
\begin{array}{ccccccccc}
\operatorname{Homgr}_{A}^{n-1}(Z,H')&
\xrightarrow{\operatorname{Homgr}^{n-1}(i,1)}&
\operatorname{Homgr}_{A}^{n-1}(B,H')&
\xrightarrow{\varphi^{n-1}}&
\displaystyle\prod_{p+q=n-1}\operatorname{Ext}^{1}(H_p,H^q)&
\longrightarrow&0
\\[2ex]
\uparrow\scriptstyle{\lambda_Z^{n-1}}&&
\uparrow\scriptstyle{\lambda_B^{n-1}}&&&&
\\[-1ex]
H^{n-1}(\operatorname{Homgr}_{A}(Z,C'))&
\xrightarrow{H^{n-1}(\operatorname{Homgr}(i,1))}&
H^{n-1}(\operatorname{Homgr}_{A}(B,C'))&
\xrightarrow{H^n(\operatorname{Homgr}(\delta,1))}&
H^n(\operatorname{Homgr}_{A}(C,C'))&
\xrightarrow{H^n(\operatorname{Homgr}(j,1))}&
H^n(\operatorname{Homgr}_{A}(Z,C'))&
\xrightarrow{H^n(\operatorname{Homgr}(i,1))}&
H^n(\operatorname{Homgr}_{A}(B,C'))
\\[2ex]
&&&&
\uparrow\scriptstyle{\lambda_C^n}&&
\uparrow\scriptstyle{\lambda_Z^n}&&
\uparrow\scriptstyle{\lambda_B^n}
\\[-1ex]
&&&
0\longrightarrow&
\operatorname{Homgr}_{A}^{n}(H,H')&
\xrightarrow{\operatorname{Homgr}^{n}(j,1)}&
\operatorname{Homgr}_{A}^{n}(Z,H')&
\xrightarrow{\operatorname{Homgr}^{n}(i,1)}&
\operatorname{Homgr}_{A}^{n}(B,H')
\end{array}
$$

#### Hệ quả 2 {#alg-x-s5-lem-3-cor-2 .statement}

Nếu $B(C)$ và $Z(C)$ là xạ ảnh, thì với mọi $A$-môđun $N$ và mọi số nguyên $n$, ta có một dãy khớp tách:

(13) $0 \longrightarrow \mathrm{Ext}_A^1(H_{n-1}(C), N) \xrightarrow{\beta^n} H^n(\mathrm{Homgr}_A(C, N)) \xrightarrow{\lambda^n} \mathrm{Hom}_A(H_n(C), N) \longrightarrow 0$.

#### Hệ quả 3 (« công thức hệ số phổ quát ») {#alg-x-s5-lem-3-cor-3 .statement}

Giả sử $A$ là chính và $C$ tự do. Với mọi $A$-môđun $N$ và mọi số nguyên $n$, ta có một dãy khớp tách (13).
Thật vậy, $B(C)$ và $Z(C)$ là tự do như các môđun con của môđun tự do $C$ (VII. § 3, hệ quả 2 của định lý 1).

#### Hệ quả 4 {#alg-x-s5-lem-3-cor-4 .statement}

Nếu $C$ bị chặn về bên phải và nếu $C$ và $H(C)$ là xạ ảnh, thì

$$
\lambda(C, C') : H(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H(C), H(C'))
$$

là song ánh.
Theo định lý, chỉ cần chứng minh rằng $B(C)$ và $Z(C)$ là xạ ảnh. Ta có các dãy khớp

$$
\begin{align*}
0 &\to B_n(C) \to Z_n(C) \to H_n(C) \to 0 \\
0 &\to Z_n(C) \to C_n \to B_{n-1}(C) \to 0,
\end{align*}
$$

do đó $(B_{n-1}(C) \text{ là xạ ảnh}) \Rightarrow (Z_n(C) \text{ là xạ ảnh}) \Rightarrow (B_n(C) \text{ là xạ ảnh}).$ Ta kết luận bằng cách nhận xét rằng $B_n(C) = 0$ với $n$ đủ nhỏ.

### 7. Phép tổng quát hóa cho các phức của các song môđun ; các đẳng cấu chính tắc

Cho $B, B'$ là hai vành, $C$ là một phức của các $(A, B)$-song môđun, $C'$ là một phức của các $(A, B')$-song môđun ; khi đó $(\mathrm{Homgr}_A(C, C'), D)$ là một phức của các $(B, B')$-song môđun và đồng cấu chính tắc $\lambda : H(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H(C), H(C'))$ là một đồng cấu của các $(B, B')$-song môđun.

Nếu $M$ là một $(A, B)$-song môđun và $N$ là một $(A, B')$-song môđun, thì $\mathrm{Homgr}_A(L(M), I(N))$ là một phức của các $(B, B')$-song môđun, do đó $\mathrm{Ext}_A(M, N)$ được trang bị một cấu trúc tự nhiên của $(B, B')$-song môđun phân bậc ; trên số hạng có bậc 0, cấu trúc này trùng với cấu trúc của $\mathrm{Hom}_A(M, N)$ (II, p. 35).

Nếu $\lambda \in B, \lambda' \in B'$ và nếu ta ký hiệu bởi $\lambda_M, \lambda'_N, \lambda_E, \lambda'_E$ các phép vị tự $x \mapsto x\lambda, y \mapsto y\lambda', z \mapsto \lambda z, z \mapsto z\lambda'$ tương ứng của $M, N, \mathrm{Ext}_A(M, N), \mathrm{Ext}_A(M, N)$, thì

$$
\lambda_E = \mathrm{Ext}_A(\lambda_M, 1), \quad \lambda'_E = \mathrm{Ext}(1, \lambda'_N),
$$

điều này cho một mô tả khác của cấu trúc song môđun của $\mathrm{Ext}_A(M, N)$.

Ta để cho độc giả nhiệm vụ tổng quát hóa các Số 4 và 6 sang trường hợp các phức của các song môđun.

Cho $C, C', C''$ là các phức của các $A$-môđun. Hợp thành của các ánh xạ xác định một đồng cấu phân bậc có bậc không :

(14)
$$
\mathrm{Homgr}_A(C', C'') \otimes_k \mathrm{Homgr}_A(C, C') \to \mathrm{Homgr}_A(C, C'').
$$

Cho B, B', E là các vành, C, C', C'' lần lượt là các phức của các $(B', A)$-song môđun, $(A, E)$-song môđun, $(B, E)$-song môđun. Bằng hạn chế của đẳng cấu chính tắc của II, p. 73, ta thu được một đồng cấu song ánh của các $(B, B')$-song môđun :

(15) $\operatorname{Homgr}_E(C \otimes_A C', C'') \to \operatorname{Homgr}_A(C, \operatorname{Homgr}_E(C', C''))$.

Cuối cùng, cho B là một vành, C là một phức của các B-môđun phải, C' là một phức của các A-môđun phải, C'' là một phức của các $(B, A)$-song môđun. Từ các đồng cấu chính tắc (II. p. 75) ta suy ra

$$
C_p \otimes_B \operatorname{Hom}_A(C'_q, C''_r) \to \operatorname{Hom}_A(C'_q, C_p \otimes_B C''_r)
$$

một đồng cấu phân bậc có bậc không :

(16) $C \otimes_B \operatorname{Homgr}_A(C', C'') \to \operatorname{Homgr}_A(C', C \otimes_B C'')$.

Đồng cấu này là song ánh khi C là một môđun xạ ảnh hữu hạn sinh (II, p. 75, mệnh đề 2).

#### Mệnh đề 12 {#alg-x-s5-prop-12 .statement}

Các đồng cấu (14), (15), (16) là các cấu xạ của các phức.

Ta chứng minh điều này chẳng hạn đối với đồng cấu (14). Ký hiệu

$$
\kappa : \operatorname{Homgr}_A(C', C'') \otimes_k \operatorname{Homgr}_A(C, C') \to \operatorname{Homgr}_A(C, C')
$$

đồng cấu này. Cho $f \in \operatorname{Homgr}_A(C', C'')_p$ và $g \in \operatorname{Homgr}_A(C, C')_q$; khi đó theo định nghĩa ta có $\kappa(f \otimes g) = f \circ g$. Hơn nữa :

$$
\mathrm{D}(f \otimes g) = \mathrm{D}f \otimes g + (-1)^p f \otimes \mathrm{D}g = (d'' \circ f) \otimes g - (-1)^p (f \circ d') \otimes g +
+ (-1)^p f \otimes (d' \circ g) - (-1)^{p+q} f \otimes (g \circ d),
$$

do đó

$$
\kappa(\mathrm{D}(f \otimes g)) = d'' \circ f \circ g - (-1)^p f \circ d' \circ g +
+ (-1)^p f \circ d' \circ g - (-1)^{p+q} f \circ g \circ d \\
= d'' \circ f \circ g - (-1)^{p+q} f \circ g \circ d = \mathrm{D}(f \circ g) = \mathrm{D}(\kappa(f \otimes g)).
$$

Ta chứng minh tương tự rằng các đồng cấu (15) và (16) là các cấu xạ của các phức.

Từ cấu xạ (14) ta suy ra các đồng cấu của các $k$-môđun (X, p. 62)

(17) $\mathrm{H}^p(\operatorname{Homgr}_A(C', C'')) \otimes_k \mathrm{H}^q(\operatorname{Homgr}_A(C, C')) \to \mathrm{H}^{p+q}(\operatorname{Homgr}_A(C, C''))$.

Lấy $C = A$, ta thấy rằng đồng cấu :

(18) $\operatorname{Homgr}_A(C', C'') \otimes_k C' \to C''$ gửi $f \otimes x$ đến $f(x)$ là một cấu xạ của các phức của các $A$-môđun trái ; có liên kết với nó một đồng cấu chính tắc ($X$, p. 80) của các $A$-môđun phân bậc $\gamma : H(\mathrm{Homgr}_A(C', C'')) \otimes_k H(C') \to H(C'')$, tương ứng với đồng cấu chính tắc của các $k$-môđun

$$
\lambda : H(\mathrm{Homgr}_A(C', C'')) \to \mathrm{Homgr}_A(H(C'), H(C''))
$$

## BÀI TẬP {#alg-x-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
