---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 1
section_title: Lie groups
lang: vi
source: lie-i-iii
pdf_pages: 0227-0251, 0388-0390
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A LIE GROUP
      page: 0
      pdf_page: 227
    - "no": 2
      title: MORPHISMS OF LIE GROUPS
      page: 0
      pdf_page: 231
    - "no": 3
      title: LIE SUBGROUPS
      page: 0
      pdf_page: 232
    - "no": 4
      title: SEMI-DIRECT PRODUCTS OF LIE GROUPS
      page: 0
      pdf_page: 233
    - "no": 5
      title: QUOTIENT OF A MANIFOLD BY A LIE GROUP
      page: 0
      pdf_page: 235
    - "no": 6
      title: HOMOGENEOUS SPACES AND QUOTIENT GROUPS
      page: 0
      pdf_page: 237
    - "no": 7
      title: ORBITS
      page: 0
      pdf_page: 240
    - "no": 8
      title: VECTOR BUNDLES WITH OPERATORS
      page: 0
      pdf_page: 241
    - "no": 9
      title: LOCAL DEFINITION OF A LIE GROUP
      page: 0
      pdf_page: 244
    - "no": 10
      title: GROUP GERMS
      page: 0
      pdf_page: 246
    - "no": 11
      title: LAW CHUNKS OF OPERATION
      page: 0
      pdf_page: 249
statements: 54
exercises: 10
content_sha256: 4bdfc293d1f16b398c8ea54d542999896a8b6d2d566c3d1f0d1197be51f8b5a9
translated_from: content/en/lie/III/01_s1_lie_groups.md
source_content_sha256: dd2d78e49a8cf1c806338cbfc272462a001b25086267bd90fe9ce27fd5ddf915
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4
translation_run: translate-vi-6a201bc1
glossary_version: 34
glossary_terms_sha256: 34558afb06b7341dfe7c3ec61765ca805c3ce8d713b68663799ee853e4af4717
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. NHÓM LIE

### 1. ĐỊNH NGHĨA NHÓM LIE

Cho G là một tập hợp. Một cấu trúc nhóm và một cấu trúc đa tạp K giải tích trên G được gọi là tương thích nếu điều kiện sau đây được thỏa mãn:
(GL) Ánh xạ $(g, h) \mapsto gh^{-1}$ của $G \times G$ vào G là giải tích.

#### Định nghĩa 1 {#lie-iii-s1-def-1 .statement}

*Một nhóm Lie trên K là một tập hợp G cùng với một cấu trúc nhóm và một cấu trúc đa tạp K giải tích sao cho hai cấu trúc này tương thích.*

Một nhóm Lie trên $\mathbf{R}$ (tương ứng $\mathbf{C}$, $\mathbf{Q}_p$) được gọi là nhóm Lie thực (tương ứng phức, $p$-adic).

Cho G là một nhóm với một cấu trúc đa tạp giải tích. Với $g, h, g_0, h_0$ trong G,
$$
gh^{-1} = (g_0 h_0^{-1}) h_0 ((g_0^{-1} g)(h_0^{-1} h)^{-1}) h_0^{-1}.
$$
Suy ra G là một nhóm Lie khi và chỉ khi ba điều kiện sau được thỏa mãn:

(GL$_1$) với mọi $g_0 \in G$, ánh xạ $g \mapsto g_0 g$ của G vào G là giải tích;
(GL$_2$) với mọi $g_0 \in G$, ánh xạ $g \mapsto g_0 g g_0^{-1}$ của G vào G là giải tích trong một lân cận mở của $e$;
(GL$_3$) ánh xạ $(g, h) \mapsto gh^{-1}$ của $G \times G$ vào G là giải tích trong một lân cận mở của $(e, e)$.

Cho G là một nhóm Lie. Với mọi $g \in G$, $\gamma(g)$ và $\delta(g)$ là các tự đẳng cấu của đa tạp cơ sở của G. Suy ra đa tạp này là thuần nhất (*Differentiable and Analytic Manifolds*, R, 5.1.7). Đặc biệt, chiều của G tại $g$ bằng $\dim G$ với mọi $g \in G$ (nhắc lại rằng $\dim G$ là một số nguyên $\geqslant 0$ hoặc $+\infty$).

Vì một ánh xạ giải tích là liên tục, một nhóm Lie là một nhóm tôpô với tôpô cơ sở của cấu trúc đa tạp của nó. Cho G là một tập hợp. Một cấu trúc nhóm tôpô và một cấu trúc đa tạp K giải tích trên G được gọi là *tương thích* nếu cấu trúc nhóm và cấu trúc đa tạp tương thích và tôpô trên G là tôpô cơ sở của cấu trúc đa tạp.

#### Bổ đề 1 {#lie-iii-s1-lem-1 .statement}

*Cho G là một nhóm Lie, U là một lân cận mở của e, E là một không gian định chuẩn đầy đủ và $\phi : U \to E$ là một bản đồ của đa tạp G. Tồn tại một lân cận W của e được chứa trong U sao cho $\phi | W$ là một đẳng cấu của W (với cấu trúc đều phải) lên $\phi(W)$ (với cấu trúc đều cảm sinh bởi cấu trúc đều trên E).*

Có thể giả sử rằng $\phi(e) = 0$. Đặt $U' = \phi(U)$. Gọi $\psi : U' \to U$ là ánh xạ nghịch đảo của $\phi$. Cho V là một lân cận mở đối xứng của e sao cho $V^2 \subset U$ và đặt $V' = \phi(V)$. Ta định nghĩa các ánh xạ $\theta_1, \theta_2$ từ $V' \times V'$ vào $V' \times U'$ như sau:
$$
\begin{align*}
\theta_1(x, y) &= (x, \phi(\psi(x)\psi(y)^{-1})) \\
\theta_2(x, y) &= (x, \phi(\psi(y)^{-1}\psi(x))).
\end{align*}
$$
Ngay lập tức kiểm tra được rằng $\theta_2(\theta_1(x, y)) = \theta_1(\theta_2(x, y)) = (x, y)$ với $x, y$ đủ gần 0. Mặt khác, $\theta_1$ và $\theta_2$ là giải tích và do đó khả vi nghiêm ngặt tại $(0, 0)$. Do đó (*Differentiable and Analytic Manifolds*, R, 1.2.2) tồn tại một lân cận $W'$ của 0 trong $V'$ và các hằng số $a > 0, b > 0$ sao cho
$$
a(\|x_1 - x_2\| + \|\phi(\psi(x_1)\psi(y_1)^{-1}) - \phi(\psi(x_2)\psi(y_2)^{-1})\|)
\leq \|x_1 - x_2\| + \|y_1 - y_2\|
\leq b(\|x_1 - x_2\| + \|\phi(\psi(x_1)\psi(y_1)^{-1}) - \phi(\psi(x_2)\psi(y_2)^{-1})\|)
$$

với mọi $x_1, x_2, y_1, y_2$ trong $W'$. Đặt $x_1 = x_2 = y_2$, ta được

$$
(2) \quad a \| \phi(\psi(x_1)\psi(y_1)^{-1}) \| \leq \| x_1 - y_1 \| \leq b \| \phi(\psi(x_1)\psi(y_1)^{-1}) \|.
$$

Với $\delta > 0$, đặt $N_\delta$ là tập hợp các cặp có thứ tự $(x, y) \in W' \times W'$ sao cho $\| x - y \| \leq \delta$. Các $N_\delta$ tạo thành một hệ cơ bản các lân cận đồng đều trong $W'$. Ta viết $W = \psi(W')$. Đặt $M_\delta$ là tập hợp các cặp có thứ tự $(u, v) \in W \times W$ sao cho $\| \phi(uv^{-1}) \| \leq \delta$. Các $M_\delta$ tạo thành một hệ cơ bản các lân cận đồng đều trong $W$ với cấu trúc đồng đều phải. Nhưng quan hệ (2) chứng minh rằng

$$
N_\delta \subset (\phi \times \phi)(M_{a^{-1}\delta}), \qquad (\phi \times \phi)(M_\delta) \subset N_{b\delta}
$$

và do đó $W$ có tính chất của bổ đề.

#### Mệnh đề 1 {#lie-iii-s1-prop-1 .statement}

*Một nhóm Lie là một nhóm tôpô đầy đủ mêtric hóa được.*

Vì $e$ có một lân cận mở đồng phôi với một quả cầu mở của một không gian định chuẩn, nên $e$ có một hệ cơ bản đếm được các lân cận có giao là $\{e\}$. Do đó $G$ là mêtric hóa được (*General Topology*, Chương III, § 1, Hệ quả của Mệnh đề 2 và Chương IX, § 3, Mệnh đề 1). Theo Bổ đề 1, tồn tại một lân cận của $e$ đầy đủ đối với cấu trúc đồng đều phải và do đó $G$ là đầy đủ (*General Topology*, Chương III, § 3, Mệnh đề 4).

#### Mệnh đề 2 {#lie-iii-s1-prop-2 .statement}

*Cho $G$ là một nhóm Lie.*
(i) *Nếu $K = \mathbf{R}$ hoặc $\mathbf{C}$, $G$ là liên thông địa phương.*
(ii) *Nếu $K$ phân biệt với $\mathbf{R}$ và $\mathbf{C}$, $G$ là chiều không* (*General Topology*, Chương IX, § 6, Định nghĩa 5).
(iii) *Giả sử rằng $K$ là compact địa phương. Để $G$ là compact địa phương, điều kiện cần và đủ là $G$ có hữu hạn chiều.*
(iv) *Nếu $G$ được sinh bởi một không gian con mà tôpô của nó có một cơ sở đếm được, thì tôpô trên $G$ có một cơ sở đếm được.*

Cho $U$ là một lân cận của $e$. Tồn tại một lân cận mở $U_1$ của $e$ được chứa trong $U$ và đồng phôi với một quả cầu mở của một không gian định chuẩn $E$ trên $K$. Nếu $K = \mathbf{R}$ hoặc $\mathbf{C}$, $U_1$ liên thông, điều này chứng minh (i). Giả sử rằng $K$ là siêu mêtric. Tồn tại một lân cận $U_2$ của $e$ đóng trong $G$ và sao cho $U_2 \subset U_1$. Khi đó tồn tại một lân cận $U_3$ của $e$ sao cho $U_3 \subset U_2$ và $U_3$ vừa mở vừa đóng tương đối với $U_1$. Khi đó $U_3$ đóng tương đối với $U_2$ và do đó với $G$, và mở tương đối với $U_1$ và do đó với $G$. Điều này chứng minh (ii). Để $G$ là compact địa phương, điều kiện cần và đủ là $E$ compact địa phương; nếu $K$ compact địa phương, điều này tương đương với việc nói rằng $E$ hữu hạn chiều (*Topological Vector Spaces*, Chương I, § 2, Định lý 3), do đó có (iii). Giả sử rằng $G$ được sinh bởi một tập con $V$ và đặt $W = V \cup V^{-1}$; khi đó

$$
G = W \cup W^2 \cup W^3 \cup \ldots;
$$

nếu tồn tại một dãy trù mật trong $V$, ta thấy rằng tồn tại một dãy trù mật trong G và, vì G mêtric hóa được (Mệnh đề 1), tôpô trên G thừa nhận một cơ sở đếm được.

#### Hệ quả {#lie-iii-s1-n1-cor-1 .statement}

Nếu K = R hoặc C và G liên thông và hữu hạn chiều, thì G liên thông địa phương và compact địa phương và tôpô của nó thừa nhận một cơ sở đếm được.

#### Bổ đề 2 {#lie-iii-s1-lem-2 .statement}

Cho X là một đa tạp thuộc lớp C^r, e là một điểm của X, U và V là các lân cận mở của e và m là một ánh xạ thuộc lớp C^r từ U × U vào X thỏa mãn các điều kiện sau:
(a) m(e, x) = m(x, e) = x với mọi x ∈ U;
(b) V ⊂ U, m(V × V) ⊂ U và m(m(x, y), z) = m(x, m(y, z)) với mọi x, y, z trong V.

Khi đó tồn tại một lân cận mở W của e trong V và một tự đẳng cấu θ của đa tạp W sao cho θ(e) = e, θ(θ(x)) = x và m(x, θ(x)) = m(θ(x), x) = e với mọi x ∈ W.

m(e, y) = y với mọi y ∈ U và do đó, theo định lý hàm ẩn, tồn tại một lân cận mở W_1 của e trong V và một ánh xạ θ_1 thuộc lớp C^r từ W_1 vào V sao cho θ_1(e) = e, m(x, θ_1(x)) = e với mọi x ∈ W_1. Tương tự, tồn tại một lân cận mở W_2 của e trong V và một ánh xạ θ_2 thuộc lớp C^r từ W_2 vào V sao cho θ_2(e) = e, m(θ_2(x), x) = e với mọi x ∈ W_2. Với x ∈ W_1 ∩ W_2,

