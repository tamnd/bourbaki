---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 2
section_title: Flat modules
lang: vi
source: ac-i-vii
book_pages: 9-27, 41-49
pdf_pages: 0029-0047, 0061-0069
extraction: ocr
subsections:
    - "no": 1
      title: REVISION OF TENSOR PRODUCTS
      page: 9
      pdf_page: 29
    - "no": 2
      title: M-FLAT MODULES
      page: 10
      pdf_page: 30
    - "no": 3
      title: FLAT MODULES
      page: 12
      pdf_page: 32
    - "no": 4
      title: EXAMPLES OF FLAT MODULES
      page: 14
      pdf_page: 34
    - "no": 5
      title: FLATNESS OF QUOTIENT MODULES
      page: 15
      pdf_page: 35
    - "no": 6
      title: INTERSECTION PROPERTIES
      page: 17
      pdf_page: 37
    - "no": 7
      title: TENSOR PRODUCTS OF FLAT MODULES
      page: 19
      pdf_page: 39
    - "no": 8
      title: FINITELY PRESENTED MODULES
      page: 20
      pdf_page: 40
    - "no": 9
      title: EXTENSION OF SCALARS IN HOMOMORPHISM MODULES
      page: 22
      pdf_page: 42
    - "no": 10
      title: 'EXTENSION OF SCALARS: CASE OF COMMUTATIVE RINGS'
      page: 22
      pdf_page: 42
    - "no": 11
      title: INTERPRETATION OF FLATNESS IN TERMS OF RELATIONS (*)
      page: 25
      pdf_page: 45
statements: 37
exercises: 24
content_sha256: 46703582e490494ae14604a14446f76d5d0b9a87ea22388f84989197512c6261
translated_from: content/en/ac/I/02_s2_flat_modules.md
source_content_sha256: 9ada776b7c0aa973a418227eaada671c4629e279b41b24c1ad82f46743b38d27
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-e41856f7
glossary_version: 34
glossary_terms_sha256: 91dde6875552f34b49bc11deffc5199fbc403efa40094708be1c646c1c540c70
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. MÔĐUN PHẲNG(*)

### 1. NHẮC LẠI VỀ TÍCH TENXƠ

Cho A là một vành, E là một A-môđun phải và M là một A-môđun trái. Trong Đại số, Chương II, §3, no. 1, chúng tôi đã định nghĩa tích tenxơ $E \otimes_A M$, là một $\mathbf{Z}$-môđun. Nếu E' (tương ứng M') là một A-môđun phải (tương ứng trái) và $u : E \to E'$ (tương ứng $v : M \to M'$) là một đồng cấu, chúng tôi cũng đã định nghĩa (loc. cit, no. 2) một $\mathbf{Z}$-đồng cấu

$$
u \otimes v : E \otimes_A M \to E' \otimes_A M'.
$$

#### Bổ đề 1 {#ac-i-s2-lem-1 .statement}

*Cho* $M' \xrightarrow{v} M \xrightarrow{w} M'' \to 0$ *là một dãy khớp các A-môđun trái và E là một A-môđun phải. Khi đó dãy*

$$
E \otimes_A M' \xrightarrow{\text{1}\otimes v} E \otimes_A M \xrightarrow{u \otimes w} E \otimes_A M'' \longrightarrow 0
$$

*là một dãy khớp các nhóm giao hoán.*

Đây là Hệ quả của Mệnh đề 5 trong Đại số, Chương II, § 3, no. 6.

Suy ra rằng, với mọi đồng cấu A-môđun trái $u : M \to N$,

$$
E \otimes_A (\operatorname{Coker} u)
$$

được đồng nhất một cách chính tắc với $\operatorname{Coker}(1_E \otimes u)$, như Bổ đề 1 cho thấy khi áp dụng cho dãy khớp

$$
M \xrightarrow{u} N \longrightarrow \operatorname{Coker} u \longrightarrow 0.
$$

Theo ký hiệu của Bổ đề 1, ta biết (loc. cit.) rằng nếu v là *đơn ánh*, nghĩa là nếu dãy $0 \to M' \xrightarrow{v} M \xrightarrow{w} M'' \to 0$ là khớp, thì không nhất thiết suy ra rằng $1_E \otimes v$ là đơn ánh và do đó nói chung không thể đồng nhất $E \otimes_A M'$ với một

(*) Chúng tôi thông báo với những độc giả đã quen thuộc với Đại số đồng điều rằng họ sẽ tìm thấy các đặc trưng khác của môđun phẳng trong § 4.

nhóm con của $E \otimes_A M$. Tuy nhiên, hãy nhắc lại (Đại số, Chương II, § 3, no. 7, Hệ quả 5 của Mệnh đề 7) kết quả sau đây:

#### Bổ đề 2 {#ac-i-s2-lem-2 .statement}

*Nếu $v : M' \to M$ là đơn ánh và $v(M')$ là một nhân tử trực tiếp của $M$, thì đồng cấu $1, \otimes v$ là đơn ánh và ảnh của nó là một nhân tử trực tiếp của $E \otimes_A M$.*

### 2. MÔĐUN PHẲNG ĐỐI VỚI M

#### Định nghĩa 1 {#ac-i-s2-def-1 .statement}

Cho $A$ là một vành, $E$ là một A-môđun phải và $M$ là một A-môđun trái. Ta nói $E$ là phẳng đối với $M$ (hay $M$-phẳng) nếu, với mọi A-môđun trái $M'$ và mọi đơn cấu $v : M' \to M$, đồng cấu $l_E \otimes v : E \otimes_A M' \to E \otimes_A M$ là đơn ánh.

Với mọi A-môđun phải $N$, khái niệm môđun trái $N$-phẳng được định nghĩa tương tự. Nói rằng một A-môđun phải $E$ là phẳng đối với một A-môđun trái $M$ là tương đương với việc nói rằng $E$, được xét như một A$^0$-môđun trái (nhắc lại rằng $A^0$ ký hiệu vành đối của $A$), là phẳng đối với A$^0$-môđun phải $M$.

#### Bổ đề 3 {#ac-i-s2-lem-3 .statement}

*Để một A-môđun phải $E$ là $M$-phẳng, điều kiện cần và đủ là với mọi môđun con sinh hữu hạn $M'$ của $M$, đồng cấu chính tắc*

$$
l_E \otimes j : E \otimes_A M' \to E \otimes_A M
$$

