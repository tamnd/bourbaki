---
book: top
book_title: General Topology
chapter: VI
chapter_title: Real number spaces and projective spaces
section: 2
section_title: Euclidean distance, balls and spheres
lang: vi
source: top-v-x
pdf_pages: 0044-0050, 0064-0067
extraction: ocr
subsections:
    - "no": 1
      title: EUCLIDEAN DISTANCE IN $ \mathbf{R}^n $
      page: 0
      pdf_page: 44
    - "no": 2
      title: DISPLACEMENTS
      page: 0
      pdf_page: 45
    - "no": 3
      title: EUCLIDEAN BALLS AND SPHERES
      page: 0
      pdf_page: 46
    - "no": 4
      title: STEREOPHIC PROJECTION
      page: 0
      pdf_page: 48
statements: 12
exercises: 13
content_sha256: e6748e1c0ef8e9f42fd779e6865045e8deb53164e86282644f393ebc8ca088a6
translated_from: content/en/top/VI/02_s2_euclidean_distance_balls_and_spheres.md
source_content_sha256: c079d162d43af341a9f2928c20803b7b5597940eb20b9c983f7ce0bcd9e63c46
translation_model: gpt-5.4-mini
translation_run: translate-vi-499bfda2
glossary_version: 34
glossary_terms_sha256: 58f5bddfe79e5e6f6933b4bb81d895166194f03bad7e46f5a21d67b2bbd94fea
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. KHOẢNG CÁCH EUCLID; CÁC QUẢ CẦU VÀ MẶT CẦU

### 1. KHOẢNG CÁCH EUCLID TRONG $ \mathbf{R}^n $

Phù hợp với các định nghĩa chung, *khoảng cách Euclid* giữa hai điểm $ x = (x_i) $ và $ y = (y_i) $ là số

$$
d(x, y) = \sqrt{\sum_{i=1}^n (x_i - y_i)^2} \geq 0.
$$

Ta nhắc lại các tính chất chính của nó. Quan hệ $ d(x, y) = 0 $ tương đương với $ x = y $. Ta có $ d(x, y) = d(y, x) $; với mọi vô hướng $ t \in \mathbf{R} $, $ d(tx, ty) = |t| d(x, y) $; với mọi $ z \in \mathbf{R}^n $, $ d(x + z, y + z) = d(x, y) $; nói cách khác, khoảng cách giữa hai điểm là *bất biến qua phép tịnh tiến*. Khoảng cách $ d(o, x) $ từ gốc $ o $ đến một điểm $ x $ cũng được ký hiệu bởi $ \|x\| $ và được gọi là *chuẩn Euclid* của $ x $ (hay đơn giản là *chuẩn* của $ x $, khi không có nguy cơ nhầm lẫn; xem Chương IX, § 3, no. 3). Khi đó $ d(x, y) = \|y - x\| $.

Với $ n = 1 $, khoảng cách Euclid giữa các điểm $ x, y $ của $ \mathbf{R} $ quy về độ dài $ |y - x| $ của các khoảng có $ x $ và $ y $ làm đầu mút. Với mọi $ n $, ta nói rằng $ d(x, y) = \|y - x\| $ là *độ dài* của các đoạn có $ x $ và $ y $ làm đầu mút.

Khoảng cách Euclid thỏa mãn *bất đẳng thức tam giác*

(I)
$$
d(x, y) \leq d(x, z) + d(z, y)
$$
với mọi $ x, y, z $ trong $ \mathbf{R}^n $.

Ta nhắc lại rằng chứng minh của (I) quy về chứng minh bất đẳng thức

$$
\left( \sum_{i=1}^n (x_i + y_i)^2 \right)^{1/2} \leq \left( \sum_{i=1}^n x_i^2 \right)^{1/2} + \left( \sum_{i=1}^n y_i^2 \right)^{1/2};
$$

điều này lại tương đương với bất đẳng thức Cauchy-Schwarz