$$
\begin{align*}
θ_2(x) &= m(θ_2(x), e) = m(θ_2(x), m(x, θ_1(x))) \\
&= m(m(θ_2(x), x), θ_1(x)) = m(e, θ_1(x)) = θ_1(x).
\end{align*}
$$

Gọi θ(x) là giá trị chung của θ_1(x) và θ_2(x) đối với x ∈ W_1 ∩ W_2. Gọi W là tập hợp các x ∈ W_1 ∩ W_2 sao cho θ(x) ∈ W_1 ∩ W_2. Tập hợp W là mở. Với x ∈ W,

$$
θ(θ(x)) = m(m(x, θ(x)), θ(θ(x))) = m(x, m(θ(x), θ(θ(x)))) = m(x, e) = x
$$

và do đó θ(x) ∈ W. Ta thấy rằng θ | W xác định một tự đẳng cấu của đa tạp W.

#### Mệnh đề 3 {#lie-iii-s1-prop-3 .statement}

Cho X là một đa tạp giải tích và m là một luật hợp thành kết hợp giải tích trên X thừa nhận một phần tử đơn vị. Tập hợp G các phần tử khả nghịch của X là mở trong X và G là một nhóm Lie với m | (G × G) và cấu trúc đa tạp cảm sinh bởi cấu trúc trên X.

Theo Bổ đề 2, G là một lân cận của phần tử đơn vị. Với mọi g ∈ G, ánh xạ x ↦ m(g, x) là một tự đẳng cấu của đa tạp X. Do đó ảnh của G qua ánh xạ này là một lân cận của g, hiển nhiên được chứa trong G. Vì vậy G là mở trong X. Rõ ràng các điều kiện (GL_1) và (GL_2) được thỏa mãn. Điều kiện (GL_3) được thỏa mãn theo Bổ đề 2.

Ví dụ về các nhóm Lie

(1) Cho E là một không gian định chuẩn đầy đủ trên K. Ánh xạ (x, y) ↦ x − y từ E × E vào E là liên tục và tuyến tính và do đó là giải tích.

Do đó E, với cấu trúc nhóm cộng và các cấu trúc đa tạp giải tích của nó, là một nhóm Lie.

Đặc biệt, K là một nhóm Lie.

(2) Cho A là một đại số kết hợp có đơn vị định chuẩn đầy đủ trên K. Phép nhân $(x, y) \mapsto xy$ của $A \times A$ vào A là song tuyến tính và liên tục và do đó là giải tích. Mệnh đề 3 chỉ ra rằng nhóm $A^*$ các phần tử khả nghịch của A là mở trong A (điều này cũng suy ra từ *General Topology*, Chương IX, § 3, Mệnh đề 13) và rằng $A^*$ là một nhóm Lie.

Ví dụ, cho E là một không gian định chuẩn đầy đủ trên K và cho $A = \mathcal{L}(E)$ (*General Topology*, Chương IX, § 3, Mệnh đề 5). Khi đó $A^*$ là nhóm tự đẳng cấu $\mathbf{GL}(E)$ của E. *Nhóm này do đó có một cách chính tắc một cấu trúc nhóm Lie trên K*. Cụ thể hơn, $\mathbf{GL}(n, K)$, với cấu trúc đa tạp cảm sinh bởi cấu trúc trên $\mathbf{M}_n(K)$, là một nhóm Lie. Với $n = 1$, ta thấy rằng nhóm nhân $K^*$ là một nhóm Lie với cấu trúc đa tạp cảm sinh bởi cấu trúc trên K.

(3) Cho G là một nhóm Lie trên K. Cho $K' = \mathbf{R}$ hoặc $\mathbf{C}$ hoặc một trường siêu mêtric đầy đủ không rời rạc và $\sigma$ là một đẳng cấu của trường định giá $K'$ lên một trường con định giá của K. Khi đó nhóm G, với cấu trúc $K'$-đa tạp thu được bằng hạn chế vô hướng, là một nhóm Lie trên $K'$, được gọi là *dẫn xuất từ nhóm Lie G bởi hạn chế vô hướng* (từ K đến $K'$ bằng cách sử dụng $\sigma$). Ví dụ, mọi nhóm Lie phức có một cách chính tắc một cấu trúc nhóm Lie thực. Một lần nữa, với mỗi nhóm Lie phức G được liên kết một nhóm Lie phức gọi là *liên hợp* của G, dẫn xuất từ G bằng tự đẳng cấu $z \mapsto \overline{z}$ của $\mathbf{C}$.

### 2. CÁC CẤU XẠ CỦA NHÓM LIE

#### Định nghĩa 2 {#lie-iii-s1-def-2 .statement}

*Cho G và H là các nhóm Lie. Một cấu xạ nhóm Lie từ G vào H (hoặc đơn giản là một cấu xạ từ G vào H nếu không thể có nhầm lẫn) là một ánh xạ từ G vào H là một đồng cấu nhóm và là giải tích. Nhóm tự đẳng cấu của G được ký hiệu bởi $\operatorname{Aut}(G)$.*.

Ánh xạ đồng nhất của G là một cấu xạ. Hợp thành của hai cấu xạ là một cấu xạ. Nếu $f : G \to H$ và $f' : H \to G$ là hai cấu xạ nghịch đảo, $f$ và $f'$ là các đẳng cấu nhóm Lie.

#### Ví dụ {#lie-iii-s1-n2-exa-1 .statement}

(1) Cho G là một nhóm Lie. Với mọi $x \in G$, $\operatorname{Int}(x)$ là một tự đẳng cấu của nhóm Lie G.

(2) Cho G là một nhóm Lie. Ký hiệu $G^\vee$ là nhóm đối của G, với cùng cấu trúc đa tạp như G. Ngay lập tức thấy rằng $G^\vee$ là một nhóm Lie (gọi là nhóm Lie *đối* của G) và ánh xạ $g \mapsto g^{-1}$ là một đẳng cấu của nhóm Lie G lên nhóm Lie $G^\vee$.

(3) Cho G là một nhóm Lie và E là một không gian chuẩn hóa đầy đủ. Một *biểu diễn tuyến tính giải tích* của G trên E (hay đơn giản là một biểu diễn tuyến tính của G trên E khi không thể có nhầm lẫn) là một cấu xạ của nhóm Lie G vào nhóm Lie $\mathbf{GL}(E)$, nói cách khác là một ánh xạ giải tích $\pi$ từ G vào $\mathbf{GL}(E)$ sao cho $\pi(gg') = \pi(g)\pi(g')$ với $g, g'$ trong G. Giả sử rằng E có một cơ sở hữu hạn $(e_1, e_2, \ldots, e_n)$ trên K; gọi $(e_1^*, e_2^*, \ldots, e_n^*)$ là cơ sở đối ngẫu; gọi $\rho$ là một đồng cấu của nhóm G vào nhóm $\mathbf{GL}(E)$; khi đó các điều kiện sau là tương đương:
(i) $\rho$ là một biểu diễn tuyến tính giải tích;
(ii) với mọi $x \in E$ và $x' \in E'$, hàm $g \mapsto \langle \rho(g)x, x' \rangle$ trên G là giải tích;
(iii) với mọi i và j, hàm $g \mapsto \langle \rho(g)e_i, e_j^* \rangle$ trên G là giải tích.
Các kéo theo (i) $\Rightarrow$ (ii) $\Rightarrow$ (iii) là rõ ràng. Mặt khác, các hàm $u \mapsto \langle ue_i, e_j^* \rangle$ tạo thành một hệ tọa độ trên $\mathscr{L}(E)$; do đó các hạn chế của chúng lên $\mathbf{GL}(E)$ tạo thành một hệ tọa độ trên $\mathbf{GL}(E)$, do đó có kéo theo (iii) $\Rightarrow$ (i).

Cho G là một nhóm Lie thực, E là một không gian chuẩn hóa đầy đủ thực và $\rho$ là một đồng cấu của nhóm G vào nhóm $\mathbf{GL}(E)$. Ta sẽ thấy trong § 8, Định lý 1 rằng, nếu $\rho$ liên tục (khi $\mathbf{GL}(E)$ có tôpô cảm sinh bởi chuẩn trên $\mathbf{L}(E)$), thì $\rho$ là giải tích. Nhưng chú ý rằng khái niệm liên tục này khác với khái niệm được xét trong Tích phân, Chương VIII, § 2, Định nghĩa 1 (iii) (Bài tập 1).

(4) Cho G là một nhóm Lie thực và E là một không gian chuẩn hóa đầy đủ phức. Một biểu diễn tuyến tính giải tích của G trên E là một cấu xạ từ G vào nhóm Lie thực nền của $\mathbf{GL}(E)$.

#### Mệnh đề 4 {#lie-iii-s1-prop-4 .statement}

Cho G và H là các nhóm Lie và f là một đồng cấu của nhóm G vào nhóm H. Để f là giải tích, điều kiện cần và đủ là tồn tại một tập con mở khác rỗng U của G sao cho $f|_U$ là giải tích.

Điều kiện hiển nhiên là cần. Giả sử điều kiện đó đúng. Với mọi $x_0 \in G$, $f(x_0x) = f(x_0)f(x)$ với mọi $x \in U$ và do đó $f|_{x_0U}$ là giải tích. Nhưng các tập hợp $x_0U$, với $x_0 \in G$, tạo thành một phủ mở của G.

#### Nhận xét {#lie-iii-s1-n2-rem-1 .statement}

Nếu f là một phép nhúng tại e (tương ứng, một phép toàn ánh dưới tại e), thì rõ ràng f là một phép nhúng (tương ứng, một phép toàn ánh dưới).

### 3. CÁC NHÓM CON LIE

Cho G là một nhóm Lie và H là một nhóm con của G đồng thời là một đa tạp con của G. Khi đó ánh xạ $(x, y) \mapsto xy^{-1}$ từ $H \times H$ vào G là giải tích và do đó ánh xạ $(x, y) \mapsto xy^{-1}$ từ $H \times H$ vào H là giải tích. (Các đa tạp khả vi và giải tích, R, 5.8.5). Vì vậy H, với các cấu trúc nhóm và đa tạp cảm sinh bởi các cấu trúc trên G, là một nhóm Lie.

#### Định nghĩa 3 {#lie-iii-s1-def-3 .statement}

Cho G là một nhóm Lie. Một tập con H của G được gọi là một nhóm con Lie nếu H là một nhóm con và là một đa tạp con của G.

Một nhóm con mở của G là một nhóm con Lie của G. Đặc biệt, nếu G là một nhóm Lie thực hoặc phức, thành phần đồng nhất của nó là một nhóm con Lie của G.

#### Mệnh đề 5 {#lie-iii-s1-prop-5 .statement}

Cho G là một nhóm Lie và H là một nhóm con Lie của G.
(i) H là đóng trong G.
(ii) Đơn ánh chính tắc của H vào G là một cấu xạ nhóm Lie.
(iii) Cho L là một nhóm Lie và f là một ánh xạ từ L vào G sao cho f(L) ⊂ H. Để f là một cấu xạ từ L vào H, điều kiện cần và đủ là f là một cấu xạ từ L vào G.

Theo Các đa tạp khả vi và giải tích, R, 5.8.3, H là đóng địa phương. Do đó H là đóng (Tôpô đại cương, Chương III, § 2, Mệnh đề 4). Mệnh đề (ii) là hiển nhiên. Mệnh đề (iii) suy ra từ Các đa tạp khả vi và giải tích, R, 5.8.5.

#### Mệnh đề 6 {#lie-iii-s1-prop-6 .statement}

Cho G là một nhóm Lie và H là một nhóm con của G. Để H là một nhóm con Lie của G, điều kiện cần và đủ là tồn tại một điểm h ∈ H và một lân cận mở U của h trong G sao cho H ∩ U là một đa tạp con của G.

Điều kiện hiển nhiên là cần. Giả sử điều kiện đó đúng. Với mọi h' ∈ H, phép tịnh tiến γ(h'h^{-1}) là một tự đẳng cấu của đa tạp G và biến đa tạp con H ∩ U của U vào đa tạp con (h'h^{-1}H) ∩ (h'h^{-1}U) của h'h^{-1}U. Vì h'h^{-1}H = H và h'h^{-1}U là một lân cận mở của h' trong G, ta thấy rằng mọi điểm của H có một lân cận mở V sao cho V ∩ H là một đa tạp con của G. Do đó H là một đa tạp con của G.

Cho G là một nhóm Lie và H là một nhóm con Lie của G. Nếu L là một nhóm con Lie của H, thì L là một nhóm con Lie của G theo Các đa tạp khả vi và giải tích, R, 5.8.6. Cho M là một nhóm con Lie của G sao cho M ⊂ H. Khi đó M là một nhóm con Lie của H, vì đơn ánh chính tắc của M vào H hiển nhiên là một phép nhúng.

Cho k là một trường con đóng không rời rạc của K. Một nhóm con Lie k của G là một nhóm con Lie của nhóm Lie k nền của G.

#### Nhận xét {#lie-iii-s1-n3-rem-1 .statement}

