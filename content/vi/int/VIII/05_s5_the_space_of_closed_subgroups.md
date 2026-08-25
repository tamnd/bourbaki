---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 5
section_title: The space of closed subgroups
lang: vi
source: int-vii-ix
book_pages: INT VIII.73-INT VIII.74
pdf_pages: 0146-0159, 0173-0174
extraction: ocr
subsections:
    - "no": 1
      title: The space of Haar measures on the closed subgroups of G
      page: 46
      pdf_page: 146
    - "no": 2
      title: Semi-continuity of the volume of the homogeneous space
      page: 48
      pdf_page: 148
    - "no": 3
      title: The space of closed subgroups of G
      page: 51
      pdf_page: 151
    - "no": 4
      title: The case of groups without arbitrarily small finite subgroups
      page: 53
      pdf_page: 153
    - "no": 5
      title: The case of abelian groups
      page: 55
      pdf_page: 155
    - "no": 6
      title: Another interpretation of the topology of the space of closed subgroups
      page: 56
      pdf_page: 156
statements: 20
exercises: 6
content_sha256: 8de4920034db5ca7cf72789b5b7670eef05b671c28df48a955c57eb0980d32e9
translated_from: content/en/int/VIII/05_s5_the_space_of_closed_subgroups.md
source_content_sha256: 09d2c118abf8c6df99cf173ca74772db4f4d2cb82538ea26cffac744572ce1a0
translation_model: gpt-5.4-mini
translation_run: translate-vi-1ea08f37
glossary_version: 34
glossary_terms_sha256: dff56eebc0c0d919a5d221a83fcf6c179746fdc0a16939f449bdecb5d2b356a5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. KHÔNG GIAN CÁC NHÓM CON ĐÓNG

Trong toàn tiết này, G ký hiệu một nhóm địa phương compact và $\mu$ là một độ đo Haar phải trên G.

### 1. Không gian các độ đo Haar trên các nhóm con đóng của G

#### Bổ đề 1 {#int-viii-s5-lem-1 .statement}

Cho $\alpha$ là một độ đo dương $\neq 0$ trên G, S là giá đỡ của nó; hai điều kiện sau tương đương:
a) S là một nhóm con đóng của G và độ đo cảm sinh bởi $\alpha$ trên S là một độ đo Haar phải trên S.
b) $\delta(s)\alpha = \alpha$ với mọi $s \in S$.
Hơn nữa, khi các điều kiện này được thỏa mãn, tập hợp các $t \in G$ sao cho $\delta(t)\alpha = \alpha$ bằng S.
Rõ ràng a) suy ra b); ngược lại, quan hệ b) suy ra rằng $Sx = S$ với mọi $x \in S$; nói cách khác, các quan hệ $x \in S$ và $y \in S$ suy ra rằng $y \in Sx$, hay cũng suy ra rằng $yx^{-1} \in S$, và vì S khác rỗng, S là một nhóm con đóng của G. Khi đó tập hợp các $t \in G$ sao cho $St = S$ bằng chính S, do đó có khẳng định cuối cùng.

Trong phần còn lại của tiết này, ta ký hiệu bằng $\Gamma$ tập hợp các độ đo dương $\neq 0$ trên G thỏa mãn các điều kiện của Bổ đề 1, và với mọi $\alpha \in \Gamma$ ta ký hiệu bằng $H_\alpha$ nhóm con đóng của G là giá đỡ của $\alpha$.

#### Mệnh đề 1 {#int-viii-s5-prop-1 .statement}

Tập hợp $\Gamma$ là đóng trong không gian $\mathcal{M}_+(G) - \{0\}$ với tôpô mơ hồ.
Trước hết ta chứng minh các bổ đề sau:

#### Bổ đề 2 {#int-viii-s5-lem-2 .statement}

Cho X là một không gian địa phương compact và với mọi độ đo $\alpha \in \mathcal{M}_+(X) - \{0\}$, ký hiệu $S_\alpha$ là giá đỡ của $\alpha$. Cho $\Phi$ là một bộ lọc trên $\mathcal{M}_+(X) - \{0\}$ hội tụ mơ hồ đến một độ đo $\alpha_0 \neq 0$. Khi đó, với mọi lân cận V của một điểm s thuộc giá đỡ của $\alpha_0$, tồn tại một tập $M \in \Phi$ sao cho, với mọi $\alpha \in M$, ta có $V \cap S_\alpha \neq \varnothing$.
Thật vậy, nếu $\varphi \in \mathcal{K}_+(X)$ là một hàm có giá đỡ chứa trong V và sao cho $\int \varphi(x) d\alpha_0(x) > 0$, thì theo định nghĩa tồn tại một tập $M \in \Phi$ sao cho $\int \varphi(x) d\alpha(x) > 0$ với mọi $\alpha \in M$, điều này suy ra $V \cap S_\alpha \neq \varnothing$.

#### Bổ đề 3 {#int-viii-s5-lem-3 .statement}

Cho E là một tập được lọc bởi một bộ lọc $\Phi$, và cho $\xi \mapsto \alpha(\xi)$ là một ánh xạ từ E vào $\Gamma$ hội tụ mơ hồ đối với $\Phi$ tới một độ đo $\alpha_0 \neq 0$. Mặt khác, cho $\xi \mapsto t_\xi$ là một ánh xạ từ E vào G sao cho $t_\xi \in H_{\alpha(\xi)}$ với mọi $\xi \in E$. Nếu s là một điểm tụ của ánh xạ $\xi \mapsto t_\xi$ đối với $\Phi$, thì $\delta(s)\alpha_0 = \alpha_0$.

Nếu cần, thay $\Phi$ bằng một bộ lọc mịn hơn, ta có thể giả sử rằng $s$ là một giới hạn của $\xi \mapsto t_\xi$ đối với $\Phi$; theo Bổ đề 1, $\delta(t_\xi)\alpha(\xi) = \alpha(\xi)$ với mọi $\xi \in E$, và kết luận suy ra từ tính liên tục của ánh xạ $(u, \lambda) \mapsto \delta(u)\lambda$ trên $G \times \mathcal{M}_+(G)$ (\S 3, No. 3, Mệnh đề 13).

