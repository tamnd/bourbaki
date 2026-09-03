---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 6
section_title: The Hausdorff series
lang: vi
source: lie-i-iii
book_pages: 155-164, 201-204
pdf_pages: 0173-0182, 0219-0222
extraction: ocr
subsections:
    - "no": 1
      title: EXPONENTIAL AND LOGARITHM IN FILTERED ALGEBRAS
      page: 155
      pdf_page: 173
    - "no": 2
      title: HAUSDORFF GROUP
      page: 157
      pdf_page: 175
    - "no": 3
      title: LIE FORMAL POWER SERIES
      page: 158
      pdf_page: 176
    - "no": 4
      title: THE HAUSDORFF SERIES
      page: 160
      pdf_page: 178
    - "no": 5
      title: SUBSTITUTIONS IN THE HAUSDORFF SERIES
      page: 161
      pdf_page: 179
statements: 14
exercises: 3
content_sha256: 3d18de902feba9dfe197eea55458a137cc67e3f70efdc760adef94d0bba33569
translated_from: content/en/lie/II/06_s6_the_hausdorff_series.md
source_content_sha256: 0784af06abccc4ac51e2a4bf54599a3d414a0162e422d6ea3345f1958570374c
translation_model: gpt-5.4
translation_run: translate-vi-55539167
glossary_version: 34
glossary_terms_sha256: 8ce4abfbc4bd7239603a90305a7ef86677113f05052521632d47b9459931fb22
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. CHUỖI HAUSDORFF

*Trong đoạn này ta giả sử rằng $K$ là một trường có đặc số $0$.*

### 1. HÀM MŨ VÀ LOGARIT TRONG CÁC ĐẠI SỐ ĐƯỢC LỌC

Cho $A$ là một đại số kết hợp có đơn vị, Hausdorff và đầy đủ đối với một bộ lọc thực $(A_\alpha)$. Ta viết $m = A_0^+ = \bigcup_{\alpha > 0} A_\alpha$.

Với $x \in m$, họ $(x^n/n!)_{n \in \mathbf{N}}$ là khả tổng. Ta viết

$$
e^x = \exp x = \sum_{n \geqslant 0} x^n/n!.
$$

Khi đó $\exp(x) \in 1 + m$ và ánh xạ $\exp : m \to 1 + m$ được gọi là *ánh xạ mũ* của $A$.

Với mọi $y \in 1 + m$, họ $((-1)^{n-1}(y-1)^n/n)_{n \geqslant 1}$ là khả tổng. Ta viết

$$
\log y = \sum_{n \geqslant 1} (-1)^{n-1}(y-1)^n/n.
$$

Khi đó $\log y \in m$ và ánh xạ $\log : 1 + m \to m$ được gọi là *ánh xạ logarit* của $A$.

#### Mệnh đề 1 {#lie-ii-s6-prop-1 .statement}

*Ánh xạ mũ là một đồng phôi từ $m$ lên $1 + m$ và ánh xạ logarit là đồng phôi nghịch đảo.*

Với $x \in A_\alpha$, $\frac{x^n}{n!} \in A_{n\alpha}$. Suy ra chuỗi xác định hàm mũ hội tụ đều trên mỗi tập $A_\alpha$ với $\alpha > 0$; vì $A_\alpha$ là mở trong $m$ và $m = \bigcup_{\alpha > 0} A_\alpha$, ánh xạ mũ là liên tục. Tương tự, có thể chứng minh rằng ánh xạ logarit là liên tục.

Gọi $e$ và $l$ là các chuỗi lũy thừa hình thức không có số hạng hằng

$$
e(X) = \sum_{n \geq 1} \frac{X^n}{n!}, \quad l(X) = \sum_{n \geq 1} (-1)^{n-1} X^n / n.
$$

Ta biết (*Algebra*, Chương IV, § 6, no. 9) rằng $e(l(X)) = l(e(X)) = X$ trên $\hat{A}(\{X\}) = K[[X]]$. Bởi phép thế (§ 5, no. 1), ta suy ra rằng

$$
e(l(x)) = l(e(x)) = x
$$

với $x \in m$; vì

$$
\exp x = e(x) + 1, \quad \log(1 + x) = l(x)
$$

nên ngay lập tức suy ra

$$
\log \exp x = x, \quad \exp \log(1 + x) = 1 + x
$$

với $x$ trong $m$, do đó có mệnh đề.

#### Nhận xét {#lie-ii-s6-n1-rem-1 .statement}

