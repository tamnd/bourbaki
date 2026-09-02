---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 2
section_title: Operations on measures
lang: vi
source: int-vii-ix
book_pages: INT IX.22-INT IX.41, INT IX.108
pdf_pages: 0204-0223, 0290-0290
extraction: ocr
subsections:
    - "no": 1
      title: Induced measure on a measurable subspace
      page: 22
      pdf_page: 204
    - "no": 2
      title: Measures defined by numerical densities
      page: 24
      pdf_page: 206
    - "no": 3
      title: Image of a measure
      page: 26
      pdf_page: 208
    - "no": 4
      title: Lifting of measures
      page: 29
      pdf_page: 211
    - "no": 5
      title: Product of two measures
      page: 31
      pdf_page: 213
    - "no": 6
      title: Integration with respect to the product of two measures
      page: 33
      pdf_page: 215
    - "no": 7
      title: A result on the disintegration of measures
      page: 37
      pdf_page: 219
statements: 38
exercises: 3
content_sha256: 02abd689324a5ce6efd4c482bc97777f183d92ec58a35284e29dd8a916ed5323
translated_from: content/en/int/IX/02_s2_operations_on_measures.md
source_content_sha256: 5d3aed35c21d37dd0891ce27752ff8c2c681733ce8a642742891a5f7895e1d07
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4-mini
translation_run: translate-vi-59d57011
glossary_version: 34
glossary_terms_sha256: 80d7c48c3adfa2f507cd2939a7eb58a954a36214c2f15886e9aeec1b44c12623
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC PHÉP TOÁN TRÊN CÁC ĐỘ ĐO

Như trong mục trước, $T$ ký hiệu một không gian tôpô Hausdorff, và $\mu$ một độ đo trên $T$. Nhắc lại rằng mọi độ đo được giả thiết là dương, nếu không có nói khác.

### 1. Độ đo cảm sinh trên một không gian con đo được

Cho $X$ là một tập con của $T$, và cho $\nu$ là hạn chế của ánh xạ $\mu : K \mapsto \mu_K$ lên tập hợp các tập con compact của $X$; rõ ràng rằng $\nu$ là một tiền độ đo trên $X$. Mặt khác, cho $x \in X$ và cho $V$ là một lân cận mở của $x$ trong $T$ sao cho $\mu^\bullet(V) < +\infty$; khi đó

$$
\nu^\bullet(X \cap V) = \sup_{\substack{K \text{ compact} \\ K \subset X \cap V}} \mu^\bullet(K) \leq \mu^\bullet(V) < +\infty
$$

theo *Nhận xét 3* của §1, No. 2, do đó $\nu$ là một độ đo.

Khi $X$ không $\mu$-đo được, các bao hàm $\nu^\bullet$ và $(\mu^\bullet)_X$ không nhất thiết bằng nhau và độ đo $\nu$ không có lợi ích gì.

#### Định nghĩa 1 {#int-ix-s2-def-1 .statement}

*Cho $X$ là một tập con $\mu$-đo được của $T$. Hạn chế của $\mu : K \mapsto \mu_K$ lên tập hợp các tập con compact của $X$ được gọi là độ đo cảm sinh bởi $\mu$ trên không gian con $X$, và được ký hiệu bởi $\mu_X$ hoặc $\mu|X$.*

#### Mệnh đề 1 {#int-ix-s2-prop-1 .statement}

*Cho $X$ là một tập con $\mu$-đo được của $T$. Bao hàm $(\mu_X)^\bullet$ bằng với bao hàm $(\mu^\bullet)_X$ cảm sinh bởi $\mu^\bullet$ trên $X$ (§1, No. 1). Nói cách khác, $(\mu_X)^\bullet(g) = \mu^\bullet(g^0)$ với mọi hàm $g \in \mathcal{F}_+(X)$.*

Cho $f \in \mathcal{F}_+(X)$ và gọi $f^0$ là mở rộng bằng 0 của $f$ lên $T$. Ta có $(\mu^\bullet)_X(f) = \mu^\bullet(f^0) = \sup_L \mu^\bullet(f^0 \varphi_L)$, trong đó $L$ chạy trên tập hợp các tập con compact của $T$ (§1, No. 2, Prop. 2); tương tự $(\mu_X)^\bullet(f) = \sup_K \mu_K^\bullet(f_K) = \sup_K \mu^\bullet(f^0 \varphi_K)$, trong đó $K$ chạy trên tập hợp các tập con compact của $X$. Do đó tất cả quy về việc chỉ ra rằng $\mu^\bullet(f^0 \varphi_L) = \sup_K \mu^\bullet(f^0 \varphi_K)$ đối với mọi tập con compact $L$ của $T$, trong đó $K$ chạy trên tập hợp các tập con compact của $L \cap X$. Bây giờ, cho $(K_n)$ là một dãy tăng các tập compact được chứa trong $L \cap X$, sao cho $(L \cap X) - \bigcup_n K_n$ là địa phương $\mu$-không đáng kể (§1, No. 8, Prop. 11); vì $f^0$ bằng không bên ngoài $X$, $f^0 \varphi_L$ bằng không bên ngoài $L \cap X$, do đó bằng địa phương hầu khắp nơi với bao trên của dãy $(f^0 \varphi_{K_n})$. Điều này suy ra rằng $\mu^\bullet(f^0 \varphi_L) = \sup_n \mu^\bullet(f^0 \varphi_{K_n})$, do đó có kết quả mong muốn.*

#### Nhận xét 1 {#int-ix-s2-n1-rem-1 .statement}

Quan hệ $(\mu_X)^\bullet = (\mu^\bullet)_X$ cho phép sử dụng ký hiệu $\mu_X^\bullet$ mà không có sự nhập nhằng; từ nay về sau ta sẽ làm như vậy. Prop. 1 và Prop. 2 trước đó của §1, No. 2 chỉ ra rằng các độ đo được ký hiệu $\mu_K$ cho đến nay, với $K$ compact, thực sự là các độ đo cảm sinh theo nghĩa của Định nghĩa 1. Tương tự, nếu $T$ là compact địa phương, và nếu $X$ là một không gian con compact địa phương của $T$, Prop. 1 ở trên và Prop. 1 của Ch. V, §7, No. 1 chỉ ra rằng Định nghĩa 1 trùng với định nghĩa của Ch. IV, §5, No. 7.

#### Nhận xét 2 {#int-ix-s2-n1-rem-2 .statement}

Định nghĩa 1 có thể được mở rộng đến trường hợp $\mu$ là một độ đo phức trên $T$. Để chỉ ra trong trường hợp này rằng tiền độ đo $\mu_X$ là một độ đo, chỉ cần nhận xét rằng $|\mu_K| = |\mu|_K$ đối với mọi tập con compact $K$ của $X$ (§1, No. 2).

Theo Prop. 1, một tập con $Y$ của $X$ là $\mu_X$-đo được (tương ứng. địa phương $\mu_X$-không đáng kể) khi và chỉ khi nó là $\mu$-đo được (tương ứng. địa phương $\mu$-không đáng kể). Nếu $Y$ là $\mu_X$-đo được, do đó là $\mu$-đo được, thì các độ đo cảm sinh $(\mu_X)_Y$ và $\mu_Y$ hiển nhiên bằng nhau nhờ Prop. 1 (*tính bắc cầu của các độ đo cảm sinh*).

