---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 9
section_title: Equations différentielles et feuilletages
lang: vi
source: var-fr
pdf_pages: 0116-0125
extraction: ocr
subsections:
    - "no": 1
      title: Courbes intégrales
      page: 0
      pdf_page: 116
    - "no": 2
      title: Feuilletages
      page: 0
      pdf_page: 119
    - "no": 3
      title: Sous-fibrés intégrables
      page: 0
      pdf_page: 121
    - "no": 4
      title: Fibrés intégrables en caractéristique p ≠ 0
      page: 0
      pdf_page: 124
statements: 2
exercises: 0
content_sha256: 9a7b35caf5ca08886fd8fe47314703d5f1fe681ebc1f262bb9901c01b02dc9de
translated_from: content/en-mt/var/2/09_s9_equations_differentielles_et.md
source_lang: en-mt
translation_method: machine
source_content_sha256: e3c377f68c06b091929ac36db234b8f79caaef31ed09f6a129b1ece0caf8c8f1
translation_model: gpt-5-6
translation_run: translate-vi-7d9d2edd
glossary_version: 34
glossary_terms_sha256: d7f1adb52e0a19f3ba729913bf4ddc5e14dc64ab7e14dd020920393388c9cf20
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. Phương trình vi phân và các lá

Trong các số $^{\mathrm{os}}$ 9.1, 9.2 và 9.3, giả sử K có đặc số 0. Trong số $^\circ$ 9.4, giả sử K có đặc số $p \ne 0$.

### 9.1. Các đường cong nguyên

Trong số $^\circ$ này, X ký hiệu một đa tạp thuộc lớp $C^r$ và $\xi$ một trường vectơ thuộc lớp $C^s$ trên X, với $r$, $s$ thuộc $\mathbf{N}_K$, $s \leq r - 1$.

9.1.1. Cho I là một tập con mở của K, và cho $f : I \to X$ là một ánh xạ thuộc lớp $C^k$ ($k \in \mathbf{N}_K$, $k \leq r$) từ I vào X. Với $t \in I$, ta ký hiệu vectơ $T_t(f)(1) \in T_{f(t)}(X)$ là $f'(t)$; vectơ này đôi khi được gọi là vận tốc của $f$ tại thời điểm $t$. Khi X là một không gian Banach, $f'(t)$ là đạo hàm của $f$ tại $t$.

Ta nói rằng $f$ là một đường cong nguyên của $\xi$ nếu ta có

$$(1)\qquad f'(t)=\xi(f(t))$$

với mọi $t \in I$. Một đường cong như vậy thuộc lớp $C^{s+1}$.

Nếu $x$ là một điểm của X, ta gọi đường cong nguyên của $\xi$ có gốc $x$ là một đường cong nguyên $f : I \to X$ của $\xi$ sao cho $0 \in I$ và $f(0)=x$; với mọi $x \in X$, tồn tại một đường cong nguyên của $\xi$ có gốc $x$, được xác định trong một lân cận mở thích hợp của 0 trong K.

Nếu $f : I \to X$ là một đường cong nguyên của $\xi$ và nếu $a \in K$, ánh xạ $t \mapsto f(t-a)$ từ $I+a$ vào X là một đường cong nguyên của $\xi$.

Cho $f_1 : I_1 \to X$ và $f_2 : I_2 \to X$ là hai đường cong nguyên của $\xi$, và $t \in I_1 \cap I_2$. Nếu $f_1(t)=f_2(t)$, các ánh xạ $f_1$ và $f_2$ trùng nhau trong một lân cận của $t$.

9.1.2 (« Các dòng »). Cho W là một tập mở của $X \times K$. Với mọi $x \in X$, ký hiệu $W_x$ là tập hợp các $t \in K$ sao cho $(x,t) \in W$. Một dòng nguyên của $\xi$ với miền W được gọi là một ánh xạ $f$ thuộc lớp $C^k$ ($k \leq r$) từ W vào X sao cho, với mọi $x \in X$, ánh xạ $f_x : W_x \to X$ xác định bởi $f_x(t)=f(x,t)$ là một đường cong nguyên của $\xi$, và sao cho với $(x,0) \in W$ ta có $f(x,0)=x$.

Với mọi điểm $x \in X$, tồn tại một dòng nguyên của $\xi$ thuộc lớp $C^s$ có miền là một lân cận của $(x,0)$ trong $X \times K$. Hai dòng nguyên của $\xi$ được xác định trong một lân cận của $(x,0)$ trùng nhau trên một lân cận của $(x,0)$.

Cho $x \in X$ và cho $f$ là một dòng nguyên của $\xi$ có miền W là một lân cận của (x, 0). Tồn tại một lân cận V của (x, 0, 0) trong X × K × K sao cho, nếu (x, t_1, t_2) ∈ V, ta có
$$(x, t_1) \in W,\quad (f(x, t_1), t_2) \in W,\quad (x, t_1 + t_2) \in W$$
và
(2)
$$f(f(x, t_1), t_2) = f(x, t_1 + t_2).$$
Nếu X là paracompact, hoặc nếu X là tách được và K = R hoặc C, tồn tại một dòng nguyên của $\xi$ có miền là một lân cận của X × {0}.

9.1.3 (« Trường hợp thực »). Ta giả sử rằng K = R và X là tách được. Một *cung nguyên* của $\xi$ là bất kỳ đường cong nguyên nào của $\xi$ có miền là một khoảng mở của R. Hai cung nguyên $f_1$ và $f_2$ của $\xi$, được xác định trên các khoảng $I_1$ và $I_2$, và trùng nhau tại một điểm của $I_1 \cap I_2$, trùng nhau trong $I_1 \cap I_2$.

