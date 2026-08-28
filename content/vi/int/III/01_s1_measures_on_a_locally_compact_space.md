---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 1
section_title: Measures on a locally compact space
lang: vi
source: int-i-vi
pdf_pages: 0046-0068, 0100-0104
extraction: ocr
subsections:
    - "no": 1
      title: Continuous functions with compact support
      page: 0
      pdf_page: 46
    - "no": 2
      title: Approximation properties
      page: 4
      pdf_page: 49
    - "no": 3
      title: Definition of a measure
      page: 7
      pdf_page: 52
    - "no": 4
      title: Product of a measure by a continuous function
      page: 10
      pdf_page: 55
    - "no": 5
      title: Real measures. Positive measures
      page: 11
      pdf_page: 56
    - "no": 6
      title: Absolute value of a complex measure
      page: 13
      pdf_page: 58
    - "no": 7
      title: Definition of a measure by extension
      page: 15
      pdf_page: 60
    - "no": 8
      title: Bounded measures
      page: 16
      pdf_page: 61
    - "no": 9
      title: Vague topology on the space of measures
      page: 18
      pdf_page: 63
    - "no": 10
      title: Compact convergence in $\mathcal{M}(X; \mathbf{C})$
      page: 21
      pdf_page: 66
statements: 41
exercises: 18
content_sha256: 537a1077247b8bc3b925580a9e360ade89eb6f7add7ead3d6efb9731ff48fde0
translated_from: content/en/int/III/01_s1_measures_on_a_locally_compact_space.md
source_content_sha256: 7a621ccaf41aa9696a8e26acf7ca61fbadd6582267dd5d90d4a9b8e5b4e6599f
translation_model: gpt-5.4, gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-fc85bf3a
glossary_version: 34
glossary_terms_sha256: de83b1ccc456b659a8ad623abf3d6c8c356a4950c1639100d7db93f7659a0a17
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. CÁC ĐỘ ĐO TRÊN MỘT KHÔNG GIAN COMPACT ĐỊA PHƯƠNG

### 1. Các hàm liên tục có giá đỡ compact

#### Định nghĩa 1 {#int-iii-s1-def-1 .statement}

— Cho X là một không gian tôpô, E là hoặc $\overline{\mathbf{R}}$ hoặc một không gian vectơ trên $\mathbf{R}$, và f là một ánh xạ từ X vào E. Tập đóng nhỏ nhất S trong X sao cho $f(x) = 0$ trên $X - S$ (nói cách khác, bao đóng trong X của tập hợp mọi $x \in X$ sao cho $f(x) \neq 0$) được gọi là giá đỡ của f và được ký hiệu là Supp(f).

Cho X là một không gian compact địa phương, E là một không gian vectơ tôpô trên $\mathbf{R}$ hoặc $\mathbf{C}$; nhắc lại rằng $\mathcal{C}(X;E)$ ký hiệu không gian vectơ các ánh xạ liên tục từ X vào E; khi $E = \mathbf{R}$ hoặc $E = \mathbf{C}$, ta sẽ bỏ không nhắc đến E trong ký hiệu này nếu không thể gây nhầm lẫn. Ta sẽ ký hiệu bởi $\mathcal{K}(X;E)$ không gian con của $\mathcal{C}(X;E)$ gồm các ánh xạ liên tục có giá đỡ compact; với mọi tập con A của X, ta ký hiệu bởi $\mathcal{C}(X,A;E)$ (tương ứng, $\mathcal{K}(X,A;E)$) không gian con của $\mathcal{C}(X;E)$ (tương ứng, $\mathcal{K}(X;E)$) gồm các ánh xạ f sao cho $\operatorname{Supp}(f) \subset A$. Nếu $E = \mathbf{R}$ hoặc $E = \mathbf{C}$, ta viết $\mathcal{K}(X)$ (tương ứng, $\mathcal{K}(X,A)$) thay cho $\mathcal{K}(X;\mathbf{R})$ hoặc $\mathcal{K}(X;\mathbf{C})$ (tương ứng, $\mathcal{K}(X,A;\mathbf{R})$ hoặc $\mathcal{K}(X,A;\mathbf{C})$), miễn là không thể gây nhầm lẫn; ta ký hiệu bởi $\mathcal{K}_+(X)$ nón lồi nhọn tạo bởi các hàm $\geq 0$ của $\mathcal{K}(X;\mathbf{R})$.

Với mọi tập con compact K của X, không gian $\mathcal{K}(X,K;E)$ có thể được đồng nhất với một không gian con của không gian các hàm liên tục $\mathcal{C}(K;E)$ (cụ thể là không gian con các ánh xạ liên tục từ K vào E triệt tiêu trên biên$^1$ của K). Khi $\mathcal{C}(K;E)$ được trang bị tôpô hội tụ đều trên K, thì $\mathcal{K}(X,K;E)$ là một không gian con đóng của $\mathcal{C}(K;E)$. Đặc biệt, nếu E là một không gian Fréchet (tương ứng, một không gian Banach), thì $\mathcal{K}(X,K;E)$ cũng vậy, vì nếu tôpô của E được xác định bởi các nửa chuẩn $p_n$ (tương ứng, chuẩn $x \mapsto \|x\|$) thì tôpô của $\mathcal{K}(X,K;E)$ được xác định

\footnotetext{1}{Nguyên bản là frontière, cũng được dịch là 'frontier' (GT, I, §1, No. 6, Def. 11).}

bởi các nửa chuẩn $f \mapsto \sup_{x \in K} p_n(f(x))$ (tương ứng, chuẩn $f \mapsto \sup_{x \in K} \|f(x)\|$, ký hiệu là $\|f\|$).

Không gian $\mathcal{K}(X; E)$ là hợp của họ tăng có hướng các không gian con $\mathcal{K}(X, K; E)$, trong đó $K$ chạy qua tập hợp các tập con compact của $X$; hơn nữa, nếu $K_1 \subset K_2$ là hai tập con compact của $X$, thì đơn ánh chính tắc $\mathcal{K}(X, K_1; E) \to \mathcal{K}(X, K_2; E)$ là liên tục đối với các tôpô đã xác định ở trên. Nếu $E$ là *lồi địa phương*, do đó ta có thể định nghĩa trên $\mathcal{K}(X; E)$ *giới hạn trực tiếp*² của các tôpô lồi địa phương của các $\mathcal{K}(X, K; E)$ (TVS, II, §4, No. 4); trừ khi nói rõ ngược lại, đây sẽ luôn luôn là tôpô đang xét khi ta xem $\mathcal{K}(X; E)$ như một không gian vectơ tôpô.

#### Mệnh đề 1 {#int-iii-s1-prop-1 .statement}

*Cho $X$ là một không gian compact địa phương, $E$ là một không gian Hausdorff lồi địa phương.*

(i) *Không gian lồi địa phương $\mathcal{K}(X; E)$ là Hausdorff. Với mọi tập con compact $K$ của $X$, tôpô trên $\mathcal{K}(X, K; E)$ cảm sinh bởi tôpô của $\mathcal{K}(X; E)$ là tôpô hội tụ đều trên $K$, và mỗi không gian con $\mathcal{K}(X, K; E)$ đều đóng trong $\mathcal{K}(X; E)$.*

(ii) *Nếu $E$ là tích của một số hữu hạn các không gian lồi địa phương $E_i$ ($1 \leq i \leq n$), thì ánh xạ $f \mapsto (\mathrm{pr}_i \circ f)$ là một đẳng cấu của không gian $\mathcal{K}(X; E)$ lên không gian tích $\prod_{1 \leq i \leq n} \mathcal{K}(X; E_i)$.*

(iii) *Nếu $X$ là tổng của một họ $(X_\lambda)_{\lambda \in L}$ các không gian compact địa phương, thì ánh xạ $f \mapsto (f|X_\lambda)_{\lambda \in L}$ là một đẳng cấu của không gian $\mathcal{K}(X; E)$ lên không gian tổng trực tiếp tôpô của họ $(\mathcal{K}(X_\lambda; E))_{\lambda \in L}$.*

