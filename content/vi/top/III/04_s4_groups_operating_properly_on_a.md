---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 4
section_title: Groups operating properly on a topological space; compact ness in topological groups and spaces with operators
lang: vi
source: top-i-iv
pdf_pages: 0256-0267, 0314-0320
extraction: ocr
subsections:
    - "no": 1
      title: GROUPS OPERATING PROPERLY ON A TOPOLOGICAL SPACE
      page: 0
      pdf_page: 256
    - "no": 2
      title: PROPERTIES OF GROUPS ACTING PROPERLY
      page: 0
      pdf_page: 259
    - "no": 3
      title: GROUPS OPERATING FREELY ON A TOPOLOGICAL SPACE
      page: 0
      pdf_page: 260
    - "no": 4
      title: LOCALLY COMPACT GROUPS OPERATING PROPERLY
      page: 0
      pdf_page: 261
    - "no": 5
      title: GROUPS OPERATING CONTINUOUSLY ON A LOCALLY COMPACT SPACE
      page: 0
      pdf_page: 263
    - "no": 6
      title: LOCALLY COMPACT HOMOGENEOUS SPACES
      page: 0
      pdf_page: 265
statements: 33
exercises: 23
content_sha256: 6c2ab4005e4f2c740902b5093e40fbfb1ec90ccad489b06a72c549f7ac42fb6c
translated_from: content/en/top/III/04_s4_groups_operating_properly_on_a.md
source_content_sha256: 3ca46d1a9c871ef504c2f339d9da2414e8fff5747912bc9df5ba1469bda2f343
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4
translation_run: translate-vi-819ebfcb
glossary_version: 34
glossary_terms_sha256: aaf4f4eb312360051d7adc5147664d4bc4accae695ee933a0a5067d3e91cfdb2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. CÁC NHÓM TÁC ĐỘNG MỘT CÁCH THỰC SỰ LÊN MỘT KHÔNG GIAN TÔPÔ; TÍNH COMPACT TRONG CÁC NHÓM TÔPÔ VÀ CÁC KHÔNG GIAN CÓ TOÁN TỬ

### 1. CÁC NHÓM TÁC ĐỘNG MỘT CÁCH THỰC SỰ LÊN MỘT KHÔNG GIAN TÔPÔ

#### Định nghĩa 1 {#top-iii-s4-def-1 .statement}

Cho $G$ là một nhóm tôpô tác động liên tục trên một không gian tôpô $X$. Ta nói $G$ tác động một cách thực sự trên $X$ nếu ánh xạ

$$
\theta : (s, x) \to (x, s.x) \text{ của } G \times X \text{ vào } X \times X
$$

là thực sự (Chương I, § 10, no. 1, Định nghĩa 1).

Cho $\Gamma \subset G \times X \times X$ là đồ thị của ánh xạ $\rho : (s, x) \to s.x$. Vì $\rho$ liên tục, ánh xạ $\sigma : (s, x) \to (s, x, s.x)$ là một đồng phôi của $G \times X$ lên $\Gamma$, và ánh xạ hợp thành

$$
G \times X \xrightarrow{\sigma} \Gamma \xrightarrow{\mathrm{pr}_{23}} X \times X
$$

chính là $\theta$. Do đó, Định nghĩa 1 tương đương với việc nói rằng hạn chế của $\mathrm{pr}_{23}$ lên $\Gamma$ là một ánh xạ thực sự của $\Gamma$ vào $X \times X$.

Định lý 1 của Chương I, § 10, no. 2 cho thấy rằng G tác động một cách thực sự trên X khi và chỉ khi điều kiện sau được thỏa mãn:
Với mỗi tập hợp A được lọc bởi một siêu lọc $\mathfrak{F}$, và mỗi ánh xạ
$$
\alpha \to (s_\alpha, x_\alpha)
$$
của A vào $G \times X$, nếu ánh xạ $\alpha \to (s_\alpha \cdot x_\alpha, x_\alpha)$ có giới hạn $(b, a)$ theo $\mathfrak{F}$, thì $\alpha \to s_\alpha$ có giới hạn $t \in G$ theo $\mathfrak{F}$, sao cho $t.a = b$.

#### Ví dụ 1 {#top-iii-s4-n1-exa-1 .statement}

Cho H là một nhóm con đóng của một nhóm tôpô G. Nếu G tác động một cách thực sự trên X, thì H cũng vậy, vì $H \times X$ đóng trong $G \times X$ (Chương I, § 10, no. 1, Mệnh đề 5, Hệ quả 1). Chẳng hạn, nếu lấy $X = G$, với G tác động lên chính nó bằng các phép tịnh tiến trái, thì ánh xạ $G \times X \to X \times X$ là một đồng phôi, do đó là thực sự; vậy H tác động một cách thực sự trên G bằng các phép tịnh tiến trái.

#### Ví dụ 2 {#top-iii-s4-n1-exa-2 .statement}

Nếu G tác động một cách thực sự trên X, thì nó tác động một cách thực sự trên mọi không gian con $X'$ của X là hợp của các quỹ đạo của các điểm của X (nói cách khác, $X'$ là bão hòa đối với quan hệ tương đương được xác định bởi G). Vì ảnh ngược của $X' \times X'$ trong $G \times X$ là $G \times X'$, và ta có thể áp dụng Mệnh đề 3 của Chương I, § 10, no. 1.

#### Mệnh đề 1 {#top-iii-s4-prop-1 .statement}

