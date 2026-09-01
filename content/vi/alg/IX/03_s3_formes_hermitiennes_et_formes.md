---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 3
section_title: Formes hermitiennes et formes quadratiques
lang: vi
source: alg-ix-fr
pdf_pages: 0047-0061
extraction: ocr
subsections:
    - "no": 1
      title: Formes hermitiennes et $\varepsilon$-hermitiennes.
      page: 0
      pdf_page: 47
    - "no": 2
      title: '*Modules sur une extension quadratique*.'
      page: 0
      pdf_page: 49
    - "no": 3
      title: Formes bilinéaires associées à une forme hermitienne.
      page: 0
      pdf_page: 50
    - "no": 4
      title: Formes quadratiques.
      page: 0
      pdf_page: 52
statements: 7
exercises: 0
content_sha256: cc25ccc3eabfcbf9ee0aaf83548b2b5e3c7e97d23614b59502d61733fbf6d7d4
translated_from: content/en-mt/alg/IX/03_s3_formes_hermitiennes_et_formes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: d377fe8e8b62ddb12247032d22e12f921fdb53e65ce67e7cd126d8fc7cc7a270
translation_model: gpt-5-mini, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-be0708bf
glossary_version: 34
glossary_terms_sha256: 766691716632bf8a0b471b5342bacb4f3ab2aef1fa23e7075154346dd1078693
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. Các dạng Hermit và các dạng toàn phương

Trong tất cả những gì tiếp theo trong Chương này, trừ khi được phát biểu rõ ràng ngược lại, $A$ ký hiệu một vành và $E$ một $A$-môđun trái. Ta giả sử rằng $A$ được trang bị một phản tự đẳng cấu đối hợp $J$, ký hiệu $\alpha \to \overline{\alpha}$; do đó ta có $(\alpha + \beta) = \overline{\alpha} + \overline{\beta}$, $(\alpha \beta) = \overline{\beta} \cdot \overline{\alpha}$ và $\overline{\alpha} = \alpha$ với mọi $\alpha, \beta$ trong A. Trừ khi được phát biểu rõ ràng ngược lại, các dạng nửa song tuyến tính được xét là nửa song tuyến tính phải (§ 1, No. 2, đn. 4) đối với phản tự đẳng cấu này.

### 1. Các dạng Hermit và các dạng $\varepsilon$-Hermit.

#### Định nghĩa 1 {#alg-ix-s3-def-1 .statement}

Cho $\varepsilon$ là một phần tử của tâm của A. Một dạng nửa song tuyến tính $\Phi$ trên E sao cho có $\Phi(x, y) = \varepsilon \overline{\Phi(y, x)}$ với mọi $x$ và $y$ trong E được gọi là một dạng $\varepsilon$-Hermit. Một dạng 1-Hermit (tương ứng, (−1)-Hermit) được gọi là Hermit (tương ứng, phản Hermit).

Khi J là đồng nhất (điều này kéo theo rằng A là giao hoán), một dạng Hermit (tương ứng, dạng phản Hermit) (đối với J) không gì khác hơn là một dạng song tuyến tính đối xứng (tương ứng, phản đối xứng) (Chương III, § 5, No. 1, đn. 2). Nhắc lại rằng một dạng song tuyến tính phản xứng (Chương III, § 5, No. 2, đn. 4) là phản đối xứng; đảo lại đúng nếu, trong A, quan hệ $2a = 0$ kéo theo $a = 0$.

Quan hệ trực giao ($§ 1, n° 3$) đối với một dạng $\varepsilon$-Hermit hiển nhiên là đối xứng (cf. bài tập 1).

Nếu $\alpha$ là một phần tử khả nghịch của A, ánh xạ $T : \lambda \to \alpha^{-1} \overline{\lambda} \alpha$ là một phản tự đẳng cấu của A, và người ta dễ dàng kiểm chứng rằng dạng $\Phi \alpha$ là nửa song tuyến tính đối với T. Nếu hơn nữa có $\alpha = \overline{\alpha}$, thì T là đối hợp, và, nếu $\Phi$ là $\varepsilon$-Hermit, $\Phi \alpha$ cũng vậy; thật vậy ta có
$$
(\lambda^T)^T = \alpha^{-1} (\overline{\alpha^{-1} \lambda \alpha}) \alpha = \alpha^{-1} \overline{\alpha} \lambda \overline{\alpha^{-1}} \alpha = \lambda
$$
$$
\Phi(y, x) \alpha = \varepsilon \overline{\Phi(x, y)} \alpha = \varepsilon (\Phi(x, y) \alpha)^T.
$$

Đặc biệt, khi A là một trường, các phần tử $\alpha$ của tâm của A sao cho $\overline{\alpha} = \alpha$ tạo thành một trường con K của A, và các dạng $\varepsilon$-Hermit trên E (đối với J) tạo thành một không gian vectơ trên K.

#### Nhận xét 1 {#alg-ix-s3-n1-rem-1 .statement}

Nếu $\Phi$ là một dạng $\varepsilon$-Hermit trên E, ta có $\Phi(x, y) = \varepsilon \overline{\Phi(x, y)} \overline{\varepsilon}$ với mọi $x, y$ trong E. Do đó, nếu $\Phi$ nhận các giá trị khả nghịch, ta có $\varepsilon \overline{\varepsilon} = 1$.
2) Nếu tồn tại một phần tử khả nghịch $i$ của tâm của A sao cho $\overline{i} = i \varepsilon$, thì, để $\Phi$ là $\varepsilon$-Hermit, điều kiện cần và đủ là $i \Phi$ là Hermit.

