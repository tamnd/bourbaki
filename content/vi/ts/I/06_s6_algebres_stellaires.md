---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 6
section_title: Algèbres stellaires
lang: vi
source: ts-i-ii-fr
book_pages: TS I.95-TS I.127, TS I.180-TS I.187
pdf_pages: 0108-0140, 0193-0200
extraction: native
subsections:
    - "no": 1
      title: Involutions semi-linéaires
      page: 95
      pdf_page: 108
    - "no": 2
      title: Algèbres involutives
      page: 96
      pdf_page: 109
    - "no": 3
      title: Algèbres normées involutives
      page: 100
      pdf_page: 113
    - "no": 4
      title: Algèbres stellaires
      page: 102
      pdf_page: 115
    - "no": 5
      title: Algèbres stellaires commutatives
      page: 107
      pdf_page: 120
    - "no": 6
      title: Calcul fonctionnel dans les algèbres stellaires unifères
      page: 109
      pdf_page: 122
    - "no": 7
      title: Applications du calcul fonctionnel
      page: 112
      pdf_page: 125
    - "no": 8
      title: Calcul fonctionnel dans une algèbre non unifère
      page: 114
      pdf_page: 127
    - "no": 9
      title: Éléments positifs dans les algèbres stellaires
      page: 115
      pdf_page: 128
    - "no": 10
      title: Unités approchées dans les algèbres stellaires
      page: 120
      pdf_page: 133
    - "no": 11
      title: Quotient par un idéal bilatère fermé
      page: 122
      pdf_page: 135
    - "no": 12
      title: Algèbre stellaire enveloppante d’une algèbre de Banach involutive
      page: 123
      pdf_page: 136
    - "no": 13
      title: Algèbre stellaire d’un groupe localement compact
      page: 125
      pdf_page: 138
statements: 94
exercises: 32
content_sha256: c7c84a58ed35291da363fe0855bb4655c9fa387cd6d6d1a79ec9b7798275a72a
translated_from: content/en-mt/ts/I/06_s6_algebres_stellaires.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 418c15132f405d471cda0725f703ed4fefdfc3b5f9396eba1fce2ac8cbf4f2cb
translation_model: gpt-5.4
translation_run: translate-vi-e47d6fa4
glossary_version: 34
glossary_terms_sha256: 1f4dfbf33805611fe01e663112861fe9310d12a467ae42023b9f10ff49058ab7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. ĐẠI SỐ STELLAR

Trong đoạn này, trường cơ sở là $\mathbf{C}$.

### 1. Các phép đối hợp nửa tuyến tính

Cho E là một không gian vectơ phức. Một phép đối hợp nửa tuyến tính trên E là một ánh xạ tuyến tính trên $\mathbf{R}$ từ E vào E sao cho $u\circ u=$ Id$_E$ và $u(\lambda x) =\lambda u(x)$ với mọi $\lambda \in \mathbf{C}$ và mọi $x\in E$. Khi đó ta ký hiệu bởi $E^u$ không gian con vectơ thực của E gồm các phần tử $x\in E$ sao cho $u(x) =x$.

#### Bổ đề 1 {#ts-i-s6-lem-1 .statement tag=02CI}

Cho E là một không gian vectơ phức và $u$ là một phép đối hợp nửa tuyến tính trên E. Cho $x\in E$; đặt

$$
x_1=\frac{1}{2}(x+u(x)),x_2=\frac{1}{2i}(x-u(x))
$$

Cặp $(x_1, x_2)$ là phần tử duy nhất của $E^u\times E^u$ sao cho $x=x_1+ix_2$.

Các phần tử $x_1$ và $x_2$ thỏa mãn $x_1+ix_2=x$ và thuộc $E^u$ vì $u(u(x)) =x$. Ngược lại, nếu $y_1$ và $y_2$ trong $E^u$ thỏa mãn $x=y_1+iy_2$, thì suy ra $u(x) =u(y_1) +u(iy_2) =y_1-iy_2$, do đó

$$
y_1=\frac{1}{2}(x+u(x)) =x_1,iy_2=\frac{1}{2}(x-u(x)) =ix_2
$$

#### Mệnh đề 1 {#ts-i-s6-prop-1 .statement tag=02CJ}

Cho $E_1$ và $E_2$ là các không gian vectơ phức, và cho $u_1$ và $u_2$ lần lượt là các phép đối hợp nửa tuyến tính trên $E_1$ và $E_2$. Cho $f$ là một ánh xạ tuyến tính từ $E_1$ vào $E_2$. Khi đó $f\circ u_1=u_2\circ f$ khi và chỉ khi $f(E^{u_1}_1)\subset E^{u_2}_2$.

Nếu $f\circ u_1=u_2\circ f$, ta ngay lập tức được $f(E^{u_1}_1)\subset E^{u_2}_2$. Ngược lại, giả sử điều kiện này được thỏa mãn. Cho $x\in$ E. Viết $x=x_1+ix_2$ với $(x_1, x_2)\in E^{u_1}_1\times E^{u_1}_1$ (bổ đề trên). Khi đó ta có $f(u_1(x)) =f(x_1)-if(x_2)$ và $u_2(f(x)) =u_2(f(x_1))-iu_2(f(x_2)) =$ $f(x_1)-if(x_2) =f(u_1(x))$.

### 2. Các đại số có đối hợp

#### Định nghĩa 1 {#ts-i-s6-def-1 .statement tag=02CK}

Cho A là một đại số trên $\mathbf{C}$. Một đối hợp trong A được gọi là một ánh xạ $x\mapsto x^*$ từ A vào A sao cho:

$$
(x^*)^*=x,(x+y)^*=x^*+y^*,(\lambda x)^*=\lambda x^*
$$

$$
(xy)^*=y^*x^*
$$

với mọi $x, y\in A$ và $\lambda \in \mathbf{C}$. Một đại số trên $\mathbf{C}$ được trang bị một đối hợp được gọi là một đại số có đối hợp.

Đặc biệt, một đối hợp trên A là một đẳng cấu của vành A lên vành đối $A^{\circ}$.

Cho A là một đại số có phép đối hợp. Người ta gọi $x^*$ là liên hợp của $x$. Một tập con của A ổn định đối với phép đối hợp được gọi là tự liên hợp. Nếu A có một phần tử đơn vị $e$, thì ta có $e^*=e$; người ta nói rằng $(A, e)$ là một đại số có đơn vị có phép đối hợp. Một phần tử $u$ của một đại số có đơn vị có phép đối hợp được gọi là unita nếu $uu^*=u^*u=e$, nói cách khác nếu $u$ khả nghịch và nếu nghịch đảo của nó là $u^*$.

Một phần tử $x\in A$ được gọi là Hermit nếu $x=x^*$ và chuẩn tắc nếu $xx^*=$ $x^*x$. Thuật ngữ này khái quát thuật ngữ của A, IX, § 7, No.$^o3$. Mọi phần tử Hermit đều chuẩn tắc, mọi phần tử unita đều chuẩn tắc. Tập $A_h$ các phần tử Hermit của A là một không gian con vectơ thực của A. Nếu $x$ và $y$ là Hermit và giao hoán, thì ta có $(xy)^*$ = $y^*x^*=yx=xy$, do đó $xy$ là Hermit. Với mọi $x\in A$, các phần tử $xx^*$ và $x^*x$ của A là Hermit.

Nếu $A =\mathbf{C}$ được trang bị phép đối hợp $z\mapsto \overline{z}$, thì ta có $A_h=\mathbf{R}$.

#### Bổ đề 2 {#ts-i-s6-lem-2 .statement tag=02CL}

Cho A là một đại số có phép đối hợp và $x\in A$. Các phần tử

$$
x_1=\frac{1}{2}(x+x^*),x_2=\frac{1}{2i}(x-x^*)
$$

là Hermit và thỏa mãn $x=x_1+ix_2$. Nếu $x=y_1+iy_2$ với $y_1$ và $y_2$ Hermit, thì $x_1=y_1$ và $x_2=y_2$. Hơn nữa, phần tử $x$ là chuẩn tắc khi và chỉ khi $x_1$ và $x_2$ giao hoán.

Hai khẳng định đầu suy ra từ Bổ đề 1 của I, p. 95. Ta tính được rằng $xx^*-x^*x= 2i(x_2x_1-x_1x_2)$, do đó $x$ là chuẩn tắc khi và chỉ khi $x_1$ và $x_2$ giao hoán.

Cho A là một đại số có đơn vị có phép đối hợp. Để $x\in A$ khả nghịch, điều kiện cần và đủ là $x^*$ cũng vậy, và khi đó ta có $(x^*)^{-1}= (x^{-1})^*$. Vì $(x-\lambda e)^*=x^*-\lambda e$ với mọi $\lambda \in \mathbf{C}$, suy ra Sp$_A(x^*) =$ Sp$_A(x)$.

Cho A là một đại số có phép đối hợp và $\widetilde{A}$ là đại số suy ra từ A bằng phép nối thêm một phần tử đơn vị. Trong $\widetilde{A}$ tồn tại duy nhất một phép đối hợp kéo dài phép đối hợp của A, được cho bởi $(\lambda , x)^*= (\lambda , x^*)$ với $\lambda \in \mathbf{C}$ và $x\in A$. Nếu $x\in A$, thì ta có Sp$'_A(x^*) =$ Sp$'_A(x)$.

Cho A và B là các đại số có đối hợp. Bởi một cấu xạ của A vào B, ta hiểu là một cấu xạ đại số $\varphi$ của A vào B sao cho $\varphi (x^*) =\varphi (x)^*$ với mọi $x$ và $y$ thuộc A. Ánh xạ đồng nhất của A là một cấu xạ của các đại số có đối hợp. Nếu C là một đại số có đối hợp và $\pi : B\rightarrow C$ là một cấu xạ của các đại số có đối hợp, thì $\pi \circ \varphi$ là một cấu xạ của các đại số có đối hợp. Nếu $\varphi$ là một đẳng cấu đại số, thì $\varphi^{-1}$ là một cấu xạ của các đại số có đối hợp, và khi đó người ta nói rằng $\varphi$ là một đẳng cấu của các đại số có đối hợp.

Theo mệnh đề 1 của I, p. 95, nếu A và B là các đại số có đối hợp, một cấu xạ đại số $\varphi$ của A vào B là một cấu xạ của các đại số có đối hợp khi và chỉ khi $\varphi (A_h)\subset B_h$. Bởi một đại số con có đối hợp của A, ta hiểu là một đại số con tự liên hợp. Tâm của A là một đại số con có đối hợp. Nếu $A_1$ là một iđêan hai phía tự liên hợp của A, đối hợp của A xác định, bằng cách chuyển qua thương, một đối hợp trong đại số $A/A_1$, và ánh xạ chính tắc của A lên $A/A_1$ là một cấu xạ của các đại số có đối hợp.

Cho A là một đại số có đối hợp. Căn của A bằng căn của đại số đối (A, VIII, p. 431, mệnh đề 7), và do đó tự liên hợp.

Cho A là một đại số có đối hợp. Nếu $M\subset A$ là tự liên hợp, thì hoán tập $M'$ của nó là một đại số con có đối hợp của A. Nếu $x\in A$, đối giao hoán tử kép của $\{x, x^*\}$ là một đại số con có đối hợp chứa $x$ và $x^*$, và đại số con này giao hoán khi và chỉ khi $x$ là chuẩn tắc (n$^o5$ của I, p. 5).

#### Nhận xét {#ts-i-s6-n2-rem-1 .statement tag=02CM}

Cho A là một đại số có đối hợp và B là một đại số con có đối hợp giao hoán cực đại của A. Khi đó B là một đại số con giao hoán cực đại. Đặc biệt, nếu A có đơn vị, thì đại số B là đầy.

Thật vậy, cho $x\in A$ là một phần tử giao hoán với B. Khi đó $x^*$ giao hoán với B. Viết $x=x_1+ix_2$ với $x_1$ và $x_2$ Hermit; các phần tử $x_1$ và $x_2$ giao hoán với B (bổ đề 2). Do đó đại số con của A sinh bởi B và $x_1$ là giao hoán và có đối hợp. Vì vậy, nó bằng B, nên $x_1\in B$. Tương tự, ta có $x_2\in B$, và do đó cuối cùng $x\in B$.

Cho A là một đại số có đối hợp. Nếu $f$ là một dạng tuyến tính trên A, thì ánh xạ $x\mapsto \overline{f(x^*)}$ trên A là một dạng tuyến tính trên A, được ký hiệu bởi $f^*$. Ánh xạ $f\mapsto f^*$ là một đối hợp nửa tuyến tính trên $A'$. Người ta nói rằng $f$ là Hermit nếu $f=f^*$. Theo bổ đề 1 của I, p. 95, mọi dạng tuyến tính $f$ trên A có một biểu diễn duy nhất $f=f_1+if_2$ trong đó $f_1$ và $f_2$ là Hermit, cụ thể là $f_1=\frac{1}{2}(f+f^*)$ và $f_2=\frac{1}{2i}(f-f^*)$.

Để một dạng tuyến tính $f$ là Hermit, điều kiện cần và đủ là hạn chế của $f$ trên $A_h$ nhận giá trị thực (mệnh đề 1 của I, p. 95). Ánh xạ $f\mapsto f|A_h$ là một đẳng cấu của không gian vectơ thực các dạng Hermit lên không gian đối ngẫu của không gian vectơ thực $A_h$.

Đặc biệt, $\mathsf{X}'(A)_h$ (tương ứng $\mathsf{X}(A)_h$) sẽ ký hiệu tập hợp các đặc trưng Hermit của A (tương ứng tập hợp các đặc trưng Hermit khác không của A). Do đó một đặc trưng là Hermit nếu hạn chế của nó trên $A_h$ nhận giá trị thực.

Nếu A giao hoán và nếu $\chi$ là một đặc trưng của A, thì $\chi^*$ là một đặc trưng của A, và ánh xạ $\chi \mapsto \chi^*$ là một đồng phôi của $\mathsf{X}'(A)$ lên $\mathsf{X}'(A)$.

#### Bổ đề 3 {#ts-i-s6-lem-3 .statement tag=02CN}

Cho A là một đại số có đối hợp giao hoán. Biến đổi Gelfand của A vào $\mathscr{C}_0(\mathsf{X}(A))$ là một cấu xạ của các đại số có đối hợp khi và chỉ khi mọi đặc trưng của A đều là Hermit.

Thật vậy, nói rằng $\mathscr{G}_A$ là một cấu xạ của các đại số có đối hợp có nghĩa là nói rằng, với mọi $x\in A$ và $\chi \in \mathsf{X}(A)$, ta có

$$
\chi (x^*) =\mathscr{G}_A(x^*)(\chi ) =\mathscr{G}_A(x)(\chi ) =\overline{\chi(x)}
$$

nghĩa là, mọi $\chi$ đều là Hermit.

#### Ví dụ 1 {#ts-i-s6-n2-exa-1 .statement tag=02CO}

