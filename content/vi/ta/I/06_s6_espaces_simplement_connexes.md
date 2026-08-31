---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 6
section_title: Espaces simplement connexes
lang: vi
source: ta-i-iv-fr
book_pages: TA I.120-TA I.137, TA I.149-TA I.150
pdf_pages: 0136-0153, 0165-0166
extraction: native
subsections:
    - "no": 1
      title: Revêtement universel
      page: 120
      pdf_page: 136
    - "no": 2
      title: Parties convexes d’un espace numérique
      page: 122
      pdf_page: 138
    - "no": 3
      title: Espaces simplement connexes
      page: 124
      pdf_page: 140
    - "no": 4
      title: Produit d’un espace par un espace simplement connexe
      page: 129
      pdf_page: 145
    - "no": 5
      title: Groupes d’homéomorphismes des espaces simplement connexes
      page: 133
      pdf_page: 149
statements: 37
exercises: 6
content_sha256: 26de2adf9b9405f7fcae958fe1d676d0dcac6933de0b443d001c385e396a0e13
translated_from: content/en-mt/ta/I/06_s6_espaces_simplement_connexes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: ea73a4b6ca508a16865cbf192ca6bdf346b0d854357139b45cb4fefd332cffaf
translation_model: gpt-5.4
translation_run: translate-vi-b7a3a707
glossary_version: 34
glossary_terms_sha256: cc6bb84846d007968895234893af32a05a43419d9451acd7fe762f8570e308da
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. KHÔNG GIAN ĐƠN LIÊN THÔNG

### 1. Phủ phổ quát

#### Định nghĩa 1 {#ta-i-s6-def-1 .statement tag=01RR}

Một tập hợp có điểm gốc là một tập hợp X được trang bị một trong các phần tử của nó, gọi là điểm gốc. Tập hợp X được trang bị điểm $x$ đôi khi được ký hiệu bởi $(X, x)$. Cho $(X, x)$ và $(Y, y)$ là các tập hợp có điểm gốc; một ánh xạ có điểm gốc từ $(X, x)$ vào $(Y, y)$ là một ánh xạ $f$ từ X vào Y sao cho $f(x) =y$.

Các khái niệm không gian tôpô có điểm gốc, ánh xạ liên tục có điểm gốc, phủ có điểm gốc của một không gian tôpô có điểm gốc, v.v., được định nghĩa tương tự.

Nếu $(X, x)$ và $(Y, y)$ là các không gian tôpô có điểm gốc, thì tập hợp các ánh xạ liên tục có điểm gốc từ $(X, x)$ vào $(Y, y)$ được ký hiệu bởi $\mathscr{C}((X, x); (Y, y))$.

Thay vì nói “cho $f$ là một ánh xạ có điểm gốc từ $(X, x)$ vào $(Y, y)$”, người ta thường dùng cách nói sau: “cho $f: (X, x)\rightarrow (Y, y)$ là một ánh xạ có điểm gốc”.

Cho B là một không gian tôpô và cho $b$ là một điểm của B.

#### Định nghĩa 2 {#ta-i-s6-def-2 .statement tag=01RS}

Một phủ có điểm gốc $(E, x)$ của $(B, b)$ được gọi là một phủ phổ quát nếu, với mọi phủ có điểm gốc $(E', x')$ của $(B, b)$, tồn tại một cấu xạ duy nhất của các phủ của B, $f: E\rightarrow E'$, sao cho $f(x) =x'$.

Nếu $(E, x)$ và $(E', x')$ là các phủ phổ quát của $(B, b)$, thì B-cấu xạ duy nhất từ $(E, x)$ vào $(E', x')$ là một đẳng cấu của các B-không gian.

Cho E là một phủ liên thông của B và cho $x$ là một điểm của sợi $E_b$. Giả sử rằng, với mọi phủ có điểm gốc $(E', x')$ của $(B, b)$, tồn tại một cấu xạ $f: E\rightarrow E'$ của các phủ của B sao cho $f(x) =x'$. Khi đó một cấu xạ như vậy $f$ là duy nhất (I, p. 34, Hệ quả 1 của Mệnh đề 11), do đó $(E, x)$ là một phủ phổ quát của $(B, b)$. *Ta sẽ thấy sau này (I, p. 126, Hệ quả của Mệnh đề 3) rằng điều này đặc biệt đúng nếu mọi phủ của E đều khả tầm thường hóa.*

#### Mệnh đề 1 {#ta-i-s6-prop-1 .statement tag=01RT}

Cho B là một không gian tôpô liên thông và địa phương liên thông và cho $b$ là một điểm của B. Cho $(E, x)$ là một phủ phổ quát của $(B, b)$. Khi đó E là một phủ Galois của B và mọi phủ của B đều có thể được liên kết với E.

Không gian E là địa phương liên thông, vì B có tính chất đó. Cho $E_0$ là thành phần liên thông của $x$ trong E, để không gian $(E_0, x)$ là một phủ có điểm gốc của $(B, b)$ (I, p. 80, Hệ quả 1 của Mệnh đề 6). Khi đó tồn tại một cấu xạ duy nhất của các phủ $f: E\rightarrow E_0$ sao cho $f(x) =x$. Nếu $i$ ký hiệu đơn ánh chính tắc của $E_0$ vào E, thì ánh xạ $i\circ f: E\rightarrow E$ là một cấu xạ của các phủ biến $x$ thành $x$, cũng như ánh xạ Id$_E$; vì $(E, x)$ là một phủ phổ quát của $(B, b)$, do đó ta có $i\circ f=$ Id$_E$. Suy ra $i$ là toàn ánh, nên $E_0= E$. Do đó, E là liên thông.

Cho $y$ là một điểm của $E_b$ và xét phủ có điểm gốc $(E, y)$ của $(B, b)$; theo giả thiết tồn tại một cấu xạ duy nhất của các phủ $f: E\rightarrow E$ sao cho $f(x) =y$. Ánh xạ $s: E\rightarrow E\times_BE$ được xác định bởi $t\mapsto (t, f(t))$ là một tiết diện liên tục của ánh xạ pr$_1: E\times_BE\rightarrow E$. Theo Hệ quả 4 của I, p. 81, điều này chứng minh rằng phủ $E\times_BE$ của E cho bởi ánh xạ pr$_1$ là tầm thường hóa được. Do đó phủ E là Galois (Định lý 2 của I, p. 102). Khi đó suy ra từ I, p. 112, hệ quả của Mệnh đề 10, rằng mọi phủ của B đều có thể được liên kết với E.

#### Hệ quả {#ta-i-s6-n1-cor-1 .statement tag=01RU}

Cho B là một không gian tôpô địa phương liên thông. Cho $b$ là một điểm của B và cho $(E, x)$ là một phủ phổ quát của $(B, b)$. Với một không gian con A của B, hai tính chất sau là tương đương:

(i) Phủ E là tầm thường hóa được trên A;

(ii) Mọi phủ của B đều là tầm thường hóa được trên A.

Tính chất (ii) hiển nhiên kéo theo tính chất (i). Chiều đảo lại suy ra từ sự kiện rằng mọi phủ của B đều có thể được liên kết với phủ E (I, p. 105, Mệnh đề 7).

### 2. Các tập con lồi của một không gian số

Cho E là không gian số $n$-chiều *(hoặc, tổng quát hơn, một không gian vectơ tôpô trên $\mathbf{R}$)$*$. Với mọi cặp $(x, y)$ điểm của E, đoạn thẳng (tương ứng, đoạn thẳng mở) có các đầu mút $x$ và $y($xem EVT, II, p. 7) theo định nghĩa là tập hợp các điểm của E có dạng $tx+$ $(1-t)y$, với $t\in [0,1]$ (tương ứng với $t\in ]0,1[$). Cho A là một tập con của E. Người ta nói rằng tập hợp A là lồi nếu với mọi cặp $(x, y)$ điểm của A và mọi $t\in \mathbf{I}$, điểm $tx+ (1-t)y$ thuộc A.

*Một tập con lồi thì liên thông bằng cung.*

#### Bổ đề 1 {#ta-i-s6-lem-1 .statement tag=01RV}

Cho E là không gian số $n$-chiều và cho A là một tập con lồi compắc của E mà 0 là một điểm trong của nó. Với mọi $x\in E$, ký hiệu $p_A(x)$ là cận dưới lớn nhất trong $\overline{\mathbf{R}}$ của tập hợp các số thực $t >0$ sao cho $x\in tA$.

Ánh xạ $p_A$ là hữu hạn, liên tục, và có các tính chất sau:

(i) Với mọi $x\in E$ sao cho $x= 0\not$ , ta có $p_A(x)>0$ ;

