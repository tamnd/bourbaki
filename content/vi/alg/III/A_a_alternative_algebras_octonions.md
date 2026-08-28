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
pdf_pages: 0635-0641, 0678-0678
extraction: ocr
subsections:
    - "no": 1
      title: ALTERNATIVE ALGEBRAS
      page: 0
      pdf_page: 635
    - "no": 2
      title: ALTERNATIVE CAYLEY ALGEBRAS
      page: 0
      pdf_page: 637
    - "no": 3
      title: OCTONIONS
      page: 0
      pdf_page: 639
statements: 11
exercises: 3
content_sha256: 4076c5a121c8c1f00019e97a82398e53fa7d69936cc2ba9f3a3f5b6b08321270
translated_from: content/en/alg/III/A_a_alternative_algebras_octonions.md
source_content_sha256: 281581bb5201e4e85a70581608d54b3807414edb6034cc7863fc7fe4de4c8db0
translation_model: gpt-5-6-mini
translation_run: translate-vi-19aaef7b
glossary_version: 34
glossary_terms_sha256: 091bf3569760f7015399b2b0dcb42c77fdd2f637c79d4f438a0881586836da5f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# ĐẠI SỐ ALTERNATIVE. OCTONION

### 1. ĐẠI SỐ ALTERNATIVE

Cho A là một vành giao hoán và F là một đại số trên A (không nhất thiết kết hợp). Với mọi ba phần tử $x, y, z$ của F, ta viết

$$
a(x, y, z) = x(yz) - (xy)z
$$

(associator của $x, y, z$); $a$ hiển nhiên là một ánh xạ A-tuyến tính ba của $F \times F \times F$ vào F.

#### Bổ đề 1 {#alg-iii-a0-lem-1 .statement}

*Với mọi $p, q, r, s$ trong đại số $F$,*

$$
a(pq, r, s) - a(p, qr, s) + a(p, q, rs) = a(p, q, r)s + pa(q, r, s).
$$

Việc kiểm tra theo ngay lập tức từ định nghĩa (1).

#### Mệnh đề 1 {#alg-iii-a0-prop-1 .statement}

*Đối với một đại số trên A $F$, các điều kiện sau là tương đương:*
(a) *Với mọi cặp có thứ tự các phần tử $x, y$ của F, đại số con sinh bởi $x$ và $y$ là kết hợp.*
(b) *Ánh xạ ba tuyến tính $(x, y, z) \mapsto a(x, y, z)$ là phản xứng (§ 7, no. 3).*
(c) *Với mọi cặp có thứ tự các phần tử $x, y$ của F, $x^2y = x(xy)$ và $yx^2 = (yx)x$.*

Rõ ràng (a) suy ra (c). Ta chứng minh (c) suy ra (b): theo định nghĩa (§ 7, no. 3), để chứng minh (b), chỉ cần kiểm tra rằng $a(x, x, y) = 0$ và $a(x, y, y) = 0$, điều này chính xác là (c).

Để chứng minh (b) suy ra (a), ta sử dụng 4 bổ đề sau:

#### Bổ đề 2 {#alg-iii-a0-lem-2 .statement}

*Cho $E$ là một đại số trên A sao cho ánh xạ ba tuyến tính $(x, y, z) \mapsto a(x, y, z)$ là phản xứng, $S$ là một hệ sinh của $E$ và $U$ là một môđun con trên A của $E$ chứa $S$ và sao cho $sU \subset U$ và $Us \subset U$ với mọi $s \in S$. Khi đó $U = E$.*

Tập hợp $U'$ gồm các $x \in E$ sao cho $xU \subset U$ và $Ux \subset U$ hiển nhiên là một môđun con trên A của $E$, theo giả thiết nó chứa $S$. Mặt khác, với $x, y$ trong $U'$ và $u \in U$, theo giả thiết

$$
(xy)u = x(yu) + a(x, y, u) = x(yu) - a(x, u, y) = x(yu) - (xu)y + x(uy) \in U;
$$