Cho A là đại số các hàm nhận giá trị phức trên một tập hợp X. Ánh xạ $f\mapsto \overline{f}$ là một phép đối hợp trong A. Đại số con các hàm bị chặn trên X là một đại số con có đối hợp của A. Nếu X là một không gian tôpô compact địa phương, thì các đại số con $\mathscr{C}(X),\mathscr{C}_b(X),\mathscr{C}_0(X)$ và $\mathscr{K}(X)$ là những đại số con có đối hợp của A.

#### Ví dụ 2 {#ts-i-s6-n2-exa-2 .statement tag=02CP}

Cho X là một không gian tôpô compact địa phương và $\mu$ là một độ đo dương trên X. Ánh xạ $f\mapsto \overline{f}$ là một phép đối hợp trên đại số $\mathscr{L}^{\infty}(X, \mu)$; khi chuyển qua thương, nó cảm sinh một phép đối hợp trên đại số có đơn vị $L^{\infty}(X, \mu)$.

#### Ví dụ 3 {#ts-i-s6-n2-exa-3 .statement tag=02CQ}

Cho E là một không gian Hilbert phức. Trên đại số Banach $\mathscr{L}(E)$, ánh xạ $x\mapsto x^*$ (EVT, V, p. 37, prop. 1) là một phép đối hợp.

#### Ví dụ 4 {#ts-i-s6-n2-exa-4 .statement tag=02CR}

Cho G là một nhóm compact địa phương. Cho $\mathscr{M}^1(G)$ là đại số Banach của các độ đo phức bị chặn trên G (ví dụ 6 của I, p. 19).

Ánh xạ $x\mapsto x^{-1}$ của G lên G biến mọi độ đo $\mu\in$ $\mathscr{M}^1(G)$ thành một độ đo $\check{\mu}\in \mathscr{M}^1(G)$ (INT, VII, p. 12, công thức (13)). Ta ký hiệu bởi $\mu^*$ độ đo liên hợp phức của $\check{\mu}$. Ánh xạ $\mu\mapsto \check{\mu}$ là một đẳng cấu đẳng cự của đại số Banach $\mathscr{M}^1(G)$ lên đại số Banach $\mathscr{M}^1(G^{\circ})$ (INT, VIII, §3, n$^o1$, cor. of prop. 7), do đó $\mu\mapsto \mu^*$ là một phép đối hợp đẳng cự của đại số Banach $\mathscr{M}^1(G)$.

Tập hợp A của các độ đo bị chặn có một mật độ đối với một độ đo Haar là một đại số con đóng của $\mathscr{M}^1(G)$ ổn định dưới phép đối hợp (xem INT, VIII, §4, n$^o5$); nó không phụ thuộc vào lựa chọn một độ đo Haar.

Cho $\nu$ là một độ đo Haar trái trên G và ta ký hiệu bởi Δ môđun củavolution$Gf$. Ta trang bị$\mapsto f^*=\widetilde{f}L\overset{1}{\cdot}(G\Delta^-, \nu_1$, trong đó) với tích$\widetilde{f}(x) =\frac{(f, g)}{f(x^{-1})}\mapsto$với mọi$f*^{\nu}g$ và đối hợpin-$x\in G$. Khi đó ánh xạ $f\mapsto f\cdot \nu$ là một đẳng cấu của đại số có đối hợp $L^1(G, \nu )$ lên A. Đẳng cấu này là đẳng cự. Đặc biệt, $L^1(G, \nu )$ được đồng nhất với một đại số con có đối hợp của $\mathscr{M}^1(G)$.

#### Ví dụ 5 {#ts-i-s6-n2-exa-5 .statement tag=02CS}

Cho U là một tập con mở của $\mathbf{C}$ ổn định dưới liên hợp phức. Xét đại số $\mathscr{O}(U)$ của các hàm chỉnh hình nhận giá trị phức trên U. Với mọi hàm $f\in \mathscr{O}(U)$, ánh xạ $f^*:z\mapsto f(\overline{z})$ là một hàm chỉnh hình trên U. Ánh xạ $f\mapsto f^*$ là một phép đối hợp trên $\mathscr{O}(U)$.

Tương tự, cho S là một tập con compact của $\mathbf{C}$ ổn định dưới liên hợp phức. Xét đại số $\mathscr{O}(S)$ của các mầm hàm chỉnh hình nhận giá trị phức trong một lân cận của S. Ánh xạ $f\mapsto f^*$ là một phép đối hợp trên $\mathscr{O}(S)$.

Đại số con $\mathscr{O}_{\mathbf{R}}(U)$ (resp. đại số con $\mathscr{O}_{\mathbf{R}}(S)$) được định nghĩa trong n$^o13$ của I, p. 85 là tập hợp các phần tử Hermit của $\mathscr{O}(U)$ (resp. của $\mathscr{O}(S)$).

### 3. Các đại số định chuẩn có đối hợp

#### Định nghĩa 2 {#ts-i-s6-def-2 .statement tag=02CT}

Một đại số định chuẩn có đối hợp là một đại số định chuẩn A được trang bị một phép đối hợp $x\mapsto x^*$ sao cho $\|x^*\|=\|x\|$ với mọi $x$. Nếu A là một đại số Banach, người ta nói rằng A là một đại số Banach có đối hợp.

#### Ví dụ 1 {#ts-i-s6-n3-exa-1 .statement tag=02CU}

Cho X là một không gian tôpô compact địa phương. Đại số Banach $\mathscr{C}_b(X)$ của các hàm liên tục bị chặn trên X, nhận giá trị phức, được trang bị chuẩn $\|f\|$ = sup$_{x\in X}|f(x)|$ và phép đối hợp $f\mapsto \overline{f}$, là một đại số Banach có đối hợp. Đại số con $\mathscr{C}_0(X)$ của các hàm liên tục tiến tới 0 ở vô cực là một đại số con đóng có đối hợp của $\mathscr{C}_b(X)$.

#### Ví dụ 2 {#ts-i-s6-n3-exa-2 .statement tag=02CV}

Cho X là một không gian tôpô compact địa phương và $\mu$ một độ đo dương trên X. Đại số có đối hợp $L^{\infty}(X, \mu)$ (ví dụ 2 của I, p. 99) là một đại số Banach có đối hợp, vì $|f|=|\overline{f}|$ với mọi phần tử $f\in L^{\infty}(X, \mu)$.

#### Ví dụ 3 {#ts-i-s6-n3-exa-3 .statement tag=02CW}

Đại số có đối hợp $\mathscr{L}(E)$ của các nội cấu liên tục của một không gian Hilbert phức E (I, p. 99, ví dụ 3), được trang bị chuẩn

$\|u\|=$ sup$_{\|xx\in\|\leqslant E1}\|u(x)\|$

(EVT, III, p. 14) là một đại số Banach có đối hợp (EVT, V, p. 37, mệnh đề 1).

#### Ví dụ 4 {#ts-i-s6-n3-exa-4 .statement tag=02CX}

Đại số có đối hợp $\mathscr{M}^1(G)$ của các độ đo bị chặn trên một nhóm compact địa phương (I, p. 99, ví dụ 4), được trang bị chuẩn thông thường (ví dụ 6 của I, p. 19), là một đại số Banach có đối hợp. Cho $\nu$ là một độ đo Haar trái trên G. Đại số Banach có đối hợp $L^1(G, \nu )$ được đồng nhất với một đại số con đóng của $\mathscr{M}^1(G)$.

#### Ví dụ 5 {#ts-i-s6-n3-exa-5 .statement tag=02CY}

Cho $(A_i)$ là một họ các đại số định chuẩn có đối hợp. Cho A là đại số định chuẩn tích của các $A_i$ (No.$^o1$ của I, p. 15). Đại số A, được trang bị phép đối hợp $(x_i)^*= (x^*_i)$, là một đại số định chuẩn có đối hợp. Nếu mỗi đại số $A_i$ là một đại số Banach có đối hợp, thì A là một đại số Banach có đối hợp. Người ta nói rằng A là đại số định chuẩn có đối hợp tích (tương ứng, đại số Banach có đối hợp tích) của các $A_i$.

#### Ví dụ 6 {#ts-i-s6-n3-exa-6 .statement tag=02CZ}

Cho A là một đại số định chuẩn có đối hợp và cho $\widetilde{A}$ là đại số định chuẩn suy ra từ A bằng phép nối thêm một phần tử đơn vị. Được trang bị phép đối hợp xác định trong No.$^o2$, đại số $\widetilde{A}$ là một đại số định chuẩn có đối hợp. Nếu A là một đại số Banach có đối hợp, thì $\widetilde{A}$ cũng vậy là một đại số Banach có đối hợp.

Nếu A là một đại số định chuẩn có đối hợp, bao đóng của một đại số con có đối hợp là một đại số con có đối hợp. Nếu $M\subset A$, đại số con đóng có đối hợp nhỏ nhất chứa M được gọi là đại số con đóng có đối hợp sinh bởi M; nó là bao đóng của đại số con sinh bởi $M\cup M^*$. Nếu M thu về một phần tử chuẩn tắc, thì đại số đóng có đối hợp sinh bởi M là giao hoán, và mọi phần tử của nó đều chuẩn tắc.

Tương tự, nếu A là một đại số định chuẩn có đối hợp, có đơn vị và M là một tập con của A, thì đại số con đóng có đối hợp, có đơn vị nhỏ nhất chứa M được gọi là đại số con đóng có đối hợp, có đơn vị sinh bởi M; nó là bao đóng của đại số con có đơn vị sinh bởi $M\cup M^*$. Nếu M thu về một phần tử chuẩn tắc, thì đại số có đối hợp, có đơn vị, đóng sinh bởi M là giao hoán, và mọi phần tử của nó đều chuẩn tắc.

Thương của một đại số định chuẩn có đối hợp theo một iđêan hai phía tự liên hợp đóng, phép hoàn thành, và đại số đối của một đại số định chuẩn có đối hợp đều một cách tự nhiên là những đại số định chuẩn có đối hợp.

Nếu A là một đại số định chuẩn có đối hợp, tập $A_h$ các phần tử Hermit của A là một không gian vectơ thực định chuẩn.

#### Bổ đề 4 {#ts-i-s6-lem-4 .statement tag=02D0}

Cho A là một đại số định chuẩn có đối hợp. Với mọi dạng tuyến tính liên tục $f$ trên A, ta có $\|f^*\|=\|f\|$. Hơn nữa, nếu $f$ là Hermit, thì $\|f\|=\|f|A_h\|$.

Mệnh đề thứ nhất suy ra từ các định nghĩa. Với mệnh đề thứ hai, cho $g$ ký hiệu hạn chế của $f$ lên $A_h$. Ta có $\|f\|\geqslant \|g\|$. Hãy chứng minh bất đẳng thức đảo lại. Với mọi $\varepsilon  >$ 0, tồn tại $x\in$ A sao cho $\|x\|\leqslant 1$ và $|f(x)|\geqslant \|f\| -\varepsilon$. Nhân $x$ với một số phức có môđun 1, ta có thể giả sử $f(x)\geqslant 0$. Khi đó phần tử $\frac{1}{2}(x+x^*)$ thuộc $A_h$ và có chuẩn $\leqslant 1$. Ta có

$|(1_*)|$ 1 $*$

$$
g(x+x)|=|f(x) +f(x)|=f(x)\geqslant \|f\| -\varepsilon
$$

2 2

do đó $\|g\|\geqslant \|f\| -\varepsilon$. Suy ra $\|g\|\geqslant \|f\|$.

Trong phần tiếp theo, các dạng tuyến tính liên tục Hermit trên A và các dạng tuyến tính liên tục thực trên $A_h$ sẽ được đồng nhất.

#### Bổ đề 5 {#ts-i-s6-lem-5 .statement tag=02D1}

Cho A là một đại số Banach có đối hợp.

a) Với mọi $x\in A$, ta có exp($x$)$^*=$ exp($x^*$) ;

b) Cho $x\in A_h$ là một phần tử Hermit. Khi đó exp($ix$) là unita.

Thật vậy, vì phép đối hợp trên A là liên tục, ta có

exp($x$)$^*=(\sum_{n=0}^{\infty}xn^n$! $)^*=\sum_{n=0}^{\infty}(x\overset{*}{n}$!$)^n=$ exp($x^*$)

với mọi $x\in A$ (công thức (9) của I, p. 78). Nếu $x\in A_h$, suy ra

exp($ix$)$^*=$ exp(($ix$)$^*$) $=$ exp($-ix$) $=$ exp($ix$)$^{-1}$

(công thức (11) của I, p. 78).

### 4. Đại số stellar

#### Định nghĩa 3 {#ts-i-s6-def-3 .statement tag=02D2}

Một đại số Banach có đối hợp A sao cho $\|x\|^2=\|x^*x\|$ với mọi $x\in A$ được gọi là một đại số stellar.

Nếu A và B là các đại số stellar, một cấu xạ, hay cấu xạ của các đại số stellar, từ A vào B là một cấu xạ của các đại số có đối hợp từ A vào B. Một đẳng cấu từ A lên B là một đẳng cấu của các đại số có đối hợp từ A lên B.

Một số tác giả gọi đó là một "$C^*$-algebra".

Cho A là một đại số stellar. Một đại số con stellar của A là một đại số con đóng có đối hợp của A.

#### Ví dụ 1 {#ts-i-s6-n4-exa-1 .statement tag=02D3}

Đại số Banach có đối hợp của các nội cấu liên tục của một không gian Hilbert phức (ví dụ 3 của I, p. 100) là một đại số stellar (EVT, V, p. 39, prop. 2).

#### Ví dụ 2 {#ts-i-s6-n4-exa-2 .statement tag=02D4}

Cho X là một không gian tôpô compact địa phương. Đại số Banach có đối hợp $\mathscr{C}_b(X)$ của các hàm liên tục bị chặn nhận giá trị phức trên X (ví dụ 1 của I, p. 100) là một đại số stellar. Thật vậy, với mọi hàm $f\in \mathscr{C}_b(X)$, ta có $f^*f=|f|^2$, và do đó $\|f^*f\|=\||f|^2\|=\|f\|^2$.

Cho $A =\mathscr{C}_0(X)$ là đại số con Banach có đối hợp gồm các hàm tiến tới 0 ở vô cực. Nó là một đại số con stellar của $\mathscr{C}_b(X)$. Với mọi hàm $f\in A$, ta có $\|f\|=\varrho (f)$, vì Sp$'_A(f) =f(X)\cup  \{0\}$.

Cho X và Y là các không gian tôpô compact địa phương. Với mọi ánh xạ bộ phận thực sự $\varphi$ từ X vào Y (định nghĩa 1 của I, p. 33), cấu xạ đại số $\varphi^*$ từ $\mathscr{C}_0(Y)$ vào $\mathscr{C}_0(X)$ (mệnh đề 3 của I, p. 34) là một cấu xạ của các đại số có đối hợp. Ngược lại, mọi cấu xạ của các đại số stellar $\pi :\mathscr{C}_0(Y)\rightarrow \mathscr{C}_0(X)$ đều có dạng này (loc. cit.).

