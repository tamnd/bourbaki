---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 1
section_title: Definition of Lie algebras
lang: vi
source: lie-i-iii
pdf_pages: 0019-0030, 0091-0101
extraction: ocr
subsections:
    - "no": 1
      title: ALGEBRAS
      page: 0
      pdf_page: 19
    - "no": 2
      title: LIE ALGEBRAS
      page: 0
      pdf_page: 21
    - "no": 3
      title: COMMUTATIVE LIE ALGEBRAS
      page: 0
      pdf_page: 23
    - "no": 4
      title: IDEALS
      page: 0
      pdf_page: 23
    - "no": 5
      title: DERIVED SERIES, LOWER CENTRAL SERIES
      page: 0
      pdf_page: 24
    - "no": 6
      title: UPPER CENTRAL SERIES
      page: 0
      pdf_page: 24
    - "no": 7
      title: EXTENSIONS
      page: 0
      pdf_page: 25
    - "no": 8
      title: SEMI-DIRECT PRODUCTS
      page: 0
      pdf_page: 26
    - "no": 9
      title: CHANGE OF BASE RING
      page: 0
      pdf_page: 29
statements: 19
exercises: 27
content_sha256: 507dab0c72aa73204422fd06bb8d45d5704beaf345630caf3b9cbddf560c87fc
translated_from: content/en/lie/I/01_s1_definition_of_lie_algebras.md
source_content_sha256: 6f24a032c35720d8217f4a61a4f790ea698f94a79a12e0f692ee1ad01c4e55e0
translation_model: gpt-5.4
translation_run: translate-vi-6b649d28
glossary_version: 34
glossary_terms_sha256: cd87722793c09a65b53fe8f2ad1c1054079e7853832686d80d0b51705ede152a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐỊNH NGHĨA CÁC ĐẠI SỐ LIE

### 1. ĐẠI SỐ

Cho M là một môđun unita trên K cùng với một ánh xạ song tuyến tính $(x, y) \mapsto xy$ từ $M \times M$ vào M. Khi đó mọi tiên đề của đại số đều được thỏa mãn, trừ tính kết hợp của phép nhân. Do một sự lạm dụng ngôn ngữ, M được gọi là một đại số trên K không nhất thiết kết hợp, hoặc đôi khi, khi không thể có sự nhầm lẫn, là một đại số trên K. Trong số này, chúng tôi sẽ dùng cách gọi sau.

Nếu K-môđun M được trang bị phép nhân $(x, y) \mapsto yx$ thì ta thu được một đại số gọi là đại số đối của đại số trên.

Một môđun con K N của M ổn định đối với phép nhân được trang bị cấu trúc đại số trên K theo một cách hiển nhiên. N được gọi là một đại số con của M. N được gọi là một iđêan trái (tương ứng, iđêan phải) của M nếu các điều kiện $x \in N, y \in M$ kéo theo $yx \in N$ (tương ứng, $xy \in N$). Nếu N vừa là một iđêan trái vừa là một iđêan phải của M thì N được gọi là một iđêan hai phía của M. Trong trường hợp này, phép nhân trên M cho phép ta định nghĩa, sau khi chuyển qua thương, một phép nhân song tuyến tính trên môđun thương $M/N$ sao cho $M/N$ có một cấu trúc đại số. $M/N$ được gọi là đại số thương của M theo N.

† Các mệnh đề được chứng minh trong chương này chỉ phụ thuộc vào các tính chất đã được thiết lập trong các Sách I đến VI và vào một số kết quả của Đại số giao hoán, Chương III, § 2.

Cho $M_1$ và $M_2$ là hai đại số trên $K$ và $\phi$ là một ánh xạ từ $M_1$ vào $M_2$. $\phi$ được gọi là một *đồng cấu* nếu $\phi$ là $K$-tuyến tính và $\phi(xy) = \phi(x)\phi(y)$ với $x \in M_1, y \in M_1$. Hạt nhân $N$ của $\phi$ là một iđêan hai phía của $M_1$ và ảnh của $\phi$ là một đại số con của $M_2$. Khi chuyển qua thương, $\phi$ xác định một đẳng cấu từ đại số $M_1/N$ lên đại số $\phi(M_1)$.

Cho $M$ là một đại số trên $K$. Một ánh xạ $D$ từ $M$ vào $M$ được gọi là một *đạo hàm* của $M$ nếu nó là $K$-tuyến tính và $D(xy) = (Dx)y + x(Dy)$ với mọi $x \in M$ và $y \in M$. Định nghĩa này tổng quát hóa Định nghĩa 3 của *Đại số*, Chương IV, § 4, no. 3. Hạt nhân của một đạo hàm của $M$ là một đại số con của $M$. Nếu $D_1$ và $D_2$ là các đạo hàm của $M$, thì $D_1D_2 - D_2D_1$ là một đạo hàm của $M$ (xem *Đại số*, Chương IV, § 4, no. 3, Mệnh đề 5: chứng minh của mệnh đề này không dùng tính kết hợp của đại số).

Cho $M_1$ và $M_2$ là hai đại số trên $K$. Trên $K$-môđun tích $M = M_1 \times M_2$ ta định nghĩa một phép nhân bằng cách viết

$$
(x_1, x_2)(y_1, y_2) = (x_1y_1, x_2y_2),
$$