(i) Chú ý rằng, trên $\mathcal{K}(X; E)$, tôpô hội tụ đều *trên* $X$ là tương thích với cấu trúc không gian vectơ của $\mathcal{K}(X; E)$ bởi vì, với mọi $f \in \mathcal{K}(X; E)$, có giá compact là $S$, tập $f(X) = f(S) \cup \{0\}$ là compact, do đó bị chặn trong $E$ (TVS, III, §3, No. 1, Prop. 1). Vì tôpô này $\mathcal{T}_0$ là lồi địa phương và cảm sinh trên mỗi $\mathcal{K}(X, K; E)$ tôpô hội tụ đều trên $K$, nên điều đó cũng đúng đối với tôpô giới hạn trực tiếp $\mathcal{T}$ trên $\mathcal{K}(X; E)$ (TVS, II, §4, No. 4, *Nhận xét*); hơn nữa, $\mathcal{T}$ mịn hơn $\mathcal{T}_0$ và $\mathcal{T}_0$ là Hausdorff, vì vậy $\mathcal{T}$ là Hausdorff. Sau cùng, giả sử rằng một hàm $f \in \mathcal{K}(X; E)$ thuộc bao đóng của $\mathcal{K}(X, K; E)$; theo các định nghĩa, tồn tại một tập con compact $K' \supset K$ của $X$ sao cho $f \in \mathcal{K}(X, K'; E)$. Theo điều vừa nói trên, $f$ thuộc bao đóng của $\mathcal{K}(X, K; E)$ trong không gian $\mathcal{K}(X, K'; E)$, do đó thuộc $\mathcal{K}(X, K; E)$.

(ii) Tiêu chuẩn về tính liên tục trong một giới hạn trực tiếp (TVS, II, §4, No. 4, Prop. 5) cho thấy ngay rằng ánh xạ $f \mapsto (\mathrm{pr}_i \circ f)$ là liên tục và điều tương tự cũng đúng với ánh xạ nghịch đảo (đối với ánh xạ sau, chỉ cần chú ý rằng nếu, với mọi hàm $f_i \in \mathcal{K}(X; E_i)$, ta ký hiệu bởi $f'_i$ ánh xạ

² *Limite inductive*, được dịch là "giới hạn trực tiếp" trong S, A và GT.

từ X vào E sao cho $\mathrm{pr}_i \circ f'_i = f_i$ và $\mathrm{pr}_j \circ f'_i = 0$ với $j \neq i$, thì mỗi ánh xạ $f_i \mapsto f'_i$ đều liên tục).

(iii) Mỗi tập compact K của X chỉ cắt các $X_\lambda$ của một họ con hữu hạn $(X_\lambda)_{\lambda \in H}$ của $(X_\lambda)_{\lambda \in L}$, và ngay lập tức thấy rằng nếu đặt $K_\lambda = K \cap X_\lambda$ với $\lambda \in H$, thì ánh xạ $f \mapsto (f|X_\lambda)_{\lambda \in H}$ là một đẳng cấu từ $\mathcal{K}(X, K; E)$ lên $\prod_{\lambda \in H} \mathcal{K}(X_\lambda, K_\lambda; E)$. Ngược lại, với mọi hàm $f_\lambda \in \mathcal{K}(X_\lambda; E)$, gọi $f''_\lambda$ là ánh xạ từ X vào E sao cho $f''_\lambda|X_\lambda = f_\lambda$ và $f''_\lambda|X_\mu = 0$ nếu $\mu \neq \lambda$; ngay lập tức thấy rằng ánh xạ $f_\lambda \mapsto f''_\lambda$ từ $\mathcal{K}(X_\lambda; E)$ vào $\mathcal{K}(X; E)$ là liên tục. Mệnh đề (iii) suy ra từ các nhận xét này và tiêu chuẩn về tính liên tục trong các giới hạn trực tiếp (TVS, II, §4, No. 4, Prop. 5).

#### Mệnh đề 2 {#int-iii-s1-prop-2 .statement}

— *Cho X là một không gian địa phương compact, E là một không gian lồi địa phương Hausdorff.*

(i) *Nếu E là một không gian Fréchet, thì không gian $\mathcal{K}(X; E)$ là tròn.*

(ii) *Nếu X là paracompact thì, với mọi tập bị chặn B trong $\mathcal{K}(X; E)$, tồn tại một tập compact K của X sao cho $B \subset \mathcal{K}(X, K; E)$.*

Giả sử E là một không gian Fréchet. Khi đó, với mọi tập compact K của X, $\mathcal{K}(X, K; E)$ là một không gian Fréchet, nên là tròn, và ta biết rằng giới hạn trực tiếp của các không gian tròn là tròn (TVS, III, §4, No. 1, Cor. 3 of Prop. 3), do đó suy ra (i).

Nếu X là paracompact, ta biết (GT, I, §9, No. 10, Th. 5) rằng X là tổng của một họ $(X_\lambda)_{\lambda \in L}$ các không gian địa phương compact và *đếm được ở vô cùng*; do đó (Prop. 1, (iii)), $\mathcal{K}(X; E)$ là *tổng trực tiếp tôpô* của họ các không gian con $\mathcal{K}(X_\lambda; E)$ ($\lambda \in L$). Theo đặc trưng hóa của các tập bị chặn trong một tổng trực tiếp tôpô (TVS, III, §1, No. 4, Prop. 5), mọi tập bị chặn trong $\mathcal{K}(X; E)$ đều được chứa trong tổng của một số *hữu hạn* các không gian con $\mathcal{K}(X_\lambda; E)$, và chỉ cần chứng minh rằng mọi tập bị chặn trong $\mathcal{K}(X_\lambda; E)$ đều được chứa trong một không gian con $\mathcal{K}(X_\lambda, K_\lambda; E)$, với $K_\lambda$ compact trong $X_\lambda$. Như vậy ta được quy về trường hợp X đếm được ở vô cùng, nói cách khác là hợp của một dãy các tập mở tương đối compact $U_n$ sao cho $\overline{U}_n \subset U_{n+1}$ (GT, I, §9, No. 9, Prop. 15). Nhưng khi đó $\mathcal{K}(X; E)$ là giới hạn trực tiếp *ngặt* của dãy các không gian $\mathcal{K}(X, \overline{U}_n; E)$, do đó suy ra mệnh đề (ii) (TVS, III, §1, No. 4, Prop. 6).

Ta sẽ nói rằng một tập con H của $\mathcal{K}(X; E)$ là *compact ngặt* nếu nó compact và nếu tồn tại một tập compact K của X sao cho $H \subset \mathcal{K}(X, K; E)$. Suy ra ngay từ Mệnh đề 2 rằng nếu X là một không gian địa phương compact *paracompact* và nếu E là Hausdorff, thì *mọi tập compact* trong $\mathcal{K}(X; E)$ đều là *compact ngặt*. Có thể cho các ví dụ về những không gian địa phương compact

3 *Dénombrable à l'infini*, cũng được dịch là "σ-compact" (GT, I, §9, No. 9, Def. 5).

$X$ (không paracompact) sao cho tồn tại những tập trong $\mathcal{K}(X; \mathbf{R})$ *compact nhưng không compact ngặt* (Bài tập 3 và 4).

Ta nhắc lại rằng, theo định lý Ascoli (GT, X, §2, No. 5, Cor. 3 of Th. 2), một tập con compact ngặt $H$ của $\mathcal{K}(X; E)$ được chứa trong $\mathcal{K}(X, K; E)$ được đặc trưng bởi các điều kiện sau đây: $1^\circ$ nó đóng; $2^\circ$ nó đồng liên tục; $3^\circ$ với mọi $x \in K$, tập $H(x)$ là tương đối compact trong $E$.

#### Hệ quả {#int-iii-s1-n1-cor-1 .statement}

*Cho $X$ là một không gian paracompact, địa phương compact; nếu $E$ là một không gian lồi địa phương quasi-đầy đủ, thì không gian $\mathcal{K}(X; E)$ là quasi-đầy đủ.*

Chỉ cần, theo Mệnh đề 2, (ii), chú ý rằng với mọi tập compact $K$ của $X$, $\mathcal{K}(X, K; E)$ là một không gian con đóng của $C(K; E)$, mà không gian này là quasi-đầy đủ vì mọi tập con bị chặn của $C(K; E)$ đều gồm những hàm nhận giá trị trong cùng một tập con bị chặn của $E$.

### 2. Các tính chất xấp xỉ

#### Bổ đề 1 {#int-iii-s1-lem-1 .statement}

*Cho $X$ là một không gian địa phương compact, $K$ là một tập con compact của $X$, và $(V_k)_{1 \leq k \leq n}$ là một phủ hữu hạn của $K$ bởi các tập mở của $X$. Khi đó, tồn tại $n$ ánh xạ liên tục $f_k$ từ $X$ vào $[0, 1]$, sao cho giá của $f_k$ được chứa trong $V_k$ với $1 \leq k \leq n$ và sao cho $\sum_{k=1}^n f_k(x) \leq 1$ với mọi $x \in X$ và $\sum_{k=1}^n f_k(x) = 1$ với mọi $x \in K$.

Thật vậy, gọi $X'$ là không gian compact thu được bằng cách thêm vào $X$ một điểm ở vô cực $\omega$ (GT, I, §9, No. 8, Đl. 4); các tập hợp $V_0 = X' - K$ và $V_k$ ($1 \leq k \leq n$) tạo thành một phủ mở của $X'$. Gọi $(f_k)_{0 \leq k \leq n}$ là một phân hoạch đơn vị liên tục phụ thuộc phủ này của $X'$ (GT, IX, §4, No. 3, Mệnh đề 3); các hàm $f_k$ với chỉ số $k \geq 1$ thỏa mãn các điều kiện của bổ đề.

#### Bổ đề 2 {#int-iii-s1-lem-2 .statement}

*Cho $X$ là một không gian địa phương compact, $K$ là một tập con compact của $X$, $E$ là một không gian lồi địa phương, $q$ là một nửa chuẩn liên tục trên $E$, và $\Phi$ là một tập hợp đồng liên tục các ánh xạ từ $X$ vào $E$ mà các giá được chứa trong $K$. Khi đó, với mọi $\varepsilon > 0$, tồn tại một phân hoạch đơn vị liên tục $(\varphi_j)_{0 \leq j \leq n}$ trên $X$ có các tính chất sau:
(i) $\operatorname{Supp}(\varphi_j) \subset K$ với $1 \leq j \leq n$.
(ii) *Nếu, với $1 \leq j \leq n$, $x_j$ là một điểm bất kỳ của $\operatorname{Supp}(\varphi_j)$, thì, với mọi hàm $f \in \Phi$ và mọi $x \in X$,
$$
q\left(f(x) - \sum_{j=1}^n \varphi_j(x) f(x_j)\right) \leq \varepsilon.
$$*

Với mọi $y$ thuộc biên của $K$, ta có $f(y) = 0$ với mọi $f \in \Phi$, do đó tồn tại một lân cận mở $V_y$ của $y$ trong $X$ sao cho, với mọi $z \in V_y$ và mọi $f \in \Phi$, ta có $q(f(z)) \leq \varepsilon/2$. Gọi $K'$ là tập hợp các điểm của $K$ không thuộc bất kỳ $V_y$ nào khi $y$ chạy trên biên của $K$; $K'$ là compact và được chứa trong phần trong của $K$. Tập hợp $\Phi$ là liên tục đều đồng bậc trong $K$; do đó, tồn tại một phủ mở hữu hạn $(U_j)_{1 \leq j \leq n}$ của $K'$ gồm các tập mở trong $X$ được chứa trong $K$, sao cho với mọi cặp điểm $x, y$ của cùng một $U_j$, ta có $q(f(x) - f(y)) \leq \varepsilon/2$ với mọi $f \in \Phi$. Theo Bổ đề 1, tồn tại $n$ ánh xạ liên tục $\varphi_j$ từ $X$ vào $[0, 1]$ ($1 \leq j \leq n$) sao cho $\operatorname{Supp}(\varphi_j) \subset U_j$ và sao cho
$$
\sum_{j=1}^n \varphi_j(x) \leq 1 \text{trên } X \text{và } \sum_{j=1}^n \varphi_j(x) = 1 \text{trên } K'.
$$
Với $x_j \in \operatorname{Supp}(\varphi_j)$ ($1 \leq j \leq n$) và $f \in \Phi$, do đó ta có, với mọi $x \in U_j$,
$$
q(f(x)\varphi_j(x) - f(x_j)\varphi_j(x)) = \varphi_j(x)q(f(x) - f(x_j)) \leq \frac{\varepsilon}{2}\varphi_j(x),
$$
và quan hệ này vẫn đúng nếu $x \notin U_j$ vì khi đó $\varphi_j(x) = 0$. Bằng phép cộng ta suy ra rằng, với mọi $x \in X$,
$$
q\left(f(x)(1 - \varphi_0(x)) - \sum_{j=1}^n \varphi_j(x)f(x_j)\right) \leq \frac{\varepsilon}{2}(1 - \varphi_0(x)),
$$
trong đó $\varphi_0 = 1 - \sum_{j=1}^n \varphi_j$; do đó suy ra (1) với $x \in K'$, vì khi đó $\varphi_0(x) = 0$;
(1) cũng đúng với $x \notin K$, khi đó số hạng thứ nhất bằng không. Cuối cùng, với $x \in K - K'$ ta có $q(f(x)\varphi_0(x)) \leq \varepsilon/2$ theo định nghĩa của $K'$, do đó quan hệ này và (2) lại suy ra (1) trong trường hợp này.

Cho $X$ là một không gian compact địa phương; với mỗi không gian Banach $E$ (thực hoặc phức) ta ký hiệu bởi $\mathcal{C}^b(X; E)$ không gian vectơ của các ánh xạ liên tục và bị chặn từ $X$ vào $E$; ta biết rằng tôpô hội tụ đều trong $X$ là tương thích với cấu trúc không gian vectơ (thực, tương ứng phức) của $\mathcal{C}^b(X; E)$, và nó được xác định bởi chuẩn
$$
||f|| = \sup_{x \in X} ||f(x)||.
$$
Hơn nữa, không gian định chuẩn được xác định như vậy là một không gian Banach (GT, X, §3, No. 2, và No. 1, Hệ quả 2 của Mệnh đề 2); tôpô được xác định bởi chuẩn này trên $\mathscr{K}(X; E)$ (nói cách khác, tôpô hội tụ đều trong $X$) thô hơn tôpô giới hạn trực tiếp trên $\mathscr{K}(X; E)$ được xác định trong No. 1.

#### Mệnh đề 3 {#int-iii-s1-prop-3 .statement}

— Cho $X$ là một không gian compact địa phương, $X'$ là không gian compact thu được bằng cách thêm vào $X$ một điểm ở vô cực $\omega$ (GT, I, §9, No. 8,

Định lý 4), và E là một không gian Banach. Bao đóng của $\mathcal{K}(X;E)$ trong không gian định chuẩn $C^b(X;E)$ là không gian vectơ của các hàm liên tục trên X, nhận giá trị trong E và dần tới 0 tại điểm $\omega$.

Cho $f \in C^b(X;E)$ là một hàm thuộc bao đóng của $\mathcal{K}(X;E)$; với mọi $\varepsilon > 0$, tồn tại một hàm $g \in \mathcal{K}(X;E)$ sao cho $\|f(x) - g(x)\| \leq \varepsilon$ với mọi $x \in X$; nếu K là giá của g, thì suy ra rằng $\|f(x)\| \leq \varepsilon$ với mọi $x \in \mathbf{C}K$, do đó $f(x)$ dần tới 0 khi $x$ dần tới $\omega$. Ngược lại, nếu f có tính chất này thì, với mọi $\varepsilon > 0$, tồn tại một tập compact $K \subset X$ sao cho $\|f(x)\| \leq \varepsilon$ với mọi $x \in \mathbf{C}K$. Theo Bổ đề 1 tồn tại một ánh xạ liên tục h từ X vào $[0,1]$, có giá compact, bằng 1 trên K; khi đó $\|f(x)h(x)\| \leq \varepsilon$ trên $\mathbf{C}K$ và $f(x) = f(x)h(x)$ trên K; vì $fh$ có giá compact và $\|f(x) - f(x)h(x)\| \leq 2\varepsilon$ với mọi $x \in X$, mệnh đề được chứng minh.

Ta sẽ ký hiệu bởi $C^0(X;E)$ không gian con của $C^b(X;E)$ tạo bởi các hàm dần tới không tại điểm ở vô cực $\omega$; do đó nó là phần bù của không gian định chuẩn $\mathcal{K}(X;E)$.

#### Mệnh đề 4 {#int-iii-s1-prop-4 .statement}

— Cho X là một không gian compact địa phương, E là một không gian lồi địa phương; khi đó, không gian $\mathcal{K}(X;E)$ là trù mật trong $C(X;E)$ đối với tôpô hội tụ compact.

Với mỗi tập compact $K \subset X$, tồn tại một hàm $h \in \mathcal{K}(X;\mathbf{R})$ bằng 1 trên K, theo Bổ đề 1; với mỗi hàm $f \in C(X;E)$ hàm $hf$, thuộc $\mathcal{K}(X;E)$, bằng f trên K, do đó có mệnh đề của ta.

#### Mệnh đề 5 {#int-iii-s1-prop-5 .statement}

— Cho X là một không gian compact địa phương, E là một không gian lồi địa phương thực (tương ứng phức). Với mỗi tập con compact K của X, không gian vectơ $\mathcal{K}(X,K;\mathbf{R}) \otimes_{\mathbf{R}} E$ (tương ứng $\mathcal{K}(X,K;\mathbf{C}) \otimes_{\mathbf{C}} E$) (được đồng nhất với một tập hợp các ánh xạ từ X vào E, cf. A, II, §7, No. 7, Hệ quả của Mệnh đề 15) là trù mật trong $\mathcal{K}(X,K;E)$; không gian vectơ $\mathcal{K}(X;\mathbf{R}) \otimes_{\mathbf{R}} E$ (tương ứng $\mathcal{K}(X;\mathbf{C}) \otimes_{\mathbf{C}} E$) là trù mật trong $\mathcal{K}(X;E)$.

Vì khẳng định thứ hai là một hệ quả hiển nhiên của khẳng định thứ nhất, chỉ cần chứng minh khẳng định sau. Ta áp dụng Bổ đề 2 với $\Phi$ thu gọn về một phần tử duy nhất $f$ của $\mathcal{K}(X,K;E)$; khi đó, với mọi $x \in X$,

$$
q\left(f(x) - \sum_{j=1}^n \varphi_j(x)f(x_j)\right) \leq \varepsilon,
$$

trong đó các $\varphi_j$ thuộc $\mathcal{K}(X,K;\mathbf{R})$; vì ánh xạ $x \mapsto \sum_{j=1}^n \varphi_j(x)f(x_j)$ có thể được đồng nhất một cách chính tắc với phần tử $\sum_{j=1}^n \varphi_j \otimes f(x_j)$, điều này chứng minh mệnh đề, theo định nghĩa của tôpô của $\mathcal{K}(X,K;E)$.

### 3. Định nghĩa một độ đo

#### Định nghĩa 2 {#int-iii-s1-def-2 .statement}

— *Một dạng tuyến tính liên tục trên* $\mathcal{K}(X; \mathbf{C})$, *X một không gian compact địa phương*, *được gọi là một độ đo* (hay *độ đo phức*) *trên X*.

Nếu $\mu$ là một độ đo trên một không gian compact địa phương $X$, giá trị của độ đo đối với một hàm $f \in \mathcal{K}(X; \mathbf{C})$ được gọi là *tích phân của f theo* $\mu$; ngoài các ký hiệu tổng quát $\mu(f)$ và $\langle f, \mu \rangle$, người ta còn dùng các ký hiệu $\int f d\mu$, $\int f \mu$, $\int f(x) d\mu(x)$ và $\int f(x) \mu(x)$ để chỉ nó; về việc sử dụng chữ cái $x$, xem S, I, §1, No. 1.

Theo tiêu chuẩn về tính liên tục trong các giới hạn trực tiếp (TVS, Ch. II, §4, No. 4, Mệnh đề 5), nói rằng $\mu$ là một độ đo trên $X$ có nghĩa là $\mu$ là một dạng tuyến tính trên $\mathcal{K}(X; \mathbf{C})$ thỏa mãn điều kiện sau: với mọi tập con compact $K$ của $X$, tồn tại một số $M_K$ sao cho, với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$ *có giá đỡ được chứa trong* $K$,

$$
| \mu(f) | \leq M_K \cdot \| f \| \quad \text{(trong đó } \| f \| = \sup_{x \in X} |f(x)| ).
$$

Tổng quát hơn:

#### Mệnh đề 6 {#int-iii-s1-prop-6 .statement}

— *Cho X là một không gian compact địa phương, ($K_\alpha$) là một họ các tập con compact của X mà các phần trong $\overset{\circ}{K}_\alpha$ lập thành một phủ mở của X. Đối với một dạng tuyến tính $\mu$ trên $\mathcal{K}(X; \mathbf{C})$, để là một độ đo trên X, điều kiện cần và đủ là, với mỗi $\alpha$, tồn tại một số $M_\alpha$ sao cho*

$$
| \mu(f) | \leq M_\alpha \cdot \| f \|
$$

*đối với mọi hàm* $f \in \mathcal{K}(X, K_\alpha; \mathbf{C})$.

Điều kiện này hiển nhiên là cần, chỉ cần chứng minh rằng (5) kéo theo (4) đối với mọi tập con compact $K$ của $X$. Bây giờ, $K$ được phủ bởi một số hữu hạn các tập mở $\overset{\circ}{K}_{\alpha_i}$ ($1 \leq i \leq n$); áp dụng Bổ đề 1 của No. 2 cho $K$ và cho các $\overset{\circ}{K}_{\alpha_i}$, tồn tại các hàm liên tục $g_i \geq 0$ trên $X$ sao cho $\operatorname{Supp}(g_i) \subset K_{\alpha_i}$, $0 \leq \sum_{i=1}^n g_i(x) \leq 1$ với mọi $x \in X$ và $\sum_{i=1}^n g_i(x) = 1$ với $x \in K$. Với mọi hàm $f \in \mathcal{K}(X, K; \mathbf{C})$, do đó ta có thể viết $f = \sum_{i=1}^n f g_i$ và ta có $f g_i \in \mathcal{K}(X, K_{\alpha_i}; \mathbf{C})$ và $\| f g_i \| \leq \| f \|$; nếu $M_K = \sum_{i=1}^n M_{\alpha_i}$, khi đó ta có quan hệ (4).

Ta ký hiệu bởi $\mathcal{M}(X; \mathbf{C})$, hoặc đơn giản là $\mathcal{M}(X)$ nếu không thể gây nhầm lẫn, không gian vectơ các độ đo trên $X$, nói cách khác, *đối ngẫu* của $\mathcal{K}(X; \mathbf{C})$.

Ta biết rằng với mọi tập hợp $\mathscr{S}$ các tập con *bị chặn* của $\mathscr{K}(X;\mathbf{C})$, có xác định trên $\mathscr{M}(X;\mathbf{C})$ tôpô $\mathscr{S}$, tôpô này lồi địa phương (TVS, III, §3, No. 1, Hệ quả của Mệnh đề 1). Ta ký hiệu không gian vectơ tôpô thu được bằng cách trang bị cho $\mathscr{M}(X;\mathbf{C})$ tôpô $\mathscr{S}$ bởi $\mathscr{M}_{\mathscr{S}}(X;\mathbf{C})$ hoặc $\mathscr{M}_{\mathscr{S}}(X)$.

#### Mệnh đề 7 {#int-iii-s1-prop-7 .statement}

*Với mọi tập hợp $\mathscr{S}$ các tập con bị chặn của $\mathscr{K}(X;\mathbf{C})$ là một phủ của $\mathscr{K}(X;\mathbf{C})$, không gian $\mathscr{M}_{\mathscr{S}}(X;\mathbf{C})$ là Hausdorff và gần đầy đủ.*

Điều này suy ra từ việc $\mathscr{K}(X;\mathbf{C})$ là thùng (TVS, III, §4, No. 2, Hệ quả 4 của Định lý 1).

*Các ví dụ về độ đo.* — I. *Các độ đo nguyên tử.* Cho X là một không gian compact địa phương, $a$ là một điểm của X; ánh xạ $f\mapsto f(a)$ từ $\mathscr{K}(X;\mathbf{C})$ vào $\mathbf{C}$ hiển nhiên thỏa mãn điều kiện (4) với $M_K=1$ đối với mọi tập con compact K của X chứa $a$, do đó là một độ đo trên X, được ký hiệu bởi $\varepsilon_a$; nó được gọi là *độ đo Dirac* tại điểm $a$, hoặc độ đo được xác định bởi một *khối lượng đơn vị đặt tại điểm $a$.*

Tổng quát hơn, cho $\alpha$ là một ánh xạ từ X vào $\mathbf{C}$ sao cho, với mọi tập con compact K của X,
$$
\sum_{x\in K}|\alpha(x)|<+\infty.
$$
Khi đó, với mọi hàm $f\in\mathscr{K}(X,K;\mathbf{C})$, tổng
$$
\mu(f)=\sum_{x\in X}\alpha(x)f(x)
$$
được xác định, vì nó bằng
$$
\sum_{x\in K}\alpha(x)f(x);
$$
rõ ràng $\mu$ là một dạng tuyến tính trên $\mathscr{K}(X;\mathbf{C})$ và, với $f\in\mathscr{K}(X,K;\mathbf{C})$,
$$
|\mu(f)|\leq\left(\sum_{x\in K}|\alpha(x)|\right)\cdot\|f\|,
$$
nói cách khác điều kiện (4) được thỏa mãn.

Một độ đo $\mu$ trên X được gọi là *nguyên tử* nếu tồn tại một ánh xạ $\alpha$ từ X vào $\mathbf{C}$ sao cho
$$
\sum_{x\in K}|\alpha(x)|<+\infty
$$
đối với mọi tập con compact K của X, và sao cho $\mu$ bằng độ đo được xác định như trên. Nếu N là tập hợp các $x\in X$ sao cho $\alpha(x)\neq0$, điều kiện đặt lên $\alpha$ kéo theo rằng với mọi tập con compact K của X, $K\cap N$ là *đếm được*. Người ta cũng nói rằng $\mu$ được xác định bởi các *khối lượng* $\alpha(x)$ *đặt tại các điểm* $x\in N$. Nếu giả sử rằng $N\cap K$ là *hữu hạn* đối với mọi tập compact $K\subset X$, thì hiển nhiên
$$
\sum_{x\in K}|\alpha(x)|<+\infty;
$$
điều đó tương đương với việc nói rằng N là một không gian con *đóng* và *rời rạc* của X, vì khi đó mọi điểm của X đều có một lân cận compact chỉ chứa một số hữu hạn điểm của N, và ngược lại, nếu điều này đúng, thì mọi tập con compact của X có thể được phủ bởi một số hữu hạn lân cận như thế. Khi N đóng và rời rạc, mọi độ đo nguyên tử được xác định bởi một hàm $\alpha$ sao cho $\alpha(x)=0$ trên $\mathbf C N$ được gọi là một độ đo rời rạc trên X (xem §2, No. 5).

### II. *Độ đo Lebesgue.* Với mọi hàm $f\in\mathcal K(\mathbf R;\mathbf C)$, tồn tại một khoảng compact $[a,b]$ của $\mathbf R$ mà bên ngoài đó $f$ bằng không. Tích phân

$$
\mathrm I(f)=\int_{-\infty}^{+\infty}f(x)\,dx=\int_a^b f(x)\,dx
$$

do đó được xác định; hơn nữa, theo định lý giá trị trung bình (FRV, II, §1, No. 5, Prop. 6), ta có $|\mathrm I(f)|\leq(b-a)\|f\|$; điều này cho thấy rằng $f\mapsto\mathrm I(f)$ là một độ đo trên $\mathbf R$, được gọi là *độ đo Lebesgue*.

Đối với mọi khoảng J (bị chặn hoặc không) của $\mathbf R$, tương tự người ta gọi *độ đo Lebesgue trên J* là độ đo $f\mapsto\int_Jf(x)\,dx$, một dạng tuyến tính trên $\mathcal K(J;\mathbf C)$ (tích phân có nghĩa vì tồn tại một khoảng compắc $[a,b]$ được chứa trong J mà bên ngoài đó $f$ bằng không).

### III. Cho $g$ là một ánh xạ liên tục từ một khoảng compắc $I\subset\mathbf R$ vào $\mathbf C$, có đạo hàm liên tục trên I. Đặt $\Gamma=g(I)$, là một không gian con compắc của $\mathbf C$; ánh xạ

$$
f\mapsto\int_I f(g(t))g'(t)\,dt
$$

từ $\mathcal C(\Gamma;\mathbf C)$ vào $\mathbf C$ là một dạng tuyến tính liên tục theo định lý giá trị trung bình, do đó là một *độ đo phức trên $\Gamma$*; tích phân đối với độ đo này cũng được viết là $\int_\Gamma f(z)\,dz$, mặc dù nó không những phụ thuộc vào $\Gamma$ mà còn phụ thuộc vào $g$.

#### Nhận xét {#int-iii-s1-n3-rem-1 .statement}

Việc cho một độ đo $\mu$ trên một không gian địa phương compắc X xác định trên X (cùng với tôpô của X) một cấu trúc $\mathscr S$. Cho $X_1$ là một tập hợp thứ hai, $\varphi$ là một ánh xạ song ánh từ X lên $X_1$; phù hợp với các định nghĩa tổng quát (S, R, §8), cấu trúc $\mathscr S_1$ thu được bằng cách *chuyển* lên $X_1$ cấu trúc $\mathscr S$ của X, nhờ $\varphi$, được xác định theo cách sau. Tôpô của X được chuyển sang $X_1$ bởi $\varphi$; khi đó các hàm của $\mathcal K(X_1;\mathbf C)$ là các hàm $f$ sao cho $f\circ\varphi$ thuộc $\mathcal K(X;\mathbf C)$, và độ đo $\mu_1$ trên $X_1$ được xác định bởi $\mu_1(f)=\mu(f\circ\varphi)$.

Đặc biệt, một *tự đẳng cấu* của cấu trúc $\mathscr S$ là một đồng phôi $\sigma$ của X lên chính nó, sao cho

$$
\mu(f)=\mu(f\circ\sigma)
$$

đối với mọi hàm $f\in\mathcal K(X;\mathbf C)$; khi đó độ đo $\mu$ cũng được gọi là *bất biến dưới đồng phôi* $\sigma$.

#### Ví dụ {#int-iii-s1-n3-exa-1 .statement}

Độ đo Lebesgue trên $\mathbf{R}$ là bất biến dưới mọi phép tịnh tiến của nhóm cộng $\mathbf{R}$. Thật vậy, với mọi hàm $f \in \mathcal{K}(\mathbf{R}; \mathbf{C})$ và mọi số thực $a$, ta có

$$
\int_{-\infty}^{+\infty} f(x + a)\, dx = \int_{-\infty}^{+\infty} f(t)\, dt
$$

theo công thức đổi biến (FRV, II, §2, No. 1, formula (1)). Để biết một phép tổng quát hóa, xem Ch. VII, §1, No. 2, Định lý 1.

### 4. Tích của một độ đo với một hàm liên tục

Cho $X$ là một không gian địa phương compact, $g$ là một ánh xạ liên tục từ $X$ vào $\mathbf{C}$. Hiển nhiên $f \mapsto gf$ là một ánh xạ tuyến tính của $\mathcal{K}(X; \mathbf{C})$ vào chính nó; ta hãy chỉ ra rằng ánh xạ này liên tục. Thật vậy, với mọi tập con compact $K$ của $X$, và với mọi hàm $f \in \mathcal{K}(X, K; \mathbf{C})$, ta có $gf \in \mathcal{K}(X, K; \mathbf{C})$; hơn nữa, nếu $b_K = \sup_{x \in K} |g(x)|$ thì $\|gf\| \leq b_K \|f\|$, do đó mệnh đề của ta (TVS, II, §4, No. 4, Prop. 5). Chuyển vị của ánh xạ tuyến tính liên tục này (TVS, II, §6, No. 4) vì thế là một ánh xạ tuyến tính của $\mathcal{M}(X; \mathbf{C})$ vào chính nó, được ký hiệu là $\mu \mapsto g \cdot \mu$ (hoặc $\mu \mapsto g\mu$, nếu không thể gây nhầm lẫn). Nếu $\nu = g \cdot \mu$ thì do đó, với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$,

$$
\langle f, \nu \rangle = \langle gf, \mu \rangle
$$

hay cũng có thể viết

$$
\int f(x)\, d\nu(x) = \int f(x)g(x)\, d\mu(x)
$$

(được viết tắt dưới dạng $d\nu(x) = g(x)\, d\mu(x)$). Người ta nói rằng $g \cdot \mu$ là tích của độ đo $\mu$ với hàm $g$, hoặc cũng là độ đo có mật độ $g$ đối với $\mu$ (xem Ch. V, §5, No. 2, Def. 2). Nếu $g_1, g_2$ là hai ánh xạ liên tục từ $X$ vào $\mathbf{C}$, và $\mu_1, \mu_2$ là hai độ đo trên $X$, thì

$$
(g_1 + g_2) \cdot \mu = g_1 \cdot \mu + g_2 \cdot \mu, \quad g \cdot (\mu_1 + \mu_2) = g \cdot \mu_1 + g \cdot \mu_2,
$$
$$
(g_1 g_2) \cdot \mu = g_1 \cdot (g_2 \cdot \mu).
$$

Hơn nữa, $1 \cdot \mu = \mu$ (ở đây 1 ký hiệu hàm hằng bằng 1 trên $X$); do đó tập hợp $\mathcal{M}(X; \mathbf{C})$, được trang bị phép toán ngoài hợp thành $(g, \mu) \mapsto g \cdot \mu$ và cấu trúc cộng tính của nó, là một môđun trên vành $\mathcal{C}(X; \mathbf{C})$.

### 5. Độ đo thực. Độ đo dương

Cho X là một không gian địa phương compact. Không gian vectơ thực $\mathcal{K}(X; \mathbf{R})$ là một không gian con của không gian vectơ thực nền của không gian vectơ phức $\mathcal{K}(X; \mathbf{C})$; hơn nữa, ánh xạ $(f_1, f_2) \mapsto f_1 + i f_2$ là một *đẳng cấu* của không gian vectơ tôpô tích $\mathcal{K}(X; \mathbf{R}) \times \mathcal{K}(X; \mathbf{R})$ lên không gian vectơ tôpô thực $\mathcal{K}(X; \mathbf{C})$ (No. 1, Prop. 1).

Với mọi độ đo (phức) $\mu \in \mathcal{M}(X; \mathbf{C})$, hạn chế $\mu_0$ của $\mu$ lên $\mathcal{K}(X; \mathbf{R})$ là một ánh xạ tuyến tính $\mathbf{R}$-liên tục từ $\mathcal{K}(X; \mathbf{R})$ vào $\mathbf{C}$; hơn nữa, hạn chế này xác định $\mu$, vì nếu $f = f_1 + i f_2$ với $f_1, f_2$ thuộc $\mathcal{K}(X; \mathbf{R})$, thì $\mu(f) = \mu_0(f_1) + i \mu_0(f_2)$. Ngược lại, cho $\mu_0$ là một ánh xạ tuyến tính $\mathbf{R}$-liên tục từ $\mathcal{K}(X; \mathbf{R})$ vào $\mathbf{C}$; hiển nhiên ánh xạ

$$
f_1 + i f_2 \mapsto \mu_0(f_1) + i \mu_0(f_2)
$$

là một độ đo (phức) trên X. Do đó, mọi độ đo trên X có thể được đồng nhất với hạn chế của nó lên $\mathcal{K}(X; \mathbf{R})$.

Cho $\mu$ là một độ đo trên X. Ta gọi *độ đo liên hợp* của $\mu$ là độ đo $\overline{\mu}$ được xác định bởi $\overline{\mu}(f) = \overline{\mu(\overline{f})}$ với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$; vì hiển nhiên $\overline{\mu}$ là một dạng tuyến tính C và nó liên tục trên $\mathcal{K}(X; \mathbf{C})$; hiển nhiên $\overline{\mu} = \mu$, và, với hai độ đo $\mu, \nu$ và hai vô hướng $\alpha, \beta$ trong $\mathbf{C}$,

$$
(\alpha \mu + \beta \nu) = \overline{\alpha} \cdot \overline{\mu} + \overline{\beta} \cdot \overline{\nu}.
$$

Nói chung, với mọi hàm $g \in \mathcal{C}(X; \mathbf{C})$ và mọi độ đo $\mu$ trên X,

$$
g \cdot \overline{\mu} = \overline{g} \cdot \overline{\mu},
$$

điều này suy ra ngay lập tức từ định nghĩa (No. 4).

Một độ đo $\mu$ trên X được gọi là *thực* nếu $\overline{\mu} = \mu$; theo điều nói trên, nói như vậy cũng tương đương với việc với mọi hàm $f \in \mathcal{K}(X; \mathbf{R})$, $\mu(f)$ là một số *thực*. Nếu ta đồng nhất một độ đo thực với hạn chế của nó trên $\mathcal{K}(X; \mathbf{R})$, thì do đó có thể nói rằng tập hợp các độ đo thực trên X là *đối ngẫu* của không gian lồi địa phương thực $\mathcal{K}(X; \mathbf{R})$; đó là một không gian vectơ thực, được ký hiệu là $\mathcal{M}(X; \mathbf{R})$ (hoặc đôi khi là $\mathcal{M}(X)$ nếu điều này không gây ra nhầm lẫn nào). Độ đo Lebesgue trên $\mathbf{R}$ là một độ đo *thực*, cũng như độ đo Dirac $\varepsilon_a$ với mọi điểm $a \in X$. Nếu $g \in \mathcal{C}(X; \mathbf{R})$ và nếu $\mu$ là một độ đo thực, thì $g \cdot \mu$ cũng vậy theo (7).

Cho $\mu$ là một độ đo (phức) trên X. Từ định nghĩa trước đó suy ra rằng các độ đo $\mu_1 = (\mu + \overline{\mu})/2$ và $\mu_2 = (\mu - \overline{\mu})/2i$ là *thực*; chúng lần lượt được gọi là *phần thực* và *phần ảo* của $\mu$, và lần lượt được ký hiệu bởi $\mathcal{R}\mu$ và $\mathcal{I}\mu$; các độ đo này còn được đặc trưng bởi tính chất là, với mọi hàm $f \in \mathcal{K}(X; \mathbf{R})$,

$$
\mu_1(f) = \mathcal{R}(\mu(f)) , \quad \mu_2(f) = \mathcal{I}(\mu(f)).
$$

Hiển nhiên
$$
\mu = \mu_1 + i \mu_2,\quad \overline{\mu} = \mu_1 - i \mu_2.
$$

Không gian $\mathcal{K}(X; \mathbf{R})$ gồm các hàm thực liên tục trên $X$ có giá compact hiển nhiên là một *không gian Riesz* đối với quan hệ thứ tự $f \leq g$. Ta sẽ nói rằng một độ đo thực $\mu$ trên $X$ là *dương* nếu $\mu(f) \geq 0$ với mọi hàm $f \geq 0$ thuộc $\mathcal{K}(X; \mathbf{R})$; do đó nó là một dạng tuyến tính dương trên không gian Riesz $\mathcal{K}(X; \mathbf{R})$ (Ch. II, §2, No. 1, Def. 1). Ngược lại:

#### Định lý 1 {#int-iii-s1-thm-1 .statement}

*Mọi dạng tuyến tính dương trên không gian Riesz $\mathcal{K}(X; \mathbf{R})$ đều là một độ đo thực (dương) trên $X$.*

Vì, cho $\mu$ là một dạng tuyến tính dương trên $\mathcal{K}(X; \mathbf{R})$ và cho $K$ là một tập con compắc của $X$. Tồn tại một ánh xạ liên tục $f_0$ từ $X$ vào $[0, 1]$, có giá compact, sao cho $f_0(x) = 1$ trên $K$ (No. 2, Bổ đề 1). Với mọi hàm $g \in \mathcal{K}(X, K; \mathbf{R})$, do đó ta có $-\|g\|f_0 \leq g \leq \|g\|f_0$, do đó $|\mu(g)| \leq \|g\| \cdot \mu(f_0)$, điều này chứng minh định lý.

Ta ký hiệu bởi $\mathcal{M}_+(X)$ nón lồi nhọn của các độ đo dương trên $X$ (hay, điều quy về cùng một điều, nón các dạng tuyến tính dương trên không gian Riesz $\mathcal{K}(X; \mathbf{R})$).

#### Định lý 2 {#int-iii-s1-thm-2 .statement}

*Mọi độ đo thực trên một không gian địa phương compắc $X$ đều là hiệu của hai độ đo dương.*

Xét theo Định lý 1 và Ch. II, §2, No. 2, Th. 1, tất cả quy về việc chứng minh rằng một độ đo thực $\mu$ trên $X$ là một dạng tuyến tính *bị chặn tương đối* trên không gian Riesz $\mathcal{K}(X; \mathbf{R})$. Cho $f$ là một hàm liên tục $\geq 0$ trên $X$, có giá compact $K$; quan hệ $0 \leq g \leq f$ trong $\mathcal{K}(X; \mathbf{R})$ kéo theo $\|g\| \leq \|f\|$ và giá của $g$ được chứa trong $K$. Theo giả thiết, tồn tại một số $M_K \geq 0$ sao cho $|\mu(h)| \leq M_K \cdot \|h\|$ với mọi hàm $h \in \mathcal{K}(X, K; \mathbf{R})$; do đó $|\mu(g)| \leq M_K \cdot \|g\| \leq M_K \cdot \|f\|$, điều này chứng minh định lý.

Do đó, không gian $\mathcal{M}(X; \mathbf{R})$ các độ đo thực trên $X$ đồng nhất với không gian các dạng tuyến tính bị chặn tương đối trên không gian Riesz $\mathcal{K}(X; \mathbf{R})$; ta nhắc lại rằng trong $\mathcal{M}(X; \mathbf{R})$, quan hệ thứ tự $\mu \leq \nu$ có nghĩa là $\nu - \mu$ là một độ đo dương, hay cũng có nghĩa là $\mu(f) \leq \nu(f)$ với mọi hàm $f \in \mathcal{K}_+(X)$.

#### Định lý 3 {#int-iii-s1-thm-3 .statement}

*Không gian $\mathcal{M}(X; \mathbf{R})$ các độ đo thực trên một không gian địa phương compắc $X$ là một dàn đầy đủ.*

Điều này suy ra từ Ch. II, §2, No. 2, Th. 1.

Phù hợp với các ký hiệu của Ch. II, §1, ta định nghĩa, với mọi độ đo *thực* $\mu$ trên $X$,

$$
\mu^+ = \sup(\mu, 0),\quad \mu^- = \sup(-\mu, 0),\quad |\mu| = \sup(\mu, -\mu);
$$

khi đó $\mu = \mu^+ - \mu^-,\ |\mu| = \mu^+ + \mu^-$ và $\inf(\mu^+, \mu^-) = 0$. Hơn nữa, với mọi hàm $f \in \mathcal{K}_+(\mathrm{X})$,

$$
\int f\, d\mu^+ = \sup_{0 \leq g \leq f,\ g \in \mathcal{K}(\mathrm{X})} \int g\, d\mu
$$

và

$$
\int f\, d|\mu| = \sup_{|g| \leq f,\ g \in \mathcal{K}(\mathrm{X})} \int g\, d\mu,
$$

do đó, riêng biệt,

$$
\left| \int f\, d\mu \right| \leq \int |f|\, d|\mu|
$$

với mọi hàm $f \in \mathcal{K}(\mathrm{X}; \mathbf{R})$.

Bất đẳng thức này cũng đúng nếu $f \in \mathcal{K}(\mathrm{X}; \mathbf{C})$; vì, khi nhân $f$ với một số phức có giá trị tuyệt đối bằng $1$ (điều này không làm thay đổi vế nào của bất đẳng thức), ta có thể giả sử rằng $\int f\, d\mu \geq 0$. Khi đó

$$
\left| \int f\, d\mu \right| = \int f\, d\mu = \int (\Re f)\, d\mu \leq \int |\Re f|\, d|\mu| \leq \int |f|\, d|\mu|.
$$

### 6. Giá trị tuyệt đối của một độ đo phức

Cho $\mu$ là một độ đo phức trên một không gian địa phương compắc $\mathrm{X}$; với mọi hàm $f \in \mathcal{K}_+(\mathrm{X})$, số thực dương

$$
L(f) = \sup_{|g| \leq f,\ g \in \mathcal{K}(\mathrm{X}; \mathbf{C})} \left| \int g\, d\mu \right|
$$

là hữu hạn, क्योंकि quan hệ $|g| \leq f$ kéo theo $\operatorname{Supp}(g) \subset \operatorname{Supp}(f)$ và $\|g\| \leq \|f\|$, do đó mệnh đề của chúng ta suy ra từ công thức (4) của No. 3. Hãy chỉ ra rằng $L$ có thể được mở rộng, theo đúng một cách, thành một độ đo dương trên $\mathrm{X}$; xét No. 5, Th. 1 và Ch. II, §2, No. 1, Prop. 3, chỉ cần chỉ ra rằng nếu $f_1,\ f_2$ là hai hàm trong $\mathcal{K}_+(\mathrm{X})$, thì $L(f_1 + f_2) = L(f_1) + L(f_2)$. Bây giờ, nếu $|g_1| \leq f_1$ và $|g_2| \leq f_2$, trong đó $g_1$ và $g_2$ là các hàm trong $\mathcal{K}(\mathrm{X}; \mathbf{C})$, thì ta có $|g_1 + \zeta g_2| \leq f_1 + f_2$ với mọi số phức $\zeta$ có giá trị tuyệt đối bằng 1, do đó

$$
|\mu(g_1 + \zeta g_2)| = |\mu(g_1) + \zeta \mu(g_2)| \leq L(f_1 + f_2).
$$

Hơn nữa, ta có thể giả sử $\zeta$ được chọn sao cho
$$
|\mu(g_1) + \zeta \mu(g_2)| = |\mu(g_1)| + |\mu(g_2)|;
$$
vì $|\mu(g_i)|$ gần tùy ý với $L(f_i)$ ($i = 1, 2$), điều này chứng minh rằng $L(f_1) + L(f_2) \leq L(f_1 + f_2)$. Mặt khác, xét một hàm $g \in \mathcal{K}(X; \mathbf{C})$ sao cho $|g| \leq f_1 + f_2$. Hàm $g_i$ bằng $g f_i/(f_1 + f_2)$ tại các điểm mà $f_1(x) + f_2(x) \neq 0$, và bằng 0 ở những nơi khác ($i = 1, 2$), là liên tục trên X vì $f_i/(f_1 + f_2)$ ($i = 1, 2$) liên tục tại mọi điểm mà $f_1(x) + f_2(x) \neq 0$ và ta có $|g_i(x)| \leq |g(x)|$ với mọi $x \in X$, điều này chứng minh tính liên tục của $g_i$ tại các điểm mà $f_1(x) + f_2(x) = 0$ ($i = 1, 2$), vì tại các điểm ấy ta cũng có $g(x) = 0$. Hiển nhiên là $|g_i| \leq f_i$ ($i = 1, 2$) và $g = g_1 + g_2$, do đó
$$
|\mu(g)| \leq |\mu(g_1)| + |\mu(g_2)| \leq L(f_1) + L(f_2);
$$
vì $|\mu(g)|$ gần tùy ý với $L(f_1 + f_2)$, ta có
$$
L(f_1 + f_2) \leq L(f_1) + L(f_2),
$$
điều này hoàn tất chứng minh mệnh đề của chúng ta.

Khi $\mu$ là một độ đo thực, từ công thức (9) suy ra rằng $|\mu| \leq L$; mặt khác, nhờ phần cuối của No. 5, nếu $g \in \mathcal{K}(X; \mathbf{C})$ và $|g| \leq f \in \mathcal{K}_+(X)$ thì $|\int g \, d\mu| \leq \int |g| \cdot d|\mu| \leq \int f \, d|\mu|$, do đó theo định nghĩa $L \leq |\mu|$, nói cách khác $L = |\mu|$.

Ta lại ký hiệu bởi $|\mu|$ độ đo dương $L$ đối với mọi độ đo phức $\mu$, và ta nói rằng $|\mu|$ là giá trị tuyệt đối của $\mu$. Do đó định nghĩa của $|\mu|$ có thể được viết
$$
|\mu|(f) = \sup_{|g| \leq f,\ g \in \mathcal{K}(X; \mathbf{C})} |\mu(g)|,
$$
do đó, với mọi hàm $g \in \mathcal{K}(X; \mathbf{C})$,
$$
\left| \int g \, d\mu \right| \leq \int |g| \, d|\mu|.
$$

Rõ ràng là với mọi vô hướng $\alpha \in \mathbf{C}$ và mọi độ đo $\mu$ trên $X$,
$$
|\alpha \mu| = |\alpha| \cdot |\mu|.
$$

Mặt khác, nếu $\mu$ và $\nu$ là hai độ đo trên $X$, $f$ là một hàm trong $\mathcal{K}_+(X)$, và $g$ là một hàm trong $\mathcal{K}(X; \mathbf{C})$ sao cho $|g| \leq f$, thì
$$
\left| \int g \, d(\mu + \nu) \right| = \left| \int g \, d\mu + \int g \, d\nu \right| \leq \int f \, d|\mu| + \int f \, d|\nu|,
$$

do đó

$$(15)$$
$$|\mu + \nu| \leq |\mu| + |\nu|.$$

Với cùng các ký hiệu ấy, các quan hệ $|g| \leq f$ và $|\overline{g}| \leq f$ là tương đương, vì vậy

$$(16)$$
$$|\overline{\mu}| = |\mu|.$$

Suy ra từ (14), (15) và (16) rằng

$$(17)$$
$$|\mathcal{R}\mu| \leq |\mu|,\quad |\mathcal{I}\mu| \leq |\mu|,\quad |\mu| \leq |\mathcal{R}\mu| + |\mathcal{I}\mu|.$$

#### Mệnh đề 8 {#int-iii-s1-prop-8 .statement}

*Nếu $\mu$ là một độ đo trên $X$ thì, với mọi hàm $h \in \mathcal{C}(X; \mathbf{C})$,*

$$(18)$$
$$|h \cdot \mu| \leq |h| \cdot |\mu|.$$

Thật vậy, nếu $f \in \mathcal{K}_+(X)$ và nếu $g \in \mathcal{K}(X; \mathbf{C})$ sao cho $|g| \leq f$, thì, theo (13), $|\int gh d\mu| \leq \int |gh| d|\mu| \leq \int f|h| d|\mu|$, điều này chứng minh (18).

### 7. Định nghĩa một độ đo bằng mở rộng

Cho $X$ là một không gian compact địa phương; nếu $V$ là một không gian con tuyến tính *trù mật* của $\mathcal{K}(X; \mathbf{C})$, thì rõ ràng là hai độ đo $\mu_1, \mu_2$ trên $X$ trùng nhau trên $V$ thì bằng nhau, và mọi dạng tuyến tính trên $V$ liên tục đối với tôpô cảm sinh bởi tôpô của $\mathcal{K}(X; \mathbf{C})$ đều có thể được mở rộng (chỉ theo một cách) thành một độ đo trên $X$. Đối với các độ đo dương, một tiêu chuẩn thuận tiện là như sau:

#### Mệnh đề 9 {#int-iii-s1-prop-9 .statement}

*Cho $V$ là một không gian con tuyến tính của $\mathcal{K}(X; \mathbf{R})$ có tính chất sau:
(P) Với mọi tập con compact $K$ của $X$, tồn tại một hàm $f \in V$ sao cho $f \geq 0$ và $f(x) > 0$ với mọi $x \in K$.
Trong các điều kiện ấy, mọi dạng tuyến tính dương trên $V$ đối với thứ tự cảm sinh bởi thứ tự của $\mathcal{K}(X; \mathbf{R})$ (Ch. II, §2, No. 1, Định nghĩa 1) đều có thể được mở rộng thành một độ đo dương trên $X$ (độ đo này là duy nhất khi $V$ trù mật trong $\mathcal{K}(X; \mathbf{R})$).
Với mọi hàm $f \in \mathcal{K}(X; \mathbf{R})$, có giá là $K$, tồn tại một hàm $g \in V$ sao cho $f \leq g$; thật vậy, tồn tại một hàm $h \geq 0$ trong $V$ sao cho $h(x) > 0$ với mọi $x \in K$; đặt $\alpha = \inf_{x \in K} h(x)$, do đó ta có $\alpha > 0$ và hàm $g = (\alpha^{-1} \|f\|)h$ thỏa mãn yêu cầu. Khi đó chỉ cần áp dụng Định lý 1 của No. 5 và Mệnh đề 1 của TVS, II, §3, No. 1.*

### 8. Độ đo bị chặn

Cho X là một không gian compact địa phương. Vì tôpô trên $\mathcal{K}(X; \mathbf{C})$ cảm sinh bởi tôpô của $\mathcal{C}^b(X; \mathbf{C})$ là thô hơn tôpô giới hạn trực tiếp trên $\mathcal{K}(X; \mathbf{C})$, nên một độ đo trên X không nhất thiết liên tục đối với tôpô hội tụ đều trên X.

#### Định nghĩa 3 {#int-iii-s1-def-3 .statement}

*Một độ đo trên một không gian compact địa phương X được gọi là bị chặn nếu nó liên tục trên $\mathcal{K}(X; \mathbf{C})$ đối với tôpô hội tụ đều.*

Điều đó tương đương với việc nói rằng tồn tại một số hữu hạn $M \geq 0$ sao cho, với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$,

$$
|\mu(f)| \leq M \|f\|
$$

(trong đó $\|f\|$ được xác định bởi công thức (3) của No. 2).

Như vậy, nói rằng $\mu$ là một độ đo bị chặn có nghĩa là $\mu$ thuộc đối ngẫu của không gian $\mathcal{K}(X; \mathbf{C})$ được chuẩn hóa bởi $\|f\|$; ta sẽ ký hiệu đối ngẫu này bởi $\mathcal{M}^1(X; \mathbf{C})$ (hoặc đơn giản là $\mathcal{M}^1(X)$ khi không thể có sự lẫn lộn). Ta biết rằng $\mathcal{M}^1(X; \mathbf{C})$ được trang bị một chuẩn, $\|\mu\|$ là số nhỏ nhất trong các số $M \geq 0$ mà với chúng bất đẳng thức (19) đúng với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$, hay cũng vậy,

$$
\|\mu\| = \sup_{\|f\| \leq 1,\ f \in \mathcal{K}(X; \mathbf{C})} |\mu(f)| .
$$

Được trang bị chuẩn này, $\mathcal{M}^1(X; \mathbf{C})$ được biết là một không gian Banach (TVS, III, §3, No. 8, Hệ quả 2 của Mệnh đề 12).

Định nghĩa của $\|\mu\|$ bằng công thức (20) có thể được mở rộng cho mọi độ đo $\mu$ trên X và, do lạm dụng ngôn ngữ, $\|\mu\|$ lại được gọi là chuẩn của $\mu$; để $\mu$ bị chặn, điều kiện cần và đủ là $\|\mu\|$ hữu hạn.

Nếu X compact, thì mọi độ đo trên X đều bị chặn.

#### Ví dụ {#int-iii-s1-n8-exa-1 .statement}

— 1) Độ đo $\varepsilon_a$ được xác định bởi một khối lượng đơn vị tại một điểm $a \in X$ là bị chặn, và $\|\varepsilon_a\| = 1$.

