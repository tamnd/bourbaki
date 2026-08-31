---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 1
section_title: Homotopies, homéotopies
lang: vi
source: ta-i-iv-fr
book_pages: TA III.229-TA III.256, TA III.321-TA III.330
pdf_pages: 0245-0272, 0337-0346
extraction: native
subsections:
    - "no": 1
      title: Applications continues homotopes
      page: 229
      pdf_page: 245
    - "no": 2
      title: Homotopies pointées
      page: 231
      pdf_page: 247
    - "no": 3
      title: Espaces homéotopes
      page: 232
      pdf_page: 248
    - "no": 4
      title: Homéotopies relatives
      page: 234
      pdf_page: 250
    - "no": 5
      title: Rétractions et contractions
      page: 235
      pdf_page: 251
    - "no": 6
      title: Cylindre d’une application
      page: 237
      pdf_page: 253
    - "no": 7
      title: La propriété d’extension des homotopies
      page: 240
      pdf_page: 256
    - "no": 8
      title: Attachement d’un espace topologique
      page: 247
      pdf_page: 263
    - "no": 9
      title: Espace obtenu par contraction d’un sous-espace
      page: 251
      pdf_page: 267
    - "no": 10
      title: Cône d’une application
      page: 253
      pdf_page: 269
statements: 55
exercises: 32
content_sha256: 172e8bcc537cb4480b91553dfa5d66ddc48cbbef70188596950252462aa4bc45
translated_from: content/en-mt/ta/III/01_s1_homotopies_homeotopies.md
source_lang: en-mt
translation_method: machine
source_content_sha256: de0ef62b9f9d66991b9ad4548ceb259cb8f282c2877ebedb8e720ef4cfcd07b6
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-3a7ebede
glossary_version: 34
glossary_terms_sha256: 5626f9a44d44cc6efc75d26f2eb36b21cf200b583c6a769e69db763781381c03
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐỒNG LUÂN, ĐỒNG PHÔI

Trong đoạn này và các đoạn tiếp theo, $\mathbf{I}$ ký hiệu khoảng $[0,1]$ của $\mathbf{R}$.

### 1. Các ánh xạ liên tục đồng luân

#### Định nghĩa 1 {#ta-iii-s1-def-1 .statement tag=01V4}

Cho X và Y là các không gian tôpô và $f$ và $g$ là các ánh xạ liên tục từ X vào Y. Một phép đồng luân liên hệ $f$ với $g$ theo định nghĩa là một ánh xạ liên tục $\sigma : X\times \mathbf{I}\rightarrow Y$ sao cho, với mọi $x\in X$, ta có $\sigma (x,0) =f(x)$ và $\sigma (x,1) =g(x)$. Người ta nói rằng $f$ đồng luân với $g$ nếu tồn tại một phép đồng luân liên hệ $f$ với $g$.

Người ta nói rằng $f$ là điểm đầu và $g$ là số hạng của phép đồng luân $\sigma ($xem dưới đây, III, p. 257, nhận xét 2).

Cho A là một tập con của X. Người ta nói rằng phép đồng luân $\sigma$ cố định trên A nếu, với mọi $a\in A$, ánh xạ $t\mapsto \sigma (a, t)$ từ $\mathbf{I}$ vào Y là hằng. Trong trường hợp này, điểm đầu và số hạng của $\sigma$ trùng nhau tại mọi điểm của A.

Cho X và Y là các không gian tôpô. Người ta nói rằng các phép đồng luân $\sigma : X\times \mathbf{I}\rightarrow Y$ và $\tau : X\times \mathbf{I}\rightarrow Y$ được ghép nối nếu số hạng của $\sigma$ là

N. Bourbaki và Springer-Verlag Berlin Heidelberg 2   016

N.©  Bourbaki, Algebraic Topology, DOI 10.1007/978-3-662-49361-8_3  229 điểm đầu của $\tau$, nói cách khác nếu ta có $\sigma (x,1) =\tau (x,0)$ với mọi $x\in X$. Trong trường hợp này, ánh xạ $\sigma *\tau$ từ $X\times \mathbf{I}$ vào Y được xác định bởi

$\sigma (x,2t)$ với $0\leqslant t\leqslant 1/2$

$$
(\sigma *\tau )(x, t) = \tag{1}
$$

$\tau (x,2t-1)$ với $1/2\leqslant t\leqslant 1$

là liên tục (TG, I, p. 19, mệnh đề 4) và là một phép đồng luân liên hệ điểm đầu của $\sigma$ với số hạng của $\tau$. Nó được gọi là phép đồng luân ghép của các phép đồng luân $\sigma$ và $\tau$.

Nếu $\sigma : X\times \mathbf{I}\rightarrow Y$ là một phép đồng luân, ánh xạ $\overline{\sigma}: X\times \mathbf{I}\rightarrow Y$ được xác định bởi điểm đầu của$(\sigma x, t$. Ta có$)\mapsto \frac{\sigma}{\sigma}(=x,1\sigma -$. Nếu$t)\sigma$là một phép đồng luân liên hệ số hạng củaand $\tau$ là các phép đồng luân ghép$\sigma$ với

của $X\times \mathbf{I}$ vào Y, các phép đồng luân $\overline{\tau}$ và $\overline{\sigma}$ được ghép nối và ta có $\overline{\sigma*\tau}=\overline{\tau}*\overline{\sigma}$.

#### Mệnh đề 1 {#ta-iii-s1-prop-1 .statement tag=01V5}

Cho X và Y là các không gian tôpô. Quan hệ “ $f$ đồng luân với $g$ ” là một quan hệ tương đương trong tập hợp $\mathscr{C}(X; Y)$ các ánh xạ liên tục từ X vào Y.

Cho $f$ là một phần tử của $\mathscr{C}(X; Y)$. Ánh xạ $f\circ$ pr$_1: X\times \mathbf{I}\rightarrow Y$ là một phép đồng luân liên hệ $f$ với $f$; do đó quan hệ này là phản xạ.

Cho $f$ và $g$ là các phần tử của $\mathscr{C}(X; Y)$ và $\sigma : X\times \mathbf{I}\rightarrow Y$ là một đồng luân nối $f$ với $g$. Khi đó ánh xạ $\overline{\sigma}: X\times \mathbf{I}\rightarrow Y$ là một đồng luân nối $g$ với $f$; do đó quan hệ đang xét là đối xứng.

Cuối cùng, hãy chứng minh rằng nó là bắc cầu. Nếu $f,g$ và $h$ là các phần tử của $\mathscr{C}(X; Y),\sigma$ là một đồng luân nối $f$ với $g$ và $\tau$ là một đồng luân nối $g$ với $h$, thì $\sigma$ và $\tau$ được ghép nối với nhau và $\sigma *\tau$ là một đồng luân nối $f$ với $h$.

Cho X và Y là các không gian tôpô. Quan hệ tương đương “$f$ đồng luân với $g$” trong $\mathscr{C}(X; Y)$ (Mệnh đề 1) được gọi là quan hệ đồng luân. Tập thương của $\mathscr{C}(X; Y)$ theo quan hệ này được ký hiệu là [X; Y]. Các phần tử của nó được gọi là các lớp đồng luân của các ánh xạ liên tục từ X vào Y. Lớp đồng luân của một ánh xạ liên tục $f: X\rightarrow Y$ thường được ký hiệu bởi $[f]$.

#### Mệnh đề 2 {#ta-iii-s1-prop-2 .statement tag=01V6}

Cho X, Y và Z là các không gian tôpô, $f$ và $f'$ là các ánh xạ liên tục từ X vào Y$,g$ và $g'$ là các ánh xạ liên tục từ Y vào Z. Nếu $f$ đồng luân với $f'$ và nếu $g$ đồng luân với $g'$, thì $g\circ f$ đồng luân với $g'\circ f'$.

Cho $\sigma$ là một đồng luân nối $f$ với $f'$ và $\tau$ là một đồng luân nối $g$ với $g'$. Khi đó ánh xạ $\theta : X\times \mathbf{I}\rightarrow Z$ được xác định bởi $\theta (x, t) =\tau (\sigma (x, t), t)$ là một đồng luân nối $g\circ f$ với $g'\circ f'$.

Cho X, Y và Z là các không gian tôpô. Với các lớp đồng luân $\varphi \in [X; Y]$ và $\psi \in [Y; Z]$, các ánh xạ $g\circ f: X\rightarrow Z$, trong đó $f\in \varphi ,g\in \psi$, đều thuộc cùng một lớp đồng luân duy nhất (Mệnh đề 2), lớp này được ký hiệu là $\psi \circ \varphi$ và được gọi là lớp đồng luân hợp thành của các lớp $\psi$ và $\varphi$. Ánh xạ $[X; Y]\times [Y; Z]\rightarrow [X; Z]$ gán $\psi \circ \varphi$ cho $(\varphi , \psi )$ được gọi là ánh xạ hợp thành.

Cho $\varphi \in [X; Y]$ ; ta có $\varphi =\varphi \circ$ [Id$_X] =$ [Id$_Y]\circ \varphi$.

Cho X, Y, Z và T là các không gian tôpô, $\varphi \in [X; Y]$, $\psi \in [Y; Z]$ và $\chi \in [Z; T]$. Lớp đồng luân $\chi \circ (\psi \circ \varphi )$ bằng $(\chi \circ \psi )\circ \varphi$; nó được ký hiệu là $\chi \circ \psi \circ \varphi$.

#### Mệnh đề 3 {#ta-iii-s1-prop-3 .statement tag=01V7}

Cho X là một không gian tôpô và $(Y_j)_{j\in J}$ là một họ các không gian tôpô. Ánh xạ từ $[X;\prod_{j\in J}Y_j]$ vào tập hợp tích $\prod_{j\in J}[X; Y_j]$ xác định bởi $\varphi \mapsto$ ([pr$_j]\circ \varphi$ )$_{j\in J}$ là song ánh.

Tính toàn ánh suy ra ngay lập tức từ I, p. 25, mệnh đề 1. Ta hãy chứng minh tính đơn ánh. Cho $f$ và $g$ là các ánh xạ liên tục từ X vào $\prod_{j\in J}Y_j$. Với mỗi $j\in J$, đặt $f_j=$ pr$_j\circ f$ và $g_j=$ pr$_j\circ g$; giả sử $f_j$ đồng luân với $g_j$ và gọi $\sigma_j$ là một đồng luân nối $f_j$ với $g_j$. Ánh xạ $\sigma = (\sigma_j)$ từ $X\times \mathbf{I}$ vào $\prod_{j\in J}Y_j$ là liên tục (loc. cit.) ; nó là một đồng luân nối $f$ với $g$, do đó mệnh đề.

#### Hệ quả {#ta-iii-s1-n1-cor-1 .statement tag=01V8}

Cho $(X_j)_{j\in J}$ và $(Y_j)_{j\in J}$ là các họ không gian tôpô có cùng tập chỉ số. Với mỗi $j\in J$, cho $f_j$ và $g_j$ là các ánh xạ liên tục từ $X_j$ vào $Y_j$. Nếu, với mỗi $j\in J$, các ánh xạ $f_j$ và $g_j$ đồng luân, thì điều tương tự cũng đúng đối với các ánh xạ tích $f: (x_j)\mapsto (f_j(x_j))$ và $g: (x_j)\mapsto (g_j(x_j))$ từ $\prod_{j\in J}X_j$ vào $\prod_{j\in J}Y_j$.

Giả sử ta có $[f_j] = [g_j]$ với mỗi $j\in J$. Ta có [pr$_j]\circ [f] =$ $[f_j\circ$ pr$_j]$ và [pr$_j]\circ [g] = [g_j\circ$ pr$_j]$, do đó [pr$_j]\circ [f] =$ [pr$_j]\circ [g]$ theo mệnh đề 2, do đó $[f] = [g]$ theo mệnh đề 3.

### 2. Các đồng luân có điểm đánh dấu

Cho X và Y là các không gian tôpô và $x$ là một điểm của X. Một đồng luân $\sigma : X\times \mathbf{I}\rightarrow Y$ được gọi là có điểm tại $x$ nếu nó cố định trên $\{x\}$, nghĩa là nếu ánh xạ $t\mapsto \sigma (x, t)$ từ $\mathbf{I}$ vào Y là hằng. Phép ghép của hai đồng luân có điểm tại $x$ là một đồng luân có điểm tại $x$. Gốc và ngọn của một đồng luân có điểm tại $x$ nhận cùng giá trị $y$ tại $x$; do đó chúng là các ánh xạ liên tục có điểm từ $(X, x)$ vào $(Y, y)$.

Cho $(X, x)$ và $(Y, y)$ là các không gian tôpô có điểm (I, p. 120, định nghĩa 1). Quan hệ « $f$ liên quan với $g$ bởi một đồng luân có điểm tại $x$ » là một quan hệ tương đương trong tập hợp $\mathscr{C}((X, x); (Y, y))$, gọi là quan hệ đồng luân có điểm. Tập thương của $\mathscr{C}((X, x); (Y, y))$ theo quan hệ tương đương này được ký hiệu là $[(X, x); (Y, y)]$. Các phần tử của nó được gọi là các lớp đồng luân có điểm của các ánh xạ liên tục có điểm từ $(X, x)$ vào $(Y, y)$.

