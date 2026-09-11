---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 4
section_title: Some classes of operators in hilbertian spaces
lang: vi
source: evt-i-v
pdf_pages: 0295-0318
extraction: ocr
subsections:
    - "no": 1
      title: Adjoint
      page: 38
      pdf_page: 296
    - "no": 2
      title: Partially isometric linear mappings
      page: 41
      pdf_page: 299
    - "no": 3
      title: Normal endomorphisms
      page: 43
      pdf_page: 301
    - "no": 4
      title: Hermitian endomorphisms
      page: 44
      pdf_page: 302
    - "no": 5
      title: Positive endomorphisms
      page: 45
      pdf_page: 303
    - "no": 6
      title: Trace of an endomorphism
      page: 48
      pdf_page: 306
    - "no": 7
      title: Hilbert-Schmidt mappings
      page: 52
      pdf_page: 310
    - "no": 8
      title: Diagonalization of Hilbert-Schmidt mappings
      page: 55
      pdf_page: 313
    - "no": 9
      title: Trace of a quadratic form with respect to another
      page: 57
      pdf_page: 315
statements: 48
exercises: 0
content_sha256: 7dbac925289bf22c96f67bb077097e2a57c151146b3f522311451feb927b9faf
translated_from: content/en/evt/V/04_s4_some_classes_of_operators_in_hilbertian.md
source_content_sha256: e91bc304651ce770d0fd7f9268828dea76e99a75428b9ae2fa319330bd7c91db
translation_model: gpt-5-6, gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-e606aaac
glossary_version: 34
glossary_terms_sha256: 6810319ed53a66f78bac96282c2a1077ec0c09b0eef014d0a7f43f415fc3a4b4
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. MỘT SỐ LỚP CÁC TOÁN TỬ TRONG CÁC KHÔNG GIAN HILBERT

Trong suốt đoạn này, $l_E$ ký hiệu ánh xạ đồng nhất của một không gian Hilbert E. Hợp thành $v \circ u$ của hai ánh xạ tuyến tính thường sẽ được ký hiệu là $vu$ hoặc $v.u$.

### 1. Liên hợp

#### Mệnh đề 1 {#evt-v-s4-prop-1 .statement}

— Cho E và F là hai không gian Hilbert. Với mọi ánh xạ $u \in \mathcal{L}(E; F)$, tồn tại một ánh xạ duy nhất $u^* \in \mathcal{L}(F; E)$ sao cho

$$
\langle u(x)|y \rangle_F = \langle x|u^*(y) \rangle_E
$$

với mọi $x \in E$ và mọi $y \in F$. Ánh xạ $u \mapsto u^*$ từ $\mathcal{L}(E, F)$ vào $\mathcal{L}(F; E)$ là song ánh, đẳng cự và nửa tuyến tính (đối với tự đẳng cấu $\xi \mapsto \overline{\xi}$ của K).

Gọi $\mathscr{S}(E, F)$ là không gian của tất cả các dạng sesquilinear liên tục trên $E \times F$, được trang bị chuẩn

$$
\| \Phi \| = \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi(x, y)| .
$$

Ta định nghĩa không gian $\mathscr{S}(F, E)$ một cách tương tự. Ta đã định nghĩa (V, p. 16, cor. 2) một đẳng cấu không gian Banach từ $\mathcal{L}(E; F)$ lên $\mathscr{S}(F, E)$, ký hiệu bởi $u \mapsto \Phi_u$ và được đặc trưng bởi

$$
\Phi_u(y, x) = \langle y|u(x) \rangle_F \quad (x \in E, \ y \in F) .
$$

Theo cách tương tự, ta định nghĩa một đẳng cấu từ $\mathcal{L}(F, E)$ lên $\mathscr{S}(E, F)$. Cuối cùng ta định nghĩa một ánh xạ $\Phi \mapsto \Phi^*$ từ $\mathscr{S}(F, E)$ lên $\mathscr{S}(E, F)$ bởi

$$
\Phi^*(x, y) = \overline{\Phi(y, x)} \quad (x \in E, \ y \in F) .
$$

Ánh xạ này là song ánh, nửa tuyến tính và đẳng cự. Nhưng công thức (1) được chuyển thành $\Phi_{u^*} = (\Phi_u)^*$, do đó suy ra mệnh đề.

#### Định nghĩa 1 {#evt-v-s4-def-1 .statement}

— Cho E và F là hai không gian Hilbert. Với mọi ánh xạ tuyến tính liên tục $u : E \to F$, ánh xạ tuyến tính liên tục từ F vào E được xác định bởi công thức (1) được gọi là ánh xạ liên hợp của u và được ký hiệu bởi $u^*$.

Ta có

$$
\begin{align*}
(u + v)^* &= u^* + v^* \\
(\lambda u)^* &= \overline{\lambda} u^* \\
(u^*)^* &= u \\
(1_E)^* &= 1_E \\
(wu)^* &= u^* w^* ;
\end{align*}
$$

trong tất cả các công thức này, $u$ và $v$ thuộc $\mathcal{L}(E; F)$, $\lambda$ thuộc K, và $w$ thuộc $\mathcal{L}(F; G)$ trong đó G là một không gian Hilbert. Các công thức (5) và (6) có nghĩa là $u \mapsto u^*$ là nửa tuyến tính. Công thức (8) là hiển nhiên. Để chứng minh (7), ta lấy liên hợp của hai vế của (1), thu được $\langle u^*(y)|x\rangle = \langle y|u(x)\rangle$, và điều này chứng minh rằng $u$ là liên hợp của $u^*$. Cuối cùng, với các ký hiệu của (9), ta có, với mọi $z \in G$

$$
\langle w(u(x))|z\rangle = \langle u(x)|w^*(z)\rangle = \langle x|u^*(w^*(z))\rangle ,
$$

do đó $u^*w^*$ là liên hợp của $wu$.

Cho $u : E \to F$ là một ánh xạ tuyến tính liên tục và song ánh; khi đó nó cũng là song liên tục (I, p. 19, cor. 1). Từ (8) và (9) ta suy ra ngay lập tức rằng $u^*$ là song ánh và song liên tục và rằng

(10)
$$
(u^{-1})^* = (u^*)^{-1} .
$$

#### Mệnh đề 2 {#evt-v-s4-prop-2 .statement}

*Với mọi $u \in \mathcal{L}(E ; F)$, ta có*

(11)
$$
\|u^*u\| = \|uu^*\| = \|u\|^2 = \|u^*\|^2 .
$$

Theo mệnh đề 1, $\|u^*\| = \|u\|$, do đó $\|u^*u\| \leq \|u^*\|\cdot\|u\| \leq \|u\|^2$. Mặt khác,

$$
\|u\|^2 = \sup_{\|x\| \leq 1} \|u(x)\|^2 = \sup_{\|x\| \leq 1} \langle u(x)|u(x)\rangle = \sup_{\|x\| \leq 1} \langle x|u^*u(x)\rangle \leq \|u^*u\| ,
$$

do đó $\|u^*u\| = \|u\|^2$. Thay thế $u$ bởi $u^*$, ta được $\|uu^*\| = \|u^*\|^2$, do đó (11) suy ra vì $\|u\| = \|u^*\|$.

Cho $E_1, ..., E_n$ và $F_1, ..., F_n$ là các không gian Hilbert, và với mọi số nguyên $i$ giữa 1 và $n$, cho $u_i$ là một ánh xạ tuyến tính liên tục từ $E_i$ vào $F_i$. Khi đó

(12)
$$
(u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n)^* = u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^* .
$$

Cho $v$ là ánh xạ tuyến tính liên tục $u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$ từ

$$
E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n \quad \text{vào} \quad F = F_1 \hat{\otimes}_2 ... \hat{\otimes}_2 F_n
$$

và $w$ là ánh xạ tuyến tính liên tục $u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^*$ từ $F$ vào $E$. Chỉ cần chứng minh đẳng thức $\langle y|v(x)\rangle = \langle w(y)|x\rangle$ với $x \in E$ và $y \in F$. Nhờ tính tuyến tính và tính liên tục, ta rút gọn về trường hợp khi $x$ và $y$ có dạng sau

$$
x = x_1 \otimes ... \otimes x_n , \quad y = y_1 \otimes ... \otimes y_n
$$

với $x_i \in E_i$ và $y_i \in F_i$ cho $1 \leq i \leq n$. Từ định nghĩa của tích vô hướng trong một tích tenxơ (V, p. 27, công thức (6)), ta suy ra

$$
\langle y|v(x)\rangle = \prod_{i=1}^n \langle y_i|u_i(x_i)\rangle = \prod_{i=1}^n \langle u_i^*(y_i)|x_i\rangle = \langle w(y)|x\rangle .
$$

Điều đó chứng minh mệnh đề của chúng ta.

Cho $E$ và $F$ là hai không gian Hilbert, $u \in \mathcal{L}(E ; F)$ và $n$ là một số nguyên dương. Nếu ta đặt $u_1 = ... = u_n = u$ trong công thức (12) thì ta thu được kết quả rằng ánh xạ tuyến tính liên tục $\hat{T}^n(u^*)$ từ $\hat{T}^n(F)$ vào $\hat{T}^n(E)$ là liên hợp của ánh xạ tuyến tính liên tục $\hat{T}^n(u)$ từ $\hat{T}^n(E)$ vào $\hat{T}^n(F)$. Các công thức

$$
\hat{S}^n(u)^* = \hat{S}^n(u^*) , \quad \hat{\Lambda}^n(u)^* = \hat{\Lambda}^n(u^*)
$$

có thể được thiết lập theo cùng một cách như công thức (12), do định nghĩa của tích vô hướng trong $\hat{S}^n(E)$ (V, p. 30, công thức (15)) và trong $\hat{\Lambda}^n(E)$ (V, p. 33, công thức (26)).

#### Nhận xét 1 {#evt-v-s4-n1-rem-1 .statement}

Giả sử không gian Hilbert E không rút gọn về 0. Ta đồng nhất $\mathcal{L}(K;E)$ với E qua ánh xạ $u \mapsto u(1)$; nói cách khác, vectơ x của E được đồng nhất với ánh xạ $\lambda \mapsto \lambda.x$ từ K vào E. Khi đó liên hợp của x là ánh xạ $x^*:E \to K$ được cho bởi $x^*(y) = \langle x|y \rangle$. Nói cách khác, $x \mapsto x^*$ là ánh xạ nửa tuyến tính chính tắc từ E lên đối ngẫu của nó (V, p. 15).

Tương tự, ta đồng nhất số $\lambda \in K$ với tự đồng cấu $\lambda.1_E$ của E. Khi đó $\lambda^*$ chính xác là liên hợp của $\lambda$.

Với các đồng nhất này, ta có thể định nghĩa một tích $t_1 ... t_n$ trong đó mỗi $t_i$ là, hoặc một số trong K, hoặc một vectơ trong E, hoặc một dạng tuyến tính thuộc E', hoặc một phần tử của $\mathcal{L}(E)$, với điều kiện là không bao giờ có hai thừa số liên tiếp $t_i$ và $t_{i+1}$ thuộc một trong các kiểu sau :
• $xy$ khi $x, y$ đều thuộc E, hoặc đều thuộc E' ;
• $xA$ hoặc $Ax'$ với $A \in \mathcal{L}(E)$, $x \in E$ và $x' \in E'$.

Ta có các quy tắc hợp thành sau :
a) tính kết hợp ;
b) mọi phần tử của K giao hoán với mọi thừa số khác ;
c) ta có $(t_1 ... t_n)^* = t_n^* ... t_1^*$; nói cách khác, liên hợp của một tích là tích của các liên hợp lấy theo thứ tự ngược lại. Đồng thời $t^{**} = t$.

