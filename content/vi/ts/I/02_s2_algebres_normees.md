---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 2
section_title: Algèbres normées
lang: vi
source: ts-i-ii-fr
book_pages: TS I.15-TS I.29, TS I.155-TS I.165
pdf_pages: 0028-0042, 0168-0178
extraction: native
subsections:
    - "no": 1
      title: Généralités
      page: 15
      pdf_page: 28
    - "no": 2
      title: Exemples
      page: 17
      pdf_page: 30
    - "no": 3
      title: Rayon spectral
      page: 20
      pdf_page: 33
    - "no": 4
      title: Inverses
      page: 22
      pdf_page: 35
    - "no": 5
      title: Spectre d’un élément dans une algèbre normée
      page: 24
      pdf_page: 37
    - "no": 6
      title: Spectre relatif à une sous-algèbre
      page: 28
      pdf_page: 41
statements: 28
exercises: 37
content_sha256: 25491c70f0bc9884b9e5f08138792090105073898fb42df6824ea042c6ecaa53
translated_from: content/en-mt/ts/I/02_s2_algebres_normees.md
source_lang: en-mt
translation_method: machine
source_content_sha256: eac18d96db0024c9ae65b4cdc9982700a66796dc8684b068f789f813a68e6fef
translation_model: gpt-5-6-mini
translation_run: translate-vi-fa1635aa
glossary_version: 34
glossary_terms_sha256: 437e62dbb5b36a1f90b88aac9f1261de68f6f5cf2833c0931d9264a81a382bab
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ĐẠI SỐ CHUẨN

Trong tiết này, K ký hiệu một trong các trường $\mathbf{R}$ hoặc $\mathbf{C}$.

### 1. Những điều tổng quát

Nhắc lại (xem TG, IX, p. 37, định nghĩa 9) rằng một đại số chuẩn là một đại số A trên K được trang bị một chuẩn $x\mapsto  \|x\|$ sao cho:

$$
\|xy\|\leqslant \|x\| \|y\| \tag{1}
$$

với mọi $x,y\in A$. Nếu A đầy đủ, ta nói A là một đại số Banach.

Cho A là một đại số khả chuẩn đầy đủ trên K. Tôpô của A có thể được xác định bởi một chuẩn thỏa mãn (1) (xem TG, IX, p. 38). Khi A được trang bị cấu trúc đại số chuẩn được xác định bởi một chuẩn như vậy, ta cũng nói rằng đại số A là một đại số Banach.

Ta cũng nhắc lại các tính chất sau (xem TG, IX, p. 38–39):

(1) Nếu A là một đại số chuẩn khác không và có một phần tử đơn vị $e$, thì $\|e\|\geqslant 1$.

(2) Cho A là một K-đại số chuẩn. Đại số đối của A, được trang bị cùng một chuẩn, là một đại số chuẩn. Bao đầy đủ của A, được trang bị chuẩn thu được bằng cách mở rộng liên tục chuẩn của A, là một K-đại số Banach. Mọi đại số con của A, được trang bị chuẩn cảm sinh, đều là một đại số chuẩn. Nếu I là một iđêan hai phía đóng của A, đại số $A/I$, được trang bị chuẩn xác định bởi $\|\dot{x}\|=$ inf$_{x\in\dot{x}}\|x\|$ với mọi $\dot{x}\in A/I$, là một đại số chuẩn.

(3) Cho $(A_i)_{\in I}$ là một họ các đại số chuẩn và B là đại số tích của các đại số $A_i$. Đại số con gồm các phần tử $(x_i)_{i\in I}$ của B sao cho $\|(x_i)\|=$ sup$_{i\in I}\|x_i\|<+\infty$, là một đại số chuẩn, được gọi là đại số chuẩn tích của các đại số $(A_i)_{i\in I}$. Nếu $A_i$ là một đại số Banach với mọi $i$, thì A là một đại số Banach.

Cho A là một đại số chuẩn. Cho $(y_i)_{i\in I}$ là một họ các phần tử của A; đại số con đóng nhỏ nhất B của A chứa các phần tử $y_i$ được gọi là đại số con đóng của A sinh bởi các $y_i$; nếu B = A, ta nói rằng các $y_i$ sinh tôpô đại số chuẩn A, hay họ $(y_i)_{i\in I}$ là một hệ sinh tôpô của đại số chuẩn A.

Tương tự, nếu A là một đại số chuẩn có đơn vị, đại số con có đơn vị đóng nhỏ nhất chứa các phần tử $y_i$ được gọi là đại số con có đơn vị đóng của A sinh bởi các $y_i$. Nếu nó bằng A, ta nói rằng các $y_i$ sinh tôpô đại số chuẩn có đơn vị A.

Cho A là một K-đại số chuẩn. Ký hiệu $\widetilde{A}$ là đại số thu được từ A bằng phép nối một phần tử đơn vị. Trên $\widetilde{A}$, định nghĩa một chuẩn bằng cách đặt $\|(\lambda , x)\|=|\lambda |+\|x\|$ với mọi $\lambda \in K$ và mọi $x\in A$. Ta có

$$
\|(\lambda , x)(\mu, y)\|=|\lambda \mu|+\|xy+\mu x+\lambda y\|
$$

$$
\leqslant |\lambda | |\mu|+\|x\| \|y\|+|\mu| \|x\|+|\lambda | \|y\|
$$

$$
=\|(\lambda , x)\| \|(\mu, y)\|
$$

Do đó $\widetilde{A}$ trở thành một đại số chuẩn, được gọi là đại số chuẩn có đơn vị suy ra từ A bằng phép nối một phần tử đơn vị. Đại số A được đồng nhất với iđêan hai phía đóng $\{0\} \times A$ của $\widetilde{A}$.

#### Định nghĩa 1 {#ts-i-s2-def-1 .statement tag=025W}

Cho A là một đại số chuẩn. Với $a\in A$, ký hiệu $\boldsymbol{\gamma }_a$ và $\boldsymbol{\delta }_a$ là các ánh xạ $x\mapsto ax$, và $x\mapsto xa$ từ A vào A. Ánh xạ $\boldsymbol{\gamma }:a\mapsto \boldsymbol{\gamma }_a$ là một biểu diễn của A trong A, được gọi là biểu diễn chính quy trái của A. Ánh xạ $\boldsymbol{\delta }:a\mapsto \boldsymbol{\delta }_a$ là một biểu diễn của đại số đối của A trong A, được gọi là biểu diễn chính quy phải của A.

