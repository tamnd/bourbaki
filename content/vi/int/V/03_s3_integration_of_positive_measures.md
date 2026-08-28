---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 3
section_title: Integration of positive measures
lang: vi
source: int-i-vi
book_pages: INT V.96-INT V.98
pdf_pages: 0270-0286, 0351-0353
extraction: ocr
subsections:
    - "no": 1
      title: Functions with values in a space of measures
      page: 0
      pdf_page: 270
    - "no": 2
      title: Superimposed integrals of positive functions
      page: 20
      pdf_page: 275
    - "no": 3
      title: Superimposed integrals of functions with values in a Banach space
      page: 24
      pdf_page: 279
    - "no": 4
      title: Universally measurable functions
      page: 25
      pdf_page: 280
    - "no": 5
      title: Diffusions
      page: 26
      pdf_page: 281
    - "no": 6
      title: Composition of bounded diffusions
      page: 29
      pdf_page: 284
statements: 30
exercises: 11
content_sha256: 11306991b1b7f0dcd6ac0bb13b57ca9f2559ef18b13a0939259151792731d3c3
translated_from: content/en/int/V/03_s3_integration_of_positive_measures.md
source_content_sha256: e1261c3f72bc79e2b7cb47c3cf24fb5d5a8d76df9ace5b843b9c4605464b3519
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4-mini
translation_run: translate-vi-56c0243e
glossary_version: 34
glossary_terms_sha256: 3403046be5e01809ad9ea1d80317d7fc384b2befb39de6a93aca5c7baa8bd3ca
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. TÍCH PHÂN CỦA CÁC ĐO DƯƠNG

### 1. Các hàm có giá trị trong một không gian các độ đo

Cho $X$ là một không gian compact địa phương, $\mathcal{M}_+(X)$ là nón lồi của các độ đo dương trên $X$. Trong suốt phần còn lại của chương này, $\mathcal{M}_+(X)$ sẽ được trang bị tôpô cảm sinh bởi tôpô yếu trên $\mathcal{M}(X)$ (Ch. III, §1, No. 9); do đó, nói rằng một ánh xạ $\Lambda : t \mapsto \lambda_t$ của không gian compact địa phương $T$ vào $\mathcal{M}_+(X)$ là liên tục có nghĩa là, với mọi hàm $f \in \mathcal{K}(X)$, hàm số $t \mapsto \lambda_t(f)$ là liên tục. Trong trường hợp này ta cũng sẽ nói rằng $\Lambda$ là liên tục yếu trên $T$. Nói rằng một ánh xạ $\Lambda : t \mapsto \lambda_t$ là $\mu$-đo được có nghĩa là tập hợp các tập con compact $K$ của $T$, sao cho hạn chế của $\Lambda$ lên $K$ là liên tục yếu, là

Cho $\Lambda : t \mapsto \lambda_t$ là một ánh xạ của T vào $\mathcal{M}_+(X)$; ta sẽ nói rằng Λ là khả tích cốt yếu vô hướng đối với độ đo μ nếu, với mọi hàm $f \in \mathcal{K}(X)$, hàm $t \mapsto \lambda_t(f)$ là khả tích cốt yếu μ. Nếu đặt $\nu(f) = \int \lambda_t(f)\, d\mu(t)$, thì rõ ràng ν là một dạng tuyến tính dương trên $\mathcal{K}(X)$, do đó là một độ đo trên X (Ch. III, §1, No. 5, Th. 1). Ta sẽ nói rằng ν là tích phân của hàm Λ có giá trị trong $\mathcal{M}_+(X)$, và ta sẽ viết $\nu = \int \lambda_t\, d\mu(t)$.

Định nghĩa trên là một trường hợp đặc biệt của khái niệm tích phân yếu, khái niệm này sẽ được xét một cách tổng quát trong Ch. VI.

Nếu $f$ biểu thị một phần tử của $\mathcal{K}(X)$, tích phân $\int \lambda_t(f)\, d\mu(t)$ cũng sẽ, do một sự lạm dụng ký hiệu, được ký hiệu là $\int d\mu(t) \int f(x)\, d\lambda_t(x)$; khi đó định nghĩa của tích phân $\nu = \int \lambda_t\, d\mu(t)$ có thể được viết

$$
\int f(x)\, d\nu(x) = \int d\mu(t) \int f(x)\, d\lambda_t(x).
$$

Ta sẽ thực hiện những sự lạm dụng ký hiệu tương tự trong phần sau, đối với các tích phân trên, các tích phân trên cốt yếu, và các tích phân của các hàm có giá trị trong một không gian Banach.

#### Ví dụ 1 {#int-v-s3-n1-exa-1 .statement}

Giả sử rằng T là một không gian rời rạc, và μ là độ đo trên T được xác định bằng cách đặt một khối lượng +1 tại mỗi điểm của T (Ch. III, §1, No. 3). Cho h là một hàm $\geqslant 0$ xác định trên T; vì hàm h là nửa liên tục dưới (thậm chí liên tục) trên T, $\mu^*(h) = \mu^\bullet(h) = \sum_{t \in T} h(t)$ (Ch. IV, §1, No. 1, Ví dụ).

Đối với độ đo μ, các khái niệm hàm khả tích và hàm khả tích cốt yếu do đó là đồng nhất. Như vậy, nói rằng một ánh xạ $t \mapsto \lambda_t$ của T vào $\mathcal{M}_+(X)$ là khả tích cốt yếu μ vô hướng tương đương với việc nói rằng họ $(\lambda_t)_{t \in T}$ là cộng được (§2, No. 1), và khi đó ta có $\int \lambda_t\, d\mu(t) = \sum_{t \in T} \lambda_t$. Chú ý rằng ánh xạ $t \mapsto \lambda_t$ là liên tục yếu.

#### Ví dụ 2 {#int-v-s3-n1-exa-2 .statement}

Ánh xạ $t \mapsto \varepsilon_t$ của T vào $\mathcal{M}_+(T)$ là liên tục yếu, khả tích cốt yếu μ vô hướng đối với mọi độ đo dương μ trên T, và ta có $\int \varepsilon_t\, d\mu(t) = \mu$.

#### Mệnh đề 1 {#int-v-s3-prop-1 .statement}

Giả sử rằng μ là cận trên của một họ có hướng tăng $(\mu_i)_{i \in I}$ các độ đo dương trên T; để $\Lambda : t \mapsto \lambda_t$ là khả tích cốt yếu μ vô hướng, điều kiện cần và đủ là Λ khả tích cốt yếu $\mu_i$ vô hướng với mọi $i \in I$ và họ $(\int \lambda_t\, d\mu_i(t))_{i \in I}$ bị chặn trên trong $\mathcal{M}(X)$. Khi đó,

$$
\int \lambda_t\, d\mu(t) = \sup_{i \in I} \int \lambda_t\, d\mu_i(t).
$$

Thật vậy, việc kiểm tra rằng $\Lambda$ là khả tích cốt yếu vô hướng đối với một độ đo dương $\eta$ trên $T$ quy về việc kiểm tra rằng $t \mapsto \lambda_t(g)$ là $\eta$-đo được và nhận một tích phân trên cốt yếu hữu hạn, đối với $\eta$, với mọi hàm $g \in \mathcal{H}_+(X)$. Vì vậy mệnh đề suy ra ngay từ Mệnh đề 11 của §1, No. 4 và Hệ quả 2 của nó.

#### Hệ quả {#int-v-s3-n1-cor-1 .statement}

— *Giả sử rằng $\mu$ là tổng của một họ khả tổng $(\mu_\alpha)_{\alpha \in A}$ các độ đo dương trên $T$; để cho $\Lambda : t \mapsto \lambda_t$ là khả tích vô hướng thiết yếu $\mu$, điều kiện cần và đủ là $\Lambda$ khả tích vô hướng thiết yếu $\mu_\alpha$ với mọi $\alpha \in A$ và họ các độ đo $\int \lambda_t d\mu_\alpha(t)$ là khả tổng. Khi đó ta có*

