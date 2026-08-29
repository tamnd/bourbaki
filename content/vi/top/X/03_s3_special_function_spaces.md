---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 3
section_title: Special function spaces
lang: vi
source: top-v-x
pdf_pages: 0299-0314, 0333-0343
extraction: ocr
subsections:
    - "no": 1
      title: SPACES OF MAPPINGS INTO A METRIC SPACE
      page: 0
      pdf_page: 299
    - "no": 2
      title: SPACES OF MAPPINGS INTO A NORMED SPACE
      page: 0
      pdf_page: 301
    - "no": 3
      title: COUNTABILITY PROPERTIES OF SPACES OF CONTINUOUS FUNCTIONS
      page: 0
      pdf_page: 304
    - "no": 4
      title: THE COMPACT-OPEN TOPOLOGY
      page: 0
      pdf_page: 306
    - "no": 5
      title: TOPOLOGIES ON GROUPS OF HOMEOMORPHISMS
      page: 0
      pdf_page: 311
statements: 31
exercises: 10
content_sha256: 959d51e0b17c1e53acd1b04ec5addba3190172ba3449001ca8efef0e093433a6
translated_from: content/en/top/X/03_s3_special_function_spaces.md
source_content_sha256: 0242e85ddd5aef10eee50cb9154a8440bef872dc1313f8c42d3c58a661af6a30
translation_model: gpt-5.4, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-db4d7dc7
glossary_version: 34
glossary_terms_sha256: 1726272806081c8b29f42eaf4ad44250975f26a010bf0d168e42f204df71de36
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC KHÔNG GIAN HÀM ĐẶC BIỆT

### 1. CÁC KHÔNG GIAN ÁNH XẠ VÀO MỘT KHÔNG GIAN MÊTRIC

Cho $X$ là một tập hợp, $Y$ là một không gian đều, $(f_i)_{i \in I}$ là một họ giả mêtric xác định cấu trúc đều của $Y$ (Chương IX, § 1, no. 4), và $\mathcal{S}$ là một tập hợp các tập con của $X$. Với mỗi $i \in I$, mỗi tập hợp $A \in \mathcal{S}$, và mỗi cặp $(u, v)$ các ánh xạ từ $X$ vào $Y$, viết

$$
g_{i, A}(u, v) = \sup_{x \in A} f_i(u(x), v(x));
$$

ngay lập tức suy ra rằng $g_{i, A}$ là một *giả mêtric* trên $\mathcal{F}(X; Y)$ và rằng họ các giả mêtric $(g_{i, A})_{i \in I, A \in \mathcal{S}}$ xác định cấu trúc đều của sự *hội tụ* theo $\mathcal{S}$ trên $\mathcal{F}(X; Y)$. Đặc biệt:

#### Mệnh đề 1 {#top-x-s3-prop-1 .statement}

*Nếu $Y$ là một không gian đều mêtric hóa được, thì cấu trúc đều của sự hội tụ đều trên $\mathcal{F}(X; Y)$ là mêtric hóa được.*

Thật vậy, nếu $d$ là một mêtric trên $Y$ tương thích với cấu trúc đều của nó, thì cấu trúc của sự hội tụ đều trên $\mathcal{F}(X; Y)$ được xác định bởi giả mêtric duy nhất

$$
\varepsilon(u, v) = \sup_{x \in X} d(u(x), v(x));
$$

nói chung giả mêtric này không hữu hạn, nhưng nó tương đương với một giả mêtric hữu hạn (Chương IX, § 1, no. 2), và vì cấu trúc đều của sự hội tụ đều là Hausdorff (§ 1, no. 2, Mệnh đề 1), nên nó là mêtric hóa được.

#### Hệ quả {#top-x-s3-n1-cor-1 .statement}

Cho $X$ là một không gian tôpô và $Y$ là một không gian đều mêtric hóa được. Giả sử rằng tồn tại một dãy $(K_n)$ các tập con compact của $X$ sao cho mọi tập con compact của $X$ đều được chứa trong một $K_n$ nào đó. Khi đó cấu trúc đều của sự hội tụ compact trên $\mathcal{F}(X; Y)$ là mêtric hóa được.

Vì các $K_n$ phủ $X$, $\mathcal{F}_c(X; Y)$ đẳng cấu với một không gian con đều của $\prod_n \mathcal{F}_u(K_n; Y)$ ($§ 1$, no. 2, Nhận xét 3), và do đó hệ quả suy ra từ Mệnh đề 1 (Chương IX, § 2, no. 4, Định lý 1, Hệ quả 2).

Chú ý rằng hệ quả này áp dụng đặc biệt khi $X$ là *địa phương compact và σ-compact* (Chương I, § 9, no. 9, Mệnh đề 15, Hệ quả 1).

Bây giờ cho $Y$ là một không gian mêtric và $d$ là mêtric của nó. Nếu $X$ là một tập hợp bất kỳ và $\mathcal{S}$ là một tập hợp bất kỳ các tập con của $X$, ta sẽ ký hiệu bởi $\mathcal{B}_{\mathcal{S}}(X; Y)$ tập hợp tất cả các ánh xạ $u : X \to Y$ sao cho $u(A)$ là *bị chặn* với mỗi $A \in \mathcal{S}$. Trừ khi nói rõ điều ngược lại, ta sẽ xem $\mathcal{B}_{\mathcal{S}}(X; Y)$ được trang bị cấu trúc đều của sự hội tụ theo $\mathcal{S}$, được xác định bởi họ giả mêtric sau trên $\mathcal{B}_{\mathcal{S}}(X; Y)$:

$$
d_A(u, v) = \sup_{x \in A} d(u(x), v(x)) \tag{$A \in \mathcal{S}$}
$$

chúng là *hữu hạn* theo giả thiết. Khi $\mathcal{S} = \{X\}$, ta viết $\mathcal{B}(X; Y)$ thay cho $\mathcal{B}_{\mathcal{S}}(X; Y)$. Một ánh xạ $u : X \to Y$ được gọi là *bị chặn* nếu nó thuộc $\mathcal{B}(X; Y)$, tức là nếu $u(X)$ là một tập con bị chặn của $Y$.

#### Mệnh đề 2 {#top-x-s3-prop-2 .statement}

Cho $X$ là một tập hợp và $Y$ là một không gian mêtric. Tập hợp $\mathcal{B}(X; Y)$ các ánh xạ bị chặn vừa mở vừa đóng trong không gian $\mathcal{F}_u(X; Y)$.

Nếu $u$ bị chặn, thì mọi ánh xạ $v : X \to Y$ sao cho với mọi $x \in X$, ta có $d(u(x), v(x)) \leq 1$ đều bị chặn, vì

$$
d(v(x), v(x_0)) \leq d(u(x), u(x_0)) + 2;
$$

do đó $\mathcal{B}(X; Y)$ là mở. Mặt khác, nếu $u$ nằm trong bao đóng của $\mathcal{B}(X; Y)$ trong $\mathcal{F}_u(X; Y)$, thì có một ánh xạ $u_0 \in \mathcal{B}(X; Y)$ sao cho $d(u(x), u_0(x)) \leq 1$ với mọi $x \in X$; do đó $u$ bị chặn.

#### Hệ quả 1 {#top-x-s3-prop-2-cor-1 .statement}

Cho $X$ là một tập hợp và $Y$ là một không gian mêtric. Khi đó $\mathcal{B}_{\mathcal{S}}(X; Y)$ là đóng trong $\mathcal{F}_{\mathcal{S}}(X; Y)$. Đặc biệt, nếu $Y$ đầy đủ thì $\mathcal{B}_{\mathcal{S}}(X; Y)$ đầy đủ đối với cấu trúc đều của sự hội tụ $\mathcal{S}$.

Vì $\mathcal{B}_\mathfrak{S}(X; Y)$ là ảnh ngược của tập con $\prod_{A \in \mathfrak{S}} \mathcal{B}(A; Y)$ của tích $\prod_{A \in \mathfrak{S}} \mathcal{F}_u(X; Y)$ qua ánh xạ chính tắc của $\mathcal{F}_\mathfrak{S}(X; Y)$ vào $\prod_{A \in \mathfrak{S}} \mathcal{F}_u(A; Y)$; mệnh đề thứ nhất do đó suy ra từ § 1, no. 2, Nhận xét 3, và mệnh đề thứ hai suy ra từ mệnh đề thứ nhất, nếu ta tính đến Định lý 1 của § 1, no. 5.