#### Bổ đề 1 {#ts-i-s2-lem-1 .statement tag=025X}

Cho A là một đại số chuẩn. Biểu diễn chính quy trái của A và biểu diễn chính quy phải của A là liên tục với chuẩn $\leqslant 1$.

Nếu đại số A có đơn vị, các ánh xạ $x\mapsto  \|\boldsymbol{\gamma }_x\|$ và $x\mapsto  \|\boldsymbol{\delta }_x\|$ là các chuẩn trên A, xác định tôpô của A. Chúng thỏa mãn bất đẳng thức (1).

Nếu đại số chuẩn có đơn vị A khác không, nghĩa là nếu $e\not= 0$, ta còn có $\|\boldsymbol{\gamma }_e\|=\|\boldsymbol{\delta }_e\|= 1$.

Ngay lập tức thấy rằng $\|\boldsymbol{\gamma }_x\|\leqslant \|x\|$ và $\|\boldsymbol{\delta }_x\|\leqslant \|x\|$.

Nếu A có một phần tử đơn vị $e$, thì ta có $x=\boldsymbol{\gamma }_xe=\boldsymbol{\delta }_xe$, do đó: (2) $\|x\|\leqslant \|\boldsymbol{\gamma }_x\| \cdot  \|e\|\|x\|\leqslant \|\boldsymbol{\delta }_x\| \cdot  \|e\|$.

Trong trường hợp này, $x\mapsto  \|\boldsymbol{\gamma }_x\|$ và $x\mapsto  \|\boldsymbol{\delta }_x\|$ do đó là các chuẩn tương đương với chuẩn của A. Chúng thỏa mãn (1) vì $\boldsymbol{\gamma }$ và $\boldsymbol{\delta }$ là các biểu diễn.

Khẳng định cuối cùng suy ra từ sự kiện rằng $\boldsymbol{\gamma }_e=\boldsymbol{\delta }_e=$ Id$_A$.

### 2. Ví dụ

1) Cho E là một không gian chuẩn. Trang bị cho E tích được xác định bởi $ab= 0$ với mọi $a$ và $b$ trong E; điều này xác định trên E một cấu trúc đại số chuẩn.

2) Cho X là một tập hợp. Ta ký hiệu bởi $\mathscr{B}(X; K)$ đại số chuẩn của các hàm bị chặn trên X với các giá trị trong K, được trang bị chuẩn

$\|f\|=$ sup$_{x\in X}|f(x)|$

(TG, X, p. 22). Nó là một đại số Banach có đơn vị trên K (TG, X, p. 21, hệ quả 1). Nó là giao hoán. Cho $f$ là một phần tử của $\mathscr{B}(X; K)$. Khi đó $f$ khả nghịch trong $\mathscr{B}(X; K)$ khi và chỉ khi ta có

inf$_{x\in X}|f(x)|>0$.

Phổ của $f$ do đó là tập hợp các $\lambda \in K$ sao cho

inf$_{x\in X}|f(x)-\lambda |= 0$,

nghĩa là bao đóng trong K của tập hợp $f(X)$ gồm các giá trị của $f$.

3) Cho X là một không gian tôpô. Ta ký hiệu bởi $\mathscr{C}_b(X; K)$ đại số con có đơn vị của $\mathscr{B}(X; K)$ gồm các hàm liên tục và bị chặn trên X với các giá trị trong K$,\mathscr{C}_0(X; K)$ đại số con của $\mathscr{C}_b(X; K)$ gồm các hàm tiến về 0 ở vô cực (cf. INT, III, §1, n$^o2$ và TG, X, p. 40, hệ quả 2). Ta nhắc lại rằng $\mathscr{K}(X; K)$ ký hiệu đại số con của $\mathscr{C}_b(X; K)$ gồm các hàm liên tục có giá compact.

Các đại số $\mathscr{C}_b(X; K)$ và $\mathscr{C}_0(X; K)$ là các đại số Banach giao hoán trên K; thật vậy, chúng là các không gian con đóng của $\mathscr{B}(X; K)$ (TG, X, p. 21, hệ quả 2 và INT, III, §1, n$^o2$).

Nghịch đảo của một hàm liên tục khác không ở mọi nơi là liên tục, đại số con $\mathscr{C}_b(X; K)$ là một đại số con đầy đủ của $\mathscr{B}(X; K)$. Đặc biệt, phổ của một phần tử $f$ của $\mathscr{C}_b(X; K)$ bằng $\overline{f(X)}$.

Nếu X là rời rạc, ta có $\mathscr{C}_b(X; K) =\mathscr{B}(X; K)$.

Nếu X là compact, ta có $\mathscr{C}_b(X; K) =\mathscr{K}(X; K) =\mathscr{C}(X; K)$, đại số chuẩn có đơn vị $\mathscr{C}(X; K)$ của các hàm liên tục trên X với các giá trị trong K. Trong trường hợp này, một phần tử $f\in \mathscr{C}(X; K)$ khả nghịch khi và chỉ khi $f$ không nhận giá trị 0, và phổ của $f$ bằng tập hợp $f(X)$ gồm các giá trị của $f$.

Bây giờ giả sử rằng X không compact. Đại số $\mathscr{C}_0(X; K)$ khi đó không có đơn vị; đại số thu được từ nó bằng phép nối một phần tử đơn vị được đồng nhất với đại số con $K\cdot 1\oplus \mathscr{C}_0(X; K)$ của $\mathscr{C}(X; K)$ gồm các hàm có giới hạn ở vô cực. Để một phần tử của đại số con này khả nghịch, điều kiện cần và đủ là nó không triệt tiêu và giới hạn của nó ở vô cực khác không. Suy ra rằng với mọi $f\in \mathscr{C}_0(X; K)$, phổ của $f$ bằng $f(X)\cup  \{0\}$.

Phổ của $f\in \mathscr{K}(X; K)$ bằng $f(X)$ (thật vậy, nếu X không compact, thì 0 thuộc $f(X)$).

4) Cho $n\geqslant 0$ là một số nguyên. Cho $A_n$ là đại số của các hàm $f: [0,1]\rightarrow K$ có các đạo hàm liên tục trong $[0,1]$ đến cấp $n$, được trang bị chuẩn

$\|f\|=\sum^nk1$

sup$_{0\leqslant t\leqslant 1}|f^{(k)}(t)|$.

$k=0$

Nếu $f, g\in A_n$, ta có