Ví dụ, cho x, y thuộc E và cho A thuộc $\mathcal{L}(E)$. Khi đó $x^*y$ biểu diễn tích vô hướng $\langle x|y \rangle$ và $x^*Ay$ biểu diễn tích vô hướng $\langle x|Ay \rangle$. Ta cũng có $(A^*x)^* = x^*A^{**} = x^*A$, do đó $(A^*x)^*y = x^*Ay$, điều này có thể được hiểu là

$$
\langle A^*x|y \rangle = \langle x|Ay \rangle
$$

phù hợp với định nghĩa của toán tử liên hợp. Ta nhận thấy rằng $yx^*$ là tự đồng cấu $z \mapsto y \langle x|z \rangle$ của E, vì $yx^*z$ có thể được hiểu là $y(x^*z)$ nhờ tính kết hợp, hoặc là $y.\langle x|z \rangle$.

Theo Dirac $^1$, trong phần lớn các công trình về Vật lý Toán học, các phần tử của E được biểu diễn bởi ký hiệu $|x\rangle$, các phần tử của E' bởi $\langle t|$. Tích vô hướng được viết là $\langle x|y \rangle = \langle x|.|y \rangle$ và quy tắc cấm đầu tiên trong các tích loại trừ các tổ hợp của các dấu $|$ và $|<$, chẳng hạn $|x\rangle|y\rangle$.

#### Mệnh đề 3 {#evt-v-s4-prop-3 .statement}

— Cho E và F là hai không gian Hilbert và $u \in \mathcal{L}(E;F)$. Các điều kiện sau là tương đương :

(i) $u$ là một đẳng cấu không gian vectơ tôpô, với nghịch đảo bằng $u^*$;
(ii) $u$ là toàn ánh và $u^*u = 1_E$;
(iii) $u$ là đơn ánh và $uu^* = 1_F$;
(iv) $u$ là một đẳng cấu của các không gian chuẩn;
(v) $u$ là một đẳng cấu không gian Hilbert.

Điều kiện (1) có nghĩa là ta có $u^*u = 1_E$ và $uu^* = 1_F$. Do đó sự tương đương của (i), (ii) và (iii) suy ra từ E, II, § 3, No. 8, mệnh đề 8. Ta đã thấy sự tương đương của (iv) và (v) (V, p. 5). Cuối cùng, quan hệ $u^*u = 1_E$ tương đương với

$^1$ Xem P. A. M. Dirac, Quantum Mechanics, Oxford University Press, New York, 1935.

$
\langle x|u^*u(y)\rangle = \langle x|y\rangle$, nghĩa là, với $\langle u(x)|u(y)\rangle = \langle x|y\rangle$ với mọi $x, y$ trong $E$, và hiển nhiên kéo theo rằng $u$ là đơn ánh; điều này chứng minh sự tương đương của (ii) và (v).

Một tự đẳng cấu của không gian Hilbert $E$ còn được gọi là một *toán tử unita*, nghĩa là, một toán tử $u \in \mathcal{L}(E)$ thỏa mãn $uu^* = u^*u = 1_E$.

#### Nhận xét 2 {#evt-v-s4-n1-rem-2 .statement}

— Quan hệ $u^*u = 1_E$ không đặc trưng cho tất cả các tự đẳng cấu của không gian Hilbert $E$. Ví dụ, cho $E = \ell^2(\mathbf{N})$ và cho $u$ được xác định bởi $u(x_n) = x_{n-1}$ với $n \geq 1$ và $u(x)_0 = 0$. Ta có $\|u(x)\| = \|x\|$ với mọi $x \in E$, nghĩa là, $u^*u = 1_E$, nhưng $u$ không là toàn ánh.

#### Nhận xét 3 {#evt-v-s4-n1-rem-3 .statement}

— Định nghĩa (1) của toán tử liên hợp $u^*$ cũng có thể được viết là
$$
\langle y|u(x)\rangle = \langle u^*(y)|x\rangle ,
$$
hoặc, theo V, p. 15, là
$$
\langle u(x), y^*\rangle = \langle x, (u^*(y))^*\rangle .
$$
Nhưng ta cũng có $\langle u(x), y^*\rangle = \langle x, {}^t u(y^*)\rangle$, do đó ta có thể biểu diễn toán tử liên hợp theo chuyển vị,
$$
(u^*(y))^* = {}^t u(y^*) .
$$

### 2. Các ánh xạ tuyến tính từng phần đẳng cự

#### Định nghĩa 2 {#evt-v-s4-def-2 .statement}

*Cho $E$ và $F$ là hai không gian Hilbert và $u \in \mathcal{L}(E; F)$. Phần bù trực giao của hạt nhân của $u$ trong $E$ được gọi là không gian con ban đầu của $u$ và bao đóng của ảnh của $u$ trong $F$ được gọi là không gian con cuối của $u$. Phép chiếu trực giao từ $E$ (tương ứng $F$) lên không gian con ban đầu (tương ứng cuối) của $u$ được gọi là phép chiếu trực giao ban đầu (tương ứng cuối) của $u$.*

Cho $P$ là không gian con ban đầu của $u$. Vì $E$ là tổng trực tiếp của $P$ và hạt nhân của $u$, ta có $u(P) = u(E)$.

#### Mệnh đề 4 {#evt-v-s4-prop-4 .statement}

(i) *Không gian con ban đầu (tương ứng cuối) của $u^*$ bằng không gian con cuối (tương ứng ban đầu) của $u$.*

(ii) *Giả sử rằng $E = F$. Cho $M$ là một không gian vectơ con đóng của $E$ và $M^\circ$ là phần bù trực giao của nó. Các quan hệ $u(M) \subset M$ và $u^*(M^\circ) \subset M^\circ$ là tương đương.*

Cho $Q = \overline{u(E)}$ là không gian con cuối của $u$. Phần bù trực giao $Q^\circ$ của $Q$ trong $F$ gồm tất cả các vectơ $y$ sao cho $\langle u(x)|y\rangle = 0$ với mọi $x \in E$; điều này tương đương với : $\langle x|u^*(y)\rangle = 0$ với mọi $x \in E$, hay với $u^*(y) = 0$. Do đó ta có $Q^\circ = \mathrm{Ker}\, u^*$, và $Q$ là không gian con ban đầu của $u^*$. Vì $u$ là chuyển vị của $u^*$, không gian con cuối của $u^*$ cũng là không gian con ban đầu của $u$. Điều này chứng minh (i).

Quan hệ $u(M) \subset M$ suy ra rằng $u(M)$ trực giao với $M^\circ$, và quan hệ $u^*(M^\circ) \subset M^\circ$ suy ra rằng $u^*(M^\circ)$ trực giao với $M$. Nhưng ta có $\langle u(x)|y\rangle = \langle u^*(y)|x\rangle$ với mọi $x \in M$ và $y \in M^\circ$; do đó (ii) suy ra.

Ta nhận xét rằng mệnh đề 4 có thể được suy ra từ các tính chất tổng quát của chuyển vị (II, p. 51, hệ quả 2) xét đến nhận xét 3, V, p. 41.

#### Định nghĩa 3 {#evt-v-s4-def-3 .statement}

*Cho $E$ và $F$ là hai không gian Hilbert. Một ánh xạ $u \in \mathcal{L}(E; F)$ được* gọi là đẳng cự từng phần nếu $\|u(x)\| = \|x\|$ với mọi $x$ thuộc không gian con ban đầu của $u$.

Cho $u \in \mathcal{L}(E; F)$ và gọi $N$ là hạt nhân và $I$ là ảnh của nó. Nói rằng $u$ là đẳng cự bộ phận cũng chính là nói rằng ánh xạ tuyến tính $\tilde{u}: E/N \to I$ suy ra từ $u$ là đẳng cự (V, p. 13). Khi đó không gian con $I$ của $F$ là đầy đủ, do đó đóng, và là không gian con cuối của $u$. Do đó, $u$ cảm sinh một đẳng cấu không gian Hilbert từ không gian con ban đầu của $u$ lên không gian con cuối của nó.

#### Mệnh đề 5 {#evt-v-s4-prop-5 .statement}

*Cho $u \in \mathcal{L}(E; F)$, gọi $P$ là không gian con ban đầu và $Q$ là không gian con cuối của nó. Gọi $p$ (tương ứng $q$) là phép chiếu trực giao ban đầu (tương ứng cuối) của $u$. Giả sử rằng $u$ là đẳng cự bộ phận.*

(i) *Ánh xạ $u^* \in \mathcal{L}(F; E)$ là đẳng cự bộ phận, với không gian con ban đầu $Q$ và không gian con cuối $P$. Khi đó, đẳng cấu từ $P$ lên $Q$ cảm sinh bởi $u$ là nghịch đảo của đẳng cấu từ $Q$ lên $P$ cảm sinh bởi $u^*$.*

(ii) *Ta có $u^*u = p$ và $uu^* = q$.*

Theo mệnh đề 4 (i), mệnh đề (i) là một hệ quả của (ii).

Bây giờ chứng minh (ii). Vì $P$ chứa ảnh của $u^*$, nên ánh xạ $u^*u$ ánh xạ $E$ vào $P$. Cho $x \in E$ và $y \in P$, khi đó

$$
\langle u^*u(x)|y \rangle = \langle u(x)|u(y) \rangle .
$$

Nếu $x$ thuộc $P$, thì $\langle u(x)|u(y) \rangle = \langle x|y \rangle$ theo định nghĩa của ánh xạ đẳng cự bộ phận; nếu $x$ thuộc hạt nhân $N$ của $u$, thì $u(x) = 0$, do đó $\langle u(x)|u(y) \rangle = 0$ và $\langle x|y \rangle = 0$ vì $N$ và $P$ trực giao. Vì $E = P \oplus N$, ta có $\langle u^*u(x) - x|y \rangle = 0$ trong mọi trường hợp, và do đó $u^*u$ là phép chiếu trực giao $p$ từ $E$ lên $P$. Hệ thức $uu^* = q$ suy ra bằng cách đổi chỗ $u$ và $u^*$ trong lập luận trên.

#### Mệnh đề 6 {#evt-v-s4-prop-6 .statement}

*Với mọi $u \in \mathcal{L}(E; F)$, các điều kiện sau đây là tương đương :*

(i) *$u$ là đẳng cấu từng phần ;*
(ii) *$u^*$ là đẳng cấu từng phần ;*
(iii) *$u^*u$ là một phép chiếu trực giao ;*
(iv) *$uu^*$ là một phép chiếu trực giao ;*
(v) *$uu^*u = u ;*$
(vi) *$u^*uu^* = u^* .*$

Theo mệnh đề 5, (i) tương đương với (ii).

(i) $\Rightarrow$ (v) : Giả sử $u$ là đẳng cấu từng phần. Khi đó $u^*u$ là phép chiếu trực giao ban đầu của $u$ theo mệnh đề 5. Do đó với mọi $x \in E$, $u^*u(x) - x$ thuộc hạt nhân của $u$, nghĩa là $uu^*u(x) = u(x)$.

(v) $\Rightarrow$ (iii) : Giả sử rằng $uu^*u = u$ và đặt $p = u^*u$; khi đó $p = p^*$ và $p^2 = p$. Gọi $M$ (tương ứng $N$) là ảnh (tương ứng hạt nhân) của $p$. Với $x \in M$ và $y \in N$, ta có $\langle x|y \rangle = \langle p(x)|y \rangle = \langle x|p^*(y) \rangle = \langle x|p(y) \rangle = 0$. Vì $M$ và $N$ trực giao, $p$ là phép chiếu trực giao từ $E$ lên $M$.

(iii) $\Rightarrow$ (i) : Giả sử $p = u^*u$ là một phép chiếu trực giao có ảnh $M$ và hạt nhân $N$.