Ánh xạ $(y, x) \to \overline{\Phi(x, y)}$ là dạng nửa tuyến tính đối với J, để $\Phi$ là $\varepsilon$-Hermit, điều kiện cần và đủ là có $\Phi(y, x) = \varepsilon \overline{\Phi(x, y)}$ khi $x$ và $y$ chạy qua một hệ sinh của E. Đặc biệt, nếu E thừa nhận một cơ sở hữu hạn $(e_i)_{1 \leq i \leq n}$, để một dạng nửa tuyến tính $\Phi$ trên E là $\varepsilon$-Hermit, điều kiện cần và đủ là ma trận của nó $R = (\rho_{ij}) = (\Phi(e_i, e_j))$ thỏa mãn các hệ thức $\rho_{ji} = \varepsilon \overline{\rho_{ij}}$ với mọi $i, j$, tức là $'R = \varepsilon \overline{R}$ ; một ma trận $R$ có tính chất này được gọi là $\varepsilon$-Hermit. Khi $\varepsilon = 1$ (resp. $-1$) người ta nói rằng $R$ là Hermit (resp. phản Hermit) đối với phản tự đồng cấu J. Khi J là đồng nhất (do đó A giao hoán), một ma trận Hermit (resp. phản Hermit) $R$ là sao cho $'R = R$ (resp. $'R = -R$) ; khi đó người ta nói rằng $R$ là một ma trận đối xứng (resp. phản đối xứng). Để $\Phi$ là một dạng phản xứng, điều kiện cần và đủ là ma trận của nó phản đối xứng và, ngoài ra, các phần tử đường chéo của $R$ đều bằng không; một ma trận có các tính chất này được gọi là phản xứng.

Cho $\Phi$ là một dạng nửa tuyến tính trên $E$, và cho $s_\Phi$ và $d_\Phi$ là các ánh xạ của $E$ vào $E^*$ liên kết với $\Phi$ ở bên trái và bên phải ($§ 1$, n° 6). Để $\Phi$ là $\varepsilon$-Hermit, điều kiện cần và đủ là $\langle x, s_\Phi(y) \rangle = \bar{\varepsilon} \langle x, d_\Phi(y) \rangle$ với mọi phần tử $x, y$ của $E$, do đó $s_\Phi = \bar{\varepsilon} d_\Phi$, hoặc tương đương là $\langle x, d_\Phi(y) \rangle = \varepsilon \langle x, s_\Phi(y) \rangle$, do đó $d_\Phi = \varepsilon s_\Phi$.

Cho $\Phi$ là một dạng $\varepsilon$-Hermit sao cho ánh xạ $d_\Phi$ của $E$ vào $E^*$ liên kết ở bên phải với $\Phi$ là song ánh. Với mọi tự đồng cấu $u$ của $E$ ta có
$$
u^{**} = \varepsilon \bar{\varepsilon} u.
$$
Thật vậy, với mọi phần tử $x$ và $y$ của $E$, ta có
$$
\begin{align*}
\Phi(x, u^{**(y)}) &= \Phi(u^*(x), y) = \varepsilon \overline{\Phi(y, u^*(x))} = \varepsilon \overline{\Phi(u(y), x)} \\
&= \varepsilon \Phi(x, u(y)) \bar{\varepsilon} = \Phi(x, \varepsilon \bar{\varepsilon} u(y))
\end{align*}
$$
do đó $u^{**(x)} = \varepsilon \bar{\varepsilon} u(x)$ vì $\Phi$ không suy biến.

Nếu $\Phi$ là một dạng $\varepsilon$-hermit thì các ánh xạ $s_\Phi$ và $d_\Phi$ là song ánh, khi đó *dạng nghịch đảo* $\widehat{\Phi}$ của $\Phi$ ($§ 1$, No. 7) *là một dạng* $\bar{\varepsilon}$-hermit. Thật vậy, đặt $s = s_\Phi$, $d = d_\Phi$ để viết gọn, từ $d = \varepsilon s$ ta suy ra $s^{-1} = \bar{\varepsilon} d^{-1}$, do $s$ là nửa tuyến tính. Do đó, với mọi $u, v$ trong $E$, ta có
$$
\widehat{\Phi}(u, v) = \Phi(s^{-1}(u), d^{-1}(v)) = \bar{\varepsilon} \Phi(d^{-1}(u), d^{-1}(v)),
$$
suy ra
$$
\widehat{\Phi}(v, u) = \bar{\varepsilon} \varepsilon \overline{\Phi(d^{-1}(u), d^{-1}(v))} = \bar{\varepsilon} \overline{\widehat{\Phi}(u, v)},
$$
vì $\varepsilon$ nằm trong tâm của $A$.

Cuối cùng, khi vành $A$ là giao hoán, các mở rộng chính tắc của một dạng $\varepsilon$-hermit $\Phi$ lên các lũy thừa tenxơ và ngoài $\bigotimes^p E$ và $\wedge^p E$ của $E$ là các dạng $\varepsilon^p$-hermit, như suy ra ngay từ các công thức (35) và (37) của $§ 1$, No. 9.

### 2. *Các môđun trên một mở rộng bậc hai*.

Cho $K$ là một vành giao hoán. Ta lấy $A$ là mở rộng bậc hai $A = K(i)$ với $i^2 = -1$, và $J$ là tự đẳng cấu λ + iμ → λ − iμ ($\lambda \in K, \mu \in K$) (chương II, § 7, No. 7). Nếu E là một A-môđun, ta ký hiệu $E_0$ là K-môđun suy ra từ E bởi hạn chế vành các vô hướng, và ký hiệu j là tự đẳng cấu $x \to ix$ của $E_0$; hiển nhiên ta có $j^2 = -I$, trong đó I là ánh xạ đồng nhất của $E_0$. Ngược lại, cho $E_0$ là một K-môđun và j là một tự đẳng cấu của $E_0$ sao cho $j^2 = -I$; ánh xạ $\lambda + i\mu \to \lambda I + \mu j$ hiển nhiên là một đồng cấu của A vào vành $\mathcal{L}(E_0)$ các tự đồng cấu của $E_0$; do đó ta đã xác định trên $E_0$ một cấu trúc A-môđun, mà với cấu trúc đó ta có

(2) $$(\lambda + i\mu)x = \lambda x + \mu j(x)$$ $(x \in E_0, \lambda \in K, \mu \in K).$

Nếu $E'$ là một A-môđun khác, $E'_0$ là K-môđun nền của $E'$, $j'$ là tự đẳng cấu $x' \to ix'$ của $E'_0$, thì các ánh xạ A-tuyến tính f từ E vào $E'$ không gì khác ngoài các ánh xạ K-tuyến tính từ $E_0$ vào $E'_0$ sao cho $f \circ j = j' \circ f$. Đặc biệt, nếu ta ký hiệu bởi $E^*$ và $(E_0)^*$ các đối ngẫu tương ứng của E và $E_0$, và nếu $f_1$ và $f_2$ là hai ánh xạ từ E vào K, để ánh xạ $x \to f_1(x) + if_2(x)$ từ E vào A là A-tuyến tính, điều kiện cần và đủ là $f_1$ và $f_2$ thuộc $(E_0)^*$ và ta có $f_1 \circ j + i(f_2 \circ j) = if_1 - f_2$, tức là $f_1 = f_2 \circ j$ và $f_1 \circ j = -f_2$. Vì j là một tự đẳng cấu của $E_0$ và vì $j^2 = -I$, hai điều kiện này là tương đương. Khử $f_1$ hoặc $f_2$, ta thấy rằng các công thức

(3) $$f(x) = f_1(x) - if_1(j(x))$$
(4) $$f(x) = f_2(j(x)) + if_2(x)$$

$(x \in E,\ f \in E^*,\ f_1 \in (E_0)^*,\ f_2 \in (E_0)^*)$ thiết lập hai tương ứng một-một giữa $E^*$ và $(E_0)^*$.

### 3. Các dạng song tuyến tính liên kết với một dạng Hermit.

Ta lại giả sử ở đây rằng vành A là mở rộng bậc hai $A = K(i)$ (trong đó $i^2 = -1$) của một vành giao hoán K, và J là tự đẳng cấu $\lambda + i\mu \to \lambda - i\mu$ của A ($\lambda \in K, \mu \in K$). Cho E và $E'$ là hai A-môđun, $E_0$ và $E'_0$ là các K-môđun nền của E và $E'$, j và $j'$ là các tự đẳng cấu $x \to ix$ và $x' \to ix'$ của E và $E'$ (xem n° 2). Một dạng K-song tuyến tính $f$ trên $E_0 \times E'_0$ được gọi là *bất biến dưới j và $j'$* nếu có

(5) $$f(j(x), j'(x')) = f(x, x')$$

với $x \in E_0$ và $x' \in E'_0$. Thay thế x bởi $j(x)$, ta thấy rằng điều kiện này tương đương với

$$
f(x, j'(x')) = - f(j(x), x')
$$

với mọi $x \in E_0$ và $x' \in E'_0$.

#### Mệnh đề 1 {#alg-ix-s3-prop-1 .statement}

Cho $\Phi_1$ (resp. $\Phi_2$) là một dạng song tuyến tính trên K trên $E_0 \times E'_0$, bất biến dưới $j$ và $j'$. Ánh xạ gán cho $\Phi_1$ (resp. $\Phi_2$) ánh xạ $\Phi$ từ $E \times E'$ vào $A$ được xác định bởi

$$
\Phi(x, x') = \Phi_1(x, x') + i \Phi_1(x, j'(x'))
$$
(resp. $\Phi(x, x') = - \Phi_2(x, j'(x')) + i \Phi_2(x, x')$)

$(x \in E, x' \in E)$, là một đẳng cấu từ không gian vectơ trên K của các dạng song tuyến tính trên $E_0 \times E'_0$ bất biến dưới $j$ và $j'$ lên không gian vectơ trên K của các dạng sesqui tuyến tính trên $E \times E'$. Giả sử thêm rằng $E = E'$; để $\Phi$ là Hermit, điều kiện cần và đủ là $\Phi_1$ đối xứng (resp. $\Phi_2$ phản đối xứng) (cf. Bài tập 4).

Thật vậy, mọi ánh xạ $\Phi$ từ $E \times E'$ vào $A$ đều có thể được viết, theo một và chỉ một cách, dưới dạng $\Phi = \Phi_1 + i \Phi_2$, trong đó $\Phi_1$ và $\Phi_2$ là các ánh xạ từ $E \times E'$ vào $K$. Để ánh xạ bộ phận $x \to \Phi(x, x')$ là A-tuyến tính, điều kiện cần và đủ, theo công thức (3) (resp. (4)) của No. 2, là $\Phi_1$ (resp. $\Phi_2$) K-tuyến tính theo $x$ và ta có

$$
\Phi(x, x') = \Phi_1(x, x') - i \Phi_1(j(x), x')
$$
(resp. $\Phi(x, x') = \Phi_2(j(x), x') + i \Phi_2(x, x')$).

Tương tự, để $\overline{\Phi}(x, x')$ là A-tuyến tính theo $x'$, điều kiện cần và đủ là $\Phi_1$ (resp. $\Phi_2$) K-tuyến tính theo $x'$ và ta có

$$
\Phi(x, x') = \Phi_1(x, x') + i \Phi_1(x, j'(x'))
$$
(resp. $\Phi(x, x') = - \Phi_2(x, j'(x')) + i \Phi_2(x, x')$).

Suy ra ngay lập tức rằng, để $\Phi$ là sesqui tuyến tính, điều kiện cần và đủ là nó được viết dưới một trong các dạng (9) và (11) (resp. (10) và (12)) với $\Phi_1$ (resp. $\Phi_2$) là một dạng song tuyến tính trên K bất biến dưới $j$ và $j'$.

Từ đó suy ra rằng, để một dạng sesqui tuyến tính $\Phi = \Phi_1 + i \Phi_2$ là không, điều kiện cần và đủ là $\Phi_1$ (resp. $\Phi_2$) là không. Bây giờ, nếu $E = E'$, ta có $\Phi(y, x) = \Phi_1(y, x) + i \Phi_2(y, x)$ và $\overline{\Phi(x, y)} = \Phi_1(x, y) - i \Phi_2(x, y)$; để hai biểu thức này bằng nhau, nói cách khác để $\Phi$ là Hermit, do đó điều kiện cần và đủ là $\Phi_1$ đối xứng (resp. $\Phi_2$ phản đối xứng).

#### Nhận xét 1 {#alg-ix-s3-n3-rem-1 .statement}

Các công thức (7) và (8) chỉ ra rằng, nếu $x \in E$, để $\Phi(x, x') = 0$ với mọi $x' \in E'$, điều kiện cần và đủ là $\Phi_1(x, x') = 0$ (resp. $\Phi_2(x, x') = 0$) với mọi $x' \in E'$.
2) Liên hợp của một tự đồng cấu $u$ của $E$ đối với $\Phi$ ($§ 1$, n° 8) cũng chính là liên hợp của $u$ (được xem như một tự đồng cấu của $E_0$) đối với $\Phi_1$ (resp. $\Phi_2$).

### 4. Các dạng toàn phương.

#### Định nghĩa 2 {#alg-ix-s3-def-2 .statement}

Ta giả sử rằng vành $A$ là giao hoán. Ta nói rằng một ánh xạ $Q$ từ $E$ vào $A$ là một dạng toàn phương trên $E$ nếu
1) $Q(\alpha x) = \alpha^2 Q(x)$ với $\alpha \in A$ và $x \in E$;
2) ánh xạ $\Phi : (x, y) \to Q(x + y) - Q(x) - Q(y)$ từ $E \times E$ vào $A$ là một dạng song tuyến tính.
Dạng song tuyến tính $\Phi$ (vốn nhất thiết đối xứng) được gọi là dạng song tuyến tính liên kết với $Q$. Nếu $\Phi$ không suy biến, ta nói rằng $Q$ không suy biến.

Vì $Q(2x) = 4Q(x)$, suy ra ngay từ 2) rằng
$$
\Phi(x, x) = 2Q(x).
$$
Đặc biệt, nếu $A$ là một vành có đặc số 2, dạng $\Phi$ là phản xứng.

Ta sẽ nói rằng hai phần tử (resp. hai tập con) của $E$ là trực giao đối với $Q$ nếu chúng trực giao đối với dạng song tuyến tính liên kết với $\Phi$.

Cho $(x_i)_{i \in I}$ là một họ các phần tử của $E$ và $(a_i)_{i \in I}$ là một họ các phần tử của $A$ mà tất cả trừ một số hữu hạn trong chúng là không. Theo quy nạp theo số các chỉ số $i$ mà $a_i \neq 0$, người ta dễ dàng chứng minh rằng
$$
Q(\sum_i a_i x_i) = \sum_i a_i^2 Q(x_i) + \sum_{\{i, j\}} a_i a_j \Phi(x_i, x_j),
$$

tổng cuối cùng được lấy trên các tập con hai phần tử của I.

Đối với mọi dạng song tuyến tính $f$ trên $E \times E$, ta định nghĩa một dạng toàn phương $Q$ bằng cách đặt $Q(x) = f(x, x)$; dạng song tuyến tính $\Phi$ liên kết với $Q$ khi đó được định nghĩa bởi $\Phi(x, y) = f(x, y) + f(y, x)$ đối với $x, y$ trong $E$. Hơn nữa, nếu giả sử rằng vô hướng 2 có một nghịch đảo $\frac{1}{2}$ trong $A$, tồn tại duy nhất một dạng song tuyến tính đối xứng $f$ sao cho $Q(x) = f(x, x)$, cụ thể là $f = \frac{1}{2} \Phi$; biệt thức của $f$ đối với một hệ $S = (x_1, \ldots, x_n)$ cũng được gọi là biệt thức của $Q$ đối với $S$. Do đó, trong trường hợp này có một sự tương ứng một-một giữa các dạng toàn phương và các dạng song tuyến tính đối xứng trên $E$ (xem bài tập 6).

Trong trường hợp của một môđun tự do, ta còn có thêm kết quả sau:

#### Mệnh đề 2 {#alg-ix-s3-prop-2 .statement}

Giả sử rằng $A$ là giao hoán và rằng $E$ nhận một cơ sở $(e_i)_{i \in I}$. Khi đó, đối với mọi dạng toàn phương $Q$ trên $E$, tồn tại một dạng song tuyến tính $f$ trên $E \times E$ sao cho $Q(x) = f(x, x)$ đối với mọi $x \in E$. Đối với mọi họ $(b_{ij})_{(i,j) \in I \times I}$ các vô hướng sao cho $b_{ij} = b_{ji}$ đối với $(i, j) \in I \times I$, tồn tại duy nhất một dạng toàn phương $Q$ sao cho

$$
Q(e_i) = b_{ii}, \quad \Phi(e_i, e_j) = b_{ij} \text{ cho } i \neq j,
$$

trong đó $\Phi$ chỉ dạng song tuyến tính liên kết với $Q$; khi đó $Q$ được cho bởi công thức

$$
Q(\sum_i a_i e_i) = \sum_{\{i,j\}} b_{ij} a_i a_j,
$$

phép tổng cuối cùng lấy trên các tập con $\{i, j\}$ của $I$ có một hoặc hai phần tử.

Thật vậy, vì công thức (16) chỉ là một phép chép lại công thức (14), tính duy nhất của một dạng toàn phương $Q$ thỏa mãn (15) được chứng minh. Để chứng minh sự tồn tại của nó, trước hết ta nhận xét rằng tồn tại một họ $(b'_{ij})$ các phần tử của $A$ sao cho $b'_{ii} = b_{ii}$ và $b'_{ij} + b'_{ji} = b_{ij}$ với $i \neq j$; chẳng hạn, ta thu được một họ như vậy bằng cách trang bị cho $I$ một cấu trúc tập hợp có thứ tự (*LÝ THUYẾT TẬP HỢP*, Chương III, § 2, No. 3, Định lý 1) và bằng cách đặt $b'_{ij} = b_{ij}$ với $i < j$ và $b'_{ij} = 0$ với $i > j$. Vì các $e_i$ tạo thành một cơ sở của $E$, tồn tại một dạng song tuyến tính $f$ trên $E \times E$ sao cho $f(e_i, e_j) = b'_{ij}$; bằng cách đặt $Q'(x) = f(x, x)$ và ký hiệu $\Phi'$ là dạng song tuyến tính liên kết với dạng toàn phương $Q'$, ta thu được $Q'(e_i) = b_{ii}$ và $\Phi'(e_i, e_j) = f(e_i, e_j) + f(e_j, e_i) = b_{ij}$. Điều này chứng minh mệnh đề thứ hai của chúng ta. Đối với mệnh đề thứ nhất, nó suy ra ngay lập tức, vì, theo tính duy nhất, nếu một dạng toàn phương $Q$ thỏa mãn (15), ta có $Q(x) = Q'(x) = f(x, x)$.

Môđun $E$ được trang bị cấu trúc xác định bởi một dạng toàn phương $Q$ được gọi là một *môđun toàn phương*. Một đồng cấu của môđun toàn phương $(E, Q)$ vào một môđun toàn phương $(E', Q')$ là một ánh xạ tuyến tính $u$ của $E$ vào $E'$ sao cho $Q = Q' \circ u$; nếu $\Phi$ và $\Phi'$ là các dạng song tuyến tính liên kết với $Q$ và $Q'$, khi đó ta có $\Phi(x, y) = \Phi'(u(x), u(y))$ với $x \in E,\ y \in E$; nói cách khác $\Phi'$ là ảnh ngược của $\Phi$ bởi $u$ (§ 1, No. 1). Ta nói rằng hai dạng toàn phương $Q$ và $Q'$ trên hai $A$-môđun $E$ và $E'$ là *tương đương* nếu các môđun toàn phương tương ứng là đẳng cấu.

Cho $(E_i, Q_i)_{i \in I}$ là một họ các môđun toàn phương, và cho $E$ là tổng trực tiếp của các môđun $E_i$. *Tổng trực tiếp ngoài* của các môđun toàn phương $(E_i, Q_i)$ là môđun toàn phương thu được bằng cách trang bị cho $E$ dạng toàn phương $Q$ được xác định bởi $Q(\sum_i x_i) = \sum_i Q_i(x_i)$ với $x_i \in E_i$. Người ta cũng nói rằng dạng toàn phương $Q$ là *tổng trực tiếp ngoài* của các dạng toàn phương $Q_i$.

Nếu các dạng $Q_i$ là không suy biến, thì điều tương tự cũng đúng đối với $Q$.

Cho $Q$ là một dạng toàn phương trên $A$-môđun $E$; nếu $F$ là một môđun con của $E$ và nếu $Q$ là hằng trên mỗi lớp modulo $F$, ánh xạ $\overline{Q}$ của $E/F$ vào $A$ suy ra từ $Q$ bằng cách chuyển qua thương là hiển nhiên một dạng toàn phương, và ánh xạ chính tắc của $E$ lên $E/F$ là một đồng cấu đối với các cấu trúc của các môđun toàn phương. Để $Q$ là hằng trên mỗi lớp modulo $F$, điều kiện cần và đủ là ta có $Q(x + y) = Q(x)$ với $x \in E$ và $y \in F$, nghĩa là, ký hiệu dạng song tuyến tính liên kết với $Q$ là $\Phi$, ta có $Q(y) + \Phi(x, y) = 0$ với $y \in F$ và $x \in E$. Lấy $x = 0$, ta thấy rằng ta có $Q(y) = 0$ với $y \in F$, và do đó

$\Phi(x, y) = 0$ với $x \in E$ và $y \in F$. Nói cách khác, nếu ta gọi hạt nhân của môđun toàn phương $(E, Q)$ là tập hợp $N$ các phần tử $x$ của $E$ sao cho $Q(x) = 0$ và $\Phi(x, z) = 0$ với mọi $z \in E$, để $Q$ là hằng trên mỗi lớp modulo $F$, điều kiện cần và đủ là $F$ được chứa trong hạt nhân $N$ của $(E, Q)$. Ta kiểm tra ngay được rằng $N$ là một môđun con của $E$. Do đó, để $Q$ là hằng trên mỗi lớp modulo $F$, điều kiện cần và đủ là $F$ được sinh bởi các phần tử của $N$.

Ta thấy ngay lập tức rằng hạt nhân của môđun toàn phương $|E/N$ là $\{0\}$.

#### Mệnh đề 3 {#alg-ix-s3-prop-3 .statement}

*Cho $h$ là một đồng cấu của $A$ vào một vành giao hoán $A'$. Đối với mỗi dạng toàn phương $Q$ trên $A$-môđun $E$, tồn tại duy nhất một dạng toàn phương $Q'$ trên $A'$-môđun $A' \otimes_A E$ (chương III, ấn bản thứ 2, Phụ lục II, No. 10) sao cho ta có*
$$
Q'(1 \otimes x) = h(Q(x))
$$
với mọi $x \in E$. *Ngoài ra dạng song tuyến tính $\Phi'$ liên kết với $Q'$ thu được bằng phép mở rộng vành các vô hướng từ dạng song tuyến tính $\Phi$ liên kết với $Q$.*

Trước hết ta chứng minh rằng, nếu tồn tại một dạng toàn phương $Q'$ thỏa mãn (17), thì nó là duy nhất và dạng song tuyến tính $\Phi'$ liên kết với $Q'$ thu được bằng phép mở rộng vành các vô hướng từ dạng $\Phi$ liên kết với $Q$. Thật vậy khẳng định cuối cùng này suy ra từ việc ta có
$$
\Phi'(1 \otimes x, 1 \otimes y) = Q'(1 \otimes x + 1 \otimes y) - Q'(1 \otimes x) - Q'(1 \otimes y)
= h(\Phi(x, y))
$$
với $x \in E, y \in E$. Công thức (14) khi đó cho thấy ta có
$$
Q'(\sum_i a'_i \otimes x_i) = \sum_i a'_i{}^2 h(Q(x_i)) + \sum_{\{i, j\}} a'_i a'_j h(\Phi(x_i, x_j))
$$
với $a'_i \in A'$ và $x_i \in E$, điều này chứng minh tính duy nhất của $Q'$.

Để chứng minh sự tồn tại của $Q'$, trước hết ta giả sử rằng môđun $E$ có một cơ sở $(e_i)_{i \in I}$. Khi đó tồn tại các phần tử $b_{ij}$ của $A$ sao cho $b_{ij} = b_{ji}$ và sao cho $Q(\sum_i a_i e_i) = \sum_{\{i, j\}} b_{ij} a_i a_j$ với $a_i \in A$ (mđề 2). Vì các phần tử $1 \otimes_A e_i$ tạo thành một cơ sở của

A'-môđun $A' \otimes_A E$, ta định nghĩa một dạng toàn phương $Q'$ trên môđun sau cùng này bằng cách đặt
$$
Q'(\sum_i a'_i \otimes e_i) = \sum_{\{i,j\}} a'_i a'_j h(b_{ij})
$$
với $a'_i \in A'$; do đó, với $x = \sum_i a_i e_i \in E$
$$
Q'(1 \otimes x) = Q'(\sum_i h(a_i) \otimes e_i) = \sum_{\{i,j\}} h(a_i) h(a_j) h(b_{ij}) = h(Q(x)),
$$
điều này chứng minh sự tồn tại của $Q'$ trong trường hợp này.

Bây giờ ta chuyển sang trường hợp tổng quát. Cho $(x_i)_{i \in I}$ là một hệ phần tử sinh của $E$, $A^{(t)}$ là môđun các tổ hợp tuyến tính hình thức của các phần tử của $I$ (Ch. II, § 1, No. 8), và $(e_i)_{i \in I}$ là cơ sở chính tắc của $A^{(t)}$. Ánh xạ tuyến tính $u$ từ $A^{(t)}$ vào $E$ xác định bởi $u(e_i) = x_i$ là toàn ánh vì các phần tử $x_i$ sinh $E$. Suy ra (Ch. III, ấn bản lần 2, Phụ lục II, No. 5, Mệnh đề 4) rằng ánh xạ $1 \otimes u$ từ $A' \otimes A^{(t)}$ vào $A' \otimes E$ là toàn ánh, và hạt nhân $P'$ của nó được sinh bởi các phần tử có dạng $1 \otimes p$ với $u(p) = 0$. Khi đó, gọi $Q'_1$ là mở rộng lên $A' \otimes_A A^{(t)}$ của dạng toàn phương $Q_1 = Q \circ u$ trên $A^{(t)}$. Nếu $p$ là một phần tử của $A^{(t)}$ sao cho $u(p) = 0$, ta có $Q'_1(1 \otimes p) = h(Q_1(p)) = 0$ và (ký hiệu $\Phi'_1$ là dạng song tuyến tính liên kết với $Q'_1$) $\Phi'_1(1 \otimes p, 1 \otimes x) = h(\Phi(u(p), u(x))) = 0$ với mọi $x \in A^{(t)}$. Do đó, nếu $u(p) = 0$ ($p \in A^{(t)}$), thì $1 \otimes p$ thuộc hạt nhân của môđun toàn phương $A' \otimes_A A^{(t)}$, và tồn tại do đó, như ta đã thấy ở trên, một dạng toàn phương $Q'$ trên $A' \otimes_A E$ sao cho $Q'_1 = Q' \circ (1 \otimes u)$. Vì $u$ là toàn ánh, ta thấy rằng $Q'$ thỏa mãn điều kiện (17). Q.E.D.

Dạng toàn phương $Q'$, mà sự tồn tại và tính duy nhất của nó được bảo đảm bởi Mệnh đề 3, được gọi là mở rộng của $Q$ lên $A' \otimes_A E$ (đối với $h$). Người ta cũng nói rằng $Q'$ thu được từ $Q$ bằng mở rộng vành các vô hướng.

Bài tập. — 1) Cho $A$ là một trường, $E$ là một không gian vectơ trái trên $A$, $\Phi$ là một dạng sesquilinear trên $E$ (đối với một phản tự đồng cấu $J$ của $A$). Giả sử rằng hạng (hữu hạn hoặc vô hạn) của $\Phi$ là $\geqslant 2$, và các quan hệ $\Phi(x, y) = 0$ và $\Phi(y, x) = 0$ là tương đương.
a) Bây giờ chứng minh rằng tồn tại $\lambda \neq 0$ trong $A$ sao cho có $\Phi(y, x) = \lambda (\Phi(x, y))^J$. (Dùng bài tập 8 của § 1).
b) Bây giờ chứng minh rằng tồn tại $\alpha \in A$ sao cho dạng sesquilinear $\Phi \alpha$ (đối với phản tự đồng cấu $\xi \to \alpha^{-1} \xi^J \alpha$) là Hermit hoặc phản xứng.

(Trước hết chú ý rằng có $\xi^{J^2} = \lambda^{-1} \xi \lambda^{-J}$ và $\lambda \lambda^J = \lambda^J \lambda = 1$. Sau đó phân biệt hai trường hợp tùy theo $\xi + \xi^J \lambda^{-1} = 0$ với mọi $\xi \in A$ hay không; trong trường hợp thứ hai, chứng minh rằng mọi phần tử $\neq 0$ có dạng $\alpha = \xi + \xi^J \lambda^{-1}$ đều trả lời câu hỏi).

2) Cho $\Phi$ là một dạng sesquilinear $\varepsilon$-Hermit trên một không gian vectơ hữu hạn chiều $E$ trên một trường $A$.

