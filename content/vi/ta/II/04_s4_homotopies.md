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
content_sha256: 18ed896787ceac7a0cce6966a70415c9fedd3ad124217db1afcd4e9384dba32d
translated_from: content/en-mt/ta/II/04_s4_homotopies.md
source_lang: en-mt
translation_method: machine
source_content_sha256: e32055ea451e7df87f25887fbf6aebc11fc734c7b092667a2f3abc000a796629
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-1aaff44f
glossary_version: 34
glossary_terms_sha256: df0a98704dd2ee9dd8c850d8f7398e80239cb4c5abf86392e3baf22d86fbbf9e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. ĐỒNG LUÂN

### 1. Định nghĩa về các phép đồng luân

#### Định nghĩa 1 {#ta-ii-s4-def-1 .statement tag=01U3}

Cho G là một groupoid, H là một quiver, $\varphi$ và $\varphi '$ là các đồng cấu của các quiver từ H vào G. Một phép đồng luân nối $\varphi$ với $\varphi '$ là một ánh xạ $h$ của tập hợp các đỉnh của H vào tập hợp các mũi tên của G có các tính chất sau:

(i) Với mọi đỉnh $a$ của H, mũi tên $h(a)$ có gốc $\varphi (a)$ và ngọn $\varphi '(a)$;

(ii) Với mọi mũi tên $f$ của H, có gốc $a$ và ngọn $b$, ta có $\varphi (f)h(b) =h(a)\varphi '(f)$.

Ta nói rằng $\varphi$ và $\varphi '$ là đồng luân nếu tồn tại một phép đồng luân nối $\varphi$ với $\varphi '$.

Cho G là một groupoid, cho H là một quiver và cho $\varphi ,\varphi ',\varphi ''$ là các đồng cấu của các quiver từ H vào G. Ánh xạ $a\mapsto e_{\varphi(a)}$ là một phép đồng luân nối $\varphi$ với $\varphi$. Nếu $h$ là một phép đồng luân nối $\varphi$ với $\varphi '$, ánh xạ $a\mapsto h(a)^{-1}$ là một phép đồng luân nối $\varphi '$ với $\varphi$. Cho $h$ và $h'$ lần lượt là các phép đồng luân nối $\varphi$ với $\varphi '$ và $\varphi '$ với $\varphi ''$. Với mọi đỉnh $a$ của H, các mũi tên $h(a)$ và $h'(a)$ có thể hợp thành. Ánh xạ $a\mapsto h(a)h'(a)$ là một phép đồng luân nối $\varphi$ với $\varphi ''$.

Suy ra rằng quan hệ “ $\varphi$ đồng luân với $\varphi '$ ” là một quan hệ tương đương trên tập hợp các đồng cấu của các quiver từ H vào G.

Cho G là một groupoid, H là một quiver và $\varphi ,\varphi '$ là các đồng cấu của các quiver từ H vào G đồng luân với nhau. Theo điều kiện (i) của Định nghĩa 1, với mọi đỉnh $a$ của H, các đỉnh $\varphi (a)$ và $\varphi '(a)$ thuộc cùng một quỹ đạo của G.

Giả sử thêm rằng H là một groupoid, và $h$ là một đồng luân nối $\varphi$ với $\varphi '$. Các ánh xạ Orb($\varphi$ ) và Orb($\varphi '$) suy ra từ $\varphi$ và $\varphi '$ bằng cách chuyển qua các quỹ đạo do đó bằng nhau. Với mọi đỉnh $a$ của H và mọi mũi tên $f\in H_a$, ta có $\varphi (f) =h(a)\varphi '(f)h(a)^{-1}=$ Int($h(a)$)$(\varphi '(f))$, theo điều kiện (ii) của Định nghĩa 1. Nói cách khác, đồng cấu $\varphi_a$ bằng Int($h(a)$)$\circ \varphi '_a$. Đặc biệt, nếu đồng cấu $\varphi_a$ là đơn ánh (resp. song ánh, resp. toàn ánh), thì điều tương tự cũng đúng với đồng cấu $\varphi '_a$.

#### Nhận xét 1 {#ta-ii-s4-n1-rem-1 .statement tag=01U4}

Cho G, $G'$ là các groupoid, H, $H'$ là các quiver, $u: H'\rightarrow H$ là một cấu xạ của các quiver và $v: G\rightarrow G'$ là một cấu xạ của các groupoid. Nếu các cấu xạ của các quiver $\varphi ,\varphi '$ từ H vào G là đồng luân, thì các cấu xạ của các quiver $v\circ \varphi \circ u$ và $v\circ \varphi '\circ u$ từ $H'$ vào $G'$ là đồng luân. Chính xác hơn, nếu $h$ là một đồng luân nối $\varphi$ với $\varphi '$, thì ánh xạ Fl($v$)$\circ h\circ$ Som($u$) là một đồng luân nối $v\circ \varphi \circ u$ với $v\circ \varphi '\circ u$.

#### Nhận xét 2 {#ta-ii-s4-n1-rem-2 .statement tag=01U5}

Cho G là một groupoid, H là một quiver, và $\varphi , \psi$ là các cấu xạ của các quiver từ H vào G. Ký hiệu $j$ là cấu xạ chính tắc của H vào Grp(H), và $\overline{\varphi}$ và $\overline{\psi}$ là các cấu xạ của các groupoid từ Grp(H) vào G sao cho $\overline{\varphi}\circ j=\varphi$ và $\overline{\psi}\circ j=\psi$.

Nhắc lại rằng Som(H) = Som(Grp(H)).

Một đồng luân $h:$ Som(H) $\rightarrow$ Fl(G) nối $\varphi$ với $\psi$ là một đồng luân nối $\overline{\varphi}$ với $\overline{\psi}$.

### 2. Các cấu xạ đồng luân của groupoid

Trong No$^o$ này, ta sẽ dùng ký hiệu $u\sim v$ để biểu thị rằng hai cấu xạ của các groupoid $u$ và $v$ là đồng luân.

#### Định nghĩa 2 {#ta-ii-s4-def-2 .statement tag=01U6}

Cho G, $G'$ là các groupoid và $\varphi$ là một cấu xạ từ G vào $G'$. Một nghịch đảo tới đồng luân của $\varphi$ là một cấu xạ groupoid $\psi$ từ $G'$ vào G sao cho các cấu xạ $\psi \circ \varphi$ và $\varphi \circ \psi$ lần lượt đồng luân với Id$_G$ và Id$_{G'}$. Người ta nói rằng $\varphi$ là một homotopism nếu tồn tại một nghịch đảo tới đồng luân của $\varphi$.

Một đẳng cấu của các groupoid là một homotopism.