Với mọi $x \in E$, ta có
$$
\|u(x)\|^2 = \langle u^*u(x)|x \rangle = \langle p(x)|x \rangle .
$$
Do đó $u(x) = 0$ với $x \in N$ và $\|u(x)\| = \|x\|$ với $x \in M$, và vì thế $u$ là đẳng cấu từng phần với hạt nhân $N$ và không gian con ban đầu $M$.

Ta đã chứng minh sự tương đương của (i), (iii) và (v). Thay $u$ bởi $u^*$, ta có thể suy ra sự tương đương của (ii), (iv) và (vi). Điều này chứng minh mệnh đề 6.

### 3. Các tự đồng cấu chuẩn

#### Định nghĩa 4 {#evt-v-s4-def-4 .statement}

Cho $E$ là một không gian Hilbert và $u \in \mathcal{L}(E)$. Ta nói rằng $u$ là chuẩn nếu nó giao hoán với tự liên hợp $u^*$ của nó.

Ví dụ, mọi tự đẳng cấu $u$ của không gian Hilbert $E$ đều là chuẩn vì ta có $uu^* = u^*u = 1_E$.

#### Mệnh đề 7 {#evt-v-s4-prop-7 .statement}

Để $u \in \mathcal{L}(E)$ là chuẩn, điều kiện cần và đủ là $\|u(x)\| = \|u^*(x)\|$ với mọi $x \in E$.

Ta định nghĩa một dạng Hermit $\Phi$ trên $E$ bởi
$$
\Phi(x, y) = \langle uu^*(x)|y \rangle - \langle u^*u(x)|y \rangle .
$$
Để $u$ là chuẩn thường, điều kiện cần và đủ là $\Phi = 0$. Theo các công thức phân cực (V, p. 2), điều này tương đương với $\Phi(x, x) = 0$ với mọi $x \in E$. Mệnh đề được suy ra ngay vì
$$
\Phi(x, x) = \|u^*(x)\|^2 - \|u(x)\|^2 .
$$

#### Mệnh đề 8 {#evt-v-s4-prop-8 .statement}

Giả sử rằng $u \in \mathcal{L}(E)$ là chuẩn thường. Gọi $N$ là hạt nhân của $u$ và $M$ là không gian trực giao của $N$ trong $E$; gọi $m$ và $n$ là hai số nguyên dương sao cho $m + n \geq 1$. Khi đó $N$ là hạt nhân của $u^m(u^*)^n$ và $M$ vừa là không gian con ban đầu vừa là không gian con cuối của $u^m(u^*)^n$. Đặc biệt, $M$ vừa là không gian con ban đầu vừa là không gian con cuối của $u$ và của $u^*$, và ổn định đối với $u$ và $u^*$.

Mệnh đề 7 chỉ ra rằng $u$ và $u^*$ có cùng hạt nhân $N$. Theo mệnh đề 4, (ii) của V, p. 41, không gian con $M$ của $E$ là ổn định đối với $u$ và $u^*$ vì điều này đúng với $N = M^\circ$, vì $M \cap N = \{0\}$, các tự đồng cấu của $M$ cảm sinh bởi $u$ và $u^*$ là đơn ánh. Đặt $v = u^m(u^*)^n$; lập luận trước cho thấy hạn chế của $v$ trên $M$ (tương ứng $N$) là đơn ánh (tương ứng không), do đó $N$ là hạt nhân của $v$. Do đó, $M = N^\circ$ là không gian con ban đầu của $v$. Theo mệnh đề 4, (i) của V, p. 41, không gian con cuối của $v$ bằng không gian con ban đầu của $v^*$. Nhưng $v^* = u^n(u^*)^m$ và do đó không gian con ban đầu của $v^*$ bằng $M$ theo điều đã chứng minh ở trên.

#### Hệ quả {#evt-v-s4-n3-cor-1 .statement}

Cho $\lambda \in K$. Các không gian con sau đây của $E$ là bằng nhau :
a) không gian con riêng của $u$ ứng với $\lambda$;
b) không gian con riêng của $u^*$ ứng với $\overline{\lambda}$;

c) *không gian con nguyên sơ của u đối với* $\lambda$ (nói cách khác, theo LIE, VII, § 1, No. 1, tập hợp mọi vectơ $x$ của E sao cho tồn tại một số nguyên $n \geqslant 0$ để $(u - \lambda.1_E)^n(x) = 0$);
d) *không gian con nguyên sơ của* $u^*$ *đối với* $\overline{\lambda}$.

Rõ ràng $w = u - \lambda.1_E$ là một tự đồng cấu chuẩn của E, do đó các tự đồng cấu $w, w^* = u^* - \overline{\lambda}.1_E, w^n$ và $(w^*)^n$ của E có cùng hạt nhân theo mệnh đề 8.

### 4. Các tự đồng cấu Hermit

#### Định nghĩa 5 {#evt-v-s4-def-5 .statement}

*Cho E là một không gian Hilbert và cho* $u \in \mathcal{L}(E)$. *Ta nói rằng u là Hermit nếu* $u^* = u$.

Kí hiệu $\mathcal{H}(E)$ là tập hợp tất cả các phần tử Hermit của $\mathcal{L}(E)$; đây là một không gian con vectơ của không gian vectơ $\mathcal{L}(E)_{[\mathbf{R}]}$ trên $\mathbf{R}$ thu được từ $\mathcal{L}(E)$ bằng cách hạn chế vô hướng.

Với mỗi $u \in \mathcal{L}(E)$, ta đã liên kết (V, p. 16, hệ quả 2) một dạng sesquilinear $\Phi_u : (x, y) \mapsto \langle x|u(y)\rangle$ trên $E \times E$. Ta có

$$
\Phi_{u^*}(x, y) = \overline{\Phi_u(y, x)} \quad (x, y \text{ trong } E);
$$

do đó, $u$ là Hermit nếu và chỉ nếu dạng $\Phi_u$ là Hermit. Khi $K$ là $\mathbf{C}$, chỉ cần giả sử rằng $\Phi_u(x, x) = \langle x|u(x)\rangle$ là thực với mọi $x \in E$ (V, p. 2, *Nhận xét*).

Cho $u \in \mathcal{L}(E)$. Ta đã thấy (V, p. 16, hệ quả 2) rằng chuẩn của $u$ có thể được tính bởi công thức

$$
\|u\| = \sup_{\|x\| \leqslant 1, \|y\| \leqslant 1} |\Phi_u(x, y)|.
$$

Khi $u$ là Hermit, ta có kết quả sau:

#### Mệnh đề 9 {#evt-v-s4-prop-9 .statement}

*Với mọi tự đồng cấu Hermit u của* E, *ta có*

$$
\|u\| = \sup_{\|x\| \leqslant 1} |\langle x|u(x)\rangle|.
$$

Đặt $\Phi = \Phi_u$ và $c = \sup_{\|x\| \leqslant 1} |\Phi(x, x)|$, khi đó hiển nhiên $c \leqslant \|u\|$. Cho $x, y \in E$ sao cho $\|x\| \leqslant 1, \|y\| \leqslant 1$. Khi đó

$$
\Phi(x + y, x + y) = \Phi(x, x) + \Phi(y, y) + 2\Re\Phi(x, y),
$$
do đó
$$
4\Re\Phi(x, y) = \Phi(x + y, x + y) - \Phi(x - y, x - y);
$$
nhưng $|\Phi(t, t)| \leqslant c\|t\|^2$ với mọi $t \in E$, vì thế
$$
4|\Re\Phi(x, y)| \leqslant c(\|x + y\|^2 + \|x - y\|^2) = 2c(\|x\|^2 + \|y\|^2) \leqslant 4c.
$$
Đặt $a = \Phi(x, y)$; tồn tại một số phức $\lambda$ có giá trị tuyệt đối bằng 1 sao cho

λa = |a|. Thay $y$ bởi $\lambda y$ trong bất đẳng thức trên, ta được $|\Phi(x, y)| \leqslant c$. Theo (15), $\|u\| \leqslant c$ và mệnh đề được suy ra. ĐPCM.

Hiển nhiên mọi tự đồng cấu Hermit đều chuẩn. Ngược lại:

#### Mệnh đề 10 {#evt-v-s4-prop-10 .statement}

— Giả sử $K$ là C. Cho $u \in \mathcal{L}(E)$. Khi đó tồn tại duy nhất một cặp $(h_1, h_2)$ gồm các tự đồng cấu Hermit của E, sao cho $u = h_1 + ih_2$. Để u là chuẩn, cần và đủ rằng $h_1$ và $h_2$ giao hoán.

Thật vậy, quan hệ « $u = h_1 + ih_2,\ h_1^* = h_1,\ h_2^* = h_2$ » tương đương với

$$
\text{« } h_1 = \frac{1}{2}(u + u^*) \text{ và } h_2 = \frac{i}{2}(u^* - u) \text{ »}.
$$

Hơn nữa, ta có $h_1 h_2 - h_2 h_1 = \frac{i}{2}(uu^* - u^*u)$. Điều đó chứng minh mệnh đề 10.

#### Mệnh đề 11 {#evt-v-s4-prop-11 .statement}

— Cho $p \in \mathcal{L}(E)$. Để p là phép chiếu trực giao từ E lên một không gian con vectơ đóng của E, cần và đủ rằng $p^2 = p = p^*$.

Giả sử $p^2 = p$. Cho M là ảnh của p và N là hạt nhân của nó. E là tổng trực tiếp tôpô của M và N. Để p là một phép chiếu trực giao, cần và đủ rằng M trực giao với N, tức là ta có $\langle p(x)|y - p(y) \rangle = 0$ với mọi x, y trong E. Quan hệ sau cùng này tương đương với $p = p^*p$, và suy ra $p^* = (p^*p)^* = p^*p = p$; ngược lại nếu $p^* = p$, ta có $p = p^2 = p^*p$.

### 5. Các tự đồng cấu dương

#### Định nghĩa 6 {#evt-v-s4-def-6 .statement}

— Cho E là một không gian Hilbert và $u \in \mathcal{L}(E)$. Ta nói rằng u là dương, và viết $u \geq 0$, nếu u là Hermit và nếu $\langle x|u(x) \rangle \geq 0$ với mọi $x \in E$.

Khi K bằng C, quan hệ

$$
\langle x|u(x) \rangle \geq 0 \quad \text{với mọi } x \in E
$$

suy ra rằng u là Hermit (V, p. 2, Nhận xét), do đó là dương.

Ký hiệu $\mathcal{L}_+(E)$ cho tập hợp tất cả các phần tử dương của $\mathcal{L}(E)$; đây là một nón lồi nhọn thực sự trong không gian vectơ thực $\mathcal{L}(E)_{[\mathbf{R}]}$ nền dưới $\mathcal{L}(E)$. Để u là dương, điều kiện cần và đủ là dạng sesquilinear $\Phi_u$ trên $E \times E$ liên kết với u là Hermit dương. Cho u và v trong $\mathcal{L}(E)$, quan hệ $u - v \geq 0$ cũng có thể viết là $u \geq v$ hoặc $v \leq u$; đây là một quan hệ thứ tự trên $\mathcal{L}(E)_{[\mathbf{R}]}$ tương thích với cấu trúc không gian vectơ thực của nó.

#### Mệnh đề 12 {#evt-v-s4-prop-12 .statement}

— Cho u là một phần tử Hermit (resp. dương) của $\mathcal{L}(E)$ và cho v là một ánh xạ tuyến tính liên tục từ E vào một không gian Hilbert F. Khi đó $vuv^*$ là một phần tử Hermit (resp. dương) của $\mathcal{L}(F)$.

Thật vậy, ta có $(vuv^*)^* = v^{**}u^*v^* = vuv^*$. Mặt khác, nếu $u \geq 0$, ta có

$$
\langle y|vuv^*(y) \rangle = \langle v^*(y)|u(v^*(y)) \rangle \geq 0
$$

với mọi $y \in F$, do đó $vuv^* \geq 0$.