Tập hợp $\mathscr{C}((X, x); (Y, y))$ là một tập con của $\mathscr{C}(X; Y)$. Cần lưu ý rằng đồng luân có điểm là một quan hệ tương đương mịn hơn quan hệ cảm sinh bởi đồng luân trong $\mathscr{C}(X; Y)$. Nói chung, đó là một quan hệ thực sự mịn hơn (xem III, p. 321, exerc. 1 và III, p. 234, ví dụ 3).

Cho thêm $(Z, z)$ là một không gian tôpô có điểm. Cho $f$ và $f'$ là các ánh xạ liên tục có điểm từ $(X, x)$ vào $(Y, y),g$ và $g'$ là các ánh xạ liên tục có điểm từ $(Y, y)$ vào $(Z, z)$. Nếu $f$ và $f'$ liên quan với nhau bởi một đồng luân $\sigma$ có điểm tại $x$, và nếu $g$ và $g'$ liên quan với nhau bởi một đồng luân $\tau$ có điểm tại $y$, thì $g\circ f$ và $g'\circ f'$ liên quan với nhau bởi đồng luân $\theta : X\times \mathbf{I}\rightarrow Z$, $(u, t)\mapsto \tau (\sigma (u, t), t)$, có điểm tại $x$. Như trên, điều này cho phép định nghĩa ánh xạ hợp thành của $[(X, x); (Y, y)]\times [(Y, y); (Z, z)]$ vào $[(X, x); (Z, z)]$. Chúng tôi để người đọc phát biểu và chứng minh cho các ánh xạ và đồng luân có điểm các mệnh đề tương tự như mệnh đề 3 và hệ quả của nó.

### 3. Các không gian đồng luân

#### Định nghĩa 2 {#ta-iii-s1-def-2 .statement tag=01V9}

Cho X và Y là các không gian tôpô. Một lớp đồng luân $\varphi \in$ [X; Y] được gọi là khả nghịch nếu tồn tại một lớp đồng luân $\psi \in [Y; X]$ sao cho $\psi \circ \varphi =$ [Id$_X]$ và $\varphi \circ \psi =$ [Id$_Y]$. Một ánh xạ liên tục được gọi là một đẳng cấu đồng luân nếu lớp đồng luân của nó khả nghịch.

Cho $\varphi \in$ [X; Y] là một lớp đồng luân khả nghịch. Có duy nhất một lớp đồng luân $\psi \in [Y; X]$ có các tính chất của định nghĩa 2. Thật vậy, giả sử $\psi ,\psi '$ là các lớp có những tính chất này; ta có

$\psi =\psi \circ$ [Id$_Y] =\psi \circ \varphi \circ \psi '=$ [Id$_X]\circ \psi '=\psi '$.

Lớp duy nhất này được gọi là nghịch đảo của lớp đồng luân $\varphi$ và được ký hiệu là $\varphi^{-1}$.

Cho Z là một không gian tôpô. Ta có $\chi \circ \varphi \circ \varphi^{-1}=\chi$ với mọi $\chi \in$ [Y; Z] và $\theta \circ \varphi^{-1}\circ \varphi =\theta$ với mọi $\theta \in [X; Z]$. Suy ra rằng các ánh xạ $\chi \mapsto \chi \circ \varphi$ từ [Y; Z] vào [X; Z] và $\theta \mapsto \theta \circ \varphi^{-1}$ từ [X; Z] vào [Y; Z] là các song ánh ngược nhau. Tương tự, ánh xạ $\chi \mapsto \varphi \circ \chi$ từ [Z; X] vào [Z; Y] là song ánh và song ánh ngược của nó là ánh xạ $\theta \mapsto \varphi^{-1}\circ \theta$ từ [Z; Y] vào [Z; X].

Cho X, Y, Z là các không gian tôpô, $\varphi \in [X; Y]$ và $\psi \in [Y; Z]$ là các lớp đồng luân khả nghịch. Khi đó lớp $\psi \circ \varphi$ là khả nghịch, với nghịch đảo $\varphi^{-1}\circ \psi^{-1}$. Thật vậy, ta có

$$
(\psi \circ \varphi )\circ (\varphi^{-1}\circ \psi^{-1}) =\psi \circ (\varphi \circ \varphi^{-1})\circ \psi^{-1}
$$

$=\psi \circ$ [Id$_Y]\circ \psi^{-1}$

$=\psi \circ \psi^{-1}=$ [Id$_Z]$

và, tương tự, $(\varphi^{-1}\circ \psi^{-1})\circ (\psi \circ \varphi ) =$ [Id$_X]$.

Cho X, Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một tương đương đồng luân. Mọi ánh xạ liên tục $g: Y\rightarrow X$ mà lớp của nó là nghịch đảo của lớp của $f$ được gọi là một ánh xạ đối ứng (hoặc nghịch đảo) của $f$ đến đồng luân. Một ánh xạ như vậy $g$ là một tương đương đồng luân.

Một đồng phôi $f$ là một tương đương đồng luân, và $[f]^{-1}= [f^{-1}]$. Ánh xạ hợp thành của hai tương đương đồng luân là một tương đương đồng luân. Quan hệ "X và Y là các không gian tôpô và tồn tại một tương đương đồng luân từ X vào Y" là một quan hệ tương đương.

#### Định nghĩa 3 {#ta-iii-s1-def-3 .statement tag=01VA}

Người ta nói rằng các không gian tôpô X và Y là tương đương đồng luân nếu tồn tại một tương đương đồng luân từ X vào Y.

#### Ví dụ 1 {#ta-iii-s1-n3-exa-1 .statement tag=01VB}

Không gian tôpô rỗng chỉ tương đương đồng luân với chính nó.

#### Ví dụ 2 {#ta-iii-s1-n3-exa-2 .statement tag=01VC}

Cho X là một không gian tôpô khác rỗng. Để X tương đương đồng luân với một không gian thu gọn thành một điểm, điều kiện cần và đủ là tồn tại một ánh xạ hằng $p: X\rightarrow$ X đồng luân với ánh xạ đồng nhất của X. (Khi đó điều này đúng với mọi ánh xạ hằng $q: X\rightarrow X$, vì $[p] = [p]\circ [q] =$ [Id$_X]\circ [q] = [q]$.) Thật vậy, cho P là một không gian thu gọn thành một điểm, $f: P\rightarrow X$ một ánh xạ và $g: X\rightarrow P$ là ánh xạ duy nhất từ X vào P. Ta có $g\circ f=$ Id$_P$; để $f$ là một tương đương đồng luân, điều kiện cần và đủ là $f\circ g$ đồng luân với Id$_X$. Bây giờ, $f\circ g$ là hằng, có ảnh là $f(P)$.

#### Ví dụ 3 {#ta-iii-s1-n3-exa-3 .statement tag=01VD}

Người ta nói rằng một không gian tôpô có điểm cơ sở $(X, x)$ là co rút được, hoặc rằng không gian tôpô X là co rút được tại $x$, nếu tồn tại một đồng luân có điểm cơ sở tại $x$ nối Id$_X$ với ánh xạ hằng của X vào X có ảnh $\{x\}$. Một không gian như vậy tương đương đồng luân với một điểm. Tuy nhiên, tồn tại những không gian tương đương đồng luân với một điểm nhưng không co rút được tại bất kỳ điểm nào của chúng, và những không gian co rút được tại một điểm nhưng không tại mọi điểm (III, p. 321, exerc. 1).

#### Ví dụ 4 {#ta-iii-s1-n3-exa-4 .statement tag=01VE}

Cho E là không gian số học $n$ chiều (hoặc, nói chung hơn, một không gian vectơ tôpô trên $\mathbf{R}$) và cho X là một tập con của E. Người ta nói rằng tập hợp X là có dạng sao tại một điểm $x$ của X nếu, với mọi $y\in X$ và mọi $t\in \mathbf{I}$, điểm $tx+ (1-t)y$ thuộc X. Một tập con lồi (I, p. 122) của E là có dạng sao tại mỗi điểm của nó.

Một không gian con tôpô X của E là hình sao tại một trong các điểm của nó $x$ thì co được tại điểm này. Thật vậy, ánh xạ $\sigma : X\times \mathbf{I}\rightarrow X$ được định nghĩa bởi $\sigma (y, t) =tx+ (1-t)y$ là một phép đồng luân có điểm gốc tại $x$ nối Id$_X$ với ánh xạ hằng có ảnh $\{x\}$.

Đặc biệt, mọi khoảng của $\mathbf{R}$, mọi tập lồi của một không gian số hoặc, nói chung hơn, của một không gian vectơ tôpô trên $\mathbf{R}$ đều co được tại mỗi điểm của nó.

#### Ví dụ 5 {#ta-iii-s1-n3-exa-5 .statement tag=01VF}

Ta sẽ chứng minh sau (TA, V) rằng các mặt cầu Euclid $\mathbf{S}_n,n\geqslant 1$, không phải là các không gian đồng luân với một điểm. Mặt cầu đơn vị của một không gian Hilbert kiểu đếm được và chiều vô hạn là co được tại mỗi điểm của nó (EVT, V, p. 71, exerc. 13).

### 4. Các phép đồng luân tương đối

Cho X, Y là các không gian tôpô, cho A là một không gian con của X và cho B là một không gian con của Y.

Cho $f: X\rightarrow Y$ là một ánh xạ liên tục sao cho $f(A)\subset B$. Ta nói rằng $f$ là một phép đồng luân của cặp $(X,A)$ lên cặp $(Y,B)$ nếu tồn tại một ánh xạ liên tục $g: Y\rightarrow X$ sao cho $g(B)\subset A$, một phép đồng luân $\sigma : X\times \mathbf{I}\rightarrow X$, cố định trên A, nối Id$_X$ với $g\circ f$, và một phép đồng luân $\tau : Y\times \mathbf{I}\rightarrow Y$, cố định trên B, nối Id$_Y$ với $f\circ g$.

Giả sử các điều kiện này được thỏa mãn. Khi đó:

a) Ánh xạ $f$ là một phép đồng luân của X vào Y, ánh xạ $g$ là một phép đồng luân của Y vào X, và các phép đồng luân này là nghịch đảo của nhau sai khác một phép đồng luân.

b) Khi đó ánh xạ $g$ là một phép đồng luân của cặp $(Y,B)$ lên cặp $(X,A)$, được gọi là nghịch đảo của $f$ sai khác một phép đồng luân.

c) Các ánh xạ $f$ và $g$ định nghĩa, bằng cách chuyển qua các không gian con, các đồng phôi của A lên B là nghịch đảo của nhau.

Ta nói rằng các cặp $(X,A)$ và $(Y,B)$ là đồng luân nếu tồn tại một phép đồng luân của cặp $(X,A)$ lên cặp $(Y,B)$. Quan hệ “X, Y là các không gian tôpô, A là một không gian con của X, B là một không gian con của Y và các cặp $(X,A)$ và $(Y,B)$ là đồng luân” là một quan hệ tương đương.

### 5. Các phép rút và các phép co

#### Định nghĩa 4 {#ta-iii-s1-def-4 .statement tag=01VG}

Cho X là một không gian tôpô và cho A là một tập con của X.

Một phép rút của X lên A được gọi là một ánh xạ liên tục từ X vào A là một phép rút của đơn ánh chính tắc của A vào X. Nếu tồn tại một phép rút của X lên A, ta nói rằng X có thể được rút về A, hoặc cũng nói rằng A là một phần rút của X.

Cho X là một không gian tôpô và cho A là một không gian con của X.

Giả sử tồn tại một phép rút $r$ của X lên A. Không gian con A được đồng nhất với tập hợp các điểm $x\in X$ sao cho $x=r(x)$. Nếu X là một không gian phân ly, thì A đóng trong X.

Theo bổ đề sau đây, để một không gian con A là một phần rút của X, điều kiện cần và đủ là mọi ánh xạ liên tục từ A vào một không gian tôpô Y đều mở rộng được thành một ánh xạ liên tục từ X vào Y.

#### Bổ đề 1 {#ta-iii-s1-lem-1 .statement tag=01VH}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Các điều kiện sau là tương đương:

(i) Với mọi không gian tôpô Z và mọi ánh xạ liên tục $g: X\rightarrow Z$, tồn tại một ánh xạ liên tục $g': Y\rightarrow Z$ sao cho $g=$ $g'\circ f$;

(ii) Ánh xạ $f$ là đơn ánh và có một phép rút liên tục ;

(iii) Ánh xạ $f$ định nghĩa một đồng phôi của X lên ảnh của nó $f(X)$, là một phần rút của Y.

Giả sử rằng $f$ là đơn ánh và rằng $r: Y\rightarrow$ X là một phép rút liên tục của ánh xạ $f$. Với mọi ánh xạ liên tục $g: X\rightarrow Z$, ánh xạ $g'=g\circ r: Y\rightarrow Z$ thỏa mãn $g'\circ f=g\circ r\circ f=g$. Điều này chứng minh rằng (ii)$\Rightarrow$(i).

Giả sử điều kiện (i) được thỏa mãn. Cho $g: X\rightarrow X$ là ánh xạ đồng nhất. Theo giả thiết, tồn tại một ánh xạ liên tục $g': Y\rightarrow X$ sao cho $g'\circ f=g$. Điều này suy ra rằng ánh xạ $f$ là đơn ánh và rằng $g'$ là một phép rút liên tục của $f$.