(ii) Với mọi $s\in \mathbf{R}_+$ và mọi $x\in E$, ta có $p_A(sx) =sp_A(x)$.

(iii) Với mọi $x$ và $y\in E$, ta có $p_A(x+y)\leqslant p_A(x) +p_A(y)$.

(iv) Điều kiện cần và đủ để một điểm $x$ của E thuộc A là $p_A(x)\leqslant 1$.

Với $x\in E$, ký hiệu $\|x\|$ là chuẩn Euclid của $x$ (TG, VI, p. 7). Vì A compắc, tồn tại một số thực $M>0$ sao cho mọi điểm $x$ của A đều thỏa mãn $\|x\|\leqslant M$. Vì 0 là một điểm trong của A, tồn tại một số thực $m >0$ sao cho mọi điểm $x$ của E thỏa mãn $\|x\|\leqslant m$ đều thuộc A. Do đó, ta có quan hệ $\|x\|/M\leqslant p_A(x)\leqslant \|x\|/m$, với mọi $x\in E$. Đặc biệt, $p_A(0) = 0$ và $p_A(x)= 0\not$ nếu $x= 0\not$ .

Các khẳng định (ii) và (iv) suy ra ngay lập tức từ định nghĩa của ánh xạ $p_A$.

Cho $x$ và $y$ là các điểm của E. Cho $x'$ và $y'$ là các điểm của A sao cho $x=p_A(x)x'$ và $y=p_A(y)y'$. Nếu $x$ và $y$ không đồng thời bằng không thì $p_A(x) +p_A(y)>0$ và ta có

$$
x+y=p_A(x)x'+p_A(y)y'
$$

$$
= (p_A(x) +p_A(y))(\frac{p_A(x)}{p_A(x) + p_A(y)}x'+\frac{p_A(y)}{p_A(x) + p_A(y)}y')
$$

Vì A lồi, điều này chứng tỏ rằng $x+y$ thuộc về $(p_A(x) +$ $p_A(y))A$, do đó $p_A(x+y)\leqslant p_A(x) +p_A(y)$. Nếu $x=y= 0$, bất đẳng thức này vẫn đúng, vì $p_A(0) = 0$. Điều này chứng minh mệnh đề (iii).

Áp dụng bất đẳng thức này cho $x+y$ và $-y$, suy ra rằng, với mọi cặp $(x, y)$ điểm của E, ta có

$|p_A(x+y)-p_A(x)|\leqslant$ max($p_A(y), p_A(-y)$)$\leqslant m^{-1}\|y\|$.

Điều này chứng minh rằng ánh xạ $p_A$ là liên tục, do đó bổ đề.

Ánh xạ $p_A$ được gọi là chuẩn Minkowski của tập con lồi A.

#### Mệnh đề 2 {#ta-i-s6-prop-2 .statement tag=01RW}

Cho E là không gian số chiều $n$ và cho A là một tập con lồi và compáct của E mà 0 là một điểm trong của nó. Tồn tại một song ánh duy nhất $u$ của E lên chính nó thỏa mãn ba tính chất sau:

(i) Với mọi $x\in E$ và mọi $t\in \mathbf{R}_+,u(tx) =tu(x)$;

(ii) Với mọi $x\in E$, tồn tại $\lambda \in \mathbf{R}_+$ sao cho $u(x) =\lambda x$;

(iii) Ta có $u(A) =\mathbf{B}_n$.

Ánh xạ $u$ là một đồng phôi và cảm sinh, bằng cách chuyển qua các không gian con, một đồng phôi của A lên $\mathbf{B}_n$, một đồng phôi của phần trong của A lên phần trong của $\mathbf{B}_n$ và một đồng phôi của biên của A trong E lên mặt cầu $\mathbf{S}_{n-1}$.

Cho $p_A$ là chuẩn Minkowski của tập con lồi A. Cho $x\in E$ và $t\in \mathbf{R}_+$; để có $x\in tA$, điều kiện cần và đủ là $p_A(x)\leqslant t$. Vì A compáct, tồn tại một số thực M sao cho $\|x\|\leqslant M$ với mọi $x\in A$.

Cho $u$ là một ánh xạ thỏa mãn các điều kiện của mệnh đề. Ta có $u(0) = 0$. Cho $x\in E-\{0\}$ và cho $\lambda \in \mathbf{R}_+$ sao cho $u(x) =\lambda x$. Với mọi $t\in \mathbf{R}_+$ sao cho $tx\in A$, ta có $u(tx) =t\lambda x$. Vì $u$ là đơn ánh, $\lambda = 0\not$ . Vì $u(A)$ được chứa trong $\mathbf{B}_n$, ta cũng có $\lambda \leqslant p_A(x)/\|x\|$. Đặt $z=x/\|x\|$; đó là một điểm của $\mathbf{S}_{n-1}$. Để $z$ có một ảnh ngược trong A qua $u$, điều kiện cần và đủ là điểm $(\lambda \|x\|)^{-1}x$ thuộc A, nghĩa là $\lambda \|x\|\geqslant p_A(x)$, tức là $\lambda \geqslant p_A(x)/\|x\|$. Điều này suy ra tính duy nhất của một ánh xạ như vậy $u$.

Bây giờ ký hiệu bởi $u$ ánh xạ từ E vào chính nó biến 0 thành 0 và biến $x$ thành $(p_A(x)/\|x\|)x$, với mọi $x\in E-\{0\}$.

Theo Bổ đề $1,u$ liên tục tại mọi điểm của E $-\{0\}$. Ta có $\|u(x)\|=p_A(x)$ với mọi $x\in E$ và $p_A(x)\rightarrow 0$ khi $x\rightarrow 0$ (loc. cit.); do đó, $u$ liên tục tại 0. Vậy $u$ là liên tục.

Ảnh ngược duy nhất của 0 qua $u$ là 0. Cho $y\in E-\{0\}$. Để một phần tử $x$ của E thỏa mãn $u(x) =y$, điều kiện cần và đủ là $x= (\|y\|/p_A(y))y$. Suy ra $u$ là một song ánh liên tục từ E lên chính nó. Nghịch đảo của nó là ánh xạ $v:y\mapsto (\|y\|/p_A(y))y$. Vì $p_A$ là liên tục và chỉ triệt tiêu tại 0, ánh xạ $v$ liên tục tại mọi điểm của E $-\{0\}$; bất đẳng thức $p_A(y)\geqslant \|y\|/M$ suy ra rằng $\|v(y)\|\leqslant M\|y\|$ với mọi $y\in E$. Suy ra $v$ là liên tục. Vậy ánh xạ $u$ là một đồng phôi từ E lên chính nó. Vì các quan hệ $p_A(x)\leqslant 1$ và $x\in A$ là tương đương, ta cũng có $u(X) =\mathbf{B}_n$. Mệnh đề được chứng minh.

#### Ví dụ {#ta-i-s6-n2-exa-1 .statement tag=01RX}

