---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 1
section_title: Semi-norms
lang: vi
source: evt-i-v
pdf_pages: 0038-0044
extraction: ocr
subsections:
    - "no": 1
      title: Definition of semi-norms
      page: 0
      pdf_page: 38
    - "no": 2
      title: Topologies defined by semi-norms
      page: 2
      pdf_page: 39
    - "no": 3
      title: Semi-norms in quotient spaces and in product spaces
      page: 4
      pdf_page: 41
    - "no": 4
      title: Equicontinuity criteria of multilinear mappings for topologies defined by semi-norms
      page: 5
      pdf_page: 42
statements: 15
exercises: 0
content_sha256: 8493bdc4159252db6d4a81e1fc3b9dffdec35b473cedbc72d2ef667c110541a0
translated_from: content/en/evt/II/01_s1_semi_norms.md
source_content_sha256: d28b60958840fb6479c20b64e3b06c944a5472a72ea0c800ef6c6b129ef104b1
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4
translation_run: translate-vi-c37b3e9e
glossary_version: 34
glossary_terms_sha256: 8f1f932251d67382d708584c484880a119ed8355447b4e40c2116ab41b26d0b9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. CHUẨN NỬA

Trong suốt đoạn này, $\mathbf{K}$ ký hiệu một vành chia có giá trị không rời rạc.

### 1. Định nghĩa về các chuẩn nửa

#### Định nghĩa 1 {#evt-ii-s1-def-1 .statement}

Cho E là một không gian vectơ trái trên $\mathbf{K}$. Một ánh xạ $p$ của E vào $\mathbf{R}_+ = \{ 0, + \infty \}$, được gọi là một chuẩn nửa trên E nếu nó thỏa mãn các tiên đề sau :
(SN_I) Nếu $x \in \mathrm{E}$ và $\lambda \in \mathbf{K}$ thì $p(\lambda x) = |\lambda| \, p(x)$.
(SN_II) Nếu $x \in \mathrm{E}$ và $y \in \mathrm{E}$ thì $p(x + y) \leq p(x) + p(y)$.

Vì $p(x) \leq p(y) + p(x - y)$ và $p(y) \leq p(x) + p(y - x)$, từ $p(y - x) = p(x - y)$, ta suy ra
$$
|p(x) - p(y)| \leq p(x - y) .
$$

#### Ví dụ 1 {#evt-ii-s1-n1-exa-1 .statement}

Một chuẩn trên E là một bán chuẩn $p$ sao cho quan hệ $p(x) = 0$ kéo theo $x = 0$ (I, p. 3).

#### Ví dụ 2 {#evt-ii-s1-n1-exa-2 .statement}

Đối với mọi dạng tuyến tính $f$ trên E, hàm $x \mapsto |f(x)|$ là một bán chuẩn trên E.

#### Ví dụ 3 {#evt-ii-s1-n1-exa-3 .statement}

Nếu $p_i (1 \leq i \leq n)$ là một tập hợp hữu hạn các bán chuẩn trên E, thì rõ ràng $p'(x) = \sup_{1 \leq i \leq n} p_i(x)$
và $p''(x) = \sum_{i=1}^n \alpha_i p_i(x)$ (trong đó các $\alpha_i$ là $\geq 0$) đều là các bán chuẩn trên E.

Một ánh xạ $p$ của E vào $\mathbf{R}_+$ được gọi là một *bán chuẩn siêu* nếu nó thỏa mãn (SN$_I$) và tiên đề sau :

(SN$_{II}'$) *Nếu $x \in E$ và $y \in E$, thì $p(x + y) \leq \sup(p(x), p(y))$.*

Rõ ràng một siêu nửa-chuẩn là một nửa-chuẩn.

Nói rằng giá trị tuyệt đối trên K là *siêu mêtric* (CA, VI, § 6.2) có nghĩa là nó là một siêu nửa-chuẩn trên không gian vectơ trái $K_s$, không đồng nhất bằng không.

#### Mệnh đề 1 {#evt-ii-s1-prop-1 .statement}

*Cho E là một không gian vectơ tôpô trái trên K và p là một nửa-chuẩn trên E. Các điều kiện sau là tương đương :*
  *a)* *p liên tục trên E.*
  *b)* *p liên tục tại điểm 0.*
  *c)* *p liên tục đều.*
  *d)* *Với mỗi số thực $\alpha > 0$, tập W(p, $\alpha$), gồm các $x \in E$ sao cho $p(x) < \alpha$, là mở trong E.*
  *e)* *Tồn tại một số thực $\alpha > 0$ sao cho W(p, $\alpha$) là một lân cận của 0 trong E.*
  *f)* *Với mọi số thực $\alpha > 0$, tập V(p, $\alpha$), gồm các $x \in E$ sao cho $p(x) \leq \alpha$, là một lân cận của 0 trong E.*

