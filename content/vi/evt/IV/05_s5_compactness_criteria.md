---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 5
section_title: Compactness criteria
lang: vi
source: evt-i-v
book_pages: TVS IV.32-TVS IV.38, TVS IV.67-TVS IV.71
pdf_pages: 0214-0220, 0249-0253
extraction: ocr
subsections:
    - "no": 1
      title: General remarks
      page: 32
      pdf_page: 214
    - "no": 2
      title: Simple compactness of sets of continuous functions
      page: 33
      pdf_page: 215
    - "no": 3
      title: The Eberlein and Šmulian theorems
      page: 35
      pdf_page: 217
    - "no": 4
      title: The case of spaces of bounded continuous functions*
      page: 36
      pdf_page: 218
    - "no": 5
      title: Convex envelope of a weakly compact set
      page: 37
      pdf_page: 219
statements: 8
exercises: 18
content_sha256: 7ed8812d2f5b1d7e282558e3f425040ac7523654371e779a2bac9789b3a0bdc4
translated_from: content/en/evt/IV/05_s5_compactness_criteria.md
source_content_sha256: 74acd4eb366456136b6614676effa587ce4c4fa1a461711a3f53b2c158904c50
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-659a8e67
glossary_version: 34
glossary_terms_sha256: 7a5d3a55190fa97aec2bdad72c890c7e12f1eeea8b1a2f26da5ea15a9aa177bb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC TIÊU CHUẨN VỀ TÍNH COMPACT

### 1. Các nhận xét chung

Cho A là một tập con của một không gian tôpô E. Để một dãy $(x_n)_{n \in \mathbf{N}}$ các điểm của A có một điểm x của E làm điểm giới hạn, điều kiện cần và đủ là điều kiện sau được thỏa mãn (GT, I, § 7, No. 3) :

(A) Với mọi số nguyên $m \geq 0$ và mọi lân cận U của x, tồn tại một số nguyên $n \geq m$ sao cho $x_n \in U$.

Một dãy có dạng $(y_k)_{k \in \mathbf{N}}$ với $y_k = x_{n_k}$ đối với một dãy tăng ngặt $(n_k)_{k \in \mathbf{N}}$ các số nguyên dương được gọi là một dãy trích xuất của dãy $(x_n)_{n \in \mathbf{N}}$. Nếu tồn tại một dãy trích xuất của dãy $(x_n)_{n \in \mathbf{N}}$ hội tụ đến x, thì x là một điểm giới hạn của $(x_n)$; đảo lại, nếu x có một hệ cơ bản đếm được các lân cận, và x là điểm giới hạn của dãy $(x_n)$, thì tồn tại một dãy trích xuất của $(x_n)$ hội tụ đến x.

Theo GT, IX, § 2, No. 9, hệ quả, ta kết luận rằng khi E mêtric hóa được, các điều kiện sau là tương đương :
a) tập hợp A là compact tương đối trong E ;
b) mọi dãy vô hạn các điểm của A đều có một điểm giới hạn trong E ;
c) từ mọi dãy vô hạn các điểm của A, ta có thể trích xuất một dãy hội tụ đến một điểm của E.

Trong mục này, ta sẽ mở rộng tiêu chuẩn này đến một số không gian vectơ tôpô không mêtric hóa được. Mệnh đề sau cho phép ta rút gọn việc nghiên cứu các tập compact về việc nghiên cứu các tập compact yếu trong một số trường hợp.

#### Mệnh đề 1 {#evt-iv-s5-prop-1 .statement}

— Cho E là một không gian lồi địa phương Hausdorff, và A là một tập con của E. Ký hiệu $E_\sigma$ là không gian E với tôpô yếu hơn.
a) Nếu mọi dãy vô hạn các điểm của A đều có một điểm giới hạn trong E, thì A là tiềncompact trong E.
b) Để A là compact tương đối trong E, điều kiện cần và đủ là A tiềncompact trong E và compact tương đối trong $E_\sigma$.