Cho G và $G'$ là các groupoid. Cho $\varphi ,\varphi '$ là các cấu xạ groupoid từ G vào $G'$ và đồng luân với nhau. Nếu $\varphi$ là một homotopism thì $\varphi '$ cũng vậy. Thật vậy, nếu $\psi$ là một nghịch đảo của $\varphi$ tới đồng luân, ta có $\psi \circ \varphi '\sim \psi \circ \varphi \sim$ Id$_G$ và $\varphi '\circ \psi \sim \varphi \circ \psi \sim$ Id$_{G'}$, điều này chứng minh rằng $\psi$ là một nghịch đảo tới đồng luân của $\varphi '$.

Cho G, $G',G''$ là các groupoid và $\varphi : G\rightarrow G',\varphi ': G'\rightarrow G''$, $\psi : G'\rightarrow G,\psi ': G''\rightarrow G'$ là các cấu xạ groupoid. Khi đó, trong các điều kiện sau:

(i) $\psi$ là một nghịch đảo tới đồng luân của $\varphi$;

(ii) $\psi '$ là một nghịch đảo tới đồng luân của $\varphi '$;

(iii) $\psi \circ \psi '$ là một nghịch đảo tới đồng luân của $\varphi '\circ \varphi$; bất kỳ hai điều kiện nào kéo theo điều kiện thứ ba. Thật vậy, trước hết giả sử (i) và (ii) được thỏa mãn; khi đó ta có

$\psi \circ \psi '\circ \varphi '\circ \varphi \sim \psi \circ$ Id$_{G'}\circ \varphi \sim \psi \circ \varphi \sim$ Id$_G$

và, tương tự, $\varphi '\circ \varphi \circ \psi \circ \psi '\sim$ Id$_{G'}$, do đó (iii). Nếu (i) và (iii) được thỏa mãn,

$\varphi '\circ \psi '\sim \varphi '\circ \varphi \circ \psi \circ \psi '\sim$ Id$_{G''}$

và

$\psi '\circ \varphi '\sim (\varphi \circ \psi )\circ \psi '\circ \varphi '\circ (\varphi \circ \psi )\sim \varphi \circ \psi \sim$ Id$_{G'}$,

do đó điều kiện (ii). Chứng minh rằng các điều kiện (ii) và (iii) kéo theo điều kiện (i) là tương tự.

Đặc biệt, nếu hai trong ba cấu xạ $\varphi ,\varphi ',\varphi '\circ \varphi$ là các homotopism thì cấu xạ thứ ba cũng vậy.

#### Mệnh đề 1 {#ta-ii-s4-prop-1 .statement tag=01U7}

Cho G, $G'$ là các groupoid, cho $\varphi$ là một cấu xạ từ G vào $G'$, và cho A là một tập con của tập hợp các đỉnh của G, giao với mọi quỹ đạo của G. Để $\varphi$ là một homotopism, điều kiện cần và đủ là các điều kiện sau được thỏa mãn:

(i) ánh xạ Orb($\varphi$ ) từ Orb(G) vào Orb(G$'$), suy ra từ $\varphi$ bằng cách chuyển qua các quỹ đạo, là song ánh;

(ii) với mọi $a\in A$, đồng cấu $\varphi_a: G_a\rightarrow G'_{\varphi(a)}$ là song ánh.

Giả sử trước hết rằng $\varphi$ là một homotopism và $\psi$ là một nghịch đảo của $\varphi$ tới đồng luân. Khi đó,

Orb($\psi$ )$\circ$ Orb($\varphi$ ) $=$ Orb($\psi \circ \varphi$ ) $=$ Orb(Id$_G$) $=$ Id$_{Orb(G)}$,

vì hai cấu xạ nhómoid đồng luân cảm sinh cùng một ánh xạ khi chuyển qua các quỹ đạo. Tương tự, Orb($\varphi$ )$\circ$ Orb($\psi$ ) $=$ Id$_{Orb(G')}$. Do đó ánh xạ Orb($\varphi$ ) là song ánh, do đó mệnh đề (i). Ta cũng có, với mọi đỉnh $a$ của G,

$$
\psi_{\varphi(a)}\circ \varphi_a= (\psi \circ \varphi )_a
$$

vì $\psi \circ \varphi$ đồng luân với Id$_G$, đồng cấu $(\psi \circ \varphi )_a$ là song ánh (cf. p. 180), nên $\varphi_a$ là đơn ánh và $\psi_{\varphi(a)}$ là toàn ánh. Đổi chỗ vai trò của $\varphi$ và $\psi$, ta thấy rằng $\varphi_a$ cũng là toàn ánh, do đó điều kiện (ii).

Giả sử bây giờ các điều kiện (i) và (ii) được thỏa mãn, và ta chứng minh rằng $\varphi$ là một phép đồng luân.

Trước hết, ta xét trường hợp mỗi quỹ đạo của $G'$ được thu gọn thành một điểm.

Với mỗi đỉnh $b$ của $G'$, chọn một đỉnh $u(b)$ của G thuộc A và có ảnh qua $\varphi$ là $b$. Điều này có thể thực hiện được vì ánh xạ Orb($\varphi$ ) là toàn ánh và A gặp mỗi quỹ đạo của G. Cho $f$ là một mũi tên của $G'$; theo giả thiết, ta có $o(f) =t(f)$; đặt $b=o(f)$ và $a=u(b)$. Theo điều kiện (ii), tồn tại duy nhất một mũi tên $v(f)\in G_a$ có ảnh qua $\varphi$ là $f$. Cặp $\psi = (u, v)$ là một cấu xạ nhómoid từ $G'$ vào G. Ta chứng minh rằng $\psi$ là nghịch đảo của $\varphi$ theo nghĩa đồng luân. Theo cách dựng $\psi$, ta đã có $\varphi \circ \psi =$ Id$_{G'}$.

Cho $x$ là một đỉnh của G. Đặt $a=\psi (\varphi (x))$; đây là một phần tử của A sao cho $\varphi (a) =\varphi (x)$. Vì Orb($\varphi$ ) là đơn ánh, $a$ thuộc quỹ đạo của $x$ trong G và tồn tại một mũi tên $f$ trong G nối $a$ với $x$. Khi đó mũi tên $h(x) =\psi (\varphi (f))^{-1}f$ nối $a$ với $x$ và ta có $\varphi (h(x)) =e_{\varphi(a)}$.

Ta hãy chứng minh rằng ánh xạ $h:$ Som(G) $\rightarrow$ Fl(G) thu được là một phép đồng luân nối $\psi \circ \varphi$ với Id$_G$. Điều kiện (i) của định nghĩa 1 được thỏa mãn theo phép dựng. Cho $f$ là một mũi tên của G$,x$ là gốc của nó và $y$ là số hạng của nó. Ta có $\varphi (x) =\varphi (y)$ ; đặt $a=\psi (\varphi (x)) =\psi (\varphi (y))$. Các mũi tên $h(x)f h(y)^{-1}$ và $\psi \circ \varphi (f)$ thuộc $G_a$ và đều có ảnh $\varphi (f)$ trong $G'_{\varphi(a)}$. Vì ánh xạ $\varphi_a$ là đơn ánh, ta có $h(x)f h(y)^{-1}=\psi \circ \varphi (f)$. Do đó điều kiện (ii) của định nghĩa 1 được thỏa mãn.

Bây giờ ta hãy chứng minh mệnh đề 1 trong trường hợp tổng quát. Cho X là một rừng định hướng cực đại của $G'($II, p. 157, prop. 1). Cho $G''$ là groupoid suy ra từ $G'$ bằng phép co các mũi tên của X và cho $\varphi ': G'\rightarrow G''$ là cấu xạ chính tắc. Cấu xạ $\varphi '$ thỏa mãn các điều kiện của prop. 1 (II, p. 170, nhận xét 1 và p. 178, hệ quả 2), và do đó điều tương tự cũng đúng với cấu xạ $\varphi '\circ \varphi$.

Vì các quỹ đạo của $G''$ đều suy biến thành các điểm, từ trường hợp đặc biệt đã được chứng minh suy ra rằng $\varphi '$ và $\varphi '\circ \varphi$ là các phép đồng luân, do đó $\varphi$ cũng là một phép như vậy. Điều này hoàn tất chứng minh mệnh đề.

#### Hệ quả 1 {#ta-ii-s4-prop-1-cor-1 .statement tag=01U8}

Cho G là một groupoid, cho A là một tập hợp và cho $f: A\rightarrow$ Som(G) là một ánh xạ. Nếu ảnh của $f$ gặp mỗi quỹ đạo của G, thì cấu xạ groupoid chính tắc $\varphi$ của $f^*G$ vào G là một phép đồng luân.

Theo định nghĩa của groupoid ảnh ngược (II, p. 166, ví dụ 4), A là tập hợp các đỉnh của groupoid $f^*G$ và ta có Fl$_{a,b}(f^*G) =$ Fl$_{f(a),f(b)}(G)$ với mọi cặp $(a, b)$ các phần tử của A. Hơn nữa, ta có Som($\varphi$ ) $=f$ và Fl($\varphi$ ) cảm sinh ánh xạ đồng nhất từ Fl$_{a,b}(f^*G)$ vào Fl$_{f(a),f(b)}(G)$. Do đó, ánh xạ Orb($\varphi$ ) là song ánh và đồng cấu $\varphi_a: (f^*G)_a\rightarrow G_{f(a)}$ là một đẳng cấu, với mọi $a\in A$. Vì vậy, các giả thiết của mệnh đề 1 được thỏa mãn.

#### Hệ quả 2 {#ta-ii-s4-prop-1-cor-2 .statement tag=01U9}

Cho G là một groupoid, cho X là một rừng định hướng của G, cho $G'$ là groupoid suy ra từ G bằng phép co các mũi tên của X. Cấu xạ chính tắc của G vào $G'$ là một phép đồng luân.

Thực vậy, từ nhận xét 1 của II, p. 170 và hệ quả 2 của II, p. 178 suy ra rằng các giả thiết của mệnh đề 1 được thỏa mãn.

### 3. Cohomotoper

Cho H là một quiver, cho G là một groupoid và cho $\varphi$ và $\psi$ là các cấu xạ quiver của H vào G.

Gọi $G_1$ là khuyên được định nghĩa như sau: các đỉnh của $G_1$ là các đỉnh của G; các mũi tên của $G_1$ là các phần tử của tổng của các tập hợp Fl(G) và Som(H); ánh xạ gốc của $G_1$ trùng với ánh xạ gốc của G trên Fl(G) và với Som($\varphi$ ) trên Som(H); ánh xạ số hạng của $G_1$ trùng với ánh xạ số hạng của G trên Fl(G) và với Som($\psi$ ) trên Som(H). Gọi $\alpha_1$ là cấu xạ khuyên từ G vào $G_1$ được xác định bởi ánh xạ đồng nhất của Som(G) và bởi đơn ánh chính tắc của Fl(G) vào Fl(G$_1$). Gọi $h_1$ là đơn ánh chính tắc Som(H) $\rightarrow$ Fl(G$_1$).

Xét groupoid tự do Grp(G$_1$) được dựng trên $G_1($II, p. 174, def. 9), và gọi $\theta_1$ là cấu xạ khuyên chính tắc của $G_1$ vào Grp(G$_1$). Cuối cùng, ký hiệu Coh($\varphi , \psi$ ) là groupoid suy ra từ Grp(G$_1$) bằng cách co các vòng (tại gốc của $x$)

$$
\alpha_1(x)\alpha_1(y)\alpha_1(xy)^{-1} \tag{1}
$$

với mọi cặp $(x, y)$ các mũi tên khả hợp của G, cũng như các vòng (tại $\varphi (a)$)

$$
\alpha_1(\varphi (f))h_1(b)\alpha_1(\psi (f))^{-1}h_1(a)^{-1} \tag{2}
$$

với $a,b$ thuộc Som(H) và $f\in$ Fl$_{ab}(H)$. Gọi $\pi :$ Grp(G$_1$)$\rightarrow$ Coh($\varphi , \psi$ ) là cấu xạ chính tắc; đặt $\alpha$ = $\pi \circ \theta_1\circ \alpha_1$ và $h=$ Fl($\pi \circ \theta_1$)$\circ h_1$.

#### Mệnh đề 2 {#ta-ii-s4-prop-2 .statement tag=01UA}

Groupoid Coh($\varphi , \psi$ ) được sinh bởi khuyên con có tập hợp các đỉnh là Som(G) và có tập hợp các mũi tên là hợp của các ảnh của các ánh xạ Fl($\alpha$ ) và $h$.

Vì khuyên con này là ảnh của khuyên $G_1$ qua cấu xạ khuyên $\pi \circ \theta_1$, mệnh đề suy ra ngay từ phép dựng của Coh($\varphi , \psi$ ).

#### Mệnh đề 3 {#ta-ii-s4-prop-3 .statement tag=01UB}

Cấu xạ khuyên $\alpha$ là một cấu xạ groupoid từ G vào Coh($\varphi , \psi$ ), và ánh xạ $h$ là một đồng luân nối $\alpha \circ \varphi$ với $\alpha \circ \psi$.

Bộ ba (Coh($\varphi , \psi$ )$, $\alpha$ , $h$) có tính chất phổ quát sau: nếu $G'$ là một groupoid, $\alpha '$ là một cấu xạ của các groupoid từ G vào $G'$ và $h':$ Som(H) $\rightarrow$ Fl(G$'$) là một đồng luân nối $\alpha '\circ \varphi$ với $\alpha '\circ \psi$, thì tồn tại một cấu xạ duy nhất của các groupoid $\eta :$ Coh($\varphi , \psi$ )$\rightarrow G'$ sao cho

(3) $\alpha '=\eta \circ \alpha$ và $h'=$ Fl($\eta$ )$\circ h$.

Theo định nghĩa của groupoid suy ra bởi phép co các mũi tên, phép co các vòng (1) kéo theo rằng $\alpha$ là một cấu xạ của các groupoid, và phép co các vòng (2) kéo theo rằng $h$ là một đồng luân nối $\alpha \circ \varphi$ với $\alpha \circ \psi$.

Cho $G',\alpha ',h'$ như trong mệnh đề. Gọi $\eta_1$ là cấu xạ của các quiver từ $G_1$ vào $G'$ sao cho Som($\eta_1$) bằng Som($\alpha '$) và sao cho Fl($\eta_1$) trùng với Fl($\alpha '$) trên Fl(G) và với $h'$ trên Som(H). Tồn tại một cấu xạ duy nhất của các groupoid $\eta_2:$ Grp(G$_1$)$\rightarrow G'$ sao cho $\eta_1=\eta_2\circ \theta_1$. Vì $\alpha '$ là một cấu xạ của các groupoid và $h'$ là một đồng luân nối $\alpha '\circ \varphi$ với $\alpha '\circ \psi ,\eta_2$ xác định, bằng cách chuyển qua thương, một cấu xạ của các groupoid $\eta$ từ Coh($\varphi , \psi$ ) vào $G'($II, p. 170, mệnh đề 3). Cấu xạ này thỏa mãn các hệ thức (3), và nó là cấu xạ duy nhất (II, p. 185, mệnh đề 2).

#### Định nghĩa 3 {#ta-ii-s4-def-3 .statement tag=01UC}

Groupoid Coh($\varphi , \psi$ ) được gọi là cohomotopizer của cặp $(\varphi , \psi )$. Ta nói rằng $\alpha$ là cấu xạ chính tắc từ G vào Coh($\varphi , \psi$ ) và $h$ là đồng luân chính tắc nối $\alpha \circ \varphi$ với $\alpha \circ \psi$.

Quiver mà tập hợp các đỉnh của nó là tập hợp các quỹ đạo của G, tập hợp các mũi tên của nó là tập hợp các thành phần liên thông của H, và các ánh xạ gốc và ngọn của nó được suy ra từ $\varphi$ và $\psi$ bằng cách chuyển qua các thương được gọi là khung của cặp $(\varphi , \psi )$.

#### Mệnh đề 4 {#ta-ii-s4-prop-4 .statement tag=01UD}

Ánh xạ Orb($\alpha$ )$:$ Orb(G) $\rightarrow$ Orb(Coh($\varphi , \psi$ )) là toàn ánh; các thớ của nó là các thành phần liên thông của khung của cặp $(\varphi , \psi )$.

Cấu xạ $\alpha$ là hợp thành của các cấu xạ $\alpha_1: G\rightarrow G_1$, $\theta_1: G_1\rightarrow$ Grp(G$_1$) và $\pi :$ Grp(G$_1$)$\rightarrow$ Coh($\varphi , \psi$ ). Ánh xạ $\theta_1$ cảm sinh một song ánh từ tập hợp các thành phần liên thông của quiver $G_1$ lên tập hợp các quỹ đạo của Grp(G$_1$), và ánh xạ Orb($\pi$ )$:$ Orb(Grp(G$_1$))$\rightarrow$ Orb(Coh($\varphi , \psi$ )) là song ánh (II, p. 170, nhận xét 1). Do đó, chỉ cần chứng minh rằng ánh xạ từ Orb(G) vào $\pi_0(G_1)$ suy ra từ $\alpha_1$ là toàn ánh và các sợi của nó là các thành phần liên thông của khung của cặp $(\varphi , \psi )$. Tính toàn ánh suy ra từ sự kiện rằng ánh xạ Som($\alpha_1$) là ánh xạ đồng nhất. Quan hệ tương đương trong Som(G) được xác định bởi “$a$ và $b$ thuộc cùng một thành phần liên thông của $G_1$” được sinh bởi các quan hệ “tồn tại một mũi tên của G nối $a$ với $b$” và “tồn tại một đỉnh $h$ của H sao cho $\varphi (h) =a$ và $\psi (h) =b$”. Quan hệ tương đương này tương thích với ánh xạ từ Som(G) vào Orb(G), và quan hệ suy ra từ nó trong Orb(G) được sinh bởi quan hệ “tồn tại một quỹ đạo $\eta$ của H sao cho Orb($\varphi$ )$(\eta ) =\alpha$ và Orb($\psi$ )$(\eta ) =\beta$”. Do đó, nó chính là quan hệ “$\alpha$ và $\beta$ thuộc cùng một thành phần liên thông của khung của cặp $(\alpha , \beta )$”.

#### Mệnh đề 5 {#ta-ii-s4-prop-5 .statement tag=01UE}

Cho $G'$ là một groupoid, cho $\eta ,\eta '$ là các cấu xạ groupoid từ Coh($\varphi , \psi$ ) vào $G'$, và cho $k$ là một ánh xạ từ Som(G) vào Fl(G$'$). Để $k$ là một đồng luân nối $\eta$ với $\eta '$, điều kiện cần và đủ là hai điều kiện sau được thỏa mãn:

(i) Ánh xạ $k$ là một đồng luân nối $\eta \circ \alpha$ với $\eta '\circ \alpha$;

(ii) Với mọi đỉnh $a$ của H, ta có

$$
\eta (h(a))k(\psi (a)) =k(\varphi (a))\eta '(h(a))
$$

Theo định nghĩa, để $k$ là một đồng luân nối $\eta$ với $\eta '$, điều kiện cần và đủ là hai điều kiện sau được thỏa mãn (nhớ rằng Som(G) = Som(Coh($\varphi , \psi$ ))) :

a) Với mọi đỉnh $x$ của Coh($\varphi , \psi$ )$,k(x)$ nối $\eta (x)$ với $\eta '(x)$;

b) Với mọi cặp $(x, y)$ đỉnh của Coh($\varphi , \psi$ ) và mọi mũi tên $f\in$ Fl$_{x,y}$(Coh($\varphi , \psi$ )), ta có $\eta (f)k(y) =k(x)\eta '(f)$.

Theo Mệnh đề 2, chỉ cần kiểm tra điều kiện b) khi $f$ thuộc ảnh của Fl($\alpha$ ) hoặc ảnh của $h$, do đó b) tương đương với phép hội của hai điều kiện c) và d) dưới đây:

