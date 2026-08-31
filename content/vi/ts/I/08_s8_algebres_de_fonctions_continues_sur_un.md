---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 8
section_title: Algèbres de fonctions continues sur un espace compact
lang: vi
source: ts-i-ii-fr
book_pages: TS I.142-TS I.151, TS I.191-TS I.197
pdf_pages: 0155-0164, 0204-0210
extraction: native
subsections:
    - "no": 1
      title: Sous-algèbres de l’algèbre des fonctions continues sur un espace compact
      page: 142
      pdf_page: 155
    - "no": 2
      title: Fonctions continues sur un sous-ensemble compact de $\mathbf{C}^{\Lambda}$
      page: 146
      pdf_page: 159
    - "no": 3
      title: Fonctions continues sur un sous-ensemble compact de C
      page: 148
      pdf_page: 161
statements: 11
exercises: 11
content_sha256: 1745f9465b418fd63aba5f7aa7bbcd4f2436f8ac2bc206aeb84499cf7b2e5ec4
translated_from: content/en-mt/ts/I/08_s8_algebres_de_fonctions_continues_sur_un.md
source_lang: en-mt
translation_method: machine
source_content_sha256: d8f7b6ac584fa670d9d39d065ac50a5e2ff38fc71c4b21390194bd47731cada3
translation_model: gpt-5-6-mini
translation_run: translate-vi-db071105
glossary_version: 34
glossary_terms_sha256: a06523da5345110305d1aa49f6ac8a6db7a9de7f7b110a275d72adea9193fa8d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. ĐẠI SỐ CÁC HÀM LIÊN TỤC TRÊN MỘT KHÔNG GIAN COMPACT

Trong đoạn này, trường cơ sở là $\mathbf{C}$.

### 1. Các đại số con của đại số các hàm liên tục trên một không gian compact

Cho X là một không gian tôpô compact và B là một đại số con có đơn vị của $\mathscr{C}(X)$. Ta ký hiệu ev là ánh xạ $x\mapsto$ ev$_x$ từ X vào $\mathsf{X}(B)$ sao cho ev$_x(f) =f(x)$ với mọi $f\in B$. Ta ký hiệu $j$ là đơn ánh từ B vào $\mathscr{C}(X)$, do đó $\mathsf{X}(j) =$ ev.

#### Mệnh đề 1 {#ts-i-s8-prop-1 .statement tag=02H4}

Cho $f\mapsto  \|f\|_B$ là một chuẩn biến B thành một đại số Banach.

a) Ánh xạ $j$ có chuẩn $\leqslant 1$ trong $\mathscr{L}(B;\mathscr{C}(X))$ ;

b) Căn của đại số B là không ;

c) Ánh xạ ev liên tục từ X vào $\mathsf{X}(B)$ ;

d) Nếu B phân biệt các điểm của X, thì ánh xạ ev là một phép đồng phôi từ X lên một tập con đóng của $\mathsf{X}(B)$.

Có thể đồng nhất X với $\mathsf{X}(\mathscr{C}(X))$ và $\mathscr{G}_{\mathscr{C}(X)}$ với ánh xạ đồng nhất (ví dụ 1 của I, p. 36). Khi đó ánh xạ ev được đồng nhất với $\mathsf{X}(j)$, điều này chứng minh c).

Với mọi hàm $f\in B$ và mọi $x\in X$, ta có $\mathscr{G}_B(f$)(ev$_x$) $=f(x)$, do đó

$\|f\|_{\mathscr{C}(X)}=$ sup$_{x\in X}|\mathscr{G}_B(f$)(ev$_x$)$|\leqslant \varrho_B(f)\leqslant \|f\|_B$,

(xem mệnh đề 7 của I, p. 38, a)) suy ra a). Hơn nữa, điều này cho thấy biến đổi Gelfand của B là đơn ánh, do đó b) (mệnh đề 8 của I, p. 38). Nếu B phân biệt các điểm của X, thì ánh xạ ev là đơn ánh, do đó d) vì X compact.

Bây giờ ta xét tính toàn ánh của ánh xạ ev.

