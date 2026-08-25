---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 1
section_title: Uniform spaces
lang: vi
source: top-i-iv
pdf_pages: 0175-0180, 0212-0213
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A UNIFORM STRUCTURE
      page: 0
      pdf_page: 175
    - "no": 2
      title: TOPOLOGY OF A UNIFORM SPACE
      page: 0
      pdf_page: 177
statements: 13
exercises: 5
content_sha256: 63ab0c8bbee85469664f185818704ce4d2ca2bb0a05bfe19e141b99d7bd7fe36
translated_from: content/en/top/II/01_s1_uniform_spaces.md
source_content_sha256: 836a98a1f448d26c2dd28d696efabd443182ff29cecbdaa1f98458ad64ae6550
translation_model: gpt-5-6-mini
translation_run: translate-vi-e8f30170
glossary_version: 34
glossary_terms_sha256: fd1e7aa77e725250a5ad9b5b921eb1a578ee742ccfa661c189c6dc9b94d9a708
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. KHÔNG GIAN UNIFORM

### 1. ĐỊNH NGHĨA CẤU TRÚC UNIFORM

#### Định nghĩa 1 {#top-ii-s1-def-1 .statement}

*Một cấu trúc uniform* (hay *uniformity*) *trên một tập hợp* $ X $ *là một cấu trúc được cho bởi một tập hợp* $ \mathcal{U} $ *các tập con của* $ X \times X $ *thỏa mãn các tiên đề* $ (\mathrm{F}_1) $ *và* $ (\mathrm{F}_{\mathrm{II}}) $ *của Chương I, § 6, no. 1 và cũng thỏa mãn các tiên đề sau*:

(U₁) *Mọi tập hợp thuộc* $ \mathcal{U} $ *đều chứa đường chéo* $ \Delta $.

(U₂) *Nếu* $ V \in \mathcal{U} $ *thì* $ \overline{V}^{-1} \in \mathcal{U} $.

(U₃) *Với mỗi* $ V \in \mathcal{U} $ *tồn tại* $ W \in \mathcal{U} $ *sao cho* $ W \circ W \subset V $.

![Hình 2](../images/chapter_ii_uniform_structures.png)

Các tập hợp của $ \mathcal{U} $ được gọi là các lân cận của uniformity xác định trên $ X $ bởi $ \mathcal{U} $. Một tập hợp được trang bị một uniformity được gọi là một không gian uniform.

