---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 3
section_title: Infinite sums and products of complex numbers
lang: vi
source: top-v-x
pdf_pages: 0121-0124, 0132-0133
extraction: ocr
subsections:
    - "no": 1
      title: INFINITE SUMS OF COMPLEX NUMBERS
      page: 0
      pdf_page: 121
    - "no": 2
      title: MULTIPLIABLE FAMILIES IN $ \mathbf{C}^* $
      page: 0
      pdf_page: 121
    - "no": 3
      title: INFINITE PRODUCTS OF COMPLEX NUMBERS
      page: 0
      pdf_page: 123
statements: 9
exercises: 5
content_sha256: 6001c9f03e29701f6f15383ca12ea594da95819ca9d3cae6abeb7f9293206857
translated_from: content/en/top/VIII/03_s3_infinite_sums_and_products_of_complex.md
source_content_sha256: eb379725f3c19b6a8e62a17af5bcf3140e38228c63930c467fc44e289de48cf9
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-818dcaf8
glossary_version: 34
glossary_terms_sha256: 408bb6804dc40cef31763f999abd67380a1ed982eee0be96c60323fe4bfcc093
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. TỔNG VÀ TÍCH VÔ HẠN CỦA CÁC SỐ PHỨC

### 1. TỔNG VÔ HẠN CỦA CÁC SỐ PHỨC

Vì nhóm cộng của trường $ \mathbf{C} $ chính là nhóm cộng của $ \mathbf{R}^2 $, nên không cần nghiên cứu riêng các họ khả tổng và các chuỗi trong $ \mathbf{C} $, vì điều này đã được bao hàm trong lý thuyết tổng quát của Chương VII, § 3; ta để người đọc làm bài tập chuyển các kết quả của lý thuyết này sang ngôn ngữ của lý thuyết số phức. Ta chỉ phát biểu mệnh đề sau đây, là một hệ quả của Mệnh đề 3 của Chương VII, § 3, no. 1:

#### Mệnh đề 1 {#top-viii-s3-prop-1 .statement}

*Nếu* $ (u_\lambda)_{\lambda \in L} $ *và* $ (v_\mu)_{\mu \in M} $ *là hai họ khả tổng của các số phức, thì họ* $ (u_\lambda v_\mu)_{(\lambda, \mu) \in L \times M} $ *khả tổng và ta có*

$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = \left( \sum_{\lambda \in L} u_\lambda \right) \left( \sum_{\mu \in M} v_\mu \right).
$$

Ta để người đọc phát biểu kết quả tương ứng cho các quaternion.

### 2. CÁC HỌ KHẢ TÍCH TRONG $ \mathbf{C}^* $

Trong nhóm nhân $ \mathbf{C}^* $ của các số phức khác không, một họ $ (z_i)_{i \in I} $ không thể khả tích trừ khi $ \lim z_i = 1 $ theo bộ lọc các phần bù của các tập con hữu hạn của $ I $ (Chương III, § 5, no. 2, Mệnh đề 1); hơn nữa, vì mọi điểm của $ \mathbf{C}^* $ đều có một hệ cơ bản đếm được các lân cận, tập các chỉ số $ i $ sao cho $ z_i \neq 1 $ là đếm được nếu họ $ (z_i) $ khả tích (Chương III, § 5, no. 2, Hệ quả của Mệnh đề 1).

#### Mệnh đề 2 {#top-viii-s3-prop-2 .statement}

*Một họ* $ (z_i) $ *các số phức* $ z_i = r_i (\cos \theta_i + i \sin \theta_i) $ *khả tích khi và chỉ khi họ* $ (r_i) $ *các giá trị tuyệt đối của các* $ z_i $ *khả tích trong* $ \mathbf{R}_+^* $ *và họ* $ (\theta_i) $ *các biên độ của các* $ z_i $ *khả tổng trong nhóm các góc* $ \mathfrak{A} $.

Xét cấu trúc của nhóm $ \mathbf{C}^* $ ($ \S $ 1, no. 3, Mệnh đề 1), mệnh đề này là một hệ quả ngay lập tức của Mệnh đề 4 của Chương III, $ \S $ 5, no. 4.