Nhận xét 3). — Cho X là một tập con $\mu$-đo được của T. Theo Mệnh đề 10 của §1, No. 8, áp dụng cho $g = \varphi_X$, tồn tại một phân hoạch nghiền $(K_\alpha)_{\alpha \in A}$ của T sao cho với mỗi $\alpha \in A$, hoặc là $K_\alpha \subset X$ hoặc là $K_\alpha \subset \mathbf{C}X$. Nếu sửa đổi tôpô của T bằng thủ tục của Chú giải của §1, No. 8, không gian $X'$ thu được bằng cách trang bị cho X tôpô cảm sinh bởi $T'$ là compact địa phương, và người ta biết cách liên kết với $\mu$ (tương ứng với $\mu_X$) một độ đo $\mu'$ (tương ứng với $\nu$) trên $T'$ (tương ứng trên $X'$) nhận cùng nguyên trên cốt yếu trên như $\mu$ (tương ứng với $\mu_X$): điều này kéo theo rằng $\mu'_{X'} = \nu$. Vì các tập hợp không đáng kể địa phương, các ánh xạ đo được, và các hàm khả tích cốt yếu có giá trị trong một không gian Banach, là như nhau đối với $\mu$ và $\mu'$, và đối với $\mu_X$ và $(\mu_X)' = \nu = \mu'_{X'}$, lý thuyết lấy tích phân đối với một độ đo cảm sinh quy về trường hợp đã được xét trong Ch. V, §7 trong trường hợp đặc biệt của các không gian compact địa phương. Ta để lại cho người đọc việc chuyển các kết quả này.

### 2. Các độ đo được xác định bởi các mật độ số

#### Định nghĩa 2 {#int-ix-s2-def-2 .statement}

*Một hàm f xác định trên T, có giá trị trong $\overline{\mathbf{R}}$ hoặc trong một không gian Banach, được gọi là khả tích $\mu$ địa phương nếu f là $\mu$-đo được và mọi điểm $x \in T$ đều có một lân cận V sao cho $\mu^\bullet(|f|\varphi_V) < +\infty$.*

Định nghĩa này trùng với định nghĩa đã cho trong Ch. V, §5, No. 1, trong trường hợp T là compact địa phương.

Cho $f$ là một hàm dương khả tích $\mu$ địa phương; ánh xạ $K \mapsto f_K \cdot \mu_K$ là một độ đo tiền (Ch. V, §7, No. 1, Hệ quả 2 của Định lý 1), sẽ được ký hiệu là $f \cdot \mu$.

#### Mệnh đề 2 {#int-ix-s2-prop-2 .statement}

*Nếu f là một hàm dương khả tích $\mu$ địa phương, thì, với mọi hàm $g \in \mathcal{F}_+(T)$, ta có quan hệ*

$$
(f \cdot \mu)^\bullet(g) = \mu^\bullet(fg).
$$

Thật vậy, với mọi tập compact K trong T,

$$
(f \cdot \mu)_K^\bullet(g_K) = (f_K \cdot \mu_K)^\bullet(g_K) = \mu_K^\bullet(f_K g_K) = \mu_K^\bullet((fg)_K),
$$

bằng cách sử dụng định nghĩa của $f \cdot \mu$ và Mệnh đề 3 của Ch. V, §5, No. 3. Mệnh đề 2 suy ra từ điều này bằng cách chuyển qua giá trị lớn nhất trên K.

Bây giờ cho $x \in T$ và cho V là một lân cận của x sao cho $\mu^\bullet(f \varphi_V) < +\infty$ (Định nghĩa 2); khi đó $(f \cdot \mu)^\bullet(V) = \mu^\bullet(f \varphi_V) < +\infty$, do đó $f \cdot \mu$ là một độ đo.

#### Định nghĩa 3 {#int-ix-s2-def-3 .statement}

*Cho f là một hàm dương khả tích $\mu$ địa phương. Độ đo $f \cdot \mu : K \mapsto f_K \cdot \mu_K$ được gọi là độ đo với mật độ f đối với* $\mu$, hoặc là độ đo tích của $\mu$ bởi hàm $f$. Mọi độ đo có dạng $f \cdot \mu$, trong đó $f$ là dương và khả tích $\mu$ địa phương, được gọi là một độ đo có cơ sở $\mu$.

#### Nhận xét 1 {#int-ix-s2-n2-rem-1 .statement}

Định nghĩa của $f \cdot \mu$ mở rộng sang trường hợp f là một hàm phức khả tích địa phương; khi đó ta có $|f \cdot \mu| = |f| \cdot \mu$, điều này kéo theo ngay rằng $f \cdot \mu$ là một độ đo, không chỉ là một độ đo tiền. Ta giữ lại biểu thức 'các độ đo có cơ sở $\mu$' để chỉ các độ đo phức được định nghĩa như vậy.

#### Nhận xét 2 {#int-ix-s2-n2-rem-2 .statement}

Tương tự, nếu $\theta$ là một độ đo phức, f được gọi là khả tích $\theta$ địa phương nếu nó khả tích $|\theta|$ địa phương, và người ta định nghĩa độ đo $f \cdot \theta : K \mapsto f_K \cdot \theta_K$. Ta có $|f \cdot \theta| = |f| \cdot |\theta|$ (Ch. V, §5, No. 2, Mệnh đề 2). Trong No. này, ta sẽ bỏ qua mọi điều liên quan đến các độ đo không dương.

#### Mệnh đề 3 {#int-ix-s2-prop-3 .statement}

— Cho $\nu$ là một độ đo trên T. Để $\nu$ có dạng $f \cdot \mu$, trong đó $f$ là một hàm dương khả tích địa phương theo $\mu$, thì điều kiện cần và đủ là mọi tập compact không đáng kể theo $\mu$ đều không đáng kể theo $\nu$. Nếu $f'$ là một hàm khả tích địa phương theo $\mu$ thứ hai sao cho $\nu = f' \cdot \mu$, thì $f = f'$ hầu khắp nơi địa phương theo $\mu$.

Điều kiện này hiển nhiên là cần thiết (Mệnh đề 2). Ngược lại, giả sử rằng mọi tập compact không đáng kể theo $\mu$ đều không đáng kể theo $\nu$. Ta đưa vào một sự phân mảnh $(K_\alpha)_{\alpha \in A}$ của T cho độ đo $\mu + \nu$ và đặt $N = T - \bigcup_{\alpha \in A} K_\alpha$. Hiển nhiên $(K_\alpha)_{\alpha \in A}$ là một sự phân mảnh cho $\mu$ và cho $\nu$, và do đó Mệnh đề 9 của §1, No. 8 kéo theo các hệ thức sau đây với mọi $g \in \mathcal{F}_+$:

$$
\mu^\bullet(g) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(g_{K_\alpha}), \quad \nu^\bullet(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^\bullet(g_{K_\alpha}).
$$

Xét một tập compact $C \subset K_\alpha$ không đáng kể theo $\mu_{K_\alpha}$; khi đó $C$ không đáng kể địa phương theo $\mu$, do đó không đáng kể địa phương theo $\nu$, và cuối cùng không đáng kể theo $\nu_{K_\alpha}$ theo định nghĩa của $\nu$. Khi đó từ định lý Lebesgue–Nikodym (Ch. V, §5, No. 5, Định lý 2) suy ra rằng $\nu_{K_\alpha}$ nhận một mật độ $f_\alpha$ đối với $\mu_{K_\alpha}$. Gọi $f$ là hàm trùng với $f_\alpha$ trên mỗi tập $K_\alpha$, và bằng 0 trên $N$; hàm $f$ là đo được theo $\mu$ (Ch. IV, §5, No. 10, Mệnh đề 16), và với mọi hàm $g \in \mathcal{F}_+$ ta có, theo các hệ thức trên và Mệnh đề 3 của Ch. V, §5, No. 3,

$$
\nu^\bullet(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^\bullet(g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_\alpha g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet((f g)_{K_\alpha}) = \mu^\bullet(f g).
$$

Trước hết suy ra rằng $f$ khả tích địa phương theo $\mu$: nếu $x$ là một điểm của T, và nếu $V$ là một lân cận của $x$ sao cho $\nu^\bullet(V) < +\infty$, thì $\mu^\bullet(f \varphi_V) < +\infty$. Tiếp theo, Mệnh đề 2 chỉ ra rằng các độ đo $\nu$ và $f \cdot \mu$ có cùng nguyên trên cốt yếu. Do đó chúng bằng nhau (§1, No. 2, Hệ quả của Mệnh đề 2). Tính duy nhất của $f$ là hiển nhiên dựa trên trường hợp các không gian compact, nên mệnh đề được chứng minh.

Nhận xét 3). — Lý thuyết về tích phân đối với một độ đo $\nu = f \cdot \mu$ được quy về ngay lý thuyết đã xét trong Ch. V. Thật vậy, cho $(K_\alpha)_{\alpha \in A}$ là một phân hoạch của T đối với $\mu$, do đó đối với $\nu$, và cho $T'$ là không gian compact địa phương được xác định trong Chú giải của §1, No. 8; ta có thể liên kết với $\mu$ (tương ứng với $\nu$) một độ đo $\mu'$ (tương ứng với $\nu'$) trên $T'$, sao cho các hàm đo được, các hàm khả tích cốt yếu nhận giá trị trong một không gian Banach, và các tích phân trên cốt yếu của các hàm dương, là như nhau đối với $\mu$ và $\mu'$ (tương ứng đối với $\nu$ và $\nu'$). Do đó hàm $f$ là $\mu'$-đo được; nó là $\mu'$-khả tích địa phương, vì $T'$ là compact địa phương, và một tập con compact của $T'$ chỉ giao với một số hữu hạn các tập compact $K_\alpha$ ($\alpha \in A$). Cuối cùng, quan hệ ${\nu'}^\bullet(g) = \nu^\bullet(g) = \mu^\bullet(fg) = {\mu'}^\bullet(fg)$ chứng minh rằng $\nu' = f \cdot \mu'$ (Ch. V, §5, No. 3, Prop. 3). Ta để lại cho người đọc nhiệm vụ chuyển các kết quả của Ch. V, §5.

### 3. Ảnh của một độ đo

#### Định nghĩa 4 {#int-ix-s2-def-4 .statement}

Cho $\pi$ là một ánh xạ từ T vào một không gian tôpô X. Ta nói rằng $\pi$ là $\mu$-thực sự nếu $\pi$ là $\mu$-đo được, và nếu mỗi điểm x của X thừa nhận một lân cận V sao cho $\mu^\bullet(\overline{\pi}(V)) < +\infty$.

#### Nhận xét 1 {#int-ix-s2-n3-rem-1 .statement}

Khi T và X là compact địa phương, định nghĩa này tương đương với định nghĩa trong Ch. V, §6, No. 1.
2) Một ánh xạ liên tục thực sự (GT, I, §10, No. 1, Def. 1) từ T vào X là $\mu$-thực sự đối với mọi độ đo $\mu$. Thật vậy, cho $x \in X$; vì $\overline{\pi}(x)$ là compact (loc. cit., No. 2, Th. 1), tập $\overline{\pi}(x)$ có một lân cận mở H sao cho $\mu^\bullet(H) < +\infty$. Đặt $V = X - \pi(T - H)$; vì $\pi$ là đóng, V là mở trong X, chứa x, và thỏa mãn $\overline{\pi}(V) \subset H$, do đó $\mu^\bullet(\overline{\pi}(V)) \leq \mu^\bullet(H) < +\infty$.
3) Nếu $\mu$ bị chặn, mọi ánh xạ $\mu$-đo được từ T vào X là $\mu$-thực sự.
4) Nếu $\theta$ là một độ đo phức trên T, $\pi$ được gọi là $\theta$-thực sự nếu $\pi$ là thực sự đối với độ đo dương $|\theta|$.

#### Mệnh đề 4 {#int-ix-s2-prop-4 .statement}

Cho $\pi$ là một ánh xạ $\mu$-thực sự từ T vào một không gian tôpô X. Tồn tại một và chỉ một độ đo $\nu$ trên X sao cho $\nu^\bullet$ bằng ảnh của $\pi(\mu^\bullet)$ (§1, No. 1), nói cách khác, sao cho $\nu^\bullet(g) = \mu^\bullet(g \circ \pi)$ với mọi $g \in \mathcal{F}_+(X)$.

Tính duy nhất là hiển nhiên (§1, No. 2, Hệ quả của Mệnh đề 2). Để thiết lập sự tồn tại, trước hết ta xét trường hợp $\mu$ được mang bởi một tập compact K, sao cho hạn chế của $\pi$ trên K là liên tục. Khi đó $L = \pi(K)$ là compact; gọi $\pi'$ là ánh xạ liên tục từ K vào L cảm sinh bởi $\pi$, và gọi $\nu'$ là độ đo ảnh $\pi'(\mu_K)$ trên L, $\nu$ là độ đo trên X được xác định bởi $\nu'$ (§1, No. 3, Ví dụ 2). Với mọi $g \in \mathcal{F}_+(X)$,

$$
\nu^\bullet(g) = {\nu'}^\bullet(g_L) = \mu_K^\bullet(g_L \circ \pi') = \mu_K^\bullet((g \circ \pi)_K) = \mu^\bullet((g \circ \pi)_K^0) = \mu^\bullet(g \circ \pi)
$$

(ta đã lần lượt sử dụng công thức (3) của §1, No. 3; Mệnh đề 2 của Ch. V, §6, No. 2; định nghĩa của $\mu_K^\bullet$; và sự kiện rằng $\mu$ được mang bởi K). Nói cách khác, $\nu^\bullet = \pi(\mu^\bullet)$.

Bây giờ ta chuyển sang trường hợp tổng quát; theo các Mệnh đề 10 và 9 của §1, No. 8, $\mu$ là tổng của một họ khả tổng $(\mu_\alpha)_{\alpha \in A}$ các độ đo có giá compact, sao cho hạn chế của $\pi$ trên giá $K_\alpha$ của $\mu_\alpha$ là liên tục với mọi $\alpha \in A$. Trường hợp đặc biệt đã xét ở trên cho phép gán cho mỗi độ đo $\mu_\alpha$ trên T một độ đo $\nu_\alpha$ trên X sao cho $\nu_\alpha^\bullet = \pi(\mu_\alpha^\bullet)$. Khi đó, với $g \in \mathcal{F}_+(X)$,

$$
\sum_{\alpha \in A} \nu_\alpha^\bullet(g) = \sum_{\alpha \in A} \mu_\alpha^\bullet(g \circ \pi) = \mu^\bullet(g \circ \pi).
$$

Độ đo $\pi(\mu^\bullet)$ bị chặn địa phương, vì $\pi$ là $\mu$-thực sự; do đó họ $(\nu_\alpha)_{\alpha \in A}$ là khả tổng (§1, No. 7, Mệnh đề 7), và tổng của nó $\nu$ thỏa mãn mệnh đề.

#### Định nghĩa 5 {#int-ix-s2-def-5 .statement}

*Nếu $\pi$ là một ánh xạ $\mu$-thực sự từ T vào một không gian tôpô X, thì độ đo duy nhất $\nu$ trên X sao cho $\nu^\bullet(g) = \mu^\bullet(g \circ \pi)$ với mọi $g \in \mathcal{F}_+(X)$ được gọi là độ đo ảnh của $\mu$ qua $\pi$, và được ký hiệu là $\pi(\mu)$.*

#### Ví dụ {#int-ix-s2-n3-exa-1 .statement}

— Cho K là một không gian con compact của T, i là đơn ánh chính tắc của K vào T, và $\lambda$ là một độ đo trên K; vì i là liên tục và $\lambda$ bị chặn, i là $\lambda$-thực sự. Công thức (3) của §1, No. 3 chỉ ra rằng "độ đo trên T được xác định bởi $\lambda$" là độ đo ảnh $i(\lambda)$.

*Nhận xét 5).* — Nếu $\theta$ là một độ đo thực và $\pi$ là $\theta$-thực sự, thì $\pi$ là thực sự đối với các độ đo $\theta^+$ và $\theta^-$; khi đó ta đặt $\pi(\theta) = \pi(\theta^+) - \pi(\theta^-)$. Nếu $\theta$ là một độ đo phức và $\pi$ là $\theta$-thực sự, thì $\pi$ là thực sự đối với các độ đo thực $\Re(\theta)$ và $\Im(\theta)$; khi đó ta đặt

$$
\pi(\theta) = \pi(\Re(\theta)) + i \pi(\Im(\theta)).
$$

#### Mệnh đề 5 {#int-ix-s2-prop-5 .statement}

*Cho $\pi$ là một ánh xạ $\mu$-thực sự của T vào một không gian tôpô X, và cho f là một ánh xạ của X vào một không gian tôpô F (Hausdorff hoặc không). Để f là $\pi(\mu)$-đo được, điều kiện cần và đủ là $f \circ \pi$ là $\mu$-đo được.*

Ta xét lại chứng minh của Mệnh đề 4, và bắt đầu với trường hợp đặc biệt được xét ở đầu, với cùng các ký hiệu; g là đo được đối với độ đo $\pi(\mu) = \nu$ khi và chỉ khi $g_L$ là $\nu'$-đo được (§1, No. 5, *Ví dụ*); khi đó, điều này tương đương với việc nói rằng $g_L \circ \pi' = (g \circ \pi)_K$ là $\mu_K$-đo được (Ch. V, §6, No. 2, Mệnh đề 3), và cuối cùng là $g \circ \pi$ là $\mu$-đo được (§1, No. 5, *Ví dụ*). Bây giờ ta chuyển sang trường hợp tổng quát, với cùng các ký hiệu như trong chứng minh của Mệnh đề 4; f là $\nu$-đo được khi và chỉ khi f là $\nu_\alpha$-đo được với mọi $\alpha \in A$ (§1, No. 7, Mệnh đề 8), do đó khi và chỉ khi $f \circ \pi$ là $\mu_\alpha$-đo được với mọi $\alpha \in A$ (trường hợp đặc biệt vừa xét) và cuối cùng khi và chỉ khi $f \circ \pi$ là $\mu$-đo được ($§ 1$, No. 7, Mệnh đề 8).

#### Hệ quả {#int-ix-s2-n3-cor-1 .statement}

— *Cho X và Y là hai không gian tôpô, $\pi$ là một ánh xạ $\mu$-thực sự của T vào X, và $\pi'$ là một ánh xạ $\pi(\mu)$-thực sự của X vào Y. Ánh xạ $\pi'' = \pi' \circ \pi$ khi đó là $\mu$-thực sự, và $\pi''(\mu) = \pi'(\pi(\mu))$ ('tính bắc cầu của các ảnh của độ đo').*

Vì, $\pi''$ là $\mu$-đo được (Mệnh đề 5). Đặt $\mu' = \pi(\mu)$; bao hàm ảnh $\pi'({\mu'}^\bullet) = \pi'(\pi(\mu^\bullet))$ hiển nhiên bằng $\pi''(\mu^\bullet)$. Vì nó bị chặn địa phương, $\pi''$ là $\mu$-thực sự. Khi đó các độ đo $\pi''(\mu)$ và $\pi'(\mu')$ có cùng tích phân trên cốt yếu, do đó bằng nhau.

#### Mệnh đề 6 {#int-ix-s2-prop-6 .statement}

— *Cho $\pi$ là một ánh xạ $\mu$-thực sự của T vào một không gian tôpô X, và cho B là một tập con $\pi(\mu)$-đo được của X. Đặt $A = \overline{\pi^{-1}(B)}$, và ký hiệu $\pi'$ là ánh xạ của A vào B trùng với $\pi$ trên A. Khi đó tập hợp A là $\mu$-đo được, $\pi_A$ và $\pi'$ là $\mu_A$-thực sự, và*

$$
(\pi(\mu))_B = (\pi_A(\mu_A))_B = \pi'(\mu_A).
$$

Tập hợp A là $\mu$-đo được theo Mệnh đề 5 áp dụng cho $\varphi_B$; ánh xạ $\pi_A$ rõ ràng là $\mu_A$-đo được theo định nghĩa của các độ đo cảm sinh (No. 1), và suy ra rằng $\pi'$ là đo được. Cho $f$ là một phần tử của $\mathscr{F}_+(B)$; ký hiệu các số mũ không là các mở rộng bằng 0 trong X và trong T, ta có

$$
(\pi(\mu)_B)^\bullet(f) = \pi(\mu)^\bullet(f^0) = \mu^\bullet(f^0 \circ \pi) = \mu^\bullet((f \circ \pi')^0) = \mu_A^\bullet(f \circ \pi'),
$$

do đó $(\pi(\mu)_B)^\bullet = \pi'(\mu_A^\bullet)$. Vì bao hàm $(\pi(\mu)_B)^\bullet$ bị chặn địa phương, điều tương tự đúng với $\pi'(\mu_A^\bullet)$ và do đó $\pi'$ là $\mu_A$-thực sự. Các độ đo $\pi'(\mu_A)$ và $(\pi(\mu))_B$ có cùng tích phân trên cốt yếu, do đó bằng nhau. Quan hệ kia có thể được thiết lập theo một cách tương tự.

#### Mệnh đề 7 {#int-ix-s2-prop-7 .statement}

— *Cho T là một không gian con của một không gian tôpô X, và cho i là đơn ánh của T vào X.

a) *Nếu $\mu$ là một độ đo trên T, và nếu i là $\mu$-thực sự, thì độ đo $i(\mu)$ tập trung trên T, và ta có $(i(\mu))_T = \mu$.

b) *Nếu $\lambda$ là một độ đo trên X sao cho T là $\lambda$-đo được, thì i là $\lambda_T$-thực sự, và $i(\lambda_T) = \varphi_T \cdot \lambda$.

a) Đặt $\nu = i(\mu)$; quan hệ $\nu^\bullet(A) = \mu^\bullet(A \cap T)$, áp dụng cho $A = X - T$, cho thấy rằng $\nu$ tập trung trên T. Quan hệ $\nu_T = \mu$ là một trường hợp đặc biệt của quan hệ (2), khi lấy $B = T = A$.

