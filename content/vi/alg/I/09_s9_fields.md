---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 9
section_title: Fields
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0138-0142, 0198-0203
extraction: ocr
subsections:
    - "no": 1
      title: FIELDS
      page: 0
      pdf_page: 138
    - "no": 2
      title: INTEGRAL DOMAINS
      page: 0
      pdf_page: 140
    - "no": 3
      title: PRIME IDEALS
      page: 0
      pdf_page: 140
    - "no": 4
      title: THE FIELD OF RATIONAL NUMBERS
      page: 0
      pdf_page: 141
statements: 17
exercises: 21
content_sha256: 6c0359b710c06bfc49eb6fa6c47f382919ab897dfd305a178aee44ce21b28c62
translated_from: content/en/alg/I/09_s9_fields.md
source_content_sha256: fee761e3a01ac2b07d1598dce540a09343de6c16c63a3089ff4316bb4f64f378
translation_model: gpt-5-6-mini
translation_run: translate-vi-6fafc88f
glossary_version: 34
glossary_terms_sha256: 495b454c2eb829e4659f6b61436ece1e810726db671487d97fbdae92c499fdb3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. TRƯỜNG

### 1. TRƯỜNG

#### Định nghĩa 1 {#alg-i-s9-def-1 .statement}

*Một vành $ K $ được gọi là một trường nếu nó không chỉ gồm $ 0 $ và mọi phần tử khác không của $ K $ đều khả nghịch.*

Tập hợp các phần tử khác không của trường $ K $, với phép nhân, là một nhóm, chính xác là nhóm nhân $ K^* $ của vành $ K $ (\S 8, no. 1). Vành đối của một trường là một trường. Một trường được gọi là *giao hoán* nếu phép nhân của nó giao hoán; khi đó trường này được đồng nhất với vành đối của nó. Một trường không giao hoán đôi khi được gọi là một *trường skew*.

#### Ví dụ {#alg-i-s9-n1-exa-1 .statement}

*(1)* Trong no. 4, chúng ta sẽ định nghĩa trường các *số hữu tỉ*; trong *Tôpô đại cương*, trường các số thực sẽ được định nghĩa (*Tôpô đại cương*, IV, \S 1, no. 3), cũng như trường các số phức (*Tôpô đại cương*, VIII, \S 1, no. 1) và trường các quaternion (*Tôpô đại cương*, VIII, \S 1, no. 4). Các trường này giao hoán, ngoại trừ trường các quaternion.*
*(2)* Vành $ \mathbf{Z}/2\mathbf{Z} $ hiển nhiên là một trường.

Cho $ K $ là một trường. Mọi vành con $ L $ của $ K $ là một trường đều được gọi là một *trường con* của $ K $ và khi đó $ K $ được gọi là một *mở rộng trường* của $ L $; nói như vậy cũng tương đương với việc $ L $ là một vành con của $ K $ và $ x^{-1} \in L $ với mọi phần tử khác không $ x $ của $ L $. Nếu $ (L_i)_{i \in I} $ là một họ các trường con của $ K $, thì $ \bigcap_{i \in I} L_i $ là một trường con của $ K $; do đó, với mọi tập con $ X $ của $ K $, tồn tại một trường con nhỏ nhất của $ K $ chứa $ X $; trường này được gọi là *sinh bởi* $ X $.

#### Mệnh đề 1 {#alg-i-s9-prop-1 .statement}

*Cho $ K $ là một trường. Với mọi tập con $ X $ của $ K $, bộ tâm hóa (\S 8, no. 5, Ví dụ 3) $ X' $ của $ X $ là một trường con của $ K $.*

Ta biết (*loc. cit.*) rằng $ X' $ là một vành con của $ K $. Mặt khác, nếu $ x \neq 0 $ giao hoán với $ z \in X $, thì $ x^{-1} $ cũng vậy (I, \S 2, no. 3, Mệnh đề 5), và do đó $ X' $ chứa nghịch đảo của mọi phần tử khác không của $ X' $.

#### Hệ quả {#alg-i-s9-n1-cor-1 .statement}

*Tâm của một trường $ K $ là một trường con (giao hoán) của $ K $.*

#### Định lý 1 {#alg-i-s9-thm-1 .statement}

Cho $ \mathbf{A} $ là một vành. Các điều kiện sau là tương đương:

