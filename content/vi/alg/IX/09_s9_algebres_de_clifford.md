---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 9
section_title: Algèbres de Clifford
lang: vi
source: alg-ix-fr
pdf_pages: 0137-0158
extraction: ocr
subsections:
    - "no": 1
      title: Définition et propriété universelle de l’algèbre de Clifford.
      page: 0
      pdf_page: 137
    - "no": 2
      title: Quelques opérations dans l’algèbre tensorielle.
      page: 0
      pdf_page: 139
    - "no": 3
      title: Base de l’algèbre de Clifford.
      page: 0
      pdf_page: 141
    - "no": 4
      title: Structure de l’algèbre de Clifford.
      page: 0
      pdf_page: 144
    - "no": 5
      title: Groupe de Clifford.
      page: 0
      pdf_page: 148
statements: 24
exercises: 0
content_sha256: ee2d1a682ff713a4454555f5034513e6261d1632c48f8b019209328165737a4b
translated_from: content/en-mt/alg/IX/09_s9_algebres_de_clifford.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 355af7c8ef8453df16903a634621da0925a1f8d1741b4a808ddc188a9e4815d8
translation_model: gpt-5.4
translation_run: translate-vi-35f4c7df
glossary_version: 34
glossary_terms_sha256: e946a6f18a2f4484bfc095642cbb4631f7eba6202c0223d53b89e0adaf87b3f6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. Đại số Clifford

Trong đoạn này, ta giả sử rằng vành $\mathbf{A}$ là giao hoán. Ta sẽ ký hiệu bởi $Q$ một dạng toàn phương trên $\mathbf{A}$-môđun $E$, và bởi $\Phi$ dạng song tuyến tính liên kết ($§\ 3$, No. 4).

### 1. Định nghĩa và tính chất phổ quát của đại số Clifford.

#### Định nghĩa 1 {#alg-ix-s9-def-1 .statement}

Đại số Clifford của $Q$, ký hiệu bởi $C(Q)$, là đại số thương của đại số tenxơ $T(E)$ của môđun $E$ theo iđêan hai phía (ký hiệu bởi $I(Q)$) sinh bởi các phần tử có dạng $x \otimes x - Q(x)\cdot 1$ $(x \in E)$.

Ta sẽ ký hiệu bởi $\rho_Q$ (hoặc đơn giản bởi $\rho$ khi không có nguy cơ nhầm lẫn) ánh xạ từ $E$ vào $C(Q)$ hợp thành bởi ánh xạ chính tắc từ $E$ vào $T(E)$ và ánh xạ chính tắc $\sigma$ từ $T(E)$ lên $C(Q)$; ánh xạ $\rho_Q$ được gọi là chính tắc. Chú ý rằng $C(Q)$ được sinh bởi $\rho_Q(E)$, và với $x \in E$, ta có

$$
\rho(x)^2 = Q(x)\cdot 1;
$$

do đó, thay thế $x$ bởi $x + y$ ($x,\ y$ trong $E$)

$$
\rho(x)\rho(y) + \rho(y)\rho(x) = \Phi(x,\ y)\cdot 1
$$

#### Ví dụ {#alg-ix-s9-n1-exa-1 .statement}

Nếu $E$ thừa nhận một cơ sở gồm một phần tử duy nhất $e$, thì $T(E)$ đẳng cấu với đại số đa thức $\mathbf{A}[X]$, và $C(Q)$ là một mở rộng bậc hai của $\mathbf{A}$, có cơ sở là $(1,\ u)$, trong đó $u$ là phần tử $u = \rho(e)$ và thỏa mãn $u^2 = Q(e)$.

Ký hiệu bởi $T^h$ lũy thừa tenxơ bậc $h$, $\bigotimes^h E$, trong $T(E)$, và gọi $T^+$ (tương ứng $T^-$) là tổng của các $T^h$ với $h$ chẵn (tương ứng lẻ).

Vì $T(E)$ là tổng trực tiếp của $T^+$ và $T^-$ và $I(Q)$ được sinh bởi các phần tử của $T^+$, nên $I(Q)$ là tổng trực tiếp của $T^+ \cap I(Q)$ và $T^- \cap I(Q)$, và $C(Q)$ là tổng trực tiếp của hai môđun con $C^+(Q) = \sigma(T^+)$ và $C^-(Q) = \sigma(T^-)$ (cũng được ký hiệu là $C^+$ và $C^-$). Các phần tử của $C^+$ sẽ được gọi là chẵn (tương ứng, lẻ). Ta có các quan hệ

(3) $C^+C^+ \subset C^+, \quad C^+C^- \subset C^-, \quad C^-C^+ \subset C^-, \quad C^-C^- \subset C^+$.

Đặc biệt $C^+$ là một đại số con của $C(Q)$.

#### Mệnh đề 1 {#alg-ix-s9-prop-1 .statement}

*Cho f là một ánh xạ tuyến tính từ E vào một đại số D trên A sao cho $f(x)^2 = Q(x).1$ với mọi $x \in E$. Tồn tại một và chỉ một đồng cấu $\bar{f}$ từ $C(Q)$ vào D sao cho $f = \bar{f} \circ \rho_Q$.

Tính duy nhất của $\bar{f}$ suy ra từ việc $C(Q)$ được sinh bởi $\rho_Q(E)$. Gọi $h$ là đồng cấu duy nhất từ $T(E)$ vào D mở rộng $f$ ($h$ được xác định bởi $h(x_1 \otimes \cdots \otimes x_n) = f(x_1) \ldots f(x_n)$). Ta có

$$
h(x \otimes x - Q(x).1) = (f(x)^2 - Q(x)).1 = 0,
$$

và do đó $h$ triệt tiêu trên $I(Q)$ và xác định, bằng cách chuyển qua thương, đồng cấu $\bar{f}$ đang xét.

Mệnh đề 1 biểu thị rằng $C(Q)$ là nghiệm của một bài toán ánh xạ phổ quát (*Tập hợp*, Chương IV, § 3, No. 1).

Lấy riêng cho D đại số đối của $C(Q)$ và cho $f$ ánh xạ $\rho$; mệnh đề 1 kéo theo rằng tồn tại một và chỉ một phản tự đẳng cấu $\beta$ của $C(Q)$ mà hạn chế trên $\rho(E)$ là đồng nhất; nó được gọi là phản tự đẳng cấu *chính* của $C(Q)$. Hiển nhiên là $\beta^2 = 1$.

Mặt khác cho $Q'$ là một dạng toàn phương trên một A-môđun $E'$ và $f$ là một ánh xạ tuyến tính từ $E$ vào $E'$ sao cho $Q' \circ f = Q$. Ta có $\rho_Q(f(x))^2 = Q'(f(x)).1 = Q(x).1$, và do đó tồn tại một và chỉ một đồng cấu $C(f)$ từ $C(Q)$ vào $C(Q')$ sao cho $C(f) \circ \rho_Q = \rho_{Q'} \circ f$. Nếu $f$ là ánh xạ đồng nhất, thì $C(f)$ là đồng nhất; nếu $Q''$ là một dạng toàn phương trên một A-môđun $E''$ và $g$ là một ánh xạ tuyến tính từ $E'$ vào $E''$ sao cho $Q'' \circ g = Q'$, thì ta có $C(g \circ f) = C(g) \circ C(f)$. Khi $E'$ là một môđun con của $E$ và $f$ là đơn ánh chính tắc từ $E'$ vào $E$ (để $Q'$ là hạn chế của $Q$ lên $E'$), ta nói rằng $C(f)$ là đồng cấu *chính tắc* từ $C(Q')$ vào $C(Q)$.

Hãy lấy riêng $Q' = Q$ và $f$ là ánh xạ $x \to -x$; ta thấy rằng tồn tại một và chỉ một tự đẳng cấu $\alpha$ của $C(Q)$ sao cho $\alpha \circ \rho = -\rho$; nó được gọi là tự đẳng cấu chính của $C(Q)$. Hiển nhiên là $\alpha^2 = 1$, và hạn chế của $\alpha$ lên $C^+$ (resp. $C^-$) là đồng nhất (resp. ánh xạ $u \to -u$).

#### Mệnh đề 2 {#alg-ix-s9-prop-2 .statement}

Cho $A'$ là một vành giao hoán, $\varphi$ là một đồng cấu từ $A$ vào $A'$, $Q’$ là dạng toàn phương trên $E' = A' \otimes_A E$ suy ra từ $Q$ bởi mở rộng các vô hướng ($§ 3$, no 4, mệnh đề 3). Tồn tại một và chỉ một đẳng cấu $j$ từ đại số $A' \otimes_A C(Q)$ lên $C(Q')$ sao cho $j (1 \otimes \rho_Q(x)) = \rho_{Q'}(1 \otimes x)$ với mọi $x \in E$.

Chỉ cần chứng minh rằng đại số $C' = A' \otimes C(Q)$ và ánh xạ $1 \otimes \rho_Q$ từ $E'$ vào $C'$ tạo thành một nghiệm của cùng bài toán ánh xạ phổ quát như $C(Q')$ và $\rho_{Q'}$. Bây giờ, cho D’ là một đại số trên $A'$ và cho $f'$ là một ánh xạ $A'$-tuyến tính từ $E'$ vào D’ sao cho $f'(x')^2 = Q'(x').1$ với mọi $x' \in E'$. Ánh xạ $g : x \to f' (1 \otimes x)$ từ E vào D’ (được xét như một A-môđun bằng đồng cấu $\varphi$) là A-tuyến tính và ta có $g(x)^2 = Q' (1 \otimes x).1 = Q(x).1$ với mọi $x \in E$. Do đó tồn tại một và chỉ một A-đồng cấu $\overline{g}$ từ $C(Q)$ vào D’ sao cho $\overline{g}(\rho_Q(x)) = f'(1 \otimes x)$. Do đó tồn tại một và chỉ một $A'$-đồng cấu $\overline{f}'$ từ $C'$ vào D’ sao cho $\overline{f}'(1 \otimes \rho_Q(x)) = f'(1 \otimes x)$ với mọi $x \in E$; theo tính tuyến tính suy ra $\overline{f}'((1 \otimes \rho_Q)(x')) = f'(x')$ với mọi $x' \in E'$. ĐPCM.

### 2. Một số phép toán trong đại số tenxơ.

Trong số này ta sẽ ký hiệu bởi $e_x$ ($x \in E$) ánh xạ tuyến tính $u \to x \otimes u$ từ đại số tenxơ T(E) vào chính nó.

#### Bổ đề 1 {#alg-ix-s9-lem-1 .statement}