b) Cho $f$ là một hàm dương xác định trên X; đặt $\mu = \lambda_T$, ta có $\mu^\bullet(f \circ i) = \lambda_T^\bullet(f_T) = \lambda^\bullet(f \varphi_T) \leq \lambda^\bullet(f)$ (Mệnh đề 1); suy ra rằng i là $\mu$-thực sự. Mặt khác, $\mu^\bullet(f \circ i)$ (tương ứng $\lambda^\bullet(f \varphi_T)$) là tích phân trên cốt yếu của $f$ đối với $i(\mu)$ (tương ứng $\varphi_T \cdot \lambda$). Do đó hai độ đo này bằng nhau.

*Nhận xét 6).* — Cho $\pi$ là một ánh xạ $\mu$-thực sự từ $T$ vào một không gian tôpô $X$. Người ta quy giản lý thuyết tích phân đối với độ đo ảnh $\nu = \pi(\mu)$ về lý thuyết đã xét trong Ch. V, §6, theo cách sau. Cho $(K_\alpha)_{\alpha \in A}$ (tương ứng $(L_\beta)_{\beta \in B}$) là một phép chia vụn của $T$ (tương ứng của $X$) đối với $\mu$ (tương ứng đối với $\nu$), và đặt $N = T - \bigcup_{\alpha \in A} K_\alpha,\ P = X - \bigcup_{\beta \in B} L_\beta$. Ta có thể giả sử rằng hạn chế của $\pi$ trên mỗi $K_\alpha$ là liên tục (§1, No. 8, Mệnh đề 10). Gọi $T', X'$ là các không gian compact địa phương được xây dựng như trong Chú giải của §1, No. 8 và gọi $\mu'$ và $\nu'$ là các độ đo trên các không gian này liên kết với $\mu$ và $\nu$. Tôpô của $T'$ là tổng của các tôpô của các không gian con $K_\alpha$ và tôpô rời rạc trên $N$, $\pi$ là một ánh xạ liên tục từ $T'$ vào $X$ và quan hệ ${\mu'}^\bullet(g \circ \pi) = \mu^\bullet(g \circ \pi) = \nu^\bullet(g)$ (với $g \in \mathcal{F}_+(X)$) chỉ ra rằng $\pi$ là $\mu'$-thực sự và $\pi(\mu') = \nu$. Mặt khác, ánh xạ đồng nhất $i$ của $X$ lên $X'$ là $\nu$-thực sự, và $i(\nu) = \nu'$. Suy ra rằng $\pi$ là một ánh xạ $\mu'$-thực sự từ $T'$ vào $X'$, và ảnh của $\mu'$ qua $\pi$ là $\nu'$ (Hệ quả của Mệnh đề 5). Ta để lại cho người đọc nhiệm vụ chuyển các kết quả của Ch. V, §6.

### 4. Nâng độ đo

#### Mệnh đề 8 {#int-ix-s2-prop-8 .statement}

*Cho $T$ và $X$ là hai không gian tôpô, $\pi$ là một ánh xạ từ $T$ vào $X$.

a) Cho $\nu$ là một độ đo bị chặn trên $X$. Để tồn tại một độ đo $\mu$ trên $T$ sao cho $\pi$ là $\mu$-thực sự và $\pi(\mu) = \nu$, điều kiện cần và đủ là tồn tại, với mọi số $\varepsilon > 0$, một tập compact $K_\varepsilon \subset T$ sao cho hạn chế của $\pi$ trên $K_\varepsilon$ là liên tục và $\nu^\bullet(X - \pi(K_\varepsilon)) < \varepsilon$.

b) Giả sử rằng $\pi$ là đơn ánh; cho $\mu$ và $\mu'$ là hai độ đo trên $T$, sao cho $\pi$ là thực sự đối với $\mu$ và $\mu'$, và sao cho $\pi(\mu) = \pi(\mu')$. Khi đó $\mu = \mu'$.

Điều kiện được nêu trong *a)* là cần thiết. Thật vậy, nếu $\pi$ là $\mu$-thực sự và $\pi(\mu) = \nu$, quan hệ $\mu^\bullet(1) = \nu^\bullet(1) < +\infty$ kéo theo rằng $\mu$ bị chặn. Prop. 2 của §1, No. 2, áp dụng cho hàm 1, kéo theo sự tồn tại của một tập compact $K$ của $T$ sao cho $\mu^\bullet(T - K) < \varepsilon/2$. Vì $\pi$ là đo được đối với $\mu$, tồn tại một tập compact $K_\varepsilon \subset K$ sao cho hạn chế của $\pi$ trên $K_\varepsilon$ là liên tục, và sao cho $\mu^\bullet(K - K_\varepsilon) < \varepsilon/2$. Khi đó (No. 3, Prop. 4)

