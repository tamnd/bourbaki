---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 6
section_title: Extensions, solvable groups, nilpotent groups
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0089-0105, 0171-0183
extraction: ocr
subsections:
    - "no": 1
      title: EXTENSIONS
      page: 0
      pdf_page: 89
    - "no": 2
      title: COMMUTATORS
      page: 0
      pdf_page: 92
    - "no": 3
      title: LOWER CENTRAL SERIES, NILPOTENT GROUPS
      page: 0
      pdf_page: 95
    - "no": 4
      title: DERIVED SERIES, SOLVABLE GROUPS
      page: 0
      pdf_page: 98
    - "no": 5
      title: $p$-GROUPS
      page: 0
      pdf_page: 100
    - "no": 6
      title: SYLOW SUBGROUPS
      page: 0
      pdf_page: 102
    - "no": 7
      title: FINITE NILPOTENT GROUPS
      page: 0
      pdf_page: 104
statements: 58
exercises: 8
content_sha256: b4008e5b33ae3a61a679bee986e706a43300e30dc53a69879e7dba7895f964fa
translated_from: content/en/alg/I/06_s6_extensions_solvable_groups_nilpotent.md
source_content_sha256: 444ce10c845cf4285699a41f8315e02aaa1384af2372bd4fd0466da5aa4acee7
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4-mini
translation_run: translate-vi-91a0ea53
glossary_version: 34
glossary_terms_sha256: 48390f32aa9962888412870dc8b619a10858bd79521e9880efcd5f2c70c63e49
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. MỞ RỘNG, NHÓM GIẢI ĐƯỢC, NHÓM LŨY LINH

Trong suốt tiết này, các phép toán nhóm, trừ khi có nói rõ khác đi, đều được viết theo phép nhân.

### 1. MỞ RỘNG

#### Định nghĩa 1 {#alg-i-s6-def-1 .statement}

Cho $F$ và $G$ là hai nhóm. Một mở rộng của $G$ bởi $F$ là một bộ ba $\mathcal{E} = (E, i, p)$, trong đó $E$ là một nhóm, $i$ là một đơn cấu của $F$ vào $E$ và $p$ là một đồng cấu toàn ánh từ $E$ lên $G$ sao cho $\operatorname{Im}(i) = \operatorname{Ker}(p)$. Một đồng cấu $s : G \to E$ (tương ứng $r : E \to F$) sao cho $p \circ s = \operatorname{Id}_G$ (tương ứng $r \circ i = \operatorname{Id}_F$) được gọi là một tiết diện (tương ứng một phép co rút) của mở rộng $\mathcal{E}$.

Một mở rộng $\mathcal{E} = (E, i, p)$ của $G$ bởi $F$ thường được ký hiệu bởi biểu đồ $\mathcal{E} : F \xrightarrow{i} E \xrightarrow{p} G$, trong đó $i$ và $p$ đôi khi được bỏ qua nếu không thể gây nhầm lẫn. Đôi khi người ta cũng chỉ nói rằng nhóm $E$ là một mở rộng của $G$ bởi $F$.

Để một nhóm $E$ là một mở rộng của $G$ bởi $F$, điều kiện cần và đủ là nó chứa một nhóm con chuẩn tắc $F'$ đẳng cấu với $F$ sao cho nhóm thương $E/F'$ đẳng cấu với $G$.

Một mở rộng $\mathcal{E} : F \xrightarrow{i} E \xrightarrow{p} G$ được gọi là trung tâm nếu ảnh $i(F)$ được chứa trong tâm của $E$; điều này chỉ có thể xảy ra nếu $F$ giao hoán.

Cho $\mathcal{E} : F \xrightarrow{i} E \xrightarrow{p} G$ và $\mathcal{E}' : F \xrightarrow{i'} E' \xrightarrow{p'} G$ là hai mở rộng của $G$ bởi $F$. Một cấu xạ từ $\mathcal{E}$ vào $\mathcal{E}'$ là một đồng cấu $u : E \to E'$ sao cho $p' \circ u = p$ và $u \circ i = i'$, hay nói cách khác, sao cho biểu đồ sau đây giao hoán:

$$
\begin{array}{ccc}
& & E \\
& i & \\
F & \xrightarrow{i'} & E' \\
& \downarrow & \downarrow \\
& & E \\
& p & \\
& & G
\end{array}
$$

u ↑ \quad \text{and} \quad p' ↑

#### Mệnh đề 1 {#alg-i-s6-prop-1 .statement}

Cho $\mathcal{E}: F \xrightarrow{i} E \xrightarrow{p} G$ và $\mathcal{E}': F \xrightarrow{i'} E' \xrightarrow{p'} G$ là các mở rộng của $G$ bởi $F$. Nếu $u: E \to E'$ là một cấu xạ của $\mathcal{E}$ vào $\mathcal{E}'$, thì $u$ là một đẳng cấu của $E$ lên $E'$ và $u^{-1}$ là một cấu xạ của $\mathcal{E}'$ vào $\mathcal{E}$.

Cho $x \in E$ sao cho $u(x) = e$. Khi đó $p(x) = p'(u(x)) = e$, do đó $x \in i(F)$. Cho $y \in F$ sao cho $x = i(y)$; khi đó $i'(y) = u(i(y)) = e$. Vì $i'$ là đơn ánh, $y = e$ và $x = e$. Do đó $u$ là đơn ánh. Theo § 4, no. 6, Hệ quả 1 của Mệnh đề 7, $u$ là toàn ánh vì $u(i(F)) = i'(F)$. Khẳng định cuối cùng là ngay lập tức.

Nói cách khác, các mở rộng $\mathcal{E}$ và $\mathcal{E}'$ là *đẳng cấu* khi và chỉ khi tồn tại một cấu xạ của $\mathcal{E}$ vào $\mathcal{E}'$.

Cho $F$ và $G$ là hai nhóm và đặt $E_0 = F \times G$; cho $i: F \to E_0$ là đơn ánh chính tắc và $p: E_0 \to G$ là phép chiếu chính tắc. Mọi mở rộng của $G$ bởi $F$ đẳng cấu với mở rộng $\mathcal{E}_0: F \xrightarrow{i} E_0 \xrightarrow{p} G$ được gọi là một *mở rộng tầm thường*.

#### Mệnh đề 2 {#alg-i-s6-prop-2 .statement}

*Cho $\mathcal{E}: F \xrightarrow{i} E \xrightarrow{p} G$ là một mở rộng của $G$ bởi $F$. Các điều kiện sau là tương đương*:

(i) $\mathcal{E}$ là một mở rộng tầm thường;
(ii) $\mathcal{E}$ có một phép rút gọn $r$;
(iii) $\mathcal{E}$ có một tiết diện $s$ sao cho $s(G)$ được chứa trong tâm hóa của $i(F)$.

Rõ ràng (i) kéo theo (ii) và (iii). Nếu (ii) đúng, ánh xạ $(r, p): E \to F \times G$ là một cấu xạ của $\mathcal{E}$ vào $\mathcal{E}_0$, do đó (i). Nếu (iii) đúng, đồng cấu từ $F \times G$ vào $E$ tương ứng với $(i, s)$ ($\S$ 4, no. 9, Mệnh đề 12) là một cấu xạ của $\mathcal{E}_0$ vào $\mathcal{E}$, do đó (i).

Có thể xảy ra trường hợp một mở rộng $\mathcal{E}: F \to E \to G$ không tầm thường nhưng nhóm $E$ lại đẳng cấu với $F \times G$ (Bài tập 6).

#### Định nghĩa 2 {#alg-i-s6-def-2 .statement}

*Cho $F$ và $G$ là hai nhóm và $\tau$ là một đồng cấu của $G$ vào nhóm tự đẳng cấu của $F$. Viết $\tau(g)(f) = gf$ với $g \in G$ và $f \in F$. Tập hợp $F \times G$ với luật hợp thành*

$$
((f, g), (f', g')) \mapsto (f, g) \cdot_{\tau} (f', g') = (f \cdot gf', gg')
$$

*được gọi là* tích nửa trực tiếp ngoài của $G$ bởi $F$ tương đối với $\tau$.

Tích nửa trực tiếp ngoài của $G$ bởi $F$ tương đối với $\tau$ được ký hiệu là $F \times_{\tau} G$.

#### Mệnh đề 3 {#alg-i-s6-prop-3 .statement}

