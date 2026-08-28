---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 4
section_title: Passage from Lie algebras to Lie groups
lang: vi
source: lie-i-iii
pdf_pages: 0297-0315, 0394-0400
extraction: ocr
subsections:
    - "no": 1
      title: PASSAGE FROM LIE ALGEBRA MORPHISMS TO LIE GROUP MORPHISMS
      page: 0
      pdf_page: 297
    - "no": 2
      title: PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS
      page: 0
      pdf_page: 299
    - "no": 3
      title: EXPONENTIAL MAPPINGS
      page: 0
      pdf_page: 302
    - "no": 4
      title: FUNCTORIZATION OF EXPONENTIAL MAPPINGS
      page: 0
      pdf_page: 306
    - "no": 5
      title: STRUCTURE INDUCED ON A SUBGROUP
      page: 0
      pdf_page: 307
    - "no": 6
      title: PRIMITIVES OF DIFFERENTIAL FORMS WITH VALUES IN A LIE ALGEBRA
      page: 0
      pdf_page: 309
    - "no": 7
      title: PASSAGE FROM LAWS OF INFINITESIMAL OPERATION TO LAWS OF OPERATION
      page: 0
      pdf_page: 312
statements: 40
exercises: 8
content_sha256: e7df828f400d76a3b15860f86adea3f888736429cd8516520616f3839854a8d3
translated_from: content/en/lie/III/04_s4_passage_from_lie_algebras_to_lie_groups.md
source_content_sha256: f6119fafd0c50520cc240963bc402a61a2e75894df4eadd672f32edea82dae6f
translation_model: gpt-5-6-mini, gpt-5.4-mini, gpt-5-6, gpt-5-mini
translation_run: translate-vi-cbb0aad0
glossary_version: 34
glossary_terms_sha256: be2124c0fbb974b0ffcc925c62f2d576d23e3c9329680633fa84bdf5084c15dd
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CHUYỂN TỪ CÁC ĐẠI SỐ LIE SANG CÁC NHÓM LIE

Nhắc lại rằng, cho đến hết chương này, K được giả thiết là có đặc số 0.

### 1. CHUYỂN TỪ CÁC ĐỒNG CẤU ĐẠI SỐ LIE SANG CÁC ĐỒNG CẤU NHÓM LIE

#### Bổ đề 1 {#lie-iii-s4-lem-1 .statement}

*Cho G là một mầm nhóm Lie và $\mathfrak{h}$ là một đại số con Lie của $L(G)$ thừa nhận một phần bù tôpô. Hợp của các $g\mathfrak{h}$ (tương ứng $\mathfrak{h}g$) với $g \in G$ là một phân bó vectơ con khả tích của $T(G)$.*

Bằng cách xét phép tầm thường hóa trái của $T(G)$ (\S 2, no. 3), ta thấy ngay lập tức rằng các $g\mathfrak{h}$, với $g \in G$, là các thớ của một phân bó vectơ con E của $T(G)$. Cho $g \in G$. Tập hợp các $(L_a)_g$, trong đó $a \in \mathfrak{h}$, bằng $g\mathfrak{h}$. Bây giờ, nếu $a$ và $b$ thuộc $\mathfrak{h}$, thì $[L_a, L_b] = L_{[a, b]}$ và $[a, b] \in \mathfrak{h}$. Do đó E là khả tích (*Differentiable and Analytic Manifolds*, R, 9.3.3 (iv)). Lập luận tương tự đối với các $\mathfrak{h}g$.

Phân lá nguyên (*Differentiable and Analytic Manifolds*, R, 9.3.2) của hợp các $g\mathfrak{h}$ (tương ứng $\mathfrak{h}g$) được gọi là *phân lá* *trái* (tương ứng *phải*) của G liên kết với $\mathfrak{h}$.

#### Định lý 1 {#lie-iii-s4-thm-1 .statement}

*Cho G và H là các mầm nhóm Lie và f là một cấu xạ liên tục của $L(G)$ vào $L(H)$.
(i) Tồn tại một mầm nhóm con Lie mở $G'$ của G và một cấu xạ $\phi$ của $G'$ vào H sao cho $f = L(\phi)$.
(ii) Cho $G_1, G_2$ là các mầm nhóm con Lie mở của G và $\phi_i$ là một cấu xạ của $G_i$ vào H sao cho $f = L(\phi_i)$ với $i = 1, 2$. Khi đó $\phi_1$ và $\phi_2$ trùng nhau trên một lân cận của e.

Cho $p_1 : G \times H \to G, p_2 : G \times H \to H$ là các phép chiếu chính tắc. Với mọi $(g, h) \in G \times H$, ký hiệu $f_{g, h}$ là ánh xạ $ga \mapsto hf(a)$ của $T_g(G) = gL(G)$ vào $T_h(H) = hL(H)$. Xét các phép tầm thường hóa trái của $T(G)$ và $T(H)$, ta thấy ngay rằng các $f_{g, h}$ định nghĩa một cấu xạ từ $p_1^*T(G)$ vào* $p_2^*T(H)$. Gọi $a$ là đồ thị của $f$; đó là một đại số con Lie đóng của $L(G) \times L(H)$ và nhận $\{0\} \times L(H)$ làm phần bù tôpô. Với mọi $(g, h) \in G \times H$, đồ thị của $f_{g,h}$ là $(g, h) \cdot a$. Hợp của các đồ thị này là một phân thớ con vectơ khả tích của $T(G \times H)$ (Bổ đề 1). Khi đó tồn tại (Differentiable and Analytic Manifolds, R, 9.3.7) một lân cận mở $U$ của $e_G$ trong $G$ và một ánh xạ giải tích $\phi$ từ $U$ vào $H$ sao cho $\phi(e_G) = e_H$ và $T_g(\phi) = f_{g, \phi(g)}$ với mọi $g \in U$. Đặc biệt, $T_{e_G}(\phi) = f$.

Cho $V$ là một lân cận mở của $e_G$ trong $G$ sao cho, với $(s, t) \in V \times V$, các tích $st$ và $\phi(s)\phi(t)$ được xác định và $st \in U$. Xét các ánh xạ $\alpha_1, \alpha_2$ từ $V \times V$ vào $H$ được định nghĩa bởi

$$
\alpha_1(s, t) = \phi(ts), \quad \alpha_2(s, t) = \phi(t)\phi(s).
$$

Sau đó $\alpha_1(t, e) = \phi(t) = \alpha_2(t, e)$. Mặt khác, cố định $t$ trong $V$ và gọi $\beta_i$ là ánh xạ $s \mapsto \alpha_i(s, t)$ của $V$ vào $H$. Khi đó, với mọi $s \in V$ và mọi $a \in L(G)$,

$$
\begin{align*}
T_s(\beta_1)(sa) &= T_{ts}(\phi)(tsa) = f_{ts, \phi(ts)}(tsa) \\
&= \phi(ts)f(a) = f_{s, \beta_1(s)}(sa) \\
T_s(\beta_2)(sa) &= \phi(t)T_s(\phi)(sa) = \phi(t)f_{s, \phi(s)}(sa) \\
&= \phi(t)\phi(s)f(a) = f_{s, \beta_2(s)}(sa).
\end{align*}
$$

Do đó (Differentiable and Analytic Manifolds, R, 9.3.7) $\alpha_1$ và $\alpha_2$ trùng nhau trên một lân cận của $(e_G, e_G)$. Hạn chế của $\phi$ lên một lân cận mở đối xứng đủ nhỏ của $e_G$ vì thế là một cấu xạ của các mầm nhóm Lie, do đó (i).

Cho $G_1, G_2, \phi_1, \phi_2$ như trong (ii) và ta chứng minh rằng $\phi_1, \phi_2$ trùng nhau trên một lân cận của $e_G$. Tồn tại một lân cận mở $W$ của $e_G$ sao cho $\phi_1(ts) = \phi_1(t)\phi_1(s)$, $\phi_2(ts) = \phi_2(t)\phi_2(s)$ với mọi $s, t$ trong $W$. Khi đó, nếu $s \in W$ và $a \in L(G)$,

$$
T_s(\phi_i)(sa) = \phi_i(s)T_e(\phi_i)(a) = \phi_i(s)f(a) = f_{s, \phi_i(s)}(sa)
$$

với $i = 1, 2$. Vì $\phi_1(e_G) = e_H = \phi_2(e_G)$, suy ra từ Differentiable and Analytic Manifolds, R, 9.3.7 rằng $\phi_1$ và $\phi_2$ trùng nhau trên một lân cận của $e_G$.

#### Hệ quả 1 {#lie-iii-s4-thm-1-cor-1 .statement}

Cho $G$ và $H$ là hai mầm nhóm Lie. Nếu $L(G)$ và $L(H)$ đẳng cấu, thì $G$ và $H$ địa phương đẳng cấu.

Điều này suy ra từ Định lý 1 và § 1, no. 10, Mệnh đề 21.

#### Hệ quả 2 {#lie-iii-s4-thm-1-cor-2 .statement}

Cho $G$ là một mầm nhóm Lie. Nếu $L(G)$ giao hoán, thì $G$ địa phương đẳng cấu với nhóm Lie cộng tính $L(G)$.

Đại số Lie của nhóm cộng $L(G)$ đẳng cấu với $L(G)$. Do đó chỉ cần áp dụng Hệ quả 1.

#### Hệ quả 3 {#lie-iii-s4-thm-1-cor-3 .statement}

Cho $G$ là một nhóm Lie. Nếu $L(G)$ giao hoán, thì $G$ chứa một nhóm con mở giao hoán.