với mọi $x_1, y_1$ trong $M_1$, $x_2, y_2$ trong $M_2$. Đại số được xác định như vậy được gọi là *đại số tích* của $M_1$ và $M_2$. Ánh xạ $x_1 \mapsto (x_1, 0)$ (resp. $x_2 \mapsto (0, x_2)$) là một đẳng cấu từ $M_1$ (resp. $M_2$) lên một iđêan hai phía của $M$. Theo các đẳng cấu này, $M_1$ và $M_2$ được đồng nhất với các iđêan hai phía của $M$. Khi đó $K$-môđun $M$ là tổng trực tiếp của $M_1$ và $M_2$. Ngược lại, cho $M$ là một đại số trên $K$ và $M_1, M_2$ là hai iđêan hai phía của $M$ sao cho $M$ là tổng trực tiếp của $M_1$ và $M_2$. Khi đó $M_1M_2 \subset M_1 \cap M_2 = \{0\}$; do đó, nếu $x_1, y_1$ thuộc $M_1$ và $x_2, y_2$ thuộc $M_2$, thì $(x_1 + x_2)(y_1 + y_2) = x_1y_1 + x_2y_2$, nên $M$ được đồng nhất với đại số tích $M_1 \times M_2$. Mọi iđêan trái (resp. phải, hai phía) của $M_1$ đều là một iđêan trái (resp. phải, hai phía) của $M$. Chúng tôi để độc giả tự phát biểu các kết quả tương tự trong trường hợp một họ hữu hạn tùy ý các đại số.

Cho $M$ là một đại số trên $K$ và giả sử rằng $K$-môđun $M$ thừa nhận một cơ sở $(a_\lambda)_{\lambda \in L}$. Tồn tại một hệ duy nhất $(\gamma_{\lambda \mu \nu})_{(\lambda, \mu, \nu) \in L \times L \times L}$ gồm các phần tử của $K$ sao cho $a_\lambda a_\mu = \sum_v \gamma_{\lambda \mu v} a_v$ với mọi $\lambda, \mu$ trong $L$. Các $\gamma_{\lambda \mu \nu}$ được gọi là *các hằng số cấu trúc của $M$ đối với cơ sở* $(a_\lambda)$.

Cho $M$ là một đại số trên $K$, $K_0$ là một vành giao hoán có phần tử đơn vị và $\rho$ là một đồng cấu từ $K_0$ vào $K$ ánh xạ phần tử đơn vị thành phần tử đơn vị. Khi đó $M$ có thể được xem như một đại số trên $K_0$ bằng cách viết $\alpha.x = \rho(\alpha).x$ với $\alpha \in K_0, x \in M$. Đặc biệt, đây là trường hợp khi $K_0$ là một vành con của $K$ chứa phần tử đơn vị và $\rho$ được lấy là ánh xạ bao hàm từ $K_0$ vào $K$.

Cho $M$ là một đại số trên $K$, $K_1$ là một vành giao hoán có phần tử đơn vị và $\sigma$ là một đồng cấu của $K$ vào $K_1$ ánh xạ phần tử đơn vị lên phần tử đơn vị. Cho $M_{(K_1, \sigma)} = M_{(K_1)}$ là $K_1$-môđun dẫn xuất từ $M$ bằng cách mở rộng vành các vô hướng tới $K_1$ (*Đại số*, Chương II, § 5). Phép nhân trên $M$ xác định một cách chính tắc một ánh xạ $K_1$-song tuyến tính từ $M_{(K_1)} \times M_{(K_1)}$ vào $M_{(K_1)}$ (*Đại số*, Chương IX, § 1, no. 4) sao cho $M_{(K_1)}$ được trang bị cấu trúc của một đại số trên $K_1$ (đại số này được gọi là *dẫn xuất từ* $M$ *bằng cách mở rộng vành các vô hướng tới* $K_1$). Điều này đặc biệt xảy ra khi $K$ là một vành con của $K_1$ chứa phần tử đơn vị và $\sigma$ là ánh xạ bao hàm của $K$ vào $K_1$.

### 2. ĐẠI SỐ LIE

#### Định nghĩa 1 {#lie-i-s1-def-1 .statement}

*Một đại số g trên K được gọi là một đại số Lie trên K nếu phép nhân của nó (được ký hiệu bởi $(x, y) \mapsto [x, y]$) thỏa mãn các đồng nhất thức:*

(1) $$ [x, x] = 0 $$

(2) $$ [x, [y, z]] + [y, [z, x]] + [z, [x, y]] = 0 $$

*đối với mọi* $x, y, z$ *trong g*.

Tích $[x, y]$ được gọi là *ngoặc* của $x$ và $y$. Đồng nhất thức (2) được gọi là *đồng nhất thức Jacobi*.

Ngoặc $[x, y]$ là một hàm song tuyến tính phản xứng của $x$ và $y$. Ta có đồng nhất thức:

(3) $$ [x, y] = -[y, x] $$

nên đồng nhất thức Jacobi có thể được viết:

(4) $$ [x, [y, z]] = [[x, y], z] + [y, [x, z]]. $$

Mọi đại số con và mọi đại số thương của một đại số Lie đều là một đại số Lie. Mọi tích của các đại số Lie đều là một đại số Lie. Nếu $g$ là một đại số Lie, thì đại số đối $g^0$ là một đại số Lie và ánh xạ $x \mapsto -x$ là một đẳng cấu từ $g$ lên $g^0$, theo đồng nhất thức (3).

#### Ví dụ 1 {#lie-i-s1-n2-exa-1 .statement}

Cho $L$ là một đại số kết hợp trên $K$. Dấu ngoặc $[x, y] = xy - yx$ là một hàm song tuyến tính của $x$ và $y$. Dễ kiểm tra rằng luật hợp thành $(x, y) \mapsto [x, y]$ trên $K$-môđun $L$ biến $L$ thành một đại số Lie trên $K$.

#### Ví dụ 2 {#lie-i-s1-n2-exa-2 .statement}

Trong Ví dụ 1, chọn $L$ là đại số kết hợp các nội đồng cấu của một $K$-môđun $E$. Ta thu được *đại số Lie các nội đồng cấu của* $E$, được ký hiệu bởi $gl(E)$. (Nếu $E = K^n$, đại số Lie $gl(E)$ được ký hiệu bởi $gl(n, K)$.)

