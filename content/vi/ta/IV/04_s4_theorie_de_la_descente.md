---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 4
section_title: Théorie de la descente
lang: vi
source: ta-i-iv-fr
book_pages: TA IV.382-TA IV.405, TA IV.462-TA IV.463
pdf_pages: 0398-0421, 0478-0479
extraction: native
subsections:
    - "no": 1
      title: Données de descente
      page: 382
      pdf_page: 398
    - "no": 2
      title: Données de descente effectives
      page: 384
      pdf_page: 400
    - "no": 3
      title: Descente de morphismes
      page: 387
      pdf_page: 403
    - "no": 4
      title: 'Descente : cas des espaces étalés'
      page: 388
      pdf_page: 404
    - "no": 5
      title: 'Descente : cas des revêtements'
      page: 390
      pdf_page: 406
    - "no": 6
      title: Descente de groupoïdes
      page: 394
      pdf_page: 410
    - "no": 7
      title: Descente par une application étale et surjective
      page: 399
      pdf_page: 415
    - "no": 8
      title: Groupoïde de Poincaré d’un espace quotient
      page: 402
      pdf_page: 418
statements: 29
exercises: 7
content_sha256: 02e5fb7544ba8701230cea5dca9bb6d080bd89f3fc6fed7d77ba98bee4059042
translated_from: content/en-mt/ta/IV/04_s4_theorie_de_la_descente.md
source_lang: en-mt
translation_method: machine
source_content_sha256: a9cfa1530684da37c0beb2dba5cd1ad16832230c665fd22fc8bc4f1c1f58d3a3
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-62fad221
glossary_version: 34
glossary_terms_sha256: 5ffe7de4c15bb50f2bcd5002dcc1e862c72a5c2be2d0763678a61e6358929a24
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. LÝ THUYẾT HẠ GIÁNG

### 1. Dữ liệu hạ giáng

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Cho $(Z, p)$ là một không gian X.

#### Định nghĩa 1 {#ta-iv-s4-def-1 .statement tag=0227}

Một dữ liệu hạ giáng đối với $f$ trên không gian X $(Z, p)$ được gọi là một ánh xạ liên tục $\tau : Z\times_YX\rightarrow Z$ thỏa mãn hai tính chất sau:

(i) Với mọi cặp $(x, x')\in X\times_YX$, ánh xạ $z\mapsto \tau (z, x')$ cảm sinh bởi hạn chế một song ánh $\tau_{x,x'}$ của $Z_x$ lên $Z_{x'}$;

(ii) Với mọi bộ ba $(x, x', x'')$ các điểm của X sao cho $f(x) =$ $f(x') =f(x'')$, ta có

$$
\tau_{x,x''}=\tau_{x',x''}\circ \tau_{x,x'}
$$

Nếu $\tau$ là một dữ liệu hạ giáng trên $(Z, p)$, họ $(\tau_{x,x'})$, với $(x, x')\in X\times_YX$, do đó là một luật phép toán (bên phải) của groupoid $X\times_YX$ trên không gian X $(Z, p)$ (II, p. 167). Đặc biệt, ta có $\tau_{x,x}=$ Id$_{Z_x}$ với mọi $x\in X$, điều này cũng được viết là $\tau (z, p(z)) =z$ với mọi $z\in Z$. Ngược lại, cho một luật phép toán (bên phải) của groupoid $X\times_YX$ trên $(Z, p)$, ánh xạ từ $Z\times_YX$ vào Z được xác định bởi $(z, x)\mapsto z\cdot (p(z), x)$ thỏa mãn các quan hệ (i) và (ii) của định nghĩa.

Cho X và Y là các không gian tôpô, $f: X\rightarrow Y$ là một ánh xạ liên tục và cho $(Z, p)$ là một không gian X. Nếu $\tau$ là một dữ liệu hạ giáng đối với $f$ trên $(Z, p)$, quan hệ $R_{\tau}(z_1, z_2)$ được xác định bởi « $f(p(z_1)) =$ $f(p(z_2))$ và $\tau (z_1, p(z_2)) =z_2$ » là quan hệ tương đương trong Z suy ra từ phép toán của groupoid $X\times_YX$ được xác định bởi $\tau$; nó tương thích với ánh xạ $f\circ p$. Người ta nói rằng đây là quan hệ tương đương liên kết với dữ liệu hạ giáng $\tau$. Song ánh chính tắc $(z_1, z_2)\mapsto (z_1, p(z_2))$ của đồ thị Γ của quan hệ tương đương $R_{\tau}$ lên $Z\times_YX$ là một đồng phôi, đồng phôi ngược áp dụng một phần tử $(z_1, x_2)\in Z\times_YX$ vào $(z_1, \tau (z_1, x_2))$.

Ngược lại, cho R là một quan hệ tương đương trong Z tương thích với ánh xạ $f\circ p: Z\rightarrow Y$ và cho Γ là đồ thị của R. Giả sử thêm rằng ánh xạ $p_2: (z_1, z_2)\mapsto (z_1, p(z_2))$ xác định một đồng phôi của Γ lên $Z\times_YX$. Ánh xạ $\tau : Z\times_YX\rightarrow Z$ cho bởi pr$_2\circ p^{-1}_2$ là liên tục; nó là một dữ liệu hạ giáng đối với $f$ trên $(Z, p)$ và quan hệ R là quan hệ tương đương liên kết với $\tau$.

#### Ví dụ 1 {#ta-iv-s4-n1-exa-1 .statement tag=0228}

Cho X và Y là các không gian tôpô, cho $f: X\rightarrow Y$ là một ánh xạ liên tục và cho $(T, q)$ là một không gian Y. Đặt $Z = X\times_YT$. Ánh xạ $\tau$ từ $Z\times_YX$ vào Z, gán cho $((x, t), x')$ phần tử $(x', t)$, là một dữ liệu descent tương đối với $f$ trên không gian X $(X\times_YT$, pr$_1)$, được gọi là dữ liệu descent chính tắc. Với $z_1= (x_1, t_1)$ và $z_2= (x_2, t_2)\in Z$, quan hệ $R_{\tau}\{z_1, z_2\}$ tương đương với $t_1=t_2$.

#### Ví dụ 2 {#ta-iv-s4-n1-exa-2 .statement tag=0229}

Cho Y là một không gian tôpô, $(V_i)_{i\in I}$ là một họ các tập con của Y, và với mỗi $i\in I$, cho $(Z_i, p_i)$ là một không gian $V_i$. Gọi X là không gian tôpô tổng của họ $(V_i)_{i\in I}$ và $(Z, p)$ là không gian X tổng của họ $(Z_i)_{i\in I}$. Cho $f: X\rightarrow Y$ là ánh xạ chính tắc.

Không gian $X\times_YX$ khi đó được đồng nhất với không gian tổng của họ $(V_i\cap$ $V_j)_{(i,j)\in I\times I}($I, p. 4, Ví dụ 5). Cho $\tau$ là một dữ liệu descent tương đối với $f$ trên $(Z, p)$. Với mỗi cặp $(i, j)\in I\times I$, định nghĩa một ánh xạ liên tục $\tau_{i,j}:\overset{-1}{p_{i}}(V_i\cap V_j)\rightarrow \overset{-1}{p_{j}}(V_i\cap V_j)$ bởi $z\mapsto \tau (z,(p_i(z), j))$. Họ $(\tau_{i,j})$ thỏa mãn các tính chất sau:

(i) Với mỗi $i\in I$, ta có $\tau_{i,i}=$ Id$_{Z_i}$;

(ii) Với mỗi cặp $(i, j)\in I\times I,\tau_{i,j}$ là một đẳng cấu của các không gian $(V_i\cap V_j)$ ;

(iii) Với mỗi bộ ba $(i, j, k)\in I\times I\times I$ và mỗi $z\in \overset{-1}{p_{i}}(V_i\cap V_j\cap V_k)$, ta có $\tau_{j,k}(\tau_{i,j}(z)) =\tau_{i,k}(z)$.

Ngược lại, mọi họ $(\tau_{i,j})$ có các tính chất trên đều xuất phát từ một dữ liệu descent duy nhất tương đối với $f$ trên $(Z, p)$.

### 2. Các dữ liệu descent hiệu dụng

Cho X và Y là các không gian tôpô, $f: X\rightarrow Y$ là một ánh xạ liên tục và $(Z, p)$ là một không gian X. Cho $\tau$ là một dữ liệu descent tương đối với $f$ trên $(Z, p)$, cho $R_{\tau}$ là quan hệ tương đương liên kết và cho $g: Z\rightarrow Z/R_{\tau}$ là ánh xạ chính tắc. Vì quan hệ $R_{\tau}$ tương thích với ánh xạ $f\circ p$, tồn tại một ánh xạ liên tục duy nhất $q: Z/R_{\tau}\rightarrow Y$ sao cho biểu đồ

Z $^gZ/R_{\tau}$

$$
pq \tag{1}
$$

X $^f$ Y

cho nó là một bình phương giao hoán. Không gian Y $(Z/R_{\tau}, q)$ được gọi là không gian thương của $(Z, p)$ bởi dữ kiện đi xuống $\tau$. Ta ký hiệu bởi $h: Z\rightarrow X\times_Y$ $(Z/R_{\tau})$ ánh xạ được xác định bởi $h(z) = (p(z), g(z))$ với $z\in Z$. Nó liên tục. Cho $(x, u)\in X\times_Y(Z/R_{\tau})$ và cho $z\in Z$ sao cho $g(z) =u$; khi đó ta có $(z, x)\in Z\times_YX$ và điểm $z'=\tau (z, x)$ là phần tử duy nhất của Z sao cho $h(z') = (x, u)$; do đó, ánh xạ $h$ là song ánh.

Ta nói rằng dữ kiện đi xuống $\tau$ đối với $f$ trên $(Z, p)$ là hiệu dụng nếu biểu đồ (1) là một bình phương Descartes, nghĩa là nếu song ánh liên tục $h$ là một phép đồng phôi. Để dữ kiện đi xuống $\tau$ là hiệu dụng, điều kiện cần và đủ là các tập hợp $\overset{-1}{p}(U)\cap V$, trong đó U là một tập con mở của X và V là một tập con mở của Z bão hòa đối với $R_{\tau}$, tạo thành một cơ sở của tôpô của Z. Đặc biệt, điều kiện để một dữ kiện đi xuống đối với $f$ là hiệu dụng có bản chất địa phương trên Y.

#### Ví dụ 1 {#ta-iv-s4-n2-exa-1 .statement tag=022A}