c) Với $x\in$ Som(G), $y\in$ Som(G) và $g\in$ Fl$_{x,y}(G)$, ta có $\eta (\alpha (g))k(y) =k(x)\eta '(\alpha (g))$;

d) Với mọi $a\in$ Som(H), ta có $\eta (h(a))k(\psi (a)) =k(\varphi (a))\eta '(h(a))$. Điều kiện (i) tương đương với phép hội của a) và c), còn điều kiện (ii) chính là điều kiện d), do đó có hệ quả.

### 4. So sánh hai cohomotopiser

Xét một biểu đồ

H $^{\varphi}$ G

$$
u^{\psi}_v \tag{4}
$$

$$
{H'}^{\varphi'}_{\psi'}G'
$$

trong đó H, $H'$, G, $G'$ là các groupoid và $u,v,\varphi ,\psi ,\varphi ',\psi '$ là các cấu xạ của groupoid sao cho $v\circ \varphi =\varphi '\circ u$ và $v\circ \psi =\psi '\circ u$.

Gọi $\alpha$ là cấu xạ chính tắc của G vào cohomotopiser Coh($\varphi , \psi$ ) và $h$ là phép đồng luân chính tắc nối $\alpha \circ \varphi$ với $\alpha \circ \psi$; định nghĩa $\alpha '$ và $h'$ tương tự. Khi đó $\alpha '\circ v$ là một cấu xạ của groupoid từ G vào Coh($\varphi ', \psi '$) và $h'\circ$ Som($u$) là một phép đồng luân nối $\alpha '\circ \varphi '\circ u$ với $\alpha '\circ \psi '\circ u$, nghĩa là nối $\alpha '\circ v\circ \varphi$ với $\alpha '\circ v\circ \psi$. Theo tính chất phổ quát của các cohomotopiser (II, p. 185, Mệnh đề 3), tồn tại một cấu xạ duy nhất của groupoid $w$ từ Coh($\varphi , \psi$ ) vào Coh($\varphi ', \psi '$) sao cho $w\circ \alpha =\alpha '\circ v$ và Fl($w$)$\circ h=h'\circ$ Som($u$). Đặc biệt, ta đã mở rộng biểu đồ (4) thành biểu đồ

H $^{\varphi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )

$$
u^{\psi}_vw \tag{5}
$$

${H'}^{\varphi'}_{\psi'}{G'}^{\alpha'}$ Coh($\varphi ', \psi '$)

trong đó bình phương thứ hai là giao hoán.

#### Định lý 1 {#ta-ii-s4-thm-1 .statement tag=01UF}

Đặt các giả thiết sau:

(i) cấu xạ của groupoid $v$ là một homotopism;

(ii) ánh xạ Orb($u$)$:$ Orb(H) $\rightarrow$ Orb(H$'$), suy ra từ $u$ bằng cách chuyển qua các quỹ đạo, là song ánh;

(iii) trong mỗi quỹ đạo của H tồn tại một điểm $a$ sao cho đồng cấu $u_a: H_a\rightarrow H'_{u(a)}$ là toàn ánh.

Sau đó, cấu xạ groupoid $w:$ Coh($\varphi , \psi$ )$\rightarrow$ Coh($\varphi ', \psi '$) là một phép đồng luân.

Cho $G''$ là groupoid suy ra từ $G'$ bằng phép co các mũi tên của một rừng có hướng cực đại. Cấu xạ chính tắc $v': G'\rightarrow G''$ là một phép đồng luân (II, p. 184, Hệ quả 2 của Mệnh đề 1). Hai sơ đồ

H $^{\varphi}$ G ${H'}^{\varphi'}G'$

$u\psi v'\circ v$ và Id$_{H'}\psi 'v'$

$$
H'vv''\circ \circ \psi \varphi ''G'H'vv''\circ \circ \psi \varphi ''G''
$$

cho các cấu xạ groupoid $w'_1:$ Coh($\varphi , \psi$ )$\rightarrow$ Coh($v'\circ \varphi ', v'\circ \psi '$) và $w'_2:$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($v'\circ \varphi ', v'\circ \psi '$) ; ta có $w'_1=w'_2\circ w$. Do đó, chỉ cần chứng minh rằng $w'_1$ và $w'_2$ là các phép đồng luân. Vì các ánh xạ Som($v'\circ v$)$:$ Som(G) $\rightarrow$ Som(G$''$) và Som($v'$)$:$ Som(G$'$)$\rightarrow$ Som(G$''$) là toàn ánh, do đó chỉ cần chứng minh định lý dưới giả thiết bổ sung rằng ánh xạ Som($v$) là toàn ánh, và ta sẽ giữ giả thiết này trong suốt phần còn lại của chứng minh.

Ta lần lượt chứng minh các khẳng định sau:

– Ánh xạ Orb($w$) là song ánh;

– Với mọi đỉnh $a$ của G, đồng cấu $w_a$ là toàn ánh;

– Với mọi đỉnh $a$ của G, đồng cấu $w_a$ là đơn ánh.

a) Theo giả thiết, ánh xạ Orb($u$) là song ánh; điều tương tự cũng đúng với ánh xạ Orb($v$) theo II, p. 182, Mệnh đề 1, vì $v$ là một phép đồng luân. Cấu xạ các quiver từ khung của cặp $(\varphi , \psi )$ đến khung của cặp $(\varphi ', \psi ')$ được xác định bởi các ánh xạ Orb($u$) và Orb($v$) do đó là một đẳng cấu. Đặc biệt, ánh xạ suy ra từ nó bằng cách chuyển qua các thành phần liên thông là song ánh. Mệnh đề 4 của II, p. 185 khi đó suy ra rằng ánh xạ Orb($w$) là song ánh.

5 sau đó suy ra rằng ánh xạ Orb($w$) là song ánh.

(b) Cho $f'$ là một mũi tên của $G'$, và ký hiệu $a'$ là điểm gốc của nó và $b'$ là số hạng của nó. Vì ánh xạ Som($v$) là toàn ánh, tồn tại các đỉnh $a$ và $b$ trong G sao cho $a'=v(a)$ và $b'=v(b)$. Vì cấu xạ $v$ là một đồng luân đẳng cấu, tồn tại một mũi tên $f$ của G nối $a$ với $b$ và một phần tử $g\in G_a$ sao cho $v(g) =f'v(f)^{-1}($II, p. 182, mệnh đề 1), do đó $f'=v(gf)$. Điều này chứng tỏ rằng ánh xạ Fl($v$) là toàn ánh.

Bây giờ hãy chứng minh rằng ánh xạ Fl($w$) là toàn ánh. Ảnh của nó chứa ảnh của Fl($\alpha '$), vì ta có $\alpha '\circ v=w\circ \alpha$ và ánh xạ Fl($v$) là toàn ánh. Cho $b$ là một đỉnh của $H'$; cho $a$ là một đỉnh của H sao cho $b$ và $u(a)$ nằm trong cùng một quỹ đạo của $H'$, và cho $f$ là một mũi tên của $H'$ nối $u(a)$ với $b$. Khi đó,

$$
h'(u(a))\cdot (\alpha '\circ \psi ')(f) = (\alpha '\circ \varphi ')(f)\cdot h'(b)
$$

vì $h'$ là một đồng luân nối $\alpha '\circ \varphi '$ với $\alpha '\circ \psi '$. Mũi tên $h'(u(a)) =$ $w(h(a))$ thuộc ảnh của Fl($w$), và hai mũi tên $\alpha '(\psi '(f))$ và $\alpha '(\varphi '(f))$ cũng vậy theo điều đã nói ở trên. Suy ra mũi tên $h'(b)$ thuộc ảnh của Fl($w$), điều này chứng tỏ rằng ảnh của Fl($w$) chứa ảnh của $h'$. Theo mệnh đề 2 của II, p. 185, ánh xạ Fl($w$) là toàn ánh.

Cho $g'\in$ Coh($\varphi ', \psi '$)$_{u(a)}$. Gọi $g$ là một mũi tên của Coh($\varphi , \psi$ ) sao cho $w(g) =g'$. Ký hiệu $x$ và $y$ lần lượt là điểm đầu và điểm cuối của $g$; ta có $u(x) =$ $u(y) =u(a)$. Gọi $g_1$ (resp. $g_2$) là một mũi tên của G nối $a$ với $x$ (resp. $a$ với $y$), có ảnh qua $v$ là $e_{u(a)}$. Khi đó, $\alpha (g_1)g\alpha (g_2)^{-1}$ là một phần tử của Coh($\varphi , \psi$ )$_a$ có ảnh qua $w_a$ là $g'$. Do đó, với mọi đỉnh $a$ của G, đồng cấu $w_a$ là toàn ánh.

c) Hãy chứng minh rằng, với mọi đỉnh $a$ của G, đồng cấu $w_a$ là đơn ánh. Bằng cách lần lượt xét các biểu đồ