Cho G là một nhóm tôpô tác động liên tục trên một không gian tôpô X, và cho K là một tập con quasi-compact của G. Khi đó ánh xạ $\rho : (s, x) \to s.x$ của $K \times X$ vào X là thực sự.

$\rho$ phân tích thành $K \times X \to K \times X \xrightarrow{\mathrm{pr}_2} X$, trong đó $\alpha(s, x) = (s, s.x)$. $\alpha$ là một đồng phôi, vì $\alpha^{-1} : (s, y) \to (s, s^{-1}.y)$ liên tục. Vì K quasi-compact, $\mathrm{pr}_2$ là thực sự (Chương I, § 10, no. 2, Định lý 1, Hệ quả 5); do đó $\rho$ là thực sự (Chương I, § 10, no. 1, Mệnh đề 5).

#### Hệ quả 1 {#top-iii-s4-prop-1-cor-1 .statement}

Nếu A là một tập con đóng (resp. compact) của X, thì K.A đóng trong X (resp. compact nếu X Hausdorff).

Mệnh đề về các tập đóng suy ra từ Mệnh đề 1 và sự kiện rằng một ánh xạ thực sự là đóng (Chương I, § 10, no. 1, Mệnh đề 1). Mệnh đề về các tập compact là tầm thường.

Cần lưu ý rằng nếu L là một tập con compact của X, và F là một tập con đóng của G, thì F.L không nhất thiết đóng trong X ($§ 2$, Bài tập 29; cf. no. 5, Hệ quả của Mệnh đề 12).

#### Hệ quả 2 {#top-iii-s4-prop-1-cor-2 .statement}

Nếu K là một nhóm con quasi-compact của một nhóm tôpô G, thì quan hệ tương đương $x^{-1}y \in K$ là đóng, và ánh xạ chính tắc $\varphi : G \to G/K$ là thực sự.

#### Hệ quả 3 {#top-iii-s4-prop-1-cor-3 .statement}

Cho K là một nhóm con chuẩn tắc quasi-compact của một nhóm tôpô G, và cho φ là ánh xạ chính tắc G → G/K. Khi đó, với mỗi nhóm con đóng A của G, song ánh chính tắc của A/A ∩ K lên φ(A) là một đẳng cấu của các nhóm tôpô.

Vì x⁻¹y ∈ K là một quan hệ tương đương đóng (Hệ quả 2), Hệ quả này suy ra từ Chương I, § 5, no. 2, Mệnh đề 4.

#### Mệnh đề 2 {#top-iii-s4-prop-2 .statement}

Cho K là một nhóm compact tác động liên tục trên một không gian Hausdorff X. Khi đó:

a) K tác động một cách thực sự trên X.
b) Ánh xạ (s, x) → s.x của K × X vào X là thực sự.
c) Ánh xạ chính tắc của X lên X/K là thực sự.

b) là một hệ quả của Mệnh đề 1. Còn đối với a), vì K compact, pr₂ : (s, x) → x là thực sự (Chương I, § 10, no. 2, Định lý 1, Hệ quả 5); do đó, vì X là Hausdorff, (s, x) → (x, s.x) là thực sự (Chương I, § 10, no. 1, Mệnh đề 5, Hệ quả 3). Còn phải chứng minh c). Theo Hệ quả 1 của Mệnh đề 1, ánh xạ chính tắc φ : X → X/K là đóng. Nếu Z là một không gian tôpô bất kỳ và ta cho K tác động tầm thường trên Z, thì K tác động liên tục trên X × Z và do đó ánh xạ chính tắc X × Z → (X × Z)/K là đóng. Nhưng (X × Z)/K có thể được đồng nhất một cách chính tắc với (X/K) × Z (§ 2, no. 4, Bổ đề 2 và Chương I, § 5, no. 3, Hệ quả của Mệnh đề 8); do đó ánh xạ chính tắc X × Z → (X × Z)/K có thể được đồng nhất với φ × 1, và vì nó là đóng với mọi Z, suy ra rằng φ là thực sự.

#### Hệ quả 1 {#top-iii-s4-prop-2-cor-1 .statement}

Theo các giả thiết của Mệnh đề 2, X compact (resp. địa phương compact) khi và chỉ khi X/K compact (resp. địa phương compact).

Điều này suy ra từ sự kiện rằng ánh xạ chính tắc X → X/K là thực sự, theo Mệnh đề 9 của Chương I, § 10, no. 4.

#### Hệ quả 2 {#top-iii-s4-prop-2-cor-2 .statement}

Cho G là một nhóm tôpô Hausdorff và K là một nhóm con compact của G. Khi đó G compact (resp. địa phương compact) khi và chỉ khi G/K compact (resp. địa phương compact).

Áp dụng Hệ quả 1 cho K tác động trên G bằng các phép tịnh tiến phải.

### 2. CÁC TÍNH CHẤT CỦA CÁC NHÓM TÁC ĐỘNG MỘT CÁCH THỰC SỰ

#### Mệnh đề 3 {#top-iii-s4-prop-3 .statement}

*Nếu một nhóm tôpô* $G$ *tác động thực sự trên một không gian tôpô* $X$, *thì không gian quỹ đạo* $X/G$ *là Hausdorff*. *Nếu thêm* $G$ *là Hausdorff*, *thì* $X$ *là Hausdorff*.

