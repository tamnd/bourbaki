---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 6
section_title: Images of a measure
lang: vi
source: int-i-vi
book_pages: INT V.62-INT V.74, INT V.107-INT V.112
pdf_pages: 0317-0329, 0362-0367
extraction: ocr
subsections:
    - "no": 1
      title: Image of a positive measure
      page: 62
      pdf_page: 317
    - "no": 2
      title: Integration with respect to the image of a positive measure
      page: 64
      pdf_page: 319
    - "no": 3
      title: Properties of the image of a positive measure
      page: 65
      pdf_page: 320
    - "no": 4
      title: Image of a complex measure
      page: 68
      pdf_page: 323
    - "no": 5
      title: 'Application: change of variable in the Lebesgue integral'
      page: 69
      pdf_page: 324
    - "no": 6
      title: Decomposition into slices. Inverse image of a measure under a local homeomorphism
      page: 71
      pdf_page: 326
statements: 29
exercises: 22
content_sha256: 708db2f6a2a0023330296f34858ea0baafd4263b7209e5997e0fea78431974e4
translated_from: content/en/int/V/06_s6_images_of_a_measure.md
source_content_sha256: 73962a5c4cf064782750832647a7c8af054354b0c2d06dc9e0217cee3b249fec
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-469b03b9
glossary_version: 34
glossary_terms_sha256: e2a99cde39cd70130b211d25a6c8a2b91cdfac59234a9da99df039730159ad7e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. ẢNH CỦA MỘT ĐỘ ĐO

### 1. Ảnh của một độ đo dương

Cho $ X $ là một không gian compact địa phương, $ \pi $ là một ánh xạ $ \mu $-đo được từ $ T $ vào $ X $. Nói rằng cặp $ (\pi, 1) $ là *$ \mu $-thích nghi* (§4, No. 1) tương đương với việc nói rằng đối với mọi hàm $ f \in \mathcal{K}(X) $, hàm $ f \circ \pi $ là *$ \mu $-khả tích về bản chất*.

#### Mệnh đề 1 {#int-v-s6-prop-1 .statement}

*Cho $ \pi $ là một ánh xạ $ \mu $-đo được của $ T $ vào một không gian compact địa phương $ X $. Hai tính chất sau là tương đương:*

a) *đối với mọi hàm* $ f \in \mathcal{K}(X) $, $ f \circ \pi $ *là* $ \mu $-*khả tích về bản chất*.

b) *đối với mọi tập compact* $ K \subset X $, $ \overline{\pi}^{-1}(K) $ *là* $ \mu $-*khả tích về bản chất*.

Ta đã nhận thấy rằng a) kéo theo rằng cặp $ (\pi, 1) $ là $ \mu $-thích nghi. Do đó (\S 4, No. 4, Th. 2), đối với mọi tập compact $ K \subset X $, hàm $ \varphi_K \circ \pi = \varphi_A $, trong đó $ A = \overline{\pi}^{-1}(K) $, là $ \mu $-khả tích về bản chất, nói cách khác, a) kéo theo b).

Ngược lại, giả sử rằng $ \overline{\pi}^{-1}(K) $ là $ \mu $-khả tích về bản chất đối với mọi tập con compact $ K $ của $ X $, và ta hãy chứng minh rằng a) được thỏa mãn. Thật vậy, cho $ S $ là giá của $ f $; vì $ S $ là compact, đặt $ A = \overline{\pi}^{-1}(S) $ ta có, theo giả thiết,

$$
\int^\bullet |f(\pi(t))| \, d\mu(t) \leq \|f\| \int^\bullet \varphi_S(\pi(t)) \, d\mu(t) = \|f\| \int^\bullet \varphi_A(t) \, d\mu(t) < +\infty.
$$

Vì $ f \circ \pi $ là $ \mu $-đo được (Ch. IV, \S 5, No. 3, Th. 1), ta thấy rằng $ f \circ \pi $ là $ \mu $-khả tích về bản chất (\S 1, No. 3, Prop. 9).

Tính chất b) hiển nhiên tương đương với tính chất sau (do đó cũng tương đương với a)):

c) *Đối với mọi điểm* $ x $ *của* $ X $, *tồn tại một lân cận* $ V $ *của* $ x $ *sao cho* $ \overline{\pi}^{-1}(V) $ *là* $ \mu $-*khả tích về bản chất*.

#### Định nghĩa 1 {#int-v-s6-def-1 .statement}

*Cho* $ \mu $ *là một độ đo dương trên một không gian địa phương compact* $ T $. *Một ánh xạ* $ \pi $ *của* $ T $ *vào một không gian địa phương compact* $ X $ *được gọi là* $ \mu $*-thực sự* (*hay thực sự đối với độ đo* $ \mu $) *nếu cặp* $ (\pi, 1) $ *là* $ \mu $*-thích nghi*, *nghĩa là* (\S 4, No. 1), *nếu* $ \pi $ *là* $ \mu $*-đo được và thỏa mãn các điều kiện (tương đương) của Mệnh đề 1*. *Độ đo* $ \int \varepsilon_{\pi(t)} \, d\mu(t) $ *trên* $ X $ *khi đó được gọi là ảnh của* $ \mu $ *qua* $ \pi $ *và được ký hiệu là* $ \pi(\mu) $.

Do đó nếu $ \nu = \pi(\mu) $ thì, theo định nghĩa, với $ f \in \mathcal{K}(X) $ ta có

$$
\int f(x) \, d\nu(x) = \int f(\pi(t)) \, d\mu(t).
$$

#### Nhận xét {#int-v-s6-n1-rem-1 .statement}

— 1) Nếu $ \mu $ là *bị chặn* (đặc biệt, nếu $ \mu $ có giá compact) thì mọi ánh xạ $ \mu $-đo được từ $ T $ vào $ X $ đều là $ \mu $-thực sự (Ch. IV, \S 5, No. 3, Th. 1 và No. 6, Th. 5).

2) Nếu $ \pi $ là $ \mu $-đo được và nếu, với mọi tập con compact $ K $ của $ X $, $ \overline{\pi}^{-1}(K) $ là tương đối compact, thì $ \pi $ là $ \mu $-thực sự (Ch. IV, \S 5, No. 5, Prop. 7 và No. 6, Th. 5); đặc biệt, mọi ánh xạ liên tục *thực sự* từ $ T $ vào $ X $ (GT, I, \S 10, No. 2, Th. 1) đều là $ \mu $-thực sự đối với mọi độ đo dương $ \mu $ trên $ T $. Đặc biệt hơn, điều này đúng với mọi *đồng phôi* $ \pi $ của $ T $ lên X; độ đo $ \nu = \pi(\mu) $ khi đó chính là độ đo trên X là phép chuyển của $ \mu $ bởi $ \pi $ (Ch. III, §1, No. 3).

