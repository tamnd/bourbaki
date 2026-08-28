---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 3
section_title: Metrizable groups, valued fields, normed spaces and algebras
lang: vi
source: top-v-x
pdf_pages: 0167-0185, 0242-0245
extraction: ocr
subsections:
    - "no": 1
      title: METRIZABLE TOPOLOGICAL GROUPS
      page: 0
      pdf_page: 167
    - "no": 2
      title: VALUED DIVISION RINGS
      page: 0
      pdf_page: 171
    - "no": 3
      title: NORMED SPACES OVER A VALUED DIVISION RING
      page: 0
      pdf_page: 175
    - "no": 4
      title: QUOTIENT SPACES AND PRODUCT SPACES OF NORMED SPACES
      page: 0
      pdf_page: 178
    - "no": 5
      title: CONTINUOUS MULTILINEAR FUNCTIONS
      page: 0
      pdf_page: 179
    - "no": 6
      title: ABSOLUTELY SUMMABLE FAMILIES IN A NORMED SPACE
      page: 0
      pdf_page: 180
    - "no": 7
      title: NORMED ALGEBRAS OVER A VALUED FIELD
      page: 0
      pdf_page: 181
statements: 40
exercises: 4
content_sha256: 43eea9c619372c2df354ddab959ee245f95c5c9e40315025ac2258ab6dc0d304
translated_from: content/en/top/IX/03_s3_metrizable_groups_valued_fields_normed.md
source_content_sha256: 8b0735f9661569735192e866f56800cc2ca77e68b63b4e1c9aade01fcd82bfa5
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-45e66895
glossary_version: 34
glossary_terms_sha256: 9001305b0225a5e87ca9c956938e7de749915e1c1b268a267815eacbe85ed605
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC NHÓM CÓ METRIC, CÁC TRƯỜNG ĐỊNH GIÁ, CÁC KHÔNG GIAN ĐỊNH CHUẨN VÀ CÁC ĐẠI SỐ

### 1. CÁC NHÓM TÔPÔ CÓ METRIC

#### Mệnh đề 1 {#top-ix-s3-prop-1 .statement}

Các uniformity trái và phải của một nhóm tôpô $G$ là có metric khi và chỉ khi $G$ là Hausdorff và phần tử đơn vị $e$ của $G$ có một hệ cơ bản đếm được các lân cận.

Điều kiện này rõ ràng là cần. Ngược lại, nếu nó được thỏa mãn, lấy $(V_n)$ là một hệ cơ bản các lân cận của $e$; nếu $U_n$ ký hiệu tập hợp các cặp $(x, y) \in G \times G$ sao cho $x^{-1}y \in V_n$, thì các $U_n$ tạo thành một hệ cơ bản đếm được các lân cận của uniformity trái của $G$; vì uniformity này là Hausdorff, theo § 2, no. 4, Định lý 1, suy ra rằng nó có metric. Tương tự đối với uniformity phải của $G$.

Một nhóm tôpô $G$ được gọi là *có metric* nếu tôpô của nó có metric. Khi đó Mệnh đề 1 cho thấy rằng hai uniformity của nó đều có metric.

Kết quả này có thể được làm mạnh hơn nhờ khái niệm sau đây:

#### Định nghĩa 1 {#top-ix-s3-def-1 .statement}

*Một metric* $d$ *trên một nhóm* $G$ *(viết theo phép nhân)* *được gọi là bất biến trái* (resp. *bất biến phải*) *nếu ta có*

$$
d(zx, zy) = d(x, y) \quad [\text{resp. } d(xz, yz) = d(x, y)]
$$

*đối với mọi* $x, y, z$ *trong* $G$.

#### Mệnh đề 2 {#top-ix-s3-prop-2 .statement}

*Uniformity trái* (resp. *phải*) *của một nhóm có metric* $G$ *có thể được xác định bởi một metric bất biến trái* (resp. *bất biến phải*) *trên* $G$.

Giả sử rằng hệ cơ bản $(V_n)$ các lân cận của $e$ gồm các lân cận đối xứng sao cho $V_{n+1}^3 \subset V_n$ với mỗi $n$. Khi đó các entourage tương ứng $U_n$ của uniformity trái là các entourage đối xứng sao cho $U_{n+1} \subset U_n$. Phương pháp được sử dụng trong chứng minh Mệnh đề 2 của § 1, no. 4 cho phép ta xây dựng, từ dãy các entourage $(U_n)$, một metric $d$ trên $G$ tương thích với uniformity trái của $G$; và vì với mỗi $z \in G$, ánh xạ $(x, y) \to (zx, zy)$ giữ bất biến từng $U_n$, định nghĩa của $d$ cho thấy rằng nó là một metric bất biến trái. Phương pháp này cũng áp dụng cho uniformity phải.

Chú ý rằng, nếu hai uniformity của $G$ phân biệt, metric $d$ không bất biến phải, và do đó nói chung $d(x^{-1}, y^{-1}) \neq d(x, y)$.

Đặc biệt, nếu $G$ là một nhóm Abel có metric, uniformity của nó được xác định bởi một metric bất biến $d$: nếu $G$ được viết theo phép cộng, ta có

$$
d(x, y) = d(0, y - x) = d(0, x - y).
$$

Ta thường viết $|x|$ (hoặc $||x|$) cho $d(0, x)$; khi đó ta có

$$
d(x, y) = |x - y|.
$$

Hàm $|x|$ thỏa mãn ba điều kiện sau:

a) $|-x| = |x|$ với mọi $x \in G$.

b) $|x + y| \leq |x| + |y|$ với mọi $x \in G$ và mọi $y \in G$.

c) $|x| = 0$ khi và chỉ khi $x = 0$.

Ngược lại:

#### Mệnh đề 3 {#top-ix-s3-prop-3 .statement}

*Cho $G$ là một nhóm Abel, được viết theo phép cộng, và cho $x \to |x|$ là một ánh xạ $G \to \mathbf{R}$ thỏa mãn các điều kiện a), b) và c) ở trên. Khi đó hàm $d(x, y) = |x - y|$ là một mêtric bất biến trên $G$; tôpô $\mathcal{T}$ mà nó xác định trên $G$ tương thích với cấu trúc nhóm của $G$, và cấu trúc đều xác định bởi $d$ trùng với cấu trúc đều của nhóm tôpô thu được bằng cách trang bị cho $G$ tôpô $\mathcal{T}$.*

Hàm $d(x, y)$ là một mêtric trên $G$, vì quan hệ $d(x, y) = 0$ tương đương với $x = y$ theo c); ta có $d(x, y) = d(y, x)$ theo a); và

$$
d(x, y) = |(x - z) + (z - y)| \leq |x - z| + |z - y| = d(x, z) + d(z, y)
$$

theo b). Hơn nữa, $d$ là bất biến, vì $(x + z) - (y + z) = x - y$.
Với mỗi số thực $x > 0$, gọi $V_x$ là tập hợp tất cả các $x \in G$ sao cho $|x| < x$; khi đó các $V_x$ tạo thành một hệ cơ bản $\mathfrak{S}$ các lân cận của $0$ đối với tôpô $\mathcal{T}$, và vì $d$ là bất biến, $a + \mathfrak{S}$ là một hệ cơ bản các lân cận của $a$ đối với tôpô $\mathcal{T}$, với mỗi $a \in G$. Theo a), các $V_x$ là đối xứng, và theo b), ta có $V_a + V_x \subset V_{2a}$; do đó tôpô $\mathcal{T}$ tương thích với cấu trúc nhóm của $G$ (Chương III, § 1, no. 2). Phần cuối của mệnh đề suy ra ngay lập tức.

Các điều kiện a', b' và c' tương đương với c) cùng với điều kiện

$$
|x - y| \leq |x| + |y|.
$$

Vì a' và b' rõ ràng kéo theo b'); ngược lại, lấy $x = 0$ trong b') và sử dụng c), ta thấy rằng $|-y| \leq |y|$; thay thế $y$ bởi $-y$ ta suy ra $|-y| = |y|$, đó là a); thay thế $y$ bởi $-y$ trong b') khi đó ta được b').

#### Mệnh đề 4 {#top-ix-s3-prop-4 .statement}

*Nếu G là một nhóm mêtric hóa được, thì mọi nhóm thương Hausdorff G/H của G đều mêtric hóa được. Nếu G cũng đầy đủ, thì G/H đầy đủ (*).*

Phần đầu của mệnh đề là một hệ quả của sự kiện rằng phần tử đơn vị của G/H có một hệ cơ bản đếm được các lân cận trong G/H; vì nếu (V_n) là một hệ cơ bản các lân cận của e trong G, thì các ảnh chính tắc $\dot{V}_n$ của các tập hợp V_n trong G/H tạo thành một hệ cơ bản các lân cận của phần tử đơn vị của G/H (Chương III, § 2, no. 6, Mệnh đề 17).