$$
\int \lambda_t d\mu(t) = \sum_{\alpha \in A} \int \lambda_t d\mu_\alpha(t).
$$

Suy ra ngay lập tức rằng mọi ánh xạ khả tích vô hướng thiết yếu $\mu$ cũng là khả tích vô hướng thiết yếu $\mu'$ đối với mọi độ đo $\mu' \leq \mu$.

Trong tiết này chúng ta sẽ chỉ giới hạn vào việc nghiên cứu các ánh xạ khả tích vô hướng thiết yếu từ $T$ vào $\mathcal{M}_+(X)$ có tính chất được xét đến trong định nghĩa sau:

#### Định nghĩa 1 {#int-v-s3-def-1 .statement}

— *Cho $X$ là một không gian compact địa phương, $\Lambda : t \mapsto \lambda_t$ là một ánh xạ khả tích vô hướng thiết yếu $\mu$ từ $T$ vào $\mathcal{M}_+(X)$, và $\nu$ là tích phân của $\Lambda$.

Ta nói rằng $\Lambda$ là $\mu$-tiền thích hợp nếu, với mọi hàm nửa liên tục dưới $f \geq 0$ xác định trên $X$, hàm $t \mapsto \int^\bullet f d\lambda_t$ là $\mu$-đo được trên $T$ và*

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

*Ta nói rằng $\Lambda$ là $\mu$-thích hợp (*) nếu $\Lambda$ là $\mu'$-tiền thích hợp đối với mọi độ đo dương $\mu' \leq \mu$.*

Có thể chứng minh rằng nếu $\Lambda$ là $\mu$-tiền thích hợp và nếu độ đo $\nu = \int \lambda_t d\mu(t)$ là điều hòa—đặc biệt nếu $X$ đếm được tại vô hạn—thì $\Lambda$ là $\mu$-thích hợp (Bài tập 7); tuy nhiên, hiện chưa biết liệu các khái niệm này nói chung có tương đương hay không. Trong các mệnh đề ở Số 2 và 3 dưới đây, các khẳng định đi trước bởi a) hoặc b) mở rộng ngay lập tức cho các ánh xạ tiền thích hợp, trong khi các khẳng định đi trước bởi c) chỉ đúng đối với các ánh xạ thích hợp.

(*) Trong ấn bản đầu tiên, các ánh xạ “$\mu$-thích hợp” được định nghĩa là các ánh xạ khả tích vô hướng thiết yếu $\mu$ và $\mu$-đo được yếu. Định nghĩa được cho ở đây tổng quát hơn (Mệnh đề 2 dưới đây).

Mệnh đề sau đây thường cho phép kiểm tra rằng một ánh xạ đã cho là $\mu$-thích hợp.

#### Mệnh đề 2 {#int-v-s3-prop-2 .statement}

— Cho $\Lambda : t \mapsto \lambda_t$ là một ánh xạ khả tích vô hướng thiết yếu $\mu$ từ $T$ vào $\mathcal{M}_+(X)$, và cho $\nu = \int \lambda_t \, d\mu(t)$.

a) *Nếu $\Lambda$ liên tục yếu, thì ánh xạ $t \mapsto \lambda_t^\bullet(f)$ là nửa liên tục dưới đối với mọi hàm nửa liên tục dưới $f \geqslant 0$ xác định trên $X$, $\Lambda$ là $\mu$-thích hợp, và ta có quan hệ*

$$
\int^* f(x) \, d\nu(x) = \int^* d\mu(t) \int^* f(x) \, d\lambda_t(x).
$$

b) *Nếu $\Lambda$ là đo được mơ hồ $\mu$, thì $\Lambda$ là $\mu$-thích hợp.*

c) *Nếu tôpô của $X$ có một cơ sở đếm được, thì $\Lambda$ là đo được mơ hồ $\mu$ (do đó cũng $\mu$-thích hợp).*

Cho $f$ là một hàm nửa liên tục dưới $\geqslant 0$ xác định trên $X$. Cho $F$ là tập hợp, có hướng đối với quan hệ $\leqslant$, của các hàm $g \in \mathcal{K}(X)$ sao cho $0 \leqslant g \leqslant f$. Với $g \in F$, ký hiệu $h_g$ là hàm xác định trên $T$ bởi $h_g(t) = \lambda_t(g)$. Tương tự, đặt

$$
h_f(t) = \lambda_t^*(f) = \lambda_t^\bullet(f) = \sup_{g \in F} h_g(t)
$$

(§1, No. 1, Mệnh đề 4). Ta đưa ra giả thiết sau đây, yếu hơn giả thiết trong a): chỉ giả sử rằng hạn chế của $\Lambda$ lên $S$ là liên tục mơ hồ, trong đó $S$ là một tập con đóng của $T$ chứa giá của $\mu$. Với $g \in F$, ký hiệu $\overline{h}_g$ là hàm số trùng với $h_g$ trên $S$ và có giá trị $+\infty$ trên $C_S$. Đặt $\overline{h}_f = \sup_{g \in F} \overline{h}_g$; khi đó $\overline{h}_f = h_f$ trên $S$. Với mọi $g \in F$, hàm $\overline{h}_g$ là nửa liên tục dưới; do đó $\overline{h}_f$ là nửa liên tục dưới và, vì họ $(\overline{h}_g)_{g \in F}$ là có hướng,

$$
\mu^*(\overline{h}_f) = \sup_{g \in F} \mu^*(\overline{h}_g) = \sup_{g \in F} \mu^*(h_g) = \sup_{g \in F} \nu(g) = \nu^*(f)
$$

(Ch. IV, §1, No. 1, Định lý 1 và §2, No. 3, Mệnh đề 6). Vì $h_f = \overline{h}_f$ trên $S$, do đó hầu khắp nơi, điều này cũng có thể được viết $\mu^*(h_f) = \nu^*(f)$, một đẳng thức đồng nhất với (5). Tương tự, vì $f$ và $\overline{h}_f$ là nửa liên tục dưới, các quan hệ trước đó cho đẳng thức $\mu^\bullet(\overline{h}_f) = \nu^\bullet(f)$ (§1, No. 1, Mệnh đề 4); vì $\overline{h}_f = h_f$ trên $S$, suy ra $\mu^\bullet(h_f) = \nu^\bullet(f)$ (§1, No. 1, Mệnh đề 1), một đẳng thức đồng nhất với (4). Ánh xạ $\Lambda$ do đó là $\mu$-tiền-thích hợp; nhưng trong toàn bộ lập luận này người ta có thể thay $\mu$ bởi $\mu' \leqslant \mu$, và $\nu$ bởi $\nu' = \int \lambda_t \, d\mu'(t)$, bởi vì $\Lambda$ cũng là khả tích $\mu'$-theo vô hướng một cách bản chất và $S$ chứa giá của $\mu'$. Từ đó suy ra rằng $\Lambda$ là $\mu$-thích hợp.

Giả sử $\Lambda$ là liên tục theo nghĩa mơ hồ; ta có thể lấy $S = T$; khi đó $h_f = \overline{h}_f$ là nửa liên tục dưới, điều này hoàn tất chứng minh phần a) của mệnh đề.

Giả sử rằng $\Lambda$ là $\mu$-đo được theo nghĩa mơ hồ và ta chứng minh b). Tập $\mathcal{K}$ gồm các tập con compact K của T sao cho hạn chế của $\Lambda$ trên K là liên tục là $\mu$-trù mật (Ch. IV, §5, No. 10, Mệnh đề 15), tồn tại một họ tổng được $(\mu_\alpha)_{\alpha \in A}$ các độ đo trên T sao cho $\mu = \sum_{\alpha \in A} \mu_\alpha$ và giá của mỗi độ đo $\mu_\alpha$ thuộc $\mathcal{K}$ (§2, No. 3, Mệnh đề 4). Với mọi $\alpha \in A$, ánh xạ $\Lambda$ là khả tích thiết yếu theo vô hướng $\mu_\alpha$, và ta đặt $\nu_\alpha = \int \lambda_t d\mu_\alpha(t)$; họ $(\nu_\alpha)$ là tổng được, và tổng của nó bằng $\nu$ (Hệ quả của Mệnh đề 1). Nếu $f$ là một hàm dương nửa liên tục dưới xác định trên X, phần thứ nhất của chứng minh, áp dụng cho các độ đo $\mu_\alpha$ và các tập đóng $S_\alpha$, chỉ ra rằng:

$1^\circ$ $h_f$ là $\mu_\alpha$-đo được với mọi $\alpha \in A$, do đó là $\mu$-đo được (§2, No. 2, Mệnh đề 2), và

$2^\circ$ $\int^* f(x) d\nu_\alpha(x) = \int^* d\mu_\alpha(t) \int^* f(x) d\lambda_t(x)$.

Công thức (4) suy ra bằng cách lấy tổng theo $\alpha$ (§2, No. 2, Mệnh đề 1). Áp dụng lập luận trước cho một độ đo tùy ý $\mu' \leq \mu$ (điều này là hợp lệ, vì $\Lambda$ là khả tích thiết yếu theo vô hướng $\mu'$ và $\mu'$-đo được theo nghĩa mơ hồ, cf. §2, No. 2, Mệnh đề 2), ta kết luận rằng $\Lambda$ là $\mu'$-tiền-thích đáng, và b) được chứng minh.

Cuối cùng, giả sử rằng tôpô của X có một cơ sở đếm được, ta chứng minh rằng mọi ánh xạ khả tích thiết yếu theo vô hướng $\mu$ $\Lambda : t \mapsto \lambda_t$ của T vào $\mathcal{M}_+(X)$ đều là $\mu$-đo được theo nghĩa mơ hồ. Điều này sẽ suy ra từ bổ đề sau:

#### Bổ đề {#int-v-s3-n1-lem-1 .statement}

*Cho X là một không gian compact địa phương có một cơ sở đếm được. Khi đó, tồn tại trong $\mathcal{K}(X)$ một tập con đếm được S có tính chất sau: với mọi hàm $f \in \mathcal{K}(X)$, tồn tại một dãy $(f_n)$ các phần tử của S và một hàm dương $\varphi \in S$ sao cho, với mọi số $\varepsilon > 0$, $|f_n - f| \leq \varepsilon \varphi$ với điều kiện n đủ lớn.*

Gọi $X'$ là compact hóa Alexandroff của X, là một không gian compact mêtric hóa được (GT, IX, §2, No. 9, Prop. 16 và Cor.); ta đồng nhất $\mathcal{K}(X)$ với một tập con của $\mathcal{C}(X')$. Gọi $S'$ là một tập con đếm được trù mật của không gian Banach $\mathcal{C}(X')$ (GT, X, §3, No. 3, Th. 1); ta có thể giả sử rằng $S'$ chứa hàm hằng $n$ với mọi $n \in \mathbf{N}$. Gọi $(U_n)$ là một dãy các tập mở tương đối compact trong X, có hợp là X, sao cho $\overline{U}_n \subset U_{n+1}$ với mọi n (GT, I, §9, No. 9, Prop. 15), và gọi $\varphi_n$ là một hàm trong $\mathcal{K}_+(X)$ bằng 1 trên $\overline{U}_n$. Ta ký hiệu S là tập hợp đếm được các phần tử của $\mathcal{K}(X)$ có dạng $\varphi_n g$ ($n \in \mathbf{N}, g \in S'$). Nếu $f \in \mathcal{K}(X)$, gọi $(g_n)$ là một dãy các phần tử của $S'$ hội tụ đều đến $f$, và gọi k là một số nguyên sao cho giá của $f$ được chứa trong $U_k$. Cuối cùng, gọi m là một số nguyên là cận trên của các chuẩn của các hàm $g_n$. Các hàm $f_n = \varphi_k g_n$ thuộc S và thỏa mãn mệnh đề, với $\varphi = m \varphi_k$.

Sau khi bổ đề đã được thiết lập, và ánh xạ $t \mapsto \lambda_t(g)$ là khả tích $\mu$-theo nghĩa thực chất đối với mọi $g \in S$, ánh xạ $t \mapsto (\lambda_t(g))_{g \in S}$ từ T vào $\mathbf{R}^S$ là $\mu$-đo được (Ch. IV, §5, No. 3, Th. 1). Tập hợp $\mathcal{K}$, gồm các tập compact K của T sao cho hạn chế của ánh xạ này lên K là liên tục, do đó là $\mu$-trù mật, và chỉ cần chứng minh rằng hạn chế của $\Lambda$ lên mọi $K \in \mathcal{K}$ là liên tục. Bây giờ, gọi $f$ là một phần tử bất kỳ của $\mathcal{K}(X)$, $f_n$ và $\varphi$ là các phần tử của S thỏa mãn mệnh đề của Bổ đề; khi đó hàm $t \mapsto \lambda_t(f)$ là giới hạn đều trên K của các hàm liên tục $t \mapsto \lambda_t(f_n)$; do đó nó liên tục trên K, và mệnh đề được chứng minh.

### 2. Các tích phân chồng của các hàm dương

Trong phần còn lại của tiết này, nếu không có chỉ rõ ngược lại, ta sẽ ký hiệu X là một không gian địa phương compact, $\Lambda : t \mapsto \lambda_t$ là một ánh xạ $\mu$-thích hợp từ T vào $\mathcal{M}_+(X)$, và $\nu$ là tích phân của $\Lambda$.

#### Mệnh đề 3 {#int-v-s3-prop-3 .statement}

— Gọi f là một hàm số $\geqslant 0$ xác định trên X.
a) Các bất đẳng thức sau đúng:

$$
\int^* f(x)\, d\nu(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

b) Nếu $\Lambda$ liên tục yếu, thì

$$
\int^* f(x)\, d\nu(x) \geqslant \int^* d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

c) Nếu $\lambda_t^\bullet(1) < +\infty$ địa phương $\mu$-hầu khắp nơi, thì

$$
\int^\bullet f(x)\, d\nu(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) = \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

Gọi g là một hàm nửa liên tục dưới trên X sao cho $f \leqslant g$. Với mọi $t \in T$,

$$
\int^* f(x)\, d\lambda_t(x) \leqslant \int^* g(x)\, d\lambda_t(x),
$$

do đó, theo (4) và Prop. 4 của §1,

$$
\int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) \leqslant \int^\bullet d\mu(t) \int^* g(x)\, d\lambda_t(x) = \int^* g(x)\, d\nu(x).
$$

Bất đẳng thức thứ nhất trong các bất đẳng thức (6) sau đó suy ra từ định nghĩa của $\int^* f(x)\, d\nu(x)$ (Ch. IV, §1, No. 3, Def. 3), và bất đẳng thức thứ hai suy ra ngay lập tức từ nó. Bất đẳng thức (7) được chứng minh theo cách tương tự nếu $\Lambda$ liên tục yếu, sử dụng (5) thay cho (4).

Ta chuyển sang chứng minh của (8). Ánh xạ $t \mapsto \lambda_t^*(1)$ là đo được, và hữu hạn địa phương $\mu$-hầu khắp nơi. Tập $\mathcal{K}$ các tập con compact của $T$ sao cho hạn chế của $t \mapsto \lambda_t^*(1)$ trên $K$ là hữu hạn và liên tục do đó là $\mu$-trù mật, và Mệnh đề 4 của §2, No. 3 suy ra sự tồn tại của một họ tổng được $(\mu_\alpha)_{\alpha \in A}$ các độ đo dương, với các giá đỡ thuộc $\mathcal{K}$, sao cho $\mu = \sum_{\alpha \in A} \mu_\alpha$. Ánh xạ $\Lambda$ là $\mu_\alpha$-thích hợp đối với mọi $\alpha \in A$; đặt $\nu_\alpha = \int \lambda_t d\mu_\alpha(t)$. Mệnh đề 1 chỉ ra rằng $\nu = \sum_{\alpha \in A} \nu_\alpha$, và quan hệ (4), áp dụng cho độ đo $\mu_\alpha$ và hàm 1, chỉ ra rằng $\nu_\alpha$ là một độ đo bị chặn (vì $\lambda_t^*(1)$ bị chặn trên $\operatorname{Supp}(\mu_\alpha)$). Khi đó ta viết công thức (6) cho độ đo $\mu_\alpha$, thay thế ký hiệu $\int^*$ trong vế thứ nhất bằng $\int^\bullet$, điều này hợp lệ theo Mệnh đề 7 của §1; khi đó