3) Giả sử rằng tôpô của X có một cơ sở đếm được; khi đó mọi ánh xạ $ \pi $ của T vào X thỏa mãn điều kiện b) của Mệnh đề 1 là $ \mu $-đo được, do đó là $ \mu $-thực sự. Chỉ cần áp dụng Th. 4 của Ch. IV, §5, No. 5, bằng cách nhận thấy rằng X khi đó mêtric hóa được (GT, IX, §2, No. 9, Hệ quả của Prop. 16) và rằng, đối với mọi mêtric tương thích với tôpô của X, mọi quả cầu đóng là một hợp đếm được của các tập hợp compact.

### 2. Tích phân đối với ảnh của một độ đo dương

Cho $ \pi $ là một ánh xạ $ \mu $-thực sự của T vào X, và cho $ \nu = \pi(\mu) $. Áp dụng các kết quả của §4, ta thu được các mệnh đề sau:

#### Mệnh đề 2 {#int-v-s6-prop-2 .statement}

— *Đối với mọi hàm số* $ f \geqslant 0 $ *xác định trên* X,
$$
\int^\bullet f(x)\, d\nu(x) = \int^\bullet f(\pi(t))\, d\mu(t).
$$
(2)

Điều này suy ra từ Th. 1 của §4, No. 2.

#### Hệ quả 1 {#int-v-s6-prop-2-cor-1 .statement}

— *Đối với mọi tập con* A *của* X,
$$
\nu^\bullet(A) = \mu^\bullet(\pi^{-1}(A)).
$$

#### Hệ quả 2 {#int-v-s6-prop-2-cor-2 .statement}

— *Để một tập con* A *của* X *là không đáng kể địa phương đối với* $ \nu $, *điều kiện cần và đủ là* $ \pi^{-1}(A) $ *là không đáng kể địa phương đối với* $ \mu $.

#### Hệ quả 3 {#int-v-s6-prop-2-cor-3 .statement}

— *Nếu độ đo* $ \mu $ *tập trung trên một tập hợp* M, *thì* $ \pi(\mu) $ *tập trung trên* $ \pi(M) $.

Vì, nếu $ N = X - \pi(M) $ thì $ \pi^{-1}(N) $ không giao với M, do đó là địa phương $ \mu $-không đáng kể, do đó (Hệ quả 2) N là địa phương $ \nu $-không đáng kể.

#### Hệ quả 4 {#int-v-s6-prop-2-cor-4 .statement}

— *Cho* S *là giá của* $ \mu $. *Nếu* $ \pi $ *liên tục, thì giá của* $ \pi(\mu) $ *là* $ \pi(S) $.

Vì, từ Hệ quả 3 suy ra rằng $ \pi(\mu) $ tập trung trên $ \pi(S) $, do đó nếu $ S' $ là giá của $ \pi(\mu) $ thì $ S' \subset \pi(S) $. Mặt khác, $ \pi^{-1}(X - S') $ là một tập mở địa phương $ \mu $-không đáng kể (Hệ quả 2), nên là $ \mu $-không đáng kể (Ch. IV, §5, No. 2, Hệ quả 2 của Mệnh đề 5). Do đó $ \pi^{-1}(X - S') \subset T - S $, do đó $ \pi(S) \subset S' $, điều này chứng minh hệ quả.

#### Mệnh đề 3 {#int-v-s6-prop-3 .statement}

— *Để một ánh xạ* f *của* X *vào một không gian tôpô* G *là* $ \nu $*-đo được, điều kiện cần và đủ là* $ f \circ \pi $ *là* $ \mu $*-đo được.*

Đây là một hệ quả ngay lập tức của Mệnh đề 3 của §4, No. 3.

#### Hệ quả {#int-v-s6-n2-cor-1 .statement}

— Để một tập con A của X là $ \nu $-đo được, điều kiện cần và đủ là $ \pi^{-1}(A) $ là $ \mu $-đo được.

Tuy nhiên, ảnh theo $ \pi $ của một tập con M $ \mu $-đo được của T không nhất thiết là $ \nu $-đo được, ngay cả khi $ \pi $ liên tục và M là $ \mu $-không đáng kể (Bài tập 7 và §8, Bài tập 1).

#### Định lý 1 {#int-v-s6-thm-1 .statement}

— Cho f là một hàm xác định trên X với các giá trị trong $ \overline{\mathbf{R}} $ hoặc trong một không gian Banach F. Để f là khả tích $ \nu $-theo nghĩa bản chất, điều kiện cần và đủ là $ f \circ \pi $ là khả tích $ \mu $-theo nghĩa bản chất, trong trường hợp đó

$$
\int f(x)\, d\nu(x) = \int f(\pi(t))\, d\mu(t).
$$

Hơn nữa, giả sử rằng $ \pi $ liên tục và thực sự. Khi đó, để f là $ \nu $-khả tích, điều kiện cần và đủ là $ f \circ \pi $ là $ \mu $-khả tích.

Chỉ cần áp dụng Định lý 2 của §4, No. 4.

#### Hệ quả {#int-v-s6-n2-cor-2 .statement}

— Để một tập con A của X là $ \nu $-khả tích theo nghĩa bản chất, điều kiện cần và đủ là $ \pi^{-1}(A) $ là $ \mu $-khả tích theo nghĩa bản chất, trong trường hợp đó $ \nu(A) = \mu(\pi^{-1}(A)) $.

Đặc biệt, với mọi tập compact $ K \subset X $, $ \nu(K) = \mu(\pi^{-1}(K)) $. Từ điều này và Hệ quả 3 của Mệnh đề 2 suy ra rằng nếu $ \mu $ là nguyên tử (\S5, No. 10) thì $ \pi(\mu) = \nu $ cũng vậy. Vì, gọi M là tập hợp các $ t \in T $ sao cho $ \mu(\{t\}) \neq 0 $; vì $ \mu $ được mang bởi M, $ \nu $ được mang bởi $ \pi(M) $; hơn nữa, với mọi $ x \in \pi(M) $ ta có $ \nu(\{x\}) = \mu(\pi^{-1}(x)) > 0 $, vì $ \pi^{-1}(x) $ chứa ít nhất một điểm của M. Do đó $ \nu $ là nguyên tử (\S5, No. 10, Mệnh đề 15).

