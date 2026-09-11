---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 4
section_title: Homotopie et revêtements
lang: vi
source: ta-i-iv-fr
book_pages: TA III.300-TA III.307, TA III.334
pdf_pages: 0316-0323, 0350-0350
extraction: native
subsections:
    - "no": 1
      title: Homotopie et revêtements
      page: 300
      pdf_page: 316
    - "no": 2
      title: Relèvement des chemins
      page: 301
      pdf_page: 317
    - "no": 3
      title: Opérations du groupoïde de Poincaré dans les revêtements
      page: 303
      pdf_page: 319
    - "no": 4
      title: Cas des revêtements associés à un revêtement principal
      page: 305
      pdf_page: 321
statements: 16
exercises: 1
content_sha256: 87f8991e9ab2be882b0716def516550a05fb7469a460d1c3d3c02d9d9efbb7f4
translated_from: content/en-mt/ta/III/04_s4_homotopie_et_revetements.md
source_lang: en-mt
translation_method: machine
source_content_sha256: f960904cd7e582f971e9ae716460b2848676516ab8cab1144e1942067c2951c5
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-f58b756c
glossary_version: 34
glossary_terms_sha256: 22abb67ab6e9894b89ecfaa5fbbaf3c2fc375398998a69295b41b763c00dcff1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. ĐỒNG LUÂN VÀ PHỦ

### 1. Đồng luân và phủ

#### Mệnh đề 1 {#ta-iii-s4-prop-1 .statement tag=01Z5}

Cho B là một không gian tôpô và E là một phủ của B. Cho $B'$ là một không gian tôpô và $f_0$ và $f_1$ là các ánh xạ liên tục từ $B'$ vào B. Nếu các ánh xạ $f_0$ và $f_1$ đồng luân, thì các phủ $f_0^*(E)$ và $f_1^*(E)$ của $B'$ đẳng cấu.

Cho $\sigma : B'\times \mathbf{I}\rightarrow B$ là một phép đồng luân nối $f_0$ với $f_1$. Ta ký hiệu $i_0$ và $i_1$ là các ánh xạ $x\mapsto (x,0)$ và $x\mapsto (x,1)$ từ $B'$ vào $B'\times \mathbf{I}$. Nếu $t\in  \{0,1\}$, ta có $f_t=\sigma \circ i_t$ và do đó các phủ $f_t^*(E)$ và $i^*_t(\sigma^*(E))$ của $B'$ đẳng cấu (I, p. 15). Vì không gian tôpô $\mathbf{I}$ liên thông địa phương và đơn liên (I, p. 127, hệ quả), các phủ $i^*_0(\sigma^*(E))$ và $i^*_1(\sigma^*(E))$ của $B'$ đẳng cấu (I, p. 130, hệ quả 1 của mệnh đề 8).

#### Hệ quả {#ta-iii-s4-n1-cor-1 .statement tag=01Z6}

Một không gian tôpô đồng luân với một không gian tôpô đơn liên là đơn liên.

Cho B và $B'$ là các không gian tôpô, cho $f: B\rightarrow B'$ là một tương đương đồng luân và cho $g: B'\rightarrow B$ là một ánh xạ liên tục, nghịch đảo của $f$ theo nghĩa đồng luân. Cho E là một phủ của B. Vì $g\circ f$ đồng luân với ánh xạ đồng nhất của B, nên phủ E đẳng cấu với phủ $f^*(g^*(E))$ (mệnh đề 1). Nếu không gian $B'$ đơn liên, phủ $g^*(E)$ là tầm thường hóa được. Do đó, phủ E là tầm thường hóa được. Điều này chứng minh rằng không gian B là đơn liên.

#### Nhận xét {#ta-iii-s4-n1-rem-1 .statement tag=01Z7}