#### Mệnh đề 2 {#ts-i-s8-prop-2 .statement tag=02H5}

Cho $f\mapsto  \|f\|_B$ là một chuẩn sao cho $(B,\|\cdot \|_B)$ là một đại số Banach.

a) Nếu ánh xạ ev là toàn ánh, thì đại số B là một đại số con đầy đủ của $\mathscr{C}(X)$ ;

b) Giả sử rằng B là một đại số con đầy đủ của $\mathscr{C}(X)$, và tồn tại một phần tử $a\in B$ sao cho tập hợp các phần tử $f(a)$, trong đó f chạy trên tập hợp các hàm hữu tỉ trên $\mathbf{C}$ không có cực tại Sp$_B(a)$, là trù mật trong B. Khi đó ánh xạ ev là toàn ánh ;

c) Nếu B là một đại số con đầy đủ bất biến qua phép liên hợp của $\mathscr{C}(X)$, thì ánh xạ ev là toàn ánh.

Mệnh đề a) suy ra từ mệnh đề 10 của I, p. 40, và mệnh đề b) từ mệnh đề 11 của I, p. 41, vì đại số con đầy đủ của B sinh bởi $a$ là tập hợp các phần tử $f(a)$, trong đó f chạy trên tập hợp các hàm hữu tỉ trên $\mathbf{C}$ không có cực tại Sp$_B(a)$ (bổ đề I, p. 6 và mệnh đề 6 của I, p. 37, b)).

Hãy chứng minh c). Khi đó, giả sử $B$ là một đại số con bất biến đầy đủ của $\mathscr{C}(X)$. Để chứng minh rằng ev là toàn ánh, chỉ cần chứng minh rằng với mọi $\chi \in \mathsf{X}(B)$, tồn tại $y\in X$ sao cho Ker($\chi$ ) $=$ Ker(ev$_y$) (th. 2 của I, p. 30). Đặt I = Ker($\chi$ ). Đó là một iđêan cực đại của B. Gọi Φ là tập hợp các $x\in X$ sao cho $f(x) = 0$ với mọi $f\in I$. Ta hãy chứng minh rằng Φ không rỗng. Nếu không, vì X compact, sẽ tồn tại một số nguyên $n\geqslant 1$, một phủ mở $(V_1, . . . ,V_n)$ của X và, với mỗi số nguyên $i$ sao cho $1\leqslant i\leqslant n$, một hàm $f_i\in I$ sao cho $f_i(x)\not= 0$ với mọi $x\in V_i$. Vì đại số B là một đại số con bất biến của $\mathscr{C}(X)$, hàm

$$
f=\sum_{i=1}^nf_i\overline{f}_i
$$

sẽ thuộc I. Khi đó $f(x)>0$ với mọi $x\in X$, và do đó f sẽ khả nghịch trong $\mathscr{C}(X)$. Vì B được giả thiết là một đại số con đầy đủ của $\mathscr{C}(X)$, hàm $f\in$ I sẽ khả nghịch trong B, điều này là không thể. Do đó, tập hợp Φ không rỗng. Lấy $y$ là một phần tử của Φ; hạt nhân của đặc trưng ev$_y$ chứa I, và do đó bằng I.

#### Ví dụ {#ts-i-s8-n1-exa-1 .statement tag=02H6}

Cho $X = [0,1]$ và cho $n\geqslant 0$ là một số nguyên. Gọi B là đại số các hàm $f: X\rightarrow \mathbf{C}$ có các đạo hàm liên tục trên $[0,1]$ đến cấp $n$, được trang bị chuẩn đã xét trong ví dụ 4 của I, p. 18. Khi đó B là một đại số con bất biến đầy đủ của $\mathscr{C}(X)$ tách các điểm của X, do đó $\mathsf{X}(B)$ được đồng nhất với X.

Ta xét hàm lôgarit được định nghĩa trên $\mathbf{R}_+$ và nhận giá trị trong $\mathbf{R}\cup  \{-\infty \}$ bằng cách đặt log(0) $=-\infty$.

#### Mệnh đề 3 {#ts-i-s8-prop-3 .statement tag=02H7}