Để chứng minh Mệnh đề 1, theo Bổ đề 1, chỉ cần chỉ ra rằng nếu một bộ lọc $\Psi$ trên $\Gamma$ hội tụ một cách mơ hồ đến một độ đo $\alpha_0 \neq 0$ và nếu $s$ thuộc giá đỡ của $\alpha_0$, thì $\delta(s)\alpha_0 = \alpha_0$. Thật vậy, với mọi lân cận $V$ của $s$ trong $G$, tồn tại một $M \in \Psi$ sao cho, với mọi $\alpha \in M$, ta có $V \cap H_\alpha \neq \varnothing$, theo Bổ đề 2. Với mọi lân cận $V$ của $s$ và mọi $\alpha \in \Gamma$, hãy lấy $t_{V,\alpha}$ là một điểm của $V \cap H_\alpha$ nếu $V \cap H_\alpha \neq \varnothing$, và là bất kỳ điểm nào của $H_\alpha$ trong trường hợp ngược lại; nếu $\Theta$ là bộ lọc tiết diện của bộ lọc các lân cận của $s$, và $\Phi$ là bộ lọc tích $\Theta \times \Psi$, thì theo điều trên, $s$ là một điểm tụ của $(V, \alpha) \mapsto t_{V,\alpha}$ đối với $\Phi$. Mặt khác, vì ánh xạ $(V, \alpha) \mapsto \alpha$ có giới hạn $\alpha_0$ đối với $\Phi$, mệnh đề suy ra từ Bổ đề 3.

#### Mệnh đề 2 {#int-viii-s5-prop-2 .statement}

— Cho $\varphi$ là một hàm trong $\mathscr{K}_+(G)$ sao cho $\varphi(e) > 0$. Khi đó tập $\Gamma_\varphi$ các độ đo $\alpha \in \Gamma$ sao cho $\int \varphi(x)\,d\alpha(x) = 1$ là compact theo tôpô mơ hồ.

Tập $\Gamma_\varphi$ là giao của $\Gamma$ với siêu phẳng của $\mathcal{M}(G)$ được tạo bởi các $\alpha$ sao cho $\int \varphi(x)\,d\alpha(x) = 1$; vì siêu phẳng này đóng mơ hồ trong $\mathcal{M}(G)$ và không chứa 0, suy ra từ Mệnh đề 1 rằng $\Gamma_\varphi$ đóng mơ hồ trong $\mathcal{M}(G)$. Do đó chỉ cần chứng minh rằng với mọi tập con compact $K$ của $G$, ta có $\sup_{\alpha \in \Gamma_\varphi} \alpha(K) < +\infty$ (Ch. III, §1, No. 9, Mệnh đề 15). Bây giờ, cho $U$ là lân cận mở của $e$ trong $G$ được xác định bởi bất đẳng thức $\varphi(x) > \varphi(e)/2$; vì $1 = \int \varphi(x)\,d\alpha(x) \geq \int_U \varphi(x)\,d\alpha(x)$ đối với $\alpha \in \Gamma_\varphi$, ta thấy rằng, khi đặt $c = 2/\varphi(e)$, ta có $\alpha(U) \leq c$ với mọi $\alpha \in \Gamma_\varphi$. Cho $V$ là một lân cận mở đối xứng của $e$ trong $G$ sao cho $V^2 \subset U$; hãy chứng minh rằng $\alpha(Vx) \leq c$ với mọi $x \in G$ và mọi $\alpha \in \Gamma_\varphi$. Thật vậy, quan hệ này là tầm thường nếu $Vx không giao với giá đỡ H_\alpha$ của α; nếu, ngược lại, tồn tại một $h \in Vx \cap H_\alpha$, thì $h = vx$ với một $v \in V$, do đó
$$
Vx = Vv^{-1}h \subset V^2h \subset Uh,
$$
và vì $\delta(h)\alpha = \alpha$, suy ra rằng $\alpha(Vx) \leq \alpha(Uh) = \alpha(U) \leq c$. Bây giờ lấy $(x_i)_{1 \leq i \leq n}$ là một dãy các điểm của $K$ sao cho các $Vx_i$ tạo thành một phủ của $K$; suy ra từ điều trên rằng $\alpha(K) \leq \sum_{i=1}^n \alpha(Vx_i) \leq nc$ với mọi $\alpha \in \Gamma_\varphi$; Q.E.D.

#### Mệnh đề 3 {#int-viii-s5-prop-3 .statement}

— *Dưới các giả thiết của Mệnh đề 2, ánh xạ* $\alpha \mapsto \left( \langle \varphi, \alpha \rangle, \frac{\alpha}{\langle \varphi, \alpha \rangle} \right)$ *là một đồng phôi từ* $\Gamma$ *lên không gian tích* $\mathbf{R}_+^* \times \Gamma_\varphi$.

Vì ánh xạ $\alpha \mapsto \langle \varphi, \alpha \rangle$ liên tục mơ hồ, chỉ cần nhận xét rằng $\langle \varphi, \alpha \rangle \neq 0$ với mọi độ đo $\alpha \in \Gamma$, vì $e$ thuộc giá đỡ $H_\alpha$ của $\alpha$ và $\varphi(e) > 0$.

### 2. Tính nửa liên tục của thể tích của không gian thuần nhất

Trong mục này, với mỗi độ đo $\alpha \in \Gamma$ ta đặt

$$
Q_\alpha = G / H_\alpha ,
$$

và kí hiệu $\pi_\alpha$ là ánh xạ chính tắc $G \to Q_\alpha$.

Cho $\Gamma^0$ là tập con của $\Gamma$ gồm các độ đo $\alpha$ sao cho nhóm con $H_\alpha$ của $G$ là *đơn môđula*; các phần tử của $\Gamma^0$ được đặc trưng bởi tính chất rằng $\alpha(f) = \alpha(\dot{f})$ với mọi hàm $f \in \mathcal{K}(G)$ (mọi hàm của $\mathcal{K}(H_\alpha)$ đều có thể mở rộng thành một hàm của $\mathcal{K}(G)$ theo định lý Urysohn); suy ra $\Gamma^0$ là một tập con *đóng* của $\Gamma$. Nhắc lại rằng với mọi $\alpha \in \Gamma^0$, độ đo thương $\mu_\alpha = \mu / \alpha$ trên $Q_\alpha$ được xác định và là bất biến tương đối dưới $G$ (Ch. VII, §2, No. 6, Th. 3); cũng nhắc lại rằng với mọi hàm $f \in \mathcal{K}(G)$,

$$
\int_G f(x) d\mu(x) = \int_{Q_\alpha} d\mu_\alpha(\dot{x}) \int_{H_\alpha} f(xs) d\alpha(s) ,
$$