khi chuyển qua đại số đối, ta cũng có tương tự $u(xy) \in U$. Do đó $U'$ là một đại số con của $E$ và, vì nó chứa $S$, $U' = E$. Suy ra $EU \subset U$ và *a fortiori* $UU \subset U$, điều này chứng minh rằng $U$ là một đại số con của $E$; vì nó chứa $S$, $U = E$, điều này chứng minh bổ đề.

Một tập con $H$ của $F$ được gọi là *kết hợp mạnh* nếu $a(u, v, w) = 0$ khi *ít nhất hai* trong các phần tử $u, v, w$ thuộc $H$.

#### Bổ đề 3 {#alg-iii-a0-lem-3 .statement}

*Giả sử rằng ánh xạ $a$ là phản xứng. Nếu $H$ là một tập hợp kết hợp mạnh của $F$, đại số con của $F$ sinh bởi $H$ là kết hợp mạnh.*

Vì tập hợp các tập hợp kết hợp mạnh của $F$ là quy nạp, chỉ cần chứng minh rằng nếu $H$ là một tập hợp kết hợp mạnh *cực đại* của $F$, thì $H$ là một *đại số con* của $F$. Vì $H$ hiển nhiên là một dưới-A-môđun của $F$, chỉ cần kiểm tra rằng với mọi hai phần tử $u, v$ của $H$, $H \cup \{uv\}$ cũng là kết hợp mạnh, bởi theo định nghĩa của $H$, điều này sẽ suy ra $uv \in H$. Bây giờ, với mọi $z \in H$ và mọi $t \in F$, theo (2)

$$
a(uv, t, z) - a(u, vt, z) + a(u, v, tz) = 0
$$

vì $\mathbf{H}$ là kết hợp mạnh; do $u, v, z$ thuộc $\mathbf{H}$, cũng có
$$
a(u, vt, z) = a(u, v, tz) = 0,
$$
do đó $a(uv, t, z) = 0$. Sử dụng tính chất rằng $a$ là phản xứng, điều này chỉ ra rằng $a(p, q, r) = 0$ bất cứ khi nào ít nhất hai trong các phần tử $p, q, r$ thuộc $\mathbf{H} \cup \{uv\}$ do đó bổ đề.

#### Bổ đề 4 {#alg-iii-a0-lem-4 .statement}

*Giả sử rằng ánh xạ $a$ là phản xứng. Khi đó, với mọi $x \in \mathbf{F}$, đại số con của $\mathbf{F}$ sinh bởi $x$ là kết hợp mạnh.*

$a(u, v, w) = 0$ bất cứ khi nào hai trong ba phần tử $u, v, w$ bằng $x$ và chỉ cần áp dụng Bổ đề 3.

#### Bổ đề 5 {#alg-iii-a0-lem-5 .statement}

*Giả sử rằng ánh xạ $a$ là phản xứng và cho $\mathbf{X}, \mathbf{Y}$ là hai đại số con kết hợp mạnh của $\mathbf{F}$. Khi đó đại số con của $\mathbf{E}$ sinh bởi $\mathbf{X} \cup \mathbf{Y}$ là kết hợp.*

