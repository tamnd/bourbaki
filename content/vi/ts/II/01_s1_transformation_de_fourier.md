---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 1
section_title: Transformation de Fourier
lang: vi
source: ts-i-ii-fr
book_pages: TS II.201-TS II.243, TS II.262-TS II.304
pdf_pages: 0213-0255, 0274-0316
extraction: native
subsections:
    - "no": 1
      title: Caractères unitaires d’un groupe localement compact commutatif
      page: 201
      pdf_page: 213
    - "no": 2
      title: Définition de la transformation de Fourier
      page: 206
      pdf_page: 218
    - "no": 3
      title: Le théorème de Plancherel
      page: 210
      pdf_page: 222
    - "no": 4
      title: La formule d’inversion de Fourier
      page: 217
      pdf_page: 229
    - "no": 5
      title: Le théorème de dualité de Pontryagin
      page: 220
      pdf_page: 232
    - "no": 6
      title: Propriétés fonctorielles de la dualité
      page: 224
      pdf_page: 236
    - "no": 7
      title: La formule de Poisson
      page: 229
      pdf_page: 241
    - "no": 8
      title: Exemples de dualité
      page: 232
      pdf_page: 244
    - "no": 9
      title: Transformée de Fourier euclidienne et séries de Fourier
      page: 237
      pdf_page: 249
statements: 95
exercises: 68
content_sha256: f32d9966ebceeb0ef974291e23bd994ce0eb8fbf1391b33fec758ee023127d6d
translated_from: content/en-mt/ts/II/01_s1_transformation_de_fourier.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 4709ffeb6bc4b8d9e3cb7310b2947b2de94e621599ed95e7d680b38ec7f2f419
translation_model: gpt-5.4
translation_run: translate-vi-980b4706
glossary_version: 34
glossary_terms_sha256: 45ebd9ad1880cad967b25bc8cd77738ec67b0ecf29f0156c44b0bf836e6b42b7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. BIẾN ĐỔI FOURIER

### 1. Các đặc trưng unita của một nhóm giao hoán compact địa phương

#### Định nghĩa 1 {#ts-ii-s1-def-1 .statement tag=02HQ}

Một đồng cấu liên tục từ G vào nhóm nhân $\mathbf{U}$ của các số phức có môđun 1 được gọi là một đặc trưng unita của G.

Nói cách khác, một đặc trưng unita là một hàm liên tục $\chi$ trên G nhận giá trị phức sao cho:

$$
\chi (xy) =\chi (x)\chi (y),|\chi (x)|= 1(x, y\in G)
$$

Trong chương này, chúng tôi thường chỉ nói "đặc trưng" thay cho "đặc trưng unita".

Cho E là một không gian Hilbert chiều 1, và cho $\chi$ là một đặc trưng unita của G. Ánh xạ gán cho $x\in G$ phép vị tự tỉ số $\chi (x)$ trong E là một biểu diễn tuyến tính đẳng cự liên tục của G trong E. Ngược lại, mọi biểu diễn tuyến tính liên tục bị chặn của G trong E đều thu được bằng quá trình này, và đặc biệt là unita.

Ngay lập tức thấy rằng tích của hai đặc trưng unita, nghịch đảo của một đặc trưng unita, và hàm hằng bằng 1 đều là những đặc trưng unita. Do đó tập $\widehat{G}$ các đặc trưng unita của G là một nhóm đối với phép nhân. Nhóm này là giao hoán. Mặt khác, ánh xạ $(\chi_1, \chi_2)\mapsto \chi_1\chi^{-1}_2=\chi_1\overline{\chi}_2$ là liên tục đối với tôpô hội tụ compact, và $\widehat{G}$ được trang bị tôpô hội tụ compact là một nhóm tôpô (TG, X, p. 6, Hệ quả 2 và Nhận xét 1).

#### Định nghĩa 2 {#ts-ii-s1-def-2 .statement tag=02HR}

Nhóm tôpô $\widehat{G}$ được gọi là nhóm đối ngẫu của G.

Vì G compact địa phương, ánh xạ $(x, \chi )\mapsto \chi (x)$ là liên tục trên $G\times \widehat{G}$ (TG, X, p. 28, đl. 3).

Nhắc lại rằng $\mathscr{M}^1(G)$ ký hiệu đại số Banach có đơn vị, có đối hợp của các độ đo phức bị chặn trên G (Ví dụ 4 của I, p. 99). Với mọi độ đo phức bị chặn $\mu\in \mathscr{M}^1(G)$ và mọi $\chi \in \widehat{G}$, ta viết

$$
\chi (\mu) =\int_G\chi (x)d\mu(x) \tag{1}
$$

(xem INT, VIII, §2, No$^o6$).

#### Bổ đề 1 {#ts-ii-s1-lem-1 .statement tag=02HS}

Với mọi $\chi \in \widehat{G}$, ánh xạ $\mu\mapsto \chi (\mu)$ là một đặc trưng Hermit của đại số Banach có đối hợp $\mathscr{M}^1(G)$.

Theo INT, VIII, §3, No$^o3$, Mệnh đề 11, ánh xạ $\mu\mapsto \chi (\mu)$ là một đặc trưng của đại số Banach có đối hợp $\mathscr{M}^1(G)$. Hơn nữa, ta có:

$$
\chi (\mu^*) =\int_G\chi (x^{-1})d\mu(x) =\int_G\overline{\chi(x)}d\mu(x) =\overline{\chi(\mu)}
$$

và do đó đặc trưng này là Hermit.

Như vậy ta đã xác định một ánh xạ từ $\widehat{G}$ vào $\mathsf{X}(\mathscr{M}^1(G))$; nó sẽ được gọi là chính tắc.

Cho $\chi \in \widehat{G}$. Hạn chế của $\mu\mapsto \chi (\mu)$ lên $L^1(G)$ là khác không (xem INT, VIII, §2, No$^o7$, Mệnh đề 10). Bởi sự hạn chế lên đại số con Banach có đối hợp $L^1(G)$, do đó ta thu được một ánh xạ từ $\widehat{G}$ vào $\mathsf{X}(L^1(G))$, gọi là chính tắc. Nó gán cho $\chi \in \widehat{G}$ đặc trưng Hermit

$$
f\mapsto \chi (f) =\chi (f\cdot dx) =\int_Gf(x)\chi (x)dx(f\in L^1(G)) \tag{2}
$$

của $L^1(G)$.

#### Mệnh đề 1 {#ts-ii-s1-prop-1 .statement tag=02HT}

Ánh xạ chính tắc từ $\widehat{G}$ vào $\mathsf{X}(L^1(G))$ là một đồng phôi.

Ta ký hiệu ánh xạ chính tắc này bởi ev và, với $\chi \in \widehat{G}$, ta ký hiệu bởi ev$_{\chi}$ ảnh của đặc trưng $\chi$ dưới ev, nghĩa là đặc trưng Hermit $f\mapsto \chi (f)$ của $L^1(G)$. Xét như một ánh xạ từ $\widehat{G}$ vào đối ngẫu của $L^1(G)$, ánh xạ ev là hợp thành của đơn ánh từ $\widehat{G}$ vào $L^{\infty}(G)$, được trang bị tôpô yếu $\sigma (L^{\infty}(G),L^1(G))$, và đơn ánh từ $L^{\infty}(G)$ vào đối ngẫu của $L^1(G)$, được trang bị tôpô hội tụ đơn giản. Vì $\widehat{G}$ là một tập con bị chặn của $L^{\infty}(G)$, ánh xạ thứ nhất là liên tục theo định lý Lebesgue (INT, IV, §3, No$^o7$, Định lý 6). Ánh xạ thứ hai cũng liên tục, theo định nghĩa. Điều này chứng minh rằng ánh xạ ev là liên tục.

Nếu $\chi \in \widehat{G}$ và nếu $f\in L^1(G)$, ta có ev$_{\chi}(\varepsilon_x*f) =\chi (x$)ev$_{\chi}(f)$. Lấy $f$ sao cho ev$_{\chi}(f)\not= 0$, ta suy ra rằng ánh xạ ev là đơn ánh.

Cho $\zeta \in \mathsf{X}(L^1(G))$ và cho $f\in L^1(G)$ sao cho $\zeta (f)\not= 0$. Định nghĩa một ánh xạ $\chi : G\rightarrow \mathbf{C}$ bằng cách đặt, với $x\in G$:

$$
\chi (x) =\frac{\zeta(\varepsilon_x*f)}{\zeta(f)} \tag{3}
$$

Ta có $\chi (e) = 1$. Vì ánh xạ $x\mapsto \varepsilon_x*f=\boldsymbol{\gamma }(x)(f)$ từ G vào $L^1(G)$ là liên tục (INT, VIII, §2, n$^o5$, mệnh đề 8), ánh xạ $\chi$ là liên tục. Nó bị chặn vì, với mọi $x\in G$, ta có

$$
|\chi (x)|\leqslant \frac{\|\varepsilon_x*f\|}{|\zeta(f)|}=\frac{\|f\|}{|\zeta(f)|}
$$

(Định lý 1 của I, p. 29 và INT, VIII, loc. cit.).

Bây giờ cho $\mathfrak{B}$ là một cơ sở của bộ lọc các lân cận của $e$ gồm các lân cận compact. Với mọi $V\in \mathfrak{B}$, cho $g_V$ là một hàm liên tục dương, bằng không ngoài V và có tích phân bằng 1 (Bổ đề 1 của II, p. 200). Khi đó, với mọi hàm $h\in L^1(G)$, ta có

$\varepsilon_x*h=$ lim$_{V,\mathfrak{B}}(\varepsilon_x*h)*g_V=$ lim$_{V,\mathfrak{B}}(\varepsilon_x*g_V*h)$,

trong $L^1(G)$, giới hạn được lấy theo bộ lọc các thiết diện của $\mathfrak{B}$ (INT, VIII, §4, n$^o7$, mệnh đề 20). Đặc biệt, vì $\zeta (\varepsilon_x*g_V*f) =$ $\zeta (\varepsilon_x*g_V)\zeta (f)$, suy ra rằng

$\chi (x) =$ lim$_{V,\mathfrak{B}}\zeta (\varepsilon_x*g_V)$.

Với mọi $h\in L^1(G)$, ta thu được

$\zeta (\varepsilon_x*h) =$ lim$_{V,\mathfrak{B}}\zeta (\varepsilon_x*g_V*h) =\zeta (h)$ lim$_{V,\mathfrak{B}}\zeta (\varepsilon_x*g_V) =\chi (x)\zeta (h)$.

Do đó, với $x, y\in G$ ta có:

$$
\chi (xy) =\frac{\zeta(\varepsilon_x*\varepsilon_y*f)}{\zeta(f)}=\frac{\chi(x)\zeta(\varepsilon_y*f)}{\zeta(f)}=\chi (x)\chi (y)
$$

điều này chứng minh rằng $\chi$ là một đồng cấu từ G vào $\mathbf{C}^*$. Vì $\chi$ bị chặn và liên tục, nó là một đặc trưng unita của G. Hơn nữa, nếu $g\in L^1(G)$, ta có

$$
g*f=\int_G(\varepsilon_x*f)g(x)dx
$$

trong $L^1(G)$ (INT, VIII, §1, n$^o5$, mệnh đề 7), do đó

$$
\zeta (g)\zeta (f) =\zeta (g*f) =\int_G\zeta (\varepsilon_x*f)g(x)dx
$$

$=\zeta (f)\int_G\chi (x)g(x)dx=$ ev$_{\chi}(g)\zeta (f)$ (INT, VI, §1, n$^o1$, mệnh đề 1), điều này cho thấy rằng $\zeta =$ ev$_{\chi}$. Do đó, ev là toàn ánh, nên song ánh.

Sau hết, hãy chỉ ra rằng ánh xạ ngược ev$^{-1}$ là liên tục. Cho $\zeta \in \mathsf{X}(L^1(G))$. Cho $f\in L^1(G)$ là một hàm sao cho $\zeta (f)\not= 0$. Tập W các $\xi \in \mathsf{X}(L^1(G))$ sao cho $\xi (f)\not= 0$ là một lân cận mở của $\zeta$ trong $\mathsf{X}(L^1(G))$. Với mọi $\xi \in W$, điều trước đó cho thấy rằng ev$^{-1}(\xi )$ là đặc trưng

$$
x\mapsto \frac{\xi(\varepsilon_x*f)}{\xi(f)}
$$

Cho $\mathfrak{F}$ là một bộ lọc trên $W\subset \mathsf{X}(L^1(G))$ hội tụ đến $\zeta$. Vì tập $\mathsf{X}(L^1(G))$ bị chặn, do đó đồng liên tục, trong $L^{\infty}(G)$, cấu trúc đều của hội tụ đơn giản trùng với cấu trúc đều của hội tụ compắc (TG, X, p. 16, Định lý 1). Cho K là một tập con compắc của G. Tập hợp các $\varepsilon_x*f$ với $x\in K$ là compắc trong $L^1(G)$ (INT, VIII, §2, No.$^o5$, Mệnh đề 8). Do đó ta có

lim$_{\xi ,\mathfrak{F}}\xi (\varepsilon_x*f) =\zeta (\varepsilon_x*f)$

đều theo $x\in K$. Suy ra

lim$_{\xi ,\mathfrak{F}}$ ev$^{-1}(\xi ) =$ ev$^{-1}(\zeta )$,

do đó ev$^{-1}$ liên tục tại $\zeta$. Điều này hoàn tất chứng minh của mệnh đề.

Từ đây về sau ta sẽ đồng nhất một đặc trưng unita $\chi$ của G với đặc trưng $f\mapsto \int_Gf(x)\chi (x)dx$ của $L^1(G)$.

#### Nhận xét 1 {#ts-ii-s1-n1-rem-1 .statement tag=02HU}

*Song ánh của ánh xạ từ $\widehat{G}$ vào $\mathsf{X}(L^1(G))$ của Mệnh đề 1 là một trường hợp riêng của sự tương ứng giữa các biểu diễn liên tục của một nhóm địa phương compắc H (không nhất thiết giao hoán) và các biểu diễn liên tục của đại số $L^1(H)$.*

#### Nhận xét 2 {#ts-ii-s1-n1-rem-2 .statement tag=02HV}

Ánh xạ chính tắc từ $\widehat{G}$ vào $\mathsf{X}(\mathscr{M}^1(G))$ nói chung không toàn ánh (II, p. 308, bài tập 14).

#### Hệ quả 1 {#ts-ii-s1-prop-1-cor-1 .statement tag=02HW}

Mọi đặc trưng của $L^1(G)$ đều là Hermit. Ánh xạ chính tắc từ $\mathsf{X}$(Stell(G)) (Định nghĩa 9 của I, p. 125) vào $\mathsf{X}(L^1(G))$ là một đồng phôi.

Mệnh đề thứ nhất suy ra từ Mệnh đề 1 và Bổ đề 1 bằng cách hạn chế vào $L^1(G)$. Mệnh đề thứ hai suy ra từ mệnh đề thứ nhất và từ hệ quả của Mệnh đề 20 của I, p. 124.

#### Hệ quả 2 {#ts-ii-s1-prop-1-cor-2 .statement tag=02HX}

Nhóm tôpô $\widehat{G}$ là địa phương compắc.

Thật vậy, $\mathsf{X}(L^1(G))$ là địa phương compắc (hệ quả của Định lý 1 của I, p. 29).

Ta sẽ đồng nhất $\widehat{G}$ với $\mathsf{X}(L^1(G))$ và $\mathsf{X}$(Stell(G)). Với $x\in G$ và $\chi \in \widehat{G}$, ta sẽ ký hiệu bởi $\langle \chi , x\rangle$ số phức $\chi (x)$, thuộc $\mathbf{U}$.

Ta nói rằng $x$ và $\chi$ trực giao nếu $\langle \chi , x\rangle = 1$. Cho A là một tập con của G (resp. của $\widehat{G}$); tập hợp các phần tử của $\widehat{G}$ (resp. của G) trực giao với A là một nhóm con đóng của $\widehat{G}$ (resp. của G), được gọi là trực giao của A và được ký hiệu bởi $A^{\bot}$. Trực giao của G thu về $e$.

Với $x\in G$, ký hiệu $\eta (x)$ là ánh xạ từ $\widehat{G}$ vào $\mathbf{U}$ được xác định bởi $\chi \mapsto$ $\langle \chi , x\rangle$. Theo định nghĩa của phép nhân trong $\widehat{G}$, ánh xạ $\eta (x)$ là một đồng cấu nhóm. Nó liên tục vì ánh xạ $(x, \chi )\mapsto  \langle \chi , x\rangle$ từ $G\times \widehat{G}$ vào $\mathbf{U}$ là liên tục (TG, X, p. 28, th. 3). Như vậy ta đã xác định được một ánh xạ $\eta$, gọi là chính tắc, từ G vào nhóm đối ngẫu kép $\widehat{\widehat{G}}$; đó là một đồng cấu nhóm. Hơn nữa, ánh xạ $\eta$ là liên tục (TG, X, p. 28, th. 3). Ta sẽ chứng minh sau (II, p. 220, th. 2) rằng $\eta$ là một đẳng cấu nhóm từ G lên $\widehat{\widehat{G}}$.

Cho G và H là các nhóm giao hoán địa phương compact, và cho $\varphi : G\rightarrow H$ là một cấu xạ của các nhóm tôpô. Với mọi $\chi \in \widehat{H}$, ánh xạ $\chi \circ \varphi$ là một đặc trưng của G, được ký hiệu bởi $\widehat{\varphi}(\chi )$. Định nghĩa này được biểu diễn bởi công thức

$$
\langle \chi , \varphi (x)\rangle =\langle \widehat{\varphi}(\chi ), x\rangle \tag{4}
$$

với mọi $\chi \in \widehat{H}$ và mọi $x\in G$. Suy ra rằng $\widehat{\varphi}$ là một cấu xạ từ nhóm tôpô $\widehat{H}$ vào nhóm tôpô $\widehat{G}$; người ta nói rằng $\widehat{\varphi}$ là đối ngẫu của cấu xạ $\varphi$.

Cho K là một nhóm giao hoán địa phương compact và cho $\psi : H\rightarrow K$ là một cấu xạ của các nhóm tôpô. Định nghĩa cho thấy rằng $\widehat{\psi}\circ \varphi =\widehat{\varphi}\circ \widehat{\psi}$. Nếu $\varphi$ là ánh xạ đồng nhất của G, thì $\widehat{\varphi}$ là ánh xạ đồng nhất của $\widehat{G}$. Đặc biệt, nếu $\varphi$ là một đẳng cấu nhóm, thì $\widehat{\varphi}$ cũng vậy, và $\widehat{\varphi}^{-1}$ là đối ngẫu của $\varphi^{-1}$.

#### Bổ đề 2 {#ts-ii-s1-lem-2 .statement tag=02HY}

Cho G và H là các nhóm giao hoán địa phương compact và cho $f: H\rightarrow G$ là một cấu xạ của các nhóm tôpô. Hạt nhân của $\widehat{f}$ là trực giao của ảnh của $f$.

Theo định nghĩa, ta có $\chi \in$ Ker($\widehat{f}$) khi và chỉ khi hạn chế của $\chi$ trên ảnh của $f$ là tầm thường.

#### Mệnh đề 2 {#ts-ii-s1-prop-2 .statement tag=02HZ}

Cho $n\geqslant 0$ là một số nguyên và cho $G_1, . . . ,G_n$ là các nhóm giao hoán địa phương compact. Cho G là nhóm tích của các nhóm $G_j$ với $1\leqslant j\leqslant n$. Với $1\leqslant j\leqslant n$, cho $\lambda_j$ là đơn ánh từ $G_j$ vào G gán cho $x\in G_j$ phần tử $(x_k)$ sao cho $x_k=e$ nếu $k\not=j$ và $x_j=x$. Ánh xạ

$$
(\widehat{\lambda}_j)_{1\leqslant j\leqslant n}:\widehat{G}\rightarrow \prod_{1\leqslant j\leqslant n}\widehat{G}_j
$$

là một đẳng cấu nhóm.

Cho $m$ là ánh xạ tích của $\widehat{G}^n$ vào $\widehat{G}$, và với mọi $j$ sao cho $1\leqslant j\leqslant n$, cho $\pi_j$ là phép chiếu của G lên $G_j$. Cho $\mu$ là cấu xạ của các nhóm tôpô $m\circ (\widehat{\pi}_j)_j$ từ $\prod\widehat{G}_j$ vào $\widehat{G}$, sao cho

