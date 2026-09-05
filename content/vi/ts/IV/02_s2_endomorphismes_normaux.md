---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 2
section_title: Endomorphismes normaux
lang: vi
source: ts-iii-v-fr
book_pages: TS IV.179-TS IV.195, TS IV.319-TS IV.330
pdf_pages: 0192-0208, 0332-0343
extraction: native
subsections:
    - "no": 1
      title: Compléments sur les espaces $L^p(X, \mu)$
      page: 179
      pdf_page: 192
    - "no": 2
      title: Image essentielle d’une fonction mesurable
      page: 181
      pdf_page: 194
    - "no": 3
      title: Fonctions universellement mesurables
      page: 182
      pdf_page: 195
    - "no": 4
      title: L’algèbre stellaire $L^{\infty}(X, \mu)$
      page: 185
      pdf_page: 198
    - "no": 5
      title: Endomorphismes de multiplication
      page: 186
      pdf_page: 199
    - "no": 6
      title: Mesures spectrales
      page: 190
      pdf_page: 203
    - "no": 7
      title: Algèbres stellaires commutatives d’endomorphismes d’un espace hilbertien
      page: 191
      pdf_page: 204
    - "no": 8
      title: Continuité du calcul fonctionnel
      page: 194
      pdf_page: 207
statements: 32
exercises: 28
content_sha256: b5c8c5e1262ed991340ee0d7fd7a14dce3adc25054063479cc27425f25a2c0bf
translated_from: content/en-mt/ts/IV/02_s2_endomorphismes_normaux.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 0067987d155820404a75f619ade4cf9674a5866210669997c73b0916f3d2e730
translation_model: gpt-5.4
translation_run: translate-vi-49311ae8
glossary_version: 34
glossary_terms_sha256: 7dd30a555e1865ad61d7b51c1ba831a0f57e821835aa355a04e4b449899551bd
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC TỰ ĐỒNG CẤU CHUẨN

Trong đoạn này, các không gian Hilbert được xét là phức, trừ khi có nói khác.

### 1. Bổ sung về các không gian $L^p(X, \mu)$

#### Mệnh đề 1 {#ts-iv-s2-prop-1 .statement tag=02YO}

Cho X là một không gian tôpô compact địa phương. Cho $\mu$ là một độ đo dương trên X và cho $p\in [1,+\infty [$. Cho $(X_i)_{i\in I}$ là một họ đếm được địa phương (INT, IV, p. 190, § 5, n$^o9$, def. 7) các tập con compact địa phương đôi một rời nhau của X sao cho phần bù của hợp các $X_i$ là địa phương không đáng kể đối với $\mu$. Gọi $\varphi_i$ là hàm đặc trưng của $X_i$ và $\mu_i$ là độ đo cảm sinh bởi $\mu$ trên $X_i$ (INT, IV, p. 186, §5, n$^o7$, def. 4).

a) Ánh xạ $p_i:f\mapsto f \varphi_i$ là một phép chiếu của $\mathscr{L}^p(X, \mu)$ và xác định, khi chuyển qua các thương, một phép chiếu $\widetilde{p}_i$ của $L^p(X, \mu)$. Phép chiếu sau là một phép chiếu trực giao của $L^2(X, \mu)$ nếu $p= 2$;

b) Ánh xạ $f\mapsto f|X_i$ cảm sinh một đẳng cấu đẳng cự từ ảnh của $p_i$ lên không gian $\mathscr{L}^p(X_i, \mu_i)$ và xác định, khi chuyển qua các thương, một đẳng cấu đẳng cự từ ảnh của $\widetilde{p}_i$ lên $L^p(X_i, \mu_i)$, qua đó hai không gian này được đồng nhất;

c) Tổng của các không gian $L^p(X_i, \mu_i)$ là trù mật trong không gian $L^p(X, \mu)$. Trong trường hợp $p= 2$, không gian $L^2(X, \mu)$ là tổng Hilbert của các không gian $L^2(X_i, \mu_i)$.

Mệnh đề a) là sơ cấp. Mệnh đề b) suy ra từ chú giải của INT, V, p. 84, § 7, n$^o1$.

Cho $q\in ]1,+\infty ]$ là số mũ liên hợp của $p$. Ta đồng nhất đối ngẫu của $L^p(X, \mu)$ với $L^q(X, \mu)$ (INT, V, p. 61, § 5, n$^o8$, th. 4). Gọi $f$ là một hàm trong $\mathscr{L}^q(X, \mu)$ mà lớp $\widetilde{f}$ của nó trong $L^q(X, \mu)$ thỏa mãn $\langle \widetilde{f} ,\widetilde{p}_i(\varphi )\rangle = 0$ với mọi $i\in I$ và mọi $\varphi \in L^p(X, \mu)$. Vì ảnh của $p_i$ chứa $\mathscr{K}(X_i)$, suy ra độ đo $(f|X_i)\cdot \mu_i$ trên $X_i$ bằng không, điều đó có nghĩa là hạn chế của $f$ trên $X_i$ là địa phương không đáng kể đối với $\mu_i$ trên $X_i$ (INT, V, p. 46, § 5, n$^o3$, hệ quả 2). Vì phần bù trong X của hợp các $X_i$ là địa phương không đáng kể đối với $\mu$, ta kết luận rằng hàm $f$ là địa phương không đáng kể đối với $\mu$ trên X (INT, IV, p. 190, § 5, n$^o9$ and p. 172, n$^o2$, mệnh đề 5). Khi đó lớp của $f$ bằng không trong $L^q(X, \mu)$ (dùng INT, V, p. 8, § 1, n$^o3$, bổ đề 1 và hệ quả của mệnh đề 9 khi $p\not = 1$). Theo định lý Hahn–Banach (EVT, II, p. 46, hệ quả 1), phần thứ nhất của mệnh đề c) suy ra.

Nếu $p= 2$, ảnh của $p_i$ trực giao với ảnh của $p_j$ với mọi $i\not =j$, vì khi đó $X_i$ và $X_j$ rời nhau, do đó có khẳng định cuối cùng.

#### Mệnh đề 2 {#ts-iv-s2-prop-2 .statement tag=02YP}

