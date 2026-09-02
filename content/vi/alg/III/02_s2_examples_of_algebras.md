---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 2
section_title: Examples of algebras
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0462-0481, 0642-0650
extraction: ocr
subsections:
    - "no": 1
      title: ENDOMORPHISM ALGEBRAS
      page: 0
      pdf_page: 462
    - "no": 2
      title: MATRIX ELEMENTS
      page: 0
      pdf_page: 462
    - "no": 3
      title: QUADRATIC ALGEBRAS
      page: 0
      pdf_page: 463
    - "no": 4
      title: CAYLEY ALGEBRAS
      page: 0
      pdf_page: 465
    - "no": 5
      title: CONSTRUCTION OF CAYLEY ALGEBRAS. QUATERNIONS
      page: 0
      pdf_page: 467
    - "no": 6
      title: ALGEBRA OF A MAGMA, A MONOID, A GROUP
      page: 0
      pdf_page: 470
    - "no": 7
      title: FREE ALGEBRAS
      page: 0
      pdf_page: 472
    - "no": 8
      title: DEFINITION OF AN ALGEBRA BY GENERATORS AND RELATIONS
      page: 0
      pdf_page: 474
    - "no": 9
      title: POLYNOMIAL ALGEBRAS
      page: 0
      pdf_page: 476
    - "no": 10
      title: TOTAL ALGEBRA OF A MONOID
      page: 0
      pdf_page: 478
    - "no": 11
      title: FORMAL POWER SERIES OVER A COMMUTATIVE RING
      page: 0
      pdf_page: 479
statements: 17
exercises: 3
content_sha256: efcac11f6e5095f707ece0ba51bf7b1f08d82a5631a512761cb5396f0a198b58
translated_from: content/en/alg/III/02_s2_examples_of_algebras.md
source_content_sha256: bd5951cd090d56ae73c754360396e4a160968b09d8b97344a2867e90be9ed798
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5.4
translation_run: translate-vi-f8bdd831
glossary_version: 34
glossary_terms_sha256: 5f6f452911382bf73dfbd881f3741e3c6b255dec78df456a638450d9c2c9e914
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. VÍ DỤ VỀ CÁC ĐẠI SỐ

Trong suốt đoạn này, A ký hiệu một vành giao hoán.

### 1. CÁC ĐẠI SỐ TỰ ĐỒNG CẤU

Cho B là một đại số kết hợp trên A có phần tử đơn vị ký hiệu bởi 1 và cho M là một B-môđun phải. Ta biết rằng vành $E = \mathrm{End}_B(M)$ cũng có một cấu trúc môđun trên tâm của B. Bây giờ ảnh của đồng cấu $h : \alpha \mapsto \alpha . 1$ từ A vào B được chứa trong tâm của B (§ 1, no. 1); do đó $h$ cho E một cấu trúc A-môđun. Hơn nữa, với $\alpha \in A$ và $f, g$ trong E,

$$
\alpha(f \circ g) = f \circ (\alpha g) = (\alpha f) \circ g;
$$

do đó phép nhân trong E và cấu trúc A-môđun trên E định nghĩa một cấu trúc đại số kết hợp trên A trên E; ánh xạ đồng nhất của M là một phần tử đơn vị của đại số này.

### 2. CÁC PHẦN TỬ MA TRẬN

Cho B là một đại số kết hợp có đơn vị trên A và $\mathbf{M}_n(B)$ là tập hợp các ma trận bình phương cấp n trên B (II, § 10, no. 7). Khi đó $\mathbf{M}_n(B)$ có một cấu trúc A-môđun được định nghĩa bởi $\alpha . (b_{ij}) = (\alpha b_{ij})$ ($\alpha \in A, b_{ij} \in B, 1 \leq i \leq n, 1 \leq j \leq n$); cấu trúc này và phép nhân ma trận định nghĩa một cấu trúc đại số kết hợp có đơn vị trên A trên $\mathbf{M}_n(B)$. Song ánh chính tắc của $\mathbf{M}_n(B)$ lên $\mathrm{End}_B(B_d^n)$ (II, § 10, no. 7) là một đẳng cấu đại số trên A.

Khi $B = A$, đại số trên A $\mathbf{M}_n(A)$ thừa nhận một cơ sở chính tắc $(E_{ij})$ gồm các phần tử đơn vị ma trận (II, § 10, no. 3); bảng phép nhân tương ứng là

$$
E_{ij} E_{hk} = \delta_{jh} E_{ik}.
$$

Phần tử đơn vị $I_n$ bằng $\sum_{i=1}^n E_{ii}$.

### 3. CÁC ĐẠI SỐ BẬC HAI

Cho $\alpha, \beta$ là hai phần tử của A và $(e_1, e_2)$ là cơ sở chính tắc của $A^2$. Đại số bậc hai kiểu $(\alpha, \beta)$ trên A là A-môđun $A^2$ với cấu trúc đại số được định nghĩa bởi bảng phép nhân (§ 1, no. 7)

$$
e_1^2 = e_1, \quad e_1 e_2 = e_2 e_1 = e_2, \quad e_2^2 = \alpha e_1 + \beta e_2.
$$

Một đại số trên A E đẳng cấu với một đại số bậc hai cũng được gọi là một đại số bậc hai. Nói rằng E thừa nhận một cơ sở gồm hai phần tử mà một trong chúng là phần tử đơn vị cũng tương đương với điều đó.

Có thể chứng minh rằng mọi đại số trên A có đơn vị thừa nhận một cơ sở gồm hai phần tử đều là một đại số bậc hai (Bài tập 1).

Nếu một cơ sở $(e_1, e_2)$ của một đại số trên A có bảng phép nhân (2), nó được gọi là một cơ sở kiểu $(\alpha, \beta)$. Do lạm dụng ngôn ngữ, một đại số bậc hai được nói là có kiểu $(\alpha, \beta)$ khi nó có một cơ sở kiểu $(\alpha, \beta)$.

#### Mệnh đề 1 {#alg-iii-s2-prop-1 .statement}

*Một đại số bậc hai E là kết hợp và giao hoán.*

Sự kiện E giao hoán suy ra từ phương trình $e_1 e_2 = e_2 e_1$ trong (2); tương tự, để kiểm tra tính kết hợp, chỉ cần thấy rằng $x(yz) = (xy)z$ khi $x, y, z$ mỗi phần tử đều bằng $e_1$ hoặc $e_2$. Bây giờ, quan hệ này là hiển nhiên nếu ít nhất một trong các phần tử $x, y, z$ bằng $e_1$; nó cũng đúng với $x = y = z = e_2$ vì E giao hoán; do đó có mệnh đề.

Gọi $e$ là phần tử đơn vị của một đại số bậc hai E và cho $(e, i)$ là một cơ sở của E kiểu $(\alpha, \beta)$; mọi cơ sở khác của E chứa $e$ do đó có dạng $(e, j)$ với $j = \gamma e + \delta i$ (II, § 7, no. 2, Hệ quả của Mệnh đề 3); hơn nữa, để $(e, j)$ là một cơ sở của E, điều kiện cần và đủ là $\delta$ khả nghịch trong A; điều kiện này hiển nhiên là đủ; ngược lại, nếu $\bar{i}$ là ảnh chính tắc của $i$ trong $E/Ae$, thì $\bar{i}$ và $\bar{j} = \delta \bar{i}$ mỗi cái phải tạo thành một cơ sở của $E/Ae$, do đó tính cần thiết của điều kiện. Khi đó

$$
j^2 = (\gamma^2 + \alpha \delta^2)e + (2\gamma \delta + \beta \delta^2)i = (\alpha \delta^2 - \gamma^2 - \beta \gamma \delta)e + (2\gamma + \beta \delta)j;
$$

do đó thấy rằng E có kiểu

$$
(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)
$$

cho mọi $\delta \in A$ khả nghịch và mọi $\gamma \in A$. Đặc biệt, nếu $E$ có kiểu $(\alpha, 2\beta')$, thì $i$ cũng có kiểu $(\alpha + {\beta'}^2, 0)$ như thấy được bằng cách lấy $\gamma = -\beta'$ và $\delta = 1$.

#### Mệnh đề 2 {#alg-iii-s2-prop-2 .statement}

*Cho $E$ là một đại số bậc hai trên $A$ và $e$ là phần tử đơn vị của nó. Với mọi $u \in E$, gọi $T(u)$ là vết của tự đồng cấu $m_u : x \mapsto ux$ của $A$-môđun tự do $E$ (II, § 4, no. 3). Khi đó ánh xạ $s$ xác định bởi $s(u) = T(u).e - u$ là một tự đẳng cấu của đại số $E$ và $s^2(u) = u$ với mọi $u \in E$.*

Cho $(e, i)$ là một cơ sở của $E$ có kiểu $(\alpha, \beta)$; khi đó $T(e) = 2$, vì $s(e) = e$, và $T(i) = \beta$, do đó $s(i) = \beta e - i$. Vì vậy $(e, s(i))$ là một cơ sở của $E$, có kiểu được cho bởi (3) với $\gamma = \beta$ và $\delta = -1$, điều này lại cho $(\alpha, \beta)$; suy ra rằng $s$ là một tự đẳng cấu của đại số $E$. Vì $m_{s(u)} = s m_u s^{-1}$, các tự đồng cấu $m_u$ và $m_{s(u)}$ của $A$-môđun $E$ có cùng một vết (II, § 4, no. 3, Mệnh đề 3), do đó

$$
s^2(u) = T(u).e - s(u) = T(u).e - (T(u).e - u) = u
$$

với mọi $u \in E$.