Với mọi điểm $x \in X$, tồn tại duy nhất một cung nguyên có gốc x, $f_x : I_x \to X$, sao cho, với mọi cung nguyên $f : I \to X$ có gốc x, ta có $I \subset I_x$ và $f = f_x|I$. Cung $f_x$ được gọi là *cung nguyên cực đại* của $\xi$ có gốc x, và miền $I_x$ của nó đôi khi được gọi là *khoảng sống* của điểm x đối với trường $\xi$.

Nếu $I_x = ] -a_-, a_+ [$ và nếu $a_+$ là hữu hạn, hạn chế của $f_x$ trên khoảng $[0, a_+ [$ là một ánh xạ thực sự của $[0, a_+ [$ vào X. Đặc biệt, $f(t)$ không có giới hạn khi t tiến tới $a_+$.

9.1.4. Với các ký hiệu và giả thiết của 9.1.3, tập hợp $\Omega$ gồm các cặp $(x, t) \in X \times \mathbf{R}$ sao cho $t \in I_x$ là mở trong $X \times \mathbf{R}$ và ánh xạ $f : \Omega \to X$ xác định bởi $f(x, t) = f_x(t)$ là thuộc lớp $C^s$; nó là một dòng nguyên của $\xi$ với miền xác định $\Omega$.

Các hàm $\alpha_+$ và $\alpha_- : X \to ]0, +\infty]$ được xác định bởi $I_x = ] -\alpha_-(x), \alpha_+(x)[$ là nửa liên tục dưới. Với $(x, t) \in \Omega$ và $y = f(x, t)$, ta có $\alpha_+(y) = \alpha_+(x) - t$ và $\alpha_-(y) = \alpha_-(x) + t$.

Nếu $t_1 \in I_x$ và nếu $t_2 \in I_{f(x, t_1)}$, thì $t_1 + t_2 \in I_x$ và
(3)
$$f(f(x, t_1), t_2) = f(x, t_1 + t_2).$$

Nếu hàm $\alpha_+$ (tương ứng $\alpha_-$) bị chặn dưới trên X bởi một hằng số $> 0$, thì nó là hằng và bằng $+\infty$.

Ta có $\alpha_+ = \alpha_- = +\infty$ (nói cách khác, ta có $\Omega = X \times \mathbf{R}$) trong mỗi trường hợp sau:

(i) trường $\xi$ có giá compact (ví dụ nếu X là compact);
(ii) tồn tại một nhóm các tự đẳng cấu của X, bắc cầu, và bảo toàn $\xi$;
*(iii) tồn tại trên X một cấu trúc Riemann mà đối với nó X là đầy đủ và $\xi$ bị chặn.*

Nếu $\Omega = X \times \mathbf{R}$, ánh xạ $f : X \times \mathbf{R} \to X$ là một luật phép toán phải thuộc lớp $C^s$ của đa tạp nhóm $\mathbf{R}$ trên đa tạp X, xem 5.12.5.

9.1.5 (« Trường hợp phức »). Giả sử rằng K = C và rằng X là tách được. Với mọi $a \in ]0, +\infty]$, ký hiệu $D_a$ là đĩa mở tâm 0 và bán kính a trong C. Với mọi $x \in X$, tồn tại một và chỉ một số $\rho(x) \in ]0, +\infty]$, một và chỉ một đường cong nguyên $f_x : D_{\rho(x)} \to X$ với gốc x sao cho, với mọi $a \in ]0, +\infty]$ và mọi đường cong nguyên $f : D_a \to X$ với gốc x, ta có $a \leq \rho(x)$ và $f = f_x|D_a$.

Với mọi $\lambda \in \mathbf{C}$, gọi $\alpha_\lambda(x)$ là cận trên đúng của khoảng tồn tại của x đối với trường vectơ $\lambda \xi$ trên đa tạp thực suy ra từ X bằng hạn chế vô hướng. Ta có $\rho(x) = \inf_{|\lambda|=1} \alpha_\lambda(x)$.

Tập hợp $\Delta$ gồm các cặp $(x, t) \in X \times \mathbf{C}$ sao cho $t \in D_{\rho(x)}$ là mở trong $X \times \mathbf{C}$ và ánh xạ $f$ từ $\Delta$ vào $X$ được xác định bởi $f(x, t) = f_x(t)$ là một dòng nguyên của $\xi$. Hàm $\rho : X \to ]0, +\infty]$ là nửa liên tục dưới. Với $(x, t) \in \Delta$ và $y = f(x, t)$, ta có $\rho(y) \geq \rho(x) - |t|$. Nếu $\rho$ bị chặn dưới trên $X$ bởi một hằng $> 0$, ta có $\rho = +\infty$ và $\Delta = X \times \mathbf{C}$.

Khi $\Delta = X \times \mathbf{C}$, ánh xạ $f : X \times \mathbf{C} \to X$ là một luật phép toán phải của nhóm đa tạp $\mathbf{C}$ trên đa tạp $X$.