$$
\langle \mu((\chi_j)),(x_j)\rangle =\prod_{j=1}^n\langle \chi_j, x_j\rangle
$$

Ánh xạ $\mu$ là liên tục, và người ta kiểm tra rằng $\mu$ và $(\widehat{\lambda}_j)$ là các song ánh nghịch đảo của nhau. Mệnh đề được suy ra.

#### Nhận xét {#ts-ii-s1-n1-rem-3 .statement tag=02I0}

Việc tính nhóm đối ngẫu của một tích vô hạn các nhóm compact giao hoán là đối tượng của Hệ quả 4 của II, p. 234 dưới đây. Trường hợp một nhóm giao hoán địa phương compact là một tích tùy ý của các nhóm địa phương compact được suy ra từ hai mệnh đề này, vì trong một tích như thế, mọi thừa số trừ một số hữu hạn đều là compact (TG, I, p. 66, prop. 14, b)).

### 2. Định nghĩa của biến đổi Fourier

#### Định nghĩa 3 {#ts-ii-s1-def-3 .statement tag=02I1}

Cho $\mu\in \mathscr{M}^1(G)$ là một độ đo phức bị chặn trên G. Biến đổi Fourier của $\mu$ được gọi là hàm $\mathscr{F}_G(\mu)$ trên $\widehat{G}$ được định nghĩa bởi

$$
\mathscr{F}_G(\mu)(\widehat{x}) =\int_G\overline{\langle\widehat{x}, x\rangle}d\mu(x) \tag{5}
$$

Biến đổi đối Fourier của $\mu$ được gọi là hàm $\overline{\mathscr{F}}_G(\mu)$ trên $\widehat{G}$ được định nghĩa bởi

$$
\overline{\mathscr{F}}_G(\mu)(\widehat{x}) =\int_G\langle \widehat{x}, x\rangle d\mu(x) \tag{6}
$$

Khi không có sự mơ hồ nào về nhóm G được xét, người ta cũng sẽ viết $\mathscr{F}(\mu)$ và $\overline{\mathscr{F}}(\mu)$. Người ta cũng đôi khi ký hiệu $\widehat{\mu}=\mathscr{F}_G(\mu)$.

#### Mệnh đề 3 {#ts-ii-s1-prop-3 .statement tag=02I2}

Với mọi độ đo $\mu\in \mathscr{M}^1(G)$, các hàm $\mathscr{F}_G(\mu)$ và $\overline{\mathscr{F}}_G(\mu)$ đều liên tục và bị chặn. Các ánh xạ $\mathscr{F}_G:\mu\mapsto$ $\mathscr{F}_G(\mu)$ và $\overline{\mathscr{F}}_G:\mu\mapsto \overline{\mathscr{F}}_G(\mu)$ là các cấu xạ liên tục của đại số có phép đối hợp $\mathscr{M}^1(G)$ vào đại số có phép đối hợp của các hàm liên tục bị chặn trên $\widehat{G}$ (Ví dụ 1 của I, p. 99).

Cho $\mu\in \mathscr{M}^1(G)$. Với mọi $\chi \in \widehat{G}$, ta có

$$
|\mathscr{F}(\mu)(\chi )|=|\int_G\overline{\langle\chi , x\rangle}d\mu(x)|\leqslant \|\mu\|_1 \tag{7}
$$

do đó biến đổi Fourier của $\mu$ là bị chặn. Tương tự, người ta kiểm tra rằng $\overline{\mathscr{F}}(\mu)$ là bị chặn.

Nếu $\chi$ tiến tới $\chi_0$ trong $\widehat{G}$, thì hàm $\chi$ trên G tiến tới $\chi_0$ đều trên mọi compact đồng thời vẫn bị chặn bởi hàm hằng 1 thuộc $L^1(G, \mu)$. Theo định lý Lebesgue (INT, IV, §3, n$^o7$, th. 6), suy ra $\mathscr{F}(\mu)(\chi )$ tiến tới $\mathscr{F}(\mu)(\chi_0)$. Do đó $\mathscr{F}(\mu)$ là liên tục. Điều tương tự cũng đúng với $\overline{\mathscr{F}}(\mu)$.

Với mọi $\chi \in \widehat{G}$, ánh xạ $\mu\mapsto \chi (\mu) =\int\langle \chi , x\rangle d\mu(x)$ là một đặc trưng Hermit của $\mathscr{M}^1(G)$ (Bổ đề 1 của II, p. 202). Điều này suy ra rằng $\mathscr{F}$ và $\overline{\mathscr{F}}$ là các cấu xạ của các đại số có phép đối hợp từ $\mathscr{M}^1(G)$ vào đại số có phép đối hợp của các hàm liên tục bị chặn trên $\widehat{G}$. Bất đẳng thức (7) chứng minh rằng các cấu xạ này là liên tục.

Biến đổi Fourier của G (tương ứng, đối biến đổi Fourier của G) là ánh xạ $\mu\mapsto \mathscr{F}_G(\mu)$ (tương ứng, ánh xạ $\mu\mapsto$ $\overline{\mathscr{F}}_G(\mu)$) từ $\mathscr{M}^1(G)$ vào $\mathscr{C}_b(\widehat{G})$.

Hãy chú ý một số công thức hữu ích đối với $\mu\in \mathscr{M}^1(G),x\in G$ và $\chi \in \widehat{G}:$

$$
\overline{\mathscr{F}}(\mu)(\chi ) =\mathscr{F}(\mu)(\chi^{-1}) =\overline{\mathscr{F}(\overline{\mu})(\chi)} \tag{8}
$$

$$
\|\mathscr{F}(\mu)\|_{\infty}=\|\overline{\mathscr{F}}(\mu)\|_{\infty}\leqslant \|\mu\|_1 \tag{9}
$$

$$
\mathscr{F}(\varepsilon_x)(\chi ) =\overline{\langle\chi , x\rangle}
$$

(10)

$$
\overline{\mathscr{F}}(\varepsilon_x)(\chi ) =\langle \chi , x\rangle
$$

(đặc biệt $\mathscr{F}(\varepsilon_e) =\overline{\mathscr{F}}(\varepsilon_e) = 1$),

$$
\mathscr{F}(\varepsilon_x*\mu)(\chi ) =\overline{\langle\chi , x\rangle}\mathscr{F}(\mu)(\chi )
$$

(11)

$$
\overline{\mathscr{F}}(\varepsilon_x*\mu)(\chi ) =\langle \chi , x\rangle \overline{\mathscr{F}}(\mu)(\chi )
$$

$$
\mathscr{F}(\chi \cdot \mu) =\varepsilon_{\chi}*\mathscr{F}(\mu)
$$

(12)

$$
\overline{\mathscr{F}}(\chi \cdot \mu) =\varepsilon_{\chi^{-1}}*\overline{\mathscr{F}}(\mu)
$$

Các công thức (8), (9), (10) và (11) suy ra từ các định nghĩa. Hãy chứng minh công thức thứ nhất trong (12), công thức thứ hai là tương tự. Với mọi $\xi$ trong $\widehat{G}$ ta có các đẳng thức

$$
\mathscr{F}(\chi \cdot \mu)(\xi ) =\int_G\langle \xi , x\rangle \langle \chi , x\rangle d\mu(x) =\int_G\overline{\langle\xi \chi^{-1}, x\rangle}d\mu(x)
$$

$$
=\mathscr{F}(\mu)(\xi \chi^{-1}) = (\varepsilon_{\chi}*\mathscr{F}(\mu))(\xi )
$$

Hơn nữa, hãy chú ý rằng với mọi $\chi \in \widehat{G}$ và mọi độ đo $\mu$ và $\nu$ trong $\mathscr{M}^1(G)$, ta có

$$
(\varepsilon_{\chi}*\mathscr{F}(\mu))(\varepsilon_{\chi}*\mathscr{F}(\nu )) =\varepsilon_{\chi}*(\mathscr{F}(\mu)\mathscr{F}(\nu )) \tag{13}
$$

vì hai vế của đẳng thức này là các hàm trên $\widehat{G}$ mà giá trị tại $\xi \in \widehat{G}$ là

$$
\mathscr{F}(\mu)(\xi \chi^{-1})\mathscr{F}(\nu )(\xi \chi^{-1})
$$

Cho H là một nhóm giao hoán compact địa phương và $\varphi : G\rightarrow H$ là một cấu xạ liên tục. Cho $\mu\in \mathscr{M}^1(G)$. Độ đo ảnh $\varphi (\mu)$ được định nghĩa (INT, V, §6, n$^o1$, nhận xét 1), và ta được $\mathscr{F}_H(\varphi (\mu)) =\mathscr{F}_G(\mu)\circ$ $\widehat{\varphi}($xem INT, V, §6, n$^o4$, mệnh đề 7).

Bằng cách hạn chế lên đại số con $L^1(G)$ của $\mathscr{M}^1(G)$, ta thu được định nghĩa của biến đổi Fourier và của đối biến đổi Fourier trên $L^1(G)$. Do đó, với $f\in L^1(G)$ và $\chi \in \widehat{G}:$

$$
(14)\mathscr{F}_G(f)(\chi ) =\int_G\overline{\langle\chi , x\rangle}f(x)dx,\overline{\mathscr{F}}_G(f)(\chi ) =\int_G\langle \chi , x\rangle f(x)dx
$$

Đặc biệt, $\mathscr{F}_G(f) =\overline{\overline{\mathscr{F}}_G(\overline{f})}$. Ta cũng có

$$
\overline{\mathscr{F}}(f)(\chi ) =\chi (f) \tag{15}
$$

với mọi $f\in L^1(G)$ và mọi $\chi \in \widehat{G}$.

Cho $\sigma$ là một tự đẳng cấu của G và Δ là môđun của $\sigma$ (INT, VII, §1, n$^o4$, định nghĩa 4). Với $f\in L^1(G)$, ta có

$$
\mathscr{F}(f\circ \sigma ) = \Delta^{-1}\mathscr{F}(f)\circ \widehat{\sigma}^{-1} \tag{16}
$$

(xem chỗ đã dẫn, công thức (31)).

Nếu đồng nhất $\widehat{G}$ với $\mathsf{X}(L^1(G))$ (mệnh đề 1 của II, p. 202), thì đối biến đổi Fourier không là gì khác ngoài biến đổi Gelfand của đại số Banach $L^1(G)$ (I, p. 7, định nghĩa 5).

#### Mệnh đề 4 {#ts-ii-s1-prop-4 .statement tag=02I3}

Biến đổi Fourier và đối biến đổi Fourier là các cấu xạ đơn ánh của các đại số có đối hợp của $L^1(G)$ vào đại số $\mathscr{C}_0(\widehat{G})$ gồm các hàm liên tục triệt tiêu tại vô cực trên $\widehat{G}$.

Đối biến đổi Fourier là một cấu xạ của các đại số có đối hợp của $L^1(G)$ vào đại số các hàm liên tục bị chặn trên $\widehat{G}$ (mệnh đề 3). Vì nó đồng nhất với biến đổi Gelfand, ảnh của nó được chứa trong $\mathscr{C}_0(\widehat{G})$ (I, p. 37, mệnh đề 5), và hạt nhân của nó là căn của $L^1(G)$ (mệnh đề 8 của I, p. 38), căn này bằng không (hệ quả của mệnh đề 22 của I, p. 126).

Ta sẽ thấy về sau (hệ quả của mệnh đề 13 của II, p. 221) rằng đối biến đổi Fourier trên $\mathscr{M}^1(G)$ cũng là đơn ánh.

#### Nhận xét {#ts-ii-s1-n2-rem-1 .statement tag=02I4}

Biến đổi Fourier trên không gian $L^1(G)$ phụ thuộc vào lựa chọn độ đo Haar $dx$, khác với biến đổi Fourier trên $\mathscr{M}^1(G)$. Nếu thay $dx$ bằng độ đo $a\cdot dx$ (với $a >0$), thì với mọi hàm khả tích $f$ trên G, biến đổi Fourier của $f$ là $a\widehat{f}$, trong đó $\widehat{f}$ là biến đổi Fourier được xác định đối với độ đo $dx$.

Xét đại số sao Stell(G) của nhóm G (định nghĩa 9 của I, p. 125), và đồng nhất $L^1(G)$ với một đại số con trù mật của Stell(G) (mệnh đề 22 của I, p. 126).

#### Mệnh đề 5 {#ts-ii-s1-prop-5 .statement tag=02I5}

Do tính liên tục, biến đổi Fourier và đối biến đổi Fourier mở rộng duy nhất thành các đẳng cấu của các đại số sao từ Stell(G) lên $\mathscr{C}_0(\widehat{G})$.

Đối biến đổi Fourier mở rộng bởi tính liên tục thành một cấu xạ đại số sao từ Stell(G) vào $\mathscr{C}_0(\widehat{G})$. Nếu đồng nhất $\widehat{G}$ với $\mathsf{X}$(Stell(G)) (hệ quả 1 của II, p. 204 và mệnh đề 1 của II, p. 202), thì phép mở rộng này là biến đổi Gelfand của Stell(G). Theo định lý 1 của I, p. 108, nó là một đẳng cấu. Mệnh đề liên quan đến biến đổi Fourier suy ra từ điều này.

Ta sẽ luôn ký hiệu bởi $\overline{\mathscr{F}}$ và $\mathscr{F}$ các đẳng cấu của mệnh đề 5.

#### Hệ quả {#ts-ii-s1-n2-cor-1 .statement tag=02I6}

Ảnh của $L^1(G)$ dưới biến đổi Fourier của G là trù mật trong $\mathscr{C}_0(\widehat{G})$.

Vì $L^1(G)$ là trù mật trong Stell(G), điều này suy ra từ mệnh đề 5.

#### Mệnh đề 6 {#ts-ii-s1-prop-6 .statement tag=02I7}

Giả sử G là compắc. Độ đo Haar chuẩn hóa $dx$ thuộc $\mathscr{M}^1(G)$, và biến đổi Fourier của nó là $\varphi_e$, hàm đặc số của $\{e\}$.

Cho $\chi \in \widehat{G}$. Vì $\varepsilon_y*dx=dx$ với mọi $y\in G$, ta có

$$
\mathscr{F}(dx)(\chi ) =\overline{\langle\chi , y\rangle}\mathscr{F}(dx)(\chi )
$$

theo công thức (11). Nếu $\chi \not= 1$, tồn tại $y\in G$ sao cho $\langle \chi , y\rangle  \not= 1$, do đó $\mathscr{F}(dx)(\chi ) = 0$. Nếu $\chi = 1$, thì $\mathscr{F}(dx)(\chi ) =\int_Gdx= 1$ vì độ đo $dx$ là chuẩn hóa.

### 3. Định lý Plancherel

Ký hiệu bởi A(G) không gian con của $L^1(G)$ sinh bởi các hàm $f*g$ với $f, g\in L^1(G)\cap L^2(G)$.

#### Mệnh đề 7 {#ts-ii-s1-prop-7 .statement tag=02I8}

Không gian A(G) là một iđêan tự liên hợp của $L^1(G)$. Nó được chứa trong $L^1(G)\cap L^2(G)$, và trong ảnh của $\mathscr{C}(G)$ trong $L^1(G)$.

Cho $f\in L^1(G)$. Với mọi $g\in L^2(G)$, ta có $f*g\in L^1(G)$ (INT, VIII, §4, n$^o5$, mệnh đề 12). Do đó, không gian $L^1(G)\cap L^2(G)$ là một iđêan của $L^1(G)$, và điều tương tự cũng đúng với không gian A(G). Iđêan A(G) là tự liên hợp.

Cho $f$ và $g$ thuộc $L^2(G)$. Khi đó tích chập $f*g$ là lớp của hàm liên tục cho bởi

$$
y\mapsto \int_Gf(yx^{-1})g(x)dx
$$

(INT, VIII, §4, n$^o5$, mệnh đề 15). Mệnh đề thứ hai suy ra từ đó.

Vì $\chi (f*g) = (\chi f)*(\chi g)$ với $\chi \in \widehat{G},f\in L^1(G)$ và $g\in L^1(G)$ (INT, VIII, §3, No.$^o1$, prop. 6), nên $\chi h\in A(G)$ với mọi $h\in A(G)$ và $\chi \in \widehat{G}$. Vì $\varepsilon_x*f=\boldsymbol{\gamma }(x)f$ và biểu diễn tuyến tính $\boldsymbol{\gamma }$ là đẳng cự trên $L^p(G)$ với mọi $p$ (INT, VIII, §2, No.$^o5$, prop. 8), nên $\varepsilon_x*f\in A(G)$ với mọi $x\in G$ và $f\in A(G)$.

Ta ký hiệu bởi $\widehat{A}(G)$ ảnh của A(G) dưới phép biến đổi Fourier. Đó là một không gian con của $\mathscr{C}_0(\widehat{G})$.

#### Mệnh đề 8 {#ts-ii-s1-prop-8 .statement tag=02I9}

Tồn tại một cơ sở lọc $\mathfrak{B}$ trên $A(G)\cap \mathscr{K}_+(G)$ sao cho các điều kiện sau được thỏa mãn:

(i) Với mọi phần tử $\varphi$ của một tập hợp thuộc $\mathfrak{B}$, ta có $\|\varphi \|_1= 1$ và $\|\mathscr{F}(\varphi )\|_{\infty}\leqslant 1$ ;

(ii) Ta có

lim$_{\varphi ,\mathfrak{B}}\varphi \cdot dx=\varepsilon_e$

trong không gian $\mathscr{C}'(G)$ các độ đo có giá compắc trên G được trang bị tôpô hội tụ đều trên các phần compắc của $\mathscr{C}(G)$ ;

(iii) Ta có

lim$_{\varphi ,\mathfrak{B}}\mathscr{F}(\varphi ) = 1$

đối với tôpô hội tụ compắc trên $\widehat{G}$;

(iv) Với $p= 1$ hoặc $p= 2$, và với mọi $f\in L^p(G)$, ta có $\varphi *f\in$ A(G) với mọi $\varphi$ thuộc một tập hợp của $\mathfrak{B}$ và

lim$_{\varphi ,\mathfrak{B}}\varphi *f=f$

trong $L^p(G)$.

Cho $K_0$ là một lân cận compắc cố định của $e$ trong G. Cho $\mathfrak{B}_0$ là một cơ sở của bộ lọc các lân cận của $e$ trong G gồm các lân cận compắc đối xứng được chứa trong $K_0$ (xem TG, III, p. 4). Với K $\in \mathfrak{B}_0$, gọi $X'_K$ là tập hợp các hàm $\psi \in \mathscr{K}_+(G)$ sao cho Supp$(\psi )\subset K$ và $\int\psi (x)dx= 1$ ; nó khác rỗng (bổ đề 1 của II, p. 200). Gọi $X_K$ là tập hợp các hàm $\psi *\psi$ với $\psi \in X'_K$. Nó khác rỗng và được chứa trong $A(G)\cap \mathscr{K}_+(G)$. Tập hợp $\mathfrak{B}$ mà các phần tử là các tập hợp $X_K$ khi K thay đổi trong $\mathfrak{B}_0$ là một cơ sở lọc trên $A(G)\cap \mathscr{K}_+(G)$. Ta sẽ chứng minh rằng $\mathfrak{B}$ thỏa mãn các tính chất đã yêu cầu.

Nếu $X\in \mathfrak{B}$ và $\varphi \in X$, ta có $\|\varphi \|_1=\int_G\varphi (x)dx= 1$, do đó $\|\mathscr{F}(\varphi )\|_{\infty}\leqslant 1$, điều này thiết lập tính chất (i).

Tính chất (ii) suy ra từ INT, VIII, § 2, No.$^o7$, Hệ quả 1 của Bổ đề 4. Một tập con compact của $\widehat{G}$ là một tập con compact của $\mathscr{C}(G)$, do đó (ii) kéo theo lim$_{\varphi ,\mathfrak{B}}\mathscr{F}(\varphi ) = 1$ đối với tôpô hội tụ compact trên $\widehat{G}$, tức là, (iii).

Sau cùng, cho $p= 1$ hoặc $p= 2$. Cho $f\in L^p(G)$. Ta có $\varphi *f\rightarrow f$ trong $L^p(G)$ đối với bộ lọc $\mathfrak{B}$ (INT, VIII, §4, n$^o7$, mệnh đề 20). Hơn nữa, với mọi K trong $\mathfrak{B}_0$ và $\varphi \in X_K$, tồn tại $\psi \in X'_K$ sao cho $\varphi =\psi *\psi$, do đó $\varphi *f=\psi *(\psi *f)$. Ta có $\psi \in L^1(G)\cap L^2(G)$ và $\psi *f\in L^1(G)\cap L^2(G)$, vì thế $\varphi *f\in A(G)$.

