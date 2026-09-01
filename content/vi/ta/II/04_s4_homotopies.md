---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 4
section_title: Homotopies
lang: vi
source: ta-i-iv-fr
book_pages: TA II.180-TA II.196
pdf_pages: 0196-0212
extraction: native
subsections:
    - "no": 1
      title: Définition des homotopies
      page: 180
      pdf_page: 196
    - "no": 2
      title: Homotopismes de groupoïdes
      page: 181
      pdf_page: 197
    - "no": 3
      title: Cohomotopeur
      page: 184
      pdf_page: 200
    - "no": 4
      title: Comparaison de deux cohomotopeurs
      page: 187
      pdf_page: 203
    - "no": 5
      title: Groupes d’isotropie d’un cohomotopeur
      page: 192
      pdf_page: 208
statements: 15
exercises: 0
content_sha256: 432e1fe232625b589ee7595044bae75aa89aa5eeeaaffb94c1ba7f769ffaa976
translated_from: content/en-mt/ta/II/04_s4_homotopies.md
source_lang: en-mt
translation_method: machine
source_content_sha256: e32055ea451e7df87f25887fbf6aebc11fc734c7b092667a2f3abc000a796629
translation_model: gpt-5.4
translation_run: translate-vi-1aaff44f
glossary_version: 34
glossary_terms_sha256: df0a98704dd2ee9dd8c850d8f7398e80239cb4c5abf86392e3baf22d86fbbf9e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. ĐỒNG LUÂN

### 1. Định nghĩa các đồng luân

#### Định nghĩa 1 {#ta-ii-s4-def-1 .statement tag=01U3}

Cho G là một groupoid, H là một đồ thị có hướng, $\varphi$ và $\varphi '$ là các cấu xạ của đồ thị có hướng từ H vào G. Một đồng luân nối $\varphi$ với $\varphi '$ là một ánh xạ $h$ từ tập hợp các đỉnh của H vào tập hợp các mũi tên của G có các tính chất sau đây:

(i) Với mọi đỉnh $a$ của H, mũi tên $h(a)$ có gốc là $\varphi (a)$ và ngọn là $\varphi '(a)$;

(ii) Với mọi mũi tên $f$ của H, có gốc $a$ và ngọn $b$, ta có $\varphi (f)h(b) =h(a)\varphi '(f)$.

Ta nói rằng $\varphi$ và $\varphi '$ đồng luân nếu tồn tại một đồng luân nối $\varphi$ với $\varphi '$.

Cho G là một groupoid, cho H là một đồ thị có hướng và cho $\varphi ,\varphi ',\varphi ''$ là các cấu xạ của đồ thị có hướng từ H vào G. Ánh xạ $a\mapsto e_{\varphi(a)}$ là một đồng luân nối $\varphi$ với $\varphi$. Nếu $h$ là một đồng luân nối $\varphi$ với $\varphi '$, thì ánh xạ $a\mapsto h(a)^{-1}$ là một đồng luân nối $\varphi '$ với $\varphi$. Cho $h$ và $h'$ là các đồng luân nối lần lượt $\varphi$ với $\varphi '$ và $\varphi '$ với $\varphi ''$. Với mọi đỉnh $a$ của H, các mũi tên $h(a)$ và $h'(a)$ hợp thành được. Ánh xạ $a\mapsto h(a)h'(a)$ là một đồng luân nối $\varphi$ với $\varphi ''$.

Suy ra rằng quan hệ “ $\varphi$ đồng luân với $\varphi '$ ” là một quan hệ tương đương trên tập hợp các cấu xạ của đồ thị có hướng từ H vào G.

Cho G là một groupoid, H là một đồ thị có hướng và $\varphi ,\varphi '$ là các cấu xạ của đồ thị có hướng từ H vào G đồng luân với nhau. Theo điều kiện (i) của Định nghĩa 1, với mọi đỉnh $a$ của H, các đỉnh $\varphi (a)$ và $\varphi '(a)$ thuộc cùng một quỹ đạo của G.

Giả sử hơn nữa rằng H là một groupoid, và gọi $h$ là một đồng luân nối $\varphi$ với $\varphi '$. Khi đó các ánh xạ Orb($\varphi$ ) và Orb($\varphi '$) suy ra từ $\varphi$ và $\varphi '$ bằng cách chuyển qua các quỹ đạo là bằng nhau. Với mọi đỉnh $a$ của H và mọi mũi tên $f\in H_a$, ta có $\varphi (f) =h(a)\varphi '(f)h(a)^{-1}=$ Int($h(a)$)$(\varphi '(f))$, theo điều kiện (ii) của Định nghĩa 1. Nói cách khác, đồng cấu $\varphi_a$ bằng Int($h(a)$)$\circ \varphi '_a$. Đặc biệt, nếu đồng cấu $\varphi_a$ là đơn ánh (tương ứng, song ánh, tương ứng, toàn ánh), thì đồng cấu $\varphi '_a$ cũng có tính chất đó.

#### Nhận xét 1 {#ta-ii-s4-n1-rem-1 .statement tag=01U4}

Cho G, $G'$ là các groupoid, H, $H'$ là các đồ thị có hướng, cho $u: H'\rightarrow H$ là một cấu xạ của các đồ thị có hướng và $v: G\rightarrow G'$ là một cấu xạ của các groupoid. Nếu các cấu xạ của đồ thị có hướng $\varphi ,\varphi '$ từ H vào G là đồng luân, thì các cấu xạ của đồ thị có hướng $v\circ \varphi \circ u$ và $v\circ \varphi '\circ u$ từ $H'$ vào $G'$ là đồng luân. Chính xác hơn, nếu $h$ là một đồng luân nối $\varphi$ với $\varphi '$, thì ánh xạ Fl($v$)$\circ h\circ$ Som($u$) là một đồng luân nối $v\circ \varphi \circ u$ với $v\circ \varphi '\circ u$.

#### Nhận xét 2 {#ta-ii-s4-n1-rem-2 .statement tag=01U5}

Cho G là một groupoid, H là một đồ thị có hướng, và cho $\varphi , \psi$ là các cấu xạ của đồ thị có hướng từ H vào G. Ta ký hiệu bởi $j$ cấu xạ chính tắc từ H vào Grp(H), và bởi $\overline{\varphi}$ và $\overline{\psi}$ các cấu xạ của các groupoid từ Grp(H) vào G sao cho $\overline{\varphi}\circ j=\varphi$ và $\overline{\psi}\circ j=\psi$.

Nhắc lại rằng Som(H) = Som(Grp(H)).

Một đồng luân $h:$ Som(H) $\rightarrow$ Fl(G) nối $\varphi$ với $\psi$ là một đồng luân nối $\overline{\varphi}$ với $\overline{\psi}$.

### 2. Homotopism của các groupoid

Trong No$^o$ này, ta sẽ dùng ký hiệu $u\sim v$ để biểu thị rằng hai cấu xạ của các groupoid $u$ và $v$ là đồng luân.

#### Định nghĩa 2 {#ta-ii-s4-def-2 .statement tag=01U6}

Cho G, $G'$ là các vị nhóm và cho $\varphi$ là một cấu xạ từ G vào $G'$. Một nghịch đảo tới đồng luân của $\varphi$ là một cấu xạ vị nhóm $\psi$ từ $G'$ vào G sao cho các cấu xạ $\psi \circ \varphi$ và $\varphi \circ \psi$ lần lượt đồng luân với Id$_G$ và với Id$_{G'}$. Ta nói rằng $\varphi$ là một đồng luân tương đương nếu tồn tại một nghịch đảo của $\varphi$ tới đồng luân.

Một đẳng cấu của các vị nhóm là một đồng luân tương đương.

