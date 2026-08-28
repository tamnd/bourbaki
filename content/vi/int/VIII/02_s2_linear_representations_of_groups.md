---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 2
section_title: Linear representations of groups
lang: vi
source: int-vii-ix
book_pages: INT VIII.8-INT VIII.17
pdf_pages: 0108-0117, 0159-0161
extraction: ocr
subsections:
    - "no": 1
      title: Continuous linear representations
      page: 8
      pdf_page: 108
    - "no": 2
      title: Contragredient representation
      page: 10
      pdf_page: 110
    - "no": 3
      title: 'Example: linear representations in spaces of continuous functions'
      page: 11
      pdf_page: 111
    - "no": 4
      title: 'Example: linear representations in spaces of measures'
      page: 12
      pdf_page: 112
    - "no": 5
      title: 'Example: linear representations in the spaces $L^p$'
      page: 13
      pdf_page: 113
    - "no": 6
      title: Extension of a linear representation of $G$ to the measures on $G$
      page: 15
      pdf_page: 115
    - "no": 7
      title: Relations between the endomorphisms $U(\mu)$ and the endomorphisms $U(s)$
      page: 16
      pdf_page: 116
statements: 22
exercises: 10
content_sha256: 5a935f4165ab1ebcdc6e23b783d7a08cc3102b8b9369da68d714e534ff9c8d27
translated_from: content/en/int/VIII/02_s2_linear_representations_of_groups.md
source_content_sha256: dcacb32e43faf87afa9b413eaa1d8bbbe9c968d661d131b722608dd9e997415d
translation_model: gpt-5-6-mini, gpt-5.4, gpt-5-6
translation_run: translate-vi-6cdc5c31
glossary_version: 34
glossary_terms_sha256: 6f77a6ae61cc583f50e3362f5a41b1f1d80e39034281afd9187ec71aa3b09450
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC BIỂU DIỄN TUYẾN TÍNH CỦA NHÓM

### 1. Các biểu diễn tuyến tính liên tục

Cho G là một nhóm tôpô, E là một không gian lồi địa phương, U là một biểu diễn tuyến tính của G trong E.

#### Định nghĩa 1 {#int-viii-s2-def-1 .statement}

— (i) $U$ được gọi là liên tục riêng nếu, với mọi $s \in G$, $U(s)$ là một tự đồng cấu liên tục của $E$, và nếu, với mọi $x \in E$, ánh xạ $s \mapsto U(s)x$ của $G$ vào $E$ là liên tục.

(ii) $U$ được gọi là liên tục nếu $(s, x) \mapsto U(s)x$ là một ánh xạ liên tục của $G \times E$ vào $E$.

(iii) $U$ được gọi là liên tục đều nếu nó là liên tục và nếu tập hợp các tự đồng cấu $U(s)$, trong đó $s$ chạy trên $G$, là liên tục đều.

#### Nhận xét 1 {#int-viii-s2-n1-rem-1 .statement}

Nói rằng $U$ liên tục riêng có nghĩa là $s \mapsto U(s)$ là một ánh xạ liên tục của $G$ vào không gian $\mathcal{L}(E; E)$ các tự đồng cấu liên tục của $E$, được trang bị tôpô hội tụ điểm.

#### Nhận xét 2 {#int-viii-s2-n1-rem-2 .statement}

Nói rằng $U$ liên tục tương đương với tập hợp ba điều kiện sau:

a) với mọi $s \in G$, $U(s)$ là liên tục; b) tồn tại một lân cận $V$ của $e$ sao cho $U(V)$ là liên tục đều; c) tồn tại một tập hợp toàn phần $D$ trong $E$ sao cho, với mọi $x \in D$, ánh xạ $s \mapsto U(s)x$ là liên tục.

Các điều kiện này hiển nhiên là cần thiết. Ngược lại, giả sử các điều kiện $a)$, $b)$, $c)$ được thỏa mãn. Trên $U(V)$, tôpô hội tụ điểm đồng nhất với tôpô hội tụ điểm trên $D$ (TVS, III, §3, No. 4, Prop. 5). Do đó ánh xạ $(s, x) \mapsto U(s)x$ của $V \times E$ vào $E$ là liên tục (GT, X, §2, No. 1, Cor. 3 of Prop. 1). Vì $U(s_0s)x = U(s_0)(U(s)x)$ với mọi $s_0 \in G$, $s \in G$, $x \in E$, ta thấy rằng $U$ là liên tục.

Khi $G$ là compact địa phương, các điều kiện $a)$ và $b)$ tương đương với điều kiện:
$a')$ với mọi tập con compact $K$ của $G$, $U(K)$ là liên tục đều.

#### Nhận xét 3 {#int-viii-s2-n1-rem-3 .statement}

