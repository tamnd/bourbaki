---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 6
section_title: Espaces classifiants
lang: vi
source: ta-i-iv-fr
book_pages: TA IV.437-TA IV.454, TA IV.477-TA IV.480
pdf_pages: 0453-0470, 0493-0496
extraction: native
subsections:
    - "no": 1
      title: Prolongement des homotopies
      page: 437
      pdf_page: 453
    - "no": 2
      title: Espaces fibrés localement triviaux de base $B\times \mathbf{I}$
      page: 440
      pdf_page: 456
    - "no": 3
      title: Espaces fibrés principaux de base $B\times \mathbf{I}$
      page: 443
      pdf_page: 459
    - "no": 4
      title: Espaces fibrés universels
      page: 446
      pdf_page: 462
    - "no": 5
      title: Espace classifiant pour un groupe discret
      page: 449
      pdf_page: 465
statements: 32
exercises: 9
content_sha256: d179622f8b70d9f6bea337024c2a5171790911ad2eab466ceaa32088ff80a1eb
translated_from: content/en-mt/ta/IV/06_s6_espaces_classifiants.md
source_lang: en-mt
translation_method: machine
source_content_sha256: b015eaffc395a390ad89b5be3071d4a836f54b19acf3405ffc848c6477ed66de
translation_model: gpt-5-6-mini
translation_run: translate-vi-0a1caab1
glossary_version: 34
glossary_terms_sha256: 87a7da845cc3232cdfdea17f05b3394276faef4e1406aedc62dd05b75b2be4df
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. PHÂN LOẠI CÁC KHÔNG GIAN

### 1. Mở rộng các phép đồng luân

#### Mệnh đề 1 {#ta-iv-s6-prop-1 .statement tag=023V}

Cho $X'$ là một không gian tôpô chuẩn, cho X là một không gian con của $X'$, cho A là một không gian con đóng của $X'$ được chứa trong X, và cho U là một lân cận của A trong X.

Ta ký hiệu $i_A$ là đơn ánh chính tắc của A vào X$,i_U$ là đơn ánh chính tắc của U vào X; ký hiệu $j_A$ và $j_U$ là các đơn ánh tương ứng của Cyl($i_A$) và Cyl($i_U$) vào $X\times \mathbf{I}$.

Tồn tại một ánh xạ liên tục $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) sao cho $j_U\circ$ $r(x) =x$ với mọi điểm $x\in j_A$(Cyl($i_A$)).

