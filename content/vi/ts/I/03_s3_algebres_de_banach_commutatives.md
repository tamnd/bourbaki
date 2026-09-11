---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 3
section_title: Algèbres de Banach commutatives
lang: vi
source: ts-i-ii-fr
book_pages: TS I.29-TS I.49, TS I.166-TS I.172
pdf_pages: 0042-0062, 0179-0185
extraction: native
subsections:
    - "no": 1
      title: Caractères d’une algèbre de Banach commutative
      page: 29
      pdf_page: 42
    - "no": 2
      title: Fonctions continues nulles à l’infini sur un espace localement compact
      page: 31
      pdf_page: 44
    - "no": 3
      title: Applications partielles propres
      page: 33
      pdf_page: 46
    - "no": 4
      title: Transformation de Gelfand
      page: 36
      pdf_page: 49
    - "no": 5
      title: Morphismes d’algèbres de Banach commutatives
      page: 40
      pdf_page: 53
    - "no": 6
      title: Spectre simultané
      page: 41
      pdf_page: 54
    - "no": 7
      title: Ensembles polynomialement convexes
      page: 44
      pdf_page: 57
statements: 48
exercises: 29
content_sha256: 615296abef00f2e6b337fb694f15c5661ca2601e474f667a4b4ae3d46ccedf0f
translated_from: content/en-mt/ts/I/03_s3_algebres_de_banach_commutatives.md
source_lang: en-mt
translation_method: machine
source_content_sha256: b9d684863d94c428b172784825e0ca71705997ae103ae44665bb23553a6e15e6
translation_model: gpt-5.4
translation_run: translate-vi-abae4149
glossary_version: 34
glossary_terms_sha256: eafed7c2afe8beadddef337ca82fa6bdd1f8d142965c3094ea3a445d317a1dfe
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ĐẠI SỐ BANACH GIAO HOÁN

Trong tiết này, trường cơ sở là $\mathbf{C}$.

### 1. Các đặc trưng của một đại số Banach giao hoán

#### Định lý 1 {#ts-i-s3-thm-1 .statement tag=027P}

Cho A là một đại số Banach và cho $\chi : A\rightarrow \mathbf{C}$ là một cấu xạ đại số (xem I, p. 9). Khi đó $\chi$ liên tục, có chuẩn không vượt quá 1. Nếu A có đơn vị và nếu $\chi$ là một cấu xạ có đơn vị, thì $\chi$ có chuẩn bằng 1.

Ta hãy chứng minh rằng $|\chi (x)|\leqslant \|x\|$ với mọi $x\in$ A. Nếu cần, thay thế A bằng đại số Banach sinh bởi $x$, ta có thể giả sử rằng A là giao hoán; khi đó, $\chi \in \mathsf{X}'(A)$. Với mọi $x\in A$, ta có $\chi (x)\in$ Sp$'_A(x)$ (I, p. 9, Số $^o7$), do đó $|\chi (x)|\leqslant \varrho (x)\leqslant \|x\|($I, p. 28, hệ quả 5), suy ra mệnh đề thứ nhất.

Hơn nữa, nếu A có đơn vị, đẳng thức $\chi (1) = 1$ suy ra rằng $\|\chi \|\geqslant 1$, do đó có được đẳng thức cần chứng minh.

#### Nhận xét {#ts-i-s3-n1-rem-1 .statement tag=027Q}