Cho $f$ là một phần tử của đối ngẫu $E^*$ của E. Tồn tại một và chỉ một ánh xạ tuyến tính $i_f$ từ T(E) vào chính nó sao cho
$$
i_f(1) = 0 \tag{4}
$$
$$
i_f \circ e_x + e_x \circ i_f = f(x).I \tag{5}
$$
với mọi $x \in E$
(trong đó I ký hiệu ánh xạ đồng nhất). Ánh xạ $f \to i_f$ từ $E^*$ vào $\mathcal{L}(T(E))$ là tuyến tính. Ta có $i_f(T^n) \subset T^{n-1}$, $(i_f)^2 = 0$, và $i_f \circ i_g + i_g \circ i_f = 0$ với $f, g$ trong $E^*$. Ánh xạ $i_f$ bằng không trên đại số con của

T(E) sinh bởi hạt nhân của f. Iđêan I(Q) ổn định dưới $i_f$; chuyển qua thương, do đó $i_f$ xác định một ánh xạ tuyến tính (vẫn ký hiệu bởi $i_f$) từ $C(Q)$ vào chính nó.

Thật vậy công thức (5) có thể được viết

$$
i_f(x \otimes u) = -x \otimes i_f(u) + f(x) \cdot u \quad (x \in E,\ u \in T(E)).
$$

Vì (4) xác định hoàn toàn $i_f$ trên $T^0$, và vì (6) xác định $i_f$ trên $T^n$ nếu các giá trị của nó trên $T^{n-1}$ đã biết, nên tính duy nhất của $i_f$ được chứng minh. Mặt khác, với $x \in E$ và $u \in T^{n-1}$, vế phải của (6) là song tuyến tính trên $E \times T^{n-1}$; điều này chứng minh sự tồn tại của $i_f$ bằng quy nạp theo $n$ (Ch. III, § 1, No. 2) và cũng chứng minh, bằng quy nạp theo $n$, rằng $i_f(T^n) \subset T^{n-1}$. Nếu $f = ag + bh$ (a, b thuộc A, g, h thuộc E*) thì hiển nhiên $ai_g + bi_h$ thỏa mãn (4) và (5), nên bằng $i_f$. Ta có

$$
(i_f)^2 \circ e_x = -i_f \circ e_x \circ i_f + f(x)i_f = e_x \circ (i_f)^2
$$

và, vì $(i_f)^2(1) = 0$, suy ra bằng quy nạp theo $n$ rằng $(i_f)^2$ bằng không trên $T^n$. Thay thế $f$ bởi $f + g$, quan hệ $(i_f)^2 = 0$ cho $i_f \circ i_g + i_g \circ i_f = 0$. Một lập luận tương tự bằng quy nạp như các lập luận trước cho thấy $i_f$ bằng không trên đại số con sinh bởi hạt nhân của $f$. Cuối cùng, (6) kéo theo rằng tập hợp các phần tử $u$ của $I(Q)$ sao cho $i_f(u) \in I(Q)$ là một iđêan trái của $T(E)$; hơn nữa, nếu $u = (x \otimes x - Q(x) \cdot 1) \otimes \nu$ ($x \in E,\ \nu \in T(E)$), ta có

$$
\begin{align*}
i_f(u) &= f(x)x \otimes \nu - x \otimes i_f(x \otimes \nu) - Q(x)i_f(\nu) \\
&= f(x)x \otimes \nu - f(x)x \otimes \nu + x \otimes x \otimes i_f(\nu) - Q(x)i_f(\nu) \\
&= (x \otimes x - Q(x) \cdot 1) \otimes i_f(\nu);
\end{align*}
$$

do đó $I(Q)$ ổn định dưới $i_f$, và khẳng định cuối cùng suy ra. CQFD.

Cho F là một dạng song tuyến tính trên E; trong phần còn lại của đoạn này, ta sẽ ký hiệu bởi $i_x^F$ ($x \in E$) ánh xạ $i_f$ tương ứng với dạng tuyến tính $f : y \to F(x, y)$ trên E.

#### Bổ đề 2 {#alg-ix-s9-lem-2 .statement}

Tồn tại một và chỉ một ánh xạ tuyến tính $\lambda_F$ từ $T(E)$ vào chính nó sao cho

$$
\begin{align*}
\lambda_F(1) &= 1 \\
\lambda_F \circ e_x &= (e_x + i_x^F) \circ \lambda_F \qquad (x \in E).
\end{align*}
$$

Với mọi $f \in E^*$, ta có

$$
\lambda_F \circ i_f = i_f \circ \lambda_F.
$$

Thật vậy, công thức (8) tương đương với

$$
\lambda_F(x \otimes u) = x \otimes \lambda_F(u) + i_x^F(\lambda_F(u)) \quad (x \in E, u \in T(E)).
$$

Vì (7) xác định hoàn toàn $\lambda_F$ trên $T^0$, và vì (10) xác định $\lambda_F$ trên $T^n$ nếu các giá trị của nó trên $T^{n-1}$ đã biết, nên tính duy nhất của $\lambda_F$ được chứng minh. Mặt khác, với $x \in E$ và $u \in T^{n-1}$, vế phải của (10) là song tuyến tính trên $E \times T^{n-1}$; điều này chứng minh sự tồn tại của $\lambda_F$ bằng quy nạp theo $n$. Còn lại phải chứng minh (9), điều mà ta sẽ làm bằng quy nạp; cả hai vế của (9) đều bằng không trên $T^0$; giả sử (9) đúng trên $\sum_{h=0}^{n-1} T^h$; khi đó, với $x \in E$ và $u \in T^{n-1}$, ta có:

$$
\begin{align*}
(\lambda_F \circ i_f)(x \otimes u) &= (-\lambda_F \circ e_x \circ i_f + f(x)\lambda_F)(u) \\
&= -(e_x + i_x^F) \circ \lambda_F \circ i_f(u) + f(x)\lambda_F(u) \\
&= -(e_x + i_x^F) \circ i_f \circ \lambda_F(u) + f(x)\lambda_F(u) \\
&= (i_f \circ e_x \circ \lambda_F - f(x)\lambda_F + i_f \circ i_x^F \circ \lambda_F + f(x)\lambda_F)(u) \\
&= (i_f \circ (e_x + i_x^F) \circ \lambda_F)(u) = (i_f \circ \lambda_F)(x \otimes u),
\end{align*}
$$

do đó có khẳng định cuối cùng của ta.

#### Bổ đề 3 {#alg-ix-s9-lem-3 .statement}

Cho F và G là hai dạng song tuyến tính trên E. Ta có $\lambda_F \circ \lambda_G = \lambda_{F+G}$. Với mọi dạng song tuyến tính F trên E, $\lambda_F$ là một song ánh của $T(E)$ lên chính nó.

Thật vậy, $\lambda_F \circ \lambda_G$ có các tính chất đặc trưng (7) và (8) của $\lambda_{F+G}$: ta có $(\lambda_F \circ \lambda_G)(1) = 1$, và

$$
\begin{align*}
\lambda_F \circ \lambda_G \circ e_x &= \lambda_F \circ (e_x + i_x^G) \circ \lambda_G = (e_x + i_x^G + i_x^F) \circ \lambda_F \circ \lambda_G \\
&= (e_x + i_x^{F+G}) \circ \lambda_F \circ \lambda_G.
\end{align*}
$$

Mặt khác, nếu $F = 0$, ta có $i_x^F = 0$ với mọi $x \in E$, và do đó $\lambda_F = I$, suy ra rằng, với mọi F, ta có $\lambda_F \circ \lambda_{-F} = \lambda_{-F} \circ \lambda_F = I$.

### 3. Cơ sở của đại số Clifford.

#### Mệnh đề 3 {#alg-ix-s9-prop-3 .statement}

Cho Q và Q' là hai dạng toàn phương và F là một dạng song tuyến tính trên E sao cho $Q'(x) = Q(x) + F(x, x)$ với mọi $x \in E$. Ánh xạ $\lambda_F$ biến iđêan $I(Q')$ thành iđêan $I(Q)$, và xác định một đẳng cấu (ký hiệu là $\overline{\lambda_F}$) của A-môđun $C(Q')$ lên A-môđun $C(Q)$.

Vì $\lambda_F$ là một song ánh mà song ánh ngược là $\lambda_{-F}$ (Bổ đề 3), chỉ cần chứng minh bao hàm thức $\lambda_F(I(Q')) \subset I(Q)$. Vì $I(Q)$ là một iđêan trái ổn định dưới $i_x^F$ (Bổ đề 1), (8) cho thấy rằng tập hợp các $u \in T(E)$ sao cho $\lambda_F(u) \in I(Q)$ là một iđêan trái. Do đó chỉ cần chứng minh rằng, với mọi $u \in T(E)$ và $x \in E$, ta có $\lambda_F(x \otimes x \otimes u - Q'(x)u) \in I(Q)$. Bây giờ, theo (8) và Bổ đề 1, ta có
$$
\lambda_F \circ e_x^2 = (e_x + i_x^F)^2 \circ \lambda_F = (e_x^2 + F(x, x)) \circ \lambda_F,
$$
do đó
$$
\begin{align*}
\lambda_F(x \otimes x \otimes u - Q'(x)u) &= (e_x^2 + F(x, x) - Q'(x)) \circ \lambda_F(u) \\
&= (x \otimes x - Q(x)) \otimes \lambda_F(u) \in I(Q).
\end{align*}
$$

#### Bổ đề 4 {#alg-ix-s9-lem-4 .statement}

Nếu dạng toàn phương $Q$ bằng không, thì $C(Q)$ không là gì khác ngoài đại số ngoài của E.

Thật vậy, đại số ngoài của $E$ không gì khác hơn là thương của $T(E)$ bởi iđêan hai phía $J$ sinh bởi các phần tử dạng $a \otimes \nu \otimes a$ ($a \in E, \nu \in T(E)$) (Chương III, § 5, No. 5 và No. 9). Hiển nhiên là $I(Q) \subset J$. Vậy chỉ cần chứng minh rằng $a \otimes \nu \otimes a \in I(Q)$. Điều này hiển nhiên nếu $\nu \in T^0$. Giả sử mệnh đề này đã được chứng minh với $\nu \in \sum_{h=0}^{n-1} T^h$, và lấy $x \in E$ và $u \in T^{n-1}$; ta có
$$
a \otimes x \otimes u \otimes a = (a + x) \otimes (a + x) \otimes u \otimes a
- a \otimes a \otimes u \otimes a - x \otimes a \otimes u \otimes a - x \otimes x \otimes u \otimes a
$$
và bốn hạng ở vế phải đều thuộc $I(Q)$.

Đặc biệt, giả sử môđun $E$ có một cơ sở $(x_i)_{i \in L}$, và sắp thứ tự toàn phần trên tập hợp các chỉ số $L$. Ta biết (Chương III, § 5, No. 6) rằng đại số ngoài của $E$ có một cơ sở là họ các phần tử $x_H$, trong đó $H$ chạy qua tập hợp các tập con hữu hạn của $L$ và trong đó $x_H$ là phần tử $x_{h_1} \wedge \ldots \wedge x_{h_q}$, $(h_1, \ldots, h_q)$ ký hiệu dãy tăng ngặt các phần tử của $H$.

Mặt khác, xét dạng song tuyến tính $F$ xác định bởi $F(x_i, x_j) = -\Phi(x_i, x_j)$ nếu $i > j$, $F(x_i, x_j) = 0$ nếu $i < j$ và $F(x_i, x_i) = -Q(x_i)$. Hiển nhiên là $Q(x) + F(x, x) = 0$; với các ký hiệu của Mệnh đề 3, từ mệnh đề này và Bổ đề 4 suy ra rằng $\bar{\lambda}_F$ là một đẳng cấu từ $\wedge E$ lên $C(Q)$, do đó $C(Q)$ là một A-môđun tự do. Bây giờ chứng minh, bằng quy nạp theo số phần tử của $H$, rằng ta có

$$
\bar{\lambda}_F(x_H) = \rho(x_{h_1}) \ldots \rho(x_{h_q})
$$

(trong đó $(h_1, \ldots, h_q)$ là dãy tăng ngặt các phần tử của $H$). Điều này hiển nhiên nếu $H$ có 0 hoặc 1 phần tử. Giả sử (11) đúng với các tập con có nhiều nhất $q - 1$ phần tử. Xét một tập con $H$ có $q$ phần tử, ký hiệu phần tử nhỏ nhất của nó là $j$, và viết $H = \{ j \} \cup K$, trong đó $K$ là một tập con có $q - 1$ phần tử. Theo (8) và giả thiết quy nạp, ta có

$$
\bar{\lambda}_F(x_H) = \bar{\lambda}_F(x_j \wedge x_K) = \rho(x_j) \bar{\lambda}_F(x_K) + i^F_{x_j}(\bar{\lambda}_F(x_K)) = x'_H + i^F_{x_j}(x'_K),
$$

