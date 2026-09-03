---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 4
section_title: Représentations des groupes compacts
lang: vi
source: ts-iii-v-fr
book_pages: TS V.456-TS V.482, TS V.504-TS V.516
pdf_pages: 0469-0495, 0517-0529
extraction: native
subsections:
    - "no": 1
      title: Semi-simplicité des représentations de dimension finie
      page: 456
      pdf_page: 469
    - "no": 2
      title: Représentations irréductibles
      page: 457
      pdf_page: 470
    - "no": 3
      title: Le théorème de Peter–Weyl
      page: 462
      pdf_page: 475
    - "no": 4
      title: Coefficients matriciels et fonctions G-finies
      page: 464
      pdf_page: 477
    - "no": 5
      title: Représentations dans un espace séparé quasi-complet
      page: 464
      pdf_page: 477
    - "no": 6
      title: Caractères et classes de conjugaison
      page: 466
      pdf_page: 479
    - "no": 7
      title: La cotransformation de Fourier
      page: 470
      pdf_page: 483
    - "no": 8
      title: La transformation de Fourier
      page: 471
      pdf_page: 484
    - "no": 9
      title: Indicateur de Frobenius–Schur et alternative de Larsen
      page: 476
      pdf_page: 489
statements: 54
exercises: 32
content_sha256: 48509c695cdce962381c70226114a4b324310928ddd38c24111f722e1723a076
translated_from: content/en-mt/ts/V/04_s4_representations_des_groupes_compacts.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 8b79212d5331d4bf78f506367fe72d2eeb57e31b3c25f268beebd4529fb3ad94
translation_model: gpt-5.4
translation_run: translate-vi-c279d198
glossary_version: 34
glossary_terms_sha256: a6ac4d758ef781a6a1973d72a772074802bf14fea332d157c3bed46d1ad36ec1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. BIỂU DIỄN CỦA CÁC NHÓM COMPACT

Trong đoạn này, mọi không gian vectơ tôpô được xét đều là phức, trừ khi nói tường minh điều ngược lại.

Cho G là một nhóm tôpô compact, mà phần tử đơn vị được ký hiệu bởi $e$. Nhóm G là đơn môđula (INT, VII, p. 20, § 1, n$^o3$, cor. of prop. 3). Ký hiệu $\mu$ là độ đo Haar chuẩn hóa trên G (nghĩa là sao cho $\mu(G) = 1$), và với $1\leqslant p\leqslant +\infty$, ký hiệu $\mathscr{L}^p(G)$ (tương ứng $L^p(G)$) là không gian $\mathscr{L}_{\mathbf{C}}^p(G, \mu)$ (tương ứng là không gian $L^p_{\mathbf{C}}(G, \mu)$). Các phép chập sẽ luôn được xét đối với độ đo $\mu$. Cho $p\in [1,+\infty ]$. Ta đồng nhất $\mathscr{C}(G)$ với một không gian con của $L^p$(G), điều này là được phép vì giá đỡ của $\mu$ bằng G.

Với mọi biểu diễn unita bất khả quy $\pi \in \widehat{G}$, ký hiệu $E_{\pi}$ là không gian của $\pi$.

### 1. Tính nửa đơn của các biểu diễn hữu hạn chiều

Ta nhắc lại (INT, VII, p. 71, § 3, n$^o1$, lemma 1) rằng với mọi biểu diễn liên tục $\varrho$ của G trong một không gian Hilbert E, tồn tại một dạng Hermit dương không suy biến $q$ trên E sao cho cấu trúc không gian vectơ tôpô của E được xác định bởi $q$ là đồng nhất với cấu trúc ban đầu của E, và sao cho $\varrho$ là một biểu diễn unita của G trong không gian Hilbert E được trang bị tích vô hướng $q$.

#### Mệnh đề 1 {#ts-v-s4-prop-1 .statement tag=03DN}

Cho $\varrho$ là một biểu diễn tuyến tính hữu hạn chiều của G trong một không gian vectơ tôpô tách được E. Tồn tại một tích vô hướng $q$ trên E sao cho $\varrho$ là một biểu diễn unita trong không gian Hilbert E được trang bị $q$. Đặc biệt, $\varrho$ là nửa đơn.

Vì E là hữu hạn chiều, tồn tại một cấu trúc không gian Hilbert trên E. Kết quả suy ra bằng cách áp dụng nhận xét đứng trước và hệ quả 2 của V, p. 392.

#### Nhận xét {#ts-v-s4-n1-rem-1 .statement tag=03DO}

Ta sẽ thấy sau này (hệ quả 4 của V, p. 466) rằng mọi biểu diễn unita của G đều là nửa đơn.

#### Hệ quả {#ts-v-s4-n1-cor-1 .statement tag=03DP}

Cho $\varrho_1$ và $\varrho_2$ là các biểu diễn hữu hạn chiều của G. Các biểu diễn $\varrho_1$ và $\varrho_2$ là đẳng cấu khi và chỉ khi các đặc trưng của chúng bằng nhau.

Điều này suy ra từ mệnh đề và hệ quả 3 của V, p. 392.

### 2. Các biểu diễn bất khả quy

#### Bổ đề 1 {#ts-v-s4-lem-1 .statement tag=03DQ}

Mọi biểu diễn unita bất khả quy của G đều khả tích bình phương.

Thật vậy, các hệ số ma trận của một biểu diễn unita bất khả quy là liên tục và bị chặn, do đó khả tích bình phương trên G, vì G là compact.

#### Mệnh đề 2 {#ts-v-s4-prop-2 .statement tag=03DR}

Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert E. Chiều của E là hữu hạn và bằng bậc hình thức của $\pi$.

Vì biểu diễn $\pi$ là khả tích bình phương (bổ đề 1), bậc hình thức $c_\mu(\pi )$ của nó đối với $\mu$ được xác định (định nghĩa 4 của V, p. 423); đó là một số thực dương ngặt. Cho $(e_i)_{i\in I}$ là một họ trực chuẩn hữu hạn trong E. Cho $x$ là một phần tử của E có chuẩn bằng 1 (có một phần tử như vậy vì E khác không). Với $i\in I$, ta có

$$
c_\mu(\pi )\int_G|\langle e_i|\pi (g)x\rangle |^2d\mu(g) = 1
$$

(prop. 8 of V, p. 424). Hãy lấy tổng công thức này theo $i\in I$. Ta được

Card(I) $=c_\mu(\pi )\int_G\sum_{i\in I}|\langle e_i|\pi (g)x\rangle |^2d\mu(g)$

$$
\leqslant c_\mu(\pi )\int_G\|\pi (g)x\|^2d\mu(g) =c_\mu(\pi )
$$

theo bất đẳng thức Bessel (EVT, V, p. 21, prop. 4). Do đó lực lượng của I bị chặn trên bởi $c_\mu(\pi )$. Điều này kéo theo chiều của E là hữu hạn.

Khi đó có thể áp dụng điều trên cho một cơ sở trực chuẩn $(e_i)_{i\in I}$ của E. Theo EVT, V, p. 22, prop. 5, ta được

dim(E) $=c_\mu(\pi )\int_G\sum_{i\in I}|\langle e_i|\pi (g)x\rangle |^2d\mu(g)$

$$
=c_\mu(\pi )\int_G\|\pi (g)x\|^2d\mu(g) =c_\mu(\pi )
$$

điều này hoàn tất chứng minh.

Đặc biệt, do đó được phép nói đến đặc trưng $\chi_{\pi}$ của một biểu diễn unita bất khả quy $\pi$ của G. Đó là một hàm liên tục trên G.

#### Hệ quả 1 {#ts-v-s4-prop-2-cor-1 .statement tag=03DS}

Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert E. Đặc trưng của $\pi$ là một phần tử Hermit của đại số có đối hợp $L^1(G)$.

Cho $x\in G$. Vì G là đơn môđula, ta có $\chi^*_{\pi}(x) =$ Tr($\pi (x^{-1})$), do đó $\chi^*_{\pi}(x) =$ Tr($\pi (x)$) vì $\pi$ là một biểu diễn unita.

#### Hệ quả 2 {#ts-v-s4-prop-2-cor-2 .statement tag=03DT}

a) Cho $\pi$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert E. Ta có

$\int'$ 1 $''$

$$
\langle x|\pi (g)x'\rangle  \langle y|\pi (g)y\rangle d\mu(g) =\langle x|y\rangle  \langle x|y\rangle
$$

$_G$ dim(E)

với mọi $(x, y, x', y')\in E^4$;

b) Cho $\pi_1($tương ứng $\pi_2)$ là một biểu diễn unita bất khả quy của G trong một không gian Hilbert $E_1($tương ứng $E_2)$. Nếu $\pi_1$ và $\pi_2$ không đẳng cấu, ta có

$$
\int_G\langle x|\pi_1(g)x'\rangle  \langle y|\pi_2(g)y'\rangle d\mu(g) = 0
$$

với mọi $(x, x', y, y')\in E^2_1\times E^2_2$.

Điều này suy ra ngay từ Mệnh đề 8 của V, p. 424 và Mệnh đề 9 của V, p. 424, có tính đến Bổ đề 1 và công thức $c_\mu(\pi ) =$ dim(E) (Mệnh đề 2).

#### Hệ quả 3 {#ts-v-s4-prop-2-cor-3 .statement tag=03DU}

Cho $\pi_1$ và $\pi_2$ là các biểu diễn bất khả quy của G. Trong không gian Hilbert $L^2(G)$, ta có $\langle \chi_{\pi_1}|\chi_{\pi_2}\rangle = 1$ nếu $\pi_1$ và $\pi_2$ đẳng cấu và $\langle \chi_{\pi_1}|\chi_{\pi_2}\rangle = 0$ nếu không. Nói cách khác, họ các đặc trưng của các lớp $\pi \in \widehat{G}$ là một họ trực chuẩn trong $L^2(G)$.

Điều này suy ra từ Mệnh đề 1 của V, p. 457 và Hệ quả 2, khi nhận thấy rằng với mọi cơ sở trực chuẩn $(e_i)_{i\in I}$ của không gian của một biểu diễn unita hữu hạn chiều $\pi$ của G, và với mọi $g\in G$, ta có công thức

$$
\chi_{\pi}(g) =\sum_{i\in I}\langle e_i|\pi (g)e_i\rangle
$$

#### Hệ quả 4 {#ts-v-s4-prop-2-cor-4 .statement tag=03DV}

a) Cho $\varrho$ là một biểu diễn liên tục hữu hạn chiều của G. Ta có

$\chi_{\varrho}=\sum_{\pi\in\widehat{G}}$ dim(Hom$_G(\pi , \varrho )$)$\chi_{\pi}=\sum_{\pi\in\widehat{G}}$ dim(Hom$_G(\varrho , \pi )$)$\chi_{\pi}$.

b) Cho $\varrho_1$ và $\varrho_2$ là các biểu diễn liên tục hữu hạn chiều của G. Ta có

$\langle \chi_{\varrho_1}|\chi_{\varrho_2}\rangle =$ dim(Hom$_G(\varrho_1, \varrho_2)$) $=$ dim(Hom$_G(\varrho_2, \varrho_1)$).

c) Một biểu diễn liên tục hữu hạn chiều $\varrho$ của G là bất khả quy khi và chỉ khi $\|\chi_{\varrho}\|^2= 1$.

Vì $\varrho$ là nửa đơn, nó đẳng cấu với tổng trực tiếp của các thành phần đẳng kiểu $\pi$ của nó $M_{\pi}(\varrho )$ với $\pi \in \widehat{G}$. Ký hiệu $m_{\pi}(\varrho )$ là bội số của $\pi$ trong $\varrho$ (Định nghĩa 10 của V, p. 398), khi đó ta có

$$
\chi_{\varrho}=\sum_{\pi\in\widehat{G}}m_{\pi}(\varrho )\chi_{\pi}
$$

Mệnh đề a) do đó suy ra từ sự kiện rằng

$m_{\pi}(\varrho ) =$ dim Hom$_G(\pi , \varrho ) =$ dim Hom$_G(\varrho , \pi )$

(công thức (1) của V, p. 377 và Hệ quả 2 của V, p. 387).

Bởi tính song tuyến tính và tính trực chuẩn của các đặc trưng, mệnh đề a) kéo theo rằng

$\langle \chi_{\varrho_1}|\chi_{\varrho_2}\rangle =\sum_{\pi\in\widehat{G}}$ dim(Hom$_G(\pi , \varrho_1)$) dim(Hom$_G(\pi , \varrho_2)$), và mặt khác ta có các đẳng cấu chính tắc