#### Ví dụ 3 {#ts-i-s6-n4-exa-3 .statement tag=02D5}

Cho X là một không gian tôpô compact và cho $x_0\in X$ là một phần tử cố định của X. Đại số con $\mathscr{C}'(X)$ của $\mathscr{C}(X)$ gồm các hàm liên tục $f: X\rightarrow$ $\mathbf{C}$ sao cho $f(x_0) = 0$ là một đại số stellar.

#### Ví dụ 4 {#ts-i-s6-n4-exa-4 .statement tag=02D6}

Cho X là một không gian tôpô Hausdorff và $\mu$ là một độ đo dương trên X. Đại số Banach có đối hợp $L^{\infty}(X, \mu)$ là một đại số stellar giao hoán có đơn vị.

#### Ví dụ 5 {#ts-i-s6-n4-exa-5 .statement tag=02D7}

Cho $(A_i)$ là một họ các đại số stellar. Tích đại số Banach có đối hợp A của các $A_i$ (ví dụ 5 của I, p. 101) là một đại số stellar, được gọi là đại số stellar tích của các $A_i$.

#### Ví dụ 6 {#ts-i-s6-n4-exa-6 .statement tag=02D8}

Cho A là một đại số stellar. Nếu B là một đại số con đóng có đối hợp của A, thì B là một đại số stellar. Ta sẽ thấy (V, sẽ xuất hiện) rằng mọi đại số stellar đều đẳng cấu với một đại số con đóng có đối hợp của đại số stellar các nội cấu của một không gian Hilbert (ví dụ 1).

#### Ví dụ 7 {#ts-i-s6-n4-exa-7 .statement tag=02D9}

Cho A là một đại số stellar. Nếu $M\subset A$ là một tập con bất kỳ, thì đại số con đóng có đối hợp của A sinh bởi M là một đại số stellar, được gọi là đại số con stellar của A sinh bởi M. Hơn nữa nếu A có đơn vị, thì đại số con đóng có đối hợp có đơn vị sinh bởi M là một đại số stellar có đơn vị, được gọi là đại số con stellar có đơn vị của A sinh bởi M.

#### Ví dụ 8 {#ts-i-s6-n4-exa-8 .statement tag=02DA}

Nói chung, đại số Banach có đối hợp $\mathscr{M}^1(G)$ (ví dụ 4 của I, p. 100) không phải là một đại số stellar (I, p. 181, exerc. 8).

#### Bổ đề 6 {#ts-i-s6-lem-6 .statement tag=02DB}

Cho A là một đại số Banach được trang bị một đối hợp thỏa mãn

$$
\|x\|^2\leqslant \|x^*x\| \tag{1}
$$

với mọi $x\in A$. Khi đó A là một đại số stellar.

Cho $x\in A$. Khi đó $\|x\|^2\leqslant \|x^*\| \cdot  \|x\|$, do đó $\|x\|\leqslant \|x^*\|$. Bằng cách đổi chỗ vai trò của $x$ và $x^*$, ta thấy rằng $\|x\|=\|x^*\|$. Vì thế $\|x^*x\|\leqslant$ $\|x^*\|\|x\|\leqslant \|x\|^2$ và giả thiết suy ra đẳng thức $\|x\|^2=\|x^*x\|$.

#### Bổ đề 7 {#ts-i-s6-lem-7 .statement tag=02DC}

Cho A là một đại số stellar.

a) Biểu diễn chính quy $\boldsymbol{\gamma }$ của A (định nghĩa 1 của I, p. 16) là đẳng cự, nghĩa là

$\|x\|=$ sup$_{\|y\|\leqslant 1}\|xy\|$,

đối với mọi $x\in A$;

b) Với mọi $x\in A_h$, ta có

$$
\varrho (x) =\|x\| \tag{2}
$$

Cho $x\in A$. Ta có sup$_{\|y\|\leqslant 1}\|xy\|\leqslant \|x\|$. Để chứng minh rằng $\|x\|\leqslant$ sup$_{\|y\|\leqslant 1}\|xy\|$, ta có thể giả sử rằng $\|x\|= 1$. Khi đó phần tử $y$ = $x^*$ thỏa mãn $\|y\|=\|x^*\|= 1$, và $\|xy\|=\|x\|^2= 1$, do đó có mệnh đề a).

Giả sử rằng $x$ là Hermit. Khi đó $\|x^2\|=\|x^*x\|=\|x\|^2$, do đó theo quy nạp $\|x^{2^n}\|^{2^{-n}}=\|x\|$ với mọi số nguyên $n\geqslant 1$, do đó có mệnh đề b) theo mệnh đề 1 của I, p. 20.

#### Nhận xét 1 {#ts-i-s6-n4-rem-1 .statement tag=02DD}

Cho A là một đại số stellar có đơn vị. Ta có

$$
\|1\|^2=\|1^*1\|=\|1\|
$$

vì vậy chuẩn $\|1\|$ bằng không hoặc bằng 1. Nếu $A\not=\{0\}$, ta suy ra rằng $\|1\|= 1$. Do đó, với mọi phần tử unita $u$ của A, ta có $\|u\|=$ $\|u^*u\|^{1/2}= 1$.

#### Nhận xét 2 {#ts-i-s6-n4-rem-2 .statement tag=02DE}

Cho A là một đại số đối hợp định chuẩn. Nếu $\|x\|^2=\|x^*x\|$ đối với mọi $x\in A$, sự hoàn thành $\widehat{A}$ của A là một đại số stellar.

#### Mệnh đề 2 {#ts-i-s6-prop-2 .statement tag=02DF}

Cho A là một đại số Banach đối hợp, cho B là một đại số stellar, và cho $\pi$ là một cấu xạ các đại số đối hợp từ A vào B. Ta có $\|\pi (x)\|\leqslant \|x\|$ đối với mọi $x\in A$, và đặc biệt $\pi$ liên tục.

Với mọi $x\in A$, ta có Sp$'_B(\pi (x))\subset$ Sp$'_A(x)$, vì vậy $\varrho (\pi (x))\leqslant \varrho (x)\leqslant$ $\|x\|$. Vì $\pi (x^*x)\in B_h$, ta có $\|\pi (x^*x)\|=\varrho (\pi (x^*x))$ (công thức (2)), vì vậy

$$
\|\pi (x)\|^2=\|\pi (x^*x)\|=\varrho (\pi (x^*x))\leqslant \|x^*x\|=\|x\|^2
$$

#### Mệnh đề 3 {#ts-i-s6-prop-3 .statement tag=02DG}

Cho A là một đại số stellar và cho $\widetilde{A}$ là đại số đối hợp suy ra từ A bằng phép nối một phần tử đơn vị. Tồn tại một chuẩn duy nhất trên $\widetilde{A}$ kéo dài chuẩn của A và biến $\widetilde{A}$ thành một đại số stellar.

Tính duy nhất của một chuẩn như vậy suy ra từ mệnh đề 2. Bây giờ ta hãy chứng minh sự tồn tại của nó. Kí hiệu $\widetilde{e}$ là phần tử đơn vị của $\widetilde{A}$.

Trước hết giả sử rằng A có một phần tử đơn vị $e$. Tích của các đại số đối hợp định chuẩn A và $\mathbf{C}(\widetilde{e}-e)$ được đồng nhất với $\widetilde{A}$ và là một đại số stellar (ví dụ 5). Chuẩn trên $\widetilde{A}$ kéo dài chuẩn của A, do đó có mệnh đề.

Từ đây giả sử rằng A không có phần tử đơn vị. Với mọi $x\in \widetilde{A}$, gọi $\boldsymbol{\gamma }_x$ là toán tử phép nhân $y\mapsto xy$ từ A vào A, và đặt $\|x\|_{\widetilde{A}}=\|\boldsymbol{\gamma }_x\|$. Ánh xạ $x\mapsto  \|x\|_{\widetilde{A}}$ là một nửa chuẩn trên $\widetilde{A}$. Với mọi $x$ và $x'$ trong $\widetilde{A}$, ta có $\|xx'\|_{\widetilde{A}}\leqslant \|x\|_{\widetilde{A}}\|x'\|_{\widetilde{A}}$. Hơn nữa, theo bổ đề 7, ta có $\|x\|_{\widetilde{A}}=\|x\|$ đối với mọi $x\in A$.

Ta hãy chứng minh rằng ánh xạ $x\mapsto  \|x\|_{\widetilde{A}}$ là một chuẩn trên $\widetilde{A}$. Cho $\lambda \in \mathbf{C}$ và $x\in A$ sao cho $\|\lambda \widetilde{e}+x\|_{\widetilde{A}}$ = 0. Nếu $\lambda \not= 0$, điều kiện $(\lambda \widetilde{e}+x)y= 0$ với mọi $y\in A$ kéo theo rằng $-\lambda^{-1}x$ là một phần tử đơn vị trái trong A. Tương tự, phần tử $-\overline{\lambda}^{-1}x^*$ là một phần tử đơn vị phải. Như vậy đại số A khi đó sẽ có một phần tử đơn vị, trái với giả thiết. Do đó $\lambda = 0$. Nhưng khi đó $0 =\|x\|_{\widetilde{A}}=$ $\|x\|$, và vì thế $x= 0$.

Vì A là đầy đủ và có đối chiều 1 trong $\widetilde{A}$, không gian $\widetilde{A}$ được trang bị chuẩn $x\mapsto  \|x\|_{\widetilde{A}}$ là đầy đủ. Để kết luận, do đó chỉ cần chứng minh rằng ta có $\|x\|^2_{\widetilde{A}}\leqslant \|x^*x\|_{\widetilde{A}}$ với mọi $x\in \widetilde{A}$ (Bổ đề 6). Có thể giả sử rằng $\|x\|_{\widetilde{A}}= 1$. Khi đó, với mọi số thực $r <1$, tồn tại $y\in A$ sao cho $\|y\|=\|y^*\|\leqslant 1$ và $\|xy\|^2\geqslant r$. Vì $xy\in A$, ta có

$$
\|x^*x\|_{\widetilde{A}}\geqslant \|x^*xy\|\geqslant \|y^*(x^*x)y\|=\|(xy)^*(xy)\|=\|xy\|^2\geqslant r
$$

Suy ra $\|x^*x\|_{\widetilde{A}}\geqslant 1$, và do đó đại số đối hợp $\widetilde{A}$ được trang bị chuẩn $x\mapsto  \|x\|_{\widetilde{A}}$ là một đại số sao.

#### Định nghĩa 4 {#ts-i-s6-def-4 .statement tag=02DH}

Người ta nói rằng $\widetilde{A}$, được trang bị chuẩn của Mệnh đề 3, là đại số sao suy ra từ A bằng phép nối một phần tử đơn vị.

Khi $A\not=\{0\}$, chuẩn đại số sao trên đại số đối hợp định chuẩn $\widetilde{A}$ không phải là chuẩn đã xét trong Ví dụ 6 của I, p. 101 (x. Bài tập 10 của I, p. 181).

#### Mệnh đề 4 {#ts-i-s6-prop-4 .statement tag=02DI}

Cho A là một đại số sao.

a) Nếu A có một phần tử đơn vị và nếu $u$ là một phần tử unita của A, thì Sp($u$)$\subset \mathbf{U}$;

b) Nếu $h$ là một phần tử Hermit của A, thì Sp$'(h)\subset \mathbf{R}$.

Có thể giả sử rằng A khác không. Ta hãy chứng minh mệnh đề a). Cho $u$ là một phần tử unita của A. Ta có $\|u\|=\|u^{-1}\|= 1$ (Nhận xét 1), do đó Sp($u$)$\subset \mathbf{U}($I, p. 26, Hệ quả 3). Để chứng minh b), có thể giả sử rằng A có đơn vị (Mệnh đề 3). Cho $h$ là một phần tử Hermit của A. Khi đó exp($ih$) là unita (Bổ đề 5 của I, p. 102). Như vậy, theo Hệ quả 2 của I, p. 67 và a), ta có exp($i$ Sp($h$)) $=$ Sp(exp($ih$))$\subset \mathbf{U}$, điều đó có nghĩa là Sp($h$)$\subset \mathbf{R}$.

#### Mệnh đề 5 {#ts-i-s6-prop-5 .statement tag=02DJ}

Cho A là một đại số sao có đơn vị và B là một đại số con sao của A chứa phần tử đơn vị của A. Khi đó B là một đại số con đầy đủ của A. Đặc biệt, ta có Sp$_B(x) =$ Sp$_A(x)$ với mọi $x$ trong B.

Cho $x$ là một phần tử Hermit của B. Vì Sp$_B(x)\subset \mathbf{R}$ (Mệnh đề 4), Mệnh đề 6 của I, p. 28 cho thấy rằng Sp$_B(x) =$ Sp$_A(x)$. Đặc biệt, $x$ khả nghịch trong B khi và chỉ khi nó khả nghịch trong A.

Bây giờ giả sử $x$ là một phần tử bất kỳ của B khả nghịch trong A. Khi đó $x^*$ khả nghịch trong A, và $xx^*$ khả nghịch trong A. Vì $xx^*$ là Hermit, điều đi trước cho thấy $xx^*$ khả nghịch trong B. Điều này kéo theo rằng $x$ khả nghịch phải trong B. Tương tự, ta kiểm tra được rằng $x$ khả nghịch trái trong B, và do đó rằng $x$ khả nghịch trong B. Vậy, B là một đại số con đầy đủ của A.

#### Hệ quả {#ts-i-s6-n4-cor-1 .statement tag=02DK}

Cho A là một đại số sao và B là một đại số con sao của A. Khi đó ta có Sp$'_B(x) =$ Sp$'_A(x)$ với mọi $x$ trong B.

Bằng cách thêm vào một phần tử đơn vị (mệnh đề 3), điều này suy ra từ mệnh đề 5.

Mệnh đề 6 (Định lý Fuglede–Putnam)

Cho A là một đại số sao có đơn vị. Cho $a$ và $b$ là các phần tử chuẩn tắc của A. Nếu $c\in A$ thỏa mãn $ac=cb$, thì $a^*c=cb^*$.

Giả thiết kéo theo $(wa)^kc=c(wb)^k$ với mọi số nguyên $k\geqslant 0$ và mọi $w\in \mathbf{C}$, do đó $e^{wa}c=ce^{wb}$ (công thức (9) của I, p. 78). Xét hàm $f$ từ $\mathbf{C}$ vào A được xác định bởi $z\mapsto e^{-za^*}ce^{zb^*}$. Đó là một hàm chỉnh hình trên $\mathbf{C}$, mà đạo hàm thỏa mãn

$$
f'(z) =-a^*e^{-za^*}ce^{zb^*}+e^{-za^*}cb^*e^{zb^*}
$$

với mọi $z\in \mathbf{C}$. Vì $c=e^{-za}ce^{zb}$, ta có thể viết

$$
f(z) =e^{-za^*}e^{za}c e^{-zb}e^{zb^*}
$$