*Tích nửa trực tiếp ngoài $F \times_{\tau} G$ là một nhóm. Các ánh xạ $i: F \to F \times_{\tau} G$ xác định bởi $i(f) = (f, e)$, $p: F \times_{\tau} G \to G$ xác định bởi $p(f, g) = g$, và $s: G \to F \times_{\tau} G$ xác định bởi $s(g) = (e, g)$ là các đồng cấu nhóm. Bộ ba $(F \times_{\tau} G, i, p)$ là một mở rộng của $G$ bởi $F$ và $s$ là một tiết diện của mở rộng.*

Ta có:

$$
((f, g) \cdot_{\tau} (f', g')) \cdot_{\tau} (f'', g'') = (f.gf', gg') \cdot_{\tau} (f'', g'')
= (f.gf'.gg'f'', gg'g'');
$$
$$
(f, g) \cdot_{\tau} ((f', g') \cdot_{\tau} (f'', g'')) = (f, g) \cdot_{\tau} (f'g'f'', g'g'')
= (f.g(f'.g'f''), gg'g'').
$$

Bây giờ $g(f'.g'f'') = gf'.gg'f''$, điều này chứng minh rằng luật hợp thành được định nghĩa bởi (1) là kết hợp. Phần tử $(e, e)$ là phần tử đơn vị đối với luật này. Phần tử $(f, g)$ có nghịch đảo là $(g^{-1}f^{-1}, g^{-1})$. Do đó luật hợp thành trên $F \times_{\tau} G$ là một luật nhóm. Các khẳng định khác là ngay lập tức.

Sử dụng ký hiệu của Mệnh đề 3, $\mathscr{E}_{\tau}$ sẽ ký hiệu mở rộng

$$
F \xrightarrow{i} F \times_{\tau} G \xrightarrow{p} G.
$$

Cho $\mathscr{E}' : F \xrightarrow{i'} E' \xrightarrow{p'} G$ là một mở rộng của $G$ bởi $F$ và $s' : G \to E'$ là một tiết diện của $\mathscr{E}'$. Ta định nghĩa một phép toán $\tau$ của $G$ trên nhóm $F$ bởi:

(2)
$$
i'(\tau(g, f)) = s'(g)i'(f)s'(g)^{-1} = \operatorname{Int}(s'(g))(i'(f)).
$$

#### Mệnh đề 4 {#alg-i-s6-prop-4 .statement}

*Với ký hiệu trên, tồn tại một và chỉ một đẳng cấu u của $\mathscr{E}_{\tau}$ lên $\mathscr{E}'$ sao cho $u \circ s = s'$.

$$(f, g) = (f, e) \cdot_{\tau} (e, g) = i(f) \cdot_{\tau} s(g).$$ Do đó, nếu $u$ là một nghiệm của bài toán, tất yếu $u(f, g) = i'(f).s'(g)$, do đó tính duy nhất của $u$. Ta chứng minh sự tồn tại. Ta viết $u(f, g) = i'(f).s'(g)$. Khi đó

$$
\begin{align*}
u(f, g).u(f', g') &= i'(f)s'(g)i'(f')s'(g') \\
&= i'(f)(s'(g)i'(f')s'(g)^{-1})s'(g)s'(g') \\
&= i'(f)i'(\tau(g, f')).s'(g)s'(g') \\
&= i'(f.\tau(g, f')).s'(gg') \\
&= u((f, g) \cdot_{\tau} (f', g')).
\end{align*}
$$

Do đó, $u$ là một đồng cấu từ $F \times_{\tau} G$ vào $E'$. Hiển nhiên $u \circ i = i'$, $p' \circ u = p$ và $u \circ s = s'$.

#### Nhận xét {#alg-i-s6-n1-rem-1 .statement}

Định nghĩa phép toán $\tau$ bởi công thức (2) phụ thuộc vào mở rộng $\mathscr{E}'$ và tiết diện $s'$. Khi $F$ giao hoán, phép toán $\tau$ không phụ thuộc vào $s'$. Vì khi đó $\operatorname{Int}(s'(g)) | i'(F)$ chỉ phụ thuộc vào lớp kề của $s'(g)$ mod. $i'(F)$.

Nói chung, cho $\mathscr{E} : F \to E \to G$ là một mở rộng của $G$ bởi một nhóm giao hoán $F$ (không giả thiết rằng $\mathscr{E}$ có một tiết diện). Nhóm $E$ tác động lên $F$ bởi các tự đẳng cấu nội, phép ánh xạ này tầm thường trên ảnh của $F$ và do đó xác định một phép toán của $G$ trên $F$. Nếu $\mathscr{E}$ có một tiết diện, thì phép toán này chính là phép toán được xác định bởi công thức (2).

#### Hệ quả {#alg-i-s6-n1-cor-1 .statement}

*Cho $G$ là một nhóm và $H$ và $K$ là hai nhóm con của $G$ sao cho $H$ là chuẩn tắc, $H \cap K = \{e\}$ và $H.K = G$. Cho $\tau$ là phép toán của $K$ trên $H$ bởi các tự đẳng cấu nội của $G$. Ánh xạ $(h, k) \mapsto hk$ là một đẳng cấu từ $H \times_{\tau} K$ lên $G$.

Với các giả thiết của hệ quả này, $G$ được gọi là tích nửa trực tiếp của $K$ bởi $H$.

#### Ví dụ {#alg-i-s6-n1-exa-1 .statement}