Tự đẳng cấu $s$ được gọi là *liên hợp* của $A$-đại số $E$ và $s(u)$ là *liên hợp* của $u$.

Nếu $u = \xi e + \eta i$, với $\xi, \eta$ thuộc $A$, thì $s(u) = (\xi + \beta \eta)e - \eta i$, do đó

(4)
$$
T(u)e = u + s(u) = (2\xi + \beta \eta)e
$$
(5)
$$
u.s(u) = (\xi^2 + \beta \xi \eta - \alpha \eta^2)e = N(u)e
$$

nơi ta đã viết $N(u) = \xi^2 + \beta \xi \eta - \alpha \eta^2$. Các phần tử $T(u)$ và $N(u)$ (hoặc, khi $A$ và $Ae$ được đồng nhất một cách chính tắc, các phần tử $T(u)e$ và $N(u)e$) lần lượt được gọi là *vết* và *chuẩn* của $u$.

Khi $\beta = 0$, các công thức trên được rút gọn thành

(6)
$$
s(\xi e + \eta i) = \xi e - \eta i, \quad T(\xi e + \eta i) = 2\xi, \quad N(\xi e + \eta i) = \xi^2 - \alpha \eta^2.
$$

Rõ ràng $T$ là một *dạng tuyến tính* trên $E$*và* $N$ là một *dạng toàn phương* trên $E$ (IX, § 3, no. 4)*. Vì $E$ là giao hoán và kết hợp, suy ra từ (5) rằng

(7)
$$
N(uv) = N(u)N(v).
$$

Để $u$ là *khả nghịch trong* $E$, điều kiện cần và đủ là $N(u)$ *khả nghịch trong* $A$. Thật vậy, vì $N(e) = 1$, tính cần thiết của điều kiện suy ra từ (7), bằng cách viết $v = u^{-1}$. Ngược lại, nếu $N(u)$ khả nghịch trong $A$, thì từ (5) suy ra rằng $u$ khả nghịch và

(8)
$$
u^{-1} = (N(u))^{-1}s(u).
$$

*Có thể chứng minh rằng $N(u)$ là định thức (§ 8, no. 1) của tự đồng cấu $m_u$ (xem § 9 no. 3, Ví dụ 1).*

Mệnh đề sau đây cho cấu trúc của các đại số bậc hai trên một trường giao hoán:

#### Mệnh đề 3 {#alg-iii-s2-prop-3 .statement}

*Cho E là một đại số trên A bậc hai kiểu* $(\alpha, \beta)$.

(i) *Nếu A là một trường và không chứa phần tử* $\zeta$ *sao cho* $\zeta^2 = \alpha + \beta \zeta$, *thì E là một trường (giao hoán)* (xem V, § 3).

(ii) *Nếu vành* A *chứa một phần tử* $\zeta$ *sao cho* $\zeta^2 = \alpha + \beta \zeta$ *và* $\beta - 2\zeta$ *là khả nghịch* (tương ứng, không), *thì E đẳng cấu với* A $\times$ A *tương ứng, có kiểu* $(0, 0))$.

Ta chứng minh (i). Cho $\xi, \eta$ là hai phần tử của A và $u = \xi e + \eta i$. Nếu $\eta \neq 0$ và ta viết $\theta = -\xi \eta^{-1}$, thì $\mathrm{N}(u) = \eta^2 (\theta^2 - \beta \theta - \alpha)$ theo (5), do đó $\mathrm{N}(u) \neq 0$ theo giả thiết trên A; nếu $\eta = 0$, thì $\mathrm{N}(u) = \xi^2$. Trong mọi trường hợp, nếu $u \neq 0$, thì $\mathrm{N}(u) \neq 0$, do đó $\mathrm{N}(u)$ khả nghịch trong A và vì vậy $u$ khả nghịch trong E.

Bây giờ ta chứng minh (ii). Cơ sở chính tắc $(e_1, e_2)$ của đại số A $\times$ A có kiểu $(0, 1)$. Ta đã thấy (công thức (3)) rằng E có kiểu

$$
(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)
$$

với mọi $\gamma \in A$ và mọi $\delta$ khả nghịch trong A. Nếu $\beta - 2\zeta$ khả nghịch, lấy $\delta = (\beta - 2\zeta)^{-1}$ và $\gamma = -\zeta (\beta - 2\zeta)^{-1}$; khi đó $2\gamma + \beta \delta = 1$ và

$$
\alpha \delta^2 - \gamma^2 - \beta \gamma \delta = \delta^2 (\alpha - \zeta^2 + \beta \zeta) = 0;
$$

do đó E thuộc kiểu $(0, 1)$ và vì thế đẳng cấu với A $\times$ A. Nếu $\beta - 2\zeta = 0$, đã nhận xét rằng E thuộc kiểu $(\alpha + \zeta^2, 0)$ và vì thế thuộc kiểu $(0, 0)$ vì $\alpha + \zeta^2 = 2\zeta^2 - \beta \zeta = 0$.

Một đại số bậc hai trên A thuộc kiểu $(0, 0)$ cũng được gọi là *đại số số đối ngẫu* trên A.

### 4. ĐẠI SỐ CAYLEY

#### Định nghĩa 1 {#alg-iii-s2-def-1 .statement}

*Một đại số Cayley trên* A *là một cặp có thứ tự* (E, s), *trong đó* E *là một đại số trên* A *có phần tử đơn vị* e *và* s *là một phản tự đẳng cấu của* E *sao cho*

$$
u + s(u) \in Ae \quad \text{and} \quad u.s(u) \in Ae
$$

*với mọi* $u \in E$.

$s$ được gọi là *phép liên hợp* của đại số Cayley (E, s) và $s(u)$ là *liên hợp* của $u$. Điều kiện $u + s(u) \in Ae$ kéo theo rằng $u$ và $s(u)$ là *giao hoán được*. Ta viết

(9) $$
T(u) = u + s(u)
$$
(10) $$
N(u) = u.s(u) = s(u).u
$$

và các phần tử này của đại số con $Ae$ được gọi tương ứng là *vết Cayley* và *chuẩn* của $u$.

Cặp có thứ tự gồm một đại số bậc hai E và phép liên hợp của nó s (là một phản tự đẳng cấu vì E giao hoán) (no. 3) là một đại số Cayley.

Cho (E, s) là một đại số Cayley; vì $s(e) = e,\ s(u + s(u)) = u + s(u)$, nói cách khác $s(u) + s^2(u) = u + s(u)$ hay cũng

$$
s^2(u) = u
$$

nên $s^2$ là ánh xạ đồng nhất của E. Suy ra rằng

$$
T(s(u)) = T(u), \quad N(s(u)) = N(u).
$$

Sau hết, quan hệ $(u - u)(u - s(u)) = 0$ cho

$$
u^2 - T(u).u + N(u) = 0
$$

với mọi $u \in E$.

#### Mệnh đề 4 {#alg-iii-s2-prop-4 .statement}

*Cho E là một A-đại số và s và s' là các phản tự đẳng cấu của E sao cho (E, s) và (E, s') là các đại số Cayley. Nếu E thừa nhận một cơ sở chứa phần tử đơn vị e, thì s' = s.*

Rõ ràng $s'(u) = s(u) = u$ với mọi $u \in Ae$. Nếu T, N (ứng với T', N') là các hàm vết và chuẩn của (E, s) (ứng với (E, s')), thì từ (13) suy ra rằng

$$
(T(u) - T'(u)).u - (N(u) - N'(u)) = 0.
$$

Cho B là một cơ sở của E chứa e và u là một phần tử của B phân biệt với e; khi đó $T(u) - T'(u) = 0$, do đó $s(u) = s'(u)$. Vì s và s' trùng nhau trên B, nên chúng bằng nhau.

Trong phần sau, ta sẽ viết $\bar{u} = s(u)$, sao cho

$$
\left\{\begin{array}{lll}
u + \bar{u} = T(u), & u\bar{u} = \bar{u}u = N(u), & \bar{u} = u \\
u + v = \bar{u} + \bar{v}, & \alpha u = \alpha \bar{u}, & uv = \bar{v}.\bar{u}
\end{array}\right.
$$

với $u, v$ trong E, $\alpha \in A$; hơn nữa

$$
T(e) = 2e, \quad N(e) = e.
$$

Từ công thức

$$
T(uv) = uv + \overline{uv} = uv + \bar{v}.\bar{u} = uv + (T(v) - v)(T(u) - u),
$$

ta suy ra rằng

$$
uv + vu = T(u)v + T(v)u + (T(uv) - T(u)T(v))
$$

do đó, khi đổi chỗ $u$ và $v$,

$$
T(vu) = T(uv).
$$

Mặt khác, $N(u + v) = (u + v)(\bar{u} + \bar{v}) = N(u) + N(v) + T(u\bar{v})$, do đó

(18)
$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v).
$$

Bây giờ, áp dụng (16) với $u$ được thay bởi $\bar{u}$ ta được
$$
T(u\bar{v}) = T(u)T(v) + \bar{u}v + v\bar{u} - T(u)v - T(v)\bar{u} = T(u)T(v) - uv - \bar{v}.\bar{u};
$$
do đó

(19)
$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v) = T(u)T(v) - T(uv).
$$

Sau hết, rõ ràng với mọi $\alpha \in A$,

(20)
$$
N(\alpha u) = \alpha^2 N(u);
$$
đặc biệt $N(2u) = 4N(u)$, nên công thức (19) cho

(21)
$$
(T(u))^2 - T(u^2) = 2N(u).
$$