Cho X và Y là các không gian tôpô và $f: X\rightarrow Y$ là một ánh xạ liên tục. Cho $(T, q)$ là một không gian Y. Cho Z là không gian X $X\times_YT$, được trang bị ánh xạ pr$_1$; ta ký hiệu $\tau$ là dữ kiện đi xuống chính tắc của nó đối với $f$ (IV, p. 383, Ví dụ 1). Các tập con của Z có dạng $X\times_YV$, trong đó V là một tập con mở của T, là mở trong Z và bão hòa đối với quan hệ $R_{\tau}($loc. cit.). Theo định nghĩa của tôpô tích, các tập hợp $U\times_Y$ pr$^{-1}_2(V)$, trong đó U là mở trong X và V là mở trong T, tạo thành một cơ sở của tôpô của $X\times_YZ$. Do đó, dữ kiện đi xuống chính tắc trên một tích sợi $X\times_YT$ là hiệu dụng.

Ánh xạ chính tắc $Z/R_{\tau}\rightarrow T$ là đơn ánh và liên tục. Tuy nhiên, nó không nhất thiết là toàn ánh, cũng không nhất thiết là ngặt (IV, p. 462, exerc. 1).

#### Ví dụ 2 {#ta-iv-s4-n2-exa-2 .statement tag=022B}

Ta lấy lại ký hiệu của Ví dụ 2 (IV, p. 383). Khi đó không gian tôpô $Z/R_{\tau}$ là không gian tôpô thu được bằng cách dán các không gian $Z_i$ theo các $\overset{-1}{p_{i}}(V_i\cap V_j)$ nhờ các song ánh $\tau_{i,j}$ (TG, I, p. 16). Do đó, nếu với mọi $i\in I$, tập hợp $V_i$ là mở (resp. đóng) trong Y, thì tập hợp $g(Z_i)$ là mở (resp. đóng) trong $Z/R_{\tau}$ và hạn chế của $g$ trên $Z_i$ cảm sinh một phép đồng phôi của $Z_i$ lên $g(Z_i)$ (TG, I, p. 17, Prop. 9). Không gian Z là không gian tổng của các không gian $Z_i$; không gian $X\times_Y(Z/R_{\tau})$ là không gian tổng của các không gian $V_i\times_Y$ $(Z/R_{\tau}) =g(Z_i)$. Ánh xạ $h$ được đồng nhất với ánh xạ tổng của các ánh xạ $g|Z_i: Z_i\rightarrow g(Z_i)$. Do đó nó là một phép đồng phôi, điều này chỉ ra rằng dữ kiện đi xuống $\tau$ là hiệu dụng.

Không có một giả thiết riêng biệt nào trên các tập con $V_i$, không phải lúc nào cũng đúng rằng hạn chế của $g$ trên $Z_i$ cảm sinh một phép đồng phôi của $Z_i$ lên ảnh của nó; trong trường hợp này, dữ kiện đi xuống $\tau$ không hiệu dụng (IV, p. 462, exerc. 2).

#### Mệnh đề 1 {#ta-iv-s4-prop-1 .statement tag=022C}

Cho X và Y là các không gian tôpô, cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Giả sử rằng mọi điểm của Y đều có một lân cận trên đó tồn tại một tiết diện liên tục của ánh xạ $f$. Khi đó mọi dữ liệu hạ xuống đối với $f$ trên một không gian X đều là hiệu dụng.

Cho $(Z, p)$ là một không gian X và cho $\tau$ là một dữ liệu hạ xuống đối với $f$ trên $(Z, p)$. Mệnh đề rằng $\tau$ là một dữ liệu hạ xuống hiệu dụng là địa phương trong Y, do đó cho phép ta giả sử rằng ánh xạ $f$ có một tiết diện liên tục $s$. Gọi $g: Z\rightarrow Z/R_{\tau}$ và $q: Z/R_{\tau}\rightarrow Y$ là các ánh xạ chính tắc, và cho $h: Z\rightarrow X\times_Y(Z/R_{\tau})$ là ánh xạ được cho bởi $z\mapsto (p(z), g(z))$. Ánh xạ $h$ là song ánh và liên tục; chỉ cần chứng minh rằng nó là một đồng phôi.

Ánh xạ từ Z vào Z, ánh xạ mà ứng với $z$, liên kết $\tau (z, s(f(p(z))))$, là liên tục và ánh xạ mọi phần tử của Z vào phần tử duy nhất $z'$ của Z tương đương với nó đối với quan hệ $R_{\tau}$ và sao cho $p(z')$ thuộc ảnh của $s$. Do đó nó xác định, bằng cách chuyển qua thương, một ánh xạ liên tục $t: Z/R_{\tau}\rightarrow Z$ là một tiết diện của ánh xạ $g$. Đặc biệt, ta có $f\circ p\circ t=q\circ g\circ t=q$.

Với mọi $(x, u)\in X\times_Y(Z/R_{\tau})$, ta có $f(p(t(u))) =f(x)$; khi đó đặt $h'(x, u) =\tau (t(u), x)$. Ánh xạ thu được $h'$ từ $X\times_Y(Z/R_{\tau})$ vào Z là liên tục. Với mọi $(x, u)\in X\times_Y(Z/R_{\tau})$, ta có