### 3. Các tính chất của ảnh của một độ đo dương

#### Mệnh đề 4 {#int-v-s6-prop-4 .statement}

— Cho T, T', T'' là ba không gian compact địa phương, $ \mu $ là một độ đo dương trên T, $ \pi $ là một ánh xạ $ \mu $-đo được của T vào T', $ \pi' $ là một ánh xạ của T' vào T'', và $ \pi'' = \pi' \circ \pi $.

(a) Giả sử rằng $ \pi $ là $ \mu $-thực sự và đặt $ \mu' = \pi(\mu) $. Để $ \pi' $ là $ \mu' $-thực sự, điều kiện cần và đủ là $ \pi'' $ là $ \mu $-thực sự, trong trường hợp đó $ \pi''(\mu) = \pi'(\pi(\mu)) $ ('tính bắc cầu của ảnh của một độ đo').

(b) Giả sử rằng $ \pi' $ liên tục, và $ \pi'' $ là $ \mu $-thực sự; khi đó $ \pi $ là $ \mu $-thực sự, $ \pi' $ là $ \pi(\mu) $-thực sự và $ \pi''(\mu) = \pi'(\pi(\mu)) $.

Dưới các giả thiết của a), để $ \pi'' $ là $ \mu $-đo được, điều kiện cần và đủ là $ \pi' $ là $ \mu' $-đo được (No. 2, Mệnh đề 3). Mặt khác nếu $ K $ là một tập con compact của $ T'' $, thì $ \pi''(K) = \pi^{-1}(\pi'(K)) $; để $ \pi''(K) $ khả tích theo nghĩa hầu khắp đối với $ \mu $, điều kiện cần và đủ là $ \pi'(K) $ khả tích theo nghĩa hầu khắp đối với $ \mu' $, theo Hệ quả của Định lý 1. Cuối cùng, nếu $ \pi'' $ là $ \mu $-thực sự thì, đặt $ \mu'' = \pi''(\mu) $, ta có, với mọi hàm $ f \in \mathcal{H}(T'') $,

$$
\int f(t'')\, d\mu''(t'') = \int f(\pi''(t))\, d\mu(t)
$$
$$
= \int f\left(\pi'\left(\pi(t)\right)\right)\, d\mu(t) = \int f(\pi'(t'))\, d\mu'(t')
$$

theo Định lý 1 của No. 2, điều này hoàn tất chứng minh của a).

Dưới các giả thiết của b), cho $ K' $ là một tập con compact của $ T' $. Khi đó $ K'' = \pi'(K') $ là compact, do đó $ \pi''(K'') $ khả tích theo nghĩa hầu khắp đối với $ \mu $, do đó $ \pi^{-1}(K') \subset \pi''(K'') $ khả tích theo nghĩa hầu khắp đối với $ \mu $ (Ch. IV, §5, No. 5, Mệnh đề 7), vì vậy $ \pi $ là $ \mu $-thực sự. Chứng minh được kết thúc bằng cách áp dụng phần a) của mệnh đề.

#### Hệ quả {#int-v-s6-n3-cor-1 .statement}

*Cho $ T $ và $ T' $ là hai không gian compact địa phương, $ \mu $ là một độ đo dương trên $ T $, $ \pi $ là một ánh xạ song ánh của $ T $ lên $ T' $, và $ \pi^{-1} $ là ánh xạ nghịch đảo. Giả sử rằng $ \pi $ là $ \mu $-thực sự, và đặt $ \mu' = \pi(\mu) $. Khi đó $ \pi^{-1} $ là $ \mu' $-thực sự và $ \pi^{-1}(\pi(\mu)) = \mu $.*

#### Mệnh đề 5 {#int-v-s6-prop-5 .statement}

*Cho $ T $ và $ X $ là hai không gian compact địa phương, $ \mu $ là một độ đo dương trên $ T $, $ \pi $ là một ánh xạ $ \mu $-thực sự của $ T $ vào $ X $, $ g $ là một hàm số hữu hạn $ \geqslant 0 $, xác định trên $ X $ và sao cho $ g \circ \pi $ khả tích địa phương đối với $ \mu $. Để $ g $ khả tích địa phương đối với $ \pi(\mu) $, điều kiện cần và đủ là $ \pi $ thực sự đối với độ đo $ (g \circ \pi) \cdot \mu $, khi đó*

$$
\pi((g \circ \pi) \cdot \mu) = g \cdot \pi(\mu).
$$

Đặt $ \nu = \pi(\mu) $. Để $ g $ khả tích địa phương đối với $ \nu $, điều kiện cần và đủ là $ gf $ khả tích đối với $ \nu $ với mọi hàm $ f \in \mathcal{H}(X) $; vì $ gf $ có giá compact, cũng có thể nói rằng $ gf $ khả tích đối với $ \nu $ theo nghĩa hầu khắp nơi, và điều này tương đương với việc $ (g \circ \pi)(f \circ \pi) $ khả tích đối với $ \mu $ theo nghĩa hầu khắp nơi (Định lý 1). Nhưng, theo Định lý 1 của §5, No. 3, điều này có nghĩa là $ f \circ \pi $ khả tích theo nghĩa hầu khắp nơi đối với $ \rho = (g \circ \pi) \cdot \mu $, và theo định nghĩa, điều này nói rằng $ \pi $ là $ \rho $-thực sự (vì hiển nhiên $ \pi $ là $ \rho $-đo được). Hơn nữa,

$$
\int fg\, d\nu = \int f(\pi(t))g(\pi(t))\, d\mu(t) = \int f(\pi(t))\, d\rho(t)
$$

(No. 2, Định lý 1 và §5, Định lý 1), điều này chứng minh quan hệ (4).

#### Mệnh đề 6 {#int-v-s6-prop-6 .statement}

— Cho T và X là hai không gian compact địa phương, $(\lambda_\alpha)_{\alpha \in A}$ là một họ các độ đo dương trên T, có hướng theo quan hệ $ \leq $, nhận một cận trên đúng $\mu$ trong $ \mathcal{M}(T) $. Để một ánh xạ $ \pi $ của T vào X là $ \mu $-thực sự, điều kiện cần và đủ là nó $ \lambda_\alpha $-thực sự với mọi $ \alpha \in A $, và họ $ (\pi(\lambda_\alpha))_{\alpha \in A} $ bị chặn trên trong $ \mathcal{M}(X) $. Trong trường hợp này,

$$
\pi(\mu) = \sup_\alpha \pi(\lambda_\alpha).
$$

Để $ \pi $ là $ \mu $-đo được, điều kiện cần và đủ là $ \pi $ $ \lambda_\alpha $-đo được với mọi $ \alpha \in A $ (\S 1, No. 4, Hệ quả 2 của Mệnh đề 11). Giả sử điều kiện này được thỏa mãn; khi đó, nói rằng $ \pi $ là $ \mu $-thực sự tương đương với nói rằng, với mọi hàm $ f \in \mathcal{K}_+(X) $,

$$
\mu^\bullet(f \circ \pi) < +\infty.
$$

Bây giờ,

$$
\int^\bullet (f \circ \pi)\, d\mu = \sup_\alpha \int^\bullet (f \circ \pi)\, d\lambda_\alpha = \sup_\alpha \int^\bullet f\, d(\pi(\lambda_\alpha))
$$

(\S 1, No. 4, Prop. 11); do đó phần tử thứ nhất là hữu hạn với mọi $ f \in \mathcal{K}_+(X) $ khi và chỉ khi họ $ (\pi(\lambda_\alpha)) $ nhận một cận trên nhỏ nhất $ \theta $ trong $ \mathcal{M}(X) $, trong trường hợp đó $ \int (f \circ \pi)\, d\mu = \int f\, d\theta $, một quan hệ tương đương với (5).

#### Hệ quả 1 {#int-v-s6-prop-6-cor-1 .statement}

— Cho $ (\mu_\alpha)_{\alpha \in A} $ là một họ tổng được của các độ đo dương trên T, sao cho $ \mu = \sum_{\alpha \in A} \mu_\alpha $; để một ánh xạ $ \pi $ từ T vào một không gian compact địa phương X là $ \mu $-thực sự, điều kiện cần và đủ là nó là $ \mu_\alpha $-thực sự với mọi $ \alpha \in A $, và họ $ (\pi(\mu_\alpha))_{\alpha \in A} $ là tổng được. Trong trường hợp này,

$$
\pi(\mu) = \sum_{\alpha \in A} \pi(\mu_\alpha).
$$

#### Hệ quả 2 {#int-v-s6-prop-6-cor-2 .statement}

— Cho T và X là hai không gian compact địa phương, $ (\lambda_i)_{1 \leq i \leq n} $ là một dãy hữu hạn các độ đo dương trên T, và đặt $ \mu = \sum_{i=1}^n \lambda_i $. Để một ánh xạ $ \pi $ từ T vào X là $ \mu $-thực sự, điều kiện cần và đủ là nó là $ \lambda_i $-thực sự với mọi chỉ số i, trong trường hợp đó

$$
\sum_{i=1}^n \pi(\lambda_i) = \pi\left( \sum_{i=1}^n \lambda_i \right).
$$

### 4. Ảnh của một độ đo phức

Cho $ \theta $ là một độ đo phức trên $ T $, và cho $ \pi $ là một ánh xạ từ $ T $ vào một không gian compact địa phương $ X $; giả sử rằng $ \pi $ là $ \theta $-đo được, và rằng với mỗi $ f \in \mathcal{K}(X; \mathbf{C}) $, $ f \circ \pi $ là khả tích theo $ \theta $ một cách hầu khắp. Vì nói rằng một hàm là đo được (tương ứng khả tích một cách hầu khắp) đối với $ \theta $ hay đối với $ |\theta| $ là tương đương, điều này có nghĩa là $ \pi $ là $ |\theta| $-thực sự. Nếu $ f \in \mathcal{K}(X; \mathbf{C}) $,

$$
\left| \int (f \circ \pi) \, d\theta \right| \leq \int (|f| \circ \pi) \, d|\theta| ;
$$

suy ra ngay lập tức rằng dạng tuyến tính $ f \mapsto \int (f \circ \pi) \, d\theta $ trên $ \mathcal{K}(X; \mathbf{C}) $ là một *độ đo phức* trên $ X $ (Ch. III, §1, No. 3, Prop. 6), và ta có thể đưa ra định nghĩa sau:

#### Định nghĩa 2 {#int-v-s6-def-2 .statement}

*Cho $ \theta $ là một độ đo phức trên một không gian compact địa phương $ T $. Một ánh xạ $ \pi $ từ $ T $ vào một không gian compact địa phương $ X $ được gọi là $ \theta $-thực sự nếu nó là $ |\theta| $-thực sự. Khi đó độ đo $ f \mapsto \int (f \circ \pi) \, d\theta $ được gọi là ảnh của $ \theta $ qua $ \pi $ và được ký hiệu là $ \pi(\theta) $.*

Quan hệ (7) khi đó có thể được viết dưới dạng sau:

$$
|\pi(\theta)| \leq \pi(|\theta|) .
$$

Độ đo $ \pi(\theta) $ có thể bằng không mà $ \theta $ không bằng không, như thấy ngay lập tức khi lấy cho $ T $ một không gian thu gọn thành hai điểm $ a, b $, cho $ \theta $ là độ đo $ \varepsilon_a - \varepsilon_b $, và cho $ \pi $ là một ánh xạ hằng.

Cho $ \theta $ và $ \theta' $ là hai độ đo phức trên $ T $; nếu $ \pi $ là $ \theta $-thực sự và $ \theta' $-thực sự, thì từ Hệ quả 2 của Mệnh đề 6 suy ra rằng $ \pi $ là $ (\theta + \theta') $-thực sự vì $ |\theta + \theta'| \leq |\theta| + |\theta'| $, và hiển nhiên $ \pi(\theta + \theta') = \pi(\theta) + \pi(\theta') $.

Đặc biệt, nếu $ \theta $ là một độ đo thực và $ \pi $ là $ \theta $-thực sự, thì

$$
\pi(\theta) = \pi(\theta^+) - \pi(\theta^-) .
$$

Một số kết quả đã được thiết lập trước đó mở rộng ngay lập tức cho các độ đo phức; chúng tôi nêu những kết quả quan trọng nhất trong số đó.

#### Mệnh đề 7 {#int-v-s6-prop-7 .statement}

*Cho $ \theta $ là một độ đo phức trên $ T $, $ \pi $ là một ánh xạ $ \theta $-thực sự từ $ T $ vào một không gian compact địa phương $ X $, $ \nu $ là độ đo ảnh $ \pi(\theta) $.

a) Cho $ A $ là một tập con của $ X $; nếu $ \overline{\pi^{-1}}(A) $ là không đáng kể địa phương đối với $ \theta $, thì $ A $ là không đáng kể địa phương đối với $ \nu $.

b) Cho $ f $ là một ánh xạ từ $ X $ vào một không gian tôpô; nếu $ f \circ \pi $ là $ \theta $-đo được, thì $ f $ là $ \nu $-đo được.*

c) Cho $ f $ là một hàm xác định trên $ X $, có các giá trị trong một không gian Banach $ F $; nếu $ f \circ \pi $ là khả tích $ \theta $ về bản chất, thì $ f $ là khả tích $ \nu $ về bản chất và