Cho X là một không gian địa phương compact đếm được tại vô cực. Cho $\mu$ là một độ đo dương trên X. Với mọi $p\in [1,+\infty [$, không gian $L^p(X, \mu)$ thuộc kiểu đếm được.

Gọi $(U_n)_{n\in\mathbf{N}}$ là một dãy các tập con mở tương đối compact của X mà hợp của chúng bằng X và thỏa mãn $U_n\subset U_{n+1}$ với mọi $n\in \mathbf{N}$ (TG, I, p. 68, mệnh đề 15). Với mọi $n\in \mathbf{N}$, không gian $\mathscr{K}(X,\overline{U}_n)$ được đồng nhất với một không gian con đóng của không gian Banach $\mathscr{C}(U_n)$ (INT, III, p. 40, § 1, n$^o1$); vì không gian sau này thuộc kiểu đếm được (TG, X, p. 25, hệ quả), điều tương tự cũng đúng với $\mathscr{K}(X,\overline{U}_n)$ (TG, IX, p. 19, hệ quả, (i)). Gọi $\mathscr{F}_n$ là một tập con đếm được trù mật của $\mathscr{K}(X,\overline{U}_n)$.

Cho $f\in \mathscr{L}^p(X, \mu)$ và $\varepsilon  >0$. Tồn tại một số nguyên $n\in \mathbf{N}$ sao cho $\int_{X-U_n}|f|^p< \varepsilon /2$, và tồn tại $g\in \mathscr{F}_n$ sao cho $\int_{\overline{U}_n}|f-g|^p< \varepsilon /2$. Vậy hợp các lớp trong $L^p(X, \mu)$ của các phần tử của các tập $\mathscr{F}_n$ là trù mật trong $L^p(X, \mu)$, điều này kết thúc chứng minh (TG, IX, p. 18, prop. 12).

### 2. Ảnh cốt yếu của một hàm đo được

Trong số này, X chỉ một không gian tôpô địa phương compact, và $\mu$ một độ đo dương trên X.

#### Định nghĩa 1 {#ts-iv-s2-def-1 .statement tag=02YQ}

Cho Y là một không gian tôpô. Với mọi hàm đo được $g$ từ X vào Y, ảnh cốt yếu theo $\mu$ của $g$ là tập con các $y\in Y$ sao cho, với mọi lân cận mở U của $y$, tập $\overset{-1}{g}(U)$ không địa phương $\mu$-không đáng kể trong X (INT, IV, p. 172, § 5, n$^o2$, định nghĩa 3).

#### Bổ đề 1 {#ts-iv-s2-lem-1 .statement tag=02YR}

Cho $g$ là một hàm $\mu$-đo được từ X vào một không gian tôpô Y, và S là ảnh cốt yếu theo $\mu$ của nó. Tập hợp các phần tử $x\in X$ sao cho $g(x)$ không thuộc S là địa phương $\mu$-không đáng kể trong X.

Đặt $Z =\overset{-1}{g}(Y$ - S) là tập hợp đang xét.

Trước hết giả sử rằng X compact và $g$ liên tục. Trong trường hợp này, độ đo ảnh $g(\mu)$ được xác định (INT, V, p. 69, § 6, n$^o1$, định nghĩa 1) vì $\mu$ là một độ đo bị chặn. Từ các định nghĩa suy ra rằng ảnh cốt yếu theo $\mu$ của $g$ là giá của độ đo $g(\mu) ($xem INT, V, p. 70, § 6, n$^o2$, hệ quả 2), do đó $\mu(Z) =g(\mu)(Y$ - S) = 0 (INT, IV, p. 118, § 2, n$^o2$, mệnh đề 5).

Bây giờ xét trường hợp tổng quát. Cho C là một tập con compact của X, và cho $\varepsilon  >0$ là một số thực. Vì $g$ đo được, tồn tại một tập con compact $C_1\subset C$ sao cho $\mu(C$- $C_1)\leqslant \varepsilon$ và sao cho $g|C_1$ liên tục (INT, IV, p. 169, § 5, n$^o1$, mệnh đề 1). Khi đó ta có

$\mu(Z\cap C)\leqslant \mu(C$ - $C_1) +\mu(Z\cap C_1)\leqslant \varepsilon +\mu(Z\cap C_1)$.

Cho $\mu_1$ là độ đo cảm sinh bởi $\mu$ trên $C_1$ (INT, IV, p. 186, § 5, n$^o7$, định nghĩa 4). Cho $S_1$ là ảnh cốt yếu theo $\mu_1$ của $g|C_1$. Ta có $Z\cap C_1\subset$ $(g|C_1)^{-1}(Y$ - $S_1)$. Theo trường hợp thứ nhất, do đó tập $Z\cap C_1$ là $\mu_1$-không đáng kể, và do đó $\mu$-không đáng kể (INT, IV, p. 187, § 5, n$^o7$, bổ đề 2, (i)). Bất đẳng thức trên trở thành $\mu(Z\cap C)\leqslant \varepsilon$; vì $\varepsilon$ và C là tùy ý, tập Z là địa phương $\mu$-không đáng kể (INT, IV, p. 172, § 5, n$^o2$, mệnh đề 5).

#### Bổ đề 2 {#ts-iv-s2-lem-2 .statement tag=02YS}

Cho $g$ là một hàm liên tục từ X vào $\mathbf{C}$. Ảnh cốt yếu theo $\mu$ của $g$ là bao đóng của ảnh qua $g$ của giá của $\mu$.

Gọi Y là giá của $\mu$. Nếu $z\in \mathbf{C}$ không dính với $g$(Y), thì tồn tại một lân cận mở U của $z$ sao cho tập mở $\overset{-1}{g}(U)$ không gặp Y và do đó địa phương $\mu$-không đáng kể; điều này có nghĩa là $z$ không thuộc ảnh $\mu$-cốt yếu của $g$.

Ngược lại, nếu $z\in \mathbf{C}$ dính với $g$(Y), thì với mọi lân cận mở U của $z$, tập $\overset{-1}{g}(U)$ là một tập mở trong X mà gặp Y. Vậy nó không $\mu$-không đáng kể, và vì nó là mở, nó không địa phương $\mu$-không đáng kể (INT, IV, p. 172, § 5, n$^o2$, Hệ quả 2). Do đó $z$ thuộc ảnh $\mu$-cốt yếu của $g$.

#### Bổ đề 3 {#ts-iv-s2-lem-3 .statement tag=02YT}

Cho $g$ là một hàm liên tục từ X vào $\mathbf{C}$ và S là ảnh $\mu$-cốt yếu của nó. Giả sử S không rỗng và $0\notin S$; ký hiệu bởi $\delta$ khoảng cách từ 0 đến S. Khi đó $\delta  >0$.

Đặt $h(x) = 1/g(x)$ nếu $g(x)\not = 0$ và $h(x) = 0$ trong trường hợp ngược lại. Hàm $h$ thuộc $\mathscr{L}^{\infty}(X, \mu)$. Gọi $\widetilde{h}$ là lớp của $h$ trong $L^{\infty}(X, \mu)$. Khi đó ta có công thức $\delta^{-1}=\|\widetilde{h}\|_{\infty}$.

Lấy U là một lân cận mở của 0 sao cho tập mở $Z =\overset{-1}{g}(U)$ là địa phương $\mu$-không đáng kể, do đó không đáng kể (INT, IV, p. 172, § 5, n$^o2$, Hệ quả 2). Gọi Y là giá của $\mu$; ta có $Y\subset X$ - Z. Hạn chế của hàm $h$ lên X - Z là liên tục và bị chặn; do đó $h\in \mathscr{L}^{\infty}(X, \mu)$ và chuẩn của $\widetilde{h}$ trong $\mathscr{L}^{\infty}(X, \mu)$ bằng chuẩn của hạn chế của nó lên X - Z. Hơn nữa, với mọi $\alpha \in \mathbf{R}_+$, tập các $x\in X$ - Z sao cho $|h(x)|> \alpha$ là một tập mở trong X - Z; do đó nó địa phương $\mu$-không đáng kể khi và chỉ khi nó không gặp Y (INT, IV, loc. cit. and INT, III, p. 66, § 3, n$^o2$, Def. 1). Do đó, ta có

$\|\widetilde{h}\|_{\infty}=$ sup$_{x\in Y}\frac{1}{|g(x)|}$,

do đó

$\|\widetilde{h}1\|=$ inf$_{\infty x\in Y}|g(x)|=$ inf$_{\lambda\in g(Y)}|\lambda |=$ inf$_{\lambda\in\overline{g(Y)}}|\lambda |$

và lượng này bằng $\delta$ theo bổ đề trước.

### 3. Hàm đo được phổ dụng

Trong số này, X là một không gian tôpô compact địa phương. Ta nhắc lại (INT, V, p. 28, § 3, No$^o4$, def. 2) rằng một ánh xạ $f$ từ X vào một không gian tôpô Y là đo được phổ dụng nếu nó là $\mu$-đo được đối với mọi độ đo dương $\mu$ trên X. Để được như vậy, chỉ cần $f$ là $\mu$-đo được đối với mọi độ đo dương $\mu$ có giá compact trên X (INT, V, p. 28, § 4, No$^o3$, prop. 6).

#### Bổ đề 4 {#ts-iv-s2-lem-4 .statement tag=02YU}

Cho Y và Z là các không gian tôpô compact địa phương, $f: X\rightarrow Y$ và $g: Y\rightarrow Z$ là các ánh xạ đo được phổ dụng. Ánh xạ $g\circ f: X\rightarrow Z$ là đo được phổ dụng.

Cho $\mu$ là một độ đo dương có giá compact trên X và C là giá của nó. Hạn chế của $f$ trên C là $(\mu|$C)-thực sự. Ánh xạ $g$ là đo được đối với độ đo ảnh $(f|C)(\mu|C)$, do đó ánh xạ $(g\circ f)|C =g\circ (f|C)$ là $(\mu|$C)-measurable. Do đó, ánh xạ $g\circ f$ là $\mu$-đo được. Bổ đề được chứng minh.

Ta ký hiệu bởi $\mathscr{L}_u(X)$ không gian vectơ các hàm giá trị phức đo được phổ dụng trên X, và bởi $\mathscr{L}_u^{\infty}(X)$ không gian con các hàm $f\in \mathscr{L}_u(X)$ bị chặn trên X. Với $f\in \mathscr{L}_u^{\infty}$(X), ta đặt $\|f\|_{\infty}=$ sup$_{x\in X}|f(x)|$.

#### Mệnh đề 3 {#ts-iv-s2-prop-3 .statement tag=02YV}

a) Tập hợp $\mathscr{L}_u(X)$ là một đại số con có đối hợp của đại số có đối hợp các hàm từ X vào $\mathbf{C}$;

b) Tập hợp $\mathscr{L}_u^{\infty}(X)$ là một đại số con của $\mathscr{L}_u(X)$ và ánh xạ được xác định bởi $f\mapsto  \|f\|_{\infty}$ là một chuẩn trên $\mathscr{L}_u^{\infty}(X)$ đối với đó $\mathscr{L}_u^{\infty}(X)$ là một đại số stellar có đơn vị;