#### Hệ quả 1 {#ts-ii-s1-prop-8-cor-1 .statement tag=02IA}

Không gian A(G) là trù mật trong $L^1(G)$ và trong $L^2(G)$. Nó cũng trù mật trong Stell(G), và ảnh $\widehat{A}(G)$ của nó dưới phép biến đổi Fourier là trù mật trong $\mathscr{C}_0(\widehat{G})$.

Mệnh đề (iv) của mệnh đề cho khẳng định thứ nhất. Vì $L^1(G)$ trù mật trong Stell(G), khẳng định thứ hai suy ra từ đó, và khi ấy khẳng định cuối cùng suy ra từ Mệnh đề 5 của II, p. 209.

#### Hệ quả 2 {#ts-ii-s1-prop-8-cor-2 .statement tag=02IB}

Với $f\in A(G)$, đặt $\Omega_f$ là tập hợp các $\chi \in \widehat{G}$ sao cho $\mathscr{F}(f)(\chi )\not= 0$. Các tập $\Omega_f$ tạo thành một phủ mở của $\widehat{G}$.

Điều này suy ra từ hệ quả trên vì, với mọi $\chi \in \widehat{G}$, ánh xạ $f\mapsto \mathscr{F}(f)(\chi )$ là một đặc trưng khác không của $L^1(G)$.

Nhớ lại rằng biểu diễn chính quy trái $\boldsymbol{\gamma }$ của Stell(G) trên $L^2(G)$ (x. I, p. 125, n$^o13$) được ký hiệu bởi $\boldsymbol{\gamma }(\varphi )f$ = $\varphi *f$ với $\varphi \in$ Stell(G) và $f\in L^2(G)$.

#### Bổ đề 3 {#ts-ii-s1-lem-3 .statement tag=02IC}

Với mọi $f\in A(G)$, tồn tại một độ đo bị chặn duy nhất $\mu_f$ trên $\widehat{G}$ sao cho

$$
(\varphi *f)(e) =\int_{\widehat{G}}\mathscr{F}(\varphi )d\mu_f \tag{17}
$$

với mọi $\varphi \in$ Stell(G).

Hơn nữa, với mọi $f$ và $g$ trong A(G), ta có đẳng thức

$$
\mathscr{F}(f)\cdot \mu_g=\mathscr{F}(g)\cdot \mu_f \tag{18}
$$

giữa độ đo có mật độ $\mathscr{F}(f)$ đối với $\mu_g$ và độ đo có mật độ $\mathscr{F}(g)$ đối với $\mu_f$.

Cho $f,g$ là các phần tử của $L^1(G)\cap L^2(G)$. Với mọi $\varphi \in$ Stell(G), ta có $\varphi *f\in L^2(G)$ và $\|\varphi *f\|_2\leqslant \|\varphi \|_*\|f\|_2($I, p. 126, công thức (8)). Hơn nữa, ta có $\varphi *(f*g) = (\varphi *f)*g($loc. cit., công thức (9)). Hàm sau này thuộc bao đóng $\mathscr{C}_0(G)$ của $\mathscr{K}(G)$ trong $\mathscr{C}(G)$ (INT, VIII, §4, n$^o5$, mệnh đề 15). Hơn nữa, ta có

$$
\|\varphi *(f*g)\|_{\infty}\leqslant \|\varphi *f\|_2\|g\|_2\leqslant \|\varphi \|_*\|f\|_2\|g\|_2
$$

Vì các hàm $f*g$ với $f$ và $g$ trong $L^1(G)\cap L^2(G)$ sinh ra A(G), suy ra rằng $\varphi *f\in \mathscr{C}_0(G)$ với mọi $f\in A(G)$ và $\varphi \in$ Stell(G), và ánh xạ $\varphi \mapsto (\varphi *f)(e)$ là một dạng tuyến tính liên tục trên Stell(G). Vì $\mathscr{F}$ là một đẳng cấu từ Stell(G) lên $\mathscr{C}_0(\widehat{G})$ (mệnh đề 5 của II, p. 209), mệnh đề thứ nhất được suy ra.

Bây giờ cho $f$ và $g$ thuộc A(G). Với $\varphi \in L^1(G)$, ta có

$$
(\mathscr{F}(f)\cdot \mu_g)(\mathscr{F}(\varphi )) =\int_{\widehat{G}}\mathscr{F}(\varphi )\mathscr{F}(f)d\mu_g=\int_{\widehat{G}}\mathscr{F}(\varphi *f)d\mu_g
$$

$$
= ((\varphi *f)*g)(e) \tag{19}
$$

Vì $(\varphi *f)*g= (\varphi *g)*f$ và vì ảnh của $L^1(G)$ dưới phép biến đổi Fourier là trù mật trong $\mathscr{C}_0(\widehat{G})$ (hệ quả của II, p. 210), từ công thức (19) suy ra rằng công thức (18) được thỏa mãn với mọi $f$ và $g$ trong A(G).

#### Bổ đề 4 {#ts-ii-s1-lem-4 .statement tag=02ID}

Tồn tại một độ đo $\nu$ duy nhất trên $\widehat{G}$ sao cho

$$
\mu_f=\mathscr{F}(f)\cdot \nu
$$

với mọi $f\in A(G)$. Với $f\in A(G)$, ta có $\mathscr{F}(f)\in L^1(\widehat{G}, \nu )\cap L^2(\widehat{G}, \nu )$.

Cho $f\in A(G)$. Ký hiệu bởi $\Omega_f$ tập mở trong $\widehat{G}$ gồm các $\chi \in \widehat{G}$ sao cho $\mathscr{F}(f)(\chi )\not= 0$. Gọi $\varphi$ là hàm đặc số của $\widehat{G}-\Omega_f$. Khi đó với mọi $g\in A(G)$, ta có

$$
\int_{\widehat{G}}\mathscr{F}(g)d(\varphi \cdot \mu_f) =\int_{\widehat{G}}\varphi \mathscr{F}(f)d\mu_g= 0
$$

chiếu theo công thức (18).

Theo hệ quả 1 của II, p. 212, ảnh $\widehat{A}(G)$ của A(G) dưới phép biến đổi Fourier là trù mật trong $\mathscr{C}_0(\widehat{G})$. Khi đó từ công thức trên suy ra rằng $\varphi \cdot \mu_f= 0$, do đó $\mu_f$ tập trung trên $\Omega_f$ (INT, IV, §4, n$^o7$, định nghĩa 4). Gọi $\nu_f$ là độ đo trên $\Omega_f$ có mật độ $\mathscr{F}(f)^{-1}$ đối với $\mu_f|\Omega_f$.

Các tập hợp $\Omega_f$, với $f\in A(G)$, tạo thành một phủ mở của $\widehat{G}$ (hệ quả 2). Với mọi $f$ và $g$ trong A(G), công thức (18) cho thấy rằng $\nu_f|(\Omega_f\cap \Omega_g) =\nu_g|(\Omega_f\cap \Omega_g)$. Do đó, tồn tại một độ đo duy nhất $\nu$ trên $\widehat{G}$ sao cho ta có $\nu_f=\nu |\Omega_f$ với mọi $f\in A(G)$ (INT, III, §2, No.$^o1$, mệnh đề 1).

Nếu $f\in A(G)$, các độ đo $\mu_f$ và $\mathscr{F}(f)\cdot \nu$ tập trung trên $\Omega_f$, và các hạn chế của chúng lên $\Omega_f$ đều bằng $\mathscr{F}(f)\cdot \nu_f$; do đó các độ đo này bằng nhau.

Vì $\mu_f$ là một độ đo bị chặn, biến đổi Fourier $\mathscr{F}(f)$ thuộc không gian $L^1(\widehat{G}, \nu )$. Hơn nữa, vì $\mathscr{F}(f)$ thuộc $\mathscr{C}_0(\widehat{G})$, ta cũng có $\mathscr{F}(f)\in L^2(\widehat{G}, \nu )$.

Công thức (17) khi đó có dạng sau, với $\varphi \in$ Stell(G) và $f\in A(G)$: (20) $(\varphi *f)(e) =\int_{\widehat{G}}\mathscr{F}(\varphi )\mathscr{F}(f)d\nu$.

Đặc biệt, với $f$ và $g$ trong A(G), ta có

$$
\int_{\widehat{G}}\mathscr{F}(f)\mathscr{F}(g)d\nu = (f*g)(e) =\int_Gf(x)g(x^{-1})dx \tag{21}
$$

#### Mệnh đề 9 {#ts-ii-s1-prop-9 .statement tag=02IE}

Độ đo $\nu$ được đặc trưng bởi bổ đề 4 là một độ đo Haar trên $\widehat{G}$.

Cho $\chi \in \widehat{G}$. Với $f$ và $g$ trong A(G), hãy áp dụng công thức (21) cho $\chi  f$ và $\chi  g$. Vế phải không đổi, do đó

$$
\nu (\mathscr{F}(f)\mathscr{F}(g)) =\nu (\mathscr{F}(\chi  f)\mathscr{F}(\chi  g))
$$

Từ các công thức (12) của II, p. 208 và (13) của II, p. 208, suy ra

$$
\nu (\mathscr{F}(f)\mathscr{F}(g)) =\nu (\varepsilon_{\chi}*(\mathscr{F}(f)\mathscr{F}(g)))
$$

Khi đó suy ra từ INT, VIII, §4, No.$^o3$, mệnh đề 7 rằng

$$
\nu (\mathscr{F}(f)\mathscr{F}(g)) = (\varepsilon_{\chi^{-1}}*\nu )(\mathscr{F}(f)\mathscr{F}(g))
$$

nghĩa là

$$
(\mathscr{F}(f)\cdot \nu )(\mathscr{F}(g)) = (\mathscr{F}(f)\cdot (\varepsilon_{\chi^{-1}}*\nu ))(\mathscr{F}(g))
$$

Vì không gian $\widehat{A}(G)$ là trù mật trong $\mathscr{C}_0(\widehat{G})$ (hệ quả 1), suy ra ta có đẳng thức

$$
\mathscr{F}(f)\cdot \nu =\mathscr{F}(f)\cdot (\varepsilon_{\chi^{-1}}*\nu )
$$

Do đó các độ đo $\nu$ và $\varepsilon_{\chi^{-1}}*\nu$ trùng nhau trên tập hợp mở $\Omega_f$ nơi $\mathscr{F}(f)$ khác không. Bởi hệ quả 2 và INT, III, §2, No.$^o1$, hệ quả của mệnh đề 1, do đó các độ đo này bằng nhau.

Điều này cho thấy rằng độ đo $\nu$ tỉ lệ với một độ đo Haar trên $\widehat{G}$. Cho $f\in A(G)$. Lấy $g=\widetilde{f}$ trong công thức (21). Khi đó nó có dạng

$$
\int_{\widehat{G}}|\mathscr{F}(f)|^2d\nu =\int_G|f|^2dx \tag{22}
$$

điều này cho thấy rằng độ đo $\nu$ không bằng không. Vậy độ đo $\nu$ là một độ đo Haar trên $\widehat{G}$.

#### Định nghĩa 4 {#ts-ii-s1-def-4 .statement tag=02IF}

Độ đo Haar $\nu$ trên $\widehat{G}$ của mệnh đề 9 được gọi là độ đo đối ngẫu của độ đo Haar đã cho $dx$ trên G.

Ta sẽ thường ký hiệu bởi $d\chi$ hoặc $d\widehat{x}$ độ đo Haar trên $\widehat{G}$ đối ngẫu với độ đo Haar $dx$.

#### Nhận xét {#ts-ii-s1-n3-rem-3 .statement tag=02IG}

Cho $a$ là một số thực $>0$. Nếu thay $dx$ bằng độ đo $a\cdot dx$, thì tích chập của các hàm $f$ và $g\in L^1(G)$ được thay bằng $a(f*g)$. Ta đã thấy (II, p. 209, nhận xét) rằng $\mathscr{F}(f)$ được thay bằng $a\mathscr{F}(f)$. Do đó $\mu_f$ không đổi và $\nu$ được thay bằng $a^{-1}\cdot \nu$. Đặc biệt, độ đo $dx\otimes d\widehat{x}$ trên $G\times \widehat{G}$ là độc lập với lựa chọn độ đo Haar trên G.

#### Bổ đề 5 {#ts-ii-s1-lem-5 .statement tag=02IH}

Không gian $A(\widehat{G})$ trù mật trong $L^2(\widehat{G})$.

Cho $h$ là một phần tử của $L^2(\widehat{G})$ trực giao với $\widehat{A}(G)$. Với $f$ và $g$ trong A(G), ta có $\mathscr{F}(f)\cdot \mathscr{F}(g) =\mathscr{F}(f*g)\in \widehat{A}(G)$, do đó $h\cdot \overline{\mathscr{F}(f)}$ trực giao với $\mathscr{F}(g)$. Vì vậy, với mọi $f\in A(G)$, hàm $h\cdot \mathscr{F}(f)$ trực giao với $\widehat{A}(G)$. Nhưng $h\cdot \mathscr{F}(f)\in L^1(\widehat{G})$, và $\widehat{A}(G)$ trù mật trong $\mathscr{C}_0(\widehat{G})$, bởi thế độ đo $h\mathscr{F}(f)\cdot \nu$ bằng không, nghĩa là $h\mathscr{F}(f)$ là không đáng kể địa phương đối với $\nu$ (INT, V, §5, n$^o3$, hệ quả 2 của mệnh đề 3). Đặc biệt, $h$ là không đáng kể địa phương đối với $\nu$ trên tập hợp $\Omega_f$ các đặc trưng $\chi$ sao cho $\mathscr{F}(f)(\chi )\not= 0$. Theo Hệ quả 2, suy ra $h$ là không đáng kể địa phương đối với $\nu$, nên bằng không vì $h$ thuộc $L^2(\widehat{G})$. Điều này kết thúc chứng minh.

#### Định lý 1 (Plancherel) {#ts-ii-s1-thm-1 .statement tag=02II}

Hạn chế của biến đổi Fourier lên không gian con A(G) của $L^2(G)$ mở rộng theo một cách duy nhất thành một đẳng cự Φ từ $L^2(G)$ lên $L^2(\widehat{G})$.

Hơn nữa, nếu $f\in L^1(G)\cap L^2(G)$, thì biến đổi Fourier của nó thuộc $L^2(\widehat{G})$ và trùng trong $L^2(\widehat{G})$ với $\Phi (f)$.

Theo công thức (22), hạn chế của $\mathscr{F}$ lên A(G) là một đẳng cự từ không gian con A(G) của $L^2(G)$ lên không gian con $\widehat{A}(G)$ của $L^2(\widehat{G})$. Vì A(G) trù mật trong $L^2(G)$ (hệ quả 1 của II, p. 212), biến đổi Fourier mở rộng duy nhất thành một đẳng cự Φ từ $L^2(G)$ lên một không gian con đóng của $L^2(\widehat{G})$. Nhưng vì ảnh của nó chứa $\widehat{A}(G)$, mà tập này trù mật trong $L^2(\widehat{G})$ (bổ đề 5), nên ánh xạ Φ là toàn ánh.

Bây giờ cho $f\in L^1(G)\cap L^2(G)$; hãy chứng minh rằng biến đổi Fourier của nó thuộc $L^2(\widehat{G})$. Theo mệnh đề 8, (iv) của II, p. 211, và do A(G) là một iđêan của $L^1(G)$, tồn tại một cơ sở lọc $\mathfrak{B}$ trên A(G) hội tụ đến $f$ cả trong $L^1(G)$ lẫn trong $L^2(G)$. Khi đó ta có

$\Phi (f) =$ lim$_{g,\mathfrak{B}}\Phi (g) =$ lim$_{g,\mathfrak{B}}\mathscr{F}(g)$ trong $L^2(\widehat{G})$ và $\mathscr{F}(f) =$ lim$_{g,\mathfrak{B}}\mathscr{F}(g)$ trong $\mathscr{C}_0(\widehat{G})$. Do đó tồn tại một

dãy $(g_n)$ trong A(G) sao cho $\mathscr{F}(g_n)$ hội tụ đến $\Phi (f)$ trong $L^2(\widehat{G})$ và đến $\mathscr{F}(f)$ trong $\mathscr{C}_0(\widehat{G})$. Theo INT, IV, §3, No.$^o4$, định lý 3 và hệ quả 1, ta có $\mathscr{F}(f) = \Phi (f)$, và đặc biệt $\mathscr{F}(f)\in L^2(\widehat{G})$. Điều này hoàn tất việc chứng minh định lý.

Ta vẫn ký hiệu bởi $\mathscr{F}$ đẳng cự từ $L^2(G)$ lên $L^2(\widehat{G})$ được định nghĩa trong định lý 1, và gọi nó là biến đổi Fourier trong $L^2(G)$. Tương tự, biến đổi Fourier nghịch đảo có một mở rộng đẳng cự duy nhất lên $L^2(G)$, vẫn được gọi là biến đổi Fourier nghịch đảo và được ký hiệu bởi $\overline{\mathscr{F}}$.

#### Hệ quả {#ts-ii-s1-n3-cor-1 .statement tag=02IJ}

Giả sử rằng G là compact và $dx$ là độ đo Haar đã chuẩn hóa trên G. Khi đó họ các đặc trưng unita của G là một cơ sở trực chuẩn của $L^2(G)$.

Vì G là compact, các đặc trưng của G thuộc $L^2(G)$. Với $\chi$ và $\xi$ trong $\widehat{G}$, ta có

$$
\int_G\langle \chi , x\rangle \langle \xi , x\rangle dx=\mathscr{F}_G(dx)(\chi \xi^{-1})
$$

do đó họ các đặc trưng của G là trực chuẩn (mệnh đề 6 của II, p. 210). Hơn nữa nó là toàn phần vì tích vô hướng của $\chi \in \widehat{G}$ và của $f\in L^2(G)$ bằng $\mathscr{F}_G(f)(\chi )$, và do đó $f$ trực giao với $\widehat{G}$ khi và chỉ khi $\mathscr{F}_G(f)$ bằng không trong $L^2(\widehat{G})$, khi và chỉ khi $f$ bằng không (định lý 1).

#### Nhận xét 1 {#ts-ii-s1-n3-rem-1 .statement tag=02IK}

Một số công thức liên quan đến biến đổi Fourier trên $L^1(G)$ mở rộng được sang biến đổi Fourier trên $L^2(G)$. Đặc biệt, với $f\in L^2(G)$ và $\chi \in \widehat{G}$, ta có

$$
\overline{\mathscr{F}}(f) = (\chi \mapsto \mathscr{F}(f)(\chi^{-1})) =\overline{\mathscr{F}(\overline{f})}
$$

$$
\mathscr{F}(\varepsilon_x*f) =\eta (x^{-1})\mathscr{F}(f),\overline{\mathscr{F}}(\varepsilon_x*f) =\eta (x)\mathscr{F}(f)
$$

$$
\mathscr{F}(\chi  f) =\varepsilon_{\chi}*\mathscr{F}(f),\overline{\mathscr{F}}(\chi  f) =\varepsilon_{\chi}*\mathscr{F}(f)
$$

Nếu $\sigma$ là một tự đẳng cấu của G và Δ môđun của $\sigma$ (INT, VII, §1, No.$^o4$, định nghĩa 4), thì đối với $f\in L^2(G)$, ta có

$$
\mathscr{F}(f\circ \sigma ) = \Delta^{-1}\mathscr{F}(f)\circ \widehat{\sigma}^{-1}
$$

trong $L^2(G)$.

#### Nhận xét 2 {#ts-ii-s1-n3-rem-2 .statement tag=02IL}

Các công thức

$$
\|\overline{\mathscr{F}}(f)\|^2=\|f\|^2 \tag{23}
$$

đối với $f\in L^2(G)$, hoặc cũng

$$
\int_Gf(x)\overline{g(x)}dx=\int_{\widehat{G}}\mathscr{F}(f)(\chi )\overline{\mathscr{F}(g)(\chi)}d\chi \tag{24}
$$

đối với $f$ và $g$ trong $L^2(G)$, được gọi là "các công thức Plancherel".

#### Mệnh đề 10 {#ts-ii-s1-prop-10 .statement tag=02IM}