Rõ ràng $T$ là một dạng tuyến tính trên $(Ae)$-môđun $E$. Vì $(u, v) \mapsto T(v\bar{u})$ là một dạng song tuyến tính trên môđun này, *nên từ (18) và (20) suy ra rằng $N$ là một dạng bậc hai (x. IX, § 3, no. 4).*

### 5. PHÉP DỰNG CÁC ĐẠI SỐ CAYLEY. QUATERNION

Cho $(E, s)$ là một đại số Cayley trên $A$, mà ta sẽ dùng các ký hiệu của no. 4, và cho $\gamma \in A$. Gọi $F$ là đại số trên $A$ có môđun nền tảng là $E \times E$ và phép nhân được định nghĩa bởi

(22)
$$
(x, y)(x', y') = (xx' + \gamma \bar{y}'y, y\bar{x}' + y'x);
$$
rõ ràng $(e, 0)$ là phần tử đơn vị của $F$ và $E \times \{0\}$ là một đại số con của $F$ đẳng cấu với $E$; trong phần sau ta sẽ *đồng nhất* nó với $E$, để cho $x \in E$ được đồng nhất với $(x, 0)$ và đặc biệt $e$ được đồng nhất với phần tử đơn vị của $F$.

Gọi $t$ là phép hoán vị của $F$ được định nghĩa bởi

(23)
$$
t((x, y)) = (\bar{x}, -y) \quad (x \in E, y \in E).
$$

#### Mệnh đề 5 {#alg-iii-s2-prop-5 .statement}

(i) *Cặp có thứ tự $(F, t)$ là một đại số Cayley trên $A$*.

(ii) *Cho $j = (0, e)$, để cho $(x, y) = xe + yj$ với $x \in E, y \in E$. Vết Cayley và chuẩn Cayley $T_F$ và $N_F$ của $F$ được cho bởi các công thức*

(24)
$$
T_F(xe + yj) = T(x), \quad N_F(xe + yj) = N(x) - \gamma N(y).
$$

(iii) *Để $F$ kết hợp, điều kiện cần và đủ là $E$ kết hợp và giao hoán.*

Với $(x, y) \in \mathbf{F}$,

$$
(x, y) + t((x, y)) = (x + \overline{x}, 0) = T(x)e
$$
(25)
$$
(x, y)t((x, y)) = (x, y)(\overline{x}, -y) = (xx - \gamma \overline{y}y, y\overline{x} - yx)
= (\mathrm{N}(x) - \gamma \mathrm{N}(y), 0) = (\mathrm{N}(x) - \gamma \mathrm{N}(y))e.
$$
(26)