9.1.6. Cho $\varphi : X \to Y$ là một cấu xạ của các đa tạp và $\eta$ là một trường vectơ trên $Y$ sao cho $\xi$ liên quan $\varphi$ với $\eta$ (xem 8.2.6). Nếu $f : I \to X$ là một đường cong nguyên của $\xi$, ánh xạ $\varphi \circ f : I \to Y$ là một đường cong nguyên của $\eta$. Nếu $K = \mathbf{R}$ và nếu $X$ và $Y$ là tách được, với mọi $x \in X$, khoảng tồn tại của $x$ đối với $\xi$ được chứa trong khoảng tồn tại của $\varphi(x)$ đối với $\eta$. Nếu hơn nữa, $\varphi$ là thực sự, các khoảng này bằng nhau.

9.1.7 (“Các phương trình phụ thuộc thời gian”). Cho $W$ là một tập con mở của $X \times K$ và cho $\Xi : W \to T(X)$ là một phép nâng lớp $C^s$ của $\mathrm{pr}_1 : W \to X$, nghĩa là một ánh xạ lớp $C^s$ từ $W$ vào $T(X)$ sao cho $\Xi(x, t)$ thuộc $T_x(X)$ với mọi $(x, t) \in W$. Một đường cong nguyên của $\Xi$ là một ánh xạ $f$ lớp $C^k$ (với $k \in \mathbf{N}_K$ và $k \leq r$), từ một tập con mở $I$ của $K$ vào $X$ sao cho, với mọi $t \in I$, ta có

$$
(f(t), t) \in W \text{ và } f'(t) = \Xi(f(t), t).
$$

Cho $\eta$ là trường vectơ lớp $C^s$ trên $W$ được xác định bởi $\eta(x, t) = (\Xi(x, t), (t, 1))$. Đối với một ánh xạ $f$ từ một tập con mở $I$ của $K$ vào $X$ là một đường cong nguyên của $\Xi$, điều kiện cần và đủ là $t \mapsto (f(t), t)$ là một đường cong nguyên của $\eta$ theo nghĩa của 9.1.1.

Cho $g : I \to W$ là một đường cong nguyên của $\eta$ và $t_0$ là một điểm của $I$ sao cho $\mathrm{pr}_2(g(t_0)) = t_0$. Tập hợp các phần tử $t \in I$ sao cho $\mathrm{pr}_2(g(t)) = t$ là một lân cận của $t_0$ trùng với $I$ nếu $I$ là liên thông.

9.1.8 (“Các tham số và các điều kiện ban đầu”). Cho $Z$ là một đa tạp lớp $C^r$, cho $W$ là một tập con mở của $X \times K \times Z$, và cho $\Xi$ là một phép nâng lớp $C^s$ của $\mathrm{pr}_1 : W \to X$ (8.6.1). Nếu $z \in Z$, ta ký hiệu $W_z$ là tập hợp các $(x, t) \in X \times K$ sao cho $(x, t, z) \in W$, và ta ký hiệu $\Xi_z$ là ánh xạ $(x, t) \mapsto \Xi(x, t, z)$ từ $W_z$ vào $T(X)$.

Cho $(x_0, t_0, z_0)$ là một điểm của $W$. Khi đó tồn tại một lân cận mở $X_1 \times I_1 \times Z_1$ của $(x_0, t_0, z_0)$ trong $W$ và một ánh xạ lớp $C^s$

$$
f : X_1 \times I_1 \times I_1 \times Z_1 \to X
$$

sao cho, với mọi $(x_1, t_1, z_1) \in X_1 \times I_1 \times Z_1$, ánh xạ $t \mapsto f(x_1, t_1, t, z_1)$ là một đường cong nguyên của $\Xi_{z_1}$ (theo nghĩa của 9.1.7) thỏa mãn quan hệ $f(x_1, t_1, t_1, z_1) = x_1$.

Hai ánh xạ

$$
f_1 : X_1 \times I_1 \times I_1 \times Z_1 \to X \quad \text{và} \quad f_2 : X_2 \times I_2 \times I_2 \times Z_2 \to X
$$

thỏa mãn các điều kiện trên trùng nhau trong một lân cận của $(x_0, t_0, t_0, z_0)$.

### 9.2. Các phân lá

Trong No. này, X ký hiệu một đa tạp lớp $C^r$, với $r \in \mathbf{N}_K$. Trừ khi có nói khác đi, tất cả các đa tạp và tất cả các cấu xạ được xét đều được giả thiết là thuộc lớp $C^r$.

9.2.1. Cho S là một đa tạp, và cho $p : X \to S$ là một ánh xạ ngập chìm. Với mỗi $s \in S$, trang bị cho $X_s = p^{-1}(s)$ cấu trúc đa tạp cảm sinh bởi cấu trúc của X (5.10.5); tập hợp X là hợp rời nhau của các $X_s$. Ký hiệu $X_p$ là cấu trúc đa tạp trên X thu được bằng cách dán các $X_s$, với $s \in S$ (5.2.4); đó là cấu trúc đa tạp duy nhất trên X mà đối với nó các $X_s$ là các đa tạp con mở. Không gian tôpô $X_p$ là tổng của các không gian $X_s$.

Cho V là một đa tạp và $f$ là một ánh xạ từ V vào X. Để $f$ là một cấu xạ từ V vào $X_p$, điều kiện cần và đủ là $f$ là một cấu xạ từ V vào X và $p \circ f$ là hằng địa phương.

9.2.2. Một phân lá của X được gọi là một đa tạp Y có cùng tập nền với X và thỏa mãn điều kiện sau:

(F) Với mọi $x \in X$, tồn tại một đa tạp con mở U của X chứa x, một đa tạp S và một ánh xạ ngập chìm $p : U \to S$ sao cho đa tạp $U_p$ là một đa tạp con mở của Y.