$\|f g\|=\sum^nk1$! sup$|(f g)^{(k)}(t)|=\sum^nk1$! sup$|\sum^k(ks)f^{(s)}(t)g^{(k-s)}(t)|$

$k=0k=0s=0$

$\leqslant \sum^n\sum^ks$!($k1-s$)! sup$_{0\leqslant t\leqslant 1}|f^{(s)}(t)|$ sup$_{0\leqslant t\leqslant 1}|g^{(k-s)}(t)|=\|f\| \|g\|$,

$k=0s=0$

theo công thức Leibniz (FVR, I, p. 28, mệnh đề 2), do đó $A_n$ là một đại số Banach giao hoán có đơn vị.

5) Cho E là một không gian Banach mà chuẩn được ký hiệu bởi $p$. Đại số $\mathscr{L}(E)$ của các cấu xạ liên tục của E, được trang bị với chuẩn

$\|u\|=$ sup$_{p(x)\leqslant 1}p(u(x))$

là một đại số Banach có đơn vị (EVT, III, p. 14 và p. 24, hệ quả 2 ; TG, X, p. 23, công thức (3)).

6) Cho G là một nhóm compact địa phương. Gọi $e$ là phần tử đơn vị của nó. Cho $\mathscr{M}^1(G)$ là không gian Banach của các độ đo phức bị chặn trên G (INT, III, p. 57). Tích chập (INT, VIII, p. 120, định nghĩa 1) trang bị cho $\mathscr{M}^1(G)$ một cấu trúc đại số Banach phức (INT, VIII, §3, no$^o1$, mệnh đề 2) nhận làm phần tử đơn vị độ đo $\varepsilon_e$ được xác định bởi khối lượng đơn vị đặt tại điểm $e$. Nếu G giao hoán, đại số Banach này giao hoán. Không gian $\mathscr{C}'(G)$ của các độ đo có giá compact là một đại số con của $\mathscr{M}^1(G)$ (loc. cit.).

7) Cho G là một nhóm compact địa phương được trang bị một độ đo Haar $\mu$. Khi đó $L^1_K(G, \mu)$ là một đại số Banach đối với tích chập (INT, VIII, mệnh đề 12, p. 166). Nếu $K =\mathbf{C}$, ánh xạ được xác định bởi $f\mapsto f \mu$ cho phép đồng nhất $L^1_{\mathbf{C}}(G, \mu)$ với một đại số con của đại số Banach $\mathscr{M}^1(G)$.

Nếu G giao hoán, đại số Banach $L^1_K(G, \mu)$ giao hoán.

8) Lấy $G =\mathbf{Z}$ và $K =\mathbf{C}$ trong Ví dụ 7. Khi đó $L^1_{\mathbf{C}}(\mathbf{Z})$ là đại số Banach phức giao hoán của các dãy $(x_n)_{n\in\mathbf{Z}}$ sao cho $\sum_n|x_n|<+\infty$, tích của các phần tử $(x_n)$ và $(y_n)$ là $(z_n)$, trong đó

$$
z_n=\sum_{k\in\mathbf{Z}}x_ky_{n-k}
$$

và chuẩn $\|(x_n)\|=\sum_n|x_n|$. Đại số này nhận làm phần tử đơn vị dãy $\varepsilon = (\varepsilon_n)$ sao cho $\varepsilon_0= 1$ và $\varepsilon_n= 0$ với $n\not= 0$.

Gọi $\mathbf{U}$ là đường tròn đơn vị trong $\mathbf{C}$. Nếu $x= (c_n)$ là một phần tử của A, gọi $\varphi (x)$ là hàm liên tục trên $\mathbf{U}$ có giá trị tại $e^{it}$ là

$$
\varphi (x)(e^{it}) =\sum_{n\in\mathbf{Z}}c_ne^{int}
$$

Người ta kiểm tra rằng $\varphi$ là một cấu xạ của $L^1_{\mathbf{C}}(\mathbf{Z})$ lên một đại số A các hàm liên tục trên $\mathbf{U}$, phép nhân trong A là phép nhân thông thường. Bằng cách lấy tích phân từng số hạng của đẳng thức

$$
((\sum_{m\in\mathbf{Z}}c_me^{imt})\cdot e^{-int}=\varphi (x)(e^{it})\cdot e^{-int}
$$

suy ra

$$
c_n=\frac{1}{2\pi}\int_0^1\varphi (x)(e^{it})e^{-int}dt
$$

Đặc biệt, suy ra rằng cấu xạ $\varphi$ là đơn ánh. Đại số A, được trang bị với chuẩn suy ra từ chuẩn của $L^1_{\mathbf{C}}(\mathbf{Z})$ qua $\varphi$, được gọi là đại số Banach của các chuỗi Fourier hội tụ tuyệt đối. Nó nhận làm phần tử đơn vị hàm $1 =\varphi (\varepsilon )$.

9) Cho Δ là đĩa các số phức $z$ thỏa mãn $|z|\leqslant 1$. Đại số A gồm các hàm liên tục trên Δ và giải tích ở phần trong của Δ (VAR, R1, p. 26, 3.2.1) được trang bị chuẩn $\|f\|=$ sup$_{z\in\Delta}|f(z)|$. Khi đó A là một đại số Banach giao hoán có đơn vị.

### 3. Bán kính phổ

#### Bổ đề 2 (Bổ đề Fekete) {#ts-i-s2-lem-2 .statement tag=025Y}

Cho $(a_n)_{n\geqslant 1}$ là một dãy các số thực. Giả sử rằng

$$
a_{n+m}\leqslant a_n+a_m
$$

với mọi $n\geqslant 1$ và mọi $m\geqslant 1$. Khi đó dãy $(a_n/n)_{n\geqslant 1}$ hội tụ và thỏa mãn

lim$_{n\rightarrow+\infty}\frac{a_n}{n}=$ inf$_{n\geqslant 1}\frac{a_n}{n}$.

Đặt $a_0= 0$ ; bất đẳng thức $a_{n+m}\leqslant a_n+a_m$ vẫn đúng với mọi $n\geqslant$ 0 và mọi $m\geqslant 0$. Cố định một số nguyên $m\geqslant$ 1. Với mọi số nguyên $n\geqslant 1$, gọi $q(n)$ và $r(n)$ là các số nguyên sao cho $n=q(n)m+r(n)$ và $0\leqslant r(n)< m$ (E, III, p. 39, th. 1). Khi đó giả thiết kéo theo