đặt, với mọi tập con hữu hạn $J$ của $L$, $x'_J = \rho(x_{j_1}) \ldots \rho(x_{j_s})$, trong đó $(j_1, \ldots, j_s)$ là dãy tăng các phần tử của $J$. Bây giờ, với $i \in K$, $x_i$ thuộc hạt nhân của dạng tuyến tính $y \to F(x_j, y)$, nên $i^F_{x_j}(x'_K) = 0$ (Bổ đề 1). Điều này chứng minh kết quả cần chứng minh.

Vậy ta đã chứng minh định lý sau:

#### Định lý 1 {#alg-ix-s9-thm-1 .statement}

*Giả sử rằng $A$-môđun $E$ thừa nhận một cơ sở $(x_i)_{i \in L}$, tập hợp chỉ số $L$ được trang bị một thứ tự toàn phần. Với mọi tập con hữu hạn $H$ của $L$, đặt $x_H = \rho(x_{h_1}) \rho(x_{h_2}) \ldots \rho(x_{h_q})$, trong đó $(h_1, \ldots, h_q)$ là dãy tăng ngặt của các phần tử của $H$. Khi đó các phần tử $x_H$ tạo thành một cơ sở của $A$-môđun $C(Q)$.*

#### Hệ quả 1 {#alg-ix-s9-thm-1-cor-1 .statement}

*Nếu $E$ là một môđun tự do chiều $n$, thì $C(Q)$ là một môđun tự do chiều $2^n$; hơn nữa, nếu $n > 0$, thì $C^+$ và $C^-$ là các môđun tự do chiều $2^{n-1}$.

Điều này suy ra ngay từ các tính chất của các hệ số nhị thức.*

#### Hệ quả 2 {#alg-ix-s9-thm-1-cor-2 .statement}

*Nếu $E$ là một môđun tự do, thì ánh xạ chính tắc $\rho$ từ $E$ vào $C(Q)$ và ánh xạ $a \to a.1$ từ $A$ vào $C(Q)$ đều là đơn ánh.*

#### Hệ quả 3 {#alg-ix-s9-thm-1-cor-3 .statement}

*Giả sử rằng $E$ là tổng trực tiếp của hai môđun con tự do $E_1$ và $E_2$. Gọi $Q_i$ là hạn chế của $Q$ lên $E_i$ và $p_i$ là ánh xạ chính tắc từ $C(Q_i)$ vào $C(Q)$ ($i = 1, 2$). Khi đó ánh xạ tuyến tính $p$ từ $C(Q_1) \otimes C(Q_2)$ vào $C(Q)$ suy ra từ ánh xạ song tuyến tính $(a, b) \to p_1(a)p_2(b)$ từ $C(Q_1) \times C(Q_2)$ vào $C(Q)$ là một song ánh.

Thực vậy, chỉ cần xét cơ sở của $E$ thu được bằng cách lấy hợp của một cơ sở của $E_1$ và một cơ sở của $E_2$.*

#### Hệ quả 4 {#alg-ix-s9-thm-1-cor-4 .statement}

Các giả thiết và ký hiệu vẫn như trong Hệ quả 3, giả sử thêm rằng $E_1$ và $E_2$ trực giao, và chuyển cấu trúc đại số của $C(Q)$ lên $C(Q_1) \otimes C(Q_2)$ nhờ song ánh $p$. Nếu $a_i$ và $b_i$ là các phần tử chẵn hoặc lẻ của $C(Q_i)$ ($i = 1,\ 2$), thì $a\ (a_1 \otimes a_2)(b_1 \otimes b_2) = \varepsilon(a_1b_1) \otimes (a_2b_2)$, với $\varepsilon = 1$ trừ khi $a_2$ và $b_1$ là lẻ, trong trường hợp đó $\varepsilon = -1$.

Thật vậy, chỉ cần chứng minh rằng $p_2(a_2)p_1(b_1) = \varepsilon p_1(b_1)p_2(a_2)$, và vì mục đích đó ta có thể giả sử rằng $p_2(a_2)$ (resp. $p_1(b_1)$) là một tích $x_1 \ldots x_h$ (resp. $y_1 \ldots y_k$) của các phần tử của $\rho_Q(E_2)$ (resp. $\rho_Q(E_1)$). Vì $E_1$ và $E_2$ trực giao, ta có

$$
x_iy_j + y_jx_i = \Phi(x_i, y_j) = 0,
$$

do đó

$$
x_1 \ldots x_h y_1 \ldots y_k = (-1)^{hk} y_1 \ldots y_k x_1 \ldots x_h.
$$

Các kết luận của hệ quả 3 và 4 vẫn đúng nếu ta bỏ giả thiết rằng $E_1$ và $E_2$ là các môđun tự do (xem bài tập 1).

### 4. Cấu trúc của đại số Clifford.

Trong số này, ta sẽ giả sử rằng $A$ là một trường, rằng $E$ là một không gian vectơ hữu hạn chiều có chiều $m$ trên $A$, và rằng dạng toàn phương $Q$ là không suy biến (điều này, theo định lý 1 của § 5, no. 1, đòi hỏi $m$ phải chẵn nếu $A$ có đặc no. 2). Vì $E$ là tự do, ánh xạ chính tắc $\rho$ là đơn ánh (no. 3, hệ quả 2 của định lý 1). Từ đây về sau ta sẽ đồng nhất $E$ với ảnh của nó trong $C(Q)$.

#### Định lý 2 {#alg-ix-s9-thm-2 .statement}

Giả sử rằng chiều của $E$ là một số chẵn $m = 2r$ và rằng $Q$ là trung tính (§ 4, no. 2). Khi đó đại số $C(Q)$ là tách được (chương VIII, § 7, no. 5, định nghĩa 1) và đẳng cấu với đại số các tự đồng cấu của một không gian vectơ có chiều $2^r$ trên $A$. Hơn nữa, nếu $m > 0$, thì $C^+(Q)$ là tách được và là tổng trực tiếp của hai ideal đẳng cấu với đại số các tự đồng cấu của một không gian vectơ có chiều $2^{r-1}$ trên $A$.

Thật vậy, vì Q là trung tính, E có thể được phân tích thành tổng trực tiếp của hai không gian con hoàn toàn kỳ dị N và P có chiều r (§ 4, no. 2, hệ quả 1 của mệnh đề 2). Hạn chế của Q lên N bằng không, nên đại số con S của C(Q) sinh bởi N được đồng nhất với đại số ngoại của N (no. 3, bổ đề 4). Với $n \in \mathbf{N}$, ta sẽ ký hiệu bởi $e'_n$ ánh xạ $t \to nt$ từ S vào chính nó.

Gọi $(n_1, \ldots, n_r)$ là một cơ sở của N; ta sẽ ký hiệu bởi $(p_1, \ldots, p_r)$ cơ sở của P sao cho $\Phi(n_i, p_j) = \delta_{ij}$ (§ 4, no. 2, mệnh đề 2). Với $p \in P$, ta sẽ ký hiệu bởi $p'$ dạng tuyến tính $n \to \Phi(n, p)$ trên N, và bởi $i_p$ tự đồng cấu của S thu được bằng cách chuyển qua thương từ tự đồng cấu $i_{p'}$ của $T(N)$ liên kết với $p'$ như đã nói trong bổ đề 1 của no. 2. Theo (5), ta có

$$
e'_n \circ i_p + i_p \circ e'_n = \Phi(n, p) \qquad (n \in \mathbf{N}, \ p \in \mathbf{P}).
$$