$$
\int^\bullet f(x) d\nu_\alpha(x) \geq \int^\bullet d\mu_\alpha(t) \int^* f(x) d\lambda_t(x) = \int^\bullet d\mu_\alpha(t) \int^\bullet f(x) d\lambda_t(x)
$$

(đẳng thức cuối cùng do sự kiện rằng $\lambda_t$ bị chặn hầu khắp nơi địa phương, và Mệnh đề 7 của § 1). Bất đẳng thức trong (8) khi đó thu được bằng cách lấy tổng theo $\alpha$ (§2, No. 2, Mệnh đề 1).

Nếu không đưa ra giả thiết tương tự như giả thiết của c), bất đẳng thức (8) có thể không đúng (Bài tập 2).

#### Hệ quả 1 {#int-v-s3-prop-3-cor-1 .statement}

— *Cho $f$ là một hàm $\geq 0$ xác định trên $X$, và cho $H$ là tập hợp các $t \in T$ sao cho $f$ không $\lambda_t$-bỏ qua được.*
a) *Nếu $f$ $\nu$-bỏ qua được, thì $H$ là địa phương $\mu$-bỏ qua được.*
b) *Nếu $f$ là $\nu$-bỏ qua được và $\Lambda$ liên tục theo nghĩa mơ hồ, thì $H$ là $\mu$-bỏ qua được.*
c) *Nếu $f$ là địa phương $\nu$-bỏ qua được và $\lambda_t^\bullet(1) < +\infty$ địa phương $\mu$-hầu khắp nơi, thì $H$ là địa phương $\mu$-bỏ qua được.*

#### Hệ quả 2 {#int-v-s3-prop-3-cor-2 .statement}

— *Cho $f$ là một hàm $\geq 0$ xác định trên $X$, $\nu$-đo được và $\nu$-điều hòa. Tập hợp các $t \in T$ sao cho $f$ không $\lambda_t$-điều hòa được khi đó là địa phương $\mu$-bỏ qua được (và thậm chí $\mu$-bỏ qua được nếu $\Lambda$ liên tục theo nghĩa mơ hồ).*

Vì, $f$ là tổng của một dãy các hàm $f_n \geq 0$ sao cho $f_n$ bằng không bên ngoài một tập compact $K_n$ với $n \geq 1$, và $f_0$ là $\nu$-không đáng kể (§1, No. 2, Mệnh đề 6); khi đó $f_0$ là $\lambda_t$-không đáng kể ngoại trừ các $t$ tạo thành một tập địa phương $\mu$-không đáng kể (và thậm chí $\mu$-không đáng kể, nếu $\Lambda$ liên tục mơ hồ) theo Hệ quả 1, và mệnh đề suy ra ngay lập tức.

#### Mệnh đề 4 {#int-v-s3-prop-4 .statement}

— *Cho $f$ là một hàm $\nu$-đo được xác định trên $X$, với các giá trị trong một không gian tôpô $G$, và cho $M$ là tập hợp các $t \in T$ sao cho $f$ không $\lambda_t$-đo được.*
a) *Giả sử rằng $f$ là hằng trên phần bù của một tập con $\nu$-điều hòa của $X$; khi đó $M$ là địa phương $\mu$-không đáng kể.*

b) *Giả sử rằng f là hằng trên phần bù của một tập con ν-điều hòa của X, và rằng Λ liên tục mơ hồ; khi đó M là μ-không đáng kể.*

c) *Giả sử rằng $\lambda_t^\bullet(1) < +\infty$ hầu khắp mọi nơi theo μ địa phương; khi đó M là địa phương μ-không đáng kể.*

Trước hết ta chứng minh a) (tương ứng b)). Vì mọi tập ν-tích phân đều được chứa trong một tập mở ν-tích phân, nên hàm f là hằng trên phần bù B của một hợp đếm được các tập mở ν-tích phân. Có một phân hoạch của X − B tạo bởi một tập ν-không đáng kể N và một dãy $(K_n)$ các tập compact sao cho hạn chế của f trên mỗi $K_n$ là liên tục. Gọi S là tập hợp các $t \in T$ sao cho N không là $\lambda_t$-không đáng kể: S là địa phương μ-không đáng kể (tương ứng μ-không đáng kể) theo Hệ quả 1 của Mệnh đề 3. Các tập $K_n, B, N$ là đo được đối với mọi độ đo trên X, và hạn chế của f trên mỗi tập trong chúng là $\lambda_t$-đo được đối với mọi $t \notin S$. Do đó hàm f là $\lambda_t$-đo được đối với mọi $t \notin S$ (Ch. IV, §5, No. 10, Mệnh đề 16).

Để thiết lập c), ta dùng lại các ký hiệu trong chứng minh của Mệnh đề 3; vì f là ν-đo được, nó đo được đối với mỗi độ đo $\nu_\alpha \leq \nu$. Bây giờ, các độ đo này bị chặn, do đó được điều hòa, và từ a) suy ra rằng M là địa phương $\mu_\alpha$-không đáng kể với mọi $\alpha \in A$. Điều này kéo theo rằng M là địa phương μ-không đáng kể (§2, No. 2, Hệ quả 2 của Mệnh đề 1).

#### Mệnh đề 5 {#int-v-s3-prop-5 .statement}

*Cho f là một hàm số dương ν-đo được xác định trên X, và cho N là tập hợp các $t \in T$ sao cho f không đồng thời $\lambda_t$-đo được và $\lambda_t$-điều hòa.*

a) *Giả sử rằng f là ν-điều hòa. Khi đó tập N là địa phương μ-không đáng kể, hàm $t \mapsto \int^\bullet f(x) d\lambda_t(x)$ là μ-đo được, và*

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

b) *Giả sử rằng f là ν-điều hòa, và rằng Λ liên tục mơ hồ. Khi đó tập N là μ-không đáng kể, hàm $t \mapsto \int^* f(x) d\lambda_t(x)$ là μ-đo được và μ-điều hòa, và*

$$
\int^* f(x) d\nu(x) = \int^* d\mu(t) \int^* f(x) d\lambda_t(x).
$$

c) *Giả sử rằng $\lambda_t^\bullet(1) < +\infty$ hầu khắp mọi nơi theo μ địa phương. Khi đó tập N là địa phương μ-không đáng kể, hàm $t \mapsto \int^\bullet f(x) d\lambda_t(x)$ là μ-đo được, và (9) đúng.*

Trước hết ta chứng minh a) (tương ứng b)), giả sử rằng f là ν-điều hòa. Các khẳng định liên quan đến tập N đã được thiết lập (Mệnh đề 4, và Hệ quả 2 của Mệnh đề 3). Theo Mệnh đề 6 của §1, No. 2, ta có thể tự giới hạn vào việc chứng minh a) (tương ứng b)) trong mỗi trường hợp đặc biệt sau:

1) Hàm $f$ là $\nu$-không đáng kể.
2) Tồn tại một tập compact $K$ sao cho $f$ bằng không bên ngoài $K$ và hạn chế của $f$ trên $K$ là liên tục.