#### Hệ quả 2 {#top-x-s3-prop-2-cor-2 .statement}

*Cho X là một không gian tôpô và Y là một không gian mêtric. Khi đó không gian của tất cả các ánh xạ liên tục bị chặn của X vào Y vừa mở vừa đóng trong $C_u(X; Y)$; nó đầy đủ nếu Y đầy đủ.*

Không gian được xét là $\mathcal{B}(X; Y) \cap C_u(X; Y)$; mệnh đề thứ nhất suy ra từ Mệnh đề 2; mệnh đề thứ hai suy ra từ mệnh đề thứ nhất ($§ 1$, no. 6, Định lý 2, Hệ quả 1).

### 2. CÁC KHÔNG GIAN CỦA CÁC ÁNH XẠ VÀO MỘT KHÔNG GIAN CÓ CHUẨN

Xét cụ thể hơn tình huống trong đó Y là một không gian vectơ *có chuẩn* trên một vành chia định giá không rời rạc K (Chương IX, § 3, no. 3). Ta ký hiệu $||y||$ là chuẩn của $y \in Y$. Tập hợp $\mathcal{F}(X; Y) = Y^X$ khi đó được trang bị một cách chính tắc một cấu trúc không gian vectơ trên K. Một ánh xạ $u : X \to Y$ bị chặn khi và chỉ khi hàm thực $x \mapsto ||u(x)||$ bị chặn trong X. Nếu $u, v$ là các ánh xạ bị chặn của X vào Y, hiển nhiên rằng $u + v$ và $\lambda u (\lambda \in K)$ bị chặn; nói cách khác, $\mathcal{B}(X; Y)$ là một *không gian con vectơ* của $\mathcal{F}(X; Y)$. Hơn nữa, $||u|| = \sup_{x \in X} ||u(x)||$ là một *chuẩn* trên $\mathcal{B}(X; Y)$; vì nó thỏa mãn bất đẳng thức tam giác và $||u|| = 0$ kéo theo $u = 0$, và với mỗi $\lambda \in K$ ta có

$$
||\lambda u|| = \sup_{x \in X} ||\lambda u(x)|| = \sup_{x \in X} |\lambda| \cdot ||u(x)|| = |\lambda| \cdot \sup_{x \in X} ||u(x)|| = |\lambda| \cdot ||u||.
$$

Hơn nữa, ta kiểm tra ngay lập tức rằng cấu trúc đều trên $\mathcal{B}(X; Y)$ được xác định bởi chuẩn này là cấu trúc đều của sự hội tụ đều. Trừ khi điều ngược lại được phát biểu rõ ràng, mỗi khi $\mathcal{B}(X; Y)$ được xem như một không gian có chuẩn, thì chính chuẩn được xác định ở trên là chuẩn đang được xét.

#### Mệnh đề 3 {#top-x-s3-prop-3 .statement}

*Nếu không gian có chuẩn Y đầy đủ, thì mọi chuỗi $(u_n)$ các ánh xạ bị chặn của X vào Y hội tụ tuyệt đối trong không gian có chuẩn $\mathcal{B}(X; Y)$ (nghĩa là thỏa mãn $\sum_{n=0}^\infty ||u_n|| < +\infty$; xem Chương IX, § 3, no. 6) đều hội tụ đều trong X.*

Vì $\mathcal{B}(X; Y)$ đầy đủ (no. 1, Mệnh đề 2, Hệ quả 1), kết quả suy ra từ Chương IX, § 3, no. 6, Mệnh đề 11 và định nghĩa của một chuỗi hội tụ đều.

#### Nhận xét 1 {#top-x-s3-n2-rem-1 .statement}

Nếu $\sum_{n=0}^{\infty} \|u_n\| < +\infty$, thì $\sum_{n=0}^{\infty} |u_n(x)| \leq \sum_{n=0}^{\infty} |u_n| < +\infty$
với mỗi $x \in X$; nói cách khác, với mỗi $x \in X$ chuỗi có số hạng tổng quát $u_n(x)$ hội tụ tuyệt đối trong không gian $Y$. Đảo lại không đúng. Để tránh mọi sự nhầm lẫn, đôi khi ta sẽ nói rằng chuỗi có số hạng tổng quát $u_n$ là *hội tụ chuẩn*, nghĩa là chuỗi có số hạng tổng quát $\|u_n\|$ là hội tụ. Một chuỗi có thể hội tụ đều trong $X$ mà không hội tụ chuẩn; chẳng hạn, đây là trường hợp của chuỗi $(u_n)$ trong không gian $\mathcal{B}(\mathbf{R}, \mathbf{R})$, được định nghĩa như sau:
$u_n(x) = (1/n) \sin x$ nếu $x \in [n\pi, (n+1)\pi]$, $u_n(x) = 0$ nếu không.

Khi $Y$ là một *đại số chuẩn* (Chương IX, § 3, no. 7) trên một trường định giá không rời rạc $K$, thì $\mathcal{B}(X; Y)$ là một $K$-đại số, và chuẩn $\|u\|$ tương thích với cấu trúc đại số, vì
$$
\|uv\| = \sup_{x \in X} \|u(x)v(x)\| \leq \sup_{x \in X} \|u(x)\| \cdot \|v(x)\|
\leq \sup_{x \in X} \|u(x)\| \cdot \sup_{x \in X} \|v(x)\| = \|u\| \cdot \|v\|.
$$
Do đó $\mathcal{B}(X; Y)$ bây giờ là một *đại số chuẩn* trên $K$.

#### Mệnh đề 4 {#top-x-s3-prop-4 .statement}

*Cho $X_i$ ($1 \leq i \leq n$) và $Y$ là các không gian vectơ có chuẩn trên một vành chia định giá không rời rạc $K$, và cho $X = \prod_{i=1}^n X_i$. Khi đó tập hợp tất cả các ánh xạ đa tuyến tính từ $X$ vào $Y$ là đóng trong không gian $\mathcal{F}_s(X; Y)$.*