Cho G là một nhóm tôpô rời rạc. Với ký hiệu của mệnh đề, giả sử E là một phủ chính với nhóm G. Khi đó các phủ $f_0^*(E)$ và $f_1^*(E)$ là các phủ chính đẳng cấu (I, p. 131, nhận xét).

#### Mệnh đề 2 (Nâng của các phép đồng luân) {#ta-iii-s4-prop-2 .statement tag=01Z8}

Cho B là một không gian tôpô và E là một phủ của B. Cho $B'$ là một không gian tôpô và $f_0$ và $f_1$ là các ánh xạ liên tục từ $B'$ vào B. Cho $\sigma : B'\times$ $\mathbf{I}\rightarrow B$ là một phép đồng luân nối $f_0$ với $f_1$. Cho $g_0: B'\rightarrow E$ là một phép nâng liên tục của $f_0$ lên E. Tồn tại duy nhất một ánh xạ liên tục $\widetilde{\sigma}: B'\times \mathbf{I}\rightarrow$ E nâng $\sigma$, là một phép đồng luân có số hạng ban đầu $g_0$. Số hạng $g_1: B'\rightarrow E$ của nó là một phép nâng liên tục của $f_1$ lên E.

Điều này suy ra từ hệ quả 3 của mệnh đề 8 của I, p. 130, áp dụng cho không gian tôpô $\mathbf{I}$ đơn liên và liên thông địa phương.

### 2. Nâng các đường

#### Mệnh đề 3 {#ta-iii-s4-prop-3 .statement tag=01Z9}

Cho B là một không gian tôpô và $p: E\rightarrow B$ là một phủ. Ta ký hiệu bằng $\widetilde{p}:\mathscr{C}_c(\mathbf{I}; E)\rightarrow \mathscr{C}_c(\mathbf{I}; B)$ ánh xạ $c\mapsto p\circ c$. Ta ký hiệu bằng $o_E:\mathscr{C}_c(\mathbf{I}; E)\rightarrow E$ ( resp. $o_B:\mathscr{C}_c(\mathbf{I}; B)\rightarrow B$) ánh xạ được xác định bởi $c\mapsto c(0)$. Khi đó, biểu đồ

$\mathscr{C}_c(\mathbf{I}; E)^{o_E}$ E

$\widetilde{p}p$

$\mathscr{C}_c(\mathbf{I}; B)^{o_B}$ B là một bình phương Descartes.

Không gian tôpô $\mathbf{I}$ liên thông địa phương, compact địa phương và đơn liên. Mệnh đề do đó suy ra từ mệnh đề 9 của I, p. 131, áp dụng với $T =\mathbf{I}$ và $t= 0$.

#### Hệ quả 1 {#ta-iii-s4-prop-3-cor-1 .statement tag=01ZA}

Ánh xạ $\widetilde{p}:\mathscr{C}_c(\mathbf{I}; E)\rightarrow \mathscr{C}_c(\mathbf{I}; B)$ là một phủ.

Điều này suy ra từ I, p. 71, hệ quả 2 của mệnh đề 1.

#### Hệ quả 2 (Nâng các đường đi) {#ta-iii-s4-prop-3-cor-2 .statement tag=01ZB}

Cho $p: E\rightarrow B$ là một phủ, cho $x$ là một điểm của E và $a=p(x)$. Ánh xạ $c\mapsto p\circ c$ là một phép đồng phôi của không gian $\Lambda_x(E)$ các đường đi trong E có gốc $x$ lên không gian $\Lambda_a(B)$ các đường đi trong B có gốc $a$.

Với ký hiệu của mệnh đề 3, ta có $\Lambda_a(B) =o^{-1}_B(a)$ và $\Lambda_x(E) =\overset{-1}{o_{E}}(x)$. Hệ quả khi đó suy ra từ I, p. 10, hệ quả của mệnh đề 4.

