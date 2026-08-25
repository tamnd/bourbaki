---
book: fvr
book_title: Functions of a Real Variable
chapter: II
chapter_title: PRIMITIVES AND INTEGRALS
section: 3
section_title: DERIVATIVES AND INTEGRALS OF FUNCTIONS DEPENDING ON A PARAMETER
lang: vi
source: fvr-i-vii
pdf_pages: 0083-0093, 0101-0105
extraction: ocr
subsections:
    - "no": 1
      title: INTEGRAL OF A LIMIT OF FUNCTIONS ON A COMPACT INTERVAL
      page: 0
      pdf_page: 83
    - "no": 2
      title: INTEGRAL OF A LIMIT OF FUNCTIONS ON A NON-COMPACT INTERVAL
      page: 0
      pdf_page: 84
    - "no": 3
      title: NORMALLY CONVERGENT INTEGRALS
      page: 0
      pdf_page: 87
    - "no": 4
      title: DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A COMPACT INTERVAL
      page: 0
      pdf_page: 88
    - "no": 5
      title: DERIVATIVE WITH RESPECT TO A PARAMETER OF AN INTEGRAL OVER A NON-COMPACT INTERVAL
      page: 0
      pdf_page: 90
    - "no": 6
      title: CHANGE OF ORDER OF INTEGRATION
      page: 0
      pdf_page: 91
statements: 17
exercises: 10
content_sha256: 9546936bea626722ef1defb300bf180078c7b29ccbe56245a5ed5d81cce979a3
translated_from: content/en/fvr/II/03_s3_derivatives_and_integrals_of_functions.md
source_content_sha256: 62bb6cd48dfc0b7f2b01d57475721e621137ba34388ad9ae689438f7ab394731
translation_model: gpt-5.4, copied
translation_run: translate-vi-8709dd68
glossary_version: 34
glossary_terms_sha256: 8d550981053815e9f0c0eb9dfef7c7f87c3bd95fd83835a9a053c952efe817e3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ĐẠO HÀM VÀ TÍCH PHÂN CỦA CÁC HÀM PHỤ THUỘC VÀO MỘT THAM SỐ

### 1. TÍCH PHÂN CỦA GIỚI HẠN CỦA CÁC HÀM TRÊN MỘT ĐOẠN COMPACT

Định lý 1 của II, p. 52, áp dụng cho trường hợp riêng của các hàm điều chỉnh trên một đoạn compact, được phát biểu như sau theo ký hiệu thích hợp cho tích phân:

#### Mệnh đề 1 {#fvr-ii-s3-prop-1 .statement}

Cho A là một tập hợp được lọc bởi một bộ lọc $\mathfrak{F}$, và $(f_\alpha)_{\alpha \in A}$ là một họ các hàm điều chỉnh trên một đoạn compact $I = [a, b]$; nếu các hàm $f_\alpha$ hội tụ đều trên I đến một hàm f (điều chỉnh) đối với bộ lọc $\mathfrak{F}$, thì

$$
\lim_{\mathfrak{F}} \int_a^b f_\alpha(t) \, dt = \int_a^b f(t) \, dt.
$$

Hai hệ quả của mệnh đề này là quan trọng trong các áp dụng:

#### Hệ quả 1 {#fvr-ii-s3-prop-1-cor-1 .statement}

Cho $(f_n)$ là một dãy các hàm điều chỉnh trên một đoạn compact $I = [a, b]$. Nếu dãy $(f_n)$ hội tụ đều trên I đến một hàm f (điều chỉnh), ta có

$$
\lim_{n \to \infty} \int_a^b f_n(t) \, dt = \int_a^b f(t) \, dt.
$$

Đặc biệt, nếu một chuỗi mà số hạng tổng quát $u_n$ là một hàm điều chỉnh trên I, hội tụ đều đến f trên I, thì chuỗi có số hạng tổng quát $\int_a^b u_n(t) \, dt$ là hội tụ và tổng của nó là $\int_a^b f(t) \, dt$ ("lấy tích phân từng số hạng của một chuỗi hội tụ đều").

#### Hệ quả 2 {#fvr-ii-s3-prop-1-cor-2 .statement}

Cho $A$ là một tập con của một không gian tôpô $F$, và $f$ là một ánh xạ từ $I \times A$ vào một không gian định chuẩn đầy đủ $E$ trên $\mathbf{R}$, sao cho, với mỗi $\alpha \in A$, hàm $x \mapsto f(x, \alpha)$ là điều hòa trên $I$. Nếu các hàm $x \mapsto f(x, \alpha)$ hội tụ đều trên $I$ tới một hàm (điều hòa) $x \mapsto g(x)$, khi $\alpha$ tiến tới một điểm $\alpha_0 \in \overline{A}$ mà vẫn nằm trong $A$, thì ta có

$$
\lim_{\alpha \to \alpha_0,\ \alpha \in A} \int_a^b f(x, \alpha)\, dx = \int_a^b g(x)\, dx.
$$

Đặc biệt:

#### Mệnh đề 2 ("tính liên tục của một nguyên đối với một tham số") {#fvr-ii-s3-prop-2 .statement}

Cho $F$ là một không gian compact, $I = [a,\ b]$ là một khoảng compact trong $\mathbf{R}$, và $f$ là một ánh xạ liên tục từ $I \times F$ vào một không gian định chuẩn đầy đủ $E$ trên $\mathbf{R}$; khi đó hàm $h(\alpha) = \int_a^b f(x, \alpha)\, dx$ liên tục trên $F$.

