---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 2
section_title: The Structure of Modules of Finite Length
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.25-A VIII.43
pdf_pages: 0042-0060
extraction: native
subsections:
    - "no": 1
      title: Local Rings
      page: 25
      pdf_page: 42
    - "no": 2
      title: Weyr–Fitting Decomposition
      page: 27
      pdf_page: 44
    - "no": 3
      title: Indecomposable Modules and Primordial Modules
      page: 30
      pdf_page: 47
    - "no": 4
      title: Semiprimordial Modules
      page: 32
      pdf_page: 49
    - "no": 5
      title: The Structure of Modules of Finite Length
      page: 37
      pdf_page: 54
statements: 37
exercises: 20
content_sha256: d7776ec35d5d611c5699dde0b1cfa2c51b9995125e0b3952b18824dc2cdd6619
translated_from: content/en/alg/VIII/02_s2_the_structure_of_modules_of_finite.md
source_content_sha256: 937d6660bbf18635e63c4c1addfaf3e44ee88a5456fdc47cb5c2eacabc9099b5
translation_model: gpt-5-6, gpt-5-mini, gpt-5.4
translation_run: translate-vi-d30757fd
glossary_version: 34
glossary_terms_sha256: 0b375e7b70e79ed8ef7734aeeed55aa643d09d6e3e6cc2cefc88772f9f7e88e5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CẤU TRÚC CỦA CÁC MÔĐUN CÓ ĐỘ DÀI HỮU HẠN

### 1. Các vành địa phương

#### Mệnh đề 1 {#alg-viii-s2-prop-1 .statement tag=001P}

Cho A là một vành khác không, và $\mathfrak{r}$ là tập hợp các phần tử không khả nghịch của A. Các tính chất sau là tương đương:

(i) Tập hợp $\mathfrak{r}$ là một iđêan hai phía của A.

(ii) Tập hợp $\mathfrak{r}$ ổn định đối với phép cộng.

(iii) Vành A có duy nhất một iđêan trái cực đại.

(iv) Với mọi $a\in A$, một trong hai phần tử $a$ và $1-a$ là khả nghịch.

(v) Với mọi $a\in A$, một trong hai phần tử $a$ và $1-a$ là khả nghịch trái.

Hàm ý (i) $\Rightarrow$ (ii) suy ra từ định nghĩa của một iđêan. Vì 1 không thuộc $\mathfrak{r}$, ta có (ii) $\Rightarrow$ (iv).

Ta có $\mathfrak{r}\not= A$, và tập hợp $\mathfrak{r}$ chứa mọi iđêan trái của A khác A. Nếu $\mathfrak{r}$ là một iđêan trái của A, thì do đó nó là iđêan trái cực đại duy nhất của A. Điều này chứng minh rằng (i) kéo theo (iii).

Giả sử rằng A có một iđêan trái cực đại duy nhất $\mathfrak{m}$. Lấy $b\in A-\mathfrak{m}$. Iđêan trái $Ab$ không được chứa trong bất kỳ iđêan trái cực đại nào của A, do đó bằng A (I, §8, No. 6, p. 104, định lý 1), và $b$ là khả nghịch trái. Với mọi $a\in A$, một trong các phần tử $a$ và $1-a$ thuộc A $-\mathfrak{m}$ vì $\mathfrak{m}$ là một iđêan không chứa 1. Vậy, (iii) suy ra (v).

Giả sử tính chất (v) đúng. Cho $b$ là một phần tử khả nghịch trái của A. Cho $c\in A$ sao cho $cb= 1$. Ta có $(1-bc)b= 0$ và $b\not= 0$; do đó, $1-bc$ không khả nghịch trái. Theo tính chất (v), $bc$ khả nghịch trái và, a fortiori, $c$ khả nghịch trái. Nhưng khi đó $c$ khả nghịch; $b$ là nghịch đảo của nó, vậy $b$ khả nghịch. Suy ra (v) kéo theo (iv).

Còn lại phải chứng minh rằng (iv) kéo theo (i). Giả sử (iv) đúng. Khi đó $\mathfrak{r}$ là một iđêan hai phía của A theo các khẳng định a) đến d) sau:

a) Ta có $0\in \mathfrak{r}$ vì vành A là khác không.

b) Tích của hai phần tử của A, một phần tử thuộc $\mathfrak{r}$ và phần tử kia thuộc A $-\mathfrak{r}$, thuộc $\mathfrak{r}$.

c) Tập hợp $\mathfrak{r}$ ổn định dưới phép cộng.

Thật vậy, cho $a$ và $b$ là các phần tử của $\mathfrak{r}$ sao cho $s=a+b$ khả nghịch. Theo b), các phần tử $s^{-1}a$ và $s^{-1}b$ của A thuộc $\mathfrak{r}$; vì $s^{-1}b= 1-s^{-1}a$, điều này mâu thuẫn với giả thiết rằng (iv) đúng.

d) Tập hợp $\mathfrak{r}$ ổn định dưới phép nhân.

Thật vậy, cho $a$ và $b$ là hai phần tử của $\mathfrak{r}$. Phần tử $a'=-a(1-b)$ thuộc $\mathfrak{r}$ theo b), do đó phần tử $ab$, bằng $a+a'$, thuộc $\mathfrak{r}$ theo c); mệnh đề d) được suy ra.

#### Định nghĩa 1 {#alg-viii-s2-def-1 .statement tag=001Q}

Một vành địa phương là một vành khác không có các tính chất tương đương của Mệnh đề 1.

Một vành A là địa phương khi và chỉ khi vành đối $A^o$ là địa phương.

Nếu A là một vành địa phương, thì tập hợp $\mathfrak{r}$ các phần tử không khả nghịch của A là một iđêan hai phía của A; nó chứa mọi iđêan trái hoặc phải của A khác A. Do đó vành $A/\mathfrak{r}$ là một trường, mà ta gọi là trường thặng dư của A. Tập hợp $\mathfrak{r}$ là iđêan duy nhất cực đại trái (tương ứng, phải, hai phía của A); ta nói đơn giản rằng $\mathfrak{r}$ là iđêan cực đại của A.

#### Ví dụ 1 {#alg-viii-s2-n1-exa-1 .statement tag=001R}

Mọi trường đều là một vành địa phương.

#### Ví dụ 2 {#alg-viii-s2-n1-exa-2 .statement tag=001S}

Cho A là một vành khác không trong đó mọi phần tử đều khả nghịch hoặc lũy linh. Khi đó A là một vành địa phương. Thật vậy, nếu $a\in A$ không khả nghịch, thì theo giả thiết, tồn tại một số nguyên $n\geqslant 0$ sao cho $a^{n+1}= 0$, và $1-a$ có nghịch đảo $1 +a+\cdots +a^n$.

