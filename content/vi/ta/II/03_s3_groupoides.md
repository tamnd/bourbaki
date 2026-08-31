---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 3
section_title: Groupoïdes
lang: vi
source: ta-i-iv-fr
book_pages: TA II.159-TA II.179, TA II.223-TA II.227
pdf_pages: 0175-0195, 0239-0243
extraction: native
subsections:
    - "no": 1
      title: Catégories
      page: 159
      pdf_page: 175
    - "no": 2
      title: Foncteurs
      page: 161
      pdf_page: 177
    - "no": 3
      title: Groupoïdes
      page: 162
      pdf_page: 178
    - "no": 4
      title: Orbites d’un groupoïde
      page: 162
      pdf_page: 178
    - "no": 5
      title: Exemples de groupoïdes
      page: 163
      pdf_page: 179
    - "no": 6
      title: Sous-groupoïdes
      page: 164
      pdf_page: 180
    - "no": 7
      title: Opérations d’un groupoïde
      page: 167
      pdf_page: 183
    - "no": 8
      title: Sous-groupoïdes distingués ; quotients de groupoïdes
      page: 168
      pdf_page: 184
    - "no": 9
      title: Groupoïde des classes de chemins d’un graphe
      page: 171
      pdf_page: 187
    - "no": 10
      title: Groupoïdes libres
      page: 174
      pdf_page: 190
    - "no": 11
      title: Contraction de flèches d’un groupoïde
      page: 175
      pdf_page: 191
    - "no": 12
      title: Groupe de Poincaré d’un graphe
      page: 178
      pdf_page: 194
statements: 40
exercises: 12
content_sha256: 96af1a04d50c1790471b381947348bad0409e743d4fc9d933852f0e64557a832
translated_from: content/en-mt/ta/II/03_s3_groupoides.md
source_lang: en-mt
translation_method: machine
source_content_sha256: edbca22829fbf6d3252d8d0fe702290bb710700d90133cb8833f67e30b2d8f37
translation_model: gpt-5.4
translation_run: translate-vi-4c41275b
glossary_version: 34
glossary_terms_sha256: e849ca5dccbb3e75433573a5745df4aa151e54dd9c6be78020e46c5cde13327a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. GROUPOID

### 1. Phạm trù

#### Định nghĩa 1 {#ta-ii-s3-def-1 .statement tag=01SZ}

Cho C là một đồ thị có hướng. Ký hiệu J là tập hợp các cặp $(f, g)$ các mũi tên của C sao cho $t(f) =o(g)$. Một luật hợp thành trong C là một ánh xạ $m: J\rightarrow$ Fl(C) sao cho, với mọi cặp $(f, g)\in J$, gốc của mũi tên $m(f, g)$ là gốc của $f$ và đích của nó là đích của $g$.

Cho C là một đồ thị có hướng được trang bị một luật hợp thành $m$. Hai mũi tên $f$ và $g$ sao cho $t(f) =o(g)$ được gọi là hợp thành được; mũi tên $m(f, g)$ được gọi là hợp thành của chúng, hoặc tích của chúng, và thường được ký hiệu bởi $f\cdot g$, hoặc thậm chí bởi $f g$.

Với mỗi đỉnh $a$ của C, tập hợp $C_{a,a}$ = Fl$_{a,a}(C)$, được trang bị ánh xạ suy ra từ $m$ bằng cách chuyển qua các tập con, là một magma (A, I, p. 1, Def. 1).

Người ta nói rằng một họ $(f_i)_{i\in I}$ các mũi tên của C, được đánh chỉ số bởi một tập sắp thứ tự toàn phần hữu hạn khác rỗng I, là hợp thành được nếu, với mọi cặp $(i, j)$ các phần tử liên tiếp của I, các mũi tên $f_i$ và $f_j$ là hợp thành được. Tích $\prod_{i\in I}f_i$ của một họ như vậy được định nghĩa bằng quy nạp theo lực lượng của I theo cách sau (xem A, I, p. 3):

(i) nếu I chỉ có một phần tử $\omega ,\prod_{i\in I}f_i=f_{\omega}$;

(ii) nếu I có ít nhất hai phần tử và nếu $\omega$ là phần tử nhỏ nhất của I, đặt $\prod_{i\in I}f_i=f_{\omega}\cdot \prod_{i\in I-\{\omega\}}f_i$.

Luật hợp thành $m$ được gọi là kết hợp nếu ta có $f\cdot (g\cdot h) =$ $(f\cdot g)\cdot h$ với mọi bộ ba hợp thành được $(f, g, h)$ các mũi tên của C. Khi luật $m$ là kết hợp, tích của một dãy $(f_1, . . . , f_n)$ gồm $n$ mũi tên hợp thành được, trong đó $n$ là một số nguyên $\geqslant 1$, được ký hiệu bởi $f_1f_2. . . f_n$.

Cho $a$ là một đỉnh của C. Người ta nói rằng một mũi tên $e\in C_{a,a}$ là một phần tử đơn vị của $m$ tại $a$ nếu ta có $ef=f$ với mọi mũi tên $f$ có gốc là $a$ và $ge=g$ với mọi mũi tên $g$ có đích là $a$. Tồn tại nhiều nhất một phần tử đơn vị của $m$ tại $a:$ nếu $e$ và $e'$ là hai phần tử như vậy, thì ta có $e'=ee'=e$. Khi một phần tử đơn vị như vậy tồn tại, nó thường được ký hiệu bởi $e_a$; khi đó nó là một phần tử đơn vị của magma $C_{a,a}$ (A, I, p. 12).

#### Định nghĩa 2 {#ta-ii-s3-def-2 .statement tag=01T0}

Một phạm trù là một đồ thị có hướng được trang bị một luật hợp thành kết hợp mà tại mỗi đỉnh đều tồn tại một phần tử đơn vị.

#### Ví dụ 1 {#ta-ii-s3-n1-exa-1 .statement tag=01T1}

Cho C là một đồ thị có hướng. Ký hiệu Ch(C) là tập hợp các đường đi trong C và $o:$ Ch(C) $\rightarrow$ Som(C)$,t:$ Ch(C) $\rightarrow$ Som(C) là các ánh xạ gán cho một đường đi gốc và đích của nó. Bộ bốn $\Omega_C=$ (Som(C), Ch(C)$, o, t$) là một đồ thị có hướng. Trang bị cho nó luật hợp thành được định nghĩa bởi phép ghép liền các đường đi. Luật hợp thành này có tính kết hợp; với mọi đỉnh $a$ của C, vòng lặp hằng $e_a= (a)$ có gốc $a$ là một phần tử đơn vị tại $a$. Do đó, $\Omega_C$ là một phạm trù. Nó được gọi là phạm trù các đường đi của đồ thị có hướng C.

#### Ví dụ 2 {#ta-ii-s3-n1-exa-2 .statement tag=01T2}

Cho Σ là một Loài cấu trúc trong một lý thuyết $\mathscr{T}$ mạnh hơn lý thuyết tập hợp và $\sigma (x, y, s, u)$ là một số hạng của $\mathscr{T}$ thỏa mãn các điều kiện (MO$_I$), (MO$_{II}$) và (MO$_{III}$) của E, IV, p. 11. Cho S là một tập hợp; giả sử rằng mọi phần tử của S là một cặp $(x, s)$, trong đó $x$ là một tập hợp và $s$ là một cấu trúc thuộc loài Σ trên $x$. Gọi F là tập hợp các ánh xạ $f$ sao cho tồn tại $(x, s)$ và $(y, t)$ trong S để $f$ là một $\sigma$-cấu xạ từ $x$, được trang bị cấu trúc $s$, vào $y$, được trang bị cấu trúc $t$; khi đó đặt $o(f) = (x, s)$ và $t(f) = (y, t)$. Khi được trang bị luật hợp thành cho bởi $m(f, g) =g\circ f$, đồ thị có hướng $(S,F, o, t)$ là một phạm trù. Trong ngữ cảnh này, các phần tử của S đúng ra được gọi là các đối tượng.

Cho C là một phạm trù.

Với mọi đỉnh $a$ của C, tập hợp $C_{a,a}$, được trang bị luật hợp thành $(f, g)\mapsto f g$, là một monoid có phần tử đơn vị $e_a$.

Một ánh xạ $f$ của C được gọi là khả nghịch nếu tồn tại một ánh xạ $g$ của C sao cho $o(g) =t(f),t(g) =o(f)$ và sao cho $f g$ và $gf$ lần lượt là các phần tử đơn vị tại $o(f)$ và $t(f)$. Một ánh xạ như vậy $g$ là duy nhất (nếu $f g=e_{o(f)}$ và $g'f=e_{t(f)}$, ta có $g=e_{t(f)}g= (g'f)g=$ $g'(f g) =g'e_{o(f)}=g'$) và được gọi là nghịch đảo của $f$; nghịch đảo của một ánh xạ khả nghịch $f$ được ký hiệu là $f^{-1}$.

### 2. Hàm tử

#### Định nghĩa 3 {#ta-ii-s3-def-3 .statement tag=01T3}

Cho C và $C'$ là các phạm trù. Một hàm tử từ C vào $C'$ là một cấu xạ của các đồ thị có hướng $\varphi : C\rightarrow C'$ sao cho $\varphi (f g) =$ $\varphi (f)\varphi (g)$ với mọi cặp $(f, g)$ các ánh xạ hợp thành được của C.

Cho C và $C'$ là các phạm trù và cho $\varphi : C\rightarrow C'$ là một hàm tử. Cho $f$ là một mũi tên của C$,a$ là gốc của nó và $b$ là đích của nó; khi đó, $\varphi (f)$ là một mũi tên của $C'$ có gốc là $\varphi (a)$ và đích là $\varphi (b)$.