Cho G và $G'$ là các vị nhóm. Cho $\varphi ,\varphi '$ là các cấu xạ vị nhóm từ G vào $G'$ đồng luân với nhau. Nếu $\varphi$ là một đồng luân tương đương, thì $\varphi '$ cũng vậy. Thật vậy, nếu $\psi$ ký hiệu một nghịch đảo của $\varphi$ tới đồng luân, ta có $\psi \circ \varphi '\sim \psi \circ \varphi \sim$ Id$_G$ và $\varphi '\circ \psi \sim \varphi \circ \psi \sim$ Id$_{G'}$, điều đó chứng minh rằng $\psi$ là một nghịch đảo tới đồng luân của $\varphi '$.

Cho G, $G',G''$ là các vị nhóm và cho $\varphi : G\rightarrow G',\varphi ': G'\rightarrow G''$, $\psi : G'\rightarrow G,\psi ': G''\rightarrow G'$ là các cấu xạ vị nhóm. Khi đó, trong các điều kiện sau:

(i) $\psi$ là một nghịch đảo tới đồng luân của $\varphi$;

(ii) $\psi '$ là một nghịch đảo tới đồng luân của $\varphi '$;

(iii) $\psi \circ \psi '$ là một nghịch đảo tới đồng luân của $\varphi '\circ \varphi$; bất kỳ hai điều kiện nào cũng suy ra điều kiện thứ ba. Thật vậy, trước hết giả sử rằng (i) và (ii) được thỏa mãn; khi đó ta có

$\psi \circ \psi '\circ \varphi '\circ \varphi \sim \psi \circ$ Id$_{G'}\circ \varphi \sim \psi \circ \varphi \sim$ Id$_G$

và, tương tự, $\varphi '\circ \varphi \circ \psi \circ \psi '\sim$ Id$_{G'}$, do đó có (iii). Nếu (i) và (iii) được thỏa mãn,

$\varphi '\circ \psi '\sim \varphi '\circ \varphi \circ \psi \circ \psi '\sim$ Id$_{G''}$

và

$\psi '\circ \varphi '\sim (\varphi \circ \psi )\circ \psi '\circ \varphi '\circ (\varphi \circ \psi )\sim \varphi \circ \psi \sim$ Id$_{G'}$,

do đó có điều kiện (ii). Chứng minh rằng các điều kiện (ii) và (iii) suy ra điều kiện (i) là tương tự.

Đặc biệt, nếu hai trong ba cấu xạ $\varphi ,\varphi ',\varphi '\circ \varphi$ là các đồng luân tương đương, thì cấu xạ thứ ba cũng vậy.

#### Mệnh đề 1 {#ta-ii-s4-prop-1 .statement tag=01U7}

Cho G, $G'$ là các vị nhóm, cho $\varphi$ là một cấu xạ từ G vào $G'$, và cho A là một tập con của tập hợp các đỉnh của G cắt mọi quỹ đạo của G. Để $\varphi$ là một đồng luân tương đương, điều kiện cần và đủ là các điều kiện sau được thỏa mãn:

(i) ánh xạ Orb($\varphi$ ) từ Orb(G) vào Orb(G$'$), suy ra từ $\varphi$ bằng cách chuyển qua các quỹ đạo, là song ánh;

(ii) với mọi $a\in A$, đồng cấu $\varphi_a: G_a\rightarrow G'_{\varphi(a)}$ là song ánh.

Trước hết giả sử rằng $\varphi$ là một đồng luân tương đương và cho $\psi$ là một nghịch đảo của $\varphi$ tới đồng luân. Khi đó,

Orb($\psi$ )$\circ$ Orb($\varphi$ ) $=$ Orb($\psi \circ \varphi$ ) $=$ Orb(Id$_G$) $=$ Id$_{Orb(G)}$,

vì hai cấu xạ groupoid đồng luân cảm sinh cùng một ánh xạ khi chuyển qua các quỹ đạo. Tương tự, Orb($\varphi$ )$\circ$ Orb($\psi$ ) $=$ Id$_{Orb(G')}$. Do đó ánh xạ Orb($\varphi$ ) là song ánh, do đó suy ra mệnh đề (i). Ta cũng có, với mọi đỉnh $a$ của G,

$$
\psi_{\varphi(a)}\circ \varphi_a= (\psi \circ \varphi )_a
$$

vì $\psi \circ \varphi$ đồng luân với Id$_G$, đồng cấu $(\psi \circ \varphi )_a$ là song ánh (xem p. 180), nên $\varphi_a$ là đơn ánh và $\psi_{\varphi(a)}$ là toàn ánh. Khi đổi chỗ vai trò của $\varphi$ và $\psi$, ta thấy rằng $\varphi_a$ cũng là toàn ánh, do đó suy ra điều kiện (ii).

Bây giờ giả sử rằng các điều kiện (i) và (ii) được thỏa mãn, và hãy chứng minh rằng $\varphi$ là một homotopism.

Trước hết hãy xét trường hợp mỗi quỹ đạo của $G'$ thu về một điểm.

Với mỗi đỉnh $b$ của $G'$, chọn một đỉnh $u(b)$ của G thuộc A và có ảnh dưới $\varphi$ là $b$. Điều này là có thể vì ánh xạ Orb($\varphi$ ) là toàn ánh và A cắt mỗi quỹ đạo của G. Cho $f$ là một mũi tên của $G'$; theo giả thiết ta có $o(f) =t(f)$; đặt $b=o(f)$ và $a=u(b)$. Theo điều kiện (ii), tồn tại một mũi tên duy nhất $v(f)\in G_a$ có ảnh dưới $\varphi$ là $f$. Cặp $\psi = (u, v)$ là một cấu xạ groupoid từ $G'$ vào G. Hãy chứng minh rằng $\psi$ là nghịch đảo của $\varphi$ đến đồng luân. Theo phép dựng của $\psi$, ta đã có $\varphi \circ \psi =$ Id$_{G'}$.

Cho $x$ là một đỉnh của G. Đặt $a=\psi (\varphi (x))$; đây là một phần tử của A sao cho $\varphi (a) =\varphi (x)$. Vì Orb($\varphi$ ) là đơn ánh, $a$ thuộc quỹ đạo của $x$ trong G và tồn tại một mũi tên $f$ trong G nối $a$ với $x$. Khi đó mũi tên $h(x) =\psi (\varphi (f))^{-1}f$ nối $a$ với $x$ và ta có $\varphi (h(x)) =e_{\varphi(a)}$.

Hãy chỉ ra rằng ánh xạ $h:$ Som(G) $\rightarrow$ Fl(G) thu được là một đồng luân nối $\psi \circ \varphi$ với Id$_G$. Điều kiện (i) của định nghĩa 1 được thỏa mãn, theo phép dựng. Cho $f$ là một mũi tên của G$,x$ là gốc của nó và $y$ là đích của nó. Ta có $\varphi (x) =\varphi (y)$ ; đặt $a=\psi (\varphi (x)) =\psi (\varphi (y))$. Các mũi tên $h(x)f h(y)^{-1}$ và $\psi \circ \varphi (f)$ thuộc $G_a$ và cả hai đều có ảnh là $\varphi (f)$ trong $G'_{\varphi(a)}$. Vì ánh xạ $\varphi_a$ là đơn ánh, ta có $h(x)f h(y)^{-1}=\psi \circ \varphi (f)$. Vậy điều kiện (ii) của định nghĩa 1 được thỏa mãn.

Bây giờ chứng minh mệnh đề 1 trong trường hợp tổng quát. Cho X là một rừng có hướng cực đại của $G'($II, p. 157, mệnh đề 1). Gọi $G''$ là groupoid suy ra từ $G'$ bằng phép co các mũi tên của X và gọi $\varphi ': G'\rightarrow G''$ là cấu xạ chính tắc. Cấu xạ $\varphi '$ thỏa mãn các điều kiện của mệnh đề 1 (II, p. 170, nhận xét 1 và p. 178, hệ quả 2), và do đó điều tương tự cũng đúng với cấu xạ $\varphi '\circ \varphi$.

Vì các quỹ đạo của $G''$ rút về các điểm, suy ra từ trường hợp riêng đã được chứng minh rằng $\varphi '$ và $\varphi '\circ \varphi$ là các homotopism, nên $\varphi$ cũng vậy. Điều này hoàn tất chứng minh của mệnh đề.

#### Hệ quả 1 {#ta-ii-s4-prop-1-cor-1 .statement tag=01U8}

Cho G là một groupoid, A là một tập hợp và $f: A\rightarrow$ Som(G) là một ánh xạ. Nếu ảnh của $f$ cắt mỗi quỹ đạo của G, thì cấu xạ groupoid chính tắc $\varphi$ từ $f^*G$ vào G là một homotopism.

Theo định nghĩa của groupoid ảnh ngược (II, p. 166, ví dụ 4), A là tập hợp các đỉnh của groupoid $f^*G$ và ta có Fl$_{a,b}(f^*G) =$ Fl$_{f(a),f(b)}(G)$ với mọi cặp $(a, b)$ phần tử của A. Hơn nữa, ta có Som($\varphi$ ) $=f$ và Fl($\varphi$ ) cảm sinh ánh xạ đồng nhất từ Fl$_{a,b}(f^*G)$ vào Fl$_{f(a),f(b)}(G)$. Do đó, ánh xạ Orb($\varphi$ ) là song ánh và đồng cấu $\varphi_a: (f^*G)_a\rightarrow G_{f(a)}$ là một đẳng cấu, với mọi $a\in A$. Vậy các giả thiết của mệnh đề 1 được thỏa mãn.

#### Hệ quả 2 {#ta-ii-s4-prop-1-cor-2 .statement tag=01U9}

Cho G là một groupoid, X là một rừng có hướng của G, và $G'$ là groupoid suy ra từ G bằng phép co các mũi tên của X. Cấu xạ chính tắc từ G vào $G'$ là một homotopism.

Thật vậy, điều này suy ra từ nhận xét 1 của II, p. 170 và hệ quả 2 của II, p. 178 rằng các giả thiết của mệnh đề 1 được thỏa mãn.

### 3. Cohomotoper

Cho H là một quiver, G là một groupoid, và $\varphi$ và $\psi$ là các cấu xạ quiver từ H vào G.

Gọi $G_1$ là quiver được xác định như sau: các đỉnh của $G_1$ là các đỉnh của G; các mũi tên của $G_1$ là các phần tử của tổng các tập hợp Fl(G) và Som(H); ánh xạ gốc của $G_1$ trùng với ánh xạ gốc của G trên Fl(G) và với Som($\varphi$ ) trên Som(H); ánh xạ đích của $G_1$ trùng với ánh xạ đích của G trên Fl(G) và với Som($\psi$ ) trên Som(H). Gọi $\alpha_1$ là cấu xạ quiver từ G vào $G_1$ được xác định bởi ánh xạ đồng nhất của Som(G) và bởi đơn ánh chính tắc từ Fl(G) vào Fl(G$_1$). Gọi $h_1$ là đơn ánh chính tắc Som(H) $\rightarrow$ Fl(G$_1$).

Xét vị nhóm tự do Grp(G$_1$) được dựng trên $G_1($II, p. 174, định nghĩa 9), và gọi $\theta_1$ là cấu xạ quiver chính tắc từ $G_1$ vào Grp(G$_1$). Sau cùng, ký hiệu Coh($\varphi , \psi$ ) là vị nhóm suy ra từ Grp(G$_1$) bằng cách co các vòng (tại gốc của $x$)

$$
\alpha_1(x)\alpha_1(y)\alpha_1(xy)^{-1} \tag{1}
$$

với mọi cặp $(x, y)$ gồm các mũi tên ghép được của G, cũng như các vòng (tại $\varphi (a)$)

$$
\alpha_1(\varphi (f))h_1(b)\alpha_1(\psi (f))^{-1}h_1(a)^{-1} \tag{2}
$$

với $a,b$ thuộc Som(H) và $f\in$ Fl$_{ab}(H)$. Gọi $\pi :$ Grp(G$_1$)$\rightarrow$ Coh($\varphi , \psi$ ) là cấu xạ chính tắc; đặt $\alpha$ = $\pi \circ \theta_1\circ \alpha_1$ và $h=$ Fl($\pi \circ \theta_1$)$\circ h_1$.

#### Mệnh đề 2 {#ta-ii-s4-prop-2 .statement tag=01UA}

Vị nhóm Coh($\varphi , \psi$ ) được sinh bởi quiver con mà tập hợp các đỉnh là Som(G) và tập hợp các mũi tên là hợp của các ảnh của các ánh xạ Fl($\alpha$ ) và $h$.

Quiver con này là ảnh của quiver $G_1$ dưới cấu xạ quiver $\pi \circ \theta_1$, nên mệnh đề suy ra ngay từ phép dựng của Coh($\varphi , \psi$ ).

#### Mệnh đề 3 {#ta-ii-s4-prop-3 .statement tag=01UB}

Cấu xạ quiver $\alpha$ là một cấu xạ vị nhóm từ G vào Coh($\varphi , \psi$ ), và ánh xạ $h$ là một đồng luân nối $\alpha \circ \varphi$ với $\alpha \circ \psi$.

Bộ ba (Coh($\varphi , \psi$ )$, \alpha , h$) có tính chất phổ quát sau đây: nếu $G'$ là một groupoid, $\alpha '$ là một cấu xạ của các groupoid từ G vào $G'$ và $h':$ Som(H) $\rightarrow$ Fl(G$'$) là một đồng luân nối $\alpha '\circ \varphi$ với $\alpha '\circ \psi$, thì tồn tại một cấu xạ duy nhất của các groupoid $\eta :$ Coh($\varphi , \psi$ )$\rightarrow G'$ sao cho

(3) $\alpha '=\eta \circ \alpha$ và $h'=$ Fl($\eta$ )$\circ h$.

Theo định nghĩa của groupoid suy ra bằng co các mũi tên, việc co các vòng (1) kéo theo rằng $\alpha$ là một cấu xạ của các groupoid, và việc co các vòng (2) kéo theo rằng $h$ là một đồng luân nối $\alpha \circ \varphi$ với $\alpha \circ \psi$.

Cho $G',\alpha ',h'$ như trong mệnh đề. Gọi $\eta_1$ là cấu xạ của các đồ thị có hướng từ $G_1$ vào $G'$ sao cho Som($\eta_1$) bằng Som($\alpha '$) và sao cho Fl($\eta_1$) trùng với Fl($\alpha '$) trên Fl(G) và với $h'$ trên Som(H). Tồn tại một cấu xạ duy nhất của các groupoid $\eta_2:$ Grp(G$_1$)$\rightarrow G'$ sao cho $\eta_1=\eta_2\circ \theta_1$. Vì $\alpha '$ là một cấu xạ của các groupoid và $h'$ là một đồng luân nối $\alpha '\circ \varphi$ với $\alpha '\circ \psi ,\eta_2$ xác định bằng cách chuyển qua thương một cấu xạ của các groupoid $\eta$ từ Coh($\varphi , \psi$ ) vào $G'($II, p. 170, mệnh đề 3). Cấu xạ này thỏa mãn các hệ thức (3), và đó là cấu xạ duy nhất (II, p. 185, mệnh đề 2).

#### Định nghĩa 3 {#ta-ii-s4-def-3 .statement tag=01UC}

Groupoid Coh($\varphi , \psi$ ) được gọi là bộ đối đồng luân hóa của cặp $(\varphi , \psi )$. Ta nói rằng $\alpha$ là cấu xạ chính tắc từ G vào Coh($\varphi , \psi$ ) và $h$ là đồng luân chính tắc nối $\alpha \circ \varphi$ với $\alpha \circ \psi$.

Đồ thị có hướng mà tập các đỉnh là tập các quỹ đạo của G, tập các mũi tên là tập các thành phần liên thông của H, và các ánh xạ gốc và ngọn được suy ra từ $\varphi$ và $\psi$ bằng cách chuyển qua các thương, được gọi là khung của cặp $(\varphi , \psi )$.

#### Mệnh đề 4 {#ta-ii-s4-prop-4 .statement tag=01UD}

Ánh xạ Orb($\alpha$ )$:$ Orb(G) $\rightarrow$ Orb(Coh($\varphi , \psi$ )) là toàn ánh; các thớ của nó là các thành phần liên thông của khung của cặp $(\varphi , \psi )$.

Cấu xạ $\alpha$ là hợp thành của các cấu xạ $\alpha_1: G\rightarrow G_1$, $\theta_1: G_1\rightarrow$ Grp(G$_1$) và $\pi :$ Grp(G$_1$)$\rightarrow$ Coh($\varphi , \psi$ ). Ánh xạ $\theta_1$ cảm sinh một song ánh từ tập hợp các thành phần liên thông của đồ thị có hướng $G_1$ lên tập hợp các quỹ đạo của Grp(G$_1$), và ánh xạ Orb($\pi$ )$:$ Orb(Grp(G$_1$))$\rightarrow$ Orb(Coh($\varphi , \psi$ )) là song ánh (II, p. 170, nhận xét 1). Vì vậy chỉ cần chứng minh rằng ánh xạ từ Orb(G) vào $\pi_0(G_1)$ suy ra từ $\alpha_1$ là toàn ánh và các thớ của nó là các thành phần liên thông của khung của cặp $(\varphi , \psi )$. Tính toàn ánh suy ra từ việc ánh xạ Som($\alpha_1$) là ánh xạ đồng nhất. Quan hệ tương đương trong Som(G) được xác định bởi “$a$ và $b$ thuộc cùng một thành phần liên thông của $G_1$” được sinh bởi các quan hệ “tồn tại một mũi tên của G nối $a$ với $b$” và “tồn tại một đỉnh $h$ của H sao cho $\varphi (h) =a$ và $\psi (h) =b$”. Quan hệ tương đương này tương thích với ánh xạ từ Som(G) vào Orb(G), và quan hệ suy ra từ nó trên Orb(G) được sinh bởi quan hệ “tồn tại một quỹ đạo $\eta$ của H sao cho Orb($\varphi$ )$(\eta ) =\alpha$ và Orb($\psi$ )$(\eta ) =\beta$”. Do đó nó là quan hệ “$\alpha$ và $\beta$ thuộc cùng một thành phần liên thông của khung của cặp $(\alpha , \beta )$”.

#### Mệnh đề 5 {#ta-ii-s4-prop-5 .statement tag=01UE}

Cho $G'$ là một groupoid, cho $\eta ,\eta '$ là các cấu xạ groupoid từ Coh($\varphi , \psi$ ) vào $G'$, và cho $k$ là một ánh xạ từ Som(G) vào Fl(G$'$). Để $k$ là một đồng luân nối $\eta$ với $\eta '$, điều kiện cần và đủ là hai điều kiện sau được thỏa mãn:

(i) Ánh xạ $k$ là một đồng luân nối $\eta \circ \alpha$ với $\eta '\circ \alpha$;

(ii) Với mọi đỉnh $a$ của H, ta có

$$
\eta (h(a))k(\psi (a)) =k(\varphi (a))\eta '(h(a))
$$

Theo định nghĩa, để $k$ là một đồng luân nối $\eta$ với $\eta '$, điều kiện cần và đủ là hai điều kiện sau được thỏa mãn (nhắc lại rằng Som(G) = Som(Coh($\varphi , \psi$ ))) :

a) Với mọi đỉnh $x$ của Coh($\varphi , \psi$ )$,k(x)$ nối $\eta (x)$ với $\eta '(x)$ ;

b) Với mọi cặp $(x, y)$ đỉnh của Coh($\varphi , \psi$ ) và mọi mũi tên $f\in$ Fl$_{x,y}$(Coh($\varphi , \psi$ )), ta có $\eta (f)k(y) =k(x)\eta '(f)$.

Theo Mệnh đề 2, chỉ cần kiểm tra điều kiện b) khi $f$ thuộc ảnh của Fl($\alpha$ ) hoặc thuộc ảnh của $h$, vì thế b) tương đương với phép hội của hai điều kiện c) và d) dưới đây:

c) Với $x\in$ Som(G), $y\in$ Som(G) và $g\in$ Fl$_{x,y}(G)$, ta có $\eta (\alpha (g))k(y) =k(x)\eta '(\alpha (g))$;

d) Với mọi $a\in$ Som(H), ta có $\eta (h(a))k(\psi (a)) =k(\varphi (a))\eta '(h(a))$. Điều kiện (i) tương đương với phép hội của a) và c), và điều kiện (ii) là điều kiện d), do đó hệ quả.

### 4. So sánh hai cohomotopiser

Xét một biểu đồ

H $^{\varphi}$ G

$$
u^{\psi}_v \tag{4}
$$

$$
{H'}^{\varphi'}_{\psi'}G'
$$

trong đó H, $H'$, G, $G'$ là các groupoid và $u,v,\varphi ,\psi ,\varphi ',\psi '$ là các cấu xạ groupoid sao cho $v\circ \varphi =\varphi '\circ u$ và $v\circ \psi =\psi '\circ u$.

Ký hiệu $\alpha$ là cấu xạ chính tắc từ G vào cohomotopiser Coh($\varphi , \psi$ ) và $h$ là phép đồng luân chính tắc nối $\alpha \circ \varphi$ với $\alpha \circ \psi$; định nghĩa $\alpha '$ và $h'$ tương tự. Khi đó $\alpha '\circ v$ là một cấu xạ groupoid từ G vào Coh($\varphi ', \psi '$) và $h'\circ$ Som($u$) là một phép đồng luân nối $\alpha '\circ \varphi '\circ u$ với $\alpha '\circ \psi '\circ u$, nghĩa là nối $\alpha '\circ v\circ \varphi$ với $\alpha '\circ v\circ \psi$. Theo tính chất phổ quát của các cohomotopiser (II, p. 185, Mệnh đề 3), tồn tại một cấu xạ duy nhất của groupoid $w$ từ Coh($\varphi , \psi$ ) vào Coh($\varphi ', \psi '$) sao cho $w\circ \alpha =\alpha '\circ v$ và Fl($w$)$\circ h=h'\circ$ Som($u$). Đặc biệt, ta đã mở rộng biểu đồ (4) thành một biểu đồ

H $^{\varphi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )

$$
u^{\psi}_vw \tag{5}
$$

${H'}^{\varphi'}_{\psi'}{G'}^{\alpha'}$ Coh($\varphi ', \psi '$)

trong đó hình vuông thứ hai là giao hoán.

#### Định lý 1 {#ta-ii-s4-thm-1 .statement tag=01UF}

Đặt các giả thiết sau:

(i) cấu xạ groupoid $v$ là một homotopism;

(ii) ánh xạ Orb($u$)$:$ Orb(H) $\rightarrow$ Orb(H$'$), suy ra từ $u$ bằng cách chuyển qua quỹ đạo, là song ánh;

(iii) trong mỗi quỹ đạo của H tồn tại một điểm $a$ sao cho đồng cấu $u_a: H_a\rightarrow H'_{u(a)}$ là toàn ánh.

Khi đó, cấu xạ nhóm vị $w:$ Coh($\varphi , \psi$ )$\rightarrow$ Coh($\varphi ', \psi '$) là một đồng luân cấu.

Gọi $G''$ là nhóm vị suy ra từ $G'$ bằng cách co các mũi tên của một rừng định hướng cực đại. Cấu xạ chính tắc $v': G'\rightarrow G''$ là một đồng luân cấu (II, p. 184, hệ quả 2 của mệnh đề 1). Hai biểu đồ

H $^{\varphi}$ G ${H'}^{\varphi'}G'$

$u\psi v'\circ v$ và Id$_{H'}\psi 'v'$

$$
H'vv''\circ \circ \psi \varphi ''G'H'vv''\circ \circ \psi \varphi ''G''
$$

sinh ra các cấu xạ nhóm vị $w'_1:$ Coh($\varphi , \psi$ )$\rightarrow$ Coh($v'\circ \varphi ', v'\circ \psi '$) và $w'_2:$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($v'\circ \varphi ', v'\circ \psi '$) ; ta có $w'_1=w'_2\circ w$. Do đó chỉ cần chứng minh rằng $w'_1$ và $w'_2$ là các đồng luân cấu. Vì các ánh xạ Som($v'\circ v$)$:$ Som(G) $\rightarrow$ Som(G$''$) và Som($v'$)$:$ Som(G$'$)$\rightarrow$ Som(G$''$) là toàn ánh, nên do đó chỉ cần chứng minh định lý dưới giả thiết bổ sung rằng ánh xạ Som($v$) là toàn ánh, một giả thiết mà ta sẽ giả sử trong toàn bộ phần còn lại của chứng minh.

Ta sẽ lần lượt chứng minh các khẳng định sau:

– Ánh xạ Orb($w$) là song ánh;

– Với mọi đỉnh $a$ của G, đồng cấu $w_a$ là toàn ánh;

– Với mọi đỉnh $a$ của G, đồng cấu $w_a$ là đơn ánh.

a) Theo giả thiết, ánh xạ Orb($u$) là song ánh; điều tương tự cũng đúng với ánh xạ Orb($v$) theo II, p. 182, mệnh đề 1, vì $v$ là một đồng luân cấu. Do đó cấu xạ của các quiver từ khung của cặp $(\varphi , \psi )$ tới khung của cặp $(\varphi ', \psi ')$ được xác định bởi các ánh xạ Orb($u$) và Orb($v$) là một đẳng cấu. Đặc biệt, ánh xạ suy ra từ đó khi chuyển qua các thành phần liên thông là song ánh. Mệnh đề 4 của II, p. 185 khi đó suy ra rằng ánh xạ Orb($w$) là song ánh.

(b) Gọi $f'$ là một mũi tên của $G'$, và ký hiệu $a'$ là gốc của nó và $b'$ là đích của nó. Vì ánh xạ Som($v$) là toàn ánh, tồn tại các đỉnh $a$ và $b$ trong G sao cho $a'=v(a)$ và $b'=v(b)$. Vì cấu xạ $v$ là một đồng luân cấu, tồn tại một mũi tên $f$ của G nối $a$ với $b$ và một phần tử $g\in G_a$ sao cho $v(g) =f'v(f)^{-1}($II, p. 182, prop. 1), do đó $f'=v(gf)$. Điều này chứng tỏ rằng ánh xạ Fl($v$) là toàn ánh.

Bây giờ ta chứng minh rằng ánh xạ Fl($w$) là toàn ánh. Ảnh của nó chứa ảnh của Fl($\alpha '$), vì ta có $\alpha '\circ v=w\circ \alpha$ và ánh xạ Fl($v$) là toàn ánh. Gọi $b$ là một đỉnh của $H'$; gọi $a$ là một đỉnh của H sao cho $b$ và $u(a)$ nằm trong cùng một quỹ đạo của $H'$, và gọi $f$ là một mũi tên của $H'$ nối $u(a)$ với $b$. Khi đó,

$$
h'(u(a))\cdot (\alpha '\circ \psi ')(f) = (\alpha '\circ \varphi ')(f)\cdot h'(b)
$$

vì $h'$ là một đồng luân nối $\alpha '\circ \varphi '$ với $\alpha '\circ \psi '$. Mũi tên $h'(u(a)) =$ $w(h(a))$ thuộc ảnh của Fl($w$), và hai mũi tên $\alpha '(\psi '(f))$ và $\alpha '(\varphi '(f))$ cũng vậy theo điều vừa nói trên. Suy ra mũi tên $h'(b)$ thuộc ảnh của Fl($w$), điều này chứng tỏ rằng ảnh của Fl($w$) chứa ảnh của $h'$. Theo mệnh đề 2 của II, p. 185, ánh xạ Fl($w$) là toàn ánh.

Lấy $g'\in$ Coh($\varphi ', \psi '$)$_{u(a)}$. Gọi $g$ là một mũi tên của Coh($\varphi , \psi$ ) sao cho $w(g) =g'$. Ký hiệu $x$ và $y$ là gốc và đích của $g$; ta có $u(x) =$ $u(y) =u(a)$. Gọi $g_1$ (tương ứng $g_2$) là một mũi tên của G nối $a$ với $x$ (tương ứng $a$ với $y$) mà ảnh của nó dưới $v$ là $e_{u(a)}$. Khi đó, $\alpha (g_1)g\alpha (g_2)^{-1}$ là một phần tử của Coh($\varphi , \psi$ )$_a$ mà ảnh của nó dưới $w_a$ là $g'$. Do đó, với mọi đỉnh $a$ của G, đồng cấu $w_a$ là toàn ánh.

c) Ta hãy chứng minh rằng, với mọi đỉnh $a$ của G, đồng cấu $w_a$ là đơn ánh. Bằng cách lần lượt xét các biểu đồ