Cho $n\geqslant 0$ là một số nguyên và cho $G_1,\cdots ,G_n$ là các nhóm giao hoán compact địa phương. Cho $\mu_j$, với $1\leqslant j\leqslant n$, là các độ đo Haar trên $G_j$. Cho G là nhóm tích của các nhóm $G_j$ với $1\leqslant j\leqslant n$. Cho $\beta$ là đẳng cấu của $\widehat{G}$ lên $\prod\widehat{G}_j$ của Mệnh đề 2 của II, p. 206. Độ đo Haar trên $\widehat{G}$ đối ngẫu với độ đo Haar tích $\mu=\mu_1\otimes  \cdots  \otimes \mu_n$ trên G được đồng nhất với tích của các độ đo Haar $\widehat{\mu}_j$.

Thật vậy, với mọi họ $(f_j)$ các phần tử khác không của $\mathscr{L}^2(G_j)$, hàm $f$ trên G được xác định bởi $(x_j)\mapsto \prod f_j(x_j)$ thuộc $\mathscr{L}^2(G)$, và thỏa mãn

$$
\int_G|f|^2d\mu=\prod_j\int_{G_j}|f_j|^2d\mu_j=\prod_j\int_{\widehat{G}_j}|\mathscr{F}_{G_j}(f)|^2d\widehat{\mu}_j
$$

theo công thức Plancherel, điều này chứng tỏ rằng độ đo Haar tích của các $\widehat{\mu}_j$ được đồng nhất với độ đo Haar đối ngẫu với $\mu$.

### 4. Công thức đảo Fourier

Nhắc lại rằng mọi phần tử $f$ của A(G) là lớp của một hàm liên tục duy nhất (Mệnh đề 7, b) của II, p. 210). Với $x\in G$, ta ký hiệu bởi $f(x)$ giá trị của hàm này tại $x$.

#### Mệnh đề 11 {#ts-ii-s1-prop-11 .statement tag=02IN}

Cho $f\in A(G)$. Khi đó $\mathscr{F}(f)\in L^1(\widehat{G})$ và, với mọi $x\in G$, ta có

$$
f(x) =\int_{\widehat{G}}\langle \widehat{x}, x\rangle \mathscr{F}(f)(\widehat{x})d\widehat{x} \tag{25}
$$

Nói cách khác, đối với $f\in A(G)$, ta có

$$
f=\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(f))\circ \eta \tag{26}
$$

trong đó $\eta$ ký hiệu ánh xạ chính tắc của G vào nhóm đối ngẫu kép $\widehat{\widehat{G}}$.

Theo Bổ đề 4 của II, p. 213 và Mệnh đề 9 của II, p. 214, ta có $\mathscr{F}(f)\in L^1(\widehat{G})$ đối với mọi hàm $f\in A(G)$. Theo công thức Plancherel (24), đối với $f$ và $g$ trong $L^2(G)$, ta có

$$
(f*\widetilde{g})(e) =\int_{\widehat{G}}\mathscr{F}(f)(\chi )\overline{\mathscr{F}(g)(\chi)}d\widehat{x}(\chi ) \tag{27}
$$

Cho $f$ và $g$ thuộc $L^1(G)\cap L^2(G)$ và cho $h=f*\widetilde{g}\in A(G)$. Vì biến đổi Fourier là một cấu xạ đối hợp, công thức (27) là mệnh đề (25) đối với hàm $h$ tại điểm $x=e$. Theo tính tuyến tính, suy ra rằng công thức (25) đúng tại điểm $x=e$ đối với mọi hàm $h\in A(G)$.

Cho $x\in G$ và $h\in A(G)$. Đặt $h_1=\varepsilon_{x^{-1}}*h$. Khi đó $h_1\in A(G)$ và $h_1(e) =h(x)$. Hơn nữa, vì $\mathscr{F}(h_1)(\chi ) =\overline{\langle\chi , x\rangle}\mathscr{F}(f)(\chi )$ với mọi $\chi \in \widehat{G}($xem công thức (11) của II, p. 208), công thức (25) đối với hàm $h_1$ tại điểm $e$ suy ra công thức (25) đối với $h$ tại điểm $x$.

#### Bổ đề 6 {#ts-ii-s1-lem-6 .statement tag=02IO}

Cho $\varphi \in L^1(\widehat{G})\cap L^2(\widehat{G})$. Khi đó $f=\overline{\mathscr{F}}_{\widehat{G}}(\varphi )\circ \eta$ thuộc $L^2(G)$ và $\mathscr{F}_G(f) =\varphi$ trong $L^2(\widehat{G})$.

Hàm $f$ liên tục và bị chặn trên G vì $\varphi \in L^1(\widehat{G})$. Với mọi hàm $g\in L^1(G)\cap L^2(G)$, ta có

$$
\int_Gg(x)f(x)dx=\int_Gg(x)(\int_{\widehat{G}}\langle \chi , x\rangle \varphi (\chi )d\widehat{x}(\chi ))dx
$$

$$
=\int_{\widehat{G}}\overline{\mathscr{F}}_G(g)(\chi )\varphi (\chi )d\widehat{x}(\chi ) \tag{28}
$$

áp dụng định lý Lebesgue-Fubini (INT, V, §8, n$^o4$, định lý 1, a)) cho hàm $(x, \chi )\mapsto g(x)\varphi (\chi )\langle \chi , x\rangle$ là hàm khả tích trên $G\times \widehat{G}$ đối với độ đo tích $dx\otimes d\widehat{x}$. Suy ra

$$
|\int_Gg(x)f(x)dx|\leqslant \|\overline{\mathscr{F}}_G(g)\|_2\|\varphi \|_2=\|g\|_2\|\varphi \|_2
$$

theo công thức Plancherel. Do đó dạng tuyến tính $g\mapsto \int_Gf g$ liên tục trên $L^1(G)\cap L^2(G)$, và vì $L^1(G)\cap L^2(G)$ trù mật trong không gian Hilbert $L^2(G)$, suy ra $f$ thuộc $L^2(G)$.

Mặt khác, áp dụng Định lý 1 của II, p. 215, ta được

$$
\int_Gg(x)f(x)dx=\int_{\widehat{G}}\overline{\mathscr{F}_G(\overline{g})(\chi)}\mathscr{F}_G(f)(\chi )d\widehat{x}(\chi )
$$

$$
=\int_{\widehat{G}}\overline{\mathscr{F}}_G(g)(\chi )\mathscr{F}_G(f)(\chi )d\widehat{x}(\chi )
$$

với mọi $g\in L^2(G)$. So sánh với (28), ta kết luận rằng $\varphi =\mathscr{F}_G(f)$ trong $L^2(\widehat{G})$, vì A(G) được chứa trong $L^1(G)\cap L^2(G)$ và $\widehat{A}(G)$ trù mật trong $L^2(\widehat{G})$ (Bổ đề 5 của II, p. 215).

Mệnh đề 12 (công thức đảo Fourier)

Cho $f\in L^2(G)$ sao cho $\mathscr{F}_G(f)\in L^1(\widehat{G})$. Khi đó ta có $f$ = $\overline{\mathscr{F}}_G(\mathscr{F}_G(f))\circ \eta$ trong $L^2(G)$. Nói cách khác, với hầu khắp mọi $x\in G$, ta có

$$
f(x) =\int_{\widehat{G}}\langle \widehat{x}, x\rangle \mathscr{F}_G(f)(\widehat{x})d\widehat{x}
$$

Hàm $\varphi =\mathscr{F}_G(f)$ thuộc $L^1(\widehat{G})\cap L^2(\widehat{G})$, và công thức cần tìm thu được bằng cách áp dụng bổ đề.

#### Hệ quả 1 {#ts-ii-s1-lem-6-cor-1 .statement tag=02IP}

Với mọi tập con đóng P của $\widehat{G}$ và mọi $\chi \in \widehat{G}$ không thuộc P, tồn tại một hàm $f\in L^1(G)$ sao cho $\mathscr{F}(f)$ bằng không trên P và khác không tại $\chi$.

Vì, theo (12), ta có $\mathscr{F}(\chi f) =\varepsilon_{\chi}*\mathscr{F}(f)$ với mọi $\chi \in \widehat{G}$, chỉ cần xét trường hợp trong đó $\chi$ là phần tử đơn vị của $\widehat{G}$.

Cho U là một lân cận đối xứng compắc của $e\in \widehat{G}$ sao cho $U^2\cap P =\emptyset$. Cho $\varphi$ là một hàm liên tục dương trên $\widehat{G}$, bằng không ngoài U và sao cho $\varphi (e) = 1$. Khi đó hàm $\varphi_1=\varphi *\varphi$ bằng không trên P và $\varphi_1(e)>0$. Do đó chỉ cần chứng minh rằng $\varphi_1$ thuộc ảnh của biến đổi Fourier trên $L^1(G)$. Bây giờ $\varphi$ và $\varphi_1$ thuộc $L^1(\widehat{G})\cap L^2(\widehat{G})$. Đặt $f=\overline{\mathscr{F}}(\varphi )\circ \eta$ và $f_1=\overline{\mathscr{F}}(\varphi_1)\circ \eta$. Bổ đề 6 kéo theo rằng $f$ và $f_1$ thuộc $L^2(G)$ và thỏa mãn $\varphi =\mathscr{F}(f)$ và $\varphi_1=\mathscr{F}(f_1)$. Hơn nữa

$$
f_1=\overline{\mathscr{F}}(\varphi *\varphi )\circ \eta = (\overline{\mathscr{F}}(\varphi )\circ \eta )^2=f^2
$$

và do đó $f_1\in L^1(G)$. Vậy $\varphi_1=\mathscr{F}(f_1)$ quả thật thuộc ảnh của $L^1(G)$ bởi biến đổi Fourier.

#### Hệ quả 2 {#ts-ii-s1-lem-6-cor-2 .statement tag=02IQ}

Đại số Banach $L^1(G)$ là chính quy (I, p. 89, Định nghĩa 1).

Theo Mệnh đề 1 của I, p. 88 và việc đồng nhất biến đổi Gelfand của $L^1(G)$ với đối biến đổi Fourier của G, điều này suy ra từ hệ quả đứng trước.

### 5. Định lý đối ngẫu Pontryagin

#### Định lý 2 (Pontryagin) {#ts-ii-s1-thm-2 .statement tag=02IR}

Ánh xạ chính tắc $\eta$ của G vào $\widehat{\widehat{G}}$ là một đẳng cấu của các nhóm tôpô. Nó biến đổi độ đo Haar $dx$ thành độ đo Haar đối ngẫu kép $d\widehat{\widehat{x}}$.

Trước hết ta hãy chứng minh rằng $\eta$ là đơn ánh và ngặt. Để làm điều đó, chỉ cần chỉ ra rằng với mọi lân cận U của $e$ trong G, tồn tại một lân cận W của $e$ trong $\widehat{\widehat{G}}$ sao cho $\overset{-1}{\eta}(W)\subset U$ (Bổ đề 2 của II, p. 200). Bây giờ cho V là một lân cận đối xứng compắc của $e$ trong G sao cho $V^2\subset U$, cho $f$ là một hàm liên tục dương trên G, có giá được chứa trong V, và sao cho $f(e)>0$. Đặt $g=\widetilde{f}*f$. Khi đó $g$ thuộc A(G), giá của nó được chứa trong U và $g(e)>0$. Hơn nữa, $\mathscr{F}_G(g)\in L^1(\widehat{G})$ theo Mệnh đề 11 của II, p. 217. Tập W gồm các $\xi$ trong $\widehat{\widehat{G}}$ sao cho

$$
|\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(g))(\xi )-\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(g))(e)|<\frac{1}{2}g(e)
$$

là một lân cận của $e$ trong $\widehat{\widehat{G}}$ vì hàm $\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(g))$ liên tục trên $\widehat{\widehat{G}}$. Cho $x\in \overset{-1}{\eta}(W)$. Theo công thức (26), ta có

$$
\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(g))(\eta (x)) =g(x)
$$

và do đó $|g(x)-g(e)|<\frac{1}{2}g(e)$. Điều này kéo theo rằng $g(x)\not= 0$ và vì thế $x\in U$, do giá của $g$ được chứa trong U. Vậy $\overset{-1}{\eta}(W)\subset U$.

Hãy chứng minh rằng ánh xạ $\eta$ là toàn ánh. Vì ánh xạ này là một đồng phôi lên ảnh của nó, nhóm $\eta (G)$ là một nhóm con địa phương compact của $\widehat{\widehat{G}}$. Do đó nó đóng trong $\widehat{\widehat{G}}$ (TG, III, p. 22, Hệ quả 2). Lập luận bằng phản chứng, giả sử tồn tại một đặc trưng $\xi \in \widehat{\widehat{G}}$ sao cho $\xi \notin \eta (G)$. Khi đó tồn tại (Hệ quả 1 của II, p. 219) một phần tử khác không $f$ của $L^1(\widehat{G})$ sao cho $\mathscr{F}_{\widehat{G}}(f)$ bằng không trên $\eta (G)$. Đặt $g\in L^1(G)$. Hàm $(x, \chi )\mapsto g(x)f(\chi )\langle \chi , x\rangle$ thuộc $L^1(G\times \widehat{G})$. Do đó, theo định lý Lebesgue-Fubini (INT, V, §8, n$^o4$, th. 1, a)), suy ra

$$
\int_{\widehat{G}}f(\chi )\mathscr{F}_G(g)(\chi )d\chi =\int_Gg(x)(\int_{\widehat{G}}f(\chi )\overline{\langle\chi , x\rangle}d\chi )dx
$$

$$
=\int_Gg(x)\mathscr{F}_{\widehat{G}}(f)(\eta (x))dx= 0
$$

Vì ảnh của biến đổi Fourier là trù mật trong $\mathscr{C}_0(\widehat{G})$ (hệ quả của Mệnh đề 5 của II, p. 209), suy ra độ đo $f\cdot d\chi$ là không. Điều này mâu thuẫn với sự kiện $f\not= 0$ trong $L^1(\widehat{G})$, và chứng minh rằng $\eta$ là toàn ánh.

Độ đo ảnh $\eta (dx)$ và độ đo $\nu$ đối ngẫu với độ đo $d\chi$ là các độ đo Haar trên $\widehat{\widehat{G}}$. Cho $f$ là một phần tử khác không của A(G) ; đặc biệt $f\in L^2(G)$. Theo Mệnh đề 12 của II, p. 219$,\mathscr{F}_G(f)\in L^1(\widehat{G})$ và ta có

$$
\int_{\widehat{\widehat{G}}}|\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(f))|^2\eta (dx) =\int_G|f|^2dx=\int_{\widehat{\widehat{G}}}|\overline{\mathscr{F}}_{\widehat{G}}(\mathscr{F}_G(f))|^2d\nu
$$

trong đó đẳng thức thứ hai suy ra từ hai lần áp dụng công thức Plancherel, do đó độ đo Haar đối ngẫu với $d\chi$ là độ đo $\eta (dx)$.

Từ đây về sau ta sẽ đồng nhất G và $\widehat{\widehat{G}}$ nhờ đẳng cấu $\eta$. Khi đó ta có:

#### Hệ quả {#ts-ii-s1-n5-cor-1 .statement tag=02IS}

Biến đổi Fourier đối của $L^2(\widehat{G})$ lên $L^2(G)$ và biến đổi Fourier của $L^2(G)$ lên $L^2(\widehat{G})$ là những đẳng cự nghịch đảo của nhau.

#### Nhận xét {#ts-ii-s1-n5-rem-1 .statement tag=02IT}

Cho $f\in L^2(G)$ và $g\in L^2(\widehat{G})$. Áp dụng công thức Plancherel (24) cho $f$ và $\overline{\mathscr{F}_{\widehat{G}}(g)}$, ta thu được công thức

$$
\int_Gf(x)\mathscr{F}_{\widehat{G}}(g)(x)dx=\int_{\widehat{G}}\mathscr{F}_G(f)(\chi )g(\chi )d\widehat{x}(\chi ) \tag{29}
$$

vì ta có $\mathscr{F}_G(\mathscr{F}_{\widehat{G}}(g)) =\mathscr{F}_G(\overline{\mathscr{F}}_{\widehat{G}}(\overline{g})) =\overline{g}$.

Biến đổi Fourier và biến đổi Fourier đối xác định trên $\mathscr{M}^1(\widehat{G})$ nhận giá trị trong không gian các hàm liên tục bị chặn trên G. Với $\beta \in \mathscr{M}^1(\widehat{G})$ và $x\in G$, ta có

$$
\mathscr{F}_{\widehat{G}}(\beta )(x) =\int_{\widehat{G}}\overline{\langle\chi , x\rangle}d\beta (\chi ),\overline{\mathscr{F}}_{\widehat{G}}(\beta )(x) =\int_{\widehat{G}}\langle \chi , x\rangle d\beta (\chi )
$$

Các biến đổi Fourier của G và $\widehat{G}$ cũng là các ánh xạ chuyển vị của nhau. Chính xác hơn:

#### Mệnh đề 13 {#ts-ii-s1-prop-13 .statement tag=02IU}

Cho $\alpha \in \mathscr{M}^1(G)$ và $\beta \in \mathscr{M}^1(\widehat{G})$. Khi đó ta có (30) $\mathscr{F}_G(\overline{\mathscr{F}}_{\widehat{G}}(\beta )\cdot \alpha ) =\beta *\mathscr{F}_G(\alpha )$

và đặc biệt

$$
\int_G\mathscr{F}_{\widehat{G}}(\beta )(x)d\alpha (x) =\int_{\widehat{G}}\mathscr{F}_G(\alpha )(\chi )d\beta (\chi ) \tag{31}
$$

Công thức (30) suy ra công thức (31) khi lấy giá trị hai vế của đẳng thức tại $\chi = 1$. Hãy chứng minh (30). Cho $\chi \in \widehat{G}$. Suy ra

$$
(\mathscr{F}_G(\overline{\mathscr{F}}_{\widehat{G}}(\beta )\cdot \alpha ))(\chi ) =\int_G\overline{\langle\chi , x\rangle}\overline{\mathscr{F}}_{\widehat{G}}(\beta )(x)d\alpha (x)
$$

$$
=\int_G\overline{\langle\chi , x\rangle}(\int_{\widehat{G}}\langle \xi , x\rangle d\beta (\xi ))d\alpha (x)
$$

Hàm $(x, \xi )\mapsto  \langle \chi , x\rangle \langle \xi , x\rangle$ là liên tục và bị chặn, do đó khả tích trên $G\times \widehat{G}$ đối với độ đo $\alpha \otimes \beta$. Theo định lý Lebesgue-Fubini (INT, V, §8, n$^o4$, th. 1, a)), ta được

$$
(\mathscr{F}_G(\overline{\mathscr{F}}_{\widehat{G}}(\beta )\cdot \alpha ))(\chi ) =\int_{\widehat{G}}(\int_G\overline{\langle\chi \xi^{-1}, x\rangle}d\alpha (x))d\beta (\xi )
$$

$$
=\int_{\widehat{G}}\mathscr{F}_G(\alpha )(\chi \xi^{-1})d\beta (\xi ) = (\beta *\mathscr{F}_G(\alpha ))(\chi )
$$

như đã mong muốn.

#### Hệ quả {#ts-ii-s1-n5-cor-2 .statement tag=02IV}

Biến đổi Fourier $\mathscr{F}_G$ là đơn ánh trên $\mathscr{M}^1(G)$.

Thật vậy, nếu $\alpha \in \mathscr{M}^1(G)$ thỏa mãn $\mathscr{F}_G(\alpha ) = 0$, ta suy ra từ (31) rằng $\alpha (\mathscr{F}_G(f)) = 0$ với mọi $f\in L^1(\widehat{G})$; vì ảnh của $L^1(\widehat{G})$ dưới biến đổ$\widehat{i}$ Fourier là trù mật trong $\mathscr{C}_0(G)$ (hệ quả của Mệnh đề 5 của II, p. 209), nên suy ra $\alpha = 0$.

Tồn tại những không gian hàm trên G và $\widehat{G}$, khác với $L^2(G)$ và $L^2(\widehat{G})$, trên đó $\mathscr{F}$ và $\overline{\mathscr{F}}$ là các đẳng cấu nghịch đảo của nhau. Định lý sau cho một ví dụ về điều đó. Ta ký hiệu bởi B(G) không gian con vectơ của $L^1(G)$ gồm các phần tử $f\in L^1(G)$ sao cho $\mathscr{F}_G(f)\in L^1(\widehat{G})$. Đây là một đại số con của $L^1(G)$. Thật vậy, cho $f$ và $g$ thuộc B(G). Khi đó $f*g\in L^1(G)$ và $\mathscr{F}_G(f*g) =\mathscr{F}_G(f)\mathscr{F}_G(g)\in L^1(\widehat{G})$, vì $\mathscr{F}_G(f)\in L^1(\widehat{G})$ và $\mathscr{F}_G(g)\in \mathscr{C}_0(\widehat{G})$.

