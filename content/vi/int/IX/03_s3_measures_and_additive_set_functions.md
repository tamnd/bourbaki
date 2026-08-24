---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 3
section_title: Measures and additive set functions
lang: vi
source: int-vii-ix
book_pages: INT IX.41-INT IX.49, INT IX.108-INT IX.112
pdf_pages: 0223-0231, 0290-0294
extraction: ocr
subsections:
    - "no": 1
      title: Measures and additive set functions of compact sets
      page: 41
      pdf_page: 223
    - "no": 2
      title: Inner regular set functions
      page: 44
      pdf_page: 226
    - "no": 3
      title: Radon spaces
      page: 46
      pdf_page: 228
statements: 11
exercises: 18
content_sha256: e9f956b39521a90d7f06c0d54766dc95dd7c2b13c57e70c9f20b396f1637d989
translated_from: content/en/int/IX/03_s3_measures_and_additive_set_functions.md
source_content_sha256: 9f804be3c07f04ffa908e1c9375a7fe2ea3976b356b3a4f02273e2e005639ec8
translation_model: gpt-5.4
translation_run: translate-vi-6850220c
glossary_version: 34
glossary_terms_sha256: 7a7b9c23d830293e8157c2d7073b332db7cd8a25f1522ec28942b86f3ba2ab08
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ĐỘ ĐO VÀ CÁC HÀM TẬP HỢP CỘNG TÍNH

Trong tiết này, tương ứng ta sẽ ký hiệu bởi $ \mathcal{K}(T) $ và $ \mathcal{B}(T) $ tập hợp các tập con compact của một không gian tôpô Hausdorff T và bộ tộc Borel của T.

### 1. Độ đo và các hàm tập hợp cộng tính của các tập compact

#### Định lý 1 {#int-ix-s3-thm-1 .statement}

— Cho T là một không gian tôpô, và I một ánh xạ từ $ \mathcal{K}(T) $ vào $ \mathbf{R}_+ $. Điều kiện cần và đủ để tồn tại một độ đo $ \mu $ trên T sao cho $ I(K) = \mu^\bullet(K) $ với mọi $ K \in \mathcal{K}(T) $ là I thỏa mãn các điều kiện sau:

1) Nếu K và L là các tập con compact của T sao cho $ K \subset L $, thì $ I(K) \leq I(L) $ ('I tăng').

2) Nếu K và L là các tập con compact của T, thì $ I(K \cup L) \leq I(K) + I(L) $.

3) Nếu K và L là các tập con compact rời nhau của T, thì $ I(K \cup L) = I(K) + I(L) $ ('I cộng tính').

4) Với mọi họ có hướng giảm $ (K_\alpha)_{\alpha \in A} $ gồm các tập con compact của T, ta có $ I(\bigcap_{\alpha \in A} K_\alpha) = \inf_{\alpha \in A} I(K_\alpha) $.

5) Với mọi $ x \in T $, tồn tại một lân cận V của x sao cho
$$
\sup_{\substack{K \in \mathcal{K}(T) \\ K \subset V}} I(K) < +\infty
$$
('I bị chặn địa phương').

Khi đó độ đo $ \mu $ là duy nhất.

Tính duy nhất của $ \mu $ suy ra từ Hệ quả của Mệnh đề 2 của \S 1, No. 2. Các điều kiện trên là cần thiết, ba điều kiện đầu theo cách hiển nhiên, điều kiện cuối cùng do việc $ \mu^\bullet $ là một encumbrance bị chặn địa phương, và điều kiện 4) theo Hệ quả của Mệnh đề 5 của \S 1, No. 6.

Để chỉ ra rằng các điều kiện này là đủ, trước hết ta xét trường hợp T compact.

#### Bổ đề 1 {#int-ix-s3-lem-1 .statement}

— Giả sử rằng T compact, và đặt l = I(T). Với mọi $ A \subset T $, đặt

$$
J(A) = \sup_{\substack{K \in \mathcal{K}(T) \\ K \subset A}} I(K)
$$

và gọi $ \Phi $ là tập hợp các $ A \subset T $ sao cho $ J(A) + J(\mathbf{C}A) = l $. Khi đó tập hợp $ \Phi $ là một họ chứa $ \mathcal{K}(T) $, và hàm $ J $ trên $ \Phi $ là tăng và cộng tính.