Đặt, với $x = n + p \in E$ (với $n \in \mathbf{N}$ và $p \in \mathbf{P}$), $s(x) = e'_n + i_p$. Hiển nhiên s là một ánh xạ tuyến tính từ E vào $\mathcal{L}(S)$. Vì ta có
$$
s(x)^2 = (e'_n + i_p)^2 = Q(n) + \Phi(n, p) = Q(x)
$$
theo (12) và bổ đề 1 (số 2), s mở rộng thành một đồng cấu (mà ta vẫn sẽ ký hiệu là s) từ C(Q) vào $\mathcal{L}(S)$ (no. 1, mệnh đề 1). Bây giờ ta chứng minh rằng đồng cấu này là toàn ánh; điều này, vì C(Q) và $\mathcal{L}(S)$ đều có chiều $2^{2r}$, sẽ suy ra rằng s là một đẳng cấu và sẽ chứng minh mệnh đề thứ nhất của ta.

Thật vậy, gọi $I$ là khoảng $[1, r]$. Với mọi tập con H của I, đặt $H' = I - H$ và ký hiệu bởi $n_H$ (tương ứng $p_H$) tích của các $n_i$ (tương ứng $p_i$) với $i \in H$, được sắp theo thứ tự tăng của các chỉ số. Nhớ rằng các $n_H$ tạo thành một cơ sở của S (No. 3, Định lý 1). Cuối cùng, với mọi hai tập con H, K của I, đặt $x_{H, K} = n_H p_I n_K$. Bây giờ chúng ta sẽ chứng minh rằng các phần tử $s(x_{H, K})$ của $s(C(Q))$ sinh ra $\mathcal{L}(S)$. Thật vậy, nếu $j \notin H$, ta có $s(p_j)(n_H) = i_{p_j}(n_H) = 0$ theo Bổ đề 1, vì các $n_i$ với $i \in H$ thuộc hạt nhân của dạng tuyến tính $n \to \Phi(n, p_j)$ trên N; mặt khác, ta có
$$
s(p_j)(n_j n_H) = (i_{p_j} \circ e'_{n_j})(n_H) = \Phi(p_j, n_j)n_H - n_j \cdot s(p_j)(n_H) = n_H
$$
(theo (12)). Vì s là một đồng cấu, do đó suy ra rằng, với mọi hai tập con H, K của I, $s(p_K)(n_H) = 0$ nếu $K \not\subset H$, và $s(p_K)(n_H) = \pm n_{H-K}$ nếu $K \subset H$. Vì, với $M \subset I$ và $L \subset I$, theo định nghĩa $s(n_M)(n_L) = n_M n_L$, và $n_M n_L$ bằng không nếu $M \cap L \neq \emptyset$ và bằng $\pm n_{M \cup L}$ trong trường hợp ngược lại, nên từ điều trên suy ra rằng, với mọi tập con $H, K, L$ của $I$, $s(x_{H,K})(n_L) = s(n_H)s(p_I)s(n_{K'}) (n_L)$ bằng không nếu $K \neq L$ và bằng $\pm n_H$ nếu $K = L$. Điều này cho thấy rằng các $s(x_{H,K})$ sinh ra $\mathcal{L}(S)$ và hoàn tất chứng minh của mệnh đề thứ nhất.

Để chứng minh mệnh đề thứ hai, đặt $S^+ = S \cap C^+$ và $S^- = S \cap C^-$; hiển nhiên $S^+$ (tương ứng $S^-$) là không gian con của S được sinh bởi các $n_H$ sao cho H có một số chẵn (tương ứng lẻ) phần tử, rằng S là tổng trực tiếp của $S^+$ và $S^-$, và rằng $s(C^+)$ giữ cho $S^+$ và $S^-$ ổn định. Do đó $s$ ánh xạ $C^+$ vào một đại số con của $\mathcal{L}(S)$, đẳng cấu với tích $\mathcal{L}(S^+) \times \mathcal{L}(S^-)$; hạn chế của $s$ lên $C^+$ là một đẳng cấu từ $C^+$ lên đại số con này, vì $s$ là đơn ánh và $C^+$ và $\mathcal{L}(S^+) \times \mathcal{L}(S^-)$ đều có chiều $2^{2r-1}$ (No. 2, Hệ quả 1 của Định lý 1). QED.

#### Hệ quả {#alg-ix-s9-n4-cor-1 .statement}

*Nếu $m$ chẵn, nhưng $Q$ có chỉ số tùy ý, thì đại số $C(Q)$ là một đại số đơn tâm có chiều $2^m$. Hơn nữa, nếu $m > 0$, đại số con $C^+(Q)$ là tách được, và tâm Z của nó có chiều 2 trên A. Khi Z là một trường, Z là một mở rộng bậc hai tách được của A và $C^+(Q)$ là đơn; nếu không, Z là tích trực tiếp của hai trường đẳng cấu với A, và khi đó $C^+(Q)$ là tích trực tiếp của hai đại số con đơn có chiều $2^{m-2}$.

Thật vậy, gọi $A'$ là bao đóng đại số của A, và $Q'$ là dạng toàn phương trên $E' = A' \otimes_A E$ suy ra từ Q bằng mở rộng vô hướng. Ta đã thấy rằng $C(Q')$ đẳng cấu với $A' \otimes_A C(Q)$ (mệnh đề 2), và hiển nhiên $C^+(Q')$ đẳng cấu với $A' \otimes_A C^+(Q)$. Vì $Q'$ là trung tính ($§ 4$, No. 2, Hệ quả 2 của mệnh đề 3), hệ quả là một hệ quả ngay lập tức của Định lý 2 và các định lý bảo toàn của Chương VIII, $§ 7$.

#### Nhận xét 1 {#alg-ix-s9-n4-rem-1 .statement}

Vì đại số $C(Q)$ là đơn, nó chỉ có một lớp các biểu diễn bất khả quy; chúng được gọi là *các biểu diễn spinor*; khi ta cố định sự chú ý vào một biểu diễn trong số đó, chẳng hạn $\tau$, thì các phần tử của không gian mà trên đó $\tau$ được thực hiện được gọi là *spinor*. Nếu Q trung tính, hạn chế của $\tau$ lên $C^+(Q)$, cũng như hạn chế của $s$, là tổng của hai biểu diễn tuyệt đối bất khả quy không tương đương; các phần tử của các không gian con mà trên đó hai biểu diễn này được thực hiện được gọi là các semispinor. Trong trường hợp tổng quát, nếu $C^+(Q)$ không đơn, thì hạn chế của $\tau$ lên $C^+(Q)$, do nó trung thành, phải chứa các biểu diễn con thuộc mỗi một trong hai lớp biểu diễn bất khả quy của $C^+(Q)$, và do đó là tổng của hai biểu diễn tuyệt đối bất khả quy không tương đương, vì điều này đúng sau khi mở rộng vô hướng tới bao đóng đại số $A'$ của $A$. Mặt khác, nếu $C^+(Q)$ đơn, thì nó chỉ có một lớp biểu diễn bất khả quy, và vì thế hạn chế của $\tau$ lên $C^+(Q)$ là bất khả quy, vì nó phân tích, bằng mở rộng vô hướng tới $A'$, thành hai biểu diễn không tương đương.

#### Nhận xét 2 {#alg-ix-s9-n4-rem-2 .statement}

Giả sử rằng $A$ có đặc số $\neq 2$, và gọi $(x_1, \ldots, x_m)$ ($m = 2r$) là một cơ sở trực giao của $E$. Đặt
$$
z = 2^r x_1 \ldots x_m \in C(Q);
$$
vì $x_i x_j + x_j x_i = 0$ với $i \neq j$, ta có $zx_j = -x_j z$, kéo theo z thuộc tâm $Z$ của $C^+(Q)$ mà không thuộc $A$. Ta có
$$
z^2 = 2^{2r}(-1)^r Q(x_1) \ldots Q(x_m) = (-1)^r D
$$
trong đó D ký hiệu biệt thức của $\Phi$ đối với cơ sở $(x_j)$ (xem bài tập 9).

#### Định lý 3 {#alg-ix-s9-thm-3 .statement}

*Giả sử rằng chiều của $E$ là một số lẻ $m = 2r + 1$ (và do đó $A$ có đặc số $\neq 2$).*

a) *Đại số $C^+(Q)$ là đơn tâm. Nếu Q có chỉ số cực đại $r$, thì $C^+(Q)$ đẳng cấu với đại số tự đồng cấu của một không gian vectơ có chiều $2^r$ trên $A$.*

b) *Đại số $C(Q)$ là tách được. Tâm của nó $Z$ có chiều bằng 2, và $C(Q)$ đẳng cấu với $Z \otimes_A C^+(Q)$, và do đó là đơn hoặc là tổng trực tiếp của hai đại số con đơn.*

Cho $x_0$ là một vectơ không đẳng hướng của $E$, và gọi $F$ là trực giao của $x_0$; ký hiệu bởi $Q_1$ dạng toàn phương $y \to -Q(x_0)Q(y)$ trên $F$; hiển nhiên $Q_1$ là không suy biến. Vì $x_0 y = -y x_0$ (với $y \in F$), ta có $(x_0 y)^2 = -Q(x_0)Q(y) = Q_1(y)$, và do đó ánh xạ $y \to x_0 y$ từ $F$ vào $C^+(Q)$ kéo dài thành một đồng cấu $h$ từ $C(Q_1)$ vào $C^+(Q)$ (No. 1, Prop. 1). Khi đó $C(Q_1)$ là đơn (Th. 2) và có cùng chiều $2^{2r}$ như $C^+(Q)$; điều này suy ra, vì $h(1) = 1$, rằng $h$ là một đẳng cấu. Hơn nữa, nếu $Q$ có chỉ số $r$, thì có thể chọn $x_0$ sao cho $Q_1$ cũng có chỉ số $r$ (§ 4, No. 2, Prop. 3), điều này chứng minh $a$.

Bây giờ lấy $(x_1, \ldots, x_{2r})$ là một cơ sở trực giao của $F$; đặt $z = x_0 x_1 \ldots x_{2r}$. Người ta kiểm tra ngay lập tức rằng $z$ giao hoán với $x_j$ với $j = 0, \ldots, 2r$, và do đó thuộc tâm của $C(Q)$. Gọi $Z$ là không gian con của $C(Q)$ được sinh bởi $1$ và $z$; đó là một đại số con của tâm của $C(Q)$ và là một mở rộng bậc hai của $A$, vì $z$ là lẻ và $z^2$ bằng vô hướng $(-1)^r Q(x_0) \ldots Q(x_{2r})$. Xét đồng cấu $\theta$ từ $Z \otimes_A C^+(Q)$ vào $C(Q)$ được xác định bởi $\theta(u \otimes v) = uv$. Vì $z \in C^-$ và khả nghịch, ánh xạ $u \to zu$ là một đẳng cấu của môđun $C^+$ lên $C^-$, điều này kéo theo rằng $\theta(Z \otimes C^+)$ chứa $C^+$ và $C^-$, và do đó trùng với $C(Q)$. Vì $Z \otimes C^+$ và $C(Q)$ có cùng chiều $2^{2r+1}$, nên $\theta$ là một đẳng cấu; điều này chứng minh $b$, xét theo các kết quả của Chương VIII, § 7.

#### Nhận xét {#alg-ix-s9-n4-rem-3 .statement}

Biệt thức $D$ của $\Phi$ đối với cơ sở $(x_j)_{(j=0,\ldots,2r)}$ bằng $2^{2r+1} Q(x_0) \ldots Q(x_{2r})$. Do đó $Z$ được sinh bởi $1$ và bởi phần tử lẻ $z' = 2^{r+1} z$ sao cho ${z'}^2 = (-1)^r 2D$. Vì vậy đại số $C(Q)$ là đơn khi và chỉ khi $2(-1)^r D$ không là một bình phương trong $A$.

### 5. Nhóm Clifford.

Trong số này, ta giả sử rằng $A$ là một trường, rằng $E$ có số chiều hữu hạn $m$, và rằng $Q$ không suy biến. Ta đồng nhất $E$ với ảnh chính tắc của nó trong $C(Q)$.

#### Định nghĩa 2 {#alg-ix-s9-def-2 .statement}

Nhóm Clifford của $Q$ (tương ứng, nhóm Clifford đặc biệt của $Q$) được gọi là nhóm nhân của các phần tử khả nghịch $s$ của $C(Q)$ (tương ứng, $C^+(Q)$) sao cho $sEs^{-1} = E$.

Trong số này ta sẽ ký hiệu bởi $G$ và $G^+$ nhóm Clifford và nhóm Clifford đặc biệt của $Q$. Hiển nhiên là $G^+ = G \cap C^+(Q)$.

#### Định lý 4 {#alg-ix-s9-thm-4 .statement}

Đặt, với $s \in G$ và $x \in E$, $\varphi(s).x = sx s^{-1}$.

a) Ánh xạ $\varphi$ là một đồng cấu của $G$ vào nhóm trực giao $O(Q)$ của $Q$ và hạt nhân của nó là tập hợp các phần tử khả nghịch của tâm $Z$ của $C(Q)$.

b) Tập hợp $E \cap G$ là tập hợp các vectơ không suy biến của $E$; với $x \in E \cap G$, $-\varphi(x)$ là phép đối xứng đối với siêu phẳng trực giao với $x$.

c) Nếu $\dim(E)$ là chẵn, ta có $\varphi(G) = O(Q)$, $\varphi(G^+)$ có chỉ số 2 trong $O(Q)$ nếu $E \neq \{0\}$, và bằng $SO(Q)$ nếu $A$ có đặc số $\neq 2$.