Cho C, $C',C''$ là các phạm trù và cho $\varphi : C\rightarrow C'$ và $\varphi ': C'\rightarrow C''$ là các hàm tử. Khi đó, $\varphi '\circ \varphi$ là một hàm tử.

Cho C là một phạm trù. Khi đó cấu xạ của đồ thị có hướng Id$_C$ là một hàm tử.

Cho $\varphi : C\rightarrow C'$ là một hàm tử. Để $\varphi$ là một đẳng cấu, điều kiện cần và đủ là các ánh xạ Som($\varphi$ ) và Fl($\varphi$ ) là song ánh.

Vì vậy, nếu người ta gọi một cấu trúc phạm trù trên các tập hợp S và F là dữ liệu của một cấu trúc đồ thị có hướng trên các tập hợp đó và của một luật hợp thành kết hợp mà tại mỗi đỉnh đều tồn tại một phần tử đơn vị, thì có thể lấy các hàm tử làm các cấu xạ của cấu trúc phạm trù (E, IV, p. 11).

### 3. Groupoid

#### Định nghĩa 4 {#ta-ii-s3-def-4 .statement tag=01T4}

Một groupoid là một phạm trù mà mọi mũi tên của nó đều khả nghịch.

Cho G là một groupoid và cho $a$ là một đỉnh của G. Monoid $G_{a,a}$ là một nhóm, ký hiệu bởi $G_a$ và được gọi là nhóm đẳng hướng của G tại $a$.

Cho $a,b$ là các đỉnh của G và cho $f\in G_{a,b}$ là một mũi tên nối $a$ với $b$. Ánh xạ $g\mapsto f gf^{-1}$ là một đẳng cấu nhóm từ $G_b$ lên $G_a$, ký hiệu là Int($f$). Nếu $f$ và $f'$ là các mũi tên hợp thành được của G, ta có Int($f f'$) $=$ Int($f$)$\circ$ Int($f'$) ; nghịch đảo của đẳng cấu Int($f$) là đẳng cấu Int($f^{-1}$).

Một cấu xạ của các groupoid $\varphi : G\rightarrow G'$ là một cấu xạ của các phạm trù. Hơn nữa, $\varphi$ là một đẳng cấu của các groupoid nếu và chỉ nếu nó là một đẳng cấu của các phạm trù.

Cho $\varphi : G\rightarrow G'$ là một cấu xạ của các groupoid. Với mọi đỉnh $a$ của G, ánh xạ $f\mapsto \varphi (f)$ từ $G_a$ vào $(G')_{\varphi(a)}$ là một đồng cấu nhóm, ký hiệu bởi $\varphi_a$. Đặc biệt, ta có $\varphi (e_a) =e_{\varphi(a)}$.

Với mọi mũi tên $f$ của G$,\varphi (f^{-1})$ là nghịch đảo của $\varphi (f)$. Nếu $f$ là một mũi tên của G nối một đỉnh $a$ với một đỉnh $b$, do đó ta có, với mọi phần tử $g\in G_b$, quan hệ Int($\varphi (f)$)$(\varphi (g)) =\varphi$(Int($f$)$(g)$).

### 4. Quỹ đạo của một groupoid

Cho G là một groupoid. Các thành phần liên thông của đồ thị có hướng nền của G được gọi là các quỹ đạo của G. Tập hợp các quỹ đạo của G được ký hiệu là Orb(G); nếu $\varphi : G\rightarrow G'$ là một cấu xạ của các groupoid, ánh xạ $\pi_0(\varphi )$ suy ra từ $\varphi$ bằng cách chuyển qua các thành phần liên thông của các đồ thị liên kết nói trên nói chung được ký hiệu là Orb($\varphi$ ) và được gọi là ánh xạ suy ra từ $\varphi$ bằng cách chuyển qua các quỹ đạo.

Một groupoid chỉ có đúng một quỹ đạo được gọi là bắc cầu. Nếu G là một groupoid bắc cầu, thì các nhóm $G_a$, với $a\in$ Som(G), là đẳng cấu. Người ta nói rằng groupoid G là đơn bắc cầu nếu nó là bắc cầu và hơn nữa, các nhóm đẳng hướng $G_a$ đều thu về phần tử đơn vị của chúng.

#### Mệnh đề 1 {#ta-ii-s3-prop-1 .statement tag=01T5}

Cho G là một groupoid. Quan hệ "tồn tại một mũi tên của G nối $a$ với $b$" là một quan hệ tương đương trên tập hợp các đỉnh của G mà các lớp tương đương là các quỹ đạo của G.

Cho $a,b,c$ là các đỉnh của G. Ta có $e_a\in G_{a,a}$; nếu $f\in G_{a,b}$, thì $f^{-1}\in G_{b,a}$; nếu $f\in G_{a,b}$ và $g\in G_{b,c}$, thì ta có $f g\in G_{a,c}$. Điều này cho thấy quan hệ đã nêu là phản xạ, đối xứng và bắc cầu; do đó nó là một quan hệ tương đương. Mệnh đề thứ hai khi đó suy ra từ định nghĩa các thành phần liên thông của một đồ thị có hướng.

### 5. Ví dụ về các groupoid

1) Cho G là một nhóm. Ký hiệu bởi $\mathscr{G}$ đồ thị có hướng mà tập hợp các đỉnh thu về một phần tử và tập hợp các mũi tên là G. Được trang bị luật hợp thành cảm sinh từ luật của G$,\mathscr{G}$ là một groupoid, gọi là groupoid liên kết với nhóm G.

2) Cho X là một tập hợp. Cho G là đồ thị có hướng $(X,X\times X$, pr$_1$, pr$_2)$; định nghĩa một luật hợp thành trên G bằng cách đặt $(x, x')\cdot (x', x'') = (x, x'')$, nếu $x, x', x''$ là các phần tử của X. Luật này là kết hợp; với mọi $x\in X$, $(x, x)$ là phần tử đơn vị tại $x$; nghịch đảo của mũi tên $(x, x')$ là mũi tên $(x', x)$. Groupoid được định nghĩa như vậy được gọi là groupoid các cặp của tập hợp X. Nếu X không rỗng, nó là đơn bắc cầu.

3) Cho X và S là các tập hợp và cho $p: X\rightarrow S$ là một ánh xạ. Với $a\in S$, đặt $X_a=\overset{-1}{p}(a)$. Với $a$ và $b$ trong S, đặt $G_{a,b}$ là tập hợp $\mathscr{B}(X_a; X_b)$ các song ánh từ $X_a$ lên $X_b$ và đặt G là tổng của các tập hợp $G_{a,b}$. Cho $o$ và $t$ là các ánh xạ từ G vào S sao cho $o(f) =a$ và $t(f) =b$ với mọi phần tử $f\in G_{a,b}$. Bộ bốn $(S,G, o, t)$ là một đồ thị có hướng. Trang bị cho nó luật hợp thành được định nghĩa bởi $m(f, g) =g\circ f$ nếu $f\in \mathscr{B}(X_a; X_b)$ và $g\in \mathscr{B}(X_b; X_c)$, trong đó $a, b, c$ là các điểm của S. Đó là một groupoid; nó được ký hiệu là $\mathscr{B}(X, p)$ và được gọi là groupoid các phép thế của X đối với $p$.

4) Cho $(G_i)_{i\in I}$ là một họ các vị nhóm. Ký hiệu G là tích đồ thị có hướng của họ các đồ thị có hướng nền; với mỗi $i\in I$, ký hiệu pr$_i: G\rightarrow G_i$ là cấu xạ đồ thị có hướng chính tắc. Tồn tại duy nhất một luật hợp thành trên G sao cho G là một vị nhóm và sao cho, với mỗi $i\in I$, pr$_i$ là một cấu xạ vị nhóm. Cho $f= (f_i)_{i\in I}$ và $g= (g_i)_{i\in I}$ là các mũi tên của G; chúng hợp thành được nếu và chỉ nếu các mũi tên $f_i$ và $g_i$ hợp thành được, với $i\in I$. Khi đó có $f g= (f_ig_i)_{i\in I}$.

Đồ thị có hướng G, được trang bị luật hợp thành này, được gọi là vị nhóm tích của họ $(G_i)_{i\in I}$. Nó thỏa mãn tính chất phổ quát sau: với mọi vị nhóm $G'$ và mọi họ $(\varphi_i)_{i\in I}$, trong đó $\varphi_i$ là một cấu xạ vị nhóm từ $G'$ vào $G_i$, tồn tại duy nhất một cấu xạ vị nhóm $\varphi : G'\rightarrow G$ sao cho $\varphi_i=$ pr$_i\circ \varphi$ với mỗi $i\in I$.

5) Cho $((G_i)_{i\in I},(\varphi_{i,j})_{i\prec j})$ là một hệ quy nạp các vị nhóm, được đánh chỉ số bởi một tập tiền thứ tự lọc phải $(I,\prec )$, các $\varphi_{i,j}$ là những cấu xạ vị nhóm. Cho G là đồ thị có hướng mà tập các đỉnh là lim$\longrightarrow_i$ Som(G$_i$), tập các mũi tên là lim$\longrightarrow_i$ Fl(G$_i$), các ánh xạ nguồn và đích lần lượt là các ánh xạ lim$\longrightarrow_io_{G_i}$ và lim$\longrightarrow_it_{G_i}$. Các luật hợp thành của các $G_i$ cảm sinh một luật hợp thành trên G làm cho nó thành một vị nhóm (xem A, I, p. 114). Các ánh xạ chính tắc Som(G$_i$)$\rightarrow$ Som(G) và Fl(G$_i$)$\rightarrow$ Fl(G) xác định một cấu xạ vị nhóm $\varphi_i$ từ $G_i$ vào G. Nếu $i,j$ là các phần tử của I sao cho $i\prec j$, thì có $\varphi_j\circ \varphi_{i,j}=\varphi_i$. Vị nhóm G được gọi là giới hạn quy nạp của họ các vị nhóm $G_i$ và được ký hiệu bởi lim$\longrightarrow_iG_i$. Nó thỏa mãn tính chất phổ quát sau: với mọi vị nhóm H và mọi họ $(\psi_i)_{i\in I}$, trong đó, với $i\in I,\psi_i: G_i\rightarrow H$ là một cấu xạ vị nhóm, sao cho $\psi_j\circ \varphi_{i,j}=\psi_i$ với mọi cặp $(i, j)$ các phần tử của I sao cho $i\prec j$, tồn tại duy nhất một cấu xạ vị nhóm $\psi : G\rightarrow H$ sao cho $\psi_i=\psi \circ \varphi_i$.

