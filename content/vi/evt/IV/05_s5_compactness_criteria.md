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
statements: 6
exercises: 18
content_sha256: e7ff8a28bb3df355a7c541ca16aa1c28767af4c4dd241047bce7da1e310c7fa1
translated_from: content/en/evt/IV/05_s5_compactness_criteria.md
source_content_sha256: 4702a615033dfbad2393a5c1455faef75a03a10034ae4dba1ab3b73fab718883
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-659a8e67
glossary_version: 34
glossary_terms_sha256: 7a5d3a55190fa97aec2bdad72c890c7e12f1eeea8b1a2f26da5ea15a9aa177bb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC TIÊU CHUẨN COMPACT

### 1. Nhận xét tổng quát

Cho A là một tập con của một không gian tôpô E. Để một dãy $(x_n)_{n \in \mathbf{N}}$ các điểm của A có một điểm x của E làm điểm giới hạn, điều kiện cần và đủ là điều kiện sau đây được thỏa mãn (GT, I, § 7, No. 3) :

(A) Với mọi số nguyên $ m \geq 0 $ và mọi lân cận U của x, tồn tại một số nguyên $ n \geq m $ sao cho $ x_n \in U $.

Một dãy có dạng $(y_k)_{k \in \mathbf{N}}$ với $ y_k = x_{n_k} $ ứng với một dãy tăng ngặt $(n_k)_{k \in \mathbf{N}}$ các số nguyên dương được gọi là một dãy trích ra của dãy $(x_n)_{n \in \mathbf{N}}$. Nếu tồn tại một dãy trích ra của dãy $(x_n)_{n \in \mathbf{N}}$ hội tụ tới x, thì x là một điểm giới hạn của $(x_n)$; ngược lại, nếu x có một hệ cơ bản đếm được các lân cận, và x là điểm giới hạn của dãy $(x_n)$, thì tồn tại một dãy trích ra của $(x_n)$ hội tụ tới x.

Do GT, IX, § 2, No. 9, hệ quả, ta kết luận rằng khi E là khả mêtric, các điều kiện sau là tương đương :
a) tập hợp A là compact tương đối trong E ;
b) mọi dãy vô hạn các điểm của A đều có một điểm giới hạn trong E ;
c) từ mọi dãy vô hạn các điểm của A, ta có thể trích ra một dãy hội tụ tới một điểm của E.

Trong tiết này, chúng ta sẽ mở rộng tiêu chuẩn này cho một số không gian vectơ tôpô không khả mêtric. Mệnh đề sau cho phép ta rút gọn việc nghiên cứu các tập hợp compact về việc nghiên cứu các tập hợp compact yếu trong một số trường hợp.

#### Mệnh đề 1 {#evt-iv-s5-prop-1 .statement}

— Cho E là một không gian lồi địa phương Hausdorff, và A là một tập con của E. Ký hiệu $ E_\sigma $ là không gian E được trang bị tôpô yếu hơn.
a) Nếu mọi dãy vô hạn các điểm của A đều có một điểm giới hạn trong E, thì A là tiền compact trong E.
b) Để A compact tương đối trong E, điều kiện cần và đủ là nó tiền compact trong E và compact tương đối trong $ E_\sigma $.

Chúng ta sẽ chứng minh a) bằng phản chứng. Nếu A không tiền compact, thì theo định lý 3 của GT, II, § 3, No. 7, suy ra rằng tồn tại một lân cận đối xứng lồi V của 0 trong E sao cho A không thể được phủ bởi một số hữu hạn các bản dịch của V.

