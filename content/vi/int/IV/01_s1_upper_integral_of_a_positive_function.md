---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 1
section_title: Upper integral of a positive function
lang: vi
source: int-i-vi
pdf_pages: 0108-0118, 0225-0227
extraction: ocr
subsections:
    - "no": 1
      title: Upper integral of a lower semi-continuous positive function
      page: 0
      pdf_page: 108
    - "no": 2
      title: Outer measure of an open set
      page: 4
      pdf_page: 111
    - "no": 3
      title: Upper integral of a positive function
      page: 6
      pdf_page: 113
    - "no": 4
      title: Outer measure of an arbitrary set
      page: 10
      pdf_page: 117
statements: 34
exercises: 8
content_sha256: 248ece4171f98318144858e172dbe8ae135d79da347aff2f4e261c922669d86b
translated_from: content/en/int/IV/01_s1_upper_integral_of_a_positive_function.md
source_content_sha256: e5ef9bf2f4017611f76e55300bcf998cbe85db5496f00758c65208639bce4f88
translation_model: gpt-5.4
translation_run: translate-vi-cbe59f39
glossary_version: 34
glossary_terms_sha256: 6078b7cce7c3a561b0ade80547670b0e34506686db512dcba2939e531620dd6e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. TÍCH PHÂN TRÊN CỦA MỘT HÀM DƯƠNG

### 1. Tích phân trên của một hàm dương nửa liên tục dưới

Cho X là một không gian compact địa phương, $ \mu $ một độ đo dương trên X; ta biết rằng $ \mu $ là một hàm tăng trên dàn $ \mathcal{K}_+(X) $ (dàn này cũng sẽ được ký hiệu là $ \mathcal{K}_+ $).

Ta ký hiệu bởi $ \mathcal{I}_+(X) $ (hoặc đơn giản là $ \mathcal{I}_+ $) tập hợp các hàm số trên X, hữu hạn hoặc không, dương và nửa liên tục dưới trên X.\footnote{1} Nhắc lại rằng tổng của một họ bất kỳ các hàm thuộc $ \mathcal{I}_+ $ thuộc $ \mathcal{I}_+ $; tích của một hàm thuộc $ \mathcal{I}_+ $ với một số hữu hạn $ \alpha > 0 $ thuộc $ \mathcal{I}_+ $; bao trên của *mọi* họ hàm thuộc $ \mathcal{I}_+ $ và bao dưới của một họ *hữu hạn* các hàm thuộc $ \mathcal{I}_+ $ cũng thuộc $ \mathcal{I}_+ $ (GT, IV, §6, No. 2, Mệnh đề 2 và Định lý 4). Ta cũng sẽ dùng bổ đề sau:

#### Bổ đề {#int-iv-s1-n1-lem-1 .statement}

— *Mọi hàm* $ f \in \mathcal{I}_+ $ *đều là bao trên của tập hợp* (có hướng đối với quan hệ $ \leq $) *của mọi hàm* $ g \in \mathcal{K}_+ $ *sao cho* $ g \leq f $.

Với mọi $ x \in X $ sao cho $ f(x) > 0 $, và với mọi số thực $ a $ sao cho $ 0 < a < f(x) $, theo giả thiết tồn tại một lân cận compắc V của $ x $ sao cho $ f(y) \geq a $ trên V; mặt khác, tồn tại một hàm $ g \in \mathcal{K}_+ $, có giá được chứa trong V, bằng $ a $ tại điểm $ x $ và $ \leq a $

\footnotetext{1 'I' như trong 'inferior'; chữ cái $ \mathcal{L} $ (như trong 'lower') đã được dành cho các không gian hàm khác, sẽ được bàn trong §3.}

trên V (GT, IX, §1, No. 5, Định lý 2); do đó $ 0 \leq g \leq f $ và $ g(x) \geq a $, điều này chứng minh bổ đề.

#### Định nghĩa 1 {#int-iv-s1-def-1 .statement}

*Cho một độ đo dương $ \mu $ trên $ X $, người ta gọi tích phân trên của một hàm $ f \in \mathcal{J}_+ $ (đối với $ \mu $) là số dương (hữu hạn hoặc bằng $ +\infty $)*

$$
\mu^*(f) = \sup_{g \in \mathcal{H}_+, g \leq f} \mu(g).
$$

Đối với mọi hàm $ f \in \mathcal{H}_+ $, rõ ràng là $ \mu^*(f) = \mu(f) $, nói cách khác $ \mu^* $ là một *mở rộng* của $ \mu $ lên $ \mathcal{J}_+ $.

#### Ví dụ {#int-iv-s1-n1-exa-1 .statement}