$$
\int f(\pi(t))\ d\theta(t) = \int f(x)\ d\nu(x).
$$

Có tính đến công thức (8), các kết quả này có thể được suy ra từ Hệ quả 2 của Mệnh đề 2, từ Mệnh đề 3, và từ Định lý 1 của No. 2.

### 5. Áp dụng: thay đổi biến trong nguyên Lebesgue

Cho I là một khoảng (bị chặn hoặc không) của $ \mathbf{R} $, $ a $ là đầu mút trái của nó và $ b $ là đầu mút phải của nó trong $ \overline{\mathbf{R}} $, và $ \mu $ là độ đo Lebesgue trên I. Đối với mọi hàm khả tích $ \mu $ $ f $ và mọi khoảng $ H \subset I $, có đầu mút trái $ \alpha $ và đầu mút phải $ \beta $, ta viết $ \int_{\alpha}^{\beta} f(t)\ dt $ thay cho $ \int_H f(t)\ dt = \int_H f\ d\mu $, và ta đặt $ \int_{\beta}^{\alpha} f(t)\ dt = -\int_{\alpha}^{\beta} f(t)\ dt $; ý nghĩa được gán như vậy cho các ký hiệu này trùng với ý nghĩa đã được gán cho chúng trong FRV, II, §§1 và 2, khi $ f $ là một hàm điều hòa có giá đỡ compact (Ch. IV, §4, No. 4, Ví dụ).