trong đó $\dot{x} = \pi_\alpha(x)$ là ảnh chính tắc của $x \in G$ trong $Q_\alpha$.

#### Mệnh đề 4 {#int-viii-s5-prop-4 .statement}

— *Cho* $\Gamma^0$ *là tập các độ đo* $\alpha \in \Gamma$ *sao cho* $H_\alpha$ *là đơn môđula, và với mọi* $\alpha \in \Gamma^0$ *đặt* $\mu_\alpha = \mu / \alpha$; *khi đó ánh xạ* $\alpha \mapsto \| \mu_\alpha \|$ *từ* $\Gamma^0$ *vào* $\overline{\mathbf{R}}$ *là nửa liên tục dưới đối với tôpô mơ hồ*.

Với mọi $\alpha \in \Gamma^0$ và mọi hàm $f \in \mathcal{K}(G)$, đặt

$$
f_\alpha(\dot{x}) = \int_{H_\alpha} f(xs) d\alpha(s) = (f * \alpha)(x) ,
$$

trong đó tích chập được lấy tương ứng với độ đo Haar phải $\mu$ và trong đó ta dùng đến thực tế là $\dot{\alpha} = \alpha$ (\S 4, No. 4, công thức (11)). Ta biết (Ch. VII, §2, No. 1, Prop. 2) rằng ánh xạ $f \mapsto f_\alpha$ của $\mathcal{K}_+(G)$ vào $\mathcal{K}_+(Q_\alpha)$ là *toàn ánh*; do đó, theo (2),

$$
\| \mu_\alpha \| = \sup_{f \in \mathcal{K}_+(G), f \neq 0} \mu_\alpha(f_\alpha) / \| f_\alpha \| = \sup_{f \in \mathcal{K}_+(G), f \neq 0} \mu(f) / \| f_\alpha \|,
$$

trong đó ta đã đặt

$$
\|f_\alpha\| = \sup_{\dot{x} \in Q_\alpha} |f_\alpha(\dot{x})| = \sup_{x \in G} |(f * \alpha)(x)| .
$$

Để chứng minh mệnh đề, chỉ cần chỉ ra rằng, cho trước $f \in \mathcal{H}_+(G)$, ánh xạ $\alpha \mapsto \|f_\alpha\|$ là liên tục theo tôpô mơ hồ. Bây giờ, gọi K là giá đỡ của f; hàm $f * \alpha$ có giá đỡ được chứa trong $KH_\alpha$ và bất biến phải dưới $H_\alpha$; do đó

$$
\|f_\alpha\| = \sup_{x \in K} |(f * \alpha)(x)| .
$$

Suy ra kết luận từ thực tế rằng ánh xạ $\alpha \mapsto f * \alpha$ của $\mathcal{M}_+(G)$, được trang bị tôpô mơ hồ, vào $\mathcal{C}(G)$, được trang bị tôpô hội tụ trên các tập compact, là liên tục (\S 4, No. 2, Nhận xét 1).

Nhắc lại rằng nếu, với một độ đo $\alpha \in \Gamma^0$, $\|\mu_\alpha\|$ là hữu hạn, thì G tất yếu là đơn môđula (Ch. VII, §2, No. 6, Hệ quả 3 của Th. 3).

#### Mệnh đề 5 {#int-viii-s5-prop-5 .statement}

*Cho g là một hàm số dương khả tích theo $\mu$ và cho $\Gamma^0(g)$ là tập các độ đo $\alpha \in \Gamma^0$ sao cho $\int^* g(xs)\, d\alpha(s) \geq 1$ với mọi $x \in G$. Khi đó ánh xạ $\alpha \mapsto \|\mu_\alpha\|$ của $\Gamma^0(g)$ vào $\overline{\mathbf{R}}$ là liên tục theo tôpô mơ hồ.*

Với mọi độ đo $\alpha \in \Gamma^0(G)$, nhắc lại (Ch. VII, §2, No. 3, Prop. 5) rằng hàm

$$
g_\alpha(\dot{x}) = \int_{H_\alpha} g(xs)\, d\alpha(s)
$$

được xác định $\mu_\alpha$-gần khắp trên $Q_\alpha$, khả tích theo $\mu_\alpha$, và

$$
\int_G g(x)\, d\mu(x) = \int_{Q_\alpha} g_\alpha(\dot{x})\, d\mu_\alpha(\dot{x}) .
$$

Xét theo Mệnh đề 4, chỉ cần chứng minh rằng, trong $\Gamma^0(g)$, $\alpha \mapsto \|\mu_\alpha\|$ là *nửa liên tục trên*. Cố định một độ đo $\alpha \in \Gamma^0(g)$, và cho $K$ là một tập con compact của $G$. Có một hàm liên tục trên $Q_\alpha$ với giá compact, nhận các giá trị trong $[0, 1]$, bằng 1 trên tập compact $\pi_\alpha(K)$; vì ánh xạ $f \mapsto f_\alpha$ của $\mathcal{H}_+(G)$ vào $\mathcal{H}_+(Q_\alpha)$ là toàn ánh (Ch. VII, §2, No. 1, Mệnh đề 2), suy ra tồn tại một hàm $f \in \mathcal{H}_+(G)$ sao cho