d) Nếu $\dim(E)$ là lẻ (điều này kéo theo rằng $A$ có đặc số $\neq 2$), ta có $\varphi(G) = \varphi(G^+) = SO(Q)$.

Thật vậy, ta có $Q(sxs^{-1}) = (sxs^{-1})^2 = sx^2 s^{-1} = Q(x)$ với $s \in G$ và $x \in E$, điều này cho thấy rằng $\varphi(s) \in O(Q)$. Để $\varphi(s) = 1$ đúng, điều kiện cần và đủ là $s$ giao hoán với các phần tử của $E$, nghĩa là, thuộc tâm $Z$ của $C(Q)$. Điều này chứng minh a).

Để một phần tử $x$ của $E$ thuộc $G$, điều cần thiết là nó khả nghịch, nghĩa là, nó là một vectơ không suy biến (vì $x^2 = Q(x)$). Nếu đúng như vậy, ta có $x^{-1} = Q(x)^{-1} x$, do đó, với mọi $y \in E$,
$$ xy x^{-1} = Q(x)^{-1} xy x = Q(x)^{-1} x (\Phi(x, y) - xy) = - (y - \Phi(x, y) Q(x)^{-1} x); $$
điều này chứng minh b) (§ 6, số 4).

#### Bổ đề 5 {#alg-ix-s9-lem-5 .statement}

Mọi phần tử $s$ của $G$ đều có dạng $zs'$, trong đó $z$ là một phần tử khả nghịch của $Z$ và $s'$ thuộc $G \cap C^+(Q)$ hoặc thuộc $G \cap C^-(Q)$; nhóm con $G^+$ có chỉ số 2 trong $G$ khi $E \neq \{0\}$.

Mệnh đề thứ hai hiển nhiên suy ra từ mệnh đề thứ nhất, vì các vectơ không suy biến thuộc $G \cap C^-(Q)$. Trước hết giả sử $\dim(E)$ là chẵn, và đặt $s = t' + t''$, với $t' \in C^+(Q)$ và $t'' \in C^-(Q)$; theo định nghĩa ta có $sx = (\varphi(s).x)s$ với mọi $x \in E$; vì $t'x$ và $(\varphi(s).x)t'$ (tương ứng, $t''x$ và $(\varphi(s).x)t''$) là các phần tử lẻ (tương ứng, chẵn), nên ta có $t'x = (\varphi(s).x)t'$, do đó $s^{-1} t' x = xs^{-1} t'$ với mọi $x \in E$. Suy ra $s^{-1} t' \in Z$ và, vì $\dim(E)$ là chẵn, $Z = A$ (No. 4, hệ quả của Định lý 2), do đó $t' = as$, với $a \in A$. Nếu $a \neq 0$, ta do đó có $s = a^{-1} t'$ và $t' \in G \cap C^+(Q)$; nếu $a = 0$, thì $s = t'' \in G \cap C^-(Q)$ và bổ đề được chứng minh trong trường hợp này. Nếu $\dim(E)$ là lẻ, $A$ có đặc số $\neq 2$, nên với mọi $s \in G$, $\varphi(s)$ là một tích các đối xứng đối với các vectơ không suy biến $x_i (i = 1, 2, \ldots, h)$ (§ 6, No. 4, Mệnh đề 5); nếu ta đặt $s' = x_1 x_2 \ldots x_h$, thì ta có $\varphi(s) = \varphi(s')$, do đó $s = z s'$, với $z \in \mathbf{Z}$, và $s'$ thuộc $C^+(Q)$ hoặc $C^-(Q)$ tùy theo $h$ là chẵn hay lẻ.

Giả sử $\dim(E)$ là chẵn. Vì mọi phần tử $u$ của $\mathbf{O}(Q)$ mở rộng được theo một và chỉ một cách thành một tự đẳng cấu $\bar{u}$ của $C(Q)$ (Mệnh đề 1), và vì $C(Q)$ là đơn tâm (Định lý 2), nên $\bar{u}$ là một tự đẳng cấu trong (Chương VIII, § 10, No. 1, Định lý 1). Vậy tồn tại một phần tử $s$ của $G$ sao cho $\varphi(s) = u$. Mặt khác, tâm của $C(Q)$ được chứa trong $C^+$, điều này kéo theo $\varphi(G)/\varphi(G^+)$ đẳng cấu với $G/G^+$, nên $\varphi(G^+)$ có chỉ số 2 trong $\varphi(G) = \mathbf{O}(Q)$ nếu $E \not= \{0\}$. Điều này chứng minh hai mệnh đề đầu của c).

Giả sử cuối cùng rằng $A$ có đặc số $\not= 2$. Khi đó mọi phần tử $u$ của $\mathbf{O}(Q)$ là một tích các đối xứng qua các siêu phẳng trực giao với các vectơ không suy biến $x_i (i = 1, \ldots, h)$ (§ 6, n° 4, mệnh đề 5); do đó ta có $u = (-1)^h \varphi(x_1 \ldots x_h)$ và $\det(u) = (-1)^h$. Để $u$ thuộc $\mathbf{SO}(Q)$, điều kiện cần và đủ là $h$ chẵn, điều đó cho thấy $\varphi(G^+) \supset \mathbf{SO}(Q)$. Vì $\mathbf{SO}(Q)$ có chỉ số 2 trong $\mathbf{O}(Q)$ khi $E \not= \{0\}$, nên ta có $\varphi(G^+) = \mathbf{SO}(Q)$ nếu $E$ có chiều *chẵn*, điều này hoàn tất chứng minh của c). Mặt khác, nếu chiều của $E$ là *lẻ*, thì $\varphi(G)$ không chứa phép biến đổi trực giao $x \to -x$; thật vậy, phép này mở rộng thành tự đẳng cấu chính $\alpha$ của $C(Q)$ (n° 1), và $\alpha$ không phải là một tự đẳng cấu trong vì tâm $Z$ của $C(Q)$ chứa một phần tử khác không của $C^-(Q)$ (định lý 3). Vậy $\varphi(G) \not= \mathbf{O}(Q)$, và, vì $\varphi(G) \supset \varphi(G^+) \supset \mathbf{SO}(Q)$ và $\mathbf{SO}(Q)$ có chỉ số 2 trong $\mathbf{O}(Q)$, ta có $\varphi(G) = \varphi(G^+) = \mathbf{SO}(Q)$. Điều này chứng minh d). Q.E.D.

Nhóm con $\varphi(G^+)$ của $\mathbf{O}(Q)$, có chỉ số 2 nếu $E \not= \{0\}$, được gọi là *nhóm các phép quay* của $E$, và các phần tử của nó được gọi là *các phép quay*; nó được ký hiệu bởi $\mathbf{O}^+(Q)$. Chú ý rằng, nếu $A$ không có đặc số 2, thì ta có $\mathbf{O}^+(Q) = \mathbf{SO}(Q)$ (x. bài tập 9).

#### Mệnh đề 4 {#alg-ix-s9-prop-4 .statement}

*Cho $\beta$ là phản tự đẳng cấu chính của $C(Q)$ (n° 1). Với mọi $s \in G^+$, $\beta(s)s$ là một vô hướng. Ánh xạ $N : s \to \beta(s)s$ là một đồng cấu từ $G^+$ vào nhóm nhân $A^*$ của các phần tử khác không của $A$.*

Thật vậy, với $s \in G^+$, ta có $sEs^{-1} = E$, do đó $\beta(s)^{-1}E\beta(s) = E$, điều này cho thấy rằng $\beta(s) \in G^+$. Vì $sx = (\varphi(s).x)s$ với mọi $x \in E$, ta có $x\beta(s) = \beta(sx) = \beta(s)(\varphi(s).x)$, và do đó $\beta(s)sx = \beta(s)(\varphi(s).x)s = x\beta(s)s$, điều này suy ra rằng $\beta(s)s$ thuộc tâm của $C(Q)$. Hơn nữa, vì $\beta(s)s$ thuộc $C^+(Q)$, nên $\beta(s)s$ là một vô hướng (Định lý 2 và 3). Cuối cùng ta có $\beta(st)st = \beta(t)\beta(s)st = \beta(s)s\beta(t)t$, tức là $N(st) = N(s)N(t)$ với $s, t$ trong $G^+$. QED.

Vô hướng $N(s) = \beta(s)s$ ($s \in G^+$) được gọi là chuẩn spinor của $s$. Ta ký hiệu bởi $G_0^+$ và gọi là nhóm Clifford thu gọn hạt nhân của đồng cấu $N$. Ảnh $\varphi(G_0^+)$ được ký hiệu bởi $O_0^+(Q)$ và được gọi là nhóm trực giao thu gọn của $Q$. Vì hạt nhân của hạn chế của $\varphi$ lên $G^+$ là tập hợp các phần tử chẵn và khả nghịch của tâm của $C(Q)$ (Định lý 4) và do đó được đồng nhất với $A^*$ (Định lý 2 và 3), $\varphi(G^+)/O_0^+(Q)$ đẳng cấu với $G^+/A^*G_0^+$, và vì thế cũng đẳng cấu với $N(G^+)/N(A^*)$, và đặc biệt là giao hoán. Rõ ràng $N(A^*)$ là nhóm con $(A^*)^2$ gồm các bình phương của các phần tử của $A^*$. Nếu $Q$ có chỉ số $> 0$, thì với mọi $a \in A^*$, tồn tại hai phần tử $x$ và $y$ của $E$ sao cho $Q(x) = a$ và $Q(y) = 1$ (§ 4, No. 2, Mệnh đề 4) ; vì $xy \in G^+$ và $N(xy) = Q(x)Q(y) = a$, điều này cho thấy rằng $N(G^+) = A^*$, và do đó $\varphi(G^+)/O_0^+(Q)$ đẳng cấu với $A^*/(A^*)^2$.