c) Đại số $\mathscr{L}_u(X)$ chứa $\mathscr{C}(X)$ và $\mathscr{L}_u^{\infty}(X)$ chứa $\mathscr{C}_b(X)$;

d) Mọi hàm Borel từ X vào $\mathbf{C}$ (TG, IX, p. 61, def. 5) đều thuộc $\mathscr{L}_u(X)$;

e) Với mọi dãy $(f_n)_{n\in\mathbf{N}}$ trong $\mathscr{L}_u(X)$ hội tụ đơn giản tới một hàm $f$ từ X vào $\mathbf{C}$, ta có $f\in \mathscr{L}_u(X)$.

Các mệnh đề a) và c) suy ra từ các định nghĩa (x. INT, IV, p. 175, § 5, No$^o3$, cor. 3). Mệnh đề d) là một hệ quả của INT, IV, p. 179, § 5, No$^o5$, th. 4, vì ảnh ngược qua một hàm Borel của mọi tập con Borel của $\mathbf{C}$ là một tập con Borel của X, mà tập này đo được phổ dụng (INT, V, p. 28, § 3, No$^o4$). Cuối cùng, mệnh đề e) suy ra từ định lý Egoroff (INT, IV, p. 175, § 5, No$^o4$, th. 2).

Để chứng minh mệnh đề b), chỉ cần nhận xét rằng e) kéo theo, a fortiori, rằng một giới hạn đều của các hàm đo được phổ dụng là đo được phổ dụng.

Có thể tồn tại các hàm đo được phổ dụng trên X mà không phải là Borel. Thật vậy, nếu X là khả mêtric, hàm đặc số của một tập con Souslin của X là đo được phổ dụng (x. INT, IV, p. 171, § 5, No$^o1$, cor. 2); mà trong mọi không gian Polish không đếm được, tồn tại một tập con Souslin không phải là Borel ("định lý Souslin"; điều này suy ra từ TG, IX, p. 120, bài tập 8 và từ sự kiện rằng với mọi không gian Polish không đếm được X, tồn tại một song ánh Borel $X\rightarrow \mathbf{N}^{\mathbf{N}}$ mà nghịch đảo của nó là Borel).

#### Bổ đề 5 {#ts-iv-s2-lem-5 .statement tag=02YW}

Cho $\mu$ là một độ đo dương trên X. Cho $g$ là một hàm $\mu$-đo được từ X vào $\mathbf{C}$, và cho S là ảnh cốt yếu theo $\mu$ của nó. Đối với mọi hàm $f\in \mathscr{L}_u(S)$, ánh xạ $h$ từ X vào $\mathbf{C}$ sao cho $h(x) = 0$ nếu $g(x)\notin S$ và $h(x) =f(g(x))$ nếu $g(x)\in S$ là $\mu$-đo được.

Cho $x\in X$ và cho U là một lân cận mở tương đối compắc của $x$. Tập N = U - $(U\cap \overset{-1}{g}(S))$ là không đáng kể đối với $(\mu|$U). Với mọi số nguyên $n\geqslant 1$, cho $V_n$ là một tập mở sao cho $N\subset V_n\subset U$ và $\mu(V_n-N)<1/n$ (INT, IV, p. 116, § 1, n$^o4$, mđ. 19).

Hạn chế $\widetilde{g}$ của $g$ lên U- $V_n$ là thực sự đối với $\mu|(U$- $V_n$), và ảnh của nó được chứa trong S. Vì $f$ là đo được phổ dụng, ánh xạ $x\mapsto f(g(x))$ từ U - $V_n$ vào $\mathbf{C}$ là đo được đối với độ đo $\mu|(U$ - $V_n)$ (INT, V, p. 71, § 6, n$^o2$, mđ. 3). Do đó ánh xạ $h_n$ từ X vào $\mathbf{C}$ sao cho $h_n(x) = 0$ nếu $x \notin U$ - $V_n$ và $h_n(x) =f(g(x))$ nếu $x\in U$ - $V_n$ là $\mu$-đo được (INT, IV, p. 193, § 5, n$^o10$, mđ. 16).

Vì $h_n(x)\rightarrow h(x)$ với $\mu$-hầu khắp mọi $x\in U$, hạn chế của $h$ lên U là $\mu$-đo được (INT, IV, p. 175, § 5, n$^o4$, đl. 2). Suy ra $h$ là $\mu$-đo được theo nguyên lý địa phương hoá (INT, IV, p. 171, § 4, n$^o2$, mđ. 4).

#### Nhận xét {#ts-iv-s2-n3-rem-1 .statement tag=02YX}

Dưới các giả thiết của bổ đề, ta sẽ ký hiệu, với một sự lạm dụng ngôn ngữ, hàm $h$ được định nghĩa trong bổ đề bởi $f\circ g$.

Nếu $g=g_1$ cục bộ $\mu$-hầu khắp nơi trên X, thì các hàm $g$ và $g_1$ có cùng ảnh $\mu$-cốt yếu và ta có $f\circ g=f\circ g_1$.

Nếu $g$ là một hàm $\mu$-đo được được xác định $\mu$-hầu khắp trên X, người ta cũng ký hiệu bởi $f\circ g$ hàm $f\circ g_1$, trong đó $g_1$ là một hàm $\mu$-đo được xác định trên X và bằng $g$ cục bộ $\mu$-hầu khắp nơi.

### 4. Đại số sao $L^{\infty}(X, \mu)$

Cho X là một không gian tôpô compact địa phương và cho $\mu$ là một độ đo dương trên X. Ta xét đại số sao giao hoán $L^{\infty}(X, \mu)$ (Ví dụ 4 của I, p. 103).

#### Bổ đề 6 {#ts-iv-s2-lem-6 .statement tag=02YY}

Cho $g\in \mathscr{L}^{\infty}(X, \mu)$. Phổ của lớp của $g$ trong $L^{\infty}(X, \mu)$ bằng ảnh $\mu$-cốt yếu của $g$.

Ký hiệu bởi $\widetilde{g}$ lớp của $g$ trong $L^{\infty}(X, \mu)$ và bởi S ảnh $\mu$-cốt yếu của $g$. Cho $z\in \mathbf{C}-$ S. Theo định nghĩa, tồn tại một lân cận mở U của $z$ sao cho $Y =\overset{-1}{g}(U)$ là cục bộ $\mu$-không đáng kể. Hàm $h$ được xác định bởi $h(x) = (g(x)-z)^{-1}$ nếu $x \notin Y$, và $h(x) = 0$ nếu $x\in Y$, khi đó thuộc $\mathscr{L}^{\infty}(X, \mu)$. Lớp của nó $\widetilde{h}$ trong $L^{\infty}(X, \mu)$ thỏa mãn $(\widetilde{g}-z)\widetilde{h}= 1$, vì $(g(x)-z)h(x) = 1$ với mọi $x$ không thuộc tập cục bộ $\mu$-không đáng kể Y. Do đó $z\in \mathbf{C}-$ Sp($\widetilde{g}$).

Ngược lại, giả sử $z\in \mathbf{C}-$ Sp($\widetilde{g}$). Gọi $h\in \mathscr{L}^{\infty}(X, \mu)$ là một hàm mà lớp của nó là nghịch đảo của $\widetilde{g}-z$ trong $L^{\infty}(X, \mu)$. Tồn tại một số thực $M>0$ sao cho $|h(x)|\leqslant M$ địa phương $\mu$-hầu khắp nơi, và hơn nữa ta có $(g(x)-z)h(x) = 1$ địa phương $\mu$-hầu khắp nơi. Gọi U là quả cầu mở tâm $z$ và bán kính $M^{-1}$ trong $\mathbf{C}$; khi đó $\overset{-1}{g}(U)$ được chứa trong tập địa phương $\mu$-không đáng kể

$$
\overset{-1}{h}(]M,+\infty [)\cup  \{x\in X|(g(x)-z)h(x)\not = 1\}
$$

vì thế $z\in \mathbf{C}-$ S. Bổ đề được chứng minh.

#### Mệnh đề 4 {#ts-iv-s2-prop-4 .statement tag=02YZ}