Hiển nhiên là $ J $ là một hàm tập hợp tăng, mở rộng $ I $, và rằng $ J(A) + J(\mathbf{C}A) \leq l $ với mọi $ A \subset T $.

Cho $ K $ và $ S $ là hai tập compact trong $ T $; trước hết ta sẽ chỉ ra rằng

$$
J(K \cap S) + J(\mathbf{C}K \cap S) = J(S).
$$

Khi xét các hạn chế của $ I $ lên $ \mathcal{K}(S) $ và của $ J $ lên $ \mathfrak{P}(S) $, người ta quy ngay lập tức về trường hợp $ S = T $. Vì $ T $ là chuẩn tắc, $ K $ là giao của họ có hướng giảm các lân cận compắc của nó, và điều kiện 4) kéo theo sự tồn tại, với mọi $ \varepsilon > 0 $, của một lân cận compắc $ H $ của $ K $ sao cho $ I(H) \leq I(K) + \varepsilon $. Gọi $ L $ là bao đóng của $ T - H $; $ L $ là compắc, $ L \cap K = \varnothing $ và $ H \cup L = T $, do đó $ l = I(H \cup L) \leq I(H) + I(L) \leq I(K) + I(L) + \varepsilon $ (điều kiện 2)), từ đó có quan hệ $ J(K) + J(\mathbf{C}K) \geq I(K) + I(L) \geq l - \varepsilon $. Vì $ \varepsilon $ là tùy ý, $ J(K) + J(\mathbf{C}K) = l $. Điều này chứng minh công thức (2), cũng như sự bao hàm $ \mathcal{K}(T) \subset \Phi $.

Bây giờ chứng minh rằng $ \Phi $ là một clan. Vì $ \Phi $ hiển nhiên ổn định khi lấy phần bù, nên chỉ cần chỉ ra rằng nếu $ A_1 $ và $ A_2 $ là các phần tử của $ \Phi $, thì $ A_1 \cup A_2 \in \Phi $, hay cũng có nghĩa là

$$
J(A_1 \cup A_2) + J(\mathbf{C}(A_1 \cup A_2)) \geq l.
$$

Ký hiệu bởi $ \varepsilon $ một số $ > 0 $, và, với $ i = 1, 2 $, gọi $ K_i $ là một tập compact được chứa trong $ A_i $, và $ L_i $ là một tập compact được chứa trong $ \mathbf{C}A_i $, sao cho

$$
I(K_i) \geq J(A_i) - \varepsilon, \quad I(L_i) \geq J(\mathbf{C}A_i) - \varepsilon.
$$

Đặt $ M_1 = K_1 \cup L_1 $; các quan hệ $ l = J(M_1) + J(\mathbf{C}M_1) $ và

$$
J(M_1) = I(K_1) + I(L_1) \geq J(A_1) + J(\mathbf{C}A_1) - 2\varepsilon = l - 2\varepsilon
$$

suy ra rằng $ J(\mathbf{C}M_1) \leq 2\varepsilon $. Khi đó nếu $ S $ là một tập con compắc của $ T $, quan hệ (2) (áp dụng cho $ K = M_1 $) suy ra $ J(S) \leq J(M_1 \cap S) + 2\varepsilon $, do đó

$$
J(S) \leq J(K_1 \cap S) + J(L_1 \cap S) + 2\varepsilon.
$$

Hãy cộng các bất đẳng thức thu được khi lấy $ S = K_2 $ và $ S = L_2 $, đồng thời tính đến bất đẳng thức $ J(K_2) + J(L_2) \geq l - 2\varepsilon $ và thực tế rằng $ K_1 \cap K_2 $, $ L_1 \cap K_2 $ và $ K_1 \cap L_2 $ là ba tập compact rời nhau được chứa trong $ A_1 \cup A_2 $. Ký hiệu $ C $ là hợp của ba tập compact này, suy ra rằng

$$
l - 2\varepsilon \leq J(K_2) + J(L_2) \leq J(C) + J(L_1 \cap L_2) + 4\varepsilon \\
\leq J(A_1 \cup A_2) + J(\mathcal{C}(A_1 \cup A_2)) + 4\varepsilon,
$$

