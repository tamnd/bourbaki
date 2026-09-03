---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 3
section_title: Rational fractions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.19-A IV.24, A IV.89-A IV.90
pdf_pages: 0028-0033, 0098-0099
extraction: ocr
subsections:
    - "no": 1
      title: Definition of rational fractions
      page: 19
      pdf_page: 28
    - "no": 2
      title: Degrees
      page: 20
      pdf_page: 29
    - "no": 3
      title: Substitutions
      page: 21
      pdf_page: 30
    - "no": 4
      title: Differentials and derivations
      page: 23
      pdf_page: 32
statements: 6
exercises: 7
content_sha256: 245d2428f87dc52cac16107b001d5b8e93f7181582c1085fb67cf4178299ffef
translated_from: content/en/alg/IV/03_s3_rational_fractions.md
source_content_sha256: 7198747b0b6bbdd08037685e5f795da17bcc151029f7c5022d6d539a5ea0b283
translation_model: gpt-5.4
translation_run: translate-vi-f4318889
glossary_version: 34
glossary_terms_sha256: f73a5ae1d01c1698995b7f8178887ba5a6c8e55c8538f7abb4f950f62292be9e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. PHÂN THỨC HỮU TỈ

### 1. Định nghĩa các phân thức hữu tỉ

#### Định nghĩa 1 {#alg-iv-s3-def-1 .statement}

*Cho K là một trường giao hoán và I một tập hợp. Trường phân thức (I, p. 116) của miền nguyên $K[(X_i)_{i \in I}]$ được ký hiệu là $K((X_i)_{i \in I})$ hoặc $K(X_i)_{i \in I}$. Các phần tử của nó được gọi là các phân thức hữu tỉ theo các ẩn số $X_i$ với hệ số trong K.*

Với $I = \{1, 2, \ldots, n\}$ ta viết $K(X_1, X_2, \ldots, X_n)$ thay cho $K((X_i)_{i \in I})$.

Cho A là một miền nguyên và K trường phân thức của nó. Vành $A[(X_i)_{i \in I}]$ có thể được đồng nhất với một vành con của $K[(X_i)_{i \in I}]$, do đó cũng của $K((X_i)_{i \in I})$. Với mỗi $f \in K[(X_i)_{i \in I}]$ tồn tại một phần tử khác không $\alpha$ của A sao cho $\alpha f \in A[(X_i)_{i \in I}]$. Vì thế mọi phần tử của $K((X_i)_{i \in I})$ đều có thể viết dưới dạng $u/v$ với $u, v \in A[(X_i)_{i \in I}], v \neq 0$. Do đó $K((X_i)_{i \in I})$ có thể được đồng nhất với trường phân thức của $A[(X_i)_{i \in I}]$.

Bây giờ cho K là một trường giao hoán, I một tập hợp và J ⊂ I. Đặt B = K[(X_i)_{i ∈ J}], khi đó K[(X_i)_{i ∈ I}] = B[(X_i)_{i ∈ I - J}], và theo điều đã nói ở trên, K((X_i)_{i ∈ I}) có thể được đồng nhất với K'((X_i)_{i ∈ I - J}), trong đó K' = K((X_i)_{i ∈ J}).

### 2. Bậc

Cho K là một trường giao hoán. Với mọi phần tử r của K((X_i)_{i ∈ I}) tồn tại u, v ∈ K[(X_i)_{i ∈ I}] sao cho v ≠ 0 và r = $\frac{u}{v}$. Quan hệ $\frac{u}{v} = \frac{u_1}{v_1}$, trong đó v ≠ 0, v_1 ≠ 0, là tương đương với uv_1 = vu_1; nếu r ≠ 0, ta có u ≠ 0 và u_1 ≠ 0, nên deg u + deg v_1 = deg v + deg u_1 (IV, p. 9), hay cũng vậy deg u − deg v = deg u_1 − deg v_1. Vì thế số nguyên hữu tỉ deg u − deg v chỉ phụ thuộc vào r; ta gọi nó là bậc, hay tổng bậc, của r, và ký hiệu nó là deg r. Ta quy ước viết deg 0 = −∞. Nếu J ⊂ I, ta cũng có thể định nghĩa bậc đối với các X_j có chỉ số j ∈ J. Khi r là một đa thức, các khái niệm này trùng với các khái niệm được định nghĩa trong IV, p. 2.