$$
(f * \alpha)(x) = \int_G f(xs)\, d\alpha(s) \left\{ \begin{array}{ll}
\leq 1 & \text{với mọi } x \in G \\
= 1 & \text{với mọi } x \in K .
\end{array} \right.
$$

Vì $\beta \mapsto f * \beta$ là một ánh xạ liên tục từ $\mathcal{M}_+(G)$, được trang bị tôpô mơ hồ, vào $\mathcal{C}(G)$ được trang bị tôpô hội tụ compact (\S 4, No. 2, Nhận xét 1), ta thấy rằng với mọi $\varepsilon > 0$, tập $U_\varepsilon$ gồm các $\beta \in \Gamma^0(G)$ sao cho
$$
f_\beta(\dot{x}) = \int_G f(xs)\, d\beta(s) > 1 - \varepsilon \quad \text{với mọi } x \in K
$$
là một lân cận mở của $\alpha$ trong $\Gamma^0(g)$; với mọi $\beta \in U_\varepsilon$, khi đó, nhờ công thức (2),
$$
(5) \quad \| \mu_\alpha \| \geq \int_G f(x)\, d\mu(x) = \int_{Q_\beta} f_\beta(\dot{x})\, d\mu_\beta(\dot{x}) \geq (1 - \varepsilon) \mu_\beta(\pi_\beta(K)).
$$
Cho một số $\varepsilon > 0$, ta chọn một hàm $h \in \mathcal{K}_+(G)$ sao cho $\int_G |g(x) - h(x)|\, d\mu(x) \leq \varepsilon$, và trong phần trên lấy $K = \mathrm{Supp}(h)$. Với mọi $\beta \in \Gamma^0(g)$, theo giả thiết $g_\beta(\dot{x}) \geq 1$ hầu khắp (đối với $\mu_\beta$) trên $Q_\beta$, do đó
$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{Q_\beta - \pi_\beta(K)} g_\beta(\dot{x})\, d\mu_\beta(\dot{x}) = \int_{G - KH_\beta} g(x)\, d\mu(x)
$$
nhờ (4); vì $h$ bằng không ngoài $K$, và a fortiori ngoài $KH_\beta$, suy ra rằng
$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{G - KH_\beta} |g(x) - h(x)|\, d\mu(x) \\
\leq \int_G |g(x) - h(x)|\, d\mu(x) \leq \varepsilon;
$$
kết hợp kết quả này với (5), ta thấy rằng
$$
\| \mu_\beta \| \leq \varepsilon + \| \mu_\alpha \|/(1 - \varepsilon)
$$
khi $\beta \in U_\varepsilon$, và điều đó hoàn tất chứng minh.

#### Hệ quả 1 {#int-viii-s5-prop-5-cor-1 .statement}

— Cho $K$ là một tập con compact của $G$, $V$ là một lân cận compact đối xứng của $e$ trong $G$, $c$ là một số thực $> 0$. Hạn chế của ánh xạ $\alpha \mapsto \| \mu_\alpha \|$ lên tập các $\alpha \in \Gamma^0$ sao cho $G = KH_\alpha$ và $\alpha(V) \geq c$ là liên tục theo tôpô mơ hồ.

Vì, cho $g \in \mathcal{K}_+(G)$ là một hàm sao cho $g(x) \geq 1/c$ với $x \in KV$. Với mọi $x \in K$,
$$
\int g(xs)\, d\alpha(s) \geq \int_V g(xs)\, d\alpha(s) \geq 1
$$

cho $\alpha$ thỏa mãn các điều kiện của mệnh đề; hơn nữa, vì $\pi_\alpha(K) = Q_\alpha$, nên $\alpha \in \Gamma^0(g)$, do đó suy ra hệ quả.

#### Hệ quả 2 {#int-viii-s5-prop-5-cor-2 .statement}

*Cho A là một tập con $\mu$-khả tích của G. Sự hạn chế của ánh xạ $\alpha \mapsto \| \mu_\alpha \|$ lên tập $N_A$ của các độ đo Haar chuẩn hóa của các nhóm con rời rạc H của G sao cho $G = AH$, là liên tục mơ hồ.*

Với $a \in A$ và $\alpha \in N_A$,

$$
\int \varphi_A(as)\ d\alpha(s) \geq \varphi_A(a) = 1,
$$

và vì $\pi_\alpha(A) = Q_\alpha$, nên $N_A \subset \Gamma^0(\varphi_A)$, và do đó hệ quả suy ra từ Mệnh đề 5.

### 3. Không gian các nhóm con đóng của G

Ký hiệu $\Sigma$ là tập hợp các *nhóm con đóng* của G; nếu gán cho mỗi độ đo $\alpha \in \Gamma$ nhóm con $H_\alpha$ là giá đỡ của $\alpha$, ta thu được một ánh xạ (gọi là chính tắc) từ $\Gamma$ vào $\Sigma$, ánh xạ này rõ ràng là toàn ánh và cho phép xác định một cách chính tắc $\Sigma$ với tập hợp các quỹ đạo của nhóm các phép vị tự trong $\Gamma$ với tỉ số $> 0$. Tập $\Sigma$, được trang bị tôpô thương của tôpô mơ hồ trên $\Gamma$, được gọi là *không gian các nhóm con đóng* của G.

#### Định lý 1 {#int-viii-s5-thm-1 .statement}

*Cho G là một nhóm địa phương compact. Không gian $\Sigma$ của các nhóm con đóng của G là compact. Hơn nữa, ta có các tính chất sau:*

(i) *Tập $\Sigma^0$ của các nhóm con đóng đơn môđula của G là đóng trong $\Sigma$ (nên compact).*

(ii) *Nếu G được sinh bởi một lân cận compact của e, thì tập $\Sigma_c^0$ của các nhóm con đóng đơn môđula H của G sao cho không gian thương $G/H$ là compact, là mở trong $\Sigma^0$ (nên là địa phương compact).*

(iii) *Với mọi lân cận mở U tương đối compact của e trong G, tập $D_U$ của các nhóm con rời rạc H của G sao cho $H \cap U = \{e\}$ là đóng trong $\Sigma^0$ (nên compact).*

Suy ra từ Mệnh đề 3 của No. 1 rằng $\Sigma$ đẳng cấu tôpô với $\Gamma_\varphi$, nên compact theo Mệnh đề 2 của No. 1. Hơn nữa, ở đầu No. 2 đã nhận xét rằng tập $\Gamma^0$ các độ đo $\alpha \in \Gamma$ sao cho $H_\alpha$ là đơn môđula là đóng trong $\Gamma$; vì $\Gamma^0$ ổn định qua các phép vị tự với tỉ số $> 0$, ảnh $\Sigma^0$ của $\Gamma^0$ trong $\Sigma$ là một tập con đóng của $\Sigma$, điều này chứng minh (i).

Tính chất (ii) sẽ là hệ quả của mệnh đề sau:

#### Mệnh đề 6 {#int-viii-s5-prop-6 .statement}

*Giả sử rằng nhóm địa phương compact G được sinh bởi một lân cận compact của e. Khi đó tập $\Gamma_c^0$ của các độ đo $\alpha \in \Gamma^0$* sao cho $G/H_\alpha$ là compact là mở trong $\Gamma^0$, và sự hạn chế lên $\Gamma_c^0$ của ánh xạ $\alpha \mapsto \| \mu_\alpha \|$ là liên tục mơ hồ.

Với các ký hiệu của Mệnh đề 5 của No. 2, ta có, với $g \in \mathcal{K}_+(G)$,

$$
\Gamma^0(g) \subset \Gamma_c^0.
$$

Vì, nếu K là giá đỡ của $g$, thì quan hệ $\int g(xs)\, d\alpha(s) \geq 1$ với mọi $x \in G$ suy ra $KH_\alpha = G$, do tích phân hiển nhiên bằng không trên phần bù của $KH_\alpha$, do đó $G/H_\alpha = \pi_\alpha(K)$ là compact. Cho một độ đo $\alpha \in \Gamma_c^0$, vì thế chỉ cần định nghĩa một hàm $g \in \mathcal{K}_+(G)$ sao cho $\Gamma^0(g)$ là một lân cận của $\alpha$ trong $\Gamma^0$. Vì $G/H_\alpha$ là compact và ánh xạ chính tắc $f \mapsto f_\alpha$ của $\mathcal{K}_+(G)$ vào $\mathcal{K}_+(G/H_\alpha)$ là toàn ánh (Ch. VII, §2, No. 2), nên tồn tại một hàm $g \in \mathcal{K}_+(G)$ sao cho $\int g(xs)\, d\alpha(s) = 2$ với mọi $x \in G$. Cho K là giá đỡ (compact) của $g$, L là một lân cận compact đối xứng của $e$ trong G sinh ra G; vì ánh xạ $\beta \mapsto g * \beta$ của $\mathcal{M}_+(G)$ vào $\mathcal{C}(G)$ là liên tục mờ (\S4, No. 2, *Nhận xét* 1), nên tồn tại một lân cận $W$ của $\alpha$ trong $\Gamma^0$ sao cho

$$
(g * \beta)(x) = \int g(xs)\, d\beta(s) \geq 1
$$

với mọi $\beta \in W$ và $x \in LK$. Vì vế thứ nhất của (7) bằng không ngoài $KH_\beta$, nên điều kiện $\beta \in W$ suy ra

$$
LK \subset KH_\beta,
$$

từ đó suy ra, bằng quy nạp theo $n$, rằng $L^n K \subset KH_\beta$ với mọi số nguyên $n > 0$; vì L sinh ra G, nên ta có $G = KH_\beta$ với mọi độ đo $\beta \in W$, điều đó chứng minh rằng $W \subset \Gamma_c^0$. Mặt khác, vì vế thứ nhất của (7) bất biến phải dưới $H_\beta$, nên bất đẳng thức (7) cũng đúng với $x \in LKH_\beta = G$; do đó $W \subset \Gamma^0(g)$, điều đó chứng minh mệnh đề.

Sau cùng, (iii) sẽ là hệ quả của mệnh đề sau:

#### Mệnh đề 7 {#int-viii-s5-prop-7 .statement}

*Cho $N \subset \Gamma^0$ là không gian con gồm các độ đo Haar chuẩn hóa trên các nhóm con rời rạc của G, và với mọi lân cận mở tương đối compact U của e trong G, cho $N_U$ là tập con của N gồm các $\alpha$ sao cho $H_\alpha \cap U = \{e\}$. Khi đó:
a) $N_U$ là compact.
b) Các miền trong của các tập $N_U$ trong N tạo thành một phủ của N, khi U chạy qua tập các lân cận mở tương đối compact của e trong G.
c) Để một tập con M của N là tương đối compact trong N, điều kiện cần và đủ là tồn tại một lân cận mở tương đối compact U của e trong G sao cho $M \subset N_U$.*

