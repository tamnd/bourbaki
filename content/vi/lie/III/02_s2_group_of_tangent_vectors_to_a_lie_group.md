---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 2
section_title: Group of tangent vectors to a Lie group
lang: vi
source: lie-i-iii
pdf_pages: 0251-0256
extraction: ocr
subsections:
    - "no": 1
      title: TANGENT LAWS OF COMPOSITION
      page: 0
      pdf_page: 251
    - "no": 2
      title: GROUP OF TANGENT VECTORS TO A LIE GROUP
      page: 0
      pdf_page: 253
    - "no": 3
      title: CASE OF GROUP GERMS
      page: 0
      pdf_page: 255
statements: 10
exercises: 0
content_sha256: 6e766b3dca880cbcf4b6aea4bd295328ae2a32580fae7cb2410eea31f7e3d07d
translated_from: content/en/lie/III/02_s2_group_of_tangent_vectors_to_a_lie_group.md
source_content_sha256: 7845b7e2bd4a655ddc90c51d69de092ba1cf892797854eb6ec7e8069c2d39675
translation_model: gpt-5-6-mini
translation_run: translate-vi-e80acfda
glossary_version: 34
glossary_terms_sha256: bb63172a74008c374a16e4003bbaa26a1b7c90328dd9870731057ff8be4ad9e3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. NHÓM CÁC VECTƠ TIẾP XÚC CỦA MỘT NHÓM LIE

### 1. CÁC LUẬT HỢP THÀNH TIẾP XÚC

Cho X và Y là các đa tạp thuộc lớp C^r. Ta biết (Các đa tạp khả vi và giải tích, R, 8.1.4) rằng X \times Y là một đa tạp thuộc lớp C^r và rằng ánh xạ (T(pr_1), T(pr_2)), tích của các ánh xạ tiếp xúc của các phép chiếu chính tắc, là một đẳng cấu thuộc lớp C^{r-1} của T(X \times Y) lên T(X) \times T(Y).\footnote{Đối với r = 1, điều này có nghĩa là (T(pr_1), T(pr_2)) là một đồng cấu của T(X \times Y) lên T(X) \times T(Y).} Đẳng cấu này tương thích với các cấu trúc bó vectơ có không gian cơ sở là X \times Y và cho phép ta đồng nhất T(X \times Y) với T(X) \times T(Y). Cho a ∈ X, b ∈ Y, u ∈ T_a(X), v ∈ T_b(Y); sự đồng nhất ở trên cho phép ta xem (u, v) như một phần tử của T_{(a, b)}(X × Y); khi đó

$$(u, v) = (u, 0) + (0, v)$$

và (u, 0) (tương ứng (0, v)) là ảnh của u (tương ứng v) qua ánh xạ tiếp xúc của phép nhúng x ↦ (x, b) (tương ứng y ↦ (a, y)) của X (tương ứng Y) vào X × Y. Khi cần chính xác, ta sẽ viết 0_a cho phần tử không của T_a(x).

Bây giờ cho X, Y, Z là các đa tạp thuộc lớp C^r và f là một ánh xạ thuộc lớp C^r của X × Y vào Z. Ánh xạ tiếp xúc là, nhờ sự đồng nhất ở trên, một ánh xạ thuộc lớp C^{r-1} của T(X) × T(Y) vào T(Z). Với u ∈ T_a(X) và v ∈ T_b(Y),

(1)
$$T(f)(u, v) = T(f)(u, 0_b) + T(f)(0_a, v),$$
(2)
$$T(f)(0_a, 0_b) = 0_{f(a, b)}.$$

Mặt khác, ánh xạ y ↦ f(a, y) là hợp thành của phép nhúng y ↦ (a, y) và f; do đó

(3) $T(f)(0, v)$ là ảnh của v qua ánh xạ tiếp xúc của ánh xạ $y ↦ f(a, y)$.

Tương tự

(4) $T(f)(u, 0)$ là ảnh của u qua ánh xạ tiếp xúc của ánh xạ $x ↦ f(x, b)$.

Nếu ánh xạ f của X × Y vào Z được ký hiệu bởi (x, y) ↦ xy, thì uv thường được dùng để ký hiệu phần tử T(f)(u, v) với u ∈ T(X), v ∈ T(Y).

