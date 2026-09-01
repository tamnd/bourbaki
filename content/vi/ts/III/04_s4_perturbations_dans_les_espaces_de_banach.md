---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 4
section_title: Perturbations dans les espaces de Banach
lang: vi
source: ts-iii-v-fr
book_pages: TS III.55-TS III.70, TS III.123-TS III.124
pdf_pages: 0069-0084, 0137-0138
extraction: native
subsections:
    - "no": 1
      title: Morphismes directs
      page: 55
      pdf_page: 69
    - "no": 2
      title: Perturbation des applications de Fredholm
      page: 58
      pdf_page: 72
    - "no": 3
      title: Perturbation des endomorphismes de Riesz
      page: 59
      pdf_page: 73
    - "no": 4
      title: Conorme d’une application linéaire continue
      page: 61
      pdf_page: 75
    - "no": 5
      title: Sous-espaces vectoriels de dimension finie d’un espace normé
      page: 64
      pdf_page: 78
    - "no": 6
      title: Perturbations des applications linéaires continues injectives ou surjectives
      page: 67
      pdf_page: 81
statements: 30
exercises: 9
content_sha256: a4cf23b6e9c7f56373d1f0b9b696bb30b5130f17e3272e44044260d216db314d
translated_from: content/en-mt/ts/III/04_s4_perturbations_dans_les_espaces_de_banach.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 910670a80334f4bc17a1ba846cbcae9dfc4d7bd9a3a996a8e9e2f73e3cf9c369
translation_model: gpt-5.4
translation_run: translate-vi-3c39d970
glossary_version: 34
glossary_terms_sha256: e747ed039eda495cd279811a399baa1f7526f8212b047aabe585328b14a48aaa
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. NHIỄU ĐỘNG TRONG CÁC KHÔNG GIAN BANACH

### 1. Các cấu xạ trực tiếp

#### Định nghĩa 1 {#ts-iii-s4-def-1 .statement tag=02SH}

Cho E là một không gian vectơ tôpô. Một không gian con vectơ của E được gọi là trực tiếp nếu nó có một phần bù tôpô.

Để một không gian con vectơ F của E là trực tiếp, điều kiện cần và đủ là tồn tại trong $\mathscr{L}(E)$ một phép chiếu có ảnh là F. Nếu $p$ là một phép chiếu như vậy thì E là tổng trực tiếp tôpô của F và hạt nhân của $p$. Hạt nhân của $1_E-p$ là F; do đó nếu E tách được thì F đóng.

Cho F là một không gian con vectơ trực tiếp của E và cho $E_1$ là một không gian con vectơ của E chứa F; khi đó F là một không gian con vectơ trực tiếp của $E_1$.

Mọi không gian con vectơ đóng có đối chiều hữu hạn trong E đều trực tiếp (TVS, I, p. 15, mệnh đề 3), và mọi không gian con vectơ F của E được chứa trong bao đóng của $\{0\}$ đều trực tiếp (thật vậy, tồn tại một phép chiếu có ảnh là F, và một phép chiếu như vậy tất yếu là liên tục).

#### Mệnh đề 1 {#ts-iii-s4-prop-1 .statement tag=02SI}

Cho E là một không gian lồi địa phương. Mọi không gian con vectơ hữu hạn chiều của E đều trực tiếp.

Cho F là một không gian con vectơ hữu hạn chiều của E. Ký hiệu S là một phần bù tôpô của bao đóng của $\{0\}$ trong F, là một không gian con trực tiếp của E. Không gian $F_2= F\cap S$ là tách được và hữu hạn chiều; do đó tồn tại một số nguyên $n\geqslant 0$ sao cho $F_2$ đẳng cấu với $K^n$ (TVS, I, p. 14, th. 2). Khi đó tồn tại một ánh xạ tuyến tính liên tục $p: S\rightarrow F_2$ mở rộng ánh xạ đồng nhất của $F_2$ (TVS, II, p. 26, nhận xét). Hạt nhân của $p$ là một phần bù tôpô của $F_2$ trong S, và cũng là một phần bù tôpô của F trong E.

#### Định nghĩa 2 {#ts-iii-s4-def-2 .statement tag=02SJ}

Cho E và F là các không gian lồi địa phương, và cho $u$ là một ánh xạ tuyến tính liên tục từ E vào F. Ta nói rằng $u$ là một cấu xạ trực tiếp nếu $u$ là một cấu xạ ngặt mà hạt nhân của nó là một không gian con vectơ trực tiếp của E và ảnh của nó là một không gian con vectơ trực tiếp của F.

Cho $u\in \mathscr{L}(E; F)$. Để hạt nhân và ảnh của $u$ lần lượt là các không gian con vectơ trực tiếp của E và F, điều kiện cần và đủ là tồn tại các phân tích $E = E_1\oplus E_2$ và $F = F_1\oplus F_2$ thành các tổng trực tiếp tôpô sao cho $u$ được biểu diễn bởi một ma trận $\begin{pmatrix} u_1 & 0 \\ 0 & 0 \end{pmatrix}$ trong đó $u_1\in \mathscr{L}(E_1; F_1)$ là song ánh. Vì khi đó hạt nhân của $u$ là $E_2$, vì ánh xạ tuyến tính chính tắc từ $E_1$ lên $E/E_2$ là một đẳng cấu, và vì ảnh của $u$ là $F_1$, ta thấy rằng $u$ là một cấu xạ ngặt khi và chỉ khi $u_1$ là một đẳng cấu từ $E_1$ lên $F_1$. Ký hiệu $v$ là phần tử của $\mathscr{L}(F; E)$ được biểu diễn bởi ma trận $\begin{pmatrix} u_1^{-1} & 0 \\ 0 & 0 \end{pmatrix}$ . Khi đó ánh xạ tuyến tính $u\circ v$ là phép chiếu trong F có hạt nhân là $F_2$ và ảnh là $F_1$, ánh xạ tuyến tính $v\circ u$ là phép chiếu trong E có hạt nhân là $E_2$ và ảnh là $E_1$, và ta có $u\circ v\circ u=u$.

Ngược lại, ta có kết quả sau:

#### Mệnh đề 2 {#ts-iii-s4-prop-2 .statement tag=02SK}

Cho E và F là các không gian lồi địa phương, cho $u\in \mathscr{L}(E; F)$ và $v\in \mathscr{L}(F; E)$. Giả sử rằng $u=u\circ v\circ u$. Khi đó $u$ là một cấu xạ trực tiếp. Hơn nữa, $v\circ u$ là một phép chiếu liên tục trong E có hạt nhân Ker($u$), và $u\circ v$ là một phép chiếu liên tục trong F có ảnh Im($u$).

Đặt $p=v\circ u$ và $q=u\circ v$. Ta có

$$
p^2=v\circ (u\circ v\circ u) =v\circ u=p ,q^2= (u\circ v\circ u)\circ v=u\circ v=q
$$

do đó $p$ và $q$ là các phép chiếu. Chúng liên tục. Gọi $E_1$ và $E_2$ lần lượt là ảnh và hạt nhân của $p$, và gọi $F_1$ và $F_2$ lần lượt là ảnh và hạt nhân của $q$. Vì $u\circ v\circ u=u$, ta có

Ker($u$)$\subset$ Ker($v\circ u$)$\subset$ Ker($u\circ v\circ u$) $=$ Ker($u$),