Vì $a$ và $b$ là chuẩn tắc, các phần tử $e^{-za^*}e^{za}=e^{-za^*+za}$ và $e^{-zb}e^{zb^*}=e^{-zb+zb^*}$ của A là unita với mọi $z\in \mathbf{C}$ (bổ đề 5 của I, p. 102), nên có chuẩn bằng 1. Do đó, ta có $\|f(z)\|\leqslant \|c\|$ với mọi $z\in \mathbf{C}$. Vì vậy hàm $f$ là hằng (VAR, R1, 3.3.6, p. 29), nghĩa là $f(z) =f(0) =c$ với mọi $z\in \mathbf{C}$. Nhưng khi đó $-a^*c+cb^*=f'(0) = 0$.

#### Hệ quả {#ts-i-s6-n4-cor-2 .statement tag=02DL}

Cho A là một đại số sao và $a$ là một phần tử chuẩn tắc của A. Hoán tập (tương ứng, đối giao hoán tử kép) của $\{a, a^*\}$ trùng với hoán tập (tương ứng, đối giao hoán tử kép) của $a$.

Chỉ cần lấy $b=a$ trong mệnh đề.

### 5. Đại số Sao Giao Hoán

#### Bổ đề 8 {#ts-i-s6-lem-8 .statement tag=02DM}

Cho X và Y là các không gian mêtric, trong đó không gian X là đầy đủ. Cho $f$ là một ánh xạ từ X vào Y sao cho

$$
d(f(x), f(y))\geqslant d(x, y)
$$

với mọi $x$ và $y$ trong X, và sao cho đồ thị của $f$ là đóng trong $X\times Y$. Khi đó $f$ là một ánh xạ đóng.

Cho F là một tập con đóng của X và $(y_n)_{n\in\mathbf{N}}$ là một dãy trong $f(F)$ hội tụ đến $y\in Y$. Với mọi $n\in \mathbf{N}$, lấy $x_n\in F$ sao cho $f(x_n) =y_n$. Giả thiết kéo theo rằng dãy $(x_n)_{n\in\mathbf{N}}$ là một dãy Cauchy; gọi $x\in X$ là giới hạn của nó; đó là một phần tử của F, vì F là đóng. Hơn nữa, ta có $(x_n, f(x_n))\rightarrow (x, y)$ trong $X\times Y$. Vì đồ thị của $f$ là đóng, suy ra $y=f(x)$ thuộc $f(F)$.

#### Bổ đề 9 {#ts-i-s6-lem-9 .statement tag=02DN}

Cho A là một đại số sao giao hoán. Mọi đặc trưng của A đều là Hermit và biến đổi Gelfand là một cấu xạ của các đại số sao từ A vào $\mathscr{C}_0(\mathsf{X}(A))$.

Chỉ cần chứng minh mệnh đề thứ nhất (mệnh đề 7 của I, p. 38 và bổ đề 3 của I, p. 98). Cho $\chi$ là một đặc trưng của A. Với mọi phần tử Hermit $y$ của A, ta có $\chi (y) =\mathscr{G}_A(y)(\chi )\in$ Sp$'(y)\subset \mathbf{R}$ (mệnh đề 4 của I, p. 106). Do đó, đặc trưng $\chi$ là Hermit (mệnh đề 1 của I, p. 95).

#### Định lý 1 {#ts-i-s6-thm-1 .statement tag=02DO}

Cho A là một đại số sao giao hoán. Biến đổi Gelfand là một đẳng cấu đẳng cự của đại số sao A lên đại số sao $\mathscr{C}_0(\mathsf{X}(A))$ gồm các hàm liên tục trên $\mathsf{X}(A)$ tiến tới 0 ở vô cực.

Biến đổi Gelfand là một cấu xạ của các đại số đối hợp từ A vào $\mathscr{C}_0(\mathsf{X}(A))$ (bổ đề 9). Gọi B là ảnh của nó. Đó là một đại số con đối hợp của $\mathscr{C}_0(\mathsf{X}(A))$. Theo định nghĩa, các phần tử của B phân biệt các điểm của $\mathsf{X}(A)$. Cho $\chi \in \mathsf{X}(A)$. Tồn tại $x\in A$ sao cho $\chi (x)\not= 0$, do đó $f=\mathscr{G}(x)$ là một phần tử của B sao cho $f(\chi )\not= 0$. Theo TG, X, p. 40, hệ quả 2, vì vậy đại số con B là trù mật trong $\mathscr{C}_0(\mathsf{X}(A))$.

Với mọi phần tử Hermit $y$ của A, ta có $\|\mathscr{G}(y)\|=\varrho (y) =\|y\|$ (mệnh đề 7 của I, p. 38 và công thức (2) của I, p. 104), do đó, với mọi $x\in A$, các đẳng thức

$$
\|x\|^2=\|x^*x\|=\|\mathscr{G}(x^*x)\|=\|\overline{\mathscr{G} (x)}\cdot \mathscr{G}(x)\|=\|\mathscr{G}(x)\|^2
$$

Suy ra $\mathscr{G}$ là đẳng cự, và do đó ảnh của nó là B đóng (bổ đề 8). Kết luận rằng $B =\mathscr{C}_0(\mathsf{X}(A))$.

#### Hệ quả 1 {#ts-i-s6-thm-1-cor-1 .statement tag=02DP}

Cho A là một đại số sao và $x$ là một phần tử chuẩn tắc của A. Khi đó $\|x\|=\varrho (x)$.

Vì đại số con sao của A sinh bởi $x$ và $x^*$ là giao hoán, ta có thể giả sử rằng A là giao hoán. Trong trường hợp này, hệ quả suy ra từ định lý 1, từ ví dụ 2 của I, p. 102 và từ định lý 1 của I, p. 24.

#### Hệ quả 2 {#ts-i-s6-thm-1-cor-2 .statement tag=02DQ}

Cho A là một đại số sao giao hoán.

a) Tồn tại một không gian tôpô compact địa phương X sao cho A đẳng cấu với đại số sao $\mathscr{C}_0(X)$;

b) Cho B là một đại số sao giao hoán. Ánh xạ $\pi \mapsto$ $\mathsf{X}'(\pi )$ là một song ánh từ tập hợp các cấu xạ đại số sao từ A vào B lên tập hợp các ánh xạ bộ phận thực sự của $\mathsf{X}(B)$ vào $\mathsf{X}(A)$ (định nghĩa 1 của I, p. 33).

Định lý 1 thiết lập mệnh đề thứ nhất, và mệnh đề thứ hai suy ra từ mệnh đề 3 của I, p. 34 và từ ví dụ 2 của I, p. 102.

#### Hệ quả 3 {#ts-i-s6-thm-1-cor-3 .statement tag=02DR}

Cho A là một đại số sao giao hoán có đơn vị.

a) Tồn tại một không gian tôpô compact X sao cho A đẳng cấu với đại số sao $\mathscr{C}(X)$;

b) Cho B là một đại số sao giao hoán có đơn vị. Ánh xạ $\pi \mapsto \mathsf{X}(\pi )$ là một song ánh từ tập hợp các cấu xạ đại số sao có đơn vị $A\rightarrow B$ lên tập hợp các ánh xạ liên tục từ $\mathsf{X}(B)$ vào $\mathsf{X}(A)$.

Điều này suy ra từ những điều trên và từ mệnh đề 4 của I, p. 35.

#### Nhận xét {#ts-i-s6-n5-rem-1 .statement tag=02DS}

*Gọi $\mathbf{G}$ là phạm trù mà các đối tượng là các không gian compact địa phương và các cấu xạ là các ánh xạ bộ phận thực sự (định nghĩa 1 của I, p. 33), và gọi $\mathbf{S}$ là phạm trù các đại số sao giao hoán, mà các cấu xạ là các cấu xạ của các đại số đối hợp. Xét hàm tử từ $\mathbf{S}$ vào phạm trù đối $\mathbf{G}^{\circ}$ gắn với một đại số sao giao hoán A không gian compact địa phương $\mathsf{X}(A)$ gồm các đặc trưng khác không của A, và với một cấu xạ $\varphi : A\rightarrow B$ của các đại số sao giao hoán ánh xạ liên tục $\mathsf{X}'(\varphi )$. Định lý 1 và hệ quả 2 có nghĩa là hàm tử này là một tương đương phạm trù, và rằng một quasi-nghịch đảo của hàm tử này là hàm tử gắn với một không gian tôpô compact địa phương X đại số sao giao hoán $\mathscr{C}_0(X)$.

Tương tự, hệ quả 3 có nghĩa là phạm trù đối của phạm trù các không gian compact là tương đương với phạm trù các đại số sao giao hoán có đơn vị.*

### 6. Phép tính phiếm hàm trong các đại số sao có đơn vị

Trong số này, A là một đại số sao có đơn vị và $x$ là một phần tử chuẩn tắc của A.

Cho B là đại số con \* có đơn vị của A sinh bởi $x$; nó giao hoán và được chứa trong đối giao hoán tử kép của $\{x, x^*\}$, do đó trong đối giao hoán tử kép của $x$ (hệ quả của mệnh đề 6 của I, p. 106). Biến đổi Gelfand $\mathscr{G}_B: B\rightarrow \mathscr{C}(\mathsf{X}(B))$ là một đẳng cấu của các đại số \* (định lý 1 của I, p. 108). Ta có Sp$_B(x) =$ Sp$_A(x)$ (mệnh đề 5 của I, p. 106).

#### Bổ đề 10 {#ts-i-s6-lem-10 .statement tag=02DT}

Ánh xạ ev$_x:\chi \mapsto \chi (x)$ cảm sinh một đồng phôi từ $\mathsf{X}(B)$ lên Sp$_A(x)$.

Ánh xạ $x\mapsto \chi (x)$ từ $\mathsf{X}(B)$ vào $\mathbf{C}$ là liên tục, và ảnh của nó bằng Sp$_B(x)$ theo mệnh đề 6 của I, p. 37, do đó bằng Sp$_A(x)$. Vì các đặc trưng của B là Hermit (bổ đề 9 của I, p. 107), các đặc trưng của B trùng nhau tại $x$ thì cũng bằng nhau tại $x^*$, do đó bằng nhau trên đại số con \* có đơn vị B sinh bởi $x$. Điều này chứng tỏ rằng ánh xạ ev$_x$ là đơn ánh. Vì $\mathsf{X}(B)$ là compact và $\mathbf{C}$ là tách biệt, nó cảm sinh một đồng phôi từ $\mathsf{X}(B)$ lên ảnh của nó, do đó có bổ đề.

Từ bổ đề suy ra một đẳng cấu của các đại số \* $\varphi_x:\mathscr{C}$(Sp$_A(x)$)$\rightarrow \mathscr{C}(\mathsf{X}(B))$. Nó biến một hàm $f\in \mathscr{C}$ (Sp$_A(x)$) thành hàm $\chi \mapsto f(\chi (x))$. Ánh xạ $\mathscr{G}_B^{-1}\circ \varphi_x$ là một đẳng cấu của đại số \* $\mathscr{C}$(Sp$_A(x)$) lên B.

#### Định nghĩa 5 {#ts-i-s6-def-5 .statement tag=02DU}

Cấu xạ đối hợp $f\mapsto (\mathscr{G}_B^{-1}\circ \varphi_x)(f)$ từ $\mathscr{C}$(Sp$_A(x)$) vào A được gọi là ánh xạ của phép tính phiếm hàm liên tục của $x$ trong A. Nó được ký hiệu bởi $f\mapsto f(x)$.

#### Nhận xét {#ts-i-s6-n6-rem-1 .statement tag=02DV}

Ánh xạ $f\mapsto f(x)$ là đẳng cự; ảnh của nó là đại số con \* có đơn vị B sinh bởi $x$, được chứa trong đối giao hoán tử kép của $x$.

Nếu $f$ là hạn chế trên Sp$_A(x)$ của một hàm có dạng $z\mapsto$ $P(z, z)$, trong đó $P\in \mathbf{C}[X,Y]$ là một đa thức, thì ta có $f(x) = P(x, x^*)$ theo nghĩa đại số thông thường.

#### Ví dụ 1 {#ts-i-s6-n6-exa-1 .statement tag=02DW}

Giả sử rằng tồn tại $\lambda \in \mathbf{C}$ sao cho Sp$_A(x)$ thu về $\lambda$. Khi đó ta có $x=\lambda \cdot 1$. Thật vậy, hàm đồng nhất của Sp$_A(x)$ bằng $\lambda$, vì vậy ảnh của nó dưới ánh xạ phép tính phiếm hàm, tức là $x$, bằng $\lambda \cdot 1$.

#### Ví dụ 2 {#ts-i-s6-n6-exa-2 .statement tag=02DX}

Để $x$ là Hermit, điều kiện cần và đủ là Sp$_A(x)$ được chứa trong $\mathbf{R}$. Thật vậy, gọi $f$ là ánh xạ liên tục trên Sp$_A(x)$ được cho bởi $f(z) =z-\overline{z}$. Khi đó $x$ là Hermit khi và chỉ khi $f(x) = 0$, nghĩa là, khi $f$ bằng không, tức là, khi Sp$_A(x)$ được chứa trong $\mathbf{R}$.

#### Ví dụ 3 {#ts-i-s6-n6-exa-3 .statement tag=02DY}

Để $x$ là unita, điều kiện cần và đủ là phổ của nó được chứa trong đường tròn đơn vị của $\mathbf{C}$. Thật vậy, gọi $f\in \mathscr{C}$ (Sp$_A(x)$) là hàm được xác định bởi $f(z) =zz-1$; phần tử $x$ là unita khi và chỉ khi $f(x) = 0$, nghĩa là, khi $f$ bằng không.

#### Mệnh đề 7 {#ts-i-s6-prop-7 .statement tag=02DZ}

Ánh xạ $f\mapsto f(x)$ là cấu xạ có đơn vị duy nhất của các đại số có đối hợp từ $\mathscr{C}$ (Sp$_A(x)$) vào A sao cho ánh xạ đồng nhất $z$ của Sp$_A(x)$ có ảnh là $x$.

Thật vậy, đại số con có đơn vị của $\mathscr{C}$ (Sp$_A(x)$) được sinh bởi các phần tử $z$ và $\overline{z}$ của $\mathscr{C}$(Sp$_A(x)$) là trù mật trong $\mathscr{C}$ (Sp$_A(x)$) (TG, X, p. 40, hệ quả 1). Vì mọi cấu xạ của các đại số có đối hợp từ $\mathscr{C}$ (Sp$_A(x)$) vào A đều liên tục (I, p. 104, mệnh đề 2), nên tồn tại nhiều nhất một cấu xạ của các đại số có đối hợp từ $\mathscr{C}$(Sp$_A(x)$) vào A biến $z$ thành $x$.

Hệ quả sau đây cho thấy rằng khi $f$ là hạn chế của một hàm chỉnh hình trong một lân cận của Sp$_A(x)$, định nghĩa của $f(x)$ trùng với định nghĩa của phép tính phiếm hàm chỉnh hình một biến ở No. 9 của I, p. 74.