$$
\nu^\bullet(X - \pi(K_\varepsilon)) = \mu^\bullet(T - \overline{\pi}^{-1}(\pi(K_\varepsilon))) < \varepsilon.
$$

Để chứng minh rằng điều kiện là đủ, trước hết ta xét một trường hợp đặc biệt.

#### Bổ đề 1 {#int-ix-s2-lem-1 .statement}

Cho U và V là hai không gian compact, h là một ánh xạ liên tục từ U lên V. Khi đó ánh xạ $\lambda \mapsto h(\lambda)$ từ $\mathcal{M}_+(U)$ vào $\mathcal{M}_+(V)$ là toàn ánh.

Thật vậy, cho a là ánh xạ tuyến tính $f \mapsto f \circ h$ từ $\mathcal{C}(V)$ vào $\mathcal{C}(U)$; vì h là toàn ánh, a là một đẳng cấu đẳng cự của $\mathcal{C}(V)$ lên một không gian con H của $\mathcal{C}(U)$. Cho $\theta$ là một độ đo dương trên V; khi đó $\theta \circ a^{-1}$ là một dạng tuyến tính liên tục trên H, có thể mở rộng thành một dạng tuyến tính $\eta$ trên $\mathcal{C}(U)$ với cùng chuẩn, nhờ định lý Hahn–Banach (TVS, II, §3, No. 2, Hệ quả 3 của Định lý 1); khi đó $\eta$ là một độ đo trên U, và $\theta(f) = \eta(f \circ h)$ với mọi $f \in \mathcal{C}(V)$, do đó $\theta = h(\eta)$. Cuối cùng, $\theta(1) = \| \theta \| = \| \eta \|$, và $\theta(1) = \eta(1)$, do đó $\eta$ là dương (Ch. V, §5, No. 5, Mệnh đề 9).

Bây giờ ta chứng minh tính đủ của điều kiện được nêu trong a). Điều kiện này kéo theo sự tồn tại của một dãy $(K_n)_{n \geq 1}$ gồm các tập compact của T, sao cho hạn chế của $\pi$ trên mỗi $K_n$ là liên tục, và sao cho, với mọi $n$, $\nu^\bullet(X - \pi(K_n)) < 1/n$. Có thể giả sử rằng dãy $(K_n)$ là tăng. Đặt $L_n = \pi(K_n)$ và ký hiệu bởi $\nu'_n$ độ đo $\varphi_{L_n - L_{n-1}} \cdot \nu_{L_n}$ trên $L_n$, với quy ước $L_0 = \varnothing$.

Hạn chế $\pi_{K_n}$ liên tục, tồn tại một độ đo $\mu'_n$ trên $K_n$ sao cho $\pi_{K_n}(\mu'_n) = \nu'_n$ (Bổ đề 1). Gọi $\mu_n$ là ảnh của $\mu'_n$ qua đơn ánh chính tắc của $K_n$ vào T, và gọi g là một phần tử của $\mathcal{F}_+(X)$. Lần lượt sử dụng sự kiện rằng $\nu$ tập trung trên $\bigcup L_n$, Mệnh đề 4 của §1, No. 5; Mệnh đề 2 của §1, No. 2; Mệnh đề 4 của No. 3, và cuối cùng là Mệnh đề 7 của No. 3, ta có

$$
\nu^\bullet(g) = \sum_n \nu^\bullet(\varphi_{L_n - L_{n-1}} g) = \sum_n \nu'_n \bullet (g_{L_n}) = \sum_n \mu'_n \bullet (g_{L_n} \circ \pi_{K_n})
$$
$$
= \sum_n \mu'_n \bullet ((g \circ \pi)_{K_n}) = \sum_n \mu_n^\bullet (g \circ \pi).
$$

Lấy $g = 1$ trong công thức này, ta thấy rằng họ $(\mu_n)$ là khả tổng và tổng của nó là một độ đo bị chặn $\mu$ (§1, No. 7, Mệnh đề 7). Theo Mệnh đề 5 của No. 3, ánh xạ $\pi$ là $\mu_n$-đo được với mọi $n$, vì $\pi_{K_n}$ liên tục, do đó $\mu'_n$-đo được; suy ra $\pi$ là $\mu$-đo được (§1, No. 7, Mệnh đề 8), do đó $\mu$-thực sự vì $\mu$ bị chặn. Các quan hệ trên khi đó chứng minh rằng các độ đo $\pi(\mu)$ và $\nu$ có cùng tích phân trên cốt yếu, do đó chúng bằng nhau (§1, No. 2, Hệ quả của Mệnh đề 2).

Cuối cùng, giả sử rằng $\pi$ là đơn ánh, và ta chứng minh b). Gọi f là một phần tử của $\mathcal{F}_+(T)$; vì $\pi$ là đơn ánh, tồn tại một hàm $g \in \mathcal{F}_+(X)$ sao cho $f = g \circ \pi$ và, đặt $\nu = \pi(\mu) = \pi(\mu')$, theo Mệnh đề 4 của No. 3 ta có

$$
\mu^\bullet(f) = \mu^\bullet(g \circ \pi) = \nu^\bullet(g) = {\mu'}^\bullet(g \circ \pi) = {\mu'}^\bullet(f).
$$

Hai độ đo $\mu$ và $\mu'$ do đó có cùng tích phân trên cốt yếu, điều này kéo theo chúng bằng nhau (§ 1, No. 2, Hệ quả của Mệnh đề 2).

#### Nhận xét {#int-ix-s2-n4-rem-1 .statement}

Giả sử rằng $\pi$ là đơn ánh. Gọi $\theta$ là một độ đo phức sao cho $\pi$ là $\theta$-thực sự và $\pi(\theta) = 0$; khi đó $\theta = 0$. Thật vậy, bằng cách tách $\theta$ thành các phần thực và ảo của nó, ta có thể rút gọn về trường hợp $\theta$ là thực. Khi đó ta có $\pi(\theta^+) = \pi(\theta^-)$, do đó $\theta^+ = \theta^-$ (Mệnh đề 8), và cuối cùng $\theta = 0$.

Sau đây là một trường hợp quan trọng trong đó điều kiện a) của Mệnh đề 8 luôn được thỏa mãn.

#### Mệnh đề 9 {#int-ix-s2-prop-9 .statement}

— *Cho T là một không gian Souslin* (GT, IX, §6, No. 2, Định nghĩa 2), *X là một không gian Hausdorff*, $\pi$ *là một ánh xạ liên tục từ T lên X*, và $\nu$ *là một độ đo bị chặn trên X*. *Khi đó tồn tại một độ đo bị chặn $\mu$ trên T sao cho $\pi(\mu) = \nu$*.