Cho $C \subset X \times X$ là đồ thị của quan hệ tương đương $R$ xác định bởi $G$ trên $X$; khi đó $C$ là ảnh của $G \times X$ qua ánh xạ $\theta : (s, x) \to (x, s.x)$. Vì $\theta$ là thực sự, $C$ là đóng trong $X \times X$ (chương I, § 10, no. 1, Mệnh đề 1). Vì quan hệ $R$ là mở ($§ 2$, no. 4, Bổ đề 2), do đó $X/G$ là Hausdorff (chương I, § 8, no. 3, Mệnh đề 8).

Bây giờ giả sử rằng $G$ là Hausdorff. Khi đó ánh xạ $x \to (e, x)$ của $X$ vào $G \times X$ là một đẳng cấu tôpô của $X$ lên một không gian con đóng của $G \times X$, và do đó là thực sự (chương I, § 10, no. 1, Mệnh đề 2). Nếu ta hợp thành ánh xạ này với ánh xạ $(s, x) \to (x, s.x)$ của $G \times X$ vào $X \times X$, vốn là thực sự theo giả thiết, ta được một ánh xạ thực sự của $X$ vào $X \times X$, cụ thể là ánh xạ đường chéo $x \to (x, x)$. Do đó đường chéo $\Delta$ của $X \times X$ là đóng trong $X$, và vì vậy $X$ là Hausdorff.

#### Mệnh đề 4 {#top-iii-s4-prop-4 .statement}

*Cho* $G$ *là một nhóm tôpô tác động thực sự trên một không gian tôpô* $X$, *và cho* $x$ *là một điểm của* $X$. *Ký hiệu* $G.x$ *là quỹ đạo của* $x$, *và ký hiệu* $K_x$ *là nhóm ổn định của* $x$. *Khi đó*:

a) *Ánh xạ* $s \to s.x$ *của* $G$ *vào* $X$ *là thực sự*.

b) $K_x$ *là gần compact*.

c) *Ánh xạ chính tắc của* $G/K_x$ *lên* $G.x$ *là một đẳng cấu tôpô*.

d) *Quỹ đạo* $G.x$ *là đóng trong* $X$.

Ảnh ngược của $\{ x \} \times X$ qua $\theta : (s, x) \to (x, s.x)$ là $G \times \{ x \}$; do đó, theo Mệnh đề 3 của chương I, § 10, no. 1, hạn chế của $\theta$ trên $G \times \{ x \}$ là một ánh xạ thực sự của $G \times \{ x \}$ vào $\{ x \} \times X$, do đó a) suy ra. Vì $K_x$ là ảnh ngược của $x$ qua $s \to s.x$, b) suy ra từ chương I, § 10, no. 2, Định lý 1. c) và d) là các hệ quả của a), theo chương I, § 10, no. 1, các Mệnh đề 2 và 5 b).

#### Nhận xét {#top-iii-s4-n2-rem-1 .statement}

Mệnh đề 4 cho thấy rằng nếu một nhóm tôpô $G$ tác động thực sự trên một không gian thuần nhất $G/H$, thì nhóm con $H$ là giả compact (và do đó compact nếu $G$ là Hausdorff). Có thể chứng minh rằng đây cũng là một điều kiện đủ để $G$ tác động thực sự trên $G/H$ (Bài tập 3).

#### Mệnh đề 5 {#top-iii-s4-prop-5 .statement}

*Cho* $G$ *(tương ứng.* $G'$) *là một nhóm tôpô tác động liên tục trên một không gian tôpô* $X$ *(tương ứng.* $X'$). *Cho* $\varphi$ *là một đồng cấu liên tục* từ $G$ vào $G'$ và $\psi$ là một ánh xạ liên tục từ $X$ vào $X'$ tương thích với $\varphi$ (§ 2, no. 4). Khi đó:

(i) *Nếu $\varphi$ là toàn ánh và $\psi$ là toàn ánh và thực sự, và nếu $G$ tác động thực sự trên $X$, thì $G'$ tác động thực sự trên $X'$.*

(ii) *Nếu $\varphi$ là thực sự, nếu $G'$ tác động thực sự trên $X'$ và nếu $X$ là Hausdorff, thì $G$ tác động thực sự trên $X$.*

Để chứng minh (i), xét biểu đồ giao hoán

$$
\begin{array}{ccc}
G \times X & \xrightarrow{\theta} & X \times X \\
\alpha \downarrow & & \downarrow \beta \\
G' \times X' & \xrightarrow{\theta'} & X' \times X'
\end{array}
$$

trong đó $\alpha = \varphi \times \psi$ và $\beta = \psi \times \psi$. Theo giả thiết, $\theta$ là thực sự; $\beta$ cũng vậy [Chương I, § 10, no. 1, Mệnh đề 4 a)]; do đó $\beta \circ \theta = \theta' \circ \alpha$ là thực sự [Chương I, § 10, no. 1, Mệnh đề 5 a)]. Vì $\alpha$ là toàn ánh nên suy ra $\theta'$ là thực sự [Chương I, § 10, no. 1, Mệnh đề 5 b)].

Để chứng minh (ii), xét một siêu bộ lọc $U$ trên $G \times X$, sao cho các ánh xạ

$$
(s, x) \to s.x \quad \text{và} \quad (s, x) \to x
$$

