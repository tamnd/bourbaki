---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 2
section_title: Applications étales
lang: vi
source: ta-i-iv-fr
book_pages: TA I.25-TA I.42, TA I.140-TA I.141
pdf_pages: 0041-0058, 0156-0157
extraction: native
subsections:
    - "no": 1
      title: Applications séparées
      page: 25
      pdf_page: 41
    - "no": 2
      title: Applications étales
      page: 28
      pdf_page: 44
    - "no": 3
      title: Sections locales des applications étales
      page: 32
      pdf_page: 48
    - "no": 4
      title: Relèvements continus des applications étales
      page: 33
      pdf_page: 49
    - "no": 5
      title: Construction de sections continues d’applications étales
      page: 35
      pdf_page: 51
    - "no": 6
      title: Majoration du cardinal des fibres d’une application étale et séparée
      page: 40
      pdf_page: 56
statements: 47
exercises: 7
content_sha256: 4abf035357f6193eaf351616a36bb188cafc3e0dc365ce637da8108e166f8942
translated_from: content/en-mt/ta/I/02_s2_applications_etales.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 87d728a77058cb1073bd8346d18c7e5ba69f05eb6a61904c13c511f71918bf39
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-92226984
glossary_version: 34
glossary_terms_sha256: dc6f82d0137ed2bdd744a790aafacc4b840ef330a45075b3b90c08f847589822
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ÁNH XẠ ÉTALE

### 1. Ánh xạ tách

#### Mệnh đề 1 {#ta-i-s2-prop-1 .statement tag=01MH}

Cho X và Y là các không gian tôpô và cho $f: X\rightarrow$ Y là một ánh xạ liên tục. Các tính chất sau là tương đương:

(i) Đường chéo $\Delta_X$ của tích thớ $X\times_YX$ là một không gian con đóng;

(ii) Với mọi không gian tôpô W và mọi cặp ánh xạ liên tục $(g_1, g_2)$ từ W vào X sao cho $f\circ g_1=f\circ g_2$, tập hợp các điểm $w\in W$ sao cho $g_1(w) =g_2(w)$ là đóng trong W;

(iii) Với mọi cặp $(x_1, x_2)$ các điểm của X sao cho $x_1=\not x_2$ và $f(x_1) =f(x_2)$, tồn tại một lân cận $V_1$ của $x_1$ trong X và một lân cận $V_2$ của $x_2$ trong X sao cho $V_1\cap V_2=\emptyset$.

(i)$\Rightarrow$(ii) : Cho $g_1,g_2$ là các ánh xạ liên tục từ W vào X sao cho $f\circ g_1=f\circ g_2$, và cho $g: W\rightarrow X\times_YX$ là ánh xạ suy ra từ $g_1$ và $g_2$. Tập hợp các điểm $w\in W$ sao cho $g_1(w) =g_2(w)$ là $\overset{-1}{g}(\Delta_X)$. Vì $g$ liên tục, do đó nó là đóng nếu đường chéo $\Delta_X$ là đóng.

(ii)$\Rightarrow$(i) : Đường chéo $\Delta_X$ là tập hợp các điểm $z\in X\times_YX$ sao cho pr$_1(z) =$ pr$_2(z)$. Suy ra từ (ii) áp dụng cho $W = X\times_YX$ và cho cặp ánh xạ (pr$_1$, pr$_2$) rằng đường chéo $\Delta_X$ là đóng trong $X\times_YX$.

(i)$\Leftrightarrow$(iii) : Cho $(x_1, x_2)$ là một điểm của $X\times_YX$ và cho $V_1$ và $V_2$ lần lượt là các lân cận của $x_1$ và $x_2$. Điều kiện $V_1\cap V_2=\emptyset$ tương đương với điều kiện $(V_1\times V_2)\cap \Delta_X=\emptyset$, tức là, với $(V_1\times V_2)\cap$ $(X\times_YX)\cap \Delta_X=\emptyset$. Vì các tập hợp $(V_1\times V_2)\cap (X\times_YX)$ tạo thành một cơ sở các lân cận của $(x_1, x_2)$ trong $X\times_YX$, điều này chứng minh tính tương đương của (i) và (iii).

#### Định nghĩa 1 {#ta-i-s2-def-1 .statement tag=01MI}

Cho X và Y là các không gian tôpô. Một ánh xạ liên tục $f: X\rightarrow Y$ được gọi là tách nếu nó thỏa mãn các điều kiện tương đương của mệnh đề 1.

#### Mệnh đề 2 {#ta-i-s2-prop-2 .statement tag=01MJ}

Cho X, Y, Z là các không gian tôpô và cho $f: X\rightarrow Y$ và $g: Y\rightarrow Z$ là các ánh xạ liên tục.

a) Nếu $f$ và $g$ là tách, thì $g\circ f$ là tách.

b) Nếu $g\circ f$ là tách, thì $f$ là tách.

c) Hơn nữa, giả sử ánh xạ $f$ là thực sự và toàn ánh. Khi đó, nếu $g\circ f$ là tách, thì $g$ là tách.

Xét, trong $X\times X$, các không gian con $\Delta_X$ (đường chéo), $X\times_YX$ và $X\times_ZX$. Chúng lần lượt là các tập hợp các điểm $u$ của $X\times X$ sao cho pr$_1(u) =$ pr$_2(u),f\circ$pr$_1(u) =f\circ$pr$_2(u),g\circ f\circ$pr$_1(u) =g\circ f\circ$pr$_2(u)$. Nếu $g\circ f$ là tách, thì $\Delta_X$ đóng trong $X\times_ZX$, do đó cũng đóng trong $X\times_YX$, do đó b).

Theo mệnh đề 1, (ii), áp dụng cho $W = X\times_ZX,g_1=f\circ$ pr$_1$ và $g_2=f\circ$ pr$_2,X\times_YX$ đóng trong $X\times_ZX$ nếu $g$ là tách. Hơn nữa, nếu $f$ là tách, thì $\Delta_X$ đóng trong $X\times_YX$ (mệnh đề 1, (i)), do đó trong $X\times_ZX$, do đó a).

Cuối cùng, ta chứng minh c). Ánh xạ $(f, f): X\times X\rightarrow Y\times Y$ là thực sự (TG, I, p. 73, mệnh đề 4). Không gian con $X\times_ZX$ là ảnh ngược của $Y\times_ZY$ qua $(f, f)$; theo TG, I, p. 72, mệnh đề 3, ánh xạ $u: X\times_Z$ $X\rightarrow Y\times_ZY$ suy ra từ $(f, f)$ là thực sự. Vì $g\circ f$ là tách, đường chéo $\Delta_X$ đóng trong $X\times_ZX$. Do đó, $u(\Delta_X)$ đóng trong $Y\times_ZY$. Vì $f$ toàn ánh, $u(\Delta_X)$ là đường chéo của $Y\times_ZY$. Điều này chứng tỏ rằng $g$ là tách.

#### Nhận xét 1 {#ta-i-s2-n1-rem-1 .statement tag=01MK}

Một ánh xạ liên tục đơn ánh là tách.

#### Nhận xét 2 {#ta-i-s2-n1-rem-2 .statement tag=01ML}

Đối với một không gian tôpô X, để X là tách (TG, I, p. 52, định nghĩa 1), điều kiện cần và đủ là ánh xạ của X vào một không gian thu gọn về một điểm là tách. Trong trường hợp này, mọi ánh xạ liên tục từ X vào một không gian tôpô đều là tách (mệnh đề 1, (iii)).

Cho $f: X\rightarrow$ Y là một ánh xạ liên tục và tách. Với mọi điểm $y$ của Y, thớ $\overset{-1}{f}(y)$ là một không gian tôpô tách (loc. cit.). Tuy nhiên, tồn tại những ánh xạ liên tục không tách mà mọi thớ của chúng đều là những không gian tôpô tách (I, p. 140, bài tập 1).