(1) Cho $G$ là một nhóm và $E$ là một $G$-tập hợp chính thuần nhất; ký hiệu $\Gamma$ là nhóm tự đẳng cấu của $G$. Cho $A$ là tập hợp các phép hoán vị $f$ của $E$ có tính chất sau:
Tồn tại $\gamma \in \Gamma$ sao cho $f$ là một $\gamma$-cấu xạ của $E$ vào $E$ (nghĩa là, $f(gb) = \gamma(g)f(b)$ với $b \in E$ và $g \in G$).
Công thức trên $f(gb) = \gamma(g)f(b)$ cho thấy rằng nếu $f \in A$ thì tồn tại duy nhất $\gamma \in \Gamma$ sao cho $f$ là một $\gamma$-cấu xạ, ta sẽ ký hiệu nó là $p(f)$.
Cho $f, f'$ thuộc $A$, $\gamma = p(f), \gamma' = p(f')$. Khi đó, với mọi $b \in E$ và mọi $g \in G$,
$$
(f' \circ f)(gb) = f'(\gamma(g)f(b)) = \gamma'(\gamma(g))f'(f(b))
$$
điều này chứng minh rằng $f' \circ f \in A$ và rằng $p(f' \circ f) = p(f')p(f)$. Mặt khác, $f(\gamma^{-1}(g)f^{-1}(b)) = gb$, do đó $f^{-1}(gb) = \gamma^{-1}(g)f^{-1}(b)$ và $f^{-1} \in A$. Vậy $A$ là một nhóm con của $\mathcal{S}_E$ và $p$ là một đồng cấu của $A$ vào $\Gamma$. Hạt nhân của $p$ là tập hợp $\mathrm{Aut}_G(E)$ các tự đẳng cấu của $G$-tập hợp $E$.
Ta cố định $a \in E$. Trong § 5, no. 6 ta đã định nghĩa một đẳng cấu $\psi_a$ của $G^0$ lên $\mathrm{Aut}_G(E)$ sao cho $\psi_a(x)(ga) = gxa$ với mọi $g, x$ trong $G$. Mặt khác, với $\gamma \in \Gamma$, gọi $s_a(\gamma)$ là phép hoán vị của $E$ được xác định bởi $s_a(\gamma)(ga) = \gamma(g)a$ với mọi $g \in G$; ta kiểm tra ngay lập tức rằng $s_a$ là một đồng cấu của $\Gamma$ vào $A$ sao cho $p \circ s_a = \mathrm{Id}_{\tau}$. Do đó $G^0 \xrightarrow{\psi_a} A \xrightarrow{p} \Gamma$ là một mở rộng của $\Gamma$ bởi $G^0$ và $s_a$ là một tiết diện của mở rộng này. Mở rộng này và tiết diện này xác định một phép toán của $\Gamma$ trên $G^0$, $s_a(\Gamma)$ tác động lên $\psi_a(G^0)$ bởi các tự đẳng cấu nội; ta viết phép toán này dưới dạng lũy thừa. Ta chứng minh rằng phép toán này là phép toán tự nhiên ($\S 3$, no. 1, Ví dụ 3): với $x, g$ trong $G$ và $\gamma \in \Gamma$,
$$
(\psi_a(\gamma x))(ga) = (s_a(\gamma) \circ \psi_a(x) \circ s_a(\gamma)^{-1})(ga)
= (s_a(\gamma) \circ \psi_a(x))(\gamma^{-1}(g)a) = s_a(\gamma)(\gamma^{-1}(g)xa)
= g\gamma(x)a = \psi_a(\gamma(x))ga
$$
do đó $^\gamma x = \gamma(x)$.
Mệnh đề 4 sau đó cho thấy rằng $A$ là đẳng cấu với tích nửa trực tiếp của $\Gamma = \mathrm{Aut}(G)$ bởi $G^0$ theo phép toán tự nhiên của $\mathrm{Aut}(G)$ trên $G^0$. Chú ý rằng đẳng cấu mà ta đã xây dựng nói chung phụ thuộc vào lựa chọn phần tử $a \in E$.
(2) *Cho $A$ là một vành giao hoán. Nhóm tam giác trên $T(n, A)$ là tích nửa trực tiếp của nhóm con đường chéo $D(n, A)$ bởi nhóm tam giác trên ngặt $T_1(n, A)$.*

### 2. GIAO HOÁN TỬ

#### Định nghĩa 3 {#alg-i-s6-def-3 .statement}

Cho $G$ là một nhóm và $x$ và $y$ là hai phần tử của $G$. Phần tử $x^{-1}y^{-1}xy$ của $G$ được gọi là giao hoán tử của $x$ và $y$.

Ta dùng (x, y) để chỉ giao hoán tử của x và y. Khi đó hiển nhiên
$$(y, x) = (x, y)^{-1}.$$
Điều kiện cần và đủ để x và y giao hoán là $(x, y) = e$. Nói chung,
$$xy = yx(x, y).$$
Mặt khác, ta viết
(3)
$$x^y = y^{-1}xy = x(x, y) = (y, x^{-1})x.$$
Vì ánh xạ $x \mapsto x^y$ là tự đẳng cấu trong $\operatorname{Int}(y^{-1})$, nên $(x, y)^z = (x^z, y^z)$ với mọi $x, y, z \in G$.

Với $x, y, z \in G$, ta chứng minh các hệ thức sau:
(4)
$$(x, yz) = (x, z).(x, y)^z = (x, z).(z, (y, x)).(x, y)$$
(4 bis)
$$(xy, z) = (x, z)^y.(y, z) = (x, z).((x, z), y).(y, z)$$
(5)
$$(x^y, (y, z)).(y^z, (z, y)).(z^x, (x, y)) = e$$
(6)
$$(x, yz).(z, xy).(y, zx) = e$$
(6 bis)
$$(xy, z).(yz, x).(zx, y) = e.$$

Bây giờ
$$
\begin{align*}
(x, yz) &= x^{-1}z^{-1}y^{-1}xyz = (x, z)z^{-1}x^{-1}y^{-1}xyz = (x, z)(x, y)^z \\
&= (x, z)(z, (x, y)^{-1})(x, y)
\end{align*}
$$
theo (3), điều này chứng minh (4). Công thức (4 bis) được suy ra tương tự. Mặt khác,
$$
\begin{align*}
(x^y, (y, z)) &= (x^y)^{-1}(z, y)(x^y)(y, z) \\
&= y^{-1}x^{-1}yz^{-1}y^{-1}zyy^{-1}xyy^{-1}z^{-1}yz \\
&= (yzy^{-1}xy)^{-1}(zxz^{-1}yz).
\end{align*}
$$
Đặt $u = yzy^{-1}xy, v = zxz^{-1}xy$ và $w = xyx^{-1}zx$, ta được
$$(x^y, (y, z)) = u^{-1}v.$$
Bằng cách hoán vị vòng quanh $x, y, z$, ta suy ra $(y^z, (z, x)) = v^{-1}w$ và
$$(z^x, (x, y)) = w^{-1}u,$$
từ đó suy ra ngay lập tức (5). Cuối cùng, (6) được suy ra bằng cách nhân với nhau hai vế của ba công thức thu được bằng cách hoán vị vòng quanh $x, y, z$ trong công thức $(x, yz) = x^{-1}z^{-1}y^{-1}xyz = (yzx)^{-1}(xyz)$, và tương tự đối với (6 bis).

Nếu A và B là hai nhóm con của G, (A, B) ký hiệu nhóm con được sinh bởi các giao hoán tử $(a, b)$ với $a \in A$ và $b \in B$.† Khi đó $(A, B) = \{e\}$ khi và chỉ khi A giao hoán với B. $(A, B) \subset A$ khi và chỉ khi B chuẩn hóa A. Nếu A và B là chuẩn tắc (tương ứng, đặc trưng), thì $(A, B)$ cũng vậy.

† Ở đây chúng tôi bác bỏ quy ước ký hiệu được đưa ra trong § 1, no 1 về việc mở rộng một luật hợp thành cho các tập con.

#### Mệnh đề 5 {#alg-i-s6-prop-5 .statement}

Cho $A, B, C$ là ba nhóm con của $G$.

(i) Nhóm con $A$ chuẩn hóa nhóm con $(A, B)$.

(ii) Nếu nhóm con $(B, C)$ chuẩn hóa $A$, thì nhóm con $(A, (B, C))$ được sinh bởi các phần tử $(a, (b, c))$ với $a \in A, b \in B$ và $c \in C$.

(iii) Nếu $A, B$ và $C$ là chuẩn tắc, thì

$$
(A, (B, C)) \subset (C, (B, A)).(B, (C, A)).
$$

Theo (4 bis), với $a, a' \in A$ và $b \in B$,

$$
(a, b)^{a'} = (aa', b).(a', b)^{-1},
$$

do đó (i). Bây giờ giả sử rằng $(B, C)$ chuẩn hóa $A$. Với $a \in A, b \in B, c \in C$ và $x \in G$, (4) cho

$$
(a, (b, c).x) = (a, x).(x, ((b, c), a))(a, (b, c))
$$

và $((b, c), a) \in A$ vì $(B, C)$ chuẩn hóa $A$, do đó bằng quy nạp theo $p$ ta có rằng $\left( a, \prod_{i=1}^p (b_i, c_i) \right)$, với $b_i \in B, c_i \in C$, thuộc nhóm con sinh bởi các phần tử có dạng $(a, (b, c))$. Nếu cuối cùng $A, B$ và $C$ là chuẩn hóa, thì các nhóm con $(A, (B, C))$, $(C, (B, A))$ và $(B, (C, A))$ cũng vậy. Do đó, theo (ii), chỉ cần chứng minh rằng

$$
(a, (b, c)) \in (C, (B, A)).(B, (C, A))
$$

với mọi $a \in A, b \in B$ và $c \in C$. Bây giờ theo (5), viết $a^{b^{-1}} = u$

$$
(a, (b, c)) = ((u^b), (b, c)) = (c^u, (u, b))^{-1}.(b^c, (c, u))^{-1},
$$

do đó (iii).

#### Định nghĩa 4 {#alg-i-s6-def-4 .statement}

Cho $G$ là một nhóm. Nhóm con được sinh bởi các giao hoán tử của các phần tử của $G$ được gọi là nhóm dẫn xuất của $G$.

Nhóm dẫn xuất của $G$ do đó là nhóm con $(G, G)$. Nó cũng được ký hiệu là $D(G)$. Do lạm dụng ngôn ngữ, đôi khi nó được gọi là *nhóm giao hoán tử* của $G$ mặc dù nói chung nó phân biệt với tập hợp các giao hoán tử của các phần tử của $G$ (Bài tập 16). $D(G) = \{e\}$ khi và chỉ khi $G$ là giao hoán.

#### Mệnh đề 6 {#alg-i-s6-prop-6 .statement}

Cho $f : G \to G'$ là một đồng cấu nhóm. Khi đó $f(D(G)) \subset D(G')$. Nếu $f$ là toàn ánh, đồng cấu của $D(G)$ vào $D(G')$ là hạn chế của $f$ thì là toàn ánh.

Ảnh theo $f$ của một giao hoán tử của các phần tử của $G$ là một giao hoán tử của các phần tử của $G'$. Nếu $f$ là toàn ánh, ảnh theo $f$ của tập hợp các giao hoán tử của $G$ là tập hợp các giao hoán tử của $G'$. Mệnh đề do đó suy ra từ § 4, no. 3, Hệ quả 3 của Mệnh đề 2.

#### Hệ quả 1 {#alg-i-s6-prop-6-cor-1 .statement}

Nhóm dẫn xuất của một nhóm $G$ là một nhóm con đặc số của $G$. Đặc biệt nó là một nhóm con chuẩn của $G$.

#### Hệ quả 2 {#alg-i-s6-prop-6-cor-2 .statement}

Cho G là một nhóm. Nhóm thương G/D(G) là giao hoán. Cho $\pi : G \to G/D(G)$ là đồng cấu chính tắc. Mọi đồng cấu f của G vào một nhóm giao hoán G' có thể được biểu diễn duy nhất dưới dạng $f = \bar{f} \circ \pi$, trong đó $\bar{f} : G/D(G) \to G'$ là một đồng cấu.

Bây giờ $\pi(D(G)) = \{e\}$. Vì $\pi$ là toàn ánh, suy ra rằng $D(G/D(G)) = \{e\}$, do đó mệnh đề thứ nhất. Mệnh đề thứ hai suy ra từ § 4, no. 4, Mệnh đề 5.

#### Hệ quả 3 {#alg-i-s6-prop-6-cor-3 .statement}

Cho H là một nhóm con của G. Các điều kiện sau là tương đương:

(i) $H \supset D(G)$;
(ii) H là một nhóm con chuẩn và $G/H$ là giao hoán.
(ii) $\Rightarrow$ (i) theo Hệ quả 2 và (i) $\Rightarrow$ (ii) theo § 4, no. 7, Định lý 4, vì mọi nhóm con của một nhóm giao hoán là chuẩn.

#### Hệ quả 4 {#alg-i-s6-prop-6-cor-4 .statement}

Cho G là một nhóm và X là một tập con của G sinh ra G. Nhóm D(G) là nhóm con chuẩn của G được sinh bởi các giao hoán tử của các phần tử của X.

Cho H là nhóm con chuẩn của G được sinh bởi các giao hoán tử của các phần tử của X và $\phi : G \to G/H$ là đồng cấu chính tắc. Tập hợp $\phi(X)$ sinh ra $G/H$. Các phần tử của $\phi(X)$ từng đôi một khả hoán và do đó H là giao hoán (§ 4, no. 3, Hệ quả 2 của Mệnh đề 2). Vì vậy (Hệ quả 3) H chứa D(G). Mặt khác, hiển nhiên $H \subset D(G)$.

#### Nhận xét {#alg-i-s6-n2-rem-1 .statement}

(1) Hệ quả 2 cũng có thể được phát biểu bằng cách nói rằng $G/D(G)$, cùng với $\pi$, là một nghiệm của bài toán ánh xạ phổ quát đối với G, liên quan đến các nhóm giao hoán và các đồng cấu từ G đến các nhóm giao hoán.

(2) Dưới các giả thiết của Hệ quả 4, nhóm con được sinh bởi các giao hoán tử của các phần tử của X được chứa trong D(G) nhưng nói chung không bằng D(G) (xem Bài tập 15e).

#### Ví dụ {#alg-i-s6-n2-exa-1 .statement}

(1) Nếu G là một nhóm đơn không giao hoán, thì $D(G) = G$. Do đó mọi đồng cấu của G vào một nhóm giao hoán đều tầm thường.

(2) Nhóm dẫn xuất của nhóm đối xứng $S_n$ là nhóm phản xứng $A_n$. Vì $A_n$ được sinh bởi các tích của hai phép hoán vị chuyển; nếu $\tau = \tau_{x,y}$ và $\tau' = \tau_{x',y'}$ là hai phép hoán vị chuyển, lấy $\sigma$ là một phép hoán vị sao cho $\sigma(x') = x$ và $\sigma(y') = y$. Khi đó $\tau' = \sigma^{-1} \tau \sigma$ và $\tau \tau' = \tau^{-1} \tau' = \tau^{-1} \sigma^{-1} \tau \sigma$ là một giao hoán tử. Suy ra $A_n \subset D(S_n)$. Vì $S_n/A_n$ là giao hoán, $A_n \supset D(S_n)$ (Hệ quả 3).

### 3. CHUỖI TRUNG TÂM DƯỚI, CÁC NHÓM LŨY LINH

Cho G là một nhóm, H là một nhóm con của G và K là một nhóm con chuẩn của G. Ảnh của H trong G/K được chứa trong tâm của G/K khi và chỉ khi $(G, H) \subset K$.

#### Định nghĩa 5 {#alg-i-s6-def-5 .statement}

Cho G là một nhóm. Chuỗi trung tâm dưới của G là dãy $(C^n(G))_{n \geq 1}$ các nhóm con của G được xác định bằng quy nạp bởi:
$$
C^1(G) = G, \quad C^{n+1}(G) = (G, C^n(G)).
$$

Cho $f : G \to G'$ là một đồng cấu nhóm. Bằng quy nạp theo $n$, ta thấy rằng $f(C^n(G)) \subset C^n(G')$ và rằng, nếu $f$ là toàn ánh, $f(C^n(G)) = C^n(G')$. Đặc biệt, với mọi $n \geq 1$, $C^2(G)$ là một nhóm con có đặc số (và do đó là chuẩn) của $G$. Với mọi $n \geq 1$, $C^n(G)/C^{n+1}(G)$ được chứa trong tâm của $G/C^{n+1}(G)$.

Cho $(G_1, G_2, \ldots)$ là một dãy giảm các nhóm con chuẩn của $G$ sao cho (1) $G_1 = G$; (2) với mọi $i$, $G_i/G_{i+1}$ được chứa trong tâm của $G/G_{i+1}$. Khi đó $C^i(G) \subset G_i$, như thấy được bằng quy nạp theo $i$.

Bây giờ
$$
(C^m(G), C^n(G)) \subset C^{m+n}(G).
$$
Vì, nếu quan hệ này được ký hiệu bởi $(F_{m,n})$, thì suy ra từ $(F_{m,n})$, theo No. 2, Mệnh đề 5, rằng
$$
\begin{align*}
(C^m(G), C^{n+1}(G)) &\subset (G, (C^m(G), C^n(G))).(C^n(G), (G, C^m(G))) \\
&\subset C^{m+n+1}(G).(C^{m+1}(G), C^n(G)).
\end{align*}
$$
Do đó $((F_{m,n}) \text{ và } (F_{m+1,n})) \Rightarrow (F_{m,n+1})$. Vì $(F_{m,1})$ và $(F_{1,n})$ là hiển nhiên nên $(F_{m,n})$ suy ra bằng quy nạp.

#### Định nghĩa 6 {#alg-i-s6-def-6 .statement}

*Một nhóm $G$ được gọi là lũy linh nếu tồn tại một số nguyên $n$ sao cho $C^{n+1}(G) = \{e\}$. Số nguyên nhỏ nhất $n$ sao cho $C^{n+1}(G) = \{e\}$ được gọi là lớp lũy linh của một nhóm lũy linh $G$.*

Nếu $n \in \mathbf{N}$, một nhóm có lớp lũy linh $n$ được gọi là một nhóm lũy linh lớp $n$. Đôi khi người ta nói rằng lớp lũy linh của một nhóm $G$ là hữu hạn nếu $G$ là lũy linh.

#### Ví dụ {#alg-i-s6-n3-exa-1 .statement}

(1) Một nhóm là lũy linh lớp 0 (tương ứng $\leq 1$) khi và chỉ khi nó gồm phần tử đơn vị (tương ứng là giao hoán).

(2) *Với mọi vành giao hoán $A$ và mọi số nguyên $n \geq 1$, nhóm tam giác trên ngặt $T_1(n, A)$ là lũy linh có lớp $\leq n - 1$ (và có lớp đúng bằng $n - 1$ nếu $A \neq \{0\}$).*

(3) Cho $G$ là một nhóm lũy linh có lớp $n$. Mọi nhóm con (tương ứng, mọi nhóm thương) của $G$ đều lũy linh có lớp $\leq n$. Thật vậy, nếu $H$ là một nhóm con của $G$, thì $C^n(H) \subset C^n(G)$. Nếu $G'$ là một nhóm thương của $G$ và $\pi : G \to G'$ là đồng cấu chính tắc, thì $C^n(G') = \pi(C^n(G))$.

(4) Tích hữu hạn của các nhóm lũy linh là lũy linh.

#### Mệnh đề 7 {#alg-i-s6-prop-7 .statement}

*Cho $G$ là một nhóm và $n$ là một số nguyên. Các điều kiện sau là tương đương:*

(a) $G$ là lũy linh có lớp $\leq n$.
(b) *Tồn tại một chuỗi các nhóm con của $G$:*
$$
G = G^1 \supset G^2 \supset \ldots \supset G^{n+1} = \{e\}
$$
*sao cho* $(G, G^{k'}) \subset G^{k'+1}$ *với mọi* $k \in \{1, n\}$.

(c) Tồn tại một nhóm con $A$ của $G$ được chứa trong tâm của $G$ sao cho $G/A$ là lũy linh có lớp $\leq n - 1$.

(a) $\Rightarrow$ (b): chỉ cần lấy $G^k = C^k(G)$.
(b) $\Rightarrow$ (a): theo quy nạp theo $k$, $C^k(G) \subset G^k$.
(a) $\Rightarrow$ (c): chỉ cần lấy $A = C^n(G)$.
(c) $\Rightarrow$ (a): đặt $\pi : G \to G/A$ là đồng cấu chính tắc; khi đó $\pi(C^n(G)) = C^n(G/A) = \{e\}$ và do đó $C^n(G) \subset A$, do đó $C^{n+1}(G) = \{e\}$.

Nói ngắn gọn hơn: một nhóm là lũy linh có lớp $\leq n$ nếu nó có thể được thu được từ nhóm $\{e\}$ bằng $n$ mở rộng trung tâm liên tiếp.

#### Hệ quả {#alg-i-s6-n3-cor-1 .statement}

*Một mở rộng trung tâm của một nhóm lũy linh (bởi một nhóm giao hoán tất yếu) là lũy linh.*

#### Mệnh đề 8 {#alg-i-s6-prop-8 .statement}

*Cho $G$ là một nhóm lũy linh có lớp $\leq n$ và $H$ là một nhóm con của $G$. Tồn tại một dãy các nhóm con*

$$
G = H^1 \supset H^2 \supset \ldots \supset H^{n+1} = H,
$$

*sao cho* $H^{k+1}$ *là chuẩn tắc trong* $H^k$ *và* $H^k/H^{k+1}$ *là giao hoán với mọi* $k \leq n$.

Chọn một dãy $(G^k)$ các nhóm con của $G$ thỏa mãn các điều kiện của Mệnh đề 7 (b) với mọi $k$; $G^k$ là chuẩn tắc trong $G$. Đặt:

$$
H^k = H.G^k.
$$

Cần kiểm tra rằng $H^{k+1}$ được chuẩn hóa bởi $H^k = H.G^k$; vì nó được chuẩn hóa bởi $H$, chỉ cần kiểm tra rằng nó được chuẩn hóa bởi $G^k$. Bây giờ, nếu $s \in G^k$ và $h \in H$,

$$
shs^{-1} = shs^{-1}h^{-1}.h \in (G, G^k).H
$$

và $(G, G^k).H$ được chứa trong $G^{k+1}.H = H^{k+1}$; do đó $s.H^{k+1}.s^{-1} = H^{k+1}$, điều này chứng tỏ rằng $H^{k+1}$ là chuẩn tắc trong $H^k$.

Cuối cùng, đồng cấu chính tắc $G^k/G^{k+1} \to H^k/H^{k+1}$ là hiển nhiên toàn ánh; vì nhóm thứ nhất giao hoán, nên nhóm thứ hai cũng vậy.

#### Hệ quả 1 {#alg-i-s6-prop-8-cor-1 .statement}

*Cho $G$ là một nhóm lũy linh và $H$ là một nhóm con của $G$. Nếu $H$ phân biệt với $G$, thì chuẩn hóa tử $N_G(H)$ của $H$ trong $G$ phân biệt với $H$.*

Cho $k$ là chỉ số lớn nhất sao cho $H^k \neq H$. Nhóm $H^k$ chuẩn hóa $H$ và phân biệt với $H$.

#### Hệ quả 2 {#alg-i-s6-prop-8-cor-2 .statement}

*Cho $G$ là một nhóm lũy linh và $H$ là một nhóm con của $G$. Nếu $H$ phân biệt với $G$, tồn tại một nhóm con chuẩn tắc $N$ của $G$, chứa $H$, phân biệt với $G$ và sao cho $G/N$ là giao hoán.*

Cho $k$ là chỉ số nhỏ nhất sao cho $H^k \neq G$. Nhóm $H^k$ thỏa mãn các điều kiện yêu cầu.

#### Hệ quả 3 {#alg-i-s6-prop-8-cor-3 .statement}

*Cho G là một nhóm lũy linh và H là một nhóm con của G. Nếu G = H.(G, G), thì G = H.*

Mọi nhóm con N của G chứa H và sao cho G/N là giao hoán đều chứa H.(G, G). Hệ quả 3 do đó suy ra từ Hệ quả 2.

Hệ quả 3 cũng có thể được phát biểu như sau: cho X là một tập con của G. Để X sinh ra G, điều kiện cần và đủ là ảnh của X trong G/D(G) sinh ra G/D(G).

#### Hệ quả 4 {#alg-i-s6-prop-8-cor-4 .statement}

*Cho f: G' → G là một đồng cấu nhóm. Giả sử rằng*
(a) *G là lũy linh.*
(b) *Đồng cấu f₁: G'/(G', G') → G/(G, G), dẫn xuất từ f bằng cách chuyển qua các thương, là toàn ánh.*
*Khi đó f là toàn ánh.*

Điều này suy ra từ Hệ quả 3 áp dụng cho nhóm con H = f(G').

#### Mệnh đề 9 {#alg-i-s6-prop-9 .statement}

*Cho G là một nhóm lũy linh thuộc lớp ≤ n và cho N là một nhóm con chuẩn tắc của G. Tồn tại một chuỗi các nhóm con*

$$
N = N^1 \supset N^2 \supset \ldots \supset N^{n+1} = \{e\}
$$

*sao cho* (G, N^k) ⊂ N^{k+1} *với k = 1, ..., n.*

Nếu (G^k) thỏa mãn điều kiện (b) của Mệnh đề 7, thì lấy

$$
N^k = G^k \cap N.
$$

#### Hệ quả 1 {#alg-i-s6-prop-9-cor-1 .statement}

*Cho G là một nhóm lũy linh, Z là tâm của G và N là một nhóm con chuẩn tắc của G. Nếu N ≠ {e}, thì N ∩ Z ≠ {e}.*

Cho k là chỉ số lớn nhất sao cho N^k ≠ {e}. Nhóm N^k được chứa trong N. Mặt khác, (G, N^k) ⊂ N^{k+1} = {e}; do đó N^k được chứa trong tâm Z của G.

#### Hệ quả 2 {#alg-i-s6-prop-9-cor-2 .statement}

*Cho f là một đồng cấu từ một nhóm lũy linh G đến một nhóm G'. Nếu hạn chế của f lên tâm của G là đơn ánh, thì f là đơn ánh.*

Đây là Hệ quả 1 được áp dụng cho Ker(f).

### 4. CHUỖI DẪN XUẤT, CÁC NHÓM GIẢI ĐƯỢC

#### Định nghĩa 7 {#alg-i-s6-def-7 .statement}

*Cho G là một nhóm. Chuỗi dẫn xuất của G là chuỗi (D^n(G))_{n \in \mathbf{N}} được xác định bằng quy nạp bởi:*

$$
D^0(G) = G; \quad D^{n+1}(G) = D(D^n(G)) \quad \text{cho } n \in \mathbf{N}.
$$

Khi đó $D^0(G) = C^1(G) = G,\ D^1(G) = C^2(G) = D(G) = (G, G)$. Với mọi n \in \mathbf{N}, D^n(G) \subset C^{2^n}(G), như thấy được bằng quy nạp theo n sử dụng công thức (7) của no. 3.

Cho $f : G \to G'$ là một đồng cấu nhóm. Ta thấy, bằng quy nạp theo n, rằng $f(D^n(G)) \subset D^n(G')$ và rằng, nếu $f$ là toàn ánh, $f(D^n(G)) = D^n(G')$. Đặc biệt, với mọi $n \in \mathbf{N}$, $D^n(G)$ là một nhóm con đặc số (và do đó chuẩn tắc) của G. Với mọi $n \in \mathbf{N}$, nhóm $D^n(G)/D^{n+1}(G)$ là một nhóm con chuẩn tắc giao hoán (nhưng nói chung không phải trung tâm) của $G/D^{n+1}(G)$.

Cho $(G_0, G_1, \ldots)$ là một dãy giảm các nhóm con của G sao cho: (1) $G_0 = G$; (2) với mọi $i$, $G_{i+1}$ là chuẩn trong $G_i$ và $G_i/G_{i+1}$ là giao hoán. Khi đó $D^i(G) \subset G_i$ với mọi $i$, như thấy được bằng quy nạp theo $i$.

#### Định nghĩa 8 {#alg-i-s6-def-8 .statement}

*Một nhóm G được gọi là giải được nếu tồn tại một số nguyên n sao cho $D^n(G) = \{e\}$. Nếu G là một nhóm giải được, số nguyên n nhỏ nhất sao cho $D^n(G) = \{e\}$ được gọi là lớp giải được của G.*

Một nhóm giải được có lớp giải được $n$ được gọi là một nhóm giải được lớp $n$. Một nhóm đôi khi được nói là có lớp giải được hữu hạn nếu nó là giải được.

#### Ví dụ {#alg-i-s6-n4-exa-1 .statement}

(1) Một nhóm là giải được lớp 0 (tương ứng $\leq 1$) khi và chỉ khi nó thu về $\{e\}$ (tương ứng là giao hoán).

(2) Mọi nhóm lũy linh lớp $\leq 2^n - 1$ đều là giải được lớp $\leq n$; điều này suy ra từ quan hệ $D^n(G) \subset C^{2^n}(G)$ đã được chứng minh ở trên.

(3) Cho G là một nhóm giải được lớp $\leq n$. Mọi nhóm con (tương ứng nhóm thương) của G đều là giải được lớp $\leq n$ (chứng minh tương tự như chứng minh của no. 3, Ví dụ 3).

(4) Nếu G là một nhóm giải được lớp $p$ và F là một nhóm giải được lớp $q$, mọi mở rộng E của G bởi F là một nhóm giải được lớp $\leq p + q$. Thật vậy, gọi $\pi : E \to G$ là phép chiếu; khi đó $\pi(D^p(E)) \subset D^p(G) = \{e\}$ và do đó $D^p(E) \subset F$; suy ra $D^{p+q}(E) = D^q(D^p(E)) \subset D^q(F) = \{e\}$.

(5) Nhóm đối xứng $S_n$ là giải được khi và chỉ khi $n < 5$ (xem § 5, các Bài tập 10 và 16).

(6) *Nếu A là một vành giao hoán, nhóm tam giác trên T(n, A) là giải được nhưng nói chung không lũy linh.*

#### Mệnh đề 10 {#alg-i-s6-prop-10 .statement}

*Cho G là một nhóm và n là một số nguyên. Các điều kiện sau là tương đương:*

(i) *G là giải được lớp $\leq n$.*
(ii) *Tồn tại một chuỗi các nhóm con chuẩn của G*
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
*trong đó các nhóm $G^k/G^{k+1}$ là giao hoán.*
(iii) *Tồn tại một chuỗi các nhóm con của G*
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = e
$$
*trong đó, với mọi k, $G^{k+1}$ là một nhóm con chuẩn của $G^k$ và $G^k/G^{k+1}$ là giao hoán.*

(iv) Tồn tại một nhóm con giao hoán chuẩn $A$ của $G$ sao cho $G/A$ là giải được lớp $\leq n - 1$.

Đối với (i) $\Rightarrow$ (ii) chỉ cần lấy $G^k$ bằng $D^k(G)$. (ii) $\Rightarrow$ (iii) là hiển nhiên. (iii) $\Rightarrow$ (i) vì $D^k(G)$ nhất thiết được chứa trong $G^k$. Sự tương đương của (ii) và (iv) là ngay lập tức bằng quy nạp theo $n$.

Nói ngắn gọn hơn: một nhóm là giải được lớp $\leq n$ nếu nó có thể nhận được bằng các mở rộng liên tiếp của $n$ nhóm giao hoán.

#### Hệ quả {#alg-i-s6-n4-cor-1 .statement}

Cho $G$ là một nhóm hữu hạn và
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
là một chuỗi Jordan-Hölder của $G$ Để $G$ là giải được, điều kiện cần và đủ là các nhóm thương $G^k/G^{k+1}$ là cyclic có cấp nguyên tố.

Nếu các nhóm thương của một chuỗi hợp thành của $G$ là cyclic và do đó giao hoán, thì $G$ giải được theo Mệnh đề 10. Ngược lại, nếu $G$ giải được, nhóm $G^k/G^{k+1}$ là, với mọi $k$, giải được và đơn ($\S 4$, no. 7, Mệnh đề 9). Bây giờ, mọi nhóm đơn giải được $H$ đều là cyclic có cấp nguyên tố. Thật vậy, $D(H)$ là một nhóm con chuẩn tắc của $H$; $D(H) = H$ là không thể xảy ra vì trong trường hợp đó $D^k(H) = H$ với mọi $k$; khi đó $D(H) = \{e\}$ và $H$ là giao hoán. Hệ quả suy ra từ $\S 4$, no. 10, Hệ quả của Mệnh đề 20.

### 5. $p$-NHÓM

Trong số này và các số sau, chữ cái $p$ ký hiệu một số nguyên tố ($\S 4$, no 10, Mệnh đề 16).

#### Định nghĩa 9 {#alg-i-s6-def-9 .statement}

Một nhóm hữu hạn có cấp là một lũy thừa của $p$ được gọi là một $p$-nhóm.

Cho $G$ là một $p$-nhóm có cấp $p^r$. Mọi ước của $p^r$ đều là một lũy thừa của $p$ ($\S 4$, no. 10, Hệ quả của Định lý 7). Do đó mọi nhóm con và mọi nhóm thương của $G$ đều là một $p$-nhóm ($\S 4$, no. 4, Hệ quả của Mệnh đề 4); lực lượng của mọi không gian thuần nhất của $G$ là một lũy thừa của $p$ ($\S 5$, no. 5, Định lý 1).

Một mở rộng của một $p$-nhóm bởi một $p$-nhóm là một $p$-nhóm.

*Ví dụ. (1) Một $p$-nhóm giao hoán đẳng cấu với một tích của các nhóm cyclic $\mathbf{Z}/p^n\mathbf{Z}$ (xem Bài tập 19 và cũng VII, $\S 4$, no. 7, Mệnh đề 7).
(2) Cho $k$ là một trường hữu hạn có đặc số $p$. Nhóm tam giác ngặt $T_1(n, k)$ là một $p$-nhóm.
(3) Nhóm quaternion $\{ \pm 1, \pm i, \pm j, \pm k \}$ là một 2-nhóm (xem Bài tập 4).*

#### Mệnh đề 11 {#alg-i-s6-prop-11 .statement}

Cho $E$ là một tập hợp hữu hạn và $G$ là một $p$-nhóm tác động trên $E$. Ký hiệu $E^G$ là tập hợp các $x \in E$ sao cho $gx = x$ với mọi $g \in G$ (các điểm bất động). Khi đó
$$
\operatorname{Card}(E^G) \equiv \operatorname{Card}(E) \pmod{p}.
$$

E — E^G là một hợp rời nhau của các quỹ đạo không thu về một điểm. Lực lượng của một quỹ đạo như vậy là một lũy thừa của $p$ phân biệt với $p^0 = 1$ và do đó là một bội của $p$.

#### Hệ quả {#alg-i-s6-n5-cor-1 .statement}

*Cho G là một p-nhóm. Nếu G không thu về e, thì tâm của nó không thu về e.*

Cho G tác động lên chính nó bởi các tự đẳng cấu nội. Tập hợp các điểm bất động là tâm Z của G. Theo Mệnh đề 11,

$$
\operatorname{Card}(Z) \equiv \operatorname{Card}(G) \equiv 0 \pmod{p},
$$

do đó $\operatorname{Card}(Z) \neq 1$ và $Z \neq \{e\}$.

#### Định lý 1 {#alg-i-s6-thm-1 .statement}

*Cho G là một p-nhóm và $p^r$ là cấp của nó. Tồn tại một dãy các nhóm con của G*

$$
G = G^1 \supset G^2 \supset \ldots \supset G^{r+1} = \{e\}
$$

*sao cho* $(G, G^k) \subset G^{k+1}, 1 \leq k \leq r,$ và $G^k/G^{k+1}, 1 \leq k \leq r,$ *là cyclic có cấp* $p$.

Định lý đúng với $G = \{e\}$. Ta chứng minh nó bằng quy nạp theo $\operatorname{Card}(G)$. Cho Z là tâm của G, $x \neq e$ là một phần tử của Z (Hệ quả của Mệnh đề 11) và $p^s, s \neq 0,$ là cấp của x. Khi đó $x^{p^s - 1}$ là một phần tử có cấp $p$ và do đó Z chứa một nhóm con $G'$ cyclic có cấp $p$. Theo giả thiết quy nạp, nhóm $G' = G/G'$ có một dãy các nhóm con $({G'}^k)_{1 \leq k \leq r}$ với các tính chất yêu cầu. Cho $\pi : G \to G'$ là đồng cấu chính tắc. Dãy các nhóm con của G được xác định bởi $G^k = \pi^{-1}({G'}^k), 1 \leq k \leq r, G^{r+1} = \{e\}$ là một lời giải vì $G^k/G^{k+1}$ đẳng cấu với ${G'}^k/{G'}^{k+1}$ đối với $1 \leq k \leq r$ (\S 4, mục 7, Định lý 4).

#### Hệ quả {#alg-i-s6-n5-cor-2 .statement}

*Mọi p-nhóm đều là lũy linh.*

Điều này suy ra từ mục 3, Mệnh đề 7.

#### Mệnh đề 12 {#alg-i-s6-prop-12 .statement}

*Cho G là một p-nhóm và H là một nhóm con của G phân biệt với G. Khi đó:*

(a) *Bộ chuẩn hoá* $N_G(H)$ *của H trong G phân biệt với G*.
(b) *Tồn tại một nhóm con chuẩn tắc* N *của G có chỉ số p trong G, chứa* H.

Mệnh đề (a) suy ra từ mục 3, Hệ quả 1 của Mệnh đề 8. Ta chứng minh (b). Theo mục 3, Hệ quả 2 của Mệnh đề 8, tồn tại một nhóm con chuẩn tắc $N'$ của G chứa H, phân biệt với G và sao cho $G/N'$ là giao hoán. Cho N là một nhóm con cực đại phân biệt với G chứa $N'$. Khi đó N là chuẩn tắc (mục 2, Hệ quả 3 của Mệnh đề 6) và $G/N$ là một p-nhóm giao hoán đơn và do đó cyclic có cấp $p$ (\S 4, mục 10, Hệ quả của Mệnh đề 20).

#### Hệ quả {#alg-i-s6-n5-cor-3 .statement}

*Cho G là một p-nhóm. Mọi nhóm con của G có chỉ số p đều là chuẩn tắc.*

### 6. CÁC NHÓM CON SYLOW

#### Định nghĩa 10 {#alg-i-s6-def-10 .statement}

Cho G là một nhóm hữu hạn. Một p-nhóm con Sylow của G là bất kỳ nhóm con P nào của G thỏa mãn hai điều kiện sau:

(a) P là một p-nhóm.
(b) (G : P) không là bội của p.

Nếu cấp của G được viết dưới dạng $p^r m$, trong đó m không là bội của $p$, thì các điều kiện (a) và (b) tương đương với $\mathrm{Card}(P) = p^r$.

#### Ví dụ {#alg-i-s6-n6-exa-1 .statement}

(1) Trong nhóm $\mathfrak{S}_p$ cho $\zeta$ là một chu trình có cấp $p$. Nhóm con sinh bởi $\zeta$ là một p-nhóm con Sylow của $\mathfrak{S}_p$ vì $p$ không chia hết $(p - 1)!$.
(2) *Cho k là một trường hữu hạn có đặc số $p$ và cho n là một số nguyên dương. Nhóm tam giác ngặt $T_1(n, k)$ là một p-nhóm con Sylow của nhóm $\mathbf{GL}(n, k)$.*

#### Định lý 2 {#alg-i-s6-thm-2 .statement}

Mọi nhóm hữu hạn đều chứa một p-nhóm con Sylow.

Chứng minh định lý phụ thuộc vào bổ đề sau.

#### Bổ đề {#alg-i-s6-n6-lem-1 .statement}

Cho $n = p^r m$, trong đó m là một số nguyên không là bội của $p$. Khi đó
$$
\binom{n}{p^r} \not\equiv 0 \pmod{p}.
$$

Cho S là một nhóm có cấp $p^r$ (ví dụ $\mathbf{Z}/p^r \mathbf{Z}$) và T là một tập hợp có m phần tử. Đặt $X = S \times T$ và cho E là tập hợp các tập con của X có $p^r$ phần tử. Khi đó $\mathrm{Card}(X) = n$, do đó $\mathrm{Card}(E) = \binom{n}{p^r}$ (Lý thuyết tập hợp, III, § 5, mục 8, Hệ quả 1 của Mệnh đề 11). Cho S tác động lên X bởi $s.(x, y) = (sx, y) (s, x \in S, y \in T)$ và xét phép mở rộng chính tắc của phép toán này đến E. Theo ký hiệu ở mục 5, Mệnh đề 11, tập $E^S$ là tập hợp các quỹ đạo của X, tức là tập hợp các tập con $Y \subset X$ có dạng $S \times \{ t \}, t \in T$, do đó $\mathrm{Card}(E^S) = m$. Theo mục 5, Mệnh đề 11,
$$
\binom{n}{p^r} = \mathrm{Card}(E) \equiv \mathrm{Card}(E^S) = m \not\equiv 0 \pmod{p},
$$
điều này chứng minh bổ đề.

Chúng ta bây giờ chứng minh định lý. Cho G là một nhóm hữu hạn và n là cấp của nó; ta viết $n = p^r m$, trong đó m không là bội của $p$. Cho E là tập hợp các tập con của G có $p^r$ phần tử. Khi đó
$$
\mathrm{Card}(E) = \binom{n}{p^r};
$$
do đó, nhờ bổ đề, $\mathrm{Card}(E) \not\equiv 0 \pmod{p}$. Xét sự mở rộng lên E của phép toán của G trên chính nó bởi phép tịnh tiến trái. Tồn tại $X \in E$ sao cho quỹ đạo của nó có số lực lượng khác 0 mod. $p$. Nếu $H_X$ ký hiệu nhóm ổn định của X, thì

(G:H_x) \not\equiv 0 \pmod{p}, điều đó có nghĩa là $p^r$ chia Card(H_x). Nhưng H_x gồm các $s \in G$ sao cho $sX = X$; nếu $x \in X$, thì $H_x \subset X.x^{-1}$, do đó Card(H_x) $\leqslant$ Card(X) = $p^r$. Suy ra Card(H_x) = $p^r$.

#### Hệ quả {#alg-i-s6-n6-cor-1 .statement}

*Nếu cấp của G chia hết cho p, thì nhóm G chứa một phần tử có cấp p.*

Nhờ Định lý 2, điều này quy về trường hợp G là một $p$-nhóm $\neq \{e\}$; nếu $x \in G$ khác e, thì nhóm tuần hoàn được sinh bởi x khi đó có cấp $p^n$ với $n \geqslant 1$ và do đó nó chứa một nhóm con có cấp $p$.

#### Nhận xét {#alg-i-s6-n6-rem-1 .statement}

Với mỗi số nguyên tố q chia Card(G), cho P_q là một q-nhóm Sylow của G. Khi đó nhóm con H của G được sinh bởi các P_q có cấp là một bội của Card(P_q) đối với mỗi q và có cấp là một ước của Card(G), do đó H bằng G.

#### Định lý 3 {#alg-i-s6-thm-3 .statement}

*Cho G là một nhóm hữu hạn.*
(a) *Các p-nhóm Sylow của G liên hợp với nhau. Số lượng của chúng đồng dư với 1 mod. p.*
(b) *Mọi nhóm con của G là một p-nhóm đều được chứa trong một p-nhóm Sylow.*

Cho P là một p-nhóm Sylow của G (Định lý 2) và cho H là một p-nhóm của G. Cho E = G/P và xét phép toán của H trên G/P. Vì Card(E) $\not\equiv 0$ mod. $p$, Mệnh đề 11 của no. 5 cho thấy tồn tại $x \in G/P$ sao cho $hx = x$ với mọi $h \in H$. Nếu g là một đại diện của x trong G, điều đó có nghĩa là $H \subset gPg^{-1}$, do đó mệnh đề (b).

Nếu H là một p-nhóm Sylow, thì Card(H) = Card(P) = Card($gPg^{-1}$), do đó $H = gPg^{-1}$, điều này chứng minh mệnh đề thứ nhất của (a).

Chúng ta bây giờ chứng minh mệnh đề thứ hai của (a). Cho $\mathcal{S}$ là tập hợp các p-nhóm Sylow của G và cho P tác động lên $\mathcal{S}$ bởi các tự đẳng cấu nội. Phần tử $P \in \mathcal{S}$ là một điểm bất động đối với phép toán này, ta chứng minh rằng đó là điểm duy nhất. Cho $Q \in \mathcal{S}$ là một điểm bất động; Q là một p-nhóm Sylow của G được P chuẩn hóa và do đó P được chứa trong nhóm chuẩn hóa N của Q. Các nhóm P và Q là các p-nhóm Sylow của N; do đó tồn tại $n \in N$ sao cho $P = nQn^{-1} = Q$. Theo no. 5, Mệnh đề 11, Card($\mathcal{S}^P$) $\equiv$ Card($\mathcal{S}^{P^P}$) = 1 (mod. $p$).

#### Hệ quả 1 {#alg-i-s6-thm-3-cor-1 .statement}

*Cho P là một p-nhóm Sylow của G, cho N là nhóm chuẩn hóa của nó trong G và cho M là một nhóm con của G chứa N. Nhóm chuẩn hóa của M trong G bằng M.*

Cho $s \in G$ sao cho $sMs^{-1} = M$. Nhóm con $sPs^{-1}$ của M là một p-nhóm Sylow của M. Do đó tồn tại $t \in M$ sao cho $sPs^{-1} = tPt^{-1}$; khi đó $t^{-1}s \in N$, do đó $s \in tN \subset M$.

#### Hệ quả 2 {#alg-i-s6-thm-3-cor-2 .statement}

*Cho $f : G_1 \to G_2$ là một đồng cấu của các nhóm hữu hạn. Với mỗi p-nhóm Sylow $P_1$ của $G_1$ tồn tại một p-nhóm Sylow $P_2$ của $G_2$ sao cho $f(P_1) \subset P_2$.*

Điều này suy ra từ Định lý 3 (b) áp dụng cho nhóm con $f(P_1)$ của $G_2$.

#### Hệ quả 3 {#alg-i-s6-thm-3-cor-3 .statement}

(a) Cho $H$ là một nhóm con của $G$. Với mỗi nhóm con Sylow $p$ $P$ của $H$ luôn tồn tại một nhóm con Sylow $p$ $Q$ của $G$ sao cho $P = Q \cap H$.

(b) Ngược lại, nếu $Q$ là một nhóm con Sylow $p$ của $G$ và $H$ là chuẩn tắc trong $G$, thì nhóm $Q \cap H$ là một nhóm con Sylow $p$ của $H$.

(a) $p$-nhóm $P$ được chứa trong một nhóm con Sylow $p$ $Q$ của $G$ và $Q \cap H$ là một $p$-nhóm con của $H$ chứa $P$ và do đó bằng $P$.

(b) Cho $P'$ là một nhóm con Sylow $p$ của $H$. Tồn tại một phần tử $g \in G$ sao cho $gP'g^{-1} \subset Q$. Vì $H$ là chuẩn tắc, $P = gP'g^{-1}$ được chứa trong $H$ và do đó trong $Q \cap H$. Vì $Q \cap H$ là một $p$-nhóm con của $H$ và $P$ là một nhóm con Sylow $p$ của $H$, $P = Q \cap H$.

#### Hệ quả 4 {#alg-i-s6-thm-3-cor-4 .statement}

Cho $N$ là một nhóm con chuẩn tắc của $G$. Ảnh trong $G/N$ của một nhóm con Sylow $p$ của $G$ là một nhóm con Sylow $p$ của $G/N$ và mọi nhóm con Sylow $p$ của $G/N$ đều thu được theo cách này.

Cho $G' = G/N$ và $P'$ là ảnh trong $G'$ của một nhóm con Sylow $p$ $P$ của $G$. Nhóm $G$ tác động bắc cầu trên $G'/P'$ và do đó $G'/P'$ có cùng số phần tử với $G/S$, trong đó $S$ là một nhóm con của $G$ chứa $P$. Vì vậy $(G':P')$ chia hết $(G:P)$, nên không phải là bội của $p$ và $p$-nhóm $P'$ là một nhóm con Sylow $p$ của $G'$. Cho $Q'$ là một nhóm con Sylow $p$ khác của $G'$; khi đó $Q' = g'P'{g'}^{-1}$ với một $g' \in G'$ nào đó; nếu $g \in G$ là một đại diện của $g'$, thì nhóm $Q'$ là ảnh của $Q = gPg^{-1}$.

### 7. CÁC NHÓM HỮU HẠN LŨY LINH

#### Định lý 4 {#alg-i-s6-thm-4 .statement}

Cho $G$ là một nhóm hữu hạn. Các điều kiện sau là tương đương:

(a) $G$ là lũy linh.
(b) $G$ là một tích của các $p$-nhóm.
(c) Với mọi số nguyên tố $p$ đều tồn tại một nhóm con Sylow $p$ chuẩn của $G$.
(b) $\Rightarrow$ (a) (mục 5, Hệ quả của Định lý 1).

Giả sử (a) đúng và cho $P$ là một nhóm con Sylow $p$ của $G$. Nếu $N$ là nhóm chuẩn hoá của $P$ trong $G$, Hệ quả 1 của Định lý 3 cho thấy rằng $N$ là nhóm chuẩn hoá của chính nó. Theo § 6, no. 3, Hệ quả của Mệnh đề 8, điều đó suy ra $N = G$. Do đó (a) $\Rightarrow$ (c).

Giả sử (c) đúng và cho $I$ là tập hợp các số nguyên tố chia hết $\mathrm{Card}(G)$. Với mọi $p \in I$, cho $P_p$ là một $p$-nhóm Sylow chuẩn tắc của $G$. Với mọi $p \neq q$, $P_p \cap P_q$ chỉ còn $e$ vì nó vừa là một $p$-nhóm vừa là một $q$-nhóm, nên $P_p$ và $P_q$ trung tâm hóa lẫn nhau ($\S 4$, no. 9, Proposition 15). Cho $\phi$ là đồng cấu chính tắc ($\S 4$, no. 9, Proposition 12) của $\prod_{p \in I} P_p$ vào $G$. Đồng cấu $\phi$ là toàn ánh theo Nhận xét của no. 6. Vì $\mathrm{Card}\left(\prod_{p \in I} P_p\right) = \mathrm{Card}(G)$, suy ra $\phi$ là song ánh.

#### Nhận xét {#alg-i-s6-n7-rem-1 .statement}

(1) Cho $G$ là một nhóm hữu hạn và $p$ là một số nguyên tố. Theo no. 6, Định lý 3 (a) và no. 6, Định lý 2, các điều kiện sau là tương đương:
(i) tồn tại một $p$-nhóm Sylow chuẩn tắc của $G$;
(ii) mọi $p$-nhóm Sylow của $G$ đều chuẩn tắc;
(iii) chỉ tồn tại một $p$-nhóm Sylow của $G$.

(2) Cho $G$ là một nhóm hữu hạn lũy linh. Cho $I$ là tập hợp các ước nguyên tố của $\mathrm{Card}(G)$. Theo Định lý 4 và Nhận xét 1, $G = \prod_{p \in I} G_p$, trong đó $G_p$ là $p$-nhóm Sylow duy nhất của $G$.

(3) Áp dụng cho các nhóm giao hoán, Định lý 4 cho phân tích các nhóm hữu hạn giao hoán thành tích của các thành phần nguyên sơ, điều này sẽ được khảo sát từ một quan điểm khác trong Chương VII.

#### Ví dụ {#alg-i-s6-n7-exa-1 .statement}

Nhóm $\mathfrak{S}_3$ có cấp 6. Nó chứa một $3$-nhóm Sylow chuẩn tắc có cấp 3: nhóm $A_3$. Nó chứa ba $2$-nhóm Sylow có cấp 2: các nhóm $\{e, \tau\}$, trong đó $\tau$ là một hoán vị đổi chỗ. Như vậy nhóm $\mathfrak{S}_3$ không lũy linh.

### Bài tập {#alg-i-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
