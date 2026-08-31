---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 2
section_title: Homotopie et chemins
lang: vi
source: ta-i-iv-fr
book_pages: TA III.256-TA III.289, TA III.330-TA III.333
pdf_pages: 0272-0305, 0346-0349
extraction: native
subsections:
    - "no": 1
      title: Chemins
      page: 256
      pdf_page: 272
    - "no": 2
      title: Espaces connexes par arcs
      page: 258
      pdf_page: 274
    - "no": 3
      title: Espaces localement connexes par arcs
      page: 260
      pdf_page: 276
    - "no": 4
      title: Liens entre connexité et connexité par arcs
      page: 264
      pdf_page: 280
    - "no": 5
      title: Applications continues par arcs
      page: 267
      pdf_page: 283
    - "no": 6
      title: Compléments sur les espaces topologiques compacts métrisables
      page: 269
      pdf_page: 285
    - "no": 7
      title: Propriétés topologiques de l’image d’un chemin
      page: 272
      pdf_page: 288
    - "no": 8
      title: Caractérisations de l’intervalle
      page: 274
      pdf_page: 290
    - "no": 9
      title: Chemins injectifs
      page: 282
      pdf_page: 298
    - "no": 10
      title: Relèvement de chemins
      page: 284
      pdf_page: 300
statements: 63
exercises: 14
content_sha256: 0511f216e8c3d5a83468e67c1c86443fe5797303afd05d91dd35fda0ca79473c
translated_from: content/en-mt/ta/III/02_s2_homotopie_et_chemins.md
source_lang: en-mt
translation_method: machine
source_content_sha256: cab9fc5ba5b92b75bbb3ee22fc440f67b9b9db559ed7fb0d29ade6a5d0fb5596
translation_model: gpt-5-6-mini
translation_run: translate-vi-bcd0abf2
glossary_version: 34
glossary_terms_sha256: 638215456b9bdd4013ef8576b421c2cba48e7159c7560a6814402dd0c4bf4d9b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ĐỒNG LUYẾN VÀ CÁC ĐƯỜNG

### 1. Các đường

#### Định nghĩa 1 {#ta-iii-s2-def-1 .statement tag=01WN}

Cho X là một không gian tôpô. Một đường trong X được gọi là một ánh xạ liên tục bất kỳ $c$ của $\mathbf{I}$ vào X. Điểm $c(0)$ được gọi là gốc, điểm $c(1)$ được gọi là số hạng của đường $c$. Một vòng trong X được gọi là một đường trong X mà gốc của nó bằng số hạng.

Cho $x$ và $y$ là các điểm của X. Ta nói rằng một đường $c$ trong X nối $x$ với $y$ nếu $x$ là gốc của nó và $y$ là số hạng của nó.

#### Định nghĩa 2 {#ta-iii-s2-def-2 .statement tag=01WO}

Cho X là một không gian tôpô. Ta nói rằng các đường $c$ và $d$ trong X là ghép kề nếu có $c(1) =d(0)$. Khi đó ta gọi đường ghép kề của $c$ và $d$ là đường $c*d$ được xác định bởi công thức:

$c(2t)$ for $0\leqslant t\leqslant 1/2$,

$$
(c*d)(t) = \tag{1}
$$

$d(2t-1)$ for $1/2\leqslant t\leqslant 1$.

Gốc của nó là gốc của $c$, số hạng của nó là số hạng của $d$.

Cho $c$ là một đường trong X; ta gọi đường đối với $c$ và ký hiệu bởi $\overline{c}$ là đường được xác định bởi $\overline{c}(t) =c(1-t)$ với $t\in \mathbf{I}$.

ta cóNếu $cc$và$*dd=$là hai đường ghép kề trong$\overline{d}*\overline{c}$. Với mọi đường $c$ trong X, ta cóX$,\overline{\overline{\overline{c}}d}=$và$c\overline{c.}$ là, và

#### Nhận xét 1 {#ta-iii-s2-n1-rem-1 .statement tag=01WP}

Cho X là một không gian tôpô và cho P là một không gian tôpô thu gọn thành một điểm. Đồng nhất $P\times \mathbf{I}$ với $\mathbf{I}$ bởi phép chiếu pr$_2$. Tập hợp $\mathscr{C}(P\times \mathbf{I}; X)$ các đồng luân giữa các ánh xạ (nhất thiết liên tục) từ P vào X khi đó được đồng nhất với tập hợp $\mathscr{C}(\mathbf{I}; X)$ các đường trong X. Với một đồng luân nối ánh xạ hằng có ảnh $x$ với ánh xạ hằng có ảnh $y$ tương ứng một đường có gốc $x$ và số hạng $y$. Các sự đồng nhất trước đó tương thích với các khái niệm ghép kề và chuyển qua đối (xem III, p. 230).

#### Nhận xét 2 {#ta-iii-s2-n1-rem-2 .statement tag=01WQ}

Cho X và Y là các không gian tôpô. Ánh xạ chính tắc

$$
\mathscr{C}(X\times \mathbf{I}; Y)\rightarrow \mathscr{C}(\mathbf{I};\mathscr{C}_c(X; Y))
$$

ứng với mỗi đồng luân $\sigma : X\times \mathbf{I}\rightarrow Y$ nối hai ánh xạ $f$ và $g$ từ X vào Y một đường có gốc $f$, số hạng $g$, trong không gian $\mathscr{C}_c(X; Y)$. Nếu X là một không gian compact địa phương, ánh xạ chính tắc này là song ánh (TG, X, p. 28, định lý 3).

Cho X là một không gian tôpô. Ta gọi không gian các đường của X, và ký hiệu bởi Λ(X), là không gian tôpô $\mathscr{C}_c(\mathbf{I}; X)$ mà các phần tử của nó là các đường trong X và tôpô của nó là tôpô hội tụ compact (xem TG, X, p. 27). Nếu $x$ là một điểm của X, ta ký hiệu bởi $\Lambda_x(X)$ không gian con của Λ(X) tạo bởi các đường có gốc $x$. Nếu $y$ là một điểm thứ hai của X, ta ký hiệu bởi $\Lambda_{x,y}(X)$ không gian con của Λ(X) tạo bởi các đường có gốc $x$ và số hạng $y$.

#### Mệnh đề 1 {#ta-iii-s2-prop-1 .statement tag=01WR}

Cho X và Z là các không gian tôpô. Đối với một ánh xạ $\varphi$ của Z vào không gian các đường đi $\mathscr{C}_c(\mathbf{I}; X)$ là liên tục, điều kiện cần và đủ là ánh xạ $(z, t)\mapsto \varphi (z)(t)$ là một ánh xạ liên tục của $Z\times \mathbf{I}$ vào X. Đặc biệt, ánh xạ $(c, t)\mapsto c(t)$ của $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}$ vào X là liên tục.

Không gian tôpô $\mathbf{I}$ là compact địa phương, nên mệnh đề suy ra từ TG, X, p. 28, th. 3.

Ta ký hiệu $o$ và gọi là ánh xạ gốc ánh xạ $c\mapsto c(0)$ của Λ(X) vào X; ta ký hiệu $e$ và gọi là ánh xạ số hạng ánh xạ $c\mapsto c(1)$ của Λ(X) vào X. Các ánh xạ $o$ và $e$ là liên tục (TG, X, p. 27, nhận xét 1). Các cặp đường đi ghép trong X là các phần tử của tích bó của các không gian X $(\Lambda (X), e)$ và $(\Lambda (X), o)$.

#### Mệnh đề 2 {#ta-iii-s2-prop-2 .statement tag=01WS}

Cho X là một không gian tôpô. Ánh xạ gắn với một đường đi $c$ đường đi đối $\overline{c}$ là một phép đồng phôi của Λ(X) lên chính nó. Phép ghép các đường đi $(c, d)\mapsto c*d$ là một phép đồng phôi của không gian $(\Lambda (X), e)\times_X(\Lambda (X), o)$ lên Λ(X).

Ánh xạ $t\mapsto 1-t$ là một phép đồng phôi của không gian $\mathbf{I}$ lên chính nó; mệnh đề đầu tiên suy ra.

Ký hiệu C là tích bó $(\Lambda (X), e)\times_X(\Lambda (X), o)$. Gọi $\gamma : C\rightarrow$ Λ(X) là ánh xạ $(c, d)\mapsto c*d$ và $\delta : C\times \mathbf{I}\rightarrow$ X là ánh xạ $((c, d), t)\mapsto (c*d)(t)$. Các hạn chế của ánh xạ $\delta$ lên $C\times [0,\frac{1}{2}]$ và $C\times [\frac{1}{2},1]$ là liên tục theo công thức (1) và mệnh đề 1. Ánh xạ $\delta$ do đó là liên tục (TG, I, p. 19, mệnh đề 4), cũng như ánh xạ $\gamma$ (mệnh đề 1). Ta có $c(t) = (c*d)(\frac{t}{2})$ và $d(t) = (c*d)(\frac{1+t}{2})$, do đó $\gamma$ là đơn ánh.

Cho $g$ là một đường đi trong X; với $t\in \mathbf{I}$, đặt

$c_g(t) =g(\frac{t}{2})$ và $d_g(t) =g(\frac{1 + t}{2})$.

Các ánh xạ $c_g$ và $d_g$ được định nghĩa như vậy là các đường đi ghép trong X và ta có $c_g*d_g=g$. Hơn nữa, các ánh xạ $g\mapsto c_g$ và $g\mapsto d_g$ là các ánh xạ liên tục của không gian Λ(X) vào chính nó (mệnh đề 1). Suy ra ánh xạ $\gamma$ là một phép đồng phôi.

#### Hệ quả {#ta-iii-s2-n1-cor-1 .statement tag=01WT}

Cho X là một không gian tôpô và cho $x,y,z$ là các điểm của X. Các ánh xạ $c\mapsto \overline{c}$ của $\Lambda_{x,y}(X)$ vào $\Lambda_{y,x}(X)$ và $(c, d)\mapsto$ $c*d$ của $\Lambda_{x,y}(X)\times \Lambda_{y,z}(X)$ vào $\Lambda_{x,z}(X)$ là liên tục.

### 2. Các không gian liên thông theo cung

#### Định nghĩa 3 {#ta-iii-s2-def-3 .statement tag=01WU}

Một không gian tôpô X được gọi là liên thông theo cung nếu với mọi cặp $(x, y)$ các điểm của X, tồn tại một đường đi có gốc $x$ và có số hạng $y$.

#### Ví dụ 1 {#ta-iii-s2-n2-exa-1 .statement tag=01WV}

Mọi khoảng của $\mathbf{R}$, mọi tập con lồi của một không gian số hoặc, nói chung hơn, của một không gian vectơ tôpô trên $\mathbf{R}$ đều liên thông theo cung.

#### Mệnh đề 3 {#ta-iii-s2-prop-3 .statement tag=01WW}

Ảnh bởi một ánh xạ liên tục của một không gian liên thông theo cung là liên thông theo cung.

Cho X là một không gian liên thông đường, $f: X\rightarrow Y$ là một ánh xạ liên tục. Cho $x$ và $y$ là hai điểm của $f(X)$; cho $x'$ và $y'$ là các điểm của X sao cho $f(x') =x$ và $f(y') =y$. Tồn tại một đường $c$ trong X có gốc là $x'$ và số hạng là $y'$. Khi đó, $f\circ c$ là một đường trong $f(X)$ có gốc là $x$ và số hạng là $y$.

#### Mệnh đề 4 {#ta-iii-s2-prop-4 .statement tag=01WX}

Một không gian tôpô liên thông đường là liên thông.

Vì mọi khoảng của $\mathbf{R}$ là liên thông, ảnh của một đường là liên thông (TG, I, p. 82, Mệnh đề 4). Không gian rỗng là liên thông. Vì một không gian liên thông đường khác rỗng là hợp của các ảnh của các đường xuất phát từ một điểm của nó, nên nó là liên thông (TG, I, p. 81, Mệnh đề 2).

Xét đến sự đồng nhất (III, p. 256, nhận xét 1) các đường trong X với các đồng luân giữa các ánh xạ từ một không gian tôpô P thu gọn về một điểm vào X, Mệnh đề 1 của III, p. 230 cho:

#### Mệnh đề 5 {#ta-iii-s2-prop-5 .statement tag=01WY}

Trong một không gian tôpô, quan hệ “tồn tại một đường có gốc $x$ và số hạng $y$” là một quan hệ tương đương.

Các thành phần liên thông đường của một không gian tôpô X được gọi là các lớp tương đương đối với quan hệ trên. Một thành phần liên thông đường là một không gian liên thông đường. Cho $x$ là một điểm của X. Thành phần liên thông đường của $x$ là hợp của các không gian con liên thông đường của X chứa $x$. Nó cũng là hợp của các ảnh của các đường có gốc $x$ trong X.

#### Ví dụ 2 {#ta-iii-s2-n2-exa-2 .statement tag=01WZ}

Hợp của một họ các tập hợp liên thông đường, có giao khác rỗng, là liên thông đường (cf. TG, I, p. 81, Mệnh đề 2).

#### Ví dụ 3 {#ta-iii-s2-n2-exa-3 .statement tag=01X0}

Một tập con của một không gian số (hoặc, nói chung, một không gian vectơ tôpô trên $\mathbf{R}$) là hình sao tại một trong các điểm của nó thì là liên thông đường.

Cho X là một không gian tôpô. Ta ký hiệu bởi $\pi_0(X)$ tập hợp các thành phần liên thông đường của X. Cho P là một không gian tôpô thu gọn về một điểm. Ánh xạ từ X vào [P; X] mà, với mỗi điểm $x$ của X, gán lớp đồng luân $\varphi_x$ của ánh xạ $f_x: P\rightarrow X$ có ảnh là $x$, xác định bằng cách chuyển qua thương một song ánh, gọi là chính tắc, từ $\pi_0(X)$ lên [P; X]. Ta có $\pi_0(\emptyset ) =\emptyset$. Để một không gian tôpô khác rỗng là liên thông đường, điều kiện cần và đủ là $\pi_0(X)$ là một tập hợp có một phần tử.

Cho X và Y là các không gian tôpô và $f: X\rightarrow Y$ là một ánh xạ liên tục. Ảnh $f(C)$ của mọi thành phần liên thông đường C của X là liên thông đường (III, p. 258, Mệnh đề 3), do đó được chứa trong một thành phần liên thông đường của Y. Ta ký hiệu bởi $\pi_0(f):\pi_0(X)\rightarrow \pi_0(Y)$ ánh xạ mà, với một thành phần liên thông đường C của X, gán thành phần liên thông đường duy nhất $C'$ của Y sao cho $f(C)\subset C'$. Nếu ta đồng nhất $\pi_0(X)$ và $\pi_0(Y)$ với [P; X] và [P; Y] tương ứng, ánh xạ $\pi_0(f)$ đồng nhất với ánh xạ $\chi \mapsto [f]\circ \chi$ từ [P; X] vào [P; Y]. Đặc biệt, nếu $f$ và $g$ là các ánh xạ đồng luân từ X vào Y, ta có $\pi_0(f) =\pi_0(g)$ (III, p. 230, Mệnh đề 2).

Cho Z là một không gian tôpô và cho $g: Y\rightarrow$ Z là một ánh xạ liên tục; ta có $\pi_0(g\circ f) =\pi_0(g)\circ \pi_0(f)$. Đặc biệt, nếu Z = X và nếu $f$ và $g$ là các nghịch đảo đồng luân của nhau đến sai khác đồng luân, ta có $\pi_0(g)\circ \pi_0(f) =\pi_0$(Id$_X$) $=$ Id$_{\pi_0(X)}$ và $\pi_0(f)\circ \pi_0(g) =\pi_0$(Id$_Y$) $=$ Id$_{\pi_0(Y)}$, điều này chứng minh rằng $\pi_0(f)$ và $\pi_0(g)$ là các song ánh nghịch đảo của nhau. Một không gian tương đương đồng luân với một không gian liên thông đường do đó tự nó là liên thông đường. Đặc biệt, một không gian tương đương đồng luân với một điểm là liên thông đường.