Giả sử $U$ là một biểu diễn tuyến tính liên tục của $G$ trong $E$. Với mỗi $s \in G$, gọi $\widehat{U}(s)$ là mở rộng liên tục của $U(s)$ lên phần hoàn thành $\widehat{E}$ của $E$. Khi đó $\widehat{U}$ là một biểu diễn tuyến tính của $G$ trong $\widehat{E}$, thỏa mãn các điều kiện $a)$ và $c)$ của Nhận xét 2, và cả điều kiện $b)$ theo GT, X, §2, No. 2, Prop. 4. Vậy nên $\widehat{U}$ là một biểu diễn tuyến tính liên tục của $G$ trong $\widehat{E}$.

#### Nhận xét 4 {#int-viii-s2-n1-rem-4 .statement}

Khi $E$ là một không gian định chuẩn, người ta nói $U$ là đẳng cự nếu $\|U(s)\| = 1$ với mọi $s \in G$. Để được như vậy, chỉ cần có $\|U(s)\| \leq 1$ với mọi $s \in G$, vì khi đó ta có
$$
1 = \|1\| \leq \|U(s)\| \cdot \|U(s^{-1})\|,
$$
do đó $\|U(s)\| = \|U(s^{-1})\| = 1$ với mọi $s \in G$.

#### Mệnh đề 1 {#int-viii-s2-prop-1 .statement}

— Nếu $G$ là một nhóm địa phương compact và $E$ là tròn hóa, thì mọi biểu diễn tuyến tính riêng liên tục $U$ của $G$ trong $E$ đều liên tục.

Với mọi tập con compact $K$ của $G$, $U(K)$ là compact đối với tôpô hội tụ từng điểm (Nhận xét 1), do đó là đẳng liên tục (TVS, III, §4, No. 2, Định lý 1); khi ấy áp dụng Nhận xét 2.

#### Bổ đề 1 {#int-viii-s2-lem-1 .statement}

Cho G là một nhóm địa phương compact, $\rho$ là một hàm số hữu hạn nửa liên tục dưới $\geqslant 0$ trên G sao cho $\rho(st) \leqslant \rho(s)\rho(t)$ với mọi $s,t \in G$. Khi đó $\rho$ bị chặn trên trên mọi tập con compact của G.

Tồn tại một tập con mở khác rỗng U của G sao cho $\rho$ bị chặn trên trên U (GT, IX, §5, No. 4, Định lý 2). Cho K là một tập con compact của G. Khi đó K được phủ bởi một số hữu hạn các tập $s_1U, \ldots, s_nU$. Với mọi $x \in U$, ta có $\rho(s_ix) \leqslant \rho(s_i)\rho(x)$, do đó $\rho$ bị chặn trên trên các $s_iU$, suy ra trên K.

#### Bổ đề 2 {#int-viii-s2-lem-2 .statement}

Cho G là một nhóm tôpô, U là một biểu diễn tuyến tính của G trong một không gian định chuẩn E, và A là một tập con trù mật của E. Giả sử rằng với mọi $s \in G$, $U(s)$ là liên tục, và rằng, với mọi $x \in A$, $s \mapsto U(s)x$ là một ánh xạ liên tục từ G vào E. Khi đó hàm số $s \mapsto g(s) = \|U(s)\|$ trên G là nửa liên tục dưới và thỏa mãn $g(st) \leqslant g(s)g(t)$.

Gọi B là quả cầu đơn vị của E. Khi đó $g(s) = \sup_{x \in B \cap A} \|U(s)x\|$, và mỗi hàm số $s \mapsto \|U(s)x\|$ đều liên tục trên G, do đó $g$ là nửa liên tục dưới. Mặt khác,

$$
g(st) = \|U(s)U(t)\| \leqslant \|U(s)\| \cdot \|U(t)\| = g(s)g(t).
$$

#### Mệnh đề 2 {#int-viii-s2-prop-2 .statement}

Cho G là một nhóm địa phương compact, U là một biểu diễn tuyến tính của G trong một không gian định chuẩn E. Gọi A là một tập con trù mật của E. Giả sử rằng với mọi $s \in G$, $U(s)$ là liên tục và rằng, với mọi $x \in A$, $s \mapsto U(s)x$ là một ánh xạ liên tục từ G vào E. Khi đó U là liên tục.

Thật vậy, $\|U(s)\|$ bị chặn trên trên mọi tập con compact của G theo các Bổ đề 1 và 2, rồi khi ấy áp dụng Nhận xét 2.

### 2. Biểu diễn đối ngẫu