Ta sẽ chứng minh a) bằng phản chứng. Nếu A không tiềncompact, thì theo định lý 3 của GT, II, § 3, No. 7, suy ra rằng tồn tại một lân cận lồi đối xứng V của 0 trong E sao cho A không thể được phủ bởi một số hữu hạn các phép tịnh tiến của V.

Nói cách khác, nếu $x_0, x_1, ..., x_{n-1}$ là các điểm của A, thì $A \notin \bigcup_{0 \leq i < n} (x_i + V)$ và do đó tồn tại một điểm $x_n$ của A sao cho $x_n - x_i \notin V$ với $0 \leq i < n$. Khi đó, bằng quy nạp theo số nguyên $n$, ta có thể xây dựng một dãy vô hạn $(x_n)_{n \in \mathbf{N}}$ các điểm của A sao cho $x_n - x_m \notin V$ bất cứ khi nào $n > m$; vì V đối xứng, ta cũng có $x_m - x_n \notin V$ với $m \neq n$ và các tập hợp $x_n + \frac{1}{2} V$ rời nhau. Với mọi điểm $x$ trong E, tồn tại nhiều nhất một số nguyên $n \geq 0$ sao cho $x_n \in x + \frac{1}{2} V$, do đó dãy $(x_n)_{n \in \mathbf{N}}$ không có điểm giới hạn nào. Điều này chứng minh *a)*.

Bây giờ giả sử rằng A tiềncompact trong E và được chứa trong một tập compact B của $E_\sigma$. Khi đó B đầy đủ trong $E_\sigma$, do đó cũng đầy đủ trong E (IV, p. 5, *Nhận xét 2*). Ta có $\overline{A} \subset B$, do đó A compact tương đối trong E. Điều đảo lại là hiển nhiên và *b)* được suy ra.

### 2. Tính compact đơn giản của các tập hợp hàm liên tục

Trong mục này, X ký hiệu một không gian *compact* và $\mathcal{C}_s(X)$ là không gian các hàm liên tục trên X, nhận các giá trị trong trường K (bằng $\mathbf{R}$ hoặc $\mathbf{C}$). Không gian $\mathcal{C}_s(X)$ được trang bị tôpô hội tụ đơn giản trên X.

#### Mệnh đề 2 {#evt-iv-s5-prop-2 .statement}

*Cho D là một tập con trù mật của X và A là một tập con của không gian $\mathcal{C}_s(X)$. Các điều kiện sau là tương đương :*
(i) *A là compact tương đối trong $\mathcal{C}_s(X)$.*
(ii) *Từ mọi dãy vô hạn các phần tử của A, ta có thể trích xuất một dãy hội tụ trong $\mathcal{C}_s(X)$.*
(iii) *Mọi dãy vô hạn các phần tử của A đều có một điểm giới hạn trong $\mathcal{C}_s(X)$.*
(iv) *Cho $(f_n)_{n \in \mathbf{N}}$ là một dãy các hàm thuộc A và $(x_m)_{m \in \mathbf{N}}$ là một dãy các điểm của D. Nếu các giới hạn lặp*

$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$

*tồn tại, thì chúng bằng nhau. Ngoài ra, ta có $\sup_{f \in A} |f(x)| < + \infty$ với mọi $x \in X$.*