do đó ngay lập tức có công thức cần tìm (3), xét đến tính tùy ý của $ \varepsilon $. Sau khi điều này đã được thiết lập, các bất đẳng thức trước đó kéo theo rằng $ J(C) \geq J(A_1 \cup A_2) - 6\varepsilon $; nếu $ A_1 $ và $ A_2 $ rời nhau, thì $ C $ là hợp của $ K_1 \cap L_2 \subset A_1 $ và $ K_2 \cap L_1 \subset A_2 $, từ đó suy ra rằng $ J(A_1 \cup A_2) \leq J(A_1) + J(A_2) $. Vì bất đẳng thức ngược lại là hiển nhiên, $ J $ quả thật là cộng tính trên $ \Phi $, và bổ đề được thiết lập.

Hãy hoàn tất chứng minh định lý trong trường hợp $ T $ compact. Gọi $ \mathcal{E}(\Phi) $ là không gian vectơ các hàm bậc thang theo $ \Phi $ trên $ T $, được trang bị tôpô hội tụ đều (Ch. IV, §4, No. 9, Def. 4); ta lại ký hiệu bởi $ J $ dạng tuyến tính dương trên $ \mathcal{E}(\Phi) $ liên kết với hàm cộng tính $ J $ (loc. cit., Prop. 18). Vì $ J(T) = l $, $ J $ liên tục và có chuẩn bằng $ l $. Khi đó gọi $ \mathcal{H} $ là bao đóng của $ \mathcal{E}(\Phi) $ đối với tôpô hội tụ đều; kiểm tra ngay được rằng $ J $ có thể được kéo dài bằng tính liên tục thành một dạng tuyến tính *dương* trên $ \mathcal{H} $, vẫn ký hiệu là $ J $. Vì $ \mathcal{H} $ chứa $ \mathcal{C}(T) $ (loc. cit., No. 10, Prop. 19), hạn chế của $ J $ trên $ \mathcal{C}(T) $ là một độ đo dương $ \mu $. Còn phải chứng minh rằng $ \mu^\bullet(K) = I(K) $ với mọi tập con compact $ K $ của $ T $. Bây giờ, ta có $ \mu^\bullet(K) = \inf_{f \in S_K} \mu^\bullet(f) $, trong đó $ S_K $ ký hiệu tập hợp các phần tử của $ \mathcal{C}(T) $ mà $ \geq \varphi_K $ (\S1, No. 6, Prop. 5). Vì $ J(f) = \mu^\bullet(f) $ với $ f \in \mathcal{C}(T) $, rõ ràng chỉ cần chứng minh rằng $ J(K) \geq \inf_{f \in S_K} J(f) $. Như trong chứng minh của Bổ đề 1, gọi $ H $ là một lân cận compact của $ K $ sao cho $ J(H) \leq J(K) + \varepsilon $, và gọi $ f $ là một hàm liên tục trên $ T $, nhận giá trị giữa 0 và 1, bằng 1 trên $ K $ và bằng 0 ở ngoài $ H $ (GT, IX, §4, No. 1, Prop. 1). Khi đó

$$
J(f) \leq J(H) \leq J(K) + \varepsilon;
$$

vì $ \varepsilon $ là tùy ý, bất đẳng thức cần chứng minh được chứng tỏ, và do đó định lý được thiết lập khi $ T $ là compact.