Ta sẽ nói rằng một ánh xạ liên tục $p: E\rightarrow B$ thỏa mãn tính chất nâng đường đi nếu, với mọi đường đi $c:\mathbf{I}\rightarrow$ B và mọi điểm $x$ của E nằm trên $c(0)$, tồn tại một đường đi $c'$ trong E có gốc $x$ nâng $c$. Khi đó một đường đi như vậy là duy nhất nếu $p$ étale và tách được (I, p. 34, hệ quả 1 của mệnh đề 11). Cho E là một phủ và $p$ là phép chiếu của nó; ánh xạ $p$ là étale, tách được và có tính chất nâng đường đi (hệ quả 2). Đối với đảo lại từng phần, cf. III, p. 315, hệ quả.

#### Mệnh đề 4 {#ta-iii-s4-prop-4 .statement tag=01ZC}

Cho $p: E\rightarrow B$ là một ánh xạ étale và tách được thỏa mãn tính chất nâng đường đi. Cho $a$ và $b$ là các điểm của B và cho $x$ là một điểm của E sao cho $p(x) =a$. Cho $c_0$ và $c_1$ là hai đường đi đồng luân ngặt nối $a$ với $b$ trong B. Các đường đi có gốc $x$ trong E lần lượt nâng $c_0$ và $c_1$ có cùng số hạng và đồng luân ngặt.

Cho $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow$ B là một đồng luân ngặt nối $c_0$ với $c_1$. Với $s\in \mathbf{I}$, cho $c'_s$ là đường đi duy nhất có gốc $x$ trong E nâng đường đi $t\mapsto \sigma (t, s)$. Với $(t, s)\in \mathbf{I}\times \mathbf{I}$, đặt $\sigma '(t, s) =c'_s(t)$; ta có $p\circ \sigma '=\sigma$. Ánh xạ $\sigma '$ là hằng trên $\{0\} \times \mathbf{I}$; theo cách dựng, nó liên tục trên $\mathbf{I}\times  \{s\}$ với mọi $s\in \mathbf{I}$. Do đó nó liên tục, theo I, p. 37, hệ quả 1 của định lý 1. Đặc biệt, ánh xạ từ $\mathbf{I}$ vào $E_b$ xác định bởi $s\mapsto \sigma '(1, s)$ là một nâng liên tục của đường đi hằng có ảnh là $b$; do đó nó là hằng. Điều này chứng minh rằng ánh xạ $\sigma '$ là một đồng luân ngặt nối $c'_0$ với $c'_1$.

#### Hệ quả 1 {#ta-iii-s4-prop-4-cor-1 .statement tag=01ZD}

Cho B là một không gian tôpô và E là một phủ của B; ký hiệu $p$ là phép chiếu của nó. Với mọi cặp $(x, y)$ các điểm của E, ánh xạ $\varpi_{x,y}(p):\varpi_{x,y}(E)\rightarrow \varpi_{p(x),p(y)}(B)$ là đơn ánh. Đặc biệt, với mọi điểm $x$ của E, đồng cấu $\pi_1(p, x):\pi_1(E, x)\rightarrow \pi_1(B, p(x))$ là đơn ánh.

#### Hệ quả 2 {#ta-iii-s4-prop-4-cor-2 .statement tag=01ZE}

Cho B là một không gian tôpô và E là một phủ của B; ký hiệu $p$ là phép chiếu của nó. Cho $x$ là một điểm của E, và đặt $b=p(x)$. Để lớp trong $\pi_1(B, b)$ của một đường cong kín $c$ trong B tại $a$ thuộc nhóm con ảnh của đồng cấu $\pi_1(p, x)$, điều kiện cần và đủ là đường đi $c'$ có điểm đầu $x$ nâng $c$ phải là một đường cong kín của E tại $x$.

Điều kiện này hiển nhiên là đủ. Ngược lại, cho $c'_1$ là một đường cong kín của E tại $x$. Đặt $c_1=p\circ c'_1$ và giả sử rằng các đường cong kín $c$ và $c_1$ đồng luân chặt. Theo Mệnh đề 4, đường đi $c'$ có cùng điểm cuối với đường đi $c'_1$. Do đó nó là một đường cong kín tại $x$.

