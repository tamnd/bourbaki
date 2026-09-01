---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 3
section_title: Fonctions de type positif
lang: vi
source: ts-iii-v-fr
book_pages: TS V.431-TS V.456, TS V.492-TS V.504
pdf_pages: 0444-0469, 0505-0517
extraction: native
subsections:
    - "no": 1
      title: Noyaux universellement positifs
      page: 432
      pdf_page: 445
    - "no": 2
      title: Complément sur le calcul fonctionnel holomorphe
      page: 435
      pdf_page: 448
    - "no": 3
      title: Formes linéaires positives
      page: 436
      pdf_page: 449
    - "no": 4
      title: Représentations des algèbres stellaires
      page: 441
      pdf_page: 454
    - "no": 5
      title: Fonctions de type positif sur un groupe topologique
      page: 442
      pdf_page: 455
    - "no": 6
      title: Dual unitaire d’un groupe localement compact
      page: 446
      pdf_page: 459
    - "no": 7
      title: Existence de représentations irréductibles
      page: 450
      pdf_page: 463
    - "no": 8
      title: Fonctions de type positif sur un groupe localement compact commutatif
      page: 454
      pdf_page: 467
statements: 39
exercises: 23
content_sha256: 09fd70717b7daf3cbe03d7594ea4145d6c11de6e9c8160e0f7fb787cea475730
translated_from: content/en-mt/ts/V/03_s3_fonctions_de_type_positif.md
source_lang: en-mt
translation_method: machine
source_content_sha256: a6b6b45dafab3a0447148b0aad242724b9c02290041f3925c9ca84a89191bfc2
translation_model: gpt-5.4
translation_run: translate-vi-06675c45
glossary_version: 34
glossary_terms_sha256: 840198867afec10dd28ba65f3fab83912ae64ca6540693a4e08caf7d2fcf0bb5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. HÀM KIỂU DƯƠNG

Trong đoạn này, mọi không gian vectơ, cũng như mọi không gian Hilbert và đại số được xét, đều trên $\mathbf{C}$, trừ khi nói ngược lại.

### 1. Các hạt nhân dương phổ quát

Trong số này, X là một không gian tôpô tách.

#### Định lý 1 {#ts-v-s3-thm-1 .statement tag=03BX}

Cho $f\in \mathscr{C}(X\times X)$. Các điều kiện sau là tương đương:

(i) Với mọi tập con compac Y của X và mọi độ đo dương $\mu$ trên Y, tự đồng cấu của $L^2(Y, \mu)$ được xác định bởi hạt nhân $f|(Y\times Y)$ (Định nghĩa 1 của III, p. 29) là dương; nói cách khác, ta có

$$
\int_{Y\times Y}\overline{h(x)}h(y)f(x, y)d(\mu\otimes \mu)(x, y)\geqslant 0
$$

với mọi $h\in \mathscr{L}^2(Y, \mu)$;

(ii) Với mọi số nguyên $n\in \mathbf{N}$, mọi họ $(x_i)_{0\leqslant i\leqslant n}$ trong X và mọi họ $(t_i)_{0\leqslant i\leqslant n}$ các số phức, ta có

$$
\sum_{i=0}^n\sum_{j=0}^n\overline{t}_it_jf(x_i, x_j)\geqslant 0
$$

(iii) Tồn tại một không gian Hilbert phức E và một ánh xạ liên tục $g: X\rightarrow E$ có ảnh toàn phần sao cho $f(x, y) =\langle g(x)|g(y)\rangle$ với mọi $x$ và $y$ trong X;

(iv) Tồn tại một không gian Hilbert phức E và một ánh xạ liên tục $g: X\rightarrow E$ sao cho $f(x, y) =\langle g(x)|g(y)\rangle$ với mọi $x$ và $y$ trong X.

Hiển nhiên là (iii) kéo theo (iv), và ta thấy rằng (i) kéo theo (ii) bằng cách xét độ đo rời rạc $\mu$ là ảnh của độ đo đếm trên $\{0, . . . , n\}$ dưới ánh xạ $i\mapsto x_i$ và hàm $h$ sao cho

$$
h(x) =\sum_{0\leqslant i\leqslant n}t_i
$$

$x_i=x$

Hãy chứng minh rằng (iv) kéo theo (i). Giả sử tồn tại một không gian Hilbert phức E và một ánh xạ liên tục $g: X\rightarrow E$ sao cho $f(x, y) =\langle g(x)|g(y)\rangle$ với mọi $(x, y)\in X\times X$. Cho Y là một tập con compac của $X,\mu$ là một độ đo dương trên Y và $h\in \mathscr{L}^2(Y, \mu)$. Ta có

$$
\int_{Y\times Y}\overline{h(x)}h(y)f(x, y)d(\mu\otimes \mu)(x, y)
$$

$$
=\int_{Y\times Y}\overline{h(x)}h(y)\langle g(x)|g(y)\rangle d(\mu\otimes \mu)(x, y)
$$

$$
=\langle\int_Yh(x)g(x)d\mu(x)|\int_Yh(y)g(y)d\mu(y)\rangle\geqslant 0
$$

theo INT, V, p. 97, § 8, no$^o4$, Prop. 9.

Cuối cùng, hãy chứng minh rằng (ii) kéo theo (iii). Cho $\widetilde{E}$ là không gian các độ đo phức có giá hữu hạn trên X. Với $\mu_1$ và $\mu_2$ trong $\widetilde{E}$, đặt

$$
\langle \mu_1|\mu_2\rangle =\int_{X\times X}f(x, y) (\overline{\mu}_1\otimes \mu_2)(x, y)
$$

Dạng sesquilinear thu được trên $\widetilde{E}$ là một dạng Hermit dương. Thật vậy, cho $\mu\in \widetilde{E}$; tồn tại một họ hữu hạn $(x_i)_{0\leqslant i\leqslant n}$ trong X và các số phức $(t_i)_{0\leqslant i\leqslant n}$ sao cho $\mu=\sum^n_{i=0}t_i\varepsilon_{x_i}$. Khi đó ta có

$$
\langle \mu|\mu\rangle =\sum_{i=0}^n\sum_{j=0}^n\overline{t}_it_jf(x_i, x_j)\geqslant 0
$$

theo giả thiết. Định nghĩa $\widetilde{g}: X\rightarrow \widetilde{E}$ bởi $\widetilde{g}(x) =\varepsilon_x$. Ảnh của ánh xạ $\widetilde{g}$ sinh ra $\widetilde{E}$. Hơn nữa, với mọi $(x, y)\in X\times X$, một mặt ta có $f(x, y) =\langle \widetilde{g}(x)|\widetilde{g}(y)\rangle$ và mặt khác

$$
\|\widetilde{g}(x)-\widetilde{g}(y)\|^2=f(x, x) +f(y, y)-f(x, y)-f(y, x)
$$

điều này kéo theo $\widetilde{g}$ là liên tục vì $f$ là liên tục.

Cho E là không gian Hilbert tách và hoàn thành của $\widetilde{E}$ (EVT, V, p. 8, hệ quả của mệnh đề 4) và $g: X\rightarrow E$ là hợp thành của $\widetilde{g}$ với ánh xạ chính tắc $\widetilde{E}\rightarrow E$. Khi đó ánh xạ $g$ là liên tục, ảnh của nó là toàn phần trong E, và ta có $f(x, y) =\langle g(x)|g(y)\rangle$ với mọi $(x, y)\in X\times X$.

Phương pháp dùng để chứng minh rằng (ii) kéo theo (iii) được gọi là phép dựng Gelfand–Naimark–Segal.

#### Định nghĩa 1 {#ts-v-s3-def-1 .statement tag=03BY}

Một hàm $f\in \mathscr{C}(X\times X)$ được gọi là một hạt nhân dương phổ dụng trên X nếu nó thỏa mãn các điều kiện tương đương của Định lý 1.

Nếu $f$ là một hạt nhân dương phổ dụng trên X, thì một cặp $(E, g)$ thỏa mãn điều kiện (iv) của loc. cit. được gọi là một hiện thực Hilbert của $f$; nếu điều kiện (iii) được thỏa mãn, thì nó được gọi là một hiện thực Hilbert xyclic.

Ta ký hiệu bởi Noy$_+(X)$ tập hợp các hạt nhân dương phổ dụng trên X.