Mệnh đề 12 cho thấy, đặc biệt, rằng $vv^*$ là dương với mọi $v \in \mathcal{L}(E; F)$. Vì, đặc biệt, một toán tử chiếu trực giao $p$ thỏa $p = p^2 = pp^*$, nên nó là dương.

#### Nhận xét 1 {#evt-v-s4-n5-rem-1 .statement}

Với mọi $u$ Hermit trong $\mathcal{L}(E)$, đặt $m(u) = \inf_{\|x\|=1} \langle x|u(x)\rangle$, $M(u) = \sup_{\|x\|=1} \langle x|u(x)\rangle$. Nếu $E$ không chỉ là $0$, thì $m(u)$ và $M(u)$ là hữu hạn; hơn nữa, $M(u)$ là số thực nhỏ nhất $\lambda$ sao cho $u \leq \lambda \cdot 1_E$ và $m(u)$ là số thực lớn nhất $\mu$ sao cho $u \geq \mu \cdot 1_E$. Rõ ràng ta có $m(-u) = -M(u)$ và $M(-u) = -m(u)$. Rõ ràng là
$$
\sup(|m(u)|, |M(u)|) = \sup_{\|x\|=1} |\langle x|u(x)\rangle|
$$
và Mệnh đề 9 (V, p. 44) suy ra (với $E \neq \{0\}$) rằng
$$
\|u\| = \sup(|m(u)|, |M(u)|).
$$
\* Để xem một chứng minh khác của công thức này khi $K$ là $\mathbf{C}$, xem Mệnh đề 14 của TS, I, § 6, No. 8. \*
2) Cho $M$ và $N$ là hai không gian con vectơ đóng của $E$, và $p_M$ (resp. $p_N$) là phép chiếu trực giao từ $E$ lên $M$ (resp. $N$). Khi đó $M \subset N$ khi và chỉ khi $p_M \leq p_N$. Thật vậy, ta có $p_M^* p_M = p_M$, do đó
$$
\|p_M(x)\|^2 = \langle p_M(x)|p_M(x)\rangle = \langle x|p_M^* p_M(x)\rangle = \langle x|p_M(x)\rangle
$$
với mọi $x \in E$. Vì thế quan hệ $p_M \leq p_N$ tương đương với « $\|p_M(x)\| \leq \|p_N(x)\|$ với mọi $x \in E$ ». Nếu $M \subset N$, ta có $p_M = p_M p_N$, do đó $\|p_M(x)\| \leq \|p_N(x)\|$ vì $\|p_M\| \leq 1$. Ngược lại, nếu $\|p_M(x)\| \leq \|p_N(x)\|$ với mọi $x \in E$, thì hạt nhân của $p_M$ chứa hạt nhân của $p_N$, nghĩa là $M^\circ \supset N^\circ$, điều này suy ra $M \subset N$.

#### Mệnh đề 13 {#evt-v-s4-prop-13 .statement}

— *Cho $\mathcal{H}(E)$ là tập hợp tất cả các tự đồng cấu Hermit liên tục của không gian Hilbert $E$. Cho $\mathcal{F}$ là một tập con không rỗng, có hướng tăng và bị chặn của $\mathcal{H}(E)$.*

(i) *Tập $\mathcal{F}$ có một cận trên $u_0$ trong $\mathcal{H}(E)$; ta có*
$$
\langle x|u_0(x)\rangle = \sup_{u \in \mathcal{F}} \langle x|u(x)\rangle \quad \text{với mọi} \quad x \in E .
$$

(ii) *Bộ lọc các phần cắt của $\mathcal{F}$ hội tụ đến $u_0$ trong không gian $\mathcal{L}(E)$ được trang bị tôpô hội tụ đơn.*

Cho $\Sigma$ là bộ lọc các tiết diện của $\mathcal{F}$; với mỗi $u \in \mathcal{H}(E)$, đặt $\Phi_u$ là dạng Hermit liên tục trên $E$ được xác định bởi
$$
\Phi_u(x, y) = \langle x|u(y)\rangle .
$$
Đặt
$$
\Psi_u(x) = \Phi_u(x, x)
$$
với $u \in \mathcal{H}(E)$ và $x \in E$. Theo các công thức phân cực (V, p. 2), ta có
$$
\begin{align*}
(19) \quad 4\Phi_u(x, y) &= \Psi_u(x+y) - \Psi_u(x-y) & \text{nếu } K = \mathbf{R} \\
(20) \quad 4\Phi_u(x, y) &= \Psi_u(x+y) - \Psi_u(x-y) - i\Psi_u(x+iy) + i\Psi_u(x-iy) & \text{nếu } K = \mathbf{C} .
\end{align*}
$$

Với mọi $x \in E$, ánh xạ $u \mapsto \Psi_u(x)$ vào $\mathbf{R}$ là tăng và bị chặn, nên có một giới hạn đối với $\Sigma$. Theo các công thức trên, giới hạn
$$
\lim_{u,\Sigma} \Phi_u(x, y) = \Phi(x, y)
$$
tồn tại với mọi cặp $(x, y)$ các phần tử của $E$. Rõ ràng $\Phi$ là một dạng Hermit trên $E$. Nếu $v_1 \in \mathcal{F}$ và $v_2$ là một cận trên của $\mathcal{F}$, các dạng Hermit $f_1 = \Phi - \Phi_{v_1}$ và $f_2 = \Phi_{v_2} - \Phi$ là dương; tồn tại một số thực $M \geq 0$ sao cho
$$
f_1(x, x) + f_2(x, x) = \Phi_{v_2 - v_1}(x, x) \leq M \|x\|^2,
$$
do đó
$$
f_1(x, x) \leq M \|x\|^2, \quad f_2(x, x) \leq M \|x\|^2 \quad (x \in E);
$$
do đó các bán chuẩn $x \mapsto f_i(x, x)^{1/2}$ liên tục trên $E$. Vì
$$
f_2 - f_1 = \Phi_{v_2} + \Phi_{v_1} - 2\Phi,
$$
ta kết luận rằng $x \mapsto \Phi(x, x)$ là một hàm liên tục trên $E$, và theo các công thức (19) và (20), rằng $\Phi$ liên tục trên $E \times E$. Do đó tồn tại (V, p. 16, Hệ quả 2) một phần tử $u_0$ của $\mathcal{H}(E)$ sao cho $\Phi = \Phi_{u_0}$. Công thức (18) hiển nhiên được thỏa mãn, do đó $u_0$ là cận trên của $\mathcal{F}$ trong $\mathcal{H}(E)$. Điều này chứng minh (i).

Theo phép dựng, ta có
$$
\lim_{u,\Sigma} \langle x|(u_0 - u)(x)\rangle = 0 \quad \text{với mọi } x \in E.
$$
Cho $v_1 \in \mathcal{F}$; với một $u \in \mathcal{F}$ sao cho $u \geq v_1$, đặt $v = u_0 - u$. Nếu áp dụng bất đẳng thức Cauchy-Schwarz cho dạng Hermit dương $\Phi_v$ trên $E$, ta được
$$
\begin{align*}
\|v(x)\|^4 &= |\Phi_v(v(x), x)|^2 \leq \Phi_v(v(x), v(x)) \cdot \Phi_v(x, x) \\
&= \langle v(x)|v^2(x)\rangle \langle x|v(x)\rangle \leq \|v\|^3 \|x\|^2 \langle x|v(x)\rangle \\
&\leq \|u_0 - v_1\|^3 \|x\|^2 \langle x|v(x)\rangle,
\end{align*}
$$
vì $\|v\| \leq \|u_0 - v_1\|$ theo V, p. 44, Mệnh đề 9. Khi đó theo (21) ta được $\lim_{u,\Sigma} \|(u_0 - u)(x)\| = 0$ với mọi $x \in E$; điều này chứng minh mệnh đề (ii).

Đặc biệt, mệnh đề 13 có thể được áp dụng cho trường hợp của một dãy $(u_n)_{n \in \mathbf{N}}$ tăng và bị chặn của các phần tử của $\mathcal{H}(E)$. Khi đó tồn tại một phần tử $v$ của $\mathcal{H}(E)$ được xác định bởi
$$
\langle x|v(x)\rangle = \lim_{n \to \infty} \langle x|u_n(x)\rangle = \sup_{n \in \mathbf{N}} \langle x|u_n(x)\rangle \quad (x \in E),
$$
và ta có $v(x) = \lim_{n \to \infty} u_n(x)$ với mọi $x \in E$. Hơn nữa, $v$ là cận trên của tập hợp các $u_n$ trong $\mathcal{H}(E)$.

### 6. Vết của một tự đồng cấu

Cho E và F là hai không gian Hilbert. Theo các quy ước của V, p. 40, với $a$ trong E và $b$ trong F, ta ký hiệu $ba^*$ là ánh xạ tuyến tính liên tục $x \mapsto b \langle a|x \rangle$ từ E vào F.

#### Bổ đề 1 {#evt-v-s4-lem-1 .statement}

*Có một đẳng cấu $\theta$ từ không gian vectơ $F \otimes E'$ lên không gian $\mathcal{L}_f(E; F)$ gồm tất cả các ánh xạ tuyến tính liên tục hạng hữu hạn từ E vào F, được đặc trưng bởi $\theta(b \otimes a^*) = ba^*$ với $a \in E, b \in F$.

Theo A, II, § 4, No. 2, tồn tại một ánh xạ tuyến tính đơn ánh $\theta$ từ $F \otimes E'$ vào $\mathcal{L}(E; F)$ và chỉ có một ánh xạ như vậy, biến $b \otimes a'$ thành ánh xạ tuyến tính $x \mapsto ba'(x)$ với $a' \in E', b \in F$. Hiển nhiên $\theta(b \otimes a^*) = ba^*$, và ảnh của $\theta$ được chứa trong $\mathcal{L}_f(E; F)$. Tuy nhiên, cho $u \in \mathcal{L}_f(E; F)$ và cho $(e_1, ..., e_n)$ là một cơ sở trực chuẩn của ảnh của $u$ trong F. Đặt $f_i = u^*(e_i)$ với $1 \leq i \leq n$. Với mọi $x \in E$, ta có

$$
u(x) = \sum_{i=1}^n \langle e_i|u(x) \rangle \cdot e_i = \sum_{i=1}^n \langle f_i|x \rangle \cdot e_i,
$$

suy ra $u = \sum_{i=1}^n e_i f_i^* = \theta(\sum_{i=1}^n e_i \otimes f_i^*)$. Vì vậy ảnh của $\theta$ bằng $\mathcal{L}_f(E; F)$.