#### Mệnh đề 6 {#ta-iii-s2-prop-6 .statement tag=01X1}

Cho $(Y_j)_{j\in J}$ là một họ các không gian tôpô. Ánh xạ

$(\pi_0$(pr$_j$))$:\pi_0(\prod_{j\in J}Y_j)\rightarrow \prod_{j\in J}\pi_0(Y_j)$

là song ánh. Đặc biệt, không gian tích của một họ các không gian liên thông đường đi là liên thông đường đi.

Điều này suy ra từ Mệnh đề 3 của III, p. 231, trong đó lấy X là một không gian thu gọn về một điểm.

### 3. Các không gian liên thông đường đi địa phương

#### Định nghĩa 4 {#ta-iii-s2-def-4 .statement tag=01X2}

Một không gian tôpô được gọi là liên thông đường đi địa phương nếu mỗi điểm của nó có một hệ lân cận cơ bản gồm các lân cận liên thông đường đi.

#### Mệnh đề 7 {#ta-iii-s2-prop-7 .statement tag=01X3}

Một không gian tôpô liên thông đường đi địa phương là liên thông địa phương. Các thành phần liên thông của nó trùng với các thành phần liên thông đường đi của nó. Đặc biệt, nếu một không gian tôpô liên thông đường đi địa phương là liên thông thì nó là liên thông đường đi.

Mệnh đề thứ nhất suy ra từ mệnh đề 4. Ta hãy chứng minh mệnh đề thứ hai. Cho X là một không gian tôpô liên thông đường đi địa phương và C là một thành phần liên thông đường đi của X. Mỗi điểm của C có một lân cận liên thông đường đi, do đó được chứa trong C; do đó, C là một tập con mở của X. Các thành phần liên thông đường đi lập thành một phân hoạch của X, nên thành phần như vậy cũng là đóng. Vì nó liên thông (III, p. 258, mệnh đề 4), nó là một thành phần liên thông (TG, I, p. 83). Mệnh đề thứ ba suy ra từ mệnh đề thứ hai.

Do đó ta thấy rằng không có sự mơ hồ khi nói rằng một không gian tôpô là liên thông và liên thông đường đi địa phương.

#### Hệ quả 1 {#ta-iii-s2-prop-7-cor-1 .statement tag=01X4}

Mọi tập con mở liên thông của một không gian tôpô liên thông đường đi địa phương đều là liên thông đường đi.

#### Hệ quả 2 {#ta-iii-s2-prop-7-cor-2 .statement tag=01X5}

Cho B là một không gian tôpô liên thông đường đi địa phương và E là một không gian étalé trên B. Không gian E là liên thông đường đi địa phương. Nếu nó liên thông thì nó liên thông đường đi.

Mệnh đề thứ nhất suy ra ngay lập tức từ định nghĩa 4 và định nghĩa của một ánh xạ étalé (I, p. 28, định nghĩa 2). Mệnh đề thứ hai suy ra từ đó theo mệnh đề 7.

Để một không gian tôpô X là liên thông đường đi địa phương, điều kiện cần và đủ là mọi thành phần liên thông đường đi của một tập mở của X đều là một tập mở của X (xem I, p. 85, chứng minh mệnh đề 11). Nếu không gian X là liên thông đường đi địa phương, do đó mỗi điểm của X có một hệ lân cận cơ bản gồm các lân cận mở liên thông đường đi.

#### Mệnh đề 8 {#ta-iii-s2-prop-8 .statement tag=01X6}

Mọi không gian thương của một không gian liên thông đường đi địa phương đều là liên thông đường đi địa phương.

Cho X là một không gian liên thông đường đi địa phương, cho R là một quan hệ tương đương trong X và cho $\varphi : X\rightarrow X/R$ là ánh xạ chính tắc. Chỉ cần chứng minh rằng các thành phần liên thông đường đi của một tập con mở của $X/R$ là mở. Vậy cho A là một tập con mở của $X/R$ và cho C là một thành phần liên thông đường đi của A. Cho $x\in \overset{-1}{\varphi}(C)$, và cho K là thành phần liên thông đường đi của x trong $\overset{-1}{\varphi}(A)$. Tập hợp $\varphi (K)$ là liên thông đường đi (III, p. 258, mệnh đề 3), được chứa trong A và chứa $\varphi (x)$; do đó $\varphi (K)\subset C$, suy ra $K\subset \overset{-1}{\varphi}(C)$. Điều này chứng minh rằng $\overset{-1}{\varphi}(C)$ là hợp của các thành phần liên thông đường đi của $\overset{-1}{\varphi}(A)$. Vì X liên thông đường đi địa phương và $\overset{-1}{\varphi}(A)$ là mở trong X$, \overset{-1}{\varphi}(C)$ là mở trong X. Do đó, C là mở trong $X/R$. Điều này chứng minh mệnh đề.

#### Mệnh đề 9 {#ta-iii-s2-prop-9 .statement tag=01X7}

Tích của một họ các không gian liên thông đường đi địa phương, liên thông ngoại trừ một số hữu hạn không gian, là liên thông đường đi địa phương.

Cho $(X_j)_{j\in J}$ là một họ các không gian liên thông đường đi địa phương và liên thông, ngoại trừ một số hữu hạn không gian. Cho $x=$ $(x_j)_{j\in J}$ là một điểm của không gian tích X = $\prod_{j\in J}X_j$. Theo giả thiết, một hệ lân cận cơ bản của $x$ trong X gồm các tập hợp có dạng $V =\prod_{j\in J}V_j$ trong đó, với mọi $j\in J$, $V_j$ là một lân cận liên thông đường đi của $x_j$ trong $X_j$ và $V_j= X_j$ ngoại trừ một tập hữu hạn các chỉ số $j\in J$ (TG, I, p. 24). Vì các tập hợp này liên thông đường đi (III, p. 260, mệnh đề 6), X là liên thông đường đi địa phương.

#### Hệ quả {#ta-iii-s2-n3-cor-1 .statement tag=01X8}

Mọi tập con mở của một không gian số đều là liên thông đường đi địa phương.

Mỗi điểm của $\mathbf{R}$ có một cơ sở lân cận tạo bởi các khoảng; do đó, $\mathbf{R}$ là liên thông đường đi địa phương. Theo Mệnh đề 9, không gian số $\mathbf{R}^n$ là liên thông đường đi địa phương, với mọi số nguyên $n\geqslant 1$. Hơn nữa, một tập con mở của một không gian tôpô liên thông đường đi địa phương lại là liên thông đường đi, do đó có hệ quả.

#### Ví dụ {#ta-iii-s2-n3-exa-1 .statement tag=01X9}

Cho G là nhóm con của $\mathbf{G}\mathbf{L}(n,\mathbf{R})$ gồm các ma trận vuông cấp $n$ có định thức dương ngặt. Nhóm G là liên thông và liên thông đường đi địa phương.

Theo A, III, p. 104, mệnh đề 17, nhóm $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ được sinh bởi các phần tử $B_{ij}(\lambda )$ (với $1\leqslant i, j\leqslant n$ sao cho $i=\not j$ và $\lambda \in \mathbf{R}$). Các ánh xạ $\lambda \mapsto B_{ij}(\lambda )$ từ $\mathbf{R}$ vào $\mathbf{G}\mathbf{L}(n,\mathbf{R})$ là liên tục, ảnh của chúng là các tập con liên thông của $\mathbf{S}\mathbf{L}(n,\mathbf{R})$; vì tất cả chúng đều chứa ma trận đơn vị $I_n$, hợp của chúng là liên thông (TG, I, p. 81, mệnh đề 2). Do đó, nhóm $\mathbf{S}\mathbf{L}(n,\mathbf{R})$ là liên thông (TG, III, p. 8, mệnh đề 7). Cho A là nhóm con của G gồm các ma trận dạng diag(1$, . . . ,1, \lambda$ ), với $\lambda \in \mathbf{R}_+^*$; nó liên thông và ta có $\mathbf{G}\mathbf{L}(n,\mathbf{R}) = A\cdot \mathbf{S}\mathbf{L}(n,\mathbf{R})$. Suy ra nhóm G là liên thông. Vì nó là ảnh ngược của $\mathbf{R}_+^*$ qua ánh xạ định thức của $\mathbf{M}_n(\mathbf{R})$ vào $\mathbf{R}$, nó là một tập con mở của $\mathbf{M}_n(\mathbf{R})$; do đó nó liên thông địa phương theo cung (hệ quả trên), cũng như liên thông theo cung (III, p. 261, hệ quả 1).

#### Mệnh đề 10 {#ta-iii-s2-prop-10 .statement tag=01XA}

Cho X là một không gian tôpô. Ánh xạ $(o, e)$ của $\Lambda (X) =\mathscr{C}_c(\mathbf{I}; X)$ vào $X\times X$, gán cho một đường đi $c$ trong X cặp $(c(0), c(1))$, là liên tục. Nếu không gian X liên thông địa phương theo cung, thì ánh xạ này là mở.

Ta đã biết các ánh xạ gốc $o$ và số hạng $e$ của Λ(X) vào X là liên tục (III, p. 257), do đó mệnh đề đầu tiên.

#### Bổ đề {#ta-iii-s2-n3-lem-1 .statement tag=01XB}

Cho $c:\mathbf{I}\rightarrow X$ là một đường đi và W là một lân cận của $c$ trong không gian $\mathscr{C}_c(\mathbf{I}; X)$. Tồn tại một số thực $\varepsilon \in ]0,1/2]$, một lân cận $V_0$ của $c(0)$ và một lân cận $V_1$ của $c(1)$ trong X có các tính chất sau: ta có $c([0, \varepsilon ])\subset V_0,c([1-\varepsilon ,1])\subset V_1$, và mọi đường đi $c':\mathbf{I}\rightarrow X$ sao cho

$c'(t)\in V_0$ với $0\leqslant t\leqslant \varepsilon$,

(2) $c'(t) =c(t)$ với $\varepsilon \leqslant t\leqslant 1-\varepsilon$,

$c'(t)\in V_1$ với $1-\varepsilon \leqslant t\leqslant 1$,

đều thuộc W.

Theo định nghĩa của tôpô hội tụ compact (TG, X, p. 26, déf. 1), tồn tại một tập hữu hạn J, một họ $(U_j)_{j\in J}$ các tập mở trong X và một họ $(K_j)_{j\in J}$ các tập con compact của $\mathbf{I}$ sao cho tập $W'$ gồm các đường đi $c'$ thỏa mãn $c'(K_j)\subset U_j$ với mọi chỉ số $j$ là một lân cận của $c$ được chứa trong W. Khi đó, ký hiệu $A_0$ (resp. $A_1$) là tập các chỉ số $j$ sao cho $0\in K_j$ (resp. $1\in K_j$); đặt $V_0=\bigcap_{j\in A_0}U_j$ và $V_1=\bigcap_{j\in A_1}U_j$.

Vì ánh xạ $c$ liên tục, tồn tại một số thực $\varepsilon \in$ $]0,1/2]$ sao cho $c([0, \varepsilon ])\subset V_0,c([1-\varepsilon ,1])\subset V_1,[0, \varepsilon ]\cap K_j=\emptyset$ với mọi $j\notin A_0$ và $[1-\varepsilon ,1]\cap K_j=\emptyset$ với mọi $j\notin A_1$. Khi đó, cho $c'$ là một đường đi thỏa mãn các điều kiện (2). Hãy chứng minh rằng $c'\in W'$. Cho $j\in J$ và cho $t\in K_j$. Nếu $\varepsilon \leqslant t\leqslant 1-\varepsilon ,c'(t) =c(t)$ thuộc $U_j$. Nếu $0\leqslant t\leqslant \varepsilon ,c'(t)\in V_0$; do lựa chọn $\varepsilon$, ta có $j\in A_0$, do đó $c'(t)\in U_j$. Tương tự, nếu $1-\varepsilon \leqslant t\leqslant 1$, ta có $j\in A_1$ và $c'(t)\in V_1\subset U_j$. Vậy, $c'(K_j)\subset U_j$ và $c'$ thuộc $W'$, do đó thuộc W.

Bây giờ hãy chứng minh mệnh đề thứ hai của Mệnh đề 10. Giả sử rằng không gian X liên thông địa phương bởi các cung. Cho $c$ là một đường đi trong X và cho W là một lân cận của $c$ trong $\mathscr{C}_c(\mathbf{I}; X)$. Cho $\varepsilon ,V_0$ và $V_1$ như trong bổ đề. Cho $T_0$ và $T_1$ là các lân cận liên thông bởi các cung của $c(0)$ và $c(1)$ được chứa trong $V_0$ và $V_1$ tương ứng. Có một số thực $\theta$ sao cho $0< \theta  < \varepsilon$ và sao cho $c([0, \theta ])\subset T_0,c([1-\theta ,1])\subset T_1$. Cho $x_0\in T_0$ và $x_1\in T_1$; cho $c_0$ là một đường đi có điểm đầu $x_0$ và điểm cuối $c(\theta )$ trong $T_0$ và cho $c_1$ là một đường đi có điểm đầu $x_1$ và điểm cuối $c(1-\theta )$ trong $T_1$. Đặt

$c_0(t/\theta )$ cho $0\leqslant t\leqslant \theta$,

$c'(t) =c(t)$ cho $\theta \leqslant t\leqslant 1-\theta$,

$c_1((1-t)/\theta )$ cho $1-\theta \leqslant t\leqslant 1$.

Như vậy ta xác định được một đường đi $c'$ nối $x_0$ với $x_1$ và thỏa mãn các điều kiện (2). Điều này chứng minh rằng ảnh của W trong $X\times X$ bởi ánh xạ $(o, e)$ chứa lân cận $T_0\times T_1$ của $(c(0), c(1))$, do đó có mệnh đề.

#### Hệ quả {#ta-iii-s2-n3-cor-2 .statement tag=01XC}

Cho X là một không gian tôpô liên thông địa phương theo cung và cho $x$ là một điểm của X. Ánh xạ $c\mapsto c(1)$ của $\Lambda_x(X)$ vào X là mở.

Theo mệnh đề, ánh xạ $\varphi : \Lambda (X)\rightarrow X\times X$ được xác định bởi $\varphi (c) = (c(0), c(1))$ là mở và ta có $\Lambda_x(X) =\overset{-1}{\varphi}(\{x\} \times X)$. Do đó, ánh xạ $\Lambda_x(X)\rightarrow  \{x\} \times X$ suy ra từ $\varphi$ là mở (TG, I, p. 30, mệnh đề 2), cũng như hợp của nó với phép chiếu thứ hai pr$_2$.

### 4. Các liên hệ giữa tính liên thông và tính liên thông theo cung

Một không gian liên thông theo cung là liên thông (III, p. 258, mệnh đề 4). Có những không gian liên thông, thậm chí những không gian liên thông địa phương, không liên thông theo cung (xem III, p. 331, bài tập 2 và 4). Tuy nhiên:

#### Mệnh đề 11 {#ta-iii-s2-prop-11 .statement tag=01XD}

Một không gian tôpô liên thông và liên thông địa phương, có tôpô được xác định bởi một khoảng cách mà theo đó nó đầy đủ, là liên thông theo cung.