Tập hợp $[0,1]^n$ là một tập con lồi, compắc, có phần trong khác rỗng của $\mathbf{R}^n$. Suy ra từ mệnh đề 2 của I, p. 123 rằng nó đồng phôi với quả cầu Euclid đóng. Chính xác hơn, với mọi điểm $x$ của phần trong $]0,1[^n$ và mọi điểm $b$ của quả cầu Euclid mở, tồn tại một đồng phôi từ $[0,1]^n$ lên $\mathbf{B}_n$ biến $x$ thành $b$ và cảm sinh, khi chuyển qua các không gian con, một đồng phôi từ $]0,1[^n$ lên quả cầu Euclid mở, và cả một đồng phôi từ biên của $[0,1]^n$ lên mặt cầu $\mathbf{S}_{n-1}$.

Suy ra rằng mọi tập con lồi, compắc, có phần trong khác rỗng của $\mathbf{R}^n$ đều đồng phôi với một hình lập phương (loc. cit.).

### 3. Không gian Đơn liên thông

#### Định nghĩa 3 {#ta-i-s6-def-3 .statement tag=01RY}

Một không gian tôpô được gọi là đơn liên thông nếu mọi phủ của nó đều tầm thường hoá được.

Một không gian đơn liên thông thì liên thông. Thật vậy, nếu một không gian X là hợp rời nhau của hai tập hợp mở khác rỗng U và V, thì đơn ánh chính tắc từ U vào X là một phủ không tầm thường hoá được.

Không gian rỗng là đơn liên thông. Mọi không gian tôpô chỉ gồm một điểm đều là đơn liên thông.

#### Nhận xét 1 {#ta-i-s6-n3-rem-1 .statement tag=01RZ}

Cho B là một không gian tôpô đơn liên thông và cho $(E, p)$ là một phủ của B. Nếu không gian E liên thông và khác rỗng, thì ánh xạ $p$ là một đồng phôi. Chẳng hạn, cho G là một nhóm tôpô liên thông và H là một nhóm con rời rạc của G, sao cho ánh xạ chính tắc $p: G\rightarrow G/H$ làm cho G thành một phủ của $G/H$ (I, p. 100, hệ quả 2 của định lý 1). Nếu không gian $G/H$ là đơn liên thông, thì ánh xạ $p$ là một đồng phôi và H là nhóm con một phần tử.

#### Nhận xét 2 {#ta-i-s6-n3-rem-2 .statement tag=01S0}

Cho B là một không gian tôpô sao cho mọi điểm đều có một lân cận đơn liên thông; khi đó mọi phủ của một phủ của B đều là một phủ của B. Thật vậy, hãy xét một phủ $(E, p)$ của B cùng với một phủ $(F, q)$ của E. Ta sẽ chứng minh rằng $(F, p\circ q)$ là một phủ của B. Vì vấn đề là địa phương trên B, ta có thể giả sử rằng không gian B là đơn liên thông và do đó E là một phủ tầm thường hoá được của B. Cho V là một thành phần liên thông của E. Nó vừa mở vừa đóng và $p|V: V\rightarrow B$ là một đồng phôi (I, p. 69, mệnh đề 1); suy ra không gian V là đơn liên thông. Mọi thành phần liên thông W của $\overset{-1}{q}(V)$ đều vừa mở vừa đóng trong $\overset{-1}{q}(V)$, do đó trong F, và ánh xạ $q$ cảm sinh một đồng phôi từ W lên V. Vậy ánh xạ $p\circ q$ làm cho F thành một phủ của B, tầm thường hoá được (loc. cit.).

#### Mệnh đề 3 {#ta-i-s6-prop-3 .statement tag=01S1}

Cho B là một không gian tôpô. Cho $(E, p)$ là một phủ của B và cho $y$ là một điểm của E. Cho X là một không gian tôpô đơn liên thông, cho $f: X\rightarrow B$ là một ánh xạ liên tục và cho $x$ là một điểm của X sao cho $f(x) =p(y)$. Khi đó tồn tại một nâng liên tục duy nhất $g: X\rightarrow E$ của ánh xạ $f$ sao cho $g(x) =y$.

Các ánh xạ $g$ cần tìm tương ứng song ánh (I, p. 9, mệnh đề 3) với các tiết diện liên tục $s$ của phủ pr$_1: X\times_BE\rightarrow X$ sao cho $s(x) = (x, y)$. Một tiết diện như thế tồn tại vì không gian X là đơn liên thông; nó là duy nhất vì không gian X là liên thông (I, p. 34, hệ quả 1 của mệnh đề 11).

#### Ví dụ 1 {#ta-i-s6-n3-exa-1 .statement tag=01S2}

Cho X là một không gian tôpô đơn liên thông và cho $f$ là một hàm liên tục từ X vào $\mathbf{C}^*$. Nhắc lại (I, p. 101, ví dụ 6) rằng ánh xạ $z\mapsto e^z$ làm cho $\mathbf{C}$ thành một phủ của $\mathbf{C}^*$. Theo mệnh đề 3, tồn tại một hàm liên tục $h: X\rightarrow \mathbf{C}$ sao cho $f(x) =e^{h(x)}$ với mọi $x\in X$. Nếu $h': X\rightarrow \mathbf{C}$ là một hàm liên tục khác sao cho $f(x) =e^{h'(x)}$ với mọi $x\in X$, thì tồn tại một số nguyên $q\in \mathbf{Z}$ sao cho $h'=h+ 2\pi iq$.

Tương tự, cho $n$ là một số nguyên $>0$; ánh xạ $z\mapsto z^n$ làm cho $\mathbf{C}^*$ thành một phủ của chính nó (I, p. 101, ví dụ 5). Do đó tồn tại một hàm liên tục $k$ từ X vào $\mathbf{C}^*$ sao cho $k(x)^n=f(x)$ với mọi $x\in X$, chẳng hạn hàm $k(x) =e^{h(x)/n}$. Nếu $k': X\rightarrow \mathbf{C}^*$ là một hàm liên tục khác sao cho $k'(x)^n=f(x)$ với mọi $x\in X$, thì tồn tại một căn bậc $n^e$ của đơn vị $\mu\in \mathbf{C}$ sao cho $k'=\mu k$.

#### Hệ quả {#ta-i-s6-n3-cor-1 .statement tag=01S3}

Cho B là một không gian tôpô và cho $b$ là một điểm của B. Cho E là một phủ đơn liên của B. Với mọi điểm $x$ của $E_b$, không gian có điểm gốc $(E, x)$ là một phủ phổ quát của $(B, b)$.

#### Mệnh đề 4 {#ta-i-s6-prop-4 .statement tag=01S4}

Tích của hai không gian đơn liên, trong đó một không gian là địa phương liên thông, là một không gian đơn liên.

Cho X và Y là các không gian đơn liên, và giả sử rằng Y là địa phương liên thông. Không gian $X\times Y$ là liên thông, vì X và Y đều như vậy (I, p. 124). Cho $(Z, f)$ là một phủ khác rỗng của $X\times Y$; ta sẽ chứng minh rằng nó tầm thường hóa được. Theo hệ quả 2 của I, p. 70, chỉ cần chứng minh rằng với mọi điểm $z_0$ của Z, tồn tại một tiết diện liên tục $s$ của $f$ sao cho $s(f(z_0)) =z_0$. Vậy cho $z_0$ là một điểm của Z. Đặt $(x_0, y_0) =f(z_0)$. Không gian con $X\times  \{y_0\}$ của $X\times Y$ đồng phôi với X. Do đó phủ suy ra từ Z trên $X\times  \{y_0\}$ tầm thường hóa được và có một tiết diện liên tục $\sigma$ sao cho $\sigma (x_0, y_0) =z_0$. Tương tự, với mọi điểm $x$ của X, tồn tại một tiết diện liên tục $\tau_x$ của $f$ trên $\{x\}\times Y$ sao cho $\tau_x(x, y_0) =\sigma (x, y_0)$. Với $(x, y)\in X\times Y$, đặt $s(x, y) =\tau_x(x, y)$. Ánh xạ $s$ là một tiết diện của $f$, và ta có $s(x_0, y_0) =z_0$. Vì không gian Y liên thông và địa phương liên thông, theo định lý 1 của I, p. 35 suy ra rằng ánh xạ $s$ là liên tục.

#### Mệnh đề 5 {#ta-i-s6-prop-5 .statement tag=01S5}

Một không gian tôpô liên thông và địa phương liên thông sao cho giao của hai tập mở liên thông bất kỳ là liên thông thì là một không gian đơn liên.

Cho B là một không gian tôpô như vậy. Cho $(E, p)$ là một phủ của B, cho $x$ là một điểm của E và viết $b=p(x)$. Ta phải chứng minh rằng tồn tại một tiết diện liên tục $s$ của $p$ sao cho $s(b) =x$ (hệ quả 2, I, p. 70). Gọi $\mathscr{S}$ là tập hợp các cặp $(U, s_U)$ trong đó U là một tập con mở liên thông của B chứa $b$ và $s_U$ là một tiết diện liên tục của $p_U:\overset{-1}{p}(U)\rightarrow U$ sao cho $s_U(b) =x$. Tập hợp $\mathscr{S}$ không rỗng ( I, p. 34, mệnh đề 10). Cho $(U, s_U)$ và $(V, s_V)$ là các phần tử của $\mathscr{S}$. Khi đó $s_U|U\cap V$ và $s_V|U\cap V$ là các tiết diện liên tục của $p_{U\cap V}$ nhận giá trị $x$ tại $b$. Theo giả thiết, $U\cap V$ là liên thông; do đó $s_U|U\cap V =s_V|U\cap V$ (I, p. 34, hệ quả 1 của mệnh đề 11). Gọi A là hợp của các tập mở U khi $(U, s_U)$ chạy trên $\mathscr{S}$ và gọi $s: A\rightarrow E$ là ánh xạ duy nhất sao cho $s|U =s_U$ với mọi cặp $(U, s_U)\in \mathscr{S}$. Tập hợp A là mở và liên thông (TG, I, p. 81, mệnh đề 2), nó chứa $b$, và $s$ là một tiết diện liên tục của $p_A$ sao cho $s(b) =x$. Bây giờ chỉ còn đủ chứng minh rằng tập hợp A là đóng, điều này sẽ kéo theo rằng nó bằng B.