Tập hợp này gồm tất cả các $u \in F(X; Y)$ thỏa mãn tất cả các hệ thức
$$
\begin{align*}
u(x_1, \ldots, x_i' + x_i'', \ldots, x_n) &= u(x_1, \ldots, x_i', \ldots, x_n) \\
&\quad + u(x_1, \ldots, x_i'', \ldots, x_n), \\
u(x_1, \ldots, \lambda x_i, \ldots, x_n) &= \lambda u(x_1, \ldots, x_i, \ldots, x_n)
\end{align*}
$$
($1 \leq i \leq n,\ x_i,\ x_i',\ x_i''$ là các phần tử tùy ý của $X_i$, $\lambda$ là một phần tử tùy ý của $K$); vì hai vế của các hệ thức (1) là các hàm liên tục của $u$ trên $\mathcal{F}_s(X; Y)$ (§ 1, no. 2, Nhận xét 6), kết quả suy ra (Chương I, § 8, no. 1, Mệnh đề 2).

#### Mệnh đề 5 {#top-x-s3-prop-5 .statement}

*Dưới các giả thiết của Mệnh đề 4, tập hợp $\mathcal{L}(X_1, \ldots, X_n; Y)$ gồm các ánh xạ đa tuyến tính liên tục từ $X$ vào $Y$ là đóng trong $\mathcal{F}(X; Y)$ đối với tôpô của hội tụ bị chặn; nó là đầy đủ đối với tính đều của hội tụ bị chặn nếu $Y$ là đầy đủ.*

Vì nếu $\mathcal{G}$ là tập hợp tất cả các tập con bị chặn của $X$, thì $\mathcal{L}(X_1, \ldots, X_n; Y)$ là giao của tập hợp tất cả các ánh xạ đa tuyến tính từ $X$ vào $Y$ và tập hợp $\mathcal{B}_\mathcal{G}(X; Y)$ (Chương IX, § 3, no. 5, Định lý 1); do đó kết quả suy ra từ Mệnh đề 4 và Mệnh đề 2, Hệ quả 1.

Trong phần còn lại của tiểu mục này, $K$ ký hiệu một trường định giá không rời rạc.

Khi đó $\mathcal{L}(X_1, \ldots, X_n; Y)$ là một không gian con vectơ của $\mathcal{F}(X; Y)$. Gọi $B$ là quả cầu đơn vị trong $X$, tập hợp tất cả các $(x_i)_{1 \leq i \leq n}$ sao cho $\sup_{1 \leq i \leq n} \|x_i\| \leq 1$.

Khi đó ánh xạ $u \to u|B$ từ $\mathcal{L}(X_1, \ldots, X_n; Y)$ vào $\mathcal{B}(B; Y)$ là đơn ánh; hơn nữa, ảnh ngược, qua ánh xạ này, của cấu trúc đều hội tụ đều trên $\mathcal{B}(B; Y)$ là cấu trúc đều hội tụ bị chặn trên $\mathcal{L}(X_1, \ldots, X_n; Y)$. Vì mọi tập con bị chặn của $X$ đều được chứa trong một tập có dạng $\mu B$ (với một $\mu \in K^*$ nào đó), và nếu $u$ là một phần tử của $\mathcal{L}(X_1, \ldots, X_n; Y)$, nói rằng $\|u(z)\| \leq a$ với mọi $z \in \mu B$ tương đương với nói rằng $\|u(z)\| \leq a/|\mu|^n$ với mọi $z \in B$. Người ta dễ dàng kiểm tra rằng số
$$
\|u\| = \sup_{z \neq 0} \frac{\|u(z)\|}{\|z\|}
$$
là một chuẩn trên $\mathcal{L}(X_1, \ldots, X_n; Y)$ và xác định cấu trúc đều hội tụ bị chặn trên tập hợp này, và rõ ràng ta có
$$
(2) \quad \|u(x_1, \ldots, x_n)\| \leq \|u\| \cdot \|x_1\| \cdots \|x_n\|.
$$

Trừ khi điều ngược lại được phát biểu rõ ràng, bất cứ khi nào $\mathcal{L}(X_1, \ldots, X_n; Y)$ được xét như một không gian định chuẩn, thì chuẩn được định nghĩa ở trên là chuẩn đang được xét.

#### Mệnh đề 6 {#top-x-s3-prop-6 .statement}

*Ánh xạ đa tuyến tính*
$$
(u, x_1, \ldots, x_n) \to u(x_1, \ldots, x_n)
$$
*của không gian định chuẩn* $\mathcal{L}(X_1, \ldots, X_n; Y) \times X_1 \times \cdots \times X_n$ *vào* $Y$ *là liên tục*.

Đây là một hệ quả ngay lập tức của bất đẳng thức (2) (Chương IX, § 3, no. 5, Định lý 1).

#### Mệnh đề 7 {#top-x-s3-prop-7 .statement}

*Cho* $X, Y, Z$ *là ba không gian định chuẩn trên* $K$. *Ánh xạ chính tắc của không gian định chuẩn* $\mathcal{L}(X, Y; Z)$ *vào không gian các ánh xạ tuyến tính từ* $X$ *vào* $\mathcal{L}(Y; Z)$ *gửi mỗi* $u \in \mathcal{L}(X, Y; Z)$ *thành ánh xạ* $x \to u(x, .)$ *là một đẳng cự từ* $\mathcal{L}(X; Y; Z)$ *lên* $\mathcal{L}(X; \mathcal{L}(Y; Z))$.

Điều này suy ra ngay lập tức từ các định nghĩa và quan hệ
$$
\sup_{\|x\| \leq 1} \left( \sup_{\|y\| \leq 1} \|u(x, y)\| \right) = \sup_{\|x\| \leq 1, \|y\| \leq 1} \|u(x, y)\|.
$$

#### Mệnh đề 8 {#top-x-s3-prop-8 .statement}

Cho $X, Y, Z$ là ba không gian định chuẩn trên $K$. Ánh xạ song tuyến tính $(u, v) \to v \circ u$ của $\mathcal{L}(X; Y) \times \mathcal{L}(Y; Z)$ vào $\mathcal{L}(X; Z)$ là liên tục.

Vì nếu $u \in \mathcal{L}(X; Y)$ và $v \in \mathcal{L}(Y; Z)$ thì ta có
$$
||v \circ u|| \leq ||u|| \cdot ||v||,
$$
vì với mọi $x \in X$ ta có $||v(u(x))|| \leq ||v|| \cdot ||u(x)|| \leq ||v|| \cdot ||u|| \cdot ||x||$ do (2).

Đặc biệt, trên tập hợp $\mathcal{L}(X)$ các tự đồng cấu liên tục của một không gian định chuẩn $X$ trên $K$, chuẩn $||u||$ tương thích với cấu trúc đại số-$K$ của $\mathcal{L}(X)$.

#### Nhận xét 2 {#top-x-s3-n2-rem-2 .statement}

Tập hợp $\mathcal{L}(\mathbf{R}^m; \mathbf{R}^n)$ các ánh xạ tuyến tính (tất nhiên là liên tục) từ $\mathbf{R}^m$ vào $\mathbf{R}^n$ có thể được đồng nhất với tập hợp $M_{n,m}(\mathbf{R})$ các ma trận có $n$ hàng và $m$ cột với các hệ số trong $\mathbf{R}$ và do đó có thể được đồng nhất với $\mathbf{R}^{mn}$; trên $\mathcal{L}(\mathbf{R}^m; \mathbf{R}^n)$, cấu trúc đều của hội tụ bị chặn (đối với mêtric Euclid trên $\mathbf{R}^m$), của hội tụ compact và của hội tụ từng điểm khi đó được đồng nhất với cấu trúc đều *cộng tính* trên $\mathbf{R}^{mn}$. Lấy chuẩn của $x = (x_i) \in \mathbf{R}^n$ là
$$
||x|| = \sup_i |x_i|,
$$
và gọi $(e_j)$ là cơ sở chính tắc của $\mathbf{R}^m$; nếu $u$ và $v$ là hai ánh xạ tuyến tính từ $\mathbf{R}^m$ vào $\mathbf{R}^n$ sao cho $\|u(e_j) - v(e_j)\| \leq \epsilon$ với $1 \leq j \leq m$, thì ta có $|\alpha_{ij} - \beta_{ij}| \leq \epsilon$ với mỗi cặp $(i, j)$ [$U = (\alpha_{ij})$ và $V = (\beta_{ij})$ lần lượt là các ma trận của $u, v$]; và ngược lại, nếu các bất đẳng thức này được thỏa mãn, ta có $\|u(x) - v(x)\| \leq ma\epsilon$ với mọi điểm $x$ của một hình lập phương tâm o và cạnh $a$ trong $\mathbf{R}^m$.

### 3. CÁC TÍNH CHẤT ĐẾM ĐƯỢC CỦA CÁC KHÔNG GIAN CÁC HÀM LIÊN TỤC

#### Định lý 1 {#top-x-s3-thm-1 .statement}

Cho $X$ là một không gian compact.
a) *Nếu $X$ là mêtric hóa được và nếu $Y$ là một không gian đều mêtric hóa được bất kỳ có kiểu đếm được* (Chương IX, § 2, no. 8), *thì không gian mêtric hóa được $C_u(X; Y)$ gồm các ánh xạ liên tục từ $X$ vào $Y$, được trang bị tôpô hội tụ đều, có kiểu đếm được*.
b) *Ngược lại, nếu không gian mêtric hóa được $C_u(X; \mathbf{R})$ có kiểu đếm được, thì $X$ là mêtric hóa được*.