hội tụ theo $U$ lần lượt đến $y_0$ và $x_0$. Suy ra rằng $(s, x) \to \varphi(s).\psi(x)$ và $(s, x) \to \psi(x)$ hội tụ theo $U$. Vì $G'$ tác động thực sự trên $X'$, điều này suy ra (no. 1) rằng $(s, x) \to \varphi(s)$ hội tụ theo $U$ đến một điểm $s'_0 \in G'$. Vì $\varphi$ là thực sự, ta suy ra (Chương I, § 10, no. 2, Định lý 1) rằng $(s, x) \to s$ hội tụ theo $U$ đến một điểm $s_0 \in G$. Tính duy nhất của giới hạn trong $X$ khi đó cho thấy rằng $y_0 = s_0 x_0$, và do đó $G$ tác động thực sự trên $X$ (no. 1).

### 3. CÁC NHÓM TÁC ĐỘNG TỰ DO TRÊN MỘT KHÔNG GIAN TÔPÔ

#### Định nghĩa 2 {#top-iii-s4-def-2 .statement}

*Cho $G$ là một nhóm tác động trên một tập hợp $X$. Ta nói $G$ tác động tự do trên $X$ nếu nhóm ổn định của mọi phần tử của $X$ là $\{e\}$, nói cách khác nếu các quan hệ $s.x = x,\ s \in G,\ x \in X$ kéo theo $s = e$.*

#### Ví dụ {#top-iii-s4-n3-exa-1 .statement}

Cho $G$ là một nhóm và $H$ là một nhóm con của $G$. Khi đó $H$ tác động tự do lên $G$ bởi các phép tịnh tiến (trái hoặc phải).

Cho $G$ là một nhóm tác động tự do trên một tập hợp $X$, cho $R$ là quan hệ tương đương do $G$ xác định trên $X$, và cho $C \subset X \times X$ là đồ thị của $R$. Nếu $(x, y) \in C$, thì tồn tại $s \in G$ sao cho $s.x = y$; và $s$ là *duy nhất*, vì $s.x = s'.x$ kéo theo ${s'}^{-1}s.x = x$, và do đó ${s'}^{-1}s = e$ (vì $G$ tác động tự do). Nếu cho tương ứng với $(x, y) \in C$ phần tử duy nhất $s \in G$ sao cho $s.x = y$, ta định nghĩa một ánh xạ $\varphi : C \to G$, mà ta sẽ gọi là ánh xạ chính tắc của $C$ vào $G$. Với ký hiệu này:

#### Mệnh đề 6 {#top-iii-s4-prop-6 .statement}

*Cho $G$ là một nhóm tôpô tác động liên tục trên một không gian tôpô $X$, và giả sử rằng $G$ tác động tự do trên $X$. Khi đó $G$ tác động đúng trên $X$ khi và chỉ khi điều kiện sau đây được thỏa mãn:*

(FP) *Đồ thị $C$ của quan hệ tương đương do $G$ xác định là đóng trong $X \times X$, và ánh xạ chính tắc $\varphi : C \to G$ là liên tục.*

Tập hợp $C$ là ảnh của ánh xạ $\theta : (s, x) \to (x, s.x)$ từ $G \times X$ vào $X \times X$. Ta biết (Chương I, § 10, no. 1, Mệnh đề 2) rằng $\theta$ là đúng khi và chỉ khi $C$ là đóng trong $X \times X$ và (nếu $\theta'$ ký hiệu ánh xạ $\theta$ được xét như một ánh xạ từ $G \times X$ vào $C$) $\theta'$ là một đồng phôi. Bây giờ giả thiết kéo theo rằng $\theta'$ là song ánh và ánh xạ nghịch đảo của nó là ánh xạ $(x, y) \to (\varphi(x, y), x)$. Vậy $\theta'$ là một đồng phôi khi và chỉ khi $\varphi$ liên tục.

### 4. CÁC NHÓM ĐỊA PHƯƠNG COMPACT TÁC ĐỘNG ĐÚNG

#### Mệnh đề 7 {#top-iii-s4-prop-7 .statement}

*Cho $G$ là một nhóm địa phương compact tác động liên tục trên một không gian Hausdorff $X$. Khi đó $G$ tác động riêng trên $X$ khi và chỉ khi, với mỗi cặp điểm $x, y$ của $X$, tồn tại một lân cận $V_x$ của $x$ và một lân cận $V_y$ của $y$ sao cho tập $K$ gồm mọi $s \in G$ mà với chúng $s.V_x \cap V_y \neq \emptyset$ là tương đối compact trong $G$.*

Cho $F$ là không gian compact thu được bằng cách thêm vào $G$ một điểm ở vô cùng $\omega$, và cho $\Gamma$ là đồ thị của $\rho : (s, x) \to s.x$ được xét như một tập con của $F \times X \times X$. Ta hãy chỉ ra rằng nếu hạn chế của $\mathrm{pr}_{23}$ lên $\Gamma$ là thực sự, thì $\Gamma$ là *đóng trong* $F \times X \times X$. Thật vậy, giả thiết này kéo theo rằng ánh xạ $u : (t, s, x, y) \to (t, x, y)$ từ $F \times \Gamma$ vào $F \times X \times X$ là đóng. Nếu $\Gamma'$ là tập các điểm $(s, s)$ trong $F \times G$, với $s \in G$, thì $\Gamma'$ đóng trong $F \times G$, vì nó là đồ thị của đơn ánh chính tắc $G \to F$ (Chương I, § 8, no. 1, Hệ quả 2 của Mệnh đề 2); do đó giao $(\Gamma' \times X \times X) \cap (F \times \Gamma)$ đóng trong $F \times \Gamma$, và thấy ngay rằng ảnh của nó dưới $u$ là tập $\Gamma$ được xét như một tập con của $F \times X \times X$; vậy $\Gamma$ đóng trong $F \times X \times X$. Bây giờ, ta có $(\{\omega\} \times X \times X) \cap \Gamma = \emptyset$. Do định nghĩa của $F$, vì thế, với mọi điểm $(x, y) \in X \times X$ tồn tại một lân cận $W$ của $(x, y)$ trong $X \times X$ và một tập con compact $K$ của $G$ sao cho

$$
((G - K) \times W) \cap \Gamma;
$$

là rỗng; và vì ta có thể lấy $W$ là một lân cận $V_x \times V_y$, trong đó $V_x$ và $V_y$ lần lượt là các lân cận của $x$ và $y$ trong $X$, mệnh đề “((G — K) × W) ∩ Γ = ∅” trở thành “nếu s ∉ K, thì s · V_x ∩ V_y = ∅”. Như vậy ta đã chứng minh tính cần thiết của điều kiện được phát biểu trong mệnh đề. Ngược lại, giả sử điều kiện này được thỏa mãn; cho A là một tập hợp được lọc bởi một ultrafilter 𝔾, và cho α → (s_α, x_α) là một ánh xạ từ A vào G × X sao cho lim_𝔖 x_α = x và lim_𝔖 s_α · x_α = y. Giả sử rằng K, V_x và V_y thỏa mãn điều kiện của mệnh đề. Theo giả thiết có một tập M ∈ 𝔾 sao cho nếu α ∈ M thì x_α ∈ V_x và s_α · x_α ∈ V_y, do đó s_α ∈ K. Điều này chứng tỏ rằng α → s_α hội tụ đối với 𝔾, và chứng minh hoàn tất.

Nếu G là compact, điều kiện của Mệnh đề 7 được thỏa mãn một cách tầm thường; do đó ta thu lại Mệnh đề 2 a).

Đặc biệt, Mệnh đề 7 chỉ ra rằng một nhóm rời rạc G, tác động liên tục trên một không gian Hausdorff X, tác động riêng trên X khi và chỉ khi, với mỗi cặp (x, y) điểm của X, tồn tại một lân cận V_x của x và một lân cận V_y của y sao cho tập các điểm s ∈ G mà với chúng s · V_x ∩ V_y ≠ ∅ là hữu hạn.

#### Mệnh đề 8 {#top-iii-s4-prop-8 .statement}

Cho G là một nhóm rời rạc tác động riêng trên một không gian Hausdorff X. Cho x là một điểm của X và cho K_x là nhóm ổn định của x. Khi đó:

a) Nhóm con K_x là hữu hạn và tồn tại một tập mở U ⊂ X, chứa x, ổn định dưới K_x, và trên đó quan hệ tương đương cảm sinh bởi quan hệ do G xác định là quan hệ tương đương do K_x xác định.

b) Ánh xạ chính tắc U/K_x → X/G là một đồng phôi từ U/K_x lên một lân cận mở của lớp của x trong X/G.