Cho X là một đa tạp thuộc lớp C^r và m: X × X → X là một luật hợp thành thuộc lớp C^r trên X. Khi đó T(m) là một luật hợp thành thuộc lớp C^{r-1} trên T(X). Nó được gọi là luật hợp thành tiếp xúc với m. Phép chiếu chính tắc p của T(X) lên X tương thích với các luật m và T(m); nói cách khác,

(5)
$$p \circ T(m) = m \circ (p \times p).$$

Từ (2) suy ra rằng

(6)
$$T(m)(0_x, 0_y) = 0_{m(x, y)}$$

với mọi x, y trong X; nói cách khác, tiết diện không $x ↦ 0_x$ của T(X) tương thích với các luật m và T(m).

#### Mệnh đề 1 {#lie-iii-s2-prop-1 .statement}

*Cho X là một đa tạp thuộc lớp C^r và m là một luật hợp thành thuộc lớp C^r trên X. Nếu m là kết hợp (tương ứng giao hoán), thì T(m) là kết hợp (tương ứng giao hoán).*

Nếu m là kết hợp, thì $m \circ (m \times \mathrm{Id}_X) = m \circ (\mathrm{Id}_X \times m)$, do đó

$$T(m) \circ (T(m) \times \mathrm{Id}_{T(X)}) = T(m) \circ (\mathrm{Id}_{T(X)} \times T(m))$$

và do đó $T(m)$ là kết hợp. Gọi $s$ là ánh xạ $(x, y) \mapsto (y, x)$ của $X \times X$ vào $X \times X$. Nếu $m$ là giao hoán, thì $m \circ s = m$ và do đó

$$
T(m) \circ T(s) = T(m).
$$

Nhưng $T(s)$ là ánh xạ $(u, v) \mapsto (v, u)$ của $T(X) \times T(X)$ vào $T(X) \times T(X)$. Do đó $T(m)$ là giao hoán.

#### Mệnh đề 2 {#lie-iii-s2-prop-2 .statement}

*Cho $X$ là một đa tạp thuộc lớp $C^r$, $m$ là một luật hợp thành thuộc lớp $C^r$ trên $X$ và $e$ là một phần tử đơn vị đối với $m$.

(i) *Vectơ $0_e$ là một phần tử đơn vị đối với $T(m)$.
(ii) *$T_e(X)$ là ổn định đối với $T(m)$ và luật hợp thành cảm sinh trên $T_e(X)$ bởi $T(m)$ là phép cộng của không gian vectơ $T_e(X)$.
(iii) *Cho $U$ là một tập con mở của $X$ và $\alpha$ là một ánh xạ thuộc lớp $C^r$ của $U$ vào $X$ sao cho, với mọi $x \in U$, $\alpha(x)$ là nghịch đảo của $x$ đối với $m$. Khi đó, với mọi $u \in T(U)$, $T(\alpha)u$ là nghịch đảo của $u$ đối với $T(m)$.

Các tính chất (3) và (4) chỉ ra rằng $T(m)(0_e, u) = T(m)(u, 0_e) = u$ với mọi $u \in T(X)$, do đó (i). Với $u, v$ trong $T_e(X)$,

$$
T(m)(u, v) = T(m)(u, 0_e) + T(m)(0_e, v) = u + v,
$$

do đó (ii). Cuối cùng các hệ thức $m(x, \alpha(x)) = m(\alpha(x), x) = e$ với mọi $x \in U$ kéo theo

$$
T(m)(u, T(\alpha)(u)) = T(m)(T(\alpha)u, u) = 0_e
$$

với mọi $u \in T(U)$, do đó (iii).

#### Mệnh đề 3 {#lie-iii-s2-prop-3 .statement}

*Cho $X_1, X_2, \ldots, X_p, Y$ là các đa tạp thuộc lớp $C^r$, $i$ là một số nguyên của $\{1, p\}$, $m_i$ (tương ứng $n$) là một luật hợp thành thuộc lớp $C^r$ trên $X_i$ (tương ứng $Y$) và $u$ là một ánh xạ thuộc lớp $C^r$ từ $X_1 \times X_2 \times \cdots \times X_p$ vào $Y$. Nếu $u$ là phân phối đối với biến có chỉ số $i$, thì $T(u)$ là phân phối đối với biến có chỉ số $i$.