$$\begin{array}{ccccccc} H & \underset{\psi}{\overset{\varphi}{\rightrightarrows}} & G & & H & \underset{v\circ\psi}{\overset{v\circ\varphi}{\rightrightarrows}} & G' \\ {\scriptstyle \mathrm{Id}_H}\big\downarrow & & \big\downarrow{\scriptstyle v} & \text{and} & {\scriptstyle u}\big\downarrow & & \big\downarrow{\scriptstyle \mathrm{Id}_{G'}} \\ H & \underset{v\circ\psi}{\overset{v\circ\varphi}{\rightrightarrows}} & G' & & H' & \underset{\psi'}{\overset{\varphi'}{\rightrightarrows}} & G' \end{array}$$

ta quy về xét hai trường hợp sau: 1) Có $H'= H$ và $u=$ Id$_H$; 2) Có $G'= G$ và $v=$ Id$_G$.

1) Giả sử $H'= H$ và $u=$ Id$_H$.

Xét một cấu xạ của các nhómoid $v': G'\rightarrow G$ là nghịch đảo của $v$ theo đồng luân và một đồng luân $k:$ Som(G) $\rightarrow$ Fl(G) nối $v'\circ v$ với Id$_G$. Theo Nhận xét 1 của II, p. 181, các ánh xạ $\alpha \circ k\circ \varphi$ và $\alpha \circ k\circ \psi$ lần lượt là các đồng luân nối $\alpha \circ v'\circ \varphi '$ với $\alpha \circ \varphi$ và $\alpha \circ v'\circ \psi '$ với $\alpha \circ \psi$. Do đó (xem II, p. 180), ánh xạ

