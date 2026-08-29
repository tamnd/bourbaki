---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 0
section_title: Alternative algebras. Octonions
appendix: true
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 611-617, 654
pdf_pages: 0635-0641, 0678-0678
extraction: ocr
subsections:
    - "no": 1
      title: ALTERNATIVE ALGEBRAS
      page: 611
      pdf_page: 635
    - "no": 2
      title: ALTERNATIVE CAYLEY ALGEBRAS
      page: 613
      pdf_page: 637
    - "no": 3
      title: OCTONIONS
      page: 615
      pdf_page: 639
statements: 11
exercises: 3
content_sha256: 597c6956b3012437b53b21a38d59a11c2bee3747d48268f9b9c1890e36b22570
translated_from: content/en/alg/III/A_a_alternative_algebras_octonions.md
source_content_sha256: 0651f3bed82b7df7a8e6ef9f2573f410b9f48cf8e11708f9e289377e24833536
translation_model: gpt-5.4
translation_run: translate-vi-19aaef7b
glossary_version: 34
glossary_terms_sha256: 091bf3569760f7015399b2b0dcb42c77fdd2f637c79d4f438a0881586836da5f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# ĐẠI SỐ THAY THẾ. OCTONION

### 1. ĐẠI SỐ THAY THẾ

Cho A là một vành giao hoán và F là một đại số trên A (không nhất thiết kết hợp). Với ba phần tử bất kỳ $x, y, z$ của F, ta viết

$$
a(x, y, z) = x(yz) - (xy)z
$$

(kết hợp tử của $x, y, z$); $a$ hiển nhiên là một ánh xạ A-tuyến tính theo ba biến từ $F \times F \times F$ vào $F$.

#### Bổ đề 1 {#alg-iii-a0-lem-1 .statement}

*Với mọi $p, q, r, s$ trong đại số $F$,*

$$
a(pq, r, s) - a(p, qr, s) + a(p, q, rs) = a(p, q, r)s + pa(q, r, s).
$$

Việc kiểm tra suy ra ngay lập tức từ định nghĩa (1).

#### Mệnh đề 1 {#alg-iii-a0-prop-1 .statement}

*Đối với một đại số trên A $F$, các điều kiện sau là tương đương:*
(a) *Với mọi cặp có thứ tự các phần tử $x, y$ của $F$, đại số con sinh bởi $x$ và $y$ là kết hợp.*
(b) *Ánh xạ tuyến tính theo ba biến $(x, y, z) \mapsto a(x, y, z)$ là phản xứng (§ 7, no. 3).*
(c) *Với mọi cặp có thứ tự các phần tử $x, y$ của $F$, $x^2y = x(xy)$ và $yx^2 = (yx)x$.*

Hiển nhiên (a) kéo theo (c). Ta chỉ ra rằng (c) kéo theo (b): theo định nghĩa (§ 7, no. 3), để chứng minh (b), chỉ cần kiểm tra rằng $a(x, x, y) = 0$ và $a(x, y, y) = 0$, điều này chính xác là (c).

Để chứng minh rằng (b) kéo theo (a), ta dùng 4 bổ đề sau:

#### Bổ đề 2 {#alg-iii-a0-lem-2 .statement}

*Cho $E$ là một đại số trên A sao cho ánh xạ tuyến tính theo ba biến $(x, y, z) \mapsto a(x, y, z)$ là phản xứng, $S$ là một hệ sinh của $E$ và $U$ là một môđun con trên A của $E$ chứa $S$ và sao cho $sU \subset U$ và $Us \subset U$ với mọi $s \in S$. Khi đó $U = E$.*

Tập hợp $U'$ các $x \in E$ sao cho $xU \subset U$ và $Ux \subset U$ hiển nhiên là một môđun con trên A của $E$, và theo giả thiết nó chứa $S$. Mặt khác, với $x, y$ trong $U'$ và $u \in U$, theo giả thiết

$$
(xy)u = x(yu) + a(x, y, u) = x(yu) - a(x, u, y) = x(yu) - (xu)y + x(uy) \in U;
$$