$$
\left( \sum_{i=1}^n x_i y_i \right)^2 \leq \left( \sum_{i=1}^n x_i^2 \right) \left( \sum_{i=1}^n y_i^2 \right),
$$

vốn là một hệ quả ngay lập tức của đẳng thức Lagrange

$$
\left( \sum_{i=1}^n x_i^2 \right) \left( \sum_{i=1}^n y_i^2 \right) - \left( \sum_{i=1}^n x_i y_i \right)^2 = \frac{1}{2} \sum_{i,j} (x_i y_j - x_j y_i)^2.
$$

Chứng minh này đồng thời cho thấy rằng hai vế của (1) chỉ có thể bằng nhau nếu $ z $ là một điểm của đoạn có $ x $ và $ y $ làm đầu mút.

Từ (1) suy ra bất đẳng thức

$$
d(x, y) \geq |d(x, z) - d(y, z)|.
$$

Cuối cùng, nếu $ x = (x_i), y = (y_i) $, ta có

$$
\sup_{1 \leq i \leq n} |x_i - y_i| \leq d(x, y) \leq \sqrt{n} \cdot \sup_{1 \leq i \leq n} |x_i - y_i|.
$$

Vì vậy, một tập con $ A $ của $ \mathbf{R}^n $ là *bị chặn* (\S 1, no. 1) khi và chỉ khi

$$
\sup_{x \in A} \|x\| < +\infty.
$$

### 2. CÁC PHÉP DỜI HÌNH

Ta nhắc lại một lần nữa rằng các biến đổi afin $ f $ của $ \mathbf{R}^n $ lên chính nó, làm *bất biến* khoảng cách giữa mọi hai điểm [nghĩa là sao cho $ d(f(x), f(y)) = d(x, y) $ với mọi $ x, y $], được gọi là *phép dời hình Euclid* (hay đơn giản là *phép dời hình*) (*); chúng tạo thành một nhóm, gọi là *nhóm các phép dời hình* của $ \mathbf{R}^n $. Nhóm này tác động bắc cầu lên $ \mathbf{R}^n $; nói chung hơn, nếu $ V $ và $ V' $ là hai đa tạp afin tuyến tính bất kỳ cùng chiều trong $ \mathbf{R}^n $, thì tồn tại một phép dời hình biến $ V $ thành $ V' $. Những phép dời hình giữ nguyên gốc, gọi là *phép biến đổi trực giao*, tạo thành một nhóm con của nhóm tất cả các phép dời hình. Nhóm con này được gọi là *nhóm trực giao* theo $ n $ biến thực; các ánh xạ tuyến tính thuộc nhóm này được đặc trưng bởi việc chúng làm bất biến *chuẩn* $ \|x\| $ của mọi điểm $ x \in \mathbf{R}^n $, hay, tương đương, *dạng bậc hai*

(*) Nếu $ f $ chỉ thỏa điều kiện $ d(f(x), f(y)) = d(x, y) $ với mọi $ x, y $, thì thực ra $ f $ phải là affine và tuyến tính, và do đó là một phép dời.

dạng $ \|x\|^2 = \sum_{i=1}^n x_i^2 $. Tích vô hướng của hai vectơ $ x = (x_i) $ và $ y = (y_i) $ của $ \mathbf{R}^n $ là giá trị $ \sum_{i=1}^n x_i y_i $ của dạng song tuyến tính liên kết với dạng toàn phương $ \sum_{i=1}^n x_i^2 $; nó được ký hiệu bởi $ (x|y) $, hay đơn giản là bởi $ xy $ nếu không có nguy cơ nhầm lẫn. Mọi phép biến đổi trực giao đều giữ bất biến tích vô hướng của bất kỳ hai vectơ nào. Hai vectơ $ x, y $ được gọi là trực giao nếu $ (x|y) = 0 $; hai không gian con vectơ $ V, V' $ của $ \mathbf{R}^n $ được gọi là trực giao nếu mỗi $ x \in V $ đều trực giao với mỗi $ y \in V' $; và hai đa tạp affine tuyến tính $ P, P' $ được gọi là trực giao nếu các không gian con vectơ song song lần lượt với $ P $ và $ P' $ là trực giao.