(a) $ \mathbf{A} $ là một trường;
(b) $ \mathbf{A} $ không chỉ gồm 0 và các iđêan trái duy nhất của $ \mathbf{A} $ là 0 và $ \mathbf{A} $.

Giả sử $ \mathbf{A} $ là một trường. Khi đó $ \mathbf{A} $ không chỉ gồm 0. Cho $ a $ là một iđêan trái của $ \mathbf{A} $ khác 0. Tồn tại một $ a $ khác không thuộc $ a $. Với mọi $ x \in \mathbf{A} $, $ x = (xa^{-1})a \in a $; do đó $ a = \mathbf{A} $.

Giả sử $ \mathbf{A} $ thỏa mãn điều kiện (b). Lấy $ x \neq 0 $ thuộc $ \mathbf{A} $. Ta cần chứng minh rằng $ x $ khả nghịch. Iđêan trái $ Ax $ chứa $ x $ và do đó không bằng không, suy ra $ Ax = \mathbf{A} $. Do đó tồn tại $ x' \in \mathbf{A} $ sao cho $ x'x = 1 $. Khi đó $ x' \neq 0 $ vì $ 1 \neq 0 $. Áp dụng kết quả trên cho $ x' $, ta thấy tồn tại $ x'' \in \mathbf{A} $ sao cho $ x''x' = 1 $. Khi đó $ x'' = x'' . 1 = x''x'x = 1 . x = x $, do đó $ xx' = 1 $. Vậy $ x' $ là nghịch đảo của $ x $.

#### Nhận xét {#alg-i-s9-n1-rem-1 .statement}

Trong Định lý 1, có thể thay các iđêan trái bằng các iđêan phải. Trong Chương VIII, § 5, no. 2, ta sẽ nghiên cứu các vành khác không $ \mathbf{A} $ không có iđêan *hai phía* nào khác 0 và $ \mathbf{A} $; các vành như vậy (gọi là *tựa đơn*) không nhất thiết là trường *(chẳng hạn, vành $ \mathbf{M}_2(\mathbf{Q}) $ các ma trận vuông cấp 2 với các hệ số hữu tỉ là tựa đơn nhưng không phải là trường)*.

#### Hệ quả 1 {#alg-i-s9-thm-1-cor-1 .statement}

Cho $ \mathbf{A} $ là một vành và $ a $ là một iđêan hai phía của $ \mathbf{A} $. Để vành $ \mathbf{A}/a $ là một trường, điều kiện cần và đủ là $ a $ là một iđêan trái cực đại của $ \mathbf{A} $.

Các iđêan trái của $ \mathbf{A}/a $ có dạng $ b/a $, trong đó $ b $ là một iđêan trái của $ \mathbf{A} $ chứa $ a $ ($ \S 8 $, no. 8, Hệ quả của Mệnh đề 5). Nói rằng $ \mathbf{A}/a \neq 0 $ có nghĩa là $ a \neq \mathbf{A} $. Với giả thiết này, $ \mathbf{A}/a $ là một trường khi và chỉ khi các iđêan trái duy nhất của $ \mathbf{A} $ chứa $ a $ là $ a $ và $ \mathbf{A} $ (Định lý 1), do đó có hệ quả.

#### Hệ quả 2 {#alg-i-s9-thm-1-cor-2 .statement}

Cho $ \mathbf{A} $ là một vành giao hoán khác 0. Tồn tại một đồng cấu của $ \mathbf{A} $ lên một trường giao hoán.

Theo Định lý của Krull ($ \S 8 $, no. 6, Định lý 1), tồn tại trong $ \mathbf{A} $ một iđêan cực đại $ a $. Khi đó $ \mathbf{A}/a $ là một trường (Hệ quả 1).

#### Hệ quả 3 {#alg-i-s9-thm-1-cor-3 .statement}

Cho $ a $ là một số nguyên $ \geqslant 0 $. Để vành $ \mathbf{Z}/a\mathbf{Z} $ là một trường, điều kiện cần và đủ là $ a $ là nguyên tố.

Điều này suy ra từ Hệ quả 1 và $ \S 8 $, no. 11.

Với $ p $ nguyên tố, trường $ \mathbf{Z}/p\mathbf{Z} $ được ký hiệu là $ \mathbf{F}_p $.

#### Định lý 2 {#alg-i-s9-thm-2 .statement}