#### Nhận xét 3 {#ta-i-s2-n1-rem-3 .statement tag=01MM}

Cho $f: X\rightarrow Y$ là một ánh xạ liên tục và tách. Nếu không gian Y là tách, thì không gian X là tách. Điều này suy ra từ nhận xét 2 và mệnh đề 2 được áp dụng với một không gian Z thu gọn về một điểm.

#### Nhận xét 4 {#ta-i-s2-n1-rem-4 .statement tag=01MN}

Cho $f: X\rightarrow Y$ là một ánh xạ liên tục và tách, $y$ một điểm

của Y và A là một tập con hữu hạn của $\overset{-1}{f}(y)$. Ta hãy chỉ ra rằng tồn tại một họ $(V_a)_{a\in A}$ gồm các tập rời nhau từng đôi một sao cho với mỗi $a\in A$, tập $V_a$ là một lân cận của $a$ trong X. Vì vậy, với mỗi tập con $\{a, b\}$ của A có hai phần tử, ta chọn một lân cận $V_{(a,b)}$ của $a$ và một lân cận $V_{(b,a)}$ của $b$ trong X sao cho $V_{(a,b)}\cap V_{(b,a)}=\emptyset$ (mđ. 1, (iii)). Gọi $V_a$ là giao của họ gồm X và các tập $V_{(a,b)}$ với $b\in A,b=\not a$. Tập $V_a$ là một lân cận của $a$ trong X, và nếu $a,b$ là hai phần tử phân biệt của A, tập $V_a\cap V_b$ được chứa trong $V_{(a,b)}\cap V_{(b,a)}$, do đó là rỗng.

#### Nhận xét 5 {#ta-i-s2-n1-rem-5 .statement tag=01MO}

Cho Y là một không gian tôpô. Cho $(A_i)_{i\in I}$ là một họ các tập con của Y và X là không gian tổng của họ $(A_i)_{i\in I}$. Ánh xạ chính tắc của X vào Y là tách được.

#### Mệnh đề 3 {#ta-i-s2-prop-3 .statement tag=01MP}

Cho $f: X\rightarrow Y$ là một ánh xạ liên tục và tách được. Mọi tiết diện liên tục của $f$ cảm sinh một phép đồng phôi của Y lên một tập con đóng của X.

Cho $s: Y\rightarrow X$ là một tiết diện liên tục của $f$. Ánh xạ $s$ cảm sinh một phép đồng phôi của Y lên không gian con $s(Y)$ của X (TG, I, p. 22, mđ. 9). Ánh xạ đồng nhất của X và ánh xạ $s\circ f$ là liên tục và ta có $f\circ$ Id$_X=f\circ (s\circ f)$. Vì ánh xạ $f$ là tách được, tập $s(Y)$, là tập các điểm $x$ của X sao cho $x=s\circ f(x)$, là đóng trong X (mđ. 1, (ii)).

#### Mệnh đề 4 {#ta-i-s2-prop-4 .statement tag=01MQ}

Cho

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

là một bình phương Descartes. Nếu ánh xạ $p$ là tách được, điều tương tự cũng đúng với $p'$. Ngược lại, nếu $p'$ là tách được và nếu $f$ là ngặt phổ quát và toàn ánh, thì $p$ là tách được.

Xét bình phương

$$
X'\times_{B'}{X'}^{\varphi}X\times_BX
$$

$q'q$

${B'}^f$ B

trong đó ánh xạ $\varphi$ được cảm sinh bởi ánh xạ $f'\times f': X'\times X'\rightarrow X\times X$. Nhắc lại (I, p. 13, ví dụ 1) rằng bình phương này là Descartes và ta có $\overset{-1}{\varphi}(\Delta_X) = \Delta_{X'}$.

Nếu ánh xạ $p$ là tách được, tập $\Delta_X$ là đóng trong $X\times_BX$; do đó, $\Delta_{X'}$ là một tập con đóng của $X'\times_{B'}X'$, điều này chứng minh rằng ánh xạ $p'$ là tách được.

Nếu ánh xạ $f$ là toàn ánh, ánh xạ $\varphi$ là toàn ánh (I, p. 10, cor.) ; nếu $f$ là ngặt phổ quát, $\varphi$ là ngặt (I, p. 20, def. 6). Giả sử ánh xạ $p'$ tách được. Khi đó $\Delta_{X'}$ là đóng trong $X'\times_{B'}X'$. Vì $\Delta_{X'}=\overset{-1}{\varphi}(\Delta_X)$ và vì $\varphi$ là toàn ánh và ngặt, $\Delta_X$ là đóng trong $X\times_BX$, điều này chứng minh rằng ánh xạ $p$ tách được.

#### Mệnh đề 5 {#ta-i-s2-prop-5 .statement tag=01MR}

Cho X, Y, Z là các không gian tôpô và $f: X\rightarrow Y,g: Y\rightarrow Z$ là các ánh xạ liên tục. Giả sử ánh xạ $g$ tách được và ánh xạ $g\circ f$ là thực sự. Khi đó ánh xạ $f$ là thực sự.

Xét bình phương Descartes sau:

$X\times_ZY^{pr_2}$ Y

pr$_1g$

X $^{g\circ f}Z$.

Gọi $s: X\rightarrow X\times_ZY$ là ánh xạ $x\mapsto (x, f(x))$. Nó là một tiết diện liên tục của pr$_1: X\times_ZY\rightarrow X$. Theo mệnh đề 4, ánh xạ pr$_1$ tách được; suy ra ánh xạ $s$ là thực sự (I, p. 27, prop. 3 và TG, I, p. 72, prop. 2). Mặt khác, ánh xạ pr$_2$ là thực sự (I, p. 17, prop. 8). Do đó ánh xạ $f$, bằng pr$_2\circ s$, là thực sự (TG, I, p. 73, prop. 5).

### 2. Các ánh xạ étale

#### Định nghĩa 2 {#ta-i-s2-def-2 .statement tag=01MS}

Cho E và B là các không gian tôpô, cho $p: E\rightarrow B$ là một ánh xạ và $x$ là một điểm của E. Ta nói rằng ánh xạ $p$ là étale tôpô tại $x$ nếu tồn tại một lân cận U của $x$ trong E và một lân cận V của $p(x)$ trong B sao cho $p$ cảm sinh một phép đồng phôi từ U lên V.

Ta nói rằng ánh xạ $p$ là étale tôpô nếu nó étale tôpô tại mọi điểm $x$ của E.

Khi không thể có nhầm lẫn, cf. ví dụ 3 dưới đây, ta sẽ nói étale thay cho étale tôpô. Thay vì nói rằng $p: E\rightarrow B$ là một ánh xạ étale, người ta cũng nói rằng B-không gian $(E, p)$ là một B-không gian étale, hoặc đơn giản E là một không gian trải trên B, khi không có nghi ngờ nào về ánh xạ $p$.

#### Nhận xét 1 {#ta-i-s2-n2-rem-1 .statement tag=01MT}

Tập hợp các điểm của E tại đó một ánh xạ $p: E\rightarrow B$ là étale là một tập mở U của E, và hạn chế của $p$ lên U là một ánh xạ étale từ U vào B.

#### Nhận xét 2 {#ta-i-s2-n2-rem-2 .statement tag=01MU}

Một ánh xạ étale là liên tục và mở (TG, I, p. 33, prop. 5) ; đặc biệt, ảnh của một ánh xạ étale là mở. Ngược lại, nếu $p: E\rightarrow B$ là một ánh xạ liên tục và mở, và nếu mọi điểm $x$ của E có một lân cận V sao cho ánh xạ $p|V$ là đơn ánh, thì ánh xạ $p$ là étale. Các thớ của một ánh xạ étale là rời rạc.

#### Ví dụ 1 {#ta-i-s2-n2-exa-1 .statement tag=01MV}

Cho B là một không gian tôpô và $(U_i)_{i\in I}$ là một họ các tập con của B. Gọi E là không gian tổng của họ $(U_i)_{i\in I}$ và $p: E\rightarrow B$ là ánh xạ suy ra từ các phép nhúng chính tắc của các $U_i$ vào B. Để ánh xạ $p$ là étale, điều kiện cần và đủ là các $U_i,i\in I$, đều mở.

#### Ví dụ 2 {#ta-i-s2-n2-exa-2 .statement tag=01MW}

Cho U là một tập mở của $\mathbf{C}$. Để một hàm chỉnh hình $f: U\rightarrow \mathbf{C}$ là một ánh xạ étale, điều kiện cần và đủ là đạo hàm của nó không triệt tiêu ở đâu cả.

#### Ví dụ 3 {#ta-i-s2-n2-exa-3 .statement tag=01MX}

Một cấu xạ étale của các đa tạp (VAR, R, 5.7.8) là một ánh xạ étale tôpô, nhưng tồn tại các cấu xạ của các đa tạp thực là étale tôpô nhưng không phải là các cấu xạ étale. Chẳng hạn, đây là trường hợp của ánh xạ $x\mapsto x^3$ từ $\mathbf{R}$ vào $\mathbf{R}$. Tuy nhiên, một cấu xạ của các đa tạp giải tích phức mà étale tôpô thì là một cấu xạ étale (I, p. 141, exerc. 6).

#### Mệnh đề 6 {#ta-i-s2-prop-6 .statement tag=01MY}

Cho X, Y, Z là các không gian tôpô và $f: X\rightarrow Y,g: Y\rightarrow Z$ là các ánh xạ.

a) Giả sử rằng $f$ và $g$ là étale; khi đó $g\circ f$ là étale.

b) Giả sử rằng $g$ là étalé, $f$ liên tục và $g\circ f$ là mở. Khi đó $f$ là mở.