Cho A là một đại số Banach giao hoán. Từ định lý này suy ra rằng tôpô hội tụ đơn giản trên $\mathsf{X}'(A)$ trùng với hạn chế lên $\mathsf{X}'(A)$ của tôpô yếu $\sigma (A',A)$ của đối ngẫu $A'$ của A.

#### Hệ quả {#ts-i-s3-n1-cor-1 .statement tag=027R}

Cho A là một đại số Banach giao hoán. Không gian $\mathsf{X}'(A)$ là compact. Không gian $\mathsf{X}(A)$ là compact địa phương, và là compact nếu A có một phần tử đơn vị.

Cho $A'$ là đối ngẫu của không gian Banach A. Quả cầu đơn vị $A'_1$ của nó là compact yếu (EVT, III, p. 17, hệ quả 2). Theo Định lý 1, ta có $\mathsf{X}'(A)\subset A'_1$. Hơn nữa, $\mathsf{X}'(A)$ là đóng trong $A'$ đối với tôpô yếu, vì nó là giao của các tập đóng yếu

$X_{x,y}=\{f\in A'|f(xy)-f(x)f(y) = 0\}$ (với $x,y\in A$).

Suy ra $\mathsf{X}'(A)$ là compact và $\mathsf{X}(A) =\mathsf{X}'(A)-\{0\}$ là compact địa phương.

Nếu A có một phần tử đơn vị 1, thì $\mathsf{X}(A)$ là tập hợp các $\chi \in$ $\mathsf{X}'(A)$ sao cho $\chi (1) = 1$, và do đó là một tập con đóng, nên compact, của $\mathsf{X}'(A)$.

Mọi không gian compact đều đồng phôi với $\mathsf{X}(A)$ đối với một đại số Banach giao hoán có đơn vị A thích hợp (xem I, p. 32, hệ quả 2).

#### Định lý 2 {#ts-i-s3-thm-2 .statement tag=027S}

Cho A là một đại số Banach giao hoán. Ánh xạ $\chi \mapsto$ Ker($\chi$ ) là một song ánh từ $\mathsf{X}(A)$ lên tập J(A) các iđêan cực đại chính quy của A.

Cho I là một iđêan cực đại chính quy của A. Nó đóng (I, p. 22, hệ quả 2), do đó $A/I$ là một đại số Banach. Vì nó là một trường (A, VIII, p. 426, mệnh đề 2), định lý Gelfand-Mazur (I, p. 26, hệ quả 2) suy ra rằng $A/I$ có chiều bằng 1 trên $\mathbf{C}$. Vậy I có đồng chiều 1 trong A. Khi đó định lý suy ra từ Bổ đề 3 ở I, p. 10.

Có thể xảy ra rằng một đại số Banach giao hoán khác không A, không có phần tử đơn vị, lại không có iđêan cực đại nào; khi đó $\mathsf{X}'(A)$ thu về $\{0\}($xem I, p. 186, bài tập 31).

Định lý này cho thấy rằng các tập J(A) và $\widehat{A}$ của I, p. 11, vốn được đồng nhất vì A là giao hoán, cũng có thể được đồng nhất với tập $\mathsf{X}(A)$. Do đó có lý do để xét trên $\mathsf{X}(A)$ tôpô yếu, và tôpô Jacobson là tôpô kém mịn hơn (I, p. 15, mệnh đề 5). Các tập đóng V(M) của tôpô Jacobson, với $M\subset A$, là các tập

$$
\{\chi \in \mathsf{X}(A)|\chi (M) = 0\}
$$

của $\mathsf{X}(A)$, mà đôi khi ta vẫn sẽ ký hiệu là V(M). Tương tự, với mọi tập con M của $\mathsf{X}(A)$, ta sẽ ký hiệu bởi Υ(M) giao iđêan của các hạt nhân của các $\chi \in M$; nó bằng tập $\Upsilon (M')$ được định nghĩa ở I, p. 13 cho tập con $M'\subset J(A)$ tương ứng với M khi J(A) và $\mathsf{X}(A)$ được đồng nhất.

Khi một khái niệm tôpô được dùng trong $\mathsf{X}(A)$ mà không chỉ rõ là tôpô nào, thì đó luôn luôn là tôpô yếu.

### 2. Các hàm liên tục triệt tiêu ở vô cực trên một không gian compact địa phương

Trong số này, X là một không gian compact địa phương. Ký hiệu bởi $\mathscr{C}_0(X)$ đại số Banach giao hoán các hàm liên tục nhận giá trị phức trên X và tiến tới 0 ở vô cực, được trang bị chuẩn $\|f\|=$ sup$_{x\in X}|f(x)|$

(Ví dụ 3 của I, p. 17).

#### Mệnh đề 1 {#ts-i-s3-prop-1 .statement tag=027T}

Với mọi tập con đóng Φ của X, ký hiệu $I_{\Phi}$ là tập hợp các $f\in \mathscr{C}_0(X)$ triệt tiêu trên Φ. Khi đó $\Phi \mapsto I_{\Phi}$ là một song ánh từ tập hợp các tập con đóng của X lên tập hợp các iđêan đóng của $\mathscr{C}_0(X)$.

Tập hợp $I_{\Phi}$ là một iđêan đóng của $\mathscr{C}_0(X)$.

Cho $\Phi \not= \Phi '$ là các tập con đóng của X. Hoán đổi Φ và $\Phi '$ nếu cần, ta có thể giả sử rằng tồn tại $x\in \Phi '$ sao cho $x\notin \Phi$, và khi đó tồn tại một hàm $f\in \mathscr{C}_0(X)$ triệt tiêu trên Φ và khác không tại $x$ (TG, IX, p. 43, mệnh đề 1). Ta có $f\in I_{\Phi}$ và $f\notin I_{\Phi'}$, do đó ánh xạ $\Phi \mapsto I_{\Phi}$ là đơn ánh.

Cho I là một iđêan đóng của $\mathscr{C}_0(X)$. Gọi Φ là tập hợp các $x\in X$ sao cho $f(x) = 0$ với mọi $f\in I$; đây là một tập con đóng của X, và ta có $I\subset I_{\Phi}$. Ta sẽ chứng minh rằng $I_{\Phi}\subset I$, điều này sẽ kéo theo $I = I_{\Phi}$ và hoàn tất chứng minh của mệnh đề.

Cho $f\in I_{\Phi}$. Với mọi số thực $\varepsilon  >0$, gọi $C_{\varepsilon}$ là tập hợp các $x\in X$ sao cho $|f(x)|\geqslant \varepsilon$. Vì $f$ tiến tới 0 ở vô cực, tập hợp $C_{\varepsilon}$ là compact. Cho $x\in C_{\varepsilon}$; vì $f(x)\not= 0$ và $f\in I_{\Phi}$, ta có $x\notin \Phi$; theo định nghĩa của Φ, khi đó tồn tại một hàm $\varphi_x\in I$ sao cho $|\varphi_x(x)|>1$, do đó sao cho $|\varphi_x(y)|>1$ với mọi $y$ thuộc một lân cận $V_x$ của $x$. Các tập mở $V_x\cap C_{\varepsilon}$ phủ $C_{\varepsilon}$. Vì tập hợp $C_{\varepsilon}$ là compact, tồn tại một tập con hữu hạn $T_{\varepsilon}\subset X$ sao cho

$$
C_{\varepsilon}\subset \bigcup_{x\in T_{\varepsilon}}V_x
$$

Khi đó phần tử

1

$$
g_{\varepsilon}=\sum\varphi_x\overline{\varphi_x}\geqslant 0
$$

$$
\varepsilon
$$

$x\in T_{\varepsilon}$

của $\mathscr{C}_0(X)$ thuộc I, và ta có $g_{\varepsilon}\geqslant \varepsilon^{-1}$ trên $C_{\varepsilon}$. Hàm

$$
f_{\varepsilon}=\frac{f g_{\varepsilon}}{1 + g_{\varepsilon}}
$$

thuộc I. Với $x \notin C_{\varepsilon}$, ta có

$$
|f(x)-f_{\varepsilon}(x)|\leqslant 2\varepsilon
$$

và với $x\in C_{\varepsilon}$, ta có

$$
|f(x)-f_{\varepsilon}(x)|=\frac{|f(x)|}{1 + g_{\varepsilon}(x)}\leqslant \varepsilon |f(x)|
$$

Vậy $f_{\varepsilon}$ hội tụ đều tới $f$ trên X khi $\varepsilon$ tiến tới 0. Suy ra $f\in \overline{I}$, do đó $f\in I$ vì I đóng.

#### Hệ quả 1 {#ts-i-s3-prop-1-cor-1 .statement tag=027U}

Với mọi $x\in X$, gọi $I_x$ là tập hợp các $f\in \mathscr{C}_0(X)$ triệt tiêu tại $x$. Khi đó $x\mapsto I_x$ là một song ánh từ X lên tập hợp các iđêan đóng cực đại của $\mathscr{C}_0(X)$. Các iđêan này là chính quy.

Điều này suy ra ngay từ Mệnh đề 1.

Gọi $X'$ là compact hóa Alexandroff của X, tức là không gian compact suy ra từ X bằng phép nối thêm một điểm ở vô cực $\omega_X$ (TG, I, p. 67 and 68). Đại số $\mathscr{C}_0(X)$ được đồng nhất với đại số Banach các hàm liên tục nhận giá trị phức trên $X'$ triệt tiêu tại $\omega_X$.

Với mọi $x\in X'$, ký hiệu ev$_x$ là đặc trưng của $\mathscr{C}_0(X)$ được xác định bởi ev$_x(f) =f(x)$ với mọi $f\in \mathscr{C}_0(X)$.

#### Hệ quả 2 {#ts-i-s3-prop-1-cor-2 .statement tag=027V}

Ánh xạ $x\mapsto$ ev$_x$ là một đồng phôi từ $X'$ lên $\mathsf{X}'(\mathscr{C}_0(X))$, và hạn chế của nó lên X là một đồng phôi từ X lên $\mathsf{X}(\mathscr{C}_0(X))$. Hơn nữa, tôpô yếu và tôpô Jacobson trùng nhau trên $\mathsf{X}(\mathscr{C}_0(X))$.

Ánh xạ ev$:x\mapsto$ ev$_x$ từ $X'$ vào $\mathsf{X}'(\mathscr{C}_0(X))$ là đơn ánh. Nó là toàn ánh theo Hệ quả 1 và Định lý 2 của I, p. 30. Nó liên tục, vì với mọi hàm $f\in \mathscr{C}_0(X)$ và mọi tập con mở U của $\mathbf{R}$, ta có

ev$^{-1}(\{\chi \in \mathsf{X}'(\mathscr{C}_0(X))|\chi (f)\in U\}) =\overset{-1}{f}(U)$

là mở trong X. Vậy ánh xạ ev là một đồng phôi vì $X'$ là compact. Khi đó hạn chế của ev lên X là một đồng phôi lên $\mathsf{X}(\mathscr{C}_0(X))$.

Nếu F là một tập con đóng yếu của $\mathsf{X}(\mathscr{C}_0(X))$, thì dưới đồng phôi ev nó tương ứng với một tập con đóng Φ của X; chính xác, theo Mệnh đề 1, ta có $F =\{\chi \in \mathsf{X}(\mathscr{C}_0(X))|I_{\Phi}\subset$ Ker $\chi \}$, tập này đóng đối với tôpô Jacobson.

#### Hệ quả 3 {#ts-i-s3-prop-1-cor-3 .statement tag=027W}

Giả sử X compact. Khi đó ánh xạ $x\mapsto$ ev$_x$ là một đồng phôi từ X lên $\mathsf{X}(\mathscr{C}(X))$. Tôpô yếu và tôpô Jacobson trùng nhau trên $\mathsf{X}(\mathscr{C}(X))$.

### 3. Ánh xạ bộ phận thực sự

Trong số này, X và Y là các không gian tôpô địa phương compact. Ta ký hiệu $X'$ (resp. $Y'$) là không gian compact thu được từ X (resp. Y) bằng phép nối thêm một điểm ở vô cực $\omega_X$ (resp. $\omega_Y$) (TG, I, p. 67–68). Ta đồng nhất $X'$ và $Y'$ tương ứng với $\mathsf{X}'(\mathscr{C}_0(X))$ và $\mathsf{X}'(\mathscr{C}_0(Y))$ (Hệ quả 2 của I, p. 32).

#### Định nghĩa 1 {#ts-i-s3-def-1 .statement tag=027X}

Một ánh xạ bộ phận thực sự từ X vào Y là một sự tương ứng $f= (\Gamma ,X,Y)$ (E, II, p. 10, Def. 2) giữa X và Y sao cho

(i) Đồ thị Γ là phiếm hàm;

(ii) Miền xác định của $f$ là một tập con mở U của X;

(iii) Ánh xạ $x\mapsto f(x)$ từ U vào Y là thực sự.

Ánh xạ đồng nhất của X là một ánh xạ bộ phận thực sự từ X vào X. Cho Z là một không gian tôpô địa phương compact và $f$ (resp. $g$) là một ánh xạ bộ phận thực sự từ X vào Y (resp. từ Y vào Z). Khi đó sự tương ứng hợp thành $g\circ f$ (E, II, p. 11, Def. 6) là một ánh xạ bộ phận thực sự từ X vào Z (TG, I, p. 72, Prop. 3, and p. 73, Prop. 5).

#### Bổ đề 1 {#ts-i-s3-lem-1 .statement tag=027Y}

Với mọi ánh xạ bộ phận thực sự $f$ từ X vào Y, có miền xác định là U, gọi $\widetilde{f}$ là ánh xạ từ $X'$ vào $Y'$ được xác định bởi $\widetilde{f}(x) =f(x)$ nếu $x\in U$ và $\widetilde{f}(x) =\omega_Y$ nếu $x \notin U$; nó liên tục.

Ánh xạ $f\mapsto \widetilde{f}$ là một song ánh giữa tập hợp các ánh xạ bộ phận thực sự $f$ của X vào Y và tập hợp các ánh xạ liên tục $g$ của $X'$ vào $Y'$ sao cho $g(\omega_X) =\omega_Y$.

Cho $f$ là một ánh xạ bộ phận thực sự của X vào Y, và cho U là miền xác định của nó. Ta sẽ chứng minh rằng ánh xạ $\widetilde{f}$ là liên tục. Nó liên tục tại mọi điểm của U, vì U là mở trong $X'$. Ta sẽ chứng minh rằng nó cũng liên tục tại mọi điểm $x$ của $X'-$ U; khi đó $\widetilde{f}(x) =\omega_Y$. Cho V là một lân cận mở của $\omega_Y$ trong $Y'$; ta sẽ chứng minh rằng $\widetilde{f}^{-1}(V)$ là một lân cận của $x$. Theo định nghĩa của không gian tôpô $Y'$, ta có thể giả sử rằng V có dạng $Y'-$ K, trong đó K là một tập con compắc của Y. Vì $f$ xác định một ánh xạ thực sự của U vào Y, tập hợp $f^{-1}(K)$ là compắc trong U (TG, I, p. 77, prop. 6), do đó compắc trong $X'$. Đặc biệt, nó là một tập con đóng của $X'$, và $\widetilde{f}^{-1}(V) =$ $X'-f^{-1}(K)$ là một tập con mở của $X'$, và vì thế là một lân cận của $x$.

Ngược lại, cho $g: X'\rightarrow Y'$ là một ánh xạ liên tục sao cho $g(\omega_X) =\omega_Y$, và cho $\Gamma_g\subset X'\times Y'$ là đồ thị của nó. Tập hợp U = X $-\overset{-1}{g}(\omega_Y)$ là mở trong X. Sự tương ứng $f= (\Gamma_g\cap (U\times Y),X,Y)$ là một ánh xạ bộ phận thực sự của X vào Y (TG, I, p. 77, prop. 7) sao cho $\widetilde{f}=g$, và nó là duy nhất.

Ta sẽ đồng nhất các ánh xạ bộ phận thực sự của X vào Y với các ánh xạ liên tục của $X'$ vào $Y'$ mà ánh xạ $\omega_X$ lên $\omega_Y$. Đặc biệt, các ánh xạ thực sự của X vào Y là các ánh xạ bộ phận thực sự có miền xác định là X; chúng được đồng nhất với các ánh xạ liên tục $f$ của $X'$ vào $Y'$ sao cho that $\overset{-1}{f}(\omega_Y) =\{\omega_X\}$. Nếu X là compắc, thì đó đơn giản là các ánh xạ liên tục của X vào Y.

Cho A là một đại số Banach phức giao hoán. Nhắc lại rằng $\mathsf{X}'(A)$ được đồng nhất với không gian compắc thu được từ $\mathsf{X}(A)$ bằng cách thêm vào một điểm ở vô cực (I, p. 29, hệ quả).

#### Mệnh đề 2 {#ts-i-s3-prop-2 .statement tag=027Z}

Cho A và B là các đại số Banach phức giao hoán. Với mọi cấu xạ đại số $\pi : A\rightarrow B$, ánh xạ $\mathsf{X}'(\pi )$ là một ánh xạ bộ phận thực sự của $\mathsf{X}(B)$ vào $\mathsf{X}(A)$.

Thật vậy, $\mathsf{X}'(\pi )$ là một ánh xạ liên tục của $\mathsf{X}'(B)$ vào $\mathsf{X}'(A)$ (I, p. 10). Điểm ở vô cực của $\mathsf{X}'(B)$ (resp. của $\mathsf{X}'(A)$) là đặc trưng không, và ta có $\mathsf{X}'(\pi )(0) = 0$.

#### Mệnh đề 3 {#ts-i-s3-prop-3 .statement tag=0280}

a) Với mọi ánh xạ bộ phận thực sự $\varphi$ của X vào Y, ánh xạ $f\mapsto f\circ \varphi$ từ $\mathscr{C}(Y')$ vào $\mathscr{C}(X')$ cảm sinh một cấu xạ đại số $\varphi^*$ của $\mathscr{C}_0(Y)$ vào $\mathscr{C}_0(X)$ ;

b) Ánh xạ $\varphi \mapsto \varphi^*$ là một song ánh từ tập các ánh xạ bộ phận thực sự của X vào Y lên tập các cấu xạ đại số của $\mathscr{C}_0(Y)$ vào $\mathscr{C}_0(X)$. Song ánh ngược của nó là ánh xạ $\pi \mapsto \mathsf{X}'(\pi )$.

Ta hãy chứng minh a). Cho $\varphi$ là một ánh xạ bộ phận thực sự của X vào Y, được đồng nhất với một ánh xạ liên tục của $X'$ vào $Y'$ sao cho $\varphi (\omega_X) =\omega_Y$. Với $f\in \mathscr{C}_0(Y)$, ta có $(f\circ \varphi )(\omega_X) =f(\omega_Y) = 0$, do đó ánh xạ $\varphi^*$ được xác định tốt. Đó là một cấu xạ đại số.

Ta hãy chứng minh rằng $\mathsf{X}'(\varphi^*)$ đồng nhất với $\varphi$. Cho $x\in X$. Với mọi hàm $f\in \mathscr{C}_0(Y)$, đặc trưng $\mathsf{X}'(\varphi^*$)(ev$_x$) gán cho $f$ số phức

(ev$_x\circ \varphi^*$)$(f) =$ ev$_x(f\circ \varphi ) =f(\varphi (x))$,

do đó $\mathsf{X}'(\varphi^*$)(ev$_x$) $=$ ev$_{\varphi(x)}$. Điều này chứng minh mệnh đề.

Ngược lại, cho $\pi :\mathscr{C}_0(Y)\rightarrow \mathscr{C}_0(X)$ là một cấu xạ đại số. Ta hãy chứng minh rằng $\mathsf{X}'(\pi )^*=\pi$. Cho $f\in \mathscr{C}_0(Y)$, và viết $g=\mathsf{X}'(\pi )^*(f)\in$ $\mathscr{C}_0(X)$. Với mọi $x\in X$, ta có

$g(x) = (f\circ \mathsf{X}'(\pi ))(x) =$ ev$_{\mathsf{X}'(\pi)(x)}(f) =$ (ev$_x\circ \pi$ )$(f) =\pi (f)(x)$,

vì $\mathsf{X}'(\pi )$ thỏa mãn ev$_{\mathsf{X}'(\pi)(x)}=$ ev$_x\circ \pi$. Vậy $g=\pi (f)$, điều này cho phép ta kết luận rằng $\mathsf{X}'(\pi )^*=\pi$.