a) Bây giờ chứng minh rằng với mọi không gian con vectơ $M$ của $E$, ta có $(M^0)^0 = M + E^0$ và $\dim M^0 + \dim M = \dim E + \dim (M \cap E^0)$.

b) Nếu $M_1, M_2$ là hai không gian con vectơ của $E$, bây giờ chứng minh rằng có $\dim (M_1 \cap M_2^0) + \dim (M_2 + M_1^0) = \dim E + \dim (M_1 \cap E^0)$ (xét ánh xạ chính tắc của $E$ lên $E/E^0$).

3) Cho $K$ là một vành giao hoán, $f$ là một đa thức đơn khởi của $K[X]$, có bậc $n \geqslant 1$; cho $A$ là đại số thương $K[X]/(f)$ nhận làm cơ sở trên $K$ các phần tử $1, \xi, \xi^2, \ldots, \xi^{n-1}$ (chương IV, § 1, số 5, mệnh đề 4). Bây giờ chứng minh rằng dữ kiện của một $A$-môđun $E$ tương đương với dữ kiện của một $K$-môđun $E_0$ và của một $K$-tự đồng cấu $j$ của $E_0$ sao cho $f(j) = 0$. Với mọi $u \in E^*$, đặt $u(x) = \sum_{k=0}^{n-1} u_k(x) \xi^k$; chứng minh rằng nếu $\alpha_0 = f(0)$ là khả nghịch trong $K$, ánh xạ $u \to u_0$ là một $K$-đẳng cấu của $E^*$ lên $(E_0)^*$, mà đẳng cấu nghịch đảo của nó cần được viết tường minh.