c) Giả sử rằng $g\circ f$ và $g$ là étalé và $f$ liên tục. Khi đó ánh xạ $f$ là étalé.

d) Giả sử rằng $g\circ f$ là étalé và ánh xạ $f$ liên tục và mở; khi đó $f$ là étalé và $g$ là étalé tại mọi điểm của $f(X)$.

Ta chứng minh a). Giả sử các ánh xạ $f$ và $g$ là étalé. Khi đó chúng liên tục và mở, do đó ánh xạ $g\circ f$ liên tục và mở. Cho $x$ là một điểm của X. Tồn tại một lân cận W của $f(x)$ trong Y sao cho ánh xạ $g|W$ đơn ánh, và một lân cận V của $x$

trong X, được chứa trong $\overset{-1}{f}(W)$, sao cho ánh xạ $f|V$ đơn ánh; khi đó ánh xạ $(g\circ f)|V$ đơn ánh. Điều này chứng minh rằng ánh xạ $g\circ f$ là étalé (nhận xét 2).

Ta chứng minh b). Cho $x$ là một điểm của X và W là một lân cận mở của $f(x)$ sao cho $g$ cảm sinh một phép đồng phôi từ W lên tập mở $g(W)$. Cho V là một lân cận của $x$ sao cho $f(V)$ được chứa trong W; khi đó $g\circ f(V)$ là một lân cận của $g\circ f(x)$, do đó $f(V)$ là một lân cận của $f(x)$ trong tập mở W, và cũng trong Y. Điều này chứng minh rằng ánh xạ $f$ là mở (TG, I, p. 33, mệnh đề 5).

Ta chứng minh c). Theo b$),f$ là mở. Cho $x$ là một điểm của X. Vì $g\circ f$ là étalé, tồn tại một lân cận V của $x$ trong X sao cho $g\circ f|V$ đơn ánh. Do đó, $f|V$ đơn ánh và $f$ là étalé (I, p. 29, nhận xét 2).

Ta chứng minh d). Cho $x$ là một điểm của X và đặt $y=f(x)$. Tồn tại một lân cận mở V của $x$ sao cho $g\circ f$ cảm sinh một phép đồng phôi từ V lên tập mở $g\circ f(V)$. Vì ánh xạ $f$ là mở, $f(V)$ là một lân cận mở của $y$. Ánh xạ $f|V: V\rightarrow f(V)$ suy ra từ $f$ bằng cách chuyển qua các không gian con là liên tục, mở và song ánh; do đó nó là một phép đồng phôi, vậy $f$ là étalé tại $x$. Hơn nữa, ánh xạ $g$ cảm sinh một phép đồng phôi từ $f(V)$ lên $g\circ f(V)$, do đó là étalé tại $y$.

#### Hệ quả 1 {#ta-i-s2-prop-6-cor-1 .statement tag=01MZ}

Cho B là một không gian tôpô. Một B-cấu xạ từ một B-không gian étalé vào một B-không gian étalé khác là étalé.

Điều này suy ra từ mệnh đề c) của mệnh đề 6.

#### Hệ quả 2 {#ta-i-s2-prop-6-cor-2 .statement tag=01N0}

Cho B là một không gian tôpô; một B-cấu xạ song ánh từ một B-không gian étalé vào một B-không gian étalé khác là một B-đẳng cấu.

Theo hệ quả 1, cấu xạ như vậy là étalé; do đó nó là mở (I, p. 29, nhận xét 2). Nếu nó song ánh, thì nó là một B-đẳng cấu.

#### Hệ quả 3 {#ta-i-s2-prop-6-cor-3 .statement tag=01N1}

Cho $p: E\rightarrow B$ là một ánh xạ étalé. Mọi tiết diện liên tục của $p$ đều cảm sinh một phép đồng phôi từ B lên một tập con mở của E.

Thật vậy, một tiết diện như vậy là étalé (hệ quả 1), do đó là mở.

#### Hệ quả 4 {#ta-i-s2-prop-6-cor-4 .statement tag=01N2}

Cho $p: E\rightarrow B$ là một ánh xạ étale và tách. Giả sử E liên thông và $p$ có một tiết diện. Khi đó $p$ là một đồng phôi.

Cho $s$ là một tiết diện của $p$; vì $p$ là étale, ảnh của $s$ là mở trong E (Hệ quả 3); nó cũng đóng, vì $p$ là tách (I, p. 27, Mệnh đề 3). Vì E liên thông, ta có $s(B) = E$ và $p$ là một đồng phôi.

#### Mệnh đề 7 {#ta-i-s2-prop-7 .statement tag=01N3}

Cho $p: E\rightarrow B$ là một ánh xạ liên tục. Để ánh xạ $p$ là étale, điều kiện cần và đủ là nó mở và đường chéo $\Delta_E$ của $E\times_BE$ mở trong $E\times_BE$.

Trước hết, giả sử ánh xạ $p$ là étale. Khi đó nó mở và mọi điểm của E đều có một lân cận V sao cho $p|V$ là đơn ánh, điều này tương đương với việc nói rằng ta có $(V\times V)\cap (E\times_BE)\subset \Delta_E$. Do đó $\Delta_E$ là một tập con mở của $E\times_BE$.

Ngược lại, giả sử $p$ là một ánh xạ mở và $\Delta_E$ là một tập con mở của $E\times_BE$. Cho $x$ là một điểm của E. Cho V là một lân cận mở của $x$ trong E sao cho $(V\times V)\cap (E\times_BE)$ được chứa trong $\Delta_E$. Khi đó $p|V$ là đơn ánh. Theo Nhận xét 2, I, p. 29, ánh xạ $p$ là étale.

#### Mệnh đề 8 {#ta-i-s2-prop-8 .statement tag=01N4}