$h_1:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )),

$$
x\mapsto (\alpha \circ k\circ \varphi )(x)\cdot h(x)\cdot ((\alpha \circ k\circ \psi )(x))^{-1}
$$

is một đồng luân nối $\alpha \circ v'\circ \varphi '$ với $\alpha \circ v'\circ \psi '$. Theo tính chất phổ quát của các cohomotoper (II, p. 185, prop. 3), tồn tại duy nhất một cấu xạ groupoid $w':$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($\varphi , \psi$ ) sao cho $\alpha \circ v'=$ $w'\circ \alpha '$ và $h_1=$ Fl($w'$)$\circ h'$.

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )

Id$_Hvw$

H $^{\varphi'}_{\psi'}{G'}^{\alpha'}$ Coh($\varphi ', \psi '$)

Id$_Hv'w'$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ ) .

Đặc biệt, ta có

$$
\alpha \circ v'\circ v=w'\circ \alpha '\circ v=w'\circ w\circ \alpha
$$

Vì $k$ là một đồng luân nối $v'\circ v$ với Id$_G,\alpha \circ k$ là một đồng luân nối $w'\circ w\circ \alpha$ với $\alpha$. Vì Fl($w'\circ w$)$\circ h=$ Fl($w'$)$\circ h'=h_1$, với mọi đỉnh $x$ của H, ta có