2) Độ đo Lebesgue trên $\mathbf{R}$ không bị chặn; thực vậy, với mọi số nguyên $n > 0$ tồn tại một hàm $f \in \mathcal{K}(\mathbf{R}; \mathbf{C})$ nhận giá trị trong $[0, 1]$ và bằng 1 trên khoảng $[ -n, n ]$ (No. 2, Bổ đề 1); do đó $\|f\| = 1$ và

$$
\int_{-\infty}^{+\infty} f(x)\, dx \geq \int_{-n}^{n} f(x)\, dx = 2n ,
$$

điều này chứng tỏ rằng không tồn tại số hữu hạn nào M thỏa mãn quan hệ (19).

3) Trên đường thẳng thực $\mathbf{R}$$, ánh xạ

$$
f \mapsto \int_{-\infty}^{+\infty} \frac{f(x)\,dx}{1 + x^2}
$$

là một độ đo bị chặn vì, với mọi hàm $f \in \mathcal{H}(\mathbf{R}; \mathbf{C})$,

$$
\left| \int_{-\infty}^{+\infty} \frac{f(x)\,dx}{1 + x^2} \right| \leq \|f\| \int_{-\infty}^{+\infty} \frac{dx}{1 + x^2} = \pi \cdot \|f\|.
$$