Hoàn toàn tương tự, ta có:

#### Mệnh đề 4 {#ts-i-s3-prop-4 .statement tag=0281}

Giả sử X và Y compact. Hãy đồng nhất không gian X (resp. không gian Y) với $\mathsf{X}(\mathscr{C}(X))$ (resp. $\mathsf{X}(\mathscr{C}(Y))$) (hệ quả 3 của I, p. 33).

a) Với mọi ánh xạ liên tục $\varphi : X\rightarrow$ Y, ánh xạ $\varphi^*:f\mapsto f\circ \varphi$ là một cấu xạ đại số của $\mathscr{C}(Y)$ vào $\mathscr{C}(X)$;

b) Các ánh xạ $\varphi \mapsto \varphi^*$ và $\pi \mapsto \mathsf{X}(\pi )$ là các song ánh ngược giữa tập các ánh xạ liên tục của X vào Y và tập các cấu xạ đại số của $\mathscr{C}(Y)$ vào $\mathscr{C}(X)$.

#### Nhận xét {#ts-i-s3-n3-rem-1 .statement tag=0282}

*Trong ngôn ngữ của lý thuyết phạm trù, các kết quả trên có thể được giải thích theo cách sau. Cho $\mathbf{G}$ là phạm trù mà các đối tượng là các không gian tôpô compact địa phương và các cấu xạ là các ánh xạ bộ phận thực sự. Hàm tử X $\mapsto \mathscr{C}_0(X)$ là một hàm tử phản biến, trung thành đầy đủ từ phạm trù $\mathbf{G}$ vào phạm trù các đại số Banach phức giao hoán. Hơn nữa, $A\mapsto \mathsf{X}(A)$ là một hàm tử phản biến từ phạm trù các đại số Banach phức giao hoán vào phạm trù $\mathbf{G}$. Nếu với một không gian tôpô compact địa phương X, ta gắn phép đồng phôi

ev$: X\rightarrow \mathsf{X}(\mathscr{C}_0(X))$,

thì ta thu được một đẳng cấu từ hàm tử đồng nhất của phạm trù $\mathbf{G}$ lên hàm tử hợp thành $X\mapsto \mathsf{X}(\mathscr{C}_0(X))$.

Không đúng là hàm tử hợp thành $A\mapsto \mathscr{C}_0(\mathsf{X}(A))$ đẳng cấu với hàm tử đồng nhất của phạm trù các đại số Banach phức giao hoán (xem ví dụ 2 của I, p. 36 và bài tập 2 của I, p. 155). Tuy nhiên, người ta sẽ thấy một mệnh đề thuộc kiểu này đối với các đại số sao giao hoán (No. 5 of I, p. 107).*

### 4. Biến đổi Gelfand

Cho A là một đại số Banach giao hoán. Nhớ lại rằng, với mọi $x\in A$, $\mathscr{G}_A(x)$, hay $\mathscr{G}(x)$, ký hiệu hàm $\chi \mapsto \chi (x)$ trên $\mathsf{X}(A)$, rằng $\mathscr{G}(x)$ được gọi là biến đổi Gelfand của $x$, và rằng ánh xạ $x\mapsto \mathscr{G}(x)$ được gọi là biến đổi Gelfand (x. định nghĩa 5 của I, p. 7). Do đó theo định nghĩa ta có:

$$
\mathscr{G}(x)(\chi ) =\chi (x)
$$

#### Ví dụ 1 {#ts-i-s3-n4-exa-1 .statement tag=0283}

Cho X là một không gian tôpô compact địa phương và xét đại số Banach giao hoán $\mathscr{C}_0(X)$ (ví dụ 3 của I, p. 17 và No. 2 của I, p. 31). Theo Hệ quả 1 của I, p. 32, không gian các đặc trưng $\mathsf{X}(\mathscr{C}_0(X))$ được đồng nhất với X bằng ánh xạ gán cho một phần tử $x\in X$ đặc trưng $f\mapsto f(x)$ của $\mathscr{C}_0(X)$, và khi đó biến đổi Gelfand của $\mathscr{C}_0(X)$ được đồng nhất với ánh xạ đồng nhất.

#### Ví dụ 2 {#ts-i-s3-n4-exa-2 .statement tag=0284}

Cho $n\geqslant 0$ là một số nguyên. Gọi $A_n$ là đại số các hàm $f: [0,1]\rightarrow K$ có các đạo hàm liên tục trên $[0,1]$ đến cấp $n$. Được trang bị chuẩn

$\|f\|=\sum^nk1$! sup$_{0\leqslant t\leqslant 1}|f^{(k)}(t)|$,

$k=0$

nó là một đại số Banach (ví dụ 4 của I, p. 18). Với mọi $n$, không gian các đặc trưng $\mathsf{X}(A_n)$ được đồng nhất với $[0,1]$ và $\mathscr{G}$ được đồng nhất với phép bao hàm của $A_n$ vào $\mathscr{C}([0,1])$ (x. ví dụ 1 của I, p. 144).

#### Ví dụ 3 {#ts-i-s3-n4-exa-3 .statement tag=0285}