Vì $D_U$ là ảnh của $N_U$ qua ánh xạ liên tục chính tắc $\Gamma \to \Sigma$, nên mệnh đề (iii) của Định lý 1 sẽ suy ra ngay từ Mệnh đề 7 a).

Để chứng minh Mệnh đề 7, ta nhận thấy rằng $N_U$ có thể được định nghĩa như là tập con của $\Gamma^0$ gồm các $\alpha$ sao cho cả hai

$$
\alpha(\{e\}) \geq 1 \quad \text{và} \quad \alpha(U) \leq 1.
$$

Bây giờ, nếu $A$ là compact (resp. open and relatively compact) trong $G$, thì ánh xạ $\alpha \mapsto \alpha(A)$ của $\mathcal{M}_+(G)$ vào $\mathbf{R}$ là nửa liên tục trên (resp. nửa liên tục dưới) đối với tôpô mơ hồ (Ch. IV, §4, No. 4, Hệ quả 3 của Mệnh đề 5 và loc. cit., §1, No. 1, Mệnh đề 4); do đó ta thấy rằng $N_U$ là một tập con đóng của $\Gamma^0$. Hơn nữa, cho $\varphi \in \mathcal{K}_+(G)$ là một hàm sao cho $\varphi(e) = 1$ và $\varphi(x) = 0$ trên $G - U$; hiển nhiên là $\int \varphi(x) d\alpha(x) = 1$ với mọi $\alpha \in N_U$; Mệnh đề 2 của No. 1 do đó cho thấy rằng $N_U$ là một tập compact, điều này chứng minh a). Mặt khác, hãy cho $V$ là một lân cận mở compact tương đối của $e$ trong $G$ sao cho $\overline{V} \subset U$, và cho $\varphi \in \mathcal{K}_+(G)$, với giá được chứa trong $U$ và sao cho $\varphi(x) = 1$ trên $V$. Khi đó $\alpha(\varphi) = 1$ với $\alpha \in N_U$, do đó tồn tại một lân cận $W$ của $\alpha$ trong $N$ sao cho $\beta(\varphi) < 2$ với $\beta \in W$; khi đó hiển nhiên là $W \subset N_V$, do đó $N_V$ là một lân cận của $N_U$. Vì các $N_U$ phủ $N$, điều này chứng minh b). Cuối cùng, mọi tập con compact $M$ của $N$ đều được chứa trong một hợp hữu hạn các tập $N_{U_i}$ ($1 \leq i \leq n$), và vì $\bigcup_i N_{U_i} \subset N_U$, với $U = \bigcap_i U_i$, điều này chứng minh c).

#### Hệ quả {#int-viii-s5-n3-cor-1 .statement}

— *Không gian con* $N$ *của* $\Gamma^0$ *là locally compact*.

### 4. Trường hợp các nhóm không có các nhóm con hữu hạn tùy ý nhỏ

#### Định lý 2 {#int-viii-s5-thm-2 .statement}