#### Ví dụ 3 {#alg-viii-s2-n1-exa-3 .statement tag=001T}

Cho X là một đa tạp $C^r$ (VAR, R, 5.1.5) và $x$ là một điểm của X. Gọi $\mathscr{O}_x$ là vành các mầm tại $x$ của các hàm $C^r$ nhận giá trị trong trường vô hướng K. Khi đó $\mathscr{O}_x$ là một vành địa phương giao hoán, và iđêan cực đại của nó gồm các

mầm của những hàm bằng không tại $x.*$

#### Ví dụ 4 {#alg-viii-s2-n1-exa-4 .statement tag=001U}

Cho A là một vành địa phương giao hoán và $B = A[[X_i]]_{i\in I}$ là một đại số các chuỗi lũy thừa hình thức với hệ số trong A (III, §2, No. 11, p. 456). Theo Mệnh đề 6 của IV, §4, No. 4, p. 30, vành B là địa phương, và iđêan cực đại của nó gồm các chuỗi lũy thừa hình thức có số hạng hằng thuộc iđêan cực đại của A. Đặc biệt, nếu A là một trường, thì iđêan cực đại của $A[[X_i]]_{i\in I}$ gồm các chuỗi lũy thừa hình thức có số hạng hằng bằng không.

#### Ví dụ 5 {#alg-viii-s2-n1-exa-5 .statement tag=001V}

Cho $p$ là một số nguyên tố. Ta ký hiệu bởi $\mathbf{Z}_{(p)}$ vành con của trường $\mathbf{Q}$ của các số hữu tỉ gồm các phân thức $a/b$ với $a\in \mathbf{Z},b\in \mathbf{Z}$, và $b$ không chia hết cho $p*$(xem Comm. Alg., II, §2, No. 1, p. 60). Khi đó $\mathbf{Z}$ là

$*(_{p)}$

một vành địa phương giao hoán, với iđêan cực đại $p\mathbf{Z}_{(p)}$. Vành $\mathbf{Z}_p$ của các số nguyên $p$-adic (V, §12, No. 3, p. 96) là một vành địa phương giao hoán, với iđêan cực đại $p\mathbf{Z}_p$ (VIII, p. 40, Bài tập 9).

#### Ví dụ 6 {#alg-viii-s2-n1-exa-6 .statement tag=001W}

Cho K là một trường giao hoán có đặc số $p >0$ và G là một $p$-nhóm (I, §6, No. 5, p. 76, Định nghĩa 9). Đại số K[G] của nhóm G trên K (III, §2, No. 6, p. 446) là một vành địa phương; iđêan cực đại của nó là tập hợp các phần tử $(a_g)_{g\in G}$ của K[G] sao cho $\sum_{g\in G}a_g= 0$ (VIII, p. 41, Bài tập 10).

### 2. Phân rã Weyr–Fitting

Cho A là một vành, M là một A-môđun, và $u$ là một tự đồng cấu của M. Với mọi số nguyên $p\geqslant 0$, ta ký hiệu hạt nhân của $u^p$ bởi $N_p$. Dãy các môđun con $(N_p)$ là tăng, và hợp của chúng là một môđun con $N_{\infty}$ của M ổn định dưới $u$. Với mọi số nguyên $p\geqslant 0$, ta có $N_{p+1}=\overset{-1}{u}(N_p)$, và quan hệ $N_p= N_{p+1}$ do đó kéo theo $N_{p+1}= N_{p+2}$. Do đó, hoặc dãy $(N_p)$ là tăng ngặt, hoặc tồn tại một số nguyên $p\geqslant 0$ sao cho $N_0, . . . ,N_p$ phân biệt và $N_p= N_{\infty}$.

Với mọi số nguyên $q\geqslant 0$, ký hiệu ảnh của $u^q$ là $I_q$. Dãy các môđun con $(I_q)$ là giảm, và giao của chúng là một môđun con $I_{\infty}$ của M ổn định dưới $u$. Với mọi số nguyên $q\geqslant 0$, ta có $u(I_q) = I_{q+1}$, và do đó quan hệ $I_q= I_{q+1}$ kéo theo $I_{q+1}= I_{q+2}$. Do đó, hoặc dãy $(I_q)$ giảm nghiêm ngặt, hoặc tồn tại một số nguyên $q\geqslant 0$ sao cho $I_0, . . . ,I_q$ phân biệt và $I_q= I_{\infty}$.

#### Mệnh đề 2 {#alg-viii-s2-prop-2 .statement tag=001X}

a) Giả sử dãy $(N_p)$ là dừng. Khi đó ta có $N_{\infty}\cap I_{\infty}= 0$, hạn chế của $u$ trên $I_{\infty}$ là đơn ánh, và $u$ cảm sinh một tự đồng cấu lũy linh của $N_{\infty}$.

b) Giả sử dãy $(I_p)$ là dừng. Khi đó ta có M = $N_{\infty}+ I_{\infty}$ và $u(I_{\infty}) = I_{\infty}$.

c) (“Phân rã Weyr–Fitting” đôi khi được gọi là “phân rã Fitting”) Giả sử rằng các dãy $(N_p)$ và $(I_p)$ là dừng. Khi đó M là tổng trực tiếp của các môđun con $N_{\infty}$ và $I_{\infty}$ ổn định dưới $u$, và $u$ cảm sinh một tự đồng cấu lũy linh trên $N_{\infty}$ và một tự đẳng cấu trên $I_{\infty}$.

Cho $p$ là một số tự nhiên sao cho $N_p= N_{\infty}$, và đặt $v=u^p$. Theo phép dựng, $v$ và $v^2$ có cùng hạt nhân $N_{\infty}$, và $I_p$ là ảnh của $v$. Với $x$ trong $N_{\infty}\cap I_p$, tồn tại một $y\in M$ sao cho $x=v(y)$ và do đó $v^2(y) =v(x) = 0$; vì thế, ta có $y\in N_{\infty}$ và do đó $x= 0$. Đặc biệt, ta có $N_{\infty}\cap I_{\infty}= 0$. Vì hạt nhân $N_1$ của $u$ được chứa trong $N_{\infty}$, hạn chế của $u$ lên $I_{\infty}$ là đơn ánh; mặt khác, ta có $u^p(N_{\infty}) = 0$. Điều này chứng minh a).