Fl($w'\circ w$)$\circ h(x)\cdot (\alpha \circ k\circ \psi )(x) =h_1(x)\cdot (\alpha \circ k\circ \psi )(x) = (\alpha \circ k\circ \varphi )(x)\cdot h(x)$,

theo định nghĩa của $h_1$. Theo mệnh đề 5 của II, p. 186, áp dụng cho các cấu xạ groupoid $w'\circ w$ và Id$_{Coh(\varphi ,\psi)}$, ánh xạ $\alpha \circ k$ là một đồng luân nối $w'\circ w$ với Id$_G$. Đặc biệt, $w'\circ w$ là một đồng luân đẳng cấu.

Với mọi đỉnh $a$ của G, đồng cấu nhóm $(w'\circ w)_a$ do đó là song ánh (II, p. 182, prop. 1). Suy ra đồng cấu $w_a$ là đơn ánh, do đó kết quả trong trường hợp A).

2) Giả sử rằng $G'= G$ và $v=$ Id$_G$.

Cho $x$ là một đỉnh của $H'$. Vì ánh xạ Orb($u$) là toàn ánh, tồn tại một đỉnh $a$ của H và một mũi tên $f$ của $H'$ nối $u(a)$ với $x$. Các mũi tên $\alpha (\varphi '(f))^{-1},h(a)$ và $\alpha (\psi '(f))$ lần lượt nối $\varphi '(x)$ với $\varphi '(u(a)) =\varphi (a),\varphi (a)$ với $\psi (a)$ và $\psi '(u(a)) =\psi (a)$ với $\psi '(x)$, và do đó có thể hợp thành trong Coh($\varphi , \psi$ ). Đặt

$$
h_2(x) =\alpha (\varphi '(f))^{-1}\cdot h(a)\cdot \alpha (\psi '(f))
$$

Ta hãy kiểm tra rằng mũi tên thu được $h_2(x)$ không phụ thuộc vào các phần tử $a$ và $f$ đã chọn. Cho $a'$ là một đỉnh của H và $f'$ là một mũi tên của $H'$ nối $u(a')$ với $x$. Vì ánh xạ Orb($u$) là đơn ánh, các đỉnh $a$ và $a'$ của H thuộc cùng một quỹ đạo và tồn tại một mũi tên $c\in$ Fl(H) nối $a$ với $a'$. Khi đó $u(c)f'f^{-1}$ là một vòng tại $u(a)$ trong $H'$. Theo giả thiết (iii), tồn tại một đỉnh $b$ của H sao cho đồng cấu $u_b$ là toàn ánh và một mũi tên $c'$ của H nối $b$ với $a$; khi đó, Int($u(c')$)$(u(c)f'f^{-1})$ là một vòng tại $u(b)$ trong H, và do đó là ảnh dưới $u_b$ của một vòng $c''$ tại $b$. Do đó, mũi tên $g= (c'c)^{-1}c''c'$ của H nối đỉnh $a'$ với đỉnh $a$ và thỏa mãn $f'=u(g)f$. Ta có

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

vì $h$ là một đồng luân nối $\alpha \circ \varphi$ với $\alpha \circ \psi$. Điều này chứng minh sự độc lập đã nêu.