Cho $U'$ là một tập hợp mở của $X'$ sao cho $A\subset X\cap U'\subset U$. Theo định nghĩa của một không gian chuẩn (TG, IX, p. 41), tồn tại một lân cận mở $V'$ của A trong $X'$ sao cho $A\subset V'\subset \overline{V'}\subset U'$ và một hàm liên tục $\varphi ': X'\rightarrow \mathbf{I}$ bằng 1 tại mọi điểm của A và bằng 0 tại mọi điểm của $\complement V'$. Đặt $\varphi =\varphi '|X$ và $V = X\cap V'$. Ta cũng ký hiệu $\alpha : U\times \mathbf{I}\rightarrow$ Cyl($i_U$) và $\beta : X\rightarrow$ Cyl($i_U$) là các ánh xạ chính tắc (III, p. 238).

Cho $r$ là ánh xạ từ $X\times \mathbf{I}$ vào Cyl($i_U$) được xác định bởi

$\alpha (x,1-(1-t)\varphi (x))$ với $(x, t)\in U\times \mathbf{I}$,

$$
r(x, t) =
$$

$\beta (x)$ trong các trường hợp khác.

Ánh xạ $r$ liên tục trên $U\times \mathbf{I}$. Với mọi điểm $(x, t)\in U\times \mathbf{I}$ sao cho $x\notin V$, ta có $\varphi (x) = 0$, do đó $r(x, t) =\alpha (x,1) =\beta (x)$. Suy ra các ánh xạ $r$ và $\beta \circ$ pr$_1$ trùng nhau trên $(X-V)\times \mathbf{I}$, điều này suy ra rằng $r$ liên tục trên không gian con này. Vì U và phần trong của X-V phủ X, ánh xạ $r$ liên tục.

Cho $y$ là một điểm của Cyl($i_A$) ; đặt $(x, t) =j_A(y)$. Nếu $x\in$ A, $\varphi (x) = 1$ và $r(x, t) =\alpha (x, t)$, do đó $j_U(r(x, t)) = (x, t)$. Ngược lại, $t= 1$ và ta có $r(x, t) =\alpha (x,1)$ nếu $x\in U$ và $r(x, t) =\beta (x)$ trong trường hợp ngược lại ; do đó $j_U(r(x, t)) = (x, t)$ trong trường hợp này. Điều này kéo theo rằng $j_U\circ r$ ánh xạ mọi điểm của $j_A$(Cyl($i_A$)) vào chính nó, do đó có mệnh đề.

#### Hệ quả 1 {#ta-iv-s6-prop-1-cor-1 .statement tag=023W}

Cho X là một không gian tôpô chuẩn, cho $f$ là một ánh xạ liên tục từ X vào một không gian tôpô Z. Cho A là một không gian con đóng của X, cho U là một lân cận của A trong X và cho $\sigma : U\times$ $\mathbf{I}\rightarrow Z$ là một phép đồng luân có số hạng là ánh xạ $f|U$. Tồn tại một phép đồng luân $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow Z$ có số hạng là ánh xạ $f$ và trùng với $\sigma$ trên $A\times \mathbf{I}$.

Đặt $X'= X$ và cho $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) là ánh xạ liên tục được cho bởi Mệnh đề 1. Với các ký hiệu đã đưa vào trong chứng minh của mệnh đề này, tồn tại một ánh xạ liên tục duy nhất F: Cyl($i_U$)$\rightarrow Z$ sao cho $F(\alpha (x, t)) =\sigma (x, t)$ với $(x, t)\in U\times \mathbf{I}$ và $F(\beta (x)) =f(x)$ với $x\in$ X (III, p. 238, Mệnh đề 4). Ánh xạ $F\circ r: X\times \mathbf{I}\rightarrow$ Z là một phép đồng luân ; số hạng của nó ánh xạ một điểm $x\in$ X vào $F(r(x,1)) = F(\beta (x)) =f(x)$. Nếu $(x, t)\in A\times \mathbf{I}$, $F(r(x, t)) = F(\alpha (x, t)) =\sigma (x, t)$, do đó phép đồng luân này trùng với $\sigma$ trên $A\times \mathbf{I}$.

#### Hệ quả 2 {#ta-iv-s6-prop-1-cor-2 .statement tag=023X}

Cho X là một không gian tôpô chuẩn, cho A là một không gian con đóng của X và cho U là một lân cận của A trong X. Cho $f$ và $f'$ là các ánh xạ liên tục đồng luân được từ U vào một không gian tôpô Z. Nếu $f$ có một mở rộng liên tục đến X, thì điều tương tự cũng đúng với ánh xạ $f'|A$.

Cho F là một ánh xạ liên tục từ X vào Z sao cho $F|U =f$. Ta chọn một phép đồng luân $\sigma : A\times \mathbf{I}\rightarrow Z$ nối $f'$ với $f$. Theo Hệ quả 1, tồn tại một phép đồng luân $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow Z$ có số hạng F và mở rộng $\sigma$. Gốc của $\widetilde{\sigma}$ khi đó là một ánh xạ liên tục từ X vào Z trùng với $f'$ trên A.

#### Hệ quả 3 {#ta-iv-s6-prop-1-cor-3 .statement tag=023Y}

Cho X là một không gian tôpô chuẩn, cho A là một không gian con đóng của X và cho U là một lân cận của A trong X. Cho Z là một không gian tôpô đồng luân với một điểm và cho $g: U\rightarrow$ Z là một ánh xạ liên tục. Tồn tại một ánh xạ liên tục $\widetilde{g}: X\rightarrow Z$ trùng với $g$ trên A.

Vì Z đồng luân với một điểm, ánh xạ $g$ đồng luân với một ánh xạ hằng $f$. Ánh xạ $f$ mở rộng liên tục đến X ; do đó mệnh đề suy ra từ Hệ quả 2.

#### Hệ quả 4 {#ta-iv-s6-prop-1-cor-4 .statement tag=023Z}

Cho $X$ là một không gian tôpô paracompact, cho $A$ là một không gian con đóng của $X$. Cho $n$ là một số nguyên $\geqslant 0$ và cho $V$ là một tập con mở của $\mathbf{R}^n$. Cho $f: X\rightarrow V$ là một ánh xạ liên tục và cho $\sigma : A\times \mathbf{I}\rightarrow V$ là một phép đồng luân có ánh xạ cuối $f|A$. Tồn tại một phép đồng luân $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow V$ có ánh xạ cuối $f$ và mở rộng $\sigma$.

Ta ký hiệu $i_A$ là đơn ánh chính tắc của A vào X, $\alpha_A: A\times \mathbf{I}\rightarrow$ Cyl($i_A$) và $\beta_A: X\rightarrow$ Cyl($i_A$) là các ánh xạ chính tắc, và cũng ký hiệu $j_A:$ Cyl($i_A$)$\rightarrow$ $X\times \mathbf{I}$ là đơn ánh chính tắc. Vì A đóng trong X, $j_A$ xác định một đồng phôi của Cyl($i_A$) lên không gian con đóng $(A\times \mathbf{I})\cup (X\times \{1\})$ của $X\times \mathbf{I}$. Gọi $\widetilde{\sigma}_0$ là ánh xạ duy nhất của Cyl($i_A$) vào V sao cho $\widetilde{\sigma}_0\circ \alpha_A=\sigma$ và $\widetilde{\sigma}_0\circ \beta_A=f$; nó liên tục (III, p. 238, mệnh đề 4).

Vì X là paracompact và $\mathbf{I}$ compact, không gian $X\times \mathbf{I}$ là paracompact (TG, I, p. 70, mệnh đề 17), do đó là chuẩn tắc (TG, IX, p. 49, mệnh đề 4). Do đó tồn tại một ánh xạ liên tục $k: X\times \mathbf{I}\rightarrow \mathbf{R}^n$ sao cho $k\circ j_A=\widetilde{\sigma}_0$ (TG, IX, p. 45, hệ quả).

Tập hợp U gồm các điểm $x\in$ X sao cho $k(x, t)\in$ V với mọi $t\in \mathbf{I}$ là mở trong X (IV, p. 439, bổ đề 1). Do đó nó là một lân cận của A. Theo hệ quả 1, áp dụng cho ánh xạ $f$ và phép đồng luân $k|U\times \mathbf{I}$, tồn tại một phép đồng luân $\widetilde{\sigma}: X\times \mathbf{I}\rightarrow V$ có ánh xạ ban đầu $f$ trùng với $k$, do đó với $\sigma$, trên $A\times \mathbf{I}$.

#### Bổ đề 1 {#ta-iv-s6-lem-1 .statement tag=0240}

Cho Z là một không gian tôpô, K là một không gian tôpô compact và W là một tập con mở của $Z\times K$. Tập hợp U gồm các điểm $z\in Z$ sao cho $\{z\} \times K$ được chứa trong W là mở trong Z.

Phép chiếu thứ nhất pr$_1: Z\times K\rightarrow Z$ là thực sự (TG, I, p. 77, hệ quả 5), do đó là đóng. Do đó, $\complement U =$ pr$_1(\complement W)$ là đóng trong Z và U là mở.

#### Hệ quả 5 {#ta-iv-s6-lem-1-cor-5 .statement tag=0241}

Cho $X'$ là một không gian tôpô chuẩn tắc, cho X là một không gian con của $X'$, cho A là một không gian con đóng của $X'$ được chứa trong X, và cho U là một lân cận của A trong X.

Cho Y và Z là các không gian tôpô; cho $f: X\times  \{1\} \times Y\rightarrow$ $X\times  \{1\} \times Z$ là một $X\times  \{1\}$-cấu xạ và cho $g: U\times \mathbf{I}\times Y\rightarrow U\times \mathbf{I}\times Z$ là một $U\times \mathbf{I}$-cấu xạ trùng với $f$ trên $U\times  \{1\} \times Y$.

Khi đó tồn tại một $X\times \mathbf{I}$-cấu xạ $h: X\times \mathbf{I}\times Y\rightarrow X\times \mathbf{I}\times Z$ trùng với $f$ trên $X\times  \{1\} \times Y$ và với $g$ trên $A\times \mathbf{I}\times Y$.

Hơn nữa, nếu $f$ và $g$ là các phép đồng phôi, ta có thể chọn một phép đồng phôi $h$ có các tính chất yêu cầu.

Cho $U'$ là một lân cận mở của A trong $X'$ sao cho $U'\cap X\subset U$. Vì không gian $X'$ là chuẩn tắc, tồn tại một lân cận mở $V'$ của A trong $X'$ sao cho $A\subset V'\subset \overline{V'}\subset U'$ (TG, IX, p. 41). Thay thế U bởi $\overline{V'}\cap X$ nếu cần, do đó ta có thể giả sử rằng U là đóng trong X. Khi đó, ta dùng lại ký hiệu của Mệnh đề 1 và chứng minh của nó; cho $r: X\times \mathbf{I}\rightarrow$ Cyl($i_U$) là một ánh xạ liên tục sao cho $j_U\circ r(x) =x$ với mọi điểm $x\in j_A$(Cyl($i_A$)).

Đặt thêm $f'=$ pr$_3\circ f$ và $g'=$ pr$_3\circ g$. Vì $f'$ và $g'$ trùng nhau trên $U\times  \{1\} \times Y$, tồn tại một ánh xạ duy nhất

$\varphi :$ Cyl($i_U$)$\times Y\rightarrow$ Cyl($i_U$)$\times Z$

sao cho $\varphi (\alpha (x, t), y) = (\alpha (x, t), g'(x, t, y))$ với $(x, t, y)\in U\times \mathbf{I}\times Y$ và $\varphi (\beta (x), y) = (\beta (x), f'(x,1, y))$ với $(x, y)\in X\times Y$. Vì U là đóng trong X, toàn cấu chính tắc $\pi$ của $(U\times \mathbf{I})\cup X$ lên Cyl($i_U$) là ngặt phổ quát (III, p. 239, nhận xét 2). Vì ánh xạ $\varphi \circ (\pi \times$ Id$_Y)$ là liên tục, ánh xạ $\varphi$ là liên tục. Do đó nó là một cấu xạ của các không gian Cyl($i_U$), và thậm chí là một đẳng cấu nếu $f$ và $g$ là các phép đồng phôi.

Khi đó, cho $h: X\times \mathbf{I}\times Y\rightarrow X\times \mathbf{I}\times Z$ là ánh xạ $r^*(\varphi )$ suy ra từ $\varphi$ bởi phép thay đổi cơ sở $r$. Nó được cho bởi $h(x, t, y) =$ $(x, t$, pr$_2(\varphi (r(x, t), y)))$ với $(x, t, y)\in X\times \mathbf{I}\times Y$. Nó là một cấu xạ của các không gian $X\times \mathbf{I}$, và thậm chí là một đẳng cấu nếu $\varphi$ là một đẳng cấu. Với $(x, t, y)\in$ $A\times \mathbf{I}\times Y$, ta có $r(x, t) = (x, t)$, do đó

