---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 5
section_title: The topology defined by a valuation
lang: vi
source: ac-i-vii
book_pages: 399-403, 454-459
pdf_pages: 0417-0421, 0472-0477
extraction: ocr
subsections:
    - "no": 1
      title: THE TOPOLOGY DEFINED BY A VALUATION
      page: 399
      pdf_page: 417
    - "no": 2
      title: TOPOLOGICAL VECTOR SPACES OVER A FIELD WITH A VALUATION
      page: 401
      pdf_page: 419
    - "no": 3
      title: THE COMPLETION OF A FIELD WITH A VALUATION
      page: 402
      pdf_page: 420
statements: 10
exercises: 9
content_sha256: 9ebbea3d983442716c904ee098f27e24297ce604b5054c89d34a7ea7375f7e8d
translated_from: content/en/ac/VI/05_s5_the_topology_defined_by_a_valuation.md
source_content_sha256: b771ebddcf3acdd2226c56d72c2ea5f26745e679f803c00eac83b9bd0bcaa51c
translation_model: gpt-5.4-mini
translation_run: translate-vi-0671723b
glossary_version: 34
glossary_terms_sha256: 1e0b13179443998ccada4d996ba5dd89eeb01ca1923ffc7e8ecf569b4a6bf9cb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. TÔPÔ ĐƯỢC XÁC ĐỊNH BỞI MỘT ĐỊNH GIÁ

### 1. TÔPÔ ĐƯỢC XÁC ĐỊNH BỞI MỘT ĐỊNH GIÁ

Cho K là một trường không nhất thiết giao hoán, v là một định giá trên K và G là nhóm được sắp thứ tự toàn phần $v(K^*)$. Với mọi $a \in G$, đặt V, là tập hợp các $x \in K$ sao cho $v(x) > a$; tập này là một nhóm con cộng tính của K (§ 3, no. 1). Tồn tại duy nhất một tôpô $\mathcal{T}_v$ trên K sao cho các V, tạo thành một hệ cơ bản các lân cận của 0 (*General Topology*, Chapter III, § 1, no. 2, Example). Để v là định giá tầm thường, điều kiện cần và đủ là $\mathcal{T}_v$ là tôpô rời rạc.

#### Bổ đề 1 {#ac-vi-s5-lem-1 .statement}

*Cho $x \in K^*, y \in K^*$ và $\alpha \in G$. Nếu*
$$
v(x - y) > \sup(\alpha + 2v(y), v(y)),
$$
*thì* $v(x^{-1} - y^{-1}) > a$.

$x^{-1} - y^{-1} = x^{-1}(y - x)y^{-1}$ và do đó
$$
v(x^{-1} - y^{-1}) = v(x - y) - v(x) - v(y).
$$
Nếu $v(x - y) > v(y)$, Mệnh đề 1 của § 3, no. 1 suy ra rằng $v(x) = v(y)$, vì $x = y + (x - y)$. Hơn nữa, nếu $v(x - y) > a + 2v(y)$, thì
$$
v(x^{-1} - y^{-1}) > a + 2v(y) - 2v(y) = a.
$$

#### Mệnh đề 1 {#ac-vi-s5-prop-1 .statement}

*Tôpô $\mathcal{T}_v$ là Hausdorff và tương thích với cấu trúc vành trên K. Ánh xạ $v : K^* \to G$ là liên tục nếu G được cho tôpô rời rạc.*

Cho $x \in K^*$ và $a = v(x)$; khi đó $x \notin V_a$, điều này cho thấy rằng $\mathcal{T}_v$ là Hausdorff. Với mọi $x_0 \in K$ và $a \in G$, tồn tại $\beta \in G$ sao cho $x_0 V_\beta \subset V_\alpha$ và $V_\beta x_0 \subset V$, (chỉ cần lấy $\beta \geqslant a - v(x_0)$). Mặt khác, nếu $a \geqslant 0$, thì $V_\alpha V_\alpha \subset V_v$. Vì vậy các tiên đề (AV_I) và (AV_{II}) của *General Topology*, Chapter III, § 6, no. 3 được thỏa mãn, nên $\mathcal{T}_v$ tương thích với cấu trúc vành trên K. Cho $x_0 \in K^*$; nếu $x \in K^*$ thỏa mãn $v(x - x_0) > \sup(\alpha + 2v(x_0), v(x_0))$, thì $v(x^{-1} - x_0^{-1}) > a$ (Bổ đề 1), điều này cho thấy ánh xạ $x \mapsto x^{-1}$ là liên tục và do đó $\mathcal{T}_v$ tương thích với cấu trúc trường trên K. Cuối cùng, điều kiện duy nhất $v(x - x_0) > v(x_0)$ suy ra $v(x) = v(x_0)$ (§ 3, no. 1, Mệnh đề 1) và do đó ánh xạ $v : K^* \to G$ là liên tục nếu G được cho tôpô rời rạc.