— Cho $ X $ là một không gian *rời rạc*, $ \mu $ là một độ đo dương trên $ X $, và đặt $ \alpha(x) = \mu(\varphi_{\{x\}}) $ với mọi $ x \in X $. Khi đó mọi hàm số trị số $ f $ xác định trên $ X $ đều liên tục; đối với một hàm như vậy thỏa $ f \geq 0 $, ta có $ \mu^*(f) = \sum_{x \in X} \alpha(x)f(x) $, trong đó ta quy ước đặt $ \alpha(x)f(x) = 0 $ mỗi khi $ \alpha(x) = 0 $ và $ f(x) = +\infty $. Thật vậy,
$$
\sum_{x \in X} \alpha(x)f(x) = \sup_M \left( \sum_{x \in M} \alpha(x)f(x) \right),
$$
trong đó $ M $ chạy qua tập hợp tất cả các tập con hữu hạn của $ X $. Nếu tồn tại một $ x_0 \in X $ sao cho $ f(x_0) = +\infty $ và $ \alpha(x_0) > 0 $, thì $ \sum_{x \in M} \alpha(x)f(x) = +\infty $ mỗi khi $ x_0 \in M $, và mặt khác $ f \geq n \cdot \varphi_{\{x_0\}} $ với mọi số nguyên $ n > 0 $, do đó $ \mu^*(f) \geq n \alpha(x_0) $ và vì thế $ \mu^*(f) = +\infty $. Nếu ngược lại, $ \alpha(x) = 0 $ tại mọi điểm mà ở đó $ f(x) = +\infty $, thì hàm $ g $ bằng $ f $ tại các điểm $ x \in M $ mà $ \alpha(x) > 0 $ và bằng 0 ở nơi khác thuộc $ \mathcal{H}_+ $, và do đó, theo các quy ước đã đặt ra, $ \mu(g) = \sum_{x \in M} \alpha(x)f(x) $, điều này lại chứng minh quan hệ $ \mu^*(f) = \sum_{x \in X} \alpha(x)f(x) $.

#### Mệnh đề 1 {#int-iv-s1-prop-1 .statement}

*Với mọi số thực hữu hạn $ \alpha > 0 $ và mọi hàm $ f \in \mathcal{J}_+ $,*
$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### Mệnh đề 2 {#int-iv-s1-prop-2 .statement}

*Trên tập hợp $ \mathcal{J}_+ $, hàm $ \mu^* $ là tăng.*
Các chứng minh suy ra ngay lập tức từ Định nghĩa 1.

#### Định lý 1 {#int-iv-s1-thm-1 .statement}

*Cho $ H $ là một tập hợp khác rỗng các hàm trong $ \mathcal{J}_+ $, có hướng đối với quan hệ $ \leq $. Với mọi độ đo dương $ \mu $ trên $ X $,*
$$
\mu^*\left( \sup_{g \in H} g \right) = \sup_{g \in H} \mu^*(g) = \lim_{g \in H} \mu^*(g).
$$

Cho $ f = \sup_{g \in H} g $. Trước hết ta sẽ chứng minh định lý trong trường hợp riêng khi các hàm $ g \in H $ và bao trên của chúng $ f $ *thuộc* $ \mathcal{H}_+ $. Khi đó, theo định lý Dini (GT, X, §4, No. 1, ĐL. 1), bộ lọc các tiết diện của $ H $ hội tụ *đều* tới $ f $ trên mọi tập compắc con của $ X $, và đặc biệt trên giá đỡ K của $ f $. Vì $ 0 \leq g \leq f $ đối với mọi hàm $ g \in \mathbf{H} $, giá đỡ của mọi hàm trong $ \mathbf{H} $ đều được chứa trong $ K $; nhưng theo định nghĩa, $ \mu $ liên tục trên không gian vectơ $ \mathcal{K}(X, K; \mathbf{C}) $ của các hàm liên tục có giá đỡ được chứa trong $ K $, đối với tôpô hội tụ đều; do đó có quan hệ (2) trong trường hợp này.

Xét trường hợp tổng quát. Rõ ràng là $ \mu^*(g) \leq \mu^*(f) $ đối với mọi hàm $ g \in \mathbf{H} $. Theo Định nghĩa 1, toàn bộ vấn đề quy về việc chứng minh rằng, với mọi hàm $ \psi \in \mathcal{K}_+ $ sao cho $ \psi \leq f $,

$$
\mu(\psi) \leq \sup_{g \in \mathbf{H}} \mu^*(g).
$$

Với mọi hàm $ g \in \mathbf{H} $, gọi $ \Phi_g $ là tập hợp các hàm $ \varphi \in \mathcal{K}_+ $ sao cho $ \varphi \leq g $, và gọi $ \Phi $ là hợp của các tập hợp $ \Phi_g $ khi $ g $ chạy trên $ \mathbf{H} $; vì $ \mathbf{H} $ có hướng nên $ \Phi $ cũng có hướng, và $ f = \sup_{\varphi \in \Phi} \varphi $. Vì $ \psi \leq f $, nên $ \psi $ là bao trên của tập hợp các hàm $ \inf(\psi, \varphi) $ khi $ \varphi $ chạy trên $ \Phi $; nhưng vì $ \psi $ và các hàm $ \inf(\psi, \varphi) $ thuộc $ \mathcal{K}_+ $, nên phần đầu của chứng minh cho thấy rằng $ \mu(\psi) = \sup_{\varphi \in \Phi} \mu(\inf(\psi, \varphi)) $. Bây giờ, mỗi $ \varphi \in \Phi $ thuộc một tập hợp $ \Phi_g $, do đó

