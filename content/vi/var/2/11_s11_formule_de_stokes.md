---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 11
section_title: Formule de Stokes
lang: vi
source: var-fr
pdf_pages: 0136-0142
extraction: ocr
subsections:
    - "no": 1
      title: Pièces
      page: 0
      pdf_page: 136
    - "no": 2
      title: Formule de Stokes pour les pièces
      page: 0
      pdf_page: 137
    - "no": 3
      title: Formule de Stokes pour les ensembles localement polyédraux[^1]
      page: 0
      pdf_page: 138
    - "no": 4
      title: Formule de Stokes relative (intégration sur les fibres)
      page: 0
      pdf_page: 139
statements: 1
exercises: 0
content_sha256: fe1d36ac7b27ad3dd7a298870f87147c6c3ebcc6a984b9a60cff421436dbeb6e
translated_from: content/en-mt/var/2/11_s11_formule_de_stokes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: dd75a45f272b35f901b1a2d1405444b8385e25ecaa6feb881fa35299d399d447
translation_model: gpt-5-6
translation_run: translate-vi-b2d383d4
glossary_version: 34
glossary_terms_sha256: 293d43ad81412046505b20fc14b8a9b30199d51be6c26983dd08954e035d2bb1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 11. Công thức Stokes

Trong đoạn này, ta giả sử $\mathbf{K}=\mathbf{R}$.

### 11.1. Mảnh

### 11.1.1. Cho E là một không gian Banach. Một tập con S của E được gọi là một nửa không gian đóng nếu tồn tại một dạng tuyến tính liên tục $h\neq 0$ và một số thực $k$ sao cho $S=\{x|h(x)\leq k\}$ (xem EVT, II, § 2, No. 6); khi đó biên của S là siêu phẳng đóng $\{x|h(x)=k\}$; nó cũng được gọi là biên của S, và được ký hiệu bởi $\partial S$.

### 11.1.2. Cho X là một đa tạp thuộc lớp $C^r$ và A là một tập con của X. Ta nói rằng A là một mảnh của X nếu, với mọi $a\in A$, tồn tại một biểu đồ $c=(U,\varphi,E)$ của X tại a sao cho $\varphi(A\cap U)$ là một tập mở của một nửa không gian đóng của E. Ta đặt $\partial A=A-\mathring{A}$ (tập hợp các điểm không nội của A). Đây là một đa tạp con của A, được gọi là biên của A.[^1] Nếu $a\in\partial A$, tồn tại một biểu đồ $c=(U,\varphi,E)$ của X tâm tại a và một siêu phẳng đóng H của E sao cho $\varphi(A\cap U)$ là một lân cận mở của 0 trong một trong các nửa không gian đóng $S_c$ của E xác định bởi H (EVT, II, § 2, No. 6), và sao cho $\varphi(\partial A\cap U)=H\cap\varphi(A\cap U)$. Một biểu đồ như vậy được gọi là thích nghi với A tại a. Khi đó nửa không gian đóng $S_c$ là nửa không gian đóng duy nhất của E mà $\varphi(A\cap U)$ là một tập mở của nó.

Đối với một tập con đóng A của X là một mảnh của X, điều kiện cần và đủ là $\mathring{A}$ trù mật trong A và $A-\mathring{A}$ là một đa tạp con của X có đối chiều 1 tại mỗi điểm của nó.

### 11.1.3. Ví dụ

a) Trong $\mathbf{R}^n$, một quả cầu đóng bán kính $>0$ là một mảnh; biên của nó là mặt cầu tương ứng.

b) Nếu A là một mảnh của đa tạp X và B là một tập con đóng của $\partial A$, thì $A-B$ là một mảnh của X.

c) Cho $\varphi:X\rightarrow X'$ là một cấu xạ của các đa tạp thuộc lớp $C^r$, và cho $A'$ là một mảnh của $X'$. Nếu $\varphi$ ngang với $\partial A'$ (5.11.6), thì $\varphi^{-1}(A')$ là một mảnh của X có biên là $\varphi^{-1}(\partial A')$.