Theo Mệnh đề 7, K_x là hữu hạn. Để xây dựng một tập mở U thỏa mãn các điều kiện đòi hỏi, trước hết nhận thấy rằng theo Mệnh đề 7 tồn tại một tập mở U_0 chứa x và sao cho tập K các s ∈ G mà với chúng s · U_0 ∩ U_0 ≠ ∅ là hữu hạn. Rõ ràng K_x ⊂ K; cho s_1, ..., s_n là các phần tử của K — K_x. Nếu đặt x_i = s_i · x (1 ≤ i ≤ n), thì x_i ≠ x với mọi i; vì X là Hausdorff, với mỗi chỉ số i tồn tại một lân cận mở V_i của x và một lân cận mở V'_i của s_i · x sao cho V_i ∩ V'_i = ∅. Đặt U_i = V_i ∩ s_i^{-1} · V'_i; khi đó U_i rõ ràng là mở và chứa x, và ta có U_i ∩ s_i · U_i ⊂ V_i ∩ V'_i = ∅. Cho U' = U_0 ∩ U_1 ∩ ... ∩ U_n; U' là mở, chứa x và sao cho U' ∩ s · U' = ∅ nếu s ∉ K_x. Đặt U = ⋂_{t ∈ K_x} t · U' thì cuối cùng ta thu được một tập mở, ổn định dưới K_x, chứa x và sao cho U ∩ s · U = ∅ nếu s ∉ K_x: U là tập mở phải tìm.

Việc ánh xạ chính tắc U/K_x → X/G là một đồng phôi từ U/K_x lên một tập mở trong X/G suy ra từ Chương I, § 5, no. 2, Mệnh đề 4, vì U là mở và quan hệ tương đương do G xác định là mở (§ 2, no. 4, Bổ đề 2).

#### Hệ quả {#top-iii-s4-n4-cor-1 .statement}

*Nếu giả sử thêm rằng $K_x = \{ e \}$, thì điểm $x$ có một lân cận mở $U$ sao cho hạn chế lên $U$ của ánh xạ chính tắc $X \to X/G$ là một đồng phôi của $U$ lên một tập con mở của $X/G$.*

### 5. CÁC NHÓM TÁC ĐỘNG LIÊN TỤC TRÊN MỘT KHÔNG GIAN ĐỊA PHƯƠNG COMPACT