$$
\mu(\inf(\psi, \varphi)) \leq \mu(\varphi) \leq \mu^*(g) \leq \sup_{g \in \mathbf{H}} \mu^*(g),
$$

từ đó suy ra ngay rằng $ \mu(\psi) \leq \sup_{g \in \mathbf{H}} \mu^*(g) $. Như vậy ta đã chứng minh rằng $ \mu^*(f) = \sup_{g \in \mathbf{H}} \mu^*(g) $; quan hệ $ \mu^*(f) = \lim_{g \in \mathbf{H}} \mu^*(g) $ khi đó là một hệ quả của định lý giới hạn đơn điệu (GT, IV, §5, No. 2, Th. 2).

#### Định lý 2 {#int-iv-s1-thm-2 .statement}

*Nếu $ f_1 $ và $ f_2 $ là hai hàm thuộc $ \mathcal{I}_+ $ thì*

$$
\mu^*(f_1 + f_2) = \mu^*(f_1) + \mu^*(f_2).
$$

Khi $ \varphi_1 $ (tương ứng $ \varphi_2 $) chạy qua tập các hàm trong $ \mathcal{K}_+ $ sao cho $ \varphi_1 \leq f_1 $ (tương ứng $ \varphi_2 \leq f_2 $), các hàm $ \varphi_1 + \varphi_2 $ tạo thành một tập có hướng (đối với $ \leq $) có bao trên là $ f_1 + f_2 $. Vì vậy, theo Định lý 1,

$$
\mu^*(f_1 + f_2) = \sup \mu(\varphi_1 + \varphi_2) = \sup (\mu(\varphi_1) + \mu(\varphi_2)),
$$

trong đó $ (\varphi_1, \varphi_2) $ chạy qua tập các cặp hàm trong $ \mathcal{K}_+ $ sao cho $ \varphi_1 \leq f_1 $ và $ \varphi_2 \leq f_2 $; vì

$$
\sup (\mu(\varphi_1) + \mu(\varphi_2)) = \sup \mu(\varphi_1) + \sup \mu(\varphi_2)
$$

(GT, IV, §5, No. 7, Hệ quả 2 của Mệnh đề 12), nên định lý được chứng minh.

#### Mệnh đề 3 {#int-iv-s1-prop-3 .statement}

— *Với mọi họ* $(f_\iota)_{\iota \in I}$ *các hàm trong* $J_+$,

$$
\mu^*\left( \sum_{\iota \in I} f_\iota \right) = \sum_{\iota \in I} \mu^*(f_\iota).
$$

Với mọi tập con hữu hạn $J$ của $I$, suy ra từ Định lý 2 (bằng quy nạp theo số phần tử của $J$) rằng $\mu^*\left( \sum_{\iota \in J} f_\iota \right) = \sum_{\iota \in J} \mu^*(f_\iota)$; khi $J$ chạy qua tập hợp các tập con hữu hạn của $I$, các hàm $g_J = \sum_{\iota \in J} f_\iota$ thuộc $J_+$ và tạo thành một tập có hướng đối với quan hệ $\leq$, mà bao trên của nó là hàm $\sum_{\iota \in I} f_\iota$; do đó mệnh đề được suy ra từ Định lý 1.

#### Mệnh đề 4 {#int-iv-s1-prop-4 .statement}

— *Cho* $f$ *là một hàm trong* $J_+$. *Ánh xạ* $\mu \mapsto \mu^*(f)$ *của tập hợp* $\mathcal{M}_+(X)$ *các độ đo dương trên* $X$, *vào đường thẳng thực mở rộng* $\overline{\mathbf{R}}$, *là nửa liên tục dưới đối với tôpô mơ hồ trên* $\mathcal{M}_+(X)$ *(Ch. III, §1, No. 9)*.

Thật vậy, ánh xạ này theo định nghĩa là bao trên của các ánh xạ $\mu \mapsto \mu(g)$, trong đó $g$ chạy qua tập hợp các hàm trong $\mathcal{K}_+$ sao cho $g \leq f$; và theo định nghĩa của tôpô mơ hồ, các ánh xạ $\mu \mapsto \mu(g)$ là liên tục trên $\mathcal{M}(X)$.

### 2. Độ đo ngoài của một tập hợp mở

Cho một tập hợp *mở* $G \subset X$, hàm đặc số $\varphi_G$ của nó là *nửa liên tục dưới* trên $X$ (GT, IV, §6, No. 2, Hệ quả của Mệnh đề 1). Vì vậy ta có thể đưa ra định nghĩa sau:

#### Định nghĩa 2 {#int-iv-s1-def-2 .statement}

— *Cho một độ đo dương* $\mu$ *trên* $X$, *với mọi tập hợp mở* $G \subset X$ *tích phân trên* $\mu^*(\varphi_G)$ *được gọi là độ đo ngoài của* $G$ *và được ký hiệu là* $\mu^*(G)$.

