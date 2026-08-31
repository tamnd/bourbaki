---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 10
section_title: Angles
lang: vi
source: alg-ix-fr
pdf_pages: 0158-0182
extraction: ocr
subsections:
    - "no": 1
      title: Similitudes directes dans un plan.
      page: 0
      pdf_page: 158
    - "no": 2
      title: Trigonométrie plane.
      page: 0
      pdf_page: 162
    - "no": 3
      title: Angles.
      page: 0
      pdf_page: 165
    - "no": 4
      title: Secteurs angulaires.
      page: 0
      pdf_page: 171
statements: 31
exercises: 0
content_sha256: 7b972f2e56f0aa83907e79c6be0316c16ea05c53093f0c61e1124b0e9574c2d3
translated_from: content/en-mt/alg/IX/10_s10_angles.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 9f10e6564e0b8cbdecdb53808d1d40c774e976cf722d13b8bb1395ecdf4e8f0d
translation_model: gpt-5.4, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-851c2afc
glossary_version: 34
glossary_terms_sha256: cb30a26eab8870a54c44dc33fdc67d324709cd10056842fa6edccbecb9877381
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. Góc

Trong suốt đoạn này, A ký hiệu một trường giao hoán có đặc số $\neq 2$, E một không gian vectơ chiều 2 trên A, và $\Phi$ một dạng song tuyến tính đối xứng không suy biến trên E.

### 1. Các phép vị tự trực tiếp trong một mặt phẳng.

Nhắc lại (§ 6, No. 5) rằng một phép vị tự trực tiếp của E là một tự đẳng cấu $u$ của không gian vectơ E sao cho $\Phi(u(x), u(y)) = (\det u)\Phi(x, y)$ với mọi $x, y$ trong E.

#### Mệnh đề 1 {#alg-ix-s10-prop-1 .statement}

Gọi $A(\Phi)$ là đại số con của $\mathcal{L}_A(E)$ được sinh bởi các phép vị tự trực tiếp của E.

a) Các phép vị tự trực tiếp là các phần tử khả nghịch của $A(\Phi)$. Đại số $A(\Phi)$ là một đại số giao hoán bậc 2 trên A. Khi E không chứa vectơ đẳng hướng nào $\neq 0$, $A(\Phi)$ là một trường, một mở rộng bậc hai của A; trong trường hợp ngược lại nó là tổng trực tiếp của hai trường đẳng cấu với A.

b) Gọi $(e_1, e_2)$ là một cơ sở trực giao của E; đặt $\alpha_i = \Phi(e_i, e_i)$ $(i = 1, 2)$ và $\delta = -\alpha_2/\alpha_1$. Khi đó các ma trận của các phần tử của $A(\Phi)$ đối với cơ sở này là các ma trận dạng $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$ trong đó $a \in A, b \in A$.

c) Không gian E là một $A(\Phi)$-môđun tự do đơn sinh, được sinh bởi bất kỳ vectơ không đẳng hướng nào.

Thật vậy, ta đưa vào một dạng song tuyến tính phản xứng phụ $B \neq 0$ trên E; khi đó B là không suy biến. Do đó tồn tại một tự đồngNo. 1

cấu xạ $\omega$ của E sao cho $\Phi(x, y) = B(\omega(x), y)$ với mọi $x, y$ trong E. Với mọi tự đồng cấu khả nghịch $u$ của E, ta có
$$
\begin{align*}
\Phi(u(x), u(y)) &= B(\omega u(x), u(y)) = B(uu^{-1}\omega u(x), u(y)) \\
&= (\det u)B(u^{-1}\omega u(x), y);
\end{align*}
$$
do đó, để $u$ là một phép vị tự trực tiếp, điều kiện cần và đủ là có
$$
(\det u)B(u^{-1}\omega u(x), y) = (\det u)\Phi(x, y) = (\det u)B(\omega(x), y)
$$
với mọi $x, y$ trong E; vì $\det u \neq 0$ và B là không suy biến, điều này tương đương với $u^{-1}\omega u = \omega$, hay cũng lại là $u\omega = \omega u$. Lấy B là dạng song tuyến tính phản xứng có ma trận $S$ đối với $(e_1, e_2)$ là $\begin{pmatrix} 0 & 1 \\ -1 & 0 \end{pmatrix}$; ký hiệu bởi $R$ và $W$ các ma trận của $\Phi$ và của $\omega$ đối với cơ sở này, hệ thức $\Phi(x, y) = B(\omega(x), y)$ được viết, theo công thức (47) của § 1, No. 10, là $R = {}^tW.S$; khai triển ra cho thấy ta có $W = \begin{pmatrix} 0 & \alpha_2 \\ -\alpha_1 & 0 \end{pmatrix}$. Nếu $\begin{pmatrix} a & c \\ b & d \end{pmatrix}$ ký hiệu ma trận của $u$ đối với $(e_1, e_2)$, thì hệ thức $u\omega = \omega u$ do đó tương đương với các hệ thức $b\alpha_2 = -c\alpha_1, a\alpha_2 = d\alpha_2, a\alpha_1 = d\alpha_1$, tức là với $a = d$ và $c = \delta b$; điều này chứng minh rằng các ma trận của các phép vị tự trực tiếp là các ma trận khả nghịch dạng $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$ ($a, b$ trong A).

Bây giờ các tự đồng cấu của E mà các ma trận có dạng $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$ ($a, b$ trong A) tạo thành một không gian con vectơ chiều 2 của $\mathfrak{L}_A(E)$, sinh bởi 1 và bởi tự đồng cấu $\omega$; vì $\omega^2$ là phép vị tự tỉ số $-\alpha_1\alpha_2$, không gian con này là đại số con $A(\Phi)$ của $\mathfrak{L}_A(E)$ sinh bởi các phép đồng dạng trực tiếp. Các phép đồng dạng trực tiếp là các phần tử khả nghịch của $A(\Phi)$, nghĩa là những phần tử mà các ma trận của chúng thỏa mãn $a^2 - \delta b^2 \neq 0$. Việc đại số $A(\Phi)$ là giao hoán là hiển nhiên. Hãy áp dụng cho nó các kết quả của Chương II, § 7, No. 7: nếu $\delta$ không là một bình phương trong A, nghĩa là nếu không có vectơ khác không nào của E là đẳng hướng, thì $A(\Phi)$ là một trường; ngược lại, nếu $\delta$ là một bình phương trong A, nghĩa là nếu E chứa các vectơ đẳng hướng $\neq 0$, thì $A(\Phi)$ là tổng trực tiếp của hai trường đẳng cấu với A. Điều này chứng minh a) và b).

Sau cùng, mọi vectơ không đẳng hướng của E đều có thể được lấy làm vectơ thứ nhất $e_1$ của một cơ sở trực giao $(e_1, e_2)$ (§ 6, No. 1); do đó các ảnh của nó $u(e_1)$ bởi các phần tử $u$ của $\Lambda(\Phi)$ là các vectơ có dạng $ae_1 + be_2$ ($a, b$ trong $\Lambda$), nghĩa là tất cả các vectơ của $E$, vì mọi ma trận $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$ đều là ma trận của các phần tử của $\Lambda(\Phi)$. Nói cách khác, $E$ là một $\Lambda(\Phi)$-môđun đơn sinh, sinh bởi bất kỳ vectơ không đẳng hướng nào. Hơn nữa, ta còn thấy rằng nó là một $\Lambda(\Phi)$-môđun đơn sinh tự do, vì $u(e_1) = ae_1 + be_2 = 0$ kéo theo $a = b = 0$, do đó $u = 0$. Điều này chứng minh c).

#### Nhận xét 1 {#alg-ix-s10-n1-rem-1 .statement}

Gọi $\nu$ là phép đồng dạng có ma trận $\begin{pmatrix} 0 & \delta \\ 1 & 0 \end{pmatrix}$ đối với $(e_1, e_2)$; phép đồng dạng $\omega$ được đưa vào trong chứng minh của Mệnh đề 1 bằng $-\alpha_1 \nu$; ta có $\nu^2 = \delta$. Nhân tử của phép đồng dạng trực tiếp $u = a + b \nu$ ($a, b$ trong $\Lambda$) bằng định thức của ma trận $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$ của nó, nghĩa là bằng $a^2 - \delta b^2 = (a + b \nu)(a - b \nu) = u . \overline{u}$, trong đó $\overline{u}$ là liên hợp của $u$ trong đại số $\Lambda(\Phi)$ (Chương II, § 7, No. 7); nói cách khác nhân tử của $u$ là chuẩn $N(u)$ của $u$ trong đại số $\Lambda(\Phi)$ (cùng chỗ đó). Đặc biệt, để một phép đồng dạng trực tiếp $u$ là một phép quay, điều kiện cần và đủ là $N(u) = 1$; để $u$ là một phép vị tự, điều kiện cần và đủ là $u \in \Lambda^*$.

#### Nhận xét 2 {#alg-ix-s10-n1-rem-2 .statement}

Các phép đồng dạng trực tiếp $u = a + b \nu$ ($a, b$ in $\Lambda$, $b \neq 0$) có bình phương là một phép vị tự là các phép vị tự và các bội vô hướng $b \nu$ của $\nu$, vì $(a + b \nu)^2 = (a^2 + \delta b^2) + 2ab \nu$. Các phép sau đây không gì khác ngoài các tự đẳng cấu của không gian vectơ $E$ mà *biến mọi vectơ thành một vectơ vuông góc với nó*; thực vậy, ma trận của một tự đẳng cấu như vậy nhất thiết có dạng $\begin{pmatrix} 0 & c \\ d & 0 \end{pmatrix}$ ($c, d$ in $\Lambda$), và điều kiện để vectơ $\lambda e_1 + \mu e_2$ được biến thành một vectơ vuông góc khi đó được viết là $\lambda \mu (d \alpha_2 + c \alpha_1) = 0$.

#### Nhận xét 3 {#alg-ix-s10-n1-rem-3 .statement}

Dễ dàng kiểm tra rằng, với $x, y$ in $E$ và $u \in \Lambda(\Phi)$, ta có $\Phi(u(x), y) = \Phi(x, \overline{u}(y))$. Do đó, tự đồng cấu *liên hợp* của một phép đồng dạng trực tiếp $u$ là phép đồng dạng trực tiếp $\overline{u}$ *liên hợp* của $u$ trong $\Lambda(\Phi)$.

#### Nhận xét 4 {#alg-ix-s10-n1-rem-4 .statement}

Vì mọi *phép đồng dạng nghịch* của $E$ là tích của một phép đồng dạng trực tiếp và phép đối xứng đối với $Ae_1$, nên các ma trận No. 1

của các phép đồng dạng nghịch đối với $(e_1, e_2)$ là các ma trận có dạng $\begin{pmatrix} a & -\delta b \\ b & -a \end{pmatrix}$.

Kể từ đây ta sẽ ký hiệu bởi $S$ nhóm các phép đồng dạng của $E$, bởi $S^+$ nhóm các phép đồng dạng trực tiếp, bởi $H$ nhóm các phép vị tự $\neq 0$, và bởi $O^+$ nhóm các phép quay. Nhắc lại rằng có $H \subset S^+ (§ 6, n° 5)$.

#### Hệ quả 1 {#alg-ix-s10-prop-1-cor-1 .statement}

*Nhóm $S^+$ của các phép đồng dạng trực tiếp là giao hoán. Với mọi các vectơ không đẳng hướng $x, y$ của $E$, tồn tại một và chỉ một phép đồng dạng trực tiếp $u$ sao cho $y = u(x)$.*