Thật vậy, các hàm ý c) $\Rightarrow$ a) $\Rightarrow$ b) $\Rightarrow$ d) $\Rightarrow$ e) $\Rightarrow$ f) $\Rightarrow$ c) suy ra ngay lập tức từ (SN$_I$) và bất đẳng thức (1).

#### Hệ quả {#evt-ii-s1-n1-cor-1 .statement}

*Nếu p là một nửa chuẩn liên tục trên E và q là một nửa chuẩn sao cho $q \leq p$, thì q liên tục trên E.*

Khi p là một *nửa chuẩn siêu* trên E, thì các tập hợp W(p, $\alpha$) và V(p, $\alpha$) *đều vừa mở vừa đóng*. Thật vậy, ta đã thấy rằng W(p, $\alpha$) là mở; mặt khác nếu z là một điểm tụ của W(p, $\alpha$), thì tồn tại $y \in W(p, \alpha)$ sao cho $p(y - z) < \alpha$, và từ (SN$_{II}'$) ta có $p(z) < \alpha$, do đó W(p, $\alpha$) là đóng. Ngoài ra, V(p, $\alpha$) là đóng vì p liên tục; hơn nữa nếu $p(x) \leq \alpha$ và $p(y) \leq \alpha$, thì $p(x + y) \leq \alpha$ theo (SN$_{II}'$), và điều này cho thấy rằng V(p, $\alpha$) là mở.

### 2. Các tôpô được xác định bởi các nửa chuẩn

Cho p là một nửa chuẩn trên không gian vectơ E trên K; với mọi $\alpha > 0$ đặt V(p, $\alpha$) là tập con gồm những x của E sao cho $p(x) \leq \alpha$. Rõ ràng, nếu $x \in V(p, \alpha)$ và $\lambda \in K$ sao cho $|\lambda| \leq 1$, thì $\lambda x \in V(p, \alpha)$, nói cách khác V(p, $\alpha$) là *cân bằng*. Hơn nữa, với mọi $x_0 \in E$, tồn tại một vô hướng khác không $\mu \in K$ sao cho $|\mu| \geq p(x_0) \alpha^{-1}$, do đó $\mu^{-1} x_0 \in V(p, \alpha)$, nghĩa là V(p, $\alpha$) là *hấp thụ*. Cuối cùng, từ (SN$_{II}$), ta có $V(p, \alpha/2) + V(p, \alpha/2) \subset V(p, \alpha)$, và từ (SN$_I$) suy ra rằng với mọi vô hướng khác không $\lambda$ trong K ta có $\lambda V(p, \alpha) = V(p, |\lambda| \alpha)$. Từ những nhận xét này, theo I, p. 7, mệnh đề 4, ta kết luận rằng, khi $\alpha$ biến thiên trong tập hợp các số $> 0$ (hoặc chỉ trong một dãy các số dương ngặt tiến tới 0) thì các tập hợp V(p, $\alpha$) tạo thành một hệ cơ bản các lân cận của 0 đối với một tôpô tương thích với cấu trúc không gian vectơ của E; ta nói rằng tôpô này được *xác định bởi nửa chuẩn p*. Một không gian vectơ E với một tôpô như thế được gọi là một *không gian nửa chuẩn*. Chú ý rằng nếu W(p, $\alpha$) là tập con gồm những x của E sao cho $p(x) < \alpha$, thì các W(p, $\alpha$) tạo thành (khi $\alpha > 0$, hoặc khi $\alpha$ biến thiên trong một dãy dương ngặt các số tiến tới không) một hệ cơ bản các lân cận của 0 đối với tôpô được xác định bởi $p$.