$$
\frac{a_n}{n}\leqslant \frac{a_{q(n)m}}{n}+\frac{a_{r(n)}}{n}\leqslant \frac{q(n)a_m}{n}+\frac{a_{r(n)}}{n}\leqslant \frac{q(n)}{n}a_m+\frac{m}{n}
$$

Cho $n$ tiến tới $+\infty$, ta suy ra lim sup$_n(a_n/n)\leqslant a_m/m$ vì $q(n)/n\rightarrow 1/m$. Vì điều này đúng với mọi $m\geqslant 1$, do đó ta có

lim sup$_{n\rightarrow+\infty}\frac{a_n}{n}\leqslant$ inf$_{m\geqslant 1}\frac{a_m}{m}\leqslant$ lim inf$_{n\rightarrow+\infty}\frac{a_n}{n}$.

Các bất đẳng thức này chứng minh sự hội tụ của dãy $(a_n/n)_{n\geqslant 1}$ cũng như công thức lim $a_n/n=$ inf$_{n\geqslant 1}a_n/n$.

#### Mệnh đề 1 {#ts-i-s2-prop-1 .statement tag=025Z}

Cho A là một đại số chuẩn. Với mọi $x\in A$, dãy $(\|x^n\|^{1/n})_{n\geqslant 1}$ hội tụ và giới hạn của nó $\varrho (x)$ bằng inf$_{n\geqslant 1}\|x^n\|^{1/n}$. Hơn nữa, với mọi chuẩn $x\mapsto  \|x\|_1$ xác định tôpô của A, ta cũng có

$\varrho (x) =$ lim$_{n\rightarrow+\infty}\|x^n\|^{1/n}_1=$ inf$_{n\geqslant 1}\|x^n\|^{1/n}_1$.

Nếu $x$ là lũy linh, thì $\|x^n\|^{1/n}_1= 0$ với mọi số nguyên $n$ đủ lớn và mọi chuẩn $x\mapsto  \|x\|_1$ xác định tôpô của A.

Giả sử bây giờ rằng $x$ không lũy linh, và đặt $\alpha_n=$ $\|x^n\|$. Ta có $\alpha_n>0$ với mọi số nguyên $n\geqslant 1$, và $\alpha_{n+m}\leqslant \alpha_n\alpha_m$ với mọi $n, m\in \mathbf{N}$ theo (1). Bổ đề 2, áp dụng cho dãy $a_n=$ log($\alpha_n$), cho thấy sự tồn tại của giới hạn $\varrho (x)$ và công thức $\varrho (x) =$ inf$_{n>0}\alpha_n^{1/n}$.

Cho $x\mapsto  \|x\|_1$ là một chuẩn xác định tôpô của A. Tồn tại các số thực $a >0$ và $b >0$ sao cho

$a\|x\|\leqslant\|x\|_1\leqslant b\|x\|$.

$$
a\|x\|\leqslant \|x\|_1\leqslant b\|x\|
$$

với mọi $x\in A$ (EVT, II, p. 7, hệ quả 2). Do đó,

$$
a^{1/n}\|x^n\|^{1/n}\leqslant \|x^n\|^{1/n}_1\leqslant b^{1/n}\|x^n\|^{1/n}
$$

với mọi $n\geqslant 1$, do đó, bằng cách chuyển qua giới hạn, hoặc bằng cách lấy cận dưới lớn nhất, ta có đẳng thức

$\varrho (x) =$ lim$_{n\rightarrow+\infty}\|x^n\|^{1/n}_1=$ inf$_{n>0}\|x^n\|^{1/n}_1$.

#### Định nghĩa 2 {#ts-i-s2-def-2 .statement tag=0260}

Với mọi phần tử $x$ của một đại số định chuẩn A, số thực

$\varrho (x) =$ lim$_{n\rightarrow \infty}\|x^n\|^{1/n}=$ inf$_{n>0}\|x^n\|^{1/n}$

được gọi là bán kính phổ của $x$.

Với mọi phần tử $x$ của A, ta có

$$
\varrho (x)\leqslant \|x\| \tag{3}
$$

(4) $\varrho (x^n) =\varrho (x)^n$, với mọi số nguyên $n\geqslant 1$.

#### Định nghĩa 3 {#ts-i-s2-def-3 .statement tag=0261}

Một phần tử $x$ của A là lũy linh gần nếu $\varrho (x) = 0$.

Điều này tương đương với việc nói rằng, bất kể $\lambda \in K$ là gì, các số $\|(\lambda x)^n\|$ bị chặn với $n\geqslant 1$; hoặc lại rằng, bất kể $\lambda \in K$ là gì, dãy $(\lambda x)^n$ tiến tới 0 khi $n\rightarrow +\infty$.

#### Nhận xét 1 {#ts-i-s2-n3-rem-1 .statement tag=0262}

Cho A là một đại số định chuẩn. Nếu một phần tử $x\in A$ thỏa mãn $\varrho (x) =\|x\|$, ta có $\|x^n\|=\|x\|^n$ với mọi $n\in \mathbf{N}$, theo (3) và (4).

Ngược lại, giả sử rằng $\|x^2\|=\|x\|^2$ với mọi $x\in A$. Khi đó, với mọi số nguyên $n\geqslant 0$, ta có đẳng thức $\|x^{2^n}\|=\|x\|^{2^n}$, do đó $\|x\|=$ $\|x^{2^n}\|^{2^{-n}}$; khi $n$ tiến tới $+\infty$, ta thu được $\|x\|=\varrho (x)$.

#### Nhận xét 2 {#ts-i-s2-n3-rem-2 .statement tag=0263}

Hàm $x\mapsto \varrho (x)$ trên A, là cận dưới lớn nhất của các hàm liên tục $x\mapsto  \|x^n\|^{1/n}$ với $n\geqslant 1$, là nửa liên tục trên (TG, IV, p. 31, hệ quả), nhưng nói chung nó không liên tục. Thậm chí có thể xảy ra (xem bài tập 12 của I, p. 157) rằng một dãy các phần tử lũy linh của A tiến tới một phần tử không lũy linh gần.

### 4. Nghịch đảo

Cho A là một đại số Banach có đơn vị, mà phần tử đơn vị được ký hiệu bởi 1. Nhắc lại (TG, IX, mệnh đề 14, p. 40) rằng nhóm G các phần tử khả nghịch của A là một tập con mở của A, rằng tôpô cảm sinh trên G bởi tôpô của A là tương thích với cấu trúc nhóm và rằng nhóm tôpô G là đầy đủ.

