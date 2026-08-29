---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 3
section_title: Passage from a Lie group to its Lie algebra
lang: vi
source: lie-i-iii
pdf_pages: 0256-0297, 0390-0394
extraction: ocr
subsections:
    - "no": 1
      title: CONVOLUTION OF POINT DISTRIBUTIONS ON A LIE GROUP
      page: 0
      pdf_page: 256
    - "no": 2
      title: FUNCTIORAL PROPERTIES
      page: 0
      pdf_page: 259
    - "no": 3
      title: CASE OF A GROUP OPERATING ON A MANIFOLD
      page: 0
      pdf_page: 262
    - "no": 4
      title: CONVOLUTION OF POINT DISTRIBUTIONS AND FUNCTIONS
      page: 0
      pdf_page: 263
    - "no": 5
      title: FIELDS OF POINT DISTRIBUTIONS DEFINED BY THE ACTION OF A GROUP ON A MANIFOLD
      page: 0
      pdf_page: 266
    - "no": 6
      title: INVARIANT FIELDS OF POINT DISTRIBUTIONS ON A LIE GROUP
      page: 0
      pdf_page: 267
    - "no": 7
      title: LIE ALGEBRA OF A LIE GROUP
      page: 0
      pdf_page: 269
    - "no": 8
      title: FUNCTIORIAL PROPERTIES OF THE LIE ALGEBRA
      page: 0
      pdf_page: 272
    - "no": 9
      title: LIE ALGEBRA OF THE GROUP OF INVERTIBLE ELEMENTS OF AN ALGEBRA
      page: 0
      pdf_page: 275
    - "no": 10
      title: LIE ALGEBRAS OF CERTAIN LINEAR GROUPS
      page: 0
      pdf_page: 276
    - "no": 11
      title: LINEAR REPRESENTATIONS
      page: 0
      pdf_page: 277
    - "no": 12
      title: ADJOINT REPRESENTATION
      page: 0
      pdf_page: 282
    - "no": 13
      title: TENSORS AND INVARIANT FORMS
      page: 0
      pdf_page: 286
    - "no": 14
      title: MAURER–CARTAN FORMULAE
      page: 0
      pdf_page: 287
    - "no": 15
      title: CONSTRUCTION OF INVARIANT DIFFERENTIAL FORMS
      page: 0
      pdf_page: 289
    - "no": 16
      title: HAAR MEASURE ON A LIE GROUP
      page: 0
      pdf_page: 289
    - "no": 17
      title: LEFT DIFFERENTIAL
      page: 0
      pdf_page: 292
    - "no": 18
      title: LIE ALGEBRA OF A LIE GROUP GERM
      page: 0
      pdf_page: 294
statements: 111
exercises: 9
content_sha256: 5b855e461b7be902c53dc17423395fa303518f486e7b80881751a14b80b25b79
translated_from: content/en/lie/III/03_s3_passage_from_a_lie_group_to_its_lie.md
source_content_sha256: 116ee476020d95a20632b0a93e7c92ab47b1013c10697310c58d2ebb5dec4db5
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4-mini, gpt-5-mini
translation_run: translate-vi-36d03b2e
glossary_version: 34
glossary_terms_sha256: e4941a69ba07ea62b910cb6b3b296023187819bc958439ee07c893dec6015980
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. TỪ MỘT NHÓM LIE ĐẾN ĐẠI SỐ LIE CỦA NÓ

### 1. PHÉP TÍCH CHẬP CỦA CÁC PHÂN BỐ ĐIỂM TRÊN MỘT NHÓM LIE

#### Định nghĩa 1 {#lie-iii-s3-def-1 .statement}

*Cho $G$ là một nhóm Lie, $g$ và $g'$ là hai điểm của $G$ và cho $t \in T_g^{(\infty)}(G)$ $t' \in T_{g'}^{(\infty)}(G)$ là hai phân bố điểm tại $g$ và $g'$ trên $G$ (*Differentiable and Analytic Manifolds*, R, 13.2.1). Tích chập của $t$ và $t'$, ký hiệu bởi $t * t'$, là ảnh của $t \otimes t'$ qua ánh xạ $(h, h') \mapsto hh'$ của $G \times G$ vào $G$ (*Differentiable and Analytic Manifolds*, R, 13.2.3).*

#### Mệnh đề 1 {#lie-iii-s3-prop-1 .statement}