Khẳng định thứ nhất suy ra từ sự kiện rằng đại số $A(\Phi)$ là giao hoán. Vì $E$ là một $A(\Phi)$-môđun tự do đơn sinh được sinh bởi $x$ (tương ứng $y$), tồn tại một và chỉ một phần tử $u$ (tương ứng $u'$) của $A(\Phi)$ sao cho $y = u(x)$ (tương ứng $x = u'(y)$); do đó $x = u(u'(x))$, và $uu'$ là phần tử đơn vị; điều này chứng minh rằng $u$ là khả nghịch, và vì thế là một phép đồng dạng trực tiếp.

#### Hệ quả 2 {#alg-ix-s10-prop-1-cor-2 .statement}

*Nhóm $O^+$ của các phép quay là giao hoán. Với mọi các vectơ $x, y$ của $E$ sao cho $\Phi(x, x) = \Phi(y, y) \neq 0$, tồn tại một và chỉ một phép quay $u$ sao cho $y = u(x)$.*

Khẳng định đầu tiên suy ra từ Hệ quả 1. Điều sau cũng chỉ ra rằng tồn tại duy nhất một phép đồng dạng trực tiếp $u$ sao cho $y = u(x)$; vì $\Phi(u(x), u(x)) = \Phi(x, x)$, nhân tử của $u$ bằng 1, và do đó $u$ là một phép quay.

#### Hệ quả 3 {#alg-ix-s10-prop-1-cor-3 .statement}

*Nhóm $S^+/H$ là giao hoán. Nó tác động lên tập hợp các đường thẳng không đẳng hướng của $E$. Với mọi các đường thẳng không đẳng hướng $D, D'$ của $E$, tồn tại duy nhất một phần tử $\varphi$ của $S^+/H$ sao cho $D' = \varphi(D)$.*

Điều này suy ra từ Hệ quả 1 và từ sự kiện rằng $H$ bất biến toàn cục mọi đường thẳng của $E$.

#### Mệnh đề 2 {#alg-ix-s10-prop-2 .statement}

*Hạt nhân của đồng cấu chính tắc của $O^+$ vào $S^+/H$ là $\{1, -1\}$.*

Thật vậy 1 và $-1$ là các phần tử duy nhất của $H \cap O^+$.

#### Mệnh đề 3 {#alg-ix-s10-prop-3 .statement}

Đồng cấu $u \to u/\overline{u} = u^2 / N(u)$ của $S^+$ vào chính nó có $H$ làm hạt nhân, và xác định, bằng cách chuyển qua thương, một đẳng cấu của $S^+/H$ lên $O^+$.

Thật vậy quan hệ $u/\overline{u} = 1$ tương đương với $u = \overline{u}$, nghĩa là với $u \in A^* = H$; do đó $H$ là hạt nhân của $u \to u/\overline{u}$. Vì $N(u/\overline{u}) = 1$, $u/\overline{u}$ là một phép quay (Nhận xét 1). Còn lại phải chứng minh rằng mọi phần tử $\varphi$ của $O^+$ đều có dạng $u/\overline{u}$ ($u \in S^+$). Nếu $1 + \varphi$ khả nghịch, ta có thể lấy $u = 1 + \varphi$, vì quan hệ $N(\varphi) = \varphi \overline{\varphi} = 1$ kéo theo $1 + \varphi = \varphi(1 + \overline{\varphi})$. Ngược lại, ta có $N(1 + \varphi) = (1 + \varphi)(1 + \overline{\varphi}) = 0$, nghĩa là, khi đặt $\varphi = a + b\omega$ ($a \in A,\ b \in A,\ \omega^2 = \delta \in A$), $2(1 + a) = 0$, do đó $a = -1$; bây giờ các quan hệ $a = -1$ và $N(\varphi) = a^2 - \delta b^2 = 1$ kéo theo $b = 0$, do đó $\varphi = -1$; vì $\overline{\omega} = -\omega$, trong trường hợp này chỉ cần lấy $u = \omega$.

Khi $A(\Phi)$ là một trường, Mệnh đề 3 là một trường hợp riêng của định lý Hilbert (Chương V, § 11, No. 5, Định lý 3).

#### Hệ quả {#alg-ix-s10-n1-cor-1 .statement}

Ký hiệu $i : O^+ \to S^+/H$ và $d : S^+/H \to O^+$ là các đồng cấu được xác định trong các Mệnh đề 2 và 3, và viết các nhóm Abel $O^+$ và $S^+/H$ theo phép cộng; khi đó $d(i(\theta)) = 2\theta$ cho $\theta \in O^+$
và $i(d(\varphi)) = 2\varphi$ cho $\varphi \in S^+/H$.

Thật vậy, nếu $\overline{\varphi}$ là một phép quay, ta có $\overline{\varphi} = \varphi^{-1}$, do đó $d(i(\varphi)) = \varphi/\overline{\varphi} = \varphi^2$. Mặt khác, nếu $\varphi \in S^+/H$, $\varphi$ là lớp mod. $H$ của một phép đồng dạng trực tiếp $u$, và $d(\varphi) = u/\overline{u} = u^2 / N(u)$ đồng dư với $u^2$ mod. $H$; do đó có công thức thứ hai.

### 2. Lượng giác phẳng.

Trong số này, ta sẽ chọn một phần tử sinh $\omega$ của đại số $A(\Phi)$ sao cho $\omega^2 \in A$. Một phần tử sinh như thế được xác định tới một phép vị tự (No. 1, Nhận xét 2), vì vậy phần tử $\omega^2$ của $A$, mà ta sẽ ký hiệu là $\delta$, được xác định modulo nhóm nhân $(A^*)^2$ gồm các bình phương của các phần tử khác không của $A$.

#### Nhận xét {#alg-ix-s10-n2-rem-1 .statement}

Khi –1 thuộc lớp mod. $(A^*)^2$ đang xét, nói chung người ta chọn $\omega$ sao cho $\omega^2 = -1$, điều này xác định nó tới dấu. Khi lớp này chứa 1 nhưng không chứa –1, nói chung người ta chọn $\omega$ sao cho $\omega^2 = 1$, điều này lại xác định nó tới dấu.

No. 2

GÓC

Như vậy, mọi phần tử $\varphi$ của $S^+$ đều có thể viết được, theo một và chỉ một cách, dưới dạng

(1)
$$
\varphi = c_w(\varphi) + s_w(\varphi)\omega
$$
trong đó $c_w(\varphi), s_w(\varphi)$ thuộc $A$; phần tử $s_w(\varphi)/c_w(\varphi)$ của trường xạ ảnh $\tilde{A}$ (Chap. II, 2nd ed., App. III, No. 5) được ký hiệu là $t_w(\varphi)$; nó chỉ phụ thuộc vào lớp của $\varphi$ mod. $H$; như vậy $t_w$ xác định, bằng cách chuyển qua thương, một ánh xạ từ $S^+/H$ vào trường xạ ảnh $\tilde{A}$, mà ta lại ký hiệu là $t_w$ do sự lạm dụng ngôn ngữ. Ta sẽ thường viết $c, s$ và $t$ thay cho $c_w, s_w$ và $t_w$. Ta có $c_{-w} = c_w, s_{-w} = -s_w$ và $t_{-w} = -t_w$.

#### Mệnh đề 4 {#alg-ix-s10-prop-4 .statement}

a) Khi $\omega^2 = \delta$ không là một bình phương trong $A$ (nghĩa là khi $E$ không chứa bất kỳ phải đẳng hướng nào), ánh xạ $t$ từ $S^+/H$ vào $\tilde{A}$ là một song ánh.

b) Khi $\delta$ là bình phương của một phần tử $\gamma$ của $A$, ánh xạ $t$ là một song ánh từ $S^+/H$ lên $\tilde{A}$ bỏ đi các phần tử $1/\gamma$ và $-1/\gamma$.

c) Ký hiệu $S^+/H$ theo lối cộng, ta có, với $\varphi, \varphi'$ trong $S^+/H$