Cho $\alpha \in G$ và $V'_\alpha$ là tập hợp các $x \in K$ sao cho $v(x) \geq \alpha$. Nếu $\beta < a$, thì $V_\beta \supset V'_\alpha \supset V_v$. Nếu v không phải là định giá tầm thường, do đó thấy rằng các $V'_\alpha$ tạo thành một hệ cơ bản các lân cận của 0 đối với $\mathcal{T}_v$.

Các $V_v$ và các $V'_\alpha$ là các nhóm con cộng mở và do đó đóng trong $K$, và do đó trường tôpô $K$ là *không liên thông hoàn toàn*. Vì mọi iđêan khác không của vành của $v$ chứa một $V_v$, nên nó *mở và đóng* trong $K$. Tôpô thương trên trường thặng dư của $v$ do đó là *rời rạc*.

Cho $A$ là vành của $u$. Nếu $v$ là rời rạc, Mệnh đề 8 của $§ 3$, no. 6 cho thấy tôpô cảm sinh bởi $\mathcal{T}_v$ trên $A$ là tôpô $m(A)$-adic. Điều này nói chung không đúng (Bài tập 4).

#### Mệnh đề 2 {#ac-vi-s5-prop-2 .statement}

*Cho $K$ là một trường không nhất thiết giao hoán, $v$ là một định giá không tầm thường trên $K$, $A$ là vành của $v$ và $m$ là iđêan của $v$. Để $K$ với tôpô $\mathcal{T}_v$ là compact địa phương, cần và đủ rằng các điều kiện sau được thỏa mãn:*

(i) $K$ đầy đủ;
(ii) $v$ rời rạc;
(iii) *trường thặng dư $\kappa(A)$ hữu hạn.*

*Nếu vậy*, $A$ là compact.

Giả sử $K$ là compact địa phương. Khi đó nó đầy đủ (*General Topology*, Chương 111, $§ 3$, no. 3, Hệ quả 1 của Mệnh đề 4); hơn nữa tồn tại một lân cận compact của 0, chứa một lân cận $V'_a$, với $a$ thuộc nhóm giá trị của $v$; nói cách khác, tồn tại $a \neq 0$ trong $K^*$ sao cho $A . a$ là compact và suy ra rằng $A = (A . a)a^{-1}$ là compact. Vì mọi iđêan $b \neq (0)$ của $A$ là mở, $A/b$ là compact và rời rạc (*General Topology*, Chương III, $§ 2$, no. 5, Mệnh đề 14) nên hữu hạn và đặc biệt $\kappa(A) = A/m$ là hữu hạn. Hơn nữa, với $y \neq 0$ trong $m$, vì vành $A/Ay$ là hữu hạn, chỉ có hữu hạn nhiều iđêan của $A$ chứa $Ay$ và tập $P$ gồm các phần tử có dạng $v(x)$ sao cho

$$
0 < v(x) \leq v(y)
$$

is finite; như $v(K^*)$ được sắp thứ tự toàn phần, $P$ có một phần tử nhỏ nhất $y$. Khi đó, với mọi $x \in A$ sao cho $v(x) > 0$, hoặc $v(x) > v(y) \geq y$, hoặc $v(x) \leq v(y)$ và khi đó $v(x) \geq y$ theo định nghĩa, do đó $y$ là phần tử nhỏ nhất trong các phần tử $> 0$ của $v(K^*)$. *Vì* $P$ *là* hữu hạn, tồn tại một số nguyên lớn nhất $m \geq 0$ sao cho $my \in P$, do đó my \leq v(y) < (m+1)\gamma. Suy ra 0 \leq v(y) - my < y và theo định nghĩa của $y$ điều này suy ra $v(y) = my$. Vậy $v(K^*) = \mathbf{Z}.\gamma$ và định giá $v$ là rời rạc.