Cho $a$ là một điểm của B dính với A và cho V là một lân cận mở liên thông của $a$ sao cho phủ E tầm thường hóa được trên V. Tồn tại một điểm $c$ trong $A\cap V$ và một tiết diện liên tục $s_V$ của $p_V$ sao cho $s_V(c) =s(c)$. Gọi $A'$ là tập mở $A\cup V$. Vì $A\cap V$ là liên thông, tồn tại một tiết diện liên tục $s'$ của $p_{A'}$ kéo dài $s$ và $s_V($I, p. 35, hệ quả 3 của mệnh đề 11); cặp $(A', s')$ thuộc $\mathscr{S}$ và do đó $A'$ được chứa trong A. Suy ra $a$ thuộc A và A là đóng.

#### Hệ quả {#ta-i-s6-n3-cor-2 .statement tag=01S6}

Mọi khoảng của đường thẳng thực $\mathbf{R}$ đều đơn liên.

Thật vậy, các không gian con liên thông của $\mathbf{R}$ là các khoảng (TG, IV, p. 8, định lý 4) và giao của hai khoảng là một khoảng.

#### Ví dụ 2 {#ta-i-s6-n3-exa-2 .statement tag=01S7}

Không gian số có $n$ chiều $\mathbf{R}^n$ (TG, VI, p. 1) là đơn liên. Thật vậy, đó là một tích của các không gian đơn liên và địa phương liên thông (I, p. 126, mệnh đề 4 và hệ quả của mệnh đề 5 ở trên). Điều tương tự cũng đúng với mọi ô mở hoặc đóng trong $\mathbf{R}^n$. Một hình hộp song song, một quả cầu Euclid, mở hoặc đóng, trong $\mathbf{R}^n$ đều đơn liên vì chúng đồng phôi với một ô (TG, VI, p. 10, mệnh đề 2 và I, p. 124, ví dụ).

#### Mệnh đề 6 {#ta-i-s6-prop-6 .statement tag=01S8}

Cho X là một không gian tôpô. Cho $U_1$ và $U_2$ là các không gian con mở ( tương ứng đóng) của X sao cho $X = U_1\cup U_2$. Giả sử rằng $U_1$ và $U_2$ đơn liên và giao của chúng $U_1\cap U_2$ liên thông và khác rỗng. Khi đó không gian X là đơn liên.

Cho $(E, p)$ là một phủ của X và cho $y$ là một điểm của E. Chỉ cần chứng minh rằng tồn tại một tiết diện liên tục $s$ của $p$ sao cho $s(p(y)) =y$ (I, p. 70, hệ quả 2 của mệnh đề 1). Chẳng hạn giả sử rằng $p(y)$ thuộc $U_1$. Khi đó tồn tại một tiết diện liên tục $s_1: U_1\rightarrow E$ của $p_{U_1}$ sao cho $s_1(p(y)) =y$. Cho $x$ là một điểm của $U_1\cap U_2$; tồn tại một tiết diện liên tục $s_2$ của $p_{U_2}$ sao cho $s_2(x) =s_1(x)$. Theo hệ quả 3 của mệnh đề 11 của I, p. 34, tồn tại một tiết diện liên tục $s$ của $p$ kéo dài cả $s_1$ lẫn $s_2$.

#### Ví dụ 3 {#ta-i-s6-n3-exa-3 .statement tag=01S9}

Với $n\geqslant 2$, mặt cầu $\mathbf{S}_n$ (TG, VI, p. 10) là đơn liên. Thật vậy, mặt cầu $\mathbf{S}_n$ là hợp của hai bán cầu đóng đồng phôi với $\mathbf{B}_n$ mà giao của chúng đồng phôi với $\mathbf{S}_{n-1}($xem TG, VI, p. 12). Với $n\geqslant 2$, mặt cầu $\mathbf{S}_{n-1}$ liên thông, do đó mệnh đề được chứng minh.

Mặt khác, đường tròn $\mathbf{S}_1$ không đơn liên. Thật vậy, ánh xạ liên tục $p:\mathbf{R}\rightarrow \mathbf{S}_1$ được xác định bởi $p(\theta ) =$ (cos $\theta$, sin $\theta$ ) làm cho $\mathbf{R}$ thành một phủ liên thông của $\mathbf{S}_1$ có bậc vô hạn, do đó không tầm thường hóa được.

#### Ví dụ 4 {#ta-i-s6-n3-exa-4 .statement tag=01SA}

Cho E là một không gian vectơ hữu hạn chiều có chiều $n$ trên $\mathbf{R}$ và cho F là một không gian con afin của E có đối chiều $p\geqslant 3$. Tập hợp $\mathbf{R}^p-\{0\}$ đồng phôi với $\mathbf{R}\times \mathbf{S}_{p-1}$ (TG, VI, p. 10, hệ quả 2), và vì vậy là đơn liên, vì $\mathbf{R}$ và $\mathbf{S}_{p-1}$ liên thông địa phương và đơn liên (I, p. 126, mệnh đề 4). Do đó tập hợp E-F, đồng phôi với $\mathbf{R}^{n-p}\times$ $(\mathbf{R}^p-\{0\})$, là đơn liên (loc. cit.).

#### Mệnh đề 7 {#ta-i-s6-prop-7 .statement tag=01SB}

Cho X là một không gian tôpô. Cho $U_1$ và $U_2$ là các không gian con liên thông mở ( tương ứng đóng) của X sao cho $X = U_1\cup$ $U_2$. Nếu không gian X là đơn liên, thì $U_1\cap U_2$ liên thông.

Đặt $U = U_1\cap U_2$ và giả sử, để đi đến mâu thuẫn, rằng không gian U không liên thông. Ta sẽ xây dựng một phủ liên thông của X có bậc vô hạn; một phủ như vậy không tầm thường hóa được.

Theo giả thiết, tập hợp U là hợp của hai tập hợp rời nhau, không rỗng A và B, mở (tương ứng là đóng) trong X. Với $i\in  \{1,2\}$, cho $Y_i$ là $U_i$-không gian $(U_i\times \mathbf{Z}$, pr$_1)$ và cho $Z_i$ là không gian con $U\times \mathbf{Z}$ của $Y_i$. Ánh xạ $h: Z_1\rightarrow Z_2$ được xác định bởi

$(x, n)$ nếu $x\in A$ và $n\in \mathbf{Z}$

$$
h(x, n) =
$$

$(x, n+ 1)$ nếu $x\in B$ và $n\in \mathbf{Z}$

là một đồng phôi. Cho Y là không gian thu được bằng cách dán $Y_1$ và $Y_2$ dọc theo $Z_1$ và $Z_2$ bằng đồng phôi $h$ (TG, I, p. 17).

Với $i\in  \{1,2\}$, ánh xạ chính tắc $g_i$ từ $Y_i$ vào Y là một đồng phôi của $Y_i$ lên một tập con mở (tương ứng là đóng) của Y (loc. cit., mệnh đề 9). Với mọi số nguyên $n\in \mathbf{Z}$, các tập hợp $g_i(U_i\times  \{n\})$, $i\in  \{1,2\}$, đều liên thông; vì A và B không rỗng, $g_1(U_1\times \{n\})$ cắt $g_2(U_2\times  \{n\})$ và $g_2(U_2\times  \{n+1\})$. Suy ra không gian Y là liên thông (TG, I, p. 81, hệ quả).

Với $x\in U$ và $n\in \mathbf{Z}$, ta có (pr$_1\circ h$)$(x, n) =x=$ pr$_1(x, n)$. Do đó tồn tại một ánh xạ liên tục duy nhất $p: Y\rightarrow X$ sao cho $p\circ g_i=$ pr$_1$ với $i\in  \{1,2\}$. Hãy chứng minh rằng X-không gian $(Y, p)$ là một phủ. Theo phép dựng, các thớ của ánh xạ $p$ đẳng cấu với không gian rời rạc $\mathbf{Z}$.

Với $i\in  \{1,2\}$, ánh xạ $g_i$ xác định, bằng cách chuyển qua các không gian con, một đẳng cấu của các $U_i$-không gian từ $U_i\times \mathbf{Z}$ lên $\overset{-1}{p}(U_i)$.

Theo định nghĩa của không gian Y, tồn tại một ánh xạ duy nhất $k$ từ $(X-A)\times \mathbf{Z}$ vào Y sao cho $k(x, n) =g_1(x, n)$ với $x\in (U_1-A)\times \mathbf{Z}$ và $k(x, n) =g_2(x, n-1)$ với $x\in (U_2-A)\times \mathbf{Z}$; đó là một đẳng cấu các không gian trên X-A từ $(X-A)\times \mathbf{Z}$ lên $\overset{-1}{p}(X-A)$. Tương tự, tồn tại một ánh xạ duy nhất $k'$ từ $(X-B)\times \mathbf{Z}$ vào Y trùng với $g_1$ trên $(U_1-B)\times \mathbf{Z}$ và với $g_2$ trên $(U_2-B)\times \mathbf{Z}$ và đó là một đẳng cấu các không gian trên X-B từ $(X-B)\times \mathbf{Z}$ lên $\overset{-1}{p}(X-B)$.

Điều này chứng tỏ rằng không gian trên X $(Y, p)$ tầm thường hóa được trên các tập con $U_1,U_2$, X-A và X-B. Ta có $U_1\cup U_2= X$; nếu $U_1$ và $U_2$ mở trong X, điều này chứng tỏ rằng $(Y, p)$ là một phủ của X. Điều tương tự cũng đúng khi $U_1$ và $U_2$ đóng trong X, vì khi đó X-A và X-B là những tập con mở của X mà hợp là X. Như vậy mệnh đề được chứng minh.

#### Hệ quả {#ta-i-s6-n3-cor-3 .statement tag=01SC}

Cho X là một không gian tôpô đơn liên và A là một tập con liên thông của X. Nếu phần bù của A là liên thông, thì biên của nó cũng liên thông.

Gọi $X_1$ và $X_2$ lần lượt là các bao đóng của A và của X-A. Các tập hợp $X_1$ và $X_2$ là đóng và liên thông (TG, I, p. 81, mệnh đề 1); ta có $X_1\cup X_2= X$ và giao của chúng $X_1\cap X_2$ bằng biên của A. Khi đó chỉ cần áp dụng mệnh đề 7.

### 4. Tích của một Không gian với một Không gian Đơn liên

#### Mệnh đề 8 {#ta-i-s6-prop-8 .statement tag=01SD}

Cho B là một không gian tôpô. Cho T là một không gian đơn liên và địa phương liên thông. Cho E là một phủ của $B\times T$, với phép chiếu $p$, và cho $t$ là một điểm của T. Ký hiệu $E_t$ là không gian $\overset{-1}{p}(B\times  \{t\})$; được trang bị ánh xạ $p_t=$ pr$_1\circ p|E_t: E_t\rightarrow B$, nó là một phủ của B. Khi đó tồn tại một $(B\times T)$-đẳng cấu duy nhất của phủ $(E_t\times T, p_t\times$ Id$_T)$ lên phủ E, ánh xạ $(x, t)$ thành $x$ với mọi $x\in E_t$.

Có thể giả sử rằng B không rỗng. Cho $x$ là một điểm của $E_t$. Theo mệnh đề 3 của I, p. 125 áp dụng cho phủ E và cho ánh xạ liên tục $T\rightarrow B\times T,u\mapsto (p_t(x), u)$, tồn tại một ánh xạ liên tục duy nhất $f_x: T\rightarrow E$ sao cho $f_x(t) =x$ và $p(f_x(u)) =$ $(p_t(x), u)$ với mọi $u\in T$. Cho $h: E_t\times T\rightarrow E$ là ánh xạ được xác định bởi $h(x, u) =f_x(u)$. Ta có $h(x, t) =x$ và $p\circ h=p_t\times$ Id$_T$. Ánh xạ $h$ là một phép nâng lên E của ánh xạ $p_t\times$ Id$_T$. Hạn chế của $h$ trên $E_t\times  \{t\}$ là liên tục, cũng như hạn chế của $h$ trên $\{x\} \times T$ với mọi điểm $x$ của $E_t$. Vì không gian T liên thông địa phương, ánh xạ $h$ là liên tục ( I, p. 37, hệ quả 1 của định lý 1).

Cho $b$ là một điểm của B. Theo phép dựng, ánh xạ $h$ cảm sinh một song ánh từ thớ $\overset{-1}{p_{t}}(b)\times  \{t\}$ của $E_t\times T$ lên thớ $\overset{-1}{p}(b, t)$ của E tại $(b, t)$. Vì không gian T liên thông và liên thông địa phương, ánh xạ $h$ là song ánh (I, p. 84, hệ quả của mệnh đề 7). Do đó nó là một $(B\times T)$-đẳng cấu (I, p. 30, hệ quả 2 của mệnh đề 6).

Cho $h'$ là một $(B\times T)$-đẳng cấu từ phủ $(E_t\times T, p_t\times$ Id$_T)$ lên phủ E sao cho nó ánh xạ $(x, t)$ thành $x$ với mọi điểm $x\in E_t$. Với mọi $x\in E_t$, các ánh xạ $u\mapsto h(x, u)$ và $u\mapsto h'(x, u)$ là bằng nhau (I, p. 34, hệ quả 1 của mệnh đề 11). Vậy $h=h'$.

#### Hệ quả 1 {#ta-i-s6-prop-8-cor-1 .statement tag=01SE}

Dưới các giả thiết của mệnh đề 8, nếu $t$ và $t'$ là hai điểm của T, thì các phủ $E_t$ và $E_{t'}$ là B-đẳng cấu.