Trường hợp đặc biệt 1) đã được xử lý rồi (Hệ quả 1 của Mệnh đề 3). Để xử lý trường hợp thứ hai, ta ký hiệu bởi $G$ một tập mở $\nu$-nguyên chứa $K$, bởi $M$ một cận trên hằng của $f$, bởi $h$ hàm nửa liên tục dưới $M \varphi_G$, và bởi $g$ hàm $h - f$. Vì hàm $f$ là nửa liên tục trên trên $X$, nên $g$ là nửa liên tục dưới và dương. Hơn nữa, $f, g, h$ là $\nu$-nguyên.

Khi đó ta áp dụng công thức (4) (tương ứng (5)) cho các hàm nửa liên tục dưới $h$ và $g$. Lấy hiệu, ta thấy rằng hàm

$$
t \mapsto \int^\bullet f(x)\, d\lambda_t(x) \quad (\text{resp. } \int^* f(x)\, d\lambda_t(x))
$$

là $\mu$-đo được và công thức (9) (tương ứng (10)) đúng. Cuối cùng, dưới giả thiết của b), hàm $t \mapsto \int^* f(x)\, d\lambda_t(x)$ có tích phân trên hữu hạn, do đó thực sự là $\mu$-bị chặn.

Để chứng minh c), ta xét lại các độ đo $\mu_\alpha$ và $\nu_\alpha$ của chứng minh Mệnh đề 3; vì $f$ là $\nu_\alpha$-đo được và $\nu_\alpha$-bị chặn, mệnh đề a) suy ra rằng $t \mapsto \int^\bullet f(x)\, d\lambda_t(x)$ là $\mu_\alpha$-đo được và

$$
\int^\bullet f(x)\, d\nu_\alpha(x) = \int^\bullet d\mu_\alpha(t) \int^\bullet f(x)\, d\lambda_t(x).
$$

Chỉ còn việc lấy tổng theo $\alpha$, áp dụng các Mệnh đề 1 và 2 của §2, No. 2.

Nếu $f$ không được giả thiết là $\nu$-bị chặn, và nếu không đặt giả thiết trong c), thì quan hệ (9) có thể không đúng (Bài tập 3).

#### Hệ quả {#int-v-s3-n2-cor-1 .statement}

— *Cho $\mathbf{f}$ là một hàm xác định trên $X$, nhận giá trị trong một không gian Banach $F$ hoặc trong $\overline{\mathbf{R}}$, là $\nu$-đo được và $\nu$-bị chặn. Để $\mathbf{f}$ là $\nu$-nguyên, điều kiện cần và đủ là*

$$
\int^\bullet d\mu(t) \int^\bullet |\mathbf{f}(x)|\, d\lambda_t(x) < +\infty.
$$

Điều này suy ra ngay từ Mệnh đề 5 và tiêu chuẩn về tính nguyên (Ch. IV, §5, No. 6, Định lý 5).

### 3. Các tích phân chồng lên nhau của các hàm có giá trị trong một không gian Banach

#### Định lý 1 {#int-v-s3-thm-1 .statement}

— Cho $f$ là một hàm nhận giá trị trong một không gian Banach $F$ hoặc trong $\overline{\mathbf{R}}$, và cho $H$ là tập hợp các $t \in T$ sao cho $f$ không $\lambda_t$-nguyên.

a) *Nếu $f$ là $\nu$-nguyên, thì $H$ là $\mu$-vô nghĩa địa phương, hàm $t \mapsto \int f(x)\, d\lambda_t(x)$ (được xác định với $t \notin H$) là $\mu$-nguyên theo nghĩa bản chất, và*

$$
\int f(x)\, d\nu(x) = \int d\mu(t) \int f(x)\, d\lambda_t(x).
$$

b) *Nếu $f$ là $\nu$-khả tích và $\Lambda$ là liên tục yếu, thì $H$ còn là $\mu$-không đáng kể và hàm $t \mapsto \int f(x)\, d\lambda_t(x)$ (được xác định với $t \notin H$) là $\mu$-khả tích.*

c) *Nếu $\lambda_t^*(1) < +\infty$ địa phương $\mu$-hầu khắp nơi, thì các kết luận của a) vẫn đúng đối với $f$ là một hàm $\nu$-khả tích thiết yếu.*

Trước hết ta sẽ thiết lập a) (tương ứng b)). Mệnh đề này đúng khi $f$ là một hàm số dương (Mệnh đề 5); nếu $f$ là một hàm khả tích nhận giá trị trong $\overline{\mathbf{R}}$, kết quả này có thể áp dụng cho các hàm dương $f^+$ và $f^-$, và do đó ngay lập tức mở rộng đến $f$ bằng phép trừ. Còn lại cần xét trường hợp các hàm nhận giá trị trong $F$. Gọi $\mathcal{H}$ là không gian con của $\mathcal{L}_F^1(\nu)$ tạo bởi các tổ hợp tuyến tính, với các hệ số trong $F$, của các hàm thuộc $\mathcal{K}(X)$; kết quả liên quan đến các hàm thực suy ra ngay tính đúng đắn của mệnh đề đối với các phần tử của $\mathcal{H}$. Bây giờ, $\mathcal{H}$ trù mật trong $\mathcal{L}_F^1(\nu)$; do đó, với mọi $f \in \mathcal{L}_F^1(\nu)$, tồn tại một dãy $(f_n)$ các phần tử của $\mathcal{H}$ có các tính chất sau:

1) dãy $(f_n)$ hội tụ đến $f$ theo trung bình trong $\mathcal{L}_F^1(\nu)$, và $\nu$-hầu khắp nơi;
2) hàm $g = |f_0| + \sum_{n \in \mathbf{N}} |f_{n+1} - f_n|$ sao cho $\nu^*(g) < +\infty$ (Ch. IV, §3, No. 4, Đl. 3).

Gọi $N_1$ là tập hợp các $t \in T$ sao cho $\lambda_t^*(g) = +\infty$; $N_1$ là địa phương $\mu$-không đáng kể (tương ứng $\mu$-không đáng kể) theo công thức (6) (tương ứng (7)). Với $t \notin N_1$, các $f_n$ thuộc $\mathcal{L}_F^1(\lambda_t)$, dãy $(f_n)$ hội tụ $\lambda_t$-hầu khắp nơi, cũng như đối với tôpô của sự hội tụ theo trung bình trong $\mathcal{L}_F^1(\lambda_t)$ (Ch. IV, §3, No. 3, Mệnh đề 6). Gọi $M$ là tập hợp các $x \in X$ sao cho $f_n(x)$ không hội tụ đến $f(x)$: vì $M$ là $\nu$-không đáng kể, tập hợp $N_2$ gồm các $t \in T$ sao cho $M$ không là $\lambda_t$-không đáng kể là địa phương $\mu$-không đáng kể (tương ứng $\mu$-không đáng kể) theo Hệ quả 1 của Mệnh đề 3.

Giả sử rằng $t$ không thuộc $N_1 \cup N_2$; dãy $(f_n)$ hội tụ theo trung bình trong $\mathcal{L}_F^1(\lambda_t)$, và hội tụ $\lambda_t$-hầu khắp nơi đến $f$. Do đó $f \in \mathcal{L}_F^1(\lambda_t)$ và $\int f\, d\lambda_t = \lim_{n \to \infty} \int f_n\, d\lambda_t$ (Ch. IV, §4, No. 1). Tập hợp $H$ của mệnh đề do đó được chứa trong $N_1 \cup N_2$; vì vậy nó là địa phương $\mu$-không đáng kể (tương ứng $\mu$-không đáng kể). Mặt khác, hàm $t \mapsto \int f\, d\lambda_t$ bằng địa phương $\mu$-hầu khắp nơi với giới hạn của một dãy các hàm $\mu$-đo được; do đó nó là $\mu$-đo được. Cuối cùng, với mọi $t \notin N_1 \cup N_2$ và mọi $n$, ta có
$$
\left| \int f_n(x)\, d\lambda_t(x) \right| \leq \int^* g(x)\, d\lambda_t(x)
$$
do bất đẳng thức $|f_n| \leq g$ và Mệnh đề 2 của Ch. IV, §4, No. 2. Khi đó, hàm $t \mapsto \int^* g(x)\, d\lambda_t(x)$ là khả tích $\mu$-cốt yếu (tương ứng $\mu$-khả tích) theo Mệnh đề 5. Vì vậy ta có thể áp dụng định lý Lebesgue, cho
$$
\int d\mu(t) \int f(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int d\mu(t) \int f_n(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int f_n(x)\, d\nu(x).
$$
Vì $\int f_n(x)\, d\nu(x)$ tiến tới $\int f(x)\, d\nu(x)$ khi $n$ tiến tới $\infty$, theo các giả thiết đặt ra trên dãy $(f_n)$, quan hệ (11) suy ra và ta đã chứng minh a) (tương ứng b)).