Do đó, để chứng minh cả (i) lẫn (ii), chỉ cần chỉ ra rằng $t$ là một phản tự đẳng cấu của $\mathbf{F}$. Rõ ràng $t$ là một song ánh A-tuyến tính. Mặt khác,
$$
t((x, y) \cdot (x', y')) = t((xx' + \gamma \overline{y}'y, y\overline{x}' + y'x)) = (\overline{x}'\overline{x} + \gamma \overline{y}y', -y\overline{x} - y'x)
= (\overline{x}', -y')(\overline{x}, -y) = t((x', y'))t((x, y))
$$
và vì thế $t$ là một phản tự đẳng cấu.

Còn lại phải chứng minh (iii). Vì E được đồng nhất với một đại số con của F, có thể giả sử E là kết hợp. Cho $u = (x, y)$, $u' = (x', y')$, $u'' = (x'', y'')$ là các phần tử của F. Khi đó
$$
\begin{cases}
(uu')u'' = ((xx' + \gamma \overline{y}'y)x'' + \gamma \overline{y}''(\overline{y}x' + y'x), \\
\phantom{(uu')u'' = } (y\overline{x}' + y'x)\overline{x}'' + y''(xx' + \gamma \overline{y}'y)) \\
u(u'u'') = (x(x'x'' + \gamma \overline{y}''y') + (\gamma(x''\overline{y}' + \overline{x}'\overline{y}'')y, \\
\phantom{u(u'u'') = } y(\overline{x}''\overline{x}' + \gamma \overline{y}'y'') + (y'\overline{x}'' + y''x')x).
\end{cases}
$$
(27)

Xét các công thức này cho thấy rằng tính giao hoán của E kéo theo tính kết hợp của F. Ngược lại, nếu F kết hợp, các công thức (27) áp dụng với $y = y' = 0$, $x'' = 0$ và $y'' = e$ cho $(0, x'x) = (0, xx')$, tức là $x'x = xx'$ với mọi $x, x'$ trong E; do đó khi ấy E là giao hoán.

Cũng chú ý rằng, trong ký hiệu trên, với $x, y$ trong E,
$$
yj = j\overline{y}, \quad x(yj) = (yx)j, \quad (xj)y = (x\overline{y})j, \quad (xj)(yj) = \overline{y}xe
$$
(28)
$$
j^2 = e.
$$
(29)

Đại số Cayley $(\mathbf{F}, t)$ được gọi là *mở rộng Cayley của* $(\mathbf{E}, s)$ *được xác định bởi* $\gamma$.

#### Ví dụ {#alg-iii-s2-n5-exa-1 .statement}

(1) Nếu ta lấy $\mathbf{E} = \mathbf{A}$ (và do đó $s = 1_A$), thì đại số $\mathbf{F}$ là một *đại số bậc hai trên A* với cơ sở $(e, j)$ trong đó $j^2 = \gamma e$.

(2) Lấy E là một *đại số bậc hai kiểu* $(\alpha, \beta)$, sao cho môđun nền của E là $\mathbf{A}^2$, với bảng phép nhân (2) (no. 3) đối với cơ sở chính tắc. Lấy s là phép liên hợp của E (no. 3, Mệnh đề 2). Khi đó, với mọi$\gamma \in \mathbf{A}$, mở rộng Cayley F của$(\mathbf{E}, s)$xác định bởi$\gamma$được gọi là *đại số quaternion kiểu*$(\alpha, \beta, \gamma)$, là *kết hợp* theo no. 3, Mệnh đề 1 và Mệnh đề 5 ở trên; môđun nền của nó là$\mathbf{A}^4$và, nếu$(e, i, j, k)$ký hiệu cơ sở chính tắc của$\mathbf{A}^4$, thì bảng phép nhân tương ứng được cho bởi
$$
\left\{\begin{array}{lll}
i^2 = \alpha e + \beta i, & ij = k, & ik = \alpha j + \beta k, \\
ji = \beta j - k, & j^2 = \gamma e, & jk = \beta \gamma e - \gamma i, \\
ki = -\alpha j, & kj = \gamma i, & k^2 = -\alpha \gamma e.
\end{array}\right.
$$
(30)

Hơn nữa, với$u = \rho e + \xi i + \eta j + \zeta k$(trong đó$\rho, \xi, \eta, \zeta$thuộc$\mathbf{A}$), ta có (viết$\bar{u}$thay cho$t(u)$và đồng nhất$\mathbf{A}$với$\mathbf{Ae}$):

$$
\left\{
\begin{array}{l}
u = (\rho + \beta \xi)e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho + \beta \xi \\
N_F(u) = \rho^2 + \beta \rho \xi - \alpha \xi^2 - \gamma (\eta^2 + \beta \eta \zeta - \alpha \zeta^2).
\end{array}
\right.
$$

Các công thức (30) suy ra từ (28) và (29), và các công thức (31) suy ra từ (23) và (24), có tính đến các công thức của đại số bậc hai E.

Khi đó, với$u, v$thuộc F,

$$
N_F(uv) = N_F(u)N_F(v)
$$

vì$N_F(uv) = uv.\overline{uv} = uv(\overline{v}.\overline{u}) = u(v\overline{v})\overline{u} = (u\overline{u})(v\overline{v})$nhờ tính kết hợp và việc$N_F(u)$thuộc tâm của F.

Một A-đại số đẳng cấu với một đại số quaternion cũng được gọi là một *đại số quaternion*; nếu một cơ sở của một đại số như vậy có bảng phép nhân (30), thì nó được gọi là một *cơ sở kiểu*$(\alpha, \beta, \gamma)$. Theo một lối nói lạm dụng, một đại số quaternion được nói là *kiểu*$(\alpha, \beta, \gamma)$khi nó có một cơ sở kiểu$(\alpha, \beta, \gamma)$.

Khi$\beta = 0$, các công thức (30) và (31) đơn giản thành

$$
\left\{
\begin{array}{lll}
i^2 = \alpha e, & ij = k, & ik = \alpha j, \\
ji = -k, & j^2 = \gamma e, & jk = -\gamma i, \\
ki = -\alpha i, & kj = \gamma i, & k^2 = -\alpha \gamma e,
\end{array}
\right.
$$

và

$$
\left\{
\begin{array}{l}
\bar{u} = \rho e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho \\
N_F(u) = \rho^2 - \alpha \xi^2 - \gamma \eta^2 + \alpha \gamma \zeta^2.
\end{array}
\right.
$$

Khi đó,$(\alpha, \beta, \gamma)$được thay ở mọi chỗ bằng$(\alpha, \gamma)$trong các biểu thức trên. Ngay lập tức thấy rằng các đại số quaternion kiểu$(\alpha, \gamma)$và$(\gamma, \alpha)$là *đẳng cấu*.

Chú ý rằng các công thức (32) cho thấy F không giao hoán khi$-1 \neq 1$trong$\mathbf{A}$.

*Lấy A là trường$\mathbf{R}$các số thực và$\alpha = \gamma = -1, \beta = 0$, đại số tương ứng F được gọi là *đại số quaternion Hamilton* và được ký hiệu bởi$\mathbf{H}$. Nếu$u = \rho e + \xi i + \eta j + \zeta k$($\rho, \xi, \eta, \zeta$thuộc$\mathbf{R}$) là một phần tử$\neq 0$của$\mathbf{H}$, thì công thức$u\bar{u} = \bar{u}u = \rho^2 + \xi^2 + \eta^2 + \zeta^2$(xem (34)) cho thấy$N(u) \neq 0$trong$\mathbf{R}$, do đó$u$thừa nhận một *nghịch đảo*$u^{-1} = N(u)^{-1}\bar{u}$trong$\mathbf{H}$và vì thế$\mathbf{H}$là một *trường không giao hoán*.

(3) Nếu lấy E là một đại số quaternion (xem *Ví dụ 2*), thì mở rộng Cayley của E xác định bởi một phần tử$\delta \in \mathbf{A}$nói chung là không kết hợp

(Mệnh đề 5); nó được gọi là một đại số octonion trên A (xem Phụ lục, no. 3).

### 6. ĐẠI SỐ CỦA MỘT MAGMA, MỘT MONOID, MỘT NHÓM

Nhắc lại rằng một magma là một tập hợp với một luật hợp thành (I, § 1, no. 1). Cho S là một magma được viết theo phép nhân và đặt E = A^{(S)} là A-môđun các tổ hợp tuyến tính hình thức của các phần tử của S (II, § 1, no. 11); ta biết rằng một ánh xạ chính tắc$s \mapsto e_s$được xác định từ S vào A^{(S)} sao cho họ$(e_s)_{s \in S}$là một cơ sở (gọi là chính tắc) của A^{(S)}, khi đó mọi phần tử của A^{(S)} được viết duy nhất dưới dạng$\sum_{s \in S} \alpha_s e_s$, trong đó$(\alpha_s)$là một họ các phần tử của A có giá hữu hạn. Khi đó một cấu trúc A-đại số được xác định trên E bằng cách lấy làm bảng phép nhân của cơ sở chính tắc

$$
e_s e_t = e_{st}.
$$

Đại số E được xác định như vậy được gọi là đại số của magma S trên A. Nếu$x = \sum_{s \in S} \xi_s e_s$và$y = \sum_{s \in S} \eta_s e_s$là hai phần tử của E, thì

$$
xy = \sum_{s \in S} \left( \sum_{tu = s} \xi_t \eta_u \right) e_s.
$$

Khi S là một monoid (tương ứng, nhóm), E được gọi là đại số của monoid (tương ứng, nhóm) S trên A; khi đó nó là một đại số kết hợp (§ 1, no. 7); tương tự, khi S là một monoid giao hoán, đại số của nó là kết hợp và giao hoán. Cuối cùng nếu magma S thừa nhận một phần tử đơn vị u, thì$e_u$là phần tử đơn vị của đại số E; vì phần tử$e_u$là tự do, khi đó A được đồng nhất với đại số con Ae_u của E.

Khi A \neq \{0\}, đôi khi S được đồng nhất với ảnh của nó qua đơn ánh$s \mapsto e_s$, sao cho một phần tử của E được viết dưới dạng$\sum_{s \in S} \alpha_s s$; nhưng sự đồng nhất này là không thể (nếu không gây nhầm lẫn) khi S được viết theo phép cộng. Khi đó$e^s$cũng thường được viết thay cho$e_s$.

Cho B là một vành giao hoán khác và$\rho : A \to B$một đồng cấu vành; xét các đại số E = A^{(S)} và E' = B^{(S)} của cùng một magma S trên A và B và gọi $(e_s)_{s \in S}$ và $(e'_s)_{s \in S}$ là các cơ sở chính tắc tương ứng của chúng. Đại số $B^{(S)}$ được đồng nhất một cách chính tắc, dưới ánh xạ A-tuyến tính j sao cho $j(e_s \otimes 1) = e'_s$ với mọi $s \in S$, với đại số $A^{(S)} \otimes_A B$ thu được từ $A^{(S)}$ bằng cách mở rộng vành các vô hướng thành B (II, § 1, no. 11, Hệ quả 3 của Mệnh đề 17).

#### Mệnh đề 6 {#alg-iii-s2-prop-6 .statement}

*Cho S là một magma, F một A-đại số và f một đồng cấu của*

S vào F chỉ với cấu trúc nhân của nó. Khi đó tồn tại một và chỉ một đồng cấu A-đại số $\bar{f}: A^{(S)} \to F$ làm cho biểu đồ

$$
\begin{array}{ccc}
S & \xrightarrow{f} & F \\
| & & | \\
A^{(S)} & \xrightarrow{\bar{f}} & F
\end{array}
$$

giao hoán

(trong đó mũi tên đứng bên trái là ánh xạ chính tắc $s \mapsto e_s$).

Cho $\bar{f}: A^{(S)} \to F$ là đồng cấu A-môđun duy nhất sao cho $\bar{f}(e_s) = \bar{f}(s)$ (II, § 1, no. 11, Hệ quả 3 của Mệnh đề 17); chỉ cần kiểm tra rằng $\bar{f}$ là một đồng cấu đại số và để làm việc này chỉ cần chứng minh rằng $\bar{f}(e_s e_t) = \bar{f}(e_s) \bar{f}(e_t)$, điều này suy ra ngay lập tức từ định nghĩa và giả thiết $f(st) = f(s)f(t)$.

Mệnh đề 6 biểu thị sự kiện rằng cặp có thứ tự gồm $A^{(S)}$ và ánh xạ chính tắc $s \mapsto e_s$ là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1) trong đó $\Sigma$ là loài cấu trúc A-đại số và các ánh xạ $\alpha$ là các đồng cấu của S vào một A-đại số chỉ với luật nhân của nó.

#### Hệ quả {#alg-iii-s2-n6-cor-1 .statement}

Cho S, S' là hai magma và $g: S \to S'$ một đồng cấu. Khi đó tồn tại một và chỉ một đồng cấu A-đại số $u: A^{(S)} \to A^{(S')}$ làm cho biểu đồ

$$
\begin{array}{ccc}
S & \xrightarrow{g} & S' \\
| & & | \\
A^{(S)} & \xrightarrow{u} & A^{(S')}
\end{array}
$$

giao hoán

(trong đó các mũi tên đứng là các ánh xạ chính tắc).

Chỉ cần áp dụng Mệnh đề 6 bằng cách lấy $f$ là ánh xạ hợp thành $S \xrightarrow{g} S' \to A^{(S')}$.

Đặc biệt, nếu T là một tập con ổn định của magma S (I, § 1, no. 4), tập hợp các phần tử $\sum_{s \in T} \alpha_s e_s$ của $A^{(S)}$ là một đại số con của $A^{(S)}$ đẳng cấu chính tắc với đại số $A^{(T)}$ và đôi khi được đồng nhất với đại số sau.

#### Ví dụ {#alg-iii-s2-n6-exa-1 .statement}

Cho V là một A-môđun và S một monoid tác động lên V ở bên trái; điều này có nghĩa (I, § 5, no. 1) là cho trước một ánh xạ $(s, x) \mapsto s.x$ của S vào V sao cho $s.(x + y) = s.x + s.y, s.(\alpha x) = \alpha(s.x)$ và $s.(t.x) = (st).x$ với $s, t$ trong S, $x, y$ trong V và $\alpha \in A$ và, ký hiệu e là phần tử đơn vị của S, e.x = x với x ∈ V. Viết f(s)(x) = s.x, f là một đồng cấu của S vào đại số End_A(V) (chỉ với luật nhân của nó), ánh xạ phần tử đơn vị e lên phần tử đơn vị l_V. Áp dụng Mệnh đề 6, ta thu được một đồng cấu A-đại số $\bar{f}: A^{(S)} \to \mathrm{End}_A(V)$, đồng cấu này cho nhóm cơ sở của V một cấu trúc môđun trái trên $A^{(S)}$.

Điều này cho phép ta rút gọn việc nghiên cứu các nhóm giao hoán có toán tử về việc nghiên cứu các môđun. Thật vậy, cho M là một nhóm giao hoán có toán tử được viết theo lối cộng, mà mọi luật ngoài của nó đều được viết theo lối nhân. Gọi $\Omega$ là tập hợp tổng (Lý thuyết tập hợp, II, § 4, no. 8) của các miền của các toán tử của những luật ngoài khác nhau trên M, mỗi miền trong số này được đồng nhất một cách chính tắc với một tập con của $\Omega$. Gọi Mo($\Omega$) là monoid tự do (I § 7, no. 2) được xây dựng trên $\Omega$; một luật tác động

$$
(s, x) \mapsto s.x
$$

được xác định trên M với miền các toán tử là Mo($\Omega$), bằng quy nạp theo độ dài của từ s trong Mo($\Omega$); nếu s có độ dài 0, thì nó là từ rỗng e và ta viết $e.x = x$ với mọi $x \in M$. Nếu x có độ dài $n \geq 1$, nó có thể được viết duy nhất dưới dạng $s = tu$, trong đó u có độ dài $n - 1$ và t có độ dài 1, sao cho $t \in \Omega$; khi đó ta viết $s.x = t.(u.x)$. Với mọi hai từ s, $s'$ trong Mo($\Omega$), quan hệ $s.(s'.x) = (ss').x$ được kiểm tra bằng quy nạp theo độ dài của s.

Khi đó áp dụng phương pháp được mô tả ở trên, ta thu được trên M một cấu trúc môđun trái trên $\mathbf{Z}^{(Mo(\Omega))}$ và không khó để kiểm tra rằng các khái niệm thông thường trong lý thuyết các nhóm có toán tử (các nhóm con ổn định, các đồng cấu) là như nhau đối với các nhóm giao hoán có toán tử và các môđun nhờ đó liên kết với chúng.

### 7. ĐẠI SỐ TỰ DO

#### Định nghĩa 2 {#alg-iii-s2-def-2 .statement}

*Cho I là một tập hợp; gọi M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) là magma tự do (resp. monoid tự do, resp. monoid giao hoán tự do) dẫn xuất từ I. Đại số của M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) trên A được gọi là đại số tự do (resp. đại số kết hợp tự do, resp. đại số giao hoán kết hợp tự do (hoặc, do lạm dụng ngôn ngữ, đại số giao hoán tự do)) của tập hợp I trên vành A.*

Ta sẽ ký hiệu đại số tự do (resp. đại số kết hợp tự do, resp. đại số giao hoán tự do) của I trên A bởi Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)). Bằng cách hợp thành ánh xạ chính tắc của I vào M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) với ánh xạ chính tắc của M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) vào Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)), ta thu được một ánh xạ chính tắc của I vào Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)), ánh xạ này là đơn ánh nếu $A \neq \{0\}$. Ta sẽ ký hiệu ảnh của một phần tử $i \in I$ dưới ánh xạ chính tắc này bởi $X_i$ và ta sẽ nói rằng $X_i$ là bất định nguyên có chỉ số i của Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)).