Từ nay về sau, ta giả sử rằng $E = F$, và ta đặt $\mathcal{L}_f(E) = \mathcal{L}_f(E; E)$. Theo bổ đề 1, tồn tại duy nhất một dạng tuyến tính $\tau$ trên $\mathcal{L}_f(E)$, sao cho $\tau(\theta(a \otimes a')) = a'(a)$ với $a \in E, a' \in E'$; nói cách khác, ta có

(22)
$$
\tau(ba^*) = \langle a|b \rangle \quad \text{cho } a, b \text{ trong } E.
$$

Khi E hữu hạn chiều, ta có $\mathcal{L}_f(E) = \mathcal{L}(E)$ và $\tau(u)$ là *vết* của tự đồng cấu $u$ của E (A, II, § 4, No. 3).

#### Bổ đề 2 {#evt-v-s4-lem-2 .statement}

*Cho $(e_i)_{i \in I}$ là một cơ sở trực chuẩn của E. Khi đó*

$$
\tau(u) = \sum_{i \in I} \langle e_i|u(e_i) \rangle
$$

*với mọi* $u \in \mathcal{L}_f(E)$.

Chỉ cần xét trường hợp $u = ba^*$ với $a, b$ trong E. Khi đó

$$
\langle e_i|u(e_i) \rangle = e_i^* b \cdot a^* e_i = \overline{\langle e_i|a \rangle} \langle e_i|b \rangle
$$

và bổ đề 2 suy ra từ công thức (22) và công thức (3) của V, p. 22.

#### Bổ đề 3 {#evt-v-s4-lem-3 .statement}

*Cho u là một tự đồng cấu liên tục và dương của E, và $\mathcal{F}$ là tập hợp tất cả các phép chiếu trực giao hạng hữu hạn trên E. Khi đó với mọi cơ sở trực chuẩn $(e_i)_{i \in I}$ của E, ta có (trong $\mathbf{R}_+$) đẳng thức*

$$
\sum_{i \in I} \langle e_i|u(e_i) \rangle = \sup_{p \in \mathcal{F}} \tau(pup).
$$

Với mỗi tập con hữu hạn J của I, đặt $p_J = \sum_{i \in J} e_i e_i^*$; đây là phép chiếu trực giao từ E lên không gian con vectơ sinh bởi các vectơ $e_i$, với i chạy trên J. Ta có
$$
p_J u p_J = \sum_{i \in J, j \in J} \langle e_i | u(e_j) \rangle e_i e_j^* ,
$$
do đó $\tau(p_J u p_J) = \sum_{i \in J} \langle e_i | u(e_i) \rangle$. Vì $p_J \in \mathcal{F}$,
$$
\sum_{i \in J} \langle e_i | u(e_i) \rangle \leq \sup_{p \in \mathcal{F}} \tau(p u p) ;
$$
và do đó ta kết luận rằng
$$
\sum_{i \in I} \langle e_i | u(e_i) \rangle = \sup_J \sum_{i \in J} \langle e_i | u(e_i) \rangle \leq \sup_{p \in \mathcal{F}} \tau(p u p) .
$$

Cho $v$ là một tự đồng cấu liên tục, dương và có hạng hữu hạn của E và cho $p \in \mathcal{F}$. Theo định lý 2 của V, p. 23 tồn tại một cơ sở trực chuẩn $(f_\alpha)_{\alpha \in A}$ của E và một tập con hữu hạn B của A sao cho $(f_\alpha)_{\alpha \in B}$ là một cơ sở trực chuẩn của ảnh của p. Khi đó ta có $p = \sum_{\alpha \in B} f_\alpha f_\alpha^*$, và do đó, như trên, hệ thức $\tau(p v p) = \sum_{\alpha \in B} \langle f_\alpha | v(f_\alpha) \rangle$. Theo bổ đề 2 (V, p. 48) ta có $\tau(v) = \sum_{\alpha \in A} \langle f_\alpha | v(f_\alpha) \rangle$, suy ra công thức
$$
\sum_{\alpha \in B} \langle f_\alpha | v(f_\alpha) \rangle \leq \tau(v) .
$$
Áp dụng bất đẳng thức này cho trường hợp $v = p_J . u p_J$ và J là một tập con hữu hạn của I, ta được
$$
\sum_{\alpha \in B} \langle p_J(f_\alpha) | u p_J(f_\alpha) \rangle \leq \sum_{i \in J} \langle e_i | u(e_i) \rangle .
$$
Với mọi $x \in E$, ta có $p_J(x) = \sum_{i \in J} \langle e_i | x \rangle e_i$, và do đó $x = \lim_J p_J(x)$ đối với tập có hướng có thứ tự gồm các tập con hữu hạn J của I. Chuyển qua giới hạn theo J trong (23), ta được
$$
\tau(p u p) = \sum_{\alpha \in B} \langle f_\alpha | u(f_\alpha) \rangle \leq \sum_{i \in I} \langle e_i | u(e_i) \rangle ,
$$
và điều này hoàn tất chứng minh của bổ đề 3.

#### Định nghĩa 7 {#evt-v-s4-def-7 .statement}

*Cho u là một tự đồng cấu liên tục và dương của không gian Hilbert E. Đặt*
$$
\operatorname{Tr}(u) = \sup_{p \in \mathcal{F}} \tau(p u p)
$$
*(cận trên trong $\overline{\mathbf{R}}_+$), trong đó $\mathcal{F}$ là tập tất cả các phép chiếu trực giao có hạng hữu hạn trên E. Ta nói rằng $\operatorname{Tr}(u)$ là vết của u.*

Cho $p$ là phép chiếu trực giao từ $E$ lên một không gian con vectơ hữu hạn chiều của $E$, và cho $(x_1, ..., x_m)$ là một cơ sở trực chuẩn của F. Ta đã thiết lập hệ thức
$$
\tau(pup) = \sum_{i=1}^m \langle x_i | u(x_i) \rangle.
$$
Do đó, ta có thể định nghĩa vết bởi công thức
$$
\text{Tr}(u) = \sup_{x_1, ..., x_m} \sum_{i=1}^m \langle x_i | u(x_i) \rangle,
$$
trong đó $(x_1, ..., x_m)$ chạy qua tập mọi dãy hữu hạn trực chuẩn của các vectơ của E.

Theo bổ đề 3 (V, p. 48), ta có
$$
\text{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle
$$
với mọi cơ sở trực chuẩn $(e_i)_{i \in I}$ của E. Từ đó, ta suy ra
$$
\text{Tr}(u + v) = \text{Tr}(u) + \text{Tr}(v)
$$
$$
\text{Tr}(\lambda u) = \lambda \cdot \text{Tr}(u)
$$
đối với mọi tự đồng cấu liên tục và dương $u$ và $v$ của E và với mọi số thực $\lambda \geq 0$ (ta quy ước $0.(+\infty) = 0$ trong (27)). Cho $\phi$ là một đẳng cấu từ E lên một không gian Hilbert F; vì $\phi$ biến mọi cơ sở trực chuẩn của E thành một cơ sở trực chuẩn của F, từ (25) ta được
$$
\text{Tr}(\phi u \phi^{-1}) = \text{Tr}(u).
$$

Cho $(u_\alpha)_{\alpha \in A}$ là một họ không rỗng, có hướng, tăng và bị chặn của các tự đồng cấu liên tục và dương của E; cho $u = \sup_\alpha u_\alpha$, khi đó $\langle x | u(x) \rangle = \sup_\alpha \langle x | u_\alpha(x) \rangle$ với mọi $x \in E$ (V, p. 46, mệnh đề 13). Ta có $\text{Tr}(u) = \sup_{J \subset I} \sum_{i \in J} \langle e_i | u(e_i) \rangle$, trong đó J chạy qua mọi tập con hữu hạn của I, do đó
$$
\text{Tr}(u) = \sup_\alpha \text{Tr}(u_\alpha) \quad \text{với} \quad u = \sup_\alpha u_\alpha.
$$

Cho $p_F$ là phép chiếu trực giao từ $E$ lên không gian con Hilbert $F$; tồn tại một cơ sở trực chuẩn $(e_i)_{i \in I}$ của $E$ và một tập con $J$ của $I$, sao cho $(e_i)_{i \in J}$ là một cơ sở trực chuẩn của $F$. Ta có $\text{Tr}(p_F up_F) = \sum_{i \in J} \langle e_i | u(e_i) \rangle$. Công thức này có hai hệ quả: thứ nhất, ta có $\text{Tr}(p_F up_F) \leq \text{Tr}(u)$; thứ hai, lấy $u = 1_E$, ta được
$$
\text{Tr}(p_F) = \begin{cases}
\dim F & \text{nếu } F \text{ là hữu hạn chiều} \\
+ \infty & \text{nếu không}.
\end{cases}
$$

#### Định nghĩa 8 {#evt-v-s4-def-8 .statement}

— Cho $E$ là một không gian Hilbert phức. Ta viết $\mathcal{L}^1(E)$ cho không gian con vectơ của $\mathcal{L}(E)$ sinh bởi mọi tự đồng cấu liên tục, dương của E có vết hữu hạn.

Nhờ công thức (25) của V, p. 50, vết mở rộng thành một dạng tuyến tính trên $\mathcal{L}^1(E)$, cũng được ký hiệu là Tr, và thỏa mãn quan hệ $\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle$ với mọi $u$ trong $\mathcal{L}^1(E)$ và với mọi cơ sở trực chuẩn $(e_i)_{i \in I}$ của E. Với mọi $u \in \mathcal{L}^1(E)$, ta có $u^* \in \mathcal{L}^1(E)$ và $\operatorname{Tr}(u^*) = \overline{\operatorname{Tr}(u)}$. Các công thức (25) và (28) của V, p. 50 vẫn đúng trong trường hợp $u$ thuộc $\mathcal{L}^1(E)$. Cho F là một không gian con Hilbert của E; theo công thức (30), phép chiếu trực giao $p_F$ thuộc $\mathcal{L}^1(E)$ khi và chỉ khi F là hữu hạn chiều. Với mọi a và b trong E, ta có $4ab^* = \sum_{\varepsilon^4 = 1} \varepsilon(a + \varepsilon b)(a + \varepsilon b)^*$ và $cc^*$ là một toán tử dương có vết hữu hạn với mọi $c \in E$; do đó, nếu $u$ là một tự đồng cấu liên tục của E có hạng hữu hạn, thì $u \in \mathcal{L}^1(E)$ và $\operatorname{Tr}(u) = \tau(u)$.

Cho E là một không gian Hilbert thực, và cho $E_{(c)}$ là phức hóa của nó (V, p. 5). Ta đồng nhất E với một tập con của $E_{(c)}$. Khi đó $\mathcal{L}(E)$ có thể được đồng nhất với một không gian con vectơ thực của $\mathcal{L}(E_{(c)})$ gồm tất cả các ánh xạ tuyến tính liên tục $u$ từ $E_{(c)}$ vào $E_{(c)}$ sao cho $u(E) \subset E$. Trong trường hợp này ta viết $\mathcal{L}^1(E) = \mathcal{L}(E) \cap \mathcal{L}^1(E_{(c)})$. Với mọi $u \in \mathcal{L}^1(E)$, vết $\operatorname{Tr}(u)$ là thực và bằng $\operatorname{Tr}(u^*)$. Các công thức (25) và (28) lại đúng, $\mathcal{L}_f(E) \subset \mathcal{L}^1(E)$ và $\operatorname{Tr}(u) = \tau(u)$ với mọi $u \in \mathcal{L}_f(E)$. Sau cùng, một không gian con vectơ đóng F của E là hữu hạn chiều khi và chỉ khi $p_F$ thuộc $\mathcal{L}^1(E)$.

\* Nhận xét 1. — Sau này chúng ta sẽ định nghĩa khái niệm một ánh xạ hạt nhân từ một không gian Banach E vào một không gian Banach F. Chúng ta sẽ chứng minh rằng khi $\mathcal{L}^1(E)$ gồm tất cả các ánh xạ hạt nhân từ E vào E, thì E là một không gian Hilbert thực hoặc phức. \*

#### Mệnh đề 14 {#evt-v-s4-prop-14 .statement}

— Cho $E_1, ..., E_n$ là các không gian Hilbert, $E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$, và $u_i$ là một tự đồng cấu liên tục của $E_i$ với $1 \leq i \leq n$. Nếu $u_1, ..., u_n$ dương, thì $u = u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$ cũng dương, và

$$
\operatorname{Tr}(u) = \prod_{i=1}^n \operatorname{Tr}(u_i).
$$

Nếu $u_i \in \mathcal{L}^1(E_i)$ với mọi $1 \leq i \leq n$, thì $u \in \mathcal{L}^1(E)$ và công thức (31) vẫn đúng trong trường hợp này.

Làm quy nạp theo $n$, ta ngay lập tức rút gọn về trường hợp $n = 2$.

Với $i = 1, 2$, ta định nghĩa một dạng sesquilinear $\Phi_i$ trên $E_i$ bởi công thức $\Phi_i(x, y) = \langle x | u_i(y) \rangle$ với $x, y$ trong $E_i$. Nếu $u_1$ và $u_2$ dương, thì các dạng $\Phi_1$ và $\Phi_2$ là Hermit và dương. Theo Mệnh đề 1 của V, p. 25 tồn tại một dạng Hermit dương trên không gian vectơ $E_1 \otimes E_2$ sao cho

$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = \Phi_1(x_1, y_1) \cdot \Phi_2(x_2, y_2)
$$

với $x_1, y_1$ trong $E_1$ và $x_2, y_2$ trong $E_2$. Ta kiểm tra ngay lập tức quan hệ $\Phi(z, t) = \langle z | u(t) \rangle$ với $z$ và $t$ trong $E_1 \otimes E_2$. Vì $\Phi$ dương, ta có $\langle z | u(z) \rangle \geq 0$ với mọi $z$ trong $E_1 \otimes E_2$. Vì $u$ liên tục và $E_1 \otimes E_2$ trù mật trong không gian Hilbert $E = E_1 \hat{\otimes}_2 E_2$, ta kết luận rằng $u$ là một tự đồng cấu liên tục và dương của E.

Cho $(e_i)_{i \in I}$ là một cơ sở trực chuẩn của $E_1$ và $(f_j)_{j \in J}$ là một cơ sở trực chuẩn của $E_2$; khi đó họ $(e_i \otimes f_j)_{i \in I, j \in J}$ là một cơ sở trực chuẩn của $E$ và ta có

$$
\operatorname{Tr}(u) = \sum_{i \in I} \sum_{j \in J} \langle e_i \otimes f_j | u(e_i \otimes f_j) \rangle \\
= \sum_{i \in I} \sum_{j \in J} \langle e_i | u_1(e_i) \rangle \cdot \langle f_j | u_2(f_j) \rangle \\
= \operatorname{Tr}(u_1) \cdot \operatorname{Tr}(u_2) .
$$

Đặc biệt, nếu $u_1$ và $u_2$ là các tự đồng cấu dương có vết hữu hạn, thì $u$ cũng vậy. Do tính tuyến tính, ta suy ra rằng $u$ thuộc $\mathcal{L}^1(E)$ khi $K = \mathbf{C}$ và rằng các $u_i$ thuộc $\mathcal{L}^1(E_i)$ với $i = 1, 2$; công thức (31) mở rộng sang trường hợp này bởi tính tuyến tính. Cuối cùng, trường hợp $K = \mathbf{R}$ và các $u_i \in \mathcal{L}^1(E_i)$ rút gọn về trường hợp phức bằng mở rộng vô hướng.

#### Nhận xét 2 {#evt-v-s4-n6-rem-2 .statement}

— Cho $E$ là một không gian Hilbert, là tổng Hilbert của một họ $(E_i)_{i \in I}$ các không gian con Hilbert. Cho $u$ là một phần tử của $\mathcal{L}(E)$ sao cho $u(E_i) \subset E_i$ với mọi $i \in I$; cho $u_i$ là phần tử của $\mathcal{L}(E_i)$ trùng với $u$ trên $E_i$. Khi đó $\operatorname{Tr}(u) = \sum_{i \in I} \operatorname{Tr}(u_i)$ khi $u$ dương, hoặc thuộc $\mathcal{L}^1(E)$; quan hệ này suy ra từ công thức (25) của V, p. 50 áp dụng cho một cơ sở trực chuẩn của $E$ là hợp của các cơ sở trực chuẩn của từng $E_i$.

### 7. Các ánh xạ Hilbert-Schmidt

#### Định nghĩa 9 {#evt-v-s4-def-9 .statement}

*Cho $E$ và $F$ là hai không gian Hilbert. Một ánh xạ tuyến tính liên tục $u$ từ $E$ vào $F$ được gọi là một ánh xạ Hilbert-Schmidt nếu vết của tự đồng cấu dương $u^*u$ của $E$ là hữu hạn. Tập hợp của tất cả các ánh xạ Hilbert-Schmidt từ $E$ vào $F$ được ký hiệu bởi $\mathcal{L}^2(E, F)$. \*

Khi $E = F$, ta viết $\mathcal{L}^2(E)$ thay cho $\mathcal{L}^2(E; E)$.

Với mọi $u \in \mathcal{L}(E, F)$, cho $\|u\|_2 = \operatorname{Tr}(u^*u)^{1/2}$, do đó $u$ thuộc $\mathcal{L}^2(E; F)$ khi và chỉ khi $\|u\|_2$ hữu hạn. Theo định nghĩa của vết, ta có

$$
\|u\|_2^2 = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \|u(x_i)\|^2
$$

trong đó $(x_1, \ldots, x_m)$ chạy qua tập hợp các dãy trực chuẩn hữu hạn trong $E$. Đặc biệt, lấy $m = 1$ trong công thức (32), ta có

$$
\|u\| \leq \|u\|_2 \quad (u \in \mathcal{L}(E; F)) .
$$

Cho $(e_i)_{i \in I}$ là một cơ sở trực chuẩn của $E$ và $(f_j)_{j \in J}$ là một cơ sở trực chuẩn của $F$. Theo công thức (25) của V, p. 50 và hệ thức Parseval (V, p. 22), ta có

$$
\|u\|_2^2 = \sum_{i \in I} \|u(e_i)\|^2 = \sum_{i,j} |\langle f_j | u(e_i) \rangle|^2 .
$$

Vì $|\langle f_j|u(e_i)\rangle| = |\langle e_i|u^*(f_j)\rangle|$, nên công thức (34) suy ra rằng
$$
\|u^*\|_2 = \|u\| ;
$$
do đó, ánh xạ liên hợp của một ánh xạ Hilbert-Schmidt là một ánh xạ Hilbert-Schmidt. Cho $E_1, F_1$ là các không gian Hilbert và $v : E_1 \to E, w : F \to F_1$ là các ánh xạ tuyến tính liên tục. Từ (32), suy ra ngay lập tức rằng
$$
\|wu\|_2 \leq \|w\|.\|u\|_2 .
$$
Theo (35), (36) và quan hệ $uv = (v^*u^*)^*$, ta có
$$
\|uv\|_2 \leq \|u\|_2\,\|v\| .
$$
Đặc biệt, nếu $u$ thuộc $\mathcal{L}^2(E, F)$ thì $wuv$ thuộc $\mathcal{L}^2(E_1, F_1)$.

#### Định lý 1 {#evt-v-s4-thm-1 .statement}

*Cho E và F là hai không gian hilbert.*
(i) *Tập $\mathcal{L}^2(E, F)$ là một không gian con vectơ của $\mathcal{L}(E; F)$ và $u \mapsto \|u\|_2$ là một chuẩn hilbert* (V, p. 6) *trên $\mathcal{L}^2(E; F)$.*
(ii) *Đẳng cấu $\theta$ từ $F \otimes E'$ lên $\mathcal{L}_f(E; F)$ được xác định bởi $\theta(y \otimes x^*) = yx^*$ được mở rộng thành một đẳng cấu $\hat{\theta}$ từ $F \otimes_2 E'$ lên $\mathcal{L}^2(E; F)$. Đặc biệt, $\mathcal{L}_f(E; F)$ trù mật trong $\mathcal{L}^2(E; F)$.*

Với $(e_i)_{i \in I}$ (resp. $(f_j)_{j \in J}$) là một cơ sở trực chuẩn của $E$ (resp. $F$). Với mọi $u \in \mathcal{L}(E; F)$, gọi $\Lambda(u)$ là ma trận của $u$ theo các cơ sở trực chuẩn đã chọn của $E$ và $F$ (V, p. 22). Ký hiệu $\|a\|_2$ là chuẩn của một phần tử $a$ của không gian hilbert $\ell^2(J \times I)$. Theo công thức (34), $\Lambda$ là một ánh xạ từ $\mathcal{L}^2(E; F)$ vào $\ell^2(J \times I)$ sao cho $\|\Lambda(u)\|_2 = \|u\|$; hiển nhiên $\Lambda$ là *đơn ánh*. Để chứng minh (i), chỉ cần chứng minh rằng $\Lambda$ là *toàn ánh*. Cho $a = (a_{ji})$ là một phần tử của $\ell^2(J \times I)$; theo bất đẳng thức Cauchy-Schwarz, ta có
$$
|\sum_{j,i} \overline{\eta}_j a_{ji} \xi_i|^2 \leq \sum_{j,i} |a_{ji}|^2 \sum_{j,i} |\overline{\eta}_j \xi_i|^2 = \|a\|_2^2\,\|\xi\|^2\,\|\eta\|^2
$$
với mọi $\xi = (\xi_i)$ trong $\ell^2(I)$ và $\eta = (\eta_j)$ trong $\ell^2(J)$. Khi đó tồn tại một dạng sesquilinear liên tục $\Phi$ trên $F \times E$ sao cho $\Phi(y, x) = \sum_{j,i} \overline{\eta}_j a_{ji} \xi_i$ với $x = \sum_i \xi_i e_i$ trong $E$ và $y = \sum_j \eta_j f_j$ trong $F$. Chọn $u \in \mathcal{L}(E; F)$ sao cho $\Phi(y, x) = \langle y|u(x)\rangle$ (V, p. 16, cor. 2). Ta được
$$
a_{ji} = \Phi(f_j, e_i) = \langle f_j|u(e_i)\rangle \quad \text{với} \quad i \in I, j \in J ,
$$
suy ra $a = \Lambda(u)$.

Vì $\Lambda$ là một đẳng cấu giữa các không gian hilbert từ $\mathcal{L}^2(E; F)$ lên $\ell^2(J \times I)$ và vì $(f_j \otimes e_i^*)$ là một cơ sở trực chuẩn của $F \otimes_2 E'$, nên tồn tại một đẳng cấu $\hat{\theta}$ từ $F \otimes_2 E'$ lên $\mathcal{L}^2(E; F)$ sao cho
$$
\langle f_j|\hat{\theta}(t)\,e_i\rangle = \langle f_j \otimes e_i^*|t\rangle
$$

với mọi $i \in I,\ j \in I$ và $t \in F \otimes_2 E'$. Đặc biệt, với $t = y \otimes x^*$, ta được
$$
\langle f_j | \hat{\theta}(y \otimes x^*) e_i \rangle = \langle f_j \otimes e_i^* | y \otimes x^* \rangle = \langle f_j | y \rangle \langle x | e_i \rangle = \langle f_j | y x^* e_i \rangle
$$
do đó $\hat{\theta}(y \otimes x^*) = y x^*$. Điều này chứng minh (ii). Q.E.D.

#### Ví dụ 1 {#evt-v-s4-n7-exa-1 .statement}

Cho I và J là hai tập hợp. Theo chứng minh đã cho ở trên, để một ánh xạ $u$ từ $\ell^2(I)$ vào $\ell^2(J)$ là một ánh xạ Hilbert-Schmidt, điều kiện cần và đủ là tồn tại một ma trận $(a_{ji})$ trong $\ell^2(J \times I)$ sao cho $u(\xi)_j = \sum_{i \in I} a_{ji} \xi_i$ với mọi $\xi = (\xi_i)$ trong $\ell^2(I)$.

#### Ví dụ 2 {#evt-v-s4-n7-exa-2 .statement}

Cho X và Y là hai không gian tôpô Hausdorff, được trang bị lần lượt các độ đo dương $\mu$ và $\nu$. Ta có thể chứng minh rằng các ánh xạ Hilbert-Schmidt từ $\mathcal{L}^2(X)$ vào $\mathcal{L}^2(Y)$ tương ứng song ánh với các lớp của các hàm khả tích bình phương trên $Y \times X$; với lớp của một hàm $N \in \mathcal{L}^2(Y \times X, \nu \otimes \mu)$ tương ứng là ánh xạ $u_N$ cho bởi
$$
(u_N f)(y) = \int_X N(y, x) f(x) \, d\mu(x)
$$
với $\nu$-hầu khắp mọi $y \in Y$ và $f \in \mathcal{L}^2(X, \mu)$. Ta có
$$
\| u_N \|_2^2 = \int_X \int_Y |N(y, x)|^2 \, d\mu(x) \, d\nu(y) .
$$

#### Nhận xét 1 {#evt-v-s4-n7-rem-1 .statement}

Giả sử $K = \mathbf{C}$. Cho $u$ và $v$ thuộc $\mathcal{L}^2(E; F)$. Ta có quan hệ
$$
4\, u^* v = \sum_{\varepsilon^4 = 1} \overline{\varepsilon}(u + \varepsilon v)^* (u + \varepsilon v),
$$
do đó $u^* v$ thuộc $\mathcal{L}^1(E)$. Tích vô hướng trong không gian Hilbert $\mathcal{L}^2(E; F)$ được cho bởi
$$
\langle u | v \rangle = \operatorname{Tr}(u^* v)
$$
vì công thức này xác định một dạng Hermit trên $\mathcal{L}^2(E; F)$ và ta thu được $\langle u | u \rangle = \| u \|_2^2$.

Nếu $u \in \mathcal{L}^2(E; F)$ và $v \in \mathcal{L}^2(F; E)$, thì theo trên $vu$ thuộc $\mathcal{L}^1(E)$ và $uv$ thuộc $\mathcal{L}^1(F)$; hơn nữa, ta có
$$
\operatorname{Tr}(uv) = \operatorname{Tr}(vu) .
$$
Nhờ tính tuyến tính và tính liên tục, chỉ cần kiểm tra công thức này khi $u = y_1 x_1^*$ và $v = x_2 y_2^*$ (với $x_1, x_2$ trong E, $y_1, y_2$ trong F); nhưng khi đó $uv$ là ánh xạ $y \mapsto y_1 \langle x_1 | x_2 \rangle \langle y_2 | y \rangle$ và $vu$ là ánh xạ $x \mapsto x_2 \langle y_2 | y_1 \rangle \langle x_1 | x \rangle$, và (41) suy ra từ công thức (22) của V, p. 48.

Do đó, nếu $u_1, u_2$ là hai phần tử của $\mathcal{L}^2(E; F)$, ta có, trong không gian Hilbert $\mathcal{L}^2(F; E)$, $$
\langle u_1^* | u_2^* \rangle = \operatorname{Tr}(u_1 u_2^*) = \operatorname{Tr}(u_2^* u_1) = \langle u_2 | u_1 \rangle = \overline{\langle u_1 | u_2 \rangle} ;
$$ nói cách khác, $u \mapsto u^*$ là một đẳng cấu từ không gian Hilbert $\mathcal{L}^2(E; F)$ lên không gian liên hợp (V, p. 6) của không gian Hilbert $\mathcal{L}^2(F; E)$. Nếu ta đồng nhất không gian liên hợp này với không gian đối ngẫu của $\mathcal{L}^2(F; E)$ (V, p. 15), ta thấy rằng $\mathcal{L}^2(E; F)$ có thể được đồng nhất với không gian đối ngẫu của $\mathcal{L}^2(F; E)$, với dạng song tuyến tính chính tắc $(v, u) \mapsto \langle v, u \rangle$ được đồng nhất với $(v, u) \mapsto \operatorname{Tr}(vu)$.

#### Nhận xét 2 {#evt-v-s4-n7-rem-2 .statement}

Giả sử $K = \mathbf{R}$. Chúng tôi để bạn đọc kiểm tra rằng các công thức (40) và (41) vẫn đúng, và hãy chứng minh rằng $\mathcal{L}^2(E; F)$ có thể được đồng nhất với không gian đối ngẫu của $\mathcal{L}^2(F; E)$ nhờ dạng song tuyến tính $(u, v) \mapsto \operatorname{Tr}(uv)$.

### 8. Chéo hóa các ánh xạ Hilbert-Schmidt

#### Định lý 2 {#evt-v-s4-thm-2 .statement}

*Cho E và F là hai không gian Hilbert và u là một ánh xạ Hilbert-Schmidt từ E vào F. Tồn tại một cơ sở trực chuẩn $(e_i)_{i \in I}$ của E được u biến thành một họ trực giao trong F.*

Ký hiệu B là quả cầu đơn vị (đóng) của E, với tôpô yếu được gán cho nó; đó là một không gian compact (V, p. 17). Đặt $Q(x) = \|u(x)\|^2$ với mọi $x \in B$. Cuối cùng, ký hiệu P là tập hợp tất cả các vectơ x trong E thỏa mãn tính chất sau ;

(H) *Với mọi $y \in E$ trực giao với x, phần tử $u(y)$ của E trực giao với $u(x)$.*

#### Bổ đề 4 {#evt-v-s4-lem-4 .statement}

*Hàm $Q : B \to \mathbf{R}$ liên tục.*

Cho $(f_j)_{j \in J}$ là một cơ sở trực chuẩn của F. Đặt $\lambda_j = \|u^*(f_j)\|^2$ với mọi $j \in J$. Vì $u$ thuộc $\mathcal{L}^2(E; F)$ nên $u^* \in \mathcal{L}^2(F; E)$, do đó $\sum_j \lambda_j < +\infty$. Hơn nữa, ta có
$$
Q(x) = \|u(x)\|^2 = \sum_j |\langle u^*(f_j)|x \rangle|^2
$$
theo công thức Parseval (V, p. 22) và định nghĩa của toán tử liên hợp (V, p. 38). Với mọi $x \in B$, $|\langle u^*(f_j)|x \rangle|^2 \leq \lambda_j$ theo bất đẳng thức Cauchy-Schwarz; do đó, sự hội tụ của tổng trong công thức (43) là đều trên B, suy ra bổ đề 4 (GT, X, § 1, No. 6).

#### Bổ đề 5 {#evt-v-s4-lem-5 .statement}

*Cho $E_1$ là một không gian con vectơ đóng của E, ổn định dưới $u^*u$. Nếu $E_1 \neq \{0\}$, thì tồn tại một vectơ có chuẩn 1 trong $E_1 \cap P$.*

Vì B compact yếu, nên không gian con đóng yếu $B \cap E_1$ của B cũng compact yếu. Do đó tồn tại (GT, IV, § 6, No. 1, th. 1) một điểm $x_0$ trong $B \cap E_1$ sao cho $Q(x_0) \geq Q(x)$ với mọi $x \in B \cap E_1$. Nếu $Q(x_0) = 0$, ta có $Q(x) = 0$ và do đó $u(x) = 0$ với mọi $x \in B \cap E_1$. Suy ra $E_1 \subset P$ và bổ đề 5 suy ra trong trường hợp này.

Giả sử bây giờ rằng $Q(x_0) > 0$, thì $x_0 \neq 0$. Vì vectơ $\|x_0\|^{-1} \cdot x_0$ thuộc $B \cap E_1$, ta có
$$
Q(x_0) \geq Q(\|x_0\|^{-1} \cdot x_0) = Q(x_0)/\|x_0\|^2
$$
*tức là* $\|x_0\| = 1$. Ta sẽ chứng minh rằng $x_0$ thuộc P; cho $y \in E$ vuông góc với $x_0$. Chỉ cần chứng minh rằng $u(y)$ vuông góc với $u(x_0)$. Nhưng vì $y$ là tổng của một vectơ của $E_1$ và một vectơ vuông góc với $E_1$, và cả hai đều vuông góc với $x_0$ (vì $x_0 \in E_1$), nên chỉ cần xét hai trường hợp sau:

a) $y$ vuông góc với $E_1$: vì $E_1$ ổn định dưới $u^*u$, $u^*u(x_0) \in E_1$, do đó $0 = \langle y|u^*u(x_0)\rangle = \langle u(y)|u(x_0)\rangle$.

b) $y$ thuộc $E_1$: với mọi $t \in \mathbf{R}$, vectơ $x(t) = (x_0 + ty)/\|x_0 + ty\|$ thuộc $B \cap E_1$. Ta có $Q(xt) = f(t)/g(t)$ với
$$
f(t) = \|u(x_0)\|^2 + 2t \Re \langle u(x_0)|u(y)\rangle + t^2 \|u(y)\|^2 \\
g(t) = 1 + t^2 \|y\|^2 .
$$
Xét đến định nghĩa của $x_0$, ta có $Q(x(0)) \geq Q(x(t))$ với mọi $t$ thực, do đó $\frac{d}{dt} Q(x(t))$ bằng không khi $t = 0$. Nhưng $f(0) = \|u(x_0)\|^2$, $g(0) = 1$, $f'(0) = 2 \Re \langle u(x_0)|u(y)\rangle$, $g'(0) = 0$. Vì
$$
\frac{d}{dt} Q(x(t)) = \frac{f'(t)\,g(t) - f(t)\,g'(t)}{g(t)^2},
$$
ta suy ra rằng $f'(0) = 0$, tức là $\Re \langle u(x_0)|u(y)\rangle = 0$. Khi $K = \mathbf{R}$, $u(x_0)$ vuông góc với $u(y)$, khi $K = \mathbf{C}$, vectơ $iy$ thuộc $E_1$ và vuông góc với $x_0$, do đó $\mathcal{I} \langle u(x_0)|u(y)\rangle = -\Re \langle u(x_0)|u(iy)\rangle = 0$, và cuối cùng $u(x_0)$ vuông góc với $u(y)$. Điều này chứng minh bổ đề 5.

Ta chứng minh định lý 2. Áp dụng định lý 1 của S, III, § 4, No. 5 ta thấy, như ở V, p. 23, rằng tồn tại một tập hợp $S$ cực đại trong số các tập con trực chuẩn của $E$ được chứa trong $P$. Gọi $E_1$ là tập hợp tất cả các vectơ trực giao với $S$. Cho $y \in E_1$; nếu $x \in S$, thì các vectơ $x$ và $y$ trực giao, và vì $S \subset P$, ta suy ra rằng $u(x)$ và $u(y)$ trực giao; khi đó
$$
\langle x|u^*u(y)\rangle = \langle u(x)|u(y)\rangle = 0
$$
và $u^*u(y)$ trực giao với $S$. Do đó $E_1$ ổn định dưới $u^*u$. Nếu $E_1 \neq \{0\}$, thì sẽ tồn tại một vectơ $x$ có chuẩn 1 trong $E_1 \cap P$ (bổ đề 5) và $S \cup \{x\}$ sẽ là một tập con trực chuẩn của $E$ được chứa trong $P$. Điều này mâu thuẫn với tính cực đại của $S$. Suy ra $E_1 = \{0\}$ và $S$ là một cơ sở trực chuẩn của $E$. ĐPCM.

#### Hệ quả 1 {#evt-v-s4-lem-5-cor-1 .statement}

— *Cho $v$ là một tự đồng cấu liên tục, dương có vết hữu hạn của không gian Hilbert $E$. Tồn tại một cơ sở trực chuẩn $(e_i)_{i \in I}$ của $E$ và một họ khả tổng các số thực dương $(\lambda_i)_{i \in I}$ sao cho $v(e_i) = \lambda_i e_i$ với mọi $i \in I$.*

Đặt $\Phi(x, y) = \langle x|v(y)\rangle$ với $x, y$ trong $E$. Khi đó $\Phi$ là một dạng Hermit dương trên $E$. Tồn tại (V, p. 8, hệ quả) một không gian Hilbert $F$ và một ánh xạ tuyến tính liên tục $u$ từ $E$ vào $F$ sao cho $\Phi(x, y) = \langle u(x)|u(y)\rangle$ với $x, y$ trong $E$. Nói cách khác, ta có $v = u^*u$. Theo định nghĩa 9 (V, p. 52), $u$ là một ánh xạ Hilbert-Schmidt từ $E$ vào $F$. Theo định lý 2, tồn tại một cơ sở trực chuẩn $(e_i)_{i \in I}$ của $E$ sao cho các vectơ $u(e_i)$ đôi một trực giao. Lấy $i \in I$; với mọi $j \neq i$ trong $I$, ta có
$$
\langle e_j|v(e_i)\rangle = \langle u(e_j)|u(e_i)\rangle = 0
$$

do đó $v(e_i)$ tỉ lệ với $e_i$ và có dạng $\lambda_i e_i$, trong đó $\lambda_i = \langle e_i | v(e_i) \rangle$; khi đó

$$
\lambda_i \geqslant 0 \quad \text{và} \quad \sum_{i \in I} \lambda_i = \operatorname{Tr}(v) < + \infty .
$$

#### Hệ quả 2 {#evt-v-s4-lem-5-cor-2 .statement}

*Cho E là một không gian Hilbert. Khi đó $\mathcal{L}^1(E) \subset \mathcal{L}^2(E)$.*

Trường hợp thực quy về trường hợp phức bằng mở rộng vô hướng; do đó có thể giả sử rằng $K = \mathbf{C}$.

Vì $\mathcal{L}^2(E)$ là một không gian con vectơ của $\mathcal{L}(E)$, chỉ cần chứng minh rằng mọi tự đồng cấu dương liên tục $v$ của E có vết hữu hạn đều thuộc $\mathcal{L}^2(E)$. Với các ký hiệu của hệ quả 1, ta có

$$
\sum_{i \in I} \| v(e_i) \|^2 = \sum_{i \in I} \lambda_i^2 \leq (\sum_i \lambda_i)^2 < + \infty .
$$

#### Hệ quả 3 {#evt-v-s4-lem-5-cor-3 .statement}

*Cho v là một tự đồng cấu dương liên tục của không gian Hilbert E có vết hữu hạn. Tồn tại một tự đồng cấu Hilbert-Schmidt dương w của E sao cho $v = w^2$ và sao cho v giao hoán với w.*

Với các ký hiệu của hệ quả 1, chỉ cần xét tự đồng cấu w biến vectơ $\sum_{i \in I} \xi_i e_i$ thành vectơ $\sum_i \lambda_i^{1/2} \xi_i e_i$.

#### Nhận xét {#evt-v-s4-n8-rem-1 .statement}

— Với các ký hiệu của định lý 2, cho J là tập hợp tất cả các i \in I sao cho $u(e_i) \neq 0$. Với mọi i \in J, đặt $\lambda_i = \| u(e_i) \|$ và $f_i = \lambda_i^{-1} u(e_i)$. Khi đó $(e_i)_{i \in J}$ (tương ứng $(f_i)_{i \in J}$) là một cơ sở trực chuẩn của không gian con ban đầu (tương ứng cuối) của u, ta có $u(e_i) = \lambda_i f_i$ với mọi i \in J và $\sum_{i \in J} \lambda_i^2 = \| u \|_2^2$ là hữu hạn.

### 9. Vết của một dạng toàn phương đối với một dạng khác

Trong tiết này, E sẽ ký hiệu một không gian vectơ thực và Q, H là hai *dạng toàn phương dương* trên E. Có hai dạng song tuyến tính đối xứng $(x, y) \mapsto \langle x | y \rangle_Q$ và $(x, y) \mapsto \langle x | y \rangle_H$ trên $E \times E$, được đặc trưng bởi

$$
Q(x) = \langle x | x \rangle_Q , \quad H(x) = \langle x | x \rangle_H
$$

với mọi $x \in E$.

Ta gọi *vết của Q theo H*, và viết $\operatorname{Tr}(Q/H)$, là một số thực dương, hữu hạn hay không, được định nghĩa như sau :

*a)* Nếu tồn tại $x \in E$ sao cho $H(x) = 0$ và $Q(x) \neq 0$, ta đặt $\operatorname{Tr}(Q/H) = + \infty$.