Nói cách khác, nếu $ x_0, x_1, ..., x_{n-1} $ là các điểm của A, thì $ A \notin \bigcup_{0 \leq i < n} (x_i + V) $ và do đó tồn tại một điểm $ x_n $ của A sao cho $ x_n - x_i \notin V $ với $ 0 \leq i < n $. Khi đó, bằng quy nạp theo số nguyên $ n $, ta có thể xây dựng một dãy vô hạn $ (x_n)_{n \in \mathbf{N}} $ các điểm của A sao cho $ x_n - x_m \notin V $ mỗi khi $ n > m $; vì V là đối xứng, ta cũng có $ x_m - x_n \notin V $ với $ m \neq n $ và các tập hợp $ x_n + \frac{1}{2} V $ rời nhau. Với mọi điểm $ x $ trong E, tồn tại nhiều nhất một số nguyên $ n \geq 0 $ sao cho $ x_n \in x + \frac{1}{2} V $, do đó dãy $ (x_n)_{n \in \mathbf{N}} $ không có điểm giới hạn nào. Điều này chứng minh *a)*.

Bây giờ giả sử rằng A là tiền compắc trong E và được chứa trong một tập con compắc B của $ E_\sigma $. Khi đó B là đầy đủ trong $ E_\sigma $, do đó cũng đầy đủ trong E (IV, p. 5, *Nhận xét 2*). Ta có $ \overline{A} \subset B $, vì thế A là tương đối compắc trong E. Điều đảo lại là hiển nhiên và *b)* suy ra.

### 2. Tính compắc đơn của các tập các hàm liên tục

Trong tiết này, X ký hiệu một không gian *compắc* và $ \mathcal{C}_s(X) $ là không gian các hàm liên tục trên X, nhận giá trị trong trường K (bằng $ \mathbf{R} $ hoặc $ \mathbf{C} $). Không gian $ \mathcal{C}_s(X) $ được trang bị tôpô hội tụ đơn trên X.

#### Mệnh đề 2 {#evt-iv-s5-prop-2 .statement}

*Cho D là một tập con trù mật của X và A là một tập con của không gian $ \mathcal{C}_s(X) $. Các điều kiện sau là tương đương :*
(i) *A là tương đối compắc trong $ \mathcal{C}_s(X) $.*
(ii) *Từ mọi dãy vô hạn các phần tử của A, ta có thể trích ra một dãy hội tụ trong $ \mathcal{C}_s(X) $.*
(iii) *Mọi dãy vô hạn các phần tử của A đều có một điểm giới hạn trong $ \mathcal{C}_s(X) $.*
(iv) *Cho $ (f_n)_{n \in \mathbf{N}} $ là một dãy các hàm thuộc A và $ (x_m)_{m \in \mathbf{N}} $ là một dãy các điểm của D. Nếu các giới hạn lặp*

$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$

*nếu tồn tại, thì chúng bằng nhau. Ngoài ra, ta có $ \sup_{f \in A} |f(x)| < + \infty $ với mọi $ x \in X $.*

(i) $ \Rightarrow $ (ii) : gọi $ \overline{A} $ là bao đóng của A trong $ \mathcal{C}_s(X) $. Giả sử A là compắc, và xét một dãy các hàm $ f_n \in A $ (với $ n \in \mathbf{N} $). Gọi $ \phi $ là ánh xạ liên tục $ x \mapsto (f_n(x))_{n \in \mathbf{N}} $ từ X vào không gian mêtric hóa được $ K^\mathbf{N} $. Ảnh $ X' $ của X qua $ \phi $ là một không gian compắc mêtric hóa được, vì X là compắc. Gọi E là không gian con đóng của $ \mathcal{C}_s(X) $ gồm các hàm liên tục $ f $ trên X sao cho quan hệ $ \phi(x) = \phi(y) $ kéo theo $ f(x) = f(y) $ với mọi cặp điểm $ x, y $ trong X. Theo hệ quả 2 của GT, I, § 9, No. 4 và mệnh đề 3 của GT, I, § 5, No. 2, ánh xạ $ f' \mapsto f' \circ \phi $ là một đồng phôi $ \phi^* $ từ $ \mathcal{C}_s(X') $ lên E. Do đó tập hợp $ A' = (\phi^*)^{-1}(\overline{A}) $ là compắc trong $ \mathcal{C}_s(X') $, và hiển nhiên là tồn tại các phần tử $ f'_n $ trong $ A' $ sao cho $ \phi^*(f'_n) = f'_n \circ \phi $ bằng $ f_n $.

Vì $ X' $ là một không gian compact khả mêtric, nên tồn tại một tập con trù mật đếm được D' trong $ X' $ (GT, IX, § 2, No. 8, mệnh đề 12 và § 2, No. 9, mệnh đề 16). Gọi $ \mathcal{T}_1 $ (resp. $ \mathcal{T}_2 $) là tôpô trên $ A' $ cảm sinh bởi tôpô hội tụ đơn giản trên D' (resp. $ X' $). Khi đó $ \mathcal{T}_1 $ là khả mêtric, $ \mathcal{T}_2 $ là compact và mịn hơn $ \mathcal{T}_1 $, do đó $ \mathcal{T}_1 $ và $ \mathcal{T}_2 $ trùng nhau; nói cách khác, $ A' $ là một không gian con compact *khả mêtric* của $ \mathcal{C}_s(X') $. Vì thế, tồn tại một dãy $(f'_{n_k})$ trích từ $(f'_n)$ và hội tụ tới một phần tử $f'$ của $\mathcal{C}_s(X')$. Do đó, dãy $(f_{n_k})$ hội tụ tới $f = f' \circ \phi$ trong $\mathcal{C}_s(X)$.