Cho $q$ là một số tự nhiên sao cho $I_q= I_{\infty}$, và đặt $w=u^q$. Khi đó $w$ và $w^2$ có cùng ảnh $I_{\infty}$, và $N_q$ là hạt nhân của $w$. Cho $x\in M$. Ta có $w(x)\in I_{\infty}$, nên tồn tại một $y\in M$ sao cho $w(x) =w^2(y)$; khi đó ta có $x-w(y)\in N_q$, do đó $M = N_q+ I_{\infty}$ và a fortiori $M = N_{\infty}+ I_{\infty}$. Ta có $u(I_{\infty}) =u(I_q) = I_{q+1}= I_{\infty}$. Điều này chứng minh b).

Mệnh đề c) suy ra ngay lập tức từ a) và b).

#### Nhận xét 1 {#alg-viii-s2-n2-rem-1 .statement tag=001Y}

Cho $p$ là một số nguyên sao cho $N_p= N_{p+1}$; chứng minh đã cho ở trên chỉ ra rằng $N_{\infty}\cap I_p= 0$, và hạn chế của $u$ lên $I_p$ là đơn ánh. Tương tự, cho $q$ là một số nguyên sao cho $I_q= I_{q+1}$; khi đó ta có $N_q+ I_{\infty}= M$, và tự đồng cấu của $M/N_q$ suy ra từ $u$ bằng cách chuyển qua thương là toàn ánh.

#### Nhận xét 2 {#alg-viii-s2-n2-rem-2 .statement tag=001Z}

Giả sử rằng M là tổng trực tiếp của hai môđun con N và I ổn định dưới $u$ và rằng $u$ cảm sinh một tự đồng cấu lũy linh $u_N$ của N và một tự đẳng cấu của I. Khi đó ta có $N_{\infty}= N$ và $I_{\infty}= I$, và các dãy $(N_p)$ và $(I_p)$ là dừng. Hơn nữa, các số nguyên sau đây bằng nhau:

$\alpha )$ số nguyên nhỏ nhất $p\geqslant 0$ sao cho $N_p= N_{\infty}$,

$\beta )$ số nguyên nhỏ nhất $q\geqslant 0$ sao cho $I_q= I_{\infty}$,

$\gamma )$ số nguyên nhỏ nhất $r\geqslant 0$ sao cho $(u_N)^r= 0$.

#### Nhận xét 3 {#alg-viii-s2-n2-rem-3 .statement tag=0020}

Giả thiết của mệnh đề a) được thỏa mãn nếu A-môđun M là Noether; giả thiết của mệnh đề b) được thỏa mãn nếu M là Artin; theo Mệnh đề 1 của VIII, p. 2, giả thiết của mệnh đề c) được thỏa mãn nếu M có độ dài hữu hạn.

#### Hệ quả 1 {#alg-viii-s2-prop-2-cor-1 .statement tag=0021}

Cho A là một vành, và cho M là một A-môđun.

a) Nếu môđun M là Noether, thì mọi tự đồng cấu toàn ánh của M đều là song ánh.

b) Nếu môđun M là Artin, thì mọi tự đồng cấu đơn ánh của M đều là song ánh.

c) Nếu môđun M có độ dài hữu hạn, thì mọi tự đồng cấu đơn ánh hoặc toàn ánh của M đều là song ánh.

d) Nếu vành A là giao hoán và A-môđun M sinh hữu hạn, thì mọi tự đồng cấu toàn ánh của M đều là song ánh.

Cho $u$ là một tự đồng cấu của A-môđun M. Ta dùng ký hiệu được đưa vào ở đầu tiểu mục này. Nếu tự đồng cấu $u$ là toàn ánh, thì ta có $I_{\infty}= M$. Khi đó mệnh đề a) suy ra từ Mệnh đề 2, a) và Nhận xét 3. Tương tự, nếu tự đồng cấu $u$ là đơn ánh, thì ta có $N_{\infty}= 0$. Vì vậy mệnh đề b) suy ra từ Mệnh đề 2, b) và Nhận xét 3. Mệnh đề c) suy ra ngay lập tức từ a) và b).

Bây giờ, giả sử rằng vành A là giao hoán, A-môđun M là sinh hữu hạn, và tự đồng cấu $u$ là toàn ánh. Ta sẽ chứng minh rằng $u$ là đơn ánh. Gọi $x$ là một phần tử của M sao cho $u(x) = 0$. Chọn một họ sinh hữu hạn $(x_i)_{i\in I}$ của A-môđun M và, với mọi $i\in I$, một phần tử $y_i$ của M sao cho $u(y_i) =x_i$. Tồn tại các họ $(a_i)_{i\in I}, (b_{ij})_{(i,j)\in I\times I}$, và $(c_{ij})_{(i,j)\in I\times I}$ gồm các phần tử của A sao cho ta có

$$
x=\sum_{i\in I}a_ix_i,y_j=\sum_{i\in I}b_{ij}x_i,u(x_j) =\sum_{i\in I}c_{ij}x_i
$$

với mọi $j\in I$. Gọi $A'$ là một vành con Noether của A chứa các phần tử $a_i,b_{ij}$, và $c_{ij}$ (VIII, p. 12, Hệ quả 3). Gọi $M'$ là môđun con trên $A'$ của M sinh bởi họ $(x_i)_{i\in I}$. Ta có $u(x_j)\in M',y_j\in M'$, và $u(y_j) =x_j$ với mọi $j\in I$; do đó $u$ xác định, bởi hạn chế, một tự đồng cấu toàn ánh $u'$ của $A'$-môđun $M'$. Vì vành $A'$ là Noether, $A'$-môđun sinh hữu hạn $M'$ là Noether (VIII, p. 7, Mệnh đề 4 a)). Theo a), tự đồng cấu $u'$ của $M'$ là song ánh. Theo phép dựng, $x$ thuộc $M'$, và ta có $u'(x) =u(x) = 0$. Vậy nên $x= 0$, điều này chứng minh d).

#### Hệ quả 2 {#alg-viii-s2-prop-2-cor-2 .statement tag=0022}

Trong một vành Noether trái, mọi phần tử khả nghịch trái hoặc phải đều khả nghịch.

Thật vậy, xét các phần tử $x,y$ của một vành Noether trái A sao cho $xy= 1$. Ký hiệu bởi $\boldsymbol{\delta }(x)$ và $\boldsymbol{\delta }(y)$, tương ứng, các tự đồng cấu $a\mapsto ax$ và $a\mapsto ay$ của A-môđun $A_s$. Ta có $\boldsymbol{\delta }(y)\circ \boldsymbol{\delta }(x) = 1_{A_s}$; do đó $\boldsymbol{\delta }(y)$ là toàn ánh. Theo Hệ quả 1, a), $\boldsymbol{\delta }(y)$ là song ánh. Khi đó tự đồng cấu $\boldsymbol{\delta }(x)$ là song ánh ngược của $\boldsymbol{\delta }(y)$, và ta có $yx= (\boldsymbol{\delta }(x)\circ \boldsymbol{\delta }(y))(1) = 1$. Hệ quả được chứng minh.

