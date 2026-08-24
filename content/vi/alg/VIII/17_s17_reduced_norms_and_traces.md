---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 17
section_title: Reduced Norms and Traces
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.335-A VIII.353
pdf_pages: 0352-0370
extraction: native+ocr
subsections:
    - "no": 1
      title: Complements on Characteristic Polynomials
      page: 335
      pdf_page: 352
    - "no": 2
      title: Reduced Norms and Traces
      page: 339
      pdf_page: 356
    - "no": 3
      title: Properties of Reduced Norms and Traces
      page: 341
      pdf_page: 358
    - "no": 4
      title: The Reduced Norm is a Polynomial Function
      page: 344
      pdf_page: 361
    - "no": 5
      title: Transitivity of Reduced Norms and Traces
      page: 346
      pdf_page: 363
    - "no": 6
      title: Reduced Norms and Determinants
      page: 349
      pdf_page: 366
statements: 30
exercises: 7
content_sha256: cf54e0fca6eaa9208d844a14c62fb66990eb007626a448cdb8abb1dd6688a423
translated_from: content/en/alg/VIII/17_s17_reduced_norms_and_traces.md
source_content_sha256: 11f069df657704342996d2122efce87e5dccfa6a1cfa49a5616defd552614a6d
translation_model: gpt-5-6, gpt-5.4, copied
translation_run: translate-vi-02ef20f9
glossary_version: 34
glossary_terms_sha256: 181915ac1ce0d19e06964343acbfed0ff77ea19ad561b6fb5654494979494c95
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 17. CÁC CHUẨN VÀ VẾT RÚT GỌN

Trong tiết diện này, K là một trường giao hoán và A là một đại số đơn tâm trên K có bậc hữu hạn. Ta ký hiệu bậc rút gọn của A bởi $n$.

### 1. Các bổ sung về các đa thức đặc trưng

Cho L là một vành giao hoán và M là một L-môđun tự do có hạng hữu hạn $m$. Nếu $u$ là một tự đồng cấu của M và $r$ là một số tự nhiên, thì ta ký hiệu $c_r(u)$ là vết của tự đồng cấu $\wedge^r(u)$ của L-môđun tự do $\wedge^r(M)$. Đặc biệt, ta có

(1) $c_0(u) = 1,c_1(u) =$ Tr($u$)$,c_m(u) =$ det($u$),

và $c_r(u) = 0$ với $r > m$. Theo Mệnh đề 7 của III, §8, No. 4, p. 527, ánh xạ $u\mapsto$ det($u$) từ End(M) vào L là một ánh xạ đa thức thuần nhất bậc $m$ (IV, §5, No. 9, p. 55). Nói chung, với mọi số nguyên $r$ sao cho $0\leqslant r\leqslant m$, ánh xạ $c_r$ từ End(M) vào L là một ánh xạ đa thức thuần nhất bậc $r$; điều này suy ra từ Mệnh đề 10 của III, §8, No. 5, p. 529.

Cho $u$ là một tự đồng cấu của M và $\overline{u}$ là tự đồng cấu của L[X]-môđun $M[X] = M\otimes_LL[X]$ suy ra từ $u$ bởi mở rộng vô hướng (II, §5, No. 1, p. 277). Nhắc lại rằng (III, §8, No. 11, p. 541, Định nghĩa 3 và (50)) đa thức đặc trưng của $u$ là định thức $\chi_u(X)$ của tự đồng cấu L[X] $X-\overline{u}$ của M[X] và ta có quan hệ

$$
\chi_u(X) =\sum_{r=0}^m(-1)^rc_r(u) X^{m-r} \tag{2}
$$

Mệnh đề 1. — Cho L là một vành giao hoán, M là một L-môđun tự do có hạng hữu hạn m $ \geqslant 1 $, và u là một tự đồng cấu của M. Tồn tại một tự đồng cấu duy nhất $ \tilde{u} $ của M thỏa mãn quan hệ

$$
\tilde{u}(x) \wedge w = x \wedge \wedge^{m-1}(u)(w)
$$

với $ x \in M $ và $ w \in \wedge^{m-1}(M) $. Hơn nữa, ta có các quan hệ

$$
u \circ \tilde{u} = \tilde{u} \circ u = \det(u)_M,
$$
$$
\det(\tilde{u}) = \det(u)^{m-1},
$$
$$
\tilde{u} = \sum_{r=0}^{m-1} (-1)^r c_{m-1-r}(u) u^r.
$$

#### Bổ đề 1 {#alg-viii-s17-lem-1 .statement tag=00KE}

— Cho p là một số nguyên sao cho $ 0 \leqslant p \leqslant m $. Với mọi w thuộc $ \wedge^p(M) $, đặt $ h_p(w) $ là ánh xạ tuyến tính $ w' \mapsto w \wedge w' $ từ $ \wedge^{m-p}(M) $ vào $ \wedge^m(M) $. Ánh xạ tuyến tính $ h_p : w \mapsto h_p(w) $ từ $ \wedge^p(M) $ vào $ \operatorname{Hom}_L(\wedge^{m-p}(M), \wedge^m(M)) $ là một đẳng cấu.

Cho $ (e_i)_{i \in I} $ là một cơ sở của M; ta trang bị cho tập hợp I một thứ tự toàn phần. Với mọi tập con J của I, đặt $ e_J = e_{i_1} \wedge \cdots \wedge e_{i_r} $, trong đó $ (i_1, \ldots, i_r) $ là dãy các phần tử của J theo thứ tự tăng. L-môđun $ \wedge^{m-p}(M) $ nhận các phần tử $ e_S $ làm một cơ sở, trong đó S chạy qua tập hợp các tập con của I có $ m - p $ phần tử; $ \wedge^m(M) $ có $ \{e_I\} $ làm một cơ sở. Do đó, tồn tại một cơ sở của $ \operatorname{Hom}_L(\wedge^{m-p}(M), \wedge^m(M)) $ gồm các ánh xạ tuyến tính $ e_J^* $ được đặc trưng bởi công thức

$$
e_J^*(e_S) = \begin{cases}
e_I & \text{nếu } I = J \cup S, \\
0 & \text{nếu không},
\end{cases}
$$

trong đó J chạy qua tập hợp các tập con của I có p phần tử. Từ công thức (20) của III, §7, No. 8, p. 519 suy ra rằng với mọi tập con J của I có p phần tử, ta có $ h_p(e_J) \in \{e_J^*, -e_J^*\} $; vì các phần tử $ e_J $ lập thành một cơ sở của $ \wedge^p(M) $, ánh xạ tuyến tính $ h_p $ là song ánh.