Bài tập. — ¶ 1) Chứng minh Hệ quả 3 và 4 của Định lý 1 của No. 3 khi $E_1$ và $E_2$ là hai môđun con bù nhau bất kỳ trong $E$. (Trước hết thiết lập Hệ quả 4: bây giờ chứng minh với mục đích đó rằng tích tenxơ $C(Q_1) \otimes C(Q_2)$ được trang bị một cấu trúc đại số bởi quy ước dấu đã nêu trong mệnh đề của Hệ quả 4, và rằng đại số này $S$ là nghiệm của cùng bài toán ánh xạ phổ quát như $C(Q)$; với mục đích đó, hãy xét, với mọi ánh xạ tuyến tính $f$ của $E$ vào một đại số $D$ trên $A$ sao cho $(f(x))^2 = Q(x).1$, đồng cấu $\bar{f}_i$ của $C(Q_i)$ vào $D$ sao cho $\bar{f}_i(1) = 1$, $\bar{f}_i(\rho_{Q_i}(x_i)) = f(x_i)$ với $x_i \in E_i$ ($i = 1, 2$) và hãy chứng minh rằng tồn tại một đồng cấu $\bar{f}$ của đại số $S$ vào $D$ sao cho
$$
\bar{f}(z_1 \otimes z_2) = \bar{f}_1(z_1)\bar{f}_2(z_2)
$$
với $z_i \in C(Q_i)$ ($i = 1, 2$). Sau đó để chứng minh Hệ quả 3, hãy xét dạng toàn phương $Q'$ là tổng trực tiếp ngoài của $Q_1$ và $Q_2$ (§ 3, No. 4), và nhận xét rằng ta có $Q'(x) = Q(x) + F(x, x)$, trong đó $F$ là dạng song tuyến tính được xác định bởi $F(x_1 + x_2, y_1 + y_2) = -\Phi(x_1, y_2)$ với $x_i, y_i$ trong $E_i$ ($i = 1, 2$) ; sau đó dùng Mệnh đề 3.)

¶ 2) Giả sử rằng $E$ là tổng trực tiếp của hai môđun con trực giao $E_1, E_2$ và ký hiệu bởi $Q_i$ hạn chế của $Q$ trên $E_i$ ($i = 1, 2$);

giả sử thêm rằng tồn tại $u \in C^+(Q_2)$ sao cho $u^2 = a . 1$, với $a$ khả nghịch trong $A$, và rằng $u \rho_{Q_2}(x_2) = -\rho_{Q_2}(x_2)$ với mọi $x_2 \in E_2$. Bây giờ chứng minh rằng tồn tại một đẳng cấu $\varphi$ từ $C(Q)$ lên tích tensor $C(aQ_1) \otimes C(Q_2)$ (như được định nghĩa trong chap. III, § 3, n° 1), có tính chất là với mọi $x = x_1 + x_2$ ($x_i \in E_i, i = 1, 2$), ta có
$$
\varphi(\rho_Q(x)) = \rho_{aQ_1}(x_1) \otimes u^{-1} + 1 \otimes \rho_{Q_2}(x_2).
$$
(Chứng minh sự tồn tại của đồng cấu $\varphi$ như một hệ quả của tính chất phổ quát của $C(Q)$. Mặt khác, có một đồng cấu $g_1$ từ $C(aQ_1)$ vào $C(Q)$ sao cho $g_1(\rho_{aQ_1}(x_1)) = h_2(u)\rho_{Q_1}(x_1)$, trong đó $h_2$ ký hiệu đồng cấu chính tắc từ $C(Q_2)$ vào $C(Q)$; khi đó nhận xét rằng $g_1(z_1)$ và $h_2(z_2)$ giao hoán với $z_1 \in C(aQ_1)$ và $z_2 \in C(Q_2)$, và suy ra sự tồn tại của một đồng cấu nghịch đảo của $\varphi$.)

Kết quả này áp dụng trong trường hợp nào khi $A$ là một trường có đặc số $\neq 2$ (dùng Nhận xét 2 sau Hệ quả của Định lý 2)?

3) a) Với ký hiệu của No. 2, cho $x_i$ ($1 \leqslant i \leqslant n$) là các phần tử của $E$ sao cho $f(x_i) = 0$; chứng minh rằng ta có $i_f(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = 0$. Đặc biệt, nếu $F$ là một dạng song tuyến tính trên $E$ sao cho $F(x_i, x_j) = 0$ với $i > j$, ta có $i_F^E(x_2 \otimes x_3 \otimes \cdots \otimes x_n) = 0$.

b) Với ký hiệu của Mệnh đề 3 ở No. 3, cho $x_i$ ($1 \leqslant i \leqslant n$) là các phần tử của $E$ sao cho $F(x_i, x_j) = 0$ với $i > j$. Chứng minh rằng ta có $\overline{\lambda}_F(\rho_{Q'}(x_1) \ldots \rho_{Q'}(x_n)) = \rho_Q(x_1) \ldots \rho_Q(x_n)$ (dùng a) và công thức (10) của No. 2).

c) Giả sử rằng $A$ là một trường có đặc số $\neq 2$; với mọi dạng toàn phương $Q$ trên $E$, gọi $\mu_Q$ là ánh xạ $\overline{\lambda}_F$ từ $C(Q)$ lên $\wedge E$ tương ứng với $F(x, y) = \frac{1}{2} \Phi(x, y)$. Bây giờ chứng minh rằng nếu các vectơ $x_i$ ($1 \leqslant i \leqslant n$) trực giao từng đôi một, ta có
$$
\mu_Q(x_1 x_2 \ldots x_n) = x_1 \wedge x_2 \wedge \ldots \wedge x_n.
$$
Suy ra rằng nếu $y_i$ ($1 \leqslant i \leqslant n$) là $n$ vectơ tùy ý, ta có
$$
n! \; \mu_Q^{-1}(y_1 \wedge y_2 \wedge \ldots \wedge y_n) = \sum_{\sigma \in S_n} \varepsilon_\sigma y_{\sigma(1)} y_{\sigma(2)} \cdots y_{\sigma(n)}.
$$

4) Gọi $C_h$ là môđun con của $C(Q)$ sinh bởi các tích của $k$ phần tử của $\rho_Q(E)$ với $0 \leqslant k \leqslant h$. Hãy chỉ ra rằng ánh xạ
$$
(x_1, \ldots, x_h) \to \rho_Q(x_1) \ldots \rho_Q(x_h)
$$
xác định, sau khi chuyển qua các thương, một ánh xạ đa tuyến tính phản xứng từ $E^h$ vào $C_h/C_{h-1}$. Từ đó suy ra một ánh xạ tuyến tính $\pi_h$ từ $\wedge^h E$ vào $C_h/C_{h-1}$; hãy chứng minh rằng $\pi_h$ là một đẳng cấu khi $E$ là một môđun tự do. Nếu $f$ là một biến đổi trực giao, ta có $C(f) \circ \pi_h = \pi_h \circ (\wedge^h f)$. Khi $A$ là một trường có đặc số $\neq 2$, hãy chỉ ra rằng $\pi_h$ là hạn chế của ánh xạ nghịch đảo $\mu_Q^{-1}$ được định nghĩa trong bài tập 3 c).

5) Với ký hiệu của No. 2, xét ánh xạ $i_f$ từ $\wedge E$ vào chính nó. Hãy chỉ ra rằng ta có

$$
i_f(x_1 \wedge \ldots \wedge x_h) = \sum_{i=1}^{h} (-1)^{i-1} f(x_i) (x_1 \wedge \ldots \wedge x_{i-1} \wedge x_{i+1} \wedge \ldots \wedge x_h)
$$

và suy ra rằng $i_f$ không là gì khác ngoài tích trong bên phải $z \to z \llcorner f$ (chap. III, § 8, No. 4, định nghĩa 2).

6) Hãy chỉ ra rằng, nếu $E$ thừa nhận một cơ sở trực giao $(e_1, e_2)$ đối với Q, và nếu đặt $\alpha_i = Q(e_i)$ ($i = 1, 2$), thì đại số $C(Q)$ đẳng cấu với đại số quaternion trên $A$ tương ứng với cặp $(\alpha_1, \alpha_2)$.

7) Gọi $A$ là một trường có thứ tự cực đại, $E$ một không gian vectơ có chiều chẵn $2r$ trên $A$, và $Q$ một dạng toàn phương không suy biến trên $E$, dương hoặc âm. Hãy chỉ ra rằng, nếu $Q$ dương, thì $C(Q)$ đẳng cấu với một đại số ma trận trên $A$ khi $r(r-1)/2$ chẵn, và với một đại số ma trận trên đại số quaternion trên $A$ khi $r(r-1)/2$ lẻ. Nếu $Q$ âm, thì $C(Q)$ đẳng cấu với một đại số ma trận trên $A$ khi $r(r+1)/2$ chẵn, và với một đại số ma trận trên đại số quaternion trên $A$ khi $r(r+1)/2$ lẻ (dùng bài tập 2 và 6). Cấu trúc của $C^+(Q)$ trong các trường hợp khác nhau ấy là gì?

8) Cho $A$ là vành $\mathbf{Z}/(4)$, $E$ là $A$-môđun $\mathbf{Z}/(2)$; nếu đặt Q(0) = 0, Q(u) = 1 với phần tử duy nhất $u \neq 0$ của $E$, thì $Q$ là một dạng toàn phương trên $E$. Chứng minh rằng các $A$-môđun $C(Q)$ và $\wedge E$ không đẳng cấu (sẽ được chứng minh rằng $C(Q)$ đẳng cấu với tổng trực tiếp của hai môđun đẳng cấu với E).

¶ 9) Giả sử rằng $A$ là một trường có đặc số 2, $E$ là một không gian vectơ có số chiều hữu hạn $2r$, $Q$ là một dạng toàn phương không suy biến trên $E$.

a) Cho $(e_i)$ là một cơ sở symplectic ($§ 5,$ No. 1) của $E$ đối với dạng song tuyến tính phản xứng $\Phi$ liên kết với Q. Chứng minh rằng phần tử

$$
z = e_1 e_2 + e_3 e_4 + \cdots + e_{2r-1} e_{2r}
$$

của $C^+(Q)$ cùng với phần tử đơn vị tạo thành một cơ sở của tâm Z của $C^+(Q)$. Để Z là tổng trực tiếp của hai trường, điều kiện cần và đủ là phần tử

$$
\Delta(Q) = Q(e_1) Q(e_2) + Q(e_3) Q(e_4) + \cdots + Q(e_{2r-1}) Q(e_{2r})
$$

(được gọi là *giả biệt thức* của Q đối với cơ sở symplectic $(e_i)$) có dạng $\lambda^2 + \lambda$, với $\lambda \in A$.

b) Cho $u$ là một phép đồng dạng của $\Phi$ ($§ 6,$ No. 5) với nhân tử $\mu(u)$, và đặt $Q_1(x) = Q(u(x))$. Đặt