#### Hệ quả 1 {#ts-i-s6-prop-7-cor-1 .statement tag=02E0}

Cho $f\in \mathscr{O}$(Sp$_A(x)$) là một mầm của hàm chỉnh hình trong một lân cận của Sp$_A(x)$ và cho $\widetilde{f}\in \mathscr{C}$(Sp$_A(x)$) là hàm liên tục trên Sp$_A(x)$ liên kết với $f$. Khi đó $\widetilde{f}(x) =f(x)$, trong đó $f(x)$ là phần tử của A do phép tính phiếm hàm chỉnh hình xác định.

Thật vậy, ánh xạ $f\mapsto \widetilde{f}(x)$ là một cấu xạ có đơn vị liên tục từ $\mathscr{O}$(Sp$_A(x)$) vào A, biến mầm của hàm đồng nhất trong một lân cận của Sp$_A(x)$ thành $x$. Kết quả khi đó là một hệ quả của định lý 5 của I, p. 74.

#### Hệ quả 2 {#ts-i-s6-prop-7-cor-2 .statement tag=02E1}

Cho $f\in \mathscr{C}$ (Sp$_A(x)$).

a) Ta có

Sp$_A(f(x)) =f$(Sp$_A(x)$) ;

b) Với mọi $g\in \mathscr{C}$ (Sp$_A(f(x))$), ta có $(g\circ f)(x) =g(f(x))$.

Vì $f(x)$ thuộc đại số con đầy đủ B của A, nên ta có Sp$_A(f(x)) =$ Sp$_B(f(x))$ (Mệnh đề 5 của I, p. 106). Đẳng cấu $f\mapsto f(x)$ của $\mathscr{C}$(Sp$_A(x)$) vào B bảo toàn phổ; do đó ta có Sp$_B(f(x)) =$ Sp$_{\mathscr{C}(Sp_A(x))}(f) =f$(Sp$_A(x)$) (Ví dụ 3 của I, p. 17). Điều này chứng minh mệnh đề a).

Ánh xạ $g\mapsto (g\circ f)(x)$ là một cấu xạ có đơn vị của các đại số có đối hợp từ $\mathscr{C}$(Sp$_A(f(x))$) vào A, biến hàm đồng nhất trên Sp$_A(f(x))$ thành $f(x)$. Bởi Mệnh đề 7, do đó ta có $(g\circ f)(x) =g(f(x))$ với mọi $g\in \mathscr{C}$ (Sp$_A(f(x))$).

#### Ví dụ 4 {#ts-i-s6-n6-exa-4 .statement tag=02E2}

Cho X là một không gian địa phương compact và cho $A =\mathscr{C}_b(X)$ là đại số sao giao hoán có đơn vị của các hàm liên tục bị chặn trên X (Ví dụ 2 của I, p. 102). Cho $g\in A$; phổ của nó S là bao đóng trong $\mathbf{C}$ của tập hợp $g(X)$ các giá trị của $g$ (Ví dụ 3 của I, p. 17). Khi đó ánh xạ phép tính phiếm hàm của $g$ là ánh xạ $f\mapsto f\circ g$, với $f\in \mathscr{C}(S)$. Thật vậy, ánh xạ này là một cấu xạ có đơn vị của các đại số sao sao cho ánh xạ đồng nhất trên S có ảnh là $g$.

Trong trường hợp X compact, ta có $A =\mathscr{C}(X)$ và $S =g(X)$.

Cho $\pi : A\rightarrow A'$ là một cấu xạ có đơn vị của các đại số sao có đơn vị. Phần tử $\pi (x)$ của $A'$ là chuẩn tắc và phổ của nó đối với $A'$ được chứa trong Sp$_A(x)$. Khi đó ta có:

#### Mệnh đề 8 {#ts-i-s6-prop-8 .statement tag=02E3}

Cho $f\in \mathscr{C}$(Sp$_A(x)$). Vẫn ký hiệu bởi $f$ hạn chế của $f$ lên Sp$_{A'}(\pi (x))$, ta có đẳng thức $\pi (f(x)) =f(\pi (x))$. Đặc biệt, với mọi $\chi \in \mathsf{X}(A)$, ta có $\chi (f(x)) =f(\chi (x))$.

Cho $z$ là ánh xạ đồng nhất trên Sp$_A(x)$. Các ánh xạ được xác định bởi $f\mapsto \pi (f(x))$ và $f\mapsto f(\pi (x))$ là các cấu xạ liên tục có đơn vị của các đại số có đối hợp từ $\mathscr{C}$(Sp$_A(x)$) vào B, biến $z$ thành $\pi (x)$. Vậy nên các cấu xạ này trùng nhau trên đại số con có đơn vị và có đối hợp của $\mathscr{C}$ (Sp$_A(x)$) sinh bởi $z$. Vì đại số sau là trù mật trong $\mathscr{C}$(Sp$_A(x)$) (TG, X, p. 40, Hệ quả 1), nên các cấu xạ này bằng nhau.

#### Hệ quả {#ts-i-s6-n6-cor-1 .statement tag=02E4}

Giả sử rằng A là giao hoán. Với mọi $f\in$ $\mathscr{C}$(Sp$_A(x)$), ta có $\mathscr{G}_A(f(x)) =f\circ \mathscr{G}_A(x)$.

Chỉ cần áp dụng Mệnh đề 8 cho biến đổi Gelfand $\mathscr{G}_A$ của A vào $\mathscr{C}(\mathsf{X}(A))$ và nhận thấy (ví dụ ở trên) rằng $f(\mathscr{G}_A(x)) =f\circ \mathscr{G}_A(x)$.

### 7. Các ứng dụng của phép tính phiếm hàm

#### Mệnh đề 9 {#ts-i-s6-prop-9 .statement tag=02E5}

Mọi cấu xạ đơn ánh của các đại số stellar đều là đẳng cự và, đặc biệt, có ảnh đóng.

Cho A và $A'$ là các đại số stellar và cho $\pi : A\rightarrow A'$ là một cấu xạ các đại số đối hợp từ A vào $A'$.

Trước hết giả sử rằng A và $A'$ có đơn vị và rằng $\pi$ có đơn vị. Ta có $\|\pi \|\leqslant 1$ (Mệnh đề 2). Giả sử tồn tại $x$ trong A sao cho $\|\pi (x)\|<\|x\|$. Đặt $y=x^*x$; đây là một phần tử Hermit của A. Vì A và $A'$ là các đại số stellar, ta có $\|\pi (y)\|=\|\pi (x)\|^2<\|x\|^2=$ $\|y\|$, tức là, $\varrho (\pi (y))< \varrho (y)$ (Bổ đề 7 của I, p. 104). Đặc biệt, Sp$_{A'}(\pi (y))$ là một tập con đóng của Sp$_A(y)$, phân biệt với Sp$_A(y)$ (Nhận xét 6 của I, p. 3 và Định lý 1 của I, p. 24). Khi đó tồn tại một hàm khác không $f\in \mathscr{C}$(Sp$_A(y)$) sao cho $f|$ Sp$_{A'}(\pi (y)) = 0$ (TG, IX, p. 13, Mệnh đề 3). Đặt $w=f(y)\in$ A. Ta có $w\not= 0$ vì $f\not= 0$, nhưng $\pi (w) =\pi (f(y)) =f(\pi (y)) = 0$ vì $f$ triệt tiêu trên Sp$_{A'}(\pi (y))$ (Mệnh đề 8). Vậy $\pi$ không đơn ánh.

Bây giờ ta xét trường hợp tổng quát. Cho $\widetilde{A}$ và $\widetilde{A}'$ là các đại số stellar suy ra từ A và $A'$ tương ứng bằng phép nối thêm một phần tử đơn vị (Định nghĩa 4 của I, p. 106). Tồn tại một cấu xạ duy nhất có đơn vị của các đại số đối hợp $\widetilde{\pi}:\widetilde{A}\rightarrow \widetilde{A}'$ kéo dài $\pi$. Cấu xạ này là đơn ánh, nên là đẳng cự theo điều ở trên. Với mọi $x\in A$, khi đó ta có $\|\pi (x)\|=\|\widetilde{\pi}(x)\|=\|x\|$.

#### Bổ đề 11 {#ts-i-s6-lem-11 .statement tag=02E6}

Cho X là một không gian tôpô chính quy hoàn toàn, nghĩa là có thể uniform hóa và tách biệt (TG, IX, p. 8, Định nghĩa 4), chứa ít nhất hai điểm. Tồn tại các hàm liên tục khác không $f$ và $g$ trong $\mathscr{C}(X)$ sao cho $f g= 0$.

Cho $x\not=y$ là các điểm phân biệt của X. Cho U và V lần lượt là các lân cận mở của $x$ và $y$, sao cho U và V rời nhau. Vì X có thể uniform hóa, theo TG, IX, p. 7, Định lý 2, tồn tại một hàm $f\in \mathscr{C}(X)$ sao cho $f(x) = 1$ và $f|X$ - U = 0. Tương tự, tồn tại $g\in \mathscr{C}(X)$ sao cho $g(y) = 1$ và $g|X$ - V = 0. Khi đó ta có $f g= 0$.

#### Mệnh đề 10 {#ts-i-s6-prop-10 .statement tag=02E7}

Cho A là một đại số stellar có đơn vị. Giả sử rằng với mọi cặp $(x, y)$ các phần tử hoán vị được của A, điều kiện $xy= 0$ kéo theo rằng $x= 0$ hoặc $y= 0$. Khi đó $A =\mathbf{C}\cdot 1$.

Nếu A khác $\mathbf{C}\cdot 1$, thì tồn tại một phần tử Hermit $x$ trong A không thuộc $\mathbf{C}\cdot 1$ (Bổ đề 2 của I, p. 96). Gọi B là đại số con đối hợp có đơn vị của A sinh bởi $x$. Nó giao hoán, và đẳng cấu với $\mathscr{C}$ (Sp$_A(x)$) (I, p. 110, Nhận xét). Vì $x$ không vô hướng, phổ của nó trong B không thu về một phần tử duy nhất (Ví dụ 1 của I, p. 110). Do đó tồn tại các hàm liên tục khác không $f$ và $g$ trên Sp$_A(x)$ sao cho $f g= 0$ (Bổ đề 11). Các phần tử $f(x)$ và $g(x)$ của A là khác không, giao hoán với nhau, và thỏa mãn $f(x)g(x) = 0$ trong A.

#### Mệnh đề 11 {#ts-i-s6-prop-11 .statement tag=02E8}

Cho A là một đại số đối hợp có đơn vị, và cho $a,x$ và $y$ là các phần tử của A. Giả sử rằng $x$ và $y$ là chuẩn tắc. Nếu $xa=$ $ay$, thì ta có $f(x)a=af(y)$ đối với mọi hàm $f$ liên tục trên hợp của phổ của $x$ và phổ của $y$. Đặc biệt, ta có $f(aa^*)a=af(a^*a)$ đối với mọi hàm $f\in \mathscr{C}$ (Sp$'(a^*a)$).

Đặt S = Sp($x$)$\cup$ Sp($y$). Mệnh đề 6 của I, p. 106 suy ra rằng $x^*a=ay^*$. Do đó, ta có $f(x)a=af(y)$ đối với mọi hàm $f$ có dạng $z\mapsto P(z, z)$, trong đó $P\in \mathbf{C}[X,Y]$ là một đa thức. Vì tập hợp các hàm $f\in \mathscr{C}(S)$ thỏa mãn $f(x)a=$ $af(y)$ là một đại số con đóng của $\mathscr{C}(S)$, nên nó trùng với $\mathscr{C}(S)$ theo TG, X, p. 40, Hệ quả 1.

Mệnh đề thứ hai là một hệ quả của mệnh đề thứ nhất, áp dụng cho các phần tử Hermit $x=aa^*$ và $y=a^*a$, có lưu ý đến sự kiện rằng Sp$'(a^*a) =$ Sp$'(aa^*)$ (Mệnh đề 1 của I, p. 5).

### 8. Phép tính phiếm hàm trong một đại số không có đơn vị

Cho A là một đại số đối hợp và gọi $\widetilde{A}$ là đại số đối hợp có đơn vị suy ra từ A bằng phép nối một phần tử đơn vị $e$. Ký hiệu bởi $\pi$ đặc trưng Hermit $x+\lambda e\mapsto \lambda$ của $\widetilde{A}$ vào $\mathbf{C}$; ta có Ker($\pi$ ) $= A$.

Cho $x\in A$ là một phần tử chuẩn tắc. Nó chuẩn tắc trong $\widetilde{A}$ và Sp$_{\widetilde{A}}(x) =$ Sp$'_A(x)$. Ký hiệu bởi $\mathscr{C}'$(Sp$'_A(x)$) đại số sao của các hàm liên tục $f$ trên Sp$'_A(x)$ sao cho $f(0) = 0$.

Cho $f\in \mathscr{C}$ (Sp$'_A(x)$). Vì $\pi (f(x)) =f(\pi (x))$ (mệnh đề 8 của I, p. 112), ta có $f(x)\in A$ khi và chỉ khi $f(0) = 0$. Ánh xạ $f\mapsto f(x)$ xác định một cấu xạ của các đại số có đối hợp từ đại số sao $\mathscr{C}'$(Sp$'_A(x)$) vào A mà ảnh của ánh xạ đồng nhất $z$ của Sp$'_A(x)$ là $x$. Cấu xạ này là đẳng cự và ảnh của nó là đại số con sao của A sinh bởi $x$.

#### Mệnh đề 12 {#ts-i-s6-prop-12 .statement tag=02E9}

Ánh xạ $f\mapsto f(x)$ là cấu xạ duy nhất của các đại số có đối hợp từ đại số sao $\mathscr{C}'$(Sp$'_A(x)$) vào A sao cho ánh xạ đồng nhất $z$ của Sp$'_A(x)$ có ảnh là $x$.

Các phần tử $z$ và $\overline{z}$ của $\mathscr{C}'$(Sp$'_A(x)$) sinh một đại số con trù mật của $\mathscr{C}'$(Sp$'_A(x)$) (xem TG, X, p. 40, hệ quả 2). Vì mọi cấu xạ của các đại số có đối hợp từ đại số sao $\mathscr{C}'$(Sp$'_A(x)$) vào đại số sao A đều liên tục (I, p. 104, mệnh đề 2), kết quả suy ra.

Các kết quả của số trước liên quan đến phép tính phiếm hàm được mở rộng sang trường hợp tổng quát. Ta sẽ chỉ phát biểu chúng và để bạn đọc tự hoàn thành các chứng minh, mutatis mutandis.

#### Mệnh đề 13 {#ts-i-s6-prop-13 .statement tag=02EA}

Ta có các tính chất sau:

a) Với mọi $f\in \mathscr{C}'$(Sp$'_A(x)$), ta có Sp$'_A(f(x)) =f$(Sp$'_A(x)$) ;