#### Định lý 3 {#ts-ii-s1-thm-3 .statement tag=02IW}

Hạn chế của biến đổi Fourier lên B(G) cảm sinh một đẳng cấu các không gian vectơ từ B(G) lên $B(\widehat{G})$, mà nghịch đảo của nó được cảm sinh bởi hạn chế của biến đổi đồng-Fourier lên $B(\widehat{G})$.

Cho $f\in B(G)$. Đặt $g=\mathscr{F}_G(f)$. Khi đó $g\in L^1(\widehat{G})\cap \mathscr{C}_0(\widehat{G})\subset$ $L^1(\widehat{G})\cap L^2(\widehat{G})$. Đặt $f_1=\overline{\mathscr{F}}_{\widehat{G}}(g)\in L^2(G)$. Với mọi hàm liên tục có giá compact $h\in \mathscr{K}(\widehat{G})$, ta có $h\in L^1(\widehat{G})\cap L^2(\widehat{G})$ và

$$
\int_Gf_1(x)\mathscr{F}_{\widehat{G}}(h)(x)dx=\int_G\overline{\mathscr{F}}_{\widehat{G}}(g)(x)\overline{\overline{\mathscr{F}}_{\widehat{G}}(\overline{h})(x)}dx
$$

$$
=\int_{\widehat{G}}g(\chi )h(\chi )d\widehat{x}(\chi )
$$

$$
=\int_{\widehat{G}}\mathscr{F}_G(f)(\chi )h(\chi )d\widehat{x}(\chi ) =\int_Gf(x)\mathscr{F}_{\widehat{G}}(h)(x)dx
$$

bằng cách dùng định lý Plancherel và công thức (31). Vì $\mathscr{K}(\widehat{G})$ là trù mật trong $L^2(\widehat{G})$, ảnh của nó dưới biến đổi Fourier là trù mật trong $L^2(G)$. Do đó, ta có $f_1=f$ trong $L^1(G)$; điều này chứng minh rằng $g\in B(\widehat{G})$.

Công thức $f_1=f$ có nghĩa là hạn chế lên B(G) của hợp thành $\overline{\mathscr{F}}_{\widehat{G}}\circ \mathscr{F}_G$ là ánh xạ đồng nhất của B(G). Bằng cách đổi vai trò của G và $\widehat{G}$, ta thấy rằng $\mathscr{F}_G\circ \mathscr{F}_{\widehat{G}}$ là ánh xạ đồng nhất của $B(\widehat{G})$, điều này hoàn thành chứng minh định lý.

#### Hệ quả 1 {#ts-ii-s1-thm-3-cor-1 .statement tag=02IX}

Cho $f\in L^1(G)$. Khi đó $f\in B(G)$ khi và chỉ khi $f$ thuộc ảnh của biến đổi Fourier $\mathscr{F}_{\widehat{G}}$ trên $L^1(\widehat{G})$. Đặc biệt, ta có $A(G)\subset B(G)$.

Định lý 3 chứng minh rằng nếu $f\in B(G)$, thì $f=\mathscr{F}_{\widehat{G}}(\overline{\mathscr{F}}_G(f))$, trong đó $\mathscr{F}_G(f)$ thuộc $L^1(\widehat{G})$. Ngược lại, nếu $f=\mathscr{F}_{\widehat{G}}(g)$, trong đó $g\in L^1(\widehat{G})$, thì ta có $g\in B(\widehat{G})$ và do đó $f\in B(G)$ theo định lý. Khẳng định cuối cùng khi đó suy ra từ mệnh đề 11 của II, p. 217.

#### Hệ quả 2 {#ts-ii-s1-thm-3-cor-2 .statement tag=02IY}

Không gian vectơ B(G) là một đại số đối với cả phép nhân lẫn phép chập. Biến đổi Fourier hoán đổi phép chập và phép nhân trong B(G) và $B(\widehat{G})$.

Ta đã thấy rằng B(G) là một đại số con của $L^1(G)$. Mặt khác, nếu $f$ và $g$ thuộc B(G), thì $f g\in L^1(G)$ vì $f\in L^1(G)$ và $g$ thuộc ảnh của biến đổi Fourier trên $L^1(\widehat{G})$ (Hệ quả 1). Vì tồn tại $f_1$ và $g_1$ trong $L^1(\widehat{G})$ sao cho $f$ = $\mathscr{F}_{\widehat{G}}(f_1)$ và $g=\mathscr{F}_{\widehat{G}}(g_1)$ (loc. cit.), ta có $f g=\mathscr{F}_{\widehat{G}}(f_1*g_1)$, và do đó $f g\in B(G)$, lại theo hệ quả trước.

#### Mệnh đề 14 {#ts-ii-s1-prop-14 .statement tag=02IZ}

Cho $f$ và $g$ thuộc $L^2(G)$. Khi đó $\mathscr{F}_G(f g) =$ $\mathscr{F}_G(f)*\mathscr{F}_G(g)$.

Đẳng thức là đúng nếu $f$ và $g$ thuộc B(G) (Hệ quả 2), và đặc biệt nếu $f$ và $g$ thuộc A(G) vì $A(G)\subset B(G)$ (Hệ quả 1). Vì A(G) trù mật trong $L^2(G)$ (Hệ quả 1 của II, p. 212), chỉ cần chứng minh rằng hai vế của đẳng thức là các hàm liên tục của $(f, g)\in L^2(G)\times L^2(G)$ nhận giá trị trong $\mathscr{C}_0(\widehat{G})$. Bây giờ ánh xạ $(f, g)\mapsto \mathscr{F}_G(f g)$ thu được bằng cách hợp thành ánh xạ liên tục $(f, g)\mapsto f g$ từ $L^2(G)\times L^2(G)$ vào $L^1(G)$ và biến đổi Fourier $\mathscr{F}_G$ từ $L^1(G)$ vào $\mathscr{C}_0(\widehat{G})$, ánh xạ này cũng liên tục. Tương tự, ánh xạ $(f, g)\mapsto \mathscr{F}_G(f)*\mathscr{F}_G(g)$ thu được bằng cách hợp thành các ánh xạ liên tục $(f, g)\mapsto (\mathscr{F}_G(f),\mathscr{F}_G(g))$ từ $L^2(G)\times L^2(G)$ vào $L^2(\widehat{G})\times L^2(\widehat{G})$ và $(h_1, h_2)\mapsto h_1*h_2$ từ $L^2(\widehat{G})\times L^2(\widehat{G})$ vào $\mathscr{C}_0(\widehat{G})$ (INT, VIII, §4, n$^o5$, mệnh đề 15).

#### Nhận xét {#ts-ii-s1-n5-rem-2 .statement tag=02J0}

Xem n$^o9$ và các bài tập 22 của II, p. 270 và 31 của II, p. 275 để có những ví dụ khác về các không gian hàm trên đó biến đổi Fourier là một đẳng cấu, trong trường hợp các nhóm G riêng biệt.

### 6. Các tính chất hàm tử của đối ngẫu

Cho G và H là các nhóm giao hoán compact địa phương. Nhắc lại rằng nếu $\varphi : G\rightarrow H$ là một cấu xạ của các nhóm tôpô, thì cấu xạ đối ngẫu $\widehat{\varphi}:\widehat{H}\rightarrow \widehat{G}$ được định nghĩa bởi $\langle \chi , \varphi (x)\rangle =\langle \widehat{\varphi}(\chi ), x\rangle$ với mọi $\chi \in \widehat{H}$ và $x\in G$. Định nghĩa này cho thấy rằng $\widehat{\widehat{\varphi}}=\varphi$ khi đồng nhất G (resp. H) với $\widehat{\widehat{G}}$ (resp. $\widehat{\widehat{H}}$) của Định lý 2 trong II, p. 220.

Cho $\theta$ là một ánh xạ từ $G\times H$ vào $\mathbf{U}$. Với mỗi $x\in G$ (resp. mỗi $y\in H$), ký hiệu $\theta_x$ (resp. $\theta^y$) là hàm từ G vào $\mathbf{U}$ xác định bởi $y\mapsto$ $\theta (x, y)$ (resp. hàm từ H vào $\mathbf{U}$ xác định bởi $x\mapsto \theta (x, y)$). Giả sử rằng ánh xạ $\alpha :x\mapsto \theta_x$ là một đẳng cấu của nhóm tôpô G lên nhóm tôpô $\widehat{H}$. Với mọi $y\in H$ và $x\in G$, ta có

$$
\theta^y(x) =\theta (x, y) =\langle \alpha (x), y\rangle =\langle x,\widehat{\alpha}(y)\rangle
$$

nghĩa là, $\theta^y=\widehat{\alpha}(y)$. Do đó theo Định lý 2 trong II, p. 220, ánh xạ $\beta :y\mapsto \theta^y$ là một đẳng cấu của nhóm tôpô H lên nhóm tôpô $\widehat{G}$. Trong các điều kiện ấy, ta sẽ nói rằng $\theta$ đặt G và H vào đối ngẫu, hoặc rằng G và H đối ngẫu tương đối đối với $\theta$. Khi đó ta sẽ đồng nhất mỗi nhóm G và H với đối ngẫu của nhóm kia. Độ đo Haar trên H thu được bằng phép chuyển cấu trúc từ độ đo đối ngẫu của $dx$ sẽ được gọi là độ đo đối ngẫu của độ đo Haar $dx$.

#### Bổ đề 7 {#ts-ii-s1-lem-7 .statement tag=02J1}

Cho $(G_i)_{i\in I}$ và $(H_i)_{i\in I}$ là các họ hữu hạn các nhóm tôpô compact địa phương. Với $i\in I$, cho $\theta_i: G_i\times H_i\rightarrow \mathbf{U}$ là một ánh xạ đặt các nhóm $G_i$ và $H_i$ vào đối ngẫu. Ánh xạ $\theta$ xác định bởi

$$
\theta ((g_i),(h_i)) =\prod_{i\in I}\theta_i(g_i, h_i)
$$

đặt các nhóm $\prod G_i$ và $\prod H_i$ vào đối ngẫu.

Điều này suy ra từ Mệnh đề 2 trong II, p. 206 và từ định nghĩa trên.

#### Định nghĩa 5 {#ts-ii-s1-def-5 .statement tag=02J2}

Cho G, H và K là các nhóm tôpô. Cho $f: H\rightarrow G$ và $g: G\rightarrow K$ là các cấu xạ của các nhóm tôpô. Cặp $(f, g)$ được gọi là một dãy khớp của các nhóm tôpô nếu nó là một dãy khớp của các nhóm (A, II, p. 10, Nhận xét 5) và nếu $f$ và $g$ là các cấu xạ ngặt.

Một dãy khớp sẽ được biểu diễn bởi biểu đồ

$$
H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K
$$

và người ta sẽ nói rằng một biểu đồ

$$
G_1\longrightarrow^{f_1}G_2\longrightarrow^{f_2}G_3\rightarrow  \cdots  \rightarrow G_n\longrightarrow^{f_n}G_{n+1}
$$

là khớp nếu mỗi cặp $(f_i, f_{i+1})$ với $1\leqslant i\leqslant n-1$ là khớp.

Một dãy

$$
1\rightarrow H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K\rightarrow 1
$$

là khớp khi và chỉ khi $f$ là một cấu xạ đơn ánh ngặt, $g$ là một cấu xạ toàn ánh ngặt, và hạt nhân của $g$ bằng ảnh của $f$. Nếu K tách, ảnh của $f$ là một nhóm con đóng của G.

#### Ví dụ 1 {#ts-ii-s1-n6-exa-1 .statement tag=02J3}

Cho $f: H\rightarrow$ G là một cấu xạ đơn ánh ngặt mà ảnh của nó là một nhóm con phân biệt. Dãy

$$
1\rightarrow H\overset{f}{\longrightarrow}G\overset{p}{\longrightarrow}G/f(H)\rightarrow 1
$$

trong đó $p$ là phép chiếu chính tắc, là khớp. Đặc biệt, nếu H là một nhóm con phân biệt đóng của G, dãy các nhóm tôpô

$$
1\rightarrow H\overset{j}{\longrightarrow}G\overset{p}{\longrightarrow}G/H\rightarrow 1
$$

trong đó $j$ là phép nhúng và $p$ là phép chiếu chính tắc, là khớp.

#### Ví dụ 2 {#ts-ii-s1-n6-exa-2 .statement tag=02J4}

Cho $g: G\rightarrow K$ là một cấu xạ ngặt toàn ánh. Dãy

$1\rightarrow$ Ker($g$)$\overset{j}{\longrightarrow}G\overset{g}{\longrightarrow}K\rightarrow 1$,

trong đó $j$ là phép nhúng, là khớp

#### Định lý 4 {#ts-ii-s1-thm-4 .statement tag=02J5}

Một dãy

$$
H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K
$$

các nhóm tôpô giao hoán địa phương compact là khớp nếu, và chỉ nếu, dãy đối ngẫu

$$
\widehat{K}\widehat{\longrightarrow}^g\widehat{G}\widehat{\longrightarrow}^f\widehat{H}
$$

là khớp.

Chúng tôi sẽ bắt đầu bằng việc chứng minh một vài bổ đề. Ta sẽ nhận thấy rằng mỗi bổ đề đó hơn nữa còn là một hệ quả dễ dàng của mệnh đề của định lý 4.

#### Bổ đề 8 {#ts-ii-s1-lem-8 .statement tag=02J6}

Cho $g: G\rightarrow K$ là một cấu xạ của các nhóm tôpô giao hoán địa phương compact. Nếu cấu xạ $g$ là toàn ánh và ngặt, thì $\widehat{g}$ là đơn ánh và ngặt.

Vì $g$ là toàn ánh, cấu xạ $\widehat{g}$ là đơn ánh (bổ đề 2 của II, p. 205). Để chứng minh rằng $\widehat{g}$ là một cấu xạ ngặt, chỉ cần chứng minh rằng với mọi lân cận U của $e$ trong $\widehat{K}$, tồn tại một lân cận V của $e$ trong $\widehat{G}$ sao cho $\overset{-1}{\widehat{g}}(V)\subset U$ (bổ đề 2 của II, p. 200). Cho U là một lân cận như vậy của $e$ trong $\widehat{K}$. Theo định nghĩa của tôpô của $\widehat{K}$, tồn tại một tập con compact X của K và một số $\varepsilon  >0$ sao cho U chứa tập hợp các $\widehat{z}\in \widehat{K}$ mà, với mọi $z\in X$, thỏa mãn $|\langle \widehat{z}, z\rangle  -1|< \varepsilon$. Vì $g$ là ngặt và toàn ánh, theo TG, I, p. 80, mệnh đề 10, tồn tại một tập con compact $X_0$ của G sao cho $g(X_0) = X$. Gọi V là lân cận của $e$ trong $\widehat{G}$ gồm các phần tử $\chi \in \widehat{G}$ sao cho,

với mọi $x\in X_0$, ta có $|\langle \chi , x\rangle  -1|< \varepsilon$. Khi đó ta có $\overset{-1}{\widehat{g}}(V)\subset U$. Điều này chứng minh mệnh đề.

#### Bổ đề 9 {#ts-ii-s1-lem-9 .statement tag=02J7}

Cho $f: H\rightarrow G$ là một cấu xạ của các nhóm tôpô địa phương compact. Nếu cấu xạ $f$ là đơn ánh và ngặt, thì $\widehat{f}$ là toàn ánh và ngặt.

Giả sử rằng $f$ là đơn ánh và ngặt. Cấu xạ $\widehat{f}$ cảm sinh, bằng cách chuyển qua thương, một cấu xạ $q:\widehat{G}/$ Ker($\widehat{f}$)$\rightarrow \widehat{H}$. Điều phải chứng minh là đây là một đẳng cấu của các nhóm tôpô; theo đối ngẫu, để chứng minh điều này chỉ cần chứng minh rằng đối ngẫu của nó $\widehat{q}$ là một đẳng cấu.

Gọi L là nhóm đối ngẫu của $\widehat{G}/$ Ker($\widehat{f}$) và $p:\widehat{G}\rightarrow \widehat{G}/$ Ker($\widehat{f}$) là phép chiếu chính tắc. Trước hết chúng tôi sẽ chứng minh rằng $\widehat{p}$ cảm sinh, bằng cách chuyển qua các không gian con, một đẳng cấu của L lên $f(H)$.

Ta có $q\circ p=\widehat{f}$, do đó $\widehat{p}\circ \widehat{q}=f$. Vì vậy ảnh của $\widehat{p}$ chứa $f(H)$.

Vì $f$ là ngặt, ảnh của nó $f(H)$ là một nhóm con địa phương compact của G, và do đó là đóng (TG, III, p. 22, hệ quả 2). Đặt K = $G/f(H)$ và xét dãy khớp

$$
1\rightarrow H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K\rightarrow 1
$$

liên kết (Ví dụ 1). Theo đối ngẫu, cấu xạ $\widehat{f}\circ \widehat{g}$ là tầm thường và do đó ảnh của $\widehat{g}$ được chứa trong Ker($\widehat{f}$) $=$ Ker($p$). Vì thế $p\circ \widehat{g}$ là cấu xạ tầm thường và, lại theo đối ngẫu, $g\circ \widehat{p}$ cũng tầm thường. Suy ra ảnh của $\widehat{p}$ được chứa trong hạt nhân của $g$, hạt nhân này bằng $f(H)$. Kết luận rằng ảnh của $\widehat{p}$ bằng $f(H)$.

Hơn nữa, vì $p$ là một cấu xạ ngặt toàn ánh, cấu xạ đối ngẫu $\widehat{p}$ là một cấu xạ ngặt đơn ánh từ L vào G (Bổ đề 8). Suy ra $\widehat{p}$ cảm sinh một đẳng cấu nhóm tôpô của L lên $f(H)$. Vì $\widehat{p}\circ \widehat{q}=f$, và $f$ cảm sinh một đẳng cấu của H lên ảnh của nó $f(H)$, cấu xạ $\widehat{q}$ là một đẳng cấu.

#### Bổ đề 10 {#ts-ii-s1-lem-10 .statement tag=02J8}

Cho

$$
H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K
$$

là một dãy khớp các nhóm giao hoán địa phương compact. Hạt nhân của $\widehat{f}$ bằng ảnh của $\widehat{g}$.

Đồng cấu $\widehat{f}\circ \widehat{g}$ là tầm thường theo đối ngẫu, do đó ảnh của $\widehat{g}$ được chứa trong hạt nhân của $\widehat{f}$. Ngược lại, giả sử $\chi$ thuộc hạt nhân của $\widehat{f}$. Điều này có nghĩa là Im($f$) $=$ Ker($g$) được chứa trong hạt nhân của $\chi$, do đó tồn tại một đặc trưng $\eta$ của Im($g$) sao cho $\eta \circ g=\chi$. Vì phép bao hàm của Im($g$) vào K là ngặt, ánh xạ hạn chế đối ngẫu từ các đặc trưng của K tới Im($g$) là toàn ánh (Bổ đề 9). Do đó tồn tại một đặc trưng $\beta$ của K sao cho $\eta$ là hạn chế của $\beta$, và khi đó $\chi =\beta \circ g=\widehat{g}(\beta )$. Kết luận rằng hạt nhân của $\widehat{f}$ được chứa trong ảnh của $\widehat{g}$.

Bây giờ chứng minh Định lý 4. Theo đối ngẫu, chỉ cần chứng minh rằng dãy $\widehat{K}\widehat{\longrightarrow}^g\widehat{G}\widehat{\longrightarrow}^f\widehat{H}$ là khớp khi dãy $H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K$ là khớp. Mà theo các Bổ đề 8 và 9, các cấu xạ $\widehat{f}$ và $\widehat{g}$ là ngặt, và theo Bổ đề 10, hạt nhân của $\widehat{f}$ bằng ảnh của $\widehat{g}$.

#### Hệ quả 1 {#ts-ii-s1-lem-10-cor-1 .statement tag=02J9}

Cho

$$
1\rightarrow H\overset{f}{\longrightarrow}G\overset{g}{\longrightarrow}K\rightarrow 1
$$

là một dãy khớp các nhóm tôpô giao hoán địa phương compact. Cấu xạ $\widehat{g}$ cảm sinh một đẳng cấu giữa $\widehat{K}$ và $f(H)^{\bot}$, và $\widehat{f}$ cảm sinh, khi chuyển qua thương, một đẳng cấu giữa $\widehat{G}/f(H)^{\bot}$ và $\widehat{H}$.