Để chỉ ra rằng G/H là đầy đủ nếu G là đầy đủ, theo § 2, no. 6, Mệnh đề 9, chỉ cần chỉ ra rằng mọi dãy Cauchy $(\dot{x}_n)$ (đối với đồng đều trái của G/H) đều hội tụ. Ta có thể giả sử, bằng cách chuyển qua một dãy con của $(\dot{x}_n)$ nếu cần, rằng với mỗi cặp chỉ số $p, q$ sao cho $p \geq n$ và $q \geq n$, ta có $\dot{x}_p^{-1}\dot{x}_q \in \dot{V}_n$; điều này có nghĩa là với mỗi cặp điểm $y \in \dot{x}_p, z \in \dot{x}_q$, ta có $y^{-1}z \in HV_n = V_nH$; và do đó, với mỗi $y \in \dot{x}_p$, giao của $\dot{x}_q$ và lân cận $yV_n$ của $y$ là không rỗng. Khi đó giả sử rằng dãy (V_n) đã được chọn sao cho $V_{n+1}^2 \subset V_n$, và định nghĩa quy nạp một dãy $(x_n)$ các điểm của G, sao cho $x_n \in \dot{x}_n$ và $x_{n+1} \in x_n V_n$; điều này có thể thực hiện được theo điều đã nói. Suy ra theo quy nạp rằng với mỗi $p > 0$ ta có $x_{n+p} \in x_n V_n V_{n+1} \ldots V_{n+p-1} \subset x_n V_{n-1}$. Do đó dãy $(x_n)$ là một dãy Cauchy trong G, nên nó hội tụ đến một điểm $a$; và suy ra ngay lập tức rằng ảnh chính tắc $\dot{a}$ của $a$ trong G/H là giới hạn của dãy $(\dot{x}_n)$.

#### Hệ quả 1 {#top-ix-s3-prop-4-cor-1 .statement}

*Cho G là một nhóm tôpô mêtric đầy đủ, cho G_0 là một nhóm con trù mật của G và cho H_0 là một nhóm con chuẩn đóng của G_0. Nếu H là bao đóng của H_0 trong G, thì nhóm thương G_0/H_0 có một phép đầy đủ đẳng cấu với G/H.*

H là một nhóm con chuẩn của G (Chương III, § 2, no. 3, Mệnh đề 8) và Mệnh đề 4 chỉ ra rằng G/H là đầy đủ. Hơn nữa nếu $\varphi$ là ánh xạ chính tắc của G lên G/H, thì rõ ràng rằng $\varphi(G_0)$ là trù mật trong G/H. Kết quả do đó suy ra từ Chương III, § 2, no. 7, Mệnh đề 21.

Cho G, G' là hai nhóm tôpô Abel Hausdorff, và $\hat{G}, \hat{G}'$ là các phép đầy đủ tương ứng của chúng. Ta nhắc lại (Chương III, § 3, no. 3, Mệnh đề 5) rằng nếu $u$ là một đồng cấu liên tục của G vào G', thì $u$ là đồng đều liên tục và mở rộng duy nhất thành một đồng cấu liên tục của $\hat{G}$ vào $\hat{G}'$, mà ta sẽ ký hiệu là $\hat{u}$ trong phần còn lại

(*) Tồn tại các nhóm đầy đủ không mêtric G chứa một nhóm con đóng H sao cho G/H không đầy đủ.

của tiểu mục này. Biểu đồ

$$
\begin{array}{ccc}
G & \xrightarrow{u} & G' \\
i \downarrow & & i' \downarrow \\
\hat{G} & \xrightarrow{\hat{u}} & \hat{G}'
\end{array}
$$

trong đó $i, i'$ là các đơn ánh chính tắc) là giao hoán. Nếu $v$ là một đồng cấu liên tục của $G'$ vào một nhóm tôpô Abel Hausdorff $G''$, và nếu $w = v \circ u$, thì ngay lập tức suy ra rằng $\hat{w} = \hat{v} \circ \hat{u}$.

Cho $H$ là một nhóm con đóng của $G$ và cho $E = G/H$. Gọi $j : H \to G$ và $p : G \to E$ là các ánh xạ chính tắc. Gọi $\overline{H}$ là bao đóng của $H$ trong $\hat{G}$; $\overline{H}$ là một nhóm đầy đủ và ta đồng nhất nó với phép đầy đủ $\hat{H}$ của $H$. Mở rộng liên tục $\hat{j}$ của $j$ đến $\hat{H}$ hiển nhiên là đơn ánh chính tắc của $\hat{H}$ vào $\hat{G}$.

Giả sử từ nay $G$ là mêtric hóa được. Khi đó ánh xạ chính tắc của $E = GH$ vào $\hat{G}\hat{H}$ là một đẳng cấu tôpô của $E$ lên một nhóm con trù mật của nhóm đầy đủ $\hat{G}/\hat{H}$ (Hệ quả 1), và do đó ta có thể đồng nhất $\hat{G}\hat{H}$ với $\hat{E}$ và mở rộng liên tục $\hat{p}$ của $p$ lên $\hat{G}$ với ánh xạ chính tắc của $\hat{G}$ lên $\hat{G}/\hat{H}$.

#### Hệ quả 2 {#top-ix-s3-prop-4-cor-2 .statement}

*Cho $G, G'$ là hai nhóm tôpô Abel mêtric hóa được; cho $u : G \to G'$ là một cấu xạ ngặt có hạt nhân $N$ và ảnh $P$. Khi đó $\hat{u} : \hat{G} \to \hat{G}'$ là một cấu xạ ngặt có hạt nhân $\hat{N}$ và ảnh $\hat{P}$.*

Cho $u = j \circ v \circ p$ là phân tích nhân tử chính tắc của $u$, trong đó $v$ là một đẳng cấu của nhóm tôpô $G/N$ lên nhóm tôpô $u(G) = P$. Ta có $\hat{u} = \hat{j} \circ \hat{v} \circ \hat{p}$, và ta đã thấy rằng $\hat{p}$ là ánh xạ chính tắc của $\hat{G}$ lên $\hat{G}\hat{N}$, và rằng $\hat{j}$ là ánh xạ chính tắc của $\hat{P}$ vào $\hat{G}$. Mặt khác, $\hat{v}$ là một đẳng cấu của $\hat{G}/\hat{N}$ lên $\hat{P}$ (Chương III, § 3, no. 4, Mệnh đề 5), do đó có kết quả.

#### Hệ quả 3 {#top-ix-s3-prop-4-cor-3 .statement}

*Cho $G, G', G''$ là ba nhóm tôpô Abel mêtric hóa được và cho $u : G \to G'$ và $v : G' \to G''$ là hai cấu xạ ngặt sao cho dãy $G \xrightarrow{u} G' \xrightarrow{v} G''$ là khớp [tức là, $u(G) = \overline{v}(0)$]. Khi đó dãy $\hat{G} \xrightarrow{\hat{u}} \hat{G}' \xrightarrow{\hat{v}} \hat{G}''$ là khớp.*

Thật vậy, nếu đặt $N = u(G) = \overline{v}(0)$, thì từ Hệ quả 2 suy ra $\hat{N}$ vừa là ảnh của $\hat{u}$ vừa là hạt nhân của $\hat{v}$.

#### Nhận xét 1 {#top-ix-s3-n1-rem-1 .statement}

Cho $G$ là một nhóm tôpô không Hausdorff sao cho nhóm Hausdorff liên kết với $G$ là mêtric hóa được; tương đương với việc phần tử đơn vị của $G$ có một hệ cơ bản đếm được các lân cận trong G. Chứng minh của Mệnh đề 4 áp dụng cho trường hợp này mà không cần sửa đổi, H là một nhóm con chuẩn tùy ý của G, và chỉ ra rằng nhóm Hausdorff liên kết với G/H là mêtric hóa được, và rằng G/H là một nhóm đầy đủ (nói chung không Hausdorff) bất cứ khi nào G là đầy đủ.

#### Nhận xét 2 {#top-ix-s3-n1-rem-2 .statement}

Cho d là một mêtric bất biến trái xác định tôpô của một nhóm mêtric hóa được G, và cho H là một nhóm con chuẩn đóng của G. Nếu $\dot{x}$ và $\dot{y}$ là hai điểm tùy ý của G/H, xét khoảng cách $d(\dot{x}, \dot{y})$ của hai tập con đóng $\dot{x}, \dot{y}$ trong G (\S 2, no. 2); ta sẽ thấy rằng hàm này là một mêtric bất biến trái trên G/H và xác định tôpô của nhóm thương này.