Cho U là một biểu diễn tuyến tính liên tục riêng của G trong E. Gọi E' là đối ngẫu của E. Ánh xạ $s \mapsto {}^tU(s)$ là một biểu diễn tuyến tính trong E' của nhóm $G^0$ đối của G; ta sẽ nói rằng biểu diễn này là chuyển vị của U. Ánh xạ $s \mapsto {}^tU(s^{-1}) = {}^tU(s)^{-1}$ là một biểu diễn tuyến tính của G trong E', được gọi là biểu diễn đối ngẫu tương phản của U.

#### Bổ đề 3 {#int-viii-s2-lem-3 .statement}

Cho X là một không gian compact địa phương, Y và Z là các không gian tôpô, $\varphi$ là một ánh xạ liên tục từ $X \times Y$ vào Z, và $\varphi_x$ là ánh xạ $y \mapsto \varphi(x,y)$ từ Y vào Z. Các không gian $\mathcal{C}(Y), \mathcal{C}(Z)$ được trang bị tôpô hội tụ compact, ánh xạ $(x,f) \mapsto f \circ \varphi_x$ từ $X \times \mathcal{C}(Z)$ vào $\mathcal{C}(Y)$ là liên tục.

Rõ ràng chỉ cần xét trường hợp X là compact. Cho $(x_0, f_0) \in X \times \mathcal{C}(Z)$, K là một tập con compact của Y, và $\varepsilon > 0$. Đặt $K' = \varphi(X \times K)$. Vì f_0 \circ \varphi \text{ là liên tục đều trong } X \times K, \text{ tồn tại một lân cận W của } x_0 \text{ sao cho } |f_0(\varphi(x,y)) - f_0(\varphi(x_0,y))| \leq \varepsilon \text{ với } x \in W \text{ và } y \in K. \text{ Mặt khác, nếu lấy } f \in \mathcal{C}(Z) \text{ sao cho } |f(z) - f_0(z)| \leq \varepsilon \text{ với mọi } z \in K', \text{ ta sẽ có } |f(\varphi(x,y)) - f_0(\varphi(x,y))| \leq \varepsilon \text{ với } x \in X, y \in K, \text{ và do đó } |f(\varphi(x,y)) - f_0(\varphi(x_0,y))| \leq 2\varepsilon \text{ với } x \in W, y \in K. \text{ Do đó có bổ đề.}

Bây giờ ta trở lại các ký hiệu trước đây.

#### Mệnh đề 3 {#int-viii-s2-prop-3 .statement}

(i) *Nếu U là liên tục riêng, thì $^tU$ là liên tục riêng khi E' được trang bị tôpô yếu $\sigma(E', E)$.*
(ii) *Nếu G là compact địa phương và U là liên tục, thì $^tU$ là liên tục khi E' được trang bị tôpô hội tụ compact.*

Mệnh đề (i) là ngay lập tức. Mệnh đề (ii) suy ra từ Bổ đề 3 trong đó đã lấy $X = G, Y = Z = E, \varphi(s, x) = U(s)x$.

### 3. Ví dụ: các biểu diễn tuyến tính trong các không gian các hàm liên tục

Cho G là một nhóm rời rạc tác động bên trái lên một tập hợp X. Một hàm phức $\chi$ trên $G \times X$ được gọi là một *nhân tử* nếu

(1) $\chi(e, x) = 1$ với mọi $x \in X;$
(2) $\chi(st, x) = \chi(s, tx)\chi(t, x)$ với mọi $s, t$ trong G, $x \in X$.

Suy ra rằng

(3) $\chi(t^{-1}, tx)\chi(t, x) = 1$ với mọi $t \in G, x \in X,$

và đặc biệt $\chi(t, x) \neq 0$ với mọi $t \in G, x \in X$.

Với mỗi hàm phức $f$ xác định trên X và mỗi $s \in G$, gọi $\gamma_\chi(s)f$ là hàm phức trên X được xác định bởi

(4) $(\gamma_\chi(s)f)(x) = \chi(s^{-1}, x)f(s^{-1}x)$.

Khi đó $\gamma_\chi(e)f = f$ và