Cho $g\in \mathscr{L}^{\infty}(X, \mu)$. Ký hiệu $\widetilde{g}$ là lớp của $g$ trong $L^{\infty}(X, \mu)$ và S là phổ của $\widetilde{g}$. Ánh xạ $f\mapsto f\circ g$ (nhận xét, p. 184) là ánh xạ phép tính phiếm hàm từ $\mathscr{C}(S)$ vào $L^{\infty}(X, \mu)$ liên kết với $\widetilde{g}$.

Cho $f\in \mathscr{C}(S)$. Hàm $h=f\circ g$ là $\mu$-đo được (Bổ đề 5 của IV, p. 184) và bị chặn. Ký hiệu $f\widetilde{\circ}g$ là lớp của nó trong $L^{\infty}(X, \mu)$. Ánh xạ $f\mapsto f\widetilde{\circ}g$ là một cấu xạ liên tục của các đại số đối hợp có đơn vị từ $\mathscr{C}(S)$ vào $L^{\infty}(X, \mu)$. Vì $g(x)$ thuộc S địa phương $\mu$-hầu khắp nơi (Bổ đề 1 của IV, p. 181 và Bổ đề 6), cấu xạ này liên kết với ánh xạ đồng nhất của S lớp $\widetilde{g}$ của hàm $g$. Vậy nên nó trùng với ánh xạ phép tính phiếm hàm của $\widetilde{g}$ (Mệnh đề 7 của I, p. 111).

### 5. Các tự đồng cấu phép nhân

Cho X là một không gian tôpô compact địa phương và cho $\mu$ là một độ đo dương trên X. Cho $p\in [1,+\infty [$.

Cho $g\in \mathscr{L}^{\infty}(X, \mu)$. Ký hiệu $m_g$ là ánh xạ $f\mapsto g\cdot f$ từ $\mathscr{L}^p(X, \mu)$ vào chính nó. Ánh xạ $m_g$ là tuyến tính và liên tục vì

$$
N_p(m_g(f))\leqslant N_{\infty}(g)N_p(f) \tag{1}
$$

đối với mọi hàm $f\in \mathscr{L}^p(X, \mu)$. Đặc biệt, hàm $m_g(f)$ là $\mu$-không đáng kể nếu $f$ là $\mu$-không đáng kể. Do đó ánh xạ $m_g$ suy ra, bằng cách chuyển qua các thương, một tự đồng cấu của $L^p(X, \mu)$, sẽ được ký hiệu bởi $\widetilde{m}_g$.

#### Bổ đề 7 {#ts-iv-s2-lem-7 .statement tag=02Z0}

Cho $g\in \mathscr{L}^{\infty}(X, \mu)$. Tự đồng cấu $\widetilde{m}_g$ của $L^p(X, \mu)$ là đơn ánh nếu và chỉ nếu tập hợp các $x\in X$ sao cho $g(x) = 0$ là địa phương $\mu$-không đáng kể.

Gọi A là tập hợp các $x\in X$ sao cho $g(x) = 0$.

Giả sử rằng A là địa phương $\mu$-không đáng kể. Cho $f\in \mathscr{L}^p(X, \mu)$ và $\widetilde{f}$ là lớp của nó trong $L^p(X, \mu)$. Giả sử rằng $\widetilde{m}_g(\widetilde{f}) = 0$. Theo định nghĩa, điều này xảy ra nếu và chỉ nếu hàm $f g$ là $\mu$-không đáng kể, nên tập hợp B các $x\in X$ sao cho $f(x)g(x)\not = 0$ là $\mu$-không đáng kể. Hàm $f$ bằng không ở ngoài $A\cup B$, do đó là $\mu$-không đáng kể. Điều này suy ra rằng tự đồng cấu $\widetilde{m}_g$ là đơn ánh.

Ngược lại, giả sử rằng A không địa phương $\mu$-không đáng kể. Cho C là một tập con compắc của X sao cho $A\cap C$ không $\mu$-không đáng kể, và gọi $\varphi$ là hàm đặc số của $A\cap C$. Lớp của hàm $\varphi$ trong $L^p(X, \mu)$ khác không, nhưng lớp của $m_g(\varphi )$ thì bằng không, do đó $m_g$ không đơn ánh.

Vì tích của một hàm địa phương $\mu$-không đáng kể và một hàm $\mu$-không đáng kể là $\mu$-không đáng kể, tự đồng cấu $\widetilde{m}_g$ chỉ phụ thuộc vào lớp của $g$ trong $L^{\infty}(X, \mu)$. Với $\widetilde{g}\in L^{\infty}(X, \mu)$, người ta cũng ký hiệu bởi $\widetilde{m}_g$ tự đồng cấu $\widetilde{m}_g$ của $L^p(X, \mu)$ đối với mọi hàm $g\in \mathscr{L}^{\infty}(X, \mu\widetilde{)}$ có lớp là $\widetilde{g}$. Người ta nói rằng $\widetilde{m}_g$ là tự đồng cấu phép nhân bởi $\widetilde{g}$ trong $L^p(X, \mu)$.

#### Mệnh đề 5 {#ts-iv-s2-prop-5 .statement tag=02Z1}

Cho $p\in [1,+\infty [$. Ánh xạ $m:g\mapsto \widetilde{m}_g$ từ $L^{\infty}(X, \mu)$ vào $\mathscr{L}(L^p(X, \mu))$ là một cấu xạ đẳng cự của các đại số Banach có đơn vị.

Với $a,b$ trong $\mathbf{C}$ và $g_1,g_2$ trong $L^{\infty}(X, \mu)$, ta kiểm tra ngay được rằng $\widetilde{m}_{ag_1+bg_2}=a\widetilde{m}g_1+b\widetilde{m}_{g_2}$, do đó ánh xạ $\widetilde{m}$ là tuyến tính. Hơn nữa, ta có $\widetilde{m}_1= 1_{L^p(X,\mu)}$ và $\widetilde{m}_{g_1g_2}=\widetilde{m}_{g_1}\widetilde{m}_{g_2}$, do đó ánh xạ $\widetilde{m}$ là một cấu xạ đại số có đơn vị từ $L^{\infty}(X, \mu)$ vào $\mathscr{L}(L^p(X, \mu))$.

Công thức (1) ở trên chứng minh rằng $\widetilde{m}$ có chuẩn $\leqslant 1$.

Cho $g\in \mathscr{L}^{\infty}(X, \mu)$ và $\widetilde{g}$ là lớp của nó trong $L^{\infty}(X, \mu)$. Cho $\varepsilon  >$ 0. Tập hợp Y gồm các $x\in X$ sao cho $|g(x)|>\|\widetilde{g}\|_{\infty}-\varepsilon$ không phải là địa phương $\mu$-không đáng kể. Do đó tồn tại một tập con compact C của X sao cho $\mu(Y\cap C)>0$. Gọi $\varphi$ là hàm đặc trưng của $Y\cap C$. Vì

$$
\|\widetilde{m}_{\widetilde{g}}(\varphi )\|_p=(\int_X|\varphi g|^pd\mu)^{1/p}\geqslant (\int_Y|\varphi g|^pd\mu)^{1/p}
$$

$$
\geqslant (\|\widetilde{g}\|_{\infty}-\varepsilon )\mu(Y\cap C)^{1/p}= (\|\widetilde{g}\|_{\infty}-\varepsilon )\|\varphi \|_p
$$

suy ra $\|\widetilde{m}_{\widetilde{g}}\|\geqslant \|\widetilde{g}\|_{\infty}-\varepsilon$. Vì $\varepsilon$ là tùy ý, suy ra $\|\widetilde{m}_{\widetilde{g}}\|\geqslant \|\widetilde{g}\|_{\infty}$, điều này chứng minh rằng $\widetilde{m}$ là đẳng cự.

#### Bổ đề 8 {#ts-iv-s2-lem-8 .statement tag=02Z2}

Cho $(g_n)$ là một dãy bị chặn trong $\mathscr{L}^{\infty}(X, \mu)$ hội tụ từng điểm $\mu$-hầu khắp nơi. Gọi $\widetilde{m}\in L^{\infty}(X, \mu)$ là lớp của giới hạn của nó. Khi đó $\widetilde{m}_{g_n}$ hội tụ đến $\widetilde{m}_{\widetilde{g}}$ trong không gian $\mathscr{L}(L^p(X, \mu))$ được trang bị tôpô hội tụ đơn.

Cho $f\in \mathscr{L}^p(X, \mu)$. Dãy $(g_nf)$ bị chặn trong $\mathscr{L}^p(X, \mu)$ và hội tụ từng điểm $\mu$-hầu khắp nơi đến $gf$. Theo định lý của Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6), dãy $(g_nf)$ hội tụ đến $gf$ trong $\mathscr{L}^p(X, \mu)$, và mệnh đề được suy ra.

Bây giờ ta sẽ xét trường hợp $p= 2$.

#### Mệnh đề 6 {#ts-iv-s2-prop-6 .statement tag=02Z3}

Ánh xạ $m:g\mapsto \widetilde{m}_g$ là một cấu xạ đẳng cự có đơn vị của đại số có phép đối hợp $L^{\infty}(X, \mu)$ vào đại số có phép đối hợp $\mathscr{L}(L^2(X, \mu))$.

Đặc biệt, với mọi $g\in L^{\infty}(X, \mu)$, tự đồng cấu phép nhân $\widetilde{m}_g$ là chuẩn tắc; nó là Hermit khi và chỉ khi $g$ nhận giá trị thực địa phương $\mu$-hầu khắp nơi.

Theo Mệnh đề 5, ánh xạ $\widetilde{m}$ là một cấu xạ đơn ánh đẳng cự của các đại số Banach có đơn vị từ $L^{\infty}(X, \mu)$ vào $\mathscr{L}(L^2(X, \mu))$. Cho $g\in \mathscr{L}^{\infty}(X, \mu)$. Với $f_1$ và $f_2\in \mathscr{L}^2(X, \mu)$, ta có

$$
\langle f_1|\widetilde{m}_g(f_2)\rangle =\int_X\overline{f_1(x)}g(x)f_2(x)d\mu(x) =\langle \widetilde{m}_{\overline{g}}(f_1)|f_2\rangle
$$

do đó suy ra $\widetilde{m}^*_g=\widetilde{m}_{\overline{g}}$, điều này chứng minh rằng $m$ là một cấu xạ đối hợp. Các khẳng định cuối cùng suy ra từ đó (x. I, p. 106, Mệnh đề 5).

#### Hệ quả {#ts-iv-s2-n5-cor-1 .statement tag=02Z4}

Cho $g\in L^{\infty}(X, \mu)$.

a) phổ của $\widetilde{m}_g$ trong $\mathscr{L}(L^2(X, \mu))$ là ảnh μ-cốt yếu của $g$;

b) tự đồng cấu $\widetilde{m}_g$ là dương khi và chỉ khi $g$ có các giá trị dương địa phương μ-hầu khắp nơi;

c) với mọi hàm $f\in \mathscr{C}$ (Sp($\widetilde{m}_g$)), ta có $f(\widetilde{m}_g) =\widetilde{m}_{f\circ g}$.