Do đó độ đo ngoài của một tập hợp mở $G$ là một số $\geq 0$, hữu hạn hoặc bằng $+\infty$. Rõ ràng $\mu^*(\varnothing) = 0$. Hơn nữa, $\mu^*(X) = \| \mu \|,$ như được chỉ ra bởi công thức (22) của Ch. III, §1, No. 8.

#### Mệnh đề 5 {#int-iv-s1-prop-5 .statement}

— *Độ đo ngoài của một tập hợp mở compact tương đối* $G$ *là hữu hạn*.

Vì, trong trường hợp này, tồn tại một hàm $f \in \mathcal{K}_+$ sao cho $\varphi_G \leq f$ (Ch. III, §1, No. 2, Bổ đề 1), do đó

$$
\mu^*(G) = \mu^*(\varphi_G) \leq \mu^*(f) = \mu(f) < +\infty.
$$

Một tập hợp mở có ngoại độ đo hữu hạn không phải lúc nào cũng là tương đối compắc (Bài tập 3).

#### Mệnh đề 6 {#int-iv-s1-prop-6 .statement}

— *Nếu* G₁ và G₂ *là hai tập hợp mở sao cho* G₁ ⊂ G₂, *thì* μ*(G₁) ≤ μ*(G₂).
Thật vậy, quan hệ G₁ ⊂ G₂ tương đương với φG₁ ≤ φG₂.

#### Mệnh đề 7 {#int-iv-s1-prop-7 .statement}

— *Cho* 𝔅 *là một tập hợp các tập con mở của* X *có hướng đối với quan hệ* ⊂; *khi đó*

$$
\mu^*\left(\bigcup_{G \in \mathfrak{B}} G\right) = \sup_{G \in \mathfrak{B}} \mu^*(G).
$$

Các hàm φ_G lập thành một tập có hướng (đối với ≤) trong $ \mathcal{I}_+ $ và bao trên của chúng là hàm đặc số của hợp các tập hợp G ∈ 𝔅; vì vậy mệnh đề là một hệ quả của Định lý 1.

#### Mệnh đề 8 {#int-iv-s1-prop-8 .statement}

— *Cho* (G_ι)_{ι \in I} *là một họ bất kỳ các tập hợp mở; khi đó*

$$
\mu^*\left(\bigcup_{ι \in I} G_ι\right) \leq \sum_{ι \in I} \mu^*(G_ι).
$$

*Hơn nữa, nếu các* G_ι *rời nhau từng đôi một thì*

$$
\mu^*\left(\bigcup_{ι \in I} G_ι\right) = \sum_{ι \in I} \mu^*(G_ι).
$$

Thật vậy, nếu G = $ \bigcup_{ι \in I} G_ι $ thì φ_G = sup_{ι \in I} φ_{G_ι} ≤ $ \sum_{ι \in I} \varphi_{G_ι} $; khi các G_ι rời nhau từng đôi một, φ_G = $ \sum_{ι \in I} \varphi_{G_ι} $; do đó mệnh đề là một hệ quả của các Mệnh đề 2 và 3.

#### Ví dụ {#int-iv-s1-n2-exa-1 .statement}