(ii) $\Rightarrow$ (iii) : điều này là hiển nhiên.

(iii) $\Rightarrow$ (iv) : giả sử rằng mọi dãy vô hạn các phần tử của A đều có một điểm giới hạn trong $\mathcal{C}_s(X)$. Cho $x \in X$. Ánh xạ $\phi_x : f \mapsto f(x)$ từ A vào K là liên tục. Do đó, mọi dãy vô hạn trong $\phi_x(A)$ đều có một điểm giới hạn; vì trường K (bằng $\mathbf{R}$ hoặc $\mathbf{C}$) là khả mêtric, tập hợp $\phi_x(A)$ là compắc tương đối trong K, vì thế bị chặn. Nói cách khác, ta có $\sup_{f \in A} |f(x)| < \infty$.

Cho $f_n, x_m, \gamma$ và $\delta$ như trong (iv). Cho $f$ là một điểm giới hạn của dãy $(f_n)$ trong $\mathcal{C}_s(X)$, và $x$ là một điểm giới hạn của dãy $(x_m)$ trong không gian compact X. Với mọi $m$, ánh xạ $h \mapsto h(x_m)$ từ $\mathcal{C}_s(X)$ vào K là liên tục. Theo các giả thiết, ta có $f(x_m) = \lim_{n \to \infty} f_n(x_m)$, và vì thế $\gamma = \lim_{m \to \infty} f(x_m)$; vì $f : X \to K$ là liên tục và $x$ là một điểm giới hạn của dãy $(x_m)$, ta được $\gamma = f(x)$. Bằng một cách tương tự, ta chứng minh đẳng thức $\delta = f(x)$, do đó $\gamma = \delta$.

(iv) $\Rightarrow$ (i) : giả sử rằng tập hợp các số $f(x)$, khi $f$ chạy qua A, là bị chặn trong K với mọi $x \in X$. Điều này tương đương với việc giả sử rằng bao đóng $\overline{A}$ của A trong không gian tích $K^X$ là compac (GT, I, § 9, No. 5). Giả sử rằng A *không tương đối compac trong* $\mathcal{C}_s(X)$. Điều đó có nghĩa là tồn tại một hàm $u \in \overline{A}$ và một điểm $a \in X$ sao cho $u$ không liên tục tại $a$. Do đó tồn tại một số thực $\varepsilon > 0$ sao cho trong mọi lân cận U của $a$, tồn tại một điểm $x$ với $|u(x) - u(a)| \geq \varepsilon$.

Ta sẽ xây dựng bằng quy nạp một dãy $(x_n)_{n \in \mathbf{N}}$ các điểm trong D và một dãy $(f_n)_{n \in \mathbf{N}}$ các phần tử của A, thỏa mãn các hệ thức sau :

(1)$_m$ $$ |u(x_m) - u(a)| \geq \varepsilon \quad \text{với} \quad m \geq 1 ; $$