Vì $\widetilde{m}$ là đơn ánh, ta có Sp($\widetilde{m}_g$) $=$ Sp($g$) theo Mệnh đề 5 của I, p. 106; khi đó kết quả suy ra từ Bổ đề 6 của IV, p. 185, từ Mệnh đề 4 của IV, p. 185 và từ Định nghĩa 6 của I, p. 115.

#### Mệnh đề 7 {#ts-iv-s2-prop-7 .statement tag=02Z5}

Ảnh của cấu xạ $\widetilde{m}$ từ $L^{\infty}(X, \mu)$ vào $\mathscr{L}(L^2(X, \mu))$ là một đại số con giao hoán cực đại của đại số $\mathscr{L}(L^2(X, \mu))$.

Chỉ cần chứng minh rằng nếu $u\in \mathscr{L}(L^2(X, \mu))$ là một tự đồng cấu giao hoán với $\widetilde{m}_g$ với mọi hàm $g\in \mathscr{L}^{\infty}(X, \mu)$, thì $u$ thuộc ảnh của $\widetilde{m}$. Cho $u$ là một tự đồng cấu như vậy.

Ta ký hiệu bởi $\widetilde{f}$ lớp trong $L^2(X, \mu)$ của một hàm $f\in \mathscr{L}^2(X, \mu)$. Ký hiệu $v$ là ánh xạ tuyến tính từ $\mathscr{L}^2(X, \mu)$ vào $L^2(X, \mu)$ được xác định bởi $f\mapsto u(\widetilde{f})$. Ta có $v\circ m_g=\widetilde{m}_g\circ v$ với mọi $g\in \mathscr{L}^{\infty}(X, \mu)$.

Với mọi tập con μ-đo được Y của X, ký hiệu $\varphi_Y$ là hàm đặc trưng của nó; tự đồng cấu $\widetilde{m}_{\varphi_Y}$ là một phép chiếu trực giao của $L^2(X, \mu)$.

Trước hết giả sử rằng X là compac, để lớp của hàm hằng 1 thuộc $L^2(X, \mu)$. Cho $g$ là một hàm trong $\mathscr{L}^2(X, \mu)$ mà lớp của nó trong $L^2(X, \mu)$ là $v(1)$.

Cho $c$ là một số thực dương và Y là tập các $x\in X$ sao cho $|g(x)|\geqslant c$; đó là một tập μ-đo được. Ta có trong $L^2(X, \mu)$ các đẳng thức $\varphi_{\widetilde{Y}}g=\widetilde{m}_{\varphi_Y}(v(1)) =v(m_{\varphi_Y}(1)) =v(\varphi_Y)$.

Hơn nữa, vì $|c\varphi_Y|\leqslant |g\varphi_Y|$, ta được

$$
c^2\mu(Y) =\int_X(c\varphi_Y)^2d\mu\leqslant \int_X|\varphi_Yg|^2d\mu=\|\widetilde{u}(\varphi_Y)\|^2\leqslant \|u\|^2\mu(Y)
$$

Bất đẳng thức này kéo theo $\mu(Y) = 0$ nếu $c >\|u\|$, do đó hàm $g$ bị chặn μ-hầu khắp nơi bởi $\|u\|$. Cuối cùng, với mọi hàm $f\in \mathscr{C}$(X), ta có

$$
u(\widetilde{f}) =v(m_f(1)) =\widetilde{m}_f(v(1)) =\widetilde{m}_f(\widetilde{g}) =\widetilde{m}_g(\widetilde{f})
$$

do đó có đẳng thức $u=\widetilde{m}_g$, và đặc biệt $N_{\infty}(g) =\|u\|$.

Xét bây giờ trường hợp tổng quát. Tồn tại một họ đếm được địa phương $(X_i)_{i\in I}$ các tập con compac rời nhau từng đôi một của X sao cho Z = X $-\bigcup_{i\in I}X_i$ là địa phương $\mu$-không đáng kể (INT, IV, p .190, § 5, n$^o9$, prop. 14). Ký hiệu $\mu_i$ là độ đo cảm sinh bởi $\mu$ trên $X_i$ (INT, IV, p. 186, § 5, n$^o7$, def. 4).

Theo prop. 1 của IV, p. 179, với mọi $i\in I$, ảnh $E_i$ của $\widetilde{m}_{\varphi_{Xi}}$ được đồng nhất với $L^2(X_i, \mu_i)$ bởi $f\mapsto f|X_i$. Với mọi hàm $g\in \mathscr{L}^{\infty}(X, \mu)$, tự đồng cấu phép nhân $\widetilde{m}_g$ giao hoán với $\widetilde{m}_{\varphi_{Xi}}$, do đó để $E_i$ ổn định, và tự đồng cấu của $E_i$ suy ra từ $\widetilde{m}_g$ bằng cách chuyển qua các không gian con trùng với tự đồng cấu phép nhân bởi $g|X_i$ trên $L^2(X_i, \mu_i)$.

Vì $u$ giao hoán với $m_{\varphi_{Xi}}$, nó cũng để không gian con $E_i$ ổn định. Ký hiệu $u_i$ là tự đồng cấu của $L^2(X_i, \mu_i)$ suy ra từ $u$ bằng cách chuyển qua các không gian con.

Ánh xạ từ $\mathscr{L}^{\infty}(X, \mu)$ vào $\mathscr{L}^{\infty}(X_i, \mu_i)$ xác định bởi $g\mapsto g|X_i$ là toàn ánh, nên giả thiết kéo theo rằng $u_i$ giao hoán với $\widetilde{m}_g$ với mọi hàm $g\in \mathscr{L}^{\infty}(X_i, \mu_i)$. Theo phần đầu của chứng minh, tồn tại một hàm $g_i\in \mathscr{L}^{\infty}(X_i, \mu_i)$ sao cho $u_i=\widetilde{m}_{g_i}$ và $N_{\infty}(g_i)\leqslant \|u_i\|\leqslant \|u\|$.