— Cho X = \mathbf{R} và cho μ là độ đo Lebesgue trên \mathbf{R} (Ch. III, §1, No. 3); chúng ta sẽ xác định ngoại độ đo của một *khoảng mở* G = ]a, b[ (−∞ ≤ a < b ≤ +∞). Trước hết giả sử rằng a và b là hữu hạn. Với mọi hàm f trong $ \mathcal{K}_+ $ sao cho f ≤ φ_G, ta có, theo định lý giá trị trung bình (FRV, II, §1, No. 5, Prop. 6),

$$
\int_{-\infty}^{+\infty} f(x)\, dx = \int_a^b f(x)\, dx \leq b - a,
$$

do đó $ \mu^*(G) \leq b - a $. Mặt khác, với mọi $ \varepsilon > 0 $ tồn tại một hàm $ f \in \mathcal{K}_+ $ sao cho $ f \leq \varphi_G $ và $ f(x) = 1 $ với $ a + \varepsilon \leq x \leq b - \varepsilon $, do đó $ \mu^*(G) \geq b - a - 2\varepsilon $; vì $ \varepsilon $ là tùy ý, nên $ \mu^*(G) = b - a $; nói cách khác, độ đo ngoài của $ G $ bằng *độ dài* của nó. Kết quả này mở rộng ngay cho trường hợp $ G $ là một khoảng mở không bị chặn, vì khi đó nó chứa các khoảng mở bị chặn có độ dài lớn tùy ý; do đó trong trường hợp này $ \mu^*(G) = +\infty $.

Bây giờ xét $ G $ là một tập mở bất kỳ trong $ \mathbf{R} $; $ G $ là hợp của một tập đếm được (hữu hạn hoặc vô hạn) các khoảng mở rời nhau từng đôi một $ ]a_k, b_k[ $ (GT, IV, §2, No. 5, Prop. 2), do đó

$$
\mu^*(G) = \sum_k (b_k - a_k)
$$

(Mệnh đề 8); nói cách khác:

#### Mệnh đề 9 {#int-iv-s1-prop-9 .statement}

*Đối với độ đo Lebesgue trên $ \mathbf{R} $, độ đo ngoài của một tập mở trong $ \mathbf{R} $ bằng tổng các độ dài của các thành phần liên thông của nó.*

Đặc biệt chú ý rằng nếu $ G $ là một tập mở trong $ \mathbf{R} $ sao cho $ \mu^*(G) = 0 $, thì $ G $ là *rỗng*.

### 3. Tích phân trên của một hàm dương

Với mọi hàm số $ f \geq 0 $ (hữu hạn hoặc không) xác định trên $ X $, tồn tại các hàm $ h \in \mathcal{I}_+ $ sao cho $ f \leq h $, nếu không có hàm nào khác thì ít ra cũng có hàm hằng $ +\infty $.

#### Định nghĩa 3 {#int-iv-s1-def-3 .statement}

*Cho $ \mu $ là một độ đo dương trên $ X $; với mọi hàm số $ f \geq 0 $ (hữu hạn hoặc không) xác định trên $ X $, số dương*

$$
\mu^*(f) = \inf_{h \geq f, h \in \mathcal{I}_+} \mu^*(h)
$$

(*hữu hạn hoặc bằng $ +\infty $) *được gọi là tích phân trên của $ f $ (đối với $ \mu $).*

Khi $ f \in \mathcal{I}_+ $, số $ \mu^*(f) $ được định nghĩa như vậy bằng với tích phân trên được định nghĩa trong Đn. 1, vì $ \mu^* $ tăng trên $ \mathcal{I}_+ $.

Thay cho ký hiệu $ \mu^*(f) $, chúng tôi cũng sẽ dùng các ký hiệu $ \int^* f d\mu $, $ \int^* f(x) d\mu(x) $, $ \int^* f \mu $ và $ \int^* f(x) \mu(x) $.

#### Ví dụ {#int-iv-s1-n3-exa-1 .statement}

— Nếu $ X $ là một không gian *rời rạc*, $ \mu $ là một độ đo dương trên $ X $, và nếu đặt $ \alpha(x) = \mu(\varphi_{\{x\}}) $, thì $ \mu^*(f) = \sum_{x \in X} \alpha(x) f(x) $ với mọi hàm số $ f \geq 0 $ xác định trên $ X $, vì một hàm như vậy là liên tục (No. 1, *Ví dụ*).

#### Mệnh đề 10 {#int-iv-s1-prop-10 .statement}

— *Nếu f và g là hai hàm số $ \geqslant 0 $ xác định trên X sao cho $ f \leqslant g $, thì $ \mu^*(f) \leqslant \mu^*(g) $.*

#### Mệnh đề 11 {#int-iv-s1-prop-11 .statement}

— *Với mọi số thực hữu hạn $ \alpha > 0 $ và mọi hàm số $ f \geqslant 0 $ xác định trên X,

$$
\mu^*(\alpha f) = \alpha \mu^*(f).
$$

#### Mệnh đề 12 {#int-iv-s1-prop-12 .statement}

— *Nếu $ f_1 $ và $ f_2 $ là hai hàm số trị số $ \geqslant 0 $ xác định trên X, thì

$$
\mu^*(f_1 + f_2) \leqslant \mu^*(f_1) + \mu^*(f_2).
$$

Với mọi hàm $ h_1 \in \mathcal{I}_+ $ sao cho $ f_1 \leqslant h_1 $ và mọi hàm $ h_2 \in \mathcal{I}_+ $ sao cho $ f_2 \leqslant h_2 $, theo ĐL. 2 ta có

$$
\mu^*(f_1 + f_2) \leqslant \mu^*(h_1 + h_2) = \mu^*(h_1) + \mu^*(h_2),
$$
do đó (GT, IV, §5, No. 7, Hệ quả 2 của Mệnh đề 12)

$$
\mu^*(f_1 + f_2) \leqslant \inf_{h_1 \geqslant f_1, h_1 \in \mathcal{I}_+} \mu^*(h_1) + \inf_{h_2 \geqslant f_2, h_2 \in \mathcal{I}_+} \mu^*(h_2),
$$
đó chính là bất đẳng thức (9).

Các Mệnh đề 10, 11 và 12 biểu thị rằng $ \mu^* $ là một hàm *tăng, thuần nhất dương* và *lồi* trên tập hợp các hàm số trị số $ \geqslant 0 $ xác định trên X (Ch. I, No. 1). Chú ý rằng nếu $ f_1 $ và $ f_2 $ là hai hàm dương bất kỳ, thì hai vế của (9) không nhất thiết bằng nhau (\$4, Exer. 8 d)); trong §5, No. 6 chúng tôi sẽ cho các điều kiện để có đẳng thức.