Cho X là một không gian compact. Cho B là một đại số con Banach có đơn vị của $\mathscr{C}(X)$, được trang bị chuẩn cảm sinh, tách các điểm của X. Ta đồng nhất X với một tập con đóng của $\mathsf{X}(B)$ (mệnh đề 1, d)).

a) Với mọi $f\in B$, biến đổi Gelfand $\mathscr{G}_B(f)$ là một hàm liên tục trên $\mathsf{X}(B)$ mở rộng f và thỏa mãn $\|f\|=$ sup$|\mathscr{G}_B(f)|$. Đặc biệt, $\mathscr{G}_B$ là một đẳng cấu đẳng chuẩn của B lên một đại số con Banach của $\mathscr{C}(\mathsf{X}(B))$ ;

b) Gọi $B^*$ là tập hợp các phần tử khả nghịch của B. Với mọi đặc trưng $\chi \in \mathsf{X}(B)$, tồn tại một độ đo dương $\mu$ có khối lượng 1 trên X sao cho, với mọi $f\in B^*$, ta có

log($|\chi (f)|$) $=\int_X$ log($|f|$)$d\mu$.

Hơn nữa, với mọi $f\in B$, ta có

$$
\chi (f) =\int_Xf d\mu
$$

c) Giả sử mọi phần tử của $\mathscr{C}_{\mathbf{R}}(X)$ đều là giới hạn đều của phần thực của các hàm thuộc B. Khi đó, với mọi $\chi \in \mathsf{X}(B)$, tồn tại duy nhất một độ đo $\mu_{\chi}\geqslant 0$ trên X sao cho, với mọi hàm $f\in B$, ta có

$$
\chi (f) =\int_Xf d\mu_{\chi}
$$

Hơn nữa, với mọi hàm $f\in B$, ta có

log($|\chi (f)|$)$\leqslant \int_X$ log($|f|$)$d\mu_{\chi}$; hàm log$|f|$ bị chặn trên, nên tích phân tồn tại trong $\mathbf{R}\cup  \{-\infty \}$.

Mệnh đề a) suy ra từ việc đồng nhất X với một không gian con đóng của $\mathsf{X}(B)$ và từ các bất đẳng thức

$\|f\|=$ sup$_{x\in X}|f(x)|\leqslant$ sup$_{\chi\in\mathsf{X}(B)}|\chi (f)|=$ sup$|\mathscr{G}_B(f)|=\varrho_B(f)\leqslant \|f\|$

với mọi $f\in B$.

Cho $\chi \in \mathsf{X}(B)$ và n là một số nguyên dương. Cho $\lambda_1, . . . , \lambda_n\in \mathbf{R}$ và $f_1, . . . , f_n\in B^*$. Khi đó ta có

(1) $\sum_{i=1}^n\lambda_i$ log($|\chi (f_i)|$)$\leqslant$ sup$_{x\in X}(\sum_{i=1}^n\lambda_i$ log($|f_i(x)|$)).

Thật vậy, do tính liên tục, chỉ cần chứng minh bất đẳng thức này khi các số thực $\lambda_i$ là hữu tỉ. Quy về một mẫu số chung, ta đưa được về trường hợp $\lambda_i\in \mathbf{Z}$ với mọi $i$. Khi đó bất đẳng thức có dạng

log($|\chi (f_1^{\lambda_1}\cdots f_n^{\lambda_n})|$)$\leqslant$ sup$_{x\in X}$ log($|(f_1^{\lambda_1}\cdots f_n^{\lambda_n})(x)|$),

và suy ra từ $\|\chi \|= 1$ (th. 1 của I, p. 29).