Bây giờ chứng minh Mệnh đề 1. Cho u và $ \tilde{u} $ là các tự đồng cấu của M. Quan hệ (3) tương đương với

$$
h_1 \circ \tilde{u} = \operatorname{Hom}(\wedge^{m-1}(u) \cdot 1_{\wedge^m(M)}) \circ h_1;
$$

ánh xạ $ h_1 $ là một đẳng cấu từ M lên $ \operatorname{Hom}_L(\wedge^{m-1}(M), \wedge^m(M)) $ theo Bổ đề 1. Do đó, với mọi tự đồng cấu u của M, tồn tại một tự đồng cấu duy nhất $ \tilde{u} $ của M thỏa mãn quan hệ (3).

Cho $x_1, . . . , x_m$ là các phần tử của M. Hãy thay thế $x$ bằng $u(x_1)$ và $w$ bằng $x_2\wedge  \cdots  \wedge x_m$ trong (3); ta thu được

$\widetilde{u}(u(x_1))\wedge x_2\wedge  \cdots  \wedge x_m=u(x_1)\wedge  \cdots  \wedge u(x_m) =$ det($u$)$x_1\wedge  \cdots  \wedge x_m$.

Do đó, $h_1(\widetilde{u}\circ u(x_1)) =h_1$(det($u$)$x_1$), điều đó cho quan hệ $\widetilde{u}\circ u=$ det($u$)$_M$ theo Bổ đề 1.

Ta ký hiệu bởi U tự đồng cấu $X-\overline{u}$ của L[X]-môđun M[X] (VIII, p. 335). Theo điều trên khi áp dụng cho U, tồn tại một tự đồng cấu $\widetilde{U}$ của L[X]-môđun M[X] thỏa mãn các quan hệ

$$
\widetilde{U}(x_1)\wedge x_2\wedge  \cdots  \wedge x_m=x_1\wedge (Xx_2-u(x_2))\wedge  \cdots  \wedge (Xx_m-u(x_m)) \tag{9}
$$

với $x_1, . . . , x_m$ trong M và

(10) $\widetilde{U}\circ U =$ det(X $-\overline{u}$)$_{M[X]}$.

Hãy xem $\widetilde{U}$ như một phần tử của End(M)[X] (VIII, p. 9); theo công thức (9) và Bổ đề 1, nó có bậc $\leqslant m-1$, vì vậy ta có thể viết nó thành

$$
\widetilde{U} =\sum^{m-1}_{r=0}(-1)^ru_rX^{m-1-r} \tag{11}
$$

trong đó các $u_r$ là các nội tự đồng cấu của M. Theo công thức (2), quan hệ (10) cho đẳng thức

$$
(\sum^{m-1}_{r=0}(-1)^ru_rX^{m-1-r})(X-u) =\sum_{r=0}^m(-1)^rc_r(u)X^{m-r} \tag{12}
$$

trong vành End(M)[X]. Khi đồng nhất các hệ số của các đơn thức theo X ở mỗi vế, ta thu được các quan hệ

(13) $u_r+u_{r-1}\circ u=c_r(u)_M$ với $1\leqslant r\leqslant m-1$

và

$$
u_0=c_0(u)_M,u_{m-1}\circ u=c_m(u)_M \tag{14}
$$

Từ đó, suy ra

$$
u_{m-1}=\sum^{m-1}_{r=0}(-1)^rc_{m-1-r}(u)u^r \tag{15}
$$

Bây giờ, khi ta đồng nhất các hạng hằng, các đẳng thức (9) và (11) suy ra $u_{m-1}=\widetilde{u}$; công thức (6) được suy ra.

Đặc biệt, $\widetilde{u}$ thuộc đại số con của End(M) sinh bởi $u$ và do đó giao hoán với $u$. Ta đã thiết lập quan hệ $\widetilde{u}\circ u=$ det($u$)$_M$; công thức (4) được suy ra.

Cuối cùng, cho $x_1, . . . , x_m$ là các phần tử của M. Ta thay $x$ bằng $x_1$ và $w$ bằng $\widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m)$ trong công thức (3). Điều này cho

$$
\widetilde{u}(x_1)\wedge \widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m) =x_1\wedge u\circ (\widetilde{u}(x_2))\wedge  \cdots  \wedge u\circ (\widetilde{u}(x_m))
$$

= det($u$)$^{m-1}x_1\wedge x_2\wedge  \cdots  \wedge x_m$

và do đó là công thức (5).

#### Nhận xét 1 {#alg-viii-s17-n1-rem-1 .statement tag=00KF}

Tự đồng cấu $\widetilde{u}$ của M trùng với cái mà chúng tôi đã gọi là đối chuyển vị của $u$ trong III, §8, No. 6, p. 532.

#### Nhận xét 2 {#alg-viii-s17-n1-rem-2 .statement tag=00KG}

Từ các công thức (1), (2), (4), và (6), ta suy ra quan hệ $\chi_u(u) = 0$ và do đó có một chứng minh khác của định lý Cayley–Hamilton (III, §8, No. 11, p. 541).

#### Nhận xét 3 {#alg-viii-s17-n1-rem-3 .statement tag=00KH}

Vì ánh xạ $c_r$ từ End(M) vào L là một ánh xạ đa thức thuần nhất bậc $r$ với $0\leqslant r\leqslant m-1$, suy ra từ công thức (6) rằng ánh xạ $u\mapsto \widetilde{u}$ từ End(M) vào End(M) là một ánh xạ đa thức thuần nhất bậc $m-1$.

Cho B là một đại số trên vành L; giả sử rằng B là một L-môđun tự do hạng $m\geqslant 1$, và đồng nhất L với vành con $L\cdot 1$ của B. Cho $b$ là một phần tử của B. Ta áp dụng điều trên cho tự đồng cấu $\gamma (b) :x\mapsto bx$ của L-môđun B. Đặt $\gamma_r(b) =c_r(\gamma (b))$ với $0\leqslant r\leqslant m$; đặc biệt, ta có $\gamma_m(b) = N_{B/L}(b)$ (III, §9, No. 3, p. 543). Đa thức đặc trưng của $b$ (loc. cit.) có thể viết thành

(16) Pc$_{B/L}(b; X) =\sum_{r=0}^m(-1)^r\gamma_r(b) X^{m-r}$.

Vì ánh xạ $\gamma$ từ B vào End$_L(B)$ là L-tuyến tính, nên ánh xạ $\gamma_r$ từ B vào L là một ánh xạ đa thức thuần nhất bậc $r$. Đặc biệt, ánh xạ $b\mapsto N_{B/L}(b)$ từ B vào L là một ánh xạ đa thức thuần nhất bậc $m$.

Với mọi phần tử $b$ của B, đặt