Cho X là một không gian tôpô. Gọi một đoàn tàu trong X là một dãy hữu hạn khác rỗng $T = (W_i)_{1\leqslant i\leqslant n}$ gồm các tập con mở liên thông của X sao cho $W_i\cap W_{i+1}=\not\emptyset$ với $1\leqslant i\leqslant n-1$. Ta nói rằng $n$ là độ dài của đoàn tàu T và các $W_i$ là các toa của nó. Nếu X được trang bị một khoảng cách tương thích với tôpô của nó, ta gọi bề rộng của đoàn tàu T là số lớn nhất của các đường kính của các toa của nó. Ta nói rằng đoàn tàu nối một điểm $a$ với một điểm $b$ nếu $a$ thuộc toa đầu tiên và $b$ thuộc toa cuối cùng. Ta gọi một sự làm mịn của T là một cặp $(T', f)$ tạo bởi một đoàn tàu $T'= (W'_j)_{1\leqslant j\leqslant m}$ và một ánh xạ tăng ngặt $f:\{0,1, . . . , n\} \rightarrow  \{0,1, . . . , m\}$ sao cho $f(0) = 0,f(n) =m$ và $W'_j\subset W_i$ với $1\leqslant i\leqslant n$ và $f(i-1)< j\leqslant f(i)$.

#### Bổ đề 1 {#ta-iii-s2-lem-1 .statement tag=01XE}

Cho X là một không gian metric liên thông và liên thông địa phương, cho $a$ và $b$ là các điểm của X và cho $\varepsilon$ là một số thực $>0$. Tồn tại trong X một đoàn tàu có bề rộng $\leqslant \varepsilon$ nối $a$ với $b$.

Chính xác hơn, mọi đoàn tàu T nối $a$ với $b$ đều có một sự làm mịn $(T', f)$, trong đó $T'$ là một đoàn tàu có bề rộng $\leqslant \varepsilon$ nối $a$ với $b$.

Quan hệ “tồn tại một đoàn tàu có bề rộng $\leqslant \varepsilon$ nối $x$ với $y$” là một quan hệ tương đương giữa $x$ và $y$ trong X. Lớp tương đương của một điểm $x$ chứa mọi lân cận mở liên thông của $x$ có đường kính $\leqslant \varepsilon$, và $x$ có một lân cận như vậy vì X là liên thông địa phương. Do đó các lớp tương đương của quan hệ này là mở, và do đó cũng đóng. Có nhiều nhất một lớp như vậy, vì X là liên thông. Điều này chứng minh mệnh đề đầu tiên.

Cho $T = (W_i)_{1\leqslant i\leqslant n}$ là một chuỗi trong X nối $a$ với $b$. Đặt $x_0=a$, $x_n=b$ và chọn đối với $1\leqslant i\leqslant n-1$ một điểm $x_i$ trong tập hợp khác rỗng $W_i\cap W_{i+1}$. Với $1\leqslant i\leqslant n$, tập hợp mở $W_i$ là liên thông và liên thông địa phương và $x_{i-1},x_i$ là hai điểm của nó; tồn tại theo đoạn trước một chuỗi $(W_{i,k})_{1\leqslant k\leqslant m_i}$ trong $W_i$, có bề rộng $\leqslant \varepsilon$, nối $x_{i-1}$ với $x_i$.

Đặt $m=m_1+\cdots +m_n$. Với $1\leqslant j\leqslant m$, đặt $W'_j= W_{i,k}$, trong đó $(i, k)$ là cặp duy nhất các số nguyên sao cho $1\leqslant i\leqslant n,1\leqslant k\leqslant m_i$ và $j=m_1+\cdots +m_{i-1}+k$. Với $0\leqslant i\leqslant n$, đặt $f(i) =m_1+\cdots +m_i$. Khi đó $T'= (W'_j)_{1\leqslant j\leqslant m}$ là một chuỗi có bề rộng $\leqslant \varepsilon$ trong X nối $a$ với $b$, và $(T', f)$ là một tinh luyện của T.

Bây giờ chứng minh Mệnh đề 11. Trang bị cho không gian X liên thông và liên thông địa phương một khoảng cách $d$, tương thích với tôpô của nó, mà đối với khoảng cách đó nó là đầy đủ. Cho $a$ và $b$ là các điểm của X. Bổ đề 1 cho phép ta xây dựng bằng quy nạp các dãy $(T_s)_{s\geqslant 0}$ và $(f_s)_{s\geqslant 1}$ sao cho, với mọi $s\geqslant 0$, $T_s= (W_{s,i})_{1\leqslant i\leqslant n_s}$ là một chuỗi có bề rộng $\leqslant 2^{-s}$ nối $a$ với $b$ và $(T_{s+1}, f_{s+1})$ là một tinh luyện của $T_s$.

Ta có thể chọn bằng quy nạp, với $s\geqslant 0$, một ánh xạ tăng ngặt $g_s:\{0,1, . . . , n_s\} \rightarrow \mathbf{I}$ sao cho $g_s(0) = 0$ và $g_s(n_s) = 1$, theo cách mà $g_{s+1}\circ f_s=g_s$. Định nghĩa, với $s\geqslant 0$, một tập con $A_s$ của $\mathbf{I}\times X$ bằng cách đặt

$$
A_s=\bigcup_{1\leqslant i\leqslant n_s}([g_s(i-1), g_s(i)]\times W_{s,i})
$$

Dãy $(A_s)_{s\geqslant 0}$ là giảm: thật vậy, với mọi số nguyên $j\in  \{1, . . . , n_{s+1}\}$, tồn tại một số nguyên duy nhất $i\in  \{1, . . . , n_s\}$ sao cho $f_s(i-1)< j\leqslant f_s(i)$, và ta có

$$
[g_{s+1}(j-1), g_{s+1}(j)]\subset [g_s(i-1), g_s(i)],W_{s+1,j}\subset W_{s,i}
$$

Cho $t\in \mathbf{I}$. Với mọi $s\geqslant 0$, ký hiệu $A_s(t)$ là tập hợp các $x\in X$ sao cho $(t, x)\in A_s$. Tập hợp $A_s(t)$ hoặc là một trong các toa, hoặc là hợp của hai toa liên tiếp của đoàn tàu $T_s$; do đó nó là một tập con khác rỗng của X, có đường kính $\leqslant 2^{1-s}$. Dãy $(A_s(t))_{s\geqslant 0}$ là giảm. Tập hợp các số hạng của nó là một cơ sở lọc Cauchy. Cơ sở này hội tụ đến một điểm $c(t)$ vì không gian metric X là đầy đủ.

Vì $a$ thuộc mỗi tập hợp $A_s(0) = W_{s,1}$, ta có $c(0) =a$; tương tự $c(1) =b$. Cho $t\in \mathbf{I}$ và cho $s$ là một số nguyên $\geqslant 0$. Điểm $t$ có trong $\mathbf{I}$ một lân cận V có một trong các dạng sau: $[g_s(0), g_s(1)[$, $]g_s(i-1), g_s(i+ 1)[$ với một số nguyên $i$ sao cho $1\leqslant i\leqslant$ $n_s-1$, hoặc $]g_s(n_s-1), g_s(n_s)]$. Tùy theo trường hợp, tập hợp $c(V)$ được chứa trong bao đóng của toa thứ nhất, của hợp hai toa liên tiếp, hoặc của toa cuối cùng của đoàn tàu $T_s$. Do đó nó có đường kính $\leqslant 2^{1-s}$, và ta có $d(c(t), c(t'))\leqslant 2^{1-s}$ với $t'\in V$. Điều này chứng minh rằng ánh xạ $c:\mathbf{I}\rightarrow$ X là liên tục. Vậy $c$ là một đường trong X nối $a$ với $b$, và X là liên thông theo cung.

#### Hệ quả 1 {#ta-iii-s2-lem-1-cor-1 .statement tag=01XF}

Một không gian tôpô liên thông địa phương, có tôpô có thể được xác định bởi một khoảng cách đầy đủ, là liên thông theo cung địa phương.

Cho X là một không gian như vậy và cho U là một tập con mở và liên thông của X. Theo Bổ đề 2 dưới đây, tồn tại một khoảng cách trên U tương thích với tôpô của nó sao cho U là đầy đủ. Vì U liên thông địa phương, suy ra từ Mệnh đề 11 rằng U liên thông theo cung.

#### Bổ đề 2 {#ta-iii-s2-lem-2 .statement tag=01XG}

Cho X là một không gian metric đầy đủ và cho U là một tập con mở của X. Tồn tại một khoảng cách trên U tương thích với tôpô của nó sao cho U là đầy đủ.

Ta sẽ lấy lại các lập luận của chứng minh mệnh đề 2 của TG, IX, p. 57. Ta có thể giả sử U phân biệt với X. Cho V là tập con của tích $\mathbf{R}\times X$ tạo bởi các điểm $(t, x)$ sao cho $t d(x,X-U) = 1$ ; không gian con V của $\mathbf{R}\times X$ là đóng và ánh xạ $(t, x)\mapsto x$ từ V vào U là một phép đồng phôi (TG, IX, p. 13, mệnh đề 3). Trên $\mathbf{R}\times X$ tồn tại một khoảng cách $d'$ tương thích với tôpô của nó sao cho $\mathbf{R}\times X$ là đầy đủ (TG, IX, p. 15, hệ quả 2 và TG, II, p. 17, mệnh đề 10). Không gian V là đầy đủ đối với khoảng cách cảm sinh bởi $d'$ (TG, II, p. 16, mệnh đề 8), do đó có bổ đề.

#### Hệ quả 2 {#ta-iii-s2-lem-2-cor-2 .statement tag=01XH}

Một không gian tôpô compact địa phương, liên thông địa phương và mêtric hóa được là liên thông theo cung địa phương. Nếu nó liên thông, thì nó liên thông theo cung.

Chỉ cần chứng minh mệnh đề đầu tiên (III, p. 260, mệnh đề 7). Cho X là một không gian metric compact địa phương và liên thông địa phương. Các tập con mở, liên thông và tương đối compact của X tạo thành một cơ sở của tôpô của X. Cho U là một tập như vậy; vì U là một tập con mở của bao đóng của nó, là một không gian metric compact, do đó đầy đủ, nên theo Bổ đề 2 tồn tại một khoảng cách trên U tương thích với tôpô của nó sao cho U là đầy đủ. Suy ra từ mệnh đề 11 của III, p. 264 rằng U là liên thông theo cung, do đó có hệ quả.

### 5. Các ánh xạ liên tục theo cung

#### Định nghĩa 5 {#ta-iii-s2-def-5 .statement tag=01XI}

Cho X và Y là các không gian tôpô. Một ánh xạ $f: X\rightarrow Y$ được gọi là liên tục theo cung nếu, với mọi đường $c$ trong X, ánh xạ $f\circ c:\mathbf{I}\rightarrow Y$ là liên tục.

#### Nhận xét {#ta-iii-s2-n5-rem-1 .statement tag=01XJ}

Giả sử không gian X là liên thông theo cung. Cho $x$ là một điểm của X. Để $f$ liên tục theo cung, chỉ cần rằng, với mọi đường $c$ có gốc $x$, ánh xạ $f\circ c$ là liên tục. Thật vậy, cho $d$ là một đường tùy ý trong X và cho $c$ là một đường trong X có gốc $x$ và có số hạng cuối $d(0)$. Nếu ánh xạ $f\circ (c*d)$ là liên tục, thì điều tương tự đúng với ánh xạ $f\circ d$ vì ta có $f\circ d(t) =f\circ (c*d)((t+ 1)/2)$.

Một ánh xạ liên tục là liên tục theo cung. Điều đảo lại không phải luôn luôn đúng; các mệnh đề 12 và 13 dưới đây cung cấp các tiêu chuẩn cho phép khẳng định rằng một ánh xạ liên tục theo cung là liên tục.

#### Mệnh đề 12 {#ta-iii-s2-prop-12 .statement tag=01XK}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ. Giả sử không gian X là liên thông theo cung địa phương và mọi điểm của X đều có một hệ cơ bản đếm được các lân cận. Nếu ánh xạ $f$ liên tục theo cung, thì nó liên tục.

Theo (TG, IX, p. 18), chỉ cần chứng minh rằng, với mọi điểm $x$ của X và mọi dãy $(x_n)_{n\geqslant 1}$ các điểm của X hội tụ tới $x$, dãy $(f(x_n))_{n\geqslant 1}$ hội tụ tới $f(x)$. Bằng cách loại bỏ, nếu cần thiết, các số hạng đầu tiên của dãy $(x_n)_{n\geqslant 1}$, ta rút gọn về trường hợp tất cả các số hạng của dãy thuộc cùng một lân cận liên thông theo cung của $x$ trong X. Theo bổ đề dưới đây, khi đó tồn tại một đường đi $c:\mathbf{I}\rightarrow X$ sao cho $c(0) =x$ và $c(1/n) =x_n$ với $n\geqslant 1$. Nếu ánh xạ $f$ liên tục theo cung, ánh xạ $f\circ c$ liên tục và phần tử $f(x) =f(c(0))$ là giới hạn của dãy $(f(c(1/n)))_{n\geqslant 1}$, nghĩa là của dãy $(f(x_n))_{n\geqslant 1}$, do đó có hệ quả.

#### Bổ đề {#ta-iii-s2-n5-lem-1 .statement tag=01XL}

Cho X là một không gian tôpô liên thông và liên thông địa phương theo cung và cho $x$ là một điểm của X. Giả sử rằng điểm $x$ có một hệ cơ bản đếm được các lân cận. Khi đó, với mọi dãy $(x_n)_{n\geqslant 1}$ các điểm của X hội tụ tới $x$, tồn tại một đường đi $c$ trong X sao cho $c(0) =x$ và $c(1/n) =x_n$ với $n\geqslant 1$.

Cho $(W_m)_{m\geqslant 1}$ là một hệ cơ bản các lân cận của $x$. Đặt $V_0= X$ và với mọi $m\geqslant 1$, cho $V_m$ là một lân cận liên thông theo cung của $x$ được chứa trong $V_{m-1}\cap W_m$.

Với mọi số nguyên $n\geqslant 1$, ký hiệu $m_n$ là số nguyên lớn nhất $m\leqslant n$ sao cho $x_k\in V_m$ với mọi $k\geqslant n$. Dãy $(m_n)_{n\geqslant 1}$ là tăng theo định nghĩa; nó tiến tới vô hạn, vì dãy $(x_n)_{n\geqslant 1}$ hội tụ tới $x$. Với mọi số nguyên $n\geqslant 1$, cho $c_n:\mathbf{I}\rightarrow V_{m_n}$ là một đường đi có điểm đầu $x_{n+1}$ và điểm cuối $x_n$ trong $V_{m_n}$. Định nghĩa một ánh xạ $c:\mathbf{I}\rightarrow X$ bằng cách đặt $c(0) =x$ và $c(t) =c_n(n(n+ 1)t-n)$ nếu $1/(n+ 1)< t\leqslant$ $1/n$. Ta có $c(1/n) =x_n$ với mọi $n\geqslant 1$. Do đó ánh xạ $c$ liên tục trên mọi khoảng có dạng $[1/(n+ 1),1/n]$ với $n\geqslant 1$, và do đó trên khoảng $]0,1]$. Nếu $t\leqslant 1/n$, điểm $c(t)$ thuộc $V_{m_n}$; do đó ánh xạ $c$ liên tục tại 0.

#### Mệnh đề 13 {#ta-iii-s2-prop-13 .statement tag=01XM}

Cho $p: E\rightarrow B$ là một ánh xạ étale và tách được và cho $s: B\rightarrow E$ là một tiết diện của $p$. Nếu không gian B địa phương liên thông theo đường và nếu tiết diện $s$ liên tục theo đường, thì nó liên tục.

Cho $b$ là một điểm của B; ta hãy chứng minh rằng $s$ liên tục tại điểm $b$. Vì $p$ là một ánh xạ étale, tồn tại một lân cận V của $b$ và một tiết diện địa phương liên tục $s'$ của $p$ xác định trong V sao cho $s'(b) =s(b)$ (I, p. 33, prop. 9). Vì B địa phương liên thông theo đường, ta có thể giả sử rằng V liên thông theo đường. Với mọi đường đi $c$ trong V, có gốc $b$, các ánh xạ $s\circ c$ và $s'\circ c$ là hai phép nâng liên tục lên B của ánh xạ $c:\mathbf{I}\rightarrow X$ và ta có $s\circ c(0) =s'\circ c(0) =s(b)$. Theo Hệ quả 1 của I, p. 34, ta có $s\circ c=s'\circ c$ và đặc biệt $s\circ c(1) =s'\circ c(1)$. Vì mọi điểm của V là điểm cuối của một đường đi trong V có gốc $b$, các ánh xạ $s$ và $s'$ trùng nhau trong V. Do đó ánh xạ $s$ liên tục trong V.

#### Hệ quả {#ta-iii-s2-n5-cor-1 .statement tag=01XN}

Cho B là một không gian tôpô, cho $(E, p)$ và $(E', p')$ là hai B-không gian. Giả sử rằng ánh xạ $p$ là étale và tách được và rằng không gian $E'$ địa phương liên thông theo đường. Khi đó mọi ánh xạ liên tục theo đường $f: E'\rightarrow E$ sao cho $p\circ f=p'$ là liên tục.

Ánh xạ pr$_1: E'\times_BE\rightarrow E'$ là étale và tách được (I, p. 31, prop. 8 và I, p. 27, prop. 4) và ánh xạ $x\mapsto (x, f(x))$ là một tiết diện liên tục theo đường của nó. Theo Mệnh đề 13, nó liên tục, do đó $f$ liên tục.

### 6. Các bổ sung về các không gian tôpô mêtric hóa compact

Ta trang bị cho tập hợp có hai phần tử $\{0,1\}$ tôpô rời rạc và cho tập hợp $\{0,1\}^{\mathbf{N}}$ tôpô tích. Không gian tôpô $\{0,1\}^{\mathbf{N}}$ là compact (TG, I, p. 63, th. 3), mêtric hóa được (TG, IX, p. 15, cor. 2), khác rỗng, hoàn toàn không liên thông (TG, I, p. 84, prop. 10) và không có điểm cô lập.

#### Mệnh đề 14 {#ta-iii-s2-prop-14 .statement tag=01XO}

Mọi không gian tôpô compact, mêtric hóa được, khác rỗng, hoàn toàn không liên thông không có điểm cô lập đều đồng phôi với $\{0,1\}^{\mathbf{N}}$.

Cho X là một không gian tôpô như vậy. Ta trang bị cho nó một khoảng cách tương thích với tôpô của nó. Vì không gian X là compact, nó đầy đủ đối với khoảng cách này (TG, II, p. 27, th. 1).

#### Bổ đề 3 {#ta-iii-s2-lem-3 .statement tag=01XP}

Cho $\varepsilon$ là một số thực $>0$. Tồn tại một số nguyên $m\geqslant 1$ sao cho, với mọi số nguyên $n\geqslant m$, X thừa nhận một phân hoạch gồm $n$ tập hợp mở và đóng khác rỗng có đường kính $\leqslant \varepsilon$.

Mọi điểm của X thừa nhận một lân cận mở và đóng có đường kính $\leqslant \varepsilon$ (TG, II, p. 32, hệ quả của prop. 6). Vì không gian X là compact, nó có một phủ hữu hạn bởi các tập hợp như vậy. Chọn một phủ, $(U_i)_{1\leqslant i\leqslant m}$, mà ở đó $m$ là cực tiểu. Ta có $m\geqslant 1$ vì X khác rỗng. Với $1\leqslant i\leqslant m$, ký hiệu $V_i$ là giao của $U_i$ và các $X-U_k$ với $k < i$. Khi đó $(V_i)_{1\leqslant i\leqslant m}$ là một phân hoạch của X, gồm $m$ tập hợp mở và đóng khác rỗng có đường kính $\leqslant \varepsilon$.

Vì X không có điểm cô lập, mọi tập con mở và đóng khác rỗng V của X chứa ít nhất hai điểm. Hơn nữa vì X compact và hoàn toàn không liên thông, V là hợp của hai tập con mở và đóng khác rỗng rời nhau (loc. cit.). Suy ra, bằng quy nạp, rằng với mọi số nguyên $n\geqslant m$, X thừa nhận một phân hoạch gồm $n$ tập hợp mở và đóng khác rỗng có đường kính $\leqslant \varepsilon$.

Bây giờ ta hoàn tất chứng minh của mệnh đề 14. Mọi không gian con mở và đóng khác rỗng của X là một không gian mêtric compact, hoàn toàn không liên thông và không có điểm cô lập. Do đó Bổ đề 3 cho phép ta xây dựng bằng quy nạp một dãy $(J_n)_{n\geqslant 0}$ các tập hợp hữu hạn và, với mọi $n\geqslant 0$, một ánh xạ $\varphi_n$ từ tập hợp $C_n= J_0\times  \cdots  \times J_n$ vào tập hợp các tập con mở và đóng khác rỗng của X có đường kính $\leqslant 2^{-n}$, sao cho :

(i) Với mọi $n\geqslant 0$, tồn tại một số nguyên $m_n\geqslant 1$ sao cho Card(J$_n$) $=$ $2^{m_n}$;

(ii) Họ $(\varphi_0(c))_{c\in C_0}$ là một phân hoạch của X ;

(iii) Với mọi $n\geqslant 0$ và mọi $c\in C_n$, họ $(\varphi_{n+1}(c, j))_{j\in J_{n+1}}$ là một phân hoạch của $\varphi_n(c)$.

Ta ký hiệu $p_n$ là phép chiếu chính tắc của $C_{n+1}$ lên $C_n$. Dãy C = $(C_n, p_n)_{n\geqslant 0}$ là một sàng (TG, IX, p. 63, định nghĩa 8). Không gian tôpô liên kết với sàng này (TG, IX, p. 63) được đồng nhất với không gian tôpô J, tích của các không gian tôpô rời rạc $J_n$. Sàng C và dãy các ánh xạ $(\varphi_n)_{n\geqslant 0}$ định nghĩa một phép sàng ngặt của không gian mêtric X (TG, IX, p. 63 và p. 64). Ánh xạ $f: J\rightarrow X$ suy ra từ phép sàng này là liên tục và song ánh (TG, IX, p. 65). Vì không gian tôpô J là compact (TG, I, p. 63, định lý 3) và X là tách, $f$ là một phép đồng phôi (TG, I, p. 63, hệ quả 2). Vì $J_n$ đồng phôi với $\{0,1\}^{m_n}$ với mọi $n\geqslant 0$, J đồng phôi với $\{0,1\}^{\mathbf{N}}$ (TG, I, p. 25, mệnh đề 2).

#### Ví dụ {#ta-iii-s2-n6-exa-1 .statement tag=01XQ}

Cho K là tập Cantor tam phân (TG, IV, p. 9, ví dụ). Với mọi $n\geqslant 0$, đặt $J_n=\{0,1\}$ và định nghĩa một ánh xạ $K_n$ từ tập hợp $C_n= J_0\times  \cdots  \times J_n$ vào tập hợp các khoảng đóng của $[0,1]$ theo cách sau: đặt $K_0(0) = [0,\frac{1}{3}]$ và $K_0(1) = [\frac{2}{3},1]$; với mọi $n\geqslant 0$ và mọi $c\in C_n,K_{n+1}(c,0)$ và $K_{n+1}(c,1)$ lần lượt là “phần ba bên trái” và “phần ba bên phải” của $K_n(c)$. Nếu $c= (j_0, j_1, . . . , j_n)\in C_n,K_n(c)$ là khoảng được ký hiệu bởi $K_{n,p}$ trong loc. cit., với $p= 2^nj_0+2^{n-1}j_1+\cdots +j_n+1$, thì nó cũng là khoảng $[a, a+\frac{1}{3^{n+1}}]$, trong đó $a= 2(\frac{j_0}{3}+\frac{j_1}{3^2}+\cdots +\frac{j_n}{3^{n+1}})$. Với $n\geqslant 0$ và $c\in C_n$, đặt $\varphi_n(c) = K_n(c)\cap K$. Họ $(\varphi_n(c))_{c\in C_n}$ là một phân hoạch của K được tạo thành bởi các tập đóng. Do đó các tập hợp này cũng mở trong K; chúng khác rỗng và có đường kính $\frac{1}{3^{n+1}}$, bởi vì các đầu mút của các khoảng $K_n(c)$ thuộc K. Dãy $C = (C_n, p_n)_{n\geqslant 0}$, trong đó $p_n: C_{n+1}\rightarrow C_n$ là phép chiếu chính tắc $(c, j)\mapsto c$, là một sàng, và không gian tôpô liên kết với sàng này được đồng nhất với $\{0,1\}^{\mathbf{N}}$. Sàng C và dãy các ánh xạ $(\varphi_n)_{n\geqslant 0}$ định nghĩa một phép sàng ngặt của không gian mêtric K. Ánh xạ $f:\{0,1\}^{\mathbf{N}}\rightarrow K$ suy ra từ phép sàng này là một phép đồng phôi, được cho bởi công thức

$$
f((j_n)_{n\geqslant 0}) = 2\sum_{n=0}^{\infty}\frac{j_n}{3^{n+1}}
$$

#### Hệ quả {#ta-iii-s2-n6-cor-1 .statement tag=01XR}

Cho X là một không gian tôpô mêtric hóa được, compact và khác rỗng. Tồn tại một ánh xạ liên tục và toàn ánh từ $\{0,1\}^{\mathbf{N}}$ vào X.

Mọi không gian tôpô compact và mêtric hóa được đều đồng phôi với một không gian con nhất thiết đóng của không gian tôpô $\mathbf{I}^{\mathbf{N}}$ (TG, IX, p. 18, mệnh đề 12 và p. 21, mệnh đề 16). Cho A là một không gian con đóng của $\mathbf{I}^{\mathbf{N}}$ và $h$ là một phép đồng phôi của A lên X.

Cho $K = \{0,1\}^{\mathbf{N}}$ và, với $\alpha = (a_n)\in$ K, đặt $f(\alpha ) =$ $\sum^{\infty}_{n=0}a_n2^{-n-1}$; ta có $f(\alpha )\in \mathbf{I}$. Ánh xạ $f: K\rightarrow \mathbf{I}$ thu được như vậy là toàn ánh (TG, IV, p. 42) và liên tục. Thật vậy, nếu hai phần tử $\alpha$ và $\beta$ của K có cùng các tọa độ có chỉ số $< n$, ta có $|f(\beta )-f(\alpha )|\leqslant 2^{-n}$. Gọi $g$ là ánh xạ $(\alpha_n)\mapsto (f(\alpha_n))$ của $K^{\mathbf{N}}$ vào $\mathbf{I}^{\mathbf{N}}$; nó liên tục và toàn ánh. Không gian tôpô $K^{\mathbf{N}}$ là compact (TG, I, p. 63, th. 3), mêtric hóa được (TG, IX, p. 15, hệ quả 2) và hoàn toàn không liên thông (TG, I, p. 84, mệnh đề 10) và điều tương tự đúng cho không gian con đóng $\overset{-1}{g}(A)$ của nó; không gian sau khác rỗng vì các ánh xạ $g$ và $h$ là toàn ánh.

Khi đó, không gian $\overset{-1}{g}(A)\times K$ đồng phôi với $\{0,1\}^{\mathbf{N}}$ (mệnh đề 14), vì nó là một không gian tôpô compact, mêtric hóa được, hoàn toàn không liên thông không có điểm cô lập và ánh xạ $(x, y)\mapsto h(g(x))$ của $\overset{-1}{g}(A)\times K$ vào X là liên tục toàn ánh.

### 7. Các tính chất tôpô của ảnh của một đường

#### Mệnh đề 15 {#ta-iii-s2-prop-15 .statement tag=01XS}

Ảnh của một đường trong một không gian tôpô tách là một không gian tôpô compact, mêtric hóa được, liên thông và liên thông địa phương bởi các cung.

Cho X là một không gian tôpô tách và $c:\mathbf{I}\rightarrow X$ là một ánh xạ liên tục. Gọi R là quan hệ tương đương $c(s) =c(t)$ trong $\mathbf{I}$. Không gian tôpô $c(\mathbf{I})$ là tách (TG, I, p. 63, hệ quả 1), không gian $\mathbf{I}/R$ là quasi-compact (TG, I, p. 62, th. 2), do đó song ánh $\mathbf{I}/R\rightarrow c(\mathbf{I})$ suy ra từ $c$ là một đồng phôi (TG, I, p. 63, hệ quả 2). Do đó, không gian $c(\mathbf{I})$ là compact, mêtric hóa được (TG, IX, p. 22, mệnh đề 17), liên thông (TG, I, p. 82, mệnh đề 6) và liên thông địa phương bởi các cung (III, p. 261, mệnh đề 8).

#### Định lý 1 (Hahn và Mazurkiewicz) {#ta-iii-s2-thm-1 .statement tag=01XT}

Mọi không gian tôpô mêtric hóa được, compact, khác rỗng, liên thông và liên thông địa phương đều đồng phôi với một không gian thương của đoạn $[0,1]$.

#### Bổ đề 4 {#ta-iii-s2-lem-4 .statement tag=01XU}

Cho K là một không gian tôpô compact và $\mathscr{R}$ là một tập hợp các tập con mở của K phủ K. Tồn tại một lân cận V của cấu trúc đều của K (TG, II, p. 27, th. 1) sao cho, với mọi $x\in K$, $V(x)$ được chứa trong một trong các tập hợp thuộc $\mathscr{R}$.

Với mọi điểm $x$ của K, tồn tại một lân cận $W_x$ của cấu trúc đều của K sao cho $W_x(x)$ được chứa trong một trong các tập hợp thuộc $\mathscr{R}$. Gọi $V_x$ là một lân cận của cấu trúc đều của K sao cho $\overset{2}{V_{x}}$ được chứa trong $W_x$. Các phần trong của các $V_x(x)$ phủ K; vì không gian K là compact, tồn tại một tập con hữu hạn F của K sao cho họ $(V_y(y))_{y\in F}$ là một phủ của K (TG, I, p. 59). Gọi V là giao của họ $(V_y)_{y\in F}$; tập hợp V là một lân cận của cấu trúc đều của K. Với mọi điểm $x\in K$, tồn tại một điểm $y\in F$ sao cho $x$ thuộc $V_y(y)$. Do đó, tập hợp

$V(x)$ được chứa trong $\overset{2}{V_{y}}(y)$, do đó trong một trong các tập hợp thuộc $\mathscr{R}$.

#### Bổ đề 5 {#ta-iii-s2-lem-5 .statement tag=01XV}

Cho X và Y là các không gian đều và $f$ là một ánh xạ từ X vào Y. Cho $\mathscr{F}$ là một tập hợp các tập con đóng của X phủ X và có các tính chất sau:

(i) Tồn tại một tập hợp $F_0\in \mathscr{F}$ giao với mọi tập hợp $F\in \mathscr{F}$;

(ii) Với mọi lân cận U của cấu trúc đều của X, chỉ có một số hữu hạn các tập hợp $F\in \mathscr{F}$ không nhỏ cấp U;

(iii) Với mọi lân cận V của cấu trúc đều của Y, chỉ có một số hữu hạn các tập hợp $F\in \mathscr{F}$ sao cho $f(F)$ không nhỏ cấp V.

Do đó, nếu hạn chế của $f$ trên mỗi tập hợp $F\in \mathscr{F}$ là liên tục, thì $f$ là liên tục.

Cho $x$ là một điểm của X. Bây giờ chứng minh rằng $f$ liên tục tại $x$. Tồn tại một tập hợp $F_1\in \mathscr{F}$ sao cho $x\in F_1$. Hạn chế của $f$ trên $F_0\cup F_1$ là liên tục (TG, I, p. 19, mệnh đề 4). Bằng cách thay thế $F_0$ bởi $F_0\cup F_1$, ta rút gọn về trường hợp $x\in F_0$.

Cho V là một lân cận của cấu trúc đều trên Y. Chọn

một lân cận $V'$ của cùng cấu trúc đều này sao cho $\overset{2}{V'}\subset V$. Vì hạn chế của $f$ trên $F_0$ là liên tục, tồn tại một lân cận U của cấu trúc đều trên X sao cho $f(z)\in V'(f(x))$ với mọi $z\in F_0\cap U(x)$. Cho $U'$ là một lân cận của cấu trúc đều trên X

sao cho $\overset{2}{U'}\subset U$. Gọi A là hợp của $F_0$, của các tập hợp $F\in \mathscr{F}$ không nhỏ cấp $U'$ và của các tập hợp sao cho $f(F)$ không nhỏ cấp $V'$. Theo giả thiết, A là hợp của một số hữu hạn các tập hợp thuộc $\mathscr{F}$, và hạn chế của $f$ trên A là liên tục (loc. cit.). Do đó tồn tại một lân cận W của $x$ trong X, được chứa trong $U'(x)$, sao cho $f(y)\in V(f(x))$ với $y\in A\cap W$. Để kết luận, chỉ cần chứng minh rằng ta cũng có $f(y)\in V(f(x))$ với mọi điểm $y\in (X-A)\cap W$. Cho $y$ là một điểm như vậy. Cho F là một phần tử của $\mathscr{F}$ sao cho $y\in F$. Theo định nghĩa của A, F là nhỏ cấp $U'$ và $f(F)$ là nhỏ cấp $V'$. Theo giả thiết, F gặp $F_0$. Cho $z\in F\cap F_0$. Ta có $z\in U'(y)$ vì F là nhỏ cấp $U'$ và $y\in U'(x)$ vì W

được chứa trong $U'(x)$, do đó $z\in \overset{2}{U'}(x)$ và a fortiori $z\in U(x)$. Nhưng khi đó, vì $z$ thuộc $F_0$, ta có $f(z)\in V'(f(x))$. Hơn nữa $f(F)$ là nhỏ cấp $V'$, do đó $f(y)\in V'(f(z))$. Suy ra ta có

$f(y)\in \overset{2}{V'}(f(x))$ và cuối cùng $f(y)\in V(f(x))$. Điều này kết thúc chứng minh của bổ đề 5.

Bây giờ chứng minh định lý 1. Cho X là một không gian metric compact khác rỗng, liên thông và liên thông địa phương. Một không gian như vậy liên thông bởi các cung và liên thông địa phương bởi các cung (III, p. 267, hệ quả 2). Theo hệ quả và ví dụ của III, p. 270, tồn tại một ánh xạ liên tục và toàn ánh $f$ từ tập hợp Cantor tam phân K (TG, IV, p. 9, ví dụ) vào X. Ta sẽ xây dựng một mở rộng liên tục $g$ của $f$ tới $[0,1]$, điều này sẽ chứng minh định lý 1.

Cho $\varepsilon$ là một số thực $>0$. Các tập con mở và liên thông cung của X có đường kính $\leqslant \varepsilon$ phủ X. Gọi $\mathscr{R}$ là tập hợp các ảnh nghịch đảo của chúng qua $f$: đó là một tập hợp các tập mở của K phủ K. Theo Bổ đề 4 của III, p. 272, tồn tại một số thực $\alpha  >0$ sao cho mọi hình cầu đóng của K bán kính $\alpha$ đều được chứa trong một phần tử của $\mathscr{R}$. Đặc biệt, nếu $t$ và $t'$ là các điểm của K sao cho $|t-t'|\leqslant \alpha$, thì tồn tại một đường trong X nối $f(t)$ với $f(t')$ có ảnh có đường kính $\leqslant \varepsilon$.

Đoạn văn trước cho phép xây dựng bằng quy nạp một dãy tăng ngặt $(n_k)_{k\geqslant 0}$ các số nguyên $\geqslant$ 0 có tính chất sau: với mọi số nguyên $k\geqslant 0$ và mọi cặp $(t, t')$ các điểm của K sao cho $|t-t'|\leqslant 3^{-n_k}$, tồn tại một đường trong X nối $f(t)$ với $f(t')$ có ảnh có đường kính $\leqslant 2^{-k}$. Phần bù của K trong $[0,1]$ là hợp của một họ $(I_{n,p})$ các khoảng mở rời nhau từng đôi một, trong đó $n$ chạy qua tập hợp các số nguyên $\geqslant 0$ và $p$ chạy qua tập hợp các số nguyên giữa 1 và $2^n$ (TG, IV, p. 9, ví dụ). Xét một trong các khoảng này $I_{n,p}$ và viết nó là $]a, b[$. Các điểm $a$ và $b$ thuộc K và ta có $b-a= 3^{-n-1}$. Hàm $g$ được xác định trên khoảng $I_{n,p}$ theo cách sau: ta chọn một đường $c$ trong X nối $f(a)$ với $f(b)$, có ảnh có đường kính $\leqslant 2^{-k}$ nếu $n_k\leqslant n < n_{k+1}$, và đặt $g(t) =c(\frac{t-a}{b-a})$ với $t\in I_{n,p}$. Hàm $g: [0,1]\rightarrow X$ được định nghĩa như vậy mở rộng $f$. Nó liên tục trên K cũng như trên mỗi khoảng đóng $\overline{I_{n,p}}$. Các khoảng sau gặp K. Hơn nữa, với mọi số thực $\varepsilon  >0$, chỉ có hữu hạn các khoảng $\overline{I_{n,p}}$ có độ dài $> \varepsilon$, và chỉ có hữu hạn các khoảng $\overline{I_{n,p}}$ mà các ảnh của chúng qua $g$ có đường kính $> \varepsilon$. Theo Bổ đề 5, ánh xạ $g$ là liên tục.

### 8. Các đặc trưng của khoảng

#### Bổ đề 6 {#ta-iii-s2-lem-6 .statement tag=01XW}

Cho D là một tập sắp thứ tự toàn phần đếm được, không rút gọn thành một phần tử, có một phần tử nhỏ nhất và một phần tử lớn nhất. Giả sử rằng D không có khe hở (E, III, p. 73, bài tập 19), nghĩa là mọi khoảng mở $]x, y[$, trong đó $x$ và $y$ là các phần tử của D sao cho $x < y$, đều khác rỗng. Khi đó tồn tại một đẳng cấu của các tập hợp có thứ tự từ $\mathbf{I}\cap \mathbf{Q}$ lên D.

Cho $a$ là phần tử nhỏ nhất và $b$ là phần tử lớn nhất của D. Theo giả thiết, ta có $b=\not a$ và $]a, x[=\not\emptyset$ với mọi $x\in D-{a}$. Tập hợp D$-{a}$ được sắp thứ tự toàn phần, không rỗng và không có phần tử nhỏ nhất; do đó nó là vô hạn (E, III, p. 34, hệ quả 1 của mệnh đề 3). Các tập hợp $\mathbf{I}\cap \mathbf{Q}$ và D, vô hạn và đếm được, là tương đương lực lượng với $\mathbf{N}$.

Chọn các song ánh $n\mapsto a_n$ và $n\mapsto b_n$ của $\mathbf{N}$ lên $\mathbf{I}\cap \mathbf{Q}$ và D tương ứng, sao cho $a_0= 0,a_1= 1,b_0=a,b_1=b$. Tồn tại duy nhất một ánh xạ tăng ngặt $f:\mathbf{I}\cap \mathbf{Q}\rightarrow D$ có các tính chất sau: ta có $f(0) =a$ và $f(1) =b$; với $n\geqslant 2$, ta có $f(a_n) =b_m$, trong đó $m$ là số tự nhiên nhỏ nhất sao cho ánh xạ của ${a_0, . . . , a_n}$ vào D trùng với $f$ trên ${a_0, . . . , a_{n-1}}$ và gửi $a_n$ lên $b_m$ là tăng ngặt. Thật vậy, các tính chất này định nghĩa $f(a_n)$ bằng quy nạp theo $n$, sự tồn tại của số nguyên $m$ được bảo đảm bởi sự kiện rằng D không có khe hở.

Vì ánh xạ $f$ là tăng ngặt và $\mathbf{I}\cap \mathbf{Q}$ được sắp thứ tự toàn phần, $f$ định nghĩa một đẳng cấu của các tập hợp có thứ tự từ $\mathbf{I}\cap \mathbf{Q}$ lên ảnh của nó (E, III, p. 14, mệnh đề 11). Còn lại đối với chúng ta là chứng minh rằng $f$ là toàn ánh. Để làm điều này, ta hãy chứng minh bằng quy nạp rằng $b_m$ thuộc ảnh của $f$ với mọi $m\in \mathbf{N}$.

Ta có $b_0=f(0)$ và $b_1=f(1)$. Giả sử ta có $m\geqslant 2$ và với $0\leqslant k\leqslant m-1$, tồn tại $c_k\in \mathbf{I}\cap \mathbf{Q}$ sao cho $f(c_k) =b_k$. Ta có $c_0= 0$ và $c_1= 1$, vì $f$ là đơn ánh. Xét số nguyên nhỏ nhất $n\in \mathbf{N}$ sao cho $a_n$ không thuộc $\{c_0, . . . , c_{m-1}\}$ và ánh xạ $g$ từ $\{c_0, . . . , c_{m-1}, a_n\}$ vào D trùng với $f$ trên $\{c_0, . . . , c_{m-1}\}$ và ánh xạ $a_n$ lên $b_m$ là tăng ngặt; một số nguyên như vậy tồn tại vì $\mathbf{I}\cap \mathbf{Q}$ không có khoảng trống. Gọi $f'$ là ánh xạ từ $\{a_0, . . . , a_n\}$ vào D trùng với $f$ trên $\{a_0, . . . , a_{n-1}\}$ và ánh xạ $a_n$ lên $b_m$. Ta chứng minh rằng nó là tăng ngặt. Lấy $j\in  \{0, . . . , n-1\}$; theo định nghĩa của số nguyên $n$, tồn tại $k\in  \{0, . . . , m-1\}$ sao cho $a_j=c_k$, hoặc $a_j< c_k$ và $b_m\geqslant f(c_k)$, hoặc $a_j> c_k$ và $b_m\leqslant f(c_k)$. Giả sử $b_k< b_m$; khi đó ta có $g(c_k) =f(c_k) =b_k< b_m=g(a_n)$, do đó $c_k< a_n$ vì $g$ là tăng ngặt, suy ra $a_j\leqslant c_k< a_n$; hơn nữa, $f'(a_j) =$ $f(a_j)\leqslant f(c_k) =b_k< b_m=f'(a_n)$. Tương tự, nếu $b_k> b_m$, ta được $a_n< c_k\leqslant a_j$ và $f'(a_j) =f(a_j)\geqslant f(c_k) =b_k> b_m=f'(a_n)$. Vì bản thân $f$ là tăng ngặt, suy ra ánh xạ $f'$ là tăng ngặt.

Nếu $m'$ là số nguyên sao cho $f(a_n) =b_{m'}$, thì $m'\leqslant m$, theo định nghĩa của $f$. Nếu $m'< m$, ta có $f(a_n) =b_{m'}=f(c_{m'})$, do đó $a_n=c_{m'}$, vì $f$ là đơn ánh, điều này mâu thuẫn với định nghĩa của $a_n$. Vậy $m'=m$ và $f(a_n) =b_m$, điều này chứng minh rằng $b_m$ thuộc ảnh của $f$ và hoàn tất, bằng quy nạp, chứng minh tính toàn ánh của $f$.

#### Mệnh đề 16 {#ta-iii-s2-prop-16 .statement tag=01XX}

Cho E là một tập sắp thứ tự toàn phần không chỉ gồm một phần tử. Giả sử mọi tập con của E đều có một supremum và tồn tại một tập con đếm được của E gặp mọi khoảng mở $]x, y[$, trong đó $x$ và $y$ là các phần tử của E sao cho $x < y$. Khi đó tồn tại một đẳng cấu của các tập hợp có thứ tự từ $\mathbf{I}$ lên E.

Vì $\emptyset$ và E đều có một supremum trong E, nên E có một phần tử nhỏ nhất $a$ và một phần tử lớn nhất $b$. Hai phần tử này phân biệt vì E không chỉ gồm một phần tử. Gọi $D'$ là một tập con đếm được của E gặp mọi khoảng mở của E có dạng $]x, y[$, với $x < y$. Đặt $D = D'\cup  \{a, b\}$. Tập D được sắp thứ tự toàn phần và không có khoảng trống. Theo bổ đề 6, tồn tại một đẳng cấu của các tập hợp có thứ tự $f$ từ $\mathbf{I}\cap \mathbf{Q}$ lên D.

Với mọi $t\in \mathbf{I}$, gọi $g(t)$ là supremum trong E của $f([0, t]\cap \mathbf{Q})$. Với mọi $x\in E$, gọi $h(x)$ là supremum trong $\mathbf{I}$ của $f^{-1}([a, x]\cap D)$. Các ánh xạ $g:\mathbf{I}\rightarrow E$ và $h: E\rightarrow \mathbf{I}$ được định nghĩa như vậy là tăng, $g$ trùng với $f$ trên $\mathbf{I}\cap \mathbf{Q}$ và $h$ trùng với $f^{-1}$ trên D.

Do đó ta có $g(h(y)) =y$ với mọi $y\in D$. Cho $x\in E$. Nếu có $g(h(x))> x$, thì khoảng $]x, g(h(x))[$ sẽ chứa một điểm $y$ của D và các quan hệ $g(h(y)) =y < g(h(x))$ sẽ mâu thuẫn với việc $g\circ h$ là tăng. Tương tự, ta không có $g(h(x))< x$. Do đó ta có $g(h(x)) =x$, điều này chứng tỏ rằng $g\circ h$ là ánh xạ đồng nhất của E. Tương tự, ta chứng minh được rằng $h\circ g$ là ánh xạ đồng nhất của $\mathbf{I}$. Vậy $g:\mathbf{I}\rightarrow E$ và $h: E\rightarrow \mathbf{I}$ là các đẳng cấu tương hỗ của các tập hợp có thứ tự.

#### Nhận xét {#ta-iii-s2-n8-rem-1 .statement tag=01XY}

Cho E là một tập sắp thứ tự toàn phần. Tập hợp các khoảng mở của E (bị chặn hoặc không) ổn định đối với giao hữu hạn. Nó là một cơ sở của một tôpô $\mathscr{T}_0(E)$ trên E (TG, I, p. 91, exerc. 5). Tôpô $\mathscr{T}_0(\mathbf{I})$ trùng với tôpô cảm sinh trên $\mathbf{I}$ bởi tôpô của $\mathbf{R}$. Suy ra rằng, trong mệnh đề 16, mọi đẳng cấu của các tập hợp có thứ tự từ $\mathbf{I}$ lên E đều là một đồng phôi từ $\mathbf{I}$ lên không gian tôpô thu được bằng cách trang bị cho E tôpô $\mathscr{T}_0(E)$.

#### Hệ quả {#ta-iii-s2-n8-cor-1 .statement tag=01XZ}

Cho R là một quan hệ tương đương trong $\mathbf{I}$. Các điều kiện sau là tương đương:

(i) Mọi lớp tương đương theo R đều là một khoảng đóng của $\mathbf{I}$, phân biệt với $\mathbf{I}$;

(ii) Tồn tại một ánh xạ toàn ánh tăng $u:\mathbf{I}\rightarrow \mathbf{I}$ sao cho R là quan hệ tương đương liên kết với $u$.

Một ánh xạ $u$ như vậy, khi tồn tại, là liên tục và xác định, bằng cách chuyển qua thương, một đồng phôi từ $\mathbf{I}/R$ lên $\mathbf{I}$.

Ta sẽ ký hiệu $p:\mathbf{I}\rightarrow \mathbf{I}/R$ là toàn cấu chính tắc.

Giả sử điều kiện (i) được thỏa mãn. Đối với các lớp tương đương A và B theo R, viết $A<B$ nếu có $a < b$ với mọi $a\in A$ và mọi $b\in B$. Trong $\mathbf{I}/R$, quan hệ « A = B hoặc $A<B$ » là một quan hệ thứ tự. Thật vậy, nó phản xạ; nó phản đối xứng vì không thể đồng thời có $A<B$ và $B<A$; nó bắc cầu vì các quan hệ $A<B$ và $B<C$ kéo theo $A<C$. Nếu A và B là các phần tử phân biệt của $\mathbf{I}/R$, thì chúng là các khoảng đóng rời nhau của $\mathbf{I}$, và khi đó ta có hoặc $A<B$, hoặc $B<A$. Được trang bị với quan hệ thứ tự được xác định như vậy, $\mathbf{I}/R$ do đó được sắp thứ tự toàn phần. Ánh xạ $p:\mathbf{I}\rightarrow \mathbf{I}/R$ là tăng.

Tập $\mathbf{I}/R$ không thu gọn thành một phần tử, nhờ vào (i).

Cho F là một tập con của $\mathbf{I}/R$. Ta chứng minh rằng F có một cận trên nhỏ nhất trong $\mathbf{I}/R$. Đặt $F'=\overset{-1}{p}(F)$; ký hiệu a là cận trên nhỏ nhất của $F'$ trong $\mathbf{I}$ và A là lớp tương đương của a theo R. Vì $a$ là một cận trên của $F'$ trong $\mathbf{I}$, A là một cận trên của F trong $\mathbf{I}/R$. Ngược lại, cho $B\in \mathbf{I}/R$ là một cận trên của F; đặt $b=$ sup(B). Mọi phần tử của $F'$ khi đó đều bị chặn trên bởi $b$. Do đó ta có $a\leqslant b$. Vì các lớp tương đương theo R là các khoảng đóng, $a$ thuộc A và $b$ thuộc B. Do đó ta có $A =p(a)\leqslant p(b) = B$. Điều này chứng minh rằng A là cận trên nhỏ nhất của F.

Cho A và B là các phần tử của $\mathbf{I}/R$ sao cho $A<B$. Gọi a là cận dưới lớn nhất của A và b là cận trên nhỏ nhất của B. Vì $a\in A$ và $b\in B$, ta có $a < b$. Lớp tương đương theo R của mọi phần tử của $]a, b[$ là một phần tử của khoảng $]A,B[$ của $\mathbf{I}/R$. Vì $\mathbf{I}\cap \mathbf{Q}$ giao với $]a, b[$, ảnh của nó qua $p$ giao với $]A,B[$.

Như vậy ta đã chứng minh rằng tập sắp thứ tự toàn phần $\mathbf{I}/R$ thỏa mãn các giả thiết của mệnh đề 16. Do đó tồn tại một đẳng cấu của các tập hợp có thứ tự $f:\mathbf{I}/R\rightarrow \mathbf{I}$. Ánh xạ $u=f\circ p$ là một ánh xạ toàn ánh và tăng từ $\mathbf{I}$ lên $\mathbf{I}$ và quan hệ tương đương liên kết với $u$ là quan hệ R; điều này chứng minh rằng điều kiện (ii) được thỏa mãn.

Ngược lại, giả sử rằng điều kiện (ii) được thỏa mãn. Cho $u:\mathbf{I}\rightarrow \mathbf{I}$ là một ánh xạ tăng và toàn ánh sao cho R là quan hệ tương đương liên kết với $u$.

Cho $a$ là một điểm của $\mathbf{I}$. Tập hợp $A =\overset{-1}{u}(a)$ là một khoảng của $\mathbf{I}$, vì ánh xạ $u$ là tăng. Vì $u$ là toàn ánh, A không rỗng cũng không bằng $\mathbf{I}$. Gọi $b$ là cận dưới lớn nhất của A trong $\mathbf{I}$. Ta có $u(b)\geqslant a$. Nếu $u(b)> a$, tồn tại $c\in ]a, u(b)[$ và $d\in \mathbf{I}$ sao cho $u(d) =c$ vì $u$ là toàn ánh. Vì $u$ là tăng và $a < u(d)< u(b),d$ lớn hơn mọi phần tử của A và ta có $d < b$, điều này mâu thuẫn với giả thiết rằng $b$ là cận dưới lớn nhất của A. Do đó ta có $u(b) =a$, nghĩa là $b\in A$. Tương tự ta chứng minh được rằng A chứa cận dưới lớn nhất của nó. Vậy tập hợp A là một khoảng đóng của $\mathbf{I}$, phân biệt với $\mathbf{I}$. Điều này chứng minh rằng điều kiện (i) được thỏa mãn.

Bây giờ ta chứng minh rằng ánh xạ $u$ là liên tục. Chỉ cần chứng minh rằng, với mọi $a\in \mathbf{I}$, các tập hợp $\overset{-1}{u}(]a,\rightarrow [)$ và $\overset{-1}{u}(]\leftarrow , a[)$ là mở. Gọi $b$ là cận dưới lớn nhất của $\overset{-1}{u}(a)$; ta có $u(b) =a$. Nếu $x\in \mathbf{I}$ thỏa mãn $u(x)> a$, ta tất yếu có $x > b$; ngược lại, nếu $x > b$, ta có $u(x)\geqslant a$ và $u(x)=\not a$ vì $b$ là cận dưới lớn nhất của $\overset{-1}{u}(a)$. Do đó $\overset{-1}{u}(]a,\rightarrow [) = ]b,\rightarrow [$, điều này chứng minh rằng ảnh ngược bởi $u$ của khoảng $]a,\rightarrow [$ là mở. Tương tự ta chứng minh rằng ảnh ngược của $]\leftarrow , a[$ là mở. Suy ra rằng ánh xạ $u$ là liên tục.

Ánh xạ $v:\mathbf{I}/R\rightarrow \mathbf{I}$ suy ra từ $u$ bằng cách chuyển qua thương khi đó là liên tục và song ánh. Vì $\mathbf{I}$ là compact, $\mathbf{I}/R$ là quasi-compact (TG, I, p. 62, th. 2) và $v$ là một đồng phôi (TG, I, p. 63, cor. 2).

#### Mệnh đề 17 {#ta-iii-s2-prop-17 .statement tag=01Y0}

Cho X là một không gian tôpô liên thông và compact. Cho $a$ là một điểm của X, cho U là một tập con mở đóng khác rỗng của X $-\{a\}$.

(a) Bao đóng $\overline{U}$ của U trong X bằng $U\cup  \{a\}$ và là liên thông.

(b) Cho $a'$ là một điểm của X phân biệt với $a$, và cho $U'$ là một tập con mở và đóng khác rỗng của X $-\{a'\}$. Nếu $a\notin U'$ và nếu $\overline{U}\cap \overline{U'}=\not\emptyset$, thì $\overline{U'}\subset U$. Ngược lại, nếu $a\in U'$ và X $= U\not\cup U'$, thì $\overline{U}\subset U'$.

(c) Tồn tại một điểm $b$ của U sao cho X $-\{b\}$ là liên thông.

Chứng minh mệnh đề a). Ký hiệu bởi V phần bù của U trong X $-\{a\}$. Vì U là đóng trong X $-\{a\}$, nên V là mở trong X$-\{a\}$ và a fortiori trong X. Do đó ta có $U\subset \overline{U}\subset X-V = U\cup \{a\}$. Tương tự, U là một tập con mở của X. Vì X là liên thông, U không đóng trong X, do đó đẳng thức $\overline{U}= U\cup  \{a\}$. Tương tự ta có $\overline{V}= V\cup  \{a\}$.

Cho F và G là các tập con đóng rời nhau của $\overline{U}$ sao cho $U = F\cup G$. Giả sử rằng $a\in G$ và ta chứng minh rằng F là rỗng; ta sẽ lập luận theo cùng một cách nếu $a\in F$. Tập hợp $G\cup V = G\cup \overline{V}$ là một tập con đóng của X, rời nhau với F, và ta có $X =\overline{U}\cup V = F\cup (G\cup V)$. Vì X là liên thông và G khác rỗng, F là rỗng. Điều này chứng minh rằng $\overline{U}$ là liên thông.

Chứng minh b). Giả sử rằng $a\notin U'$ và rằng $\overline{U}\cap \overline{U'}=\not\emptyset$. Theo mệnh đề a), ta có $U = U\cup  \{a\}$ và $\overline{U'}= U'\cup  \{a'\}$. Vì $a\notin U'$ và $a=\not a'$, các tập con U và $\overline{U'}$ có một điểm chung. Vẫn theo a), $\overline{U'}$ là một tập con liên thông của X; vì nó được chứa trong X$-\{a\}$ và nó gặp tập con mở và đóng U của tập hợp sau, ta có $\overline{U'}\subset U$, điều này đã được chứng minh. Mệnh đề thứ hai suy ra từ mệnh đề thứ nhất bằng cách xét các phần bù trong X của $\overline{U}$ và $\overline{U'}$ tương ứng.

Cuối cùng ta chứng minh mệnh đề c). Giả sử, bằng phản chứng, rằng, với mọi $x\in U$, tập hợp X $-\{x\}$ không liên thông và chọn các tập con $U_x$ và $V_x$, mở và đóng trong X $-\{x\}$, rời nhau và khác rỗng, sao cho X $-\{x\}= U_x\cup V_x$ và $a\in V_x$. Theo mệnh đề b), áp dụng cho các tập con mở và đóng U, $U_x$ của X$-\{a\}$ và X$-\{x\}$ tương ứng, ta có $\overline{U_x}\subset U$ với mọi $x\in U$. Gọi $x$ và $y$ là các điểm của U sao cho $x\in U_y$; khi đó ta có $x=\not y$. Lại theo mệnh đề b), áp dụng cho các tập con mở và đóng $U_x$ và $U_y$ của X $-\{x\}$ và X $-\{y\}$, quan hệ $x\in U_y$ kéo theo quan hệ $\overline{U_x}\subset \overline{U_y}$. Do đó, các quan hệ $x\in U_y$ và $\overline{U_x}\subset \overline{U_y}$ là tương đương.