### 3. CÁC QUẢ CẦU VÀ MẶT CẦU EUCLID

Với mỗi số nguyên $ p > 0 $, ký hiệu $ U_p $ là tập hợp tất cả các cặp $ (x, y) $ gồm các điểm của $ \mathbf{R}^n $ sao cho $ d(x, y) < 1/p $; các bất đẳng thức (3) cho thấy các tập $ U_p $ tạo thành một hệ cơ bản của các lân cận trong cấu trúc đều của $ \mathbf{R}^n $ (xem Chương IX, § 2).

Từ तथ्य này và từ bất đẳng thức
$$
|d(x, y) - d(x', y')| \leq d(x, x') + d(y, y'),
$$
là hệ quả của (1), ta suy ra rằng $ d(x, y) $ là liên tục đều trên $ \mathbf{R}^n \times \mathbf{R}^n $; do đó chuẩn $ \|x\| = d(0, x) $ là liên tục đều trên $ \mathbf{R}^n $.

#### Định nghĩa 1 {#top-vi-s2-def-1 .statement}

Cho một điểm $ x_0 \in \mathbf{R}^n $ và một số thực $ r > 0 $, quả cầu Euclid mở (resp. đóng) có $ n $ chiều với tâm $ x_0 $ và bán kính $ r $ là tập hợp tất cả các điểm $ x \in \mathbf{R}^n $ sao cho $ d(x_0, x) < r $ [resp. $ d(x_0, x) \leq r $]; mặt cầu Euclid $ n - 1 $ chiều với tâm $ x_0 $ và bán kính $ r $ là tập hợp tất cả $ x \in \mathbf{R}^n $ sao cho $ d(x_0, x) = r $.

Khi không có nguy cơ nhầm lẫn, ta chỉ nói "quả cầu" (resp. "mặt cầu") thay cho "quả cầu Euclid" (resp. "mặt cầu Euclid"). Khi $ n = 2 $, một quả cầu hai chiều được gọi là một đĩa, và một mặt cầu một chiều được gọi là một đường tròn. Khi $ n = 1 $, quả cầu mở (resp. đóng) có tâm $ x_0 $ và bán kính $ r $ là khoảng $ ]x_0 - r, x_0 + r[ $ (resp. $ [x_0 - r, x_0 + r] $); mặt cầu có tâm $ x_0 $ và bán kính $ r $ là tập gồm hai đầu mút $ x_0 - r, x_0 + r $ của các khoảng này.

Từ những điều đã nói, các quả cầu (mở hay đóng) có tâm $ x_0 $ (hoặc chỉ những quả cầu có bán kính $ 1/p $, trong đó $ p $ chạy qua tập các số nguyên $ > 0 $) tạo thành một hệ cơ bản các lân cận của điểm $ x_0 $.

#### Mệnh đề 1 {#top-vi-s2-prop-1 .statement}

Mọi quả cầu mở (resp. đóng) của $ \mathbf{R}^n $ đều là một tập hợp mở (resp. compact). Bao đóng của một quả cầu mở là quả cầu đóng có cùng tâm và cùng bán kính; phần trong của một quả cầu đóng là quả cầu mở có cùng tâm và cùng bán kính.

Quả cầu mở (resp. đóng) có tâm $ x_0 $ và bán kính $ r $ là ảnh ngược của khoảng ]$-\infty, r[$ (resp. ]$-\infty, r]$) qua hàm liên tục $ d(x_0, x) $; do đó nó là mở (resp. đóng và bị chặn, nên compact). Nếu $ d(x_0, x) = r $, và nếu $ y = x_0 + t(x - x_0) $ ($ 0 < t < 1 $) là một điểm của đoạn mở có hai đầu mút $ x_0 $ và $ x $, ta có $ d(x_0, y) = tr < r $, và $ d(x, y) = (1 - t)r $ nhỏ tùy ý; suy ra $ x $ nằm trong bao đóng của quả cầu mở có tâm $ x_0 $ và bán kính $ r $. Lại nữa, nếu $ z = x + t(x - x_0) $ ($ t > 0 $) là một điểm của tia mở có gốc $ x $ và vectơ chỉ phương $ x - x_0 $, ta có
$$
d(x_0, z) = (1 + t)r > r,
$$
và $ d(x, z) = tr $ nhỏ tùy ý; do đó $ x $ không phải là một điểm trong của quả cầu đóng có tâm $ x_0 $ và bán kính $ r $.