Cho Δ là đĩa các số phức $z$ thỏa mãn $|z|\leqslant 1$ và cho A là đại số Banach phức các hàm liên tục trên Δ, giải tích trong phần trong của Δ, được trang bị chuẩn $\|f\|=$ sup$_{z\in\Delta}|f(z)|$ (ví dụ 9 của I, p. 20). Khi đó $\mathsf{X}(A)$ được đồng nhất với Δ và $\mathscr{G}$ được đồng nhất với phép bao hàm của A vào $\mathscr{C}(\Delta )$ (x. Bài tập 6 của I, p. 193).

#### Ví dụ 4 {#ts-i-s3-n4-exa-4 .statement tag=0286}

Xét đại số Banach phức A của các chuỗi Fourier hội tụ tuyệt đối (ví dụ 8 của I, p. 19). Với mọi phần tử $u$ của đường tròn đơn vị $\mathbf{U}$, ánh xạ $f\mapsto f(u)$ là một đặc trưng ev$_u$ của A. Nếu $f_0\in A$ là ánh xạ đồng nhất của $\mathbf{U}$, ta có ev$_u(f_0) =u$, do đó ánh xạ ev$:u\mapsto$ ev$_u$ từ $\mathbf{U}$ vào $\mathsf{X}(A)$ là đơn ánh; nó liên tục.

Cho $\chi \in \mathsf{X}(A)$. Ta có $\|f_0\|$ = $\|f_0^{-1}\|$ = 1, do đó $|\chi (f_0)|\leqslant$ 1 và $|\chi (f_0)^{-1}|\leqslant 1$. Điều này cho thấy $\chi (f_0)\in \mathbf{U}$ và tồn tại $u\in \mathbf{U}$ sao cho $\chi (f_0) =$ ev$_u(f_0)$. Vì $\{f_0, f_0^{-1}\}$ sinh ra đại số có đơn vị A về mặt tôpô, nên ta có $\chi =$ ev$_u$. Vậy ánh xạ ev là một đồng phôi từ $\mathbf{U}$ lên $\mathsf{X}(A)$, nhờ đó các không gian này được đồng nhất. Khi đó biến đổi Gelfand của A được đồng nhất với phép bao hàm của A vào $\mathscr{C}(\mathbf{U})$.

Vì A đẳng cấu với đại số Banach $L^1(\mathbf{Z})$ (ví dụ 8 của I, p. 19), không gian $\mathsf{X}(L^1(\mathbf{Z}))$ được đồng nhất với $\mathbf{U}$ và, với mọi phần tử $(c_n)\in L^1(\mathbf{Z})$, biến đổi Gelfand $\mathscr{G}_{L^1(\mathbf{Z})}((c_n))$ được đồng nhất với hàm $u\mapsto \sum_{n\in\mathbf{Z}}c_nu^n$ trên $\mathbf{U}$.

#### Ví dụ 5 {#ts-i-s3-n4-exa-5 .statement tag=0287}

Cho Δ là đĩa đơn vị gồm các số phức $z$ sao cho $|z|\leqslant 1$. Biên của nó trong $\mathbf{C}$ là $\mathbf{U}$. Cho A là đại số Banach các hàm phức $f$ trên $\mathbf{U}$ sao cho tồn tại một hàm liên tục $\widetilde{f}\in \mathscr{C}(\Delta )$ mở rộng $f$ và giải tích trong $\mathring{\Delta}$, được trang bị chuẩn $\|f\|=$ sup$_{z\in\mathbf{U}}|f(z)|$. Theo nguyên lý cực đại (VAR, R1, p. 30, 3.3.7), khi đó ta có $\|f\|=$ sup$_{z\in\Delta}|\widetilde{f}(z)|$, và do đó A trùng với đại số trong ví dụ 9 của I, p. 20. Tập hợp $\mathsf{X}(A)$ được đồng nhất với Δ và, nếu $f\in A$, ánh xạ $\mathscr{G}(f)$ được đồng nhất với mở rộng liên tục của $f$ lên Δ, giải tích trong $\mathring{\Delta}($xem exerc. 6 của I, p. 193).

#### Mệnh đề 5 {#ts-i-s3-prop-5 .statement tag=0288}

Cho A là một đại số Banach giao hoán. Với mọi $x\in A$, hàm $\mathscr{G}(x)$ thuộc đại số Banach giao hoán $\mathscr{C}_0(\mathsf{X}(A))$ gồm các hàm liên tục trên $\mathsf{X}(A)$ tiến tới 0 ở vô cực.

Theo định nghĩa (xem n$^o7$ của I, p. 9), hàm $\mathscr{G}'_A(x) :\chi \mapsto \chi (x)$ liên tục trên $\mathsf{X}'(A)$ và bằng không tại 0. Vì $\mathsf{X}'(A)$ được đồng nhất với compact hóa Alexandroff của $\mathsf{X}(A)$ theo hệ quả 1 của I, p. 29, mệnh đề được suy ra.

#### Mệnh đề 6 {#ts-i-s3-prop-6 .statement tag=0289}

Cho A là một đại số Banach giao hoán và cho $x\in A$.

a) Hợp của tập hợp các giá trị của $\mathscr{G}(x)$ và của $\{0\}$ bằng Sp$'_A(x)$ ;

b) Nếu A có phần tử đơn vị, tập hợp các giá trị của $\mathscr{G}(x)$ là Sp$_A(x)$. Đặc biệt, để $x$ khả nghịch, điều kiện cần và đủ là $\mathscr{G}(x)$ không triệt tiêu.

Giả sử rằng A có một phần tử đơn vị. Ta biết rằng, với mọi $\chi \in \mathsf{X}(A)$, ta có $\chi (x)\in$ Sp$_A(x)$. Ngược lại, lấy $\lambda \in$ Sp$_A(x)$. Khi đó $x-\lambda$ không khả nghịch, nên thuộc một iđêan cực đại của A. Khi đó tồn tại $\chi \in \mathsf{X}(A)$ sao cho $\chi (x-\lambda ) = 0$ (Định lý 2 của I, p. 30), do đó b).

Bây giờ ta xét trường hợp tổng quát. Gọi $\widetilde{A}$ là đại số Banach nhận được từ A bằng cách thêm vào một phần tử đơn vị; nó là giao hoán. Tập hợp Sp$'_A(x)$ bằng Sp$_{\widetilde{A}}(x)$, nghĩa là bằng tập hợp các giá trị của $\mathscr{G}_{\widetilde{A}}(x)$ trên $\mathsf{X}(\widetilde{A}) =\mathsf{X}'(A)$. Do đó a).

#### Ví dụ {#ts-i-s3-n4-exa-6 .statement tag=028A}

Xét đại số Banach A của các chuỗi Fourier hội tụ tuyệt đối (Ví dụ 4). Mệnh đề 6, b), cho thấy rằng nếu $\varphi$ là một hàm trên đường tròn đơn vị $\mathbf{U}$ có một chuỗi Fourier hội tụ tuyệt đối, và nếu $\varphi$ không triệt tiêu, thì hàm $1/\varphi$ cũng có một chuỗi Fourier hội tụ tuyệt đối ("định lý Wiener").

#### Mệnh đề 7 {#ts-i-s3-prop-7 .statement tag=028B}

Cho A là một đại số Banach giao hoán.

a) Biến đổi Gelfand $\mathscr{G}$ xác định một cấu xạ từ A vào $\mathscr{C}_0(\mathsf{X}(A))$ sao cho $\|\mathscr{G}(x)\|=\varrho (x)\leqslant \|x\|$ với mọi $x\in A$;

b) Để biến đổi Gelfand $\mathscr{G}$ là đẳng cự, điều kiện cần và đủ là $\|x^2\|=\|x\|^2$ với mọi $x\in A$.

Ánh xạ $\mathscr{G}$ là một cấu xạ từ A vào $\mathscr{C}_0(\mathsf{X}(A))$ theo No. $^o7$ của I, p. 9 và Mệnh đề 5 của I, p. 37, và thỏa mãn $\|\mathscr{G}(x)\|=\varrho (x)$ theo Mệnh đề 6 và Hệ quả 5 của I, p. 28. Mệnh đề b) suy ra từ a) và Nhận xét 1 của I, p. 21.

#### Hệ quả {#ts-i-s3-n4-cor-1 .statement tag=028C}

Cho A là một đại số Banach, và gọi $x$ và $y$ là các phần tử giao hoán với nhau của A.

a) Ta có $\varrho (xy)\leqslant \varrho (x)\varrho (y)$ và $\varrho (x+y)\leqslant \varrho (x) +\varrho (y)$;

b) Nếu $y$ là giả lũy linh, thì Sp$'_A(x) =$ Sp$'_A(x+y)$; hơn nữa nếu A có đơn vị, thì Sp$_A(x) =$ Sp$_A(x+y)$.

Bằng cách xét đại số Banach suy ra từ A bằng cách thêm vào một phần tử đơn vị, trước hết ta quy về trường hợp đại số A là có đơn vị. Sau đó, bằng cách xét đại số con đầy đủ đóng của A sinh bởi $x$ và $y$, ta quy về trường hợp A là giao hoán và có đơn vị. Mệnh đề a) khi đó là một hệ quả của Mệnh đề 7, a), và mệnh đề b) suy ra từ Mệnh đề 6 của I, p. 37 và Hệ quả 5 của I, p. 28.

#### Mệnh đề 8 {#ts-i-s3-prop-8 .statement tag=028D}

Cho A là một đại số Banach giao hoán. Bốn tập hợp sau đây bằng nhau:

(i) Hạt nhân của biến đổi Gelfand;

(ii) Tập hợp các phần tử $x$ của A sao cho Sp$'_A(x) =\{0\}$;

(iii) Tập hợp các phần tử giả lũy linh của A;

(iv) Căn của A.