(2)
$$
t(\varphi + \varphi') = (t(\varphi) + t(\varphi'))/(1 + \delta t(\varphi)t(\varphi'))
$$
khi $t(\varphi)$ và $t(\varphi')$ là hữu hạn và $1 + t(\varphi)t(\varphi')$ là $\neq 0$.

Thật vậy, vì $S^+/H$ là một tập hợp các đường thẳng (bỏ qua 0) của $A(\Phi)$ được xét như một mặt phẳng vectơ trên $A$, nên $t$ là đơn ánh. Mặt khác, để một phần tử $a + b\omega$ ($a \in A, b \in A$) của $A(\Phi)$ là một phép đồng dạng trực tiếp, điều kiện cần và đủ là nó khả nghịch, nghĩa là phải có $N(a + b\omega) = a^2 - \delta b^2 \neq 0$, hay cũng vậy $(b/a)^2 \neq 1/\delta$; điều này chứng minh các khẳng định về tính toàn ánh trong a) và b). Cuối cùng, tích của các phép đồng dạng $1 + t(\varphi)\omega$ và $1 + t(\varphi')\omega$ là phép đồng dạng $1 + \delta t(\varphi)t(\varphi') + (t(\varphi) + t(\varphi'))\omega$, điều này chứng minh c).

#### Mệnh đề 5 {#alg-ix-s10-prop-5 .statement}

Ta viết $O^+$ theo lối cộng. Với mọi cặp phần tử $\theta, \theta'$ của $O^+$, ta có

(3)
$$
c(\theta)^2 - \delta s(\theta)^2 = 1
$$
(4)
$$
c(\theta + \theta') = c(\theta)c(\theta') + \delta s(\theta)s(\theta')
$$
(5)
$$
s(\theta + \theta') = s(\theta)c(\theta') + c(\theta)s(\theta').
$$

Quan hệ (3) thực ra biểu thị rằng $N(c(\theta) + s(\theta)\omega) = 1$. Đối với (4) và (5), chỉ cần tính, trong $A(\Phi)$, tích của các phép quay $c(\theta) + s(\theta)\omega$ và $c(\theta') + s(\theta')\omega$.

#### Mệnh đề 6 {#alg-ix-s10-prop-6 .statement}

*Gọi d là đẳng cấu từ $S^+/H$ lên $O^+$ được định nghĩa trong Mệnh đề 3. Với mọi phần tử $\varphi$ của $S^+/H$ sao cho $t = t(\varphi)$ là hữu hạn, ta có*

(6)
$$
s(d(\varphi)) = 2t/(1 - \delta t^2), \qquad c(d(\varphi)) = (1 + \delta t^2)/(1 - \delta t^2).
$$

Thật vậy $\varphi$ là lớp mod. $H$ của phép đồng dạng $1 + t\omega$, và do đó phép quay $d(\varphi)$ là $(1 + t\omega)^2/N(1 + t\omega) = (1 + \delta t^2 + 2t\omega)/(1 - \delta t^2)$ (Mệnh đề 3), điều này chứng minh (6).

#### Hệ quả {#alg-ix-s10-n2-cor-1 .statement}

*Với mọi phần tử $\theta$ của $O^+$ sao cho $t(\theta)$ là hữu hạn, ta có*

(7)
$$
s(2\theta) = 2t(\theta)/(1 - \delta t(\theta)^2), \qquad c(2\theta) = (1 + \delta t(\theta)^2)/(1 - \delta t(\theta)^2).
$$
*Với mọi phần tử $\varphi$ của $S^+/H$ sao cho $t(\varphi)$ là hữu hạn và $1 + \delta t(\varphi)^2 \neq 0$, ta có*
(8)
$$
t(2\varphi) = 2t(\varphi)/(1 + \delta t(\varphi)^2).
$$

Thật vậy điều này suy ra ngay lập tức từ Mệnh đề 6 và từ hệ quả của Mệnh đề 3.

#### Nhận xét {#alg-ix-s10-n2-rem-2 .statement}

Các công thức (6) vẫn đúng với $t = \infty$ miễn là ta thay các hàm hữu tỉ xuất hiện ở vế phải bằng các mở rộng chính tắc của chúng lên trường xạ ảnh $\tilde{A}$ (Chương II, ấn bản thứ 2, Phụ lục III, No. 5); thật vậy, nếu $t = \infty$, thì $\varphi$ là lớp của $\omega$, và ta có $d(\varphi) = -1, s(d(\varphi)) = 0$ và $c(d(\varphi)) = -1$; đó quả thực là các giá trị mà các mở rộng chính tắc của các vế phải nhận được khi $t = \infty$. Điều tương tự cũng đúng với (7) khi $t(\theta) = \infty$, và với (8) khi $t(\varphi) = \infty$ hoặc khi $1 + \delta t(\varphi)^2 = 0$. Tương tự, công thức (2) vẫn đúng khi chỉ một trong các phần tử $t(\varphi), t(\varphi'), t(\varphi)$, chẳng hạn, là vô hạn, miễn là ta xét vế phải của nó như một hàm hữu tỉ chỉ theo $t(\varphi)$: thật vậy tích của các phép đồng dạng $1 + t(\varphi')\omega$ và $\omega$ là $\delta t(\varphi') + \omega$, trong khi giá trị mà mở rộng chính tắc của vế phải của (2) nhận được là $1/\delta t(\varphi')$. Cuối cùng, khi $t(\varphi)$ và $t(\varphi')$ là hữu hạn và ta có $1 + \delta t(\varphi)t(\varphi') = 0$, thì ta có $t(\varphi) + t(\varphi') = 0$ (nếu không thì $t(\varphi)^2$ sẽ bằng $1/\delta$, điều này là không thể (mệnh đề 4)); do đó có thể quy ước rằng giá trị của vế phải của (2) là $\infty$, và giá trị này quả thực là giá trị của vế trái. Khi $t(\varphi)$ và $t(\varphi')$ đều vô hạn, vế phải của (2) không được xác định.

### 3. Góc.

Trong Số này và Số tiếp theo, ta sẽ giả sử rằng A là một trường có thứ tự, do đó có đặc số không. Nhắc lại (Đính chính của Chương VI) rằng, nếu F là một không gian vectơ trên A, thì quan hệ "tồn tại $\lambda > 0$ sao cho $y = \lambda x$" là một quan hệ tương đương giữa các phần tử $x, y$ của $F - \{ 0 \}$, rằng mỗi lớp tương đương đối với quan hệ này được gọi là một nửa đường thẳng mở gốc 0, và hợp của một nửa đường thẳng mở với $\{ 0 \}$ được gọi là một nửa đường thẳng đóng (hay đơn giản là nửa đường thẳng) gốc 0; nếu D là một đường thẳng và $\Delta$ là một nửa đường thẳng đóng được chứa trong D, thì D là hợp của $\Delta$ và của $-\Delta$, và không chứa nửa đường thẳng đóng nào khác. Ta sẽ nói rằng một nửa đường thẳng là đẳng hướng nếu đường thẳng chứa nó là đẳng hướng.

Cũng nhắc lại (loc. cit.) rằng, cho một không gian vectơ hữu hạn chiều chiều $n$ trên A, một định hướng trên F là việc cho một trong hai nửa đường thẳng của không gian $\wedge^n F$; các $n$-vectơ thuộc nửa đường thẳng này được gọi là dương. Một không gian vectơ hữu hạn chiều được trang bị một định hướng được gọi là có định hướng.

Các phép vị tự của E có tỉ số $> 0$ hiển nhiên tạo thành một nhóm con chỉ số 2 của H; ta sẽ ký hiệu nó là $H^+$. Đồng cấu chính tắc $i : O^+ \to S^+/H$ (xem mệnh đề 2) là hợp thành của các đồng cấu chính tắc từ $S^+/H^+$ lên $S^+/H$ và từ $O^+$ vào $S^+/H^+$; vì $O^+ \cap H^+ = \{ 1 \}$, đồng cấu sau này là đơn ánh.

#### Mệnh đề 7 {#alg-ix-s10-prop-7 .statement}

Giả sử rằng A là một trường có thứ tự cực đại và $\Phi$ là một dạng dương (§ 7). Khi đó các đồng cấu chính tắc từ $O^+$ vào $S^+/H^+$ và từ $O^+/\{ 1, -1 \}$ vào $S^+/H$ là song ánh, và $S^+$ đẳng cấu với $O^+ \times H^+$.

Ta đã thấy rằng các đồng cấu đang xét là đơn ánh, và chỉ cần chứng minh rằng đồng cấu thứ nhất là toàn ánh. Gọi $(e_1, e_2)$ là một cơ sở trực chuẩn của E, và gọi $\omega$ là phép đồng dạng trực tiếp sao cho $\omega(e_1) = e_2$ (hệ quả 1 của mệnh đề 1, No. 1); khi đó ta có $\omega^2 = -1$ (mệnh đề 1, b)). Cho một phép đồng dạng trực tiếp tùy ý u = a + bw (a \in A,\ b \in A),\ \text{ta có}\ N(u) = a^2 + b^2 > 0,\ \text{và tồn tại một và chỉ một phép quay thuộc cùng nửa đường thẳng của } A(\Phi) \text{ với } u, \text{cụ thể là } (a^2 + b^2)^{1/2}\ u.\ \text{đpcm.}

#### Hệ quả {#alg-ix-s10-n3-cor-1 .statement}

*Cho hai nửa đường thẳng* D, D' *gốc* 0, *tồn tại một và chỉ một phép quay* v *sao cho* v(D) = D'.

Các giả thiết thực ra kéo theo rằng E không chứa đường thẳng đẳng hướng nào. Khi đó mệnh đề của ta suy ra từ hệ quả 1 của mệnh đề 1 (No. 1).

Từ nay về sau ta sẽ giả sử rằng A là một *trường có thứ tự cực đại*, và rằng dạng $\Phi$ là *dương*. Trên tập hợp các cặp $(D_1, D_2)$ các đường thẳng (tương ứng các nửa đường thẳng gốc 0) của E, quan hệ “tồn tại một phép đồng dạng trực tiếp (tương ứng một phép quay) u sao cho $u(D_1) = D'_1$ và $u(D_2) = D'_2$” là một quan hệ tương đương giữa các cặp $(D_1, D_2)$ và $(D'_1, D'_2)$. Lớp tương đương của cặp $(D_1, D_2)$ được gọi, theo định nghĩa, là *góc của các đường thẳng* (tương ứng *nửa đường thẳng*) $D_1, D_2$ (lấy theo thứ tự này); nó được ký hiệu bởi $(\widehat{D_1, D_2})$.

#### Mệnh đề 8 {#alg-ix-s10-prop-8 .statement}

*Giả sử rằng* A *là một trường có thứ tự cực đại*, và rằng *dạng* $\Phi$ *là dương*. *Cho* $D_1, D_2, D'_1, D'_2$ *là bốn đường thẳng* (tương ứng *nửa đường thẳng*) *gốc* 0 *của* E. *Điều kiện cần và đủ để các góc* $(\widehat{D_1, D_2})$ *và* $(\widehat{D'_1, D'_2})$ *bằng nhau là các góc* $(\widehat{D_1, D'_1})$ *và* $(\widehat{D_2, D'_2})$ *bằng nhau*.

Ta hãy chứng minh tính cần thiết của điều kiện đã nêu. Cho u là một phép đồng dạng trực tiếp (tương ứng một phép quay) sao cho $u(D_1) = D'_1$ và $u(D_2) = D'_2$. Tồn tại, theo hệ quả 3 của mệnh đề 1, một phép đồng dạng trực tiếp (tương ứng theo hệ quả của mệnh đề 7, một phép quay) v sao cho $v(D_1) = D_2$. Vì nhóm $S^+$ (tương ứng $O^+$) là *giao hoán*, ta có $D'_2 = u(v(D_1)) = v(u(D_1)) = v(D'_1)$, và điều này cho thấy rằng $(\widehat{D_1, D'_1}) = (\widehat{D_2, D'_2})$. Tính đủ được suy ra từ tính cần bằng cách đổi chỗ $D_2$ và $D'_1$.

Từ mệnh đề 8 suy ra rằng với mỗi góc $(\widehat{D_1, D_2})$ của các đường thẳng (tương ứng nửa đường thẳng) gốc 0 của E, có một phần tử của $S^+/H$ (tương ứng $O^+$) được liên kết với nó một cách chính tắc và được xác định rõ, đó là lớp mod. H của các phép đồng dạng trực tiếp $\varphi$ (tương ứng phép quay $\varphi$) sao cho $u(D_1) = D_2$ với bất kỳ đại diện $(D_1, D_2)$ nào của góc $(\widehat{D_1, D_2})$. Như vậy đã xác định được một song ánh chính tắc $h$ (tương ứng $h'$) từ tập hợp $\mathfrak{A}_0$ các góc của các đường thẳng (tương ứng $\mathfrak{A}$ các góc của các nửa đường thẳng) lên $S^+/H$ (tương ứng $O^+$); đặc biệt, với mọi $\varphi \in \mathfrak{A}$, ta nói rằng $h(\varphi)$ là phép quay góc $\varphi$. Ta sẽ chuyển lên $\mathfrak{A}_0$ và $\mathfrak{A}$, bằng $h^{-1}$ và ${h'}^{-1}$, các cấu trúc nhóm giao hoán của $S^+/H$ và của $O^+$, và ta sẽ ký hiệu theo lối cộng các nhóm $\mathfrak{A}_0$ và $\mathfrak{A}$ thu được như vậy. Nếu $D, D', D''$ ký hiệu các đường thẳng (tương ứng nửa đường thẳng) gốc 0 của E, thì theo định nghĩa ta có

$$
(9) \quad (\widehat{D, D''}) = (\widehat{D, D'}) + (\widehat{D', D''}) \tag{relation de Chasles};
$$

do đó suy ra

$$
(10) \quad (\widehat{D, D}) = 0, \qquad (\widehat{D, D'}) = - (\widehat{D', D}).
$$

#### Nhận xét 1 {#alg-ix-s10-n3-rem-1 .statement}

Tập hợp L các đường thẳng (tương ứng nửa đường thẳng) gốc 0 của E là một không gian thuần nhất đối với nhóm Abel $S^+/H$ (tương ứng $O^+$) sao cho phần tử đơn vị là toán tử duy nhất để bất biến mọi phần tử của L. Do đó có thể áp dụng cho L các công thức của Chương II, 2nd ed., App. II, No. 1; mệnh đề 8 vì thế là một trường hợp riêng của “quy tắc hình bình hành”, và các công thức (9) và (10) là những trường hợp riêng của các công thức (2) (loc. cit.).

#### Nhận xét 2 {#alg-ix-s10-n3-rem-2 .statement}

Trong định nghĩa của nhóm các góc của các đường thẳng, ta có thể, thay vì dùng nhóm $S^+/H$, dùng nhóm $O^+/ \{ -1, 1 \}$ đẳng cấu chính tắc với nó (Mệnh đề 7). Đồng cấu chính tắc của $O^+$ lên $O^+/ \{ -1, 1 \}$ do đó tương ứng với một đồng cấu của $\mathfrak{A}$ lên $\mathfrak{A}_0$, cụ thể là đồng cấu gán cho góc của hai nửa đường thẳng $\Delta, \Delta'$ góc của các đường thẳng $D, D'$ lần lượt chứa $\Delta, \Delta'$. *Trong trường hợp trường A là trường các số thực, nhóm $\mathfrak{A}$ do đó là một phủ cấp 2 của nhóm $\mathfrak{A}_0$*

Theo Mệnh đề 8, mọi góc của các đường thẳng (tương ứng nửa đường thẳng) có dạng $(\widehat{D', D''})$ trong đó $D'$ và $D''$ vuông góc (tương ứng

có dạng ($\widehat{D, - D}$) đều bằng nhau: điều này thực tế suy ra từ Nhận xét 2 của No. 1 (tương ứng là hiển nhiên). Góc của các đường thẳng (tương ứng của các nửa đường thẳng) này được gọi là góc phải (tương ứng góc phẳng); nó là một phần tử cấp 2 của $\mathfrak{A}_0$ (tương ứng của $\mathfrak{A}$).

#### Mệnh đề 9 {#alg-ix-s10-prop-9 .statement}

Giả sử trường $\mathbf{A}$ có thứ tự cực đại, và $\Phi$ là một dạng dương. Với mọi số nguyên $n > 1$, số các phần tử $\theta$ của nhóm $\mathfrak{A}_0$ các góc của các đường thẳng (tương ứng $\mathfrak{A}$ các góc của các nửa đường thẳng) sao cho $n\theta = 0$ bằng $n$.

Vì $\mathfrak{A}_0, S^+/H, \mathfrak{A}$ và $O^+$ là đẳng cấu (Mệnh đề 3), chỉ cần đưa ra chứng minh cho $O^+$, nghĩa là chỉ ra rằng có đúng $n$ phép quay $\varphi$ sao cho $\varphi^n = 1$. Bây giờ, vì $\mathbf{A}$ là một trường có thứ tự cực đại và $\mathbf{A}(\Phi)$ là một trường mở rộng bậc 2 của $\mathbf{A}$ (Mệnh đề 1 a)), $\mathbf{A}(\Phi)$ là một trường đóng đại số (Chương VI, § 2, No. 6, Định lý 3). Do đó các căn bậc $n$ của đơn vị trong $\mathbf{A}(\Phi)$ tạo thành một nhóm xyclic cấp $n$ (Chương V, § 11, No. 1, Định lý 1). Vì ta có $N(u) = u \overline{u} \geqslant 0$ với mọi $u \in \mathbf{A}(\Phi)$, quan hệ $u^n = 1$ kéo theo ta có $N(u) = 1$, do đó $u$ là một phép quay (No. 1, Nhận xét 1). Điều này chứng minh mệnh đề của ta.

#### Hệ quả {#alg-ix-s10-n3-cor-2 .statement}

Góc phải (tương ứng góc phẳng) là phần tử cấp 2 duy nhất của nhóm $\mathfrak{A}_0$ (tương ứng $\mathfrak{A}$).

Cuối cùng, ta sẽ giả sử rằng mặt phẳng $E$ được định hướng.

#### Bổ đề 1 {#alg-ix-s10-lem-1 .statement}

Cho $u$ là một phép đồng dạng trực tiếp của $E$; tất cả các song vectơ có dạng $x \wedge u(x)$ đều thuộc cùng một nửa đường thẳng đóng của $\overset{2}{\wedge} E$.

Trường hợp $u$ là một phép vị tự là tầm thường. Trong trường hợp trái lại ta có $x \wedge u(x) \neq 0$ với mọi $x \neq 0$; cho $x, y$ là hai vectơ của $E$ ($x \neq 0, y \neq 0$); tồn tại $\varphi \in S^+$ sao cho $y = \varphi(x)$, do đó $y \wedge u(y) = \varphi(x) \wedge u \varphi(x) = \varphi(x) \wedge \varphi(u(x)) = (\det \varphi)(x \wedge u(x))$; chọn một cơ sở trực chuẩn của $E$, ta thấy rằng $\det \varphi$ là dương (Mệnh đề 1 b)); do đó suy ra mệnh đề của chúng ta.

Như vậy, trong hai phần tử sinh $\omega$ của $\mathbf{A}(\Phi)$ sao cho $\omega^2 = -1$, tồn tại một và chỉ một phần tử sao cho lưỡng vectơ $x \wedge \omega(x)$ là dương với mọi $x \in E$. Chính phần tử sinh này mà ta sẽ chọn để định nghĩa các hàm $c_w, s_w$ và $t_w$ (No. 2). Cho $h$ và $h'$ là các song ánh chính tắc được định nghĩa ở trên từ nhóm $\mathfrak{A}_0$ các góc của các đường thẳng lên $S^+/H$ và từ nhóm $\mathfrak{A}$ các góc của các nửa đường thẳng lên $O^+$. Các ánh xạ hợp thành $t_w \circ h$ từ $\mathfrak{A}_0$ vào trường xạ ảnh $\tilde{\mathfrak{A}}$, $c_w \circ h'$ và $s_w \circ h'$ từ $\mathfrak{A}$ vào trường $A$ được ký hiệu tương ứng bởi $\operatorname{tg}$, $\cos$ và $\sin$, và được gọi là các *hàm tang*, *côsin* và *sin*. Ánh xạ $\varphi \to 1/\operatorname{tg} \varphi$ từ $\mathfrak{A}_0$ vào $\tilde{\mathfrak{A}}$ được ký hiệu bởi $\operatorname{cotg}$ và được gọi là *hàm côtang*. Ta nói rằng các hàm sin, tang và côtang là các *hàm lượng giác*. Các ánh xạ hợp thành $\operatorname{tg} \circ p$ và $\operatorname{cotg} \circ p$, trong đó $p$ ký hiệu đồng cấu chính tắc của $\mathfrak{A}$ lên $\mathfrak{A}_0$ (Nhận xét 2 ở trên), lại được ký hiệu bởi $\operatorname{tg}$ và $\operatorname{cotg}$ do lạm dụng ngôn ngữ.

Các công thức (2), (8), (3), (4), (5) và (7) của No. 2 cho, vì ở đây ta có $\delta = -1$

$$
\begin{align*}
(11) \quad & \operatorname{tg} (\varphi + \varphi') = (\operatorname{tg} \varphi + \operatorname{tg} \varphi')/(1 - \operatorname{tg} \varphi \operatorname{tg} \varphi') \\
(12) \quad & \operatorname{tg} (2\varphi) = 2 \operatorname{tg} \varphi/(1 - \operatorname{tg}^2 \varphi)
\end{align*}
$$

với $\varphi, \varphi'$ trong $\mathfrak{A}_0$;

$$
\begin{align*}
(13) \quad & \cos^2 \theta + \sin^2 \theta = 1 \\
(14) \quad & \cos (\theta + \theta') = \cos \theta \cos \theta' - \sin \theta \sin \theta' \\
(15) \quad & \sin (\theta + \theta') = \sin \theta \cos \theta' + \cos \theta \sin \theta' \\
(16) \quad & \left\{ \begin{array}{l}
\sin (2\theta) = 2 \operatorname{tg} \theta/(1 + \operatorname{tg}^2 \theta), \\
\cos (2\theta) = (1 - \operatorname{tg}^2 \theta)/(1 + \operatorname{tg}^2 \theta)
\end{array} \right.
\end{align*}
$$

với $\theta, \theta'$ trong $\mathfrak{A}$. Mặt khác ta có, theo định nghĩa hoặc như một hệ quả dễ dàng của các công thức trên:

$$
\begin{align*}
(17) \quad & \operatorname{tg} \theta = \sin \theta/\cos \theta, \qquad \operatorname{cotg} \theta = \cos \theta/\sin \theta \\
(18) \quad & 1 + \operatorname{tg}^2 \theta = 1/\cos^2 \theta, \qquad 1 + \operatorname{cotg}^2 \theta = 1/\sin^2 \theta
\end{align*}
$$

với $\theta \in \mathfrak{A}$.

Cho hai vectơ khác không $x, y$ của $E$, *góc* của hai vectơ này (lấy theo thứ tự ấy) được định nghĩa là, và được ký hiệu bởi $\widehat{(x, y)}$, góc của các tia mà chúng thuộc vào. Với mọi vectơ $x$ của $E$, *độ dài* của $x$ được định nghĩa là, và được ký hiệu bởi $|x|$, phần tử $\Phi(x, x)^{1/2}$ của $A$.

#### Mệnh đề 10 {#alg-ix-s10-prop-10 .statement}

Giả sử rằng trường $\mathbf{A}$ là có thứ tự cực đại, rằng mặt phẳng $\mathbf{E}$ được định hướng, và rằng dạng $\Phi$ là dương. Với mọi cặp vectơ khác không $x, y$ của $\mathbf{E}$, ta có

$$
\cos (\widehat{x, y}) = \Phi(x, y)/|x|.|y|
$$
$$
\sin (\widehat{x, y}).e = (x \wedge y)/|x|.|y|,
$$

trong đó $e$ ký hiệu lưỡng vectơ dương sao cho $\Phi_{(2)}(e, e) = 1$.

Thật vậy, vì các vectơ $x' = x/|x|$ và $y' = y/|y|$ đều có độ dài bằng 1, nên tồn tại một và chỉ một phép quay $\varphi$ sao cho $\varphi(x') = y'$ (No. 1, Hệ quả 2 của Mệnh đề 1). Nếu viết $\varphi = a + b \omega$ ($a, b$ trong $\mathbf{A}$), thì theo định nghĩa ta có $a = \cos (\widehat{x, y})$ và $b = \sin (\widehat{x, y})$. Quan hệ $y' = \varphi(x') = ax' + b \omega(x')$ cho $\Phi(x', y') = a \Phi(x', x') = a$ vì $x'$ và $\omega(x')$ trực giao (Nhận xét 2 của No. 1); điều này chứng minh (19). Mặt khác quan hệ này cũng cho $x' \wedge y' = bx' \wedge \omega(x') = b.e$ theo định nghĩa của mở rộng $\Phi_{(2)}$ của $\Phi$ lên $\bigwedge^2 \mathbf{E}$ ($§ 1,$ No. 9, công thức (37)) và theo lựa chọn của $\omega$; điều này chứng minh (20).

#### Nhận xét 3 {#alg-ix-s10-n3-rem-3 .statement}

Cho hai đường thẳng (tương ứng, tia) $D, D'$ của một *mặt phẳng afin* $L$ gắn với $E$, góc của $D$ và $D'$ được định nghĩa là, và được ký hiệu bởi $(\widehat{D, D'})$, góc tạo bởi các phương của chúng trong $E$ (tương ứng, bởi các tia gốc 0 của $E$ tương ứng với $D$ và $D'$) (Chương II, ấn bản thứ 2, Phụ lục II, No. 1 và No. 3).

#### Nhận xét 4 {#alg-ix-s10-n3-rem-4 .statement}

Cho $F$ là một không gian vectơ *có chiều tùy ý* trên trường có thứ tự cực đại $\mathbf{A}$, và cho $\Psi$ là một dạng song tuyến tính đối xứng không suy biến dương trên $F$. Cho hai vectơ độc lập tuyến tính $x, y$ của $F$, gọi $F'$ là mặt phẳng vectơ mà chúng sinh; *góc* của $x$ và $y$ được định nghĩa là góc của $x$ và $y$ khi xét như các phần tử của mặt phẳng $F'$; nó được ký hiệu bởi $(\widehat{x, y})$. Cosin của góc này, theo (19), được cho bởi

$$
\cos (\widehat{x, y}) = \Psi(x, y)/|x|.|y|
$$

(với $|x| = \Psi(x, x)^{1/2}$ còn được gọi là *độ dài* của vectơ $x$), và do đó là *độc lập với định hướng đã chọn* trên $F'$; sin và tang của $(\widehat{x, y})$ đổi dấu nếu ta thay đổi định hướng của $F'$. Cho hai vectơ tỉ lệ khác không $x, y$ của $F$, theo quy ước ta đặt $(\widehat{x, y}) = 0$.

### 4. Các cung góc.

Trước hết ta sẽ giả thiết, không thêm bất kỳ giả thiết nào khác, rằng E là một mặt phẳng có định hướng trên trường có thứ tự A. Ta nói rằng ba nửa đường thẳng D₀, D₁, D₂ (có gốc 0) của E tạo thành một dãy trực tiếp nếu, với $xᵢ ∈ Dᵢ$, $xᵢ ≠ 0$ (i = 0, 1, 2), ít nhất hai trong các song vectơ $x₀ ∧ x₁, x₁ ∧ x₂, x₂ ∧ x₀$ là > 0; trong trường hợp này các dãy D₁, D₂, D₀ và D₂, D₀, D₁ cũng là trực tiếp. Hiển nhiên rằng ba nửa đường thẳng tạo thành một dãy trực tiếp là phân biệt. Cho hai nửa đường thẳng D₁, D₂ của E, cung góc mở (tương ứng đóng) có gốc D₁ và đầu mút D₂ là tập hợp (hoặc, do lạm dụng ngôn ngữ, hợp) của các nửa đường thẳng D sao cho dãy D₁, D, D₂ là trực tiếp (tương ứng sao cho D = D₁ hoặc D = D₂ hoặc dãy D₁, D, D₂ là trực tiếp).

#### Mệnh đề 11 {#alg-ix-s10-prop-11 .statement}

Cho E là một mặt phẳng có định hướng trên một trường có thứ tự A, D₀ là một nửa đường thẳng của E, và G là tập hợp các nửa đường thẳng của E phân biệt với D₀. Quan hệ

“D₁ = D₂, hoặc dãy D₀, D₁, D₂ là trực tiếp”

giữa các phần tử D₁, D₂ của G là một quan hệ thứ tự toàn phần trong G.

Thật vậy, các tiên đề của các quan hệ thứ tự toàn phần được kiểm tra một cách hiển nhiên, ngoại trừ tính bắc cầu. Cho D₁, D₂, D₃ là ba nửa đường thẳng sao cho các dãy D₀, D₁, D₂ và D₀, D₂, D₃ là trực tiếp; ta sẽ bây giờ chứng minh rằng dãy D₀, D₁, D₃ là trực tiếp. Vì vậy hãy lấy một vectơ $xᵢ ≠ 0$ trong Dᵢ (i = 0, 1, 2, 3), chọn một song vectơ e > 0, và đặt $xᵢ ∧ xⱼ = aᵢⱼe (aᵢⱼ ∈ A)$. Viết $e = x₀ ∧ y (y ∈ E)$, và lấy $(x₀, y)$ làm một cơ sở của E, ta dễ dàng kiểm tra được quan hệ

$$
a_{01}a_{23} + a_{02}a_{31} + a_{03}a_{12} = 0.
$$

Điều này cho thấy rằng, nếu a₀₁ ≤ 0, thì ta có a₁₂ > 0 và a₂₀ > 0 (vì dãy thứ nhất là trực tiếp), rồi a₂₃ > 0 và a₃₀ > 0 (vì a₀₂ < 0 và dãy thứ hai là trực tiếp), do đó a₁₃ > 0 (theo (22)); vì vậy dãy (D₀, D₁, D₃) là trực tiếp trong trường hợp này. Từ nay giả sử rằng a₀₁ > 0. Nếu a₃₀ ≤ 0, ta có a₀₂ > 0 và a₂₃ > 0 (vì dãy thứ hai là trực tiếp), rồi a₁₂ > 0 (vì a₂₀ < 0 và dãy thứ nhất là trực tiếp), do đó $a_{13} > 0$ (theo (22)), và dãy $(D_0, D_1, D_3)$ là trực tiếp. Cuối cùng hiển nhiên là tương tự nếu $a_{01} > 0$ và $a_{30} > 0$. QED.

#### Hệ quả {#alg-ix-s10-n4-cor-1 .statement}

*Cho $D_1$ và $D_2$ là hai nửa đường thẳng phân biệt của E. Với mọi nửa đường thẳng $D_0$ của E sao cho dãy $D_0, D_1, D_2$ là trực tiếp, tập hợp các nửa đường thẳng $D$ của E sao cho $D_1 < D < D_2$ (đối với quan hệ thứ tự toàn phần được xác định bởi $D_0$) bằng cung góc mở có gốc $D_1$ và đầu mút $D_2$.

Thật vậy, cho một nửa đường thẳng $D_3$, vấn đề là chứng minh rằng các quan hệ “dãy $D_1, D_3, D_2$ là trực tiếp” và “các dãy $D_0, D_1, D_3$ và $D_0, D_3, D_2$ là trực tiếp” là tương đương. Để ngắn gọn, ta ký hiệu bởi $(ijk)$ quan hệ “dãy $(D_i, D_j, D_k)$ là trực tiếp”. Theo mệnh đề 11, phép hội của (132) và (120) kéo theo (130); tương tự, phép hội của (201) và (213) kéo theo (203); do đó ta có một nửa của mệnh đề của mình. Ngược lại, giả sử (012), (013), và (032); vì phép hội của (312) và (320) kéo theo (310) (mệnh đề 11), và vì (310) và (013) không tương thích, (312) là sai; điều này chứng minh (132) và hoàn tất chứng minh.

Theo hệ quả trước, cung góc mở (tương ứng đóng) có gốc $D_1$ và đầu mút $D_2$ được ký hiệu bởi $\{D_1, D_2\}$ (tương ứng $[D_1, D_2]$), với điều hiểu rằng đây là các khoảng đối với cấu trúc thứ tự được xác định bởi bất kỳ nửa đường thẳng $D_0$ nào sao cho dãy $D_0, D_1, D_2$ là trực tiếp.

#### Mệnh đề 12 {#alg-ix-s10-prop-12 .statement}

*Cho A là một trường có thứ tự cực đại, E là một mặt phẳng có định hướng trên A, $D_0$ là một nửa đường thẳng của E, và G là tập hợp các nửa đường thẳng của E phân biệt với $D_0$. Các tập hợp có thứ tự toàn phần A và G (mệnh đề 11) là đẳng cấu.

Thật vậy, $(x, y)$ là một cơ sở của E sao cho $x \in - D_0$ và song vectơ $x \wedge y$ là $> 0$. Với mỗi phần tử $t$ của A, ta cho tương ứng nửa đường thẳng $f(t)$ mà vectơ $(1 - t^2)x + 2ty$ thuộc vào. Hiển nhiên rằng $f(A) \subset G$. Ta hãy chứng minh rằng $f$ tăng ngặt. Thật vậy, để dãy $D_0, f(t), f(t')$ ($t, t'$ trong A) là trực tiếp, theo định nghĩa, điều kiện cần và đủ là ít nhất hai trong các phần tử

$$
-2t, \quad (1-t^2)2t' - (1-{t'}^2)2t, \quad 2t'
$$

hãy cho chúng là $> 0$. Bây giờ cái thứ hai bằng $2(t' - t)(1 + tt')$. Do đó, nếu $t < t'$, thì hoặc $tt' \geqslant 0$, do đó $t' > 0$ hoặc $-t > 0$, hoặc $tt' < 0$, do đó $-t > 0$ và $t' > 0$; trong mọi trường hợp $D_0, f(t), f(t')$ là trực tiếp. Vì $A$ được sắp thứ tự toàn phần, $f$ là một đẳng cấu của $A$ lên tập hợp có thứ tự $f(A)$ (*Ens*, chương III, § 1, No. 14, Mệnh đề 13).

Còn phải chứng minh rằng $f$ là *toàn ánh*. Vì mục đích này, xét dạng dương $\Phi$ trên $E$ sao cho $(x, y)$ là một cơ sở trực chuẩn đối với $\Phi$. Với mỗi nửa đường thẳng $D \in G$, tồn tại một góc $\varphi$ và duy nhất một góc như vậy sao cho $2\varphi = (\widehat{-D_0, D})$ (No. 1, Mệnh đề 3); vì $(\widehat{-D_0, D})$ không phải là góc bẹt, $\varphi$ không phải là góc phải, và do đó $\operatorname{tg} \varphi$ là hữu hạn. Khi đó, theo các công thức (16) (No. 3), ta có $D = f(\operatorname{tg} \varphi)$. Điều này hoàn tất chứng minh.

*Bài tập.* 1) Với ký hiệu của No. 1, đặt $Q(x) = \Phi(x, x)$; không gian vectơ $E$ được đồng nhất một cách chính tắc với $C^-(Q)$ (§ 9, No. 1). Với mọi $z \in C^+(Q)$, và mọi $x \in E$, ta có $zx \in E$; hãy chứng minh rằng $x \to zx$ là một phần tử của $A(\Phi)$, và rằng $z \to s_z$ là một đẳng cấu của $C^+(Q)$ lên đại số $A(\Phi)$.

2) Các giả thiết và ký hiệu là những giả thiết và ký hiệu của No. 1 và của Bài tập 1.