#### Mệnh đề 9 {#top-iii-s4-prop-9 .statement}

*Cho $G$ là một nhóm tôpô tác động liên tục trên một không gian địa phương compact $X$. Khi đó nếu $X/G$ là Hausdorff thì nó địa phương compact.*

Vì quan hệ tương đương trên $X$ do $G$ xác định là mở ($§ 2$, no. 4, Bổ đề 2), mệnh đề suy ra từ Chương I, $§ 10$, no. 4, Mệnh đề 10.

#### Mệnh đề 10 {#top-iii-s4-prop-10 .statement}

*Cho $G$ là một nhóm tôpô tác động liên tục trên một không gian địa phương compact $X$, và giả sử rằng $X/G$ là Hausdorff. Gọi $\varphi$ là ánh xạ chính tắc từ $X$ lên $X/G$. Khi đó nếu $K'$ là một tập con compact bất kỳ của $X/G$, thì tồn tại một tập con compact $K$ của $X$ sao cho $\varphi(K) = K'$.*

Vì quan hệ tương đương do $G$ xác định là mở ($§ 2$, no. 4, Bổ đề 2), mệnh đề là một trường hợp riêng của Mệnh đề 10 của Chương I, $§ 10$, no. 4.

#### Mệnh đề 11 {#top-iii-s4-prop-11 .statement}

*Cho $G$ là một nhóm tôpô Hausdorff tác động riêng trên một không gian không rỗng $X$. Nếu $X$ compact (resp. địa phương compact) thì $G$ và $X/G$ cũng vậy.*

Theo giả thiết, ánh xạ $\theta : (s, x) \to (x, s.x)$ từ $G \times X$ vào $X \times X$ là riêng; nếu $X \times X$ compact (resp. địa phương compact) thì Hệ quả của Mệnh đề 9 của Chương I, $§ 10$, no. 4 cho thấy rằng $G \times X$ cũng compact (resp. địa phương compact), và do đó $G$ cũng vậy vì $X \neq \emptyset$. Vì $X/G$ là Hausdorff (no. 2, Mệnh đề 3), tính compact (resp. tính địa phương compact) của $X$ kéo theo tính compact (resp. tính địa phương compact) của $X/G$ [Chương I, $§ 10$, no. 4, Mệnh đề 8 (resp. Mệnh đề 9)] (xem $§ 2$, Bài tập 29).

Bây giờ chúng ta sẽ đưa ra các tiêu chuẩn cho phép khẳng định rằng một nhóm tôpô Hausdorff $G$ tác động riêng trên một không gian địa phương compact $X$. Với mỗi cặp tập con $K, L$ của $X$ ta ký hiệu bởi $P(K, L)$ tập hợp mọi $s \in G$ sao cho $s.K \cap L \neq \emptyset$.

#### Định lý 1 {#top-iii-s4-thm-1 .statement}

*Cho $G$ là một nhóm tôpô Hausdorff tác động liên tục trên một không gian tôpô $X$. Cho $K$ là một tập compact của $X$ và $L$ là một tập đóng của $X$. Khi đó:
a) Tập $P(K, L)$ là đóng trong $G$.*

b) *Nếu G tác động thực sự trên X và nếu L compact, thì P(K, L) compact.*

c) *Ngược lại, nếu X địa phương compact và nếu, với mỗi cặp K, L gồm các tập compact của X, P(K, L) tương đối compact trong G [và do đó compact theo a)]; thì G tác động thực sự trên X (và nếu X không rỗng, G địa phương compact theo Mệnh đề 11).*

Ánh xạ $(s, x) \to s.x$ từ $G \times K$ vào $X$ là liên tục, và do đó ảnh ngược $L'$ của $L$ qua ánh xạ này là đóng. Vì $K$ compact, phép chiếu $\operatorname{pr}_1 : G \times K \to G$ là thực sự (Chương I, § 10, no. 2, Hệ quả 5 của Định lý 1) và do đó ảnh của $L'$ qua $\operatorname{pr}_1$ là đóng. Ảnh này là $P(K, L)$, vậy a) được chứng minh.

Để chứng minh b): $X$ là Hausdorff (no. 2, Mệnh đề 3). Theo giả thiết, ánh xạ $\theta : (s, x) \to (x, s.x)$ từ $G \times X$ vào $X \times X$ là thực sự; vì $K \times L$ compact, nên $\overline{\theta}(K \times L)$ cũng compact do $X$ là Hausdorff (Chương I, § 10, no. 2, Mệnh đề 6). Vậy phép chiếu $P(K, L)$ của $\overline{\theta}(K \times L)$ vào $G$ là một tập compact.

Để chứng minh c): vì $K \times L$ đóng trong $X \times X$, suy ra $\overline{\theta}(K \times L)$ đóng trong $P(K, L) \times K$ và do đó compact dưới các giả thiết của c). Vì mọi tập compact của $X \times X$ đều được chứa trong một tập compact có dạng $K \times L$, suy ra ảnh ngược của mọi tập compact của $X \times X$ qua $\theta$ là compact, và vì $X \times X$ địa phương compact, điều này cho thấy $\theta$ là thực sự (Chương I, § 10, no. 3, Mệnh đề 7) [xem Chương IV, § 1, Bài tập 4c)].

#### Nhận xét {#top-iii-s4-n5-rem-1 .statement}