Tồn tại một mầm nhóm con Lie mở U của G giao hoán (Hệ quả 2). Cho V là một lân cận của e sao cho V^2 ⊂ U. Khi đó xy = yx với mọi x, y trong V. Do đó nhóm con của G sinh bởi V là giao hoán; hiển nhiên nó là mở.

### 2. CHUYỂN TỪ CÁC ĐẠI SỐ LIE SANG CÁC NHÓM LIE

Ta sẽ ký hiệu chuỗi Hausdorff bởi H(X, Y) (Chương II, § 6, no. 4, Định nghĩa 1).

#### Bổ đề 2 {#lie-iii-s4-lem-2 .statement}

Cho L là một đại số Lie chuẩn đầy đủ trên $\mathbf{R}$ hoặc $\mathbf{C}$. Cho G là tập hợp các $x \in L$ sao cho $\|x\| < \frac{1}{3} \log \frac{3}{2}$. Cho $\theta$ là ánh xạ $x \mapsto -x$ của G vào G. Cho H là hạn chế vào $G \times G$ của hàm Hausdorff của L (Chương II, § 7, no. 2).
(i) $(G, 0, \theta, H)$ là một mầm nhóm Lie.
(ii) Cho $\phi$ là ánh xạ đồng nhất của G vào L. Vi phân của $\phi$ tại 0 là một đẳng cấu của đại số Lie chuẩn được $L(G)$ lên L.
(i) suy ra từ Chương II, § 7, no. 2.
Vì $\phi$ là một bản đồ tọa độ trên G, vi phân $\psi$ của $\phi$ tại 0 là một đẳng cấu của các không gian chuẩn. Mặt khác, khai triển thành chuỗi nguyên $H = \sum_{i,j \geq 0} H_{ij}$ của ánh xạ H có tính chất $H_{11}(x, y) = \frac{1}{2}[x, y]$. Theo § 3, Mệnh đề 24, với mọi $a, b$ trong $L(G)$,
$$
\psi([a, b]) = H_{11}(\psi(a), \psi(b)) - H_{11}(\psi(b), \psi(a)) = [\psi(a), \psi(b)]
$$
điều này chứng minh (ii).

G được gọi là *mầm nhóm Lie xác định bởi L*.

Giả sử K là ultramêtric. Cho $p$ là đặc số của trường thặng dư của K. Nếu $p \neq 0$, cho $\lambda = |p|^{1/(p-1)}$; nếu $p = 0$, cho $\lambda = 1$.

#### Bổ đề 3 {#lie-iii-s4-lem-3 .statement}

Cho L là một đại số Lie chuẩn đầy đủ trên K. Cho G là tập hợp các $x \in L$ sao cho $\|x\| < \lambda$. Cho $H : G \times G \to G$ là hàm Hausdorff của L (Chương II, § 8, no. 3).
(i) Với luật hợp thành H, G là một nhóm Lie trong đó 0 là phần tử đơn vị và $-x$ là nghịch đảo của x với mọi $x \in G$.
(ii) Cho $\phi$ là ánh xạ đồng nhất của G vào L. Vi phân của $\phi$ tại 0 là một đẳng cấu của đại số Lie chuẩn $L(G)$ lên L.
(iii) Với mọi $\mu \in \mathbf{R}_+^*$, cho $G_\mu$ là tập hợp các $x \in L$ sao cho $\|x\| < \mu$. Khi đó các $G_\mu$, với $\mu < \lambda$, tạo thành một hệ cơ bản các lân cận mở và đóng của 0 và là các nhóm con của G.
Các mệnh đề (i) và (iii) suy ra từ Chương II, § 8, no. 3, Mệnh đề 3 và (ii) có thể được chứng minh như trong Bổ đề 2.

G được gọi là *nhóm Lie xác định bởi L*.

#### Định lý 2 {#lie-iii-s4-thm-2 .statement}

Cho L là một đại số Lie chuẩn hóa được đầy đủ. Tồn tại một mầm nhóm Lie G sao cho L(G) đẳng cấu với L. Hai mầm nhóm Lie như vậy đẳng cấu địa phương.

Mệnh đề thứ nhất suy ra từ các Bổ đề 2 và 3. Mệnh đề thứ hai suy ra từ Hệ quả 1 của Định lý 1 của no. 1.

#### Hệ quả 1 {#lie-iii-s4-thm-2-cor-1 .statement}

Cho G là một nhóm Lie. Tồn tại một lân cận của e không chứa nhóm con hữu hạn nào phân biệt với {e}. Nếu K = R hoặc C, tồn tại một lân cận mở của e không chứa nhóm con nào phân biệt với {e}.

Ta viết L(G) = L. Chọn một chuẩn trên L xác định tôpô trên L và sao cho $\| [x, y] \| \leq \| x \| \| y \|$ với mọi x, y trong L.

Giả sử K = R hoặc C. Cho G' là mầm nhóm Lie được xác định bởi L. Tồn tại một quả cầu mở U' có tâm 0 trong G' và một đẳng cấu $\phi$ của mầm nhóm Lie U' lên một lân cận mở U của e trong G. Cho V' = $\frac{1}{2} U'$, $V = \phi(V')$, H là một nhóm con của G được chứa trong V và $h \in H$. Cho $x = \phi^{-1}(h) \in V'$. Nếu $x \neq 0$, tồn tại một số nguyên $n > 0$ sao cho $x, 2x, \ldots, nx$ thuộc V', $(n+1)x \in U'$, $(n+1)x \notin V'$. Khi đó $h, h^2, \ldots, h^n$ thuộc V,

$$
h^{n+1} \in U, \qquad h^{n+1} \notin V,
$$

là điều vô lý. Do đó H = {e}.

Giả sử K là ultramêtric. Chỉ cần chứng minh hệ quả khi G là nhóm Lie liên kết với L. Nếu $g \in G$, các lũy thừa của g được tính trong G là các phần tử của $\mathbf{Z}g$ được tính trong L. Các phần tử này phân biệt nếu $g \neq e$. Do đó G không chứa nhóm con hữu hạn nào phân biệt với {e}.

#### Hệ quả 2 {#lie-iii-s4-thm-2-cor-2 .statement}

Cho k là một trường con đóng không rời rạc của K, G là một nhóm Lie trên k và L = L(G). Giả sử rằng L có một cấu trúc đại số Lie K chuẩn hóa được L', tương thích với cấu trúc đại số Lie k chuẩn hóa được và bất biến dưới biểu diễn phụ hợp của G. Khi đó trên G tồn tại duy nhất một cấu trúc nhóm Lie K tương thích với cấu trúc nhóm Lie k và có đại số Lie là L'.

Tồn tại một mầm nhóm Lie $G_1$ trên K sao cho $L(G_1) = L'$ (Định lý 2). Theo Hệ quả 1 của Định lý 1 ở no. 1, G và $G_1$, được xem như các mầm nhóm Lie-k, là đẳng cấu địa phương. Do đó tồn tại một lân cận mở G' của e trong G và một cấu trúc mầm nhóm Lie-K trên G', với đại số Lie L, tương thích với cấu trúc mầm nhóm Lie trên k. Gọi V là một lân cận mở đối xứng của e trong G sao cho $V^2 \subset G'$. Cho $g \in G$. Khi đó $\phi = \operatorname{Int} g$ là một đẳng cấu-k của một mầm nhóm con Lie mở đủ nhỏ của G' lên một mầm nhóm con Lie mở của G'; và $T_e(\phi)$ là K-tuyến tính, do đó $T_x(\phi)$ là K-tuyến tính với x đủ gần e; vì vậy hạn chế của Int g vào một lân cận mở đủ nhỏ của e trong V là K-giải tích (Các đa tạp khả vi và giải tích, R, 5.14.6). Theo § 1, no. 9, Mệnh đề 18, tồn tại trên G một cấu trúc đa tạp K-giải tích sao cho G là một

nhóm K-Lie và V là một đa tạp con-K mở của G. Bằng phép tịnh tiến, thấy rằng cấu trúc đa tạp-k cơ sở của G là cấu trúc đã cho. Đại số Lie của nhóm Lie-K G là cùng một đại số với đại số của mầm nhóm con Lie-K mở V và do đó là L'. Cuối cùng, tính duy nhất được nêu trong hệ quả suy ra từ § 3, no. 8, Mệnh đề 32.

#### Định lý 3 {#lie-iii-s4-thm-3 .statement}

Cho G là một mầm nhóm Lie và $\mathfrak{h}$ là một đại số con Lie của $L(G)$ thừa nhận một phần bù tôpô. Tồn tại một mầm nhóm con Lie H của G sao cho $L(H) = \mathfrak{h}$. Nếu $H_1$ và $H_2$ là các mầm nhóm con Lie của G sao cho

$$
L(H_1) = L(H_2) = \mathfrak{h},
$$

thì $H_1 \cap H_2$ là mở trong $H_1$ và $H_2$.

Tồn tại một mầm nhóm Lie $H'$ có đại số Lie đẳng cấu với $\mathfrak{h}$ (Định lý 2). Nếu cần thiết thu nhỏ $H'$, có thể giả sử rằng tồn tại một cấu xạ $\phi$ từ $H'$ vào G sao cho $L(\phi)$ là một đẳng cấu của $L(H')$ lên $\mathfrak{h}$ (no. 1, Định lý 1). Vì $\mathfrak{h}$ thừa nhận một phần bù tôpô, $\phi$ là một phép nhúng tại e. Do đó, nếu thu nhỏ thêm $H'$, có thể giả sử rằng $\phi$ là một đẳng cấu của đa tạp $H'$ lên một đa tạp con của G. Điều này chứng minh sự tồn tại của H. Mệnh đề thứ hai suy ra từ mệnh đề sau:

#### Mệnh đề 1 {#lie-iii-s4-prop-1 .statement}

Cho G là một mầm nhóm Lie và H và $H'$ là hai mầm nhóm con Lie. Để $L(H) \supset L(H')$, điều kiện cần và đủ là $H \cap H'$ mở trong $H'$.

Nếu $H \cap H'$ là mở trong $H'$, thì $L(H') = L(H \cap H') \subset L(H)$. Giả sử rằng $L(H) \supset L(H')$. Gọi i, $i'$ là các đơn ánh chính tắc của H, $H'$ vào G. Bằng cách thu nhỏ $H'$ nếu cần thiết, có thể giả sử rằng tồn tại một cấu xạ $\psi$ từ $H'$ vào H sao cho $L(\psi)$ là đơn ánh chính tắc của $L(H')$ vào $L(H)$ (no. 1, Định lý 1). Khi đó $L(i \circ \psi) = L(i')$ và do đó tồn tại một lân cận V của $e_{H'}$ trong $H'$ sao cho $i \circ \psi$ và $i'$ trùng nhau trên V (Định lý 1). Vì vậy $V \subset H$, do đó $V \subset H \cap H'$ và $H \cap H'$ là mở trong $H'$ (\S 1, no. 10).

#### Mệnh đề 2 {#lie-iii-s4-prop-2 .statement}

Cho G là một nhóm Lie trên K, k là một trường con đóng không rời rạc của K và H là một nhóm con Lie của nhóm Lie-k G. Giả sử rằng $L(H)$ là một không gian con-K vectơ của $L(G)$ thừa nhận một phần bù tôpô. Khi đó H là một nhóm con Lie của nhóm Lie-K G.

Tồn tại một mầm nhóm con Lie $H'$ của nhóm Lie K G sao cho $L(H') = L(H)$ (Định lý 3). Xét G, H, $H'$ như các mầm nhóm Lie k; khi đó Định lý 3 chứng minh rằng $H \cap H'$ là mở trong H và $H'$. Do đó tồn tại một lân cận mở U của e trong G sao cho $U \cap H$ là một đa tạp con của G trên K. Vì vậy, H là một nhóm con Lie của nhóm Lie K G (\S 1, no. 3, Mệnh đề 6).

### 3. ÁNH XẠ MŨ

#### Định lý 4 {#lie-iii-s4-thm-4 .statement}

Cho G là một mầm nhóm Lie, L là đại số Lie của nó, V là một lân cận mở của 0 trong L, φ là một ánh xạ giải tích từ V vào G sao cho φ(0) = 0 và T_0(φ) = Id_L. Các điều kiện sau là tương đương:
(i) Với mọi b ∈ L, φ((λ + λ')b) = φ(λb)φ(λ'b) với |λ| và |λ'| đủ nhỏ.
(ii) Với mọi b ∈ L và mọi số nguyên n > 0, φ_*(b^n) là thuần nhất bậc n trong U(G) (T_0^{(∞)}(L) được đồng nhất với TS(L) và b^n được tính trong TS(L)).
(iii) Ánh xạ φ_* của TS(L) vào U(G) tương thích với các phép phân bậc của TS(L) và U(G).
(iv) Ánh xạ φ_* của TS(L) vào U(G) là ánh xạ chính tắc của TS(L) vào đại số bao của L.
(v) Tồn tại một chuẩn trên L xác định tôpô của L và sao cho
$$
\|[x, y]\| \leq \|x\|\|y\|
$$
với mọi x, y trong L và một mầm nhóm con mở W ⊂ V của mầm nhóm Lie xác định bởi L (no. 2) sao cho φ|W là một đẳng cấu của W lên một mầm nhóm con Lie mở của G.

(v) ⇒ (i): hiển nhiên, vì (λb).(λ'b) = (λ + λ')b trong W với |λ| và |λ'| đủ nhỏ.
(i) ⇒ (ii): giả sử rằng điều kiện (i) được thỏa mãn. Cho b ∈ L. Gọi ψ là hạn chế của φ vào V ∩ Kb. Theo giả thiết, tồn tại một lân cận đối xứng T của 0 trong nhóm Lie cộng tính Kb sao cho ψ|T là một cấu xạ của mầm nhóm Lie T vào G. Do đó
$$
φ_*(b^n) = (ψ|T)_*(b^n) = ((ψ|T)_*(b))^n = (φ_*(b))^n,
$$
suy ra φ_*(b^n) là thuần nhất bậc n trong U(G).
(ii) ⇒ (iii): điều này suy ra từ sự kiện rằng TS^n(L) là không gian con vectơ của TS(L) sinh bởi các lũy thừa bậc n của các phần tử của L (Đại số, Chương IV, § 5, Mệnh đề 5).
(iii) ⇒ (iv): ánh xạ chính tắc của TS(L) vào đại số bao của L là cấu xạ duy nhất của các đối đại số phân bậc biến 1 thành 1 và mở rộng Id_L (Chương II, § 1, no. 5, Nhận xét 3). Bây giờ φ_* là một cấu xạ đối đại số và φ_*|L = Id_L theo giả thiết. Nếu điều kiện (iii) đúng, ta thấy rằng điều kiện (iv) cũng đúng.
(iv) ⇒ (v): giả sử rằng điều kiện (iv) được thỏa mãn. Chọn một chuẩn trên L xác định tôpô của L và sao cho \|[x, y]\| \leq \|x\|\|y\| với mọi x, y trong L. Gọi H là mầm nhóm Lie được xác định bởi đại số Lie chuẩn hóa L. Theo Định lý 1, tồn tại một mầm nhóm con mở S ⊂ V của H và một đẳng cấu φ' của S lên một mầm nhóm con mở của G. Như ta đã biết rằng (v) ⇒ (iv), ánh xạ φ_* của TS(L) vào U(G) là ánh xạ chính tắc của TS(L) vào đại số bao của L. Do đó φ_*(t) = φ'_*(t) với mọi t ∈ T_0^{(∞)}(L). Vì φ và φ' là giải tích, φ và φ' trùng nhau trên một lân cận của 0.

#### Định nghĩa 1 {#lie-iii-s4-def-1 .statement}

Cho G là một mầm nhóm Lie và L là đại số Lie của nó. Một ánh xạ mũ của G là bất kỳ ánh xạ giải tích $\phi$ nào được xác định trên một lân cận mở của 0 trong L, có giá trị trong G và thỏa mãn các điều kiện của Định lý 4.

Định lý 4 suy ra ngay lập tức rằng, với mọi mầm nhóm Lie G, tồn tại một ánh xạ mũ của G và hai ánh xạ mũ của G trùng nhau trên một lân cận của 0.

#### Ví dụ {#lie-iii-s4-n3-exa-1 .statement}

(1) Cho G là nhóm cộng của một không gian chuẩn hóa đầy đủ E. Đẳng cấu chính tắc của L(G) lên E thỏa mãn điều kiện (i) của Định lý 4 và do đó là một ánh xạ mũ của G.

(2) Cho A là một đại số kết hợp có đơn vị chuẩn đầy đủ. Gọi A* là nhóm Lie gồm các phần tử khả nghịch của A. Ta đồng nhất L(A*) với A (\$ 3, no. 9, Hệ quả của Mệnh đề 33). Nếu K = \mathbf{R} hoặc \mathbf{C}, ta biết rằng ánh xạ exp của A vào A* được định nghĩa trong Chương II, \$ 7, no. 3 thỏa mãn điều kiện (i) của Định lý 4 và do đó là một ánh xạ mũ. Bây giờ cho K là ultrametric. Gọi $p$ là đặc số của trường thặng dư của K. Nếu $p \neq 0$, đặt $\lambda = |p|^{1/(p-1)}$; nếu $p = 0$, đặt $\lambda = 1$. Gọi U là tập hợp các $x \in A$ sao cho $\|x\| < \lambda$. Ta biết (Chương II, \$ 8, no. 4) rằng ánh xạ exp của U vào A* thỏa mãn điều kiện (i) của Định lý 4 và do đó là một ánh xạ mũ. Chú ý rằng U là một nhóm con cộng tính của A.

Ví dụ này giải thích thuật ngữ được dùng trong Định nghĩa 1.

Cho G là một mầm nhóm Lie và $\phi$ là một ánh xạ mũ của G. Khi đó $\phi$ là étale tại 0 và do đó tồn tại một lân cận mở U của 0 trong L(G) sao cho $\phi(U)$ là mở trong G và $\phi|U$ là một đẳng cấu của đa tạp giải tích U lên đa tạp giải tích $\phi(U)$.

Một biểu đồ chính tắc (loài thứ nhất) trên G là một biểu đồ $\psi$ trên đa tạp giải tích G mà ánh xạ nghịch đảo của nó là một ánh xạ mũ. Nếu thêm nữa G là hữu hạn chiều và một cơ sở của L(G) được chọn, hệ tọa độ được xác định bởi $\psi$ và cơ sở này trong miền của $\psi$ được gọi là một hệ tọa độ chính tắc (loài thứ nhất).

#### Mệnh đề 3 {#lie-iii-s4-prop-3 .statement}

Cho G là một mầm nhóm Lie, L là đại số Lie của nó và $\phi$ là một ánh xạ mũ của G. Cho $L_1, \ldots, L_n$ là các không gian con vectơ của L sao cho L là tổng trực tiếp tôpô của $L_1, \ldots, L_n$. Ánh xạ

$$
(b_1, b_2, \ldots, b_n) \mapsto \theta(b_1, b_2, \ldots, b_n) = \phi(b_1)\phi(b_2)\cdots\phi(b_n),
$$

được xác định trên một tập con mở của $L_1 \times L_2 \times \cdots \times L_n$, là giải tích. Ánh xạ tiếp tuyến tại $(0, 0, \ldots, 0)$ của $\theta$ là ánh xạ chính tắc của $L_1 \times \cdots \times L_n$ vào L.

Cho $k_i$ là đơn ánh chính tắc của $L_i$ vào $L_1 \times L_2 \times \cdots \times L_n$. Khi đó, với mọi $b \in L_i$, $(T_{(0, \ldots, 0)}\theta)(T_0k_i)(b) = (T_0\phi)(b) = b$ và do đó $(T_{(0, \ldots, 0)}\theta)|L_i$ là đơn ánh chính tắc của $L_i$ vào L.

Đặc biệt, $\theta$ là étale tại $(0, 0, \ldots, 0)$. Hạn chế của nó lên một

NHÓM LIE

lân cận mở đủ nhỏ U của $(0, 0, \ldots, 0)$ có ảnh mở trong G và là một đẳng cấu của đa tạp U lên đa tạp $\theta(U)$. Ánh xạ nghịch đảo $\eta$ của $\theta(U)$ lên U được gọi là một *biểu đồ chính tắc của loài thứ hai* của G, liên kết với phân tích đã cho của L thành một tổng trực tiếp. Nếu thêm nữa G là hữu hạn chiều và mỗi $L_i$ được sinh bởi một vectơ khác không $e_i$, hệ tọa độ trên $\theta(U)$ được xác định bởi $\eta$ và các $e_i$ được gọi là một *hệ tọa độ chính tắc của loài thứ hai*.

#### Mệnh đề 4 {#lie-iii-s4-prop-4 .statement}

*Cho G là một mầm nhóm Lie và $\phi$ là một ánh xạ mũ đơn ánh của G. Với mọi x, y trong $L(G)$,*

(1)
$$
x + y = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))
$$
(2)
$$
[x, y] = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-2} \phi^{-1}(\phi(\lambda x) \phi(\lambda y) \phi(-\lambda x) \phi(-\lambda y))
$$
(chú ý rằng $\phi^{-1}(\phi(\lambda x) \phi(\lambda y))$ và $\phi^{-1}(\phi(\lambda x) \phi(\lambda y) \phi(-\lambda x) \phi(-\lambda y))$ được xác định với $|\lambda|$ đủ nhỏ).

