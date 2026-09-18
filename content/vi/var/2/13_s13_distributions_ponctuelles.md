---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 13
section_title: Distributions ponctuelles
lang: vi
source: var-fr
pdf_pages: 0152-0161
extraction: ocr
subsections:
    - "no": 1
      title: Tenseurs symétriques et espaces de Banach
      page: 0
      pdf_page: 152
    - "no": 2
      title: Distributions ponctuelles
      page: 0
      pdf_page: 153
    - "no": 3
      title: Distributions ponctuelles et espaces tangents
      page: 0
      pdf_page: 156
    - "no": 4
      title: Produit tensoriel de distributions ponctuelles
      page: 0
      pdf_page: 157
    - "no": 5
      title: Coproduits
      page: 0
      pdf_page: 159
    - "no": 6
      title: Distributions à support fini
      page: 0
      pdf_page: 160
    - "no": 7
      title: Affaiblissement de structure
      page: 0
      pdf_page: 161
statements: 0
exercises: 0
content_sha256: 3e61e06b81ee8231852e7d2b92278cbf541c2bd53267cf0e299f437e1c2808c1
translated_from: content/en-mt/var/2/13_s13_distributions_ponctuelles.md
source_lang: en-mt
translation_method: machine
source_content_sha256: c08a2c7e88efd6da15237d6acfbddbe178e993d69a8ca0743673273708ddd20c
translation_model: gpt-5-6
translation_run: translate-vi-27fbaee9
glossary_version: 34
glossary_terms_sha256: 013cd83ef0a92ed0fb189b0770b22d31a935bdb23ff52bfdb0d314703e94927f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 13. Phân bố điểm

### 13.1. Tenxơ đối xứng và không gian Banach

### 13.1.1. Cho E là một môđun trên một vành giao hoán A. Nếu n là một số nguyên $\geq 0$, ký hiệu $TS^n(E)$ là môđun của các tenxơ đối xứng hạng n của E (A, III, p. 71 và A, IV, § 5, no 2); tổng trực tiếp của các $TS^n(E)$ được ký hiệu là $TS(E)$. Nếu r là một số nguyên, một trong các ký hiệu $\infty,\omega$, đặt

$$
TS^{(r)}(E)=\bigoplus_{n\leq r}TS^n(E)\quad\text{và}\quad TS^{(r)+}(E)=\bigoplus_{1\leq n\leq r}TS^n(E);
$$

do đó, nếu $r\geq 0$, $TS^{r}(E)$ là tổng trực tiếp của $TS^{(0)}(E)=A$ và của $TS^{(r)+}(E)$. Ta có $TS^{(1)+}(E)=E$ và $TS^{(\infty)}(E)=TS^{(\omega)}(E)=TS(E)$.

Nếu $n$ là một số nguyên $\geq 0$, và nếu $x\in E$, ký hiệu $\gamma_n(x)$ là phần tử $x\otimes\cdots\otimes x$ của $TS^n(E)$; với $n=0$, $\gamma_0(x)=1$.

### 13.1.2. (« Các ánh xạ đa thức »). Giả sử rằng A là nguyên vô hạn và rằng E là một A-môđun tự do. Cho F là một A-môđun. Một ánh xạ $f:E\rightarrow F$ được gọi là đa thức thuần nhất bậc n nếu nó thỏa mãn các điều kiện tương đương sau đây (xem A, IV, § 5, no 9):

a) Tồn tại một ánh xạ tuyến tính $\tilde f:TS^n(E)\rightarrow F$ sao cho $f(x)=\tilde f(\gamma_n(x))$ với mọi $x\in E$.

b) Tồn tại một ánh xạ đa tuyến tính $u:E^n\rightarrow F$ sao cho $f(x)=u(x,\ldots,x)$ với mọi $x\in E$.

Giả sử trường hợp này xảy ra. Ánh xạ $\tilde f$ thỏa mãn a) khi đó là duy nhất; nếu $t\in TS^n(E)$, ký hiệu $\langle f,t\rangle$ là phần tử $\tilde f(t)$. Nếu $u:E^n\rightarrow F$ thỏa mãn b), ánh xạ tuyến tính tương ứng của $\otimes^nE$ vào F trùng với nó trong môđun con $TS^n(E)$. Khi $n!$ khả nghịch trong A, người ta có thể chọn u đối xứng, và việc này theo một cách duy nhất.

### 13.1.3. Cho E là một không gian Banach trên K và F là một không gian đa thức tách được trên K. Cho U là một lân cận mở của 0 trong E, $f:U\rightarrow F$ là một ánh xạ thuộc lớp $C^r$ ($r\in\mathbf{N}_K$), và $t$ là một phần tử của $TS^{(r)}(E)$, xem 13.1.1 (áp dụng cho vành $A=K$). Cho $k$ là một số nguyên $\leq r$ sao cho $t\in TS^{(k)}(E)$. Ta có thể phân tích duy nhất $t$ và $f$ thành

$$
t=t_0+\cdots+t_k,\qquad \text{với }t_i\in TS^i(E)
$$

và

$$
f=f_0+\cdots+f_k+h,
$$

trong đó $f_i$ là một đa thức liên tục thuần nhất bậc $i$ ($0 \leq i \leq k$) và trong đó $h$ có tiếp xúc cấp $\geq k$ với 0 tại điểm 0. Khi đó đặt

$$
\langle f, t \rangle = \sum_{i=0}^{k} \langle f_i, t_i \rangle;
$$

đây là một phần tử của F không phụ thuộc vào lựa chọn $k$.