— *Cho* $G$ *là một nhóm compact địa phương thỏa mãn điều kiện sau*:
(L) *Tồn tại một lân cận của* $e$ *trong* $G$ *chứa không có nhóm con hữu hạn nào của* $G$ *không thu gọn về* $e$.
*Các tính chất sau đó đúng*:
(i) *Tập* $D$ *các nhóm con rời rạc của* $G$ *là đóng địa phương trong* $\Sigma$ *(điều đó tương đương với việc nói rằng nó là compact địa phương)*.
(ii) *Để một tập con đóng* $A$ *của* $D$ *là compact, điều kiện cần và đủ là tồn tại một lân cận* $U$ *của* $e$ *trong* $G$ *sao cho* $H \cap U = \{e\}$ *với mọi nhóm con* $H \in A$.
(iii) *Nếu thêm vào đó* $G$ *được sinh bởi một lân cận compact của* $e$, *thì tập* $D_c$ *các nhóm con rời rạc* $H$ *của* $G$ *sao cho* $G/H$ *là compact là đóng địa phương trong* $\Sigma$ *(do đó là compact địa phương)*.

Ta có $D_c = D \cap \Sigma_c^0$, do đó (iii) là hệ quả của (i), và ĐL. 1 (ii) của No. 3.

Với các ký hiệu của No. 3, Mệnh đề 7, để chứng minh (i) và (ii), chỉ cần chứng minh rằng:

#### Mệnh đề 8 {#int-viii-s5-prop-8 .statement}

*Song ánh chính tắc của N lên D là một đồng phôi.*

Bây giờ, nếu $\Gamma_d$ là tập các độ đo Haar trên các nhóm con rời rạc của $G$, thì $D$ đồng phôi một cách chính tắc với không gian các quỹ đạo của nhóm các phép đồng dạng trong $\Gamma_d$ với tỉ số $> 0$ (GT, I, §5, No. 2, Prop. 4). Vì vậy chỉ cần chứng minh rằng ánh xạ chính tắc $\alpha \mapsto (\alpha(\{e\}), \alpha/\alpha(\{e\}))$ của $\Gamma_d$ lên $\mathbf{R}_+^* \times \mathbf{N}$ là một *đồng phôi*, điều này sẽ suy ra từ bổ đề sau:

#### Bổ đề 4 {#int-viii-s5-lem-4 .statement}

*Nếu nhóm* G *thỏa mãn điều kiện (L), thì ánh xạ* $\alpha \mapsto \alpha(\{e\})$ *của* $\Gamma_d$ *vào* $\mathbf{R}_+^*$ *là liên tục mơ hồ.*

Cho ta xét một độ đo $\alpha \in \Gamma_d$; cho $V_0$ là một lân cận mở tương đối compact của $e$ trong $G$ sao cho $H_\alpha \cap V_0 = \{e\}$ và sao cho không có nhóm con hữu hạn nào của $G$ được chứa trong $V_0$ mà không thu gọn về $e$. Cho $V$ là một lân cận compact đối xứng của $e$ sao cho $V^3 \subset V_0$, và cho $U$ là một lân cận đối xứng của $e$ sao cho $U^2 \subset V$. Cho $\varphi$ (tương ứng $\psi$) là một hàm trong $\mathcal{H}_+(G)$, với giá trị trong $[0, 1]$, bằng 1 trên $V^3$ (tương ứng tại điểm $e$) và có giá đỡ được chứa trong $V_0$ (tương ứng trong $U$). Tập các độ đo $\beta \in \Gamma_d$ sao cho $|\beta(\varphi) - \alpha(\varphi)| \leq \varepsilon$ và $|\beta(\psi) - \alpha(\psi)| \leq \varepsilon$ là một lân cận $W$ của $\alpha$. Ta sẽ chứng minh rằng, nếu lấy $\varepsilon$ đủ nhỏ, thì $H_\beta \cap V = \{e\}$ *với mọi* $\beta \in W$; khi đó suy ra $\beta(\psi) = \beta(\{e\})$, do đó $|\beta(\{e\}) - \alpha(\{e\})| \leq \varepsilon$, và điều này sẽ chứng minh bổ đề.

Chỉ cần chứng minh rằng, với $\beta \in W$,

$$
(V^2 - V) \cap H_\beta = \varnothing.
$$

Thật vậy, giả sử mệnh đề này đã được thiết lập: khi đó, với $x$ và $y$ trong $V \cap H_\beta$, ta có $xy^{-1} \in V^2 \cap H_\beta$; nhưng, nhờ (8), điều này suy ra $xy^{-1} \in V \cap H_\beta$; nói cách khác, $V \cap H_\beta$ là một *nhóm con* của $G$, điều này hiển nhiên là rời rạc và compact, suy ra hữu hạn; nhưng khi đó, do cách chọn $V_0$, suy ra thật vậy $V \cap H_\beta = \{e\}$.

Ta lập luận phản chứng và giả sử rằng tồn tại một phần tử $z$ của $V^2 - V$ thuộc $H_\beta$; do cách chọn $U$ và $V$, ta có $\psi(sz^{-1}) + \psi(s) \leq \varphi(s)$ trong $G$, quan hệ $z \notin U^2$ suy ra $Uz \cap U = \varnothing$. Vì

$$
\int \psi(sz^{-1})\, d\beta(s) = \int \psi(s)\, d\beta(s),
$$

suy ra $2\beta(\psi) \leq \beta(\varphi) \leq \alpha(\varphi) + \varepsilon$; nhưng ta cũng có
$$
\beta(\psi) \geq \alpha(\psi) - \varepsilon,
$$
và theo cách dựng $\alpha(\varphi) = \alpha(\psi) = \alpha(\{e\})$. Vì thế ta đi đến mâu thuẫn khi lấy $\varepsilon < \alpha(\{e\})/3$. Q.E.D.

Nói một cách hình tượng, một nhóm $G$ thỏa mãn điều kiện (L) được nói là *không có các nhóm con hữu hạn tùy ý nhỏ*. Có thể chứng minh rằng mọi nhóm Lie đều thỏa mãn điều kiện (L); nhưng điều kiện này không đặc trưng cho các nhóm Lie; chẳng hạn, nhóm nhân của các số nguyên p-adic đồng dư với 1 mod p thỏa mãn (L).*

### 5. Trường hợp các nhóm Abel