Về sự tồn tại của một vị nhóm thỏa mãn tính chất phổ quát này khi không giả sử rằng tập I là lọc phải, xem II, p. 228, exerc. 3.

### 6. Vị nhóm con

#### Định nghĩa 5 {#ta-ii-s3-def-5 .statement tag=01T6}

Cho C là một phạm trù. Một phạm trù con của C là một đồ thị có hướng con D của C thỏa mãn các điều kiện sau:

(i) Với mọi đỉnh $a$ của D$,e_a$ là một mũi tên của D;

(ii) Với mọi cặp hợp thành được $(f, g)$ các mũi tên của C thuộc D, tích $f g$ là một mũi tên của D;

Cho C là một phạm trù và cho D là một phạm trù con của D; được trang bị luật hợp thành suy ra từ luật hợp thành của C bằng cách chuyển qua các tập con, D là một phạm trù.

Mọi đồ thị có hướng con đầy đủ của C đều là một phạm trù con của C. Giao của một họ các phạm trù con của C là một phạm trù con của C.

#### Định nghĩa 6 {#ta-ii-s3-def-6 .statement tag=01T7}

Cho G là một vị nhóm. Một vị nhóm con của G là một phạm trù con H của G sao cho nghịch đảo của mọi mũi tên của G thuộc H là một mũi tên của H.

Cho G là một vị nhóm. Mọi vị nhóm con của G đều là một vị nhóm. Mọi đồ thị có hướng con đầy đủ của G đều là một vị nhóm con của G. Giao của một họ các vị nhóm con của G là một vị nhóm con của G.

Cho H là một đồ thị có hướng con của G. Giao của các vị nhóm con của G mà H là một đồ thị có hướng con được gọi là vị nhóm con của G sinh bởi H. Tập các đỉnh của nó bằng tập các đỉnh của H và các quỹ đạo của nó là các thành phần liên thông của H.

#### Ví dụ 1 {#ta-ii-s3-n6-exa-1 .statement tag=01T8}

Cho X là một tập hợp; ký hiệu bởi $X\times X$ vị nhóm các cặp của X (II, p. 163, Ví dụ 2). Cho R là một quan hệ tương đương trên X. Đồ thị có hướng con của vị nhóm $X\times X$ mà tập các đỉnh là X và tập các mũi tên là đồ thị của quan hệ tương đương R là một vị nhóm con của $X\times X$. Các quỹ đạo của nó là các lớp tương đương của quan hệ R.

Ngược lại, mọi vị nhóm con của $X\times X$ mà tập các đỉnh là X đều có dạng này.

Cho X và S là các tập hợp và cho $p: X\rightarrow$ S là một ánh xạ. Ánh xạ $p$ xác định một quan hệ tương đương trên X (E, II, p. 41). Người ta ký hiệu bởi $X\times_SX$ nhóm vị con của $X\times X$ được xác định bởi quan hệ tương đương này, và gọi nó là nhóm vị các cặp của $(X, p)$.

#### Ví dụ 2 {#ta-ii-s3-n6-exa-2 .statement tag=01T9}

Cho G và $G'$ là các nhóm vị, cho $\varphi$ và $\psi$ là các cấu xạ nhóm vị từ G vào $G'$. Bộ cân bằng của $\varphi$ và $\psi ($xem II, p. 153) là một nhóm vị con của G.

#### Ví dụ 3 {#ta-ii-s3-n6-exa-3 .statement tag=01TA}

Cho X là một tập hợp và Γ là một nhóm. Ký hiệu bởi $X\times \Gamma \times X$ đồ thị mà tập hợp các đỉnh là X, mà tập hợp các mũi tên là $X\times \Gamma \times X$, các ánh xạ đầu và cuối lần lượt là pr$_1$ và pr$_3$. Được trang bị luật hợp thành $(x, \gamma , x')\cdot (x', \gamma ', x'') = (x, \gamma \gamma ', x'')$, nó là một nhóm vị. Hơn nữa nó là nhóm vị suy ra bằng phép chuyển cấu trúc từ nhóm vị $(X\times X)\times \Gamma$, tích của nhóm vị các cặp $X\times X$ và của nhóm vị liên kết với nhóm Γ (II, p. 163, ví dụ 1), bằng song ánh $(x, x', \gamma )\mapsto (x, \gamma , x')$ từ $X\times X\times \Gamma$ lên $X\times \Gamma \times X$.