¶ 4) a) Cho $A$ là một vành (giao hoán hoặc không), $\sigma$ là một tự đẳng cấu của $A$ sao cho tồn tại một phần tử khả nghịch $\gamma \in A$ thỏa mãn $\gamma^\sigma = \gamma$, và sao cho $\xi^{\sigma^2} = \gamma \xi \gamma^{-1}$ với mọi $\xi \in A$. Cho $B$ là một A-môđun trái có một cơ sở gồm hai phần tử $(e_1, e_2)$; bây giờ chứng minh rằng một cấu trúc vành được xác định trên $B$ bằng cách lấy làm phép nhân trong $B$ luật hợp thành

$$
(\xi e_1 + \eta e_2)(\xi' e_1 + \eta' e_2) = (\xi \xi' + \eta \eta' \gamma) e_1 + (\eta {\xi'}^\sigma + \xi \eta') e_2.
$$

Đối với cấu trúc vành này, $e_1$ là phần tử đơn vị (mà ta đồng nhất với phần tử đơn vị 1 của $A$); nếu đặt $e_2 = \rho$, ta có $\rho^2 = \gamma$ và $\rho \xi = \xi^\sigma \rho$ với mọi $\xi \in A$; hơn nữa, $B$ là một A-môđun phải, trong đó 1 và $\rho$ tạo thành một cơ sở. Nếu $A$ là một trường, một điều kiện cần và đủ để $B$ là một trường là $\gamma$ không có dạng $\lambda^\sigma \lambda$ (trong đó $\lambda \in A$). (Xem Chương VIII, § 12, bài tập 8).

b) Cho $J$ là một phản tự đẳng cấu đối hợp của $A$. Giả sử tồn tại một phần tử khả nghịch $\delta \in A$ thỏa mãn các điều kiện sau:

(1) $\delta^J = \delta, \quad \delta^\sigma \delta = \gamma \gamma^J, \quad (\xi^J)^\sigma = \delta (\xi^\sigma)^J \delta^{-1}$ với mọi $\xi \in A$.

Bây giờ chứng minh rằng $J$ có thể được mở rộng thành một phản tự đẳng cấu đối hợp của $B$ (vẫn ký hiệu là $J$) bằng cách đặt

(2) $$ (\xi + \eta \rho)^J = \xi^J + \gamma^{-1} \delta^\sigma (\eta^J)^\sigma \rho. $$

Nếu hơn nữa, $A$ và $B$ là các trường và nếu $\sigma$ không phải là một tự đẳng cấu trong, bây giờ chứng minh rằng các điều kiện (1) là cần thiết cho sự tồn tại của một mở rộng của $J$ thành một phản tự đẳng cấu đối hợp của $B$ (đặt $\rho^J = \alpha + \beta \rho$, với $\alpha, \beta$ trong $A$, bây giờ chứng minh rằng nhất thiết $\alpha = 0$, bằng cách viết điều kiện $(\rho \xi)^J = \xi^J \rho^J$ với mọi $\xi \in A$).

c) Giả sử các điều kiện (1) được thỏa mãn và phản tự đẳng cấu đối hợp $J$ được mở rộng tới $B$ bởi (2). Cho $F$ là một B-môđun đơn vị, $E$ là A-môđun đơn vị suy ra từ $F$ bằng hạn chế về $A$ của vành các vô hướng; ánh xạ $j : x \to \rho x$ khi đó là một ánh xạ nửa tuyến tính song ánh của $E$ lên chính nó, tương ứng với tự đẳng cấu $\sigma$ của $A$ và sao cho $j^2(x) = \gamma x$. Cho $\Phi$ là một dạng Hermit trên $F$ (đối với $J$); với $x \in E$, $y \in E$, đặt $\Phi(x, y) = \Phi_1(x, y) + \Phi_2(x, y)\rho$, trong đó $\Phi_1(x, y) \in A$, $\Phi_2(x, y) \in A$. Bây giờ chứng minh rằng $\Phi_1$ là một dạng Hermit trên $E$ (đối với $J$), sao cho
$$
\Phi_1(j(x), j(y)) = (\Phi_1(x, y))^{\sigma \delta};
$$
ta có $\Phi_2(x, y) = \Phi_1(x, j(y))\delta^{-1}$, $\Phi_2$ là một dạng nửa song tuyến tính trên $E$ đối với phản tự đẳng cấu (nói chung không đối hợp) $\xi \to (\xi^J)^{\sigma}$, sao cho
$$
\Phi_2(j(x), j(y)) = (\Phi_2(x, y))^{\sigma \delta^{\sigma}}
$$
và
$$
\Phi_2(y, x) = \gamma^J \delta^{-1}((\Phi_2(x, y))^J)^{\sigma}.
$$