### 3. Môđun Không Phân Tích Được và Môđun Nguyên Thủy

Cho A là một vành. Nhắc lại định nghĩa sau (VII, §4, No. 8, p. 23, Định nghĩa 3).

#### Định nghĩa 2 {#alg-viii-s2-def-2 .statement tag=0023}

Một A-môđun M được gọi là không phân tích được nếu nó không phải là tổng trực tiếp của một họ các môđun con phân biệt với 0 và M.

Theo hệ quả của Mệnh đề 12 trong II, §1, No. 8, p. 209, các tính chất sau là tương đương:

a) A-môđun M là không phân tích được.

b) A-môđun M khác không, và mọi môđun con hạng tử trực tiếp của M đều bằng 0 hoặc M.

c) A-môđun M khác không, và vành End$_A(M)$ không chứa lũy đẳng nào phân biệt với 0 và $1_M$.

Đặc biệt, vì vành các tự đồng cấu của A-môđun $A_s$ đẳng cấu với vành đối của A, ta thấy rằng A-môđun $A_s$ là không phân tích được khi và chỉ khi vành A khác không và các phần tử lũy đẳng duy nhất của nó là 0 và 1.

#### Ví dụ {#alg-viii-s2-n3-exa-1 .statement tag=0024}

Giả sử rằng vành A là một miền iđêan chính. Các A-môđun sinh hữu hạn không phân tích được là các A-môđun đẳng cấu với hoặc A, hoặc $A/p^nA$, trong đó $p$ là một phần tử bất khả quy của A và $n$ là một số nguyên $>0$ (VII, §4, No. 8, p. 24, Mệnh đề 8).

#### Mệnh đề 3 {#alg-viii-s2-prop-3 .statement tag=0025}

Một A-môđun M Noether hoặc Artin là tổng trực tiếp của một họ hữu hạn các môđun con không phân tích được.

Trước hết ta hãy chứng minh rằng mọi môđun con khác không P của M đều có một môđun con hạng tử trực tiếp không phân tích được. Nếu không phải như vậy, thì mọi môđun con hạng tử trực tiếp của P đều sẽ phân tích được; khi đó, tiến hành bằng quy nạp, ta có thể xây dựng, với mọi $n\in \mathbf{N}$, các môđun con khác không $N'_n$ và $N''_n$ của P sao cho $P = N'_0\oplus N''_0$ và $N'_{n-1}= N'_n\oplus N''_n$ với $n\geqslant 1$. Nhưng khi đó, dãy các môđun con $N''_0+\cdots + N''_n$ sẽ tăng ngặt, còn dãy các môđun con $N'_n$ sẽ giảm nghiêm ngặt. Môđun M sẽ không là Noether cũng không là Artin, trái với giả thiết.

Bây giờ, giả sử rằng M không phải là tổng trực tiếp của một họ hữu hạn các môđun con không phân tích được. Bằng quy nạp, ta xây dựng các môđun con không phân tích được $P''_n$ của M và các môđun con khác không $P'_n$ của M với mọi $n\in \mathbf{N}$ sao cho $M = P'_0\oplus P''_0$ và $P'_{n-1}= P'_n\oplus P''_n$ với $n\geqslant 1$. Thật vậy, M là khác không, và phần đầu của chứng minh, áp dụng cho P = M, cho ta $P'_0$ và $P''_0$. Vì các môđun $P'_k$ và $P''_k$ được xác định với $k < n$, theo phần đầu của chứng minh, tồn tại các môđun con $P'_n$ và $P''_n$ sao cho $P'_{n-1}= P'_n\oplus P''_n$ với $P''_n$ không phân tích được. Khi đó quan hệ $M = P'_n\oplus P''_0\oplus  \cdots  \oplus P''_n$ suy ra rằng $P'_n\not= 0$ vì M không phải là tổng trực tiếp của một họ hữu hạn các môđun không phân tích được.

Dãy các môđun con $P''_0\oplus  \cdots  \oplus P''_n$ là tăng ngặt, và dãy các môđun con $P'_n$ là giảm nghiêm ngặt. Điều này mâu thuẫn với giả thiết rằng M là Noether hoặc Artin.

Vấn đề về tính duy nhất của sự phân tích của một môđun thành tổng trực tiếp của các môđun con không phân tích được sẽ được nghiên cứu trong tiểu mục tiếp theo.

#### Định nghĩa 3 {#alg-viii-s2-def-3 .statement tag=0026}

Một môđun được gọi là nguyên thủy[^1] nếu vành tự đồng cấu của nó là địa phương.

Theo định nghĩa, một vành địa phương không phải chỉ gồm 0; do đó, một môđun nguyên thủy là khác không. Hơn nữa, A-môđun $A_s$ là nguyên thủy khi và chỉ khi vành A là địa phương.

#### Mệnh đề 4 {#alg-viii-s2-prop-4 .statement tag=0027}

a) Một môđun nguyên thủy là không phân tích được.

b) Một môđun không phân tích được có độ dài hữu hạn là nguyên thủy.

Cho M là một A-môđun. Giả sử rằng M là nguyên thủy; gọi $e$ là một phần tử lũy đẳng trong vành địa phương End$_A(M)$. Vì $e^2=e$, hoặc $e$ là khả nghịch và ta có $e= 1$, hoặc $1-e$ là khả nghịch và ta có $e= 0$. Điều này chứng minh rằng M là không phân tích được (VIII, p. 30).

Bây giờ, giả sử rằng M là không phân tích được và có độ dài hữu hạn. Theo Mệnh đề 2, c) của VIII, p. 27, mọi tự đồng cấu của M đều khả nghịch hoặc lũy linh; do đó vành End$_A(M)$ là địa phương theo Ví dụ 2 của VIII, p. 26.

$\mathbf{Z}$-môđun $\mathbf{Z}$ là không phân tích được, Noether, nhưng không Artin. Vành tự đồng cấu của nó đẳng cấu với $\mathbf{Z}$, nên không địa phương. Do đó, $\mathbf{Z}$ không phải là một $\mathbf{Z}$-môđun nguyên thủy.

$*$Cho $p$ là một số nguyên tố. Vành tự đồng cấu của $\mathbf{Z}$-môđun $\mathbf{Q}_p/\mathbf{Z}_p$ đẳng cấu với vành địa phương $\mathbf{Z}_p$ (x. VII, §4, p. 65, Bài tập 13); do đó nó là một $\mathbf{Z}$-môđun nguyên thủy.