13.1.4. Cho E và E’ là hai không gian Banach, U là một lân cận mở của 0 trong E và $\varphi : U \to E'$ là một ánh xạ lớp $C^r$ sao cho $\varphi(0) = 0$. Cho $t \in TS^{(r)}(E)$. Tồn tại duy nhất một phần tử $t' \in TS^{(r)}(E')$ sao cho, với mọi không gian đa chuẩn tách được F, mọi lân cận mở U’ của 0 trong E’, và mọi ánh xạ $f : U' \to F$ lớp $C^r$, ta có

(*) $$
\langle f, t' \rangle = \langle f \circ \varphi, t \rangle.
$$

Phần tử $t'$ này được ký hiệu là $\varphi_*(t)$. Ánh xạ

$$
\varphi_* : TS^{(r)}(E) \to TS^{(r)}(E')
$$

được xác định như vậy là tuyến tính.

### 13.2. Phân bố tại điểm

Trong No. này, X ký hiệu một đa tạp lớp $C^r$, và $x$ là một điểm của X.

13.2.1. Cho $\mathscr{A}$ là tập hợp các cặp $(c, t)$, trong đó $c = (U, \varphi, E)$ là một biểu đồ của X tâm tại $x$, và $t \in TS^{(r)}(E)$. Hai phần tử $((U, \varphi, E), t)$ và $((U', \varphi', E'), t')$ của $\mathscr{A}$ được gọi là tương đương nếu $t' = \gamma_*(t)$, trong đó $\gamma = \varphi' \circ \varphi^{-1}$. Theo cách này ta được một quan hệ tương đương trên $\mathscr{A}$; một lớp tương đương đối với quan hệ này được gọi là một phân bố tại điểm $x$ trên X.

Gọi $T_x^{(r)}(X)$ là tập hợp các phân bố tại điểm $x$ trên X. Nếu $c$ là một biểu đồ của X tâm tại $x$, ánh xạ

$$
\theta_c : TS^{(r)}(E) \to T_x^{(r)}(X)
$$

gán cho $t$ lớp của $(c, t)$ là một song ánh. Trong tất cả những gì sau đây, $T_x^{(r)}(X)$ được trang bị cấu trúc của một không gian vectơ trên K thu được bằng cách chuyển cấu trúc của $TS^{(r)}(E)$ qua $\theta_c$; cấu trúc này không phụ thuộc vào lựa chọn $c$. Tương tự, nếu $k \leq r$, $T_x^{(k)}(X)$ và $T_x^{(k)+}(X)$ ký hiệu các ảnh của $TS^{(k)}(E)$ và $TS^{(k)+}(E)$ qua $\theta_c$; chúng không phụ thuộc vào lựa chọn $c$. Một phần tử của $T_x^{(r)}(X)$ được gọi là có cấp $\leq k$ nếu nó thuộc $T_x^{(k)}(X)$. Ta có

$$
T_x^{(k)}(X) = T_x^{(0)}(X) \oplus T_x^{(k)+}(X).
$$

Tồn tại duy nhất một phần tử $\varepsilon_x$ của $T_x^{(0)}(X)$ sao cho $\theta_c(1) = \varepsilon_x$ với mọi biểu đồ $c$ của X tâm tại $x$. Nếu $t$ là một phân bố tại điểm $x$, số hạng hằng của $t$ là phần tử $\lambda$ của K sao cho $t - \lambda \varepsilon_x \in T_x^{(r)+}(X)$; ta nói rằng $t$ không có số hạng hằng nếu số hạng hằng của nó bằng không.

13.2.2. Cho F là một không gian đa chuẩn tách được, và cho $f$ là một hàm thuộc lớp $C^r$ với các giá trị trong F, được xác định trên một lân cận của $x$. Cho $t$ là một phân bố có giá tại $x$ trên X.

Xét một biểu đồ $c = (U, \varphi, E)$ của $X$ lấy $x$ làm tâm, và đặt $f_c = f \circ \varphi^{-1}$ và $t_c = \theta_c^{-1}(t)$; phần tử $\langle f_c, t_c \rangle$ của $F$ được xác định trong 13.1.3 không phụ thuộc vào lựa chọn $c$; ta ký hiệu nó bởi $\langle f, t \rangle$. Ta có $\varepsilon_x(f) = f(x)$.¹ Số hạng hằng của $t$ là $\langle 1, t \rangle$.

Nếu $F'$ là một không gian đa chuẩn tách được và nếu $u : F \to F'$ là ánh xạ tuyến tính liên tục, ta có $\langle u \circ f, t \rangle = u(\langle f, t \rangle)$.

Giả sử rằng $F$ là một không gian Banach, và rằng $t$ có cấp $\leq k$, với $k$ hữu hạn. Cho $j \in J_x^k(X, F)$, cf. 12.1.2, và cho $f \in j$. Khi đó $\langle f, t \rangle$ chỉ phụ thuộc vào jet $j$; ta ký hiệu nó bởi $\langle j, t \rangle$. Ánh xạ từ $T_x^{(k)}(X) \times J_x^k(X, F)$ vào $F$ được xác định như vậy là song tuyến tính. Khi $F = K$, ta đã đặt $J_x^k(X, F) = P_x^k(X)$, cf. 12.6.2, và ta thu được một *dạng song tuyến tính* trên $T_x^{(k)}(X) \times P_x^k(X)$.

13.2.3. Cho $\varphi : X \to Y$ là một cấu xạ giữa các đa tạp thuộc lớp $C^r$ và cho $y = \varphi(x)$. Cho $c = (U, \psi, E)$ là một biểu đồ của $X$ lấy $x$ làm tâm và cho $c' = (U', \psi', E')$ là một biểu đồ của $Y$ lấy $y$ làm tâm; cho $\tilde{\varphi}$ là biểu thức của $\varphi$ trong các biểu đồ này (5.3.2), và cho $\tilde{\varphi}_*$ là ánh xạ tương ứng từ $TS^{(r)}(E)$ vào $TS^{(r)}(E')$, cf. 13.1.4. Tồn tại duy nhất một ánh xạ tuyến tính, ký hiệu bởi $T_x^{(r)}(\varphi)$ hoặc $\varphi_*$, từ $T_x^{(r)}(X)$ vào $T_y^{(r)}(Y)$, làm cho biểu đồ sau giao hoán

$$
\begin{array}{ccc}
TS^{(r)}(E) & \xrightarrow{\tilde{\varphi}_*} & TS^{(r)}(E') \\
\downarrow_{\theta_c} & & \downarrow_{\theta_c} \\
T_x^{(r)}(X) & \xrightarrow{\varphi_*} & T_y^{(r)}(Y).
\end{array}
$$

Ánh xạ này không phụ thuộc vào lựa chọn của $c$ và $c'$. Nếu $t \in T_x^{(r)}(X)$, $\varphi_*(t)$ được gọi là *ảnh* của $t$ qua $\varphi$. Ta có $\varphi_*(\varepsilon_x) = \varepsilon_y$. Nếu $k \leq r$, ta có
$$
\varphi_*(T_x^{(k)}(X)) \subset T_y^{(k)}(Y) \quad \text{và} \quad \varphi_*(T_x^{(k)+}(X)) \subset T_y^{(k)+}(Y).
$$

Nếu $\varphi' : X \to Y$ là một cấu xạ lớp $C^r$ ánh xạ $x$ lên $y$, ta có $\varphi_* = \varphi'_*$ khi và chỉ khi $j_x^r(\varphi) = j_x^r(\varphi')$, cf. 12.1.

Nếu $\varphi$ là một phép nhúng (tương ứng. một phép ngập) tại $x$, $\varphi_*$ là đơn ánh (tương ứng. toàn ánh); đảo lại đúng nếu $\dim_y Y < +\infty$.

Nếu $\varphi' : Y \to Z$ là một cấu xạ của các đa tạp $C^r$, và nếu $t \in T_x^{(r)}(X)$, ta có $(\varphi' \circ \varphi)_*(t) = \varphi'_*(\varphi_*(t))$.

Cho $F$ là một không gian đa chuẩn tách được, và cho $f$ là một hàm lớp $C^r$ với các giá trị trong $F$, được xác định trong một lân cận của $y$. Khi đó ta có
$$(1)$$
$$
\langle f, \varphi_*(t) \rangle = \langle f \circ \varphi, t \rangle \quad \text{với mọi } t \in T_x^{(r)}(X).
$$
Với $t$ đã cho, các hệ thức (1) (đối với biến $f$ và $F$) *đặc trưng* cho $\varphi_*(t)$; khi $\dim_y Y < +\infty$, ta có thể hạn chế về $F = K$.

13.2.4. Giả sử rằng $X$ là một đa tạp con mở của một *không gian Banach* $E$. Ký hiệu $\varphi_x$ là ánh xạ $y \mapsto y - x$ của $X$ vào $E$; biểu đồ $c = (X, \varphi_x, E)$ được lấy tâm

¹ Khi $K = \mathbf{R}$ hoặc $\mathbf{C}$ và $X$ là compact địa phương, công thức trước dẫn đến việc đồng nhất phân bố điểm $\varepsilon_x$ với *độ đo Dirac* $\varepsilon_x$ được định nghĩa trong JNT, III, § 1, No. 3. Nói chung hơn, mọi độ đo có giá hữu hạn trong $X$ đều được đồng nhất với một phân bố có giá hữu hạn theo nghĩa của No. 13.6.

tại $x$. Khi đó ta đồng nhất $T_x^{(r)}(X)$ với $TS^{(r)}(E)$ bằng $\theta_c^{-1}$; đặc biệt, ta có $T_x^{(\infty)}(X) = TS(E)$.

Cho $F$ là một không gian Banach, cho $u : E \to F$ là một ánh xạ tuyến tính liên tục, và cho $x \in E, y \in F$ là sao cho $u(x) = y$. Đồng nhất như trên $T_x^{(\infty)}(E)$ với $TS(E)$ và $T_y^{(\infty)}(F)$ với $TS(F)$. Ánh xạ
$$
u_* : TS(E) \to TS(F) \quad (\text{cf. } 13.2.3)
$$
trùng với ánh xạ $TS(u)$ cảm sinh bởi mở rộng chính tắc của $u$ lên đại số tenxơ.

13.2.5. Nếu $k \leq r$, ký hiệu $T^{(k)}(X)$ (tương ứng $T^{(k)+}(X)$) là tập hợp tổng của các $T_a^{(k)}(X)$ (tương ứng của các $T_a^{(k)+}(X)$) với $a \in X$. Một ánh xạ $t : X \to T^{(k)}(X)$ sao cho $t(a) \in T_a^{(k)}(X)$ với mọi $a \in X$ được gọi là một trường các phân bố điểm có cấp $\leq k$.

Giả sử $k$ hữu hạn và $X$ địa phương có số chiều hữu hạn. Với mọi $a \in X$, dạng song tuyến tính $(j, t) \mapsto \langle j, t \rangle$ (cf. 13.2.2) định nghĩa một đẳng cấu $i_a$ của $T_a^{(k)}(X)$ lên đối ngẫu $P_a^k(X)^*$ của $P_a^k(X)$. Các $i_a$ định nghĩa một song ánh $i : T^{(k)}(X) \to P^k(X)^*$, trong đó $P^k(X)^*$ là đối ngẫu của bó vectơ $P^k(X)$; bằng phép chuyển cấu trúc nhờ $i^{-1}$, ta trang bị cho $T^{(k)}(X)$ một cấu trúc của bó vectơ với cơ sở $X$ và thuộc lớp $C^{r-k}$. Một trường các phân bố điểm có cấp $\leq k$ được gọi là thuộc lớp $C^s$, với $s \leq r - k$, nếu nó là một tiết diện thuộc lớp $C^s$ của bó vectơ $T^{(k)}(X)$.

Cho $\varphi : X \to Y$ là một cấu xạ của các đa tạp thuộc lớp $C^r$ và giả sử rằng $Y$, cũng như $X$, địa phương có số chiều hữu hạn. Khi đó $\varphi_* : T^{(k)}(X) \to T^{(k)}(Y)$ là một $\varphi$-cấu xạ của các bó vectơ thuộc lớp $C^{r-k}$.

13.2.6. Cho $k$ là một số nguyên sao cho $0 \leq k \leq r$. Nếu $U$ là một tập hợp mở của một không gian Banach $E$ có số chiều hữu hạn, bó vectơ $T^{(k)}(U)$ được đồng nhất, nhờ 13.2.4, với bó tầm thường có thớ $TS^{(k)}(E)$.

Đặc biệt lấy $E = K^n$, với $n \geq 0$, và gọi $(e_1, \ldots, e_n)$ là cơ sở chính tắc của $E$. Nếu $\alpha = (\alpha_1, \ldots, \alpha_n)$ là một phần tử của $\mathbf{N}^n$, ký hiệu $\Delta^\alpha$ là phần tử $\gamma_{\alpha_1}(e_1) \ldots \gamma_{\alpha_n}(e_n)$ của $TS(E)$ (tích được sử dụng là tích đối xứng của các tenxơ đối xứng, cf. A, IV, § 5, No. 3).(1) Các $\Delta^\alpha$, với $|\alpha| \leq k$, lập thành một cơ sở của $TS^{(k)}(E)$; nếu $a \in K^n$, ký hiệu $\Delta_a^\alpha$ là các phần tử tương ứng của $T_a^{(k)}(E)$. Cho $F$ là một không gian đa chuẩn tách được, và $f$ là một hàm thuộc lớp $C^r$, với các giá trị trong $F$, được xác định trong một lân cận của $a$; nếu $\alpha \in \mathbf{N}^n$, phần tử $\langle f, \Delta_a^\alpha \rangle$ trùng với phần tử $(\Delta^\alpha f)(a)$ được định nghĩa trong 2.5.3, 3.2.1 và 4.2.1.

Giả sử $X$ có chiều hữu hạn địa phương, và gọi $\xi = (\xi^1, \ldots, \xi^n)$ là một hệ tọa độ của $X$ trong một tập mở $U$. Nếu $a \in U$ và nếu $\alpha$ là một đa chỉ số sao cho $|\alpha| \leq k$, ký hiệu $(\Delta_\xi^\alpha)_a$ là phân bố điểm tại $a$ mà ảnh của nó qua $\xi$ là phân bố điểm $\Delta_{\xi(a)}^\alpha$ trên $K^n$; các trường phân bố
$$
\Delta_\xi^\alpha : a \mapsto (\Delta_\xi^\alpha)_a \quad (|\alpha| \leq k)
$$
lập thành một khung trên $U$ của bó vectơ $T^{(k)}(X)$. Nếu $f : U \to F$ thuộc lớp $C^r$, đặt $\langle f, (\Delta_\xi^\alpha)_a \rangle = \Delta_\xi^\alpha f(a)$ và ký hiệu $\Delta_\xi^\alpha f$ là hàm $a \mapsto \Delta_\xi^\alpha f(a)$; đây là một hàm thuộc lớp $C^{r-k}$ trong $U$.

(1) Nếu $m = |\alpha|$ và nếu $\Sigma$ là tập hợp các ánh xạ $\sigma$ của $\{1, \ldots, m\}$ vào $\{1, \ldots, n\}$ sao cho $\mathrm{Card}\, \sigma^{-1}(i) = \alpha_i$, ta có
$$
\Delta^\alpha = \gamma_{\alpha_1}(e_1) \ldots \gamma_{\alpha_n}(e_n) = \sum_{\sigma \in \Sigma} e_{\sigma(1)} \otimes \cdots \otimes e_{\sigma(n)}, \quad \text{cf. A, IV, § 5, n° 4.}
$$

### 13.3. Phân bố điểm và không gian tiếp xúc

Trong No. này, $X$ ký hiệu một đa tạp thuộc lớp $C^r$.

### 13.3.1. Cho $x \in X$ và cho $k$ là một số nguyên $\leq r$. Cho $c=(U,\varphi,E)$ là một biểu đồ của $X$ có tâm tại $x$; đẳng cấu $\theta_c:T^S(X)(E)\to T_x(X)$ được định nghĩa trong 13.2.1 ánh xạ $T^S{}^{(k)}(E)$ lên $T_x^{(k)}(X)$ và $T^S{}^{(k-1)}(E)$ lên $T_x^{(k-1)}(X)$; bằng hạn chế và chuyển qua thương, nó cảm sinh một đẳng cấu

$$
\theta_{c,k}:T^S{}^{(k)}(E)=T^S{}^{(k)}(E)/T^S{}^{(k-1)}(E)\longrightarrow T_x^{(k)}(X)/T_x^{(k-1)}(X).
$$

Mặt khác, $c$ định nghĩa một đẳng cấu, đã được ký hiệu là $\theta_c$, từ $E$ lên không gian tiếp xúc $T_x(X)$, xem 5.5.1. Gọi $i_k$ là ánh xạ hợp thành

$$
T_x^{(k)}(X)/T_x^{(k-1)}(X)\xrightarrow{\theta_{c,k}^{-1}}T^S{}^{(k)}(E)\xrightarrow{T^S(\theta_c)}T^S{}^{(k)}(T_x(X)).
$$

Đẳng cấu $i_k$ là độc lập với lựa chọn $c$; với $k=1$, nó được dùng để đồng nhất $T_x^{(1)}(X)=T_x^{(1)}(X)/T_x^{(0)}(X)$ với không gian tiếp xúc $T_x(X)$. Nếu $t\in T_x^{(k)}(X)$, ta cho phép mình ký hiệu $i_k(t)$ là ảnh qua $i_k$ của lớp của $t$ modulo $T_x^{(k-1)}(X)$.

Đặt

$$
\operatorname{gr}_k T_x^{(r)}(X)=T_x^{(k)}(X)/T_x^{(k-1)}(X)
$$

và

$$
\operatorname{gr}T_x^{(r)}(X)=\bigoplus_{0\leq k\leq r}\operatorname{gr}_k T_x^{(r)}(X).
$$

Ta nói rằng $\operatorname{gr}T_x^{(r)}(X)$ là phân bậc liên kết với lọc tăng $(T_x^{(k)}(X))_{k\leq r}$ của $T_x^{(r)}(X)$. Các $i_k$ xác định một đẳng cấu của các không gian vectơ phân bậc

$$
i:\operatorname{gr}T_x^{(r)}(X)\longrightarrow T^S{}^{(r)}(T_x(X)).
$$

Nếu $r=\infty$ hoặc $\omega$, $i$ là một đẳng cấu từ $\operatorname{gr}T_x^{(r)}(X)$ lên $T^S(T_x(X))$. Khi muốn chỉ rõ $x$ (hoặc $X$, hoặc cả hai), người ta viết $i_x$ (hoặc $i_X$, hoặc $i_{x,X}$) thay cho $i$.

### 13.3.2. Ngoài các giả thiết trên, giả sử rằng $X$ là hữu hạn chiều địa phương. Các đẳng cấu $i_k$ tương ứng với các điểm khác nhau của $X$ xác định một đẳng cấu của các bó vectơ

$$
i_k:T^{(k)}(X)/T^{(k-1)}(X)\longrightarrow TS^{(k)}(T(X))
$$

trong đó $TS^{(k)}(T(X))$ ký hiệu bó vectơ lớp $C^{r-1}$ nhận được từ $T(X)$ bởi hàm tử vectơ hữu hạn chiều $TS^{(k)}$ (xem 7.6.5). Với $k\geq 1$, $i_k$ là một đẳng cấu lớp $C^{r-k}$; với $k=0$, nó là ánh xạ đồng nhất của bó tầm thường $K_X$.

### 13.3.3. **Ví dụ.** — Với các giả thiết như trên, cho $\xi=(\xi^1,\ldots,\xi^n)$ là một hệ tọa độ của $X$ tại $x$. Cho $(\partial_i)_{1\leq i\leq n}$ là cơ sở của $T_x(X)$ được xác định bởi $\xi$ (xem 5.5.8) và cho $(\Delta^\alpha_x)_{|\alpha|\leq k}$ là cơ sở của $T_x^{(k)}(X)$ được xác định trong 13.2.6. Ta có:

$$
i_k(\Delta^\alpha_x)=0 \qquad \text{nếu } |\alpha|<k
$$

$$
i_k(\Delta^\alpha_x)=\gamma_{\alpha_1}(\partial_1,x)\cdots\gamma_{\alpha_n}(\partial_n,x)
\qquad \text{nếu } |\alpha|=k.
$$

[^1]

13.3.4. Giả sử rằng K có đặc số không hoặc X có số chiều hữu hạn địa phương. Cho k là một số nguyên sao cho $0 \leq k \leq r$ và cho $x \in X$; cho F là một không gian Banach. Theo 12.6.8, ta có một dãy khớp

(i)
$$
0 \to P_k(T_x(X); F) \xrightarrow{i} P_x^k(F_X) \xrightarrow{\sigma} P_x^{k-1}(F_X) \to 0,
$$
với $\sigma = r^{k, k-1}$. Mặt khác, theo 13.3.1, ta có một dãy khớp

(ii)
$$
0 \leftarrow TS^k(T_x(X)) \xleftarrow{i} T_x^{(k)}(X) \xleftarrow{s} T_x^{(k-1)}(X) \leftarrow 0,
$$
trong đó s là phép nhúng của $T_x^{(k-1)}(X)$ vào $T_x^{(k)}(X)$ và $i = i_k$. Các dãy khớp này được “liên kết trong F”. Chính xác hơn, viết chúng dưới dạng:

(i)
$$
0 \to A \xrightarrow{i} B \xrightarrow{\sigma} C \to 0
$$

(ii)
$$
0 \leftarrow A' \xleftarrow{i} B' \xleftarrow{s} C' \leftarrow 0.
$$

Nếu $a \in A$ và $a' \in A'$, phần tử $\langle a, a' \rangle$ của F được xác định bởi 13.1.2; nếu $b \in B$ và $b' \in B'$ (tương ứng, nếu $c \in C$ và $c' \in C'$), phần tử $\langle b, b' \rangle$ (tương ứng $\langle c, c' \rangle$) của F được xác định bởi 13.2.2; khi đó ta có:
$$
\langle ia, b' \rangle = \langle a, ib' \rangle \quad \text{và} \quad \langle \sigma b, c' \rangle = \langle b, sc' \rangle \quad \text{nếu} \quad a \in A,\ b \in B,\ b' \in B',\ c' \in C'.
$$

13.3.5. Cho Y là một đa tạp thuộc lớp $C^r$, cho $\varphi : X \to Y$ là một cấu xạ thuộc lớp $C^r$ và cho $x \in X,\ y \in Y$ sao cho $y = \varphi(x)$. Ánh xạ $\varphi_* : T_x^{(r)}(X) \to T_y^{(r)}(Y)$ được xác định trong 13.2.3 là tương thích với các lọc của các không gian này; nó xác định, bằng cách chuyển qua các không gian phân bậc liên kết, một ánh xạ tuyến tính
$$
\operatorname{gr}(\varphi_*) : \operatorname{gr}\ T_x^{(r)}(X) \to \operatorname{gr}\ T_y^{(r)}(Y).
$$
Mặt khác, cho $TS^{(r)}(T_x(\varphi))$ là ánh xạ của $TS^{(r)}(T_x(X))$ vào $TS^{(r)}(T_y(Y))$ cảm sinh bởi mở rộng chính tắc $TS(T_x(\varphi))$ của $T_x(\varphi)$. Biểu đồ

$$
\begin{array}{ccc}
\operatorname{gr}\ T_x^{(r)}(X) & \xrightarrow{\operatorname{gr}(\varphi_*)} & \operatorname{gr}\ T_y^{(r)}(Y) \\
\downarrow^{i_{X,x}} & & \downarrow^{i_{Y,y}} \\
TS^{(r)}(T_x(X)) & \xrightarrow{TS^{(r)}(T_x(\varphi))} & TS^{(r)}(T_y(Y))
\end{array}
$$

là giao hoán.

13.3.6. Giả sử rằng K có đặc số không. Sử dụng các đẳng cấu $\varphi_M : S^k(M) \to TS^k(M)$ được xác định trong A, IV, § 5, No. 8, ta có thể thay thế, trong tất cả những điều đã nêu trước đây, $TS^k(T_x(X))$ bởi các lũy thừa đối xứng thứ k $S^k(T_x(X))$ của không gian tiếp xúc $T_x(X)$.

### 13.4. Tích tenxơ của các phân phối điểm

13.4.1. Cho $X_1$ và $X_2$ là hai đa tạp thuộc lớp $C^r$, cho $x_1 \in X_1,\ x_2 \in X_2$ và $t_1 \in T_{x_1}^{(k_1)}(X_1),\ t_2 \in T_{x_2}^{(k_2)}(X_2)$ với $k_1 + k_2 \leq r$. Đặt $X = X_1 \times X_2,\ x = (x_1, x_2)$ và k = k_1 + k_2. Với i = 1, 2, cho c_i = (U_i, \varphi_i, E_i) là một biểu đồ của X_i lấy tâm tại x_i và ký hiệu $\tilde{t}_i$ là phần tử của TS(E_i) sao cho $\theta_c(\tilde{t}_i) = t_i$, xem 13.2.1. Cho $\sigma$ là đẳng cấu chính tắc của TS(E_1) $\otimes$ TS(E_2) lên TS(E_1 $\times$ E_2), xem A, IV, § 5, no. 5. Phần tử $\sigma(\tilde{t}_1 \otimes \tilde{t}_2)$ là tích đối xứng của $\tilde{t}_1$ và $\tilde{t}_2$ (được đồng nhất với các phần tử của TS(E_1 $\times$ E_2) nhờ các phép nhúng chính tắc TS(E_i) $\to$ TS(E_1 $\times$ E_2)); nó thuộc TS^{(k)}(E_1 $\times$ E_2). Đặt $c = c_1 \times c_2$; đây là một biểu đồ của X lấy tâm tại x. Ảnh bởi $\theta_c$ của $\sigma(\tilde{t}_1 \otimes \tilde{t}_2)$ là một phần tử của T_x^{(k)}(X), không phụ thuộc vào lựa chọn các biểu đồ $c_i$. Nó được gọi là tích trực tiếp, hoặc tích tenxơ đối xứng (hoặc đơn giản là tích tenxơ) của $t_1$ và $t_2$ và được ký hiệu bởi $t_1 \times t_2$ hoặc $t_1 \otimes t_2$.

Ta có $\varepsilon_{x_1} \otimes \varepsilon_{x_2} = \varepsilon_x$. Số hạng hằng của $t_1 \otimes t_2$ là tích của các số hạng hằng của $t_1$ và $t_2$.

Đẳng cấu $(y_1, y_2) \mapsto (y_2, y_1)$ của $X_1 \times X_2$ lên $X_2 \times X_1$ biến $t_1 \otimes t_2$ thành $t_2 \otimes t_1$.

13.4.2 (« Tính kết hợp và tính hàm tử »). Cho $X_i$ ($i = 1, 2, 3$) là các đa tạp thuộc lớp $C^r$, và cho $x_i \in X_i$, $t_i \in T^{(k_i)}_{x_i}(X_i)$ với $k_1 + k_2 + k_3 \leq r$. Ta có
$$
(t_1 \otimes t_2) \otimes t_3 = t_1 \otimes (t_2 \otimes t_3);
$$
ta ký hiệu phân phối điểm này bởi $t_1 \otimes t_2 \otimes t_3$. Các tích tenxơ hữu hạn với một số bất kỳ các thừa số được định nghĩa tương tự.

Cho $\varphi_1 : X_1 \to Y_1$ và $\varphi_2 : X_2 \to Y_2$ là các đồng cấu của các đa tạp thuộc lớp $C^r$, và cho $t_1 \in T^{(k_1)}(X_1)$, $t_2 \in T^{(k_2)}(X_2)$ với $k_1 + k_2 \leq r$. Ta có
$$
(\varphi_1 \times \varphi_2)_*(t_1 \otimes t_2) = \varphi_{1*}(t_1) \otimes \varphi_{2*}(t_2).
$$

13.4.3. Với ký hiệu của 13.4.1, cho $F_1, F_2$ và F là các không gian đa chuẩn tách được, và cho $(u_1, u_2) \mapsto u_1 . u_2$ là một ánh xạ song tuyến tính liên tục của $F_1 \times F_2$ vào F. Cho
$$
f_i : X_i \to F_i \quad (i = 1, 2)
$$
là một ánh xạ thuộc lớp $C^r$, và định nghĩa $f_1 \otimes f_2 : X \to F$ bởi
$$
(f_1 \otimes f_2)(y_1, y_2) = f_1(y_1) . f_2(y_2).
$$
Ánh xạ $f_1 \otimes f_2$ thuộc lớp $C^r$, và ta có
$$
\langle f_1 \otimes f_2, t_1 \otimes t_2 \rangle = \langle f_1, t_1 \rangle . \langle f_2, t_2 \rangle.
$$

13.4.4. Với ký hiệu của 13.4.1, cho $f$ là một ánh xạ thuộc lớp $C^r$ của X vào một không gian đa chuẩn tách được F. Nếu $y_1 \in X_1$, ký hiệu $f_{y_1}$ là ánh xạ $y_2 \mapsto f(y_1, y_2)$ của $X_2$ vào F và đặt $g(y_1) = \langle f_{y_1}, t_2 \rangle$. Hàm $g : X_1 \to F$ được định nghĩa như vậy thuộc lớp $C^{r - k_1}$, và ta có
$$
\langle f, t_1 \otimes t_2 \rangle = \langle g, t_1 \rangle,
$$
nói cách khác
$$
\langle f, t_1 \otimes t_2 \rangle = \langle y_1 \mapsto \langle y_2 \mapsto f(y_1, y_2), t_2 \rangle, t_1 \rangle.
$$
Tương tự
$$
\langle f, t_1 \otimes t_2 \rangle = \langle y_2 \mapsto \langle y_1 \mapsto f(y_1, y_2), t_1 \rangle, t_2 \rangle.
$$

13.4.5. Với ký hiệu của 13.4.1, cho

$$
\alpha_{k_1, k_2} : T^{(k_1)}_{x_1}(X_1) \otimes T^{(k_2)}_{x_2}(X_2) \to T^{(k)}_x(X)
$$

là ánh xạ tuyến tính được xác định bởi ánh xạ song tuyến tính $(t_1, t_2) \mapsto t_1 \otimes t_2$; ánh xạ này là đơn ánh; nó là song ánh nếu $k_1$ và $k_2$ là vô hạn.

Nếu $n \leq r$, ký hiệu $T^{(n)}_x(X_1, X_2)$ là không gian con vectơ của $T^{(n)}_{x_1}(X_1) \otimes T^{(n)}_{x_2}(X_2)$ sinh bởi các không gian con $T^{(k_1)}_{x_1}(X_1) \otimes T^{(k_2)}_{x_2}(X_2)$ với $k_1 + k_2 \leq n$. Tồn tại duy nhất một ánh xạ tuyến tính

$$
\alpha_n : T^{(n)}_x(X_1, X_2) \to T^{(n)}_x(X)
$$

mở rộng các ánh xạ $\alpha_{k_1, k_2}$ đã định nghĩa ở trên; nó là một đẳng cấu. Trong phần tiếp theo, ta đồng nhất $T^{(n)}_x(X)$, bằng $\alpha_n^{-1}$, với không gian con vectơ $T^{(n)}_x(X_1, X_2)$ của $T^{(n)}_{x_1}(X_1) \otimes T^{(n)}_{x_2}(X_2)$.

13.4.6. Giữ lại ký hiệu của 13.4.5 và 13.3.1. Bằng cách chuyển qua thương, $\alpha_{k_1, k_2}$ xác định một ánh xạ tuyến tính

$$
\varepsilon_{k_1, k_2} : \operatorname{gr}_{k_1} T^{(r)}_{x_1}(X_1) \otimes \operatorname{gr}_{k_2} T^{(r)}_{x_2}(X_2) \to \operatorname{gr}_k T^{(r)}_x(X).
$$

Các ánh xạ $\varepsilon_{k_1, k_2}$ ($k_1 + k_2 \leq r$) là các thành phần của một ánh xạ tuyến tính phân bậc bậc không

$$
\varepsilon : \bigoplus_{k_1 + k_2 \leq r} (\operatorname{gr}_{k_1} T^{(r)}_{x_1}(X_1) \otimes \operatorname{gr}_{k_2} T^{(r)}_{x_2}(X_2)) \to \bigoplus_{k \leq r} \operatorname{gr}_k T^{(r)}_x(X)
$$

là một đẳng cấu. Biểu đồ

$$
\begin{array}{ccc}
\bigoplus_{k_1 + k_2 \leq r} (\operatorname{gr}_{k_1} T^{(r)}_{x_1}(X_1) \otimes \operatorname{gr}_{k_2} T^{(r)}_{x_2}(X_2)) & \xrightarrow{\varepsilon} & \operatorname{gr} T^{(r)}_x(X) \\
\downarrow i_{12} & & \downarrow i_X \\
\bigoplus_{k_1 + k_2 \leq r} (\mathrm{TS}^{k_1}(T_{x_1}(X_1)) \otimes \mathrm{TS}^{k_2}(T_{x_2}(X_2))) & \xrightarrow{\sigma} & \bigoplus_{k \leq r} \mathrm{TS}^k(T_{x_1}(X_1) \times T_{x_2}(X_2))
\end{array}
$$

là giao hoán (trong biểu đồ này, $i_{12}$ ký hiệu đồng cấu cảm sinh bởi $i_{x_1} \otimes i_{x_2}$ và $\sigma$ là đẳng cấu được định nghĩa trong A, IV, § 5, No. 5). Nếu $r$ là vô hạn, biểu đồ này được viết đơn giản là:

$$
\begin{array}{ccc}
\operatorname{gr} T^{(\infty)}_{x_1}(X_1) \otimes \operatorname{gr} T^{(\infty)}_{x_2}(X_2) & \xrightarrow{\varepsilon} & \operatorname{gr} T^{(\infty)}_x(X) \\
\downarrow i_{x_1} \otimes i_{x_2} & & \downarrow i_X \\
\mathrm{TS}(T_{x_1}(X_1)) \otimes \mathrm{TS}(T_{x_2}(X_2)) & \xrightarrow{\sigma} & \mathrm{TS}(T_x(X)).
\end{array}
$$

### 13.5. Tích đồng sản

Trong số này, $X$ ký hiệu một đa tạp thuộc lớp $C^r$ và $x$ là một điểm của $X$.

13.5.1. Cho $k \leq r$. Nếu $\Delta$ là ánh xạ đường chéo $y \mapsto (y, y)$ của $X$ vào $X \times X$, thì $\Delta_*$ ánh xạ $T^{(k)}_x(X)$ vào $T^{(k)}_{(x,x)}(X \times X)$, là một không gian con vectơ của

$T^{(k)}_x(X)\otimes T^{(k)}_x(X)$, xem 13.4.5. Do đó thu được một ánh xạ tuyến tính, vẫn được ký hiệu bởi $\Delta_*$ (hoặc $c$):

$$
T^{(k)}_x(X)\longrightarrow T^{(k)}_x(X)\otimes T^{(k)}_x(X);
$$

nó được gọi là đồng tích gắn với $T^{(k)}_x(X)$. Được trang bị đồng tích này, $T^{(k)}_x(X)$ là một đối đại số kết hợp và đối giao hoán (A, III, p. 144-145); đồng đơn vị của nó là dạng tuyến tính gán cho một phân bố điểm số hạng hằng của nó (13.2.1).
Nếu $k'\leq k$, phép nhúng của $T^{(k')}_x(X)$ vào $T^{(k)}_x(X)$ là một cấu xạ của các đối đại số.
Nếu $c=(U,\varphi,\overline{E})$ là một biểu đồ của $X$ tâm tại $x$, đẳng cấu

$$
\theta_c:T^{(k)}(E)\longrightarrow T^{(k)}_x(X)
$$

là một đẳng cấu của các đối đại số, $T^{(k)}(E)$ được trang bị đồng tích cảm sinh bởi đồng tích của $T(E)$, xem A, IV, § 5, số 7.
Nếu $\varphi:X\longrightarrow Y$ là một cấu xạ của các đa tạp thuộc lớp $C^r$, ánh xạ từ $T^{(k)}(X)$ vào $T^{(k)}_{\varphi(x)}(Y)$ cảm sinh bởi $\varphi_*$ là một cấu xạ của các đối đại số.

### 13.5.2. Cho $F_1$, $F_2$ và $F$ là các không gian đa thức tách được, và $(u_1,u_2)\mapsto u_1.u_2$ là một ánh xạ song tuyến tính liên tục từ $F_1\times F_2$ vào $F$. Cho $t\in T^{(r)}_x(X)$ và

$$
c(t)=\sum_j u_j\otimes v_j\quad(u_j,v_j\text{ trong }T^{(r)}_x(X))
$$

là ảnh của nó qua đồng tích. Cho $f_i:X\longrightarrow F_i$ $(i=1,2)$ là các ánh xạ thuộc lớp $C^r$. Ta có

$$
\langle f_1.f_2,t\rangle=\sum_j\langle f_1,u_j\rangle\langle f_2,v_j\rangle,
$$

mà ta viết, bằng lạm dụng ký hiệu:

$$
\langle f_1.f_2,t\rangle=\langle f_1\otimes f_2,c(t)\rangle.
$$

### 13.5.3. Cho $t\in T^{(k)}_x(X)$, với $k\leq r$.

a) Đối với $c(t)=t\otimes 1$, điều kiện cần và đủ là $t$ bằng $0$ hoặc bằng $\varepsilon_x$.

b) Đối với $c(t)=1\otimes t+\varepsilon_x\otimes t$, điều kiện cần và đủ là $t$ là một vectơ tiếp xúc, tức là $t\in T^{(1)}_x(X)$.

### 13.6. Các phân bố có giá hữu hạn

### 13.6.1. Cho $X$ là một đa tạp thuộc lớp $C^r$, và cho $k\leq r$. Ta ký hiệu bởi $\mathscr{T}^{(k)}(X)$ tổng trực tiếp của các không gian $T^{(k)}_x(X)$, với $x\in X$. Một phần tử của $\mathscr{T}^{(k)}(X)$ được gọi là một phân bố có giá hữu hạn trên $X$, cấp $\leq k$. Nếu $f:X\longrightarrow F$ là một hàm thuộc lớp $C^r$ với các giá trị trong một không gian đa thức tách được $F$, và nếu

$$
t=\sum_{x\in X}t_x,
$$

trong đó $t_x\in T^{(k)}_x(X)$ với mọi $x\in X$ là một phân bố có giá hữu hạn, ta đặt

$$
\langle f,t\rangle=\sum_{x\in X}\langle f,t_x\rangle.
$$

Tương tự, ta đặt

$$
c(t)=\sum_{x\in X}c(t_x),
$$

which trang bị cho $\mathscr{T}^{(k)}(X)$ một cấu trúc đối đại số cođồng kết hợp, đối giao hoán, với một đồng đơn vị $t\mapsto\langle1,t\rangle$. Các phép nhúng

$$
\mathscr{T}^{(k')}(X)\longrightarrow\mathscr{T}^{(k)}(X),
$$

trong đó $k'\leq k$, là các cấu xạ đối đại số.

Nếu $\varphi : X \to Y$ là một cấu xạ của các đa tạp lớp $C^r$, các ánh xạ $T_x^{(k)}(\varphi) : T_x^{(k)}(X) \to T_{\varphi(x)}^{(k)}(Y)$ tương ứng với các điểm khác nhau $x$ của $X$ định nghĩa một ánh xạ tuyến tính $\varphi_*$ của $\mathscr{T}^{(k)}(X)$ vào $\mathscr{T}^{(k)}(Y)$, là một cấu xạ đối đại số.

Nếu $X_1$ và $X_2$ là hai đa tạp lớp $C^r$, các ánh xạ $\alpha_k^{-1}$ (xem 13.4.5) định nghĩa một ánh xạ tuyến tính
$$
\mathscr{T}^{(k)}(X_1 \times X_2) \to \mathscr{T}^{(k)}(X_1) \otimes \mathscr{T}^{(k)}(X_2)
$$
là đơn ánh; nó là một cấu xạ đối đại số. Nếu $k = \infty$ hoặc $\omega$, nó là một đẳng cấu của các đối đại số.

13.6.2. Cho $X$ là một đa tạp lớp $C^r$, và cho $V$ là một không gian vectơ $K$ có số chiều hữu hạn. Một phần tử của $\mathscr{T}^{(r)}(X) \otimes V$ được gọi là một phân bố có giá hữu hạn trên $X$ với các giá trị trong $V$. Khi $K = \mathbf{R}$, $V = \mathbf{C}$, một phân bố như vậy cũng được gọi là một phân bố phức có giá hữu hạn trên $X$. Các định nghĩa và các kết quả của các No. trước đó mở rộng ngay lập tức, bởi tính tuyến tính, đến các phân bố với các giá trị trong $V$.

### 13.7. Làm yếu cấu trúc

Giả sử $K = \mathbf{R}$. Cho $r' \in \mathbf{N}_K$ sao cho $r' \leq r$. Cho $X$ là một đa tạp lớp $C^r$, và cho $X'$ là đa tạp lớp $C^{r'}$ thu được bằng cách làm yếu cấu trúc (5.13.1). Cho $x \in X$, và cho $t \in T_x^{(k)}(X)$, với $k \leq r'$. Chọn một biểu đồ $c = (U, \varphi, E)$ của $X$ tâm tại $x$, và cho $\tilde{t}$ là phần tử của $TS^{(k)}(E)$ sao cho $\theta_c(\tilde{t}) = t$. Vì $c$ là một biểu đồ của $X'$ tâm tại $x$, phần tử $t' = \theta_c(\tilde{t})$ của $T_x^{(k)}(X')$ được định nghĩa; nó độc lập với lựa chọn $c$. Ánh xạ $t \mapsto t'$ là một song ánh của $T_x^{(k)}(X)$ lên $T_x^{(k)}(X')$ nhờ đó hai không gian này được đồng nhất. Các sự đồng nhất thu được như vậy tương thích với các phép toán $\langle f, t \rangle, \varphi_*(t), t_1 \otimes t_2, c(t), \ldots$ của các No. trước đó.

[^1]: Ở đây một lần nữa, tích của các $\gamma_{\alpha_i}(\partial_i,x)$ là một tích đối xứng trong $TS(T_x(X))$.