Vì Mo(I) và $\mathbf{N}^{(I)}$ mỗi cái đều có một phần tử đơn vị, nên Libas_A(I) và Libasc_A(I) là những đại số kết hợp có đơn vị và hơn nữa Libasc_A(I) là giao hoán. Nếu e là phần tử đơn vị của Libas_A(I) (resp. Libasc_A(I)), thì ánh xạ $\alpha \mapsto \alpha e$ là một đẳng cấu từ A lên một vành con của tâm của Libas_A(I) (resp. Libasc_A(I)), và vành con này được đồng nhất với A (no. 1).

#### Mệnh đề 7 {#alg-iii-s2-prop-7 .statement}

*Cho I là một tập hợp và F là một đại số (resp. đại số kết hợp có đơn vị, resp. đại số kết hợp giao hoán có đơn vị) trên A. Với mọi ánh xạ $f : I \to F$, tồn tại một và chỉ một đồng cấu (resp. đồng cấu có đơn vị) $\bar{f}$ từ Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)) vào F sao cho $\bar{f}(X_i) = f(i)$ với mọi $i \in I$.*

Gọi $F_m$ là magma (resp. monoid) thu được bằng cách trang bị cho tập hợp F luật hợp thành nhân của nó. Tồn tại một và chỉ một đồng cấu (resp. đồng cấu có đơn vị) $g$ từ M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) vào $F_m$ sao cho $g(i) = f(i)$ với mọi $i \in I$ (I, § 7, các số 1, 2 và 7); khi đó Mệnh đề 7 suy ra từ no. 6, Mệnh đề 6.

#### Nhận xét {#alg-iii-s2-n7-rem-1 .statement}

(1) Về sau ta sẽ định nghĩa một đẳng cấu từ Libas_A(I) lên đại số tenxơ của môđun tự do $A^{(I)}$ (§ 5, no. 5) và cả một đẳng cấu từ Libasc_A(I) lên đại số đối xứng của $A^{(I)}$ (§ 6, no. 6).

(2) Cho $\rho$ là một đồng cấu có đơn vị từ A vào một vành giao hoán B. Như đã thấy (§ 2, no. 6), từ $\rho$ dẫn xuất ra một đẳng cấu $\sigma$ từ Lib_B(I) (resp. Libas_B(I), resp. Libasc_B(I)) lên đại số $(\mathrm{Lib}_A(I))_{(B)}$ (resp. $(\mathrm{Libas}_A(I))_{(B)}$, resp. $(\mathrm{Libasc}_A(I))_{(B)}$) thu được bằng cách mở rộng vô hướng sang B nhờ $\rho$; nếu $X_i^A, X_i^B$ là các ẩn số có chỉ số $i$ tương ứng với A và B, thì $\sigma(X_i^B) = X_i^A \otimes 1$.

(3) Cho J là một tập con của I; ta biết rằng M(J) được đồng nhất với một tập con ổn định của magma M(I) và do đó (no. 6) Lib_A(J) được đồng nhất một cách chính tắc với một đại số con của Lib_A(I), được sinh bởi các $X_i$ sao cho $i \in J$; người ta nói rằng chỉ những ẩn số có chỉ số thuộc J mới xuất hiện trong một phần tử của Lib_A(J). Định nghĩa đã cho ở no. 6 của đại số của một magma cho thấy rằng Lib_A(I) là hợp của họ có hướng các đại số con Lib_A(J) khi J chạy qua tập hợp các tập con *hữu hạn* của I. Có những kết quả tương tự cho Libas_A(I) và Libasc_A(I).

(4) Với phần tử s của M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) liên kết một *độ dài* $l(s)$, là một số nguyên $\geqslant 1$ (resp. $\geqslant 0$) sao cho $l(ss') = l(s) + l(s')$ (I, § 7, các số 1, 2 và 7). Nếu $e_s$ là phần tử của Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)) tương ứng với s, thì *bậc toàn phần* (hay đơn giản là *bậc*) của một phần tử $x = \sum_s \alpha_s e_s \neq 0$ của Lib_A(I) (resp. Libas_A(A), resp. Libasc_A(I)) là lớn nhất trong các số $l(s)$ khi s chạy qua tập hợp (không rỗng theo giả thiết) các phần tử sao cho $\alpha_s \neq 0$. Chẳng hạn, nếu $i, j, k$ là ba phần tử phân biệt của I, thì phần tử $(X_i(X_jX_k))X_i - (X_iX_j)(X_kX_i)$ là một phần tử $\neq 0$ có bậc toàn phần 4 trong Lib_A(I).

### 8. ĐỊNH NGHĨA MỘT ĐẠI SỐ BỞI CÁC PHẦN TỬ SINH VÀ CÁC QUAN HỆ

Cho F là một đại số trên A và $(x_i)_{i \in I}$ một họ các phần tử của F. Theo no. 7, Mệnh đề 7, tồn tại một đồng cấu duy nhất $f : \mathrm{Lib}_A(I) \to F$ sao cho $f(X_i) = x_i$ với mọi $i \in I$. Để $f$ là toàn ánh, điều kiện cần và đủ là $(x_i)_{i \in I}$ là một hệ sinh của F.

Nếu $U \in \mathrm{Lib}_A(I)$, thì $f(U)$ được gọi là *phần tử của F dẫn xuất từ U bằng cách thay các phần tử $x_i$ vào các ẩn số $X_i$*, hoặc cũng gọi là *giá trị* của U ứng với các giá trị $x_i$ của các ẩn số $X_i$; nó thường được ký hiệu bởi $U((x_i)_{i \in I})$; đặc biệt $U((X_i)_{i \in I}) = U$. Nếu $\lambda$ là một đồng cấu từ F vào một đại số $F'$ trên A, thì
$$
\lambda(U((x_i)_{i \in I})) = U((\lambda(x_i))_{i \in I}).
$$

Xét riêng trường hợp $F = \mathrm{Lib}_A(J)$, trong đó J là một tập hợp khác; với mọi họ $(H_i)_{i \in I}$ các phần tử của $\mathrm{Lib}_A(J)$ và mọi họ $(y_j')_{j \in J}$ các phần tử của một đại số trên A $F'$,
$$
U((H_i)_{i \in I}))((y_j')_{j \in J}) = U((H_i((y_j')_{j \in J})))_{i \in I}).
$$
(37)

Trong các ký hiệu trên, mọi phần tử U của $\mathrm{Lib}_A(I)$ sao cho $U((x_i)_{i \in I}) = 0$, hoặc tương đương sao cho $f(U) = 0$, được gọi là một *hệ thức* của họ $(x_i)_{i \in I}$ trong F. Iđêan hai phía $\mathrm{Ker}(f)$ gồm các phần tử đó được gọi là *iđêan các hệ thức* của $(x_i)$.

Cho $(R_j)_{j \in J}$ là một họ các phần tử của $\mathrm{Lib}_A(I)$. $((x_i)_{i \in I}, (R_j)_{j \in J})$ được gọi là một *dạng trình bày* của đại số F nếu $(x_i)_{i \in I}$ là một hệ sinh của F và iđêan hai phía của $\mathrm{Lib}_A(I)$ sinh bởi các $R_j$ bằng iđêan các hệ thức của họ $(x_i)_{i \in I}$; các $x_i$ được gọi là các *phần tử sinh* và các $R_j$ là các *hệ thức* của dạng trình bày.

Bây giờ xét một tập hợp I bất kỳ và một họ $(R_j)_{j \in J}$ các phần tử của $\mathrm{Lib}_A(I)$. Đại số thương E của $\mathrm{Lib}_A(I)$ theo iđêan hai phía sinh bởi họ $(R_j)$ được gọi là *đại số phổ quát xác định bởi hệ sinh I liên quan bởi họ các hệ thức* $(R_j)_{j \in J}$. Rõ ràng, nếu $\overline{X}_i$ ký hiệu ảnh của $X_i$ trong E,
$$
((\overline{X}_i)_{i \in I}, (R_j)_{j \in J})
$$
là một *dạng trình bày* của E. Hơn nữa, nếu $(x_i)_{i \in I}$ là một họ các phần tử của một đại số F và $R_j((x_i)_{i \in I}) = 0$ với mọi $j \in J$, thì tồn tại một đồng cấu duy nhất $g : E \to F$ sao cho $g(\overline{X}_i) = x_i$ với mọi $i \in I$; để $((x_i)_{i \in I}, (R_j)_{j \in J})$ là một dạng trình bày của F, điều kiện cần và đủ là $g$ *song ánh*.