Cho

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

là một bình phương Descartes. Nếu ánh xạ $p$ là étale, thì ánh xạ $p'$ là étale. Ngược lại, nếu ánh xạ $p'$ là étale và ánh xạ $f$ là ngặt phổ dụng và toàn ánh, thì ánh xạ $p$ là étale.

Giả sử ánh xạ $p$ là étale. Khi đó, đặc biệt, nó mở và $p'$ mở (I, p. 17, Mệnh đề 8). Xét bình phương Descartes (I, p. 13, Ví dụ 1)

$$
E'\times_{B'}{E'}^{\varphi}E\times_BE
$$

$q'q$

${B'}^fB$. Ta có $\Delta_{E'}=\overset{-1}{\varphi}(\Delta_E)$ (loc. cit.). Hơn nữa, đường chéo $\Delta_E$ mở trong $E\times_BE$ (Mệnh đề 7), do đó đường chéo $\Delta_{E'}$ mở trong $E'\times_{B'}E'$. Điều này chứng minh rằng ánh xạ $p'$ là étale (loc. cit.).

Bây giờ giả sử ánh xạ $f$ là toàn ánh và ngặt phổ dụng và ánh xạ $p'$ là étale. Khi đó $p'$ mở, do đó $p$ mở (I, p. 21, Mệnh đề 11, a)). Mặt khác $\Delta_{E'}$ là một tập con mở của $E'\times_{B'}E'$. Vì $\Delta_{E'}=\overset{-1}{\varphi}(\Delta_E)$ và ánh xạ $\varphi$ là toàn ánh và ngặt (I, p. 20, Định nghĩa 6), $\Delta_E$ mở trong $E\times_BE$. Theo Mệnh đề 7, ánh xạ $p$ là étale.

#### Hệ quả {#ta-i-s2-n2-cor-1 .statement tag=01N5}

Cho B là một không gian tôpô. Tích sợi của hai B-không gian étale là một B-không gian étale.

Cho $(E, p)$ và $(E', p')$ là các B-không gian étale. Ánh xạ pr$_1: E\times_B$ $E'\rightarrow E$ là étale (mệnh đề 8), do đó ánh xạ $p\circ$ pr$_1: E\times_BE'\rightarrow B$ là étale (mệnh đề 6, a)).

#### Nhận xét 3 {#ta-i-s2-n2-rem-3 .statement tag=01N6}

Cho

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

là một bình phương Descartes. Nếu ánh xạ $p$ là étale và ánh xạ $f$ là ngặt, thì ánh xạ $f'$ là ngặt. Thật vậy, dưới các giả thiết này, mọi điểm của E đều có một lân cận mở U sao cho $p$ cảm sinh một phép đồng phôi của U lên tập mở $p(U)$. Khi đó ánh xạ $p'$ cảm sinh

một phép đồng phôi của $(\overset{-1}{f}')(U)$ lên $\overset{-1}{f}(p(U))$. Ánh xạ $f$ cảm sinh

một ánh xạ ngặt từ $\overset{-1}{f}(p(U))$ lên $p(U)$ (I, p. 20) và ánh xạ

$f'$ do đó cảm sinh một ánh xạ ngặt từ $(\overset{-1}{f}')(U)$ vào U. Suy ra ánh xạ $f'$ là ngặt ( I, p. 23, hệ quả 2).

### 3. Tiết diện địa phương của các ánh xạ étale

Cho E và B là các tập hợp, A là một tập con của B và $p: E\rightarrow B$ là một ánh xạ. Một tiết diện của $p$ trên A (hoặc trên A) là một ánh xạ $s: A\rightarrow E$ sao cho $p\circ s$ là đơn ánh chính tắc của A vào B. Cho một tiết diện $s$ của $p$ trên A tương đương với việc cho một tiết diện của ánh xạ $p_A:\overset{-1}{p}(A)\rightarrow A$ suy ra từ $p$. Nếu $s$ là một tiết diện của $p$ trên A và $A'$ là một tập con của A, hạn chế $s'$ của $s$ trên $A'$ là một tiết diện của $p$ trên $A'$. Khi đó người ta nói rằng $s$ là một mở rộng của $s'$ lên A.

Khi E và B là các không gian tôpô và $p: E\rightarrow$ B là một ánh xạ liên tục, tập hợp $\mathscr{C}_B(A; E)$ (I, p. 2) các tiết diện liên tục của $p$ trên A cũng được ký hiệu là $\mathscr{S}(A;p)$ hoặc $\mathscr{S}(A; E)$. Cho $s$ là một tiết diện liên tục của $p$ trên A. Ánh xạ $s$ cảm sinh một phép đồng phôi của A lên $s(A)$, và $p$ cảm sinh phép đồng phôi ngược lại. Theo định nghĩa 2, I, p. 28, do đó ta có:

#### Mệnh đề 9 {#ta-i-s2-prop-9 .statement tag=01N7}

Cho $p: E\rightarrow B$ là một ánh xạ liên tục. Để ánh xạ $p$ là étale, điều kiện cần và đủ là mọi điểm của E đều có một lân cận mở là ảnh của một tiết diện liên tục của $p$ trên một tập con mở của B.

#### Nhận xét 1 {#ta-i-s2-n3-rem-1 .statement tag=01N8}

Cho $p: E\rightarrow B$ là một ánh xạ liên tục và mở. Để một tập mở U của E là ảnh của một tiết diện liên tục của $p$ trên một tập mở của B, điều kiện cần và đủ là hạn chế của $p$ trên U là đơn ánh.

#### Nhận xét 2 {#ta-i-s2-n3-rem-2 .statement tag=01N9}

Cho $p: E\rightarrow$ B là một ánh xạ liên tục. Giả sử mọi điểm của B đều có một lân cận mở V sao cho tồn tại một tiết diện liên tục của $p$ trên V. Một ánh xạ $p$ như vậy không nhất thiết là étale, thậm chí không nhất thiết là mở. Tuy nhiên, nó là toàn ánh và ngặt phổ quát (I, p. 20, hệ quả).

### 4. Các nâng liên tục của các ánh xạ étale

Cho $p: E\rightarrow B$ và $f: Z\rightarrow B$ là các ánh xạ liên tục. Một nâng liên tục của $f$ lên E là một ánh xạ liên tục $g: Z\rightarrow E$ sao cho $p\circ g=f$. Tập hợp các nâng liên tục của $f$ lên E không gì khác hơn là $\mathscr{C}_B(Z; E)$. Nó cũng được đồng nhất với tập hợp $\mathscr{S}(Z; Z\times_BE)$ các tiết diện liên tục của phép chiếu của không gian Z $(Z\times_BE$, pr$_1)$.

Nếu T là một tập con của Z, một nâng liên tục của $f$ lên E xác định trên T là một nâng liên tục của $f|T$ lên E:

$$
\begin{array}{ccc}
 &  & E\\
 & \nearrow & \Big\downarrow{\scriptstyle p}\\
T\subset Z & \xrightarrow{\ f\ } & B.
\end{array}
$$

#### Mệnh đề 10 {#ta-i-s2-prop-10 .statement tag=01NA}

Cho E, B và Z là các không gian tôpô, $p: E\rightarrow B$ là một ánh xạ étale và $f: Z\rightarrow B$ là một ánh xạ liên tục.

Cho $z\in Z$ và $x\in E$ là các điểm sao cho $f(z) =p(x)$. Tồn tại một lân cận W của $z$ trong Z và một nâng liên tục $g$ của $f$ lên E, xác định trên W, sao cho $g(z) =x$.

Tồn tại một lân cận mở V của $p(x)$ trong B và một tiết diện liên tục $s$ của $p$ trên V sao cho $s(p(x)) =x$ (mệnh đề 9). Tập hợp

$W =\overset{-1}{f}(V)$ là một lân cận mở của $z$ và ánh xạ $g=s\circ (f|W)$ là một nâng liên tục của $f$ lên E, xác định trên W và sao cho $g(z) =x$.

#### Mệnh đề 11 {#ta-i-s2-prop-11 .statement tag=01NB}

Cho E, B và Z là các không gian tôpô, $p: E\rightarrow B$ và $f: Z\rightarrow B$ là các ánh xạ liên tục. Cho $g$ và $g'$ là các nâng liên tục của $f$ lên E. Gọi W là tập hợp các điểm của Z tại đó $g$ và $g'$ trùng nhau.

a) Nếu ánh xạ $p$ là tách, W đóng.

b) Nếu ánh xạ $p$ là étale, W mở.

Ta ký hiệu $h$ là ánh xạ liên tục $(g, g'): Z\rightarrow E\times E$. Ảnh của $h$ được chứa trong $E\times_BE$ vì $p\circ g=f=p\circ g'$ và tập hợp W các điểm của Z tại đó $g$ và $g'$ trùng nhau là ảnh ngược qua $h$ của đường chéo $\Delta_E$.

Nếu ánh xạ $p$ là étale, đường chéo $\Delta_E$ mở trong $E\times_BE$ (I, p. 31, mệnh đề 7), do đó tập hợp W mở trong Z.

Nếu ánh xạ $p$ là tách, đường chéo $\Delta_E$ đóng trong $E\times_BE$ (I, p. 25, định nghĩa 1) và tập hợp W đóng trong Z.

#### Hệ quả 1 {#ta-i-s2-prop-11-cor-1 .statement tag=01NC}

Nếu không gian Z liên thông và nếu ánh xạ $p$ là étale và tách, các nâng liên tục của $f$ lên E trùng nhau tại một điểm thì bằng nhau.

#### Hệ quả 2 {#ta-i-s2-prop-11-cor-2 .statement tag=01ND}

Cho $p: E\rightarrow B$ là một ánh xạ étale và tách. Nếu không gian E liên thông, nhóm Aut$_B(E)$ tác động tự do trên E.

Thực vậy, nếu $f: E\rightarrow E$ là một B-cấu xạ, tập hợp các điểm tại đó $f$ và Id$_E$ trùng nhau bằng E hoặc tập rỗng theo Hệ quả 1.

#### Hệ quả 3 {#ta-i-s2-prop-11-cor-3 .statement tag=01NE}

Cho E, B và Z là các không gian tôpô, cho $p: E\rightarrow B$ là một ánh xạ étale và tách được, và cho $f: Z\rightarrow B$ là một ánh xạ liên tục. Với $i= 1$, 2, cho $U_i$ là một tập con mở ( resp. tập con đóng) của Z và $g_i: U_i\rightarrow E$ là một nâng liên tục của $f$ xác định trên $U_i$. Giả sử giao $U_1\cap U_2$ là liên thông và tồn tại một điểm $z$ của $U_1\cap U_2$ sao cho $g_1(z) =g_2(z)$. Khi đó tồn tại một nâng liên tục của $f$ xác định trên $U_1\cup U_2$ mở rộng $g_1$ và $g_2$.

Theo Hệ quả 1, các hạn chế của $g_1$ và $g_2$ lên $U_1\cap U_2$ bằng nhau. Ánh xạ $g: U_1\cup U_2\rightarrow E$ xác định bởi $g(z) =g_i(z)$ với $z\in U_i(i= 1$, 2) là một nâng liên tục của $f$ xác định trên $U_1\cup U_2$ (TG, I, p. 19, Mệnh đề 4).

Trong các kết quả trên, trường hợp riêng trong đó Z = B và $f=$ Id$_B$ là quan trọng: khi đó các nâng liên tục của $f$ là các tiết diện liên tục của $p$.

#### Mệnh đề 12 {#ta-i-s2-prop-12 .statement tag=01NF}

Cho $p: E\rightarrow B$ là một ánh xạ étale. Để ánh xạ $p$ tách được, điều kiện cần và đủ là với mọi tập con mở V của B và mọi cặp $(s, s')$ các tiết diện liên tục của $p$ trên V, tập hợp các điểm tại đó $s$ và $s'$ trùng nhau là đóng trong V.

Điều kiện này là cần thiết (Mệnh đề 11, I, p. 34). Ta hãy chứng minh rằng nó là đủ. Cho $b$ là một điểm của B, cho $x$ và $x'$ là hai điểm phân biệt của E sao cho $p(x) =p(x') =b$. Cho V là một lân cận mở của $b$ và $s,s'$ là các tiết diện liên tục của $p$ trên V sao cho $s(V)$ và $s'(V)$ lần lượt là các lân cận mở của $x$ và $x'$ (Mệnh đề 9). Theo giả thiết, tập hợp W các điểm $x\in V$ sao cho $s(x)=\not s'(x)$ là mở trong V, do đó trong B. Các tập hợp $s(W)$ và $s'(W)$ lần lượt là các lân cận mở của $x$ và $x'$; chúng rời nhau theo phép dựng. Điều này chứng minh rằng ánh xạ $p$ tách được (I, p. 25, Định nghĩa 1).

### 5. Phép dựng các tiết diện liên tục của các ánh xạ étale

#### Định lý 1 {#ta-i-s2-thm-1 .statement tag=01NG}

Cho $X$, $Y$, $Z$ là các không gian tôpô, cho $f: Z\rightarrow$ $X\times Y$ là một ánh xạ étale và tách, và cho $y_0$ là một điểm của $Y$. Cho $s: X\times Y\rightarrow Z$ là một tiết diện của $f$. Giả sử rằng hạn chế của $s$ lên $X\times  \{y_0\}$ là liên tục, và tương tự các hạn chế của $s$ lên $\{x\} \times Y$ với mọi $x\in X$ cũng vậy. Nếu không gian $Y$ liên thông và liên thông địa phương (TG, I, p. 84, định nghĩa 4), ánh xạ $s$ là liên tục.

#### Bổ đề {#ta-i-s2-n5-lem-1 .statement tag=01NH}

Cho $U$ là một tập hợp mở của $X$, cho $V$ là một tập hợp mở liên thông của $Y$, và cho $(x_1, y_1)\in U\times V$. Giả sử rằng hạn chế của $s$ lên $U\times  \{y_1\}$ là liên tục. Cho $\sigma$ là một tiết diện liên tục của $f$ trên $U\times V$ sao cho $\sigma (x_1, y_1) =s(x_1, y_1)$. Tồn tại một lân cận $U'$ của $x_1$ sao cho $s=\sigma$ trên $U'\times V$. Đặc biệt, $s$ liên tục trong một lân cận của $(x_1, y_1)$.

Vì hạn chế của $s$ lên $U\times  \{y_1\}$ là liên tục và ánh xạ $f$ là étale, tồn tại một lân cận $U'$ của $x_1$ sao cho $s(x, y_1) =\sigma (x, y_1)$ với mọi $x\in U'($I, p. 34, prop. 11, b)). Cho $x\in U'$; vì hạn chế của $s$ lên $\{x\} \times V$ là liên tục và ánh xạ $f$ là étale và tách, theo Hệ quả 1, I, p. 34, ta có $\sigma (x, y) =s(x, y)$ với mọi $y\in V$. Do đó $s$ và $\sigma$ trùng nhau trên $U'\times V$.

Bây giờ chứng minh định lý. Trước hết, hãy chứng minh rằng ánh xạ $s$ liên tục trong một lân cận của mọi điểm của $X\times  \{y_0\}$. Cho $x_0\in$ X; ta có thể chọn một lân cận mở $U$ của $x_0$ trong $X$, một lân cận mở liên thông $V$ của $y_0$ trong $Y$, và một tiết diện liên tục $\sigma : U\times V\rightarrow Z$ của $f$ sao cho $\sigma (x_0, y_0) =s(x_0, y_0)$. Theo bổ đề trên, $s$ liên tục trong một lân cận của $(x_0, y_0)$.

Bây giờ hãy chứng minh rằng ánh xạ $s$ liên tục tại mọi điểm của $X\times Y$. Với $x_0\in X$, ký hiệu $C(x_0)$ là tập hợp các điểm $y\in$ Y sao cho $s$ liên tục trong một lân cận của $(x_0, y)$. Theo định nghĩa, tập hợp $C(x_0)$ là mở trong $Y$, và chứa $y_0$ theo điều đã chứng minh ở trên.

Ta chứng minh rằng nó đóng trong Y. Xét một điểm $y_1$ của Y dính với $C(x_0)$, một lân cận mở U của $x_0$ trong X, một lân cận mở V của $y_1$ trong Y, và một tiết diện liên tục $\sigma : U\times V\rightarrow Z$ của $f$ sao cho $\sigma (x_0, y_1) =s(x_0, y_1)$. Vì hạn chế của $s$ lên $\{x_0\} \times V$ là liên tục và $f$ là étale, tồn tại một lân cận mở $V'$ của $y_1$ trong Y sao cho $\sigma (x_0, y) =s(x_0, y)$ với mọi $y\in V'$ (mệnh đề 11 của I, p. 34). Vì Y liên thông địa phương, ta có thể giả sử rằng $V'$ liên thông. Vì $y_1$ dính với $C(x_0)$, tập hợp $C(x_0)\cap V'$ không rỗng; lấy $y_2$ là một điểm của $C(x_0)\cap V'$. Theo bổ đề áp dụng cho $(x_0, y_2)$, tồn tại một lân cận $U'$ của $x_0$ được chứa trong U sao cho $s=\sigma$ trên $U'\times V'$. Điều này chứng minh rằng $C(x_0)$ đóng, vì $U'\times V'$ là một lân cận của $(x_0, y_1)$. Vì Y liên thông, ta có $C(x_0) = Y$, và điều này đúng với mọi $x_0\in X$, do đó định lý.

#### Hệ quả 1 {#ta-i-s2-thm-1-cor-1 .statement tag=01NI}

Cho X, Y, E, B là các không gian tôpô. Cho $p: E\rightarrow B$ là một ánh xạ étale và tách, cho $h: X\times Y\rightarrow B$ là một ánh xạ liên tục và cho $y_0$ là một điểm của Y. Cho $g: X\times Y\rightarrow E$ là một ánh xạ sao cho $p\circ g=h$. Giả sử rằng các hạn chế của $g$ lên $X\times  \{y_0\}$ một mặt và, với mọi $x\in X$, lên $\{x\} \times Y$ mặt khác, đều liên tục. Nếu không gian Y liên thông và liên thông địa phương, thì ánh xạ $g$ liên tục.

Ký hiệu Z là tích sợi $(X\times Y)\times_BE$ và $f: Z\rightarrow X\times Y,h': Z\rightarrow E$ là các phép chiếu chính tắc. Ánh xạ $f$ là étale (I, p. 31, mệnh đề 8) và tách (I, p. 27, mệnh đề 4). Ánh xạ $s: X\times Y\rightarrow$ Z được xác định bởi $s(x, y) = ((x, y), g(x, y))$ là một tiết diện của $f$ thỏa mãn các giả thiết của định lý 1. Do đó nó liên tục, cũng như $g=h'\circ s$.

#### Nhận xét {#ta-i-s2-n5-rem-1 .statement tag=01NJ}

Nếu trong định lý 1 không giả sử rằng không gian Y liên thông địa phương, thì kết luận của định lý không còn nhất thiết đúng (I, p. 141, bài tập 7).

#### Định lý 2 {#ta-i-s2-thm-2 .statement tag=01NK}

Cho B là một không gian tôpô và A là một không gian con của B. Đặt một trong các giả thiết sau:

(i) A có một hệ cơ bản các lân cận paracompact;

(ii) B là paracompact và A đóng;

(iii) B mêtric hóa được;

(iv) A compact và hai điểm phân biệt của A có các lân cận rời nhau trong B.

Khi đó mọi tiết diện liên tục trên A của một ánh xạ étale $p: E\rightarrow B$ đều mở rộng thành một tiết diện liên tục của p trên một lân cận của A.

Xét tính chất sau đây (PCV) của cặp $(B,A)$:

(PCV) Với mọi phủ $(U_i)_{i\in I}$ của A bởi các tập con mở

của B, tồn tại một lân cận V của A và một họ

hữu hạn địa phương $(F_j)_{j\in J}$ các tập con đóng của V phủ V, sao cho

mỗi $F_j$ được chứa trong một trong các $U_i$.

Định lý 2 suy ra từ các Bổ đề 1 và 3 dưới đây.

#### Bổ đề 1 {#ta-i-s2-lem-1 .statement tag=01NL}

Mỗi tính chất (i) đến (iv) của định lý 2 đều kéo theo tính chất (PCV).

Cho $(U_i)_{i\in I}$ là một phủ mở của A bởi các tập mở của B. Theo giả thiết (i), tồn tại một lân cận V của A có tính chất paracompact được chứa trong hợp của các $U_i$, một phủ mở $(U'_j)_{j\in J}$ của không gian V, hữu hạn địa phương và mịn hơn phủ $(V\cap U_i)_{i\in I}$, và một phủ mở $(U''_j)_{j\in J}$ của không gian V sao cho với mọi $j\in J$, bao đóng $F_j$ của $U''_j$ trong V được chứa trong $U'_j$ (TG, IX, p. 49, prop. 4 và p. 48, cor. 1 to th. 3). Do đó, trong trường hợp này có tính chất (PCV).

Điều kiện (ii) suy ra điều kiện (i) theo Hệ quả 2 của TG, IX, p. 50. Tương tự, điều kiện (iii) suy ra điều kiện (i): thật vậy, nếu B khả mêtric, mọi lân cận của A đều khả mêtric, do đó có tính chất paracompact (TG, IX, p. 51, th. 4).

Cuối cùng, giả sử điều kiện (iv) được thỏa mãn, và ta chứng minh rằng tính chất (PCV) được thỏa mãn. Vì A compact, chỉ cần xét trường hợp một phủ hữu hạn $(U_i)_{0\leqslant i\leqslant n}$. Khi đó ta xây dựng bằng quy nạp các tập mở $V_0, . . . ,V_n$ của B thỏa mãn các điều kiện sau với $0\leqslant i\leqslant n:$

$$
\alpha )A\subset V_0\cup  \cdots  \cup V_i\cup U_{i+1}\cup  \cdots  \cup U_n
$$

$$
\beta )\overline{V_i}\cap A\subset U_i
$$

Giả sử rằng $V_0, . . . ,V_{r-1}$ đã được xây dựng thỏa mãn các điều kiện trên với $0\leqslant i\leqslant r-1$, và ta xây dựng $V_r$. Các tập K = $A\cap \complement U_r$ và $L = A\cap \complement (V_0\cup \cdots \cup V_{r-1}\cup U_{r+1}\cup \cdots \cup U_n)$ là đóng trong A, do đó compact. Theo $(\alpha )$, chúng rời nhau. Theo giả thiết, với mọi điểm $a$ của L và mọi điểm $b$ của K, tồn tại các lân cận rời nhau của $a$ và $b$ trong B. Theo Bổ đề 2 dưới đây, tồn tại các tập mở rời nhau $V_r$ và W trong B sao cho $L\subset V_r$ và $K\subset W$. Từ các bao hàm $L\subset V_r$ và $A\subset V_0\cup  \cdots  \cup V_{r-1}\cup U_r\cup  \cdots  \cup U_n$ và từ định nghĩa của L, suy ra $(\alpha )$ đúng với $i=r$. Mặt khác, ta có $\overline{V_r}\cap K =\emptyset$, do đó $\overline{V_r}\cap A\subset U_r$.

Tập $M =\bigcup_{0\leqslant i\leqslant n}(V_i\cap \complement U_i)$ là đóng và không gặp A theo $(\beta )$. Theo $(\alpha )$, tập $V =((\bigcup_{0\leqslant i\leqslant n}\overline{V_i})-$ M là một lân cận của A trong B. Với $i= 0, . . . , n$, đặt $F_i= V\cap \overline{V_i}:$ đây là một tập con đóng của V, được chứa trong $U_i$. Họ $(F_i)_{0\leqslant i\leqslant n}$ là một phủ của V, do đó có tính chất (PCV).

#### Bổ đề 2 {#ta-i-s2-lem-2 .statement tag=01NM}

Cho B là một không gian tôpô, và K và L là các tập con quasi-compact của B. Giả sử rằng với mọi điểm $a$ của K và mọi điểm $b$ của L, tồn tại các lân cận rời nhau của $a$ và $b$ trong B. Khi đó tồn tại hai tập mở rời nhau U và V trong B sao cho $K\subset U$ và $L\subset V$.

Cho $a$ là một điểm của K. Với mọi $b\in L$, gọi $U_{a,b}$ và $V_{a,b}$ là các lân cận mở rời nhau của $a$ và $b$. Với $a$ cố định, họ $(V_{a,b})_{b\in L}$ là một phủ mở của L. Vì không gian này là quasi-compact, tồn tại một họ hữu hạn $T_a\subset L$ sao cho hợp $V_b$ của các $V_{a,b}$ với $b\in T_a$ chứa L. Giao $U_a$ của các $U_{a,b}$ với $b\in T_a$ là một lân cận mở của $a$, vì $T_a$ hữu hạn; hơn nữa, $U_a$ và $V_a$ rời nhau. Các $(U_a)_{a\in A}$ lập thành một phủ mở của K. Vì K là quasi-compact, tồn tại một họ hữu hạn $S\subset K$ sao cho $U =\bigcup_{a\in S}U_a$ chứa K. Khi đó $V =\bigcap_{a\in S}V_a$ là một tập con mở của B chứa L. Bổ đề được chứng minh.

#### Bổ đề 3 {#ta-i-s2-lem-3 .statement tag=01NN}

Cho B là một không gian tôpô và A là một không gian con của B sao cho cặp $(B,A)$ thỏa mãn tính chất (PCV) của I, p. 37. Khi đó mọi tiết diện liên tục trên A của một ánh xạ étalé $p: E\rightarrow B$ đều mở rộng thành một tiết diện liên tục của $p$ trên một lân cận của A.

Cho $p: E\rightarrow B$ là một ánh xạ étalé và $s: A\rightarrow E$ là một tiết diện liên tục của $p$ trên A. Với mọi điểm $a$ của A, tồn tại một lân cận mở $U_a$ của $a$ và một tiết diện liên tục $s_a: U_a\rightarrow E$ trùng với $s$ trên $U_a\cap A$ (I, p. 34, Mệnh đề 10 và I, p. 34, Mệnh đề 11). Họ $(U_a)_{a\in A}$ là một phủ của A bởi các tập con mở của B. Gọi V là một lân cận của A trong B, gọi $(F_j)_{j\in J}$ là một họ hữu hạn địa phương các tập con đóng của V phủ V, và gọi $a: J\rightarrow A$ là một ánh xạ sao cho $F_j$ được chứa trong $U_{a(j)}$ với mọi $j\in J$ (tính chất (PCV)). Gọi $s_j$ là hạn chế của $s_{a(j)}$ lên $F_j$. Gọi W là tập hợp các điểm $b\in V$ thỏa mãn $s_j(b) =s_k(b)$ với mọi cặp $(j, k)\in J\times J$ sao cho $b\in F_j\cap F_k$. Ta định nghĩa một tiết diện $s': W\rightarrow E$ bởi $s'(b) =s_j(b)$ nếu $b\in F_j$. Ta có $A\subset W$ và $s'|A =s$. Tiết diện $s'$ liên tục theo Mệnh đề 4 của I, p. 19.

Còn phải chứng minh rằng W là một lân cận của A trong B. Với mỗi cặp $(j, k)\in J\times J$, ký hiệu $T_{jk}$ là tập hợp các điểm $b\in F_j\cap F_k$ sao cho $s_j(b)=\not s_k(b)$. Tập hợp $T_{jk}$ là đóng trong $F_j\cap F_k$ (Mệnh đề 11, b) của I, p. 34), do đó trong V, và các tập hợp $T_{jk}$ lập thành một họ hữu hạn địa phương các tập con của V. Hợp T của họ $(T_{jk})$ do đó là một tập hợp đóng của V (TG, I, p. 6, Mệnh đề 4). Theo định nghĩa, W là phần bù của T trong V. Do đó nó là một lân cận của A trong V và do đó trong B.

### 6. Cận trên của lực lượng các thớ của một ánh xạ étale và tách

#### Định lý 3 {#ta-i-s2-thm-3 .statement tag=01NO}

Cho E và B là các không gian tôpô và cho $p: E\rightarrow B$ là một ánh xạ étale và tách. Giả sử E liên thông và B liên thông địa phương. Cho $\mathscr{W}$ là một cơ sở của tôpô của B. Khi đó, với mọi điểm $a$ của B, ta có Card(E$_a$)$\leqslant$ sup(Card($\mathscr{W}$), Card($\mathbf{N}$)).

Vì không gian B liên thông địa phương, tôpô của nó có một cơ sở $\mathscr{W}'$ gồm các tập mở liên thông, chẳng hạn các thành phần liên thông của các tập mở của $\mathscr{W}$ (TG, I, p. 85, Mệnh đề 11). Theo Bổ đề 4 dưới đây, tồn tại một cơ sở $\mathscr{V}$ của tôpô của B gồm các tập mở liên thông và sao cho Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2$.

#### Bổ đề 4 {#ta-i-s2-lem-4 .statement tag=01NP}

Cho B là một không gian tôpô, và cho $\mathscr{W}$ và $\mathscr{W}'$ là các cơ sở của tôpô của B. Tồn tại một tập con $\mathscr{V}$ của $\mathscr{W}'$ là một cơ sở của tôpô của B và sao cho Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2$.

Cho $\mathscr{A}\subset \mathscr{W}\times \mathscr{W}$ là tập hợp các cặp $(W_1,W_2)$ sao cho tồn tại $W'\in \mathscr{W}'$ thỏa mãn $W_1\subset W'\subset W_2$; cho $\varphi :\mathscr{A}\rightarrow \mathscr{W}'$ là một ánh xạ sao cho $W_1\subset \varphi (W_1,W_2)\subset W_2$ với mọi cặp $(W_1,W_2)\in \mathscr{A}$, và cho $\mathscr{V}\subset \mathscr{W}'$ là ảnh của $\varphi$. Ta có

Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{A}$)$\leqslant$ Card($\mathscr{W}\times \mathscr{W}$)