Cho $m: X\times \Gamma \rightarrow X$ là một phép toán phải của nhóm Γ trên X. Đồ thị F của ánh xạ $m$, nghĩa là tập hợp các bộ ba $(x, \gamma , x')\in X\times \Gamma \times X$ sao cho $x'=x\gamma$, là tập hợp các mũi tên của một nhóm vị con duy nhất G của $X\times \Gamma \times X$. Các quỹ đạo của nhóm vị này là các quỹ đạo của Γ trong X; nếu $x\in X$, thì nhóm đẳng hướng của G tại $x$ là tập hợp các $(x, \gamma , x)$, trong đó $\gamma$ chạy qua nhóm ổn định của $x$ trong Γ.

Ngược lại, mọi nhóm vị con G của nhóm vị $X\times \Gamma \times X$ sao cho ánh xạ (pr$_1$, pr$_2$) từ Fl(G) vào $X\times \Gamma$ là một song ánh đều có dạng ấy.

#### Ví dụ 4 {#ta-ii-s3-n6-exa-4 .statement tag=01TB}

Cho G là một nhóm vị, cho X là một tập hợp và cho $\varphi : X\rightarrow$ Som(G) là một ánh xạ. Định nghĩa một đồ thị $G'$ theo cách sau. Tập hợp Som(G$'$) là tập hợp X; với mọi cặp $(x, y)$ phần tử của X, tập hợp Fl$_{x,y}(G')$ là tập hợp các bộ ba $(x, f, y)\in X\times$ Fl(G) $\times X$, trong đó $f$ là một phần tử của Fl$_{\varphi(x),\varphi(y)}(G)$. Cho $x,y,z$ là các phần tử của X$,f\in$ Fl$_{\varphi(x),\varphi(y)}(G)$ và $g\in$ Fl$_{\varphi(y),\varphi(z)}(G)$ là các mũi tên của G, và đặt $(x, f, y)\cdot (y, g, z) = (x, f g, z)$. Điều này xác định một luật hợp thành trên đồ thị $G'$ khiến nó thành một nhóm vị. Nó được gọi là nhóm vị ảnh ngược của nhóm vị G bởi ánh xạ $\varphi$ và được ký hiệu bởi $\varphi^*(G)$.

Cặp $(\varphi , \psi )$, trong đó $\psi :$ Fl($\varphi^*(G)$)$\rightarrow$ Fl(G) là ánh xạ được xác định bởi $(x, f, y)\mapsto f$ là một cấu xạ nhóm vị từ $\varphi^*(G)$ vào G, được gọi là cấu xạ chính tắc.

#### Ví dụ 5 {#ta-ii-s3-n6-exa-5 .statement tag=01TC}

Cho $\varphi : G\rightarrow G'$ là một cấu xạ groupoid. Gọi H là đồ thị có hướng con của G có tập đỉnh là Som(G) và có tập mũi tên gồm các $f\in$ Fl(G) sao cho $\varphi (f)$ là một phần tử đơn vị của $G'$. Với mọi $a\in$ Som(G)$,e_a\in H_{a,a}$. Với mọi $f\in$ Fl(H), $\varphi (f^{-1}) =\varphi (f)^{-1}$, do đó $f^{-1}\in$ Fl(H). Hơn nữa, nếu $f$ và $g$ là các mũi tên ghép được của H, ta có $\varphi (f g) =\varphi (f)\varphi (g) =e_{t(\varphi(f))}e_{o(\varphi(g))}=$ $e_{t(\varphi(f))}$, do đó $f g$ là một mũi tên của H. Điều này cho thấy H là một groupoid con của G. Nó được gọi là hạt nhân của $\varphi$ và được ký hiệu là Ker($\varphi$ ).

#### Ví dụ 6 {#ta-ii-s3-n6-exa-6 .statement tag=01TD}

Cho $\varphi : G\rightarrow G'$ là một cấu xạ groupoid. Đồ thị có hướng $\varphi (G)$ có tập đỉnh là $\varphi$(Som(G)) và có tập mũi tên là $\varphi$(Fl(G)) nói chung không phải là một groupoid con của $G'$. Tuy vậy, điều này vẫn đúng nếu ánh xạ Som($\varphi$ ) là đơn ánh (II, p. 225, exerc. 5).

### 7. Các phép toán của một groupoid

Cho G là một groupoid; gọi S là tập đỉnh của nó. Cho X là một tập hợp và cho $p: X\rightarrow S$ là một ánh xạ. Một phép toán (phải) $\varphi$ của groupoid G trên tập hợp X, đối với $p$, là một cấu xạ groupoid $\varphi$ từ G vào groupoid $\mathscr{B}(X, p)$ các hoán vị của tập hợp X đối với $p($II, p. 163) cảm sinh đồng nhất trên tập đỉnh. Nói cách khác, $\varphi$ gồm, với mỗi cặp $(a, b)$ điểm của S và với mỗi mũi tên $g\in G$ nối $a$ với $b$, một ánh xạ $\varphi (g): X_a\rightarrow X_b$, sao cho, với mọi cặp $(f, g)$ mũi tên ghép được của G,

$$
\varphi (f g) =\varphi (g)\circ \varphi (f)
$$

và sao cho, với mọi $a\in S,\varphi (e_a)$ là đồng nhất của $X_a$.

Cho $\varphi$ và $\varphi '$ là các phép toán của groupoid G trên một tập hợp X, đối với một ánh xạ $p: X\rightarrow S$. Để có $\varphi =\varphi '$, chỉ cần tồn tại một đồ thị có hướng con H của G, sinh ra G, sao cho $\varphi (f) =\varphi '(f)$ với mọi $f\in$ Fl(H). Thật vậy, tập các mũi tên $f$ của G sao cho $\varphi (f) =\varphi '(f)$ là tập các mũi tên của một groupoid con của G, có tập đỉnh là S.

Cho G là một groupoid có tập đỉnh là S, cho X là một tập hợp, cho $p: X\rightarrow S$ là một ánh xạ, và cho $\varphi$ là một phép toán của G trên X đối với $p$. Gọi $G_{\varphi}$ là đồ thị có hướng con của $p^*(G)$ có tập đỉnh là X và có tập mũi tên là tập các bộ ba $(x, f, y)\in X\times$ Fl(G) $\times X$ sao cho $\varphi (f)(x) =y$. Nó là một groupoid con của $p^*(G)$.

Ngược lại, cho Γ là một nhóm vị con của $p^*(G)$; giả sử rằng ánh xạ $(x, f, y)\mapsto (x, f)$ từ Fl(Γ) vào $X\times$ Fl(G) là đơn ánh và ảnh của nó là tập hợp các cặp $(x, f)$ sao cho $p(x) =o(f)$. Khi đó tồn tại một phép toán duy nhất $\varphi$ của nhóm vị G trên X sao cho $\Gamma  = G_{\varphi}$.

Các quỹ đạo của nhóm vị $G_{\varphi}$ được gọi là các quỹ đạo của phép toán của G trên X. Theo định nghĩa, chúng là các lớp tương đương của quan hệ trong X được xác định bởi $R\{x, y\}$ khi và chỉ khi tồn tại $f\in$ Fl(G) sao cho $\varphi (f)(x) =y$.

#### Ví dụ 1 {#ta-ii-s3-n7-exa-1 .statement tag=01TE}

Cho G là một nhóm, và cho $\mathscr{G}$ là nhóm vị liên kết với G (II, p. 163, Ví dụ 1). Nếu X là một tập hợp, một phép toán (ở phải) của nhóm vị $\mathscr{G}$ trên X không là gì khác hơn một phép toán (ở phải) của nhóm G trên X. Hơn nữa, các quỹ đạo của phép toán của $\mathscr{G}$ trùng nhau với các quỹ đạo của nhóm G.

#### Ví dụ 2 {#ta-ii-s3-n7-exa-2 .statement tag=01TF}

Cho $G = (S,F, o, t)$ là một nhóm vị. Tồn tại một phép toán duy nhất của G trên tập hợp S, tương đối với Id$_S$. Nó được cho bởi $\varphi (f)(a) =b$ nếu $f\in G_{a,b}$. Các quỹ đạo đối với phép toán này là các quỹ đạo của G theo nghĩa đã định nghĩa ở p. 162.

Cho G là một nhóm vị, cho S là tập hợp các đỉnh của nó, cho X là một tập hợp, và cho $p: X\rightarrow S$ là một ánh xạ. Cho $\varphi$ là một phép toán của G trên X tương đối với $p$. Người ta nói rằng nhóm vị G tác động không có đơn trị trên X nếu, với mọi điểm $a\in S$ và mọi phần tử $f\in G_a,\varphi (f)$ là đồng nhất của $X_a$. Nếu nhóm vị G là bắc cầu, chỉ cần điều này đúng đối với một điểm của S.

Cho $a$ là một điểm của S và giả sử rằng ta có $\varphi (f) =$ Id$_{X_a}$ với mọi $f\in G_a$. Cho $b$ là một điểm của S thuộc quỹ đạo của $a$ và cho $g$ là một mũi tên của G nối $a$ với $b$. Với mọi $f\in G_b$, Int($g$)$(f) =gf g^{-1}$ là một phần tử của $G_a$; do đó ta có Id$_{X_a}=\varphi (gf g^{-1}) =\varphi (g)\varphi (f)\varphi (g)^{-1}$, nên $\varphi (f) =$ Id$_{X_b}$. Cho $b$ là một điểm của S thuộc quỹ đạo của $a$ và cho $g,g'$ là các mũi tên của G nối $a$ với $b$; khi đó $g'g^{-1}$ là một vòng tại $a$, do đó $\varphi (g'g^{-1}) =$ Id$_{X_a}$ và $\varphi (g) =\varphi (g')$.

### 8. Nhóm Vị Chuẩn Tắc; Nhóm Vị Thương

#### Định nghĩa 7 {#ta-ii-s3-def-7 .statement tag=01TG}

Cho G là một nhóm vị. Người ta nói rằng một nhóm vị con H của G là chuẩn tắc nếu Som(H) = Som(G) và nếu với mọi cặp $(a, b)$ đỉnh của H và mọi mũi tên $f\in G_{a,b}$, ta có Int($f$)$(H_b) = H_a$.

Cho G là một phân thớ và cho H là một phân thớ con của G mà tập các đỉnh bằng Som(G). Để kiểm tra rằng H là bất biến, chỉ cần chứng minh rằng $fH_bf^{-1}\subset H_a$ với mọi $a\in$ Som(G), mọi $b\in$ Som(G) và mọi $f\in G_{a,b}$. Thật vậy, nếu như vậy thì cũng có $f^{-1}H_af\subset H_b$ với mọi mũi tên $f\in G_{b,a}$, nghĩa là, $H_a\subset fH_bf^{-1}$, và do đó $fH_bf^{-1}= H_a$.

Cho G là một phân thớ và cho H là một phân thớ con bất biến của G. Với mọi đỉnh $a$ của G, nhóm con $H_a$ của $G_a$ là một nhóm con bất biến của $G_a$.

Cho $\varphi : G\rightarrow G'$ là một cấu xạ các phân thớ. Hạt nhân của $\varphi ($II, p. 166, ví dụ 5) là một phân thớ con bất biến của G. Thật vậy, cho $f$ là một mũi tên trong G nối $a$ với $b$ và cho $g\in$ Ker($\varphi$ )$_b$; khi đó ta có $\varphi (f gf^{-1}) =\varphi (f)\varphi (g)\varphi (f^{-1}) =\varphi (f)e_{\varphi(b)}\varphi (f)^{-1}=e_{\varphi(a)}$, do đó có bao hàm thức $f$Ker($\varphi$ )$_bf^{-1}\subset$ Ker($\varphi$ )$_a$.

Cho G là một phân thớ. Phân thớ G và phân thớ con của G mà tập các mũi tên là tập các phần tử đơn vị của G là những phân thớ con bất biến của G. Giao của một họ các phân thớ con bất biến của G là một phân thớ con bất biến của G. Đặc biệt, với mọi tập con $F\subset$ Fl(G), tồn tại một phân thớ con bất biến nhỏ nhất của G mà tập các mũi tên chứa F. Nó được gọi là phân thớ con bất biến sinh bởi F.

Cho H là một phân thớ con bất biến của G. Cho $\mathscr{R}$ là quan hệ tương đương trong Fl(G) được xác định bởi $\mathscr{R}\{f, g\}$ khi và chỉ khi tồn tại các mũi tên $x$ và $y$ trong Fl(H) sao cho $f=xgy$. Nếu $f$ và $g$ là các mũi tên của G tương đương theo môđun $\mathscr{R}$, thì các gốc của chúng (resp. các ngọn của chúng) thuộc cùng một quỹ đạo của H. Đặt $F'=$ Fl(G)$/\mathscr{R}$ và ký hiệu bởi $o'$ và $t'$ các ánh xạ từ $F'$ vào Orb(H) suy ra từ $o$ và $t$ bằng cách chuyển qua các thương. Ký hiệu bởi $G/H$ đồ thị có hướng (Orb(H)$,F', o', t'$).

#### Bổ đề {#ta-ii-s3-n8-lem-1 .statement tag=01TH}

Cho $u$ và $v$ là các mũi tên hợp thành được của $G/H$, ta có thể chọn các đại diện $f$ và $g$ của $u$ và $v$ trong Fl(G) sao cho chúng hợp thành được. Lớp theo môđun $\mathscr{R}$ của tích $f g$ không phụ thuộc vào việc lựa chọn $f$ và $g$.

Cho $f$ và $g$ là các đại diện tùy ý của $u$ và $v$ trong Fl(G). Đầu cuối của $f$ và gốc của $g$ thuộc cùng một quỹ đạo của H, do đó có thể được nối bởi một mũi tên $x$ của H (II, p. 162, prop. 1). Khi đó các mũi tên $f x$ và $g$ là các đại diện của $u$ và $v$ trong F mà ghép được trong G. Điều này chứng minh mệnh đề thứ nhất.

Bây giờ giả sử một mặt, $f,g$, và mặt khác, $f',g'$, là các đại diện của $u$ và $v$ mà ghép được trong G. Theo giả thiết, tồn tại các mũi tên $x,y,z,t$ trong H sao cho ta có $f'=xf y$ và $g'=zgt$. Khi đó ta có $yz\in H_{t(f)}$ và $f'g'=xf yzgt=xf(yz)f^{-1}f gt$. Vì H là một phân nhóm vị chuẩn tắc của G, mũi tên $f(yz)f^{-1}$ là một mũi tên của H. Do đó mũi tên $xf(yz)f^{-1}$ cũng vậy, điều này chứng minh rằng $f'g'$ và $f g$ là tương đương theo môđun $\mathscr{R}$.

Nhờ bổ đề này, tồn tại một luật hợp thành duy nhất $m$ trên đồ thị có hướng $G/H$ sao cho, với mọi cặp $(u, v)$ các mũi tên ghép được, $m(u, v)$ là lớp theo môđun $\mathscr{R}$ của tích $f g$, đối với mọi cặp $(f, g)$ các mũi tên ghép được của G sao cho $u$ là lớp của $f$ và $v$ là lớp của $g$. Được trang bị luật hợp thành này, $G/H$ là một nhóm vị. Gọi $p_1:$ Som(G) $\rightarrow$ Som(G$/H$) và $p_2:$ Fl(G) $\rightarrow$ Fl(G$/H$) là các toàn ánh chính tắc. Cặp $p= (p_1, p_2)$ là một cấu xạ nhóm vị từ G vào $G/H$ mà hạt nhân là phân nhóm vị chuẩn tắc H.

#### Định nghĩa 8 {#ta-ii-s3-def-8 .statement tag=01TI}

Người ta nói rằng $G/H$ là nhóm vị thương của G theo H và rằng $p: G\rightarrow G/H$ là cấu xạ chính tắc.

#### Nhận xét 1 {#ta-ii-s3-n8-rem-1 .statement tag=01TJ}

Ánh xạ Som($p$) xác định, khi chuyển qua các thương, một song ánh từ tập hợp các quỹ đạo của G lên tập hợp các quỹ đạo của $G/H$. Đặc biệt, G là bắc cầu khi và chỉ khi $G/H$ là bắc cầu.

#### Nhận xét 2 {#ta-ii-s3-n8-rem-2 .statement tag=01TK}

Cho $a$ và $b$ là các đỉnh của G. Ánh xạ từ $G_{a,b}$ vào $(G/H)_{p(a),p(b)}$ suy ra từ $p$ là toàn ánh. Thật vậy, giả sử $u$ là một mũi tên của $G/H$ nối $p(a)$ với $p(b)$; nó là lớp modulo $\mathscr{R}$ của một mũi tên $f$ của G. Gốc $o(f)$ của $f$ thuộc quỹ đạo của $a$ trong H; do đó tồn tại một mũi tên $x$ trong H nối $a$ với $o(f)$. Tương tự, tồn tại một mũi tên $y$ trong H nối $t(f)$ với $b$. Khi đó $f'=xf y$ là một phần tử của $G_{a,b}$ mà lớp modulo $\mathscr{R}$ của nó là $u$.

#### Mệnh đề 2 {#ta-ii-s3-prop-2 .statement tag=01TL}

Cho $a$ là một đỉnh của G. Đồng cấu nhóm $p_a: G_a\rightarrow (G/H)_{p(a)}$ suy ra từ $p$ bằng cách chuyển qua các nhóm đẳng hướng là toàn ánh; hạt nhân của nó là $H_a$.

Đồng cấu $p_a$ là toàn ánh theo nhận xét trước. Hạt nhân của nó chứa $H_a$ theo phép dựng của groupoid $G/H$. Cho $f$ là một phần tử của $G_a$ sao cho $p_a(f) =e_{p(a)}$. Điều đó có nghĩa là $f$ và $e_a$ tương đương modulo $\mathscr{R}$; khi đó tồn tại các mũi tên $x$ và $y$ của H sao cho $f=xe_ay$. Tất yếu, $x$ và $y$ thuộc $H_a$, do đó $f\in H_a$.

#### Mệnh đề 3 {#ta-ii-s3-prop-3 .statement tag=01TM}

Cho G là một groupoid, cho H là một groupoid con phân biệt của G và cho $p: G\rightarrow G/H$ là cấu xạ chính tắc. Cho $\varphi : G\rightarrow G'$ là một cấu xạ groupoid sao cho $H\subset$ Ker($\varphi$ ). Tồn tại một cấu xạ groupoid duy nhất $\overline{\varphi}: G/H\rightarrow G'$ sao cho $\overline{\varphi}\circ p=\varphi$.

Người ta nói rằng $\overline{\varphi}$ là cấu xạ groupoid suy ra từ $\varphi$ bằng cách chuyển qua thương.

Tính duy nhất của một cấu xạ như thế là hiển nhiên, vì các ánh xạ Som($p$) và Fl($p$) là toàn ánh.

Cho $a$ và $b$ là các đỉnh của G. Nếu chúng thuộc cùng một quỹ đạo của H, thì tồn tại một mũi tên $f$ nối $a$ với $b$ trong H, và ta có $\varphi (f) =e_{\varphi(a)}$. Đặc biệt, $\varphi (a) =\varphi (b)$. Do đó, ánh xạ Som($\varphi$ ) xác định, bằng cách chuyển qua thương, một ánh xạ $\overline{\varphi}_1:$ Orb(H) $\rightarrow$ Som(G$'$). Cho $f$ và $g$ là các mũi tên trong G. Nếu $f$ và $g$ là tương đương modulo $\mathscr{R}$, thì tồn tại các mũi tên $x$ và $y$ trong H sao cho $f$ = $xgy$. Do đó, $\varphi (f) =\varphi (x)\varphi (g)\varphi (y) =\varphi (g)$ vì $\varphi (x)$ và $\varphi (y)$ là các phần tử đơn vị. Bởi vậy, ánh xạ Fl($\varphi$ ) xác định, bằng cách chuyển qua thương, một ánh xạ $\overline{\varphi}_2:$ Fl(G)$/\mathscr{R}\rightarrow$ Fl(G$'$).

Cho $f$ và $g$ là các mũi tên khả hợp của G; ký hiệu bởi $u$ và $v$ các lớp của chúng trong Fl(G$/H$). Ta có $\overline{\varphi}_2(uv) =\varphi (f g) =\varphi (f)\varphi (g) =$ $\overline{\varphi}_2(u)\overline{\varphi}_2(v)$.

Cặp $\overline{\varphi}= (\overline{\varphi}_1, \varphi_2)$ là một cấu xạ groupoid từ $G/H$ vào $G'$ và ta có $\overline{\varphi}\circ p=\varphi$.

### 9. Groupoid các lớp đường đi của một đồ thị

Cho G là một đồ thị. Ký hiệu bởi $\Omega_G$ phạm trù các đường đi của quiver nền của G (II, p. 160, ví dụ 1). Xét quan hệ tương đương tinh nhất $\mathscr{R}$ trên Ch(G) sao cho ta có:

(i) Với mọi cặp $(a, b)$ đỉnh của G và mọi mũi tên $f$ trong G nối $a$ với $b$, các đường đi $(a, f, b,\overline{f}, a)$ và $e_a$ là tương đương modulo $\mathscr{R}$;

(ii) Nếu $(c, d)$ và $(c', d')$ là các cặp đường đi kề nhau trong G sao cho $\mathscr{R}\{c, c'\}$ và $\mathscr{R}\{d, d'\}$, thì các đường đi $c*d$ và $c'*d'$ là tương đương modulo $\mathscr{R}$.

Hai đường đi tương đương modulo $\mathscr{R}$ có cùng gốc và cùng ngọn. Các ánh xạ $o$ và $t$ từ Ch(G) vào Som(G) xác định, khi chuyển qua thương, các ánh xạ $o'$ và $t'$ từ Ch(G)$/\mathscr{R}$ vào Som(G). Ta ký hiệu bởi $\varpi_G$ quiver (Som(G), Ch(G)$/\mathscr{R}, o', t'$). Cặp $\varphi$ gồm ánh xạ đồng nhất của Som(G) và phép chiếu chính tắc của Ch(G) lên Ch(G)$/\mathscr{R}$ là một cấu xạ của các quiver từ $\Omega_G$ vào $\varpi_G$. Phép ghép các đường đi trong Ch(G) xác định, khi chuyển qua các thương, một luật hợp thành trong $\varpi_G$.

#### Mệnh đề 4 {#ta-ii-s3-prop-4 .statement tag=01TN}

Được trang bị luật hợp thành này, $\varpi_G$ là một groupoid.

Theo phép dựng, ta có quan hệ $\varphi (cc') =\varphi (c)\varphi (c')$, với mọi cặp đường đi ghép được $(c, c')$ trong G. Mọi mũi tên của $\varpi_G$ đều có dạng $\varphi (c)$, trong đó $c$ là một đường đi trong G. Suy ra luật hợp thành của $\varpi_G$ là kết hợp và $\varphi (e_a)$ là một phần tử đơn vị tại $a$, với mọi đỉnh $a$ của $\varpi_G$. Còn phải chứng minh rằng mọi mũi tên của $\varpi_G$ đều khả nghịch. Cho $c$ là một đường đi trong G, và chứng minh bằng quy nạp theo độ dài của $c$ rằng ta có $\varphi (c)\varphi (\overline{c}) =\varphi (e_{o(c)})$. Đẳng thức này đúng nếu $c$ có độ dài 0. Nếu $c$ có độ dài $n\geqslant 1$, ta có thể viết $c=c_1c_2$, với $c_1$ có độ dài 1 và $c_2$ có độ dài $n-1$. Khi đó, $\overline{c}=\overline{c_2}\overline{c_1}$ và ta có

$$
\varphi (c)\varphi (\overline{c}) =\varphi (c_1)\varphi (c_2)\varphi (\overline{c_2})\varphi (\overline{c_1}) =\varphi (c_1)\varphi (e_{o(c_2)})\varphi (\overline{c_1}) =\varphi (c_1)\varphi (\overline{c_1})
$$

$$
=\varphi (c_1\overline{c_1}) =\varphi (e_{o(c_1)})
$$

theo định nghĩa của quan hệ $\mathscr{R}$.

Áp dụng đẳng thức này cho đường đi $\overline{c}$, ta thấy rằng $\varphi (\overline{c})\varphi (c) =$ $\varphi (e_{t(c)})$. Vậy $\varphi (c)$ là khả nghịch, với nghịch đảo là $\varphi (\overline{c})$.

Các lớp tương đương của quan hệ $\mathscr{R}$ được gọi là các lớp đường đi trong đồ thị G; groupoid $\varpi_G$ được gọi là groupoid các lớp đường đi của đồ thị G. Nó có cùng tập hợp đỉnh như G, và các quỹ đạo của nó là các thành phần liên thông của đồ thị G.

Ta ký hiệu bởi $v$ ánh xạ gắn với một mũi tên $f$ của G lớp của đường đi $(o(f), f, t(f))$ của G. Cặp $j$ = (Id$_{Som(G)}, v$) là một cấu xạ, gọi là chính tắc, của các quiver từ G vào $\varpi_G$. Ảnh của nó sinh ra $\varpi_G$; với mọi mũi tên $f$ của G, ta có $j(\overline{f}) =j(f)^{-1}$.

Cho G và $G'$ là các đồ thị, và $\varphi : G\rightarrow G'$ là một cấu xạ đồ thị. Ký hiệu bởi $j: G\rightarrow \varpi_G$ và $j': G'\rightarrow \varpi_{G'}$ các cấu xạ chính tắc. Nếu $c= (a_0, f_1, a_1, . . . , a_n)$ là một đường đi trong G, thì lớp của đường đi $\varphi (c) = (\varphi (a_0), \varphi (f_1), \varphi (a_1), . . . , \varphi (a_n))$ chỉ phụ thuộc vào lớp của $c$. Do đó, bằng cách chuyển qua các lớp tương đương, ta định nghĩa được một cấu xạ quiver $\varpi (\varphi ):\varpi_G\rightarrow \varpi_{G'}$ sao cho $\varpi (\varphi )\circ j=j'\circ \varphi$. Đó là một cấu xạ groupoid.

#### Mệnh đề 5 {#ta-ii-s3-prop-5 .statement tag=01TO}

Cho G là một đồ thị; ký hiệu bởi $j$ cấu xạ quiver chính tắc của G vào $\varpi_G$. Cho $\varphi$ là một cấu xạ quiver từ G vào một groupoid $G'$ sao cho $\varphi (\overline{f}) =\varphi (f)^{-1}$ với mọi mũi tên $f$ của G. Khi đó tồn tại một cấu xạ groupoid duy nhất $\varphi '$ từ $\varpi_G$ vào $G'$ sao cho $\varphi '\circ j=\varphi$.

Ta định nghĩa một ánh xạ $u:$ Ch(G) $\rightarrow$ Fl(G$'$) bằng cách đặt, với mọi đường đi $c= (a_0, f_1, a_1, . . . , f_n, a_n)$ trong G$,u(c) =e_{a_0}\varphi (f_1). . . \varphi (f_n)$. Với mọi cặp $(c, c')$ các đường đi hợp thành được trong G, ta có $u(cc') =$ $u(c)u(c')$. Ánh xạ $u$ tương thích với quan hệ tương đương $\mathscr{R}$ đã được định nghĩa ở trên, do đó, bằng cách chuyển qua thương, ta được một ánh xạ $u':$ Ch(G)$/\mathscr{R}\rightarrow$ Fl(G$'$). Khi đó đặt $\varphi '=$ (Som($\varphi$ )$, u'$). Đó là một cấu xạ groupoid từ $\varpi_G$ vào $G'$ sao cho $\varphi '\circ j=\varphi$.

Cho $\psi$ là một cấu xạ groupoid từ $\varpi_G$ vào $G'$ sao cho $\psi \circ j=\varphi$. Bộ đẳng hóa của $\varphi '$ và $\psi$ là một groupoid con của $\varpi_G$ chứa $j(G)$. Vậy nó bằng $\varpi_G$, vì $\varpi_G$ được sinh bởi $j(G)$, và ta có $\psi =\varphi '$.

#### Hệ quả 1 {#ta-ii-s3-prop-5-cor-1 .statement tag=01TP}

Trong một đồ thị, mỗi lớp đường đi chứa một đường đi duy nhất không quay lui.

Cho G là một đồ thị. Ký hiệu bởi $j: G\rightarrow \varpi_G$ cấu xạ quiver chính tắc.

Sự tồn tại, với mọi đường đi $c$ của G, của một đường đi tương đương không quay lui là ngay lập tức theo quy nạp trên độ dài của $c$ (xem II, p. 157).

Cho A là một định hướng của G và gọi $G'$ là nhóm vị liên kết với nhóm tự do F(A) được xây dựng trên A (II, p. 163, Ví dụ 1). Gọi $\psi$ là cấu xạ của các quiver từ G vào $G'$ sao cho, với mọi $f\in A,\psi (f)$ là phần tử $f$ của F(A) và $\psi (\overline{f})$ là phần tử $f^{-1}$ của F(A). Gọi $\psi '$ là cấu xạ duy nhất của các nhóm vị từ $\varpi_G$ vào $G'$ sao cho $\psi '\circ j=\psi$.

Gọi $c,c'$ là các đường đi không quay lui tương đương modulo $\mathscr{R}$. Chúng có cùng gốc và cùng ngọn. Để chứng minh rằng chúng bằng nhau, chỉ cần chứng minh rằng các dãy $(f_1, . . . , f_n)$ và $(g_1, . . . , g_m)$ các cạnh của chúng bằng nhau. Ảnh qua $\psi '$ của lớp chung của $c$ và $c'$ bằng $\psi (f_1). . . \psi (f_n)$ và bằng $\psi (g_1). . . \psi (g_m)$. Bây giờ các hạng của các dãy $(\psi (f_1), . . . , \psi (f_n))$ và $(\psi (g_1), . . . , \psi (g_m))$ thuộc tập con $A\cup A^{-1}$ của F(A) và hai phần tử liên tiếp của các dãy này không là nghịch đảo của nhau. Theo A, I, p. 84, Mệnh đề 7, hai dãy này bằng nhau. Suy ra các dãy $(f_1, . . . , f_n)$ và $(g_1, . . . , g_m)$ bằng nhau, và do đó $c=c'$, từ đó có tính duy nhất.

#### Hệ quả 2 {#ta-ii-s3-prop-5-cor-2 .statement tag=01TQ}

Cấu xạ chính tắc từ G vào $\varpi_G$ là đơn ánh.

Điều này suy ra ngay lập tức từ Hệ quả 1.

#### Hệ quả 3 {#ta-ii-s3-prop-5-cor-3 .statement tag=01TR}

Cho $G'$ là một đồ thị con của G. Cấu xạ từ $\varpi_{G'}$ vào $\varpi_G$ suy ra từ đơn ánh của $G'$ vào G là đơn ánh.