Mọi đại số con Lie của $gl(E)$ đều là một đại số Lie trên $K$. Đặc biệt:
(1) Nếu $E$ được trang bị một cấu trúc đại số (không nhất thiết kết hợp), thì các phép đạo hàm của $E$ tạo thành một đại số Lie trên $K$.
(2) Nếu $E$ có một cơ sở hữu hạn, thì các nội đồng cấu của $E$ có vết bằng không tạo thành một đại số Lie trên $K$ ký hiệu bởi $sl(E)$ (hoặc $sl(n, K)$ nếu $E = K^n$).
(3) Tập hợp $M_n(K)$ các ma trận vuông cấp $n$ có thể được xem như một đại số Lie trên K đẳng cấu chính tắc với gl(n, K). Gọi $(E_{ij})$ là cơ sở chính tắc của $\mathbf{M}_n(K)$ (Đại số, Chương II, § 10, no. 3). Suy ra dễ dàng rằng:

$$
\begin{cases}
[E_{ij}, E_{kl}] = 0 & \text{nếu } j \neq k \text{ và } i \neq l \\
[E_{ij}, E_{jl}] = E_{il} & \text{nếu } i \neq l \\
[E_{ij}, E_{kt}] = -E_{kj} & \text{nếu } j \neq k \\
[E_{ij}, E_{ji}] = E_{ii} - E_{jj}
\end{cases}
$$

(5)

Đại số con Lie của $\mathbf{M}_n(K)$ gồm các ma trận tam giác (resp. các ma trận tam giác có vết không, resp. các ma trận tam giác có đường chéo không) được ký hiệu bởi $t(n, K)$ (resp. st(n, K), resp. n(n, K)) (Đại số, Chương II, § 10; no. 7).

*Ví dụ 3. Cho V là một đa tạp thực khả vi vô hạn lần. Các toán tử vi phân với hệ số thực khả vi vô hạn lần lập thành một đại số kết hợp trên $\mathbf{R}$ và do đó, theo Ví dụ 1, một đại số Lie $\Delta$ trên $\mathbf{R}$. Ngoặc của hai trường vectơ khả vi vô hạn lần trên V là một trường vectơ khả vi vô hạn lần và do đó các trường vectơ khả vi vô hạn lần trên V lập thành một đại số con Lie $\mathfrak{f}$ của $\Delta$. Nếu V là một nhóm Lie thực *nhóm Lie*, thì các trường vectơ bất biến trái lập thành một đại số con Lie $g$ của $\mathfrak{f}$ được gọi là *đại số Lie* của V. Không gian vectơ $g$ được đồng nhất với không gian tiếp xúc của V tại $e$ (phần tử đơn vị của V). Cho V' là một nhóm Lie thực khác, $e'$ là phần tử đơn vị của nó và $g'$ là đại số Lie của nó. Mọi đồng cấu giải tích từ V vào V' đều xác định một ánh xạ tuyến tính từ không gian tiếp xúc của V tại $e$ vào không gian tiếp xúc của V' tại $e'$; ánh xạ này là một đồng cấu của đại số Lie $g$ vào đại số Lie $g'$. Nếu V là nhóm tuyến tính của một không gian vectơ thực hữu hạn chiều E thì tồn tại một đẳng cấu chính tắc từ $gl(E)$ lên đại số Lie $g$ của V, mà theo đó $g$ được đồng nhất với $gl(E)$.*

#### Định nghĩa 2 {#lie-i-s1-def-2 .statement}

*Cho g là một đại số Lie và x là một phần tử của g. Ánh xạ tuyến tính $y \mapsto [x, y]$ từ g vào g được gọi là ánh xạ tuyến tính liên hợp của x và được ký hiệu bởi $\operatorname{ad}_g x$ hoặc $\operatorname{ad} x$.*

#### Mệnh đề 1 {#lie-i-s1-prop-1 .statement}

*Cho g là một đại số Lie. Với mọi $x \in g$, $\operatorname{ad} x$ là một đạo hàm. Ánh xạ $x \mapsto \operatorname{ad} x$ là một đồng cấu của đại số Lie g vào đại số Lie $\mathfrak{d}$ các đạo hàm của g. Nếu $D \in \mathfrak{d}$ và $x \in g$, thì $[D, \operatorname{ad} x] = \operatorname{ad}(Dx)$.

Đẳng thức (4) có thể được viết:

$$
(\operatorname{ad} x) \cdot [y, z] = [(\operatorname{ad} x) \cdot y, z] + [y, (\operatorname{ad} x) \cdot z]
$$

hoặc:

$$
(\operatorname{ad}[x, y]) \cdot z = (\operatorname{ad} x) \cdot ((\operatorname{ad} y) \cdot z) - (\operatorname{ad} y) \cdot ((\operatorname{ad} x) \cdot z)
$$

do đó có hai mệnh đề đầu tiên. Mặt khác, nếu $D \in \mathfrak{d}$, $x \in g$, $y \in g$, thì $[D, \operatorname{ad} x] \cdot y = D([x, y]) - [x, Dy] = [Dx, y] = (\operatorname{ad} Dx) \cdot y$, do đó có khẳng định cuối cùng.

Ánh xạ $\operatorname{ad} x$ cũng được gọi là *đạo hàm nội* được xác định bởi $x$.

### 3. ĐẠI SỐ LIE GIAO HOÁN

#### Định nghĩa 3 {#lie-i-s1-def-3 .statement}

*Hai phần tử x, y của một đại số Lie được gọi là hoán vị được nếu [x, y] = 0. g được gọi là giao hoán nếu hai phần tử bất kỳ của nó đều hoán vị được.*

#### Ví dụ 1 {#lie-i-s1-n3-exa-1 .statement}