$h(x, t, y) = (x, t$, pr$_2(\varphi (x, t, y))) = (x, t, g'(x, t, y)) =g(x, t, y)$,

điều này chứng minh rằng $h$ trùng với $g$ trên $A\times \mathbf{I}\times Y$. Tương tự, với $x\in X$ và $y\in Y$, ta có $r(x,1) = (x,1)$, do đó

$h(x,1, y) = (x,1$, pr$_2(\varphi (x,1, y))) = (x,1, f'(x,1, y)) =f(x,1, y)$

suy ra $h$ trùng với $f$ trên $X\times  \{1\} \times Y$. Hệ quả được chứng minh.

### 2. Các không gian thớ địa phương tầm thường với cơ sở $B\times \mathbf{I}$

#### Mệnh đề 2 {#ta-iv-s6-prop-2 .statement tag=0242}

Cho B là một không gian tôpô paracompact và $(E, p)$ là một không gian thớ địa phương tầm thường trên $B\times \mathbf{I}$. Đặt $E_1=\overset{-1}{p}(B\times \{1\})$ và ký hiệu $p_1: E_1\rightarrow B$ là ánh xạ pr$_1\circ p|E_1$. Khi đó các $B\times \mathbf{I}$-không gian $(E, p)$ và $(E_1\times \mathbf{I}, p_1\times$ Id$_{\mathbf{I}})$ là đẳng cấu.

Trước hết ta chứng minh hai bổ đề.

#### Bổ đề 2 {#ta-iv-s6-lem-2 .statement tag=0243}

Cho $\alpha ,\beta ,\gamma$ là các số thực sao cho $\alpha \leqslant \beta \leqslant \gamma$, cho B là một không gian tôpô và cho $p: E\rightarrow B\times [\alpha , \gamma ]$ là một ánh xạ liên tục. Đặt $B_0= B\times [\alpha , \beta ]$, $B_1= B\times [\beta , \gamma ]$, $E_0=\overset{-1}{p}(B_0)$, $E_1=$ $\overset{-1}{p}(B_1)$ và ký hiệu $p_0: E_0\rightarrow B_0,p_1: E_1\rightarrow B_1$ là các ánh xạ suy ra từ p. Nếu $(E_0, p_0)$ và $(E_1, p_1)$ là các không gian thớ tầm thường hóa được, thì điều tương tự cũng đúng đối với $(E, p)$.

Cho $g_0: E_0\rightarrow B_0\times F_0$ và $g_1: E_1\rightarrow B_1\times F_1$ là các phép tầm thường hóa của $E_0$ và $E_1$ tương ứng. Gọi $g'_0$ và $g'_1$ là các phép tầm thường hóa của không gian phân thớ $B\times  \{\beta \}$ $\overset{-1}{p}(B\times  \{\beta \})$ suy ra từ $g_0$ và $g_1$ bằng hạn chế. Ánh xạ $h=g'_0\circ (g'_1)^{-1}$ là một $B\times  \{\beta \}$-đẳng cấu của $B\times  \{\beta \} \times F_1$ lên $B\times  \{\beta \} \times F_0$. Định nghĩa một ánh xạ liên tục $h'$ từ $B\times F_1$ vào $F_0$ bằng cách đặt $h'(a, y) =$ pr$_3\circ h(a, \beta , y)$ với $(a, y)\in B\times F_1$. Với $(a, t, y)\in B\times [\beta , \gamma ]\times F_1$, đặt $H(a, t, y) = (a, t, h'(a, y))$. Ánh xạ H thu được là một $(B\times [\beta , \gamma ])$-đẳng cấu của $B\times [\beta , \gamma ]\times F_1$ lên $B\times [\beta , \gamma ]\times F_0$, và ta có $g_0|\overset{-1}{p}(B\times  \{\beta \}) = H\circ g_1|\overset{-1}{p}(B\times  \{\beta \})$. Do đó tồn tại một ánh xạ liên tục $g: E\rightarrow B\times [\alpha , \gamma ]\times F_0$ sao cho $g|E_0=g_0$ và $g|E_1= H\circ g_1$. Ánh xạ $g$ là một đẳng cấu của các không gian $B\times [\alpha , \gamma ]$, do đó E là tầm thường hóa được.

#### Bổ đề 3 {#ta-iv-s6-lem-3 .statement tag=0244}

Cho B là một không gian tôpô và cho $(E, p)$ là một không gian phân thớ $B\times \mathbf{I}$ địa phương tầm thường. Mọi điểm $a$ của B đều có một lân cận V sao cho không gian $V\times \mathbf{I}$ $E_{V\times\mathbf{I}}$ là tầm thường hóa được.

Cho $a$ là một điểm của B; với mọi điểm $t$ của $\mathbf{I}$, tồn tại một lân cận mở $W_t$ của $t$ trong $\mathbf{I}$ và một lân cận $V_t$ của $a$ trong B sao cho E là tầm thường hóa được trên $V_t\times W_t$. Khi đó tồn tại một số nguyên $n >0$ và, với mọi số nguyên $i$ sao cho 1 $\leqslant i\leqslant n$, một điểm $t_i$ của $\mathbf{I}$ sao cho khoảng $[\frac{i-1}{n},\frac{i}{n}]$ được chứa trong $W_{t_i}($III, p. 272, bổ đề 4). Đặt $V =\cap_{1\leqslant i\leqslant n}V_{t_i}$. Không gian phân thớ E là tầm thường hóa được trên $V\times$ $[\frac{i-1}{n},\frac{i}{n}]$ với mọi số nguyên $i$ sao cho $1\leqslant i\leqslant n$. Bổ đề 3 khi đó suy ra từ Bổ đề 2 bằng quy nạp theo $n$.

#### Hệ quả 1 {#ta-iv-s6-lem-3-cor-1 .statement tag=0245}

Cho B là một không gian tôpô paracompact và $(E, p)$ là một không gian sợi địa phương tầm thường trên $B\times \mathbf{I}$ (I, p. 71, Hệ quả 2). Với $t\in \mathbf{I}$, ký hiệu $(E_t, p_t)$ là không gian sợi địa phương tầm thường trên B $i^*_tE$, trong đó $i_t: B\rightarrow B\times  \{t\}$ là ánh xạ $b\mapsto (b, t)$. Các không gian sợi địa phương tầm thường trên B $E_0$ và $E_t$ là đẳng cấu với nhau với mọi $t\in \mathbf{I}$.

#### Hệ quả 2 {#ta-iv-s6-lem-3-cor-2 .statement tag=0246}

Cho B và $B'$ là các không gian tôpô, và E là một không gian sợi địa phương tầm thường trên B. Cho $f_0$ và $f_1$ là các ánh xạ liên tục từ $B'$ vào B. Giả sử không gian $B'$ là paracompact. Nếu các ánh xạ $f_0$ và $f_1$ đồng luân, thì các không gian sợi địa phương tầm thường trên $B'$ $f_0^*E$ và $f_1^*E$ là đẳng cấu.

Cho $\sigma : B'\times \mathbf{I}\rightarrow B$ là một phép đồng luân nối $f_0$ với $f_1$ và ký hiệu E' là không gian trên $B'\times \mathbf{I}$ $\sigma^*E$; đây là một không gian sợi địa phương tầm thường. Ký hiệu $i_0$ và $i_1$ là các ánh xạ từ $B'$ vào $B'\times \mathbf{I}$ được cho bởi $x\mapsto (x,0)$ và $x\mapsto (x,1)$. Theo Hệ quả 1, các không gian sợi trên $B'$ $i^*_0E'$ và $i^*_1E'$ là đẳng cấu. Vì $\sigma \circ i_0=f_0$, không gian trên $B'$ $i^*_0E'$ được đồng nhất với $f_0^*E$; tương tự, không gian trên $B'$ $i^*_1E'$ được đồng nhất với $f_1^*E$. Do đó, các không gian sợi trên $B'$ $f_0^*E$ và $f_1^*E$ là đẳng cấu, như cần phải chứng minh.

#### Hệ quả 3 {#ta-iv-s6-lem-3-cor-3 .statement tag=0247}

Cho B là một không gian tôpô paracompact. Nếu B đồng luân với một điểm, thì mọi không gian sợi địa phương tầm thường có cơ sở B đều tầm thường hóa được.

#### Hệ quả 4 {#ta-iv-s6-lem-3-cor-4 .statement tag=0248}

Cho B và $B'$ là các không gian tôpô, $(E, p)$ là một không gian sợi địa phương tầm thường trên B, $f$ là một ánh xạ liên tục từ $B'$ vào B, $\sigma : B'\times \mathbf{I}\rightarrow B$ là một phép đồng luân bắt đầu từ $f$, và $\widetilde{f}$ là một nâng liên tục của $f$ vào E. Nếu không gian $B'$ là paracompact, tồn tại một phép đồng luân $\widetilde{\sigma}: B'\times \mathbf{I}\rightarrow E$ bắt đầu từ $\widetilde{f}$ là một nâng của $\sigma$ vào E.

Cho $(E', p')$ là không gian $B'\times \mathbf{I}$ suy ra từ $(E, p)$ bằng phép đổi cơ sở bởi ánh xạ $\sigma : B'\times \mathbf{I}\rightarrow B$. Nó là một không gian thớ địa phương tầm thường (I, p. 71, Hệ quả 2), và ánh xạ $s: B'\times  \{0\} \rightarrow E'$ được định nghĩa bởi $s((a,0)) = ((a,0),\widetilde{f}(a))$ với $a\in B'$ là một tiết diện liên tục của $p'$ trên $B'\times  \{0\}$. Theo Mệnh đề 2, tồn tại một tiết diện liên tục $\widetilde{s}$ của $p'$ mở rộng $s$. Ánh xạ $\widetilde{\sigma}=$ pr$_2\circ \widetilde{s}$ có tính chất yêu cầu.

### 3. Các không gian thớ chính với cơ sở $B\times \mathbf{I}$

Cho G là một nhóm tôpô. Ta sẽ thấy rằng Mệnh đề 2 và các hệ quả của nó vẫn đúng khi, trong mỗi mệnh đề, thay “không gian thớ địa phương tầm thường” bằng “không gian thớ chính với nhóm G”.

#### Bổ đề 4 {#ta-iv-s6-lem-4 .statement tag=0249}

Cho B là một không gian tôpô, cho G là một nhóm tôpô và cho E, $E'$ là các không gian thớ chính với nhóm G và cơ sở B. Gọi F là không gian tôpô G được trang bị phép toán trái của $G\times G$ cho bởi $(g, g')\cdot f=g'f g^{-1}$, và gọi $M = (E\times_BE')\times^{G\times G}F$ là không gian thớ địa phương tầm thường với kiểu thớ F và cơ sở B liên kết với nó.