$$
\widetilde{b}=\sum^{m-1}_{r=0}(-1)^r\gamma_{m-1-r}(b)b^r \tag{17}
$$

Theo Mệnh đề 1, ánh xạ tuyến tính $\gamma (\widetilde{b})$ từ B vào B là đối chuyển vị của ánh xạ $\gamma (b)$; từ đó, suy ra

$$
b\widetilde{b}=\widetilde{b}b= N_{B/L}(b) \tag{18}
$$

Hơn nữa, ánh xạ $b\mapsto \widetilde{b}$ từ B vào B là một ánh xạ đa thức thuần nhất bậc $m-1$.

### 2. Các chuẩn và vết rút gọn

Nhắc lại rằng ta ký hiệu bởi A một đại số đơn tâm trên trường giao hoán K, có bậc rút gọn $n$.

#### Mệnh đề 2 {#alg-viii-s17-prop-2 .statement tag=00KI}

Cho $a$ là một phần tử của A và Pc($a; X$) là đa thức đặc trưng của nó. Tồn tại một đa thức đơn khởi duy nhất P trong K[X] sao cho ta có Pc($a; X$) $= P(X)^n$.

A) Tính duy nhất của P suy ra từ Bổ đề 2 dưới đây.

#### Bổ đề 2 {#alg-viii-s17-lem-2 .statement tag=00KJ}

Cho P và Q là các đa thức đơn khởi trong K[X] và $s$ là một số nguyên dương. Nếu $P^s= Q^s$, thì ta có P = Q.

Cho $\mathscr{I}$ là tập hợp các đa thức đơn nhất bất khả quy trong K[X]. Vì P và Q là đơn nhất, tồn tại các phần tử $(a_F)$ và $(b_F)$ của $\mathbf{N}^{(\mathscr{I})}$ sao cho ta có $P =\prod_{F\in\mathscr{I}}F^{a_F}$ và $Q =\prod_{F\in\mathscr{I}}F^{b_F}$. Từ đẳng thức $P^s= Q^s$ và tính duy nhất của phân tích thành các nhân tử bất khả quy, suy ra rằng ta có $sa_F=sb_F$ với mọi $F\in \mathscr{I}$. Vì $s$ là dương ngặt, do đó ta có $a_F=b_F$ với mọi $F\in \mathscr{I}$, và vì thế P = Q.

B) Bây giờ chứng minh sự tồn tại của P.

Theo Định lý 1 của VIII, p. 252, tồn tại một mở rộng Galois L của K bậc hữu hạn và một đẳng cấu của các đại số trên L $\theta : A_{(L)}\rightarrow \mathbf{M}_n(L)$. Theo công thức (12) của III, §9, No. 1, p. 542, đa thức Pc($a; X$) cũng là đa thức đặc trưng của phần tử $1\otimes a$ của đại số trên L $A_{(L)}$, do đó cũng là đa thức đặc trưng của phần tử $\theta (1\otimes a)$ của đại số trên L $\mathbf{M}_n(L)$.

Đặt P(X) = det(X$I_n-\theta (1\otimes a)$); đó là một đa thức đơn khởi trong L[X]. Theo Ví dụ 3 của III, §9, No. 3, p. 545, ta có

(19) Pc($a; X$) $= P(X)^n$.

Cho G là nhóm Galois của L trên K. Với $\sigma \in G$, ký hiệu bởi $\overline{\sigma}$ tự đẳng cấu của vành L[X] trùng với $\sigma$ trên L và cố định X. Khi đó K[X] là tập hợp các đa thức Q của L[X] sao cho ta có $\overline{\sigma}(Q) = Q$ với mọi $\sigma \in G$ (V, §10, No. 1, p. 56, Định lý 1). Vì đa thức Pc($a; X$) $= P(X)^n$ thuộc K[X], nên ta có $\overline{\sigma}(P)^n= P^n$ với mọi $\sigma \in G$. Theo Bổ đề 2, do đó ta có $\overline{\sigma}(P) = P$ với mọi $\sigma \in G$, vậy P thuộc K[X].

#### Định nghĩa 1 {#alg-viii-s17-def-1 .statement tag=00RM}

Cho $a$ là một phần tử của đại số A. Đa thức đặc trưng rút gọn của $a$ (đối với A) là đa thức đơn khởi duy nhất trong K[X], ký hiệu là Pcrd$_{A/K}(a; X)$, thỏa mãn quan hệ

(20) Pc$_{A/K}(a; X) =$ Pcrd$_{A/K}(a; X)^n$.

Cho $a$ là một phần tử của A. Vì A có bậc $n^2$ trên K, đa thức Pc$_{A/K}(a; X)$ có bậc $n^2$, nên Pcrd$_{A/K}(a; X)$ là một đa thức đơn khởi bậc $n$; ta viết nó dưới dạng

(21) Pcrd$_{A/K}(a; X) = X^n+\sum^{n-1}_{r=0}(-1)^rb_r(a)X^{n-r}$.

Ta đặt

(22) Trd$_{A/K}(a) =b_1(a)$, Nrd$_{A/K}(a) =b_n(a)$.

#### Định nghĩa 2 {#alg-viii-s17-def-2 .statement tag=00KK}

Ta gọi Trd$_{A/K}(a)$ là vết rút gọn của A và Nrd$_{A/K}(a)$ là chuẩn rút gọn của nó (đối với đại số trên K A).

Khi không có nguy cơ nhầm lẫn, ta bỏ A và K khỏi ký hiệu và chỉ viết Pcrd($a; X$), Trd($a$), và Nrd($a$).

Các công thức sau suy ra từ các công thức (20) và (22) và các công thức (7) và (8) của III, §9, No. 1, p. 542:

(23) Tr$_{A/K}(a) =n$ Trd$_{A/K}(a)$,

(24) $N_{A/K}(a) =$ (Nrd$_{A/K}(a)$)$^n$.

#### Mệnh đề 3 {#alg-viii-s17-prop-3 .statement tag=00KL}

Một phần tử $a$ của A là khả nghịch khi và chỉ khi chuẩn rút gọn của nó khác không. Đặc biệt, A là một trường khi và chỉ khi ta có Nrd$_{A/K}(a)\not= 0$ với mọi phần tử khác không $a$ của A.

Một phần tử $a$ của A là khả nghịch khi và chỉ khi chuẩn của nó khác không (III, §9, No. 4, p. 545, Mệnh đề 3). Do đó Mệnh đề 3 suy ra từ công thức (24).

#### Nhận xét {#alg-viii-s17-n2-rem-1 .statement tag=00KM}