Chứng minh tương tự như chứng minh của Mệnh đề 1.

### 2. NHÓM CÁC VECTƠ TIẾP XÚC CỦA MỘT NHÓM LIE

#### Mệnh đề 4 {#lie-iii-s2-prop-4 .statement}

*Cho $G$ là một nhóm Lie. Khi đó $T(G)$, với luật hợp thành tiếp xúc với phép nhân của $G$, là một nhóm Lie. Phần tử đơn vị của $T(G)$ là vectơ $0_e$.

Điều này suy ra từ các Mệnh đề 1 và 2.

#### Mệnh đề 5 {#lie-iii-s2-prop-5 .statement}

*Cho $G$ và $H$ là các nhóm Lie và $f$ là một cấu xạ từ $G$ vào $H$. Khi đó $T(f)$ là một cấu xạ từ nhóm Lie $T(G)$ vào nhóm Lie $T(H)$.

Ta biết rằng $T(f')$ là giải tích. Mặt khác, gọi $m$ (tương ứng $n$) là phép nhân trên $G$ (tương ứng $H$). Khi đó $f \circ m = n \circ (f \times f)$, do đó

$$
T(f) \circ T(m) = T(n) \circ (T(f) \times T(f)),
$$

điều này biểu thị rằng $T(f)$ là một đồng cấu nhóm.

#### Hệ quả {#lie-iii-s2-n2-cor-1 .statement}

*Cho $G_1, \ldots, G_n$ là các nhóm Lie. Đẳng cấu chính tắc của đa tạp $T(G_1 \times \cdots \times G_n)$ lên đa tạp $T(G_1) \times \cdots \times T(G_n)$ là một đẳng cấu nhóm Lie.*

$\mathrm{pr}_i$ là một cấu xạ từ $G_1 \times \cdots \times G_n$ vào $G_i$ và do đó $T(\mathrm{pr}_i)$ là một cấu xạ từ $T(G_1 \times \cdots \times G_n)$ vào $T(G_i)$.

#### Mệnh đề 6 {#lie-iii-s2-prop-6 .statement}

*Cho $G$ là một nhóm Lie.*
  (i) *Phép chiếu chính tắc $p : T(G) \to G$ là một cấu xạ nhóm Lie.*
  (ii) *Hạt nhân của $p$ là $T_e(G)$. Nó là một nhóm con Lie của $T(G)$. Cấu trúc nhóm Lie cảm sinh trên $T_e(G)$ bởi cấu trúc trên $T(G)$ là cấu trúc nhóm Lie của không gian khả chuẩn đầy đủ $T_e(G)$.*
  (iii) *Tiết diện không $s$ là một đẳng cấu của nhóm Lie $G$ lên một nhóm con Lie $s(G)$ của $T(G)$ (mà nhóm con này ta đồng nhất với $G$).*
  (iv) *Nhóm Lie $T(G)$ là tích nửa trực tiếp của $G$ bởi $T_e(G)$.*

Mệnh đề (i) suy ra từ (5). Mệnh đề (ii) là hiển nhiên khi tính đến Mệnh đề 2 (ii). Các mệnh đề (iii) và (iv) suy ra từ (6) và § 1, Mệnh đề 8.

Cho $u \in T(G)$ và $g \in G$. Theo (3) và (4), các tích $ug, gu$ được tính trong nhóm $T(G)$ là các ảnh của $u$ qua $T(\delta(g^{-1}))$ và $T(\gamma(g))$. Suy ra từ § 1, Hệ quả 2 của Mệnh đề 17 rằng ánh xạ $(g, u) \mapsto gu$ từ $G \times T_e(G)$ vào $T(G)$ là một đẳng cấu của bó vectơ tầm thường $G \times T_e(G)$ với không gian cơ sở $G$ lên bó vectơ $T(G)$. Đẳng cấu nghịch đảo được gọi là *phép tầm thường hóa trái* của $T(G)$. Bằng cách xét ánh xạ $(g, u) \mapsto ug$, *phép tầm thường hóa phải* của $T(G)$ được định nghĩa tương tự.

#### Mệnh đề 7 {#lie-iii-s2-prop-7 .statement}

*Cho $G$ là một nhóm Lie, $M$ là một đa tạp lớp $C^r$ và $f$ và $g$ là các ánh xạ lớp $C^r$ từ $M$ vào $G$, sao cho $fg$ là một ánh xạ lớp $C^r$ từ $M$ vào $G$. Cho $m \in M, x = f(m), y = g(m), u \in T_m(M)$. Khi đó*

$$
(T fg)u = T(f)u.y + x.T(g)u.
$$

Cho $m$ là phép nhân của $G$. Khi đó $fg = m \circ (f, g)$. Bây giờ

$$
T(f, g)(u) = (T(f)u, T(g)u),
$$

do đó $T(fg)u = T(f)u.T(g)u$. Khi đó chỉ cần áp dụng (1) với $f$ được thay bởi $m$.

#### Hệ quả {#lie-iii-s2-n2-cor-2 .statement}

*Cho $n \in \mathbf{Z}$. Ánh xạ tiếp xúc tại $e$ của ánh xạ $g \mapsto g^n$ của $G$ vào $G$ là ánh xạ $x \mapsto nx$ của $T_e(G)$ vào $T_e(G)$.*

Đối với $n \geqslant 0$, điều này suy ra bằng quy nạp theo $n$ từ Mệnh đề 7. Mặt khác, ánh xạ tiếp xúc tại $e$ của ánh xạ $g \mapsto g^{-1}$ là ánh xạ $x \mapsto -x$ (no. 1, Mệnh đề 2).

Cho G là một nhóm Lie, X là một đa tạp lớp C^r và $(g, x) \mapsto gx$ là một luật phép toán trái lớp C^r của G trên X. Lập luận như đối với Mệnh đề 1, ta suy ra một luật phép toán trái lớp C^{r-1} của T(G) trên T(X), mà ta cũng sẽ ký hiệu bởi $(u, v) \mapsto uv$. Đồng nhất G (tương ứng X) với ảnh của tiết diện không của T(G) (tương ứng T(X)), ta thấy theo (6) rằng luật phép toán trái của T(G) trên T(X) mở rộng luật phép toán trái của G trên X. Với mọi $u \in T_g(G)$ và $v \in T_x(X)$, theo (1),

$$
uv = gv + ux.
$$

Nếu $g \in G$ và $v \in T_x(X)$, thì gv, theo (3), là ảnh của v qua ánh xạ tiếp xúc tại x của ánh xạ $y \mapsto gy$ của X vào X. Ánh xạ tiếp xúc này là một đẳng cấu của $T_x(X)$ lên $T_{gx}(X)$. Đặc biệt,

$$
g(v + v') = gv + gv', \quad g(\lambda v) = \lambda(gv) \quad \text{đối với } v, v' \text{ trong } T_x(X), \lambda \in K.
$$

Nếu $x \in X$ và $u \in T_g(G)$, thì ux, theo (4), là ảnh của u qua ánh xạ tiếp xúc tại g của ánh xạ $h \mapsto hx$ của G vào X. Do đó

$$
(u + u')x = ux + u'x, \quad (\lambda u)x = \lambda(ux) \quad \text{đối với } u, u' \text{ trong } T_g(G), \lambda \in K.
$$

Điều trên có thể áp dụng cho trường hợp một nhóm Lie tác động lên chính nó bởi phép tịnh tiến trái (tương ứng phải). Luật phép toán tương ứng của T(G) trên T(G) được xác định bởi phép tịnh tiến trái (tương ứng phải) của nhóm Lie T(G). Vì vậy các công thức (7), (8) và (9) đúng trong T(G).

#### Mệnh đề 8 {#lie-iii-s2-prop-8 .statement}

Cho G_1 và G_2 là các nhóm Lie, X_1 và X_2 là các đa tạp lớp C^r và $f_i$ là một luật phép toán trái lớp C^r của G_i trên X_i ($i = 1, 2$). Cho $\phi$ là một cấu xạ của G_1 vào G_2 và $\psi$ là một $\phi$-cấu xạ của X_1 vào X_2. Khi đó T(\psi) là một T(\phi)-cấu xạ của T(X_1) vào T(X_2).

$f_2 \circ (\phi \times \psi) = \psi \circ f_1$, do đó

$$
T(f_2) \circ (T(\phi) \times T(\psi)) = T(\psi) \circ T(f_1).
$$

Cho G là một nhóm Lie, X là một đa tạp lớp C^r và $(g, x) \mapsto gx$ là một luật phép toán trái lớp C^r của G trên X. Cho I là một tập con mở của K chứa 0 và $\gamma: I \to G$ là một ánh xạ lớp C^r sao cho $\gamma(0) = e$. Cho

$$
a = T_0(\gamma)1 \in T_e(G).
$$

Cho $x \in X$. Sử dụng (4), ax là ảnh qua ánh xạ tiếp xúc của $\lambda \mapsto \gamma(\lambda)x$ của vectơ tiếp xúc 1 của I tại 0. Do đó *trường vectơ* $x \mapsto ax$ trên X *là trường vectơ được xác định bởi ánh xạ* $(\lambda, x) \mapsto \gamma(\lambda)x$ *theo nghĩa của Differentiable and Analytic Manifolds*, R, 8.4.5.

### 3. TRƯỜNG HỢP CỦA MẦM NHÓM

Cho $(G, e, \theta, m)$ là một mầm nhóm Lie và $\Omega$ là tập hợp định nghĩa của m. Khi đó T(\Omega) được đồng nhất với một tập con mở của $T(G) \times T(G)$ và T(m) là một ánh xạ giải tích của $T(\Omega)$ vào $T(G)$. Có thể kiểm tra như trong no. 2 rằng $(T(G), 0_e, T(\theta), T(m))$ là một mầm nhóm Lie. Các phép tích của $G$ và $T(G)$ thường được viết theo dạng nhân. Phép chiếu chính tắc của $T(G)$ lên $G$ là một cấu xạ của các mầm nhóm Lie. Hạn chế của $T_e(m)$ lên $T_e(G)$ là phép cộng không gian vectơ của $T_e(G)$. Tiết diện không của T(G) là một đẳng cấu của mầm nhóm Lie $G$ lên một mầm nhóm con Lie của T(G) mà ta đồng nhất với G. Nếu $f$ là một cấu xạ của $G$ vào một mầm nhóm Lie $H$, thì $T(f): T(G) \to T(H)$ là một cấu xạ của các mầm nhóm Lie.

Ánh xạ $\phi: (g, u) \mapsto gu$ của $G \times T_e(G)$ vào $T(G)$ là một đẳng cấu của bó vectơ tầm thường $G \times T_e(G)$ với không gian cơ sở G lên bó vectơ $T(G)$; vì $\phi$ và $\phi^{-1}$ là giải tích và là các cấu xạ bó vectơ, nên chỉ cần áp dụng *Differentiable and Analytic Manifolds*, R, 7.2.1. (Chứng minh của no. 2 cũng có thể được thích nghi.) Đẳng cấu $\phi^{-1}$ được gọi là phép tầm thường hóa trái của $T(G)$. Đẳng cấu nghịch đảo của ánh xạ $(g, u) \mapsto ug$ được gọi là phép tầm thường hóa phải.

Cho $X$ là một đa tạp lớp $C^r$ và $\psi$ là một mảnh luật của phép toán trái lớp $C^r$ của $G$ trên $X$. Khi đó $T(\psi)$ là một mảnh luật của phép toán trái lớp $C^{r-1}$ của $T(G)$ trên $T(X)$ mở rộng $\psi$. Các công thức (7), (8) và (9) vẫn đúng nếu $gx$ được xác định. Nếu $I$ là một tập con mở của $K$ chứa 0, nếu $\gamma: I \to G$ là một ánh xạ lớp $C^r$ sao cho $\gamma(0) = e$ và nếu $a = T_0(\gamma)1$, trường vectơ $x \mapsto ax$ xác định trên $X$ là trường vectơ được xác định bởi ánh xạ $(\lambda, x) \mapsto \gamma(\lambda)x$ theo nghĩa của *Đa tạp khả vi và giải tích*, R, 8.4.5.