khi chuyển qua đại số đối, tương tự ta có $u(xy) \in U$. Vậy $U'$ là một đại số con của $E$ và, vì nó chứa $S$, nên $U' = E$. Do đó $EU \subset U$ và *a fortiori* $UU \subset U$, điều này chứng minh rằng $U$ là một đại số con của $E$; vì nó chứa $S$, nên $U = E$, điều này chứng minh bổ đề.

Một tập con $H$ của $F$ được gọi là *kết hợp mạnh* nếu $a(u, v, w) = 0$ khi *ít nhất hai* trong các phần tử $u, v, w$ thuộc $H$.

#### Bổ đề 3 {#alg-iii-a0-lem-3 .statement}

*Giả sử ánh xạ $a$ là phản xứng. Nếu $H$ là một tập con kết hợp mạnh của $F$, thì đại số con của $F$ sinh bởi $H$ là kết hợp mạnh.*

Vì tập hợp các tập con kết hợp mạnh của $F$ là quy nạp, nên chỉ cần chứng minh rằng nếu $H$ là một tập con kết hợp mạnh *cực đại* của $F$, thì khi đó $H$ là một *đại số con* của $F$. Vì $H$ hiển nhiên là một A-môđun con của $F$, nên chỉ cần kiểm tra rằng với mọi cặp phần tử $u, v$ của $H$, $H \cup \{uv\}$ cũng kết hợp mạnh, vì theo định nghĩa của $H$, điều này sẽ suy ra $uv \in H$. Bây giờ, với mọi $z \in H$ và mọi $t \in F$, theo (2)

$$
a(uv, t, z) - a(u, vt, z) + a(u, v, tz) = 0
$$

vì $\mathbf{H}$ kết hợp mạnh; mà do $u, v, z$ thuộc $\mathbf{H}$, cũng có
$$
a(u, vt, z) = a(u, v, tz) = 0,
$$
do đó $a(uv, t, z) = 0$. Dùng tính chất phản xứng của $a$, điều này cho thấy rằng $a(p, q, r) = 0$ mỗi khi ít nhất hai trong các phần tử $p, q, r$ thuộc $\mathbf{H} \cup \{uv\}$, do đó suy ra bổ đề.

#### Bổ đề 4 {#alg-iii-a0-lem-4 .statement}

*Giả sử ánh xạ $a$ là phản xứng. Khi đó, với mọi $x \in \mathbf{F}$, đại số con của $\mathbf{F}$ sinh bởi $x$ là kết hợp mạnh.*

$a(u, v, w) = 0$ mỗi khi hai trong ba phần tử $u, v, w$ bằng $x$ và chỉ cần áp dụng Bổ đề 3.

#### Bổ đề 5 {#alg-iii-a0-lem-5 .statement}

*Giả sử ánh xạ $a$ là phản xứng và cho $\mathbf{X}, \mathbf{Y}$ là hai đại số con kết hợp mạnh của $\mathbf{F}$. Khi đó đại số con của $\mathbf{E}$ sinh bởi $\mathbf{X} \cup \mathbf{Y}$ là kết hợp.*