Thật vậy, vì $f$ liên tục đều trên không gian compắc $I \times F$, nên các hàm $f(x, \alpha)$ hội tụ đều tới $f(x, \alpha_0)$ trên $I$, khi $\alpha$ tiến tới một điểm tùy ý $\alpha_0 \in F$.

Sau đây là một ứng dụng của mệnh đề này: hàm $(x, \alpha) \mapsto x^\alpha$ liên tục trên tích $I \times J$, trong đó $I = [a,\ b]$ là một khoảng compắc sao cho $0 < a < b$, và $J$ là một khoảng compắc bất kỳ trong $\mathbf{R}$; suy ra rằng $\int_a^b x^\alpha\, dx$ là một hàm liên tục của $\alpha$ trên $\mathbf{R}$; bây giờ, với $\alpha$ hữu tỉ và $\neq -1$, hàm này bằng $\frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$, và hàm $\alpha \mapsto \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$ liên tục trên mọi khoảng của $\mathbf{R}$ không chứa $-1$; do đó ta có (mở rộng các đẳng thức) $\int_a^b x^\alpha\, dx = \frac{b^{\alpha+1} - a^{\alpha+1}}{\alpha + 1}$ với mọi $\alpha \neq -1$ thực; điều này lại có nghĩa là, với mọi $\alpha$ thực, đạo hàm của $x^\alpha$ là $\alpha x^{\alpha-1}$ (xem III, p. 94).

### 2. TÍCH PHÂN CỦA GIỚI HẠN CỦA CÁC HÀM SỐ TRÊN MỘT KHOẢNG KHÔNG COMPACT

Đl. 1 của II, p. 52 áp dụng cho những hàm số tổng quát hơn các hàm điều hòa, vì ở đó người ta chỉ giả thiết rằng các hàm số thừa nhận nguyên hàm. Đặc biệt, ta thấy rằng mệnh đề 1 của II, p. 68 vẫn còn áp dụng được khi, trên một khoảng $I \subset \mathbf{R}$, các hàm số $f_\alpha$ chỉ được giả thiết là *điều hòa từng khúc* và thừa nhận một *tích phân* trên $I$; tuy nhiên kết quả này giả thiết rằng hai giả thuyết kia của mệnh đề 1 được thỏa mãn, tức là:
1. $I$ là một *khoảng bị chặn*; 2' các $f_\alpha$ hội tụ *đều trên* $I$ tới $f$. Công thức (1) của II, p. 68 *có thể sai* khi một trong các điều kiện ấy không còn được thỏa mãn nữa: có thể xảy ra rằng một hoặc điều kia trong hai vế này không tồn tại, hoặc cả hai đều tồn tại nhưng có các giá trị khác nhau.

Ví dụ, nếu $f_n$ là hàm điều hòa trên $]0,\ 1[$, được xác định bởi $f_n(x) = n$ với $0 < x < 1/n$ và $f_n(x) = 0$ với $1/n \leq x \leq 1$, thì dãy $(f_n)$ hội tụ đều tới 0 trên mọi khoảng compact được chứa trong ]0, 1[, nhưng không hội tụ đều trên [0, 1], và ta có $\int_0^1 f_n(t) \, dt = 1$ với mọi $n$. Ta có một ví dụ trong đó $\int_0^1 f_n(t) \, dt$ không tiến tới một giới hạn nào khi thay thế dãy trước đó $(f_n)$ bằng dãy $((-1)^n f_n)$, dãy này lại cũng hội tụ đều tới 0 trên mọi khoảng compact được chứa trong ]0, 1].