Cho $ g $ là một hàm số xác định trên I và *địa phương $ \mu $*-khả tích, $ x_0 $ là một điểm của I; với mọi $ x \in I $, đặt

$$
G(x) = c + \int_{x_0}^{x} g(t)\ dt \quad (c \text{ một hằng}).
$$

Hàm số số G là *liên tục* trên I; điều này suy ra ngay từ định lý Lebesgue (Ch. IV, §4, No. 3, Hệ quả 1 của Định lý 2), vì tích của $ g $ và hàm đặc số của khoảng có hai đầu mút $ x $ và $ x+h $ tiến tới một hàm không đáng kể khi $ h $ tiến tới 0. Do đó G(I) là một *khoảng* của $ \mathbf{R} $. Trong toàn bộ No. này, ta sẽ xem G như một ánh xạ của I lên không gian compact địa phương G(I). Ta ký hiệu $ \lambda $ là độ đo $ g \cdot \mu $ trên I.

Trước hết giả sử rằng $ g $ là $ \mu $*-khả tích*. Khi đó, cùng một lập luận như trên cho thấy các giới hạn $ G(a+) $ và $ G(b-) $ tồn tại và là *hữu hạn*; hơn nữa, độ đo $ |\lambda| $ là *bị chặn* (§5, No. 3, Hệ quả của Định lý 1), và ánh xạ G của I vào G(I) là *$ \lambda $*-thực sự.

#### Mệnh đề 8 {#int-v-s6-prop-8 .statement}

*Giả sử g là $ \mu $*-khả tích*. Nếu J ký hiệu khoảng mở trong $ \mathbf{R} $ có hai đầu mút $ G(a+) $ và $ G(b-) $, thì ảnh theo G của độ đo $ g \cdot \mu $ là độ đo $ \varphi_J \cdot \nu $ nếu $ G(a+) \leq G(b-) $ và là độ đo $ -\varphi_J \cdot \nu $ nếu $ G(a+) \geq G(b-) $ (trong đó $ \nu $ ký hiệu độ đo Lebesgue trên G(I)).*

Chỉ cần chứng minh rằng, với mọi hàm $ f \in \mathcal{K}(G(I)) $,

$$
\int_{G(a+)}^{G(b-)} f(\xi) d\xi = \int_a^b f(G(t))g(t)\,dt.
$$

Bây giờ, công thức này đã được chứng minh cho $ g \in \mathcal{K}(I) $ (FRV, II, §2, No. 1, công thức (1)). Ta chuyển sang trường hợp tổng quát; tồn tại một dãy $ (g_n) $ các hàm trong $ \mathcal{K}(I) $ sao cho: $ 1^\circ $ dãy $ (g_n(t)) $ tiến tới $ g(t) $ hầu khắp nơi trong $ I $; $ 2^\circ $ tồn tại một hàm $ \mu $-khả tích $ h \geq 0 $ sao cho $ |g_n| \leq h $ với mọi $ n $ (Ch. IV, §3, No. 4, Định lý 3). Suy ra ngay từ định lý Lebesgue rằng, đặt $ G_n(x) = c + \int_{x_0}^x g_n(t)\,dt $, dãy $ (G_n) $ hội tụ đều đến G trên $ I $, và các số $ G_n(a+) $ và $ G_n(b-) $ lần lượt tiến tới $ G(a+) $ và $ G(b-) $. Gọi $ f' $ là một hàm trong $ \mathcal{K}(\mathbf{R}) $ mở rộng f; điều đã nêu ở trên chứng minh rằng $ f'(G_n(t)) $ tiến tới $ f'(G(t)) = f(G(t)) $ với mọi $ t \in I $; áp dụng định lý Lebesgue, ta thấy rằng công thức (12) suy ra từ công thức

$$
\int_{G_n(a+)}^{G_n(b-)} f'(\xi)\,d\xi = \int_a^b f'(G_n(t))g_n(t)\,dt
$$

bằng cách chuyển qua giới hạn.

#### Hệ quả {#int-v-s6-n5-cor-1 .statement}