do đó Ker($u$) $=$ Ker($v\circ u$) $=$ Ker($p$) $= E_2$. Tương tự, từ các bao hàm

Im($u$)$\supset$ Im($u\circ v$)$\supset$ Im($u\circ v\circ u$) $=$ Im($u$)

suy ra ảnh của $u$ là $F_1$. Các không gian $E_2$ và $F_1$ lần lượt là các không gian con vectơ trực tiếp của E và F.

Không gian vectơ E là tổng trực tiếp tôpô của $E_1$ và $E_2$, và $u$ xác định bằng hạn chế một ánh xạ tuyến tính song ánh $u_1$ từ $E_1$ lên $F_1$. Với mọi $x\in E_1$, ta có $v(u(x)) =p(x) =x$, và ánh xạ $u^{-1}_1$ từ $F_1$ lên $E_1$ trùng với $v$ trên $F_1$. Do đó, $u_1$ là một đẳng cấu từ $E_1$ lên $F_1$ và $u$ là một cấu xạ ngặt từ E vào F.

Cho E và F là các không gian lồi địa phương và cho $u\in \mathscr{L}(E; F)$. Để $u$ là một cấu xạ đơn ánh trực tiếp (tương ứng, toàn ánh), điều kiện cần và đủ là tồn tại $v$ trong $\mathscr{L}(F; E)$ sao cho $v\circ u= 1_E$ (tương ứng $u\circ v= 1_F$) (xem TG, III, p. 47 and 48).

#### Mệnh đề 3 {#ts-iii-s4-prop-3 .statement tag=02SL}

Cho E và F là các không gian Banach. Các tập hợp sau là các tập con mở của không gian Banach $\mathscr{L}(E; F):$

a) Tập hợp $\mathscr{I}(E; F)$ các đẳng cấu từ E lên F ;

b) Tập $\mathscr{M} \mathscr{D}(E; F)$ các cấu xạ trực tiếp đơn ánh từ E vào F, và chính xác hơn, với mỗi không gian con vectơ đóng $F_1$ của F, tập $\mathscr{M}_{F_1}(E; F)$ các phần tử của $\mathscr{M} \mathscr{D}(E; F)$ mà ảnh là một phần bù tôpô của $F_1$;

c) Tập $\mathscr{E} \mathscr{D}(E; F)$ các cấu xạ trực tiếp toàn ánh từ E lên F, và chính xác hơn, với mỗi không gian con vectơ đóng $E_1$ của E, tập $\mathscr{E}_{E_1}(E; F)$ các phần tử của $\mathscr{E} \mathscr{D}(E; F)$ mà hạt nhân là một phần bù tôpô của $E_1$.

Hơn nữa, ánh xạ $u\mapsto u^{-1}$ từ $\mathscr{I}(E; F)$ lên $\mathscr{I}(F; E)$ là giải tích.

Theo định nghĩa, $\mathscr{I}(E; E)$ là tập các phần tử khả nghịch của đại số định chuẩn đầy đủ $\mathscr{L}(E)$. Theo TG, IX, p. 40, Prop. 14, đó là một tập con mở của $\mathscr{L}(E)$. Ánh xạ $u\mapsto u^{-1}$ từ $\mathscr{I}(E; E)$ vào $\mathscr{I}(E; E)$ là giải tích (LIE, III, § 1, n$^o1$, Ví dụ 2).

Nếu tập $\mathscr{I}(E; F)$ là rỗng, thì nó mở. Nếu không, cho $u_0$ là một đẳng cấu của E lên F. Khi đó ánh xạ $v\mapsto u_0\circ v$ là một đẳng cấu từ $\mathscr{L}(E)$ lên $\mathscr{L}(E; F)$ biến đổi $\mathscr{I}(E; E)$ thành $\mathscr{I}(E; F)$. Do đó tập $\mathscr{I}(E; F)$ là mở trong $\mathscr{L}(E; F)$. Hơn nữa, nếu $u=u_0\circ v$ là một phần tử của $\mathscr{I}(E; F)$, ta có $u^{-1}=v^{-1}\circ u^{-1}_0$, và do đó ánh xạ $u\mapsto u^{-1}$ từ $\mathscr{I}(E; F)$ lên $\mathscr{I}(F; E)$ là giải tích.

Cho $F_1$ là một không gian con vectơ đóng của F. Với mỗi $u\in \mathscr{L}(E; F)$, gọi $\overline{u}$ là phần tử của $\mathscr{L}(E\times F_1; F)$ được xác định bởi $\overline{u}(x, y) =u(x) +y$. Ánh xạ $u\mapsto \overline{u}$ từ $\mathscr{L}(E; F)$ vào $\mathscr{L}(E\times F_1; F)$ là liên tục, và $\mathscr{M}_{F_1}(E; F)$ là tập các phần tử $u$ của $\mathscr{L}(E; F)$ sao cho $\overline{u}$ thuộc $\mathscr{I}(E\times F_1; F)$. Vì $\mathscr{I}(E\times F_1; F)$ là mở trong $\mathscr{L}(E\times F_1; F)$ theo điều đi trước, tập $\mathscr{M}_{F_1}(E; F)$ là mở trong $\mathscr{L}(E; F)$. Điều tương tự cũng đúng với $\mathscr{M} \mathscr{D}(E; F)$, là hợp của các $\mathscr{M}_{F_1}(E; F)$ khi $F_1$ chạy qua tập các không gian con vectơ đóng của F.

Cho $E_1$ là một không gian con vectơ đóng của E, và gọi $p$ là ánh xạ chính tắc từ E lên không gian Banach thương $E/E_1$. Để một phần tử $u$ của $\mathscr{L}(E; F)$ thuộc $\mathscr{E}_{E_1}(E; F)$, điều kiện cần và đủ là ánh xạ $(u, p)$ từ E vào $F\times E/E_1$ thuộc $\mathscr{I}(E; F\times E/E_1)$. Như trên, suy ra rằng $\mathscr{E}_{E_1}(E; F)$ là mở trong $\mathscr{L}(E; F)$; điều tương tự cũng đúng với $\mathscr{E} \mathscr{D}(E; F)$, là hợp của các $\mathscr{E}_{E_1}(E; F)$.

### 2. Nhiễu xạ của các ánh xạ Fredholm

#### Định lý 1 {#ts-iii-s4-thm-1 .statement tag=02SM}

Cho E và F là các không gian Banach. Tập $\mathscr{F}(E; F)$ các ánh xạ Fredholm từ E vào F là mở trong không gian Banach $\mathscr{L}(E; F)$, và ánh xạ $u\mapsto$ ind($u$) từ $\mathscr{F}(E; F)$ vào $\mathbf{Z}$ là hằng địa phương.

Định lý suy ra từ mệnh đề chính xác hơn sau đây:

#### Mệnh đề 4 {#ts-iii-s4-prop-4 .statement tag=02SN}

Cho E và F là các không gian Banach, cho $u_0: E\rightarrow F$ là một ánh xạ Fredholm và $v_0$ là một nghịch đảo giả của $u_0$. Tồn tại một lân cận mở U của $u_0$ trong $\mathscr{L}(E; F)$ và một ánh xạ giải tích $\varphi : U\rightarrow \mathscr{L}(F; E)$ sao cho

(i) Ta có $\varphi (u_0) =v_0$;