$$\begin{array}{ccccccc} H & \underset{\psi}{\overset{\varphi}{\rightrightarrows}} & G & & H & \underset{v\circ\psi}{\overset{v\circ\varphi}{\rightrightarrows}} & G' \\ {\scriptstyle \mathrm{Id}_H}\big\downarrow & & \big\downarrow{\scriptstyle v} & \text{và} & {\scriptstyle u}\big\downarrow & & \big\downarrow{\scriptstyle \mathrm{Id}_{G'}} \\ H & \underset{v\circ\psi}{\overset{v\circ\varphi}{\rightrightarrows}} & G' & & H' & \underset{\psi'}{\overset{\varphi'}{\rightrightarrows}} & G' \end{array}$$

như vậy người ta được quy về việc xét hai trường hợp sau: 1) Ta có $H'= H$ và $u=$ Id$_H; 2)$ Ta có $G'= G$ và $v=$ Id$_G$.

1) Giả sử rằng ta có $H'= H$ và $u=$ Id$_H$.

Xét một cấu xạ groupoid $v': G'\rightarrow G$ là một nghịch đảo của $v$ theo nghĩa đồng luân và một đồng luân $k:$ Som(G) $\rightarrow$ Fl(G) nối $v'\circ v$ với Id$_G$. Theo Nhận xét 1 của II, p. 181, các ánh xạ $\alpha \circ k\circ \varphi$ và $\alpha \circ k\circ \psi$ là các đồng luân nối tương ứng $\alpha \circ v'\circ \varphi '$ với $\alpha \circ \varphi$ và $\alpha \circ v'\circ \psi '$ với $\alpha \circ \psi$. Do đó (xem II, p. 180), ánh xạ