b) Với mọi $f\in \mathscr{C}'$(Sp$'_A(x)$) và với mọi $g\in \mathscr{C}'$(Sp$'_A(f(x))$), ta có $(g\circ f)(x) =g(f(x))$ ;

c) Cho $A'$ là một đại số sao và $\pi$ là một cấu xạ từ A vào $A'$; khi đó $\pi (x)$ là chuẩn tắc trong $A'$, ta có Sp$'_{A'}(\pi (x))\subset$ Sp$'_A(x)$ và $\pi (f(x)) =f(\pi (x))$ với mọi $f\in \mathscr{C}'$(Sp$'_A(x)$);

d) Nếu A giao hoán, và nếu $f\in \mathscr{C}'$(Sp$'_A(x)$), thì $\mathscr{G}'_A(f(x)) =$ $f\circ \mathscr{G}'_A(x)$.

#### Nhận xét {#ts-i-s6-n8-rem-1 .statement tag=02EB}

Cho A là một đại số involutive có đơn vị và gọi $\widetilde{A}$ là đại số involutive có đơn vị suy ra từ A bằng phép nối một phần tử đơn vị $e$. Với mọi $x\in A$, ta có Sp$'_A(x) =$ Sp$_A(x)\cup  \{0\}$. Gọi $x$ là một phần tử chuẩn tắc của A. Khi đó nó là một phần tử chuẩn tắc của $\widetilde{A}$, và do đó ta có hai ánh xạ phép tính phiếm hàm trong A, ánh xạ thứ nhất được xác định trên $\mathscr{C}$ (Sp$_A(x)$) và ánh xạ thứ hai trên $\mathscr{C}'$(Sp$'_A(x)$). Gọi $f'\in \mathscr{C}'$(Sp$'_A(x)$); nếu $f$ ký hiệu hạn chế của nó trên Sp$_A(x)$, thì khi đó ta có $f'(x) =f(x)$.

### 9. Các Phần Tử Dương Trong Các Đại Số Involutive

#### Định nghĩa 6 {#ts-i-s6-def-6 .statement tag=02EC}

Cho A là một đại số involutive. Một phần tử $x$ của A được gọi là dương nếu nó là Hermit và nếu Sp$'_A(x)\subset \mathbf{R}_+$. Tập hợp các phần tử dương của A được ký hiệu là $A_+$. Nó là một tập con của $A_h$.

Ta viết $x\geqslant y$ nếu $x-y\in A_+$.

Nếu đại số involutive A có đơn vị, thì phần tử đơn vị của nó là dương.

Nếu B là một đại số con involutive của A, ta có $B_+= B\cap A_+$ (hệ quả của mệnh đề 5 của I, p. 106).

Nếu $\pi : A\rightarrow$ B là một cấu xạ của các đại số involutive, thì $\pi (A_+)\subset B_+$.

#### Ví dụ 1 {#ts-i-s6-n9-exa-1 .statement tag=02ED}

Cho X là một không gian địa phương compact. Trong đại số involutive $\mathscr{C}_0(X)$ của các hàm liên tục trên X tiến tới 0 ở vô cùng, tương ứng trong đại số involutive $\mathscr{C}_b(X)$ của các hàm liên tục bị chặn, một hàm $f$ là một phần tử dương khi và chỉ khi nó nhận giá trị thực và nếu $f(x)\geqslant 0$ với mọi $x\in X$ (xem ví dụ 3 của I, p. 17).

#### Ví dụ 2 {#ts-i-s6-n9-exa-2 .statement tag=02EE}

Cho A là một đại số involutive giao hoán. Gọi $a$ là một phần tử của A. Vì Sp$'_A(x)$ là hợp của $\{0\}$ và của ảnh của biến đổi Gelfand $\mathscr{G}(a)$ (mệnh đề 6 của I, p. 37), phần tử $a$ là dương khi và chỉ khi biến đổi Gelfand $\mathscr{G}(a)$ là một hàm dương.

#### Ví dụ 3 {#ts-i-s6-n9-exa-3 .statement tag=02EF}

Cho E là một không gian Hilbert phức. Một phần tử $x$ của đại số involutive $\mathscr{L}(E)$ (ví dụ 1 của I, p. 102) là dương khi và chỉ khi nó là một tự đồng cấu dương của E theo nghĩa của EVT, V, p. 45, đn. 6 (mệnh đề 8 của I, p. 138).

#### Bổ đề 12 {#ts-i-s6-lem-12 .statement tag=02EG}

Cho A là một đại số involutive có đơn vị và gọi $x\in A$ là một phần tử Hermit.

a) Phần tử $x$ là dương khi và chỉ khi $\|\|x\| \cdot 1-x\|\leqslant \|x\|$;

b) Nếu $\|x\|\leqslant 1$, thì $x$ là dương khi và chỉ khi $\|1-x\|\leqslant 1$ ;

c) Nếu $x$ là dương, thì $1-x$ là dương khi và chỉ khi $\|x\|\leqslant 1$ ;

d) Nếu $x$ là dương và nếu $y\in A_+$ giao hoán với $x$, thì $xy$ là dương.

Phần tử $x$ là Hermit, do đó chuẩn tắc. Bằng cách xét đại số con involutive sinh bởi $x$, vốn giao hoán, ta quy được về trường hợp đại số A là giao hoán, nghĩa là về trường hợp A = $\mathscr{C}_0(X)$ với X là một không gian tôpô địa phương compact (định lý 1 của I, p. 108). Ba mệnh đề đầu khi đó suy ra ngay lập tức từ ví dụ 1 ở trên. Tương tự, để bây giờ chứng minh mệnh đề d), ta có thể xét đại số con involutive sinh bởi $x$ và $y$, vốn giao hoán.

#### Mệnh đề 14 {#ts-i-s6-prop-14 .statement tag=02EH}

Cho A là một đại số involutive. Tập $A_+$ là một nón lồi lồi, đóng, nhọn và có đỉnh trong không gian Banach thực $A_h$ (EVT, II, p. 11).

Gọi $\widetilde{A}$ là đại số có phép đối hợp suy ra từ A bằng phép nối một phần tử đơn vị. Vì $A_+= A\cap \widetilde{A}_+$, chỉ cần chứng minh mệnh đề đối với $\widetilde{A}$. Do đó ta có thể giả sử rằng A có một phần tử đơn vị.

Ta có $0\in A_+$. Với mọi $\lambda \in \mathbf{R}_+^*$ và mọi $x\in A$, ta có Sp$'_A(\lambda x) =$ $\lambda$ Sp$'_A(x)$, điều này suy ra rằng $A_+$ là một nón trong không gian Banach thực $A_h$.

Để chứng tỏ rằng $A_+$ là lồi, chỉ cần chứng tỏ rằng nếu $x$ và $y$ là dương, thì $x+y\geqslant 0$ (EVT, II, p. 11, mệnh đề 10). Bằng phép vị tự, chỉ cần chứng minh rằng nếu $x\geqslant 0$ và $y\geqslant 0$ hơn nữa thỏa mãn $\|x\|\leqslant 1$, $\|y\|\leqslant 1$, thì phần tử $\frac{1}{2}(x+y)$ là dương. Bây giờ ta có

$$
\|1-\frac{1}{2}(x+y)\|\leqslant \frac{1}{2}\|1-x\|+\frac{1}{2}\|1-y\|\leqslant 1
$$

theo mệnh đề b) của bổ đề 12, và chính mệnh đề đó khi ấy cho thấy rằng $\frac{1}{2}(x+y)$ là dương.

Sau cùng, mệnh đề a) của bổ đề 12 cũng suy ra rằng $A_+$ là đóng.

Vì $A_+$ là một nón nhọn trong $A_h$, nó là lồi nhọn nếu và chỉ nếu $A_+\cap (-A_+)$ thu về 0. Nhưng nếu $x\in A_+\cap (-A_+)$, ta có Sp$'_A(x) =$ $\{0\}$, do đó $\varrho (x) = 0$, và $\|x\|= 0$ vì $x$ là Hermit (bổ đề 7, (2) của I, p. 104), do đó $x= 0$.

Mệnh đề 14 có nghĩa là quan hệ “ $x\geqslant y$ ” là một quan hệ thứ tự trên $A_h$ (EVT, II, p. 13, mệnh đề 13).

#### Mệnh đề 15 {#ts-i-s6-prop-15 .statement tag=02EI}

Cho A là một đại số có phép đối hợp. Cho $x$ là một phần tử chuẩn tắc của A.

a) Giả sử rằng A có đơn vị và cho $f$ là một hàm liên tục từ Sp$_A(x)$ vào $\mathbf{C}$. Điều kiện cần và đủ để $f(x)$ là dương là ảnh của $f$ được chứa trong $\mathbf{R}_+$;

b) Cho $f$ là một hàm liên tục từ Sp$'_A(x)$ vào $\mathbf{C}$ sao cho $f(0) =$ 0. Điều kiện cần và đủ để $f(x)$ là một phần tử dương của A là ảnh của $f$ được chứa trong $\mathbf{R}_+$.

Mệnh đề a) suy ra từ mệnh đề a) của hệ quả 2 của I, p. 111, và mệnh đề b) suy ra từ mệnh đề 13 của I, p. 114.

Cho $x$ là một phần tử Hermit của đại số có phép đối hợp A. Phổ của nó được chứa trong $\mathbf{R}$ (mệnh đề 4 của I, p. 106). Xét các hàm liên tục từ Sp$'_A(x)$ vào $\mathbf{R}$ được xác định bởi

$f_1:t\mapsto$ sup($t,0$)$,f_2:t\mapsto$ sup($-t,0$)$,f_3:t\mapsto  |t|$.

Ta đặt

$$
x^+=f_1(x),x^-=f_2(x),|x|=f_3(x) \tag{3}
$$

Vì các hàm $f_1,f_2,f_3$ nhận các giá trị thực dương và triệt tiêu tại 0, nên các phần tử $x^+,x^-$ và $|x|$ là những phần tử dương của A (Mệnh đề 15, a)) thuộc đại số con sao của A sinh bởi $x$.

Ta có $f_1(t)-f_2(t) =t$ với mọi $t\in \mathbf{R}$, cũng như các hệ thức $f_1+f_2=f_3$ và $f_1f_2= 0$. Do đó có các hệ thức:

$$
x=x^+-x^-,|x|=x^++x^-,x^+x^-=x^-x^+= 0 \tag{4}
$$

Vì ánh xạ phép tính phiếm hàm là đẳng cự, ta có

$$
\| |x| \|=\|x\|,\|x^+\|\leqslant \|x\|,\|x^-\|\leqslant \|x\|
$$

Cho $x$ là một phần tử dương của A. Nó là Hermit, nên chuẩn tắc. Cho $\alpha \in \mathbf{R}^*_+$, và gọi $g$ là hạn chế lên Sp$'_A(x)$ của hàm $t\mapsto t^{\alpha}$; ta viết $x^{\alpha}=g(x)$. Đó là một phần tử dương của đại số con sao của A sinh bởi $x$. Cho $\alpha$ và $\beta$ thuộc $\mathbf{R}^*_+$. Vì ánh xạ phép tính phiếm hàm là một cấu xạ đại số, và theo Mệnh đề 13 của I, p. 114, ta có

$$
x^{\alpha}x^{\beta}=x^{\alpha+\beta}(x^{\alpha})^{\beta}=x^{\alpha \beta} \tag{5}
$$

$$
\surd_/
$$

Ta cũng sẽ viết $\overline{x}=x^{12}$.

#### Mệnh đề 16 {#ts-i-s6-prop-16 .statement tag=02EJ}

Cho $x$ là một phần tử dương của A. Cho $\alpha \in \mathbf{R}^*_+$. Khi đó $x^{1/\alpha}$ là phần tử dương duy nhất $y$ của A sao cho $y^{\alpha}=x$.

Ở trên đã thấy rằng $x^{1/\alpha}$ thỏa mãn các tính chất cần có. Ngược lại, cho $y$ là một phần tử dương của A sao cho $y^{\alpha}=x$. Theo công thức (5), ta có $y= (y^{\alpha})^{1/\alpha}=x^{1/\alpha}$, điều phải chứng minh.

#### Bổ đề 13 {#ts-i-s6-lem-13 .statement tag=02EK}

Cho A là một đại số sao có đơn vị. Mọi phần tử của A đều là một tổng của các phần tử unita.

Theo bổ đềCho $x$ là một phần tử Hermit của12, c), ta có $1-\frac{1}{4}Ax$. Trước hết giả sử rằng$_2\in A_+$. Đặt $y=\frac{1}{2}x+i\surd\|1x-\|\leqslant_{1\overline{4}}x2_2$..

Ta có $y^*=\frac{1}{2}x-i\surd\overline{1 -\frac{1}{4}x^2}$, do đó $yy^*= 1$ và $x=y+y^*$ là một tổng của hai phần tử unita. Trong trường hợp tổng quát, cho $k$ là một số nguyên sao cho $\|\frac{1}{k}x\|\leqslant 2$ ; khi đó phần tử $x$ là tổng của $2k$ phần tử unita. Theo Bổ đề 2 của I, p. 96, bổ đề được chứng minh.

#### Định lý 2 {#ts-i-s6-thm-2 .statement tag=02EL}

Cho A là một đại số sao. Một phần tử $x$ của A là dương nếu và chỉ nếu tồn tại $y\in A$ sao cho $x=y^*y$.

Giả sử $x$ là dương. Đặt $y=x^{1/2}$; đó là một phần tử Hermit của A và ta có $y^*y=y^2=x$.

Ngược lại, cho $y$ là một phần tử của A và đặt $x=y^*y$. Đó là một phần tử Hermit của A. Ta sẽ chứng minh rằng $x$ là dương. Để làm điều đó, ta viết $z=x^-$ và đặt $w=yz$. Khi đó ta có

$$
w^*w=z^*y^*yz=zxz=z(x^+-z)z=-z^3
$$

Vì $z\geqslant 0$, ta có $z^3\geqslant 0$, và do đó suy ra Sp$'_A(w^*w)\subset \mathbf{R}_-$. Hãy viết $w=w_1+iw_2$ trong đó $w_1$ và $w_2$ là Hermit (Bổ đề 2 của I, p. 96). Các phần tử $w^2_1$ và $w_2^2$ là dương. Ta có $ww^*+w^*w=$ $2w^2_1+ 2w_2^2$, và vì thế Mệnh đề 14 cho thấy rằng $ww^*= 2w_1^2+ 2w^2_2+ (-w^*w)$ là dương. Vì Sp$'_A(ww^*) =$ Sp$'_A(w^*w)$ (I, p. 5, Mệnh đề 1), được chứa trong $\mathbf{R}_-$, ta kết luận rằng Sp$'_A(w^*w) =\{0\}$. Vì $w^*w$ là Hermit, điều này kéo theo (Hệ quả 1 của I, p. 108) rằng $\|w^*w\|=\varrho (w^*w) = 0$, do đó $z^3= 0$. Vì $z$ là Hermit, ta có $z= 0$. Vậy, $x=x^+$ là dương.