$$
h(h'(x, u)) = (p(h'(x, u)), g(h'(x, u)))
$$

$$
= (p(\tau (t(u), x)), g(\tau (t(u), x)))
$$

$$
= (x, u)
$$

vì $\tau (t(u), x)$ là tương đương với $t(u)$ đối với quan hệ $R_{\tau}$. Điều này chứng minh rằng ánh xạ $h\circ h'$ là ánh xạ đồng nhất của $X\times_Y(Z/R_{\tau})$. Với $z\in Z$, khi đó ta có $t(g(z)) =\tau (z, s(f(p(z)))$ và $f(p(t(g(z)))) =f(p(z))$, do đó $z=\tau (t(g(z)), p(z))$, theo định nghĩa của quan hệ tương đương $R_{\tau}$. Vì vậy ta có $h'(h(z)) =z$ và $h'\circ h=$ Id$_Z$. Ánh xạ $h$ do đó là một đồng phôi, điều phải chứng minh.

#### Mệnh đề 2 {#ta-iv-s4-prop-2 .statement tag=022D}

Cho $f: X\rightarrow$ Y là một ánh xạ liên tục, cho $(Z, p)$ là một không gian X và cho $\tau$ là một dữ liệu hạ xuống đối với $f$ trên Z. Quan hệ tương đương $R_{\tau}$ là đóng nếu $f$ là thực sự; nó là mở nếu $f$ là mở.

Ánh xạ $\widetilde{\tau}: Z\times_YX\rightarrow$ X $\times_Y$ Z được xác định bởi $(z, x)\mapsto$ $(p(z), \tau (z, x))$ là một đồng phôi, với ánh xạ nghịch đảo $(x, z)\mapsto (\tau (z, x), p(z))$. Ta có $\tau$ = pr$_2\circ \widetilde{\tau}$, trong đó pr$_2: X\times_YZ\rightarrow$ Z là phép chiếu thứ hai. Nếu $f$ là thực sự, thì pr$_2$ là thực sự; nếu $f$ là mở, thì pr$_2$ là mở (I, p. 17, prop. 8). Suy ra rằng $\tau$ là thực sự (tương ứng mở) nếu $f$ là như vậy. Bao bão hòa của một tập con A của Z đối với quan hệ $R_{\tau}$ là ảnh của $A\times_YX$ qua $\tau$. Do đó, nếu $f$ là thực sự, bao bão hòa của một tập con đóng là đóng; nếu $f$ là mở, bao bão hòa của một tập con mở là mở.

### 3. Sự hạ tầng của các cấu xạ

Cho X và Y là các không gian tôpô và cho $f$ là một ánh xạ liên tục từ X vào Y. Cho $(Z, p)$ và $(Z', p')$ là các X-không gian được trang bị dữ liệu hạ tầng đối với $f$, lần lượt được ký hiệu bởi $\tau$ và $\tau '$. Ta nói rằng một cấu xạ X $\varphi : Z\rightarrow Z'$ là tương thích với các dữ liệu hạ tầng $\tau$ và $\tau '$ nếu ta có

$$
\tau '(\varphi (z), x) =\varphi (\tau (z, x))
$$

với mọi $(z, x)\in Z\times_YX$. Điều này tương đương với việc nói rằng các ảnh qua $\varphi$ của hai điểm tương đương đối với quan hệ $R_{\tau}$ là tương đương đối với quan hệ $R_{\tau'}$. Một cấu xạ như vậy $\varphi$ xác định, bằng cách chuyển qua các thương, một ánh xạ liên tục $\overline{\varphi}: Z/R_{\tau}\rightarrow Z'/R_{\tau'}$; nó là một cấu xạ Y của các không gian.

Ta ký hiệu bởi $\mathscr{C}_{\tau ,\tau'}(Z; Z')$ tập hợp các cấu xạ X từ Z vào $Z'$ tương thích với các dữ liệu hạ tầng $\tau$ và $\tau '$.

#### Mệnh đề 3 {#ta-iv-s4-prop-3 .statement tag=022E}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow$ Y là một ánh xạ liên tục. Cho $(Z, p)$ và $(Z', p')$ là các X-không gian được trang bị dữ liệu hạ tầng đối với $f$, lần lượt được ký hiệu bởi $\tau$ và $\tau '$. Nếu dữ liệu hạ tầng $\tau '$ là hiệu dụng, ánh xạ $\varphi \mapsto \overline{\varphi}$ là một song ánh từ $\mathscr{C}_{\tau ,\tau'}(Z; Z')$ lên $\mathscr{C}_Y(Z/R_{\tau}; Z'/R_{\tau'})$.

Đối với mọi cấu xạ X $\varphi$ từ Z vào $Z'$ tương thích với dữ liệu hạ tầng, ánh xạ $\overline{\varphi}$ là một cấu xạ Y. Ngược lại, cho $g: Z\rightarrow Z/R_{\tau}$ và $g': Z'\rightarrow Z'/R_{\tau'}$ là các ánh xạ chính tắc, và cho $\psi : Z/R_{\tau}\rightarrow Z'/R_{\tau'}$ là một cấu xạ Y. Các ánh xạ $p: Z\rightarrow X$ và $\psi \circ g: Z\rightarrow Z'/R_{\tau'}$ là các cấu xạ Y. Giả thiết rằng dữ liệu hạ tầng $\tau '$ là hiệu dụng có nghĩa là biểu đồ

$$
{Z'}^{g'}Z'/R_{\tau'}
$$

$p'q'$

X $^f$ Y

là một bình phương Descartes. Do đó tồn tại một cấu xạ liên tục duy nhất $\varphi : Z\rightarrow Z'$ sao cho $p'\circ \varphi =p$ và $g'\circ \varphi =\psi \circ g$. Đẳng thức thứ nhất có nghĩa là $\varphi$ là một X-cấu xạ, đẳng thức thứ hai có nghĩa là $\varphi$ tương thích với dữ liệu giáng và $\overline{\varphi}=\psi$, do đó có mệnh đề.

### 4. Giáng: trường hợp của các không gian trải

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Cho T và $T'$ là các Y-không gian; trang bị cho các X-không gian $X\times_YT$ và $X\times_YT'$ các dữ liệu giáng chính tắc của chúng và ký hiệu bởi $\mathscr{C}_f(X\times_YT; X\times_YT')$ tập hợp các X-cấu xạ của $X\times_YT$ vào $X\times_YT'$ tương thích với các dữ liệu giáng này. Với mọi Y-cấu xạ $\varphi : T\rightarrow T'$, X-cấu xạ $f^*(\varphi ): (x, t)\mapsto$ $(x, \varphi (t))$ của $X\times_YT$ vào $X\times_YT'$ tương thích với các dữ liệu giáng chính tắc. Ta sẽ ký hiệu bởi $f^*:\mathscr{C}_Y(T; T')\rightarrow \mathscr{C}_f(X\times_YT; X\times_YT')$ ánh xạ thu được.

#### Mệnh đề 4 {#ta-iv-s4-prop-4 .statement tag=022F}

Giả sử rằng ánh xạ $f$ là ngặt và toàn ánh và rằng T là một Y-không gian trải. Khi đó ánh xạ $f^*:\mathscr{C}_Y(T; T')\rightarrow \mathscr{C}_f(X\times_YT; X\times_YT')$ là song ánh.

Gọi $\tau$ (tương ứng $\tau '$) là quan hệ tương đương trên $X\times_YT$ (tương ứng trên $X\times_YT'$) liên kết với dữ liệu giáng chính tắc. Vì ánh xạ $f$ là toàn ánh, phép chiếu pr$_2: X\times_YT\rightarrow T$ là toàn ánh và ánh xạ chính tắc $(X\times_YT)/R_{\tau}\rightarrow T$ là song ánh. Đặc biệt, ánh xạ $f^*$ là đơn ánh. Ta hãy chứng minh rằng nó là toàn ánh. Cho $\varphi : X\times_YT\rightarrow X\times_YT'$ là một X-cấu xạ tương thích với các dữ liệu giáng chính tắc. Khi đó với $(x, t)\in X\times_YT$, ta có $\varphi (x, t) = (x, \varphi (t))$, trong đó $\overline{\varphi}$ là một ánh xạ từ T vào $T'$.

Theo định nghĩa của $\overline{\varphi}$, ánh xạ $\overline{\varphi}\circ$ pr$_2: X\times_YT\rightarrow T'$ bằng với pr$_2\circ \varphi$, và do đó là liên tục. Vì ánh xạ $f$ là toàn ánh và ngặt và T là một Y-không gian trải, phép chiếu pr$_2: X\times_YT\rightarrow T$ là ngặt (I, p. 32, nhận xét 3). Theo mệnh đề 9 của I, p. 18, ánh xạ $\overline{\varphi}$ do đó là liên tục. Nó là một Y-cấu xạ sao cho $f^*(\overline{\varphi}) =\varphi$, điều này chứng minh mệnh đề.

#### Hệ quả {#ta-iv-s4-n4-cor-1 .statement tag=022G}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ ngặt và toàn ánh. Cho T và $T'$ là các Y-không gian trải. Nếu tồn tại một X-đẳng cấu $X\times_YT\rightarrow X\times_YT'$ tương thích với các dữ liệu giáng chính tắc, thì các Y-không gian T và $T'$ là đẳng cấu.

Cho $\psi : X\times_YT\rightarrow X\times_YT'$ là một X-đẳng cấu của các không gian trải. Theo mệnh đề 4, tồn tại một cấu xạ duy nhất của các Y-không gian $\varphi : T\rightarrow T'$ sao cho $\psi =f^*(\varphi )$. Vì $f$ là toàn ánh, ánh xạ $\varphi$ là song ánh. Khi đó suy ra từ hệ quả 2 của I, p. 30 rằng $\varphi$ là một đẳng cấu, vì các Y-không gian T và $T'$ là trải.

#### Mệnh đề 5 {#ta-iv-s4-prop-5 .statement tag=022H}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Giả sử rằng ánh xạ $f$ là thực sự và tách, hoặc ngược lại là mở. Mọi dữ liệu giáng tương đối với $f$ trên một X-không gian trải đều là hiệu dụng. Hơn nữa, nếu $f$ là toàn ánh, không gian thương là một Y-không gian trải.

Cho $(Z, p)$ là một không gian X-étalé và cho $\tau$ là một dữ liệu hạ giáng đối với $f$ trên $(Z, p)$. Ta ký hiệu $R_{\tau}$ là quan hệ tương đương trong Z liên kết với $\tau$, ký hiệu $g: Z\rightarrow Z/R_{\tau}$ là toàn cấu chính tắc và ký hiệu $h$ là ánh xạ của Z vào $X\times_Y(Z/R_{\tau})$ được xác định bởi $z\mapsto (p(z), g(z))$. Nó liên tục và song ánh; ta hãy chứng minh rằng nó là một phép đồng phôi.

a) Trước hết giả sử rằng ánh xạ $f$ là mở.

Cho $z_0$ là một điểm của Z; đặt $x_0=p(z_0)$. Vì $p$ là étalé, tồn tại một lân cận U của $x_0$ trong X và một tiết diện liên tục $s: U\rightarrow Z$ của $p$ trên U sao cho $s(x_0) =z_0$. Ánh xạ $p\times p: Z\times_YZ\rightarrow$ $X\times_YX$ là étalé, và các ánh xạ từ $U\times_YU$ vào $Z\times_YZ$ được xác định bởi $(x, x')\mapsto (s(x), s(x'))$ và $(x, x')\mapsto (s(x), \tau (s(x), x'))$ là các tiết diện liên tục của nó trên $U\times_YY$. Vì chúng trùng nhau tại mọi điểm của $U\times_YU$ có dạng $(x, x)$, do đó chúng trùng nhau trên một lân cận mở V của $\Delta_U$ được chứa trong $U\times_YU$. Cho $U_0$ là một lân cận của $x_0$ trong X sao cho $U_0\times_YU_0$ được chứa trong V. Cho $(x, u)$ là một điểm của $U_0\times_Yg(s(U_0))$; cho $x'\in U_0$ sao cho $u=g(s(x'))$. Khi đó ta có $s(x) =\tau (s(x'), x)$, do đó $R_{\tau}\{s(x), s(x')\}$ và $(x, u) = (x, g(s(x'))) =$ $(x, g(s(x))) =h(s(x))$.

Vì ánh xạ $g$ là mở (IV, p. 386, prop. 2), tập hợp $U_0\times_Yg(s(U_0))$ là một tập con mở của $X\times_Y(Z/R_{\tau})$ trên đó ánh xạ $h^{-1}$ bằng ánh xạ liên tục $s\circ$ pr$_1$. Ánh xạ $h$ do đó là một phép đồng phôi.

b) Bây giờ giả sử rằng ánh xạ $f$ là thực sự và tách được.

Cho $z_0$ là một điểm của Z; đặt $x_0=p(z_0)$ và $y_0=f(x_0)$. Ánh xạ $s$ cho bởi $x\mapsto \tau (z_0, x)$ là một tiết diện của $p$ trên $\overset{-1}{f}(y_0)$.

Tập hợp $\overset{-1}{f}(y_0)$ là compact (TG, I, p. 75, Định lý 1 và I, p. 26, Nhận xét 2), và hai điểm phân biệt của $\overset{-1}{f}(y_0)$ có các lân cận rời nhau trong X, vì $f$ là tách được (I, p. 25, Mệnh đề 1). Theo Định lý 2 của I, p. 37, do đó tồn tại một lân cận $U_0$ của $\overset{-1}{f}(y_0)$ trong X và một tiết diện $s_0$ của $p$ trên $U_0$ mở rộng $s$. Tập hợp $s_0(U_0)$ là một tập hợp mở của Z, vì $p$ là étale (I, p. 30, Hệ quả 3), và chứa tập hợp bão hòa của $\{z_0\}$ đối với quan hệ $R_{\tau}$. Ánh xạ $g$ là đóng (IV, p. 386, Mệnh đề 2). Khi đó tồn tại một tập hợp mở V của $Z/R_{\tau}$ sao cho $W =\overset{-1}{g}(V)\cap \overset{-1}{p}(U_0)$ là một lân cận của $z_0$ được chứa trong $s_0(U_0)$ (I, p. 75, Bổ đề).

Bây giờ lấy $(x, u)\in U_0\times_YV$, và gọi $z$ là điểm duy nhất của Z sao cho $h(z) = (x, u)$; theo định nghĩa, ta có $z\in W$. Vì $W\subset s_0(U_0)$, ta có $z=s_0(p(x))$. Điều này chứng minh rằng hạn chế của $h^{-1}$ vào tập hợp mở $U_0\times_YV$ của $X\times_Y(Z/R_{\tau})$ bằng $s_0\circ p\circ$ pr$_1$. Do đó, $h$ là một đồng phôi.

Như vậy ta đã chứng minh rằng dữ liệu hạ tầng $\tau$ là hiệu dụng. Ánh xạ $f$ là ngặt phổ quát (I, p. 20, hệ quả). Dưới giả thiết rằng $f$ là toàn ánh, từ Mệnh đề 8 của I, p. 31 suy ra rằng $q: Z/R_{\tau}\rightarrow Y$ là étale.

### 5. Hạ tầng: trường hợp của các phủ

Cho X, Y là các không gian tôpô, và cho $f: X\rightarrow Y$ là một ánh xạ liên tục toàn ánh. Cho $(Z, p)$ là một phủ của X, và cho $\tau$ là một dữ liệu hạ tầng tương đối với $f$ trên Z.

Nếu $f$ là thực sự và tách được (tương ứng, nếu $f$ là mở), dữ liệu hạ tầng $\tau$ là hiệu dụng và không gian Y $Z/R_{\tau}$ là một không gian étale (IV, p. 389, Mệnh đề 5). Nó thậm chí là một phủ của Y nếu $f$ có một tiết diện liên tục trong một lân cận của mỗi điểm (I, p. 72, Mệnh đề 3) hoặc nếu Z là một phủ hữu hạn địa phương của X (I, p. 77, Hệ quả 4). Số này dành để nêu ra các điều kiện khác mà dưới đó $Z/R_{\tau}$ là một phủ của Y.

Trước hết ta hãy chứng minh một bổ đề.

#### Bổ đề 1 {#ta-iv-s4-lem-1 .statement tag=022I}

Cho B, $B'$ là các không gian tôpô, và cho $f: B'\rightarrow B$ là một ánh xạ liên tục. Nếu bình phương thớ $B'\times_BB'$ là liên thông địa phương, thì không gian tôpô $B'$ là liên thông địa phương.

Cho $a$ là một điểm của $B'$ và cho V là một lân cận của $a$. Giả sử rằng bình phương thớ $B'\times_BB'$ là liên thông địa phương và cho W là một lân cận liên thông của $(a, a)$ trong $B'\times_BB'$ được chứa trong $V\times V$. Đặt U = pr$_1(W)$. Tập hợp U được chứa trong V, và là liên thông vì ảnh của một tập hợp liên thông qua một ánh xạ liên tục là liên thông. Nếu $\Delta_{B'}$ ký hiệu đường chéo của $B'\times_BB'$, ánh xạ pr$_1|\Delta_{B'}: \Delta_{B'}\rightarrow B'$ là một phép đồng phôi. Vì U chứa pr$_1(W\cap \Delta_{B'})$ và $W\cap \Delta_{B'}$ là một lân cận của $(a, a)$ trong $\Delta_{B'}$, U là một lân cận của $a$ trong $B'$. Điều này chứng minh bổ đề.