Ký hiệu bởi $i$ cấu xạ bao hàm của $G'$ vào G và bởi $\varpi (i)$ cấu xạ từ $\varpi_{G'}$ vào $\varpi_G$ suy ra từ nó. Các ánh xạ Som($i$) và Som($\varpi (i)$) trùng nhau. Hơn nữa, nếu $c$ là một đường đi không quay lui trong $G'$, thì đường đi $i(c)$ là một đường đi không quay lui trong G. Do đó mệnh đề được suy ra từ Hệ quả 1.

#### Hệ quả 4 {#ta-ii-s3-prop-5-cor-4 .statement tag=01TS}

Một đồ thị khác rỗng G là một cây nếu và chỉ nếu nhóm vị $\varpi_G$ là đơn bắc cầu.

Cho $a$ là một điểm của G. Theo Hệ quả 1, các tính chất sau là tương đương:

(i) Nhóm đẳng hướng của $\varpi_G$ tại $a$ thu về phần tử đơn vị;

(ii) Chu trình duy nhất trong G có gốc $a$ mà không quay lui là chu trình hằng có gốc $a$.

Nhóm vị $\varpi_G$ là đơn bắc cầu nếu và chỉ nếu nó bắc cầu và có tính chất (i) với mọi $a$. Đồ thị G là một cây nếu và chỉ nếu nó liên thông và có tính chất (ii) với mọi điểm $a$. Vì các quỹ đạo của $\varpi_G$ được đồng nhất với các thành phần liên thông của G, hệ quả được chứng minh.