#### Định lý 3 {#int-iv-s1-thm-3 .statement}

— *Với mọi dãy tăng $ (f_n) $ các hàm số $ \geqslant 0 $ xác định trên X,

$$
\mu^*\left( \sup_n f_n \right) = \sup_n \mu^*(f_n).
$$

Vì mỗi hàm $ f_n $ đều nhỏ hơn hoặc bằng $ \sup_n f_n $, mọi sự quy về việc chứng minh rằng $ \mu^*(\sup_n f_n) \leqslant \sup_n \mu^*(f_n) $; điều này hiển nhiên nếu vế thứ hai của bất đẳng thức là $ +\infty $. Trong trường hợp ngược lại, $ \mu^*(f_n) < +\infty $ với mọi $ n $; ta sẽ chỉ ra rằng, với mọi $ \varepsilon > 0 $, tồn tại một dãy *tăng* $ (g_n) $ các hàm trong $ \mathcal{I}_+ $ sao cho $ f_n \leqslant g_n $ và $ \mu^*(g_n) \leqslant \mu^*(f_n) + \varepsilon $. Nếu $ g $ là bao trên của dãy $ (g_n) $, thì khi đó ta sẽ có $ \mu^*(g) = \sup_n \mu^*(g_n) $ (No. 1, Đl. 1), do đó $ \mu^*(g) \leqslant \sup \mu^*(f_n) + \varepsilon $; vì $ \sup f_n \leqslant g $ và $ \varepsilon $ là tùy ý, khi đó định lý sẽ được chứng minh.

Theo giả thiết, tồn tại một hàm $ h_n \in \mathcal{J}_+ $ sao cho $ f_n \leq h_n $ và $ \mu^*(f_n) \leq \mu^*(h_n) \leq \mu^*(f_n) + \varepsilon/2^n $; hãy chứng minh rằng các hàm $ g_n = \sup(h_1, h_2, \ldots, h_n) $ thỏa mãn các yêu cầu. Chúng thuộc $ \mathcal{J}_+ $, tạo thành một dãy tăng, và thỏa mãn $ f_n \leq g_n $ với mọi $ n $; ta sẽ chứng minh rằng

$$
\mu^*(g_n) \leq \mu^*(f_n) + \varepsilon \left( 1 - \frac{1}{2^n} \right).
$$

Ta lập luận bằng quy nạp theo $ n $; trường hợp $ n = 1 $ là tầm thường. Mặt khác $ g_{n+1} = \sup(g_n, h_{n+1}) $, $ g_n \geq f_n $ và $ h_{n+1} \geq f_{n+1} \geq f_n $, do đó $ \inf(g_n, h_{n+1}) \geq f_n $; vì

$$
\inf(g_n, h_{n+1}) + \sup(g_n, h_{n+1}) = g_n + h_{n+1},
$$

nên suy ra từ Định lý 2 của No. 1 rằng

$$
\begin{align*}
\mu^*(g_{n+1}) &= \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(\inf(g_n, h_{n+1})) \\
&\leq \mu^*(g_n) + \mu^*(h_{n+1}) - \mu^*(f_n) \\
&\leq \mu^*(f_{n+1}) + \varepsilon \left( 1 - \frac{1}{2^n} \right) + \frac{\varepsilon}{2^{n+1}} \\
&= \mu^*(f_{n+1}) + \varepsilon \left( 1 - \frac{1}{2^{n+1}} \right).
\end{align*}
$$

ĐPCM.

#### Hệ quả {#int-iv-s1-n3-cor-1 .statement}

— *Cho $ \mathfrak{F} $ là một tập hợp các hàm số $ \geq 0 $, có hướng đối với quan hệ $ \leq $, sao cho tồn tại một tập con đồng tận đếm được $ \mathfrak{G} $ của $ \mathfrak{F} $* (S, III, §1, No. 7); khi đó

$$
\mu^*\left( \sup_{f \in \mathfrak{F}} f \right) = \sup_{f \in \mathfrak{F}} \mu^*(f).
$$

Thật vậy, tồn tại một dãy tăng các hàm trong $ \mathfrak{G} $ có cùng bao trên như $ \mathfrak{F} $: nếu $ (f_n) $ là dãy các hàm của $ \mathfrak{G} $, được xếp theo một thứ tự tùy ý, thì đặt $ (f_{n_k}) $ là một dãy con được xác định đệ quy bởi các điều kiện $ n_1 = 1 $, $ f_{n_{k+1}} \geq \sup(f_{n_k}, f_k) $; hiển nhiên dãy con này có các tính chất đã nêu.

#### Nhận xét {#int-iv-s1-n3-rem-1 .statement}