Rõ ràng, ta có $P(K, L) \subset P(K \cup L, K \cup L)$; do đó để $G$ tác động thực sự trên một không gian địa phương compact $X$, điều kiện đủ là, với mỗi tập compact $K$ của $X$, tập $P(K, K)$ tương đối compact trong $G$. Đặc biệt, một nhóm *rời rạc* $G$ tác động thực sự trên một không gian địa phương compact $X$ khi và chỉ khi, với mỗi tập compact $K$ của $X$, tập các $s \in G$ sao cho $s.K \cap K \neq \emptyset$ là *hữu hạn*.

#### Ví dụ {#top-iii-s4-n5-exa-1 .statement}

Cho $X$ là một đa tạp giải tích phức, đẳng cấu giải tích với một tập con mở bị chặn của $\mathbf{C}^n$, và cho $G$ là nhóm các tự đẳng cấu giải tích của $X$. Tôpô hội tụ compact tương thích với cấu trúc nhóm của $G$, và có thể chứng minh rằng $G$ tác động thực sự trên $X$. Đặc biệt, mọi nhóm con rời rạc của $G$ đều tác động thực sự trên $X$.

Lấy ví dụ $X$ là nửa mặt phẳng trên $\mathcal{J}(z) > 0$, giải tích đẳng cấu với một đĩa mở trong $\mathbf{C}$. Khi đó $G$ là nhóm gồm mọi phép biến đổi $z \to (az + b)/(cz + d)$, trong đó $a, b, c, d$ là các số thực và $ad - bc \neq 0$. Nhóm con $H$ của $G$ gồm tất cả các phép biến đổi như vậy mà ở đó $a, b, c, d$ là các số nguyên và $ad - bc = 1$ là một nhóm con rời rạc của $G$, được gọi là *nhóm môđun*. Theo điều đã nói ở trên, nó tác động một cách thực sự trên nửa mặt phẳng trên $\mathcal{J}(z) > 0$.*

#### Mệnh đề 12 {#top-iii-s4-prop-12 .statement}

Cho G là một nhóm tôpô Hausdorff tác động liên tục trên một không gian tôpô X. Cho K là một tập con compact của X, và cho $\rho_K$ là ánh xạ $(s, x) \to s.x$ từ $G \times K$ vào X. Khi đó:

a) Nếu G tác động một cách thực sự trên X thì $\rho_K$ là thực sự.

b) Nếu X compact địa phương và $\rho_K$ là thực sự với mỗi tập con compact K của X, thì G tác động một cách thực sự trên X.

Ánh xạ $\rho_K$ phân tích thành $G \times K \xrightarrow{\theta_K} K \times X \xrightarrow{\mathrm{pr}_2} X$, trong đó $\theta_K$ là hạn chế trên $G \times K$ của ánh xạ $\theta : (s, x) \to (x, s.x)$ từ $G \times X$ vào $X \times X$. Vì $\theta^{-1}(K \times X) = G \times K$, nên $\theta_K$ là thực sự nếu $\theta$ là thực sự (Chương I, § 10, no. 1, Mệnh đề 3). Mặt khác, vì K compact, phép chiếu $\mathrm{pr}_2 : K \times X \to X$ là thực sự (Chương I, § 10, no. 2, Định lý 1, Hệ quả 5), do đó $\rho_K$ là thực sự (đd., no. 1, Mệnh đề 5).

Ngược lại, giả sử rằng $\rho_K$ là thực sự với mọi compact $K \subset X$. Nếu L là một tập con compact của X, thì $\rho_K^{-1}(L)$ là một tập con compact của $G \times K$, có phép chiếu vào G là $P(K, L)$; do đó $P(K, L)$ compact. Vậy nếu X compact địa phương thì từ Định lý 1 suy ra G tác động một cách thực sự trên X.

#### Hệ quả {#top-iii-s4-n5-cor-1 .statement}

Cho G là một nhóm tôpô Hausdorff tác động một cách thực sự trên một không gian tôpô X. Nếu K là một tập con compact bất kỳ của X và nếu F là một tập con đóng bất kỳ của G, thì F.K đóng trong X.

Điều này suy ra từ Mệnh đề 12 và từ Chương I, § 10, no. 1, Mệnh đề 1.

### 6. KHÔNG GIAN THUẦN NHẤT COMPACT ĐỊA PHƯƠNG

#### Mệnh đề 13 {#top-iii-s4-prop-13 .statement}

Cho G là một nhóm compact địa phương và cho H là một nhóm con đóng của G. Khi đó không gian thuần nhất $G/H$ là compact địa phương và paracompact.

Vì $G/H$ là Hausdorff (§ 2, no. 5, Mệnh đề 13) nên nó compact địa phương, theo Mệnh đề 9 của no. 5 áp dụng cho H tác động trên G ở bên phải. Vậy còn phải chứng minh rằng $G/H$ là paracompact. Cho V là một lân cận compact đối xứng của e trong G, và cho $G_0 = V^\infty$ là nhóm con của G sinh bởi V. $G_0$ là mở (§ 2, no. 1, Hệ quả của Mệnh đề 4) và tác động liên tục trên $G/H$ (§ 2, no. 5, Mệnh đề 12). Nếu ta có thể chứng minh rằng mỗi quỹ đạo $G_0.z \ (z \in G/H)$ là một tập con mở của $G/H$ và là một hợp đếm được của các tập compact, thì sẽ suy ra rằng $G/H$ là *tổng tôpô* của các quỹ đạo phân biệt $G_0.z$ và là