#### Mệnh đề 2 {#ts-i-s2-prop-2 .statement tag=0264}

Cho A là một đại số Banach và $x$ là một phần tử của A. Chuỗi $\sum_{n=1}^{\infty}\lambda^nx^n$, được xét như một chuỗi lũy thừa theo $\lambda$, có bán kính hội tụ $\varrho (x)^{-1}$. Nếu A có đơn vị và nếu $\varrho (x)<1$, thì $1-x$ là khả nghịch và có nghịch đảo là $\sum_{n=0}^{\infty}x^n$.

Chuỗi $\sum^{\infty}_{n=1}\lambda^nx^n$ có bán kính hội tụ

(lim sup$_{n\rightarrow+\infty}\|x^n\|^{1/n}$)$^{-1}=\varrho (x)^{-1}$

(xem VAR, R1, p. 23, 3.1.4). Giả sử rằng A nhận một phần tử đơn vị. Nếu $\varrho (x)<1$, chuỗi $\sum_{n=0}^{\infty}x^n$ do đó hội tụ tuyệt đối. Vì

$$
(1-x)(\sum_{n=0}^kx^n)=(\sum_{n=0}^kx^n)(1-x) = 1-x^{k+1}
$$

với mọi số nguyên $k\geqslant 0$, phần tử $1-x$ là khả nghịch và nghịch đảo của nó bằng $\sum_{n=0}^{\infty}x^n$.

#### Hệ quả 1 {#ts-i-s2-prop-2-cor-1 .statement tag=0265}

Nếu A là một đại số Banach có đơn vị, thì nhóm các phần tử khả nghịch của A chứa quả cầu mở tâm 1 và bán kính 1.

Điều này ngay lập tức vì $\|x\|<1$ kéo theo $\varrho (x)<1$.

#### Hệ quả 2 {#ts-i-s2-prop-2-cor-2 .statement tag=0266}

Cho A là một đại số Banach và I là một iđêan trái cực đại chính quy (tương ứng iđêan phải) của A. Khi đó I là đóng.

Cho $(\widetilde{A}, e)$ là đại số Banach có đơn vị suy ra từ A bằng phép nối một phần tử đơn vị. Tồn tại một iđêan trái cực đại (tương ứng phải) J của $\widetilde{A}$ sao cho $J\cap A = I$ (A, VIII, p. 428, mệnh đề 4). Khi đó J rời nhau với quả cầu mở tâm $e$ và bán kính 1 (hệ quả 1), và do đó $\overline{J}\not=\widetilde{A}$. Vì J là một iđêan cực đại, điều này suy ra $\overline{J}= J$, và do đó $I = J\cap A =\overline{J}\cap A$ là đóng trong A.

#### Hệ quả 3 {#ts-i-s2-prop-2-cor-3 .statement tag=0267}

Căn của một đại số Banach là đóng.

Thật vậy, căn là giao của các iđêan trái cực đại chính quy (A, VIII, p. 430, Định nghĩa 3).

#### Mệnh đề 3 {#ts-i-s2-prop-3 .statement tag=0268}

Cho A là một đại số Banach có đơn vị.

a) Nếu $x\in A$ có một nghịch đảo trái (tương ứng phải) $y$, thì mọi phần tử $x'\in A$ sao cho $\|x'-x\|<\|y\|^{-1}$ đều có một nghịch đảo trái (tương ứng phải).

b) Tập hợp các phần tử của A khả nghịch (tương ứng trái, tương ứng phải) là mở trong A.

c) Cho $(x_n)$ là một dãy các phần tử của A có các nghịch đảo trái (tương ứng phải)$y_n$, và hội tụ đến một phần tử $x\in A$. Nếu dãy $(y_n)$ bị chặn, thì x khả nghịch trái (tương ứng phải).

Chỉ cần xét trường hợp các nghịch đảo trái; trường hợp các nghịch đảo phải suy ra bằng cách xét đại số đối.

Cho $x, y, x'\in A$ sao cho $yx= 1$ và $\|x'-x\|<\|y\|^{-1}$. Ta có

$$
\|1-yx'\|=\|yx-yx'\|\leqslant \|y\| \cdot  \|x-x'\|<1
$$

do đó $yx'$ khả nghịch: tồn tại $z\in$ A sao cho $z(yx') = 1$. Vậy phần tử $x'$ khả nghịch trái với nghịch đảo $zy$. Điều này chứng minh mệnh đề a) và mệnh đề b) suy ra ngay lập tức từ đó.

Cho $(x_n)$ là một dãy các phần tử của A có các nghịch đảo trái $y_n$, hội tụ đến một phần tử $x\in$ A, và sao cho dãy $(y_n)$ bị chặn. Nếu $M\geqslant 1$ là một số thực sao cho $\|y_n\|\leqslant M$ với mọi $n\geqslant 1$, thì ta có $\|x_n-x\|<M^{-1}\leqslant \|y_n\|^{-1}$ với n đủ lớn, và do đó x có một nghịch đảo trái theo a).

#### Định nghĩa 4 {#ts-i-s2-def-4 .statement tag=0269}

Cho A là một đại số chuẩn, cho $x$ là một phần tử của A. Ký hiệu $\boldsymbol{\gamma }_x$ và $\boldsymbol{\delta }_x$ là các ánh xạ $y\mapsto xy$ và $y\mapsto yx$ từ A vào A. Ta nói rằng x là một ước của không tôpô bên trái (tương ứng phải) nếu $\boldsymbol{\gamma }_x($tương ứng $\boldsymbol{\delta }_x)$ không phải là một đồng phôi của A lên $\boldsymbol{\gamma }_x(A)$ (tương ứng lên $\boldsymbol{\delta }_x(A)$).

#### Nhận xét {#ts-i-s2-n4-rem-1 .statement tag=026A}

Theo TG, IX, p. 36, hệ quả $2,x$ là một ước của không tôpô bên trái (tương ứng phải) khi và chỉ khi tồn tại một dãy $(z_n)$ trong A sao cho $\|z_n\|= 1$ và sao cho $xz_n$ tiến tới 0 (tương ứng $z_nx$ tiến tới 0) khi $n\rightarrow +\infty$.