$$
u(e_{2i-1}) = \sum_{j=1}^{r} a_{ij} e_{2j-1} + \sum_{j=1}^{r} b_{ij} e_{2j},
$$
$$
u(e_{2i}) = \sum_{j=1}^{r} c_{ij} e_{2j-1} + \sum_{j=1}^{r} d_{ij} e_{2j},
$$

và $Q(e_{2i-1}) = \alpha_i, Q(e_{2i}) = \beta_i$ ($1 \leq i \leq r$). Bây giờ chứng minh rằng
$$
\Delta(Q_1) = (\mu(u))^2 \Delta(Q) + (\mathrm{D}(u))^2 + \mu(u)\mathrm{D}(u)
$$
trong đó
$$
\mathrm{D}(u) = \sum_{i,j} (\alpha_j a_{ij} c_{ij} + \beta_j b_{ij} d_{ij} + b_{ij} c_{ij})
$$
(bất biến Dickson của $u$ đối với cơ sở $(e_i)$). (Hãy để ý rằng phần tử
$$
(\mu(u))^{-1}(u(e_1)u(e_2) + u(e_3)u(e_4) + \cdots + u(e_{2r-1})u(e_{2r}))
$$
thuộc $\mathbf{Z}$.) Để $u$ là một phép đồng dạng của $Q$ ($§ 4$, Exercise 9) với nhân tử $\mu(u)$, điều kiện cần và đủ là $\mathrm{D}(u) = 0$ hoặc $\mathrm{D}(u) = \mu(u)$; các phép đồng dạng của $Q$ sao cho $\mathrm{D}(u) = 0$ được gọi là trực tiếp.

c) Bây giờ chứng minh rằng, nếu $\varphi$ là một phép đồng dạng đối với $\Phi$, $u$ là một phép đồng dạng đối với $Q$, thì ta có
$$
\mathrm{D}(u\varphi) = \mu(\varphi)\mathrm{D}(u) + \mu(u)\mathrm{D}(\varphi)
$$
(xét bất biến Dickson của $\varphi$ đối với cơ sở đối xứng tạo bởi các $u(e_{2i-1})$ và $(\mu(u))^{-1}u(e_{2i})$ với $1 \leq i \leq r$). Suy ra rằng các phép đồng dạng trực đối với $Q$ tạo thành một nhóm con chuẩn tắc chỉ số 2 trong nhóm các phép đồng dạng đối với $Q$.

d) Nếu $u$ là phép đối xứng đối với siêu phẳng trực giao với một vectơ không suy biến trong $E$, bây giờ chứng minh rằng $\mathrm{D}(u) = 1$. Suy ra rằng nhóm $\varphi(G^+)$ (các kí hiệu của No. 5) là nhóm $\mathbf{SO}(Q)$ được định nghĩa trong Bài tập 28 c) của $§ 6$.

e) Cho $u \in \mathbf{O}(Q)$, và giả sử $\Lambda$ đóng đại số. Hãy chỉ ra rằng, để có $u \in \mathbf{SO}(Q)$, điều kiện cần và đủ là số các ước sơ cấp của môđun $E_u$ là chẵn. (Với các kí hiệu của Bài tập 15 của $§ 5$, trước hết nhận xét rằng nếu $p, q$ là hai nhân tử bất khả quy phân biệt của đa thức tối tiểu của $u$, thì số các môđun con không phân tích được mà $G(p, q)$ là tổng trực tiếp của chúng bằng với số các môđun con không phân tích được mà $G(q, p)$ là tổng trực tiếp của chúng. Mặt khác, nhận xét rằng $G(p, p) = \{0\}$ trừ khi $p = X - 1$. Cuối cùng chứng minh rằng có thể hạn chế vào trường hợp $E_u$ bằng $G(p, p)$ (với $p = X - 1$) và là không phân tích được. Khi đó tồn tại một cơ sở đối xứng $(e_i)$ của $E$ sao cho $e_1, e_3, \ldots, e_{2k-1}$ tạo thành một cơ sở của $(p(u))^{2r-k}(E)$ với $1 \leq k \leq r$; hãy chỉ ra rằng $e_1, e_3, \ldots, e_{2r-3}$ là các vectơ kỳ dị, và kết luận rằng $\mathrm{D}(u) = 1$.)

$§ 10$ Ta giả sử rằng $A$ là một trường, $E$ là một không gian vectơ hữu hạn chiều, $Q$ là một dạng toàn phương suy biến trên $E$; gọi $M$ là một không gian con bù của $E^0$ trong $E$, $B$ là đại số Clifford (nửa đơn) của hạn chế của $Q$ lên $M$.

a) Trước hết giả sử rằng $A$ có đặc số $\neq 2$. Gọi $L$ là đại số Clifford của hạn chế của $Q$ lên $E^0$ (đẳng cấu với $\wedge E^0$), $\mathcal{R}_0$ là căn của nó (iđêan sinh trong $L$ bởi $E^0$, và có đối chiều 1 trong $L$); hãy chứng minh rằng căn $\mathcal{R}$ của $C(Q)$ thu được (lên đến một đẳng cấu) bằng cách xác định cấu trúc đại số trên $B \otimes_A \mathcal{R}_0$ như trong Hệ quả 4 của Định lý 1, rằng $C(Q)/\mathcal{R}$ đẳng cấu với $B$ và $C(Q)$ là tổng trực tiếp của $B$ và $\mathcal{R}$.

b) Giả sử rằng A có đặc số 2. Gọi F là không gian con của E⁰ tạo bởi các vectơ kỳ dị $x \in E^0$, và gọi N là một không gian con bù của F trong E⁰. Nếu $(a_i)_{1 \leq i \leq d}$ là một cơ sở của N, và Q$(a_i) = \alpha_i$, thì các phần tử $\alpha_i^{1/2}$, trong một bao đóng đại số của A, độc lập tuyến tính trên A. Gọi $(\alpha_i^{1/2})_{1 \leq i \leq e}$ là một 2-cơ sở của trường $A_1 = A(\alpha_1^{1/2}, \ldots, \alpha_d^{1/2})$ trên A (ch. V, § 8, bài tập 1), và đặt $h = \dim F$. Nếu B₁ là đại số đơn tâm $B \otimes_A A_1$, bây giờ chứng minh rằng C(Q) đẳng cấu với đại số $B_1 \otimes_{A_1} L_1$, trong đó $L_1$ là đại số ngoài của một không gian vectơ chiều $h + d - e$ trên $A_1$. Nếu $R_1$ là căn của $L_1$ (có đối chiều 1 (trên $A_1$) trong $L_1$), thì căn $R$ của C(Q) đẳng cấu với đại số $B_1 \otimes_{A_1} R_1$, $C(Q)/R$ đẳng cấu với $B_1$, và C(Q) là tổng trực tiếp của $B_1$ và $R$.

c) Với các giả thiết của b), giả sử thêm rằng $h = 0$, $d = 1, e = 0$ (điều này kéo theo rằng dim M là chẵn). Nếu $Q_0$ là hạn chế của Q lên M, bây giờ chứng minh rằng $C^+(Q)$ đẳng cấu với $C(Q_0)$.

¶ 11) a) Với các giả thiết và ký hiệu của No. 5, bây giờ chứng minh rằng $N(G^+)$ là nhóm con của $A^*$ sinh bởi các tích $Q(x)Q(y)$, trong đó $x$ và $y$ chạy qua tập hợp các vectơ không đẳng hướng của E. (Rút gọn về trường hợp $A \neq \mathbf{F}_2$; dùng mệnh đề 5 và bài tập 28 c) của § 6, cũng như bài tập 9 d) của § 9.) Trường hợp trong đó Q có chỉ số $\geq 1$.

b) Giả sử thêm rằng $A \neq \mathbf{F}_2$, rằng E có chiều $n \geq 2$ và rằng Q có chỉ số $> 0$. Bây giờ chứng minh rằng $O_0^+(Q)$ là nhóm giao hoán tử của nhóm $O(Q)$. (Rút gọn về trường hợp $n = 2$, dùng bài tập 17 c) và 28 e) của § 6.)

c) Giữ các giả thiết của b), và giả sử thêm rằng A có đặc số $\neq 2$ và E có chiều chẵn. Để tự đẳng cấu $x \to -x$ của E thuộc $O_0^+(Q)$, điều kiện cần và đủ là biệt thức của Q (đối với một cơ sở bất kỳ của E) là một bình phương.

¶ 12) a) Cho $a$ là một phần tử khả nghịch của A; bây giờ chứng minh rằng tồn tại một và chỉ một đẳng cấu $\theta_a$ từ $C^+(Q)$ lên $C^+(aQ)$ sao cho

$$
\theta_a(\rho(x)\rho(y)) = a^{-1}\rho_1(x)\rho_1(y)
$$

với mọi $x, y$ trong E ($\rho$ và $\rho_1$ lần lượt chỉ các ánh xạ chính tắc từ E vào $C(Q)$ và $C(aQ)$). Suy ra rằng nếu A là một trường có đặc số $\neq 2$, E là một không gian vectơ có chiều lẻ và Q là một dạng toàn phương không suy biến, thì $C(Q)$ và $C(aQ)$ đẳng cấu (x. bài tập 7).

b) Giả sử rằng $A$ là một trường, $E$ là một không gian vectơ có chiều chẵn $2r > 0$, $Q$ là một dạng toàn phương không suy biến. Cho $u$ là một phép tương tự đối với $Q$; chứng minh rằng tồn tại một và chỉ một tự đẳng cấu $A$-đại số $\bar{u}$ của đại số $C^+(Q)$ sao cho với $1 \leq h \leq r$ và $x_i \in E$ ($1 \leq i \leq 2h$), ta có

$$
\bar{u}(x_1x_2 \ldots x_{2h}) = \mu^{-h}u(x_1)u(x_2) \ldots u(x_{2h})
$$

trong đó $\mu$ chỉ nhân tử của $u$. Để $\bar{u}$ là một tự đẳng cấu trong, điều kiện cần và đủ là $u$ là một phép tương tự trực tiếp (§ 6, No. 5 và § 9, Bài tập 9 b)). Giả sử thêm rằng $r \geq 2$; khi đó, để $\bar{u}$ là đồng nhất, điều kiện cần và đủ là $u$ là một phép vị tự.

Chứng minh rằng tự đẳng cấu $\bar{u}$ của $C^+(Q)$ là hạn chế lên $C^+(Q)$ của một tự đẳng cấu trong của $C(Q)$.

¶ 13) Giả sử rằng $A$ là một trường có đặc số $\neq 2$, $E$ là một không gian vectơ có chiều chẵn $2r > 0$, $Q$ là một dạng toàn phương không suy biến. Ta ký hiệu bởi $E_h$ ảnh ngược của $\wedge^h E$ theo đẳng cấu $\mu_Q$ của Bài tập 3 c), sao cho $E_h$ là không gian con của $C(Q)$ sinh bởi các tích $x_1 x_2 \ldots x_h$, trong đó các $x_i$ ($1 \leq i \leq h$) trực giao từng đôi một.