#### Mệnh đề 1 {#alg-iv-s3-prop-1 .statement}

— Cho r, s là hai phân thức hữu tỉ.

(i) Nếu deg r ≠ deg s, ta có

$$
r + s \neq 0 \quad \text{and} \quad \deg(r + s) = \sup(\deg r, \deg s)
$$

Nếu deg r = deg s, ta có deg(r + s) ≤ deg r.

(ii) Ta có deg(rs) = deg r + deg s.

Ta có thể chỉ xét trường hợp r và s khác không.

Hãy viết r = $\frac{u}{v}$, s = $\frac{w}{z}$, trong đó u, v, w, z là các đa thức khác không. Ta có rs = $\frac{uw}{vz}$, do đó

$$
\deg(rs) = \deg(uw) - \deg(vz) = \deg u - \deg v + \deg w - \deg z =
= \deg r + \deg s.
$$

Mặt khác, ta có r + s = $\frac{uz + vw}{vz}$. Giả sử deg r ≠ deg s, nói cách khác deg u + deg z ≠ deg w + deg v. Khi đó uz + vw ≠ 0, và

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&= \sup(\deg(uz), \deg(vw)) - \deg(vz) \\
&= \sup(\deg(uz) - \deg(vz), \deg(wv) - \deg(vz)) \\
&= \sup(\deg r, \deg s).
\end{align*}
$$

Giả sử deg r = deg s, tức là deg u + deg z = deg w + deg v. Nếu r + s ≠ 0, thì ta có

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&\leq \deg(uz) - \deg(vz) = \deg r
\end{align*}
$$

\* Ánh xạ r ↦ −deg r vì thế là một định giá rời rạc trên trường K((X_i)_{i ∈ I}). \*

### 3. Phép thế

Cho K là một trường giao hoán, E một K-đại số kết hợp có đơn vị, $x = (x_i)_{i \in I}$ một họ các phần tử từng đôi một hoán vị được của E. Đặt $B = K[(X_i)_{i \in I}]$ và $S_x$ là tập hợp tất cả các $v \in B$ khác không sao cho $v(x)$ khả nghịch trong E. Cho $u \in B,\ v \in S_x$ và $f = \frac{u}{v} \in K((X_i)_{i \in I})$. Phần tử $u(x)\ v(x)^{-1} = v(x)^{-1}u(x)$ được xác định trong E; hơn nữa, nếu $u_1,\ v_1$ là hai đa thức sao cho $f = \frac{u_1}{v_1}$ và $v_1 \in S_x$, thì $uv_1 = vu_1$, do đó $u(x)v_1(x) = v(x)u_1(x)$ và vì thế
$$
u(x)\ v(x)^{-1} = u_1(x)\ v_1(x)^{-1}.
$$

Cho $f \in K((X_i)_{i \in I})$. Nếu tồn tại *ít nhất một cặp* $(u, v)$ sao cho $f = \frac{u}{v}$ và $v \in S_x$, ta sẽ nói rằng x *có thể thế được* vào $f$; khi đó phần tử $u(x)\ v(x)^{-1}$, chỉ phụ thuộc vào $f$ và $x$, được ký hiệu là $f(x)$ hoặc $f((x_i))$ hoặc $f((x_i)_{i \in I})$.

#### Mệnh đề 2 {#alg-iv-s3-prop-2 .statement}

*Cho K là một trường giao hoán, E là một K-đại số kết hợp có đơn vị và $x = (x_i)_{i \in I}$ là một họ các phần tử của E hoán vị từng đôi một. Tập $S_x^{-1}B$ các $f \in K((X_i)_{i \in I})$ sao cho có thể thế x vào $f$ là một K-đại số con của $K((X_i)_{i \in I})$. Ánh xạ $f \mapsto f(x)$ là một đồng cấu có đơn vị $\varphi$ từ $S_x^{-1}B$ vào E. Ảnh $\varphi(S_x^{-1}B)$ là tập tất cả các $yz^{-1}$, trong đó y chạy qua đại số con có đơn vị $K[x]_E$ của E được sinh bởi họ x và z chạy qua tập tất cả các phần tử khả nghịch của $K[x]_E$.