Sự tương đương của các tính chất (ii) và (iii) là ngay lập tức.

#### Định nghĩa 5 {#ta-iii-s1-def-5 .statement tag=01VI}

Cho X là một không gian tôpô và cho A là một tập con của X. Một phép co của X lên A là một phép đồng luân $\sigma : X\times \mathbf{I}\rightarrow X$ cố định trên A có số hạng đầu là ánh xạ đồng nhất của X và có số hạng cuối là một phép co rút của X lên A. Nếu tồn tại một phép co của X lên A, người ta nói rằng X có thể co được lên A, hay cũng nói rằng A là một tập con co rút được của X.

#### Nhận xét {#ta-iii-s1-n5-rem-1 .statement tag=01VJ}

Nói cách khác, một phép co của X lên A là một phép đồng luân $\sigma : X\times \mathbf{I}\rightarrow X$ có các tính chất sau:

(i) $\sigma (x,0) =x$ với mọi $x\in X$;

(ii) $\sigma (x,1)\in A$ với mọi $x\in X$;

(iii) $\sigma (x, t) =x$ với mọi $x\in A$ và mọi $t\in \mathbf{I}$.

Để tồn tại một phép co của X lên A, điều kiện cần và đủ là đơn ánh chính tắc của A vào X là một phép đồng luân của cặp $(A,A)$ lên cặp $(X,A)$.

Cho $a$ là một điểm của X. Một phép co của X lên không gian con $\{a\}$ không gì khác hơn là một phép đồng luân điểm tại $a$ nối ánh xạ Id$_X$ với ánh xạ hằng có ảnh $\{a\}$. Do đó, X co được lên $\{a\}$ khi và chỉ khi X co được tại $a$ (Ví dụ 3 của III, p. 234).

Cho X là một không gian tôpô và cho A là một tập con của X. Cho $\sigma$ là một phép co của X lên A. Ánh xạ $r$ của X vào A được xác định bởi $r(x) =\sigma (x,1)$ là một phép co rút của X lên A và $\sigma$ là một phép đồng luân nối Id$_X$ với $r$. Các hệ thức $r\circ i=$ Id$_A$ và $i\circ r=r$ khi đó suy ra rằng các ánh xạ $i$ và $r$ là các phép đồng luân, nghịch đảo của nhau sai khác một phép đồng luân.

#### Định nghĩa 6 {#ta-iii-s1-def-6 .statement tag=01VK}

Với các ký hiệu trước đó, người ta nói rằng $\sigma$ là một phép co mạnh nếu, hơn nữa, ta có $r(\sigma (x, t)) =r(x)$ với mọi $x\in X$ và mọi $t\in \mathbf{I}$,

#### Ví dụ {#ta-iii-s1-n5-exa-1 .statement tag=01VL}

Cho X là phần bù của điểm gốc trong $\mathbf{B}_n$. Ánh xạ của $X\times \mathbf{I}$ vào X cho bởi $(x, t)\mapsto ((1-t) +t\frac{1}{\|x\|})x$ là một phép co mạnh của X lên $\mathbf{S}_{n-1}$. Phép co rút của X lên $\mathbf{S}_{n-1}$ liên kết với nó là ánh xạ cho bởi $x\mapsto x/\|x\|$.

#### Bổ đề 2 {#ta-iii-s1-lem-2 .statement tag=01VM}

Cho X là một không gian tôpô, cho U là một tập con mở của X và cho $\sigma$ là một phép co mạnh của X lên X-U. Khi đó $\sigma (U\times \mathbf{I})\subset \overline{U}$. Đặc biệt, $\sigma (U\times  \{1\})$ được chứa trong biên của U.

Cho $x\in U$. Tập hợp các số thực $t\in \mathbf{I}$ sao cho $\sigma (x, t)\in U$ là mở trong $\mathbf{I}$ và chứa 0; gọi $s$ là cận trên nhỏ nhất của nó. Ta có $\sigma (x, s)\in \overline{U}$. Nếu $s <1,\sigma (x, s)\notin U$, theo định nghĩa của $s$; điều tương tự cũng đúng nếu $s= 1$ vì $\sigma (x,1)\in X-U$. Do đó, $\sigma (x, s)\in$ Fr(U). Theo định nghĩa của một phép co mạnh, khi đó ta có $\sigma (x, s) =\sigma (\sigma (x, s),1) =\sigma (x,1)$; đặc biệt, $\sigma (x,1)\in \overline{U}$. Do đó, $\sigma (x,1)$ thuộc biên $\overline{U}\cap (X-U)$ của U.

Cho $t\in \mathbf{I}$; nếu $\sigma (x, t)\notin U$, lại có $\sigma (x, t) =\sigma (\sigma (x, t),1) =$ $\sigma (x,1)$, do đó $\sigma (x, t)\in \overline{U}$, suy ra bổ đề.

### 6. Hình trụ của một ánh xạ

Cho X và Y là các không gian tôpô và $f$ là một ánh xạ liên tục từ X vào Y. Ký hiệu U là tổng của không gian tôpô $U_1= X\times \mathbf{I}$ và không gian $U_2$ = Y và đồng nhất $U_1$ và $U_2$ với các không gian con của U qua các phép nhúng chính tắc. Gọi R là quan hệ tương đương trên U nhỏ nhất sao cho các điểm $(x,1)$ của $U_1$ và $f(x)$ của $U_2$ là tương đương, với mọi $x\in X$.

#### Định nghĩa 7 {#ta-iii-s1-def-7 .statement tag=01VN}

Hình trụ của ánh xạ $f$ được gọi là và được ký hiệu là Cyl($f$), không gian tôpô thương $U/R$.

Ký hiệu $\alpha_f: X\times \mathbf{I}\rightarrow$ Cyl($f$) và $\beta_f: Y\rightarrow$ Cyl($f$) là các hạn chế lên $U_1$ và $U_2$ của toàn cấu chính tắc từ U lên $U/R$. Ánh xạ $\alpha_f$ là một đồng luân và số hạng của nó là $\beta_f\circ f$.

Mệnh đề 4 (Tính chất phổ quát của các hình trụ)

Cho Z là một không gian tôpô, $\beta : Y\rightarrow Z$ là một ánh xạ liên tục và $\alpha : X\times \mathbf{I}\rightarrow Z$ là một đồng luân có số hạng là $\beta \circ f$. Tồn tại duy nhất một ánh xạ liên tục $\varphi$ từ Cyl($f$) vào Z sao cho $\alpha =\varphi \circ \alpha_f$ và $\beta =\varphi \circ \beta_f$.

Ánh xạ $\psi$ từ U vào Z trùng với $\alpha$ trên $X\times \mathbf{I}$ và với $\beta$ trên Y là liên tục. Ta có $\alpha (x,1) =\beta (f(x))$ với mọi $x\in X$, do đó $\psi$ xác định, bằng cách chuyển qua thương, một ánh xạ liên tục $\varphi$ từ Cyl($f$) vào Z sao cho $\alpha =\varphi \circ \alpha_f$ và $\beta =\varphi \circ \beta_f$. Vì ảnh của $\alpha_f$ và $\beta_f$ phủ Cyl($f$)$,\varphi$ là ánh xạ duy nhất từ Cyl($f$) vào Z thỏa mãn các quan hệ này.

#### Ví dụ 1 {#ta-iii-s1-n6-exa-1 .statement tag=01VO}