(ii) Với mọi $u$ trong U, ánh xạ $\varphi (u)$ là một nghịch đảo giả của $u$, và đặc biệt $u$ là một ánh xạ Fredholm;

(iii) Với mọi $u$ trong U, ta có ind($u$) $=$ ind($u_0$).

Theo mệnh đề 2 của III, p. 42, (ii), tồn tại các phân tích tổng trực tiếp tôpô $E = E_1\oplus E_2$ và $F = F_1\oplus F_2$, và tồn tại $\alpha_0\in \mathscr{I}(E_1; F_1)$, sao cho $E_2$ và $F_2$ là hữu hạn chiều và $u_0$ được biểu diễn bởi ma trận $\begin{pmatrix} \alpha_0 & 0 \\ 0 & 0 \end{pmatrix}$ đối với các phân tích này.

Gọi U là tập các phần tử $u$ của $\mathscr{L}(E; F)$ sao cho, trong biểu diễn ma trận $\begin{pmatrix} \alpha & \beta \\ \gamma & \delta \end{pmatrix}$ của $u$ đối với các phân tích này, ta có $\alpha \in \mathscr{I}(E_1; F_1)$. Vì $\mathscr{I}(E_1; F_1)$ là mở trong $\mathscr{L}(E_1; F_1)$ (mệnh đề 3 của III, p. 57), U là một lân cận mở của $u_0$ trong $\mathscr{L}(E; F)$. Với $u=\begin{pmatrix} \alpha & \beta \\ \gamma & \delta \end{pmatrix}$ trong U, đặt

$$
\varphi (u) =v_0+\begin{pmatrix} \alpha^{-1}-\alpha_0^{-1} & 0 \\ 0 & 0 \end{pmatrix} \tag{1}
$$

Ta có $\varphi (u_0) =v_0$ và ánh xạ $\varphi$ là giải tích (loc. cit.). Theo modulo các ánh xạ tuyến tính liên tục hạng hữu hạn, ta có các đồng dư

$$
u\equiv \begin{pmatrix} \alpha & 0 \\ 0 & 0 \end{pmatrix},v_0\equiv \begin{pmatrix} \alpha_0^{-1} & 0 \\ 0 & 0 \end{pmatrix},\varphi (u)\equiv \begin{pmatrix} \alpha^{-1} & 0 \\ 0 & 0 \end{pmatrix}
$$

Do đó, $\varphi (u)$ là một nghịch đảo giả của $u$. Mọi phần tử $u$ của U xác định bởi hạn chế một đẳng cấu từ $E_1$ lên một phần bù tôpô của $F_2$ trong F. Theo mệnh đề 3 của III, p. 44, do đó ta có

ind($u$) $=$ codim$_F(u(E_1))-$ codim$_E(E_1)$

= dim(F$_2$)$-$ dim(E$_2$) $=$ ind($u_0$),

điều này hoàn tất chứng minh.

### 3. Nhiễu của các tự đồng cấu Riesz

#### Bổ đề 1 {#ts-iii-s4-lem-1 .statement tag=02SO}

Cho E là một không gian Banach. Cho $p$ và $q$ là các phép chiếu liên tục của E sao cho $\|q-p\|<1$. Khi đó $p$ cảm sinh một đẳng cấu của Im($q$) lên Im($p$), và $1_E-p$ cảm sinh một đẳng cấu của Ker($q$) lên Ker($p$).

Xét các ánh xạ tuyến tính liên tục $u:x\mapsto p(x)$ từ Im($q$) vào Im($p$) và $v:y\mapsto q(y)$ từ Im($p$) vào Im($q$). Với mọi $x\in$ Im($q$), ta có $x=q(x)$, do đó

$$
(q-p)^2(x) =q^2(x)-q(p(x))-p(q(x)) +p^2(x)
$$

$$
=x-q(p(x)) =x-v(u(x))
$$

Vậy $\|1_E-v\circ u\|\leqslant \|q-p\|^2<1$. Theo Hệ quả 1 của I, p. 22$,v\circ u$ là một tự đẳng cấu của Im($q$). Chứng minh tương tự cho thấy $u\circ v$ là một tự đẳng cấu của Im($p$). Điều này kéo theo rằng $u$ là một đẳng cấu của Im($q$) lên Im($p$), do đó có mệnh đề thứ nhất của bổ đề. Mệnh đề thứ hai suy ra bằng cách thay thế $p$ và $q$ lần lượt bởi $1_E-p$ và $1_E-q$.

#### Định lý 2 {#ts-iii-s4-thm-2 .statement tag=02SP}

Cho E là một không gian Banach. Tập $\mathscr{R}(E)$ các tự đồng cấu Riesz của E là mở trong $\mathscr{L}(E)$. Ánh xạ gán cho một phần tử của $\mathscr{R}(E)$ chiều của không gian lũy linh của nó là nửa liên tục trên trên $\mathscr{L}(E)$.

Định lý suy ra từ mệnh đề chính xác hơn sau đây:

#### Mệnh đề 5 {#ts-iii-s4-prop-5 .statement tag=02SQ}

Cho E là một không gian Banach và $u_0$ là một tự đồng cấu Riesz của E. Gọi N (tương ứng I) là không gian lũy linh (tương ứng đối không gian lũy linh) của $u_0$. Ký hiệu $d$ là chiều của N. Tồn tại một lân cận mở U của $u_0$ trong $\mathscr{L}(E)$ và một ánh xạ giải tích $\pi : U\rightarrow \mathscr{L}(E)$ sao cho

(i) Tự đồng cấu $\pi (u_0)$ là phép chiếu có ảnh là N và hạt nhân là I;

(ii) Với mọi $u\in U$, ánh xạ tuyến tính $\pi (u)$ là một phép chiếu hạng $d$ thuộc đối giao hoán tử kép của $u$ và, đặc biệt, giao hoán với $u$. Hơn nữa, $u$ cảm sinh một tự đẳng cấu của Ker($\pi (u)$);

(iii) Mọi phần tử của U đều là một tự đồng cấu Riesz mà không gian lũy linh có chiều $\leqslant d$.

Nếu K = $\mathbf{C}$, gọi Sp($u_0$) là phổ của $u_0$ đối với đại số $\mathscr{L}(E)$. Khi K = $\mathbf{R}$, gọi Sp($u_0$) là phổ phức Sp$_{\mathscr{L}(E_{(\mathbf{C})})}((u_0)_{(\mathbf{C})})$ của $u_0($I, p. 85, n$^o13$). Theo mệnh đề 14 của III, p. 54, điểm 0 là cô lập trong $\{0\} \cup$ Sp($u_0$). Lấy $r >0$ là một số thực sao cho mọi phần tử của Sp($u_0$)$-\{0\}$ đều có môđun $> r$. Gọi V là tập mở trong $\mathbf{C}$ gồm các số phức có trị tuyệt đối $\not =r$; gọi $f$ là hàm chỉnh hình trên V được xác định bởi $f(z) = 0$ nếu $|z|> r$ và $f(z) = 1$ nếu $|z|< r$. Nếu $K =\mathbf{C}$ (tương ứng $K =\mathbf{R}$), gọi $U'$ là tập hợp các phần tử $u$ của $\mathscr{L}(E)$ mà phổ của chúng (tương ứng phổ phức của chúng) được chứa trong V. Tập hợp $U'$ là một lân cận mở của $u_0$ trong $\mathscr{L}(E)$ và ánh xạ $u\mapsto f(u)$ từ $U'$ vào $\mathscr{L}(E)$ là chỉnh hình (I, p. 76, mệnh đề 10 và I, p. 85, n$^o13$).