Hom$_G(\varrho_1, \varrho_2)\rightarrow \bigoplus_{(\pi_1,\pi_2)\in\widehat{G}\times\widehat{G}}$ Hom$_G(M_{\pi_1}(\varrho_1),M_{\pi_2}(\varrho_2))$

$\rightarrow \bigoplus_{\pi\in\widehat{G}}$ Hom$_G(M_{\pi}(\varrho_1),M_{\pi}(\varrho_2))$

(công thức (1) của V, p. 377), do đó suy ra rằng

dim(Hom$_G(\varrho_1, \varrho_2)$) $=\sum_{\pi\in\widehat{G}}m_{\pi}(\varrho_1)m_{\pi}(\varrho_2)$,

do đó mệnh đề b). Mệnh đề c) cũng suy ra từ a) và Bổ đề Schur (mệnh đề 6 của V, p. 386).

#### Hệ quả 5 {#ts-v-s4-prop-2-cor-5 .statement tag=03DW}

Cho $\pi_1$ và $\pi_2$ là các biểu diễn unita bất khả quy của G. Ta có $\pi_1(\overline{\chi}_{\pi_2}) = 0$ nếu $\pi_1$ không đẳng cấu với $\pi_2$, và $\pi_1(\overline{\chi}_{\pi_1})$ là phép nhân bởi $1/$ dim($\pi_1$).

Đặc trưng của $\pi_2$ là một hàm trung tâm liên tục trên G, do đó ánh xạ tuyến tính $u$ = $\pi_1(\overline{\chi}_{\pi_2})$ được xác định và thuộc không gian Hom$_G(\pi_1, \pi_1)$. Nó là một phép vị tự theo Bổ đề Schur (mệnh đề 6 của V, p. 386), với vết là

Tr($u$) $=$ Tr$(\int_G\overline{\chi_{\pi_2}(g)}\pi_1(g)d\mu(g))$

$$
=\int_G\overline{\chi_{\pi_2}(g)}\chi_{\pi_1}(g)d\mu(g)
$$

Theo các quan hệ trực giao, vết của $u$ vì thế bằng không nếu $\pi_1$ không đẳng cấu với $\pi_2$, và bằng 1 trong trường hợp ngược lại. Mệnh đề được suy ra.

#### Nhận xét {#ts-v-s4-n2-rem-1 .statement tag=03DX}

Khi G hữu hạn, quan hệ trực giao của Schur (tương ứng, công thức trực giao cho các đặc trưng) trùng với công thức ở A, VIII, p. 399 (tương ứng, công thức ở A, VIII, p. 400, mệnh đề 4). Mặt khác, “quan hệ trực giao thứ hai” đối với các đặc trưng của các nhóm hữu hạn (A, VIII, p. 402, công thức (32)) không có một tương tự khớp nào khi G compact.

Đối với G hữu hạn, trường hợp riêng của công thức trực giao thứ hai ứng với lớp liên hợp của $e$ là công thức

Card G1 $\sum_{\pi\in\widehat{G}}$ dim($\pi$ )$\chi_{\pi}(g) =$ 10 sisinon$g=,e$ cũng được diễn giải như phép tính đặc trưng của biểu diễn chính quy $\boldsymbol{\gamma }_G$ của G, và tương đương với công thức Tr($\boldsymbol{\gamma }_G(f)$) $=f(e)$ với mọi hàm $f$ từ G vào $\mathbf{C}$.

Bây giờ lại cho G là một nhóm compact bất kỳ. Với mọi hàm $f\in \mathscr{C}$(G), tự đồng cấu $\boldsymbol{\gamma }_G(f)$ của $L^2(G)$ trùng với tự đồng cấu $\varphi \mapsto f*\varphi$, và nó có vết hữu hạn (bổ đề 4 của V, p. 407 và hệ quả 2 của III, p. 33). Theo loc. cit. và Định lý 2 của IV, p. 177, ta cũng có

Tr($\boldsymbol{\gamma }_G(f)$) $=\int_Gf(x^{-1}x)d\mu(x) =f(e)$.

#### Mệnh đề 3 {#ts-v-s4-prop-3 .statement tag=03DY}

Giả sử rằng $G = G_1\times G_2$ trong đó $G_1$ và $G_2$ là các nhóm compact. Ánh xạ $b$ từ $\widehat{G}_1\times \widehat{G}_2$ vào $\widehat{G}$ mà với $(\pi_1, \pi_2)$ gán lớp của $\pi_1\boxtimes \pi_2$ là một song ánh.

Theo hệ quả 6 của V, p. 389, ánh xạ $b$ được xác định tốt.

Cho $\pi_1$ và $\pi_2$ là các phần tử của $\widehat{G}$. Cho $\pi \in \widehat{G}$. Thành phần đẳng kiểu theo $\pi$ của hạn chế $\varpi$ của $\pi_1\boxtimes \pi_2$ lên $G_1\times  \{e\}$ bằng $\varpi$ nếu $\pi_1=\pi$ và bằng không trong trường hợp ngược lại (bổ đề 8 của V, p. 384). Do đó, biểu diễn unita $\pi_1\boxtimes \pi_2$ xác định $\pi_1$ tới đẳng cấu; tương tự, nó xác định $\pi_2$, điều này chứng minh rằng $b$ là đơn ánh.

Ta hãy chứng minh rằng $b$ là toàn ánh. Cho $\pi$ là một biểu diễn unita bất khả quy của $G_1\times G_2$ trong một không gian Hilbert E. Nó là hữu hạn chiều (mệnh đề 2). Cho $\pi_1$ là một biểu diễn unita bất khả quy của $G_1$ trong một không gian Hilbert $E_1$ sao cho hạn chế của $\pi$ lên $G_1\times  \{e\}$ chứa một biểu diễn con đẳng cấu với $\pi_1$ (bổ đề 3 của V, p. 379). Đặt F = Hom$_{G_1}(\pi_1, \pi )$. Đó là một không gian vectơ hữu hạn chiều khác không. Với $h\in G_2$ và $u\in F$, gọi $\varrho (h)(u)$ là ánh xạ tuyến tính từ $E_1$ vào E được xác định bởi $x\mapsto \pi (e, h)(u(x))$. Vì $G_1\times  \{e\}$ và $\{e\} \times G_2$ giao hoán trong G, ánh xạ $\varrho (h)(u)$ thuộc không gian F. Ánh xạ $\varrho$ là một biểu diễn tuyến tính của $G_2$ trong không gian F; nó liên tục. Vì F không thu về 0, tồn tại một biểu diễn con bất khả quy $\pi_2$ của $\varrho$ (bổ đề 3 của V, p. 379). Gọi $E_2$ là không gian của $\pi_2$. Khi đó ánh xạ tuyến tính $v: E_1\otimes E_2\rightarrow E$ sao cho $x\otimes u\mapsto u(x)$ với $x\in E_1$ và $u\in E_2$ là một cấu xạ G khác không từ $\pi_1\boxtimes \pi_2$ vào $\pi$; vì các biểu diễn $\pi$ và $\pi_1\boxtimes \pi_2$ là bất khả quy và hữu hạn chiều, cấu xạ $v$ là một đẳng cấu (bổ đề 2 của V, p. 378).

Mệnh đề này cần được so sánh với định lý 1 của A, VIII, p. 208.

### 3. Định lý Peter–Weyl

Nhớ rằng Θ(G) kí hiệu không gian các hệ số ma trận của các biểu diễn unita hữu hạn chiều của G. Không gian Θ(G) là một đại số con có đơn vị của $\mathscr{C}(G)$ ổn định dưới phép liên hợp phức (mệnh đề 5 của V, p. 386).

Với $\pi \in \widehat{G}$, gọi $\boldsymbol{\varrho }_G(\pi )$ là không gian con của $\mathscr{C}(G)$ sinh bởi các hệ số ma trận của $\pi$. Ta đồng nhất nó với một không gian con của $L^2(G)$.

Không gian Θ(G) trùng với tổng của các không gian $\boldsymbol{\varrho }_G(\pi )$ với $\pi \in \widehat{G}$ (thật vậy, mọi phần tử của Θ(G) là một tổng các hệ số ma trận của các biểu diễn bất khả quy của G vì các biểu diễn hữu hạn chiều của G là nửa đơn theo mệnh đề 1 của V, p. 457). Hơn nữa, tổng này là trực tiếp vì, theo hệ quả 2 của V, p. 458, các không gian $\boldsymbol{\varrho }_G(\pi )$ trực giao từng đôi một.

#### Mệnh đề 4 {#ts-v-s4-prop-4 .statement tag=03DZ}

Không gian Θ(G) trù mật trong $\mathscr{C}(G)$ và trong $L^2(G)$.

Đại số con có đơn vị Θ(G) của $\mathscr{C}(G)$ ổn định dưới phép liên hợp. Nó trùng với đại số con Υ(G) theo mệnh đề 2 của V, p. 457, do đó nó phân biệt các điểm của G (hệ quả của định lý 4 của V, p. 454). Do đó, nó trù mật trong $\mathscr{C}(G)$ theo TG, X, p. 40, cor. 2, và, a fortiori, nó trù mật trong không gian $L^2(G) ($xem INT, IV, p. 155, §4, n$^o7$, mệnh đề 13).

Nhớ rằng biểu diễn biregular unita của G là biểu diễn $\boldsymbol{\varrho }_G$ của $G\times G$ trong $L^2(G)$ sao cho $(g_1, g_2)\mapsto \boldsymbol{\gamma }_G(g_1)\boldsymbol{\delta }_G(g_2)$.

#### Mệnh đề 5 {#ts-v-s4-prop-5 .statement tag=03E0}

Cho $\pi \in \widehat{G}$. Không gian $\boldsymbol{\varrho }_G(\pi )$ là một biểu diễn con của $\boldsymbol{\varrho }_G$ đẳng cấu với $\overline{\pi}\boxtimes \pi$. Đặc biệt, nó là một biểu diễn bất khả quy của $G\times G$.

Theo mệnh đề 7 của V, p. 422 (áp dụng với $Z =\{e\}$), không gian $\boldsymbol{\varrho }_G(\pi )$ là một biểu diễn con của $\boldsymbol{\varrho }_G$ và ánh xạ tuyến tính từ $\overline{E}_{\pi}\otimes E_{\pi}$ vào $L^2(G)$ gán cho $x\otimes y$ hệ số ma trận $g\mapsto  \langle x|\pi (g)y\rangle$ là một $(G\times$ G)-đẳng cấu của $\overline{\pi}\boxtimes \pi$ lên $\boldsymbol{\varrho }_G(\pi )$. Do đó biểu diễn con $\boldsymbol{\varrho }_G(\pi )$ là bất khả quy (mệnh đề 3 của V, p. 461).

#### Định lý 1 (Peter–Weyl) {#ts-v-s4-thm-1 .statement tag=03E1}

Cho G là một nhóm tôpô compact. Biểu diễn song chính quy $\boldsymbol{\varrho }_G$ của G là tổng Hilbert của các biểu diễn con $\boldsymbol{\varrho }_G(\pi )$ với $\pi \in \widehat{G}$.

Các không gian $\boldsymbol{\varrho }_G(\pi )$ trực giao từng đôi một; chúng là các biểu diễn con bất khả quy của biểu diễn song chính quy của G (mệnh đề 5) và đôi một không đẳng cấu (mệnh đề 3 của V, p. 461). Khi đó định lý suy ra từ tính chất rằng tổng Θ(G) của các không gian $\boldsymbol{\varrho }_G(\pi )$ khi $\pi$ chạy qua $\widehat{G}$ là trù mật trong $L^2(G)$ (mệnh đề 4).

#### Hệ quả 1 {#ts-v-s4-thm-1-cor-1 .statement tag=03E2}

Với mọi $\pi \in \widehat{G}$, biểu diễn con $\boldsymbol{\varrho }_G(\pi )$ là thành phần đẳng kiểu $(\overline{\pi}\boxtimes \pi )$ của $\boldsymbol{\varrho }_G$.

Cho F là thành phần đẳng kiểu $(\overline{\pi}\boxtimes \pi$) của $\boldsymbol{\varrho }_G$. Không gian F chứa $\boldsymbol{\varrho }_G(\pi )$ (mệnh đề 5). Hơn nữa, với mọi $\tau \in \widehat{G}$ khác $\pi$, giao của F và $\boldsymbol{\varrho }_G(\tau )$ bằng không (mệnh đề 3 của V, p. 461). Suy ra $F =\boldsymbol{\varrho }_G(\pi )$ do áp dụng định lý.

#### Hệ quả 2 {#ts-v-s4-thm-1-cor-2 .statement tag=03E3}