Một môđun đơn ánh là không phân tích được khi và chỉ khi nó là nguyên thủy (X, §1, n$^o9$, p. 21, mệnh đề $14$)$.*$

### 4. Môđun nửa nguyên thủy

#### Định nghĩa 4 {#alg-viii-s2-def-4 .statement tag=0028}

Một môđun được gọi là nửa nguyên thủy nếu nó là tổng trực tiếp của một họ các môđun con nguyên thủy.

#### Ví dụ 1 {#alg-viii-s2-n4-exa-1 .statement tag=00SE}

$*$Mọi môđun đơn đều là nguyên thủy (VIII, p. 45); do đó mọi môđun nửa đơn đều là nửa nguyên thủy (VIII, p. 55, Định nghĩa 1).

#### Ví dụ 2 {#alg-viii-s2-n4-exa-2 .statement tag=01L7}

Nếu A là một vành Noether trái, thì mọi A-môđun đơn ánh đều nửa nguyên thủy (X, §1, n$^o9$, p. 21, mệnh đề 14 và X, §1, n$^o10$, p. 22, định lý 3, b)).$*$

#### Định lý 1 (Azumaya) {#alg-viii-s2-thm-1 .statement tag=00RX}

Cho A là một vành, L một A-môđun nguyên thủy, và M một A-môđun nửa nguyên thủy. Tồn tại một lực lượng duy nhất, ký hiệu là [M : L], có tính chất sau:

Với mọi phân tích $M =\bigoplus_{i\in I}M_i$ của M thành tổng trực tiếp các môđun nguyên thủy, tập hợp các chỉ số $i\in I$ sao cho $M_i$ đẳng cấu với L có lực lượng [M : L].

Chứng minh dựa trên bốn bổ đề sau đây.

#### Bổ đề 1 {#alg-viii-s2-lem-1 .statement tag=0029}

Cho M là một A-môđun, $M'$ một môđun con nguyên thủy của M, và $M''$ một môđun con của M bổ sung với $M'$. Cho $u$ là một tự đồng cấu của M. Khi đó $u$ hoặc $1_M-u$ cảm sinh một đẳng cấu từ $M'$ lên một môđun con của M bổ sung với $M''$.

Cho $p$ là phép chiếu từ M lên $M'$ với hạt nhân $M''$, và cho $v$ là hạn chế của $p\circ u$ lên $M'$. Trước hết, giả sử rằng $v$ là một tự đẳng cấu của $M'$. Vì $v$ là đơn ánh, hạn chế của $u$ lên $M'$ là đơn ánh, và ta có $u(M')\cap M''= 0$. Vì $v$ là toàn ánh, ta có $u(M')\oplus M''= M$. Do đó, $u$ cảm sinh một đẳng cấu từ $M'$ lên một môđun con phụ với $M''$ trong M. Bây giờ, giả sử rằng $v$ không phải là một tự đẳng cấu của $M'$. Khi đó $1_{M'}-v$ là một tự đẳng cấu của $M'$ vì $M'$ là nguyên thủy. Bây giờ, $1_{M'}-v$ là hạn chế của $p\circ (1_M-u)$ lên $M'$. Lập luận trước chứng minh rằng $1_M-u$ cảm sinh một đẳng cấu từ $M'$ lên một môđun con của M phụ với $M''$.

#### Bổ đề 2 {#alg-viii-s2-lem-2 .statement tag=002A}

Cho M là một A-môđun là tổng trực tiếp của một họ $(M_i)_{i\in I}$ các môđun con nguyên thủy, và cho $u$ là một tự đồng cấu của M. Đặt $v= 1_M-u$ và $M_J=\bigoplus_{i\in J}M_i$ với mọi tập con J của I. Khi đó một trong hai tính chất sau đây được thỏa mãn:

a) Tồn tại một chỉ số $i\in I$ sao cho $u$ cảm sinh một đẳng cấu từ $M_i$ lên một môđun con hạng tử trực tiếp của M.

b) Với mọi tập con hữu hạn J của I$,v$ cảm sinh một đẳng cấu từ $M_J$ lên một môđun con phụ của $M_{I-J}$.

Nếu tính chất b) được thỏa mãn, thì $v$ là đơn ánh.