Ký hiệu các tập hợp này lần lượt là $N_1,N_2,N_3,N_4$. Ta có $N_1=$ $N_2$ (Mệnh đề 6, a)), và $N_2= N_3($I, p. 28, Hệ quả 5). Theo định nghĩa, tập hợp $N_4$ là giao của các iđêan cực đại chính quy của A; do đó nó là giao của các hạt nhân của các đặc trưng của A (Định lý 2 của I, p. 30), giao này bằng $N_1$.

#### Nhận xét 1 {#ts-i-s3-n4-rem-1 .statement tag=028E}

Nói chung, ảnh của biến đổi Gelfand không đóng trong $\mathscr{C}_0(\mathsf{X}(A))$, cũng không trù mật trong $\mathscr{C}_0(\mathsf{X}(A))$ (Bài tập 7 của I, p. 193).

#### Nhận xét 2 {#ts-i-s3-n4-rem-2 .statement tag=028F}

Ảnh của biến đổi Gelfand tách các điểm của $\mathsf{X}(A)$, vì nếu $\chi_1\not=\chi_2$ là các phần tử của $\mathsf{X}(A)$, thì tồn tại $x\in A$ sao cho $\chi_1(x)\not=\chi_2(x)$.

#### Nhận xét 3 {#ts-i-s3-n4-rem-3 .statement tag=028G}

Nếu $\chi \in \mathsf{X}(A)$, thì tồn tại một phần tử của ảnh của biến đổi Gelfand không triệt tiêu tại $\chi$.

#### Nhận xét 4 {#ts-i-s3-n4-rem-4 .statement tag=028H}

Nếu A có một phần tử đơn vị, thì ảnh của biến đổi Gelfand là một đại số con đầy đủ của đại số các hàm liên tục trên $\mathsf{X}(A)$ (Mệnh đề 6, b)).

#### Bổ đề 2 {#ts-i-s3-lem-2 .statement tag=028I}

Cho A là một đại số Banach giao hoán. Cho M là một tập con của $\mathsf{X}(A)$. Khi đó M đóng đối với tôpô Jacobson nếu và chỉ nếu, với mọi đặc trưng $\chi \in \mathsf{X}(A)$ - M, tồn tại một phần tử $x$ của A sao cho $\mathscr{G}(x)$ bằng không trên M và khác không tại $\chi$.

Cho Υ(M) là giao của các hạt nhân của các phần tử của M. Tập hợp M đóng đối với tôpô Jacobson nếu và chỉ nếu M = V(Υ(M)) (x. I, p. 13 và I, p. 30). Điều kiện này tương đương với việc nói rằng các phần tử $\chi$ của M chính xác là các đặc trưng triệt tiêu trên Υ(M). Do đó M đóng nếu và chỉ nếu với mọi đặc trưng $\chi  \notin M$, tồn tại $x\in \Upsilon (M)$ sao cho $\chi (x)\not= 0$. Điều này chuyển thành $\mathscr{G}(x)(\chi )\not= 0$ và $\mathscr{G}(x)|M = 0$.

### 5. Các cấu xạ của các đại số Banach giao hoán

#### Mệnh đề 9 {#ts-i-s3-prop-9 .statement tag=028J}

Cho A là một đại số Banach, cho B là một đại số Banach giao hoán không có căn, mọi cấu xạ của đại số nền của A vào đại số nền của B đều liên tục.

Cho $h: A\rightarrow B$ là một cấu xạ đại số và cho $(a, b)\in A\times B$ là một điểm dính của đồ thị Γ của $h$. Cho $\chi \in \mathsf{X}'(B)$. Hàm $x\mapsto \chi (h(x))$ từ A vào $\mathbf{C}$ là một đồng cấu đại số, do đó là liên tục (I, p. 29, đ. lý 1). Vì thế ánh xạ từ $A\times B$ vào $\mathbf{C}$ cho bởi $(x, y)\mapsto \chi (h(x))-\chi (y)$ là liên tục; nó bằng không trên Γ, nên bằng không tại $(a, b)$. Vậy ta có $\chi (h(a)) =\chi (b)$ với mọi $\chi \in \mathsf{X}'(B)$. Vì B không có căn, ta có $h(a) =b$. Do đó đồ thị của $h$ là đóng và vì thế $h$ là liên tục (EVT, I, p. 19, hệ quả 5).

#### Hệ quả {#ts-i-s3-n5-cor-1 .statement tag=028K}

Trên một đại số phức giao hoán không có căn, hai chuẩn xác định các cấu trúc đại số Banach là tương đương.

Chỉ cần áp dụng mệnh đề 9 cho ánh xạ đồng nhất của đại số.

Cho A và B là các đại số Banach giao hoán. Theo No.$^o7$ của I, p. 9, nếu $h: A\rightarrow B$ là một cấu xạ toàn ánh, $\mathsf{X}'(h)$ là một đồng phôi của $\mathsf{X}'(B)$ lên một không gian con đóng của $\mathsf{X}'(A)$ biến 0 thành 0. (Trong trường hợp $h$ là đơn ánh của một đại số con vào $\mathscr{C}(X)$, ánh xạ $\mathsf{X}'(h)$ là đơn ánh dưới những giả thiết yếu hơn nhiều, x. I, p. 142, mệnh đề 1, d).)

Bây giờ cho $h: A\rightarrow B$ là một cấu xạ đơn ánh. Nói chung, $\mathsf{X}'(h)$ không toàn ánh, nhưng mệnh đề sau cho một điều kiện cần để điều này xảy ra.

#### Mệnh đề 10 {#ts-i-s3-prop-10 .statement tag=028L}

Cho A và B là các đại số Banach giao hoán có đơn vị, $h: A\rightarrow B$ là một cấu xạ đại số có đơn vị, không nhất thiết liên tục. Nếu $\mathsf{X}(h)$ là toàn ánh, thì $h(A)$ là một đại số con đầy của B.

Cho $x\in A$ sao cho $h(x)$ khả nghịch trong B. Với mọi $\chi \in \mathsf{X}(A)$, tồn tại $\xi \in \mathsf{X}(B)$ sao cho $\chi =\mathsf{X}(h)(\xi )$, do đó $\chi (x) =\xi (h(x))\not= 0$. Mệnh đề 6 của I, p. 37 khi đó cho thấy rằng $x$ khả nghịch trong A, và do đó $h(x)$ khả nghịch trong $h(A)$.

Điều kiện cần của mệnh đề không phải là điều kiện đủ, ngay cả khi $h$ là đẳng cự (I, p. 168, bài tập 14). Tuy vậy vẫn có kết quả sau:

#### Mệnh đề 11 {#ts-i-s3-prop-11 .statement tag=028M}

Cho A và B là các đại số Banach giao hoán có đơn vị, cho $a$ là một phần tử của A và cho $h: A\rightarrow B$ là một cấu xạ có đơn vị đơn ánh (không nhất thiết liên tục). Giả sử rằng đại số con đầy đóng của A sinh bởi $a$ bằng A. Các điều kiện sau là tương đương:

(i) $\mathsf{X}(h)$ là toàn ánh;

(ii) $h(A)$ là một đại số con đầy của B;

(iii) Sp$_A(a) =$ Sp$_B(h(a))$.

(i) $=\Rightarrow$ (ii) suy ra từ mệnh đề 10.

(ii) $=\Rightarrow$ (iii) suy ra từ công thức Sp$_A(a) =$ Sp$_{h(A)}(h(a)) =$ Sp$_B(h(a))$, đúng vì $h(A)$ là một đại số con đầy đủ của B.

(iii) $=\Rightarrow$ (i) theo công thức (4) của No.$^o6$ của I, p. 6, ta có biểu đồ giao hoán

$$
\leftarrow^{\mathsf{X}(h)}
$$

$$
\mathsf{X}(B)\rightarrow \mathsf{X}(A)
$$

$$
\rightarrow \leftarrow_{\mathscr{G}_B(h(a))}\rightarrow \leftarrow_{\mathscr{G}_A(a)}
$$

$$
\leftarrow_i
$$

Sp$_B(h(a))\rightarrow$ Sp$_A(a)$

trong đó các mũi tên thẳng đứng biểu thị các ánh xạ toàn ánh (I, p. 37, mệnh đề 6) và $i$ là phép bao hàm chính tắc. Giả thiết (iii) có nghĩa là $i$ là song ánh. Hơn nữa ánh xạ toàn ánh $\mathscr{G}_A(a) :\mathsf{X}(A)\rightarrow$ Sp$_A(a)$ là song ánh: thật vậy, với mọi đặc trưng $\chi_1$ và $\chi_2$ của A, tập hợp $A_{\chi_1,\chi_2}=\{x\in A|\chi_1(x) =\chi_2(x)\}$ là một đại số con đầy đủ đóng của A. Bởi giả thiết, do đó, ta có $A_{\chi_1,\chi_2}$ = A nếu $a\in A_{\chi_1,\chi_2}$, nghĩa là $\chi_1=\chi_2$ nếu $\mathscr{G}_A(a)\chi_1=\mathscr{G}_A(a)\chi_2$. Khi đó biểu đồ suy ra rằng ánh xạ $\mathsf{X}(h)$ là toàn ánh.

### 6. Phổ Đồng Thời

Cho Λ là một tập hợp. Đặt $C_{\Lambda}=\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$ là đại số có đơn vị của các đa thức phức theo một họ các bất định $(X_{\lambda})_{\lambda\in\Lambda}$. Với mọi $\chi \in \mathsf{X}(C_{\Lambda})$, ta có $(\chi (X_{\lambda}))_{\lambda\in\Lambda}\in \mathbf{C}^{\Lambda}$; ánh xạ $\chi \mapsto$ $(\chi (X_{\lambda}))_{\lambda\in\Lambda}$ là một đồng phôi của $\mathsf{X}(C_{\Lambda})$ lên không gian tích $\mathbf{C}^{\Lambda}$, nhờ đó các không gian này được đồng nhất.