Nếu $ V $ là một lân cận của một uniformity trên $ X $, ta có thể biểu thị quan hệ $ (x, x') \in V $ bằng cách nói rằng "$ x $ và $ x' $ là $ V $-gần".

#### Nhận xét 1 {#top-ii-s1-n1-rem-1 .statement}

Để làm cho ngôn ngữ biểu đạt hơn, ta có thể sử dụng các biểu thức "$ x $ đủ gần với $ y $" và "$ x $ và $ y $ gần nhau tùy ý" trong một số mệnh đề. Chẳng hạn, ta sẽ nói rằng một quan hệ

R $ \{ x, y \} $ là đúng bất cứ khi nào $ x $ và $ y $ đủ gần nếu tồn tại một lân cận $ V $ sao cho quan hệ $ (x, y) \in V $ kéo theo $ R \{ x, y \} $.

#### Nhận xét 2 {#top-ii-s1-n1-rem-2 .statement}

Phép hội của các tiên đề (U_{II}) và (U_{III}) là tương đương (giả sử các tiên đề khác của các cấu trúc uniform) với tiên đề sau:

(U_a) Với mỗi $ V \in \mathcal{U} $ tồn tại $ W \in \mathcal{U} $ sao cho $ W \circ \overline{W} \subset V $ (*).

Rõ ràng (U_{II}) và (U_{III}) kéo theo (U_a). Ngược lại, nếu (U_a) được thỏa mãn thì ta có $ \overline{W} = \Delta \circ W \subset V $, bởi (U_I); do đó $ W \subset \overline{V} $ và vì vậy [bởi (F_1)] $ \overline{V} \in \mathcal{U} $. Đặt $ W' = W \cap \overline{W} $; khi đó $ W' \in \mathcal{U} $ bởi điều vừa được chứng minh và tiên đề (F_{II}), và ta có $ W' \circ W' \subset W \circ \overline{W} \subset V $.

Trong suốt chương này ta sẽ viết $ \overline{V}^2 $ thay cho $ V \circ V $, và nói chung $ \overline{V}^{n-1} = \overline{V} \circ V = V \circ \overline{V}^{n-1} $, với mỗi số nguyên $ n > 1 $ và mỗi tập con $ V $ của $ X \times X $.

#### Nhận xét 3 {#top-ii-s1-n1-rem-3 .statement}

Nếu $ X $ không rỗng, thì tiên đề (U_I) kéo theo rằng không có tập hợp nào của $ \mathcal{U} $ là rỗng, và do đó $ \mathcal{U} $ là một lọc trên $ X \times X $. Chỉ có một uniformity trên tập rỗng, đó là $ \mathcal{U} = \{ \emptyset \} $.

#### Định nghĩa 2 {#top-ii-s1-def-2 .statement}

Một hệ cơ sở các lân cận của một uniformity là bất kỳ tập hợp $ \mathcal{B} $ các lân cận nào sao cho mọi lân cận đều chứa một tập hợp thuộc $ \mathcal{B} $.

Tiên đề (U_{III}) cho thấy rằng nếu $ n $ là bất kỳ số nguyên $ > 0 $ nào và $ V $ chạy qua một hệ cơ sở các lân cận, thì các tập hợp $ \overline{V}^n $ lại tạo thành một hệ cơ sở các lân cận.

Các lân cận $ V $ sao cho $ V = \overline{V}^1 $ được gọi là đối xứng. Nếu $ V $ là một lân cận bất kỳ, thì $ V \cap \overline{V}^1 $ và $ V \cup \overline{V}^1 $ là các lân cận đối xứng, và các tiên đề (F_{II}) và (U_{II}) chỉ ra rằng các lân cận đối xứng tạo thành một hệ cơ bản các lân cận.

Một tập hợp $ \mathcal{B} $ các tập con của $ X \times X $ là một hệ cơ bản các lân cận của một cấu trúc đều trên $ X $ khi và chỉ khi $ \mathcal{B} $ thỏa mãn tiên đề (B_I) của Chương I, § 6, no. 3, và cũng thỏa mãn các tiên đề sau:

(U'_I) Mọi tập hợp của $ \mathcal{B} $ đều chứa đường chéo $ \Delta $.

(U'_II) Với mỗi $ V \in \mathcal{B} $ tồn tại $ V' \in \mathcal{B} $ sao cho $ V' \subset \overline{V}^1 $.

(U'_III) Với mỗi $ V \in \mathcal{B} $ tồn tại $ W \in \mathcal{B} $ sao cho $ \overline{W}^2 \subset V $.

Nếu $ X $ không rỗng, một hệ cơ bản các lân cận của một cấu trúc đều trên $ X $ là một cơ sở của bộ lọc được tạo bởi các lân cận của cấu trúc này (Chương I, § 6, no. 3, Mệnh đề 3).

(*) Ta nhắc lại (Lý thuyết tập hợp, R, § 3, các số 4 và 10) rằng nếu $ V $ và $ W $ là hai tập con của $ X \times X $, thì tập hợp các cặp $ (x, y) \in X \times X $, sao cho $ (x, z) \in W $ và $ (z, y) \in V $ với một $ z \in X $, được ký hiệu là $ V \circ W $ hoặc $ VW $, và rằng tập hợp các cặp $ (x, y) \in X \times X $ sao cho $ (y, x) \in V $ được ký hiệu là $ \overline{V}^1 $.

Các ví dụ về các cấu trúc đều. \* 1) Trên tập hợp $ \mathbf{R} $ các số thực ta có thể định nghĩa một cấu trúc đều, được gọi là *cấu trúc đều cộng tính*, như sau: với mỗi $ \alpha > 0 $ đặt $ V_\alpha $ là tập con của $ \mathbf{R} \times \mathbf{R} $ gồm tất cả các cặp $ (x, y) $ sao cho $ |x - y| < \alpha $; khi $ \alpha $ chạy qua tập hợp tất cả các số thực $ > 0 $, các $ V_\alpha $ tạo thành một hệ cơ bản các lân cận của cấu trúc đều cộng tính trên $ \mathbf{R} $. Tương tự ta có thể định nghĩa một cấu trúc đều (cũng được gọi là *cấu trúc đều cộng tính*) trên tập hợp $ \mathbf{Q} $ các số hữu tỉ; ta sẽ nghiên cứu các cấu trúc này, và các cấu trúc đều tương tự trên *các nhóm*, trong các Chương III và IV. \*
2) Cho $ X $ là một tập hợp và cho $ R $ là một *quan hệ tương đương* trên $ X $; gọi $ C $ là đồ thị của $ R $ trong $ X \times X $. Khi đó $ \Delta \subset C $ và $ \overset{2}{C} = \overset{-1}{C} = C $; (*Lý thuyết tập hợp, R, § 5, no. 1*); tập hợp các tập con của $ X \times X $ gồm riêng tập hợp $ C $ do đó là một hệ cơ bản các lân cận của một cấu trúc đều trên $ X $. Đặc biệt, nếu ta lấy $ R $ là quan hệ đẳng thức, thì $ C = \Delta $ và các lân cận của cấu trúc đều tương ứng là *tất cả các tập con* của $ X \times X $ chứa $ \Delta $; cấu trúc đều này được gọi là *cấu trúc đều rời rạc* trên $ X $, và tập hợp $ X $ được trang bị cấu trúc đều này được gọi là một *không gian đều rời rạc*.
3) Trên tập hợp $ \mathbf{Z} $ các số nguyên hữu tỉ ta có thể định nghĩa một cấu trúc đều, quan trọng trong lý thuyết số, như sau: cho một số nguyên tố $ p $, gọi $ W_n $ là tập hợp tất cả các cặp $ (x, y) \in \mathbf{Z} \times \mathbf{Z} $ sao cho $ x \equiv y \pmod{p^n} $, với mỗi số nguyên $ n > 0 $. Dễ dàng kiểm tra rằng các tập hợp $ W_n $ (với $ p $ cố định) tạo thành một hệ cơ bản các lân cận của một cấu trúc đều trên $ \mathbf{Z} $, được gọi là cấu trúc đều *$ p $-adic* (xem Chương III, § 6, các Bài tập 23 tiếp theo, và Chương IX, § 3, no. 2).

Theo các định nghĩa tổng quát (*Lý thuyết tập hợp, R, § 8, no. 5*), nếu $ X $ và $ X' $ là hai tập hợp mỗi tập được trang bị các cấu trúc đều mà các tập hợp các lân cận của chúng lần lượt là $ U $ và $ U' $, thì một song ánh $ f $ của $ X $ lên $ X' $ là một *đẳng cấu* của cấu trúc đều của $ X $ lên cấu trúc đều của $ X' $ nếu $ g(U) = U' $, trong đó $ g = f \times f $.

Chẳng hạn, nếu $ X $ và $ X' $ là hai tập hợp cùng lực lượng, thì mọi song ánh của $ X $ lên $ X' $ đều là một đẳng cấu của cấu trúc đều rời rạc của $ X $ lên cấu trúc đều rời rạc của $ X' $.

### 2. TÔPÔ CỦA MỘT KHÔNG GIAN ĐỀU

#### Mệnh đề 1 {#top-ii-s1-prop-1 .statement}

*Cho $ X $ là một tập hợp được trang bị một cấu trúc đều $ U $, và với mỗi $ x \in X $ ký hiệu $ \mathcal{B}(x) $ là tập hợp các tập con $ V(x) $ của $ X (*) $, trong đó $ V $ chạy qua tập hợp các lân cận của $ U $. Khi đó tồn tại duy nhất một tôpô trên $ X $ sao cho, với mỗi $ x \in X $, $ \mathcal{B}(x) $ là lọc lân cận của $ x $ trong tôpô này.*

Ta phải chứng minh rằng $ \mathcal{B}(x) $ thỏa mãn các điều kiện (V_I), (V_{II}), (V_{III}) và (V_{IV}) của Chương I, § 1, no. 2. Việc điều này đúng đối với ba điều kiện đầu tiên trong

(*) Ta nhắc lại (*Lý thuyết tập hợp, R, § 3, no. 7*) rằng nếu $ V $ là một tập con bất kỳ của $ X \times X $ và $ x $ là một phần tử bất kỳ của $ X $, thì $ V(x) $ ký hiệu tập hợp tất cả các $ y \in X $ sao cho $ (x, y) \in V $.

các điều kiện này suy ra ngay lập tức từ sự kiện rằng các lân cận của $ \mathcal{U} $ thỏa mãn $ (\mathbf{F}_I),\ (\mathbf{F}_{II}) $ và $ (\mathbf{U}_I) $. Đối với $ (\mathbf{V}_{IV}) $, cho $ V $ là một lân cận của $ \mathcal{U} $, $ W $ là một lân cận của $ \mathcal{U} $ sao cho $ \dot{W} \subset V $; khi đó nếu $ (x, y) \in W $ và $ (y, z) \in W $ thì ta có $ (x, z) \in V $, do đó $ W(y) \subset V(x) $ với mọi $ y \in W(x) $, và vì vậy $ V(x) \in \mathfrak{B}(y) $ với mọi $ y \in W(x) $. Điều này hoàn tất chứng minh.

#### Định nghĩa 3 {#top-ii-s1-def-3 .statement}

*Tôpô được xác định trong Mệnh đề 1 được gọi là tôpô cảm sinh bởi cấu trúc đều $ \mathcal{U} $.*

#### Ví dụ 1 {#top-ii-s1-n2-exa-1 .statement}

Tôpô cảm sinh bởi cấu trúc đều cộng tính trên tập hợp các số thực là tôpô của đường thẳng thực (Chương I, § 1, no. 2); tương tự, tôpô cảm sinh bởi cấu trúc đều cộng tính trên tập hợp các số hữu tỉ là tôpô của đường thẳng hữu tỉ.*
2) Trên một tập hợp bất kỳ $ X $, tôpô cảm sinh bởi cấu trúc đều rời rạc (no. 1, Ví dụ 2) là tôpô rời rạc.