### 10. Nhóm vị tự do

#### Định nghĩa 9 {#ta-ii-s3-def-9 .statement tag=01TT}

Cho C là một quiver. Nhóm vị $\varpi_{\widetilde{C}}$ của các lớp đường đi của đồ thị $\widetilde{C}$ liên kết với C được gọi là nhóm vị tự do được xây dựng trên C, và được ký hiệu bởi Grp(C).

Tập hợp các đỉnh của Grp(C) bằng tập hợp các đỉnh của C; các quỹ đạo của Grp(C) là các thành phần liên thông của C.

Cho C là một quiver khác rỗng. Theo Hệ quả 4, p. 174, đồ thị $\widetilde{C}$ liên kết với C là một cây nếu và chỉ nếu nhóm vị tự do Grp(C) được xây dựng trên C là đơn bắc cầu.

Hợp thành của các cấu xạ đồ thị có hướng chính tắc $i: C\rightarrow \widetilde{C}$ và $j:\widetilde{C}\rightarrow \varpi_C$ là một cấu xạ đồ thị có hướng từ C vào Grp(C), được gọi là cấu xạ chính tắc của C vào Grp(C). Ký hiệu nó là $\theta$. Với mọi đỉnh $a$ của C, ta có $\theta (a) =a$. Nếu $f$ là một mũi tên của C$,\theta (f)$ là lớp của đường đi $(o(f),(f,1), t(f))$ của $\widetilde{C}$. Cấu xạ $\theta$ là đơn ánh (II, p. 174, Hệ quả 2) và ảnh của nó sinh groupoid Grp(C).