Cho $L = L(G)$ được trang bị một chuẩn xác định tôpô của L và sao cho $\| [x, y] \| \leq \| x \| \| y \|$ với mọi $x, y$ trong L. Dùng các Định lý 2 và 4, có thể giả sử rằng G là mầm nhóm Lie được xác định bởi L và rằng $\phi = \mathrm{Id}_G$. Ký hiệu $(x, y) \mapsto x \cdot y$ là tích trong nhóm G. Các công thức cần chứng minh khi đó có thể được viết
(3)
$$
x + y = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1}((\lambda x) \cdot (\lambda y))
$$
(4)
$$
[x, y] = \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-2}((\lambda x) \cdot (\lambda y) \cdot (-\lambda x) \cdot (-\lambda y)).
$$

Tồn tại một lân cận mở V của 0 trong K sao cho hàm
$$
\lambda \mapsto f(\lambda) = (\lambda x) \cdot (\lambda y)
$$
được xác định và giải tích trên V. Theo Chương II, § 6, no. 4, *Nhận xét 2*, khai triển của $f$ thành một chuỗi nguyên quanh gốc là
$$
\lambda(x + y) + \frac{1}{2} \lambda^2 [x, y] + \cdots
$$
và điều này chứng minh (3). Mặt khác, với $u, v$ trong G và $\|u\|, \|v\|$ đủ nhỏ, $u \cdot v$ là một hàm giải tích của $(u, v)$ và các số hạng bậc 1 và 2 trong khai triển của hàm này thành một chuỗi nguyên quanh gốc là $u + v + \frac{1}{2}[u, v]$. Theo *Các đa tạp khả vi và giải tích*, R, 3.2.7 và 4.2.3, các số hạng bậc 1 và 2 trong khai triển của hàm $f(\lambda) \cdot f(-\lambda)$ thành một chuỗi nguyên quanh gốc là các số hạng bậc 1 và 2 trong
$$
f(\lambda) + f(-\lambda) + \frac{1}{2}[f(\lambda), f(-\lambda)]
$$
hoặc cũng trong
$$
\lambda(x + y) + \frac{1}{2} \lambda^2 [x, y] - \lambda(x + y) + \frac{1}{2} \lambda^2 [x, y] \\
+ \frac{1}{2} [\lambda(x + y), -\lambda(x + y)] = \lambda^2 [x, y]
$$
và điều này chứng minh (4).

Ánh xạ mũ

§ 4.3

#### Mệnh đề 5 {#lie-iii-s4-prop-5 .statement}

Cho G là một nhóm Lie, k là một trường con đóng không rời rạc của K, G' là nhóm G được xem như một nhóm Lie trên k và $\phi$ (resp. $\phi'$) là một ánh xạ mũ của G (resp. G'). Khi đó $\phi$ và $\phi'$ trùng nhau trên một lân cận của 0.

$\phi$ thỏa mãn giả thiết (i) của Định lý 4 đối với G' và do đó là một ánh xạ mũ của G'.

#### Mệnh đề 6 {#lie-iii-s4-prop-6 .statement}

Cho G là một mầm nhóm Lie, L là đại số Lie của nó và $\phi : V \to G$ là một ánh xạ mũ của G. Với mọi $x \in V$, cho $T_x(L)$ được đồng nhất với L, sao cho vi phân phải $\varpi(x)$ của $\phi$ tại x là một ánh xạ tuyến tính của L vào L. Với x đủ gần 0,

$$
\varpi(x) = \sum_{n \geq 0} \frac{1}{(n+1)!} (\operatorname{ad} x)^n.
$$

Cho L được trang bị một chuẩn tương thích với tôpô của nó và sao cho $\| [x, y] \| \leq \| x \| \| y \|$ với mọi $x, y \in L$. Chỉ cần xét trường hợp G là mầm nhóm Lie được xác định bởi L và $\phi = \operatorname{Id}_G$. Theo định nghĩa, $\varpi(x)$ khi đó là ánh xạ tiếp xúc tại x của ánh xạ $y \mapsto y . x^{-1}$ của G vào G. Nếu $H(X, Y)$ ký hiệu chuỗi Hausdorff, thì $\varpi(x)$ do đó, với $\| x \|$ đủ nhỏ, là ánh xạ tiếp xúc tại 0 của ánh xạ $y \mapsto H(x, +y, -x)$ của G vào G. Trong $H(X + Y, -X)$, tổng các số hạng bậc thứ nhất theo Y là

$$
\sum_{m \geq 0} \frac{1}{(m+1)!} (\operatorname{ad} X)^m Y
$$

(Chương II, § 6, no. 5, Mệnh đề 5). Mệnh đề sau đó suy ra từ Các đa tạp khả vi và giải tích, R, 3.2.4 và 4.2.3.

Cho G là một mầm nhóm Lie và $t \in K$. Một *ánh xạ lũy thừa bậc t của G* là bất kỳ ánh xạ nào, được xác định và giải tích trên một lân cận mở của e, có giá trị trong G và trùng nhau trên một lân cận của e với một ánh xạ

$$
g \mapsto \phi(t \phi^{-1}(g))
$$

trong đó $\phi$ là một ánh xạ mũ đơn ánh của G.

#### Mệnh đề 7 {#lie-iii-s4-prop-7 .statement}

(i) *Nếu $t \in \mathbf{Z}$, một ánh xạ lũy thừa bậc t trùng nhau trên một lân cận của e với ánh xạ $g \mapsto g^t$.*

(ii) *Ánh xạ tiếp xúc tại e của một ánh xạ lũy thừa bậc t là phép vị tự với tỉ số t.*

(iii) *Nếu h là một ánh xạ lũy thừa bậc t và h' là một ánh xạ lũy thừa bậc t' của G, $h \circ h'$ là một ánh xạ lũy thừa bậc (tt') và $g \mapsto h(g)h'(g)$ là một ánh xạ lũy thừa bậc (t + t').*

(iv) *Nếu h là một ánh xạ lũy thừa bậc t và $u \in U^n(G)$, thì $h_*(u) = t^n u$.*

Chỉ cần chứng minh mệnh đề trong trường hợp G là mầm nhóm Lie được xác định bởi một đại số Lie chuẩn đầy đủ và các ánh xạ lũy thừa bậc t được xét được xây dựng bằng ánh xạ mũ $\phi = \operatorname{Id}_G$. Nhưng trong trường hợp đó mọi thứ là hiển nhiên.

### 4. HÀM TỬ HÓA CÁC ÁNH XẠ MŨ

#### Mệnh đề 8 {#lie-iii-s4-prop-8 .statement}

Cho G và H là các mầm nhóm Lie, h là một cấu xạ từ G vào H và $\phi_G$ và $\phi_H$ là các ánh xạ mũ của G và H. Tồn tại một lân cận V của 0 trong $L(G)$ sao cho $h \circ \phi_G$ và $\phi_H \circ L(h)$ trùng nhau trên V.