Cho $X'$ là một không gian tôpô tách và $h: X\rightarrow X'$ là một ánh xạ liên tục. Ánh xạ $f\mapsto f\circ (h, h)$ từ $\mathscr{C}(X'\times X')$ vào $\mathscr{C}(X\times X)$ gây ra, khi chuyển qua các không gian con, một ánh xạ Noy$_+(X')\rightarrow$ Noy$_+(X)$.

#### Mệnh đề 1 {#ts-v-s3-prop-1 .statement tag=03BZ}

Cho $f$ là một hạt nhân dương phổ dụng trên X. Cho $(E_1, g_1)$ và $(E_2, g_2)$ là các hiện thực Hilbert của $f$. Giả sử rằng $(E_1, g_1)$ là một hiện thực Hilbert xyclic. Khi đó tồn tại một và chỉ một ánh xạ tuyến tính liên tục $u: E_1\rightarrow E_2$ sao cho $g_2=u\circ g_1$. Ánh xạ này là đẳng cự. Nếu $(E_2, g_2)$ cũng xyclic, thì $u$ là một đẳng cấu.

Tính duy nhất của $u$ suy ra từ việc ảnh của $g_1$ là toàn phần trong $E_1$. Đặt $F =\mathbf{C}^{(X)}$ và cho $(e_x)_{x\in X}$ là cơ sở chính tắc của F. Với $j= 1$ và $j= 2$, ký hiệu bởi $u_j$ ánh xạ tuyến tính từ F vào $E_j$ được xác định bởi $u_j(e_x) =g_j(x)$, và ký hiệu bởi $F_j$ ảnh của nó; không gian $F_1$ là trù mật trong $E_1$.

Cho $t=\sum t_xe_x$ là một phần tử của F. Ta có

$$
\|u_1(t)\|^2=\sum_{x,y}\overline{t}_xt_y\langle g_1(x)|g_1(y)\rangle =\sum_{x,y}\overline{t}_xt_yf(x, y)
$$

$$
=\sum_{x,y}\overline{t}_xt_y\langle g_2(x)|g_2(y)\rangle =\|u_2(t)\|^2
$$

Do đó, tồn tại một ánh xạ tuyến tính đẳng cự $v$ từ $F_1$ vào $F_2$ sao cho $u_2=v\circ u_1$, và đặc biệt $g_2(x) =v(g_1(x))$ với mọi $x\in X$. Vì ảnh của $g_1$ là toàn phần trong $E_1$, ánh xạ này kéo dài thành một ánh xạ tuyến tính đẳng cự $u$ từ $E_1$ vào $E_2$ sao cho $g_2=u\circ g_1$.

Theo Bổ đề 8 của I, p. 107, ảnh của $u$ là đóng trong $E_2$. Nếu $(E_2, g_2)$ là một thể hiện Hilbert chu trình, thì ảnh của $u$ cũng trù mật trong $E_2$ và do đó $u$ là một đẳng cấu.

#### Mệnh đề 2 {#ts-v-s3-prop-2 .statement tag=03C0}

Tập hợp Noy$_+(X)$ là một nón tự liên hợp trong không gian $\mathscr{C}(X\times X)$; nó ổn định đối với tích và đóng khi $\mathscr{C}(X\times X)$ được trang bị tôpô hội tụ đơn giản.

số thựcHiển nhiên là nếu$t\geqslant 0$, và rằng $\frac{f}{f}\in \in$ NoyNoy$_{++}(X)$.(X), thì $tf\in$ Noy$_+(X)$ với mọi

Nếu $(E_1, g_1)$ và $(E_2, g_2)$ là các thể hiện Hilbert của các hạt nhân dương phổ dụng $f_1$ và $f_2$ trên X, thì cặp $(E_1\oplus E_2, g_1+g_2)$ (resp. cặp $(E_1\widehat{\otimes}_2E_2, g_1\otimes g_2)$) là một thể hiện Hilbert của $f_1+f_2$ (resp. của $f_1f_2$); do đó đây là các hạt nhân dương phổ dụng.

Đặc trưng hóa (ii) của Noy$_+(X)$ (Định lý 1) kéo theo rằng tập hợp này là đóng trong $\mathscr{C}(X\times X)$ được trang bị tôpô hội tụ đơn giản.

### 2. Phần bù về phép tính phiếm hàm chỉnh hình

Với mọi tập con X của $\mathbf{C}$, $X^*$ ký hiệu ảnh của X qua phép liên hợp phức. Cho U là một tập con mở của $\mathbf{C}$ và $g: U\rightarrow \mathbf{C}$ là một hàm chỉnh hình. Khi đó hàm $f^*:z\mapsto g(\overline{z})$ được xác định và chỉnh hình trên $U^*$. Ánh xạ $f\mapsto f^*$ là một song ánh liên tục từ $\mathscr{O}(U)$ lên $\mathscr{O}(U^*)$ sao cho $(f_1f_2)^*=f_1^*f_2^*$ và $(f_1+f_2)^*=f_1^*+f_2^*$ với $f_1$ và $f_2$ trong $\mathscr{O}(U)$.

Cho C là một tập con compắc của $\mathbf{C}$. Các ánh xạ $f\mapsto f^*$ từ $\mathscr{O}(U)$ vào $\mathscr{O}(U^*)$, khi U chạy trong các tập con mở của $\mathbf{C}$ chứa C, cảm sinh một song ánh liên tục của không gian $\mathscr{O}(C)$ lên $\mathscr{O}(C^*)$(I, p. 49, n$^o1$), cũng được ký hiệu bởi $f\mapsto f^*$ và thỏa mãn $(f_1f_2)^*=f_1^*f_2^*$ và $(f_1+f_2)^*=f_1^*+f_2^*$ với $f_1$ và $f_2$ trong $\mathscr{O}(C)$.

#### Mệnh đề 3 {#ts-v-s3-prop-3 .statement tag=03C1}

Cho A là một đại số Banach có đơn vị với phép đối hợp. Cho $a\in A$. Phổ của $a^*$ là ảnh Sp$_A(a)^*$ của Sp$_A(a)$ qua phép liên hợp phức. Với mọi $f\in \mathscr{O}$(Sp$_A(a)$), ta có $f(a)^*=f^*(a^*)$.

Mệnh đề thứ nhất suy ra từ I, p. 97. Theo điều đi trước, ánh xạ $\varphi$ từ $\mathscr{O}$(Sp$_A(a)$) vào A được xác định bởi $f\mapsto (f^*(a^*))^*$ là một cấu xạ có đơn vị liên tục từ $\mathscr{O}$(Sp$_A(a)$) vào A sao cho ảnh của mầm trong một lân cận của Sp$_A(a)$ của hàm đồng nhất của $\mathbf{C}$ bằng $a$. Do đó, $\varphi$ là ánh xạ $f\mapsto f(a)$ của phép tính phiếm hàm chỉnh hình (I, p. 74, đl. 5).

#### Bổ đề 1 {#ts-v-s3-lem-1 .statement tag=03C2}

Gọi D là đĩa mở đơn vị trong $\mathbf{C}$. Tồn tại một hàm chỉnh hình duy nhất $f$ xác định trên D sao cho $f(z)^2= 1-z$ với mọi $z\in D$ và $f(0) = 1$. Ta có $f^*=f$.

Bán kính hội tụ của chuỗi lũy thừa

$$
^{+\infty}(1/2)_n
$$

$$
\sum(-z)
$$

$$
n
$$

$n=0$

bằng 1 và tổng của nó $f$ xác định một hàm chỉnh hình trên D (VAR,

$$
\surd
$$

R1, p. 27, 3.2.9) nhận giá trị 1 tại 0. Nó thỏa mãn $f(x) =1-x$ với mọi $x\in D\cap \mathbf{R}$ (FVR, III, p. 19), do đó $f(z)^2= 1-z$ với $z\in D$ vì hiệu $f(z)^2-(1-z)$ là một hàm chỉnh hình mà mọi đạo hàm liên tiếp của nó đều triệt tiêu tại 0 (VAR, R1, p. 27, 3.2.5). Theo định nghĩa, ta kiểm tra được rằng $f^*=f$.

Gọi $g$ là một hàm chỉnh hình trên D sao cho $g(z)^2= 1-z$ với mọi $z\in D$ và sao cho $g(0) = 1$. Hàm $g$ không triệt tiêu và hàm liên tục $f /g$ trên D nhận các giá trị trong $\{-1,1\}$; vì D liên thông và $f(0) =g$(0), nên ta có $f=g$.

### 3. Các dạng tuyến tính dương

#### Định nghĩa 2 {#ts-v-s3-def-2 .statement tag=03C3}

Cho A là một đại số có phép hợp involution. Một dạng tuyến tính $\lambda$ trên A được gọi là dương nếu $\lambda (a^*a)\in \mathbf{R}_+$ với mọi $a\in A$.

Nếu A là một đại số Banach có phép hợp involution, ta ký hiệu bởi $A'_+$ tập hợp các dạng tuyến tính dương liên tục trên A.

Cho A là một đại số Banach có phép hợp involution. Tập hợp $A'_+$ là một nón lồi nhọn trong không gian vectơ thực của các dạng tuyến tính $\mathbf{C}$-tuyến tính trên A.

#### Bổ đề 2 {#ts-v-s3-lem-2 .statement tag=03C4}

Cho A là một đại số Banach có phép hợp involution và $\lambda$ là một dạng tuyến tính dương trên A.

a) Với mọi $a$ và $b$ trong A, ta có $\lambda (a^*b) =\overline{\lambda(b^*a)}$ và

$$
|\lambda (a^*b)|^2\leqslant \lambda (a^*a)\lambda (b^*b)
$$

b) Nếu A có đơn vị, thì dạng tuyến tính $\lambda$ là liên tục và chuẩn của nó bằng $\lambda (1)$.

Ánh xạ $(a, b)\mapsto \lambda (a^*b)$ là một dạng Hermit dương trên A; vì vậy nó thỏa mãn $\lambda (a^*b) =\lambda (b^*a)$ và $|\lambda (a^*b)|^2\leqslant \lambda (a^*a)\lambda (b^*b)$ với mọi $a$ và $b$ trong A (EVT, V, p. 2, nhận xét and p. 3, mđ. 2).

Hãy chứng minh b). Cho $a\in A$ là một phần tử Hermit có chuẩn $<1$. Bán kính phổ của $a$ nhỏ hơn $\|a\|$, do đó phổ của $a$ được chứa trong đĩa đơn vị mở D của $\mathbf{C}$ (Định lý 1 của I, p. 24). Cho $f$ là một hàm chỉnh hình trên D sao cho $f(z)^2= 1-z$ với mọi $z\in D$ (Bổ đề 1 của V, p. 435). Áp dụng phép tính phiếm hàm chỉnh hình cho phần tử $a$ và cho hàm $f$, phần tử $b=f(a)$ thỏa mãn $b^2= 1-a($I, p. 74, Định lý 5). Theo Mệnh đề 3 của V, p. 435, hơn nữa ta có $f(a)^*=f^*(a^*) =f(a)$, do đó $b$ là Hermit. Khi đó ta có $\lambda (1-a) =\lambda (b^*b)\geqslant 0$, do đó $\lambda (a)\leqslant \lambda (1)$.

Bây giờ cho $b\in A$ có chuẩn $<1$. Phần tử $b^*b$ là Hermit và $\|b^*b\|<1$, do đó áp dụng a) với $a= 1$, ta được

$$
|\lambda (b)|^2\leqslant \lambda (1)\lambda (b^*b)\leqslant \lambda (1)^2
$$

với đẳng thức nếu $b= 1$. Vì vậy dạng tuyến tính $\lambda$ là liên tục, và chuẩn của nó bằng $\lambda (1)$. Mệnh đề b) được chứng minh.

#### Ví dụ {#ts-v-s3-n3-exa-1 .statement tag=03C5}

Cho X là một không gian tôpô compact và cho A là star-đại số $\mathscr{C}(X)$. Các dạng tuyến tính dương trên A được đồng nhất với các độ đo dương trên X (INT, III, p. 52, § 1, n$^o6$, Định lý 1).

#### Bổ đề 3 {#ts-v-s3-lem-3 .statement tag=03C6}

Cho A là một đại số Banach có phép đối hợp, có đơn vị và thừa nhận một đơn vị xấp xỉ (I, p. 120, Định nghĩa 7). Cho $\lambda$ là một dạng tuyến tính dương liên tục trên A.

a) Với mọi $a$ trong A, ta có $\lambda (a^*) =\overline{\lambda(a)}$ và $|\lambda (a)|^2\leqslant \|\lambda \|\lambda (a^*a)$;

b) Gọi $\widetilde{A}$ là đại số có phép đối hợp thu được từ A bằng phép nối thêm một phần tử đơn vị, và gọi $e$ là phần tử đơn vị của nó. Tồn tại một dạng tuyến tính dương liên tục $\widetilde{\lambda}$ trên $\widetilde{A}$ kéo dài $\lambda$ và sao cho $\widetilde{\lambda}(e) =\|\lambda \|$;

c) Với mọi $a$ và $b$ trong A, ta có $|\lambda (b^*ab)|\leqslant \|a\|\lambda (b^*b)$.

Hãy chứng minh a). Gọi $\mathfrak{F}$ là một đơn vị xấp xỉ của A. Cho $a\in A$. Dùng Bổ đề 2, a) và định nghĩa của đơn vị xấp xỉ, ta được

$\lambda (a^*) =$ lim$_{f,\mathfrak{F}}\lambda (f a^*) =$ lim$_{f,\mathfrak{F}}\lambda (af^*) =$ lim$_{f,\mathfrak{F}}\lambda ((f a^*)^*) =\overline{\lambda(a)}$,

do đó (loc. cit.)

$|\lambda (a)|^2=$ lim$_{f,\mathfrak{F}}|\lambda (f a)|^2\leqslant \lambda (a^*a)$ lim sup$_{f,\mathfrak{F}}\lambda (f f^*)\leqslant \|\lambda \|\lambda (a^*a)$,

vì $\mathfrak{F}$ là một bộ lọc trên quả cầu đơn vị của A.

Để chứng minh b), ta có thể giả sử rằng $\lambda$ khác không, rồi giả sử rằng $\|\lambda \|= 1$. Với $a\in A$ và $z\in \mathbf{C}$, đặt $\widetilde{\lambda}(a+z\cdot e) =\lambda (a) +z$. Ánh xạ $\widetilde{\lambda}$ là một dạng tuyến tính liên tục trên $\widetilde{A}$ kéo dài $\lambda$ và thỏa mãn $\widetilde{\lambda}(e) = 1$. Nó là dương: với mọi $a\in A$ và $z\in \mathbf{C}$, theo a), ta tính được

$$
\widetilde{\lambda}((a+z\cdot e)^*(a+z\cdot e)) =\lambda (a^*a) +z\lambda (a) +z\lambda (a^*) +|z|^2
$$