(1) Nếu $x \in m, y \in m$ và $x$ và $y$ giao hoán với nhau, thì

$$
\exp(x + y) = \exp(x) \exp(y),
$$

vì họ $\left( \frac{x^i}{i!} \cdot \frac{y^j}{j!} \right)_{i,j \in \mathbf{N}}$ là khả tổng (x. *Algebra*, Chương IV, § 6, no. 9, Mệnh đề 11).

(2) Vì các chuỗi $e$ và $l$ không có số hạng hằng và $A_\alpha$ là một iđêan đóng của $A$, nên $\exp A_\alpha \subset 1 + A_\alpha$ và $\log(1 + A_\alpha) \subset A_\alpha$ do đó $\exp A_\alpha = 1 + A_\alpha$ và $\log(1 + A_\alpha) = A_\alpha$ với $\alpha > 0$.

(3) Cho $B$ là một đại số kết hợp có đơn vị, được lọc, đầy đủ và Hausdorff và $n = \bigcup_{\alpha > 0} B_\alpha$. Gọi $f$ là một đồng cấu có đơn vị liên tục từ $A$ vào $B$ sao cho $f(m) \subset n$. Khi đó $f(\exp x) = \exp f(x)$ với $x \in m$ và $f(\log y) = \log f(y)$ với $y \in 1 + m$; chẳng hạn, ta chứng minh công thức thứ nhất trong các công thức này:

$$
f(\exp x) = \sum_{n \geq 0} f(x^n)/n! = \sum_{n \geq 0} f(x)^n/n! = \exp f(x).
$$

(4) Cho E là một đại số kết hợp có đơn vị. Nếu a là một phần tử lũy linh của E, thì họ $\left( \frac{a^n}{n!} \right)_{n \in \mathbf{N}}$ có giá hữu hạn và ta viết $\exp a = \sum_{n \geq 0} a^n / n!$. Một phần tử b được gọi là unipotent nếu $b - 1$ là lũy linh; khi đó ta viết

$$
\log b = \sum_{n \geq 1} (-1)^{n-1} (b - 1)^n / n.
$$

Ta suy ra từ các quan hệ $e(l(X)) = l(e(X)) = X$ rằng ánh xạ $a \mapsto \exp a$ là một song ánh từ tập hợp các phần tử lũy linh của E lên tập hợp các phần tử unipotent của E và ánh xạ $b \mapsto \log b$ là ánh xạ nghịch đảo.

### 2. NHÓM HAUSDORFF

Cho X là một tập hợp. Ta dùng ký hiệu của § 5, no. 1 và 2. Đại số Lie tự do L(X) được đồng nhất với ảnh chính tắc của nó trong A(X) (§ 3, no. 1, Định lý 1). Ta ký hiệu bởi $\hat{L}(X)$ bao đóng của L(X) trong $\hat{A}(X)$, tức là tập hợp các phần tử của $\hat{A}(X)$ có dạng $a = \sum_{n \geq 1} a_n$ sao cho $a_n \in L^n(X)$ với mọi $n \geq 0$; đó là một đại số Lie con được lọc của $\hat{A}(X)$.

#### Định lý 1 {#lie-ii-s6-thm-1 .statement}

*Hạn chế của ánh xạ mũ của $\hat{A}(X)$ lên $\hat{L}(X)$ là một song ánh từ $\hat{L}(X)$ lên một nhóm con đóng của nhóm Magnus $\Gamma(X)$.*

Ta viết $A(X) = A, A^n(X) = A^n, \hat{A}(X) = \hat{A}, L^n(X) = L^n, \hat{L}(X) = \hat{L}, \Gamma(X) = \Gamma$. Cho B là đại số $A \otimes A$ với phân bậc kiểu $\mathbf{N}$ được định nghĩa bởi $B^n = \sum_{i+j=n} A^i \otimes A^j$. Cho $\hat{B} = \prod_{n \geq 0} B^n$ là đại số được lọc đầy đủ liên kết (*Đại số giao hoán*, Chương III, § 2, no. 12, *Ví dụ* 1). Đồng tích $c : A \to A \otimes A$ được định nghĩa trong § 3, no. 1, Hệ quả 1 của Định lý 1 là phân bậc bậc 0 và do đó kéo dài bởi tính liên tục thành một đồng cấu $\hat{c} : \hat{A} \to \hat{B}$ cho bởi

$$
\hat{c}\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} c(a_n) \quad \text{với } a_n \in A^n.
$$