(a) Gọi $C$ là tập hợp các $x \in E$ sao cho $\Phi(x, x) = 1$ (*đường tròn đơn vị*), và gọi $\mathcal{D}$ là tập hợp các đường thẳng $D$ mà giao của chúng với $C$ là khác rỗng (và do đó gồm hai phần tử đối của $E$). Một *đường thẳng có điểm đánh dấu* là, theo định nghĩa, bất kỳ cặp nào $\Delta = (D, z)$ được tạo bởi một đường thẳng $D \in \mathcal{D}$ và một trong các điểm $z \in D \cap C$. Bây giờ chứng minh rằng nếu $\Delta_1 = (D_1, z_1)$, $\Delta_2 = (D_2, z_2)$ là hai đường thẳng có điểm đánh dấu, thì tồn tại một và chỉ một phép quay $u$ sao cho $u(z_1) = z_2$ (và do đó $u(D_1) = D_2$), điều này được biểu thị bằng cách viết $u(\Delta_1) = \Delta_2$. Trong tập hợp các cặp $(\Delta_1, \Delta_2)$ của các đường thẳng có điểm đánh dấu, quan hệ “tồn tại một phép quay $u$ sao cho $u(\Delta_1) = \Delta_1'$ và $u(\Delta_2) = \Delta_2'$” là một quan hệ tương đương. Tập hợp $\mathfrak{U}_1$ các lớp tương đương của các cặp đường thẳng có điểm đánh dấu đối với quan hệ này được gọi là tập hợp các *góc của các đường thẳng có điểm đánh dấu*, và lớp tương đương mà một cặp $(\Delta_1, \Delta_2)$ các đường thẳng có điểm đánh dấu thuộc về được gọi là *góc* của cặp này và được ký hiệu bởi $(\widehat{\Delta_1, \Delta_2})$; quan hệ $(\widehat{\Delta_1, \Delta_2}) = (\widehat{\Delta_1', \Delta_2'})$ tương đương với $(\widehat{\Delta_1, \Delta_1'}) = (\widehat{\Delta_2, \Delta_2'})$ và phép quay biến $\Delta_1$ thành $\Delta_2$ được gọi là một *phép quay góc* $0 = (\widehat{\Delta_1, \Delta_2})$ và được ký hiệu bởi $h_1(\theta)$; $h_1$ là một song ánh của $\mathfrak{U}_1$ lên $O^+$, và cấu trúc nhóm giao hoán của $O^+$ được chuyển sang $\mathfrak{U}_1$ nhờ $h_1^{-1}$, nhóm $\mathfrak{U}_1$ được xác định như vậy được viết theo phép cộng; góc của cặp tạo bởi một đường thẳng có điểm đánh dấu $(D, z)$ và đường thẳng có điểm đánh dấu “đối” $(D, -z)$, tương ứng với phép quay $x \to -x$, lại được gọi là góc *phẳng* trong $\mathfrak{U}_1$.