Theo Định lý 4, dãy

$$
1\rightarrow \widehat{K}\widehat{\longrightarrow}^g\widehat{G}\widehat{\longrightarrow}^f\widehat{H}\rightarrow 1 \tag{32}
$$

là khớp. Do đó cấu xạ $\widehat{g}$ cảm sinh một đẳng cấu từ $\widehat{K}$ lên Ker($\widehat{f}$) $=f(H)^{\bot}$ (Bổ đề 2 của II, p. 205), và $\widehat{f}$ cảm sinh, bằng cách chuyển qua thương, một đẳng cấu từ $\widehat{G}/Ker(\widehat{f}) =\widehat{G}/f(H)^{\bot}$ lên $\widehat{H}($loc. cit.).

#### Hệ quả 2 {#ts-ii-s1-lem-10-cor-2 .statement tag=02JA}

Cho $f: G\rightarrow H$ là một cấu xạ của các nhóm tôpô giao hoán compact địa phương. Cấu xạ $f$ là ngặt khi và chỉ khi $\widehat{f}$ là ngặt.

Theo phân tích chính tắc (E, II, p. 44) của một cấu xạ ngặt, điều này suy ra từ các Bổ đề 8 và 9.

#### Hệ quả 3 {#ts-ii-s1-lem-10-cor-3 .statement tag=02JB}

Cho H là một nhóm con của G. Khi đó $(H^{\bot})^{\bot}= H$.

Vì $H^{\bot}$ = $\overline{H}^{\bot}$, ta có thể giả sử rằng H đóng. Cho $f: H\rightarrow G$ là đơn ánh chính tắc và $p: G\rightarrow G/H$ là phép chiếu chính tắc. Ta có $H^{\bot}=$ Ker($\widehat{f}$) (Bổ đề 10). Cho $k$ là đơn ánh chính tắc của $H^{\bot}$ vào $\widehat{G}$. Theo Định lý 4, cấu xạ $\widehat{p}$ cảm sinh một đẳng cấu $\widehat{p}_H:\widehat{G}/H\rightarrow H^{\bot}$ của các nhóm tôpô và ta có $k\circ \widehat{p}_H=\widehat{p}$. Do đó (Hệ quả 1), ta được

$(H^{\bot})^{\bot}=$ Ker($\widehat{k}$) $=$ Ker( $\widehat{\widehat{p}}_H\circ \widehat{k}$) $=$ Ker($p$) $= H$.

#### Hệ quả 4 {#ts-ii-s1-lem-10-cor-4 .statement tag=02JC}

Cho I là một tập hợp và cho $(H_i)_{i\in I}$ là một họ các nhóm con đóng của G. Trực giao của nhóm con đóng sinh bởi các $H_i$ là $\bigcap_{i\in I}H^{\bot}_i$. Trực giao của $\bigcap_iH_i$ là nhóm con đóng sinh bởi các nhóm con $H^{\bot}_i$.

Mệnh đề thứ nhất suy ra từ định nghĩa của trực giao. Áp dụng kết quả này và Hệ quả 3 cho họ các nhóm con đóng $(H^{\bot}_i)_{i\in I}$ của $\widehat{G}$, ta thấy rằng $\bigcap_iH_i$ là trực giao của nhóm con đóng sinh bởi các nhóm con $H^{\bot}_i$, và khi đó mệnh đề thứ hai được suy ra bằng đối ngẫu.

#### Hệ quả 5 {#ts-ii-s1-lem-10-cor-5 .statement tag=02JD}

Cho $\varphi : G\rightarrow H$ là một cấu xạ của các nhóm giao hoán compact địa phương. Khi đó nhóm con Im($\varphi$ ) của H và nhóm con Ker($\widehat{\varphi}$) của $\widehat{H}$ trực giao với nhau. Đặc biệt, để $\widehat{\varphi}$ là đơn ánh, điều kiện cần và đủ là ảnh của $\varphi$ trù mật trong H.

Ta có Ker($\widehat{\varphi}$) $=\varphi (G)^{\bot}$ (Bổ đề 2 của II, p. 205), do đó kết quả suy ra từ Hệ quả 3.

#### Hệ quả 6 {#ts-ii-s1-lem-10-cor-6 .statement tag=02JE}

Cho $k\in \mathbf{Z}$. Khi đó hạt nhân của đồng cấu $x\mapsto x^k$ từ G vào G và bao đóng của ảnh của cấu xạ $\chi \mapsto \chi^k$ từ $\widehat{G}$ vào $\widehat{G}$ trực giao với nhau.

Điều này suy ra từ Hệ quả trên vì các cấu xạ $x\mapsto x^k$ từ G vào G và $\chi \mapsto \chi^k$ từ $\widehat{G}$ vào $\widehat{G}$ là đối ngẫu của nhau.

Nhắc lại (A, X, p. 17) rằng một nhóm giao hoán A được gọi là chia được nếu, với mọi $n\in \mathbf{Z}$ khác không, ánh xạ $a\mapsto a^n$ từ A vào A là toàn ánh.

#### Hệ quả 7 {#ts-ii-s1-lem-10-cor-7 .statement tag=02JF}

Cho G là một nhóm giao hoán compact địa phương.

a) Nếu G chia được, thì nhóm đối ngẫu $\widehat{G}$ không xoắn ;

b) Nếu nhóm đối ngẫu $\widehat{G}$ không xoắn, và nếu $k\in \mathbf{Z}$ là khác không, thì ảnh của đồng cấu $x\mapsto x^k$ từ G vào G là trù mật trong G ;

c) Giả sử G rời rạc hoặc compact. Để G chia được, điều kiện cần và đủ là $\widehat{G}$ không xoắn.

Các khẳng định a) và b) suy ra từ Hệ quả 6. Nếu G rời rạc hoặc compact, ảnh của cấu xạ $x\mapsto x^k$ từ G vào G là đóng, và c) suy ra từ a) và b).

#### Nhận xét {#ts-ii-s1-n6-rem-1 .statement tag=02JG}

Tồn tại các nhóm giao hoán compact địa phương G không chia được và sao cho $\widehat{G}$ không xoắn (Bài tập 63 của II, p. 299).

### 7. Công thức Poisson

Trong số này, ta xét một nhóm con đóng H của G. Ta ký hiệu bởi $\beta =dx$ độ đo Haar trên G và bởi $\widehat{\beta}$ độ đo Haar đối ngẫu trên $\widehat{G}$. Ta ký hiệu bởi $\alpha$ một độ đo Haar trên H và bởi $\widehat{\alpha}$ độ đo Haar đối ngẫu trên nhóm đối ngẫu $\widehat{H}$, được đồng nhất với $\widehat{G}/H^{\bot}$ (Định lý 4 của II, p. 226). Ta cũng đồng nhất $\widehat{G}/H$ với $H^{\bot}$ bởi ánh xạ đối ngẫu của phép chiếu chính tắc $G\rightarrow G/H$ (loc. cit.).

Ta sẽ ký hiệu bởi $\dot{x}$ ảnh chính tắc của một phần tử $x$ của G trong $G/H$ và bởi $\dot{\chi}$ ảnh chính tắc của một phần tử $\chi$ của $\widehat{G}$ trong $\widehat{G}/H^{\bot}$.

Ta ký hiệu bởi $\gamma$ độ đo Haar $\beta /\alpha$ trên $G/H$ (INT, VII, §2, n$^o2$, Định nghĩa 1 và n$^o7$, Mệnh đề 10), và bởi $\widehat{\gamma}$ độ đo Haar đối ngẫu trên $H^{\bot}$. Nhắc lại (INT, VII, §2, n$^o3$, Mệnh đề 5, c)) rằng độ đo $\gamma$ được đặc trưng bởi tính chất sau: với mọi $f\in \mathscr{L}^1(G)$, hàm $y\mapsto f(xy)$ trên H là $\alpha$-khả tích với $\beta$-hầu khắp mọi $x\in G$ ; tích phân của nó chỉ phụ thuộc vào $\dot{x}$ và hàm được xác định $\gamma$-hầu khắp nơi trên $G/H$ bởi

$$
f^{\flat}: \dot{x}\mapsto \int_Hf(xh)d\alpha (h)
$$

thuộc $L^1(G/H, \gamma )$ và thỏa mãn

$$
\int_{G/H}f^{\flat}d\gamma =\int_Gf d\beta \tag{33}
$$

#### Mệnh đề 15 {#ts-ii-s1-prop-15 .statement tag=02JH}

Cho $f\in L^1(G)$ sao cho hạn chế lên $H^{\bot}$ của hàm liên tục $\mathscr{F}_G(f)$ là khả tích đối với $\widehat{\gamma}$. Khi đó, với hầu khắp mọi $x\in G$, hàm $y\mapsto f(xy)$ trên H là $\alpha$-khả tích, và ta có:

$$
\int_Hf(xy)d\alpha (y) =\int_{H^{\bot}}\langle \chi , x\rangle \mathscr{F}_G(f)(\chi )d\widehat{\gamma}(\chi )
$$

Từ điều trên, hàm $f^{\flat}$ được xác định hầu khắp nơi trên $G/H$ bởi

$$
f^{\flat}( \dot{x}) =\int_Hf(xy)d\alpha (y)
$$

thuộc $L^1(G/H)$. Biến đổi Fourier của $f^{\flat}$ được đồng nhất với hàm trên $H^{\bot}=\widehat{G}/H$ cho bởi, với $\chi \in H^{\bot}$,

$$
\mathscr{F}_{G/H}(f^{\flat})(\chi ) =\int_{G/H}\overline{\langle\chi ,\dot{x}\rangle}f^{\flat}( \dot{x})d\gamma ( \dot{x})
$$

$$
=\int_G\overline{\langle\chi , x\rangle}f(x)d\beta (x) =\mathscr{F}_G(f)(\chi )
$$

theo công thức (33), áp dụng cho hàm khả tích $x\mapsto$ $\overline{\langle\chi , x\rangle}f(x)$. Theo giả thiết, hàm $\mathscr{F}(f)|H^{\bot}=\mathscr{F}_{G/H}(f^{\flat})$ thuộc $L^1(H^{\bot})$, và do đó hàm $f^{\flat}$ thuộc không gian $B(G/H)$. Suy ra (Định lý 3 của II, p. 222) rằng $f^{\flat}$ trùng với $\overline{\mathscr{F}}_{\widehat{G}/H}(\mathscr{F}_{G/H}(f^{\flat}))$ hầu khắp nơi. Vì thế, với hầu hết mọi $\dot{x}\in G/H$, ta có

$$
f^{\flat}( \dot{x}) =\int_{H^{\bot}}\langle \chi , x\rangle \mathscr{F}_{G/H}(f^{\flat})(\chi )d\widehat{\gamma}(\chi ) =\int_{H^{\bot}}\langle \chi , x\rangle \mathscr{F}_G(f)(\chi )d\widehat{\gamma}(\chi )
$$

Điều này hoàn tất chứng minh.

#### Hệ quả (Công thức Poisson) {#ts-ii-s1-n7-cor-1 .statement tag=02JI}

Cho $f\in \mathscr{L}^1(G)$. Giả sử rằng các điều kiện sau được thỏa mãn:

(i) Hạn chế của $\mathscr{F}_G(f)$ lên $H^{\bot}$ là khả tích;

(ii) Với mọi $x\in G$, hàm $y\mapsto f(xy)$ trên H là khả tích;

(iii) Ánh xạ $x\mapsto \int_Hf(xy)d\alpha (y)$ là liên tục trên G.

Khi đó ta có

$$
\int_Hf(y)d\alpha (y) =\int_{H^{\bot}}\mathscr{F}_G(f)(\chi )d\widehat{\gamma}(\chi ) \tag{34}
$$

Thật vậy, với ký hiệu của chứng minh mệnh đề trước, các hàm $f^{\flat}$ và $\overline{\mathscr{F}}_{\widehat{G}/H}(\mathscr{F}_{G/H}(f^{\flat}))$ trên $G/H$ là liên tục và bằng nhau hầu khắp nơi. Vậy chúng bằng nhau khắp nơi và đặc biệt tại $e$, điều này cho công thức (34).

#### Mệnh đề 16 {#ts-ii-s1-prop-16 .statement tag=02JJ}

Độ đo $\widehat{\alpha}$ trên $\widehat{H} =\widehat{G}/H^{\bot}$ bằng $\widehat{\beta /}\widehat{\gamma}$.

Ta cố định một $f\in \mathscr{K}(G)$ khác không. Với $x\in G$ và $\chi \in \widehat{G}$, đặt

$$
\varphi (x, \chi ) =\int_Hf(xy)\langle \chi , y\rangle d\alpha (y)
$$

Hàm $\varphi$ là liên tục trên $G\times \widehat{G}$ (INT, IV, §4, n$^o3$, hệ quả 1 của Định lý 2). Với $x$ cố định, $\varphi (x, \chi )$ chỉ phụ thuộc vào lớp của $\chi$ trong $\widehat{G}/H^{\bot}=\widehat{H}$. Với $\chi$ cố định, $\langle \chi , x\rangle \varphi (x, \chi )$ chỉ phụ thuộc vào lớp của $x$ trong $G/H$, và hàm $\dot{x}\mapsto  \langle \chi , x\rangle \varphi (x, \chi )$ trên $G/H$ có giá compact.

Cho $x\in G$. Hàm $\dot{\chi}\mapsto \varphi (x, \chi )$ trên $\widehat{H}$ là đối biến đổi Fourier của hàm $y\mapsto f(xy)$ trên H. Hàm sau là khả tích bình phương, nên theo công thức Plancherel (23) của II, p. 217, ta có

$$
\int_{\widehat{G}/H^{\bot}}|\varphi (x, \chi )|^2d\widehat{\alpha}( \dot{\chi}) =\int_H|f(xy)|^2d\alpha (y) \tag{35}
$$

Cho $\chi \in \widehat{G}$. Hàm $\dot{x}\mapsto  \langle \chi , x\rangle \varphi (x, \chi )$ thuộc $\mathscr{K}(G/H)$, nên thuộc $L^1(G/H)$. Đối biến đổi Fourier của nó là hàm trên $H^{\bot}$ có giá trị tại $\xi \in H^{\bot}$ là

$$
\int_{G/H}\langle \xi ,\dot{x}\rangle \langle \chi , x\rangle \varphi (x, \chi )d\gamma ( \dot{x}) =\int_{G/H}(\int_H\langle \chi \xi , xy\rangle f(xy)d\alpha (y))d\gamma ( \dot{x})
$$

$$
=\int_G\langle \chi \xi , x\rangle f(x)d\beta (x) =\overline{\mathscr{F}}_G(f)(\chi \xi )
$$

theo công thức (33). Do đó

$$
\int_{G/H}|\varphi (x, \chi )|^2d\gamma ( \dot{x}) =\int_{H^{\bot}}|\overline{\mathscr{F}}_G(f)(\chi \xi )|^2d\widehat{\gamma}(\xi ) \tag{36}
$$

lại theo công thức Plancherel.

Cuối cùng ta tính được

$\int_{\widehat{G}}|\overline{\mathscr{F}}_G(f)|^2d\widehat{\beta}=\int_G|f|^2d\beta$ (theo (23))

$=\int_{G/H}d\gamma ( \dot{x})\int_H|f(xy)|^2d\alpha (y)$ (theo (33))

$=\int_{G/H}d\gamma ( \dot{x})\int_{\widehat{G}/H^{\bot}}|\varphi (x, \chi )|^2d\widehat{\alpha}( \dot{\chi})$ (theo (35))

$$
=\int_{\widehat{G}/H^{\bot}}d\widehat{\alpha}( \dot{\chi})\int_{G/H}|\varphi (x, \chi )|^2d\gamma ( \dot{x})
$$

$=\int_{\widehat{G}/H^{\bot}}d\widehat{\alpha}( \dot{\chi})\int_{H^{\bot}}|\overline{\mathscr{F}}_G(f)(\chi \xi )|^2d\widehat{\gamma}(\xi )$ (theo (36)),

trong đó INT, V, §8, No.$^o3$, mệnh đề 5 đã được áp dụng cho hàm liên tục dương $( \dot{x},\dot{\chi})\mapsto  |\varphi (x, \chi )|^2$ trên $G/H\times \widehat{G}/H^{\bot}$.

So sánh đẳng thức này với công thức tích phân (33) cho nhóm $\widehat{G}$, khi đó ta kết luận rằng các độ đo Haar $\widehat{\alpha}$ và $\widehat{\beta /}\widehat{\gamma}$ trùng nhau.

### 8. Ví dụ về đối ngẫu

#### Mệnh đề 17 {#ts-ii-s1-prop-17 .statement tag=02JK}

Cho $n\geqslant 1$ là một số nguyên. Ký hiệu bởi $\boldsymbol{\mu}_n$ nhóm các căn bậc $n$ của đơn vị trong $\mathbf{C}$. Các nhóm $\mathbf{Z}/n\mathbf{Z}$ và $\boldsymbol{\mu}_n$ đối ngẫu với nhau đối với ánh xạ cảm sinh khi chuyển sang thương từ ánh xạ $\mathbf{Z}\times \boldsymbol{\mu}_n\rightarrow \mathbf{U}$ được xác định bởi $(m, z)\mapsto z^m$.

Nhóm $\mathbf{Z}\widehat{/n}\mathbf{Z}$ trùng với tập hợp các đồng cấu $\chi$ từ $\mathbf{Z}/n\mathbf{Z}$ vào $\mathbf{U}$. Chúng có dạng $m\mapsto \chi (1)^m$, trong đó $\chi (1)$ là một phần tử tùy ý của $\mathbf{U}$ sao cho $\chi (1)^n= 1$, do đó suy ra kết quả.

#### Hệ quả 1 {#ts-ii-s1-prop-17-cor-1 .statement tag=02JL}

Cho G là một nhóm giao hoán hữu hạn. Nhóm đối ngẫu $\widehat{G}$ đẳng cấu với G.

Nhóm G đẳng cấu với một tích hữu hạn các nhóm cyclic (A, VII, p. 22, định lý 3), và nhóm đối ngẫu của nó đẳng cấu với tích của các nhóm đối ngẫu của các nhóm ấy (mệnh đề 2 của II, p. 206). Vì thế quy về trường hợp G là cyclic, trường hợp này thuộc mệnh đề 17 vì nhóm $\boldsymbol{\mu}_n$ là cyclic cấp $n$ (A, V, p. 75, định lý 1).

#### Hệ quả 2 {#ts-ii-s1-prop-17-cor-2 .statement tag=02JM}

Cho G là một nhóm giao hoán compact địa phương. Nhóm G là hữu hạn khi và chỉ khi $\widehat{G}$ hữu hạn. Một nhóm con đóng H của G có chỉ số hữu hạn khi và chỉ khi trực giao của nó là hữu hạn.

Theo đối ngẫu, mệnh đề thứ nhất suy ra từ sự kiện rằng đối ngẫu của một nhóm hữu hạn là hữu hạn (hệ quả 1). Mệnh đề thứ hai suy ra từ đó, vì $\widehat{G}/H$ được đồng nhất với $H^{\bot}$ (định lý 4 của II, p. 226).

#### Mệnh đề 18 {#ts-ii-s1-prop-18 .statement tag=02JN}

Để $\widehat{G}$ là compact, điều kiện cần và đủ là G rời rạc. Nếu G rời rạc, độ đo đối ngẫu của độ đo đếm trên G là độ đo Haar chuẩn hóa trên $\widehat{G}$. Nếu G compact, độ đo đối ngẫu của độ đo Haar chuẩn hóa là độ đo đếm trên $\widehat{G}$.

Giả sử G rời rạc, và gọi $\alpha$ là độ đo đếm trên G. Gọi $\varphi$ là hàm đặc số của $e\in G$. Ta có $\mathscr{F}_G(\varphi ) = 1$ trên $\widehat{G}$. Vì $\mathscr{F}_G(\varphi )$ tiến tới 0 tại vô cực, nhóm $\widehat{G}$ là compact.

Hơn nữa, đối với độ đo đối ngẫu $\widehat{\alpha}$ của $\alpha$, hàm $\mathscr{F}_G(\varphi )$ phải có tích phân bằng $\varphi (e) = 1$ (mệnh đề 12 của II, p. 219). Do đó $\widehat{\alpha}(\widehat{G}) = 1$.