Tập hợp các tập con S của U sao cho $\bigcap_{x\in S}\overline{U_x}=\not\emptyset$ có đặc trưng hữu hạn (E, III, p. 34), vì không gian X là compact. Theo E, III, p. 35, th. 1, tồn tại một tập con cực đại S của U sao cho $C =\bigcap_{x\in S}\overline{U_x}$ là khác rỗng. Gọi $c$ là một điểm của C. Với mọi phần tử $x$ của S, ta có $c\in \overline{U_x}$, do đó $c\in U$ và khi đó $\overline{U_c}\subset \overline{U_x}$. Do đó, ta có $\overline{U_c}\subset C$ và khi đó, bởi tính cực đại của S, $C = U_c$. Với mọi $x\in C$ sao cho $x=\not c$, ta cũng có $\overline{U_x}\subset \overline{U_c}$ và $\overline{U_x}= U\not_c$. Bởi tính cực đại của S, $C =\{c\}$, suy ra $\overline{U_c}=\{c\}$, điều này mâu thuẫn với giả thiết rằng $U_c$ là một tập con mở và đóng khác rỗng của X $-\{c\}$.

#### Hệ quả {#ta-iii-s2-n8-cor-2 .statement tag=01Y1}

Cho X là một không gian tôpô compact liên thông, gọi N là tập hợp các điểm của X mà phần bù của chúng là liên thông. Tập X là tập con liên thông và compact duy nhất của X chứa N.