#### Hệ quả 2 {#ta-i-s6-prop-8-cor-2 .statement tag=01SF}

Dưới các giả thiết của mệnh đề 8, cho $(E, p)$ và $(E', p')$ là các phủ của $B\times T$ và cho $k: E_t\rightarrow E'_t$ là một B-cấu xạ. Tồn tại một $(B\times T)$-cấu xạ duy nhất $\widetilde{k}: E\rightarrow E'$ mở rộng $k$. Nếu $k$ là một B-đẳng cấu, thì $\widetilde{k}$ là một $(B\times T)$-đẳng cấu.

Theo mệnh đề 8, có thể giả sử rằng tồn tại các phủ F và $F'$ của B sao cho E và $E'$ lần lượt là các $(B\times T)$-không gian $F\times T$ và $F'\times T$. Khi đó có $E_t= F\times  \{t\},E'_t= F'\times  \{t\}$ và ánh xạ $k$ được viết là $(x, t)\mapsto (k'(x), t)$, trong đó $k'$ là một B-cấu xạ từ F vào $F'$. Ánh xạ $k'\times$Id$_T$ là một $B\times T$-cấu xạ mở rộng $k$; nó là một đẳng cấu nếu $k$ là một đẳng cấu.

Cho $\widetilde{k}: E\rightarrow E'$ là một $(B\times T)$-cấu xạ mở rộng $k$. Lấy $x$ là một điểm của F. Ký hiệu bởi $q$ phép chiếu của F và đặt $b=q(x)$. Các ánh xạ $u\mapsto \widetilde{k}(x, u)$ và $u\mapsto (k'(x), u)$ là các phép nâng trong $E'$ của ánh xạ $u\mapsto (b, u)$ từ T vào $B\times T$. Chúng trùng nhau tại $t$. Vì không gian T liên thông, chúng bằng nhau. Do đó, $\widetilde{k}$ là $(B\times T)$-cấu xạ $k'\times$ Id$_T: F\times T\rightarrow F'\times T$.

#### Hệ quả 3 {#ta-i-s6-prop-8-cor-3 .statement tag=01SG}

Cho B và $B'$ là các không gian tôpô, cho T là một không gian tôpô đơn liên và địa phương liên thông. Cho $f: B'\times T\rightarrow B$ là một ánh xạ liên tục và cho E là một phủ của B. Với một điểm $t$ của T và một phép nâng liên tục $g_t: B'\times \{t\} \rightarrow E$ của $f|B'\times  \{t\}$ vào E, tồn tại một phép nâng liên tục duy nhất $g$ của $f$ vào E mở rộng $g_t$.