Vì các quan hệ $\|f\| \leq 1$ và $\|\overline{f}\| \leq 1$ là tương đương, suy ra từ (20) rằng

(21)
$$
\|\overline{\mu}\| = \|\mu\|
$$
đối với mọi độ đo $\mu$ trên $X$.

#### Mệnh đề 10 {#int-iii-s1-prop-10 .statement}

— *Đối với mọi độ đo $\mu$ trên $X$*,

(22)
$$
\|\mu\| = \sup_{0 \leq f \leq 1,\ f \in \mathcal{H}(X; \mathbf{R})} |\mu|(f).
$$

Thật vậy, có kể đến công thức (12) dùng để xác định giá trị tuyệt đối của một độ đo, vế thứ hai của (22) có thể viết thành

$$
\sup_{0 \leq f \leq 1,\ f \in \mathcal{H}(X; \mathbf{R})} \left( \sup_{|g| \leq f,\ g \in \mathcal{H}(X; \mathbf{C})} |\mu(g)| \right) = \sup_{\|g\| \leq 1,\ g \in \mathcal{H}(X; \mathbf{C})} |\mu(g)|.
$$

#### Hệ quả 1 {#int-iii-s1-prop-10-cor-1 .statement}

— *Đối với mọi độ đo $\mu$ trên $X$, các chuẩn của $\mu$ và $|\mu|$ bằng nhau; $\mu$ bị chặn khi và chỉ khi $|\mu|$ bị chặn.*