Trước hết nhận xét rằng nếu $x \in \dot{x}$ và $y \in \dot{y}$ thì ta có $d(\dot{x}, \dot{y}) = d(x, Hy)$; vì $d(x, Hy) = \inf_{h \in H} d(x, h y)$, và do đó $d(h'x, Hy) = d(x, Hy)$ với mọi $h' \in H$, vì d là bất biến trái; điều này chứng minh mệnh đề (\S 2, no. 2). Vậy với mỗi $\dot{z} \in G/H$ ta có [\S 2, no. 2, công thức (2)]

$$
|d(\dot{x}, \dot{z}) - d(\dot{y}, \dot{z})| = |d(x, \dot{z}) - d(y, \dot{z})| \leq d(x, y);
$$

and since this inequality is valid for all $x \in \dot{x}$ and all $y \in \dot{y}$, ta có $|d(\dot{x}, \dot{z}) - d(\dot{y}, \dot{z})| \leq d(\dot{x}, \dot{y})$, điều này cho thấy rằng $d(\dot{x}, \dot{y})$ là một metric trên G/H. Hơn nữa, với mọi $z \in \dot{z}$, ta có

$$
d(\dot{z}x, \dot{z}y) = \inf_{h \in H} d(zx, hzy)
$$

như trên; nhưng vì $hzy = z(z^{-1}hz) y$ và vì $z^{-1}hz$ chạy qua H khi h chạy qua H (H là chuẩn tắc), tính bất biến trái của $d(x, y)$ cho thấy rằng ta có $d(zx, Hz y) = d(x, Hy) = d(\dot{x}, \dot{y})$. Cuối cùng, nếu V là một lân cận của e trong G được xác định bởi $d(e, x) < \alpha$, thì ảnh V của V trong G/H là tập hợp được xác định bởi $d(e, \dot{x}) < \alpha$; điều này hoàn tất chứng minh.

### 2. CÁC VÀNH CHIA CÓ GIÁ TRỊ

#### Định nghĩa 2 {#top-ix-s3-def-2 .statement}

*Một giá trị tuyệt đối trên một vành chia* K *là một ánh xạ* $x \to |x|$ *của* K *vào* $\mathbf{R}_+$ *thỏa mãn các điều kiện sau:*

(VM_I) $|x| = 0$ nếu và chỉ nếu $x = 0$.
(VM_II) $|xy| = |x| \cdot |y|$ với mọi $x, y$ trong K.
(VM_III) $|x + y| \leq |x| + |y|$ với mọi $x, y$ trong K.

Theo (VM_II) ta có $|x| = |1| \cdot |x|$, và vì theo (VM_I) tồn tại ít nhất một x sao cho $|x| \neq 0$, nên $|1| = 1$; suy ra $1 = |1|^2$, do đó $|1| = 1$ và vì thế

$$
|-x| = |-1| |x| = |x|;
$$

do đó $|x - y| \leq |x| + |y|$ với mọi $x, y$ trong K. Vì vậy ta có thể nói rằng $d(x, y) = |x - y|$ là một metric bất biến trên nhóm cộng K, và ánh xạ $x \to |x|$ là một đồng cấu của nhóm nhân $K^*$ gồm các phần tử khác không của K vào nhóm nhân $\mathbf{R}_+^*$ của các số thực $> 0$.

Metric bất biến $|x - y|$ xác định một tôpô không gian metric trên K, tương thích với cấu trúc nhóm cộng của nó (no. 1, Mệnh đề 3); nhưng hơn nữa, tôpô này còn tương thích với cấu trúc vành chia của K. Thật vậy, tính liên tục của $xy$ trên $K \times K$ suy ra từ quan hệ

$$
xy - x_0 y_0 = (x - x_0)(y - y_0) + (x - x_0)y_0 + x_0(y - y_0),
$$

từ đó cho

$$
|xy - x_0 y_0| \leq |x - x_0| \cdot |y - y_0| + |x_0| \cdot |y - y_0| + |y_0| \cdot |x - x_0|.
$$

Tương tự, tính liên tục của $x^{-1}$ tại mọi điểm $x_0 \neq 0$ suy ra từ đẳng thức $x^{-1} - x_0^{-1} = x^{-1}(x_0 - x)x_0^{-1}$, từ đó, theo (VM_{II}),

$$
|x^{-1} - x_0^{-1}| = \frac{|x - x_0|}{|x_0| \cdot |x|};
$$

bây giờ nếu $\varepsilon > 0$ sao cho $\varepsilon < |x_0|$, thì quan hệ $|x - x_0| \leq \varepsilon$ suy ra $|x| \geq |x_0| - \varepsilon$, do đó $|x^{-1} - x_0^{-1}| \leq \varepsilon / |x_0|(|x_0| - \varepsilon)$; và điều này thiết lập tính liên tục của $x^{-1}$ tại điểm $x_0$.

#### Định nghĩa 3 {#top-ix-s3-def-3 .statement}

*Một vành chia có giá trị là một vành chia* $K$ *được trang bị cấu trúc được xác định bởi một giá trị tuyệt đối cho trước trên* $K$.

Một vành chia có giá trị sẽ luôn được xem là được trang bị tôpô xác định bởi giá trị tuyệt đối của nó, điều này làm cho nó trở thành một vành chia *tôpô*. Nếu $K_0$ là một vành chia con của một vành chia có giá trị $K$, hạn chế lên $K_0$ của giá trị tuyệt đối trên $K$ là một giá trị tuyệt đối trên $K_0$, xác định trên $K_0$ tôpô cảm sinh bởi tôpô của $K$.

#### Ví dụ 1 {#top-ix-s3-n2-exa-1 .statement}

Cho $K$ là một vành chia tùy ý. Với mỗi $x \in K$, đặt $|x| = 1$ nếu $x \neq 0$, và $|0| = 0$. Ánh xạ $x \to |x|$ được xác định như vậy là một giá trị tuyệt đối trên $K$, được gọi là giá trị tuyệt đối *không chính quy*. Tôpô xác định bởi một giá trị tuyệt đối $|x|$ trên một vành chia $K$ là *rời rạc* khi và chỉ khi $|x|$ là giá trị tuyệt đối không chính quy. Điều kiện này rõ ràng là đủ; ngược lại, nếu tôpô của $K$ là rời rạc, $|x|$ không thể nhận giá trị $\alpha > 0$ nào khác ngoài 1; vì nếu ta có $|x_0| = \alpha < 1$, dãy $(x_0^n)$ sẽ gồm các số hạng khác không và sẽ hội tụ về 0; để xử lý trường hợp $\alpha > 1$, xét $x_0^{-1}$ thay cho $x_0$.

#### Ví dụ 2 {#top-ix-s3-n2-exa-2 .statement}

Giá trị tuyệt đối của một số thực (Chương IV, § 1, no. 6) thỏa mãn các tiên đề (VM_I), (VM_{II}) và (VM_{III}), và tôpô mà nó xác định trên trường $\mathbf{R}$ là tôpô của đường thẳng thực. Trên trường $\mathbf{C}$ của các số phức (được đồng nhất với $\mathbf{R}^2$) [tương ứng vành chia $\mathbf{H}$ của các quaternion (được đồng nhất với $\mathbf{R}^4$)] chuẩn Euclid lại là một giá trị tuyệt đối và xác định tôpô của trường $\mathbf{C}$ (tương ứng vành chia $\mathbf{H}$) (Chương VIII, § 1, các số 2 và 4).

#### Ví dụ 3 {#top-ix-s3-n2-exa-3 .statement}

Trên một vành chia $K$, một định giá thực là một hàm $v$ xác định trên $K^*$ với các giá trị trong $\mathbf{R}$ thỏa mãn các điều kiện sau: a) nếu $x \in K^*$ và $y \in K^*$, thì $v(xy) = v(x) + v(y)$; b) nếu ngoài ra $x + y \neq 0$, thì $v(x + y) \geq \inf(v(x), v(y))$. Nếu $a$ là một số thực $> 1$, ta có thể khi đó định nghĩa một giá trị tuyệt đối trên $K$ bằng cách đặt $|x| = a^{-v(x)}$ với $x \neq 0$, và $|0| = 0$. Vì quan hệ $v(xy) = v(x) + v(y)$ với $x \neq 0$ và $y \neq 0$ suy ra quan hệ $|xy| = |x|.|y|$ đối với các giá trị này của $x$ và $y$, và quan hệ này hiển nhiên đúng nếu một trong $x, y$ bằng không; tương tự, từ quan hệ $v(x + y) \geq \inf(v(x), v(y))$ với $x \neq 0, y \neq 0$ và $x + y \neq 0$ ta suy ra $|x + y| \leq \sup(|x|, |y|) \leq |x| + |y|$, và các bất đẳng thức này vẫn được thỏa mãn nếu một trong $x, y, x + y$ bằng không. Đặc biệt, nếu $v_p(x)$ là định giá $p$-adic trên trường $\mathbf{Q}$ của các số hữu tỉ (số mũ của $p$ trong phân tích của $x$ thành tích của các thừa số nguyên tố), thì giá trị tuyệt đối tương ứng $|x|_p = p^{-v_p(x)}$ được gọi là giá trị tuyệt đối $p$-adic trên trường $\mathbf{Q}$ (xem Chương III, § 6, Bài tập 23).

#### Nhận xét {#top-ix-s3-n2-rem-1 .statement}

Nếu $x$ là một nghiệm đơn vị trong một vành chia có định giá, thì $|x| = 1$, vì $x^n = 1$ suy ra $|x|^n = 1$ và do đó $|x| = 1$. Đặc biệt, giá trị tuyệt đối duy nhất trên một trường hữu hạn là giá trị tuyệt đối không đúng, vì mọi phần tử $\neq 0$ của một trường như vậy đều là một nghiệm đơn vị.

#### Định nghĩa 4 {#top-ix-s3-def-4 .statement}

Hai giá trị tuyệt đối trên một vành chia $K$ được gọi là tương đương nếu chúng định nghĩa cùng một tôpô trên $K$.

#### Mệnh đề 5 {#top-ix-s3-prop-5 .statement}