a) Cho $d$ (resp. $d'$) là một metric tương thích với tôpô của $X$ (resp. với cấu trúc đều của $Y$); khi đó $\delta(f, g) = \sup_{x \in X} d'(f(x), g(x))$ là một metric xác định cấu trúc đều của sự hội tụ đều trên không gian $C(X; Y)$, các hàm của $C(X; Y)$ bị chặn vì $X$ compact (no. 1). Với mỗi cặp số nguyên $m > 0, n > 0$, cho $G_{mn}$ là tập hợp các hàm $f \in \mathcal{C}(X; Y)$ sao cho quan hệ $d(x, x') \leq 1/m$ kéo theo $d(f(x), f(x')) \leq 1/n$. Mọi hàm $f \in \mathcal{C}(X; Y)$ đều liên tục đều (chương II, § 4, no. 1, định lý 2) và do đó, với mỗi $n > 0$, $\mathcal{C}(X; Y)$ là hợp của các tập hợp $G_{mn}$ ($m > 0$). Cho $\{a_1, \ldots, a_{p(m)}\}$ là một tập con hữu hạn của $X$ sao cho các quả cầu mở có tâm $a_i$ và bán kính $1/m$ phủ $X$ ($1 \leq i \leq p(m)$); và cho $(b_r)_{r \in \mathbf{N}}$ là một dãy đếm được trù mật trong $Y$. Với mỗi ánh xạ $\varphi : [1, p(m)] \to \mathbf{N}$, cho $H_\varphi$ là tập hợp các $f \in G_{mn}$ sao cho $d'(f(a_k), b_{\varphi(k)}) \leq 1/n$ với $1 \leq k \leq p(m)$. Theo định nghĩa của các $b_r$, $G_{mn}$ là hợp của các tập hợp $H_\varphi$ với $\varphi \in \mathbf{N}^{p(m)}$; cho $C_{mn}$ là tập hợp các ánh xạ $\varphi \in \mathbf{N}^{p(m)}$ sao cho $H_\varphi \neq \emptyset$, và với mỗi $\varphi \in C_{mn}$ cho $g_\varphi$ là một phần tử của $H_\varphi$; cuối cùng, ký hiệu $L_{mn}$ là tập hợp đếm được các $g_\varphi$ với $\varphi \in C_{mn}$. Cho $f \in G_{mn}$, và cho $\varphi$ là một phần tử của $C_{mn}$ sao cho $f \in H_\varphi$; khi đó ngay lập tức từ các định nghĩa ta có $d'(f(x), g_\varphi(x)) \leq 4/n$ với mọi $x \in X$, tức là $\delta(f, g_\varphi) \leq 4/n$. Do đó hợp của các tập hợp $L_{mn}$ là trù mật trong $\mathcal{C}_u(X; Y)$, vì với mỗi số nguyên $n > 0$ và mỗi $f \in \mathcal{C}(X; Y)$ tồn tại $m$ sao cho $f \in G_{mn}$, và ta vừa thấy rằng khoảng cách từ $f$ đến $L_{mn}$ là $\leq 4/n$.

b) Cho $I = [0, 1]$. Vì $\mathcal{C}_u(X; I)$ là một không gian con đều của $\mathcal{C}_u(X; \mathbf{R})$, nên nó có kiểu đếm được. Gọi $(f_n)$ là một dãy trù mật trong $\mathcal{C}_u(X; I)$. Xét không gian tích $K = \mathbf{N}$ và ánh xạ $\psi : x \to (f_n(x))$ của $X$ vào $K$, hiển nhiên liên tục. Ánh xạ $\psi$ là đơn ánh; thật vậy, theo định nghĩa của dãy $(f_n)$, quan hệ $f_n(x) = f_n(x')$ với mọi $n$ suy ra, khi chuyển qua giới hạn, $f(x) = f(x')$ với mọi hàm $f \in \mathcal{C}(X; I)$; nhưng điều này là không thể nếu $x \neq x'$ theo Tiên đề (OIV) áp dụng cho điểm $x$ và cho một lân cận $V$ của $x$ không chứa $x'$ (Chương IX, § 1, no. 5, Định lý 2). Suy ra rằng không gian compact $X$ đồng phôi với không gian con $\psi(X)$ của $K$ (Chương I, § 9, no. 4, Định lý 2, Hệ quả 2); vì $K$ mêtric hóa được và có kiểu đếm được, $\psi(X)$ cũng vậy và do đó $X$ cũng vậy.

Q.E.D.

#### Hệ quả {#top-x-s3-n3-cor-1 .statement}

Cho $X$ là một không gian compact địa phương có tôpô nhận một cơ sở đếm được, và cho $Y$ là một không gian đều mêtric hóa được có kiểu đếm được.

a) Không gian $\mathcal{L}$ các ánh xạ liên tục của $X$ vào $Y$ có giới hạn tại vô cực, được trang bị tôpô hội tụ đều trong $X$, là một không gian mêtric hóa được có kiểu đếm được.

b) Không gian $\mathcal{C}_c(X; Y)$ các ánh xạ liên tục của $X$ vào $Y$, được trang bị tôpô hội tụ compact, là một không gian mêtric hóa được có kiểu đếm được.

a) Gọi $X'$ là không gian compact thu được bằng cách thêm vào $X$ một điểm tại vô cực (Chương I, § 9, no. 8, Định lý 4); theo định nghĩa, mọi hàm $f \in \mathcal{L}$ đều có thể được mở rộng duy nhất thành một hàm liên tục $\overline{f} : X' \to Y$, và $f \to \overline{f}$ do đó là một song ánh từ L lên $C(X'; Y)$; và song ánh này là một đồng phôi từ không gian L lên $C_u(X'; Y)$ theo Mệnh đề 6 của § 1, no. 6. Vì $X'$ mêtric hóa được (Chương IX, § 2, no. 9, Mệnh đề 16, Hệ quả), kết quả suy ra từ Định lý 1, áp dụng cho $X'$ và Y.

b) Gọi $(U_n)$ là một phủ của X bởi các tập mở tương đối compact, sao cho mọi tập con compact của X được chứa trong một $U_n$ nào đó (Chương I, § 9, no. 9, Mệnh đề 15, Hệ quả 1). Nếu $S$ là tập hợp các $\overline{U}_n$, thì tôpô hội tụ compact trên $C(X; Y)$ trùng với tôpô hội tụ theo $S$. Do đó ($§ 1,$ no. 2, Nhận xét 3) không gian $C_c(X; Y)$ đồng phôi với một không gian con của tích $\prod_n C_u(\overline{U}_n; Y)$; vì mỗi không gian compact $\overline{U}_n$ có một cơ sở đếm được, nó mêtric hóa được (Chương IX, § 2, no. 9, Mệnh đề 16); mỗi không gian $C_u(\overline{U}_n; Y)$ do đó mêtric hóa được và có kiểu đếm được theo Định lý 1, và do đó $C_c(X; Y)$ cũng vậy.

Chú ý rằng không gian của tất cả các hàm liên tục bị chặn nhận giá trị thực trên $\mathbf{R}$, được trang bị tôpô hội tụ đều, không có kiểu đếm được (Bài tập 4).

### 4. TÔPÔ COMPACT-MỞ

#### Định lý 2 {#top-x-s3-thm-2 .statement}

*Cho X là một không gian tôpô, Y là một không gian đều. Với mỗi tập con compact K của X và mỗi tập con mở U của Y, ký hiệu T(K, U) là tập hợp của tất cả các ánh xạ liên tục $u : X \to Y$ sao cho $u(K) \subset U$. Khi đó các tập hợp $T(K, U)$ sinh ra tôpô hội tụ compact trên $C(X; Y)$.*