#### Hệ quả 3 {#ta-iii-s4-prop-4-cor-3 .statement tag=01ZF}

Cho B là một không gian tôpô và $(E_1, p_1)$ và $(E_2, p_2)$ là các phủ của B. Ký hiệu $(E, p)$ là tích thớ của chúng trên B, và cho $x= (x_1, x_2)$ là một điểm của E. Ảnh của đồng cấu $\pi_1(p, x)$ là giao của các ảnh của các đồng cấu $\pi_1(p_1, x_1)$ và $\pi_1(p_2, x_2)$.

Cho $c$ là một đường cong kín trong B tại $p_1(x_1) =p_2(x_2)$ và, với $i\in  \{1,2\}$, cho $c'_i$ là đường đi có điểm đầu $x_i$ trong $E_i$ nâng $c$. Tích thớ trên B $E = E_1\times_BE_2$ là một phủ của B (I, p. 72, hệ quả 3 của Mệnh đề 2), và đường đi $c':t\mapsto$ $(c'_1(t), c'_2(t))$ là đường đi duy nhất có điểm đầu $x$ trong E nâng $c$. Để $c'$ là một đường cong kín, điều kiện cần và đủ là $c'_1$ và $c'_2$ cũng là các đường cong kín. Hệ quả 3 do đó suy ra từ Hệ quả 2.

### 3. Các phép toán của groupoid Poincaré trong các phủ

Cho B là một không gian tôpô và $p: E\rightarrow$ B là một ánh xạ étale và tách được thỏa mãn tính chất nâng đường đi (III, p. 302); đây là trường hợp nếu ánh xạ $p$ làm cho E trở thành một phủ của B (loc. cit.). Cho $b$ và $b'$ là các điểm của B và $c\in \Lambda_{b,b'}(B)$ là một đường đi trong B nối $b$ với $b'$. Với mỗi điểm $x$ của thớ $E_b$, ta ký hiệu $x\cdot c$ là số hạng của đường đi có điểm đầu $x$ trong E nâng $c$. Điểm $x\cdot c$ thuộc thớ $E_{b'}$ và chỉ phụ thuộc vào lớp $\gamma \in \varpi_{b,b'}(B)$ của đường đi $c($III, p. 302, prop. 4); do đó ta sẽ viết $x\cdot \gamma$ thay cho $x\cdot c$.

Nếu $c$ là đường đi hằng tại $b$, thì $x\cdot \gamma =x$ vì đường đi hằng có điểm đầu $x$ nâng $c$.

Cho $b''$ là một điểm khác của B và $c'\in \Lambda_{b',b''}(B)$. Với mọi điểm $x$ của $E_b$, ta có:

$$
(x\cdot c)\cdot c'=x\cdot (c*c') \tag{1}
$$

Thật vậy, gọi $\widetilde{c}$ là phép nâng của $c$ có điểm đầu $x$ và $\widetilde{c}'$ là phép nâng của $c'$ có điểm đầu $x\cdot c=\widetilde{c}(1)$. Các đường đi $\widetilde{c}$ và $\widetilde{c}'$ có thể ghép nối với nhau và $\widetilde{c}*\widetilde{c}'$ là đường đi có điểm đầu $x$ nâng $c*c'$.