Ta cũng định nghĩa các đồng cấu liên tục $\delta'$ và $\delta''$ từ $\hat{A}$ vào $\hat{B}$ bởi

$$
\delta'\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (a_n \otimes 1), \qquad \delta''\left( \sum_{n \geq 0} a_n \right) = \sum_{n \geq 0} (1 \otimes a_n) \quad \text{với } a_n \in A^n.
$$

Theo Hệ quả 2 của Định lý 1 ở § 3, số 1, $L^n$ là tập hợp các $a_n \in A^n$ sao cho $c(a_n) = a_n \otimes 1 + 1 \otimes a_n$. Suy ra $\hat{L}$ là tập hợp các $a \in \hat{A}$ sao cho

$$
\hat{c}(a) = \delta'(a) + \delta''(a).
$$

Cho $\Delta$ là tập hợp các $b \in \hat{A}$ có số hạng hằng bằng 1 và thỏa mãn quan hệ

$$
\hat{c}(b) = \delta'(b) \cdot \delta''(b),
$$

nói cách khác, tập hợp các $b = \sum_{n \geq 0} b_n$ sao cho $b_n \in \mathbf{A}^n$ với mọi $n \geq 0$, $b_0 = 1$ và $c(b_n) = \sum_{i+j=n} b_i \otimes b_j$ với $n \geq 0$. Đặc trưng hóa sau cùng cho thấy rằng $\Delta$ là một tập con đóng của $\Gamma$; vì $\hat{\epsilon}$, $\delta'$ và $\delta''$ là các đồng cấu vành và mọi phần tử của $\delta'(\hat{\mathbf{A}})$ đều giao hoán với mọi phần tử của $\delta''(\hat{\mathbf{A}})$, các hạn chế lên $\Gamma$ của các ánh xạ $c$ và $\delta'\delta''$ là các đồng cấu nhóm và $\Delta$ là một nhóm con của $\Gamma$.

Theo Mệnh đề 1 của no. 1, ánh xạ mũ của $\hat{\mathbf{A}}$ là một song ánh từ tập hợp $\hat{\mathbf{A}}^+$ các phần tử của $\hat{\mathbf{A}}$ không có số hạng hằng lên $\Gamma$. Cho $a \in \hat{\mathbf{A}}^+$ và $b = \exp a$. Vì $\hat{\epsilon}$ là một đồng cấu vành liên tục,

$$
\hat{\epsilon}(b) = \hat{\epsilon}\left( \sum_{n \geq 0} a^n/n! \right) = \sum_{n \geq 0} \hat{\epsilon}(a)^n/n! = \exp \hat{\epsilon}(a).
$$

Các hệ thức

$$
\delta'(b) = \exp \delta'(a), \quad \delta''(b) = \exp \delta''(a)
$$

được chứng minh tương tự và, vì $\delta'(a)$ giao hoán với $\delta''(a)$ (no. 1, Nhận xét 1),

$$
\delta'(b) \delta''(b) = \exp (\delta'(a) + \delta''(a)).
$$

Do đó $a$ thỏa mãn (3) khi và chỉ khi $b$ thỏa mãn (4), điều này chứng minh định lý.

#### Nhận xét {#lie-ii-s6-n2-rem-1 .statement}

Chứng minh trên cho thấy $\exp(\hat{\mathbf{L}})$ là nhóm con $\Delta$ của $\Gamma$ gồm các $b$ thỏa mãn (4).

Do đó luật nhóm của $\Delta$ có thể được chuyển sang $\hat{\mathbf{L}}$ bởi ánh xạ mũ. Nói cách khác, $\hat{\mathbf{L}}$ là một nhóm tôpô đầy đủ với luật hợp thành $(a, b) \mapsto a \mathbin{\mathbf{h}} b$ cho bởi

$$
a \mathbin{\mathbf{h}} b = \log(\exp a \cdot \exp b).
$$

Nhóm tôpô thu được như vậy được gọi là *nhóm Hausdorff* (dẫn xuất từ X đối với K).

Cho $g$ là đồng cấu từ nhóm tự do $F = F(X)$ vào $\Gamma$ sao cho $g(x) = \exp x$ với $x \in X$. Vì $\exp x - 1 - x = \sum_{n \geq 2} x^n/n!$ có cấp $\geq 2$, $g$ là đơn ánh theo Định lý 1 của § 5, no. 3. Do đó *ánh xạ $\log \circ g$ là một đơn cấu từ $F$ vào nhóm Hausdorff, mở rộng đơn ánh chính tắc $X \to \hat{\mathbf{L}}$*.