(E, III, p. 25, Mệnh đề 3). Hãy chứng minh rằng $\mathscr{V}$ là một cơ sở của tôpô của B. Cho x là một điểm của B và U là một lân cận của x. Theo giả thiết, x có một lân cận $W_2\in \mathscr{W}$ được chứa trong U, một lân cận $W'\in \mathscr{W}'$ được chứa trong $W_2$ và một lân cận $W_1\in \mathscr{W}$ được chứa trong $W'$. Do đó $W_1\subset W'\subset W_2\subset U$. Khi đó $(W_1,W_2)\in \mathscr{A}$ và $\varphi (W_1,W_2)$ là một lân cận của x được chứa trong U. Theo Mệnh đề 3 của TG, I, p. 5, tập hợp $\mathscr{V}$ là một cơ sở của tôpô của B.

Cho $\mathscr{V}$ là một cơ sở của tôpô của B gồm các tập mở liên thông khác rỗng và sao cho Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2$. Cho $\mathscr{U}$ là tập hợp các tập mở U của E sao cho $p$ cảm sinh một phép đồng phôi từ U lên một tập mở V thuộc $\mathscr{V}$. Mọi phần tử của $\mathscr{U}$ đều là một tập mở liên thông khác rỗng. Vì ánh xạ $p$ là étale, theo Định nghĩa 2 (I, p. 28) và Mệnh đề 3 của TG, I, p. 5, tập hợp $\mathscr{U}$ là một cơ sở của tôpô của E. Ta gọi một dãy sâu róm là một dãy hữu hạn $(U_0, . . . ,U_n)$ gồm các phần tử của $\mathscr{U}$ sao cho với $1\leqslant i\leqslant n,U_{i-1}\cap U_i$ khác rỗng và $p(U_{i-1})\cap p(U_i)$ liên thông. Ký hiệu S là tập hợp các dãy hữu hạn gồm các phần tử của $\mathscr{V}$ và, với mỗi dãy sâu róm $c= (U_0, . . . ,U_n)$, ký hiệu $p(c)$ là dãy $(p(U_0), . . . , p(U_n))$.