*Nếu một hàm $ \mathbf{f} $ xác định trên $ G(I) $, có giá trị trong $ \overline{\mathbf{R}} $ hoặc trong một không gian Banach, sao cho hàm $ t \mapsto \mathbf{f}(G(t))g(t) $ là khả tích trên $ I $ đối với độ đo Lebesgue, thì $ \mathbf{f} $ là khả tích trên $ J $ đối với độ đo Lebesgue và*

$$
\int_{G(a+)}^{G(b-)} \mathbf{f}(\xi)\,d\xi = \int_a^b \mathbf{f}(G(t))g(t)\,dt
$$

(công thức đổi biến trong tích phân Lebesgue).

Vì, $ \mathbf{f}(G(t)) $ khả tích đối với độ đo $ |g|\cdot\mu $, do đó cũng đối với các độ đo $ g^+\cdot\mu $ và $ g^-\cdot\mu $; suy ra từ Đl. 1 (No. 2) rằng $ \mathbf{f} $ khả tích đối với các độ đo ảnh $ G(g^+\cdot\mu) $ và $ G(g^-\cdot\mu) $, do đó cũng đối với độ đo $ \varphi_J \cdot \nu $, và rằng (13) đúng, khi tính đến Mđ. 8 và công thức (9).

Có thể xảy ra rằng $ \mathbf{f} $ khả tích trên $ J $ đối với độ đo Lebesgue, nhưng $ t \mapsto \mathbf{f}(G(t))g(t) $ không khả tích trên $ I $ đối với độ đo Lebesgue (Bài tập 10).

Bây giờ giả sử rằng $ g $ giữ *dấu hằng* hầu khắp nơi (và là $ \mu $-khả tích địa phương); chẳng hạn ta có thể giả sử rằng $ g(t) \geq 0 $ hầu khắp nơi trong $ I $. Khi đó $ G $ là một hàm liên tục tăng trên $ I $, do đó $ G(a+) $ và $ G(b-) $ tồn tại (nhưng có thể là vô hạn). Hơn nữa, $ G $ là một ánh xạ *$ \lambda $-thực sự* của $ I $ vào $ G(I) $: vì, nếu $ G(b-) \in G(I) $, tồn tại một x_1 \geq x_0 \text{ sao cho } G \text{ là hằng với } x \geq x_1, \text{ và khi đó ảnh ngược qua } G \text{ của khoảng compact } [G(x_0), G(b-)] \text{ là } \lambda\text{-khả tích; nếu ngược lại, } G(b-) \notin G(I), \text{ thì ảnh ngược qua } G \text{ của mọi khoảng compact có điểm đầu trái } G(x_0), \text{ được chứa trong } G(I), \text{ sai khác với một khoảng compact nhiều nhất bởi một khoảng } \lambda\text{-không đáng kể. Ta lập luận tương tự đối với các khoảng compact có điểm đầu phải } G(x_0), \text{ do đó có mệnh đề của ta. Hơn nữa:}

#### Mệnh đề 9 {#int-v-s6-prop-9 .statement}

*Giả sử $ g \geq 0 $ và $ \mu $-khả tích địa phương. Khi đó, ảnh qua $ G $ của độ đo dương $ g \cdot \mu $ là độ đo Lebesgue trên $ G(I) $. Đối với một hàm $ f $, xác định trên $ G(I) $, nhận giá trị trong $ \overline{\mathbf{R}} $ hoặc trong một không gian Banach, để khả tích trên $ G(I) $ đối với độ đo Lebesgue, điều kiện cần và đủ là hàm $ t \mapsto f(G(t))g(t) $ khả tích trên $ I $ đối với độ đo Lebesgue, trong trường hợp đó quan hệ (13) đúng.*

Phần đầu của mệnh đề suy ra từ sự kiện rằng công thức (12) đúng đối với mọi hàm $ f \in \mathcal{K}(G(I)) $; vì giá của hàm $ t \mapsto f(G(t)) $ được chứa trong một khoảng $ K \subset I $ trên đó $ g $ khả tích, theo các nhận xét ở trên, và chỉ cần áp dụng Mđ. 8 cho $ K $. Phần thứ hai là một hệ quả của Đl. 1 của No. 2.

### 6. Phân tích thành các lát. Ảnh ngược của một độ đo qua một phép đồng phôi địa phương

Cho $ X $ là một không gian compact địa phương, $ \pi $ là một ánh xạ của $ X $ vào một không gian compact địa phương $ T $, $ \mu $ là một độ đo dương trên $ T $, $ \Lambda : t \mapsto \lambda_t $ là một ánh xạ khả $ \mu $-tích phân theo vô hướng thực sự và đo được $ \mu $-theo nghĩa mơ hồ từ $ T $ vào $ \mathcal{M}_+(X) $. Đặt $ \nu = \int \lambda_t d\mu(t) $. Nếu $ \lambda_t $ được *mang bởi* $ \overline{\pi}^{-1}(t) $ với mọi $ t \in T $, đẳng thức $ \nu = \int \lambda_t d\mu(t) $ được gọi là một *phân tích thành các lát* (hay một *phân ly*) của $ \nu $ đối với $ \pi $. Khái niệm này sẽ được nghiên cứu chi tiết trong Ch. VI.

#### Mệnh đề 10 {#int-v-s6-prop-10 .statement}

*Với các ký hiệu trên, giả sử rằng $ \pi $ là $ \nu $-đo được. Gọi $ g $ là hàm $ t \mapsto \lambda_t^*(1) $ trên $ T $. Để $ \pi $ là $ \nu $-thực sự, điều kiện cần và đủ là $ g $ nguyên địa phương theo $ \mu $, trong trường hợp đó*

$$
\pi(\nu) = g \cdot \mu.
$$

Ta bắt đầu bằng cách lập luận với giả thiết rằng $ g $ hữu hạn địa phương hầu khắp nơi theo $ \mu $; ta sẽ loại bỏ giả thiết phụ này ở cuối chứng minh. Vì $ \pi $ theo giả thiết là $ \nu $-đo được, nói rằng $ \pi $ là $ \nu $-thực sự tương đương với nói rằng $ \nu^*(f \circ \pi) < +\infty $ với mọi hàm $ f \in \mathcal{K}_+(T) $; do $ g $ hữu hạn địa phương hầu khắp nơi, ta ở trong các điều kiện để áp dụng mệnh đề c) của Mệnh đề 5 của §3, No. 2. Do đó