Cho $Z$ là tập hợp các $z \in \mathbf{E}$ sao cho $a(u, v, z) = 0$ với mọi $u \in \mathbf{X}$ và $v \in \mathbf{Y}$, đây hiển nhiên là một A-môđun con chứa $\mathbf{X}$ và $\mathbf{Y}$ vì $\mathbf{X}$ và $\mathbf{Y}$ kết hợp mạnh; theo Bổ đề 2, chỉ cần kiểm tra rằng, với $u \in \mathbf{X}$ và $v \in \mathbf{Y}$, $uZ \subset Z, vZ \subset Z, Zu \subset Z$ và $Zv \subset Z$. Bây giờ, với $u, u'$ thuộc $\mathbf{X}$, $v \in \mathbf{Y}$ và $z \in Z$, theo (2)
$$
a(u'u, z, v) - a(u', uz, v) + a(u', u, zv) = a(u', u, z)v + u'a(u, z, v) = 0
$$
do $\mathbf{X}$ kết hợp mạnh và theo định nghĩa của $Z$. Nhưng vì $\mathbf{X}$ kết hợp mạnh, $a(u', u, zv) = 0$ và vì $u'u \in \mathbf{X}$, $a(u'u, z, v) = 0$ theo định nghĩa của $Z$. Do đó $a(u', uz, v) = 0$, suy ra $uZ \subset Z$. Áp dụng (2) với $(p, q, r, s) = (v, z, u, u')$, ta cũng thu được $Zu \subset Z$. Đổi chỗ vai trò của $\mathbf{X}$ và $\mathbf{Y}$ và sử dụng tính phản xứng của $a$, ta thu được $vZ \subset Z$ và $Zv \subset Z$; do đó có bổ đề.

Để chứng minh (b) suy ra (a) trong Mệnh đề 1, bây giờ chỉ cần lấy $\mathbf{X} = \{x\}$ và $\mathbf{Y} = \{y\}$, sử dụng Bổ đề 4.

#### Định nghĩa 1 {#alg-iii-a0-def-1 .statement}

*Một đại số $\mathbf{F}$ được gọi là thay thế nếu nó thỏa mãn các điều kiện tương đương của Mệnh đề 1.*

Một đại số kết hợp hiển nhiên là thay thế. Trong no. 3 chúng ta sẽ đưa ra một ví dụ về một đại số thay thế không kết hợp.

Nếu $\mathbf{F}$ là một đại số thay thế trên A, thì mọi A-đại số $\mathbf{F} \otimes_A A'$ thu được từ $\mathbf{F}$ bằng cách mở rộng vô hướng (§ 1, no. 5) đều là một $A'$-đại số thay thế, như suy ra từ điều kiện (b) của Mệnh đề 1.

### 2. ĐẠI SỐ THAY THẾ CAYLEY

#### Mệnh đề 2 {#alg-iii-a0-prop-2 .statement}

*Cho $\mathbf{A}$ là một vành, $\mathbf{F}$ là một Cayley $\mathbf{A}$-đại số, e là phần tử đơn vị của nó, $s : x \mapsto \overline{x}$ là phép liên hợp của nó và $\mathbf{N} : \mathbf{F} \to \mathbf{A}$ là chuẩn Cayley của nó (§ 3, no. 4).

(i) Để $\mathbf{F}$ là thay thế, điều kiện cần và đủ là, với mọi cặp có thứ tự các phần tử $x, y$ của $\mathbf{F}$, $x^2y = x(xy)$.*

(ii) *Nếu F là thay thế, thì N(xy) = N(x)N(y) với mọi x, y trong F.*
(iii) *Giả sử F là thay thế. Đối với một phần tử x ∈ F, điều kiện cần và đủ để x khả nghịch là N(x) khả nghịch trong Ae; khi đó nghịch đảo của x là duy nhất và bằng N(x)^{-1}\overline{x}; ký hiệu phần tử này là x^{-1},*
$$
x^{-1}(xy) = x(x^{-1}y) = y
$$
*hoặc mọi y ∈ F.*

Điều kiện $x^2y = x(xy)$ hiển nhiên là cần thiết để F là thay thế (no. 1, Mệnh đề 1). Ngược lại, nếu nó đúng với mọi cặp có thứ tự các phần tử của F, áp dụng nó cho $\overline{x}$ và $\overline{y}$, ta được $\overline{x}^2\overline{y} = \overline{x}(\overline{xy})$; áp dụng phép liên hợp s vào quan hệ này, ta thu được $yx^2 = (yx)x$, do đó các điều kiện (c) của Mệnh đề 1 của no. 1 được thỏa mãn.

Hiển nhiên $a(e, x, y) = 0$ với mọi $x, y$ trong F. Nếu F là thay thế, do đó ta suy ra từ Mệnh đề 1 (no. 1) rằng đại số con G của F sinh bởi e, x và y là kết hợp. Vì $\overline{x} = -x + T(x) \in -x + Ae, \overline{x} \in G$ và tương tự $\overline{y} \in G$. Khi đó $N(xy) = (xy)(\overline{xy}) = xy.\overline{y}.\overline{x} = N(y)x\overline{x} = N(y)N(x)$, sử dụng tính chất $N(y) \in Ae$. Điều này chứng minh (ii).

Cuối cùng ta chứng minh (iii). Nếu $N(x)$ khả nghịch trong Ae và ta viết $x' = N(x)^{-1}\overline{x}$, thì $xx' = x'x = e$, vì $N(x) = x\overline{x} = \overline{x}x$. Ngược lại, nếu x có nghịch đảo trái $x''$, thì $N(x'')N(x) = N(e) = e$ theo (ii) và $N(x)$ khả nghịch trong Ae; hơn nữa, vì $x' = N(x)^{-1}\overline{x}$ thuộc đại số con sinh bởi x và e, các phần tử $x, x', x''$ thuộc đại số con kết hợp sinh bởi x, $x''$ và e, do đó $x'' = x''(xx') = (x''x)x' = x'$, do đó có tính duy nhất. Các công thức $x^{-1}(xy) = x(x^{-1}y) = y$ suy ra từ việc $x^{-1}, x$ và y là các phần tử của đại số con sinh bởi x, y và e, đại số này là kết hợp.

#### Mệnh đề 3 {#alg-iii-a0-prop-3 .statement}

*Cho E là một đại số Cayley A, γ là một phần tử của A và F là mở rộng Cayley của E xác định bởi γ và phép liên hợp của E (§ 2, no. 5, Mệnh đề 5). Để F là thay thế, điều kiện cần và đủ là E kết hợp.*

Cho $u = (x, y), v = (x', y')$ là hai phần tử của F (trong đó x, y, $x', y'$ thuộc E). Khi đó (§ 2, no. 5, công thức (27))

$$
\begin{cases}
u^2v = ((x^2 + \gamma \overline{y}y)x' + \gamma \overline{y}'(y\overline{x} + yx), (y\overline{x} + yx)\overline{x}' + y'(x^2 + \gamma \overline{y}y)) \\
u(uv) = (x(xx' + \gamma \overline{y}'y) + \gamma (x'\overline{y} + \overline{x}.\overline{y}')y, y(\overline{x}'\overline{x} + \gamma \overline{y}y') + (y\overline{x}' + y'x)x).
\end{cases}
$$

Sử dụng tính chất $\overline{y}y$ và $\overline{x} + x$ thuộc Ae, việc xét các công thức này cho thấy tính kết hợp của E kéo theo $u^2v = u(uv)$ và do đó F là thay thế (Mệnh đề 2). Ngược lại, nếu F là thay thế, phương trình $u^2v = u(uv)$ áp dụng khi $y' = 0$ cho
$$
(y\overline{x} + yx)\overline{x}' = y(\overline{x}'\overline{x}) + (y\overline{x}')x.
$$
Vế trái bằng $(yT(x))\overline{x}' = y(\overline{x}'T(x)) = y(\overline{x}'x + \overline{x}'\overline{x});$ so sánh với vế phải, ta được $(y \bar{x}') x = y (\bar{x}' x)$, điều này chứng minh tính kết hợp của E, vì $x, y$ và $\bar{x}'$ là các phần tử tùy ý của E.