Cho $B'$ là không gian vectơ sinh trong $\mathscr{C}_{\mathbf{R}}(X)$ bởi các hàm log($|f|$) với $f\in B^*$. Cận trên (1) chứng minh rằng tồn tại một dạng tuyến tính $h$ có chuẩn $\leqslant$ 1 trên $B'$ sao cho log($|\chi (f)|$) $=h$(log($|f|$)) với mọi $f\in B^*$. Theo định lý Hahn-Banach (EVT, II, p. 24, cor. 2), dạng tuyến tính $h$ mở rộng thành một dạng tuyến tính $\mu$ có chuẩn $\leqslant$ 1 trên $\mathscr{C}_{\mathbf{R}}(X)$, tức là, thành một độ đo thực $\mu$ trên X sao cho $\|\mu\|\leqslant 1$ (INT, III, §1, n$^o5$). Lấy phần tử $f$ của $B^*$ là hằng $e=$ exp(1), ta thấy rằng $1 =\mu(1)$. Do đó, viết $\mu=\mu^+-\mu^-$ dưới dạng hiệu của hai độ đo dương kỳ dị lẫn nhau (INT, III, §1, n$^o6$, th. 3), ta được

$$
1 =\mu^+(1)-\mu^-(1)\leqslant \mu^+(1) +\mu^-(1) =\|\mu\|\leqslant 1
$$

do đó $\mu=\mu^+\geqslant 0$ và $\|\mu\|= 1$.

Với mọi $f\in B$, ta có exp($f$)$\in B^*$, do đó

$\int_X\mathscr{R}(f)d\mu=\int_X$ log($|$exp($f$)$|$)$d\mu=$ log($|\chi$(exp($f$))$|$)

= log($|$exp($\chi (f)$)$|$) $=\mathscr{R}(\chi (f))$,

trong đó Hệ quả 1 của I, p. 66 đã được sử dụng. Áp dụng đẳng thức này cho $if$, ta kết luận rằng $\int_Xf d\mu=\chi (f)$. Điều này thiết lập b).

Ta xét dưới các giả thiết của c). Sự tồn tại của $\mu_{\chi}$ suy ra từ b). Mặt khác, ta có $\mu_{\chi}(\mathscr{R}(f)) =\mathscr{R}(\chi (f))$ với mọi $f\in B$. Vì phần thực của các hàm $f\in B$ là trù mật trong $\mathscr{C}_{\mathbf{R}}(X)$ theo giả thiết, độ đo $\mu_{\chi}$ được xác định duy nhất bởi $\chi$.

Cho $f\in B$. Cho $\varepsilon  >0$ là một số thực. Theo giả thiết, tồn tại một hàm $g\in B$ sao cho

(2) $\mathscr{R}(g)-\varepsilon \leqslant$ log($|f|+\varepsilon$ )$\leqslant \mathscr{R}(g) +\varepsilon$.

Đặt $h=$ exp($g$)$\in B^*$. Theo (2), ta có

$$
|h|e^{-\varepsilon}\leqslant |f|+\varepsilon \leqslant |h|e^{\varepsilon} \tag{3}
$$

Cận trên suy ra $|f h^{-1}|\leqslant e^{\varepsilon}$, do đó $|\chi (f h^{-1})|\leqslant e^{\varepsilon}$, và do đó

(4) log($|\chi (f)|$)$\leqslant$ log($|\chi (h)|$) $+\varepsilon =\int_X$ log($|h|$)$d\mu_{\chi}+\varepsilon$.

Cận dưới trong (3) khi đó suy ra

log($|\chi (f)|$)$\leqslant \int_X$ log $(|f|+\varepsilon )d\mu_{\chi}+ 2\varepsilon$.

Cho $\varepsilon$ tiến tới 0, ta suy ra rằng

log($|\chi (f)|$)$\leqslant \int_X$ log($|f|$)$d\mu_{\chi}$.

Điều này hoàn thành chứng minh.

### 2. Các hàm liên tục trên một tập con compact của $\mathbf{C}^{\Lambda}$

Cho Λ là một tập hợp và X là một tập con compact của $\mathbf{C}^{\Lambda}$. Ta ký hiệu P(X) là đại số con Banach có đơn vị của $\mathscr{C}(X)$ gồm các hàm trên X là các giới hạn đều trên X của các hàm đa thức trên $\mathbf{C}^{\Lambda}$. Các hàm tọa độ $z_{\lambda}|X$ sinh P(X) về mặt tôpô, và P(X) phân biệt các điểm của X. Gọi Y là bao lồi đa thức của X (Định nghĩa 4 của I, p. 45). Vì