Cặp (X, Y) cũng được gọi là một đa tạp phân lá. Nếu (X, Y) và (X', Y') là các đa tạp phân lá, một cấu xạ từ (X, Y) vào (X', Y') là bất kỳ ánh xạ nào $f : X \to X'$ vừa là một cấu xạ của đa tạp X vào đa tạp X' vừa là một cấu xạ của đa tạp Y vào đa tạp Y'.

Cho (X, Y) là một đa tạp phân lá. Ánh xạ đồng nhất $Y \to X$ là một phép nhúng song ánh. Một tập con U của X được gọi là một lá nếu nó là một tập mở của Y; trong trường hợp này, U được trang bị cấu trúc tôpô và cấu trúc đa tạp cảm sinh bởi các cấu trúc của Y; chẳng hạn, U được gọi là một lá liên thông nếu nó là một tập con mở và liên thông của Y. Các lá là các đa tạp con của X tạo thành một cơ sở của tôpô của Y. Khi $K = \mathbf{R}$ hoặc $\mathbf{C}$, các thành phần liên thông của Y là các lá, được gọi là các lá liên thông cực đại của (X, Y).

9.2.3. Nếu $s \in \mathbf{N}_K, s \leq r$, một phân lá lớp $C^s$ của X được gọi là một phân lá của đa tạp lớp $C^s$ nền X.

9.2.4. Ví dụ

a) Đa tạp X là một phân lá của X, được gọi là phân lá thô của X.

b) Nếu $p : X \to S$ là một ánh xạ ngập chìm, $X_p$ là một phân lá của X, được gọi là phân lá của X xác định bởi p. Phân lá của X xác định bởi ánh xạ đồng nhất là tập hợp X được trang bị cấu trúc đa tạp thuần túy của chiều 0 (5.2.1); nó được gọi là phân lá rời rạc của X.

c) Cho E là một không gian Banach, F là một không gian con vectơ đóng của E có một phần bù tôpô, và $p$ là phép chiếu chính tắc $E \to E/F$. Phân lá $E_p$ của E được gọi là phân lá của E xác định bởi F.

d) Cho $\Gamma$ là một nhóm rời rạc tác động chính quy và tự do lên không gian tôpô $X$ (TG, III, § 4, n° 4). Cho $Y$ là một phân lá của $X$, và giả sử rằng, với mọi $s \in \Gamma$, ánh xạ $x \mapsto sx$ là một tự đẳng cấu của $(X, Y)$. Quan hệ tương đương trên $X$ (resp. $Y$) mà các lớp của nó là các quỹ đạo của $\Gamma$ là chính quy (5.9.5). Nếu $X/\Gamma$ (resp. $Y/\Gamma$) được gọi là đa tạp thương tương ứng, cặp $(X/\Gamma, Y/\Gamma)$ là một đa tạp phân lá, được gọi là thương của $(X, Y)$ bởi $\Gamma$.

9.2.5. Cho $Y$ là một phân lá của $X$ và $U$ là một tập con mở của $X$. Khi đó $U$ là mở trong $Y$ và $U$, được trang bị cấu trúc của đa tạp cảm sinh bởi cấu trúc của $Y$, là một phân lá của $X$, được gọi là phân lá cảm sinh bởi $Y$.

Nói chung hơn, cho $f : X' \to X$ là một cấu xạ sao cho $f$ và ánh xạ đồng nhất $Y \to X$ tạo thành một cặp ngang (5.11.1). Tích sợi $Y' = X' \times_X Y$ được đồng nhất một cách chính tắc với một phân lá của $X'$ được gọi là phân lá ảnh ngược của $Y$ bởi $f$.