Một ước của không bên trái (tương ứng phải) là một ước của không tôpô bên trái (tương ứng phải). Giả sử A khác không và có đơn vị. Một ước của không tôpô bên trái (tương ứng phải) x không khả nghịch trái (tương ứng phải). Thật vậy, chẳng hạn nếu $yx= 1$ và nếu $xz_n$ tiến tới 0, thì $z_n=y(xz_n)$ tiến tới 0 và không thể có $\|z_n\|= 1$ với mọi n.

#### Mệnh đề 4 {#ts-i-s2-prop-4 .statement tag=026B}

Let A là một đại số Banach có đơn vị. Cho $x$ là một phần tử của A không khả nghịch trái. Nếu tồn tại một dãy $(x_n)$ các phần tử khả nghịch trái của A hội tụ đến $x$, thì $x$ là một ước của không phải tôpô phải.

Cho $y_n$ là một nghịch đảo trái của $x_n$. Theo Mệnh đề 3 (ii), $\|y_n\|$ tiến tới $+\infty$. Đặt $z_n=\|y_n\|^{-1}y_n$. Ta có $\|z_n\|= 1$, và $z_nx_n=\|y_n\|^{-1}$ tiến tới 0, do đó $z_nx=z_nx_n+z_n(x-x_n)$ tiến tới 0. Khi đó, theo nhận xét sau Định nghĩa 4, ta có kết luận.

#### Mệnh đề 5 {#ts-i-s2-prop-5 .statement tag=026C}

Cho A là một đại số Banach có đơn vị và B là một đại số con đầy đủ của A. Khi đó B là một đại số con đầy đủ của A.

Thật vậy, cho $x$ là một phần tử của $\overline{B}$ khả nghịch trong A, và $(x_n)$ là một dãy các phần tử của B tiến tới $x$. Khi $n$ đủ lớn, $x_n$ khả nghịch trong A và $x^{-1}_n$ tiến tới $x^{-1}$. Vì đại số con B là đầy đủ, ta có $x^{-1}_n\in B$, do đó $x^{-1}\in \overline{B}$.

Cho A là một đại số Banach có đơn vị và $(y_i)_{i\in I}$ là một họ các phần tử của A. Cho B là đại số con đầy đủ của A sinh bởi các phần tử $y_i$. Khi đó $\overline{B}$ là đại số con đầy đủ đóng nhỏ nhất của A chứa các $y_i$. Nó được gọi là đại số con đầy đủ đóng sinh bởi các phần tử $y_i$.

### 5. Phổ của một phần tử trong một đại số định chuẩn

Trong số này, giả sử rằng $K =\mathbf{C}$.

#### Định lý 1 {#ts-i-s2-thm-1 .statement tag=026D}

Cho A là một đại số Banach có đơn vị và $x\in A$.

a) Tập hợp Sp$_A(x)$ là một tập con compact của $\mathbf{C}$;

b) bán kính phổ $\varrho (x)$ là bán kính của đĩa đóng nhỏ nhất có tâm 0 trong $\mathbf{C}$ chứa Sp$_A(x)$ ;

c) giải thức $\lambda \mapsto R(x, \lambda ) = (\lambda -x)^{-1}$ của $x$ là hàm chỉnh hình trong $\mathbf{C}-$ Sp$_A(x)$ và bằng không tại vô cực. Hơn nữa, với mọi số nguyên $k\geqslant 0$, ta có công thức

$\frac{\partial^k}{\partial \lambda^k}R(x, \lambda ) = (-1)^kk$! $R(x, \lambda )^{k+1}$;

d) Với mọi số phức $\lambda$ sao cho $|\lambda |>1/\varrho (x)$, ta có

$$
R(x, \lambda ) =\sum_{n=0}^{+\infty}\lambda^{-n-1}x^n
$$

Phần bù của phổ Sp$_A(x)$ là ảnh ngược của nhóm G gồm các phần tử khả nghịch của A qua ánh xạ liên tục $\lambda \mapsto$ $x-\lambda$ từ $\mathbf{C}$ vào A; theo Mệnh đề 3, b) của I, p. 23, phổ Sp$_A(x)$ là một tập con đóng của $\mathbf{C}$. Mặt khác, cho $\lambda \in \mathbf{C}$ sao cho $|\lambda |> \varrho (x)$. Ta có $\lambda -x=\lambda (1-\lambda^{-1}x)$. Vì $\varrho (\lambda^{-1}x) =|\lambda |^{-1}\varrho (x)<1$, phần tử $1-\lambda^{-1}x$, và do đó cả phần tử $\lambda -x$, đều khả nghịch và

$$
R(x, \lambda ) = (\lambda -x)^{-1}=\sum_{n=0}^{\infty}\lambda^{-n-1}x^n \tag{5}
$$

(I, p. 22, Mệnh đề 2). Đặc biệt, $\lambda \notin$ Sp$_A(x)$. Điều này chứng tỏ rằng Sp$_A(x)$ được chứa trong đĩa có tâm 0 và bán kính $\varrho (x)$. Do đó Sp$_A(x)$ là compact. Công thức (5) này cũng chứng tỏ rằng giải thức của $x$ được xác định và chỉnh hình trong phần bù của đĩa đóng $\Delta_{\varrho(x)}$ có tâm 0 và bán kính $\varrho (x)$, và tiến tới 0 tại vô cực.

Cho $\lambda_0\in \mathbf{C}-$ Sp$_A(x)$. Đặt $y=\lambda_0-x$. Cho $\mu\in \mathbf{C}$ sao cho $|\lambda_0-\mu|<\|y^{-1}\|^{-1}$. Ta có

$$
\mu-x=y-(\lambda_0-\mu) =y(1-(\lambda_0-\mu)y^{-1})
$$

do đó $\mu-x$ khả nghịch và có nghịch đảo

$$
(\mu-x)^{-1}=y^{-1}\sum_{n=0}^{\infty}(\lambda_0-\mu)^ny^{-n} \tag{6}
$$

theo Mệnh đề 2 của I, p. 22. Do đó giải thức của $x$ được xác định và chỉnh hình trong đĩa mở có tâm $\lambda_0$ và bán kính $\|y^{-1}\|^{-1}$. Suy ra giải thức của $x$ là một ánh xạ chỉnh hình của $\mathbf{C}-$ Sp$_A(x)$ vào A.

Công thức (1) của I, p. 4 suy ra $\frac{\partial}{\partial \lambda}R(x, \lambda ) =-R(x, \lambda )^2$, do đó, bằng quy nạp theo $k$,

$\frac{\partial^k}{\partial \lambda^k}R(x, \lambda ) = (-1)^kk$! $R(x, \lambda )^{k+1}$.