Đặc biệt, cho $h : X \to \mathbf{R}$ là một hàm thuộc lớp $C^r$, và cho $a \in \mathbf{R}$; giả sử không tồn tại $x \in X$ sao cho $h(x) = a$ và $d_x h = 0$. Tập hợp $\{ x | h(x) \leq a \}$ là một mảnh đóng của $X$ có biên $h^{-1}(a)$.

d) Nếu $r = \infty$ và X là compact địa phương, mọi tập con compact của X đều có một hệ lân cận cơ bản gồm các mảnh compact.

11.1.4. Cho $X$ là một đa tạp lớp $C^r$ và $A$ là một mảnh của $X$. Cho $a \in \partial A$ và $v \in T_a(X)$. Cho $c = (U, \varphi, E)$ là một biểu đồ của $X$ thích nghi với $A$ tại $a$ (11.1.2) và cho $h = \theta_c^{-1}(v)$ là phần tử của $E$ tương ứng với $v$ (5.5.1). Cho $S_c$ là nửa không gian đóng của $E$ mà $\varphi(A \cap U)$ là một tập hợp mở trong đó (11.1.2). Ta nói rằng $v$ là một *vectơ hướng vào* (tương ứng *hướng vào nghiêm ngặt*, tương ứng *hướng ra*, tương ứng *hướng ra nghiêm ngặt*) đối với $A$ tại $a$ nếu $h$ thuộc $S_c$ (tương ứng $\dot{S}_c, -S_c, -\dot{S}_c$), một điều kiện độc lập với lựa chọn biểu đồ thích nghi $c$. Ta ký hiệu $T_a^+(A)$ (tương ứng $T_a^-(A)$) là tập hợp các vectơ hướng ra (tương ứng hướng vào) của $T_a(X)$ đối với $A$. Đây là các nửa không gian đóng của $T_a(X)$, có biên chứa $0$. Ta có
$$
T_a(\partial A) = T_a^+(A) \cap T_a^-(A).
$$

**11.2. Công thức Stokes cho các mảnh**

Trong No. này, cho $X$ là một đa tạp tách được, thuần nhất lớp $C^r$ ($r \geq 2$) có số chiều hữu hạn $n$. Cho $A$ là một mảnh của $X$ và $i$ là đơn ánh chính tắc của $\partial A$ vào $X$. Cho $E$ là một không gian Banach.

11.2.1. Cho $x \in \partial A$ và cho $\xi$ là một định hướng của $T_x(\partial A)$; ta ký hiệu $\tilde{i}_x(\xi)$ là định hướng của $T_x(X)$ chứa các phần tử $v \wedge u$, trong đó $v$ là một vectơ hướng hoàn toàn ra ngoài đối với $A$ tại $x$ (11.1.4) và $u$ là một phần tử khác không của $\wedge^{n-1} T_x(\partial A)$ thuộc định hướng $\xi$. Ánh xạ $\tilde{i}_x$ là một song ánh của $\mathrm{Or}(T_x(\partial A))$ lên $\mathrm{Or}(T_x(X))$. Các ánh xạ $\tilde{i}_x$ với $x \in \partial A$ xác định một cấu xạ $\tilde{i} : \tilde{\partial A} \to \tilde{X}$ là một *định hướng* của $i$ (10.2.5). Nếu $\xi$ là một định hướng của $X$, thì định hướng của $\partial A$ liên kết với $\xi$ bởi $\tilde{i}$ (10.2.5) được gọi là *được xác định bởi* $\xi$.

#### Ví dụ {#var-2-s11-n2-exa-1 .statement}

Khi $X = \mathbf{R}^n$, $\xi$ là định hướng thông thường của $\mathbf{R}^n$ và $A$ là một quả cầu đóng bán kính $> 0$, định hướng của mặt cầu $\partial A$ được xác định bởi $\xi$ là định hướng chính tắc (10.2.8, b)).