Nếu $\Gamma$ là một tập hợp các nửa chuẩn trên $E$, thì *cận trên* của các tôpô được xác định bởi các nửa chuẩn $p \in \Gamma$ là tương thích với cấu trúc không gian vectơ (I, p. 10, hệ quả 4). Một hệ cơ bản các lân cận của 0, đối với tôpô này, được cho bởi các giao hữu hạn $\bigcap_i V(p_i, \alpha_i)$ trong đó $p_i \in \Gamma$ và $\alpha_i > 0$. Tôpô này được gọi là *được xác định bởi tập hợp các nửa chuẩn* $\Gamma$. Đó là tôpô *thô nhất* trên $E$ trong số các tôpô bất biến dưới mọi phép tịnh tiến và đối với chúng các nửa chuẩn $p \in \Gamma$ là liên tục.

Cho $E$ là một không gian vectơ tôpô trên $K$: một hệ các nửa chuẩn trên $E$, chẳng hạn $\Gamma$, được gọi là một *hệ cơ bản các nửa chuẩn* nếu tôpô trên $E$ trùng với tôpô được xác định bởi $\Gamma$.

Cho $E$ là một không gian vectơ trên $K$, với tôpô được xác định bởi một tập hợp các nửa chuẩn $\Gamma$. Với mọi nửa chuẩn $p$, ta có $p(x - z) \leq p(x - y) + p(y - z)$, điều này cho thấy hàm $(x, y) \mapsto p(x - y)$ là một *giả mêtric* trên $E$ (GT, IX, § 1.1): từ các định nghĩa suy ra rằng, khi $p$ biến thiên trong $\Gamma$, tập hợp các giả mêtric này xác định cấu trúc đều của không gian vectơ tôpô $E$.

#### Nhận xét {#evt-ii-s1-n2-rem-1 .statement}

— 1) Tôpô được xác định bởi một tập hợp *hữu hạn* các nửa chuẩn $p_i$ ($1 \leq i \leq n$) trên $E$, có thể được xác định bởi nửa chuẩn *duy nhất* $p = \sup_{1 \leq i \leq n} p_i$. Nhưng một tôpô được xác định bởi một tập hợp vô hạn các nửa chuẩn nói chung không thể được xác định bởi một nửa chuẩn duy nhất (III, p. 37, exerc. 2).

2) Cho $(\mathcal{T}_i)_{i \in I}$ là một họ các tôpô trên một không gian vectơ $E$ trên $K$, mỗi tôpô được xác định bởi một họ nửa chuẩn $\Gamma_i$. Khi đó tôpô được xác định bởi tập các nửa chuẩn $\Gamma = \bigcup_{i \in I} \Gamma_i$ là cận trên của các tôpô $\mathcal{T}_i$.

3) Nếu $\Gamma_0$ là một tập hợp các nửa chuẩn *có hướng bởi* quan hệ thứ tự *tăng* được xác định giữa hai nửa chuẩn $p, q$ trên $E$ bởi « tồn tại $\lambda > 0$ sao cho $p \leq \lambda q$ », thì một hệ cơ bản các lân cận của 0, đối với tôpô xác định bởi $\Gamma_0$, thu được bằng cách lấy các tập hợp $V(p, \alpha)$ trong đó $p \in \Gamma_0$ và $\alpha > 0$. Nếu $\Gamma$ là một tập hợp bất kỳ các nửa chuẩn trên $E$, thì một tập hợp lọc các nửa chuẩn, xác định cùng một tôpô như $\Gamma$, là tập hợp $\Gamma_0$ gồm các bao trên của mọi họ hữu hạn các nửa chuẩn thuộc $\Gamma$.

4) Ngay cả khi $K = \mathbf{R}$, tôpô của một không gian vectơ tôpô trên $K$ cũng không phải lúc nào cũng có thể được xác định bởi một tập hợp các nửa chuẩn (*xem* II, p. 24, hệ quả).

#### Ví dụ {#evt-ii-s1-n2-exa-1 .statement}

— Cho $\mathscr{C}^\infty(\mathbf{R})$ là không gian vectơ trên $\mathbf{R}$ gồm các hàm nhận giá trị thực và khả vi vô hạn trên $\mathbf{R}$. Với mọi hàm và mọi cặp số nguyên $n \geq 0$, $m \geq 1$, đặt

$$
p_{n,m}(f) = \sup_{-m \leq t \leq m} |f^{(n)}(t)|
$$