Mặt khác, cho A là một đại số Banach giao hoán có đơn vị và $x= (x_{\lambda})_{\lambda\in\Lambda}$ là một họ các phần tử của A. Tồn tại duy nhất một cấu xạ có đơn vị $h$ từ $C_{\Lambda}$ vào A sao cho $h(X_{\lambda}) =x_{\lambda}$ với mọi $\lambda$. Ánh xạ liên tục $\mathsf{X}(h)$ từ $\mathsf{X}(A)$ vào $\mathbf{C}^{\Lambda}$ là ánh xạ gán cho $\chi$ họ $(\chi (x_{\lambda}))_{\lambda\in\Lambda}$. Nó được gọi là ánh xạ từ $\mathsf{X}(A)$ vào $\mathbf{C}^{\Lambda}$ xác định bởi $x$.

#### Định nghĩa 2 {#ts-i-s3-def-2 .statement tag=028N}

Ảnh của ánh xạ $\mathsf{X}(h)$ được gọi là phổ đồng thời của $x$, và được ký hiệu bởi Sp$^{\Lambda}_A(x)$ hoặc Sp$^{\Lambda}(x)$.

Phổ đồng thời của $x$ là một tập con compắc của $\mathbf{C}^{\Lambda}$. Một phần tử $c= (c_{\lambda})\in \mathbf{C}^{\Lambda}$ thuộc Sp$^{\Lambda}_A(x)$ nếu và chỉ nếu các phần tử $x_{\lambda}-c_{\lambda}$ thuộc cùng một iđêan cực đại của A, nói cách khác nếu họ $(x_{\lambda}-c_{\lambda})_{\lambda\in\Lambda}$ không sinh đại số A.

Nếu $\Lambda$ chỉ chứa một phần tử, sao cho họ $x$ quy về một phần tử duy nhất $x\in A$, thì ta có Sp$^{\Lambda}_A(x) =$ Sp$_A(x)$ (I, p. 37, prop. 6, b)). Nếu $\Lambda '\subset \Lambda$, thì Sp$^{\Lambda'}_A((x_{\lambda})_{\lambda\in\Lambda'})$ là ảnh của Sp$^{\Lambda}_A((x_{\lambda})_{\lambda\in\Lambda})$ dưới ánh xạ phép chiếu chính tắc của $\mathbf{C}^{\Lambda}$ lên $\mathbf{C}^{\Lambda'}$. Đặc biệt, ta có

Sp$^{\Lambda}_A(x)\subset \prod_{\lambda\in\Lambda}$ Sp$_A(x_{\lambda})$.

Ký hiệu $z_{\lambda}$, với $\lambda \in \Lambda$, là các hàm tọa độ trên $\mathbf{C}^{\Lambda}$. Nếu $\chi \in$ $\mathsf{X}(A)$, giá trị tại $\chi$ của $z_{\lambda}\circ \mathsf{X}(h)$ là $\chi (x_{\lambda})$, do đó $z_{\lambda}\circ \mathsf{X}(h) =\mathscr{G}(x_{\lambda})$.

Cho A và B là các đại số Banach giao hoán có đơn vị, $\varphi$ là một cấu xạ có đơn vị từ A vào B, và $x= (x_{\lambda})_{\lambda\in\Lambda}$ là một họ các phần tử của A. Ký hiệu $\varphi (x)$ là họ $(\varphi (x_{\lambda}))_{\lambda\in\Lambda}$ các phần tử của B. Ta có, với mọi $\chi \in \mathsf{X}(B)$, và mọi $\lambda \in \Lambda$

$$
\chi (\varphi (x_{\lambda})) = (\mathsf{X}(\varphi )(\chi ))(x_{\lambda})
$$

do đó Sp$^{\Lambda}_B(\varphi (x))\subset$ Sp$^{\Lambda}_A(x)$. Biểu đồ

$$
\leftarrow^{\mathsf{X}(\varphi)}
$$

$$
\mathsf{X}(B)\rightarrow \mathsf{X}(A)
$$

$$
\rightarrow \leftarrow \rightarrow \leftarrow \tag{1}
$$

$$
_{\Lambda}\leftarrow_{i\Lambda}
$$

Sp$_B(\varphi (x))\rightarrow$ Sp$_A(x)$

trong đó $i$ ký hiệu phép bao hàm, và trong đó các mũi tên thẳng đứng ký hiệu các ánh xạ được xác định bởi các họ $\varphi (x)$ và $x$, vì thế là giao hoán.

#### Ví dụ {#ts-i-s3-n6-exa-1 .statement tag=028O}

Cho K $\subset \mathbf{C}^{\Lambda}$ là một tập con compắc. Cho $z= (z_{\lambda})_{\lambda\in\Lambda}$ là họ trong $\mathscr{C}(K)$ gồm các hạn chế lên K của các hàm tọa độ của $\mathbf{C}^{\Lambda}$. Khi đó phổ chung Sp$^{\Lambda}_{\mathscr{C}(K)}(z)$ bằng K. Thật vậy, theo Hệ quả 2 của I, p. 32, mọi đặc trưng $\chi$ của $\mathscr{C}(K)$ đều có dạng $f\mapsto f(x)$ với một phần tử $x\in K$, và khi đó ta có $(\chi (z_{\lambda}))_{\lambda\in\Lambda}=x$.

#### Mệnh đề 12 {#ts-i-s3-prop-12 .statement tag=028P}

Cho Λ là một tập hợp và A là một đại số Banach giao hoán có đơn vị. Cho $x= (x_{\lambda})_{\lambda\in\Lambda}$ là một họ các phần tử của A.

a) Giả sử rằng đại số con đầy đủ của A được sinh bởi họ $x$ là trù mật trong A. Ánh xạ từ $\mathsf{X}(A)$ vào $\mathbf{C}^{\Lambda}$ được xác định bởi $x$ là một đồng phôi từ $\mathsf{X}(A)$ lên phổ chung Sp$^{\Lambda}_A(x)$ ;

b) Giả sử rằng đại số con có đơn vị của A được sinh bởi họ $x$ là trù mật trong A. Với mọi $c\in \mathbf{C}^{\Lambda}$, các điều kiện sau là tương đương :

(i) $c\in$ Sp$^{\Lambda}_A(x)$ ;

(ii) $|P(c)|\leqslant \varrho (P(x))$ với mọi đa thức $P\in \mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$;

(iii) $|P(c)|\leqslant \|P(x)\|$ với mọi đa thức $P\in \mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$.

a) Ánh xạ từ $\mathsf{X}(A)$ vào Sp$^{\Lambda}_A(x)$ được xác định bởi họ $x$ là liên tục và toàn ánh. Cho $\chi ,\chi '\in \mathsf{X}(A)$ là các đặc trưng có cùng ảnh, nghĩa là, sao cho $\chi (x_{\lambda}) =\chi '(x_{\lambda})$ với mọi $\lambda \in \Lambda$. Các đặc trưng $\chi$ và $\chi '$ trùng nhau trên các phần tử dạng $P(x)Q(x)^{-1}$, trong đó $P\in \mathbf{C}[(X_{\lambda})]$, $Q\in \mathbf{C}[(X_{\lambda})]$ và $Q(x)$ là khả nghịch trong A, nghĩa là, trên toàn bộ đại số con của A sinh bởi các phần tử $x_{\lambda}$ (bổ đề 2 của I, p. 6). Vì $\chi$ và $\chi '$ là liên tục (Định lý 1 của I, p. 29), do đó chúng bằng nhau trên A. Điều này chứng minh rằng $\mathsf{X}(h)$ là một song ánh liên tục từ $\mathsf{X}(A)$ lên Sp$^{\Lambda}_A(x)$, và vì thế là một đồng phôi vì $\mathsf{X}(A)$ là compact.

b) Ta hãy chứng minh rằng (i) kéo theo (ii): nếu $c= (c_{\lambda})_{\lambda\in\Lambda}\in$ Sp$^{\Lambda}_A(x)$, thì tồn tại $\chi \in \mathsf{X}(A)$ sao cho $c_{\lambda}=\chi (x_{\lambda})$ với mọi $\lambda$. Với mọi $P\in \mathbf{C}[(X_{\lambda})]$, do đó ta có $|P(c)|=|P((\chi (x_{\lambda}))_{\lambda\in\Lambda})|=|\chi (P(x))|\leqslant \varrho (P(x))$.

Mệnh đề (ii) kéo theo (iii) do bất đẳng thức $\varrho (x)\leqslant \|x\|$, đúng với mọi $x\in A$ theo định nghĩa của bán kính phổ.

Sau cùng ta hãy chứng minh rằng (iii) kéo theo (i). Cho $c= (c_{\lambda})_{\lambda\in\Lambda}\in \mathbf{C}^{\Lambda}$ sao cho

$$
|P(c)|\leqslant \|P(x)\| \tag{2}
$$