Mặt khác, trên khoảng *không bị chặn* $I = [0, +\infty[$, cho $f_n$ là hàm điều tiết sao cho $f_n(x) = 1/n$ với $n^2 \leq x \leq (n+1)^2$ và $f_n(x) = 0$ với mọi giá trị khác của $x$ trong $I$ ($n \geq 1$); dãy $(f_n)$ hội tụ đều về 0 trên $I$, nhưng nguyên $\int_0^{+\infty} f_n(t) \, dt = (2n+1)/n$ tiến tới 2 khi $n$ tăng vô hạn.

Nói cách khác, khi $I$ không bị chặn, nếu ký hiệu bởi $\mathcal{I}$ không gian vectơ tạo bởi các hàm điều chỉnh $\mathbf{f}$ trên $I$, nhận giá trị trong $E$, và chấp nhận được một tích phân trên $I$, thì ánh xạ $\mathbf{f} \mapsto \int_I \mathbf{f}(t) \, dt$ *không liên tục* khi ta trang bị cho $\mathcal{I}$ tôpô hội tụ đều trên $I$ (*x.* II, p. 53, hệ quả 2)

Ta sẽ tìm các điều kiện *đủ* để bảo đảm tính đúng đắn của mệnh đề 1, dưới các giả thiết sau:

1. $I$ is an arbitrary interval in $\mathbf{R}$, the function $\mathbf{f}_\alpha$ is regulated on $I$, and admits an integral over $I$;
2. the family $(\mathbf{f}_\alpha)$ converges uniformly to $\mathbf{f}$ with respect to the filter $\mathfrak{F}$ on every compact interval contained in $I$.

Ký hiệu $\mathfrak{K}(I)$ là tập có hướng các khoảng compact được chứa trong $I$ (II, p. 64), vế trái của công thức (1) ở II, p. 68 có thể được viết là $\lim_{\delta} \left( \lim_{J \in \mathfrak{K}(I)} \int_J \mathbf{f}_\alpha(t) \, dt \right)$; mặt khác, có xét đến mệnh đề 1 (II. p. 68), và cả thực tế là họ $(\mathbf{f}_\alpha)$ hội tụ đều trên mọi khoảng compact $J \subset I$, vế phải của (1) (II, p. 68) có thể được viết là $\lim_{J \in \mathfrak{K}(I)} \left( \lim_{\delta} \int_J \mathbf{f}_\alpha(t) \, dt \right)$. Do đó thấy rằng mệnh đề 1 của II, p. 19 được mở rộng khi ta có thể *đổi chỗ các giới hạn* của ánh xạ$(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$ đối với bộ lọc $\mathfrak{F}$ và đối với bộ lọc $\Phi$ của các thiết diện của tập có hướng $\mathfrak{K}(I)$. Nay, ta biết một điều kiện *đủ* để việc đổi chỗ này là chính đáng, tức là sự tồn tại của giới hạn của ánh xạ $(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$ đối với *bộ lọc tích* $\Phi \times \mathfrak{F}$ (*Gen. Top.*, I, p. 81, hệ quả của đ. lý 1). Ta sẽ biến đổi điều kiện này thành một điều kiện tương đương, dễ xử lý hơn.

Trước hết, vì $E$ là đầy đủ, để cho $(J, \alpha) \mapsto \int_J \mathbf{f}_\alpha(t) \, dt$ có một giới hạn đối với $\Phi \times \mathfrak{F}$ thì điều kiện cần và đủ là, với mọi $\varepsilon > 0$, tồn tại một khoảng compact $J_0 \subset I$ và một tập hợp $M \in \mathfrak{F}$ sao cho, với mọi phần tử $\alpha, \beta$ của $M$ và mọi khoảng compact $J \supset J_0$ được chứa trong $I$, ta có

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t) \, dt - \int_J \mathbf{f}_\beta(t) \, dt \right| \leq \varepsilon.
$$

Mặt khác, ta sẽ chỉ ra rằng điều kiện này tự nó tương đương với điều kiện sau: với mọi $\varepsilon > 0$ tồn tại một khoảng compact $J_0 \subset I$ và một tập hợp $M \in \mathfrak{F}$ sao cho, với mọi $\alpha$ của $M$ và mọi khoảng compact $J \supset J_0$ được chứa trong $I$, ta có

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t) \, dt - \int_J \mathbf{f}_\alpha(t) \, dt \right| \leq \varepsilon.
$$

Quả thật hiển nhiên là điều kiện sau cùng này là cần thiết; ngược lại, nếu nó được thỏa mãn, thì tồn tại (do sự hội tụ đều của $(\mathbf{f}_\alpha )$ trên mọi khoảng compact) một tập hợp $N \in \mathfrak{F}$ sao cho, với mọi $\alpha,\ \beta$ trong $N$ ta có

$$
\left| \int_{J_0} \mathbf{f}_\alpha(t)\,dt - \int_{J_0} \mathbf{f}_\beta(t)\,dt \right| \leq \varepsilon;
$$

và do đó $\left| \int_{J_0} \mathbf{f}_\alpha(t)\,dt - \int_J \mathbf{f}_\beta(t)\,dt \right| \leq 2\varepsilon$ với mọi $\alpha$ và $\beta$ trong $M \cap N \in \mathfrak{F}$ và với mọi khoảng compact $J \supset J_0$.

Sau cùng, bổ đề ở II, p. 65 cho phép ta viết điều kiện cuối cùng này dưới dạng tương đương sau đây: *với mọi $\varepsilon > 0$ tồn tại một khoảng compact $J_0 \subset I$ và một tập hợp $M \in \mathfrak{F}$ (phụ thuộc vào $\varepsilon$) sao cho, với mọi khoảng compact $K \subset I$ không có điểm trong nào chung với $J_0$, và mọi $\alpha \in M$, ta có* $\left| \int_K \mathbf{f}_\alpha(t)\,dt \right| \leq \varepsilon$.

Thông thường nhất, người ta dùng một điều kiện chặt hơn thu được bằng cách giả sử rằng, trong mệnh đề sau cùng, tập hợp $M$ *không phụ thuộc vào $\varepsilon$*:

#### Định nghĩa 1 {#fvr-ii-s3-def-1 .statement}

*Người ta nói rằng tích phân $\int_I \mathbf{f}_\alpha(t)\,dt$ hội tụ đều đối với $\alpha \in A$ (hay hội tụ đều trên $A$) nếu, với mọi $\varepsilon > 0$ tồn tại một khoảng compact $J_0 \subset J$ sao cho, với mọi khoảng compact $K \subset I$ không có điểm trong nào chung với $J_0$, và mọi $\alpha \in A$, ta có*

$$
\left| \int_K \mathbf{f}_\alpha(t)\,dt \right| \leq \varepsilon.
$$

Định nghĩa này tương đương với việc nói rằng họ các ánh xạ $\alpha \mapsto \int_I \mathbf{f}_\alpha(t)\,dt$ *hội tụ đều trên $A$* (về ánh xạ $\alpha \mapsto \int_I \mathbf{f}_\alpha(t)\,dt$) đối với bộ lọc các thiết diện $\Phi$ của $\mathcal{K}(I)$; mỗi một trong các tích phân $\int_I \mathbf{f}_\alpha(t)\,dt$ *a fortiori* là hội tụ (đảo lại là sai). Hơn nữa, từ điều ta vừa thấy (hoặc từ *Gen. Top.*, X, p. 281, hệ quả 2):

#### Mệnh đề 3 {#fvr-ii-s3-prop-3 .statement}

*Cho* $(\mathbf{f}_\alpha )$ *là một họ các hàm điều hòa trên một khoảng* $I$ *sao cho: 1* đối với bộ lọc $\mathfrak{F}$ *họ* $(\mathbf{f}_\alpha )$ *hội tụ đều đến một hàm* $f$ *(điều hòa trên* $I$) *trên mọi khoảng compact được chứa trong* $I$; *2* tích phân $\int_I \mathbf{f}_\alpha(t)\,dt$ *hội tụ đều theo* $\alpha \in A$. *Dưới các giả thiết đó, tích phân* $\int_I f(t)\,dt$ *hội tụ, và ta có*

$$
\lim_{\mathfrak{F}} \int_I \mathbf{f}_\alpha(t)\,dt = \int_I f(t)\,dt.
$$

Các giả thiết của mệnh đề 3 được thỏa mãn chẳng hạn khi $I$ là một khoảng *bị chặn*, các $\mathbf{f}_\alpha$ là *bị chặn đều* trên $I$, và hội tụ đều đến $f$ trên mọi khoảng compact được chứa trong $I$; thật vậy, nếu $\| \mathbf{f}_\alpha(x) \| \leq h$ với mọi $x \in I$ và mọi $\alpha$, và nếu $J_0$ sao cho hiệu giữa độ dài của $I$ và $J_0$ là $\leq \varepsilon / h$, thì điều kiện (7) được thỏa mãn đối với mọi khoảng $K \subset I$ không có điểm trong nào chung với $J_0$.

Cũng như đối với mệnh đề 1 của II, p. 68, hai hệ quả của mệnh đề 3 là quan trọng trong các ứng dụng:

#### Hệ quả 1 {#fvr-ii-s3-prop-3-cor-1 .statement}

*Cho* $(f_n)$ *là một dãy các hàm điều chỉnh trên một khoảng tùy ý* $I$, *hội tụ đều về một hàm* $f$ *trên mỗi khoảng compắc được chứa trong* $I$; *nếu tích phân* $\int_I f_n(t)\,dt$ *hội tụ đều, thì tích phân* $\int_I f(t)\,dt$ *hội tụ, và*
$$
\lim_{n \to \infty} \int_I f_n(t)\,dt = \int_I f(t)\,dt.
$$
(9)

#### Nhận xét {#fvr-ii-s3-n2-rem-1 .statement}

Các giả thiết đặt ra trong hệ quả này là đủ, nhưng không cần, để công thức (9) đúng; về sau chúng tôi sẽ tổng quát hóa công thức này, đồng thời với khái niệm tích phân (xem INT, IV), và thu được những điều kiện ít hạn chế hơn nhiều.

#### Hệ quả 2 {#fvr-ii-s3-prop-3-cor-2 .statement}

*Cho* $A$ *là một tập con của một không gian tôpô* $F$, *và* $f$ *là một ánh xạ từ* $I \times A$ *vào một không gian định chuẩn đầy đủ* $E$ *trên* $\mathbf{R}$, *sao cho, với mọi* $\alpha \in A$, *hàm* $x \mapsto f(x, \alpha)$ *là điều hòa trên* $I$. *Nếu, một mặt, các hàm* $x \mapsto f(x, \alpha)$ *hội tụ đều trên mọi khoảng compact được chứa trong* $I$ *đến một hàm* $x \mapsto f(x)$ *khi* $\alpha$ *tiến tới* $\alpha_0 \in \overline{A}$ *trong khi vẫn thuộc* $A$; *nếu, mặt khác, tích phân* $\int_I f(x, \alpha)\,dx$ *hội tụ đều trên* $A$, *thì tích phân* $\int_I f(x)\,dx$ *hội tụ, và ta có*
$$
\lim_{\alpha \to \alpha_0,\ \alpha \in A} \int_I f(x, \alpha)\,dx = \int_I f(x)\,dx.
$$
(10)

Đặc biệt:

#### Mệnh đề 4 ("tính liên tục của một nguyên suy rộng đối với một tham số") {#fvr-ii-s3-prop-4 .statement}

*Cho* $F$ *là một không gian compact, cho* $I$ *là một khoảng bất kỳ trong* $\mathbf{R}$, *và* $f$ *là một ánh xạ liên tục từ* $I \times F$ *vào một không gian định chuẩn đầy đủ* $E$ *trên* $\mathbf{R}$; *nếu nguyên* $h(\alpha) = \int_I f(x, \alpha)\,dx$ *hội tụ đều trên* $F$ *thì nó là một hàm liên tục theo* $\alpha$ *trên* $F$.

Xét đến mệnh đề 2 của II, p. 69, mệnh đề này cũng suy ra từ tính liên tục của một giới hạn đều của các hàm liên tục (*Gen. Top.*, X, p. 282, định lý 2).

### 3. CÁC NGUYÊN HỘI TỤ CHUẨN TẮC

Cho $(f_\alpha)_{\alpha \in A}$ là một họ các hàm điều hòa trên một khoảng tùy ý $I \subset \mathbf{R}$, nhận giá trị trong một không gian định chuẩn đầy đủ $E$ trên $\mathbf{R}$. Giả sử tồn tại một hàm điều hòa thực hữu hạn $g$ trên $I$ sao cho, với mọi $x \in I$ và mọi $\alpha \in A$, $\|f_\alpha(x)\| \leq g(x)$ và đồng thời tích phân $\int_I g(t)\,dt$ hội tụ. Trong các điều kiện ấy, tích phân $\int_I f_\alpha(t)\,dt$ là *hội tụ tuyệt đối và đều* trên $A$; thực vậy, với mọi khoảng compact $K$ được chứa trong $I$,
$$
\left\| \int_K f_\alpha(t)\,dt \right\| \leq \int_K g(t)\,dt
$$

và sự hội tụ của tích phân $\int_I g(t) \, dt$ kéo theo rằng với mọi $\varepsilon > 0$ tồn tại một khoảng compact $J \subset I$ sao cho với mọi khoảng compact $K \subset I$ rời nhau với $J$ ta có $\int_K g(t) \, dt \leq \varepsilon$. Khi tồn tại một hàm thực $g$ có các tính chất nói trên, người ta nói rằng tích phân $\int_I f_\alpha(t) \, dt$ hội tụ chuẩn tắc trên $A$ (xem Gen. Top., X, p. 296).

Một tích phân có thể hội tụ đều trên $A$ mà không hội tụ chuẩn. *Điều này xảy ra đối với dãy $(f_n)$ các hàm thực được xác định bởi các điều kiện $f_n(x) = 1/x$ với $n \leq x \leq n+1$, và $f_n(x) = 0$ với các giá trị khác của $x$ trong $I = [0, +\infty[$. Ngay lập tức thấy rằng tích phân $\int_1^\infty f_n(t) \, dt$ hội tụ đều, nhưng không hội tụ chuẩn, vì quan hệ $g(x) \geq f_n(x)$ với mỗi $x \in I$ và mọi $n$ kéo theo $g(x) \geq 1/x$, và do đó tích phân của $g$ trên $I$ không hội tụ..*

Đặc biệt, hãy xét một chuỗi mà số hạng tổng quát $u_n$ là một hàm điều chỉnh trên một khoảng $I$, và giả sử rằng chuỗi có số hạng tổng quát $\|u_n(x)\|$ (là một hàm điều chỉnh trên $I$) hội tụ đều trên mọi khoảng compắc được chứa trong $I$, và sao cho chuỗi có số hạng tổng quát $\int_I \|u_n(t)\| \, dt$ là hội tụ; khi đó (II, p. 66, prop. 2) hàm (điều chỉnh) $g(x)$, là tổng của chuỗi có số hạng tổng quát $\|u_n(x)\|$, có tính chất là tích phân $\int_I g(t) \, dt$ hội tụ. Nếu đặt $f_n = \sum_{p=1}^n u_p$, thì tích phân $\int_I f_n(t) \, dt$ hội tụ chuẩn tắc, vì ta có

$$
\|f_n(x)\| \leq \sum_{p=1}^n \|u_p(x)\| \leq g(x)
$$

với mọi $x \in I$ và mọi $n$; hệ quả là, tổng $f$ của chuỗi có số hạng tổng quát $u_n$ là một hàm điều tiết trên $I$ sao cho nguyên $\int_I f(t) \, dt$ hội tụ, và ta có

$$
\int_I f(t) \, dt = \sum_{n=1}^\infty \int_I u_n(t) \, dt
$$

("lấy nguyên từng số hạng của một chuỗi trên một khoảng không compắc").

### 4. ĐẠO HÀM THEO MỘT THAM SỐ CỦA MỘT NGUYÊN TRÊN MỘT KHOẢNG COMPACT

Cho $A$ là một lân cận compact của một điểm $\alpha_0$ trong trường $\mathbf{R}$ (hoặc trường $\mathbf{C}$), cho $I = [a, b]$ là một khoảng compact trong $\mathbf{R}$, và $f$ là một ánh xạ liên tục từ $I \times A$ vào một không gian định chuẩn đầy đủ $E$ trên $\mathbf{R}$ (hoặc $\mathbf{C}$). Ta đã thấy (II, p. 69, prop. 2) rằng dưới những điều kiện ấy $g(\alpha) = \int_a^b f(t, \alpha) \, dt$ là một hàm liên tục trên $A$. Hãy tìm các điều kiện đủ để $g$ có đạo hàm tại điểm $\alpha_0$. Ta có, với $\alpha \neq \alpha_0$,

$$
\frac{g(\alpha) - g(\alpha_0)}{\alpha - \alpha_0} = \int_a^b \frac{f(t, \alpha) - f(t, \alpha_0)}{\alpha - \alpha_0} \, dt
$$

vì vậy (II, p. 69, cor. 2), nếu các hàm $x \mapsto \frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ hội tụ đều trên I đến một hàm $x \mapsto \mathbf{h}(x)$ (tất yếu liên tục) khi $\alpha$ tiến tới $\alpha_0$ (trong khi vẫn $\neq \alpha_0$), thì $g$ có đạo hàm bằng $\int_a^b \mathbf{h}(t)\,dt$ tại điểm $\alpha_0$; hơn nữa, với mỗi $x \in I$, $\frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ tiến tới $\mathbf{h}(x)$, nên $\mathbf{h}(x)$ là đạo hàm tại điểm $\alpha_0$ của ánh xạ $\alpha \mapsto \mathbf{f}(x, \alpha)$; ta ký hiệu đạo hàm này (gọi là *đạo hàm riêng của* $\mathbf{f}$ *đối với* $\alpha$) bằng ký hiệu $\mathbf{f}'_{\alpha}(x, \alpha_0)$; các giả thiết mà ta đã đặt ra kéo theo rằng

$$
g'(\alpha_0) = \int_a^b \mathbf{f}'_{\alpha}(t, \alpha_0)\,dt.
$$

(12)

Mệnh đề sau đây cho một điều kiện đủ rất đơn giản để công thức (12) đúng:

#### Mệnh đề 5 {#fvr-ii-s3-prop-5 .statement}

*Giả sử rằng đạo hàm riêng* $\mathbf{f}'_{\alpha}(x, \alpha)$ *tồn tại với mọi* $x \in I$ *và mọi* $\alpha$ *trong một lân cận mở* $V$ *của* $\alpha_0$, *và rằng, với mọi* $\alpha \in V$, *ánh xạ* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ *là bị chặn điều hòa trên* $I$. *Trong các điều kiện ấy, nếu* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ *hội tụ đều trên* $I$ *về* $x \mapsto \mathbf{f}'_{\alpha}(x, \alpha_0)$ *khi* $\alpha$ *tiến tới* $\alpha_0$, *thì hàm* $g(\alpha) = \int_a^b \mathbf{f}(t, \alpha)\,dt$ *có đạo hàm, được cho bởi công thức* (12), *tại điểm* $\alpha_0$.

Thật vậy, với mọi $\varepsilon > 0$ theo giả thiết tồn tại một $r > 0$ sao cho $|\alpha - \alpha_0| \leq r$ kéo theo $\| \mathbf{f}'_{\alpha}(x, \alpha) - \mathbf{f}'_{\alpha}(x, \alpha_0) \| \leq \varepsilon$ *với mọi* $x \in I$. Theo các mệnh đề 3 và 5 của I, p. 17, ta có, với $|\alpha - \alpha_0| \leq r$ ($\alpha \neq \alpha_0$) và với mọi $x \in I$

$$
\left\| \frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0} - \mathbf{f}'_{\alpha}(x, \alpha_0) \right\| \leq \varepsilon
$$

điều đó chứng minh sự hội tụ đều của $\frac{\mathbf{f}(x, \alpha) - \mathbf{f}(x, \alpha_0)}{\alpha - \alpha_0}$ về $\mathbf{f}'_{\alpha}(x, \alpha_0)$ trên I khi $\alpha$ tiến tới $\alpha_0$ (vẫn $\neq \alpha_0$), và do đó thiết lập công thức (12).

#### Hệ quả {#fvr-ii-s3-n4-cor-1 .statement}

*Nếu đạo hàm riêng* $\mathbf{f}'_{\alpha}(x, \alpha)$ *tồn tại trên* $I \times V$ *và là một hàm liên tục theo* $(x, \alpha)$ *trên tập hợp này, thì hàm* $g$ *có đạo hàm cho bởi công thức* (12) *tại điểm* $\alpha_0$.

Thật vậy, nếu W là một lân cận compact của $\alpha_0$ được chứa trong V, thì ánh xạ $(x, \alpha) \mapsto \mathbf{f}'_{\alpha}(x, \alpha)$ là *liên tục đều* trên tập compact $I \times W$, nên $\mathbf{f}'_{\alpha}(x, \alpha)$ hội tụ tới $\mathbf{f}'_{\alpha}(x, \alpha_0)$ một cách đều trên I khi $\alpha$ tiến tới $\alpha_0$.

Từ mệnh đề 5 suy ra một mệnh đề tổng quát hơn cho phép tính đạo hàm của một tích phân khi không những hàm dưới dấu tích phân $\mathbf{f}$, mà cả các cận lấy tích phân, đều phụ thuộc vào một tham số $\alpha$:

#### Mệnh đề 6 {#fvr-ii-s3-prop-6 .statement}

*Giả sử các giả thiết của mệnh đề 5 được thỏa mãn, và gọi* $a(\alpha)$, $b(\alpha)$ *là hai hàm xác định trên* $V$, *nhận giá trị trong* $I$; *nếu các đạo hàm* $a'(\alpha_0),\ b'(\alpha_0)$ *tồn tại và hữu hạn thì hàm* $g(\alpha) = \int_{a(\alpha)}^{b(\alpha)} f(t, \alpha)\, dt$ *có tại* $\alpha_0$ *một đạo hàm được cho bởi công thức*

$$
g'(\alpha_0) = \int_{a(\alpha_0)}^{b(\alpha_0)} f'_\alpha(t, \alpha_0)\, dt + b'(\alpha_0)f(b(\alpha_0), \alpha_0) - a'(\alpha_0)f(a(\alpha_0), \alpha_0).
$$

Thật vậy, với mọi $\alpha \in V$ phân biệt với $\alpha_0$ ta có thể viết

$$
\frac{g(\alpha) - g(\alpha_0)}{\alpha - \alpha_0} = \int_{a(\alpha_0)}^{b(\alpha_0)} \frac{f(t, \alpha) - f(t, \alpha_0)}{\alpha - \alpha_0}\, dt + \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt
$$
$$
- \frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} f(t, \alpha)\, dt.
$$

Theo mệnh đề 5 của II, p. 74, tích phân thứ nhất ở vế phải tiến tới $\int_{a(\alpha_0)}^{b(\alpha_0)} f'_\alpha(t, \alpha_0)\, dt$ khi $\alpha$ tiến tới $\alpha_0$. Trong tích phân thứ hai, ta thay thế $f(t, \alpha)$ bằng $f(b(\alpha_0), \alpha_0)$ và chứng minh rằng hiệu số tiến tới 0. Đặt $M = \max (\|f(b(\alpha_0), \alpha_0)\|, |b'(\alpha_0)| + 1)$; do hàm $b(\alpha)$ liên tục tại điểm $\alpha_0$ và hàm $f$ liên tục tại điểm $(b(\alpha_0), \alpha_0)$, với mọi $\varepsilon$ sao cho $0 < \varepsilon < 1$ tồn tại một $r > 0$ sao cho quan hệ $|\alpha - \alpha_0| \leq r$ kéo theo $\|f(t, \alpha) - f(b(\alpha_0), \alpha_0)\| \leq \varepsilon$ với mọi $t$ thuộc khoảng có các đầu mút là $b(\alpha_0)$ và $b(\alpha)$; do đó cũng có thể giả sử rằng quan hệ $|\alpha - \alpha_0| \leq r$ kéo theo $\left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} - b'(\alpha_0) \right| \leq \varepsilon$.