Hai giá trị tuyệt đối $|x|_1, |x|_2$ trên một vành chia $K$, không cái nào là giá trị tuyệt đối không đúng, là tương đương khi và chỉ khi quan hệ $|x|_1 < 1$ kéo theo $|x|_2 < 1$. Khi đó tồn tại một số thực $\rho > 0$ sao cho $|x|_2 = |x|_1^\rho$ với mọi $x \in K$.

Điều kiện này là cần thiết, vì tập hợp tất cả các $x \in K$ sao cho $|x|_1 < 1$ trùng với tập hợp tất cả các $x$ sao cho, đối với tôpô được định nghĩa bởi giá trị tuyệt đối $|x|_1$, $\lim_{n \to \infty} x^n = 0$.

Giả sử ngược lại rằng $|x|_1 < 1 \Longrightarrow |x|_2 < 1$. Khi đó $|x|_1 > 1 \Longrightarrow |x|_2 > 1$, bởi vì $|x^{-1}|_1 < 1$ và do đó $|x^{-1}|_2 < 1$. Vì theo giả thiết giá trị tuyệt đối $|x|_1$ không tầm thường, tồn tại $x_0 \in K$ sao cho $|x_0|_1 > 1$. Đặt $a = |x_0|_1, b = |x_0|_2$ và đặt $\rho = \log b / \log a > 0$. Cho $x \in K^*$ và đặt $|x|_1 = |x_0|_1^\gamma$. Nếu $m$ và $n$ là các số nguyên sao cho $n > 0$ và $m/n > \gamma$, thì $|x|_1 < |x_0|_1^{m/n}$, và do đó $|x^n x_0^{-m}|_1 < 1$; suy ra $|x^n x_0^{-m}|_2 < 1, |x|_2 < |x_0|_2^{m/n}$. Tương tự, nếu $m/n < \gamma$, ta thấy rằng $|x|_2 > |x_0|_2^{m/n}$; do đó suy ra $|x|_2 = |x_0|_2^\gamma$; nói cách khác

$$
\log |x|_2 = \gamma \log b = \gamma \rho \log a = \rho \log |x|_1,
$$

tức là, $|x|_2 = |x|^p_1$. Bây giờ rõ ràng là các lân cận của không đối với các tôpô được xác định trên $K$ bởi $|x|_1$ và $|x|_2$ là đồng nhất.

Ngược lại, nếu $|x|$ là một giá trị tuyệt đối bất kỳ trên $K$, hàm $|x|^p$ là một giá trị tuyệt đối trên $K$ (tương đương với $|x|$) với mọi $p$ sao cho $0 < p \leq 1$. Ta chỉ cần kiểm tra bất đẳng thức $|x + y|^p \leq |x|^p + |y|^p$; và vì $|x + y|^p \leq (|x| + |y|)^p$ nên chỉ cần chứng minh rằng, nếu $a > 0$ và $b > 0$, ta có $(a + b)^p \leq a^p + b^p$ với mọi $p$ sao cho $0 < p \leq 1$. Nếu đặt $c = a/(a + b)$ và $d = b/(a + b)$, ta có $c + d = 1$, và bất đẳng thức cần chứng minh là $c^p + d^p \geq 1$; nhưng điều này suy ra ngay lập tức từ các hệ thức $c^p \geq c$ và $d^p \geq d$, vốn đúng vì $0 < c \leq 1$, $0 < d \leq 1$, $0 < p \leq 1$.

Do đó, tập hợp các giá trị của $r > 0$ sao cho $|x|^r$ là một giá trị tuyệt đối là một khoảng hữu hạn hoặc vô hạn của $\mathbf{R}$ có đầu mút bên trái là $0$; nếu nó hữu hạn, thì hiển nhiên nó đóng; vì nếu ta có $|x + y|^r \leq |x|^r + |y|^r$ với mọi $x, y$ trong $K$ và mọi $r$ sao cho $0 < r < r_0$, thì bởi tính liên tục, bất đẳng thức vẫn đúng với $r = r_0$. Nếu $|x|^r$ là một giá trị tuyệt đối với mọi $r > 0$, thì ta có
$$
|x + y| \leq (|x|^r + |y|^r)^{1/r}
$$
với mọi $x$ và $y$ trong $K$ và mọi $r > 0$. Bây giờ, nếu $a, b$ là hai số thực $\geq 0$, ta có $\lim_{r \to \infty} (a^r + b^r)^{1/c} = \sup (a, b)$; vì, giả sử chẳng hạn rằng $a \geq b$, ta có $a \leq (a^r + b^r)^{1/r} \leq 2^{1/r} a$, và kết quả suy ra khi cho $r \to + \infty$.

Vậy, nếu $|x|^r$ là một giá trị tuyệt đối với mọi $r > 0$, ta có
$$
|x + y| \leq \sup (|x|, |y|)
$$
điều này có thể được diễn đạt bằng cách nói rằng $v(x) = -\log |x| \ (x \neq 0)$ là một định giá trên $K$.

#### Nhận xét {#top-ix-s3-n2-rem-2 .statement}

Chứng minh của Mệnh đề 5 cho thấy rằng, nếu tôpô xác định bởi $|x|_2$ thô hơn tôpô xác định bởi $|x|_1$, và nếu $|x|_1$ không là không chính quy, thì $|x|_1$ và $|x|_2$ là tương đương, vì khi đó quan hệ $|x|_2 < 1$ suy ra $|x|_2 < 1$. Do đó, các tôpô xác định bởi hai giá trị tuyệt đối trên $K$, không cái nào trong chúng là không chính quy, không thể so sánh được mà không đồng nhất.

#### Mệnh đề 6 {#top-ix-s3-prop-6 .statement}

*Phần hoàn thành* $\hat{K}$ *của một vành chia* $K$ *được trang bị một giá trị tuyệt đối* $|x|$ *là một vành chia, và hàm* $|x|$ *có thể được mở rộng bởi tính liên tục thành một giá trị tuyệt đối trên* $\hat{K}$, *xác định tôpô của* $\hat{K}$.

Cho $\mathfrak{F}$ là một bộ lọc Cauchy trên $K$ (đối với cấu trúc đều cộng tính) không có $0$ làm điểm tụ; để chứng minh rằng $\hat{K}$ là một vành chia, chỉ cần chứng minh rằng ảnh của $\mathfrak{F}$ qua ánh xạ $x \to x^{-1}$ là một cơ sở bộ lọc Cauchy (chương III, § 6, no. 8, Mệnh đề 7). Theo giả thiết, tồn tại một số thực $\alpha > 0$ và một tập hợp $A \in \mathfrak{F}$ sao cho $|x| \geq \alpha$ với mọi $x \in A$; mặt khác, với mỗi $\varepsilon > 0$ tồn tại một tập hợp $B \in \mathfrak{F}$ sao cho $B \subset A$ và $|x - y| \leq \varepsilon$ với mọi $x \in B$.

và $y \in B$; do đó

$$
|x^{-1} - y^{-1}| = \frac{|x - y|}{|x| \cdot |y|} \leq \frac{\varepsilon}{a^2},
$$

và phần đầu tiên của mệnh đề được suy ra. Mêtric bất biến $|x - y| = d(x, y)$ được mở rộng bởi tính liên tục thành một mêtric trên $\hat{K}$ (\S 2, no. 1, Mệnh đề 1), mêtric này xác định tôpô của $\hat{K}$ và bất biến theo nguyên lý mở rộng các đồng nhất thức; ta tiếp tục ký hiệu mêtric bất biến này là $d(x, y)$. Nếu đặt $|x| = d(0, x)$ với $x \in \hat{K}$, thì rõ ràng $|x|$ là mở rộng bởi tính liên tục của hàm $|x|$ trên $K$ và do đó là một giá trị tuyệt đối trên $\hat{K}$ theo nguyên lý mở rộng các đồng nhất thức.

### 3. KHÔNG GIAN CHUẨN TRÊN MỘT VÀNH CHIA CÓ GIÁ TRỊ

#### Định nghĩa 5 {#top-ix-s3-def-5 .statement}

*Nếu E là một không gian vectơ (trái) trên một vành chia có giá trị không rời rạc K, một chuẩn trên E là một ánh xạ $x \to p(x)$ từ E vào $\mathbf{R}_+$ thỏa mãn các tiên đề sau*:

(NO_I) $p(x) = 0$ khi và chỉ khi $x = 0$;
(NO_{II}) $p(x + y) \leq p(x) + p(y)$ với mọi $x, y$ trong E;
(NO_{III}) $p(tx) = |t|p(x)$ với mọi $t \in K$ và mọi $x \in E$.

Các không gian chuẩn thường gặp nhất có $\mathbf{R}$ hoặc $\mathbf{C}$ làm trường vô hướng (với giá trị tuyệt đối thông thường).

Từ (NO_{III}) suy ra đặc biệt rằng $p(-x) = p(x)$; do đó nếu đặt $d(x, y) = p(x - y)$, thì $d$ là một *mêtric bất biến* trên nhóm cộng E, và xác định một tôpô không gian mêtric tương thích với cấu trúc nhóm cộng của E (no. 1, Mệnh đề 3); hơn nữa, ánh xạ

$$(t, x) \to tx$$

là *liên tục* trên $K \times E$; vì ta có