Các nhận xét này biện minh cho cách nói lạm dụng sau đây: thay vì nói "*$((x_i)_{i \in I}, (R_j)_{j \in J})$ là một dạng trình bày của F*", người ta cũng nói rằng "*F là đại số sinh bởi các phần tử sinh $x_i$ với các quan hệ $R_j((x_i)_{i \in I}) = 0$*". Khi các $R_j$ có dạng $P_j - Q_j$, người ta cũng nói rằng "*F là đại số sinh bởi các $x_i$ với các quan hệ $P_j((x_i)) = Q_j((x_i))$*".

Cho H là một tập hợp; ta sẽ nói rằng một phần tử S của $\mathrm{Lib}_A(H)$ là một hệ thức *phổ quát* đối với một đại số trên A F nếu $S((x_h)_{h \in H}) = 0$ với *mọi* họ $(x_h)_{h \in H}$ các phần tử của F lấy H làm tập hợp chỉ số.

#### Ví dụ {#alg-iii-s2-n8-exa-1 .statement}

(1) Lấy $H = \{1, 2, 3\}$; các đại số thừa nhận
$$
(X_1 X_2) X_3 - X_1 (X_2 X_3)
$$
làm hệ thức phổ quát là các đại số kết hợp. Các đại số thừa nhận $X_1 X_2 - X_2 X_1$ làm hệ thức phổ quát là các đại số giao hoán. *Các đại số thừa nhận các hệ thức phổ quát $X_1 X_1$ và
$$
(X_1 X_2) X_3 + (X_2 X_3) X_1 + (X_3 X_1) X_2
$$
làm hệ thức phổ quát là các đại số Lie.*

Cho I là một tập hợp; cho một họ $(S_k)_{k \in K}$ các phần tử của Lib_A(H) và xét tập T các phần tử của Lib_A(I) có dạng $S_k((U_h))_{h \in H}$, trong đó k chạy qua K và, với mỗi k, $(U_h)_{h \in H}$ chạy qua tập các họ phần tử của Lib_A(I) lấy H làm tập chỉ số; xét một họ $(R_j)_{j \in J}$ có tập hợp các phần tử là T. Khi đó cho F là đại số phổ quát xác định bởi hệ sinh I liên quan với họ $(R_j)_{j \in J}$ và cho $u : \mathrm{Lib}_A(I) \to F$ là đồng cấu chính tắc, sao cho Ker(u) được sinh bởi các phần tử $S_k((U_h)_{h \in H})$ với mọi $k \in K$ và mọi họ $(U_h)_{h \in H}$ các phần tử của Lib_A(I); rõ ràng mỗi $S_k$ ($k \in K$) là một *quan hệ tử phổ quát* của F. Bây giờ cho F' là một đại số nhận một hệ sinh $(x_i)_{i \in I}$, đối với đó mỗi $S_k$ là một quan hệ tử phổ quát, và cho $u' : \mathrm{Lib}_A(I) \to F'$ là đồng cấu sao cho $u'(X_i) = x_i$ với mọi $i \in I$; rõ ràng Ker(u) $\subset$ Ker(u') và do đó $u'$ có thể được viết một cách duy nhất dưới dạng $u' = h \circ u$, trong đó $h : F \to F'$ là một đồng cấu sao cho $h(\overline{X}_i) = x_i$ với mọi $i \in I$. Vì lý do này F được gọi là *đại số phổ quát xác định bởi hệ sinh I*, *tương ứng với họ các quan hệ tử phổ quát* $(S_k)_{k \in K}$. Do một sự lạm dụng ngôn ngữ, đôi khi F được gọi là đại số phổ quát sinh bởi I và chịu các *đồng nhất thức* $S_k((u_h)) = 0$ với mọi họ $(u_h)_{h \in H}$ các phần tử của F.

*Ví dụ* 2. Cho L' là đại số phổ quát sinh bởi I và chịu các đồng nhất thức $(uv)w - u(vw) = 0$ đối với mọi họ gồm ba phần tử của L' và cho L'' là đại số thu được bằng cách thêm một phần tử đơn vị vào L'; khi đó tồn tại một đẳng cấu có đơn vị duy nhất g từ L'' lên Libas_A(I) sao cho $g(\overline{X}_i) = X_i$ với mọi $i \in I$. Thật vậy, rõ ràng L'' là kết hợp và sự tồn tại của đồng cấu g suy ra từ định nghĩa của L' và các nhận xét đi trước nó; nhưng khi đó rõ ràng L'' thỏa mãn tính chất phổ quát (no. 7, Mệnh đề 7) đặc trưng cho Libas_A(I), do đó suy ra kết luận.

Các xét tương tự như trên có thể được áp dụng cho các đại số kết hợp (tương ứng, các đại số kết hợp giao hoán), có tính đến các nhận xét sau đây. Khi ngữ cảnh cho một chỉ dẫn đủ rõ rằng các đại số được xét là các đại số có đơn vị, thì do một sự lạm dụng ngôn ngữ, một họ $(x_i)_{i \in I}$ các phần tử của một đại số $F$, sao cho đại số con sinh bởi các $x_i$ ($i \in I$) và phần tử đơn vị bằng $F$, thường được gọi là một hệ sinh của $F$. Khi đó cho $F$ là một đại số kết hợp có đơn vị trên $A$ và cho $(x_i)_{i \in I}$ là một họ các phần tử của $F$; theo no. 7, Mệnh đề 7, tồn tại một đồng cấu có đơn vị duy nhất $f : \mathrm{Libas}_A(I) \to F$ sao cho $f(X_i) = x_i$ với mọi $i \in I$; nếu $U \in \mathrm{Libas}_A(I)$, $f(U)$ cũng được gọi là phần tử của $F$ dẫn xuất từ $U$ bằng cách thay các phần tử $x_i$ cho các bất định thức $X_i$ và cũng được ký hiệu bởi $U((x_i)_{i \in I})$. Khi đó các khái niệm quan hệ tử, biểu diễn và quan hệ tử phổ quát chuyển ngay lập tức sang các đại số kết hợp; chỉ cần đơn giản thay thế $\mathrm{Lib}_A(I)$ ở khắp nơi bằng $\mathrm{Libas}_A(I)$. *Đại số kết hợp có đơn vị phổ quát xác định bởi hệ sinh I liên quan với họ các quan hệ tử* $(R_j)_{j \in J}$ là đại số thương của $\mathrm{Libas}_A(I)$ theo iđêan hai phía sinh bởi họ $(R_j)$. Đại số kết hợp có đơn vị phổ quát sinh bởi hệ sinh $I$, tương ứng với một họ các quan hệ tử phổ quát được xác định tương tự. Chúng tôi để cho người đọc công việc phát biểu các định nghĩa tương tự đối với các đại số kết hợp giao hoán với $\mathrm{Libasc}_A(I)$ được thay cho $\mathrm{Libas}_A(I)$.

#### Ví dụ 3 {#alg-iii-s2-n8-exa-3 .statement}

Cho $L'$ là đại số kết hợp có đơn vị phổ quát sinh bởi $I$ và thỏa các đồng nhất thức $uv - vu = 0$ với mọi họ gồm hai phần tử của $L'$. Ta thấy, như trong *Ví dụ 2*, rằng $L'$ đẳng cấu chính tắc với $\mathrm{Libasc}_A(I)$.

### 9. ĐẠI SỐ ĐA THỨC

Cho $B$ là một $A$-đại số kết hợp *giao hoán* có đơn vị và cho $(x_i)_{i \in I}$ là một họ các phần tử của $B$; đại số con của $B$ sinh bởi các $x_i$ ($i \in I$) và phần tử đơn vị được ký hiệu là $A[(x_i)_{i \in I}]_B$ hoặc đơn giản là $A[(x_i)_{i \in I}]$ khi không thể có sự nhầm lẫn. Do đó, với mọi tập hợp $I$, đại số $\mathrm{Libasc}_A(I)$ bằng $A[(X_i)_{i \in I}]$ (cũng được ký hiệu là $A[X_i]_{i \in I}$); ký hiệu sau, có ưu điểm là chỉ ra ký hiệu được chọn để chỉ các bất định, là ký hiệu mà nói chung chúng ta sẽ dùng trong phần còn lại của Khảo luận này. Các phần tử của $A[(X_i)_{i \in I}]$ được gọi là *đa thức theo các bất định* $X_i$ ($i \in I$) *với hệ số trong* $A$; theo quy ước, khi nói "$A[(X_i)_{i \in I}]$ là một đại số đa thức", thì luôn hiểu rằng các $X_i$ là các bất định. Với mọi tập con $J$ của $I$, việc dùng ký hiệu trên tương đương với việc đồng nhất $\mathrm{Libasc}_A(J)$ với đại số con của $\mathrm{Libasc}_A(I)$ sinh bởi các $X_i$ có chỉ số $i \in J$ và phần tử đơn vị (xem no. 7, *Nhận xét (3)*). Với $I = \{1, 2, \ldots, n\}$, ta viết $A[X_1, X_2, \ldots, X_n]$ thay cho $A[(X_i)_{i \in I}]$.

Nếu $I$ và $I'$ là hai tập hợp cùng lực lượng, thì các đại số $\mathrm{Libasc}_A(I)$ và $\mathrm{Libasc}_A(I')$ là đẳng cấu. Người ta thường dùng $A[X]$ để chỉ đại số đa thức tương ứng với một tập hợp chỉ số không xác định chỉ có *một* phần tử, trong đó $X$ chỉ bất định duy nhất; tương tự, $A[X, Y]$, $A[X, Y, Z]$, ... được dùng để chỉ các đại số đa thức tương ứng với các tập hợp chỉ số không xác định có 2, 3, ... phần tử. Chú ý rằng, do các quy ước đã nêu ở trên, chẳng hạn $A[X]$ và $A[Y]$ là các đại số con (phân biệt) của $A[X, Y, Z]$ nếu $A \neq \{0\}$.