Cho S là một tập con liên thông và compact của X sao cho $N\subset S$. Giả sử rằng S $= X\not$ và lấy $x\in X-S$. Theo giả thiết, X $-\{x\}$ không liên thông; do đó tồn tại các tập con mở và đóng U và V của X $-\{x\}$, rời nhau và khác rỗng, sao cho X $-\{x\}= U\cup V$. Ta có thể giả sử rằng $S\subset V$. Ta có $\overline{U}= U\cup \{x\}$ và $V = V\cup  \{x\}$ và các không gian này là liên thông (III, p. 278, prop. 17, a)). Theo mệnh đề c) của mệnh đề này, tồn tại $y\in U$ sao cho X $-\{y\}$ là liên thông, điều này mâu thuẫn với các bao hàm $N\subset S\subset V$.

#### Bổ đề 7 {#ta-iii-s2-lem-7 .statement tag=01Y2}

Một không gian tôpô liên thông địa phương T. Cho $\mathscr{U}$ là một tập hợp lọc tăng của các phần mở của T, có hợp là T. Với $t\in T$ và $U\in \mathscr{U}$, ký hiệu $U_t$ là thành phần liên thông của $t$ trong U nếu $t\in U$ và đặt $U_t=\emptyset$ nếu $t\notin U$. Với mọi $t\in T,\bigcup_{U\in\mathscr{U}}U_t$ là thành phần liên thông của $t$ trong T.