Trong tương lai, khi nói về tôpô của một không gian đều $ X $, ta sẽ luôn hiểu đó là tôpô cảm sinh bởi cấu trúc đều của không gian, trừ khi điều ngược lại được phát biểu rõ ràng. Không gian tôpô thu được bằng cách đặt tôpô này trên tập hợp $ X $ đôi khi được gọi là không gian tôpô *nền tảng* của không gian đều đang xét. Chẳng hạn, khi ta nói rằng một không gian đều là *Hausdorff*, hoặc *compact*, hoặc *compact địa phương*, v.v., ta muốn nói rằng không gian tôpô nền tảng có tính chất này.

Nếu $ X $ và $ X' $ là hai không gian đều, mọi đẳng cấu $ f $ của cấu trúc đều của $ X $ lên cấu trúc đều của $ X' $ cũng là một *đồng phôi* của $ X $ lên $ X' $; ta nói rằng $ X $ là một *đẳng cấu* của không gian đều $ X $ lên không gian đều $ X' $. Cần lưu ý rằng một đồng phôi của $ X $ lên $ X' $ không nhất thiết là một đẳng cấu của cấu trúc đều của $ X $ lên cấu trúc đều của $ X' $.

Nói cách khác, các cấu trúc đều *phân biệt* trên cùng một tập hợp $ X $ có thể cảm sinh cùng một tôpô. *Chẳng hạn, trên ]0, +∞[, các cấu trúc đều *cộng tính* và *nhân tính* (là phân biệt: Chương III, § 6, Bài tập 17) cảm sinh cùng một tôpô.*
Một ví dụ khác xem § 2, no. 2, Nhận xét 1.

#### Mệnh đề 2 {#top-ii-s1-prop-2 .statement}

*Cho $ X $ là một không gian đều. Với mọi lân cận đối xứng $ V $ của $ X $ và mọi tập con $ M $ của $ X \times X $, $ VMV $ là một lân cận của $ M $ trong không gian tích $ X \times X $, và bao đóng của $ M $ trong không gian này được cho bởi công thức*

$$
\overline{M} = \bigcap_{V \in \mathcal{S}} VMV
$$

*trong đó $ \mathcal{S} $ ký hiệu tập hợp các lân cận đối xứng của $ X $.*

Cho $ V $ là một lân cận đối xứng của $ X $. Quan hệ $ (x, y) \in VMV $ có nghĩa là tồn tại một phần tử $ (p, q) $ của $ M $ sao cho $ (x, p) \in V $ và $ (q, y) \in V $: nói cách khác (do $ V $ đối xứng) $ x \in V(p) $ và $ y \in V(q) $, tức là $ (x, y) \in V(p) \times V(q) $. Vì $ V(p) \times X(q) $ là một lân cận của $ (p, q) $ trong $ X \times X $, phần đầu tiên của mệnh đề được chứng minh. Các quan hệ $ (x, p) \in V, (y, q) \in V $ cũng có thể được viết là $ p \in V(x), q \in V(y) $ hoặc $ (p, q) \in V(x) \times V(y) $. Khi $ V $ chạy qua $ \mathcal{S} $, các tập hợp $ V(x) \times V(y) $ tạo thành một hệ cơ bản các lân cận của $ (x, y) $ trong $ X \times X $; vì nếu $ U, U' $ là hai lân cận bất kỳ thì luôn tồn tại một lân cận đối xứng $ V \subset U \cap U' $, sao cho $ V(x) \times V(y) \subset U(x) \times U'(y) $. Do đó $ V(x) \times V(y) $ gặp $ M $ với mỗi $ V \in \mathcal{S} $ khi và chỉ khi $ (x, y) \in \overline{M} $, và công thức (1) suy ra.

#### Hệ quả 1 {#top-ii-s1-prop-2-cor-1 .statement}

*Nếu $ A $ là một tập con bất kỳ của $ X $ và $ V $ là một lân cận đối xứng bất kỳ của $ X $, thì $ V(A) $ là một lân cận của $ A $ trong $ X $, và*

$$
\overline{A} = \bigcap_{V \in \mathcal{S}} V(A) = \bigcap_{U \in \mathfrak{U}} V(A)
$$

*trong đó $ \mathfrak{U} $ ký hiệu tập hợp tất cả các lân cận trong $ X $.*

Nếu $ M = A \times A $, thì $ VMV = V(A) \times V(A) $ với mọi $ V \in \mathcal{S} $; vì quan hệ "tồn tại $ p \in A $ sao cho $ (x, p) \in V $ " theo định nghĩa tương đương với $ x \in V(A) $. Hệ quả bây giờ suy ra từ Chương I, § 4, số. 2, Mệnh đề 5 và số. 3, Mệnh đề 7.

$ V(A) $ được gọi là *lân cận-V của* $ A $.

Nếu $ V $ là một quan hệ lân cận *mở* trong $ X \times X $, thì $ V(x) $ là mở trong $ X $ với mỗi $ x \in X $ (Chương I, § 4, No. 2, Hệ quả của Mệnh đề 4) và do đó $ V(A) $, là hợp của các $ V(x) $ khi $ x $ chạy qua $ A $, là *mở* trong $ X $. Mặt khác, nếu $ V $ là một quan hệ lân cận đóng trong $ X \times X $, $ V(A) $ không nhất thiết đóng trong $ X $ với mọi tập con $ A $ của $ X $ (Bài tập 3).

Cũng cần nhận xét rằng khi $ V $ chạy qua tập hợp các quan hệ lân cận của $ X $, các tập hợp $ V(A) $ không nhất thiết tạo thành một hệ lân cận cơ bản của $ A $ trong $ X $ (Bài tập 2).

#### Hệ quả 2 {#top-ii-s1-prop-2-cor-2 .statement}

*Các phần trong (tương ứng, các bao đóng của) các quan hệ lân cận của $ X $ trong $ X \times X $ tạo thành một hệ các quan hệ lân cận cơ bản của $ X $.*

Nếu $ V $ là một quan hệ lân cận bất kỳ của $ X $, thì tồn tại một quan hệ lân cận đối xứng $ W $ sao cho $ W \subset V $; vì $ W $ là một lân cận của $ W $ (Mệnh đề 2), phần trong của $ V $ trong $ X \times X $ chứa $ W $ và do đó là một quan hệ lân cận. Hơn nữa, ta có $ W \subset W \subset W \subset V $ theo Mệnh đề 2, và do đó $ V $ chứa bao đóng của một quan hệ lân cận.

#### Hệ quả 3 {#top-ii-s1-prop-2-cor-3 .statement}

*Mọi không gian đều thỏa mãn tiên đề* $ (O_{III}) $.

#### Mệnh đề 3 {#top-ii-s1-prop-3 .statement}

*Một không gian đều $ X $ là Hausdorff khi và chỉ khi giao của tất cả các quan hệ lân cận của cấu trúc đều của nó là đường chéo $ \Delta $ của $ X \times X $. Mọi không gian đều Hausdorff đều chính quy.*

Mệnh đề sau đây suy ra ngay lập tức từ Hệ quả 3 của Mệnh đề 2. Ta đã thấy rằng các quan hệ lân cận đóng tạo thành một hệ các quan hệ lân cận cơ bản (Mệnh đề 2, Hệ quả 2); nếu giao của chúng là $ \Delta $, thì $ \Delta $ đóng trong $ X \times X $ và do đó $ X $ là Hausdorff (Chương I, § 8, No. 1, Mệnh đề 1). Ngược lại, nếu $ X $ là Hausdorff thì với mọi điểm $ (x, y) \notin \Delta $ tồn tại một quan hệ lân cận $ V $ của $ X $ sao cho $ y \notin V(x) $, hay tương đương $ (x, y) \notin V $; do đó $ \Delta $ là giao của tất cả các quan hệ lân cận.

Nếu một không gian đều $ X $ là Hausdorff, ta nói rằng cấu trúc đều của $ X $ là *Hausdorff*. Nếu $ \mathcal{B} $ là một hệ các quan hệ lân cận cơ bản của cấu trúc này; thì $ X $ là Hausdorff khi và chỉ khi giao của tất cả các tập hợp của $ \mathcal{B} $ là $ \Delta $.

### Bài tập {#top-ii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