Bây giờ giả sử rằng $\lambda_t^\bullet(1) < +\infty$ địa phương $\mu$-hầu khắp nơi, và rằng $g$ là một hàm $\nu$-khả tích cốt yếu. Gọi $f$ là một hàm $\nu$-khả tích sao cho $g = f$ địa phương $\nu$-hầu khắp nơi (\S1, No. 3). Khi đó $g = f$ hầu khắp nơi đối với $\lambda_t$, trừ các $t$ tạo thành một tập hợp $\mu$-không đáng kể địa phương $P$ (Hệ quả 1 c) của Mệnh đề 3). Do đó $\int g\, d\lambda_t = \int f\, d\lambda_t$ với mọi $t \notin P \cup H$, và điều này hoàn tất chứng minh.

#### Nhận xét {#int-v-s3-n3-rem-1 .statement}

Cho $\Lambda : t \mapsto \lambda_t$ là một ánh xạ $\mu$-thích hợp của $T$ vào $\mathcal{M}_+(X)$. Nếu một ánh xạ $\Lambda' : t \mapsto \lambda'_t$ của $T$ vào $\mathcal{M}_+(X)$ bằng $\Lambda$ địa phương $\mu$-hầu khắp nơi, thì suy ra ngay từ các định nghĩa rằng $\Lambda'$ cũng là $\mu$-thích hợp, và rằng $\Lambda$ và $\Lambda'$ có cùng tích phân. Nếu bây giờ $H : t \mapsto \eta_t$ là một hàm nhận giá trị trong $\mathcal{M}_+(X)$, được xác định địa phương $\mu$-hầu khắp nơi, ta lại nói rằng $H$ là $\mu$-thích hợp nếu nó bằng địa phương $\mu$-hầu khắp nơi với một ánh xạ $\Lambda : t \mapsto \lambda_t$ xác định khắp nơi và $\mu$-thích hợp. Khi đó ta đặt $\int \eta_t\, d\mu(t) = \int \lambda_t\, d\mu(t)$, một định nghĩa không phụ thuộc vào hàm $\Lambda$ được sử dụng. Ta để cho người đọc kiểm chứng rằng các mệnh đề đã chứng minh trong các Số trước mở rộng được cho các hàm $\mu$-thích hợp được xác định địa phương $\mu$-hầu khắp nơi.

### 4. Các hàm đo được phổ quát

#### Định nghĩa 2 {#int-v-s3-def-2 .statement}

*Một ánh xạ f của T vào một không gian tôpô F được gọi là đo được phổ quát nếu nó là $\mu$-đo được đối với mọi độ đo dương $\mu$ trên T.*

Các tập con của T mà hàm đặc trưng của chúng là đo được phổ quát được gọi là các tập đo được phổ quát. Chúng tạo thành một σ-đại số trên T (Ch. IV, §5, No. 4, Hệ quả 2 của Định lý 2) chứa các tập Borel (cùng tham chiếu, Hệ quả 3), và các tập Souslin nếu T là mêtric hóa được (Ch. IV, §5, No. 1, Hệ quả 2 của Mệnh đề 3). Để một ánh xạ $f$ của T vào một không gian tôpô F, mêtric hóa được và tách được, là đo được phổ quát, điều kiện cần và đủ là ảnh ngược qua $f$ của mọi quả cầu đóng trong F là một tập con đo được phổ quát của T (Ch. IV, §5, No. 5, Định lý 4).

#### Mệnh đề 6 {#int-v-s3-prop-6 .statement}

*Một ánh xạ $f$ của T vào một không gian tôpô F là đo được phổ quát khi và chỉ khi $f$ là đo được đối với mọi độ đo dương trên T có giá compact.*

Điều kiện này hiển nhiên là cần; mặt khác nó là đủ, vì mọi độ đo dương $\mu$ là tổng của một họ các độ đo có giá compact (§2, No. 3, Mệnh đề 4): mệnh đề khi đó suy ra từ Mệnh đề 2 của §2, No. 2.

#### Mệnh đề 7 {#int-v-s3-prop-7 .statement}

*Cho $\mu$ là một độ đo dương trên T, và cho $f$ là một ánh xạ $\mu$-đo được của T vào một không gian tôpô F. Khi đó tồn tại một ánh xạ đo được phổ quát $f'$ của T vào F sao cho $f = f'$ địa phương $\mu$-hầu khắp nơi.*

Gọi $\mathcal{K}$ là tập hợp các tập compact trong T sao cho hạn chế của $f$ lên K là liên tục; vì $\mathcal{K}$ là $\mu$-trù mật (Ch. IV, §5, No. 10, Mệnh đề 15), tồn tại một họ đếm được địa phương $(K_i)_{i \in I}$ gồm các phần tử rời nhau từng đôi một của $\mathcal{K}$ sao cho tập $N = T - \bigcup_{i \in I} K_i$ là không đáng kể địa phương $\mu$ (Ch. IV, §5, No. 9, Mệnh đề 14). Cho $x$ là một phần tử của F; đặt

$$
f'(t) = f(t) \quad \text{nếu } t \in \bigcup_{i \in I} K_i,
$$
$$
f'(t) = x \quad \text{nếu } t \in N.
$$

Các hàm $f$ và $f'$ bằng nhau địa phương $\mu$-hầu khắp nơi. Mặt khác, $N \cap K$ là một tập con Borel của K đối với mọi tập compact K trong T, vì họ $(K_i)$ là đếm được địa phương. Suy ra rằng N là một tập đo được phổ quát, và rằng $f'$ là một hàm đo được phổ quát (Ch. IV, §5, No. 10, Mệnh đề 16).

### 5. Các khuếch tán

#### Định nghĩa 3 {#int-v-s3-def-3 .statement}

*Cho X là một không gian compact địa phương, và cho $\Lambda : t \mapsto \lambda_t$ là một ánh xạ của T vào $\mathcal{M}_+(X)$. Ánh xạ $\Lambda$ được gọi là một khuếch tán* của T trong X nếu Λ là thích hợp đối với mọi độ đo dương trên T có giá compact. Khuếch tán Λ được gọi là bị chặn nếu tất cả các độ đo λ_t là bị chặn và $\sup_{t \in T} \| \lambda_t \| < +\infty$; đại lượng này khi đó được gọi là chuẩn của Λ và được ký hiệu $\| \Lambda \|$.

Mệnh đề sau đây chỉ đơn giản là dịch lại định nghĩa:

#### Mệnh đề 8 {#int-v-s3-prop-8 .statement}

— Để một ánh xạ $\Lambda : t \mapsto \lambda_t$ của T vào $\mathcal{M}_+(X)$ là một phép khuếch tán, điều kiện cần và đủ là các điều kiện sau được thỏa mãn:
1) Với mọi hàm nửa liên tục dưới $f \geqslant 0$ xác định trên X, hàm $t \mapsto \lambda_t^\bullet(f)$ là khả đo được phổ dụng trên T.
2) Với mọi hàm $g \in \mathcal{K}_+(X)$, hàm $t \mapsto \lambda_t(g)$ bị chặn địa phương trên T.
3) Với mọi hàm nửa liên tục dưới $f \geqslant 0$ xác định trên X và với mọi độ đo dương $\mu$ trên T có giá compact, đẳng thức sau đúng, trong đó $\nu$ ký hiệu $\int \lambda_t d\mu(t)$:

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