Với $t\in T$, đặt $C_t=\bigcup_{U\in\mathscr{U}}U_t$. Ta có $t\in C_t$. Các tập hợp $U_t$ là mở và liên thông và điều tương tự cũng đúng đối với $C_t$ vì ta có $t\in U_t$ nếu $U_t=\not\emptyset$ (TG, I, p. 81, Mệnh đề 2). Cho $u,v$ là các điểm của T sao cho $C_u\cap C_v=\not\emptyset$. Cho $t$ là một điểm của $C_u\cap C_v$; cho $U\in \mathscr{U}$ sao cho $t\in U_u$ và cho $V\in \mathscr{U}$ sao cho $v\in V_v$. Vì $\mathscr{U}$ là lọc tăng, tồn tại $W\in \mathscr{U}$ chứa $U\cup V$. Khi đó, $W_u\cap W_v=\not\emptyset$, do đó $W_u= W_v$. Nói chung, ta có $W'_u= W'_v$ với mọi $W'\in \mathscr{U}$ sao cho $W\subset W'$, do đó $C_u= C_v$. Điều này chứng minh rằng các tập hợp có dạng $C_t$ tạo thành một phân hoạch của T thành các tập con mở liên thông. Do đó, với mọi $t\in T$, $C_t$ là thành phần liên thông của $t$ trong T.

#### Định lý 2 {#ta-iii-s2-thm-2 .statement tag=01Y3}

Cho X là một không gian tôpô compact liên thông có một tập con đếm được trù mật khắp nơi. Cho $a,b$ là các điểm phân biệt của X. Các điều kiện sau là tương đương:

(i) Tồn tại một đồng phôi $f:\mathbf{I}\rightarrow X$ sao cho $f(0) =a$ và $f(1) =b$;

(ii) Mọi tập con liên thông của X chứa $\{a, b\}$ đều bằng X ;

(iii) Không gian X là liên thông địa phương và mọi tập con compact liên thông của X chứa $\{a, b\}$ đều bằng X ;

(iv) Với mọi $x\in X-\{a, b\}$, không gian X $-\{x\}$ không liên thông.

Mệnh đề (i) kéo theo tất cả các mệnh đề còn lại.

Cho $x$ là một điểm của X $-\{a, b\}$. Vì X $-\{x\}$ chứa $\{a, b\}$, mệnh đề (ii) kéo theo rằng nó không phải là một tập con liên thông của X, do đó (ii) kéo theo (iv).

Ta chứng minh rằng (iii) kéo theo (iv). Giả sử các giả thiết của (iii) được thỏa mãn. Cho $x\in X-\{a, b\}$ và giả sử rằng X$-\{x\}$ là liên thông. Cho T là không gian X $-\{x\}$ và cho $\mathscr{U}$ là tập hợp các tập con của T có dạng X-V, trong đó V là một lân cận compact của $x$. Theo Bổ đề 7, tồn tại một lân cận compact V của $x$ sao cho $a$ và $b$ thuộc cùng một thành phần liên thông của X-V. Chúng đặc biệt thuộc cùng một thành phần liên thông của $X-\mathring{V}$; đây là một tập hợp compact liên thông của X, phân biệt với X, điều này mâu thuẫn với giả thiết (iii).

Còn lại phải chứng minh rằng mệnh đề (iv) kéo theo điều kiện (i).

Cho $x$ là một điểm của X $-\{a, b\}$ và cho U, V là các tập con mở và đóng, rời nhau và khác rỗng của X$-\{x\}$, sao cho X$-\{x\}= U\cup V$. Theo III, p. 278, Mệnh đề 17, c), tồn tại một điểm của U (tương ứng của V) mà phần bù của nó trong X là liên thông. Vì X chỉ nhận hai điểm như vậy, $a$ và $b$, một trong chúng, giả sử $a$, được chứa trong U và điểm kia trong V. Theo chỗ đã dẫn, một tập con mở và đóng khác rỗng, $U'$ của U, chứa một điểm của $\{a, b\}$, do đó chứa $a$. Áp dụng điều này cho $U-U'$, suy ra rằng $U = U'$. Do đó, U là liên thông; nó là thành phần liên thông của $a$ trong X$-\{x\}$. Tương tự, V là thành phần liên thông của $b$ trong X $-\{x\}$.