Với mọi số nguyên $m \geq 1$ ta ký hiệu bởi $\hat{\mathbf{L}}_m$ tập hợp các phần tử có cấp $\geq m$ trong $\hat{\mathbf{L}}$ và bởi $\Gamma_m$ tập hợp các $u \in \Gamma$ sao cho $u - 1$ có cấp $\geq m$. Khi đó $\hat{\mathbf{L}}_m = \exp(\Gamma_m)$ theo Nhận xét 2 của no. 1; vì $(\Gamma_m)_{m \geq 1}$ là một lọc trung tâm nguyên trên $\Gamma$ (§ 4, no. 5 mệnh đề 2), nên $(\hat{\mathbf{L}}_m)_{m \geq 1}$ *là một lọc trung tâm nguyên trên nhóm $\hat{\mathbf{L}}$*.

### 3. CHUỖI LŨY THỪA HÌNH THỨC LIE

#### Bổ đề 1 {#lie-ii-s6-lem-1 .statement}

*Cho $\mathfrak{g}$ là một đại số Lie được lọc (§ 4, no. 1), $(\mathfrak{g}_\alpha)_{\alpha \in \mathbf{R}}$ là lọc của nó và cho $\alpha \in \mathbf{R}$. Cho P là một đa thức Lie thuần nhất bậc n theo các bất định $(\Gamma_i)_{i \in I}$ (§ 2, no. 4). Khi đó $P((a_i)) \in \mathfrak{g}_{n\alpha}$ với mọi họ $(a_i)_{i \in I}$ các phần tử của $\mathfrak{g}_\alpha$*.

Mọi đa thức Lie bậc $n \geqslant 2$ đều là một tổng hữu hạn các hạng tử dạng $[Q, R]$ trong đó $Q$ và $R$ có bậc $< n$ và tổng các bậc của chúng bằng $n$ (§ 2, no. 7, mệnh đề 7). Bổ đề được suy ra bằng quy nạp theo $n$.

Một *chuỗi lũy thừa hình thức Lie*† (với các hệ số trong $K$) *theo các bất định* $(T_i)_{i \in I}$ là bất kỳ phần tử nào của đại số Lie $\hat{L}((T_i)_{i \in I}) = \hat{L}(I)$. Một phần tử như vậy $u$ có thể được viết duy nhất thành tổng của một họ khả tổng $(u_\nu)_{\nu \in \mathbf{N}^{(I)}}$ trong đó $u_\nu \in L^\nu(I)$.

Giả sử rằng $I$ là *hữu hạn*. Cho $g$ là một đại số Lie lọc Hausdorff đầy đủ sao cho $g = \bigcup_{\alpha > 0} g_\alpha$; cho $t = (t_i)_{i \in I}$ là một họ các phần tử của $g$.

#### Mệnh đề 2 {#lie-ii-s6-prop-2 .statement}

*Đồng cấu* $f_t : L(I) \to g$ *sao cho* $f_t(T_i) = t_i$ (§ 2, no. 4) *có thể được mở rộng bằng tính liên tục thành một và chỉ một đồng cấu liên tục* $\hat{f}_t$ *từ* $\hat{L}(I)$ *vào* $g$.

Tồn tại $\alpha > 0$ sao cho $t_i \in g_\alpha$ với mọi $i \in I$; do đó $f_t(L^\nu(I)) \subset g_{|\nu| \wedge \alpha}$ với mọi $\nu$ (Bổ đề 1), điều này suy ra tính liên tục của $\hat{f}_t$.

Nếu $u \in \hat{L}(I)$, ta viết $u((t_i)) = \hat{f}_t(u)$. Đặc biệt, khi lấy $g = \hat{L}(I)$, thì $u = u((T_i))$; trong trường hợp tổng quát, $u((t_i))$ được gọi là kết quả của phép thế các $t_i$ cho các $T_i$ trong chuỗi lũy thừa hình thức Lie $u((T_i))$. Nếu $u = \sum_{\nu \in \mathbf{N}^{(I)}} u_\nu$, trong đó $u_\nu \in L^\nu(X)$, thì họ $(u_\nu((t_i)))_{\nu \in \mathbf{N}^{(I)}}$ là khả tổng và
$$
u((t_i)) = \sum_{\nu \in \mathbf{N}^{I}} u_\nu((t_i)).
$$