Theo mệnh đề 3 của I, p. 9, vấn đề là chứng minh rằng mọi tiết diện liên tục của $f^*(E)$ trên $B'\times  \{t\}$ đều mở rộng duy nhất thành một tiết diện liên tục của $f^*(E)$. Nhưng điều này suy ra từ hệ quả 2 áp dụng cho các phủ $(B'\times T$, Id$_{B'\times T})$ và $f^*E$ của $B'\times T$.

#### Nhận xét {#ta-i-s6-n4-rem-1 .statement tag=01SH}

Hãy giữ lại các giả thiết và ký hiệu của mệnh đề 8. Cho G là một nhóm tôpô rời rạc. Giả sử rằng E là một phủ chính của nhóm G. Nếu các phủ $E_t$ của B và $E_t\times T$ của $B\times T$ được trang bị các cấu trúc phủ chính của nhóm G suy ra từ cấu trúc của E (I, p. 92, ví dụ 1 và 4), thì các phủ E và $E_t\times T$ là các phủ chính đẳng cấu. Thật vậy, gọi $h: E_t\times T\rightarrow E$ là $(B\times T)$-cấu xạ duy nhất sao cho $h(x, t) =x$ với mọi $x\in E_t$. Với mọi phần tử $g$ của G, ánh xạ $(x, u)\mapsto h(x\cdot g, u)\cdot g^{-1}$ là một $(B\times T)$-cấu xạ biến $(x, t)$ thành $x$ với mọi $x\in E_t$, do đó bằng $h$. Điều này chứng minh rằng $h$ là một $(B\times T)$-cấu xạ của các phủ chính.

Đặc biệt, dưới các giả thiết trên, các phủ chính $E_t$ và $E_{t'}$ là đẳng cấu, với $t'\in T$. Người ta chứng minh tương tự rằng nếu, trong hệ quả 2, E và $E'$ là các phủ chính của nhóm G và nếu $k$ là một B-đẳng cấu của các phủ chính của nhóm G$,\widetilde{k}$ là một $(B\times T)$-đẳng cấu của các phủ chính.

#### Mệnh đề 9 {#ta-i-s6-prop-9 .statement tag=01SI}

Cho B là một không gian tôpô và cho $(E, p)$ là một phủ của B. Cho T là một không gian tôpô đơn liên, liên thông địa phương và compact địa phương. Ký hiệu $\widetilde{p}:\mathscr{C}_c(T; E)\rightarrow \mathscr{C}_c(T; B)$ là ánh xạ $g\mapsto p\circ g$. Cho $t$ là một điểm của T. Ký hiệu $e_E:\mathscr{C}_c(T; E)\rightarrow E$ là ánh xạ gán cho $g\in \mathscr{C}_c(T; E)$ phần tử $g(t)$, và $e_B:\mathscr{C}_c(T; B)\rightarrow B$ là ánh xạ gán cho $f\in \mathscr{C}_c(T; B)$ phần tử $f(t)$.

Hình vuông

$\mathscr{C}_c(T; E)^{e_E}$ E

$\widetilde{p}p$

$\mathscr{C}_c(T; B)^{e_B}$ B là Đề-các.

Trước hết hãy chứng minh một bổ đề.

#### Bổ đề {#ta-i-s6-n4-lem-1 .statement tag=01SJ}

Cho X, Y, Z là các không gian tôpô và cho $g: Y\rightarrow Z$ là một ánh xạ liên tục.

a) Ánh xạ $f\mapsto g\circ f$ từ $\mathscr{C}_c(X; Y)$ vào $\mathscr{C}_c(X; Z)$ là liên tục.

b) Nếu không gian tôpô Z là tách biệt, thì ánh xạ $h\mapsto h\circ g$ từ $\mathscr{C}_c(Z; X)$ vào $\mathscr{C}_c(Y; X)$ là liên tục.

Cho K là một tập con compact của X, U là một tập con mở của Z và $f$ là một ánh xạ liên tục từ X vào Y, để có $(g\circ f)(K)\subset U$, điều kiện cần và đủ là có $f(K)\subset \overset{-1}{g}(U)$. Do đó mệnh đề thứ nhất suy ra từ định nghĩa của tôpô hội tụ compact (TG, X, p. 26, định nghĩa 1).

Tương tự, cho K là một tập con compact của Y và U là một tập con mở của X. Vì Z được giả sử là tách biệt nên tập hợp $g(K)$ là compact (TG, I, p. 63, hệ quả 1). Nếu $h$ là một ánh xạ từ Z vào X, điều kiện $(h\circ g)(K)\subset U$ không gì khác hơn là điều kiện $h(g(K))\subset U$, do đó suy ra mệnh đề thứ hai.

Bây giờ hãy chứng minh mệnh đề 9. Theo bổ đề, ánh xạ $\widetilde{p}$ là liên tục; theo nhận xét 1 của TG, X, p. 27, các ánh xạ $e_E$ và $e_B$ là liên tục. Với mọi ánh xạ $g\in \mathscr{C}_c(T; E)$, ta có

$$
(p\circ e_E)(g) =p(g(t)) = (p\circ g)(t) =\widetilde{p}(g)(t) = (e_B\circ \widetilde{p})(g)
$$

do đó biểu đồ hình vuông của mệnh đề là giao hoán.

Cho $\varphi :\mathscr{C}_c(T; E)\rightarrow \mathscr{C}_c(T; B)\times_BE$ là ánh xạ liên tục được xác định bởi $\varphi (g) = (p\circ g, g(t))$ với mọi $g\in \mathscr{C}_c(T; E)$. Theo mệnh đề 3 của I, p. 125, nó là song ánh. Thực vậy, với mọi cặp $(f, x)\in \mathscr{C}_c(T; B)\times_BE,\varphi^{-1}(f, x)$ là nâng liên tục duy nhất $g$ của $f$ lên E sao cho $g(t) =x$. Vì không gian T là compact địa phương, ánh xạ $\psi : (\mathscr{C}_c(T; B)\times_BE)\times T\rightarrow B$ được xác định bởi $\psi ((f, x), u) =f(u)$ là liên tục (TG, X, p. 28, hệ quả 1). Theo hệ quả 3 ở trên, ánh xạ $\psi$ có một nâng liên tục duy nhất $\theta : (\mathscr{C}_c(T; B)\times_B$ $E)\times T\rightarrow E$ sao cho $\theta ((f, x), t) =x$ với $(f, x)\in \mathscr{C}_c(T; B)\times_BE$. Do đó $\theta ((f, x), u) =\varphi^{-1}(f, x)(u)$ với $(f, x)\in \mathscr{C}_c(T; B)\times_BE$ và $u\in T$. Theo định lý 3 của TG, X, p. 28, ánh xạ $(f, x)\mapsto \theta ((f, x),\cdot )$ từ $\mathscr{C}_c(T; B)\times_BE$ vào $\mathscr{C}_c(T; E)$ là liên tục, nghĩa là $\varphi^{-1}$ là liên tục.

Vậy, ánh xạ $\varphi$ là một đồng phôi của $\mathscr{C}_c(T; E)$ lên tích thớ $\mathscr{C}_c(T; B)\times_BE$, do đó có mệnh đề (I, p. 8, mệnh đề 2).

### 5. Các nhóm đồng phôi của các không gian đơn liên

Cho X là một không gian tôpô liên thông khác rỗng và cho G là một nhóm rời rạc tác động liên tục bên trái trên X; ký hiệu $e$ là phần tử đơn vị của G. Cho M là một tập con của X sao cho $G\cdot M = X$. Đặt

$$
S =\{g\in G|g\cdot M\cap M=\not\emptyset \}
$$

Khi đó $e\in S$ và $S = S^{-1}$.

Với mọi $x\in X$, ký hiệu $E_x$ là tập hợp các $g\in G$ sao cho $x\in g\cdot M$. Cho $g, h\in E_x$; khi đó $g\cdot M\cap h\cdot M=\not\emptyset$, nên $g^{-1}h\in S$. Đặc biệt, với mọi $x\in M$, ta có $e\in E_x$ do đó $E_x\subset S$.

Ta đặt một trong hai giả thiết sau:

(i) Tập hợp M là mở;

(ii) Tập hợp M là đóng và phủ $(g\cdot M)_{g\in G}$ của X là hữu hạn địa phương.

#### Bổ đề 2 {#ta-i-s6-lem-2 .statement tag=01SK}

Với mọi điểm $x\in X$, ánh xạ $\mu_x: E_x\times M\rightarrow X$ cho bởi $(g, u)\mapsto g\cdot u$ là ngặt theo nghĩa phổ quát, và ảnh của nó $E_x\cdot M$ là một lân cận của $x$ trong X. Đặc biệt, $S\cdot M$ là một lân cận của M.

Dưới giả thiết (i), ánh xạ $\mu_x$ là mở, vì $E_x\times M$ là mở trong $G\times M$. Do đó ảnh của nó là mở trong X.

Bây giờ giả sử giả thiết (ii) được thỏa mãn. Ánh xạ $\mu_x$ là thực sự (TG, I, p. 6, mệnh đề 4, và p. 75, định lý 1), nên ngặt theo nghĩa phổ quát (I, p. 20, hệ quả 11). Hơn nữa, $(G-E_x)\cdot M$ là một tập con đóng của X không chứa $x$, nên $E_x\cdot M$ là một lân cận của $x$.

Khẳng định cuối cùng suy ra từ việc $E_x\subset S$ nếu $x\in M$.

#### Bổ đề 3 {#ta-i-s6-lem-3 .statement tag=01SL}