Giả sử rằng $\Lambda$ là một phép khuếch tán. Khi đó điều kiện 1) được thỏa mãn theo định nghĩa các ánh xạ thích đáng (No. 1, Định nghĩa 1) và Mệnh đề 6; điều kiện 3) được thỏa mãn bởi công thức (4), vì $\Lambda$ là $\mu$-thích đáng. Cho $g \in \mathcal{K}_+(X)$ và cho $u$ là hàm $t \mapsto \lambda_t(g)$ (khả đo được phổ dụng, theo 1)); giả sử rằng $u$ không bị chặn địa phương. Khi đó sẽ tồn tại một tập compact K sao cho $u$ không bị chặn trên K, do đó sẽ tồn tại một dãy $(t_n)$ gồm các phần tử của K sao cho $u(t_n) \geqslant n^2$ với mọi $n \geqslant 1$; khi đó $u$ không khả tích đối với độ đo $\mu = \sum_{n \geqslant 1} \frac{1}{n^2} \varepsilon_{t_n}$ có giá compact, trái với giả thiết về $\Lambda$, giả thiết này suy ra rằng $t \mapsto \lambda_t(g)$ khả tích đối với mọi độ đo dương có giá compact. Vậy ba điều kiện trên là cần thiết. Ngược lại, các điều kiện 1) và 2) suy ra rằng $\Lambda$ khả tích thiết yếu theo vô hướng đối với $\mu$ với mọi độ đo $\mu$ có giá compact. Vì mọi độ đo $\mu' \geq 0$ bị chặn trên bởi một độ đo $\mu$ có giá compact thì cũng có giá compact, các điều kiện 1) và 3) diễn đạt rằng $\Lambda$ là $\mu$-thích đáng đối với mọi độ đo dương có giá compact, và đó chính là kết quả cần tìm.

#### Mệnh đề 9 {#int-v-s3-prop-9 .statement}

— Cho $\Lambda : t \mapsto \lambda_t$ là một ánh xạ từ T vào $\mathcal{M}_+(X)$, sao cho hàm $t \mapsto \lambda_t(g)$ là khả đo được phổ dụng và bị chặn địa phương trên T với mọi $g \in \mathcal{K}_+(X)$. Có thể khẳng định rằng $\Lambda$ là một phép khuếch tán trong mỗi trường hợp sau:

a) *tôpô của X có một cơ sở đếm được*;
b) *Λ khả đo được phổ dụng đối với tôpô mơ hồ*.

Thật vậy, cho $μ$ là một độ đo dương trên T có giá compact; ánh xạ $Λ$ khả tích thiết yếu theo vô hướng đối với $μ$, do đó $μ$-thích đáng nếu hoặc a) hoặc b) được thỏa mãn (No. 1, Mệnh đề 2).

Đối với phần còn lại của tiết này, ta sẽ dùng các ký hiệu sau: ta sẽ ký hiệu bởi $⟨η, h⟩$ tích phân thiết yếu trên, đối với một độ đo dương $η$, của một hàm dương khả đo được theo $η$ là $h$. Ánh xạ $Λ : t ↦ λ_t$ sẽ là một phép khuếch tán của $T$ trong $X$. Nếu $f$ là một hàm dương khả đo được phổ dụng xác định trên $X$, ta sẽ ký hiệu bởi $Λf$ ánh xạ $t ↦ λ_t^*(f)$. Nếu $μ$ là một độ đo dương trên $T$ sao cho $Λ$ khả tích thiết yếu theo vô hướng đối với $μ$, ta sẽ ký hiệu bởi $μΛ$ độ đo $∫ λ_t dμ(t)$. Định nghĩa của tích phân khi đó có dạng

$$
⟨μΛ, f⟩ = ⟨μ, Λf⟩ \quad \text{với } f ∈ \mathcal{K}_+(X).
$$

Ta sẽ nói rằng một độ đo dương $μ$ trên $T$ *thuộc miền của $Λ$* nếu $Λ$ là $μ$-thích hợp: điều đó có nghĩa là nói (theo Mệnh đề 8) rằng $Λ$ là khả tích cốt yếu theo vô hướng đối với $μ$ và $⟨μ'Λ, f⟩ = ⟨μ', Λf⟩$ với mọi độ đo dương $μ' ≤ μ$ và mọi hàm dương nửa liên tục dưới $f$.

#### Mệnh đề 10 {#int-v-s3-prop-10 .statement}

*Hãy cho $f, g$ là hai hàm dương đo được theo mọi độ đo trên $X$, cho $a$ là một số $≥ 0$, và cho $μ$ và $ν$ là hai độ đo dương trên $T$. Khi đó:*

a) $Λ(f + g) = Λf + Λg$, $Λ(af) = aΛf$.
b) *Nếu $μ$ và $ν$ thuộc miền của $Λ$, thì $μ + ν$ và $aμ$ cũng thuộc miền đó, và ta có* $(μ + ν)Λ = μΛ + νΛ$, $(aμ)Λ = a(μΛ)$.

Điểm duy nhất không hiển nhiên là $μ + ν$ thuộc miền của $Λ$, và điều này được xét bằng cách nhận thấy rằng mọi độ đo dương bị chặn trên bởi $μ + ν$ đều có dạng $μ' + ν'$, trong đó $μ' ≤ μ$, $ν' ≤ ν$ (''bổ đề phân tích'', Ch. II, §1, No. 1). Xem thêm mệnh đề sau.

#### Mệnh đề 11 {#int-v-s3-prop-11 .statement}

*Để một độ đo dương $μ$ trên $T$ thuộc miền của $Λ$, điều kiện cần và đủ là $Λ$ khả tích cốt yếu theo vô hướng đối với $μ$. \*

Điều kiện này hiển nhiên là cần thiết. Ngược lại, giả sử điều đó đúng, và cho $f$ là một hàm dương nửa liên tục dưới xác định trên $X$. Hàm $Λf$ là đo được theo mọi độ đo, do đó $μ$-đo được. Ta sẽ chứng minh rằng $⟨μ, Λf⟩ = ⟨μΛ, f⟩$; vì đẳng thức này cũng đúng với mọi độ đo dương $μ' ≤ μ$, do $Λ$ cũng khả tích cốt yếu theo vô hướng đối với $μ'$, nên suy ra rằng $Λ$ là $μ$-thích hợp.

Cho $(\mu_i)_{i∈I}$ là một họ khả tổng các độ đo dương có giá compact, sao cho $μ = ∑_{i∈I} μ_i$ (§2, No. 3, Mệnh đề 4); khi đó họ các độ đo $\mu_i \Lambda$ cũng khả tổng, và $\mu \Lambda = \sum_{i \in I} \mu_i \Lambda$ (No. 1, Hệ quả của Mệnh đề 1). Do đó $\langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle$ (\S 2, No. 2, Mệnh đề 1); nhưng $\Lambda$ là $\mu_i$-thích hợp, nên $\langle \mu_i \Lambda, f \rangle = \langle \mu_i, \Lambda f \rangle$. Áp dụng lại Mệnh đề 1 của \S 2, ta được đẳng thức cần tìm:

$$
\langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i, \Lambda f \rangle = \langle \mu, \Lambda f \rangle .
$$

#### Hệ quả 1 {#int-v-s3-prop-11-cor-1 .statement}

— *Nếu $\Lambda$ là một diffusion bị chặn, thì mọi độ đo dương bị chặn $\mu$ đều thuộc miền xác định của $\Lambda$, và $\| \mu \Lambda \| \leq \| \mu \| \| \Lambda \|$.*

#### Hệ quả 2 {#int-v-s3-prop-11-cor-2 .statement}