Cho $u\in U'$. Tự đồng cấu $f(u)$ là phép chiếu phổ $e_0(u)$; nó giao hoán với $u$, và $u$ cảm sinh, khi chuyển qua các không gian con, một tự đẳng cấu của Ker($e_0(u)$) $($xem III, p. 53, n$^o6$).

Phép chiếu $e_0(u_0)$ có ảnh là N và hạt nhân là I (III, p. 54, mệnh đề 14); hạng của nó là $d$. Theo bổ đề 1, tập hợp U các phần tử $u\in U'$ sao cho $e_0(u)$ có hạng $d$ là một lân cận mở của $u_0$. Tập hợp U và ánh xạ $\pi :u\mapsto e_0(u)$ từ U vào $\mathscr{L}(E)$ thỏa mãn các điều kiện (i) và (ii) của mệnh đề.

Cho $u\in U$. Vì $u$ cảm sinh một tự đẳng cấu của Ker($e_0(u)$), là một không gian con đóng đối chiều hữu hạn của E, nên tự đồng cấu $u$ là một tự đồng cấu Riesz của E (III, p. 48, mệnh đề 8), không gian lũy linh của $u$ được chứa trong ảnh của $\pi (u) =e_0(u)$, và có chiều $\leqslant d$.

### 4. Đồng chuẩn của một ánh xạ tuyến tính liên tục

Cho E và F là các không gian chuẩn, $u: E\rightarrow F$ một ánh xạ tuyến tính liên tục, N là hạt nhân của $u$ và I là ảnh của nó. Ký hiệu $p$ là toàn cấu chính tắc từ E lên $E/N$ và $i$ là đơn ánh chính tắc từ I vào F. Gọi $\widetilde{u}$ là ánh xạ tuyến tính song ánh từ $E/N$ lên I sao cho $u=i\circ \widetilde{u}\circ p$. Không gian vectơ $E/N$ được trang bị chuẩn thương, nghĩa là

(2) $\|y\|=$ inf$_{x\in\overset{-1}{p}(y)}\|x\|$

với mọi $y\in E/N$. Ánh xạ $\widetilde{u}$ là liên tục và $\|u\|=\|\widetilde{u}\|$, do đó (3) $\|u\|=$ sup$_{y\in E/N}\frac{\|\widetilde{u}(y)\|}{\|y\|}$,

$y\not =0$

cận trên nhỏ nhất được lấy trong $\overline{\mathbf{R}}_+$. Số

(4) $((u)) =$ inf$_{y\in E/N}\frac{\|\widetilde{u}(y)\|}{\|y\|}$,

$y\not =0$

cận dưới lớn nhất được lấy trong $\overline{\mathbf{R}}_+$. Do đó

$$
((u))\|y\|\leqslant \|\widetilde{u}(y)\|\leqslant \|u\| \|y\| \tag{5}
$$

với mọi phần tử $y$ của $E/N$. Đặt $v=i\circ \widetilde{u}$. Khi đó $u=v\circ p$ và

(6) $((u)) =$ inf$_{y\in E/N}\frac{\|v(y)\|}{\|y\|}=$ inf$_{y\in E/N}\|v(y)\|$.

$y\not =0\|y\|=1$

Khi $u$ là ánh xạ không, không gian $E/N$ thu về 0 và ta có $((u)) = +\infty$ và $\|u\|= 0$. Khi $u\not = 0$, từ (3) và (4) suy ra các bất đẳng thức

$$
0\leqslant ((u))\leqslant \|u\|<+\infty \tag{7}
$$

Khi $u$ là đơn ánh, ta có

(8) $((u)) =$ inf$_{xx\in\not=0E}\frac{\|u(x)\|}{\|x\|}$,

và, với mọi $x\in E$, ta có

$$
((u))\|x\|\leqslant \|u(x)\|\leqslant \|u\| \|x\| \tag{9}
$$

Ký hiệu $j$ là đơn ánh chính tắc từ không gian chuẩn F vào bổ sung đầy đủ của nó $\widehat{F}$. Ta có $((u)) = ((j\circ u))$.

#### Nhận xét {#ts-iii-s4-n4-rem-1 .statement tag=02SR}

Theo định nghĩa, để có $((u))>0$, điều kiện cần và đủ là ánh xạ tuyến tính song ánh $\widetilde{u}$ là song liên tục, nghĩa là $u$ là một cấu xạ ngặt (TG, III, p. 16). Khi đó ta có

$$
((u)) =\|\widetilde{u}^{-1}\|^{-1} \tag{10}
$$

#### Bổ đề 2 {#ts-iii-s4-lem-2 .statement tag=02SS}

Cho $c$ là một số thực. Nếu $c <((u))$, thì với mọi phần tử $z\in$ Im($u$), tồn tại một phần tử $x$ của E sao cho $u(x) =z$ và $c\|x\|\leqslant \|z\|$. Ngược lại, nếu với mọi $z\in$ Im($u$) tồn tại $x\in E$ sao cho $u(x) =z$ và $c\|x\|\leqslant \|z\|$, thì $c\leqslant ((u))$.

Điều này là một hệ quả của các công thức (2) và (5) và của định nghĩa đối chuẩn của $u$.

#### Mệnh đề 6 {#ts-iii-s4-prop-6 .statement tag=02ST}

Cho E và F là các không gian chuẩn và $u\in \mathscr{L}(E; F)$. Ký hiệu B là tập hợp các phần tử của E có chuẩn $<1$. Đặt

$P =u(E)-u(B),Q =u(E)$ - $(\overline{u(B)}\cap u(E))$.

Đối chuẩn của $u$ bằng khoảng cách từ 0 đến P trong F. Nếu không gian chuẩn E là đầy đủ hoặc nếu $u$ là một cấu xạ ngặt, thì đối chuẩn của $u$ bằng khoảng cách từ 0 đến Q trong F.

Cho N là hạt nhân của $u$; cho $p: E\rightarrow E/N$ là toàn cấu chính tắc và cho $v: E/N\rightarrow F$ là ánh xạ suy ra từ $u$ bằng cách chuyển qua thương. Tập hợp $p(B)$ là tập hợp các phần tử của $E/N$ có chuẩn $<1$. Ta có

$$
P =u(E)-u(B) =v(E/N)-v(p(B)) =v((E/N)-p(B))
$$

vì ánh xạ $v$ là đơn ánh. Nói cách khác, P gồm các phần tử của F có dạng $v(y)$ với $y\in E/N$ và $\|y\|\geqslant 1$. Ký hiệu $d_P$ là khoảng cách từ 0 đến P trong F. Ta có

$d_P=$ inf$_{y\|\in yE\|\geqslant/N1}\|v(y)\|=$ inf$_{y\|\in yE\|=1/N}\|v(y)\|= ((u))$ theo (6).