Hàm $g$ trên X trùng với $g_i$ trên $X_i$ và bằng không trên Z là bị chặn và $\mu$-đo được (INT, IV, p. 193, § 5, n$^o10$, prop. 16), do đó $g\in \mathscr{L}^{\infty}(X, \mu)$. Với mọi $i\in I$, hạn chế của $u$ lên $E_i$ trùng với hạn chế của $\widetilde{m}_g$; vì vậy ta có $u=m_g$ theo prop. 1, c) của IV, p. 179.

#### Hệ quả {#ts-iv-s2-n5-cor-2 .statement tag=02Z6}

Cho $u$ là một tự đồng cấu của không gian Hilbert $L^2(X, \mu)$ giao hoán với $\widetilde{m}_g$ với mọi hàm $g\in \mathscr{K}(X)$. Khi đó tồn tại một phần tử duy nhất $f\in L^{\infty}(X, \mu)$ sao cho $u=\widetilde{m}_f$.

Sau Mệnh đề 7, chỉ cần chứng minh rằng $u$ giao hoán với $\widetilde{m}_g$ với mọi $g\in \mathscr{L}^{\infty}(X, \mu)$. Cho $h_1$ và $h_2$ là các phần tử của $\mathscr{L}^2(X, \mu)$, có các lớp tương ứng $\widetilde{h}_1$ và $\widetilde{h}_2$ trong $L^2(X, \mu)$. Cho $k_1$ (tương ứng $k_2$) là một hàm trong $\mathscr{L}^2(X, \mu)$ mà lớp của nó là $u(\widetilde{h}_1)$ (tương ứng $u^*(\widetilde{h}_2)$).

Đặt $h=h_1\overline{k}_2-k_1\overline{h}_2$; khi đó $h\in \mathscr{L}^1(X, \mu)$. Định nghĩa độ đo $\nu =h\cdot \mu$ trên X; nó bị chặn. Với mọi $g\in \mathscr{L}^{\infty}(X, \mu)$, ta có

$$
\langle \widetilde{h}_2|u(\widetilde{m}_g(\widetilde{h}_1))-\widetilde{m}_g(u(\widetilde{h}_1))\rangle =\langle u^*(\widetilde{h}_2)|\widetilde{m}_g(\widetilde{h}_1)\rangle  - \langle \widetilde{h}_2|\widetilde{m}_g(u(\widetilde{h}_1))\rangle
$$

$$
=\int_Xg\cdot h_1\cdot \overline{k}_2d\mu-\int_Xg\cdot k_1\cdot \overline{h}_2d\mu=\nu (g)
$$

Vậy theo giả thiết $\nu (g) = 0$ với mọi hàm $g\in \mathscr{K}$ (X), nghĩa là $\nu = 0$. Do đó, suy ra

$$
\langle \widetilde{h}_2|u(\widetilde{m}_g(\widetilde{h}_1))-\widetilde{m}_g(u(\widetilde{h}_1))\rangle =\nu (g) = 0
$$

với mọi $g\in \mathscr{L}^{\infty}(X, \mu)$. Vì điều này đúng với mọi $h_1$ và $h_2$ trong $\mathscr{L}^2(X, \mu)$, ta có $u\circ \widetilde{m}_g=\widetilde{m}_g\circ u$.

#### Nhận xét {#ts-iv-s2-n5-rem-1 .statement tag=02Z7}

Trong phần sau, ta sẽ thường ký hiệu đơn giản bởi $m_g$ tự đồng cấu phép nhân bởi $g$ trên $L^p(X, \mu)$.

### 6. Độ đo phổ

Trong số này, ta cố định một không gian Hilbert phức E.

Nhắc lại rằng nếu A là một đại số sao có đơn vị giao hoán, thì người ta ký hiệu bởi $\mathsf{X}(A)$ không gian tôpô compắc các đặc trưng có đơn vị của nó (Hệ quả 1 của I, p. 29) và bởi $\mathscr{G}_A$ biến đổi Gelfand của A (Định nghĩa 5 của I, p. 7), là một đẳng cấu đẳng cự của các đại số sao có đơn vị đối hợp từ A lên $\mathscr{C}(\mathsf{X}(A))$ (Định lý 1 của I, p. 108). Ta sẽ ký hiệu bởi $\mathscr{H}_A$ đẳng cấu nghịch đảo.

#### Bổ đề 9 {#ts-iv-s2-lem-9 .statement tag=02Z8}

Cho A là một đại số con sao có đơn vị giao hoán của $\mathscr{L}(E)$. Với mọi $x$ và $y$ trong E, ánh xạ $\mu$ từ $\mathsf{X}(A)$ vào $\mathbf{C}$ được định nghĩa bởi $\mu(f) =\langle x|\mathscr{H}_A(f)y\rangle$ với mọi $f\in \mathscr{C}(\mathsf{X}(A))$ là một độ đo bị chặn trên không gian compắc $\mathsf{X}(A)$. Nó dương nếu $x=y$. Chuẩn của nó là $\leqslant \|x\| \|y\|$, với đẳng thức xảy ra nếu $x=y$.

Ánh xạ $\mu$ là tuyến tính. Với mọi hàm $f\in \mathscr{C}(\mathsf{X}$(A)), ta có

$$
|\mu(f)|\leqslant \|x\| \|y\| \|\mathscr{H}_A(f)\|=\|x\| \|y\| \|f\|
$$

do đó $\mu$ là một độ đo bị chặn trên $\mathsf{X}(A)$ có chuẩn $\leqslant \|x\| \|y\|$.

Giả sử $x=y$. Với mọi hàm dương $f\in \mathscr{C}(\mathsf{X}$(A)), phần tử $\mathscr{H}_A(f)$ là một phần tử dương của A (ví dụ 1 của I, p. 115), do đó là một phần tử dương của $\mathscr{L}$ (E), suy ra $\mu(f) =\langle x|\mathscr{H}_A(f)(x)\rangle \geqslant 0$ (mệnh đề 8 của I, p. 138). Điều này cho thấy rằng $\mu$ là một độ đo dương. Vì $\mu(1) =\|x\|^2$, khối lượng toàn phần của $\mu$ là $\|x\|^2$ (INT, III, p. 58, § 1, No.$^o8$, hệ quả 2).

#### Định nghĩa 2 {#ts-iv-s2-def-2 .statement tag=02Z9}

Cho A là một đại số con có sao giao hoán có đơn vị của $\mathscr{L}(E)$. Với mọi $x$ và $y$ trong E, dạng tuyến tính $f\mapsto  \langle x|\mathscr{H}_A(f)y\rangle$ trên $\mathscr{C}(\mathsf{X}(A))$ được gọi là độ đo phổ của $(x, y)$ đối với A. Nếu $x=y$, nó được gọi là độ đo phổ của $x$ đối với A.

#### Nhận xét {#ts-iv-s2-n6-rem-1 .statement tag=02ZA}

Cho A là một đại số con có sao giao hoán có đơn vị của $\mathscr{L}(E)$. Với mọi $x$ và $y$ trong E, ký hiệu $\mu_{x,y}$ là độ đo phổ của $(x, y)$ đối với A. Ánh xạ xác định bởi $(x, y)\mapsto \mu_{x,y}$ từ $E\times E$ vào $\mathscr{M}^1(\mathsf{X}(A))$ là nửa song tuyến tính.

Cho $u$ là một tự đồng cấu chuẩn tắc của E và A là đại số con có sao có đơn vị của $\mathscr{L}(E)$ sinh bởi $u$. Nó là giao hoán. Không gian $\mathsf{X}(A)$ được đồng nhất với Sp($u$) nhờ ánh xạ $\chi \mapsto \chi (u)$ (bổ đề 10 của I, p. 109). Do đó độ đo phổ $\mu_{x,y}$ của $(x, y)$ đối với A được đồng nhất với một độ đo trên Sp($u$), gọi là độ đo phổ của $(x, y)$ đối với $u$. Với mọi hàm $f\in \mathscr{C}$ (Sp($u$)), khi đó ta có

$$
\int f d\mu_{x,y}=\langle x|f(u)y\rangle
$$

Sp($u$)

theo định nghĩa 5 của I, p. 110.

### 7. Các đại số có sao giao hoán của các tự đồng cấu của một không gian Hilbert

#### Định nghĩa 3 {#ts-iv-s2-def-3 .statement tag=02ZB}

Cho A là một đại số trên $\mathbf{C}$ và E là một không gian vectơ tôpô phức. Cho $\pi$ là một biểu diễn của A trong E. Một phần tử $x$ của E được gọi là một vectơ cyclic đối với $\pi$ nếu tập các phần tử $\pi (a)x$ với $a\in A$ là toàn phần trong E.