Ngược lại. Để $\Phi$ không suy biến, điều kiện cần và đủ là $\Phi_1$ hoặc $\Phi_2$ không suy biến. Trường hợp đặc biệt khi $B$ là một đại số quaternion trên một vành giao hoán $K$, tương ứng với một cặp $(\alpha, \beta)$ các phần tử của $K$, $\beta$ khả nghịch, $A$ là đại số con $K + Ku$ của $B$, và $J$ và $\sigma$ là ánh xạ $\xi \to \bar{\xi}$ (chương II, § 7, số 8).

d) Cho $u$ là một tự đẳng cấu của A-môđun $E$. Để $u$ là một tự đẳng cấu của B-môđun $F$, giữ bất biến dạng $\Phi$, điều kiện cần và đủ là $u$ thỏa mãn hai bất kỳ trong ba điều kiện sau:
1° $u$ giữ bất biến $\Phi_1$;
2° $u$ giữ bất biến $\Phi_2$;
3° $u$ giao hoán với $j$.

5) Cho $A$ là một vành giao hoán, $E$ là một $A$-môđun, $(x_i)_{i \in I}$ là một hệ sinh của $E$; cho $R$ là môđun con của môđun $A^{(1)}$ tạo bởi các phần tử $(y_i)_{i \in I}$ sao cho $\sum_i y_i x_i = 0$, và cho $(a_{\lambda})_{\lambda \in L}$ là một hệ sinh của $R$ (với $a_{\lambda} = (a_{\lambda i})_{i \in I}$). Cho $(b_{ij})$ là một họ các phần tử của $A$ $(i \in I, j \in I)$. Để tồn tại một dạng toàn phương $Q$ sao cho $Q(x_i) = b_{ii}$ và $\Phi(x_i, x_j) = b_{ij}$ với $i \neq j$ ($\Phi$ ký hiệu dạng song tuyến tính liên kết với $Q$), điều kiện cần và đủ là $b_{ij} = b_{ji}$ với mọi $i, j$ trong $I$, và với mọi $\lambda \in L$ và $i \in I$, ta có
$$
\sum_{\{i, j\}} b_{ij} a_{\lambda i} a_{\lambda j} = \sum_{j \neq i} b_{ij} a_{\lambda j} + 2b_{ii} a_{\lambda i} = 0;
$$
khi đó ta có $Q(\sum a_i x_i) = \sum_{\{i, j\}} b_{ij} a_i a_j$. Suy ra một chứng minh mới của Mệnh đề 3 của No. 4. (Chú ý rằng $x'_i = 1 \otimes x_i$ tạo thành một hệ sinh của $A' \otimes_A E$, và rằng A-môđun $A' \otimes_A E$ là đẳng cấu với ${A'}^{(1)}/R'$, trong đó ${A'}^{(1)}$ được đồng nhất với $A' \otimes_A A^{(1)}$ và $R'$ được sinh bởi ảnh của R qua ánh xạ chính tắc của $A^{(1)}$ vào ${A'}^{(1)}$.

6) Cho $A$ là một vành giao hoán có đặc số 2, $E$ là một A-môđun tự do, $\mathcal{A}$ (tương ứng $\mathcal{S}$, $\mathcal{Q}$) là A-môđun của các dạng song tuyến tính phản xứng (tương ứng các dạng song tuyến tính đối xứng, các dạng toàn phương) trên $E$. Ta có $\mathcal{A} \subset \mathcal{S}$; ngoài ra ta định nghĩa một ánh xạ tuyến tính $\omega$ từ $\mathcal{S}$ vào $\mathcal{Q}$, và một ánh xạ tuyến tính $\theta$ từ $\mathcal{Q}$ vào $\mathcal{A}$ như sau: với mọi dạng song tuyến tính $\Phi \in \mathcal{S}$, $\omega(\Phi)$ là dạng toàn phương $x \to \Phi(x, x)$, và với mọi dạng toàn phương $Q \in \mathcal{Q}$, $\theta(Q)$ là dạng song tuyến tính liên kết với $Q$, dạng này là phản xứng. Chứng minh rằng $\omega(0) = \mathcal{A}$, $\theta(\mathcal{Q}) = \mathcal{A}$ và $\theta(0) = \omega(\mathcal{S})$.