Nhóm G được sinh bởi S.

Gọi H là nhóm con của G sinh bởi S. Đặt $U = H\cdot M$; nhận thấy rằng U là hợp của các tập con có dạng $h\cdot (S\cdot M)$, với $h\in H$. Vì $S\cdot M$ là một lân cận của M (bổ đề 2), nên U là một lân cận của $H\cdot M = U$; suy ra U là mở trong X. Cho $g, g'\in G$ sao cho $g\cdot U\cap g'\cdot U=\not\emptyset$; lấy $h, h'\in H$ và $x, x'\in M$ sao cho $gh\cdot x=g'h'\cdot x'$; khi đó $h^{-1}g^{-1}g'h'\cdot x'=x$, nên $h^{-1}g^{-1}g'h'\in S$; đặc biệt, $g^{-1}g'\in H$. Khi $g$ chạy qua một hệ đại biểu của các lớp trái theo modulo H, thì các tập $g\cdot U$ do đó rời nhau từng đôi một; vì $G\cdot M = X$, chúng phủ X. Do X liên thông, suy ra $(G : H) = 1$, do đó H = G.

Gọi T là tập hợp các cặp $(s, t)$ phần tử của G sao cho $M\cap s\cdot$ $M\cap st\cdot M=\not\emptyset$; nếu $(s, t)\in T$, thì $s,t$ và $st$ thuộc S. Gọi F là nhóm $F(S,\mathbf{r})$ được xác định bởi tập sinh S và bởi tập $\mathbf{r}$ các hệ thức $str^{-1}$ với $r, s, t\in S$ sao cho $(s, t)\in T$ và $r=st$; ký hiệu $\varepsilon$ là phần tử đơn vị của nó và $\varphi : F\rightarrow G$ là đồng cấu chính tắc (A, I, p. 86, mệnh đề 9). Nếu $s\in S$, ta sẽ ký hiệu bởi $x_s$ phần tử của F, là ảnh của $s$ dưới ánh xạ chính tắc từ S vào F; với mọi $s\in S$, ta có $\varphi (x_s) =s$. Vì vậy đồng cấu $\varphi$ là toàn ánh (bổ đề 3). Với $(s, t)\in T$ và $r=st$, ta có $x_r=x_sx_t$; do đó $x_e=\varepsilon$, vì $(e, e)\in T$; với mọi $s\in S$, ta cũng có $x_{s^{-1}}=x^{-1}_s$ vì $(s, s^{-1})\in T$.

Trang bị cho tập hợp F tôpô rời rạc và gọi Z là không gian tôpô $F\times M$, được trang bị phép toán của F cho bởi $(\gamma ,(g, x))\mapsto$ $(\gamma g, x)$, với $\gamma$ và $g\in$ F và $u\in$ M. Cho $(g_1, u_1)$ và $(g_2, u_2)$ là các phần tử của Z; ta sẽ nói rằng $(g_1, u_1)$ đồng dư với $(g_2, u_2)$ nếu tồn tại $s\in S$ sao cho $g_2=g_1\cdot x_s$ và $s\cdot u_2=u_1$.

#### Bổ đề 4 {#ta-i-s6-lem-4 .statement tag=01SM}

Quan hệ “$(g_1, u_1)$ đồng dư với $(g_2, u_2)$” là một quan hệ tương đương trong Z, tương thích với phép toán của F.

Quan hệ này là phản xạ, vì ta có $x_e=\varepsilon$. Cho $(g_1, u_1)$ và $(g_2, u_2)$ là các phần tử của Z sao cho $(g_1, u_1)$ đồng dư với $(g_2, u_2)$. Lấy $s\in S$ sao cho $g_2=g_1x_s$ và $s\cdot u_2=u_1$; vì $x_{s^{-1}}=x^{-1}_s$, ta có $g_1=g_2x_{s^{-1}}$ và $u_2=s^{-1}\cdot u_1$, do đó $(g_2, u_2)$ đồng dư với $(g_1, u_1)$; bởi vậy, quan hệ này là đối xứng. Cuối cùng, hãy chỉ ra rằng nó là bắc cầu. Cho $(g_1, u_1)$, $(g_2, u_2)$ và $(g_3, u_3)$ là các điểm của Z sao cho $(g_1, u_1)$ và $(g_2, u_2)$ đồng dư, và đồng thời $(g_2, u_2)$ và $(g_3, u_3)$ cũng đồng dư. Cho $s$ và $t$ trong S sao cho một mặt $g_2=g_1x_s$ và $s\cdot u_2=u_1$, và mặt khác $g_3=g_2x_t$ và $t\cdot u_3=u_2$. Ta có $u_1=s\cdot u_2=st\cdot u_3$, nên $u_1\in M\cap s\cdot M\cap st\cdot M$, điều đó chỉ ra rằng $(s, t)$ thuộc T và $st$ thuộc S. Khi đó ta có $g_3=g_2x_t=g_1x_sx_t=g_1x_{st}$ và $u_1=st\cdot u_3$; do đó, $(g_1, u_1)$ và $(g_3, u_3)$ đồng dư. Vậy quan hệ "đồng dư" là một quan hệ tương đương trong Z. Nó tương thích với phép toán của F trong Z.

Cho Y là không gian tôpô thương của Z đối với quan hệ tương đương đã định nghĩa ở trên. Ký hiệu $\pi : Z\rightarrow Y$ là ánh xạ chính tắc. Ký hiệu thêm $q: Z\rightarrow X$ là ánh xạ được cho bởi $(g, x)\mapsto \varphi (g)\cdot x$; nó là toàn ánh (bổ đề 3). Bằng cách chuyển qua thương, ánh xạ $q$ suy ra một ánh xạ liên tục và toàn ánh $p: Y\rightarrow X$; theo bổ đề 4, phép toán của F trong Z suy ra một phép toán liên tục của F trong Y sao cho $p(g\cdot y) =\varphi (g)\cdot p(y)$ với mọi $g\in F$ và mọi $y\in Y$. Đặc biệt, nhóm N = Ker($\varphi$ ) tác động liên tục trên X-không gian $(Y, p)$.

#### Bổ đề 5 {#ta-i-s6-lem-5 .statement tag=01SN}

Nếu M liên thông, không gian Y liên thông.

Cho $g\in F$ và $s\in S$. Gọi $u$ và $v$ là các phần tử của M sao cho $v=s\cdot u$; do đó $\pi (g, v) =\pi (gx_s, u)$, và các tập $\pi (\{g\} \times M)$ và $\pi (\{gx_s\} \times M)$ của Y có một điểm chung. Vì chúng liên thông, chúng được chứa trong cùng một thành phần liên thông của Y. Vì S là một tập con đối xứng của nhóm G, và vì $x_{s^{-1}}=x^{-1}_s$ với mọi $s\in S$, mọi phần tử $g$ của F đều có dạng $x_{s_1}. . . x_{s_n}$, trong đó $n\in \mathbf{N}$ và $s_1, . . . , s_n$ là các phần tử của S. Theo quy nạp trên $n$, các tập $\pi (\{e\} \times M)$ và $\pi (\{g\} \times M)$ được chứa trong cùng một thành phần liên thông của Y, với mọi $g\in F$. Do đó Y liên thông.

#### Bổ đề 6 {#ta-i-s6-lem-6 .statement tag=01SO}

Với mọi $x\in X$, nhóm N tác động trung thành và bắc cầu trên thớ $\overset{-1}{p}(x)$.

Vì $p$ là toàn ánh, thớ $\overset{-1}{p}(x)$ không rỗng. Cho $y, y'\in$ $\overset{-1}{p}(x)$; hãy chứng minh rằng tồn tại một phần tử duy nhất $n\in$ N sao cho $n\cdot y=y'$. Cho $g, h\in$ F và cho $u, v\in$ M sao cho $y=\pi (g, u)$ và $y'=\pi (h, v)$. Đặt $s=\varphi (g^{-1}h)$. Vì $x=\varphi (g)\cdot u=\varphi (h)\cdot v$, ta có $u=s\cdot v$, do đó $s\in S$. Suy ra $\varphi (h) =\varphi (gx_s)$, nên tồn tại $n\in N$ sao cho $h=ngx_s$. Khi đó,

$$
y'=\pi (h, v) =\pi (ngx_s, v) =n\cdot \pi (gx_s, v) =n\cdot \pi (g, s\cdot v) =n\cdot y
$$