với mọi P $\in \mathbf{C}[(X_{\lambda})]$. Gọi $A'$ là đại số con có đơn vị của A sinh bởi họ $x$; các phần tử của nó có dạng $P(x)$ với $P\in \mathbf{C}[(X_{\lambda})]$. Sự major hóa (2) kéo theo rằng điều kiện $P(x) = 0$ dẫn đến $P(c) = 0$. Do đó tồn tại một cấu xạ đại số có đơn vị $\xi$ từ $A'$ vào $\mathbf{C}$ sao cho $\xi (x_{\lambda}) =c_{\lambda}$ với mọi $\lambda \in \Lambda$. Theo (2), cấu xạ $\xi$ là liên tục. Vì vậy nó kéo dài được bằng tính liên tục thành một đặc trưng $\chi$ của $\overline{A'}= A$, thỏa mãn $c= (\chi (x_{\lambda}))_{\lambda\in\Lambda}\in$ Sp$^{\Lambda}_A(x)$. Điều này hoàn tất chứng minh.

### 7. Các tập hợp lồi đa thức

#### Định nghĩa 3 {#ts-i-s3-def-3 .statement tag=028Q}

Cho Λ là một tập hợp và V là một tập con của $\mathbf{C}^{\Lambda}$. Ta nói rằng V là lồi đa thức nếu V là tập hợp các điểm $(c_{\lambda})_{\lambda\in\Lambda}$ của $\mathbf{C}^{\Lambda}$ sao cho

$|P((c_{\lambda}))|\leqslant$ sup$_{c\in V}|P(c)|$

với mọi $P\in \mathbf{C}[(X_{\lambda})]$.

#### Bổ đề 3 {#ts-i-s3-lem-3 .statement tag=028R}

Cho $\Lambda$ là một tập hợp. Một tập con V của $\mathbf{C}^{\Lambda}$ là lồi đa thức nếu và chỉ nếu tồn tại một họ $(P_i)_{i\in I}$ gồm các phần tử của $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$ và một họ $(M_i)_{i\in I}$ gồm các phần tử của $[0,+\infty ]$ sao cho V là tập hợp các $c\in \mathbf{C}^{\Lambda}$ thỏa mãn

$$
|P_i(c)|\leqslant M_i
$$

với mọi $i\in I$.

Nếu tập con V của $\mathbf{C}^{\Lambda}$ là lồi đa thức, thì nó thỏa mãn điều kiện trên đối với họ gồm các phần tử P của $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$ bằng cách đặt $M_P=$ sup$_{c\in V}|P(c)|$.

Ngược lại, cho $(P_i)_{i\in I}$ là một họ các phần tử của $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$ và $(M_i)_{i\in I}$ là một họ các phần tử của $[0,+\infty ]$. Cho V là tập hợp các $c$ trong $\mathbf{C}^{\Lambda}$ sao cho $|P_i(c)|\leqslant M_i$ với mọi $i\in I$. Khi đó sup$_{c\in V}|P_i(c)|\leqslant M_i$ với $i\in I$. Giả sử rằng $x\in \mathbf{C}^{\Lambda}$ thỏa mãn

$|P(x)|\leqslant$ sup$_{c\in V}|P(c)|$

với mọi $P\in \mathbf{C}[(X_{\lambda})]$. Đặc biệt, với $i\in I$, ta có $|P_i(x)|\leqslant M_i$, do đó $x\in V$. Ngược lại, với mọi phần tử $x\in V$ và mọi đa thức $P\in \mathbf{C}[(X_{\lambda})]$, ta có $|P(x)|\leqslant$ sup$_{c\in V}|P(c)|$. Do đó, tập hợp V là lồi đa thức.

#### Bổ đề 4 {#ts-i-s3-lem-4 .statement tag=028S}

Cho A là một đại số Banach giao hoán có đơn vị. Cho $\Lambda$ là một tập hợp và $x= (x_{\lambda})_{\lambda\in\Lambda}$ là một họ các phần tử của A. Nếu đại số con có đơn vị sinh bởi họ $x$ là trù mật trong A, thì phổ đồng thời Sp$^{\Lambda}_A(x)$ là lồi đa thức.

Điều này suy ra từ mệnh đề b) của Mệnh đề 12 của I, p. 43 và Định nghĩa 3.

Mọi giao của các tập con lồi đa thức của $\mathbf{C}^{\Lambda}$ đều là lồi đa thức (Bổ đề 3). Điều này biện minh cho định nghĩa sau:

#### Định nghĩa 4 {#ts-i-s3-def-4 .statement tag=028T}

Cho $\Lambda$ là một tập hợp và V là một tập con của $\mathbf{C}^{\Lambda}$. Bao lồi đa thức của V là tập con lồi đa thức nhỏ nhất của $\mathbf{C}^{\Lambda}$ chứa V.

Bao lồi đa thức của V là tập hợp các $c$ thuộc $\mathbf{C}^{\Lambda}$ sao cho $|P(c)|\leqslant$ sup$_W|P|$ với mọi $P\in \mathbf{C}[(X_{\lambda})]$. Thật vậy, tập hợp này là lồi đa thức theo Bổ đề 3, và theo định nghĩa, nó được chứa trong mọi tập hợp lồi đa thức chứa V.

#### Ví dụ {#ts-i-s3-n7-exa-1 .statement tag=028U}

Cho $\Lambda$ là một tập hợp hữu hạn và $V\subset \mathbf{C}^{\Lambda}$ là một tập con lồi compắc. Khi đó V là lồi đa thức. Thật vậy, gọi W là bao lồi đa thức của V. Ta sẽ chứng minh rằng $W\subset V$, điều này sẽ kéo theo mệnh đề. Lấy $x\in \mathbf{C}^{\Lambda}-$V. Tồn tại một siêu phẳng thực H trong $\mathbf{C}^{\Lambda}$ tách chặt $x$ và V (EVT, II, p. 41, Prop. 4). Gọi $f_{\mathbf{R}}$ là một dạng tuyến tính $\mathbf{R}$ trên $\mathbf{C}^{\Lambda}$ và $\alpha \in \mathbf{R}$ sao cho H là tập hợp các $y\in \mathbf{C}^{\Lambda}$ thỏa mãn $f_{\mathbf{R}}(y) =\alpha$. Gọi $f$ là một dạng tuyến tính trên $\mathbf{C}^{\Lambda}$ sao cho $f_{\mathbf{R}}=\mathscr{R}(f)$. Do đó ta có

$\mathscr{R}(f(x))>$ sup$_{y\in V}\mathscr{R}(f(y))$.

Với mọi $t\in \mathbf{R}$ và mọi $y\in V$, đặt $f_t(y) =t+f(y)$. Ta có $|f_t|-\mathscr{R}(f_t)\rightarrow 0$ trong $\mathscr{C}(\mathbf{C}^{\Lambda},\mathbf{R})$ được trang bị tôpô hội tụ compắc khi $t\rightarrow +\infty$. Với $t$ đủ lớn, suy ra $|f_t(x)|>$ sup$_{y\in V}|f_t(y)|$ vì V là compắc. Do đó $x\in \mathbf{C}^{\Lambda}-$ W vì $f_t$ là một hàm đa thức.

#### Bổ đề 5 {#ts-i-s3-lem-5 .statement tag=028V}

Cho K là một tập con compắc của $\mathbf{C}$. Ta ký hiệu bởi $\widehat{K}$ hợp của K và các thành phần liên thông của $\mathbf{C}-$ K là tương đối compắc. Khi đó tập hợp $\widehat{K}$ là compắc.

Vì K là compắc, tồn tại một số thực $r >0$ sao cho K được chứa trong đĩa mở D tâm 0 bán kính $r$. Khi đó $\mathbf{C}-$ K chứa $\mathbf{C}-$D. Vì không gian $\mathbf{C}-$ D là liên thông (do đồng phôi với $[r,+\infty [\times \mathbf{S}^1)$, nó được chứa trong một thành phần liên thông U của $\mathbf{C}^-$K. Mọi thành phần liên thông khác của $\mathbf{C}^-$ K đều được chứa trong D, nên bị chặn. Vậy thành phần liên thông U là thành phần liên thông không bị chặn duy nhất của $\mathbf{C}^-$ K, tức là, $U =\mathbf{C}-\widehat{K}$. Vì U là mở và chứa phần bù của đĩa D, tập hợp $\widehat{K}$ là compắc.

#### Mệnh đề 13 {#ts-i-s3-prop-13 .statement tag=028W}

Cho $n\geqslant 1$ là một số nguyên. Cho $K\subset \mathbf{C}^n$ là một tập con đóng và V là bao lồi đa thức của nó.

a) Mọi thành phần liên thông bị chặn của $\mathbf{C}^n-$ K đều được chứa trong V;

b) Nếu $n= 1$, và nếu K compắc, thì V là hợp $\widehat{K}$ của K và các thành phần liên thông bị chặn của $\mathbf{C}-$ K.

Vì $K\subset \mathbf{C}^n$ là đóng, phần bù của nó $\mathbf{C}^n-$ K là mở, nên liên thông địa phương, do đó mỗi thành phần liên thông của $\mathbf{C}^n-$ K là mở. Nguyên lý cực đại (VAR, R1, p. 29, 3.3.7) khi đó cho thấy rằng mọi thành phần liên thông bị chặn của $\mathbf{C}^n-$ K đều được chứa trong V, điều này chứng minh mệnh đề a).

Bây giờ giả sử $n= 1$ và K compắc. Hãy ký hiệu bởi $\widehat{K}$ hợp của K với các thành phần liên thông bị chặn của $\mathbf{C}-$ K, sao cho $\widehat{K}\subset$ V theo điều đi trước. Tập hợp $\widehat{K}$ là compắc (Bổ đề 5). Cho A là đại số Banach giao hoán có đơn vị $\mathscr{C}(\widehat{K})$. Cho $x\in A$ là hàm đồng nhất của $\widehat{K}$ và B là đại số con đóng có đơn vị của A sinh bởi $x$. Ta có Sp$_A(x) =\widehat{K}$ (Ví dụ 3 của I, p. 17), do đó $\mathbf{C}-$ Sp$_A(x)$ liên thông. Do đó ta có Sp$_B(x) =$ Sp$_A(x)$ (Hệ quả của Mệnh đề 6 của I, p. 28). Vì Sp$_B(x)$ là lồi đa thức theo Bổ đề 4, điều này cho thấy $\widehat{K}$ là lồi đa thức và bởi vậy $V\subset \widehat{K}$.