Cho $\sigma$ là một đồng cấu liên tục từ $g$ vào một đại số Lie lọc Hausdorff đầy đủ $g'$ sao cho $g' = \bigcup_{\alpha > 0} g'_\alpha$. Với mọi họ *hữu hạn* $t = (t_i)_{i \in I}$ các phần tử của $g$ và mọi $u \in \hat{L}(I)$,
$$
\sigma(u((t_i))) = u((\sigma(t_i))),
$$
vì đồng cấu $\sigma \circ \hat{f}_t$ là liên tục và biến $T_i$ thành $\sigma(t_i)$ với $i \in I$.

Cho $u = (u_j)_{j \in J}$ là một họ *hữu hạn* các phần tử của $\hat{L}(I)$ và cho $v \in \hat{L}(J)$; bằng cách thay các $u_j$ cho các $T_j$ trong $v$, ta thu được một phần tử $w = v((u_j)_{j \in J})$ của $\hat{L}(I)$, ký hiệu là $v \circ u$. Khi đó
$$
w((t_i)_{i \in I}) = v((u_j((t_i)_{i \in I}))_{j \in J})
$$
đối với mọi họ *hữu hạn* $t = (t_i)_{i \in I}$ gồm các phần tử của $g$, như thấy được khi tác động đồng cấu liên tục $\hat{f}_t$ lên đẳng thức $w = v((u_j)_{j \in J})$.

Cho $u = \sum_{\nu \in \mathbf{N}^{I}} u_\nu \in \hat{L}(I)$, trong đó $u_\nu \in L^\nu(I)$. Ánh xạ $\tilde{u}$ $(t_i) \mapsto u((t_i))$ từ $g^I$ vào $g$ là *liên tục*: vì trên mỗi tập mở $g_\alpha$ với $\alpha > 0$ thì họ các $\tilde{u}_\alpha$ là cộng được đều, và chỉ cần chứng minh rằng mỗi $\tilde{u}_\nu$ là liên tục, điều này là ngay lập tức bằng quy nạp theo $|\nu|$.

† Một chuỗi lũy thừa hình thức Lie nói chung không phải là một chuỗi lũy thừa hình thức theo nghĩa của *Đại số*, Chương IV, § 6.

### 4. CHUỖI HAUSDORFF

Cho {U, V} là một tập hợp có hai phần tử.

#### Định nghĩa 1 {#lie-ii-s6-def-1 .statement}

*Phần tử* $H = U \circledast V = \log(\exp U \cdot \exp V)$ (no. 2) *của đại số Lie* $\hat{L}_\mathbf{Q}(\{U, V\})$ *được gọi là chuỗi Hausdorff theo các bất định* U *và* V.

Ta ký hiệu bởi $H_n$ (tương ứng $H_{r,s}$) thành phần thuần nhất của H có bậc toàn phần n (tương ứng đa bậc $(r, s)$). Khi đó

$$
H = \sum_{n \geq 0} H_n = \sum_{r, s \geq 0} H_{r,s}, \quad H_n = \sum_{r+s=n \atop r, s \geq 0} H_{r,s}.
$$

#### Định lý 2 {#lie-ii-s6-thm-2 .statement}

*Nếu r và s là hai số nguyên dương sao cho* $r + s \geq 1$, *thì* $H_{r,s} = H'_{r,s} + H''_{r,s}$, *trong đó*

$$
(r + s)H'_{r,s} =
\sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_{m-1} = s-1 \\ 1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}}
\left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\, U)^{r_m}}{r_m!} (V)
$$

$$
(r + s)H''_{r,s} =
\sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_{m-1} = r-1 \\ s_1 + \cdots + s_{m-1} = s \\ r_1 + s_1 \geq 1, \ldots, r_{m-1} + s_{m-1} \geq 1}}
\left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) (U).
$$

Trong $\hat{A}_\mathbf{Q}(\{U, V\})$, $\exp U \cdot \exp V = 1 + W$, trong đó $W = \sum_{r+s \geq 1} \frac{U^r V^s}{r! s!}$, do đó

$$
H = \sum_{m \geq 1} (-1)^{m-1} W^m / m \text{ (no. 2)}, \text{ nghĩa là:}
$$

$$
H_{r,s} = \sum_{m \geq 1} \frac{(-1)^{m-1}}{m}
\sum_{\substack{r_1 + \cdots + r_m = r \\ s_1 + \cdots + s_m = s \\ r_1 + s_1 \geq 1, \ldots, r_m + s_m \geq 1}}
\prod_{i=1}^m \frac{U^{r_i} V^{s_i}}{r_i! s_i!}.
$$