Gọi $Y'$ là không gian đều Hausdorff liên kết với Y (Chương II, § 3, no. 8) và gọi $i : Y \to Y'$ là ánh xạ chính tắc của Y lên $Y'$. Tôpô hội tụ compact là tôpô thô nhất sao cho các ánh xạ $u \to (i \circ u)|K$ từ $C(X; Y)$ vào $C_u(K; Y')$ là liên tục, khi K chạy qua tập hợp của tất cả các tập con compact của X ($§ 1,$ no. 4, Mệnh đề 4). Do đó ta thu được một cơ sở phụ của tôpô của $C_c(X; Y)$ bằng cách lấy một cơ sở phụ của tôpô của $C_c(K; Y')$ với mỗi tập con compact K của X rồi lấy hợp [trong $\mathfrak{B}(C(X; Y))$] của các ảnh ngược của các cơ sở phụ này trong $C(X, Y)$. Mặt khác, mọi tập con mở của Y đều có dạng $\overline{i}^{-1}(U')$, trong đó $U'$ là mở trong $Y'$ (Chương II, § 3, no. 7, Mệnh đề 12); do đó, với mỗi tập con compact $K' \supset K$, $T(K, \overline{i}^{-1}(U'))$ là ảnh ngược của $T(K, U')$ theo ánh xạ

$$
C(X; Y) \to C_a(K'; Y').
$$

Vì vậy, ta chỉ còn phải chứng minh định lý khi X là *compact* và Y là *Hausdorff*; từ nay ta sẽ đặt các giả thiết này.

Trước hết hãy chứng minh rằng $T(K, U)$ là mở trong $C_c(X; Y)$. Gọi $u_0$ là một điểm của tập hợp này; vì $u_0(K)$ là compact (Chương I, § 9, no. 4, Định lý 2, Hệ quả 1) và được chứa trong tập mở $U$, nên tồn tại một lân cận đối xứng $V$ của $Y$ sao cho $V(u_0(K)) \subset U$ (Chương II, § 4, no. 3, Mệnh đề 4, Hệ quả). Gọi $W$ là lân cận của $u_0$ trong $C_c(X; Y)$ gồm tất cả các ánh xạ liên tục $u : X \to Y$ sao cho $(u(x), u_0(x)) \in V$ với mọi $x \in K$. Với các ánh xạ như vậy, rõ ràng ta có $u(K) \subset V(u_0(K)) \subset U$; do đó $u \in T(K, U)$ và vì thế $W \subset T(K, U)$, điều này chứng minh mệnh đề của ta.

Ngược lại, nếu $W$ là một lân cận của một điểm $u_0 \in C_c(X; Y)$, ta hãy chứng minh rằng $W$ chứa giao của một số hữu hạn các lân cận có dạng $T(K, U)$. Ta có thể giả sử rằng $W$ là tập hợp tất cả các $u \in C(X; Y)$ sao cho $(u(x), u_0(x)) \in V$ với mọi $x \in X$, $V$ là một lân cận đồng đều đã cho của $Y$. Vì $u_0$ liên tục trên $X$, nó liên tục đều (Chương II, § 4, no. 1, Định lý 2). Gọi $V_1$ là một lân cận đồng đều đối xứng của $Y$, mở trong $Y \times Y$ và sao cho $V_1^2 \subset V$. $X$ có thể được phủ bởi một số hữu hạn các tập compact $K_i$ ($1 \leq i \leq n$) sao cho mỗi $u_0(K_i)$ là $V_1$-nhỏ ($1 \leq i \leq n$). Gọi $U_i$ là tập mở $V_1(u_0(K_i))$, và gọi $u : X \to Y$ là một ánh xạ liên tục được chứa trong giao của $n$ tập $T(K_i, U_i)$ (là các lân cận của $u_0$). Khi đó, với mọi $x \in K_i$, $u(x)$ thuộc $U_i$ và do đó $u_0(x)$ và $u(x)$ là $V_1^2$-gần nhau, suy ra là $V$-gần nhau. Vì mỗi $x \in X$ thuộc một $K_i$ nào đó, ta có $u \in W$ và chứng minh hoàn tất.

Kết quả này dẫn đến định nghĩa sau:

#### Định nghĩa 1 {#top-x-s3-def-1 .statement}

*Cho $X, Y$ là hai không gian tôpô, không nhất thiết khả quy đồng đều. Với mỗi tập con compact $K$ của $X$ và mỗi tập con mở $U$ của $Y$, gọi $T(K, U)$ là tập hợp tất cả các $u \in C(X; Y)$ sao cho $u(K) \subset U$. Tôpô trên $C(X; Y)$ sinh bởi các tập $T(K, U)$ được gọi là tôpô hội tụ compact hoặc tôpô mở-compact; và ta ký hiệu bởi $C_c(X; Y)$ không gian tôpô thu được bằng cách trang bị cho $C(X; Y)$ tôpô này.*

Nếu $Y$ là một không gian đồng đều thì từ Định lý 2 suy ra rằng định nghĩa này trùng với định nghĩa đã cho trong § 1, no. 3.

Nếu $H$ là một tập con của $C(X; Y)$, ta sẽ nói rằng tôpô cảm sinh trên $H$ bởi tôpô của $C_c(X; Y)$ là tôpô mở-compact trên $H$.

#### Ví dụ {#top-x-s3-n4-exa-1 .statement}

Cho $I$ là khoảng $[0, 1]$ trong $\mathbf{R}$. Nếu $Y$ là một không gian tôpô bất kỳ, không gian $C_c(I; Y)$ được gọi là *không gian các đường đi* trong $Y$. Với mỗi $y \in Y$, không gian con $\Omega_y(Y)$ của $C_c(I; Y)$ gồm các đường đi $u$ sao cho $u(0) = u(1) = y$ được gọi là *không gian các vòng* (trong $Y$) *tại điểm* $y$.

#### Nhận xét 1 {#top-x-s3-n4-rem-1 .statement}

Tương tự, tôpô cảm sinh trên $C(X; Y)$ bởi tôpô tích trên $Y^X = \mathcal{F}(X; Y)$ được gọi là *tôpô hội tụ điểm* ($Y$ không nhất thiết là khả tôpô đều); nó được sinh bởi các tập hợp có dạng $T(\{x\}, U)$ khi $x$ chạy qua $X$ và $U$ chạy qua tập hợp tất cả các tập hợp mở của $Y$, và do đó nó thô hơn tôpô mở compact. Ta suy ra rằng, *nếu $Y$ là Hausdorff, không gian $C_c(X; Y)$ là Hausdorff* (Chương I, § 8, no. 1, Mệnh đề 5, Hệ quả).

#### Nhận xét 2 {#top-x-s3-n4-rem-2 .statement}

Cho $\mathcal{S}$ là một cơ sở phụ của tôpô của $Y$, và cho $\mathcal{K}$ là một tập hợp các tập con compact của $X$ có tính chất sau:

(R) Nếu $L$ là một tập con compact bất kỳ của $X$ và $V$ là một lân cận bất kỳ của $L$, thì tồn tại một số hữu hạn các tập hợp $K_i \in \mathcal{K}$ sao cho $L \subset \bigcup_i K_i \subset V$.

Khi đó các tập hợp $T(K, U)$, trong đó $K \in \mathcal{K}$ và $U \in \mathcal{S}$, tạo thành một *cơ sở phụ* cho tôpô mở compact trên $C(X; Y)$. Để chứng minh điều này, ta phải chỉ ra rằng nếu $L$ là một tập con compact bất kỳ của $X$ và $V$ là một tập con mở bất kỳ của $Y$, và nếu $u \in T(L, V)$, thì tồn tại một số hữu hạn các cặp $(K_i, U_i)$ sao cho $K_i \in \mathcal{K}$, $U_i \in \mathcal{S}$ và $u \in \bigcap_i T(K_i, U_i) \subset T(L, V)$. Trước hết hãy chú ý rằng đối với mọi dãy hữu hạn $(s_k)$ các tập hợp của $\mathcal{S}$ và mọi tập con compact $M$ của $X$, ta có $T\left(M, \bigcap_k S_k\right) = \bigcap_k T(M, S_k)$ theo định nghĩa. Vì vậy trước hết ta có thể thay thế $\mathcal{S}$ bởi tập hợp các giao hữu hạn của các tập hợp của $\mathcal{S}$, nghĩa là ta có thể giả sử rằng $\mathcal{S}$ là một *cơ sở* của tôpô của $Y$. Theo giả thiết, $u(L)$ là quasi-compact và được chứa trong $V$, do đó tồn tại một số hữu hạn các tập hợp $U_i \in \mathcal{S}$ được chứa trong $V$ phủ $u(L)$.

Các tập hợp $\overline{u}^{-1}(U_i)$ là mở trong $X$ và phủ $L$. Do đó, với mỗi $x \in L$ có một lân cận compact $N_x$ của $x$ trong $L$, được chứa trong một trong các tập $\overline{u}^{-1}(U_i)$. Ta có thể phủ $L$ bằng một số hữu hạn các tập này $N_{x_j} = L_j$; với mỗi $j$, ta ký hiệu bởi $i(j)$ một trong các chỉ số $i$ sao cho $L_j \subset \overline{u}^{-1}(U_i)$. Với điều này, với mỗi chỉ số $j$ tồn tại [theo (R)] một số hữu hạn các tập $K_{jk} \subset \overline{u}^{-1}(U_{i(j)})$, thuộc về $\mathcal{K}$, phủ $L_j$. Với mỗi $v \in \bigcap_{j,k} T(K_{jk}, U_{i(j)})$ ta có $\bigcup_k v(K_{jk}) \subset U_{i(j)}$ và do đó $v(L_j) \subset U_{i(j)}$, và $v(L) = \bigcup_j v(L_j) \subset \bigcup_j U_{i(j)} \subset V$; như vậy mệnh đề của ta được chứng minh.

#### Định lý 3 {#top-x-s3-thm-3 .statement}

*Cho $X, Y, Z$ là ba không gian tôpô và cho $f$ là một ánh xạ từ $X \times Y$ vào $Z$. Nếu $f$ liên tục thì $\tilde{f}: x \to f(x, .)$ là một ánh xạ liên tục từ $X$ vào $C_c(Y; Z)$. Mệnh đề đảo lại đúng nếu $Y$ là lân cận compact.*

Giả sử rằng $f$ là liên tục. Để chứng minh rằng $\tilde{f}$ là liên tục, ta phải chứng minh rằng, với mỗi tập con compact $K$ của $Y$ và mỗi tập con mở $U$ của $Z$, ảnh ngược $V$ của $T(K, U)$ qua $\tilde{f}$ là mở trong $X$. Cho $x_0 \in V$; với mỗi $y \in K$, ta có $f(x_0, y) \in U$, và vì $f$ là liên tục nên tồn tại một lân cận $V_y$ của $x_0$ trong $X$ và một lân cận $W_y$ của $y$ trong $Y$ sao cho $f(V_y \times W_y) \subset U$. Vì $K$ compact, tồn tại một số hữu hạn các điểm $y_i \in K$ sao cho các tập hợp $W_{y_i} (1 \leq i \leq n)$ phủ $K$. Gọi $V'$ là giao của các lân cận $V_{y_i}$ của $x_0$, là một lân cận của $x_0$; nếu $x \in V'$ và $y \in K$, ta có $f(x, y) \in U$, vì $y$ được chứa trong một trong các $W_{y_i}$ và $x$ được chứa trong mỗi $V_{y_i}$; do đó $V' \subset V$, và vì vậy $V$ là một lân cận của mỗi điểm của nó và do đó là mở trong $X$.

Ngược lại, giả sử rằng $\tilde{f}$ liên tục và $Y$ là địa phương compact, ta chứng minh rằng $f$ liên tục. Cho $x_0 \in X$, cho $y_0 \in Y$ và cho $U$ là một lân cận mở của $f(x_0, y_0)$ trong $Z$; ta sẽ chứng minh rằng tồn tại một lân cận $V$ của $x_0$ trong $X$ và một lân cận $W$ của $y_0$ trong $Y$ sao cho $f(V \times W) \subset U$. Vì $y \to f(x_0, y)$ là liên tục, tồn tại một lân cận *compact* $W$ của $y_0$ sao cho $f(\{x_0\} \times W) \subset U$. Mặt khác, vì $\tilde{f}$ liên tục, tập hợp $V$ gồm các $x \in X$ sao cho $f(x, .) \in T(W, U)$ [nghĩa là sao cho $f(x, y) \in U$ với mọi $y \in W$] là một tập con mở của $X$ và do đó là một lân cận của $x_0$; và ta có $f(V \times W) \subset U$.

Q.E.D.

#### Hệ quả 1 {#top-x-s3-thm-3-cor-1 .statement}

*Cho $X$ là một không gian địa phương compact, $Y$ một không gian tôpô, $H$ một tập con của $C(X; Y)$. Khi đó tôpô compact-mở trên $H$ là tôpô thô nhất sao cho ánh xạ $(u, x) \to u(x)$ của $H \times X$ vào $Y$ là liên tục.*

Thật vậy, theo Định lý 3, ánh xạ này liên tục khi và chỉ khi đơn ánh chính tắc $H \to C_c(X; Y)$ là liên tục.

#### Nhận xét 3 {#top-x-s3-n4-rem-3 .statement}

Cho $X$ là một không gian địa phương compact và $Y$ là một không gian tôpô Hausdorff. Nếu $\mathcal{T}$ là một tôpô trên một tập con $H$ của $C(X; Y)$ sao cho ánh xạ $(u, x) \to u(x)$ là liên tục trên $H \times X$ và nếu thêm nữa $H$ là *compact* đối với $\mathcal{T}$, thì $\mathcal{T}$ là tôpô compact-mở. Thật vậy, nó mịn hơn tôpô sau theo Hệ quả 1, và vì tôpô compact-mở là Hausdorff, hai tôpô là đồng nhất. Chú ý rằng nếu thêm vào đó $Y$ là *chính quy hoàn toàn*, thì $H$ là *đồng liên tục* đối với mọi cấu trúc đều tương thích với tôpô của $Y$ (§ 2, no. 5, Định lý 2, Hệ quả 3), và với mọi tập con compact $K$ của $X$, tập hợp

$$
H(K) = \bigcup_{x \in K} H(x)
$$

là compact, vì nó là ảnh của $H \times K$ qua ánh xạ liên tục $(u, x) \to u(x)$.

#### Hệ quả 2 {#top-x-s3-thm-3-cor-2 .statement}

*Cho $X, Y, Z$ là ba không gian tôpô sao cho $X$ là Hausdorff và $Y$ là compact địa phương. Khi đó hạn chế vào $C(X \times Y; Z)$ của song ánh chính tắc $\mathcal{F}(X \times Y; Z) \to \mathcal{F}(X; \mathcal{F}(Y; Z))$ (Lý thuyết tập hợp, R, § 4, no. 14) là một đồng phôi từ $C_c(X \times Y; Z)$ lên $C_c(X; C_c(Y; Z))$.*

Hạn chế này hiển nhiên là một song ánh

$$
\rho : \mathcal{C}(X \times Y; Z) \to \mathcal{C}(X; \mathcal{C}_c(Y; Z))
$$

bởi Định lý 3; do đó còn phải chỉ ra rằng tôpô compact-mở trên $\mathcal{C}(X \times Y; Z)$ là ảnh ngược theo $\rho$ của tôpô compact-mở trên $\mathcal{C}(X; \mathcal{C}_c(Y; Z))$. Vì các tập hợp $T(K, U)$, trong đó $K$ là một tập con compact của $Y$ và $U$ là một tập con mở của $Z$, tạo thành một tiền cơ sở của tôpô của $\mathcal{C}_c(Y; Z)$, nên từ Nhận xét 2 suy ra rằng tôpô của $\mathcal{C}_c(X; \mathcal{C}_c(Y; Z))$ được sinh bởi các tập hợp có dạng $T(J, T(K, U))$, trong đó $K$ và $U$ như trên và $J$ là một tập con compact của $X$. Bây giờ ảnh của $T(J, T(K, U))$ theo $\rho$ chính xác là $T(J \times K, U)$, và do đó là một tập mở; vậy ta đã chứng minh rằng $\rho$ liên tục. Để chứng minh rằng $\rho$ là một phép đồng phôi, trước hết ta chú ý rằng các tập hợp có dạng $J \times K$ trong $X \times Y$ (trong đó $J$ là một tập con compact của $X$, và $K$ là một tập con compact của $Y$) thỏa mãn điều kiện (R) của Nhận xét 2: vì nếu $L$ là một tập con compact của $X \times Y$ và $V$ là một lân cận của $L$ trong $X \times Y$, thì các phép chiếu $M = \operatorname{pr}_1(L)$, $N = \operatorname{pr}_2(L)$ là compact, vì $X$ và $Y$ là Hausdorff và $V \cap (M \times N)$ là một lân cận của $L$ trong không gian compact $M \times N$, do đó mọi điểm của $L$ có một lân cận trong $M \times N$ có dạng $J \times K \subset V$, trong đó $J \subset M$ và $K \subset N$ là compact; vì $L$ có thể được phủ bởi một số hữu hạn các lân cận này, nên mệnh đề được chứng minh. Do đó các tập hợp có dạng $T(J \times K; U)$, trong đó $J$ là một tập con compact của $X$, $K$ là một tập con compact của $Y$ và $U$ là một tập con mở của $Z$, sinh tôpô của $\mathcal{C}_c(X \times Y; Z)$. Nhưng ta đã thấy rằng ảnh của $T(J \times K, U)$ theo $\rho$ là tập mở $T(J, T(K, U))$ trong $\mathcal{C}_c(X; \mathcal{C}_c(Y; Z))$; do đó $\rho$ là một phép đồng phôi.

Chú ý rằng nếu ngoài ra $Z$ được giả thiết là khả năng đồng nhất hóa, thì Hệ quả 2 là một hệ quả tầm thường của § 1, no. 4, Mệnh đề 2.

#### Mệnh đề 9 {#top-x-s3-prop-9 .statement}

*Cho $X, Y, Z$ là ba không gian tôpô, $Y$ là địa phương compact. Khi đó ánh xạ $(u, v) \to v \circ u$ của $\mathcal{C}_c(X; Y) \times \mathcal{C}_c(Y; Z)$ vào $\mathcal{C}_c(X; Z)$ là liên tục.*

Ta phải chỉ ra rằng, với mọi tập con compact $K$ của $X$ và mọi tập con mở $U$ của $Z$, tập hợp $R$ gồm các cặp $(u, v)$ sao cho $v(u(K)) \subset U$ là mở trong $\mathcal{C}_c(X; Y) \times \mathcal{C}_c(Y; Z)$. Cho $(u_0, v_0) \in R$; khi đó $u_0(K)$ là một tập con compact của không gian địa phương compact $Y$, được chứa trong tập mở $\overline{v_0^{-1}}(U)$, và do đó tồn tại một lân cận compact $L$ của $u_0(K)$ được chứa trong $\overline{v_0^{-1}}(U)$ (Chương I, § 9, no. 7, Mệnh đề 10). Tập hợp $V$ gồm mọi $u \in \mathcal{C}_c(X; Y)$ sao cho $u(K) \subset L$ là một lân cận của $u_0$, và tập hợp $W$ gồm mọi $v \in \mathcal{C}_c(Y; Z)$ sao cho $v(L) \subset U$ là một lân cận của $v_0$; hơn nữa, quan hệ $(u, v) \in V \times W$ kéo theo $v(u(K)) \subset U$. Vậy kết quả được chứng minh.

### 5. CÁC TÔPÔ TRÊN CÁC NHÓM CỦA CÁC PHÉP ĐỒNG PHÔI

#### Mệnh đề 10 {#top-x-s3-prop-10 .statement}

Cho $X$ là một không gian đều và cho $H$ là một tập hợp đồng liên tục của các phép đồng phôi từ $X$ lên chính nó. Nếu $H$ và $H^{-1}$ được trang bị tôpô của sự hội tụ điểm trong $X$, thì ánh xạ $u \to u^{-1}$ của $H^{-1}$ lên $H$ là liên tục.

Chỉ cần chỉ ra rằng, với mỗi $x_0 \in X$, ánh xạ $u \to u^{-1}(x_0)$ của $H^{-1}$ vào $X$ là liên tục tại mọi điểm $u_0 \in H^{-1}$. Cho $V$ là một quan hệ lân cận đối xứng của $X$, và cho $y_0 = u_0^{-1}(x_0)$. Theo giả thiết, tồn tại một quan hệ lân cận đối xứng $U$ của $X$ sao cho quan hệ $(x, x_0) \in U$ kéo theo $(u^{-1}(x), u^{-1}(x_0)) \in V$ với mọi $u \in H^{-1}$. Lấy một phần tử $u \in H^{-1}$ là $W(\{y_0\}, U)$-gần với $u_0$; khi đó ta có $(u(y_0), u_0(y_0)) \in U$, tức là $(u(y_0), x_0) \in U$. Suy ra $(y_0, u^{-1}(x_0)) \in V$, tức là $(u_0^{-1}(x_0), u^{-1}(x_0)) \in V$; điều này hoàn thành chứng minh.

#### Hệ quả {#top-x-s3-n5-cor-1 .statement}

Cho $X$ là một không gian đều và cho $H$ là một nhóm các tự đồng phôi liên tục đều của $X$ lên chính nó. Khi đó tôpô hội tụ điểm trong $X$ là tương thích với cấu trúc nhóm của $H$.

Đây là một hệ quả của Mệnh đề 10, cùng với § 2, no. 1, Mệnh đề 1, Hệ quả 5.

#### Mệnh đề 11 {#top-x-s3-prop-11 .statement}

Cho $X$ là một không gian compact và cho $\Gamma$ là nhóm gồm tất cả các tự đồng phôi của $X$ lên chính nó. Khi đó tôpô hội tụ đều trong $X$ là tương thích với cấu trúc nhóm của $\Gamma$.

Ta đã biết (no. 4, Mệnh đề 9) rằng ánh xạ $(u, v) \to v \circ u$ của $\Gamma \times \Gamma$ vào $\Gamma$ là liên tục đối với tôpô này; do đó ta phải chứng minh rằng $u \to u^{-1}$ là liên tục tại mọi điểm $u_0$ của $\Gamma$. Vì $u_0^{-1}$ là liên tục đều trên $X$, với mọi lân cận đối xứng $V$ của $X$ tồn tại một lân cận $W$ của $X$ sao cho quan hệ $(x, x') \in W$ kéo theo $(u_0^{-1}(x), u_0^{-1}(x')) \in V$. Vì vậy, nếu $u \in \Gamma$ sao cho $(u_0(x), u(x)) \in W$ với mọi $x \in X$, thì suy ra rằng $(x, u_0^{-1}(u(x))) \in V$ với mọi $x \in X$, và do đó (vì $u$ là song ánh) $(u^{-1}(x), u_0^{-1}(x)) \in V$ với mọi $x \in X$. Điều này hoàn tất chứng minh.