Ngược lại, giả sử các điều kiện (i), (ii), (iii) đúng. Ta có thể chỉ xét trường hợp $v$ là chuẩn hóa; cho $u$ là một phần tử đều hóa của $v$. Khi đó $\kappa(A) = A/Au$ và do đó $A/Au$ là hữu hạn. Vì ánh xạ $x \mapsto xu^n$, khi lấy thương, xác định một đẳng cấu của nhóm cộng $A/Au$ lên $Au^n/Au^{n+1}$, nên $A/Au^j$ là hữu hạn với mọi $j \geq 0$. Vì $A$ đóng trong $K$, nó đầy đủ và do đó đẳng cấu với giới hạn ngược của các $A/Au^j$ (General Topology, Chapter 111, § 7, no. 3, Mệnh đề 2) và vì thế compact. Vì $A$ mở trong $K$, suy ra $K$ là compact địa phương.

#### Nhận xét {#ac-vi-s5-n1-rem-1 .statement}

Lưu ý rằng trong chứng minh này chỉ cần giả sử rằng $A$ đầy đủ.

Ta sẽ thấy ở § 9 rằng một trường $K$ thỏa các điều kiện của Mệnh đề 2 có một tâm hoặc là một mở rộng đại số hữu hạn của một trường $p$-adic, hoặc là một trường $\mathbf{F}_q((T))$ của chuỗi lũy thừa hình thức trên một trường hữu hạn; hơn nữa $K$ có hạng hữu hạn trên tâm của nó.

### 2. KHÔNG GIAN VECTƠ TÔPÔ TRÊN MỘT TRƯỜNG CÓ ĐỊNH GIÁ

Trong toàn bộ mục này, cho $K$ là một trường (không nhất thiết giao hoán), $v$ là một định giá trên $K$ và $G$ là nhóm thứ tự của nó. $K$ được cho tôpô $\mathcal{T}_v$.

#### Mệnh đề 3 {#ac-vi-s5-prop-3 .statement}

Cho $E$ là một không gian vectơ tôpô trái trên $K$ tách Hausdorff và có chiều 1. Giả sử rằng $v$ không tầm thường. Với mọi $x_0 \neq 0$ trong $E$, ánh xạ $a \mapsto ax_0$ từ $K_s$ lên $E$ là một đẳng cấu tôpô.

Ánh xạ này là một đẳng cấu đại số liên tục. Chỉ cần chứng minh nó liên tục hai chiều. Cho $\alpha \in G$. Ta cần chứng minh rằng tồn tại một lân cận $V$ của 0 trong $E$ sao cho quan hệ $ax_0 \in V$ suy ra $v(a) > a$. Cho $a, \in K^*$ sao cho $v(a_0) = a$. Vì $E$ là Hausdorff, tồn tại một lân cận $W$ của 0 trong $E$ sao cho $a_0x_0 \notin W$. Vì $v$ không tầm thường, tồn tại một lân cận $W'$ của 0 trong $E$ và một phần tử $\beta$ của $G$ sao cho các quan hệ $y \in W'$, $v(a) \geq \beta$ suy ra $ay \in W$. Cho $a, \in K^*$ sao cho $v(a_1) = -\beta$. Các quan hệ $ax_0 \in a_1^{-1}W'$ và $v(a) \leq a$ suy ra $a_1ax_0 \in W$ và $v(a_0a^{-1}a_1^{-1}) = \alpha + \beta - v(a) \geq \beta$ và do đó $a_0x_0 = a_0a^{-1}a_1^{-1}(a_1ax_0) \in W$, điều này là vô lý; nói cách khác, quan hệ $ax, \in a_1^{-1}W$ suy ra $v(a) > a$.

#### Hệ quả {#ac-vi-s5-n2-cor-1 .statement}

Cho $E$ là một không gian vectơ tôpô trái trên K, $H$ là một siêu phẳng đóng của $E$ và $D$ là một không gian con vectơ một chiều của $E$ là một phần bù đại số của $H$. Giả sử rằng $v$ không tầm thường. Khi đó $D$ là một phần bù tôpô của $H$.

Xét đến các Mệnh đề 1 và 3, chứng minh giống như trong Topological Vector Spaces, Chương I, § 2, Hệ quả 2 của Định lý 1.

#### Mệnh đề 4 {#ac-vi-s5-prop-4 .statement}

Giả sử rằng $v$ không tầm thường và $K$ đầy đủ. Cho $E$ là một không gian vectơ tôpô trái trên K, Hausdorff và có số chiều hữu hạn n. Với mọi cơ sở $(e_i)_{1 \leq i \leq n}$ của $E$ trên $K$, ánh xạ $(a_i) \mapsto \sum_{i=1}^n a_i e_i$ từ $K^n_s$ lên $E$ là một đẳng cấu không gian vectơ tôpô.