Giả sử rằng $u$ là một cấu xạ ngặt. Cho $\varepsilon  >0$. Tập $\varepsilon u(B)$ là một lân cận của 0 trong $u(E)$. Bao đóng của $u(B)$ trong $u(E)$ bằng $\overline{u(B)}\cap u(E)$. Nó được chứa trong tập $u(B) +\varepsilon u(B)$, tập này bằng $(1 +\varepsilon )u(B)$ vì $u(B)$ là lồi. Do đó ta có $(1 +\varepsilon )P\subset Q\subset P$, và khoảng cách $d_Q$ từ 0 đến Q trong F thỏa mãn các bất đẳng thức $d_P\leqslant d_Q\leqslant (1 +\varepsilon )d_P$. Vì điều này đúng với mọi $\varepsilon  >0$, ta có $d_Q=d_P= ((u))$.

Giả sử rằng $u$ không phải là một cấu xạ ngặt, nhưng không gian chuẩn E là đầy đủ. Khi đó $((u)) = 0$ (nhận xét trên). Bao đóng của $u(B)$ trong $u$(E), bằng $\overline{u(B)}\cap u$(E), không phải là một lân cận của 0 trong $u(E)$ (EVT, I, p. 17, th. 1). Khi đó tồn tại các điểm của Q tùy ý gần 0, do đó $d_Q= 0 = ((u))$.

#### Mệnh đề 7 {#ts-iii-s4-prop-7 .statement tag=02SU}

Cho E là một không gian Banach và F là một không gian chuẩn. Ánh xạ $u\mapsto ((u))$ từ $\mathscr{L}(E; F)$ vào $\overline{\mathbf{R}}$ là nửa liên tục trên.

Cho $u\in \mathscr{L}(E; F)$. Ta phải chứng minh rằng với mọi số thực $c >((u))$, tập các phần tử $v\in \mathscr{L}(E; F)$ sao cho $((v))< c$ là một lân cận của $u$. Ký hiệu B là tập các phần tử của E có chuẩn $<1$. Theo Mệnh đề 6, tồn tại $y\in E$ sao cho $u(y)\notin u(B)$ và $\|u(y)\|< c$. Khoảng cách $d$ từ $u(y)$ đến tập đóng $u(B)$ là dương ngặt. Tập V gồm các phần tử $v$ của $\mathscr{L}(E; F)$ thỏa mãn các hệ thức $\|v(y)\|< c$ và $\|u-v\|(1 +\|y\|)< d$ là một lân cận của $u$ trong $\mathscr{L}(E; F)$. Cho $v\in V$. Với mọi $x\in B$, ta có

$$
d\leqslant \|u(y)-u(x)\|\leqslant \|v(y)-v(x)\|+\|u-v\|(\|y\|+\|x\|)
$$

$$
<\|v(y)-v(x)\|+d
$$

Do đó $v(y)$ không thuộc $v$(B), và ta có $((v))\leqslant \|v(y)\|< c$ theo Mệnh đề 6.

#### Mệnh đề 8 {#ts-iii-s4-prop-8 .statement tag=02SV}

Cho E là một không gian Banach, F một không gian chuẩn. Với mọi $u\in \mathscr{L}(E; F)$, ta có $((u)) = ((^tu))$.

Ký hiệu $j$ là đơn ánh chính tắc của không gian chuẩn F vào không gian đầy đủ $\widehat{F}$ của nó. Ta có $((u)) = ((j\circ u))$. Vì ánh xạ tuyến tính $^tj: (\widehat{F})'\rightarrow F'$ là song ánh và đẳng cự, tương tự ta cũng có $((^tu)) = ((^t(j\circ u)))$. Vậy nên chỉ cần chứng minh mệnh đề khi không gian chuẩn F là đầy đủ, và ta sẽ giả thiết điều đó trong phần còn lại của chứng minh.

Nếu $u$ bằng không, ta có $((u)) = ((^tu)) = +\infty$. Nếu $u$ không phải là một cấu xạ ngặt, thì $^tu$ cũng không phải như vậy (EVT, IV, p. 29, Hệ quả 3), và ta có $((u)) = ((^tu)) = 0$.

Từ đây giả sử rằng $u$ là một cấu xạ ngặt khác không. Ký hiệu N là hạt nhân của $u$ và I là ảnh của nó, và xét phân tích chính tắc của $u:$

$$
E\overset{p}{\longrightarrow}E/N\longrightarrow^vI\longrightarrow^iF
$$

Hạt nhân của $^tu$ là trực giao $I^{\circ}$ của I trong $F'$ (EVT, IV, p. 27, Mệnh đề 2), và $^ti$ xác định bằng cách chuyển qua thương một đẳng cự $\iota$ từ $F'/I^{\circ}$ lên $I'$ (EVT, IV, p. 9, Mệnh đề 10). Hơn nữa, $^tp$ xác định một đẳng cự $\pi$ từ $(E/N)'$ lên trực giao $N^{\circ}$ của N trong $E'$ (EVT, IV, p. 8, Mệnh đề 9). Do đó phân tích chính tắc của $^tu$ là