Cho L là trường K(X) các phân thức hữu tỉ theo một biến X. Đa thức đặc trưng rút gọn của một phần tử $a$ của A đơn giản là chuẩn rút gọn của phần tử $X\otimes 1-1\otimes a$ của đại số trên L $A_{(L)}$. Điều này suy ra từ định nghĩa của đa thức đặc trưng rút gọn và công thức (III, §9, No. 3, p. 544)

(25) Pc$_{A/K}(a; X) = N_{A_{(L)}/L}(X\otimes 1-1\otimes a)$.

#### Ví dụ 1 {#alg-viii-s17-n2-exa-1 .statement tag=00RN}

Theo Định lý 1 của VIII, p. 120, tồn tại một số nguyên $r\geqslant 1$ và một trường D sao cho A đẳng cấu với $\mathbf{M}_r(D)$. Đặt $d$ là bậc thu gọn của D trên K; ta có $r=n/d$. Cho M là một A-môđun có độ dài hữu hạn $\ell$; ta sẽ chứng minh công thức

(26) Pc$_{M/K}(a_M; X) =$ Pcrd$_{A/K}(a; X)^{d\ell}$

với mọi phần tử $a$ của A. A-môđun $A_s$ có độ dài $r$ (VIII, p. 121, Bổ đề 2). Các A-môđun $M^r$ và $A^{\ell}_s$ có cùng độ dài, nên chúng đẳng cấu, và ta có

Pc$_{M/K}(a_M; X)^r=$ Pc$_{A/K}(a; X)^{\ell}$

theo công thức (15) của III, §9, No. 2, p. 542. Vì ta có $rd=n$, công thức (26) suy ra từ công thức (20) và Bổ đề 2 (VIII, p. 339).

#### Ví dụ 2 {#alg-viii-s17-n2-exa-2 .statement tag=00RO}

Xét trường hợp riêng khi A là đại số End$_K(V)$ các tự đồng cấu của một không gian vectơ hữu hạn chiều V trên K. Lấy M là A-môđun đơn V, ta thu được các hệ thức

Pcrd$_{A/K}(u; X) =\chi_u(X)$,

(27) Nrd$_{A/K}(u) =$ det($u$),

Trd$_{A/K}(u) =$ Tr($u$)

đối với mọi tự đồng cấu $u$ của V.

### 3. Các chuẩn và vết rút gọn

#### Mệnh đề 4 {#alg-viii-s17-prop-4 .statement tag=00KN}

Cho L là một mở rộng của K và $a$ là một phần tử của đại số đơn tâm A. Ta có các hệ thức

(28) Pcrd$_{A_{(L)}/L}(1\otimes a; X) =$ Pcrd$_{A/K}(a; X)$,

(29) Trd$_{A_{(L)}/L}(1\otimes a) =$ Trd$_{A/K}(a)$,

(30) Nrd$_{A_{(L)}/L}(1\otimes a) =$ Nrd$_{A/K}(a)$

(“bất biến đối với mở rộng vô hướng”).

Hai vế của đẳng thức (28) có cùng lũy thừa bậc $n$ theo định nghĩa (công thức (20) của VIII, p. 340) và quan hệ

Pc$_{A_{(L)}/L}(1\otimes a; X) =$ Pc$_{A/K}(a; X)$ (III, §9, No. 3, p. 544, công thức (21)). Do đó đẳng thức (28) suy ra từ Bổ đề 2 của VIII, p. 339. Các công thức (29) và (30) suy ra từ (28), (21), và (22).

#### Hệ quả 1 {#alg-viii-s17-prop-4-cor-1 .statement tag=00KO}

Cho L là một mở rộng của K. Cho V là một không gian vectơ chiều $n$ trên L và $\theta$ là một đồng cấu đại số trên K từ A vào End$_L(V)$. Với mọi phần tử $a$ của A, ta có

(31) Pcrd$_{A/K}(a; X) =\chi_{\theta(a)}(X)$,

(32) Trd$_{A/K}(a) =$ Tr($\theta (a)$),

(33) Nrd$_{A/K}(a) =$ det($\theta (a)$).

Cho $\theta '$ là đồng cấu đại số trên L từ $A_{(L)}$ vào End$_L(V)$ sao cho $\theta '(\lambda \otimes a) =\lambda \theta (a)$ với $\lambda \in L$ và $a\in A$. Đại số $A_{(L)}$ là đơn theo Hệ quả 2 của VIII, p. 222; do đó đồng cấu $\theta '$ là đơn ánh. Nhưng các đại số $A_{(L)}$ và End$_L(V)$ trên trường L có cùng bậc, bằng $n^2$, nên $\theta '$ là một đẳng cấu. Khi đó Hệ quả 1 suy ra từ Mệnh đề 4 và Ví dụ 2 ở trên.

#### Hệ quả 2 {#alg-viii-s17-prop-4-cor-2 .statement tag=00KP}

Cho $a$ và $a'$ là các phần tử của A và $\lambda$ là một phần tử của K. Ta có các hệ thức

(34) Pcrd$_{A/K}(a;a) = 0$,

(35) Pcrd$_{A/K}(\lambda a;\lambda X) =\lambda^n$ Pcrd$_{A/K}(a; X)$,

(36) Trd$_{A/K}(a+a') =$ Trd$_{A/K}(a) +$ Trd$_{A/K}(a')$,

Trd$_{A/K}(\lambda a) =\lambda$ Trd$_{A/K}(a)$,

(37) Trd$_{A/K}(aa') =$ Trd$_{A/K}(a'a)$,

(38) Nrd$_{A/K}(aa') =$ Nrd$_{A/K}(a)\cdot$ Nrd$_{A/K}(a')$,

Nrd$_{A/K}(\lambda a) =\lambda^n$ Nrd$_{A/K}(a)$,

(39) Trd$_{A/K}(1) =n$, Nrd$_{A/K}(1) = 1$.

Vì A là đại số đơn tâm và có bậc thu gọn $n$ trên K, nên tồn tại một mở rộng L của K và một không gian vectơ V chiều $n$ trên L sao cho $A_{(L)}$ đẳng cấu với đại số End$_L(V)$ (VIII, p. 252, Định lý 1). Hệ quả 2 khi đó suy ra từ Hệ quả 1 và các tính chất của vết và định thức của một tự đồng cấu. Đặc biệt, công thức (34) suy ra từ định lý Cayley– Hamilton (III, §8, No. 11, p. 541, Mệnh đề 20, xem thêm VIII, p. 338, Nhận xét 2).

#### Hệ quả 3 {#alg-viii-s17-prop-4-cor-3 .statement tag=00RP}

Cho $A^o$ là đại số đối của A. Với mọi $a$ trong A, ta có

(40) Pcrd$_{A^o/K}(a; X) =$ Pcrd$_{A/K}(a; X)$,