#### Bổ đề 5 {#ta-i-s2-lem-5 .statement tag=01NQ}

a) Cho $c= (U_0, . . . ,U_n)$ và $c'= (U'_0, . . . ,U'_m)$ là các dãy sâu róm sao cho $U_0= U'_0$ và $p(c) =p(c')$. Khi đó $c=c'$.

b) Cho U và $U'$ là các phần tử của $\mathscr{U}$. Khi đó tồn tại một dãy sâu róm $c= (U_0, . . . ,U_n)$ sao cho $U_0= U$ và $U_n= U'$.

a) Tất yếu, $m=n$. Với mỗi số nguyên $i$ sao cho $0\leqslant i\leqslant n$, đặt $V_i=p(U_i)$ và gọi $s_i$ và $s'_i$ là các tiết diện liên tục của $p$ trên $V_i$ có ảnh tương ứng là $U_i$ và $U'_i$. Để chứng minh đẳng thức $c=c'$, ta sẽ chứng minh, bằng quy nạp theo $i$, đẳng thức $s_i=s'_i$ với mọi số nguyên $i$ sao cho $0\leqslant i\leqslant n$. Theo giả thiết, ta có $s_0=s'_0$. Cho $i$ sao cho $1\leqslant i\leqslant n$ và $s_{i-1}=s'_{i-1}$. Vì $U_{i-1}\cap U_i$ chứa một điểm $x$, các tiết diện liên tục $s_{i-1}$ và $s_i$ trùng nhau tại $p(x)$, do đó tại mọi điểm của $V_{i-1}\cap V_i$, vì tập này liên thông (Hệ quả 1 của I, p. 34). Điều tương tự đúng đối với $s'_{i-1}$ và $s'_i$. Vì cùng lý do, $s_i$ và $s'_i$, vốn trùng nhau trên $V_{i-1}\cap V_i$, cũng trùng nhau trên $V_i$, do đó có kết quả.