Cho $u\in \mathscr{L}(E)$ là một tự đồng cấu của E. Ta nói rằng $x\in E$ là một vectơ cyclic đối với $u$ nếu nó là một vectơ cyclic đối với biểu diễn đồng nhất của đại số con có sao sinh bởi $u$ trong $\mathscr{L}(E)$.

#### Mệnh đề 8 {#ts-iv-s2-prop-8 .statement tag=02ZC}

Cho E là một không gian Hilbert phức. Cho A là một đại số con có sao giao hoán có đơn vị của $\mathscr{L}(E)$. Cho $x$ là một phần tử của E. Đặt $E_x= A\cdot x$ và ký hiệu $\mu_x$ là độ đo phổ của $x$ đối với A.

Tồn tại một đẳng cấu đẳng cự duy nhất $\theta_x$ từ $L^2(\mathsf{X}(A), \mu_x)$ lên $E_x$ sao cho $\theta_x(f) =\mathscr{H}_A(f)(x)$ với mọi hàm $f\in \mathscr{C}(\mathsf{X}(A))$. Với mọi phần tử $a\in A$, không gian $E_x$ ổn định dưới $a$, và nếu $a_x$ ký hiệu tự đồng cấu của $E_x$ suy ra từ $a$ bằng cách chuyển qua các không gian con, thì ta có $a_x\circ \theta_x=\theta_x\circ m_{\mathscr{G}_A(a)}$.

Gọi $\widetilde{\theta}_x$ là ánh xạ tuyến tính từ $\mathscr{C}(\mathsf{X}(A))$ vào $E_x$ được xác định bởi

$$
\widetilde{\theta}_x(f) =\mathscr{H}_A(f)(x)
$$

Với mọi hàm $f\in \mathscr{C}(\mathsf{X}$(A)), ta có

$$
\|\widetilde{\theta}_x(f)\|^2=\langle \mathscr{H}_A(f)x|\mathscr{H}_A(f)x\rangle =\langle x|\mathscr{H}_A(|f|^2)x\rangle =\int_{\mathsf{X}(A)}|f|^2d\mu_x
$$

Vì $\mathscr{C}(\mathsf{X}(A))$ trù mật trong $\mathscr{L}^2(\mathsf{X}(A), \mu_x)$, nên tồn tại một ánh xạ tuyến tính đẳng cự duy nhất từ $L^2(\mathsf{X}(A), \mu_x)$ vào $E_x$ kéo dài $\widetilde{\theta}_x$; gọi nó là $\theta_x$. Ánh xạ $\theta_x$ là toàn ánh vì ảnh của nó đóng (bổ đề 8 của I, p. 107) và chứa $A\cdot x$. Do đó nó là một đẳng cấu đẳng cự.

Gọi $a\in A$. Đặt $g=\mathscr{G}_A(a)\in \mathscr{C}(\mathsf{X}(A))$. Không gian $E_x$ ổn định dưới $a$. Khi đó, với $f\in \mathscr{C}(\mathsf{X}$(A)), ta có

$$
\widetilde{\theta}_x(m_g(f)) =\mathscr{H}_A(\mathscr{G}_A(a)f)x= (a\circ \mathscr{H}_A(f))x=a(\widetilde{\theta}_x(f))
$$

và suy ra rằng $\theta_x\circ m_g=a_x\circ \theta_x$.

#### Hệ quả {#ts-iv-s2-n7-cor-1 .statement tag=02ZD}

Cho E là một không gian Hilbert phức. Cho A là một đại số con stellar giao hoán có đơn vị của $\mathscr{L}(E)$ nhận một vectơ cyclic $x$. Gọi $\mu_x$ là độ đo phổ của $x$ đối với A. Tồn tại một đẳng cấu đẳng cự duy nhất

$$
\theta_x: L^2(\mathsf{X}(A), \mu_x)\rightarrow E
$$

sao cho $\theta_x(f) =\mathscr{H}_A(f)$ với mọi hàm $f\in \mathscr{C}(\mathsf{X}(A))$. Với mọi $a$ trong A, ta có $a\circ \theta_x=\theta_x\circ m_{\mathscr{G}_A(a)}$.

Thật vậy, khi đó ta có $E_x= E$ và $a_x=a$ với mọi $a\in A$.

Cho E là một không gian Hilbert phức. Cho $x\in E$ và cho A là một đại số con stellar giao hoán có đơn vị của $\mathscr{L}(E)$. Gọi $E_x$ là không gian con đóng $A\cdot x$ của E. Khi đó, với mọi $a\in A$, ta có $a(E_x)\subset E_x$. Gọi $A_x$ là đại số con stellar giao hoán có đơn vị của $\mathscr{L}(E_x)$ gồm các tự đồng cấu của $E_x$ suy ra từ các phần tử của A bằng cách chuyển qua các không gian con. Vectơ $x$ là một vectơ cyclic cho $A_x\subset \mathscr{L}(E_x)$.

#### Mệnh đề 9 {#ts-iv-s2-prop-9 .statement tag=02ZE}

Tồn tại một tập con C của E sao cho E là tổng Hilbert của các không gian $E_x$ với $x\in$ C. Nếu E thuộc kiểu đếm được, thì tập hợp C là đếm được.

Cho $\mathscr{O}$ là tập hợp các tập con C của E sao cho các không gian con $E_x$ với $x\in C$ trực giao từng đôi một. Tập hợp $\mathscr{O}$, được sắp thứ tự bởi quan hệ bao hàm, có kiểu hữu hạn (E, III, p. 34, Def. 2) vì C thuộc $\mathscr{O}$ khi và chỉ khi các tập hợp gồm hai phần tử của C thuộc $\mathscr{O}$. Theo E, III, p. 35, Định lý 1, tồn tại một phần tử cực đại C của $\mathscr{O}$.

Cho F là không gian con đóng của E sinh bởi các không gian con $E_x$ với $x\in C$. Chỉ cần chứng minh rằng $F^{\circ}$ rút gọn thành 0 là đủ để hoàn tất chứng minh của mệnh đề. Cho $y$ là một phần tử của $F^{\circ}$. Với mọi $x\in C$ và mọi $a$ và $b$ trong A, ta có $\langle a(y)|b(x)\rangle =\langle y|a^*b(x)\rangle = 0$ vì $a^*b(x)$ thuộc $E_x$, nên thuộc F. Vì các phần tử $a(y)$ (tương ứng $b(x)$) sinh một không gian con trù mật của $E_y$ (tương ứng $E_x$), do đó ta có $E_y\subset E^{\circ}_x$. Vì C là cực đại trong $\mathscr{O}$, điều này có nghĩa là $E_y$ rút gọn thành 0, do đó $y= 0$.

Giả sử rằng E có kiểu đếm được. Vì $E_x$ khác không với mọi $x\in C$ khác không, mọi tập hợp C sao cho E là tổng Hilbert của các không gian $E_x$ với $x\in C$ đều là đếm được.

#### Định lý 1 {#ts-iv-s2-thm-1 .statement tag=02ZF}

Cho A là một đại số con stellar giao hoán có đơn vị của $\mathscr{L}(E)$. Tồn tại một không gian tôpô compact địa phương X, một độ đo dương $\mu$ trên X, một đẳng cấu đẳng cự $\theta$ từ $L^2(X, \mu)$ lên E, và một cấu xạ đẳng cự của các đại số stellar $\pi$ từ A vào $\mathscr{C}_b(X)$ sao cho với mọi $a\in A$, ta có

$$
a\circ \theta =\theta \circ m_{\pi(a)}
$$

Theo Mệnh đề 9, tồn tại một tập con C của E sao cho E là tổng Hilbert của các không gian con $E_x$ với $x\in C$. Cho X là không gian tôpô compact địa phương $\mathsf{X}(A)\times C$, trong đó C được trang bị tôpô rời rạc. Tồn tại một độ đo duy nhất $\mu$ trên X sao cho $\mu|(\mathsf{X}(A)\times  \{x\})$ được đồng nhất với độ đo phổ $\mu_x$ của $x$ với mọi $x\in C$ (INT, III, p. 65, § 2, n$^o1$, Prop. 1); độ đo này là dương (xem chỗ đã dẫn). Khi đó ta có một phân tích thành tổng Hilbert

$$
L^2(X, \mu) =\bigoplus_{x\in C}L^2(\mathsf{X}(A), \mu_x)
$$