Bây giờ ta chuyển sang trường hợp tổng quát. Với mọi tập compact $ L $ trong $ T $, ký hiệu $ I_L $ là hạn chế của $ I $ lên $ \mathfrak{K}(L) $. Theo trường hợp riêng vừa xét, tồn tại một độ đo $ \mu_L $ trên $ L $, duy nhất, sao cho $ \mu_L(K) = I_L(K) $ với mọi tập compact $ K \subset L $. Bây giờ cho $ L' $ là một tập compact được chứa trong $ L $; ta có $ (\mu_L)_{L'}^\bullet(K) = \mu_{L'}^\bullet(K) = \mu_{L'}^\bullet(K) $ với mọi tập compact $ K \subset L' $, do đó $ \mu_{L'} = (\mu_L)_{L'} $; ánh xạ $ \mu : L \mapsto \mu_L $ là một tiền độ đo. Điều kiện 5) biểu thị rằng $ \mu $ là một độ đo, và quan hệ $ I(K) = \mu^*(K) $ với mọi tập compact $ K \subset T $ là hiển nhiên.

#### Nhận xét {#int-ix-s3-n1-rem-1 .statement}

— 1) Điều kiện 4) có thể được thay thế, trong phát biểu của Định lý 1, bởi điều kiện sau đây ("liên tục phải"):
$ 4') $ Với mọi $ K \in \mathcal{K}(T) $ và mọi $ \varepsilon > 0 $, tồn tại một tập mở $ U $ chứa $ K $, sao cho $ I(H) \leq I(K) + \varepsilon $ với mọi tập compact $ H \subset U $.
Thật vậy, nếu $ \mu $ là một độ đo, hàm $ I : K \mapsto \mu^*(K) $ thỏa mãn $ 4' $ (\S 1, No. 9, Mệnh đề 13). Ngược lại, giả sử rằng $ I $ thỏa mãn 1) và $ 4' $; hãy chứng tỏ rằng khi đó $ I $ thỏa mãn 4). Với các ký hiệu như trong phát biểu của Định lý 1, chọn một $ \varepsilon > 0 $ và một tập mở $ U $ chứa tập compact $ K = \bigcap_{\alpha \in A} K_\alpha $ và sao cho $ 4' $) được thỏa mãn. Khi đó tồn tại một chỉ số $ \beta \in A $ sao cho $ K_\beta \subset U $, và điều này suy ra
$$
\inf_{\alpha \in A} I(K_\alpha) \leq I(K_\beta) \leq I(K) + \varepsilon
$$
và 4) quả thật được thỏa mãn.
2) Hệ các điều kiện 2) và 3) có thể được thay thế, trong phát biểu của Định lý 1, bởi điều kiện sau đây:
Nếu $ K $ và $ L $ là các tập con compact của $ T $, thì
$$
I(K \cup L) + I(K \cap L) = I(K) + I(L).
$$
Thật vậy, điều kiện này kéo theo 2) và 3), và mặt khác
$$
\mu^*(K \cup L) = \mu^*(K \cap L) = \mu^*(K) + \mu^*(L)
$$
đối với mọi độ đo $ \mu $, do quan hệ $ \varphi_{K \cup L} + \varphi_{K \cap L} = \varphi_K + \varphi_L $ giữa các hàm đặc trưng.

### 2. Các hàm tập hợp chính quy nội

Định nghĩa 1. — Cho $ T $ là một không gian tôpô, và $ \mathcal{B}(T) $ là bộ tộc Borel của $ T $; cho $ I $ là một ánh xạ từ $ \mathcal{B}(T) $ vào $ \overline{\mathbf{R}}_+ $.
a) $ I $ được gọi là cộng tính đếm được nếu, với mọi dãy $ (A_n) $ gồm các phần tử của $ \mathcal{B}(T) $ rời nhau từng đôi một,
$$
I\left( \bigcup_n A_n \right) = \sum_n I(A_n).
$$
b) $ I $ được gọi là chính quy nội nếu, với mọi tập hợp $ A \in \mathcal{B}(T) $,
$$
I(A) = \sup_K I(K),
$$
trong đó $ K $ chạy qua tập hợp các tập con compac của $ A $.

c) I được gọi là bị chặn (tương ứng, bị chặn địa phương) nếu $ I(T) < +\infty $ (tương ứng, nếu mọi điểm $ x \in T $ đều có một lân cận mở $ V $ sao cho $ I(V) < +\infty $).

#### Nhận xét {#int-ix-s3-n2-rem-1 .statement}

— 1) Điều kiện a) rõ ràng kéo theo rằng I là một ánh xạ tăng từ $ \mathcal{B}(T) $ (được sắp thứ tự bởi quan hệ bao hàm) vào $ \overline{\mathbf{R}}_+ $.

2) Giả sử rằng I là cộng tính đếm được; gọi $ (A_n)_{n \in \mathbf{N}} $ là một dãy tăng các tập hợp Borel, và đặt $ A = \bigcup_{n \in \mathbf{N}} A_n $. Các tập hợp $ D_0 = A_0 $, $ D_n = A_n - A_{n-1} $ rời nhau từng đôi một, và hợp của chúng là A, nên ta có $ I(A) = \sum_n I(D_n) = \lim_{n \to \infty} I(A_n) $. Tương tự, nếu $ (B_n) $ là một dãy giảm các tập hợp Borel, và nếu $ I(B_0) < +\infty $, thì $ I(\bigcap_n B_n) = \lim_{n \to \infty} I(B_n) $: chỉ cần áp dụng điều trên cho các tập hợp $ A_n = B_0 - B_n $.