Cho $L(G)$ và $L(H)$ được trang bị các chuẩn xác định các tôpô của chúng và sao cho $\| [x, y] \| \leq \| x \| \| y \|$ với mọi x và y. Có thể giả sử rằng G (tương ứng H) là mầm nhóm Lie được xác định bởi $L(G)$ (tương ứng $L(H)$), sao cho $\phi_G$ (tương ứng $\phi_H$) trùng với $\mathrm{Id}_G$ (tương ứng $\mathrm{Id}_H$) trong một lân cận của 0. Mặt khác, tồn tại một lân cận mở đối xứng W của 0 trong $L(G)$ sao cho $L(h)$ là một cấu xạ của mầm nhóm Lie W vào H. Theo Định lý 1, $L(h)$ trùng với h trên một lân cận của 0, do đó có mệnh đề.

Nói một cách không chặt chẽ, nếu G và H được đồng nhất trong một lân cận của phần tử đơn vị với $L(G)$ và $L(H)$ bằng các ánh xạ mũ, thì mọi cấu xạ từ G vào H là *tuyến tính* trong một lân cận của 0.

#### Hệ quả 1 {#lie-iii-s4-prop-8-cor-1 .statement}

Cho G là một mầm nhóm Lie, G' là một mầm nhóm con Lie của G và $\phi$ là một ánh xạ mũ của G.