Cho $\pi_1$ và $\pi_2$ là các biểu diễn bất khả quy không đẳng cấu của G. Thành phần đẳng kiểu $(\overline{\pi}_1\boxtimes \pi_2)$ của $\boldsymbol{\varrho }_G$ bằng không.

#### Hệ quả 3 {#ts-v-s4-thm-1-cor-3 .statement tag=03E4}

Biểu diễn chính quy phải (tương ứng, trái) của G đẳng cấu với tổng Hilbert

$\pi \bigoplus\in \widehat{G}\pi$dim($\pi$ ).

Theo định lý và mệnh đề 5, hạn chế của biểu diễn song chính quy của G lên nhóm con $H =\{e\} \times G$ đẳng cấu với tổng Hilbert của các hạn chế lên H của các biểu diễn $\overline{\pi}\boxtimes \pi$ với $\pi \in \widehat{G}$. Các biểu diễn này đẳng cấu với tổng trực tiếp của dim($\pi$ ) bản sao của $\pi$ (bổ đề 8 của V, p. 384). Điều này kéo theo kết quả đối với biểu diễn chính quy phải, và trường hợp của biểu diễn chính quy trái là tương tự.

#### Hệ quả 4 {#ts-v-s4-thm-1-cor-4 .statement tag=03E5}

Cho $\pi \in \widehat{G}$. Thành phần đẳng kiểu $\pi$ của $\boldsymbol{\delta }_G$ (tương ứng, thành phần đẳng kiểu $\overline{\pi}$ của $\boldsymbol{\gamma }_G$) bằng $\boldsymbol{\varrho }_G(\pi )$.

Lập luận tương tự như của hệ quả trước, khi xem $\boldsymbol{\varrho }_G(\pi )$ như một biểu diễn con của $\boldsymbol{\delta }_G$ (tương ứng, của $\boldsymbol{\gamma }_G$).

#### Nhận xét 1 {#ts-v-s4-n3-rem-1 .statement tag=03E6}

Nếu G hữu hạn, các mệnh đề này tương ứng với các kết quả ở A, VIII, p. 398, nhận xét.

#### Nhận xét 2 {#ts-v-s4-n3-rem-2 .statement tag=03E7}

Giả sử rằng G giao hoán. Tập hợp $\widehat{G}$ được đồng nhất với nhóm đối ngẫu của G (V, p. 393, nhận xét). Với mọi $\chi \in \widehat{G}$, không gian của $\boldsymbol{\varrho }_G(\chi )$ là không gian con 1-chiều của $L^2(G)$ sinh bởi $\chi$. Do đó Định lý 1 cho G tương đương với hệ quả của định lý 1 của II, p. 215.

#### Nhận xét 3 {#ts-v-s4-n3-rem-3 .statement tag=03E8}

Nếu tồn tại một số nguyên $n\geqslant 0$ sao cho G là một nhóm con compact của $\mathbf{G}\mathbf{L}(\mathbf{C}^n)$, thì biểu diễn đồng nhất của G trong $\mathbf{G}\mathbf{L}(\mathbf{C}^n)$ đủ để tách các điểm của G, và do đó khi ấy có thể chứng minh trực tiếp mệnh đề 4, rồi sau đó định lý Peter–Weyl, mà không cần viện đến định lý Gelfand–Raikov.

#### Nhận xét 4 {#ts-v-s4-n3-rem-4 .statement tag=03E9}

Định lý Peter–Weyl đặc biệt kéo theo rằng đồng cấu liên tục tự nhiên từ G vào $\prod_{\pi\in\widehat{G}}\mathbf{U}(E_{\pi})$ là đơn ánh.

### 4. Các hệ số ma trận và các hàm G-hữu hạn

#### Mệnh đề 6 {#ts-v-s4-prop-6 .statement tag=03EA}

Các không gian con sau đây của $L^2(G)$ bằng nhau:

a) Không gian Θ(G) ;

b) Tổng đại số trực tiếp của các không gian con $\boldsymbol{\varrho }_G(\pi )$ của $L^2(G)$;

c) Không gian các vectơ G-hữu hạn (xem V, p. 376) của $\boldsymbol{\gamma }_G$;

d) Không gian các vectơ G-hữu hạn của $\boldsymbol{\delta }_G$;

e) Không gian các vectơ $(G\times G)$-hữu hạn của $\boldsymbol{\varrho }_G$.

Đặc biệt, mọi vectơ G-hữu hạn của $\boldsymbol{\gamma }_G,\boldsymbol{\delta }_G$ hoặc $\boldsymbol{\varrho }_G$ đều thuộc $\mathscr{C}(G)$.

Ký hiệu bởi $F_a$ (tương ứng $F_b, F_c, F_d, F_e$) không gian được xác định bởi điều kiện a) (tương ứng b), c), d), e)). Ta đã nhận thấy rằng $F_a= F_b$.

Ta có $F_b\subset F_c$ vì $\boldsymbol{\varrho }_G(\pi )$ là một biểu diễn con hữu hạn chiều của $\boldsymbol{\gamma }_G$ với mọi $\pi \in \widehat{G}$. Ngược lại, giả sử $f$ là một vectơ G-hữu hạn của $\boldsymbol{\gamma }_G$. Không gian con $E_f$ sinh bởi các hàm $\boldsymbol{\gamma }_G(g)f$ với $g\in G$ là một biểu diễn con hữu hạn chiều của $\boldsymbol{\gamma }_G$. Nó bằng tổng trực tiếp các thành phần đẳng kiểu của nó ứng với $\pi \in \widehat{G}$ (Mệnh đề 1 của V, p. 457). Theo Hệ quả 4 của V, p. 463, điều này kéo theo rằng $E_f$ được chứa trong tổng các không gian $\boldsymbol{\varrho }_G(\pi )$, do đó $F_c\subset F_b$.

Bằng lập luận tương tự, ta được $F_b= F_d$, và vì $\boldsymbol{\varrho }_G(\pi )$ là một biểu diễn con của $\boldsymbol{\varrho }_G$, ta cũng thiết lập theo cùng cách ấy rằng $F_b= F_e$.

#### Hệ quả {#ts-v-s4-n4-cor-1 .statement tag=03EB}

Cho $E\subset L^2(G)$ là một không gian con vectơ hữu hạn chiều xác định một biểu diễn con của $\boldsymbol{\gamma }_G($tương ứng của $\boldsymbol{\delta }_G$, của $\boldsymbol{\varrho }_G)$. Khi đó E được chứa trong $\mathscr{C}(G)$.

Thật vậy, mọi phần tử của E đều là một vectơ G-hữu hạn của biểu diễn $\boldsymbol{\gamma }_G$.

### 5. Biểu diễn trong một không gian tách được giả đầy đủ

#### Mệnh đề 7 {#ts-v-s4-prop-7 .statement tag=03EC}

Cho $\varrho$ là một biểu diễn liên tục của G trong một không gian lồi địa phương tách được giả đầy đủ E. Tổng của các biểu diễn con hữu hạn chiều của E là trù mật trong E.

Cho $x\in E$ và U là một lân cận mở của $x$. Tập hợp các độ đo $\nu \in \mathscr{M}(G)$ sao cho $\varrho (\nu )x\in U$ là mở trong $\mathscr{M}(G)$ đối với tôpô hội tụ compact (xem n$^o2$ của V, p. 400). Nó chứa $\varepsilon_e$, vì thế nó chứa một độ đo dạng $\nu =f_1\cdot \mu$ trong đó $f_1\in \mathscr{C}(G)$ (INT, VIII, p. 171, § 4, n$^o7$, Mệnh đề 19) và, do đó, nó chứa một độ đo dạng $f_2\cdot \mu$ trong đó $f_2$ là một hàm G-hữu hạn (Mệnh đề 6 của V, p. 464 và Mệnh đề 4 của V, p. 462).

Biểu diễn con F của $\boldsymbol{\gamma }_G$ sinh bởi $f_2$ là hữu hạn chiều. Gọi $\widetilde{F}$ là ảnh của ánh xạ tuyến tính $f\mapsto \varrho (f)x$ từ F vào E. Không gian $\widetilde{F}$ là hữu hạn chiều, và nó chứa phần tử $\varrho (f_2)x$ của U. Vì $\varrho (g)\varrho (f) =\varrho (\boldsymbol{\gamma }_G(g)f)$ với mọi $g\in G$ và mọi $f\in F$ (công thức (1) của V, p. 406), không gian $\widetilde{F}$ là một biểu diễn con của $\varrho$ giao với U. Mệnh đề được chứng minh.

#### Hệ quả 1 {#ts-v-s4-prop-7-cor-1 .statement tag=03ED}

Cho $\pi$ là một biểu diễn liên tục bất khả quy của G trong một không gian lồi địa phương tách được quasi-đầy đủ E. Không gian E là hữu hạn chiều.

#### Hệ quả 2 {#ts-v-s4-prop-7-cor-2 .statement tag=03EE}

Cho $\varrho$ là một biểu diễn liên tục của G trong một không gian lồi địa phương tách được quasi-đầy đủ E và cho $\pi$ là một biểu diễn liên tục bất khả quy của G.

a) Cấu xạ G $p_{\pi}=$ dim($\pi$ )$\varrho (\overline{\chi}_{\pi})$ từ E vào E là một phép chiếu liên tục của E mà ảnh là thành phần đẳng kiểu theo $\pi$ của $\varrho$;

b) Nếu $\varrho$ là một biểu diễn unita, thì phép chiếu $p_{\pi}$ là phép chiếu trực giao của E có ảnh là $M_{\pi}(\varrho )$.

Ta chứng minh a). Ánh xạ tuyến tính $p_{\pi}=$ dim($\pi$ )$\varrho (\overline{\chi}_{\pi})$ được xác định tốt, vì E là quasi-đầy đủ và G compắc (V, p. 401). Nó là một phần tử của Hom$_G(\varrho , \varrho )$ vì đặc trưng của $\pi$ là một hàm trung tâm liên tục trên G.

Cho $\varpi$ là một biểu diễn con hữu hạn chiều của E và F là không gian của nó. Ánh xạ $p_{\pi}$ cảm sinh, bằng cách chuyển qua các không gian con, tự đồng cấu (dim $\pi$ )$\varpi (\overline{\chi}_{\pi})$ của F. Vậy tự đồng cấu này bằng không nếu $\varpi$ không đẳng cấu với $\pi$, và là ánh xạ đồng nhất của F trong trường hợp ngược lại (thực vậy, điều này đúng nếu $\varpi$ là bất khả quy theo Hệ quả 5 của V, p. 460, và trường hợp tổng quát suy ra từ đó vì $\varpi$ là nửa đơn theo Mệnh đề 1 của V, p. 457).

Cuối cùng, vì tổng của các biểu diễn con hữu hạn chiều của E là trù mật trong E (Mệnh đề 7) và $p_{\pi}$ liên tục, suy ra $p_{\pi}$ là một phép chiếu mà ảnh là thành phần đẳng kiểu theo $\pi$ của $\varrho$. Nếu E là không gian Hilbert, phép chiếu $p_{\pi}$ là Hermit theo Hệ quả 1 của V, p. 458, do đó nó là một phép chiếu trực giao (Bổ đề 3, (ii) của I, p. 133).

#### Hệ quả 3 {#ts-v-s4-prop-7-cor-3 .statement tag=03EF}

Cho $\varrho$ là một biểu diễn liên tục của G trong một không gian lồi địa phương tách được quasi-đầy đủ E. Tự đồng cấu

$$
x\mapsto \int_G\varrho (g)x d\mu(g)
$$

của E là một phép chiếu của E mà ảnh là không gian $E^G$ các vectơ bất biến trong E. Đặc biệt, nếu E là hữu hạn chiều, thì

dim(E$^G$) $=\int_G\chi_{\varrho}(g)d\mu(g)$.

Khẳng định thứ nhất là trường hợp riêng của hệ quả trước khi $\pi$ là biểu diễn tầm thường chiều 1 của G. Khẳng định thứ hai suy ra từ đó vì chiều của $E^G$ là vết của phép chiếu trực giao lên $E^G$, nghĩa là,

dim(E$^G$) $=$ Tr$(\int_G\varrho (g)d\mu(g))=\int_G\chi_{\varrho}(g)d\mu(g)$.

Đặc biệt, khi E là hữu hạn chiều, tồn tại một vectơ $x\not = 0$ trong E sao cho $\varrho (g)x=x$ với mọi $g\in G$ khi và chỉ khi

$$
\int_G\chi_{\varrho}(g)d\mu(g)\not = 0
$$

#### Hệ quả 4 {#ts-v-s4-prop-7-cor-4 .statement tag=03EG}

Cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert E. Không gian E là tổng Hilbert của các thành phần đẳng kiểu theo $\pi$ $M_{\pi}(\varrho )$ với $\pi \in \widehat{G}$. Đặc biệt, biểu diễn $\varrho$ là nửa đơn.

Các thành phần đẳng kiểu của $\varrho$ tương ứng với các biểu diễn bất khả quy không đẳng cấu của G là trực giao (mệnh đề 8 của V, p. 394). Vì mọi biểu diễn unita hữu hạn chiều của G đều là nửa đơn (mệnh đề 1 của V, p. 457), tổng các thành phần đẳng kiểu $M_{\pi}(\varrho )$ với $\pi \in \widehat{G}$ là trù mật trong E (mệnh đề 7). Hệ quả được suy ra.

### 6. Các đặc trưng và các lớp liên hợp

Cho $\varrho$ là một biểu diễn unita của G trong một không gian Hilbert hữu hạn chiều E. Đặc trưng của $\varrho$ thỏa mãn $|\chi_{\varrho}|\leqslant$ dim(E). Cho $(e_i)_{i\in I}$ là một cơ sở trực chuẩn của E; đặc trưng $\chi_{\varrho}$ là tổng của các hệ số ma trận đường chéo $g\mapsto  \langle e_i|\varrho (g)e_i\rangle$ của $\varrho$. Đặc biệt, đặc trưng của $\varrho$ là một hàm G-hữu hạn, và nếu $\varrho$ là bất khả quy, thì $\chi_{\varrho}\in \boldsymbol{\varrho }_G(\varrho )$.

Ta có các công thức sau

$$
\chi_{\varrho_1\oplus\varrho_2}=\chi_{\varrho_1}+\chi_{\varrho_2},\chi_{\varrho_1\otimes\varrho_2}=\chi_{\varrho_1}\chi_{\varrho_2},\chi_{\breve{\varrho}}=\chi_{\overline{\varrho}}=\overline{\chi}_{\varrho}
$$

(xem A, VIII, p. 388–389).

#### Mệnh đề 8 {#ts-v-s4-prop-8 .statement tag=03EH}

Ta có

(1) $\chi_{\pi}*\chi_{\sigma}= 0$ với mọi $\pi , \sigma$ thuộc $\widehat{G}, \pi \not =\sigma$,

(2) $\chi_{\pi}*\chi_{\pi}=$ dim($1\pi$ )$\chi_{\pi}$ với mọi $\pi$ thuộc $\widehat{G}$.

Cho $\pi$ và $\sigma$ là các biểu diễn bất khả quy của G. Ta có

dim($\pi$ )$(\chi_{\pi}*\chi_{\sigma}) =$ dim($\pi$ )$\boldsymbol{\gamma }_G(\chi_{\pi})\chi_{\sigma}$

(bổ đề 4 của V, p. 407). Hàm dim($\pi$ )$\boldsymbol{\gamma }_G(\chi_{\pi})\chi_{\sigma}$ là phép chiếu trực giao của $\chi_{\sigma}$ lên thành phần đẳng kiểu $\overline{\pi}$ của $\boldsymbol{\gamma }_G$ (hệ quả 2 của V, p. 465), nghĩa là, lên $\boldsymbol{\varrho }_G(\pi )$ (hệ quả 4 của V, p. 463). Vì $\chi_{\sigma}$ thuộc $\boldsymbol{\varrho }_G(\sigma )$, kết quả được suy ra từ định lý 1 của V, p. 462.

#### Bổ đề 2 {#ts-v-s4-lem-2 .statement tag=03EI}

Đồ thị của quan hệ tương đương “ $x\in G$ và $y\in G$ và $x$ liên hợp với $y$ ” trong G là đóng.

Thật vậy, đồ thị này là ảnh của ánh xạ liên tục từ không gian compact $G\times G$ vào chính nó được xác định bởi $(x, y)\mapsto (x, yxy^{-1})$.

Ta ký hiệu bởi $G^{\sharp}$ không gian các lớp liên hợp của G được trang bị tôpô thương; đó là một không gian compact theo bổ đề 2 và TG, I, p. 78, mệnh đề 8. Cho $\varpi : G\rightarrow G^{\sharp}$ là phép chiếu chính tắc. Ánh xạ từ $\mathscr{C}(G^{\sharp})$ vào $\mathscr{C}(G)$ được xác định bởi $f\mapsto f\circ \varpi$ đồng nhất đại số có đối hợp $\mathscr{C}(G^{\sharp})$ với đại số con có đối hợp của $\mathscr{C}(G)$ tạo thành bởi các hàm trung tâm liên tục.

Các độ đo trên $G^{\sharp}$ được đồng nhất với các độ đo trung tâm trên G (V, p. 402, định nghĩa 1).

Dạng tuyến tính trên $\mathscr{C}(G^{\sharp})$ được xác định bởi $f\mapsto \int_Gf$ khi đó là một độ đo dương có khối lượng 1 trên $G^{\sharp}$, ký hiệu là $\mu^{\sharp}$. Với mọi $p\in [1,+\infty ]$, ta ký hiệu bởi $\mathscr{L}^p(G^{\sharp})$ (tương ứng $L^p(G^{\sharp})$) không gian $\mathscr{L}_{\mathbf{C}}^p(G^{\sharp}, \mu^{\sharp})$ (tương ứng $L^p_{\mathbf{C}}(G^{\sharp}, \mu^{\sharp})$). Ta đồng nhất $L^p(G^{\sharp})$ với bao đóng của $\mathscr{C}(G^{\sharp})$ trong $L^p(G)$; đặc biệt, đó là một không gian con đóng của $L^p(G)$.

Ta cũng ký hiệu bởi $\Theta (G^{\sharp}) = \Theta (G)\cap \mathscr{C}(G^{\sharp})$ không gian các hệ số ma trận trung tâm của G. Đó là một đại số con có đơn vị và có đối hợp của $\mathscr{C}(G^{\sharp})$.

Khi G là một nhóm Lie, không gian $\Theta (G^{\sharp})$ cũng được ký hiệu là ZΘ(G) trong LIE, IX, p. 71.

#### Bổ đề 3 {#ts-v-s4-lem-3 .statement tag=03EJ}

Cho $\pi$ là một biểu diễn unita bất khả quy của G. Không gian vectơ $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$ có chiều bằng một và được sinh bởi đặc trưng của $\pi$.

Xét biểu diễn unita $\sigma$ của G trong không gian $\boldsymbol{\varrho }_G(\pi )$ được xác định bởi $\sigma (g) =\boldsymbol{\varrho }_G(g, g)$. Vì biểu diễn unita $\boldsymbol{\varrho }_G(\pi )$ của $G\times G$ đẳng cấu với $\overline{\pi}\boxtimes \pi$ (mệnh đề 5 của V, p. 462), nên đặc trưng của nó được cho bởi

$$
\chi_{\sigma}(g) =\chi_{\overline{\pi}\boxtimes\pi}(g, g) =|\chi_{\pi}(g)|^2
$$

với mọi $g\in G$. Không gian $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$ là không gian con của các phần tử bất biến dưới biểu diễn này, và chiều của nó bằng

$$
\int_G\chi_{\sigma}(g)d\mu(g) =\int_G|\chi_{\pi}(g)|^2d\mu(g) = 1
$$

(hệ quả 3 của V, p. 466 và hệ quả 3 của V, p. 459). Vì đặc trưng của $\pi$ là một phần tử khác không của $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$, nên nó là một cơ sở của không gian này.

#### Mệnh đề 9 {#ts-v-s4-prop-9 .statement tag=03EK}

Họ $(\chi_{\pi})_{\pi\in\widehat{G}}$ các đặc trưng của các biểu diễn unita bất khả quy của G là một cơ sở trực chuẩn của $L^2(G^{\sharp})$.

Theo định lý Peter-Weyl (định lý 1 của V, p. 462), không gian con đóng $L^2(G^{\sharp})$ của $L^2(G)$ tạo bởi các phần tử bất biến dưới biểu diễn unita $g\mapsto \boldsymbol{\varrho }_G(g, g)$ của G là tổng Hilbert của các không gian con $L^2(G^{\sharp})\cap \boldsymbol{\varrho }_G(\pi )$ với $\pi \in \widehat{G}$. Do đó mệnh đề suy ra từ bổ đề trước và hệ quả 3 của V, p. 459.

#### Hệ quả 1 {#ts-v-s4-prop-9-cor-1 .statement tag=03EL}

Không gian vectơ $\Theta (G^{\sharp})$ trù mật trong $\mathscr{C}(G^{\sharp})$ và trong $L^2(G^{\sharp})$.

Mệnh đề thứ hai suy ra từ mệnh đề 9. Đối với mệnh đề thứ nhất, xét biểu diễn tuyến tính $\varrho$ của G trên không gian Banach $\mathscr{C}(G)$ được xác định bởi

$$
\varrho (g)f(x) =f(g^{-1}xg)
$$

với mọi $f\in \mathscr{C}(G)$ và mọi $x\in G$. Đó là một biểu diễn liên tục đẳng cự, và $\mathscr{C}(G^{\sharp})$ là không gian các phần tử bất biến dưới biểu diễn này. Do đó phép chiếu liên tục $p=\varrho (1)$ của $\mathscr{C}(G)$ có ảnh là $\mathscr{C}(G^{\sharp})$ (hệ quả 3 của V, p. 466); nó có chuẩn $\leqslant 1$.

Cho $f\in \mathscr{C}(G^{\sharp})$ và cho $\varepsilon  >0$. Tồn tại $\widetilde{f}\in \Theta (G)$ sao cho $\|f-\widetilde{f}\|\leqslant \varepsilon$ (mệnh đề 4 của V, p. 462), và khi đó $\|f-p(\widetilde{f})\|=\|p(f-\widetilde{f})\|\leqslant \varepsilon$; vì $p(\widetilde{f})\in \mathscr{C}(G^{\sharp})$, ta kết luận rằng $\Theta (G^{\sharp})$ trù mật trong $\mathscr{C}(G^{\sharp})$.

Kí hiệu $R(G)$ là vành Grothendieck của các biểu diễn liên tục của $G$ trong các không gian vectơ phức tách biệt hữu hạn chiều (x. LIE, IX, p. 70 và A, VIII, p. 182, áp dụng cho lớp cộng tính của các biểu diễn liên tục của $G$ trong các không gian vectơ phức tách biệt hữu hạn chiều, được xem như các $\mathbf{C}$[G]-môđun). Vì mọi biểu diễn tuyến tính liên tục của $G$ trong một không gian vectơ tôpô tách biệt hữu hạn chiều đều là nửa đơn (mệnh đề 1 của V, p. 457), nhóm Abel $R(G)$ là tự do và các lớp của các biểu diễn unita bất khả quy $\pi \in \widehat{G}$ lập thành một cơ sở của nó (A, VIII, p. 186, mệnh đề 7).

#### Hệ quả 2 {#ts-v-s4-prop-9-cor-2 .statement tag=03EM}

a) Họ các đặc trưng của các biểu diễn bất khả quy của $G$ là một cơ sở của $\Theta (G^{\sharp})$;

b) Ánh xạ $u: R(G)\otimes_{\mathbf{Z}}\mathbf{C}\rightarrow \Theta (G^{\sharp})$ sao cho $u(\pi \otimes 1) =\chi_{\pi}$ với mọi $\pi \in \widehat{G}$ là một đẳng cấu các đại số trên $\mathbf{C}$.

Mệnh đề thứ nhất suy ra từ Mệnh đề 9 và Hệ quả 1.

Vì các lớp của các biểu diễn $\pi \in \widehat{G}$ lập thành một cơ sở của $\mathbf{Z}$-môđun tự do $R(G)$, ánh xạ $u$ được xác định tốt. Nó là một cấu xạ các $\mathbf{C}$-đại số, và là một đẳng cấu theo a).

#### Hệ quả 3 {#ts-v-s4-prop-9-cor-3 .statement tag=03EN}

Cho $H$ là một nhóm tôpô địa phương compact sao cho $G$ là một nhóm con compact của $H$. Cho $\varrho$ là một biểu diễn unita của $H$ trong một không gian Hilbert $E$. Nếu thành phần đẳng kiểu theo $\pi$ của hạn chế của $\varrho$ xuống $G$ là hữu hạn chiều với mọi $\pi \in \widehat{G}$, thì biểu diễn $\varrho$ của $H$ là nửa đơn và mọi biểu diễn unita bất khả quy của $H$ đều xuất hiện với bội số hữu hạn trong $\varrho$.