Cho $G$ là một nhóm địa phương compact, $N \subset \Gamma^0$ là không gian con của các độ đo Haar chuẩn hóa trên các nhóm con rời rạc của $G$, và $N_c$ là tập con của $N$ tương ứng với các nhóm con rời rạc $H$ của $G$ sao cho $G/H$ là *compact*; do đó $N_c = N \cap \Gamma_c^0$ theo ký hiệu của No. 3, Prop. 6; và nếu nhóm $G$ được sinh bởi một lân cận compact của $e$, thì từ No. 3, Prop. 6 suy ra rằng $N_c$ là *mở* trong $N$ (do đó là *địa phương compact* theo No. 3, Cor. của Prop. 7) và rằng hạn chế của ánh xạ $\alpha \mapsto \| \mu_\alpha \|$ lên $N_c$ là *liên tục mơ hồ*.

#### Mệnh đề 9 {#int-viii-s5-prop-9 .statement}

*Cho $G$ là một nhóm Abel địa phương compact, được sinh bởi một lân cận compact của $e$. Để một tập con $A$ của $N_c$ là tương đối compact trong $N_c$, điều kiện cần và đủ là nó thỏa mãn hai điều kiện sau:*

(i) *Tồn tại một lân cận mở $U$ của $e$ trong $G$ sao cho $H_\alpha \cap U = \{e\}$ với mọi $\alpha \in A$.*

(ii) *Tồn tại một hằng số $k$ sao cho $\mu_\alpha(G/H_\alpha) \leq k$ với mọi $\alpha \in A$.*

Nếu $A \subset N_c$ tương đối compact trong $N_c$ thì nó *a fortiori* cũng vậy trong $N$, và do đó tính cần thiết của các điều kiện (i) và (ii) suy ra từ No. 3, Props. 6 và 7 (không giả thiết $G$ là Abel). Ngược lại, giả sử rằng $A \subset N_c$ thỏa mãn các điều kiện này; nếu $\overline{A}$ là bao đóng của $A$ *trong* $N$, thì $\overline{A}$ compact nhờ No. 3, Prop. 7; hơn nữa, vì $\alpha \mapsto \| \mu_\alpha \|$ là nửa liên tục dưới trên $\Gamma^0$ đối với tôpô mơ hồ (No. 2, Prop. 4), điều kiện (ii) suy ra rằng ta cũng có $\| \mu_\alpha \| \leq k$ với mọi $\alpha \in \overline{A}$. Bây giờ, vì $G$ là Abel, $\mu_\alpha = \mu/\alpha$ là một độ đo Haar trên nhóm $G/H_\alpha$, và do đó $G/H_\alpha$ compact với mọi $\alpha \in \overline{A}$ (Ch. VII, §1, No. 2, Prop. 2). Điều này có nghĩa là $\overline{A} \subset N_c$, do đó $A$ tương đối compact trong $N_c$.

#### Hệ quả {#int-viii-s5-n5-cor-1 .statement}

*Cho $G$ là một nhóm Abel địa phương compact, được sinh bởi một lân cận compact của $e$ và thỏa mãn điều kiện (L) của No. 4.*

Cho $D_c$ là tập hợp các nhóm con rời rạc $H$ của $G$ sao cho $G/H$ là compact, và, với mọi $H \in D_c$, đặt $v(H)$ là khối lượng toàn phần $\mu_\alpha(G/H)$, trong đó $\mu_\alpha$ là độ đo thương của $\mu$ theo độ đo Haar chuẩn hóa $\alpha$ của $H$. Để một tập con $A$ của không gian $D_c$ là tương đối compact trong $D_c$, cần và đủ là nó thỏa mãn hai điều kiện sau:

(i) Tồn tại một lân cận mở $U$ của $e$ trong $G$ sao cho $H \cap U = \{e\}$ với mọi $H \in A$.

(ii) Tồn tại một hằng số $k$ sao cho $v(H) \leq k$ với mọi $H \in A$.

Xét đến Mệnh đề 9, điều này suy ra ngay từ sự kiện rằng $D_c$ là ảnh của $N_c$ qua song ánh chính tắc của $N$ lên $D$, và từ sự kiện rằng, dưới các giả thiết đã nêu, song ánh này là một đồng phôi (No. 4, Mệnh đề 8).

#### Ví dụ {#int-viii-s5-n5-exa-1 .statement}

Ta lấy $G = \mathbf{R}^n$ và lấy $\mu$ là độ đo Lebesgue; mọi giả thiết của Hệ quả của Mệnh đề 9 đều được thỏa mãn. Các nhóm con rời rạc $H$ của $G$ sao cho $G/H$ là compact chẳng gì khác ngoài các nhóm con rời rạc bậc $n$ (GT, VII, §1, No. 1, Định lý 1); một nhóm con như vậy $H$ được sinh bởi một cơ sở $(a_i)_{1 \leq i \leq n}$ của $\mathbf{R}^n$, và

$$
v(H) = |\det(a_1, \ldots, a_n)|
$$

(định thức được lấy theo cơ sở chính tắc của $\mathbf{R}^n$) (Ch. VII, §2, No. 10, Định lý 4). Không gian $D_c$ ở đây có thể được diễn giải theo cách sau: mọi nhóm con $H \in D_c$ đều là biến đổi $g \cdot \mathbf{Z}^n$ của nhóm con $\mathbf{Z}^n$ bởi một phần tử $g \in \mathbf{GL}(n, \mathbf{R})$, và nhóm con của $\mathbf{GL}(n, \mathbf{R})$ để lại $\mathbf{Z}^n$ ổn định có thể được đồng nhất với $\mathbf{GL}(n, \mathbf{Z})$. Do đó $D_c$ có thể được đồng nhất một cách chính tắc, như một không gian thuần nhất (phi tôpô), với $\mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z})$. Mặt khác, $\mathbf{GL}(n, \mathbf{R})$ tác động liên tục trên $\mathbf{R}^n$, suy ra cũng trên $\mathcal{M}_+(\mathbf{R}^n)$ đối với tôpô mơ hồ (§3, No. 3, Mệnh đề 13), suy ra trên không gian con $N_c$ của $\mathcal{M}_+(\mathbf{R}^n)$; hơn nữa, đồng phôi chính tắc (No. 4, Mệnh đề 8) của $N_c$ lên $D_c$ tương thích với các luật tác động của $\mathbf{GL}(n, \mathbf{R})$. Vì $\mathbf{GL}(n, \mathbf{R})$ là đếm được ở vô cực và $D_c$ là địa phương compact, song ánh của $\mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z})$ lên $D_c$ được định nghĩa ở trên là một *đồng phôi* (Ch. VII, App. I, Bổ đề 2). Do đó Hệ quả của Mệnh đề 9 cho một tiêu chuẩn compact trong không gian thuần nhất $\mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z})$.