(i) Tồn tại một lân cận mở V của 0 trong $L(G')$ sao cho $\phi|V$ là một đẳng cấu của đa tạp V lên một lân cận mở của e trong G'.

(ii) Cho $x \in L(G)$. Các điều kiện sau là tương đương: (a) $x \in L(G')$; (b) $\phi(\lambda x) \in G'$ với $|\lambda|$ đủ nhỏ.

(i) thu được bằng cách áp dụng Mệnh đề 8 cho đơn ánh chính tắc của G' vào G và (ii) suy ra từ (i).

#### Hệ quả 2 {#lie-iii-s4-prop-8-cor-2 .statement}

Cho G là một nhóm Lie, $\rho$ là một biểu diễn tuyến tính giải tích của G và $\phi$ là một ánh xạ mũ của G. Tồn tại một lân cận V của 0 trong $L(G)$ sao cho
$$
\rho(\phi(x)) = \exp(L(\rho)x)
$$
với mọi $x \in V$.

Điều này suy ra từ Mệnh đề 8 và Ví dụ 2 của no. 3.

#### Hệ quả 3 {#lie-iii-s4-prop-8-cor-3 .statement}

Cho G là một nhóm Lie và $\phi$ là một ánh xạ mũ của G.

(i) Tồn tại một lân cận V của 0 trong $L(G)$ sao cho
$$
\mathrm{Ad}(\phi(x)) = \exp \mathrm{ad}\ x.
$$
với mọi $x \in V$.

(ii) Nếu $g \in G$, tồn tại một lân cận W của 0 trong $L(G)$ sao cho
$$
g \phi(x) g^{-1} = (\mathrm{Ad}\ g.x)
$$
với mọi $x \in W$.

(i) suy ra từ Hệ quả 2 và § 3, no. 12, Mệnh đề 44.
(ii) suy ra từ Mệnh đề 8 áp dụng cho Int g.

### 5. CẤU TRÚC CẢM SINH TRÊN MỘT NHÓM CON

#### Bổ đề 4 {#lie-iii-s4-lem-4 .statement}

Cho G là một nhóm Lie hữu hạn chiều, $\Omega$ là một lân cận mở đối xứng của e trong G và H là một tập con của $\Omega$ chứa e sao cho các điều kiện $x \in H, y \in H, xy^{-1} \in \Omega$ kéo theo $xy^{-1} \in H$. Cho $r \in N_K$. Với mọi $x \in H$, gọi $h_x$ là tập hợp các $a \in T_x(G)$ có tính chất sau: tồn tại một lân cận mở I của 0 trong K và một ánh xạ f lớp $C^r$ từ I vào G sao cho $f(0) = x, f(I) \subset H, (T_0f)(1) = a$.

(i) Gọi $h_e = h$. Khi đó h là một đại số con Lie của $L(G)$ bất biến dưới $\mathrm{Ad}_{L(G)}(H)$.

(ii) $h_x = xh = hx$ với mọi $x \in H$ (trong đó $xh$ và $hx$ được tính trong $T(G)$).

(iii) Cho V là một đa tạp lớp $C^r$, $v_0$ là một điểm của V và f là một ánh xạ lớp $C^r$ từ V vào G sao cho $f(v_0) = e$ và $f(V) \subset H$. Với mọi mầm nhóm con Lie $H'$ của G có đại số Lie h, $f(v) \in H'$ với v đủ gần $v_0$.

(iv) Với mọi mầm nhóm con Lie $H'$ của G có đại số Lie h, $H' \cap H$ là một lân cận của e trong $H'$.

(v) Với mọi $x \in H$ và mọi $a \in h_x$, tồn tại một lân cận mở I của 0 trong K và một ánh xạ f lớp $C^a$ từ I vào G sao cho $f(0) = x, f(I) \subset H, (T_0f)(1) = a$. Rõ ràng $Kh = h$ và $xh_yz = h_{xyz}$ với $x, y, xy, xyz$ trong H. Điều này suy ra (ii) và tính chất h bất biến dưới $\mathrm{Ad}_{L(G)}(H)$.

Cho $a_1, a_2$ thuộc h. Cho I là một lân cận mở của 0 trong K và $f_1, f_2$ là các ánh xạ lớp $C^r$ từ I vào G sao cho $f_j(0) = e, f_j(I) \subset H, (T_0f_j)(1) = a_j$ ($j = 1, 2$). Ta định nghĩa $f : I \to G$ bởi $f(\lambda) = f_1(\lambda)f_2(\lambda)$. Khi đó f là lớp $C^r$ và $f(0) = e$. Bằng cách thu nhỏ I nếu cần, ta có $f(I) \subset H$. Mặt khác, ánh xạ từ $T_e(G) \times T_e(G)$ vào $T_e(G)$ tiếp xúc với ánh xạ $(g, g') \to gg'$ là phép cộng; do đó $(T_0f) = a_1 + a_2$. Vì vậy $a_1 + a_2 \in h$ và h là một không gian vectơ con của $L(G)$. Vì $xhx^{-1} = h$ với mọi $x \in H$, $(\mathrm{Ad}_{f_1(\lambda)}) . a_2 \in h$ với mọi $\lambda \in I$. Ánh xạ tiếp tuyến tại 0 của ánh xạ $\lambda \mapsto \mathrm{Ad}f_1(\lambda)$ là, theo Mệnh đề 44 của § 3, no. 12, ánh xạ $\lambda \mapsto \mathrm{ad}(a_1\lambda)$; do đó

$$
[a_1, a_2] = (\mathrm{ad}\, a_1) . a_2 \in h
$$

vì $h$ là đóng trong $L(G)$. Do đó ta đã chứng minh (i). Trong phần còn lại của chứng minh, ta cố định một mầm nhóm Lie con $H'$ của G có đại số Lie h.

Cho V, $v_0, f$ như trong (iii). Gọi Y là phân lá trái của G liên kết với h (no. 1). Với mọi $y \in H'$, $T_y(H') = yh$. Mặt khác, với mọi $v \in V$, ảnh của $T_v(V)$ qua $T_v(f)$ được chứa trong $h_{f(v)} = f(v)h$ (theo định nghĩa của $h_{f(v)}$). Theo *Differentiable and Analytic Manifolds*, R, 9.3.2, f là một cấu xạ của V vào Y. Vì $H'$ là một lá của Y (*Differentiable and Analytic Manifolds*, R, 9.2.8), $f(v) \in H'$ với v đủ gần $v_0$.

Cho $(a_1, \ldots, a_s)$ là một cơ sở của h. Tồn tại một lân cận mở I của 0 trong K và các ánh xạ $f_1, \ldots, f_s$ thuộc lớp $C^r$ từ I vào G sao cho $f_j(0) = e, f_j(I) \subset H, (Tf_j)1 = a_j$ với mọi j. Theo (iii), $f_j(\lambda) \in H'$ với $|\lambda|$ đủ nhỏ. Do đó các $f_1(\lambda_1)f_2(\lambda_2)\ldots f_s(\lambda_s)$ tạo thành, với $|\lambda_1|, |\lambda_2|, \ldots, |\lambda_s|$ đủ nhỏ, một lân cận của $e$ trong $H'$; và lân cận này được chứa trong $H$. Suy ra (iv).

Nếu $a \in \mathfrak{h}$, tồn tại một lân cận mở I của 0 trong K và một ánh xạ f thuộc lớp $C^\omega$ từ I vào G sao cho $f(0) = e, f(I) \subset H', (T_0 f)1 = a$. Điều này, cùng với (iv), suy ra (v).

#### Định nghĩa 2 {#lie-iii-s4-def-2 .statement}

$\mathfrak{h}$ được gọi là đại số con tiếp tuyến với $H$ tại $e$.

#### Mệnh đề 9 {#lie-iii-s4-prop-9 .statement}

Cho $G$ là một nhóm Lie hữu hạn chiều và $H$ là một nhóm con của $G$.

(i) Tồn tại trên $H$ một và chỉ một cấu trúc đa tạp giải tích với tính chất sau: với mọi $r$ giữa 1 và $\omega$, với mọi đa tạp V thuộc lớp $C^r$ và với mọi ánh xạ $f$ của V vào $H$, $f$ là thuộc lớp $C^r$ như một ánh xạ của V vào $H$ khi và chỉ khi $f$ là thuộc lớp $C^r$ như một ánh xạ của V vào $G$.

(ii) Với cấu trúc này, $H$ là một nhóm Lie, đơn ánh chính tắc $i$ của $H$ vào $G$ là một immersion và $L(i)(L(H))$ là đại số con Lie tiếp tuyến tại $e$ của $H$.

Trong (i), tính duy nhất là hiển nhiên. Ta chứng minh sự tồn tại. Gọi $\mathfrak{h}$ là đại số Lie tiếp tuyến tại $e$ của $H$. Gọi $H'$ là một mầm nhóm con Lie của $G$ với đại số Lie $\mathfrak{h}$. Bằng cách thay thế $H'$ bởi một mầm nhóm con mở của $H'$, có thể giả sử rằng $H' \subset H$ (Bổ đề 4 (iv)). Với mọi $x \in H$, $xH'x^{-1}$ là một mầm nhóm con Lie của $G$ với đại số Lie $x\mathfrak{h}x^{-1} = \mathfrak{h}$. Do đó $H' \cap (xH'x^{-1})$ là mở trong $H'$ (no. 2, Định lý 3) và ánh xạ $y \mapsto xyx^{-1}$ là một đẳng cấu từ $H' \cap x^{-1}H'x$ lên $xH'x^{-1} \cap H'$. Dùng Mệnh đề 18 của § 1, no. 9, tồn tại một mầm nhóm con Lie mở $W$ của $H'$ và một cấu trúc nhóm Lie trên $H$ với các tính chất sau: $W$ là mở trong $H$ và các cấu trúc đa tạp trên $H$ và $H'$ cảm sinh cùng một cấu trúc trên $W$. Từ đó suy ra rằng đơn ánh chính tắc $i$ của $H$ vào $G$ là một immersion và $L(i)(L(H)) = L(H') = \mathfrak{h}$. Hơn nữa, hãy cho $V$ và $f$ như trong (i). Nếu $f : V \to H$ thuộc lớp $C^r$, thì $i \circ f : V \to G$ thuộc lớp $C^r$. Giả sử $i \circ f : V \to G$ thuộc lớp $C^r$; khi đó ta chứng minh rằng $f : V \to H$ thuộc lớp $C^r$. Nhờ phép tịnh tiến, chỉ cần xét trường hợp tồn tại $v_0 \in V$ sao cho $f(v_0) = e$ và chứng minh rằng $f : V \to H$ thuộc lớp $C^r$ trong một lân cận mở của $v_0$. Bây giờ, theo Bổ đề 4 (iii), $f(v) \in H'$ với $v$ đủ gần $v_0$, do đó mệnh đề của chúng ta. Như vậy ta đã chứng minh (i) và (ii) đã được thu được trên đường đi.

#### Định nghĩa 3 {#lie-iii-s4-def-3 .statement}

Cấu trúc nhóm Lie trên $H$ được định nghĩa trong Mệnh đề 9 được gọi là cấu trúc cảm sinh trên $H$ bởi cấu trúc nhóm Lie trên $G$.

Nếu $H$ là một nhóm con Lie của $G$, thì cấu trúc nhóm Lie của nó được cảm sinh bởi cấu trúc trên $G$ (Đa tạp khả vi và giải tích, R, 5.8.5).

Nếu $G = \mathbf{R}$ và $H = \mathbf{Q}$, thì $\mathfrak{h} = \{0\}$ và do đó cấu trúc cảm sinh trên $H$ là cấu trúc nhóm Lie rời rạc. Tương tự nếu $G = \mathbf{C}$ (được xét như một nhóm Lie phức) và $H = \mathbf{R}$.

### 6. NGUYÊN HÀM CỦA CÁC DẠNG VI PHÂN NHẬN GIÁ TRỊ TRONG MỘT ĐẠI SỐ Lie

#### Bổ đề 5 {#lie-iii-s4-lem-5 .statement}

Cho $X$ là một đa tạp lớp $C^r$, $F$ và $F'$ là các phân thớ vectơ lớp $C^r$ với không gian cơ sở $X$ và $\phi$ là một cấu xạ từ $F$ vào $F'$. Với mọi $x \in X$, cho $S_x$ là tập hợp các
$$
(a, \phi(a)) \in F_x \oplus F'_x
$$
với $a \in F_x$. Khi đó hợp $S$ của các $S_x$ là một phân thớ con vectơ của $F \oplus F'$.

Cho $\theta$ và $\theta'$ là các ánh xạ từ $F \oplus F'$ vào chính nó được định nghĩa như sau: nếu $(u, v) \in F_x \oplus F'_x$, thì
$$
\theta(u, v) = (u, v + \phi(u)), \qquad \theta'(u, v) = (u, v - \phi(u)).
$$
Theo *Đa tạp khả vi và giải tích*, R, 7.7.1, $\theta$ và $\theta'$ là các cấu xạ của $F \oplus F'$ vào chính nó. Rõ ràng $\theta \circ \theta' = \theta' \circ \theta = \mathrm{Id}_{F \oplus F'}$. Do đó $\theta$ và $\theta'$ là các tự đẳng cấu của $F \oplus F'$. Vì vậy, $S = \theta(F \oplus \{0\})$ là một phân thớ con vectơ của $F \oplus F'$.

#### Bổ đề 6 {#lie-iii-s4-lem-6 .statement}

Cho $G$ là một mầm nhóm Lie, $\omega$ là dạng vi phân trái chính tắc của $G$ (\S 3, no. 18.9), $M$ là một đa tạp lớp $C^r$ ($r \geq 2$) và $\alpha$ là một dạng vi phân lớp $C^{r-1}$ và bậc 1 trên $M$ nhận giá trị trong $L(G)$.

(i) Các phần tử của $T(M \times G)$ tại đó dạng vi phân
$$
\theta = \mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega
$$
bằng không tạo thành một phân thớ con vectơ $S$ của $T(M \times G)$ thuộc lớp $C^{r-1}$.

(ii) Với mọi $(x, g) \in M \times G$, $T(\mathrm{pr}_1)|S_{(x, g)}$ là một đẳng cấu từ $S_{(x, g)}$ lên $T_x(M)$.

(iii) *Nếu* $d\alpha + [\alpha]^2 = 0$ (cf. \S 3, no. 14) *thì phân thớ con vectơ* $S$ *có thể tích phân*.

==========

Đó là toàn bộ đoạn văn. Hãy viết bản dịch của tất cả những gì nằm giữa hai dòng ấy, và dừng ở đó.

Nếu $(x, g) \in M \times G$ và $(u, v) \in T_x(M) \times T_g(G)$, thì
$$
\theta_{(x, g)}(u, v) = \alpha(u) - g^{-1}v.
$$
Do đó hạt nhân của $\theta_{(x, g)}$ là tập hợp $S_{(x, g)}$ gồm các $(u, g\alpha(u))$ với $u \in T_x(M)$, suy ra (ii). Ta xét $T(M \times G)$ như tổng trực tiếp của hai bó vectơ $F$ và $F'$ với $F_{(x, g)} = T_x(M) \times \{0\}$ và $F'_{(x, g)} = \{0\} \times T_g(G)$ với mọi
$$
(x, g) \in M \times G.
$$
Với $u \in T_x(M) \times \{0\}$, ta viết $\phi(u) = (0, g\alpha(u))$. Dùng sự tầm thường hóa trái của $T(G)$, thấy rằng $\phi$ là một cấu xạ của $F$ vào $F'$, suy ra (i) (Bổ đề 5). Cuối cùng, nếu $d\alpha + [\alpha]^2 = 0$, thì
$$
\begin{align*}
d\theta &= \mathrm{pr}_1^*(d\alpha) - \mathrm{pr}_2^*(d\omega) \\
&= -\frac{1}{2}(\mathrm{pr}_1^*\alpha \wedge \mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega \wedge \mathrm{pr}_2^*\omega) \\
&= -\frac{1}{2}(\mathrm{pr}_1^*\alpha - \mathrm{pr}_2^*\omega) \wedge (\mathrm{pr}_1^*\alpha + \mathrm{pr}_2^*\omega) \\
&= -\frac{1}{2}\theta \wedge (\mathrm{pr}_1^*\alpha + \mathrm{pr}_2^*\omega)
\end{align*}
$$
và do đó $S$ khả tích (*Differentiable and Analytic Manifolds*, R, 9.3.6).

#### Định lý 5 {#lie-iii-s4-thm-5 .statement}

Cho G là một mầm nhóm Lie, M là một đa tạp lớp $C^r$ ($r \geq 2$) và $\alpha$ là một dạng vi phân lớp $C^{r-1}$ và bậc 1 trên M với giá trị trong $L(G)$, sao cho $d\alpha + [\alpha]^2 = 0$. Với mọi $x \in M$ và mọi $g \in G$, tồn tại một ánh xạ $f$, được xác định và thuộc lớp $C^{r-1}$ trên một lân cận mở của $x$, với giá trị trong G, sao cho $f(x) = g$ và $f^{-1}.df = \alpha$. Hai ánh xạ thỏa mãn các điều kiện này trùng nhau trên một lân cận của $x$.

Cho $x \in M$ và $g \in G$. Theo Bổ đề 6 (chúng ta dùng ký hiệu của nó) và *Differentiable and Analytic Manifolds*, R, 9.3.7, tồn tại một lân cận mở U của $x$ trong M và một ánh xạ $m \mapsto \phi(m) = (m, f(m))$ lớp $C^{r-1}$ từ U vào $M \times G$ sao cho $f(x) = g$ và $\phi^*(0) = 0$. Khi đó

$$
f^{-1}.df = f^*(\omega) \quad (\S 3, \text{no. 18.9}) \\
= (\mathrm{pr}_2 \circ \phi)^*(\omega) \quad (\text{với } f = \mathrm{pr}_2 \circ \phi) \\
= \phi^*(\mathrm{pr}_1^*\alpha - \theta) \quad (\text{Bổ đề 6}) \\
= \phi^*(\mathrm{pr}_1^*\alpha) \quad (\text{vì } \phi^*(\theta) = 0) \\
= \alpha \quad (\text{vì } \mathrm{pr}_1 \circ \phi = \mathrm{Id}_U).
$$

Cho $f'$ là một ánh xạ lớp $C^{r-1}$ từ U vào G sao cho $f'(x) = g$ và $f'^{-1}df' = \alpha$. Theo \S 3, 18.9, $f'^{-1}$ là hằng địa phương và do đó $f' = f$ trong một lân cận của $x$.

#### Mệnh đề 10 {#lie-iii-s4-prop-10 .statement}

Cho M là một đa tạp giải tích, $\mathfrak{g}$ một đại số Lie chuẩn hoá được đầy đủ và $\alpha$ một dạng vi phân giải tích bậc 1 trên M, nhận giá trị trong $\mathfrak{g}$, với các tính chất sau:
(a) với mọi $m \in M$, $\alpha_m$ là một đẳng cấu từ $T_m(M)$ lên $\mathfrak{g}$;
(b) $d\alpha + [\alpha]^2 = 0$.

Khi đó, với mọi $m_0 \in M$, tồn tại một lân cận mở $M'$ của $m_0$ trong M và một cấu trúc mầm nhóm Lie trên $M'$, tương thích với cấu trúc đa tạp trên $M'$, có phần tử đơn vị là $m_0$ và có các tính chất sau:
(i) $\alpha_{m_0}$ là một đẳng cấu từ $L(M')$ lên $\mathfrak{g}$;
(ii) dạng vi phân $m \mapsto \alpha_{m_0}^{-1} \circ \alpha_m$ là dạng vi phân chính tắc trái của $M'$.
Nếu $M'_1$ và $M'_2$ là hai mầm nhóm như thế, thì $M'_1$ và $M'_2$ có một mầm nhóm con mở chung.

Tồn tại một mầm nhóm Lie G sao cho $L(G) = \mathfrak{g}$. Cho $m_0 \in M$. Theo Định lý 5, tồn tại một lân cận mở $M'$ của $m_0$ trong M và một ánh xạ giải tích $f$ từ $M'$ vào G sao cho $f(m_0) = e$ và $f^{-1}.df = \alpha$. Khi đó $T_{m_0}(f) = \alpha_{m_0}$ là một đẳng cấu từ $T_{m_0}(M)$ lên $\mathfrak{g}$; do đó, thu nhỏ $M'$ và G lại, có thể giả sử rằng $f$ là một đẳng cấu của đa tạp $M'$ lên đa tạp G. Ta chuyển lên $M'$ cấu trúc mầm nhóm Lie trên G bằng $f^{-1}$. Khi đó $T_{m_0}(f)$ trở thành một đẳng cấu từ $L(M')$ lên $L(G) = \mathfrak{g}$, suy ra (i). Mặt khác, nếu $\omega$ ký hiệu dạng vi phân chính tắc trái của G, thì
$$
\alpha_{m_0}^{-1} \circ \alpha_m = (\mathrm{T}_{m_0} f)^{-1} \circ (f^{-1}.df)(m)
= (\mathrm{T}_m f)^{-1} \circ \omega(f(m)) \circ \mathrm{T}_m f
$$
và do đó $m \mapsto \alpha_{m_0}^{-1} \circ \alpha_m$ là dạng vi phân chính tắc trái của $M'$.

Let $M''$ be an open neighbourhood of $m_0$, with a Lie group germ structure, with identity element $m_0$ and with the analogous properties to properties (i) and (ii). Then $\alpha_{m_0}$ is an isomorphism of $L(M')$ onto $g$ and also of $L(M'')$ onto $g$ and hence $L(M') = L(M'')$. Therefore, shrinking $M'$ and $M''$, it can be assumed that there exists an isomorphism $\phi$ of the group germ $M'$ onto the group germ $M''$ (no. 1, Corollary 1 to Theorem 1). Then $\phi^{-1}.d\phi$ is the canonical left differential of $M'$. On the other hand, let $\psi$ be the canonical injection of the manifold $M' \cap M''$ into the Lie group germ $M''$; clearly $\psi^{-1}.d\psi$ is a restriction of the canonical left differential of $M''$. Hence $(\psi^{-1}.d\psi)(m) = \alpha_{m_0}^{-1} \circ \alpha_m = (\phi^{-1}.d\phi)(m)$ for all $m \in M' \cap M''$. Therefore $\phi$ and $\psi$ coincide on a neighbourhood of $m_0$ (\S 3, 18.9). This proves the last assertion of the proposition.

#### Hệ quả {#lie-iii-s4-n6-cor-1 .statement}

Let $M$ be an analytic manifold of finite dimension $n$. Let $\omega_1, \ldots, \omega_n$ be analytic differential forms of degree 1 on $M$, with scalar values, which are linearly independent at each point of $M$ and such that, for all $k = 1, \ldots, n$, $d\omega_k$ is a linear combination with constant coefficients of the $\omega_i \wedge \omega_j$. Then, for all $m_0 \in M$, there exists an open neighbourhood $M'$ of $m_0$ in $M$ and a Lie group germ structure on $M'$ compatible with the manifold structure on $M'$, with identity element $m_0$ and such that $\omega_1|_{M'}, \ldots, \omega_n|_{M'}$ form a basis of the space of left invariant differential forms on $M'$ of degree 1 with scalar values.

If $M'_1$ and $M'_2$ are two such group germs, $M'_1$ and $M'_2$ have a common open subgroup germ.

Cho $X_1, \ldots, X_n$ là các trường vectơ trên $M$ sao cho, tại mỗi điểm $m$ của $M$, các $(X_t)_m$ tạo thành cơ sở của $T_m(M)$ đối ngẫu với $((\omega_1)_m, \ldots, (\omega_n)_m)$. Các trường này là giải tích. Theo giả thiết, tồn tại $c_{ijk} \in \mathbf{K}$ ($1 \leq i, j, k \leq n$) sao cho $c_{ijk} = -c_{jik}$ và $d\omega_k = \sum_{i < j} c_{ijk} \omega_i \wedge \omega_j$. Theo *Đa tạp khả vi và giải tích*, R, 8.5.7, công thức (11),
$$
\langle [X_i, X_j], \omega_k \rangle = -(d\omega_k)(X_i, X_j) = -\left( \sum_{r < s} c_{rsk} \omega_r \wedge \omega_s \right)(X_i, X_j) = -c_{ijk}
$$
và do đó $[X_i, X_j] = -\sum_k c_{ijk} X_k$. Suy ra rằng các $-c_{ijk}$ là các hằng số cấu trúc của một đại số Lie $g$ đối với một cơ sở $(e_1, \ldots, e_n)$. Với mọi $m \in M$, cho $\alpha_m$ là ánh xạ tuyến tính của $T_m(M)$ vào $g$ đưa $(X_1)_m$ tới $e_1, \ldots, (X_n)_m$ tới $e_n$. Khi đó $\alpha$ là một dạng vi phân giải tích trên $M$ có bậc 1 với giá trị trong $g$ và $\alpha_m$ là một đẳng cấu của $T_m(M)$ lên $g$. Mặt khác, $\alpha = \sum_{k=1}^n \omega_k e_k$ và do đó
$$
d\alpha = \sum_{k=1}^n (d\omega_k)e_k = \sum_{k=1}^n \left( \sum_{i<j} c_{ijk}\omega_i \wedge \omega_j \right)e_k
$$
và
$$
\begin{align*}
[\alpha]^2 &= \sum_{k=1}^n [\omega_k e_k]^2 + \sum_{i<j} (\omega_i e_i) \wedge (\omega_j e_j) \quad (\S 3, \text{công thức (30)}) \\
&= \sum_{i<j} (\omega_i \wedge \omega_j)[e_i, e_j] \\
&= -\sum_{k=1}^n \sum_{i<j} (c_{ijk}\omega_i \wedge \omega_j)e_k \\
&= -d\alpha.
\end{align*}
$$
Khi đó chỉ cần áp dụng Mệnh đề 10.

### 7. CHUYỂN TỪ CÁC LUẬT TÁC ĐỘNG VÔ CỰC NHỎ SANG CÁC LUẬT TÁC ĐỘNG

#### Mệnh đề 11 {#lie-iii-s4-prop-11 .statement}

Cho $G_1$ và $G_2$ là các mầm nhóm Lie và $X_1$ và $X_2$ là các đa tạp lớp $C^r$ ($r \geq 2$). Với $i = 1, 2$, cho $\psi_i$ là một mảnh luật tác động trái lớp $C^r$ của $G_i$ lên $X_i$ và $D_i$ là luật tác động vô cực nhỏ liên kết. Cho $\mu : G_1 \to G_2$ là một cấu xạ và $\phi : X_1 \to X_2$ là một ánh xạ lớp $C^r$. Giả sử rằng, với mọi $a \in L(G)$, các trường vectơ $(D_1)_a$ và $(D_2)_{L(\mu)a}$ là $\phi$-liên quan (*Đa tạp khả vi và giải tích*, R, 8.2.6). Khi đó tồn tại một lân cận $\Omega$ của $\{e\} \times X_1$ trong $G_1 \times X_1$ sao cho $\phi(\psi_1(g, x)) = \psi_2(\mu(g), \phi(x))$ với mọi $(g, x) \in \Omega$.

Cho $p_1 : G_1 \times X_2 \to G_1, p_2 : G_1 \times X_2 \to X_2$ là các phép chiếu chính tắc. Với mọi $(g_1, x_2) \in G_1 \times X_2$, cho $f_{g_1, x_2}$ là ánh xạ $g_1 a \mapsto (D_2)_{L(\mu)a}(x_2)$ từ $T_{g_1}(G_1) = g_1 L(G_1)$ vào $T_{x_2}(X_2)$. Các $f_{g_1, x_2}$ xác định một cấu xạ của $p_1^*T(G_1)$ vào $p_2^*T(X_2)$.

Cho $x_0 \in X_1$. Tồn tại một lân cận mở $G$ của $e$ trong $G_1$ và một lân cận mở $X$ của $x_0$ trong $X_1$ sao cho $\psi_1(g, x)$ và $\psi_2(\mu(g), \phi(x))$ được xác định với $(g, x) \in G \times X$. Ta viết, với $(g, x) \in G \times X$,
$$
\alpha(g, x) = \phi(\psi_1(g, x)) \in X_2, \qquad \beta(g, x) = \psi_2(\mu(g), \phi(x)) \in X_2.
$$
Nếu $G$ và $X$ đủ nhỏ, thì, với mọi $(a, g, x) \in L(G_1) \times G \times X$,
$$
\begin{align*}
(T\alpha)(ag, 0_x) &= (T\phi)((D_1)_a(\psi_1(g, x))) \\
&= (D_2)_{L(\mu)a}(\phi(\psi_1(g, x))) \\
&= (D_2)_{L(\mu)a}\alpha(g, x), \\
(T\beta)(ag, 0_x) &= (T\psi_2)(L(\mu)a.\mu(g), \phi(x)) \\
&= (D_2)_{L(\mu)a}(\psi_2(\mu(g), \phi(x))) \\
&= (D_2)_{L(\mu)a}\beta(g, x).
\end{align*}
$$

Vậy với mọi $x \in X$, các ánh xạ $g \mapsto \alpha(g, x)$ và $g \mapsto \beta(g, x)$ là các tích phân của $f$; mà
$$
\beta(e, x) = \phi(x) = \alpha(e, x)
$$
với mọi $x \in X$, suy ra từ *Differentiable and Analytic Manifolds*, R, 9.3.7, rằng $\alpha$ và $\beta$ trùng nhau trên một lân cận của $(e, x_0)$. Do đó mệnh đề.

#### Hệ quả {#lie-iii-s4-n7-cor-1 .statement}

*Cho G là một mầm nhóm Lie và X là một đa tạp lớp $C^r$. Xét hai mảnh luật của phép toán trái lớp $C^r$ của G trên X. Giả sử rằng, với mọi $a \in L(G)$, trường vectơ tương ứng $D_a$ trên X là như nhau cho cả hai mảnh luật. Khi đó hai mảnh luật này trùng nhau trên một lân cận của $\{e\} \times X$.*

#### Định lý 6 {#lie-iii-s4-thm-6 .statement}

*Cho G là một mầm nhóm Lie, X là một đa tạp lớp $C^r$ ($r \geq 2$) và $x_0$ là một điểm của X. Cho $a \mapsto D_a$ là một luật phép toán vô cùng bé trái lớp $C^{r-1}$ của $L(G)$ trên X.*

(i) *Tồn tại một lân cận mở $X'$ của $x_0$ trong X và một mảnh luật của phép toán trái lớp $C^{r-1}$ của G trên $X'$ sao cho luật phép toán vô cùng bé liên kết là $a \mapsto D_a|X'$. \*

(ii) *Cho tồn tại hai mảnh luật của phép toán trái lớp $C^{r-1}$ của G trên một lân cận mở $X''$ của $x_0$; nếu chúng nhận $a \mapsto D_a|X''$ làm luật phép toán vô cùng bé liên kết, thì chúng trùng nhau trên một lân cận của $(e, x_0)$. \*

Mệnh đề (ii) suy ra từ Hệ quả của Mệnh đề 11. Chứng minh (i). Với mọi $(g, x) \in G \times X$ và mọi $a \in L(G)$, ta viết
$$
Q_a(g, x) = (ag, D_a(x)) \in T_g(G) \times T_x(X).
$$
Cho $S_{(g, x)}$ là tập các $Q_a(g, x)$ với $a \in L(G)$. Theo Bổ đề 5 của no. 6, các $S_{(g, x)}$ là các thớ của một phân bó con vectơ S của $T(G) \times T(X)$. Cho $a, b$ thuộc $L(G)$; khi đó
$$
\begin{align*}
[Q_a, Q_b](g, x) &= ([R_a, R_b](g), [D_a, D_b](x)) \\
&= (-R_{[a, b]}(g), -D_{[a, b]}(x)) \quad (\S 3, 18.6) \\
&= Q_{-[a, b]}(g, x)
\end{align*}
$$
và do đó S là khả tích (*Differentiable and Analytic Manifolds*, R, 9.3.3, (iv)).

Theo *Differentiable and Analytic Manifolds*, R, 9.3.7, tồn tại một lân cận mở $G_1$ của e trong G, một lân cận mở $X_1$ của $x_0$ trong X và một ánh xạ $(g, x) \mapsto gx$ lớp $C^{r-1}$ của $G_1 \times X_1$ vào X sao cho $ex = x$ với mọi $x \in X_1$ và
$$
(ag)x = D_a(gx) \quad \text{theo } a \in L(G), g \in G_1, x \in X_1.
$$
Đặc biệt
$$
ax = D_a(x).
$$
Cho $G_2$ là một lân cận mở của e trong $G_1$ và $X_2$ là một lân cận mở của $x_0$ trong $X_1$ sao cho $gg'$ được xác định và thuộc $G_1$ với mọi $g, g'$ trong $G_2$ và $gx$ được xác định và thuộc $X_1$ với mọi $(g, x) \in G_2 \times X_2$. Xét các ánh xạ $\alpha_1, \alpha_2$ từ $G_2 \times (G_2 \times X_2)$ vào X được xác định bởi
$$
\alpha_1(g, (h, x)) = g(hx), \quad \alpha_2(g, (h, x)) = (gh)x.
$$
Chúng thuộc lớp $C^{r-1}$. Khi đó
$$
\alpha_1(e, (h, x)) = hx = \alpha_2(e, (h, x)).
$$
Mặt khác
$$
\begin{align*}
T(\alpha_1)(ag, 0_{(h, x)}) &= (ag)(hx) \\
&= D_a(g(hx)) \qquad \text{theo (6)} \\
&= D_a(\alpha_1(g, (h, x))), \\
T(\alpha_2)(ag, 0_{(h, x)}) &= (agh)x \\
&= D_a((gh)x) \qquad \text{theo (6)} \\
&= D_a(\alpha_2(g, (h, x))).
\end{align*}
$$
Theo *Differentiable and Analytic Manifolds*, R, 9.3.7, $\alpha_1$ và $\alpha_2$ trùng nhau trên một lân cận của $(e, (e, x_0))$. Khi đó (i) suy ra từ (7) và Mệnh đề 23 của § 1, no. 11.

#### Hệ quả 1 {#lie-iii-s4-thm-6-cor-1 .statement}

*Cho $G$ là một mầm nhóm Lie và $X$ là một đa tạp paracompact lớp $C^r$ ($r \geq 2$). Cho $a \mapsto D_a$ là một luật của phép toán vi phân trái lớp $C^{r-1}$ của $L(G)$ trên $X$.

(i) Tồn tại một mầm của phép toán trái lớp $C^{r-1}$ của $G$ trên $X$ sao cho luật phép toán vi phân liên kết là $a \mapsto D_a$.

(ii) Hai luật của phép toán trái lớp $C^{r-1}$ của $G$ trên $X$ mà nhận $a \mapsto D_a$ làm luật phép toán vi phân liên kết thì trùng nhau trên một lân cận của $\{e\} \times X$.*

Mệnh đề (ii) suy ra từ hệ quả của Mệnh đề 11. Theo Định lý 6 (i), tồn tại một phủ mở $(X_i)_{i \in I}$ của $X$ và, với mọi $i \in I$, một mảnh luật của phép toán trái $\psi_i$ lớp $C^{r-1}$ của $G$ trên $X_i$ sao cho luật liên kết của phép toán vi phân là $a \mapsto D_a|_{X_i}$. Vì $X$ là paracompact, có thể giả sử phủ $(X_i)_{i \in I}$ là hữu hạn địa phương. Với mọi $(i, j) \in I \times I$ và mọi $x \in X_i \cap X_j$, $\psi_i$ và $\psi_j$ trùng nhau trên một lân cận của $(e, x)$ (Hệ quả của Mệnh đề 11). Vì $X$ là chuẩn tắc, ta có thể áp dụng Mệnh đề 24 của § 1, no. 11, điều này chứng minh (i).

#### Hệ quả 2 {#lie-iii-s4-thm-6-cor-2 .statement}

*Cho $X$ là một đa tạp paracompact của lớp $C^r$ ($r \geq 2$) và $\xi$ là một vectơ trường lớp $C^{r-1}$ trên $X$. Tồn tại một mảnh luật của phép toán $\psi$ lớp $C^{r-1}$ của $K$ trên $X$ sao cho với mọi $x \in X$, $\xi(x)$ là ảnh qua $t \mapsto (t, x)$ của vectơ tiếp tuyến 1 của $K$ tại 0. Hai mảnh luật của phép toán có tính chất trên trùng nhau trên một lân cận của $\{0\} \times X$.

Đây là trường hợp riêng của Hệ quả 1.*

§ 5.1

#### Nhận xét {#lie-iii-s4-n7-rem-1 .statement}

Các luật của phép toán trái dĩ nhiên có thể được thay thế, trong toàn bộ no. này, bằng các luật của phép toán phải.

### Bài tập {#lie-iii-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