Kí hiệu $\sigma$ là hạn chế của $\varrho$ xuống nhóm con compact $G$ của $H$. Cho $\pi$ là một biểu diễn bất khả quy của $G$. Tự đồng cấu $\sigma (\chi_{\pi})\in \mathscr{L}(E)$ có hạng hữu hạn, vì ảnh của nó là thành phần đẳng kiểu theo $\overline{\pi}$ của $\sigma$ (hệ quả 2 của V, p. 465) và thành phần này là hữu hạn chiều theo giả thiết. Do đó, tự đồng cấu $\sigma (f)$ có hạng hữu hạn với mọi $f\in \Theta (G^{\sharp})$ và là compact với mọi $f\in \mathscr{C}(G^{\sharp})$ (hệ quả 1 của V, p. 468 và hệ quả của mệnh đề 2 của III, p. 4).

Gọi $j$ là đơn ánh chính tắc của $G$ vào $H$. Nó là một ánh xạ liên tục mà là $\nu$-thực sự đối với mọi độ đo $\nu$ trên $G$ (INT, V, p. 69, § 6, No.$^o1$, Nhận xét 1). Gọi $\mathfrak{B}$ là bộ lọc các lân cận compắc của phần tử $e$ trong $G$. Với mọi $V\in \mathfrak{B}$, tồn tại một hàm trung tâm liên tục dương $f_V$ trên $G$ có giá được chứa trong $V$ mà tích phân trên $G$ bằng $1$. Gọi $\beta_V$ là độ đo ảnh $j(f_V\cdot \mu)$; đó là một độ đo dương có giá compắc trên $H$ sao cho $\varrho (\beta_V) =\sigma (f_V)$ (INT, V, p. 71, § 6, No.$^o2$, Định lý 1). Từ những điều nói trên, cơ sở bộ lọc trên $\mathscr{M}_c(H)$ là ảnh của $\mathfrak{B}$ dưới ánh xạ $V\mapsto \beta_V$ thỏa mãn các điều kiện của Mệnh đề 2 ở V, p. 402, và mệnh đề được suy ra.

Hệ quả 4 (tiêu chuẩn Weyl về phân bố đều)

Cho $M$ là một tập hợp các độ đo trung tâm dương trên $G$ sao cho $\nu (G) = 1$ với mọi $\nu \in M$. Cho $\mathfrak{F}$ là một bộ lọc trên $M$. Điều kiện cần và đủ để bộ lọc $\mathfrak{F}$ hội tụ mơ hồ tới độ đo $\mu^{\sharp}$ trên $G^{\sharp}$ là, với mọi biểu diễn unita bất khả quy không tầm thường $\pi$, ta có

lim$_{\nu ,\mathfrak{F}}\int_G\chi_{\pi}(x)d\nu (x) = 0$.

Vì $\nu (G^{\sharp}) = 1 =\mu^{\sharp}(G^{\sharp})$ với $\nu \in M$, giả thiết có nghĩa là

lim$_{\nu ,\mathfrak{F}}\int_{G^{\sharp}}\chi_{\pi}(x)d\nu (x) =\int_{G^{\sharp}}\chi_{\pi}(x)d\mu^{\sharp}(x)$

với mọi biểu diễn $\pi \in \widehat{G}$, do đó nó tương đương với điều kiện

lim$_{\nu ,\mathfrak{F}}\int_{G^{\sharp}}f(x)d\nu (x) =\int_{G^{\sharp}}f(x)d\mu^{\sharp}(x)$

với mọi hàm $f\in \Theta (G^{\sharp})$ theo tính tuyến tính. Vì không gian $\Theta (G^{\sharp})$ là trù mật trong $\mathscr{C}(G^{\sharp})$ (Hệ quả 1), nên giả thiết do đó tương đương với sự hội tụ của bộ lọc $\mathfrak{F}$ tới $\mu^{\sharp}$ trong $\mathscr{M}(G^{\sharp})$ được trang bị tôpô hội tụ đơn giản trong $\mathscr{C}$ (G), tôpô này trùng với tôpô hội tụ mơ hồ vì G compắc (x. INT, III, p. 59, § 1, No.$^o9$).

### 7. Đối biến đổi Fourier

Tập hợp $\widehat{G}$ được trang bị tôpô rời rạc. Ta ký hiệu bởi $F(\widehat{G})$ đại số tích của các End(E$_{\pi}$) với $\pi$ thuộc $\widehat{G}$ và bởi $F_b(\widehat{G})$ đại số tích-$*$ của các End(E$_{\pi}$) (Ví dụ 5 của I, p. 103); đó là tập hợp các họ $(u_{\pi})_{\pi\in\widehat{G}}$ sao cho sup$_{\pi\in\widehat{G}}\|u_{\pi}\|<+\infty$.

Ta ký hiệu bởi $F_0(\widehat{G})$ đại số con $*$ đóng của $F_b(\widehat{G})$ được tạo bởi các họ $(u_{\pi})_{\pi\in\widehat{G}}$ sao cho $\|u_{\pi}\|$ tiến tới 0 ở vô cùng.

Cho $\nu \in \mathscr{M}^1(G)$. Với mọi $\pi \in \widehat{G}$, ta có $\|\pi (\nu )\|\leqslant \|\nu \|$, do đó họ $(\pi (\nu ))_{\pi\in\widehat{G}}$ thuộc $F_b(\widehat{G})$.

#### Định nghĩa 1 {#ts-v-s4-def-1 .statement tag=03EO}

Với mọi độ đo $\nu \in \mathscr{M}^1(G)$, phần tử $(\pi (\nu ))_{\pi\in\widehat{G}}$ của $F_b(\widehat{G})$ được ký hiệu là $\mathscr{F}_G(\nu )$. Ánh xạ từ $\mathscr{M}^1(G)$ vào $F_b(\widehat{G})$ được xác định như vậy được gọi là đối biến đổi Fourier của G, và $\overline{\mathscr{F}}_G(\nu )$ được gọi là đối biến đổi Fourier của độ đo $\nu$.

Với $f\in L^1$(G), ta sẽ viết $\overline{\mathscr{F}}_G(f) =\overline{\mathscr{F}}_G(f\cdot \mu)$.

Với mọi biểu diễn $\pi \in \widehat{G}$, ánh xạ $\nu \mapsto \pi (\nu )$ là một cấu xạ có đơn vị của các đại số Banach có đối hợp từ $\mathscr{M}^1(G)$ vào End(E$_{\pi}$) (Bổ đề 1 của V, p. 401). Do đó, đối biến đổi Fourier là một cấu xạ có đơn vị của các đại số Banach có đối hợp từ $\mathscr{M}^1(G)$ vào $F_b(\widehat{G})$.

### 8. Biến đổi Fourier

Ta giữ lại ký hiệu của số trước.

Cho $\pi \in \widehat{G}$. Ta trang bị không gian vectơ End(E$_{\pi}$) cấu trúc của một không gian Hilbert mà tích vô hướng được cho bởi

$\langle u_1|u_2\rangle =$ dim($\pi$)Tr($u^*_1u_2$) $=$ dim($\pi$)Tr($u_2u^*_1$)

đối với $u_1,u_2$ trong End(E$_{\pi}$) $($x. EVT, V, p. 52, Định lý 1).

Ta ký hiệu bởi $\|u\|_2$ = $\surd\overline{\langle u|u\rangle}$ chuẩn của một phần tử $u$ của End(E$_{\pi}$) với $\pi \in \widehat{G}$. Với mọi $g\in G$, ta có $\|\pi (g)\|_2=$ dim($\pi$ ) vì $\pi (g)$ là đơn nhất.

Chuẩn ở đây được ký hiệu bởi $\|u\|_2$ sai khác với chuẩn được định nghĩa trong EVT, V, p. 52 trên không gian các ánh xạ Hilbert-Schmidt của $E_{\pi}$ bởi một nhân tử dim($\pi$ ).

#### Bổ đề 4 {#ts-v-s4-lem-4 .statement tag=03EP}

Cho $\pi$ là một biểu diễn bất khả quy của G. Ánh xạ $f\mapsto \pi (f)$ xác định, bằng cách chuyển qua các không gian con, một đẳng cấu đẳng cự của $\boldsymbol{\varrho }_G(\overline{\pi})$ vào End(E$_{\pi}$).

Đặt $\varepsilon_{\pi}(g, h)u=\pi (g)\circ u\circ \pi (h^{-1})$ với mọi $(g, h)\in G\times G$ và với mọi $u\in$ End(E$_{\pi}$). Ánh xạ $\varepsilon_{\pi}$ là một biểu diễn liên tục của $G\times G$ trong End(E$_{\pi}$). Nó là unita. Thật vậy, vì bản thân $\pi$ là unita, ta được

$\|\varepsilon_{\pi}(g, h)u\|^2_2=$ dim($\pi$ ) Tr$((\pi (g)u\pi (h^{-1}))^*\pi (g)u\pi (h^{-1}))$

= dim($\pi$ ) Tr($\pi (h)u^*u\pi (h)^{-1}$) $=$ dim($\pi$ ) Tr($u^*u$) $=\|u\|^2_2$ với mọi $(g, h)\in G\times G$ và mọi $u\in$ End(E$_{\pi}$).

Ánh xạ Ψ được xác định bởi $f\mapsto \pi (f)$ là một $(G\times$ G)-cấu xạ từ $\boldsymbol{\varrho }_G(\overline{\pi})$ vào End(E$_{\pi}$), vì

$$
\pi (\boldsymbol{\varrho }_G(g, h)f) =\int_Gf(g^{-1}xh)\pi (x)d\mu(x) =\pi (g)\pi (f)\pi (h^{-1})
$$

với mọi $(g, h)\in G\times G$ và mọi $f\in \boldsymbol{\varrho }_G(\overline{\pi})$. Vì $\boldsymbol{\varrho }_G(\overline{\pi})$ là một biểu diễn bất khả quy (đl. 1, a) của V, p. 462), nên tồn tại $\lambda \in \mathbf{C}^*$ sao cho ánh xạ $\lambda \Psi$ bằng không hoặc đẳng cự (hệ quả 5, a) của V, p. 388).

Đặt $f=$ dim($\pi$ )$\overline{\chi}_{\pi}\in \boldsymbol{\varrho }_G(\overline{\pi})$. Khi đó $\pi (f) = 1_{E_{\pi}}$ (hệ quả 2 của V, p. 465), do đó $\|\pi (f)\|_2=$ dim($\pi$ ) $=\|f\|$ (hệ quả 3 của V, p. 459). Do đó, ánh xạ Ψ là đẳng cự. Vì $\boldsymbol{\varrho }_G(\overline{\pi})$ và End(E$_{\pi}$) có cùng chiều, Ψ là một đẳng cấu đẳng cự.

Ta ký hiệu bởi $F^2(\widehat{G})$ tổng Hilbert của các không gian Hilbert End(E$_{\pi}$). Chuẩn của một phần tử $x\in F^2(\widehat{G})$ lại được ký hiệu bởi $\|x\|_2$.

Trong LIE, IX, p. 79, không gian này được ký hiệu là $L^2(\widehat{G})$, một ký hiệu mà ở đây chúng tôi muốn tránh dùng để không gây nhầm lẫn với không gian $\ell^2(\widehat{G})$.

Cho $(u_{\pi})$ là một phần tử của $F^2(\widehat{G})$. Vì

$^{\pi\in\widehat{G}}\sum_{\pi\in\widehat{G}}\|u_{\pi}\|^2_2=\sum_{\pi\in\widehat{G}}$ dim($\pi$ ) Tr($u^*_{\pi}u_{\pi}$)$<+\infty$

và $\|u_{\pi}\|^2\leqslant$ Tr($u^*_{\pi}u_{\pi}$) $($xem EVT, V, p. 52, công thức (33)), chuẩn trong $\mathscr{L}(E_{\pi})$ của tự đồng cấu $u_{\pi}$ tiến tới 0 ở vô cực. Do đó có thể đồng nhất $F^2(\widehat{G})$ với một không gian con của $F_0(\widehat{G})$.

Cho $\pi \in \widehat{G}$ và $u\in$ End(E$_{\pi}$). Ta ký hiệu bởi $\mathscr{F}_{\pi}(u)$ hàm trên G được xác định bởi $\mathscr{F}_{\pi}(u)(g) =\langle \pi (g)|u\rangle =$ dim($\pi$)Tr($\pi (g)^*u$) với mọi $g\in G$. Đây là một hàm liên tục trên G. Nếu G là một nhóm Lie thực compact, thì hàm $\mathscr{F}_{\pi}(u)$ là giải tích trên G (LIE, III, § 8, n$^o1$, định lý 1).

Vì G compact, có thể đồng nhất $L^2(G)$ với một không gian con của $L^1(G)$.