Theo công thức giá trị trung bình (II, p 62, công thức (17)), do đó ta có

$$
\left| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt - \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} f(b(\alpha_0), \alpha_0) \right| \leq \left| \frac{b(\alpha) - b(\alpha_0)}{\alpha - \alpha_0} \right| \varepsilon
$$

và do đó

$$
\left| \frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt - b'(\alpha_0) f(b(\alpha_0), \alpha_0) \right| \leq 2M \varepsilon
$$

điều đó cho thấy rằng $\frac{1}{\alpha - \alpha_0} \int_{b(\alpha_0)}^{b(\alpha)} f(t, \alpha)\, dt$ tiến tới $b'(\alpha_0) f(b(\alpha_0), \alpha_0)$. Tương tự, ta chứng minh được rằng $\frac{1}{\alpha - \alpha_0} \int_{a(\alpha_0)}^{a(\alpha)} f(t, \alpha)\, dt$ tiến tới $a'(\alpha_0) f(a(\alpha_0), \alpha_0)$.

### 5. ĐẠO HÀM THEO MỘT THAM SỐ CỦA MỘT TÍCH PHÂN TRÊN MỘT KHOẢNG KHÔNG COMPACT

Tập hợp $V$ có cùng nghĩa như trong mệnh đề 5 của II, p. 74, bây giờ giả sử rằng I là *một khoảng bất kỳ* trong $\mathbf{R}$, và $f$ là một ánh xạ *liên tục* từ $I \times V$ vào E; nếu nguyên $g(\alpha) = \int_I f(t, \alpha)\, dt$ tồn tại với mọi $\alpha \in V$ và là một hàm liên tục theo $\alpha$, thì hàm $g$ *không nhất thiết có đạo hàm bằng* $\int_I f'_\alpha(t, \alpha_0)\, dt$ *tại điểm* $\alpha_0$, ngay cả khi $f'_\alpha(x, \alpha)$ hội tụ đều tới $f'_\alpha(x, \alpha_0)$ trên mọi khoảng compắc được chứa trong I, và nếu nguyên $\int_I f'_\alpha(t, \alpha) \, dt$ tồn tại với mọi $\alpha \in V$ (xem II, p. 87, bài tập 3).