Bó $\mathscr{S}$ trên B của các tiết diện của M là đẳng cấu với bó trên B của các đẳng cấu của các không gian thớ chính từ E lên $E'$.

Ta ký hiệu các phép chiếu của các không gian B E, $E'$ và M lần lượt là $p,p'$ và $q$. Với $(x, x')\in E\times_BE'$ và $f\in F$, gọi $[x, x', f]$ là lớp trong M của phần tử $((x, x'), f)\in (E\times_BE')\times F$. Gọi $\mathscr{M}$ là bó trên B của các đẳng cấu của các không gian thớ chính từ E lên $E'$; các tiết diện của nó trên một tập mở U của B là các đẳng cấu của các không gian thớ chính từ $E_U$ lên $E'_U$.

Gọi $e$ là phần tử đơn vị của G. Cho U là một tập mở của B và cho $\varphi : E_U\rightarrow E'_U$ là một đẳng cấu của các không gian thớ chính với nhóm G và cơ sở U. Ánh xạ từ $E_U$ vào $(E\times_BE')\times^{G\times G}F$ được định nghĩa bởi $x\mapsto [x, \varphi (x), e]$ là liên tục. Với $g\in G$ và $x\in E_U$, nó gửi $x\cdot g$ vào $[x\cdot g, \varphi (x\cdot g), e] = [x, \varphi (x), geg^{-1}] = [x, \varphi (x), e]$. Do đó tồn tại một ánh xạ liên tục duy nhất $\alpha_U(\varphi ): U\rightarrow M$ sao cho $\alpha_U(\varphi )(p(x)) = [x, \varphi (x), e]$ với mọi $x\in E_U$; ta có $\alpha_U(\varphi )\in \mathscr{S}(U)$.

Hiển nhiên rằng các ánh xạ $\alpha_U$ xác định một cấu xạ của các bó $\alpha$ từ $\mathscr{M}$ vào $\mathscr{S}$.

#### Bổ đề 5 {#ta-iv-s6-lem-5 .statement tag=024A}

Cấu xạ của các bó $\alpha$ là một đẳng cấu.

Trước hết, giả sử rằng các không gian thớ chính E và $E'$ đều tầm thường hóa được; chọn các tiết diện $i: B\rightarrow E$ và $i': B\rightarrow E'$ của chúng. Khi đó tồn tại một ánh xạ liên tục duy nhất $\theta$ từ M vào $B\times G$ sao cho