Cho L là một đại số kết hợp và g là đại số Lie được xác định bởi nó (no. 2, Ví dụ 1). Hai phần tử x, y là hoán vị được trong g khi và chỉ khi xy = yx trong L.

*Ví dụ 2. Nếu một nhóm Lie thực G là giao hoán thì đại số Lie của nó là giao hoán.*

Mọi K-môđun hiển nhiên đều có thể được trang bị một cấu trúc đại số Lie giao hoán duy nhất trên K.

Nếu g là một đại số Lie, mọi môđun con đơn sinh của g là một đại số con Lie giao hoán của g.

### 4. IĐÊAN

Từ đồng nhất thức (3) suy ra rằng trong một đại số Lie g không có sự phân biệt giữa iđêan trái và iđêan phải, mọi iđêan đều là hai phía. Vì vậy ta chỉ nói đơn giản là iđêan.

*Ví dụ. Cho G là một nhóm Lie, g là đại số Lie của nó và H là một nhóm con Lie của G. Mọi trường vectơ bất biến trái trên H đều xác định một cách chính tắc một trường vectơ bất biến trái trên G, do đó có một đơn ánh chính tắc từ đại số Lie h của H vào g; h được đồng nhất với một đại số con Lie của g qua đơn ánh này. Nếu H là chuẩn tắc trong G thì ảnh chính tắc của h trong g là một iđêan của g.*

Một iđêan của g là một môđun con của g ổn định đối với các đạo hàm nội của g.

#### Định nghĩa 4 {#lie-i-s1-def-4 .statement}

*Một môđun con của g ổn định dưới mọi đạo hàm của g được gọi là một iđêan đặc số của g.*

#### Mệnh đề 2 {#lie-i-s1-prop-2 .statement}

*Cho g là một đại số Lie, a là một iđêan (tương ứng, một iđêan đặc số) của g và b là một iđêan đặc số của a. Khi đó b là một iđêan (tương ứng, một iđêan đặc số) của g.*

Mọi đạo hàm nội (tương ứng, mọi đạo hàm) của g đều để a ổn định và cảm sinh trên a một đạo hàm, do đó để b ổn định.

Cho g là một đại số Lie. Nếu a và b là các iđêan của g thì a + b và a ∩ b là các iđêan của g.

Cho a và b là hai môđun con của g. Theo một lạm dụng ký hiệu, môđun con của g sinh bởi các phần tử dạng [x, y] (x ∈ a, y ∈ b) được ký hiệu bởi [a, b]. Ta có [a, b] = [b, a] theo đồng nhất thức (3). Nếu z ∈ g thì [z, a], hoặc [a, z], ký hiệu môđun con [Kz, a] = (ad z)(a).

#### Mệnh đề 3 {#lie-i-s1-prop-3 .statement}

*Nếu a và b là các iđêan (tương ứng, các iđêan đặc số) của g thì [a, b] là một iđêan (tương ứng, một iđêan đặc số) của g.*

Cho D là một đạo hàm nội (tương ứng, một đạo hàm) của g. Nếu $x \in a$ và $y \in b$, thì
$$
D([x, y]) = [Dx, y] + [x, Dy] \in [a, b].
$$
Do đó có mệnh đề.

Nếu a là một môđun con của g, tập hợp các $x \in g$ sao cho $(\mathrm{ad}\ x).a \subset a$ là một đại số con n của g gọi là *chuẩn hoá tử* của a trong g. Nếu hơn nữa a là một đại số con của g, thì $a \subset n$ và a là một iđêan của n.

### 5. CHUỖI DẪN XUẤT, CHUỖI TRUNG TÂM GIẢM

Iđêan đặc số $[g, g]$ được gọi là *iđêan dẫn xuất* của một đại số Lie g và được ký hiệu bởi $\mathcal{D}g$.

Mọi môđun con của g chứa $\mathcal{D}g$ đều là một iđêan của g.

*Chuỗi dẫn xuất* của g là dãy giảm $\mathcal{D}^0g, \mathcal{D}^1g, \ldots$ các iđêan đặc số của g được định nghĩa quy nạp như sau: (1) $\mathcal{D}^0g = g$; (2) $\mathcal{D}^{p+1}g = [\mathcal{D}^pg, \mathcal{D}^pg]$.

*Chuỗi trung tâm giảm* của g là dãy giảm $\mathcal{C}^1g, \mathcal{C}^2g, \ldots$ các iđêan đặc số của g được định nghĩa quy nạp như sau: (1) $\mathcal{C}^1g = g$; (2) $\mathcal{C}^{p+1}g = [g, \mathcal{C}^pg]$. Khi đó $\mathcal{C}^2g = \mathcal{D}g$ và $\mathcal{C}^{p+1}g \supset \mathcal{D}^pg$ với mọi $p$, như thấy ngay lập tức bằng quy nạp theo $p$.

#### Mệnh đề 4 {#lie-i-s1-prop-4 .statement}

*Cho g và h là hai đại số Lie trên K và f là một đồng cấu của g lên h. Khi đó $f(\mathcal{D}^pg) = \mathcal{D}^pf, f(\mathcal{C}^pg) = \mathcal{C}^ph$.*

Nếu a và b là các môđun con của g, thì ngay lập tức suy ra rằng
$$
f([a, b]) = [f(a), f(b)].
$$
Mệnh đề khi đó là ngay lập tức bằng quy nạp theo $p$.

#### Hệ quả {#lie-i-s1-n5-cor-1 .statement}

*Cho g là một đại số Lie và a là một iđêan của g. Để đại số Lie $g/a$ là giao hoán, điều kiện cần và đủ là $a \supset \mathcal{D}g$.*