11.2.2. Cho $\omega$ là một dạng vi phân xoắn bậc $p$ trên $X$ với các giá trị trong $E$ (10.4.1); ảnh ngược $i^*(\omega)$ của $\omega$ qua cấu xạ có định hướng $i : \partial A \to X$ được ký hiệu là $\omega|_{\partial A}$ và được gọi là *dạng cảm sinh bởi* $\omega$ *trên* $\partial A$ (cf. 10.4.3).

11.2.3. Ta xét một trong hai giả thiết sau:

(i) $\omega$ là một dạng vi phân xoắn bậc $n-1$ trên $X$, với các giá trị trong $E$;
(ii) $X$ có định hướng, $\partial A$ được trang bị định hướng tương ứng (11.2.1) và $\omega$ là một dạng vi phân bậc $n-1$ trên $X$ với các giá trị trong $E$.

Ngoài ra, giả sử rằng $\omega$ *thuộc lớp* $C^1$ và giao của $A$ với giá của $\omega$ là compact. Vi phân ngoài $d\omega$ của $\omega$ là liên tục (8.3.5 và 10.3.4).

Hàm đặc trưng của $A$ khả tích Lebesgue đối với độ đo vectơ xác định bởi $d\omega$ trên $X$ và dạng vi phân $\omega|_{\partial A}$ có bậc $n - 1$ trên $\partial A$ là khả tích (10.4.3 và 10.4.4). Ta có
$$
\int_A d\omega = \int_{\partial A} \omega \quad \text{(« công thức Stokes »)}.
$$
11.2.4. Cho $\alpha$ là một dạng vi phân xoắn có bậc $n$ trên $X$, nhận giá trị trong $E$, có giá compact và thuộc lớp $C^1$. Để tồn tại một dạng vi phân xoắn $\omega$ có bậc $n - 1$ trên $X$, nhận giá trị trong $E$, có giá compact và thuộc lớp $C^1$, sao cho $\alpha = d\omega$, điều kiện cần là $\int_X \alpha = 0$; nếu $X$ liên thông thì điều kiện này cũng đủ; nếu ngoài ra $\alpha$ thuộc lớp $C^k$ ($k \leq r - 1, k \neq \omega$), có thể chọn $\omega$ thuộc lớp $C^k$.

11.2.5. Giả sử $X$ là đa tạp thực nằm dưới $\mathbf{C}$, $E$ là một không gian Banach phức và $A$ là một mảnh *compact* của $X$. Trang bị cho $X$ định hướng xác định bởi cấu trúc phức của nó (10.2.7). Cho $f$ là một ánh xạ *liên tục* từ $A$ vào $E$ mà hạn chế của nó lên phần trong $\mathring{A}$ của $A$ là chỉnh hình. Ký hiệu $dz$ là vi phân của đơn ánh $z : \partial A \to \mathbf{C}$. Dạng $f.dz$, tích của $f$ và $dz$, là một dạng vi phân có bậc 1 trên $\partial A$, nhận giá trị trong $E$, thuộc lớp $C^0$, và ta có:
$$
\int_{\partial A} f.dz = 0 \quad \text{(« công thức Cauchy »)}.
$$
Khi $f$ mở rộng thành một ánh xạ chỉnh hình, vẫn ký hiệu là $f$, của một lân cận mở $U$ của $A$, nhận giá trị trong $E$, dạng vi phân $f.dz$ (trong đó $z$ lần này ký hiệu đơn ánh chính tắc của $U$ vào $\mathbf{C}$) thuộc lớp $C^\infty$ trên $U$ và vi phân ngoài của nó bằng không.