(i) $\Rightarrow$ (ii) : đặt $\overline{A}$ là bao đóng của A trong $\mathcal{C}_s(X)$. Giả sử rằng A là compact, và xét một dãy các hàm $f_n \in A$ (với $n \in \mathbf{N}$). Gọi $\phi$ là ánh xạ liên tục $x \mapsto (f_n(x))_{n \in \mathbf{N}}$ từ X vào không gian mêtric được $K^\mathbf{N}$. Ảnh $X'$ của X qua $\phi$ là một không gian compact mêtric, vì X là compact. Gọi E là không gian con đóng của $\mathcal{C}_s(X)$ gồm các hàm liên tục $f$ trên X sao cho quan hệ $\phi(x) = \phi(y)$ kéo theo $f(x) = f(y)$ với mọi cặp điểm $x, y$ trong X. Theo hệ quả 2 của GT, I, § 9, No. 4 và mệnh đề 3 của GT, I, § 5, No. 2, ánh xạ $f' \mapsto f' \circ \phi$ là một đồng phôi $\phi^*$ từ $\mathcal{C}_s(X')$ lên E. Do đó tập hợp $A' = (\phi^*)^{-1}(\overline{A})$ là compact trong $\mathcal{C}_s(X')$, và hiển nhiên tồn tại các phần tử $f'_n$ trong $A'$ sao cho $\phi^*(f'_n) = f'_n \circ \phi$ bằng $f_n$.

Vì $X'$ là một không gian compact mêtric, tồn tại một tập con đếm được trù mật D' trong $X'$ (GT, IX, § 2, No. 8, mệnh đề 12 và § 2, No. 9, mệnh đề 16). Gọi $\mathcal{T}_1$ (tương ứng $\mathcal{T}_2$) là tôpô trên $A'$ cảm sinh bởi tôpô hội tụ đơn giản trên D' (tương ứng $X'$). Khi đó $\mathcal{T}_1$ là mêtric hóa được, $\mathcal{T}_2$ là compact và mịn hơn $\mathcal{T}_1$, do đó $\mathcal{T}_1$ và $\mathcal{T}_2$ trùng nhau; nói cách khác, $A'$ là một không gian con compact *mêtric hóa được* của $\mathcal{C}_s(X')$. Vì vậy, tồn tại một dãy $(f'_{n_k})$ trích ra từ $(f'_n)$ và hội tụ đến một phần tử $f'$ của $\mathcal{C}_s(X')$. Vì vậy, dãy $(f_{n_k})$ hội tụ đến $f = f' \circ \phi$ trong $\mathcal{C}_s(X)$.

(ii) $\Rightarrow$ (iii) : điều này là hiển nhiên.

(iii) $\Rightarrow$ (iv) : giả sử rằng mọi dãy vô hạn các phần tử của A đều có một điểm giới hạn trong $\mathcal{C}_s(X)$. Cho $x \in X$. Ánh xạ $\phi_x : f \mapsto f(x)$ từ A vào K là liên tục. Do đó, mọi dãy vô hạn trong $\phi_x(A)$ đều có một điểm giới hạn; vì trường K (bằng $\mathbf{R}$ hoặc $\mathbf{C}$) là mêtric hóa được, tập hợp $\phi_x(A)$ là tương đối compact trong K, do đó bị chặn. Nói cách khác, ta có $\sup_{f \in A} |f(x)| < \infty$.

Cho $f_n, x_m, \gamma$ và $\delta$ như trong (iv). Gọi $f$ là một điểm giới hạn của dãy $(f_n)$ trong $\mathcal{C}_s(X)$, và $x$ là một điểm giới hạn của dãy $(x_m)$ trong không gian compact X. Với mọi $m$, ánh xạ $h \mapsto h(x_m)$ từ $\mathcal{C}_s(X)$ vào K là liên tục. Theo các giả thiết, ta có $f(x_m) = \lim_{n \to \infty} f_n(x_m)$, và do đó $\gamma = \lim_{m \to \infty} f(x_m)$; vì $f : X \to K$ là liên tục và $x$ là một điểm giới hạn của dãy $(x_m)$, ta được $\gamma = f(x)$. Một cách tương tự, ta chứng minh đẳng thức $\delta = f(x)$, do đó $\gamma = \delta$.

(iv) $\Rightarrow$ (i) : giả sử rằng tập hợp các số $f(x)$, khi $f$ chạy qua A, bị chặn trong K với mọi $x \in X$. Điều này tương đương với việc giả sử rằng bao đóng $\overline{A}$ của A trong không gian tích $K^X$ là compact (GT, I, § 9, No. 5). Giả sử rằng A *không tương đối compact trong* $\mathcal{C}_s(X)$. Điều này có nghĩa là tồn tại một hàm $u \in \overline{A}$ và một điểm $a \in X$ sao cho $u$ không liên tục tại $a$. Do đó tồn tại một số thực $\varepsilon > 0$ sao cho trong mọi lân cận U của $a$, tồn tại một điểm $x$ với $|u(x) - u(a)| \geq \varepsilon$.