— *Giả sử $\mu$ là tổng của một họ khả tổng $(\mu_\alpha)_{\alpha \in A}$ gồm các độ đo dương thuộc miền xác định của $\Lambda$. Để $\mu$ thuộc miền xác định của $\Lambda$, điều kiện cần và đủ là họ các độ đo $\mu_\alpha \Lambda$ khả tổng; trong trường hợp đó $\mu \Lambda = \sum_{\alpha \in A} \mu_\alpha \Lambda$.*

Chỉ cần áp dụng Hệ quả của Mệnh đề 1 của No. 1.

Mệnh đề 5, được diễn đạt bằng ngôn ngữ của các diffusion, có dạng sau:

#### Mệnh đề 12 {#int-v-s3-prop-12 .statement}

— *Cho $\mu$ là một độ đo dương trên $T$ thuộc miền xác định của $\Lambda$, và cho $f$ là một hàm khả đo lường theo mọi nghĩa $\geq 0$ được xác định trên $X$. Nếu $f$ là moderated đối với độ đo $\mu \Lambda$, hoặc nếu các độ đo $\lambda_t$ bị chặn, thì hàm $\Lambda f$ là $\mu$-khả đo và*

$$
\langle \mu \Lambda, f \rangle = \langle \mu, \Lambda f \rangle .
$$

#### Hệ quả {#int-v-s3-n5-cor-1 .statement}

— *Nếu $X$ là đếm được ở vô cực, hoặc nếu các độ đo $\lambda_t$ bị chặn, thì hàm $\Lambda f$ là khả đo lường theo mọi nghĩa trên $T$ với mọi hàm khả đo lường theo mọi nghĩa $f \geq 0$ được xác định trên $X$, và (13) đúng.*

### 6. Hợp thành các diffusion bị chặn

#### Mệnh đề 13 {#int-v-s3-prop-13 .statement}

— *Cho $T, X, Y$ là ba không gian compact địa phương, $\Lambda : t \mapsto \lambda_t$ một diffusion bị chặn của $T$ trong $X$, và $H : x \mapsto \eta_x$ một diffusion bị chặn của $X$ trong $Y$. Khi đó ánh xạ $t \mapsto \lambda_t H$ là một diffusion bị chặn của $T$ trong $Y$, được ký hiệu bởi $\Lambda H$, và*

$$
\| \Lambda H \| \leq \| \Lambda \| \| H \|.
$$

*Cho $f$ là một hàm khả đo lường theo mọi nghĩa $\geq 0$ được xác định trên $Y$, và $\mu$ là một độ đo trên $T$. Giả sử rằng $\mu$ thuộc miền xác định của $\Lambda$, và rằng* μΛ *thuộc miền xác định của $H$; khi đó $\mu$ thuộc miền xác định của $\Lambda H$, và*

$$
\langle \mu(\Lambda H), f \rangle = \langle \mu \Lambda, Hf \rangle = \langle \mu, \Lambda Hf \rangle;
$$
(15)
$$
(\mu \Lambda)H = \mu(\Lambda H); \quad \Lambda(Hf) = (\Lambda H)f.
$$

Đặt $\gamma_t = \lambda_t H$; ta sẽ ký hiệu bằng $\Gamma$ ánh xạ $\Lambda H$ của T vào $\mathcal{M}_+(Y)$, và bằng $\Gamma f$ hàm $t \mapsto \langle \gamma_t, f \rangle$ (lạm dụng ký hiệu, vì ta vẫn chưa biết liệu $\Gamma$ có phải là một khuếch tán hay không). Khi đó $\langle \gamma_t, f \rangle = \langle \lambda_t H, f \rangle = \langle \lambda_t, Hf \rangle$ theo (13); vì hàm $Hf$ là dương và đo được phổ quát trên X (Hệ quả của Mệnh đề 12), suy ra trước hết rằng $\Gamma f = \Lambda(Hf)$, và rồi $\Gamma f$ là đo được phổ quát trên T (tham chiếu như trên). Rõ ràng mọi độ đo $\gamma_t$ đều có tổng khối lượng nhiều nhất bằng $\| \Lambda \| \| H \|$. Do đó $\Gamma g$ là đo được phổ quát và bị chặn với mọi hàm $g \in \mathcal{K}_+(Y)$; vì thế $\Gamma$ khả tích thiết yếu theo vô hướng đối với mọi độ đo bị chặn trên T, và đặc biệt là đối với mọi độ đo có giá compact. Tổng quát hơn, nếu $\mu$ là một độ đo thuộc miền xác định của $\Lambda$, sao cho $\mu \Lambda$ thuộc miền xác định của H, thì, với $g \in \mathcal{K}_+(Y)$,

$$
\langle \mu, \Gamma g \rangle = \langle \mu, \Lambda(Hg) \rangle = \langle \mu \Lambda, Hg \rangle = \langle (\mu \Lambda)H, g \rangle.
$$

Vì đại lượng cuối cùng là hữu hạn, ta thấy rằng $\Gamma$ khả tích thiết yếu theo $\mu$ theo vô hướng. Ta ký hiệu $\mu \Gamma$ là tích phân $\int \gamma_t d\mu(t)$ (lạm dụng ký hiệu, vì ta vẫn chưa biết liệu $\Gamma$ có phải là một khuếch tán hay không). Khi đó các quan hệ trên có thể viết

$$
\langle \mu \Gamma, g \rangle = \langle (\mu \Lambda)H, g \rangle,
$$

hoặc cũng có thể là $\mu \Gamma = (\mu \Lambda)H$ vì $g$ tùy ý trong $\mathcal{K}_+(Y)$.

Xét lại hàm đo được phổ quát $f \geqslant 0$. Ta có

$$
\langle \mu \Gamma, f \rangle = \langle (\mu \Lambda)H, f \rangle = \langle \mu \Lambda, Hf \rangle = \langle \mu, \Lambda(Hf) \rangle = \langle \mu, \Gamma f \rangle.
$$

Khi $f$ là nửa liên tục dưới và $\mu$ chạy trên tập các độ đo dương có giá compact, các quan hệ này diễn tả rằng $\Gamma$ là một khuếch tán của T trong Y. Mệnh đề khi đó chỉ làm rõ các quan hệ thu được trong quá trình chứng minh trên.

#### Định nghĩa 4 {#int-v-s3-def-4 .statement}

*Với các ký hiệu như ở Mệnh đề 13, khuếch tán $\Lambda H$ được gọi là khuếch tán hợp thành (hay phép hợp thành) của các khuếch tán bị chặn H và $\Lambda$. \*

Cho $X_1, X_2, X_3, X_4$ là bốn không gian địa phương compact, và $\Lambda_1, \Lambda_2, \Lambda_3$ là ba khuếch tán bị chặn, lần lượt từ $X_1$ sang $X_2$, từ $X_2$ sang $X_3$, từ $X_3$ sang $X_4$. Suy ra ngay từ Mệnh đề 13 rằng

$$
(\Lambda_1 \Lambda_2) \Lambda_3 = \Lambda_1 (\Lambda_2 \Lambda_3).
$$

Vì vậy ta sẽ dùng các ký hiệu này không có ngoặc cho phép hợp thành các khuếch tán.

#### Ví dụ {#int-v-s3-n6-exa-1 .statement}

Cho $u$ là một ánh xạ đo được phổ quát của T vào X, và $v$ là một ánh xạ đo được phổ quát của X vào Y; theo Mệnh đề 2 b), ta định nghĩa các khuếch tán $\Lambda$ và $H$ bởi các công thức

$$
\lambda_t = \varepsilon_{u(t)}, \quad \eta_x = \varepsilon_{v(x)};
$$

khi đó khuếch tán $\Gamma = \Lambda H$ được cho bởi

$$
\gamma_t = \varepsilon_{(vou)(t)}.
$$

Vì thế cần lưu ý rằng thứ tự hợp thành của các khuếch tán là ngược với thứ tự thông thường của hợp thành các hàm.

### Bài tập {#int-v-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).