b) Nếu $x$ và $y$ là các điểm của E, ta nói rằng một sâu đo $c= (U_0, . . . ,U_n)$ nối $x$ với $y$ nếu $x\in U_0$ và $y\in U_n$. Trong tập hợp E, gọi R là quan hệ “tồn tại một sâu đo nối $x$ với $y$”. Quan hệ R phản xạ vì $\mathscr{U}$ là một phủ của E. Hiển nhiên nó đối xứng. Bây giờ chứng minh rằng nó bắc cầu: cho $x,y,z$ là ba điểm của E, $(U_0, . . . ,U_n)$ và $(U'_0, . . . ,U'_m)$ lần lượt là các sâu đo nối $x$ với $y$ và $y$ với $z$. Cho $U\in \mathscr{U}$ là một lân cận của $y$ được chứa trong $U_n\cap U'_0$; ta có $p(U_n)\cap p(U) =p(U'_0)\cap p(U) =p(U)$, và vì U liên thông, dãy $(U_0, . . . ,U_n,U,U'_0, . . . ,U'_m)$ là một sâu đo nối $x$ với $z$. Các lớp tương đương theo R là mở, do đó cũng đóng. Vì E liên thông, suy ra bất kỳ hai điểm nào của E cũng luôn được nối bởi một sâu đo.