Nếu thay thế "đa tạp con" bằng "đa tạp con giả" trong Định nghĩa 3, ta thu được định nghĩa của các nhóm con giả Lie của G. (Đối với G hữu hạn chiều, các nhóm con giả Lie chỉ là các nhóm con Lie.) Giả sử rằng K có đặc số 0. Mệnh đề 5 vẫn đúng với cùng chứng minh cho các nhóm con giả Lie. Mệnh đề 6 vẫn đúng với cùng chứng minh, thay thế "nhóm con Lie" bằng "nhóm con giả Lie" và "đa tạp con" bằng "đa tạp con giả".

### 4. CÁC TÍCH NỬA TRỰC TIẾP CỦA CÁC NHÓM LIE

Cho I là một tập hợp hữu hạn và (L_i)_{i \in I} là một họ các nhóm Lie. Các cấu trúc nhóm và đa tạp trên L = \prod_{i \in I} L_i là tương thích và do đó L có một cấu trúc nhóm Lie. L được gọi là nhóm Lie tích của họ các nhóm Lie (L_i)_{i \in I}.

Cho L và M là các nhóm Lie và σ là một đồng cấu từ L vào nhóm tự đẳng cấu của nhóm M. Cho S là tích nửa trực tiếp ngoài của L bởi M tương ứng với σ (Đại số, Chương I, § 6, no. 1, Định nghĩa 2).

#### Mệnh đề 7 {#lie-iii-s1-prop-7 .statement}

*Nếu ánh xạ* $(m, l) \mapsto \sigma(l)m$ *của* $M \times L$ *vào* $M$ *là giải tích, nhóm* $S$, *với cấu trúc đa tạp tích của* $M$ *và* $L$, *là một nhóm Lie*.

Với $l, l'$ trong $L$ và $m, m'$ trong $M$,