#### Hệ quả 2 {#int-iii-s1-prop-10-cor-2 .statement}

— *Đối với mọi độ đo $\mu$ trên một không gian compact $X$*,

(23)
$$
\|\mu\| = |\mu|(1) = \int d|\mu|.
$$

Công thức này sẽ được tổng quát hóa trong Ch. IV, §4, No. 7.

Trên một không gian *compact* $X$, đối với mọi độ đo (phức) $\mu$ trên $X$, số phức $\mu(1)$ được gọi là *khối lượng toàn phần* của $\mu$. Khi $\mu$ là *dương*, khối lượng toàn phần của nó do đó bằng chuẩn của nó. Khi $\mu$ là một độ đo dương trên một không gian *compact* $X$, có khối lượng toàn phần bằng 1, người ta cũng nói rằng giá trị $\mu(f)$ của nó đối với một hàm liên tục $f \in \mathcal{C}(X; \mathbf{C})$ là *trung bình* của $f$ đối với độ đo $\mu$.

#### Hệ quả 3 {#int-iii-s1-prop-10-cor-3 .statement}

— Đối với mọi độ đo thực $\mu$ trên một không gian địa phương compact $X$,

$$
\| \mu \| = \sup_{\| f \| \leq 1,\ f \in \mathcal{K}(X; \mathbf{R})} | \mu(f) | .
$$