(i) *Nếu $t \in T_g^{(s)}(G)$ và $t' \in T_{g'}^{(s')}(G)$, thì $t * t' \in T_{gg'}^{(s+s')}(G)$.*

(ii) *Nếu $t$ hoặc $t$ không có số hạng hằng, thì $t * t'$ không có số hạng hằng.*

(iii) $\varepsilon_g * \varepsilon_{g'} = \varepsilon_{gg'}$.

(iv) *Cho $t \in T_g^{(s)}(G)$, $t' \in T_{g'}^{(s')}(G)$ và cho $f$ là một hàm thuộc lớp $C^{s+s'}$ trong một lân cận mở của $gg'$ với các giá trị trong một không gian đa chuẩn Hausdorff. Khi đó*

$$
\langle t * t', f \rangle = \langle t', h' \mapsto \langle t, h \mapsto f(hh') \rangle \rangle \\
= \langle t, h \mapsto \langle t', h' \mapsto f(hh') \rangle \rangle.
$$

Điều này suy ra từ Differentiable and Analytic Manifolds, R, 13.4.1, 13.2.3 và 13.4.4.

Giả sử rằng K = \mathbf{R} hoặc \mathbf{C} và rằng G là hữu hạn chiều. Khi đó G là compact địa phương. Nếu t, t' là các độ đo điểm, định nghĩa của t \* t' trùng với định nghĩa trong Integration, Chương VIII, § 1. Sau này ta sẽ thấy rằng tích chập của các độ đo và tích chập của các phân bố điểm là hai trường hợp đặc biệt của tích chập của các phân bố không nhất thiết là phân bố điểm.

Cho \mathcal{T}^{(\infty)}(G) là tổng trực tiếp của các T_g^{(\infty)}(G) với g \in G (xem Differentiable and Analytic Manifolds, R, 13.6.1). Ta định nghĩa tích chập trong \mathcal{T}^{(\infty)}(G) là ánh xạ song tuyến tính từ \mathcal{T}^{(\infty)}(G) \times \mathcal{T}^{(\infty)}(G) vào \mathcal{T}^{(\infty)}(G) mở rộng tích chập của Định nghĩa 1. Ta cũng ký hiệu nó bởi *. Như vậy \mathcal{T}^{(\infty)}(G) có một cấu trúc đại số được lọc bởi các \mathcal{T}^{(s)}(G). Đại số con \mathcal{T}^{(0)}(G) = \bigoplus_{g \in G} T_g^{(0)}(G) được đồng nhất với đại số K^{(G)} của nhóm G trên K.

#### Mệnh đề 2 {#lie-iii-s3-prop-2 .statement}

Đại số \mathcal{T}^{(\infty)}(G) là kết hợp. Nó là giao hoán khi và chỉ khi G là giao hoán.

Cho t \in \mathcal{T}^{(\infty)}(G), t' \in \mathcal{T}^{(\infty)}(G), t'' \in \mathcal{T}^{(\infty)}(G). Khi đó t \* (t' \* t'') là ảnh của t \otimes t' \otimes t'' qua ánh xạ (g, g', g'') \mapsto g(g'g'') của G \times G \times G vào G và (t \* t') \* t'' là ảnh của t \otimes t' \otimes t'' qua ánh xạ (g, g', g'') \mapsto (gg')g'' của G \times G \times G vào G. Do đó (t \* t') \* t'' = t \* (t' \* t''). Tương tự, ta thấy rằng, nếu G là giao hoán, thì t \* t' = t' \* t. Nếu tích chập là giao hoán, G là giao hoán theo Mệnh đề 1 (iii).

#### Mệnh đề 3 {#lie-iii-s3-prop-3 .statement}

Nếu t \in \mathcal{T}^{(\infty)}(G) và g \in G, thì $\gamma(g)_* t = \varepsilon_g * t, \delta(g)_* t = t * \varepsilon_{g^{-1}}$, (Int g)_* t = $\varepsilon_g * t * \varepsilon_{g^{-1}}$. Đặc biệt, $\varepsilon_e$ là phần tử đơn vị của \mathcal{T}^{(\infty)}(G).

Xét biểu đồ

$$
\begin{array}{ccccc}
G & \xrightarrow{\phi} & G \times G & \xrightarrow{\psi} & G \\
\end{array}
$$

trong đó $\phi$ là ánh xạ $h \mapsto (g, h)$ và $\psi$ là ánh xạ $(h', h) \mapsto h'h$. Khi đó $\gamma(g) = \psi \circ \phi$ và do đó $\gamma(g)_* t = \psi_*(\phi_*(t))$. Nhưng $\phi_*(t) = \varepsilon_g \otimes t$ và do đó $\psi_*(\phi_*(t)) = \varepsilon_g * t$. Lập luận tương tự đối với $\delta(g)_* t$. Cuối cùng,

$$
\operatorname{Int} g = \gamma(g) \circ \delta(g)
$$

và do đó $(\operatorname{Int} g)_* = \gamma(g)_* \circ \delta(g)_*$.

Vì vậy ta thấy rằng, với $t \in T(G)$, $\varepsilon_g * t$ và $t * \varepsilon_g$ bằng với $gt$ và $tg$ được tính trong nhóm T(G) (§ 2, no. 2). Nhưng cần lưu ý rằng, với $t, t'$ trong T(G), tích $tt'$ theo nghĩa của § 2 nói chung khác với $t * t'$.

#### Định nghĩa 2 {#lie-iii-s3-def-2 .statement}

Cho G là một nhóm Lie. Đại số con của $\mathcal{T}^{(\infty)}(G)$ gồm các phân bố có giá được chứa trong e được ký hiệu bởi $U(G)$.

Đại số này được lọc bởi các không gian con
$$
U_s(G) = U(G) \cap \mathcal{T}^{(s)}(G) = T_e^{(s)}(G).
$$
Ta viết $U^+(G) = T_e^{(\infty)+}(G)$, $U_s^+(G) = U^+(G) \cap U_s(G)$ (xem Các đa tạp khả vi và giải tích, R, 13.2.1). Nhắc lại rằng $U_0(G)$ được đồng nhất với K và $U_1^+(G)$ với không gian tiếp xúc $T_e(G)$. Trong $U(G)$, $U^+(G)$ là một iđêan hai phía bù cho $U_0(G)$.

#### Ví dụ {#lie-iii-s3-n1-exa-1 .statement}

Cho E là một không gian chuẩn được đầy đủ được xét như một nhóm Lie. Khi đó không gian vectơ $U(E)$ được đồng nhất một cách chính tắc với không gian vectơ TS(E) (Các đa tạp khả vi và giải tích, R, 13.2.4). Cho $m : E \times E \to E$ là phép cộng trên E. Khi đó
$$
m_* : TS(E \times E) \to TS(E)
$$
bằng TS(m) (Các đa tạp khả vi và giải tích, R, 13.2.4). Với $t, t'$ trong $U(E) = TS(E)$, ảnh $t * t'$ của tích tenxơ đối xứng $t \otimes t'$ qua $m_*$ do đó là TS(m)($t \otimes t'$). Theo Đại số, Chương IV, § 5, no. 6, Mệnh đề 7, ảnh này chính là tích $tt'$ trong đại số TS(E). Do đó đại số $U(E)$ được đồng nhất với đại số TS(E).

#### Mệnh đề 4 {#lie-iii-s3-prop-4 .statement}

Xét ánh xạ song tuyến tính $(u, v) \mapsto u * v$ (tương ứng $(u, v) \mapsto v * u$) của $U(G) \otimes K^{(G)}$ vào $\mathcal{T}^{(\infty)}(G)$. Ánh xạ tuyến tính tương ứng của $U(G) \otimes K^{(G)}$ vào $\mathcal{T}^{(\infty)}(G)$ là một đẳng cấu không gian vectơ.

$K^{(G)}$ là tổng trực tiếp của các $K_{e_x}$ với $x \in G$. Mặt khác, ánh xạ $u \mapsto u * \varepsilon_g$ (tương ứng $u \mapsto \varepsilon_g * u$) là một đẳng cấu của không gian vectơ $U(G) = \mathcal{T}_e^{(\infty)}(G)$ lên không gian vectơ $\mathcal{T}_g^{(\infty)}(G)$ theo Mệnh đề 3. Cuối cùng, $\mathcal{T}^{(\infty)}(G)$ là tổng trực tiếp của các $T_g^{(\infty)}(G)$ với $g \in G$.

Cho X là một đa tạp thuộc lớp $C^r$ ($r \geq \infty$) và $x \in X$. Ta đã định nghĩa (Các đa tạp khả vi và giải tích, R, 13.3.1) một phép lọc chính tắc trên không gian vectơ $\mathcal{T}_x^{(\infty)}(X)$ và một đẳng cấu chính tắc $i_{X,x}$ của không gian vectơ phân bậc liên kết lên không gian vectơ phân bậc TS(T_x(X)). Đặc biệt, cho $T_e(G) = L$; khi đó $i_{G,e}$ là một đẳng cấu của không gian vectơ phân bậc gr U(G) lên không gian vectơ phân bậc TS(L). Nhưng U(G) là một đại số được lọc, từ đó ta thu được một cấu trúc đại số phân bậc trên gr U(G).

#### Mệnh đề 5 {#lie-iii-s3-prop-5 .statement}

Đẳng cấu $i_{G,e} : \mathrm{gr}\ U(G) \to \mathrm{TS}(L)$ là một đẳng cấu đại số.

Cho $p$ là ánh xạ $(t, t') \mapsto t \otimes t'$ của $U(G) \times U(G)$ vào $U(G \times G)$. Cho c là ánh xạ $(t, t') \mapsto t * t'$ của $U(G) \times U(G)$ vào $U(G)$. Cho m là ánh xạ $(g, g') \mapsto gg'$ của $G \times G$ vào G. Khi đó theo Định nghĩa 1
$$
c = m_* \circ p.
$$

Xét biểu đồ
$$
\begin{array}{ccc}
\mathrm{gr}\,\mathrm{U}(G) \times \mathrm{gr}\,\mathrm{U}(G) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}\,\mathrm{U}(G \times G) \\
\downarrow i_{G,e} \times i_{G,e} & & \downarrow i_{G \times G,e} \\
\mathrm{TS}(L) \times \mathrm{TS}(L) & \xrightarrow{q} & \mathrm{TS}(L \times L) \\
& & \xrightarrow{\mathrm{TS}(T(m))} \mathrm{TS}(L)
\end{array}
$$
trong đó $q$ là ánh xạ dẫn xuất từ đẳng cấu chính tắc của $\mathrm{TS}(L) \times \mathrm{TS}(L)$ lên $\mathrm{TS}(L \times L)$. Theo *Differentiable and Analytic Manifolds*, R, 13.4.6 và 13.3.5, hai hình vuông của biểu đồ là giao hoán. Do đó theo (1), biểu đồ
$$
\begin{array}{ccc}
\mathrm{gr}\,\mathrm{U}(G) \times \mathrm{gr}\,\mathrm{U}(G) & \xrightarrow{\mathrm{gr}(c)} & \mathrm{gr}\,\mathrm{U}(G) \\
\downarrow i_{G,e} \times i_{G,e} & & \downarrow i_{G,e} \\
\mathrm{TS}(L) \times \mathrm{TS}(L) & \xrightarrow{\mathrm{TS}(T(m)) \circ q} & \mathrm{TS}(L)
\end{array}
$$
là giao hoán. Bây giờ $T(m): L \times L \to L$ ánh xạ $(x, y)$ thành $x + y$ (§ 2, no. 1, Mệnh đề 2 (ii)). Theo *Algebra*, Chương IV, § 5, no. 6, Mệnh đề 7, $\mathrm{TS}(T(m)) \circ q$ do đó là phép nhân của đại số $\mathrm{TS}(L)$.

### 2. CÁC TÍNH CHẤT HÀM TỬ

#### Mệnh đề 6 {#lie-iii-s3-prop-6 .statement}

Cho $G, H$ là các nhóm Lie và $\phi$ là một cấu xạ của $G$ vào $H$. Với $t, t'$ trong $\mathcal{T}^{(\infty)}(G)$, $\phi_*(t * t') = \phi_*(t) * \phi_*(t')$.

Xét biểu đồ
$$
\begin{array}{ccc}
G \times G & \xrightarrow{m} & G \\
\phi \times \phi \downarrow & & \downarrow \phi \\
H \times H & \xrightarrow{n} & H
\end{array}
$$
trong đó $m(g, g') = gg'$, $n(h, h') = hh'$. Biểu đồ này là giao hoán. Do đó
$$
\begin{align*}
\phi_*(t * t') &= \phi_*(m_*(t \otimes t')) = n_*((\phi \times \phi)_*(t \otimes t')) \\
&= n_*(\phi_*(t) \otimes \phi_*(t')) = \phi_*(t) * \phi_*(t').
\end{align*}
$$

Các nhóm Lie $G$ và $G^\vee$ có cùng đa tạp nền và do đó các không gian vectơ $\mathcal{T}^{(\infty)}(G)$ và $\mathcal{T}^{(\infty)}(G^\vee)$ là như nhau. Gọi $\theta$ là ánh xạ $g \mapsto g^{-1}$, là một đẳng cấu của nhóm Lie $G$ lên nhóm Lie $G^\vee$. Khi đó $\theta^*$ là một tự đẳng cấu của không gian vectơ $\mathcal{T}^{(\infty)}(G)$, mà tự đẳng cấu này ta ký hiệu bởi $t \mapsto t^\vee$. Khi đó $(\varepsilon_g)^\vee = \varepsilon_{g^{-1}}$. Nếu $t \in T_e(G)$, thì
$$
t^\vee = -t \quad (§ 2, \text{Mệnh đề 2}).
$$

#### Ví dụ {#lie-iii-s3-n2-exa-1 .statement}

Giả sử rằng $G$ là nhóm Lie được xác định bởi một không gian chuẩn hóa đầy đủ $E$. Khi đó $\mathrm{U}(G)$ được đồng nhất với $\mathrm{TS}(E)$ và hạn chế $\theta_*$ vào $\mathrm{U}(G)$ được đồng nhất với $\mathrm{TS}(T_e(\theta))$ (*Differentiable and Analytic Manifolds*, R, 13.2.4). Do đó, nếu $t \in \mathrm{TS}^s(E)$, $t^\vee = (-1)^s t$.

#### Mệnh đề 7 {#lie-iii-s3-prop-7 .statement}

Cho G là một nhóm Lie. Cho t, t' thuộc $\mathcal{T}^{(\infty)}(G)$.

(i) Tích $t * t'$ được tính đối với $G^\vee$ bằng tích $t' * t$ được tính đối với G.

(ii) $(t * t')^\vee = {t'}^\vee * t^\vee$.

Xét biểu đồ

$$
\begin{array}{ccc}
(G_1 \times G_2) \times (G_1 \times G_2) & \xrightarrow{m} & G_1 \times G_2 \\
\downarrow n & & \uparrow p_1 \times p_2 \\
(G_1 \times G_1) \times (G_2 \times G_2)
\end{array}
$$

trong đó $s(g, g') = (g', g)$, $m(g, g') = gg'$, $n(g, g') = g'g$ với mọi $g, g'$ trong G. Biểu đồ này là giao hoán. Do đó $n_*(t \otimes t') = m_*(s_*(t \otimes t')) = m_*(t' \otimes t)$. Đẳng thức này chính xác là (i). Mệnh đề (ii) suy ra từ (i) và Mệnh đề 6.

#### Mệnh đề 8 {#lie-iii-s3-prop-8 .statement}

Cho G, H là các nhóm Lie và $\phi$ là một cấu xạ của G vào H. Nếu $t \in \mathcal{T}^{(\infty)}(G)$, thì $\phi_*(t^\vee) = (\phi_*(t))^\vee$.

Cho $\theta$ (tương ứng $\theta'$) là ánh xạ $g \mapsto g^{-1}$ của G vào G (tương ứng của H vào H). Khi đó $\phi \circ \theta = \theta' \circ \phi$, do đó $\phi_*(\theta_*(t)) = \theta'_*(\phi_*(t))$.

#### Mệnh đề 9 {#lie-iii-s3-prop-9 .statement}

Cho $G_1, \ldots, G_n$ là các nhóm Lie và $G = G_1 \times \cdots \times G_n$. Nếu các không gian vectơ $\mathcal{T}^{(\infty)}(G)$ và $\mathcal{T}^{(\infty)}(G_1) \otimes \cdots \otimes \mathcal{T}^{(\infty)}(G_n)$ được đồng nhất một cách chính tắc, thì đại số $\mathcal{T}^{(\infty)}(G)$ là tích tenxơ của các đại số $\mathcal{T}^{(\infty)}(G_1), \ldots, \mathcal{T}^{(\infty)}(G_n)$. Nếu $t_i \in \mathcal{T}^{(\infty)}(G_i)$ với $i = 1, \ldots, n$, thì

$$
(t_1 \otimes \cdots \otimes t_n)^\vee = t_1^\vee \otimes \cdots \otimes t_n^\vee.
$$

Chỉ cần xét trường hợp $n = 2$. Cho $t_1, t_1'$ thuộc $\mathcal{T}^{(\infty)}(G_1)$, $t_2, t_2'$ thuộc $\mathcal{T}^{(\infty)}(G_2)$. Ta cần chứng minh rằng $(t_1 \otimes t_2) * (t_1' \otimes t_2') = (t_1 * t_1') \otimes (t_2 * t_2')$ và rằng $(t_1 \otimes t_2)^\vee = t_1^\vee \otimes t_2^\vee$. Xét biểu đồ

$$
\begin{array}{ccc}
G \times G & \xrightarrow{s} & G \times G \\
\downarrow n & & \downarrow m \\
G & & G
\end{array}
$$

trong đó $m((x_1, x_2), (x_1', x_2')) = (x_1 x_1', x_2 x_2')$,

$$
n((x_1, x_2), (x_1', x_2')) = ((x_1, x_1'), (x_2, x_2')),
$$

$p_1(x_1, x_1') = x_1 x_1'$, $p_2(x_2, x_2') = x_2 x_2'$. Biểu đồ này giao hoán. Do đó

$$
m_*((t_1 \otimes t_2) \otimes (t_1' \otimes t_2')) = (p_1 \otimes p_2)_*(n_*((t_1 \otimes t_2) \otimes (t_1' \otimes t_2'))),
$$

nghĩa là

$$
\begin{align*}
(t_1 \otimes t_2) * (t_1' \otimes t_2') &= (p_1 \otimes p_2)_*((t_1 \otimes t_1') \otimes (t_2 \otimes t_2')) \\
&= p_1*(t_1 \otimes t_1') \otimes p_2*(t_2 \otimes t_2') \\
&= (t_1 * t_1') \otimes (t_2 * t_2').
\end{align*}
$$

Tương tự, ta thấy rằng $(t_1 \otimes t_2)^\vee = t_1^\vee \otimes t_2^\vee$.

#### Mệnh đề 10 {#lie-iii-s3-prop-10 .statement}

Cho H là một nhóm con Lie của G và $i : H \to G$ là đơn ánh chính tắc. Khi đó $i_*$ là một đồng cấu đơn ánh của đại số $\mathcal{T}^{(\infty)}(H)$ vào đại số $\mathcal{T}^{(\infty)}(H)$ và $i_*(t^\vee) = (i_*(t))^\vee$ với mọi $t \in \mathcal{T}^{(\infty)}(H)$.

Điều này suy ra từ các Mệnh đề 6 và 8 và Differentiable and Analytic Manifolds, R, 13.2.3.

$\mathcal{T}^{(\infty)}(H)$ được đồng nhất với một đại số con của $\mathcal{T}^{(\infty)}(G)$ nhờ đẳng cấu của Mệnh đề 10.

#### Nhận xét {#lie-iii-s3-n2-rem-1 .statement}

Mệnh đề 10 vẫn đúng nếu H là một nhóm quasi-con Lie.

Ta nhắc lại (Differentiable and Analytic Manifolds, R, 13.5.1) rằng, nếu V là một đa tạp giải tích trên K, $\mathcal{T}^{(\infty)}(V)$ có một cách chính tắc một cấu trúc đối đại số trên K với một đồng đơn vị; đồng đơn vị là ánh xạ tuyến tính của $\mathcal{T}^{(\infty)}(G)$ vào K gán cho mỗi phần tử của $T_x^{(\infty)}(V)$ số hạng hằng của nó.

#### Mệnh đề 11 {#lie-iii-s3-prop-11 .statement}

Cho G là một nhóm Lie.
(i) Đối đại số $\mathcal{T}^{(\infty)}(G)$, với tích chập, là một đại đối đại số (Algebra, Chapter III, § 11, no. 4).
(ii) Cho c là đồng tích trên $\mathcal{T}^{(\infty)}(G)$. Cho $t \in \mathcal{T}^{(\infty)}(G)$ và viết
$$
c(t) = \sum_{i=1}^n t_i \otimes t_i'.
$$
Khi đó $c(t^\vee) = \sum_{i=1}^n t_i^\vee \otimes t_{i'}^\vee$.

Ta chứng minh (i). Trong định nghĩa về đại đối đại số được dẫn chiếu, điều kiện (1) suy ra từ các Mệnh đề 2 và 3 và điều kiện (2) suy ra từ Differentiable and Analytic Manifolds, R, 13.5.1. Cho d là ánh xạ $g \mapsto (g, g)$ của G vào $G \times G$. Khi đó $c = d_*$ và do đó c là một cấu xạ đại số (các Mệnh đề 6 và 9), đó là điều kiện (3). Cho $t \in T_g^{(\infty)}(G)$, $t' \in T_{g'}^{(\infty)}(G)$ không có số hạng hằng và $\lambda, \lambda'$ là các phần tử của K; khi đó $\varepsilon_g \otimes t', t \otimes \varepsilon_{g'}, t \otimes t'$ không có số hạng hằng (Differentiable and Analytic Manifolds, R, 13.4.1) và do đó số hạng hằng của $(\lambda \varepsilon_g + t) * (\lambda' \varepsilon_{g'} + t')$ là $\lambda \lambda'$; do đó điều kiện (4) được thỏa mãn.

Ta chứng minh (ii). Theo các Mệnh đề 8 và 9,
$$
c(t^\vee) = d_*(t^\vee) = (d_*(t))^\vee = \left( \sum_{i=1}^n t_i \otimes t_i' \right)^\vee = \sum_{i=1}^n t_{i'}^\vee \otimes t_{i'}^\vee.
$$

#### Mệnh đề 12 {#lie-iii-s3-prop-12 .statement}

Cho G, H là hai nhóm Lie và $\phi$ là một cấu xạ của G vào H. Khi đó $\phi_*$ là một cấu xạ đại đối đại số của $\mathcal{T}^{(\infty)}(G)$ vào $\mathcal{T}^{(\infty)}(H)$.

Điều này suy ra từ Mệnh đề 6 và Differentiable and Analytic Manifolds, R, 13.5.1.

Cho G là một nhóm Lie. Các hạn chế của phép chập và đồng tích lên U(G) định nghĩa một cấu trúc bigebra trên U(G). Ta có U(G)^{\vee} = U(G). Nếu $\phi : G \to H$ là một cấu xạ nhóm Lie, ta ký hiệu U($\phi$) là ánh xạ $t \mapsto \phi_*(t)$ của U(G) vào U(H); đây là một cấu xạ bigebra. Nếu $\psi : H \to L$ là một cấu xạ nhóm Lie khác, thì U($\psi \circ \phi$) = U($\psi$) \circ U($\phi$). Nếu $\phi$ là một phép nhúng (tương ứng. một phép chiếu), U($\phi$) là đơn ánh (tương ứng. toàn ánh) theo *Differentiable and Analytic Manifolds*, R, 13.2.3. Đặc biệt, nếu H là một nhóm con Lie của G, U(H) được đồng nhất với một đại số con của U(G), đồng tích trên U(H) là hạn chế của đồng tích trên U(G). Nếu H là mở trong G, thì U(H) = U(G). Nếu G_1, G_2 là các nhóm Lie, U(G_1 \times G_2) được đồng nhất với U(G_1) \times U(G_2). Các phần tử nguyên thủy của U(G) là các phần tử của T_e(G) (*Differentiable and Analytic Manifolds*, R, 13.5.3).

Một lần nữa cho $\phi : G \to H$ là một cấu xạ nhóm Lie. Nếu gr U(G) được đồng nhất với TS(T_e(G)) và gr U(H) với TS(T_e(H)), thì gr U($\phi$) được đồng nhất với TS(T_e($\phi$)) (*Differentiable and Analytic Manifolds*, R, 13.3.5). Ta áp dụng điều này cho đẳng cấu $g \mapsto g^{-1}$ của G lên G^{\vee}; khi đó T_e($\phi$) = -1 và do đó

$$
t \in U_s(G) \Rightarrow t^{\vee} \equiv (-1)^s t \mod U_{s-1}(G).
$$

### 3. TRƯỜNG HỢP MỘT NHÓM TÁC ĐỘNG LÊN MỘT ĐA TẠP

Cho G là một nhóm Lie, X là một đa tạp thuộc lớp C^r và f là một luật tác động trái thuộc lớp C^r của G lên X. Nếu $t \in T^{(s)}_g(G)$ và $u \in T^{(s')}_x(X)$ và $s + s' \leq r$, ta ký hiệu $t * u$ là ảnh của $t \otimes u$ qua $f_*$. Ta mở rộng tích \* thành một ánh xạ song tuyến tính cũng được ký hiệu bởi *, từ $\mathcal{T}^{(s)}(G) + \mathcal{T}^{(s')}(X)$ vào $\mathcal{T}^{(s+s')}(X)$. Mệnh đề 1 của no. 1 có thể được mở rộng với những sửa đổi hiển nhiên cho trường hợp hiện tại.

Khi G tác động lên chính nó bằng phép tịnh tiến trái, ta thu được lại Định nghĩa 1 của no. 1.

#### Mệnh đề 13 {#lie-iii-s3-prop-13 .statement}

Cho $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G)$, $u \in \mathcal{T}^{(s'')}(X)$, sao cho

$$
s + s' + s'' \leq r.
$$

Khi đó $(t * t') * u = t * (t' * u)$.

Điều này có thể được chứng minh như Mệnh đề 2 của no. 1.

Đặc biệt, nếu $r \leq \infty$, không gian vectơ $\mathcal{T}^{(\infty)}(X)$ là một môđun trái trên đại số $\mathcal{T}^{(\infty)}(G)$ với tích *.

#### Mệnh đề 14 {#lie-iii-s3-prop-14 .statement}

(i) Cho $g_0 \in G$ và $\tau(g_0)$ là ánh xạ $x \mapsto f(g_0, x)$ của X vào X. Nếu $u \in \mathcal{T}^{(r)}(X)$, thì $\tau(g_0)*u = \varepsilon_{g_0}*u$.

(ii) Cho $x_0 \in X$ và $\varrho(x_0)$ là ánh xạ $g \mapsto f(g, x_0)$ của G vào X. Nếu $t \in T^{(r)}(G)$, thì $\varrho(x_0)*t = t*\varepsilon_{x_0}$.

Điều này có thể được chứng minh như Mệnh đề 3 của no. 1.

Đặc biệt, nếu $u \in T(X)$ và $t \in T(G)$, $\varepsilon_{g_0} * u$ và $t * \varepsilon_{x_0}$ bằng các tích $g_0u$ và $tx_0$ được định nghĩa trong § 2, no. 2.

#### Mệnh đề 15 {#lie-iii-s3-prop-15 .statement}

Cho G (tương ứng. G') là một nhóm Lie và X (tương ứng. X') là một đa tạp thuộc lớp C^r. Giả sử đã cho một luật tác động trái thuộc lớp C^r của G (tương ứng. G') lên X (tương ứng. X'). Cho $\phi$ là một cấu xạ của G vào G' và $\psi$ là một $\phi$-cấu xạ của X vào X'. Cho $t \in \mathcal{T}^{(s)}(G)$, $u \in T^{(s')}(X)$ sao cho $s + s' \leq r$. Khi đó
$$
\psi_*(t * u) = \phi_*(t) * \psi_*(u).
$$
Điều này có thể được chứng minh như Mệnh đề 6 của no. 2.

#### Nhận xét {#lie-iii-s3-n3-rem-1 .statement}

Cho f là một luật tác động phải thuộc lớp C^r của G lên X. Nếu $t \in \mathcal{T}^{(s)}(G)$ và $u \in \mathcal{T}^{(s')}(X)$, với $s + s' \leq r$, ta ký hiệu $u * t$ là ảnh của $u \otimes t$ qua $f_*$. Các Mệnh đề 13, 14, 15 chuyển sang trường hợp này theo một cách hiển nhiên.

#### Mệnh đề 16 {#lie-iii-s3-prop-16 .statement}

Cho G, G' là các nhóm Lie, X là một đa tạp lớp C^r và giả sử G (tương ứng G') tác động lên X bên trái (tương ứng bên phải), với $(gx)g' = g(xg')$ với mọi $x \in X, g \in G, g' \in G'$. Cho $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G')$, $t'' \in T^{(s'')}(X)$, với $s + s' + s'' \leq r$. Khi đó
$$
(t * t'') * t' = t * (t'' * t').
$$
$(t * t'') * t'$ (tương ứng $t * (t'' * t')$) là ảnh của $t \otimes t'' \otimes t'$ qua ánh xạ $(g, x, g') \mapsto (gx)g'$ (tương ứng $g(xg')$) từ $G \times X \times G'$ vào X.

### 4. TÍCH CHẬP CỦA PHÂN BỐ ĐIỂM VÀ HÀM SỐ

Cho G là một nhóm Lie, X là một đa tạp lớp C^r và $(g, x) \mapsto gx$ là một luật của phép toán trái lớp C^r của G trên X. Với mọi $x \in X$, ký hiệu $\varrho(x)$ là ánh xạ quỹ đạo của x.

#### Definition 3 {#lie-iii-s3-def-3 .statement}

Cho $t \in \mathcal{T}^{(s)}(G)$ với $s \leq r$. Cho $f : X \to F$ là một hàm lớp C^r nhận giá trị trong một không gian đa chuẩn Hausdorff (chẳng hạn $F = \mathbf{K}$). Tích chập của t và f, ký hiệu là $t * f$, là hàm trên X nhận giá trị trong F được xác định bởi
$$
(t * f)(x) = \langle t^\vee * \varepsilon_x, f \rangle.
$$
Khi đó
$$
\begin{align*}
(t * f)(x) &= \langle \varrho(x)_*(t^\vee), f \rangle \quad \text{(no. 3, Mệnh đề 14 (ii))} \\
&= \langle t^\vee, f \circ \varrho(x) \rangle \quad \text{(Diff. \& Anal. Man., R, 13.2.3)} \\
&= \langle t, (f \circ \varrho(x))^\vee \rangle \quad \text{(Diff. \& Anal. Man., R, 13.2.3)}.
\end{align*}
$$
Chú ý rằng Định nghĩa 3 cũng có thể được viết dưới dạng đối xứng hơn
$$
\langle \varepsilon_x, t * f \rangle = \langle t^\vee * \varepsilon_x, f \rangle.
$$
Hàm $(g, x) \mapsto f(gx) = (f \circ \varrho(x))(g)$ trên $G \times X$ thuộc lớp C^r. Theo Differentiable and Analytic Manifolds, R, 13.4.4, hàm $x \mapsto \langle t^\vee, f \circ \varrho(x) \rangle$ do đó thuộc lớp $C^{r-s}$ nếu $s < \infty$. Nói cách khác, nếu $s < \infty$, $t * f$ thuộc lớp $C^{r-s}$.

Rõ ràng $t * f$ phụ thuộc tuyến tính vào $t$ và $f$.

Công thức (4) suy ra, đặc biệt, với $g \in G$,
$$
(\varepsilon_g * f)(x) = f(g^{-1}x)
$$
tức là
$$
\varepsilon_g * f = \gamma(g)f.
$$

Giả sử $K = \mathbf{R}$ hoặc $\mathbf{C}$, G và X đều hữu hạn chiều và X có một độ đo dương bất biến dưới G. Định nghĩa của $\varepsilon_g * f$ trùng với định nghĩa trong Integration, Chương VIII, § 4, no. 1 (xem công thức (2), loc. cit.).

#### Mệnh đề 17 {#lie-iii-s3-prop-17 .statement}

Cho $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(X)$ và $f : X \to F$ là một hàm lớp $C^r$ với $s + s' \leq r$. Khi đó
$$
\langle t', t * f \rangle = \langle t^\vee * t', f \rangle.
$$
$$
\begin{align*}
\langle t', t * f \rangle &= \langle t', x \mapsto \langle t, g \mapsto f(g^{-1}x) \rangle \rangle \quad \text{theo (4)} \\
&= \langle t \otimes t', (g, x) \mapsto f(g^{-1}x) \rangle \quad (\text{Diff. \& Anal. Man., R, 13.4.4}) \\
&= \langle t^\vee \otimes t', (g, x) \mapsto f(gx) \rangle \quad (\text{Diff. \& Anal. Man., R, 13.2.3}) \\
&= \langle t^\vee * t', f \rangle.
\end{align*}
$$

#### Mệnh đề 18 {#lie-iii-s3-prop-18 .statement}

Cho $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G)$ và $f : X \to F$ là một hàm lớp $C^r$, với $s + s' \leq r$. Khi đó
$$
(t * t') * f = t * (t' * f).
$$
Với mọi $x \in X$,
$$
\begin{align*}
\langle \varepsilon_x, (t * t') * f \rangle &= \langle ((t * t')^\vee * \varepsilon_x), f \rangle \quad \text{theo (5)} \\
&= \langle {t'}^\vee * (t^\vee * \varepsilon_x), f \rangle \quad (\text{Mệnh đề 2 và 7}) \\
&= \langle t^\vee * \varepsilon_x, t' * f \rangle \quad (\text{Mệnh đề 17}) \\
&= \langle \varepsilon_x, t * (t' * f) \rangle \quad (\text{Mệnh đề 17}).
\end{align*}
$$

Nếu $r \geq \infty$, ta thấy rằng tập hợp các hàm thuộc lớp $C^\infty$ trên $X$ với các giá trị trong $F$ là một môđun trái trên đại số $\mathcal{T}^{(\infty)}(G)$.

#### Mệnh đề 19 {#lie-iii-s3-prop-19 .statement}

Cho $t \in \mathcal{T}^{(s)}(G)$, với $s \leq r$. Cho $f$ (tương ứng $f'$) là một hàm thuộc lớp $C^r$ trên $X$ với các giá trị trong một không gian đa chuẩn Hausdorff $F$ (tương ứng $F'$). Cho $(u, u') \mapsto uu'$ là một ánh xạ song tuyến tính liên tục của $F \times F'$ vào một không gian đa chuẩn Hausdorff $F''$, sao cho $ff'$ là một hàm thuộc lớp $C^r$ trên $X$ với các giá trị trong $F''$. Cho
$$
\sum_{i=1}^n t_i \otimes t'_i \text{ là ảnh của } t \text{ trong } \mathcal{T}^{(s)}(G) \otimes \mathcal{T}^{(s)}(G) \text{ dưới đồng tích. Khi đó}
$$
$$
t * (ff') = \sum_{i=1}^n (t_i * f)(t'_i * f').
$$

Cho $x \in X$ và cho $\rho(x)$ ký hiệu ánh xạ quỹ đạo của $x$. Khi đó
$$
\langle \varepsilon_x, t * (ff') \rangle = \langle t^\vee, (ff') \circ \rho(x) \rangle \quad \text{theo (4)} \\
= \langle t^\vee, (f \circ \rho(x))(f' \circ \rho(x)) \rangle \\
= \sum_{i=1}^n \langle t_i^\vee, f \circ \rho(x) \rangle \langle t_{i'}^\vee, f' \circ \rho(x) \rangle \tag{Diff. \& Man. Anal., R, 13.5.2} \\
= \sum_{i=1}^n \langle \varepsilon_x, t_i * f \rangle \langle \varepsilon_x, t_i' * f' \rangle \quad \text{theo (4).}
$$

#### Nhận xét 1 {#lie-iii-s3-n4-rem-1 .statement}

Cho G là một nhóm Lie, X là một đa tạp thuộc lớp $C^r$ và $(x, g) \mapsto xg$ là một luật phép toán phải thuộc lớp $C^r$ của G trên X. Nếu $t \in \mathcal{T}^{(s)}(G)$ với $s \leq r$ và $f : X \to F$ là một hàm thuộc lớp $C^r$ trên X, ta ký hiệu bởi $f * t$ hàm trên X được xác định bởi
$$
\langle \varepsilon_x, f * t \rangle = \langle \varepsilon_x * t^\vee, f \rangle \\
= \langle \rho(x) * (t^\vee), f \rangle \\
= \langle t^\vee, f \circ \rho(x) \rangle \\
= \langle t, (f \circ \rho(x))^\vee \rangle.
$$
Đặc biệt
$$
(f * \varepsilon_g)(x) = f(xg^{-1})
$$
nghĩa là
$$
f * \varepsilon_g = \delta(g)^{-1} f.
$$
Các Mệnh đề 17, 18, 19 trở thành, với ký hiệu hiển nhiên,
$$
\langle t', f * t \rangle = \langle t' * t^\vee, f \rangle \tag{11}
$$
$$
f * (t * t') = (f * t) * t' \tag{12}
$$
$$
(ff') * t = \sum_{i=1}^n (f * t_i)(f' * t_i') \tag{13}
$$

#### Mệnh đề 20 {#lie-iii-s3-prop-20 .statement}

*Cho G, G' là các nhóm Lie, X là một đa tạp thuộc lớp $C^r$ và $(g, x) \mapsto gx$ (tương ứng $(x, g') \mapsto xg'$) là một luật phép toán trái (tương ứng phải) thuộc lớp $C^r$ của G (tương ứng G') trên X. Giả sử rằng $(gx)g' = g(xg')$ với mọi $x \in X, g \in G, g' \in G'$. Cho $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G')$ và $f : X \to F$ là một hàm thuộc lớp $C^r$ sao cho $s + s' \leq r$. Khi đó*
$$
(t * f) * t' = t * (f * t').
$$
Với mọi $x \in X$,
$$
\langle \varepsilon_x, (t * f) * t' \rangle = \langle \varepsilon_x * {t'}^\vee, t * f \rangle \quad \text{theo (8)} \\
= \langle t^\vee * (\varepsilon_x * {t'}^\vee), f \rangle \quad \text{(Mệnh đề 17)} \\
= \langle t^\vee * \varepsilon_x, f * t' \rangle \quad \text{(Mệnh đề 2 và (11))} \\
= \langle \varepsilon_x, t * (f * t') \rangle \quad \text{theo (5).}
$$

Đặc biệt, xét G như tác động lên chính nó bởi các phép tịnh tiến trái và phải. Nếu $f : G \to F$ là một hàm thuộc lớp $C^r$ trên G và $t \in \mathcal{T}^{(s)}(G)$ (với $s \leq r$), $t * f$ và $f * t$ là, nếu $s < \infty$, các hàm thuộc lớp $C^{r-s}$ trên G. Hơn nữa, cho $t' \in \mathcal{T}^{(s')}(G)$, với $s + s' \leq r$. Khi đó
$$
(t * f) * t' = t * (f * t').
$$
Đặc biệt, $\mathcal{C}^\infty(G)$ là một song môđun $(\mathcal{T}^{(\infty)}(G), \mathcal{T}^{(\infty)}(G))$. Các công thức (5) và (8) có các trường hợp đặc biệt là
$$
\langle t, f \rangle = \langle \varepsilon_e, t^\vee * f \rangle = \langle \varepsilon_e, f * t^\vee \rangle.
$$

#### Nhận xét 2 {#lie-iii-s3-n4-rem-2 .statement}

Cho $(g, x) \mapsto gx$ là một luật tác động trái của lớp $C^r$ của G trên X. Cho $t \in U_s(G)$ với $s \leq r$, $\Omega$ là một tập con mở của X và $f : \Omega \to F$ là một hàm thuộc lớp $C^r$. $t * f$ cũng có thể được xác định bởi công thức (4) hoặc (5); đó là một hàm xác định trên $\Omega$ với các giá trị trong F, thuộc lớp $C^{r-s}$ nếu $s < \infty$. Các kết quả của số này mở rộng theo một cách hiển nhiên cho tình huống này.

### 5. CÁC TRƯỜNG PHÂN BỐ ĐIỂM ĐƯỢC XÁC ĐỊNH BỞI TÁC ĐỘNG CỦA MỘT NHÓM TRÊN MỘT ĐA TẠP

Cho $(g, x) \mapsto \lambda(g, x) = gx$ là một luật tác động trái cấp $C^r$ của G trên X. Cho $s \leq r$ và $t \in U_s(G)$. Với mọi $x \in X$, $t * \varepsilon_x \in T^{(s)}_x(X)$. Ánh xạ $x \mapsto t * \varepsilon_x$ được gọi là trường các phân bố điểm xác định bởi t và tác động của G trên X và đôi khi được ký hiệu bởi $D_t^\lambda$ hoặc đơn giản là $D_t$. Cho $\Omega$ là một tập con mở của X và F là một không gian đa chuẩn Hausdorff. Nếu $f : \Omega \to F$ có lớp $C^r$ và $s \leq r$, hàm $t^\vee * f$ trên $\Omega$ cũng được ký hiệu là $D_t f$. Khi đó
$$
(D_t f)(x) = \langle t * \varepsilon_x, f \rangle.
$$
Nếu $s < \infty$, thì $D_t f \in \mathcal{C}^{r-s}(\Omega, F)$ theo no. 4. Do đó $f \mapsto D_t f$ là một ánh xạ từ $\mathcal{C}^r(\Omega, F)$ vào $\mathcal{C}^{r-s}(\Omega, F)$ (thường cũng được ký hiệu là $D_t$ bằng một sự lạm dụng ký hiệu).
Nếu $t \in U_s(G)$, $t' \in U_{s'}(G)$ và $s + s' \leq r$, thì, theo Mệnh đề 18 của no. 4,
$$
D_{t*t'} = D_{t'}(D_t f)
$$
và do đó, sử dụng sự lạm dụng ký hiệu đã chỉ ra ở trên,
$$
D_{t*t'} = D_{t'} \circ D_t.
$$
Giả sử rằng G và X là hữu hạn chiều. Ánh xạ $(t, x) \mapsto t \otimes \varepsilon_x$ từ $T^{(s)}(G) \times X$ vào bó vectơ $T^{(s)}(G \times X)$ (xem Differentiable and Analytic Manifolds, R, 13.2.5) có lớp $C^{r-s}$. Do đó (Differentiable and Analytic Manifolds, R, 13.2.5) ánh xạ $(t, x) \mapsto t * \varepsilon_x$ từ $T^{(s)}(G) \times X$ vào bó vectơ $T^{(s)}(X)$ có lớp $C^{r-s}$. Đặc biệt, $D_t$ là một toán tử vi phân cấp $\leq s$ và lớp $C^{r-s}$ theo nghĩa của Differentiable and Analytic Manifolds, R, 14.1.6. Theo công thức (16), hàm $D_t f$ khi đó là ảnh của $f$ qua toán tử vi phân này (Differentiable and Analytic Manifolds, R, 14.1.4).

Bây giờ ta không còn giả thiết rằng G và X là hữu hạn chiều nữa. Cho $\psi$ là một tự đẳng cấu của đa tạp X và $\Delta$ là một trường các phân bố điểm trên X. Phù hợp với các định nghĩa tổng quát, biến đổi của $\Delta$ dưới $\psi$ là trường các phân bố điểm trên X có giá trị tại $\psi(x)$ là $\psi_*(\Delta(x))$; ta ký hiệu ánh xạ này bởi $\psi(\Delta)$. Nếu $g \in G$ và $\tau(g)$ ký hiệu tự đẳng cấu $x \mapsto gx$ của X, thì biến đổi của $\Delta$ dưới $\tau(g)$ cũng được gọi là biến đổi của $\Delta$ dưới g.

#### Mệnh đề 21 {#lie-iii-s3-prop-21 .statement}

*Cho $\psi$ là một tự đẳng cấu của X giao hoán với các phép toán của G. Khi đó $D_t$ là bất biến dưới $\psi$.*

Với mọi $x \in X$,

$$
\begin{align*}
(\psi(D_t))(\psi(x)) &= \psi_*(D_t(x)) = \psi_*(t * \varepsilon_x) \\
&= t * \psi_*(\varepsilon_x) \tag{Proposition 15} \\
&= t * \varepsilon_{\psi(x)} = D_t(\psi(x)).
\end{align*}
$$

#### Mệnh đề 22 {#lie-iii-s3-prop-22 .statement}

*Nếu $g \in G$, biến đổi của $D_t$ theo g là $D_{\varepsilon_g * t * \varepsilon_g^{-1}}$.*

Giá trị của biến đổi này tại $gx$ là

$$
\begin{align*}
\tau(g)_*(D_t(x)) &= \tau(g)_*(t * \varepsilon_x) \\
&= \varepsilon_g * (t * \varepsilon_x) \quad \text{(Mệnh đề 14 (i))} \\
&= (\varepsilon_g * t * \varepsilon_g^{-1}) * \varepsilon_{gx} \quad \text{(Mệnh đề 1 và 2)} \\
&= D_{\varepsilon_g * t * \varepsilon_g^{-1}}(gx).
\end{align*}
$$

Cho $(x, g) \mapsto \mu(x, g) = xg$ là một luật phép toán phải thuộc lớp $C'$ của G trên X. Cho $s \leq r$ và $t \in U_s(G)$. Với mọi $x \in X$, $\varepsilon_x * t \in T^{(s)}_x(X)$. Ánh xạ $x \mapsto \varepsilon_x * t$ được gọi là trường các phân phối xác định bởi t và tác động của G trên X và đôi khi được ký hiệu bởi $D_t^u$ hoặc đơn giản là $D_t$. Cho $\Omega$ là một tập con mở của X. Nếu $f : \Omega \to F$ thuộc lớp $C'$, hàm $f * t^\vee$ được ký hiệu bởi $D_t f$. Khi đó

$$(19)$$
$$(D_t f)(x) = \langle \varepsilon_x * t, f \rangle$$

và, theo ký hiệu hiển nhiên,

$$(20)$$
$$D_{t * t'} f = D_t(D_{t'} f)$$

$$(21)$$
$$D_{t * t'} = D_t \circ D_{t'}.$$

Mệnh đề 21 vẫn đúng. Cho $g \in G$. Biến đổi của $D_t$ theo g (nghĩa là theo tự đẳng cấu $x \mapsto xg$ của X) là $D_{\varepsilon_g^{-1} * t * \varepsilon_g}$.

### 6. CÁC TRƯỜNG BẤT BIẾN CỦA CÁC PHÂN PHỐI ĐIỂM TRÊN MỘT NHÓM LIE

#### Định nghĩa 4 {#lie-iii-s3-def-4 .statement}

*Một nhóm Lie G. Một trường các phân phối trên G được gọi là bất biến trái (tương ứng phải) nếu nó bất biến qua các phép tịnh tiến trái (tương ứng phải) của G.*

Nói cách khác, một trường các phân phối $g \mapsto \Delta_g$ trên $G$ là bất biến trái nếu
$$
\Delta_{gg'} = \gamma(g) * \beta_{g'}
$$
với $g, g'$ trong $G$,
hoặc cũng vậy nếu
$$
\Delta_{gg'} = \varepsilon_g * \Delta_{g'}
$$
với $g, g'$ trong $G$.
Nó là bất biến phải nếu
$$
\Delta_{gg'} = \delta({g'}^{-1}) * \Delta_g
$$
với $g, g'$ trong $G$,
hoặc cũng vậy nếu:
$$
\Delta_{gg'} = \Delta_g * \varepsilon_g,
$$
với $g, g'$ trong $G$.

#### Định nghĩa 5 {#lie-iii-s3-def-5 .statement}

*Cho $G$ là một nhóm Lie và $t \in U(G)$. Gọi $L_t$ là trường các phân phối $g \mapsto \varepsilon_g * t$ trên $G$ và $R_t$ là trường các phân phối $g \mapsto t * \varepsilon_g$ trên $G$.*

Nói cách khác, $L_t$ (tương ứng $R_t$) là trường các phân phối được xác định bởi $t$ và $G$ tác động lên $G$ ở bên phải (tương ứng bên trái) nhờ ánh xạ $(g, g') \mapsto gg'$. Cho $\Omega$ là một tập con mở của $G$ và $F$ là một không gian đa chuẩn Hausdorff; nếu $f \in C^\omega(\Omega, F)$, thì $L_t f = f * t^\vee \in C^\omega(\Omega, F)$ và
$$
R_t f = t^\vee * f \in C^\omega(\Omega, F)
$$
(no. 5). Nếu $G$ là hữu hạn chiều, các toán tử vi phân $L_t$ và $R_t$ thuộc lớp $C^\omega$ (no. 5).

#### Mệnh đề 23 {#lie-iii-s3-prop-23 .statement}

(i) *Ánh xạ $t \mapsto L_t$ (tương ứng $t \mapsto R_t$) là một đẳng cấu của không gian vectơ $U(G)$ lên trường vectơ các phân phối bất biến trái (tương ứng phải) trên $G$.*
(ii) *Đối với $t, t'$ trong $U(G)$, $L_{t*t'} = L_t \circ L_{t'}$, $R_{t*t'} = R_{t'} \circ R_t$, $L_t \circ R_{t'} = R_{t'} \circ L_t$ (với sự lạm dụng ký hiệu ở no. 5).*
(iii) *Nếu $\theta$ là ánh xạ $g \mapsto g^{-1}$ của $G$ lên $G$, thì $\theta(L_t) = R_{t^\vee}$.*
(iv) *Nếu $t \in U(G)$ và $g \in G$, thì $(L_t)_g = (R_{\varepsilon_g * t * \varepsilon_g^{-1}})_g$.*

Trong $G$ mọi phép tịnh tiến phải giao hoán với mọi phép tịnh tiến trái. Theo Mệnh đề 21 của no. 5, $L_t$ do đó là bất biến trái. Vì $(L_t)_e = t$, ánh xạ $t \mapsto L_t$ là đơn ánh. Cho $\Delta$ là một trường các phân bố bất biến trái trên $G$; đặt $t = \Delta_e$; khi đó $\Delta$ và $L_t$ có cùng giá trị tại $e$ và đều bất biến trái, do đó $\Delta = L_t$. Điều này chứng minh (i) đối với $L_t$ và lập luận tương tự đối với $R_t$. Các công thức $L_{t*t'} = L_t \circ L_{t'}$, $R_{t*t'} = R_{t'} \circ R_t$ suy ra từ (21) và (18). Cho $t \in U_s(G)$, $t' \in U_{s'}(G)$, $f \in C^r(\Omega, F)$, trong đó $\Omega$ là mở trong $G$ và $s + s' \leq r$; khi đó
$$
\begin{align*}
L_t R_{t'} f &= L_t ({t'}^\vee * f) = ({t'}^\vee * f) * t \\
&= {t'}^\vee * (f * t^\vee) \tag{Proposition 20} \\
&= R_{t'} L_t f
\end{align*}
$$
và do đó $L_t \circ R_{t'} = R_{t'} \circ L_t$. Vì $\theta$ là một đẳng cấu của $G$ lên $G^\vee$, $\theta(L_t)$ là một trường các phân bố bất biến phải trên $G$; giá trị của nó tại $e$ là $\theta(t) = t^\vee$; do đó $\theta(L_t) = R_{t^\vee}$. Cuối cùng,
$$
(L_t)_g = \varepsilon_g * t = (\varepsilon_g * t * \varepsilon_g^{-1}) * \varepsilon_g = (R_{\varepsilon_g * t * \varepsilon_g^{-1}})_g.
$$

#### Nhận xét 1 {#lie-iii-s3-n6-rem-1 .statement}

Chính tác động của G lên chính nó bởi phép tịnh tiến phải xác định các trường các phân bố bất biến trái.

#### Nhận xét 2 {#lie-iii-s3-n6-rem-2 .statement}

Giả sử rằng G là hữu hạn chiều. Ánh xạ

$$(t, g) \mapsto (\mathbf{R}_t)_g = t * \varepsilon_g$$

từ $U_s(G) \times G$ vào $T^{(s)}(G)$ là một đẳng cấu của các bó vectơ giải tích; vì ánh xạ này là song ánh, tuyến tính trên mỗi thớ và giải tích (no. 5); mặt khác, cho $\phi : T^{(s)}(G) \to U_s(G) \times G$ là song ánh ngược; nếu $t \in T^{(s)}_g(G)$, thì $\phi(t) = (t * \varepsilon_{g^{-1}}, g)$ và do đó $\phi$ là giải tích. Đẳng cấu $\phi$ được gọi là phép tầm thường hóa phải của $T^{(s)}(G)$. Tương tự, xét ánh xạ $(t, g) \mapsto (\mathbf{L}_t)_g = \varepsilon_g * t$ từ $U_g(G) \times G$ vào $T^{(s)}(G)$; đẳng cấu nghịch đảo được gọi là phép tầm thường hóa trái của $T^{(s)}(G)$. Bằng hạn chế ta thu được các phép tầm thường hóa phải và trái của $T(G)$ (§ 2, no. 2).

### 7. ĐẠI SỐ LIE CỦA MỘT NHÓM LIE

Cho G là một nhóm Lie. Trong $U(G)$, cũng như trong mọi đại số kết hợp, ta viết $[t, t'] = t * t' - t' * t$. Vì $T_e(G)$ là tập hợp các phần tử nguyên thủy của $U(G)$, $[T_e(G), T_e(G)] \subset T_e(G)$ (Chương II, § 1, no. 2, Mệnh đề 4). Hạn chế của móc Lie trên $T_e(G)$ do đó xác định trên $T_e(G)$ một cấu trúc đại số Lie.

#### Bổ đề 1 {#lie-iii-s3-lem-1 .statement}

Cho X và $X'$ là các không gian khả chuẩn đầy đủ, $X_0$ là một lân cận mở của 0 trong X và f là một ánh xạ giải tích của $X_0$ vào $X'$ sao cho $f(0) = 0$. Cho $f = f_1 + f_2 + f_3 + \cdots$ là khai triển của f dưới dạng một chuỗi nguyên quanh 0, trong đó $f_i$ là một đa thức liên tục thuần nhất bậc i trên X nhận giá trị trong $X'$. Cho t là một phần tử của TS$^2(X)$, được xét như một phân bố điểm trên X có giá đỡ được chứa trong \{0\}. Cho $t' = f_*(t) \in TS(X')$. Thành phần thuần nhất bậc 1 của $t'$ là $\langle f_2, t \rangle$.

Cho $t'_1$ là thành phần này. Khi đó, với mọi ánh xạ tuyến tính liên tục u từ $X'$ vào một không gian đa chuẩn,

$$
u(t'_1) = \langle t', u \rangle \quad \text{vì } u \text{ liên tục và tuyến tính}
$$
$$
= \langle t, u \circ f \rangle \quad (\text{Diff. \& Anal. Man., R, 13.2.3})
$$
$$
= \langle t, u \circ f_2 \rangle \quad \text{vì } t \in TS^2(X)
$$
$$
= u(\langle t, f_2 \rangle) \quad (\text{Diff. \& Anal. Man., R, 13.2.2}),
$$

suy ra bổ đề.

#### Mệnh đề 24 {#lie-iii-s3-prop-24 .statement}

Cho G là một nhóm Lie và $(U, \phi, E)$ là một biểu đồ trên G sao cho $\phi(e) = 0$. Cho V là một lân cận mở của e sao cho $V^2 \subset U$. Cho m là ánh xạ giải tích $(a, b) \mapsto \phi(\phi^{-1}(a)\phi^{-1}(b))$ từ $\phi(V) \times \phi(V)$ vào E. Cho

$$
m = \sum_{i, j \geq 0} m_{i, j}
$$

là khai triển của m dưới dạng một chuỗi nguyên quanh (0, 0), trong đó $m_{i,j}$ là một đa thức liên tục song thuần nhất bậc $(i, j)$ trên $E \times E$ với giá trị trong E.

(i) $m_{i,0} = m_{0,j} = 0$ đối với mọi $i \neq 1$ và $j \neq 1$.
(ii) $m_{1,0}(a, b) = a$ và $m_{0,1}(a, b) = b$ với mọi $a \in E, b \in E$.
(iii) *Cho $\psi : T_e(G) \to E$ là vi phân của $\phi$ tại e. Với mọi $u, v$ trong $T_e(G)$,*

$$
\psi([u, v]) = m_{1,1}(\psi(u), \psi(v)) - m_{1,1}(\psi(v), \psi(u)).
$$

$m(a, 0) = a,\ m(0, b) = b$ với mọi $a, b$ trong $\phi(V)$, điều đó chứng minh (i) và (ii).
Cho $u, v$ trong $T_e(G)$. Đồng nhất $T_0(E)$ với $E$ và do đó $\psi$ với $T_e(\phi)$:
Ảnh của $u$ và $v$ qua $T_e(\phi)$ là $\psi(u)$ và $\psi(v)$. Phân bố điểm tích tenxơ của các ảnh này là tích đối xứng của $(\psi(u), 0)$ và $(0, \psi(v))$ trong $TS(E \times E) = TS(E) \times TS(E)$, nghĩa là

$$
(\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0).
$$

Do đó $\phi * (u * v)$ là ảnh của phần tử trên qua ánh xạ $m$ từ $\phi(V) \times \phi(V)$ vào $E$. Thành phần bậc 1 của nó trong $TS(E)$ là, theo Bổ đề 1,

$$
x = \langle m_{1,1}, (\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0) \rangle.
$$

Ta định nghĩa một ánh xạ song tuyến tính $n : (E \times E)^2 \to E$ bởi

$$
n((a, b), (a', b')) = m_{1,1}(a, b').
$$

Khi đó $n((a, b), (a, b)) = m_{1,1}(a, b)$ và do đó

$$
x = \langle n, (\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0) \rangle \\
= m_{1,1}(\psi(u), \psi(v)) + m_{1,1}(0, 0) = m_{1,1}(\psi(u), \psi(v)).
$$

Tương tự, $\phi * (v * u)$ nhận $m_{1,1}(\phi(v), \phi(u))$ làm thành phần bậc 1 trong $TS(E)$. Vì $\phi([u, v])$ có bậc 1, điều này chứng minh (iii).

#### Hệ quả {#lie-iii-s3-n7-cor-1 .statement}

*Không gian chuẩn hóa $T_e(G)$ cùng với móc Lie là một đại số Lie chuẩn hóa.*

#### Định nghĩa 6 {#lie-iii-s3-def-6 .statement}

*Không gian chuẩn hóa $T_e(G)$, cùng với móc Lie, được gọi là đại số Lie chuẩn hóa của G, hoặc đơn giản là đại số Lie của G, và được ký hiệu bởi $L(G)$.*

#### Mệnh đề 25 {#lie-iii-s3-prop-25 .statement}

*Cho G là một nhóm Lie và $E(G)$ là đại số bao quanh của $L(G)$. Đơn ánh chính tắc của $L(G)$ vào $E(G)$ xác định một đồng cấu $\theta$ của đại số $E(G)$ vào đại số $U(G)$. Nếu K có đặc số 0, $\eta$ là một đẳng cấu đại số kép.*

Đại số kép $U(G)$ là giao hoán tử ( *Differentiable and Analytic Manifolds*, R, 13.5.1) và lọc $(U_s(G))$ tương thích với cấu trúc đại số kép. Tập hợp các phần tử nguyên thủy của $U(G)$ là $L(G)$. Khi đó chỉ cần áp dụng chương II, § 1, no. 6, Định lý 1.

Khi K có đặc số 0, từ nay ta sẽ đồng nhất $U(G)$ với đại số bao quanh của $L(G)$. Theo (2) và Mệnh đề 7 (ii), ánh xạ $t \mapsto t^\vee$ của $U(G)$ vào $U(G)$ khi đó được đồng nhất với phản tự đồng cấu chính của $U(G)$ (Chương I, § 2, no. 4).

#### Mệnh đề 26 {#lie-iii-s3-prop-26 .statement}

*Giả sử K có đặc số $p > 0$. Với mọi $a \in L(G)$, $a^p \in L(G)$ và $\operatorname{ad}(a^p) = (\operatorname{ad} a)^p$ (lũy thừa $a^p$ được tính trong $U(G)$).*

Nếu $a \in L(G)$, $a$ là nguyên thủy trong $U(G)$, do đó $a^p$ là nguyên thủy trong $U(G)$ (Chương II, § 1, no. 2, *Nhận xét 1*) và do đó $a^p \in L(G)$. Gọi $\sigma_a$ (tương ứng $\tau_a$) là ánh xạ tuyến tính $x \mapsto a * x$ (tương ứng $x \mapsto x * a$) của $U(G)$ vào $U(G)$. Với mọi $x \in U(G)$, $(\operatorname{ad} a)(x) = (\sigma_a - \tau_a)(x)$ và do đó $(\operatorname{ad} a)^p = (\sigma_a - \tau_a)^p$. Nhưng $\sigma_a$ và $\tau_a$ giao hoán và do đó $(\sigma_a - \tau_a)^p = (\sigma_a)^p - (\tau_a)^p = \tau_a^p - \sigma_a^p$, do đó là mệnh đề thứ hai.

#### Định nghĩa 7 {#lie-iii-s3-def-7 .statement}

*Cho X là một đa tạp lớp $C^r$ ($r \geq 2$) và $g$ là một đại số Lie chuẩn hóa được đầy đủ. Một luật phép toán vi phân trái (tương ứng phải) lớp $C^{r-1}$ của $g$ trên X là một ánh xạ $a \mapsto D_a$ của $g$ vào tập hợp các trường vectơ trên X với các tính chất sau:*

(a) *ánh xạ $(a, x) \mapsto D_a(x)$ là một cấu xạ lớp $C^{r-1}$ của bó vectơ tầm thường $g \times X$ vào bó vectơ $T(X)$;*

(b) $[D_a, D_b] = -D_{[a, b]}$ (tương ứng $[D_a, D_b] = D_{[a, b]}$ với mọi $a, b$ trong $g$).

Đặc biệt, mỗi trường vectơ $D_a$ là lớp $C^{r-1}$.

#### Nhận xét {#lie-iii-s3-n7-rem-1 .statement}

Cho X là một đa tạp lớp $C^r$, $g$ là một đại số Lie hữu hạn chiều và $a \mapsto D_a$ là một ánh xạ tuyến tính của $g$ vào không gian vectơ các trường vectơ lớp $C^{r-1}$ trên X. Khi đó điều kiện (a) của Định nghĩa 7 được thỏa mãn. Thật vậy, bằng cách xét một cơ sở của $g$ và áp dụng *Differentiable and Analytic Manifolds*, R, 7.7.1, bài toán được quy về trường hợp $\dim g = 1$ và mệnh đề của ta khi đó là hiển nhiên.

#### Mệnh đề 27 {#lie-iii-s3-prop-27 .statement}

*Cho G là một nhóm Lie và X là một đa tạp lớp $C^r$. Giả sử đã cho một luật phép toán trái (tương ứng phải) lớp $C^r$ của G trên X. Với mọi $a \in L(G)$, gọi $D_a$ là trường phân bố điểm được xác định bởi a trên X.*

(i) *Ánh xạ $(a, x) \mapsto D_a(x)$ là một cấu xạ lớp $C^{r-1}$ của bó vectơ tầm thường $L(G) \times X$ vào bó vectơ $T(X)$.*

(ii) *Cho I là một tập con mở của K chứa 0 và $\gamma : I \to G$ là một ánh xạ lớp $C^r$ sao cho $\gamma(0) = e$. Cho $a = T_0(\gamma)1 \in L(G)$. Nếu f là một hàm lớp $C^r$ trên một tập con mở của X, thì*
$$
(D_a f)(x) = \lim_{k \in \mathbf{K}^*, k \to 0} k^{-1}(f(\gamma(k)x) - f(x)) \quad \text{nếu G phép toán trái,}
$$
$$
(D_a f)(x) = \lim_{k \in \mathbf{K}^*, k \to 0} k^{-1}(f(x\gamma(k)) - f(x)) \quad \text{nếu G phép toán phải.}
$$

(iii) *Nếu $r \geq 2$, ánh xạ $a \mapsto D_a$ là một luật phép toán vi phân trái (tương ứng phải) lớp $C^{r-1}$ của $L(G)$ trên X.*

Giả sử rằng G tác động lên X ở bên trái. Gọi $\phi : G \times X \to X$ là luật phép toán. Khi đó $T(\phi)$ là một $\phi$-cấu xạ lớp $C^{r-1}$ của bó vectơ $T(G) \times T(X)$ vào bó vectơ $T(X)$ (*Differentiable and Analytic*

Manifolds, R, 8.1.2). Bó vectơ cảm sinh $(\mathrm{T}(G) \times \mathrm{T}(X))|_{\{\epsilon\} \times X}$ được đồng nhất với $E = L(G) \times T(X)$. Do đó $T(\phi)|E$ là một cấu xạ bó vectơ lớp $C^{r-1}$. Với $(a, x) \in L(G) \times X, T(\phi)(a, x) = D_a(x)$, do đó (i).

Công thức cho $(D_a f)(x)$ suy ra từ § 2, cuối của no. 2, và *Differentiable and Analytic Manifolds*, R, 8.4.5.

Giả sử $r \geqslant 2$. Cho $a, b$ thuộc $L(G)$ và $f$ là một hàm thuộc lớp $C^r$ trên một tập con mở của $X$. Khi đó
$$
\begin{align*}
D_{[a, b]}f &= D_b(D_a f) - D_a(D_b f) \quad \text{theo (17)} \\
&= [D_b, D_a]f \tag{Diff. \& Anal. Man., R, 8.5.3}.
\end{align*}
$$
Cho $x \in X$. Lấy $f$ là một biểu đồ trên một lân cận mở của $x$, suy ra rằng $D_{[a, b]}(x) = [D_b, D_a](x)$, do đó (iii). Lập luận tương tự nếu $G$ tác động lên $X$ bên phải.

Khi $r \geqslant 2$, ánh xạ $a \mapsto D_a$ được gọi là luật phép toán vô cùng bé liên kết với luật phép toán đã cho.

### 8. CÁC TÍNH CHẤT HÀM TỬ CỦA ĐẠI SỐ LIE

Cho $G$ và $H$ là các nhóm Lie và $\phi$ là một cấu xạ từ $G$ vào $H$. Hạn chế của $U(\phi)$ lên $L(G)$, chính là $T_e(\phi)$, là một cấu xạ liên tục của $L(G)$ vào $L(H)$, mà ta ký hiệu là $L(\phi)$. Nếu $\psi$ là một cấu xạ từ $H$ vào một nhóm Lie, thì $L(\psi \circ \phi) = L(\psi) \circ L(\phi)$.

Để $\phi$ là một phép nhúng, điều kiện cần và đủ là $L(\phi)$ là một đẳng cấu của $L(G)$ lên một đại số con của $L(H)$ có một phần bù tôpô. Đặc biệt, nếu $G$ là một nhóm con Lie của $H$ và $\phi$ là đơn ánh chính tắc, thì $L(G)$ được đồng nhất với một đại số con Lie của $L(H)$ bằng $L(\phi)$. Cụ thể hơn nữa, nếu $G$ là một nhóm con mở của $H$, thì $L(G) = L(H)$.

Nếu $G$ là một nhóm con giả Lie của $H$, thì $L(G)$ cũng được đồng nhất với một nhóm con Lie đóng của $L(H)$.

Để $\phi$ là một phép xạ xuống, điều kiện cần và đủ là $L(\phi)$ toàn ánh và hạt nhân của nó có một phần bù tôpô. Trong trường hợp đó, hạt nhân $N$ của $\phi$ là một nhóm con Lie của $G$ và $L(N) = \operatorname{Ker} L(\phi)$. Đặc biệt, nếu $H$ là nhóm Lie thương của $G$ theo một nhóm con Lie chuẩn tắc $P$, thì $L(P)$ là một iđêan của $L(G)$ và, nếu $\phi$ là toàn cấu chính tắc của $G$ lên $H$, thì $L(G/P)$ được đồng nhất với $L(G)/L(P)$ nhờ cấu xạ suy ra từ $L(\phi)$ khi chuyển qua thương.

Cho $I$ là một tập hữu hạn, $(G_i)_{i \in I}$ là một họ các nhóm Lie, $G$ là tích của chúng và $p_i$ là cấu xạ chính tắc của $G$ lên $G_i$. Khi đó $(L(p_i))_{i \in I}$ là một cấu xạ của đại số Lie $L(G)$ vào đại số Lie $\prod_{i \in I} L(G_i)$ và là một đẳng cấu của các không gian chuẩn hóa. Vì thế $L(G)$ được đồng nhất với $\prod_{i \in I} L(G_i)$ nhờ $(L(p_i))_{i \in I}$.

#### Mệnh đề 28 {#lie-iii-s3-prop-28 .statement}

Cho $G$ và $H$ là các nhóm Lie và $\phi$ là một cấu xạ của $G$ vào $H$. Giả sử $K$ có đặc số $0$ và $H$ là hữu hạn chiều.

(i) Hạt nhân $N$ của $\phi$ là một nhóm con Lie của $G$ và $L(N) = Ker L(\phi)$.

(ii) Cấu xạ $\psi$ của $G/N$ vào $H$ suy ra từ $\phi$ khi chuyển qua thương là một phép nhúng.

(iii) Nếu $\phi(G)$ đóng trong $H$ và tôpô của $G$ có một cơ sở đếm được, thì $\phi(G)$ là một nhóm con Lie của $H$, $\psi$ là một đẳng cấu của nhóm Lie $G/N$ lên nhóm Lie $\phi(G)$ và $L(\phi(G)) = Im L(\phi)$.

Cho $G$ tác động lên $H$ bên trái bởi ánh xạ $(g, h) \mapsto \phi(g)h$. Chỉ cần áp dụng Mệnh đề 14 của § 1, no. 7, cho quỹ đạo của $e$.

#### Mệnh đề 29 {#lie-iii-s3-prop-29 .statement}

Cho $G$ và $H$ là các nhóm Lie và $\phi$ là một cấu xạ của $G$ vào $H$. Giả sử $K$ có đặc số $0$ và $H$ là hữu hạn chiều. Nếu $H'$ là một nhóm con Lie của $H$, thì $G' = \phi^{-1}(H')$ là một nhóm con Lie của $G$ và $L(G') = L(\phi)^{-1}(L(H'))$.

Cho $\pi$ là ánh xạ chính tắc của $H$ vào không gian thuần nhất $X = H/H'$. Cho $G$ tác động lên $X$ bên trái bởi ánh xạ $(g, x) \mapsto \phi(g)x$. Nhóm ổn định của $\pi(e)$ là $G'$, do đó là một nhóm con Lie của $G$ (§ 1, no. 7, Mệnh đề 14). Ánh xạ quỹ đạo của $\pi(e)$ là $\pi \circ \phi$. Theo Mệnh đề 14 của § 1, $L(G')$ là hạt nhân của $L(\pi \circ \phi) = T_e(\pi) \circ L(\phi)$. Hạt nhân của $T_e(\pi)$ là $L(H')$ (§ 1, no. 6, Mệnh đề 11 (i)) và do đó $Ker L(\pi \circ \phi) = L(\phi)^{-1}(L(H'))$.

#### Hệ quả 1 {#lie-iii-s3-prop-29-cor-1 .statement}

Cho $G$, $H$ là các nhóm Lie và $\phi_1$ và $\phi_2$ là các cấu xạ của $G$ vào $H$. Giả sử $K$ có đặc số $0$ và $H$ là hữu hạn chiều. Tập hợp các $g \in G$ sao cho $\phi_1(g) = \phi_2(g)$ là một nhóm con Lie $G'$ của $G$ và $L(G')$ là tập hợp các $x \in L(G)$ sao cho $L(\phi_1)x = L(\phi_2)x$.

Ta viết $\phi(g) = (\phi_1(g), \phi_2(g))$ với mọi $g \in G$, sao cho $\phi$ là một cấu xạ của $G$ vào $H \times H$. Cho $\Delta$ là nhóm con đường chéo của $H \times H$. Khi đó $G' = \phi^{-1}(\Delta)$ và $L(\phi)x = (L(\phi_1)x, L(\phi_2)x)$ với mọi $x \in L(G)$. Lúc này chỉ cần áp dụng Mệnh đề 29.

#### Hệ quả 2 {#lie-iii-s3-prop-29-cor-2 .statement}

Cho $G$ là một nhóm Lie hữu hạn chiều và $G_1$ và $G_2$ là hai nhóm con Lie của $G$. Giả sử $K$ có đặc số $0$. Khi đó $G_1 \cap G_2$ là một nhóm con Lie của $G$ với đại số Lie $L(G_1) \cap L(G_2)$.

Ta áp dụng Mệnh đề 29 cho đơn ánh chính tắc của $G_1$ vào $G$ và nhóm con $G_2$.

#### Hệ quả 3 {#lie-iii-s3-prop-29-cor-3 .statement}

Cho $G$, $G'$, $H$ là các nhóm Lie và $\phi : G \to H$ và $\phi' : G' \to H$ là các cấu xạ nhóm Lie. Giả sử $K$ có đặc số $0$ và $H$ là hữu hạn chiều. Cho $F$ là tập hợp các $(g, g') \in G \times G'$ sao cho $\phi(g) = \phi'(g')$. Khi đó $F$ là một nhóm con Lie của $G \times G'$ và $L(F)$ là tập hợp các $(x, x') \in L(G) \times L(G')$ sao cho $L(\phi)x = L(\phi')x'$.

Ta áp dụng Hệ quả 1 cho các cấu xạ $(g, g') \mapsto \phi(g)$ và $(g, g') \mapsto \phi'(g')$ của $G \times G'$ vào $H$.

#### Mệnh đề 30 {#lie-iii-s3-prop-30 .statement}

Cho $G$ là một nhóm Lie hữu hạn chiều với một cơ sở đếm được và

$H$ và $H'$ là các nhóm con Lie của $G$. Giả sử $K$ có đặc số $0$ và $HH'$ là đóng địa phương trong $G$.

(i) $HH'$ là một đa tạp con của $G$ và $T_e(HH') = L(H) + L(H')$.

(ii) Giả sử mọi phần tử của $H$ giao hoán với mọi phần tử của $H'$. Khi đó $HH'$ là một nhóm con Lie của $G$. Cho $\phi$ là ánh xạ $(h, h') \mapsto hh'$ của $H \times H'$ lên $HH'$. Hạt nhân của $\phi$ là tập hợp các $(m, m^{-1})$ với $m \in H \cap H'$ và cấu xạ của $(H \times H')/\mathrm{Ker}\ \phi$ lên $HH'$ suy ra từ $\phi$ khi chuyển qua thương là một đẳng cấu nhóm Lie.

Cho $H \times H'$ tác động lên $G$ bên phải bởi ánh xạ $((h, h'), g) \mapsto hg{h'}^{-1}$. Ánh xạ quỹ đạo $\rho$ của $e$ là $(h, h') \mapsto h{h'}^{-1}$. Theo Mệnh đề 14 (iii) của § 1, no. 7, $HH'$ là một đa tạp con của $G$ và $T_e(HH') = \mathrm{Im}\ T_e(\rho)$. Khi đó

$$
T_e(\rho)(L(H) \times \{0\}) = L(H) \quad \text{và} \quad T_e(\rho)(\{0\} \times L(H')) = L(H')
$$

và do đó $T_e(HH') = L(H) + L(H')$. Giả sử mọi phần tử của $H$ giao hoán với mọi phần tử của $H'$. Khi đó $HH'$ là một nhóm con của $G$. Theo (i), nó là một nhóm con Lie của $G$. Phần còn lại của mệnh đề suy ra từ Mệnh đề 28.

#### Mệnh đề 31 {#lie-iii-s3-prop-31 .statement}

Cho $G$ là một nhóm Lie hữu hạn chiều với cơ sở đếm được, $H$ là một nhóm con Lie chuẩn tắc của $G$ và $A$ là một nhóm con Lie của $G$. Giả sử $K$ có đặc số $0$ và $AH$ đóng. Cho $\phi$ là cấu xạ chính tắc của $G$ lên $G/H$. Khi đó các ánh xạ chính tắc

$$
A/(H \cap A) \to \phi(A), \qquad AH/H \to \phi(A)
$$

là các đẳng cấu nhóm Lie.

Theo Mệnh đề 30, $AH$ là một nhóm con Lie của $G$. Theo Hệ quả 2 của Mệnh đề 29, $H \cap A$ là một nhóm con Lie của $G$. Do đó có thể nói về các nhóm $AH/H$ và $A/(H \cap A)$. Mặt khác, $\phi(A)$, là ảnh chính tắc của $AH$ trong $G/H$, là đóng và do đó là một nhóm con Lie của $G/H$ (Mệnh đề 28 (iii)). Áp dụng Mệnh đề 28 cho các cấu xạ hợp thành $A \to G \to G/H$ và $AH \to G \to G/H$, cho thấy rằng các ánh xạ chính tắc của mệnh đề là các đẳng cấu nhóm Lie.

#### Mệnh đề 32 {#lie-iii-s3-prop-32 .statement}

Cho G và H là các nhóm Lie, k là một trường con đóng không rời rạc của K và $\phi$ là một cấu xạ của G vào H đối với các cấu trúc nhóm Lie trên k. Giả sử rằng K có đặc số 0. Nếu $L(\phi)$ là K-tuyến tính, thì $\phi$ là một cấu xạ đối với các cấu trúc nhóm Lie trên K.

Với mọi $g \in G$,

$$
T_g(\phi) = T_e(\gamma(\phi(g))) \circ L(\phi) \circ T_g(\gamma(g)^{-1})
$$

và do đó $T_g(\phi)$ là K-tuyến tính. Mệnh đề suy ra từ Đa tạp khả vi và giải tích, R, 5.14.6.

### 9. ĐẠI SỐ LIE CỦA NHÓM CÁC PHẦN TỬ KHẢ NGHỊCH CỦA MỘT ĐẠI SỐ

Cho $A$ là một đại số kết hợp đầy đủ chuẩn được với phần tử đơn vị $e$. Cho $A^*$ là nhóm các phần tử khả nghịch của $A$. Ta đã thấy (§ 1, no. 1) rằng $A^*$ là một đa tạp con mở của $A$ và là một nhóm Lie. Cho $G$ là một nhóm Lie và $f$ là một cấu xạ của nhóm Lie $G$ vào nhóm Lie $A^*$. Có thể xem $f$ như một ánh xạ giải tích của $G$ vào không gian đầy đủ chuẩn được $A$. Do đó, nếu $t \in \mathcal{T}^{(\infty)}(G)$, ta có thể lập $\langle t, f \rangle$, là một phần tử của $A$.

#### Mệnh đề 33 {#lie-iii-s3-prop-33 .statement}

*Ánh xạ $t \mapsto \langle t, f \rangle$ là một cấu xạ của đại số $\mathcal{T}^{(\infty)}(G)$ vào đại số $A$.*

Chỉ cần kiểm tra rằng, nếu $t$ và $t'$ là các phân phối điểm trên $G$, thì $\langle t * t', f \rangle = \langle t, f \rangle \langle t', f \rangle$. Nhưng
$$
\begin{align*}
\langle t * t', f \rangle &= \langle t \otimes t', (g, g') \mapsto f(gg') \rangle \\
&= \langle t \otimes t', (g, g') \mapsto f(g)f(g') \rangle \\
&= \langle t, f \rangle \langle t', f \rangle
\end{align*}
$$
*(Đa tạp khả vi và giải tích, R, 13.4.3)*.

Cấu xạ của Mệnh đề 33 được gọi là *liên kết* với $f$.

Lấy $G$ là chính nhóm $A^*$ và lấy $f$ là ánh xạ đồng nhất $i$ của $A^*$. Ta thu được một cấu xạ, được gọi là *chính tắc*, của đại số $\mathcal{T}^{(\infty)}(A^*)$ vào đại số $A$. Không gian tiếp xúc $T_e(A^*)$ được đồng nhất một cách chính tắc với $A$; và nếu $t \in T_e(A^*)$, thì định nghĩa của phép đồng nhất này được chọn sao cho $\langle t, i \rangle = t$. Khi đó Mệnh đề 33 suy ra hệ quả sau:

#### Hệ quả {#lie-iii-s3-n9-cor-1 .statement}

*Ánh xạ chính tắc $\zeta$ của $L(A^*)$ vào $A$ là một đẳng cấu của đại số Lie, từ $L(A^*)$ lên đại số Lie $A$. Nói cách khác,
$$
\zeta([a, b]) = \zeta(a)\zeta(b) - \zeta(b)\zeta(a)
$$
với mọi $a, b$ trong $L(A^*)$. Nếu $K$ có đặc số $p > 0$, thì $\zeta(a^p) = \zeta(a)^p$ với mọi $a \in L(A^*)$.*

Kể từ đây $L(A^*)$ và $A$ được đồng nhất thông qua đẳng cấu $\zeta$.

Cấu xạ chính tắc của $\mathcal{T}^{(\infty)}(A^*)$ vào $A$ đã thu được như một trường hợp đặc biệt của cấu xạ của Mệnh đề 33. Nhưng có thể lập luận theo chiều đối:

#### Mệnh đề 34 {#lie-iii-s3-prop-34 .statement}

*Cho $H$ là một nhóm Lie, $A$ là một đại số kết hợp có đơn vị, đầy đủ, khả chuẩn và $\phi : H \to A^*$ là một cấu xạ nhóm Lie. Cấu xạ liên kết $\phi'$ của $\mathcal{T}^{(\infty)}(H)$ vào $A$ thu được bằng cách hợp thành $\phi_*$ với cấu xạ chính tắc của $\mathcal{T}^{(\infty)}(A^*)$ vào $A$. Đặc biệt, $\phi'(x) = L(\phi)(x)$ với mọi $x \in L(H)$.*

Cho $i$ là ánh xạ đồng nhất của $A^*$ vào $A$. Khi đó, với mọi $t \in \mathcal{T}^{(\infty)}(H)$,
$$
\begin{align*}
\phi'(t) &= \langle t, \phi \rangle = \langle t, i \circ \phi \rangle \\
&= \langle \phi_*(t), i \rangle \quad \text{(Diff. \& Anal. Man., R, 13.2.3)}.
\end{align*}
$$

### 10. ĐẠI SỐ LIE CỦA MỘT SỐ NHÓM TUYẾN TÍNH

Cho E là một không gian đầy đủ khả chuẩn. Khi đó $\mathcal{L}(E)$ là một đại số kết hợp có đơn vị, đầy đủ, khả chuẩn và $\mathbf{GL}(E)$ là một nhóm Lie. Theo Hệ quả của Mệnh đề 33, no. 9, nếu $T_1(\mathbf{GL}(E))$ được đồng nhất một cách chính tắc với $\mathcal{L}(E)$, cấu trúc đại số Lie trên $\mathbf{L}(\mathbf{GL}(E))$ được cho bởi móc $(x, y) \mapsto xy - yx$ của hai phần tử của $\mathcal{L}(E)$. Đặc biệt, $\mathbf{L}(\mathbf{GL}(n, K))$ được đồng nhất một cách chính tắc với $\mathfrak{gl}(n, K)$ (Chương I, § 1, no. 2).

#### Mệnh đề 35 {#lie-iii-s3-prop-35 .statement}

*Cho E là một không gian vectơ hữu hạn chiều. Cho $\phi$ là cấu xạ $g \mapsto \det g$ của nhóm Lie $\mathbf{GL}(E)$ vào nhóm Lie $K^*$. Ánh xạ $\mathbf{L}(\phi)$ của $\mathcal{L}(E)$ vào K là ánh xạ $x \mapsto \operatorname{Tr} x$. Hạt nhân $\mathbf{SL}(E)$ của $\phi$ là một nhóm con Lie của $\mathbf{GL}(E)$ với đại số Lie $\mathfrak{sl}(E)$.*

Ta chọn một chuẩn và một cơ sở của E. Khai triển của định thức chứng minh rằng
$$
\det(1 + u) \in 1 + \operatorname{Tr} u + o(\|u\|)
$$
khi $u$ tiến về 0 trong $\mathcal{L}(E)$. Do đó, sử dụng Mệnh đề 34, no. 9, với $x \in \mathcal{L}(E) = \mathbf{L}(\mathbf{GL}(E))$:
$$
\mathbf{L}(\phi)(x) = \langle x, \phi \rangle = \operatorname{Tr} x.
$$
Suy ra rằng $\phi$ là một cấu xạ chìm. Vì vậy, $\operatorname{Ker} \phi = \mathbf{SL}(E)$ là một nhóm con Lie của $\mathbf{GL}(E)$ mà đại số Lie của nó là $\operatorname{Ker} \mathbf{L}(\phi) = \mathfrak{sl}(E)$.

Cho $E_1, \ldots, E_n$ là các không gian đầy đủ khả chuẩn và E là tổng trực tiếp của chúng. Mọi $x \in \mathcal{L}(E)$ có thể được biểu diễn bởi một ma trận $(x_{ij})_{1 \leq i, j \leq n}$, trong đó $x_{ij} \in \mathcal{L}(E_i, E_j)$.

#### Mệnh đề 36 {#lie-iii-s3-prop-36 .statement}

*Cho I là một tập con của $\{1, 2, \ldots, n\}$ và G là nhóm con của $\mathbf{GL}(E)$ gồm các $g = (g_{ij})_{1 \leq i, j \leq n} \in \mathbf{GL}(E)$ sao cho $g_{ij} = 0$ với $i < j$ và $g_{ii} = 1$ với $i \in I$. Khi đó G là một phân nhóm Lie của $\mathbf{GL}(E)$ và $\mathbf{L}(G)$ là tập hợp các $x = (x_{ij})_{1 \leq i, j \leq n} \in \mathcal{L}(E)$ sao cho $x_{ij} = 0$ với $i < j$ và $x_{ii} = 0$ với $i \in I$.

Cho S là tập hợp các $(x_{ij}) \in \mathcal{L}(E)$ sao cho $x_{ij} = 0$ với $i < j$ và $x_{ii} = 0$ với $i \in I$. Khi đó G là giao của $\mathbf{GL}(E)$ và không gian affine $1 + S$ của $\mathcal{L}(E)$. Suy ra G là một đa tạp con của $\mathbf{GL}(E)$ và không gian tiếp xúc của G tại 1 được đồng nhất với S.*

Đặc biệt, trong $\mathbf{GL}(n, K)$, nhóm tam giác dưới đầy đủ và nhóm tam giác dưới ngặt, được định nghĩa như trong Integration, Chương VII, § 3, no. 3, là các phân nhóm Lie với các đại số Lie $t(n, K)$ và $n(n, K)$ (Chương I, § 1, no. 2).

#### Mệnh đề 37 {#lie-iii-s3-prop-37 .statement}

*Cho A là một đại số kết hợp có đơn vị khả chuẩn đầy đủ và $x \mapsto x^t$ là một ánh xạ tuyến tính liên tục từ A vào A sao cho $(x^t)^t = x$ và $(xy)^t = y^t x^t$ với mọi $x, y$ trong A. Giả sử K có đặc số $\neq 2$. Cho G là nhóm con của $A^*$ gồm các $x \in A$ sao cho $xx^t = x^t x = 1$. Khi đó G là một phân nhóm Lie của $A^*$ và $\mathbf{L}(G)$ là tập hợp các $y \in A$ sao cho $y^t = -y$.*

Cho S (resp. S') là tập hợp các $y \in A$ sao cho $y = y^t$ (resp. $y = -y^t$). Khi đó S, S' là các không gian con vectơ đóng của A. Công thức

$$
y = \frac{1}{2}(y + y^t) + \frac{1}{2}(y - y^t)
$$

chứng tỏ rằng A là tổng trực tiếp tôpô của S và S'. Cho f là ánh xạ từ A vào S được xác định bởi $f(x) = xx^t$. Ánh xạ này là giải tích. Với mọi $y \in A$, $f(1 + y) = 1 + y + y^t + yy^t$; chọn một chuẩn trên A tương thích với cấu trúc đại số của nó; khi đó

$$
f(1 + y) \in 1 + y + y^t + o(\|y\|) \quad \text{khi } y \text{ tiến tới } 0.
$$

Do đó, $T_1(f)(y) = y + y^t$, nên f là một ánh xạ ngập tại 1. Vì vậy, tồn tại một lân cận mở U của 1 trong A sao cho $U \cap G$ là một đa tạp con của U. Suy ra (§ 1, no. 3, Mệnh đề 6) G là một phân nhóm Lie của $A^*$. Hơn nữa, $L(G) = T_e(G) = \operatorname{Ker} T_1(f)$.

#### Hệ quả 1 {#lie-iii-s3-prop-37-cor-1 .statement}

*Giả sử K có đặc số $\neq 2$. Cho E là một không gian vectơ hữu hạn chiều trên K và $\phi$ là một dạng song tuyến tính đối xứng (resp. phản xứng) không suy biến trên E. Với mọi $u \in \mathcal{L}(E)$, cho $u^*$ là đối ngẫu của u tương ứng với $\phi$. Cho G là nhóm trực giao (resp. xuyến vị) của $\phi$. Khi đó G là một phân nhóm Lie của $\mathbf{GL}(E)$ và $L(G)$ là tập hợp các $x \in \mathcal{L}(E)$ sao cho $x^* = -x$.*

Áp dụng Mệnh đề 37 với $A = \mathcal{L}(E)$ và $x^t = x^*$.*
#### Nhận xét {#lie-iii-s3-n10-rem-1 .statement}

Cho B là một cơ sở của E và J là ma trận của $\phi$ đối với B. Khi đó L(G) là tập hợp các phần tử của $\mathcal{L}(E)$ có ma trận X đối với B thỏa mãn phương trình

$$
{}^tX = -JXJ^{-1}.
$$

Điều này suy ra từ *Algebra*, Chapter IX, § 1, công thức (50).

#### Hệ quả 2 {#lie-iii-s3-prop-37-cor-2 .statement}

*Cho E là một không gian Hilbert phức (tương ứng thực) và U là nhóm đơn nhất của E. Khi đó U là một nhóm con thực của $\mathbf{GL}(E)$ và $L(U)$ là tập hợp các $x \in \mathcal{L}(E)$ sao cho $x^* = -x$.

Áp dụng Mệnh đề 37 với $A = \mathcal{L}(E)$, xét như một đại số trên $\mathbf{R}$, và $x^t = x^*$. \*

#### Hệ quả 3 {#lie-iii-s3-prop-37-cor-3 .statement}

*Cho E là một không gian vectơ phức hữu hạn chiều, $\phi$ là một dạng sesquilinear Hermit không suy biến trên E và U là nhóm đơn nhất của $\phi$. Khi đó U là một nhóm con Lie thực của $\mathbf{GL}(E)$ và $L(U)$ là tập hợp các $x \in \mathcal{L}(E)$ sao cho $ix$ là Hermit.*

Khi $E \neq \{0\}$, U *không* là một nhóm con Lie của nhóm Lie phức $\mathbf{GL}(E)$, vì $L(U)$ không phải là một không gian con vectơ phức của $\mathcal{L}(E)$.

### 11. BIỂU DIỄN TUYẾN TÍNH

Cho G là một nhóm Lie, E là một không gian khả chuẩn đầy đủ và $\pi$ là một biểu diễn tuyến tính giải tích của G trên E (§ 1, no. 2). Cấu xạ liên kết $t \mapsto \langle t, \pi \rangle$ của $\mathcal{T}^{(\infty)}(G)$ vào $\mathcal{L}(E)$ là một cấu xạ đại số (no. 9, Mệnh đề 33) và sự hạn chế của nó trên $L(G)$ là $L(\pi)$. Vậy $L(\pi)$ là một biểu diễn của $L(G)$ trên E (Chương I, § 3, Định nghĩa 1).

#### Mệnh đề 38 {#lie-iii-s3-prop-38 .statement}

Xét G tác động lên E ở bên trái bởi ánh xạ $(g, x) \mapsto \pi(g)x$. Cho b \in E và \varphi(b) là ánh xạ quỹ đạo của nó. Cho T_b(E) được đồng nhất chính tắc với E. Với mọi $t \in L(G)$,

$$
(L(\pi)t)(b) = \langle t, \varphi(b) \rangle = \varphi(b)*t = t * \varepsilon_b.
$$

Đặc biệt, trường vectơ được xác định bởi t trên E là trường $b \mapsto (L(\pi)t)(b)$.

$L(\pi)t = \langle t, \pi \rangle$ (no. 9, Mệnh đề 34). Vì ánh xạ $A \mapsto Ab$ của $\mathcal{L}(E)$ vào E là liên tục và tuyến tính, suy ra rằng

$$
\begin{align*}
(L(\pi)t)(b) &= \langle t, g \mapsto \pi(g)b \rangle \\
&= \langle t, \mathrm{Id}_E \circ \varphi(b) \rangle \\
&= \langle \varphi(b)*t, \mathrm{Id}_E \rangle \quad (\text{Diff. \& Anal. Man., R, 13.2.3}) \\
&= \varphi(b)*t.
\end{align*}
$$

Cuối cùng, $\varphi(b)*t = t * \varepsilon_b$ (no. 3, Mệnh đề 14 (ii)).

#### Mệnh đề 39 {#lie-iii-s3-prop-39 .statement}

Giả sử $K$ có đặc số 0. Cho $G$ là một nhóm Lie, $E$ là một không gian vectơ hữu hạn chiều và $\pi$ là một biểu diễn tuyến tính giải tích của $G$ trên $E$. Cho $E_1, E_2$ là các không gian con vectơ của $E$ sao cho $E_2 \subset E_1$. Tập hợp $G_1$ gồm các $g \in G$ sao cho $\pi(g)x \equiv x$ (mod. $E_2$) với mọi $x \in E_1$ là một nhóm con Lie của $G$ và $L(G_1)$ là tập hợp các $a \in L(G)$ sao cho $L(\pi)a$ ánh xạ $E_1$ vào $E_2$.

Điều này suy ra từ các Mệnh đề 29 (no. 8) và 36 (no. 10).

#### Hệ quả 1 {#lie-iii-s3-prop-39-cor-1 .statement}

Với ký hiệu của Mệnh đề 39, tập hợp các $g \in G$ sao cho $\pi(g)(E_1) \subset E_1$ là một nhóm con Lie của $G$ và đại số Lie của nó là tập hợp các $a \in L(G)$ sao cho $L(\pi)a$ ánh xạ $E_1$ vào $E_1$.

Ta áp dụng Mệnh đề 39 với $E_1 = E_2$.

#### Hệ quả 2 {#lie-iii-s3-prop-39-cor-2 .statement}

Cho $G, E, \pi$ như trong Mệnh đề 39. Cho $F$ là một tập con của $E$. Tập hợp các $g \in G$ sao cho $\pi(g)x = x$ với mọi $x \in F$ là một nhóm con Lie của $G$ và đại số Lie của nó là tập hợp các $a \in L(G)$ sao cho $(L(\pi)a)(x) = 0$ với mọi $x \in F$.

Ta áp dụng Mệnh đề 39 với $E_2 = \{0\}$ và $E_1$ là không gian con vectơ của $E$ sinh bởi $F$.

Cho $\pi_1, \pi_2, \ldots, \pi_n$ là các biểu diễn tuyến tính giải tích của $G$. Rõ ràng tổng trực tiếp $\pi$ của các $\pi_i$ (Đại số, Chương VIII, § 13, no. 1) là một biểu diễn tuyến tính giải tích của $G$ và $L(\pi)$ là tổng trực tiếp của $L(\pi_1), L(\pi_2), \ldots, L(\pi_n)$ (Chương I, § 3, no. 1).

#### Mệnh đề 40 {#lie-iii-s3-prop-40 .statement}

Cho $G$ là một nhóm Lie, $E$ là một không gian đầy đủ chuẩn được, $\pi$ là một biểu diễn tuyến tính giải tích của $G$ trên $E$ và $F$ là một không gian con vectơ đóng của $E$ ổn định dưới $\pi(G)$. Giả sử rằng $K$ có đặc số 0, hoặc rằng $F$ là một nhân tử trực tiếp của $E$.

(i) *Biểu diễn con* $\pi_1$ *và biểu diễn thương* $\pi_2$ *của* $\pi$ *được xác định bởi* $F$ *là các biểu diễn giải tích*.

(ii) $F$ *ổn định dưới* $L(\pi)(L(G))$.

(iii) *Cho* $\varrho_1$ *và* $\varrho_2$ *là biểu diễn con và biểu diễn thương của* $L(\pi)$ *được xác định bởi* $F$. *Khi đó* $L(\pi_1) = \varrho_1, L(\pi_2) = \varrho_2$.

Cho $A$ là tập hợp các $u \in \mathcal{L}(E)$ sao cho $u(F) \subset F$. Khi đó $A$ là một không gian vectơ con đóng của $\mathcal{L}(E)$ và $\pi$ nhận các giá trị của nó trong $A$. Nhờ các giả thiết về $K$ và $F$, ánh xạ $\pi': G \to A$ có cùng đồ thị với $\pi$ là giải tích (*Đa tạp khả vi và giải tích*, R, 5.8.5). Các ánh xạ chính tắc $\theta_1 : A \to \mathcal{L}(F)$ và $\theta_2 : A \to \mathcal{L}(E/F)$ là liên tục và tuyến tính, do đó là giải tích. Điều này chứng minh (i). Các ánh xạ $T_e(\pi)$ và $T_e(\pi')$ có cùng đồ thị và do đó $L(\pi)(L(G)) \subset A$, điều này chứng minh (ii). Ta có
$$
T_e(\pi_1) = T_e(\theta_1 \circ \pi') = \theta_1 \circ T_e(\pi') = \varrho_1 \\
T_e(\pi_2) = T_e(\theta_2 \circ \pi') = \theta_2 \circ T_e(\pi') = \varrho_2.
$$

#### Mệnh đề 41 {#lie-iii-s3-prop-41 .statement}

*Cho* $G$ *là một nhóm Lie và* $\pi_1, \pi_2, \ldots, \pi_n, \pi$ *là các biểu diễn tuyến tính giải tích của* $G$ *trên các không gian đầy đủ khả chuẩn* $E_1, E_2, \ldots, E_n, E$. *Cho*
$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n
$$
*là một ánh xạ đa tuyến tính liên tục từ* $E_1 \times E_2 \times \cdots \times E_n$ *vào* $E$. *Giả sử rằng*
$$
\pi(g)(x_1 x_2 \ldots x_n) = (\pi_1(g)x_1)(\pi_2(g)x_2) \ldots (\pi_n(g)x_n)
$$
*với mọi* $g \in G, x_1 \in E_1, \ldots, x_n \in E_n$. *Khi đó*
$$
(L(\pi)a)(x_1 x_2 \ldots x_n) = \sum_{i=1}^n x_1 x_2 \ldots x_{i-1} ((L(\pi_i)a)x_i) x_{i+1} \ldots x_n
$$
*với mọi* $a \in L(G), x_1 \in E_1, \ldots, x_n \in E_n$.

Làm một ví dụ, ta thực hiện phép tính với $n = 2$.
$$
\begin{align*}
(L(\pi)a)(x_1 x_2) &= \langle a, g \mapsto \pi(g)(x_1 x_2) \rangle & \text{(Mệnh đề 38)} \\
&= \langle a, (g \mapsto \pi_1(g)x_1)(g \mapsto \pi_2(g)x_2) \rangle \\
&= \langle a, g \mapsto \pi_1(g)x_1 \rangle \cdot x_2 + x_1 \cdot \langle a, g \mapsto \pi_2(g)x_2 \rangle & \text{(*Diff.* \& *Anal.* *Man.*, R, 5.5.6)} \\
&= ((L(\pi_1)a)x_1) \cdot x_2 + x_1 \cdot ((L(\pi_2)a)x_2) & \text{(Mệnh đề 38)}.
\end{align*}
$$

#### Hệ quả 1 {#lie-iii-s3-prop-41-cor-1 .statement}

*Cho* $G$ *là một nhóm Lie,* $E_1, \ldots, E_{n+1}$ *là các không gian đầy đủ khả chuẩn và* $\pi_1, \ldots, \pi_{n+1}$ *là các biểu diễn tuyến tính giải tích của* $G$ *trên* $E_1, \ldots, E_{n+1}$. *Cho*
$$
E = \mathcal{L}(E_1, \ldots, E_n; E_{n+1})
$$
*là không gian đầy đủ khả chuẩn của các ánh xạ đa tuyến tính liên tục từ* $E_1 \times \cdots \times E_n$ *vào* $E_{n+1}$ *(Tôpô đại cương, Chương X, § 3, no. 2)*. *Với mọi* $g \in G$, *cho* $\pi(g)$ *là tự đẳng cấu của* $E$ *được xác định bởi*
$$
(\pi(g)u)(x_1, \ldots, x_n) = \pi_{n+1}(g)(u(\pi_1(g)^{-1}x_1, \ldots, \pi_n(g)^{-1}x_n)).
$$

Khi đó $\pi$ là một biểu diễn tuyến tính giải tích của $G$ trên $E$ và
$$
((L(\pi)a)u)(x_1, \ldots, x_n) = -\sum_{i=1}^n u(x_1, \ldots, x_{i-1}, (L(\pi_i)a)x_i, x_{i+1}, \ldots, x_n)
$$
$$
\quad + (L(\pi_{n+1})a)(u(x_1, \ldots, x_n))
$$
với mọi $a \in L(G)$, $u \in E$, $x_1 \in E_1, \ldots, x_n \in E_n$.

Mỗi phần tử $(A_1, \ldots, A_{n+1})$ của $\mathcal{L}(E_1) \times \cdots \times \mathcal{L}(E_{n+1})$ xác định một tự đồng cấu liên tục $\theta(A_1, \ldots, A_{n+1})$ của $E$ bởi công thức
$$
(\theta(A_1, \ldots, A_{n+1})u)(x_1, \ldots, x_n) = A_{n+1}(u(A_1x_1, \ldots, A_nx_n)).
$$
Ánh xạ $\theta$ của $\mathcal{L}(E_1) \times \cdots \times \mathcal{L}(E_{n+1})$ vào $\mathcal{L}(E)$ là liên tục và đa tuyến tính. Khi đó, với mọi $g \in G$,
$$
\pi(g) = \theta(\pi_1(g^{-1}), \ldots, \pi_n(g^{-1}), \pi_{n+1}(g))
$$
và do đó $\pi$ là giải tích. Ta áp dụng Mệnh đề 41 cho ánh xạ
$$
(x_1, \ldots, x_n, u) \mapsto u(x_1, \ldots, x_n)
$$
từ $E_1 \times \cdots \times E_n \times E$ vào $E_{n+1}$. Khi đó
$$
\pi_{n+1}(g)(u(x_1, \ldots, x_n)) = (\pi(g)u)(\pi_1(g)x_1, \ldots, \pi_n(g)x_n)
$$
và do đó
$$
(L(\pi_{n+1})a)(u(x_1, \ldots, x_n)) = \sum_{i=1}^n u(x_1, \ldots, (L(\pi_i)a)x_i, \ldots, x_n)
$$
$$
\quad + ((L(\pi)a)u)(x_1, \ldots, x_n).
$$

Khi các $E_i$ là hữu hạn chiều, biểu diễn $L(\pi)$ của $L(G)$ được dẫn xuất từ các biểu diễn $L(\pi_1), \ldots, L(\pi_{n+1})$ theo thủ tục của Chương I, § 3, Mệnh đề 3.

#### Hệ quả 2 {#lie-iii-s3-prop-41-cor-2 .statement}

Cho $G$ là một nhóm Lie và $\pi$ là một biểu diễn tuyến tính giải tích của $G$ trên một không gian định chuẩn đầy đủ $E$. Khi đó $g \mapsto {}^t\pi(g)^{-1}$ là một biểu diễn tuyến tính giải tích $\rho$ của $G$ trên không gian định chuẩn đầy đủ $\mathcal{L}(E, K)$\footnote{Cũng như khi $K = \mathbf{R}$ hoặc $\mathbf{C}$, chuyển vị ${}^t\pi(g)$ xét ở đây là sự hạn chế lên $\mathcal{L}(E, K)$ của chuyển vị của $\pi(g)$ theo nghĩa đại số thuần túy.} và $L(\rho)a = -{}^t(L(\pi)a)$ với mọi $a \in L(G)$.

Đây là một trường hợp riêng của Hệ quả 1.

$\rho$ được gọi là biểu diễn *phản liên hợp* của $\pi$.

Khi $E$ là hữu hạn chiều, $L(\rho)$ là biểu diễn đối ngẫu của $L(\pi)$ theo nghĩa của Chương I, § 3, no. 3.

#### Hệ quả 3 {#lie-iii-s3-prop-41-cor-3 .statement}

Cho $G$ là một nhóm Lie và $\pi_1, \ldots, \pi_n$ là các biểu diễn tuyến tính giải tích của $G$ trên các không gian vectơ hữu hạn chiều $E_1, \ldots, E_n$. Khi đó biểu diễn $\pi_1 \otimes \cdots \otimes \pi_n$ của $G$ (Phụ lục) là giải tích và $L(\pi_1 \otimes \cdots \otimes \pi_n)$ là tích tenxơ của $L(\pi_1), \ldots, L(\pi_n)$.

Ánh xạ $(A_1, \ldots, A_n) \mapsto A_1 \otimes \cdots \otimes A_n$ của $\mathcal{L}(E_1) \times \cdots \times \mathcal{L}(E_n)$ vào $\mathcal{L}(E_1 \otimes \cdots \otimes E_n)$ là đa tuyến tính, do đó $\pi$ là giải tích. Xét ánh xạ $(x_1, \ldots, x_n) \mapsto x_1 \otimes \cdots \otimes x_n$ của $E_1 \times \cdots \times E_n$ vào
$$
E_1 \otimes \cdots \otimes E_n.
$$
Theo Mệnh đề 41, ta thấy rằng
$$
(L(\pi)a)(x_1 \otimes \cdots \otimes x_n) = \sum_{i=1}^n x_1 \otimes \cdots \otimes (L(\pi_i)a)x_i \otimes \cdots \otimes x_n
$$
với mọi $a \in L(G)$, $x_i \in E_i$ đối với $1 \leq i \leq n$. Do đó $L(\pi)$ là tích tenxơ của các $L(\pi_i)$.

#### Hệ quả 4 {#lie-iii-s3-prop-41-cor-4 .statement}

Cho $G$ là một nhóm Lie và $\pi$ là một biểu diễn tuyến tính giải tích của $G$ trên một không gian vectơ hữu hạn chiều $E$. Khi đó các biểu diễn $T^n(\pi)$, $S^n(\pi)$ và $\wedge^n(\pi)$ của $G$ (Phụ lục) là giải tích và
$$
L(T^n(\pi)) = T^n(L(\pi)), \quad L(S^n(\pi)) = S^n(L(\pi)), \quad L(\wedge^n(\pi)) = \wedge^n(L(\pi)).
$$
Điều này suy ra từ Hệ quả 3 và Mệnh đề 40.

#### Hệ quả 5 {#lie-iii-s3-prop-41-cor-5 .statement}

Cho $A$ là một đại số hữu hạn chiều. Giả sử $K$ có đặc số 0. Nhóm tự đẳng cấu $\mathrm{Aut}(A)$ của $A$ là một nhóm con Lie của $\mathbf{GL}(A)$ và $L(\mathrm{Aut}(A))$ là đại số Lie của các đạo hàm của $A$.

Điều này suy ra từ Hệ quả 1 (áp dụng cho $E = \mathcal{L}(A, A; A)$) và Hệ quả 2 của Mệnh đề 39 (áp dụng cho tập con của $E$ gồm chỉ phép nhân trên $A$).

#### Nhận xét {#lie-iii-s3-n11-rem-1 .statement}

Áp dụng Hệ quả 1 với $G = \mathbf{GL}(F)$ ($F$ là một không gian chuẩn hóa đầy đủ), $\pi_1 = \pi_2 = \mathrm{Id}_G$ và $\pi_3$ là biểu diễn tầm thường của $G$ trên $K$. Ta thu được một biểu diễn giải tích $\pi$ của $\mathbf{GL}(F)$ trên $\mathcal{L}(F, F; K)$. Giả sử rằng $F$ là hữu hạn chiều và rằng $K$ có đặc số 0. Áp dụng Hệ quả 2 của Mệnh đề 39 cho $\pi$, ta thu lại phần của Hệ quả 1 của Mệnh đề 37.

#### Mệnh đề 42 {#lie-iii-s3-prop-42 .statement}

Cho $G$ là một nhóm Lie, $X$ là một đa tạp giải tích, $(g, x) \mapsto gx$ (resp. $xg$) là một luật của phép toán trái (resp. phải) giải tích của $G$ trên $X$ và $x_0$ là một điểm của $X$ bất biến dưới $G$. Với mọi $g \in G$, ký hiệu $\tau(g)$ là tự đẳng cấu $x \mapsto gx$ (resp. $xg$) của $X$ và ký hiệu $\pi(g)$ là tự đẳng cấu của $T_{x_0}(X)$ tiếp xúc tại $x_0$ với $\tau(g)$.
(i) $\pi$ là một biểu diễn giải tích của $G$ (resp. $G^\vee$) trên $T_{x_0}(X)$.
(ii) Với mọi $a \in L(G)$ và mọi $\xi_0 \in T_{x_0}(X)$, $L(\pi)a.\xi_0$ có thể được tính như sau: gọi $D_a$ là trường vectơ do $a$ xác định trên $X$ và $\xi$ là một trường vectơ lớp $C^1$ trong một lân cận mở của $x_0$ sao cho $\xi(x_0) = \xi_0$; khi đó
$$
L(\pi)a.\xi_0 = -[D_a, \xi](x_0).
$$

$\tau(gg') = \tau(g)\tau(g')$ (resp. $\tau(g')\tau(g)$) và do đó $\pi(gg') = \pi(g)\pi(g')$ (resp. $\pi(g')\pi(g)$). Mặt khác, vì $TX$ là một G-tập vectơ của lớp $C^\omega$ (§ 1, no. 8, Proposition 16), $\pi$ là giải tích, do đó (i).

Để chứng minh (ii), giả sử G tác động bên trái. Tồn tại một lân cận mở I của 0 trong K và một ánh xạ giải tích $\gamma$ từ I vào G sao cho $\gamma(0) = e, T_0(\gamma)1 = a$. Khi đó $D_a$ là trường vectơ trên X được xác định bởi ánh xạ $\phi : (\lambda, x) \mapsto \gamma(\lambda)x$ của $I \times X$ vào X (§ 2, no. 2). Nếu $\phi_\lambda$ ký hiệu song ánh $x \mapsto \gamma(\lambda)x$ của X vào X, thì

$$
[D_a, \xi](x_0) = \left( \frac{d}{d\lambda} (T_{\phi_\lambda(x_0)}(\phi_\lambda^{-1})\xi(\phi_\lambda(x_0))) \right)_{\lambda=0} \quad (\text{Diff. \& Anal. Man., R,}
$$
$$
= \left( \frac{d}{d\lambda} (T_{x_0}(\phi_\lambda^{-1})\xi_0) \right)_{\lambda=0}
$$
$$
= \left( \frac{d}{d\lambda} (\pi(\gamma(\lambda))^{-1}\xi_0) \right)_{\lambda=0}.
$$

Vì các ánh xạ $\lambda \mapsto \gamma(\lambda)^{-1}$ và $\lambda \mapsto \gamma(-\lambda)$ tiếp xúc tại 0, nên điều này cũng bằng
$$
- \left( \frac{d}{d\lambda} (\pi(\gamma(\lambda))\xi_0) \right)_{\lambda=0}
$$
$$
= - \left( \frac{d}{d\lambda} (\pi \circ \gamma)(\lambda) \right)_{\lambda=0} \xi_0
$$
$$
= -L(\pi)a.\xi_0.
$$

### 12. BIỂU DIỄN LIÊN HỢP

Xét luật của phép toán trái giải tích
$$
(g, g') \mapsto gg'g^{-1} = (\operatorname{Int} g)g'
$$
của $G$ vào $G$. Luật của phép toán này xác định, theo no. 3, một ánh xạ song tuyến tính của $\mathcal{T}^{(\infty)}(G) \times \mathcal{T}^{(\infty)}(G)$ vào $\mathcal{T}^{(\infty)}(G)$, và trong no. này ta ký hiệu nó bởi $\tau$. Theo Mệnh đề 13 của no. 3,
$$
(t * t') \tau t'' = t \tau (t' \tau t'')
$$
với mọi $t, t', t''$ trong $\mathcal{T}^{(\infty)}(G)$. Theo Mệnh đề 14 (i) của no. 3,
$$
\varepsilon_g \tau t = (\operatorname{Int} g)_*t
$$
với mọi $g \in G$ và $t \in \mathcal{T}^{(\infty)}(G)$. Đặc biệt, ánh xạ $t \mapsto \varepsilon_g \tau t$ của $\mathcal{T}^{(\infty)}(G)$ vào $\mathcal{T}^{(\infty)}(G)$ là một tự đẳng cấu của đại số song $\mathcal{T}^{(\infty)}(G)$. Các hạn chế của nó lên $U(G), U_s(G), L(G)$ được ký hiệu lần lượt bởi $\operatorname{Ad}_{U(G)}(g), \operatorname{Ad}_{U_s(G)}(g), \operatorname{Ad}_{L(G)}(g)$. Ta thường viết $\operatorname{Ad}(g)$ thay cho $\operatorname{Ad}_{L(G)}(g)$ khi không thể nhầm lẫn. Theo (23), $\operatorname{Ad}(g)$ là ánh xạ tiếp tuyến tại e của $\operatorname{Int}(g)$. Nó là một tự đẳng cấu của đại số Lie khả chuẩn $\mathbf{L}(G)$. Khi $K$ có đặc số 0, $\mathrm{Ad}_{\mathbf{U}(G)}(g)$ là tự đẳng cấu duy nhất của $\mathbf{U}(G)$ mở rộng $\mathrm{Ad}(g)$.

Nếu $\phi$ là một cấu xạ của nhóm Lie $G$ vào một nhóm Lie $H$, thì
$$
\phi_*(t \top t') = \phi_*(t) \top \phi_*(t')
$$
với mọi $t, t'$ trong $\mathcal{T}^{(\infty)}(G)$; điều này suy ra từ Mệnh đề 15 của no. 3.

#### Mệnh đề 43 {#lie-iii-s3-prop-43 .statement}

*Cho $t, u$ thuộc $\mathcal{T}^{(\infty)}(G)$. Cho $\sum_{i=1}^n t_i \otimes t'_i$ là ảnh của $t$ dưới đồng tích. Khi đó*
$$
t \top u = \sum_{i=1}^n t_i * u * {t'_i}^\vee.
$$

Theo định nghĩa, $t \top u$ là ảnh của $t \otimes u$ dưới ánh xạ $(g, g') \mapsto gg'g^{-1}$ của $G \times G$ vào $G$. Nay ánh xạ này thu được bằng cách hợp thành các ánh xạ sau:
$$
\begin{aligned}
\alpha & : (g, g') \mapsto (g, g, g') & \text{của } G \times G \text{ vào } G \times G \times G \\
\beta & : (g, g', g'') \mapsto (g, {g'}^{-1}, g'') & \text{của } G \times G \times G \text{ vào } G \times G \times G \\
\gamma & : (g, g', g'') \mapsto gg''g' & \text{của } G \times G \times G \text{ vào } G.
\end{aligned}
$$

Mặt khác:
$$
\begin{aligned}
\alpha_*(t \otimes u) &= \sum_{i=1}^n (t_i \otimes t'_i) \otimes u = \sum_{i=1}^n t_i \otimes t'_i \otimes u \\
\beta_* \left( \sum_{i=1}^n t_i \otimes t'_i \otimes u \right) &= \sum_{i=1}^n t_i \otimes {t'_i}^\vee \otimes u \\
\gamma_* \left( \sum_{i=1}^n t_i \otimes {t'_i}^\vee \otimes u \right) &= \sum_{i=1}^n t_i * u * {t'_i}^\vee.
\end{aligned}
$$

#### Hệ quả 1 {#lie-iii-s3-prop-43-cor-1 .statement}

*Cho $u \in \mathbf{L}(G)$ và $u' \in \mathcal{T}^{(\infty)}(G)$. Khi đó $u \top u' = u * u' - u' * u$.*

Ảnh của $u$ dưới đồng tích là $u \otimes \varepsilon_e + \varepsilon_e \otimes u$, do đó
$$
u \top u' = u * u' * \varepsilon_e + \varepsilon_e * u' * u^\vee = u * u' - u' * u.
$$

#### Hệ quả 2 {#lie-iii-s3-prop-43-cor-2 .statement}

*Cho $t \in \mathcal{T}^{(\infty)}(G)$ và $g \in G$. Khi đó $\varepsilon_g \top t = \varepsilon_g * t * \varepsilon_{g^{-1}}$. Nếu $t \in \mathbf{L}(G)$, thì $\varepsilon_g \top t = gtg^{-1}$ (trong đó tích sau cùng được tính trong nhóm $\mathbf{T}(G)$).*

Ảnh của $\varepsilon_g$ dưới đồng tích là $\varepsilon_g \otimes \varepsilon_g$.

#### Hệ quả 3 {#lie-iii-s3-prop-43-cor-3 .statement}

*Cho $a \in \mathbf{L}(G)$. Trường vectơ được xác định bởi $a$ và phép toán trái $g \mapsto \mathrm{Int}\, g$ của $G$ trên $G$ là trường $\mathbf{R}_a - \mathbf{L}_a$.*

Giá trị của trường này tại $g$ là
$$
\begin{aligned}
a \top \varepsilon_g &= a * \varepsilon_g - \varepsilon_g * a & \text{(Hệ quả 1)} \\
&= (\mathbf{R}_a)_g - (\mathbf{L}_a)_g & \text{(Định nghĩa 5)}.
\end{aligned}
$$

Với mọi $g \in G$ và mọi $t \in L(G)$,
$$
(\mathrm{Ad}\,g)(t) = \varepsilon_g \top t = \varepsilon_g * t * \varepsilon_g^{-1} = gtg^{-1}.
$$
Vì $\mathrm{Ad}\,g = T_e(\mathrm{Int}\,g)$, Mệnh đề 42 của no. 11 chứng minh rằng $\mathrm{Ad}$ là một biểu diễn tuyến tính giải tích của $G$ trên không gian khả chuẩn $L(G)$.

#### Định nghĩa 8 {#lie-iii-s3-def-8 .statement}

*Biểu diễn Ad của G trên L(G) được gọi là biểu diễn đối liên của G.*

#### Mệnh đề 44 {#lie-iii-s3-prop-44 .statement}

*Với mọi $a \in L(G)$,*
$$
(L(\mathrm{Ad}))(a) = \mathrm{ad}_{L(G)}a.
$$
Cho $b \in L(G)$. Theo Mệnh đề 42 (ii) của no. 11 và Hệ quả 3 của Mệnh đề 43,
$$
(L(\mathrm{Ad}))(a).b = -[R_a - L_{a_1}L_b](e).
$$
Bây giờ $R_a \circ L_b = L_b \circ R_a$ (no. 6, Mệnh đề 23 (ii)), do đó $[R_a, L_b] = 0$; rồi, dùng Mệnh đề 23 (ii),
$$
(L(\mathrm{Ad}))(a).b = [L_a, L_b](e) = L_{[a, b]}(e) = [a, b] = (\mathrm{ad}_{L(G)}a)b.
$$

#### Mệnh đề 45 {#lie-iii-s3-prop-45 .statement}

*Giả sử $G$ hữu hạn chiều và $K$ có đặc số 0. Gọi $s$ là một số nguyên $\geqslant 0$. Khi đó ánh xạ $\pi : g \mapsto \mathrm{Ad}_{U_s(G)}(g)$ là một biểu diễn tuyến tính giải tích của $G$ trên $U_s(G)$ và $L(\pi)a = \mathrm{ad}_{U_s(G)}a$ với mọi $a \in L(G)$.*

Biểu diễn tuyến tính $\pi$ là một thương của $\bigoplus_{r=0}^s \mathrm{Tr}(\mathrm{Ad})$ và do đó là giải tích. Với $a \in L(G)$ và $x_1, x_2, \ldots, x_s$ trong $L(G)$,
$$
\begin{align*}
(L(\pi)a)(x_1x_2\ldots x_s) &= \sum_{i=1}^s x_1 \ldots (L(\mathrm{Ad})a.x_i) \ldots x_s & \text{(Mệnh đề 41)} \\
&= \sum_{i=1}^s x_1 \ldots ([a, x_i]) \ldots x_s & \text{(Mệnh đề 44)} \\
&= (\mathrm{Ad}_{U_s(G)}a)(x_1x_2\ldots x_s).
\end{align*}
$$

#### Mệnh đề 46 {#lie-iii-s3-prop-46 .statement}

*Cho $h \in G, x \in T_h(G)$ và $a \in L(G)$. Gọi $\phi$ là ánh xạ $(g, g') \mapsto gg'g^{-1}$ từ $G \times G$ vào $G$. Ảnh y của $(a, x) \in T_e(G) \times T_h(G)$ dưới $T_{(e, h)}(\phi)$ là $y = x + h((\mathrm{Ad}\,h^{-1})a - a)$.
Ta có*
$$
\begin{align*}
y &= (T_{(e, h)}\phi)(a \otimes \varepsilon_h + \varepsilon_e \otimes x) \\
&= a \top \varepsilon_h + \varepsilon_e \top x \\
&= a * \varepsilon_h - \varepsilon_h * a + x \\
&= h((\mathrm{Ad}\,h^{-1})a) - ha + x.
\end{align*}
$$

#### Mệnh đề 47 {#lie-iii-s3-prop-47 .statement}

Cho $G$ là một nhóm Lie, $H$ và $E$ là các nhóm con Lie của $G$ và giả sử rằng $hEh^{-1} = E$ với mọi $h \in H$. Khi đó $\mathcal{T}^{(\infty)}(H) \subset \mathcal{T}^{(\infty)}(E) \subset \mathcal{T}^{(\infty)}(E)$. Đặc biệt, $\mathrm{Ad}(H)(L(E)) \subset L(E)$ và $[L(H), L(E)] \subset L(E)$.

Nếu $t \in \mathcal{T}^{(\infty)}(H)$ và $t' \in \mathcal{T}^{(\infty)}(E)$, thì $t \otimes t' \in \mathcal{T}^{(\infty)}(H \times E)$ và ảnh của $H \times E$ dưới ánh xạ $(g, g') \mapsto gg'g^{-1}$ được chứa trong $E$.

#### Mệnh đề 48 {#lie-iii-s3-prop-48 .statement}

Cho G là một nhóm Lie và H và E là các nhóm con Lie của G. Giả sử rằng G là, với tư cách một nhóm Lie, tích nửa trực tiếp của H bởi E. Cho $\varphi$ là biểu diễn tuyến tính $g \mapsto (\mathrm{Ad}\, g) \mid L(E)$ của nhóm Lie G trên $L(E)$ (xem Mệnh đề 47) và cho $\sigma$ là hạn chế của $\varphi$ lên H. Khi đó:
(i) $L(G)$ là tổng trực tiếp tôpô của $L(H)$ và $L(E)$;
(ii) $L(H)$ là một đại số con của $L(G)$ và $L(E)$ là một iđêan của $L(G)$;
(iii) $L(\sigma)$ là một biểu diễn tuyến tính của $L(H)$ trên đại số Lie của các đạo hàm của $L(E)$;
(iv) $L(G)$ là tích nửa trực tiếp của $L(H)$ bởi $L(E)$ được xác định bởi $L(\sigma)$ (Chương I, § 1, no. 8).

(i) là hiển nhiên và (ii) suy ra từ Mệnh đề 47. $L(\sigma) = L(\varphi) \mid L(H)$. Bây giờ theo Mệnh đề 40 (no. 11) và 44 (no. 12), $L(\varphi)(t)$ là, với mọi $t \in L(G)$, hạn chế của $\mathrm{ad}_{L(G)} t$ lên $L(E)$. Điều này chứng minh (iii). Dùng (i) và (ii), điều này cũng chứng minh (iv).

#### Hệ quả {#lie-iii-s3-n12-cor-1 .statement}

Cho G là một nhóm Lie. Cho $T_e(G)$ được trang bị cấu trúc đại số Lie giao hoán duy nhất của nó. Cho $\tau$ là một biểu diễn kề của $L(G)$. Khi đó đại số Lie của $T(G)$ là tích nửa trực tiếp của $L(G)$ bởi $T_e(G)$ được xác định bởi $\tau$. Nói cách khác, với $x, x'$ trong $L(G)$ và $y, y'$ trong $T_e(G)$,

$$
[(x, y), (x', y')] = ([x, x'], [x, y'] + [y, x'])
$$

(trong đó dấu ngoặc ở vế trái được tính trong $L(T(G))$ và các dấu ngoặc ở vế phải trong $L(G)$).

Điều này suy ra từ Mệnh đề 48 và Mệnh đề 6 của § 2, no. 2.

#### Mệnh đề 49 {#lie-iii-s3-prop-49 .statement}

Cho A là một đại số kết hợp có đơn vị, đầy đủ và khả chuẩn. Ta đồng nhất A với $L(A^*)$. Khi đó, nếu $g \in A^*$ và $y \in A$, $(\mathrm{Ad}\, g)y = gyg^{-1}$.

Nhớ rằng $\mathrm{Ad}\, g = T_1(\mathrm{Int}\, g)$. Cho $u_g$ là ánh xạ $x \mapsto gxg^{-1}$ của A vào A. Bản đồ đồng nhất của $A^*$ vào A biến đổi $\mathrm{Int}\, g$ thành $u_g \mid A^*$. Ánh xạ tiếp tuyến tại mỗi điểm của $A^*$ của ánh xạ này bằng $u_g$, do đó suy ra mệnh đề.

#### Hệ quả {#lie-iii-s3-n12-cor-2 .statement}

Với mọi $g \in A^*$, đặt $i(g)$ là tự đẳng cấu $y \mapsto gyg^{-1}$ của A, sao cho $i$ là một biểu diễn tuyến tính giải tích của $A^*$ trên A. Với mọi $z \in L(A^*) = A, L(i)z$ là đạo hàm nội $y \mapsto zy - yz$ của A.

Điều này suy ra từ Mệnh đề 49 và Mệnh đề 44.

### 13. TENXƠ VÀ CÁC DẠNG BẤT BIẾN

#### Mệnh đề 50 {#lie-iii-s3-prop-50 .statement}

*Cho G là một nhóm Lie (giả sử hữu hạn chiều nếu K có đặc số > 0). Cho E là không gian vectơ của các dạng đa tuyến tính phản xứng liên tục bậc k trên \mathrm{T}_e(G). Với mọi u \in E, cho \omega^u là dạng vi phân bậc k trên G sao cho $(\omega^u)_g$ là dạng đa tuyến tính trên \mathrm{T}_g(G) được dẫn xuất từ u bởi phép tịnh tiến $h \mapsto gh$ (resp. $h \mapsto hg$). Khi đó \omega^u là giải tích và bất biến trái (resp. phải) trên G. Ánh xạ u \mapsto \omega^u là một đẳng cấu của E lên không gian vectơ của các dạng vi phân bậc k bất biến trái (resp. phải) trên G.*

Đây là một trường hợp riêng của điều đã nói ở trên.

Cho $F$ là một không gian khả chuẩn đầy đủ. Mệnh đề 50 vẫn đúng nếu các dạng vi phân trên $G$ nhận giá trị trong $K$ được thay bởi các dạng vi phân trên $G$ nhận giá trị trong $F$. Với mọi ánh xạ tuyến tính liên tục $u$ từ $\mathrm{T}_e(G)$ vào $F$, tồn tại một dạng vi phân $\omega^u$ bậc 1 trên $G$, với giá trị trong $F$, sao cho $(\omega^u)_g = u \circ \mathrm{T}_g(\gamma(g)^{-1})$. Đặc biệt, lấy $F = \mathrm{T}_e(G)$ và $u = \mathrm{Id}_{\mathrm{T}_e(G)}$. Khi đó ta thu được dạng vi phân $\omega$ trên $G$ sao cho $\omega_g = T_g(\gamma(g^{-1}))$; dạng vi phân này bất biến trái và giải tích; nó được gọi là *dạng vi phân chính tắc trái* của $G$. $\omega_g(t) = g^{-1}t$ với mọi $t \in T_g(G)$.

Nếu $F$ lại là một không gian khả chuẩn đầy đủ tùy ý và $u \in \mathcal{L}(T_e(G), F)$, thì $\omega^u = u \circ \omega$. Đặc biệt (lấy $F = K$), ánh xạ $v \mapsto v \circ \omega$ là một song ánh tuyến tính từ đối ngẫu của $T_e(G)$ lên không gian vectơ các dạng vi phân bậc 1 với giá trị trong $K$ và bất biến trái dưới $G$.

Tương tự, dạng vi phân $\omega'$ trên $G$ sao cho $\omega'_g = T_g(\delta(g))$ được gọi là *dạng vi phân chính tắc phải* của $G$. Có những tính chất tương tự như của $\omega$, mà chúng tôi để người đọc phát biểu. Ánh xạ $g \mapsto g^{-1}$ của $G$ lên $G$ biến $\omega$ thành $\omega'$.

### 14. CÔNG THỨC MAURER–CARTAN

Cho $X$ là một đa tạp lớp $C^r$, có số chiều hữu hạn nếu $K$ có đặc số $> 0$, và cho $L$ là một đại số Lie khả chuẩn đầy đủ. Cho $\alpha$ là một dạng vi phân bậc 1 trên $X$ với giá trị trong $L$, thuộc lớp $C^{r-1}$. Cho $x \in X$. Ánh xạ

$$
(u_1, u_2) \mapsto [\alpha_x(u_1), \alpha_x(u_2)]
$$

từ $T_x(X) \times T_x(X)$ vào $L$ là một dạng song tuyến tính liên tục phản xứng trên $T_x(X)$ với giá trị trong $L$. Ta ký hiệu nó bởi $[\alpha]^2_x$, do đó $[\alpha]^2$ là một dạng vi phân bậc 2 trên $X$ với giá trị trong $L$. Xác định một lân cận mở của $x$ trong $X$ với một tập mở của một không gian Banach, ta thấy ngay rằng $[\alpha]^2$ thuộc lớp $C^{r-1}$. Nếu $X'$ là một đa tạp lớp $C^r$ và $f : X' \to X$ là một cấu xạ, thì

$$
[f^*(\alpha)]^2 = f([\alpha]^2).
$$

Cho $\alpha, \beta$ là hai dạng vi phân bậc 1 trên $X$ với giá trị trong $L$ thuộc lớp $C^{r-1}$. Tích ngoài $\alpha \wedge \beta$ của $\alpha$ và $\beta$ (*Differentiable and Analytic Manifolds*, R, 7.8.2) là một dạng vi phân bậc 2 trên $X$ với giá trị trong $L$ thuộc lớp $C^{r-1}$; ta có

$$
(\alpha \wedge \beta)_x(u_1, u_2) = [\alpha_x(u_1), \beta_x(u_2)] - [\alpha_x(u_2), \beta_x(u_1)]
$$

với $u_1, u_2$ trong $T_x(X)$. Suy ra ngay rằng

$$
[\alpha + \beta]^2 = [\alpha]^2 + [\beta]^2 + \alpha \wedge \beta
$$
$$
\alpha \wedge \alpha = 2[\alpha]^2.
$$

#### Mệnh đề 51 {#lie-iii-s3-prop-51 .statement}

*Cho $G$ là một nhóm Lie, hữu hạn chiều nếu $K$ có đặc số $> 0$, và cho $a_1, \ldots, a_p$ là các phần tử của $L(G)$, $F$ là một không gian định chuẩn đầy đủ và $\alpha$ là một dạng vi phân bậc $p-1$ trên $G$ với giá trị trong $F$. Nếu $\alpha$ bất biến trái, thì*

$$
(d\alpha)_e(a_1, \ldots, a_p) = \sum_{i<j} (-1)^{i+j} \alpha_e([a_i, a_j], a_1, \ldots, a_{i-1}, a_{i+1}, \ldots, a_{j-1}, a_{j+1}, \ldots, a_p).
$$

Nếu $\alpha$ bất biến phải, thì
$$
(d\alpha)_e(a_1, \ldots, a_p)
= - \sum_{i < j} (-1)^{i+j} \alpha_e([a_i, a_j], a_1, \ldots, a_{i-1}, a_{i+1}, \ldots, a_{j-1}, a_{j+1}, \ldots, a_p).
$$
Giả sử rằng $\alpha$ bất biến trái. Theo *Differentiable and Analytic Manifolds*, R, 8.5.7, khi đó
$$
(d\alpha)(L_{a_1}, \ldots, L_{a_p}) = \sum_i (-1)^{i-1} L_{a_i} \alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p})
+ \sum_{i < j} (-1)^{i+j} \alpha([L_{a_i}, L_{a_j}], L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_{j-1}}, L_{a_{j+1}}, \ldots, L_{a_p}).
$$
Nhưng các hàm $\alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p})$ trên G là bất biến trái và do đó là hằng. Suy ra
$$
L_{a_i} \alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p}) = 0.
$$
Hơn nữa, $[L_{a_i}, L_{a_j}] = L_{[a_i, a_j]}$ (Mệnh đề 23), do đó có công thức thứ nhất của Mệnh đề 51. Công thức thứ hai có thể được thiết lập tương tự, lần này dùng quan hệ $[R_{a_i}, R_{a_j}] = -R_{[a_i, a_j]}$.

#### Hệ quả 1 {#lie-iii-s3-prop-51-cor-1 .statement}

*Cho $G$ là một nhóm Lie, hữu hạn chiều nếu $K$ có đặc số $> 0$, và $\omega$ và $\omega'$ là các dạng vi phân chính tắc trái và phải của G. Khi đó*
$$
d\omega + [\omega]^2 = 0, \qquad d\omega' - [\omega']^2 = 0.
$$
Theo Mệnh đề 51,
$$
(d\omega)_e(a_1, a_2) = -\omega_e([a_1, a_2]) = -[a_1, a_2] = -[\omega_e(a_1), \omega_e(a_2)]
= -[\omega]^2_e(a_1, a_2)
$$
do đó có công thức thứ nhất. Công thức thứ hai có thể được thiết lập tương tự.

#### Hệ quả 2 {#lie-iii-s3-prop-51-cor-2 .statement}

*Giả sử rằng G hữu hạn chiều. Cho $(e_1, \ldots, e_n)$ là một cơ sở của $L(G)$, $(e_1^*, \ldots, e_n^*)$ là cơ sở đối ngẫu, $(c_{ijk})$ là các hằng số cấu trúc của $L(G)$ theo cơ sở $(e_1, \ldots, e_n)$ và $\omega_i$ (tương ứng $\omega'_i$) là dạng vi phân bất biến trái (tương ứng phải) trên G với giá trị trong K sao cho $(\omega_i)_e = e_i^*$ (tương ứng $(\omega'_i)_e = e_i^*$). Khi đó*
$$
d\omega_k + \sum_{i < j} c_{ijk} \omega_i \wedge \omega_j = 0 \quad (k = 1, 2, \ldots, n)
$$
$$
d\omega'_k - \sum_{i < j} c_{ijk} \omega'_i \wedge \omega'_j = 0 \quad (k = 1, 2, \ldots, n).
$$
Nếu $r < s$,
$$
(d\omega_k)_e(e_r, e_s) = -(\omega_k)_e([e_r, e_s])
= -\sum_i c_{rsi} (\omega_k)_e(e_i)
= -c_{rsk}
= -\sum_{i < j} c_{ijk} (\omega_i \wedge \omega_j)_e(e_r, e_s).
$$
Lập luận tương tự cho các $\omega'_k$.

### 15. PHÉP DỰNG CÁC DẠNG VI PHÂN BẤT BIẾN

#### Bổ đề 2 {#lie-iii-s3-lem-2 .statement}

Cho G là một nhóm Lie, U là một lân cận mở đối xứng của e trong G, E là một không gian định chuẩn đầy đủ và $\phi : U^2 \to E$ là một ánh xạ giải tích. Với mọi $g \in U$, cho $\omega_g$ là vi phân tại điểm g của ánh xạ $h \mapsto \phi(g^{-1}h)$. Khi đó $\omega$ là hạn chế lên U của dạng vi phân bất biến trái trên G có giá trị tại e là $d_e \phi$.

Rõ ràng $\omega_e = d_e \phi$. Với mọi $g \in U$ và mọi $t \in T_e(G)$,

$$
\langle \omega_g, T_e(\gamma(g))t \rangle = \langle d_g(\phi \circ \gamma(g)^{-1}), T_e(\gamma(g))t \rangle \\
= \langle d_e \phi \circ T_g(\gamma(g)^{-1}), T_e(\gamma(g))t \rangle = \langle d_e \phi, t \rangle
$$

và do đó $\omega_g$ được dẫn xuất từ $d_e \phi$ bởi $T_e(\gamma(g))$.

#### Mệnh đề 52 {#lie-iii-s3-prop-52 .statement}

Cho n là một số nguyên > 0, G là một nhóm Lie n chiều, U là một lân cận mở đối xứng của e trong G và $\psi : U^2 \to K^n$ là một bản đồ của G sao cho $\psi(e) = 0$. Nếu $(x_1, \ldots, x_n)$ là các tọa độ của $x \in \psi(U)$ và $(y_1, \ldots, y_n)$ là các tọa độ của $y \in \psi(U)$, ta ký hiệu

$$
m_1(x_1, \ldots, x_n, y_1, \ldots, y_n), \ldots, m_n(x_1, \ldots, x_n, y_1, \ldots, y_n)
$$

là các tọa độ của $\psi(\psi^{-1}(x)^{-1}\psi^{-1}(y))$. Khi đó, nếu viết, với $1 \leq k \leq n$,

$$
\varpi_k(x_1, \ldots, x_n) = D_{n+1} m_k(x_1, \ldots, x_n, x_1, \ldots, x_n) dx_1 + \cdots \\
+ D_{2n} m_k(x_1, \ldots, x_n, x_1, \ldots, x_n) dx_n,
$$

thì các dạng vi phân $\varpi_k$ trên $\psi(U)$ được dẫn xuất qua $\psi$ từ các dạng vi phân bất biến trái trên G và thỏa mãn $\varpi_k(0, \ldots, 0) = dx_k$.

Ta áp dụng Bổ đề 2 với $E = K$, lấy $\phi(g)$ là tọa độ của $\psi(g)$ có chỉ số k. Ta thu được một dạng vi phân $\omega_k$; gọi $\varpi_k$ là biến đổi của nó dưới $\psi$. Giá trị của $\varpi_k$ tại $(x_1, \ldots, x_n)$ là vi phân tại $(x_1, \ldots, x_n)$ của hàm $y \mapsto m_k(x_1, \ldots, x_n, y_1, \ldots, y_n)$; do đó giá trị này được cho bởi công thức (32). Khi đó chỉ cần dùng kết luận của Bổ đề 2.

#### Mệnh đề 53 {#lie-iii-s3-prop-53 .statement}

Cho G là một nhóm Lie, A là một đại số đầy đủ chuẩn hóa được và $\phi$ là một morphism nhóm Lie của G vào $A^*$. Với mọi $g \in G$, đặt $\omega_g = \phi(g)^{-1} d_g \phi$. Khi đó $\omega$ là dạng vi phân bất biến trái trên G có giá trị tại e là d_e \phi.

Ta áp dụng Bổ đề 2 với $E = A$ và $U = G$. Vi phân tại g của ánh xạ $h \mapsto \phi(g^{-1}h) = \phi(g)^{-1} \phi(h)$ là $\phi(g)^{-1} d_g \phi$.

### 16. ĐỘ ĐO HAAR TRÊN MỘT NHÓM LIE

Cho G là một nhóm Lie có số chiều hữu hạn n. Khi đó $\bigwedge^n(T_e(G))$ có số chiều 1. Do đó (no. 13) không gian vectơ S của các dạng vi phân bất biến trái bậc n trên G có số chiều 1. Cho $(\omega_1, \ldots, \omega_n)$ là một cơ sở của không gian các dạng vi phân bất biến trái bậc 1 trên G; khi đó $\omega_1 \wedge \omega_2 \wedge \cdots \wedge \omega_n$ là một cơ sở của S.

#### Mệnh đề 54 {#lie-iii-s3-prop-54 .statement}

Cho G là một nhóm Lie có số chiều hữu hạn n, $\omega$ là một dạng vi phân bất biến trái bậc n trên G và $\phi$ là một tự đồng cấu của G. Khi đó

$$
\phi^*(\omega) = (\det L(\phi)) \omega.
$$

Ta viết $L(\phi) = u$, $w_e = f$ và $\phi^*(\omega)_e = g$. Với mọi $x_1, \ldots, x_n$ trong $L(G)$,

$$
g(x_1, \ldots, x_n) = f(ux_1, \ldots, ux_n) = (\det u)f(x_1, \ldots, x_n)
$$

và do đó $\phi^*(\omega)_e = \det L(\phi) \cdot w_e$. Mặt khác, nếu $g \in G$,

$$
\phi \circ \gamma(g) = \gamma(\phi(g)) \circ \phi
$$

và do đó $\gamma(g)^*\phi^*(\omega) = \phi^*(\omega)$. Vậy $\phi^*(\omega)$ là bất biến trái, do đó mệnh đề.

#### Hệ quả {#lie-iii-s3-n16-cor-1 .statement}

Với mọi $g \in G$,

$$
\delta(g)^*\omega = (\det \mathrm{Ad}\, g) \omega.
$$

$$
\delta(g)^*\omega = \delta(g)^*\gamma(g)^*\omega = (\mathrm{Int}\, g)^*\omega \text{ và } L(\mathrm{Int}\, g) = \mathrm{Ad}\, g.
$$

Cho G là một nhóm compact địa phương và φ là một tự đồng cấu của G. Giả sử rằng tồn tại các lân cận mở V, $V'$ của e sao cho $\phi(V) = V'$ và $\phi|V$ là một đẳng cấu địa phương của G vào G. Cho μ là một độ đo Haar trái trên G. Theo Tích phân, chương VII, § 1, Hệ quả của Mệnh đề 9, tồn tại duy nhất một số $a > 0$ sao cho $\phi(\mu|V) = a^{-1}\mu|V'$. Rõ ràng a không phụ thuộc vào lựa chọn của V, $V'$ và μ. Nó được gọi là môđun của φ và được ký hiệu bởi $\mathrm{mod}_G \phi$ hoặc đơn giản $\mathrm{mod}\, \phi$. Khi φ là một tự đẳng cấu của G, ta thu được Định nghĩa 4 của Tích phân, chương VII, § 1.

#### Mệnh đề 55 {#lie-iii-s3-prop-55 .statement}

Giả sử rằng K là compact địa phương. Cho μ là một độ đo Haar trên nhóm cộng của K. Cho G là một nhóm Lie có số chiều hữu hạn n.

(i) Cho ω là một dạng vi phân bậc n khác không, bất biến trái trên G. Khi đó độ đo $\mathrm{mod}(\omega)_\mu$ (Đa tạp khả vi và giải tích, R, 10.1.6) là một độ đo Haar trái trên G. Nếu $K = \mathbf{R}$ và G có hướng do ω xác định, thì độ đo do ω xác định (Đa tạp khả vi và giải tích, R, 10.4.3) là một độ đo Haar trái trên G.

(ii) Cho φ là một tự đồng cấu étale của G. Khi đó $\mathrm{mod}\, \phi = \mathrm{mod}\, \det L(\phi)$.

(i) hiển nhiên. Cho V, $V'$ là các lân cận mở của e sao cho $\phi(V) = V'$ và $\phi|V$ là một đẳng cấu địa phương của G vào G. Khi đó

$$
\phi^{-1}(\mathrm{mod}(\omega)_\mu|V') = \mathrm{mod}(\phi^*(\omega))_\mu|V) \quad \text{do phép chuyển cấu trúc}
$$
$$
= \mathrm{mod}(\det L(\phi)\omega|V)_\mu \quad \text{(Mệnh đề 54)}
$$
$$
= \mathrm{mod}\, \det L(\phi)(\mathrm{mod}(\omega)_\mu|V)
$$

do đó $\mathrm{mod}\, \phi = \mathrm{mod}\, \det L(\phi)$ theo định nghĩa của $\mathrm{mod}\, \phi$.

#### Hệ quả {#lie-iii-s3-n16-cor-2 .statement}

Với mọi $g \in G$, $\Delta_G(g) = (\operatorname{mod} \det \operatorname{Ad} g)^{-1}$. Đặc biệt, để $G$ là đơn môđula, điều kiện cần và đủ là $\operatorname{mod} \det \operatorname{Ad} g = 1$ với mọi $g \in G$.

$$
\Delta_G(g) = (\operatorname{mod} \operatorname{Int} g)^{-1} \quad \text{(Tích phân, chương VII, § 1, công thức (33))}
= (\operatorname{mod} \det L(\operatorname{Int} g))^{-1} \quad \text{(Mệnh đề 55)}
= (\operatorname{mod} \det \operatorname{Ad} g)^{-1}.
$$

#### Nhận xét {#lie-iii-s3-n16-rem-1 .statement}

Giữ nguyên các giả thiết và ký hiệu của Mệnh đề 52, giả sử rằng K là compact địa phương. Cho μ là độ đo
$$
\operatorname{mod} \det(D_{n+i}m_k(x_1, \ldots, x_n, x_1, \ldots, x_n))_{1 \leq i, k \leq n} dx_1 \ldots dx_n
$$
trên $\psi(U)$. Khi đó $\psi^{-1}(\mu)$ là hạn chế lên U của một độ đo Haar trên G.

#### Mệnh đề 56 {#lie-iii-s3-prop-56 .statement}

Cho G là một nhóm Lie có số chiều hữu hạn n, H là một nhóm con Lie p chiều và X là không gian thuần nhất Lie $G/H$. Giả sử rằng
$$
\det \operatorname{Ad}_{L(G)} h = \det \operatorname{Ad}_{L(H)} h
$$
với mọi $h \in H$. Khi đó:
(i) Các dạng vi phân bậc $n - p$ trên X bất biến dưới tác dụng của G là giải tích.
(ii) Không gian vectơ của các dạng đó có số chiều 1.
(iii) Nếu ω là một dạng như vậy khác không và K là compact địa phương, $\operatorname{mod}(\omega)_\mu$ là một độ đo khác không trên X bất biến dưới G.

Theo § 1, no. 8, Ví dụ, $\operatorname{Alt}^{n-p}(TX, K)$ là một bó vectơ giải tích $G$. Cho $x_0$ là ảnh chính tắc của $e$ trong $X$; nhóm ổn định của nó là $H$. Sợi của $\operatorname{Alt}^{n-p}(TX, K)$ tại $x_0$ là $\bigwedge^{n-p} T_{x_0}(X)^*$ và $T_{x_0}(X)$ được đồng nhất một cách chính tắc với $L(G)/L(H)$. Nếu $h \in H$, tự đẳng cấu $\tau_h$ của $X$ do $h$ xác định là dẫn xuất khi chuyển qua thương từ tự đẳng cấu $g \mapsto hgh^{-1}$ của $G$. Do đó tự đẳng cấu $T_{x_0}(\tau_h)$ là dẫn xuất khi chuyển qua thương từ $\operatorname{Ad}_{L(G)}(h)$. Như
$$
\det \operatorname{Ad}_{L(G)} h = (\det \operatorname{Ad}_{L(H)} h) \cdot (\det T_{x_0}(\tau_h)),
$$
giả thiết suy ra rằng $\det T_{x_0}(h) = 1$. Vậy mọi phần tử của $\bigwedge^{n-p} T_{x_0}(X)^*$ đều bất biến dưới $H$. Khi đó (i) và (ii) suy ra từ § 1, no. 8, Hệ quả 1 của Mệnh đề 17 và (iii) hiển nhiên.

Sự tồn tại của một độ đo dương khác 0 trên $X$ bất biến dưới $G$ suy ra từ Tích phân, Chương VII, § 2, Hệ quả 2 của Định lý 3, vì giả thiết của Mệnh đề 56 suy ra $\Delta_G|H = \Delta_H$ (Hệ quả của Mệnh đề 55).

#### Mệnh đề 57 {#lie-iii-s3-prop-57 .statement}

Cho $G$ là một nhóm Lie có số chiều hữu hạn $n$. Chọn một cơ sở cho $\bigwedge^n T_e(G)^*$; bằng sự tầm thường hóa phải (tương ứng trái) của $\bigwedge^n T(G)^*$, ta có thể đồng nhất bó vectơ này với bó vectơ tầm thường $G \times K$, sao cho chuyển vị của một toán tử vi phân vô hướng được đồng nhất với một toán tử vi phân vô hướng.

Khi đó, nếu $u \in U(G)$, chuyển vị của $L_u$ (tương ứng $R_u$) là $L_u^\nu$ (tương ứng $R_u^\nu$).

Ta sẽ xét trường hợp trong đó $\Lambda^n T(G)^*$ đã được tầm thường hóa bằng một dạng bất biến phải $\omega$.

Giả sử mệnh đề đã được chứng minh cho các phần tử $u_1, u_2$ của $U(G)$. Khi đó,

$$
\begin{align*}
t(L_{u_1 * u_2}) &= t(L_{u_1} \circ L_{u_2}) & \text{(Mệnh đề 23)} \\
&= t(L_{u_2}) \circ t(L_{u_1}) & \text{(\emph{Diff. \& Anal. Man.}, R, 14.3.3)} \\
&= L_{u_2}^\nu \circ L_{u_1}^\nu & \text{theo giả thiết} \\
&= L_{u_2 * u_1}^{\nu \nu} & \text{(Mệnh đề 23)} \\
&= L_{(u_1 * u_2)^\nu} & \text{(Mệnh đề 7)}
\end{align*}
$$

và do đó mệnh đề đúng với $u_1 * u_2$. Vì vậy đủ để chứng minh mệnh đề khi $u \in T_e(G)$. Bây giờ $L_u$ được xác định bởi $G$ tác động lên $G$ ở bên phải (no. 6) và do đó $\theta_{L_u} \omega = 0$ vì $\omega$ là bất biến phải (\emph{Differentiable and Analytic Manifolds}, R, 8.4.5); vì thế, nếu $f$ là một hàm giải tích trong một lân cận mở của $e$ nhận giá trị trong $K$, thì $\theta_{L_u}(f \omega) = (\theta_{L_u} f) \omega$ (\emph{Differentiable and Analytic Manifolds}, R, 8.4.8). Dùng các đồng nhất thức đã nêu và \emph{Differentiable and Analytic Manifolds}, R, 14.4.1, chuyển vị của $L_u$ là $-L_u$, tức là $L_u^\nu$.

#### Hệ quả {#lie-iii-s3-n16-cor-3 .statement}

Let $G$ be a finite-dimensional real Lie group, $\mu$ (resp. $\nu$) a left (resp. right) Haar measure on $G$, $k$ an integer $\geqslant 0$, $u \in U_k(G)$ and $f$ and $g$ real-valued functions of class $C^k$ on $G$ with compact support. Khi đó

$$
\int_G (R_u f) g \, d\mu = \int_G f (R_u^\nu g) \, d\mu
$$
$$
\int_G (L_u f) g \, d\nu = \int_G f (L_u^\nu g) \, d\nu.
$$

Điều này suy ra từ Mệnh đề 57 và \emph{Differentiable and Analytic Manifolds}, R, 14.3.8.

### 17. VI PHÂN TRÁI

#### Định nghĩa 9 {#lie-iii-s3-def-9 .statement}

Let $G$ be a Lie group, $M$ a manifold of class $C^r$ and $f$ a mapping of class $C^r$ of $M$ into $G$. Vi phân trái (tương ứng phải) của $f$ là dạng vi phân bậc 1 trên $M$ với giá trị trong $L(G)$, gán với mỗi vectơ $u \in T_m(M)$ phần tử $f(m)^{-1} \cdot (T_m f)(u)$ (tương ứng $(T_m f)(u) \cdot f(m)^{-1}$).

Trong chương này chúng ta chỉ xét vi phân trái, mà ta sẽ ký hiệu là $f^{-1}.df$, và để lại cho bạn đọc việc chuyển các kết quả sang vi phân phải.

Nếu $f$ là ánh xạ đồng nhất của $G$, $f^{-1}.df$ là dạng vi phân trái chính tắc $\omega$ của $G$. Trở lại trường hợp tổng quát của Định nghĩa 8,

$$
(f^{-1}.df)_m = \omega_{f(m)} \circ T_m(f)
$$

và do đó $f^{-1}.df = f^*(\omega)$. Điều này suy ra rằng $f^{-1}.df$ thuộc lớp $C^{r-1}$.

#### Ví dụ {#lie-iii-s3-n17-exa-1 .statement}

(1) Nếu $G$ là nhóm cộng của một không gian chuẩn hóa đầy đủ và $T_0(E)$ được đồng nhất chính tắc với $E$, thì $f^{-1}.df$ là vi phân $df$ được định nghĩa trong Differentiable and Analytic Manifolds, R, 8.2.2.

(2) Giả sử $G$ là nhóm nhân $A^*$ liên kết với một đại số chuẩn hóa đầy đủ $A$. Khi đó có thể xem $f$ như một ánh xạ của $M$ vào $A$ và do đó vi phân $df$ theo nghĩa của Differentiable and Analytic Manifolds, R, 8.2.2 được xác định, và tích $f^{-1}df$ theo nghĩa của Differentiable and Analytic Manifolds, R, 8.3.2 được xác định. Rõ ràng dạng sau cùng này trùng với vi phân trái của $f$.

#### Mệnh đề 58 {#lie-iii-s3-prop-58 .statement}

Let $G$ và $H$ là hai nhóm Lie, $M$ là một đa tạp lớp $C^r$, $f$ là một ánh xạ lớp $C^r$ của $M$ vào $G$ và $h$ là một cấu xạ của $G$ vào $H$. Khi đó

$$
(h \circ f)^{-1}.d(h \circ f) = L(h) \circ (f^{-1}.df) = (h^{-1}.dh) \circ T(f).
$$

Với mọi $x \in M$ và $u \in T_x(M)$,

$$
(h \circ f)^{-1}.d(h \circ f)(u) = ((h \circ f)(x))^{-1}.T(h \circ f)(u).
$$

Biểu thức sau bằng, một mặt, với

$$
T(h)(f(x)^{-1}.T(f)(u)) \quad (§ 2, \text{Mệnh đề 5})
$$
$$
= T_e(h)((f^{-1}.df)(u))
$$

và, mặt khác, với

$$
h(f(x))^{-1}T(h)(T(f)u)
$$
$$
= (h^{-1}.dh)(T(f)u).
$$

#### Mệnh đề 59 {#lie-iii-s3-prop-59 .statement}

Cho $G$ là một nhóm Lie, $M$ là một đa tạp lớp $C^r$, $f$ và $g$ là các ánh xạ lớp $C^r$ của $M$ vào $G$ và $p$ là toàn cấu chính tắc của $TM$ lên $M$.

(i) $(fg)^{-1}.d(fg) = (\mathrm{Ad} \circ g \circ p)^{-1} \circ (f^{-1}.df) + g^{-1}.dg.$

(ii) Viết $h(m) = f(m)^{-1}$ với mọi $m \in M$,

$$
h^{-1}.dh = -(\mathrm{Ad} \circ f \circ p) \circ (f^{-1}.df).
$$

Mệnh đề (i) suy ra từ § 2, no. 2, Mệnh đề 7. Mệnh đề (ii) suy ra từ (i) bằng cách đặt $g = h$.

#### Hệ quả 1 {#lie-iii-s3-prop-59-cor-1 .statement}

Cho $s \in G$ và $sg$ là ánh xạ $x \mapsto sg(x)$ của $M$ vào $G$. Khi đó

$$
(sg)^{-1}.d(sg) = g^{-1}.dg.
$$

Điều này suy ra từ Mệnh đề 59 (i) khi lấy $f$ là ánh xạ hằng $x \mapsto s$ của $M$ vào $G$.

#### Hệ quả 2 {#lie-iii-s3-prop-59-cor-2 .statement}

*Nếu các ánh xạ $f$ và $g$ của $M$ vào $G$ có cùng vi phân trái, thì ánh xạ tiếp tuyến của $fg^{-1}$ ở mọi nơi đều bằng không. Nếu thêm $K$ có đặc số 0, thì $fg^{-1}$ là địa phương hằng.*

Theo Mệnh đề 59,

$$
(fg^{-1})^{-1} \cdot d(fg^{-1}) = (\mathrm{Ad} \circ g \circ p) \circ (f^{-1}.df) - (\mathrm{Ad} \circ g \circ p) \circ (g^{-1}.dg).
$$

Nếu $f^{-1}.df = g^{-1}.dg$, thì $(fg^{-1})^{-1} \cdot d(fg^{-1}) = 0$, tức là $T_x(fg^{-1}) = 0$ với mọi $x \in M$. Điều này chứng minh mệnh đề thứ nhất. Mệnh đề thứ hai suy ra từ đó theo *Differentiable and Analytic Manifolds*, R, 5.5.3.

#### Mệnh đề 60 {#lie-iii-s3-prop-60 .statement}

*Cho $G$ là một nhóm Lie, hữu hạn chiều nếu $K$ có đặc số > 0, $M$ là một đa tạp lớp $C^r$, $f$ là một ánh xạ lớp $C^r$ của $M$ vào $G$ và $\alpha$ là vi phân trái của $f$. Khi đó $d\alpha + [\alpha]^2 = 0$.*

Cho $\omega$ là dạng vi phân trái chính tắc của $G$. Dùng Hệ quả 1 của Mệnh đề 51, no. 14, ta có

$$
d\alpha = d(f^*(\omega)) = f^*(d\omega) = f^*(-[\omega]^2)
= -[f^*(\omega)]^2 = -[\alpha]^2.
$$

### 18. ĐẠI SỐ LIE CỦA MỘT MẦM NHÓM LIE

Trong số này, $(G, e, \theta, m)$ ký hiệu một mầm nhóm Lie. Phần lớn các kết quả của § vẫn đúng với cùng một chứng minh. Ta sẽ xem lại những kết quả mà ta thấy hữu ích.

18.1. Cho $\Omega$ là miền xác định của $m$. Cho $(g, g') \in \Omega,\ t \in T_e^{(\infty)}(G),\ t' \in T_{g'}^{(\infty)}(G)$. Như ở no. 1, tích chập của $t$ và $t'$, ký hiệu là $t * t'$, là ảnh của $t \otimes t'$ dưới $m$. Ta viết $U(G) = T_e^{(\infty)}(G),\ U_s(G) = T_e^{(s)}(G),\ U^+(G) = T_e^{(\infty)+}(G),\ U_s^+(G) = T_e^{(s)+}(G)$. Với $t, t'$ trong $U(G)$, $t * t'$ được xác định và thuộc $U(G)$. Với tích chập, $U(G)$ là một đại số kết hợp có phần tử đơn vị $\varepsilon_e$, được lọc bởi các $U_s(G)$. Đẳng cấu chính tắc $i_{G,e}$ của gr $U(G)$ lên $TS(T_e(G))$ là một đẳng cấu đại số.

18.2. Cho $G, H$ là các mầm nhóm Lie và $\phi : G \to H$ là một cấu xạ. Nếu $t \in U(G)$, ảnh $U(\phi)(t)$ của $t$ dưới $\phi_*$ là một phần tử của $U(H)$ và $U(\phi)$ là một cấu xạ của đại số $U(G)$ vào đại số $U(H)$. Ánh xạ $\theta : x \mapsto x^{-1}$ của $G$ vào $G$ xác định một ánh xạ $t \mapsto t^\vee$ của $U(G)$ vào $U(G)$. Với $t, t'$ trong $U(G)$, tích $t * t'$ được xét tương ứng với $G^\vee$ bằng tích $t' * t$ được xét tương ứng với $G$ và $(t * t')^\vee = {t'}^\vee * t^\vee$. Khi đó $U(\phi)(t^\vee) = (U(\phi)t)^\vee$. Nếu $G_1, \ldots, G_n$ là các mầm nhóm Lie và $G = G_1 \times \cdots \times G_n$, thì đẳng cấu chính tắc của $U(G_1) \otimes \cdots \otimes U(G_n)$ lên $U(G)$ là một đẳng cấu đại số;

với $t_1, \ldots, t_n$ trong $U(G)$, $(t_1 \otimes \cdots \otimes t_n)^{\vee} = t_1^{\vee} \otimes \cdots \otimes t_n^{\vee}$. Cho $H$ là một mầm nhóm con Lie của $G$ và $i : H \to G$ là đơn ánh chính tắc. Khi đó $U(i)$ là một đồng cấu đơn cấu của đại số $U(H)$ vào $U(G)$ và
$$
U(i)(t^{\vee}) = (U(i)(t))^{\vee}
$$
với mọi $t \in U(H)$. Với tích chập và đồng tích được xác định bởi cấu trúc đa tạp trên $G$, $U(G)$ là một bigebra và $U(\phi)$ là một cấu xạ bigebra.

18.3. Cho $G$ là một mầm nhóm Lie, $X$ là một đa tạp lớp $C^r$ và $\psi$ là một mảnh luật của phép toán trái lớp $C^r$ của $G$ trên $X$. Cho $\Omega$ là tập hợp xác định của $\psi$. Nếu $t \in T^{(s)}_g(G)$, $u \in T^{(s')}_x(X)$, $(g, x) \in \Omega$ và $s + s' \leq r$, hãy ký hiệu $t * u$ là ảnh của $t \otimes u$ dưới $\psi_*$. Cho $t \in T^{(s)}_g(G)$, $t' \in T^{(s')}_x(G)$, $u \in T^{(s'')}_x(X)$; nếu $s + s' + s'' \leq r$ và $gg'$, $(gg')x$, $g'x$, $g(g'x)$ đều được xác định, thì
$$
(t * t') * u = t * (t' * u).
$$
Cho $x_0 \in X$ và $\rho(x_0)$ là ánh xạ $g \mapsto gx_0$, được xác định trên một lân cận mở của $e$. Nếu $t \in U_r(G)$, thì $\rho(x_0)_*t = t * \varepsilon_{x_0}$. Ở đây và trong phần còn lại của số này, chúng tôi sẽ để cho bạn đọc nhiệm vụ dịch các kết quả cho các mảnh luật của phép toán phải.

18.4. Giữ nguyên ký hiệu của 18.3, cho $t \in U_s(G)$ với $s \leq r$. Cho $f$ là một hàm lớp $C^r$ trên $X$ nhận giá trị trong một không gian đa chuẩn Hausdorff. Ký hiệu $t * f$ là hàm trên $X$ được xác định bởi
$$
\begin{align*}
(t * f)(x) &= \langle t, g \mapsto f(\psi(\theta(g), x)) \rangle \\
&= \langle t^{\vee}, f \circ \rho(x) \rangle = \langle \rho(x)_*(t^{\vee}), f \rangle = \langle t^{\vee} * \varepsilon_x, f \rangle.
\end{align*}
$$
Nếu $t \in U_s(G)$, $t' \in U_{s'}(G)$ và $s + s' \leq r$, thì $\langle t', t * f \rangle = \langle t^{\vee} * t', f \rangle$ và $(t * t') * f = t * (t' * f)$. Cho $t \in U_s(G)$, $f$ và $f'$ là các hàm lớp $C^r$ trên $X$ nhận giá trị trong các không gian đa chuẩn Hausdorff $F, F'$ và $(u, u') \mapsto u.u'$ là một ánh xạ song tuyến tính liên tục của $F \times F'$ vào một không gian đa chuẩn Hausdorff; cho
$$
\sum_{i=1}^n t_i \otimes t'_i
$$
là ảnh của $t$ dưới đồng tích; nếu $s \leq r$, thì
$$
t * (ff') = \sum_{i=1}^n (t_i * f)(t'_i * f').
$$

18.5. Giữ ký hiệu của 18.3, cho $t \in U_s(G)$ với $s \leq r$. Ánh xạ $x \mapsto t * \varepsilon_x$ được gọi là trường các phân phối điểm do $t$ xác định và phần luật của phép toán, và đôi khi được ký hiệu bởi $D_t^{\psi}$ hoặc $D_t$. Nếu $f : X \to F$ là một hàm lớp $C^r$, thì hàm $t^{\vee} * f$ trên $X$ cũng được ký hiệu bởi $D_t f$; nó thuộc lớp $C^{r-s}$ nếu $s < \infty$. Nếu $t \in U_s(G)$, $t' \in U_{s'}(G)$ và $s + s' \leq r$, thì $D_{t*t'} f = D_{t'}(D_t f)$. Nếu $G$ và $X$ là hữu hạn chiều, thì $D_t$ là một toán tử vi phân trên $X$ có bậc $\leq s$ và thuộc lớp $C^{r-s}$ (nếu $s < \infty$). Khi đó hàm $D_t f$ là phép biến đổi của $f$ dưới toán tử vi phân này.

18.6. Cho G là một mầm nhóm Lie và $t \in U(G)$. $L_t$ ký hiệu trường các phân phối điểm $g \mapsto \varepsilon_g * t$ trên G và $R_t$ ký hiệu trường các phân phối điểm $g \mapsto t * \varepsilon_g$ trên G. Nếu $f \in C^\omega(G, F)$, thì $L_t f \in C^\omega(G, F)$ và $R_t f \in C^\omega(G, F)$. Với $t, t'$ trong $U(G)$, $L_{t \circ t'} = L_t \circ L_{t'}$, $R_{t \circ t'} = R_{t'} \circ R_t$, $L_t \circ R_{t'} = R_{t'} \circ L_t$, $\theta(L_t) = R_t^V$.

18.7. Vì $T_e(G)$ là tập các phần tử nguyên thủy của $U(G)$,

$$
[T_e(G), T_e(G)] \subset T_e(G).
$$

Không gian khả chuẩn $T_e(G)$, cùng với ngoặc, là một đại số Lie khả chuẩn, được gọi là đại số Lie khả chuẩn của G (hay đại số Lie của G) và được ký hiệu bởi $L(G)$. Cho $E(G)$ là đại số bao của $L(G)$. Đơn ánh chính tắc của $L(G)$ vào $U(G)$ định nghĩa một đồng cấu $\eta$ của đại số $E(G)$ vào đại số $U(G)$; nếu K có đặc số 0, thì $\eta$ là một đẳng cấu bigebra, nhờ đó $U(G)$ được đồng nhất với $E(G)$. Dùng ký hiệu của 18.3, với mọi $a \in L(G)$, cho $D_a$ là trường các phân phối điểm được $a$ xác định trên X. Ánh xạ $(a, x) \mapsto D_a(x)$ là một cấu xạ lớp $C^{r-1}$ của bó vectơ tầm thường $L(G) \times X$ vào bó vectơ $T(X)$. Cho $I$ là một tập con mở của K chứa 0 và $\gamma : I \to G$ là một ánh xạ lớp $C^r$ sao cho $\gamma(0) = e$. Đặt $a = T_0(\gamma) l \in L(G)$. Nếu $f : X \to F$ là một hàm lớp $C^r$, thì

$$
(D_a f)(x) = \lim_{k \in K^*, k \to 0} k^{-1}(f(\gamma(k)x) - f(x)).
$$

Nếu $r \geq 2$, thì ánh xạ $a \mapsto D_a$ là một luật của phép toán vi phân trái lớp $C^{r-1}$ của $L(G)$ trên X.

18.8. Cho G và H là các mầm nhóm Lie và $\phi$ là một cấu xạ của G vào H. Hạn chế của $U(\phi)$ lên $L(G)$, chính là $T_e(\phi)$, là một cấu xạ liên tục của $L(G)$ vào $L(H)$, và ta ký hiệu nó bởi $L(\phi)$. Nếu $\psi$ là một cấu xạ của H vào một mầm nhóm Lie, thì $L(\psi \circ \phi) = L(\psi) \circ L(\phi)$. Để $\phi$ là một phép nhập, điều kiện cần và đủ là $L(\phi)$ là một đẳng cấu của $L(G)$ lên một đại số con Lie của $L(H)$ có một phần bù tôpô. Đặc biệt, nếu G là một mầm nhóm con Lie của H và $\phi$ là đơn ánh chính tắc, thì $L(G)$ được đồng nhất với một đại số con Lie của $L(H)$ nhờ $L(\phi)$. Nếu $(G_i)_{i \in I}$ là một họ hữu hạn các mầm nhóm Lie và G là tích của chúng, thì $L(G)$ được đồng nhất một cách chính tắc với $\prod_{i \in I} L(G_i)$.

18.9. Cho G là một mầm nhóm Lie, có số chiều hữu hạn nếu K có đặc số > 0. Cho F là một không gian khả chuẩn đầy đủ. Cho $\alpha$ là một dạng vi phân bậc k trên G nhận giá trị trong F. $\alpha$ được gọi là bất biến trái trên G nếu $\alpha_g$ được dẫn xuất từ $\alpha_e$ qua ánh xạ $h \mapsto gh$ của một lân cận của e lên một lân cận của g. Nếu $\alpha$ bất biến trái, thì $\alpha$ là giải tích. Ánh xạ $\alpha \mapsto \alpha_e$ là một song ánh từ tập hợp các dạng vi phân bất biến trái bậc k trên G nhận giá trị trong F lên tập hợp các ánh xạ k-tuyến tính phản xứng liên tục của $T_e(G)$ vào F. Nếu $\alpha_e = \mathrm{Id}_{T_e(G)}$, thì $\alpha$ được gọi là *dạng vi phân chính tắc trái của G*. Các định nghĩa của các dạng vi phân bất biến phải và dạng vi phân chính tắc phải của G là tương tự. Nếu $\omega$ là dạng vi phân chính tắc trái của G, thì $d\omega + [\omega]^2 = 0$. Cho M là một đa tạp lớp $C^r$ và $f$ là một ánh xạ lớp $C^r$ của M vào G. Vi phân trái của $f$, ký hiệu $f^{-1}.df$, là dạng vi phân bậc 1 trên M nhận giá trị trong $L(G)$, gán cho mỗi vectơ $u \in T_m(M)$ phần tử $f(m)^{-1}.(T_{m,f})(u)$. Khi đó $f^{-1}.df = f^*(\omega)$ và $d\alpha + [\alpha]^2 = 0$. Nếu hai ánh xạ $f$ và $g$ của M vào G có cùng vi phân trái và K có đặc số 0, thì $fg^{-1}$ là hằng địa phương.

### Bài tập {#lie-iii-s3-exercises}

Xem [bài tập cho § 3](exercises/s3/).