Xét đến Mệnh đề 3 và hệ quả của nó, chứng minh giống như trong Topological Vector Spaces, Chương I, § 2, Định lý 2.

#### Hệ quả {#ac-vi-s5-n2-cor-2 .statement}

Giả sử rằng $v$ không tầm thường và $K$ đầy đủ. Cho $E$ là một không gian vectơ tôpô Hausdorff trên K và $F$ là một không gian con vectơ hữu hạn chiều của $E$. Khi đó $F$ đóng.

$F$ đầy đủ.

### 3. SỰ ĐẦY ĐỦ HÓA CỦA MỘT TRƯỜNG VỚI MỘT ĐỊNH GIÁ

#### Mệnh đề 5 {#ac-vi-s5-prop-5 .statement}

Cho $K$ là một trường không nhất thiết giao hoán, $v$ là một định giá trên $K$ và $G$ là nhóm $v(K^*)$ với tôpô rời rạc.

(a) Vành hoàn thành $\hat{K}$ của $K$ (với $\mathcal{T}_v$) là một trường tôpô.

(b) Ánh xạ $v : K^* \to G$ có thể được mở rộng duy nhất thành một ánh xạ liên tục $8 : \hat{K}^* \to G$. Ánh xạ $0$ (được mở rộng bởi $\hat{v}(0) = +\infty$) là một định giá trên $\hat{K}$ và $\hat{v}(\hat{K}^*) = v(K^*)$.

(c) Tôpô trên $\hat{K}$ là tôpô được xác định bởi định giá $0$.

(d) Với mọi $a \in G$ hãy cho $V_\alpha, V'_\alpha$ là các nhóm con của $K$ được xác định bởi các điều kiện $v(x) > a, v(x) \geq a$. Khi đó các bao đóng $\overline{V}_\alpha, \overline{V}'_\alpha$ của $V_\alpha, V'_\alpha$ trong $\hat{K}$ được xác định tương ứng bởi các điều kiện $\hat{v}(x) > a, \hat{v}(x) \geq a$.

(e) Vành của $0$ là phần hoàn thành $\hat{A}$ của vành $A$ của $v$; iđêan của $0$ là phần hoàn thành $\hat{m}$ của iđêan $m$ của $v$.

(f) $\hat{A} = A + m$; trường thặng dư của $8$ được đồng nhất một cách chính tắc với trường thặng dư của $v$.

Để chứng minh (a) chỉ cần (General Topology, Chương III, § 6, no. 8, Mệnh đề 7) chứng minh điều sau: hãy cho $\mathfrak{F}$ là một bộ lọc Cauchy (đối với cấu trúc đều cộng tính) trên $K^*$ mà $0$ không là một điểm tụ; khi đó ảnh của $\mathfrak{F}$ qua song ánh $x \mapsto x^{-1}$ là một bộ lọc Cauchy (đối với cấu trúc đều cộng tính). Vì $0$ không là một điểm tụ của $\mathfrak{F}$, tồn tại $M \in \mathfrak{F}$ và $\beta \in G$ sao cho $\beta$ là một cận trên của $v(M)$ . Cho $a \in G$. Nếu $M'$ là một phần tử của $\mathfrak{F}$ được chứa trong $M$ và sao cho $v(x - y) > \sup(\alpha + 2\beta, \beta)$ với $x \in M'$ và $y \in M'$, thì $v(x^{-1} - y^{-1}) > a$ với $x \in M'$ và $y \in M'$ (no. 1, Bổ đề 1). Do đó (a).

Theo Mệnh đề 1 của no. 1, $v|K^*$ là một đồng cấu liên tục từ $K^*$ đến $G$ và do đó có thể được mở rộng duy nhất thành một đồng cấu liên tục $0$ từ $K^*$ đến $G$. Quan hệ

$$
\hat{v}(x + y) \geq \inf(\hat{v}(x), \hat{v}(y))
$$

đúng trong $K^*$ và do đó cũng đúng trong $\hat{K}^*$ nhờ tính liên tục. Do đó $0$ (được mở rộng bằng $\hat{v}(0) = +\infty$) là một định giá trên $\mathbf{K}$ và (b) được chứng minh.