Cho $ \mathbf{K} $ là một trường và $ \mathbf{A} $ là một vành khác không. Nếu $ f $ là một đồng cấu từ $ \mathbf{K} $ vào $ \mathbf{A} $, thì vành con $ f(\mathbf{K}) $ của $ \mathbf{A} $ là một trường và $ f $ xác định một đẳng cấu của $ \mathbf{K} $ lên $ f(\mathbf{K}) $.

Cho $ a $ là hạt nhân của $ f $. Khi đó $ 1 \notin a $ vì $ f(1) = 1 \neq 0 $ trong $ \mathbf{A} $ và, vì $ a $ là một iđêan trái của $ \mathbf{K} $, nên $ a = \{0\} $ theo Định lý 1. Do đó $ f $ là đơn ánh và do đó là một đẳng cấu của $ \mathbf{K} $ lên vành con $ f(\mathbf{K}) $ của $ \mathbf{A} $; vì vậy vành sau là một trường.

### 2. MIỀN NGUYÊN

#### Định nghĩa 2 {#alg-i-s9-def-2 .statement}

*Một vành $ \mathbf{A} $ được gọi là miền nguyên (hay miền toàn vẹn) nếu nó giao hoán, khác không, và tích của hai phần tử khác không của $ \mathbf{A} $ là khác không.*

Vành $ \mathbf{Z} $ các số nguyên hữu tỉ là một miền nguyên; nó giao hoán và khác không; tích của hai số nguyên $ > 0 $ là khác không; mọi số nguyên khác không đều có dạng $ a $ hoặc $ -a $ với $ a > 0 $ và $ (-a)b = -ab,\ (-a)(-b) = ab $ với $ a > 0,\ b > 0 $, do đó mệnh đề của chúng ta được chứng minh.

Mọi trường giao hoán đều là một miền nguyên. Một vành con của một miền nguyên là một miền nguyên. Đặc biệt, một vành con của một trường giao hoán là một miền nguyên. Ta sẽ chứng minh rằng ngược lại mọi miền nguyên $ \mathbf{A} $ đều đẳng cấu với một vành con của một trường giao hoán. Nhắc lại (\$ 8, no. 12) rằng $ \mathbf{A} $ đã được đồng nhất với một vành con của vành phân thức toàn phần của nó. Mệnh đề của chúng ta khi đó suy ra từ mệnh đề sau:

#### Mệnh đề 2 {#alg-i-s9-prop-2 .statement}

*Nếu $ \mathbf{A} $ là một miền nguyên, vành phân thức toàn phần $ \mathbf{K} $ của $ \mathbf{A} $ là một vành giao hoán.*

Vành $ \mathbf{K} $ là giao hoán. Nó khác không vì $ \mathbf{A} \neq \{0\} $. Vì $ \mathbf{A} $ là một miền nguyên, mọi phần tử khác không của $ \mathbf{A} $ đều giản ước được và $ \mathbf{K} $ gồm các phân thức $ a/b $ với $ b \neq 0 $. Bây giờ $ a/b \neq 0 $ kéo theo $ a \neq 0 $ và phân thức $ b/a $ khi đó là nghịch đảo của $ a/b $.

Vành phân thức toàn phần của một miền nguyên được gọi là *trường phân thức* của nó. Một vành như vậy được đồng nhất với ảnh của nó trong trường phân thức của nó.

#### Mệnh đề 3 {#alg-i-s9-prop-3 .statement}