### 3. CÁC OCTONION

Cho E là một đại số quaternion kiểu $(\alpha, \beta, \gamma)$ trên A ($§ 2$, no. 5, Ví dụ 2) và cho $\delta \in A$. Mở rộng Cayley F của E bởi $\delta$ và phép liên hợp của E được gọi là một đại số octonion trên A và được nói là kiểu $(\alpha, \beta, \gamma, \delta)$. Theo Mệnh đề 3 của no. 2, F là một đại số thay thế. Nó có một cơ sở $(e_i)_{0 \leq i \leq 7}$ gồm 8 phần tử, được xác định bởi
$$
\begin{align*}
e_0 &= (e, 0), & e_1 &= (i, 0), & e_2 &= (j, 0), & e_3 &= (k, 0) \\
e_4 &= (0, e), & e_5 &= (0, i), & e_6 &= (0, j), & e_7 &= (0, k)
\end{align*}
$$
trong đó $(e, i, j, k)$ là cơ sở của E được xác định loc. cit.; hiển nhiên $e_0$ (cũng được ký hiệu bởi $e$) là phần tử đơn vị của F. Nếu $u = \sum_{i=0}^{7} \xi_i e_i$ là một phần tử của F (với các $\xi_i \in A$), các công thức (23), (24) và (31) của $§ 2$, no. 5, cho liên hợp, vết và chuẩn của octonion $u$

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
(trong đó T ký hiệu vết trong E và đã sử dụng tính chất E là kết hợp). Vì $T(xy) = T(yx)$ với mọi quaternion x, y ($§ 2$, no. 4, công thức (17)), suy ra
$$
T_F((uu')u'') = T_F(u(u'u''))
$$
Đặc biệt ta xét các octonion kiểu $(-1, 0, -1, -1)$; các công thức (4) khi đó được rút gọn thành
$$
\left\{
\begin{aligned}
\bar{u} &= \xi_0 e_0 - \sum_{i=1}^{7} \xi_i e_i \\
T_F(u) &= 2\xi_0 \\
N_F(u) &= \sum_{i=0}^{7} \xi_i^2.
\end{aligned}
\right.
$$

*Nếu lấy $\mathbf{A}$ là trường $\mathbf{R}$ các số thực, các octonion của kiểu $(-1, 0, -1, -1)$ trên $\mathbf{R}$ được gọi là *octonion Cayley* (hay *octave*). Suy ra từ Mệnh đề 2 (ii) của no. 2 rằng mọi octonion Cayley $\neq 0$ đều *khả nghịch.*

#### Mệnh đề 4 {#alg-iii-a0-prop-4 .statement}

*Cho $F$ là một đại số octonion kiểu $(-1, 0, -1, -1)$ trên $\mathbf{A}$. Tồn tại một không gian vectơ $V$ chiều 3 trên trường có hai phần tử $\mathbf{Z}/2\mathbf{Z}$ và một song ánh $\lambda \mapsto e'_\lambda$ của $V$ lên cơ sở $(e_i)_{0 \leq i \leq 7}$ sao cho*
$$
e'_0 = e_0, \qquad e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}
$$
*đối với mọi $\lambda, \mu$ trong $V$. Để có $e'_\lambda (e'_\mu e'_\nu) = (e'_\lambda e_\mu) e'_\nu$, chỉ cần rằng, trong $V$, $\lambda, \mu, \nu$ độc lập tuyến tính trên $\mathbf{Z}/2\mathbf{Z}$; điều kiện này là cần thiết nếu $2 \neq 0$ trong $\mathbf{A}$.*