sup$_{z\in Y}|p(z)|=$ sup$_{z\in X}|p(z)|$

(cf. No.$^o7$ of I, p. 44) với mọi $p\in \mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$, các dãy đa thức hội tụ đều trên X được mở rộng duy nhất thành các dãy đa thức hội tụ đều trên Y. Do đó tồn tại một đẳng cấu đẳng cự duy nhất từ P(X) lên P(Y), biến, với mọi hàm tọa độ $z_{\lambda}$ trên $\mathbf{C}^{\Lambda}$, $z_{\lambda}|X$ thành $z_{\lambda}|Y$. Đẳng cấu này được gọi là chính tắc.

#### Mệnh đề 4 {#ts-i-s8-prop-4 .statement tag=02H8}

Cho X là một không gian compact. Cho B là một đại số con Banach có đơn vị của $\mathscr{C}(X)$, được trang bị chuẩn cảm sinh và tách các điểm của X. Ta đồng nhất X với một tập con đóng của $\mathsf{X}(B)$ (Mệnh đề 1 của I, p. 142, d)). Cho $(x_{\lambda})_{\lambda\in\Lambda}$ là một họ các phần tử của B sinh về mặt tôpô đại số có đơn vị B. Xét biểu đồ giao hoán

$$
\leftarrow_i
$$

X $\rightarrow \mathsf{X}(B)$

$$
\rightarrow \leftarrow_{\varphi}\rightarrow \leftarrow_{\varphi'}
$$

$$
_{\Lambda}\leftarrow_{j\Lambda}
$$

Sp$_{\mathscr{C}(X)}((x_{\lambda}))\rightarrow$ Sp$_B((x_{\lambda}))$

trong đó $\varphi$ và $\varphi '$ là các ánh xạ được xác định bởi họ $(x_{\lambda})_{\lambda\in\Lambda}($cf. No.$^o6$ of I, p. 41), còn i và j là các phép nhúng chính tắc. Khi đó:

a) Các ánh xạ $\varphi$ và $\varphi '$ là các đồng phôi;

b) Phổ chung Sp$^{\Lambda}_B((x_{\lambda}))$ là bao lồi đa thức của Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda}))$;

c) Ánh xạ $\varphi$ biến $\mathscr{C}(X)$ thành $\mathscr{C}$(Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda}))$) và B thành P(Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda}))$) ;

d) Ánh xạ $\varphi '$ biến $\mathscr{G}_B(B)$ thành P(Sp$^{\Lambda}_B((x_{\lambda}))$) ;

e) Các ánh xạ $\varphi$ và $\varphi '$ biến $\mathscr{G}_B$ thành đẳng cấu chính tắc của P(Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda}))$) lên P(Sp$^{\Lambda}_B((x_{\lambda}))$).

Các ánh xạ $\varphi$ và $\varphi '$ liên tục và toàn ánh (No.$^o6$ of I, p. 41). Ánh xạ $\varphi '$ là một đồng phôi theo mệnh đề a) của Mệnh đề 12 của I, p. 43, và $i$ là đơn ánh, do đó $\varphi$ là đơn ánh. Vì vậy $\varphi$ và $\varphi '$ là các đồng phôi.

Đặt $X_1$ = Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda}))$. Bao lồi đa thức của $X_1$ là $Y_1=$ Sp$^{\Lambda}_B((x_{\lambda}))$ theo Mệnh đề 14 của I, p. 46.

Với mỗi $\lambda \in \Lambda$, ký hiệu $z_{\lambda}$ là hàm tọa độ tương ứng trên $\mathbf{C}^{\Lambda}$. Ánh xạ $\varphi$ biến đổi $x_{\lambda}$ thành $z_{\lambda}|X_1$, và $\varphi '$ biến đổi $\mathscr{G}_B(x_{\lambda})$ thành $z_{\lambda}|Y_1$. Do đó $\varphi$ biến đổi B thành $P(X_1)$, và $\varphi '$ biến đổi $\mathscr{G}_B(B)$ thành $P(Y_1)$. Cuối cùng, $\varphi$ và $\varphi '$ biến đổi $\mathscr{G}_B$ thành đẳng cấu chính tắc của $P(X_1)$ lên $P(Y_1)$.