#### Mệnh đề 6 {#ta-iv-s4-prop-6 .statement tag=022J}

Cho

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

là một bình phương Descartes. Giả sử rằng ánh xạ $f$ là thực sự, tách được và toàn ánh, và đưa ra một trong các giả thiết sau:

(i) Các thớ của $f$ là liên thông địa phương và bình phương thớ $B'\times_BB'$ là liên thông địa phương.

(ii) Các thớ của $f$ là hữu hạn, đường chéo $\Delta_{B'}$ của $B'\times_BB'$ là mở trong $B'\times_BB'$ và $B'\times_BB'-\Delta_{B'}$ là một không gian liên thông địa phương.

Khi đó, nếu $(E', p')$ là một phủ, thì $(E, p)$ là một phủ.

Vì ánh xạ $f$ là ngặt một cách phổ quát (I, p. 20, hệ quả), ánh xạ $p$ là étale (I, p. 31, mệnh đề 8) và tách được (I, p. 27, mệnh đề 4). Ta sẽ giả sử, điều này là được phép, rằng $E'= B'\times_BE$.

Cho $a$ là một điểm của B; cần chứng minh rằng điểm $a$ có một lân cận W sao cho W-không gian $(E_W, p_W)$ là một phủ

có thể tầm thường hóa được. Đặt $B'_a$ = $\overset{-1}{f}(a)$ và ký hiệu bởi $E'_a$ = $(^-{p'}^1)(E_a)$. Ánh xạ $t_a: E'_a\rightarrow B'_a\times E_a$ được xác định bởi $t_a(y) = (p'(y), f'(y))$ là một $B'_a$-đẳng cấu (I, p. 9, mệnh đề 4), do đó $E'_a$ là một phủ có thể tầm thường hóa được của $B'_a$ và $t_a$ là một phép tầm thường hóa của phủ này.

Ta hãy chứng minh rằng tồn tại một lân cận $V'$ của $B'_a$ trong $B'$ và một phép tầm thường hóa liên tục $t$ của phủ $(E'_{V'}, p_{V'})$ mở rộng $t_a$. Dưới giả thiết (ii), $B'_a$ là hữu hạn và các điểm của nó có các lân cận mở rời nhau từng đôi một trên đó phủ $E'$ là có thể tầm thường hóa được, do đó mệnh đề trong trường hợp này. Dưới giả thiết (i), $B'_a$ là liên thông địa phương, và $B'($IV, p. 390, bổ đề 1) cũng vậy; vì ánh xạ $f$ là thực sự và tách được, $B'_a$ là compact và hai điểm phân biệt có các lân cận rời nhau trong $B'$, sao cho cặp $(B',B'_a)$ thỏa mãn tính chất (PCV) ( I, p. 37, bổ đề 1). Do đó mệnh đề suy ra từ Hệ quả 2 của I, p. 90.

Vì $f$ là thực sự, tồn tại một lân cận V của $a$ trong B sao cho $V'$ chứa $\overset{-1}{f}(V)$ (bổ đề, I, p. 75). Do đó ta có thể giả thiết rằng

$$
V'=\overset{-1}{f}(V)
$$

Ta trang bị cho các không gian $V'$- $V'\times E_a$ và $E'_{V'}= V'\times_BE$ dữ liệu giáng cấp chính tắc của chúng đối với $f_V: V'\rightarrow V$. Bây giờ ta sẽ chứng minh rằng, sau khi thu nhỏ V và $V'$, đẳng cấu của các không gian $V'$ $t: E'_{V'}\rightarrow$ $V'\times E_a$ mà ta vừa định nghĩa là tương thích với dữ liệu giáng cấp, nghĩa là ta có $t(b'_1, x) =t(b'_2, x)$ nếu $(b'_1, b'_2)\in V'\times_VV'$ và $x\in E_{f(b'_1)}$. Gọi $\widetilde{t}$ là ánh xạ pr$_2\circ t: E'_{V'}\rightarrow E_a$.