$$
=|z+\lambda (a)|^2+\lambda (a^*a)- |\lambda (a)|^2\geqslant 0
$$

Sau cùng, cho $b$ là một phần tử của A. Ánh xạ $a\mapsto \widetilde{\lambda}(b^*ab)$ là một dạng tuyến tính dương trên đại số Banach có đối hợp có đơn vị $\widetilde{A}$. Vậy nên nó liên tục và có chuẩn bằng giá trị của nó tại $e$ (Bổ đề 2, b)), giá trị này bằng $\lambda (b^*b)$, do đó có mệnh đề c).

#### Mệnh đề 4 {#ts-v-s3-prop-4 .statement tag=03C7}

Cho A là một đại số Banach có đối hợp.

a) Với mọi không gian Hilbert E, mọi cấu xạ của các đại số có đối hợp $\varphi : A\rightarrow \mathscr{L}(E)$ và mọi vectơ $x\in E$, dạng tuyến tính xác định trên A bởi $\lambda (a) =\langle x|\varphi (a)x\rangle$ là một dạng tuyến tính dương liên tục;

b) Cho $\lambda \in A'_+$. Ánh xạ $f$ từ $A\times A$ vào $\mathbf{C}$ xác định bởi $f(a, b) =$ $\lambda (a^*b)$ với mọi $(a, b)\in A\times A$ là một hạt nhân dương phổ dụng trên A.

Ta hãy chứng minh a). Với mọi $a\in A$, ta có

$$
\lambda (a^*a) =\langle x|\varphi (a^*a)x\rangle =\|\varphi (a)x\|^2\geqslant 0
$$

vì thế $\lambda$ là một dạng tuyến tính dương trên A; nó liên tục vì $\varphi$ liên tục (Mệnh đề 2 của I, p. 104).

Ta hãy chứng minh b). Hàm $f$ liên tục. Với mọi $n\in \mathbf{N}$, mọi họ $(a_i)_{0\leqslant i\leqslant n}$ trong A và mọi họ $(t_i)_{0\leqslant i\leqslant n}$ các số phức, ta có

$$
\sum_{i=0}^n\sum_{j=0}^n\overline{t}_it_jf(a_i, a_j) =\lambda ((\sum_{i=0}^nt_ia_i)^*(\sum_{j=0}^nt_ja_j))\geqslant 0
$$

do đó có kết quả (Định nghĩa 1 của V, p. 433).

#### Định nghĩa 3 {#ts-v-s3-def-3 .statement tag=03C8}

Cho A là một đại số Banach có đối hợp. Cho $\lambda \in A'_+$ là một dạng tuyến tính dương liên tục trên A. Một hiện thực Hilbert của $\lambda$ theo định nghĩa là một bộ ba $(E, x, \varphi )$ gồm một không gian Hilbert E, một phần tử $x$ của E và một cấu xạ của các đại số có đối hợp $\varphi$ từ A vào $\mathscr{L}(E)$, sao cho $\lambda (b^*a) =\langle \varphi (b)x|\varphi (a)x\rangle$ với mọi $(a, b)\in A^2$.

Nếu tập hợp các phần tử $\varphi (a)x$ với $a\in A$ là toàn phần trong E, ta nói rằng $(E, x, \varphi )$ là một hiện thực Hilbert cyclic của $\lambda$.

#### Mệnh đề 5 {#ts-v-s3-prop-5 .statement tag=03C9}

Cho A là một đại số Banach có đối hợp thừa nhận một đơn vị xấp xỉ. Mọi dạng tuyến tính dương liên tục trên A đều thừa nhận một hiện thực Hilbert cyclic $(E, x, \varphi )$. Nếu A có đơn vị, thì tồn tại một hiện thực như vậy trong đó cấu xạ $\varphi$ là có đơn vị.

Ta có thể giả sử rằng A là một đại số có đơn vị (Bổ đề 3, b)).

Cho $\lambda$ là một dạng tuyến tính dương liên tục trên A. Cho $(E, g)$ là một hiện thực Hilbert cyclic của hạt nhân dương phổ dụng $f$ trên A xác định bởi $f(a, b) =\lambda (a^*b)$ (Mệnh đề 4 và Định lý 1). Ánh xạ $g$ liên tục, ảnh của nó là toàn phần trong E, và ta có $\lambda (a^*b) =\langle g(a)|g(b)\rangle$ với mọi $(a, b)\in A^2$. Đặt $x=g(1)\in E$.

Ánh xạ $g$ của A vào E là tuyến tính: thật vậy, với $(a, b, c)\in A^3$ và $(s, t)\in \mathbf{C}^2$, ta có

$$
\langle g(c)|g(sa+tb)\rangle =\lambda (c^*(sa+tb))
$$

$$
=s\lambda (c^*a) +t\lambda (c^*b) =\langle g(c)|sg(a) +tg(b)\rangle
$$

do đó có mệnh đề cần chứng minh, vì ảnh của $g$ là toàn phần trong E.

Đặc biệt, ảnh F của $g$ là một không gian con vectơ trù mật của E. Hạt nhân của $g$ là một iđêan trái của A: nếu $g(b) = 0$, thì với mọi $a$ và $c$ trong A, ta có

$$
\langle g(ab)|g(c)\rangle =\lambda ((ab)^*c) =\lambda (b^*(a^*c)) =\langle g(b)|g(a^*c)\rangle = 0
$$

vì thế $g(ab) = 0$ do F là trù mật trong E.

Cho $a\in A$. Vì hạt nhân của $g$ là một iđêan trái của A, tồn tại một ánh xạ tuyến tính $\widetilde{\varphi}(a) : F\rightarrow F$ sao cho $\widetilde{\varphi}(a)(g(b)) =g(ab)$ với mọi $b\in A$. Hơn nữa, với mọi $b\in A$, ta có

$$
\|\widetilde{\varphi}(a)(g(b))\|^2=\|g(ab)\|^2=\lambda (b^*a^*ab)\leqslant \|a^*a\|\lambda (b^*b)\leqslant \|a\|^2\|g(b)\|^2
$$

(bổ đề 3, c)), vì thế $\widetilde{\varphi}(a)$ liên tục và có chuẩn $\leqslant \|a\|$. Do đó, tồn tại một tự đồng cấu duy nhất $\varphi (a)\in \mathscr{L}(E)$ cảm sinh $\widetilde{\varphi}(a)$ khi chuyển qua các không gian con.

Cho $a$ và $b$ thuộc A. Ta có

$$
(\varphi (a)\circ \varphi (b))(g(c)) =g(abc) =\varphi (ab)(g(c))
$$

với mọi $c$ trong A, vì thế $\varphi (ab) =\varphi (a)\circ \varphi (b)$ do F là trù mật trong E.

Ánh xạ $\varphi$ của A vào $\mathscr{L}(E)$ là tuyến tính: thật vậy, với mọi $(a, b)\in A^2$ và mọi $(s, t)\in \mathbf{C}^2$, ta có

$$
\varphi (sa+tb)(g(c)) =g((sa+tb)c) = (s\varphi (a) +t\varphi (b))g(c)
$$

với mọi $c\in A$, do đó $\varphi (sa+tb) =s\varphi (a) +t\varphi (b)$ vì F là trù mật trong E. Vì $\|\varphi (b)\|\leqslant \|b\|$ với mọi $b\in A$, ánh xạ $\varphi$ là liên tục. Ta cũng có $\varphi (1) = 1_E$ vì $\varphi (1)(g(a)) =g(a)$ với mọi $a\in A$ và F là trù mật trong E.

Sau cùng, cho $a,b,c$ thuộc A. Ta có

$$
\langle g(c)|\varphi (a^*)(g(b))\rangle =\langle g(c)|g(a^*b)\rangle =\lambda (c^*a^*b)
$$

$$
=\langle g(ac)|g(b)\rangle =\langle \varphi (a)(g(c))|g(b)\rangle
$$

do đó $\varphi (a^*) =\varphi (a)^*$ vì F là trù mật trong E.

Kết luận lại, ánh xạ $\varphi$ là một cấu xạ liên tục của các đại số có đối hợp từ A vào $\mathscr{L}(E)$ và $g(a) =\varphi (a)x$ với mọi $a\in A$; do đó, bộ ba $(E, x, \varphi )$ là một hiện thực Hilbert xiclíc của $\lambda$.

#### Mệnh đề 6 {#ts-v-s3-prop-6 .statement tag=03CA}

Cho A là một đại số Banach có đối hợp và cho $\lambda$ là một dạng tuyến tính dương liên tục trên A. Cho $(E_1, x_1, \varphi_1)$ và $(E_2, x_2, \varphi_2)$ là các hiện thực Hilbert của $\lambda$. Giả sử rằng $(E_1, x_1, \varphi_1)$ là một hiện thực Hilbert xiclíc.

a) Tồn tại một ánh xạ tuyến tính liên tục duy nhất $u$ từ $E_1$ vào $E_2$ là một cấu xạ của các biểu diễn từ $\varphi_1$ vào $\varphi_2($I, p. 11) và thỏa mãn $u(\varphi_1(a)x_1) =\varphi_2(a)x_2$ với mọi $a\in A$;

b) Ánh xạ tuyến tính $u$ là đẳng cự;

c) Nếu $(E_2, x_2, \varphi_2)$ là cyclic, thì $u$ là một đẳng cấu;

d) Nếu $(E_2, x_2, \varphi_2)$ là cyclic và nếu A có đơn vị, thì $u(x_1) =x_2$.

Với $j\in  \{1,2\}$, định nghĩa $\gamma_j: A\rightarrow E_j$ bởi $\gamma_j(a) =\varphi_j(a)x_j$ với mọi $a\in A$. Theo định nghĩa, các cặp $(E_j, \gamma_j)$ là những hiện thực Hilbert của hạt nhân dương phổ dụng $f$ trên A được định nghĩa bởi $(a, b)\mapsto \lambda (a^*b)$. Hiện thực Hilbert $(E_1, \gamma_1)$ là cyclic; do mệnh đề 1 của V, p. 434, vì thế tồn tại một ánh xạ tuyến tính liên tục duy nhất $u: E_1\rightarrow E_2$ sao cho $\gamma_2=u\circ \gamma_1$, và ánh xạ này là đẳng cự. Hơn nữa, nếu $(E_2, x_2, \varphi_2)$ cũng cyclic, thì $u$ là một đẳng cấu. Để chứng minh a), b) và c), chỉ cần chứng minh rằng $u$ là một cấu xạ của các biểu diễn từ $\varphi_1$ vào $\varphi_2$.

Cho $a\in A$. Với mọi $b\in A$, ta có

$$
(u\circ \varphi_1(a))(\gamma_1(b)) = (u\circ \varphi_1(ab))x_1= (u\circ \gamma_1)(ab)
$$

$$
=\gamma_2(ab) =\varphi_2(a)(\gamma_2(b)) =\varphi_2(a)(u(\gamma_1(b)))
$$

do đó các ánh xạ tuyến tính liên tục $u\circ \varphi_1(a)$ và $\varphi_2(a)\circ u$ trùng nhau trên không gian con của $E_1$ sinh bởi ảnh của $\gamma_1$; không gian con này trù mật trong $E_1$ theo giả thiết, do đó $u\circ \varphi_1(a) =\varphi_2(a)\circ u$.