Chỉ cần dùng công thức (22) và biểu thức (9) của $|\mu|(f)$ khi $\mu$ là một độ đo thực và $f \in \mathcal{K}_+(X)$.

Do đó, tập hợp các độ đo thực bị chặn là đối ngẫu của không gian chuẩn $\mathcal{K}(X; \mathbf{R})$; nó được ký hiệu là $\mathcal{M}^1(X, \mathbf{R})$, hoặc $\mathcal{M}^1(X)$ nếu không thể có sự nhầm lẫn. Đơn ánh chính tắc $\mathcal{M}^1(X, \mathbf{R}) \to \mathcal{M}^1(X; \mathbf{C})$ là một đẳng cự theo (24).

#### Mệnh đề 11 {#int-iii-s1-prop-11 .statement}

— Nếu $\mu$ và $\nu$ là hai độ đo dương trên $X$, thì $\| \mu + \nu \| = \| \mu \| + \| \nu \|$.

Thật vậy, các hàm $f \in \mathcal{K}(X; \mathbf{R})$ sao cho $0 \leq f \leq 1$ tạo thành một tập có hướng $S$ đối với quan hệ $\leq$. Do đó, đối với một độ đo dương $\mu$ trên $X$, từ (22) và định lý giới hạn đơn điệu suy ra rằng $\| \mu \| = \lim_{f \in S} \mu(f)$; kết luận của mệnh đề khi đó suy ra ngay.