Cho $\varphi : C\rightarrow C'$ là một cấu xạ đồ thị có hướng. Ký hiệu bởi $\theta_C$ (tương ứng $\theta_{C'}$) cấu xạ chính tắc của C vào Grp(C) (tương ứng của $C'$ vào Grp(C$'$)). Cấu xạ $\varpi (\widetilde{\varphi})$ là cấu xạ groupoid duy nhất $\psi$ từ Grp(C) vào Grp(C$'$) sao cho $\psi \circ \theta_C=\theta_{C'}\circ \varphi$.

#### Mệnh đề 6 {#ta-ii-s3-prop-6 .statement tag=01TU}

Cho C là một đồ thị có hướng, G là một groupoid, và $\varphi$ là một cấu xạ đồ thị có hướng từ C vào G. Tồn tại một cấu xạ groupoid duy nhất $\varphi '$ từ Grp(C) vào G sao cho $\varphi '\circ \theta_C=\varphi$.

Cho $\psi$ là cấu xạ đồ thị có hướng từ $\widetilde{C}$ vào G sao cho $\psi (a) =\varphi (a)$ với mọi đỉnh $a$ của C và $\psi (f, \varepsilon ) =\varphi (f)^{\varepsilon}$ với mọi mũi tên $f$ của C và mọi $\varepsilon \in  \{-1,1\}$. Ta có $\psi \circ i=\varphi$. Theo Mệnh đề 5, p. 173, tồn tại một cấu xạ $\varphi '$ từ Grp(C) $=\varpi_C$ vào G sao cho $\varphi '\circ j=\psi$. Khi đó ta có $\varphi '\circ \theta_C=\varphi '\circ j\circ i=\psi \circ i\widetilde{=}\varphi$. Như trong chứng minh của Mệnh đề 5, tính duy nhất của $\varphi '$ suy ra từ việc $\theta_C(C)$ sinh groupoid Grp(C).

Trong các giả thiết của Mệnh đề 6, đôi khi người ta nói rằng $\varphi '$ là cấu xạ groupoid từ Grp(C) vào G kéo dài cấu xạ đồ thị có hướng $\varphi$.

#### Ví dụ {#ta-ii-s3-n10-exa-1 .statement tag=01TV}

Cho C là một đồ thị có hướng chỉ có một đỉnh duy nhất $s$ và A là tập hợp các mũi tên của nó. Khi đó groupoid Grp(C) là groupoid liên kết với nhóm tự do F(A) được xây dựng trên A. Thật vậy, nó có một đỉnh duy nhất $s$ và suy ra ngay lập tức từ Mệnh đề 6 rằng ánh xạ chính tắc từ A vào Grp(C)$_s$ suy ra từ cấu xạ chính tắc của C vào Grp(C) thỏa mãn tính chất phổ quát của các nhóm tự do (A, I, p. 85, Mệnh đề 8).

### 11. Co các mũi tên của một groupoid

Cho G là một groupoid và F là một tập con của tập hợp các mũi tên của G. Cho H là subgroupoid chuẩn của G sinh bởi F. Groupoid $G/H$ được gọi là groupoid suy ra từ G bằng cách co tập hợp các mũi tên F và được ký hiệu là $G/F$. Nếu $p$ ký hiệu cấu xạ chính tắc từ G vào $G/F$, ta có $p(o(f)) =p(t(f))$ và $p(f) =e_{p(o(f))}$ với mọi mũi tên $f\in F$.

Cấu xạ này thỏa mãn tính chất phổ quát sau đây.

#### Mệnh đề 7 {#ta-ii-s3-prop-7 .statement tag=01TW}

Với mọi cấu xạ groupoid $\varphi : G\rightarrow G'$ biến mọi mũi tên thuộc F thành một phần tử đơn vị của $G'$, tồn tại một cấu xạ groupoid duy nhất $\varphi ': G/F\rightarrow G'$ sao cho $\varphi '\circ p=\varphi$.

Hạt nhân của $\varphi$ là một subgroupoid chuẩn của G và tập hợp các mũi tên của nó chứa F. Theo định nghĩa, H là subgroupoid chuẩn nhỏ nhất của G mà tập hợp các mũi tên chứa F; do đó nó được chứa trong hạt nhân của $\varphi$. Khi đó mệnh đề suy ra từ II, p. 170, Mệnh đề 3.

Ký hiệu bởi Γ đồ thị con có hướng của G mà tập hợp các đỉnh là Som(G) và tập hợp các mũi tên là F. Các quỹ đạo của H được đồng nhất với các thành phần liên thông của đồ thị có hướng Γ. Theo định nghĩa của thương của một groupoid theo một subgroupoid chuẩn, tập hợp các đỉnh của $G/F$ được đồng nhất với tập hợp các thành phần liên thông của Γ; nói cách khác, đó là tập thương của Som(G) theo quan hệ tương đương mịn nhất sao cho $o(f)$ tương đương với $t(f)$ với mọi mũi tên $f\in F$.

Ánh xạ $p$ cảm sinh, bằng cách chuyển qua các thương, một song ánh từ tập hợp các quỹ đạo của G lên tập hợp các quỹ đạo của $G/F$ (II, p. 170, nhận xét 1).

Mục đích của Số$^o$ này là tính các đồng cấu cảm sinh bởi $p$ khi chuyển qua các nhóm đẳng hướng, điều này quy về, theo mệnh đề 2 (II, p. 170), việc tính các nhóm đẳng hướng của phân nhóm vị H.

#### Mệnh đề 8 {#ta-ii-s3-prop-8 .statement tag=01TX}

Cho $\delta$ là cấu xạ chính tắc của nhóm vị tự do Grp(Γ) vào G kéo dài cấu xạ đơn ánh chính tắc của Γ vào G. Cho $a$ là một đỉnh của G và A là quỹ đạo của $a$ trong G. Với mọi $b\in A$, gọi $f_{ab}$ là một mũi tên của G nối $a$ với $b$. Nhóm đẳng hướng $H_a$ là nhóm con phân biệt của $G_a$ sinh bởi các phần tử Int($f_{ab}$)$(\delta (c))$, trong đó $b$ chạy qua tập hợp A và $c$ chạy qua các phần tử của Grp(Γ)$_b$.

Nếu $x$ và $y$ là các đỉnh của G thuộc cùng một quỹ đạo, với $x=\not a$, ta còn cố định một mũi tên $f_{xy}$ của G nối $x$ với $y$. Với mọi điểm $x$ của G, gọi $N_x$ là nhóm con phân biệt của $G_x$ sinh bởi các phần tử Int($f_{xy}$)$(\delta (c))$, trong đó $y$ chạy qua quỹ đạo của $x$ trong G và $c$ chạy qua nhóm Grp(Γ)$_y$. Với mọi $f\in G_{xy}$ và mọi $g\in N_y$, ta có $f gf^{-1}\in N_x$. Cho $x\in$ Som(G). Theo định nghĩa của $N_x$, ta có $\delta$(Grp(Γ)$_x$)$\subset N_x$. Theo định nghĩa của nhóm vị H$,\delta (f)$ là một mũi tên của H với mọi mũi tên $f$ của Grp(Γ) ; do đó, $\delta$(Grp(Γ)$_x$) được chứa trong $H_x$. Vì H là một phân nhóm vị phân biệt của G, suy ra

Int($f_{xy}$)$(\delta (c))\in$ Int($f_{xy}$)$(N_y)\subset$ Int($f_{xy}$)$(H_y)\subset H_x$

với mọi $y\in$ Som(G), và vì thế $N_x\subset H_x$.

Cho $x$ và $y$ là các đỉnh của Γ. Đặt $N_{x,y}=\emptyset$ nếu $x$ và $y$ không thuộc cùng một thành phần liên thông của Γ. Trong trường hợp ngược lại, gọi $c$ và $c'$ là các lớp đường đi nối $x$ với $y$ trong quiver $\widetilde{\Gamma}$ liên kết với Γ. Gọi $z$ là một đỉnh của G thuộc quỹ đạo của $y$ và gọi $\ell$ là một phần tử của Grp(Γ)$_z$; trong nhóm $G_x$, ta có đẳng thức:

$$
\delta (c)f_{yz}\delta (\ell )f_{yz}^{-1}\delta (c')^{-1}
$$

$$
=\delta (c)f_{yz}f_{xz}^{-1}(f_{xz}\delta (\ell )f_{xz}^{-1})f_{xz}f_{yz}^{-1}\delta (c)^{-1}\delta (c(c')^{-1})
$$

Mũi tên $\delta (c(c')^{-1})$ là lớp của một vòng tại $x$ trong quiver Γ, do đó thuộc $N_x$, và mũi tên $f_{xz}\delta (\ell )f_{xz}^{-1}$ cũng vậy. Vì $\delta (c)f_{yz}f_{xz}^{-1}$ thuộc $G_x$ và $N_x$ là một nhóm con phân biệt của $G_x$, suy ra $\delta (c)f_{yz}\delta (\ell )f_{yz}^{-1}\delta (c')^{-1}$ thuộc $N_x$. Do đó, $\delta (c)N_y\subset N_x\delta (c')$. Theo đối xứng, ta có $\delta (c)N_y= N_x\delta (c')$. Điều này suy ra rằng tập hợp này không phụ thuộc vào lựa chọn $c$ và $c'$; ta ký hiệu nó bởi $N_{x,y}$.

Gọi N là sous-quiver của G mà tập hợp các đỉnh là Som(G) và tập hợp các mũi tên nối $x$ với $y$ bằng $N_{x,y}$ với mọi cặp $(x, y)$ đỉnh của G. Đó là một subgroupoid phân biệt của G mà tập hợp các mũi tên chứa F; do đó H là một subgroupoid của N. Đặc biệt, $H_a\subset N_a$, do đó có đẳng thức.

#### Hệ quả 1 {#ta-ii-s3-prop-8-cor-1 .statement tag=01TY}

Giả sử thêm rằng, với mọi mũi tên $f$ của F, ta có $o(f) =t(f)$. Khi đó gốc và ngọn của mọi đường đi trong quiver Γ trùng nhau. Gọi $a$ là một đỉnh của G và gọi A là quỹ đạo của nó trong G. Với mọi phần tử $c$ của F mà gốc $b$ của nó thuộc A, cố định một mũi tên $f_c$ của G nối $a$ với $b$ và đặt $\kappa (c) =$ Int($f_c$)$(\delta (c)) =$ $f_c\delta (c)f_c^{-1}$.

Khi đó nhóm $H_a$ là nhóm con phân biệt của $G_a$ sinh bởi các mũi tên $\kappa (c)$.

Theo Mệnh đề 8, các mũi tên $\kappa (c)$ được chứa trong nhóm $H_a$. Ký hiệu $N_a$ là nhóm con chuẩn tắc nhỏ nhất của $G_a$ chứa chúng. Theo mệnh đề đó, chỉ cần chứng minh rằng, với mọi đỉnh $b$ của G thuộc A, mọi mũi tên $f_{ab}$ nối $a$ với $b$ trong G, và mọi phần tử $c$ của Grp(Γ)$_b$, Int($f_{ab}$)$(\delta (c))$ thuộc $N_a$. Vì gốc và số hạng của mọi phần tử của F đều bằng nhau, một vòng tại một đỉnh $b$ trong đồ thị $\widetilde{\Gamma}$ có dạng $(b,(f_1, \varepsilon_1), b, . . . ,(f_n, \varepsilon_n), b)$, trong đó với mọi $i\in  \{1, . . . , n\},f_i$ là một phần tử của F có gốc là $b$ và $\varepsilon_i\in  \{-1,1\}$. Ta có

Int($f_{ab}$)$(\delta (c)) =f_{ab}f_c^{-1}\kappa (f_1)^{\varepsilon_1}. . . \kappa (f_n)^{\varepsilon_n}f_cf_{ab}^{-1}$.

Vì $f_{ab}f_c^{-1}\in G_a$, suy ra Int($f_{ab}$)$(\delta (c))$ thuộc $N_a$.

#### Hệ quả 2 {#ta-ii-s3-prop-8-cor-2 .statement tag=01TZ}

Nếu đồ thị liên kết với quiver Γ là một rừng, thì đồng cấu $p_a$ từ $G_a$ vào $(G/F)_{p(a)}$ là song ánh, với mọi đỉnh $a$ của G.

Thật vậy, dưới giả thiết này, ta có Grp(Γ)$_b=\{e_b\}$ với mọi đỉnh $b$ của G (Hệ quả 1 của II, p. 173). Khi đó từ Mệnh đề 8 suy ra rằng, với mọi đỉnh $a$ của G, nhóm $H_a$ thu về phần tử đơn vị.

### 12. Nhóm Poincaré của một Đồ thị

Cho G là một đồ thị. Cho $a$ là một đỉnh của G; nhóm đẳng hướng tại $a$ của groupoid Grp(G) được gọi là nhóm Poincaré của G tại $a$ và được ký hiệu bởi $\pi_1(G, a)$. Cho $c$ là một lớp đường đi trong G, và cho $a$ là gốc của nó và $b$ là số hạng của nó. Ánh xạ Int($c$)$:\pi_1(G, b)\rightarrow \pi_1(G, a)$ được xác định bởi $c'\mapsto cc'c^{-1}$ là một đẳng cấu nhóm. Cho $\varphi : G\rightarrow H$ là một cấu xạ đồ thị. Gọi $\theta_G: G\rightarrow$ Grp(G) và $\theta_H: H\rightarrow$ Grp(H) là các cấu xạ chính tắc. Nếu $\overline{\varphi}$ ký hiệu cấu xạ groupoid duy nhất Grp(G) $\rightarrow$ Grp(H) sao cho $\overline{\varphi}\circ \theta_G=\theta_H\circ \varphi$, thì đồng cấu nhóm $\overline{\varphi}_a:\pi_1(G, a)\rightarrow \pi_1(H, \varphi (a))$ được ký hiệu bởi $\pi_1(\varphi , a)$.

Cho G là một đồ thị liên thông, cho S là một định hướng của G và cho A là một cây định hướng cực đại của G (II, p. 157, mệnh đề 1). Với các đỉnh $a$ và $b$ của G, tồn tại một lớp đường đi duy nhất $\gamma_{a,b}$ trong đồ thị $\widetilde{A}$ liên kết với A nối $a$ với $b($II, p. 174, hệ quả 4 của mệnh đề 5). Nếu $a$, $b$ và $c$ là các đỉnh của G, ta có $\gamma_{a,b}\gamma_{b,c}=\gamma_{a,c}$, hai lớp đường đi này đều bằng lớp đường đi duy nhất nối $a$ với $c$ trong $\widetilde{A}$.

#### Mệnh đề 9 {#ta-ii-s3-prop-9 .statement tag=01U0}

Cho $a$ là một đỉnh của G. Tồn tại một đồng cấu duy nhất $\lambda$ của nhóm tự do F(S-Fl(A)) vào $\pi_1(G, a)$ sao cho

$$
\lambda (f) =\gamma_{a,o(f)}\cdot f\cdot \gamma_{t(f),a} \tag{1}
$$

với $f\in S$ - Fl(A). Đồng cấu $\lambda$ là một đẳng cấu nhóm.

Ta ký hiệu bởi L nhóm F(S-Fl(A)). Sự tồn tại và tính duy nhất của đồng cấu $\lambda : L\rightarrow \pi_1(G, a)$ thỏa mãn các hệ thức (1) suy ra từ A, I, p. 85, mệnh đề 8. Cho $\mathscr{L}$ là vị nhóm liên kết với nhóm L (II, p. 163, ví dụ 1); ta ký hiệu bởi $s$ đỉnh duy nhất của nó. Tồn tại một cấu xạ vị nhóm duy nhất $\mu:$ Grp(G) $\rightarrow \mathscr{L}$ sao cho $\mu(\theta_G(f)) =f$ với mọi mũi $f\in$ S-Fl(A) và $\mu(\theta_G(f)) =e_s$ với mọi mũi $f\in$ Fl(A) (II, p. 173, mệnh đề 5). Với $f\in$ S-Fl(A), ta có $\mu(\theta_G(f)) =f$; do đó đồng cấu $\mu_a\circ \lambda$ là đẳng cấu đồng nhất của nhóm L (A, I, p. 85, mệnh đề 8). Suy ra rằng $\lambda$ là đơn ánh.

Cho $\varpi_G/A$ là vị nhóm suy ra từ $\varpi_G$ bằng cách co rút các mũi của A và cho $p:\varpi_G\rightarrow \varpi_G/A$ là cấu xạ vị nhóm chính tắc. Nó là toàn ánh và đồng cấu nhóm $p_a$ suy ra từ $p$ bằng cách chuyển qua các nhóm đẳng hướng là một đẳng cấu (II, p. 178, hệ quả 2 của mệnh đề 8). Vì đồ thị G được giả thiết là liên thông và A là một cây cực đại trong đó, vị nhóm $\varpi_G/A$ có một đỉnh duy nhất (II, p. 176). Hơn nữa, $\varpi_G$ được sinh bởi $\theta_G(G)$; do đó, $\varpi_G/A$ được sinh bởi các vòng $p(f)$, với $f\in S$, và nhóm $(\varpi_G/A)_{p(a)}$ được sinh bởi các phần tử dạng $p(\theta_G(f))$, với $f\in$ S-Fl(A). Vậy đồng cấu $p_a\circ \lambda$ là toàn ánh. Do đó, $\lambda$ là toàn ánh.

#### Nhận xét 1 {#ta-ii-s3-n12-rem-1 .statement tag=01U1}

Đồng cấu $\mu_a$ là đẳng cấu nghịch đảo của $\lambda$.

#### Nhận xét 2 {#ta-ii-s3-n12-rem-2 .statement tag=01U2}

Tồn tại một đồng cấu duy nhất $\lambda :$ F(Fl(G)) $\rightarrow \pi_1(G, a)$ được xác định bởi các hệ thức (1) với mọi $f\in$ Fl(G). Suy ra từ mệnh đề 8 rằng đồng cấu $\lambda$ là toàn ánh và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của F(Fl(G)) chứa các phần tử $f$, với $f\in$ Fl(A), và các phần tử $f\cdot \overline{f}$, với $f\in$ Fl(G).

## BÀI TẬP {#ta-ii-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