$$
\begin{align*}
(\gamma_\chi(s)\gamma_\chi(s')f)(x) &= \chi(s^{-1}, x)(\gamma_\chi(s')f)(s^{-1}x) \\
&= \chi(s^{-1}, x)\chi(s'^{-1}, s^{-1}x)f(s'^{-1}s^{-1}x) \\
&= \chi((ss')^{-1}, x))f((ss')^{-1}x) = (\gamma_\chi(ss')f)(x),
\end{align*}
$$

do đó $\gamma_\chi$ *là một biểu diễn tuyến tính* của G. Với $\chi = 1$, ta thu được lại các tự đồng cấu $\gamma(s)$ (Ch. VII, §1, No. 1, công thức (3)).

Giả sử bây giờ rằng G và X là compact địa phương, G tác động liên tục trên X, và $\chi$ liên tục trên $G \times X$. Khi đó $C(X)$ và $K(X)$ là ổn định đối với các $\gamma_\chi(s)$, do đó có các biểu diễn tuyến tính của G trong $C(X)$ và $K(X)$ mà ta vẫn ký hiệu là $\gamma_\chi$.

#### Mệnh đề 4 {#int-viii-s2-prop-4 .statement}

*Các biểu diễn tuyến tính $\gamma_\chi$ của G trong $C(X)$ và $K(X)$ là liên tục.*

Ánh xạ $(s, f) \mapsto (s, \gamma(s)f)$ của $G \times C(X)$ vào $G \times C(X)$ là liên tục (No. 2, Bổ đề 3). Mặt khác, ánh xạ $(s, f) \mapsto \chi(s, \cdot)f$ của $G \times C(X)$ vào $C(X)$ là liên tục; vì, nếu s tiến tới $s_0$ trong G, thì $\chi(s, \cdot)$ tiến tới $\chi(s_0, \cdot)$ đều trên mọi tập con compact của X; nếu hơn nữa, $f$ tiến tới $f_0$ trong $C(X)$, thì $\chi(s, \cdot)f$ tiến tới $\chi(s_0, \cdot)f_0$ đều trên mọi tập con compact của X, do đó mệnh đề của chúng ta. Vì vậy biểu diễn $\gamma_\chi$ của G trong $C(X)$ là liên tục.

Ta hãy chứng minh rằng biểu diễn $\gamma_\chi$ của G trong $K(X)$ là liên tục. Vì $K(X)$ là giới hạn trực tiếp của các không gian Banach, nó là barreled (TVS, III, §4, No. 1, Hệ quả 3 của Mệnh đề 3), do đó chỉ cần chứng minh rằng $\gamma_\chi$ là liên tục riêng (No. 1, Mệnh đề 1). Bây giờ, cho H là một tập con compact của X và cho $s_0 \in G$. Cho V là một lân cận compact của $s_0$ trong G, và đặt L = VH, là compact trong X. Với mọi $f \in K(X, H)$, giá của $\gamma_\chi(s_0)f$ được chứa trong L, và
$$
\sup_{x \in X} |(\gamma_\chi(s_0)f)(x)| \leq \sup_{x \in L} |\chi(s_0^{-1}, x)| \cdot \sup_{x \in X} |f(x)|,
$$
do đó $f \mapsto \gamma_\chi(s_0)f$ là một ánh xạ tuyến tính liên tục của $K(X, H)$ vào $K(X, L)$; suy ra rằng $f \mapsto \gamma_\chi(s_0)f$ là một ánh xạ tuyến tính liên tục của $K(X)$ vào chính nó (TVS, II, §4, No. 4, Mệnh đề 5). Mặt khác, tôpô của $K(X, L)$ được cảm sinh bởi tôpô của $C(X)$. Theo điều đã được chứng minh, ánh xạ $s \mapsto \gamma_\chi(s)f$ của V vào $K(X, L)$ là liên tục. Điều này hoàn tất chứng minh rằng $\gamma_\chi$ là liên tục riêng.

#### Mệnh đề 5 {#int-viii-s2-prop-5 .statement}

*Giả sử rằng mỗi hàm $\chi(s, \cdot)$ là bị chặn. Khi đó $\gamma_\chi$ giữ ổn định $\overline{K(X)}$, và biểu diễn tuyến tính $\gamma_\chi$ của G trong $\overline{K(X)}$ là liên tục.*

Hiển nhiên rằng $\gamma_\chi$ giữ ổn định $\overline{K(X)}$ và mỗi ánh xạ $\gamma_\chi(s)$ là liên tục trong $\overline{K(X)}$. Mặt khác, với mọi $f \in K(X)$, $s \mapsto \gamma_\chi(s)f$ là một ánh xạ liên tục của G vào $K(X)$ và *a fortiori* vào $\overline{K(X)}$. Do đó biểu diễn $\gamma_\chi$ trong $\overline{K(X)}$ là liên tục (No. 1, Mệnh đề 2).

### 4. Ví dụ: các biểu diễn tuyến tính trong các không gian độ đo

Một lần nữa cho G là một nhóm compact địa phương, tác động liên tục bên trái trên một không gian compact địa phương X, và cho $\chi$ là một nhân tử *liên tục* trên $G \times X$. Biểu diễn tuyến tính $\gamma_\chi$ của $G$ trong $\mathcal{K}(X)$ thừa nhận một biểu diễn đối ngẫu trong $\mathcal{M}(X)$, mà ta cũng sẽ ký hiệu lại bởi $\gamma_\chi$, và được xác định bởi công thức sau (trong đó $\mu \in \mathcal{M}(X) , f \in \mathcal{K}(X)$):

$$
\langle \gamma_\chi(s)\mu, f \rangle = \langle \mu, \gamma_\chi(s^{-1})f \rangle = \langle \chi(s, \cdot) \cdot \mu, \gamma(s^{-1})f \rangle = \langle \gamma(s)(\chi(s, \cdot) \cdot \mu), f \rangle ,
$$

do đó

$$
\gamma_\chi(s)\mu = \gamma(s)(\chi(s, \cdot) \cdot \mu) = (\gamma(s)\chi(s, \cdot)) \cdot (\gamma(s)\mu) .
$$

Ta chú ý rằng

$$
(\gamma(s)\chi(s, \cdot))(x) = \chi(s, s^{-1}x) .
$$

Biểu diễn tuyến tính $\gamma_\chi$ của $G$ trong $\mathcal{C}(X)$ thừa nhận một biểu diễn đối ngẫu trong không gian $\mathcal{C}'(X)$ của các độ đo trên $X$ có giá compact, một biểu diễn mà ta cũng ký hiệu lại là $\gamma_\chi$; các tự đồng cấu $\gamma_\chi(s)$ của $\mathcal{C}'(X)$ là các hạn chế của các tự đồng cấu $\gamma_\chi(s)$ của $\mathcal{M}(X)$.

#### Mệnh đề 6 {#int-viii-s2-prop-6 .statement}

*Nếu trang bị cho $\mathcal{M}(X)$ (tương ứng $\mathcal{C}'(X)$) tôpô của sự hội tụ đều trên các tập compact của $\mathcal{K}(X)$ (tương ứng $\mathcal{C}(X)$), thì biểu diễn tuyến tính $\gamma_\chi$ của $G$ trong $\mathcal{M}(X)$ (tương ứng $\mathcal{C}'(X)$) là liên tục.*

#### Mệnh đề 7 {#int-viii-s2-prop-7 .statement}

*Giả sử rằng mỗi hàm $\chi(s, \cdot)$ là bị chặn. Khi đó $\gamma_\chi$ giữ ổn định $\mathcal{M}^1(X)$ và, nếu $\mathcal{M}^1(X)$ được trang bị tôpô của sự hội tụ đều trên các tập compact của $\mathcal{K}(X)$, thì biểu diễn tuyến tính $\gamma_\chi$ của $G$ trong $\mathcal{M}^1(X)$ là liên tục.*
Các mệnh đề này suy ra từ các Mệnh đề 3, 4, 5.

### 5. Ví dụ: các biểu diễn tuyến tính trong các không gian $L^p$

Một lần nữa cho $G$ là một nhóm compact địa phương, tác động liên tục bên trái trên một không gian compact địa phương $X$. Cho $\beta$ là một độ đo dương trên $X$ có giá $X$. Giả sử rằng tồn tại một hàm *liên tục* $\chi > 0$ trên $G \times X$ sao cho, với mọi $s \in G$,

$$
\gamma(s)\beta = \chi(s^{-1}, \cdot) \cdot \beta
$$

(điều này đặc biệt kéo theo rằng $\beta$ là bất biến gần đúng dưới $G$). *Khi đó, $\chi$ là một nhân tử.* Thật vậy, với $s, t$ trong $G$, ta có

$$
\gamma(s)\gamma(t)\beta = \gamma(s)(\chi(t^{-1}, \cdot) \cdot \beta) = (\gamma(s)\chi(t^{-1}, \cdot)) \cdot (\gamma(s)\beta)
= (\gamma(s)\chi(t^{-1}, \cdot)) \cdot \chi(s^{-1}, \cdot) \cdot \beta ,
$$
$$
\gamma(st)\beta = \chi(t^{-1}s^{-1}, \cdot) \cdot \beta ,
$$

do đó
$$
\chi(t^{-1}, s^{-1}x)\chi(s^{-1}, x) = \chi(t^{-1}s^{-1}, x)
$$
hầu khắp mọi nơi địa phương theo $\beta$, do đó ở mọi nơi, vì $\chi$ liên tục và $\beta$ có giá $X$.

Cho $p \in [1, +\infty[$. Với mọi $f \in \mathcal{L}_C^p(X, \beta)$ và mọi $s \in G$, gọi $\gamma_{\chi,p}(s)f$ là hàm trên $X$ được xác định bởi
$$
(\gamma_{\chi,p}(s)f)(x) = \chi(s^{-1}, x)^{1/p} f(s^{-1}x).
$$
Ta có
$$
\int^* |\chi(s^{-1}, x)^{1/p} f(s^{-1}x)|^p d\beta(x) = \int^* |f(s^{-1}x)|^p \chi(s^{-1}, x) d\beta(x)
$$
$$
= \int |f(x)|^p d\beta(x),
$$
do đó $\gamma_{\chi,p}(s)f \in \mathcal{L}_C^p(X, \beta)$. Ta thấy rằng $\gamma_{\chi,p}(s)$ là một tự đồng cấu *đẳng cự* của $\mathcal{L}_C^p(X, \beta)$ và xác định, bằng cách chuyển sang thương, một tự đồng cấu đẳng cự của $L_C^p(X, \beta)$, cũng được ký hiệu là $\gamma_{\chi,p}(s)$. Mặt khác, $\chi^{1/p}$ hiển nhiên là một nhân tử, do đó $\gamma_{\chi,p}$ là một biểu diễn tuyến tính của $G$ trong $L_C^p(X, \beta)$ theo điều ta đã thấy ở No. 3.

#### Mệnh đề 8 {#int-viii-s2-prop-8 .statement}

*Biểu diễn tuyến tính $\gamma_{\chi,p}$ của $G$ trong $L_C^p(X, \beta)$ là liên tục và đẳng cự.*

Cho $f \in \mathcal{K}(X)$. Khi $s$ tiến tới $s_0$ trong $G$, $\gamma_{\chi,p}(s)f$ tiến tới $\gamma_{\chi,p}(s_0)f$ trong $\mathcal{K}(X)$, do đó trong $L_C^p(X, \beta)$. Vì các $\gamma_{\chi,p}(s)$ là đẳng cự, Mệnh đề 8 thu được bằng cách áp dụng *Nhận xét 2* của No. 1.

Đối với trường hợp không giả thiết $\chi$ liên tục, xem §4, Bài tập 13.

#### Mệnh đề 9 {#int-viii-s2-prop-9 .statement}

*Giả sử rằng mỗi hàm $\chi(s, \cdot)$ đều bị chặn. Khi đó $\gamma_\chi$ để $L_C^p(X, \beta)$ ổn định, và biểu diễn tuyến tính $\gamma_\chi$ của $G$ trong $L_C^p(X, \beta)$ là liên tục.*

Cho $f \in \mathcal{L}_C^p(X, \beta)$. Khi đó
$$
\int^* |\chi(s^{-1}, x)f(s^{-1}x)|^p d\beta(x)
$$
$$
\leq \sup_{x \in X} \chi(s^{-1}, x)^{p-1} \int^* |f(s^{-1}x)|^p \chi(s^{-1}, x) d\beta(x)
$$
$$
= \sup_{x \in X} \chi(s^{-1}, x)^{p-1} \int |f(x)|^p d\beta(x),
$$
do đó $\gamma_\chi(s)f \in \mathcal{L}_C^p(X, \beta)$, và
$$
\| \gamma_\chi(s) \| \leq \sup_{x \in X} \chi(s^{-1}, x)^{1/q},
$$
(5) trong đó $q$ ký hiệu số mũ liên hợp với $p$. Nếu $f \in \mathcal{K}(X)$, thì $\gamma_{\chi}(s)f$ tiến tới $\gamma_{\chi}(s_0)f$ trong $\mathcal{K}(X)$, do đó trong $\mathcal{L}_C^p(X, \beta)$, khi $s$ tiến tới $s_0$. Vậy biểu diễn $\gamma_{\chi}$ của $G$ trong $L_C^p(X, \beta)$ là liên tục (No. 1, Mệnh đề 2).

Các tính chất tương tự như các tính chất của các Số 3, 4, 5 vẫn đúng nếu $G$ tác động ở phải trên $X$.

Đặc biệt, nếu ta coi $G$ như tác động lên chính nó bởi các phép tịnh tiến trái hoặc phải, và nếu lấy $\chi = 1$, thì ta thu được các *biểu diễn chính quy trái* và *chính quy phải* của $G$ trong $\mathcal{C}(G)$, $\mathcal{K}(G)$, $\overline{\mathcal{K}}(G)$, $\mathcal{C}'(G)$, $\mathcal{M}(G)$, $\mathcal{M}^1(G)$. Nếu lấy $\beta$ là một độ đo Haar trái (resp. phải) trên $G$, và nếu lấy $\chi = 1$, thì ta thu được *biểu diễn chính quy* *trái* (resp. *phải*) của $G$ trong $L_C^p(G, \beta)$.

### 6. Mở rộng một biểu diễn tuyến tính của $G$ tới các độ đo trên $G$

Cho $G$ là một nhóm địa phương compact, $E$ một không gian lồi địa phương, $U$ một biểu diễn tuyến tính của $G$ trong $E$. Giả sử $U$ liên tục và $E$ tựa đầy đủ. Khi đó, với mọi độ đo $\mu \in \mathcal{C}'(G)$, ta có

$$
\int_G U(s)\, d\mu(s) \in \mathcal{L}(E; E)
$$

(Ch. VI, §1, No. 7). Ta sẽ viết $U(\mu) = \int_G U(s)\, d\mu(s)$. Ta trang bị cho $\mathcal{C}'(G)$ tôpô hội tụ compact trong $\mathcal{C}(G)$. Ánh xạ $(\mu, x) \mapsto U(\mu)x$ từ $\mathcal{C}'(G) \times E$ vào $E$ là *hypoliên tục* đối với các tập con đẳng liên tục của $\mathcal{C}'(G)$ và các tập con compact của $E$; đặc biệt, ánh xạ $\mu \mapsto U(\mu)$ từ $\mathcal{C}'(G)$ vào $\mathcal{L}(E; E)$ (được trang bị tôpô hội tụ compact) là liên tục (*loc. cit.*, Prop. 16).

Để có thể áp dụng các kết quả này về sau, ta lưu ý rằng nếu $X$ là một không gian địa phương compact thì $\mathcal{C}(X)$, được trang bị tôpô hội tụ compact, là đầy đủ (GT, X, §1, No. 6, Cor. 3 of Th. 2). Mặt khác, $\mathcal{K}(X)$ là thùng, do đó đối ngẫu của nó $\mathcal{M}(X)$, được trang bị tôpô hội tụ compact trong $\mathcal{K}(X)$, là tựa đầy đủ (TVS, III, §4, No. 2, Cor. 4 of Th. 1). Dĩ nhiên, $\mathcal{K}(X)$ là đầy đủ đối với tôpô suy ra từ chuẩn của nó, do đó *đối ngẫu* của nó $\mathcal{M}^1(X)$ là tựa đầy đủ đối với tôpô hội tụ compact trong $\mathcal{K}(X)$ (*loc. cit.*).

Bây giờ giả sử $U$ là một biểu diễn tuyến tính liên tục của nhóm địa phương compact $G$ trên một *không gian Banach* $E$. Đặt $g(s) = \|U(s)\|$ với mọi $s \in G$. Khi đó, nếu $\mu$ là một độ đo trên $G$ sao cho $g$ là $\mu$-khả tích, thì ta có $\int_G U(s)\, d\mu(s) \in \mathcal{L}(E; E)$ và $\|\int_G U(s)\, d\mu(s)\| \leq \int g(s)\, d|\mu|(s)$ (Ch. VI, §1, No. 7, *Nhận xét* 1). Ta კვლავ viết $U(\mu) = \int_G U(s)\, d\mu(s)$.

### 7. Các quan hệ giữa các nội tự đồng cấu $U(\mu)$ và các nội tự đồng cấu $U(s)$

#### Bổ đề 4 {#int-viii-s2-lem-4 .statement}

Cho $T$ là một không gian compact địa phương, $a$ là một điểm của $T$, $M$ là một tập con của $\mathcal{M}(T)$, và $\mathfrak{F}$ là một bộ lọc trên $M$. Giả sử rằng:
(i) với mọi tập con compact $K$ của $T$, các số $|\mu|(K)$, với $\mu \in M$, đều bị chặn trên;
(ii) $\lim_{\mu,\mathfrak{F}} |\mu|(K) = 0$ với mọi tập con compact $K$ của $T - \{a\}$.
(iii) tồn tại một lân cận compact $V$ của $a$ trong $T$ sao cho $\lim_{\mu,\mathfrak{F}} \mu(V) = 1$.

Khi đó bộ lọc $\mathfrak{F}$ hội tụ tới $\varepsilon_a$ trong $\mathcal{M}(T)$ được trang bị tôpô hội tụ compact trên $\mathcal{H}(T)$.

Theo giả thiết (i), $M$ là một tập con đồng liên tục của $\mathcal{M}(T)$ vì nó bị chặn mơ hồ và $\mathcal{H}(T)$ là thùng (TVS, III, §4, No. 2, Định lý 1). Do đó chỉ cần (GT, X, §2, No. 4, Định lý 1) chứng minh rằng nếu $f \in \mathcal{H}(T)$, thì $\lim_{\mu,\mathfrak{F}} \mu(f) = f(a)$. Gọi $K$ là hợp của $V$ và giá của $f$; nếu $K'$ là bao đóng của $K - V$, ta có

$$
|\mu(K) - \mu(V)| = |\mu(K - V)| \leq |\mu|(K');
$$

vì $K'$ là compact và không chứa $a$, từ đó suy ra $\lim_{\mu,\mathfrak{F}} \mu(K) = 1$. Cho $\varepsilon > 0$, và gọi $W$ là một lân cận mở của $a$ trong $K$ sao cho $|f(t) - f(a)| \leq \varepsilon$ với $t \in W$; ta có thể viết

$$
\mu(f) - f(a) = f(a)(\mu(K) - 1) + \int_K (f(t) - f(a)) d\mu(t);
$$

tích phân trên $K$ có thể được viết thành tổng của các tích phân tương tự trên $W$ và $K - W$; nếu $C = \sup |f|$, do đó ta có

$$
|\mu(f) - f(a)| \leq C|\mu(K) - 1| + \varepsilon \cdot |\mu|(K) + 2C \cdot |\mu|(K - W).
$$

Vì số hạng thứ nhất và thứ ba ở vế phải tiến tới 0 đối với $\mathfrak{F}$, ta thấy rằng thật vậy $\lim_{\mu,\mathfrak{F}} \mu(f) = f(a)$.

#### Hệ quả 1 {#int-viii-s2-lem-4-cor-1 .statement}

Với các giả thiết như trong Bổ đề 4, giả sử thêm rằng tồn tại một tập con compact $K_0$ của $T$ chứa các giá của mọi độ đo $\mu \in M$. Khi đó $\mathfrak{F}$ cũng hội tụ tới $\varepsilon_a$ trong $\mathcal{C}'(T)$ được trang bị tôpô hội tụ compact trên $\mathcal{C}(T)$.

Thật vậy, ánh xạ hạn chế từ $\mathcal{C}(T)$ vào $\mathcal{C}(K_0)$ là liên tục; do đó, nếu $H$ là một tập con compắc của $\mathcal{C}(T)$, thì các hạn chế trên $K_0$ của các hàm trong $H$ tạo thành một tập con compắc của $\mathcal{C}(K_0)$. Khi đó chỉ cần áp dụng Bổ đề 4 sau khi thay thế $T$ bằng $K_0$.

#### Hệ quả 2 {#int-viii-s2-lem-4-cor-2 .statement}

*Với các giả thiết như trong Hệ quả 1, cho $f$ là một ánh xạ liên tục từ $T$ vào một không gian lồi địa phương tựa-đầy đủ $E$. Khi đó*

$$
\lim_{\mu,\mathfrak{T}} \int f(t)\, d\mu(t) = f(a).
$$

Điều này suy ra từ Hệ quả 1, và Mệnh đề 14 của Ch. VI, §1, No. 6.

#### Hệ quả 3 {#int-viii-s2-lem-4-cor-3 .statement}

*Cho $G$ là một nhóm địa phương compắc, $E$ một không gian lồi địa phương tựa-đầy đủ, và $U$ một biểu diễn tuyến tính liên tục của $G$ trong $E$. Cho $\beta$ là một độ đo dương trên $G$, $a$ một phần tử của $G$, và $\mathcal{B}$ một cơ sở của bộ lọc các lân cận của $a$, gồm các lân cận compắc. Với mọi $V \in \mathcal{B}$, cho $f_V$ là một hàm liên tục $\geqslant 0$ trên $G$, có giá được chứa trong $V$, và sao cho $\int f_V\, d\beta = 1$. Khi đó, với mọi $x \in E$,

$$
U(a)x = \lim_V U(f_V \cdot \beta)x,
$$

*giới hạn được lấy đối với bộ lọc tiết diện của $\mathcal{B}$.*

Ánh xạ $s \mapsto U(s)x$ từ $G$ vào $E$ là liên tục. Theo Hệ quả 2, $U(a)x = \lim_V \int (U(s)x) \cdot f_V(s)\, d\beta(s)$ đối với bộ lọc tiết diện của $\mathcal{B}$, nghĩa là, $U(a)x = \lim_V U(f_V \cdot \beta)x$.

#### Mệnh đề 10 {#int-viii-s2-prop-10 .statement}

*Cho $G$ là một nhóm địa phương compắc, $E$ một không gian lồi địa phương tựa-đầy đủ, $U$ một biểu diễn tuyến tính liên tục của $G$ trong $E$, và $\beta$ một độ đo dương trên $G$ có giá là $G$.

(i) Các vectơ $U(f \cdot \beta)x$, trong đó $f$ chạy qua $\mathcal{K}(G)$ và $x$ chạy qua $E$, là trù mật trong $E$.

(ii) *Cho $F$ là một không gian con tuyến tính đóng của $E$. Nếu $F$ ổn định đối với $U$, thì $U(\mu)(F) \subset F$ với mọi $\mu \in \mathcal{C}'(G)$. Ngược lại, nếu $U(f \cdot \beta) \subset F$ với mọi $f \in \mathcal{K}(G)$, thì $F$ ổn định đối với $U$.*

Phần thứ nhất của (ii) là ngay lập tức, vì các hạn chế của các $U(s)$ lên $F$ ($s \in G$) xác định một biểu diễn tuyến tính liên tục của $G$ trong không gian lồi địa phương quasi-đầy đủ $F$. Phần thứ hai của (ii), và (i), suy ra từ Hệ quả 3 của Bổ đề 4.

### Bài tập {#int-viii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