Ta sẽ xây dựng bằng quy nạp một dãy $(x_n)_{n \in \mathbf{N}}$ các điểm trong D và một dãy $(f_n)_{n \in \mathbf{N}}$ các phần tử của A, thỏa mãn các hệ thức sau :

(1)$_m$ $$ |u(x_m) - u(a)| \geq \varepsilon \quad \text{cho} \quad m \geq 1 ; $$

(2)$_m$ $$ |u(x_i) - f_m(x_i)| \leq \frac{1}{m + 1} \quad \text{cho} \quad 0 \leq i \leq m - 1 ; $$

(3)$_{m,i}$ $$ |f_m(x_i) - f_m(a)| \leq \frac{1}{i + 1} \quad \text{cho} \quad 0 \leq m \leq i . $$

Ta lấy $x_0 = a$ với $f_0$ tùy ý trong A (tập hợp A không rỗng, nếu không nó sẽ là tương đối compact trong $\mathcal{C}_s(X)$). Cho $n \geq 1$ và $x_0, x_1, ..., x_{n-1}, f_0, f_1, ..., f_{n-1}$ thỏa mãn các quan hệ (1)$_m$, (2)$_m$ với $1 \leq m < n$ và (3)$_{m,i}$ với $0 \leq m \leq i < n$. Vì $u$ thuộc $\overline{A}$, tồn tại $f_n \in A$ thỏa mãn (2)$_n$. Gọi $V_n$ là tập hợp tất cả các $x \in X$ sao cho $|f_m(x) - f_m(a)| \leq \frac{1}{n + 1}$ với $0 \leq m \leq n$. Vì $f_n$ liên tục, $V_n$ là một lân cận của $a$; chọn một điểm $x_n$ trong $D \cap V_n$ sao cho $|u(x_n) - u(a)| \geq \varepsilon$, do đó (1)$_n$ và (3)$_{m,n}$ được thỏa mãn. Vậy phép dựng có thể được tiếp tục.

Vì $u(X)$ là một tập con compact của K, tồn tại một dãy $(y_k)$ trích ra từ $(x_m)$ và sao cho giới hạn $\gamma = \lim_{k \to \infty} u(y_k)$ tồn tại. Theo (2)$_m$, ta có $u(x_i) = \lim_{n \to \infty} f_n(x_i)$ với mọi $i \in \mathbf{N}$, do đó

(4) $$
\gamma = \lim_{k \to \infty} \lim_{n \to \infty} f_n(y_k) .
$$

Mặt khác ta có $f_n(a) = \lim_{i \to \infty} f_n(x_i)$ theo (3)$_{m,i}$ do đó $f_n(a) = \lim_{k \to \infty} f_n(y_k)$. Vì $x_0 = a$, ta suy ra từ (2)$_m$ rằng $\lim_{n \to \infty} f_n(a) = u(a)$. Do đó,

$$
u(a) = \lim_{n \to \infty} \lim_{k \to \infty} f_n(y_k) .
$$

Cuối cùng, từ (1)$_m$, ta được $|\gamma - u(a)| \geq \varepsilon$, và do đó $\gamma \neq u(a)$. Điều này mâu thuẫn với mệnh đề (iv); vậy ta đã chứng minh rằng (iv) kéo theo (i).

### 3. Các định lý Eberlein và Šmulian

#### Định lý 1 (Eberlein) {#evt-iv-s5-thm-1 .statement}

— *Cho E là một không gian lồi địa phương Hausdorff và đầy đủ giả, $\mathcal{T}$ là một tôpô trên E tương thích với đối ngẫu giữa E và E' và A là một tập con của E. Để A tương đối compact đối với $\mathcal{T}$, điều kiện cần và đủ là mọi dãy vô hạn các điểm của A đều có một điểm giới hạn trong E đối với $\mathcal{T}$.*

Điều kiện đã nêu hiển nhiên là cần.