9.2.6. Cho $p : X \to S$ và $p' : X' \to S'$ là hai phép ngập, và cho $f$ là một cấu xạ từ $X$ đến $X'$. Để $f$ là một cấu xạ từ $X_p$ đến $X_{p'}$, điều kiện cần và đủ là, với mọi $x \in X$, tồn tại một lân cận mở $U$ của $x$ trong $X$ và một cấu xạ $g$ từ $p(U)$ đến $S'$ sao cho $g \circ p = p' \circ f$ trên $U$.

9.2.7. Cho $Y$ là một phân lá của $X$. Một biểu đồ phân lá của $(X, Y)$ được gọi là một bộ bốn $(U, \varphi, E, F)$ sao cho $(U, \varphi, E)$ là một biểu đồ của $X$, $F$ là một không gian con vectơ đóng của không gian Banach $E$ nhận một phần bù tôpô và $\varphi$ là một đẳng cấu của phân lá của $U$ cảm sinh bởi $Y$ lên phân lá của $\varphi(U)$ được xác định bởi ánh xạ chính tắc của $E$ lên $E/F$. Với mọi điểm $x \in X$, tồn tại một biểu đồ phân lá $(U, \varphi, E, F)$ của $(X, Y)$ sao cho $x \in U$. Đặt $n = \dim_x X$ và $m = \dim_x Y$. Nếu $n$ là hữu hạn, tồn tại một lân cận mở $U$ của $x$ và một hệ tọa độ $\zeta^1, \ldots, \zeta^n$ của $X$ trên $U$ sao cho phân lá của $U$ cảm sinh bởi $Y$ trùng với phân lá được xác định bởi ánh xạ $(\zeta^{m+1}, \ldots, \zeta^n)$ của $U$ vào $K^{n-m}$.

9.2.8. Cho $Y$ là một phân lá của $X$. Khi $x$ chạy qua $X$, các không gian $T_x(Y)$ là các thớ của một phân bó con vectơ thuộc lớp $C^{r-1}$ của $T(X)$ được gọi là phân bó con của $T(X)$ tiếp xúc với phân lá $Y$ và được ký hiệu là $T(X, Y)$. Nếu phân lá $Y$ được xác định bởi một ánh xạ ngập $p : X \to S$, thì $T(X, Y) = \mathrm{Ker}\, T(p)$ là phân bó tiếp xúc tương đối $T(X/S)$ của $X$ trên $S$ (8.1.3).

Cho $(X, Y)$ và $(X', Y')$ là hai đa tạp phân lá, và cho $f$ là một cấu xạ từ $X$ vào $X'$. Để $f$ là một cấu xạ của các đa tạp phân lá, điều kiện cần và đủ là $T(f)$ ánh xạ $T(X, Y)$ vào $T(X', Y')$. Đặc biệt, cho $f : Z \to X$ là một cấu xạ của các đa tạp; để $f$ là một cấu xạ từ $Z$ vào $Y$, điều kiện cần và đủ là $T(f)$ ánh xạ $T(Z)$ vào $T(X, Y)$. Để một đa tạp con $Z$ của $X$ là một lá của $(X, Y)$, điều kiện cần và đủ là

$$
T_z(Z) = T_z(X, Y) \quad \text{với mọi } z \in Z.
$$

Cho $Y$ là một phân lá của $X$ và cho $U$ là một lá của $Y$, có một cơ sở đếm được của các tập mở. Cho $Z$ là một đa tạp và $f$ là một ánh xạ của $Z$ vào $U$. Để $f$ là một cấu xạ của các đa tạp từ Z vào U, điều kiện cần và đủ là hợp thành của f và đơn ánh chính tắc của U vào X là một cấu xạ của các đa tạp từ Z vào X. Nếu X là compact địa phương và đếm được tại vô cực, mọi lá liên thông của (X, Y) đều có một cơ sở đếm được của các tập mở (xem TG, I, 3e éd., §11, No. 7, cor. 2 du th. 1).

9.2.9. Giả sử rằng K = R hoặc C. Cho Y là một phân lá của X. Các điều kiện sau là tương đương:

a) Tồn tại một đa tạp S và một phép chìm $p : X \to S$ sao cho $Y = X_p$.

b) Với mọi $x \in X$, tồn tại một đa tạp con $S_x$ của X có hai tính chất sau:
   b₁) Không gian tiếp xúc $T_x(S_x)$ của $S_x$ tại $x$ là một phần bù tôpô của $T_x(X, Y)$ trong $T_x(X)$.
   b₂) Mọi lá liên thông của (X, Y) gặp $S_x$ tại nhiều nhất một điểm.

Giả sử các điều kiện này được thỏa mãn và cho $R \{x, y\}$ là quan hệ trên X “x và y thuộc cùng một lá liên thông”; khi đó R là một quan hệ tương đương chính quy (5.9.5) trên X, và, nếu p ký hiệu phép chiếu chính tắc $X \to X/R$, ta có $Y = X_p$.

#### Ví dụ {#var-2-s9-n2-exa-1 .statement}