*b)* Ngược lại, $\operatorname{Tr}(Q/H)$ là cận trên của tập hợp tất cả các số có dạng $\sum_{i=1}^m Q(x_i)$, trong đó $(x_1, ..., x_m)$ chạy qua tập hợp các dãy hữu hạn các phần tử của E sao cho $\langle x_i | x_j \rangle_H = \delta_{ij}$ (ký hiệu Kronecker).

#### Nhận xét {#evt-v-s4-n9-rem-1 .statement}

— 1) Với mọi không gian con F của E, ký hiệu $Q_F$ là hạn chế của Q lên F và $H_F$ là hạn chế của H lên F. Ta có $\operatorname{Tr}(Q_F/H_F) \leq \operatorname{Tr}(Q/H)$ và $\operatorname{Tr}(Q/H)$ là cận trên của tập hợp tất cả các số $\operatorname{Tr}(Q_F/H_F)$, trong đó F chạy qua họ tất cả các không gian con vectơ hữu hạn chiều của E.

2) Cho $E_1$ là một không gian vectơ thực, $Q_1$ và $H_1$ là hai dạng toàn phương dương trên $E_1$ và $\pi : E \to E_1$ là một ánh xạ tuyến tính toàn ánh. Nếu $Q = Q_1 \circ \pi$ và $H = H_1 \circ \pi$, thì $\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1)$.