Ta ký hiệu $\varphi_{b,b'}:\varpi_{b,b'}(B)\rightarrow \mathscr{F}(E_b; E_{b'})$ là ánh xạ sao cho, với $\gamma \in \varpi_{b,b'}(B)$ và $x\in E_b$, ta có

$$
\varphi_{b,b'}(\gamma )(x) =x\cdot \gamma
$$

Với mọi $\gamma \in \varpi_{b,b'}(B)$ và mọi $\gamma '\in \varpi_{b',b''}(B)$, từ quan hệ (1) suy ra

$$
\varphi_{b,b''}(\gamma \gamma ') =\varphi_{b',b''}(\gamma ')\circ \varphi_{b,b'}(\gamma ) \tag{2}
$$

Họ $\varphi = (\varphi_{b,b'})_{(b,b')\in B\times B}$ do đó xác định một luật phép toán phải của nhómoid $\varpi (B)$ trên tập hợp E đối với ánh xạ $p: E\rightarrow$ B (II, p. 167). Nó được gọi là phép toán chính tắc của nhómoid $\varpi (B)$ liên kết với ánh xạ $p: E\rightarrow B$. Ánh xạ $\varphi_{b,b}:\pi_1(B, b)\rightarrow \mathscr{F}(E_b; E_b)$ xác định một luật phép toán phải của nhóm $\pi_1(B, b)$ trên thớ $E_b$ của E. Phép toán này được gọi là phép toán chính tắc của $\pi_1(B, b)$ trên thớ $E_b$.

#### Nhận xét {#ta-iii-s4-n3-rem-1 .statement tag=01ZG}

Cho $b$ và $b'$ là hai điểm của B$,x$ một điểm của $E_b,c\in$ $\Lambda_{b,b'}(B)$ một đường đi trong B và $\widetilde{c}$ đường đi trong E khởi đầu tại $x$ nâng $c$. Với mọi $s\in \mathbf{I}$, ký hiệu $c_s$ là đường đi $t\mapsto c(st)$; đường đi trong E khởi đầu tại $x$ nâng $c_s$ là đường đi $t\mapsto \widetilde{c}(st)$ có số hạng là điểm $\widetilde{c}(s)$. Do đó ta có $\widetilde{c}(s) =x\cdot c_s$ với mọi $s\in \mathbf{I}$.

Cho $B'$ là một không gian tôpô và cho $p': E'\rightarrow B'$ là một ánh xạ étale và tách biệt thỏa mãn tính chất nâng đường đi. Cho $f: B\rightarrow B'$ và $g: E\rightarrow E'$ là các ánh xạ liên tục sao cho $p'\circ g=f\circ p$. Với $b,b'\in B,\gamma \in \varpi_{b,b'}(B)$ và $x\in E_b$, ta có:

$$
g(x\cdot \gamma ) =g(x)\cdot f_*(\gamma ) \tag{3}
$$

Thật vậy, cho $c$ là một đường đi trong B có lớp đồng luân ngặt là $\gamma$, và ký hiệu $\widetilde{c}$ là đường đi trong E khởi đầu tại $x$ nâng $c$; khi đó đường đi $g\circ \widetilde{c}$ là nâng khởi đầu tại $g(x)$ của $f\circ c$ trong $E'$.

Đặc biệt, với $B = B'$ và $f=$ Id$_B$, ta có

$$
g(x\cdot \gamma ) =g(x)\cdot \gamma \tag{4}
$$

Cho $p: E\rightarrow B$ và $p': E'\rightarrow B$ là các ánh xạ étale và tách biệt thỏa mãn tính chất nâng đường đi. Cho $b$ là một điểm của B. Nếu $f: E\rightarrow E'$ là một cấu xạ B, thì ánh xạ $f_b: E_b\rightarrow E'_b$ là một cấu xạ $\pi_1(B, b)$.

#### Định lý 1 {#ta-iii-s4-thm-1 .statement tag=01ZH}

Cho B là một không gian tôpô, cho $(E, p)$ là một phủ của B, cho $b$ là một điểm của B và cho $x$ là một điểm của thớ $E_b$.

a) Quỹ đạo của $x$ đối với phép toán chính tắc của nhóm $\pi_1(B, b)$ là giao của $E_b$ và thành phần liên cung của $x$ trong E. Đặc biệt, nếu không gian E liên cung, phép toán này là bắc cầu.

b) Nhóm ổn định (A, I, p. 51) của $x$ là nhóm con $p_*(\pi_1(E, x))$ của $\pi_1(B, b)$.

c) Với mọi $\gamma \in \pi_1(B, b)$, ta có $p_*(\pi_1(E, x)) =$ Int($\gamma$ )$(p_*(\pi_1(E, x\cdot$ $\gamma )))$.

d) Nếu không gian B liên thông và phép phủ E là Galois, nhóm con $p_*(\pi_1(E, x))$ là chuẩn tắc trong $\pi_1(B, b)$.