Giả sử G compact. Khi đó độ đo Haar $dx$ thuộc $\mathscr{M}^1(G)$. Biến đổi Fourier của nó dương ngặt tại $\chi =e$ và bằng không đối với $\chi \not= 0$ (mệnh đề 6 của II, p. 210). Vì nó liên tục trên $\widehat{G}$, nhóm $\widehat{G}$ là rời rạc. Nếu độ đo của G bằng 1, theo đối ngẫu ta suy ra từ trường hợp trước rằng độ đo đối ngẫu của độ đo $dx$ là độ đo đếm trên $\widehat{G}$.

#### Hệ quả 1 (Các hệ thức trực giao) {#ts-ii-s1-prop-18-cor-1 .statement tag=02JO}

Giả sử G rời rạc và được trang bị độ đo đếm. Với $x$ và $y$ trong G, ta có

$\int$ 0 nếu $x\not=y$

$$
\chi (x)\chi (y)d\chi =
$$

$_{\widehat{G}}$ 1 nếu $x=y$.

Điều này suy ra từ hệ quả của định lý 1 của II, p. 215 và từ đối ngẫu.

#### Hệ quả 2 {#ts-ii-s1-prop-18-cor-2 .statement tag=02JP}

Cho H là một nhóm con đóng của G.

a) Để H là compact, điều kiện cần và đủ là $H^{\bot}$ mở trong $\widehat{G}$ ;

b) Để H là mở, điều kiện cần và đủ là $H^{\bot}$ compact trong $\widehat{G}$.

a) Nói rằng $H^{\bot}$ là mở có nghĩa là nói rằng $\widehat{G}/H^{\bot}$ là rời rạc, mà $\widehat{G}/H^{\bot}$ đẳng cấu với $\widehat{H}$ (Định lý 4 của II, p. 226); do đó mệnh đề suy ra từ Mệnh đề 18. Mệnh đề b) thu được bằng đối ngẫu từ mệnh đề a) áp dụng cho $H^{\bot}$.

#### Hệ quả 3 {#ts-ii-s1-prop-18-cor-3 .statement tag=02JQ}

Cho $(H_i)_{i\in I}$ là một họ lọc giảm các nhóm con compact của G. Để G được đồng nhất với giới hạn xạ ảnh của các nhóm $G/H_i$, điều kiện cần và đủ là $\widehat{G}$ là hợp của các nhóm con mở $H^{\bot}_i$.

Nói rằng G được đồng nhất với giới hạn xạ ảnh của các $G/H_i$ có nghĩa là nói rằng $\bigcap_iH_i=\{e\}$ (TG, III, p. 60, Mệnh đề 2), tức là $\bigcup_iH^{\bot}_i$ trù mật trong $\widehat{G}$ (Hệ quả 4 của Định lý 4 của II, p. 226). Mà $\bigcup_iH^{\bot}_i$ là một nhóm con mở, nên đóng, của $\widehat{G}$.

#### Hệ quả 4 {#ts-ii-s1-prop-18-cor-4 .statement tag=02JR}

Cho I là một tập hợp và cho $(H_i)_{i\in I}$ là một họ các nhóm compact. Đối ngẫu của nhóm tích của các $H_i$ là nhóm tổng trực tiếp rời rạc của các nhóm $\widehat{H}_i$.

Đây là một trường hợp riêng của Hệ quả 3.

#### Mệnh đề 19 {#ts-ii-s1-prop-19 .statement tag=02JS}

Cho K là một trường địa phương compact không rời rạc, không nhất thiết giao hoán, và cho G là nhóm cộng của K, với luật nhóm được ký hiệu theo lối cộng. Cho $\chi$ là một đặc trưng unita của G, phân biệt với 1. Với $x, y\in G$, đặt $\theta (x, y) =\chi (xy)$. Khi đó G đối ngẫu với chính nó đối với $\theta$.

Với $y\in G$, gọi $\chi_y$ là ánh xạ từ G vào $\mathbf{U}$ sao cho $\chi_y(x) =$ $\chi (xy)$. Ta có $\chi_y\in \widehat{G}$, và cần chứng minh rằng $\beta :y\mapsto \chi_y$ là một đẳng cấu các nhóm tôpô từ G lên $\widehat{G}$.

Ánh xạ $\beta$ là một đồng cấu đơn cấu của G vào $\widehat{G}$; nó liên tục (TG, X, p. 28, Định lý 3 áp dụng cho ánh xạ liên tục $\theta$ của $G\times G$ vào $\mathbf{C}$). Hãy chứng minh rằng $\theta$ là một đồng phôi lên ảnh của nó. Theo Bổ đề 2 của II, p. 200, chỉ cần chứng minh rằng với mọi lân cận U của 0 trong K, tồn tại một lân cận V của $e$ trong $\widehat{G}$ sao cho $\overset{-1}{\beta}(V)\subset U$. Gọi $x\mapsto  |x|$ là một giá trị tuyệt đối trên K xác định tôpô của K (AC, VI, §9, No$^o1$, Mệnh đề 1), và lấy $x_0\in K$ sao cho $\chi (x_0)\not= 1$; đặt $\eta =|\chi (x_0)-1|>0$. Cho U là một lân cận của 0 trong K. Tồn tại $\delta  >0$ sao cho U chứa tập các $y\in K$ thỏa mãn $|y|< \delta$. Gọi V là tập các đặc trưng $\xi \in \widehat{G}$ sao cho $|\langle \xi , x\rangle  -1|< \eta$ với mọi phần tử $x\in K$ thỏa mãn $|x|\leqslant |x_0|/\delta$. Đây là một lân cận của $e$ trong $\widehat{G}$. Nếu $y\not= 0$ sao cho $\beta (y)$ thuộc V, thì do đó ta có $|\chi (xy)-1|<|\chi (x_0)-1|$ với mọi $x$ sao cho $|x|\leqslant |x_0|/\delta$. Do đó, ta có $|x_0y^{-1}|>|x_0|/\delta$, và vì thế $|y|< \delta$, nên $y\in U$.

Vì $\beta$ là một đồng phôi lên ảnh của nó, nên ảnh ấy đóng trong $\widehat{G}$ (TG, III, p. 22, Hệ quả 2). Nhưng hơn nữa trực giao của ảnh của $\beta$ là tập các phần tử $x$ của G sao cho $\chi (xy) = 1$ với mọi $y\in G$, và do đó thu về $\{0\}$. Vậy ảnh của $\beta$ là trù mật trong $\widehat{G}$ (Hệ quả 3 của II, p. 228). Ta kết luận rằng $\beta$ là toàn ánh.

#### Hệ quả 1 {#ts-ii-s1-prop-19-cor-1 .statement tag=02JT}

Cho K là một trường địa phương compact không rời rạc, không nhất thiết giao hoán, và $\chi$ là một đặc trưng unita không tầm thường của nhóm cộng của K. Cho E là một không gian vectơ tôpô hữu hạn chiều trên K. Ánh xạ $\theta$ của $E\times E'$ vào $\mathbf{U}$ được xác định bởi $\theta (x, \lambda ) =\chi (\langle \lambda , x\rangle )$ với $(\lambda , x)\in E'\times E$ đặt các nhóm tôpô E và $E'$ vào thế đối ngẫu.

Gọi $n$ là chiều của E và $(e_1, . . . , e_n)$ là một cơ sở của E. Khi đó có thể đồng nhất E với $K^n$ (EVT, I, p. 14, Định lý 2). Kết quả suy ra từ Mệnh đề 19 và Mệnh đề 2 của II, p. 206.

Ta ký hiệu bởi $\mathbf{T}$ nhóm $\mathbf{R}/\mathbf{Z}$.

#### Hệ quả 2 {#ts-ii-s1-prop-19-cor-2 .statement tag=02JU}

a) Nhóm $\mathbf{R}$ đối ngẫu với chính nó đối với ánh xạ $(x, y)\mapsto$ exp(2$i\pi xy$), và đối ngẫu của độ đo Lebesgue là độ đo Lebesgue ;

b) Các nhóm $\mathbf{Z}$ và $\mathbf{T}$ đối ngẫu với nhau đối với ánh xạ thu được bằng cách chuyển qua thương từ ánh xạ của $\mathbf{Z}\times \mathbf{R}$ vào $\mathbf{U}$ sao cho $(n, x)\mapsto$ exp(2$i\pi nx$). Độ đo Haar đối ngẫu của độ đo đếm trên $\mathbf{Z}$ là độ đo Haar được chuẩn hoá trên $\mathbf{R}/\mathbf{Z}$.

Nhóm $\mathbf{R}$ đối ngẫu với chính nó đối với ánh xạ $(x, y)\mapsto$ exp(2$i\pi xy$), theo Mệnh đề 19. Ta đồng nhất $\widehat{\mathbf{R}}$ với $\mathbf{R}$. Khi đó trực giao của $\mathbf{Z}$ trong $\widehat{\mathbf{R}}=\mathbf{R}$ là $\mathbf{Z}$, và b) suy ra từ Định lý 4 của II, p. 226.

Gọi $\alpha$ là độ đo đếm trên $\mathbf{Z}$ và $\gamma$ là độ đo Haar được chuẩn hoá trên $\mathbf{T}$. Nếu $\beta$ kí hiệu độ đo Lebesgue trên $\mathbf{R}$, ta có $\gamma =\beta /\alpha$, vì hai độ đo Haar này trên $\mathbf{R}/\mathbf{Z}$ đều có khối lượng 1. Độ đo Haar $\widehat{\alpha}$ trên $\widehat{\mathbf{Z}}=\mathbf{T}$ là độ đo Haar được chuẩn hoá (Mệnh đề 18), và độ đo Haar $\widehat{\gamma}$ là độ đo đếm trên $\mathbf{Z}($loc. cit.). Theo Mệnh đề 16 của II, p. 231, độ đo đối ngẫu của $\beta$ do đó là độ đo $\beta$.

#### Nhận xét {#ts-ii-s1-n8-rem-1 .statement tag=02JV}

Đặc biệt, ta tìm lại sự xác định của $\mathsf{X}(L^1(\mathbf{Z}))$ đã cho trong Ví dụ 4 của I, p. 36.

Với mọi số nguyên $n\geqslant 0$ và $(x, y)\in \mathbf{R}^n\times \mathbf{R}^n$, ta viết

$$
x\cdot y=\sum_{j=1}^nx_jy_j
$$

#### Hệ quả 3 {#ts-ii-s1-prop-19-cor-3 .statement tag=02JW}

Cho $n\geqslant 1$ là một số nguyên. Nhóm $\mathbf{R}^n$ đối ngẫu với chính nó đối với ánh xạ $(x, y)\mapsto$ exp(2$i\pi  x\cdot y$), và độ đo đối ngẫu của độ đo Lebesgue trên $\mathbf{R}^n$ là độ đo Lebesgue. Các nhóm $\mathbf{Z}^n$ và $\mathbf{T}^n=\mathbf{R}^n/\mathbf{Z}^n$ đối ngẫu với nhau đối với ánh xạ thu được bằng cách chuyển qua thương từ ánh xạ $(n, x)\mapsto$ exp(2$i\pi  x\cdot y$), và độ đo Haar đối ngẫu của độ đo đếm trên $\mathbf{Z}^n$ là độ đo Haar được chuẩn hoá trên $(\mathbf{R}/\mathbf{Z})^n$.

Điều này suy ra từ Bổ đề 7 của II, p. 225, Mệnh đề 10 của II, p. 217 và Hệ quả 2.

#### Nhận xét {#ts-ii-s1-n8-rem-2 .statement tag=02JX}

Cho một nhóm con H của $\mathbf{R}^n$, ứng với nó là trực giao của nó $H^{\bot}$, một nhóm con của $\widehat{\mathbf{R}}^n=\mathbf{R}^n$, mà không là gì khác hơn nhóm con liên kết với H được định nghĩa trong TG, VII, p. 6, n$^o3$.

Trong phần tiếp theo, người ta sẽ đồng nhất đối ngẫu của $\mathbf{R}^n$ (resp. của $\mathbf{T}^n$) với $\mathbf{R}^n$ (resp. với $\mathbf{Z}^n$) bởi tính đối ngẫu của hệ quả. Đặc biệt, với $f\in L^1(\mathbf{R}^n)$, biến đổi Fourier của nó được đồng nhất với hàm từ $\mathbf{R}^n$ vào $\mathbf{C}$ gán cho $y\in \mathbf{R}^n$

$\mathscr{F}(f)(y) =\int_{\mathbf{R}^n}f(x)$ exp($-2i\pi  x\cdot y$)$dx$.

#### Hệ quả 4 {#ts-ii-s1-prop-19-cor-4 .statement tag=02JY}

Nhóm $\mathbf{R}^*$ đối ngẫu với nhóm $\{-1,1\} \times \mathbf{R}$ qua ánh xạ $(x,(\sigma , t))\mapsto \sigma (x/|x|)|x|^{it}$. Nhóm $\mathbf{R}^*_+$ đối ngẫu với $\mathbf{R}$ qua ánh xạ $(x, t)\mapsto x^{it}$.

Thực vậy, ánh xạ $x\mapsto (x/|x|$, log($|x|$)) là một đẳng cấu nhóm tôpô từ $\mathbf{R}^*$ lên $\{-1,1\} \times \mathbf{R}$. Mệnh đề khi đó suy ra từ bổ đề 7 của II, p. 225, từ hệ quả 2, và từ sự kiện rằng các đặc trưng unita của $\{-1,1\}$ là 1 và $x\mapsto x$.

Cho $p$ là một số nguyên tố. Trường $\mathbf{Q}_p$ các số $p$-adic là phép hoàn thiện của $\mathbf{Q}$ đối với định giá $p$-adic (INT, VII, § 1, No.$^o6$, ví dụ, và AC, VI, § 3, No.$^o4$, ví dụ 4). Với mọi $x\in \mathbf{Q}_p$, tồn tại duy nhất một số nguyên $\nu \geqslant 0$ và duy nhất một số nguyên $q$ thỏa mãn $0\leqslant q < p^{\nu}$ sao cho $qp^{-\nu}-x\in \mathbf{Z}_p$ (A, VII, p. 10, Định lý 2, áp dụng cho miền iđêan chính $\mathbf{Z}_p$ và cho tập hợp $R_p$ các số nguyên $j$ sao cho $0\leqslant j < p$). Ta đặt $\lambda (x) =qp^{-\nu}$.

#### Mệnh đề 20 {#ts-ii-s1-prop-20 .statement tag=02JZ}

Ánh xạ $x\mapsto$ exp(2$i\pi \lambda (x)$) là một đặc trưng unita của $\mathbf{Q}_p$ mà hạt nhân là $\mathbf{Z}_p$.

Với $x_1$ và $x_2$ trong $\mathbf{Q}_p$, theo định nghĩa ta có $\lambda (x_1+x_2)-\lambda (x_1)-\lambda (x_2)\in$ $\mathbf{Z}_p\cap \mathbf{Q}=\mathbf{Z}$. Hơn nữa ánh xạ $\lambda$ là địa phương hằng vì $\lambda (x+y) =\lambda (x)$ nếu $y\in \mathbf{Z}_p$. Do đó suy ra rằng $x\mapsto$ exp(2$i\pi \lambda (x)$) là một đặc trưng unita của $\mathbf{Q}_p$. Vì $\lambda (x)\in \mathbf{Z}$ khi và chỉ khi $x\in \mathbf{Z}_p$, hạt nhân của đặc trưng này là $\mathbf{Z}_p$.

Ta nhắc lại rằng độ đo Haar chuẩn hoá trên nhóm cộng của $\mathbf{Q}_p$ là độ đo Haar duy nhất $\mu$ sao cho $\mu(\mathbf{Z}_p) = 1$ (INT, VII, §1, No.$^o6$, ví dụ).

#### Hệ quả {#ts-ii-s1-n8-cor-1 .statement tag=02K0}

a) Nhóm $\mathbf{Q}_p$ đối ngẫu với chính nó đối với ánh xạ $(x, y)\mapsto$ exp(2$i\pi \lambda (xy)$). Khi đó độ đo Haar chuẩn hoá trên $\mathbf{Q}_p$ là đối ngẫu của chính nó ;

b) Các nhóm $\mathbf{Z}_p$ và $\mathbf{Q}_p/\mathbf{Z}_p$ là đối ngẫu đối với ánh xạ thu được bằng cách chuyển qua thương từ ánh xạ được xác định bởi $(z, x)\mapsto$ exp(2$i\pi \lambda (zx)$), và độ đo đối ngẫu của độ đo Haar chuẩn hóa trên $\mathbf{Z}_p$ là độ đo đếm trên $\mathbf{Q}_p/\mathbf{Z}_p$.

Chứng minh theo từng bước chứng minh của Hệ quả 2 của Mệnh đề 19.

### 9. Biến đổi Fourier Euclid và Chuỗi Fourier

$*$ Cho $n\in \mathbf{N}$. Ta đồng nhất $\mathbf{R}^n$ với đối ngẫu của nó như trong Hệ quả 3 của II, p. 236. Khi đó độ đo đối ngẫu của độ đo Lebesgue là độ đo Lebesgue. Ta trang bị cho $\mathbf{R}^n$ chuẩn Euclid. Với mọi đa chỉ số $\alpha \in \mathbf{N}^n$, và mọi $x= (x_1, . . . , x_n)\in \mathbf{R}^n$, ta viết $x^{\alpha}=x^{\alpha_1}_1\cdots x^{\alpha_n}_n$, và ta ký hiệu bởi $X^{\alpha}$ hàm $x\mapsto x^{\alpha}$ trên $\mathbf{R}^n$.

Cho $m\in \mathbf{R}^m$. Mọi cấu xạ liên tục của các nhóm giao hoán từ $\mathbf{R}^m$ vào $\mathbf{R}^n$ đều là một ánh xạ tuyến tính $\sigma \in \mathscr{L}(\mathbf{R}^n,\mathbf{R}^m)$ (TG, VII, p. 11, Prop. 1). Cấu xạ đối ngẫu $\widehat{\sigma}$ được đồng nhất với ánh xạ tuyến tính $^t\sigma$.

Biến đổi Fourier trên $\mathbf{R}^n$ có một dạng đặc biệt thuận tiện trong khung cảnh của không gian các hàm Schwartz và của đối ngẫu của nó (IV, sẽ xuất hiện). Ở đây ta tóm tắt các kết quả chính của nó.

Gọi $\mathscr{S}(\mathbf{R}^n)$ là không gian các hàm $\varphi$ khả vi vô hạn lần, nhận giá trị phức trên $\mathbf{R}^n$, sao cho, với mọi đa chỉ số $\alpha \in \mathbf{N}^n$ và mọi số nguyên $k\in \mathbf{N}$, hàm

$$
x\mapsto  \|x\|^k\partial^{\alpha}\varphi (x)
$$

bị chặn trên $\mathbf{R}^n$. Ta trang bị cho $\mathscr{S}(\mathbf{R}^n)$ tôpô lồi địa phương được xác định bởi các nửa chuẩn

$p_{k,\alpha}:\varphi \mapsto$ sup$_{x\in\mathbf{R}^n}\|x\|^k|\partial^{\alpha}\varphi (x)|$.

Người ta nói rằng $\mathscr{S}(\mathbf{R}^n)$ là không gian các hàm Schwartz trên $\mathbf{R}^n$.

Với mọi $\alpha \in \mathbf{N}^n$, các ánh xạ $\varphi \mapsto \partial^{\alpha}\varphi$ và $\varphi \mapsto X^{\alpha}\varphi$ là liên tục từ $\mathscr{S}(\mathbf{R}^n)$ vào chính nó. Không gian $\mathscr{S}(\mathbf{R}^n)$ là một đại số tôpô; nó là một không gian Fréchet và một không gian Montel (TVS IV, p. 18, Def. 4). Với mọi $p\in [1,+\infty ]$, không gian $\mathscr{S}(\mathbf{R}^n)$ được chứa trong $\mathscr{L}^p(\mathbf{R}^n)$ và đơn ánh chính tắc của $\mathscr{S}(\mathbf{R}^n)$ vào $\mathscr{L}^p(\mathbf{R}^n)$ là liên tục. Ảnh của $\mathscr{S}(\mathbf{R}^n)$ trong $L^p(\mathbf{R}^n)$ là trù mật nếu $p\not= +\infty$.

Vì mọi hàm Schwartz $\varphi$ đều khả tích trên $\mathbf{R}^n$, nó có một biến đổi Fourier ký hiệu bởi $\widehat{\varphi}$, được đồng nhất với hàm liên tục trên $\mathbf{R}^n$ xác định bởi

$y\mapsto \int_{\mathbf{R}^n}\varphi (x)$ exp($-2i\pi  x\cdot y$)$dx$.