#### Định lý 2 {#ts-v-s4-thm-2 .statement tag=03EQ}

Đối biến đổi Fourier của G cảm sinh, khi chuyển qua các không gian con, một đẳng cấu đẳng cự từ $L^2(G)$ lên $F^2(\widehat{G})$. Nghịch đảo của nó $\mathscr{F}_G$ gắn với một phần tử $(u_{\pi})_{\pi\in\widehat{G}}$ của $F^2(\widehat{G})$ tổng của chuỗi

$$
\sum_{\pi\in\widehat{G}}\mathscr{F}_{\pi}(u_{\pi})
$$

hội tụ trong $L^2(G)$.

Theo định lý Peter-Weyl (định lý 1 của V, p. 462), không gian Hilbert $L^2(G)$ là tổng Hilbert của các không gian $\boldsymbol{\varrho }_G(\overline{\pi})$ với $\pi \in \widehat{G}$. Với mọi $\pi \in \widehat{G}$, ánh xạ tuyến tính $f\mapsto \pi (f)$ từ $\boldsymbol{\varrho }_G(\overline{\pi})$ vào End(E$_{\pi}$) là một đẳng cấu đẳng cự (bổ đề 4). Do đó, hạn chế của đối biến đổi Fourier lên $L^2(G)$ xác định một đẳng cấu đẳng cự từ $L^2(G)$ lên $F^2(\widehat{G})$.

Cho $f\in L^2(G)$. Cho $\pi \in \widehat{G}$, và gọi $f_{\overline{\pi}}\in \mathscr{C}(G)$ là phép chiếu trực giao của $f$ lên $\boldsymbol{\varrho }_G(\overline{\pi})$ (định lý 1 của V, p. 462). Vì không gian này là thành phần đẳng kiểu $\overline{\pi}$ của $\boldsymbol{\delta }_G$ (hệ quả 4 của V, p. 463), ta có $f_{\overline{\pi}}=$ dim($\pi$ )$\boldsymbol{\delta }_G(\chi_{\pi})(f)$ theo hệ quả 2 của V, p. 465. Với mọi $x\in G$, điều này cho

$f_{\overline{\pi}}(x) =$ dim($\pi$ )$\int_G\chi_{\pi}(g)(\boldsymbol{\delta }_G(g)f)(x)d\mu(g)$

= dim($\pi$ )$\int_G\chi_{\pi}(g)f(xg)d\mu(g)$

= dim($\pi$ )$\int_G\chi_{\pi}(x^{-1}y)f(y)d\mu(y)$

= dim($\pi$)Tr($\pi (x^{-1})\pi (f)$) $=\langle \pi (x)|\pi (f)\rangle$,

nghĩa là $f_{\overline{\pi}}=\mathscr{F}_{\pi}(\pi (f))$.

Vì $f$ là tổng trong $L^2(G)$ của họ $(f_{\overline{\pi}})$ theo định lý Peter–Weyl, ta thu được

$$
f=\sum_{\pi\in\widehat{G}}\mathscr{F}_{\pi}(\pi (f))
$$

trong đó chuỗi hội tụ trong $L^2(G)$. Điều này chứng minh định lý.

#### Định nghĩa 2 {#ts-v-s4-def-2 .statement tag=03ER}

Đẳng cấu đẳng cự $\mathscr{F}_G$ từ $F^2(\widehat{G})$ lên $L^2(G)$, nghịch đảo của đẳng cấu cảm sinh bởi đối biến đổi Fourier, được gọi là biến đổi Fourier của G. Ảnh của một phần tử của $F^2(\widehat{G})$ được gọi là biến đổi Fourier của nó.

#### Nhận xét 1 {#ts-v-s4-n8-rem-1 .statement tag=03ES}

Biến đổi Fourier của $(u_{\pi})_{\pi\in\widehat{G}}\in F^2(\widehat{G})$ do đó là lớp trong $L^2(G)$ của chuỗi

$g\mapsto \sum_{\pi\in\widehat{G}}\langle \pi (g)|u_{\pi}\rangle =\sum_{\pi\in\widehat{G}}$ dim($\pi$)Tr($u_{\pi}\circ \pi (g)^{-1}$).

#### Nhận xét 2 {#ts-v-s4-n8-rem-2 .statement tag=03ET}

Cho $f\in L^2(G)$. Khi đó ta có công thức Plancherel

$$
\|f\|^2=\|\overline{\mathscr{F}}_G(f)\|^2=\sum_{\pi\in\widehat{G}}\|\pi (f)\|^2
$$

Hơn nữa, theo Định lý 2$,f$ là tổng trong $L^2(G)$ của họ $(f_{\pi})_{\pi\in\widehat{G}}$ trong đó

$$
f_{\pi}(x) =\mathscr{F}_{\pi}(\pi (f))(x)
$$

$=\langle \pi (x)|\pi (f)\rangle =$ dim($\pi$ )$\int_Gf(g)\chi_{\pi}(x^{-1}g)d\mu(g)$

với mọi $x\in G$ và mọi $\pi \in \widehat{G}$.

Giả sử rằng G là giao hoán. Vì các biểu diễn bất khả quy của G đều có chiều bằng 1 (hệ quả 7 của V, p. 390) và nhóm đối ngẫu $\widehat{G}$ là rời rạc (mệnh đề 18 của II, p. 233), các đại số $F_b(\widehat{G})$ và $F_0(\widehat{G})$ lần lượt được đồng nhất với đại số $\mathscr{C}_b(\widehat{G})$ của các hàm liên tục bị chặn trên $\widehat{G}$ và đại số $\mathscr{C}_0(\widehat{G})$ của các hàm liên tục tiến tới 0 ở vô cùng trên $\widehat{G}$. Vì G compact, độ đo Haar trên $\widehat{G}$ đối ngẫu với $\mu$ là độ đo đếm $\widehat{\mu}$ (mệnh đề 18 của II, p. 233). Tổng Hilbert $F^2(\widehat{G})$ của các không gian End(E$_{\pi}$) với $\pi \in \widehat{G}$ được đồng nhất với không gian Hilbert $L^2(\widehat{G},\widehat{\mu})$.

Cho $\nu \in \mathscr{M}^1(G)$. Khi đó, với mọi đặc trưng unita $\chi \in \widehat{G}$, ta có

$$
\chi (\nu ) =\int_G\chi  \nu
$$

điều này chứng minh rằng đối biến đổi Fourier được định nghĩa ở trên trùng với đối biến đổi Fourier của G được định nghĩa trong II, p. 206.

Mọi $f\in \mathscr{L}^2(G)$ đều khả tích và công thức $\|\overline{\mathscr{F}}_G(f)\|_2=\|f\|$ là công thức Plancherel (II, p. 215, Định lý 1).

#### Mệnh đề 10 {#ts-v-s4-prop-10 .statement tag=03EU}

Đối biến đổi Fourier là một cấu xạ đơn ánh của các đại số Banach có phép đối hợp của $\mathscr{M}^1(G)$ vào $F_b(\widehat{G})$ và ánh xạ $L^1(G)$ vào $F_0(\widehat{G})$.

Vì G compact, không gian $\mathscr{C}(G)$ được chứa trong và trù mật trong $\mathscr{L}^1(G)$ và $\mathscr{L}^2(G)$.

Cho $\nu \in \mathscr{M}^1(G)$ sao cho $\overline{\mathscr{F}}_G(\nu ) = 0$. Khi đó với mọi hàm liên tục $f$ trên G, ta có $\overline{\mathscr{F}}_G(\nu *f) = 0$. Bây giờ $\nu *f$ thuộc $\mathscr{C}(G)$ (INT, VIII, p. 152, § 4, No.$^o2$, mệnh đề 3). Vì, theo Định lý 2, đối biến đổi Fourier là đơn ánh trên $L^2$(G), và a fortiori trên không gian $\mathscr{C}$ (G), ta có $\nu *f= 0$ với $f\in \mathscr{C}(G)$. Đặc biệt, suy ra rằng

$$
\int_Gf(x)d\nu (x) = (\nu *\check{f})(e) = 0
$$

với mọi hàm $f\in \mathscr{C}(G)$ (INT, VIII, loc. cit.), do đó độ đo $\nu$ bằng không.

Ảnh của $\mathscr{C}(G)$ dưới phản biến đổi Fourier được chứa trong $F^2(\widehat{G})$, và a fortiori trong $F_0(\widehat{G})$. Vì $F_0(\widehat{G})$ đóng trong $F_b(\widehat{G})$ và $\mathscr{C}(G)$ trù mật trong $L^1$(G), ảnh của $L^1(G)$ dưới phản biến đổi Fourier cũng được chứa trong $F_0(\widehat{G})$.

#### Mệnh đề 11 {#ts-v-s4-prop-11 .statement tag=03EV}

a) Cho $u= (u_{\pi})_{\pi\in\widehat{G}}$ là một phần tử của $F(\widehat{G})$. Nếu họ $(\mathscr{F}_{\pi}(u_{\pi}))_{\pi\in\widehat{G}}$ là tổng được đều trong $\mathscr{C}(G)$, thì tổng của nó $f$ là một hàm liên tục trên G mà phản biến đổi Fourier là $u$;

b) Cho $f\in L^1(G)$. Nếu họ $(\mathscr{F}_{\pi}(\pi (f)))_{\pi\in G}$ là tổng được đều trong $\mathscr{C}(G)$, thì tổng của nó là một hàm liên tụ$\widehat{c}$ trên G mà lớp của nó trong $L^1(G)$ bằng $f$.

Ta hãy chứng minh mệnh đề a). Vì G compắc, tổng $f$ của họ $(\mathscr{F}_{\pi}(u_{\pi}))$ thuộc $L^2(G)$ và chuỗi

$$
\sum_{\pi\in\widehat{G}}\mathscr{F}_{\pi}(u_{\pi})
$$

hội tụ trong $L^2(G)$ về $f$ (INT, IV, p. 127, § 3, No.$^o3$, prop. 4). Do đó ta có $\mathscr{F}_G((u_{\pi})_{\pi}) =f$ trong $L^2$(G), do đó $(u_{\pi})_{\pi\in\widehat{G}}=\overline{\mathscr{F}}_G(f)$ (Định lý 2).

Ta hãy chứng minh mệnh đề b). Mệnh đề a) có thể được áp dụng cho họ $(\pi (f))_{\pi\in G}$. Tổng $g$ của họ $(\mathscr{F}_{\pi}(\pi (f)))_{\pi\in G}$ là một hàm liên tục, do đó thuộc $L^2$(G), sao cho $\mathscr{F}_G(g) = (\pi (f))_{\pi\in G}$. Vì $\mathscr{F}_G$ là đơn ánh trên $L^2$(G), ta có $f=g$ trong $L^2$(G), do đó trong $L^1(G)$.

Đại số $\mathscr{C}(\widehat{G})$ các hàm nhận giá trị phức trên $\widehat{G}$ được đồng nhất với tâm của đại số $F(\widehat{G})$ bởi ánh xạ gán cho $f:\widehat{G}\rightarrow \mathbf{C}$ phần tử trung tâm $(f(\pi )1_{E_{\pi}})_{\pi\in\widehat{G}}$ của $F(\widehat{G})$. Ta ký hiệu bởi $\mathscr{M}^1(G^{\sharp})$ không gian các độ đo trung tâm bị chặn trên G. Đây là một không gian con đóng của đại số Banach $\mathscr{M}^1(G)$. Với mọi độ đo $\nu \in \mathscr{M}^1(G^{\sharp})$ và mọi biểu diễn $\pi \in \widehat{G}$, ta có $\pi (\nu )\in$ End$_G(E_{\pi})$ nên $\pi (\nu )$ là một bội của ánh xạ đồng nhất của $E_{\pi}$ theo Bổ đề Schur (Mệnh đề 6 của V, p. 386). Do đó hạn chế của đối biến đổi Fourier lên $\mathscr{M}^1(G^{\sharp})$ được đồng nhất với một cấu xạ có đơn vị của các đại số Banach có đối hợp từ $\mathscr{M}^1(G^{\sharp})$ vào $\mathscr{C}(\widehat{G})$. Cấu xạ này là đơn ánh; ảnh của $L^1(G^{\sharp})$ được chứa trong $\mathscr{C}_b(\widehat{G})$ và hạn chế của nó lên $L^2(G^{\sharp})$ là một đẳng cấu đẳng cự lên $L^2(\widehat{G},\widehat{\mu})$.

### 9. Chỉ số Frobenius-Schur và Phương án thay thế của Larsen