Các phần tử
$$
X^\nu = \prod_{i \in I} X_i^{\nu(i)},
$$
trong đó $\nu$ chạy qua $\mathbf{N}^{(I)}$, tạo thành một cơ sở của đại số đa thức $A[(X_i)_{i \in I}]$. Các phần tử này được gọi là các *đơn thức* theo các bất định $X_i$ và số $|\nu| = \sum_{i \in I} \nu(i)$ được gọi là *bậc* (hay *bậc toàn phần*) của đơn thức $X^\nu$. Đơn thức duy nhất có bậc 0 là phần tử đơn vị của $A[(X_i)_{i \in I}]$; nó thường được đồng nhất với phần tử đơn vị 1 của $A$. Mọi đa thức $u$ của $A[(X_i)_{i \in I}]$ đều có thể được viết một cách duy nhất dưới dạng
$$
u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu
$$
với $\alpha_\nu \in A$; các phần tử $\alpha_\nu$, bằng không trừ ra đối với một số hữu hạn chỉ số $\nu \in \mathbf{N}^{(I)}$, được gọi là các *hệ số* của $u$; các phần tử $\alpha_\nu X^\nu$ được gọi là các *số hạng* của $u$ (phần tử $\alpha_\nu X^\nu$ thường được gọi là "số hạng theo $X^\nu$"); riêng số hạng $\alpha_0 X^0$ (được đồng nhất với $\alpha_0 \in A$) được gọi là *số hạng hằng* của $u$. Nếu $J$ là một tập con của $I$, thì $u$ thuộc $A[(X_i)_{i \in J}]$ khi và chỉ khi $\alpha_\nu = 0$ với $\nu \notin \mathbf{N}^{(J)}$. Suy ra $A[(X_i)_{i \in I}]$ là hợp của các đại số con $A[(X_i)_{i \in J}]$, trong đó $J$ chạy qua tập các tập con hữu hạn của $I$. Nếu $\alpha_\nu = 0$ với $|\nu| > n$, thì $u$ được gọi là một *đa thức bậc* $\leq n$. Khi $\alpha_\nu = 0$, thì (do lạm dụng ngôn ngữ) người ta nói rằng $u$ *không chứa số hạng theo* $X^\nu$; riêng khi $\alpha_0 = 0$, thì $u$ được gọi là một đa thức *không có số hạng hằng*.

Với mọi đa thức *khác không* $u = \sum \alpha_\nu X^\nu$, *bậc* (hay *bậc toàn phần*) của $u$ là số lớn nhất trong các số nguyên $|\nu|$ của những đa chỉ số $\nu$ sao cho $\alpha_\nu \neq 0$.

Cho $F$ là một $A$-đại số kết hợp có đơn vị và cho $(x_i)_{i \in I}$ là một họ các phần tử của $F$, *giao hoán từng đôi một*. Đại số con $F'$ của $F$ sinh bởi các $x_i$ và phần tử đơn vị là giao hoán (§ 1, no. 7), điều đó cho phép ta định nghĩa phép thế các $x_i$ cho các $X_i$ trong đa thức $u \in A[(X_i)_{i \in I}]$ (mặc dù $F$ không nhất thiết giao hoán): $u((x_i)_{i \in I})$ là một phần tử của $F'$ và do đó của $F$ và $h: u \to u((x_i)_{i \in I})$ là một đồng cấu của $A[(X_i)_{i \in I}]$ vào $F$. Các phần tử của hạt nhân của $h$ là các hệ thức của họ $(x_i)$ trong $A[(X_i)_{i \in I}]$, cũng gọi là các *hệ thức đa thức* (với hệ số trong $A$) giữa các $x_i$. Ảnh của đồng cấu $h$ là đại số con $F'$, cũng được ký hiệu bởi $A[(x_i)_{i \in I}]$ (ngay cả khi $F$ không giao hoán); nếu $a$ là iđêan các hệ thức đa thức giữa các $x_i$, thì có một dãy khớp các $A$-môđun
$$
0 \longrightarrow a \longrightarrow A[(X_i)_{i \in I}] \xrightarrow{h} A[(x_i)_{i \in I}] \longrightarrow 0.
$$

#### Mệnh đề 8 {#alg-iii-s2-prop-8 .statement}