#### Mệnh đề 15 {#evt-v-s4-prop-15 .statement}

*Giả sử tồn tại một cấu trúc không gian Hilbert thực trên $E$ sao cho $H(x) = \|x\|^2$ với mọi $x \in E$. Để $\operatorname{Tr}(Q/H)$ hữu hạn, cần và đủ là tồn tại một tự đồng cấu liên tục và dương $u$ của $E$ có vết hữu hạn, sao cho $Q(x) = \langle x|u(x)\rangle$ với mọi $x \in E$; tự đồng cấu $u$ này là duy nhất, và ta có*

$$
\operatorname{Tr}(u) = \operatorname{Tr}(Q/H) = \sum_{i \in I} Q(e_i)
$$

*với mọi cơ sở trực chuẩn $(e_i)_{i \in I}$ của $E$.*

Giả sử $\operatorname{Tr}(Q/H)$ hữu hạn. Với mọi $x \in E$ có chuẩn 1, ta có $H(x) = 1$, do đó $Q(x) \leq \operatorname{Tr}(Q/H)$. Vì vậy, $Q(x) \leq \operatorname{Tr}(Q/H) \cdot \|x\|^2$ với mọi $x \in E$, và

$$
|\langle x|y\rangle_Q| \leq Q(x)^{1/2} Q(y)^{1/2} \leq \operatorname{Tr}(Q/H) \cdot \|x\| \cdot \|y\|
$$