Cho $f_1 = \frac{u_1}{v_1},\ f_2 = \frac{u_2}{v_2}$ là hai phần tử của $K((X_i)_{i \in I})$ sao cho $v_1,\ v_2 \in S_x$. Ta có $f_1 + f_2 = \frac{u_1v_2 + u_2v_1}{v_1v_2},\ f_1f_2 = \frac{u_1u_2}{v_1v_2}$ và $v_1,\ v_2 \in S_x$. Do đó $S_x^{-1}B$ là một K-đại số con của $K((X_i)_{i \in I})$. Phần còn lại của mệnh đề là hiển nhiên.

#### Hệ quả {#alg-iv-s3-n3-cor-1 .statement}

*Cho L là một trường giao hoán, K là một trường con của L, $x = (x_i)_{i \in I}$ là một họ các phần tử của L, M là tập gồm các $x_i$, U là tập tất cả các $f \in K((X_i)_{i \in I})$ sao cho có thể thế x vào $f$ và $\varphi$ là đồng cấu $f \mapsto f(x)$ từ U vào L. Khi đó $\varphi(U)$ là trường con của L được sinh bởi $KUM$.*

Cho L' là trường con của L được sinh bởi $KUM$. Ta có
$$
K \cup M \subset \varphi(U) \subset L'
$$
và $\varphi(U)$ là một vành con của L. Bây giờ Mệnh đề 2 suy ra rằng $\varphi(U)$ là một trường con của L, do đó $\varphi(U) = L'$.

Cho $f \in K((X_i)_{i \in I})$ và cho $(g_i)_{i \in I}$ là một họ các phần tử của $K((Y_l)_{l \in L})$. Nếu có thể thế (g_i) vào f, thì f((g_i)) là một phần tử của K((Y_l)_{l \in L}). Đặc biệt, có thể thế $(X_i)_{i \in I}$ vào f và $f = f((X_i)_{i \in I})$.

#### Mệnh đề 3 {#alg-iv-s3-prop-3 .statement}

— Cho E là một đại số trên K, kết hợp, giao hoán, có đơn vị và khác không. Cho f \in K((X_i)_{i \in I}) và với mỗi i \in I, cho $g_i \in K((Y_l)_{l \in L})$. Với một họ y = (y_l)_{l \in L} các phần tử của E, giả sử rằng có thể thế y vào mỗi $g_i$ và có thể thế $(g_i(y))_{i \in I}$ vào f. Khi đó:
(i) có thể thế $(g_i)_{i \in I}$ vào f;
(ii) nếu ký hiệu bởi h phần tử f((g_i)) của K((Y_l)_{l \in L}), thì có thể thế y vào h và h(y) = f((g_i(y))).

Ta có thể giả sử I là hữu hạn. Theo giả thiết, với mỗi $i \in I$, $g_i$ có thể viết dưới dạng $p_i/q_i$ trong đó $p_i, q_i \in K[(Y_l)_{l \in L}]$ và $q_i(y)$ khả nghịch trong E. Tương tự, f có thể viết dưới dạng $u/v$, trong đó $u, v \in K[(X_i)_{i \in I}]$ và $v((g_i(y)))$ khả nghịch. Đặt $m = \sup(\deg u, \deg v)$, và đặt $w = \prod_{i \in I} q_i \in K[(Y_l)_{l \in L}]$, $u_1 = u((g_i)) w^m$, $v_1 = v((g_i)) w^m$. Đa thức u là một tổ hợp K-tuyến tính của các đơn thức $\prod_{i \in I} X_i^{v_i}$ sao cho $\sum_{i \in I} v_i \leq m$. Ta có $w^m \prod_{i \in I} g_i^{v_i} = w^m \left( \prod_{i \in I} p_i^{v_i} \right) \left( \prod_{i \in I} q_i^{v_i} \right)^{-1} \in K[(Y_l)_{l \in L}]$ do lựa chọn m. Do đó $u_1 \in K[(Y_l)_{l \in L}]$ và tương tự $v_1 \in K[(Y_l)_{l \in L}]$. Hơn nữa, $v_1(y) = (w(y))^m v((g_i(y)))$ là khả nghịch. Vậy $v_1 \neq 0$, vì $E \neq 0$, và do đó $v((g_i)) \neq 0$. Như vậy họ $(g_i)$ có thể được thế vào f. Ngoài ra ta có $f((g_i)) = u_1/v_1$, nên có thể thế y vào $h = f((g_i))$, và $h(y) = u_1(y)/v_1(y) = u((g_i(y)))/v((g_i(y))) = f((g_i(y)))$.