#### Nhận xét {#ts-i-s6-n9-rem-1 .statement tag=02EM}

Cho A là một đại số có phép đối hợp và cho $x\in A$. Phần tử $x^*x$ của A là dương; khi đó người ta đặt $|x|= (x^*x)^{1/2}$. Ta có $\|x\|^2=\|x^*x\|=$ $\||x|^2\|=\||x|\|^2$, do đó $\|x\|=\||x|\|$.

Khi $x$ là chuẩn tắc, ta cũng có $|x|=f(x)$, trong đó $f$ là ánh xạ từ $\mathbf{C}$ vào $\mathbf{C}$, bằng không tại 0, cho bởi $f(z) =|z|$. Đặc biệt, khi $x$ là Hermit, $|x|$ trùng với phần tử được định nghĩa bởi công thức (3).

Giả sử hơn nữa rằng A có đơn vị và $x$ khả nghịch. Khi đó $|x|$ cũng khả nghịch, phần tử $u=x|x|^{-1}$ là unita và ta có $x=u|x|$ ("phân tích cực"; xem thêm I, p. 139, n$^o8$ cho trường hợp các tự đồng cấu của các không gian Hilbert).

#### Bổ đề 14 {#ts-i-s6-lem-14 .statement tag=02EN}

Cho A là một đại số có phép đối hợp, và cho $x$ và $y$ là các phần tử Hermit của A.

a) Nếu $x\leqslant y$, thì với mọi phần tử $w$ của A, ta có $w^*xw\leqslant w^*yw$. Đặc biệt, nếu $y\geqslant 0$, ta có $w^*yw\geqslant 0$;

b) Giả sử rằng A có đơn vị. Nếu $0\leqslant x\leqslant y$ và nếu $x$ khả nghịch, thì $y$ khả nghịch và $y^{-1}\leqslant x^{-1}$;

c) Nếu $0\leqslant x\leqslant y$ thì $\|x\|\leqslant \|y\|$.

Đặt $u= (y-x)^{1/2}$. Ta có $w^*yw-w^*xw=w^*u^2w= (uw)^*(uw)$, và mệnh đề a) suy ra từ Định lý 2.

Hãy chứng minh mệnh đề b). Trước hết giả sử rằng $x= 1$. Gọi B là *-đại số con có đơn vị sinh bởi $y$. Theo đẳng cấu Gelfand, $y$ tương ứng với một hàm liên tục $\geqslant 1$ trên không gian compact $\mathsf{X}(B)$. Do đó hàm này khả nghịch và nghịch đảo của nó là $\leqslant 1$. Điều này kéo theo rằng $y$ khả nghịch và $y^{-1}\leqslant 1 =x^{-1}$. Trong trường hợp tổng quát, ta nhận thấy rằng $0\leqslant 1\leqslant x^{-1/2}yx^{-1/2}$ theo a), nên trường hợp trước kéo theo rằng $z=x^{-1/2}yx^{-1/2}$ khả nghịch và $z^{-1}\leqslant 1$. Vì thế $y$ khả nghịch và $y^{-1}\leqslant x^{-1}$, lại theo a).

Để chứng minh mệnh đề c), có thể giả sử rằng A có đơn vị (Mệnh đề 3 của I, p. 105). Trước hết giả sử rằng $y$ khả nghịch. Đặt

$$
\surd -_{1-1}
$$

$b=y$. Theo a), các điều kiện $0\leqslant x\leqslant y$ kéo theo $0\leqslant bxb\leqslant$ $b^{-1}yb^{-1}= 1$, do đó $\|b^{-1}xb^{-1}\|\leqslant 1$ theo Bổ đề 12, c) của I, p. 116. Khi đó ta có

$$
\|x\|=\|b(b^{-1}xb^{-1})b\|\leqslant \|b\|\|b^{-1}xb^{-1}\|\|b\|\leqslant \|b\|^2=\|b^2\|=\|y\|
$$

Trong trường hợp tổng quát, với mọi số thực $\varepsilon  >0$, phần tử $y+\varepsilon$ là khả nghịch và $0\leqslant x\leqslant y+\varepsilon$. Theo điều trước đó, do đó ta có $\|x\|\leqslant \|y+\varepsilon \|$ với mọi số thực $\varepsilon  >0$, do đó có kết quả.

#### Nhận xét {#ts-i-s6-n9-rem-2 .statement tag=02EO}

Nói chung, nếu $x$ và $y$ là các phần tử dương của một *-đại số A, thì điều kiện $0\leqslant x\leqslant y$ không kéo theo $x^2\leqslant y^2($xem bài tập 15 của I, p. 182).

### 10. Các Phần Tử Đơn Vị Xấp Xỉ Trong Các *-Đại Số

#### Định nghĩa 7 {#ts-i-s6-def-7 .statement tag=02EP}

Cho A là một đại số định chuẩn. Một phần tử đơn vị xấp xỉ của A là một cơ sở lọc $\mathfrak{F}$ trên quả cầu đơn vị của A sao cho, với mọi $x$ trong A, các cơ sở lọc $x\mathfrak{F}$ và $\mathfrak{F}x$ trên A hội tụ đến $x$, nói cách khác:

lim$_{f,\mathfrak{F}}f x=$ lim$_{f,\mathfrak{F}}xf=x$.

Nếu A là một *-đại số, thì một phần tử đơn vị xấp xỉ $\mathfrak{F}$ được gọi là tăng nếu $\mathfrak{F}$ là một cơ sở lọc trên $A_+$.