$$tx - t_0 x_0 = (t - t_0)(x - x_0) + (t - t_0)x + t_0(x - x_0)$$

và do đó

$$p(tx - t_0 x_0) \leq |t - t_0| p(x - x_0) + |t - t_0| p(x) + |t_0| p(x - x_0),$$

điều này cho thấy vế trái có thể được làm nhỏ tùy ý bằng cách lấy $|t - t_0|$ và $p(x - x_0)$ đủ nhỏ.

Cho E là một tập con của K. Một hàm $f : E \to K$ được gọi là một không gian chuẩn trên K.

Một không gian chuẩn được trang bị tôpô và tính đồng nhất xác định bởi chuẩn của nó.

Xét một vành chia hữu hạn chiều K. Được xem như một không gian vectơ thực, giá trị tuyệt đối $|x|$ là một chuẩn.

Chuẩn $\|x\| = \sqrt{\sum x_i^2}$, mà ta đã gọi là chuẩn Euclid trên không gian $\mathbf{R}^n$ (Chương VI, § 2), hiển nhiên là một chuẩn theo nghĩa của Định nghĩa 3. Các hàm $\sup |x_i|$ và $\sum |x_i|$ cũng vậy.

Cho $S(E; K')$ là tập hợp tất cả các hàm $f$ trên một tập hợp E nhận giá trị trong một vành chia $K'$ và sao cho hàm giá trị thực $x \mapsto f(x)$ bị chặn trên E. Tập hợp này rõ ràng là một không gian vectơ trên $K'$. Ký hiệu $p(f) = \sup_{x \in E} f(x)$, khi đó $p$ là một chuẩn trên không gian vectơ $S(E; K')$ (xem Chương X, § 1).

\* 4) Trên không gian vectơ $C(I; \mathbf{R})$ của tất cả các hàm liên tục thực hữu hạn xác định trên khoảng $I = [0, 1]$ của $\mathbf{R}$, hàm

$$
p(x) = \int_0^1 |x(t)| \, dt
$$

là một chuẩn.

Trong một không gian chuẩn E, quả cầu đóng B có tâm o và bán kính 1, tức là tập hợp tất cả các $x$ sao cho $p(x) \leq 1$, sẽ được gọi là quả cầu đơn vị của E. Ta sẽ chứng minh rằng một hệ cơ bản các lân cận của o được tạo thành bởi các phép tịnh tiến của quả cầu đơn vị bởi các phần tử của K. Quả cầu mở có tâm o và bán kính 1 là quả cầu đóng có tâm o và bán kính 1; do đó chỉ cần chứng minh rằng với mỗi số thực $r > 0$ tồn tại $k \in \mathbf{N}$ sao cho $0 < |k| < r$; chỉ cần lấy $k = \lfloor c/r \rfloor$, trong đó $c$ là một số nguyên đủ lớn, sao cho $|k|^2 < r$.

Cho E là một không gian chuẩn trên một trường có giá trị không rời rạc $K$.

#### Mệnh đề 7 {#top-ix-s3-prop-7 .statement}

Hai chuẩn $p, q$ trên một không gian vectơ $E$ là tương đương khi và chỉ khi tồn tại hai số $a > 0, b > 0$ sao cho

(I)
$$
a . p(x) \leq q(x) \leq b . p(x)
$$
với mọi $x \in E$.

Các bất đẳng thức này là đủ, vì từ quan hệ $a . p(x) \leq q(x)$ suy ra rằng, với mỗi $r > 0$, quả cầu đóng tâm o bán kính $ar$ (đối với chuẩn $q$) được chứa trong quả cầu đóng tâm o bán kính $r$ (đối với chuẩn $p$); do đó tôpô xác định bởi $q$ mịn hơn tôpô xác định bởi $p$. Tương tự, bất đẳng thức $q(x) \leq b . p(x)$ cho thấy tôpô xác định bởi $p$ mịn hơn tôpô xác định bởi $q$, và do đó $p$ và $q$ là tương đương.

Bây giờ ta chứng minh rằng các bất đẳng thức (I) là cần thiết. Nếu tôpô xác định bởi $q$ mịn hơn tôpô xác định bởi $p$, thì quả cầu đơn vị đối với $p$ chứa một quả cầu đóng tâm o bán kính $\alpha > 0$ đối với $q$; nghĩa là, quan hệ $q(x) \leq \alpha$ kéo theo $p(x) \leq 1$. Nếu $t_0 \in K$ là phần tử sao cho $0 < |t_0| < 1$, thì với mỗi $x \neq o$ trong $E$ tồn tại một số nguyên hữu tỉ $k$ duy nhất sao cho $\alpha |t_0| < q(t_0^k x) \leq \alpha$; do đó $p(t_0^k x) \leq 1$, nên
$$
p(x) \leq \frac{1}{|t_0|^k} \leq \frac{1}{\alpha |t_0|} q(x);
$$
đặt $a = \alpha |t_0|$ ta có do đó $a . p(x) \leq q(x)$ với mọi $x \neq o$, và bất đẳng thức này cũng đúng khi $x = o$. Tương tự ta chứng minh rằng nếu tôpô xác định bởi $p$ mịn hơn tôpô xác định bởi $q$, thì tồn tại $b > 0$ sao cho $q(x) \leq b . p(x)$.

#### Ví dụ {#top-ix-s3-n3-exa-1 .statement}

Trong không gian $\mathbf{R}^n$, ba chuẩn
$$
\sqrt{\sum_{i=1}^n x_i^2}, \quad \sup_{1 \leq i \leq n} |x_i| \quad \text{và} \quad \sum_{i=1}^n |x_i|
$$
là tương đương, vì ta có
(2)
$$
\sup_{1 \leq i \leq n} |x_i| \leq \sqrt{\sum_{i=1}^n x_i^2} \leq \sum_{i=1}^n |x_i| \leq n . \sup_{1 \leq i \leq n} |x_i|.
$$

#### Mệnh đề 8 {#top-ix-s3-prop-8 .statement}

Cho $E$ là một không gian chuẩn trên một vành chia định giá không rời rạc, cho $p$ là chuẩn trên $E$, và cho $\hat{E}$ là nhóm tôpô cộng tính là sự hoàn thành của nhóm cộng $E$. Khi đó hàm $(t, x) \to tx$ có thể được mở rộng bởi tính liên tục đến $\hat{K} \times \hat{E}$ và xác định trên $\hat{E}$ một cấu trúc không gian vectơ trên $\hat{K}$; chuẩn $p$ có thể được mở rộng bởi tính liên tục thành một chuẩn $\bar{p}$ trên $\hat{E}$ xác định tôpô của $\hat{E}$.

Sự mở rộng của $tx$ bằng tính liên tục là một trường hợp riêng của định lý mở rộng một ánh xạ song tuyến tính liên tục của một tích của hai nhóm Abel vào một nhóm thứ ba (Chương III, § 6, no. 5, Định lý 1); ta có $1.x = x$ và $t(u x) = (t u)x$ với $t \in \hat{K}$, $u \in \hat{K}$ và $x \in \hat{E}$, theo nguyên lý mở rộng các đồng nhất thức; do đó phép toán ngoài $(t, x) \to t x$ thực sự xác định trên $\hat{E}$ một cấu trúc của một không gian vectơ trên $\hat{K}$. Mặt khác, mêtric bất biến $\overline{d}(x, y) = \overline{p}(x - y)$ mở rộng thành một mêtric bất biến $\overline{d}$ trên $\hat{E}$ (\S 2, no. 1, Mệnh đề 1), mêtric này xác định tôpô của $\hat{E}$; nếu đặt $\overline{p}(x) = \overline{d}(0, x)$, thì $\overline{p}$ là sự mở rộng của $p$ bằng tính liên tục, và thỏa mãn các tiên đề (NO_I) và (NO_{II}); do tính liên tục của $t x$ trên $\hat{K} \times \hat{E}$, $\overline{p}$ cũng thỏa mãn (NO_{III}) (nguyên lý mở rộng các đồng nhất thức) và do đó là một chuẩn trên $\hat{E}$.

Khi cần xét một cấu trúc không gian định chuẩn xác định trên một không gian vectơ $E$, thông thường ta sẽ ký hiệu chuẩn của một vectơ $x$ bằng $||x||$, trừ khi ký hiệu này có khả năng dẫn đến nhầm lẫn.

### 4. CÁC KHÔNG GIAN THƯƠNG VÀ CÁC KHÔNG GIAN TÍCH CỦA CÁC KHÔNG GIAN ĐỊNH CHUẨN

#### Mệnh đề 9 {#top-ix-s3-prop-9 .statement}

*Cho $E$ là một không gian định chuẩn trên một vành chia có giá trị không rời rạc $K$, và cho $H$ là một không gian con vectơ đóng của $E$. Nếu, với mỗi lớp $\dot{x} \in E/H$, ta đặt $||\dot{x}|| = \inf_{x \in \dot{x}} ||x||$, thì hàm $||\dot{x}||$ là một chuẩn trên không gian vectơ $E/H$, và tôpô được xác định bởi chuẩn này là thương theo $H$ của tôpô của $E$.*