Với mọi $x\in X-\{a, b\}$, do đó ký hiệu bởi $U_x$ và $V_x$ các thành phần liên thông của $a$ và $b$ trong X $-\{x\}$. Từ những điều trên, chúng là mở và đóng trong X $-\{x\}$, rời nhau, và hợp của chúng bằng X $-\{x\}$.

Ký hiệu bởi $\preccurlyeq$ quan hệ trong X được định nghĩa như sau: một mặt, $a\preccurlyeq x$ và $x\preccurlyeq b$ với mọi $x\in X$, mặt khác, nếu $x$ và $y$ thuộc X $-\{a, b\}$, thì $x\preccurlyeq y$ nếu $x\in \overline{U_y}$. Với $x$ và $y$ trong X $-\{a, b\}$, các tập con $V_x$ và $V_y$ có điểm $b$ chung, quan hệ $x\preccurlyeq y$ thực tế tương đương với mệnh đề $\overline{U_x}\subset \overline{U_y}($III, p. 278, Mệnh đề 17, b)). Suy ra rằng quan hệ $\preccurlyeq$ là một quan hệ thứ tự trong X.

Cho $x$ và $y$ là các điểm của X sao cho không có $x\preccurlyeq y$. Tất nhiên, $x=\not a$ và $y=\not b$, và $x\in V_y$. Nếu $x=b$ hoặc $y=a$, ta có $y\preccurlyeq x$. Khi đó giả sử $x$ và $y$ phân biệt với $a$ và $b$. Vì các tập hợp $U_x$ và $U_y$ có điểm $a$ chung, ta có bao hàm $\overline{V_x}\subset \overline{V_y}($loc. cit.), do đó, lấy bao đóng của các phần bù, $\overline{U_y}\subset \overline{U_x}$ và, a fortiori, $y\preccurlyeq x$. Quan hệ $\preccurlyeq$ trong không gian X vì vậy là một quan hệ thứ tự toàn phần. Với mọi $x\in X-\{a, b\}$, hơn nữa ta có $U_x= ]\leftarrow , x[$ và $V_x= ]x,\rightarrow [$; với $x, y\in X-\{a, b\}$, ta có $]x, y[ = U_y\cap V_x$. Khi $x, y$ chạy qua các điểm của X $-\{a, b\}$, các tập hợp $U_y\cap V_x$, các tập hợp $U_y$ và các tập hợp $V_x$ tạo thành một cơ sở của một tôpô trên X. Gọi $\widetilde{X}$ là không gian tôpô tương ứng với nó và gọi $i: X\rightarrow \widetilde{X}$ là ánh xạ đồng nhất của X. Vì, với mọi $x\in X$, các tập hợp $U_x$ và $V_x$ là mở trong X, ánh xạ $i$ là liên tục.

Không gian $\widetilde{X}$ là tách biệt. Thật vậy, cho $x$ và $y$ là các điểm phân biệt của $\widetilde{X}$ sao cho $x\preccurlyeq y$. Các tập hợp $]\leftarrow , y[$ và $]x,\rightarrow [$ là các lân cận mở của $x$ và $y$; nếu chúng có một điểm chung $z,]\leftarrow , z[$ và $]z,\rightarrow [$ khi đó là các lân cận mở rời nhau của $x$ và $y$. Vì X compact, ánh xạ $i$ do đó là một phép đồng phôi (TG, I, p. 63, cor. 2).

Do đó, ảnh bởi $i$ của một tập con đếm được trù mật khắp nơi của X gặp mọi khoảng mở khác rỗng của tập hợp có thứ tự $(X,\preccurlyeq )$. Từ đó suy ra theo Mệnh đề 16 của III, p. 276 rằng tồn tại một đẳng cấu $c$ của tập hợp có thứ tự $\mathbf{I}$ lên $(X,\prec )$. Theo nhận xét sau mệnh đề này, đẳng cấu này là một đồng phôi của $\mathbf{I}$ lên không gian tôpô $\widetilde{X}$. Ánh xạ $f=i^{-1}\circ c$ khi đó là một đồng phôi của $\mathbf{I}$ lên X, ánh xạ 0 lên $a$ và 1 lên $b$.

### 9. Các đường đi đơn ánh

#### Mệnh đề 18 {#ta-iii-s2-prop-18 .statement tag=01Y4}

Cho X là một không gian tôpô Hausdorff. Cho $a$ và $b$ là các điểm phân biệt của X thuộc cùng một thành phần liên thông theo cung của X. Tồn tại một đường đi đơn ánh nối $a$ với $b$ trong X.

Cho $f:\mathbf{I}\rightarrow X$ là một đường đi nối $a$ với $b$ trong X. Cho $\mathscr{U}$ là tập hợp các tập con mở U của $]0,1[$ sao cho $f(x) =f(y)$ đối với mọi thành phần liên thông $]x, y[$ của U.

#### Bổ đề 8 {#ta-iii-s2-lem-8 .statement tag=01Y5}

Tập hợp $\mathscr{U}$, có thứ tự bởi quan hệ bao hàm, là quy nạp.

Cho $\mathscr{V}$ là một tập con sắp thứ tự toàn phần của $\mathscr{U}$. Ta hãy chứng minh rằng hợp V của các tập hợp thuộc $\mathscr{V}$ là một phần tử của $\mathscr{U}$, nghĩa là, đối với mọi thành phần liên thông $]u, v[$ của V, ta có $f(u) =f(v)$.

Cho $x$ là một điểm của $]u, v[$. Cho $\mathscr{V}_x$ là tập hợp các $U\in \mathscr{V}$ sao cho $x\in U$; đối với một U như vậy, ký hiệu $]u_U, v_U[$ là thành phần liên thông của $x$ trong U. Ta có $u_{U'}\leqslant u_U< v_U\leqslant v_{U'}$ nếu U và $U'$ là các phần tử của $\mathscr{V}_x$ sao cho $U\subset U'$. Vì hợp theo $U\in \mathscr{U}_x$ của các $]u_U, v_U[$ bằng $]u, v[$ theo Bổ đề 7 của III, p. 280, ta có $u=$ lim $u_U$ và $v=$ lim $v_U$, trong đó các giới hạn được lấy theo tập hợp lọc $\mathscr{V}_x$. Vì ánh xạ $f$ liên tục và không gian tôpô X là Hausdorff, các đẳng thức $f(u_U) =f(v_U)$ đối với mọi $U\in \mathscr{V}_x$ kéo theo $f(u) =f(v)$, điều phải chứng minh.

Theo E, III, p. 20, Định lý 2, tồn tại một tập con mở U thuộc $\mathscr{U}$ là cực đại đối với quan hệ bao hàm.

Cho $g:\mathbf{I}\rightarrow X$ là ánh xạ được xác định như sau. Nếu $t\notin U$, ta đặt $g(t) =f(t)$; ngược lại, ký hiệu $]u, v[$ là thành phần liên thông của $t$ trong U, ta đặt $g(t) =f(u) =f(v)$, sao cho ánh xạ $g|[u, v]$ là hằng với ảnh $f(u)$.

Mệnh đề 18 suy ra từ bổ đề sau.

#### Bổ đề 9 {#ta-iii-s2-lem-9 .statement tag=01Y6}

Tồn tại một ánh xạ liên tục, tăng và toàn ánh $u:\mathbf{I}\rightarrow \mathbf{I}$ và một đường đi đơn $c:\mathbf{I}\rightarrow X$ nối $a$ với $b$ sao cho $g=c\circ u$.

Trước hết ta chứng minh rằng ánh xạ $g$ là liên tục. Cho $t$ là một điểm của $\mathbf{I}$. Nếu $t\in U,g$ là hằng trong một lân cận của $t$, do đó liên tục tại $t$. Giả sử rằng $t\notin U$ và W là một lân cận mở của $g(t)$ trong X. Cho V là một khoảng mở trong $\mathbf{I}$ chứa $t$ sao cho $f(V)\subset W$; một khoảng như vậy tồn tại vì $f$ liên tục tại $t$. Ta chứng minh rằng $g(V)\subset W$. Cho $x\in V$; nếu $x\notin U$, ta có $g(x) =f(x)$, do đó $g(x)\in W$. Giả sử tiếp rằng $x\in U$ và $]u, v[$ là thành phần liên thông của $x$ trong U. Nhận xét rằng $]u, v[$ không chứa $t$. Do đó, nếu $x < t$, ta có $x < v\leqslant t$ suy ra $v\in V$ và $g(x) =g(v) =f(v)\in f(V)\subset W$. Lập luận tương tự cho thấy rằng $g(x)\in W$ nếu $x > t$. Vậy $g$ liên tục tại $t$.

Cho $u$ và $v$ là các điểm của $\mathbf{I}$ sao cho $g(u) =g(v)$ và $u < v$. Ta chứng minh rằng $]u, v[\subset U$. Đặt $U'= U\cup ]u, v[$; đó là một tập con mở của $]0,1[$.

Nếu $u$ thuộc U, gọi $u'$ là cận dưới lớn nhất trong $\mathbf{I}$ của thành phần liên thông của $u$ trong U; đặt $u'=u$ nếu $u$ không thuộc U. Tương tự, nếu $v$ thuộc U, gọi $v'$ là cận trên nhỏ nhất trong $\mathbf{I}$ của thành phần liên thông của $v$ trong U; đặt $v'=v$ nếu $v$ không thuộc U. Khi đó, $]u', v'[$ là một thành phần liên thông của $U'$ và ta có $f(u') =g(u) =g(v) =f(v')$. Vì các thành phần liên thông của $U'$ phân biệt với $]u', v'[$ là các thành phần liên thông của U, nên tập mở $U'$ là một phần tử của $\mathscr{U}$. Vì U là một phần tử cực đại của $\mathscr{U}$ đối với quan hệ bao hàm, nên có $U'= U$ và $]u, v[$ được chứa trong U. Điều này chứng minh rằng $g$ là hằng trên khoảng $[u, v]$. Các thớ của $g$ do đó là các khoảng của $\mathbf{I}$, và các khoảng này là đóng vì $g$ liên tục.

Gọi R là quan hệ tương đương liên kết với $g$ và gọi $p$ là toàn cấu chính tắc của $\mathbf{I}$ lên $\mathbf{I}/R$. Tồn tại một ánh xạ liên tục duy nhất $g'$ của $\mathbf{I}/R$ vào X sao cho $g=g'\circ p$; ánh xạ này là đơn ánh. Theo hệ quả, III, p. 276, của mệnh đề 16, tồn tại một ánh xạ $u$, tăng, liên tục và toàn ánh, sao cho R là quan hệ tương đương liên kết với $u$. Vì không gian $\mathbf{I}$ là compact và không gian X là Hausdorff, ánh xạ $u$ là đóng, do đó ngặt (I, p. 18, ví dụ 2). Nó xác định, bằng cách chuyển qua thương, một đồng phôi $u'$ của $\mathbf{I}/R$ lên $\mathbf{I}$. Khi đó, ánh xạ $g'\circ (u')^{-1}$ của $\mathbf{I}$ vào X là một đường đi đơn ánh có điểm đầu $a$ và điểm cuối $b$.

### 10. Nâng của các đường đi

#### Định lý 3 {#ta-iii-s2-thm-3 .statement tag=01Y7}

Cho I là một khoảng của $\mathbf{R}$ và X là một không gian tôpô khác rỗng và Hausdorff. Cho $p: X\rightarrow I$ là một ánh xạ liên tục, mở và thực sự mà các thớ của nó là hoàn toàn rời rạc (TG, I, p. 83). Ánh xạ $p$ là toàn ánh. Với mọi điểm $x$ của X, nó có một tiết diện liên tục $s$ sao cho $s(p(x)) =x$.

Tập $p(X)$ là một tập con mở, đóng (TG, I, p. 72, mệnh đề 1), khác rỗng của I. Vì I liên thông, ta có $p(X) = I$; ánh xạ $p$ do đó là toàn ánh.

Đối với mỗi cặp $(a, b)\in I\times I$ sao cho $a\leqslant b$, ký hiệu $F_{a,b}$ là tập hợp các cặp $(y, z)\in \overset{-1}{p}(a)\times \overset{-1}{p}(b)$ sao cho $y$ và $z$ thuộc cùng một thành phần liên thông của $\overset{-1}{p}([a, b])$.

#### Bổ đề 10 {#ta-iii-s2-lem-10 .statement tag=01Y8}

Cho $a,b$ là các điểm của I sao cho $a\leqslant b$.

a) Tập hợp $F_{a,b}$ là đóng trong $\overset{-1}{p}(a)\times \overset{-1}{p}(b)$.

b) Ta có pr$_1(F_{a,b}) =\overset{-1}{p}(a)$ và pr$_2(F_{a,b}) =\overset{-1}{p}(b)$.

c) Cho $c\in I$ sao cho $b\leqslant c$. Nếu $(y, z)$ thuộc $F_{a,b}$ và $(z, t)$ thuộc $F_{b,c}$, thì $(y, t)$ thuộc $F_{a,c}$.

Tập hợp $\overset{-1}{p}([a, b])$ là compact (TG, I, p. 77, Prop. 7). Do đó, để một cặp $(y, z)\in \overset{-1}{p}(a)\times \overset{-1}{p}(b)$ thuộc $F_{a,b}$, điều kiện cần và đủ là mọi tập con mở và đóng của $\overset{-1}{p}([a, b])$ chứa $y$ đều phải chứa $z$ (TG, II, p. 32, Prop. 6).

Đặt $Y =\overset{-1}{p}([a, b])$. Với mọi tập con mở và đóng U của Y, tập hợp $((U\times U)\cup ((Y-U)\times (Y-U)))\cap (\overset{-1}{p}(a)\times \overset{-1}{p}(b))$ là đóng trong $\overset{-1}{p}(a)\times \overset{-1}{p}(b)$. Giao của các tập hợp này bằng $F_{a,b}$, do đó a).

Cho $y\in \overset{-1}{p}(a)$. Gọi $\mathscr{U}$ là tập hợp các lân cận mở và đóng của $y$ trong Y. Ánh xạ từ Y vào $[a, b]$ suy ra từ $p$ bằng cách chuyển qua các không gian con là mở và thực sự (I, p. 17, Prop. 8), do đó cũng đóng. Suy ra rằng, với mọi tập hợp U thuộc $\mathscr{U},p(U)$ là một tập con mở và đóng khác rỗng của $[a, b]$; vì khoảng $[a, b]$ là liên thông, ta có $p(U) = [a, b]$ và đặc biệt $U\cap \overset{-1}{p}(b)=\not\emptyset$. Do đó, $(U\cap \overset{-1}{p}(b))_{U\in\mathscr{U}}$ là một họ lọc giảm gồm các tập con đóng khác rỗng của không gian compact $\overset{-1}{p}(b)$. Giao của họ này không rỗng (TG, I, p. 59); cho $z$ là một phần tử của nó. Ta có $(y, z)\in F_{a,b}$. Ta đã chứng minh quan hệ pr$_1(F_{a,b}) =\overset{-1}{p}(a)$. Quan hệ pr$_2(F_{a,b}) =\overset{-1}{p}(b)$ được suy ra từ đó bằng cách thay thế $p$, I$,a,b$ bởi $-p$, $-I,-b,-a$.