11.2.6 (*Đạo hàm của một tích phân*). Giả sử $X$ được định hướng. Cho $Y$ là một đa tạp thuộc lớp $C^r$, và $\alpha$ là một dạng vi phân bậc $n$ trên $Y$, nhận giá trị trong $E$, thuộc lớp $C^1$, và có giá compact. Cho $I$ là một tập con mở của $\mathbf{R}$ chứa 0 và cho $g : I \times X \to Y$ là một cấu xạ thuộc lớp $C^r$; với $t \in I$, ký hiệu $g_t$ là ánh xạ $x \mapsto g(t, x)$ từ $X$ vào $Y$. Ký hiệu $\psi$ là cấu xạ từ $X$ vào $T(Y)$ được xác định bởi $\psi(x) = T_{(0, x)}(g)(1, 0)$; đó là một *phép nâng* của $g_0$ (8.6.5). Giả sử hạn chế của $\mathrm{pr}_1 : I \times A \to I$ trên giao của $I \times A$ và giá của $g^*(\alpha)$ là *thực sự* (TG, I, § 10). Với mọi $t \in I$, khi đó giao của $A$ và giá của $g_t^*(\alpha)$ là compact; ánh xạ $t \mapsto \int_A g_t^*(\alpha)$ thuộc lớp $C^1$ trên $I$ và đạo hàm của nó tại gốc được cho bởi công thức
$$
\frac{d}{dt} \left( \int_A g_t^*(\alpha) \right)_{t=0} = \int_A \theta_\psi \cdot \alpha = \int_A i(\psi) \, d\alpha + \int_{\partial A} i(\psi) \, \alpha,
$$
xem No. 8.6.

### 11.3. Công thức Stokes cho các tập hợp đa diện địa phương[^2]

Trong No. này, $X$ ký hiệu một đa tạp thực thuần túy hữu hạn chiều thuộc lớp $C^r$ ($r \geq 2$); ta giả sử $X$ tách được.

11.3.1. Cho $A$ là một tập con của một không gian vectơ hữu hạn chiều thực. Ta nói rằng $A$ là đa diện nếu nó là một hợp hữu hạn của các giao hữu hạn của các nửa không gian đóng. Một tập con $A$ của $X$ được gọi là đa diện địa phương nếu, với mọi $x\in X$, tồn tại một bản đồ $c=(U,\varphi,E)$ của $X$ tại $x$ và một tập con đa diện $A_c$ của $E$ sao cho $\varphi(A\cap U)=\varphi(U)\cap A_c$. Một mảnh của $X$ là một tập con đa diện địa phương.

11.3.2. Cho $A$ là một tập con đóng của $X$, và cho $\operatorname{Fr}(A)=A-\mathring{A}$ là biên của nó. Một điểm $x\in\operatorname{Fr}(A)$ được gọi là chính quy nếu tồn tại một lân cận mở $U$ của $x$ sao cho $A\cap U$ là một mảnh của đa tạp $U$ (trong trường hợp đó $x$ thuộc biên của $A\cap U$). Ta ký hiệu $\partial A$ là tập hợp các điểm chính quy của $\operatorname{Fr}(A)$ và gọi nó là biên chính quy (hay đơn giản là biên) của $A$. Tập hợp $A'=\mathring{A}\cup\partial A$ là một mảnh của $X$, với biên $\partial A$.

11.3.3. *\** **Ví dụ.** — Cho $\mathscr{H}$ là một tập hợp hữu hạn địa phương các siêu phẳng của một không gian affine thực hữu hạn chiều $E$, và cho $C$ là một buồng của $E$ đối với $\mathscr{H}$ (LIE, V, § 1, No. 3). Bao đóng $\overline{C}$ của $C$ là một tập con đa diện địa phương của đa tạp $E$; biên chính quy của $\overline{C}$ là hợp của các mặt của $C$ (loc. cit., No. 4). Đặc biệt, nếu $C$ là một đơn hình mở (loc. cit., No. 6) có các đỉnh $a_0,\ldots,a_n$, thì biên của $\overline{C}$ là hợp của các $C_{(i)}$ ($0\leq i\leq n$), trong đó $C_{(i)}$ là đơn hình mở có các đỉnh $a_0,\ldots,a_{i-1},a_{i+1},\ldots,a_n$ trong không gian affine sinh bởi các đỉnh này.*\*