#### Mệnh đề 14 {#top-iii-s4-prop-14 .statement}

*Trong một nhóm compact địa phương $G$, thành phần đơn vị $C$ là giao của các nhóm con mở của $G$.*

$C$ là một nhóm con đóng chuẩn tắc của $G$ ($§ 2$, no. 2, Mệnh đề 7), và do đó $G/C$ là compact địa phương (Mệnh đề 13) và hoàn toàn không liên thông (Chương I, $§ 11$, no. 5, Mệnh đề 9). Vì ảnh ngược của một nhóm con mở của $G/C$, dưới ánh xạ chính tắc từ $G$ lên $G/C$, là một nhóm con mở của $G$ chứa $C$, nên ta thấy rằng ta có thể chỉ cần chứng minh mệnh đề cho nhóm $G/C$. Nói cách khác, ta có thể giả sử rằng $G$ hoàn toàn không liên thông. Khi đó ta biết (Chương II, $§ 4$, no. 4, Hệ quả của Mệnh đề 6) rằng mọi lân cận compact $V$ của $e$ đều chứa một lân cận $U$ của $e$ vừa mở vừa đóng. Vì $U$ là compact và $B = C U$ là đóng, nên tồn tại một lân cận mở đối xứng $W$ của $e$ sao cho $W \subset U$ và $UW \cap BW = \varnothing$ ($§ 3$, no. 1 và Chương II, $§ 4$, no. 3, Mệnh đề 4), và *a fortiori* $UW \subset U$. Bằng quy nạp theo $n$ suy ra rằng $W^n \subset U$ với mọi số nguyên $n > 0$. Do đó nhóm con $W^\infty = \bigcup_{n > 0} W^n$, được sinh bởi $W$, được chứa trong $U$; nhưng $W^\infty$ là mở trong $G$ ($§ 2$, no. 1, Hệ quả của Mệnh đề 4). Điều này hoàn tất chứng minh.

Ta cũng đã chứng minh:

#### Hệ quả 1 {#top-iii-s4-prop-14-cor-1 .statement}

*Nếu $G$ là một nhóm compact địa phương hoàn toàn không liên thông, thì mọi lân cận của $e$ trong $G$ đều chứa một nhóm con mở của $G$.*

#### Hệ quả 2 {#top-iii-s4-prop-14-cor-2 .statement}

*Một nhóm compact địa phương là liên thông nếu nó được sinh bởi mỗi lân cận của phần tử đơn vị.*

#### Hệ quả 3 {#top-iii-s4-prop-14-cor-3 .statement}

*Cho $G$ là một nhóm compact địa phương, cho $H$ là một nhóm con đóng của $G$, và cho $\varphi$ là ánh xạ chính tắc từ $G$ lên $G/H$. Khi đó các thành phần liên thông của $G/H$ là các bao đóng của các ảnh, dưới $\varphi$, của các thành phần liên thông của $G$.*

Cho $C$ là thành phần đơn vị của $G$. Các thành phần của $G$ là các tập $sC$, trong đó $s \in G$ ($§ 2$, no. 2, Mệnh đề 7); $\varphi(sC)$ rõ ràng là liên thông, nên $\varphi(sC)$ cũng vậy (Chương I, $§ 11$, no. 1, Mệnh đề 1). Nhưng $\varphi(sC) = \varphi(sCH)$, và vì $sCH$ là bão hòa đối với quan hệ tương đương do $H$ xác định, và vì quan hệ tương đương này là mở (§ 2, no. 4, Bổ đề 2), ta có $\overline{\varphi(sCH)} = \varphi(\overline{sCH}) = \varphi(s.\overline{CH})$ (Chương I, § 5, no. 3, Mệnh đề 7).

Đặt $L = CH$. $L$ là một nhóm con đóng của $G$ chứa $C$ và $H$; do đó để chứng minh rằng các tập $\varphi(s.L) = s.\varphi(L)$ là các thành phần của $G/H$ thì đủ chứng tỏ rằng không gian thương của $G/H$ theo quan hệ tương đương mà các lớp là các tập $s.\varphi(L)$ là hoàn toàn không liên thông. Bây giờ không gian thương này đồng phôi với không gian thuần nhất $G/L$ (Chương I, § 3, no. 4, Mệnh đề 7); như vậy ta được quy về việc chứng minh rằng khi $C \subset H$, $G/H$ là *hoàn toàn không liên thông*. Vì $G/H$ có thể được đồng nhất với $(G/C)/(H/C)$ (§ 2, no. 7, Mệnh đề 22), ta thậm chí có thể giả sử rằng chính $G$ là hoàn toàn không liên thông. Mọi lân cận của $\varphi(e)$ trong $G/H$ đều chứa một lân cận dạng $\varphi(V)$, trong đó $V$ là một lân cận của $e$ trong $G$, và do đó (Hệ quả 1) chứa một lân cận dạng $\varphi(K)$, trong đó $K$ là một nhóm con *mở compắc* của $G$. Vậy $\varphi(K)$ vừa mở vừa đóng trong $G/H$, và điều này cho thấy thành phần của $\varphi(e)$ trong $G/H$ chỉ gồm riêng $\varphi(e)$. Bởi phép tịnh tiến, điều tương tự cũng đúng với thành phần của mọi điểm của $G/H$, và hệ quả được chứng minh.

### Bài tập {#top-iii-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