(*j là đơn ánh chính tắc $M' \to M$) *là đơn ánh*.

Giả sử điều kiện này được thỏa mãn và N là một môđun con bất kỳ của $M$. Giả sử ảnh chính tắc trong $E \otimes_A M$ của một phần tử

$$
z = \sum x_i \otimes y_i \in E \otimes_A N \quad (x_i \in E, y_i \in N)
$$

là không và cho $M'$ là môđun con sinh hữu hạn của $N$ được sinh bởi chúng.; vì theo giả thiết ánh xạ hợp
$E \otimes_A M' \to E \otimes_A N \to E \otimes_A M$ là đơn ánh, tổng $z' = \sum x_i \otimes y_i$, được xem như một phần tử của $E \otimes_A M'$, là không. *Vì* $z$ là ảnh của $z'$, ta cũng có $z = 0$, do đó bổ đề được chứng minh.

#### Bổ đề 4 {#ac-i-s2-lem-4 .statement}

*Cho $E$ là một $A$-môđun phải và $M$ là một $A$-môđun trái sao cho $E$ là $M$-phẳng. Nếu $N$ là môđun con hoặc môđun thương của $M$, thì $E$ là $N$-phẳng.*

Trường hợp $N$ là một môđun con là hiển nhiên, vì nếu $N'$ là một môđun con của $N$, đồng cấu hợp

$$
E \otimes_A N' \to E \otimes_A N \to E \otimes_A M
$$

là đơn ánh, do đó $E \otimes_A N' \to E \otimes_A N$ cũng là đơn ánh. Giả sử khi đó $N$ là một môđun thương của $M$, nghĩa là tồn tại một dãy khớp $0 \to R \xrightarrow{i} M \xrightarrow{p} N \to 0$.

Cho $N'$ là một môđun con của $N$ và $M' = \overline{p}(N')$. Ký hiệu $i'$ là ánh xạ của $R$ vào $M'$ có cùng đồ thị với $i$, $p'$ là toàn ánh $M \to N'$ có cùng đồ thị với hạn chế của $p$ lên $M'$, $r$ là ánh xạ đồng nhất của $\mathbf{R}$ vào $\mathbf{R}$, $m$ là đơn ánh chính tắc $M' \to M$ và $n$ là đơn ánh chính tắc $N' \to N$. Biểu đồ

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & \mathbf{R} & \xrightarrow{i'} & M' & \xrightarrow{p'} & N' & \longrightarrow & 0 \\
& & \downarrow r & & \downarrow m & & \downarrow n & & \\
0 & \longrightarrow & \mathbf{R} & \xrightarrow{i} & M & \xrightarrow{p} & N & \longrightarrow & 0
\end{array}
$$

là giao hoán và các dòng của nó là khớp.

Để đơn giản hóa cách viết, ta đặt $T(Q) = E \otimes_A Q$ với mọi $A$-môđun trái $Q$ và $T(v) = 1_E \otimes v$ với mọi đồng cấu $A$-môđun trái $v$. Biểu đồ

$$
\begin{array}{ccccccccc}
T(\mathbf{R}) & \xrightarrow{T(i')} & T(M') & \xrightarrow{T(p')} & T(N') & \longrightarrow & 0 \\
\downarrow T(r) & & \downarrow T(m) & & \downarrow T(n) & & \\
T(\mathbf{R}) & \xrightarrow{T(i)} & T(M) & \xrightarrow{T(p)} & T(N) & \longrightarrow & 0
\end{array}
$$

là giao hoán và các dòng của nó là khớp theo Bổ đề 1 của no. 1. Hơn nữa, vì $E$ là $M$-phẳng, đồng cấu $T(m)$ là đơn ánh. Vì $T(r)$ và $T(p')$ là toàn ánh, suy ra từ § 1, no. 4, Hệ quả 2 của Mệnh đề 2 rằng $T(n)$ là đơn ánh, điều này chứng minh bổ đề.

#### Bổ đề 5 {#ac-i-s2-lem-5 .statement}

Cho $(M_i)_{i \in I}$ là một họ các $A$-môđun trái, $M = \bigoplus_{i \in I} M_i$, tổng trực tiếp của chúng và $E$ là một $A$-môđun phải. Nếu, với mọi $i \in I$, $E$ phẳng đối với $M_i$, thì $E$ phẳng đối với $M$.

(a) Trước hết giả sử rằng $I = \{1, 2\}$, và cho $M'$ là một môđun con của $M = M_1 \oplus M_2$, $M$, và $M$, được đồng nhất một cách chính tắc với các môđun con của $M$. Ký hiệu $M'_1$ là giao $M' \cap M_1$, và $M'_2$ là ảnh của $M'$ trong $M_2$ qua phép chiếu chính tắc $p$ của $M$ lên $M_2$. Ta có một biểu đồ

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & M'_1 & \xrightarrow{i'} & M' & \xrightarrow{p'} & M'_2 & \longrightarrow & 0 \\
& & \downarrow v_1 & & \downarrow v & & \downarrow v_2 & & \\
0 & \longrightarrow & M_1 & \xrightarrow{i} & M & \xrightarrow{p} & M_2 & \longrightarrow & 0
\end{array}
$$

trong đó $v_1, v, v_2, i, i'$ là các đơn cấu chính tắc và $p'$ là ánh xạ có cùng đồ thị với hạn chế của $p$ lên $M'$, ánh xạ này là toàn ánh. Ta kiểm tra ngay lập tức rằng biểu đồ này giao hoán và các hàng của nó là khớp. Với $T(Q)$ và $T(v)$ được dùng cùng nghĩa như trong chứng minh của Bổ đề 4, ta có một biểu đồ giao hoán

$$
\begin{array}{ccccccccc}
T(M'_1) & \xrightarrow{T(i')} & T(M') & \xrightarrow{T(p')} & T(M'_2) \\
\downarrow T(v_1) & & \downarrow T(v) & & \downarrow T(v_2) \\
T(M_1) & \xrightarrow{T(i)} & T(M) & \xrightarrow{T(p)} & T(M_2)
\end{array}
$$

Theo Bổ đề 1 của no. 1, hai hàng của biểu đồ này là khớp; vì E phẳng đối với $M_1$ và $M_n$, $T(v_1)$ và $T(v_2)$ là đơn ánh; hơn nữa, theo Bổ đề 2 của no. 1, $T(i)$ là đơn ánh. Hệ quả 2 của Mệnh đề 2 của § 1, no. 4 khi đó cho thấy rằng $T(v)$ là đơn ánh và do đó E là M-phẳng.

(b) Nếu I là một tập con hữu hạn có n phần tử, bổ đề suy ra bằng quy nạp theo n sử dụng (a).

(c) Trong trường hợp tổng quát, cho $M'$ là một môđun con sinh hữu hạn của M. Khi đó tồn tại một tập con hữu hạn J của tập chỉ số I sao cho $M'$ được chứa trong tổng trực tiếp $M_J = \bigoplus_{i \in J} M_i$. Theo (b) E phẳng đối với $M_J$; đồng cấu chính tắc $E \otimes_A M' \to E \otimes_A M$, do đó là đơn ánh. Mặt khác, vì $M_J$ là một nhân tử trực tiếp của M, đồng cấu chính tắc $E \otimes_A M_J \to E \otimes_A M$ là đơn ánh (no. 1, Bổ đề 2). Lấy hợp thành, suy ra rằng $E \otimes_A M, \to E \otimes_A M$ là đơn ánh và E phẳng đối với M theo Bổ đề 3.

### 3. MÔĐUN PHẲNG

#### Mệnh đề 1 {#ac-i-s2-prop-1 .statement}

Cho E là một A-môđun phải. Ba tính chất sau là tương đương:

(a) E phẳng đối với A, (nói cách khác, với mọi iđêan trái $a$ của A, đồng cấu chính tắc $E \otimes_A a \to E \otimes_A A, = E$ là đơn ánh).
(b) E là M-phẳng đối với mọi A-môđun trái M.
(c) Với mọi dãy khớp của các A-môđun trái và các đồng cấu

$$
M' \xrightarrow{v} M \xrightarrow{w} M''
$$

dãy

$$
E \otimes_A M' \xrightarrow{1 \otimes v} E \otimes_A M \xrightarrow{1 \otimes w} E \otimes_A M''
$$

là khớp.

Hiển nhiên rằng (b) kéo theo (a). Ngược lại, giả sử rằng (a) đúng; theo Bổ đề 5 của no. 2, E phẳng đối với mọi A-môđun trái tự do; vì mọi A-môđun trái đều đẳng cấu với một thương của một môđun tự do (Đại số, Chương 11, § 1, no. 11, Mệnh đề 20), suy ra từ Bổ đề 4 của no. 2 rằng E phẳng đối với M.

Ta chứng minh rằng (c) kéo theo (b). Nếu $v : M' \to M$ là một đơn cấu, dãy $0 \to M' \xrightarrow{v} M$ là khớp; theo (c) dãy

$$
0 \to E \otimes_A M' \xrightarrow{1 \otimes v} E \otimes_A M
$$

là khớp; điều này có nghĩa là $1 \otimes v$ là đơn ánh, nói cách khác, E là M-phẳng.

Cuối cùng, kéo theo (b) $\Rightarrow$ (c) là một hệ quả của bổ đề chính xác hơn sau đây:

#### Bổ đề 6 {#ac-i-s2-lem-6 .statement}

*Nếu $M' \xrightarrow{v} M \xrightarrow{w} M''$ là một dãy khớp của các A-môđun trái và nếu E là một A-môđun phải $M''$-phẳng, dãy*

$$
E \otimes_A M' \xrightarrow{1 \otimes v} E \otimes_A M \xrightarrow{1 \otimes w} E \otimes_A M''
$$

*là khớp.*

Chúng tôi dùng ký hiệu $T(Q)$ và $T(v)$ theo cùng nghĩa như trong chứng minh của Bổ đề 4 của no. 2. Ta viết $M_1'' = w(M)$ và gọi $i : M_1'' \to M''$ là đơn ánh chính tắc và $p$ là ánh xạ từ M tới $M_1''$ có cùng đồ thị với w. Dãy $M' \xrightarrow{v} M \xrightarrow{p} M_1'' \to 0$ là khớp và suy ra từ Bổ đề 1 của no. 1 rằng dãy

$$
T(M') \xrightarrow{T(v)} T(M) \xrightarrow{T(p)} T(M_1'') \longrightarrow 0
$$

là khớp. Hơn nữa, vì E là $M''$-phẳng, ánh xạ $T(i) : T(M_1'') \to T(M'')$ là đơn ánh, và vì $T(i) \circ T(p) = T(w)$, dãy

$$
T(M') \xrightarrow{T(v)} T(M) \xrightarrow{T(w)} T(M'')
$$

*là khớp.* (\S 1, no. 3.)

#### Định nghĩa 2 {#ac-i-s2-def-2 .statement}

*Một A-môđun phải E được gọi là phẳng nếu* nó có các tính chất tương đương của Mệnh đề 1.

Các A-môđun trái phẳng được định nghĩa tương tự. Nói rằng một A-môđun phải E là phẳng tương đương với nói rằng E, được xét như một $A^0$-môđun trái, là phẳng.

Nhận xét

(1) Theo Bổ đề 3 của no. 2, để một A-môđun phải E là phẳng, điều kiện cần và đủ là, với mọi iđêan trái *hữu hạn* sinh $a$ của A, ánh xạ chính tắc $E \otimes_A a \to E$ (Mệnh đề 1) có ảnh là Ea phải là đơn ánh.

(2) Cho E là một A-môđun phải phẳng. Nếu $M'$ là một môđun con của một A-môđun trái M, đơn ánh chính tắc $E \otimes_A M' \to E \otimes_A M$ cho phép ta đồng nhất $E \otimes_A M'$ với một nhóm con của $E \otimes_A M$. Như vậy, cho N là một A-môđun trái, $u : M \to N$ một đồng cấu, $K = \mathrm{Ker}\, u$, và $I = \mathrm{Im}\, u$. Xét dãy khớp

$$
0 \longrightarrow K \longrightarrow M \xrightarrow{u} N
$$

ta dễ thấy (Mệnh đề 1) rằng $E \otimes_A (\mathrm{Ker}\, u)$ *được đồng nhất* với $\mathrm{Ker}(1_E \otimes u)$. Mặt khác, ký hiệu $u'$ là đồng cấu toàn ánh $M \to I$ có cùng đồ thị với $u$, và $i$ là đơn ánh chính tắc $I \to N$, thì $1_E \otimes u'$ là toàn ánh (no. 1, Bổ đề 1) và $1_E \otimes i$ là đơn ánh vì E là phẳng. Vì

$$
1_E \otimes u = (1_E \otimes i) \circ (1_E \otimes u'),
$$

$E \otimes_A (\mathrm{Im}\, u)$ *được đồng nhất* với $\mathrm{Im}(1_E \otimes u)$.

#### Mệnh đề 2 {#ac-i-s2-prop-2 .statement}

(i) Cho $(E_t)_{t \in I}$ là một họ các $A$-môđun phải. Để $E = \bigoplus_{t \in I} E_t$ là phẳng, điều kiện cần và đủ là mỗi $E_t$ đều phẳng.

(ii) Cho $I$ là một tập hợp có thứ tự và $(E_\alpha, f_{\beta \alpha})$ là một hệ trực tiếp các $A$-môđun phải (Đại số, Chương II, § 6, no. 2). Nếu mỗi $E_\alpha$ đều phẳng, thì $E = \lim_{\longrightarrow} E_\alpha$ là phẳng.

Cho $M' \to M$ là một đồng cấu đơn ánh của A-môđun trái.

(i) Để đồng cấu tổng trực tiếp
$$
\bigoplus_{t \in I} (E_t \otimes_A M') \to \bigoplus_{t \in I} (E_t \otimes_A M)
$$
là khớp, điều kiện cần và đủ là mỗi đồng cấu $E_t \otimes_A M' \to E_t \otimes_A M$ đều như vậy (Đại số, Chương II, § 1, no. 6, Hệ quả 1 của Mệnh đề 7), điều này chứng minh (i) vì $\bigoplus_{t \in I} (E_t \otimes_A M)$ được đồng nhất một cách chính tắc với $E \otimes_A M$ (Đại số, Chương II, § 3, no. 7, Mệnh đề 7).

(ii) Theo giả thiết, mỗi dãy
$$
0 \to E_\alpha \otimes_A M' \to E_\alpha \otimes_A M
$$
đều khớp; do đó dãy
$$
0 \to E \otimes_A M' \to E \otimes_A M
$$
cũng khớp, vì việc lấy giới hạn trực tiếp giao hoán với tích tenxơ (Đại số, Chương II, § 6, no. 3, Mệnh đề 7) và bảo toàn tính khớp (ibid., § 6, no. 2, Mệnh đề 3).

### 4. VÍ DỤ VỀ CÁC MÔĐUN PHẲNG

(1) Với mọi vành $A$, hiển nhiên $A$ là một $A$-môđun phẳng (Đại số, Chương II, § 3, no. 4, Mệnh đề 4). Khi đó suy ra từ Mệnh đề 2, (i) của no. 3 rằng mọi $A$-môđun phải tự do, và tổng quát hơn mọi $A$-môđun phải xạ ảnh (Đại số, Chương 11, § 2, no. 2), đều là các $A$-môđun phẳng.

(2) Nếu $A$ là một vành nửa đơn (Đại số, Chương VIII, § 5, no. 1, Định nghĩa 1) thì mọi $A$-môđun phải $E$ đều là nửa đơn và do đó là tổng trực tiếp của các môđun đơn; vì mỗi môđun sau này đẳng cấu với một nhân tử trực tiếp của $A$, (cùng chỗ, § 5, no. 1, Mệnh đề 6), $E$ là xạ ảnh và do đó phẳng theo (1) (xem Bài tập 16).

*(3) Trong các Chương II và III, chúng ta sẽ nghiên cứu chi tiết hai ví dụ quan trọng về các $A$-môđun phẳng: các vành phân thức $S^{-1}A$ và các hoàn thành Hausdorff $\hat{A}$ của $A$ đối với các tôpô $S$-adic.*

#### Mệnh đề 3 {#ac-i-s2-prop-3 .statement}

Cho $A$ là một vành và $E$ là một $A$-môđun phải.

(i) Giả sử rằng $E$ là phẳng. Với mọi phần tử $a \in A$ không phải là một ước phải của $0(*)$, các quan hệ $x \in E,\ xa = 0$ kéo theo $x = 0$.

(*) Nhắc lại rằng một ước phải (tương ứng, trái) của 0 trong một vành $A$ là một phần tử $b \in A$ sao cho ánh xạ $x \mapsto xb$ (tương ứng, $x \mapsto bx$) không là đơn ánh.

Ta chứng minh (i). Cho $v : A, \to A$, là đồng cấu $A$-môđun trái $t \mapsto ta$; giả thiết kéo theo rằng $v$ là đơn ánh. Vì $E$ là phẳng, đồng cấu $1_E \otimes v : E \otimes_A A, \to E \otimes_A A$, cũng là đơn ánh. Khi $E \otimes_A A$, được đồng nhất một cách chính tắc với $E$, $1, \otimes v$ trở thành tự đồng cấu $x \mapsto xa$ của $E$. Do đó quan hệ $xa = 0$ kéo theo $x = 0$.

Ta chứng minh (ii). Theo (i), nếu $E$ là phẳng, $E$ là không xoắn. Ngược lại, cho $E$ là một $A$-môđun không xoắn; ta kiểm tra rằng, với mọi iđêan sinh hữu hạn $a$ của $A$, đồng cấu chính tắc $E \otimes_A a \to E$ là đơn ánh (no. 3, Nhận xét 1). Mệnh đề này là hiển nhiên nếu $a = (0)$; nếu không, theo giả thiết $a = Aa$ với một số $a \in A, a \neq 0$, và $t \mapsto ta$ khi đó là một đẳng cấu $v$ của $A$ lên $a$; dùng $i$ để ký hiệu đơn ánh chính tắc $a \to A$, $i \circ v$ là phép vị tự với tỉ số $a$ trên $E$ và là đơn ánh vì $E$ được giả sử là không xoắn. Khi đó $1, \otimes (i \circ v) = (1, \otimes i) \circ (1_E \otimes v)$; vì $1_E \otimes v$ là một đẳng cấu, $1, \otimes i$ là đơn ánh, điều này hoàn tất chứng minh.

#### Ví dụ {#ac-i-s2-n4-exa-1 .statement}

Áp dụng Mệnh đề 3 cho vành $\mathbf{Z}$, ta thấy rằng $\mathbf{Q}$ là một $\mathbf{Z}$-môđun phẳng, nhưng $\mathbf{Z}/n\mathbf{Z}$ (với $n \geq 2$) không phải là một $\mathbf{Z}$-môđun phẳng.

### 5. TÍNH PHẲNG CỦA CÁC MÔĐUN THƯƠNG

#### Mệnh đề 4 {#ac-i-s2-prop-4 .statement}

Cho $E$ là một A-môđun phải. Ba tính chất sau là tương đương:

(a) $E$ phẳng.
(b) Với mọi dãy khớp các A-môđun phải có dạng

(1)
$$
0 \longrightarrow G \xrightarrow{v} H \xrightarrow{w} E \longrightarrow 0
$$
và mọi A-môđun trái $F$, dãy

(2)
$$
0 \longrightarrow G \otimes_A F \xrightarrow{v \otimes 1} H \otimes_A F \xrightarrow{w \otimes 1} E \otimes_A F \longrightarrow 0
$$
là khớp.

(c) Tồn tại một dãy khớp (1), trong đó $H$ phẳng, sao cho dãy (2) là khớp với mọi A-môđun trái $F$ có dạng $A_s/a$, trong đó $a$ là một iđêan trái sinh hữu hạn của $A$.

Trước hết ta chỉ ra rằng (a) kéo theo (b). A-môđun trái $F$ đẳng cấu với một thương của một môđun tự do (Đại số, Chương II, § 1, no. 11, Mệnh đề 20); nói cách khác, ta có một dãy khớp

$$
0 \longrightarrow R \xrightarrow{i} L \xrightarrow{p} F \longrightarrow 0
$$

trong đó L là tự do. Xét biểu đồ

$$
\begin{array}{ccccccccc}
G \otimes R & \xrightarrow{v \otimes 1_R} & H \otimes R & \xrightarrow{w \otimes 1_R} & E \otimes R \\
\downarrow l_G \otimes i & & \downarrow l_H \otimes i & & \downarrow l_E \otimes i \\
G \otimes L & \xrightarrow{v \otimes 1_L} & H \otimes L & \xrightarrow{w \otimes 1_L} & E \otimes L \\
\downarrow l_G \otimes p & & \downarrow l_H \otimes p & & \\
G \otimes F & \xrightarrow{v \otimes 1_F} & H \otimes F
\end{array}
$$

(3)

Ngay lập tức suy ra rằng biểu đồ này giao hoán, và các hàng và cột của nó đều khớp theo Bổ đề 1 của no. 1; hơn nữa, vì $l_G \otimes p$ và $l_H \otimes p$ là toàn ánh (no. 1, Bổ đề 1), ta có $G \otimes F = \operatorname{Coker}(l_G \otimes i)$,

$$
H \otimes F = \operatorname{Coker}(l_H \otimes i);
$$

$w \otimes 1_1$ là toàn ánh (no. 1, Bổ đề 1); sau cùng, vì L là tự do và do đó phẳng, $v \otimes 1_L$ là đơn ánh. Như vậy có thể áp dụng biểu đồ rắn (\$ 1, no. 4, Mệnh đề 2, (iii)) để chứng minh sự tồn tại của một dãy khớp

(4) $$ \operatorname{Ker}(l_H \otimes i) \longrightarrow \operatorname{Ker}(l_E \otimes i) \xrightarrow{d} G \otimes F \xrightarrow{v \otimes 1_F} H \otimes F. $$

Do đó, nếu E phẳng thì $l_E \otimes i$ là đơn ánh, nói cách khác $\operatorname{Ker}(l_E \otimes i) = 0$, và dãy khớp (4) cho thấy $v \otimes 1_F$ là đơn ánh, vì thế dãy (2) là khớp (có kể đến Bổ đề 1 của no. 1).

Vì (b) hiển nhiên kéo theo (c), còn lại phải chứng minh rằng (c) kéo theo (a). Xét biểu đồ (3) trong trường hợp $\mathbf{R} = \mathbf{a}, \mathbf{L} = \mathbf{A}_s, \mathbf{F} = \mathbf{A}_s/\mathbf{a}$ và áp dụng dãy khớp (4). Theo giả thiết $v \otimes 1_F$ là đơn ánh, do đó $\operatorname{Im}(d) = 0$; hơn nữa, vì H phẳng, ta có $\operatorname{Ker}(1, @i) = 0$; khi đó tính khớp của dãy (4) suy ra $\operatorname{Ker}(l_E \otimes i) = 0$, nói cách khác, $1, \otimes i$ là đơn ánh và điều này chứng minh rằng E phẳng (no. 3, Nhận xét 1).

#### Mệnh đề 5 {#ac-i-s2-prop-5 .statement}

*Cho* $0 \to E' \xrightarrow{v} E \xrightarrow{w} E'' \to 0$ *là một dãy khớp các* $\mathbf{A}$*-môđun phải. Giả sử* $E''$ *phẳng. Khi đó,* *để* $E$ *phẳng, điều kiện cần và đủ là* $E'$ *phẳng.*

Cho $u : F' \to F$ là một đồng cấu đơn cấu của các $\mathbf{A}$-môđun trái. Xét biểu đồ

$$
\begin{array}{ccccccccc}
E' \otimes F' & \xrightarrow{v \otimes 1_{F'}} & E \otimes F' & \xrightarrow{w \otimes 1_{F'}} & E'' \otimes F' \\
\downarrow l_{E'} \otimes u & & \downarrow l_E \otimes u & & \downarrow l_{E''} \otimes u \\
E' \otimes F & \xrightarrow{v \otimes 1_F} & E \otimes F & \xrightarrow{w \otimes 1_F} & E'' \otimes F
\end{array}
$$

Nó giao hoán và các hàng của nó là khớp (no. 1, Bổ đề 1). Vì $E''$ phẳng, l_{E''} \otimes u là đơn ánh; hơn nữa, Mệnh đề 4 chứng minh rằng v \otimes 1_{F'}, và v \otimes 1, là đơn ánh. Do đó, nếu E phẳng, l_E \otimes u là đơn ánh, nên cũng vậy

$$(l_E \otimes u) \circ (v \otimes 1_{F'}) = (v \otimes 1_F) \circ (l_{E'} \otimes u);$$

suy ra l_{E'} \otimes u là đơn ánh và do đó E' phẳng. Ngược lại, nếu E' phẳng thì l_{E'} \otimes u là đơn ánh; khi đó từ § 1, no. 4, Hệ quả 1 của Mệnh đề 2 suy ra l_E \otimes u là đơn ánh và vì vậy E phẳng.

Nhận xét
(1) Có thể xảy ra trường hợp E và E' phẳng mà E'' thì không, như ví dụ các $\mathbf{Z}$-môđun E = \mathbf{Z}, E' = n\mathbf{Z}, E'' = \mathbf{Z}/n\mathbf{Z} (n \geq 2), cho thấy.
(2) Một môđun con của một môđun phẳng không nhất thiết là một môđun phẳng (Bài tập 3).

### 6. CÁC TÍNH CHẤT CỦA GIAO

#### Bổ đề 7 {#ac-i-s2-lem-7 .statement}

Cho E là một A-môđun phải, F là một A-môđun trái và F', F'' là hai môđun con của F sao cho F = F' + F''. Khi đó giao của các ảnh chính tắc của E \otimes F' và E \otimes F'' trong E \otimes F bằng ảnh chính tắc của E \otimes (F' \cap F'').

Xét biểu đồ

$$
\begin{array}{ccccccc}
0 & \longrightarrow & F' \cap F'' & \longrightarrow & F' & \longrightarrow & F'/(F' \cap F'') \longrightarrow 0 \\
& & \downarrow & & \downarrow & & \downarrow \\
0 & \longrightarrow & F'' & \longrightarrow & F' + F'' & \longrightarrow & (F' + F'')/F'' \longrightarrow 0
\end{array}
$$

trong đó các mũi tên không được chỉ rõ là các đơn cấu và toàn ánh chính tắc và j là đẳng cấu chính tắc được định nghĩa trong Đại số, Chương I, § 6, no. 13, Định lý 6. Biểu đồ này giao hoán và các hàng của nó là khớp. Ta suy ra (vì F = F' + F'') một biểu đồ giao hoán

$$
\begin{array}{ccc}
E \otimes (F' \cap F'') & \longrightarrow & E \otimes F' \longrightarrow E \otimes (F'/(F' \cap F'')) \\
\downarrow & & \downarrow \\
E \otimes F'' & \longrightarrow & E \otimes F \longrightarrow E \otimes (F/F'')
\end{array}
$$

Các hàng của biểu đồ này là khớp (no. 1, Bổ đề 1) và 1 \otimes j là một đẳng cấu. Mệnh đề của chúng ta khi đó là một trường hợp đặc biệt của § 1, no. 4, Mệnh đề 1, (i) (xem Bài tập 5).

#### Mệnh đề 6 {#ac-i-s2-prop-6 .statement}

Cho E là một A-môđun phải và F là một A-môđun trái sao cho E là F-phẳng. Với mọi môđun con F' của F, ta ký hiệu bởi \phi(F') ảnh của E \otimes F' qua ánh xạ chính tắc từ E \otimes F' đến E \otimes F (ánh xạ này đơn ánh theo Định nghĩa 1 của no. 2). Khi đó, nếu F', F'' là hai môđun con của F, ta có

$$\phi(F' \cap F'') = \phi(F') \cap \phi(F'').$$

Vì E là F-phẳng, $\phi(F' + F'')$ được đồng nhất với $E \otimes (F' + F'')$, và các môđun con $\phi(F')$, $\phi(F'')$ và $\phi(F' \cap F'')$ được đồng nhất tương ứng với các ảnh chính tắc của $E \otimes F'$, $E \otimes F''$ và $E \otimes (F' \cap F'')$ trong $E \otimes (F' + F'')$. Mệnh đề 6 suy ra từ Bổ đề 7.

#### Nhận xét 1 {#ac-i-s2-n6-rem-1 .statement}

Với các giả thiết của Mệnh đề 6, $E \otimes_A F'$ thường được đồng nhất với $\phi(F')$ đối với mọi môđun con $F'$ của $F$, điều này cho công thức
$$
E \otimes_A (F' \cap F'') = (E \otimes_A F') \cap (E \otimes_A F'').
$$

#### Mệnh đề 7 {#ac-i-s2-prop-7 .statement}

*Cho E là một A-môđun phải, E' là một môđun con của E, F là một A-môđun trái và F' là một môđun con của F. Giả sử rằng E/E' hoặc F/F' là phẳng. Khi đó ảnh chính tắc của $E' \otimes F'$ trong $E \otimes F$ là giao của các ảnh chính tắc của $E' \otimes F$ và $E \otimes F'$ trong $E \otimes F$.*

Giả sử chẳng hạn rằng $E/E'$ là phẳng và xét biểu đồ
$$
\begin{array}{ccc}
E' \otimes F' & \longrightarrow & E \otimes F' \\
\downarrow & & \downarrow \\
E' \otimes F & \longrightarrow & E \otimes F
\end{array}
$$
$$
\begin{array}{ccc}
& & (E/E') \otimes F' \\
E \otimes F' & \longrightarrow & (E/E') \otimes F
\end{array}
$$
trong đó các mũi tên là các đồng cấu chính tắc. Biểu đồ này là giao hoán và các hàng của nó là khớp (no. 1, Bổ đề 1). Vì $E/E'$ là phẳng, $u$ là đơn ánh. Khi đó mệnh đề của chúng ta là một trường hợp đặc biệt của § 1, no. 4, Mệnh đề 1, (i).

#### Hệ quả {#ac-i-s2-n6-cor-1 .statement}

Cho E là một A-môđun phải và E' là một môđun con của E.

(i) *Giả sử rằng E/E' là phẳng. Khi đó, với mọi iđêan trái a của A,
$$
E'a = E' \cap Ea.
$$
(ii) *Ngược lại, giả sử rằng E là phẳng và, với mọi iđêan trái sinh hữu hạn a của A, quan hệ (5) được thỏa mãn. Khi đó E/E' là phẳng.*

(i) Chỉ cần áp dụng Mệnh đề cho trường hợp $F = A$, $F' = a$.
(ii) Để chứng minh rằng $E/E'$ là phẳng, áp dụng tiêu chuẩn (c) của Mệnh đề 4 của no. 5; khi đó cần thiết lập rằng dãy
$$
0 \to E'/E'a \to E/Ea \to E/(E' + Ea) \to 0
$$
là khớp tại $E'/E'a$ đối với mọi iđêan trái sinh hữu hạn a của A. Bây giờ đây chính xác là điều mà quan hệ (5) biểu thị.

#### Nhận xét 2 {#ac-i-s2-n6-rem-2 .statement}

Kết luận của Mệnh đề 7 vẫn đúng nếu ta chỉ giả sử rằng $E/E'$ là F-phẳng hoặc rằng $F/F'$ là E-phẳng.

### 7. TÍCH TENXƠ CỦA CÁC MÔĐUN PHẲNG

Cho $A, B$ là hai vành, $E$ là một $A$-môđun phải và $F$ là một song môđun $(A,B)$ (*Đại số*, Chương II, § 1, no. 14). Nhắc lại (*Đại số*, Chương II, § 3, no. 4) rằng $E \otimes_A F$ có một cấu trúc $B$-môđun phải chính tắc, với cấu trúc đó

$$
(x \otimes y)b = x \otimes (yb) \quad \text{cho} \quad x \in E,\ y \in F,\ b \in B.
$$

#### Mệnh đề 8 {#ac-i-s2-prop-8 .statement}

*Cho $A, B$ là hai vành, $E$ là một $A$-môđun phải và $F$ là một song môđun $(A,B)$. Giả sử rằng $E$ là phẳng và rằng $F$ phẳng như một $B$-môđun. Khi đó $B$-môđun $E \otimes_A F$ là phẳng.*

Cho $G$ là một $B$-môđun trái và $G'$ là một môđun con của $G$. Vì $F$ là phẳng như một $B$-môđun phải, đồng cấu chính tắc $F \otimes_B G' \to F \otimes_B G$ là đơn ánh. Vì $E$ là phẳng, đồng cấu chính tắc

$$
E \otimes_A (F \otimes_B G') \to E \otimes_A (F \otimes_B G)
$$

là đơn ánh. Vì $E \otimes_A (F \otimes_B G')$ và $E \otimes_A (F \otimes_B G)$ lần lượt được đồng nhất một cách chính tắc với $(E \otimes_A F) \otimes_B G'$ và $(E \otimes_A F) \otimes_B G$ (*Algebra*, Chương II, § 3, no. 8, Mệnh đề 8), nên đồng cấu chính tắc

$$
(E \otimes_A F) \otimes_B G' \to (E \otimes_A F) \otimes_B G
$$

là đơn ánh, điều đó chứng minh rằng $E \otimes_A F$ là một $B$-môđun phẳng.

#### Hệ quả 1 {#ac-i-s2-prop-8-cor-1 .statement}

Cho $C$ là một vành giao hoán, $E, F$ là hai $C$-môđun phẳng. Khi đó $E \otimes_C F$ là một $C$-môđun phẳng.

$F$ là một $(C, C)$-song môđun và chỉ cần áp dụng Mệnh đề 8 với $B = A = C$.

#### Hệ quả 2 {#ac-i-s2-prop-8-cor-2 .statement}

*Cho $\rho$ là một đồng cấu từ một vành $A$ vào một vành $B$. Nếu $E$ là một $A$-môđun phải phẳng, thì $B$-môđun phải $\rho^*(E) = E_{(B)}$ thu được bằng cách mở rộng vành vô hướng lên $B$ (*Algebra*, Chương II, § 5, no. 1) là phẳng.*

Theo định nghĩa, $E_{(B)} = E \otimes_A B$, trong đó $B$ được xét như một $(A,B)$-song môđun nhờ $\rho$. Vì $B$-môđun phải $B_d$ là phẳng, chỉ cần áp dụng Mệnh đề 8.

#### Hệ quả 3 {#ac-i-s2-prop-8-cor-3 .statement}

*Cho $R, S$ là hai vành và $\phi : R \to S$ là một đồng cấu vành. Nếu $M$ là một $S$-môđun phải phẳng và $\phi_*(S_d)$ là một $R$-môđun phải phẳng, thì $\phi_*(M)$ là một $R$-môđun phải phẳng.*

Nhắc lại rằng $\phi_*(M)$ là $R$-môđun phải được xác định bởi $x.r = x.\phi(r)$ với mọi $x \in M$ và mọi $r \in R$ (*Algebra*, Chương II, § 1, no. 13). Khi đó áp dụng Mệnh đề 8 với $A = S, B = R, E = M$ và $F = S$, trong đó $S$ có cấu trúc của một $(S, R)$-song môđun xác định bởi $\phi$; khi ấy $R$-môđun phải $M \otimes_S S$ chính xác là $\phi_*(M)$.

#### Mệnh đề 9 {#ac-i-s2-prop-9 .statement}

*Cho $(A_\alpha, f_{\beta\alpha})$ là một hệ trực tiếp các vành, $A = \lim A_\alpha$ là giới hạn trực tiếp của nó, $(E_\alpha, f_{\beta\alpha})$ là một hệ trực tiếp các $A_\alpha$-môđun phải với cùng tập hợp chỉ số và $E = \lim E_\alpha$ là giới hạn trực tiếp của nó, đó là một $A$-môđun phải (Algebra, Chapter II, § 6, no. 2). Nếu với mỗi $\alpha$ thì $E_\alpha$ là một \&-môđun phẳng, thì $E$ là một $A$-môđun phẳng.*

Đặt $E'_\alpha = E_\alpha \otimes_{A_\alpha} A$, trong đó $A$ được xét như một $A_\alpha$-môđun trái thông qua đồng cấu chính tắc $A_\alpha \to A$; ta biết rằng A-môđun phải $E$ đẳng cấu chính tắc với $\lim E'_\alpha$ (*loc. cit.*, Hệ quả 2 của Mệnh đề 7). Từ Hệ quả 2 của Mệnh đề 8 suy ra rằng $E'_\alpha$ là một A-môđun phải phẳng với mọi $\alpha$, do đó $E$ là một A-môđun phẳng theo Mệnh đề 2 của no. 3.

### 8. MÔĐUN HỮU HẠN TRÌNH BÀY

Cho $A$ là một vành. Một dãy khớp
$$
L_1 \to L_0 \to E \to 0
$$
của các $A$-môđun trái (resp. phải), trong đó $L_0$ và $L_1$ là tự do, được gọi là một *trình bày* (hoặc *trình bày có độ dài* 1) của $A$-môđun trái (resp. phải) $E$.

Mọi A-môđun $E$ đều thừa nhận một trình bày. Thật vậy, ta biết (*Algebra*, Chương II, § 1, no. 11, Mệnh đề 20) rằng tồn tại một đồng cấu toàn ánh $u : L_0 \to E$, trong đó $L_0$ là tự do; nếu $R$ là hạt nhân của $u$, tương tự cũng tồn tại một đồng cấu toàn ánh $v : L_1 \to R$, trong đó $L_1$ là tự do. Nếu xem $v$ như một đồng cấu từ $L_1$ vào $L_0$, thì dãy $L_1 \xrightarrow{v} L_0 \xrightarrow{u} 0$ là khớp theo định nghĩa, do đó có mệnh đề của ta.

Nếu $\rho : A \to B$ là một đồng cấu vành, mọi trình bày (6) của $E$ sinh ra một trình bày của $E_{(B)} = E \otimes_A B$:
$$
L_1 \otimes_A B \to L_0 \otimes_A B \to E \otimes_A B \to 0
$$
theo Bổ đề 1 của no. 1 và thực tế rằng $L \otimes_A B$ là một B-môđun tự do nếu $L$ là tự do.

Một trình bày (6) của một môđun $E$ được gọi là *hữu hạn* nếu các môđun tự do $L_0$ và $L_1$ có các cơ sở hữu hạn. Rõ ràng, nếu trình bày (6) là hữu hạn thì trình bày (7) cũng vậy. $E$ được gọi là *một $A$-môđun hữu hạn trình bày* nếu nó thừa nhận một trình bày hữu hạn.

#### Bổ đề 8 {#ac-i-s2-lem-8 .statement}

(i) *Mọi môđun thừa nhận một trình bày hữu hạn đều sinh hữu hạn.*
(ii) *Nếu $A$ là một vành Noether trái, mọi A-môđun trái sinh hữu hạn đều thừa nhận một trình bày hữu hạn.*
(iii) *Mọi môđun xạ ảnh hữu hạn sinh đều thừa nhận một trình bày hữu hạn.*

Sau cùng, giả sử $E$ là một môđun xạ ảnh hữu hạn sinh; khi đó nó là một nhân tử trực tiếp của một môđun tự do hữu hạn sinh $L_0$ (*Algebra*, Chương II, §2, no. 2, Hệ quả của Mệnh đề 4); hạt nhân $R$ của đồng cấu toàn ánh $L_0 \to E$ khi đó đẳng cấu với một thương của $L_0$ và do đó sinh hữu hạn, và chứng minh được hoàn tất như đối với (ii).

#### Bổ đề 9 {#ac-i-s2-lem-9 .statement}

*Cho $A$ là một vành và $E$ là một $A$-môđun hữu hạn trình bày. Với mọi dãy khớp*

$$
0 \longrightarrow F \xrightarrow{j} G \xrightarrow{p} E \longrightarrow 0
$$

*trong đó $G$ sinh hữu hạn, môđun $F$ sinh hữu hạn.*

Cho $L, \xrightarrow{r} L_0 \xrightarrow{s} E \to 0$ là một trình bày hữu hạn; nếu $(e_i)$ là một cơ sở của $L_0$, thì với mỗi $i$ tồn tại một phần tử $g_i \in G$ sao cho $p(g_i) = s(e_i)$; khi đó đồng cấu $u : L_0 \to G$ xác định bởi $u(e_i) = g_i$ với mọi $i$ thỏa mãn $s = p \circ u$. Vì $s \circ r = 0$, ta có $u(r(L_1)) \subset \mathrm{Ker}\, p$, và vì $\mathrm{Ker}\, p$ đẳng cấu với $F$, suy ra có một đồng cấu $v : L, \to F$ sao cho biểu đồ

$$
\begin{array}{ccccccccc}
L, & \xrightarrow{r} & L_0 & \xrightarrow{s} & E & \longrightarrow & 0 \\
\downarrow v & & \downarrow u & & \downarrow 1_E & & \\
F & \xrightarrow{i} & G & \xrightarrow{p} & E & \longrightarrow & 0
\end{array}
$$

là giao hoán. Vì $j$ là đơn ánh và $s$ là toàn ánh, ta có thể áp dụng biểu đồ rắn ($\S$ 1, no. 4, Proposition 4), nói cách khác, có một dãy khớp

$$
0 = \mathrm{Ker}\, 1, \xrightarrow{d} \mathrm{Coker}\, v \longrightarrow \mathrm{Coker}\, u \longrightarrow \mathrm{Coker}\, 1, = 0.
$$

Điều này cho thấy $\mathrm{Coker}\, v$ đẳng cấu với $G / u(L_0)$, môđun này theo giả thiết là sinh hữu hạn. Hơn nữa ta có dãy khớp

$$
0 \to v(L_1) \to F \to \mathrm{Coker}\, v \to 0
$$

và vì $v(L_1)$ và $\mathrm{Coker}\, v$ là sinh hữu hạn, nên $F$ cũng vậy (*Algebra*, Chapter II, § 1, no. 7, Corollary 5 to Proposition 9).

### 9. MỞ RỘNG VÔ HƯỚNG TRONG CÁC MÔĐUN ĐỒNG CẤU

Cho $A$ và $B$ là hai vành, $E$ một $A$-môđun phải, $F$ một $B$-môđun phải và $G$ một $(B, A)$-song môđun. Nhắc lại rằng ta đã định nghĩa (Algebra, Chapter II, § 4, no. 2) một đồng cấu chính tắc của các $\mathbf{Z}$-môđun

$$
\nu : F \otimes_B \operatorname{Hom}_A(E, G) \to \operatorname{Hom}_A(E, F \otimes_B G)
$$

sao cho, với mọi $y \in F$ và $u \in \operatorname{Hom}_A(E, G)$, $\nu(y \otimes u)$ là ánh xạ $A$-tuyến tính $x \mapsto y \otimes u(x)$.

#### Mệnh đề 10 {#ac-i-s2-prop-10 .statement}

*Cho $A, B$ là hai vành, $E$ một $A$-môđun phải, $F$ một $B$-môđun phải và $G$ một $(B, A)$-song môđun. Giả sử rằng $F$ là phẳng. Khi đó, nếu $E$ sinh hữu hạn (tương ứng, có trình bày hữu hạn), thì đồng cấu chính tắc (8) là đơn ánh (tương ứng, song ánh).*

Coi $A, B, F, G$ là cố định và với mỗi $A$-môđun phải $E$ đặt

$$
T(E) = F \otimes_B \operatorname{Hom}_A(E, G), \quad T'(E) = \operatorname{Hom}_A(E, F \otimes_B G)
$$

và ký hiệu đồng cấu (8) bởi $\nu_E$; với mọi đồng cấu của các A-môđun phải $v : E \to E'$, đặt $T(v) = 1, \otimes \operatorname{Hom}(v, 1_G)$ và $T'(v) = \operatorname{Hom}(v, 1, \otimes 1_G)$. Cho $L, \xrightarrow{v} L_0 \xrightarrow{w} E \to 0$ là một trình bày của $E$; ta giả sử môđun tự do $L_0$ (tương ứng các môđun tự do $L_0$ và $L_1$) là *sinh hữu hạn*. Biểu đồ

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & T(E) & \xrightarrow{T(w)} & T(L_0) & \xrightarrow{T(v)} & T(L_1) \\
& & \downarrow{\nu_E} & & \downarrow{\nu_{L_0}} & & \downarrow{\nu_{L_1}} \\
0 & \longrightarrow & T'(E) & \xrightarrow{T'(w)} & T'(L_0) & \xrightarrow{T'(v)} & T'(L_1)
\end{array}
$$

là giao hoán và hàng thứ hai là khớp (Đại số, Chương II, § 2, no. 1, Định lý 1); hơn nữa, dãy

$$
0 \to \operatorname{Hom}_A(E, G) \to \operatorname{Hom}_A(L_0, G) \to \operatorname{Hom}_A(L_1, G)
$$

là khớp (*loc. cit.*), và vì $F$ *phẳng*, hàng thứ nhất của (9) cũng là một dãy khớp (no. 3, Mệnh đề 1). Khi đó ta biết rằng $\nu_{L_0}$ (tương ứng $\nu_{L_0}$ và $\nu_{L_1}$) là *song ánh* (tương ứng là *song ánh*) (Đại số, Chương II, § 4, no. 2, Mệnh đề 2). Nếu ta chỉ giả sử rằng $\nu_{L_0}$ là song ánh, thì từ (9) suy ra rằng

$$
\nu_{L_0} \circ T(w) = T'(w) \circ \nu_E
$$

là đơn ánh và do đó $\nu_E$ cũng vậy. Nếu ta giả sử cả $\nu_{L_0}$ và $\nu_{L_1}$ đều song ánh, thì từ § 1, no. 4, Hệ quả 2, (ii) của Mệnh đề 2 suy ra rằng $\nu_E$ là toàn ánh, và vì ta vừa thấy rằng $\nu_E$ là đơn ánh, nên nó là song ánh.

### 10. MỞ RỘNG VÔ HƯỚNG: TRƯỜNG HỢP CÁC VÀNH GIAO HOÁN

Bây giờ cho $A$ là một vành *giao hoán*, $B$ là một vành và $\rho : A \to B$ là một đồng cấu vành sao cho $\rho(A)$ được chứa trong *tâm* của $B$; nói cách khác, $\rho$ xác định trên $B$ một cấu trúc đại số trên A. Khi đó với mọi A-môđun E, B-môđun phải $E_{(B)} = E \otimes_A B$ được đồng nhất với $B \otimes_A E$, các cấu trúc A-môđun của $\rho_*(B_s)$ và $\rho_*(B_d)$ là đồng nhất theo giả thiết. Nhắc lại rằng với mọi cặp có thứ tự $(E, F)$ gồm các A-môđun, ta đã xác định một B-đồng cấu chính tắc

$$
\omega : (\operatorname{Hom}_A(E, F))_{(B)} \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

sao cho với mọi $u \in \operatorname{Hom}_A(E, F)$, $\omega(u \otimes 1) = u \otimes 1_B$ (Đại số, Chương II, § 5, no. 3).

#### Mệnh đề 11 {#ac-i-s2-prop-11 .statement}

Cho A là một vành giao hoán, B là một vành, $\varphi$ là một đồng cấu từ A vào tâm của B, và E và F là hai A-môđun. Giả sử rằng B là một A-môđun phẳng và E sinh hữu hạn (tương ứng trình bày hữu hạn). Khi đó đồng cấu chính tắc (10) là đơn ánh (tương ứng song ánh).

Vì $\omega$ là hợp thành của đẳng cấu chính tắc

$$
\operatorname{Hom}_A(E, B \otimes_A F) \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

và đồng cấu chính tắc (8)

$$
\nu : B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_A(E, B \otimes_A F)
$$

(*loc. cit.*), nên mệnh đề là hệ quả của Mệnh đề 10 của no. 9.

Bây giờ giả sử rằng A và B là giao hoán và xét ba A-môđun $E_1, E_2, E$, và một ánh xạ song tuyến tính A $f : E_1 \times E \to E_3$. Khi đó tồn tại một và chỉ một ánh xạ song tuyến tính B $f_B : E_{1(B)} \times E_{2(B)} \to E_{3(B)}$ sao cho

$$
f_B(1 \otimes x_1, 1 \otimes x_2) = 1 \otimes f(x_1, x_2)
$$

với mọi $x_1 \in E_1, x_2 \in E$, (Đại số, Chương IX, § 1, no. 4, Mệnh đề 1).

Trong mệnh đề tiếp theo ta sẽ giả sử rằng B là một A-môđun phẳng và, với mọi môđun con E' của $E_i$ ($i = 1, 2, 3$), ta sẽ đồng nhất một cách chính tắc $E'_{(B)}$ với ảnh của nó trong $E_{i(B)}$ (no. 3, Nhận xét 2).

#### Mệnh đề 12 {#ac-i-s2-prop-12 .statement}

Cho A, B là các vành giao hoán, $\varphi$ là một đồng cấu từ A vào B, $E_1, E_2, E_3$ là ba A-môđun, $f : E_1 \times E \to E_3$ là một ánh xạ song tuyến tính A và

$$
f_B : E_{1(B)} \times E_{2(B)} \to E_{3(B)}
$$

phần mở rộng của nó. Xét một môđun con $F_2$ của $E_2$, một môđun con $F_3$ của $E_3$, và ký hiệu bởi T môđun con của $E_1$ gồm những $x_1 \in E_1$ sao cho $f(x_1, x_2) \in F$, với mọi $x_2 \in F$. Giả sử rằng B là một A-môđun phẳng và $F_2$ sinh hữu hạn. Khi đó $T_{(B)}$ là tập hợp những $x'_1 \in E_{1(B)}$ sao cho $f_B(x'_1, x'_2) \in F_{3(B)}$ với mọi $x'_2 \in F_{2(B)}$.

Cho $p$ là toàn cấu chính tắc $E_3 \to E_3/F_3$; với mỗi $x_1 \in E_1$ ta gán ánh xạ A-tuyến tính $x_2 \mapsto p(f(x_1, x_2))$ từ $F_2$ vào $E_3/F_3$, và ký hiệu nó bởi $g(x_1)$; khi đó $g$ là một đồng cấu A của $E_1$ vào $\mathrm{Hom}_A(F_2, E_3/F_3)$ và hạt nhân của $g$ chính xác là T. Vì B là một A-môđun phẳng, ta có dãy khớp

$$
0 \longrightarrow T_{(B)} \longrightarrow E_{1(B)} \xrightarrow{1 \otimes g} (\mathrm{Hom}_A(F_2, E_3/F_3))_{(B)}
$$

(no. 3, Mệnh đề 1). Theo Mệnh đề 11, đồng cấu chính tắc

$$
\omega : (\mathrm{Hom}_A(F_2, E_3/F_3))_{(B)} \to \mathrm{Hom}_B(F_{2(B)}, (E_3/F_3)_{(B)})
$$

là *đơn ánh*. Mặt khác, vì B là một A-môđun phẳng, $(E_3/F_3)_{(B)}$ được đồng nhất một cách chính tắc với $E_{3(B)}/F_{3(B)}$; lấy hợp thành của $\omega$ với $1 \otimes g$, ta thu được một đồng cấu $u$ sao cho dãy

$$
0 \longrightarrow T_{(B)} \longrightarrow E_{1(B)} \xrightarrow{u} \mathrm{Hom}_B(F_{2(B)}, E_{3(B)}/F_{3(B)})
$$

là khớp. Ngay lập tức suy ra từ các định nghĩa rằng $u(x'_1)$, trong đó

$$
x'_1 = 1 \otimes x_1 \in E_{1(B)},
$$

là ánh xạ tuyến tính biến mỗi $x'_2 \in F_{2(B)}$ thành lớp mod. $F_{3(B)}$ của $f_B(x'_1, x'_2)$; theo tính tuyến tính, điều này cũng đúng với mọi $x'_1 \in E_{1(B)}$; vì hạt nhân của $u$ là $T_{(B)}$, mệnh đề được chứng minh.

#### Hệ quả 1 {#ac-i-s2-prop-12-cor-1 .statement}

*Cho A, B là hai vành giao hoán, $p : A \to B$ là một đồng cấu sao cho B là một A-môđun phẳng và E là một A-môđun hữu hạn trình bày. Với mọi môđun con sinh hữu hạn F của E, môđun con của đối ngẫu của $E_{(B)}$ trực giao với $F_{(B)}$ bằng $(F')_{(B)}$, trong đó $F'$ là môđun con của đối ngẫu $E^*$ của E trực giao với F.*

Theo Mệnh đề 11, $(E^*)_{(B)}$ đẳng cấu chính tắc với đối ngẫu $(E_{(B)})^*$ của $E_{(B)}$. Khi đó chỉ cần áp dụng Mệnh đề 12 với $E_1 = E^*$, $E_2 = E$, $E_3 = A$, $F_2 = F$, $F_3 = \{0\}$, và $f$ là dạng song tuyến tính chính tắc trên $E^* \times E$.

#### Hệ quả 2 {#ac-i-s2-prop-12-cor-2 .statement}

*Cho A, B là hai vành giao hoán, $p : A \to B$ là một đồng cấu sao cho B là một A-môđun phẳng và E là một A-môđun. Khi đó, với mọi môđun con sinh hữu hạn F của E, linh hóa tử của $F_{(B)}$ là iđêan $aB$ của B, trong đó a là linh hóa tử của F trong A.*

Chỉ cần áp dụng Mệnh đề 12 với $E_1 = A$, $E_2 = E_3 = E$, $F_2 = F$, $F_3 = \{0\}$.

#### Nhận xét {#ac-i-s2-n10-rem-1 .statement}

Nếu không có sự nhập nhằng nào về các môđun E, cũng như về ánh xạ song tuyến tính $f$, đôi khi người ta dùng $F_3 : F_2$ để chỉ môđun được ký hiệu bởi T trong Mệnh đề 12 và gọi nó là *bộ chuyển* của F, đến F,. Khi đó kết luận của Mệnh đề 12 được viết là

$$
F_{3(B)} : F_{2(B)} = (F_3 : F_2)_{(B)}.
$$

Trong trường hợp riêng khi các $E_i$ đều bằng vành $A, f$ là phép nhân và các $F_i$ là các iđêan $a_i$, ta thu được *công thức bộ chuyển*

$$
B(a_3 : a_2) = Ba_3 : Ba_2
$$

đúng khi $B$ là một $A$-môđun phẳng và $a_2$ là một iđêan sinh hữu hạn.

### 11. GIẢI THÍCH TÍNH PHẲNG THEO CÁC HỆ THỨC (*)

Trong toàn bộ số này, $A$ ký hiệu một vành, $E$ một môđun phải trên $A$ và $F$ một môđun trái trên $A$.

Mọi phần tử của $E \otimes_A F$ đều có thể viết được ít nhất theo một cách dưới dạng
$$
z = \sum_{i=1}^n e_i \otimes f_i \text{ với } e_i \in E \text{ và } f_i \in F.
$$
Bổ đề sau cho một điều kiện để tổng này bằng không:

#### Bổ đề 10 {#ac-i-s2-lem-10 .statement}

*Cho* $(f_\lambda)_{\lambda \in L}$ *là một họ sinh của* $F$ *và* $(e_\lambda)_{\lambda \in L}$ *là một họ phần tử của* $E$ *có giá hữu hạn. Để có* $\sum_{\lambda \in L} e_\lambda \otimes f_\lambda = 0$, *điều kiện cần và đủ là tồn tại một tập hợp hữu hạn* $J$, *một họ* $(x_j)_{j \in J}$ *các phần tử của* $E$ *và một họ* $(a_{j,\lambda})$ *($j \in J, \lambda \in L$) các phần tử của* $A$ *thỏa mãn các tính chất sau:*

(1) *họ* $(a_{j,\lambda})$ *có giá hữu hạn;*

(2) $\sum_{\lambda \in L} a_{j,\lambda} f_\lambda = 0$ *với mọi* $j \in J;$

(3) $e_\lambda = \sum_{j \in J} x_j a_{j,\lambda}$ *với mọi* $\lambda \in L.$

Nói một cách không chặt chẽ, hệ các $e_\lambda$ phải là một tổ hợp tuyến tính với các hệ số trong $E$ của các hệ phần tử của $A$ là những "hệ thức giữa các $f_\lambda$".

Xét $A$-môđun tự do $A_s^{(L)}$, cơ sở chính tắc của nó $(u_\lambda)$ và đồng cấu $g : A_s^{(L)} \to F$ sao cho $g(u_\lambda) = f_\lambda$ với mọi $\lambda \in L$; ký hiệu $R$ là hạt nhân của $g$, ta có (vì các $f_\lambda$ sinh ra $F$) một dãy khớp

$$
R \xrightarrow{i} A_s^{(L)} \xrightarrow{g} F \longrightarrow 0
$$

trong đó $i$ ký hiệu đơn ánh chính tắc. Từ Bổ đề 1 của no. 1 ta suy ra dãy khớp

$$
E \otimes_A R \xrightarrow{1 \otimes i} E \otimes_A A_s^{(L)} \xrightarrow{1 \otimes g} E \otimes_A F \longrightarrow 0.
$$

(*) Các kết quả của số này sẽ không được dùng trong phần còn lại của chương này, trừ ở § 3, no. 7.

$$
\sum_{\lambda \in L} e_\lambda \otimes u_\lambda = \sum_{j \in J} x_j \otimes i(r_j)
$$

trong đó $x_j \in E, r_j \in R$ và $J$ là hữu hạn. Viết $i(r_j) = \sum_{\lambda \in L} a_{j\lambda} u_\lambda$, giả thiết $r_j \in R$ kéo theo quan hệ $\sum_{\lambda \in L} a_{j\lambda} f_\lambda = 0$ với mọi $j \in J$; mặt khác quan hệ (14) kéo theo $e_\lambda = \sum_{j \in J} x_j a_{j\lambda}$ với mọi $\lambda \in L$ (*Đại số*, Chương II, § 3, no. 7, Hệ quả 1 của Mệnh đề 7), điều này hoàn tất chứng minh.

#### Mệnh đề 13 {#ac-i-s2-prop-13 .statement}

*Để E là F-phẳng* (no. 2, *Định nghĩa 1*), *điều kiện cần và đủ là điều kiện sau đây được thỏa mãn*:

*(R)* *Nếu* $(e_i)_{i \in I}$ *và* $(f_i)_{i \in I}$ *là hai họ hữu hạn các phần tử của E và F tương ứng sao cho* $\sum_{i \in I} e_i \otimes f_i = 0$ *trong* $E \otimes_A F$, *thì tồn tại một tập hữu hạn J, một họ* $(x_j)_{j \in J}$ *các phần tử của E và một họ* $(a_{ji})$ *($j \in J, i \in I$) các phần tử của A, có các tính chất sau*:

(1) $\sum_{i \in I} a_{ji} f_i = 0$ *với mọi* $j \in J$;
(2) $e_i = \sum_{j \in J} x_j a_{ji}$ *với mọi* $i \in I$.

Giả sử rằng E là F-phẳng. Gọi $(e_i)$ và $(f_i)$ là các họ hữu hạn phần tử sao cho $\sum_{i \in I} e_i \otimes f_i = 0$ trong $E \otimes_A F$, và gọi $F'$ là môđun con của F *sinh bởi các* $f_i$. Vì ánh xạ chính tắc $E \otimes_A F' \to E \otimes_A F$ là đơn ánh, ta cũng có $\sum_{i \in I} e_i \otimes f_i = 0$ *trong* $E \otimes_A F'$ *và khi đó có thể áp dụng Bổ đề 10 cho E và F'; do đó thu được các họ* $(x_j)$ *và* $(a_{ji})$ *thỏa mãn các điều kiện của (R)*.

Ngược lại, giả sử điều kiện (R) đúng. Gọi $F'$ là một môđun con của F và gọi $y = \sum_{i \in I} e_i \otimes f_i$ là một phần tử của hạt nhân của ánh xạ chính tắc $E \otimes_A F' \to E \otimes_A F$. Vì (R) đúng, tồn tại các họ $(x_j)$ và $(a_{ji})$ thỏa mãn các điều kiện (1) và (2). Ta kết luận rằng, trong $E \otimes_A F'$,

$$
y = \sum_{i,j} x_j a_{ji} \otimes f_i = \sum_{j \in J} (x_j \otimes \sum_{i \in I} a_{ji} f_i) = 0.
$$

Do đó $E \otimes_A F' \to E \otimes_A F$ là đơn ánh.

#### Hệ quả 1 {#ac-i-s2-prop-13-cor-1 .statement}

Để một $A$-môđun phải $E$ là phẳng, điều kiện cần và đủ là điều kiện sau đúng:

(RP) *Nếu* $(e_i)_{i \in I}$ và $(b_i)_{i \in I}$ là hai họ hữu hạn các phần tử của $E$ và $A$ tương ứng sao cho $\sum e_i b_i = 0$, thì tồn tại một tập hữu hạn $J$, một họ $(x_j)_{j \in J}$ các phần tử của $E$ và một họ $(a_{ji})$ ($j \in J, i \in I$) các phần tử của $A$ sao cho $\sum a_{ji} b_i = 0$ với mọi $j \in J$ và $e_i = \sum_{j \in J} x_j a_{ji}$ với mọi $i \in I$.

Điều kiện (RP) chính là điều kiện (R) của Mệnh đề 13 áp dụng cho môđun $F = A_s$.

Nói một cách gần đúng, (RP) phát biểu rằng: mọi "quan hệ" giữa các $b_i$, với hệ số trong $E$, đều là một tổ hợp tuyến tính (với hệ số trong $E$) của các "quan hệ" giữa các $b_i$ với hệ số trong $A$.

Xét riêng một đồng cấu từ $A$ vào một vành $B$, biến $B$ thành một A-môđun phải. Ta biết (no. 3, Mệnh đề 1) rằng điều này tương đương với việc nói rằng A-môđun này là phẳng, hoặc rằng nó phẳng đối với mọi A-môđun trái $A_s^m$ ($m \geqslant 1$). Áp dụng điều kiện (R) của Mệnh đề 13 với $E = B$ và $F = A_s^m$ ta thu được điều kiện sau:

#### Hệ quả 2 {#ac-i-s2-prop-13-cor-2 .statement}

Để vành $B$ là một A-môđun phải phẳng, điều cần và đủ là nó thỏa mãn điều kiện sau:
(RP') *Mọi nghiệm* $(y_k)_{1 \leq k \leq n}$, gồm các phần tử của $B$, của một hệ phương trình tuyến tính thuần nhất

$$
\sum_{k=1}^n y_k c_{ki} = 0 \quad (1 \leq i \leq m)
$$
với *hệ số* $c_{ki}$ trong $A$, *là một tổ hợp tuyến tính*
$$
y_k = \sum_{j=1}^q b_j z_{jk} \quad (1 \leq k \leq n)
$$
với *hệ số* $b_j \in B$, của các nghiệm $(z_{jk})_{1 \leq k \leq n}$ của hệ (15), gồm các phần tử $z_{jk}$ của $A$.

### Bài tập {#ac-i-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