Cho A là một *-đại số. Ta ký hiệu $A^{\leqslant 1}_+$ (resp. $A^{<1}_+$) là tập hợp các phần tử dương của A có chuẩn $\leqslant 1$ (resp. có chuẩn $<1$); đó là các phần tử Hermit của A có phổ được chứa trong $[0,1]$ (resp. trong $[0,1[$).

#### Mệnh đề 17 {#ts-i-s6-prop-17 .statement tag=02EQ}

Cho A là một *-đại số, và cho $\mathfrak{F}$ là một cơ sở lọc trên $A^{\leqslant 1}_+$. Để $\mathfrak{F}$ là một phần tử đơn vị xấp xỉ tăng của A, điều kiện cần và đủ là ta có

lim$_{f,\mathfrak{F}}f x=x$

với mọi phần tử dương $x$ của A.

Điều kiện đó hiển nhiên là cần; hãy chứng minh rằng nó là đủ. Gọi $\widetilde{A}$ là *-đại số suy ra từ A bằng phép nối một phần tử đơn vị. Cho $x$ là một phần tử của A và cho $f\in A^{\leqslant 1}_+$. Ta có

$$
\|f x-x\|^2=\|(f x-x)(f x-x)^*\|=\|(f-1)xx^*(f-1)\|
$$

$$
\leqslant \|(f-1)xx^*\|
$$

vì $\|f-1\|\leqslant 1$ (Bổ đề 12, c) của I, p. 116). Do đó ta có

lim sup$_{f,\mathfrak{F}}\|f x-x\|^2\leqslant$ lim sup$_{f,\mathfrak{F}}\|f xx^*-xx^*\|$. Vì $xx^*$ là dương (Định lý 2 của I, p. 118), giả thiết kéo theo rằng

lim sup$_{f,\mathfrak{F}}\|f x-x\|^2\leqslant \|xx^*-xx^*\|= 0$,

nên

lim$_{f,\mathfrak{F}}f x=x$.

Vì phép đối hợp của A là liên tục và vì $\mathfrak{F}$ là một cơ sở lọc trên $A_h$, ta có

lim$_{f,\mathfrak{F}}xf=$ lim$_{f,\mathfrak{F}}(f^*x^*)^*=$ lim$_{f,\mathfrak{F}}(f x^*)^*= (x^*)^*=x$.

Mệnh đề được suy ra.

#### Mệnh đề 18 {#ts-i-s6-prop-18 .statement tag=02ER}

Cho A là một đại số có đối hợp. Tập hợp có thứ tự $A^{<1}_+$ có hướng sang phải (E, III, p. 12, def. 7), và lọc các thiết diện của nó (TG, I, p. 38, ví dụ 2) là một đơn vị xấp xỉ tăng của A.

Gọi $\widetilde{A}$ là đại số có đối hợp suy ra từ A bằng phép nối một phần tử đơn vị ký hiệu là 1 (def. 4 of I, p. 106).

Gọi $g$ là hàm từ $[0,1[$ vào $\mathbf{R}_+$ được định nghĩa bởi $g(t) =t(1-t)^{-1}$. Đây là một song ánh liên tục tăng, song ánh ngược của nó được cho bởi $t\mapsto 1-(1 +t)^{-1}$.

Ta chứng minh rằng tập hợp có thứ tự $A^{<1}_+$ có hướng sang phải. Gọi $x$ và $y$ là các phần tử của $A^{<1}_+$. Vì $g(0) = 0$ và vì Sp$'_A(x)$ và Sp$'_A(y)$ được chứa trong $[0,1[$, các phần tử $g(x)$ và $g(y)$ được xác định; chúng là dương, nên $g(x) +g(y)\geqslant 0$. Do đó ta có thể lập phần tử $z=g^{-1}(g(x) +g(y))$ của A. Ta có Sp$'_A(z)\subset [0,1[$, và vì thế $z\in A^{<1}_+$.

Ta có $0\leqslant g(x)\leqslant g(z)$, do đó $1\leqslant 1+g(x)\leqslant 1+g(z)$. Mệnh đề b) của bổ đề 14 ở I, p. 119 suy ra rằng $1 +g(x)$ và $1 +g(z)$ là khả nghịch và rằng $(1 +g(z))^{-1}\leqslant (1 +g(x))^{-1}$. Do đó, $z= 1-(1 +g(z))^{-1}\geqslant$ $1-(1 +g(x))^{-1}=x$. Tương tự, ta có $z\geqslant y$. Hệ quả là, $z$ là một cận trên của $x$ và $y$ trong $A^{<1}_+$. Vậy tập hợp có thứ tự $A^{<1}_+$ có hướng sang phải. Ta ký hiệu bởi $\mathfrak{F}$ lọc các thiết diện của nó

Gọi $x$ là một phần tử dương của A. Với mọi số nguyên $n\geqslant 1$, đặt $e_n=$ $g^{-1}(nx)$; ta có $e_n\in A^{<1}_+$. Gọi $h_n$ là hàm liên tục trên $\mathbf{R}_+$ được định nghĩa, với mọi $t\in \mathbf{R}_+$, bởi $h_n(t) =t^2(1-g^{-1}(nt)) =t^2/(1 +nt)$. Ta có $|h_n(t)|\leqslant t/n$ với mọi $t\geqslant 0$, và vì thế $\|x(1-e_n)x\|=\|h_n(x)\|\leqslant$ $\|x\|/n$. Đặc biệt, $x(1-e_n)x$ tiến tới 0 khi $n$ tiến ra vô cùng.

Cho $\varepsilon  >0$ là một số thực. Cho $n$ là một số nguyên sao cho $\|x(1-e_n)x\|< \varepsilon$. Với mọi $f\in A^{<1}_+$ sao cho $f\geqslant e_n$, khi đó ta có

$$
\|x-f x\|^2=\|(1-f)x\|^2=\|((1-f)x)^*(1-f)x\|=\|x^*(1-f)^2x\|
$$

$$
=\|x(1-f)^2x\|
$$

Hơn nữa, vì $0\leqslant f\leqslant 1$, ta có $(1-f)-(1-f)^2= (1-f)f\geqslant 0$ (Bổ đề 12, d) của I, p. 116), do đó $(1-f)^2\leqslant 1-f$. Vì $1-f\leqslant 1-e_n$, suy ra $0\leqslant (1-f)^2\leqslant 1-e_n$. Theo Bổ đề 14, a) và c) của I, p. 119, suy ra

$$
\|x-f x\|^2=\|x(1-f)^2x\|\leqslant \|x(1-e_n)x\|< \varepsilon
$$

Vậy lim$_{f,\mathfrak{F}}f x=x$ với mọi $x\in A_+$. Do đó bộ lọc $\mathfrak{F}$ là một đơn vị xấp xỉ của A theo Mệnh đề 17.

### 11. Thương bởi một iđêan hai phía đóng

#### Bổ đề 15 {#ts-i-s6-lem-15 .statement tag=02ES}

Cho A là một đại số stellar và cho I là một iđêan hai phía đóng của A. Khi đó I là tự liên hợp.

Cho $J = I\cap I^*$. Tập hợp J là một iđêan hai phía tự liên hợp của A, chứa $I^*I$. Đặc biệt, J là một đại số stellar. Cho $\mathfrak{F}$ là một đơn vị xấp xỉ tăng của J (Mệnh đề 18 của I, p. 121). Với mọi $x\in I$ và mọi $f\in J^{\leqslant 1}_+$, ta có

$$
\|xf-x\|^2=\|(xf-x)^*(xf-x)\|=\|f(x^*xf-x^*x)-(x^*xf-x^*x)\|
$$

$$
\leqslant 2\|x^*xf-x^*x\|
$$

Vì $x^*x\in J$, do đó ta có

lim$_{f,\mathfrak{F}}\|xf-x\|^2= 0$.

Vì $xf\in J$ với mọi $f\in J^{\leqslant 1}_+$ và vì J là đóng, điều đó suy ra $x\in J$. Vậy I = J, và iđêan I là tự liên hợp.

#### Mệnh đề 19 {#ts-i-s6-prop-19 .statement tag=02ET}

Cho A là một đại số stellar và cho I là một iđêan hai phía đóng của A. Khi đó đại số Banach có phép đối hợp thương $A/I$ là một đại số stellar.

Iđêan I là tự liên hợp (Bổ đề 15). Xét đại số stellar $\widetilde{A}$ suy ra từ A bằng phép nối thêm một phần tử đơn vị (Định nghĩa 4 của I, p. 106). Trong đại số này, tập hợp I là một iđêan hai phía đóng tự liên hợp, và $A/I$ đồng nhất với một đại số con có phép đối hợp đóng của $\widetilde{A}/I$. Do đó có thể giả sử rằng A có đơn vị.

Đại số Banach $A/I$ có phép đối hợp. Cho $\pi : A\rightarrow A/I$ là phép chiếu chính tắc. Iđêan hai phía tự liên hợp I là một đại số con stellar của A. Cho $\mathfrak{F}$ là một đơn vị xấp xỉ tăng của I (Mệnh đề 18 của I, p. 121). Trước hết ta sẽ chỉ ra rằng với mọi $x\in A$, ta có

(6) $\|\pi (x)\|_{A/I}=$ lim$_{f,\mathfrak{F}}\|x-xf\|$.

Một mặt, vì $xf\in I$ với mọi $f\in I^{\leqslant 1}_+$, ta có

$\|\pi (x)\|_{A/I}=$ inf$_{a\in I}\|x-a\|\leqslant$ lim inf$_{f,\mathfrak{F}}\|x-xf\|$.

Mặt khác, với mọi $a\in I$, ta có

$$
\|x-xf\|\leqslant \|(x-a)-(x-a)f\|+\|a-af\|
$$

$$
=\|(x-a)(1-f)\|+\|a-af\|
$$

và do đó, vì $\|1-f\|\leqslant 1$ (Bổ đề 12 của I, p. 116) và $a\in I$, suy ra rằng

lim sup$_{f,\mathfrak{F}}\|x-xf\|\leqslant \|x-a\|$.

Vậy suy ra lim sup$_{f,\mathfrak{F}}\|x-xf\|\leqslant \|\pi (x)\|_{A/I}$ vì $a$ là tùy ý trong I. Công thức (6) do đó được chứng minh.

Bây giờ cho $x$ là một phần tử của A. Theo công thức (6), ta có

$\|\pi (x)\|^2_{A/I}=$ lim$_{f,\mathfrak{F}}\|x-xf\|^2=$ lim$_{f,\mathfrak{F}}\|x(1-f)\|^2$

= lim$_{f,\mathfrak{F}}\|(1-f)x^*x(1-f)\|\leqslant$ lim$_{f,\mathfrak{F}}\|x^*x(1-f)\|=\|\pi (x^*x)\|_{A/I}$.

Khi đó Bổ đề 6 của I, p. 103 suy ra rằng đại số Banach có phép đối hợp thương $A/I$ là một đại số stellar.

### 12. Đại số stellar bao của một đại số Banach có phép đối hợp

#### Bổ đề 16 {#ts-i-s6-lem-16 .statement tag=02EU}

Cho A là một đại số có phép đối hợp và cho $p$ là một nửa chuẩn trên A. Các điều kiện sau là tương đương :

(i) Ta có $p(xy)\leqslant p(x)p(y),p(x^*) =p(x)$ và $p(x)^2=p(x^*x)$ với mọi $x, y\in A$;

(ii) Tập hợp R các phần tử $x$ của A sao cho $p(x) = 0$ là một iđêan hai phía tự liên hợp của A, và nửa chuẩn trên $A/R$ cảm sinh bởi $p$ biến $A/R$ thành một đại số có đối hợp có chuẩn mà đầy đủ hóa của nó là một đại số stellar;

(iii) Tồn tại một đại số stellar B và một cấu xạ $\varphi$ của các đại số có đối hợp từ A vào B sao cho $p(x) =\|\varphi (x)\|$ với mọi $x\in A$.

Các suy ra (i)$=\Rightarrow$ (ii)$=\Rightarrow$ (iii)$=\Rightarrow$ (i) đều sơ cấp.

Một nửa chuẩn thỏa mãn các điều kiện của bổ đề 16 sẽ được gọi là một nửa chuẩn stellar trên đại số có đối hợp A.

Cho A là một đại số có đối hợp có chuẩn và gọi S là tập hợp các nửa chuẩn stellar trên A. Ta có $p(x)\leqslant \|x\|$ với mọi $x\in A$ và mọi $p\in S$ (I, p. 104, mệnh đề 2). Ánh xạ $x\mapsto  \|x\|_*=$ sup$_{p\in S}p(x)$ là một

nửa chuẩn stellar trên A. Nó là nửa chuẩn stellar lớn nhất trên A.

Gọi R là tập hợp các $x\in A$ sao cho $\|x\|_*= 0$. Nó là một iđêan hai phía đóng của A. Ta ký hiệu bởi Stell(A) đại số stellar đầy đủ hóa của $A/R$ đối với chuẩn cảm sinh bởi $x\mapsto  \|x\|_*$ (bổ đề 16, (ii)). Ánh xạ chính tắc từ A vào Stell(A) là liên tục, ảnh của nó trù mật trong Stell(A) và hạt nhân của nó bằng R.

#### Định nghĩa 8 {#ts-i-s6-def-8 .statement tag=02EV}

Đại số stellar Stell(A) được gọi là đại số stellar bao của đại số có đối hợp có chuẩn A.

Nếu A giao hoán, thì Stell(A) giao hoán; nếu A có đơn vị, thì Stell(A) có đơn vị.

#### Mệnh đề 20 {#ts-i-s6-prop-20 .statement tag=02EW}

Cho A là một đại số có đối hợp có chuẩn và gọi $j$ là cấu xạ chính tắc từ A vào Stell(A). Với mọi đại số stellar B và mọi cấu xạ $\varphi$ của các đại số có đối hợp từ A vào B, tồn tại một cấu xạ duy nhất $\varphi '$ của các đại số stellar từ Stell(A) vào B sao cho $\varphi =\varphi '\circ j$.

Ta ký hiệu bởi $x\mapsto  \|x\|_*$ chuẩn trên Stell(A). Gọi R là hạt nhân của $j$. Ánh xạ $x\mapsto  \|\varphi (x)\|$ là một nửa chuẩn stellar trên A. Do đó ta có $\|\varphi (x)\|\leqslant \|x\|_*$ với mọi $x\in A$. Bởi vậy, bằng cách chuyển qua thương, cấu xạ $\varphi$ xác định một cấu xạ liên tục từ $A/R$ vào B, cấu xạ này được kéo dài bằng tính liên tục thành một cấu xạ $\varphi '$ từ Stell(A) vào B thỏa mãn $\varphi =\varphi '\circ j$. Tính duy nhất của $\varphi '$ suy ra từ việc ảnh của $j$ trù mật trong Stell(A).

#### Hệ quả {#ts-i-s6-n12-cor-1 .statement tag=02EX}

Cho A là một đại số Banach có đối hợp giao hoán và $j$ là cấu xạ chính tắc từ A vào Stell(A). Ánh xạ $\mathsf{X}(j)$ là một đồng phôi của $\mathsf{X}$(Stell(A)) lên không gian con $\mathsf{X}(A)_h$ của $\mathsf{X}(A)$ gồm các đặc trưng Hermit của A.

Các đặc trưng Hermit của A là các cấu xạ của các đại số có đối hợp từ A vào đại số stellar $\mathbf{C}$. Vì thế mệnh đề 20 kéo theo rằng $\mathsf{X}(j)$ là một song ánh từ $\mathsf{X}$(Stell(A)) lên $\mathsf{X}(A)_h$. Vì $\mathsf{X}(j)$ là một đồng phôi lên ảnh của nó (xem I, p. 10), hệ quả được chứng minh.

Ta đồng nhất $\mathsf{X}$(Stell(A)) với $\mathsf{X}(A)_h$ nhờ ánh xạ $\mathsf{X}(j)$. Với mọi $x\in$ A, ánh xạ $\mathscr{G}_{Stell(A)}(j(x))$ không là gì khác ngoài hạn chế của $\mathscr{G}_A(x)$ trên $\mathsf{X}(A)_h$.

#### Mệnh đề 21 {#ts-i-s6-prop-21 .statement tag=02EY}

Cho A là một đại số Banach có đối hợp và $j$ là cấu xạ chính tắc từ A vào Stell(A). Căn của A được chứa trong hạt nhân của $j$.

Cho $x$ là một phần tử của căn của A. Khi đó $x^*x$ thuộc căn của A, và do đó Sp$'_A(x^*x) =\{0\}($I, p. 5, nhận xét 3). Vì Sp$'_{Stell(A)}(j(x^*x))\subset$ Sp$'_A(x^*x)$, nên ta có Sp$'_{Stell(A)}(j(x)^*j(x)) =\{0\}$, do đó $\|j(x)\|^2=\|j(x)^*j(x)\|=\varrho (j(x)^*j(x)) = 0$ (công thức (2) của I, p. 104), và vì vậy $j(x) = 0$.

### 13. Đại số stellar của một nhóm compact địa phương

#### Định nghĩa 9 {#ts-i-s6-def-9 .statement tag=02EZ}

Cho G là một nhóm compact địa phương và cho A là đại số Banach có đối hợp các độ đo bị chặn trên G có một mật độ đối với một độ đo Haar trên G (ví dụ 4 của I, p. 99). **Đại số stellar** của G, theo định nghĩa, là đại số stellar bao của đại số Banach có đối hợp A. Nó được ký hiệu là Stell(G).

#### Nhận xét {#ts-i-s6-n13-rem-1 .statement tag=02F0}

Cho $\nu$ là một độ đo Haar trái trên G và cho Δ là môđun của nó. Ánh xạ $f\mapsto f\cdot \nu$ là một đẳng cấu đẳng cự từ đại số $L^1(G, \nu )$ lên A (loc. cit.). Do đó cũng có thể định nghĩa Stell(G) là đại số stellar bao của đại số chuẩn có đối hợp $L^1(G, \nu )$.

Cho G là một nhóm compact địa phương và cho $\nu$ là một độ đo Haar trái trên G. Với $\mu\in \mathscr{M}^1(G)$ và $f\in L^2(G, \nu )$, ta có $\mu*f\in L^2(G, \nu )$ (INT, VIII, §4, mệnh đề 6). Khi đó, ký hiệu bởi $\boldsymbol{\gamma }(\mu)$ tự đồng cấu $f\mapsto \mu*f$ của $L^2(G, \nu )$. Ánh xạ $\mu\mapsto \boldsymbol{\gamma }(\mu)$ là một biểu diễn của đại số $\mathscr{M}^1(G)$ trong đại số Banach $\mathscr{L}(L^2(G, \nu ))$ các tự đồng cấu liên tục của $L^2(G, \nu )$ (INT, VIII, §4, hệ quả của mệnh đề 6). Mặt khác, $\boldsymbol{\gamma }(\check{\mu})$ là chuyển vị của tự đồng cấu $\boldsymbol{\gamma }(\mu)$ (INT, VIII, §4, n$^o3$, mệnh đề 8). Suy ra $\boldsymbol{\gamma }(\mu^*)$ là tự đồng cấu liên hợp của $\boldsymbol{\gamma }(\mu)$, và do đó ánh xạ $\boldsymbol{\gamma }:\mu\mapsto \boldsymbol{\gamma }(\mu)$ là một cấu xạ của các đại số có đối hợp từ $\mathscr{M}^1(G)$ vào đại số stellar $\mathscr{L}(L^2(G, \nu ))$, được gọi là biểu diễn chính quy trái của $\mathscr{M}^1(G)$ trong $L^2(G, \nu )$. Theo INT, VIII, §4, n$^o7$, mệnh đề 19, biểu diễn này là trung thành.

Cho $j$ là ánh xạ chính tắc từ $L^1(G, \nu )$ vào Stell(G). Hạn chế lên $L^1(G, \nu )$, biểu diễn chính quy $\boldsymbol{\gamma }$ xác định một cấu xạ đơn ánh của các đại số có đối hợp từ $L^1(G, \nu )$ vào $\mathscr{L}(L^2(G, \nu ))$, được gọi là biểu diễn chính quy trái của $L^1(G)$ trong $L^2(G)$. Theo mệnh đề 20, tồn tại một cấu xạ duy nhất $\boldsymbol{\gamma }':$ Stell(G) $\rightarrow \mathscr{L}(L^2(G, \nu ))$ sao cho $\boldsymbol{\gamma }=\boldsymbol{\gamma }'\circ j$. Người ta nói rằng $\boldsymbol{\gamma }'$ là biểu diễn chính quy trái của Stell(G) trong $L^2(G, \nu )$. Lạm dụng ký hiệu, ta lại viết

$$
\boldsymbol{\gamma }'(\varphi )(f) =\varphi *f \tag{7}
$$

với $f\in L^2(G, \nu )$ và $\varphi \in$ Stell(G). Ta có

$$
\|\varphi *f\|_2\leqslant \|\varphi \|_*\|f\|_2 \tag{8}
$$

#### Nhận xét {#ts-i-s6-n13-rem-2 .statement tag=02F1}

Nói chung, biểu diễn chính quy trái $\boldsymbol{\gamma }'$ của Stell(G) trong $L^2(G, \nu )$ không trung thành. Có thể chứng minh rằng nó như vậy khi và chỉ khi tồn tại trên $L^{\infty}_{\mathbf{R}}(G)$ một dạng tuyến tính dương $f$ sao cho $f(1) = 1$ và $f(\boldsymbol{\gamma }(g)x) =f(x)$ với mọi $(g, x)\in G\times G$ (khi đó người ta nói rằng nhóm G là amenable, cf. EVT, IV, p. 73, bài tập 4).

#### Mệnh đề 22 {#ts-i-s6-prop-22 .statement tag=02F2}

Ánh xạ chính tắc $j$ từ $L^1(G, \nu )$ vào Stell(G) là đơn ánh và có ảnh trù mật.

Ảnh của $j$ là trù mật theo định nghĩa của đại số sao bao của một đại số định chuẩn đối hợp. Vì biểu diễn chính quy trái $\boldsymbol{\gamma }$ là trung thành, tính đơn ánh của $j$ suy ra từ đẳng thức $\boldsymbol{\gamma }=\boldsymbol{\gamma }'\circ j$.

#### Hệ quả {#ts-i-s6-n13-cor-1 .statement tag=02F3}

Đại số $L^1(G, \nu )$ là nửa đơn.

Điều này suy ra từ Mệnh đề 21 của I, p. 125 và Mệnh đề 22.

Do đó có thể đồng nhất $L^1(G, \nu )$ với một đại số con đối hợp trù mật của Stell(G), và khi đó đơn ánh chính tắc của $L^1(G, \nu )$ vào Stell(G) là liên tục.

Bây giờ giả sử rằng nhóm G là đơn môđula (INT, VII, §1, No.$^o3$, Định nghĩa 3). Khi đó có thể lặp lại các lập luận như trên, xuất phát từ biểu diễn chính quy phải $(f, \mu)\mapsto \boldsymbol{\delta }(\mu)(f) =f*\check{\mu}$ của $L^2(G, \nu )\times \mathscr{M}^1(G)$ trong $L^2(G, \nu )$. Khi đó ta định nghĩa một cấu xạ $\boldsymbol{\delta }'$ của Stell(G) vào $\mathscr{L}(L^2(G, \nu ))$ sao cho $\boldsymbol{\delta }=\boldsymbol{\delta }'\circ j$, và ta viết $\boldsymbol{\delta }'(\varphi )(f) =f*\varphi$ với $f\in L^2(G, \nu )$ và $\varphi \in$ Stell(G).

Với $\varphi , \psi \in$ Stell(G), ta có $\boldsymbol{\delta }'(\psi )\circ \boldsymbol{\gamma }'(\varphi ) =\boldsymbol{\gamma }'(\psi )\circ \boldsymbol{\delta }'(\varphi )$, tức là

$$
(\varphi *f)*\psi =\varphi *(f*\psi ) \tag{9}
$$

với mọi $f\in L^2(G, \nu )$. Thật vậy, công thức này đúng với $\varphi , \psi \in$ $L^1(G, \nu )$, và các ánh xạ $(\varphi , \psi )\mapsto (\varphi *f)*\psi$ và $(\varphi , \psi )\mapsto \varphi *(f*\psi )$ là những ánh xạ song tuyến tính liên tục từ Stell(G) $\times$ Stell(G) vào $L^2(G, \nu )$.

## BÀI TẬP {#ts-i-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).