Cho $X',Y'$ là các không gian tôpô và $f': X'\rightarrow Y'$ là một ánh xạ liên tục. Cho $u: X\rightarrow X'$ và $v: Y\rightarrow Y'$ là các ánh xạ liên tục sao cho $f'\circ u=v\circ f$. Tồn tại duy nhất một ánh xạ liên tục $w:$ Cyl($f$)$\rightarrow$ Cyl($f'$) sao cho $w\circ \alpha_f=\alpha_{f'}\circ (u\times$ Id$_{\mathbf{I}})$ và $w\circ \beta_f=\beta_{f'}\circ v$.

Theo mệnh đề 4, áp dụng cho Z = Y và $\beta =$ Id$_Y$, tồn tại duy nhất một ánh xạ liên tục $\gamma_f:$ Cyl($f$)$\rightarrow Y$ sao cho $\gamma_f(\alpha_f(x, s)) =f(x)$ và $\gamma_f(\beta_f(y)) =y$ với $x\in X,s\in \mathbf{I}$ và $y\in Y$.

#### Mệnh đề 5 {#ta-iii-s1-prop-5 .statement tag=01VP}

Ánh xạ $\alpha_f$ cảm sinh một phép đồng phôi từ $X\times [0,1[$ lên một tập con mở của Cyl($f$). Ánh xạ $\beta_f$ xác định một phép đồng phôi từ Y lên phần bù của tập con mở này. Ánh xạ $\beta_f\circ \gamma_f$ là một phép co rút liên tục của Cyl($f$) lên $\beta_f(Y)$.

Tập hợp $X\times [0,1[$ là một tập con mở của U, bão hòa đối với quan hệ R, và quan hệ tương đương cảm sinh bởi R trên $X\times [0,1[$ là quan hệ đẳng thức. Mệnh đề đầu tiên suy ra từ điều này (TG, I, p. 23, cor. 10).

Phần bù của $\alpha_f(X\times [0,1[)$ là $\beta_f(Y)$. Vì ta có $\gamma_f\circ \beta_f=$ Id$_Y,\beta_f$ xác định một phép đồng phôi từ Y lên $\beta_f(Y)$ và $\beta_f\circ \gamma_f$ là một phép co rút liên tục của đơn ánh chính tắc của $\beta_f(Y)$ vào Cyl($f$).

Không gian con đóng $\beta_f(Y)$ của Cyl($f$) được gọi là cơ sở của hình trụ của $f$. Ánh xạ $\beta_f\circ \gamma_f$ được gọi là phép co rút chính tắc của Cyl($f$) lên cơ sở của nó.

Xét các ánh xạ $\sigma_1: U_1\times \mathbf{I}\rightarrow$ Cyl($f$) và $\sigma_2: U_2\times \mathbf{I}\rightarrow$ Cyl($f$) được xác định bởi

$\sigma_1((x, s), t) =\alpha_f(x,(1-t)s+t)$ với $(x, s)\in X\times \mathbf{I}$ và $t\in \mathbf{I}$

$\sigma_2(y, t) =\beta_f(y)$ với $y\in Y$ và $t\in \mathbf{I}$.

Chúng là các ánh xạ liên tục. Với $x\in X$ và $t\in \mathbf{I}$, ta có

$$
\sigma_1((x,1), t) =\alpha_f(x,1) =\beta_f(f(x)) =\sigma_2(f(x), t)
$$

Do đó tồn tại một ánh xạ duy nhất $\sigma_f$ của Cyl($f$)$\times \mathbf{I}$ vào Cyl($f$) sao cho $\sigma_f\circ (\alpha_f\times$ Id$_{\mathbf{I}}) =\sigma_1$ và $\sigma_f\circ (\beta_f\times$ Id$_{\mathbf{I}}) =\sigma_2$. Ánh xạ $\sigma_f$ là liên tục (I, p. 19, mệnh đề 10).

#### Mệnh đề 6 {#ta-iii-s1-prop-6 .statement tag=01VQ}

Ánh xạ $\sigma_f:$ Cyl($f$)$\times \mathbf{I}\rightarrow$ Cyl($f$) là một phép co ngặt của Cyl($f$) lên cơ sở của nó. Số hạng của nó là phép co rút chính tắc của Cyl($f$) lên cơ sở của nó.

Ánh xạ $\sigma_f$ là một đồng luân. Các hệ thức $\sigma_f(\alpha_f(x, s),0) =$ $\alpha_f(x, s)$ và $\sigma_f(\beta_f(y),0) =\beta_f(y)$ suy ra rằng điểm đầu của $\sigma_f$ là ánh xạ đồng nhất của Cyl($f$). Gọi $r_f$ là số hạng của $\sigma_f$. Các hệ thức

$$
\sigma_f(\alpha_f(x, s),1) =\alpha_f(x,1) =\beta_f(f(x)) = (\beta_f\circ \gamma_f)(\alpha_f(x, s))
$$

và $\sigma_f(\beta_f(y),1) =\beta_f(y) = (\beta_f\circ \gamma_f)(\beta_f(y))$ suy ra rằng $r_f$ là phép co rút chính tắc $\beta_f\circ \gamma_f$ của Cyl($f$) lên cơ sở của nó.

Với $(x, s)\in X\times \mathbf{I}$ và $t\in \mathbf{I}$, ta có

$$
r_f(\sigma_f(\alpha_f(x, s), t)) =r_f(\alpha_f(x, s(1-t) +t)) =\beta_f(f(x)) =r_f(\alpha_f(x, s))
$$

Với $y\in Y$ và $t\in \mathbf{I}$, ta có $r_f(\sigma_f(\beta_f(y), t)) =r_f(\beta_f(y))$. Do đó, $\sigma_f$ là một phép co ngặt của Cyl($f$) lên cơ sở của nó.

Ánh xạ $\sigma_f$ được gọi là phép co chính tắc của hình trụ của $f$ lên cơ sở của nó.

#### Nhận xét 1 {#ta-iii-s1-n6-rem-1 .statement tag=01VR}

Cho A là một tập con của $X\times \mathbf{I}$ và cho $A_1$ là tập hợp các điểm $x\in X$ sao cho $(x,1)\in A$. Ta có $\alpha^{-1}_f(\alpha_f(A)) = A\cup \overset{-1}{f}(f(A_1))\times \{1\}$ và $\beta^{-1}_f(\alpha_f(A)) =f(A_1)$. Suy ra rằng ánh xạ $\alpha_f$ là đóng (tương ứng mở) nếu $f$ là đóng (tương ứng mở).

#### Nhận xét 2 {#ta-iii-s1-n6-rem-2 .statement tag=01VS}

Giả sử rằng ánh xạ $f$ là thực sự. Cho P là một điểm của Cyl($f$). Nếu P = $\alpha_f(x, t)$, với 0 $\leqslant t <$ 1 và $x\in$ X, ta có $\alpha^{-1}_f(P) = (x, t)$. Trong trường hợp ngược lại, tồn tại $y\in Y$ sao cho $P =\beta_f(y)$ và $\alpha^{-1}_f(P) =\overset{-1}{f}(y)\times  \{1\}$. Điều này chứng minh rằng các thớ của ánh xạ $\alpha_f$ là quasi-compact. Khi đó ánh xạ $\alpha_f$ là thực sự (TG, I, p. 75, th. 1), vì nó là đóng.

Theo mệnh đề 5 và TG, I, p. 72, mệnh đề 2, ánh xạ $\beta_f$ tự nó là thực sự. Suy ra rằng, nếu $f$ là thực sự, toàn cấu chính tắc của U lên Cyl($f$) là thực sự và do đó, đặc biệt, là ngặt phổ quát (I, p. 20, hệ quả).

#### Nhận xét 3 {#ta-iii-s1-n6-rem-3 .statement tag=01VT}

Nếu các không gian X và Y tách được, điều tương tự cũng đúng đối với trụ ánh xạ của ánh xạ $f$. Thật vậy, cho $z$ và $z'$ là hai điểm phân biệt của Cyl($f$) và ta chứng minh rằng chúng có các lân cận rời nhau. Xét ba trường hợp.

– Tồn tại $(x, t)$ và $(x', t')\in X\times [0,1[$ sao cho $z=\alpha_f(x, t)$ và $z'=\alpha_f(x', t')$.

Trong trường hợp này, mệnh đề suy ra từ việc không gian $X\times [0,1[$ là tách được (TG, I, p. 54, prop. 7) và ánh xạ $\alpha_f$ cảm sinh một đồng phôi của không gian này lên một không gian con mở của Cyl($f$).

– Tồn tại $(x, t)\in X\times [0,1[$ sao cho $z=\alpha_f(x, t)$ và $y'\in Y$ sao cho $z'=\beta_f(y')$.

Khi đó, $\alpha_f(X\times [0,\frac{t+1}{2}[)$ và Cyl($f$)$-\alpha_f(X\times [0,\frac{t+1}{2}])$ là các lân cận mở rời nhau của $z$ và $z'$ trong Cyl($f$).

– Tồn tại $y$ và $y'\in Y$ sao cho $z=\beta_f(y),z'=\beta_f(y')$.

Trong trường hợp này, $y=\not y'$; vì Y là tách được, tồn tại một lân cận mở V của $y$ trong Y và một lân cận mở $V'$ của $y'$ trong Y sao cho $V\cap V'=\emptyset$. Khi đó, $(\beta_f\circ \gamma_f)^{-1}(V)$ và $(\beta_f\circ \gamma_f)^{-1}(V')$ là các tập con mở rời nhau của Cyl($f$) lần lượt chứa $y$ và $y'$.

### 7. Tính chất mở rộng đồng luân

#### Định nghĩa 8 {#ta-iii-s1-def-8 .statement tag=01VU}

Cho X là một không gian tôpô và A là một tập con của X. Ta nói rằng cặp $(X,A)$ có tính chất mở rộng đồng luân nếu, với mọi không gian tôpô Y, mọi ánh xạ liên tục $f: X\rightarrow Y$ và mọi đồng luân $\sigma : A\times \mathbf{I}\rightarrow Y$ có số hạng là ánh xạ $f|A$, tồn tại một đồng luân $\tau : X\times \mathbf{I}\rightarrow Y$ mở rộng $\sigma$ và có số hạng là ánh xạ $f$.

#### Nhận xét 1 {#ta-iii-s1-n7-rem-1 .statement tag=01VV}

Cho X là một không gian tôpô và A là một tập con của X sao cho cặp $(X,A)$ có tính chất mở rộng đồng luân. Cho Y là một không gian tôpô, cho $f: X\rightarrow Y$ là một ánh xạ liên tục và cho $\sigma : A\times \mathbf{I}\rightarrow Y$ là một đồng luân có điểm đầu là ánh xạ $f|A$. Ánh xạ $\overline{\sigma}: A\times \mathbf{I}\rightarrow Y$ được xác định bởi $(a, t)\mapsto \sigma (a,1-t)$ là một đồng luân có số hạng $f|A$; cho $\tau : X\times \mathbf{I}\rightarrow Y$ là một đồng luân có số hạng $f$ mở rộng $\overline{\sigma}$. Khi đó, ánh xạ $\overline{\tau}: X\times \mathbf{I}\rightarrow Y$ cho bởi $(x, t)\mapsto \tau (x,1-t)$ là một đồng luân mở rộng $\sigma$ và có điểm đầu là ánh xạ $f$.

Cho X là một không gian tôpô, cho A là một không gian con của X và cho $i: A\rightarrow X$ là đơn ánh chính tắc. Kí hiệu $\alpha_i: A\times \mathbf{I}\rightarrow$ Cyl($i$) và $\beta_i: X\rightarrow$ Cyl($i$) là các ánh xạ chính tắc. Cho $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ là ánh xạ liên tục duy nhất sao cho $j(\alpha_i(a, s)) = (i(a), s)$ và $j(\beta_i(x)) = (x,1)$ với $a\in A,s\in \mathbf{I}$ và $x\in X$. Nó là đơn ánh; ảnh của nó là không gian con $(A\times \mathbf{I})\cup (X\times  \{1\})$ của $X\times \mathbf{I}$. Ánh xạ $j$ là đóng nếu A là đóng trong X. Nó không phải lúc nào cũng ngặt (III, p. 325, exerc. 17).

#### Mệnh đề 7 {#ta-iii-s1-prop-7 .statement tag=01VW}

Với các kí hiệu trên, các mệnh đề sau là tương đương:

(i) Cặp $(X,A)$ có tính chất mở rộng đồng luân;

(ii) Với mọi không gian tôpô Y và mọi ánh xạ liên tục $g:$ Cyl($i$)$\rightarrow Y$, tồn tại một ánh xạ liên tục $g': X\times \mathbf{I}\rightarrow Y$ sao cho $g=g'\circ j$;

(iii) Đơn ánh $j$ có một phép co rút liên tục;

(iv) Ánh xạ $j$ là ngặt và tồn tại một phép co của $X\times \mathbf{I}$ lên ảnh của $j$.

Giả sử rằng cặp $(X,A)$ có tính chất mở rộng đồng luân. Cho $g:$ Cyl($i$)$\rightarrow Y$ là một ánh xạ liên tục; đặt $\sigma =g\circ \alpha_i$ và $f=g\circ \beta_i$. Ánh xạ $f: X\rightarrow$ Y là liên tục và $\sigma : A\times \mathbf{I}\rightarrow Y$ là một đồng luân mà điểm cuối là ánh xạ $f|A$. Do đó tồn tại một đồng luân $g': X\times \mathbf{I}\rightarrow Y$ với điểm cuối là $f$ mở rộng $\sigma$. Ta có $g'\circ j(\alpha_i(a, s)) =g'(a, s) =\sigma (a, s) =g(\alpha_i(a, s))$ và $g'\circ j(\beta_i(x)) =$ $g'(x,1) =f(x) =g(\beta_i(x))$ với $a\in A,s\in \mathbf{I}$ và $x\in X$. Do đó, $g'\circ j=g$, suy ra (ii).

Ngược lại, giả sử rằng mệnh đề (ii) được thỏa mãn, và ta chứng minh rằng cặp $(X,A)$ có tính chất mở rộng đồng luân. Cho Y là một không gian tôpô, cho $f: X\rightarrow Y$ là một ánh xạ liên tục và cho $\sigma : A\times \mathbf{I}\rightarrow Y$ là một đồng luân mà điểm cuối bằng $f|A$. Tồn tại một ánh xạ liên tục duy nhất $g:$ Cyl($i$)$\rightarrow Y$ sao cho $g\circ \alpha_i=\sigma$ và $g\circ \beta_i=f$ (III, p. 238, prop. 4). Mọi ánh xạ $g': X\times \mathbf{I}\rightarrow Y$ sao cho $g=g'\circ j$ khi đó là một đồng luân với điểm cuối $f$ mở rộng $\sigma$.

Tính tương đương của các mệnh đề (ii) và (iii) là một trường hợp riêng của bổ đề 1 của III, p. 235.

Giả sử đơn ánh $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ thừa nhận một phép co rút liên tục $r$. Ánh xạ $j$ do đó xác định một đồng phôi của Cyl($i$) lên không gian con $T = (A\times \mathbf{I})\cup (X\times  \{1\})$ của $X\times \mathbf{I}($loc. cit.). Do đó nó là ngặt.

Đặt $\rho =$ pr$_1\circ j\circ r$ và $\theta =$ pr$_2\circ j\circ r$. Nếu $x\in A$ hoặc nếu $s= 1$, ta có $\rho (x, s) =x$ và $\theta (x, s) =s$ Đối với $(x, s)\in X\times \mathbf{I}$ và $t\in \mathbf{I}$, đặt

$$
\sigma ((x, s), t) = (\rho (x,(1-t) +st),(1-t)s+t\theta (x, s))
$$

Ánh xạ $\sigma : (X\times \mathbf{I})\times \mathbf{I}\rightarrow X\times \mathbf{I}$ là liên tục. Đối với $(x, s)\in X\times \mathbf{I}$, ta có

$$
\sigma ((x, s),0) = (\rho (x,1), s) = (x, s)
$$

và

$$
\sigma ((x, s),1) = (\rho (x, s), \theta (x, s)) =j\circ r(x, s)
$$

đối với $x\in X$ và $t\in \mathbf{I}$, ta có

$$
\sigma ((x,1), t) = (\rho (x,1),(1-t) +t\theta (x,1)) = (x,1)
$$

trong khi đó, đối với $(x, s)\in A\times \mathbf{I}$ và $t\in \mathbf{I}$, ta có

$$
\sigma ((x, s), t) = (x,(1-t)s+ts) = (x, s)
$$

Do đó $\sigma$ là một phép co của $X\times \mathbf{I}$ lên T. Điều này chứng minh rằng mệnh đề (iii) kéo theo mệnh đề (iv).

Sự kéo theo (iv)$\Rightarrow$(iii) là hiển nhiên.

#### Nhận xét 2 {#ta-iii-s1-n7-rem-2 .statement tag=01VX}

Cho X là một không gian tôpô Hausdorff và cho A là một tập con của X sao cho cặp $(X,A)$ có tính chất mở rộng đồng luân. Ký hiệu $i: A\rightarrow$ X là đơn ánh chính tắc. Cho $j:$ Cyl($i$)$\rightarrow X\times \mathbf{I}$ là đơn ánh chính tắc và cho $r$ là một phép co rút liên tục của ánh xạ $j$. Không gian con $j$(Cyl($i$)) bằng với tập hợp các cặp $(x, t)\in X\times \mathbf{I}$ sao cho $j(r(x, t)) = (x, t)$. Vì không gian $X\times \mathbf{I}$ là Hausdorff, tập con $j$(Cyl($i$)) là đóng trong $X\times \mathbf{I}$. Tập hợp A, bằng với tập hợp của các $x\in X$ sao cho $(x,0)\in j$(Cyl($i$)), khi đó là một tập con đóng của X.

#### Bổ đề 3 {#ta-iii-s1-lem-3 .statement tag=01VY}

Cho X và Y là các không gian tôpô, cho $p: X\rightarrow Y$ là một ánh xạ liên tục thực sự và mở, và cho $f: X\rightarrow \mathbf{R}$ là một ánh xạ liên tục. Ánh xạ $g: Y\rightarrow \overline{\mathbf{R}}$ cho bởi $y\mapsto$ sup$_{x\in\overset{-1}{p}(y)}f(x)$ là liên tục.

Cho $b\in Y$. Vì $p$ là thực sự, sợi của nó $\overset{-1}{p}(b)$ là một không gian quasi-compact; do đó ta có $g(b)\in \mathbf{R}\cup  \{-\infty \}$.

Cho $m\in \mathbf{R}$ sao cho $g(b)< m$. Với mọi $a\in \overset{-1}{p}(b)$, ta có $f(a)\leqslant$ $g(b)< m$; lấy $V_a$ là một lân cận của $a$ trong X sao cho $f(x)< m$ với mọi $x\in V_a$. Hợp V của các tập hợp $V_a$ là một lân cận của $\overset{-1}{p}(b)$ trong X. Theo Bổ đề 5 (I, p. 75), tồn tại một lân cận W của $b$ trong Y sao cho $\overset{-1}{p}(W)\subset V$. Với mọi $y\in W$, ta có $g(y)\leqslant m$. Điều này chứng minh rằng $g$ là nửa liên tục trên tại $b$.

Bây giờ chứng minh rằng $g$ là nửa liên tục dưới tại $b$. Ta có thể giả sử rằng $g(b)\in \mathbf{R}$. Lấy $m\in \mathbf{R}$ sao cho $m < g(b)$. Lấy $a\in \overset{-1}{p}(b)$ sao cho $m < f(b)$; khi đó lấy V là một lân cận của $a$ trong X sao cho $f(x)> m$ với mọi $x\in V$. Suy ra $g(y)> m$ với mọi $y\in p(V)$. Vì $p$ là mở, $p(V)$ là một lân cận của $b$, do đó $g$ là nửa liên tục dưới.

Vậy bổ đề đã được chứng minh.

#### Định lý 1 {#ta-iii-s1-thm-1 .statement tag=01VZ}

Cho X là một không gian tôpô và A là một không gian con đóng của X; ký hiệu $i: A\rightarrow X$ là đơn ánh chính tắc. Các khẳng định sau là tương đương:

(i) Cặp $(X,A)$ có tính chất mở rộng đồng luân ;

(ii) Tồn tại một ánh xạ liên tục $\varphi : X\rightarrow \mathbf{I}$ sao cho $A =\overset{-1}{\varphi}(0)$ và một đồng luân $\sigma : X\times \mathbf{I}\rightarrow X$ cố định trên A, có số hạng là ánh xạ đồng nhất của X và sao cho $\sigma (x,0)\in A$ với mọi điểm $x\in X$ sao cho $\varphi (x)= 1\not$ .

(iii) Tồn tại một ánh xạ liên tục $\varphi : X\rightarrow \mathbf{R}_+$ sao cho $A =\overset{-1}{\varphi}(0)$ và một đồng luân $\sigma :\overset{-1}{\varphi}(\mathbf{I})\times \mathbf{I}\rightarrow X$, cố định trên A, sao cho $\sigma (x,1) =x$ và $\sigma (x,0)\in A$ với mọi $x\in \overset{-1}{\varphi}(\mathbf{I})$.

(iv) Tồn tại một ánh xạ liên tục $\varphi : X\rightarrow \mathbf{R}_+$ sao cho $A\subset \overset{-1}{\varphi}(0)$ và một ánh xạ liên tục

$$
\sigma :\{(x, t)\in X\times \mathbf{I}|t+\varphi (x)\geqslant 1\} \rightarrow X
$$

sao cho $\sigma (x,1) =x$ với mọi $x\in X$ và $\sigma (x,1-\varphi (x))\in A$ với mọi $x\in X$ sao cho $\varphi (x)\leqslant 1$.

Ta sẽ ký hiệu bởi $i$ đơn ánh chính tắc của A vào X, $\alpha_i: A\times \mathbf{I}\rightarrow$ Cyl($i$) và $\beta_i: X\rightarrow$ Cyl($i$) là các ánh xạ chính tắc, và bởi $j$ ánh xạ từ Cyl($i$) vào $X\times \mathbf{I}$ sao cho $j(\alpha_i(x, s)) = (x, s)$ với $(x, s)\in A\times \mathbf{I}$ và $j(\beta_i(x)) = (x,1)$ với $x\in X$.

Giả sử rằng cặp $(X,A)$ có tính chất mở rộng đồng luân và cho $r: X\times \mathbf{I}\rightarrow$ Cyl($i$) là một phép co rút liên tục của ánh xạ $j($III, p. 241, Proposition 7). Ta ký hiệu bởi $\sigma$ ánh xạ liên tục pr$_1\circ j\circ r$ từ $X\times \mathbf{I}$ vào X. Với mọi $(x, t)\in X\times \mathbf{I}$, ta có $|$pr$_2(j(r(x, t)))-t|\leqslant 1$. Vì $\mathbf{I}$ là compact, phép chiếu thứ nhất pr$_1: X\times \mathbf{I}\rightarrow X$ là một ánh xạ thực sự; nó cũng là mở. Theo Bổ đề 3, ánh xạ $\varphi : X\rightarrow \mathbf{I}$ cho bởi

$x\mapsto$ sup$_{t\in\mathbf{I}}(|$pr$_2(j(r(x, t)))-t|)$

do đó là liên tục.

Với $x\in X$, ta có $\sigma (x,1) =x$. Cho $x\in X$ sao cho $\sigma (x,0)\notin A$; khi đó pr$_2(j(r(x,0))) = 1$ và $\varphi (x)\geqslant 1$. Với $x\in A$ và $t\in \mathbf{I}$, ta có $j(r(x, t)) = (x, t)$; do đó, $\sigma (x, t) =x$ và $\varphi (x) = 0$. Ngược lại, cho $x\in X$ sao cho $\varphi (x) = 0$. Khi đó pr$_2(j(r(x, t))\leqslant t$ với mọi $t\in \mathbf{I}$; nếu $t <1$, điều này kéo theo $j(r(x, t))\in A\times \mathbf{I}$; vì A là đóng trong X, do đó ta có $j(r(x,1))\in A\times \mathbf{I}$, suy ra $x\in A$.

Điều này chứng minh rằng (i) kéo theo (ii).

Cho $\varphi$ và $\sigma$ là các ánh xạ thỏa mãn các tính chất của mệnh đề (ii). Đặt $\varphi_1= 2\varphi$ và gọi $\sigma_1$ là hạn chế của $\sigma$ vào $\overset{-1}{\varphi}_{1}(\mathbf{I})\times \mathbf{I}$. Ta có $\overset{-1}{\varphi}_{1}(0) = A$; với $a\in A,\sigma_1(a, t) =a$ với mọi $a\in A$. Cho $x\in X$ sao cho $\varphi_1(x)\leqslant 1$; ta có $\sigma_1(x,1) =x$; hơn nữa, $\varphi (x) =\varphi_1(x)/2<1$, do đó $\sigma_1(x,0)\in A$. Vậy, (ii) suy ra (iii).

Ta chứng minh rằng (iii) suy ra (iv). Cho $\varphi : X\rightarrow \mathbf{R}$ và $\sigma :\overset{-1}{\varphi}(\mathbf{I})\times$ $\mathbf{I}\rightarrow X$ như trong mệnh đề; đặt $B =\overset{-1}{\varphi}(\mathbf{I})$ và $C =\overset{-1}{\varphi}([1,+\infty [)$.

Gọi $u_1$ là ánh xạ từ $B\times \mathbf{I}$ vào X sao cho $u_1(x, t) =\sigma (x,1-$ $(1-t)/2\varphi (x))$ nếu $t+ 2\varphi (x)\geqslant 1$ và $\varphi (x)>0$ và $u_1(x, t) =\sigma (x,0)$ trong trường hợp ngược lại. Theo bổ đề 4 sau đây, nó liên tục.

Gọi $u_2$ là ánh xạ từ $B\times \mathbf{I}$ vào X sao cho $u_2(x, t) =$ $\sigma (x$, sup(0$,1-2(1-t)(1-\varphi (x))$)). Nó liên tục. Với $x\in B$ sao cho $\varphi (x) = 1/2$ và $t\in \mathbf{I}$, ta có $u_1(x, t) =\sigma (x, t) =u_2(x, t)$. Gọi $u: B\times \mathbf{I}\rightarrow X$ là ánh xạ sao cho $u(x, t) =u_1(x, t)$ nếu $\varphi (x)\leqslant 1/2$ và $u(x, t) =u_2(x, t)$ nếu $1/2< x\leqslant 1$ ; nó liên tục vì các hạn chế của nó vào các không gian con đóng $\overset{-1}{\varphi}([0,1/2])\times \mathbf{I}$ và $\overset{-1}{\varphi}([1/2,1])\times \mathbf{I}$ của $B\times \mathbf{I}$ là liên tục (TG, I, p. 19, prop. 4).

Với $x\in X$ sao cho $\varphi (x) = 1$ và $t\in \mathbf{I}$, ta có $u(x, t) =u_2(x, t) =$ $\sigma (x,1) =x$. Do đó tồn tại một ánh xạ duy nhất $\tau : X\times \mathbf{I}\rightarrow X$ trùng với $u$ trên $B\times \mathbf{I}$ và với ánh xạ pr$_1$ trên $C\times \mathbf{I}$; nó liên tục (loc. cit.).

Cho $x\in X$; ta kiểm tra được rằng $\tau (x,1) = 1$. Hơn nữa, nếu $x\in A$, thì $\varphi (x) = 0$, do đó $\tau (x, t) =u_1(x, t) =\sigma (x,0) =x$. Cuối cùng, nếu $2\varphi (x)\leqslant 1$, thì $\varphi (x)\leqslant 1/2$, do đó $\tau (x,1-2\varphi (x)) =\sigma (x,0)\in A$.

Điều này chứng minh rằng mệnh đề (iv) được thỏa mãn.

Cuối cùng, giả sử mệnh đề (iv) được thỏa mãn, và ta chứng minh rằng cặp $(X,A)$ có tính chất mở rộng đồng luân.

Gọi $C_1$ (resp. $C_2$) là tập hợp các cặp $(x, t)\in X\times \mathbf{I}$ sao cho $t+\varphi (x)\leqslant 1$ (resp. $t+\varphi (x)\geqslant$ 1). Đây là các tập hợp đóng. Với $(x, t)\in C_1$, ta có $\sigma (x,1-\varphi (x))\in A$; khi đó, gọi $\rho_1: C_1\rightarrow$ Cyl($i$) là ánh xạ xác định bởi $(x, t)\mapsto \alpha_i(\sigma (x,1-\varphi (x)), t+\varphi (x))$; nó liên tục. Gọi $\rho_2: C_2\rightarrow$ Cyl($i$) là ánh xạ liên tục xác định bởi $(x, t)\mapsto \beta_i(\sigma (x, t))$. Với $(x, t)\in C_1\cap C_2$, ta có $t+\varphi (x) = 1$, do đó

$$
\rho_1(x, t) =\alpha_i(\sigma (x,1-\varphi (x)),1) =\beta_i(\sigma (x,1-\varphi (x)) =\rho_2(x, t)
$$

Do đó tồn tại một ánh xạ duy nhất $\rho : X\times \mathbf{I}\rightarrow$ Cyl($i$) trùng với $\rho_1$ trên $C_1$ và với $\rho_2$ trên $C_2$; nó liên tục (TG, I, p. 19, prop. 4).

Với $x\in A$ và $t\in \mathbf{I}$, ta có $\varphi (x) = 0$, do đó $t+\varphi (x)\leqslant 1$

$$
\rho (j(\alpha_i(x, t))) =\rho (x, t) =\alpha_i(\sigma (x,1), t) =\alpha_i(x, t)
$$

Với $x\in X$, ta cũng có

$$
\rho (j(\beta_i(x))) =\rho (x,1) =\beta_i(\sigma (x,1)) =\beta_i(x)
$$

Vì các ảnh của các ánh xạ $\alpha_i$ và $\beta_i$ phủ Cyl($i$), suy ra rằng ánh xạ $\rho$ là một phép co rút liên tục của ánh xạ $j$. Do đó, cặp $(X,A)$ có tính chất mở rộng đồng luân (III, p. 241, prop. 7), điều này kết thúc chứng minh định lý.

#### Bổ đề 4 {#ta-iii-s1-lem-4 .statement tag=01W0}

Cho X và Y là các không gian tôpô, cho $\varphi : X\rightarrow \mathbf{R}_+$ là một ánh xạ liên tục, và đặt $A =\overset{-1}{\varphi}(0)$. Cho $\sigma : X\times \mathbf{I}\rightarrow Y$ là một đồng luân cố định trên A. Ánh xạ $\sigma ': X\times \mathbf{I}\rightarrow Y$ biến $(x, s)$ thành $\sigma (x, s/\varphi (x))$ nếu $s < \varphi (x)$ và thành $\sigma (x,1)$ nếu $s\geqslant \varphi (x)$ là liên tục.

Ánh xạ $\sigma '$ liên tục tại mọi điểm của tập con đóng $\overset{-1}{\varphi}([1,+\infty [)\times \mathbf{I}$; do đó chỉ cần chứng minh rằng hạn chế của nó lên $\overset{-1}{\varphi}(\mathbf{I})\times \mathbf{I}$ là liên tục. Vì vậy ta có thể giả sử rằng $\varphi (X)\subset \mathbf{I}$. Gọi C và $C'$ là các không gian con của $X\times \mathbf{I}$ gồm các cặp $(x, s)$ sao cho $s\leqslant \varphi (x)$ và $s\geqslant \varphi (x)$ tương ứng. Chúng là các tập đóng và phủ $X\times \mathbf{I}$. Ánh xạ $\sigma '$ liên tục trên $C'$; ta hãy chứng minh rằng nó liên tục trên C.

Gọi $\alpha : X\times \mathbf{I}\rightarrow X\times \mathbf{I}$ là ánh xạ liên tục được xác định bởi $\alpha (x, t) =$ $(x, t\varphi (x))$. Ảnh của nó bằng C và $\sigma '\circ \alpha$ là ánh xạ liên tục $\sigma$. Ta hãy chứng minh rằng $\alpha$ là một ánh xạ thực sự. Thật vậy, xét một siêu lọc $\mathfrak{U}$ trên $X\times \mathbf{I}$ và một điểm $(x, t)\in X\times \mathbf{I}$ dính với cơ sở siêu lọc $\alpha (\mathfrak{U})$. Vì pr$_1\circ \alpha =$ pr$_1$, cơ sở siêu lọc pr$_1(\mathfrak{U})$ trên X hội tụ về $x$. Vì $\mathbf{I}$ compact, tồn tại một điểm $s\in \mathbf{I}$ sao cho cơ sở siêu lọc pr$_2(\mathfrak{U})$ hội tụ về $s$. Khi đó $\mathfrak{U}$ hội tụ về $(x, s)$. Vì $\alpha$ liên tục, cơ sở siêu lọc $\alpha (\mathfrak{U})$ hội tụ về $(x, s\varphi (x))$. Vì $\mathbf{I}$ là Hausdorff, ta có $s\varphi (x) =t$, do đó $\alpha (x, s) = (x, t)$, nên $\alpha$ là thực sự (TG, I, p. 75, Định lý 1). Từ I, p. 18, ví dụ 2 và Mệnh đề 9, suy ra rằng $\sigma '|C$ liên tục.

#### Hệ quả 1 {#ta-iii-s1-lem-4-cor-1 .statement tag=01W1}

Cho X là một không gian tôpô chuẩn tắc và A là một không gian con đóng của X. Giả sử tồn tại một lân cận V của A trong X và một phép co V lên A, cùng với một ánh xạ liên tục $f: X\rightarrow \mathbf{R}$ sao cho $\overset{-1}{f}(0) = A$. Khi đó cặp $(X,A)$ có tính chất mở rộng đồng luân.

Gọi $\rho : V\times \mathbf{I}\rightarrow V$ là một phép co V lên A. Theo định nghĩa của một không gian chuẩn tắc (TG, IX, p. 41, Định nghĩa 1), tồn tại một ánh xạ liên tục $g: X\rightarrow \mathbf{I}$ bằng 0 trên A và bằng 1 tại mọi điểm của X - V. Gọi $\varphi : X\rightarrow \mathbf{R}$ là ánh xạ được xác định bởi $\varphi (x) =|f(x)|+g(x)$ với $x\in X$; nó liên tục. Ta có $\overset{-1}{\varphi}(0) = A$ và $\overset{-1}{\varphi}(\mathbf{I})\subset V$. Gọi $\sigma$ là ánh xạ từ $\overset{-1}{\varphi}(\mathbf{I})\times \mathbf{I}$ vào X được xác định bởi $\sigma (x, t) =\rho (x,1-t)$ với $x\in \overset{-1}{\varphi}(\mathbf{I})$ và $t\in \mathbf{I}$. Với $x\in \overset{-1}{\varphi}(\mathbf{I})$, ta có $\sigma (x,1) =\rho (x,0) =x$ và $\sigma (x,0) =\rho (x,1)\in A$.

Các ánh xạ $\varphi$ và $\sigma$ thỏa mãn các điều kiện của mệnh đề (iii) của định lý 1 của III, p. 243; do đó cặp $(X,A)$ có tính chất mở rộng đồng luân.

#### Ví dụ 1 {#ta-iii-s1-n7-exa-1 .statement tag=01W2}

Lấy không gian X là quả cầu $\mathbf{B}_n$ và không gian con A là mặt cầu $\mathbf{S}_{n-1}$. Nếu V = X$-\{0\}$, tồn tại một phép co mạnh của V lên $\mathbf{S}_{n-1}($III, p. 237, ví dụ). Do đó cặp $(\mathbf{B}_n,\mathbf{S}_{n-1})$ có tính chất mở rộng đồng luân.

#### Hệ quả 2 {#ta-iii-s1-lem-4-cor-2 .statement tag=01W3}

Cho X và Y là các không gian tôpô, cho A là một không gian con đóng của X, cho B là một không gian con đóng của Y. Nếu các cặp $(X,A)$ và $(Y,B)$ có tính chất mở rộng đồng luân, thì điều tương tự cũng đúng với cặp $(X\times Y,(X\times B)\cup (A\times Y))$.

Cho $\varphi : X\rightarrow \mathbf{R}_+$ và $\sigma :\overset{-1}{\varphi}(\mathbf{I})\times \mathbf{I}\rightarrow$ X, tương ứng $\varphi ': Y\rightarrow \mathbf{R}_+$

và $\sigma ':\overset{-1}{\psi}(\mathbf{I})\times \mathbf{I}\rightarrow Y$, thỏa mãn các điều kiện của mệnh đề (iv) của định lý 1 đối với cặp $(X,A)$, tương ứng đối với cặp $(Y,B)$. Cho $\psi : X\times Y\rightarrow \mathbf{R}_+$ là ánh xạ cho bởi $(x, y)\mapsto$ inf($\varphi (x), \varphi '(x)$) ; nó liên tục; ta cũng có $\psi (x, y) = 0$ với mọi $(x, y)\in X\times Y$ sao cho $x\in A$ hoặc $y\in B$. Với $(x, y, t)\in X\times Y\times \mathbf{I}$ sao cho $t+\psi (x)\geqslant 1$, ta có $t+\varphi (x)\geqslant 1$ và $t+\varphi '(x)\geqslant 1$. Do đó ta xác định một ánh xạ liên tục

$$
\tau :\{(x, y, t)\in X\times Y\times \mathbf{I}|t+\psi (x)\geqslant 1\} \rightarrow X\times Y
$$

bằng cách đặt $\tau (x, y, t) = (\sigma (x, t), \sigma '(y, t))$. Với mọi $(x, y)\in X\times Y$, ta có $\tau (x, y,1) = (\sigma (x,1), \sigma '(y,1)) = (x, y)$. Hơn nữa, nếu $\psi (x, y)\leqslant 1$, thì $\varphi (x)\leqslant 1$ hoặc $\varphi '(y)\leqslant 1$, do đó $\sigma (x,1)\in A$ hoặc $\sigma '(y,1)\in B$; suy ra rằng $\tau (x, y,1-\psi (x))$ thuộc $(A\times Y)\cup (X\times B)$. Điều này kiểm chứng mệnh đề (iv) của định lý 1, do đó hệ quả.

#### Ví dụ 2 {#ta-iii-s1-n7-exa-2 .statement tag=01W4}

*Đây là các trường hợp khác trong đó cặp $(X,A)$ có tính chất mở rộng đồng luân.

(i) Không gian X là một đa tạp khả vi paracompact thuộc lớp $C^1$ và A là một đa tạp con đóng của X. Theo hệ quả1, điều này suy ra từ sự kiện rằng X là hoàn toàn chuẩn (IX, p. 103, bài tập 11) và A có một lân cận hình ống trong X;

(ii) Không gian X là một không gian tế bào và A là một không gian con đầy đủ đối với một phân tích tế bào đã cho của X.*

### 8. Gắn một không gian tôpô

Cho $X,B$ là các không gian tôpô, cho A là một không gian con của B, và cho $f: A\rightarrow X$ là một ánh xạ liên tục. Ký hiệu Y là tổng tôpô của các không gian $Y_1= X$ và $Y_2= B$, và đồng nhất $Y_1$ và $Y_2$ với các không gian con của Y nhờ các đơn ánh chính tắc. Gọi R là quan hệ tương đương mịn nhất trong Y sao cho các phần tử $a$ của $Y_2$ và $f(a)$ của $Y_1$ là tương đương, với mọi $a\in A$. Quan hệ R là quan hệ đẳng thức trên $Y_1$. Cho $x\in Y_1$ và $b\in Y_2$; ta có $xRb$ khi và chỉ khi $b\in A$ và $f(b) =x$. Cho $b, b'\in Y_2$; để có $bRb'$, điều kiện cần và đủ là $b=b'$, hoặc $b, b'\in A$ và $f(b) =f(b')$.

#### Định nghĩa 9 {#ta-iii-s1-def-9 .statement tag=01W5}

Không gian tôpô thương $Y/R$ được gọi là không gian thu được bằng cách gắn không gian B vào không gian X theo ánh xạ $f$. Nó được ký hiệu là $X\cup_fB$.

Gọi $\alpha_f: X\rightarrow X\cup_fB$ và $\beta_f: B\rightarrow X\cup_fB$ là các hạn chế xuống $Y_1$ và $Y_2$ của toàn cấu chính tắc từ Y lên $Y/R$. Ta có $\alpha_f\circ f=\beta_f|A$.

#### Nhận xét 1 {#ta-iii-s1-n8-rem-1 .statement tag=01W6}

Ánh xạ $\alpha_f$ là đơn ánh. Với mọi tập con U

của X, ta có $\alpha^{-1}_f(\alpha_f(U)) = U$ và $\beta^{-1}_f(\alpha_f(U)) =\overset{-1}{f}(U)$. Nếu A là một tập con mở (tương ứng, đóng) của B, các quan hệ này suy ra rằng $\alpha_f$ là một ánh xạ mở (tương ứng, đóng) từ X vào $X\cup_fB$.

Cho U là một tập con mở của X và V là một tập con mở của B sao cho $\overset{-1}{f}(U) = V\cap A$. Hợp của các tập con U của $Y_1$ và V của $Y_2$ là một tập con mở bão hòa của Y; do đó ảnh của nó trong $X\cup_fB$ là mở, và vết của nó trên $\alpha_f(X)$ là $\alpha_f(U)$. Suy ra ánh xạ $\alpha_f$ xác định một phép đồng phôi của X lên ảnh của nó trong $X\cup_fB$.

#### Nhận xét 2 {#ta-iii-s1-n8-rem-2 .statement tag=01W7}

Cho V là một tập con của B. Ta có $\alpha^{-1}_f(\beta_f(V)) =f(V\cap A)$ và

$\beta^{-1}_f(\beta_f(V)) = V\cup \overset{-1}{f}(f(V\cap A))$. Nếu A đóng trong B và nếu ánh xạ $f$ đóng, thì ánh xạ $\beta_f$ do đó đóng. Tương tự, nếu A mở trong B và nếu ánh xạ $f$ mở, thì ánh xạ $\beta_f$ mở.

Trong hai trường hợp này, ánh xạ $\beta_f$ cảm sinh một phép đồng phôi của B-A lên ảnh của nó.

#### Nhận xét 3 {#ta-iii-s1-n8-rem-3 .statement tag=01W8}

Giả sử A đóng và ánh xạ $f$ thực sự. Ta vừa thấy rằng ánh xạ $\beta_f$ đóng. Với mọi $x\in X$,

$\beta^{-1}_f(\alpha_f(x)) =\overset{-1}{f}(x)$. Do đó nó là một tập con quasi-compact của A (TG,

I, p. 75, Định lý 1), và do đó cũng của B. Với mọi $b\in B,\beta^{-1}_f(\beta_f(b))$

bằng $\{b\}$ nếu $b\in B-A$, và bằng $\overset{-1}{f}(f(b))$ nếu $b\in A$; trong cả hai trường hợp, nó là một tập con tựa compact của B. Các thớ của ánh xạ $\beta_f$ do đó là tựa compact; do đó (loc. cit.), ánh xạ $\beta_f$ là thực sự.

Ánh xạ $\alpha_f$ cũng thực sự (TG, I, p. 72, prop. 2). Suy ra rằng ánh xạ chính tắc của Y lên $X\cup_fB$ là thực sự.

#### Ví dụ 1 {#ta-iii-s1-n8-exa-1 .statement tag=01W9}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Hình trụ Cyl($f$) chính là không gian thu được bằng cách gắn không gian Y vào không gian $X\times \mathbf{I}$ dọc theo ánh xạ $f\circ$ pr$_1$ của $X\times  \{1\}$ vào Y.

#### Ví dụ 2 {#ta-iii-s1-n8-exa-2 .statement tag=01WA}

Cho X là một không gian tôpô, cho B là một không gian tôpô và cho A là một không gian con của B, và cho $f: A\rightarrow X$ là một ánh xạ liên tục cảm sinh một đồng phôi của A lên ảnh của nó.

Đặt $A'=f(A)$; gọi $f'$ là ánh xạ của $A'$ vào B gán cho mỗi $x\in A'$ ảnh ngược duy nhất của $x$ bởi f. Ánh xạ $f'\circ f$ là liên tục; vì $f$ là ngặt, ánh xạ $f'$ là liên tục. Có một ánh xạ liên tục duy nhất $u$ của không gian $X\cup_fB$ vào không gian $B\cup_{f'}X$ biến $\alpha_f(x)$ thành $\beta_{f'}(x)$ với $x\in X$ và $\beta_f(b)$ thành $\alpha_{f'}(b)$ với $b\in B$; nó là một đồng phôi biến không gian con $\alpha_f(X)$ lên không gian con $\beta_{f'}(X)$.

#### Mệnh đề 8 {#ta-iii-s1-prop-8 .statement tag=01WB}

Cho Z là một không gian tôpô.

a) Cho $u: X\rightarrow Z$ và $v: B\rightarrow Z$ là các ánh xạ liên tục sao cho $v(a) =u(f(a))$ với mọi $a\in A$. Khi đó tồn tại một ánh xạ liên tục duy nhất $w: X\cup_fB\rightarrow Z$ sao cho $w\circ \alpha_f=u$ và $w\circ \beta_f=v$.

b) Cho $ \sigma : X\times \mathbf{I}\rightarrow Z$ và $\tau : B\times \mathbf{I}\rightarrow Z$ là các phép đồng luân. Giả sử rằng $\tau$ cố định trên A và rằng $\sigma (f(a), t) =\tau (a, t)$ với mọi $a\in A$ và mọi $t\in \mathbf{I}$. Khi đó tồn tại một phép đồng luân duy nhất $\eta : (X\cup_fB)\times \mathbf{I}\rightarrow Z$ sao cho $\eta (\alpha_f(x), t) =\sigma (x, t)$ và $\eta (\beta_f(b), t) =\tau (b, t)$ với $x\in X,b\in B$ và $t\in \mathbf{I}$. Phép đồng luân này cố định trên $\beta_f(A)$.

Mệnh đề suy ra ngay lập tức từ định nghĩa của một không gian thương và prop. 10 (I, p. 19).

#### Hệ quả 1 {#ta-iii-s1-prop-8-cor-1 .statement tag=01WC}

Cho $B'$ là một không gian tôpô, $A'$ là một không gian con của $B'$, và $f': A'\rightarrow$ X là một ánh xạ liên tục. Cho $v: B\rightarrow B'$ là một ánh xạ liên tục sao cho $v(A)\subset A'$ và $f$ = $f'\circ (v|A)$. Cho $w: X\cup_fB\rightarrow X\cup_{f'}B'$ là ánh xạ liên tục duy nhất sao cho $w\circ \alpha_f=\alpha_{f'}$ và $w\circ \beta_f=\beta_{f'}\circ v$. Nếu $v$ xác định một tương đương đồng luân của cặp $(B,A)$ lên cặp $(B',A')$, thì $w$ xác định một tương đương đồng luân của cặp $(X\cup_fB, \alpha_f(X))$ lên cặp $(X\cup_{f'}B', \alpha_{f'}(X))$.

Cho $v': B'\rightarrow B$ là một ánh xạ liên tục, cho $\tau : B\times \mathbf{I}\rightarrow B$ là một đồng luân cố định trên A nối Id$_B$ với $v'\circ v$, và cho $\tau ': B'\times \mathbf{I}\rightarrow B'$ là một đồng luân cố định trên $A'$ nối Id$_{B'}$ với $v\circ v'$. Với $a'\in A'$ và $a=v'(a')$, ta có các hệ thức $a'=v(a)$ và $\beta_f(v'(a')) =\beta_f(a) =\alpha_f(f(a)) =\alpha_f(f'(a'))$. Theo Mệnh đề 8, a), tồn tại một ánh xạ duy nhất $w': X\cup_{f'}B'\rightarrow$ $X\cup_fB$ sao cho $w'\circ \alpha_{f'}=\alpha_{f'}$ và $w'\circ \beta_{f'}=\beta_f\circ v'$. Theo Mệnh đề 8, b), tồn tại một đồng luân duy nhất $\eta : (X\cup_fB)\times \mathbf{I}\rightarrow X\cup_{f'}B'$ sao cho $\eta (\alpha_f(x), t) =\alpha_{f'}(x)$ và $\eta (\beta_f(b), t) =\beta_{f'}(\tau (b, t))$ với $x\in X,b\in B$ và $t\in \mathbf{I}$. Tương tự, tồn tại một đồng luân duy nhất $\eta ': (X\cup_{f'}B')\times \mathbf{I}\rightarrow$ $X\cup_fB$ sao cho $\eta '(\alpha_{f'}(x), t) =\alpha_f(x)$ và $\eta '(\beta_{f'}(b), t) =\beta_f(\tau '(b, t))$ với $x\in X,b\in B'$ và $t\in \mathbf{I}$. Khi đó, ánh xạ từ $(X\cup_fB)\times \mathbf{I}$ vào $X\cup_fB$ xác định bởi $(x, t)\mapsto \eta '(\eta (x, t), t)$ là một đồng luân cố định trên $\alpha_f(X)$ nối ánh xạ đồng nhất của $X\cup_fB$ với ánh xạ $w'\circ w$. Tương tự, ánh xạ từ $(X\cup_{f'}B')\times \mathbf{I}$ vào $X\cup_{f'}B'$ xác định bởi $(x, t)\mapsto \eta (\eta '(x, t), t)$ là một đồng luân cố định trên $\alpha_{f'}(X)$ nối ánh xạ đồng nhất của $X\cup_{f'}B'$ với ánh xạ $w\circ w'$. Hệ quả được suy ra.

#### Ví dụ 3 {#ta-iii-s1-n8-exa-3 .statement tag=01WD}

Cho $i$ là đơn ánh chính tắc của A vào B và lấy không gian $B'$ là trụ của ánh xạ $i$; gọi $\alpha_i: A\times \mathbf{I}\rightarrow$ Cyl($i$) và $\beta_i: B\rightarrow$ Cyl($i$) là các ánh xạ chính tắc và $r_i:$ Cyl($i$)$\rightarrow B$ là phép co rút chính tắc của trụ Cyl($i$) lên cơ sở của nó. Gọi $A_0$ là không gian con $\alpha_i(A\times  \{0\})$ của Cyl($i$) và $f_0: A_0\rightarrow X$ là ánh xạ $f\circ r_i$. Với $a\in A$, ta có

$$
\beta_f\circ r_i(\alpha_i(a,0)) =\beta_f(a) =\alpha_f(f_0(\alpha_i(a,0))) =\alpha_f(f(a))
$$

Gọi $\eta : X\cup_{f_0}$ Cyl($i$)$\rightarrow X\cup_fB$ là ánh xạ liên tục duy nhất sao cho $\eta \circ \alpha_{f_0}=\alpha_f$ và $\eta \circ \beta_{f_0}=\beta_f\circ r_i$. Giả sử cặp $(B,A)$ có tính chất mở rộng đồng luân. Khi đó ánh xạ $r_i$ xác định một tương đương đồng luân của cặp (Cyl($i$)$,A_0$) với cặp $(B,A)$ (III, p. 243, th. 1). Theo Hệ quả 1, khi đó ánh xạ $\eta$ xác định một tương đương đồng luân của cặp $(X\cup_{f'}B', \alpha_{f'}(X))$ với cặp $(X\cup_fB, \alpha_f(X))$. Đặc biệt, $\eta$ là một tương đương đồng luân.

#### Hệ quả 2 {#ta-iii-s1-prop-8-cor-2 .statement tag=01WE}

Cho $X'$ là một không gian tôpô, cho $u: X\rightarrow X'$ là một ánh xạ liên tục, và đặt $f'=u\circ f$. Gọi $w: X\cup_fB\rightarrow X'\cup_{f'}B$ là ánh xạ liên tục duy nhất sao cho $w\circ \alpha_f=\alpha_{f'}\circ u$ và $w\circ \beta_f=\beta_{f'}$. Nếu $u$ xác định một tương đương đồng luân của cặp $(X, f(A))$ với cặp $(X', f'(A))$, thì $w$ xác định một tương đương đồng luân của cặp $(X\cup_fB, \beta_f(B))$ với cặp $(X'\cup_{f'}B, \beta_{f'}(B))$.

Chứng minh tương tự như chứng minh Hệ quả 1.

#### Mệnh đề 9 {#ta-iii-s1-prop-9 .statement tag=01WF}

Cho X và B là các không gian tôpô, cho A là một không gian con của B, và cho $f: A\rightarrow X$ là một ánh xạ liên tục.

a) Nếu cặp $(B,A)$ có tính chất mở rộng đồng luân, thì cặp $(X\cup_fB, \alpha_f(X))$ cũng có tính chất đó.

b) Giả sử ánh xạ $f$ là đơn ánh và ngặt. Nếu cặp $(X, f(A))$ có tính chất mở rộng đồng luân, thì cặp $(X\cup_fB, \beta_f(B))$ cũng có tính chất đó.

a) Giả sử cặp $(B,A)$ có tính chất mở rộng đồng luân. Cho Z là một không gian tôpô, cho $u: X\cup_fB\rightarrow Z$ là một ánh xạ liên tục, và cho $\sigma :\alpha_f(X)\times \mathbf{I}\rightarrow Z$ là một đồng luân mà số hạng cuối là hạn chế của $u$ lên không gian con $\alpha_f(X)$.

Đặt $v_1=u\circ \alpha_f$ và ký hiệu $\tau_1: X\times \mathbf{I}\rightarrow Z$ là ánh xạ xác định bởi $(x, t)\mapsto \sigma (\alpha_f(x), t)$. Đặt $v_2=u\circ \beta_f$. Vì $\beta_f|A =\alpha_f\circ f$, ánh xạ từ $A\times \mathbf{I}$ vào Z biến $(a, t)$ thành $\sigma (\alpha_f(f(a)), t)$ với $a\in A$ và $t\in \mathbf{I}$ là một phép đồng luân mà số hạng cuối bằng ánh xạ $v_2|A$. Vì cặp $(B,A)$ có tính chất mở rộng phép đồng luân, tồn tại một phép đồng luân $\tau_2: B\times \mathbf{I}\rightarrow Z$ mà số hạng cuối là ánh xạ $v_2$ và thỏa mãn $\tau_2(a, t) =\sigma (\alpha_f(f(a)), t)$ với $(a, t)\in A\times \mathbf{I}$.

Với $a\in A$ và $t\in \mathbf{I}$, ta có $\tau_2(a, t) =\tau_1(f(a), t)$. Theo Mệnh đề 8, tồn tại duy nhất một ánh xạ liên tục $\sigma : (X\cup_fB)\times \mathbf{I}\rightarrow Z$ sao cho $\sigma (\alpha_f(x), t) =\sigma_1(x, t)$ và $\sigma (\beta_f(b), t) =\sigma_2(b, t)$, với $x\in X$, $b\in B$ và $t\in \mathbf{I}$. Đó là một phép đồng luân có số hạng cuối là $u$, mở rộng $\tau$, do đó mệnh đề a).

b) Theo Ví dụ 2 (III, p. 249), mệnh đề b) suy ra từ mệnh đề a).

### 9. Không gian thu được bằng cách co một không gian con

Cho X là một không gian tôpô và A là một tập con của X. Xét quan hệ tương đương R mạnh nhất trong X sao cho mọi phần tử của A là tương đương với nhau: hai phần tử của X tương đương theo quan hệ này nếu chúng bằng nhau hoặc nếu cả hai đều thuộc A.

#### Định nghĩa 10 {#ta-iii-s1-def-10 .statement tag=01WG}

Không gian thương của X theo R được ký hiệu là $X/A$ và được gọi là không gian thu được từ X bằng cách co tập con A.

Ký hiệu $\rho : X\rightarrow X/A$ là toàn cấu chính tắc. Cho Y là một không gian tôpô và $f: X\rightarrow Y$ là một ánh xạ liên tục. Để tồn tại một ánh xạ liên tục $g: X/A\rightarrow Y$ sao cho $g\circ \rho =f$, điều kiện cần và đủ là $f$ hằng trên A.

Nếu tập hợp A đóng (resp. mở) trong X, ánh xạ $\rho$ đóng (resp. mở) và cảm sinh một phép đồng phôi của X-A lên ảnh của nó. Nếu A là một tập con đóng và quasi-compact của X, ánh xạ $\rho$ là thực sự (TG, I, p. 75, th. 1).

Nếu tập hợp A rỗng, $\rho$ là một phép đồng phôi. Nếu nó không rỗng, A là một điểm của $X/A$ được gọi là điểm cơ sở của $X/A$ và được ký hiệu là $s_{X/A}$. Khi đó không gian $X/A$ được đồng nhất với không gian thu được bằng cách gắn không gian X vào không gian $\{s_{X/A}\}$ bằng ánh xạ duy nhất từ A vào $\{s_{X/A}\}$.

#### Mệnh đề 10 {#ta-iii-s1-prop-10 .statement tag=01WH}

Cho X là một không gian tôpô và A là một tập con của $x$. Giả sử tồn tại một phép đồng luân $\sigma : X\times \mathbf{I}\rightarrow X$ có điểm đầu Id$_X$, hằng trên $A\times  \{1\}$ và sao cho $\sigma (A\times \mathbf{I})\subset A$. Khi đó ánh xạ chính tắc $\rho$ của X vào $X/A$ là một tương đương đồng luân.

Cho $f$ là ánh xạ tận cùng của $\sigma$. Đó là một ánh xạ liên tục từ X vào X, đồng luân với Id$_X$. Nó là hằng trên A; do đó tồn tại duy nhất một ánh xạ liên tục $g: X/A\rightarrow X$ sao cho $g\circ \rho =f$. Mặt khác, vì $\sigma (A\times \mathbf{I})\subset A$, tồn tại một ánh xạ $\sigma '$ từ $X/A\times \mathbf{I}$ vào $X/A$ sao cho $\sigma '(\rho (x), t) =\rho (\sigma (x, t))$ với mọi $x\in X$ và mọi $t\in \mathbf{I}$. Theo I, p. 19, mệnh đề 10, ánh xạ $\sigma '$ là liên tục. Đó là một đồng luân nối ánh xạ đồng nhất của $X/A$ với ánh xạ $\rho \circ g$. Do đó, các ánh xạ $g$ và $\rho$ là nghịch đảo đồng luân của nhau.

#### Nhận xét {#ta-iii-s1-n9-rem-1 .statement tag=01WI}

Cho X là một không gian tôpô và A là một tập con của X.

1) Nếu ánh xạ chính tắc từ X lên $X/A$ là một tương đương đồng luân, thì tồn tại một đồng luân $\sigma : X\times \mathbf{I}\rightarrow X$ có ánh xạ ban đầu là Id$_X$ và là hằng trên $A\times  \{1\}$. Tuy nhiên, có thể không tồn tại đồng luân như vậy thỏa mãn thêm điều kiện $\sigma (A\times \mathbf{I})\subset A$ (III, p. 322, bài tập 4).

2) Có thể tồn tại một đồng luân nối ánh xạ đồng nhất của X với một ánh xạ từ X vào X là hằng trên A, mà không phải hai không gian X và $X/A$ tương đương đồng luân (III, p. 325, bài tập 14).

3) Giả sử A co được. Nếu cặp $(X,A)$ có tính chất mở rộng đồng luân, thì ánh xạ chính tắc từ X lên $X/A$ là một tương đương đồng luân. Thật vậy, cho $\sigma : A\times \mathbf{I}\rightarrow A$ là một đồng luân có ánh xạ ban đầu là ánh xạ đồng nhất của A và ánh xạ tận cùng là một ánh xạ hằng. Khi đó tồn tại một đồng luân $\sigma '$ có ánh xạ ban đầu Id$_X$ và mở rộng $\sigma$. Mệnh đề này suy ra từ mệnh đề 10.

4) Cho X và Y là các không gian tôpô, A là một không gian con khác rỗng của X và B là một không gian con của Y. Cho $f: X\rightarrow Y$ là một ánh xạ liên tục sao cho $f(A)\subset B$. Ký hiệu $\varphi : X/A\rightarrow Y/B$ là ánh xạ liên tục suy ra từ $f$ bằng cách chuyển qua các thương. Nếu $f$ xác định một tương đương đồng luân của cặp $(X,A)$ lên cặp $(Y,B)$, thì ánh xạ $\varphi$ là một tương đương đồng luân của cặp $(X/A, s_{X/A})$ lên cặp $(Y/B, s_{Y/B})$. Cho P là một không gian tôpô thu gọn về một điểm, và cho $\alpha$ và $\beta$ là các ánh xạ hằng từ A và B vào P. Chú ý rằng ánh xạ $\varphi$ được đồng nhất với ánh xạ từ $P\cup_{\alpha}X$ vào $P\cup_{\beta}Y$ suy ra từ $f$ và ánh xạ đồng nhất của P. Mệnh đề này suy ra từ hệ quả 1 của III, p. 249.

### 10. Nón của một ánh xạ

Cho X và Y là các không gian tôpô và cho $f$ là một ánh xạ liên tục từ X vào Y. Gọi Cyl($f$) là trụ của ánh xạ $f$. Gọi $\alpha_f$ là ánh xạ chính tắc từ $X\times \mathbf{I}$ vào Cyl($f$) và $f_0$ là ánh xạ $x\mapsto \alpha_f(x,0)$ từ X vào Cyl($f$); các ánh xạ này cảm sinh các phép đồng phôi lần lượt từ $X\times \mathbf{I}$ và X lên các ảnh của chúng trong Cyl($f$).

#### Định nghĩa 11 {#ta-iii-s1-def-11 .statement tag=01WJ}

**Nón** của ánh xạ $f$ là không gian tôpô suy ra từ Cyl($f$) bằng cách co $f_0(X)$ về một điểm; nó được ký hiệu là Côn$(f)$.

Cho $\beta '_f: Y\rightarrow$ Côn$(f)$ là hợp thành của ánh xạ chính tắc $\beta_f: Y\rightarrow$ Cyl($f$) và toàn cấu chính tắc của Cyl($f$) lên Côn$(f)$. Ánh xạ $\beta '_f$ liên tục và xác định một phép đồng phôi Y lên một tập con đóng của Côn$(f)$, gọi là cơ sở của nón, và do đó ta sẽ đồng nhất nó với Y.

Cho $\alpha '_f: X\times \mathbf{I}\rightarrow$ Côn$(f)$ là hợp thành của ánh xạ $\alpha_f$ và toàn cấu chính tắc của Cyl($f$) lên Côn$(f)$. Ánh xạ $\alpha '_f$ là một phép đồng luân mà số hạng đầu là một ánh xạ hằng và số hạng cuối là ánh xạ $\beta '_f\circ f$.

Nếu X rỗng, ánh xạ $\beta '_f$ là một phép đồng phôi Y lên Côn$(f)$.

Giả sử X không rỗng. Khi đó, gọi $s$ là điểm cơ sở của không gian Cyl($f$)$/f_0(X)$; nó được gọi là đỉnh của nón Côn$(f)$. Vì $f_0(X)$ đóng trong Cyl($f$), ánh xạ chính tắc $\pi :$ Cyl($f$)$\rightarrow$ Côn$(f)$ cảm sinh một phép đồng phôi của Cyl($f$)$-f_0(X)$ lên Côn$(f)-\{s\}($III, p. 252). Đỉnh của nón Côn$(f)$ không thuộc cơ sở của nó; đơn ánh chính tắc của Y vào Côn$(f)-\{s\}$ là một tương đương đồng luân (III, p. 239, prop. 6).

Cho $\sigma_f:$ Cyl($f$)$\times \mathbf{I}\rightarrow$ Cyl($f$) là phép co chính tắc của hình trụ của $f$ lên cơ sở của nó. Với $c\in$ Cyl($f$)$-f_0(X)$ và $t\in \mathbf{I}$, ta có $\sigma_f(c, t)\notin f_0(X)$. Do đó tồn tại một ánh xạ duy nhất $\sigma '_f: ($Côn$(f)-\{s\})\times \mathbf{I}\rightarrow$ Côn$(f)-\{s\}$ sao cho $\sigma '_f(\pi (c), t) =\pi (\sigma_f(c, t))$ với $c\in$ Cyl($f$)$-f_0(X)$ và $t\in \mathbf{I}$. Nó liên tục và là một phép co mạnh của Côn$(f)-\{s\}$ lên Y. Nó được gọi là phép co chính tắc của Côn$(f)-\{s\}$ lên cơ sở của nó. Số hạng cuối của nó là một phép rút về của Côn$(f)-\{s\}$ lên Y, gọi là phép rút về chính tắc của nón bị bỏ đỉnh lên cơ sở của nó.

Mệnh đề 11 (Tính chất phổ quát của các nón)

Cho Z là một không gian tôpô, cho $\beta : Y\rightarrow Z$ là một ánh xạ liên tục và cho $\alpha : X\times \mathbf{I}\rightarrow Z$ là một phép đồng luân mà số hạng đầu là một ánh xạ hằng và số hạng cuối bằng $\beta \circ f$. Tồn tại một ánh xạ liên tục duy nhất $\varphi$ từ Côn$(f)$ vào Z sao cho $\alpha =\varphi \circ \alpha '_f$ và $\beta =\varphi \circ \beta '_f$.

Từ tính chất phổ quát của các hình trụ (III, p. 238, prop. 4), tồn tại duy nhất một ánh xạ liên tục $h:$ Cyl($f$)$\rightarrow$ Z sao cho $\alpha =h\circ \alpha_f$ và $\beta =h\circ \beta_f$. Vì nguồn của $\alpha$ là một ánh xạ hằng, hạn chế của $h$ trên không gian con $\alpha_f(X\times \{0\})$ là hằng. Do đó tồn tại duy nhất một ánh xạ liên tục $\varphi :$ Cone$(f)\rightarrow Z$ sao cho $h=\varphi \circ \pi$, trong đó $\pi$ ký hiệu toàn cấu chính tắc của Cyl($f$) lên Cone$(f)$. Ánh xạ $\varphi$ thỏa mãn $\alpha =\varphi \circ \alpha '_f$ và $\beta =\varphi \circ \beta '_f$ và là ánh xạ duy nhất có các tính chất này, vì các ảnh của $\alpha '_f$ và $\beta '_f$ phủ Cone$(f)$.

#### Ví dụ 1 {#ta-iii-s1-n10-exa-1 .statement tag=01WK}

Cho X là một không gian tôpô. Người ta ký hiệu C(X), và gọi là nón của không gian X, nón của ánh xạ Id$_X$; đó là không gian thu được từ $X\times \mathbf{I}$ bằng cách co $X\times  \{0\}$. Gọi $\pi$ là ánh xạ chính tắc từ $X\times \mathbf{I}$ vào C(X); ảnh $C'(X)$ của $X\times [0,1[$ qua $\pi$ được gọi là nón mở của không gian X.

Giả sử X không rỗng. Khi đó nón C(X) không rỗng và điểm cơ sở của nó lại được gọi là đỉnh của nón.

Ánh xạ $((x, t), u)\mapsto (x, t(1-u))$ từ $(X\times \mathbf{I})\times \mathbf{I}$ vào $X\times \mathbf{I}$ là một đồng luân nối ánh xạ đồng nhất của $X\times \mathbf{I}$ với ánh xạ $(x, t)\mapsto (x,0)$. Từ đó, bằng cách chuyển qua các tập hợp thương, suy ra một ánh xạ $\sigma : C(X)\times \mathbf{I}\rightarrow C(X)$ sao cho $\sigma (\pi (x, t), u) =\pi (x, t(1-u))$ với $x\in X,t, u\in \mathbf{I}$. Ánh xạ $\sigma$ liên tục theo I, p. 19, prop. 10. Khi đó ánh xạ $\sigma$ là một đồng luân có điểm cơ sở tại $s$, nối ánh xạ đồng nhất của C(X) với ánh xạ hằng có ảnh $\{s\}$. Do đó, nón C(X) co được về đỉnh $s$ của nó. Vì $\sigma (C'(X)\times \mathbf{I})$ được chứa trong $C'(X)$, ánh xạ $\sigma$ xác định, bằng cách chuyển qua các không gian con, một đồng luân có điểm cơ sở tại $s$, nối ánh xạ đồng nhất của $C'(X)$ với ánh xạ hằng có ảnh $\{s\}$; do đó nón mở $C'(X)$ co được về $s$.

#### Nhận xét 1 {#ta-iii-s1-n10-rem-1 .statement tag=01WL}

Cho X là một không gian tôpô và A là một không gian con của X; ký hiệu $i$ là đơn ánh chính tắc của A vào X. Phép co rút chính tắc $r_i$ của hình trụ Cyl($i$) lên cơ sở của nó ánh xạ không gian con $\alpha_i(A\times  \{0\})$ vào A. Cho $\rho :$ Cone$(i)\rightarrow X/A$ là ánh xạ liên tục suy ra từ nó bằng cách chuyển qua các không gian thương. Giả sử cặp $(X,A)$ có tính chất mở rộng đồng luân. Theo III, p. 243, Định lý 1, ánh xạ $r_i$ xác định một tương đương đồng luân của cặp (Cyl($i$)$, \alpha_i(A\times  \{0\})$) với cặp $(X,A)$. Theo Nhận xét 4 của III, p. 253, khi đó ánh xạ $\rho$ là một tương đương đồng luân của cặp (Cone$(i), s$) với cặp $(X, s_{X/A})$. Đặc biệt, nó là một tương đương đồng luân.

#### Nhận xét 2 {#ta-iii-s1-n10-rem-2 .statement tag=01WM}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Ánh xạ chính tắc $\alpha '_f: X\times \mathbf{I}\rightarrow$ Cone$(f)$ là hằng trên $X\times  \{0\}$ và do đó xác định một ánh xạ liên tục $\gamma_f: C(X)\rightarrow$ Cone$(f)$. Hạn chế của ánh xạ $\gamma_f$ lên $C'(X)$ là đơn ánh và ngặt, và xác định, bằng cách chuyển qua các không gian con, một phép đồng phôi của nón mở $C'(X)$ lên phần bù của Y trong Cone$(f)$.

Đồng nhất cơ sở của nón C(X) với không gian X và ký hiệu $u$ là ánh xạ liên tục của $Y\cup_fC(X)$ vào Cone$(f)$ suy ra từ các ánh xạ $\beta '_f: Y\rightarrow$ Cone$(f)$ và $\gamma_f: C(X)\rightarrow$ Cone$(f)$. Ngược lại, cho $v:$ Cone$(f)\rightarrow Y\cup_fC(X)$ là ánh xạ liên tục duy nhất sao cho $v\circ \alpha '_f$ là ánh xạ chính tắc của $X\times \mathbf{I}$ lên C(X) và $v\circ \beta '_f$ là ánh xạ chính tắc của Y lên $Y\cup_fC(X)$. Các ánh xạ $u$ và $v$ là các phép đồng phôi nghịch đảo của nhau.

## BÀI TẬP {#ta-iii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