Các giả thiết hiển nhiên kéo theo rằng X là một không gian Souslin.

Ta xét hàm tập hợp $c : A \mapsto \nu^\bullet(\pi(A))$ trên $\mathfrak{P}(T)$. Quan hệ $A \subset B$ kéo theo $c(A) \leq c(B)$; nếu $(A_n)$ là một dãy tăng các tập con của T, và nếu $A = \bigcup_{n \in \mathbf{N}} A_n$, thì $c(A) = \sup_n c(A_n)$ do tính chất $\nu^\bullet$ là một độ cản. Cuối cùng, cho $A \subset T$ và cho $\varepsilon$ là một số $> 0$; chọn một tập con mở G của X chứa $\pi(A)$, sao cho $\nu^\bullet(G) \leq \nu^\bullet(\pi(A)) + \varepsilon$ (§ 1, No. 9, Mệnh đề 13); tập con mở $H = \overline{\pi^{-1}(G)}$ của T chứa A, và $c(H) \leq c(A) + \varepsilon$. Do đó hàm c là một dung lượng liên tục phải trên T (TG, IX, §6, No. 10, Định nghĩa 9)(1) và định lý về khả năng dung lượng (*loc. cit.*, Th. 6) suy ra đẳng thức $c(T) = \sup_K c(K)$, trong đó K chạy trên tập hợp các tập con compact của T. Mệnh đề 8 sau đó suy ra sự tồn tại của độ đo cần tìm $\mu$.

### 5. Tích của hai độ đo

Cho S và T là hai không gian tôpô, lần lượt được trang bị hai tiền độ đo (dương) $\lambda$ và $\mu$, và cho X là không gian tích $S \times T$. Cho K là một tập con compact của X; ký hiệu A và B lần lượt là các phép chiếu của K lên S và T, và đặt

$$
\nu_K = (\lambda_A \otimes \mu_B)_K .
$$

Ta như vậy định nghĩa một tiền độ đo trên X. Thật vậy, cho L là một tập con compact của X chứa K, và cho C và D là hai phép chiếu của nó; khi đó $A \subset C$, $B \subset D$,

(1) Một dung lượng $f$ trên T được gọi là liên tục phải nếu, với mọi tập compact K trong T, $f(K) = \inf_U f(U)$ khi U chạy trên các tập mở $U \supset K$. Khái niệm này không được định nghĩa trong GT, được dịch từ một ấn bản trước của Ch. IX.

do đó, sử dụng tính bắc cầu của các độ đo cảm sinh, và Mệnh đề 12 của Ch. V, §8, No. 5, ta có

$$
(\nu_L)_K = ((\lambda_C \otimes \mu_D)_L)_K = (\lambda_C \otimes \mu_D)_K \\
= ((\lambda_C \otimes \mu_D)_{A \times B})_K = (\lambda_A \otimes \mu_B)_K = \nu_K .
$$

#### Định nghĩa 6 {#int-ix-s2-def-6 .statement}

*$\nu$ tiền độ đo được định nghĩa bởi (3) được gọi là tiền độ đo tích của $\lambda$ và $\mu$, và được ký hiệu là $\lambda \otimes \mu$.*

Định nghĩa này hiển nhiên mở rộng sang trường hợp $\lambda$ và $\mu$ là các tiền độ đo phức, và khi đó ta có $|\lambda \otimes \mu| = |\lambda| \otimes |\mu|$ (Ch. III, §4, No. 2, Mệnh đề 3 và Ch. IV, §5, No. 7, Bổ đề 3).

Ta giữ lại các ký hiệu của Ch. III, §4 và Ch. V, §8 liên quan đến các tích của độ đo và các tích phân lặp. Đặc biệt, nếu $f$ và $g$ là hai hàm lần lượt được xác định trên $S$ và $T$, với các giá trị trong $\overline{\mathbf{R}}_+$ hoặc trong $\mathbf{C}$, thì hàm $(s, t) \mapsto f(s)g(t)$ trên $S \times T$ sẽ được ký hiệu là $f \otimes g$.

#### Mệnh đề 10 {#int-ix-s2-prop-10 .statement}

*Cho $\nu$ là tiền độ đo tích của $\lambda$ và $\mu$; với mọi hàm $f \in \mathcal{F}_+(S)$ và mọi hàm $g \in \mathcal{F}_+(T)$,*

$$
\nu^\bullet(f \otimes g) = \lambda^\bullet(f)\mu^\bullet(g) .
$$

*Tiền độ đo $\nu$ là tiền độ đo duy nhất trên $S \times T$ thỏa mãn (4).*

Khi $K$ (tương ứng $L$) chạy trên tập hợp các tập con compact của $S$ (tương ứng của $T$), ta có

$$
\begin{align*}
\nu^\bullet(f \otimes g) &= \sup_{K,L} \nu^\bullet_{K \times L}((f \otimes g)_{K \times L}) = \sup_{K,L} (\lambda_K \otimes \mu_L)^\bullet(f_K \otimes g_L) \\
&= \sup_{K,L} \lambda_K^\bullet(f_K) \cdot \mu_L^\bullet(g_L) = (\sup_K \lambda_K^\bullet(f_K)) (\sup_L \mu_L^\bullet(g_L)) \\
&= \lambda^\bullet(f)\mu^\bullet(g)
\end{align*}
$$

theo Mệnh đề 8 của Ch. V, §8, No. 3.

Cho $\eta$ là một tiền độ đo thứ hai trên $S \times T$ thỏa mãn (4), và cho $K$ và $L$ lần lượt là các tập con compact của $S$ và $T$, $f$ và $g$ lần lượt là các phần tử của $\mathcal{F}_+(K)$ và $\mathcal{F}_+(L)$. Ta có quan hệ $(f \otimes g)^0 = f^0 \otimes g^0$ giữa các mở rộng bằng 0, do đó (§1, No. 2, Prop. 2)

$$
\eta^\bullet_{K \times L}(f \otimes g) = \eta^\bullet((f \otimes g)^0) = \eta^\bullet(f^0 \otimes g^0) \\
= \lambda^\bullet(f^0)\mu^\bullet(g^0) = \lambda_K^\bullet(f)\mu_L^\bullet(g) .
$$

Đặc biệt, nếu lấy $f \in \mathcal{K}_+(K)$, $g \in \mathcal{K}_+(L)$, ta thấy rằng $\eta_{K \times L}$ có tính chất đặc trưng của độ đo tích $\lambda_K \otimes \mu_L$ (Ch. III, §4, No. 1, Th. 1). Do đó $\eta_{K \times L} = \nu_{K \times L}$; vì mọi tập con compact của $S \times T$ đều được chứa trong một tập có dạng $K \times L$, tính bắc cầu của các độ đo cảm sinh suy ra rằng $\eta = \nu$.

#### Hệ quả 1 {#int-ix-s2-prop-10-cor-1 .statement}

— *Nếu $\lambda$ và $\mu$ là các độ đo, thì $\nu$ là một độ đo.*

Thật vậy, cho $x = (s, t)$ là một điểm của $X$, và cho $U$ và $V$ lần lượt là các lân cận của $s, t$, sao cho $\lambda^\bullet(U) < +\infty$, $\mu^\bullet(V) < +\infty$; tập hợp $U \times V$ là một lân cận của $x$, và $\nu^\bullet(U \times V) = \lambda^\bullet(U)\mu^\bullet(V) < +\infty$ theo (4); bao hàm $\nu^\bullet$ do đó bị chặn địa phương, và tiền độ đo $\nu$ là một độ đo.

Kết quả này mở rộng ngay lập tức đến các độ đo phức.

#### Hệ quả 2 {#int-ix-s2-prop-10-cor-2 .statement}

— *Nếu $A$ là một tập con của $S$ không đáng kể địa phương đối với $\lambda$, thì $A \times T$ là không đáng kể địa phương đối với $\nu$.*

#### Hệ quả 3 {#int-ix-s2-prop-10-cor-3 .statement}

— *Giả sử rằng $\lambda$ (tương ứng $\mu$) là tổng của một họ cộng được $(\lambda_\alpha)_{\alpha \in A}$ (tương ứng $(\mu_\beta)_{\beta \in B}$) các độ đo trên $S$ (tương ứng $T$). Khi đó họ $(\lambda_\alpha \otimes \mu_\beta)_{(\alpha, \beta) \in A \times B}$ là cộng được, và tổng của nó là $\lambda \otimes \mu$.*

Thật vậy, cho $p$ là bao hàm $\sum_{\alpha, \beta} (\lambda_\alpha \otimes \mu_\beta)^\bullet$; nếu $f \in \mathcal{F}_+(S)$ và $g \in \mathcal{F}_+(T)$, thì hiển nhiên $p(f \otimes g) = \lambda^\bullet(f)\mu^\bullet(g)$. Chứng minh của Hệ quả 1 khi đó chỉ ra rằng $p$ bị chặn địa phương, do đó họ $(\lambda_\alpha \otimes \mu_\beta)$ là cộng được (§ 1, No. 7, Prop. 7). Tổng của nó $\eta$ khi đó thỏa mãn $\eta^\bullet = p$ (§ 1, No. 7, Prop. 7), và Mệnh đề 10 suy ra $\eta = \nu$.

### 6. Tích phân đối với tích của hai độ đo

*Trong suốt số này, $\lambda$ và $\mu$ lần lượt ký hiệu các độ đo trên $S$ và $T$, và $\nu$ ký hiệu độ đo tích $\lambda \otimes \mu$ trên $S \times T$. Ngoài ra, nếu $f$ là một hàm dương trên $S \times T$, thì với mọi $s \in S$ ta ký hiệu bởi $f_s$ hàm $t \mapsto f(s, t)$ trên $T$, và bởi $I_f$ hàm $s \mapsto \mu^\bullet(f_s)$ trên $S$.*

#### Bổ đề 2 {#int-ix-s2-lem-2 .statement}

*Cho $f$ là một hàm dương khả đo được theo $\nu$ trên $S \times T$; với mọi tập con compact $L$ của $T$, ký hiệu $I_f^L$ là hàm $s \mapsto \mu^\bullet(f_s \varphi_L)$ trên $S$. Khi đó hàm $I_f^L$ là $\lambda$-có thể đo được, và*