Sau cùng, ta chứng minh d). Vậy giả sử A có đơn vị và $(E_2, x_2, \varphi_2)$ là cyclic. Tồn tại một hiện thực Hilbert cyclic $(E_3, x_3, \varphi_3)$ của $\lambda$ sao cho $\varphi_3$ là một cấu xạ có đơn vị (mệnh đề 5). Cho $j\in  \{1,2\}$. Áp dụng điều trên cho $(E_j, x_j, \varphi_j)$ và $(E_3, x_3, \varphi_3)$, ta thấy rằng tồn tại một đẳng cấu đẳng cự $\widetilde{u}_j$ từ $E_j$ vào $E_3$ sao cho $\widetilde{u}_j\circ \varphi_j(a) =\varphi_3(a)\circ \widetilde{u}_j$ với mọi $a\in A$. Lấy $a= 1_A$, ta thấy rằng $\varphi_j$ có đơn vị. Khi đó ta có $x_2=\varphi_2(1_A)x_2=u(\varphi_1(1_A)x_1) =u(x_1)$.

#### Nhận xét {#ts-v-s3-n3-rem-1 .statement tag=03CB}

Giữ lại ký hiệu của mệnh đề. Có thể xảy ra trường hợp $u(x_1)$ khác $x_2$ (bài tập 3, b) của V, p. 493). Tuy nhiên, bộ ba $(E_2, u(x_1), \varphi_2)$ cũng là một biểu diễn Hilbert của $\lambda$.

### 4. Biểu diễn của các đại số sao

Cho A là một đại số sao. Ký hiệu $A_+$ là nón lồi đóng của các phần tử dương của A (định nghĩa 6 của I, p. 115). Một dạng tuyến tính $\lambda$ trên A là dương khi và chỉ khi $\lambda (A_+)\subset \mathbf{R}_+($I, p. 118, định lý 2).

#### Mệnh đề 7 {#ts-v-s3-prop-7 .statement tag=03CC}

Cho A là một đại số sao. Mọi dạng tuyến tính dương $\lambda$ trên A đều liên tục.

Trước hết hãy chứng minh rằng $\lambda$ bị chặn trên giao của $A_+$ với quả cầu đơn vị của A. Giả sử không phải vậy. Khi đó tồn tại một dãy $(x_n)_{n\geqslant 1}$ trong $A_+$ sao cho $\|x_n\|\leqslant 1$ và $\lambda (x_n)\geqslant n$ với mọi số nguyên $n\geqslant 1$. Chuỗi có số hạng tổng quát $n^{-2}x_n$ hội tụ đến một phần tử $x$ của A (cf. TG, IV, p. 33, Ví dụ 3). Với mọi số nguyên $N\geqslant 1$, vì

$+\infty$

$\sum\frac{1}{n^2}x_n\in A_+$,

$n=N+1$

(I, p. 116, Mệnh đề 14), suy ra rằng

N N $+\infty$

$\sum\frac{1}{n}\leqslant \sum\frac{1}{n^2}\lambda (x_n) =\lambda (x)-\lambda (\sum\frac{1}{n^2}x_n)\leqslant \lambda (x)$,

$n=1n=1n=N+1$

điều này là vô lý (TG, IV, p. 33, Ví dụ 4).

Vì mọi phần tử của quả cầu đơn vị của A là một tổ hợp tuyến tính, với các hệ số bị chặn bởi 1, của nhiều nhất bốn phần tử dương của A có chuẩn $\leqslant 1$(I, p. 96, Bổ đề 2 và công thức (4) của I, p. 117), ta kết luận rằng $\lambda$ là liên tục.

Có những đại số Banach đối hợp thừa nhận các dạng tuyến tính dương không liên tục (Bài tập 3, (a) của V, p. 493).

#### Mệnh đề 8 {#ts-v-s3-prop-8 .statement tag=03CD}

Cho A là một đại số stellar và $a$ là một phần tử khác không của A. Tồn tại một dạng tuyến tính dương $\lambda \in A'_+$ sao cho $\lambda (a^*a)>0$.

Xét không gian Banach thực $A_h$ của các phần tử Hermit của A. Tập $A_+$ là một nón lồi đóng, nhọn và có đỉnh trong $A_h$ (Mệnh đề 14 của I, p. 116). Phần tử $a^*a$ là dương (Định lý 2 của I, p. 118) và khác không; do đó phần tử Hermit $-a^*a$ không dương. Theo EVT, II, p. 42, Hệ quả 5, tồn tại một dạng tuyến tính thực liên tục $\lambda \in A'_h$ sao cho $\lambda (-a^*a)<0$ và $\lambda (A_+)\subset \mathbf{R}_+$. Dạng tuyến tính $\lambda$ kéo dài thành một dạng tuyến tính Hermit $\mathbf{C}$-tuyến tính trên A (cf. I, p. 98), dạng này là dương và có tính chất cần thiết.

#### Định lý 2 (Gelfand–Naimark) {#ts-v-s3-thm-2 .statement tag=03CE}

Cho A là một đại số stellar. Tồn tại một không gian Hilbert E và một cấu xạ đẳng cự của các đại số đối hợp $\varphi$ từ A vào $\mathscr{L}(E)$. Nếu A có đơn vị, thì tồn tại một cấu xạ có đơn vị như vậy.

Với mọi $b\in A-\{0\}$, ký hiệu $\lambda_b$ là một dạng tuyến tính dương liên tục trên A sao cho $\lambda_b(b^*b)>0$ (Mệnh đề 8). Vì A thừa nhận một đơn vị xấp xỉ (I, p. 121, Mệnh đề 18), tồn tại một hiện thực Hilbert $(E_b, x_b, \varphi_b)$ của $\lambda_b$ (Mệnh đề 5). Nếu A có đơn vị, có thể giả sử rằng $\varphi_b$ có đơn vị (loc. cit.). Ta có $\|\varphi_b(b)\|^2=\lambda_b(b^*b)\not = 0$.

Cho E là tổng Hilbert ngoài của các không gian $E_b$ với $b$ thuộc A $-\{0\}$. Với mọi $a\in A$, ký hiệu $\varphi (a)\in \mathscr{L}(E)$ là ánh xạ tuyến tính liên tục duy nhất mà hạn chế của nó lên $E_b$ trùng với $\varphi_b(a)$ với mọi $b\in A-\{0\}$. Ánh xạ $a\mapsto \varphi (a)$ là một cấu xạ của các đại số đối hợp; nó đơn ánh, do đó đẳng cự (Mệnh đề 9 của I, p. 112), và thỏa mãn $\varphi (1) = 1_E$ nếu A có đơn vị. Điều này hoàn thành chứng minh.

*Phạm trù mà các đối tượng là các đại số stellar và các cấu xạ là các cấu xạ của các đại số đối hợp do đó tương đương với phạm trù mà các đối tượng là các đại số con đối hợp đóng của các đại số các nội cấu xạ của các không gian Hilbert, và các cấu xạ là các cấu xạ của các đại số đối hợp.*

### 5. Các hàm kiểu dương trên một nhóm tôpô

Trong số này, G là một nhóm tôpô mà phần tử đơn vị được ký hiệu bởi $e$. Các không gian Hilbert được xét là phức.

#### Định nghĩa 4 {#ts-v-s3-def-4 .statement tag=03CF}

Một hàm liên tục $\varphi \in \mathscr{C}(G)$ được gọi là kiểu dương trên G nếu hàm $f$ được xác định bởi $f(g, h) =\varphi (g^{-1}h)$ trên $G\times G$ là một hạt nhân dương phổ dụng trên G.

Pos(G) ký hiệu tập các hàm kiểu dương trên G, và Pos$_1(G) ($resp. Pos$_{\leqslant 1}(G))$ ký hiệu tập con của các $\varphi \in$ Pos(G) sao cho $\varphi (e) = 1 ($resp. sao cho $\varphi (e)\leqslant 1)$.

#### Ví dụ {#ts-v-s3-n5-exa-1 .statement tag=03CG}

Cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert E và cho $x\in E$. Cho $\varphi$ là hệ số ma trận đường chéo được định nghĩa bởi $\varphi (g) =\langle x|\varrho (g)x\rangle$ với mọi $g\in G$; hàm $\varphi$ là liên tục. Ta có

$$
\varphi (g^{-1}h) =\langle x|\varrho (g)^*\varrho (h)x\rangle =\langle \varrho (g)x|\varrho (h)x\rangle
$$

với mọi $(g, h)\in G\times G$. Do đó $\varphi \in$ Pos(G) (Định lý 1 của V, p. 432, (iv)). Ta có $\varphi \in$ Pos$_1(G)$ nếu và chỉ nếu $\|x\|= 1$.

#### Định nghĩa 5 {#ts-v-s3-def-5 .statement tag=03CH}

Cho $\varphi$ là một hàm kiểu dương trên G. Một hiện thực Hilbert của $\varphi$ là một cặp $(\varrho , x)$ trong đó $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert E và $x\in E$, sao cho $\varphi (g) =\langle x|\varrho (g)x\rangle$ với mọi $g\in G$.

Nếu $x$ là một vectơ cyclic của $\varrho$, ta nói rằng đó là một hiện thực Hilbert cyclic của $\varphi$.

#### Mệnh đề 9 {#ts-v-s3-prop-9 .statement tag=03CI}

Cho $\varphi \in \mathscr{C}(G)$. Các điều kiện sau là tương đương:

(i) Hàm $\varphi$ có kiểu dương trên G;

(ii) Tồn tại một hiện thực Hilbert cyclic của $\varphi$;

(iii) Tồn tại một hiện thực Hilbert của $\varphi$.

Điều kiện (ii) suy ra điều kiện (iii), và điều kiện (iii) suy ra (i) theo ví dụ trên.

Sau cùng, ta chứng minh rằng (i) suy ra (ii). Cho $(E, \gamma )$ là một hiện thực Hilbert cyclic của hạt nhân dương phổ dụng được định nghĩa bởi $f(g, h) =\varphi (g^{-1}h)$ với $(g, h)\in G\times G$. Cho $k\in G$. Hàm liên tục $\gamma_k:g\mapsto \gamma (kg)$ trên G thỏa mãn

$$
\langle \gamma_k(g)|\gamma_k(h)\rangle =\langle \gamma (kg)|\gamma (kh)\rangle =f(kg, kh) =\varphi ((kh)^{-1}kg) =f(g, h)
$$

với mọi $(g, h)\in G\times G$, vì thế $(E, \gamma_k)$ là một hiện thực Hilbert của $f$. Theo Mệnh đề 1 của V, p. 434, tồn tại một phần tử unita duy nhất $\varrho (k)$ trong $\mathscr{L}(E)$ sao cho $\gamma_k=\varrho (k)\circ \gamma$. Với mọi $g\in G$, và mọi $(k_1, k_2)\in G\times G$, ta có

$$
\varrho (k_1k_2)(\gamma (g)) =\gamma (k_1k_2g) =\varrho (k_1)(\varrho (k_2)(\gamma (g)))
$$

do đó $\varrho (k_1k_2) =\varrho (k_1)\varrho (k_2)$ vì ảnh của $\gamma$ là một tập con toàn phần của E.

Cho $k\in G$. Với mọi $g\in G$, ta có $\varrho (g)(\gamma (k)) =\gamma (gk)$, và do đó ánh xạ từ G vào E được định nghĩa bởi $g\mapsto \varrho (g)(\gamma (k))$ là liên tục. Vì tự đồng cấu $\varrho (g)$ là unita, suy ra $\varrho$ là một biểu diễn unita của G trong E (Bổ đề 4 của V, p. 380). Khi đó đặt $x=\gamma (e)$. Tập các vectơ $\varrho (g)x=\varrho (g)(\gamma (e)) =\gamma (g)$ khi $g$ chạy trên G là toàn phần trong E, do đó $x$ là một vectơ cyclic của $\varrho$. Vì