Cho K là một trường giao hoán, E là một K-đại số giao hoán, kết hợp và có đơn vị, và cho f \in K((X_i)_{i \in I}). Gọi $T_f$ là tập tất cả các x = (x_i)_{i \in I} \in E^I có thể được thế vào f. Ánh xạ x \mapsto f(x) từ $T_f$ vào E được gọi là hàm hữu tỉ liên kết với f (và E); đôi khi ta ký hiệu nó bởi \tilde{f}. Nếu g \in K((X_i)_{i \in I}) thì ta có T_f \cap T_g \subset T_{f+g}, T_f \cap T_g \subset T_{fg}, do đó hàm hữu tỉ liên kết với f + g (tương ứng fg) được xác định trên T_f \cap T_g và có cùng giá trị trên tập này như \tilde{f} + \tilde{g} (tương ứng \tilde{f}\tilde{g}). Gọi $T'_f$ là tập các x \in T_f sao cho f(x) khả nghịch; nếu x \in T'_f, thì x có thể được thế vào 1/f và hàm hữu tỉ liên kết với 1/f nhận tại x giá trị f(x)^{-1}.

Nếu K là một trường giao hoán vô hạn, f \in K((X_i)_{i \in I}), g \in K((X_i)_{i \in I}) và \tilde{f}, \tilde{g} là các hàm hữu tỉ liên kết với f, g (và K), và nếu \tilde{f}(x) = \tilde{g}(x) với mọi x \in T_f \cap T_g thì f = g. Thật vậy, nếu f = u/v và g = u_1/v_1, trong đó u, v, u_1, v_1 là các đa thức, thì ta có u(x)v_1(x) = u_1(x)v(x) với mọi x sao cho v(x)v_1(x) \neq 0, do đó uv_1 = u_1v (IV, p. 18, Đl. 2). Vì thế ánh xạ f \mapsto \tilde{f} là đơn ánh và ta sẽ thường đồng nhất f với \tilde{f}.

\* Sử dụng tính phân tích duy nhất của $K[(X_i)_{i \in I}]$ (Comm. Alg., VII, § 3, No. 2 p. 502 và Hệ quả của Định lý 2 p. 506), người ta dễ dàng chứng minh điều sau: với mọi $f \in K((X_i)_{i \in I})$ tồn tại $u, v \in K[(X_i)_{i \in I}]$ sao cho: 1) $f = u/v$; 2) để $x \in K^I$ có thể được thay vào $f$ thì điều kiện cần và đủ là $v(x) \neq 0.$

### 4. Vi phân và đạo hàm