với $f^{(0)} = f$. Hiển nhiên các $p_{n,m}$ là các nửa chuẩn trên $\mathscr{C}^\infty(\mathbf{R})$. Để các hàm $f_\alpha$ tiến tới 0 (theo một bộ lọc $\mathfrak{F}$ trên tập hợp các chỉ số) trong $\mathscr{C}^\infty(\mathbf{R})$ đối với tôpô $\mathcal{T}$ được xác định bởi các nửa chuẩn $p_{n,m}$, điều kiện cần và đủ là với mọi số nguyên $n \geq 0$, các hàm $f_\alpha^{(n)}$ tiến tới 0 (theo $\mathfrak{F}$) *đều trên mọi tập con compắc của* $\mathbf{R}$. Ta nói rằng $\mathcal{T}$ là *tôpô hội tụ compắc đối với các hàm* $f \in \mathscr{C}^\infty(\mathbf{R})$ *và mọi đạo hàm của chúng* (*xem* III, p. 9).

#### Mệnh đề 2 {#evt-ii-s1-prop-2 .statement}

*Trên một không gian vectơ* $E$, *cho* $\mathcal{T}$ *là tôpô được xác định bởi một tập hợp các nửa chuẩn* $\Gamma$.

(i) *Bao đóng của {0} trong E, đối với* $\mathcal{T}$, *là tập con các* $x \in E$ *mà đối với chúng* $p(x) = 0$ *với mọi nửa chuẩn* $p \in \Gamma$.*

(ii) *Nếu* $\mathcal{T}$ *là Hausdorff và* $\Gamma$ *là đếm được, thì* $\mathcal{T}$ *là khả metrizable.*

Mệnh đề này suy ra ngay lập tức từ các định nghĩa và từ GT, IX, § 2 . 4, hệ quả 1.

Chú ý rằng nếu $\mathcal{T}$ là khả metrizable, thì có thể $\mathcal{T}$ không thể được xác định bởi một chuẩn duy nhất; đó là trường hợp trong ví dụ đã cho ở trên (*xem.* IV, p. 18, *Ví dụ 4*).

Cho E là một không gian vectơ trên K, với tôpô được xác định bởi một tập các nửa chuẩn $\Gamma$. Gọi $\hat{E}$ là bổ sung Hausdorff của E (I, p. 6), và $\hat{\Gamma}$ là tập các ánh xạ $\hat{p}$ từ $\hat{E}$ vào $\mathbf{R}_+$ khi $p$ chạy trong $\Gamma$ (GT, II, § 3 . 7, mệnh đề 15). Theo nguyên lý mở rộng các bất đẳng thức, các hàm $\hat{p} \in \hat{\Gamma}$ là các nửa chuẩn trên $\hat{E}$, và các hàm $\hat{p}(x - y)$ tạo thành một tập các giả khoảng cách xác định cấu trúc đều của $\hat{E}$ (GT, IX, § 1 . 3, mệnh đề 1). Do đó, ta thấy rằng $\hat{\Gamma}$ là một tập cơ bản các nửa chuẩn xác định tôpô của $\hat{E}$.

### 3. Nửa chuẩn trong các không gian thương và trong các không gian tích

Cho E là một không gian vectơ tôpô trên K, mà tôpô của nó được định nghĩa bởi $\Gamma$, một tập hợp các nửa chuẩn. Rõ ràng, các hạn chế của các nửa chuẩn của $\Gamma$ lên một không gian con vectơ M của E xác định tôpô cảm sinh trên M bởi tôpô của E.

Cho $\phi$ là ánh xạ chính tắc từ E lên không gian thương vectơ E/M. Ta chứng minh rằng, với mọi nửa chuẩn $p$ trên E, hàm

$$
\dot{p}(z) = \inf_{\phi(x) = z} p(x)
$$

là một nửa chuẩn trên E/M. Thật vậy, rõ ràng là $\dot{p}$ thỏa mãn điều kiện (SN$_1$); mặt khác, nếu $z', z''$ là hai vectơ của E/M, ta có:

$$
\begin{align*}
\inf_{\phi(x) = z' + z''} p(x) &\leq \inf_{\phi(x') = z', \phi(x'') = z''} p(x' + x'') \\
&\leq \inf_{\phi(x') = z', \phi(x'') = z''} (p(x') + p(x'')) \\
&= \inf_{\phi(x') = z'} p(x') + \inf_{\phi(x'') = z''} p(x'')
\end{align*}
$$

điều này cho thấy $\dot{p}$ thỏa mãn (SN$_2$). Ta nói rằng $\dot{p}$ là *nửa chuẩn thương* của $p$ theo M.

Lập luận tương tự chứng minh rằng, nếu $p$ là một *siêu nửa chuẩn*, thì $\dot{p}$ cũng vậy.

Như vậy, ta có (theo ký hiệu của No. 2)

$$
\phi(\mathrm{W}(p, \alpha)) = \mathrm{W}(\dot{p}, \alpha)
$$

với mọi $\alpha > 0$. Thật vậy, nói rằng $\dot{p}(z) < \alpha$ có nghĩa là tồn tại $x \in E$ sao cho $\phi(x) = z$ và $p(x) < \alpha$, từ đó suy ra quan hệ (4).

Từ đó, ta suy ra rằng, nếu tập hợp các nửa chuẩn $\Gamma$ là *có hướng* (II, p. 3, *Nhận xét 3*), thì tôpô thương trên $E/M$ được xác định bởi tập hợp các nửa chuẩn $\dot{p}$, khi $p$ chạy trong $\Gamma$.

Nếu $N$ là bao đóng của $\{0\}$ trong $E$, tôpô của $E/N$ được xác định bởi các nửa chuẩn thương $\dot{p}$, trong đó $p$ chạy trong $\Gamma$ (ngay cả khi $\Gamma$ không được lọc): ở đây $\dot{p}(\dot{x}) = p(x)$ với mọi $x$ thuộc lớp $\dot{x} \mod N$. Chú ý rằng $E/N$ không gì khác hơn là không gian Hausdorff liên kết với $E$ (I, p. 4).

Cho $E$ là một không gian vectơ trên $K$ và $(E_i)_{i \in I}$ là một họ các không gian vectơ trên $K$, trong đó $E_i$ được trang bị tôpô $\mathcal{T}_i$ xác định bởi một tập hợp các nửa chuẩn $\Gamma_i$. Với mỗi $i \in I$, gọi $f_i$ là một ánh xạ tuyến tính từ $E$ vào $E_i$; rõ ràng khi $p_i$ biến thiên trong tập hợp $\Gamma_i$, thì các $p_i \circ f_i$ tạo thành một tập hợp $\Gamma'_i$ các nửa chuẩn trên $E$. Khi đó tôpô $\mathcal{T}$ trên $E$, được định nghĩa là tôpô thô nhất trong tất cả các tôpô làm cho mọi ánh xạ $f_i$ đều liên tục (I, p. 9), được xác định bởi tập hợp các nửa chuẩn $\Gamma' = \bigcup_{i \in I} \Gamma'_i$; điều này suy ra từ định nghĩa của các lân cận của 0 đối với $\mathcal{T}$ (GT, I, § 2.3, mệnh đề 4).

Nếu các $p_i$ là các chuẩn nửa siêu, thì các $p_i \circ f_i$ cũng vậy.

Cho $E$ là một không gian vectơ trên $K$, với tôpô $\mathcal{T}$ được xác định bởi một họ các nửa chuẩn $(p_i)_{i \in I}$; với mỗi $i \in I$, gọi $\mathcal{T}_i$ là tôpô được xác định bởi nửa chuẩn duy nhất $p_i$, và ký hiệu bởi $E_i$ không gian thu được từ $E$ khi dùng tôpô $\mathcal{T}_i$. Khi đó tôpô $\mathcal{T}$ là ảnh ngược bởi ánh xạ đường chéo $\Delta : E \to \prod_{i \in I} E_i$ của tôpô tích trên $\prod_{i \in I} E_i$ (I, p. 9, prop. 7). Với mỗi $i \in I$, đặt $N_i$ là bao đóng của $\{0\}$ trong $E_i$, và gọi $F_i = E_i / N_i$ là không gian *định chuẩn* được xác định bởi chuẩn $p_i$ tương ứng với $p_i$ (II, p. 4, công thức (3)); nếu $\phi_i : E_i \to F_i$ là ánh xạ chính tắc và $\phi : (x_i) \mapsto (\phi_i(x_i))$ là ánh xạ tích, ta biết rằng tôpô tích trên $\prod_{i \in I} E_i$ là ảnh ngược bởi $\phi$ của tôpô tích trên $\prod_{i \in I} F_i$ (GT, II, § 3.9, prop. 18). Vậy tôpô $\mathcal{T}$ là ảnh ngược qua ánh xạ hợp thành $\phi \circ \Delta$ của tôpô tích trên $\prod_{i \in I} F_i$. Đặc biệt, nếu $\mathcal{T}$ là *Hausdorff* thì từ II, p. 3, prop. 2 suy ra rằng ánh xạ $\phi \circ \Delta$ là *đơn ánh*, do đó:

#### Mệnh đề 3 {#evt-ii-s1-prop-3 .statement}

*Mọi không gian vectơ tôpô Hausdorff* $E$ *trên* $K$, *mà tôpô của nó được xác định bởi một tập hợp các nửa chuẩn, đều đẳng cấu với một không gian con của một tích các không gian Banach*.

Hơn nữa, nếu tôpô của $E$ được xác định bởi một tập hợp *đếm được* các nửa chuẩn, thì $E$ là *mêtric hóa được* (I, p. 16).

### 4. Các tiêu chuẩn đồng liên tục của các ánh xạ đa tuyến tính đối với các tôpô được xác định bởi các nửa chuẩn

#### Mệnh đề 4 {#evt-ii-s1-prop-4 .statement}

*Cho* $E_i$ ($1 \leq i \leq n$) *và* $F$ *là các không gian vectơ tôpô trên* $K$; *giả sử rằng, với mọi* $i$, *tôpô của* $E_i$ *được xác định bởi một tập có hướng các nửa chuẩn* $\Gamma_i$, *và tôpô của* $F$ *được xác định bởi một tập hợp các nửa chuẩn* $\Gamma$. *Khi đó một tập hợp* $H$, *gồm các* ánh xạ đa tuyến tính của $\prod_{i=1}^n E_i$ vào F là đồng liên tục nếu, và chỉ nếu, với mỗi nửa chuẩn $q \in \Gamma$, và mỗi chỉ số i, tồn tại một nửa chuẩn $p_i \in \Gamma_i$, và một số $a > 0$, sao cho với mỗi hàm $u \in \mathbf{H}$ và điểm $(x_i) \in \prod_{i=1}^n E_i$,

$$
q(u(x_1, x_2, ..., x_n)) \leq a \cdot p_1(x_1)\ p_2(x_2) ... p_n(x_n) .
$$

Điều kiện này là đủ vì nó suy ra rằng H là đồng liên tục tại (0, 0, ..., 0) và do đó ở mọi nơi (I, p. 9, mệnh đề 6).

Ta chỉ ra rằng điều kiện là cần thiết. Theo giả thiết, với mọi nửa chuẩn $q \in \Gamma$ và mọi số $\beta > 0$, ta có $q(u(x_1, x_2, ..., x_n)) \leq \beta$ đối với mọi hàm $u \in \mathbf{H}$, miễn là $p_i(x_i) \leq \alpha_i$ đúng với mỗi chỉ số $i$, $1 \leq i \leq n$, và với những số $\alpha_i > 0$ và các nửa chuẩn $p_i \in \Gamma_i$ được chọn thích hợp nào đó. Vì K là không rời rạc, ta cũng có thể giả sử rằng, với mọi $i$, ta có $\alpha_i = |\lambda_i| < 1$ trong đó $\lambda_i \in \mathbf{K}$. Bây giờ lấy $(x_1, x_2, ..., x_n)$ là một điểm bất kỳ của $\prod_{i=1}^n E_i$, và với mỗi chỉ số $i$, lấy $m_i \in \mathbf{Z}$ là một số nguyên sao cho $p_i(x_i) \leq |\lambda_i|^{m_i + 1}$; điều này có thể viết thành $p_i(\lambda_i^{-m_i} x_i) \leq |\lambda_i|$ ($1 \leq i \leq n$), do đó, theo giả thiết, ta có

$$
q(u(x_1, x_2, ..., x_n)) \leq \beta |\lambda_1|^{m_1} |\lambda_2|^{m_2} ... |\lambda_n|^{m_n} .
$$

Trước hết giả sử rằng một trong các $p_i(x_i)$ bằng không, khi đó ta có thể lấy $m_i \in \mathbf{N}$ tùy ý lớn, do đó $q(u(x_1, x_2, ..., x_n)) = 0$. Nếu, trái lại, tất cả các $p_i(x_i)$ đều $\neq 0$, hãy lấy số nguyên $m_i$ sao cho $|\lambda_i|^{m_i + 2} < p_i(x_i) \leq |\lambda_i|^{m_i + 1}$ với mỗi $i$; khi đó ta có $|\lambda_i|^{m_i} < |\lambda_i|^{-2} p_i(x_i)$, từ đó, theo (6), suy ra quan hệ (5) với

$$
a = \beta (|\lambda_1| \cdot |\lambda_2| ... |\lambda_n|)^{-2} .
$$

Điều phải chứng minh.

#### Hệ quả {#evt-ii-s1-n4-cor-1 .statement}

— *Tập hợp H là đồng liên tục khi và chỉ khi, với mọi nửa chuẩn $q \in \Gamma$, tồn tại một lân cận của 0 trong $\prod_{i=1}^n E_i$, trong đó các hàm $q \circ u$, với $u \in \mathbf{H}$, được chặn đều.*

Điều kiện đó hiển nhiên là cần thiết, và chứng minh của mệnh đề 4 cho thấy rằng nó kéo theo một bất đẳng thức dạng (5) với mọi $u \in \mathbf{H}$, và do đó tính đẳng liên tục của H.

Chúng tôi phát biểu tường minh trường hợp riêng của mệnh đề 4 đối với các ánh xạ tuyến tính.

#### Mệnh đề 5 {#evt-ii-s1-prop-5 .statement}

— *Cho E, F là hai không gian vectơ tôpô trên một thể có định giá không rời rạc K; giả sử rằng tôpô của E (tương ứng của F) được xác định bởi một tập hợp các nửa chuẩn $\Gamma$ (tương ứng $\Gamma'$). Cho H là một tập hợp các ánh xạ tuyến tính từ E vào F. Các điều kiện sau là tương đương :*
    a) H là đẳng liên tục.

b) Với mọi nửa chuẩn $q \in \Gamma'$, tồn tại một họ hữu hạn $(p_i)_{1 \leq i \leq n}$ các nửa chuẩn thuộc $\Gamma$ và một số $a > 0$ sao cho, với mọi $x \in E$ và mọi $u \in H$,

$$
q(u(x)) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x) .
$$

c) Với mọi nửa chuẩn $q \in \Gamma'$, ánh xạ $\sup_{u \in H} (q \circ u)$ là một nửa chuẩn liên tục trên $E$.

#### Hệ quả 1 {#evt-ii-s1-prop-5-cor-1 .statement}

— Giả sử rằng $\mathcal{T}, \mathcal{T}'$ là hai tôpô trên một không gian vectơ $E$ trên $K$ được xác định, theo thứ tự, bởi hai tập hợp chuẩn nửa $\Gamma$ và $\Gamma'$. $\mathcal{T}$ mịn hơn $\mathcal{T}'$ nếu, và chỉ nếu, với mọi chuẩn nửa $q \in \Gamma'$, tồn tại một họ hữu hạn $(p_i)_{1 \leq i \leq n}$ các chuẩn nửa thuộc $\Gamma$ và một số $a > 0$ sao cho, với mọi $x \in E$, ta có $q(x) \leq a \cdot \sup_{1 \leq i \leq n} p_i(x)$.

Thực vậy điều này cho thấy rằng ánh xạ đồng nhất của $E$ với tôpô $\mathcal{T}$, vào $E$ với tôpô $\mathcal{T}'$, là liên tục.

#### Hệ quả 2 {#evt-ii-s1-prop-5-cor-2 .statement}

— Giả sử rằng tôpô $\mathcal{T}$ của một không gian vectơ tôpô $E$ trên $K$ được xác định bởi một tập có hướng các nửa chuẩn $\Gamma$; với mỗi nửa chuẩn $p \in \Gamma$, gọi $E_p$ là không gian thu được từ $E$ khi dùng tôpô do $p$ xác định. Tập hợp $E'$ các dạng tuyến tính trên $E$ liên tục đối với $\mathcal{T}$ là hợp của các tập hợp $E'_p$, trong đó $E'_p$ là tập hợp các dạng tuyến tính liên tục trên $E_p$ ($p \in \Gamma$).