Do phép dựng, ta có $h_2(u(x)) =h(x)$ với mọi $x\in$ Som(H). Do đó ta đã xác định một ánh xạ $h_2$ từ Som(H$'$) vào Fl(Coh($\varphi , \psi$ )). Cho $c$ là một mũi tên của $H'$, và gọi $x$ là điểm đầu của nó và $y$ là điểm cuối của nó. Cho $a$ là một đỉnh của H và $f$ là một mũi tên của $H'$ nối $u(a)$ với $x$. Khi đó $f c$ là một mũi tên của $H'$ nối $u(a)$ với $y$. Theo định nghĩa của $h_2$, do đó ta có

$$
h_2(x)\alpha (\psi '(c)) =\alpha (\varphi '(f))^{-1}h(a)\alpha (\psi '(f))\alpha (\psi '(c))
$$

$$
=\alpha (\varphi '(c))\alpha (\varphi '(f c))^{-1}h(a)\alpha (\psi '(f c))
$$

$$
=\alpha (\varphi '(c))h_2(y)
$$

Điều này chứng minh rằng $h_2$ là một đồng luân nối $\alpha \circ \varphi '$ với $\alpha \circ \psi '$.

Theo tính chất phổ quát của các cohomotopizer, tồn tại một cấu xạ duy nhất của các groupoid $w':$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($\varphi , \psi$ ) sao cho $w'\circ \alpha '=\alpha$ và $h_2$ = Fl($w'$)$\circ h'$. Ta có $w'\circ w\circ \alpha =w'\circ \alpha '=\alpha$ và Fl($w'\circ w$)$\circ h=$ Fl($w'$)$\circ h'\circ$ Som($u$) $=h_2\circ u=h$ theo định nghĩa của $h_2$. Theo tính chất phổ quát của các cohomotopizer, điều này suy ra rằng ta có $w'\circ w=$ Id$_{Coh(\varphi ,\psi)}$. Đặc biệt, với mọi $a\in$ Som(G), đồng cấu $w_a$ là đơn ánh.

Do đó, theo Mệnh đề 1 của II, p. 182, cấu xạ $w$ là một đồng luân đẳng cấu, do đó định lý được chứng minh.

### 5. Các nhóm đẳng hướng của một Cohomotopizer

Cho G và H là các groupoid, và cho $\varphi ,\psi$ là các cấu xạ của groupoid từ H vào G. Mục đích của n$^o$ này là tính các nhóm đẳng hướng của cohomotopizer Coh($\varphi , \psi$ ). Ta lại sử dụng các ký hiệu $G_1, h_1, \theta_1, \alpha , h$ của n$^o3$.

Gọi $\Gamma_0$ là khung của cặp $(\varphi , \psi )$; ta nhắc lại (II, p. 185, Đn. 3) rằng đây là quiver (Orb(G), Orb(H)$, \varphi_0, \psi_0$), trong đó $\varphi_0$ và $\psi_0$ là các ánh xạ từ Orb(H) vào Orb(G) suy ra từ các ánh xạ $\varphi$ và $\psi$ bằng cách chuyển qua các quỹ đạo.

Trong tất cả những gì tiếp theo trong Số này, hơn nữa ta giả sử rằng quiver $\Gamma_0$ là liên thông và khác rỗng; theo II, p. 185, Mệnh đề 4, điều này tương đương với việc giả sử groupoid Coh($\varphi , \psi$ ) là bắc cầu, hay cũng tương đương với việc quiver $G_1$ là liên thông và khác rỗng (II, p. 185, Mệnh đề 2).

#### Định nghĩa 4 {#ta-ii-s4-def-4 .statement tag=01UG}

Một trang bị cơ sở của cặp $(\varphi , \psi )$ được cho bởi các dữ liệu sau:

(i) Với mọi $i\in$ Orb(G), một đỉnh $a(i)$ trong quỹ đạo $i$ của G;

(ii) Với mọi $j\in$ Orb(H), một đỉnh $b(j)$ trong quỹ đạo $j$ của H;

(iii) Với mọi $j\in$ Orb(H), các mũi tên $c_1(j)$ và $c_2(j)$ của G lần lượt nối $\varphi (b(j))$ với $a(\varphi_0(j))$ và $\psi (b(j))$ với $a(\psi_0(j))$;

(iv) Một quiver con T của khung $\Gamma_0$ mà đồ thị liên kết của nó là một cây cực đại của đồ thị $\widetilde{\Gamma}_0$;

(v) Một quỹ đạo $i_0$ của G.

Ta chọn một trang bị cơ sở $(a, b, c_1, c_2,T, i_0)$ của cặp $(\varphi , \psi )$. Ta định nghĩa một cấu xạ quiver $\tau_1$ của $\Gamma_0$ vào Grp(G$_1$) bằng cách đặt $\tau_1(i) =a(i)$ với $i\in$ Som(Γ$_0$) $=$ Orb(G) và

$$
\tau_1(j) =c_1(j)^{-1}\cdot h_1(b(j))\cdot c_2(j)
$$

với $j\in$ Fl(Γ$_0$) $=$ Orb(H). Ta ký hiệu $\tau_0$ là hợp thành của $\tau_1$ và cấu xạ chính tắc $\theta_1$ của Grp(G$_1$) vào Coh($\varphi , \psi$ ) ; nó là một cấu xạ quiver của $\Gamma_0$ vào Coh($\varphi , \psi$ ).

Với $i\in$ Orb(G), ta ký hiệu $\alpha_i: G_{a(i)}\rightarrow$ Coh($\varphi , \psi$ )$_{a(i)}$ là đồng cấu nhóm suy ra từ cấu xạ $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) bằng cách hạn chế vào các nhóm đẳng hướng tại $a(i)$.

Với $j\in$ Orb(H), ta ký hiệu

$\varphi_j=$ Int($c_1(j)$)$^{-1}\circ \varphi_{b(j)}: H_{b(j)}\rightarrow G_{a(\varphi_0(j))}$

và

$\psi_j=$ Int($c_2(j)$)$^{-1}\circ \psi_{b(j)}: H_{b(j)}\rightarrow G_{a(\psi_0(j))}$,

sao cho, với mọi phần tử $f$ của $H_{b(j)}$,

(6) $\varphi_j(f) =c_1(j)^{-1}\varphi (f)c_1(j)$ và $\psi_j(f) =c_2(j)^{-1}\psi (f)c_2(j)$.

Với mỗi đỉnh $i$ của $\Gamma_0$, ta lại ký hiệu $d_i$ là lớp đường đi duy nhất nối $i_0$ với $i$ trong cây $\widetilde{T}$; nó được xem như một mũi tên của Grp(Γ$_0$). Khi đó ta ký hiệu $\delta_i$ là mũi tên của Coh($\varphi , \psi$ ) là ảnh của $d_i$ qua cấu xạ chính tắc từ Grp(Γ$_0$) vào Coh($\varphi , \psi$ ) suy ra từ $\tau_0$; gốc của $\delta_i$ là $a(i_0)$, ngọn của nó là $a(i)$.

Cấu xạ quiver $\tau_0$, các đồng cấu nhóm $\alpha_i$ (với $i\in$ Orb(G))$,\varphi_j$ và $\psi_j$ (với $j\in$ Orb(H)), và các mũi tên $\delta_i$ trong Coh($\varphi , \psi$ ) (với $i\in$ Orb(G)) được gọi là suy ra từ thiết bị cơ sở.

Nếu $(G_i)_{i\in I}$ là một họ các nhóm, ta ký hiệu $_i*_{\in I}G_i$ là tích tự do của chúng; ảnh của một phần tử $g\in G_i$ qua ánh xạ chính tắc từ $G_i$ vào $_i*_{\in I}G_i$ sẽ được ký hiệu là $[g]$, hoặc cũng là $g$ nếu không thể có sự nhầm lẫn. Nếu S là một tập hợp, ta ký hiệu F(S) là nhóm tự do được xây dựng trên S (A, I, p. 84).

#### Mệnh đề 6 {#ta-ii-s4-prop-6 .statement tag=01UH}

Tồn tại một đồng cấu nhóm duy nhất

$\Lambda :(*G_{a(i)})*$ F(Orb(H)) $\rightarrow$ Coh($\varphi , \psi$ )$_{a(i_0)}$

$i\in$Orb(G)

sao cho

(7) $\Lambda (f) =\delta_i\alpha_i(f)\delta_i^{-1}$ với $i\in$ Orb(G) và $f\in G_{a(i)}$,

(8) $\Lambda (j) =\delta_{\varphi_0(j)}\tau_0(j)\delta^{-1}_{\psi_0(j)}$ với $j\in$ Orb(H).

Đồng cấu nhóm Λ là toàn ánh; hạt nhân của nó là nhóm con chuẩn nhỏ nhất của $(*_iG_{a(i)})*$ F(Orb(H)) chứa các phần tử $j$ của Fl(T) và các phần tử $\varphi_j(f)j\psi_j(f)^{-1}j^{-1}$, với $j\in$ Orb(H) và $f\in H_{b(j)}$.

Tính tồn tại và tính duy nhất của đồng cấu nhóm Λ là hệ quả của tính chất phổ quát của các tích tự do và các nhóm tự do (A, I, p. 85, prop. 8).

Gọi A là tập hợp các $a(i)$ với $i\in$ Orb(G) và $G_A$ là nhóm con đầy đủ của G mà tập hợp các đỉnh là A. Với mọi $x\in$ Som(G), gọi $\overline{x}$ là quỹ đạo của $x$ trong G và chọn một mũi tên $d_x$ của G nối $x$ với $a(\overline{x})$. Cặp $v$ được tạo thành bởi ánh xạ $x\mapsto a(\overline{x})$ của Som(G) vào A và ánh xạ mà với $f\in$ Fl$_{x,y}(G)$ tương ứng phần tử $d^{-1}_xf d_y$ của Fl$_{a(\overline{x}),a(\overline{y})}(G_A)$ là một cấu xạ nhóm. Theo Mệnh đề 1 của II, p. 182, suy ra $v$ là một đồng luân cấu. Đặt $\varphi '=v\circ \varphi$ và $\psi '=v\circ \psi$, rồi đặt $w$ là cấu xạ chính tắc của Coh($\varphi , \psi$ ) vào Coh($\varphi ', \psi '$) ; đó là một đồng luân cấu (II, p. 187, Định lý 1).

Các quỹ đạo của $G_A$ là các tập hợp $\{a\}$, với $a\in A$, và đơn ánh $G_A\rightarrow G$ cảm sinh một song ánh từ Orb(G$_A$) lên Orb(G), qua đó ta đồng nhất hai tập hợp này. Ta định nghĩa một trang bị cơ bản $(a', b', \beta '_1, \beta '_2,T', i_0)$ của cặp $(\varphi ', \psi ')$ bằng cách đặt $a'(i) =a(i)$ với $i\in$ Orb(G)$,b'(j) =b(j),\beta '_1(j) =v(c_1(j)),\beta '_2(j) =v(c_2(j))$ với $j\in$ Orb(H) và $T'= T$. Các đồng cấu nhóm $\varphi '_j$ và $\psi '_j$ (với $j\in$ Orb(H)), cấu xạ quiver $\tau '_0$, các mũi tên $\delta '_i$ (với $i\in$ Orb(G)), và do đó đồng cấu nhóm $\Lambda '$, suy ra từ trang bị cơ bản này, là các hợp thành với $w$ của các đồng cấu nhóm tương ứng $\varphi_j,\psi_j$, của cấu xạ quiver $\tau_0$, của các mũi tên tương ứng $\delta_i$ và của đồng cấu Λ.

Cho B là tập hợp các $b(j)$ với $j\in$ Orb(H), cho $H_B$ là nhóm con đầy đủ của H với tập hợp các đỉnh là B; ký hiệu $u: H_B\rightarrow H$ là đơn ánh chính tắc; đặt $\varphi ''=\varphi '\circ u$ và $\psi ''=\psi '\circ u$. Cấu xạ $u$ cảm sinh một song ánh B $\rightarrow$ Orb(H) qua đó ta đồng nhất hai tập hợp này. Từ định lý 1 của II, p. 187, suy ra thêm một cấu xạ đồng luân chính tắc $w':$ Coh($\varphi '', \psi ''$)$\rightarrow$ Coh($\varphi ', \psi '$). Hơn nữa, cặp $(\varphi '', \psi '')$ được trang bị một cơ sở $(a'', b'', \beta ''_1, \beta ''_2,T'', i_0)$, sao cho $\Lambda ', \varphi '_j, \psi '_j, \tau '_0, \delta '_i(i, i'\in$ Orb(G), $j\in$ Orb(H)) là các hợp thành với $w'$ của $\Lambda '', \varphi ''_j, \psi ''_j, \tau ''_0, \delta ''_i$.

Các cấu xạ khác nhau của các nhómoid được đưa vào được tóm tắt bởi biểu đồ sau:

$H_{B\psi''}^{\varphi''}G_A^{\alpha''}$ Coh($\varphi '', \psi ''$)

$w'$

(9) H $^{\varphi'}G_A^{\alpha'}$ Coh($\varphi '', \psi ''$)

$\psi '$

$$
vw
$$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ ) .

Để chứng minh mệnh đề, do đó ta có thể giả sử rằng A = Som(G) và B = Som(H), nói cách khác rằng các ánh xạ chính tắc Som(G) $\rightarrow$ Orb(G) và Som(H) $\rightarrow$ Orb(H) là song ánh; trong phần còn lại của chứng minh, ta đặt mình dưới các giả thiết này.

Khi đó, quiver $G_1$ có tập hợp các đỉnh là A và tập hợp các mũi tên là tập hợp tổng của các tập hợp $G_a,a\in A$, và của tập hợp B. Các mũi tên của $G_a$ là các vòng tại $a$; nếu $b\in B$, mũi tên $b$ nối $\varphi (b)$ với $\psi (b)$, các mũi tên $c_1(b)$ và $c_2(b)$ lần lượt là các vòng tại $\varphi (b)$ và $\psi (b)$. Quiver T sẽ được đồng nhất với một cây định hướng của $G_1$; đó là một cây định hướng cực đại vì tập hợp các đỉnh của nó bằng tập hợp các đỉnh của $G_1($II, p. 157, mệnh đề 1). Đặt $a_0=a(i_0)$. Tập hợp các mũi tên của khung $\Gamma_0$ của cặp $(\varphi , \psi )$ được đồng nhất với B, cấu xạ của các quiver $\tau_1: \Gamma_0\rightarrow$ Grp(G$_1$) gán cho mũi tên $b$ lớp các đường đi $c_1(b)^{-1}bc_2(b)$ trong đồ thị $\widetilde{G}_1$.

Nhắc lại rằng $\theta_1$ ký hiệu cấu xạ chính tắc của các quiver của $G_1$ vào Grp(G$_1$). Đặt

$\lambda :_a*_{\in A}F(G_a)*F(B)\rightarrow$ Grp(G$_1$)$_{a_0}$

là đồng cấu nhóm duy nhất sao cho ta có

$\lambda (f) =\tau_1(d_a)\theta_1(f)\tau_1(d_a)^{-1}$ nếu $a\in A$ và $f\in G_a$;

$\lambda (b) =\tau_1(d_{\varphi(b)})\tau_1(b)\tau_1(d_{\psi(b)})^{-1}$ nếu $b\in B$.

Do đó ta có $\lambda =\lambda '\circ \varepsilon$, trong đó $\lambda '$ ký hiệu đồng cấu nhóm chính tắc từ $_a*_{\in A}F(G_a)*F(B)$ vào Grp(G$_1$)$_{a_0}$ được xác định bởi cây định hướng cực đại T (II, p. 179, prop. 9), và $\varepsilon$ là tự đẳng cấu duy nhất của nhóm $_a*_{\in A}F(G_a)*F(B)$ sao cho $\varepsilon (f) =f$ với $a\in A$ và $f\in G_a$, và $\varepsilon (b) =c_1(b)^{-1}h_1(b)c_2(b)$ với $b\in B$. Theo nhận xét 2 của II, p. 179, đồng cấu $\lambda$ là toàn ánh và hạt nhân của nó là nhóm con chuẩn nhỏ nhất của $_a*_{\in A}F(G_a)*F(B)$ chứa các mũi tên của T.

Ta ký hiệu $\pi :$ Grp(G$_1$)$\rightarrow$ Coh($\varphi , \psi$ ) là cấu xạ nhómoid chính tắc. Theo II, p. 177, hệ quả 1 của mệnh đề 8, đồng cấu nhóm $\pi_{a_0}$ từ Grp(G$_1$)$_{a_0}$ vào Coh($\varphi , \psi$ )$_{a_0}$ là toàn ánh, và hạt nhân của nó là nhóm con chuẩn nhỏ nhất của Grp(G$_1$)$_{a_0}$ chứa các vòng lặp Int($\tau_1(d_a)$)$(\alpha_1(f)\alpha_1(g)\alpha_1(f g)^{-1})$, với $a\in A$ và $f,g\in G_a$, và các vòng lặp Int($\tau_1(d_{\varphi(b)})$)$(\varphi (f)b\psi (f)^{-1}b^{-1})$, với $b\in B$ và $f\in H_b$.

Nếu $p: F(\bigcup G_a\cup B)\rightarrow (_a*_{\in A}G_a)*F(B)$ ký hiệu đồng cấu toàn ánh chính tắc, thì do đó ta có $\Lambda \circ p=\pi_{a_0}\circ \lambda$. Công thức này suy ra rằng đồng cấu Λ là toàn ánh; còn phải xác định hạt nhân của nó.

Với $a\in A$ và $f\in G_a$, ta ký hiệu $[f]$ là ảnh của $f\in F(G_a)$ trong nhóm $_a*_{\in A}F(G_a)*F(B)$. Với $a\in A,f, g\in G_a$, khi đó ta có

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

Do đó, hạt nhân của đồng cấu $\pi_{a_0}\circ \lambda$ là nhóm con chuẩn nhỏ nhất của $_a*_{\in A}F(G_a)*F(B)$ chứa các phần tử $[f][g][f g]^{-1}$ với $a\in A$ và $f,g\in G_a$, các phần tử $\varphi_b(f)[b]\psi_b(f)^{-1}[b]^{-1}$ với $b\in B$ và $f\in H_b$, và các phần tử $[b]$, với $b\in$ Fl(T).

Cuối cùng, hạt nhân của đồng cấu Λ là nhóm con chuẩn nhỏ nhất của $(_a*_{\in A}G_a)*F(B)$ chứa các ảnh qua $p$ của các phần tử nói trên, nói cách khác, các phần tử $[b]$, với $b\in$ Fl(T), và các phần tử $\varphi_b(f)[b]\psi_b(f)[b]^{-1}$, với $b\in B$ và $f\in H_b$. Mệnh đề được chứng minh.