b) Trong tập hợp $\mathcal{D}_0 \supset \mathcal{D}$ các đường thẳng không đẳng hướng, ta định nghĩa như trong No. 3 khái niệm *góc của các đường thẳng*, nhóm $\mathfrak{U}_0$ (dùng Hệ quả 3 của Mệnh đề 1 của No. 1), góc *phải* trong $\mathfrak{U}_0$, và song ánh chính tắc $h$ của $\mathfrak{U}_0$ lên $S^+/H$. Với ký hiệu của hệ quả của Mệnh đề 3, đặt $\bar{d} = h_1^{-1} \circ d \circ h$ và $\bar{i} = h^{-1} \circ i \circ h_1$, sao cho $\bar{i}$ là một đồng cấu của $\mathfrak{U}_1$ vào $\mathfrak{U}_0$ và $\bar{d}$ là một đồng cấu của $\mathfrak{U}_0$ vào $\mathfrak{U}_1$; $\bar{d}$ là song ánh, và hạt nhân của $\bar{i}$ gồm '0 và góc phẳng; hơn nữa ta có $\bar{d}(\bar{i}(\theta)) = 2\theta$ với $\theta \in \mathfrak{U}_1$ và $\bar{i}(\bar{d}(\varphi)) = 2\varphi$ với $\varphi \in \mathfrak{U}_0$. Để $\bar{i}$ là toàn ánh (nói cách khác, để $\mathcal{D}$ là tập hợp của tất cả các đường thẳng không đẳng hướng), điều kiện cần và đủ là trường A là *Pitago* (Chương VI, § 2, Bài tập 8 d)) và tồn tại một cơ sở trực chuẩn của $\Phi$; điều này tương đương với việc nói rằng $\Phi(x, x)$ là một *bình phương* với mọi $x \in E$.

3) Các giả thiết và ký hiệu là của Bài tập 2.
   a) Cho s là một đối xứng đối với một đường thẳng không đẳng hướng D ($§ 6$, No. 4). Với mọi đường thẳng có điểm gốc $\Delta_1 = (D_1, z_1)$, đặt
   $$
   \Delta_2 = s(\Delta_1) = (s(D_1), s(z_1)),
   $$
   và đặt $\varphi = (\widehat{D_1}, \widehat{D})$; bây giờ chứng minh rằng ta có $(\widehat{\Delta_1}, \widehat{\Delta_2}) = \bar{d}(\varphi)$.
   b) Bây giờ chứng minh rằng mọi phép biến đổi trực giao có định thức -1 là một đối xứng s đối với một đường thẳng không đẳng hướng (xem § 6, Bài tập 15 e)); với mọi phép quay u, ta có $sus^{-1} = u^{-1}$.
   c) Nếu $x, y$ là hai điểm bất kỳ của E sao cho $\Phi(x, x) = \Phi(y, y) \neq 0$, thì tồn tại duy nhất một đối xứng đối với một đường thẳng không đẳng hướng, biến đổi $x$ thành $y$.
   d) Cho s, s' là các đối xứng đối với hai đường thẳng không đẳng hướng D, D', và đặt $\varphi = (\widehat{D}, \widehat{D'})$; để s’s là một phép quay góc $\theta$, điều kiện cần và đủ là $\bar{d}(\varphi) = \theta$.
   e) Bây giờ chứng minh rằng nhóm con giao hoán tử của nhóm trực giao O(Q) là ảnh của $\mathfrak{U}_1$ qua đồng cấu $\theta \to h_1(2\theta)$ ($§ 6$, Bài tập 17 a)); để ảnh này bằng $O^+$, điều kiện cần và đủ là đồng cấu $\bar{i}$ là toàn ánh (Bài tập 2 b)).

4) Các giả thiết và ký hiệu là những giả thiết và ký hiệu của Bài tập 2. Cho $a, b$ là hai điểm của đường tròn C, $\Delta_a, \Delta_b$ lần lượt là các đường thẳng chỉ phương đi qua $a$ và $b$ (và đi qua 0), và đặt $\theta = (\widehat{\Delta_a}, \widehat{\Delta_b})$. Với mọi $x \in E$, phân biệt với $a$ và $b$, gọi $D_{xa}$ (tương ứng $D_{xb}$) là đường thẳng afin đi qua $a$ và $x$ (tương ứng $b$ và $x$), và gọi $D'_{xa}$ (tương ứng $D'_{xb}$) là phương của $D_{xa}$ (tương ứng $D_{xb}$); hãy chứng minh rằng, đối với $x \in C$ ($x$ phân biệt với $a$ và $b$), điều kiện cần và đủ là góc $\varphi = (\widehat{D'_{xa}}, \widehat{D'_{xb}})$ phải thỏa mãn $\bar{d}(\varphi) = \theta$ (dùng Bài tập 3). Kết quả này được biến đổi như thế nào khi $x = a$ hoặc $x = b$ (xem § 6, Bài tập 25 a))?