$$
\int^\bullet (f \circ \pi)\, d\nu = \int^\bullet d\mu(t) \int^\bullet (f \circ \pi)\, d\lambda_t = \int^\bullet f(t)g(t)\, d\mu(t),
$$

từ sự kiện rằng $ \lambda_t $ tập trung trên $ \overline{\pi}^{-1}(t) $. Ta biết rằng $ g $ là $ \mu $-đo được, vì $ \Lambda $ là $ \mu $-thích hợp (\S3, No. 1, Def. 1). Nói rằng vế đầu tiên là hữu hạn với mọi $ f \in \mathcal{K}_+(T) $ do đó tương đương với nói rằng $ g $ nguyên địa phương theo $ \mu $ (\S5, Prop. 1), và trong trường hợp này (14) suy ra ngay từ các hệ thức trên.

Vì vậy, chỉ còn lại việc loại bỏ giả thiết phụ. Nếu $ g $ nguyên địa phương theo $ \mu $, thì $ g $ hữu hạn địa phương hầu khắp nơi theo $ \mu $, và giả thiết quả thực được thỏa mãn. Giả sử rằng $ \pi $ là $ \nu $-thực sự, và hãy chứng minh rằng $ g $ hữu hạn địa phương hầu khắp nơi. Gọi $ \mathfrak{K} $ là tập hợp $ \mu $-trù mật của các tập compact $ K $ sao cho $ \Lambda|K $ liên tục theo nghĩa mơ hồ; vì $ g $ là đo được, ta chỉ cần chứng minh rằng mọi tập compact $ K \in \mathfrak{K} $ sao cho $ g|K = +\infty $ đều là $ \mu $-không đáng kể. Bây giờ, gọi $ \mathcal{H} $ là tập hợp các hàm $ h \in \mathcal{K}_+(X) $ sao cho $ h \leq 1 $; đặt $ g_h(t) = \lambda_t(h) $, ký hiệu $ \Lambda_h $ là ánh xạ $ \mu $-thích hợp $ t \mapsto h \cdot \lambda_t $, ký hiệu $ \nu_h $ là tích phân của $ \Lambda_h $, và gọi $ f $ là một phần tử của $ \mathcal{K}_+(T) $ sao cho $ f \geq \varphi_K $. Áp dụng công thức (14) cho $ \Lambda_h $, ánh xạ này thỏa mãn giả thiết phụ, ta thu được:

$$
\int (f \circ \pi)\, d\nu \geq \int (f \circ \pi)\, d\nu_h = \int fg_h\, d\mu.
$$

Nhưng các hàm $ fg_h|K $ tạo thành một tập có hướng tăng của các hàm liên tục trên $ K $, bao trên của chúng có giá trị $ +\infty $; theo định lý Dini (GT, X, §4, No. 1, Th. 1), ta có thể chọn $ h $ sao cho $ fg_h|K $ lớn hơn hoặc bằng một số dương tùy ý $ n $, và do đó suy ra rằng $ \int (f \circ \pi)\, d\nu \geq n\, \mu(K) $. Vì vế thứ nhất là hữu hạn bởi vì $ \pi $ là $ \nu $-thực sự, nên suy ra $ \mu(K) = 0 $.

#### Hệ quả 1 {#int-v-s6-prop-10-cor-1 .statement}

— *Giả sử rằng $ \pi $ là $ \nu $-đo được.*

a) *Nếu $ N \subset T $ là địa phương $ \mu $-không đáng kể, thì $ \overline{\pi}^{-1}(N) $ là địa phương $ \nu $-không đáng kể.*
b) *Nếu $ f $ là một ánh xạ $ \mu $-đo được từ $ T $ vào một không gian tôpô $ G $, thì $ f \circ \pi $ là $ \nu $-đo được.*

Ta lấy lại các ký hiệu $ \Lambda_h $, $ \nu_h $, $ g_h $ ở cuối chứng minh trước: $ \nu_h $ là một độ đo bị chặn với mọi $ h \in \mathcal{H} $, $ \pi $ là $ \nu_h $-thực sự, $ g_h $ là địa phương $ \mu $-khả tích, và $ \pi(\nu_h) = g_h \cdot \mu $, một độ đo có cơ sở $ \mu $. Do đó $ N $ là địa phương không đáng kể (tương ứng $ f $ là đo được) đối với độ đo $ \pi(\nu_h) $ (\S5, No. 3, Hệ quả 1 của Mệnh đề 3 và Mệnh đề 4). Do đó $ \overline{\pi}^{-1}(N) $ là địa phương không đáng kể (tương ứng $ f \circ \pi $ là đo được) đối với độ đo $ \nu_h $ (Hệ quả 2 của

Mệnh đề 2, tương ứng Mệnh đề 3). Cuối cùng, ta nhận xét rằng các độ đo $ \nu_h $ tạo thành một họ có hướng tăng của các độ đo dương mà cận trên là $ \nu $, và áp dụng Hệ quả 1 (tương ứng Hệ quả 2) của Mệnh đề 11 của §1, No. 4.

#### Hệ quả 2 {#int-v-s6-prop-10-cor-2 .statement}

*Giả sử rằng $ \pi $ là $ \nu $-thực sự; cho $ f $ là một ánh xạ xác định trên $ T $, có các giá trị trong một không gian Banach hoặc trong $ \overline{\mathbf{R}} $. Để $ f \circ \pi $ là thiết yếu $ \nu $-khả tích, điều kiện cần và đủ là $ gf $ là thiết yếu $ \mu $-khả tích.*

Có tính đến Mệnh đề 10, điều này suy ra ngay lập tức từ Định lý 1 của §5, No. 3 và Định lý 1 của No. 2.

#### Ví dụ {#int-v-s6-n6-exa-1 .statement}