Mệnh đề a) là ngay lập tức. Mệnh đề b) suy ra từ Hệ quả 2 của Mệnh đề 4 (III, p. 303). Mệnh đề c) suy ra từ b) và từ Mệnh đề 2 của A, I, p. 52. Cuối cùng, giả sử B liên thông và E là một phép phủ Galois của B. Với mọi $\gamma \in \pi_1(B, b)$, tồn tại một tự đẳng cấu B $g$ của E sao cho $g(x) =x\cdot \gamma ($I, p. 102, th. 2, c)). Ta có $p=p\circ g$, do đó $p_*(\pi_1(E, x)) =p_*(\pi_1(E, x\cdot \gamma ))$. Mệnh đề d) do đó suy ra từ c).

### 4. Trường hợp các phép phủ liên kết với một phép phủ chính

Cho B là một không gian tôpô, G là một nhóm tôpô rời rạc, và E là một phép phủ chính của B với nhóm G. Ký hiệu $p$ là phép chiếu của B-không gian E. Cho $b$ là một điểm của B và $x$ là một điểm của $E_b$.

#### Mệnh đề 5 {#ta-iii-s4-prop-5 .statement tag=01ZI}

Ánh xạ $h_{(E,x)}$ từ $\pi_1(B, b)$ vào G, ánh xạ mỗi $\gamma \in$ $\pi_1(B, b)$ vào phần tử duy nhất $g$ của G sao cho $x\cdot g=x\cdot \gamma^{-1}$, là một đồng cấu nhóm, có hạt nhân là nhóm con $p_*(\pi_1(E, x))$ của $\pi_1(B, b)$. Nếu E liên thông, đồng cấu này là toàn ánh.

Với mọi $g\in G$, ta có $h_{(E,x\cdot g)}=$ Int($g^{-1}$)$\circ h_{(E,x)}$.

Cho E là một phép phủ chính của B với nhóm G, cho $x$ là một điểm của $E_b$, và ký hiệu $p$ là phép chiếu của E. Với mọi $g\in G$, ánh xạ $y\mapsto y\cdot g$ là một tự đẳng cấu B của E. Do đó, với mọi $g\in G$, mọi $y\in E_b$, và mọi $\gamma \in \pi_1(B, b)$, ta có quan hệ $(y\cdot g)\cdot \gamma = (y\cdot \gamma )\cdot g($cf. III, p. 305, quan hệ (4)). Do đó, với $\gamma , \delta \in \pi_1(B, b)$, ta có

$$
x\cdot h_{(E,x)}(\gamma \delta ) =x\cdot \delta^{-1}\gamma^{-1}
$$

$$
= (x\cdot h_{(E,x)}(\delta ))\cdot \gamma^{-1}
$$

$$
= (x\cdot \gamma^{-1})\cdot h_{(E,x)}(\delta )
$$

$$
=x\cdot h_{(E,x)}(\gamma )h_{(E,x)}(\delta )
$$

điều này chứng minh rằng $h_{(E,x)}$ là một đồng cấu nhóm.