Ánh xạ tuyến tính $P_n$, được xác định bởi $P_n(x_1, \ldots, x_n) = \frac{1}{n} \left( \prod_{i=1}^{n-1} (\mathrm{ad}\, x_i) \right)(x_n)$ với $n \geq 1$ và $x_1, \ldots, x_n$ trong $\{U, V\}$, là một phép chiếu của $A^n_\mathbf{Q}(\{U, V\})$ lên $L^n_\mathbf{Q}(\{U, V\})$ (§ 3, no. 2, Hệ quả của Mệnh đề 1); vì $H_{r,s}$ thuộc $L^{r+s}_\mathbf{Q}(\{U, V\})$, nên $H_{r,s} = P_{r+s}(H_{r,s})$. Bây giờ

$$
P_{r+s} \left( \prod_{i=1}^m \frac{U^{r_i} V^{s_i}}{r_i! s_i!} \right)
= \frac{1}{r+s} \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\, U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\, V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\, U)^{r_m}}{r_m!} \frac{(\mathrm{ad}\, V)^{s_{m-1}}}{s_{m-1}!} (V)
$$

khi $s_m \geqslant 1$ và

$$
(13)\quad P_{r+s}\left(\prod_{i=1}^{m} \frac{U r_i}{r_i!} \frac{V s_i}{s_i!}\right) = \frac{1}{r+s} \left( \left( \prod_{i=1}^{m-1} \frac{(\mathrm{ad}\ U)^{r_i}}{r_i!} \frac{(\mathrm{ad}\ V)^{s_i}}{s_i!} \right) \frac{(\mathrm{ad}\ U)^{r_m-1}}{r_m!} \right)(U)
$$

khi $r_m \geqslant 1$ và $s_m = 0$. Hơn nữa, hiển nhiên là $(\mathrm{ad}\ t)^{p-1}.t = 0$ nếu $p \geqslant 2$ và $(\mathrm{ad}\ t)^0.t = t$. Do đó hai vế của (12) bằng không khi $s_m \geqslant 2$ và hai vế của (13) bằng không khi $r_m \geqslant 2$. Khi đó định lý suy ra vì $H'_{r,s}$ là tổng của các hạng tử kiểu (12) và $H''_{r,s}$ là tổng của các hạng tử kiểu (13).

#### Nhận xét {#lie-ii-s6-n4-rem-1 .statement}

(1) Ta đã định nghĩa (§ 3, no. 2, Nhận xét) một phép chiếu $Q$ của $A(X)$ lên $L(X)$ sao cho $Q(a^m) = 0$ với $a \in L(X)$ và $m \geqslant 2$ và $Q(1) = 0$. Khi đó $H = Q(\exp H) = Q(\exp U.\exp V)$, do đó ngay lập tức

$$
(14)\quad H_{r,s} = Q \left( \frac{U^r V^s}{r! s!} \right) \quad \text{với } r + s \geqslant 1.
$$

(2) Ta có

$$
(15)\quad H(U, V) \equiv U + V + \frac{1}{2}[U, V] + \frac{1}{12}[U, [U, V]] \\
+ \frac{1}{12}[V, [V, U]] - \frac{1}{24}[U, [V, [U, V]]]
$$
theo modulo $\sum_{n \geqslant 5} L^n(\{U, V\})$.

(3) $H_{0,n} = H_{n,0} = 0$ với mọi số nguyên $n \neq 1$, do đó

$$
(16)\quad H(U, 0) = H(0, U) = U.
$$

Mặt khác, vì $[U, -U] = 0$,

$$
(17)\quad H(U, -U) = 0.
$$

### 5. PHÉP THẾ TRONG CHUỖI HAUSDORFF

Vì $K$ là một trường chứa $\mathbf{Q}$, chuỗi Hausdorff có thể được coi như một chuỗi lũy thừa hình thức Lie với hệ số trong $K$. Do đó, nếu $g$ là một đại số Lie lọc Hausdorff đầy đủ với $g = \bigcup_{\alpha > 0} g_\alpha$, thì với $a, b$ trong $g$, có thể thế $a$ và $b$ cho $U$ và $V$ trong $H$ (x. no. 3 và § 2, no. 5, Nhận xét).