Một điều kiện đủ để công thức (12) (II, p. 74) vẫn đúng được cho bởi mệnh đề sau:

#### Mệnh đề 7 {#fvr-ii-s3-prop-7 .statement}

Cho I là một khoảng tùy ý trong $\mathbf{R}$, và $f$ là một hàm liên tục trên $I \times V$. Giả sử rằng:
1. đạo hàm riêng $f'_\alpha(x, \alpha)$ tồn tại với mọi $x \in I$ và mọi $\alpha \in V$, và, với mọi $\alpha \in V$, ánh xạ $x \mapsto f'_\alpha(x, \alpha)$ là bị chặn điều hòa trên I;
2. với mọi $\alpha \in V$, $f'_\alpha(x, \beta)$ hội tụ đều tới $f'_\alpha(x, \alpha)$ trên mọi khoảng compắc được chứa trong I, khi $\beta$ tiến tới $\alpha$;
3. tích phân $\int_I f'_\alpha(t, \alpha) \, dt$ hội tụ đều trên $V$;
4. tích phân $\int_I f(t, \alpha_0) \, dt$ hội tụ.

Trong những điều kiện đó, nguyên $g(\alpha) = \int_I f(t, \alpha) \, dt$ hội tụ đều trên $V$, và hàm $g$ có tại mọi điểm của $V$ một đạo hàm được cho bởi công thức