Đặt $V''= V'\times_VV'$; ta xét nó như một không gian $V'$ nhờ phép chiếu thứ nhất. Ánh xạ $((b'_1, b'_2), x)\mapsto ((b'_1, b'_2),(b'_1, x))$ từ $V''\times_VE$ vào $V''\times_{V'}E'$ là một đẳng cấu của các không gian $V''$; điều này chỉ ra rằng $V''\times_VE$ là một phủ của $V''$.

Với $i= 1$, 2, định nghĩa một ánh xạ $u_i: V''\times_VE\rightarrow V''\times E_a$ bằng cách đặt $u_i(b'_1, b'_2, x) = (b'_1, b'_2,\widetilde{t}(b'_i, x))$; đó là các phép tầm thường hóa của phủ $V''\times_VE$. Gọi $W''$ là tập hợp các điểm $w\in V''$ trên đó các phép tầm thường hóa này $u_1$ và $u_2$ trùng nhau; nó chứa $B'_a\times B'_a$, cũng như đường chéo $\Delta_{V'}$. Ta hãy chứng minh rằng $W''$ là một lân cận của $B'_a\times B'_a$. Dưới giả thiết (i), điều này suy ra từ Hệ quả 2 của I, p. 80, vì $B'\times B'$ là liên thông địa phương. Dưới giả thiết (ii), $W''$ chứa một lân cận của $(B'_a\times B'_a)-\Delta_{B'_a}$ trong $(B'\times_BB')-\Delta_{B'}$, vì tập hợp này là liên thông địa phương (chỗ đã dẫn). Vì $\Delta_{V'}$ mở trong $B'\times_BB',W''$ là một lân cận của $B'_a\times B'_a$ trong $V''$.

Vì $f$ là thực sự, ánh xạ chính tắc $f''$ của $B'\times_BB'$ vào B là thực sự, vì nó là hợp thành của phép chiếu pr$_1: B'\times_BB'\rightarrow B'$ và ánh xạ $f$.

Theo bổ đề của I, p. 75, tồn tại một lân cận W của $a$ trong V

sao cho $(f\overset{-1}{''})(W)$ được chứa trong $W''$; đặt $W'=(\overset{-1}{f}')(W)$; đó là một tập con của $V'$ và đẳng cấu của các không gian étale $t: E'_{W'}\rightarrow W'\times E_a$ là tương thích với dữ liệu giảm cấp chính tắc tương đối với ánh xạ $f_W: W'\rightarrow W$. Suy ra từ hệ quả (IV, p. 388) rằng các không gian étale trên $W$ $E_W$ và $W\times E_a$ là đẳng cấu. Đặc biệt, $E_W$ là một phủ khả giản, do đó có mệnh đề.

#### Hệ quả 1 {#ta-iv-s4-prop-6-cor-1 .statement tag=022K}

Cho E và B là các không gian tôpô, $p: E\rightarrow B$ là một ánh xạ liên tục và $(A_i)_{i\in I}$ là một phủ đóng hữu hạn địa phương của B sao cho với mọi cặp $(i, j)\in I\times I,i=\not j$, giao $A_i\cap A_j$ là một không gian liên thông địa phương. Khi đó, để không gian B $(E, p)$ là một phủ, điều kiện cần và đủ là, với mọi $i\in I$, không gian $A_i$ $(\overset{-1}{p}(A_i), p_{A_i})$ là một phủ của $A_i$.

Điều kiện là cần (xem I, p. 69). Ngược lại, gọi $B'$ là tổng tôpô của họ $(A_i)_{i\in I}$ và $f: B'\rightarrow B$ là ánh xạ chính tắc. Ánh xạ $f$ là đóng (TG, I, p. 6, mệnh đề 4), tách được (I, p. 27, nhận xét 5), có các thớ hữu hạn, do đó thực sự (TG, I, p. 75, định lý 1); nó cũng là toàn ánh. Đường chéo $\Delta_{B'}$, bằng $\bigcup_{i\in I}A_i\times_BA_i$, là mở trong $B'\times_BB'$. Cuối cùng, không gian $(B'\times_BB')-\Delta_{B'}$ là đồng phôi với tổng tôpô của họ $(A_i\cap A_j)$, $(i, j)\in I\times I$, $i=\not j$; do đó nó là liên thông địa phương. Giả thiết (ii) của mệnh đề 6 được thỏa mãn. Nếu với mọi $i,\overset{-1}{p}(A_i)$ là một phủ của $A_i,E'$ khi đó là một phủ của $B'$, do đó E là một phủ của B.

#### Hệ quả 2 {#ta-iv-s4-prop-6-cor-2 .statement tag=022L}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ thực sự, tách được và toàn ánh. Giả sử thêm một trong các giả thiết sau:

(i) Các thớ của $f$, cũng như không gian $X\times_YX$, là liên thông địa phương;

(ii) Các thớ của $f$ là hữu hạn, đường chéo $\Delta_X$ của $X\times_YX$ là mở trong $X\times_YX$ và không gian $(X\times_YX)-\Delta_X$ là liên thông địa phương. Khi đó mọi dữ liệu giảm cấp tương đối với $f$ trên một phủ của X là hiệu dụng, và không gian thương là một phủ của Y.

Cho Z là một phủ của X và cho $\tau$ là một dữ liệu giảm cấp tương đối với $f$ trên Z. Theo mệnh đề 5 (IV, p. 389), dữ liệu giảm cấp $\tau$ là hiệu dụng, nói cách khác hình vuông

Z $Z/R_{\tau}$

X $^f$ Y

là một hình vuông Descartes. Các giả thiết của mệnh đề 6 (IV, p. 391) khi đó được thỏa mãn. Do đó, $Z/R_{\tau}$ là một phủ của Y.

#### Mệnh đề 7 {#ta-iv-s4-prop-7 .statement tag=022M}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục và toàn ánh. Giả sử rằng không gian Y là không cuộn được và rằng ánh xạ $f$ là mở và có tính chất nâng đường. Khi đó mọi dữ liệu giảm cấp tương đối với $f$ trên một phủ của X là hiệu dụng, và không gian thương là một phủ của Y.

Cho $(Z, p)$ là một phủ của X và cho $\tau$ là một dữ liệu giảm cấp tương đối với $f$ trên Z. Vì ánh xạ $f$ là toàn ánh và mở, suy ra từ mệnh đề 5 của IV, p. 389, rằng dữ liệu giảm cấp $\tau$ là hiệu dụng. Đặt $T = Y/R_{\tau}$; đó là không gian Y thương; phép chiếu của nó $q$ là étale (loc. cit.); nó cũng là tách được (I, p. 27, mệnh đề 4).

Theo giả thiết, ánh xạ $f$ có tính chất nâng đường đi, và ánh xạ $p$ cũng vậy, vì Z là một phủ của X (III, p. 302, Hệ quả 2 của Mệnh đề 3). Do đó điều tương tự đúng đối với ánh xạ $p\circ f$, và vì thế đối với ánh xạ $q$. Do đó (xem IV, p. 341, Nhận xét 2), T là một phủ của Y. Mệnh đề do đó được chứng minh.

#### Nhận xét {#ta-iv-s4-n5-rem-1 .statement tag=022N}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ. Để mọi dữ liệu hạ giáng đối với $f$ trên một phủ của X đều hiệu dụng, và để không gian thương là một phủ của Y, thì cần thiết rằng $f$ là ngặt và rằng $f(X)$ là một tập con mở và đóng của X.

Thật vậy, ta đồng nhất không gian X với $X\times_YY$ và trang bị cho nó dữ liệu hạ giáng chính tắc của nó đối với $f$. Không gian thương được đồng nhất với $f(X)$, được trang bị tôpô thương của tôpô của X đối với quan hệ tương đương xác định bởi $f$. Nếu đây là một phủ của Y, thì không gian $f(X)$ khi đó được đồng nhất với một tập con mở và đóng của Y và ánh xạ $f$ là ngặt.

### 6. Hạ giáng của nhómoid

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow Y$ là một ánh xạ liên tục. Gọi $p_1$ và $p_2$ là hai phép chiếu của $X\times_YX$ vào X, Coeg($f$) là nhómoid đồng điều của cặp $(\varpi (p_1), \varpi (p_2))$ các cấu xạ nhómoid từ $\varpi (X\times_YX)$ vào $\varpi (X)$, và $\gamma :\varpi (X)\rightarrow$ Coeg($f$) là cấu xạ nhómoid chính tắc (II, p. 199, Định nghĩa 2). Vì $f\circ p_1=f\circ p_2$, ta có $\varpi (f)\circ \varpi (p_1) =\varpi (f)\circ \varpi (p_2)$. Khi đó suy ra từ tính chất phổ quát của các đồng điều (II, p. 199, Mệnh đề 3) rằng tồn tại duy nhất một cấu xạ nhómoid $\varpi '(f):$ Coeg($f$)$\rightarrow \varpi (Y)$ sao cho $\varpi (f) =\varpi '(f)\circ \gamma$.

Tập hợp các đỉnh của Coeg($f$) là tập thương của tập hợp X = Som($\varpi (X)$) bởi quan hệ tương đương xác định bởi $f($II, p. 200, Nhận xét 1). Nó được đồng nhất với $f(X)$.

#### Mệnh đề 8 {#ta-iv-s4-prop-8 .statement tag=022O}

Cho X và Y là các không gian tôpô khác rỗng và cho $f$ là một ánh xạ liên tục từ X vào Y. Giả sử rằng không gian X là liên thông cung địa phương, rằng không gian Y là liên thông, và rằng ánh xạ $f$ là ngặt và toàn ánh. Khi đó nhómoid Coeg($f$) là bắc cầu.

Gọi Γ là quiver mà tập hợp các đỉnh là X và tập hợp các mũi tên của nó là tập hợp tổng của Fl($\varpi (X)$) và $X\times_YX$, các ánh xạ gốc và đích là các ánh xạ của $\varpi (X)$ trên Fl($\varpi (X)$) và các ánh xạ $p_1$ và $p_2$ trên $X\times_YX$. Theo định nghĩa của khung của cặp $(\varpi$(pr$_1$)$, \varpi$(pr$_2$)) (II, p. 185, Định nghĩa 3) và Nhận xét 2 của II, p. 200, tập hợp các quỹ đạo của Coeg($f$) được đồng nhất với tập hợp các thành phần liên thông của quiver Γ. Vì không gian X khác rỗng, chỉ cần chứng minh rằng đồ thị Γ là liên thông.

Các thành phần liên thông của Γ là bão hòa đối với quan hệ tương đương “tồn tại một đường đi nối $x$ với $x'$”, và do đó là mở trong X, vì X là liên thông cung địa phương. Khi đó chúng cũng đóng. Chúng cũng là bão hòa đối với quan hệ tương đương R xác định bởi $f$. Theo giả thiết, ánh xạ $f$ cảm sinh một đồng phôi từ $X/R$ lên Y, do đó ảnh theo $f$ của mọi thành phần liên thông của Γ là một tập con mở và đóng của Y, và vì thế bằng Y vì không gian Y được giả thiết là liên thông.

Cho C là một thành phần liên thông của Γ, và cho $x$ là một điểm của X. Từ điều đã nêu trước đó, tồn tại một điểm $x'\in C$ sao cho $f(x') =f(x)$. Theo định nghĩa của quiver Γ, ta có $x'\in C$. Vậy C = X và do đó quiver Γ là liên thông.

#### Mệnh đề 9 {#ta-iv-s4-prop-9 .statement tag=022P}

Cho X và Y là các không gian tôpô và $f$ là một ánh xạ liên tục từ X vào Y. Giả sử không gian X địa phương liên thông cung, không gian Y đơn liên, và ánh xạ $f$ ngặt và toàn ánh. Khi đó nhóm giao $\varpi (Y)$ được sinh bởi ảnh của $\varpi (X)$ qua $\varpi (f)$.

Ta có thể giả sử các không gian X và Y khác rỗng. Ký hiệu G là nhóm giao con của $\varpi (Y)$ được sinh bởi ảnh của $\varpi (X)$ qua $\varpi (f)$. Vì ánh xạ $f$ là toàn ánh, tập hợp các đỉnh của G bằng Y. Theo mệnh đề 8, Coeg($f$) là một nhóm giao bắc cầu. Vì $\varpi '(f)$ cảm sinh đồng nhất trên các đỉnh, ảnh của Coeg($f$) qua $\varpi '(f)$ là một nhóm giao con bắc cầu của $\varpi (Y)$. Ảnh của $\varpi (X)$ qua $\gamma$ sinh Coeg($f$) (II, p. 200, hệ quả); vì có $\varpi (f) =$ $\varpi '(f)\circ \gamma$, nhóm giao G là bắc cầu.

Cho $y_0$ là một điểm của Y và H là nhóm con $G_{y_0}$ của $\pi_1(Y, y_0)$. Theo Định lý 1 của IV, p. 342, tồn tại một phủ liên thông $(T, p)$ của Y và một điểm $t_0$ của thớ $T_{y_0}$ mà H là nhóm ổn định của nó.

Nếu $x$ là một điểm của X, tập hợp Fl$_{y_0,f(x)}(G)$ không rỗng, vì G là bắc cầu. Với $u\in$ Fl$_{y_0,f(x)}(G)$, điểm $t_0\cdot u$ là một điểm của thớ $T_{f(x)}$, độc lập với $u$ vì nhóm H, nhóm đẳng hướng của G tại $y_0$, giữ cố định $t_0$. Ký hiệu điểm này là $\sigma (x)$; ký hiệu $\sigma : X\rightarrow T$ là ánh xạ thu được và $s: X\rightarrow X\times_YT$ là ánh xạ $x\mapsto (x, \sigma (x))$. Theo phép dựng, ánh xạ $s$ tương thích với các phép toán chính tắc của $\varpi (X)$ trên X và $X\times_YT$. Do đó, theo bổ đề 1 của III, p. 312, $s$ liên tục. Vì vậy ánh xạ $\sigma$ liên tục; hơn nữa nó tương thích với quan hệ tương đương xác định bởi $f$, vì $\sigma (x)$ chỉ phụ thuộc vào $f(x)$. Vì $f$ ngặt và toàn ánh, tồn tại duy nhất một ánh xạ liên tục $\overline{\sigma}: Y\rightarrow T$ sao cho $\overline{\sigma}\circ f=\sigma$, do đó phủ T có một tiết diện. Vì T liên thông, ánh xạ $p: T\rightarrow Y$ là một đồng phôi (I, p. 31, hệ quả 4 của mệnh đề 6), và ta có $H =\pi_1(Y, y_0)$, do đó $G_{y_0}=\pi_1(Y, y_0)$. Vì G là bắc cầu, suy ra $G =\varpi (Y)$.

#### Mệnh đề 10 {#ta-iv-s4-prop-10 .statement tag=022Q}

Cho X và Y là các không gian tôpô và $f$ là một ánh xạ liên tục từ X vào Y. Giả sử không gian X đơn liên, không gian $X\times_YX$ địa phương liên thông cung, và mọi dữ liệu hạ xuống đối với $f$ trên một phủ của X đều hiệu dụng và không gian thương là một phủ của Y. Khi đó cấu xạ nhóm giao $\varpi '(f)$ của Coeg($f$) vào $\varpi (Y)$ là đơn ánh.

Dưới các giả thiết của mệnh đề, $f$ là ngặt ( IV, p. 394, nhận xét); hơn nữa, ta có thể giả sử rằng nó là toàn ánh.

#### Bổ đề 2 {#ta-iv-s4-lem-2 .statement tag=022R}

Ta giữ lại ký hiệu và các giả thiết của mệnh đề. Cho T là một tập hợp được trang bị một phép toán của groupoid Coeg($f$) tương đối với một ánh xạ $q: T\rightarrow Y$. Khi đó tồn tại một tôpô duy nhất trên T sao cho $q$ làm cho T trở thành một phủ của Y, sao cho đối với mọi lớp các đường đi có gốc $c$ trong X và mọi điểm $t$ của T, ta có $t\cdot \gamma (c) =t\cdot f_*(c)$. Đặc biệt, phép toán của Coeg($f$) trên T phân tích qua một phép toán của groupoid $\varpi (Y)$.

Tính duy nhất của một tôpô như vậy trên T suy ra từ Bổ đề 1 (III, p. 312); ta hãy chứng minh sự tồn tại của nó. Trang bị cho tập hợp $X\times_YT$ một luật phép toán của $\varpi (X)$ bằng cách đặt $(x, t)\cdot u= (x\cdot u, t\cdot \gamma (u))$ đối với mọi $(x, t)\in X\times_YT$ và mọi mũi tên $u$ có gốc $x$ trong $\varpi (X)$. Vì không gian X đơn liên, luật phép toán này của $\varpi (X)$ không có đơn môđrômi địa phương (III, p. 313, Nhận xét). Do đó tồn tại trên tập hợp $X\times_YT$ một tôpô duy nhất làm cho không gian X $(X\times_YT$, pr$_1)$ là một phủ của X và sao cho phép toán chính tắc của $\varpi (X)$ trong phủ này trùng với phép toán đã cho (III, p. 313, Mệnh đề 3). Ta ký hiệu phủ này bởi $(Z, p)$. Ta hãy chứng minh rằng ánh xạ $\tau : ((x_1, t), x_2)\mapsto (x_2, t)$ từ $Z\times_YX$ vào Z là một dữ kiện xuống cấp trên Z tương đối với ánh xạ $f$. Chỉ cần kiểm tra rằng nó liên tục, các điều kiện khác của Định nghĩa 1 của IV, p. 382, là hiển nhiên.

Ánh xạ $\tau$ là một phép nâng của ánh xạ pr$_2: Z\times_YX\rightarrow X$ lên phủ Z của X. Vì không gian $X\times_YX$ liên thông địa phương theo cung, không gian $Z\times_YX$, là một phủ của nó, cũng liên thông địa phương theo cung. Theo Hệ quả (III, p. 269), để chứng minh rằng ánh xạ $\tau$ liên tục, chỉ cần chứng minh rằng nó liên tục theo cung.

Do đó, hãy cho $\widetilde{c}= ((c, g), c')$ là một đường đi trong $Z\times_YX$ và hãy chứng minh rằng ánh xạ $\tau \circ \widetilde{c}:t\mapsto (c'(t), g(t))$ của $\mathbf{I}$ vào Z là liên tục. Với mọi $s\in [0,1]$, ta ký hiệu bởi $c_s$ và $c'_s$ các đường đi trong X được xác định bởi $t\mapsto c(st)$ và $t\mapsto c'(st)$. Với mọi $s\in [0,1]$, do đó ta có $c(s) =c(0)\cdot [c_s]$, $c'(s) =c'(0)\cdot [c'_s]$ và $(c, g)(s) = (c(0), g(0))\cdot [c_s]$, trong đó $[u]$ ký hiệu lớp đồng luân ngặt của một đường đi $u($III, p. 304, Nhận xét). Ánh xạ $t\mapsto (c_s(t), c'_s(t))$ là một đường đi trong $X\times_YX$; theo định nghĩa của coequalizer Coeg($f$), do đó ta có $\gamma ([c_s]) =\gamma ([c'_s])$ và $g(s) =g(0)\cdot \gamma ([c_s]) =$ $g(0)\cdot \gamma ([c'_s])$. Theo định nghĩa của phép toán của $\varpi (X)$ trên Z, do đó ta có

$$
(\tau \circ \widetilde{c})(s) = (c'(s), g(s)) = (c'(0)\cdot [c'_s], g(0)\cdot \gamma ([c'_s]))
$$

$$
= (c'(0), g(0))\cdot [c'_s] = (\tau \circ \widetilde{c})(0)\cdot [c'_s]
$$

Điều này chứng minh rằng $\tau \circ \widetilde{c}$ là một phép nâng liên tục lên Z của đường đi $c'($loc. cit.). Do đó, ánh xạ $\tau$ liên tục theo cung, suy ra liên tục; nó là một dữ kiện xuống cấp tương đối với $f$ trên không gian X Z.

Let $R_{\tau}$ là quan hệ tương đương được xác định bởi dữ liệu descent $\tau$. Vì ánh xạ $f$ là toàn ánh, ánh xạ pr$_2: Z\rightarrow T$ cảm sinh, bằng cách chuyển qua thương, một song ánh từ $Z/R_{\tau}$ lên T. Trang bị cho T tôpô suy ra từ tôpô của $Z/R_{\tau}$ bằng phép chuyển cấu trúc, sao cho $(T, q)$ là một không gian-Y. Theo giả thiết, do đó T là một phủ của Y và biểu đồ

Z $^{pr_2}$ T

$pq$

X $^f$ Y

là một bình phương Descartes.

Cho $(x, t)$ là một điểm của Z, $c$ là một đường đi có điểm đầu $x$ trong X, và $\widetilde{c}$ là phép nâng liên tục của $c$ lên Z có điểm đầu $(x, t)$. Đường đi pr$_2\circ \widetilde{c}$ là phép nâng có điểm đầu $t$ của đường đi $f\circ c$ trong Y, do đó $t\cdot \gamma ([c]) =$ $t\cdot [f\circ c] =t\cdot f_*([c])$. Điều này hoàn tất chứng minh bổ đề.

Bây giờ chứng minh mệnh đề. Cho $u$ và $v$ là hai mũi tên của Coeg($f$) có các ảnh trong $\varpi (Y)$ bằng nhau. Vì cấu xạ groupoid $\varpi '(f)$ là đồng nhất trên các tập đỉnh, các mũi tên $u$ và $v$ có cùng điểm đầu và cùng điểm cuối. Ký hiệu $y$ là điểm đầu của $u$; gọi T là tập hợp các mũi tên của Coeg($f$) có điểm đầu $y$, và gọi $q: T\rightarrow Y$ là hạn chế vào T của ánh xạ điểm cuối. Groupoid Coeg($f$) tác động bằng phép hợp thành ở bên phải trên tập hợp T, đối với $q$. Theo bổ đề 2, các tác động của $u$ và $v$ trên T là đồng nhất. Do đó $u=$ $e_y\cdot u=e_y\cdot v=v$. Điều này chứng minh rằng cấu xạ groupoid $\varpi '(f)$ là đơn ánh.

#### Định lý 1 {#ta-iv-s4-thm-1 .statement tag=022S}

Cho X và Y là các không gian tôpô, và $f: X\rightarrow$ Y là một ánh xạ liên tục toàn ánh. Giả sử rằng các không gian X và Y liên thông đường địa phương và liên thông đơn địa phương. Cuối cùng, giả sử một trong các tính chất sau được thỏa mãn:

(i) Ánh xạ $f$ là thực sự, tách được, có các thớ liên thông địa phương, và không gian $X\times_YX$ liên thông đường địa phương;

(ii) Ánh xạ $f$ là thực sự, tách được, có các thớ hữu hạn, đường chéo $\Delta_X$ là mở trong $X\times_YX$, và phần bù của nó liên thông địa phương;

(iii) Ánh xạ $f$ là mở và có tính chất nâng đường đi. Khi đó cấu xạ groupoid $\varpi '(f)$ là một đẳng cấu của groupoid Coeg($f$) lên groupoid Poincaré $\varpi (Y)$.

Trước hết hãy chú ý rằng dưới các giả thiết này, ánh xạ $f$ là toàn ánh và ngặt (I, p. 18, ví dụ 2). Hơn nữa, mọi dữ liệu descent đối với $f$ trên một phủ của X đều hiệu dụng, và không gian thương là một phủ của Y; điều này thực sự suy ra từ IV, p. 393, hệ quả 2 của mệnh đề 4 dưới các giả thiết (i) và (ii), và từ mệnh đề 7 của IV, p. 394 dưới giả thiết (iii). Theo mệnh đề 10, cấu xạ groupoid $\varpi '(f)$ do đó là đơn ánh và ảnh của nó là một groupoid con của $\varpi (Y)$.

Theo mệnh đề 9 của IV, p. 395, ảnh này bằng $\varpi (Y)$ dưới các giả thiết (i) và (ii), nhưng cũng dưới giả thiết (iii), vì khi đó cấu xạ groupoid $\varpi (f)$ là toàn ánh.

Do đó, $\varpi '(f)$ là một đẳng cấu.

#### Ví dụ {#ta-iv-s4-n6-exa-1 .statement tag=022T}

Sau đây là hai ví dụ trong đó các giả thiết của định lý 1 được thỏa mãn.

1) Cho Y là một không gian tôpô đơn liên. Cho $(A_i)_{i\in I}$ là một phủ hữu hạn địa phương của Y bởi các tập hợp đóng. Giả sử rằng, với mọi $i\in I$, không gian $A_i$ là đơn liên và rằng, với mọi cặp $(i, j)\in I\times I$, không gian $A_i\cap A_j$ là liên thông đường địa phương. Ta có thể lấy X là không gian tổng của họ $(A_i)_{i\in I}$ và lấy $f: X\rightarrow Y$ là ánh xạ suy ra từ họ các phép nhúng chính tắc.

2) Cho G là một nhóm rời rạc tác động thực sự trên một không gian tôpô đơn liên X, đặt $Y = X/G$ và cho $f: X\rightarrow Y$ là ánh xạ chính tắc. Nó là mở (TG, III, p. 10, bổ đề 2) và có tính chất nâng đường nhờ Định lý 4 của III, p. 287. Không gian Y là đơn liên theo IV, p. 349, Mệnh đề 8, b). Theo giả thiết, ánh xạ từ $G\times X$ vào $X\times X$ cho bởi $(g, x)\mapsto (g\cdot x, x)$ là thực sự, do đó ngặt (I, p. 18, Ví dụ 2) và ảnh của nó là $X\times_YX$. Khi đó suy ra từ III, p. 261, Mệnh đề 8 rằng $X\times_YX$ là liên thông đường địa phương.