Nhắc lại rằng (LIE, VIII, §7, No. $^o6$, Định nghĩa 2) một biểu diễn bất khả quy của G trong một không gian vectơ phức E có số chiều hữu hạn được gọi là thuộc kiểu trực giao (resp. thuộc kiểu symplectic) nếu tồn tại một dạng song tuyến tính đối xứng khác không trên E bất biến dưới G (resp. nếu tồn tại một dạng song tuyến tính phản xứng khác không trên E bất biến dưới G). Nó được gọi là thuộc kiểu phức nếu không tồn tại dạng song tuyến tính khác không nào trên E bất biến dưới G.

Khi một biểu diễn bất khả quy trong E thuộc kiểu trực giao (resp. symplectic), không gian các dạng song tuyến tính đối xứng (resp. phản xứng) bất biến dưới G trên E có chiều bằng 1 và mọi dạng song tuyến tính bất biến dưới G khác không trên E đều không suy biến.

Một biểu diễn thuộc kiểu trực giao đôi khi được gọi là thuộc kiểu thực, và một biểu diễn thuộc kiểu symplectic đôi khi được gọi là thuộc kiểu quaternion (x. LIE, IX, App. II).

Cho $\pi$ là một biểu diễn bất khả quy của G trong một không gian vectơ phức E. Ba khả năng ở trên được phân biệt bởi giá trị của đại lượng

FS($\pi$ ) $=\int_G\chi_{\pi}(g^2)d\mu(g)$,

được gọi là chỉ số Frobenius-Schur của $\pi$. Thực vậy, ta có

1 nếu $\pi$ thuộc kiểu trực giao,

FS($\pi$ ) $=-1$ nếu $\pi$ thuộc kiểu symplectic,

0 nếu $\pi$ thuộc kiểu phức.

(LIE, IX, App. 2, p. 103, Mệnh đề 3 và p. 105, Mệnh đề 4).

Khi G là một nhóm Lie, ta có thể tính FS($\pi$ ) với sự trợ giúp của Mệnh đề 1 của LIE, IX, p. 69.

#### Định nghĩa 3 {#ts-v-s4-def-3 .statement tag=03EW}

Cho $\varrho$ là một biểu diễn unita hữu hạn chiều của G trong một không gian Hilbert E. Cho $k$ là một số nguyên dương. Moment tuyệt đối bậc $2k$ của $\varrho$ được định nghĩa là, và được ký hiệu bởi $M_{2k}(\varrho )$, chiều của không gian con các phần tử bất biến dưới G trong biểu diễn $\overline{\varrho}^{\otimes k}\otimes \varrho^{\otimes k}$.

#### Định lý 3 (Phương án thay thế của Larsen) {#ts-v-s4-thm-3 .statement tag=03EX}

Giả sử G là vô hạn. Cho $\pi$ là một biểu diễn unita trung thành của G trong một không gian Hilbert E có số chiều hữu hạn $\geqslant 2$.

a) Giả sử rằng nhóm dẫn xuất của G là vô hạn. Khi đó $M_4(\pi )\geqslant 2$ với đẳng thức xảy ra khi và chỉ khi G chứa $\mathbf{S}\mathbf{U}(E)$;

b) Giả sử rằng dim(E) $\geqslant 3$, rằng $\pi$ thuộc kiểu trực giao hoặc symplectic, và rằng dim(E) $\not = 4$ nếu $\pi$ thuộc kiểu trực giao. Khi đó $M_4(\pi )\geqslant 3$ với đẳng thức xảy ra khi và chỉ khi đại số Lie phức hoá của G bằng đại số Lie của một dạng song tuyến tính bất biến dưới G không suy biến trên E. *Điều này xảy ra khi và chỉ khi thành phần liên thông đơn vị $G_0$ của G là một nhóm con compact cực đại của nhóm tự đẳng cấu của một dạng song tuyến tính như vậy.*

Ta sẽ dùng các bổ đề sau trong chứng minh.

#### Bổ đề 5 {#ts-v-s4-lem-5 .statement tag=03EY}

Cho $\pi$ là một biểu diễn unita của G trong một không gian Hilbert E có số chiều hữu hạn. Cho $(\varrho_i)_{i\in I}$ là một họ các biểu diễn unita khác không của G và $(n_i)_{i\in I}$ là một họ các số nguyên $\geqslant 1$ sao cho biểu diễn $\overline{\pi}\otimes \pi$ của G (resp. biểu diễn $\pi \otimes \pi$ ) đẳng cấu với tổng trực tiếp $\bigoplus_{i\in I}\varrho^{n_i}_i$. Khi đó ta có

$$
M_4(\pi )\geqslant \sum_{i\in I}n^2_i
$$

với đẳng thức xảy ra khi và chỉ khi các biểu diễn $\varrho_i$ là bất khả quy và từng đôi một không đẳng cấu.

Ta ký hiệu bởi $\chi_i$ đặc trưng của $\varrho_i$ với $i\in I$. Ta có

$|\chi_{\pi}|^2=\chi_{\overline{\pi}\otimes\pi}=\sum_{i\in I}n_i\chi_i$, (tương ứng, $\chi^2_{\pi}=\chi_{\pi\otimes\pi}=\sum_{i\in I}n_i\chi_i$).

Từ định nghĩa và Hệ quả 3 của V, p. 466, suy ra

$$
M_4(\pi ) =\int_G|\chi_{\pi}|^4d\mu
$$

do đó, trong cả hai trường hợp, công thức

$M_4(\pi ) =\sum_{i,j}n_in_j\int_G\chi_i\overline{\chi}_jd\mu=\sum_{i,j}n_in_j$ chiều của Hom$_G(\varrho_i, \varrho_j)$

(Hệ quả 4, b) của V, p. 459). Cho $i\in I$. Vì biểu diễn $\varrho_i$ khác không, không gian Hom$_G(\varrho_i, \varrho_i)$ khác không, và suy ra cận dưới

$$
M_4(\pi )\geqslant \sum_{i\in I}n^2_i
$$

Hơn nữa, vì $n_i\geqslant$ 1, có đẳng thức khi và chỉ khi ta có chiều của Hom$_G(\varrho_i, \varrho_j) = 0$ nếu $i\not =j$ và chiều của Hom$_G(\varrho_i, \varrho_i) = 1$ với mọi $i$. Điều kiện thứ hai đúng khi và chỉ khi các biểu diễn $\varrho_i$ là bất khả quy (loc. cit.). Khi đó điều kiện thứ nhất được thỏa mãn khi và chỉ khi các biểu diễn $\varrho_i$ từng đôi một không đẳng cấu, theo Bổ đề Schur (V, p. 387, Hệ quả 2).

Nếu E là một môđun trên một vành giao hoán A, thì a-môđun $\mathsf{S}^2(E)$ (tương ứng, $\wedge^2E$) sẽ được gọi là bình phương đối xứng (tương ứng, bình phương ngoài) của E.

#### Bổ đề 6 {#ts-v-s4-lem-6 .statement tag=03EZ}

Cho $q$ là một dạng song tuyến tính không suy biến trên một không gian vectơ phức hữu hạn chiều E có chiều $\geqslant 3$.

a) Nếu $q$ đối xứng, thì biểu diễn liên hợp của đại số Lie trực giao $\mathfrak{s}\mathfrak{o}(q)$ đẳng cấu với bình phương ngoài $\wedge^2E$ của biểu diễn tự nhiên $\mathfrak{s}\mathfrak{o}(q)\rightarrow \mathfrak{g}\mathfrak{l}(E)$;

b) Nếu $q$ phản xứng, thì biểu diễn liên hợp của đại số Lie symplectic $\mathfrak{s}\mathfrak{p}(q)$ đẳng cấu với bình phương đối xứng $\mathsf{S}^2(E)$ của biểu diễn tự nhiên $\mathfrak{s}\mathfrak{p}(q)\rightarrow \mathfrak{g}\mathfrak{l}(E)$.

Cho $\mathbf{C}$ được trang bị phép tự đẳng cấu đối hợp đồng nhất. Khi đó dạng song tuyến tính $q$ là $\varepsilon$-Hermit (A, IX, § 3, n$^o1$, Def. 1) với $\varepsilon = 1$ trong trường hợp a) và $\varepsilon =-1$ trong trường hợp b). Với mọi $u\in$ End(E), ký hiệu $^tu$ là liên hợp của $u$ đối với $q$. Do đó ta có $q(x, u(y)) =q(^tu(x), y)$ với mọi $(x, y)\in E\times E$. Gọi $v$ là tự đẳng cấu duy nhất của $E\otimes E$ sao cho $v(x\otimes y) =y\otimes x$ với mọi $(x, y)\in E^2$.

Tồn tại duy nhất một ánh xạ tuyến tính $w$ từ $E\otimes E$ vào End(E) sao cho $w(a\otimes b)$ là ánh xạ tuyến tính được xác định bởi $x\mapsto q(a, x)b$ với mọi $(a, b, x)\in E^3$. Ánh xạ $w$ là một đẳng cấu. Với mọi $s\in E\otimes E$, ta có

$$
t(w(s)) =\varepsilon  w(v(s)) \tag{3}
$$

Thật vậy, với mọi $(x, y)$ và $(a, b)$ trong $E\times E$, suy ra

$$
q(x, w(a\otimes b)y) =q(a, y)q(x, b) =\varepsilon q(b, x)q(a, y) =q(\varepsilon w(b\otimes a)x, y)
$$

Cuối cùng, ký hiệu bởi $x\mapsto x^*$ đẳng cấu của E lên $E'$ suy ra từ $q$, nghĩa là đẳng cấu sao cho $\langle x^*, y\rangle =q(x, y)$ với mọi $(x, y)\in E^2$.

Với các ký hiệu ấy, gọi H là nhóm trực giao (resp. đối xứng) của $q$. Đó là một nhóm con Lie của $\mathbf{G}\mathbf{L}(E)$ mà đại số Lie $\mathfrak{h}$ của nó là không gian con của End(E) gồm các $u\in$ End(E) sao cho $^tu=-u$ (LIE, III, p. 146, cor. 1). Vì dạng $q$ là H-bất biến, ta có

$$
\langle (ga)^*, b\rangle =q(ga, b) =\langle a, g^{-1}b\rangle
$$

với mọi $g\in H$ và mọi $(a, b)\in E\times E$.

Trang bị cho End(E) biểu diễn liên hợp Ad của H. Ánh xạ tuyến tính $w$ là một cấu xạ của các biểu diễn của H: thật vậy, với mọi $g\in H$ và mọi $(a, b, x)\in E^3$, ta có

$$
w(g(a\otimes b))(x) =\langle (ga)^*, x\rangle gb=\langle a, g^{-1}x\rangle gb
$$

$=g(\langle a, g^{-1}x\rangle b) =$ Ad($g$)$(w(a\otimes b))x$,

do đó kết luận suy ra bởi tính tuyến tính.

Vì $v$ cũng là một cấu xạ của các biểu diễn của H, điều tương tự cũng đúng với ánh xạ tuyến tính $\theta =w-\varepsilon  w\circ v$; vậy nên ánh xạ sau là một cấu xạ của các $\mathfrak{h}$-môđun.

Gọi F $\subset E\otimes E$ là không gian con các phần tử $s\in E\otimes E$ sao cho $v(s) =-\varepsilon s$. Nếu $\varepsilon =-1$, hạn chế lên F của ánh xạ chính tắc từ $E\otimes E$ vào bình phương đối xứng của E là một đẳng cấu của các $\mathbf{C}$-không gian vectơ (A, III, p. 72); nếu $\varepsilon = 1$, hạn chế lên F của ánh xạ chính tắc từ $E\otimes E$ vào bình phương ngoài của E là một đẳng cấu của các $\mathbf{C}$-không gian vectơ (loc. cit., p. 82).

Ảnh của F dưới $\theta$ được chứa trong $\mathfrak{h}:$ thật vậy, với mọi $s\in F$, công thức (3) kéo theo

$$
^t\theta (s) =^tw(s)-\varepsilon^tw(v(s)) =\varepsilon  w(v(s))-w(s) =-\theta (s)
$$

Theo định nghĩa của F, hạn chế của ánh xạ $\theta$ lên F trùng với hạn chế của $2w$ và do đó ánh xạ tuyến tính $\theta$ là đơn ánh trên F. Vì dim(F) = dim($\mathfrak{h}$) (A, III, p. 75, th. 1 and p. 87, cor. 1 and LIE, VIII, p. 192 and p. 201), suy ra rằng $\theta$ cảm sinh, khi chuyển qua các không gian con, một đẳng cấu các $\mathfrak{h}$-môđun từ F lên $\mathfrak{h}$, do đó bổ đề được chứng minh.

#### Bổ đề 7 {#ts-v-s4-lem-7 .statement tag=03F0}