Bây giờ cho $X$ là một không gian compact địa phương và cho $\Gamma$ là nhóm gồm tất cả các đồng phôi của $X$ lên chính nó. Tôpô của sự hội tụ compact trong $X$ không nhất thiết tương thích với cấu trúc nhóm của $\Gamma$ (Bài tập 17). Gọi $X'$ là không gian compact thu được bằng cách ghép thêm một điểm ở vô cực $\omega$ vào $X$. Mọi đồng phôi $u$ của $X$ lên chính nó mở rộng duy nhất thành một đồng phôi $u'$ của $X'$ lên chính nó sao cho $u'(\omega) = \omega$ (Chương I, § 10, no. 3, Hệ quả của Mệnh đề 7), do đó $\Gamma$ có thể được đồng nhất với nhóm con của nhóm $\Gamma'$ gồm tất cả các đồng phôi của $X'$ lên chính nó, gồm tất cả các đồng phôi giữ cố định $\omega$. Tôpô cảm sinh trên $\Gamma$ bởi tôpô của $C_u(X'; X')$ vì thế tương thích với cấu trúc nhóm của $\Gamma'$ (Mệnh đề 11), và $\Gamma$ là đóng trong $\Gamma'$ [đối với tôpô cảm sinh bởi tôpô của $C_u(X'; X')$] vì nó được xác định bởi phương trình $u(\omega) = \omega$ (§ 1, no. 2, Nhận xét 6). Ta ký hiệu bởi $\mathcal{T}_\beta$ tôpô nhóm được xác định như vậy trên $\Gamma$; nó mịn hơn tôpô của sự hội tụ compact và cũng có thể (nhờ § 1, no. 6, Mệnh đề 6) được định nghĩa là tôpô của sự hội tụ đều trên $X$, khi $X$ được trang bị cấu trúc đều cảm sinh bởi cấu trúc đều duy nhất của $X'$.