(41) Trd$_{A^o/K}(a) =$ Trd$_{A/K}(a)$,

(42) Nrd$_{A^o/K}(a) =$ Nrd$_{A/K}(a)$.

Chọn một mở rộng L của K, một không gian vectơ V có chiều $n$ trên L, và một đồng cấu $\theta$ từ A vào End$_L(V)$ (VIII, p. 252, Định lý 1). Gọi $V^*$ là không gian vectơ đối ngẫu của V. Ánh xạ gửi một phần tử $a$ của A tới tự đồng cấu $^t\theta (a)$ của $V^*$ là một đồng cấu đại số trên K từ $A^o$ vào End$_L(V^*)$. Khi đó Hệ quả 3 suy ra từ Hệ quả 1 và Hệ quả 3 của III, §8, No. 4, p. 528.

Vì thế vết, chuẩn và đa thức đặc trưng của $a$ là như nhau dù ta xem $a$ như một phần tử của A hay như một phần tử của $A^o$. Tính chất này không phải lúc nào cũng đúng khi A không được giả thiết là đơn tâm (III, §9, p. 644, Bài tập 1).

#### Mệnh đề 5 {#alg-viii-s17-prop-5 .statement tag=00KQ}

Với mọi $x$ trong A, đặt $t_x$ là dạng tuyến tính $y\mapsto$ Trd$_{A/K}(xy)$ trên A.

a) Ánh xạ $t:x\mapsto t_x$ là một đẳng cấu các $(A,A)$-song môđun từ A lên đối ngẫu của nó Hom$_K(A,K)$.

b) Cho $h$ là một dạng tuyến tính trên A. Các tính chất sau là tương đương:

(i) Tồn tại một phần tử $\lambda$ của K sao cho $h(x) =\lambda$ Trd$_{A/K}(x)$

với mọi $x\in A$.

(ii) Ta có $h(xy) =h(yx)$ với mọi $x, y$ trong A.

Nhắc lại rằng (II, §1, No. 14, p. 225–226) cấu trúc song môđun $(A$, A)-trên $A^*=$ Hom$_K(A,K)$ được xác định bởi quan hệ

$$
\langle atb, c\rangle =\langle t, bca\rangle \tag{43}
$$

với $a, b, c\in A$ và $t\in A^*$. Đặc biệt, với mọi $x$ trong A, ta có

$\langle at_xb, c\rangle =\langle t_x, bca\rangle =$ Trd$_{A/K}(xbca)$,

$\langle t_{axb}, c\rangle =$ Trd$_{A/K}(axbc)$,

và hai phần tử này bằng nhau theo công thức (37) của VIII, p. 342. Do đó ta có $at_xb=t_{axb}$, điều đó có nghĩa là $t$ là một đồng cấu của $(A$, A)-song môđun từ A vào $A^*$.

Ta chọn một mở rộng L của trường K và một đẳng cấu $\theta$ từ L-đại số $A_{(L)}$ lên đại số ma trận $\mathbf{M}_n(L)$ (VIII, p. 252, Định lý 1). Ta đồng nhất không gian vectơ $(A^*)_{(L)}$ với đối ngẫu của không gian vectơ $A_{(L)}$ trên trường L. Theo Mệnh đề 4 của VIII, p. 341, với những quy ước này, ta có

(44) Trd$_{A_{(L)}/L}= 1_L\otimes$ Trd$_{A/K}$.

Gọi $t_{(L)}$ là ánh xạ L-tuyến tính từ $A_{(L)}$ vào $A^*_{(L)}$ suy ra từ $t$ bởi phép mở rộng vô hướng; theo công thức (44) và Hệ quả 1, ta có

(45) $\langle t_{(L)}(x), y\rangle =$ Trd$_{A_{(L)}/L}(xy) =$ Tr($\theta (x)\theta (y)$)

với $x, y$ trong $A_{(L)}$. Theo Mệnh đề 7 của II, §10, No. 11, p. 358, ánh xạ $t_{(L)}$ là song ánh; do đó $t$ là song ánh. Ta đã chứng minh a).

Cho $h$ thuộc $A^*$; theo điều trên, tồn tại một phần tử $a$ của A sao cho $h$ bằng $t_a$. Theo a), ta có

$$
h(xy)-h(yx) =t_a(xy-yx) =t_{ax}(y)-t_{xa}(y)
$$

Do đó, quan hệ “$h(xy) =h(yx)$ với $x, y$ trong A” là tương đương với “$t_{ax-xa}= 0$ với mọi $x\in$ A”, và theo phần a) của chứng minh, điều đó có nghĩa là $a$ thuộc tâm K của A. Điều này chứng minh b) theo công thức (36).

#### Hệ quả {#alg-viii-s17-n3-cor-1 .statement tag=00KR}

Không gian con tuyến tính của A sinh bởi các phần tử dạng $xy-yx$, trong đó $x$ và $y$ chạy qua A, là một siêu phẳng, hạt nhân của dạng tuyến tính khác không Trd$_{A/K}$.

#### Nhận xét {#alg-viii-s17-n3-rem-1 .statement tag=00KS}

Theo công thức (23) của VIII, p. 340, ta có

Tr$_{A/K}(a) =n$ Trd$_{A/K}(a)$

với mọi $a\in A$. Nếu đặc số của trường K bằng 0 hoặc là một số nguyên tố $p$ không chia hết $n$, thì ta có thể thay thế vết rút gọn bằng vết trong Mệnh đề 5. Mặt khác, nếu đặc số của K là một số nguyên tố chia hết $n$, thì ta có Tr$_{A/K}(a) = 0$ với mọi $a\in A$.

### 4. Chuẩn rút gọn là một hàm đa thức

#### Bổ đề 3 {#alg-viii-s17-lem-3 .statement tag=00KT}

Cho L là một mở rộng của K, và cho I là một tập hợp và $\mathbf{T}= (T_i)_{i\in I}$ là một họ các biến. Ta có $K(\mathbf{T})\cap L[\mathbf{T}] = K[\mathbf{T}]$.

Cho P và Q là các phần tử của $K[\mathbf{T}]$ với $Q\not= 0$. Các hệ số của các đa thức R trong $L[\mathbf{T}]$ sao cho P = QR là các nghiệm của một hệ phương trình tuyến tính với các hệ số trong K. Do đó, nếu tồn tại một đa thức $R\in L[\mathbf{T}]$ sao cho P = QR, thì cũng tồn tại một đa thức như vậy trong $K[\mathbf{T}]$ (II, §8, No. 5, p. 321, Mệnh đề 6). Điều này chứng minh bao hàm $K(\mathbf{T})\cap L[\mathbf{T}]\subset K[\mathbf{T}]$; bao hàm ngược lại là hiển nhiên.