$$
\theta ([i(b)\cdot g, i'(b)\cdot g', f]) = (b, g'f g^{-1})
$$

với $b\in B,g\in G,g'\in G$ và $f\in$ F; đó là một đẳng cấu của các không gian B. Cho $\varphi$ là một đẳng cấu của các không gian sợi chính từ E lên $E'$; tồn tại một ánh xạ liên tục duy nhất $\gamma : B\rightarrow G$ sao cho $\varphi (i(b)) =i'(b)\cdot \gamma (b)$ với $b\in B$. Ảnh của $\varphi$ qua ánh xạ $\alpha_B$ là ánh xạ $b\mapsto \theta^{-1}(b, \gamma (b))$ từ B vào M. Điều này suy ra rằng $\alpha_B$ là một song ánh.

Do đó, $\alpha_U$ là một song ánh với mọi tập mở U của B sao cho các không gian sợi chính $E_U$ và $E'_U$ là tầm thường hóa được. Theo hệ quả 2 của I, p. 55, điều này suy ra rằng $\alpha$ là một đẳng cấu của các bó.

#### Mệnh đề 3 {#ta-iv-s6-prop-3 .statement tag=024B}

Cho G là một nhóm tôpô, cho B là một không gian tôpô paracompact và cho $(E, p)$ là một không gian sợi chính của nhóm G và cơ sở $B\times \mathbf{I}$. Đặt $E_1=\overset{-1}{p}(B\times \{1\})$ và cho $p_1: E_0\rightarrow B$ là ánh xạ pr$_1\circ p|E_1$. Khi đó, $(E, p)$ và $(E_1\times \mathbf{I}, p_1\times$ Id$_{\mathbf{I}})$ là các không gian sợi chính đẳng cấu của nhóm G và cơ sở $B\times \mathbf{I}$.

Cho F là không gian tôpô G được trang bị phép toán trái của nhóm $G\times G$ cho bởi $(g, g')\cdot f=g'f g^{-1}$. Cho $(M, q)$ là không gian sợi địa phương tầm thường có cơ sở $B\times \mathbf{I}$ và kiểu sợi F liên kết với không gian sợi chính $E\times_{B\times\mathbf{I}}(E_1\times \mathbf{I})$ của nhóm $G\times G$. Đặt $M_1=\overset{-1}{q}(B\times \{1\})$ và $q_1=$ pr$_1\circ p|M_1$; không gian B $(M_1, q_1)$ được đồng nhất với không gian sợi địa phương tầm thường có kiểu sợi F liên kết với $E_1\times_BE_1$. Theo bổ đề 4, trong đó lấy các không gian sợi chính E và $E'$ đều bằng $E_1$, không gian B $M_1$ có một tiết diện. Vì các không gian $B\times \mathbf{I}$ $(M, q)$ và $(M_1\times \mathbf{I}, q_1\times$Id$_{\mathbf{I}})$ là đẳng cấu (IV, p. 440, prop. 2), không gian $B\times \mathbf{I}$ $(M, q)$ có một tiết diện, điều này suy ra rằng các không gian sợi chính của nhóm G, E và $E_1\times \mathbf{I}$, là đẳng cấu.

#### Hệ quả 1 {#ta-iv-s6-prop-3-cor-1 .statement tag=024C}

Cho B là một không gian tôpô paracompact, cho G là một nhóm tôpô và cho $(E, p)$ là một không gian sợi chính $B\times \mathbf{I}$ của nhóm G. Với $t\in \mathbf{I}$, ký hiệu $(E_t, p_t)$ là không gian B-sợi chính $i^*_tE$, trong đó $i_t: B\rightarrow B\times  \{t\}$ là ánh xạ $b\mapsto (b, t)$. Các không gian B-sợi chính $E_0$ và $E_t$ là đẳng cấu với mọi $t\in \mathbf{I}$.

#### Hệ quả 2 {#ta-iv-s6-prop-3-cor-2 .statement tag=024D}

Cho B và $B'$ là các không gian tôpô, cho G là một nhóm tôpô, và cho E là một không gian thớ chính trên B với nhóm G. Cho $f_0$ và $f_1$ là các ánh xạ liên tục từ $B'$ vào B. Giả sử rằng không gian $B'$ là paracompact. Nếu các ánh xạ $f_0$ và $f_1$ đồng luân, thì các không gian thớ chính trên $B'$ $f_0^*E$ và $f_1^*E$ là đẳng cấu.

#### Hệ quả 3 {#ta-iv-s6-prop-3-cor-3 .statement tag=024E}

Cho B là một không gian tôpô paracompact và cho G là một nhóm tôpô. Nếu B đồng luân với một điểm, thì mọi không gian thớ chính với nhóm G đều khả quy về tầm thường.

#### Nhận xét {#ta-iv-s6-n3-rem-1 .statement tag=024F}

Một chứng minh khác của các kết quả này sẽ bao gồm việc kiểm tra rằng các đẳng cấu của các không gian thớ được xây dựng trong mệnh đề 2 và các hệ quả của nó là các đẳng cấu của các không gian thớ chính.

### 4. Các không gian thớ phổ quát

Cho G là một nhóm tôpô, cho B và $B'$ là các không gian tôpô, và cho $(E, p)$ và $(E', p')$ là các không gian thớ chính với nhóm G và với các cơ sở lần lượt là B và $B'$.

Cho U là một tập con mở của B và cho $f':\overset{-1}{p}(U)\rightarrow E'$ là một ánh xạ liên tục tương thích với các phép toán của G trong $\overset{-1}{p}(U)$ và $E'$ tương ứng. Khi đó tồn tại duy nhất một ánh xạ liên tục $f: U\rightarrow B'$ sao cho $f\circ p_U=p'\circ f'$ và hình vuông giao hoán

$$
E_U^{f'}E'
$$

$p_Up'$

U $^fB'$

khi đó là Descartes (I, p. 94, ví dụ (FP)).

Với mọi tập con mở U của B, ta ký hiệu bởi $\mathscr{F}(U)$ tập hợp các ánh xạ liên tục $g: E_U\rightarrow E'$ tương thích với các phép toán của G trong $\overset{-1}{p}(U)$ và $E'$ tương ứng. Với mọi cặp $(U,V)$ các tập con mở của B sao cho $U\subset V$, ký hiệu $r_{UV}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$ là ánh xạ được xác định bởi $r_{UV}(g) =g|E_U$. Ta kiểm tra ngay lập tức rằng theo cách này một bó $\mathscr{F}= ((\mathscr{F}(U)),(r_{UV}))$ trên B đã được xác định. Ta sẽ gọi bó này là bó trên B của các cấu xạ của các không gian thớ chính với nhóm G từ E vào $E'$.

#### Mệnh đề 4 {#ta-iv-s6-prop-4 .statement tag=024G}

Nếu không gian B là paracompact và nếu không gian $E'$ đồng luân với một điểm, thì bó trên B của các cấu xạ của các không gian thớ chính với nhóm G từ E vào $E'$ là một bó mềm.

Tồn tại một phủ mở $(U_j)_{j\in J}$ của B sao cho, với mọi $j\in J$, không gian thớ $E_{U_j}$ là khả quy về tầm thường. Vì không gian B là paracompact, ta có thể giả sử rằng phủ $(U_j)_{j\in J}$ là hữu hạn địa phương (TG, IX, p. 49) và chọn một phủ $(A_j)_{j\in J}$ của B trong đó, với mọi $j\in J$, tập hợp $A_j$ là đóng trong B và được chứa trong $U_j$ (TG, IX, p. 49, mệnh đề 4 và p. 48, hệ quả 1).

Theo I, p. 65, hệ quả 2 của mệnh đề 6, để chứng minh mệnh đề, chỉ cần thiết lập mệnh đề sau: cho U là một tập con mở của B sao cho không gian thớ chính $(E_U, p_U)$ là khả quy về tầm thường, cho A là một tập con đóng của B được chứa trong U, cho V là một lân cận mở của A được chứa trong U, và cho $f$ là một phần tử của $\mathscr{F}(V)$; khi đó tồn tại một lân cận mở W của A trong V và một phần tử $f'$ của $\mathscr{F}(U)$ sao cho $r_{WU}(f') =r_{WV}(f)$. Ta hãy chứng minh mệnh đề này.

Cho W là một tập con mở của B sao cho $A\subset W\subset \overline{W}\subset V$. Cho $s: U\rightarrow E_U$ là một tiết diện của $(E_U, p_U)$. Áp dụng Hệ quả 3 (IV, p. 438) cho không gian B, tập con đóng $\overline{W}$ và lân cận V của $\overline{W}$, và cho ánh xạ $g=f\circ (s|_V)$ từ $E_V$ vào $E'$. Khi đó tồn tại một ánh xạ liên tục $\widetilde{g}: B\rightarrow E'$ trùng với $g$ trên $\overline{W}$. Đặt $h=\widetilde{g}|_U$. Ta có $h|_W=g|_W=f\circ (s|_W)$.

Ánh xạ $H: U\times G\rightarrow E'$ được xác định bởi $H(x, g) =h(x)\cdot g$ với $(x, g)\in U\times G$ là liên tục và tương thích với các phép toán của G trong $U\times G$ và $E'$. Đặt $f'= H\circ s^{-1}$; đây là một phần tử của $\mathscr{F}(U)$. Với mọi $x\in W$, các ánh xạ $f$ và $f'$ trùng nhau tại điểm $s(x)$, do đó tại mọi điểm của $\overset{-1}{p}(x)$, vì chúng là các đồng cấu của các không gian thớ chính. Mệnh đề được suy ra.

#### Định lý 1 {#ta-iv-s6-thm-1 .statement tag=024H}

Cho G là một nhóm tôpô, cho $B_u$ là một không gian tôpô, và cho $(E_u, p_u)$ là một không gian thớ chính với nhóm G và cơ sở $B_u$. Giả sử rằng không gian $E_u$ đồng luân với một điểm.

Cho B là một không gian tôpô paracompact.

a) Mọi không gian thớ chính với nhóm G và cơ sở B đều đẳng cấu với một không gian thớ chính có dạng $f^*E_u$, trong đó $f: B\rightarrow B_u$ là một ánh xạ liên tục.

b) Cho $f_0$ và $f_1$ là các ánh xạ liên tục từ B vào $B_u$. Để $f_0^*E_u$ và $f_1^*E_u$ là các không gian thớ chính đẳng cấu với nhóm G và cơ sở B, điều kiện cần và đủ là các ánh xạ $f_0$ và $f_1$ đồng luân.