Cho $K = R$ và $X = R^2$. Cho nhóm rời rạc $\Gamma = Z^2$ tác động lên X bởi các phép tịnh tiến. Cho $m \in R$ và cho $(X, Y_m)$ là phép phân lá được xác định bởi hàm dưới ngập $p : (x_1, x_2) \mapsto x_2 - mx_1$ của X lên R. Đặt $X' = X/\Gamma$ và $Y'_m = Y_m/\Gamma$; khi đó $Y'_m$ là một phép phân lá của xuyến $X'$ (xem 9.2.4, ví dụ d)). Nếu m là hữu tỉ, tồn tại một hàm dưới ngập $p'$ của $X'$ lên $R/Z$ sao cho $Y'_m = X'_{p'}$. Nếu m là vô tỉ, mọi lá liên thông cực đại của $(X', Y'_m)$ đều trù mật trong $X'$, và không tồn tại một hàm dưới ngập $p'$ của $X'$ vào một đa tạp S sao cho $Y'_m = X'_{p'}$.

9.2.10. Cho Y là một phép phân lá của X, và cho $\pi : X \to S$ là một cấu xạ của các đa tạp sao cho hợp thành $Y \to X \xrightarrow{\pi} S$ là étale. Nếu S’ là một tập con mở của S, một tiết diện $\sigma : S' \to X$ của $\pi$ trên S’ được gọi là ngang (đối với phép phân lá Y) nếu nó là một cấu xạ từ S’ vào Y; điều này tương đương với việc nói rằng $\sigma(S')$ là một lá của (X, Y), hay một lần nữa rằng $T(\sigma)$ ánh xạ $T(S')$ vào $T(X, Y)$. Với mọi $s_0 \in S$ và mọi $x_0 \in \pi^{-1}(s_0)$, tồn tại một tiết diện ngang được xác định trong một lân cận của $s_0$ và nhận giá trị $x_0$ tại $s_0$; hai tiết diện như vậy trùng nhau trên một lân cận của $s_0$.

Nói chung hơn, cho $s_0 \in S$, cho T là một đa tạp, cho f là một cấu xạ từ T vào đa tạp con $\pi^{-1}(s_0)$ của X, và cho $t_0 \in T$. Khi đó tồn tại một lân cận mở T’ (tương ứng S’) của $t_0$ trong T (tương ứng của $s_0$ trong S), và một cấu xạ
$$
F : S' \times T' \to X
$$
thỏa mãn điều kiện sau: với mọi $t \in T'$, ánh xạ $s \mapsto F(s, t)$ là một tiết diện ngang của $\pi$ trên S’ nhận giá trị $f(t)$ tại điểm $s_0$. Hai ánh xạ như vậy F trùng nhau trên một lân cận của $(s_0, t_0)$.

### 9.3. Các phân bó con khả tích

Trong số này, X kí hiệu một đa tạp thuộc lớp $C^r$ và F một phân bó con vectơ thuộc lớp $C^s$ của $T(X)$, với $r, s$ trong $N_K, s \leq r - 1$.

9.3.1. Cho V là một đa tạp thuộc lớp $C^k$ ($k \in \mathbf{N}_K, k \leq r$) và cho $f$ là một cấu xạ thuộc lớp $C^k$ từ V vào X. Ta nói rằng $f$ là một nguyên tích phân của F nếu $T(f)$ ánh xạ $T(V)$ vào F.

Một đa tạp con Z lớp $C^k$ của X được gọi là một đa tạp con nguyên của F nếu đơn ánh $Z \to X$ là một tích phân của F theo nghĩa trên, tức là nếu có $T_x(Z) \subset F_x$ với mọi $x \in Z$.

Cho $x \in X$. Nếu $Z_1$ và $Z_2$ là hai đa tạp con nguyên của X chứa $x$ và nếu $T_x(Z_1) = F_x$, thì tồn tại một lân cận U của $x$ sao cho $U \cap Z_2 \subset Z_1$. Nếu thêm vào đó $T_x(Z_2) = F_x$, thì các mầm của $Z_1$ và $Z_2$ tại $x$ trùng nhau.

9.3.2. Ta nói rằng F là khả tích nếu tồn tại một lá Y của X lớp $C^s$ sao cho $F = T(X, Y)$ (9.2.8). Khi đó lá như vậy là duy nhất; nó được gọi là lá nguyên của F. Để một cấu xạ $f : V \to X$ lớp $C^s$ là một tích phân của F, điều kiện cần và đủ là $f$ là một cấu xạ của V vào Y.

#### Ví dụ {#var-2-s9-n3-exa-1 .statement}

Nếu F có hạng 1 tại mọi điểm, thì F là khả tích, và xác định trên X một lá thuần nhất chiều 1. Giả sử thêm rằng $K = \mathbf{R}$, rằng X là tách được, và rằng F có một trường vectơ $\xi$ làm khung, khác không khắp nơi. Khi đó, với mọi $x \in X$, lá liên thông cực đại chứa $x$ là ảnh của cung nguyên cực đại của $\xi$ với gốc $x$ (9.1.3).

9.3.3 (« Các tiêu chuẩn khả tích »). Các điều kiện sau là tương đương:

(i) Bó con vectơ F của $T(X)$ là khả tích.

(ii) Với mọi $x \in X$, tồn tại một đa tạp con nguyên Z lớp $C^s$ của F sao cho $x \in Z$ và $T_x(Z) = F_x$.

(iii) Với mọi tập mở U của X và các trường vectơ $\xi$ và $\eta$ thuộc về $\mathscr{J}_F^s(U)$ (7.4.1), ta có $[\xi, \eta] \in \mathscr{J}_F^{s-1}(U)$.

Cho $(\xi_i)_{i \in I}$ là một họ các mặt cắt của F lớp $C^s$ sao cho, với mọi $x \in X$, tập hợp các $\xi_i(x)$ là một tập con toàn phần của không gian Banach $F_x$ (EVT, I, § 2, No. 1). Khi đó các điều kiện (i), (ii), (iii) tương đương với:

(iv) với mọi cặp $(i, j)$ các phần tử của I, và mọi $x \in X$, ta có $[\xi_i, \xi_j](x) \in F_x$.

Khi I là hữu hạn, và họ $(\xi_i)$ là một khung của F, các điều kiện trước đó cũng tương đương với:

(v) tồn tại một họ $(c_{ij}^k)_{(i, j, k) \in I \times I \times I}$ các hàm trên X với giá trị trong K sao cho $[\xi_i, \xi_j] = \sum_k c_{ij}^k \xi_k$ với mọi $i, j$ trong I.

(Nếu trường hợp này xảy ra, các hàm $c_{i,j}^k$ là lớp $C^{s-1}$.)

9.3.4. Cho $s' \in \mathbf{N}_K$, với $s' \leq s$, và cho $F'$ là bó vectơ lớp $C^{s'}$ suy ra từ F bởi sự làm yếu cấu trúc (8.7.1). Để F là khả tích, điều kiện cần và đủ là $F'$ cũng như vậy. Trong trường hợp này, lá nguyên của $F'$ được suy ra từ lá nguyên của F bởi sự làm yếu cấu trúc.

9.3.5. Cho E là một không gian Banach và $p$ là một số nguyên $\geq 0$. Với mỗi $x \in X$, ta ký hiệu

N(p, E)_x là không gian con vectơ của Alt^p(T_x(X); E) được tạo bởi các phần tử u sao cho $u(v_1, \ldots, v_p) = 0$ đối với $v_1, \ldots, v_p$ trong $F_x$. Các không gian N(p, E)_x, với $x \in X$, là các thớ của một phân cấu con vectơ thuộc lớp C^s của Alt^p(T(X); E). Ta ký hiệu nó là N(p, E). Nếu F khả tích, ta có:

(vi) với mọi tập mở U của X và mọi dạng $\omega \in \mathscr{S}_{N(p, E)}^s(U)$, ta có $d\omega \in \mathscr{S}_{N(p+1, E)}^{s-1}(U)$.

Ngược lại, nếu (vi) được thỏa mãn với $p = 1$ và với mọi không gian Banach E, thì phân bó F là khả tích; khi K = R hoặc C, thậm chí chỉ cần kiểm tra (vi) với $p = 1$ và E = K.

Giả sử rằng đối ngẫu của T(X)/F thừa nhận một khung $(\omega_1, \ldots, \omega_n)$. Khi đó tính khả tích của F tương đương với điều kiện sau:

(vii) $d\omega_i \wedge \omega_1 \wedge \cdots \wedge \omega_n = 0$ với $1 \leq i \leq n$.

Nếu ngoài ra tồn tại một phân cấu con vectơ G thuộc lớp C^s của T(X) sao cho T(X) là tổng trực tiếp của F và G, điều kiện (vii) tương đương với:

(viii) tồn tại các dạng vi phân $\alpha_i^j$ (i, j trong I) bậc 1 trên X, thuộc lớp C^{s-1}, sao cho $d\omega_i = \sum_j \alpha_i^j \wedge \omega_j$ với mọi $i \in I$.

9.3.6. Cho L là một không gian Banach và cho $\omega$ là một dạng vi phân bậc 1 trên X với các giá trị trong L, thuộc lớp C^s. Ta đặt ra hai giả thiết sau:

a) với mọi $x \in X$, $\omega_x$ là một đồng cấu toàn ánh từ $T_x(X)$ vào L, và hạt nhân của $\omega_x$ là $F_x$;
b) tồn tại một phân cấu con vectơ G của T(X) sao cho T(X) là tổng trực tiếp của F và G.