Đặc biệt, cho $A$ là một đại số kết hợp có đơn vị lọc Hausdorff đầy đủ. Ta viết $m = \bigcup_{\alpha > 0} A_\alpha$ và $m_\alpha = A_\alpha \cap m$ với $\alpha \in \mathbf{R}$; do đó $m_\alpha = A_\alpha$ với $\alpha > 0$ và $m_\alpha = m$ với $\alpha \leqslant 0$. Với ngoặc $[a, b] = ab - ba$, $m$ là một đại số Lie lọc Hausdorff đầy đủ, mà điều trên có thể được áp dụng. Với ký hiệu này, ta có kết quả sau đây, kết thúc Mệnh đề 1 của no. 1.

#### Mệnh đề 3 {#lie-ii-s6-prop-3 .statement}

*Nếu $a \in m, b \in m$, thì $\exp H(a, b) = \exp a . \exp b$.*

Cho $a, b$ thuộc $m$; tồn tại $\alpha > 0$ sao cho $a \in A_\alpha$ và $b \in A_\alpha$. Khi đó tồn tại một đồng cấu liên tục $\theta$ từ đại số Magnus $\hat{A}(\{U, V\})$ vào $A$ ánh xạ $U$ thành $a$ và $V$ thành $b$ (§ 5, no. 1, Mệnh đề 1).

Hạn chế của $\theta$ lên $\hat{L}(\{U, V\})$ là một đồng cấu liên tục của các đại số Lie từ $L(\{U, V\})$ vào $m$, ánh xạ $U$ (resp. $V$) thành $a$ (resp. $b$). Do đó, theo công thức (6) của no. 3, ta có $\theta(H) = H(a, b)$. Khi ấy chỉ cần áp dụng đồng cấu liên tục $\theta$ vào hai vế của quan hệ
$$
\exp H(U, V) = \exp U . \exp V
$$
có tính đến *Nhận xét 3* của no. 1.

#### Nhận xét 1 {#lie-ii-s6-n5-rem-1 .statement}

Nếu $a$ và $b$ giao hoán, thì $H_{r,s}(a, b) = 0$ với $r + s \geq 2$, vì mọi đa thức Lie thuần nhất bậc $\geq 2$ đều bằng không tại $(a, b)$. Khi đó $H(a, b) = a + b$ và Mệnh đề 3 cho lại công thức
$$
\exp(a + b) = \exp a . \exp b.
$$

#### Mệnh đề 4 {#lie-ii-s6-prop-4 .statement}

*Cho $g$ là một đại số Lie lọc Hausdorff đầy đủ sao cho $g = \bigcup_{\alpha > 0} g_\alpha$. Ánh xạ $(a, b) \mapsto H(a, b)$ là một luật nhóm trên $g$ tương thích với tôpô trên $g$, đối với nó $0$ là phần tử đơn vị và $-a$ là nghịch đảo của $a$ với mọi $a \in g$.*

Ánh xạ $(a, b) \mapsto H(a, b)$ từ $g \times g$ vào $g$ là liên tục (no. 3); vì ánh xạ $a \mapsto -a$ hiển nhiên là liên tục, nên chỉ cần chứng minh các quan hệ
$$
\begin{align*}
(18) \quad & H(H(a, b), c) = H(a, H(b, c)) \\
(19) \quad & H(a, -a) = 0 \\
(20) \quad & H(a, 0) = H(0, a) = a
\end{align*}
$$
với $a, b, c$ thuộc $g$. Theo công thức (7) của no. 3, chỉ cần chứng minh các công thức này khi $a, b, c$ là ba bất định và $g = \hat{L}(\{a, b, c\})$. Bây giờ hạn chế của ánh xạ mũ lên $\hat{L}(\{a, b, c\})$ là một đơn ánh vào đại số Magnus $\hat{A}(\{a, b, c\})$ và theo Mệnh đề 3:
$$
\begin{align*}
\exp H(H(a, b), c) &= \exp H(a, b) . \exp c = \exp a . \exp b . \exp c \\
\exp H(a, H(b, c)) &= \exp a . \exp H(b, c) = \exp a . \exp b . \exp c \\
\exp H(a, -a) &= \exp a . \exp(-a) = \exp(a - a) = \exp 0 \\
\exp H(a, 0) &= \exp a . \exp 0 = \exp a \\
\exp H(0, a) &= \exp 0 . \exp a = \exp a.
\end{align*}
$$
Điều này thiết lập các quan hệ (18) đến (20).

#### Nhận xét {#lie-ii-s6-n5-rem-2 .statement}