$h_1:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )),

$$
x\mapsto (\alpha \circ k\circ \varphi )(x)\cdot h(x)\cdot ((\alpha \circ k\circ \psi )(x))^{-1}
$$

là một đồng luân nối $\alpha \circ v'\circ \varphi '$ với $\alpha \circ v'\circ \psi '$. Theo tính chất phổ quát của các cohomotoper (II, p. 185, prop. 3), tồn tại một cấu xạ groupoid duy nhất $w':$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($\varphi , \psi$ ) sao cho $\alpha \circ v'=$ $w'\circ \alpha '$ và $h_1=$ Fl($w'$)$\circ h'$.

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )

Id$_Hvw$

H $^{\varphi'}_{\psi'}{G'}^{\alpha'}$ Coh($\varphi ', \psi '$)

Id$_Hv'w'$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ ) .

Đặc biệt, ta có

$$
\alpha \circ v'\circ v=w'\circ \alpha '\circ v=w'\circ w\circ \alpha
$$

Vì $k$ là một đồng luân nối $v'\circ v$ với Id$_G,\alpha \circ k$ là một đồng luân nối $w'\circ w\circ \alpha$ với $\alpha$. Vì Fl($w'\circ w$)$\circ h=$ Fl($w'$)$\circ h'=h_1$, nên với mọi đỉnh $x$ của H,