theo bất đẳng thức Cauchy-Schwarz. Do đó, dạng song tuyến tính $(x, y) \mapsto \langle x|y\rangle_Q$ trên $E \times E$ là liên tục. Có (V, p. 16, hệ quả 2) một ánh xạ $u \in \mathcal{L}(E)$ sao cho $\langle x|y\rangle_Q = \langle x|u(y)\rangle$. Ta có $\langle x|y\rangle_Q = \langle y|x\rangle_Q$ với $x, y$ trong $E$, nên $u$ là Hermit; và $\langle x|u(x)\rangle = Q(x) \geq 0$, nên $u$ là dương.

Ngược lại, cho $u$ là một tự đồng cấu liên tục và dương của $E$ sao cho $Q(x) = \langle x|u(x)\rangle$ với mọi $x \in E$. Khi đó

$$
\langle x|u(y)\rangle = \frac{1}{2}(Q(x + y) - Q(x) - Q(y)) = \langle x|y\rangle_Q,
$$

điều này cho tính duy nhất của $u$. Theo công thức (24') (V, p. 50), ta được

$$
\operatorname{Tr}(u) = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \langle x_i|u(x_i)\rangle = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m Q(x_i),
$$

trong đó $(x_1, \ldots, x_m)$ chạy qua tập hợp tất cả các dãy trực chuẩn hữu hạn các phần tử của $E$. Theo định nghĩa của $\operatorname{Tr}(Q/H)$, ta được $\operatorname{Tr}(u) = \operatorname{Tr}(Q/H)$. Cuối cùng, với mọi cơ sở trực chuẩn $(e_i)_{i \in I}$ của $E$, ta có $\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i|u(e_i)\rangle$ theo công thức (25) của V, p. 50, do đó $\operatorname{Tr}(u) = \sum_{i \in I} Q(e_i)$.

#### Nhận xét 3 {#evt-v-s4-n9-rem-3 .statement}

Cho $E$ và $F$ là hai không gian Hilbert và $v$ là một ánh xạ tuyến tính, không nhất thiết liên tục, từ $E$ vào $F$. Cho $H(x) = \|x\|^2$ và $Q(x) = \|v(x)\|^2$ với mọi $x \in E$. Suy ra từ mệnh đề 15 rằng $v$ là một ánh xạ Hilbert-Schmidt khi và chỉ khi $\operatorname{Tr}(Q/H)$ hữu hạn, và khi đó $\operatorname{Tr}(Q/H) = \|v\|_2^2$.

#### Nhận xét 4 {#evt-v-s4-n9-rem-4 .statement}

Giả sử $E$ là hữu hạn chiều. Khi dạng toàn phương $H$ khả nghịch, mệnh đề 15 áp dụng. Cho $(e_1, \ldots, e_n)$ là một cơ sở của $E$. Đặt $q_{ij} = \langle e_i|e_j\rangle_Q$ và $h_{ij} = \langle e_i|e_j\rangle_H$ và đưa vào các ma trận $q = (q_{ij})$ và $h = (h_{ij})$. Cho $u$ là một tự đồng cấu của $E$ sao cho $Q(x) = \langle x|u(x)\rangle_H$ với mọi $x \in E$. Ta có

$$
\langle x|y\rangle_Q = \langle x|u(y)\rangle_H \quad (x, y \in E),
$$

và do đó ma trận của $u$ đối với cơ sở $(e_1, ..., e_n)$ của E bằng $h^{-1} q$. Theo mệnh đề 15, ta có

$$
\text{Tr}(Q/H) = \text{Tr}(h^{-1} q) = \text{Tr}(qh^{-1}) .
$$

Nếu cơ sở $(e_1, ..., e_n)$ là trực chuẩn đối với H, thì $h$ là ma trận đơn vị cấp $n$, và ta được

$$
\text{Tr}(Q/H) = \text{Tr}(q) = \sum_{i=1}^n Q(e_i) ;
$$

do đó ta được công thức (44) trong trường hợp này.

Bây giờ giả sử rằng dạng toàn phương H không khả nghịch. Cho N là hạt nhân của H, và cho $\pi$ là ánh xạ chính tắc từ E lên E/N. Tồn tại một dạng toàn phương khả nghịch $H_1$ trên E/N sao cho $H = H_1 \circ \pi$. Cho $(e_1, ..., e_n)$ là một dãy các phần tử của E sao cho dãy $(\pi(e_1), ..., \pi(e_m))$ là một cơ sở của E/N, trực chuẩn đối với $H_1$. Cho $(e_1, ..., e_n)$ là một cơ sở của N. Khi đó $(e_1, ..., e_n)$ là một cơ sở của E và ta có

$$
H(\xi_1 e_1 + \cdots + \xi_n e_n) = \xi_1^2 + \cdots + \xi_m^2
$$

với mọi số thực $\xi_1, ..., \xi_n$.

Giả sử rằng với mọi $x \in E$, quan hệ $H(x) = 0$ kéo theo $Q(x) = 0$; nói cách khác, giả sử rằng tồn tại một dạng toàn phương $Q_1$ trên E/N sao cho $Q = Q_1 \circ \pi$. Theo nhận xét 2 và mệnh đề 15, ta có,

$$
\text{Tr}(Q/H) = Q(e_1) + \cdots + Q(e_m) .
$$

Bài tập