3) Cho $ (A_n) $ là một dãy bất kỳ các tập Borel của T. Nếu I là đếm được cộng tính, thì $ I(\bigcup_n A_n) \leq \sum_n I(A_n) $. Theo nhận xét trước, chỉ cần thiết lập bất đẳng thức này cho một dãy hữu hạn. Người ta ngay lập tức quy về trường hợp hai tập $ A_1 $ và $ A_2 $; nhưng quan hệ (4) kéo theo rằng

$$
I(A_1 \cup A_2) = I(A_1) + I(A_2 - (A_1 \cap A_2)) \leq I(A_1) + I(A_2).
$$

Bất đẳng thức cần tìm khi đó suy ra ngay lập tức.

4) Nếu I là một hàm đếm được cộng tính và bị chặn địa phương, thì nhận xét trước kéo theo ngay rằng $ I(K) < +\infty $ với mọi tập compact $ K \subset T $.

5) Có thể chứng minh rằng nếu I là cộng tính, nghĩa là, thỏa mãn (4) đối với các dãy hữu hạn, và nếu I là chính quy nội, thì I là đếm được cộng tính (Bài tập 7). Người đọc cũng có thể xác nhận rằng trong chứng minh của Định lý 2 dưới đây chỉ dùng tính cộng và tính chính quy nội.

#### Định lý 2 {#int-ix-s3-thm-2 .statement}

— Cho T là một không gian tôpô, và cho I là một hàm xác định trên $ \mathcal{B}(T) $, nhận giá trị trong $ \overline{\mathbf{R}}_+ $. Điều kiện cần và đủ để tồn tại một độ đo $ \mu $ trên T sao cho $ \mu^*(A) = I(A) $ với mọi $ A \in \mathcal{B}(T) $ là I đếm được cộng tính, bị chặn địa phương và chính quy nội. Khi đó độ đo $ \mu $ là duy nhất.

Ba điều kiện này là cần thiết: thật vậy, ánh xạ $ A \mapsto \mu^*(A) $ trên $ \mathcal{B}(T) $ là đếm được cộng tính (\S 1, No. 5, Hệ quả của Mệnh đề 4), bị chặn địa phương theo định nghĩa của các độ đo (\S 1, No. 2, Định nghĩa 5), và chính quy nội theo Nhận xét 3 của \S 1, No. 2.

Ta chuyển sang sự tồn tại. Rõ ràng là hạn chế của I lên $ \mathcal{K}(T) $ thỏa mãn các điều kiện 1), 2), 3) và 5) của mệnh đề của ĐL. 1; ta hãy chỉ ra rằng 4) cũng được thỏa mãn. Cho K là một tập con compact của T, là giao của một họ có hướng giảm $ (K_\alpha)_{\alpha \in A} $ các tập compact, và cho $ \varepsilon $ là một số $ > 0 $; vì I bị chặn địa phương, tồn tại một lân cận mở (do đó Borel) V của K sao cho $ I(V) < +\infty $, và khi đó tồn tại một chỉ số $ \alpha $ sao cho $ K_\alpha \subset V $; nếu cần thay đổi ký hiệu, ta có thể giả sử rằng $ K_\alpha \subset V $ với mọi $ \alpha \in A $. Do tính chính quy nội của I, tồn tại một tập compact $ L \subset V - K $ sao cho $ I(L) \geq I(V - K) - \varepsilon $; vì L không giao với K, tồn tại một chỉ số $ \alpha $ sao cho $ L \cap K_\alpha = \varnothing $, và khi đó ta có $ I(V - K_\alpha) \geq I(L) \geq I(V - K) - \varepsilon $. Vì $ K_\alpha \subset V $, suy ra $ I(K_\alpha) \leq I(K) + \varepsilon $ và điều kiện 4) được kiểm tra.

Theo Định lý 1, tồn tại một độ đo $ \mu $ sao cho $ \mu^\bullet(K) = I(K) $ với mọi $ K \in \mathcal{K}(T) $. Khi đó tính chính quy nội của các hàm tập hợp $ \mu^\bullet $ và $ I $ trên $ \mathcal{B}(T) $ suy ra rằng $ \mu^\bullet(A) = I(A) $ với mọi $ A \in \mathcal{B}(T) $, và sự tồn tại được chứng minh. Tính duy nhất của $ \mu $ suy ra từ mệnh đề về tính duy nhất của Định lý 1.

### 3. Các không gian Radon