Fl($w'\circ w$)$\circ h(x)\cdot (\alpha \circ k\circ \psi )(x) =h_1(x)\cdot (\alpha \circ k\circ \psi )(x) = (\alpha \circ k\circ \varphi )(x)\cdot h(x)$,

theo định nghĩa của $h_1$. Theo prop. 5 của II, p. 186, áp dụng cho các cấu xạ groupoid $w'\circ w$ và Id$_{Coh(\varphi ,\psi)}$, ánh xạ $\alpha \circ k$ là một đồng luân nối $w'\circ w$ với Id$_G$. Đặc biệt, $w'\circ w$ là một homotopism.

Do đó, với mọi đỉnh $a$ của G, đồng cấu nhóm $(w'\circ w)_a$ là song ánh (II, p. 182, prop. 1). Suy ra đồng cấu $w_a$ là đơn ánh, do đó cho kết quả trong trường hợp A).

2) Giả sử rằng ta có $G'= G$ và $v=$ Id$_G$.

Cho $x$ là một đỉnh của $H'$. Vì ánh xạ Orb($u$) là toàn ánh, tồn tại một đỉnh $a$ của H và một mũi tên $f$ của $H'$ nối $u(a)$ với $x$. Các mũi tên $\alpha (\varphi '(f))^{-1},h(a)$ và $\alpha (\psi '(f))$ lần lượt nối $\varphi '(x)$ với $\varphi '(u(a)) =\varphi (a),\varphi (a)$ với $\psi (a)$ và $\psi '(u(a)) =\psi (a)$ với $\psi '(x)$, và do đó khả hợp trong Coh($\varphi , \psi$ ). Đặt

$$
h_2(x) =\alpha (\varphi '(f))^{-1}\cdot h(a)\cdot \alpha (\psi '(f))
$$

Hãy kiểm tra rằng mũi tên thu được $h_2(x)$ không phụ thuộc vào các phần tử đã chọn $a$ và $f$. Cho $a'$ là một đỉnh của H và cho $f'$ là một mũi tên của $H'$ nối $u(a')$ với $x$. Vì ánh xạ Orb($u$) là đơn ánh, các đỉnh $a$ và $a'$ của H thuộc cùng một quỹ đạo và tồn tại một mũi tên $c\in$ Fl(H) nối $a$ với $a'$. Khi đó $u(c)f'f^{-1}$ là một vòng tại $u(a)$ trong $H'$. Theo giả thiết (iii), tồn tại một đỉnh $b$ của H sao cho đồng cấu $u_b$ là toàn ánh và một mũi tên $c'$ của H nối $b$ với $a$; khi đó, Int($u(c')$)$(u(c)f'f^{-1})$ là một vòng tại $u(b)$ trong H, và vì thế là ảnh qua $u_b$ của một vòng $c''$ tại $b$. Do đó, mũi tên $g= (c'c)^{-1}c''c'$ của H nối đỉnh $a'$ với đỉnh $a$ và thỏa mãn $f'=u(g)f$. Khi đó ta có