Nói rằng $g/a$ là giao hoán có nghĩa là nói rằng $\mathcal{D}(g/a) = \{0\}$.
Nhưng $\mathcal{D}(g/a)$ là, theo Mệnh đề 4, ảnh chính tắc của $\mathcal{D}g$ trong $g/a$.

### 6. CHUỖI TRUNG TÂM TRÊN

Cho g là một đại số Lie và P là một tập con của g. *Bộ tập trung hóa* của P trong g là tập hợp các phần tử của g giao hoán với các phần tử của P. Bộ tập trung hóa này là giao của các hạt nhân của các ad $y$, trong đó $y$ chạy qua P; do đó nó là một đại số con của g.

#### Mệnh đề 5 {#lie-i-s1-prop-5 .statement}

*Cho g là một đại số Lie và a là một iđêan (tương ứng, một iđêan đặc số) của g. Bộ tập trung hóa $a'$ của a trong g là một iđêan (tương ứng, một iđêan đặc số) của g.*

Cho D là một đạo hàm nội (tương ứng, một đạo hàm) của g. Nếu $x \in a'$ và $y \in a$, thì
$$
[Dx, y] = D([x, y]) - [x, Dy] = 0;
$$
do đó $Dx \in a'$. Suy ra mệnh đề.

Cho $g$ là một đại số Lie. Bộ tập trung của $g$ trong $g$ được gọi là tâm của $g$, tức là iđêan đặc số của các $x \in g$ sao cho $[x, y] = 0$ với mọi $y \in g$. Tâm của $g$ là hạt nhân của đồng cấu $x \mapsto \mathrm{ad}\, x$.

Chuỗi trung tâm trên của $g$ là dãy tăng $\mathcal{C}_0 g, \mathcal{C}_1 g, \ldots$ các iđêan đặc số của $g$ được định nghĩa bằng quy nạp như sau: (1) $\mathcal{C}_0 g = \{0\}$; (2) $\mathcal{C}_{p+1} g$ là ảnh ngược qua ánh xạ chính tắc từ $g$ lên $g / \mathcal{C}_p g$ của tâm của $g / \mathcal{C}_p g$
Iđêan $\mathcal{C}_1 g$ là tâm của $g$.

### 7. MỞ RỘNG

#### Định nghĩa 5 {#lie-i-s1-def-5 .statement}

Cho $a$ và $b$ là hai đại số Lie trên $K$. Một mở rộng của $b$ bởi $a$ là một dãy:

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

trong đó $g$ là một đại số Lie trên $K$, $\mu$ là một đồng cấu toàn ánh từ $g$ lên $b$ và $\lambda$ là một đơn cấu từ $a$ lên hạt nhân của $\mu$.

Hạt nhân $n$ của $\mu$ được gọi là hạt nhân của mở rộng. Đồng cấu $\lambda$ là một đẳng cấu của $a$ lên $n$ và đồng cấu $\mu$ xác định một đẳng cấu của $g / n$ lên $b$ khi chuyển qua thương.
Do lạm dụng ngôn ngữ, $g$ cũng được gọi là một mở rộng của $b$ bởi $a$.