Bây giờ cho U và $U'$ là các phần tử của $\mathscr{U}$, x là một điểm của U và $x'$ là một điểm của $U'$. Tồn tại một sâu đo $(U_2, . . . ,U_{n-2})$ nối $x$ với $x'$. Cho $U_1$ và $U_{n-1}$ là các tập mở của $\mathscr{U}$ sao cho $x\in U_1,x'\in U_{n-1}$, $U_1\subset U\cap U_2,U_{n-1}\subset U'\cap U_{n-2}$. Đặt $U_0= U$, $U_n= U'$. Khi đó dãy $(U_0, . . . ,U_n)$ là một sâu đo.

Bây giờ chứng minh định lý. Cho U là một phần tử của $\mathscr{U}$ và gọi C là tập hợp các sâu đo $(U_0, . . . ,U_n)$ sao cho $U_0= U$. Ánh xạ từ C vào S, ánh xạ mỗi sâu đo $c= (U_0, . . . ,U_n)$ của C vào dãy $p(c) = (p(U_0), . . . , p(U_n))$, là đơn ánh (Bổ đề 5, a)), do đó

(1) Card(C) $\leqslant$ Card(S).

Ánh xạ từ C vào $\mathscr{U}$, ánh xạ $c= (U_0, . . . ,U_n)\in C$ vào tập mở $U_n$, là toàn ánh theo phần thứ hai của Bổ đề 5, do đó (2) Card($\mathscr{U}$)$\leqslant$ Card(C).

Với mỗi điểm $x$ của E, ta chọn một tập hợp mở $U_x$ của $\mathscr{U}$ sao cho $x\in U_x$. Nếu $x$ và $y$ là các điểm phân biệt của cùng một sợi $E_a$ của $p$, ta có $U_x= U\not_y$ vì $p|U_x$ là đơn ánh. Do đó, với $a\in B$, (3) Card(E$_a$)$\leqslant$ Card($\mathscr{U}$).

Cuối cùng, nếu $\mathscr{V}$ là một tập hợp hữu hạn, tập hợp S các dãy hữu hạn gồm các phần tử của $\mathscr{V}$ là đếm được (E, III, p. 49, prop. 1), do đó

(4) Card(S) $\leqslant$ Card($\mathbf{N}$).

Nếu $\mathscr{V}$ là vô hạn, ta có

(5) Card(S) = Card($\mathscr{V}$)$\leqslant$ Card($\mathscr{W}$)$^2=$ Card($\mathscr{W}$)

theo hệ quả của E, III, p. 50 và Hệ quả 1 của E, III, p. 49. Định lý suy ra từ các hệ thức (1) đến (5) ở trên.

#### Nhận xét {#ta-i-s2-n6-rem-1 .statement tag=01NR}

Từ những điều trên, nếu tôpô của B có một cơ sở đếm được, thì điều tương tự cũng đúng đối với tôpô của E và các sợi của E đều đếm được (cf. TG, I, p. 88, định lý Poincaré-Volterra).

## BÀI TẬP {#ta-i-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