Dưới các giả thiết của c), cặp $(y, t)$ thuộc $\overset{-1}{p}(a)\times \overset{-1}{p}(c)$, tập hợp $\{y, z\}$ được chứa trong một phần liên thông C của $\overset{-1}{p}([a, b])$ và tập hợp $\{z, t\}$ được chứa trong một phần liên thông $C'$ của $\overset{-1}{p}([b, c])$. Khi đó, $C\cup C'$ là một phần liên thông của $\overset{-1}{p}([a, c])$ (TG, I, p. 81, mệnh đề 2) và chứa $\{y, t\}$, do đó quan hệ $(y, t)\in F_{a,c}$.

Ta trở lại chứng minh của định lý 3. Mỗi thớ của ánh xạ $p$ là compact (TG, I, p. 77, mệnh đề 7). Theo định lý Tychonoff (TG, I, p. 63, định lý 3), không gian tích $K =\prod_{a\in I}\overset{-1}{p}(a)$ là compact. Gọi $K'$ là tập hợp các phần tử $(y_a)_{a\in I}$ của K sao cho $y_{p(x)}$ bằng $x$ và sao cho ta có $(y_a, y_b)\in F_{a,b}$ với mọi cặp $(a, b)$ các phần tử của I sao cho $a < b$. Định lý 3 suy ra từ bổ đề sau.

#### Bổ đề 11 {#ta-iii-s2-lem-11 .statement tag=01Y9}

a) Tập hợp $K'$ không rỗng.

b) Cho $(s_a)_{a\in I}$ là một phần tử của $K'$. Ánh xạ $s:a\mapsto s_a$ từ I vào X là một tiết diện liên tục của $p$ sao cho $s(p(x)) =x$.

Với mọi tập con hữu hạn S của I chứa điểm $p(x)$, ký hiệu $K_S$ là tập hợp các phần tử $(y_a)_{a\in I}$ của K thỏa mãn quan hệ $y_{p(x)}=x$ và các quan hệ $(y_a, y_b)\in F_{a,b}$ với mọi cặp $(a, b)$ các phần tử của S sao cho $a < b$. Các tập hợp $K_S$ là đóng trong K (bổ đề 10, a)) và tạo thành một họ lọc giảm của các tập con của K, mà giao của chúng là $K'$. Để chứng minh rằng $K'$ không rỗng, chỉ cần chứng minh rằng, với mọi tập con hữu hạn S của I chứa điểm $p(x)$, tập hợp $K_S$ không rỗng (TG, I, p. 59).

Cho S là một tập con như vậy; sắp thứ tự các phần tử của nó thành một dãy tăng ngặt $(a_1, . . . , a_n)$ và ký hiệu i là số nguyên sao cho $p(x) =a_i$. Đặt $y_{a_i}=x$. Bổ đề 10, b), cho phép ta xây dựng bằng quy nạp các phần tử $y_{a_j}\in \overset{-1}{p}(a_j)$, với $i < j\leqslant n$, và bằng quy nạp giảm các phần tử $y_{a_j}\in \overset{-1}{p}(a_j)$ với $1\leqslant j < i$, theo cách sao cho có $(y_{a_j}, y_{a_{j+1}})\in F_{a_j,a_{j+1}}$ với mọi số nguyên $j$ sao cho $1\leqslant j < n$. Theo bổ đề 10, c), ta có $(y_a, y_b)\in F_{a,b}$ với mọi cặp $(a, b)$ các phần tử của S sao cho $a < b$. Vì ánh xạ $p$ là toàn ánh, ta có thể chọn với mọi $a\in I-S$ một phần tử $y_a\in \overset{-1}{p}(a)$. Họ $(y_a)_{a\in I}$ được xây dựng như vậy thuộc về $K_S$, do đó $K_S$ không rỗng.

Ta chứng minh b). Theo định nghĩa của $K',s$ là một tiết diện của $p$ sao cho $s(p(x)) =x$. Cho $a\in I$; ta chứng minh tính liên tục của $s$ tại điểm $a$. Cho U là một lân cận mở của $s_a$ trong X. Vì $\overset{-1}{p}(a)$ là một không gian compact (TG, I, p. 77, mệnh đề. 7) và rời rạc hoàn toàn, $s_a$ có trong $\overset{-1}{p}(a)$ một lân cận mở và đóng C, được chứa trong U (TG, II, p. 32, hệ quả). Các tập hợp C và $\overset{-1}{p}(a)-C$ là đóng trong $\overset{-1}{p}(a)$, do đó compact, và chúng rời nhau. Vì X là tách được, chúng có trong X các lân cận mở và rời nhau V và $V'$ (TG, I, p. 61, mệnh đề. 3). Tập hợp $(V\cap U)\cup V'$ là một lân cận mở của thớ $\overset{-1}{p}(a)$ trong X; vì ánh xạ $p$ là đóng (TG, I, p. 72, mệnh đề. 1), $(V\cap U)\cup V'$ chứa một tập hợp có dạng $\overset{-1}{p}(J)$, trong đó $J\subset I$ là một khoảng mở chứa $a($I, p. 75, bổ đề). Đặt $W = V\cap U\cap \overset{-1}{p}(J)$. Tập hợp W là mở trong $\overset{-1}{p}(J)$; nó cũng đóng trong $\overset{-1}{p}(J)$ vì ta có $\overset{-1}{p}(J)-W = V'\cap \overset{-1}{p}(J)$. Cho $b\in J$. Khoảng đóng của I có các đầu mút $a$ và $b$ được chứa trong J. Theo giả thiết, $(s_a, s_b)$ thuộc về $F_{a,b}$ nếu $a\leqslant b$ và $(s_b, s_a)$ thuộc về $F_{b,a}$ nếu $b\leqslant a$. Do đó tồn tại một tập con liên thông của $\overset{-1}{p}(J)$ chứa $\{s_a, s_b\}$. Do đó, điểm $s_b$ thuộc về mọi tập con mở và đóng của $\overset{-1}{p}(J)$ chứa $s_a$, suy ra đặc biệt thuộc về W; a fortiori, $s_b$ thuộc về U. Do đó ta có $s(J)\subset U$, điều này chứng minh tính liên tục của $s$ tại điểm $a$.

#### Hệ quả {#ta-iii-s2-n10-cor-1 .statement tag=01YA}

Cho X và B là các không gian tôpô và cho $p: X\rightarrow B$ là một ánh xạ liên tục, mở, thực sự và tách được mà các thớ của nó là rời rạc hoàn toàn. Cho I là một khoảng của $\mathbf{R}$, cho $f: I\rightarrow B$ là một ánh xạ liên tục, cho $a$ là một điểm của I và cho $x$ là một điểm của X sao cho $f(a) =p(x)$. Tồn tại một ánh xạ liên tục $g: I\rightarrow X$ sao cho $p\circ g=f$ và $g(a) =x$.

Đặt $X'= I\times_BX$ và ký hiệu $p': X'\rightarrow$ I và $f': X'\rightarrow$ X là các phép chiếu chính tắc. Ánh xạ $p'$ là liên tục, mở, thực sự và tách được (I, p. 17, prop. 8 và p. 27, prop. 4). Vì không gian I là tách được, không gian $X'$ là tách được (I, p. 26, nhận xét 3). Các thớ của $p'$ là hoàn toàn rời rạc ( I, p. 10, hệ quả, a)). Theo Định lý 3, tồn tại một tiết diện liên tục $s'$ của $p'$ nhận tại $a$ giá trị $(a, x)$. Ánh xạ $g=f'\circ s'$ từ I vào X là liên tục, ta có $p\circ g=p\circ f'\circ s'=f\circ p'\circ s'=f$ và $g(a) =x$, do đó có hệ quả.

#### Định lý 4 {#ta-iii-s2-thm-4 .statement tag=01YB}

Cho X là một không gian tôpô, cho G là một nhóm rời rạc tác động thực sự trên X và cho $p: X\rightarrow X/G$ là ánh xạ chính tắc. Cho I là một khoảng của $\mathbf{R}$, cho $f: I\rightarrow X/G$ là một ánh xạ liên tục, cho $a$ là một điểm của I và cho $x$ là một điểm của X sao cho $f(a) =p(x)$. Tồn tại một ánh xạ liên tục $\varphi : I\rightarrow X$ sao cho $p\circ \varphi =f$ và $\varphi (a) =x$.

Trước hết ta xét trường hợp I là một khoảng đóng bị chặn của $\mathbf{R}$.

Theo TG, III, p. 29, mệnh đề 3, không gian X là tách được.

Cho $y$ là một điểm của $X/G$ và cho $x\in X$ sao cho $y=p(x)$. Nhóm ổn định $K_x$ của $x$ là một nhóm con hữu hạn của G; hơn nữa, tồn tại các lân cận $U_x$ của $x$ trong X và $V_y$ của $y$ trong $X/G$ sao cho $U_x$ ổn định bởi $K_x,gU_x\cap U_x=\emptyset$ nếu $g\notin K_x$ và $p$ cảm sinh một đồng phôi từ $U_x/K_x$ lên $V_y$ (TG, III, p. 32, mệnh đề 8). Hơn nữa, với mọi $g\in G,p$ cảm sinh một đồng phôi từ $gU_x$ lên $V_y$. Vì I là compact, tồn tại các số nguyên $m$ và $n$ sao cho $m\leqslant 0\leqslant n$ và một dãy hữu hạn $(a_i)_{m\leqslant i\leqslant n}$ các phần tử của I sao cho $a_0=a,I = [a_m, a_n]$, và sao cho, với mọi $i\in  \{m, . . . , n-1\},f([a_i, a_{i+1}])$ được chứa trong một tập mở $V_{y_i}$ của $X/G$ được xây dựng như trên.

Cho $x_0$ là phần tử duy nhất của $\overset{-1}{p}(y_0)$ sao cho $x\in U_{x_0}$. Gọi $q_0$ là ánh xạ chính tắc của $U_{x_0}$ lên $U_{x_0}/K_{x_0}$; bằng cách chuyển qua thương, ánh xạ $p$ cảm sinh một phép đồng phôi $i_0$ của $U_{x_0}/K_{x_0}$ lên $V_{y_0}$ sao cho $i_0\circ q_0=p|U_{x_0}$. Ánh xạ $q_0$ là thực sự (TG, III, p. 29, Mệnh đề 3), mở (TG, I, p. 31, ví dụ 1) và tách được, vì X tách được. Các thớ của nó là hoàn toàn rời rạc, vì chúng hữu hạn. Theo hệ quả, III, p. 286, tồn tại một ánh xạ liên tục $\varphi_0: [a_0, a_1]\rightarrow U_{x_0}$ sao cho $p\circ \varphi_0=f|[a_0, a_1]$.

Theo cùng một cách, bằng quy nạp theo số nguyên $i\in  \{0, . . . , n-1\}$, người ta xây dựng một điểm $x_i\in \overset{-1}{p}(y_i)$, một ánh xạ liên tục $\varphi_i: [a_i, a_{i+1}]\rightarrow X$ có ảnh được chứa trong $U_{x_i}$ sao cho $p\circ \varphi_i=f|[a_i, a_{i+1}]$ và sao cho $\varphi_i(a_{i+1}) =\varphi_{i+1}(a_{i+1})$ nếu $0\leqslant i < n-1$.

Tương tự, bằng quy nạp giảm theo số nguyên $i\in  \{m, . . . ,-1\}$, người ta xây dựng một điểm $x_i\in \overset{-1}{p}(y_i)$, một ánh xạ liên tục $\varphi_i: [a_i, a_{i+1}]\rightarrow X$ có ảnh được chứa trong $U_{x_i}$ sao cho $p\circ \varphi_i=$ $f|[a_i, a_{i+1}]$ và sao cho $\varphi_i(a_{i+1}) =\varphi_{i+1}(a_{i+1})$ nếu $m\leqslant i <0$.

Tồn tại một ánh xạ duy nhất $\varphi : I\rightarrow$ X trùng với $\varphi_i$ trong $[a_i, a_{i+1}]$ với $m\leqslant i < n$. Nó liên tục (TG, I, p. 19, Mệnh đề 4). Nó là một nâng liên tục của $f$ lên X sao cho $\varphi (a) =x$.

Điều này chứng minh định lý khi I compact. Trong trường hợp tổng quát, tồn tại các dãy $(a_n)_{n\in\mathbf{N}}$ và $(b_n)_{n\in\mathbf{N}}$ sao cho $(a_n)$ là dừng với giới hạn dưới của I, $(b_n)$ là dừng với giới hạn trên của I$,a=a_0=b_0$, và sao cho $(a_n)$ (tương ứng $(b_n)$) là hằng nếu I có phần tử nhỏ nhất (tương ứng lớn nhất). Từ những điều đã nêu trước đó, với mỗi số nguyên $n\in \mathbf{N}$ tồn tại một nâng liên tục $\varphi_n$ của $f|[a_n, a_{n+1}]$ lên X, một nâng liên tục $\varphi '_n$ của $f|[b_{n+1}], b_n]$ lên X sao cho $\varphi_0(a_0) =\varphi '_0(b_0) =x$ $\varphi_{n+1}(a_{n+1}) =\varphi_n(a_{n+1}),\varphi '_{n+1}(b_{n+1}) =\varphi '_n(b_{n+1})$. Tồn tại một ánh xạ duy nhất $\varphi : I\rightarrow X$ trùng với $\varphi_n$ trong $[a_n, a_{n+1}]$ và với $\varphi '_n$ trong $[b_{n+1}, b_n]$, với mọi $n\in \mathbf{N}$. Nó liên tục (loc. cit.) và nó là một nâng liên tục của $f$ lên X sao cho $phi(a) =x$. Định lý được chứng minh.

#### Ví dụ 1 {#ta-iii-s2-n10-exa-1 .statement tag=01YC}

Cho X là một không gian tôpô tách được và cho G là một nhóm hữu hạn, được trang bị tôpô rời rạc, tác động liên tục trong X. Phép toán này khi đó là thực sự (TG, III, p. 28, Mệnh đề 2). Mệnh đề của định lý 4 suy ra trực tiếp từ hệ quả của định lý 3.

#### Ví dụ 2 {#ta-iii-s2-n10-exa-2 .statement tag=01YD}

Cho $n$ là một số nguyên $\geqslant 0$. Gọi $P_n$ là tập hợp các đa thức monic $P\in$ $\mathbf{C}[X]$ bậc $n$, được trang bị tôpô mà theo đó ánh xạ $(c_0, . . . , c_{n-1})\mapsto X^n+c_{n-1}X^{n-1}+\cdots +c_0$ là một phép đồng phôi từ $\mathbf{C}^n$ lên $P_n$. Ánh xạ $p$ từ $\mathbf{C}^n$ vào $P_n$ được xác định bởi $p(z_1, . . . , z_n) = (X-z_1). . .(X-z_n)$ là liên tục. Nhóm đối xứng $\mathfrak{S}_n$ tác động lên $\mathbf{C}^n$ bằng phép hoán vị các thừa số và $p$ xác định, bằng cách chuyển qua thương, một phép đồng phôi từ $\mathbf{C}^n/\mathfrak{S}_n$ lên $P_n$ (TG, VIII, p. 22, prop. 1, I, p. 23, cor. 1 and TG, VIII, p. 20). Do đó ta suy ra mệnh đề sau:

Cho I là một khoảng của $\mathbf{R}$, cho $(c_0, . . . , c_{n-1})$ là một dãy các ánh xạ liên tục từ I vào $\mathbf{C}$, cho $a$ là một điểm của I và cho $(z_1, . . . , z_n)$ là một dãy các số phức sao cho ta có $(X-z_1). . .(X-z_n) = X^n+$ $c_{n-1}(a)X^{n-1}+\cdots +c_0(a)$. Tồn tại một dãy $(\lambda_1, . . . , \lambda_n)$ các ánh xạ liên tục từ I vào $\mathbf{C}$ sao cho ta có $\lambda_i(a) =z_i$ for $1\leqslant i\leqslant n$ và $(X-\lambda_1(t)). . .(X-\lambda_n(t)) = X^n+c_{n-1}(t)X^{n-1}+\cdots +c_0(t)$ với mọi $t\in I$.

## BÀI TẬP {#ta-iii-s2-exercises}

Xem các [bài tập cho § 2](exercises/s2/).