Theo Nhận xét 2 của no. 1, $d(\dot{x}, \dot{y}) = ||\dot{x} - \dot{y}||$ là một mêtric bất biến trên $E/H$, mêtric này xác định thương theo $H$ của tôpô của $E$. Chỉ còn phải chứng minh rằng $||t \dot{x}|| = |t| \cdot ||\dot{x}||$, và điều này suy ra ngay lập tức từ định nghĩa của $||\dot{x}||$ [Chương IV, § 5, no. 7, công thức (23)].

Chuẩn $||\dot{x}||$ cũng có thể được hiểu như sau: đó là khoảng cách (trong $E$) *của mọi điểm* $x \in \dot{x}$ *tới không gian con* $H$, vì các điểm của $\dot{x}$ là các điểm $x - z$, trong đó $z$ chạy qua $H$.

#### Mệnh đề 10 {#top-ix-s3-prop-10 .statement}

*Cho $(E_i)_{1 \leq i \leq n}$ là một họ hữu hạn các không gian định chuẩn trên một vành chia có giá trị không rời rạc $K$, và cho $E = \prod_{i=1}^n E_i$ là không gian vectơ tích. Nếu với mỗi $x = (x_i) \in E$ ta đặt $||x|| = \sup_{1 \leq i \leq n} ||x_i||$, thì hàm $||x||$ là một chuẩn trên $E$, và tôpô mà nó xác định trên $E$ là tích của các tôpô của các $E_i$.

Vì nếu $x = (x_i)$ và $y = (y_i)$, ta có $x + y = (x_i + y_i)$ và do đó
$$
||x + y|| = \sup_i ||x_i + y_i|| \leq \sup_i (||x_i|| + ||y_i||)
\leq \sup_i ||x_i|| + \sup_i ||y_i|| = ||x|| + ||y||.
$$

Mặt khác, hiển nhiên rằng $||tx|| = |t|.||x||$, và nếu $||x|| = 0$, thì $||x_i|| = 0$ và do đó $x_i = 0$ với $1 \leq i \leq n$, suy ra $x = 0$; vậy $||x||$ là một chuẩn trên $E$. Ngoài ra quan hệ $||x|| < a$ tương đương với $n$ quan hệ $||x_i|| < a$, và do đó chuẩn $||x||$ xác định tôpô tích trên $E$.

Tương tự ta có thể chỉ ra rằng các hàm $\sum_{i=1}^n ||x_i||$ và $\sqrt{\sum_{i=1}^n ||x_i||^2}$ là các chuẩn trên $E$; các bất đẳng thức (2) chỉ ra rằng cả ba chuẩn đều *tương đương*.

Đặc biệt, trong không gian vectơ (trái hoặc phải) $K^n$, nếu đặt

$$
p_1(x) = \sup_i |x_i|, \quad p_2(x) = \sum_{i=1}^n |x_i|, \quad p_3(x) = \sqrt{\sum_{i=1}^n |x_i|^2}
$$

với $x = (x_i)_{1 \leq i \leq n}$, thì ba hàm $p_1, p_2, p_3$ là các chuẩn tương đương xác định trên $K^n$ tôpô là tích của các tôpô của các thừa số $K$.

### 5. CÁC HÀM ĐA TUYẾN TÍNH LIÊN TỤC

#### Định lý 1 {#top-ix-s3-thm-1 .statement}

*Cho $E_i (1 \leq i \leq n)$ và $F$ là các không gian có chuẩn trên một vành chia có giá trị không rời rạc $K$, và cho $f$ là một ánh xạ đa tuyến tính từ $\prod_{i=1}^n E_i$ vào $F$. Khi đó $f$ liên tục trên $\prod_{i=1}^n E_i$ khi và chỉ khi tồn tại một số thực $a > 0$ sao cho, với mọi $x_i \in E_i \ (1 \leq i \leq n)$, ta có*

$$
||f(x_1, x_2, \ldots, x_n)|| \leq a . ||x_1|| . ||x_2|| \ldots ||x_n||
$$

(3)

Điều kiện này là *cần thiết*. Thật vậy, nếu $f$ liên tục tại điểm $(0, 0, \ldots, 0)$ thì tồn tại một số $b > 0$ sao cho các quan hệ $||x_i|| \leq b \ (1 \leq i \leq n)$ kéo theo $||f(x_1, \ldots, x_n)|| \leq 1$. Cho $t_0$ là một phần tử của $K$ sao cho $0 < |t_0| < 1$; khi đó với *mọi* điểm $(x_i) \in \prod_{i=1}^n E_i$ sao cho không có $x_i$ nào bằng không, tồn tại $n$ số nguyên hữu tỉ $k_i$ sao cho $b|t_0| < ||t_0^{k_i} x_i|| \leq b$; do đó ta có

$$
|t_0|^{k_1 + k_2 + \cdots + k_n} ||f(x_1, x_2, \ldots, x_n)|| \leq 1;
$$

mặt khác ta có $\frac{1}{|t_0|^{k_i}} \leq \frac{1}{b|t_0|} ||x_i||$, và do đó quan hệ (3) suy ra, với $a = (1/b|t_0|)^n$. Rõ ràng quan hệ này vẫn đúng khi một trong các $x_i$ bằng không.

Điều kiện này là đủ. Ta sẽ chỉ ra rằng, nếu nó được thỏa mãn, thì $f$ liên tục tại mọi điểm $(a_i)$ của $\prod_{i=1}^n E_i$. Ta có thể viết

$$
f(x_1, \ldots, x_n) - f(a_1, \ldots, a_n) = \sum_{i=1}^n f(a_1, \ldots, a_{i-1}, x_i - a_i, x_{i+1}, \ldots, x_n).
$$

Bây giờ, dùng (3), các điều kiện $||x_i - a_i|| \leq r$ ($1 \leq i \leq n$) kéo theo rằng

$$
||f(a_1, \ldots, a_{i-1}, x_i - a_i, x_{i+1}, \ldots, x_n)|| \leq ar \prod_{k \neq i}^n (||a_k|| + r);
$$

do đó, nếu $c$ là số lớn nhất trong các số $||a_i||$ ($1 \leq i \leq n$), ta có

$$
||f(x_1, \ldots, x_n) - f(a_1, \ldots, a_n)|| \leq nar (c + r)^{n-1}.
$$

Vì vế phải của bất đẳng thức này là một đa thức theo $r$ có số hạng hằng bằng không, nó tiến tới 0 khi $r$ tiến tới 0; do đó $f$ là liên tục.

#### Nhận xét {#top-ix-s3-n5-rem-1 .statement}

Hai trong số các mệnh đề đã được chứng minh trước đó là hệ quả của định lý này: tính liên tục của hàm song tuyến tính $tr$, do quan hệ $xr = t \cdot x$; và Mệnh đề 7, bằng cách áp dụng Định lý 1 cho ánh xạ đồng nhất của $E$, được xem như một ánh xạ tuyến tính từ không gian $E$, được trang bị chuẩn $p$, vào không gian $E$ được trang bị chuẩn $q$ (hoặc ngược lại).

### 6. CÁC HỌ KHẢ TỔNG TUYỆT ĐỐI TRONG MỘT KHÔNG GIAN CHUẨN

#### Định nghĩa 8 {#top-ix-s3-def-8 .statement}

Trong một không gian chuẩn $E$, một họ $(x_i)$ các điểm của $E$ được gọi là khả tổng tuyệt đối nếu họ $(||x_i||)$ các chuẩn của các $x_i$ là khả tổng trong $\mathbf{R}$.

Khái niệm này dường như phụ thuộc vào chuẩn được chọn trên $E$; nhưng theo Mệnh đề 7 của no. 3 và nguyên lý so sánh đối với các họ khả tổng của các số thực, một họ khả tổng tuyệt đối đối với một chuẩn $p$ trên $E$ là khả tổng tuyệt đối đối với mọi chuẩn trên $E$ tương đương với $p$.

Nếu $(x_i)_{i \in I}$ là một họ các điểm của $E$ vừa khả tổng vừa khả tổng tuyệt đối, ta có

$$
\left\| \sum_{i \in I} x_i \right\| \leq \sum_{i \in I} \|x_i\|.
$$

Thật vậy, đối với mỗi tập con hữu hạn $J$ của $I$ ta có $\left\| \sum_{i \in J} x_i \right\| \leq \sum_{i \in J} \|x_i\|$, và bất đẳng thức (4) suy ra bằng cách chuyển qua giới hạn đối với tập có hướng gồm các tập con hữu hạn của $I$.

#### Mệnh đề 11 {#top-ix-s3-prop-11 .statement}

Trong một không gian chuẩn đầy đủ E, mọi họ khả tổng tuyệt đối đều khả tổng.

Thật vậy, nếu $(x_i)$ là một họ khả tổng tuyệt đối trong E, thì với mỗi $\varepsilon > 0$ tồn tại một tập con hữu hạn J của tập chỉ số I sao cho, với mỗi tập con hữu hạn H của I không giao với J, ta có $\sum_{i \in H} ||x_i|| \leq \varepsilon$; do đó *a fortiori* $\left\| \sum_{i \in H} x_i \right\| \leq \varepsilon$, và điều này chứng minh mệnh đề, vì E là đầy đủ (tiêu chuẩn Cauchy, Chương III, § 5, no. 2, Định lý 1).