$$
g'(\alpha) = \int_I f'_\alpha(t, \alpha) \, dt.
$$

Sự hội tụ đều của $\int_I f'_\alpha(t, \alpha) \, dt$ trên $V$ có nghĩa là hàm $\alpha \mapsto \int_J f'_\alpha(t, \alpha) \, dt$ hội tụ đều trên $V$ đối với bộ lọc các thiết diện $\Phi$ của tập có hướng $\mathfrak{K}(I)$ gồm các khoảng compact $J$ được chứa trong I. Đặt $u_J(\alpha) = \int_J f(t, \alpha) \, dt$; các giả thiết cho thấy một mặt $u_J(\alpha_0)$ có một giới hạn đối với $\Phi$, và mặt khác, theo mệnh đề 5 của II, p. 74, rằng $u'_J(\alpha) = \int_J f'_\alpha(t, \alpha) \, dt$ với mọi $\alpha \in V$. Vì vậy ta có thể áp dụng định lý 1 của II, p. 52 cho các hàm $u_J$, trong đó vai trò của tập hợp chỉ số ở đây do $\mathfrak{K}(I)$ đảm nhiệm, và vai trò của bộ lọc trên tập hợp này do bộ lọc $\Phi$ đảm nhiệm; mệnh đề được suy ra ngay lập tức.