Cho $a >0$ là một số thực sao cho Sp$_A(x)$ được chứa trong đĩa đóng $\Delta_a$ có tâm 0 và bán kính $a$. Khi đó hàm $\lambda \mapsto (\lambda^{-1}-x)^{-1}$ được xác định và chỉnh hình với $0<|\lambda |< a^{-1}$ và tiến tới 0 khi $\lambda$ tiến tới 0. Hàm liên tục duy nhất trên đĩa mở có tâm 0 và bán kính $a^{-1}$ mở rộng hàm chỉnh hình này khi đó là chỉnh hình (VAR, R1, 3.3.9), do đó bán kính hội tụ của chuỗi (5) xác định nó là $\geqslant a^{-1}$ (VAR, R1, 3.2.9). Theo Mệnh đề 2 của I, p. 22, do đó ta có $a\geqslant \varrho (x)$.

#### Nhận xét 1 {#ts-i-s2-n5-rem-1 .statement tag=026E}

Phổ của một phần tử trong một đại số Banach có đơn vị có thể là bất kỳ tập con compact khác rỗng F nào của $\mathbf{C}$(xem Ví dụ 3 của I, p. 17; với $A =\mathscr{C}(F;\mathbf{C})$ và $f\in A$ là đơn ánh chính tắc của F vào $\mathbf{C}$, ta có Sp$_A(f) = F$).

#### Nhận xét 2 {#ts-i-s2-n5-rem-2 .statement tag=026F}

Cho A là một đại số Banach có đơn vị và $x\in A$. Theo Định lý 1 của I, p. 24$,\mathbf{C}-$ Sp$_A(x)$ là một tập con mở của $\mathbf{C}$, do đó liên thông địa phương. Vì vậy các thành phần liên thông của $\mathbf{C}-$ Sp$_A(x)$ là mở. Theo Định lý 1, một trong các thành phần liên thông này chứa tập hợp các $\lambda \in \mathbf{C}$ sao cho $|\lambda |> \varrho (x)$; do đó tất cả các thành phần liên thông khác đều bị chặn.

#### Hệ quả 1 {#ts-i-s2-thm-1-cor-1 .statement tag=026G}

Cho A là một đại số định chuẩn có đơn vị và khác không. Với mọi $x\in A$, phổ Sp$_A(x)$ là khác rỗng.

Trước hết, giả sử A đầy đủ. Nếu Sp($x$) $=\emptyset$, thì giải thức của $x$ sẽ chỉnh hình trên $\mathbf{C}$ và bằng không tại vô cực, do đó đồng nhất bằng không (VAR, R., 3.3.6, p. 29). Vì $R(x, \lambda ) = (\lambda -x)^{-1}$ khả nghịch, suy ra 1 = 0 và do đó $A =\{0\}$.

Trong trường hợp tổng quát, cho $\widehat{A}$ là đại số hoàn chỉnh của A; quan hệ Sp$_A(x) =\emptyset$ sẽ kéo theo Sp$_{\widehat{A}}(x) =\emptyset$, do đó $\widehat{A} =\{0\}$ và $A =\{0\}$.

#### Hệ quả 2 (Định lý Gelfand-Mazur) {#ts-i-s2-thm-1-cor-2 .statement tag=026H}

Cho A là một đại số có chuẩn trên $\mathbf{C}$. Nếu A là một trường, thì $A =\mathbf{C}\cdot 1$.

Nếu $x\in A$, tồn tại $\lambda \in \mathbf{C}$ sao cho $x-\lambda$ không khả nghịch (hệ quả 1), do đó $x-\lambda = 0$ và $x\in \mathbf{C}\cdot 1$.

#### Hệ quả 3 {#ts-i-s2-thm-1-cor-3 .statement tag=026I}

Cho A là một đại số Banach có đơn vị và $x$ là một phần tử khả nghịch của A sao cho $\|x\|=\|x^{-1}\|= 1$. Khi đó Sp($x$)$\subset \mathbf{U}$.

Cho Δ là đĩa có tâm 0 và bán kính 1 trong $\mathbf{C}$. Theo định lý 1 b) và sự kiện rằng $\varrho (x)\leqslant \|x\|$, ta có Sp($x$)$\subset \Delta$. Tương tự, Sp($x$)$^{-1}$ = Sp($x^{-1}$)$\subset \Delta$, do đó có hệ quả (xem I, p. 2, nhận xét 4).

#### Hệ quả 4 {#ts-i-s2-thm-1-cor-4 .statement tag=026J}

Cho E là một không gian Banach phức, $\mathscr{L}(E)$ là đại số Banach của các tự đồng cấu liên tục của E và A là một đại số con khác không của $\mathscr{L}(E)$ sao cho E là một giả môđun A đơn (A, II, p. 176, Phụ lục).

a) Cho $u$ là một tự đồng cấu của E, không nhất thiết liên tục, giao hoán với A. Khi đó $u$ là một phép vị tự;

b) Cho $u$ là một tự đồng cấu của E, không nhất thiết liên tục. Với mọi số nguyên $n\geqslant 1$ và mọi $(\xi_1, . . . , \xi_n)\in E^n$, tồn tại $v\in A$ sao cho

$$
(v(\xi_1), . . . , v(\xi_n)) = (u(\xi_1), . . . , u(\xi_n))
$$

Ta chứng minh a). Cho $\widetilde{A}$ là đại số thu được từ A bằng phép nối một phần tử đơn vị. Vì E là một giả môđun A đơn, nên nó là một $\widetilde{A}$-môđun đơn.

Cho B là hoán tập của $\widetilde{A}$ trong vành các tự đồng cấu của không gian vectơ $\mathbf{C}$-E. Đại số B chứa 1 và là đại số tự đồng cấu của $\widetilde{A}$-môđun E. Vì E là một $\widetilde{A}$-môđun đơn, Bổ đề Schur (A, VIII, p. 43, hệ quả) chỉ ra rằng B là một trường.

Cho $\xi_0\in E$ sao cho $A\xi_0\not=\{0\}$. Do đó ta có $A\xi_0= E$. Với mọi $u\in B$, cho $A_u$ là tập hợp các $v\in A$ sao cho $v(\xi_0) =u(\xi_0)$. Tập hợp này là khác rỗng, vì $A\xi_0= E$. Khi đó đặt

$\|u\|_B=$ inf$_{v\in A_u}\|v\|$.