Cho $H_2$ là một nhóm Lie thực và $H_1$ là một nhóm con đóng của $H_2$. Đại số Lie phức hóa của $H_1$ được đồng nhất với một biểu diễn con của biểu diễn liên hợp của $H_1$ trên đại số Lie phức hóa của $H_2$.

Thật vậy, hạn chế lên $H_1$ của biểu diễn liên hợp của $H_2$ trên đại số Lie của nó được đồng nhất với biểu diễn liên hợp của $H_1$.

#### Bổ đề 8 {#ts-v-s4-lem-8 .statement tag=03F1}

Cho E là một không gian Hilbert phức hữu hạn chiều có chiều $n$.

a) Các nhóm $\mathbf{S}\mathbf{U}(E)$ và $\mathbf{U}(E)$ là liên thông;

b) Nhóm dẫn xuất của $\mathbf{S}\mathbf{U}(E)$ bằng $\mathbf{S}\mathbf{U}(E)$;

c) Nhóm dẫn xuất của $\mathbf{U}(E)$ bằng $\mathbf{S}\mathbf{U}(E)$.

Ta có thể giả sử rằng $n\geqslant 1$ và $E =\mathbf{C}^n$.

Gọi A là nhóm con của $\mathbf{U}(E)$ gồm các ma trận đường chéo; nó đồng phôi với $\mathbf{U}^n$, và do đó liên thông (TG, VI, p. 11, hệ quả 2 và I, p. 83, mệnh đề 8). Giao của nó với $\mathbf{S}\mathbf{U}(E)$ đồng phôi với $\mathbf{U}^{n-1}$, và do đó cũng liên thông.

Theo Định lý 1 của IV, p. 149, nhóm $\mathbf{U}(E)$ (resp. $\mathbf{S}\mathbf{U}(E)$) là hợp của các tập con liên thông $gAg^{-1}$ với $g\in G$ (resp. của các tập con liên thông $g(A\cap \mathbf{S}\mathbf{U}(E))g^{-1}$); vì phần tử đơn vị thuộc mỗi tập hợp đó, không gian $\mathbf{U}(E)$ (resp. $\mathbf{S}\mathbf{U}(E)$) là liên thông (TG, I, p. 81, mệnh đề 2).

Chứng minh b). Mệnh đề là đúng khi $n= 1$, vì khi đó $\mathbf{S}\mathbf{U}(E)$ thu về phần tử đơn vị. Vậy giả sử rằng $n\geqslant 2$. Khi đó đại số Lie của $\mathbf{S}\mathbf{U}(E)$ là đơn (LIE, IX, p. 20, § 3, No.$^o4$) và do đó nhóm dẫn xuất của $\mathbf{S}\mathbf{U}(E)$ có chỉ số hữu hạn trong $\mathbf{S}\mathbf{U}(E)$. Kết quả suy ra được, vì $\mathbf{S}\mathbf{U}(E)$ liên thông theo a).

Mệnh đề c) suy ra từ b), vì nhóm dẫn xuất của $\mathbf{U}(E)$ được chứa trong $\mathbf{S}\mathbf{U}(E)$.

Bây giờ chứng minh Định lý 3. Gọi $n$ là chiều của không gian Hilbert E. Vì biểu diễn $\pi$ là trung thành, ta có thể giả sử rằng G là một nhóm con compact của $\mathbf{U}(E)$. Nhóm G là đóng trong nhóm Lie thực $\mathbf{U}$(E), và do đó là một nhóm Lie thực compact (LIE, III, §8, No.$^o2$, Định lý 2). Theo giả thiết, G là vô hạn, và do đó có chiều $\geqslant 1$. Gọi $\mathfrak{g}$ là đại số Lie của nó; nó khác không.

Chứng minh a). Giả sử rằng nhóm dẫn xuất D(G) là vô hạn. Ta có phân tích bất biến dưới G End(E) $=\mathbf{C}1_E\oplus \mathfrak{s}\mathfrak{l}(E)$. Các biểu diễn của G trên $\mathbf{C}1_E$ và trên $\mathfrak{s}\mathfrak{l}(E)$ không đẳng cấu, vì dim $\mathfrak{s}\mathfrak{l}(E)\geqslant 2$. Do đó, theo Bổ đề 5, ta có $M_4(\pi )\geqslant 2$ với đẳng thức khi và chỉ khi biểu diễn của G trong $\mathfrak{s}\mathfrak{l}(E)$ là bất khả quy. Mặt khác, nhóm dẫn xuất của G được chứa trong $\mathbf{S}\mathbf{L}$(E), và do đó phức hóa của đại số Lie của D(G) có thể được đồng nhất với một không gian con của $\mathfrak{s}\mathfrak{l}$(E), là một biểu diễn con của biểu diễn của G trong $\mathfrak{s}\mathfrak{l}(E)$ (Bổ đề 7). Biểu diễn con này khác không, vì D(G) là vô hạn. Do đó ta có $M_4(\pi ) = 2$ khi và chỉ khi $(\mathscr{D}\mathfrak{g})_{(\mathbf{C})}=\mathfrak{s}\mathfrak{l}(E)$. Vì D(G) được chứa trong $\mathbf{S}\mathbf{U}$(E), và vì $\mathbf{S}\mathbf{U}(E) = D(\mathbf{S}\mathbf{U}(E))$ (Bổ đề 8), điều kiện này tương đương với $\mathbf{S}\mathbf{U}(E)\subset G$.

Đối với chứng minh của mệnh đề b), ta dùng lại ký hiệu của LIE, VIII, §13, No.$^o$ 2–4.

Giả sử rằng $\pi$ thuộc kiểu symplectic và dim(E) $\geqslant 3$. Gọi $q$ là một dạng song tuyến tính phản xứng bất biến dưới G khác không trên E; nó không suy biến (LIE, IX, p. 103, App. 2, mệnh đề 3) và G là một nhóm con compact của nhóm symplectic $\mathbf{S}\mathbf{p}(q)$. Gọi $q^*\in \wedge^2E$ là phần tử mà với nó dạng phản xứng $q$ được đồng nhất. Đại số Lie phức hóa $\mathfrak{g}_{(\mathbf{C})}$ của G được chứa trong $\mathfrak{s}\mathfrak{p}(q)$. Bây giờ, vì dim(E) $\geqslant 3$, biểu diễn của $\mathfrak{s}\mathfrak{p}(q)$ trong $E\otimes E$ thừa nhận phân tích tổng trực tiếp

$$
E\otimes E =\mathsf{S}^2(E)\oplus \wedge^2E =\mathsf{S}^2(E)\oplus E_2\oplus \mathbf{C}q^*
$$

trong đó $E_2$ là biểu diễn cơ bản thứ hai của $\mathfrak{s}\mathfrak{p}(q)$ (LIE, VIII, p. 202, §13, No.$^o3$, (IV)). Các biểu diễn $E_2$ và $\mathbf{C}q^*$ của $\mathfrak{s}\mathfrak{p}(q)$ là bất khả quy (loc. cit.) và biểu diễn $\mathsf{S}^2(E)$ khác không.

Sau bổ đề 5, do đó ta có $M_4(\pi )\geqslant 3$ với dấu bằng khi và chỉ khi các biểu diễn của G trong $\mathsf{S}^2$(E), $E_2$ và $\mathbf{C}q^*$ là bất khả quy và từng đôi một không đẳng cấu.

Giả sử $M_4(\pi ) = 3$. Vì biểu diễn $\mathsf{S}^2(E)$ được đồng nhất với biểu diễn liên hợp của $\mathfrak{s}\mathfrak{p}(q)$ (bổ đề 6), nó chứa như biểu diễn con phức hóa của biểu diễn liên hợp của G (bổ đề 7). Do đó ta có $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{p}(q)$.

Ngược lại, giả sử $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{p}(q)$. Biểu diễn liên hợp của $\mathfrak{s}\mathfrak{p}(q)$ và biểu diễn $E_2$ của $\mathfrak{s}\mathfrak{p}(q)$ là bất khả quy, có các chiều lần lượt là $n(n+ 1)/2$ và $n(n-1)/2-1$ (LIE, VIII, p. 202, §13, No.$^o3$, (IV)), các chiều này khác nhau và $\geqslant 2$ vì $n\geqslant 3$, do đó $M_4(\pi ) = 3$.

Cuối cùng, giả sử $\pi$ là kiểu thực và dim(E) $\geqslant 3$ và dim(E) $\not = 4$. Gọi $q$ là một dạng song tuyến tính đối xứng khác không, bất biến dưới G trên E; nó là phân ly (LIE, IX, p. 103, App. 2, mệnh đề 3) và G là một nhóm con compắc của nhóm trực giao $\mathbf{O}(q)$. Ký hiệu bởi $q^*\in \mathsf{S}^2(E)$ phần tử mà $q$ được đồng nhất với nó.

Đại số Lie phức hóa $\mathfrak{g}_{(\mathbf{C})}$ của G được chứa trong $\mathfrak{s}\mathfrak{o}(q)$. Biểu diễn của $\mathfrak{s}\mathfrak{o}(q)$ trong $E\otimes E$ chấp nhận phân tích thành tổng trực tiếp

$$
E\otimes E =\wedge^2E\oplus \mathsf{S}^2(E) =\wedge^2E\oplus \mathsf{S}^2_0(E)\oplus \mathbf{C}q^*
$$

trong đó $\mathsf{S}^2_0(E)$ là trực giao của $q^*$ trong $\mathsf{S}^2(E)$. Các biểu diễn này có chiều ít nhất bằng 2 vì dim(E) $\geqslant 3$. Sau bổ đề 5, ta có $M_4(\pi )\geqslant 3$ với dấu bằng khi và chỉ khi các biểu diễn của G trong $\wedge^2E$ và $\mathsf{S}^2_0(E)$ là bất khả quy và không đẳng cấu.

Giả sử $M_4(\pi ) = 3$. Vì biểu diễn $\wedge^2E$ được đồng nhất với biểu diễn liên hợp của $\mathfrak{s}\mathfrak{o}(q)$ (bổ đề 6), nó chứa như biểu diễn con phức hóa của biểu diễn liên hợp của G (bổ đề 7). Điều kiện $M_4(\pi ) = 3$ do đó kéo theo rằng $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{o}(q)$.

Ngược lại, giả sử rằng $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{o}(q)$. Biểu diễn phụ hợp của $\mathfrak{s}\mathfrak{o}(q)$ là bất khả quy, vì dim(E) $\not = 4$ (LIE, VIII, § 13, p. 193, (I) và p. 206, (I)), và có chiều $n(n-1)/2$. Biểu diễn $\mathsf{S}^2_0(E)$ của $\mathfrak{s}\mathfrak{o}(q)$ có trọng số cao nhất $2\varpi_1$. Bằng cách so sánh chiều của nó với chiều của biểu diễn bất khả quy của $\mathfrak{s}\mathfrak{o}(q)$ có trọng số cao nhất $2\varpi_1$, được tính bằng công thức của Weyl (x. LIE, VIII, §9, n$^o2$, th. 2 và LIE, VI, plates II và IV), ta kiểm tra được rằng $\mathsf{S}^2_0(E)$ là bất khả quy. Do đó suy ra rằng $M_4(\pi ) = 3$ nếu $\mathfrak{g}_{(\mathbf{C})}=\mathfrak{s}\mathfrak{o}(q)$.

#### Nhận xét 1 {#ts-v-s4-n9-rem-1 .statement tag=03F2}

Điều kiện "G là vô hạn" là cần thiết trong Định lý 3 (bài tập 9 của V, p. 507).

#### Nhận xét 2 {#ts-v-s4-n9-rem-2 .statement tag=03F3}

Cho $n\in \mathbf{N}$. Với mọi biểu diễn unita $\varrho$ của một nhóm compact trong một không gian Hilbert có chiều $n$, ta có $M_4(\varrho )\leqslant n^2$; đẳng thức có thể xảy ra (bài tập 15 của V, p. 508).

#### Nhận xét 3 {#ts-v-s4-n9-rem-3 .statement tag=03F4}

Người ta có thể chứng minh (x. R. Guralnick and P.H. Tiep, Phân tích của các lũy thừa tenxơ nhỏ và giả thuyết của Larsen, Biểu diễn Lý thuyết **9** (2005), 138–208) rằng có thể bỏ điều kiện G là vô hạn nếu giả sử rằng E có chiều $\geqslant 7$ và nếu thay giả thiết $M_4(\pi ) = 2$ (tương ứng, $M_4(\pi ) = 3$) bằng $M_8(\pi ) = 24$ (tương ứng, $M_8(\pi ) = 105$).

## BÀI TẬP {#ts-v-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