#### Nhận xét 1 {#fvr-ii-s3-n5-rem-1 .statement}

Các điều kiện 1 và 2 của mệnh đề 7 được thỏa mãn a fortiori khi $f'_\alpha(x, \alpha)$ là một hàm liên tục của $(x, \alpha)$ trên $I \times V$.
2) Khi, trong một tích phân $\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt$, các đầu mút của khoảng là các hàm hữu hạn của tham số, việc nghiên cứu tích phân này như một hàm của $\alpha$ có thể liên quan đến việc nghiên cứu một tích phân trên $[0, 1]$; thật vậy, với phép thay đổi biến $t = a(\alpha)(1 - u) + b(\alpha)u$, ta có

$$
\int_{a(\alpha)}^{b(\alpha)} f(t, \alpha) \, dt = \int_0^1 f(a(\alpha)(1 - u) + b(\alpha)u, \alpha) (b(\alpha) - a(\alpha)) \, du.
$$

### 6. THAY ĐỔI THỨ TỰ TÍCH PHÂN

Cho $I = [a, b]$ và $A = [c, d]$ là hai khoảng compắc trong $\mathbf{R}$; cho $f$ là một hàm liên tục trên $I \times A$ nhận giá trị trong một không gian định chuẩn đầy đủ E trên $\mathbf{R}$; theo mệnh đề 2 của II, p. 69, $\int_a^b f(x, \alpha) \, dx$ là một hàm liên tục của $\alpha$ trên $A$; tích phân của nó $\int_c^d \left( \int_a^b f(x, \alpha) \, dx \right) d\alpha$ cũng được ký hiệu, để đơn giản, bởi $\int_c^d d\alpha \int_a^b f(x, \alpha) \, dx$.