*Cho $ \mathbf{B} $ là một vành khác không và $ \mathbf{A} $ là một vành con giao hoán của $ \mathbf{B} $ sao cho mọi phần tử khác không của $ \mathbf{A} $ đều khả nghịch trong $ \mathbf{B} $.
(a) $ \mathbf{A} $ là một miền nguyên.
(b) *Cho $ \mathbf{A}' $ là trường phân thức của $ \mathbf{A} $. Đơn ánh chính tắc của $ \mathbf{A} $ vào $ \mathbf{B} $ có thể được mở rộng duy nhất thành một đẳng cấu $ f $ của $ \mathbf{A}' $ lên một trường con của $ \mathbf{B} $.
(c) *Các phần tử của $ f(\mathbf{A}') $ là các $ xy^{-1} $ trong đó $ x \in \mathbf{A},\ y \in \mathbf{A},\ y \neq 0 $.*

Mệnh đề (a) là hiển nhiên. Đơn ánh chính tắc của $ \mathbf{A} $ vào $ \mathbf{B} $ mở rộng duy nhất thành một đồng cấu $ f $ của $ \mathbf{A}' $ vào $ \mathbf{B} $ (\$ 8, no. 12, Định lý 5). Mệnh đề (b) suy ra từ no. 1, Định lý 2. Các phần tử của $ \mathbf{A}' $ là các phân thức $ x/y $ với $ x \in \mathbf{A},\ y \in \mathbf{A},\ y \neq 0 $ và $ f(x/y) = xy^{-1} $, do đó (c).

### 3. IĐÊAN NGUYÊN TỐ

#### Mệnh đề 4 {#alg-i-s9-prop-4 .statement}

*Cho $ \mathbf{A} $ là một vành giao hoán và $ \mathfrak{p} $ là một iđêan của $ \mathbf{A} $. Các điều kiện sau là tương đương:
(a) *vành $ \mathbf{A}/\mathfrak{p} $ là một miền nguyên;
(b) $ \mathbf{A} \neq \mathfrak{p} $ và, nếu $ x \in \mathbf{A} - \mathfrak{p} $ và $ y \in \mathbf{A} - \mathfrak{p} $, thì $ xy \in \mathbf{A} - \mathfrak{p} $.
(c) $ \mathfrak{p} $ là hạt nhân của một đồng cấu của $ \mathbf{A} $ vào một trường.*

Các kéo theo (c) ⇒ (b) ⇒ (a) là hiển nhiên. Nếu $ A/p $ là một miền nguyên, gọi $ f $ là đơn ánh chính tắc của $ A/p $ vào trường phân thức của nó và $ g $ là đồng cấu chính tắc của $ A $ lên $ A/p $; khi đó $ p $ là hạt nhân của $ f \circ g $, do đó có kéo theo (a) ⇒ (c).

#### Định nghĩa 3 {#alg-i-s9-def-3 .statement}

*Trong một vành giao hoán $ A $, một iđêan $ p $ thỏa mãn các điều kiện của Mệnh đề 4 được gọi là một iđêan nguyên tố.*

#### Ví dụ {#alg-i-s9-n3-exa-1 .statement}

(1) Cho $ A $ là một vành giao hoán. Nếu $ m $ là một iđêan cực đại của $ A $, thì $ m $ là nguyên tố; vành $ A/m $ là một trường (no. 1, Hệ quả 1 của Định lý 1).

(2) Nếu $ A $ là một miền nguyên, iđêan $ \{0\} $ của $ A $ là nguyên tố (nhưng nói chung không cực đại, như ví dụ về vành $ \mathbf{Z} $ chứng tỏ).

### 4. TRƯỜNG CÁC SỐ HỮU TỈ

#### Định nghĩa 4 {#alg-i-s9-def-4 .statement}

*Trường phân thức của vành $ \mathbf{Z} $ các số nguyên hữu tỉ được gọi là trường các số hữu tỉ và được ký hiệu bởi $ \mathbf{Q} $. Các phần tử của $ \mathbf{Q} $ được gọi là các số hữu tỉ.*

Mọi số hữu tỉ do đó đều có dạng $ a/b $ trong đó $ a $ và $ b $ là các số nguyên hữu tỉ với $ b \neq 0 $ (và ta thậm chí có thể lấy $ b > 0 $ vì quan hệ

$$
a/b = (-a)/(-b)
$$

chứng minh điều đó). $ \mathbf{Q}_+ $ được dùng để ký hiệu tập hợp các số hữu tỉ có dạng $ a/b $ với $ a \in \mathbf{N} $ và $ b \in \mathbf{N}^* $.

Ta có các quan hệ:

(1) $$ \mathbf{Q}_+ + \mathbf{Q}_+ = \mathbf{Q}_+ $$
(2) $$ \mathbf{Q}_+ \cdot \mathbf{Q}_+ = \mathbf{Q}_+ $$
(3) $$ \mathbf{Q}_+ \cap (-\mathbf{Q}_+) = \{0\} $$
(4) $$ \mathbf{Q}_+ \cup (-\mathbf{Q}_+) = \mathbf{Q} $$
(5) $$ \mathbf{Q}_+ \cap \mathbf{Z} = \mathbf{N} $$

Hai quan hệ đầu tiên suy ra từ các công thức $ a/b + a'/b' = (ab' + a'b)/bb' $, $ (a/b)(a'/b') = aa'/bb' $, $ 0 \in \mathbf{Q}_+ $, $ 1 \in \mathbf{Q}_+ $ và thực tế rằng $ \mathbf{N} $ ổn định đối với phép cộng và phép nhân, còn $ \mathbf{N}^* $ ổn định đối với phép nhân. Hiển nhiên $ 0 \in \mathbf{Q}_+ $, do đó $ 0 \in (-\mathbf{Q}_+) $; cho $ x $ thuộc $ \mathbf{Q}_+ \cap (-\mathbf{Q}_+) $; khi đó tồn tại các số nguyên dương $ a, b, a', b' $ với $ b \neq 0,\ b' \neq 0 $ và $ x = a/b = -a'/b' $; khi đó $ ab' + ba' = 0 $, do đó $ ab' = 0 $ (vì $ ab' \geq 0 $ và $ ba' \geq 0 $) và do đó $ a = 0 $ vì $ b' \neq 0 $; nói cách khác, $ x = 0 $. Cuối cùng, hiển nhiên $ \mathbf{N} \subset \mathbf{Z} $ và $ \mathbf{N} \subset \mathbf{Q}_+ $. Ngược lại, nếu $ x $ thuộc $ \mathbf{Z} \cap \mathbf{Q}_+ $, thì nó là một số nguyên hữu tỉ; tồn tại hai số nguyên hữu tỉ $ a $ và $ b $ với $ a \geq 0,\ b > 0 $ và $ x = a/b $, do đó $ a = bx $; nếu $ x \notin \mathbf{N} $, thì $ -x > 0 $, do đó $ -a = b(-x) > 0 $ và do đó $ a < 0 $, trái với giả thiết.

Cho hai số hữu tỉ $ x $ và $ y $, ta viết $ x \leq y $ nếu $ y - x \in \mathbf{Q}_+ $. Từ các công thức (1), (3) và (4) dễ dàng suy ra rằng $ x \leq y $ là một thứ tự toàn phần trên

Q, từ (5), rằng quan hệ này cảm sinh quan hệ thứ tự thông thường trên Z. Cuối cùng, từ (1) suy ra rằng các quan hệ $ x \leq y $ và $ x' \leq y' $ kéo theo $ x + x' \leq y + y' $ và từ (2) rằng quan hệ $ x \leq y $ kéo theo $ xz \leq yz $ với mọi $ z \geq 0 $ và $ xz \geq yz $ với $ z \leq 0 $ (xem VI, § 2, no. 1).

Cho $ x $ là một số hữu tỉ. $ x $ được gọi là *dương* nếu $ x \geq 0 $, *dương ngặt* nếu $ x > 0 $, *âm* nếu $ x \leq 0 $ và *âm ngặt* nếu $ x < 0 $.† Tập hợp các số hữu tỉ dương là $ \mathbf{Q}_+ $ và tập hợp các số âm là $ -\mathbf{Q}_+ $. Nếu $ \mathbf{Q}^* $ ký hiệu tập hợp các số hữu tỉ khác không, thì tập hợp $ \mathbf{Q}_+^* $ các số dương ngặt bằng $ \mathbf{Q}^* \cap \mathbf{Q}_+ $ và $ -\mathbf{Q}_+^* $ là tập hợp các số âm ngặt.

Các tập hợp $ \mathbf{Q}_+^* $ và $ \{1, -1\} $ là các nhóm con của nhóm nhân $ \mathbf{Q}^* $. Mọi số hữu tỉ $ x \neq 0 $ đều biểu diễn được theo một và chỉ một cách dưới dạng $ 1.y, (-1).y $, trong đó $ y > 0 $; do đó nhóm nhân $ \mathbf{Q}^* $ là tích của các nhóm con $ \mathbf{Q}_+^* $ và $ \{1, -1\} $, thành phần của $ x $ trong $ \mathbf{Q}_+^* $ được gọi là *giá trị tuyệt đối* của $ x $ và được ký hiệu là $ |x| $; thành phần của $ x $ trong $ \{-1, 1\} $ (bằng 1 nếu $ x > 0 $, bằng $ -1 $ nếu $ x < 0 $) được gọi là *dấu* của $ x $ và được ký hiệu là $ \operatorname{sgn}\, x $.

Thông thường, hai hàm này được mở rộng lên toàn bộ $ \mathbf{Q} $ bằng cách đặt $ |0| = 0 $ và $ \operatorname{sgn}\, 0 = 0 $.

### Bài tập {#alg-i-s9-exercises}

Xem [các bài tập của § 9](exercises/s9/).