5) Với các ký hiệu của các Mục 1 và 2 và của Bài tập 2, giả sử rằng $\Phi$ có chỉ số 1, nói cách khác rằng $\delta$ là một bình phương $\gamma^2$ trong A; gọi $D_1, D_2$ là các đường đẳng hướng của E, lần lượt chứa các vectơ $e_1 - \frac{1}{\gamma} e_2$ và $e_1 + \frac{1}{\gamma} e_2$.
   a) Hãy chứng minh rằng nhóm các phép quay $O^+$ là đẳng cấu với nhóm nhân $A^*$ của trường A.
   b) Với mọi góc $\theta \in \mathfrak{U}_1$, đặt $e_w(\theta) = c_w(h_1(\theta)) + \gamma s_w(h_1(0))$. Hãy chứng minh rằng $\theta \to e_w(\theta)$ là một đẳng cấu của $\mathfrak{U}_1$ lên nhóm $A^*$.

c) Cho D, D' là hai đường thẳng bất kỳ, và đặt $\varphi = (\widehat{D}, \widehat{D'})$. Hãy chứng minh rằng tỉ số chéo $\begin{bmatrix} D_1 & D_2 \\ D' & D \end{bmatrix}$ (Chương II, ấn bản thứ 2, Phụ lục III, Bài tập 5) bằng $e_w(\bar{d}(\varphi))$ ("công thức Laguerre"). (Nhận xét rằng $D_1$ và $D_2$ là bất biến dưới mọi phép đồng dạng trực tiếp, và bằng cách dùng Bài tập 4 c) của Chương II, ấn bản thứ 2, Phụ lục III, rút gọn về trường hợp $D = Ae_1$.)

6) Giả sử rằng A là một trường có thứ tự.
a) Cho $D_1, D_2$ là hai nửa đường thẳng không đẳng hướng có gốc 0. Hãy chứng minh rằng tồn tại một phép đồng dạng trực tiếp $u$ sao cho $u(D_1) = D_2$; mọi phép đồng dạng trực tiếp khác có tính chất này đều có dạng $v = su$, trong đó s là một phép vị tự với tỉ số $> 0$.

b) Trên tập hợp các cặp $(D_1, D_2)$ của các nửa đường thẳng không đẳng hướng, quan hệ “tồn tại một phép đồng dạng trực tiếp $u$ sao cho $u(D_1) = D'_1$ và $u(D_2) = D'_2$” là một quan hệ tương đương. Tập hợp $\mathfrak{A}$ các lớp tương đương của các nửa đường thẳng không đẳng hướng, đối với quan hệ này, được gọi là tập hợp các góc của các nửa đường thẳng (không đẳng hướng), và lớp tương đương của một cặp $(D_1, D_2)$ gồm các nửa đường thẳng như vậy được gọi là góc của cặp này và được ký hiệu bởi $(\widehat{D_1}, \widehat{D_2})$; nếu $\theta = (\widehat{D_1}, \widehat{D_2})$, người ta nói rằng $\theta$ là góc của mọi phép đồng dạng trực tiếp biến $D_1$ thành $D_2$; gọi $h_2(\theta)$ là lớp mod. $H^+$ của các phép đồng dạng này, sao cho $h_2$ là một song ánh từ tập hợp $\mathfrak{A}$ lên nhóm $S^+/H^+$; người ta chuyển sang $\mathfrak{A}$ bằng cách sử dụng $h_2^{-1}$ cấu trúc nhóm giao hoán của $S^+/H^+$, ký hiệu cộng cho nhóm $\mathfrak{A}$ được định nghĩa như vậy. Định nghĩa một đơn ánh chính tắc $\bar{j}$ của nhóm $\mathfrak{A}_1$, của các góc của các đường thẳng có điểm gốc (exerc. 2) vào nhóm $\mathfrak{A}$, sao cho $h_2 \circ \bar{j} \circ h_2^{-1}$ là đơn ánh chính tắc $j$ của $O^+$ vào $S^+/H^+$. Để $\bar{j}$ là toàn ánh, điều kiện cần và đủ là đồng cấu $\bar{i}$ của $\mathfrak{A}_1$ vào $\mathfrak{A}_0$ (exerc. 2 b)) là toàn ánh.

c) Bây giờ chứng minh rằng trong $\mathfrak{A}$ phương trình $2\theta = 0$ có 2 nghiệm nếu $\delta < 0$ và 4 nghiệm nếu $\delta > 0$. Trong trường hợp thứ nhất, nghiệm $\varpi \neq 0$ của phương trình này lại được gọi là góc phẳng.

¶ 7) Với các giả thiết và ký hiệu là của exerc. 6, giả sử đồng cấu $\bar{j}$ song ánh; khi đó người ta định nghĩa cos $\theta$ và sin $\theta$ với mọi $\theta \in \mathfrak{A}$ như trong No. 3. Gọi T là tập hợp các $\theta \in \mathbf{A}$ sao cho $\sin \theta \geqslant 0$.

a) Bây giờ chứng minh rằng với mọi $\theta \in T$, tồn tại một góc $\theta' \in T$, và chỉ một góc duy nhất, sao cho $2\theta' = \theta$; người ta đặt $\theta' = \theta/2$.

b) Cho L là $\mathbf{Z}$-môđun của các tổ hợp tuyến tính hình thức của các phần tử của T với các hệ số trong $\mathbf{Z}$ (Chương II, § 1, No. 8); ký hiệu $\xi + \eta$ và $-\xi$ lần lượt là tổng và phần tử đối trong L. Cho N là môđun con của L sinh bởi các phần tử của L có dạng $\xi + \eta - (\xi + \eta)$ đối với mọi cặp $(\xi, \eta)$ các phần tử của T sao cho $\xi + \eta \in T$ (tổng lấy trong nhóm $\mathfrak{A}$). Cho $\dot{f}$ là đồng cấu từ L vào $\mathfrak{A}$ mở rộng đơn ánh chính tắc của T vào $\mathfrak{A}$, và $\dot{g}$ là tự đồng cấu của L mở rộng ánh xạ $\theta \to \theta/2$ của T vào chính nó. Ta có $\dot{f}(N) = \{0\}$ và $\dot{g}(N) \subset N$; bằng cách chuyển qua các thương, ta suy ra từ $\dot{f}$ một đồng cấu $f$ của $M = L/N$ vào $\mathfrak{A}$, và từ $\dot{g}$ một tự đồng cấu $g$ của $M$; ta đặt $g(\mu) = \mu/2$ và nếu $g^m$ là lặp thứ m của g, $g^m(\mu) = 2^{-m}\mu$; ta có $2^m(2^{-m}\mu) = \mu$ với mọi $\mu \in M$.

c) Chứng minh rằng hạn chế vào T của ánh xạ chính tắc $\psi$ của L lên $M = L/N$ là đơn ánh, điều này cho phép đồng nhất T với một tập con của M nhờ $\psi$. Chứng minh rằng, nếu $\lambda_1, \ldots, \lambda_m$ là các phần tử $\neq 0$ của T, tổng $\lambda_1 + \lambda_2 + \cdots + \lambda_m$ không thể bằng 0 trong M (xét phần tử $2^{-m}(\lambda_1 + \cdots + \lambda_m)$ và lập luận bằng quy nạp theo m, nhận thấy rằng các phần tử này thuộc T).

d) Cho $M_+$ là tập hợp các tổng hữu hạn (trong M) của các phần tử của T; chứng minh rằng $M_+ \cap (-M_+) = \{0\}$ và $M = M_+ \cup (-M_+)$, và do đó $M_+$ là tập hợp các phần tử $\geqslant 0$ đối với một cấu trúc nhóm có thứ tự toàn phần trên M (cần nhận thấy rằng với mọi $\mu \in M_+$, tồn tại một số nguyên m sao cho $2^{-m}\mu \in T$); nhóm có thứ tự toàn phần này được gọi là nhóm các độ đo của các góc của các nửa đường thẳng. Chứng minh rằng đồng cấu $f$ của M vào $\mathfrak{A}$ là toàn ánh, và rằng hạt nhân của nó là tập hợp các bội nguyên của $2\pi$, trong đó $\pi$ là góc thẳng (Bài tập 6 c)). Chứng minh rằng T được đồng nhất với khoảng $[0, \pi]$ trong M (thiết lập bằng quy nạp theo m rằng nếu $\mu, \lambda_1, \ldots, \lambda_m$ thuộc T và nếu có $\lambda_1 + \cdots + \lambda_m \leqslant \mu$, thì $\lambda_1 + \cdots + \lambda_m \in T$). Chứng minh rằng trong T (được đồng nhất như vậy với một khoảng của M), hàm $\theta \to \cos \theta$ là giảm nghiêm ngặt.

e) Để nhóm có thứ tự toàn phần M là Archimede (Chương VI, § 1, Bài tập 31), điều kiện cần và đủ là nhóm cộng của trường A là Archimede. (Để thấy rằng điều kiện là cần, nhận thấy rằng nếu sin $\theta$ là vô hạn bé đối với trường con $\mathbf{Q}$ của A (Chương VI, § 2, Bài tập 1), điều tương tự cũng đúng với sin $n\theta$ với mọi số nguyên n. Để thấy rằng điều kiện là đủ, nhận thấy rằng nếu $0 \leqslant \theta \leqslant \pi/4$, ta có sin $2\theta \geqslant \sqrt{2} \sin \theta$).

8) Cho E là một mặt phẳng định hướng trên một trường có thứ tự A. Cho D', D'' là hai nửa đường thẳng phân biệt; cho $x'$ (tương ứng $x''$) là một vectơ $\neq 0$ trong D' (tương ứng D''); cung góc (mở hoặc đóng) có gốc D' và tận cùng D'' được gọi là nhọn (tương ứng lõm lại, thẳng) nếu $x' \wedge x'' > 0$ (tương ứng $x' \wedge x'' < 0, x' \wedge x'' = 0$).

a) Để tồn tại một tự đẳng cấu của không gian vectơ E biến một hình quạt góc mở (tương ứng, đóng) $\Sigma_1$ thành một hình quạt góc mở (tương ứng, đóng) $\Sigma_2$, điều kiện cần và đủ là $\Sigma_1$ và $\Sigma_2$ đều nhọn, hoặc đều lõm vào, hoặc đều phẳng.

b) Chứng minh rằng tập hợp có thứ tự $\{D', D''\}$ là đẳng cấu với khoảng $[0, 1]$ của A (trước hết xét trường hợp một hình quạt nhọn và nhận xét rằng, trong A, hai khoảng đóng bị chặn bất kỳ đều là các tập hợp có thứ tự đẳng cấu).

c) Với các ký hiệu và giả thiết của Bài tập 7, định nghĩa một ánh xạ song ánh chính tắc của tập hợp T lên một hình quạt góc phẳng, và chứng minh rằng ánh xạ này là một đẳng cấu đối với các cấu trúc thứ tự.

9) Cho A là một trường có thứ tự Pythagore, E là một không gian vectơ hữu hạn chiều trên A, Q là một dạng toàn phương dương không suy biến trên E, sao cho E thừa nhận một cơ sở trực chuẩn (nghĩa là Q(x) là một bình phương trong A với mọi x ∈ E). Chứng minh rằng nhóm giao hoán tử Ω(Q) của nhóm trực giao O(Q) là nhóm quay O⁺(Q) = SO(Q) (dùng Bài tập 3 e) của § 10 và Bài tập 17 a) của § 6).

10) Cho A là một trường có thứ tự cực đại, E là một không gian vectơ hữu hạn chiều trên A, Q là một dạng toàn phương dương không suy biến trên E. Với mọi biến đổi trực giao u ∈ O(Q), chứng minh rằng tồn tại một phân tích của E thành tổng trực tiếp của các không gian con trực giao từng đôi một P, N, R_i (1 ≤ i ≤ r) có các tính chất sau: 1° u(x) = x trong P, u(x) = −x trong N ; 2° mỗi R_i có chiều 2, ta có u(R_i) = R_i và hạn chế của u trên R_i là một phép quay qua một góc θ_i, phân biệt với 0 và với góc phẳng. Hơn nữa, đối với hai phân tích có dạng này, các không gian con P và N là như nhau, cũng như dãy các phần tử cos θ_i, sai khác không kể thứ tự (xem § 7, No. 3, Hệ quả 2 của Định lý 2). Suy ra rằng mọi phép quay u ∈ O⁺(Q) đều là một giao hoán tử tst⁻¹s⁻¹, trong đó s và t thuộc O(Q) và s² = 1 (xem Bài tập 3 d)).