Nếu ta ánh xạ mỗi góc $ \theta $ vào một trong các số đo của nó (theo một cơ sở $ a $ cho trước bất kỳ) thuộc khoảng $ ] - \frac{1}{2} a, \frac{1}{2} a ] $, thì ta có một *đẳng cấu địa phương* của $ \mathfrak{A} $ với $ \mathbf{R} $ ($ \S $ 2, no. 2); vì $ \lim \theta_i = 0 $ theo bộ lọc các phần bù của các tập con hữu hạn của $ I $, ta có thể thay thế điều kiện (trong mệnh đề của Mệnh đề 2) rằng họ $ \theta_i $ phải khả tổng trong $ \mathfrak{A} $ bằng điều kiện rằng họ $ (t_i) $ các *số đo* của các góc $ \theta_i $ thuộc $ ] - \frac{1}{2} a, \frac{1}{2} a ] $ phải khả tổng trong $ \mathbf{R} $.

Định lý sau đây cho một tiêu chuẩn khác để một họ các số phức, được viết dưới dạng $ (1 + u_i) $, khả tích trong $ \mathbf{C}^* $. (Nó tổng quát hóa Định lý 4 của Chương IV, $ \S $ 7, no. 4; xem thêm Chương IX, Phụ lục, no. 2, Mệnh đề 1):

#### Định lý 1 {#top-viii-s3-thm-1 .statement}

*Họ* $ (1 + u_i)_{i \in I} $ *khả tích trong* $ \mathbf{C}^* $ *khi và chỉ khi họ* $ (|u_i|) $ *khả tổng trong* $ \mathbf{R} $.

Với mỗi tập con hữu hạn $ J $ của $ I $, đặt

$$
p_J = \prod_{i \in J} (1 + a_i), \quad s_J = \sum_{i \in J} a_i, \quad \sigma_J = \sum_{i \in J} |a_i|.
$$

#### Bổ đề 1 {#top-viii-s3-lem-1 .statement}

*Với mỗi tập con hữu hạn* $ J $ *của* $ I $, *đặt* $ \varphi(J) = \sup_{L \subset J} (p_L - 1) $. *Khi đó với mỗi tập con* $ L $ *của* $ J $ *ta có*

$$
|p_L - 1 - s_L| \leq \varphi(J) \sigma_L.
$$

Điều này là rõ ràng nếu $ L $ rỗng. Ta tiến hành quy nạp theo lực lượng $ (L) $. Cho $ L = K \cup \{ \lambda \} $, trong đó $ \lambda \notin K $; khi đó $ p_L = p_K (1 + a_\lambda) $ và $ s_L = s_K + a_\lambda $, do đó $ p_L - 1 - s_L = (p_K - 1 - s_K) + (p_K - 1)a_\lambda $; suy ra, theo giả thiết quy nạp và định nghĩa của $ \varphi(J) $, ta có

$$
|p_L - 1 - s_L| \leq \varphi(J) \sigma_K + \varphi(J)|a_\lambda| = \varphi(J) \sigma_L,
$$

điều này chứng minh bổ đề.

#### Bổ đề 2 {#top-viii-s3-lem-2 .statement}

*Nếu* $ J $ *là một tập con hữu hạn của* $ I $ *sao cho* $ \varphi(J) < 1/4 $, *thì*

$$
|\sigma_J| \leq 4 \varphi(J)/(1 - 4 \varphi(J)).
$$

Thật vậy, vì $ \sigma_L \leq \sigma_J $ với mọi tập con $ L $ của $ J $, từ (2) suy ra $ |s_L| \leq \varphi(J) \sigma_J + |p_L - 1| \leq (1 + \sigma_J)\varphi(J) $; nhưng theo Chương VII, $ \S $ 3, no. 1, Mệnh đề 2, ta có $ |\sigma_J| \leq 4 \sup_{L \subset J} |s_L| $, do đó $ \sigma_J \leq 4 \varphi(J)(1 + \sigma_J) $, và kết quả được suy ra.