(2)$_m$ $$ |u(x_i) - f_m(x_i)| \leq \frac{1}{m + 1} \quad \text{với} \quad 0 \leq i \leq m - 1 ; $$

(3)$_{m,i}$ $$ |f_m(x_i) - f_m(a)| \leq \frac{1}{i + 1} \quad \text{với} \quad 0 \leq m \leq i . $$

Ta lấy $x_0 = a$ với $f_0$ tùy ý trong A (tập hợp A không rỗng, nếu không nó sẽ tương đối compắc trong $\mathcal{C}_s(X)$). Cho $n \geq 1$ và giả sử $x_0, x_1, ..., x_{n-1}, f_0, f_1, ..., f_{n-1}$ thỏa mãn các hệ thức (1)$_m$, (2)$_m$ với $1 \leq m < n$ và (3)$_{m,i}$ với $0 \leq m \leq i < n$. Vì $u$ thuộc $\overline{A}$, tồn tại $f_n \in A$ thỏa mãn (2)$_n$. Gọi $V_n$ là tập hợp tất cả các $x \in X$ sao cho $|f_m(x) - f_m(a)| \leq \frac{1}{n + 1}$ với $0 \leq m \leq n$. Vì $f_n$ liên tục, $V_n$ là một lân cận của $a$; chọn một điểm $x_n$ trong $D \cap V_n$ sao cho $|u(x_n) - u(a)| \geq \varepsilon$, do đó (1)$_n$ và (3)$_{m,n}$ được thỏa mãn. Vậy phép dựng có thể được tiếp tục.

Vì $u(X)$ là một tập con compact của K, tồn tại một dãy $(y_k)$ trích ra từ $(x_m)$ và sao cho giới hạn $\gamma = \lim_{k \to \infty} u(y_k)$ tồn tại. Theo (2)$_m$, ta có $u(x_i) = \lim_{n \to \infty} f_n(x_i)$ với mọi $i \in \mathbf{N}$, do đó

(4) $$
\gamma = \lim_{k \to \infty} \lim_{n \to \infty} f_n(y_k) .
$$

Mặt khác ta có $ f_n(a) = \lim_{i \to \infty} f_n(x_i) $ theo (3)$_{m,i}$ do đó $ f_n(a) = \lim_{k \to \infty} f_n(y_k) $. Vì $ x_0 = a $, ta suy ra từ (2)$_m$ rằng $ \lim_{n \to \infty} f_n(a) = u(a) $. Do đó,

$$
u(a) = \lim_{n \to \infty} \lim_{k \to \infty} f_n(y_k) .
$$

Sau cùng, từ (1)$_m$, ta được $ |\gamma - u(a)| \geq \varepsilon $, và do đó $ \gamma \neq u(a) $. Điều này mâu thuẫn với mệnh đề (iv); như vậy ta đã chứng minh rằng (iv) suy ra (i).

### 3. Các định lý Eberlein và Šmulian

#### Định lý 1 (Eberlein) {#evt-iv-s5-thm-1 .statement}

— *Cho E là một không gian lồi địa phương Hausdorff và tựa đầy đủ, $ \mathcal{T} $ là một tôpô trên E tương thích với đối ngẫu giữa E và E' và A là một tập con của E. Điều kiện cần và đủ để A tương đối compắc đối với $ \mathcal{T} $ là mọi dãy vô hạn các điểm của A đều có một điểm giới hạn trong E đối với $ \mathcal{T} $.*

Điều kiện đã phát biểu hiển nhiên là cần.