$$
(m, l)(m', l')^{-1} = mll'^{-1}m'^{-1} = m(\sigma(ll'^{-1})m'^{-1})ll'^{-1}
= (m(\sigma(ll'^{-1})m'^{-1}), ll'^{-1})
$$

do đó mệnh đề.

Nếu các điều kiện của Mệnh đề 7 được thỏa mãn, nhóm Lie $S$ được gọi là nhóm Lie tích nửa trực tiếp (*ngoài*) của $L$ bởi $M$ tương ứng với $\sigma$.

Rõ ràng đơn ánh chính tắc của $L$ (tương ứng $M$) vào $S$ là một đẳng cấu của $L$ (tương ứng $M$) lên một nhóm con Lie của $S$ mà ta đồng nhất với $L$ (tương ứng $M$). Ánh xạ chính tắc của $S$ lên $L$ là một cấu xạ nhóm Lie.

Ngược lại, cho $G$ là một nhóm Lie và $L$, $M$ là hai nhóm con Lie sao cho nhóm $G$ là tích nửa trực tiếp (đại số) của $L$ bởi $M$ (*Algebra*, Chương I, § 6, no. 1). Ta viết $\sigma(l)m = lml^{-1}$ với $l \in L$ và $m \in M$. Khi đó $\sigma$ thỏa mãn các điều kiện của Mệnh đề 7. Do đó ta có thể tạo thành nhóm Lie tích nửa trực tiếp $S$ của $L$ bởi $M$ ứng với $\sigma$. Ánh xạ $j: (m, l) \mapsto ml$ từ $S$ lên $G$ là một đẳng cấu nhóm và là giải tích. Nếu $j$ là một đẳng cấu nhóm Lie, *nhóm Lie* $G$ *được gọi là* (*nội*) *tích nửa trực tiếp của* $L$ *bởi* $M$ *và* $S$ *và* $G$ *được đồng nhất*. Với mọi $g \in G$, ta viết $g = p(g)q(g)$, trong đó $p(g) \in M$ và $q(g) \in L$. Để nhóm Lie $G$ là tích nửa trực tiếp của $L$ bởi $M$, điều kiện cần và đủ là một trong các ánh xạ $p: G \to M$ và $q: G \to L$ là giải tích, trong trường hợp đó cả hai đều là giải tích; hoặc tương đương, điều kiện cần và đủ là $T_e(G)$ là tổng trực tiếp tôpô của $T_e(M)$ và $T_e(L)$ (vì, nếu điều kiện này được thỏa mãn, $j$ là étale tại $e_S$).

#### Ví dụ {#lie-iii-s1-n4-exa-1 .statement}

Cho $E$ là một không gian chuẩn hóa được, $G = \mathbf{GL}(E)$, $T$ là nhóm chuyển của $E$ và $A$ là nhóm hoán vị của $E$ sinh bởi $G$ và $T$. Nhóm $A$ về mặt đại số là tích nửa trực tiếp của $G$ bởi $T$. (Nếu $E$ là hữu hạn chiều, $A$ là nhóm affine của $E$, xem *Đại số*, Chương II, § 9, no. 4). Gọi $\sigma$ là biểu diễn tuyến tính đồng nhất của $G$ trên $E$ và $S$ là tích nửa trực tiếp ngoài của $G$ bởi $E$ đối với $\sigma$. Với mọi $x \in E$, gọi $t_x$ là phép chuyển của $E$ được xác định bởi $x$. Ánh xạ $(x, u) \mapsto t_x \circ u$ là đẳng cấu $\Phi$ của nhóm $S$ lên nhóm $A$. Ánh xạ $(x, u) \mapsto \sigma(u)x = u(x)$ từ $E \times \mathcal{L}(E)$ vào $E$ là liên tục và song tuyến tính, do đó giải tích; hạn chế của nó trên $E \times G$ vì thế là giải tích. Như vậy nhóm $S$, với cấu trúc đa tạp tích của $E$ và $G$, là một nhóm Lie. Ta chuyển cấu trúc này sang $A$ bằng $\Phi$. Khi đó $A$ trở thành một nhóm Lie, là tích nửa trực tiếp trong của $G$ bởi $T$ như một nhóm Lie.

#### Mệnh đề 8 {#lie-iii-s1-prop-8 .statement}

*Cho* $G$ *và* $H$ *là các nhóm Lie, $p: G \to H$ *và* $s: H \to G$ *là các đồng cấu nhóm Lie sao cho* $p \circ s = \mathrm{id}_H$ *và* $N = \mathrm{Ker}\ p$. *Khi đó* $N$ *là một nhóm con Lie của* $G$, *s là một đẳng cấu của* $H$ *lên một nhóm con Lie của* $G$ *và nhóm Lie* $G$ *là tích nửa trực tiếp trong của* $s(H)$ *bởi* $N$.

$T_e(p) \circ T_e(s) = \mathrm{id}_{T_{e(H)}}$ và do đó $p$ (tương ứng, $s$) là một phép ngập chìm (tương ứng, một phép nhúng). Theo *Đa tạp khả vi và giải tích*, R, 5.10.5, N là một nhóm con Lie của G. Mặt khác, $s$ là một đồng phôi từ H lên $s(H)$ và do đó $s$ là một đẳng cấu từ H lên một nhóm con Lie của G (*Đa tạp khả vi và giải tích*, R, 5.8.3). Cuối cùng, với mọi $g \in G$, $g = (s \circ p)(g) \cdot n$ với một $n \in N$ nào đó; vì $s \circ p$ là giải tích, nhóm Lie G là tích nửa trực tiếp của $s(H)$ bởi N.

### 5. THƯƠNG CỦA MỘT ĐA TẠP THEO MỘT NHÓM LIE

Cho G là một nhóm Lie, X là một đa tạp lớp $C^r$ và $(g, x) \mapsto gx$ là một luật tác động trái (*Đại số*, Chương I, § 5, no. 1) lớp $C^r$ của G trên X. Với mọi $g \in G$, ký hiệu $\tau(g)$ là tự đẳng cấu $x \mapsto gx$ của X do g xác định. Với mọi $x \in X$, ký hiệu $\rho(x)$ là ánh xạ quỹ đạo $g \mapsto gx$ từ G vào X do x xác định. Khi đó

$$
\rho(x) = \rho(gx) \circ \delta(g), \qquad \rho(x) = \tau(g) \circ \rho(x) \circ \gamma(g^{-1})
$$

với mọi $g \in G$ và $x \in X$. Do đó

$$
T_g(\rho(x)) = T_e(\rho(gx)) \circ T_g(\delta(g))
$$
$$
T_g(\rho(x)) = T_x(\tau(g)) \circ T_e(\rho(x)) \circ T_g(\gamma(g^{-1}))
$$

#### Mệnh đề 9 {#lie-iii-s1-prop-9 .statement}

*Cho $x \in X$ và $g_0 \in G$.*

(i) *Nếu $\rho(x)$ là một phép nhúng (tương ứng, một phép ngập chìm, một phép bán nhúng) tại $g_0$, thì, với mọi $g \in G$, $\rho(gx)$ là một phép nhúng (tương ứng, một phép ngập chìm, một phép bán nhúng).*

(ii) *Nếu $\rho(x)$ có hạng k tại $g_0$, thì với mọi $g \in G$, $\rho(gx)$ có hạng không đổi bằng k.*

Điều này suy ra ngay lập tức từ các công thức (4) và (5) vì $T_g(\delta(g)), T_x(\tau(g))$ và $T_g(\gamma(g^{-1}))$ là các đẳng cấu.

#### Hệ quả {#lie-iii-s1-n5-cor-1 .statement}

*Cho $x \in X$. Nếu K có đặc số 0 và X hữu hạn chiều, thì $\rho(x)$ là một phép bán nhúng. Nếu hơn nữa $\rho(x)$ là đơn ánh, thì $\rho(x)$ là một phép nhúng.*

Điều này suy ra từ Mệnh đề 9 và *Đa tạp khả vi và giải tích*, R, 5.10.6.

Chú ý rằng, nếu $\eta$ ký hiệu ánh xạ $(g, x) \mapsto gx$ từ $G \times X$ vào X, thì, với $g \in G, x \in X, u \in T_g(G), v \in T_x(X)$,

$$
T_{(g, x)}(\eta)(u, v) = T_{(g, x)}(\eta)(u, 0) + T_{(g, x)}(\eta)(0, x)
$$

tức là

$$
T_{(g, x)}(\eta)(u, v) = T_g(\rho(x))u + T_x(\tau(g))v.
$$

#### Mệnh đề 10 {#lie-iii-s1-prop-10 .statement}

*Cho G là một nhóm Lie và X là một đa tạp lớp $C^r$ có một luật tác động trái lớp $C^r$ của G trên X. Giả sử rằng:*

(a) *nhóm G tác động một cách đúng và tự do trên X;*

(b) *với mọi $x \in X$, $\rho(x)$ là một phép nhúng (điều này là một hệ quả của (a) nếu K có đặc số 0 và X hữu hạn chiều).*

Khi đó quan hệ tương đương do G xác định trên X là chính quy (Đa tạp khả vi và giải tích, R, 5.9.5). Tồn tại trên tập thương X/G một và chỉ một cấu trúc đa tạp sao cho ánh xạ chính tắc $\pi : X \to X/G$ là một phép ngập chìm. Tôpô nền của cấu trúc đa tạp này là tôpô thương của tôpô trên X; nó là Hausdorff. Cuối cùng, $(X, G, X/G, \pi)$ là một bó sợi trái chính.\footnote{† Các bó sợi chính được định nghĩa trong Đa tạp khả vi và giải tích, R, 6.2.1 là các bó sợi phải chính. Định nghĩa các bó sợi trái chính có thể được suy ra từ đó theo một cách hiển nhiên.}

Cho $\theta$ là ánh xạ $(g, x) \mapsto (x, gx)$ từ $G \times X$ vào $X \times X$. Ánh xạ này thuộc lớp $C^\tau$. Ta sẽ chỉ ra rằng nó là một phép nhúng. Với $u \in T_g(G)$ và $v \in T_x(X)$, theo (6),

$$
T_{(g, x)}(\theta)(u, v) = (v, T_g(\rho(x))u + T_x(\tau(g))v).
$$

Nhưng $T_g(\rho(x))$ là đơn ánh theo giả thiết (b) và do đó $T_{(g, x)}(\theta)$ là đơn ánh. Ảnh của nó là tổng trực tiếp tôpô của không gian con $H_{g, x}$ gồm các vectơ $(v, T_x(\tau(g))v)$ với $v \in T_x(X)$ và không gian con

$$
I_{g, x} = \{0\} \times T_g(\rho(x))(T_g(G)).
$$

Theo giả thiết (b), $T_g(\rho(x))(T_g(G))$ nhận một phần bù tôpô $J_{g, x}$ trong $T_{gx}(X)$. Do đó ảnh của $T_{(g, x)}(\theta)$ nhận phần bù tôpô $\{0\} \times J_{g, x}$. Vậy ta đã chứng minh rằng $\theta$ là một phép ngâm của $G \times X$ vào $X \times X$.

Vì G tác động tự do trên X, $\theta$ là đơn ánh. Gọi C là đồ thị của quan hệ tương đương R do G xác định trên X. Vì G tác động đúng lên X, $\theta$ là một đồng phôi của $G \times X$ lên C (General Topology, Chapter I, § 10, Proposition 2). Theo Differentiable and Analytic Manifolds, R, 5.8.3, nó là một đa tạp con của $X \times X$ và $\theta$ là một đẳng cấu của đa tạp $G \times X$ lên đa tạp C. Không gian tiếp xúc $T_{(x, gx)}(C)$ được đồng nhất với

$$
T_{(g, x)}(\theta)(T_{(g, x)}(G \times X)) = H_{g, x} \oplus I_{g, x} \subset T_{(x, gx)}(X \times X).
$$

Gọi pr$_1$ và pr$_2$ là các phép chiếu chính tắc của $X \times X$ lên hai nhân tử. Ngay lập tức thấy rằng $T_{(x, gx)}(\mathrm{pr}_1)$ ánh xạ $H_{g, x}$ lên $T_x(X)$ và hạt nhân của $T_{(x, gx)}(\mathrm{pr}_1) | T_{(x, gx)}(C)$ là $I_{g, x}$. Vì thế $\mathrm{pr}_1 | C$ là một phép chìm từ C lên X. Theo Differentiable and Analytic Manifolds, R, 5.9.5, R là chính quy. Do đó theo định nghĩa, trên tập thương X/G tồn tại một và chỉ một cấu trúc đa tạp sao cho $\pi$ là một phép chìm. Tôpô nền của X/G là tôpô thương của tôpô của X (Differentiable and Analytic Manifolds, R, 5.9.4). Tôpô này là Hausdorff (General Topology, Chapter III, § 4, Proposition 3).

Với mọi $b \in X/G$, tồn tại một lân cận mở W của b và một cấu xạ $\sigma : W \to X$ sao cho $\pi \circ \sigma = \mathrm{id}_W$ (Differentiable and Analytic Manifolds, R, 5.9.1). Gọi $\phi$ là song ánh $(g, w) \mapsto g\sigma(w)$ từ $G \times W$ lên $\pi^{-1}(W)$. Nó thuộc lớp $C^\tau$. Khi đó $\pi(g\sigma(w)) = w$ và

$$
\theta^{-1}(\sigma(w), g\sigma(w)) = (g, \sigma(w))
$$

và do đó song ánh ngược của $\phi$ thuộc lớp $C^r$. Rõ ràng $\phi(gg', w) = g\phi(g', w)$ với $w \in W,\ g \in G,\ g' \in G$. Vậy $(X, G, X/G, \pi)$ là một phân thớ chính trái.

#### Nhận xét {#lie-iii-s1-n5-rem-1 .statement}

Với các giả thiết trên, giả sử thêm rằng $H$ là một đa tạp lớp $C^r$ và $(x, h) \mapsto m(x, h)$ là một ánh xạ lớp $C^r$ từ $X \times H$ vào $X$ sao cho $m(gx, h) = gm(x, h)$ với $x \in X,\ g \in G,\ h \in H$. Gọi $n$ là ánh xạ từ $(X/G) \times H$ vào $X/G$ dẫn xuất từ $m$ bằng cách lấy thương. Ta chứng minh rằng $n$ *thuộc lớp* $C^r$. Xét biểu đồ

$$
\begin{array}{ccc}
X \times H & \xrightarrow{m} & X \\
\pi \times 1 \downarrow & & \downarrow \pi \\
(X/G) \times H & \xrightarrow{n} & X/G
\end{array}
$$

Biểu đồ này giao hoán, $\pi \circ m$ thuộc lớp $C^r$ và $\pi \times 1$ là một phép nhúng chìm toàn ánh; do đó chỉ cần áp dụng *Differentiable and Analytic Manifolds*, R, 5.9.5.

Cho $G$ là một nhóm Lie, $X$ là một đa tạp lớp $C^r$ và $(g, x) \mapsto xg$ là một luật phép toán phải lớp $C^r$ của $G$ trên $X$. Đặt $\tau(g)x = \rho(x)g = xg$ với $g \in G,\ x \in X$. Khi đó lần này

$$(3')$$
$$
\rho(x) = \rho(xg) \circ \gamma(g^{-1}), \qquad \rho(x) = \tau(g) \circ \rho(x) \circ \delta(g)
$$
và do đó
$$(4')$$
$$
T_g(\rho(x)) = T_e(\rho(xg)) \circ T_g(\gamma(g^{-1}))
$$
$$(5')$$
$$
T_g(\rho(x)) = T_x(\tau(g)) \circ T_e(\rho(x)) \circ T_g(\delta(g)).
$$

Mặt khác, nếu $\eta$ ký hiệu ánh xạ $(g, x) \mapsto xg$ từ $G \times X$ vào $X$, thì công thức (6) vẫn còn đúng. Mệnh đề 9, Hệ quả của nó và Mệnh đề 10 cũng vẫn đúng như vậy (với việc thay "principal left fibre bundle" bằng "principal right fibre bundle" trong mệnh đề cuối).

### 6. CÁC KHÔNG GIAN THUẦN NHẤT VÀ CÁC NHÓM THƯƠNG

#### Mệnh đề 11 {#lie-iii-s1-prop-11 .statement}

*Cho $X$ là một nhóm Lie và $G$ là một nhóm con Lie của $X$.*

(i) *Trên tập hợp thuần nhất $X/G$ có một và chỉ một cấu trúc đa tạp giải tích sao cho phép chiếu chính tắc $\pi$ từ $X$ lên $X/G$ là một phép nhúng chìm. Luật phép toán của $X$ trên $X/G$ là giải tích. Với mọi $x \in X$, hạt nhân của $T_x(\pi)$ được suy ra từ $T_e(G)$ bởi $T_e(\gamma(x))$.*

(ii) *Nếu $G$ là chuẩn tắc trong $X$, thì $X/G$ là một nhóm Lie với cấu trúc nhóm của nó và cấu trúc đa tạp được xác định trong (i). Ánh xạ $\pi$ là một cấu xạ nhóm Lie.*

Theo *General Topology*, Chapter III, § 4, no. 1, *Example 1*, $G$ tác động riêng và tự do trên $X$ bằng phép tịnh tiến phải. Do đó khẳng định thứ nhất của (i) suy ra từ

Mệnh đề 10 của no. 5. Mệnh đề thứ hai suy ra từ Nhận xét của no. 5. Vì $\pi$ là một phép ngập, hạt nhân của $T_x(\pi)$ là không gian tiếp xúc tại $x$ với
$$
\pi^{-1}(\pi(x)) = xG = \gamma(x)(G)
$$
và do đó thu được từ $T_e(G)$ bởi $T_e(\gamma(x))$.

Giả sử rằng $G$ là chuẩn tắc. Gọi $m$ là ánh xạ $(x, y) \mapsto xy^{-1}$ từ $(X/G) \times (X/G)$ vào $X/G$. Khi đó $(m \circ (\pi \times \pi))(x, y) = \pi(xy^{-1})$ với mọi $x, y$ trong $X$. Vậy $m \circ (\pi \times \pi)$ là giải tích. Vì $\pi \times \pi$ là một phép ngập toàn ánh, $m$ là giải tích (Differentiable and Analytic Manifolds, R. 5.9.5), do đó có (ii).

Tập hợp thuần nhất $X/G$ với cấu trúc đa tạp được xác định trong (i) được gọi là không gian thuần nhất Lie thương (trái) của $X$ theo $G$. Không gian thuần nhất Lie (phải) $G \setminus X$ được xác định tương tự. Khi $G$ là chuẩn tắc, nhóm Lie $X/G$ được xác định trong (ii) được gọi là nhóm Lie thương của $X$ theo $G$.

#### Mệnh đề 12 {#lie-iii-s1-prop-12 .statement}

Cho $X$ là một nhóm Lie và $Y$ là một đa tạp giải tích khác rỗng với một luật phép toán trái giải tích của $X$ trên $Y$. Với mọi $y \in Y$, gọi $\varphi(y)$ là ánh xạ quỹ đạo theo $y$ và $X_y$ là nhóm ổn định của $y$ trong $X$. Các điều kiện sau là tương đương:
(i) tồn tại $y \in Y$ sao cho $\varphi(y)$ là một phép ngập toàn ánh;
(i') với mọi $y \in Y$, $\varphi(y)$ là một phép ngập toàn ánh;
(ii) tồn tại $y \in Y$ sao cho $X_y$ là một nhóm con Lie của $X$ và ánh xạ chính tắc từ $X/X_y$ vào $Y$ là một đẳng cấu đa tạp;
(ii') với mọi $y \in Y$, $X_y$ là một nhóm con Lie của $X$ và ánh xạ chính tắc từ $X/X_y$ vào $Y$ là một đẳng cấu đa tạp;
(iii) ánh xạ $(x, y) \mapsto (y, xy)$ từ $X \times Y$ vào $Y \times Y$ là một phép ngập toàn ánh.

Vì ánh xạ chính tắc từ $X$ lên $X/X_y$ là một phép ngập, các tương đương (i) $\Leftrightarrow$ (ii), (i') $\Leftrightarrow$ (ii') là ngay lập tức. (i) $\Leftrightarrow$ (i') theo Mệnh đề 9 của no. 5. Tương đương (i') $\Leftrightarrow$ (iii) suy ra từ công thức (7) của no. 5.

Trong các điều kiện của Mệnh đề 12, $Y$ được gọi là một không gian thuần nhất Lie (trái) của $X$. Các không gian thuần nhất Lie phải của $X$ được định nghĩa tương tự.

#### Ví dụ {#lie-iii-s1-n6-exa-1 .statement}

Cho $G$ là một nhóm Lie. Ta cho $G \times G$ tác động trên $G$ ở bên trái bởi $(g_1, g_2)x = g_1xg_2^{-1}$. Gọi $\rho$ là ánh xạ quỹ đạo của $e$. Khi đó các hạn chế của $T_{(e, e)}(\rho)$ lên $T_{(e, e)}(G \times \{e\}) = T_e(G) \times \{0\}$ và lên
$$
T_{(e, e)}(\{e\} \times G) = \{0\} \times T_e(G)
$$
là các đẳng cấu của các không gian ấy lên $T_e(G)$. Do đó $T_{(e, e)}(\rho)$ là toàn ánh và $\operatorname{Ker} T_{(e, e)}(\rho)$ thừa nhận chẳng hạn phần bù tôpô $T_e(G) \times \{0\}$ trong $T_{(e, e)}(G \times G)$. Vì vậy $\rho$ là một phép chìm tại $(e, e)$. Suy ra $G$ là một không gian thuần nhất Lie trái của $G \times G$.

#### Mệnh đề 13 {#lie-iii-s1-prop-13 .statement}

Cho $G$ là một nhóm Lie, $H$ là một nhóm con Lie chuẩn tắc của $G$, $X$ là một đa tạp lớp $C^r$ và $(g, x) \mapsto gx$ là một luật tác động trái lớp $C^r$ của $G$ trên $X$. Giả sử rằng các điều kiện (a) và (b) của Mệnh đề 10 được thỏa mãn.

(i) Luật tác động trái $(h, x) \mapsto hx$ của $H$ trên $X$ thỏa mãn các điều kiện (a) và (b) của Mệnh đề 10 (do đó ta có thể xét các đa tạp thương $X/G$ và $X/H$).

(ii) Luật tác động trái của $G$ trên $X$ xác định, khi lấy thương, một luật tác động trái lớp $C^r$ của $G/H$ trên $X/H$; luật này thỏa mãn các điều kiện (a) và (b) của Mệnh đề 10 (do đó ta có thể xét đa tạp thương $(X/H)/(G/H)$).

(iii) Ánh xạ chính tắc từ $X$ lên $X/H$ xác định, khi lấy thương, một song ánh từ $X/G$ lên $(X/H)/(G/H)$. Song ánh này là một đẳng cấu của các đa tạp lớp $C^r$.

Rõ ràng $H$ tác động tự do trên $X$; nó tác động đúng theo *Topologie Générale*, Chương III, § 4, no. 1, *Ví dụ* 1. Các ánh xạ quỹ đạo của $H$ trên $X$ là các phép nhúng vì đơn ánh chính tắc của $H$ vào $G$ là một phép nhúng. Điều này chứng minh (i).

Luật tác động trái của $G$ trên $X$ hiển nhiên xác định, khi lấy các thương, một luật tác động trái của $G/H$ trên $X/H$. Luật này thuộc lớp $C^r$ theo *Đa tạp khả vi và giải tích*, R, 5.9.6. Cho $g \in G$ và $x \in X$ sao cho $(Hg)(Hx) = Hx$; khi đó $H(gx) = Hx$ và do đó $gx \in Hx$ và $g \in H$; điều này chứng minh rằng $G/H$ tác động tự do trên $X/H$. Ánh xạ $\theta : (g, x) \mapsto (x, gx)$ từ $G \times X$ vào $X \times X$ là đóng; mặt khác, $\theta(Hg \times Hx) = Hx \times H(gx)$; do đó ngay lập tức suy ra rằng ánh xạ

$$(Hg, Hx) \mapsto (Hx, H(gx))$$

từ $(G/H) \times (X/H)$ vào $(X/H) \times (X/H)$ là đóng; hơn nữa, vì $G/H$ tác động tự do trên $X/H$, Định lý 1 (c) của *Tôpô đại cương*, Chương I, § 10, no. 2 chứng minh rằng $G/H$ tác động đúng trên $X/H$.

Cho $\pi$ là ánh xạ chính tắc của $X$ lên $X/H$, $\sigma$ là ánh xạ chính tắc của $G$ lên $G/H$, $x$ là một phần tử của $X$ và $y = \pi(x)$.

$$
\begin{array}{ccc}
G & \xrightarrow{\rho(x)} & X \\
\downarrow \sigma & & \downarrow \pi \\
G/H & \xrightarrow{\rho(y)} & X/H
\end{array}
$$

Khi đó $\pi \circ \rho(x) = \rho(y) \circ \sigma$ và do đó

$$
T_x(\pi) \circ T_e(\rho(x)) = T_e(\rho(y)) \circ T_e(\sigma).
$$

Cho $u \in T_e(G/H)$ sao cho $T_e(\rho(y))u = 0$. Có $v \in T_e(G)$ sao cho $u = T_e(\sigma)v$. Khi đó $T_x(\pi)(T_e(\rho(x))v) = 0$, do đó $T_e(\rho(x))v$ tiếp xúc với $Hx$ (*Đa tạp khả vi và giải tích*, R, 5.10.5) và vì vậy có dạng $T_e(\rho(x) | H)v'$ với một $v' \in T_e(H)$. Vì $T_e(\rho(x))$ đơn ánh, suy ra $v = v'$, do đó $v \in T_e(H)$ và vì vậy $u = 0$. Vậy $T_e(\rho(y))$ đơn ánh. Ảnh của $T_e(\rho(y))$ bằng ảnh của $T_x(\pi) \circ T_e(\rho(x))$; nay ảnh của $T_e(\rho(x))$ có một phần bù tôpô trong $T_x(X)$ và chứa hạt nhân của $T_x(\pi)$. Do đó thấy rằng $\rho(y)$ là một phép nhúng, điều này hoàn tất chứng minh của (ii).

Mệnh đề (iii) suy ra từ những điều trên và *Đa tạp khả vi và giải tích*, R, 5.9.7.

#### Hệ quả {#lie-iii-s1-n6-cor-1 .statement}

Cho G là một nhóm Lie và H và L là các nhóm con Lie chuẩn tắc của G với L ⊂ H. Khi đó H/L là một nhóm con Lie chuẩn tắc của G/L và song ánh chính tắc của G/H lên (G/L)/(H/L) là một đẳng cấu nhóm Lie.

### 7. QUỸ ĐẠO

#### Mệnh đề 14 {#lie-iii-s1-prop-14 .statement}

Cho G là một nhóm Lie, X là một đa tạp giải tích và (g, x) ↦ gx là một luật tác động trái giải tích của G trên X. Cho x ∈ X. Giả sử ánh xạ quỹ đạo tương ứng ρ(x) là một phép nhúng con (điều này luôn đúng nếu K có đặc số 0 và X hữu hạn chiều (Hệ quả của Mệnh đề 9)). Gọi G_x là nhóm ổn định của x trong G.
(i) G_x là một nhóm con Lie và T_e(G_x) = Ker T_e(ρ(x)).
(ii) Ánh xạ chính tắc i_x của không gian thuần nhất G/G_x vào X là một phép nhúng có ảnh Gx.
(iii) Nếu thêm quỹ đạo Gx đóng địa phương và tôpô trên G có một cơ sở đếm được, thì Gx là một đa tạp con của X, i_x là một đẳng cấu của đa tạp G/G_x lên đa tạp Gx và T_x(Gx) = Im T_e(ρ(x)).

Ảnh ngược của x qua ρ(x) là G_x. Vì ρ(x) là một phép nhúng con, G_x là một đa tạp con và, với mọi g ∈ G, không gian tiếp xúc J với gG_x = ρ_{(x)}^{-1}(gx) tại g là Ker T_g(ρ(x)) (*Đa tạp khả vi và giải tích*, R, 5.10.5), do đó (i). Cho π: G → G/G_x là ánh xạ chính tắc. Khi đó i_x ∘ π = ρ(x). Vì G/G_x là một đa tạp thương của G, đẳng thức này chứng minh rằng i_x là giải tích. Hơn nữa, các hạt nhân của T_g(ρ(x)) và T_g(π) đều bằng J. Do đó T_{π(g)}(i_x) đơn ánh. Ảnh của T_{π(g)}(i_x) bằng ảnh của T_g(ρ(x)) và do đó có một phần bù tôpô. Điều này chứng minh (ii).

Giả sử Gx đóng địa phương. Khi đó mọi điểm của Gx đều có một lân cận trong Gx đồng phôi với một không gian con đóng của một không gian mêtric đầy đủ và do đó là một không gian Baire. Vì vậy Gx là một không gian Baire (*Tôpô đại cương*, Chương IX, § 5, Mệnh đề 4). Nếu G có một cơ sở đếm được, do đó i_x là một phép đồng phôi của G/G_x lên Gx (*Tôpô đại cương*, Chương IX, § 5). Khi đó theo (ii) và *Đa tạp khả vi và giải tích*, R, 5.8.3, i_x là một đẳng cấu của các đa tạp G/G_x lên đa tạp Gx và

$$
T_x(Gx) = \operatorname{Im} T_{π(e)}(i_x) = \operatorname{Im} T_e(ρ(x)).
$$

#### Nhận xét {#lie-iii-s1-n7-rem-1 .statement}

Cho G là một nhóm Lie hữu hạn chiều, X là một đa tạp thuộc lớp C^r và (g, x) ↦ gx là một luật tác động trái thuộc lớp C^r của G trên X. Khi đó Mệnh đề 14 vẫn đúng. Điểm duy nhất cần một chứng minh khác là sự kiện G_x là một nhóm con Lie. Nhưng nếu r ≠ ω, K = \mathbf{R}; vì hiển nhiên G_x là đóng, G_x là một nhóm con Lie theo § 8, Định lý 2.

#### Hệ quả {#lie-iii-s1-n7-cor-1 .statement}

Cho G là một nhóm Lie có tôpô có một cơ sở đếm được và X là một đa tạp giải tích hữu hạn chiều, khác rỗng, với một luật tác động trái giải tích của G trên X. Giả sử G tác động bắc cầu trên X và K có đặc số 0. Khi đó X là một không gian thuần nhất Lie đối với G.

Cho x ∈ X. Quỹ đạo của x, bằng X, là đóng và do đó ta có thể áp dụng Mệnh đề 14 (iii).

### 8. BÓ VECTƠ CÓ TOÁN TỬ

Cho G là một nhóm Lie, X là một đa tạp thuộc lớp C^r và (g, x) ↦ gx là một luật tác động trái thuộc lớp C^r của G trên X. Cho E là một bó vectơ thuộc lớp C^r, có không gian cơ sở X và π : E → X là phép chiếu của E lên X. Với mọi x ∈ X, gọi E_x là thớ của E tại x. Cho (g, u) ↦ gu là một luật tác động trái của G trên E sao cho π tương thích với các phép toán của G trên X và trên E. Với mọi g ∈ G và mọi x ∈ X, hạn chế của ánh xạ u ↦ gu lên E_x là một song ánh ψ_{g, x} của E_x lên E_{gx}. Ta giả sử rằng, với mọi g ∈ G và mọi x ∈ X, ψ_{g, x} liên tục và tuyến tính và do đó là một đẳng cấu của không gian định chuẩn được E_x lên không gian định chuẩn được E_{gx}.

Cho φ là tự đẳng cấu $(g, x) ↦ (g, gx)$ của đa tạp $G × X$. Cho p là phép chiếu chính tắc của $G × X$ lên $X$ và E' là ảnh ngược của E qua p. Cho ψ : E' → E' là ánh xạ là tổng của các ψ_{g, x} : E'_{(g, x)} → E'_{(g, gx)}.

#### Định nghĩa 4 {#lie-iii-s1-def-4 .statement}

Nếu ψ là một φ-cấu xạ của các bó vectơ lớp C^r, thì E được gọi là một bó G-vectơ lớp C^r.

Nói cách khác, E là một bó G-vectơ lớp C^r nếu với mọi $(g_0, x_0) ∈ G × X$ điều kiện sau đây được thỏa mãn: tồn tại một lân cận mở U của $(g_0, x_0)$ trong $G × X$ sao cho, nếu $E' | U$ (tương ứng $E' | φ(U)$) được đồng nhất với một bó vectơ tầm thường có thớ M (tương ứng N) bằng một biểu đồ vectơ, thì ánh xạ $(g, x) ↦ ψ_{g, x}$ của U vào $L(M, N)$ là lớp C^r.

Ánh xạ ψ hiển nhiên là song ánh và suy ra từ tiêu chuẩn địa phương ở trên rằng ψ^{-1} là một $φ^{-1}$-cấu xạ của các bó vectơ, do đó ψ là một $φ$-đẳng cấu của các bó vectơ.

Một bó G-vectơ tầm thường có cơ sở X là một bó vectơ $X × F$ (trong đó F là một không gian chuẩn hóa đầy đủ) với luật phép toán $(g, (x, f)) ↦ (gx, f)$ của G trên $X × F$.

Ta lại giả sử các giả thiết và ký hiệu đứng trước Định nghĩa 4 và lấy thêm τ là một hàm tử vectơ lớp C^r đối với các đẳng cấu (*Differentiable and Analytic Manifolds*, R, 7.6.6). Khi đó τE là một bó vectơ có không gian cơ sở X. Với mọi $x ∈ X$, thớ của nó $(τE)_x$ bằng $τ(E_x)$. Với mọi không gian chuẩn hóa $N_1, N_2$, ký hiệu $Isom(N_1, N_2)$ là tập hợp các đẳng cấu của $N_1$ lên $N_2$. Nếu $g ∈ G$, thì

$$
\tau(\psi_{g, x}) \in \mathrm{Isom}((\tau E)_x, (\tau E)_{gx}).
$$

Các τ(ψ_{g, x}) xác định một luật tác động trái $(g, u) ↦ gu$ của G trên τE và phép chiếu chính tắc của τE lên X tương thích với các phép toán của G trên X và τE.

#### Mệnh đề 15 {#lie-iii-s1-prop-15 .statement}

*Nếu E là một bó G-vectơ lớp C^r, thì τE là một bó G-vectơ lớp C^r*.

Cho $g_0, x_0, U, M, N$ như trong đoạn sau Định nghĩa 4. Khi đó ánh xạ $(g, x) ↦ τ(ψ_{g,x})$ của U vào $\mathcal{L}(\tau M, \tau N)$ là hợp thành của ánh xạ $(g, x) ↦ ψ_{g,x}$ của U vào $\mathcal{L}(M, N)$ và ánh xạ $f ↦ τ(f)$ của $Isom(M, N)$ vào $Isom(τM, τN)$; hai ánh xạ này đều lớp C^r và do đó hợp thành của chúng cũng vậy, do đó có mệnh đề.

#### Mệnh đề 16 {#lie-iii-s1-prop-16 .statement}

*Cho G là một nhóm Lie, X là một đa tạp lớp C^r ($r ≥ 2$) và $(g, x) ↦ gx$ là một luật tác động trái lớp C^r của G trên X, do đó, bằng cách chuyển cấu trúc, tồn tại một luật tác động trái của G trên TX. Với luật này, TX là một bó G-vectơ lớp $C^{r-1}$.*

Cho pr_1 (tương ứng pr_2) là phép chiếu chính tắc của $G × X$ lên G (tương ứng X) và cho E_1 (tương ứng E_2) là ảnh ngược của TG (tương ứng TX) đối với pr_1 (tương ứng pr_2). Khi đó bó vectơ $T(G × X)$ là tổng trực tiếp của E_1 và E_2. Cho $i: E_2 → T(G × X)$ và $q: T(G × X) → E_2$ là các cấu xạ bó vectơ chính tắc được xác định bởi phân tích này thành một tổng trực tiếp. Cho φ là ánh xạ $(g, x) ↦ (g, gx)$ của $G × X$ vào $G × X$. Khi đó ánh xạ được ký hiệu là ψ trong Định nghĩa 4 (trong đó đặt $E = TX$) chính là $q ∘ T(φ) ∘ i$. Nhưng $T(φ)$ là một φ-cấu xạ của các bó vectơ lớp $C^{r-1}$ (*Differentiable and Analytic Manifolds*, R, 8.1.2).

#### Hệ quả {#lie-iii-s1-n8-cor-1 .statement}

*Nếu τ là một hàm tử vectơ lớp C^r đối với các đẳng cấu, thì τ(TX) là một bó G-vectơ lớp $C^{r-1}$.*

Điều này suy ra từ các Mệnh đề 15 và 16.

#### Nhận xét 1 {#lie-iii-s1-n8-rem-1 .statement}

Nếu τ là một hàm tử vectơ lớp C^r đối với các đẳng cấu *trong số chiều hữu hạn* và E có hạng hữu hạn, thì τE được định nghĩa tương tự và Mệnh đề 15 vẫn đúng; Hệ quả của Mệnh đề 16 vẫn đúng với điều kiện X là hữu hạn chiều.

#### Ví dụ {#lie-iii-s1-n8-exa-1 .statement}

Với các giả thiết và ký hiệu của Mệnh đề 16, cho F là một không gian chuẩn hóa đầy đủ. Khi đó $\mathcal{L}((TX)^p; F)$ là một bó G-vectơ lớp $C^{r-1}$; Alt^p(TX; F) cũng vậy nếu K có đặc số không hoặc X là hữu hạn chiều (*Differentiable and Analytic Manifolds*, R, 7.7, 7.8). Nếu X là hữu hạn chiều, $\bigotimes^p (TX) \otimes \bigotimes^q (TX)^*$ là một bó G-vectơ lớp $C^{r-1}$.

#### Mệnh đề 17 {#lie-iii-s1-prop-17 .statement}

*Cho G là một nhóm Lie, X là một không gian thuần nhất Lie trái của G, $x_0$ là một điểm của X, $G_0$ là nhóm ổn định của $x_0$ trong G, E và E' là các bó G-vectơ trái lớp C^r có không gian cơ sở X, E_0 (tương ứng E'_0) là thớ của E (tương ứng E') tại $x_0$ và f là một phần tử của $\mathcal{L}(E_0, E'_0)$ sao cho $f(gu) = gf(u)$ với mọi $u ∈ E_0$ và $g ∈ G_0$. Khi đó tồn tại duy nhất một cấu xạ của E vào E' tương thích với các phép toán của G và mở rộng f.*

Tính duy nhất của cấu xạ này là hiển nhiên. Ta chứng minh sự tồn tại của nó. Cho g, g' là các phần tử của G và $u ∈ E_0$ sao cho $gu = g'u$. Khi đó $g'^{-1}g ∈ G_0$ và $g'^{-1}gu = u$ và do đó $g'^{-1}gf(u) = f(u)$, nghĩa là $gf(u) = g'f(u)$. Do đó một ánh xạ φ được xác định từ E vào E' bằng cách viết $φ(gu) = gf(u)$. Rõ ràng ánh xạ này mở rộng f và nó tương thích với các phép toán của G. Ta chứng minh rằng φ là một cấu xạ bó vectơ lớp C^r. Cho $x_1 ∈ X$. Tồn tại một lân cận mở V của $x_1$ trong X và một đa tạp con W của G sao cho ánh xạ $g ↦ gx_0$ là một đẳng cấu θ lớp C^r của W lên V. Bằng cách thu nhỏ V và W, có thể giả sử rằng:
(1) $E | V$ (tương ứng $E' | V$) được đồng nhất với một bó vectơ tầm thường có thớ M (tương ứng M');
(2) nếu ψ_g (tương ứng ψ'_g) ký hiệu ánh xạ $u ↦ gu$ của E_0 (tương ứng E'_0) vào $E_{gx_0}$ (tương ứng $E'_{gx_0}$), thì các ánh xạ $g ↦ ψ_g$ và $g ↦ ψ_g^{-1}$ (tương ứng $g ↦ ψ'_g$ và $g ↦ ψ'_g^{-1}$) của W vào 𝓛(E_0, M) và 𝓛(M, E_0) (tương ứng 𝓛(E'_0, M') và 𝓛(M', E'_0)) là lớp C^r.

Với x ∈ V, gọi φ_x : M → N là hạn chế của φ lên E_x = M. Khi đó φ_x thu được bằng cách hợp thành các ánh xạ sau:
(1) ánh xạ (ψ_θ^{-1,x})^{-1} từ M vào E_0;
(2) ánh xạ f từ E_0 vào E_0;
(3) ánh xạ ψ'_θ^{-1,x} từ E_0 vào M'.
Do đó ta thấy rằng ánh xạ x ↦ φ_x từ V vào 𝓛(M, M') là lớp C^r.

#### Hệ quả 1 {#lie-iii-s1-prop-17-cor-1 .statement}

Gọi E_0^{G_0} là tập hợp các phần tử của E_0 bất biến dưới G_0. Với mọi u ∈ E_0^{G_0}, gọi σ_u là ánh xạ từ X vào E được xác định bởi σ_u(gx_0) = gu với mọi g ∈ G.
(i) Các tiết diện† bất biến dưới G của E là lớp C^r.
(ii) u ↦ σ_u là một song ánh từ E_0^{G_0} lên tập hợp các tiết diện bất biến dưới G của E.

Mệnh đề (ii) là hiển nhiên. Để chứng minh (i), chỉ cần chứng minh rằng mỗi tiết diện σ_u là lớp C^r. Gọi E' là G-bó tầm thường có cơ sở X và sợi E_0^{G_0}. Gọi f là đơn ánh chính tắc của E_0^{G_0} vào E_0. Theo Mệnh đề 17, tồn tại một cấu xạ φ từ E' vào E tương thích với các phép toán của G và mở rộng f. Nếu u ∈ E_0^{G_0} và g ∈ G, thì

$$
σ_u(gx_0) = gu = gf(u) = φ(gu) = φ((u, gx_0))
$$

và do đó σ_u(x) = φ((u, x)) với mọi x ∈ X, điều này chứng minh mệnh đề của ta.

*Ví dụ, gọi G là một nhóm Lie thực hữu hạn chiều, G_0 là một nhóm con Lie compact của G và X là không gian thuần nhất G/G_0. Ký hiệu x_0 là ảnh chính tắc của e trong X. Tồn tại một dạng song tuyến tính đối xứng xác định dương trên T_{x_0}(X) bất biến dưới G_0 (Integration, Chương VII, § 3, Mệnh đề 1). Áp dụng điều trên cho (TX)* ⊗ (TX)*, ta thấy rằng tồn tại trên X một metric Riemann giải tích bất biến dưới G_*.

† Ở đây, bởi một tiết diện của E ta hiểu là một ánh xạ σ (không nhất thiết là lớp C^r) từ X vào E sao cho p ∘ σ = Id_X, trong đó p ký hiệu phép chiếu của E lên X.

#### Hệ quả 2 {#lie-iii-s1-prop-17-cor-2 .statement}

Giả sử rằng $G_0$ tác dụng tầm thường trên $E_0$. Gọi $E'$ là $G$-bó tầm thường có không gian cơ sở $X$ và sợi $E_0$. Tồn tại một và chỉ một đẳng cấu từ $E$ lên $E'$ tương thích với các phép toán của $G$ và mở rộng $\mathrm{Id}_{E_0}$.

Điều này suy ra ngay lập tức từ Mệnh đề 17.

#### Nhận xét 2 {#lie-iii-s1-n8-rem-2 .statement}

Trong số này, các luật phép toán trái có thể được thay thế ở khắp nơi bằng các luật phép toán phải.

### 9. ĐỊNH NGHĨA ĐỊA PHƯƠNG CỦA MỘT NHÓM LIE

#### Mệnh đề 18 {#lie-iii-s1-prop-18 .statement}

Gọi $G$ là một nhóm và $U$ và $V$ là hai tập con của $G$ chứa $e$. Giả sử rằng $U$ có một cấu trúc đa tạp giải tích thỏa mãn các điều kiện sau:
(i) $V = V^{-1}, V^2 \subset U, V$ mở trong $U$;
(ii) ánh xạ $(x, y) \mapsto xy^{-1}$ từ $V \times V$ vào $U$ là giải tích;
(iii) với mọi $g \in G$, tồn tại một lân cận mở $V'$ của $e$ trong $V$ sao cho $gV'g^{-1} \subset U$ và sao cho ánh xạ $x \mapsto gxg^{-1}$ từ $V'$ vào $U$ là giải tích.

Khi đó tồn tại một và chỉ một cấu trúc đa tạp giải tích trên $G$ có các tính chất sau:
(α) $G$ với cấu trúc này là một nhóm Lie;
(β) $V$ mở trong $G$;
(γ) các cấu trúc đa tạp trên $G$ và $U$ cảm sinh cùng một cấu trúc trên $V$.

(a) Gọi $A$ là một tập con mở của $V$ và $v_0$ là một phần tử của $V$ sao cho $v_0A \subset V$. Khi đó $v_0A$ là tập hợp các $v \in V$ sao cho $v_0^{-1}v \in A$ và do đó là một tập con mở của $V$ (có tính đến (ii)). Hơn nữa, (ii) kéo theo rằng các ánh xạ $v \mapsto v_0v$ từ $A$ lên $v_0A$ và $v \mapsto v_0^{-1}v$ từ $v_0A$ lên $A$ là các song ánh giải tích nghịch đảo nhau và do đó là các đẳng cấu giải tích.

(b) Ta chọn một lân cận mở $W$ của $e$ trong $V$ sao cho $W = W^{-1}$, $W^3 \subset V$ và tồn tại một bản đồ $(W, \phi, E)$ của đa tạp $U$ với miền xác định $W$. Với mọi $g \in G$, đặt $\phi_g$ là ánh xạ $h \mapsto \phi(g^{-1}h)$ của $gW$ vào $E$. Ta chứng minh rằng các bản đồ $\phi_g$ của $G$ tương thích giải tích. Cho $g_1, g_2$ là các phần tử của $G$ sao cho $g_1W \cap g_2W \neq \emptyset$, khi đó $g_2^{-1}g_1$ và $g_1^{-1}g_2$ thuộc $W^2$. Theo (a), $W \cap g_1^{-1}g_2W$ là một tập con mở của $W$ và do đó
$$
\phi_{g_1}(g_1W \cap g_2W) = \phi(W \cap g_1^{-1}g_2W)
$$
là một tập con mở $D$ của $E$. Với $d \in D$,
$$
(\phi_{g_2} \circ \phi_{g_1}^{-1})(d) = \phi(g_2^{-1}g_1\phi^{-1}(d));
$$
theo (a), ta thấy rằng $\phi_{g_2} \circ \phi_{g_1}^{-1}$ là giải tích.

(c) Theo (b), trên $G$ tồn tại một cấu trúc đa tạp giải tích sao cho $(\phi_g)_{g \in G}$ là một atlas trên $G$. Với mọi $g_0 \in G$, ánh xạ $g \mapsto g_0g$ ($g \in G$) giữ bất biến atlas này và do đó là một tự đẳng cấu của $G$ với cấu trúc đa tạp này. Đặc biệt, điều kiện (GL₁) được thỏa mãn.

(d) Cho $v_0 \in V$. Theo (ii), tồn tại một lân cận mở $A$ của $e$ trong $W$ sao cho $v_0A \subset V$. Trước hết, điều này chứng minh rằng $V$ là mở trong $G$. Theo (a), ánh xạ $v \mapsto v_0v$ của $A$ lên $v_0A$ là một đẳng cấu giải tích với các cấu trúc cảm sinh bởi $U$. Theo (c), ta thấy rằng các cấu trúc đa tạp trên G và U cảm sinh cùng một cấu trúc trên $v_0A$ và do đó cuối cùng trên $V$.

(e) Theo (d), (ii) và (iii), ta thấy rằng các điều kiện (GL_2) và (GL_3) được thỏa mãn. Do đó G là một nhóm Lie.

(f) Nếu một cấu trúc đa tạp trên G tương thích với cấu trúc nhóm của G và sao cho V là một đa tạp con mở của G, thì $(\phi_g)_{g\in G}$ là một atlas trên G. Do đó, mệnh đề về tính duy nhất của mệnh đề.

#### Mệnh đề 19 {#lie-iii-s1-prop-19 .statement}

Cho G là một nhóm tôpô, H một nhóm Lie và f một đồng cấu của nhóm G vào nhóm H. Giả sử tồn tại một lân cận mở của e_G trong G, một bản đồ (V, \phi, E) của đa tạp H tại e_H và một không gian con vectơ đóng F của E có một phần bù tôpô, sao cho f(U) \subset V và \phi \circ f)|U là một phép đồng phôi của U lên $\phi(V) \cap F$. Khi đó tồn tại duy nhất một cấu trúc đa tạp trên G sao cho f là một phép nhúng; cấu trúc này là ảnh ngược theo f của cấu trúc đa tạp trên H. Với cấu trúc này G là một nhóm Lie.

Vì các phép tịnh tiến của G (tương ứng H) là các phép đồng phôi (tương ứng các đẳng cấu giải tích), f thỏa mãn điều kiện (R) của Differentiable and Analytic Manifolds, R, 5.8.1. Hai mệnh đề đầu tiên của mệnh đề khi đó suy ra từ Differentiable and Analytic Manifolds, R, loc. cit. Xét biểu đồ giao hoán

$$
\begin{array}{ccc}
G \times G & \xrightarrow{m} & G \\
f \times f \downarrow & & \downarrow f \\
H \times H & \xrightarrow{n} & H
\end{array}
$$

trong đó m(x, y) = xy^{-1} (tương ứng n(x, y) = xy^{-1}) với x, y trong G (tương ứng H). Khi đó n \circ (f \times f) là giải tích, do đó f \circ m là giải tích và do đó m là giải tích vì f là một phép nhúng. Vậy G là một nhóm Lie.

Cấu trúc nhóm Lie trên G được gọi là ảnh ngược của cấu trúc nhóm Lie trên H theo f.

#### Hệ quả {#lie-iii-s1-n9-cor-1 .statement}

Cho G là một nhóm tôpô, N một nhóm con chuẩn tắc rời rạc của G và \pi là ánh xạ chính tắc của G lên G/N. Giả sử một cấu trúc đa tạp giải tích được cho trên G/N, tương thích với cấu trúc nhóm tôpô trên G/N. Khi đó tồn tại duy nhất một cấu trúc đa tạp trên G sao cho \pi là một phép nhúng; cấu trúc này là ảnh ngược theo \pi của cấu trúc đa tạp trên G/N. Với cấu trúc này, \pi là étale, G là một nhóm Lie và G/N là nhóm Lie thương của G bởi N.

#### Nhận xét {#lie-iii-s1-n9-rem-1 .statement}

Cho H là một nhóm Lie thực hoặc phức liên thông, $\tilde{H}$ là phủ phổ quát của nó† và \pi là ánh xạ chính tắc của $\tilde{H}$ lên H. Khi nói về $\tilde{H}$

† Cf. General Topology, Chapter XI; trong khi chờ xuất bản chương này, xem chẳng hạn L. S. Pontrjagin, Topological groups, 2nd edition translated from Russian, Gordon and Breach, 1966; hoặc G. Hochschild, The structure of Lie groups, Holden-Day, 1965.

CÁC NHÓM LIE

với tư cách là một nhóm Lie, ta luôn luôn có nghĩa là với cấu trúc ảnh ngược của cấu trúc trên H theo $\pi$.

### 10. CÁC MẦM NHÓM

#### Định nghĩa 5 {#lie-iii-s1-def-5 .statement}

**Một mầm nhóm Lie trên K** là một hệ $(G, e, \theta, m)$ thỏa mãn các điều kiện sau:
(i) $G$ là một đa tạp giải tích trên $K$;
(ii) $e \in G$;
(iii) $\theta$ là một ánh xạ giải tích từ $G$ vào $G$;
(iv) $m$ là một ánh xạ giải tích từ một tập con mở $\Omega$ của $G \times G$ vào $G$;
(v) với mọi $g \in G$, $(e, g) \in \Omega$, $(g, e) \in \Omega$, $m(e, g) = m(g, e) = g$;
(vi) với mọi $g \in G$, $(g, \theta(g)) \in \Omega$, $(\theta(g), g) \in \Omega$, $m(g, \theta(g)) = m(\theta(g), g) = e$;
(vii) nếu $g, h, k$ là các phần tử của $G$ sao cho $(g, h) \in \Omega$, $(h, k) \in \Omega$, $(m(g, h), k) \in \Omega$, $(g, m(h, k)) \in \Omega$, thì $m(m(g, h), k) = m(g, m(h, k))$.

$e$ được gọi là phần tử đơn vị của mầm nhóm. Ta thường viết $gh$ thay cho $m(g, h)$ và (do lạm dụng ký hiệu) $g^{-1}$ thay cho $\theta(g)$.

Một nhóm Lie $G$ là một mầm nhóm Lie với lựa chọn hiển nhiên của $e, \theta, m$.

Cho $G$ là một mầm nhóm Lie. Khi đó $ee^{-1} = e$, tức là

$$
e^{-1} = e.
$$

Với mọi $g \in G$,

$$
g = eg = ((g^{-1})^{-1}g^{-1})g = (g^{-1})^{-1}(g^{-1}g) = (g^{-1})^{-1}e,
$$

tức là

$$
(g^{-1})^{-1} = g.
$$

Một tập con của $G$ bất biến dưới ánh xạ $g \mapsto g^{-1}$ được gọi là đối xứng.

Đa tạp $G$, với điểm $e$, ánh xạ $g \mapsto g^{-1}$ và ánh xạ $(g, h) \mapsto hg$ là một mầm nhóm Lie $G^\vee$ được gọi là mầm nhóm Lie đối của $G$.

Mầm nhóm Lie $G$ được gọi là giao hoán nếu, với mọi $(g, h) \in G \times G$ sao cho $gh$ được xác định, $hg$ được xác định và bằng $gh$.

Cho $G$ là một mầm nhóm Lie. Tập hợp các $(g, h) \in G \times G$ sao cho $gh$ được xác định là một lân cận của $(e, e)$. Mặt khác, các ánh xạ $(g, h) \mapsto gh$ và $g \mapsto g^{-1}$ là liên tục. Do đó $(gh)k = g(hk)$ với $g, h, k$ đủ gần $e$. Tương tự, $(h^{-1}g^{-1})(gh) = h^{-1}(eh) = h^{-1}h = e$ với $g, h$ đủ gần $e$, do đó nhân bên phải với $(gh)^{-1}$,

$$
(gh)^{-1} = h^{-1}g^{-1} \quad \text{với } g, h \text{ đủ gần với } e.
$$

#### Mệnh đề 20 {#lie-iii-s1-prop-20 .statement}

*Cho $G$ là một mầm nhóm Lie và $g \in G$. Tồn tại một lân cận mở $U$ của $e$ và một lân cận mở $V$ của $g$ với các tính chất sau:*
(a) $ug$ được xác định với mọi $u \in U$;
(b) $vg^{-1}$ được xác định với mọi $v \in V$;
(c) các ánh xạ $u \mapsto ug,\ v \mapsto vg^{-1}$ là các đẳng cấu giải tích nghịch đảo của nhau từ $U$ lên $V$ và từ $V$ lên $U$.

§ 1.10

Vì tập hợp xác định của tích là mở trong $G \times G$, tồn tại một lân cận mở $U$ của $e$ và một lân cận mở $V$ của $g$ với các tính chất (a) và (b). Đặt $\eta(u) = ug$ với $u \in U$, $\eta'(v) = vg^{-1}$ với $v \in V$. Bằng cách thu nhỏ $U$ và $V$, có thể giả sử rằng $(ug)g^{-1} = u$ và $(vg^{-1})g = v$ với $u \in U$ và $v \in V$. Khi đó $\eta$ và $\eta'$ là các đơn ánh. Bằng cách thu nhỏ $U$ thêm nữa, có thể giả sử rằng $\eta(U) \subset V$. Khi đó $\eta'(V) \supset U$ và $\eta(U)$ là ảnh ngược của $U$ qua $\eta'$ và do đó là một lân cận mở của $g$ trong $V$. Thay thế $V$ bởi $\eta(U)$, cuối cùng ta đạt tới tình huống trong đó $\eta$ và $\eta'$ là các song ánh nghịch đảo giải tích.

Cho $G_1, G_2$ là hai mầm nhóm Lie với các phần tử đơn vị $e_1, e_2$. Một ánh xạ $f$ của $G_1$ vào $G_2$ được gọi là một *cấu xạ* nếu $f$ thỏa mãn các điều kiện sau:
(i) $f$ là giải tích;
(ii) $f(e_1) = e_2$;
(iii) nếu $g, h$ là các phần tử của $G_1$ sao cho $gh$ được xác định, thì $f(g)f(h)$ được xác định và bằng $f(gh)$.

Cho $g \in G_1$. Vì $gg^{-1}$ được xác định và bằng $e_1$, $f(g)f(g^{-1})$ được xác định và bằng $e_2$ và do đó
$$
f(g)^{-1} = f(g)^{-1}(f(g)f(g^{-1})) = (f(g)^{-1}f(g))f(g^{-1})
$$
tức là
$$
f(g)^{-1} = f(g^{-1}).
$$
(11)

Hợp thành của hai cấu xạ là một cấu xạ.

Nếu $f : G_1 \to G_2$ và $f' : G_2 \to G_1$ là hai cấu xạ nghịch đảo của nhau, thì chúng là các đẳng cấu (sử dụng đặc biệt công thức (11)).

Cho $G_1, G_2$ là hai mầm nhóm Lie, và $f$ là một ánh xạ của $G_1$ vào $G_2$ thỏa mãn các điều kiện (ii) và (iii) ở trên, là giải tích trong một lân cận mở của $e_1$. Sử dụng Mệnh đề 20, có thể chứng minh như trong Mệnh đề 4 rằng $f$ là một cấu xạ.

Cho $(G, e, \theta, m)$ là một mầm nhóm Lie và $\Omega$ là tập xác định của $m$. Cho $H$ là một đa tạp con của $G$ chứa $e$, ổn định dưới $\theta$. Giả sử rằng tập hợp $\Omega_1$ của $(x, y) \in \Omega \cap (H \times H)$ sao cho $m(x, y) \in H$ là mở trong $H \times H$. Khi đó $(H, e, \theta|H, m|\Omega_1)$ là một mầm nhóm Lie. Một mầm nhóm Lie như vậy được gọi là một *mầm nhóm con Lie của G*. Đơn ánh chính tắc của $H$ vào $G$ là một cấu xạ. Nếu $f : L \to G$ là một cấu xạ của các mầm nhóm Lie sao cho $f(L) \subset H$, thì $f : L \to H$ là một cấu xạ của các mầm nhóm Lie.

Giả sử rằng $K$ có đặc số 0. Nếu ta thay thế giả thiết rằng $H$ là một đa tạp con của $G$ bằng giả thiết rằng $H$ là một đa tạp con gần của $G$, các kết quả của đoạn trên vẫn đúng (xem *Differentiable and Analytic Manifolds*, R, 5.8.5). Khi đó $H$ được gọi là một mầm nhóm con Lie gần của $G$.

Nếu $G$ là một mầm nhóm Lie với phần tử đơn vị $e$, mọi lân cận mở đối xứng của $e$ trong $G$ đều là một mầm nhóm con Lie của $G$. (Điều này đặc biệt áp dụng khi $G$ là một nhóm Lie.) Cho $H$ là một mầm nhóm con Lie của $G$; nếu $H$ là một lân cận của $e$ trong $G$, thì $H$ là mở trong $G$ theo Mệnh đề 20.

Mầm nhóm Lie *tích* của một số hữu hạn các mầm nhóm Lie được định nghĩa theo một cách hiển nhiên.

#### Mệnh đề 21 {#lie-iii-s1-prop-21 .statement}

*Cho $G, H$ là hai mầm nhóm Lie và $\phi$ là một cấu xạ từ $G$ vào $H$. Các điều kiện sau là tương đương:*

(i) $\phi$ étale tại $e$;
(ii) *tồn tại các mầm nhóm con Lie mở* $G', H'$ *của* $G, H$ *sao cho* $\phi|G'$ *là một đẳng cấu của* $G'$ *lên* $H'$.

Suy ra (ii) $\Rightarrow$ (i) là hiển nhiên. Giả sử rằng $\phi$ étale tại $e$. Tồn tại một mầm nhóm con Lie mở $G_1$ của $G$ sao cho $\phi(G_1)$ là mở trong $H$ và $\phi|G_1$ là một đẳng cấu của đa tạp $G_1$ lên đa tạp $\phi(G_1)$. Khi đó tồn tại một mầm nhóm con Lie mở $G'$ của $G_1$ sao cho tích trong $G$ của hai phần tử của $G'$ luôn được xác định và thuộc về $G_1$. Nếu $g, g'$ là các phần tử của $G'$ sao cho $gg' \in G'$, thì $\phi(g)\phi(g') = \phi(gg') \in \phi(G')$; nếu $g, g'$ là các phần tử của $G'$ sao cho $gg' \in G_1 - G'$, thì

$$
\phi(g)\phi(g') = \phi(gg') \in \phi(G_1) - \phi(G').
$$

Do đó $\phi|G'$ là một đẳng cấu của mầm nhóm Lie $G'$ lên mầm nhóm con Lie mở $\phi(G')$ của $H$.

Nếu các điều kiện của Mệnh đề 21 được thỏa mãn, $G$ và $H$ được gọi là *đẳng cấu địa phương*.

#### Mệnh đề 22 {#lie-iii-s1-prop-22 .statement}

*Cho $H$ là một nhóm Lie, $U$ là một mầm nhóm con Lie của $H$ và $N$ là tập hợp các $g \in H$ sao cho $U$ và $gUg^{-1}$ có cùng mầm tại $e$ (Tôpô đại cương, Chương I, § 6, no. 10). Khi đó $N$ là một nhóm con của $H$ chứa $U$. Tồn tại một và chỉ một cấu trúc đa tạp giải tích trên $N$ có các tính chất sau:*

(i) $N$ với cấu trúc này là một nhóm Lie;
(ii) $U$ là một đa tạp con mở của $N$;
(iii) *đơn ánh chính tắc của* $N$ *vào* $H$ *là một phép nhúng*.

Rõ ràng $N$ là một nhóm con của $H$. Nếu $g \in U$, thì $ge \in U$ và $geg^{-1} \in U$, do đó $gu \in U$ và $gug^{-1} \in U$ với $u$ đủ gần $e$ trong $U$ và do đó mầm của $gUg^{-1}$ tại $e$ được chứa trong mầm của $U$; đổi $g$ và $g^{-1}$, ta thấy rằng các mầm của $gUg^{-1}$ và $U$ tại $e$ bằng nhau. Do đó $U \subset N$.

Cho $V$ là một lân cận mở của $e$ trong $U$ sao cho $V = V^{-1}, V^2 \subset U$. Các điều kiện (i), (ii), (iii) của Mệnh đề 18 của no. 9 (trong đó $G$ được thay bởi $N$) được thỏa mãn. Do đó tồn tại một cấu trúc đa tạp giải tích trên $N$ với các tính chất sau: ($\alpha$) $N$ với cấu trúc này là một nhóm Lie; ($\beta$) $V$ là mở trong $N$; ($\gamma$) các cấu trúc đa tạp trên $N$ và $U$ cảm sinh cùng một cấu trúc trên $V$. Vì $V$ là một đa tạp con của $H$, đơn ánh chính tắc của $N$ vào $H$ là một phép nhúng tại $e$ và do đó tại mọi điểm của $N$. Cho $u \in U$. Tồn tại một lân cận mở V' của e trong V sao cho ánh xạ $v \mapsto uv$ là một đẳng cấu giải tích từ V' lên một lân cận mở của u trong U (Mệnh đề 20) và đồng thời lên một lân cận mở của u trong N. Do đó U là mở trong N và ánh xạ đồng nhất của U là một đẳng cấu với cấu trúc đa tạp đã cho trên U và cấu trúc đa tạp con mở trên N; nói cách khác, U là một đa tạp con mở của N.

Cuối cùng, ta xét một cấu trúc đa tạp giải tích trên N có các tính chất (i) và (ii) của mệnh đề và gọi N* là nhóm Lie thu được như vậy. Khi đó ánh xạ đồng nhất của N vào N* là étale tại e và do đó là một đẳng cấu nhóm Lie. Điều này chứng minh mệnh đề về tính duy nhất của mệnh đề.

Cho H là một nhóm Lie, U là một mầm nhóm con giả Lie của H và N là tập hợp các $g \in H$ sao cho U và $gUg^{-1}$ có cùng mầm tại e. Nếu K có đặc số 0, tồn tại trên G duy nhất một cấu trúc đa tạp với các tính chất (i) và (ii) của Mệnh đề 22. Chứng minh cũng giống như đối với Mệnh đề 22.

#### Hệ quả {#lie-iii-s1-n10-cor-1 .statement}

Giữ nguyên ký hiệu của Mệnh đề 22, cho G là nhóm con của H sinh bởi U. Khi đó G là một nhóm con mở của N. Tồn tại duy nhất một cấu trúc nhóm Lie trên G sao cho U là một đa tạp con mở của G và đơn ánh chính tắc của G vào H là một phép nhúng chìm.

#### Nhận xét {#lie-iii-s1-n10-rem-1 .statement}

Giữ nguyên ký hiệu của Mệnh đề 22 và hệ quả của nó, giả sử rằng K có đặc số 0, rằng H là hữu hạn chiều và rằng tôpô trên U có một cơ sở đếm được. Ngay cả với tất cả các giả thiết này, có thể xảy ra rằng G không đóng trong H (Bài tập 3). Nhưng, nếu G đóng, thì G là một nhóm con Lie của H. Vì ánh xạ $(g, h) \mapsto gh$ là một luật của phép toán trái giải tích của G trên H. Quỹ đạo của e là G. Mệnh đề của chúng ta khi đó suy ra từ các Mệnh đề 2 (iv) và 14 (iii).

### 11. CÁC MẢNH LUẬT CỦA PHÉP TOÁN

Cho $(G, e, \theta, m)$ là một mầm nhóm Lie và X là một đa tạp thuộc lớp $C^r$.

#### Định nghĩa 6 {#lie-iii-s1-def-6 .statement}

Một mảnh luật của phép toán trái thuộc lớp $C^r$ của G trên X là một ánh xạ $\psi$ xác định trên một tập con mở $\Omega$ của $G \times X$ chứa $\{e\} \times X$, có giá trị trong X và có các tính chất sau:
(i) $\psi$ thuộc lớp $C^r$;
(ii) với mọi $x \in X$, $\psi(e, x) = x$;
(iii) tồn tại một lân cận $\Omega_1$ của $\{e\} \times \{e\} \times X$ trong $G \times G \times X$ sao cho, với $(g, g', x) \in \Omega_1$, các phần tử của $m(g, g')$, $\psi(m(g, g'), x)$, $\psi(g, \psi(g', x))$ được xác định và $\psi(g, \psi(g', x)) = \psi(m(g, g'), x)$.

Các mảnh luật của phép toán phải thuộc lớp $C^r$ được định nghĩa tương tự.
Ta thường viết $gx$ thay cho $\psi(g, x)$.
Cho G' là một mầm nhóm con Lie của G và X' là một đa tạp con của X. Giả sử rằng tập hợp $\Omega'$ của $(g, x) \in \Omega \cap (G' \times X')$ sao cho $\psi(g, x) \in X'$ là mở trong $G' \times X'$ (một điều kiện luôn được thỏa mãn nếu $X'$ là mở trong $X$). Khi đó $\psi|_{\Omega'}$ là một mảnh luật của phép toán trái thuộc lớp $C^r$ của $G'$ trên $X'$, được gọi là dẫn xuất từ $\psi$ bằng hạn chế vào $G'$ và $X'$.

#### Mệnh đề 23 {#lie-iii-s1-prop-23 .statement}

*Cho $(G, e, \theta, m)$ là một mầm nhóm Lie, $X$ là một đa tạp lớp $C^r$, $x_0$ là một điểm của $X$, $\Omega$ là một lân cận mở của $(e, x_0)$ trong $G \times X$ và $\psi$ là một ánh xạ từ $\Omega$ vào $X$ có các tính chất sau:
(i) $\psi$ thuộc lớp $C^r$;
(ii) $\psi(e, x)$ bằng $x$ với $x$ đủ gần $x_0$;
(iii) $\psi(m(g, g'), x) = \psi(g, \psi(g', x))$ với $(g, g', x)$ đủ gần $(e, e, x_0)$.
Khi đó tồn tại một lân cận mở $X'$ của $x_0$ trong $X$ và một tập con mở $\Omega'$ của $\Omega \cap (G \times X')$ sao cho $\psi|_{\Omega'}$ là một mảnh luật của phép toán trái lớp $C^r$ của $G$ trên $X'$.
Tồn tại một lân cận mở $X'$ của $x_0$ trong $X$ và một lân cận mở $G'$ của $e$ trong $G$ sao cho $\psi(e, x) = x$ với mọi $x \in X$, và
$$
\psi(g, \psi(g', x)) = \psi(m(g, g'), x)
$$
với $(g, g', x) \in G' \times G' \times X'$. Gọi $\Omega'$ là tập hợp các $(g, x) \in \Omega \cap (G' \times X')$ sao cho $\psi(g, x) \in X'$. Khi đó $\Omega'$ là mở trong $G \times X'$ và $X'$, $\Omega'$ có các tính chất của mệnh đề.*

#### Bổ đề 3 {#lie-iii-s1-lem-3 .statement}

*Cho $X$ là một không gian chuẩn tắc và $(X_i)_{i \in I}$ là một phủ mở hữu hạn địa phương của $X$. Với mọi $(i, j) \in I \times I$ và mọi $x \in X_i \cap X_j$, gọi $V_{ij}(x)$ là một lân cận của $x$ được chứa trong $X_i \cap X_j$. Khi đó ta có thể gắn với mỗi $x \in X$ một lân cận $V(x)$ của $x$ sao cho các điều kiện sau được thỏa mãn:
(a) quan hệ $x \in X_i \cap X_j$ kéo theo $V(x) \subset V_{ij}(x)$;
(b) nếu $V(x)$ và $V(y)$ giao nhau, tồn tại $i \in I$ sao cho $V(x) \cup V(y) \subset X_i$.
Tồn tại một phủ mở $(X'_i)_{i \in I}$ của $X$ sao cho $\overline{X'_i} \subset X_i$ với mọi $i \in I$ (Tôpô đại cương, Chương IX, § 4, Định lý 3). Cho $x \in X$. Gọi $V_1(x)$ là giao của các $V_{ij}(x)$ và các $X'_k$ chứa $x$; đây là một lân cận mở của $x$. Gọi $V_2(x)$ là một lân cận của $x$ được chứa trong $V_1(x)$ và chỉ giao với một số hữu hạn các $X_i$. Khi đó $V_2(x)$ chỉ giao với một số hữu hạn các $\overline{X'_i}$ và do đó tập
$$
V(x) = V_2(x) \cap \bigcap_{i \in I, x \notin \overline{X'_i}} (X - \overline{X'_i})
$$
là một lân cận của $x$. Nếu $x \in X_i \cap X_j$, thì $V_1(x) \subset X_i \cap X_j$ và do đó $V(x) \subset X_i \cap X_j$. Cho $x, y$ thuộc $X$ và giả sử rằng $V(x)$ và $V(y)$ giao nhau. Tồn tại $i \in I$ sao cho $x \in X'_i$. Khi đó $V_1(x) \subset X'_i$, do đó $V(x) \subset X'_i$ và do đó $V(y) \cap \overline{X'_i} \neq \emptyset$. Khi đó $y \in \overline{X'_i}$ theo định nghĩa của $V(y)$, do đó $y \in X_i$ và $V(y) \subset X_i$. Vậy $X_i$ chứa $V(x)$ và $V(y)$.*

§ 2.1

#### Mệnh đề 24 {#lie-iii-s1-prop-24 .statement}

Cho G là một mầm nhóm Lie, X là một đa tạp lớp C^r và (X_i)_{i \in I} là một phủ mở hữu hạn địa phương của X. Với mọi i \in I, gọi $\psi_i$ là một mảnh luật của phép toán trái lớp C^r của G trên X_i. Giả sử rằng không gian tôpô nền của X là chuẩn tắc và rằng, với mọi (i, j) \in I \times I và mọi x \in X_i \cap X_j, $\psi_i$ và $\psi_j$ trùng nhau trên một lân cận của (e, x). Tồn tại một mảnh luật $\psi$ của phép toán trái lớp C^r của G trên X sao cho, với mọi i \in I và mọi x \in X_i, $\psi_i$ và $\psi$ trùng nhau trên một lân cận của (e, x).

Đối với mọi $(i, j) \in I \times I$ và mọi $x \in X_i \cap X_j$, chọn một lân cận mở $V_{ij}(x)$ của $x$ trong $X_i \cap X_j$ sao cho $\psi_i$ và $\psi_j$ được định nghĩa và bằng nhau trên một lân cận của {e} \times V_{ij}(x) trong G \times X. Đối với mọi $x \in X$ chọn một lân cận mở $V(x)$ của $x$ trong X sao cho các điều kiện (a) và (b) của Bổ đề 3 được thỏa mãn. Gọi $I_x$ là tập hợp các $i \in I$ sao cho $x \in X_i$. Đây là một tập hữu hạn. Gọi $U_x$ là tập hợp các $(g, y) \in G \times V(x)$ sao cho các $\psi_i$ với $i \in I_x$ được định nghĩa và trùng nhau trên một lân cận của $(g, y)$. Khi đó $U_x$ là mở và $(e, x) \in U_x$. Các $\psi_i$ với $i \in I_x$ đều có cùng một hạn chế lên $U_x$. Gọi $x, y$ là các phần tử của X. Nếu $U_x$ và $U_y$ giao nhau, thì $V(x)$ và $V(y)$ giao nhau và do đó tồn tại $i \in I$ sao cho

$$
V(x) \cup V(y) \subset X_i.
$$

Khi đó $i \in I_x$, $i \in I_y$, $\psi_i|U_x = \psi_x, \psi_i|U_y = \psi_y$ và do đó

$$
\psi_x|(U_x \cap U_y) = \psi_y|(U_x \cap U_y).
$$

Các $\psi_x$ do đó định nghĩa một ánh xạ $\psi$ của $U = \bigcup_{x \in X} U_x$ vào X và U là một lân cận mở của {e} \times X trong G \times X. Rõ ràng $\psi$ thuộc lớp C^r và $\psi(e, x) = x$ với mọi $x \in X$. Với mọi $i \in I$ và mọi $x \in X_i$, $\psi$ trùng với $\psi_x$ và do đó với $\psi_i$ trên một lân cận của $(e, x)$ và do đó $\psi$ thỏa mãn điều kiện (iii) của Định nghĩa 6.

### Bài tập {#lie-iii-s1-exercises}

Xem các [bài tập cho § 1](exercises/s1/).