### 6. Một cách diễn giải khác của tôpô của không gian các nhóm con đóng

Cho $\mathfrak{F}$ là tập hợp các tập con đóng của $G$; ta định nghĩa một *cấu trúc đều Hausdorff* trên $\mathfrak{F}$ theo cách sau: với mọi tập con compắc $K$ của $G$ và mọi lân cận $V$ của $e$ trong $G$, gọi $P(K, V)$ là tập hợp các cặp $(X, Y)$ của các phần tử của $\mathcal{F}$ sao cho cả hai điều sau đều đúng

$$
(9) \quad X \cap K \subset VY \quad \text{và} \quad Y \cap K \subset VX.
$$

Hãy chứng minh rằng tập hợp các $P(K, V)$ là một hệ cơ bản các lân cận chéo của một cấu trúc đều Hausdorff $\mathcal{U}$ trên $\mathcal{F}$. Các tiên đề $(U'_I)$ và $(U'_{II})$ của GT, II, §1, No. 1 hiển nhiên được thỏa mãn; hơn nữa, các hệ thức $K \subset K'$ và $V' \subset V$ suy ra $P(K', V') \subset P(K, V)$; để kiểm tra $(U'_{III})$, do đó ta có thể chỉ xét trường hợp $V$ là một lân cận compắc đối xứng của $e$, sao cho $VK$ là compắc. Giả sử rằng $(X, Y) \in P(VK, V)$ và $(Y, Z) \in P(VK, V)$; khi đó $X \cap K \subset X \cap VK \subset VY$, và nếu $y \in Y$ sao cho $vy \in K$ với một $v \in V$, thì tất yếu $y \in VK$, do đó

$$
X \cap K \subset V(Y \cap VK);
$$

mặt khác, $Y \cap VK \subset VZ$, suy ra $X \cap K \subset V^2Z$, và người ta chứng minh tương tự rằng $Z \cap K \subset V^2X$, điều đó chứng minh $(U'_{III})$. Cuối cùng, nếu $X, Y$ là hai phần tử phân biệt của $\mathcal{F}$, thì chẳng hạn tồn tại một điểm $a \in X$ sao cho $a \notin Y$, suy ra tồn tại một lân cận compắc đối xứng $V$ của $e$ sao cho $Va \cap Y = \varnothing$, tức là $a \notin VY$; *a fortiori* $(X, Y) \notin P(Va, V)$, và điều đó hoàn tất chứng minh mệnh đề của chúng ta.

Điều đó đã được thiết lập, ta xét trên tập $\Sigma$ các nhóm con đóng của $G$ tôpô $\mathcal{T}$ cảm sinh bởi tôpô của không gian đều $\mathcal{F}$ vừa được định nghĩa. Ta sẽ thấy tôpô này *đồng nhất với tôpô được định nghĩa trong No. 3*. Sẽ đủ để chứng minh rằng ánh xạ $\alpha \mapsto H_\alpha$ của $\Gamma$ vào $\Sigma$ là *liên tục* khi $\Sigma$ được trang bị tôpô $\mathcal{T}$: vì khi đó, điều tương tự cũng đúng với hạn chế của ánh xạ này lên $\Gamma_\varphi$ (với ký hiệu như trong No. 1, Mệnh đề 2), mà nó là song ánh; nhưng vì $\Gamma_\varphi$ là compắc và tôpô $\mathcal{T}$ là tách biệt, ánh xạ $\alpha \mapsto H_\alpha$ của $\Gamma_\varphi$ vào $\Sigma$ sẽ là một đồng phôi.

Vậy hãy cho $\alpha_0$ là một điểm của $\Gamma$ và cho $\Phi$ là một bộ lọc trên $\Gamma$ hội tụ đến $\alpha_0$; ta sẽ chứng minh rằng, đối với $\Phi$, $H_\alpha$ tiến tới $H_{\alpha_0}$ theo tôpô $\mathcal{T}$. Cho $K$ là một tập con compact của $G$, $V$ là một lân cận compact đối xứng của $e$ trong $G$; với mọi $x \in H_{\alpha_0} \cap K$, tồn tại một tập $M(x) \in \Phi$ sao cho với mọi $\alpha \in M(x)$, ta có $Vx \cap H_\alpha \neq \varnothing$ (No. 1, Bổ đề 2), do đó $Vx \subset V^2H_\alpha$; bằng cách phủ $H_{\alpha_0} \cap K$ bởi một số hữu hạn các tập $Vx_i$, ta thấy rằng nếu $M = \bigcap_i M(x_i)$ thì $H_{\alpha_0} \cap K \subset V^2H_\alpha$ với mọi $\alpha \in M$.

Ngược lại, giả sử tồn tại một lân cận mở $U$ của $e$ trong $G$ sao cho, với mọi tập $L \in \Phi$, có ít nhất một $\alpha \in L$ sao cho $H_\alpha \cap K \not\subset UH_{\alpha_0}$; nếu $\omega(L)$ là tập các $\alpha \in L$ có tính chất này, thì các $\omega(L)$ sẽ tạo thành một cơ sở của một bộ lọc $\Phi'$ trên $\Gamma$ mịn hơn $\Phi$, và, với mọi $\alpha$ thuộc hợp $E$ của các $\omega(L)$ khi $L \in \Phi$, sẽ tồn tại một t_\alpha \in H_\alpha \cap K \text{ không thuộc } UH_{\alpha_0}; \text{ với } \alpha \notin E, \text{ lấy } t_\alpha \text{ là bất kỳ điểm nào của } H_\alpha. \text{ Vì } K \cap C(UH_{\alpha_0}) \text{ là compact, sẽ tồn tại một điểm tụ } s \text{ của } \alpha \mapsto t_\alpha \text{ đối với } \Phi', \text{ thuộc } K \cap C(UH_{\alpha_0}); \text{ nhưng vì } \Phi' \text{ hội tụ đến } \alpha_0 \text{ trong } \Gamma, \text{ điều này mâu thuẫn với Bổ đề 3 của No. 1.}

Bài tập

### Bài tập {#int-viii-s5-exercises}

Xem [bài tập cho § 5](exercises/s5/).