#### Hệ quả {#top-vi-s2-n3-cor-1 .statement}

Mọi mặt cầu Euclid đều là một tập compact và là biên của các quả cầu mở và đóng có cùng tâm và cùng bán kính.

Ánh xạ $ x \to \frac{1}{r}(x - x_0) $ biến mặt cầu (resp. quả cầu mở, quả cầu đóng) có tâm $ x_0 $ và bán kính $ r $ thành mặt cầu (resp. quả cầu mở, quả cầu đóng) có tâm $ o $ và bán kính $ 1 $; mặt cầu này được ký hiệu bởi $ S_{n-1} $ và được gọi là mặt cầu đơn vị trong $ \mathbf{R}^n $. Tương tự, quả cầu đóng có tâm $ o $ và bán kính $ 1 $ được ký hiệu bởi $ B_n $ và được gọi là quả cầu đơn vị trong $ \mathbf{R}^n $. Do đó, việc khảo sát tôpô của một mặt cầu có $ (n - 1) $ chiều (resp. một quả cầu đóng có $ n $ chiều) được quy về việc khảo sát $ S_{n-1} $ (resp. $ B_n $). Đối với các quả cầu mở, ta có mệnh đề sau:

#### Mệnh đề 2 {#top-vi-s2-prop-2 .statement}

Mọi quả cầu mở $ n $-chiều đều đồng phôi với $ \mathbf{R}^n $.

Thật vậy, ánh xạ $ x \to \frac{x}{1 + ||x||} $ liên tục trên $ \mathbf{R}^n $ và ánh xạ $ \mathbf{R}^n $ lên quả cầu mở có tâm $ o $ và bán kính $ 1 $; hơn nữa, từ $ y = \frac{x}{1 + ||x||} $ suy ra $ x = \frac{y}{1 - ||y||} $, nên ánh xạ là song ánh và song liên tục.

Ký hiệu $ \mathbf{R}_n^* $ là phần bù của $ o $ trong $ \mathbf{R}^n $.

#### Mệnh đề 3 {#top-vi-s2-prop-3 .statement}

Không gian $ \mathbf{R}_n^* $ đồng phôi với tích của $ S_{n-1} $ và không gian $ \mathbf{R}_+^* $ của các số thực $ > 0 $.

Mọi điểm $ x \neq o $ đều có thể được viết duy nhất dưới dạng $ tz $, với $ t > 0 $ và $ ||z|| = 1 $, vì $ x = tz $ suy ra $ t = ||x|| $ và $ z = x/||x|| $. Vì $ tz $ liên tục trên tích $ \mathbf{R} \times \mathbf{R}^n $ và do đó *a fortiori* trên $ \mathbf{R}_+^* \times S_{n-1} $, và vì $ ||x|| $ và $ \frac{1}{||x||} $ liên tục trên $ \mathbf{R}_n^* $, mệnh đề được chứng minh.

Đánh xạ $ x \to x/||x|| $ được gọi là *phép chiếu tâm* của $ \mathbf{R}_n^* $ lên $ S_{n-1} $. Người ta cũng định nghĩa theo cùng một cách *phép chiếu tâm* của phần bù của một điểm $ a $ lên một mặt cầu tâm $ a $.