Bây giờ ta chứng minh rằng điều kiện nêu trong Định lý 1 là đủ. Giả thiết rằng họ $(|u_i|)$ là khả tổng trong $\mathbf{R}$ kéo theo họ $(1 + |u_i|)$ là khả tích trong $\mathbf{R}_+^*$ (Chương IV, § 7, no. 4, Định lý 4); do đó, với mỗi $\varepsilon > 0$, tồn tại một tập con hữu hạn $J_0$ của $I$ sao cho, với mỗi tập con hữu hạn $L$ của $I$ không giao với $J_0$, ta có $\prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon$. Nhưng ta có thể viết $\prod_{i \in L} (1 + u_i) - 1$ dưới dạng $\sum_M \left( \prod_{i \in M} u_i \right)$ trong đó $M$ chạy qua tất cả các tập con khác rỗng của $L$; và vì $\left| \prod_{i \in M} u_i \right| = \prod_{i \in M} |u_i|$, ta có

$$
\left| \prod_{i \in L} (1 + u_i) - 1 \right| \leq \sum_M \left( \prod_{i \in M} |u_i| \right) = \prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon.
$$

Điều này chứng minh mệnh đề của ta, theo tiêu chuẩn Cauchy, vì $\mathbf{C}^*$ là một nhóm đầy đủ.

Ta vẫn phải chứng minh rằng điều kiện của Định lý 1 là cần thiết. Nếu $(1 + u_i)_{i \in I}$ là một họ khả tích trong $\mathbf{C}^*$, tồn tại một tập con hữu hạn $J$ của $I$ sao cho, với mọi tập con hữu hạn $H$ của $I$ không giao với $J$, ta có $\left| \prod_{i \in H} (1 + u_i) - 1 \right| \leq 1/8$. Theo Bổ đề 2, suy ra $\sum_{i \in H} |u_i| \leq 1$ với mọi tập con hữu hạn $H$ của $I$ không giao với $J$, và do đó họ $(|u_i|)$ là khả tổng trong $\mathbf{R}$ (Chương IV, § 7, no. 1, Định lý 1).

Chứng minh trên cũng áp dụng, với những sửa đổi hiển nhiên, cho các tích vô hạn (có thứ tự) trong một số vành chia và đại số không giao hoán (xem Bài tập 6 và Phụ lục Chương IX).

### 3. TÍCH VÔ HẠN CỦA CÁC SỐ PHỨC

Đối với một tích vô hạn các số phức khác không có nhân tử tổng quát $z_n = r_n (\cos \theta_n + i \sin \theta_n)$ hội tụ trong $\mathbf{C}^*$, điều kiện cần và đủ, từ cấu trúc của nhóm $\mathbf{C}^*$, là tích có nhân tử tổng quát $r_n$ hội tụ trong $\mathbf{R}_+^*$ và chuỗi có số hạng tổng quát $t_n$ (số đo của $\theta_n$ nằm trong ]$-\frac{1}{2}a$, $\frac{1}{2}a$]) hội tụ trong $\mathbf{R}$.

#### Định nghĩa 1 {#top-viii-s3-def-1 .statement}

*Một tích vô hạn các số phức, có nhân tử tổng quát* $1 + u_n$, *được gọi là hội tụ tuyệt đối nếu tích có nhân tử tổng quát* $1 + |u_n|$ *hội tụ* (hoặc tương đương, nếu chuỗi có số hạng tổng quát $|u_n|$ hội tụ).

#### Mệnh đề 3 {#top-viii-s3-prop-3 .statement}

*Một tích vô hạn các số phức hội tụ giao hoán khi và chỉ khi nó hội tụ tuyệt đối.*

#### Nhận xét 1 {#top-viii-s3-n3-rem-1 .statement}

Tích có nhân tử tổng quát $ |1 + u_n| $ có thể hội tụ, và thực sự hội tụ tuyệt đối trong $ \mathbf{R}_i^* $, mà không có sự hội tụ của tích có nhân tử tổng quát $ 1 + |u_n| $ (xem Bài tập 4); dĩ nhiên, điều này không thể xảy ra nếu tất cả các $ u_n $ là thực và $ > 0 $ kể từ một chỉ số nào đó trở đi.

#### Nhận xét 2 {#top-viii-s3-n3-rem-2 .statement}

Như đã nhận xét đối với các tích của các nhân tử $ > 0 $, sự hội tụ của chuỗi có số hạng tổng quát $ u_n $ không phải là điều kiện cần cũng không phải là điều kiện đủ cho sự hội tụ của tích có nhân tử tổng quát $ 1 + u_n $.

### Bài tập {#top-viii-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