#### Hệ quả 1 {#ts-i-s8-prop-4-cor-1 .statement tag=02H9}

Cho Λ là một tập hợp và X là một tập compact của $\mathbf{C}^{\Lambda}$. Ta đồng nhất X với một tập con của $\mathsf{X}(P(X))$ (mệnh đề 1 của I, p. 142, d)). Gọi $(z_{\lambda})_{\lambda\in\Lambda}$ là họ các hàm tọa độ trên $\mathbf{C}^{\Lambda}$.

a) Ánh xạ $\theta$ từ $\mathsf{X}(P(X))$ lên Sp$^{\Lambda}_{P(X)}((z_{\lambda}))$ được xác định bởi họ $(z_{\lambda})$ là một đồng phôi của $\mathsf{X}(P(X))$ lên bao lồi đa thức Y của X. Hạn chế của nó trên X là ánh xạ đồng nhất của X ;

b) Với mọi hàm $f\in P(X)$, đồng phôi $\theta$ biến đổi phép kéo dài $\mathscr{G}_{P(X)}(f)$ của f lên $\mathsf{X}(P(X))$ thành một phép kéo dài $\widetilde{f}$ của f lên Y. Ánh xạ $f\mapsto \widetilde{f}$ là đẳng cấu chính tắc của P(X) lên P(Y).

Trong mệnh đề 4, lấy B = P(X) và $x_{\lambda}=z_{\lambda}$. Khi đó $\varphi$ trở thành ánh xạ đồng nhất và $\varphi '$ trở thành ánh xạ $\theta$. Các khẳng định của hệ quả khi đó được quy về các khẳng định của loc. cit.

#### Hệ quả 2 {#ts-i-s8-prop-4-cor-2 .statement tag=02HA}

Cho Λ là một tập hợp và cho $X\subset \mathbf{C}^{\Lambda}$ là một tập compact. Nếu X liên thông, thì bao lồi đa thức của nó liên thông.

Nếu X liên thông, các phần tử lũy đẳng duy nhất của $\mathscr{C}(X)$, và do đó của P(X), là 0 và 1 (hệ quả của mệnh đề I, p. 79). Do đó, không gian $\mathsf{X}(P(X))$ liên thông (loc. cit.); nay tập hợp này đồng phôi với bao lồi đa thức của X (hệ quả 1, a)).

### 3. Các hàm liên tục trên một tập compact của C

#### Bổ đề 1 {#ts-i-s8-lem-1 .statement tag=02HB}

Cho X là một tập compact của mặt phẳng và O là một thành phần liên thông bị chặn của $\mathbf{C}-$ X. Biên của O được chứa trong X.

Bao đóng của tập hợp O trong $\mathbf{C}-$ X bằng $\overline{O}\cap (\mathbf{C}-$ X) trong đó $\overline{O}$ là bao đóng của nó trong $\mathbf{C}$. Vì O là một thành phần liên thông của $\mathbf{C}-$ X, do đó ta có $\overline{O}\cap (\mathbf{C}-$ X) = O$, điều này chứng minh rằng $\overline{O}-O\subset X$.

Cho X là một tập compact của $\mathbf{C}$. Gọi $O_{\infty}$ là thành phần liên thông không bị chặn của $\mathbf{C}-$X$, và $(O_i)_{i\in I}$ là họ các thành phần liên thông bị chặn của $\mathbf{C}-$ X, các tập con $O_i$ từng đôi một phân biệt.

Cho E là một tập con của $\mathbf{C}-$ X. Ta ký hiệu $R_E(X)$ là bao đóng trong $\mathscr{C}(X)$ của tập hợp các hàm $f|X$, trong đó $f$ là một hàm hữu tỉ trên $\mathbf{C}$ mà mọi cực của nó đều thuộc E. Đại số $R_E(X)$ là một đại số con Banach có đơn vị của $\mathscr{C}(X)$, tách các điểm của X. Cho $z$ là hàm đồng nhất trên X. Đại số con đóng đầy đủ của $R_E(X)$ sinh bởi $z$ bằng $R_E(X)$ (Bổ đề 2 của I, p. 6). Các phần tử của $R_E(X)$ là toàn hình trong phần trong của X.