Cho $Z$ là tập hợp các $z \in \mathbf{E}$ sao cho $a(u, v, z) = 0$ với mọi $u \in \mathbf{X}$ và $v \in \mathbf{Y}$$, đây hiển nhiên là một môđun con trên A chứa $\mathbf{X}$ và $\mathbf{Y}$ vì $\mathbf{X}$ và $\mathbf{Y}$ là kết hợp mạnh; theo Bổ đề 2, sẽ đủ để kiểm tra rằng, với $u \in \mathbf{X}$ và $v \in \mathbf{Y}$, ta có $uZ \subset Z, vZ \subset Z, Zu \subset Z$ và $Zv \subset Z$. Bây giờ, với $u, u'$ trong $\mathbf{X}$, $v \in \mathbf{Y}$ và $z \in Z$, theo (2)
$$
a(u'u, z, v) - a(u', uz, v) + a(u', u, zv) = a(u', u, z)v + u'a(u, z, v) = 0
$$
do $\mathbf{X}$ là kết hợp mạnh và theo định nghĩa của $Z$. Nhưng vì $\mathbf{X}$ là kết hợp mạnh, $a(u', u, zv) = 0$ và vì $u'u \in \mathbf{X}$, ta có $a(u'u, z, v) = 0$ theo định nghĩa của $Z$. Vậy $a(u', uz, v) = 0$, điều này cho thấy $uZ \subset Z$. Bây giờ áp dụng (2) với $(p, q, r, s) = (v, z, u, u')$, ta cũng thu được tương tự $Zu \subset Z$. Đổi chỗ vai trò của $\mathbf{X}$ và $\mathbf{Y}$ và dùng sự kiện rằng $a$ là phản xứng, ta thu được $vZ \subset Z$ và $Zv \subset Z$; do đó bổ đề được chứng minh.

Bây giờ, để chứng minh rằng (b) kéo theo (a) trong Mệnh đề 1, chỉ cần lấy $\mathbf{X} = \{x\}$ và $\mathbf{Y} = \{y\}$, dùng Bổ đề 4.

#### Định nghĩa 1 {#alg-iii-a0-def-1 .statement}

*Một đại số $\mathbf{F}$ được gọi là thay thế nếu nó thỏa mãn các điều kiện tương đương của Mệnh đề 1.*

Một đại số kết hợp hiển nhiên là thay thế. Trong no. 3 chúng ta sẽ cho một ví dụ về một đại số thay thế không kết hợp.

Nếu $\mathbf{F}$ là một A-đại số thay thế, mọi đại số trên $A'$ $\mathbf{F} \otimes_A A'$ thu được từ $\mathbf{F}$ bằng cách mở rộng vô hướng (§ 1, no. 5) đều là một đại số thay thế trên $A'$, theo điều kiện (b) của Mệnh đề 1.

### 2. ĐẠI SỐ THAY THẾ CAYLEY

#### Mệnh đề 2 {#alg-iii-a0-prop-2 .statement}

*Cho $\mathbf{A}$ là một vành, $\mathbf{F}$ là một đại số Cayley trên $\mathbf{A}$, e là phần tử đơn vị của nó, $s : x \mapsto \overline{x}$ là phép liên hợp của nó và $\mathbf{N} : \mathbf{F} \to \mathbf{A}$ là chuẩn Cayley của nó (§ 3, no. 4).*

(i) *Để $\mathbf{F}$ là thay thế, điều kiện cần và đủ là, với mọi cặp có thứ tự các phần tử $x, y$ của $\mathbf{F}$, $x^2y = x(xy)$.*

(ii) *Nếu F là thay thế, thì N(xy) = N(x)N(y) với mọi x, y trong F.*
(iii) *Giả sử rằng F là thay thế. Để một phần tử x ∈ F khả nghịch, điều kiện cần và đủ là N(x) khả nghịch trong Ae; khi đó nghịch đảo của x là duy nhất và bằng N(x)^{-1}\overline{x}; ký hiệu nghịch đảo này là x^{-1},*
$$
x^{-1}(xy) = x(x^{-1}y) = y
$$
*với mọi y ∈ F.*

Điều kiện $x^2y = x(xy)$ hiển nhiên là cần để F là thay thế (no. 1, Mệnh đề 1). Ngược lại, nếu nó đúng với mọi cặp có thứ tự các phần tử của F, khi áp dụng nó cho $\overline{x}$ và $\overline{y}$, ta được $\overline{x}^2\overline{y} = \overline{x}(\overline{xy})$; áp dụng phép liên hợp s cho quan hệ này, ta thu được $yx^2 = (yx)x$, do đó các điều kiện (c) của Mệnh đề 1 ở no. 1 được thỏa mãn.

Hiển nhiên $a(e, x, y) = 0$ với mọi $x, y$ trong F. Nếu F là thay thế, do đó ta suy ra từ Mệnh đề 1 (no. 1) rằng đại số con G của F sinh bởi e, x và y là kết hợp. Vì $\overline{x} = -x + T(x) \in -x + Ae, \overline{x} \in G$ và tương tự $\overline{y} \in G$. Khi đó $N(xy) = (xy)(\overline{xy}) = xy.\overline{y}.\overline{x} = N(y)x\overline{x} = N(y)N(x)$, dùng sự kiện rằng $N(y) \in Ae$. Điều này chứng minh (ii).

Cuối cùng ta chứng minh (iii). Nếu $N(x)$ khả nghịch trong Ae và nếu ta viết $x' = N(x)^{-1}\overline{x}$, thì $xx' = x'x = e$, vì $N(x) = x\overline{x} = \overline{x}x$. Ngược lại nếu x có một nghịch đảo trái $x''$, thì $N(x'')N(x) = N(e) = e$ theo (ii) và $N(x)$ khả nghịch trong Ae; hơn nữa, vì $x' = N(x)^{-1}\overline{x}$ nằm trong đại số con sinh bởi x và e, các phần tử $x, x', x''$ thuộc đại số con kết hợp sinh bởi x, $x''$ và e và do đó $x'' = x''(xx') = (x''x)x' = x'$, do đó có mệnh đề về tính duy nhất. Các công thức $x^{-1}(xy) = x(x^{-1}y) = y$ suy ra từ sự kiện rằng $x^{-1}, x$ và y là các phần tử của đại số con sinh bởi x, y và e, đại số con này là kết hợp.

#### Mệnh đề 3 {#alg-iii-a0-prop-3 .statement}

*Cho E là một đại số Cayley trên A, γ là một phần tử của A và F là mở rộng Cayley của E xác định bởi γ và phép liên hợp của E (§ 2, no. 5, Mệnh đề 5). Để F là thay thế, điều kiện cần và đủ là E kết hợp.*

Cho $u = (x, y), v = (x', y')$ là hai phần tử của F (trong đó x, y, $x', y'$ nằm trong E). Khi đó (§ 2, no. 5, công thức (27))

$$
\begin{cases}
u^2v = ((x^2 + \gamma \overline{y}y)x' + \gamma \overline{y}'(y\overline{x} + yx), (y\overline{x} + yx)\overline{x}' + y'(x^2 + \gamma \overline{y}y)) \\
u(uv) = (x(xx' + \gamma \overline{y}'y) + \gamma (x'\overline{y} + \overline{x}.\overline{y}')y, y(\overline{x}'\overline{x} + \gamma \overline{y}y') + (y\overline{x}' + y'x)x).
\end{cases}
$$

Dùng sự kiện rằng $\overline{y}y$ và $\overline{x} + x$ thuộc Ae, việc xét các công thức này cho thấy tính kết hợp của E kéo theo $u^2v = u(uv)$ và do đó kéo theo F là thay thế (Mệnh đề 2). Ngược lại, nếu F là thay thế, phương trình $u^2v = u(uv)$ áp dụng khi $y' = 0$ cho
$$
(y\overline{x} + yx)\overline{x}' = y(\overline{x}'\overline{x}) + (y\overline{x}')x.
$$
Bây giờ vế trái bằng $(yT(x))\overline{x}' = y(\overline{x}'T(x)) = y(\overline{x}'x + \overline{x}'\overline{x});$