#### Định nghĩa 2 {#int-ix-s3-def-2 .statement}

*Cho T là một không gian tôpô. Ta nói rằng T là một không gian Radon (resp. Radon mạnh) nếu T là Hausdorff và nếu mọi hàm được xác định trên bộ tộc Borel $ \mathcal{B}(T) $ của T, nhận giá trị trong $ \overline{\mathbf{R}}_+ $, cộng tính đếm được và bị chặn (resp. bị chặn địa phương) đều là chính quy nội.*

Chẳng hạn, ta sẽ thấy về sau (Mệnh đề 3) rằng mọi không gian Ba Lan đều là Radon mạnh. Đặc biệt, mọi không gian compact địa phương có một cơ sở đếm được đều là Radon mạnh.

Tồn tại những không gian Radon không là Radon mạnh.

#### Mệnh đề 1 {#int-ix-s3-prop-1 .statement}

*Mọi không gian Radon Lindelöf*$ ^{(1)} $* đều là Radon mạnh.*

Cho T là một không gian Lindelöf là Radon, và cho I là một hàm tập hợp trên tộc $ \mathcal{B}(T) $ vừa dương, vừa cộng tính đếm được và địa phương bị chặn. Các tập mở V sao cho $ I(V) < +\infty $ tạo thành một phủ của T, từ đó có thể rút ra một phủ đếm được $ (V_n)_{n \in \mathbf{N}} $. Đặt $ G_n = V_0 \cup V_1 \cup \cdots \cup V_n $ với mọi $ n \in \mathbf{N} $; đặt $ H_0 = G_0 $ và $ H_n = G_n - G_{n-1} $ với $ n \geq 1 $; sau cùng, ký hiệu bởi $ I_n $ hàm tập hợp $ A \mapsto I(A \cap H_n) $ trên $ \mathcal{B}(T) $, hàm này hiển nhiên vừa cộng tính đếm được vừa bị chặn. Vì các tập hợp $ H_n $ tạo thành một phân hoạch của T, ta có $ I = \sum_n I_n $. Do không gian T là Radon, với mọi $ n \in \mathbf{N} $ tồn tại một độ đo bị chặn $ \mu_n $ trên T sao cho $ \mu_n^\bullet(A) = I_n(A) $ với mọi $ A \in \mathcal{B}(T) $; do đó cũng có $ \sum_n \mu_n^\bullet(A) = I(A) $. Vì I là địa phương bị chặn, họ $ (\mu_n) $ là khả tổng (\S 1, No. 7, Prop. 7); nếu $ \mu $ ký hiệu $ \sum_n \mu_n $, thì ta có $ \mu^\bullet(A) = I(A) $ với mọi $ A \in \mathcal{B}(T) $, và suy ra I là chính quy nội. Nói cách khác, T là Radon mạnh.

Nhắc lại rằng một tập con A của một không gian tôpô T được gọi là *đo được phổ dụng* nếu A là $ \mu $-đo được đối với mọi độ đo $ \mu $ trên T. Điều này tương đương với việc nói rằng A là $ \mu $-đo được đối với mọi độ đo $ \mu $ trên T có *giá compact* (\S 1, No. 8, Prop. 9).

(1) Nhắc lại (GT, I, §9, Exer. 14; TG, IX, Phụ lục I) rằng một *không gian Lindelöf* là một không gian tôpô T sao cho mọi phủ mở của T đều chứa một phủ đếm được.

#### Mệnh đề 2 {#int-ix-s3-prop-2 .statement}

— Cho X là một không gian tôpô và T là một không gian con của X.

a) Giả sử rằng T là một không gian Radon. Khi đó, đối với mọi hàm I xác định trên $ \mathcal{B}(X) $ mà dương, cộng tính đếm được và bị chặn, ta có

$$
\sup_{\substack{K \text{ compact} \\ K \subset T}} I(K) = \inf_{\substack{B \in \mathcal{B}(X) \\ B \supset T}} I(B).
$$

Hơn nữa, T là đo được phổ dụng trong X.

b) Ngược lại, giả sử rằng X là một không gian Radon và T là đo được phổ dụng trong X; khi đó T là một không gian Radon.