Một chuỗi mà số hạng tổng quát là $x_n$ được gọi là *hội tụ tuyệt đối* trong E nếu chuỗi mà số hạng tổng quát là $||x_n||$ hội tụ trong $\mathbf{R}$, hoặc (tương đương) nếu họ $(x_n)$ là khả tổng tuyệt đối; do đó (Chương III, § 5, no. 7, Mệnh đề 9):

#### Hệ quả {#top-ix-s3-n6-cor-1 .statement}

Trong một không gian chuẩn đầy đủ E, mọi chuỗi hội tụ tuyệt đối đều *hội tụ giao hoán*.

Đảo lại của Mệnh đề 11 nói chung là *sai*.

Xét ví dụ không gian $\mathcal{B}(\mathbf{N}; \mathbf{R})$ gồm các dãy bị chặn $x = (x_n)_{n \in \mathbf{N}}$ các số thực, với chuẩn $||x|| = \sup_n |x_n|$. Gọi $x_m$ là dãy $(x_{mn})_{n \in \mathbf{N}}$ sao cho $x_{mn} = 0$ nếu $m \neq n$ và $x_{mm} = 1/m$ với $m \geq 1$. Ta kiểm tra ngay lập tức rằng dãy $(x_m)_{m \in \mathbf{N}}$ là khả tổng trong $\mathcal{B}(\mathbf{N}; \mathbf{R})$ và tổng của nó là phần tử $y = (y_n)$ sao cho $y_0 = 0$ và $y_n = 1/n$ nếu $n \geq 1$; nhưng vì $||x_m|| = 1/m$, dãy các chuẩn của các $x_m$ không khả tổng trong $\mathbf{R}$.

Tuy nhiên, ta đã thấy trong Chương VII, § 3, no. 1, rằng mọi họ khả tổng trong $\mathbf{R}^n$ đều khả tổng tuyệt đối.

### 7. CÁC ĐẠI SỐ CHUẨN TRÊN MỘT TRƯỜNG CÓ GIÁ TRỊ

#### Định nghĩa 9 {#top-ix-s3-def-9 .statement}

*Nếu A là một đại số trên một trường K có giá trị không rời rạc, một chuẩn $p(x)$ trên A (A được xem như một không gian vectơ trên K) được gọi là tương thích với cấu trúc đại số của A nếu tôpô mà nó xác định là tương thích với cấu trúc vành của A. Một đại số trên K, được trang bị cấu trúc được xác định bởi một chuẩn tương thích với cấu trúc đại số, được gọi là một đại số chuẩn.*

Nếu A là một đại số chuẩn trên K, và nếu $p(x)$ là chuẩn trên A, thì ánh xạ song tuyến tính $(x, y) \to xy$ của $A \times A$ vào A là liên tục, theo giả thiết; do đó theo Định lý 1 của no. 5 tồn tại một số thực $a > 0$ sao cho $p(xy) \leq a \cdot p(x)p(y)$. Thay thế $p(x)$ bởi chuẩn tương đương $a \cdot p(x)$, do đó ta có thể luôn giả sử rằng chuẩn $||x||$ trên một đại số chuẩn A thỏa mãn

$$
||xy|| \leq ||x|| \cdot ||y||.
$$

Từ (5) suy ra bằng quy nạp rằng, với mỗi số nguyên $n > 0$, ta có

$$
||x^n|| \leq ||x||^n.
$$

#### Ví dụ 1 {#top-ix-s3-n7-exa-1 .statement}

Cho $K$ là một vành chia định giá và cho $K'$ là một trường con của tâm của $K$ sao cho vết trên $K'$ của giá trị tuyệt đối $|x|$ của $K$ không phải là giá trị tuyệt đối không đúng trên $K'$. Khi đó $K$, với $|x|$ làm chuẩn, là một đại số chuẩn trên $K'$.

#### Ví dụ 2 {#top-ix-s3-n7-exa-2 .statement}

Cho $K$ là một trường định giá không rời rạc và cho $M_n(K)$ là vành các ma trận vuông cấp $n$ trên $K$. Được xem như một không gian vectơ trên $K$, $M_n(K)$ là đẳng cấu với $K^{n^2}$. Nếu với mỗi $X = (x_{ij}) \in M_n(K)$ ta định nghĩa $\|X\| = \sup_{i,j} |x_{ij}|$, thì $\|X\|$ là một chuẩn trên $M_n(K)$, và tôpô được định nghĩa bởi chuẩn này là tôpô tích trên $K^{n^2}$ (Mệnh đề 10); từ đó suy ra (do tính liên tục của các đa thức với một số bất kỳ các biến trên $K$) rằng chuẩn này tương thích với cấu trúc đại số-$K$ của $M_n(K)$.

#### Ví dụ 3 {#top-ix-s3-n7-exa-3 .statement}

Tập hợp $\mathcal{B}(X; K)$ gồm tất cả các hàm $f$ trên một tập hợp $X$ với các giá trị trong một trường định giá không rời rạc $K$, sao cho $x \to |f(x)|$ bị chặn trên $X$, là một đại số trên $K$; chuẩn $\|f\| = \sup_{x \in X} |f(x)|$ tương thích với cấu trúc vành của $\mathcal{B}(X; K)$, vì ta có $\|fg\| \leq \|f\|\cdot\|g\|$ (xem Chương X, § 1).

Cho $a$ là một iđêan hai phía đóng trong một đại số chuẩn $A$. Nếu trong đại số thương $A/a$ ta đặt $||\dot{x}|| = \inf_{x \in X} ||x||$, ta thu được một chuẩn trên $A/a$ xác định tôpô là thương theo $a$ của tôpô của $A$ (Mệnh đề 9); vì tôpô thương này tương thích với cấu trúc vành thương của $A/a$ (Chương III, § 6, no. 4), suy ra rằng đại số thương $A/a$, với chuẩn $||x||$, là một đại số chuẩn.

Tương tự, nếu $(A_i)_{1 \leq i \leq n}$ là một họ gồm $n$ đại số định chuẩn trên một trường có giá trị $K$, và nếu trong đại số tích $A = \prod_{i=1}^n A_i$ ta đặt $||x|| = \sup_i ||x_i||$, với $x = (x_i)$, thì ta có một chuẩn trên $A$ xác định tích các tôpô của các $A_i$ (Mệnh đề 10); vì tôpô này tương thích với cấu trúc vành của $A$ (Chương III, § 6, no. 4), suy ra đại số tích $A$, với chuẩn $||x||$, là một đại số định chuẩn.

Cho $A$ là một đại số định chuẩn trên một trường có giá trị $K$. Phần hoàn thành $\hat{A}$ của $A$ (Chương III, § 6, no. 5, Mệnh đề 6) cũng được trang bị một cấu trúc $\hat{K}$-không gian vectơ (no. 3, Mệnh đề 8), và từ nguyên lý mở rộng các đẳng thức, rõ ràng là ta có $t(xy) = (tx)y = x(ty)$ với mọi $t \in \hat{K}$ và mọi $x, y \in \hat{A}$. Do đó $\hat{A}$ là một đại số trên $\hat{K}$; mặt khác (no. 3, Mệnh đề 8), chuẩn trên $A$ được mở rộng bằng tính liên tục thành một chuẩn xác định tôpô của $\hat{A}$, và vì vậy $\hat{A}$, được trang bị chuẩn này, là một *đại số định chuẩn* trên trường $\hat{K}$.

Nếu $(x_\lambda)_{\lambda \in L}$ và $(y_\mu)_{\mu \in M}$ là hai họ khả tổng tuyệt đối trong một đại số định chuẩn $A$, thì họ $(x_\lambda y_\mu)_{(\lambda, \mu) \in L \times M}$ là khả tổng tuyệt đối, vì $||x_\lambda y_\mu|| \leq ||x_\lambda|| \cdot ||y_\mu||$ (Chương IV, § 7, no. 3, Mệnh đề 1); nếu thêm vào đó $A$ là đầy đủ, thì cả ba họ đều khả tổng và ta có
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = \left( \sum_{\lambda \in L} x_\lambda \right) \left( \sum_{\mu \in M} y_\mu \right)
$$
theo tính kết hợp của tổng ở vế trái (Chương III, § 5, no. 3, công thức (2)).

Nếu đại số định chuẩn $A$ có một phần tử đơn vị $e \neq 0$, thì ánh xạ $t \to te$ là một đẳng cấu của cấu trúc trường của $K$ lên cấu trúc của trường con $Ke$ của $A$; đẳng cấu này cũng là một đẳng cấu của cấu trúc trường tôpô của $K$ lên cấu trúc của $Ke$ (tôpô của trường sau được cảm sinh bởi tôpô của $A$), vì phép hạn chế $||te||$ của chuẩn trên $A$ lên $Ke$ là một chuẩn tương đương với giá trị tuyệt đối
$$
|t| = \frac{1}{||e||} ||te||.
$$
Nếu $||e|| = 1$ thì ta có $||te|| = |t|$, và khi đó ta có thể đồng nhất trường có giá trị $K$ với trường con định chuẩn $Ke$ của $A$, và đặc biệt ta có thể ký hiệu phần tử đơn vị của $A$ bằng ký hiệu 1.