(Mệnh đề 1 của IV, p. 179, c) áp dụng cho các tập hợp $\mathsf{X}(A)\times  \{x\}$ với $x\in C)$. Do đó tồn tại một đẳng cự duy nhất $\theta : L^2(X, \mu)\rightarrow E$ trùng với $\theta_x: L^2(\mathsf{X}(A), \mu_x)\rightarrow E_x$ trên $L^2(\mathsf{X}(A), \mu_x)$ với mọi $x\in C$.

Cho $p: X\rightarrow \mathsf{X}(A)$ là phép chiếu chính tắc; nó là toàn ánh, nên ánh xạ tuyến tính $p^*:\mathscr{C}_b(\mathsf{X}(A))\rightarrow \mathscr{C}(X)$ xác định bởi $f\mapsto f\circ p$ là đơn ánh. Đặt $\pi =p^*\circ \mathscr{G}_A$; đó là một cấu xạ đơn ánh của các đại số stellar từ A vào $\mathscr{C}_b(X)$; do đó nó là đẳng cự (Mệnh đề 9 của I, p. 112).

Cho $a\in A$. Với mọi $x\in C$, ta có $a_x\circ \theta_x=\theta_x\circ m_{\mathscr{G}_A(a)}$. Do đó các ánh xạ tuyến tính liên tục $a\circ \theta$ và $\theta \circ m_{\pi(a)}$ trùng nhau trên các không gian con $L^2(\mathsf{X}(A), \mu_x)$, và vì thế bằng nhau.

#### Hệ quả (Định lý phổ) {#ts-iv-s2-n7-cor-2 .statement tag=02ZG}

Cho E là một không gian Hilbert phức. Cho $u\in \mathscr{L}(E)$ là một tự đồng cấu chuẩn tắc của E. Tồn tại một không gian tôpô compact địa phương X, một độ đo dương $\mu$ trên X, một đẳng cấu đẳng cự $\theta$ từ $L^2(X, \mu)$ lên E, và một hàm liên tục bị chặn $g$ trên X sao cho $u=\theta \circ m_g\circ \theta^{-1}$.

Nếu $u$ có một vectơ cyclic $x$, có thể lấy X = Sp($u$) và lấy $g$ là hàm đồng nhất của X.

Chỉ cần áp dụng định lý 1 (tương ứng là hệ quả của mệnh đề 8) cho đại số con có đối hợp A của $\mathscr{L}(E)$ sinh bởi $u$, và đặt $g=\pi (u)$.

Mệnh đề này quy mọi vấn đề liên quan đến một tự đồng cấu chuẩn tắc của một không gian Hilbert về một vấn đề tương tự đối với một toán tử nhân, điều này thường làm đơn giản việc nghiên cứu nó (xem chẳng hạn bài tập 19 của IV, p. 325).

### 8. Tính liên tục của phép tính phiếm hàm

Trong số này, ta xét các tính chất liên tục của phép tính phiếm hàm đối với hai biến.

Với một đại số có đối hợp A và một phần tử chuẩn tắc $a$ của A, và với một hàm liên tục $f$ trên một tập con của $\mathbf{C}$ chứa Sp$_A(a)$, ta ký hiệu bởi $f(a)$ phần tử thu được bằng phép tính phiếm hàm liên tục của $a$ áp dụng cho hạn chế của $f$ lên phổ của $a$.

#### Mệnh đề 10 {#ts-iv-s2-prop-10 .statement tag=02ZH}

Cho A là một đại số có đối hợp có đơn vị. Cho U là một tập con mở tương đối compact của $\mathbf{C}$. Cho $\Omega_n$ ký hiệu tập hợp các phần tử chuẩn tắc của A sao cho Sp$_A(a)$ được chứa trong U. Ánh xạ $(f, a)\mapsto f(a)$ từ $\mathscr{C}(U)\times \Omega_n$ vào A là liên tục.

Cho $q$ ký hiệu ánh xạ $(f, a)\mapsto f(a)$ từ $\mathscr{C}(U)\times \Omega_n$ vào A. Tập hợp các ánh xạ phép tính phiếm hàm $f\mapsto f(a)$ với $a\in \Omega_n$ là đồng liên tục trong $\mathscr{L}(\mathscr{C}(U); A)$, vì mỗi ánh xạ ấy là một ánh xạ tuyến tính liên tục có chuẩn $\leqslant 1$. Do đó, để chứng minh mệnh đề, chỉ cần kiểm tra rằng, với mọi $f\in \mathscr{C}$ (U), ánh xạ từ $\Omega_n$ vào A xác định bởi $a\mapsto f(a)$ là liên tục (TG, X, p. 13, hệ quả 3).

Cho $\mathscr{A}$ là tập hợp các $f\in \mathscr{C}(U)$ sao cho ánh xạ $a\mapsto f(a)$ từ $\Omega_n$ vào A là liên tục; còn lại phải chứng minh rằng $\mathscr{A}=\mathscr{C}(U)$.

Tập hợp $\mathscr{A}$ là một đại số con có đối hợp có đơn vị của $\mathscr{C}(U)$. Nó chứa hàm đồng nhất của U, và do đó tách các điểm. Vì vậy, nó trù mật trong $\mathscr{C}(U)$ (TG, X, p. 39, mệnh đề 7). Ta hãy chứng minh rằng nó đóng.

Cho $(f_n)$ là một dãy trong $\mathscr{A}$ hội tụ đến $f\in \mathscr{C}(U)$. Cho $\varepsilon  >0$ và chọn $n\in \mathbf{N}$ sao cho $\|f-f_n\|_{\infty}\leqslant \varepsilon /4$. Với mọi $(a_1, a_2)\in \Omega^2_n$ ta có

$$
\|f(a_1)-f(a_2)\|\leqslant 2\|f-f_n\|_{\infty}+\|f_n(a_1)-f_n(a_2)\|
$$

$$
\varepsilon
$$

$$
\leqslant +\|f_n(a_1)-f_n(a_2)\|
$$

2

Vì $f_n$ thuộc $\mathscr{A}$, tồn tại một lân cận V của $a_1$ trong $\Omega_n$ sao cho $\|f_n(a_1)-f_n(a_2)\|\leqslant \varepsilon /2$ với mọi $a_2\in$ V. Do đó $\|f(a_1)-f(a_2)\|\leqslant \varepsilon$ với mọi $a_2\in V$. Vì thế ánh xạ $a\mapsto f(a)$ liên tục tại $a_1$; mệnh đề được chứng minh.

#### Hệ quả 1 {#ts-iv-s2-prop-10-cor-1 .statement tag=02ZI}

Cho A là một star-đại số có đơn vị và gọi $A_n$ là tập hợp các phần tử chuẩn tắc của A. Trang bị cho không gian $\mathscr{C}(\mathbf{C})$ tôpô hội tụ compact. Ánh xạ $(f, a)\mapsto f(a)$ từ $\mathscr{C}(\mathbf{C})\times A_n$ vào A là liên tục.

Lấy $(f_0, a_0)\in \mathscr{C}(\mathbf{C})\times A_n$. Gọi U là một lân cận compact tương đối của phổ của $a_0$. Gọi V là tập hợp các phần tử chuẩn tắc $a$ của A sao cho Sp$_A(a)\subset U$; đó là một lân cận mở của $a_0$ trong $A_n$ (I, p. 76, Prop. 10). Với mọi $a\in V$ và mọi hàm $f\in \mathscr{C}(\mathbf{C})$, ta có $f(a) = (f|U)(a)$. Vì ánh xạ $f\mapsto  \|f|U\|_{\infty}$ là một nửa chuẩn liên tục trên $\mathscr{C}(\mathbf{C})$ được trang bị tôpô hội tụ compact, tính liên tục của ánh xạ $(f, a)\mapsto f(a)$ tại $(f_0, a_0)$ suy ra từ Prop. 10.

#### Hệ quả 2 {#ts-iv-s2-prop-10-cor-2 .statement tag=02ZJ}

Cho E là một không gian Hilbert phức và gọi $\mathscr{L}(E)_n$ là tập hợp các nội cấu chuẩn tắc của E. Trang bị cho không gian $\mathscr{C}(\mathbf{C})$ tôpô hội tụ compact. Ánh xạ từ $\mathscr{C}(\mathbf{C})\times \mathscr{L}(E)_n$ vào $\mathscr{L}(E)$ được xác định bởi $(f, u)\mapsto f(u)$ là liên tục.

## BÀI TẬP {#ts-iv-s2-exercises}

Trừ khi có nói rõ khác đi, trong các bài tập của đoạn này, E ký hiệu một không gian Hilbert phức.

Xem [các bài tập của § 2](exercises/s2/).