$$
(5) \quad I_f = \sup_L I_f^L
$$
$$
(6) \quad \nu^\bullet(f) = \sup_L \lambda^\bullet(I_f^L),
$$

*trong đó $L$ chạy qua tập hợp các tập con compact của $T$.*

Trước hết ta lưu ý rằng bao hàm $L \subset L'$ kéo theo $I_f^L \leq I_f^{L'}$; mặt khác, $I_f^L(s) = \mu_L^\bullet((f_s)_L)$ với mọi $s \in S$. Do đó công thức (5) là một hệ quả ngay lập tức của định nghĩa của độ đo bao $\mu^\bullet$ đã cho trong

§1, No. 2. Nếu K là một tập con compact của S, và L là một tập con compact của T, thì $\nu_{K \times L} = \lambda_K \otimes \mu_L$ theo phép dựng, và Mệnh đề 7 của Ch. V, §8, No. 3 suy ra quan hệ

$$
\nu^\bullet(f \varphi_{K \times L}) = \lambda_K^\bullet((I_f^L)_K).
$$

Hơn nữa, mọi tập con compact của $S \times T$ đều được chứa trong một tập compact có dạng $K \times L$; chuyển qua bao trên theo mọi K và L trong công thức trước, ta do đó được

$$
\nu^\bullet(f) = \sup_L \sup_K \lambda_K^\bullet((I_f^L)_K) = \sup_L \lambda^\bullet(I_f^L),
$$

nghĩa là (6).

Cuối cùng, Mệnh đề 7 của Ch. V, §8, No. 3 suy ra rằng hạn chế của $I_f^L$ lên mọi tập con compact K của S là $\lambda_K$-có thể đo được; điều đó tương đương với nói rằng $I_f^L$ là $\lambda$-có thể đo được.

#### Mệnh đề 11 {#int-ix-s2-prop-11 .statement}

*Cho f là một hàm nửa liên tục dưới $\geqslant 0$ được xác định trên $X = S \times T$.*

a) *Hàm $f_s : t \mapsto f(s, t)$ là nửa liên tục dưới trên T với mọi $s \in S$.*

b) *Hàm $I_f : s \mapsto \int^\bullet f(s, t) d\mu(t)$ là nửa liên tục dưới trên S, và*

$$
\iint_X^\bullet f(s, t) d\nu(s, t) = \int_S^\bullet d\lambda(s) \int_T^\bullet f(s, t) d\mu(t).
$$

Tính chất *a)* là hiển nhiên, vì ánh xạ $t \mapsto f(s, t)$ của T vào $\overline{\mathbf{R}}$ là hợp thành của $f$ với ánh xạ liên tục $t \mapsto (s, t)$ của T vào X. Để chứng minh *b)*, ta sẽ dùng một bổ đề:

#### Bổ đề 3 {#int-ix-s2-lem-3 .statement}

— *Cho X là một không gian tôpô (Hausdorff hay không), f là một hàm nửa liên tục dưới $\geqslant 0$ được xác định trên X; khi đó f là giới hạn của một dãy tăng $(f_n)_{n \in \mathbf{N}}$ các hàm nửa liên tục dưới trên X, sao cho mỗi hàm $f_n$ là một tổ hợp tuyến tính, với các hệ số dương, của các hàm đặc trưng của các tập mở.*

Cho hai số nguyên $k \geqslant 1$ và $n \geqslant 1$, ta ký hiệu bởi $J_{kn}$ hàm đặc số của khoảng $]k/2^n, +\infty]$ của $\overline{\mathbf{R}}$. Với mọi $x \in \overline{\mathbf{R}}_+$, đặt

$$
u_n(x) = 2^{-n} \sum_{k=1}^{n \cdot 2^n} J_{kn}(x);
$$

ta thấy ngay rằng dãy $(u_n(x))_{n \geqslant 1}$ là tăng và nhận x làm giới hạn. Dãy các hàm $f_n = u_n \circ f$ do đó là tăng và hội tụ về $f$, và ta có $f_n = 2^{-n} \sum_{k=1}^{n \cdot 2^n} \varphi_{U(k,n)}$,
trong đó $U(k,n)$ là tập mở $f^{-1}([k/2^n, +\infty])$ của $X$.

Ta chuyển qua chứng minh của b). Vì hàm $I_f$ là bao trên của họ có hướng tăng của các hàm $I_f^L$, trong đó $L$ chạy trên tập hợp các tập con compact của $T$ (Bổ đề 2), nên chỉ cần chứng minh rằng các hàm $I_f^L$ là nửa liên tục dưới; khi đó công thức (9) có thể được suy ra từ (6) bằng cách chuyển qua bao trên theo $L$ (§ 1, No. 6, Mệnh đề 5).

Vậy cho $\mathcal{H}$ là tập hợp các hàm dương nửa liên tục dưới $f$ trên $S \times T$ sao cho $I_f^L$ là nửa liên tục dưới với mọi tập con compact $L$ của $T$. Theo Mệnh đề 5 của § 1, No. 6, bao trên của mọi tập có hướng tăng các phần tử của $\mathcal{H}$ thuộc về $\mathcal{H}$. Theo Bổ đề 3, do đó chỉ cần chứng minh rằng hàm đặc số của một tập mở $W$ của $S \times T$ thuộc về $\mathcal{H}$. Hơn nữa, theo định nghĩa của tôpô tích trên $S \times T$, tập mở $W$ là hợp của một họ có hướng tăng $(W_\alpha)_{\alpha \in A}$ các tập mở có dạng
$$
W = \bigcup_{1 \leq i \leq n} (U_i \times V_i),
$$
trong đó các $U_i$ là mở trong $S$ và các $V_i$ là mở trong $T$; theo các nhận xét đã nêu ở trên, chỉ cần chứng minh rằng hàm đặc số của một tập mở như vậy thuộc về $\mathcal{H}$. Khi đó cho $s \in S$, và cho $U$ là giao của họ (có thể rỗng) tạo bởi các tập mở $U_i$ chứa $s$; ta thấy ngay rằng $\varphi_W(s,t) \leq \varphi_W(s',t)$ với mọi $s' \in U$ và $t \in T$, do đó, bằng cách lấy tích phân, $I_{\varphi_W}^L(s) \leq I_{\varphi_W}^L(s')$ với mọi $s' \in U$. Do đó $I_{\varphi_W}^L$ là nửa liên tục dưới, và mệnh đề được chứng minh.

#### Hệ quả 1 {#int-ix-s2-lem-3-cor-1 .statement}

*Cho $f$ là một hàm số dương xác định trên $X = S \times T$; khi đó*
$$
\iint_X^* f(s,t)\, d\nu(s,t) \geq \int_S^* d\lambda(s) \int_T^* f(s,t)\, d\mu(t).
$$

Thật vậy, cho $g$ là một hàm nửa liên tục dưới trên $X$ sao cho $g \geq f$; theo Mệnh đề 11,
$$
\iint_X^* g(s,t)\, d\nu(s,t) = \iint^* g(s,t)\, d\nu(s,t) = \int^* d\lambda(s) \int^* g(s,t)\, d\mu(t)
$$
$$
= \int^* d\lambda(s) \int^* g(s,t)\, d\mu(t) \geq \int^* d\lambda(s) \int^* f(s,t)\, d\mu(t).
$$
Bất đẳng thức (10) thu được bằng cách chuyển qua bao dưới theo $g$.

#### Hệ quả 2 {#int-ix-s2-lem-3-cor-2 .statement}

— Cho $f$ là một hàm số xác định trên $S \times T$ và $\nu$-không đáng kể. Khi đó hàm $f_s : t \mapsto f(s, t)$ là $\mu$-không đáng kể với $\lambda$-hầu khắp mọi $s \in S$.

#### Mệnh đề 12 {#int-ix-s2-prop-12 .statement}

— Cho $f$ là một hàm dương $\nu$-đo được trên $X = S \times T$. Giả sử rằng $f$ là $\nu$-điều độ (tương ứng rằng $\mu$ là điều độ). Khi đó:
a) Tập $N$ gồm các $s \in S$ sao cho hàm $f_s : t \mapsto f(s, t)$ không $\mu$-đo được là tập không đáng kể (tương ứng địa phương không đáng kể) đối với $\lambda$.
b) Ánh xạ $s \mapsto \int^\bullet f(s, t) \, d\mu(t)$ là $\lambda$-đo được, và

$$
\iint_X^\bullet f(s, t) \, d\nu(s, t) = \int_S^\bullet d\lambda(s) \int_T^\bullet f(s, t) \, d\mu(t).
$$

Ta bắt đầu bằng cách thiết lập b) khi $f$ là $\nu$-điều độ. Theo Bổ đề 2, phần này của mệnh đề đúng khi tồn tại một tập con compact $L$ của $T$ sao cho $f$ bằng không ngoài $S \times L$; vì, trong trường hợp này $I_f = I_f^{L'}$ với mọi tập con compact $L'$ của $T$ chứa $L$, và công thức (11) rút về (6). Đặc biệt, b) được thiết lập cho một hàm $f$ bằng không ngoài một tập con compact của $S \times T$. Mặt khác, Hệ quả 1 của Mệnh đề 11 suy ra rằng b) đúng khi $f$ là $\nu$-không đáng kể. Vì mọi hàm $\nu$-điều độ đều là tổng của một hàm $\nu$-không đáng kể và một dãy các hàm có giá compact (§ 1, No. 9, Hệ quả 3 của Mệnh đề 14), nên mệnh đề b) đúng khi $f$ là $\nu$-điều độ.

Tương tự, mệnh đề b) là hiển nhiên khi $\mu$ được mang bởi một tập con compact $L$ của $T$ (Bổ đề 2). Giả sử rằng $\mu$ là điều độ; khi đó tồn tại một dãy $(\mu_n)_{n \in \mathbf{N}}$ các độ đo trên $T$ có giá compact, sao cho $\mu = \sum_n \mu_n$ (§ 1, No. 9, Hệ quả 5 của Mệnh đề 14), do đó $\nu = \sum_n \lambda \otimes \mu_n$ (No. 5, Hệ quả 3 của Mệnh đề 10). Mệnh đề b), vì đúng cho từng độ đo $\nu_n = \lambda \otimes \mu_n$, cũng đúng cho $\nu = \sum_n \nu_n$.