¶ 7) Cho $A$ là một vành giao hoán, $E, F$ là hai A-môđun. Một ánh xạ $Q$ từ $E$ vào $F$ được gọi là *toàn phương* nếu nó thỏa mãn các điều kiện sau: $1^\circ$ $Q(\alpha x) = \alpha^2 Q(x)$ với $\alpha \in A, x \in E$; $2^\circ$ ánh xạ $(x, y) \to Q(x + y) - Q(x) - Q(y)$ từ $E \times E$ vào $F$ là song tuyến tính. Nếu $f$ là một ánh xạ tuyến tính từ một A-môđun $E_1$ vào $E$, thì $Q \circ f$ là một ánh xạ toàn phương từ $E_1$ vào $F$.

a) Cho $E$ là một $A$-môđun, $A^{(E)}$ là môđun của các tổ hợp tuyến tính hình thức của các phần tử của $E$ với các hệ số trong $A$ (chương II, § 1, số 8), và với mọi $x \in E$, cho $\varepsilon_x$ là phần tử tương ứng của cơ sở chính tắc của $A^{(E)}$. Cho $\Gamma^2(E)$ là thương của $A^{(E)} \times (E \otimes_A E)$ theo môđun con $R$ sinh bởi các phần tử $(\varepsilon_{x+y} - \varepsilon_x - \varepsilon_y, -x \otimes y)$ và $(\varepsilon_{\lambda x} - \lambda^2 \varepsilon_x, 0)$, với $x \in E, y \in E, \lambda \in A$. Với mọi $x \in E$, đặt $\gamma(x) = \varphi(\varepsilon_x, 0)$, trong đó $\varphi$ là ánh xạ chính tắc của $A^{(E)} \times (E \otimes E)$ lên $\Gamma^2(E)$; $\gamma$ được gọi là *ánh xạ chính tắc* của $E$ vào $\Gamma^2(E)$. Chứng minh rằng $\gamma$ là một ánh xạ bậc hai của $E$ vào $\Gamma^2(E)$ và rằng, với mọi ánh xạ bậc hai $Q$ của $E$ vào một $A$-môđun $F$, tồn tại một và chỉ một *ánh xạ tuyến tính* $q$ của $\Gamma^2(E)$ vào $F$ sao cho $Q = q \circ \gamma$ (nói cách khác, $(\Gamma^2(E), \gamma)$ là một nghiệm của một bài toán ánh xạ phổ quát; xem *Ens.*, chương IV, § 3).

Với mọi cặp $A$-môđun $E, E'$ và mọi ánh xạ tuyến tính $f$ của $E$ vào $E'$, bây giờ chứng minh rằng, nếu $\gamma'$ là ánh xạ chính tắc của $E'$ vào $\Gamma^2(E')$, thì tồn tại một và chỉ một ánh xạ tuyến tính $\bar{f}$ của $\Gamma^2(E)$ vào $\Gamma^2(E')$ sao cho $\gamma' \circ f = \bar{f} \circ \gamma$.

b) Giả sử rằng $E$ là tổng trực tiếp của hai môđun con $M, N$. Định nghĩa một đẳng cấu chính tắc của $\Gamma^2(E)$ lên tổng trực tiếp của các môđun $\Gamma^2(M), \Gamma^2(N)$ và $M \otimes N$ (chứng minh rằng tổng trực tiếp này là nghiệm của cùng một bài toán ánh xạ phổ quát như $\Gamma^2(E)$).

c) Cho $F$ là một môđun con của $E$, $j$ là đơn ánh chính tắc của $F$ vào $E$. Định nghĩa một đẳng cấu chính tắc của $\Gamma^2(E/F)$ lên

$$
\Gamma^2(E)/(\bar{j}(\Gamma^2(F)) + \psi(E \times F)),
$$

where $\psi(x, y) = \varphi(0, x \otimes j(y))$ đối với $x \in E, y \in F$. (Cùng phương pháp).