Nhắc lại rằng đa thức đặc trưng rút gọn của một phần tử $a$ của A có thể viết thành

(46) Pcrd$_{A/K}(a; X) =\sum_{r=0}^n(-1)^rb_r(a) X^{n-r}$

và rằng ta có

$b_0(a) = 1,b_1(a) =$ Trd$_{A/K}(a),b_n(a) =$ Nrd$_{A/K}(a)$.

#### Mệnh đề 6 {#alg-viii-s17-prop-6 .statement tag=00KU}

Với mọi số nguyên $r$ sao cho $0\leqslant r\leqslant n$, ánh xạ $b_r$ từ A vào K là một ánh xạ đa thức thuần nhất bậc $r$. Đặc biệt, chuẩn rút gọn là một ánh xạ đa thức thuần nhất bậc $n$ từ A vào K.

Cho $(e_i)_{i\in I}$ là một cơ sở của A trên K và $\mathbf{T}= (T_i)_{i\in I}$ là một họ biến.

#### Bổ đề 4 {#alg-viii-s17-lem-4 .statement tag=00KV}

Cho $u$ là phần tử $\sum_{i\in I}T_i\otimes e_i$ của đại số đơn tâm trên $K(\mathbf{T})$ $A_{(K(\mathbf{T}))}$. Gọi P là đa thức đặc trưng rút gọn của $u$. Khi đó P thuộc vành $K[\mathbf{T}][X]$; được xem như một phần tử của vành $K[\mathbf{T},X]$, nó là thuần nhất bậc $n$.

Ta chọn một mở rộng L của K và một đẳng cấu đại số trên L $\theta$ từ $A_{(L)}$ lên $\mathbf{M}_n(L)$. Ta ký hiệu bởi $\overline{\theta}: A_{(L(\mathbf{T}))}\rightarrow \mathbf{M}_n(L(\mathbf{T}))$ đẳng cấu của các đại số trên $L(\mathbf{T})$ suy ra từ $\theta$ bằng phép mở rộng vô hướng. Theo Hệ quả 1 của VIII, p. 342, ta có

(47) $P(X) =\chi_{\overline{\theta}(u)}(X) =$ det(X$I_n-\overline{\theta}(u)$) $=$ det$(XI_n-\sum_{i\in I}T_i\theta (1\otimes e_i))$.

Vì các ma trận $\theta (1\otimes e_i)$ thuộc $\mathbf{M}_n$(L), công thức này cho thấy rằng P là một đa thức thuần nhất bậc $n$ trong $L[\mathbf{T},X]$. Nó cũng thuộc $K(\mathbf{T})[X]$ và có thể được viết dưới dạng $P(X) =\sum_{j\geqslant 0}c_jX^j$, trong đó mỗi $c_j$ thuộc giao $K(\mathbf{T})\cap L[\mathbf{T}]$. Theo Bổ đề 3, mỗi phần tử $c_j$ đều thuộc $K[\mathbf{T}]$; Bổ đề 4 được suy ra.

#### Bổ đề 5 {#alg-viii-s17-lem-5 .statement tag=00KW}

Với mọi mở rộng $K'$ của K và mọi phần tử $(t_i)_{i\in I}$ của ${K'}^I$, ta có

(48) Pcrd$_{A_{(K')}/K'}(\sum_{i\in I}t_i\otimes e_i)= P((t_i)_{i\in I},X)$.

Cho $\varphi : K[\mathbf{T}]\rightarrow K'$ là đồng cấu đại số trên K duy nhất gửi $T_i$ tới $t_i$ với mọi $i\in I$; nó xác định trên $K'$ cấu trúc đại số trên $K[\mathbf{T}$]. Đại số trên $K'$ $A_{(K[\mathbf{T}])(K')}$ có thể được đồng nhất với $A_{(K')}$ (tính bắc cầu của mở rộng vô hướng), trong đó phần tử $1\otimes (\sum T_i\otimes e_i)$ được đồng nhất với phần tử $\sum t_i\otimes e_i$ của $A_{(K')}$. Ta ký hiệu bởi $\overline{\varphi}: K[\mathbf{T}][X]\rightarrow K'[X]$ đồng cấu đại số trên K suy ra từ $\varphi$. Theo công thức (21) của III, §9, No. 3, p. 544, đa thức đặc trưng của $\sum t_i\otimes e_i$ đối với đại số trên $K'$ $A_{(K')}$ là ảnh bởi $\overline{\varphi}$ của đa thức đặc trưng của $\sum T_i\otimes e_i$ đối với đại số trên $K[\mathbf{T}$] $A_{(K[\mathbf{T}])}$, tức là của $P^n$. Nói cách khác, ta có

(49) Pc$_{A_{(K')}/K'}(\sum_{i\in I}t_i\otimes e_i; X)= P((t_i)_{i\in I},X)^n$;

Bổ đề 5 khi đó suy ra từ Bổ đề 2 của VIII, p. 339.

Xét trường hợp riêng $K'= K$ của Bổ đề 5. Ta có

(50) Pcrd$_{A/K}(\sum_{i\in I}t_ie_i; X)= P((t_i)_{i\in I},X)$

với mọi phần tử $(t_i)_{i\in I}$ của $K^I$. Vì đa thức P trong $K[\mathbf{T},X]$ là thuần nhất bậc $n$, nên nó có thể được khai triển duy nhất thành

$$
P(\mathbf{T},X) =\sum_{r=0}^n(-1)^rB_r(\mathbf{T}) X^{n-r} \tag{51}
$$

trong đó $B_r$ là một đa thức thuần nhất bậc $r$ trong $K[\mathbf{T}]$. Theo các công thức (46), (50), và (51), ta có

$$
b_r(\sum_{i\in I}t_ie_i)= B_r((t_i)_{i\in I})
$$

với mọi phần tử $(t_i)_{i\in I}$ của $K^I$. Mệnh đề 6 suy ra.

#### Nhận xét {#alg-viii-s17-n4-rem-1 .statement tag=00KX}

Cho $K'$ là một đại số giao hoán trên K. Mọi phần tử $t$ của $A_{(K')}$ có thể viết thành $\sum_{i\in I}t_i\otimes e_i$, trong đó $(t_i)\in {K'}^I$. Từ chứng minh của Bổ đề 5 suy ra rằng đa thức đặc trưng Pc$_{A_{(K')}/K'}(t; X)$ bằng $P((t_i),X)^n$.

### 5. Tính bắc cầu của các chuẩn và vết rút gọn

#### Mệnh đề 7 {#alg-viii-s17-prop-7 .statement tag=00KY}

Cho L là một đại số con nửa đơn giao hoán cực đại của A và $a$ là một phần tử của L. Ta có

(52) Pcrd$_{A/K}(a; X) =$ Pc$_{L/K}(a; X)$,

(53) Trd$_{A/K}(a) =$ Tr$_{L/K}(a)$,

(54) Nrd$_{A/K}(a) = N_{L/K}(a)$.

Theo Mệnh đề 3 của VIII, p. 262, các L-môđun A và $L^n$ là đẳng cấu; do đó ta có quan hệ

Pc$_{A/K}(a; X) =$ Pc$_{L/K}(a; X)^n$.

Vì đa thức Pc$_{L/K}(a; X)$ là đơn nhất, do đó nó bằng với đa thức đặc trưng rút gọn Pcrd$_{A/K}(a; X)$ (VIII, p. 339, Bổ đề 2); điều này cho công thức (52). Bằng cách so sánh các hệ số của $X^{n-1}$ (tương ứng, các hạng tử hằng) ở mỗi vế của (52), ta thu được công thức (53) (tương ứng, (54)).

#### Hệ quả {#alg-viii-s17-n5-cor-1 .statement tag=00KZ}

Cho D là một trường bậc hữu hạn trên K có tâm là K. Cho $a$ là một phần tử của K và L là một trường con giao hoán cực đại của D chứa $a$. Ta có

Pcrd$_{D/K}(a; X) =$ Pc$_{L/K}(a; X)$,

(55) Tr$_{D/K}(a) =$ Tr$_{L/K}(a)$,

Nrd$_{D/K}(a) = N_{L/K}(a)$.

Thật vậy, một trường con giao hoán cực đại L của D là một đại số con nửa đơn giao hoán cực đại của D theo Hệ quả 2 của VIII, p. 265.

#### Mệnh đề 8 {#alg-viii-s17-prop-8 .statement tag=00L0}

Cho B là một đại số con đơn của A. Ký hiệu tâm của B là L và hoán tập của B trong A là $B'$. Khi đó $B'$ là một đại số đơn tâm trên trường L; ta ký hiệu bậc thu gọn của nó là $r$. Với mọi phần tử $b$ của B, ta có các hệ thức

(56) Pcrd$_{A/K}(b; X) = N_{L[X]/K[X]}$(Pcrd$_{B/L}(b; X)$)$^r$,

(57) Trd$_{A/K}(b) =r$ Tr$_{L/K}$(Trd$_{B/K}(b)$),

(58) Nrd$_{A/K}(b) = N_{L/K}$(Nrd$_{B/L}(b)$)$^r$.

#### Bổ đề 6 {#alg-viii-s17-lem-6 .statement tag=00L1}

Cho $K'$ là một đại số giao hoán bậc hữu hạn $d$ trên K và

$$
P(X) = X^s+a_1X^{s-1}+\cdots +a_s
$$

một đa thức đơn khởi với các hệ số trong $K'$. Khi đó đa thức Q = $N_{K'[X]/K[X]}(P)$ trong K[X] là đơn khởi bậc $sd$, hệ số của $X^{sd-1}$ trong Q(X) bằng Tr$_{K'/K}(a_1)$, và số hạng hằng của Q là $N_{K'/K}(a_s)$.