#### Mệnh đề 8 {#fvr-ii-s3-prop-8 .statement}

*Nếu f liên tục trên I × A thì ta có*

$$
\int_c^d d\alpha \int_a^b f(x, \alpha) dx = \int_a^b dx \int_c^d f(x, \alpha) d\alpha
$$

("công thức đổi chỗ cấp tích phân").

Chúng ta sẽ chỉ ra rằng, với mọi $y \in A$, ta có

$$
\int_c^y d\alpha \int_a^b f(x, \alpha) dx = \int_a^b dx \int_c^y f(x, \alpha) d\alpha.
$$

Vì hai vế của (16) là các hàm của $y$, và bằng nhau tại $y = c$, nên chỉ cần chứng minh rằng chúng khả vi trên $]c, d[$ và các đạo hàm của chúng bằng nhau tại mọi điểm của khoảng này. Nếu đặt $g(\alpha) = \int_a^b f(x, \alpha) dx$, và $h(x, y) = \int_c^y f(x, \alpha) dx$, thì quan hệ (16) có thể viết thành

$$
\int_c^y g(\alpha) d\alpha = \int_a^b h(x, y) dx.
$$

Bây giờ, đạo hàm của số hạng thứ nhất đối với $y$ là $g(y)$, còn đạo hàm của số hạng thứ hai là $\int_a^b h_y'(x, y) dx$, theo II, p. 74, hệ quả, vì $h_y'(x, y) = f(x, y)$ liên tục trên $I \times A$; do đó hai biểu thức thu được là đồng nhất.

Giả sử bây giờ $A = [c, d]$ là một khoảng *compact* trong $\mathbf{R}$, và I là một khoảng *tùy ý* trong $\mathbf{R}$; giả sử $f$ là một hàm liên tục trên $I \times A$, nhận giá trị trong E, sao cho nguyên hàm $g(\alpha) = \int_I f(t, \alpha) dt$ hội tụ với mọi $\alpha \in A$; ngay cả khi $g(\alpha)$ liên tục trên $A$ thì người ta cũng không phải lúc nào cũng có thể đổi thứ tự lấy tích phân trong nguyên hàm $\int_c^d d\alpha \int_I f(t, \alpha) dt$, vì nguyên hàm $\int_I dt \int_c^d f(t, \alpha) d\alpha$ có thể không tồn tại, hoặc có thể khác với nguyên hàm $\int_c^d d\alpha \int_I f(t, \alpha) dt$ (*xem* II, p. 87, exerc. 7). Tuy nhiên, ta có kết quả sau:

#### Mệnh đề 9 {#fvr-ii-s3-prop-9 .statement}

*Nếu hàm f liên tục trên I × A, và nếu nguyên hàm $\int_I f(t, \alpha) dt$ hội tụ đều trên A, thì nguyên hàm $\int_I dt \int_c^d f(t, \alpha) d\alpha$ hội tụ, và ta có*

$$
\int_c^d d\alpha \int_I f(t, \alpha) dt = \int_I dt \int_c^d f(t, \alpha) d\alpha.
$$

Với mọi khoảng compắc J được chứa trong I, đặt $u_J(\alpha) = \int_J f(t, \alpha) dt$. Giả thiết kéo theo rằng đối với bộ lọc các thiết diện $\Phi$ của tập có hướng $\mathcal{K}(I)$ thì hàm liên tục $u_J$ hội tụ đều trên A tới $\int_I f(t, \alpha) dt$; do đó (II, p. 68, prop. 1), $\int_c^d d\alpha \int_J f(t, \alpha) dt$ có giới hạn $\int_c^d d\alpha \int_I f(t, \alpha) dt$ đối với $\Phi$; nhưng, theo mệnh đề 8 (II, p. 77), ta có

$$
\int_c^d d\alpha \int_J f(t, \alpha) dt = \int_J dt \int_c^d f(t, \alpha) d\alpha.
$$

Kết quả trước đó vì thế có nghĩa là tích phân $\int_1 dt \int_c^{d} f(t, \alpha) d\alpha$ là hội tụ, và khi chuyển qua giới hạn đối với $\Phi$ trong quan hệ (18), ta thu được (17).

### Bài tập {#fvr-ii-s3-exercises}

Xem [bài tập của § 3](exercises/s3/).