Ánh xạ $u\mapsto  \|u\|_B$ là một bán chuẩn trên B.

Hãy chứng minh rằng ánh xạ này là một chuẩn. Cho $u$ là một phần tử khác không của B. Với mọi $v\in A_u$, ta có $\|v\|\geqslant \|v(\xi_0)\|/\|\xi_0\|=\|u(\xi_0)\|/\|\xi_0\|$, do đó $\|u\|_B\geqslant \|u(\xi_0)\|/\|\xi_0\|$. Vì vậy, chỉ cần chứng minh rằng $u(\xi_0)\not= 0$. Cho $\xi_1\in E$ sao cho $u(\xi_1)\not= 0$. Vì $A\xi_0= E$, tồn tại $w\in A$ sao cho $\xi_1=w(\xi_0)$. Khi đó $wu(\xi_0) =uw(\xi_0) =u(\xi_1)\not= 0$, do đó $u(\xi_0)\not= 0$.

Mặt khác, cho $u$ và $u'$ là các phần tử của B. Với mọi $\varepsilon  >0$, tồn tại $v, v'\in A$ sao cho $v(\xi_0) =u(\xi_0),v'(\xi_0) =u'(\xi_0)$ và $\|v\|\leqslant \|u\|_B+\varepsilon$, $\|v'\|\leqslant \|u'\|_B+\varepsilon$. Khi đó ta có $vv'(\xi_0) =vu'(\xi_0) =u'v(\xi_0) =u'u(\xi_0)$, do đó

$$
\|u'u\|_B\leqslant \|v'v\|\leqslant \|v\|\|v'\|\leqslant (\|u\|_B+\varepsilon )(\|u'\|_B+\varepsilon )
$$

và cuối cùng $\|u'u\|_B\leqslant \|u\|_B\|u'\|_B$. Điều này chứng tỏ rằng B, được trang bị chuẩn $u\mapsto  \|u\|_B$, là một đại số chuẩn. Vì nó là một trường, hệ quả 2 suy ra rằng $B =\mathbf{C}\cdot 1$, đó là kết luận cần chứng minh.

Hãy chứng minh b). Theo a), hoán tập của A trong End$_{\mathbf{C}}(E)$ thu gọn vào các phép vị tự của E. Do đó đối giao hoán tử kép của nó là End$_{\mathbf{C}}(E)$. Mệnh đề b) do đó là hệ quả của định lý mật độ của Jacobson (định lý 1 của A, VIII, p. 434).

#### Hệ quả 5 {#ts-i-s2-thm-1-cor-5 .statement tag=026K}

Cho A là một đại số Banach và $x\in A$.

a) Sp$'(x)$ là một tập con compact của $\mathbf{C}$;

b) Bán kính phổ $\varrho (x)$ là bán kính của đĩa đóng nhỏ nhất có tâm 0 trong $\mathbf{C}$ chứa Sp$'(x)$;

c) Để $x$ là lũy linh, điều kiện cần và đủ là Sp$'(x) =\{0\}$.

Các mệnh đề a) và b) suy ra từ định lý 1 bằng cách xét đại số Banach suy ra từ A nhờ phép nối một phần tử đơn vị. Mệnh đề c) suy ra từ b).

### 6. Phổ tương đối với một đại số con

Trong No. này, giả thiết rằng $K =\mathbf{C}$.

#### Bổ đề 3 {#ts-i-s2-lem-3 .statement tag=026L}

Cho $X_1$ và $X_2$ là các tập con compact của $\mathbf{C}$. Nếu $X_2$ được chứa trong $X_1$ và nếu biên của $X_1$ trong $\mathbf{C}$ được chứa trong $X_2$, thì $X_1$ là hợp của $X_2$ và một số thành phần liên thông bị chặn của phần bù của $X_2$ trong $\mathbf{C}$.

Cho U là một thành phần liên thông của $\mathbf{C}-X_2$. Mọi điểm biên của $X_1\cap U$ trong tập mở U cũng là một điểm biên của $X_1$ trong $\mathbf{C}$, do đó thuộc $X_2$ theo giả thiết; vì $U\cap X_2=\emptyset$, ta thấy rằng $X_1\cap U$ không có điểm biên nào trong không gian U. Vì U liên thông, giao $X_1\cap U$ hoặc rỗng hoặc bằng U (TG, I, p. 82, cor.), và bổ đề được suy ra.

#### Mệnh đề 6 {#ts-i-s2-prop-6 .statement tag=026M}

Cho A là một đại số Banach có đơn vị và B là một đại số con đóng có đơn vị của A. Với mọi $x\in B$, ta có Sp$_B(x)\supset$ Sp$_A(x)$, và biên của Sp$_A(x)$ trong $\mathbf{C}$ chứa biên của Sp$_B(x)$ trong $\mathbf{C}$. Đặc biệt, nếu Sp$_B(x)\subset \mathbf{R}$, thì ta có Sp$_B(x) =$ Sp$_A(x)$.

Ta có Sp$_B(x)\supset$ Sp$_A(x)$ (nhận xét 6 của I, p. 3). Nếu $\lambda$ là một điểm thuộc biên của Sp$_B(x)$ trong $\mathbf{C}$, tồn tại một dãy $(\lambda_n)$ các điểm nằm ngoài Sp$_B(x)$ hội tụ đến $\lambda$. Khi đó $x-\lambda_n$ khả nghịch trong B và hội tụ đến $x-\lambda$, là phần tử không khả nghịch trong B; do đó $x-\lambda$ là một ước của không tôpô trái hoặc phải trong B (Mệnh đề 4 của I, p. 24), nên cũng trong A. Vậy $\lambda \in$ Sp$_A(x)$. Nhưng vì Sp$_A(x)\subset$ Sp$_B(x)$, số phức $\lambda \in$ Fr$_{\mathbf{C}}$(Sp$_B(x)$) không thể là điểm trong của Sp$_A(x)$, và do đó thuộc biên của nó.

#### Hệ quả {#ts-i-s2-n6-cor-1 .statement tag=026N}

Tập hợp Sp$_B(x)$ là hợp của Sp$_A(x)$ và một số thành phần liên thông bị chặn của $\mathbf{C}-$ Sp$_A(x)$.

Điều này suy ra từ Mệnh đề 6 và Bổ đề 3.

Hệ quả này sẽ được hoàn thiện bởi các Mệnh đề 13 của I, p. 46 và 14 của I, p. 46.

## BÀI TẬP {#ts-i-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