Đặc biệt, ta có $R_{\emptyset}(X) = P(X)$. Ta viết $R(X) = R_{\mathbf{C}-X}(X)$. Cho I(E) là tập hợp các phần tử $i\in I$ sao cho $E\cap O_i=\emptyset$, và

$$
X_E= X\cup (\bigcup_{i\in I(E)}O_i)
$$

Tập hợp $X_E$ là compact, vì bị chặn và đóng, phần bù của nó trong $\mathbf{C}$ là hợp của tập mở $O_{\infty}$ và các tập mở $O_i$ giao với E.

#### Mệnh đề 5 {#ts-i-s8-prop-5 .statement tag=02HC}

Với ký hiệu trên:

a) Ánh xạ hạn chế $h$ từ $R_E(X_E)$ vào $R_E(X)$ là một đẳng cấu đẳng cự;

b) Đại số $R_E(X_E)$ là một đại số con đầy đủ của $\mathscr{C}(X_E)$;

c) Mọi đặc trưng của $R_E(X_E)$ đều có dạng $f\mapsto f(w)$, trong đó w là một phần tử của $X_E$;

d) Ánh xạ $\chi \mapsto \chi (z)$ là một phép đồng phôi của $\mathsf{X}(R_E(X))$ lên $X_E$;

e) Nếu $E'$ là một tập con của $\mathbf{C}-$ X, thì $R_E(X) = R_{E'}(X)$ khi và chỉ khi $X_E= X_{E'}$, điều này cũng tương đương với $I(E) = I(E')$.

Ánh xạ hạn chế $h$ của $R_E(X_E)$ vào $R_E(X)$ là một cấu xạ của các đại số Banach sao cho $\|h(f)\|\leqslant \|f\|$ với mọi hàm $f\in R_E(X_E)$. Cho $f\in R_E(X_E)$. Cho $i\in I(E)$. Vì $f$ là hàm chỉnh hình trong một lân cận của tập mở bị chặn $O_i$, nguyên lý cực đại (VAR, I, p. 29) suy ra tồn tại một phần tử $z_0$ trên biên của $O_i$ sao cho $|f(z_0)|=$ sup$_{z\in O_i}|f(z)|$. Vì biên của $O_i$ được chứa trong X (bổ đề 1), suy ra sup$_{z\in O_i}|f(z)|\leqslant \|h(f)\|$. Vì bất đẳng thức này đúng với mọi $i\in I(E)$, suy ra $\|f\|\leqslant \|h(f)\|$. Do đó cấu xạ $h$ là đẳng cự, và đặc biệt là đơn ánh. Bây giờ chứng minh rằng nó toàn ánh. Cho $g\in R_E(X)$. Tồn tại một dãy $(f_n)$ các hàm hữu tỉ có các cực thuộc E, hội tụ đều đến $g$ trên X. Các $f_n|X_E$ là các phần tử của $R_E(X_E)$. Vì $h$ là đẳng cự, dãy $(f_n|X_E)$ hội tụ trong $\mathscr{C}(X_E)$. Nếu $f$ là giới hạn của nó, thì $f\in R_E(X_E)$ và $g=f|X =h(f)$. Do đó a).