Biến đổi Fourier đối của $\varphi$ về phần nó được đồng nhất với hàm liên tục xác định bởi

$y\mapsto \int_{\mathbf{R}^n}\varphi (x)$ exp(2$i\pi  x\cdot y$)$dx$.

Cho $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Cho $\alpha \in \mathbf{N}^n$ là một đa chỉ số. Ta có

$$
\mathscr{F}(\partial^{\alpha}\varphi ) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(\varphi )
$$

$$
\mathscr{F}(X^{\alpha}\varphi ) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(\varphi ))
$$

#### Mệnh đề 21 {#ts-ii-s1-prop-21 .statement tag=02K1}

Hạn chế của biến đổi Fourier lên $\mathscr{S}(\mathbf{R}^n)$ là một tự đẳng cấu của các không gian vectơ tôpô mà nghịch đảo là hạn chế của đối biến đổi Fourier.

Cho $\Lambda \subset \mathbf{R}^n$ là một dàn (TG, VII, p. 4), và cho $\Lambda^*\subset \mathbf{R}^n$ là dàn liên kết (TG, VII, p. 6), cũng đôi khi được gọi là dàn đối ngẫu.

Đối thể tích của dàn Λ, theo định nghĩa, là độ đo của $\mathbf{R}^n/\Lambda$ đối với độ đo Haar cảm sinh bởi độ đo Lebesgue trên $\mathbf{R}^n($xem INT, VIII, §5, n$^o5$, ví dụ), và được ký hiệu bởi V(Λ). Với mọi hàm $f\in$ $\mathscr{S}(\mathbf{R}^n)$ và mọi $y\in \mathbf{R}^n$, ta có công thức Poisson

1

$\sum f(x+y) =\sum\widehat{f}(z)$ exp(2$i\pi  y\cdot z$).

V(Λ) $_*$

$x\in \Lambda z\in \Lambda$

#### Nhận xét 1 {#ts-ii-s1-n9-rem-1 .statement tag=02K2}

Tổng quát hơn, theo hệ quả của mệnh đề 15 của II, p. 230, công thức này đúng với mọi hàm phức khả tích trên $\mathbf{R}^n$ sao cho

$$
\sum_{x\in\Lambda}|f(x+y)|<+\infty
$$

với mọi $y\in \mathbf{R}^n$ và sao cho hàm trên $\mathbf{T}^n$ được xác định bởi

$$
y\mapsto \sum_{x\in\Lambda}f(x+y)
$$

là liên tục và có một chuỗi Fourier hội tụ tuyệt đối (xem dưới đây).

#### Nhận xét 2 {#ts-ii-s1-n9-rem-2 .statement tag=02K3}

Tồn tại những hàm $f\in B(\mathbf{R})$ sao cho chuỗi $\sum_{n\in\mathbf{Z}}f(n)$ phân kỳ (bài tập 4 của II, p. 263).

#### Ví dụ {#ts-ii-s1-n9-exa-1 .statement tag=02K4}

Cho Q là một dạng toàn phương xác định dương trên $\mathbf{R}^n$. Hàm được xác định bởi $\varphi (x) =$ exp($-\pi Q(x)$) thuộc $\mathscr{S}(\mathbf{R}^n)$. Tồn tại $\sigma \in$ GL($n,\mathbf{R}$) sao cho $Q(x) =\|\sigma (x)\|^2$ với mọi $x\in \mathbf{R}^n$. Biến đổi Fourier của $\varphi$ được cho, với mọi $y\in \mathbf{R}^n$, bởi

$\widehat{\varphi}(y) =|$det($1\sigma$ )$|$ exp($-\pi Q^*(y)$)

trong đó $Q^*(y) =\|^t\sigma^{-1}(y)\|^2($xem INT, IX, §6, n$^o$ 4–5 và bài tập 1, c) của II, p. 262).

#### Định nghĩa 6 {#ts-ii-s1-def-6 .statement tag=02K5}

Không gian các phân phối ôn hòa trên $\mathbf{R}^n)$, theo định nghĩa, là không gian đối ngẫu của $\mathscr{S}(\mathbf{R}^n)$ được trang bị tôpô hội tụ bị chặn. Nó được ký hiệu bởi $\mathscr{S}'(\mathbf{R}^n)$.

Vì $\mathscr{S}(\mathbf{R}^n)$ là bornological, không gian $\mathscr{S}'(\mathbf{R}^n)$ là đầy đủ và bornological (EVT, III, p. 24, cor. 1 and 2). Vì $\mathscr{S}(\mathbf{R}^n)$ là một không gian Montel, điều tương tự cũng đúng cho $\mathscr{S}'(\mathbf{R}^n)$ (EVT, IV, p. 19, prop. 9).

Cho $\alpha \in \mathbf{N}^n$. Chuyển vị của tự đồng cấu $\varphi \mapsto X^{\alpha}\varphi$ của $\mathscr{S}(\mathbf{R}^n)$ lại được ký hiệu bởi $f\mapsto X^{\alpha}f$, và $f\mapsto \partial^{\alpha}f$ ký hiệu tự đồng cấu của $\mathscr{S}'(\mathbf{R}^n)$ được xác định bởi

$$
\langle \partial^{\alpha}f, \varphi \rangle = (-1)^{|\alpha|}\langle f, \partial^{\alpha}\varphi \rangle
$$

với $f\in \mathscr{S}'(\mathbf{R}^n)$ và $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

Cho $f$ là một ánh xạ tuyến tính từ $\mathscr{S}(\mathbf{R}^n)$ vào $\mathbf{C}$. Khi đó $f$ là một phân phối ôn hòa khi, và chỉ khi, với mọi họ $(M_{k,\alpha})_{(k,\alpha)\in\mathbf{N}\times\mathbf{N}^n}$ trong $\mathbf{R}_+$, dạng tuyến tính $f$ bị chặn trên tập các hàm $\varphi \in \mathscr{S}(\mathbf{R}^n)$ sao cho với mọi $(k, \alpha )\in \mathbf{N}\times \mathbf{N}^n$, ta có $p_{k,\alpha}(\varphi )\leqslant M_{k,\alpha}$.

Một dãy $(f_m)_{m\in\mathbf{N}}$ các phân phối ôn hòa hội tụ tới một phân phối ôn hòa $f$ khi, và chỉ khi, ta có $\langle f_m, \varphi \rangle  \rightarrow  \langle f, \varphi \rangle$ với mọi $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

#### Ví dụ {#ts-ii-s1-n9-exa-2 .statement tag=02K6}

Một độ đo $\nu$ trên $\mathbf{R}^n$ được gọi là ôn hòa nếu tồn tại một số nguyên dương $r$ sao cho ánh xạ liên tục $x\mapsto (1+\|x\|)^{-r}$ là $\nu$-khả tích trên $\mathbf{R}^n$. Hạn chế của $\nu$ lên $\mathscr{S}(\mathbf{R}^n)$ là một phân phối ôn hòa. Nó bằng không khi và chỉ khi độ đo $\nu$ bằng không.

Cho $p\in [1,+\infty ]$ và $f\in \mathscr{L}^p(\mathbf{R}^n)$. Khi đó độ đo $f\cdot dx$ có mật độ $f$ đối với độ đo Lebesgue là ôn hòa. Đặc biệt, độ đo Lebesgue $\mu$ trên $\mathbf{R}^n$ là ôn hòa, và mọi độ đo bị chặn trên $\mathbf{R}^n$ đều là ôn hòa.

Với mọi $p\in [1,+\infty ]$, có thể đồng nhất $L^p(\mathbf{R}^n)$ với một không gian con của $\mathscr{S}'(\mathbf{R}^n)$ bởi ánh xạ tuyến tính $f\mapsto f\cdot dx$; ánh xạ này là liên tục.

#### Định nghĩa 7 {#ts-ii-s1-def-7 .statement tag=02K7}

Chuyển vị của biến đổi Fourier trên $\mathscr{S}(\mathbf{R}^n)$ (tương ứng, của biến đổi Fourier nghịch đảo) được gọi là biến đổi Fourier trên $\mathscr{S}'(\mathbf{R}^n)$, và được ký hiệu bởi $\mathscr{F}$ (tương ứng, được gọi là biến đổi Fourier nghịch đảo, và được ký hiệu bởi $\overline{\mathscr{F}}$).

Với $f\in \mathscr{S}'(\mathbf{R}^n)$, phân phối ôn hòa $\mathscr{F}(f)$ (tương ứng. $\overline{\mathscr{F}}(f)$) được định nghĩa bởi $\varphi \mapsto  \langle f,\mathscr{F}(\varphi )\rangle$ với $\varphi \in \mathscr{S}(\mathbf{R}^n)$ (tương ứng. bởi $\varphi \mapsto$ $\langle f,\overline{\mathscr{F}}(\varphi )\rangle$ ).

Biến đổi Fourier trên $\mathscr{S}'(\mathbf{R}^n)$ là một tự đẳng cấu của các không gian vectơ tôpô có nghịch đảo là biến đổi Fourier nghịch đảo $\overline{\mathscr{F}}$.

#### Mệnh đề 22 {#ts-ii-s1-prop-22 .statement tag=02K8}

Cho $f$ là một phân phối ôn hòa thuộc $\mathscr{M}^1(\mathbf{R}^n)$ (tương ứng. thuộc $L^2(\mathbf{R}^n)$). Biến đổi Fourier của $f$ trong $\mathscr{S}'(\mathbf{R}^n)$ là phân phối ôn hòa liên kết với biến đổi Fourier của $f$ trong $\mathscr{C}_0(\mathbf{R}^n)$ (tương ứng. trong $L^2(\mathbf{R}^n)$). Tương tự đối với biến đổi Fourier nghịch đảo.

#### Nhận xét {#ts-ii-s1-n9-rem-3 .statement tag=02K9}

Các công thức sơ cấp liên quan đến biến đổi Fourier của các độ đo vẫn còn đúng đối với biến đổi Fourier của các phân phối ôn hòa.

Do đó, nếu $\alpha \in \mathbf{N}^n$ và $f\in \mathscr{S}'(\mathbf{R}^n)$, ta có

$$
\mathscr{F}(\partial^{\alpha}f) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(f)
$$

$$
\mathscr{F}(X^{\alpha}f) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(f))
$$

Cho $y\in \mathbf{R}^n$. Ta ký hiệu bởi $\boldsymbol{\gamma }(y)$ tự đồng cấu của $\mathscr{S}'(\mathbf{R}^n)$ được xác định bởi

$$
\langle \boldsymbol{\gamma }(y)f, \varphi \rangle =\langle f,\boldsymbol{\gamma }(-y)\varphi \rangle
$$

với $f\in \mathscr{S}'(\mathbf{R}^n)$ và $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Gọi $e_y$ là đặc trưng của $\mathbf{R}^n$ sao cho $e_y(x) =$ exp(2$i\pi x\cdot y$). Khi đó $e_y\in \mathscr{S}'(\mathbf{R}^n)$. Ta có $\mathscr{F}(e_y) =\varepsilon_y$, và nói chung hơn

$$
\mathscr{F}(e_yf) =\boldsymbol{\gamma }(y)\mathscr{F}(f)
$$

với mọi $f\in \mathscr{S}'(\mathbf{R}^n).*$

Cho $n\geqslant 1$ là một số nguyên, và đặt $G =\mathbf{T}^n$, được trang bị độ đo Haar chuẩn hóa. Nhóm đối ngẫu của G được đồng nhất với $\mathbf{Z}^n$ bởi ánh xạ $h\mapsto \chi_h$, trong đó $\chi_h$ là đặc trưng unita của $\mathbf{T}^n$ thu được bằng cách chuyển qua thương từ đặc trưng $x\mapsto$ exp(2$i\pi h\cdot x$) của $\mathbf{R}^n$ (Hệ quả 3 của II, p. 236). Biến đổi Fourier của một độ đo $\mu$ trên $\mathbf{T}^n$ được đồng nhất với họ $(\widehat{\mu}(h))_{h\in\mathbf{Z}^n}$ trong đó

$$
\widehat{\mu}(h) =\int_{\mathbf{T}^n}e^{-2i\pi h\cdot x}d\mu(x)
$$

Chuỗi

$$
\sum_{h\in\mathbf{Z}^n}\widehat{\mu}(h)\chi_h
$$

được gọi là chuỗi Fourier của $\mu$.

Nếu $f\in L^1(\mathbf{T}^n)$ sao cho chuỗi Fourier của nó hội tụ tuyệt đối trong $L^1(\mathbf{Z}^n)$, thì $f\in \mathscr{C}(\mathbf{T}^n)$ và

$$
f(x) =\sum_{h\in\mathbf{Z}^n}\widehat{f}(h)e^{2i\pi h\cdot x}
$$

với mọi $x\in \mathbf{T}^n$ (Định lý 3 của II, p. 222), trong đó

$$
\widehat{f}(h) =\int_{\mathbf{T}^n}f(x)e^{-2i\pi h\cdot x}dx,h\in \mathbf{Z}^n
$$

Đối với $f\in L^2(\mathbf{T}^n)$, công thức đảo Fourier (Mệnh đề 12 của II, p. 219) phát biểu rằng, nếu chuỗi có số hạng tổng quát $\widehat{f}(h)$ hội tụ tuyệt đối, thì có

$$
f(x) =\sum_{h\in\mathbf{Z}^n}\widehat{f}(h)e^{2i\pi h\cdot x}
$$

với hầu khắp mọi $x$ trong $\mathbf{T}^n$.

Tuy nhiên, ngay cả khi $f$ liên tục, chuỗi Fourier của $f$ nói chung không hội tụ tới $f(x)$ với mọi $x$ (Bài tập 30 của II, p. 274). Kết quả sau đây vì thế càng hữu ích hơn.

#### Mệnh đề 23 (định lý Fejér) {#ts-ii-s1-prop-23 .statement tag=02KA}

Cho $n\geqslant 1$ là một số nguyên. Với mọi $h= (h_i)\in \mathbf{Z}^n$, đặt $|h|=$ sup$_i|h_i|$. Cho $f\in \mathscr{C}(\mathbf{T}^n)$. Với mọi số nguyên $N\geqslant 1$, ta ký hiệu bởi $f_N$ hàm trên $\mathbf{T}^n$ sao cho

$$
f_N(x) =\sum_{\substack{h\in\mathbf{Z}^n\\|h|\leqslant N}}\widehat{f}(h)e^{2i\pi h\cdot x}\prod_{j=1}^n\left(1-\frac{|h_j|}{N}\right)
$$

với $x\in \mathbf{T}^n$. Khi đó $f_N$ hội tụ tới $f$ trong $\mathscr{C}(\mathbf{T}^n)$.

#### Bổ đề 11 {#ts-ii-s1-lem-11 .statement tag=02KB}

Với mọi $N\geqslant 1$, gọi $\mu_N$ là độ đo trên $\mathbf{T}^n$ có mật độ là ánh xạ liên tục

$$
F_N:x\mapsto \sum_{\substack{h\in\mathbf{Z}^n\\|h|\leqslant N}}e^{2i\pi h\cdot x}\prod_{j=1}^n\left(1-\frac{|h_j|}{N}\right).
$$

Dãy các độ đo $(\mu_N)_{N\geqslant 1}$ hội tụ đến $\varepsilon_0$ trong không gian $\mathscr{M}^1(\mathbf{T}^n)$ được trang bị tôpô hội tụ compắc trong $\mathscr{C}(\mathbf{T}^n)$.

Ta quy về trường hợp $n= 1$ bằng cách nhận thấy rằng $\mu_N$ là tích của các độ đo cùng kiểu đối với $n= 1$. Khi đó chỉ cần kiểm tra rằng dãy $(\mu_N)$ thỏa mãn các giả thiết của bổ đề 4 của INT, VIII, §2, No.$^o7$ với $a= 0$.

Để làm việc đó, trước hết hãy nhận thấy rằng $F_N$ là đối biến đổi Fourier của ánh xạ $\varphi_N:h\mapsto (1- |h|/N)$ trên $\mathbf{Z}$. Điều này có thể viết thành $\varphi_N=$ $N^{-1}\psi_N*\widetilde{\psi}_N$, trong đó $\psi_N$ là hàm đặc trưng của tập hợp được xác định bởi $-N/2<|h|\leqslant N/2$. Do đó, $F_N= N^{-1}|\mathscr{F}(\psi_N)|^2\geqslant 0$. Vậy $\mu_N$ là một độ đo dương; ta có $\mu_N(\mathbf{T}) = 1$, điều này chứng minh (i) và (iii) ở nơi đã dẫn.

Ta hãy chứng minh điều kiện (ii) ở nơi đã dẫn. Cho U là một lân cận mở của 0 trong $\mathbf{T}$. Chỉ cần chứng minh rằng $\mu_N(U)\rightarrow 1$ khi $N\rightarrow +\infty$. Cho K là một lân cận compắc đối xứng của 0 sao cho $K^2\subset U$ và gọi $\psi$ là hàm đặc trưng của K. Đặt $\varphi =\psi *\psi$. Đó là một phần tử của $A(\mathbf{T})$ với giá được chứa trong U. Số thực $m=\varphi (0)$ là độ đo của tập hợp K và do đó $m >0$. Hơn nữa, ta có $0\leqslant \varphi \leqslant m$ vì $\varphi (x)$ là độ đo của tập hợp $K\cap xK$. Ta có

$$
\mu_N(U)\geqslant \frac{1}{m}\int_{\mathbf{T}}\varphi (x)\mu_N(x) =\frac{1}{m}\sum\mathscr{F}(\varphi )(h)\varphi_N(h)
$$

$h\in \mathbf{Z}$

theo các tính chất chuyển vị của biến đổi Fourier (mệnh đề 13 của II, p. 221). Vì $\varphi \in A(\mathbf{T})$, biến đổi Fourier của nó thuộc $L^1(\mathbf{Z})$ và $\varphi$ thỏa mãn công thức đảo Fourier (mệnh đề 11 của II, p. 217). Vì $\varphi_N(h)\rightarrow 1$ với mọi $h\in \mathbf{Z}$ và $|\varphi_N(h)|\leqslant 1$, định lý Lebesgue (INT, IV, §3, n$^o7$, th. 6) và công thức đảo Fourier suy ra rằng

lim inf$_{N\rightarrow+\infty}\mu_N(U)\geqslant \frac{1}{m}$ lim$_{N\rightarrow+\infty}\sum_{h\in\mathbf{Z}}\mathscr{F}(\varphi )(h)\varphi_N(h) =$

1 $\sum\mathscr{F}(\varphi )(h) =1\varphi (0) = 1$.

$$
m_{h\in\mathbf{Z}}m
$$

Ta hãy chứng minh mệnh đề. Ta có $f*F_N=f_N$ với $N\geqslant 1$. Biểu diễn chính quy $\boldsymbol{\gamma }$ của $\mathbf{T}^n$ trong $\mathscr{C}(\mathbf{T}^n)$ (INT, VIII, §2, No.$^o3$) là liên tục và thỏa mãn $f*F_N=\boldsymbol{\gamma }(\mu_N)f$ (INT, VIII, §4, No.$^o5$, prop. 5 (iv)). Ánh xạ $\mu\mapsto \boldsymbol{\gamma }(\mu)f$ là liên tục từ $\mathscr{M}^1(\mathbf{T}^n)$ vào $\mathscr{C}(\mathbf{T}^n)$ (INT, VI, §1, No.$^o6$, prop. 14). Theo bổ đề, do đó ta có

lim$_{N\rightarrow+\infty}f_N=$ lim$_{N\rightarrow+\infty}f*F_N=$ lim$_{N\rightarrow+\infty}\boldsymbol{\gamma }(\mu_N)f=\boldsymbol{\gamma }(\varepsilon_0)(f) =f$

trong $\mathscr{C}(\mathbf{T}^n)$.

#### Nhận xét {#ts-ii-s1-n9-rem-4 .statement tag=02KC}

Tồn tại các hàm $f\in L^1(\mathbf{T})$ mà chuỗi Fourier phân kỳ tại mọi điểm $x\in \mathbf{T}$ (định lý của Kolmogorov, xem bài tập 51 của II, p. 289).

Một định lý của Carleson[^1] chỉ ra rằng các tổng riêng đối xứng của chuỗi Fourier của $f$ hội tụ tới $f(x)$ với hầu khắp mọi $x\in \mathbf{T}$ nếu $f\in \mathscr{L}^2(\mathbf{T})$.

## BÀI TẬP {#ts-ii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).

[^1]: L. Carleson, On convergence and growth of partial sums of Fourier series, Acta Mathematica 116 (1), 1966, p. 135–157.