Ta hãy chứng minh a). Ta ký hiệu vế phải của (6) là $ \alpha $; với mọi $ n \in \mathbf{N} $, tồn tại một tập hợp $ C_n \in \mathcal{B}(X) $ chứa T, sao cho $ I(C_n) \leq \alpha + 2^{-n} $. Đặt $ C = \bigcap_n C_n $, khi đó ta có $ T \subset C $, $ I(C) = \alpha $. Nếu $ A \in \mathcal{B}(T) $, hãy chọn một tập hợp Borel B của X sao cho $ A = B \cap T $ (GT, IX, §6, No. 3) và đặt $ J(A) = I(B \cap C) $. Số này không phụ thuộc vào lựa chọn B, vì nếu $ B' $ là một tập hợp Borel thứ hai trong X sao cho $ A = B' \cap T $, thì $ B \cap C $ và $ B' \cap C $ chỉ khác nhau bởi một tập hợp Borel M được chứa trong $ C - T $, và $ I(M) = 0 $ theo phép dựng của C. Rõ ràng $ J(K) = I(K) $ với mọi tập compact $ K \subset T $. Gọi $ (A_n) $ là một dãy các tập hợp Borel của T, từng đôi một rời nhau, và, với mỗi $ n $, gọi $ B_n $ là một tập hợp Borel của X sao cho $ B_n \cap T = A_n $. Nếu cần, thay thế $ B_n $ bởi $ B_n - \left( \bigcup_{k < n} B_k \right) $, ta có thể giả sử rằng các tập hợp $ B_n $ từng đôi một rời nhau. Đặt $ A = \bigcup_n A_n $ và $ B = \bigcup_n B_n $; khi đó

$$
J(A) = I(B \cap C) = \sum_n I(B_n \cap C) = \sum_n J(A_n);
$$

Do đó J là một hàm cộng tính đếm được và bị chặn trên $ \mathcal{B}(T) $. Vì T theo giả thiết là một không gian Radon, nên tồn tại một độ đo bị chặn $ \mu $ trên T sao cho $ J(A) = \mu^\bullet(A) $ với mọi $ A \in \mathcal{B}(T) $; do đó

$$
\alpha = J(T) = \mu^\bullet(T) = \sup_K \mu^\bullet(K) = \sup_K J(K),
$$

theo định nghĩa của $ \mu^\bullet $. Vậy công thức (6) được thiết lập.

Bây giờ ta hãy chứng minh rằng T là đo được phổ dụng. Cho $ \lambda $ là một độ đo bị chặn trên X; lập luận trước đó có thể được áp dụng cho hàm tập hợp $ I : A \mapsto \lambda^\bullet(A) $ trên $ \mathcal{B}(X) $, do đó tồn tại một dãy $ (K_n) $ các tập con compắc của T sao cho (với các ký hiệu trên)

$$
\sup_n \lambda^\bullet(K_n) = J(T) = \lambda^\bullet(C).
$$

Đặt $ K' = \bigcup_{n \in \mathbf{N}} K_n $; $ K' $ là Borel trong $ X $, $ K' \subset T \subset C $, $ \lambda^*(K') = \lambda^*(C) $, do đó ba tập hợp này chỉ khác nhau bởi các tập hợp $ \lambda $-không đáng kể, và vì thế $ T $ là $ \lambda $-đo được. Điều này hoàn tất chứng minh của $ a) $.

Xét sang $ b) $. Giả sử rằng $ X $ là một không gian Radon, và rằng $ T $ là đo được phổ dụng trong $ X $. Gọi $ I $ là một hàm dương trên $ \mathcal{B}(T) $ vừa cộng tính đếm được vừa bị chặn; khi đó hàm $ A \mapsto I(A \cap T) $ trên $ \mathcal{B}(X) $ là dương, cộng tính đếm được và bị chặn, vì thế tồn tại một độ đo bị chặn $ \nu $ trên $ X $ sao cho $ I(A \cap T) = \nu^*(A) $ với mọi $ A \in \mathcal{B}(X) $. Khi ấy, $ T $ là $ \nu $-đo được; quan hệ trên cho thấy rằng $ \nu^*(K) = 0 $ với mọi tập con compắc $ K $ của $ X $ rời nhau với $ T $, do đó $ \nu $ tập trung trên $ T $. Do đó, với mọi tập Borel $ A $ của $ X $, ta có $ I(A \cap T) = \nu^*(A \cap T) = \mu^*(A \cap T) $, trong đó $ \mu $ là độ đo cảm sinh bởi $ \nu $ trên $ T $. Sau cùng, suy ra rằng $ I(B) = \mu^*(B) $ với mọi tập hợp $ B \in \mathcal{B}(T) $ (GT, IX, §6, No. 3, *Nhận xét 2*), và quả thật $ I $ là nội chính quy.