### 7. Sự hạ xuống bởi một ánh xạ étale và toàn ánh

Cho X và Y là các không gian tôpô và cho $f$ là một ánh xạ liên tục từ X vào Y. Ta giữ lại ký hiệu của Số trước.

#### Định lý 2 {#ta-iv-s4-thm-2 .statement tag=022U}

Giả sử rằng mọi điểm của Y đều có một lân cận phía trên đó tồn tại một tiết diện liên tục của ánh xạ $f$. Cấu xạ nhómoid $\varpi '(f)$ từ Coeg($f$) vào $\varpi (Y)$ là một đẳng cấu.

Theo giả thiết, tồn tại một phủ $(U_j)_{j\in J}$ của Y bởi các tập hợp mở và, với mọi $j\in J$, một tiết diện liên tục $s_j$ của $f_{U_j}$.

Nếu $c$ là một đường trong X, ta ký hiệu bởi $[c]$ lớp đồng luân ngặt của nó trong $\varpi (X)$ và bởi $\{c\}$ ảnh của $[c]$ trong Coeg($f$) bởi cấu xạ nhómoid $\varpi '(f)$. Nếu $c$ và $c'$ là hai đường trong X$,\{c\}$ và $\{c'\}$ khả hợp thành trong Coeg($f$) khi và chỉ khi các đường $f\circ c$ và $f\circ c'$ trong Y được ghép liền nhau.

Cho $c'$ là một đường trong Y. Theo Bổ đề 4 của III, p. 272, được áp dụng

đến không gian compact $\mathbf{I}$ và đến phủ ($(^-{c'}^1)(U_j)$)$_{j\in J}$ của $\mathbf{I}$, tồn tại một số nguyên $n$ sao cho, với mọi số nguyên $k$ thỏa mãn $1\leqslant k\leqslant n$, ảnh của khoảng $[\frac{k-1}{n},\frac{k}{n}]$ qua $c'$ được chứa trong một tập mở $U_{j(k)}$. Với mọi số nguyên $k,1\leqslant k\leqslant n$, đặt $c'_k$ là đường đi trong Y được xác định bởi $s\mapsto c'(\frac{k+s-1}{n})$; ta có $[c'] = [c'_1][c'_2]. . .[c'_n]$ (xem III, p. 291, nhận xét 1), và $c'$ là đường đi được ký hiệu bởi $c'_1*c'_2* \cdots  *c'_n$. Với mọi $k\in  \{1, . . . , n\}$, ta ký hiệu $c_k$ là đường đi $s_{j(k)}\circ c'_k$ trong X và đặt $\{c_k\}=\gamma ([c_k])$. Vì với mọi $k$, các đường đi $c'_{k-1}=f\circ c_{k-1}$ và $c'_k=f\circ c_k$ có thể ghép liền với nhau, dãy $(\{c_1\}, . . . ,\{c_n\})$ là khả hợp thành trong Coeg($f$). Theo phép dựng,

$$
\varpi '(f)(\{c_1\}. . .\{c_n\}) =\varpi '(f)(\{c_1\}). . . \varpi '(f)(\{c_n\})
$$

$$
=\varpi (f)([c_1]). . . \varpi (f)([c_n])
$$

$$
= [f\circ c_1]. . .[f\circ c_n]
$$

$$
= [c'_1]* \cdots  *[c'_n] = [c']
$$

điều này chứng minh rằng cấu xạ nhómoid $\varpi '(f)$ là toàn ánh.

Cho $u$ và $v$ là các mũi tên của Coeg($f$). Vì nhómoid Coeg($f$) được sinh bởi ảnh của $\varpi (X)$ (II, p. 200, hệ quả), tồn tại các dãy hữu hạn $(c_1, . . . , c_n)$ và $(d_1, . . . , d_n)$ gồm các đường đi trong X sao cho $u=\{c_1\}. . .\{c_n\}$ và $v=\{d_1\}. . .\{d_n\}$. Các đường đi $(f\circ c_1, . . . , f\circ c_n)$ trong Y khi đó có thể ghép liền với nhau và ta có $\varpi '(f)(u) = [(f\circ c_1)]. . .[(f\circ$ $c_n)]$; tương tự, $\varpi '(f)(v) = [(f\circ d_1)]. . .[(f\circ d_n)]$.

Giả sử ta có $\varpi '(f)(u) =\varpi '(f)(v)$. Khi đó tồn tại một đồng luân ngặt $\sigma$ nối $(f\circ c_1)* \cdots  *(f\circ c_n)$ với $(f\circ d_1)* \cdots  *(f\circ d_n)$. Theo bổ đề 4 của III, p. 272, áp dụng cho không gian compact $\mathbf{I}\times \mathbf{I}$ và cho phủ $(\overset{-1}{\sigma}(U_i))_{i\in I})$ của $\mathbf{I}\times \mathbf{I}$, tồn tại một số nguyên $m\geqslant 1$ sao cho, với mọi cặp số nguyên $(j, k)$ thỏa mãn $1\leqslant j\leqslant m$ và $1\leqslant k\leqslant m$, ảnh của $[\frac{j-1}{m},\frac{j}{m}]\times [\frac{k-1}{m},\frac{k}{m}]$ qua $\sigma$ được chứa trong một tập mở $U_{i(j,k)}$ của phủ $(U_i)_{i\in I}$.

Mọi đường đi $c$ trong X đều có dạng $c_1* \cdots  *c_m$, trong đó $c_k$ là đường đi $t\mapsto c(\frac{k-1+t}{m})$. Thay thế các số nguyên $m$ và $n$ bằng tích $mn$ nếu cần, do đó ta có thể giả sử rằng $m=n$.

Với mỗi cặp $(j, k)$ các số nguyên của $\{1, . . . , n\}$ và mỗi cặp $(s, t)\in$ $\mathbf{I}\times \mathbf{I}$, đặt

$$
\sigma_{j,k}(s, t) =s_{i(j,k)}\circ \sigma (\frac{s + j- 1}{n},\frac{t + k- 1}{n})
$$

Với $t\in \mathbf{I}$, cũng đặt $h^0_{j,k}(t) =\sigma_{j,k}(t,0)$, $h^1_{j,k}(t) =\sigma_{j,k}(t,1)$, $v^0_{j,k}(t) =\sigma_{j,k}(0, t)$ và $v_{j,k}^1(t) =\sigma_{j,k}(1, t)$. Theo bổ đề 1 của III, p. 295, các đường đi $h^0_{j,k}*v_{j,k}^1$ và $v_{j,k}^0*h^1_{j,k}$ là đồng luân chặt, do đó có quan hệ

$$
[h^0_{j,k}][v_{j,k}^1] = [v_{j,k}^0][h^1_{j,k}] \tag{2}
$$

trong $\varpi (X)$, với mọi cặp $(j, k)\in  \{1, . . . , n\}^2$. Mặt khác, với mọi cặp số nguyên $(j, k)$, với 2 $\leqslant j\leqslant n$ và 1 $\leqslant k\leqslant n$, ta có $f\circ v_{j,k}^0=f\circ v_{j-1,k}^1$, do đó có quan hệ

$$
\{v^0_{j,k}\}=\{v_{j-1,k}^1\} \tag{3}
$$

trong Coeg($f$). Tương tự, với mọi cặp số nguyên $(j, k)$ sao cho $1\leqslant j\leqslant n$ và $2\leqslant k\leqslant n$, ta có

$$
\{h^0_{j,k}\}=\{h^1_{j,k-1}\} \tag{4}
$$

Với $j\in  \{1, . . . , n\}$, các đường đi $f\circ c_j$ và $f\circ h^0_{j,1}$ trùng nhau. Theo định nghĩa của coequalizer Coeg($f$), do đó ta có $\{c_j\}=\{h^0_{j,1}\}$. Tương tự, với mọi $j\in  \{1, . . . , n\},\{d_j\}=\{h^1_{j,n}\}$. Do đó ta có các quan hệ

$$
u=\{h^0_{1,1}\}. . .\{h^0_{n,1}\},v=\{h^1_{1,n}\}. . .\{h^1_{n,n}\}
$$

Theo bổ đề 3 dưới đây, ta có

$$
\{h^0_{1,1}\}. . .\{h^0_{1,n}\}\{v_{1,n}^1\}. . .\{v^1_{n,n}\}=\{v_{1,1}^0\}. . .\{v_{n,1}^0\}\{h^1_{n,1}\}. . .\{h^1_{n,n}\}
$$

Vì các đường đi $t\mapsto \sigma (0, t)$ và $t\mapsto \sigma (1, t)$ là hằng, ta có, với $1\leqslant k\leqslant n,\{v^0_{1,k}\}=e_a$ và $\{v^1_{n,k}\}=e_b$ trong đó $a$ và $b\in Y$ là gốc và ngọn của các mũi tên $u$ và $v$ của Coeg($f$). Suy ra

$$
\{h^0_{1,1}\}. . .\{h^0_{1,n}\}=\{h^0_{n,1}\}. . .\{h^1_{n,n}\}
$$

nghĩa là, $u=v$.

#### Bổ đề 3 {#ta-iv-s4-lem-3 .statement tag=022V}

Cho G là một nhómoid và cho $p, q$ là các số nguyên $\geqslant 1$. Với mỗi cặp $(j, k)$ các số nguyên sao cho $0\leqslant j\leqslant p$ và $0\leqslant k\leqslant q$, cho $x_{j,k}$ là một đỉnh của G; với mỗi cặp $(j, k)$ sao cho $1\leqslant j\leqslant p$ và $0\leqslant k\leqslant q$, cho $h_{j,k}$ là một mũi tên của G nối $x_{j-1,k}$ với $x_{j,k}$; với mỗi cặp $(j, k)$ sao cho $0\leqslant j\leqslant p$ và $1\leqslant k\leqslant q$, cho $v_{j,k}$ là một mũi tên của G nối $x_{j,k-1}$ với $x_{j,k}$.

Giả sử rằng, với mỗi cặp $(j, k)$ các số nguyên sao cho $1\leqslant j\leqslant p$ và $1\leqslant k\leqslant q$, các mũi tên $v_{j-1,k}$ và $h_{j,k}$ có thể hợp thành, tương tự các mũi tên $h_{j,k-1}$ và $v_{j,k}$, và ta có $v_{j-1,k}h_{j,k}=h_{j,k-1}v_{j,k}$. Khi đó,

$$
h_{1,0}h_{2,0}. . . h_{p,0}v_{p,1}v_{p,2}. . . v_{p,q}=v_{0,1}v_{0,2}. . . v_{0,q}h_{1,q}h_{2,q}. . . h_{p,q}
$$

Trước hết ta xét trường hợp riêng khi $q= 1$ và chứng minh kết quả bằng quy nạp theo $p$. Nếu $p= 1$, mệnh đề cần chứng minh là đúng theo giả thiết; giả sử nó đúng với $p-1$; khi đó ta có

$$
h_{1,0}h_{2,0}. . . h_{p,0}v_{p,1}=h_{1,0}h_{2,0}. . . h_{p-1,0}v_{p-1,1}h_{p,1}=v_{0,1}h_{1,1}. . . h_{p,1}
$$

theo giả thiết quy nạp, do đó có quan hệ đối với $p$.

Bây giờ ta chứng minh kết quả bằng quy nạp theo $q$. Kết quả đúng với $q= 1$ theo điều đã nêu trước; nếu nó đúng với $q-1$, khi đó ta có

$$
h_{1,0}h_{2,0}. . . h_{p,0}v_{p,1}v_{p,2}. . . v_{p,q}=v_{0,1}v_{0,2}. . . v_{0,q-1}h_{1,q-1}. . . h_{p,q-1}v_{p,q}
$$

Từ trường hợp $q= 1$, ta có

$$
h_{1,q-1}. . . h_{p,q-1}v_{p,q}=v_{0,q}h_{1,q}. . . h_{p,q}
$$

do đó có quan hệ cần thiết.

#### Ví dụ 1 {#ta-iv-s4-n7-exa-1 .statement tag=022W}

Định lý áp dụng khi ánh xạ $f$ là étale và toàn ánh.

#### Ví dụ 2 {#ta-iv-s4-n7-exa-2 .statement tag=022X}

Nó cũng áp dụng khi không gian X là không gian tổng của một họ $(V_i)_{i\in I}$ các phần của Y mà các phần trong của chúng phủ Y, và khi $f$ là ánh xạ cảm sinh bởi các đơn ánh chính tắc của mỗi $V_i$ vào Y.

### 8. Nhómoid Poincaré của một Không gian thương

Cho X là một không gian tôpô được trang bị một tác động liên tục của một nhóm rời rạc G; đặt $Y = X/G$ và ký hiệu $f: X\rightarrow$ Y là ánh xạ chính tắc. Ký hiệu $|G|$ là nhómoid $\varpi (G)$; tập hợp các đỉnh của nó là G; với $g, g'\in G$, tồn tại một mũi tên duy nhất nối $g$ với $g'$ nếu $g'=g'$, và không có mũi tên nào trong trường hợp khác. Bằng cách chuyển qua các nhómoid cơ bản, tác động $m: G\times X\rightarrow X$ cảm sinh một cấu xạ của các nhómoid $\varpi (m):|G| \times \varpi (X)\rightarrow \varpi (X)$. Cho $\varpi (X)/G$ là đối đẳng cấu của hai cấu xạ của các nhómoid $\varpi (m)$ và $\varpi$(pr$_2$) từ $|G| \times \varpi (X)$ đến $\varpi (X)$; ký hiệu $\beta :\varpi (X)\rightarrow \varpi (X)/G$ là cấu xạ chính tắc của các nhómoid. Ta có $f\circ m=f\circ$ pr$_2$, do đó $\varpi (f)\circ \varpi (m) =\varpi (f)\circ \varpi$(pr$_2$). Theo tính chất phổ quát của các đối đẳng cấu, tồn tại do đó một cấu xạ duy nhất của các nhómoid $\varpi ''(f):\varpi (X)/G\rightarrow \varpi (Y)$ sao cho $\varpi (f) =\varpi ''(f)\circ \beta$.

#### Định lý 3 {#ta-iv-s4-thm-3 .statement tag=022Y}

Cho X là một không gian tôpô delaceable và G là một nhóm rời rạc tác động đúng trong X; cho $f: X\rightarrow X/G$ là toàn cấu chính tắc. Cấu xạ chính tắc của các nhómoid $\varpi ''(f):\varpi (X)/G\rightarrow \varpi (X/G)$ được đưa vào ở trên là một đẳng cấu.

Ký hiệu Coeg($f$) là đối đẳng cấu của hai cấu xạ của các nhómoid từ $\varpi (X\times_YX)$ đến $\varpi (X)$ cảm sinh bởi các phép chiếu pr$_1$ và pr$_2$; ký hiệu $\gamma :\varpi (X)\rightarrow$ Coeg($f$) là cấu xạ chính tắc của các nhómoid. Vì ảnh của ánh xạ $(m$, pr$_2): G\times X\rightarrow X\times X$ là không gian con $X\times_YX$ của $X\times X$, hai cấu xạ của các nhómoid $\gamma \circ \varpi (m)$ và $\gamma \circ \varpi$(pr$_2$), từ $|G|\times \varpi (X)$ đến Coeg($f$), là bằng nhau. Theo tính chất phổ quát của $\varpi (X)/G$, tồn tại một cấu xạ duy nhất của các nhómoid $\alpha :\varpi (X)/G\rightarrow$ Coeg($f$) sao cho $\gamma =\alpha \circ \beta$.

Gọi thêm $\varpi '(f)$ là cấu xạ duy nhất của các nhómoid từ Coeg($f$) đến $\varpi (Y)$ sao cho $\varpi (f) =\varpi '(f)\circ \gamma$. Theo IV, p. 399, Ví dụ 2, các giả thiết của Định lý 1 của IV, p. 398 được thỏa mãn và cấu xạ $\varpi '(f)$ là một đẳng cấu. Vì

$$
\varpi (f) =\varpi '(f)\circ \gamma =\varpi '(f)\circ \alpha \circ \beta =\varpi ''(f)\circ \beta
$$

ta có $\varpi ''(f) =\varpi '(f)\circ \alpha$. Do đó, để chứng minh Định lý 3, chỉ cần chứng minh rằng cấu xạ $\alpha$ là một đẳng cấu.

#### Bổ đề 4 {#ta-iv-s4-lem-4 .statement tag=022Z}

Với mọi đường đi $c= (c_1, c_2)$ trong $X\times_YX$, ta có $\beta ([c_1]) =\beta ([c_2])$.

Cho $c$ là một đường đi như vậy.

Cho $x\in X$, và cho $K_x$ là nhóm ổn định của nó trong G. Theo TG, III, p. 32, mệnh đề 8, tồn tại một lân cận mở $U_x$ của $x$ trong X sao cho $K_x\cdot U_x=$ $U_x,g\cdot U_x\cap U_x$ = $\emptyset$ với mọi $g\in$ G - $K_x$, và sao cho ánh xạ $f$ cảm sinh một đồng phôi từ $U_x/K_x$ lên một lân cận mở $V_x$ của $f(x)$ trong Y. Vì X là không gian không khả lộ và hạn chế của ánh xạ $f$ lên $U_x$ là mở và đóng, ta có thể giả sử thêm rằng $U_x$ là liên thông và rằng ảnh của đồng cấu chính tắc $\pi_1(U_x, x)\rightarrow \pi_1(X, x)$ được rút gọn về phần tử đơn vị. Các tập mở $(V_x)_{x\in X}$ được xây dựng như vậy tạo thành một phủ mở của Y. Theo bổ đề 4 của III, p. 272, áp dụng cho không gian compact $\mathbf{I}$ và các tập mở $(f\circ c_1)^{-1}(V_x)$ với $x\in X$, tồn tại một số nguyên $n\geqslant 1$ sao cho với mọi $i\in  \{1, . . . , n\}$, tồn tại một điểm $x_i$ trong X sao cho $c_1([\frac{i-1}{n},\frac{i}{n}])$

được chứa trong $\overset{-1}{f}(V_{x_i})$. Vì $f\circ c_1=f\circ c_2,c_2([\frac{i-1}{n},\frac{i}{n}])$ cũng

được chứa trong $\overset{-1}{f}(V_{x_i})$.

Với $j= 1$ hoặc 2 và với $i\in  \{1, . . . , n\}$, cho $c_{j,i}$ là đường đi trong X được xác định bởi $t\mapsto c_j(\frac{i+t-1}{n})$; ta có $c_j=c_{j,1}* \cdots  *c_{j,n}($III, p. 291, nhận xét 1). Do đó, để chứng minh rằng $\beta ([c_1]) =\beta ([c_2])$, chỉ cần chứng minh rằng $\beta ([c_{1,i}]) =\beta ([c_{2,i}])$ với mọi số nguyên $i\in  \{1, . . . , n\}$. Thay thế cặp đường đi $(c_1, c_2)$ bởi cặp $(c_{1,i}, c_{2,i})$ nếu cần thiết, ta giả sử rằng tồn tại $x\in X$ sao cho $(f\circ c_1)([0,1])\subset V_x$.

Ảnh ngược của $V_x$ bởi $f$ là hợp rời nhau của các thành phần liên thông $g\cdot U_x$, trong đó $g$ chạy qua một hệ các đại diện trong G của $G/K_x$. Với $i= 1$ hoặc 2, cho $g_i$ là một phần tử của G sao cho điểm $x_i=$ $g_i\cdot c_i(0)$ thuộc $U_x$. Ảnh của đường đi $g_i\cdot c_i$ khi đó được chứa trong $U_x$. Theo định nghĩa của groupoid $\varpi (X)/G$, ta có $\beta ([g_i\cdot c_i]) =\beta ([c_i])$, điều này cho phép giả sử rằng ảnh của các đường đi $c_1$ và $c_2$ được chứa trong $U_x$ và rằng $g_1=g_2=e$.

Với $s= 0$ hoặc 1, cho $d_s$ là một đường đi trong $U_x$ nối $x$ với $c_1(s)$ và cho $g_s$ là một phần tử của $K_x$ sao cho $g_s\cdot c_2(s) =c_1(s)$. Các đường đi $d_0*c_1*\overline{d_1}$ và $d_0*(g_0\cdot c_2)*(g_0g_1^{-1}\cdot \overline{d_1})$ là các vòng tại $x$ trong $U_x$. Do đó chúng đồng luân nghiêm ngặt trong X với vòng hằng tại $x$, vì ảnh của đồng cấu chính tắc $\pi_1(U_x, x)\rightarrow \pi_1(X, x)$ thu gọn về phần tử đơn vị. Các lớp của chúng đặc biệt có cùng ảnh qua cấu xạ groupoid $\beta$, do đó

$$
\beta ([d_0])\beta ([c_1])\beta ([d_1])^{-1}=\beta ([d_0])\beta ([g_0\cdot c_2])\beta ([g_0g_1^{-1}\cdot d_1])^{-1}
$$

Vì $\beta ([g\cdot c]) =\beta ([c])$ với mọi phần tử $g\in G$ và mọi đường đi $c$ trong X, suy ra $\beta ([c_1]) =\beta ([c_2])$, như cần chứng minh.

Theo bổ đề, hai cấu xạ groupoid $\beta \circ \varpi$(pr$_1$) và $\beta \circ \varpi$(pr$_2$) của $\varpi (X\times_YX)$ vào Coeg($f$) là bằng nhau. Theo tính chất phổ quát của đối đồng đẳng thức, do đó tồn tại duy nhất một cấu xạ groupoid $\alpha ':$ Coeg($f$)$\rightarrow \varpi (X)/G$ sao cho $\beta =\alpha '\circ \gamma$. Cấu xạ $\alpha '\circ \alpha$ là cấu xạ groupoid duy nhất $\varphi$ của $\varpi (X)/G$ vào chính nó sao cho $\varphi \circ \beta =\beta$; do đó $\alpha '\circ \alpha$ = Id$_{\varpi(X)/G}$. Tương tự, $\alpha \circ \alpha '=$ Id$_{Coeg(f)}$. Do đó, $\alpha$ là một đẳng cấu.

## BÀI TẬP {#ta-iv-s4-exercises}

Xem các [bài tập cho § 4](exercises/s4/).