$$
\alpha (\varphi '(f'))^{-1}h(a')\alpha (\psi '(f'))
$$

$$
=\alpha (\varphi '(f))^{-1}\alpha (\varphi '(u(g)))^{-1}h(a')\alpha (\psi '(u(g)))\alpha (\psi '(f))
$$

$$
=\alpha (\varphi '(f))^{-1}\alpha (\varphi (g))^{-1}h(a')\alpha (\psi (g))\alpha (\psi '(f))
$$

$$
=\alpha (\varphi '(f))^{-1}\cdot h(a)\cdot \alpha (\psi '(f))
$$

vì $h$ là một đồng luân nối $\alpha \circ \varphi$ với $\alpha \circ \psi$. Điều này chứng minh tính độc lập đã được thông báo.

Theo phép dựng, ta có $h_2(u(x)) =h(x)$ với mọi $x\in$ Som(H). Do đó ta đã xác định một ánh xạ $h_2$ từ Som(H$'$) vào Fl(Coh($\varphi , \psi$ )). Gọi $c$ là một mũi tên của $H'$, và gọi $x$ là gốc của nó và $y$ là ngọn của nó. Gọi $a$ là một đỉnh của H và $f$ là một mũi tên của $H'$ nối $u(a)$ với $x$. Khi đó $f c$ là một mũi tên của $H'$ nối $u(a)$ với $y$. Theo định nghĩa của $h_2$, do đó ta có

$$
h_2(x)\alpha (\psi '(c)) =\alpha (\varphi '(f))^{-1}h(a)\alpha (\psi '(f))\alpha (\psi '(c))
$$

$$
=\alpha (\varphi '(c))\alpha (\varphi '(f c))^{-1}h(a)\alpha (\psi '(f c))
$$

$$
=\alpha (\varphi '(c))h_2(y)
$$

Điều này chứng tỏ rằng $h_2$ là một đồng luân nối $\alpha \circ \varphi '$ với $\alpha \circ \psi '$.

Theo tính chất phổ quát của các cohomotopizer, tồn tại một cấu xạ duy nhất của groupoid $w':$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($\varphi , \psi$ ) sao cho $w'\circ \alpha '=\alpha$ và $h_2$ = Fl($w'$)$\circ h'$. Ta có $w'\circ w\circ \alpha =w'\circ \alpha '=\alpha$ và Fl($w'\circ w$)$\circ h=$ Fl($w'$)$\circ h'\circ$ Som($u$) $=h_2\circ u=h$ theo định nghĩa của $h_2$. Theo tính chất phổ quát của các cohomotopizer, điều đó suy ra rằng ta có $w'\circ w=$ Id$_{Coh(\varphi ,\psi)}$. Đặc biệt, với mọi $a\in$ Som(G), đồng cấu $w_a$ là đơn ánh.

Khi đó suy ra từ Mệnh đề 1 của II, p. 182 rằng cấu xạ $w$ là một homotopism, do đó định lý được chứng minh.

### 5. Các Nhóm Đẳng Hướng của một Cohomotopizer

Gọi G và H là các groupoid, và gọi $\varphi ,\psi$ là các cấu xạ groupoid từ H vào G. Mục đích của số này là tính các nhóm đẳng hướng của cohomotopizer Coh($\varphi , \psi$ ). Ta lại dùng các ký hiệu $G_1, h_1, \theta_1, \alpha , h$ của số $^o3$.

Gọi $\Gamma_0$ là khung của cặp $(\varphi , \psi )$; xin nhắc lại (II, p. 185, Định nghĩa 3) rằng đó là quiver (Orb(G), Orb(H)$, \varphi_0, \psi_0$), trong đó $\varphi_0$ và $\psi_0$ là các ánh xạ từ Orb(H) vào Orb(G) suy ra từ các ánh xạ $\varphi$ và $\psi$ bằng cách chuyển qua các quỹ đạo.

Trong tất cả những gì tiếp theo trong số này, hơn nữa ta sẽ giả sử rằng quiver $\Gamma_0$ là liên thông và khác rỗng; theo II, p. 185, Mệnh đề 4, điều này tương đương với việc giả sử rằng groupoid Coh($\varphi , \psi$ ) là bắc cầu, hay cũng tương đương với việc quiver $G_1$ là liên thông và khác rỗng (II, p. 185, Mệnh đề 2).

#### Định nghĩa 4 {#ta-ii-s4-def-4 .statement tag=01UG}

Một trang bị nền của cặp $(\varphi , \psi )$ được nói là được cho bởi dữ liệu:

(i) Với mọi $i\in$ Orb(G), một đỉnh $a(i)$ trong quỹ đạo $i$ của G;

(ii) Với mọi $j\in$ Orb(H), một đỉnh $b(j)$ trong quỹ đạo $j$ của H;

(iii) Với mọi $j\in$ Orb(H), các mũi tên $c_1(j)$ và $c_2(j)$ của G nối tương ứng $\varphi (b(j))$ với $a(\varphi_0(j))$ và $\psi (b(j))$ với $a(\psi_0(j))$;

(iv) Một đồ thị con có hướng T của khung $\Gamma_0$ mà đồ thị liên kết của nó là một cây cực đại của đồ thị $\widetilde{\Gamma}_0$;

(v) Một quỹ đạo $i_0$ của G.

Hãy chọn một trang bị nền $(a, b, c_1, c_2,T, i_0)$ của cặp $(\varphi , \psi )$. Ta định nghĩa một cấu xạ quiver $\tau_1$ của $\Gamma_0$ vào Grp(G$_1$) bằng cách đặt $\tau_1(i) =a(i)$ với $i\in$ Som(Γ$_0$) $=$ Orb(G) và

$$
\tau_1(j) =c_1(j)^{-1}\cdot h_1(b(j))\cdot c_2(j)
$$

với $j\in$ Fl(Γ$_0$) $=$ Orb(H). Ta sẽ ký hiệu bởi $\tau_0$ hợp thành của $\tau_1$ và cấu xạ chính tắc $\theta_1$ của Grp(G$_1$) vào Coh($\varphi , \psi$ ) ; đó là một cấu xạ quiver của $\Gamma_0$ vào Coh($\varphi , \psi$ ).

Với $i\in$ Orb(G), ta ký hiệu bởi $\alpha_i: G_{a(i)}\rightarrow$ Coh($\varphi , \psi$ )$_{a(i)}$ đồng cấu nhóm suy ra từ cấu xạ $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) bằng hạn chế vào các nhóm đẳng hướng tại $a(i)$.

Với $j\in$ Orb(H), ta ký hiệu

$\varphi_j=$ Int($c_1(j)$)$^{-1}\circ \varphi_{b(j)}: H_{b(j)}\rightarrow G_{a(\varphi_0(j))}$

và

$\psi_j=$ Int($c_2(j)$)$^{-1}\circ \psi_{b(j)}: H_{b(j)}\rightarrow G_{a(\psi_0(j))}$,

sao cho ta có, với mọi phần tử $f$ của $H_{b(j)}$,

(6) $\varphi_j(f) =c_1(j)^{-1}\varphi (f)c_1(j)$ và $\psi_j(f) =c_2(j)^{-1}\psi (f)c_2(j)$.

Với mỗi đỉnh $i$ của $\Gamma_0$, ta lại ký hiệu bởi $d_i$ lớp đường đi duy nhất nối $i_0$ với $i$ trong cây $\widetilde{T}$; nó được coi như một mũi tên của Grp(Γ$_0$). Khi đó ta ký hiệu bởi $\delta_i$ mũi tên của Coh($\varphi , \psi$ ) là ảnh của $d_i$ dưới cấu xạ chính tắc từ Grp(Γ$_0$) vào Coh($\varphi , \psi$ ) suy ra từ $\tau_0$; gốc của $\delta_i$ là $a(i_0)$, đích của nó là $a(i)$.

Cấu xạ quiver $\tau_0$, các đồng cấu nhóm $\alpha_i$ (với $i\in$ Orb(G))$,\varphi_j$ và $\psi_j$ (với $j\in$ Orb(H)), và các mũi tên $\delta_i$ trong Coh($\varphi , \psi$ ) (với $i\in$ Orb(G)) sẽ được gọi là được suy ra từ trang bị cơ bản.

Nếu $(G_i)_{i\in I}$ là một họ các nhóm, ta ký hiệu bởi $_i*_{\in I}G_i$ tích tự do của chúng; ảnh của một phần tử $g\in G_i$ dưới ánh xạ chính tắc từ $G_i$ vào $_i*_{\in I}G_i$ sẽ được ký hiệu bởi $[g]$, hoặc thậm chí bởi $g$ nếu không thể có sự nhầm lẫn nào. Nếu S là một tập hợp, ta ký hiệu bởi F(S) nhóm tự do được xây dựng trên S (A, I, p. 84).

#### Mệnh đề 6 {#ta-ii-s4-prop-6 .statement tag=01UH}

Tồn tại một đồng cấu nhóm duy nhất

$\Lambda :(*G_{a(i)})*$ F(Orb(H)) $\rightarrow$ Coh($\varphi , \psi$ )$_{a(i_0)}$

$i\in$Orb(G)

sao cho

(7) $\Lambda (f) =\delta_i\alpha_i(f)\delta_i^{-1}$ với $i\in$ Orb(G) và $f\in G_{a(i)}$,

(8) $\Lambda (j) =\delta_{\varphi_0(j)}\tau_0(j)\delta^{-1}_{\psi_0(j)}$ với $j\in$ Orb(H).

Đồng cấu Λ là toàn ánh; hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của $(*_iG_{a(i)})*$ F(Orb(H)) chứa các phần tử $j$ của Fl(T) và các phần tử $\varphi_j(f)j\psi_j(f)^{-1}j^{-1}$, với $j\in$ Orb(H) và $f\in H_{b(j)}$.

Sự tồn tại và tính duy nhất của đồng cấu Λ là hệ quả của tính chất phổ quát của các tích tự do và các nhóm tự do (A, I, p. 85, prop. 8).

Gọi A là tập hợp các $a(i)$ với $i\in$ Orb(G) và $G_A$ là groupoid con đầy đủ của G mà tập hợp các đỉnh là A. Với mọi $x\in$ Som(G), gọi $\overline{x}$ là quỹ đạo của $x$ trong G và chọn một mũi tên $d_x$ của G nối $x$ với $a(\overline{x})$. Cặp $v$ tạo bởi ánh xạ $x\mapsto a(\overline{x})$ từ Som(G) vào A và ánh xạ gán cho $f\in$ Fl$_{x,y}(G)$ phần tử $d^{-1}_xf d_y$ của Fl$_{a(\overline{x}),a(\overline{y})}(G_A)$ là một cấu xạ groupoid. Suy ra từ Mệnh đề 1 của II, p. 182 rằng $v$ là một homotopism. Đặt $\varphi '=v\circ \varphi$ và $\psi '=v\circ \psi$, rồi gọi $w$ là cấu xạ chính tắc từ Coh($\varphi , \psi$ ) vào Coh($\varphi ', \psi '$) ; đó là một homotopism (II, p. 187, Định lý 1).

Các quỹ đạo của $G_A$ là các tập hợp $\{a\}$, với $a\in A$, và đơn ánh $G_A\rightarrow G$ cảm sinh một song ánh từ Orb(G$_A$) lên Orb(G), nhờ đó ta sẽ đồng nhất hai tập hợp này. Người ta xác định một trang bị cơ sở $(a', b', \beta '_1, \beta '_2,T', i_0)$ của cặp $(\varphi ', \psi ')$ bằng cách đặt $a'(i) =a(i)$ với $i\in$ Orb(G)$,b'(j) =b(j),\beta '_1(j) =v(c_1(j)),\beta '_2(j) =v(c_2(j))$ với $j\in$ Orb(H) và $T'= T$. Các đồng cấu nhóm $\varphi '_j$ và $\psi '_j$ (với $j\in$ Orb(H)), cấu xạ đồ thị có hướng $\tau '_0$, các mũi tên $\delta '_i$ (với $i\in$ Orb(G)), và do đó đồng cấu nhóm $\Lambda '$, suy ra từ trang bị cơ sở này, là các hợp thành với $w$ của các đồng cấu tương ứng $\varphi_j,\psi_j$, của cấu xạ đồ thị có hướng $\tau_0$, của các mũi tên tương ứng $\delta_i$ và của đồng cấu Λ.

Cho B là tập hợp các $b(j)$ với $j\in$ Orb(H), gọi $H_B$ là groupoid con đầy đủ của H có tập đỉnh là B; ký hiệu $u: H_B\rightarrow H$ là đơn ánh chính tắc; đặt $\varphi ''=\varphi '\circ u$ và $\psi ''=\psi '\circ u$. Cấu xạ $u$ cảm sinh một song ánh B $\rightarrow$ Orb(H), nhờ đó ta sẽ đồng nhất hai tập hợp này. Từ định lý 1 của II, p. 187 còn suy ra được một đồng luân cấu chính tắc $w':$ Coh($\varphi '', \psi ''$)$\rightarrow$ Coh($\varphi ', \psi '$). Hơn nữa, cặp $(\varphi '', \psi '')$ được trang bị một trang bị cơ sở $(a'', b'', \beta ''_1, \beta ''_2,T'', i_0)$, sao cho $\Lambda ', \varphi '_j, \psi '_j, \tau '_0, \delta '_i(i, i'\in$ Orb(G), $j\in$ Orb(H)) là các hợp thành với $w'$ của $\Lambda '', \varphi ''_j, \psi ''_j, \tau ''_0, \delta ''_i$.

Các cấu xạ groupoid khác nhau đã được đưa vào được tóm tắt bằng biểu đồ sau:

$H_{B\psi''}^{\varphi''}G_A^{\alpha''}$ Coh($\varphi '', \psi ''$)

$w'$

(9) H $^{\varphi'}G_A^{\alpha'}$ Coh($\varphi '', \psi ''$)

$\psi '$

$$
vw
$$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ ) .

Do đó, để chứng minh mệnh đề, ta có thể giả sử rằng A = Som(G) và B = Som(H), nói cách khác các ánh xạ chính tắc Som(G) $\rightarrow$ Orb(G) và Som(H) $\rightarrow$ Orb(H) là song ánh; trong phần còn lại của chứng minh, ta sẽ đặt mình dưới các giả thiết ấy.

Khi đó quiver $G_1$ có tập đỉnh là A và các mũi tên là tập hợp tổng của các tập hợp $G_a,a\in A$, và của tập hợp B. Các mũi tên của $G_a$ là các vòng tại $a$; nếu $b\in B$, mũi tên $b$ nối $\varphi (b)$ với $\psi (b)$, các mũi tên $c_1(b)$ và $c_2(b)$ lần lượt là các vòng tại $\varphi (b)$ và $\psi (b)$. Quiver T sẽ được đồng nhất với một cây có hướng của $G_1$; đó là một cây có hướng cực đại vì tập hợp các đỉnh của nó bằng tập hợp các đỉnh của $G_1($II, p. 157, mệnh đề 1). Ta đặt $a_0=a(i_0)$. Vì tập hợp các mũi tên của khung $\Gamma_0$ của cặp $(\varphi , \psi )$ được đồng nhất với B, cấu xạ của quiver $\tau_1: \Gamma_0\rightarrow$ Grp(G$_1$) gán cho mũi tên $b$ lớp các đường đi $c_1(b)^{-1}bc_2(b)$ trong đồ thị $\widetilde{G}_1$.

Nhắc lại rằng $\theta_1$ ký hiệu cấu xạ chính tắc của quiver từ $G_1$ vào Grp(G$_1$). Gọi

$\lambda :_a*_{\in A}F(G_a)*F(B)\rightarrow$ Grp(G$_1$)$_{a_0}$

là đồng cấu nhóm duy nhất sao cho ta có

$\lambda (f) =\tau_1(d_a)\theta_1(f)\tau_1(d_a)^{-1}$ nếu $a\in A$ và $f\in G_a$;

$\lambda (b) =\tau_1(d_{\varphi(b)})\tau_1(b)\tau_1(d_{\psi(b)})^{-1}$ nếu $b\in B$.

Do đó ta có $\lambda =\lambda '\circ \varepsilon$, trong đó $\lambda '$ kí hiệu đồng cấu nhóm chính tắc từ $_a*_{\in A}F(G_a)*F(B)$ vào Grp(G$_1$)$_{a_0}$ được xác định bởi cây định hướng cực đại T (II, p. 179, mệnh đề 9), và trong đó $\varepsilon$ là tự đẳng cấu duy nhất của nhóm $_a*_{\in A}F(G_a)*F(B)$ sao cho $\varepsilon (f) =f$ với $a\in A$ và $f\in G_a$, và $\varepsilon (b) =c_1(b)^{-1}h_1(b)c_2(b)$ với $b\in B$. Theo nhận xét 2 của II, p. 179, đồng cấu $\lambda$ là toàn ánh và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của $_a*_{\in A}F(G_a)*F(B)$ chứa các mũi tên của T.

Kí hiệu bởi $\pi :$ Grp(G$_1$)$\rightarrow$ Coh($\varphi , \psi$ ) cấu xạ groupoid chính tắc. Theo II, p. 177, hệ quả 1 của mệnh đề 8, đồng cấu nhóm $\pi_{a_0}$ từ Grp(G$_1$)$_{a_0}$ vào Coh($\varphi , \psi$ )$_{a_0}$ là toàn ánh, và hạt nhân của nó là nhóm con chuẩn tắc nhỏ nhất của Grp(G$_1$)$_{a_0}$ chứa các vòng Int($\tau_1(d_a)$)$(\alpha_1(f)\alpha_1(g)\alpha_1(f g)^{-1})$, với $a\in A$ và $f,g\in G_a$, và các vòng Int($\tau_1(d_{\varphi(b)})$)$(\varphi (f)b\psi (f)^{-1}b^{-1})$, với $b\in B$ và $f\in H_b$.

Nếu $p: F(\bigcup G_a\cup B)\rightarrow (_a*_{\in A}G_a)*F(B)$ kí hiệu đồng cấu toàn ánh chính tắc, thì do đó ta có $\Lambda \circ p=\pi_{a_0}\circ \lambda$. Công thức này suy ra rằng đồng cấu Λ là toàn ánh; còn phải xác định hạt nhân của nó.

Với $a\in A$ và $f\in G_a$, kí hiệu bởi $[f]$ ảnh của $f\in F(G_a)$ trong nhóm $_a*_{\in A}F(G_a)*F(B)$. Khi đó, với $a\in A,f, g\in G_a$, ta có

Int($\tau_1(d_a)$)$(\alpha_1(f)\alpha_1(g)\alpha_1(f g)^{-1}) =\lambda ([f][g][f g]^{-1})$.

Tương tự, với $b\in B$ và $f\in H_b$, định nghĩa của các đồng cấu $\varphi_b$ và $\psi_b$ (công thức (6) của II, p. 193) suy ra rằng ta có

Int($\tau_1(d_{\varphi(b)})$)$(\varphi (f)h_1(b)\psi (f)^{-1}h_1(b)^{-1})$

$$
=\tau_1(d_{\varphi(b)})\varphi (f)(c_1(b)\tau_1(b)c_2(b)^{-1})\psi (f)^{-1}
$$

$$
(c_2(b)\tau_1(b)^{-1}c_1(b)^{-1})\tau_1(d_{\varphi(b)})^{-1}
$$

$$
=\tau_1(d_{\varphi(b)})c_1(b)\varphi_b(f)\tau_1(b)\psi_b(f)^{-1}\tau_1(b)^{-1}c_1(b)^{-1}\tau_1(d_{\varphi(b)})^{-1}
$$

$$
=\lambda (c_1(b))\lambda (\varphi_b(f)[b]\psi_b(f)^{-1}[b]^{-1})\lambda (c_1(b))^{-1}
$$

Do đó, hạt nhân của đồng cấu $\pi_{a_0}\circ \lambda$ là nhóm con chuẩn tắc nhỏ nhất của $_a*_{\in A}F(G_a)*F(B)$ chứa các phần tử $[f][g][f g]^{-1}$ với $a\in A$ và $f,g\in G_a$, các phần tử $\varphi_b(f)[b]\psi_b(f)^{-1}[b]^{-1}$ với $b\in B$ và $f\in H_b$, và các phần tử $[b]$, với $b\in$ Fl(T).

Cuối cùng, hạt nhân của đồng cấu Λ là nhóm con chuẩn tắc nhỏ nhất của $(_a*_{\in A}G_a)*F(B)$ chứa các ảnh qua $p$ của các phần tử đi trước, nói cách khác, các phần tử $[b]$, với $b\in$ Fl(T), và các phần tử $\varphi_b(f)[b]\psi_b(f)[b]^{-1}$, với $b\in B$ và $f\in H_b$. Mệnh đề như vậy được chứng minh.