(2) Lấy $g$ là đại số Lie $\hat{L}(X)$. Luật nhóm đưa vào trong mệnh đề trên trùng với luật được xác định ở no. 2. Nói cách khác,
$$
a \mathbin{\mathbf{h}} b = H(a, b) \quad \text{với } a, b \text{ trong } \hat{L}(X);
$$
do đó luật nhóm Hausdorff được cho bởi chuỗi Hausdorff.

(3) Cho $g$ là một đại số Lie với phép lọc nguyên ($\mathcal{C}^n g$) được xác định bởi chuỗi trung tâm dưới. Giả sử tồn tại $m \geq 1$ sao cho $\mathcal{C}^m g = \{0\}$. Với tôpô suy ra từ phép lọc $(\mathcal{C}^n g)_{n \geq 1}$, đại số Lie $g$ là Hausdorff, đầy đủ và thậm chí rời rạc. Khi đó $P(a_1, \ldots, a_r) = 0$ với $a_1, \ldots, a_r$ trong $g$ và với mọi đa thức Lie thuần nhất $P$ có bậc $\geq m$; đặc biệt, $H_{r,s}(a, b) = 0$ với $r + s \geq m$ và chuỗi $H(a, b) = \sum_{r,s} H_{r,s}(a, b)$ chỉ có một số hữu hạn số hạng khác không. Khi đó luật nhóm $(a, b) \mapsto H(a, b)$ trên $g$ là một ánh xạ đa thức (§ 2, no. 4).

#### Mệnh đề 5 {#lie-ii-s6-prop-5 .statement}

*Cho $K_{r,s}$ là thành phần của $H(U + V, -U)$ có đa bậc $(r, s)$. Khi đó*
$$
K_{n,1}(U, V) = \frac{1}{(n+1)!} (\operatorname{ad} U)^n(V) \quad \text{với } n \geq 0.
$$

Ta viết $K(U, V) = H(U + V, -U)$, $K_1(U, V) = \sum_{n \geq 0} K_{n,1}(U, V)$. Ta ký hiệu bởi L (resp. R) phép nhân trái (resp. phải) bởi $U$ trên $\hat{A}(\{U, V\})$.

Ta có thể viết
$$
e^{U}V e^{-U} = \sum_{p, q} \frac{U^p}{p!} V \frac{(-U)^q}{q!}
= \sum_{n \geq 0} \frac{1}{n!} \left( \sum_{p+q=n} \frac{n!}{p!q!} (L^p(-R)^q) \cdot V \right)
= \sum_{n \geq 0} \frac{1}{n!} (L - R)^n V
$$
và do đó
$$
e^{U}V e^{-U} = \sum_{n \geq 0} \frac{1}{n!} (\operatorname{ad} U)^n V.
$$
Bây giờ ta tính theo modulo iđêan $\sum_{m \geq 0} \sum_{n \geq 2} A^{m,n}(\{U, V\})$ của $A(\{U, V\})$. Với mọi $n \geq 1$,
$$
(U + V)^n \equiv U^n + \sum_{i=1}^{n-1} U^i V U^{n-1-i}
$$
do đó
$$
(\operatorname{ad} U)(U + V)^n \equiv ((L - R) \sum_{i=1}^{n-1} L^i R^{n-i}) \cdot V \\
\equiv (L^n - R^n) \cdot V \\
\equiv U^n V - V U^n.
$$
Vì thế
$$
(\operatorname{ad} U) \cdot e^{U+V} \equiv e^{U}V - V e^{U}
$$
sau khi lấy tổng theo $n$.

Mặt khác, $K_1(U, V) \equiv K(U, V)$ và $e^{K_1(U, V)} \equiv 1 + K_1(U, V)$ và do đó
$$
K_1 \equiv e^K - 1 \equiv e^{U+V}e^{-U} - 1
$$
theo Mệnh đề 3. Ta suy ra rằng
$$
\begin{align*}
(\mathrm{ad}\ U)K_1 &\equiv Ue^{U+V}e^{-U} - e^{U+V}e^{-U}U \\
&\equiv (e^{UV} - Ve^U)e^{-U} \quad \text{(theo (23))} \\
&\equiv e^{UV}e^{-U} - V \\
&\equiv \sum_{n \geq 1} \frac{1}{n!} (\mathrm{ad}\ U)^n V \quad \text{(theo (22))} \\
&\equiv (\mathrm{ad}\ U)\left( \sum_{n \geq 0} \frac{(\mathrm{ad}\ U)^n}{(n+1)!} V \right).
\end{align*}
$$
Khi đó chỉ cần áp dụng *Nhận xét* của § 2, no. 11.

### Bài tập {#lie-ii-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).