Bây giờ giả sử rằng mọi dãy vô hạn các điểm của A đều có một điểm giới hạn đối với $ \mathcal{T} $, do đó cũng đối với tôpô yếu hơn $ \sigma(E, E') $. Khi đó A là tiền compắc đối với $ \mathcal{T} $ (IV, p. 32, prop. 1); để A tương đối compắc đối với $ \mathcal{T} $, điều kiện cần và đủ là nó cũng như vậy đối với $ \sigma(E, E') $ (*loc. cit.*). Vậy chỉ cần chứng minh định lý khi $ \mathcal{T} $ là tôpô yếu $ \sigma(E, E') $.

Ký hiệu $ \hat{E} $ là bổ sung của E, mà như thường lệ ta sẽ đồng nhất với một không gian con của đối ngẫu đại số $ {E'}^* $ của E' (III, p. 21, đl. 2). Ký hiệu $ E_\sigma $, $ \hat{E}_\sigma $ và $ E_{\sigma'}^* $ là các không gian E, $ \hat{E} $ và $ {E'}^* $ được trang bị các tôpô $ \sigma(E, E') $, $ \sigma(\hat{E}, E') $ và $ \sigma({E'}^*, E') $ tương ứng.

Cho $ (x'_i)_{i \in I} $ là một cơ sở của không gian vectơ E' trên trường K. Ánh xạ $ f \mapsto (f(x'_i))_{i \in I} $ là một đồng phôi $ \phi $ từ $ E_{\sigma'}^* $ lên $ K^I $; với mọi $ i \in I $, ảnh của A dưới ánh xạ $ x'_i $ từ E vào K là tương đối compact : thật vậy, K khả mê và mọi dãy vô hạn các phần tử của $ x'_i(A) $ đều có một điểm giới hạn. Suy ra $ \phi(A) $ là tương đối compact trong $ K^I $, do đó bao đóng $ \overline{A} $ của A trong $ E_{\sigma'}^* $ là compact.

*Tiếp theo ta sẽ chứng minh rằng $ \overline{A} $ được chứa trong $ \hat{E} $.* Cho H là một tập con đồng liên tục của E'; gọi X là bao đóng của nó đối với $ \sigma(E', E) $; X là compắc (III, p. 17, hệ quả 2). Với mỗi $ x \in {E'}^* $, gọi $ \phi_x $ là hạn chế lên X của hàm $ x' \mapsto \langle x, x' \rangle $; gọi $ \tilde{A} \subset \mathscr{C}_s(X) $ là tập hợp các hàm $ \phi_x $ khi x chạy qua A. Theo giả thiết trên A, mọi dãy vô hạn các phần tử của $ \tilde{A} $ đều có một điểm giới hạn trong $ \mathscr{C}_s(X) $; do mệnh đề 2 (IV, p. 33), suy ra tập hợp $ \tilde{A} $ là tương đối compắc trong $ \mathscr{C}_s(X) $. *Suy ra rằng với mọi $ a \in \overline{A} $, hàm $ \phi_a $ trên X là liên tục.* Khi đó, bao hàm thức $ \overline{A} \subset \hat{E} $ suy ra từ định lý 2 của III, p. 21.

*Bây giờ ta sẽ chỉ ra rằng $ \overline{A} $ được chứa trong E.* Vì A là tiền compac trong $ E_\sigma $ (IV, p. 32, prop. 1), nên nó bị chặn trong $ E_\sigma $ (III, p. 3, prop. 2), do đó cũng bị chặn trong E (IV, p. 1, prop. 1). Gọi C là bao lồi cân bằng đóng của A trong E. Khi đó C bị chặn vì A bị chặn, do đó đầy đủ vì E là gần đầy đủ. Nói cách khác, C là một tập con lồi và đóng của $ \hat{E} $, nên cũng là một tập con của $ \hat{E}_\sigma $ (IV, p. 1, prop. 1). Vì $ A \subset C $ và tôpô của $ \hat{E}_\sigma $ được cảm sinh bởi tôpô của $ E_{\sigma'}^* $, ta có $ \overline{A} \subset C $, và do đó $ \overline{A} \subset E $.

Vì tôpô của $ E_\sigma $ được cảm sinh bởi tôpô của $ {E'_\sigma}^* $, tập con $ \overline{A} $ của $ E_\sigma $ là compac, và định lý 1 được suy ra.

**Định lý 2 (Šmulian).** — *Cho E là một không gian Fréchet và A là một tập con của E. Ký hiệu $ E_\sigma $ là không gian E được trang bị tôpô yếu hơn. Các điều kiện sau là tương đương* :

(i) *A tương đối compắc trong $ E_\sigma $;*
(ii) *mọi dãy vô hạn các điểm của A đều có một điểm giới hạn trong $ E_\sigma $;*
(iii) *từ mọi dãy vô hạn các điểm của A, ta có thể trích ra một dãy hội tụ trong $ E_\sigma $.*

Tính tương đương của (i) và (ii) suy ra từ định lý của Eberlein, và (iii) hiển nhiên kéo theo (ii).

Chúng tôi sẽ chứng minh rằng (i) kéo theo (iii). Giả sử rằng bao đóng B của A trong $ E_\sigma $ là compắc và $ (x_n)_{n \in \mathbf{N}} $ là một dãy các điểm của A. Gọi F là không gian con vectơ đóng nhỏ nhất của E chứa các $ x_n $, đây là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất. Vì F đóng trong $ E_\sigma $ và tôpô $ \sigma(F, F') $ trên F được cảm sinh bởi $ \sigma(E, E') $, tập $ B \cap F $ là compắc đối với $ \sigma(F, F') $. Theo các nhận xét ở IV, p. 32, sự tồn tại của một dãy trích từ $ (x_n)_{n \in \mathbf{N}} $ hội tụ đối với $ \sigma(E, E') $ (hay, điều cũng vậy, đối với $ \sigma(F, F') $) là hệ quả của bổ đề sau :

#### Bổ đề 1 {#evt-iv-s5-lem-1 .statement}

— *Cho F là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất. Mọi tập con C của F compact đối với tôpô $ \mathcal{T} $ cảm sinh bởi $ \sigma(F, F') $ đều khả mêtric đối với tôpô này.*

Vì tôpô hội tụ trên các tập tiền compact trên $ F' $ mịn hơn tôpô $ \sigma(F', F) $, nên tồn tại một tập con đếm được trù mật khắp nơi trong $ F'_s $ (III, p. 18, hệ quả 1). Do đó tập hợp C có thể được đồng nhất với một tập con của $ K^D $, và tôpô cảm sinh trên C bởi tôpô của $ K^D $, là một tôpô khả mêtric (GT, IX, § 2, No. 8), thô hơn tôpô cảm sinh bởi $ \sigma(F, F') $, đối với tôpô này C là compact. Vậy hai tôpô ấy là đồng nhất (GT, I, § 9, No. 4, hệ quả 3).

Định lý của Šmulian có thể được mở rộng cho trường hợp E là giới hạn quy nạp ngặt của một dãy các không gian Fréchet (IV, p. 67, bài tập 2).

### \*4. Trường hợp các không gian các hàm liên tục bị chặn*

Với mọi không gian tôpô X, ký hiệu $ \mathscr{C}^b(X) $ là không gian Banach của mọi ánh xạ liên tục và *bị chặn* từ X vào K, với chuẩn được định nghĩa bởi

$$
\| f \| = \sup_{x \in X} |f(x)|
$$

(GT, X, § 3, No. 2). Khi X compact, mọi hàm liên tục trên X đều bị chặn (GT, IV, § 6, No. 1), và ta viết $ \mathscr{C}(X) $ cho $ \mathscr{C}^b(X) $.

Trong tiết này và tiết tiếp theo, ta sẽ dùng bổ đề sau, là một trường hợp riêng của định lý Lebesgue (INT, IV, 2nd ed. § 4, No. 3, định lý 2) do cách giải thích các phần tử của $ \mathscr{C}(X)' $ như những độ đo trên X.

#### Bổ đề 2 {#evt-iv-s5-lem-2 .statement}

— Cho X là một không gian compact. Nếu một dãy $(f_n)_{n \in \mathbf{N}}$ bị chặn trong $C(X)$ và hội tụ đơn trên X tới một hàm liên tục f, thì $\mu(f) = \lim_{n \to \infty} \mu(f_n)$ với mọi $\mu$ trong $C(X)'$.

Mệnh đề 3. — Cho X là một không gian compact, và cho A là một tập con bị chặn của $C(X)$. Để A là tương đối compact đối với tôpô hội tụ đơn, điều kiện cần và đủ là nó tương đối compact đối với $\sigma(C(X), C(X)')$.

Tôpô hội tụ đơn là Hausdorff và thô hơn $\sigma(C(X), C(X)')$, nên điều kiện đã nêu là đủ (GT, I, § 9, No. 4, hệ quả 3).

Bây giờ giả sử rằng A là tương đối compact đối với tôpô hội tụ đơn. Cho $(f_n)_{n \in \mathbf{N}}$ là một dãy các phần tử của A. Theo mệnh đề 2 (IV, p. 33), tồn tại một dãy $(f_{n_k})$ trích từ $(f_n)$ và hội tụ đơn tới một hàm liên tục f. Theo bổ đề 2, dãy bị chặn $(f_{n_k})$ hội tụ tới f theo $\sigma(C(X), C(X)')$. Khi đó định lý của Šmulian (IV, p. 36, định lý 2) cho thấy rằng A là tương đối compact đối với $\sigma(C(X), C(X)')$.

Hệ quả. — Cho S là một không gian tôpô và A là một tập con bị chặn của $C^b(S)$. Các điều kiện sau là tương đương :
(i) A là tương đối compact đối với $\sigma(C^b(S), C^b(S'))$;
(ii) nếu $(f_n)_{n \in \mathbf{N}}$ là một dãy các phần tử của A và $(x_m)_{m \in \mathbf{N}}$ là một dãy các điểm của S sao cho các giới hạn lặp
$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$
tồn tại, thì $\gamma = \delta$.

Cho X là phép compact hóa Stone-Čech của S (GT, IX, § 1, No. 6) và $\alpha$ là ánh xạ chính tắc từ S vào X. Đặt D = $\alpha(S)$. Ánh xạ $\phi : f \mapsto f \circ \alpha$ là một đẳng cấu từ không gian định chuẩn $C(X)$ lên không gian định chuẩn $C^b(S)$; đặt $\tilde{A} = \phi^{-1}(A)$. Vì X là compact và D trù mật trong X, mệnh đề 2 (IV, p. 33) cho thấy rằng điều kiện (ii) là tương đương với tính compact của $\tilde{A}$ đối với tôpô hội tụ đơn. Khi đó tính tương đương của (i) và (ii) suy ra từ mệnh đề 3. \*

### \*5. Bao lồi của một tập compact yếu

#### Định lý 3 (Krein) {#evt-iv-s5-thm-3 .statement}

Cho E là một không gian lồi địa phương Hausdorff và đầy đủ giả, và cho $\mathcal{T}$ là một tôpô trên E tương thích với đối ngẫu giữa E và E'. Cho A là một tập con của E compac đối với $\mathcal{T}$. Khi đó bao lồi cân bằng đóng C của A là compac đối với $\mathcal{T}$.

Trước hết ta sẽ thực hiện một số phép quy giản.
A) Tập C là tiền compac đối với $\mathcal{T}$ (II, p. 25, mệnh đề 3), và A là compac đối với $\sigma(E, E')$. Chiếu theo mệnh đề 1 (IV, p. 32), chỉ cần chứng minh rằng C là compac đối với $\sigma(E, E')$, và do đó ta đã quy về trường hợp $\mathcal{T} = \sigma(E, E')$.
B) Vì C là tiền compac và đóng đối với $\sigma(E, E')$, nó bị chặn và đóng đối với tôpô ban đầu của E (III, p. 3, mệnh đề 2 và IV, p. 1, mệnh đề 1); do đó nó là đầy đủ vì E là đầy đủ giả. Nói cách khác, C là bao lồi cân bằng đóng của $ A $ trong hoàn thành $ \hat{E} $ của $ E $. Vì tôpô $ \sigma(\hat{E}, E') $ cảm sinh $ \sigma(E, E') $ trên $ E $, ta đã quy về *trường hợp khi $ E $ là đầy đủ*.

C) Cho $ \Gamma $ là bao lồi cân bằng của $ A $. Khi đó $ C $ là bao đóng của $ \Gamma $ đối với $ \sigma(E, E') $. Theo định lý Eberlein (IV, p. 35, đ.l. 1), chỉ cần chứng minh rằng mọi dãy $ (x_n)_{n \in \mathbf{N}} $ các điểm của $ \Gamma $ đều có một điểm giới hạn đối với $ \sigma(E, E') $ trong $ E $. Nhưng $ x_n $ thuộc bao lồi cân bằng của một tập con hữu hạn $ B_n $ của $ A $. Gọi $ F $ là không gian con vectơ đóng của $ E $ sinh bởi tập hợp đếm được $ B = \bigcup_n B_n $. Khi đó $ F $ là đầy đủ, tôpô $ \sigma(F, F') $ trên $ F $ được cảm sinh bởi $ \sigma(E, E') $ và ta có $ x_n \in F $ với mọi $ n \in \mathbf{N} $. Vậy chỉ cần chứng minh rằng $ (x_n)_{n \in \mathbf{N}} $ có một điểm giới hạn đối với $ \sigma(F, F') $, điều này dẫn đến sự quy giản về *trường hợp tồn tại một tập hợp trù mật đếm được trong $ E $*.

Cho $ A $ được gán tôpô cảm sinh bởi $ \sigma(E, E') $, tôpô này làm cho nó thành một không gian compact. Ta định nghĩa một ánh xạ tuyến tính $ u : E' \to \mathcal{C}(A) $ bởi

$$
u(x')(a) = \langle a, x' \rangle \quad (a \in A, x' \in E') .
$$

Cho $ (x'_n)_{n \in \mathbf{N}} $ là một dãy đồng liên tục trong $ E' $, hội tụ về 0 đối với $ \sigma(E', E) $. Khi đó dãy các hàm $ u(x'_n) $ bị chặn trong $ \mathcal{C}(A) $ và hội tụ đơn giản về 0. Với mọi $ \mu \in \mathcal{C}(A)' $, ta có $ \lim_{n \to \infty} \mu(u(x'_n)) = 0 $ theo bổ đề 2 (IV, p. 37). Theo tiêu chuẩn đã cho trong nhận xét ở III, p. 21, dạng tuyến tính $ \mu \circ u $ trên $ E' $ khi đó là liên tục đối với $ \sigma(E', E) $ với mọi $ \mu \in \mathcal{C}(A)' $. Do đó tồn tại một ánh xạ tuyến tính $ v : \mathcal{C}(A)' \to E $ thỏa mãn quan hệ

$$
\langle u(x'), \mu \rangle = \langle v(\mu), x' \rangle \quad (x' \in E', \mu \in \mathcal{C}(A)') .
$$

Rõ ràng là $ v $ liên tục nếu $ \mathcal{C}(A)' $ được trang bị tôpô $ \sigma(\mathcal{C}(A)', \mathcal{C}(A)) $ và $ E $ tôpô $ \sigma(E, E') $.

Quả cầu đơn vị (đóng) $ B $ của không gian Banach $ \mathcal{C}(A) $ là compact đối với tôpô $ \sigma(\mathcal{C}(A)', \mathcal{C}(A)) $ (III, p. 17, hệ quả 3). Do đó, $ v(B) $ là một tập con lồi, cân bằng và compact của $ E $ đối với $ \sigma(E, E') $. Với mọi $ a \in A $, dạng tuyến tính liên tục $ \varepsilon_a : f \mapsto f(a) $ trên $ \mathcal{C}(A) $ thuộc $ B $, và ta có $ v(\varepsilon_a) = a $ theo các công thức (7) và (8). Suy ra $ A \subset v(B) $, và vì thế $ C \subset v(B) $. Điều này chứng minh rằng $ C $ là compact đối với $ \sigma(E, E') $.

Q.E.D.

### Bài tập {#evt-iv-s5-exercises}

Xem [bài tập cho § 5](exercises/s5/).