Tôpô $\mathcal{T}_\beta$ có thể được đặc trưng như sau:

#### Mệnh đề 12 {#top-x-s3-prop-12 .statement}

*Trên nhóm $\Gamma$ gồm tất cả các đồng phôi của một không gian compact địa phương $X$, tôpô $\mathcal{T}_\beta$ là tôpô thô nhất sao cho các ánh xạ $u \to u$ và $u \to u^{-1}$ từ $\Gamma$ vào $C_c(X; X)$ là liên tục.*

Ta tạm thời ký hiệu tôpô sau bởi $\mathcal{C}'$. Vì $u \to u^{-1}$ là liên tục đối với $\mathcal{T}_\beta$ và vì $\mathcal{T}_\beta$ mịn hơn tôpô của sự hội tụ compact, rõ ràng rằng $\mathcal{T}_\beta$ mịn hơn $\mathcal{C}'$. Để chứng minh đảo lại, trang bị cho $X'$ cấu trúc đều duy nhất của nó; cho $u_0 \in \Gamma$ và cho $V$ là một lân cận đều của $X'$; khi đó ta phải chứng minh rằng tồn tại một tập con compact $K$ của $X$ và một lân cận đều đối xứng $W$ của $X'$ sao cho các quan hệ

$$
u \in \Gamma, \ (u_0(x), u(x)) \in W \text{ và } (u_0^{-1}(x), u^{-1}(x)) \in W \text{ với mọi } x \in K
$$