a) Cho $\alpha$ là một phần tử của $A$, $s$ là một phần tử của $E_2$. Chứng minh rằng, nếu $(\alpha + s)^2 \in A$, thì hoặc $s = 0$, hoặc $\alpha = 0$ và $s = xy$, trong đó $x$ và $y$ là hai vectơ trực giao. (Nhận xét rằng nếu $t = \mu_Q(\alpha + s)$, thì $t \wedge t$ tất yếu thuộc $A + \wedge^2 E$, bằng cách biểu diễn $s$ với sự trợ giúp của một cơ sở trực giao của $E$; suy ra rằng tất yếu có $t = \beta + x \wedge y$ với $\beta \in A$, $x, y$ trong $E$, dùng § 5, No. 1, Hệ quả 2 của Định lý 1).

b) Cho $(x, y), (u, v)$ là hai cặp vectơ trực giao không đẳng hướng trong $E$, $P_{xy}$ và $P_{uv}$ lần lượt là các mặt phẳng $Ax + Ay, Au + Av$. Để có $(xy)(uv) = -(uv)(xy)$ trong $C(Q)$, điều kiện cần và đủ là $P_{xy} + P_{uv}$ là một không gian con phi đẳng hướng chiều 3, trong đó $P_{xy}$ và $P_{uv}$ trực giao yếu (§ 3, bài tập 11).

c) Cho $g$ là một tự đẳng cấu của $C^+(Q)$ biến $E_2$ thành chính nó; chứng minh rằng tồn tại một phép đồng dạng $u$ đối với $Q$ sao cho $g = \bar{u}$ (bài tập 12 b)). (Cho $(e_i)_{1 \leq i \leq 2r}$ là một cơ sở trực giao của $E$; dùng a và b), chứng minh rằng tồn tại một cơ sở trực giao $(x_i)$ của $E$ sao cho $g(e_1 e_i) = x_1 x_i$ với $2 \leq i \leq 2r$.

14) Giả sử rằng $A$ là một trường có đặc số $\neq 2$, $E$ là một không gian vectơ chiều $n$ trên $A$, $Q$ và $Q_1$ là hai dạng toàn phương không suy biến trên $E$; cho $\tilde{\Delta}$ (resp. $\tilde{\Delta}_1$) là lớp của biệt thức $\Delta$ của $Q$ (resp. của biệt thức $\Delta_1$ của $Q_1$) đối với một cơ sở của $E$, trong nhóm $A^*/(A^*)^2$, một lớp không phụ thuộc vào cơ sở được chọn trong $E$. Giả sử rằng $n = 2$.

a) Chứng minh rằng nếu $\tilde{\Delta} = \tilde{\Delta}_1$ và nếu các đại số Clifford $C(Q)$ và $C(Q_1)$ là đẳng cấu, thì $Q$ và $Q_1$ là tương đương (xét trên $C(Q)$ dạng toàn phương $z \mapsto z \bar{z}$, trong đó $z \mapsto \bar{z}$ là phản tự đẳng cấu đối hợp duy nhất của $C(Q)$ mà tập hợp các phần tử bất biến là tâm của $C(Q)$ (x. bài tập 6 và chương VIII, § 11, bài tập 5 e)); áp dụng định lý Witt).

(b) Để $C(Q)$ đẳng cấu với đại số ma trận $\mathbf{M}_2(A)$ thì điều kiện cần và đủ là, với ít nhất một $x \neq 0$ trong $E$, tồn tại $y, z$ trong $E$ sao cho $Q(x) + Q(y)Q(z) = 0$; nếu đúng như vậy thì tính chất này đúng với mọi $x \neq 0$ trong $E$.

¶ 15) Ta giữ lại ký hiệu và các giả thiết tổng quát của Bài tập 14, nhưng giả sử $n = 3$.

(a) Bây giờ chứng minh rằng $C^+(Q)$ đẳng cấu với một đại số quaternion trên $A$ và rằng $\beta$ là phản tự đẳng cấu $z \mapsto \bar{z}$ của đại số này mà tập hợp các phần tử bất biến là tâm của $C^+(Q)$; nếu $P$ là không gian con của $C^+(Q)$ tạo bởi các quaternion thuần túy (nghĩa là các $z$ sao cho $z = -\bar{z}$; chương VIII, § 11, Bài tập 6), thì hạn chế lên $P$ của dạng toàn phương $z \mapsto z \bar{z}$ là tương đương với $\lambda Q$, trong đó $\lambda \in A$. Suy ra rằng để $C^+(Q)$ là một trường thì điều kiện cần và đủ là $Q$ có chỉ số 0.

(b) Bây giờ chứng minh rằng nếu $\tilde{\Delta} = \tilde{\Delta}_1$ và nếu các đại số Clifford $C(Q)$ và $C(Q_1)$ là đẳng cấu, thì $Q$ và $Q_1$ là tương đương. (Trước hết xét trường hợp $-\Delta$ là một bình phương trong $K$, và chứng minh rằng trong trường hợp này $C^+(Q)$ và $C^+(Q_1)$ là đẳng cấu; rồi lập luận như trong Bài tập 14 a), dùng a) và Bài tập 6 của chương VIII, § 11. Trong trường hợp tổng quát, dùng Bài tập 12 $a))$.

(c) Bây giờ chứng minh rằng nhóm Clifford đặc biệt $G^+$ (đối với dạng $Q$) đồng nhất với nhóm các phần tử khả nghịch của $C^+(Q)$. (Nếu $(e_1, e_2, e_3)$ là một cơ sở trực giao của $E$, và nếu $j = e_1 e_2 e_3$ trong $C(Q)$, hãy nhận thấy rằng $x \to xj$ là một đẳng cấu không gian vectơ từ $E$ lên $P$).

(d) Suy ra từ a) và c) rằng nếu $Q$ có chỉ số 1, thì nhóm quay $O^+(Q)$ đẳng cấu với nhóm xạ ảnh $\mathbf{PGL}_2(A)$ (chương II, 2e éd., App. III, No. 6).

¶ 16) Ta giữ lại các giả thiết và ký hiệu tổng quát của Bài tập 14, nhưng giả sử $n = 4$.

a) Hãy cho một ví dụ trong đó $\tilde{\Delta} = \tilde{\Delta}_1$ và trong đó $C(Q)$ và $C(Q_1)$ là đẳng cấu, nhưng $Q$ và $Q_1$ không tương đương (x. bài tập 7).

b) Gọi $(e_i)_{1 \leq i \leq 4}$ là một cơ sở trực giao của $E$ đối với $Q$, $Q_0$ là hạn chế của $Q$ lên siêu phẳng $H = Ae_1 + Ae_2 + Ae_3$. Bây giờ chứng minh rằng, nếu $Z$ là tâm của $C^+(Q)$, thì đại số $C^+(Q)$ đẳng cấu với tích tenxơ $Z \otimes_A C^+(Q_0)$. Với mọi $z \in C^+(Q)$, ta có $\beta(z)z \in Z$; để $z$ thuộc nhóm Clifford đặc biệt $G^+$, điều kiện cần và đủ là $z$ khả nghịch và $\beta(z)z \in A.1$. Suy ra rằng nhóm $O_0^+(Q)$ đẳng cấu với thương của nhóm các phần tử $z \in Z \otimes_A C^+(Q_0)$ sao cho $\beta(z)z = 1$ theo $\{1, -1\}$.

c) Giả sử rằng $\Delta$ không là một bình phương trong $A$ (điều này kéo theo, theo định lý của Witt, rằng chỉ số của $Q$ bằng 0 hoặc 1). Nếu $Q_0'$ là dạng toàn phương thu được từ $Q_0$ bằng mở rộng lên $A' = A(\sqrt{\Delta})$ của trường các vô hướng, suy ra từ b) rằng $O_0^+(Q)$ đẳng cấu với $O_0^+(Q_0')$. Đặc biệt, nếu $Q$ có chỉ số 1, $O_0^+(Q)$ là nhóm các giao hoán tử của $O(Q)$ và đẳng cấu với $\mathbf{PSL}_2(A')$ (x. bài tập 15 $d$) và chương III, § 7, bài tập 8).

d) Ta giả sử rằng $\Delta$ là một bình phương trong $A$ (điều này kéo theo, do định lý của Witt, rằng $Q$ có chỉ số 0 hoặc 2) và rằng $Q(e_4) = 1$. Nếu đặt $j = e_1 e_2 e_3$, thì mọi $x \in E$ đều có thể viết được theo một và chỉ một cách dưới dạng $x = \alpha e_4 + jz$, trong đó $\alpha \in A$ và $z$ là một quaternion thuần (Bài tập 15 $a$)) trong $L = C^+(Q_0)$; nếu đặt $\psi(x) = \alpha + z$, thì $\psi$ là một đẳng cấu không gian vectơ từ $E$ lên $L$. Đặt $Z = Ac' + Ac''$, trong đó $c'$ và $c''$ là hai phần tử lũy đẳng trực giao trong $Z$; mọi phần tử khả nghịch $s \in C^+(Q)$ đều có thể viết được theo một và chỉ một cách dưới dạng $s = uc' + vc''$, trong đó $u$ và $v$ thuộc $L$; để $s$ thuộc nhóm Clifford đặc biệt $G^+$, điều kiện cần và đủ là $u \bar{u} = v \bar{v}$, và khi đó ta có $\psi(sxs^{-1}) = u \psi(x) v^{-1}$ với mọi $x \in E$. Suy ra rằng thương của $O_0^+(Q)$ bởi tâm của nó (là một nhóm có 2 phần tử, xem Bài tập 11 $c$)) đẳng cấu với tích $O_0^+(Q_0) \times O_0^+(Q_0)$; đặc biệt, nếu $Q$ có chỉ số 2, thì nhóm thương này đẳng cấu với $\mathbf{PSL}_2(A) \times \mathbf{PSL}_2(A)$.

17) Cho K là một trường giao hoán có đặc số $\neq 2$, $A$ là trường $K(X_n)_{n \in \mathbf{N}}$ các phân thức hữu tỉ trên K, theo một họ đếm được các ẩn (Chương IV, § 3, No. 1). Cho E là một không gian vectơ trên A, có một cơ sở đếm được $(e_n)_{n \in \mathbf{N}}$, và cho $\Phi$ là một dạng song tuyến tính đối xứng trên E, sao cho $(e_n)$ là một cơ sở trực giao và $\Phi(e_n, e_n) = X_n$ với mọi $n \in \mathbf{N}$. Nếu đặt $Q(x) = \Phi(x, x)$, hãy chứng minh rằng đại số Clifford C(Q) là một trường (xem Chương VIII, § 12, Bài tập 14).