d) Cho $A'$ là một vành giao hoán, $h$ là một đồng cấu của $A$ vào $A'$. Định nghĩa một đẳng cấu chính tắc của $\Gamma^2(A' \otimes_A E)$ lên $A' \otimes_A \Gamma^2(E)$ (cùng phương pháp).

e) Tồn tại duy nhất một ánh xạ tuyến tính $s$ của $\Gamma^2(E)$ vào $E \otimes E$ sao cho $s(\gamma(x)) = x \otimes x$ với mọi $x \in E$; hãy chứng minh rằng nếu $E$ là một môđun tự do, thì s là một đẳng cấu lên môđun con của các tenxơ đối xứng cấp 2 trên E.

f) Giả sử rằng $A = \mathbf{Z}$ và E là một nhóm xyclic hữu hạn cấp n. Hãy chứng minh rằng $\Gamma^2(E)$ là một nhóm xyclic cấp n nếu n là lẻ, cấp $2n$ nếu n là chẵn. (Trước hết nhận xét rằng nếu a là một phần tử sinh của E, $\gamma(a)$ là một phần tử sinh của $\Gamma^2(E)$, và rằng $\gamma(-ha) = \gamma(ha)$ với mọi số nguyên h; suy ra từ đó rằng nếu n là lẻ, $n\gamma(a) = 0$ bằng cách lấy $h = (n-1)/2$; chứng minh tương tự rằng $2n\gamma(a) = 0$ nếu n là chẵn. Cuối cùng chứng minh rằng nếu n là lẻ (tương ứng chẵn), tồn tại một ánh xạ bậc hai Q của E vào một nhóm xyclic cấp n (tương ứng $2n$) áp dụng a vào một phần tử sinh của nhóm này).

8) Cho A là một trường giao hoán, E, F là hai không gian vectơ trên A. Cho g là một ánh xạ của E vào F, sao cho tồn tại ba ánh xạ $a, b, c$ của $E \times E$ vào F, thỏa mãn đồng nhất thức

$$
g(\lambda x + \mu y) = \lambda^2 a(x, y) + \lambda \mu b(x, y) + \mu^2 c(x, y)
$$

với mọi $x, y$ trong E, $\lambda, \mu$ trong A.

a) Chứng minh rằng ta có $a(x, y) = g(x), c(x, y) = g(y), b(y, x) = b(x, y)$ và $b(\lambda x, y) = \lambda b(x, y)$; hơn nữa, nếu đặt

$$
d(x, y, z) = b(x + y, z) - b(x, z) - b(y, z)
$$

chứng minh rằng ta có $d(x, y, z) = d(y, z, x) = d(z, x, y)$ và kết luận rằng $d(\lambda x, \mu y, v z) = \lambda \mu v d(x, y, z)$.

b) Suy ra từ a) rằng nếu $A \neq \mathbf{F}_2$, nhất thiết có $d(x, y, z) = 0$ và do đó g là một ánh xạ bậc hai (Bài tập 7). Ngược lại, nếu $A = \mathbf{F}_2$ và nếu dim E $\geqslant 3$, hãy chứng minh rằng tồn tại các ánh xạ g của E vào A, thỏa mãn (4) và sao cho $d(x, y, z)$ không đồng nhất bằng không.

9) Cho A là một vành giao hoán, E là một A-môđun có một cơ sở gồm n phần tử, $\Phi$ là một dạng song tuyến tính đối xứng trên E. Cho e là một phần tử của $\bigwedge^n E$ tạo thành một cơ sở của môđun này, $\Delta$ là biệt thức của $\Phi$ đối với e, $\varphi_p$ là đẳng cấu chính tắc của $\bigwedge^p E$ lên $\bigwedge^{n-p} E^*$ tương đối với e (Chương III, § 8, No. 5). Với $x \in \bigwedge^p E$, đặt $d_{(p)}(x) = \varphi_{n-p}^{-1}(d_{\Phi_{(p)}}(x))$; hãy chứng minh rằng ánh xạ $d_{(p)}$ của $\bigwedge^p E$ vào $\bigwedge^{n-p} E$ có các tính chất sau:

a) Với mọi $x \in \bigwedge^p E$, $d_{(n-p)}(d_{(p)}(x)) = (-1)^{p(n-p)} \Delta x$.

b) Với mọi cặp phần tử $x, y$ của $\bigwedge^p E$, ta có

$$
x \wedge d_{(p)}(y) = \Phi_{(p)}(x, y)e \quad \text{and} \quad \Phi_{(n-p)}(d_{(p)}(x), d_{(p)}(y)) = \Delta \Phi_{(p)}(x, y).
$$

c) Giả sử thêm rằng A là một trường và rằng $\Phi$ không suy biến. Khi đó, nếu x là một p-vectơ phân tích được $\neq 0$ tương ứng với một không gian con F của E (Chương III, § 7, No. 3), $d_{(p)}(x)$ là một $(n-p)$-vectơ phân tích được $\neq 0$ tương ứng với không gian con $F^0$ trực giao với F.

d) Mở rộng các kết quả trước cho trường hợp trong đó (A là một vành giao hoán), Φ là một dạng ε-Hermit nửa tuyến tính liên kết đối với một tự đẳng cấu đối hợp J ≠ 1 của A.

10) a) Cho A là một vành giao hoán, E là một A-môđun có một cơ sở gồm 3 phần tử, Φ là một dạng song tuyến tính đối xứng trên E. Với ký hiệu của Bài tập 9, đối với hai phần tử tùy ý x, y của E, đặt $x \overline{\wedge} y = d_{(2)}(x \wedge y)$, và nói rằng phần tử này là tích vectơ của x và y (đối với $\Phi$ và đối với cơ sở e của $\bigwedge^3 E$). Chứng minh rằng $(x, y) \to x \overline{\wedge} y$ là một ánh xạ song tuyến tính phản xứng của $E \times E$ vào E, và rằng $x \overline{\wedge} y$ trực giao với x và với y.

b) Cho α, β là hai phần tử khả nghịch của A, B là đại số quaternion trên A tương ứng với cặp ($α, β$) (Chương II, § 7, No. 8), 1, u, v, ω là cơ sở chính tắc của B trên A; cho E là môđun con của B có u, v, ω làm cơ sở. Chứng minh rằng nếu x, y là hai quaternion thuộc E, ta có
$$
xy = \Phi(x, y) + x \overline{\wedge} y
$$
trong đó Φ là một dạng song tuyến tính đối xứng trên E, sao cho các ánh xạ tuyến tính liên kết với Φ là song ánh, và $x \overline{\wedge} y$ là tích vectơ của x và y đối với dạng Φ và đối với cơ sở $α^{-1}β^{-1}u \wedge v \wedge \omega$ của $\bigwedge^3 E$.

11) Cho Φ là một dạng ε-Hermit nửa tuyến tính liên kết không suy biến trên một không gian vectơ hữu hạn chiều E. Một không gian con vectơ M của E được gọi là trực giao yếu với một không gian con vectơ N (đối với Φ) nếu một trong hai không gian con M, N° chứa không gian kia.

a) Chứng minh rằng quan hệ "M trực giao yếu với N" là đối xứng.

b) Nếu M và N trực giao yếu, M° và N° trực giao yếu.

c) Nếu M và N trực giao yếu và nếu $M \cap N = \{0\}$, M và N trực giao.