Cho $K$ là một trường giao hoán. Theo III, p. 558, Prop. 5, mọi đạo hàm $D$ của $K[(X_i)_{i \in I}]$ đều mở rộng theo một cách duy nhất thành một đạo hàm $\bar{D}$ của $K((X_i)_{i \in I})$. Nếu $D, D'$ là các đạo hàm hoán vị được của $K[(X_i)_{i \in I}]$, thì ngoặc $[D, D'] = DD' - D'D$ bằng không, do đó $[\bar{D}, \bar{D}']$ là một đạo hàm của $K((X_i)_{i \in I})$ mở rộng $[D, D']$ nên cũng bằng không; nói cách khác, $D$ và $D'$ hoán vị được. Đặc biệt các đạo hàm $D_i$ (IV, p. 6) mở rộng thành các đạo hàm của $K((X_i)_{i \in I})$ vẫn được ký hiệu là $D_i$ và hoán vị được từng đôi một. Nếu $f \in K((X_i)_{i \in I}), D_i f$ cũng được viết là $D_{x_i} f$ hoặc $\frac{\partial f}{\partial x_i}$ hoặc $f'_{x_i}$. Khi chỉ có một ẩn duy nhất $X$ thì người ta dùng ký hiệu $Df, \frac{df}{dX}, f'$.

Đặt $B = K[(X_i)_{i \in I}], C = K((X_i)_{i \in I})$. Theo III, p. 574, Prop. 23, ánh xạ chính tắc

$$
\Omega_K(B) \otimes_B C \to \Omega_K(C)
$$

là một đẳng cấu của các không gian vectơ trên $C$. Ghi nhớ III, p. 570, ta thấy rằng không gian vectơ trên $C$ $\Omega_K(C)$ nhận họ $(dX_i)_{i \in I}$ các vi phân của $X_i$ làm cơ sở. Gọi $\partial_i$ là dạng tọa độ chỉ số $i$ trên $\Omega_K(C)$ đối với cơ sở đó. Khi đó ánh xạ $u \mapsto (\partial_i, du)$ từ $C$ vào chính nó là một đạo hàm của $C$, biến $X_i$ thành 1 và $X_j$ thành 0 với $j \neq i$, và do đó bằng $D_i$; nói cách khác, ta có

$$
du = \sum_{i \in I} (D_i u) dX_i
$$

với mọi $u \in C$. Nếu $I$ hữu hạn, $(D_i)_{i \in I}$ là một cơ sở của không gian vectơ trên $C$ các đạo hàm của $C$.

#### Mệnh đề 4 {#alg-iv-s3-prop-4 .statement}

— *Cho $E$ là một $K$-đại số kết hợp, giao hoán và có đơn vị, $x = (x_i)_{i, I}$ một họ các phần tử của $E$ và $f \in K((X_i)_{i, I})$. Giả sử rằng có thể thế $x$ vào trong $f$ và $y = f(x)$.
(i) Với mọi đạo hàm $A$ của $K((X_i)_{i, I})$ ánh xạ $K[(X_i)_{i, I}]$ vào chính nó, có thể thế $x$ vào trong $Af$.
(ii) Với mọi đạo hàm $D$ của $E$ vào một $E$-môđun, ta có

$$
Dy = \sum_{i \in I} (D_i f)(x) \cdot Dx_i .
$$

Đặt $f = \frac{u}{v}$ với $u, v \in K[(X_i)_{i \in I}]$ và $v(x)$ khả nghịch trong E. Gọi A là một đạo hàm của $K((X_i)_{i \in I})$ ánh xạ $K[(X_i)_{i \in I}]$ vào chính nó. Ta có
$$
\Delta f = \frac{(\Delta u)\ v - u(\Delta v)}{v^2}
$$
và $v^2(x)$ khả nghịch, do đó có thể thế x vào trong $Af$. Tiếp theo đặt $r = u(x)$, $s = v(x)$; ta có $y = s^{-1}r$, do đó với mọi đạo hàm D của E vào một E-môđun, ta có
$$
\begin{align*}
Dy &= s^{-2}(s(Dr) - r(Ds)) \\
&= s^{-2}\left( s \sum_{i \in I} (D_iu)(x) \cdot Dx_i - r \sum_{i \in I} (D_iv)(x) \cdot Dx_i \right)
\end{align*}
$$
theo Mệnh đề 4 của IV, p. 6. Vậy $Dy = \sum_{i \in I} w_i \cdot Dx_i$ với
$$
w_i = v(x)^{-2}(v(x)(D_iu)(x) - u(x)(D_iv)(x)) = (D_if)(x).
$$

### Bài tập {#alg-iv-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