Trong phần tiếp theo, ta sẽ chỉ xét các đại số định chuẩn có một phần tử đơn vị $e$, và trong đó chuẩn thỏa bất đẳng thức (5); thay $x = y = e$ vào bất đẳng thức này, suy ra $||e|| \geq 1$.

#### Mệnh đề 12 {#top-ix-s3-prop-12 .statement}

*Nếu chuỗi có số hạng tổng quát là $z^n$ hội tụ trong $A$, thì $e - z$ là một phần tử khả nghịch của $A$ và ta có*
$$
(e - z)^{-1} = \sum_{n=0}^\infty z^n.
$$
*Ngược lại, nếu $||z|| < 1$ và nếu $e - z$ là một phần tử khả nghịch trong $A$, thì chuỗi có số hạng tổng quát là $z^n$ hội tụ và công thức (7) có giá trị.*

Với mỗi $p > 0$ ta có
$$
(e - z) \sum_{n=0}^p z^n = e - z^{p+1}.
$$
Nếu chuỗi có số hạng tổng quát là $z^n$ hội tụ và nếu $y$ là tổng của nó, thì $z^n$ tiến tới 0 khi $n \to + \infty$; do đó, chuyển qua giới hạn trong (8), ta được $(e - z)y = e$; tương tự ta chứng minh rằng $y(e - z) = e$, và do đó $y = (e - z)^{-1}$ (lưu ý rằng phần này của lập luận có giá trị trong mọi vành tôpô có một phần tử đơn vị).

Ngược lại, nếu $||z|| < 1$, thì vì $||z^{p+1}|| \leq ||z||^{p+1}$, suy ra $z^{p+1}$ tiến tới 0 khi $p \to +\infty$; nhân cả hai vế của (8) bên trái với $(e-z)^{-1}$ và cho $p$ tiến tới vô cùng, ta thấy rằng chuỗi có số hạng tổng quát là $z^n$ hội tụ và có $(e-z)^{-1}$ làm tổng của nó.

#### Hệ quả {#top-ix-s3-n7-cor-1 .statement}

*Cho A là một đại số chuẩn đầy đủ. Khi đó với mỗi $z \in A$ thỏa $||z|| < 1$, $e - z$ là một phần tử khả nghịch trong A.*

Chuỗi có số hạng tổng quát là $z^n$ hội tụ tuyệt đối, vì $||z^n|| \leq ||z||^n$ với $n > 0$, và do đó hội tụ, vì A đầy đủ (no. 6, Mệnh đề 11).

#### Mệnh đề 13 {#top-ix-s3-prop-13 .statement}

*Cho G là nhóm các phần tử khả nghịch của một đại số chuẩn đầy đủ A. Khi đó G là một tập mở của A; tôpô cảm sinh trên G bởi tôpô của A tương thích với cấu trúc nhóm của G; và G, được trang bị tôpô này, là một nhóm đầy đủ* (đối với mỗi một trong hai cấu trúc đều của nó).

Hệ quả của Mệnh đề 12 cho thấy G chứa một lân cận V của $e$ trong A; do đó, với mỗi $x_0 \in G$, các phần tử của $x_0V$ đều là phần tử khả nghịch, và $x_0V$ là một lân cận của $x_0$ trong A, vì $x \mapsto x_0x$ là một đồng phôi của A lên chính nó ($x_0$ là một phần tử khả nghịch của A). Suy ra G là mở trong A.

Để chứng minh rằng tôpô cảm sinh trên G bởi tôpô của A tương thích với cấu trúc nhóm của G, chỉ cần chứng minh rằng hàm $x^{-1}$ là *liên tục* trên G. Cho $x_0 \in G$, và với mỗi $x \in G$, viết $x$ dưới dạng $x = x_0(e + u)$, sao cho $u = x_0^{-1}(x - x_0)$; khi đó $||u|| \leq ||x_0^{-1}|| \cdot ||x - x_0||$, và do đó nếu $||x - x_0|| \leq 1 / ||x_0^{-1}||$, ta có $||u|| \leq 1$, $e + u = x_0^{-1}x$ là một phần tử khả nghịch, chuỗi có số hạng tổng quát là $(-1)^n u^n$ hội tụ tuyệt đối, và

$$
x^{-1} = (e + u)^{-1} x_0^{-1} = x_0^{-1} + \left( \sum_{n=1}^{\infty} (-1)^n u^n \right) x_0^{-1},
$$

từ đó suy ra rằng

$$
||x_0^{-1} - x_0^{-1}|| \leq \left| \left| \sum_{n=0}^{\infty} (-1)^n u^n \right| \right| \cdot ||u|| \cdot ||x_0^{-1}|| \\
\leq \left| \left| \sum_{n=0}^{\infty} (-1)^n u^n \right| \right| \cdot ||x_0^{-1}|^2 \cdot ||x - x_0||.
$$

Khi $x$ tiến tới $x_0$, $||x - x_0||$ tiến tới 0, và vì

$$
\left| \left| \sum_{n=0}^{\infty} (-1)^n u^n \right| \right| \leq ||e|| + \frac{||u||}{1 - ||u||}
$$

vẫn bị chặn, suy ra $x^{-1}$ tiến tới $x_0^{-1}$.

Cuối cùng, để chứng tỏ rằng cấu trúc đều trái của $G$ là đầy đủ, ta hãy chứng tỏ rằng mọi bộ lọc Cauchy $\tilde{\mathcal{F}}$ đối với cấu trúc đều này đều là một bộ lọc Cauchy đối với cấu trúc đều *cộng tính* của $A$ và hội tụ đến một điểm của $G$. Với mỗi $\varepsilon$ sao cho $0 < \varepsilon < 1$, tồn tại một tập $M \in \mathfrak{F}$ sao cho $||x^{-1}y - e|| \leq \varepsilon$ với mọi $x, y$ trong $M$, tức là sao cho
$$
||y - x|| \leq \varepsilon \ ||x||.
$$
Lấy $a$ là một điểm của $M$; với mỗi $x \in M$ ta có $||x - a|| \leq \varepsilon \ ||a||$, và do đó $||x|| \leq (1 + \varepsilon)||a||$. Mặt khác, tồn tại một tập $N \subset M$ thuộc $\mathfrak{F}$ và sao cho $||x^{-1}y - e|| \leq \varepsilon/(1 + \varepsilon)||a||$ với mọi $x$ và $y$ trong $N$; suy ra $||y - x|| \leq \varepsilon ||x||/(1 + \varepsilon)||a|| \leq \varepsilon$, điều này cho thấy rằng $\mathfrak{F}$ là một bộ lọc Cauchy đối với cấu trúc đều cộng tính của $A$, và do đó hội tụ đến một điểm $x_0$, vì $A$ là đầy đủ. Vì $x_0$ là giới hạn của $\mathfrak{F}$, ta có $||x^{-1}x_0 - e|| \leq \varepsilon$ với mọi $x \in M$ theo nguyên lý mở rộng các bất đẳng thức; vì $\varepsilon > 1$, suy ra $x^{-1}x_0$ là một phần tử khả nghịch trong $A$; do đó $x_0$ là một phần tử khả nghịch, tức là $x_0 \in G$.

#### Mệnh đề 14 {#top-ix-s3-prop-14 .statement}

*Trong một vành chia có giá trị đầy đủ, nhóm nhân của các phần tử khác 0 là một nhóm đầy đủ.*

Chứng minh giống như của Mệnh đề 13; ta chỉ cần thay chuẩn của $A$ bằng giá trị tuyệt đối của vành chia đang xét.

Chú ý rằng ta không thể áp dụng trực tiếp Mệnh đề 13, vì một vành chia có giá trị (không giao hoán) không nhất thiết là một đại số trên một trường có giá trị *không rời rạc* (sự hạn chế của giá trị tuyệt đối lên tâm của vành chia có thể không thích hợp).

#### Nhận xét {#top-ix-s3-n7-rem-1 .statement}

Mệnh đề 13 không nhất thiết đúng đối với một đại số chuẩn không đầy đủ. Chẳng hạn, trong đại số $C(I; \mathbf{R})$ của tất cả các hàm liên tục thực giá trị hữu hạn trên $I = [0, 1]$ [chuẩn là $||x|| = \sup_{t \in I} |x(t)|$], đại số con $P$ của tất cả các *đa thức* theo $t$ (hạn chế lên $I$) *không* đầy đủ; nếu $x(t)$ là một đa thức không hằng bất kỳ, thì $1 + \varepsilon x$ ở gần tùy ý phần tử đơn vị 1 của $P$ khi $\varepsilon$ là tùy ý nhỏ, nhưng $1 + \varepsilon x$ không phải là một phần tử khả nghịch *trong* $P$. Tuy nhiên, nếu $A$ là một đại số chuẩn không đầy đủ, $G$ là nhóm các phần tử khả nghịch của nó, $\hat{A}$ là sự đầy đủ hóa của $A$, thì $G$ là một nhóm con của nhóm các phần tử khả nghịch của $\hat{A}$, và do đó tôpô cảm sinh trên $G$ bởi tôpô của $A$ tương thích với cấu trúc nhóm của $G$.

### Bài tập {#top-ix-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