so sánh với vế phải, ta được $(y \bar{x}') x = y (\bar{x}' x)$, điều này chứng minh tính kết hợp của E, vì $x, y$ và $\bar{x}'$ là các phần tử tùy ý của E.

### 3. OCTONION

Cho E là một đại số quaternion kiểu $(\alpha, \beta, \gamma)$ trên A ($§ 2$, no. 5, Ví dụ 2) và cho $\delta \in A$. Mở rộng Cayley F của E bởi $\delta$ và phép liên hợp của E được gọi là một đại số octonion trên A và được nói là có kiểu $(\alpha, \beta, \gamma, \delta)$. Theo Mệnh đề 3 của no. 2, F là một đại số thay thế. Nó có một cơ sở $(e_i)_{0 \leq i \leq 7}$ gồm 8 phần tử, xác định bởi
$$
\begin{align*}
e_0 &= (e, 0), & e_1 &= (i, 0), & e_2 &= (j, 0), & e_3 &= (k, 0) \\
e_4 &= (0, e), & e_5 &= (0, i), & e_6 &= (0, j), & e_7 &= (0, k)
\end{align*}
$$
trong đó $(e, i, j, k)$ là cơ sở của E xác định loc. cit.; rõ ràng $e_0$ (cũng được ký hiệu bởi $e$) là phần tử đơn vị của F. Nếu $u = \sum_{i=0}^{7} \xi_i e_i$ là một phần tử của F (với các $\xi_i \in A$), các công thức (23), (24) và (31) của $§ 2$, no. 5 cho đối tượng liên hợp, vết và chuẩn của octonion $u$