#### Hệ quả 1 {#int-iii-s1-prop-11-cor-1 .statement}

— Nếu $\mu$ và $\nu$ là hai độ đo dương trên $X$ sao cho $\mu \leq \nu$, thì $\| \mu \| \leq \| \nu \|$; đặc biệt, nếu $\nu$ bị chặn thì $\mu$ cũng vậy.
Thật vậy, $\| \nu \| = \| \mu \| + \| \nu - \mu \|$.

#### Hệ quả 2 {#int-iii-s1-prop-11-cor-2 .statement}

— Với mọi độ đo thực $\mu$ trên $X$,

$$
\| \mu \| = \| \mu^+ \| + \| \mu^- \|.
$$

Theo (Hệ quả 1 của Mệnh đề 10), chuẩn của $\mu$ bằng chuẩn của $|\mu| = \mu^+ + \mu^-$.

#### Mệnh đề 12 {#int-iii-s1-prop-12 .statement}

— Nếu $\mu$ là một độ đo bị chặn trên $X$ và nếu $g$ là một ánh xạ liên tục bị chặn từ $X$ vào $\mathbf{C}$, thì độ đo $g \cdot \mu$ bị chặn và $\| g \cdot \mu \| \leq \| g \| \cdot \| \mu \|$.

Với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$,

$$
|\mu(fg)| \leq \| \mu \| \cdot \| fg \| \leq \| \mu \| \cdot \| g \| \cdot \| f \|.
$$

### 9. Tôpô mờ trên không gian các độ đo

Cho $X$ là một không gian compact địa phương. Trên không gian $\mathcal{M}(X; \mathbf{C})$, ta có thể xét tôpô hội tụ điểm trên $\mathcal{K}(X; \mathbf{C})$, mà ta sẽ gọi là tôpô mờ trên $\mathcal{M}(X; \mathbf{C})$.

Vì $\mathcal{K}(X; \mathbf{C}) = \mathcal{K}(X; \mathbf{R}) + i \mathcal{K}(X; \mathbf{R})$, tôpô mờ trên $\mathcal{M}(X; \mathbf{C})$ được xác định bởi các *nửa chuẩn* $\sup_{1 \leq i \leq n} |\mu(f_i)|$, trong đó $(f_i)_{1 \leq i \leq n}$ là một dãy hữu hạn bất kỳ các hàm trong $\mathcal{K}(X; \mathbf{R})$ (hoặc trong $\mathcal{K}_+(X)$). Nói rằng một bộ lọc $\mathfrak{F}$ trên $\mathcal{M}(X; \mathbf{C})$ *hội tụ mờ* tới một độ đo $\mu_0$ có nghĩa là

$$
\mu_0(f) = \lim_{\mu, \mathfrak{F}} \mu(f)
$$

với mọi hàm $f \in \mathcal{K}(X; \mathbf{R})$. Với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$, ánh xạ $\mu \mapsto \mu(f)$ là một dạng tuyến tính *liên tục đối với tôpô mờ* trên không gian $\mathcal{M}(X; \mathbf{C})$.

#### Mệnh đề 13 {#int-iii-s1-prop-13 .statement}

*Cho X là một không gian compact địa phương và, với mọi $x \in X$, ký hiệu $\varepsilon_x$ là độ đo Dirac tại điểm x. Ánh xạ $x \mapsto \varepsilon_x$ là một đồng phôi từ X lên một không gian con của không gian $\mathcal{M}(X; \mathbf{C})$ các độ đo trên X, được trang bị tôpô mờ. Hơn nữa, nếu $X'$ ký hiệu không gian compact thu được bằng cách thêm vào X một điểm ở vô cực $\omega$, thì $\varepsilon_x$ tiến tới 0 khi x tiến tới $\omega$.*

Với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$, $\langle f, \varepsilon_x \rangle = f(x)$; vì $f$ liên tục, điều này chứng tỏ rằng ánh xạ $x \mapsto \varepsilon_x$ là liên tục. Nếu $x, y$ là hai điểm phân biệt của X, thì tồn tại một hàm $f \in \mathcal{K}(X; \mathbf{C})$ sao cho $f(x) = 1, f(y) = 0$ (No. 2, Bổ đề 1), điều này chứng tỏ rằng $\varepsilon_x \neq \varepsilon_y$; do đó ánh xạ $x \mapsto \varepsilon_x$ là đơn ánh. Hơn nữa, với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$, $\langle f, \varepsilon_x \rangle$ tiến tới 0 theo định nghĩa khi $x$ tiến tới $\omega$, do đó $x \mapsto \varepsilon_x$ có thể được mở rộng liên tục lên $X' = X \cup \{ \omega \}$ bằng cách gán cho nó giá trị 0 tại điểm $\omega$. Ánh xạ mở rộng này cũng là đơn ánh, vì $\varepsilon_x \neq 0$ với mọi $x \in X$. Vậy nó là một đồng phôi của không gian compact $X'$ lên một không gian con của $\mathcal{M}(X; \mathbf{C})$, vì $\mathcal{M}(X; \mathbf{C})$ là Hausdorff đối với tôpô vague (GT, I, §9, No. 4, Hệ quả 2 của Định lý 2).

#### Mệnh đề 14 {#int-iii-s1-prop-14 .statement}

*Trong không gian $\mathcal{M}(X; \mathbf{C})$ các độ đo trên một không gian địa phương compact X, nón $\mathcal{M}_+(X)$ các độ đo dương là đầy đủ đối với cấu trúc đều suy ra từ tôpô vague* (do đó *đóng theo tôpô vague* trong $\mathcal{M}(X; \mathbf{C})$).

Thật vậy, xét một bộ lọc Cauchy $\Phi$ đối với cấu trúc đều vague trên $\mathcal{M}_+(X)$; theo định nghĩa, $\mu_0(f) = \lim_{\mu, \Phi} \mu(f)$ tồn tại với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$ và, theo nguyên lý mở rộng các bất đẳng thức, $\mu_0(f) \geq 0$ với mọi hàm $f \in \mathcal{K}_+(X)$; suy ra $\mu_0$ là một độ đo dương trên X (No. 5, Th. 1).

Cần lưu ý rằng chính không gian $\mathcal{M}(X; \mathbf{C})$ (hoặc $\mathcal{M}(X; \mathbf{R})$) *không nhất thiết là đầy đủ* đối với cấu trúc đều vague (TVS, II, §6, No. 7).

#### Hệ quả {#int-iii-s1-n9-cor-1 .statement}

*Nếu A và B là hai tập con đóng theo tôpô vague của $\mathcal{M}_+(X)$, thì $A + B$ đóng theo tôpô vague trong $\mathcal{M}_+(X)$ (do đó cũng đóng trong $\mathcal{M}(X; \mathbf{C})$).*

Đây वास्तव ra là một tính chất tổng quát của các nón đầy đủ yếu, thực sự trong các không gian lồi địa phương (TVS, II, §6, No. 8, Hệ quả 2 của Mệnh đề 11).

#### Mệnh đề 15 {#int-iii-s1-prop-15 .statement}

— Cho $H$ là một tập con của $\mathcal{M}(X; \mathbf{C})$. Các tính chất sau là tương đương:

a) $H$ bị chặn theo tôpô vague.
b) $H$ tương đối compact theo tôpô vague.
c) $H$ đồng liên tục.
d) Với mọi tập con compact $K$ của $X$, tồn tại một số $M_K \geq 0$ sao cho $|\mu(f)| \leq M_K \|f\|$ với mọi độ đo $\mu \in H$ và mọi hàm $f \in \mathcal{K}(X, K; \mathbf{C})$.

Vì $\mathcal{K}(X; \mathbf{C})$ là một không gian chặn-thùng (No. 1, Prop. 2), tính tương đương của các tính chất a), b) và c) suy ra từ TVS, III, §4, No. 1, Chú giải.

Hiển nhiên là d) kéo theo a). Cuối cùng, nếu $H$ đồng liên tục thì tập các hạn chế của các độ đo $\mu \in H$ lên $\mathcal{K}(X, K; \mathbf{C})$ cũng đồng liên tục, do đó có điều kiện d), vì $\mathcal{K}(X, K; \mathbf{C})$ là một không gian định chuẩn.