Hai mở rộng:

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b, \quad a \xrightarrow{\lambda'} g' \xrightarrow{\mu'} b
$$

được gọi là tương đương nếu tồn tại một đồng cấu $f$ của $g$ vào $g'$ sao cho biểu đồ sau đây:

$$
\begin{array}{ccccc}
a & \xrightarrow{\lambda} & g & \xrightarrow{\mu} & b \\
& & f \downarrow & & \\
& & g' & \xrightarrow{\mu'} & b \\
a & \xrightarrow{\lambda'} & g' & \xrightarrow{\mu'} & b
\end{array}
$$

là giao hoán (nghĩa là sao cho $f \circ \lambda = \lambda', \mu' \circ f = \mu$). Ta chỉ ra rằng một đồng cấu như thế tất yếu là song ánh. Trước hết $f$ là đơn ánh. Thật vậy, nếu $x \in g$ sao cho $f(x) = 0$, thì $\mu(x) = \mu'(f(x)) = 0$ và do đó $x = \lambda(y)$ với một $y \in a$ nào đó; khi đó $\lambda'(y) = f(\lambda(y)) = f(x) = 0$, suy ra $y = 0$ và vì thế $x = 0$. Mặt khác, $f$ là toàn ánh. Thật vậy, $\mu' \circ f = \mu$ là toàn ánh và do đó $f(g) + \lambda'(a) = g'$; mặt khác $f(g) \supset f(\lambda(a)) = \lambda'(a)$.

Từ đó suy ra rằng quan hệ vừa định nghĩa giữa hai mở rộng của $b$ bởi $a$ là một quan hệ tương đương.

#### Mệnh đề 6 {#lie-i-s1-prop-6 .statement}

Cho

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

là một mở rộng của $b$ bởi $a$ và $n$ là hạt nhân của nó.

(a) *Nếu tồn tại một đại số con m của g bù với n trong g, thì hạn chế của μ lên m là một đẳng cấu từ m lên b. Nếu ν ký hiệu đẳng cấu nghịch đảo của hạn chế này, thì ν là một đồng cấu từ b vào g và μ ∘ ν là tự đẳng cấu đồng nhất của b.*

(b) *Ngược lại, nếu tồn tại một đồng cấu ν từ b vào g sao cho μ ∘ ν là tự đẳng cấu đồng nhất của b, thì ν(b) là một đại số con bù với n trong g.*

Các khẳng định của (a) là ngay lập tức. Mặt khác, giả sử ν là một đồng cấu từ b vào g sao cho μ ∘ ν là tự đẳng cấu đồng nhất của b. Khi đó ν(b) là một đại số con của g và g là tổng trực tiếp của ν(b) và $\mu^{-1}(0) = n$ (*Đại số*, Chương VIII, § 1, no. 1).

#### Định nghĩa 6 {#lie-i-s1-def-6 .statement}

*Cho*

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

*là một mở rộng của b bởi a và n là hạt nhân của nó. Mở rộng này được gọi là không cốt yếu (tương ứng, tầm thường) nếu tồn tại một đại số con (tương ứng, một iđêan) của g bù với n trong g. Mở rộng này được gọi là trung tâm nếu n được chứa trong tâm của g.*

Nếu mở rộng là tầm thường, giả sử m là một iđêan của g bù với n trong g. Khi đó (xem no. 1) g được đồng nhất một cách chính tắc với đại số Lie m × n và do đó với đại số Lie a × b. Ngược lại, giả sử a và b là hai đại số Lie; khi đó a × b là một mở rộng tầm thường của a bởi b.

Một mở rộng trung tâm không cốt yếu là tầm thường. Thật vậy, giả sử g là một đại số Lie, n là một iđêan của g được chứa trong tâm của g và m là một đại số con của g bù với n trong g. Khi đó [m, g] = [m, m] + [m, n] = [m, m] ⊂ m và do đó m là một iđêan của g.

### 8. TÍCH NỬA TRỰC TIẾP

Cho a và b là hai đại số Lie trên K. Không dễ xây dựng tất cả các mở rộng của b bởi a. Nhưng chúng tôi sẽ mô tả khá đơn giản tất cả các mở rộng *không cốt yếu* của b bởi a.

Giả sử g là một mở rộng không cốt yếu của b bởi a. Ta đồng nhất a với một iđêan của g, b với một đại số con của g bù với a, và môđun g với môđun a × b. Với mọi $b \in b$, gọi $\phi_b$ là hạn chế lên a của $\mathrm{ad}_g\ b$; đó là một đạo hàm của a và ánh xạ $b \mapsto \phi_b$ là một đồng cấu từ b vào đại số Lie các đạo hàm của a. Mặt khác, với $a, a'$ trong a và $b, b'$ trong b, ta có:

$$
[(a, b), (a', b')] = [a + b, a' + b']
= [a, a'] + [a, b'] + [b, a'] + [b, b']
= ([a, a'] + \phi_b a' - \phi_{b'} a, [b, b']).
$$

Ngược lại, cho a và b là các đại số Lie trên K và $b \mapsto \phi_b$ là một đồng cấu từ b vào đại số Lie các phép đạo hàm của a. Trên tích *g của các K-môđun* a và b ta định nghĩa ngoặc của hai phần tử bằng cách viết:

$$
[(a, b), (a', b')] = ([a, a'] + \phi_b a' - \phi_{b'} a, [b, b'])
$$

với mọi $a, a'$ trong $a$, $b, b'$ trong $b$. Ngay lập tức thấy rằng ngoặc này là một hàm song tuyến tính phản xứng của $(a, b), (a', b')$; ta chứng minh rằng, với 3 phần tử $(a, b), (a', b'), (a'', b'')$ của $a \times b$:

(7)
$$
[(a, b), [(a', b'), (a'', b'')]] + [(a', b'), [(a'', b''), (a, b)]] \\
+ [(a'', b''), [(a, b), (a', b')]] = 0.
$$

Vì vế trái của (7) là một hàm tam tuyến tính phản xứng của $(a, b), (a', b'), (a'', b'')$, nên chỉ cần kiểm tra khi hệ các phần tử này có một trong các dạng sau:

(8) $(a, 0), (a', 0), (a'', 0)$

(9) $(a, 0), (a', 0), (0, b'')$

(10) $(a, 0), (0, b'), (0, b'')$

(11) $(0, b), (0, b'), (0, b'')$.

Trong các trường hợp (8) và (11), quan hệ (7) là một hệ quả ngay lập tức của đồng nhất thức Jacobi trong $a$ và $b$. Trong trường hợp (9), ta có

$$
[(a, 0), [(a', 0), (0, b'')]] = [(a, 0), (-\phi_{b''}a', 0)] = (-[a, \phi_{b''}a'], 0)
$$
$$
[(a', 0), [(0, b''), (a, 0)]] = [(a', 0), (\phi_{b''}a, 0)] = ([a', \phi_{b''}a], 0)
$$
$$
[(0, b''), [(a, 0), (a', 0)]] = [(0, b''), ([a, a'], 0)] = (\phi_{b''}([a, a']), 0)
$$

và quan hệ (7) suy ra từ đẳng thức:
$$
\phi_{b''}([a, a']) = [\phi_{b''}a, a'] + [a, \phi_{b''}a'].
$$

Trong trường hợp (10), ta có:

$$
[(a, 0), [(0, b'), (0, b'')]] = [(a, 0), (0, [b', b''])] = (-\phi_{[b', b'']}a, 0)
$$
$$
[(0, b'), [(0, b''), (a, 0)]] = [(0, b'), (\phi_{b''}a, 0)] = (\phi_{b'}\phi_{b''}a, 0)
$$
$$
[(0, b''), [(a, 0), (0, b')]] = [(0, b''), (-\phi_{b'}a, 0)] = (-\phi_{b''}\phi_{b'}a, 0)
$$

và quan hệ (7) suy ra từ đẳng thức:
$$
\phi_{[b', b'']} = \phi_{b'}\phi_{b''} - \phi_{b''}\phi_{b'}.
$$

Do đó một cấu trúc đại số Lie đã được xác định trên $g$. Ánh xạ $(a, b) \mapsto b$ từ $g$ lên $b$ là một đồng cấu $\mu$ mà hạt nhân $n$ của nó là iđêan các phần tử của $g$ có dạng $(a, 0)$. Ánh xạ $a \mapsto (a, 0)$ là một đẳng cấu $\lambda$ từ $a$ lên $n$. Do đó:

(12)
$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

là một mở rộng của $b$ bởi $a$ với hạt nhân $n$, và được gọi là *được xác định một cách chính tắc bởi* $a, b, \phi$. Ánh xạ $b \mapsto (0, b)$ là một đẳng cấu $\nu$ từ $b$ lên một đại số con của $g$ bù với $n$ trong $g$; do đó phép mở rộng là không cốt yếu.

Nếu $a$ được đồng nhất với $n$ theo $\lambda$ và $b$ với $v(b)$ theo $v$, thì, với $a \in a$ và $b \in b$:

$$
(\mathrm{ad}\ b).a = [(0, b), (a, 0)] = (\phi_b a, 0) = \phi_b a.
$$

Khi $\phi = 0$, $g$ là đại số Lie tích của $b$ và $a$. Trong trường hợp tổng quát, $g$ được gọi là *tích nửa trực tiếp của $b$ bởi $a$* (tương ứng với đồng cấu $b \mapsto \phi_b$ từ $b$ vào đại số Lie của các phép đạo của $a$).

Vậy ta đã thiết lập mệnh đề sau đây:

#### Mệnh đề 7 {#lie-i-s1-prop-7 .statement}

*Cho $a$ và $b$ là hai đại số Lie trên $K$,*

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

*một mở rộng không cốt yếu của $b$ bởi $a$, $\nu$ là một đẳng cấu từ $b$ lên một đại số con của $g$ sao cho $\mu \circ \nu$ là tự đẳng cấu đồng nhất của $b$ và $\phi$ là đồng cấu tương ứng từ $b$ vào đại số Lie các đạo phân của $a$.* Đặt

$$
a \xrightarrow{\lambda_0} g_0 \xrightarrow{\mu_0} b
$$

*là mở rộng không thiết yếu của $b$ bởi $a$ được $\phi$ xác định một cách chính tắc.* Khi đó ánh xạ $(a, b) \mapsto \lambda(a) + \nu(b)$ là một đẳng cấu $f$ từ $g_0$ lên $g$ và biểu đồ sau

$$
\begin{array}{ccccc}
& & \\
a & \xrightarrow{\lambda_0} & g_0 & \xrightarrow{\mu_0} & b \\
& \searrow f & \downarrow & \nearrow \mu_0 \\
& & g & & \\
& \swarrow i & & \searrow \mu \\
& & & &
\end{array}
$$

*là giao hoán, vì thế hai mở rộng là tương đương.*

#### Ví dụ 1 {#lie-i-s1-n8-exa-1 .statement}

Cho $g$ là một đại số Lie trên $K$ và $D$ là một đạo hàm của $g$. Cho $h$ là đại số Lie *giao hoán* $K$. Ánh xạ $\lambda \mapsto \lambda D (\lambda \in K)$ là một đồng cấu từ $h$ vào đại số Lie các đạo hàm của $g$. Ta lập tích nửa trực tiếp tương ứng $t$ của $h$ bởi $g$. Cho $x_0$ là phần tử $(0, 1)$ của $t$. Với mọi $x \in g$, $Dx = [x_0, x]$.

#### Ví dụ 2 {#lie-i-s1-n8-exa-2 .statement}

Cho $g$ là một đại số Lie trên $K$, $M$ là một $K$-môđun và $\rho$ là một đồng cấu từ $g$ vào $\mathfrak{gl}(M)$. Nếu coi $M$ như một đại số Lie giao hoán, thì đại số Lie các phép dẫn của $M$ là $\mathfrak{gl}(M)$. Do đó ta có thể lập tích nửa trực tiếp $h$ của $g$ bởi $M$ tương ứng với $\rho$.

Đặc biệt, cho $g = \mathfrak{gl}(M)$ và $\rho$ là ánh xạ đồng nhất của $\mathfrak{gl}(M)$. Tích nửa trực tiếp của $g$ bởi $M$ khi đó được ký hiệu là $\mathfrak{af}(M)$ (hoặc $\mathfrak{af}(n, K)$ nếu $M = K^n$). Một phần tử của $\mathfrak{af}(M)$ là một cặp có thứ tự $(m, u)$, trong đó $m \in M, u \in \mathfrak{gl}(M)$; và dấu ngoặc được xác định bởi

$$
[(m, u), (m', u')] = (u(m') - u'(m), [u, u']).
$$

*Khi M là một không gian vectơ hữu hạn chiều trên $\mathbf{R}$, $\mathfrak{af}(M)$ được đồng nhất một cách chính tắc với đại số Lie của *nhóm afin* của M.*

Cho $t$ là một đại số Lie trên K. Một ánh xạ tuyến tính $\theta$ từ $t$ vào $\mathfrak{af}(M)$ có thể được viết $x \mapsto ((\zeta(x), \eta(x)))$, trong đó $\zeta$ là một ánh xạ tuyến tính từ $t$ vào $M$ và $\eta$ là một ánh xạ tuyến tính từ $t$ vào $gl(M)$. Ta xét các điều kiện mà $\zeta$ và $\eta$ phải thỏa mãn để $\theta$ là một đồng cấu. Với $x \in t, y \in t$, ta phải có

$$
\theta([x, y]) = [\theta(x), \theta(y)]
$$

nghĩa là

$$
(\zeta([x, y]), \eta([x, y])) = [(\zeta(x), \eta(x)), (\zeta(y), \eta(y))] \\
= (\eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x), [\eta(x), \eta(y)]).
$$

Vậy để $\theta$ là một đồng cấu từ $t$ vào $\mathfrak{af}(M)$, điều kiện cần và đủ là $\eta$ là một đồng cấu từ $t$ vào $gl(M)$ và $\zeta$ thỏa mãn quan hệ:

(13)
$$
\zeta([x, y]) = \eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x).
$$

Cho N là K-môđun $M \times K$. Ta lấy $t$ là đại số con của $gl(N)$ gồm các $w \in gl(N)$ sao cho $w(N) \subset M$. Với mọi $w \in t$, gọi $\eta(w) \in gl(M)$ là hạn chế của $w$ trên $M$ và đặt $\zeta(w) = w(0, 1) \in M$. Với $w_1 \in t, w_2 \in t$,

$$
\zeta([w_1, w_2]) = w_1(\zeta(w_2)) - w_2(\zeta(w_1)) = \eta(w_1) \cdot \zeta(w_2) - \eta(w_2) \cdot \zeta(w_1).
$$

Vì vậy ánh xạ $w \mapsto (\zeta(w)), \eta(w))$ là một đồng cấu $\theta$ của $t$ vào $\mathfrak{af}(M)$. Rõ ràng $\theta$ là *song ánh*. Đặt $\phi = \theta^{-1}$. Nếu $(m, u) \in \mathfrak{af}(M)$, thì $\phi(m, u)$ là phần tử $w$ của $t$ được xác định bởi

$$
w(m', \lambda) = (u(m') + \lambda m, 0).
$$

$\mathfrak{af}(M)$ thường được đồng nhất với đại số con $t$ của $gl(N)$ qua đẳng cấu $\phi$.

*Khi M là một không gian vectơ hữu hạn chiều trên $\mathbf{R}$, đồng cấu $\phi$ từ $\mathfrak{af}(M)$ vào $gl(N)$ tương ứng với một đồng cấu chính tắc $\psi$ từ nhóm afin A của M vào nhóm $\mathbf{GL}(N)$; nếu $a \in A, \psi(a)$ là phần tử duy nhất $g$ của $\mathbf{GL}(N)$ sao cho $g(m, 1) = (a(m), 1)$ với mọi $m \in M$. Đồng cấu này là đơn ánh và $\psi(A)$ là tập hợp các tự đẳng cấu của N bảo toàn mọi đa tạp tuyến tính của N song song với M.*

### 9. THAY ĐỔI VÀNH CƠ SỞ

Cho $K_0$ là một vành giao hoán có phần tử đơn vị và $\rho$ là một đồng cấu từ $K_0$ vào K ánh xạ phần tử đơn vị tới phần tử đơn vị. Cho $g$ là một đại số Lie trên K. Gọi $g'$ là đại số thu được khi coi $g$ như một đại số trên $K_0$ bởi $\rho$ (x. no. 1). Khi đó $g'$ là một đại số Lie. Các đại số con (tương ứng, các iđêan) của $g$ là các đại số con (tương ứng, các iđêan) của $g'$. Nếu $a$ và $b$ là các môđun con của $g$, thì ngoặc $[a, b]$ là như nhau trong $g$ và trong $g'$; vì $[a, b]$ là tập hợp các phần tử có dạng

$$
\sum_{i=1}^n [x_i, y_i]
$$

trong đó $x_i \in a, y_i \in b$. Suy ra $\mathcal{D}^p g = \mathcal{D}^p g', \mathcal{C}^p g = \mathcal{C}^p g'$ với mọi $p$.

Bộ trung tâm hóa của một tập con là như nhau trong $g$ và $g'$. Do đó $\mathcal{C}_p g = \mathcal{C}_p g'$ với mọi $p$.

Cho $K_1$ là một vành giao hoán có phần tử đơn vị và $\sigma$ là một đồng cấu của $K$ vào $K_1$ ánh xạ phần tử đơn vị lên phần tử đơn vị. Cho $g$ là một đại số Lie trên $K$. Gọi $g_{(K_1)}$ là đại số trên $K_1$ dẫn xuất từ $g$ bằng cách mở rộng vành cơ sở (x. no. 1). Khi đó $g_{(K_1)}$ là một đại số Lie. Nếu $a$ là một đại số con (tương ứng, một iđêan) của $g$, thì ảnh chính tắc của $a_{(K_1)}$ trong $g_{(K_1)}$ là một đại số con (tương ứng, một iđêan) của $g_{(K_1)}$. Nếu $a$ và $b$ là các môđun con của $g$, thì ảnh chính tắc trong $g_{(K_1)}$ của $[a, b]_{(K_1)}$ bằng ngoặc của các ảnh chính tắc của $a_{(K_1)}$ và $b_{(K_1)}$. Suy ra $\mathcal{D}^p(g_{(K_1)})$ là ảnh chính tắc của $(\mathcal{D}^p g)_{(K_1)}$ và $\mathcal{C}^p(g_{(K_1)})$ là ảnh chính tắc của $\mathcal{C}^p(g_{(K_1)})$.

Nếu $K$ là một trường, $K_1$ là một trường mở rộng của $K$ và $\sigma$ là đơn ánh chính tắc của $K$ vào $K_1$, thì với các đồng nhất thông thường ta có
$$
[a, b]_{(K_1)} = [a_{(K_1)}, b_{(K_1)}], \quad \mathcal{D}^p(g_{(K_1)}) = (\mathcal{D}^p g)_{(K_1)},
$$
$$
\mathcal{C}^p(g_{(K_1)}) = (\mathcal{C}^p g)_{(K_1)}.
$$

Các kết quả này được hoàn chỉnh trong § 2, no. 9.

Nếu $M$ là một không gian vectơ hữu hạn chiều trên trường $K$, thì $M_{(K_1)}$ là một không gian vectơ hữu hạn chiều trên $K_1$ và đại số kết hợp $\mathcal{L}(M_{(K_1)})$ được đồng nhất một cách chính tắc với đại số kết hợp $\mathcal{L}(M)_{(K_1)}$. Do đó đại số Lie $gl(M_{(K_1)})$ được đồng nhất một cách chính tắc với đại số Lie $gl(M)_{(K_1)}$.

### Bài tập {#lie-i-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