$$
\left\{
\begin{aligned}
\bar{u} &= (\xi_0 + \beta \xi_1) e_0 - \sum_{i=1}^{7} \xi_i e_i \\
T_F(u) &= 2\xi_0 + \beta \xi_1 \\
N_F(u) &= \xi_0^2 + \beta \xi_0 \xi_1 - \alpha \xi_1^2 - \gamma (\xi_2^2 + \beta \xi_2 \xi_3 - \alpha \xi_3^2) \\
&\quad - \delta (\xi_4^2 + \beta \xi_4 \xi_5 - \alpha \xi_5^2) + \gamma \delta (\xi_6^2 + \beta \xi_6 \xi_7 - \alpha \xi_7^2).
\end{aligned}
\right.
$$

Bây giờ cho $u = (x, y)$, $u' = (x', y')$ và $u'' = (x'', y'')$ là ba octonion (trong đó các phần tử $x, x', x'', y, y', y''$ thuộc E). Các công thức (24) và (27) của $§ 2$, no. 5 cho
$$
\begin{align*}
T_F((uu')u'') &= T(xx'x'') + \delta T(\bar{y}'y x'') + \delta T(\bar{y}''y \bar{x}') + \delta T(\bar{y}''y' x) \\
T_F(u(u'u'')) &= T(xx'x'') + \delta T(x''\bar{y}'y) + \delta T(\bar{x}'\bar{y}''y) + \delta T(x\bar{y}''y')
\end{align*}
$$
(trong đó T chỉ vết trong E và có dùng sự kiện rằng E là kết hợp). Vì $T(xy) = T(yx)$ với mọi quaternion $x, y$ ($§ 2$, no. 4, công thức (17)), suy ra
$$
T_F((uu')u'') = T_F(u(u'u''))
$$
Ta đặc biệt nghiên cứu các octonion kiểu $(-1, 0, -1, -1)$; khi đó các công thức (4) được đơn giản thành
$$
\left\{
\begin{aligned}
\bar{u} &= \xi_0 e_0 - \sum_{i=1}^{7} \xi_i e_i \\
T_F(u) &= 2\xi_0 \\
N_F(u) &= \sum_{i=0}^{7} \xi_i^2.
\end{aligned}
\right.
$$

*Nếu ta lấy $\mathbf{A}$ là trường $\mathbf{R}$ các số thực, thì các octonion kiểu $(-1, 0, -1, -1)$ trên $\mathbf{R}$ được gọi là *octonion Cayley* (hay *octave*). Từ Mệnh đề 2 (ii) của no. 2 suy ra rằng mọi octonion Cayley $\neq 0$ đều *khả nghịch.**

#### Mệnh đề 4 {#alg-iii-a0-prop-4 .statement}

*Cho $F$ là một đại số octonion kiểu $(-1, 0, -1, -1)$ trên $\mathbf{A}$. Tồn tại một không gian vectơ $V$ chiều 3 trên trường hai phần tử $\mathbf{Z}/2\mathbf{Z}$ và một song ánh $\lambda \mapsto e'_\lambda$ từ $V$ lên cơ sở $(e_i)_{0 \leq i \leq 7}$ sao cho*
$$
e'_0 = e_0, \qquad e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}
$$
*với mọi $\lambda, \mu$ trong $V$. Để có $e'_\lambda (e'_\mu e'_\nu) = (e'_\lambda e_\mu) e'_\nu$, chỉ cần trong $V$ các phần tử $\lambda, \mu, \nu$ phụ thuộc tuyến tính trên $\mathbf{Z}/2\mathbf{Z}$; điều kiện này là cần thiết nếu $2 \neq 0$ trong $\mathbf{A}$.*

Ta giữ các ký hiệu ở đầu số này. Từ các công thức (33) của § 2, no. 5 suy ra rằng tập hợp $S$ gồm các phần tử $\pm e_0, \pm e_1, \pm e_2, \pm e_3$ là ổn định đối với phép nhân. Hơn nữa, với $x, y, y'$ trong $E$, theo công thức (22) của § 2, no. 5,
$$
(x, 0)(0, y') = (0, y'x), \quad (0, y')(x, 0) = (0, y'\overline{x}), \quad (0, y)(0, y') = (-\overline{y}'y, 0)
$$
nên tập hợp $T$ gồm các phần tử $\pm e_i$ ($0 \leq i \leq 7$) là ổn định đối với phép nhân; hơn nữa, bảng nhân của nó là *độc lập* với vành $\mathbf{A}$.

Đặc biệt, lấy $\mathbf{A}''$ là trường $\mathbf{Z}/2\mathbf{Z}$ có hai phần tử và $E''$ là đại số quaternion kiểu $(1, 0, 1)$ trên $\mathbf{A}''$, còn $F''$ là đại số octonion kiểu $(1, 0, 1, 1)$ trên $\mathbf{A}''$; gọi $(e''_i)_{0 \leq i \leq 7}$ là cơ sở của $F''$ được tạo thành như mô tả ở trên. Vì $-e''_i = e''_i$, tập $T''$ của các $e''_i$ có 8 phần tử và ổn định đối với phép nhân; hơn nữa, từ trên suy ra ngay lập tức rằng ánh xạ $\theta : T \to T''$ sao cho $\theta(e_i) = \theta(-e_i) = e''_i$ với $0 \leq i \leq 7$ là một đồng cấu đối với phép nhân. Hơn nữa đại số quaternion $E''$ trong trường hợp này là giao hoán và do đó $F''$ là kết hợp (§ 2, no. 5, Mệnh đề 5); thêm nữa, phép liên hợp trong $F''$ trong trường hợp này là đồng nhất. Vậy $T''$ là một *nhóm* và các công thức (8) cho thấy nó là *giao hoán*; các công thức này và các công thức (33) của § 2, no. 5 cho thấy bình phương của mọi phần tử của $T''$ là phần tử khả nghịch. Nếu dùng $V$ để chỉ nhóm $T''$ được viết theo lối cộng, thì $V$ có thể được trang bị một cấu trúc không gian vectơ duy nhất trên $\mathbf{Z}/2\mathbf{Z}$, tất yếu có chiều 3 vì
$$
\operatorname{Card}(V) = 8 = 2^{\dim(V)}.
$$

Với mọi $\lambda \in V$, khi đó ký hiệu $e'_\lambda$ là phần tử của $(e_i)_{0 \leq i \leq 7}$ sao cho $\theta(e'_\lambda) = \lambda$; khi đó $e'_0 = e_0$; hơn nữa, vì $\theta$ là một đồng cấu và quan hệ $\theta(x) = \theta(y)$ tương đương với $x = \pm y$, nên $e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}$. Nếu $\lambda, \mu, \nu$ độc lập tuyến tính trên $\mathbf{Z}/2\mathbf{Z}$, thì chúng lập thành một cơ sở của $V$ và do đó mọi phần tử $e_i$ ($0 \leq i \leq 7$) đều sẽ thuộc đại số con sinh bởi $e'_\lambda, e'_\mu$ và $e'_\nu$; khi $2 \neq 0$ trong $\mathbf{A}$, đẳng thức $e'_\lambda (e'_\mu e'_\nu) = (e'_\lambda e'_\mu) e'_\nu$ vì thế là không thể có, bởi vì khi đó $F$ sẽ kết hợp và do đó $E$ sẽ giao hoán (§ 2, no. 5, Mệnh đề 5), điều này mâu thuẫn với các quan hệ (33) của § 2, no. 5. Mặt khác, nếu $\lambda, \mu, \nu$ phụ thuộc tuyến tính trong V, thì ba phần tử $e'_\lambda, e'_\mu, e'_v$ thuộc một đại số con với 2 phần tử sinh của F, vì vậy nó là kết hợp (no. 1, Mệnh đề 1); do đó có kết luận.

#### Nhận xét {#alg-iii-a0-n3-rem-1 .statement}

Vì $\bar{e}'_\lambda = -e'_\lambda$ với $\lambda \neq 0$,

$$
e'_\lambda{}^2 = -e_0 \quad \text{với } \lambda \neq 0,
$$
$$
e'_\mu e'_\lambda = -e'_\lambda e'_\mu \quad \text{với } \lambda \neq 0, \mu \neq 0 \text{ và } \mu \neq \lambda.
$$

### Bài tập {#alg-iii-a0-exercises}

Xem [các bài tập cho Phụ lục 0](exercises/a0/).