Nói cách khác, tồn tại một ánh xạ từ $[B,B_u]$ vào P(B; G) gán cho lớp đồng luân của một ánh xạ liên tục $f$ từ B vào $B_u$ lớp đẳng cấu của không gian thớ chính $f^*E_u$. Ánh xạ này là song ánh.

Cho E là một không gian thớ chính với nhóm G và cơ sở B. Theo Mệnh đề 4, bó $\mathscr{F}$ trên B của các đồng cấu của các không gian thớ chính của E vào $E_u$ là mềm. Do đó $\mathscr{F}(B)$ không rỗng, do đó a).

Cho $f_0$ và $f_1$ là các ánh xạ liên tục từ B vào $B_u$. Nếu các ánh xạ $f_0$ và $f_1$ đồng luân, thì các không gian sợi chính $f_0^*E_u$ và $f_1^*E_u$ đẳng cấu (IV, p. 445, hệ quả 2). Ta hãy chứng minh đảo lại. Với $\alpha \in  \{0,1\}$, ký hiệu $E_{\alpha}$ là không gian sợi chính $B_u$ $f_{\alpha}^*E_u$, $g_{\alpha}: E_{\alpha}\rightarrow E_u$ là phép chiếu thứ nhất và $p_{\alpha}: E_{\alpha}\rightarrow B$ là phép chiếu thứ hai. Cho $i: E_0\rightarrow E_1$ là một đẳng cấu các không gian sợi chính. Cho $p$ là ánh xạ $p_0\times$ Id$_{\mathbf{I}}: E_0\times \mathbf{I}\rightarrow B\times \mathbf{I}$.

Vì không gian $B\times \mathbf{I}$ là paracompact (TG, IX, p. 70, mệnh đề 17), bó $\mathscr{G}$ trên $B\times \mathbf{I}$ gồm các tựa cấu của các không gian sợi chính từ $E_0\times \mathbf{I}$ vào $E_u$ là mềm (IV, p. 446, mệnh đề 4). Đặt $A = B\times  \{0,1\}$, $U = B\times ([0,\frac{1}{2}[\cup ]\frac{1}{2},1])$, và định nghĩa một phần tử $g$ của $\mathscr{G}(U)$ bằng cách đặt

$g_0(x)$ với $(x, t)\in E_0\times [0,^1[$,

$g(x, t) =$ 2

$g_1\circ i(x)$ với $(x, t)\in E_0\times ]\frac{1}{2},1]$.

Vì bó $\mathscr{G}$ là mềm, tồn tại một phần tử $h\in \mathscr{G}(B\times \mathbf{I})$ và một lân cận mở V của A trong U sao cho $h|V =g|V$; một phần tử như vậy là một ánh xạ liên tục $H: E_0\times \mathbf{I}\rightarrow E_u$, tương thích với các phép toán của G và sao cho $H(x,0) =g_0(x)$, $H(x,1) =g_1(i(x))$ với mọi $x\in E_0$. Khi đó tồn tại một ánh xạ $h': B\times \mathbf{I}\rightarrow B_u$ sao cho $h'(p_0(x), t) =p_u(H(x, t))$ với $x\in E_0$ và $t\in \mathbf{I}$; ánh xạ này liên tục, và nó là một đồng luân nối $f_0$ với $f_1$.

#### Hệ quả {#ta-iv-s6-n4-cor-1 .statement tag=024I}

Cho G là một nhóm tôpô, cho B và $B'$ là các không gian tôpô paracompact. Cho $(E, p)$ và $(E', p')$ là các không gian sợi chính với nhóm G và lần lượt có cơ sở B và $B'$. Giả sử các không gian E và $E'$ đều đồng luân với một điểm. Các không gian B và $B'$ đồng luân.