11.3.4. Cho $A$ là một tập con đa diện địa phương của $X$, và cho $\omega$ là một dạng vi phân xoắn bậc $n-1$ trên $X$ nhận giá trị trong một không gian Banach $E$; giả sử rằng $\omega$ thuộc lớp $C^1$ và giao của giá của nó với $A$ là compact. Khi đó hàm đặc trưng của $A$ (resp. $A'$, $\hat{A}$) khả tích thiết yếu đối với độ đo vectơ xác định bởi $d\omega$ trên $X$ và ta có

$$
\int_A d\omega=\int_{A'}d\omega=\int_{\hat{A}}d\omega.
$$

Dạng vi phân $\omega|\partial A$ (đối với định hướng chính tắc của đơn ánh chính tắc của $\partial A$, được xét như biên của mảnh $A'$, vào $X$) khả tích trên $\partial A$ và ta có

$$
\int_A d\omega=\int_{\partial A}\omega
\qquad\text{(« công thức Stokes »).}
$$

Khi $X$ được trang bị một định hướng, và $\partial A$ được trang bị định hướng tương ứng (11.2.1), công thức này vẫn đúng nếu $\omega$ là một dạng vi phân thông thường bậc $n-1$ nhận giá trị trong $E$, thuộc lớp $C^1$ và sao cho $A\cap\operatorname{Supp}\omega$ là compact.

### 11.4. Công thức Stokes tương đối (tích phân theo các thớ)

Trong số này, cho $X$ và $S$ là hai đa tạp (thực) thuộc lớp $C^r$ và cho $\pi:X\to S$ là một phép chìm. Cho $n$ là một số nguyên và giả sử rằng, với mọi $s\in S$, thớ $X_s=\pi^{-1}(s)$ của $\pi$ tại $s$ (là một đa tạp con của $X$ (5.10.5)) thuần túy có chiều $n$.

4—B.

11.4.1. Cho $E$ và $H$ là hai không gian vectơ và cho $F$ là một không gian con hữu hạn chiều của $H$ có chiều $n$. Cho $p$ là một số nguyên $\geqslant 0$, cho $u$ là một ánh xạ phản xứng $(n + p)$-tuyến tính từ $H^{n+p}$ vào $E$ và cho $t_1, \ldots, t_p$ là các phần tử của $H/F$; cho $t'_1, \ldots, t'_p$ là các đại diện của $t_1, \ldots, t_p$ trong $H$. Ánh xạ

$$
(x_1, \ldots, x_n) \mapsto u(t'_1, \ldots, t'_p, x_1, \ldots, x_n)
$$

là một ánh xạ phản xứng $n$-tuyến tính từ $F^n$ vào $E$, chỉ phụ thuộc vào $u$ và các $t_i$; nó được ký hiệu bởi $u \perp (t_1, \ldots, t_p)$ (xem A, III, p. 158 trong trường hợp riêng $E = K$). Ánh xạ

$$
(t_1, \ldots, t_p) \mapsto u \perp (t_1, \ldots, t_p)
$$

là phản xứng $p$-tuyến tính.

11.4.2 (« $\pi$-xoắn »). Xét bó vectơ T(X/S) trên $X$ (8.1.3); nó có hạng hữu hạn $n$ tại mọi điểm của $X$. Đặt $\tilde{R}_\pi = \tilde{R}_{T(X/S)}$ (10.3.1) và $\tilde{X}_\pi = \mathrm{Or}_{T(X/S)}$ (10.2.2). Cho $s \in S$; theo sự đồng nhất tự nhiên của $T(X/S)|_{X_s}$ với $T(X_s)$ (8.1.3), thớ tại $s$ của ánh xạ $\tilde{\pi}: \tilde{X}_\pi \to S$ hợp thành bởi $\pi$ và ánh xạ chính tắc $\tilde{X}_\pi \to X$, là $\tilde{X}_s$ (10.2.4). Một dạng vi phân được $\pi$-xoắn trên $X$ được gọi là một dạng vi phân được $T(X/S)$-xoắn (10.3.3).

11.4.3 (« Định hướng S của một cấu xạ S »). Cho $X'$ là một đa tạp được trang bị một phép chìm $\pi': X' \to S$ có các thớ $X_s$ thuần túy có số chiều hữu hạn $n'$, và cho $\varphi: X' \to X$ là một cấu xạ sao cho $\pi' = \pi \circ \varphi$. Một định hướng S của $\varphi$ được gọi là một cấu xạ $\tilde{\varphi}: \tilde{X}'_\pi \to \tilde{X}_\pi$, giao hoán với tác động của nhóm $\{ \pm 1 \}$ và sao cho biểu đồ

$$
\begin{array}{ccc}
\tilde{X}'_\pi & \xrightarrow{\tilde{\varphi}} & \tilde{X}_\pi \\
| & & | \\
X' & \xrightarrow{\varphi} & X
\end{array}
$$

là giao hoán. Dữ liệu của một định hướng S của $\varphi$ cho phép, như trong 10.4.2, đồng nhất các bó $\tilde{R}_{\pi'}$ và $\varphi^*(\tilde{R}_\pi)$ và định nghĩa ảnh ngược của một dạng vi phân xoắn $\pi$ qua cấu xạ định hướng S $\varphi$: đó là một dạng vi phân xoắn $\pi'$ trên $X'$.

11.4.4. Cho A là một mảnh của X sao cho hạn chế của $\pi$ lên $\partial A$ là một phép chìm. Với mọi $s \in S$, thớ $X_s = \pi^{-1}(s)$ là một đa tạp con của X cắt ngang $\partial A$ và $A \cap X_s$ là một mảnh của $X_s$, được ký hiệu là $A_s$, có biên $\partial A \cap X_s$.

Cho i là đơn ánh chính tắc của $\partial A$ vào X. Tồn tại duy nhất một định hướng S $\tilde{i}$ của i sao cho, với mọi $s \in S$, hạn chế của $\tilde{i}$ lên $(\partial A_s)^*$ (được đồng nhất với thớ tại s của phép chìm $\partial \tilde{A}_{\pi|\partial A} \to S$) là định hướng được định nghĩa trong 11.2.1 của đơn ánh chính tắc của $\partial A_s$ vào $X_s$. Nếu $\omega$ là một dạng vi phân xoắn $\pi$ trên X, ảnh ngược của $\omega$ qua cấu xạ i được định hướng như vậy được ký hiệu là $\omega|\partial A$ (xem 11.2.2).

11.4.5. (« Tích trong »). Cho $p$ là một số nguyên $\geqslant 0$ và cho $\omega$ là một dạng vi phân xoắn $n$ có bậc $n + p$ trên $X$, nhận giá trị trong một bó vectơ $E$ có cơ sở X. Cho $s \in S$ và $x \in X_s$; ta có $\omega(x) = \xi \otimes u$, trong đó $\xi$ là một định hướng của $T_x(X_s) = T(X/S)_x$, được đồng nhất với một phần tử của $(\tilde{R}_{X_s})_x = (\tilde{R}_\pi)_x$ (10.3.2), và trong đó $u$ là một ánh xạ tuyến tính phản xứng $(n + p)$-tuyến tính từ $T_x(X)$ vào $E_x$. Cho $t_1, \ldots, t_p$ là các vectơ tiếp xúc với S tại $s$. Đặt

$$
\theta(x) = \xi \otimes (u \wedge (t_1, \ldots, t_p)) \in (\tilde{R}_{X_s})_x \otimes (\mathrm{Alt}^n(T(X); E))_x
$$

(xem 11.4.1). Điều này định nghĩa một dạng vi phân xoắn $\theta : x \mapsto \theta(x)$ có bậc $n$ trên $X_s$, nhận giá trị trong $E|X_s$. Ta ký hiệu nó bởi $\omega \wedge (t_1, \ldots, t_p)$.

Đặc biệt, cho $M$ là một bó vectơ lớp $C^{r-1}$ trên $S$ và lấy $E = \pi^*(M)$. Bó $E|X_s$ được đồng nhất một cách tự nhiên với bó tầm thường trên $X_s$ xác định bởi không gian Banach $M_s$, và dạng $\omega \wedge (t_1, \ldots, t_p)$ được đồng nhất với một dạng vi phân xoắn trên $X_s$, với các giá trị trong $M_s$.

11.4.6. Giữ lại các ký hiệu trước đó (đặc biệt $E = \pi(*M)$) và giả sử thêm rằng $X$ là tách được và $\omega$ liên tục. Cho $A$ là một mảnh của $X$ sao cho hạn chế của $\pi$ lên $\partial A$ là một phép ngập và hạn chế của $\pi$ lên giao của $A$ và giá của $\omega$ là thực sự. Với $s \in S$ và $t_1, \ldots, t_p$ trong $T_s(S)$, dạng $\omega \wedge (t_1, \ldots, t_p)$ (11.4.5) là một dạng vi phân xoắn liên tục bậc $n$ trên $X_s$, với các giá trị trong không gian Banach $M_s$, và giá của nó gặp $A_s$ trong một tập compact. Tồn tại duy nhất một dạng vi phân $\alpha$ bậc $p$ trên $S$, với các giá trị trong bó vectơ $M$, sao cho

$$
\alpha(s)(t_1, \ldots, t_p) = \int_{A_s} \omega \wedge (t_1, \ldots, t_p)
$$

với mọi $s \in S$ và $t_1, \ldots, t_p$ trong $T_s(S)$. Dạng $\alpha$ được ký hiệu là $\int_{\pi|A} \omega$ (hoặc đơn giản là $\int_\pi \omega$ khi $A = X$); nó được gọi là thu được bằng cách lấy tích phân của $\omega$ trên $A$ dọc theo các thớ của $\pi$. Nếu $\omega$ là dạng lớp $C^k$ ($0 \leq k \leq r - 1, k \leq \infty$), thì điều tương tự cũng đúng với $\int_{\pi|A} \omega$.

Khi $\omega$ là một dạng bậc $< n$, ta quy ước rằng $\int_{\pi|A} \omega = 0$.

11.4.7. Giữ lại các giả thiết và ký hiệu trước đó.

a) Với mọi dạng vi phân vô hướng liên tục $\beta$ trên $S$, ta có

$$
\int_{\pi|A} (\pi^*\beta) \wedge \omega = \beta \wedge \int_{\pi|A} \omega.
$$

b) Cho $\eta$ là một trường vectơ liên tục trên $X$ và $\zeta$ là một trường vectơ liên tục trên $S$, sao cho $\eta$ là $\pi$-liên quan với $\zeta$ (8.2.6). Ta có

$$
i(\zeta) \int_{\pi|A} \omega = \int_{\pi|A} i(\eta)\omega.
$$

c) Giả sử thêm rằng $\eta, \zeta$ và $\omega$ thuộc lớp $C^1$, rằng $\eta(x) \in T_x(\partial A)$ với mọi $x \in \partial A$ và rằng $M$ là bó vectơ tầm thường được xác định bởi một không gian Banach $E$. Ta có

$$
\theta_\zeta \cdot \int_{\pi|A} \omega = \int_{\pi|A} \theta_\eta \cdot \omega,
$$

(xem 8.4.2 và 10.3.4).

d) Nếu $\omega$ có bậc $n + p$ và thuộc lớp $C^1$, ta có
$$
d \left( \int_{\pi|A} \omega \right) = \int_{\pi|A} d\omega + (-1)^p \int_{\pi|\partial A} \omega|_{\partial A}.
$$
e) Giả sử rằng S thu về một điểm. Khi đó các dạng xoắn theo $\pi$ trên X là các dạng xoắn thông thường (10.4.1). Nếu $\omega$ có bậc $n$, dạng $\int_{\pi|A} \omega$ có bậc 0 trên S là hằng $\int_A \omega$ (10.4.3).