Cho $n'$ là một phần tử của N sao cho $n'\cdot y=y'$. Ta có $n'\cdot \pi (g, u) =n\cdot \pi (g, u)$, do đó $\pi (n'g, u) =\pi (ng, u)$. Do đó, tồn tại $t\in S$ sao cho $n'g=$ $ngx_t$; quan hệ này kéo theo $\varphi (x_t) =e$, do đó $t=e$ và $n=n'$.

#### Bổ đề 7 {#ta-i-s6-lem-7 .statement tag=01SP}

Được trang bị với tác động của N, X-không gian $(Y, p)$ là một phủ trái chính. Nó tầm thường hóa được trên M.

Cho $x\in X$; cố định một phần tử $g\in E_x$ và một phần tử $\overline{g}\in F$ sao cho $\varphi (\overline{g}) =g$. Ta ký hiệu bởi $\mu_x: E_x\times M\rightarrow X$ ánh xạ xác định bởi $(h, u)\mapsto h\cdot u$.

Cho $n\in N$, cho $h, k\in E_x$ và cho $u, v\in M$ sao cho $h\cdot u=k\cdot v$; đặt $s=g^{-1}h,t=h^{-1}k$ và $r=st=g^{-1}k$. Vì $x$ thuộc $g\cdot M\cap h\cdot M\cap k\cdot M$, cặp $(s, t)$ thuộc T, do đó $x_sx_t=x_r$. Vậy

$$
\pi (ngx_r, v) =\pi (ngx_sx_t, v) =\pi (ngx_s, t\cdot v) =\pi (ngx_s, u)
$$

Do đó tồn tại một ánh xạ duy nhất $\theta : N\times (E_x\cdot M)\rightarrow Y$ sao cho $\theta (n, h\cdot u) =\pi (ngx_{g^{-1}h}, u)$ với mọi $n\in N$, mọi $h\in E_x$ và mọi $u\in M$. Ta có

$$
p(\theta (n, h\cdot u)) =p(\pi (ngx_s, u)) =q(ngx_s, u) =\varphi (ngx_s)\cdot u=gs\cdot u=h\cdot u
$$

Hơn nữa, với $n, n'\in N$ và $y\in E_x\cdot M$, ta có $\theta (n'n, y) =n'\cdot \theta (n, y)$. Ánh xạ $\theta ': N\times (E_x\times M)\rightarrow Y$ được xác định bởi $\theta '(n,(h, u)) =\theta (n, \mu_x(h, u))$ là liên tục; vì ánh xạ $\mu_x$ là ngặt phổ dụng (I, p. 133, Bổ đề 2), ánh xạ $\theta$ là liên tục. Đó là một song ánh từ $N\times (E_x\cdot M)$ lên không gian con $Y\times_X(E_x\cdot M)$ của Y (Bổ đề 6).

Cho $z= (k, v)\in Z$ và $(h, u)\in E_x\times M$ sao cho $q(k, v) =\mu_x(h, u)$. Đặt $s$ = $h^{-1}\varphi (\overline{k})$; vì $\varphi (\overline{k})\cdot v$ = $h\cdot u$, ta có $s\in$ S. Khi đó đặt $\lambda '(z,(h, u)) =kx^{-1}_sx_{h^{-1}g}\overline{g}^{-1}$; ta có $\varphi (\lambda '(z,(h, u))) =$ $\varphi (\overline{k})s^{-1}h^{-1}gg^{-1}$ = $e$, do đó $\lambda '(z,(h, u))\in$ N. Như vậy một ánh xạ liên tục $\lambda ': Z\times_X(E_x\times M)\rightarrow N$ được xác định. Hơn nữa, với mọi $z$ và $(h, u)$ như trên, ta có

$$
\theta (\lambda '(z,(h, u)), h\cdot u) =\pi (kx^{-1}_sx_{h^{-1}g}\overline{g}^{-1}gx_{g^{-1}h}, u)
$$

$$
=\pi (kx^{-1}_s, u) =\pi (k, s^{-1}\cdot u) =\pi (k, v) =\pi (z)
$$

và $\lambda '(z,(h, u))$ là phần tử duy nhất $n$ của N sao cho $\theta (n, h\cdot u) =\pi (z)$. Đặc biệt tồn tại một ánh xạ duy nhất

$$
\lambda : Y\times_X(E_x\cdot M)\rightarrow N
$$

sao cho $\lambda (\pi (z), h\cdot u) =\lambda '(z,(h, u))$ với mọi $z\in Z$ và mọi $(h, u)\in$ $E_x\times M$ sao cho $q(z) =h\cdot u$. Nó là liên tục, vì ánh xạ $\mu_x$ là ngặt phổ dụng. Suy ra không gian $E_x\cdot M$-$Y_{E_x\cdot M}$ suy ra từ Y bằng thay đổi cơ sở, được trang bị phép toán của N, là một không gian sợi chính với nhóm N, khả tầm thường hóa.

Vậy bổ đề được chứng minh.

#### Mệnh đề 10 {#ta-i-s6-prop-10 .statement tag=01SQ}

Cho X là một không gian tôpô khác rỗng liên thông, cho G là một nhóm rời rạc tác động liên tục bên trái trên X, và cho M là một tập con của X sao cho $G\cdot M = X$. Ta đặt ra một trong hai giả thiết sau:

(i) Tập hợp M là mở;

(ii) Tập hợp M là đóng và phủ $(g\cdot M)_{g\in G}$ của X là hữu hạn địa phương.

Gọi S là tập hợp các phần tử $g\in G$ sao cho $M\cap g\cdot M=\not\emptyset$, gọi T là tập hợp các cặp $(s, t)\in S\times S$ sao cho $M\cap s\cdot M\cap st\cdot M=\not\emptyset$. Gọi F là nhóm $F(S,\mathbf{r})$ được xác định bởi tập phần tử sinh S và bởi tập $\mathbf{r}$ các hệ thức $str^{-1}$ với $r, s, t\in$ S sao cho $(s, t)\in$ T và $r$ = $st$; với $s\in S$, gọi $x_s$ là ảnh của $s$ dưới ánh xạ chính tắc từ S vào F. Tồn tại một đồng cấu nhóm duy nhất $\varphi : F\rightarrow G$ sao cho $\varphi (x_s) =s$ với mọi $s\in S$. Nó là toàn ánh; nó là một đẳng cấu nếu không gian X đơn liên, hoặc, nói chung hơn, nếu mọi phủ của X tầm thường hóa được trên M đều tầm thường hóa được.

Đồng cấu $\varphi$ là toàn ánh (I, p. 133, bổ đề 3). Với ký hiệu của No.$^o$ này, phủ Y của X là tầm thường hóa được, vì nó tầm thường hóa được trên M. Theo bổ đề 5, Y liên thông. Do đó, $p: Y\rightarrow X$ là một đồng phôi và nhóm N thu về phần tử đơn vị. Do đó, đồng cấu $\varphi : F\rightarrow G$ là một đẳng cấu nhóm.

#### Mệnh đề 11 {#ta-i-s6-prop-11 .statement tag=01SR}

Cho X là một không gian tôpô đơn liên và G là một nhóm rời rạc tác động liên tục bên phải trên X. Nếu nhóm con của G sinh bởi hợp của các nhóm ổn định của các điểm của X bằng G, thì không gian $X/G$ đơn liên.

Cho $(E, p)$ là một phủ của $X/G$. Cần chứng minh rằng, với mọi điểm $x$ của E, tồn tại một tiết diện liên tục $s$ của $p$ sao cho $s\circ p(x) =x($I, p. 70, hệ quả 2 của mệnh đề 1). Gọi $q: X\rightarrow X/G$ là ánh xạ chính tắc và chọn một điểm $y$ của X sao cho $q(y) =p(x)$. Vì không gian X đơn liên, tồn tại một ánh xạ liên tục $f: X\rightarrow E$ sao cho $f(y) =x$ và $p\circ f=q($I, p. 125, mệnh đề 3). Gọi $z$ là một điểm của X và $g$ là một phần tử của nhóm con của G ổn định $z$. Các ánh xạ $t\mapsto f(t)$ và $t\mapsto f(t\cdot g)$ từ X vào E là các nâng liên tục lên E của ánh xạ $q$ mà trùng nhau tại $t=z$. Vì không gian X liên thông, chúng bằng nhau (I, p. 34, hệ quả 1 của mệnh đề 11). Vì hợp của các nhóm con ổn định của các điểm của X sinh ra G, ta có $f(t\cdot g) =f(t)$ với mọi $t\in X$ và mọi $g\in G$. Chuyển qua thương, từ $f$ suy ra được một ánh xạ liên tục $s: X/G\rightarrow E$ là một tiết diện liên tục của $p$ sao cho $s(p(x)) =x$.

## BÀI TẬP {#ta-i-s6-exercises}

Xem [bài tập cho § 6](exercises/s6/).