Hạt nhân của nó là nhóm ổn định của $x$ đối với phép toán chính tắc của $\pi_1(B, b)$, do đó bằng $p_*(\pi_1(E, x))$ theo Định lý 1 của III, p. 305. Ánh xạ $g\mapsto x\cdot g$ là một song ánh từ G lên $E_b$. Ảnh của đồng cấu $h_{(E,x)}$ do đó là tập hợp các $g\in G$ sao cho $x\cdot g$ thuộc quỹ đạo của $x$ đối với phép toán này. Nếu E liên thông, $\pi_1(B, b)$ tác động bắc cầu trên $E_b($loc. cit.) và đồng cấu $h_{(E,x)}$ là toàn ánh.

Cho $g\in G$; với mọi $\gamma \in \pi_1(B, b)$, ta có

$$
x\cdot gh_{(E,x\cdot g)}(\gamma ) = (x\cdot g)\cdot \gamma^{-1}= (x\cdot \gamma^{-1})\cdot g=x\cdot h_{(E,x)}(\gamma )g
$$

do đó $h_{(E,x\cdot g)}(\gamma ) =g^{-1}h_{(E,x)}(\gamma )g$. Điều này hoàn tất chứng minh mệnh đề.

#### Ví dụ 1 {#ta-iii-s4-n4-exa-1 .statement tag=01ZJ}

Cho F là một tập hợp rời rạc được trang bị một phép toán của G, và cho $X = E\times^GF$ là phép phủ liên kết của B. Ký hiệu $\varphi : E\times F\rightarrow X$ là cấu xạ B chính tắc. Nó là một cấu xạ của các phép phủ. Với mọi $\gamma \in \pi_1(B, b)$ và mọi $f\in F$, ta có

(5)

$$
\varphi (x, f)\cdot \gamma =\varphi (x\cdot \gamma , f) =\varphi (x\cdot h_{(E,x)}(\gamma )^{-1}, f) =\varphi (x, h_{(E,x)}(\gamma^{-1})\cdot f)
$$

Nếu đồng nhất F với $X_b$ bằng ánh xạ song ánh $f\mapsto \varphi (x, f)$, thì suy ra phép toán phải $\pi_1(B, b)\rightarrow$ Aut(X$_b$)$^{\circ}$ là hợp của đồng cấu $h_{(E,x)}$, phản đồng cấu $g\mapsto g^{-1}$ của G vào chính nó và đồng cấu $G\rightarrow$ Aut(F) suy ra từ phép toán của G trên F.

#### Ví dụ 2 {#ta-iii-s4-n4-exa-2 .statement tag=01ZK}

Cho H là một nhóm tôpô rời rạc, cho $f: G\rightarrow H$ là một cấu xạ nhóm. Trang bị cho H phép toán trái của G xác định bởi $g\cdot h=f(g)h$, với $g\in G$ và $h\in H$. Cho $E'= E\times^GH$ là phủ liên kết; nó là một phủ chính của nhóm H (I, p. 107, Ví dụ 6). Ký hiệu $q: E\times H\rightarrow E\times^GH$ là ánh xạ chính tắc và đặt $x'=q(x, e)$. Ta có $h_{(E',x')}=f\circ h_{(E,x)}$.

Thật vậy, cho $c$ là một vòng tại $b$ trong B, cho $\gamma$ là lớp của nó trong $\pi_1(B, b)$ và cho $g=h_{(E,x)}$; do đó ta có $x\cdot \gamma =x\cdot g^{-1}$. Cho $\widetilde{c}$ là một đường đi có gốc $x$ trong E; khi đó $t\mapsto q(\widetilde{c}(t), e)$ là một đường đi có gốc $x'$ trong $E'$ nâng đường đi $p\circ \widetilde{c}$ trong B, do đó

$$
x'\cdot \gamma =q(x\cdot \gamma , e) =q(x\cdot g^{-1}, e) =q(x, f(g)^{-1}) =q(x, e)\cdot f(g)^{-1}
$$

điều này chứng minh rằng $h_{(E',x')}(\gamma ) =f(g)$.

## BÀI TẬP {#ta-iii-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