— 1) Quan hệ (11) không nhất thiết đúng khi $ \mathfrak{F} $ là một tập có hướng *không đếm được* các hàm $ \geq 0 $ không nửa liên tục dưới. Chẳng hạn, lấy $ X = \mathbf{R} $, $ \mu $ là độ đo Lebesgue trên $ \mathbf{R} $, và xét tập có hướng (đối với $ \leq $) $ \mathfrak{F} $ gồm các hàm đặc trưng $ \varphi_M $ của mọi tập con *hữu hạn* M của $ \mathbf{R} $. Khi đó $ \mu^*(\varphi_M) = 0 $ với mọi tập con hữu hạn M, vì một điểm được chứa trong một khoảng mở có độ dài nhỏ tùy ý, và do đó hàm đặc trưng của một tập hợp thu về một điểm có tích phân trên bằng không theo Định nghĩa 3 và Mệnh đề 9 của No. 2. Nhưng bao trên của $ \mathcal{F} $ là hàm hằng bằng 1, và $ \mu^*(1) = +\infty $.

2) Chú ý rằng đối với một dãy *giảm* $ (f_n) $ các hàm số $ \geqslant 0 $, không nhất thiết có $ \mu^*(\inf_n f_n) = \inf_n \mu^*(f_n) $, ngay cả khi $ \mu^*(f_n) < +\infty $ với mọi $ n $ (xem §4, Exer. 8 c)).

#### Mệnh đề 13 {#int-iv-s1-prop-13 .statement}

*Với mọi dãy* $ (f_n) $ *các hàm số* $ \geqslant 0 $ *xác định trên* $ X $,

$$
\mu^*\left( \sum_{n=1}^\infty f_n \right) \leqslant \sum_{n=1}^\infty \mu^*(f_n).
$$

Chỉ cần áp dụng quan hệ (10) cho dãy tăng các hàm số $ g_n = \sum_{k=1}^n f_k $ đồng thời lưu ý rằng, theo (9),

$$
\mu^*(g_n) \leqslant \sum_{k=1}^n \mu^*(f_k).
$$

Trong §5, No. 6, chúng tôi sẽ nêu các điều kiện để hai vế của (12) bằng nhau.

#### Mệnh đề 14 (bổ đề Fatou) {#int-iv-s1-prop-14 .statement}

— *Với mọi dãy* $ (f_n) $ *các hàm số* $ \geqslant 0 $,

$$
\mu^*\left( \liminf_{n \to \infty} f_n \right) \leqslant \liminf_{n \to \infty} \mu^*(f_n).
$$

Với mọi số nguyên $ n $, đặt $ g_n = \inf_{p \geqslant 0} f_{n+p} $; dãy $ (g_n) $ là tăng và $ \liminf_{n \to \infty} f_n = \sup_n g_n $, do đó, theo (10),

$$
\mu^*(\liminf_{n \to \infty} f_n) = \sup_n \mu^*(g_n);
$$

nhưng vì $ g_n \leqslant f_{n+p} $ với $ p \geqslant 0 $, ta có $ \mu^*(g_n) \leqslant \mu^*(f_{n+p}) $, do đó $ \mu^*(g_n) \leqslant \inf_{p \geqslant 0} \mu^*(f_{n+p}) $ và cuối cùng

$$
\mu^*\left( \liminf_{n \to \infty} f_n \right) \leqslant \sup_n \left( \inf_{p \geqslant 0} \mu^*(f_{n+p}) \right) = \liminf_{n \to \infty} \mu^*(f_n).
$$

#### Hệ quả {#int-iv-s1-n3-cor-2 .statement}

*Cho* $ (f_n) $ *là một dãy các hàm số* $ \geqslant 0 $ *sao cho, với mọi* $ x \in X $, $ \lim_{n \to \infty} f_n(x) = +\infty $. *Nếu* $ \mu $ *không phải là độ đo không, thì* $ \lim_{n \to \infty} \mu^*(f_n) = +\infty $.

Nếu $ f_0 $ là hàm hằng bằng $ +\infty $, thì $ f_0 $ là bao trên của tất cả các hàm của $ \mathcal{K}_+ $, và, vì $ \mu \neq 0 $, ta có $ \mu^*(f_0) > 0 $; nhưng do $ f_0 = \alpha f_0 $ với mọi $ \alpha > 0 $, tất yếu $ \mu^*(f_0) = +\infty $ (Mệnh đề 11). Khi đó bất đẳng thức (13) cho thấy rằng $ \mu^*(f_n) $ tiến tới $ +\infty $ khi $ n $ tăng.

#### Mệnh đề 15 {#int-iv-s1-prop-15 .statement}

*Với mọi vô hướng $ \alpha > 0 $ và mọi cặp độ đo dương $ \mu, \nu $ trên $ X $,*

$$
(\alpha \mu)^* = \alpha \mu^*
$$
$$
(\mu + \nu)^* = \mu^* + \nu^*.
$$

*Hơn nữa, quan hệ $ \mu \leq \nu $ kéo theo $ \mu^* \leq \nu^* $.*