11) Cho A là một trường có thứ tự cực đại, L là trường quaternion trên A (đối với cặp (−1, −1)), E là không gian con (có chiều 3) của L gồm các quaternion thuần (§ 9, Bài tập 15 a)) ; do đó mọi quaternion được viết theo một và chỉ một cách dưới dạng s = α . 1 + v, trong đó α ∈ A và v ∈ E ; ta có α² − v² = ρ . 1, trong đó ρ ∈ A và ρ ≥ 0 ; đặt \|v\| = \sqrt{\rho}.

a) Cho φ(s) là phép quay x → sx s⁻¹ trong E, đối với dạng toàn phương dương không suy biến x → \|x\|^2 trên E (§ 9, No. 5, Định lý 4 và Bài tập 15). Chứng minh rằng nếu v ≠ 0, các vectơ của đường thẳng D ⊂ E chứa v là bất biến dưới φ(s) ; hạn chế của φ(s) trên mặt phẳng trực giao P = D⁰ là một phép quay qua một góc θ sao cho (với một định hướng thích hợp của P) ta có tg \frac{\theta}{2} = \|v\|/α. (Nếu (1, i, j, k) là cơ sở chính tắc của L trên A, rút gọn về trường hợp v = βi, β ∈ A, rồi tính sjs⁻¹).

b) Chứng minh rằng mọi quaternion chuẩn 1 có thể được viết thành tst⁻¹s⁻¹, trong đó s ∈ L, t ∈ E (xem Bài tập 10), và rằng, nếu a, b là hai quaternion thuần chuẩn 1, thì tồn tại một quaternion s sao cho b = sas⁻¹.

c) Để hai quaternion s = α + v, t = β + w, trong đó α, β thuộc A, v, w thuộc E, giao hoán với nhau, điều kiện cần và đủ là v = λw, λ ∈ A ; để st = −ts, điều kiện cần và đủ là α = β = 0 và các vectơ v và w trong E trực giao (xem § 3, Bài tập 10).

12) Cho A là một trường có thứ tự cực đại, L là một không gian Euclid chiều n trên A, có dạng metric Φ là dương không suy biến ; gọi d(x, y) là khoảng cách \sqrt{\Phi(x - y, x - y)} của hai điểm của L (§ 7, No. 1, Nhận xét). Với mọi điểm c ∈ L và mọi phần tử ρ > 0 của A, tập hợp các x ∈ L sao cho d(x, c) = ρ được gọi là mặt cầu có tâm c và bán kính ρ ; do đó các mặt cầu là các toàn phương afin không suy biến trong L, có một tâm (§ 6, Bài tập 25).

a) Chứng minh rằng tại mọi điểm x của một mặt cầu S có tâm c, siêu phẳng tiếp xúc với S tại x (§ 6, Bài tập 25) vuông góc (§ 6, Bài tập 22) với đường thẳng đi qua c và x.

b) Cho S là một mặt cầu có tâm c và bán kính ρ, a là một điểm của L, D là một đường thẳng đi qua a và cắt S tại hai điểm phân biệt x₁, x₂ (tương ứng, tiếp xúc với S tại một điểm x). Chứng minh rằng ta có

$$
\Phi(x_1 - a, x_2 - a) = (d(a, c))^2 - \rho^2 \quad (\text{resp. } (d(x, a))^2 = (d(a, c))^2 - \rho^2).
$$

Phần tử $(d(a, c))^2 - \rho^2$ của A được gọi là lũy thừa của a đối với S.

c) Cho S₁, S₂ là hai mặt cầu không có cùng tâm ; chứng minh rằng tập hợp các điểm của L có các lũy thừa đối với S₁ và S₂ bằng nhau là một siêu phẳng vuông góc với đường thẳng đi qua các tâm của hai mặt cầu, và chứa giao S₁ ∩ S₂ ; người ta nói rằng siêu phẳng này là siêu phẳng căn của S₁ và S₂.

d) Cho S₁, S₂ là hai mặt cầu có các tâm tương ứng c₁, c₂, và các bán kính tương ứng ρ₁, ρ₂. Chứng minh rằng các tính chất sau là tương đương :

α) Giao S₁ ∩ S₂ không rỗng và, với mọi điểm của giao này, các siêu phẳng tiếp xúc với S₁ và S₂ tại điểm này vuông góc.

$\beta_1$ Lũy thừa của c₁ đối với S₂ là $\rho_1^2$.

$\beta_2$ Lũy thừa của c₂ đối với S₁ là $\rho_2^2$.

$\gamma_1$ Siêu phẳng căn của S₁ và S₂ là siêu phẳng cực (§ 6, Bài tập 25) của c₁ đối với S₂.

$\gamma_2$ Siêu phẳng căn của S₁ và S₂ là siêu phẳng cực của c₂ đối với S₁.

Khi các tính chất này được thỏa mãn, người ta nói rằng các mặt cầu S₁, S₂ trực giao.

e) Cho S₁, S₂ là hai mặt cầu trực giao, $c_1, c_2$ là các tâm của chúng. Chứng minh rằng nếu $\varpi_1, \varpi_2$ là các lũy thừa của một điểm x đối với S₁, S₂ tương ứng, thì ta có $\varpi_1 + \varpi_2 = 2\Phi(x - c_1, x - c_2)$. Đảo lại.

13) Các giả thiết và các ký hiệu là như trong Bài tập 12. Cho một điểm c ∈ L và một phần tử $\alpha \neq 0$ của A, phép hoán vị đối hợp u của tập hợp $L - \{ c \}$ sao cho, với mọi $x \in L - \{ c \}$, $u(x)$ thuộc đường thẳng đi qua c và x và thỏa mãn quan hệ $\Phi(x - c, u(x) - c) = \alpha$ được gọi là phép nghịch đảo có cực c và lũy thừa $\alpha$. Do lạm dụng ngôn ngữ, người ta nói rằng u là một phép nghịch đảo trong L.

a) Nếu u, v là hai phép nghịch đảo có cùng cực c và có các lũy thừa $\alpha, \beta$, $uv^{-1}$ là hạn chế của phép vị tự (Chương II, lần xuất bản thứ 2, Phụ lục II, Bài tập 6) có tâm c và tỉ số $\alpha \beta^{-1}$ trên $L - \{ c \}$.

b) Cho S là một mặt cầu (Bài tập 12) chứa c. Chứng minh rằng ảnh của $S - \{ c \}$ qua một phép nghịch đảo có cực c là một siêu phẳng vuông góc với đường thẳng nối c với tâm của S (do lạm dụng ngôn ngữ, siêu phẳng này được gọi là ảnh của S qua phép nghịch đảo đang xét). Đảo lại.

c) Cho S là một mặt cầu không chứa c. Chứng minh rằng, nếu $\varpi$ là lũy thừa của c đối với S (Bài tập 12 b)), ảnh của S qua một phép nghịch đảo có cực c và lũy thừa $\alpha$ là ảnh của S qua một phép vị tự có tâm c và tỉ số $\alpha / \varpi$. Nếu $n = 2$ và nếu, với mọi $x \in S$, T (tương ứng. T’) biểu thị tiếp tuyến của S (tương ứng. $u(S)$) tại điểm x (tương ứng. $u(x)$), D là đường thẳng đi qua c, x và $u(x)$, chứng minh rằng ta có $(\widehat{D, T}) = (\widehat{T', D})$.

d) Cho $S_1, S_2$ là hai mặt cầu trực giao (Bài tập 12 d)), $S'_1, S'_2$ là các ảnh của chúng qua một phép nghịch đảo có cực $c$. Nếu $c$ không thuộc $S_1$ hoặc $S_2$, chứng minh rằng $S'_1$ và $S'_2$ là các mặt cầu trực giao. Nếu $c \in S_1$ và $c \notin S_2$, $S'_1$ là một siêu phẳng chứa tâm của $S'_2$. Nếu $c \in S_1 \cap S_2$, $S'_1$ và $S'_2$ là các siêu phẳng vuông góc (§ 6, Bài tập 22). Các đảo lại.

e) Cho $u$ là một phép nghịch đảo có cực $c$ và lũy thừa $\alpha = \rho^2 > 0$ và C là mặt cầu có tâm c và bán kính $\rho$. Nếu $x_1, x_2$ là hai điểm phân biệt nằm trên một đường thẳng đi qua c, và phân biệt với c, các tính chất sau là tương đương: $\alpha )$ $x_1$ và $x_2$ được biến đổi thành nhau bởi $u ; \beta )$ $x_1$ và $x_2$ là liên hợp đối với $C$ (§ 6, Bài tập 25); $\gamma )$ mọi mặt cầu chứa $x_1$ và $x_2$ đều trực giao với $C$. Người ta cũng nói rằng $u$ là phép nghịch đảo của mặt cầu $C$.

¶ 14) Các giả thiết và ký hiệu giống như trong Bài tập 12, chọn một gốc 0 trong L. Cho $E_1$ là tổng trực tiếp của không gian vectơ L và một không gian $Af_1$ có chiều 1; ký hiệu $Q_1$ là dạng toàn phương trên $E_1$ sao cho với $x \in L$ và $\eta \in A$, ta có

$$
Q_1(x + \eta f_1) = Q(x) + \eta^2,
$$

một dạng dương và không suy biến; ký hiệu $C$ là mặt cầu có tâm 0 và bán kính 1 trong $E_1$ (đối với $Q_1$).

Trong không gian Euclid $E_1$, cho $s$ là phép nghịch đảo có cực $-f_1$ và lũy thừa 2 (Bài tập 13); hạn chế của nó $s_0$ trên L biến L thành $C - \{ -f_1 \}$; $s_0$ (tương ứng $s_0^{-1}$) được gọi, do một sự lạm dụng ngôn ngữ, là phép chiếu lập thể của L lên C (tương ứng của C lên L) từ điểm nhìn $-f_1$. Với mỗi phép nghịch đảo $u$ trong L, có cực $c$, $s_0 us_0^{-1}$ là một phép hoán vị đối hợp của phần bù trong C của tập hợp $\{ s_0(c), -f_1 \}$; phép này được mở rộng thành một phép hoán vị đối hợp $u'$ của C bằng cách đặt $u'(s_0(c)) = -f_1,\ u'(-f_1) = s_0(c)$, và người ta nói rằng $u'$ là một phép nghịch đảo trong C. Tương tự, với mỗi phép đối xứng $\nu$ trong L đối với một siêu phẳng, $s_0 \nu s_0^{-1}$ là một phép hoán vị đối hợp của phần bù trong C của tập hợp $\{ -f_1 \}$; phép này được mở rộng thành một phép hoán vị đối hợp $\nu'$ của C bằng cách đặt $\nu'(-f_1) = -f_1$ và người ta nói rằng $\nu'$ là một phép đối xứng trong C. Nhóm các phép hoán vị của C sinh bởi các phép nghịch đảo và các phép đối xứng được gọi là nhóm bảo giác của C (hoặc của L, do một sự lạm dụng ngôn ngữ).

a) Bây giờ chứng minh rằng nhóm bảo giác của C được sinh bởi các phép đối xứng $\nu'$ và các phép nghịch đảo $u'$ tương ứng với các phép nghịch đảo $u$ trong L có lũy thừa $> 0$. (Dùng Bài tập 13 a) và nhận xét rằng trong L mọi phép tịnh tiến, cũng như phép vị tự $x \to -x$, là một tích của các phép đối xứng đối với các siêu phẳng).

b) Cho $u$ là một phép nghịch đảo trong L có lũy thừa $> 0$; bây giờ chứng minh rằng phép nghịch đảo tương ứng $u'$ trong C là hạn chế trên C của một biến đổi $u'_1$ được xác định duy nhất, biến đổi này hoặc là một phép nghịch đảo có lũy thừa $> 0$ trong $E_1$, mà mặt cầu của nó (Bài tập 13 e)) vuông góc với C, hoặc là một phép đối xứng đối với một siêu phẳng của $E_1$ đi qua 0 (xét trong $E_1$ phép nghịch đảo $u_1$ có cùng cực và cùng lũy thừa với $u$). Phát biểu mệnh đề tương ứng cho phép đối xứng $\nu'$ trong C tương ứng với một phép đối xứng $\nu$ trong L đối với một siêu phẳng.