#### Hệ quả {#int-ix-s3-n3-cor-1 .statement}

— *Nếu $ X $ là một không gian Radon, thì mọi tập con Borel $ T $ của $ X $ đều là Radon.*

Thật vậy, $ T $ là đo được phổ dụng trong $ X $.

#### Mệnh đề 3 {#int-ix-s3-prop-3 .statement}

— *Mọi không gian Souslin (đặc biệt, mọi không gian Polish hoặc Lusin) đều là Radon mạnh.*

Cho $ T $ là một không gian Souslin; vì $ T $ là một không gian Lindelöf (TG, IX, Phụ lục I, Hệ quả của Mệnh đề 1),(2) nên chỉ cần chứng minh rằng $ T $ là Radon (Mệnh đề 1). Gọi $ I $ là một hàm xác định trên $ \mathcal{B}(T) $, dương, cộng tính đếm được và bị chặn. Ta mở rộng $ I $ lên $ \mathcal{P}(T) $ bằng cách đặt, với mọi tập con $ A $ của $ T $,

$$
I(A) = \inf_{\substack{B \in \mathcal{B}(T) \\ B \supseteq A}} I(B).
$$

Ta hãy chỉ ra rằng sự mở rộng này là một *dung lượng* trên $ T $ (GT, IX, §6, No. 9). Rõ ràng quan hệ $ A \subset A' $ kéo theo $ I(A) \leq I(A') $. Cho $ (A_n) $ là một dãy tăng các tập con của $ T $, và đặt $ A = \bigcup_n A_n $. Vì tập hợp các tập Borel chứa $ A_n $ là ổn định đối với giao đếm được, nên với mỗi $ n $ tồn tại một tập Borel $ B_n $ sao cho $ A_n \subset B_n $ và $ I(A_n) = I(B_n) $ (xem chứng minh của Mệnh đề 2). Đặt $ C_n = \bigcap_{p \geq n} B_p $; $ C_n $ là Borel, và $ A_n \subset C_n \subset B_n $, do đó $ I(A_n) = I(C_n) $. Mặt khác, dãy $ (C_n) $ là tăng. Đặt $ C = \bigcup_n C_n $: quan hệ $ A \subset C $ kéo theo rằng

$$
I(A) \leq I(C) = \lim_n I(C_n) = \lim_n I(A_n),
$$

(2) Mọi không gian Souslin đều có một cơ sở đếm được của các tập hợp mở (GT, IX, §6, No. 2, Prop. 4), do đó là Lindelöf (GT, I, §9, Exer. 14).

do đó đẳng thức $ I(A) = \lim_n I(A_n) $ là ngay lập tức. Do đó, I là một dung lượng.

Nếu $(H_n)$ là một dãy giảm các tập hợp đóng trong T, hiển nhiên $ I\left( \bigcap_n H_n \right) = \inf_n I(H_n) $. Suy ra mọi tập con Souslin F của T đều khả dung đối với I (TG, IX, §6, No. 10, Prop. 15). Đặc biệt, mọi tập hợp Borel A của T đều khả dung (*loc. cit.*, §6, No. 3, Prop. 10).(3) Nói cách khác,

$$
I(A) = \sup_K I(K),
$$

trong đó K chạy trên tập hợp các tập compact được chứa trong A; chúng ta đã chứng minh rằng I là chính quy nội.

#### Nhận xét {#int-ix-s3-n3-rem-1 .statement}

— Cho X là một không gian Lusin (đặc biệt, bất kỳ không gian Polish nào), và f là một ánh xạ liên tục song ánh từ X lên một không gian chính quy (Lusin) Y. Ta biết (TG, IX, §6, No. 7, Prop. 14) rằng ánh xạ $ B \mapsto f^{-1}(B) $ là một song ánh từ bộ tộc Borel của Y lên bộ tộc Borel của X. Các không gian X và Y là Lusin, do đó là Radon mạnh (Mệnh đề 3). Ngay lập tức suy ra rằng ánh xạ $ \mu \mapsto f(\mu) $ là một song ánh từ tập hợp các độ đo bị chặn trên X lên tập hợp các độ đo bị chặn trên Y.(4)

### Bài tập {#int-ix-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