Khi đó tính khả tích của F tương đương với:

(ix) tồn tại một dạng vi phân $\alpha$ bậc 1 trên X với các giá trị trong End(L) sao cho $d\omega = \alpha \wedge \omega$, tích ngoài được xác định bởi phép ghép cặp chính tắc End(L) $\times$ L $\to$ L (7.8.2 và 8.3.2).

9.3.7 (« Các phương trình trong các vi phân toàn phần »). Giả sử rằng X là tích của hai đa tạp A và B thuộc lớp C^r; ký hiệu $p_1 : X \to A$ và $p_2 : X \to B$ là hai phép chiếu. Cho f là một cấu xạ thuộc lớp C^s từ $p_1^*T(A)$ vào $p_2^*T(B)$. Các đồ thị của các ánh xạ $f_{(a, b)} : T_a(A) \to T_b(B)$ là các thớ của một phân cấu con vectơ thuộc lớp C^s của T(X); ký hiệu nó là F^f.

Cho A’ là một tập con mở của A, và cho $\varphi : A' \to B$ là một cấu xạ thuộc lớp C^k ($k \in \mathbf{N}_K, k \leq r$). Ta nói rằng $\varphi$ là một tích phân của f nếu, với mọi $a \in A'$, ta có $T_a(\varphi) = f_{a, \varphi(a)}$; điều này tương đương với việc nói rằng ánh xạ $a \mapsto (a, \varphi(a))$ từ A’ vào X là một tích phân của F^f (9.3.1). Một ánh xạ như vậy thuộc lớp C^{s+1}. Nếu $\varphi_1$ và $\varphi_2$ là hai tích phân của f và nhận cùng một giá trị tại một điểm $a \in A$, chúng trùng nhau trong một lân cận của a.

Tổng quát hơn, cho Z là một đa tạp thuộc lớp C^k, cho A’ là một tập con mở của A, cho $a \in A'$ và cho $\Phi_1, \Phi_2$ là các cấu xạ thuộc lớp C^k từ Z $\times$ A’ vào B. Giả sử rằng

Φ₁ và Φ₂ trùng nhau trên Z × {a} và rằng, với mọi z ∈ Z, các cấu xạ
$$
a \mapsto \Phi_1(z, a) \quad \text{và} \quad a \mapsto \Phi_2(z, a)
$$
là các tích phân của f. Khi đó Φ₁ và Φ₂ trùng nhau trong một lân cận của Z × {a}.

Giả sử rằng F^f là khả tích. Cho Z là một đa tạp thuộc lớp C^k (k ∈ N_K, k ≤ s), cho $(z₀, a₀)$ là một điểm của Z × A, và cho ρ là một cấu xạ thuộc lớp C^k từ Z vào B. Tồn tại một lân cận mở Z' × A' của (z₀, a₀) trong Z × A và một cấu xạ Φ : Z' × A' → B thuộc lớp C^k sao cho, với mọi z ∈ Z', ánh xạ a ↦ Φ(z, a) từ A' vào B có f làm ánh xạ tiếp xúc của nó và nhận giá trị ρ(z) tại điểm a₀.