*Cho $A[(X_i)_{i \in I}]$ là một đại số đa thức, $J$ là một tập con của $I$ và $K$ là phần bù của $J$ trong $I$. Viết $A' = A[(X_j)_{j \in J}]$ và ký hiệu bởi $X'_k$ ($k \in K$) các ẩn trong đại số đa thức Libasc_{A'}(K) = A'[(X'_k)_{k \in K}], thì tồn tại một đẳng cấu vành duy nhất từ A'[(X'_k)_{k \in K}] lên A[(X_i)_{i \in I}] trùng với đồng nhất trên A' và ánh xạ X'_k tới X_k với mọi k \in K.*

Rõ ràng A[(X_i)_{i \in I}] là một $A'$-đại số sinh bởi các X_k với k \in K. Mặt khác, vì một hệ thức đa thức giữa các X_k (k \in K) với hệ số trong A' có thể được viết duy nhất dưới dạng $\sum_v h_v((X_j)_{j \in J}) X^v$ trong đó v chạy qua một tập con hữu hạn của $\mathbf{N}^{(K)}$ và trong đó các h_v là những phần tử của A[(X_j)_{j \in J}], nên các h_v phải là các hệ thức đa thức giữa các X_j với hệ số trong A và do đó đều bằng không, điều đó chứng minh mệnh đề.

Đẳng cấu được mô tả trong Mệnh đề 8 thường được dùng để đồng nhất các phần tử của A[(X_i)_{i \in I}] với các đa thức có hệ số trong A' = A[(X_j)_{j \in J}]. Nếu u là một phần tử $\neq 0$ của A[(X_i)_{i \in I}], bậc toàn phần của nó khi được xét như một phần tử của A'[(X_k)_{k \in K}] cũng được gọi là bậc của nó đối với các X_i có chỉ số i \in K.

#### Nhận xét {#alg-iii-s2-n9-rem-1 .statement}

Cho I và J là hai tập hợp và (P_j)_{j \in J} là một họ các phần tử của $\mathbf{Z}[(X_i)_{i \in I}]$; nếu Q là một phần tử của $\mathbf{Z}[(X_j)_{j \in J}]$ sao cho $Q((P_j)_{j \in J}) = 0$, thì, với mọi họ $(b_i)_{i \in I}$ các phần tử giao hoán từng đôi một của một vành B,
$$
Q((P_j((b_i)_{i \in I}))_{j \in J}) = 0.
$$
Các hệ thức có dạng $Q((P_j)_{j \in J}) = 0$ đôi khi được gọi là các đồng nhất thức đa thức. Ví dụ
$$
(X_1 + X_2)^2 - X_1^2 - X_2^2 - 2X_1X_2 = 0
$$
với
$$
Q = Y_1^2 - Y_2, \quad P_1 = X_1 + X_2, \quad P_2 = X_1^2 + X_2^2 + 2X_1X_2
$$
$$
X_1^n - X_2^n - (X_1 - X_2)(X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}) = 0
$$
với
$$
Q = Y_1 - Y_2Y_3, \quad P_1 = X_1^n - X_2^n, \quad P_2 = X_1 - X_2,
$$
$$
P_3 = X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}
$$
là các đồng nhất thức đa thức.

### 10. ĐẠI SỐ TOÀN PHẦN CỦA MỘT MONOID

Đại số của một monoid S trên A là (như một A-môđun) môđun con của tích $A^S$ gồm các họ $(\alpha_s)_{s \in S}$ có giá hữu hạn; phép nhân trong đại số này được định nghĩa bởi các hệ thức $(\alpha_s)(\beta_s) = (\gamma_s)$, trong đó, với mọi $s \in S$,
$$
\gamma_s = \sum_{tu = s} \alpha_t \beta_u
$$

(x. no. 6, công thức (35)). Tổng ở vế phải của (38) có nghĩa vì $(\alpha_s)$ và $(\beta_s)$ là những họ có giá hữu hạn và do đó họ kép $(\alpha_t\beta_u)_{(t,u)\in S\times S}$ cũng vậy. Nhưng vế phải của (38) cũng có nghĩa đối với các phần tử *tùy ý* $(\alpha_s),\ \beta_s)$ của $A^S$ khi monoid $S$ thỏa mãn điều kiện sau:

(D) *Với mọi* $s\in S$, *chỉ tồn tại một số hữu hạn các cặp có thứ tự* $(t,u)$ *trong* $S\times S$ *sao cho* $tu=s$.

Bây giờ giả sử rằng $S$ thỏa mãn điều kiện (D); khi đó có thể định nghĩa một luật phép nhân trên A-môđun tích $A^S$ bằng công thức (38). Ngay lập tức thấy rằng phép nhân được định nghĩa như vậy trên $A^S$ là A-song tuyến tính; hơn nữa nó *kết hợp*, vì, với $\alpha,\beta,\gamma$ trong $A^S$,

$$
\sum_{uvw=t} \alpha_u\beta_v\gamma_w = \sum_{rw=t} \left( \left( \sum_{uv=r} \alpha_u\beta_v \right) \gamma_w \right) = \sum_{us=t} \left( \alpha_u \left( \sum_{vw=s} \beta_v\gamma_w \right) \right).
$$

Vì vậy phép nhân này và cấu trúc A-môđun trên $A^S$ xác định trên $A^S$ một cấu trúc *đại số kết hợp* có đơn vị trên A; ta sẽ nói rằng tập hợp $A^S$, với cấu trúc này, là *đại số toàn phần* của monoid S trên A.

Ngay lập tức thấy rằng *đại số* $A^{(S)}$ của monoid S trên A (cũng được gọi là *đại số hạn chế* của S khi cần tránh nhầm lẫn) là một *đại số con* của đại số toàn phần của S trên A (và đồng nhất với đại số sau khi S là hữu hạn). *Do lạm dụng ngôn ngữ*, mỗi phần tử $(\xi_s)_{s\in S}$ của đại số toàn phần của S trên A cũng được ký hiệu bằng cùng ký hiệu $\sum_{s\in S} \xi_s e_s$ (hoặc cả $\sum_{s\in S} \xi_s s$) như các phần tử của đại số hạn chế của S; dĩ nhiên ký hiệu tổng xuất hiện trong ký hiệu này không tương ứng với phép toán đại số nào vì nói chung nó được lấy trên một *vô hạn* số hạng $\neq 0$. Với ký hiệu này, phép nhân trong đại số toàn phần của S cũng được cho bởi công thức (35) của no. 6.

Nếu S giao hoán thì đại số toàn phần $A^S$ của nó cũng giao hoán. Nếu T là một monoid con của S, đại số toàn phần $A^T$ của monoid được đồng nhất một cách chính tắc với một đại số con của đại số toàn phần của S. Nếu $\rho : A \to B$ là một đồng cấu vành, mở rộng chính tắc $\rho^S : A^S \to B^S$ là một A-đồng cấu từ đại số toàn phần của S trên A vào đại số toàn phần của S trên B, mở rộng đồng cấu chính tắc $A^{(S)} \to B^{(S)}$.

### 11. CHUỖI LŨY THỪA HÌNH THỨC TRÊN MỘT VÀNH GIAO HOÁN

Với mọi tập hợp I, monoid cộng tính $N^{(I)}$ thỏa mãn điều kiện (D) của no. 10; thật vậy, nếu $s = (n_i)_{i\in I}$ với $n_i = 0$ trừ các chỉ số $i$ trong một tập con hữu hạn H của I, quan hệ $s = t + u$ với $t = (p_i)_{i\in I}$ và $u = (q_i)_{i\in I}$ tương đương với $p_i + q_i = n_i$ với mọi $i$; nhưng điều này suy ra $p_i = q_i = 0$ với $i \notin H$ và $p_i \leq n_i, q_i \leq n_i$ với $i \in H$; do đó có $\prod_{i\in H} (n_i + 1)$ cặp có thứ tự $(t, u)$ trong $N^{(I)}$ sao cho $t + u = s$.

Do đó ta có thể xét đại số toàn phần của monoid $\mathbf{N}^{(I)}$ trên $A$, đại số này chứa đại số (hạn chế) $A[\mathbf{X}_i]_{i \in I}$ của monoid này. Đó là một đại số có đơn vị giao hoán kết hợp được gọi là đại số các chuỗi lũy thừa hình thức theo các bất định $X_i \ (i \in I)$ với hệ số trong $A$ và được ký hiệu bởi $A[[\mathbf{X}_i]]_{i \in I}$; các phần tử của nó được gọi là các chuỗi lũy thừa hình thức theo các bất định $X_i \ (i \in I)$ với hệ số trong $A$. Một phần tử như vậy $(\alpha_v)_{v \in \mathbf{N}^{(I)}}$ cũng được ký hiệu, theo quy ước đã nêu ở no. 10, bởi $\sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v$; các $\alpha_v$ là các hệ số của chuỗi lũy thừa hình thức và các $\alpha_v X^v$ là các số hạng của nó; do đó một đa thức theo các $X_i$ là một chuỗi lũy thừa hình thức chỉ có một số hữu hạn số hạng $\neq 0$.

Rõ ràng một đẳng cấu đại số $A[[\mathbf{X}_i]]_{i \in I_1} \to A[[\mathbf{X}_i]]_{i \in I_2}$ được dẫn xuất một cách chính tắc từ mọi song ánh $\sigma : I_1 \to I_2$ bằng cách ánh xạ chuỗi lũy thừa hình thức $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_i^{n_i}$ thành chuỗi lũy thừa hình thức $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_{\sigma(i)}^{n_i}$.

Cho $J$ là một tập con của $I$; đại số $A[[\mathbf{X}_i]]_{i \in J}$ có thể được đồng nhất với một đại số con của $A[[\mathbf{X}_i]]_{i \in I}$ gồm các chuỗi lũy thừa hình thức $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ trong đó $\alpha_{(n_i)} = 0$ đối với mọi phần tử $(n_i) \in \mathbf{N}^{(I)}$ sao cho $n_i \neq 0$ với ít nhất một chỉ số $i \in I - J$. Hơn nữa, nếu $K = I - J$, thì $A[[\mathbf{X}_i]]_{i \in I}$ được đồng nhất một cách chính tắc với $(A[[\mathbf{X}_j]]_{j \in J})[[\mathbf{X}_k]]_{k \in K}$, bằng cách đồng nhất chuỗi lũy thừa hình thức $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ với chuỗi lũy thừa hình thức $\sum_{(m_k)} \beta_{(m_k)} \cdot \prod_{k \in K} X_k^{m_k}$, trong đó
$$
\beta_{(m_k)} = \sum_{(p_j)} \gamma_{(p_j)} \cdot \prod_{j \in J} X_j^{p_j}
$$
với $\gamma_{(p_j)} = \alpha_{(n_i)}$ đối với dãy $(n_i)$ sao cho $n_i = p_i$ với $i \in J$ và $n_i = m_i$ với $i \in K$.

Cho một chuỗi lũy thừa hình thức $u = \sum_v \alpha_v X^v$, các số hạng $\alpha_v X^v$ sao cho $|v| = p$ được gọi là các số hạng trong $u$ có bậc toàn phần $p$. Chuỗi lũy thừa hình thức $u_p$ mà các số hạng có bậc toàn phần $p$ là các số hạng của $u$ còn các số hạng khác thì bằng không, được gọi là phần thuần nhất của $u$ bậc $p$; khi $I$ là hữu hạn, $u_p$ là một đa thức với mọi $p$; $u_0$ được đồng nhất với một phần tử của $A$ (cũng được gọi là số hạng hằng của $u$). Nếu $u$ và $v$ là hai chuỗi lũy thừa hình thức và $w = uv$, thì
$$
w_p = \sum_{r=0}^p u_r v_{p-r}
$$
đối với mọi số nguyên $p \geq 0$.

Đối với mọi chuỗi lũy thừa hình thức $u \neq 0$, số nguyên nhỏ nhất $p \geq 0$ sao cho $u_p \neq 0$ được gọi là cấp toàn phần (hoặc đơn giản là cấp) của $u$. Nếu cấp này được ký hiệu là $\omega(u)$ và $u$ và $v$ là hai chuỗi lũy thừa hình thức $\neq 0$, thì
$$
\omega(u + v) \geq \inf(\omega(u), \omega(v)) \quad \text{nếu } u + v \neq 0 \\
\omega(uv) \geq \omega(u) + \omega(v) \quad \text{nếu } uv \neq 0.
$$

Hơn nữa, nếu $\omega(u) \neq \omega(v)$, thì tất yếu $u + v \neq 0$ và hai vế của (40) bằng nhau.

Chú ý rằng cấp của 0 *không được xác định*. Theo một sự lạm dụng ngôn ngữ, theo quy ước người ta nói rằng "f là một chuỗi lũy thừa hình thức có cấp $\geq p$ (tương ứng $> p$)" nếu phần thuần nhất bậc n của f bằng không với mọi $n < p$ (tương ứng $n \leq p$); do đó 0 là một "chuỗi lũy thừa hình thức có cấp $> p$" với *mọi* số nguyên $p \geq 0$.

Cho J là một tập con của I và đồng nhất $A[[X_i]]_{i \in I}$ như trên với $B[[X_k]]_{k \in K}$, trong đó $K = I - J$ và $B = A[[X_j]]_{j \in J}$; tương ứng với các định nghĩa trên được áp dụng cho $B[[X_k]]_{k \in K}$, có các định nghĩa mới cho các chuỗi lũy thừa hình thức $u \in A[[X_i]]_{i \in I}$; một số hạng $\alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ được gọi là *có bậc p theo các $X_i$ có chỉ số* $i \in K$ nếu $\sum_{i \in K} n_i = p$ và chuỗi lũy thừa hình thức của $B[[X_k]]_{k \in K}$ có cùng các số hạng bậc $p$ như $u$ và các số hạng khác bằng không được *gọi là phần thuần nhất bậc p theo các $X_i$ có chỉ số* $i \in K$. Nếu $u \neq 0$, *cấp* $\omega_K(u)$ đối với các $X_i$ có chỉ số $i \in K$ là số nhỏ nhất trong các số nguyên $p \geq 0$ sao cho phần thuần nhất của $u$ bậc $p$ theo các $X_i$ có chỉ số $i \in K$ là $\neq 0$. Các bất đẳng thức (40) và (41) vẫn còn đúng khi thay $\omega$ bằng $\omega_K$.

### Bài tập {#alg-iii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