Ta chứng minh (d). Lấy $a \in G$ và $x \in \mathcal{S}, -\{0\}$. Với $y$ trong $V$, đủ gần $x$, $\hat{v}(x) = \hat{v}(y) = v(y)$ và do đó $\hat{v}(x) > a$. Ngược lại, lấy $x \in \hat{K}^*$ sao cho $\hat{v}(x) > a$; với $y$ trong $K^*$ đủ gần $x$, $v(y) = \hat{v}(y) = \hat{v}(x)$ và vì vậy $y \in V$, do đó $x \in \mathcal{S}$. Vậy $\mathcal{S}$ là tập hợp các $x \in \hat{K}$ sao cho $\hat{v}(x) > a$. Lập luận tương tự đối với $V'_a$. Điều này chứng minh (d).

Dựa vào Mệnh đề 7 của Tôpô tổng quát, Chương III, § 3, no. 4, mệnh đề (c) là hệ quả của (d). Mệnh đề (e) là một trường hợp riêng của (d). Cuối cùng, lấy $x \in \hat{A}$; tồn tại $y \in A$ sao cho $\hat{v}(x - y) > 0$; khi đó $z = x - y \in \hat{m}$ và do đó $x = y + z \in A + \hat{m}$; suy ra $\hat{A} = A + \hat{m}$, điều này chứng minh (f).

#### Nhận xét {#ac-vi-s5-n3-rem-1 .statement}

Với mọi $x \in \hat{K}$ không thuộc $\hat{A}$, tồn tại $x_0 \in K$ sao cho $\hat{v}(x - x_0) > 0$, $\hat{v}(x) = \hat{v}(x_0) = v(x_0) < 0$; khi đó $x_0^{-1} x \in \hat{A}$ và, vì $x_0^{-1} \in A$, ta thấy rằng, nếu đặt $S = A - \{0\}$, có thể viết $\hat{K} = S^{-1} \hat{A}$.

### Bài tập {#ac-vi-s5-exercises}

bậc $n > 1$ và sao cho $a_i \neq 0$; hãy chứng minh rằng tồn tại một dãy tăng ngặt $(i_k)_{0 \leq k \leq r}$ của các số nguyên trong khoảng $[0, n]$ sao cho: (1) $i_0 = 0$, $i_r = n$; (2) $v(a_{i_k})$ là hữu hạn với $0 \leq k \leq r$; (3) với mọi chỉ số $j$ sao cho $0 \leq j \leq n$ phân biệt với các $i_k$, sao cho $v(a_j)$ là hữu hạn, điểm
$$
(j, v(a_j)) \in \mathbf{R}^2
$$
nằm phía trên đường thẳng đi qua các điểm $(i_k, v(a_{i_k}))$ và $(i_{k+1}, v(a_{i_{k+1}}))$ và nằm nghiêm ngặt phía trên đường thẳng đó nếu $j < i_k$ hoặc $j > i_{k+1}$. Hợp của các đoạn nối các điểm $(i_k, v(a_{i_k}))$ và $(i_{k+1}, v(a_{i_{k+1}}))$ được gọi là đa giác Newton của P, các đoạn trên được gọi là các cạnh và các điểm $(i_k, v(a_{i_k}))$ là các đỉnh của đa giác.

(b) Giả sử rằng mọi nghiệm của P đều thuộc K. Hãy chứng minh rằng để các giá trị định giá của mọi nghiệm của P đều bằng nhau, thì điều kiện cần và đủ là $r = 1$ (nói cách khác, đa giác Newton rút gọn thành một cạnh duy nhất). (Để chứng minh rằng điều kiện là đủ, hãy xét đa giác Newton của một tích $P_1P_2$ trong đó mọi nghiệm của $P_1$ đều khả nghịch trong vành của v, còn mọi nghiệm của $P_2$ đều thuộc iđêan của v.)

(c) Giả sử rằng mọi nghiệm của P đều thuộc K; hãy lập đa giác Newton của P và viết.
$$
\rho_k = i_{k+1} - i_k, \quad \sigma_k = (v(a_{i_{k+1}}) - v(a_{i_k}))/\rho_k.
$$
Hãy chứng minh rằng, với $0 \leq k \leq r - 1$, P có đúng $\rho_k$ nghiệm (được đếm theo các bội số của chúng) mà các giá trị định giá của chúng đều bằng $\sigma_k$ (dùng (b) và chứng minh bằng quy nạp theo $r$).

(d) Khái quát hóa sang trường hợp của bất kỳ định giá nào $v$ (nhúng nhóm cấp $\Gamma$ của $v$ vào không gian Q-vectơ $\Gamma_{(0)}$, vốn có một cấu trúc nhóm được sắp thứ tự toàn phần tự nhiên).

95

Xem [các bài tập cho § 5](exercises/s5/).