Ta ký hiệu $K'$-đại số $K'[T]/(P(T))$ bởi $K''$ và lớp chính tắc của T trong $K''$ bởi $t$. Dãy $(1, t, . . . , t^{s-1})$ là một cơ sở của $K''$ trên $K'$, và ma trận của phép nhân bởi $ t $ trong cơ sở này có dạng

$$
\tau = \begin{pmatrix}
0 & 0 & \cdots & 0 & -a_s \\
1 & 0 & \cdots & 0 & -a_{s-1} \\
0 & 1 & \cdots & 0 & -a_{s-2} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
0 & \cdots & \cdots & 1 & -a_1
\end{pmatrix}.
$$

Định thức của $ XI_n - \tau $ được tính bằng quy nạp theo $ s $, bằng cách khai triển theo hàng thứ nhất. Ta thu được $ \det(XI_n - \tau) = P(X) $. Nói cách khác, ta có $ P(X) = Pc_{K''/K'}(t; X) $. Đặc biệt, $ \operatorname{Tr}_{K''/K'}(t) = -a_1 $ và $ N_{K''/K'}(t) = (-1)^s a_s $. Theo công thức tính bắc cầu (III, §9, No. 4, p. 548, Hệ quả), ta có

$$
\operatorname{Tr}_{K''/K}(t) = -\operatorname{Tr}_{K'/K}(a_1), \quad N_{K''/K}(t) = (-1)^{sd} N_{K'/K}(a_s),
$$
$$
Q(X) = Pc_{K''/K}(t; X).
$$

Mặt khác, $[K'' : K] = [K'' : K'][K' : K] = sd$, nên $ Q(X) $ là một đa thức đơn khởi bậc $ sd $. Bổ đề 6 được suy ra.

Hãy chứng minh Mệnh đề 8. Vì vành $ B $ là đơn, tâm của nó $ L $ là một trường (VIII, p. 121, Hệ quả 1). Theo Định lý 5 của VIII, p. 259, hoán tập $ B' $ của $ B $ trong $ A $ là một vành đơn có tâm $ L $, và ta có đẳng thức $[A : K] = [B : K][B' : K]$. Ta ký hiệu bậc thu gọn của $ B' $ trên $ L $ là $ r $, bậc thu gọn của $ B $ trên $ L $ là $ s $, và bậc của $ L $ trên $ K $ là $ d $. Ta có