\* Ta sẽ thấy trong Ch. IV, §4, No. 6 rằng các điều kiện của Mệnh đề 15 cũng tương đương với điều kiện sau đây: với mọi tập con compact $K$ của $X$, tồn tại một hằng $M_K$ sao cho $|\mu|(K) \leq M_K$ với mọi độ đo $\mu \in H$.*

#### Hệ quả 1 {#int-iii-s1-prop-15-cor-1 .statement}

— Cho $\nu$ là một độ đo dương trên $X$; tập hợp các độ đo $\mu$ sao cho $|\mu| \leq \nu$ là compact theo tôpô mờ.

#### Hệ quả 2 {#int-iii-s1-prop-15-cor-2 .statement}

— Tập hợp các độ đo $\mu$ sao cho $\|\mu\| \leq a$ ($a$ là một số hữu hạn bất kỳ $> 0$) là compact theo tôpô mờ.

#### Hệ quả 3 {#int-iii-s1-prop-15-cor-3 .statement}

— Nếu $X$ compact, tập hợp các độ đo dương $\mu$ trên $X$ sao cho $\|\mu\| = 1$ là compact theo tôpô mờ.

Thật vậy, đó là giao của tập compact theo tôpô mờ (Hệ quả 2) gồm các độ đo sao cho $\|\mu\| \leq 1$ và các tập đóng đối với tôpô mờ được xác định tương ứng bởi các hệ thức $\mu \geq 0$ và $\mu(1) = 1$ (No. 8, Hệ quả 2 của Mệnh đề 10).

#### Hệ quả 4 {#int-iii-s1-prop-15-cor-4 .statement}

— Trong không gian $\mathcal{M}(X; \mathbf{C})$, ánh xạ $\mu \mapsto \|\mu\|$ là nửa liên tục dưới đối với tôpô mờ.

Đây là một hệ quả ngay lập tức của Hệ quả 2.

Cần lưu ý rằng ánh xạ $\mu \mapsto |\mu|$ từ $\mathcal{M}(X; \mathbf{C})$ vào chính nó không nhất thiết liên tục đối với tôpô mờ (Bài tập 9).

#### Mệnh đề 16 {#int-iii-s1-prop-16 .statement}

— Cho $K$ là một tập con compact của $X$, $H$ là một tập con bị chặn đối với tôpô mờ của $\mathcal{M}(X; \mathbf{C})$; khi đó, dạng song tuyến tính $(f, \mu) \mapsto \langle f, \mu \rangle$ là liên tục trên $\mathcal{K}(X, K; \mathbf{C}) \times H$ khi $\mathcal{K}(X, K; \mathbf{C})$ được trang bị tôpô hội tụ đều và $H$ được trang bị tôpô mờ.

Thật vậy, tồn tại một số $M \geqslant 0$ sao cho
$$
|\mu(f)| \leqslant M \|f\|
$$
với mọi hàm $f \in \mathcal{K}(X, K; \mathbf{C})$ và mọi độ đo $\mu \in H$ (Mệnh đề 15). Nếu $\mu_0$ và $\mu$ là hai độ đo thuộc $H$, $f_0$ và $f$ là hai hàm trong $\mathcal{K}(X, K; \mathbf{C})$, thì
$$
|\mu(f) - \mu_0(f_0)| = |\mu(f - f_0) + \mu(f_0) - \mu_0(f_0)| \\
\leqslant M \|f - f_0\| + |\mu(f_0) - \mu_0(f_0)|,
$$
và đại lượng cuối cùng nhỏ tùy ý khi $\|f - f_0\|$ và $|\mu(f_0) - \mu_0(f_0)|$ nhỏ tùy ý, điều đó chứng minh mệnh đề.

### 10. Hội tụ compact trong $\mathcal{M}(X; \mathbf{C})$

Nhắc lại rằng tôpô của *hội tụ compact* trên $\mathcal{M}(X; \mathbf{C})$ là tôpô của hội tụ đều trên các tập con compact của $\mathcal{K}(X; \mathbf{C})$. Ta sẽ gọi *tôpô của hội tụ compact chặt* trên $\mathcal{M}(X; \mathbf{C})$ là tôpô của hội tụ đều trên các tập con compact chặt (No. 1) của $\mathcal{K}(X; \mathbf{C})$.

#### Mệnh đề 17 {#int-iii-s1-prop-17 .statement}

*Trên không gian $\mathcal{M}(X; \mathbf{C})$, xét các tôpô sau:*
$\mathcal{T}_1$: *tôpô của hội tụ từng điểm trên một tập con toàn phần T của $\mathcal{K}(X; \mathbf{C})$;*
$\mathcal{T}_2$: *tôpô mờ;*
$\mathcal{T}_3$: *tôpô của hội tụ compact chặt;*
$\mathcal{T}_4$: *tôpô của hội tụ compact.*
*Mỗi tôpô trong các tôpô này đều thô hơn tôpô kế tiếp. Hơn nữa:*
*(i)* *Các tập bị chặn là như nhau đối với $\mathcal{T}_2$, $\mathcal{T}_3$ và $\mathcal{T}_4$.*
*(ii)* *Nếu H là một tập con bị chặn đối với tôpô mờ của $\mathcal{M}(X; \mathbf{C})$, thì các tôpô cảm sinh trên H bởi các tôpô $\mathcal{T}_1$, $\mathcal{T}_2$, $\mathcal{T}_3$, $\mathcal{T}_4$ là trùng nhau.*

Một tập con bị chặn mơ hồ $H$ của $\mathcal{M}(X; \mathbf{C})$ là đồng liên tục (No. 9, Prop. 15), do đó mệnh đề thứ nhất suy ra từ EVT, III, §3, No. 7, Prop. 9, và mệnh đề thứ hai suy ra từ GT, X, §2, No. 4, Định lý 1.

Nhắc lại rằng khi $X$ là *paracompact*, tôpô của sự hội tụ compắc chặt trùng với tôpô của sự hội tụ compắc (No. 1, Prop. 2).

#### Mệnh đề 18 {#int-iii-s1-prop-18 .statement}

*Trên nón $\mathcal{M}_+(X)$, các tôpô cảm sinh bởi các tôpô sau đây trùng nhau:*
$\mathcal{T}_1$: *tôpô của sự hội tụ từng điểm trong một không gian con tuyến tính V của $\mathcal{K}(X; \mathbf{C})$ trù mật trong $\mathcal{K}(X; \mathbf{C})$ và thỏa mãn tính chất (P) (No. 7, Prop. 9);*

\textit{\mathcal{T}_2: tôpô mơ hồ;}

\textit{\mathcal{T}_3: tôpô của sự hội tụ compắc chặt.}

Vì mọi bộ lọc đều là giao của các siêu bộ lọc mịn hơn nó (GT, I, §6, No. 4, Prop. 7), nên chỉ cần chỉ ra rằng nếu $\mathfrak{U}$ là một siêu bộ lọc trên $\mathcal{M}_+(X)$ hội tụ tới một độ đo $\mu_0$ đối với tôpô $\mathcal{T}_1$, thì nó cũng hội tụ tới $\mu_0$ đối với $\mathcal{T}_3$. Cho $K$ là một tập con compắc của $X$; theo giả thiết, tồn tại một hàm $h \in V$ sao cho $\geqslant 0$ trên $X$ và nhận các giá trị $> 0$ trên $K$; suy ra rằng mọi hàm $f \in \mathcal{K}(X, K; \mathbf{C})$ đều có thể viết thành $f = gh$ với $g \in \mathcal{K}(X, K; \mathbf{C})$, và nếu $c = \inf_{x \in K} h(x) > 0$ thì $\|g\| \leqslant c^{-1}\|f\|$. Theo giả thiết, tồn tại một tập hợp $H_0 \in \mathfrak{U}$ sao cho, với mọi độ đo $\mu \in H_0$,

$$
0 \leqslant \mu(h) \leqslant \mu_0(h) + 1 = b.
$$

Do đó, với mọi hàm $f \in \mathcal{K}(X; \mathbf{C})$,

$$
|\langle f, h \cdot \mu \rangle| = |\langle hf, \mu \rangle| \leqslant \|f\| \cdot \mu(h) \leqslant b \|f\|
$$

với mọi độ đo $\mu \in H_0$; điều này chứng minh rằng tập hợp $H$ các độ đo $h \cdot \mu$, trong đó $\mu$ chạy khắp $H_0$, là \emph{bị chặn mơ hồ}. Nếu $\mathfrak{U}_0$ là siêu bộ lọc cảm sinh bởi $\mathfrak{U}$ trên $H_0$, thì ảnh của $\mathfrak{U}_0$ qua ánh xạ $\mu \mapsto h \cdot \mu$ là cơ sở của một siêu bộ lọc $\mathfrak{F}$ trên $H$, và vì $H$ là tương đối compắc đối với tôpô của sự hội tụ compắc chặt (Prop. 17 and No. 9, Prop. 15), $\mathfrak{F}$ hội tụ tới một độ đo $\nu_0$ đối với tôpô này. Nói cách khác, với mọi $\varepsilon > 0$ và mọi tập con compắc $L$ của $\mathcal{K}(X, K; \mathbf{C})$, tồn tại một tập con $N$ của $H_0$ thuộc $\mathfrak{U}$ sao cho, với mọi hàm $g \in L$ và mọi cặp độ đo $\mu, \mu'$ thuộc $N$, ta có $|\langle g, h \cdot \mu \rangle - \langle g, h \cdot \mu' \rangle| \leqslant \varepsilon$, tức là,

$$
|\langle gh, \mu \rangle - \langle gh, \mu' \rangle| \leqslant \varepsilon.
$$

Bây giờ, như đã thấy ở trên, ánh xạ $g \mapsto gh$ là một \emph{tự đẳng cấu} của không gian Banach $\mathcal{K}(X, K; \mathbf{C})$. Vậy ta đã chứng minh rằng $\mathfrak{U}$ là một \emph{bộ lọc Cauchy} trên $\mathcal{M}_+(X)$ đối với tôpô hội tụ compáct chặt. \emph{A fortiori}, nó là một bộ lọc Cauchy đối với hội tụ mờ, và Mệnh đề 14 của No. 9 cho thấy rằng nó hội tụ mờ đến một độ đo $\mu_1$; hơn nữa, vì $V$ trù mật trong $\mathcal{K}(X; \mathbf{C})$, giả thiết kéo theo $\mu_1 = \mu_0$; sau hết, vì $\mathfrak{U}$ là một bộ lọc Cauchy đối với tôpô hội tụ compáct chặt, nó cũng hội tụ đến $\mu_0$ theo tôpô này (GT, X, §1, No. 5, Prop. 5).

Điều phải chứng minh.

#### Hệ quả {#int-iii-s1-n10-cor-1 .statement}

— *Nếu X là paracompact thì các tôpô cảm sinh trên $\mathcal{M}_+(X)$ bởi tôpô mờ và tôpô hội tụ compáct là trùng nhau.*

Tuy nhiên, các tôpô cảm sinh trên $\mathcal{M}_+(X)$ bởi tôpô hội tụ compáct và tôpô hội tụ compáct chặt có thể khác nhau khi X không paracompact (Bài tập 3).

### Bài tập {#int-iii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