$$
F'\longrightarrow F'/I^{\circ}\longrightarrow^{v'}N^{\circ}\longrightarrow E'
$$

trong đó $v'=\pi \circ^tv\circ \iota$. Khi đó ta có

$$
\|(v')^{-1}\|=\|(^tv)^{-1}\|=\|^t(v^{-1})\|=\|v^{-1}\|
$$

(EVT, IV, p. 7, prop. 8), do đó $((u)) = ((^tu))$ sau công thức (10).

### 5. Các không gian con vectơ hữu hạn chiều của một không gian chuẩn

Mệnh đề sau sẽ được chứng minh trong TA, sẽ xuất hiện, như một hệ quả của định lý Borsuk–Ulam.

#### Định lý 3 {#ts-iii-s4-thm-3 .statement tag=02SW}

Cho $n$ là một số nguyên dương, V là một không gian vectơ chuẩn thực có chiều $n+ 1$ và W là một không gian con vectơ của V có chiều $n$. Gọi S là mặt cầu đơn vị của V. Không tồn tại một ánh xạ liên tục $f: S\rightarrow W$ sao cho $\|f(x)-x)\|<1$ với mọi $x\in S$.

#### Định lý 4 (Krein, Krasnoselskii, Milman) {#ts-iii-s4-thm-4 .statement tag=02SX}

Cho E là một không gian chuẩn, và cho F và G là các không gian con vectơ của E. Giả sử rằng chiều của G là hữu hạn và nhỏ hơn nghiêm ngặt chiều của F. Tồn tại một phần tử của F có chuẩn bằng 1 mà khoảng cách tới G bằng 1.

Chỉ cần xét trường hợp trường K bằng $\mathbf{R}$. Gọi $n$ là chiều của G. Thay thế F bởi một không gian con vectơ của F có chiều $n+ 1$ chứa G, ta được đưa về trường hợp dim(F) $=n+ 1$. Ta lập luận bằng phản chứng, giả sử rằng kết luận của định lý không được thỏa mãn. Gọi S là mặt cầu đơn vị của F. Khi đó, với mọi $x\in S$, khoảng cách từ $x$ tới G nhỏ hơn nghiêm ngặt $\|x\|= 1$, và có thể chọn một phần tử $y(x)$ của G sao cho $\|x-y(x)\|<1$. Ký hiệu $V_x$ là tập hợp các phần tử $z$ của S sao cho $\|z-y(x)\|<1$; đó là một lân cận mở của $x$ trong S. Tồn tại một phân hoạch đơn vị liên tục hữu hạn địa phương $(\varphi_x)_{x\in S}$ trên S phụ thuộc vào phủ $(V_x)_{x\in S}$ của S (TG, IX, p. 46, prop. 3 and p. 51, prop. 6). Gọi $f: S\rightarrow G$ là ánh xạ liên tục được cho bởi

$$
f(z) =\sum_{x\in S}\varphi_x(z)y(x)
$$

với mọi $z\in S$. Cho $z\in S$. Ta có $\varphi_x(z)\geqslant 0$ với mọi $x\in S$, và tồn tại $x\in S$ sao cho $\varphi_x(z)>0$, vì $\sum_{x\in S}\varphi_x(z) = 1$, do đó

$$
\|z-f(z)\|=\|\sum_{x\in S}\varphi_x(z)(z-y(x))\|\leqslant \sum_{x\in S}\varphi_x(z)\|z-y(x)\|
$$

$$
<\sum_{x\in S}\varphi_x(z) = 1
$$

Tính chất này của $f$ mâu thuẫn với Định lý 3.

#### Mệnh đề 9 {#ts-iii-s4-prop-9 .statement tag=02SY}

Cho E và F là các không gian chuẩn, $n\in \mathbf{N}$ và $u$ là một ánh xạ tuyến tính liên tục từ E vào F mà hạt nhân có chiều $n$. Chuẩn dưới của $u$ bằng khoảng cách $d$ từ $u$ tới tập hợp các ánh xạ $v\in \mathscr{L}(E; F)$ mà hạt nhân có chiều ít nhất $n+ 1$.

Khi $u= 0$, ta có $((u)) = +\infty$ và dim(E) $=n$, do đó $d= +\infty$. Từ đây về sau giả sử rằng $u$ khác không, và vì thế $((u))<+\infty$. Cho $v$ là một phần tử của $\mathscr{L}(E; F)$ sao cho $\|u-v\|<((u))$ và hãy chứng minh rằng hạt nhân của nó có chiều $\leqslant n$. Cho $x$ là một phần tử có chuẩn 1 của Ker($v$) và $y$ là ảnh của nó trong $E/$ Ker($u$). Ta có (công thức (5) của III, p. 61)

$$
((u))\|y\|\leqslant \|u(x)\|=\|(u-v)(x)\|\leqslant \|u-v\|<((u))
$$

do đó $\|y\|<1$. Bây giờ $\|y\|$ là khoảng cách từ $x$ đến Ker($u$). Định lý 4 khi đó kéo theo rằng dim Ker($v$)$\leqslant$ dim Ker($u$) $=n$. Điều này chứng minh bất đẳng thức $((u))\leqslant d$. Bất đẳng thức đảo lại $d\leqslant ((u))$ suy ra từ bổ đề chính xác hơn sau đây.

#### Bổ đề 3 {#ts-iii-s4-lem-3 .statement tag=02SZ}

Cho $c$ là một số thực sao cho $c >((u))$. Tồn tại một ánh xạ tuyến tính liên tục $h: E\rightarrow F$, có hạng 1 và chuẩn $< c$ sao cho hạt nhân của $u+h$ chứa hạt nhân của $u$ và có chiều $n+ 1$.

Gọi $p$ là ánh xạ chính tắc của E lên $E/$ Ker($u$). Tồn tại $a\in E$ sao cho $\|p(a)\|= 1$ và $\|u(a)\|< c$ (công thức (6) của III, p. 61). Theo định lý Hahn–Banach (EVT, II, p. 24, hệ quả 2), tồn tại một dạng tuyến tính liên tục $f$ trên không gian định chuẩn $E/$ Ker($u$) sao cho $f(p(a)) = 1$ và $\|f\|= 1$. Ánh xạ tuyến tính $h:x\mapsto  -(f\circ p)(x)u(a)$ của E vào F là liên tục, có hạng 1, và ta có $\|h\|\leqslant \|f\| \|p\| \|u(a)\|< c$. Hạt nhân của ánh xạ $u+h$ chứa hạt nhân của $u$ và $a$; vì $a\not \in$ Ker($u$), nên chiều của nó do đó ít nhất là $n+ 1$. Mặt khác, ánh xạ tuyến tính $u$ cảm sinh, bằng cách chuyển qua các không gian con, một ánh xạ tuyến tính từ Ker($u+h$) vào Im($h$) có hạt nhân là Ker($u$)$\cap$ Ker($u+h$), nên dim(Ker($u+h$))$\leqslant$ dim(Ker($u$)) $+ 1$. Kết luận suy ra.

#### Hệ quả 1 {#ts-iii-s4-lem-3-cor-1 .statement tag=02T0}

Cho E và F là các không gian định chuẩn, và cho $u,v$ là các ánh xạ tuyến tính liên tục khác không từ E vào F mà các hạt nhân có cùng chiều hữu hạn. Khi đó ta có

$$
|((u))-((v))|\leqslant \|u-v\|
$$

Gọi $n$ là chiều chung của các hạt nhân của $u$ và $v$. Gọi A là tập hợp các ánh xạ tuyến tính liên tục từ E vào F mà hạt nhân có chiều $\geqslant n+ 1$. Vì $u\not = 0$, ta có dim(E) $> n$ và tập hợp A chứa 0. Theo mệnh đề 9, $((u))$ và $((v))$ lần lượt là các khoảng cách từ $u$ và từ $v$ đến tập hợp A trong $\mathscr{L}(E; F)$. Khi đó chỉ cần áp dụng công thức $|d(u,A)-d(v,A)|\leqslant \|u-v\|($xem TG, IX, p. 13).

#### Hệ quả 2 {#ts-iii-s4-lem-3-cor-2 .statement tag=02T1}

Cho E và F là các không gian Banach, và cho $u$ và $v$ là các ánh xạ tuyến tính liên tục khác không từ E vào F mà các ảnh của chúng có cùng đối chiều hữu hạn trong F. Khi đó

$$
|((u))-((v))|\leqslant \|u-v\|
$$

Cấu xạ $u$ là ngặt (III, p. 52, bổ đề 6). Hạt nhân của ánh xạ tuyến tính liên tục $^tu$ là trực giao của Im($u$), tức (Im($u$))$^{\circ}$ (EVT, IV, p. 27, mệnh đề 2), do đó dim(Ker($^tu$)) $=$ codim$_F$(Im($u$)), và tương tự dim(Ker($^tv$)) $=$ codim$_F$(Im($v$)). Vậy các hạt nhân của $^tu$ và $^tv$ có cùng số chiều hữu hạn. Vì

$$
\|^tu-^tv\|=\|u-v\|,((^tu)) = ((u)),((^tv)) = ((v))
$$

(EVT, IV, p. 7, mệnh đề 8 và mệnh đề 8 của III, p. 63), mệnh đề suy ra từ hệ quả 1, áp dụng cho $^tu$ và $^tv$.

### 6. Nhiễu của các ánh xạ tuyến tính liên tục đơn ánh hoặc toàn ánh

Trong số này, các quy ước sau đây được chấp nhận: nếu E là một không gian vectơ hữu hạn chiều, dim(E) ký hiệu chiều của nó; nếu E là một không gian vectơ vô hạn chiều, đặt dim(E) $= +\infty  \in \overline{\mathbf{R}}$. Nếu $u$ là một ánh xạ tuyến tính mà hạt nhân hoặc đối hạt nhân có số chiều hữu hạn, đặt ind($u$) $=$ dim Coker($u$)$-$ dim Ker($u$), phép tính được thực hiện trong $\overline{\mathbf{R}}$.

Cho E và F là các không gian định chuẩn. Ta ký hiệu bởi $\mathscr{M}(E; F)$ tập hợp các cấu xạ ngặt đơn ánh từ E vào F, và bởi $\mathscr{Q}\mathscr{M}(E; F)$ tập hợp các cấu xạ ngặt từ E vào F mà hạt nhân có số chiều hữu hạn.

#### Mệnh đề 10 {#ts-iii-s4-prop-10 .statement tag=02T2}

Cho E và F là các không gian định chuẩn. Tập $\mathscr{M}(E; F)$ là mở trong $\mathscr{L}(E; F)$. Nó là phần trong của tập các ánh xạ trong $\mathscr{L}(E; F)$ mà đơn ánh.

Cho A là tập các ánh xạ tuyến tính liên tục đơn ánh từ E vào F. Để một ánh xạ $u\in A$ là một cấu xạ ngặt, điều kiện cần và đủ là đối chuẩn của nó $((u))$ dương ngặt (III, p. 62, nhận xét). Mà $((u))$ là khoảng cách từ $u$ đến phần bù của A trong $\mathscr{L}(E; F)$(III, p. 65, mệnh đề 9). Mệnh đề được suy ra.

#### Mệnh đề 11 {#ts-iii-s4-prop-11 .statement tag=02T3}

Cho E và F là các không gian Banach. Tập $\mathscr{Q}\mathscr{M}(E; F)$ là mở trong $\mathscr{L}(E; F)$. Nó là phần trong của tập các ánh xạ trong $\mathscr{L}(E; F)$ mà hạt nhân có số chiều hữu hạn.

Cho A là tập các ánh xạ tuyến tính liên tục từ E vào F mà hạt nhân có số chiều hữu hạn.

Cho $u$ là một phần tử của $\mathscr{Q}\mathscr{M}(E; F)$. Khi đó $((u))>0$(III, p. 62, nhận xét). Khi ấy mọi phần tử $v\in \mathscr{L}(E; F)$ mà khoảng cách đến $u$ là $<((u))$ đều thuộc A (III, p. 65, mệnh đề 9), nên $u$ là một điểm trong của A.

Ngược lại, giả sử $u$ là một phần tử của A không phải là một cấu xạ ngặt. Ta có $((u)) = 0 ($III, p. 62, Nhận xét). Gọi $v$ là một phần tử của $\mathscr{L}(E; F)$ sai khác với $u$ bởi một ánh xạ tuyến tính hạng hữu hạn; theo Hệ quả 1 của III, p. 40, cấu xạ $v$ không thể là ngặt với ảnh đóng; vì một cấu xạ ngặt từ E vào F có ảnh đóng trong F (EVT, IV, p. 28, Định lý 1), điều đó có nghĩa là $v$ không phải là một cấu xạ ngặt. Do đó $((v)) = 0$. Gọi $\varepsilon$ là một số thực $>0$. Theo điều đã nói ở trên, Bổ đề 3 của III, p. 66 cho phép ta xây dựng bằng quy nạp một dãy $(u_m)_{m\in\mathbf{N}}$ các phần tử của $\mathscr{L}(E; F)$ thỏa mãn các điều kiện sau:

(i) Ta có $u_0=u$;

(ii) Với mọi $m\geqslant 0,u_{m+1}-u_m$ là một ánh xạ tuyến tính liên tục hạng 1 và chuẩn $\leqslant 2^{-m-1}\varepsilon$;

(iii) Với mọi $m\geqslant 0$, hạt nhân của $u_m$ có chiều $n+m$ và được chứa trong hạt nhân của $u_{m+1}$.

Dãy $(u_m)$ là một dãy Cauchy trong không gian Banach $\mathscr{L}(E; F)$. Gọi $u'$ là giới hạn của nó. Hạt nhân của $u'$ chứa hạt nhân của $u_m$ với mọi $m\geqslant 0$; nó là vô hạn chiều. Vì

$$
\|u'-u\|\leqslant \sum_{m=0}^{\infty}\|u_{m+1}-u_m\|\leqslant \varepsilon \sum_{m=0}^{\infty}2^{-m-1}=\varepsilon
$$

nên khoảng cách từ $u$ đến phần bù của A nhỏ hơn $\varepsilon$. Vì điều này đúng với mọi $\varepsilon  >0$, suy ra $u$ không phải là một điểm trong của A.

#### Mệnh đề 12 {#ts-iii-s4-prop-12 .statement tag=02T4}

Cho E và F là các không gian Banach và $u$ là một phần tử của $\mathscr{Q}\mathscr{M}(E; F)$. Mọi $v\in \mathscr{L}(E; F)$ sao cho $\|v-u\|<((u))$ đều thuộc $\mathscr{Q}\mathscr{M}(E; F)$ và thỏa mãn các hệ thức

dim Ker($v$)$\leqslant$ dim Ker($u$),

dim Coker($v$)$\leqslant$ dim Coker($u$),

ind($v$) $=$ ind($u$).

Vì $u$ là ngặt, ta có $((u))>0$. Gọi B là quả cầu mở tâm $v$ và bán kính $((u))$ trong $\mathscr{L}(E; F)$. Với mọi $v\in$ B, ta có dim Ker($v$)$\leqslant$ dim Ker($u$)(III, p. 65, mệnh đề 9) và $v\in \mathscr{Q}\mathscr{M}(E; F)$ (mệnh đề 11).

Với $r\in \mathbf{Z}\cup  \{+\infty \}$, ta ký hiệu bởi $B_r$ tập hợp các phần tử $v\in B$ sao cho ind($v$) $=r$. Nếu $r\in \mathbf{Z}$, tập hợp $B_r$ là tập hợp các ánh xạ Fredholm từ E vào F có chỉ số $r$ và thuộc B (III, p. 52, Mệnh đề 11); nó mở trong B theo Định lý 1 của III, p. 58.

Ta sẽ chứng minh rằng các tập hợp $B_r$ là đóng trong B. Cho $v\in B$ là một điểm dính của $B_r$. Vì các tập hợp $B_s$, với $s\in \mathbf{Z}$, là mở trong B và rời nhau từng đôi một, nên ta có $v\in B_r$ hoặc $v\in B_{+\infty}$.

Giả sử $v\in B_{+\infty}$. Gọi $n$ là chiều của Ker($u$). Chọn một không gian con vectơ T của F có chiều $r+ 2n+ 1$ sao cho giao của nó với Im($v$) chỉ còn 0, và một phần bù tôpô S của Ker($v$) trong E (III, p. 55, Mệnh đề 1). Xét ánh xạ tuyến tính liên tục $f: (s, t)\mapsto v(s) +t$ từ $S\times T$ vào F. Nó là đơn ánh. Ánh xạ tuyến tính $v$ là một cấu xạ ngặt vì $v$ thuộc $B\subset \mathscr{Q}\mathscr{M}(E; F)$. Do đó ảnh của $v$ là đóng (EVT, IV, p. 28, Định lý 1). Theo Mệnh đề 1 của III, p. 39, hạn chế của $v$ lên S là một cấu xạ ngặt có ảnh đóng từ S vào F, và $f$ là một cấu xạ ngặt có ảnh đóng từ $S\times T$ vào F.

Theo Mệnh đề 10, tồn tại một lân cận U của $v$ trong B sao cho, với mọi $w\in U$, ánh xạ tuyến tính $(s, t)\mapsto w(s) +t$ từ $S\times T$ vào F là đơn ánh. Lấy $w$ là một phần tử của U. Khi đó Ker($w$)$\cap S =\{0\}$, nên $w$ xác định, bằng cách hạn chế rồi chuyển qua thương, một ánh xạ tuyến tính đơn ánh từ Ker($w$) vào $E/S$, điều này kéo theo Ker($w$) có chiều nhiều nhất là $n$. Ta cũng có $w(S)\cap T =\{0\}$, do đó

codim$_F$(Im($w$))$\geqslant$ dim(T) $-$ codim$_E(S) =r+n+ 1$,

điều này suy ra ind($w$)$\geqslant r+ 1$ và mâu thuẫn với giả thiết rằng $v$ là điểm dính của $B_r$.

Nếu $r$ là một phần tử của $\mathbf{Z}$ sao cho $B_r$ khác rỗng, thì $B_r= B$ vì $B_r$ là mở và đóng trong B và B là liên thông. Nếu $B_r$ rỗng với mọi $r\in \mathbf{Z}$, thì ind($v$) $= +\infty$ với mọi $v\in B$. Do đó ánh xạ $v\mapsto$ ind($v$) là hằng trên B. Sau hết, với mọi $v\in B$, ta có

dim Coker($v$) $=$ ind($v$) $+$ dim Ker($v$)

$\leqslant$ ind($u$) $+$ dim Ker($u$) $=$ dim Coker($u$).

Điều này kết thúc chứng minh.

#### Hệ quả 1 {#ts-iii-s4-prop-12-cor-1 .statement tag=02T5}

Các hàm được xác định bởi $u\mapsto$ dim Ker($u$) và bởi $u\mapsto$ dim Coker($u$) trên $\mathscr{Q}\mathscr{M}(E; F)$ là nửa liên tục trên. Hàm $u\mapsto$ ind($u$) là địa phương hằng trên $\mathscr{Q}\mathscr{M}(E; F)$.

#### Hệ quả 2 {#ts-iii-s4-prop-12-cor-2 .statement tag=02T6}

Hàm $u\mapsto$ dim Coker($u$) là địa phương hằng trên tập $\mathscr{M}(E; F)$ các cấu xạ đơn ánh ngặt từ E vào F.

Thật vậy, ta có dim Coker($u$) $=$ ind($u$) với $u\in \mathscr{M}(E; F)$.

#### Bổ đề 4 {#ts-iii-s4-lem-4 .statement tag=02T7}

Cho E và F là các không gian Banach. Để một phần tử $u$ của $\mathscr{L}(E; F)$ là một cấu xạ ngặt từ E vào F, điều kiện cần và đủ là $^tu$ là một cấu xạ ngặt từ $F'$ vào $E'$. Trong trường hợp đó, ta có dim Coker($^tu$) $=$ dim Ker($u$) và dim Ker($^tu$) $=$ dim Coker($u$).

Để $u$ là một cấu xạ ngặt, điều kiện cần và đủ là $^tu$ cũng là một cấu xạ như vậy (EVT, IV, p. 29, hệ quả 3); trong trường hợp đó, ảnh của $u$ là đóng (EVT, IV, p. 28, định lý 1) và không gian vectơ Ker($^tu$) (resp. Coker($^tu$)) đẳng cấu chính tắc với đối ngẫu của không gian định chuẩn Coker($u$) (resp. Ker($u$)) theo EVT, IV, p. 27, mệnh đề 2. Bổ đề được suy ra.

Cho E và F là các không gian Banach. Ký hiệu $\mathscr{E}(E; F)$ là tập hợp các ánh xạ tuyến tính liên tục toàn ánh từ E vào F và $\mathscr{Q}\mathscr{E}(E; F)$ là tập hợp các ánh xạ tuyến tính liên tục từ E vào F có ảnh đối chiều hữu hạn. Mọi phần tử của $\mathscr{Q}\mathscr{E}(E; F)$ đều là một cấu xạ ngặt với ảnh đóng (III, p. 52, bổ đề 6). Suy ra từ bổ đề 4 rằng $\mathscr{E}(E; F)$ và $\mathscr{Q}\mathscr{E}(E; F)$ lần lượt là các ảnh nghịch của $\mathscr{M}(F'; E')$ và $\mathscr{Q}\mathscr{M}(F'; E')$ dưới ánh xạ liên tục $u\mapsto^tu$ từ $\mathscr{L}(E; F)$ vào $\mathscr{L}(F'; E')$.

#### Mệnh đề 13 {#ts-iii-s4-prop-13 .statement tag=02T8}

Cho E và F là các không gian Banach. Các tập hợp $\mathscr{E}(E; F)$ và $\mathscr{Q}\mathscr{E}(E; F)$ là mở trong $\mathscr{L}(E; F)$. Chính xác hơn, nếu $u$ là một phần tử của $\mathscr{Q}\mathscr{E}(E; F)$ và $v$ là một phần tử của $\mathscr{L}(E; F)$ sao cho $\|v-u\|<((u))$, thì $v\in \mathscr{Q}\mathscr{E}(E; F)$ và

dim Ker($v$)$\leqslant$ dim Ker($u$), dim Coker($v$)$\leqslant$ dim Coker($u$),

ind($v$) $=$ ind($u$).

Ta đã thấy ở trên rằng $^tu\in \mathscr{Q}\mathscr{M}(F'; E')$. Hơn nữa, với mọi phần tử $v$ của $\mathscr{L}(E; F)$, ta có $\|^tv-^tu\|=\|v-u\|$ và $((^tu)) = ((u))$ (EVT, IV, p. 7, prop. 8 and III, p. 63, prop. 8). Theo mệnh đề 12, suy ra từ các quan hệ này rằng nếu $\|v-u\|<((u))$, thì $^tv$ thuộc $\mathscr{Q}\mathscr{M}(F'; E')$ và ta có các bất đẳng thức

dim Ker($^tv$)$\leqslant$ dim Ker($^tu$), dim Coker($^tv$)$\leqslant$ dim Coker($^tu$)

cũng như đẳng thức ind($^tv$) $=$ ind($^tu$). Khi đó mệnh đề suy ra từ bổ đề 4.

#### Hệ quả 1 {#ts-iii-s4-prop-13-cor-1 .statement tag=02T9}

Các hàm được xác định bởi $u\mapsto$ dim Ker($u$) và bởi $u\mapsto$ dim Coker($u$) trên $\mathscr{Q}\mathscr{E}(E; F)$ là nửa liên tục trên. Hàm $u\mapsto$ ind($u$) là hằng địa phương trên $\mathscr{Q}\mathscr{E}(E; F)$.

#### Hệ quả 2 {#ts-iii-s4-prop-13-cor-2 .statement tag=02TA}

Hàm được xác định bởi $u\mapsto$ dim Ker($u$) là hằng địa phương trên $\mathscr{E}(E; F)$.

Thật vậy, ta có dim Ker($u$) $=-$ ind($u$) với mọi $u\in \mathscr{E}(E; F)$.

## BÀI TẬP {#ts-iii-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