Ta giữ lại ký hiệu ở đầu số này. Suy ra từ các công thức (33) của § 2, no. 5 rằng tập hợp $S$ gồm các phần tử $\pm e_0, \pm e_1, \pm e_2, \pm e_3$ ổn định đối với phép nhân. Hơn nữa, đối với $x, y, y'$ trong $E$, theo công thức (22) của § 2, no. 5,
$$
(x, 0)(0, y') = (0, y'x), \quad (0, y')(x, 0) = (0, y'\overline{x}), \quad (0, y)(0, y') = (-\overline{y}'y, 0)
$$
sao cho tập hợp $T$ gồm các phần tử $\pm e_i$ ($0 \leq i \leq 7$) ổn định đối với phép nhân; hơn nữa, bảng phép nhân của nó *độc lập* với vành $\mathbf{A}$.

Đặc biệt, cho $\mathbf{A}''$ là trường $\mathbf{Z}/2\mathbf{Z}$ có hai phần tử và cho $E''$ là đại số quaternion kiểu $(1, 0, 1)$ trên $\mathbf{A}''$ và $F''$ là đại số các octonion kiểu $(1, 0, 1, 1)$ trên $\mathbf{A}''$; cho $(e''_i)_{0 \leq i \leq 7}$ là cơ sở của $F''$ được lập như đã mô tả ở trên. Vì $-e''_i = e''_i$, tập hợp $T''$ của các $e''_i$ có 8 phần tử và ổn định đối với phép nhân; hơn nữa, suy ra ngay lập tức từ điều trên rằng ánh xạ $\theta : T \to T''$ sao cho $\theta(e_i) = \theta(-e_i) = e''_i$ với $0 \leq i \leq 7$ là một đồng cấu đối với phép nhân. Hơn nữa, đại số quaternion $E''$ trong trường hợp này là giao hoán và do đó $F''$ là kết hợp (§ 2, no. 5, Mệnh đề 5); hơn nữa, phép liên hợp trong $F''$ trong trường hợp này là ánh xạ đồng nhất. Do đó $T''$ là một *nhóm* và các công thức (8) cho thấy rằng nó là *giao hoán*; các công thức này và các công thức (33) của § 2, no. 5 cho thấy rằng bình phương của mọi phần tử của $T''$ là phần tử khả nghịch. Nếu $V$ được dùng để ký hiệu nhóm $T''$ viết theo phép cộng, thì $V$ có thể được trang bị một cấu trúc không gian vectơ duy nhất trên $\mathbf{Z}/2\mathbf{Z}$, tất yếu có chiều 3 vì
$$
\operatorname{Card}(V) = 8 = 2^{\dim(V)}.
$$