9.3.8. Giữ lại các giả thiết và ký hiệu của 9.3.7 và giả sử rằng A (tương ứng B) là một đa tạp con mở của một không gian Banach E (tương ứng M). Khi đó ánh xạ f được đồng nhất với một cấu xạ thuộc lớp C^s từ X = A × B vào không gian Banach $\mathscr{L}(E; M)$. Ký hiệu D₁f (tương ứng D₂f) là đạo hàm riêng thứ nhất (tương ứng thứ hai) của f (1.6.2); đây là một cấu xạ thuộc lớp C^{s-1} từ X vào $\mathscr{L}(E; \mathscr{L}(E; M))$ (tương ứng vào $\mathscr{L}(M; \mathscr{L}(E; M))$), một không gian được đồng nhất theo cách hiển nhiên với $\mathscr{L}_2(E; M)$ (tương ứng với $\mathscr{L}(M, E; M)$). Để F khả tích, điều kiện cần và đủ là, với mọi x ∈ X, ánh xạ song tuyến tính
$$
\Delta_x : (h_1, h_2) \mapsto D_1f(x)(h_1, h_2) + D_2f(x)(f(x)h_1, h_2)
$$
từ E × E vào M là đối xứng. Dưới điều kiện này, nếu φ là một tích phân của f được xác định trong một tập con mở A' của A, đạo hàm thứ hai của φ tại một điểm a của A' là $\Delta_{(a, \varphi(a))}$.

Nếu E = K^n, và nếu ta ký hiệu bởi (x¹, ..., xⁿ) các hàm tọa độ trên K^n, ánh xạ f được xác định bởi một họ (f₁, ..., fₙ) các ánh xạ từ A × B vào M, và điều kiện khả tích được viết:
$$
\frac{\partial f_i}{\partial x^j} + (D_2f_i) \cdot f_j = \frac{\partial f_j}{\partial x^i} + (D_2f_j) \cdot f_i
$$
với mọi số nguyên i, j trong {1, n}. Một ánh xạ φ từ một tập con mở A' của A vào B là một tích phân của f khi và chỉ khi có
$$
\frac{\partial \varphi}{\partial x^i} = f_i(x, \varphi(x)) \quad \text{với mọi } x \in A' \text{ và mọi } i \in \{1, n\},
$$
nói cách khác, khi có
$$
d\varphi = \sum_{1 \leq i \leq n} f_i(x, \varphi(x)) \, dx^i.
$$

### 9.4. Các phân bó khả tích trong đặc số p ≠ 0

Trong số này, K được giả sử có đặc số p ≠ 0. Cho X là một đa tạp K-phân tích địa phương có số chiều hữu hạn.

9.4.1 (« Lũy thừa p »). Cho ξ là một trường vectơ trên một tập con mở U của X. Tồn tại duy nhất một trường vectơ ξ^p trên U sao cho
$$
D_{\xi^p}(f) = (D_\xi)^p(f) = \underbrace{D_\xi(D_\xi(\ldots(D_\xi(f))\ldots))}_{p \text{lần}}
$$
với mọi hàm phân tích f được xác định trên một tập con mở của U.

Nếu $\varphi$ là một hàm giải tích trên $U$, ta có
$$
(\varphi \xi)^p = \varphi^p \xi^p + (\mathrm{D}_{\varphi \xi})^{p-1}(\varphi) \cdot \xi
$$
và nếu $\eta$ là một trường vectơ trên $U$, ta có
$$
[\xi^p, \eta] = \mathrm{ad}(\xi)^p(\eta) = [\xi, [\xi, \ldots, [\xi, \eta]\ldots]].
$$

9.4.2 (« Đồng nhất thức Jacobson »). Cho $L$ là đại số Lie $F_p$ tự do (LIE, II, § 2, No. 2) trên một tập hợp $\{x, y\}$ có hai phần tử. Tồn tại một và chỉ một phần tử $\Lambda_p(x, y)$ của $L$ sao cho ta có
$$
(x + y)^p = x^p + y^p + \Lambda_p(x, y)
$$
trong đại số bao quanh của $L$. Ví dụ:
$$
\Lambda_2(x, y) = [x, y]; \quad \Lambda_3(x, y) = [x, [x, y]] - [y, [x, y]].
$$
Nếu $\xi$ và $\eta$ là các trường vectơ trên $X$, ta có
$$
(\xi + \eta)^p = \xi^p + \eta^p + \Lambda_p(\xi, \eta).
$$

9.4.3. *Ví dụ.* — Lấy $X = K$ (resp. $K^*$) và ký hiệu $x$ là ánh xạ chính tắc $X \to K$. Cho $\xi$ (resp. $\eta$) là trường vectơ $\partial / \partial x$ (resp. $x \cdot \partial / \partial x$); nó là bất biến dưới các phép tịnh tiến của nhóm cộng tính (resp. nhân tính) $X$. Ta có
$$
\xi^p = 0 \quad \text{và} \quad \eta^p = \eta.
$$

9.4.4 (« Bó khả tích »). Cho $F$ là một bó con vectơ của $T(X)$. Ta nói rằng $F$ là *khả tích* nếu, với mọi $x \in X$, tồn tại một hệ tọa độ $(\zeta^1, \ldots, \zeta^n)$ của $X$ tại $x$ và một số nguyên $m \leq n$ sao cho $(\partial / \partial \zeta^1, \ldots, \partial / \partial \zeta^m)$ là một cơ sở của $F$ trong một lân cận của $x$.
Để $F$ khả tích, điều kiện cần và đủ là nó thỏa mãn điều kiện sau:
*Với mọi tập mở $U$ của $X$, $\mathscr{S}_F^\omega(U)$ là một đại số con Lie của $\mathscr{S}_{T(X)}^\omega(U)$ ổn định dưới phép toán $\xi \mapsto \xi^p$.*