11.4.8. Cho $\pi': S \to S'$ là một phép chìm sao cho các thớ của $\pi'$ là các đa tạp con thuần có số chiều hữu hạn hằng $n'$. Đặt $\pi'' = \pi' \circ \pi$; đó là một phép chìm từ X lên S' mà các thớ của nó là các đa tạp con thuần có chiều $m = n + n'$.

Cho $x \in X$. Dãy
$$
0 \longrightarrow T(X/S)_x \xrightarrow{\mathrm{Id}} T(X/S')_x \xrightarrow{T_x(\pi)} T(S/S')_{\pi(x)} \longrightarrow 0
$$
là khớp. Tồn tại duy nhất một đẳng cấu $j$ của bó vectơ $\tilde{R}_{\pi} \otimes \pi^*(\tilde{R}_{\pi'})$ lên $\tilde{R}_{\pi''}$ sao cho, nếu $\xi$ (tương ứng $\eta$) là một định hướng của $T(X/S)_x$ (tương ứng của $(\pi^*T(S/S'))_x$) được đồng nhất với $T(S/S')_{\pi(x)}$, thì ta có $j(\xi \otimes \eta) = \eta \xi$ (tích được xác định bởi dãy khớp trước đó (10.2.1)).

Cho $M'$ là một bó vectơ có cơ sở $S'$; đặt $M = {\pi'}^*(M')$, và $E = \pi^*(M) = {\pi''}^*(M')$. Nếu $\omega$ là một dạng vi phân xoắn theo $\pi''$ trên X với giá trị trong E, đẳng cấu $j$ cho phép đồng nhất nó với một dạng xoắn theo $\pi$ với giá trị trong $\pi^*(\tilde{R}_{\pi'}) \otimes E$, hoặc tương đương với giá trị trong $\pi^*(\tilde{R}_{\pi'} \otimes M)$.

Ngoài ra, cho A là một mảnh của X sao cho $\pi|\partial A : \partial A \to S$ là một phép hạ chìm; khi đó điều tương tự cũng đúng đối với $\pi''|\partial A : \partial A \to S'$. Giả sử thêm rằng $\omega$ liên tục và rằng hạn chế của $\pi''$ lên $A \cap \operatorname{Supp} \omega$ là thực sự; khi đó điều tương tự cũng đúng đối với hạn chế của $\pi$ lên $A \cap \operatorname{Supp} \omega$. Một mặt, ta có thể xét dạng vi phân $\int_{\pi''|A} \omega$ trên $S'$, là một dạng với giá trị trong $M'$, và mặt khác, dạng vi phân $\int_{\pi|A} \omega$ trên S, là một dạng với giá trị trong $\tilde{R}_{\pi'} \otimes M$, hay tương đương là một dạng xoắn $\pi'-$ với giá trị trong $M = {\pi'}^*(M')$. Hơn nữa, $\pi(A)$ là một đa tạp con mở của S và hạn chế của $\pi'$ lên $\pi(A) \cap \operatorname{Supp} \int_{\pi|A} \omega$ là thực sự. Dạng vi phân $\int_{\pi'|_{\pi(A)}} \int_{\pi|A} \omega$ được xác định; nó là một dạng vi phân trên $S'$, với giá trị trong $M'$. Ta có
$$
\int_{\pi' \circ \pi|A} \omega = \int_{\pi'|_{\pi(A)}} \int_{\pi|A} \omega.
$$
Nếu $A = X$, ta có
$$
\int_{\pi' \circ \pi} \omega = \int_{\pi'} \int_{\pi} \omega.
$$

[^1]: Thuật ngữ này xuất phát từ sự kiện rằng A được trang bị một cách tự nhiên một cấu trúc của một “đa tạp có biên”, với biên $\partial A$. Để biết định nghĩa của phạm trù này, cũng như nói chung hơn, của phạm trù các “đa tạp có góc”, độc giả có thể tham khảo H. CARTAN, Séminaire 1961/62, Topologie Différentielle, exposés 1-2-3 (par A. DOUADY), Benjamin, New York, 1969. Ta hãy chỉ ra rằng người ta có thể chứng minh rằng mọi “đa tạp có biên” mà biên là paracompact đều đẳng cấu với một mảnh đóng của một đa tạp.
[^2]: Độc giả quan tâm đến các trường hợp tổng quát hơn có thể tham khảo H. WHITNEY, Geometric Integration Theory, Chap. III, § 18 (Princeton Univ. Press, 1957).