Chứng minh mệnh đề d). Áp dụng mệnh đề 3 của I, p. 144 cho đại số $B = R_E(X)$. Mệnh đề b) của tài liệu đã dẫn suy ra rằng ánh xạ gán cho $\chi$ phần tử $\chi (z)$ là một đồng phôi từ $\mathsf{X}(R_E(X))$ lên Sp$_{R_E(X)}(z)$. Gọi $z_E$ là ánh xạ đồng nhất của $X_E$. Theo tài liệu đã dẫn, a), ta có Sp$_{R_E(X)}(z) =$ Sp$_{R_E(X_E)}(z_E)$. Do đó chỉ cần chứng minh rằng Sp$_{R_E(X_E)}(z_E) = X_E$. Hệ quả của mệnh đề 6 của I, p. 28 chứng minh rằng Sp$_{R_E(X_E)}(z_E)$ là hợp của Sp$_{\mathscr{C}(X_E)}(z_E) = X_E$ và một số thành phần liên thông bị chặn của phần bù của $X_E$. Cho $O_i$ là một trong các thành phần liên thông bị chặn của phần bù của $X_E$. Khi đó giao $E\cap O_i$ là khác rỗng. Lấy $\lambda \in E\cap O_i$; vì $(\lambda -z_E)^{-1}\in R_E(X_E)$, ta có $\lambda \notin$ Sp$_{R_E(X_E)}(z_E)$. Do đó, $O_i$ không được chứa trong Sp$_{R_E(X_E)}(z_E)$. Điều này chứng minh rằng Sp$_{R_E(X_E)}(z_E) = X_E$.

Hơn nữa, đẳng thức này suy ra rằng Sp$_{R_E(X_E)}(z_E) =$ Sp$_{\mathscr{C}(X_E)}(z_E)$. Điều này thiết lập điều kiện (iii) của mệnh đề 11 của I, p. 41, áp dụng cho đơn ánh chính tắc của $R_E(X_E)$ vào $\mathscr{C}(X_E)$ và cho phần tử $z_E$. Các mệnh đề b) và c) là các điều kiện tương đương (i) và (ii) của tài liệu đã dẫn.

Mệnh đề d) cho thấy $X_E= X_{E'}$ nếu $R_E(X) = R_{E'}(X)$. Ngược lại, giả sử $X_E= X_{E'}$. Thay thế $E'$ bởi $E\cup E'$, ta có thể giả sử rằng $E\subset E'$. Theo b), đại số $R_E(X_E)$ là một đại số con đầy đủ đóng của $\mathscr{C}(X_E)$, và do đó cũng là một đại số con của $R_{E'}(X_E)$. Nó chứa $z_E$, và do đó $R_E(X_E) = R_{E'}(X_E)$. Áp dụng a), ta suy ra $R_E(X) = R_{E'}(X)$. Cuối cùng, tính tương đương của $X_E= X_{E'}$ và $I(E) = I(E')$ là một hệ quả của các định nghĩa.

#### Hệ quả 1 {#ts-i-s8-prop-5-cor-1 .statement tag=02HD}

Các điều kiện sau là tương đương:

(i) Tập hợp E gặp mọi thành phần liên thông bị chặn của $\mathbf{C}-$ X ;

(ii) Ánh xạ $\chi \mapsto \chi (z)$ là một đồng phôi từ $\mathsf{X}(R_E(X))$ lên X ;

(iii) Ta có $R_E(X) = R(X)$.

Đặt $E'=\mathbf{C}-$ X. Các điều kiện (i), (ii) và (iii) lần lượt tương đương với $I(E) = I(E')$, với $X_E= X_{E'}$ (theo mệnh đề 5, d)) và với $R_E(X) = R_{E'}(X)$. Do đó chúng tương đương với nhau theo mệnh đề 5, e).

Hệ quả sau đây làm cho định lý Runge chính xác hơn (định lý 3 của I, p. 69).

#### Hệ quả 2 (Định lý Runge) {#ts-i-s8-prop-5-cor-2 .statement tag=02HE}

Với mỗi $i\in I$, cho $\lambda_i$ là một điểm của $O_i$. Cho $f$ là một hàm phức chỉnh hình trong một lân cận mở của X. Khi đó $f|X$ là giới hạn đều của các hạn chế lên X của những phân thức hữu tỉ mà các cực của chúng là một số trong các $\lambda_i$.

Với $E =\{\lambda_i\}_{i\in I}$, giả thiết là điều kiện (i) của hệ quả 1. Do đó $R_E(X) = R(X)$, và định lý 3 của I, p. 69 cho thấy rằng $R(X) =\mathscr{O}(X)$.

## BÀI TẬP {#ts-i-s8-exercises}

Tất cả các không gian Banach và tất cả các đại số Banach dưới đây đều là phức.

Xem [các bài tập của § 8](exercises/s8/).