kéo theo

$$
(u_0(x), u(x)) \in V \text{ với mọi } x \in X.
$$

Cho $V_1$ là một lân cận đối xứng mở của $X'$ sao cho $\overset{2}{V}_1 \subset V$; khi đó $K_1 = X' - V_1(\omega)$ là một tập con compact của $X$. Chọn một lân cận đối xứng mở $W$ của $X'$ sao cho $W \subset V$ và $W(\omega) \cap W(u_0^{-1}(K_1)) = \emptyset$; điều này có thể thực hiện được theo Mệnh đề 4 của Chương II, § 4, no. 3. Đặt $K_2 = X' - W(\omega)$, là một tập con compact của $X$. Ta sẽ thấy rằng $W$ và tập compact $K = K_1 \cup K_2$ thực hiện điều cần thiết. Vì $W \subset V$, chỉ cần chứng minh rằng quan hệ

$$
(u_0^{-1}(x), u^{-1}(x)) \in W \text{ với mọi } x \in K_1 \quad (u \in \Gamma)
$$

suy ra rằng

$$
(u(y), \omega) \in V_1 \text{ với mọi } y \in W(\omega);
$$

vì khi đó ta cũng có $(u_0(y), \omega) \in V_1$ và do đó

$$
(u_0(y), u(y)) \in \overset{2}{V}_1 \subset V
$$

với mọi $y \in W(\omega) = X' - K_2$. Bây giờ nếu ta có $y \in W(\omega)$ và

$$
u(y) \in X' - V_1(\omega) = K_1,
$$

thì suy ra $y \in u^{-1}(K_1) \subset W(u_0^{-1}(K_1))$, trái với sự lựa chọn của $W$; chứng minh do đó hoàn tất.

Nói chung nhóm $\Gamma$, được trang bị $\mathcal{T}_\beta$, không là compact địa phương; nhưng ta có tiêu chuẩn sau:

#### Định lý 4 {#top-x-s3-thm-4 .statement}

*Cho $G$ là một nhóm con của nhóm $\Gamma$ gồm tất cả các đồng phôi của một không gian compact địa phương $X$. Giả sử rằng, trong không gian $C_c(X; X)$, có một lân cận $V$ của ánh xạ đồng nhất $e$ sao cho $V \cap G = H$ là đối xứng trong $G$ và tương đối compact trong $C_c(X; X)$. Khi đó bao đóng $\overline{G}$ của $G$ trong $\Gamma$ đối với tôpô $\mathcal{T}_\beta$ là một nhóm compact địa phương đối với tôpô cảm sinh bởi $\mathcal{T}_\beta$; tôpô cảm sinh này trên $\overline{G}$ trùng với tôpô hội tụ compact, và bao đóng $\overline{H}$ của $H$ trong $C_c(X; X)$ là một lân cận của $e$ trong $\overline{G}$ đối với tôpô này.*

Trước hết ta chứng minh rằng $\overline{H}$ được chứa trong $\Gamma$ và rằng tôpô cảm sinh trên $\overline{H}$ bởi $\mathcal{T}_\beta$ là *giống với tôpô của sự hội tụ compact*. Cho $u_0 \in \overline{H}$; do đó $u_0$ là giới hạn, trong $C_c(X; X)$, của một siêu lọc $\Phi$ trên $H$. Vì $\Phi^{-1}$ (ảnh của $\Phi$ qua $u \to u^{-1}$) là một cơ sở siêu lọc trên $H \subset \overline{H}$, nó hội tụ trong không gian con compact $\overline{H}$ của $C_c(X; X)$ tới một phần tử $v_0$. Ánh xạ $(u, v) \to uv$ hội tụ tới $u_0 v_0$ đối với $\Phi \times \Phi^{-1}$ (no. 4, Mệnh đề 9); *a fortiori*, $u \to uu^{-1} = e$ hội tụ tới $u_0 v_0$ đối với $\Phi$, do đó $u_0 v_0 = e$ vì $C_c(X; X)$ là Hausdorff. Tương tự $v_0 u_0 = e$; do đó $u_0$ là một đồng phôi của $X$, nghĩa là, $u_0 \in \Gamma$. Vậy $\overline{H}$ được chứa trong $\Gamma$. Hơn nữa, lập luận này chỉ ra rằng $\overline{H}^{-1} = \overline{H}$ và rằng, với mọi siêu lọc $\Phi$ trên $\overline{H}$ hội tụ tới $u_0$, $\Phi^{-1}$ hội tụ trong $C_c(X; X)$ tới $u_0^{-1}$; do đó ánh xạ $u \to u^{-1}$ từ $\overline{H}$ vào $C_c(X; X)$ là liên tục khi $\overline{H}$ mang tôpô của sự hội tụ compact (Chương I, § 7, no. 4, Mệnh đề 9, Hệ quả 1). Mệnh đề 12 khi đó chỉ ra rằng, trên $\overline{H}$, tôpô của sự hội tụ compact là giống với tôpô cảm sinh bởi $\mathcal{T}_\beta$.

Hơn nữa, vì tôpô $\mathcal{T}_\beta$ trên $\Gamma$ mịn hơn tôpô hội tụ compact, $\overline{H}$ cũng là bao đóng của $H$ đối với $\mathcal{T}_\beta$. Nhưng $H$ là một lân cận của $e$ trong $G$ đối với tôpô hội tụ compact, và *a fortiori* đối với tôpô cảm sinh bởi $\mathcal{T}_\beta$; suy ra (Chương I, § 3, no. 1, Mệnh đề 2) rằng $\overline{H}$ là một lân cận của $e$ trong $\overline{G}$ đối với tôpô cảm sinh bởi $\mathcal{T}_\beta$, và do đó $\overline{G}$ là địa phương compact trong tôpô này. Nếu $W$ là phần trong của $V$ đối với tôpô hội tụ compact, thì $W \cap \Gamma$ là mở trong $\mathcal{T}_\beta$, do đó $W \cap \overline{G}$ được chứa trong bao đóng của $H = V \cap G$ đối với $\mathcal{T}_\beta$ (Chương I, § 1, no. 6, Mệnh đề 5); điều này chứng tỏ rằng $\overline{H}$ cũng là một lân cận của $e$ trong $\overline{G}$ đối với tôpô hội tụ compact. Cuối cùng, với mỗi $u_0 \in \Gamma$, các song ánh $v \to u_0 \circ v$ và $v \to u_0^{-1} \circ v$ của $C_c(X; X)$ lên chính nó là liên tục (no. 4, Mệnh đề 9), và do đó, nếu $u_0 \in \overline{G}$, $u_0 \overline{H}$ là một lân cận của $u_0$ trong $\overline{G}$ đối với tôpô hội tụ compact. Điều này hoàn tất chứng minh.

#### Hệ quả {#top-x-s3-n5-cor-2 .statement}

*Cho $G$ là một nhóm các tự đồng phôi của một không gian địa phương compact $X$. Nếu bao đóng $\overline{G}$ của $G$ trong $C_c(X; X)$ là compact, thì $\overline{G}$ là một nhóm các tự đồng phôi của $X$, và tôpô hội tụ compact là tương thích với cấu trúc nhóm của $\overline{G}$, do đó nó là một nhóm tôpô compact.*

Một nhóm các tự đồng phôi của một không gian địa phương compact $X$ địa phương compact nhưng không compact đối với tôpô hội tụ compact là *đóng địa phương* trong $C_c(X; X)$ theo Chương I, § 9, no. 7, Mệnh đề 12, *nhưng không nhất thiết đóng*.

Ví dụ, trong vành $\mathcal{L}(\mathbf{R}^n)$ của các tự đồng cấu của $\mathbf{R}^n$, được đồng nhất với vành $M_n(\mathbf{R})$ của các ma trận $n \times n$ bình phương trên $\mathbf{R}$ và được trang bị tôpô hội tụ compact, nhóm $GL(n, \mathbf{R})$, được đồng nhất với nhóm các ma trận không suy biến, là địa phương compact nhưng trù mật (Chương VI, § 1, no. 6, Mệnh đề 6).

### Bài tập {#top-x-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