Chúng ta chứng minh a); ký hiệu $N$ là tập hợp các $s \in S$ sao cho $f_s$ không phải là $\mu$-đo được; với mọi tập con compact $L$ của $T$, tương tự ký hiệu $N_L$ là tập hợp các $s \in S$ sao cho $f_s \varphi_L$ không phải là $\mu$-đo được. Nếu $K$ và $L$ là các tập compact trong $S$ và $T$ tương ứng, thì $f_{K \times L}$ đo được đối với độ đo $\nu_{K \times L} = \lambda_K \otimes \mu_L$, và Mệnh đề 2 của Ch. V, § 8, No. 2 cho thấy rằng tập $N_L$ là không đáng kể địa phương đối với $\lambda_K$; vì $K$ tùy ý, nên $N_L$ là $\lambda$-không đáng kể địa phương.

Giả sử rằng $f$ bằng không ở ngoài một tập compact dạng $K \times L$; khi đó $N = N_L$, và $N$ được chứa trong $K$; suy ra $N$ là $\lambda$-không đáng kể. Tương tự, nếu $f$ là $\nu$-không đáng kể, Hệ quả 2 của Mệnh đề 11 suy ra rằng $N$ là $\lambda$-không đáng kể. Trường hợp $f$ là $\nu$-điều hòa thì có thể xử lý như trên, bằng cách kết hợp hai trường hợp trước.

Giả sử rằng $\mu$ được mang bởi một tập con compact $L$ của $T$; khi đó lại $N = N_L$, do đó $N$ là $\lambda$-không đáng kể địa phương. Vì mọi độ đo điều hòa đều là tổng của một dãy các độ đo có giá đỡ compact ($§ 1$, No. 9, Hệ quả 5 của Mệnh đề 14), kết quả này được suy rộng ngay sang trường hợp $\mu$ là điều hòa, bằng cách dùng Mệnh đề 8 của $§ 1$, No. 7.

#### Nhận xét {#int-ix-s2-n6-rem-1 .statement}

— Cho $(K_\alpha)_{\alpha \in A}$ là một phép co của $S$ đối với $\lambda$ và đặt $M = S - \bigcup_{\alpha \in A} K_\alpha$; định nghĩa một cách tương tự $(L_\beta)_{\beta \in B}$ và $N$ đối với độ đo $\mu$ trên $T$. Ta ký hiệu bởi $S'$ không gian compact địa phương là tổng của các không gian con $K_\alpha$ của $S$ và không gian *rời rạc* $M$; không gian $T'$ được định nghĩa tương tự, và ta đặt $X' = S' \times T'$. Không gian compact địa phương $X'$ là tổng của họ $(K_\alpha \times L_\beta)_{(\alpha, \beta) \in A \times B}$ các không gian con compact của $X$ và không gian con $P = (M \times T) \cup (S \times N)$ là một tập con không đáng kể địa phương theo $\nu$ của $X$ (ta nhận thấy rằng nói chung $P$ không phải là một không gian rời rạc). Trong *Chú giải* của $§ 1$, No. 8 ta đã thấy rằng tồn tại một độ đo $\lambda'$ trên $S'$ sao cho các hàm đo được, tích phân trên cốt yếu của các hàm dương, các hàm khả tích cốt yếu và các tích phân của chúng, là như nhau đối với $\lambda$ và $\lambda'$. Ta liên kết độ đo $\mu'$ trên $T'$ với $\mu$, và độ đo $\nu'$ trên $X'$ với $\nu$, phù hợp với Chú giải đã dẫn; ta thấy ngay lập tức rằng ${\nu'}^\bullet(f \otimes g) = {\lambda'}^\bullet(f) {\mu'}^\bullet(g)$ đối với $f \in \mathcal{F}_+(S)$ và $g \in \mathcal{F}_+(T)$; do đó $\nu' = \lambda' \otimes \mu'$ theo Mệnh đề 10 của No. 5. Vì tôpô của $X'$ mịn hơn tôpô của $X$, mọi hàm $\nu$-điều hòa đều là $\nu'$-điều hòa. Thủ tục này cho phép mở rộng không cần chứng minh mới định lý Lebesgue–Fubini (Ch. V, $§ 8$, No. 4, Th. 1) sang tình huống hiện tại.

### 7. Một kết quả về sự phân rã của các độ đo

#### Mệnh đề 13 {#int-ix-s2-prop-13 .statement}

*Cho $X$ là một không gian tôpô, $\nu$ là một độ đo điều hòa trên $X$, $p$ là một ánh xạ $\nu$-thực sự của $X$ vào một không gian tôpô $T$, và $\mu = p(\nu)$. Giả sử rằng mọi không gian con compact của $X$ đều mêtric hóa được. Khi đó tồn tại một ánh xạ $t \mapsto \lambda_t$ từ $T$ vào $\mathcal{M}_+(X)$ có các tính chất sau:*

a) với mọi $t \in T$, độ đo $\lambda_t$ được mang bởi $\overline{p}^{-1}(t)$;
b) với mọi hàm dương đo được phổ quát$^{(1)}$ $f$ trên $X$, hàm $t \mapsto \lambda_t^\bullet(f)$ là đo được phổ quát trên $T$ và*

$$
\int_X f(x)\, d\nu(x) = \int_T d\mu(t) \int_X f(x)\, d\lambda_t(x);
$$

(1) Một ánh xạ của một không gian tôpô $X$ vào một không gian tôpô $Y$ được gọi là *đo được phổ quát* nếu nó là $\mu$-đo được đối với mọi độ đo $\mu$ trên $X$ (xem Ch. V, $§ 3$, No. 4).

c) tập hợp các $t \in T$ sao cho $\lambda_t(1) \neq 1$ là địa phương $\mu$-không đáng kể.
Ngoài ra, nếu $t \mapsto \lambda'_t$ là một ánh xạ của $T$ vào $\mathcal{M}_+(X)$ thỏa mãn các điều kiện a) và b), thì tập hợp các $t \in T$ sao cho $\lambda_t \neq \lambda'_t$ là địa phương $\mu$-không đáng kể.
Ta sẽ cần một kết quả phụ trợ:

#### Bổ đề 4 {#int-ix-s2-lem-4 .statement}

Cho $X$ là một không gian tôpô, $\nu$ là một độ đo trên $X$, và $f$ là một ánh xạ $\nu$-đo được của $X$ vào một không gian tôpô $F$ (Hausdorff hoặc không). Tồn tại một ánh xạ $f'$ đo được phổ quát của $X$ vào $F$, bằng $f$ địa phương $\nu$-hầu khắp nơi.

Chứng minh giống hệt như chứng minh của Mệnh đề 7 của Ch. V, §3, No. 4, khi tính đến Mệnh đề 10 của §1, No. 8.

Chúng ta chuyển sang chứng minh Mệnh đề 13.
A) Giả sử rằng $X$ là compact và khả metric và $p$ là liên tục và toàn ánh:
Không gian $T$ khi đó là compact và khả metric (GT, IX, §2, No. 10). Theo Định lý 1 của Ch. VI, §3, No. 1, tồn tại một ánh xạ $H : t \mapsto \eta_t$ từ $T$ vào $\mathcal{M}_+(X)$, đo được mơ hồ theo $\mu$ và khả tích theo $\mu$ một cách cốt yếu theo vô hướng, sao cho $\nu = \int_T \eta_t \, d\mu(t)$ và sao cho $\eta_t$ có khối lượng toàn phần bằng 1 và được mang bởi $\overline{p}(t)$ với mọi $t \in T$. Cho $(S_n)_{n \in \mathbf{N}}$ là một phân mảnh của $T$ đối với $\mu$, sao cho hạn chế của $H$ trên mỗi tập hợp $S_n$ là liên tục (§1, No. 8, Mệnh đề 10 và 11); ta ký hiệu $\Lambda : t \mapsto \lambda_t$ là ánh xạ từ $T$ vào $\mathcal{M}_+(X)$ bằng $H$ trên $S = \bigcup_{n \in \mathbf{N}} S_n$ và bằng 0 trên $T - S$. Hiển nhiên $\nu = \int_T \lambda_t \, d\mu(t)$ và $\Lambda$ thỏa mãn điều kiện a) của mệnh đề.
Cho $\theta$ là một độ đo trên $T$; ánh xạ $\Lambda$ đo được mơ hồ theo $\theta$ và khả tích theo $\theta$ một cách cốt yếu theo vô hướng, do đó cũng $\theta$-thích hợp (Ch. V, §3, No. 1, Mệnh đề 2 b)). Cho $f$ là một hàm dương đo được phổ quát trên $X$; theo Mệnh đề 5 của Ch. V, §3, No. 2 áp dụng cho $\int \lambda_t \, d\theta(t)$, ánh xạ $t \mapsto \lambda_t^\bullet(f)$ là đo được theo $\theta$, do đó đo được phổ quát vì $\theta$ tùy ý.
Công thức (12) suy ra từ Mệnh đề 5 của Ch. V, §3, No. 2.
B) Giả sử tồn tại một tập con compact $X'$ của $X$ mang độ đo $\nu$ và sao cho $p_{X'}$ liên tục:
Đặt $T' = p(X')$, và $p' = p_{X'}$; ký hiệu $\nu'$ là độ đo $\nu_{X'}$, và $\mu'$ là độ đo ảnh $p'(\nu')$ trên $T'$. Vì $p'$ liên tục và toàn ánh, và vì $X'$ compact và khả metric, theo A) tồn tại một ánh xạ $\Lambda' : t' \mapsto \lambda'_{t'}$ từ $T'$ vào $\mathcal{M}_+(X')$ thỏa mãn các điều kiện sau:
a') với mọi $t' \in T'$, độ đo $\lambda'_{t'}$ được mang bởi $X' \cap \overline{p}'(t')$;
b') với mọi hàm dương đo được phổ quát $f'$ trên $X'$, hàm $t' \mapsto {\lambda'_{t'}}^\bullet(f')$ là đo được phổ quát trên $T'$ và
$$
\int_{X'} f'(x') \, d\nu'(x') = \int_{T'} d\mu'(t') \int_{X'} f'(x') \, d\lambda'_{t'}(x').
$$

Cho $t \in T$; nếu $t$ thuộc $T'$, ký hiệu $\lambda_t$ là ảnh của $\lambda'_t$ qua đơn ánh chính tắc của $X'$ vào $X$, và nếu $t$ thuộc $T - T'$ ta đặt $\lambda_t = 0$. Người đọc sẽ dễ dàng kiểm tra rằng ánh xạ $t \mapsto \lambda_t$ thỏa mãn các điều kiện a) và b) của mệnh đề.

C) *Tồn tại trong trường hợp tổng quát*:

Vì độ đo $\nu$ trên $X$ là điều hòa, ta có thể chọn một phủ $(U_m)_{m \in \mathbf{N}}$ của $X$ gồm các tập mở khả tích theo $\nu$. Ngoài ra, cho $(X_n)_{n \in \mathbf{N}}$ là một phân hoạch $\nu$ của $X$ sao cho hạn chế của $p$ trên mỗi tập $X_n$ là liên tục (§ 1, No. 8, Props. 10 and 11); ký hiệu $\nu_n$ là độ đo $\varphi_{X_n} \cdot \nu$ trên $X$ và $\mu_n$ là ảnh của nó qua $p$. Theo B), với mỗi số nguyên $n \in \mathbf{N}$, tồn tại một ánh xạ $t \mapsto \alpha^n_t$ của $T$ vào $\mathcal{M}_+(X)$ thỏa mãn các điều kiện sau:

$a'')$ Độ đo $\alpha^n_t$ được mang bởi $\overline{p}(t)$ với mọi $t \in T$.

$b'')$ Nếu $f$ là một hàm dương đo được phổ quát trên $X$, thì hàm dương $t \mapsto (\alpha^n_t)^*(f)$ trên $T$ là đo được phổ quát và

$$
\int_X f(x)\, d\nu_n(x) = \int_T d\mu_n(t) \int_X f(x)\, d\alpha^n_t(x).
$$

Ta có $\nu = \sum_{n \in \mathbf{N}} \nu_n$ và $\mu = \sum_{n \in \mathbf{N}} \mu_n$; từ Mệnh đề 3 của No. 2 và Bổ đề 4 ở trên, suy ra ngay lập tức rằng tồn tại một dãy $(g_n)_{n \in \mathbf{N}}$ các hàm dương đo được phổ quát trên $T$ sao cho $\mu_n = g_n \cdot \mu$ với mọi $n \in \mathbf{N}$ và sao cho $\sum_{n \in \mathbf{N}} g_n = 1$. Với mỗi $t \in T$, ký hiệu $\beta^n_t$ là độ đo $g_n(t) \cdot \alpha^n_t$ trên $X$ và $q_t$ là hàm phụ $\sum_{n \in \mathbf{N}} (\beta^n_t)^*$ trên $X$. Cho $f$ là một hàm dương đo được phổ quát trên $X$; sử dụng Mệnh đề 2 của No. 2 và lấy tổng theo $n$ trong (13), ta được

$$
\int_X f(x)\, d\nu(x) = \int_T q_t(f)\, d\mu(t);
$$

hơn nữa, rõ ràng là hàm $t \mapsto q_t(f)$ trên $T$ đo được phổ quát.

Với mọi $m \in \mathbf{N}$, gọi $E_m$ là tập hợp các $t \in T$ sao cho $q_t(U_m) = +\infty$; tập hợp $E_m$ đo được phổ quát vì điều này đúng đối với ánh xạ $t \mapsto q_t(U_m)$, và $E_m$ là không đáng kể địa phương đối với $\mu$ theo công thức (14) áp dụng cho $f = \varphi_{U_m}$, vì $\nu^*(U_m)$ là hữu hạn. Tập hợp $E = \bigcup_{m \in \mathbf{N}} E_m$ do đó đo được phổ quát và không đáng kể địa phương đối với $\mu$. Ta đặt $\lambda_t = 0$ với $t \in E$. Hơn nữa, cho $t \in T - E$; hàm tải $q_t$ bị chặn địa phương vì các tập mở $U_m$ phủ $X$ và vì $q_t(U_m)$ là hữu hạn; theo Mệnh đề 7 của § 1, No. 7, tồn tại một độ đo $\lambda_t$ trên $X$ sao cho $q_t = \lambda_t^*$ và $\lambda_t = \sum_{n \in \mathbf{N}} \beta^n_t$. Ngay lập tức, ánh xạ $t \mapsto \lambda_t$ thỏa mãn các điều kiện a) và b) của mệnh đề.

D) *Chứng minh c)*:
Cho $f$ là một hàm đo được phổ quát trên $X$, dương và bị chặn; ta sẽ chứng minh rằng hàm đo được phổ quát $h_f : t \mapsto \lambda_t^\bullet(f)$ trên $T$ là một mật độ của độ đo $\mu_f = p(f \cdot \nu)$ đối với $\mu = p(\nu)$. Cho $K$ là một tập con compact của $T$ và đặt $A = \overline{p}^{-1}(K)$. Với mọi $t \in T$, độ đo $\lambda_t$ tập trung trên $\overline{p}^{-1}(t)$; nếu $t$ thuộc $K$ thì $\overline{p}^{-1}(t) \subset A$, do đó $\lambda_t^\bullet(f \varphi_A) = \lambda_t^\bullet(f)$; ngược lại, nếu $t$ thuộc $T - K$ thì $\overline{p}^{-1}(t) \subset X - A$, do đó $\lambda_t^\bullet(f \varphi_A) = 0$. Áp dụng công thức (12) cho $f \cdot \varphi_A$,$^{(1)}$ ta được

$$
\mu_f(K) = \int_A^\bullet f(x)\, d\nu(x) = \int_K^\bullet d\mu(t) \int_X^\bullet f(x)\, d\lambda_t(x) = \int_K^\bullet h_f(t)\, d\mu(t),
$$

điều này thiết lập quan hệ $\mu_f = h_f \cdot \mu$.

Đặt $f = 1$, ta thấy rằng hàm $h_1 : t \mapsto \| \lambda_t \|$ là một mật độ của độ đo $\mu_1 = \mu$ đối với $\mu$, do đó bằng 1 hầu khắp nơi địa phương đối với $\mu$ trong $T$.

E) *Tính duy nhất*:
Cho $t \mapsto \lambda_t^i$ (với $i = 1, 2$) là hai ánh xạ của $T$ vào $\mathcal{M}_+(X)$ thỏa mãn các điều kiện a) và b) của mệnh đề. Như trong C), chọn một $(X_n)_{n \in \mathbf{N}}$ $\mu$-nghiền của $X$ sao cho $p_{X_n}$ liên tục với mọi $n \in \mathbf{N}$, và đặt $N = X - \bigcup_{n \in \mathbf{N}} X_n$. Với mọi số nguyên $n \in \mathbf{N}$, chọn một tập hợp đếm được $D_n$ các hàm dương trên $X$, bằng không bên ngoài $X_n$, mà các hạn chế của chúng lên $X_n$ tạo thành một tập hợp trù mật trong không gian định chuẩn $\mathcal{C}(X_n)$ (áp dụng Định lý 1 của GT, X, §3, No. 3 cho không gian compact mêtric hóa $X_n$). Ta đặt $D = \bigcup_{n \in \mathbf{N}} D_n$.

Cho $f \in D$; theo D), các hàm $t \mapsto (\lambda_t^1)^\bullet(f)$ và $t \mapsto (\lambda_t^2)^\bullet(f)$ là các mật độ của độ đo $\mu_f$ đối với $\mu$, và do đó tồn tại một tập hợp $E_f$ địa phương $\mu$-không đáng kể trong $T$ sao cho $(\lambda_t^1)^\bullet(f) = (\lambda_t^2)^\bullet(f)$ với $t \in T - E_f$. Hơn nữa, theo (12), tập hợp $F_i$ các $t \in T$ sao cho $(\lambda_t^i)^\bullet(N) \neq 0$ là địa phương $\mu$-không đáng kể với $i = 1, 2$. Vì $D$ là đếm được, tập hợp $G = (\bigcup_{f \in D} E_f) \cup F_1 \cup F_2$ là địa phương $\mu$-không đáng kể; với $t \in T - G$, ta có $(\lambda_t^1)^\bullet(N) = (\lambda_t^2)^\bullet(N) = 0$ và $(\lambda_t^1)_{X_n} = (\lambda_t^2)_{X_n}$, do đó $\lambda_t^1 = \lambda_t^2$ theo Mệnh đề 9 của §1, No. 8.

Q.E.D.

#### Nhận xét {#int-ix-s2-n7-rem-1 .statement}

— 1) Nếu $X$ là một không gian Souslin, thì mọi không gian con compact của $X$ đều là một không gian Souslin, do đó là mêtric hóa được (TG, IX, Phụ lục I, Hệ quả 2 của Mệnh đề 3),$^{(2)}$

(1) Trong trường hợp $f \cdot \varphi_A$ không đo được phổ quát, hãy sử dụng *Nhận xét 2*) dưới đây.
(2) Kết quả này không xuất hiện trong GT (xem chú thích cuối trang của *Nhận xét 1* của §1, No. 9).

và mọi độ đo trên X đều được điều hòa (§ 1, No. 9, Nhận xét 1). Theo Mệnh đề 13, mọi độ đo $\nu$ trên X do đó thừa nhận một phân rã đối với mọi ánh xạ $\nu$-thực sự.

2) Với các ký hiệu của Mệnh đề 13, cho $f$ là một hàm $\nu$-đo được dương. Có thể chứng minh, như trong Ch. V, § 3, No. 2, Mệnh đề 5, rằng tập hợp các $t \in T$ sao cho $f$ không $\lambda_t$-đo được là địa phương $\mu$-không đáng kể, rằng $t \mapsto \lambda_t^\bullet(f)$ là $\mu$-đo được, và rằng quan hệ (12) lại đúng.

### Bài tập {#int-ix-s2-exercises}

Xem các [bài tập cho § 2](exercises/s2/).