— Cho $ X $ và $ T $ là hai không gian compact địa phương, và cho $ \pi $ là một *phép đồng phôi địa phương của $ X $ vào $ T $*. Nói cách khác (GT, I, §11, Bài tập 25), ta giả sử rằng mỗi điểm $ x \in X $ có một lân cận $ V $ sao cho $ \pi|V $ là một phép đồng phôi từ $ V $ lên một lân cận của $ \pi(x) $; nếu cần thay thế $ V $ bởi một lân cận mở tương đối compact $ W $ của $ x $ sao cho $ \overline{W} \subset V $, ta suy ra rằng tập hợp $ \mathcal{U} $ gồm các tập con mở tương đối compact $ U $ của $ X $, sao cho $ \pi|\overline{U} $ là một phép đồng phôi từ $ \overline{U} $ lên ảnh của nó, là một *phủ mở* của $ X $. Bây giờ cho $ \mu $ là một độ đo dương trên $ T $; nếu $ U $ là một phần tử của $ \mathcal{U} $, thì $ \pi(U) $ là một tập hợp mở trong không gian compact $ \pi(\overline{U}) $, do đó là một không gian con địa phương compact của $ T $, và ta biết cách định nghĩa độ đo $ \mu|\pi(U) $ cảm sinh bởi $ \mu $ trên $ \pi(U) $ (Ch. IV, §5, No. 7). Cho $ \nu_U $ là ảnh của $ \mu|\pi(U) $ qua phép đồng phôi nghịch đảo với $ \pi|U $; ta sẽ chứng minh rằng tồn tại một và chỉ một độ đo $ \nu $ trên $ X $ cảm sinh độ đo $ \nu_U $ trên mọi tập hợp mở $ U \in \mathcal{U} $. Độ đo này được gọi là *ảnh ngược của $ \mu $ qua phép đồng phôi địa phương $ \pi $*, và được ký hiệu $ \pi^{-1}(\mu) $.

Tính duy nhất của $ \nu $ suy ra ngay từ nguyên lý địa phương hóa (Ch. III, §2, No. 1, Hệ quả của Mệnh đề 1). Để thiết lập sự tồn tại, ta chú ý rằng nếu $ t \in T $, thì mỗi điểm $ x \in \pi^{-1}(t) $ có một lân cận chỉ giao với $ \pi^{-1}(t) $ tại điểm $ x $, do đó $ \pi^{-1}(t) $ là một không gian con *rời rạc* của $ X $, và họ $ (\varepsilon_x)_{x \in \pi^{-1}(t)} $ là tổng được; ta ký hiệu tổng của nó là $ \lambda_t $. Tiếp theo ta chứng minh rằng ánh xạ $ t \mapsto \lambda_t $ là khả tích $ \mu $-nguyên cốt yếu theo vô hướng, và rằng nguyên của nó $ \nu = \int \lambda_t d\mu(t) $ là ảnh ngược cần tìm. Điều này sẽ suy ra ngay từ bổ đề sau:

#### Bổ đề {#int-v-s6-n6-lem-1 .statement}

— a) *Cho $ f $ là một phần tử của $ \mathscr{K}_+(X) $; hàm $ t \mapsto \lambda_t(f) $ là dương, nửa liên tục trên, có giá compact, và hạn chế của nó trên $ \pi(X) $ là liên tục.*

b) *Cho $ U $ là một phần tử của $ \mathcal{U} $, $ \nu $ là nguyên của hàm $ \mu $-khả tích thực chất theo vô hướng $ t \mapsto \lambda_t $; ảnh của độ đo $ \nu|U $ qua $ \pi|U $ bằng $ \mu|\pi(U) $.*

Để thiết lập a), người ta có thể rút gọn nhờ một phân hoạch đơn vị (Ch. III, §1, No. 2, Bổ đề 1) về trường hợp giá $ S $ của $ f $ được chứa trong một tập mở $ U \in \mathcal{U} $. Gọi $ g $ là ánh xạ $ t \mapsto \lambda_t(f) $; vì $ \pi|U $ là một đồng phôi, $ g|\pi(U) $ thuộc $ \mathcal{K}_+(\pi(U)) $, do đó ($ \pi(U) $ là một tập mở trong $ \pi(X) $) hạn chế của $ g $ lên $ \pi(X) $ là liên tục. Vì $ g $ là dương và hạn chế của $ g $ lên tập compact $ \pi(S) $ là liên tục, ta thấy rằng $ g $ là nửa liên tục trên trên $ T $. Suy ra rằng $ g $ là $ \mu $-khả tích.

Để thiết lập b), ký hiệu $ g $ là một phần tử của $ \mathcal{K}(\pi(U)) $, $ g^\circ $ là mở rộng của nó bởi 0 lên $ T $, $ f $ là hàm $ g \circ (\pi|U) $, và $ f^\circ $ là mở rộng bởi 0 của $ f $ lên $ X $. Mệnh đề b) tương đương với đẳng thức $ \int g^\circ d\mu = \int f^\circ d\nu $. Nhưng $ f \in \mathcal{K}(U) $, do đó $ f^\circ \in \mathcal{K}(X) $, và nguyên thứ hai do đó bằng $ \int \lambda_t(f^\circ) d\mu(t) $. Cuối cùng $ \lambda_t(f^\circ) = g^\circ(t) $, điều này hoàn thành chứng minh.

Bây giờ ta nhận xét rằng $ \pi(X) $ là *mở* trong $ T $, do đó là $ \mu $-đo được; ánh xạ $ \Lambda : t \mapsto \lambda_t $ là $ \mu $-đo được theo nghĩa mơ hồ, vì hạn chế của nó lên mỗi tập hợp $ \pi(X) $ và $ \mathbf{C}\pi(X) $ là liên tục theo nghĩa mơ hồ. Trong các điều kiện này, công thức $ \overline{\pi}^{-1}(\mu) = \int \lambda_t d\mu(t) $ xác định một phân tích thành các lát của $ \overline{\pi}^{-1}(\mu) $ tương đối với $ \pi $, và Mệnh đề 10 cho kết quả sau:

#### Mệnh đề 11 {#int-v-s6-prop-11 .statement}

*Cho $ \pi $ là một đồng phôi địa phương của một không gian compact địa phương $ X $ vào một không gian compact địa phương $ T $, và cho $ \mu $ là một độ đo dương trên $ T $. Cho $ n $ là hàm số liên kết với mỗi $ t \in T $ số phần tử của $ \overline{\pi}^{-1}(t) $ nếu số này là hữu hạn, và $ +\infty $ trong trường hợp ngược lại. Để $ \pi $ là $ \overline{\pi}^{-1}(\mu) $-thực sự, điều kiện cần và đủ là $ n $ khả tích địa phương theo $ \mu $, trong trường hợp đó*

$$
\pi\left( \overline{\pi}^{-1}(\mu) \right) = n \cdot \mu .
$$

### Bài tập {#int-v-s6-exercises}

Xem các [bài tập cho § 6](exercises/s6/).