$$
[A : K] = n^2, \quad [B' : K] = r^2 d, \quad [B : K] = s^2 d,
$$

và do đó $ n^2 = r^2 s^2 d^2 $, nghĩa là $ n = rsd $.

Cho $ b $ là một phần tử của $ B $, và gọi $ P(X) $ là đa thức đặc trưng rút gọn của nó trên $ L $-đại số $ B $; nó là monic bậc $ s $. Theo Bổ đề 6, đa thức $ Q = N_{L[X]/K[X]}(P) $ là monic bậc $ sd $. Do đó đa thức $ R = Q^r $ là monic bậc $ rsd = n $. Lại theo Bổ đề 6, hệ số của $ X^{n-1} $ trong $ R(X) $ bằng $ -r \operatorname{Tr}_{L/K}(\operatorname{Trd}_{B/L}(b)) $, và số hạng hằng của $ R(X) $ là $ (N_{L/K}((-1)^s \operatorname{Nrd}_{B/L}(b)))^r = (-1)^n N_{L/K}(\operatorname{Nrd}_{B/L}(b))^r $.

Vì $[A : K] = r^2 d[B : K]$, $ B $-môđun trái $ A $ là tự do hạng $ r^2 d $ (VIII, p. 124, Mệnh đề 5). Do đó ta có

$$
\operatorname{Pc}_{A/K}(b; X) = \operatorname{Pc}_{B/K}(b; X)^{dr^2}.
$$

Theo hệ quả của III, §9, No. 4, p. 548, ta có

$$
\operatorname{Pc}_{B/K}(b; X) = N_{L[X]/K[X]}(\operatorname{Pc}_{B/L}(b; X)),
$$

và vì P(X) là đa thức đặc trưng rút gọn của $b$ trên đại số trên L B, nên ta có

(62) Pc$_{B/L}(b; X) = P(X)^s$.

Sau cùng, theo các công thức (60)—(62) và định nghĩa của R(X), ta có

(63) Pc$_{A/K}(b; X) = N_{L[X]/K[X]}(P(X))^{dr^2s}= Q(X)^{dr^2s}= R(X)^{rsd}= R(X)^n$,

nên R(X) là đa thức đặc trưng rút gọn của $b$ trên đại số trên K A.

Chúng ta đã chứng minh công thức (56). Các công thức (57) và (58) suy ra ngay lập tức từ công thức (56) và Bổ đề 6 vì hệ số của $X^{n-1}$ trong Pcrd$_{A/K}(b; X)$ bằng $-$ Trd$_{A/K}(b)$ và số hạng hằng là $(-1)^n$ Nrd$_{A/K}(b)$.

### 6. Chuẩn thu gọn và Định thức

Trong tiểu mục này, D là một trường có bậc hữu hạn trên K với tâm là K. Ta ký hiệu bởi $D^*_{ab}$ thương của nhóm nhân $D^*$ bởi nhóm dẫn xuất (hay nhóm giao hoán tử) của nó và bởi $\pi$ đồng cấu chính tắc từ $D^*$ vào $D^*_{ab}$. Ánh xạ Nrd$_{D/K}$ cảm sinh một đồng cấu nhóm từ $D^*$ vào $K^*$; hạt nhân của đồng cấu này chứa nhóm dẫn xuất của $D^*$ vì K là giao hoán. Do đó tồn tại một đồng cấu duy nhất Nrd từ $D^*_{ab}$ vào $K^*$ sao cho Nrd$_{D/K}(x) =$ Nrd $\circ \pi (x)$ với mọi $x\in D^*$.

#### Mệnh đề 9 {#alg-viii-s17-prop-9 .statement tag=00L2}

Cho V là một không gian vectơ phải hữu hạn chiều trên trường D. Cho E là đại số End$_D(V)$ trên trường K; nó là đơn tâm và có bậc hữu hạn. Với mọi phần tử khả nghịch $u$ của E, ta có

(64) Nrd$_{E/K}(u) =$ Nrd(det $u$)

(xem VIII, p. 452, Mệnh đề 2 để biết định nghĩa của định thức det $u$ của $u$).

Ta ký hiệu chiều của V trên D là $n$ và đồng nhất E với đại số ma trận $\mathbf{M}_n(D)$ bằng cách dùng một cơ sở của V trên D. Nhóm nhân GL$_n(D)$ của đại số E được sinh bởi các ma trận đường chéo và các ma trận $B_{ij}(\lambda )$ (II, §10, No. 13, p. 362, Hệ quả 1). Do đó Mệnh đề 9 suy ra từ hai trường hợp riêng dưới đây.

A) Giả sử rằng $u$ là ma trận đường chéo diag($a_1, . . . , a_n$). Với mọi $1\leqslant i\leqslant n$, gọi $L_i$ là một trường con giao hoán cực đại của D chứa $a_i$; gọi L là đại số con của E gồm các ma trận đường chéo diag($t_1, . . . , t_n$) với $t_i\in L_i$ đối với $1\leqslant i\leqslant n$. Gọi $d$ là bậc thu gọn của D trên K. Ta có $[L_i: K] =d$ đối với $1\leqslant i\leqslant n$ (VIII, p. 265, Hệ quả 2). Đại số trên K L đẳng cấu với $L_1\times  \cdots  \times L_n$ và do đó nửa đơn bậc $nd$; mặt khác, ta có $[E : K] =n^2[D : K] =n^2d^2= [L : K]^2$. Suy ra L là một đại số con nửa đơn giao hoán cực đại của E (VIII, p. 262, Mệnh đề 3). Theo Mệnh đề 7 của VIII, p. 346, ta có Nrd$_{E/K}(u) = N_{L/K}(u)$. Do đó, theo công thức (18) của III, §9, No. 3, p. 544, ta có

Nrd$_{E/K}(u) =\prod_{i=1}^nN_{L_i/K}(a_i) =\prod_{i=1}^n$ Nrd$_{D/K}(a_i)$

= Nrd$_{D/K}(a_1\cdots a_n) =$ Nrd($\pi (a_1\cdots a_n)$).

Hơn nữa, ta có det $u=\pi (a_1\cdots a_n)$ theo Mệnh đề 3 của VIII, p. 453, điều này cho công thức (64) trong trường hợp này.

B) Giả sử rằng $u$ bằng $B_{ij}(\lambda )$, trong đó $\lambda$ là một phần tử của D và $i, j$ là các số nguyên phân biệt trong khoảng $[1, n]$. Ký hiệu $d$ là bậc thu gọn của D trên K và M là không gian vectơ trên K suy ra từ V bằng hạn chế vô hướng từ D xuống K. Khi đó M là một E-môđun đơn, và ta có

(65) Pc$_{M/K}(u; X) =$ Pcrd$_{E/K}(u; X)^d$

theo công thức (26) của VIII, p. 341. Hơn nữa, M là một không gian vectơ chiều $nd^2$ trên K, và $u-1_M$ là một tự đồng cấu lũy linh của M; do đó ta có

(66) Pc$_{M/K}(u; X) = (X-1)^{nd^2}$.

So sánh các công thức (65) và (66), ta được

(67) Pcrd$_{E/K}(u; X) = (X-1)^{nd}$

và, đặc biệt, Nrd$_{E/K}(u) = 1$. Ta cũng có det $u= 1$ theo Mệnh đề 3 của VIII, p. 453; do đó công thức (64) đúng trong trường hợp này.

#### Nhận xét {#alg-viii-s17-n6-rem-1 .statement tag=00L3}

Ta có Nrd$_{E/K}(u) = 0$ nếu phần tử $u$ của E không khả nghịch (VIII, p. 340, Mệnh đề 3).

### Bài tập {#alg-viii-s17-exercises}

Xem [bài tập của § 17](exercises/s17/).