c) Trong không gian vectơ $E_2 = A \times E_1$, xét dạng toàn phương $Q_2$ sao cho, với $\zeta \in A, y \in E_1$, ta có
$$
Q_2((\zeta, y)) = \zeta^2 - Q_1(y),
$$
một dạng không suy biến và có chỉ số dấu $(1, n + 1)$. Đồng nhất $E_1$ với ảnh chính tắc của nó trong không gian xạ ảnh $\mathbf{P}(E_2)$ (Chương II, ấn bản thứ 2, Phụ lục III, No. 4). Bây giờ chứng minh (với các ký hiệu của $b$) rằng $u'$ cũng là hạn chế xuống $C$ của một ánh xạ tuyến tính xạ ảnh $\bar{u}''$ nhận được bằng cách chuyển qua các thương từ một biến đổi $u''$ của nhóm trực giao $O(Q_2)$, là một phép đối xứng đối với một siêu phẳng không đẳng hướng trong $E_2$. Phát biểu mệnh đề tương ứng cho $\varphi'$. Suy ra rằng nhóm bảo giác của $L$ là đẳng cấu với thương của nhóm $O(Q_2)$ bởi tâm của nó (sử dụng mệnh đề 5 và Bài tập 17 c) của § 6). Kết luận từ đó rằng mọi biến đổi của nhóm bảo giác là một tích của nhiều nhất $n + 2$ biến đổi là các phép nghịch đảo hoặc các phép đối xứng trong $L$ (xem § 6, Bài tập 15 e)).

$d$ ) Cho $\Sigma$ là tập hợp mà các phần tử của nó là các mặt cầu và các siêu phẳng trong không gian afin $L$. Suy ra từ $b$ rằng tồn tại một song ánh của $\Sigma$ lên phần bù, trong $\mathbf{P}(E_2)$, của tập hợp các $x \in E_1$ sao cho $Q_1(x) \leqslant 1$, sao cho hai mặt cầu trực giao tương ứng với hai điểm liên hợp đối với $C$.

15) Tổng quát hóa các định nghĩa và các kết quả của các Bài tập 12 đến 14 cho trường hợp $A$ là một trường Pythagore và tồn tại một cơ sở trực chuẩn cho $\Phi$.

16) Cho $A$ là một trường giao hoán, $V$ là một không gian vectơ trên $A$ có chiều lẻ $2r + 1$, $F$ là không gian tích $A \times V$, $\Psi'$ là một dạng phản xứng không suy biến trên $F$; trong không gian xạ ảnh $\mathbf{P}(F)$, có chiều $2r + 1$, người ta nói rằng tập hợp $C_0$ gồm các đường thẳng là các ảnh chính tắc của các mặt phẳng hoàn toàn đẳng hướng của $F$ (đối với $\Psi'$) là phức tuyến tính (xạ ảnh) liên kết với $\Psi'$.

Giả sử trong phần sau $A$ là cực đại được sắp thứ tự; cho $\Phi$ là một dạng đối xứng không suy biến dương trên $V$. Gọi $D$ là trực giao phải của $V$ (đối với $\Psi'$) trong $F$, được chứa trong $V$, và gọi $H$ là siêu phẳng trực giao với $D$ (đối với $\Phi$) trong $V$; trong $F$, $H$ là một không gian con không đẳng hướng đối với $\Psi'$, mà trực giao của nó đối với $\Psi'$ do đó là một mặt phẳng phụ thuộc bổ sung với $H$ và chứa $D$. Trong không gian affine $E = \{1\} \times V \subset F$, tập hợp $C$ các giao tuyến với $E$ của các mặt phẳng đẳng hướng toàn phần của $F$ (đối với $\Psi'$) không được chứa trong $V$ lại được gọi là phức tuyến tính (affine) liên kết với $\Psi'$; đường phải $\Delta = P \cap E$ được gọi là trục của phức tuyến tính $C$ (đối với cấu trúc không gian Euclid xác định trên $E$ bởi dạng metric $\Phi$).

a) Bây giờ chứng minh rằng, trong $E$, mọi phép tịnh tiến bằng với một vectơ phương của $\Delta$ (Chương II, 2nd ed., Phụ lục II, No. 3) bảo toàn $C$ (xem § 4, Bài tập 6).

b) Cho $(e_i)_{0 \leq i \leq 2r}$ là một cơ sở trực chuẩn của $V$ đối với $\Phi$, sao cho $e_0 \in D$ và $\Psi'(e_{2i-1}, e_{2i}) = \rho_i > 0$ với $1 \leq i \leq r$, $\Psi'(e_j, e_k) = 0$ đối với các cặp chỉ số không có dạng $(e_{2i-1}, e_{2i})$ hoặc $(e_{2i}, e_{2i-1})$ (§ 7, No. 3, Mệnh đề 6). Lấy trong không gian afin E một gốc $a \in \Delta$, và đặt $\Psi(a, e_0) = \rho_0$. Cho $x$ là một vectơ thuộc mặt phẳng sinh bởi $e_{2i-1}$ và $e_{2i}$, và cho $y$ là vectơ của cùng mặt phẳng này sao cho $\Phi(x, y) = 0$, $\Phi(y, y) = 1$ và $x \wedge y = \lambda e_{2i-1} \wedge e_{2i}$ với $\lambda > 0$. Gọi $E_i$ là đa tạp tuyến tính afin 3 chiều sinh bởi các điểm $a, a + e_0, a + e_{2i-1}, a + e_{2i}$ trong E, và gọi $R_x$ là giao của $E_i$ và siêu phẳng afin (trong E) sinh bởi các đường thẳng của C chứa điểm $a + x$. Chứng minh rằng phương của các đường thẳng vuông góc (đối với $\Phi$) với mặt phẳng $R_x$ trong $E_i$ là một đường thẳng $L_x$ trong mặt phẳng $Ae_0 + Ay$, sao cho nếu $\theta = (\widehat{D}, \widehat{L_x})$, thì ta có

$$
\operatorname{tg} \theta = \frac{\rho_i}{\rho_0} \sqrt{\Phi(x, x)}
$$

khi mặt phẳng $Ae_0 + Ay$ được định hướng sao cho $e_0 \wedge y$ là dương.

¶ 17) a) Cho A là một trường giao hoán, $J : \xi \to \overline{\xi}$ là một tự đẳng cấu đối hợp của A, E là một không gian vectơ 2 chiều trên A, $\Phi$ là một dạng Hermit sesquilinear không suy biến (không phản xứng) trên E, $(e_1, e_2)$ là một cơ sở trực giao của E đối với $\Phi$ (§ 6, No. 1, Định lý 1), sao cho

$$
\Phi(\xi_1 e_1 + \xi_2 e_2, \eta_1 e_1 + \eta_2 e_2) = \alpha \xi_1 \overline{\eta_1} + \beta \xi_2 \overline{\eta_2}
$$

$(\alpha$ và $\beta$ thuộc trường K gồm các bất biến của J); đặt $\gamma = \beta / \alpha$. Đồng nhất điểm $\xi_1 e_1 + \xi_2 e_2 \in E$ với phần tử $\xi_1 + \xi_2 \rho$ của vành B được xác định bởi các điều kiện $\rho^2 = -\gamma$, $\rho \xi = \overline{\xi} \rho$ với $\xi \in A$ (§ 3, Bài tập 4 a)). Với mọi $x = \xi_1 + \xi_2 \rho \in B$, đặt $\tilde{x} = \overline{\xi_1} - \xi_2 \rho$ và $N(x) = x \tilde{x} = \tilde{x} x$, sao cho $x \to \tilde{x}$ là một phản tự đẳng cấu đối hợp của đại số B (trên K) và ta có $\Phi(x, x) = \alpha N(x)$. Chứng minh rằng mọi phép đồng dạng đối với $\Phi$ có định thức bằng nhân tử (còn gọi là phép đồng dạng trực tiếp) có thể được viết theo một và chỉ một cách $x \to xy$, trong đó $y$ là một vectơ không đẳng hướng của E, và nhân tử của nó là $N(y)$.

b) Trước hết giả sử rằng J là đồng nhất, do đó $K = A$. Nếu A có đặc số $\neq 2$, hãy khôi phục các kết quả của No. 1. Hãy phát triển lý thuyết tương ứng khi A có đặc số 2 (xem § 4, Bài tập 14; ta sẽ phân biệt hai trường hợp, tùy theo $\gamma$ có hay không là một bình phương trong A).

c) Giả sử $J \neq 1$, sao cho A là một mở rộng bậc hai tách được của K. Khi đó $\Phi$ nhất thiết thỏa mãn điều kiện (T) (§ 4, No. 2 và Bài tập 1); nếu $\Phi$ có chỉ số 0, B là một trường phản xạ có tâm K (Chương VIII, § 11, Bài tập 4), và nếu $\Phi$ có chỉ số 1, B đẳng cấu với $\mathbf{M}_2(K)$.

d) Giả sử $J \neq 1$ và A có đặc số $\neq 2$; khi đó $A = K(\theta)$ với $\theta^2 = -\delta \in K$. Nếu S là nhóm các phép tương tự trực tiếp đối với $\Phi$, H là nhóm các phép vị tự trong E, với tỉ số $\neq 0$ và thuộc K (một nhóm đẳng cấu với $K^*$), bây giờ chứng minh rằng nhóm S/H đẳng cấu với nhóm các phép quay $O^+(Q)$, trong đó Q là một dạng toàn phương không suy biến trên một không gian vectơ F có chiều 3 trên K, sao cho tồn tại một cơ sở trực giao $(f_1, f_2, f_3)$ của F mà đối với nó ta có

$$
Q(\zeta_1 f_1 + \zeta_2 f_2 + \zeta_3 f_3) = \gamma \zeta_1^2 + \delta \zeta_2^2 + \gamma \delta \zeta_3^2
$$

(xem § 9, Bài tập 15).

¶ 18) a) Cho $A$ là một trường giao hoán, $\xi \to \bar{\xi}$ là một tự đẳng cấu đối hợp của $A$, $E$ là một không gian vectơ có chiều chẵn $2m$ trên $A$, $\Phi$ là một dạng Hermit không suy biến có chỉ số 0 trên $E$, thỏa mãn điều kiện (T), $\Delta$ là biệt thức của $\Phi$ đối với một cơ sở của $E$. Cho $M(\Phi)$ là nhóm các nhân tử của các phép tương tự đối với $\Phi$ ($§ 4$, Bài tập 8). Bây giờ chứng minh rằng $M(\Phi)$ là một nhóm con của nhóm nhân của các phần tử của $A$ có dạng $\alpha \bar{\alpha} - (-1)^m \beta \bar{\beta} \Delta$. (Lập luận bằng quy nạp theo $m$, sử dụng Bài tập 17, cùng với hai nhận xét sau: 1° nếu $u$ là một phép tương tự với nhân tử $\mu$, $x$ là một vectơ của $E$, $y = u(x)$ và $z = u(y)$, tồn tại một phép biến đổi unita $v$ sao cho $v(y) = y$ và $v(z) = \mu x$; 2° nếu $\alpha, \beta, \lambda$ là ba phần tử $\neq 0$ của $A$ sao cho tồn tại $a, b, c, d$ trong $A$ thỏa mãn các điều kiện $\lambda = a \bar{a} + \alpha c \bar{c}$, $\lambda = b \bar{b} + \beta d \bar{d}$, thì tồn tại $s, t$ trong $A$ thỏa mãn điều kiện $\lambda = s \bar{s} - \alpha \beta t \bar{t}$.

b) Cho $K$ là một trường có thứ tự cực đại, $K_1 = K((t_1))$ là trường các chuỗi lũy thừa hình thức theo một bất định $t_1$, với các hệ số trong $K$ (Chương IV, $§ 5$, No. 7), $A = K_1((t_2))$ là trường các chuỗi lũy thừa hình thức theo một bất định thứ hai $t_2$, với các hệ số trong $K_1$. Cho $E$ là một không gian vectơ có chiều 6 trên $A$, $Q$ là một dạng toàn phương không suy biến trên $E$, sao cho tồn tại một cơ sở trực giao $(e_i)$ mà đối với nó ta có

$$
Q\left( \sum_{i=1}^{6} \xi_i e_i \right) = \xi_1^2 + \xi_2^2 + \xi_3^2 + \xi_4^2 + t_1 \xi_5^2 + t_2 \xi_6^2.
$$

Chứng minh rằng không tồn tại một phép đồng dạng của $Q$ với nhân tử $t_1 t_2$.