$$
\langle x|\varrho (g)x\rangle =f(e, g) =\varphi (g)
$$

với mọi $g\in G$, cặp $(\varrho , x)$ là một hiện thực Hilbert cyclic của $\varphi$.

#### Mệnh đề 10 {#ts-v-s3-prop-10 .statement tag=03CJ}

Cho $\varphi$ là một hàm kiểu dương trên G và cho $(\varrho_1, x_1)$ và $(\varrho_2, x_2)$ là các thực hiện Hilbert của $\varphi$, trong đó biểu diễn Hilbert $(\varrho_1, x_1)$ là cyclic. Tồn tại một G-cấu xạ đẳng cự duy nhất $u$ từ $\varrho_1$ vào $\varrho_2$ sao cho $u(x_1) =x_2$. Nếu $(\varrho_2, x_2)$ cũng cyclic, thì $u$ là một đẳng cấu.

Với $1\leqslant j\leqslant 2$, ký hiệu $E_j$ là không gian của $\varrho_j$ và $\gamma_j$ là hàm trên G xác định bởi $\gamma_j(g) =\varrho_j(g)x_j$ với mọi $g\in G$. Các cặp $(E_1, \gamma_1)$ và $(E_2, \gamma_2)$ là các thực hiện Hilbert của hàm kiểu dương $(g, h)\mapsto \varphi (g^{-1}h)$, và $(E_1, \gamma_1)$ là một thực hiện Hilbert cyclic. Theo Mệnh đề 1 của V, p. 434, tồn tại một ánh xạ tuyến tính đẳng cự duy nhất $u: E_1\rightarrow E_2$ sao cho $\gamma_2=u\circ \gamma_1$. Đặc biệt, ta có $x_2=\gamma_2(e) =u(\gamma_1(e)) =u(x_1)$. Hơn nữa, với mọi $g$ và $h$ trong G, ta có

$$
\varrho_2(g)u(\gamma_1(h)) =\varrho_2(g)\gamma_2(h) =\gamma_2(gh) =u(\gamma_1(gh)) =u(\varrho_1(g)\gamma_1(h))
$$

và vì tập hợp các phần tử $\gamma_1(h)$ với $h\in G$ là toàn phần trong $E_1$, điều đó có nghĩa là $u$ là một G-cấu xạ. Theo chỗ đã dẫn, nó là một đẳng cấu đẳng cự nếu $(\varrho_2, x_2)$ cũng cyclic.

#### Mệnh đề 11 {#ts-v-s3-prop-11 .statement tag=03CK}

Cho $\varphi \in$ Pos$_1(G)$ và cho $(\varrho , x)$ là một thực hiện Hilbert cyclic của $\varphi$. Khi đó $\varrho$ là một biểu diễn bất khả quy của G khi và chỉ khi $\varphi$ là một điểm cực biên (EVT, II, p. 57, def. 1) của Pos$_1(G)$.

Cho E là không gian của $\varrho$. Trước hết giả sử rằng $\varrho$ không bất khả quy. Cho F là một không gian con đóng khác không của E, ổn định dưới $\varrho$, và khác E. Viết $x=x_1+x_2$, trong đó $x_1\in F$ và $x_2\in F^{\circ}$. Khi đó ta có $1 =\|x\|^2=\|x_1\|^2+\|x_2\|^2$. Biểu diễn con của E sinh bởi $x_1$ được chứa trong F, do đó $x_1\not =x$ vì $x$ là một vectơ cyclic của $\varrho$, do đó $x_2\not = 0$. Tương tự, ta kiểm tra được rằng $x_1\not = 0$.

Với $j= 1$ và $j= 2$, ký hiệu $\varphi_j$ là hàm liên tục trên G sao cho

$$
\varphi_j(g) =\frac{1}{\|x_j\|^2}\langle x_j|\varrho (g)x_j\rangle
$$

với mọi $g\in G$. Ta có $\varphi_j\in$ Pos$_1(G)$(V, p. 443, ví dụ). Vì $\varphi =\|x_1\|^2\varphi_1+\|x_2\|^2\varphi_2$, chỉ cần kiểm tra rằng $\varphi_1\not =\varphi_2$ để chứng minh rằng $\varphi$ không là một điểm cực biên của Pos$_1(G)$; để làm điều này, chỉ cần chứng minh rằng $\varphi \not =\varphi_1$.

Lập luận phản chứng, giả sử rằng $\varphi =\varphi_1$. Vì ta có $\langle x_1|\varrho (g)x_2\rangle = 0$ với mọi $g\in G$, suy ra rằng

$$
\frac{1}{\|x_1\|^2}\langle x_1|\varrho (g)x\rangle =\frac{1}{\|x_1\|^2}\langle x_1|\varrho (g)x_1\rangle =\varphi_1(g) =\varphi (g) =\langle x|\varrho (g)x\rangle
$$

với mọi $g\in G$, do đó $\langle x_1|y\rangle =\langle \|x_1\|^2x|y\rangle$ với mọi phần tử $y$ của không gian con vectơ của E sinh bởi các phần tử $\varrho (g)x$ với $g\in G$, nên với mọi $y\in E$ vì $x$ là một vectơ cyclic của $\varrho$. Điều này sẽ suy ra rằng $x_1=\|x_1\|^2x$ cũng là một vectơ cyclic của $\varrho$, mâu thuẫn, do đó mệnh đề được chứng minh.

Bây giờ giả sử rằng $\varrho$ là bất khả quy, và chứng minh rằng $\varphi$ là một điểm cực biên của Pos$_1(G)$. Cho $\varphi_1\not =\varphi_2$ là các phần tử của Pos$_1(G)$ và cho $t_1,t_2\in [0,1]$ sao cho $t_1+t_2= 1$ và $\varphi =t_1\varphi_1+t_2\varphi_2$. Với $j\in  \{1,2\}$, ký hiệu bởi $(\varrho_j, x_j)$ một hiện thực Hilbert cyclic của $\varphi_j$, và ký hiệu bởi $E_j$ không gian của $\varrho_j$. Đặt $x_3=t^{1/2}_1x_1+t^{1/2}_2x_2$. Khi đó $(\varrho_1\oplus \varrho_2, x_3)$ là một hiện thực Hilbert của $\varphi$. Vì $(\varrho , x)$ là cyclic, tồn tại một G-cấu xạ đẳng cự $u: E\rightarrow E_1\oplus E_2$ sao cho $u(x) =x_3$ (Mệnh đề 10).

Cho $j= 1$ hoặc $j= 2$. Vì $\varrho$ là bất khả quy, tồn tại $\lambda_j\geqslant 0$ sao cho G-cấu xạ $u_j=$ pr$_j\circ u$ từ E vào $E_j$ thỏa mãn