For all $\lambda \in V$, ký hiệu $e'_\lambda$ là phần tử của $(e_i)_{0 \leq i \leq 7}$ sao cho $\theta(e'_\lambda) = \lambda$; khi đó $e'_0 = e_0$; hơn nữa, vì $\theta$ là một đồng cấu và quan hệ $\theta(x) = \theta(y)$ tương đương với $x = \pm y$, ta có $e'_\lambda e'_\mu = \pm e'_{\lambda + \mu}$. Nếu $\lambda, \mu, \nu$ độc lập tuyến tính trên $\mathbf{Z}/2\mathbf{Z}$, chúng tạo thành một cơ sở của $V$ và do đó mọi phần tử $e_i$ ($0 \leq i \leq 7$) sẽ thuộc đại số con sinh bởi $e'_\lambda, e'_\mu$ và $e'_\nu$; khi $2 \neq 0$ trong $\mathbf{A}$, $e'_\lambda (e'_\mu e'_\nu) = (e'_\lambda e'_\mu) e'_\nu$ vì thế là không thể xảy ra, bởi vì $F$ sẽ là kết hợp và do đó $E$ sẽ là giao hoán (§ 2, no. 5, Mệnh đề 5), điều này mâu thuẫn với các quan hệ (33) của § 2, no. 5. Mặt khác, nếu $\lambda, \mu, \nu$ phụ thuộc tuyến tính trong V, ba phần tử $e'_\lambda, e'_\mu, e'_v$ thuộc một đại số con với 2 phần tử sinh của F, do đó nó là kết hợp (no. 1, Mệnh đề 1); do đó có kết luận.

#### Nhận xét {#alg-iii-a0-n3-rem-1 .statement}

Vì $\bar{e}'_\lambda = -e'_\lambda$ với $\lambda \neq 0$,

$$
e'_\lambda{}^2 = -e_0 \quad \text{với } \lambda \neq 0,
$$
$$
e'_\mu e'_\lambda = -e'_\lambda e'_\mu \quad \text{với } \lambda \neq 0, \mu \neq 0 \text{ và } \mu \neq \lambda.
$$

### Bài tập {#alg-iii-a0-exercises}

Xem các [bài tập cho Phụ lục 0](exercises/a0/).