Phần thứ hai của mệnh đề không mở rộng được cho trường hợp $n\geqslant 2$ (x. Bài tập 23 của I, p. 170).

#### Mệnh đề 14 {#ts-i-s3-prop-14 .statement tag=028X}

Cho Λ là một tập hợp. Cho A là một đại số Banach giao hoán có đơn vị, $x= (x_{\lambda})_{\lambda\in\Lambda}$ một họ các phần tử của A, và $A'$ là đại số con Banach có đơn vị sinh bởi $x$. Khi đó phổ chung Sp$^{\Lambda}_{A'}(x)$ là bao lồi đa thức của Sp$^{\Lambda}_A(x)$.

Thật vậy, Mệnh đề 12 của I, p. 43, b) chỉ ra rằng Sp$^{\Lambda}_{A'}(x)$ là tập hợp các $c\in \mathbf{C}^{\Lambda}$ sao cho $|P(c)|\leqslant \varrho (P(x))$ với mọi $P\in \mathbf{C}[(X_{\lambda})]$. Bây giờ ta có

$\varrho (P(x)) =$ sup$_{\chi\in\mathsf{X}(A)}|\chi (P(x))|=$ sup$_{\chi\in\mathsf{X}(A)}|P((\chi (x_{\lambda}))_{\lambda\in\Lambda})|=$ sup$_{c\in Sp_{\Lambda A}(x)}|P(c)|$,

theo Mệnh đề 7 của I, p. 38, a) và Mệnh đề 12 của I, p. 43, a). Kết quả khi đó suy ra từ Bổ đề 3.

#### Mệnh đề 15 {#ts-i-s3-prop-15 .statement tag=028Y}

Cho Λ là một tập hợp. Cho K là một tập con compắc lồi đa thức của $\mathbf{C}^{\Lambda}$. Cho $A_0$ là tập hợp các hạn chế lên K của các hàm đa thức trên $\mathbf{C}^{\Lambda}$, và cho A là bao đóng của $A_0$ trong đại số $\mathscr{C}(K)$.

Cho ev$: K\rightarrow \mathsf{X}(A)$ là ánh xạ xác định bởi $x\mapsto$ ev$_x$, trong đó ev$_x$ là đặc trưng $f\mapsto f(x)$ của A. Cho $z= (z_{\lambda})_{\lambda\in\Lambda}$ là họ trong A gồm các hạn chế lên K của các hàm tọa độ trên $\mathbf{C}^{\Lambda}$, và cho $\varphi$ là ánh xạ toàn ánh của $\mathsf{X}(A)$ lên Sp$^{\Lambda}_A(z)$ được xác định bởi họ $z$.

Khi đó ta có K = Sp$^{\Lambda}_A(z)$, và các ánh xạ ev : K $\rightarrow \mathsf{X}(A)$ và $\varphi :\mathsf{X}(A)\rightarrow K$ là các đồng phôi nghịch đảo của nhau.

Ánh xạ $\varphi \circ$ ev là ánh xạ đồng nhất của K. Đặc biệt, K được chứa trong ảnh Sp$^{\Lambda}_A(z)$ của $\varphi$.

Mệnh đề 14 kéo theo rằng Sp$^{\Lambda}_A(z)$ là bao lồi đa thức của Sp$^{\Lambda}_{\mathscr{C}(K)}(z)$. Mặt khác, ta có Sp$^{\Lambda}_{\mathscr{C}(K)}(z) = K$ (I, p. 42, ví dụ), và K là lồi đa thức theo giả thiết, nên suy ra rằng Sp$^{\Lambda}_A(z) = K$.

Vì đại số con có đơn vị sinh bởi họ các phần tử $z_{\lambda}$ là trù mật trong A, ánh xạ $\varphi$ là một đồng phôi từ $\mathsf{X}(A)$ lên Sp$^{\Lambda}_A(z) = K$ (Mệnh đề 12 của I, p. 43, a)). Đẳng thức $\varphi \circ$ ev = Id$_K$ khi đó cho thấy ev là đồng phôi nghịch đảo của $\varphi$.

Với mọi tập con $\Lambda '$ của Λ, ta ký hiệu bởi pr$_{\Lambda'}$ phép chiếu chính tắc $\mathbf{C}^{\Lambda}\rightarrow \mathbf{C}^{\Lambda'}$. Cho W là một tập con của $\mathbf{C}^{\Lambda}$ và V là bao lồi đa thức của nó. Đặt $W'=$ pr$_{\Lambda'}W$. Vì mọi phần tử của $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda'}]$ được đồng nhất với một phần tử của $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$, bao lồi đa thức của $W'$ được chứa trong pr$_{\Lambda'}V$.

#### Bổ đề 6 {#ts-i-s3-lem-6 .statement tag=028Z}

Cho $K\subset \mathbf{C}^{\Lambda}$ là một tập con compắc lồi đa thức và U là một lân cận của K. Tồn tại một tập con hữu hạn $\Lambda_0$ của Λ sao cho, với mọi tập con $\Lambda '$ của Λ chứa $\Lambda_0$, tập hợp pr$_{\Lambda'}(U)$ chứa bao lồi đa thức của pr$_{\Lambda'}(K)$.

Vì K là compắc, tồn tại một họ các đĩa compắc $D_{\lambda}$ trong $\mathbf{C}$ có tâm 0 và bán kính $R_{\lambda}$ sao cho K được chứa trong tích $D =\prod_{\lambda}D_{\lambda}$. Với mọi $P\in \mathbf{C}[(X_{\lambda})]$, gọi $K_P$ là tập hợp các

$x\in \mathbf{C}^{\Lambda}$ sao cho

$|P(x)|\leqslant$ sup$_{c\in K}|P(c)|$.

Ta có

$$
D\cap \bigcap_PK_P= K \tag{3}
$$

và tập hợp này được chứa trong U. Do đó, không gian D là hợp của tập mở $D\cap U$ và họ các tập mở D - $K_P$ với $P\in \mathbf{C}[(X_{\lambda})]$. Vì D là compắc, tồn tại một số nguyên $q\geqslant 1$ và các đa thức $P_1, . . . ,P_q\in \mathbf{C}[(X_{\lambda})]$ sao cho:

$$
D\cap K_{P_1}\cap  \cdots  \cap K_{P_q}\subset U \tag{4}
$$

Tồn tại một tập con hữu hạn $\Lambda_0\subset$ Λ sao cho $P_i\in \mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda_0}]$ với $1\leqslant i\leqslant q$. Ta sẽ chứng minh rằng $\Lambda_0$ thỏa mãn mệnh đề của bổ đề.

Cho $\Lambda '$ là một tập con của Λ chứa $\Lambda_0$. Gọi E là tập con của $\mathbf{C}^{\Lambda'}$ gồm các phần tử $c= (c_{\lambda})_{\lambda\in\Lambda'}$ được xác định bởi các bất đẳng thức $|c_{\lambda}|\leqslant R_{\lambda}$ với $\lambda \in \Lambda '$, và

$|P_i(c)|\leqslant$ sup$_{c\in K}|P_i(c)|$

với $i= 1, . . . ,q$. Tập con E là lồi đa thức (bổ đề 3) và công thức (3) chứng minh rằng pr$_{\Lambda'}(K)\subset E$.

Mặt khác, cho $c= (c_{\lambda})_{\lambda\in\Lambda'}\in E$; cho $d= (d_{\lambda})_{\lambda\in\Lambda}$ là phần tử của $\mathbf{C}^{\Lambda}$ được xác định bởi $d_{\lambda}=c_{\lambda}$ với $\lambda \in \Lambda '$ và $d_{\lambda}= 0$ với $\lambda \in \Lambda$- $\Lambda '$. Khi đó (4) suy ra $d\in U$, và do đó $c\in$ pr$_{\Lambda'}(U)$. Vậy $E\subset$ pr$_{\Lambda'}(U)$, điều này hoàn tất chứng minh.

#### Bổ đề 7 {#ts-i-s3-lem-7 .statement tag=0290}

Cho $n\geqslant 1$ là một số nguyên và K là một tập con compact lồi đa thức của $\mathbf{C}^n$. Khi đó K thừa nhận một hệ cơ bản các lân cận compact lồi đa thức.

Tồn tại một đa đĩa compact (x. VAR, R1, p. 24) Δ của $\mathbf{C}^n$ là một lân cận của K. Vì K lồi đa thức, nên tồn tại một họ $(P_i)_{i\in I}$ các phần tử của $\mathbf{C}[X_1, . . . ,X_n]$, và một họ $(M_i)_{i\in I}$ các số thực dương sao cho K là tập hợp các $z\in$ Δ thỏa mãn $|P_i(z)|\leqslant M_i$ với mọi $i$ (bổ đề 3). Với mỗi tập con hữu hạn J của I và mỗi $\varepsilon  >0$, gọi $K_{J,\varepsilon}$ là tập hợp các $z\in \Delta$ sao cho $|P_i(z)|\leqslant M_i+\varepsilon$ với $i\in J$. Khi đó mỗi tập hợp $K_{J,\varepsilon}$ là một lân cận compact lồi đa thức của K (loc. cit.), và giao của các tập hợp $K_{J,\varepsilon}$ là K. Do đó các tập hợp $K_{J,\varepsilon}$ tạo thành một hệ cơ bản các lân cận lồi đa thức của K (TG, I, p. 60, đl. 1).

## BÀI TẬP {#ts-i-s3-exercises}

Trong các bài tập dưới đây, mọi đại số được xét đều là trên $\mathbf{C}$, trừ khi có nói rõ ngược lại.

Xem [bài tập của § 3](exercises/s3/).