Giả sử rằng tính chất a) không đúng, và hãy thiết lập tính chất b) bằng quy nạp theo lực lượng của J. Không có gì phải chứng minh nếu $J =\emptyset$. Do đó, giả sử J khác rỗng, chọn một phần tử $i$ của J, và đặt $J'= J-\{i\}$. Theo giả thiết quy nạp, $v$ cảm sinh một đẳng cấu từ $M_{J'}$ lên một môđun con của M phụ với $M_{I-J'}= M_{I-J}\oplus M_i$; do đó, môđun con $M''=v(M_{J'})\oplus M_{I-J}$ phụ với $M_i$. Theo Bổ đề 1 và giả thiết về $u$, tự đồng cấu $v$ cảm sinh một đẳng cấu từ $M_i$ lên một môđun con của M phụ với $M''$; do đó, $v$ cảm sinh một đẳng cấu từ $M_J= M_i\oplus M_{J'}$ lên một môđun con phụ với $M_{I-J}$.

Khẳng định cuối cùng suy ra từ sự kiện rằng M là hợp của các môđun con $M_J$, trong đó J chạy qua các tập con hữu hạn của I.

#### Bổ đề 3 {#alg-viii-s2-lem-3 .statement tag=002B}

Cho M là một A-môđun là tổng trực tiếp của một họ $(M_i)_{i\in I}$ các môđun con nguyên thủy, và cho $p$ là một phép chiếu khác không của M. Tồn tại một chỉ số $i\in I$ sao cho $p$ cảm sinh một đẳng cấu từ $M_i$ lên một môđun con hạng tử trực tiếp của $p(M)$.

Vì $p$ khác không, $1_M-p$ không đơn ánh. Theo Bổ đề 2, tồn tại một chỉ số $i\in I$ sao cho $p$ cảm sinh một đẳng cấu từ $M_i$ lên một môđun con hạng tử trực tiếp của M. Mọi phép chiếu của M có ảnh là $p(M_i)$ đều xác định, bằng hạn chế, một phép chiếu của $p(M)$ có ảnh là $p(M_i)$, do đó $p(M_i)$ là một môđun con hạng tử trực tiếp của $p(M)$.

#### Bổ đề 4 {#alg-viii-s2-lem-4 .statement tag=002C}

Cho M là một A-môđun là tổng trực tiếp của một họ $(M_i)_{i\in I}$ các môđun con nguyên thủy, cho L là một A-môđun nguyên thủy, và cho N là một môđun con hạng tử trực tiếp của M. Giả sử rằng N là tổng trực tiếp của một họ $(N_j)_{j\in J}$ các môđun con đẳng cấu với L, và ký hiệu bởi $I_L$ tập hợp các chỉ số $i\in I$ sao cho $M_i$ đẳng cấu với L. Khi đó ta có

(1) Lực lượng của J $\leqslant$ lực lượng của I$_L$.

Cho $N_0$ là một môđun con của M bổ sung với N. Môđun M là tổng trực tiếp của $N_0$ và họ $(N_j)_{j\in J}$. Với mọi $j\in J$, ký hiệu bởi $p_j$ phép chiếu của M có ảnh $N_j$ liên kết với phân tích này (II, §1, No. 8, p. 209, Mệnh đề 12). Với mọi $i\in I$, ký hiệu bởi $J(i)$ tập hợp các chỉ số $j\in J$ sao cho $p_j$ cảm sinh một đẳng cấu từ $M_i$ đến $N_j$. Tập hợp này là hữu hạn: thật vậy, nếu $x$ là một phần tử khác không của $M_i$ và K là một tập con hữu hạn của J sao cho $x$ thuộc $N_0+\sum_{k\in K}N_k$, thì ta có $p_j(x) = 0$ với $j\in J$- K, do đó $J(i)$ được chứa trong K.

Cho $j\in J$. Theo Bổ đề 3, tồn tại một chỉ số $i\in I$ sao cho $p_j$ cảm sinh một đẳng cấu từ $M_i$ lên một môđun con hạng tử trực tiếp của $N_j$. Vì $M_i$ khác không và $N_j$ là nguyên thủy nên do đó không phân tích được (VIII, p. 31, Mệnh đề 4), ta có $p_j(M_i) = N_j$, và $j$ thuộc $J(i)$. Vì môđun $M_i$ đẳng cấu với $N_j$ và do đó với L, nên chỉ số $i$ thuộc $I_L$. Điều này chứng tỏ rằng J là hợp của họ các tập hợp hữu hạn $(J(i))_{i\in I_L}$. Nếu tập hợp J là vô hạn, thì tập hợp $I_L$ là vô hạn, và ta có (Lý thuyết tập hợp, III, §6, No. 3, p. 188, Hệ quả 3)

Lực lượng của J $\leqslant \sum_{i\in I_L}$ lực lượng của J($i$)$\leqslant$ lực lượng của I$_L$.

Bây giờ, giả sử rằng tập hợp J là hữu hạn, và hãy chứng minh bổ đề bằng quy nạp theo lực lượng của J. Nếu J rỗng, thì không có gì phải chứng minh. Vậy, giả sử rằng J khác rỗng, và chọn một phần tử $j$ của J. Theo trên, tồn tại một chỉ số $i\in I_L$ sao cho $p_j$ cảm sinh một đẳng cấu từ $M_i$ lên $N_j$. Đặt $I'= I-\{i\}$ và $J'= J-\{j\}$. Môđun M là tổng trực tiếp của $M_i$ và hạt nhân của $p_j$. Nó cũng là tổng trực tiếp của $M_i$ và môđun con $M'=\oplus_{i'\in I'}M_{i'}$. Do đó, tồn tại (II, §1, No. 9, p. 210, Hệ quả của Mệnh đề 13) một đẳng cấu $\varphi$ từ Ker $p_j= N_0\oplus_{j'\in J'}N_{j'}$ lên $M'$. Đặt $N'=\varphi (\sum_{j'\in J'}N_{j'})$. Môđun con $N'$ của $M'$ là một nhân tử trực tiếp và là tổng trực tiếp của họ $(\varphi (N_{j'}))_{j'\in J'}$ các môđun con nguyên thủy đẳng cấu với L. Hãy áp dụng giả thiết quy nạp cho $M'$ và $N':$ ta có Card(J$'$)$\leqslant$ Card(I$_L-\{i\}$) và do đó có bất đẳng thức (1).

Hãy chứng minh Định lý 1. Cho $(M_i)_{i\in I}$ và $(N_j)_{j\in J}$ là hai họ các môđun con nguyên thủy có tổng trực tiếp là M. Gọi $I_L$ (resp. $J_L$) là tập hợp các $i\in I$ (resp. $j\in J$) sao cho $M_i$ (resp. $N_j$) đẳng cấu với L. Ta có Card(J$_L$)$\leqslant$ Card(I$_L$) theo Bổ đề 4. Đổi chỗ vai trò của I và J, ta được bất đẳng thức nghịch đảo và do đó định lý.

Lực lượng [M : L] được định nghĩa trong Định lý 1 được gọi là bội nguyên thủy của L trong M.

#### Hệ quả 1 {#alg-viii-s2-lem-4-cor-1 .statement tag=002D}

Cho M và N là các môđun nửa nguyên thủy. Khi đó M và N đẳng cấu nếu và chỉ nếu ta có [M : L] = [N : L] đối với mọi môđun nguyên thủy L.

#### Hệ quả 2 {#alg-viii-s2-lem-4-cor-2 .statement tag=00QY}

Cho M là một môđun nửa nguyên thủy. Cho $(M_i)_{i\in I}$ và $(M'_j)_{j\in J}$ là các họ các môđun con nguyên thủy của M sao cho

$$
M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j
$$

Khi đó tồn tại một tự đẳng cấu $u$ của M và một song ánh $\varphi$ từ I lên J sao cho ta có $u(M_i) = M'_{\varphi(i)}$ với mọi $i\in I$.

Với mọi môđun nguyên thủy L, đặt $I_L$ (tương ứng, $J_L$) là tập hợp chỉ số $i\in I$ (tương ứng, $j\in J$) sao cho $M_i$ (tương ứng, $M'_j$) đẳng cấu với L. Các tập hợp khác rỗng có dạng $I_L$ (tương ứng, $J_L$) tạo thành một phân hoạch của I (tương ứng, J), và với mọi L, ta có

Card(I$_L$) $=$ Card(J$_L$) $= [M : L]$;

hệ quả suy ra.

#### Hệ quả 3 {#alg-viii-s2-lem-4-cor-3 .statement tag=002E}

Cho M, N, và P là các môđun nửa nguyên thủy. Giả sử rằng $M\oplus P$ đẳng cấu với $N\oplus P$ và [P : L] là hữu hạn với mọi môđun nguyên thủy L. Khi đó M và N đẳng cấu.

Theo giả thiết, ta có

[M : L] + [P : L] = [N : L] + [P : L]

với mọi môđun nguyên thủy L. Vì [P : L] là hữu hạn, suy ra bằng quy nạp từ (Lý thuyết tập hợp, III, §3, No. 4, p. 162, Mệnh đề 8) rằng ta có [M : L] = [N : L] với mọi môđun nguyên thủy L. Do đó các môđun M và N đẳng cấu theo Hệ quả 1.

#### Hệ quả 4 {#alg-viii-s2-lem-4-cor-4 .statement tag=002F}

Cho M và N là các môđun nửa nguyên thủy. Giả sử rằng tồn tại một số nguyên $d >0$ sao cho $M^d$ đẳng cấu với $N^d$. Khi đó các môđun M và N đẳng cấu.

Cho L là một môđun nguyên thủy. Theo giả thiết, ta có

$$
d[M : L] =d[N : L]
$$

Do đó ta có đẳng thức [M : L] = [N : L]: thật vậy, ta có $d\mathfrak{a}=\mathfrak{a}$ với mọi bản số vô hạn $\mathfrak{a}($Lý thuyết tập hợp, III, §6, No. 3, p. 188, Hệ quả 4). Khi đó các môđun M và N đẳng cấu theo Hệ quả 1.

#### Hệ quả 5 {#alg-viii-s2-lem-4-cor-5 .statement tag=002G}

Cho M là một môđun nửa nguyên thủy là tổng trực tiếp của một họ hữu hạn $(M_i)_{i\in I}$ các môđun con nguyên thủy. Với mọi tập con J của I, đặt $M_J=\bigoplus_{i\in J}M_i$. Cho N là một môđun con hạng tử trực tiếp của M.

a) Tồn tại một tập con J của I sao cho $M_J$ là một môđun con phụ của N.

b) Cho J là một tập con của I. Nếu $M_J$ là bù của N, thì môđun N đẳng cấu với $M_{I-J}$ và là nửa nguyên thủy.

Ta ký hiệu bởi K tập hợp các chỉ số $i\in I$ sao cho $N\cap M_i= 0$; hãy dùng quy nạp theo lực lượng của K. Hệ quả là hiển nhiên nếu M = N. Giả sử $M\not= N$. Gọi $p$ là một phép chiếu của M có hạt nhân là N. Ký hiệu ảnh của nó bởi P. Nó khác không, và theo Bổ đề 3, tồn tại một $j\in I$ sao cho $p$ cảm sinh một đẳng cấu từ $M_j$ lên một môđun con hạng tử trực tiếp của P. Ta có $N\cap M_j= 0$. Đặt $N'= N\oplus M_j$. Ta có $N'= N\oplus p(M_j)$. Một môđun con phụ của $p(M_j)$ trong P cũng là môđun con phụ của $N'$ trong M, do đó $N'$ là một môđun con hạng tử trực tiếp của M. Tập hợp các chỉ số $i\in I$ sao cho $N'\cap M_i= 0$ được chứa trong K $-\{j\}$. Theo giả thiết quy nạp, tồn tại một tập con $J'$ của I sao cho $M_{J'}$ là một môđun con phụ của $N'$ trong M. Đặt $J = J'\cup  \{j\}$. Khi đó $M_J$ là một môđun con phụ của N trong M.

Cho J là một tập con của I sao cho $M_J$ là một môđun con phụ của M trong N. Vì $M_J$ cũng phụ đối với $M_{I-J}$, các môđun N và $M_{I-J}$ là đẳng cấu và N là nửa nguyên thủy.

#### Hệ quả 6 {#alg-viii-s2-lem-4-cor-6 .statement tag=002H}

Mọi môđun xạ ảnh hữu hạn sinh trên một vành địa phương đều tự do.[^2]

Cho A là một vành địa phương. A-môđun $A_s$ là nguyên thủy (VIII, p. 31). Nếu M là một A-môđun xạ ảnh hữu hạn sinh, thì tồn tại một A-môđun N và một số tự nhiên $n$ sao cho $M\oplus N$ đẳng cấu với $A^n_s$ (II, §2, No. 2, p. 232, Hệ quả 1). Suy ra từ Hệ quả 5 rằng môđun M tự nó đẳng cấu với $A^m_s$ với một số nguyên $m$ sao cho $0\leqslant m\leqslant n$, do đó là tự do.

#### Nhận xét {#alg-viii-s2-n4-rem-1 .statement tag=002I}

Cho M và $M'$ là các A-môđun nửa nguyên thủy. Từ Bổ đề 4 của VIII, p. 33 ngay lập tức suy ra rằng $M'$ đẳng cấu với một môđun con hạng tử trực tiếp của M khi và chỉ khi ta có $[M': L]\leqslant [M : L]$ đối với mọi A-môđun nguyên thủy L. Đặc biệt, nếu L là một A-môđun nguyên thủy, thì [M : L] là số lực lớn nhất trong các số lực $\mathfrak{a}$ sao cho tồn tại một môđun con hạng tử trực tiếp của M đẳng cấu với $L^{(\mathfrak{a})}$.

Do đó quan hệ [M : L] = 0 có nghĩa là không tồn tại môđun con hạng tử trực tiếp nào của M đẳng cấu với L. Điều này không loại trừ sự tồn tại của một môđun con của M đẳng cấu với L; chỉ cần xét ví dụ trong đó $A =\mathbf{Z}, L =\mathbf{Z}/2\mathbf{Z}$, và $M =\mathbf{Z}/4\mathbf{Z}:$ các $\mathbf{Z}$-môđun L và M là nguyên thủy và không đẳng cấu, nên [M : L] = 0 và L đẳng cấu với môđun con $2\mathbf{Z}/4\mathbf{Z}$ của M.

### 5. Cấu trúc của các môđun có độ dài hữu hạn

#### Định lý 2 (Krull–Remak–Schmidt) {#alg-viii-s2-thm-2 .statement tag=00RY}

Cho A là một vành và M là một A-môđun có độ dài hữu hạn.

a) Tồn tại một họ hữu hạn $(M_i)_{i\in I}$ các môđun con không phân tích được của M sao cho $M =\bigoplus_{i\in I}M_i$, và môđun M là nửa nguyên thủy.

b) Cho $(M_i)_{i\in I}$ và $(M'_j)_{j\in J}$ là hai họ hữu hạn các môđun con không phân tích được của M sao cho $M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j$. Tồn tại một song ánh $\sigma$ từ I tới J và một tự đẳng cấu $u$ của M sao cho ta có $u(M_i) = M'_{\sigma(i)}$ với mọi $i\in I$.

c) Cho N là một môđun con hạng tử trực tiếp của M, và cho $(M_i)_{i\in I}$ là một họ hữu hạn các môđun con không phân tích được của M có tổng trực tiếp là M. Tồn tại một tập con J của I sao cho $\bigoplus_{i\in I-J}M_i$ là bổ sung với N. Môđun N đẳng cấu với $\bigoplus_{j\in J}M_j$.

d) Cho N là một A-môđun. Nếu tồn tại một số nguyên $d >0$ sao cho các môđun $M^d$ và $N^d$ đẳng cấu, thì các môđun M và N đẳng cấu.

e) Cho N và P là các A-môđun có độ dài hữu hạn. Nếu các môđun $M\oplus P$ và $N\oplus P$ đẳng cấu, thì M và N đẳng cấu.