Giả sử bây giờ rằng mọi dãy vô hạn các điểm của A đều có một điểm giới hạn đối với $\mathcal{T}$, do đó cũng đối với tôpô thô hơn $\sigma(E, E')$. Khi đó A là tiền compact đối với $\mathcal{T}$ (IV, p. 32, mệnh đề 1); để A tương đối compact đối với $\mathcal{T}$, điều kiện cần và đủ là nó tương đối compact đối với $\sigma(E, E')$ (*loc. cit.*). Do đó đủ để chứng minh định lý khi $\mathcal{T}$ là tôpô yếu $\sigma(E, E')$.

Cho $\hat{E}$ là phần hoàn thành của E, mà ta sẽ đồng nhất như thường lệ với một không gian con của đối ngẫu đại số ${E'}^*$ của E' (III, p. 21, định lý 2). Kí hiệu $E_\sigma$, $\hat{E}_\sigma$ và $E_{\sigma'}^*$ là các không gian E, $\hat{E}$ và ${E'}^*$ được trang bị tương ứng các tôpô $\sigma(E, E')$, $\sigma(\hat{E}, E')$ và $\sigma({E'}^*, E')$.

Cho $(x'_i)_{i \in I}$ là một cơ sở của không gian vectơ E' trên trường K. Ánh xạ $f \mapsto (f(x'_i))_{i \in I}$ là một đồng phôi $\phi$ từ $E_{\sigma'}^*$ lên $K^I$; với mỗi $i \in I$, ảnh của A dưới ánh xạ $x'_i$ từ E vào K là tương đối compact : vì K mêtric hóa được và mọi dãy vô hạn các phần tử của $x'_i(A)$ đều có một điểm giới hạn. Suy ra rằng $\phi(A)$ là tương đối compact trong $K^I$, do đó bao đóng $\overline{A}$ của A trong $E_{\sigma'}^*$ là compact.

*Tiếp theo ta sẽ chứng minh rằng $\overline{A}$ được chứa trong $\hat{E}$.* Cho H là một tập hợp cân bằng liên tục của E'; cho X là bao đóng của nó đối với $\sigma(E', E)$; X là compact (III, p. 17, hệ quả 2). Với mọi $x \in {E'}^*$, kí hiệu $\phi_x$ là hạn chế của $x' \mapsto \langle x, x' \rangle$ lên X; cho $\tilde{A} \subset \mathscr{C}_s(X)$ là tập hợp các hàm $\phi_x$ khi x chạy trên A. Theo giả thiết về A, mọi dãy vô hạn các phần tử của $\tilde{A}$ đều có một điểm giới hạn trong $\mathscr{C}_s(X)$; theo mệnh đề 2 (IV, p. 33), tập hợp $\tilde{A}$ do đó là tương đối compact trong $\mathscr{C}_s(X)$. *Suy ra rằng với mọi $a \in \overline{A}$, hàm $\phi_a$ trên X là liên tục.* Bao hàm $\overline{A} \subset \hat{E}$ sau đó suy ra từ định lý 2 của III, p. 21.

*Bây giờ ta sẽ chỉ ra rằng $\overline{A}$ được chứa trong E.* Vì A là tiền compact trong $E_\sigma$ (IV, p. 32, mệnh đề 1), nó bị chặn trong $E_\sigma$ (III, p. 3, mệnh đề 2), do đó cũng bị chặn trong E (IV, p. 1, mệnh đề 1). Cho C là bao lồi cân bằng đóng của A trong E. Khi đó C bị chặn vì A bị chặn, do đó đầy đủ vì E là giả đầy đủ. Nói cách khác, C là một tập hợp lồi và đóng của $\hat{E}$, do đó cũng của $\hat{E}_\sigma$ (IV, p. 1, mệnh đề 1). Vì $A \subset C$ và tôpô của $\hat{E}_\sigma$ được cảm sinh bởi tôpô của $E_{\sigma'}^*$, ta có $\overline{A} \subset C$, và do đó $\overline{A} \subset E$.

Vì tôpô của $E_\sigma$ được cảm sinh bởi tôpô của ${E'_\sigma}^*$, tập con $\overline{A}$ của $E_\sigma$ là compact, và định lý 1 được suy ra.

**Định lý 2 (Šmulian).** — *Cho E là một không gian Fréchet và A là một tập con của E. Cho $E_\sigma$ là không gian E được trang bị tôpô yếu. Các điều kiện sau là tương đương* :

(i) *A là tương đối compact trong $E_\sigma$;*
(ii) *mọi dãy vô hạn các điểm của A đều có một điểm giới hạn trong $E_\sigma$;*
(iii) *từ mọi dãy vô hạn các điểm của A, ta có thể trích ra một dãy hội tụ trong $E_\sigma$.*

Sự tương đương của (i) và (ii) suy ra từ định lý Eberlein và (iii) hiển nhiên kéo theo (ii).

Chúng ta sẽ chứng minh rằng (i) kéo theo (iii). Giả sử rằng bao đóng B của A trong $E_\sigma$ là compact và rằng $(x_n)_{n \in \mathbf{N}}$ là một dãy các điểm của A. Gọi F là không gian vectơ con đóng nhỏ nhất của E chứa các $x_n$, đây là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất. Vì F là đóng trong $E_\sigma$ và tôpô $\sigma(F, F')$ trên F được cảm sinh bởi $\sigma(E, E')$, tập hợp $B \cap F$ là compact đối với $\sigma(F, F')$. Theo các nhận xét trong IV, p. 32, sự tồn tại của một dãy trích ra từ $(x_n)_{n \in \mathbf{N}}$ hội tụ đối với $\sigma(E, E')$ (hoặc, điều này là tương đương, đối với $\sigma(F, F')$) là một hệ quả của bổ đề sau :

#### Bổ đề 1 {#evt-iv-s5-lem-1 .statement}

— *Cho F là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất. Mọi tập con C của F compact đối với tôpô $\mathcal{T}$ cảm sinh bởi $\sigma(F, F')$ đều là mêtric đối với tôpô này.*

Vì tôpô của sự hội tụ tiền compact trên $F'$ mịn hơn tôpô $\sigma(F', F)$, tồn tại một tập con đếm được trù mật khắp nơi trong $F'_s$ (III, p. 18, hệ quả 1). Do đó tập hợp C có thể được đồng nhất với một tập con của $K^D$, và tôpô cảm sinh trên C bởi tôpô của $K^D$, là mêtric (GT, IX, § 2, No. 8), thô hơn tôpô cảm sinh bởi $\sigma(F, F')$, đối với tôpô này C là compact. Suy ra hai tôpô này trùng nhau (GT, I, § 9, No. 4, hệ quả 3).

Định lý Šmulian có thể được mở rộng sang trường hợp E là giới hạn quy nạp ngặt của một dãy các không gian Fréchet (IV, p. 67, bài tập 2).

### *4. Trường hợp các không gian các hàm liên tục bị chặn*

Với mọi không gian tôpô X, ký hiệu $\mathscr{C}^b(X)$ là không gian Banach của tất cả các ánh xạ liên tục và *bị chặn* từ X vào K, với chuẩn được xác định bởi

$$
\| f \| = \sup_{x \in X} |f(x)|
$$

(GT, X, § 3, No. 2). Khi X compact, mọi hàm liên tục trên X đều bị chặn (GT, IV, § 6, No. 1), và ta viết $\mathscr{C}(X)$ cho $\mathscr{C}^b(X)$.

Trong tiết diện này và tiết diện sau, ta sẽ sử dụng bổ đề sau, là một trường hợp riêng của định lý Lebesgue (INT, IV, ấn bản thứ 2. § 4, No. 3, th. 2) do cách diễn giải các phần tử của $\mathscr{C}(X)'$ như các độ đo trên X.

#### Bổ đề 2 {#evt-iv-s5-lem-2 .statement}

Cho X là một không gian compact. Nếu một dãy $(f_n)_{n \in \mathbf{N}}$ bị chặn trong $C(X)$ và hội tụ đơn giản trên X đến một hàm liên tục f, thì $\mu(f) = \lim_{n \to \infty} \mu(f_n)$ đối với mọi $\mu$ trong $C(X)'$.

#### Mệnh đề 3 {#evt-iv-s5-prop-3 .statement}

Cho X là một không gian compact, và cho A là một tập con bị chặn của $C(X)$. Để A tương đối compact đối với tôpô của sự hội tụ đơn giản, điều kiện cần và đủ là nó tương đối compact đối với $\sigma(C(X), C(X)')$.

Tôpô của sự hội tụ đơn giản là Hausdorff và thô hơn $\sigma(C(X), C(X)')$, do đó điều kiện đã nêu là đủ (GT, I, § 9, No. 4, hệ quả 3).

Bây giờ giả sử rằng A tương đối compact đối với tôpô của sự hội tụ đơn giản. Cho $(f_n)_{n \in \mathbf{N}}$ là một dãy các phần tử của A. Theo mệnh đề 2 (IV, p. 33), tồn tại một dãy $(f_{n_k})$ trích ra từ $(f_n)$ và hội tụ đơn giản đến một hàm liên tục f. Theo bổ đề 2, dãy bị chặn $(f_{n_k})$ tiến đến f đối với $\sigma(C(X), C(X)')$. Khi đó định lý Šmulian (IV, p. 36, th. 2) chỉ ra rằng A tương đối compact đối với $\sigma(C(X), C(X)')$.

#### Hệ quả {#evt-iv-s5-n4-cor-1 .statement}

Cho S là một không gian tôpô và A là một tập con bị chặn của $C^b(S)$. Các điều kiện sau là tương đương :
(i) A tương đối compact đối với $\sigma(C^b(S), C^b(S'))$;
(ii) nếu $(f_n)_{n \in \mathbf{N}}$ là một dãy các phần tử của A và $(x_m)_{m \in \mathbf{N}}$ là một dãy các điểm của S sao cho các giới hạn lặp
$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$
tồn tại, thì $\gamma = \delta$.

Cho X là compact hóa Stone-Čech của S (GT, IX, § 1, No. 6) và $\alpha$ là ánh xạ chính tắc từ S vào X. Đặt D = $\alpha(S)$. Ánh xạ $\phi : f \mapsto f \circ \alpha$ là một đẳng cấu từ không gian định chuẩn $C(X)$ lên không gian định chuẩn $C^b(S)$; đặt $\tilde{A} = \phi^{-1}(A)$. Vì X compact và D trù mật trong X, mệnh đề 2 (IV, p. 33) chỉ ra rằng điều kiện (ii) tương đương với tính compact của $\tilde{A}$ đối với tôpô của sự hội tụ đơn giản. Sự tương đương của (i) và (ii) sau đó suy ra từ mệnh đề 3. \*

### *5. Bao lồi của một tập compact yếu

#### Định lý 3 (Krein) {#evt-iv-s5-thm-3 .statement}

Cho E là một không gian lồi địa phương Hausdorff và quasi-đầy đủ, và cho $\mathcal{T}$ là một tôpô trên E tương thích với đối ngẫu giữa E và E'. Cho A là một tập con của E compact đối với $\mathcal{T}$. Khi đó bao lồi cân bằng đóng C của A là compact đối với $\mathcal{T}$.

Trước hết chúng ta sẽ thực hiện một số phép rút gọn.
A) Tập hợp C là tiền compact đối với $\mathcal{T}$ (II, p. 25, Mệnh đề 3), và A là compact đối với $\sigma(E, E')$. Do Mệnh đề 1 (IV, p. 32), chỉ cần chứng minh rằng C là compact đối với $\sigma(E, E')$, và như vậy ta đã quy về trường hợp $\mathcal{T} = \sigma(E, E')$.
B) Vì C là tiền compact và đóng đối với $\sigma(E, E')$, nên nó bị chặn và đóng đối với tôpô ban đầu của E (III, p. 3, Mệnh đề 2 và IV, p. 1, Mệnh đề 1); do đó nó đầy đủ vì E là giả đầy đủ. Nói cách khác, C là bao lồi cân bằng đóng của $A$ trong phần đầy đủ $\hat{E}$ của $E$. Vì tôpô $\sigma(\hat{E}, E')$ cảm sinh $\sigma(E, E')$ trên $E$, ta đã quy về *trường hợp khi $E$ đầy đủ*.

C) Gọi $\Gamma$ là bao lồi cân bằng của $A$. Khi đó C là bao đóng của $\Gamma$ đối với $\sigma(E, E')$. Theo định lý Eberlein (IV, p. 35, định lý 1), chỉ cần chứng minh rằng mọi dãy $(x_n)_{n \in \mathbf{N}}$ các điểm của $\Gamma$ đều có một điểm giới hạn đối với $\sigma(E, E')$ trong E. Nhưng $x_n$ thuộc bao lồi cân bằng của một tập con hữu hạn $B_n$ của $A$. Gọi $F$ là không gian con vectơ đóng của E sinh bởi tập hợp đếm được $B = \bigcup_n B_n$. Khi đó F đầy đủ, tôpô $\sigma(F, F')$ trên F được cảm sinh bởi $\sigma(E, E')$ và ta có $x_n \in F$ với mọi $n \in \mathbf{N}$. Do đó chỉ cần chứng minh rằng $(x_n)_{n \in \mathbf{N}}$ có một điểm giới hạn đối với $\sigma(F, F')$, điều này đưa đến phép rút gọn về *trường hợp khi tồn tại một tập hợp trù mật đếm được trong $E$*.

Gán cho $A$ tôpô cảm sinh bởi $\sigma(E, E')$, điều này làm cho nó trở thành một không gian compact. Ta định nghĩa một ánh xạ tuyến tính $u : E' \to \mathcal{C}(A)$ bởi

$$
u(x')(a) = \langle a, x' \rangle \quad (a \in A, x' \in E') .
$$

Cho $(x'_n)_{n \in \mathbf{N}}$ là một dãy liên tục đều trong $E'$, hội tụ về 0 đối với $\sigma(E', E)$. Khi đó dãy các hàm $u(x'_n)$ bị chặn trong $\mathcal{C}(A)$ và hội tụ đơn giản về 0. Với mọi $\mu \in \mathcal{C}(A)'$, ta có $\lim_{n \to \infty} \mu(u(x'_n)) = 0$ theo bổ đề 2 (IV, p. 37). Theo tiêu chuẩn được nêu trong nhận xét ở III, p. 21, dạng tuyến tính $\mu \circ u$ trên $E'$ khi đó liên tục đối với $\sigma(E', E)$ với mọi $\mu \in \mathcal{C}(A)'$. Do đó tồn tại một ánh xạ tuyến tính $v : \mathcal{C}(A)' \to E$ thỏa mãn quan hệ

$$
\langle u(x'), \mu \rangle = \langle v(\mu), x' \rangle \quad (x' \in E', \mu \in \mathcal{C}(A)') .
$$

Hiển nhiên rằng $v$ là liên tục nếu $\mathcal{C}(A)'$ được gán tôpô $\sigma(\mathcal{C}(A)', \mathcal{C}(A))$ và E tôpô $\sigma(E, E')$.

Quả cầu đơn vị (đóng) $B$ của không gian Banach $\mathcal{C}(A)$ là compact đối với tôpô $\sigma(\mathcal{C}(A)', \mathcal{C}(A))$ (III, p. 17, hệ quả 3). Do đó, $v(B)$ là một tập con lồi, cân bằng và compact của $E$ đối với $\sigma(E, E')$. Với mọi $a \in A$, dạng tuyến tính liên tục $\varepsilon_a : f \mapsto f(a)$ trên $\mathcal{C}(A)$ thuộc $B$, và ta có $v(\varepsilon_a) = a$ theo các công thức (7) và (8). Suy ra, $A \subset v(B)$, và do đó $C \subset v(B)$. Điều này chứng minh rằng $C$ là compact đối với $\sigma(E, E')$.

Q.E.D.

### Bài tập {#evt-iv-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