Thật vậy, tồn tại một ánh xạ liên tục $f: B\rightarrow B'$ sao cho không gian sợi chính E đẳng cấu với không gian sợi chính $f^*E'$ và một ánh xạ liên tục $g: B'\rightarrow B$ sao cho không gian sợi chính $E'$ đẳng cấu với không gian sợi chính $g^*E$ (Định lý 1, a)). Khi đó các không gian sợi chính $(g\circ f)^*E$ và E đẳng cấu, do đó ánh xạ $g\circ f$ đồng luân với ánh xạ Id$_B$ (Định lý 1, b)). Tương tự, ánh xạ $f\circ g$ đồng luân với ánh xạ Id$_{B'}$.

Cho G là một nhóm tôpô, cho B là một không gian tôpô và cho E là một không gian sợi chính với nhóm G và có cơ sở B. Giả sử không gian E đồng luân với một điểm. Ta nói rằng không gian sợi chính E là phổ quát đối với các không gian sợi chính với nhóm G và cơ sở paracompact, và ta nói rằng không gian B là một không gian phân loại đối với G. Nếu hai không gian phân loại đối với G là paracompact, thì chúng đồng luân. Khi tồn tại một không gian phân loại, việc nghiên cứu các lớp đẳng cấu của các không gian sợi chính với nhóm G và cơ sở paracompact có thể được xem như một bài toán đồng luân.

#### Ví dụ {#ta-iv-s6-n4-exa-1 .statement tag=024J}

Được trang bị ánh xạ $p:\mathbf{R}\rightarrow \mathbf{S}^1,t\mapsto e^{2\pi it}$, và với phép toán của $\mathbf{Z}$ bằng phép tịnh tiến, không gian $\mathbf{R}$ là một không gian phủ chính với nhóm $\mathbf{Z}$. Do đó, không gian $\mathbf{S}^1$ là một không gian phân loại cho nhóm $\mathbf{Z}$.

Với mọi nhóm rời rạc G, trong số tiếp theo ta sẽ xây dựng một không gian mêtric được, là một không gian phân loại cho G.

### 5. Không gian phân loại cho một nhóm rời rạc

Cho G là một nhóm tôpô; ký hiệu $e$ là phần tử đơn vị của nó. Gọi $G^*$ là tập hợp các ánh xạ $h: [0,1[\rightarrow G$ sao cho tồn tại một dãy hữu hạn $(t_i)_{0\leqslant i\leqslant n}$ với $0 =t_0< t_1<\cdots < t_n= 1$ sao cho $h$ là hằng trên các khoảng $[t_{i-1}, t_i[$ với $1\leqslant i\leqslant n$. Một dãy như vậy được gọi là thích nghi với $h$. Với mọi tập con hữu hạn của $G^*$, tồn tại một dãy thích nghi với từng phần tử của nó.

Tập hợp $G^*$ là một nhóm con của $G^{[0,1[}$. Ký hiệu $e^*$ là phần tử đơn vị của nó; nghịch đảo của một phần tử $h\in G^*$ là ánh xạ $t\mapsto$ $h(t)^{-1}$, ký hiệu là $h^{-1}$.

Cho V là một lân cận của $e$ trong G. Cho $h\in G^*$ và $(t_i)_{0\leqslant i\leqslant n}$ là một dãy thích nghi với $h$. Tập hợp các phần tử $t\in [0,1[$ sao cho $h(t)\notin V$ là hợp của một số khoảng $[t_{i-1}, t_i[$; tổng các độ dài $t_i-t_{i-1}$ của các khoảng này không phụ thuộc vào dãy $(t_i)_{0\leqslant i\leqslant n}$ được chọn; ký hiệu nó là $p_V(h)$. Với mọi số thực $\varepsilon$ sao cho $\varepsilon  >0$, ta ký hiệu $V^*_{\varepsilon}$ là tập hợp các $h\in G^*$ sao cho $p_V(h)< \varepsilon$.

#### Mệnh đề 5 {#ta-iv-s6-prop-5 .statement tag=024K}

Tồn tại duy nhất một tôpô trên $G^*$ tương thích với cấu trúc nhóm của nó, trong đó các tập hợp $V^*_{\varepsilon}$ tạo thành một cơ sở các lân cận của phần tử đơn vị.

Ta hãy kiểm tra rằng các tập hợp $V_{\varepsilon}^*$ thỏa mãn các tiên đề (GV$'_I$), (GV$'_{II}$) và (GV$'_{III}$) của TG, III, p. 4.

Cho V là một lân cận của $e$ trong G và cho $\varepsilon$ là một số thực dương ngặt. Cho W là một lân cận của $e$ trong G sao cho $W\cdot W\subset V$. Cho $h$ và $h'$ là các phần tử của $G^*$. Nếu $t\in [0,1[$ sao cho $h(t)h'(t)\notin V$, thì $h(t)\notin W$ hoặc $h'(t)\notin W$. Do đó, $p_V(hh')\leqslant p_W(h)+p_W(h')$. Do đó, $W^*_{\varepsilon /2}\cdot W^*_{\varepsilon /2}\subset V^*_{\varepsilon}$, điều này chứng minh tiên đề (GV$'_I$).

Cho W là một lân cận của $e$ trong G sao cho $W^{-1}\subset V$. Khi đó $(W^*_{\varepsilon})^{-1}=$ $(W^{-1})^*_{\varepsilon}\subset V^*_{\varepsilon}$, do đó tiên đề (GV$'_{II}$).

Cho $k$ là một phần tử của $G^*$; vì hàm $k$ chỉ nhận một số hữu hạn giá trị, tồn tại một lân cận W của $e$ trong G sao cho $k(t)Wk(t)^{-1}\subset V$ với mọi $t\in [0,1[$. Khi đó, cho $h$ là một phần tử của $G^*$. Với $t\in [0,1[$, nếu $k(t)h(t)k(t)^{-1}\notin$ V, thì $h(t)\notin W$. Do đó, $p_V(khk^{-1})\leqslant p_W(h)$. Điều này chứng minh rằng $kW^*_{\varepsilon}k^{-1}\subset V^*_{\varepsilon}$, do đó tiên đề (GV$'_{III}$).

#### Mệnh đề 6 {#ta-iv-s6-prop-6 .statement tag=024L}

Không gian $G^*$ là co rút được và co rút được địa phương tại mỗi điểm của nó.

Với $h\in G^*$ và $t\in \mathbf{I}$, ta ký hiệu bởi $\sigma (h, t)$ ánh xạ của $[0,1[$ vào G được xác định bởi $\sigma (h, t)(x) =h(x)$ nếu $0\leqslant x < t$ và $\sigma (h, t) =e$ trong trường hợp ngược lại.

Hãy chứng minh rằng ánh xạ $\sigma : G^*\times \mathbf{I}\rightarrow G^*$ thu được là liên tục. Thật vậy, cho $k\in G^*,u\in \mathbf{I}$, cho V là một lân cận của $e$ trong G và cho $\varepsilon$ là một số thực dương ngặt. Phần tử $\sigma (h, t)\sigma (k, u)^{-1}$ của $G^*$ là ánh xạ $f$ của $[0,1[$ vào G được xác định bởi

$h(x)k(x)^{-1}$ if $0\leqslant x <$ min($t, u$) ;

$h(x)$ if $u\leqslant x < t$;

$$
f(x) =
$$

$k(x)^{-1}$ if $t\leqslant x < u$;

$e$ otherwise.

Do đó,

$$
p_V(\sigma (h, t)\sigma (k, u)^{-1})\leqslant p_V(hk^{-1}) +|t-u|
$$

nói cách khác, để có $\sigma (h, t)\in V^*_{\varepsilon}\sigma (k, u)$, chỉ cần có $|t-u|\leqslant \frac{\varepsilon}{2}$ và $h\in V^*_{\varepsilon /2}k$, điều này chứng minh tính liên tục của $\sigma$ tại $(k, u)$.

Với mọi $h\in G^*,\sigma (h,0)$ là ánh xạ hằng có ảnh $\{e\}$, trong khi $\sigma (h,1) =h$. Hơn nữa, $\sigma (e, t) =e$ với mọi $t\in \mathbf{I}$. Do đó, $\sigma$ là một phép đồng luân có điểm tại $e\in G^*$ nối ánh xạ hằng có ảnh $\{e\}$ với ánh xạ đồng nhất của $G^*$. Điều này chứng minh rằng $G^*$ co rút được tại $e^*$.

Hơn nữa, với mọi lân cận V của $e$ trong G và mọi số thực $\varepsilon  >0$, ta có $\sigma (V^*_{\varepsilon}\times \mathbf{I})\subset V^*_{\varepsilon}$. Do đó $V^*_{\varepsilon}$ cũng co rút được tại $e^*\in$ $G^*$, và vì vậy $G^*$ co rút được địa phương tại $e^*$.

Vì $G^*$ là một nhóm tôpô, nó co rút được và co rút được địa phương tại mỗi điểm của nó.

Gọi $\iota$ là ánh xạ từ G vào $G^*$ gán cho $g\in G$ ánh xạ hằng có ảnh $\{g\}$ của $[0,1[$ vào G. Ánh xạ $\iota$ là một đơn cấu đồng cấu của các nhóm. Gọi V là một lân cận của $e$ trong G và gọi $\varepsilon$ là một số thực dương ngặt. Ta có $\overset{-1}{\iota}(V^*_{\varepsilon}) = V$ nếu $\varepsilon \leqslant 1$ và $\overset{-1}{\iota}(V^*_{\varepsilon}) = G$ trong trường hợp ngược lại. Ảnh ngược của một lân cận của phần tử đơn vị của $G^*$ là một lân cận của phần tử đơn vị của G, do đó $\iota$ liên tục. Hơn nữa, $\iota (V) = V^*_1\cap \iota (G)$ với mọi lân cận V của $e$ trong G. Do đó $\iota$ xác định một đẳng cấu của các nhóm tôpô từ G lên ảnh của nó.

#### Nhận xét 1 {#ta-iv-s6-n5-rem-1 .statement tag=024M}

Nếu G là một nhóm tôpô tách được, $\iota (G)$ là đóng trong $G^*$.

Thật vậy, giả sử $h\in G^*$ sao cho $h\notin \iota (G)$, gọi $(t_i)_{0\leqslant i\leqslant n}$ là một dãy thích nghi với $h$, đặt $\varepsilon =$ min$_{1\leqslant i\leqslant n}(t_i-t_{i-1})$. Gọi V là một lân cận của $e$ trong G sao cho $h(t_i)^{-1}h(t_j)\notin V$, với mọi cặp $(i, j)$ các số nguyên sao cho $0\leqslant i, j\leqslant n-1$ và $h(t_i)=\not h(t_j)$; tồn tại một lân cận như vậy vì G là tách được. Gọi W là một lân cận của $e$ trong G sao cho $W\cdot W^{-1}\subset V$. Ta chứng minh rằng khi đó $hW^*_{\varepsilon}$ không gặp $\iota (G)$.

Hãy lập luận bằng phản chứng. Cho $f$ là một phần tử của $W^*_{\varepsilon}$ và $g$ là một phần tử của G sao cho $hf$ = $\iota (g)$. Do đó ta có $f(t) =h(t)^{-1}g$ với mọi $t\in [0,1[$, vì vậy dãy $(t_i)$ cũng thích nghi với hàm $f$. Nếu giá trị mà $f$ nhận trên khoảng $[t_{i-1}, t_i[$ không thuộc W, thì $t_i-t_{i-1}< \varepsilon$, vì $f\in W^*_{\varepsilon}$. Bất đẳng thức này là sai, theo định nghĩa của $\varepsilon$, ta có $f(t)\in W$ với mọi $t\in [0,1[$. Khi đó, cho $i$ và $j$ là các phần tử của $\{0, . . . , n-1\}$ sao cho $h(t_i)=\not h(t_j)$; ta có

$$
h(t_i)^{-1}h(t_j) =f(t_i)g^{-1}gf(t_j)^{-1}=f(t_i)f(t_j)^{-1}\in W\cdot W^{-1}
$$

điều này mâu thuẫn với lựa chọn của W. Nhóm con $\iota (G)$ của $G^*$ do đó là đóng.

Giả sử rằng G là một nhóm tôpô mêtric được và cho $d$ là một khoảng cách trên G xác định tôpô của nó. Cho $h$ và $h'\in G^*$ và cho $(t_i)_{0\leqslant i\leqslant n}$ là một dãy thích nghi với $h$ và $h'$. Số thực

$$
\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), h'(t_{i-1}))
$$

không phụ thuộc vào dãy $(t_i)$ được chọn; ta ký hiệu nó là $d^*(h, h')$.

Hãy chứng minh rằng $d^*$ là một khoảng cách trên $G^*$. Ta có $d^*(h, h') =$ $d^*(h', h)$ với $h,h'\in G^*$, và $d^*(h, h) = 0$ với mọi $h\in G^*$. Ngược lại, cho $h$ và $h'$ là các phần tử của $G^*$ sao cho $d^*(h, h') = 0$. Cho $(t_i)_{0\leqslant i\leqslant n}$ là một dãy thích nghi với $h$ và $h'$. Vì

$$
0 =d^*(h, h') =\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), h'(t_{i-1}))
$$

và mọi số hạng của tổng này đều dương hoặc bằng không, ta có $d(h(t_{i-1}), h'(t_{i-1})) = 0$ với mọi $i\in  \{1, . . . , n\}$, do đó $h=h'$. Cuối cùng, cho $h,h',h''$ là các phần tử của $G^*$ và cho $(t_i)_{0\leqslant i\leqslant n}$ là một dãy thích nghi với mỗi phần tử trong số chúng. Khi đó,

$$
d^*(h, h'') =\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), h''(t_{i-1}))
$$

$$
\leqslant \sum_{i=1}^n(t_i-t_{i-1})(d(h(t_{i-1}), h'(t_{i-1}))+d(h(t_{i-1}), h''(t_{i-1})))
$$

$$
=d^*(h, h') +d^*(h, h'')
$$

do đó $d^*$ thỏa mãn bất đẳng thức tam giác.

Khoảng cách $d^*$ này là bất biến qua các phép tịnh tiến phải (tương ứng, trái) nếu $d$ là như vậy.

#### Mệnh đề 7 {#ta-iv-s6-prop-7 .statement tag=024N}

Giả sử rằng G là một nhóm tôpô mêtric hóa được. Khi đó nhóm tôpô $G^*$ là mêtric hóa được. Chính xác hơn, nếu $d$ là một khoảng cách bị chặn trên G xác định tôpô của nó, thì tôpô của $G^*$ được xác định bởi khoảng cách $d^*$.

Cho $d$ là một khoảng cách trên G xác định tôpô của nó. Khi đó, ánh xạ $d'$ cho bởi $d'(h, h') =$ inf($d(h, h'),1$) là một khoảng cách bị chặn trên G cũng xác định tôpô của nó (TG, IX, p. 3). Do đó chỉ cần chứng minh rằng $d^*$ xác định tôpô của $G^*$ dưới giả thiết rằng $d$ bị chặn.

Cho V là một lân cận của $e$ trong G và cho $\varepsilon$ là một số thực dương ngặt. Cho $\delta$ là một số thực dương ngặt sao cho V chứa hình cầu $B(e, \delta )$. Cho $h\in G^*$ và cho $(t_i)_{0\leqslant i\leqslant n}$ là một dãy thích nghi với $h$. Khi đó,

$$
p_V(h) =\sum_{h(t_ii_-=1_1)\notin V}^n(t_i-t_{i-1})
$$

$$
\leqslant \sum^n(t_i-t_{i-1})\frac{d(h(t_{i-1}), e)}{\delta}
$$

$$
i=1
$$

$d(h(t_{i-1}),e)\geqslant \delta$

$$
\leqslant \frac{d^*(h, e^*)}{\delta}
$$

Do đó, hình cầu $B(e^*, \varepsilon \delta )$ trong $G^*$ được chứa trong $V_{\varepsilon}^*$.

Ngược lại, cho $\delta$ là một số thực dương ngặt và cho Δ là một cận trên dương ngặt của đường kính của G. Cho V là một lân cận của $e$ trong G được chứa trong hình cầu $B(e, \delta /2)$. Với một hàm $h\in G^*$ và một dãy $(t_i)_{0\leqslant i\leqslant n}$ thích nghi với $h$, ta có

$$
d^*(h, e^*) =\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), e)
$$

= $\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), e)$

$d(h(t_{i-1}),e)\leqslant \delta /2$

+ $\sum_{i=1}^n(t_i-t_{i-1})d(h(t_{i-1}), e)$

$d(h(t_{i-1}),e)>\delta /2$

$\leqslant \frac{\delta}{2}+ \Delta \sum_{i=1}^n(t_i-t_{i-1})$

$h(t_{i-1})\notin V$

$$
\leqslant \frac{\delta}{2}+ \Delta p_V(h)
$$

Bất đẳng thức trước đó suy ra rằng, với mọi phần tử $h$ của $V_{\delta /2\Delta}^*$, ta có $d^*(h, e^*)\leqslant \delta$. Do đó, mọi hình cầu của $G^*$ đối với khoảng cách $d^*$ đều chứa một lân cận của phần tử đơn vị.

#### Nhận xét 2 {#ta-iv-s6-n5-rem-2 .statement tag=024O}

Cho $d$ là một khoảng cách bị chặn xác định tôpô của G. Khi nhóm tôpô $G^*$ được trang bị khoảng cách $d^*$, đồng cấu $\iota : G\rightarrow G^*$ là một đẳng cự.

#### Nhận xét 3 {#ta-iv-s6-n5-rem-3 .statement tag=024P}

Giả sử rằng G là một nhóm tôpô rời rạc. Nhóm con $\iota (G)$ khi đó là một nhóm con rời rạc của $G^*$. Thật vậy, tôpô của G được xác định bởi khoảng cách $d$ trên G cho bởi $d(g, g') = 1$ nếu $g=\not g'$ và $d(g, g') = 0$ nếu không. Mệnh đề đó suy ra từ nhận xét trước đó.

#### Định lý 2 {#ta-iv-s6-thm-2 .statement tag=024Q}

Cho G là một nhóm tôpô rời rạc. Cho G tác động bên phải trên $G^*$ bởi $h\cdot g=h\iota (g)$ và cho B ký hiệu không gian tôpô thương $G^*/G$.

Không gian $G^*$ là một phép phủ chính của B với nhóm G; nó liên thông đơn theo đường.

Không gian B là một không gian tôpô mêtric hóa được, liên thông theo đường, co được địa phương, và nhóm Poincaré của nó tại mọi điểm là đẳng cấu với G.

Do đó, không gian B là một không gian phân loại cho nhóm G.

Nhóm $G^*$ co được về phần tử đơn vị của nó (IV, p. 450, prop. 6). Đặc biệt nó liên thông theo đường (III, p. 260) và liên thông đơn theo đường (IV, p. 340).

Nhóm $\iota (G)$ là đóng trong $G^*$ (TG, III, p. 7, prop. 5), do đó không gian $G^*/G$ là khả mêtric (TG, III, p. 13, prop. 18 và TG, IX, p. 25, prop. 4). Nó cũng liên thông bằng cung (III, p. 258, prop. 3). Vì nhóm $\iota (G)$ là rời rạc, theo hệ quả 2 của I, p. 100, ta có $G^*$ là một phép phủ G chính của B. Khi đó, phép phủ có điểm đánh dấu $(G^*, e^*)$ là một phép phủ phổ quát của không gian B được đánh dấu tại ảnh của $e^*$; nhóm Poincaré của B (tại mỗi điểm của nó) là đẳng cấu với G.

## BÀI TẬP {#ta-iv-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).