#### Hệ quả 1 {#top-vi-s2-prop-3-cor-1 .statement}

*Mặt cầu* $ S_{n-1} $ *đồng phôi với thương của* $ \mathbf{R}_n^* $ *theo quan hệ tương đương mà các lớp là các tia mở có gốc* $ o $.

Những lớp này cũng có thể được định nghĩa là các *lớp quỹ đạo*, khác $ \{ o \} $, của nhóm các phép vị tự tỉ số $ > 0 $.

#### Hệ quả 2 {#top-vi-s2-prop-3-cor-2 .statement}

*Không gian* $ \mathbf{R}_n^* $ *đồng phôi với* $ \mathbf{R} \times S_{n-1} $.

Vì $ \mathbf{R}_+^* = ]0, +\infty[ $ đồng phôi với $ \mathbf{R} $ (Chương IV, § 4, No. 1, Mệnh đề 1).

#### Nhận xét {#top-vi-s2-n3-rem-1 .statement}

Những mệnh đề này không chỉ riêng đối với các quả cầu Euclid, mà còn có thể được mở rộng cho cả một lớp các lân cận compact của $ o $ trong $ \mathbf{R}^n $ (xem Bài tập 12).

Các tập hợp $ S_{n-1} $ và $ B_n $ hiển nhiên bất biến dưới mọi phép biến đổi trực giao. Nếu $ V $ là một không gian con vectơ $ p $ chiều trong $ \mathbf{R}^n $, tồn tại một phép biến đổi trực giao biến $ V $ thành một không gian con tọa độ $ p $ chiều; do đó $ V \cap S_{n-1} $ (tương ứng $ V \cap B_n $) đồng phôi với $ S_{p-1} $ (tương ứng $ B_p $).

### 4. PHÉP CHIẾU LẬP THỂ

Xét điểm $ e_n = (0, \ldots, 0, 1) $ của $ S_{n-1} $, và siêu phẳng $ H $ có phương trình $ x_n = 0 $, vuông góc với vectơ $ e_n $. Với mỗi điểm $ x = (x_i) $ của $ S_{n-1} $, khác $ e_n $, ta ứng với điểm $ y $ là giao điểm của đường thẳng đi qua $ e_n $ và $ x $ với siêu phẳng $ H $ (Hình 3). Dễ dàng kiểm tra rằng ta có

$$
y = \frac{1}{1 - x_n} (x - x_n e_n)
$$

và

$$
x = \frac{||y||^2 - 1}{||y||^2 + 1} e_n + \frac{2}{||y||^2 + 1} y.
$$

![Sơ đồ minh họa phép chiếu lập thể](https://i.imgur.com/3Q5z5QG.png)

Hình 3.

==========

Nếu ký hiệu bởi $ A $ phần bù của $ \{ e_n \} $ trong $ S_{n-1} $, thì các công thức này cho thấy như vậy ta đã xác định một đồng phôi của $ A $ lên siêu phẳng $ H $. Đồng phôi này được gọi là phép chiếu lập thể của $ A $ lên $ H $, hay (theo lối nói quen) của $ S_{n-1} $ lên $ H $; $ e_n $ là đỉnh của phép chiếu, $ H $ là siêu phẳng chiếu. Tổng quát hơn, nếu $ H' $ là bất kỳ siêu phẳng nào đi qua $ o $ (một siêu phẳng đường kính của $ B_n $) và nếu $ a $ là một trong các điểm giao của $ S_{n-1} $ với đường thẳng vuông góc với $ H' $ đi qua $ o $, ta có thể định nghĩa theo cùng cách phép chiếu lập thể với đỉnh $ a $ lên siêu phẳng chiếu $ H' $; trong mọi trường hợp, phép chiếu này có thể được đưa về phép chiếu trước đó bằng một phép biến đổi trực giao biến $ H' $ thành $ H $ và $ a $ thành $ e_n $.

#### Mệnh đề 4 {#top-vi-s2-prop-4 .statement}

*Nếu $ n > 1 $, hình cầu Euclid $ S_{n-1} $ đồng phôi với không gian $ \mathbf{R}^{n-1} $ được làm compact bằng cách ghép thêm một "điểm ở vô cực"*(Chương I, § 9, no. 8, Định lý 4).

Vì phép chiếu lập thể xác định một đồng phôi của phần bù của một điểm trong $ S_{n-1} $ lên một siêu phẳng của $ \mathbf{R}^n $, mà siêu phẳng ấy đồng phôi với $ \mathbf{R}^{n-1} $.

#### Hệ quả 1 {#top-vi-s2-prop-4-cor-1 .statement}

*Hình cầu $ S_n $ đồng phôi với không gian thương của quả cầu $ B_n $ thu được bằng cách đồng nhất tất cả các điểm của hình cầu $ S_{n-1} $*.

Quả cầu $ B_n $ là một không gian chính quy (Chương I, § 8, no. 4); do đó không gian thương $ F $ của $ B_n $ thu được bằng cách đồng nhất tất cả các điểm của $ S_{n-1} $ là *Hausdorff* (Chương I, § 8, no. 6, Mệnh đề 15). Vì $ B_n $ compact, nên $ F $ cũng compact, và do đó $ F $ đồng phôi với một quả cầu mở $ n $ chiều được làm compact bằng cách ghép thêm một điểm ở vô cực, theo định lý của Alexandroff (Chương I, § 9, no. 8, Định lý 4). Kết quả vì thế suy ra từ Mệnh đề 2 và 4.

#### Hệ quả 2 {#top-vi-s2-prop-4-cor-2 .statement}

*Đường tròn $ S_1 $ đồng phôi với xuyến $ T $*.

Trong Chương VIII, § 2, no. 1, ta sẽ lại thu được kết quả này như một hệ quả của một định lý chính xác hơn.

#### Mệnh đề 5 {#top-vi-s2-prop-5 .statement}

*Nếu $ n > 1 $, hình cầu Euclid $ S_{n-1} $ liên thông và liên thông địa phương, và mọi điểm của nó đều có một lân cận mở đồng phôi với $ \mathbf{R}^{n-1} $.*

Phần bù của một điểm trong $ S_{n-1} $ là một tập hợp trù mật liên thông, và do đó (Chương I, § 11, no. 1, Mệnh đề 1) $ S_{n-1} $ liên thông. Để thấy rằng mỗi điểm đều có một lân cận đồng phôi với $ \mathbf{R}^{n-1} $, ta chỉ cần chiếu lập thể từ một đỉnh khác với điểm đã cho.

Từ mệnh đề này và từ Mệnh đề 3 của no. 3 suy ra rằng $ \mathbf{R}_n^* $, là tích của hai không gian liên thông, nên liên thông (Chương I, § 11, no. 4, Mệnh đề 8; xem § 1, Bài tập 10).

Giao của $ S_{n-1} $ với một nửa không gian đóng (tương ứng mở) được xác định bởi một siêu phẳng đường kính của $ B_n $ được gọi là một *bán cầu đóng* (tương ứng *bán cầu mở*) của $ S_{n-1} $. Bằng phép chiếu lập thể lên siêu phẳng đường kính, bán cầu đóng (tương ứng bán cầu mở) không chứa đỉnh chiếu được ánh xạ lên một *quả cầu đóng* (tương ứng *quả cầu mở*) $ n - 1 $ chiều, nên do đó nó *đồng phôi* với nó.

Nếu $ n = 2 $, ta nói "nửa đường tròn" thay vì "bán cầu".

### Bài tập {#top-vi-s2-exercises}

Xem [bài tập cho § 2](exercises/s2/).

==========