Hãy chứng minh quan hệ (15). Đặt $ \lambda = \mu + \nu $; do đó $ \lambda(f) = \mu(f) + \nu(f) $ với $ f \in \mathcal{K}_+ $; với $ f \in \mathcal{J}_+ $, giá trị của $ \lambda^*(f) $ (tương ứng $ \mu^*(f) $, $ \nu^*(f) $) là giới hạn của $ \lambda(g) $ (tương ứng $ \mu(g) $, $ \nu(g) $) khi $ g $ chạy trên tập có hướng (đối với $ \leq $) gồm mọi $ g \in \mathcal{K}_+ $ sao cho $ g \leq f $; vì vậy $ \lambda^*(f) = \mu^*(f) + \nu^*(f) $. Cuối cùng, nếu $ f $ là một hàm bất kỳ $ \geq 0 $ xác định trên $ X $, thì $ \lambda^*(f) $ (tương ứng $ \mu^*(f) $, $ \nu^*(f) $) là giới hạn của $ \lambda^*(h) $ (tương ứng $ \mu^*(h) $, $ \nu^*(h) $) khi $ h $ chạy trên tập có hướng (đối với $ \geq $) gồm mọi hàm $ h \in \mathcal{J}_+ $ sao cho $ h \geq f $; một lần nữa, bằng cách chuyển sang giới hạn, do đó ta có $ \lambda^*(f) = \mu^*(f) + \nu^*(f) $, điều này chứng minh (15). Quan hệ (14) được thiết lập tương tự. Cuối cùng, nếu $ \mu \leq \nu $ thì ta có thể viết $ \nu = \mu + (\nu - \mu) $, trong đó $ \nu - \mu \geq 0 $, do đó $ \nu^* = \mu^* + (\nu - \mu)^* $, điều này cho thấy $ \mu^* \leq \nu^* $.

### 4. Độ đo ngoài của một tập hợp tùy ý

#### Định nghĩa 4 {#int-iv-s1-def-4 .statement}

*Cho $ \mu $ là một độ đo dương trên $ X $; với mọi tập con $ A $ của $ X $, tích phân trên $ \mu^*(\varphi_A) $ được gọi là độ đo ngoài của $ A $ (đối với độ đo $ \mu $) và được ký hiệu là $ \mu^*(A) $.*

Vậy độ đo ngoài của một tập hợp là một số $ \geq 0 $, hữu hạn hoặc bằng $ +\infty $, mà đối với một tập mở, trùng với độ đo ngoài được định nghĩa trong Định nghĩa 2 của No. 2.

#### Mệnh đề 16 {#int-iv-s1-prop-16 .statement}

*Nếu $ A $ và $ B $ là hai tập con của $ X $ sao cho $ A \subset B $, thì $ \mu^*(A) \leq \mu^*(B) $.*

#### Hệ quả {#int-iv-s1-n4-cor-1 .statement}

*Mọi tập compact tương đối trong $ X $ đều có độ đo ngoài hữu hạn.*

Thật vậy, một tập như vậy được chứa trong một tập mở compact tương đối (GT, I, §9, No. 7, Mệnh đề 10), mà độ đo ngoài của nó là hữu hạn (No. 2, Mệnh đề 5).

#### Mệnh đề 17 {#int-iv-s1-prop-17 .statement}

— *Nếu* $(A_n)$ *là một dãy tăng các tập con của X*, thì $\mu^*(\bigcup_n A_n) = \sup_n \mu^*(A_n)$.

#### Mệnh đề 18 {#int-iv-s1-prop-18 .statement}

— *Với mọi dãy* $(A_n)$ *các tập con của X*,

$$
\mu^*\left(\bigcup_n A_n\right) \leq \sum_n \mu^*(A_n).
$$

Các mệnh đề này là các bản dịch của các Mệnh đề 10 và 13 và của Định lý 3 của No. 3 cho các hàm đặc trưng của tập hợp.

#### Mệnh đề 19 {#int-iv-s1-prop-19 .statement}

— *Với mọi tập con A của X*, $\mu^*(A)$ *là cận dưới đúng của các độ đo ngoài của những tập mở chứa A*.

Mệnh đề là hiển nhiên nếu $\mu^*(A) = +\infty$. Trong trường hợp ngược lại, với mọi $\varepsilon$ sao cho $0 < \varepsilon < 1$, tồn tại một hàm $f \in \mathcal{J}_+$ sao cho $\varphi_A \leq f$ và $\mu^*(A) \leq \mu^*(f) \leq \mu^*(A) + \varepsilon$. Gọi G là tập hợp các $x \in X$ sao cho $f(x) > 1 - \varepsilon$. Vì $f$ là nửa liên tục dưới, G là *mở* (GT, IV, §6, No. 2, Prop. 1) và chứa A; mặt khác $f \geq (1 - \varepsilon)\varphi_G$, do đó

$$
\mu^*(G) \leq \frac{1}{1 - \varepsilon} \mu^*(f) \leq \frac{1}{1 - \varepsilon} (\mu^*(A) + \varepsilon);
$$

vì $\varepsilon$ là tùy ý, ta thấy rằng $\mu^*(G)$ sai khác với $\mu^*(A)$ ít đến mức tùy ý, do đó suy ra mệnh đề.

### Bài tập {#int-iv-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