Một môđun có độ dài hữu hạn vừa là Artin vừa là Noether (VIII, p. 2, Mệnh đề 1). Hơn nữa, đối với một môđun có độ dài hữu hạn, không phân tích được hay nguyên thủy thì cũng là như nhau (VIII, p. 31, Mệnh đề 4). Khi đó mệnh đề a) suy ra từ Mệnh đề 3 của VIII, p. 30. Các mệnh đề b), c), và e) suy ra lần lượt từ các Hệ quả 2, 5, và 3 của Định lý 1 của VIII, p. 32. Sau cùng, mệnh đề d) suy ra từ Hệ quả 4 của VIII, p. 35 vì dưới các giả thiết của d), môđun N có độ dài hữu hạn và do đó là nửa nguyên thủy theo a).

#### Định lý 3 {#alg-viii-s2-thm-3 .statement tag=002J}

Cho K là một trường giao hoán, A là một đại số trên K, và M và N là các môđun có độ dài hữu hạn. Cho $K'$ là một đại số giao hoán trên K khác không sao cho các $A_{(K')}$-môđun $M_{(K')}$ và $N_{(K')}$ là đẳng cấu. Khi đó các A-môđun M và N là đẳng cấu.

a) Trước hết, giả sử rằng đại số $K'$ có bậc hữu hạn $d$ trên K. Khi đó A-môđun $M_{(K')}$ đẳng cấu với $M^d$ và A-môđun $N_{(K')}$ đẳng cấu với $N^d$, nên các A-môđun $M^d$ và $N^d$ là đẳng cấu. Theo Định lý 2, d), các A-môđun M và N là đẳng cấu.

b) Bây giờ, giả sử rằng đại số trên K $K'$ được sinh bởi hữu hạn phần tử. Chọn một iđêan cực đại $\mathfrak{m}$ của $K'$, và đặt $K''= K'/\mathfrak{m}$. Theo Định lý không điểm của Hilbert (VIII, p. 462, Hệ quả 1 của Định lý 1)$, K''$ là một mở rộng bậc hữu hạn của K. Bằng mở rộng vô hướng từ $K'$ đến $K''$, ta suy ra từ đẳng cấu $A_{(K')}$-tuyến tính $M_{(K')}\rightarrow N_{(K')}$ một đẳng cấu $A_{(K'')}$-tuyến tính $M_{(K'')}\rightarrow N_{(K'')}$. Theo phần a) của chứng minh, các A-môđun M và N là đẳng cấu.

c) Sau cùng, hãy xét trường hợp tổng quát. Cho $u: M_{(K')}\rightarrow N_{(K')}$ là một đẳng cấu của các $A_{(K')}$-môđun và $v: N_{(K')}\rightarrow M_{(K')}$ là đẳng cấu nghịch đảo. Ký hiệu $\mathscr{E}$ là tập hợp các K-đại số con của $K'$ sinh bởi hữu hạn phần tử. Nếu E là một đại số con như vậy, thì $A_{(E)}$ được đồng nhất với một vành con của $A_{(K')}$, và $M_{(E)}$ và $N_{(E)}$ được đồng nhất tương ứng với các $A_{(E)}$-môđun con của $M_{(K')}$ và $N_{(K')}$ (II, §7, No. 7, p. 306); hơn nữa, $M_{(K')}$ và $N_{(K')}$ tương ứng là các hợp của các họ có hướng phải $(M_{(E)})_{E\in\mathscr{E}}$ và $(N_{(E)})_{E\in\mathscr{E}}$. Các A-môđun M và N có độ dài hữu hạn, do đó sinh hữu hạn; gọi S là một tập con sinh hữu hạn của A-môđun M và T là một tập con sinh hữu hạn của A-môđun N. Tồn tại một đại số trên K $E\in \mathscr{E}$ sao cho ta có $u(1\otimes s)\in N_{(E)}$ với mọi $s\in S$ và $v(1\otimes t)\in M_{(E)}$ với mọi $t\in T$. Từ tính tuyến tính suy ra rằng ta có $u(M_{(E)})\subset N_{(E)}$ và $v(N_{(E)})\subset M_{(E)}$. Khi đó các ánh xạ $u$ và $v$ cảm sinh các song ánh nghịch đảo từ $M_{(E)}$ đến $N_{(E)}$ và từ $N_{(E)}$ đến $M_{(E)}$. Các song ánh này rõ ràng là $A_{(E)}$-tuyến tính. Vì thế, các $A_{(E)}$-môđun $M_{(E)}$ và $N_{(E)}$ là đẳng cấu. Theo phần b) của chứng minh, các A-môđun M và N là đẳng cấu.

#### Nhận xét {#alg-viii-s2-n5-rem-1 .statement tag=002K}

Cho E và F là hai không gian vectơ hữu hạn chiều trên một trường giao hoán K, và cho $K'$ là một mở rộng của K. Cho $u$ là một tự đồng cấu của E và $v$ là một tự đồng cấu của F, và cho $u_{(K')}$ và $v_{(K')}$ là các tự đồng cấu của $E_{(K')}$ và $F_{(K')}$ thu được bằng phép mở rộng vô hướng. Từ Hệ quả 1 và 2 của VII, §5, No. 3, p. 32 suy ra rằng các tự đồng cấu $u$ và $v$ là đồng dạng nếu và chỉ nếu các tự đồng cấu $u_{(K')}$ và $v_{(K')}$ là đồng dạng. Điều này cũng suy ra từ Định lý 3 ở trên áp dụng cho đại số A = K[X] và các A-môđun $M = E_u$ và $N = F_v$ (VII, §5, No. 1, p. 29).

### Bài tập {#alg-viii-s2-exercises}

Xem [bài tập của § 2](exercises/s2/).

[^1]: Chú ý được thêm vào trong bản dịch: một số tác giả dùng thuật ngữ “môđun có vành tự đồng cấu địa phương” cho “môđun nguyên thủy.”
[^2]: Có thể chứng minh rằng mọi môđun xạ ảnh trên một vành địa phương đều tự do (VIII, p. 42, Bài tập 18).