$$
\langle u_j(y)|u_j(y')\rangle =\lambda_j\langle y|y'\rangle
$$

với mọi $y$ và $y'$ trong E (Hệ quả 5 của V, p. 388, nếu $u_j\not = 0$, và có thể lấy $\lambda_j= 0$ trong trường hợp ngược lại). Với mọi $g\in G$, ta có

$$
t_j\varphi_j(g) =\langle t^{1/2}_jx_j|\varrho_j(g)(t^{1/2}_jx_j)\rangle =\langle u_j(x)|\varrho_j(g)(u_j(x))\rangle
$$

$$
=\langle u_j(x)|u_j(\varrho (g)x)\rangle =\lambda_j\varphi (g)
$$

Vì $\varphi_j(e) =\varphi (e) = 1$, suy ra $\varphi_j=\varphi$ nếu $t_j\not = 0$. Do đó giả thiết $\varphi_1\not =\varphi_2$ kéo theo $t_1$ hoặc $t_2$ phải bằng không, điều này chứng tỏ rằng $\varphi$ là một điểm cực biên của Pos$_1(G)$.

#### Bổ đề 4 {#ts-v-s3-lem-4 .statement tag=03CL}

Cho $\varphi \in$ Pos(G). Hàm $\varphi$ bị chặn trên G và ta có $\|\varphi \|_{\infty}=\varphi (e)$. Hơn nữa, ta có

$$
|\varphi (g^{-1}h)-\varphi (h)|\leqslant \surd\overline{2\varphi(e)(\varphi(e) -\mathscr{R}(\varphi(g)))} \tag{1}
$$

với mọi $(g, h)\in G\times G$.

Cho $(\varrho , x)$ là một hiện thực Hilbert của $\varphi$. Ta có $\varphi (e) =\|x\|^2$. Do đó, với mọi $g\in G$, ta có $|\varphi (g)|=|\langle x|\varrho (g)x\rangle |\leqslant \varphi (e)$ theo bất đẳng thức Cauchy-Schwarz. Điều này chứng tỏ mệnh đề thứ nhất.

Với mọi $(g, h)\in G\times G$, ta có

$$
\varphi (g^{-1}h)-\varphi (h) =\langle x|\varrho (g^{-1}h)x\rangle  - \langle x|\varrho (h)x\rangle =\langle \varrho (g)x-x|\varrho (h)x\rangle
$$

vì $\varrho$ là unita, do đó

$$
|\varphi (g^{-1}h)-\varphi (h)|\leqslant \|\varrho (g)x-x\|\|\varrho (h)x\|\leqslant \varphi (e)^{1/2}\|\varrho (g)x-x\|
$$

Ta kết luận bằng cách nhận thấy rằng

$$
\|\varrho (g)x-x\|^2= 2\|x\|^2-2\mathscr{R}(\langle x|\varrho (g)x\rangle ) = 2(\varphi (e)-\mathscr{R}(\varphi (g)))
$$

#### Nhận xét {#ts-v-s3-n5-rem-1 .statement tag=03CM}

Các tập hợp Pos(G) (tương ứng Pos$_1(G)$ và Pos$_{\leqslant 1}(G)$) là các tập con lồi tự liên hợp của đại số có đối hợp $\mathscr{C}_b(G)$. Chúng đóng trong không gian $\mathscr{C}_b(G)$ được trang bị tôpô hội tụ đơn giản. Tập hợp Pos(G) là một nón lồi có đỉnh 0 trong không gian Banach thực $\mathscr{C}_b(G)$.

### 6. Đối ngẫu Unita của một Nhóm Compact Địa Phương

Cho G là một nhóm tôpô compact địa phương. Trang bị cho G một độ đo Haar trái $\mu$. Với $p\in [1,+\infty ]$, ký hiệu bởi $\mathscr{L}^p(G)$ (tương ứng $L^p(G)$) không gian $\mathscr{L}_{\mathbf{C}}^p(G, \mu)$ (tương ứng không gian $L^p_{\mathbf{C}}(G, \mu)$). Ta đồng nhất không gian $\mathscr{C}_b(G)$ với ảnh của nó trong $L^{\infty}(G)$.

Cho Δ ký hiệu môđun của G. Nhắc lại rằng $L^1(G)$ là một đại số Banach có đối hợp mà phép đối hợp của nó được cảm sinh, bằng cách chuyển qua thương, bởi ánh xạ $f\mapsto f^*$ trong đó $f^*(y) = \Delta^{-1}(y)f(y^{-1})$ với mọi $f\in \mathscr{L}^1(G)$ và $y\in G ($x. I, p. 99, ví dụ 4). Đại số Banach $L^1(G)$ thừa nhận một đơn vị xấp xỉ theo INT, VIII, p. 172, §4, n$^o7$, prop. 20.

Cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert phức E. Ánh xạ $f\mapsto \varrho (f)$ là một cấu xạ liên tục của các đại số có đối hợp từ $L^1(G)$ vào $\mathscr{L}(E)$ (bổ đề 1 của V, p. 401); đó là một biểu diễn không suy biến của $L^1(G)$ trong E (INT, VIII, p. 139, § 2, n$^o7$, prop. 10, (i)).

#### Mệnh đề 12 {#ts-v-s3-prop-12 .statement tag=03CN}

Cho E là một không gian Hilbert phức và $\widetilde{\pi}$ là một cấu xạ đại số có đối hợp từ $L^1(G)$ vào $\mathscr{L}(E)$. Nếu biểu diễn $\widetilde{\pi}$ là không suy biến, thì tồn tại một biểu diễn unita duy nhất $\pi$ của G trong E sao cho $\widetilde{\pi}(f) =\pi (f)$ với mọi $f\in L^1(G)$.

Tính duy nhất suy ra từ INT, VIII, p. 139, § 2, n$^o7$, hệ quả 3 của bổ đề 4.

Hãy chứng minh sự tồn tại của $\pi$. Ta có $\|\widetilde{\pi}\|\leqslant 1$ theo Mệnh đề 2 của I, p. 104. Gọi F là không gian con của E được sinh bởi các vectơ có dạng $\widetilde{\pi}(f)x$ với $f$ trong $L^1(G)$ và $x$ trong E; nó trù mật trong E vì biểu diễn $\widetilde{\pi}$ là không suy biến.

Với mọi lân cận compact V của $e$, gọi $\varphi_V$ là một hàm liên tục dương có giá đỡ được chứa trong V sao cho $\int\varphi_V\mu= 1$. Gọi $\mathfrak{B}$ là một cơ sở của bộ lọc các lân cận compact của $e$.

Gọi $g$ là một phần tử của G và $f$ là một phần tử của $L^1(G)$. Ta có $(\varphi_V*\varepsilon_g)*f\rightarrow \varepsilon_g*f$ trong $L^1(G)$ theo bộ lọc các thiết diện của $\mathfrak{B}$ (INT, VIII, p. 172, § 4, n$^o7$, Mệnh đề 20), do đó $\widetilde{\pi}(\varphi_V*\varepsilon_g)\widetilde{\pi}(f)$ hội tụ tới $\widetilde{\pi}(\varepsilon_g*f)$ trong $\mathscr{L}(E)$. Điều này kéo theo $\widetilde{\pi}(\varphi_V*\varepsilon_g)$ hội tụ đơn giản theo bộ lọc các thiết diện của $\mathfrak{B}$ tới một ánh xạ tuyến tính $\pi (g)$ từ F vào F; ánh xạ này liên tục theo EVT, III, p. 26, Hệ quả 3, vì $\|\widetilde{\pi}(\varphi_V*\varepsilon_g)\|\leqslant 1$ với mọi lân cận compact V của $e$. Vậy tồn tại một tự đồng cấu duy nhất của E cảm sinh ra $\pi (g)$ khi chuyển qua các không gian con. Ta lại ký hiệu tự đồng cấu này là $\pi (g)$; ta có $\|\pi (g)\|\leqslant 1$.

Gọi $f\in L^1(G)$. Vì $\widetilde{\pi}(\varphi_V*\varepsilon_g)\widetilde{\pi}(f)$ hội tụ tới $\widetilde{\pi}(\varepsilon_g*f)$, ta có $\pi (g)\widetilde{\pi}(f) =\widetilde{\pi}(\varepsilon_g*f)$.

Với $g=e$, quan hệ này cho thấy $\pi (e)$ là đồng nhất trên F, do đó $\pi (e) = 1_E$. Gọi $g_1$ và $g_2$ là các phần tử của G. Ta có

$$
\pi (g_1)\pi (g_2)\widetilde{\pi}(f) =\pi (g_1)\widetilde{\pi}(\varepsilon_{g_2}*f) =\widetilde{\pi}(\varepsilon_{g_1g_2}*f) =\pi (g_1g_2)\widetilde{\pi}(f)
$$

do đó $\pi (g_1)\pi (g_2) =\pi (g_1g_2)$ trên F, và vì thế trên E. Điều đó chứng minh rằng ánh xạ $g\mapsto \pi (g)$ là một biểu diễn của G trong E. Vì $\|\pi (g)\|\leqslant$ 1 và $\|\pi (g)^{-1}\|$ = $\|\pi (g^{-1})\|\leqslant$ 1, các tự đồng cấu $\pi (g)$ của E là đẳng cự, nên unita (EVT, V, p. 40, Mệnh đề 3).

Gọi $f\in L^1(G)$ và $x\in E$. Ánh xạ $g\mapsto \varepsilon_g*f$ từ G vào $L^1(G)$ là liên tục (INT, VIII, p. 136, § 2, n$^o5$ và p. 144, § 3, n$^o2$, công thức (5)), và $\widetilde{\pi}$ là liên tục, do đó ánh xạ $g\mapsto \widetilde{\pi}(\varepsilon_g*f)x=\pi (g)\widetilde{\pi}(f)x$ là liên tục tại $g=e$. Vì F trù mật trong E, biểu diễn $\pi$ là unita (Bổ đề 4 của V, p. 380).

Gọi $f_1$ và $f_2$ là các phần tử của $L^1(G)$. Theo INT, VIII, p. 127, §1, n$^o5$, Mệnh đề 7, ta có quan hệ

$$
f_1*f_2=\int_Gf_1(g)(\varepsilon_g*f_2)d\mu(g)
$$

trong $L^1$(G), do đó

$$
\widetilde{\pi}(f_1)\widetilde{\pi}(f_2) =\widetilde{\pi}(f_1*f_2) =\int_Gf_1(g)\widetilde{\pi}(\varepsilon_g*f_2)d\mu(g)
$$

$$
=\int_Gf_1(g)\pi (g)\widetilde{\pi}(f_2)d\mu(g) =(\int_Gf_1(g)\pi (g)d\mu(g))\widetilde{\pi}(f_2)
$$

theo INT, VI, p. 9, § 1, n$^o1$, mệnh đề 1. Suy ra

$$
\widetilde{\pi}(f) =\int_Gf(g)\pi (g)d\mu(g) =\pi (f)
$$

với mọi $f\in L^1(G)$. Mệnh đề được chứng minh.

#### Mệnh đề 13 {#ts-v-s3-prop-13 .statement tag=03CO}

Cho $\varphi \in L^{\infty}(G)$. Ký hiệu bởi $\lambda_{\varphi}$ dạng tuyến tính liên tục $f\mapsto  \langle f, \varphi \rangle$ trên $L^1(G)$. Khi đó $\varphi$ là lớp của một hàm kiểu dương trên G khi và chỉ khi $\lambda_{\varphi}$ là một dạng tuyến tính liên tục dương trên $L^1(G)$.

Giả sử rằng $\lambda_{\varphi}$ là một dạng tuyến tính liên tục dương trên $L^1(G)$. Cho $(E, x,\widetilde{\pi})$ là một hiện thực Hilbert cyclic của $\lambda$ (mệnh đề 5 của V, p. 438).

Cho $\pi$ là một biểu diễn unita của G trong E sao cho $\pi (f) =\widetilde{\pi}(f)$ với mọi $f\in L^1(G)$ (mệnh đề 12). Khi đó $\lambda_{\varphi}(f) =\langle x|\pi (f)x\rangle$ với mọi $f\in L^1(G)$.

Vì

$$
\pi (f) =\int_Gf(g)\pi (g)d\mu(g)
$$

với mọi $f\in L^1$(G), ta được

$$
\int_Gf(g)\varphi (g)d\mu(g) =\lambda_{\varphi}(f) =\langle x|\pi (f)x\rangle =\int_Gf(g)\langle x|\pi (g)x\rangle d\mu(g)
$$

với mọi $f\in L^1(G)$ (INT, VI, p. 9, § 1, n$^o1$, mệnh đề 1). Vậy $\varphi$ là lớp trong $L^{\infty}(G)$ của hàm trên G được xác định bởi $g\mapsto  \langle x|\pi (g)x\rangle$, là một hàm kiểu dương trên G (mệnh đề 9 của V, p. 443).

Ngược lại, cho $\varphi \in$ Pos(G). Cho $f\in \mathscr{K}(G)$. Khi đó ta có

$$
\lambda_{\varphi}(f^**f) =\int_G\varphi (y)\int_G\Delta (z)^{-1}f(z^{-1})f(z^{-1}y)d\mu(z)d\mu(y)
$$

$$
=\int_G\varphi (y)\int_Gf(z)f(zy)d\mu(z)d\mu(y)
$$

(INT, VII, p. 19, § 1, n$^o3$, công thức (22)). Hàm liên tục trên $G\times G$ được xác định bởi $(z, y)\mapsto \varphi (y)f(z)f(zy)$ là bị chặn và

$$
\int_G^*|\varphi(y)|\left(\int_G^*|\overline{f(z)}f(zy)|d\mu(z)\right)d\mu(y)
$$

$$
\leqslant\varphi(e)\int_G^*\int_G^*|f(z)||f(zy)|d\mu(z)d\mu(y)
$$

$$
=\varphi(e)\left(\int_G^*|f(z)|d\mu(z)\right)^2
$$

theo INT, V, p. 94, § 8, n$^o3$, mệnh đề 8. Do đó ta suy ra từ định lý Lebesgue-Fubini (INT, V, p. 96, § 8, n$^o4$, định lý 1) rằng

$$
\lambda_{\varphi}(f^**f) =\int_Gf(z)\int_G\varphi (y)f(zy)d\mu(y)d\mu(z)
$$

$$
=\int_{G\times G}f(z)f(y)\varphi (z^{-1}y)d(\mu\otimes \mu)(z, y)
$$

Điều này kéo theo $\lambda_{\varphi}(f^**f)\geqslant 0$ theo Định lý 1, (i) của V, p. 432 áp dụng cho độ đo cảm sinh bởi $\mu$ trên giá của $f$ (INT, IV, p. 186, § 5, n$^o7$, định nghĩa 4). Bởi tính liên tục suy ra $\lambda_{\varphi}(f^**f)\geqslant 0$ với mọi $f\in L^1(G)$.

Các không gian $L^{\infty}(G)$ và $\mathscr{C}_b(G)$ được trang bị các tôpô của chúng như các không gian Banach, mà chuẩn được ký hiệu bởi $f\mapsto  \|f\|_{\infty}$. Ở đây ta sẽ gọi tôpô yếu trên $L^{\infty}$(G), $\mathscr{C}_b(G)$ hoặc Pos(G) là tôpô cảm sinh bởi tôpô yếu $\sigma (L^{\infty}(G),L^1(G))$.

Vì $L^{\infty}(G)$ được đồng nhất với đối ngẫu của $L^1(G)$ (INT, V, p. 61, §5, n$^o8$, th. 4), mọi quả cầu đóng của $L^{\infty}(G)$ đều compact đối với tôpô yếu (EVT, III, p. 17, cor. 3).

#### Hệ quả {#ts-v-s3-n6-cor-1 .statement tag=03CP}

Trong $L^{\infty}(G)$ được trang bị tôpô yếu, tập Pos(G) là đóng và tập Pos$_{\leqslant 1}(G)$ là compact.

Mệnh đề thứ nhất suy ra từ mệnh đề trên, và mệnh đề thứ hai khi đó suy ra từ EVT, III, loc. cit.

Nói chung, Pos$_1(G)$ không compact đối với tôpô yếu, như được chỉ ra bởi ví dụ của nhóm $\mathbf{R}$ (bài tập 10 của V, p. 497).

#### Mệnh đề 14 {#ts-v-s3-prop-14 .statement tag=03CQ}

Tập các điểm cực biên của Pos$_{\leqslant 1}(G)$ bằng hợp của tập các điểm cực biên của Pos$_1(G)$ và của hàm không. Hơn nữa, bao lồi đóng của tập các điểm cực biên của Pos$_1(G)$ chứa Pos$_1(G)$.

Theo hệ quả của mệnh đề 13, tập Pos$_{\leqslant 1}(G)$ là một thiết diện của nón lồi nhọn Pos(G), được xác định bởi chuẩn Minkowski $\varphi \mapsto \varphi (e)$ (EVT, II, p. 61, def. 3 and prop. 4). Vì vậy, các điểm cực biên của nó là hàm không và các phần tử $\varphi$ của Pos$_1(G)$ thuộc các tia sinh cực biên của Pos(G) (EVT, II, p. 62, cor. 1). Đó chính là các điểm cực biên của Pos$_1(G)$ (EVT, II, p. 61, prop. 3). Mệnh đề thứ nhất được suy ra.

Hãy chứng minh mệnh đề thứ hai. Cho $\varphi \in$ Pos$_1(G)$. Vì tập Pos$_{\leqslant 1}(G)$ là compact đối với tôpô yếu (hệ quả của mệnh đề 13), tồn tại một bộ lọc $\mathfrak{F}$ trên bao lồi của tập các điểm cực biên của Pos$_{\leqslant 1}(G)$ hội tụ đến $\varphi$ (EVT, II, p. 59, th. 1). Vì các quả cầu đóng của không gian Banach $L^{\infty}(G)$ là đóng đối với tôpô yếu và vì $\|\varphi \|_{\infty}= 1$, ta có lim$_{\psi ,\mathfrak{F}}\|\psi \|_{\infty}= 1$ (thật vậy, nếu không thì sẽ tồn tại một số thực $c <1$ và một bộ lọc $\mathfrak{G}$ trên quả cầu đóng bán kính $c$ trong $L^{\infty}(G)$ mịn hơn $\mathfrak{F}$, điều này sẽ kéo theo rằng $\varphi$ thuộc quả cầu đóng này).

Từ mô tả các điểm cực biên của Pos$_{\leqslant 1}$(G), mọi phần tử $\psi$ của bao lồi của tập các điểm cực biên của Pos$_{\leqslant 1}(G)$ là một hàm kiểu dương trên G có dạng

$$
\psi =\sum_{i\in I}t_i\psi_i
$$

trong đó I là một tập hợp hữu hạn, $\psi_i$ là một điểm cực biên của Pos$_1(G)$ với mọi $i\in I$, và $t_i\in [0,1]$. Ta có $\sum_it_i=\psi (e) =\|\psi \|_{\infty}\leqslant 1$ (bổ đề 4 của V, p. 446). Nếu $\psi \not = 0$, thì hàm

$$
\frac{\psi}{\|\psi\|_{\infty}}=\sum_{i\in I}\frac{t_i}{\psi(e)}\psi_i
$$

do đó thuộc bao lồi của tập các điểm cực biên của Pos$_1(G)$. Vì lim$_{\psi ,\mathfrak{F}}\|\psi \|^{-1}_{\infty}\psi =\varphi$, ta kết luận rằng $\varphi$ thuộc bao lồi đóng của tập các điểm cực biên của Pos$_1(G)$. Mệnh đề được chứng minh.

### 7. Sự tồn tại của các biểu diễn bất khả quy

Ta giữ ký hiệu của số trước.

#### Định lý 3 (Raikov) {#ts-v-s3-thm-3 .statement tag=03CR}

Tôpô yếu trên Pos$_1(G)$ trùng với tôpô hội tụ đều trên các compact.

Trước hết ta sẽ chứng minh một vài bổ đề.

#### Bổ đề 5 {#ts-v-s3-lem-5 .statement tag=03CS}

Cho X là một không gian tôpô compact địa phương và $\nu$ một độ đo dương trên X. Trên mọi tập con bị chặn của $\mathscr{C}_b(X)$, tôpô cảm sinh bởi tôpô yếu $\sigma (L^{\infty}(X),L^1(X))$ thô hơn tôpô hội tụ đều trên các compact.

Cho B là một tập con bị chặn của $\mathscr{C}_b(X)$ và lấy $M\in \mathbf{R}_+$ sao cho $\|\varphi \|_{\infty}\leqslant M$ với mọi $\varphi \in B$. Cho $\psi \in L^1(X, \nu )$ và $\varepsilon  >0$. Cố định một tập con compact K của X sao cho

$$
\int_{X-K}|\psi |d\nu  < \varepsilon
$$

Khi đó, với mọi $\varphi_1$ và $\varphi_2$ trong B, ta có

$$
\langle \varphi_1-\varphi_2, \psi \rangle =\int_X\psi (\varphi_1-\varphi_2)d\nu
$$

$$
=\int_K\psi (\varphi_1-\varphi_2)d\nu +\int_{X-K}\psi (\varphi_1-\varphi_2)d\nu
$$

do đó

$|\langle \varphi_1-\varphi_2, \psi \rangle |\leqslant$ sup$_{x\in K}|\varphi_1(x)-\varphi_2(x)| \|\psi \|_1+ 2M\varepsilon$,

và bổ đề được chứng minh.

#### Bổ đề 6 {#ts-v-s3-lem-6 .statement tag=03CT}

Cho $\psi \in L^1(G)$. Cho B là một tập con bị chặn của không gian Banach $L^{\infty}(G)$. Ánh xạ $\varphi \mapsto \psi *\varphi$ từ B vào $\mathscr{C}_b(G)$ là liên tục khi B được trang bị tôpô yếu và $\mathscr{C}_b(G)$ được trang bị tôpô hội tụ compact.

Cho $\varphi \in L^{\infty}(G)$ và $\eta \in L^1(G)$. Hàm $\Delta^{-1}\check{\eta}$ thuộc $L^1(G)$ và $\langle \eta ,\check{\psi}\rangle =\langle \Delta^{-1}\check{\eta , \psi}\rangle ($x. INT, VII, p. 19, § 1, n$^o3$, công thức (22)). Do đó, ánh xạ $\varphi \mapsto \check{\varphi}$ là một tự đẳng cấu của không gian $L^{\infty}(G)$ được trang bị tôpô yếu.

Cho $\varphi \in L^{\infty}(G)$. Theo INT, VIII, p. 167, § 4, n$^o5$, prop. 14, hàm $\psi *\varphi$ thuộc $\mathscr{C}_b(G)$ và thỏa mãn

$$
(\psi *\varphi )(g) =\int_G\psi (h)\varphi (h^{-1}g)d\mu(h)
$$

$=\int_G\psi (gy)\check{\varphi}(y)d\mu(y) =\langle \check{\varphi ,}\boldsymbol{\gamma }$[^1]$_G(g^{-1})\psi \rangle$ với mọi $g\in G$. Suy ra ánh xạ tuyến tính $u:\varphi \mapsto \psi *\varphi$ là một ánh xạ liên tục từ không gian $L^{\infty}(G)$ được trang bị tôpô yếu vào $\mathscr{C}_b(G)$ được trang bị tôpô hội tụ đơn.

Cho $\varphi \in B$ và $(g, h)\in G\times G$. Theo công thức trên, ta có

$|u(\varphi )(g)-u(\varphi )(h)|\leqslant \|\check{\varphi}\|_{\infty}\|(\boldsymbol{\gamma }$[^1]$_G(g^{-1})-\boldsymbol{\gamma }$[^1]$_G(h^{-1}))\psi \|_1$.

Vì B bị chặn và biểu diễn chính quy trái của G trong $L^1(G)$ là liên tục (No. 4 của V, p. 405), điều này suy ra rằng $u(B)$ là một tập con đồng liên tục của $\mathscr{C}_b(G)$. Mệnh đề khi đó suy ra từ điều nói trên và từ TG, X, p. 16, đl. 1.

#### Bổ đề 7 {#ts-v-s3-lem-7 .statement tag=03CU}

Cho $\psi \in L^1(G)$ sao cho $\psi \geqslant 0$ và $\int\psi = 1$. Ký hiệu bởi $p$ nửa chuẩn trên $\mathscr{C}_b(G)$ được xác định bởi $p(\varphi ) =|\langle \varphi , \psi \rangle |$ với mọi $\varphi \in \mathscr{C}_b(G)$. Với mọi $\varphi \in$ Pos$_1(G)$, ta có

$$
\|\psi *\varphi -\varphi \|_{\infty}\leqslant \surd\overline{2p(1 -\varphi)}
$$

Cho $\varphi \in$ Pos$_1(G)$ và $x\in G$. Theo INT, VIII, p. 167, § 4, n$^o5$, prop. 14, ta được

$$
|\psi *\varphi (x)-\varphi (x)|=|\int_G(\varphi (y^{-1}x)-\varphi (x))\psi (y)d\mu(y)|
$$

$$
\leqslant \int_G|\varphi (y^{-1}x)-\varphi (x)|\psi (y)d\mu(y)
$$

$$
\leqslant \int_G\surd\overline{2(1 -\mathscr{R}\varphi(y))}\psi (y)d\mu(y)
$$

áp dụng ước lượng trên (1) của V, p. 446. Bất đẳng thức Cauchy-Schwarz khi đó cho

$\surd \int 1/2\int 1/2$

$$
\|\psi *\varphi -\varphi \|_{\infty}\leqslant \overline{2}(_G(1-\mathscr{R}(\varphi ))\psi  d\mu)(_G\psi  d\mu)
$$

$$
\surd \surd
$$

$\leqslant$ 2 $p(1-\varphi )$,

do đó suy ra kết quả.

#### Bổ đề 8 {#ts-v-s3-lem-8 .statement tag=03CV}

Cho K là một trường tôpô và E, F là các không gian vectơ tôpô trên K. Cho $f$ là một ánh xạ từ E vào F và X là một tập con của E. Cho $x\in X$. Ánh xạ $f|X$ liên tục tại $x$ nếu, với mọi lân cận W của 0 trong F, tồn tại một lân cận U của $x$ trong E và một ánh xạ liên tục $g$ từ X vào F sao cho $(f-g)(U\cap X)\subset W$.

Cho $W_0$ là một lân cận của 0 trong F và cho $V_0$ là một lân cận đối xứng của 0 trong F sao cho $V_0+V_0+V_0\subset W_0$. Cho $U_0$ là một lân cận của $x$ trong E và $g$ là một ánh xạ liên tục từ X vào F sao cho $(f-g)(U_0\cap X)\subset V_0$. Tồn tại một lân cận $U_1$ của $x$ trong E sao cho $g(U_1\cap X)\subset g(x) + V_0$. Với mọi $y\in U_0\cap U_1\cap X$, ta có

$$
f(y)-f(x) = (f(y)-g(y)) + (g(y)-g(x))+
$$

$$
(g(x)-f(x))\in V_0+ V_0+ V_0\subset W_0
$$

vì thế $f(y)\in f(x) + W_0$, do đó suy ra kết quả.

Bây giờ chứng minh định lý 3. Ký hiệu bởi Pos$_1(G)_f$ (resp. Pos$_1(G)_c$) tập Pos$_1(G)$ được trang bị tôpô yếu (resp. tôpô hội tụ compact); tương tự, ký hiệu bởi $\mathscr{C}_b(G)_f$ (resp. $\mathscr{C}_b(G)_c$) không gian $\mathscr{C}_b(G)$ được trang bị tôpô yếu (resp. tôpô hội tụ compact).

Ánh xạ đồng nhất từ Pos$_1(G)_c$ vào Pos$_1(G)_f$ là liên tục (bổ đề 5). Ngược lại, ký hiệu bởi $\iota$ phép bao hàm của Pos$_1(G)_f$ vào $\mathscr{C}_b(G)_c$. Hãy chứng minh rằng $\iota$ liên tục, để kết thúc chứng minh.

Cho $\varphi_1\in$ Pos$_1(G)$. Để kiểm tra rằng $\iota$ liên tục tại $\varphi_1$, ta áp dụng bổ đề 8. Cho W là một lân cận của 0 trong $\mathscr{C}_b(G)_c$. Chỉ cần tìm một ánh xạ tuyến tính $u$ của $\mathscr{C}_b(G)$ vào $\mathscr{C}_b(G)$ mà, khi chuyển qua các không gian con, cảm sinh một ánh xạ liên tục của Pos$_1(G)_f$ vào $\mathscr{C}_b(G)_c$, cùng với một lân cận U của 0 trong Pos$_1(G)_f$, sao cho ta có $(\iota -u)(U\cap$ Pos$_1(G))\subset W$.

Tồn tại $\varepsilon  >0$ sao cho W chứa tập các $\varphi \in \mathscr{C}_b(G)$ thỏa mãn $\|\varphi \|_{\infty}\leqslant \varepsilon$. Vì $\varphi_1(e) = 1$, tồn tại một lân cận compact V của $e$ trong G sao cho

sup$_{x\in V}|1-\varphi_1(x)|\leqslant \frac{\varepsilon^2}{4}$.

Cho $\varphi_V$ là hàm đặc số của V, và đặt $\psi_V=\mu(V)^{-1}\varphi_V$. Ánh xạ tuyến tính $u:\varphi \mapsto \psi_V*\varphi$ của Pos$_1(G)_f$ vào $\mathscr{C}_b(G)_c$ là liên tục (bổ đề 6).

Ký hiệu $q_V$ là nửa chuẩn $\varphi \mapsto  |\langle \varphi , \psi_V\rangle |$ trên $\mathscr{C}_b(G)$; nó liên tục đối với tôpô yếu. Vì $\psi_V$ triệt tiêu ở ngoài V, ta có $q_V(1-\varphi_1)\leqslant \varepsilon^2/4$; do đó tồn tại một lân cận U của $\varphi_1$ trong $\mathscr{C}_b(G)_f$ sao cho $q_V(1-\varphi )\leqslant \varepsilon^2/2$ với mọi $\varphi \in U$.

Cho $\varphi \in U\cap$ Pos$_1(G)$. Theo bổ đề 7, ta có

$$
\|(\iota -u)(\varphi )\|_{\infty}\leqslant \surd\overline{2q_V(1 -\varphi)}\leqslant \varepsilon
$$

do đó $(\iota -u)(U)\subset W$. Định lý được chứng minh.

Nói chung, tôpô yếu trên Pos$_{\leqslant 1}(G)$ không trùng với tôpô hội tụ compact, như được chỉ ra bởi ví dụ của nhóm $\mathbf{R}$.

Nhắc lại rằng $\widehat{G}$ ký hiệu tập hợp các lớp biểu diễn unita bất khả quy của G (V, p. 393, định nghĩa 8).

#### Định lý 4 (Gelfand–Raikov) {#ts-v-s3-thm-4 .statement tag=03CW}

Với mọi $x\not =e$ trong G, tồn tại một biểu diễn unita bất khả quy $\pi$ của G sao cho $\pi (x)$ không phải là tự đồng cấu đồng nhất của không gian của $\pi$.

Cho $x\in G$ sao cho $\pi (x)$ là đồng nhất với mọi $\pi \in \widehat{G}$. Suy ra $\varphi (x) =\varphi (e) = 1$ với mọi điểm cực $\varphi$ của Pos$_1(G)$ (mệnh đề 11 của V, p. 444), do đó với mọi $\varphi \in$ Pos$_1(G)$ theo mệnh đề 14 vì dạng tuyến tính $\varphi \mapsto \varphi (e)$ liên tục trên Pos$_1(G)$ được trang bị tôpô yếu (định lý 3). Nhưng nếu $x\not =e$, tồn tại $f\in L^2(G)$ có chuẩn 1 sao cho $\langle f|\boldsymbol{\gamma }_G(x)f\rangle = 0$(V, p. 406, bổ đề 3). Vì vế trái của đẳng thức này có dạng $\varphi (x)$, trong đó $\varphi \in$ Pos$_1$(G), nên đây là một mâu thuẫn.

Nếu G không compact địa phương, không phải luôn luôn đúng rằng các biểu diễn unita bất khả quy của G phân biệt các điểm của G.

#### Hệ quả {#ts-v-s3-n7-cor-1 .statement tag=03CX}

Với mọi phần tử $g\not =h$ trong G, tồn tại một biểu diễn bất khả quy $\pi \in \widehat{G}$ và một hệ số ma trận $f$ của $\pi$ sao cho $f(g)\not =f(h)$. Đặc biệt, đại số con Υ(G) của $\mathscr{C}_b(G)$ phân biệt các điểm của G.

Cho $g\not =h$ trong G. Tồn tại một biểu diễn bất khả quy $\pi \in \widehat{G}$ sao cho $\pi (g)\not =\pi (h)$ (định lý 4); do đó tồn tại $x$ và $y$ trong không gian của $\pi$ sao cho $\langle x|\pi (g)y\rangle  \not =\langle x|\pi (h)y\rangle$.

### 8. Các hàm xác định dương trên một nhóm giao hoán compact địa phương

Trong số này, G là một nhóm giao hoán compact địa phương và $\mu$ ký hiệu một độ đo Haar trên G. Ta ký hiệu $\widehat{G}$ là nhóm đối ngẫu của G và $\widehat{\mu}$ là độ đo đối ngẫu với $\mu$ (định nghĩa 4 của II, p. 214). Ta ký hiệu bởi $\mathscr{F}$ biến đổi Fourier trên không gian Banach $\mathscr{M}^1(G)$ của các độ đo bị chặn trên G.

Vì $\mathscr{C}_0(G)$ là bao đóng của $\mathscr{K}(G)$ trong $\mathscr{C}_b$(G), không gian Banach $\mathscr{M}^1(G)$ đối ngẫu của $\mathscr{K}(G)$ được trang bị tôpô của $\mathscr{C}_b(G)$ được đồng nhất với đối ngẫu của $\mathscr{C}_0(G) ($x. INT, III, p. 56, § 1, n$^o8)$. Ta trang bị cho $\mathscr{M}^1(G)$ tôpô yếu liên kết với tính đối ngẫu này.

#### Bổ đề 9 {#ts-v-s3-lem-9 .statement tag=03CY}

Biến đổi Fourier là một ánh xạ liên tục từ $\mathscr{M}^1(G)$ được trang bị tôpô yếu vào $\mathscr{C}_b(\widehat{G})$ được trang bị tôpô cảm sinh bởi tôpô yếu $\sigma (L^{\infty}(\widehat{G}),L^1(\widehat{G}))$.

Cho $\mathfrak{F}$ là một bộ lọc trên $\mathscr{M}^1(G)$ hội tụ yếu đến một độ đo bị chặn $\nu$ trên G. Với mọi $\varphi \in L^1(\widehat{G})$, ta có $\mathscr{F}(\varphi )\in \mathscr{C}_0(G)$ (Mệnh đề 4 của II, p. 209), do đó

$$
\int_{\widehat{G}}\varphi \mathscr{F}(\nu )d\widehat{\mu}=\int_G\mathscr{F}(\varphi )d\nu
$$

= lim$_{\eta ,\mathfrak{F}}\int_G\mathscr{F}(\varphi )d\eta =$ lim$_{\eta ,\mathfrak{F}}\int_{\widehat{G}}\varphi \mathscr{F}(\eta )d\widehat{\mu}$,

theo tính chất chuyển vị của biến đổi Fourier (Mệnh đề 13 của II, p. 221). Bổ đề được suy ra.

#### Định lý 5 (Bochner) {#ts-v-s3-thm-5 .statement tag=03CZ}

Một hàm liên tục $\varphi$ trên $\widehat{G}$ thuộc Pos($\widehat{G}$) khi và chỉ khi tồn tại một độ đo dương bị chặn $\nu$ trên G sao cho $\varphi =\mathscr{F}(\nu )$.

Cho $\nu \in \mathscr{M}^1(G)$ là một độ đo dương. Biến đổi Fourier của nó là liên tục. Với mọi họ hữu hạn $(x_i)_{i\in I}$ trong $\widehat{G}$ và mọi họ hữu hạn $(t_i)_{i\in I}$ các số phức, ta được

$$
\sum_{i\in I}\sum_{j\in I}\overline{t}_it_j\mathscr{F}(\nu )(x^{-1}_ix_j) =\sum_{i\in I}\sum_{j\in I}\overline{t}_it_j\int_Gx_i\overline{x}_jd\nu
$$

$$
=\int_G|\sum_{i\in I}\overline{t}_ix_i|^2d\nu \geqslant 0
$$

vì $\nu$ là một độ đo dương. Do đó biến đổi Fourier của $\nu$ là một hàm kiểu dương trên $\widehat{G}$ (Định lý 1 của V, p. 432, (ii)).

Ta hãy chứng minh đảo lại. Trang bị tập hợp Pos$_{\leqslant 1}(\widehat{G})$ với tôpô yếu, được cảm sinh như trên bởi tôpô yếu $\sigma (L^{\infty}(\widehat{G}),L^1(\widehat{G}))$. Tập Pos$_{\leqslant 1}(\widehat{G})$ là compact và lồi (Hệ quả của Mệnh đề 13 của V, p. 448). Theo Mệnh đề 14 của V, p. 450, Mệnh đề 11 của V, p. 444 và Hệ quả 7 của V, p. 390, các điểm cực biên của Pos$_{\leqslant 1}(\widehat{G})$ là hàm không và các phần tử của $\widehat{G}$.

Cho $\mathscr{N}$ là tập hợp các độ đo dương bị chặn có khối lượng $\leqslant 1$ trên G; nó là compact trong $\mathscr{M}^1(G)$ được trang bị tôpô yếu (EVT, III, p. 17, Hệ quả 3). Theo Bổ đề 9 và phần đầu của chứng minh, biến đổi Fourier trên G xác định, bằng cách chuyển qua các không gian con, một ánh xạ liên tục từ $\mathscr{N}$ vào Pos$_{\leqslant 1}(\widehat{G})$; do tính thuần nhất, chỉ cần chứng minh rằng ánh xạ này là toàn ánh. Ảnh $\mathscr{F}(\mathscr{N})$ của $\mathscr{N}$ dưới biến đổi Fourier là lồi và compact; nó chứa hàm không và các phần tử của $\widehat{G}$ (thực ra, các phần tử này có dạng ev$_x:\chi \mapsto \chi (x)$ với một phần tử $x$ của G theo Định lý 2 của II, p. 220, và ta có ev$_x=\mathscr{F}(\varepsilon_{x^{-1}})$). Vậy tập $\mathscr{F}(\mathscr{N})$ chứa các điểm cực biên của Pos$_{\leqslant 1}$(G), do đó $\mathscr{F}(\mathscr{N}) =$ Pos$_{\leqslant 1}(G)$ theo định lý Krein-Milman (EVT, II, p. 59, Định lý 1). Điều này kết thúc chứng minh.

Khi $G =\mathbf{R}^k$ với một số nguyên $k\in \mathbf{N}$, định lý này tương ứng với Mệnh đề 11 của INT, IX, p. 94, § 6, n$^o12$.

## BÀI TẬP {#ts-v-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
