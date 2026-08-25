---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $\mathbf{R}^n$
section: 3
section_title: Infinite sums in the groups $\mathbf{R}^n$
lang: vi
source: top-v-x
pdf_pages: 0089-0092, 0101-0102
extraction: ocr
subsections:
    - "no": 1
      title: SUMMABLE FAMILIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 89
    - "no": 2
      title: SERIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 92
statements: 9
exercises: 2
content_sha256: c60a39b8d817fb4dab927743e66d021c3ed385681c4f5c269a5c17360db92cda
translated_from: content/en/top/VII/03_s3_infinite_sums_in_the_groups_mathbf_r_n.md
source_content_sha256: 63ba3a9e422d70448db18bbb1c82a9347f390a6d75ddb2e4e632006793a8a2bc
translation_model: gpt-5-6-mini
translation_run: translate-vi-d93bb120
glossary_version: 34
glossary_terms_sha256: a9771ee13262b62b325ecb9f6fc909340747d86213fc4e6ee3116fa8cdbb14e8
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC TỔNG VÔ HẠN TRONG CÁC NHÓM $\mathbf{R}^n$

### 1. CÁC HỌ KHẢ TỔNG TRONG $\mathbf{R}^n$

Vì mọi điểm của $\mathbf{R}^n$ đều có một *hệ cơ bản đếm được* các lân cận, một họ $(x_t)$ các điểm của nhóm cộng $\mathbf{R}^n$ chỉ khả tổng nếu tập hợp các chỉ số $t$ sao cho $X_t \neq 0$ là *đếm được* (Chương III, \S 5, no. 2, Hệ quả của Mệnh đề 1); do đó, về cơ bản, việc nghiên cứu các họ khả tổng

#### Mệnh đề 1 {#top-vii-s3-prop-1 .statement}

*Một họ* $(x_i)_{i \in I}$ *các điểm* $x_i = (x_{i,k})_{1 \leq k \leq n}$ *của* $\mathbf{R}^n$ *là khả tổng khi và chỉ khi mỗi một trong* $n$ *họ* $(x_{i,k})_{i \in I}$ *các số thực là khả tổng trong* $\mathbf{R}$.

Điều này suy ra từ Chương III, § 5, no. 4, Mệnh đề 4.

Điều kiện của Mệnh đề 1 có thể được biến đổi như sau:

#### Định lý 1 {#top-vii-s3-thm-1 .statement}

*Một họ* $(x_i)_{i \in I}$ *các điểm của* $\mathbf{R}^n$ *là khả tổng khi và chỉ khi họ* $(||x_i||)$ *các chuẩn Euclid của các* $x_i$ *là khả tổng trong* $\mathbf{R}$.

Điều này suy ra không khó từ Mệnh đề 1, điều kiện để một họ các số thực khả tổng (Chương IV, § 7, no. 2, Định lý 3), các bất đẳng thức

$$
\sup_{1 \leq k \leq n} |x_{i,k}| \leq ||x_i|| \leq \sum_{i=1}^n |x_{i,i}|,
$$

và nguyên lý so sánh (Chương IV, § 7, no. 1, Định lý 2).

Cũng có thể tiến hành hơi khác, bằng cách trước hết chứng minh mệnh đề sau:

#### Mệnh đề 2 {#top-vii-s3-prop-2 .statement}

*Nếu* $(x_i)_{i \in I}$ *là một họ hữu hạn bất kỳ các điểm trong* $\mathbf{R}^n$, *thì*

$$
\sum_{i \in I} ||x_i|| \leq 2n \cdot \sup_{J \subset I} \left| \sum_{i \in J} x_i \right|.
$$

Vì nếu $x_i = (x_{ij})_{1 \leq j \leq n}$, ta có $||x_i|| \leq \sum_{j=1}^n |x_{ij}|$, do đó

$$
\sum_{i \in I} ||x_i|| \leq \sum_{j=1}^n \left( \sum_{i \in I} |x_{ij}| \right).
$$

Bây giờ $\sum_{i \in I} |x_{ij}| = \sum_{i \in I} x_{ij}^+ + \sum_{i \in I} x_{ij}^-$, và vì với mọi tập con $J$ của $I$ ta có

$$
-\sum_{i \in I} x_{ij}^- \leq -\sum_{i \in J} x_{ij}^- \leq \sum_{i \in J} x_{ij}^+ \leq \sum_{i \in I} x_{ij}^+
$$

suy ra rằng

$$
\sum_{i \in I} |x_{ij}| \leq 2 \cdot \sup_{J \subset I} \left| \sum_{i \in J} x_{ij} \right|.
$$

Nhưng $\left| \sum_{i \in J} x_{ij} \right| \leq \left| \sum_{i \in J} x_{ij} \right|$, do đó ta được bất đẳng thức (1).

Bây giờ, Định lý 1 tương đương với mệnh đề sau (vì $\mathbf{R}^n$ là một nhóm đầy đủ): họ $(x_i)$ thỏa mãn tiêu chuẩn Cauchy (Chương III, § 5, no. 2, Định lý 1) khi và chỉ khi họ $(||x_i||)$ cũng thỏa mãn tiêu chuẩn Cauchy. Bây giờ bất đẳng thức tam giác cho thấy điều kiện này là đủ, và bất đẳng thức (1) cho thấy nó là cần.

Hơn nữa ta có bất đẳng thức

$$
\left| \sum_i x_i \right| \leq \sum_i ||x_i||
$$

bất đẳng thức này có được bằng cách chuyển qua giới hạn từ bất đẳng thức tương ứng đối với các tổng riêng hữu hạn.

#### Hệ quả {#top-vii-s3-n1-cor-1 .statement}

*Một họ* $(x_i)$ *các điểm của* $\mathbf{R}^n$ *là khả tổng khi và chỉ khi tập hợp các tổng riêng hữu hạn của họ bị chặn trong* $\mathbf{R}^n$.

Theo Định lý 1 và bất đẳng thức tam giác, điều kiện này là cần; nó là đủ theo bất đẳng thức (1) và Định lý 1.

#### Mệnh đề 3 {#top-vii-s3-prop-3 .statement}

*Cho* $(x_\lambda)_{\lambda \in L}$ *là một họ khả tổng các điểm của* $\mathbf{R}^m$, $(y_\mu)_{\mu \in M}$ *là một họ khả tổng các điểm của* $\mathbf{R}^n$, *và cho* $f$ *là một ánh xạ song tuyến tính từ* $\mathbf{R}^m \times \mathbf{R}^n$ *vào* $\mathbf{R}^p$. *Khi đó họ* $(f(x_\lambda, y_\mu))_{(\lambda, \mu) \in L \times M}$ *là khả tổng và ta có*

$$
\sum_{(\lambda, \mu) \in L \times M} f(x_\lambda, y_\mu) = f \left( \sum_{\lambda \in \mu} x_\lambda, \sum_{\mu \in M} y_\mu \right).
$$

Để chứng minh rằng họ $(f(x_\lambda, y_\mu))$ là khả tổng, theo Mệnh đề 1 chỉ cần chứng minh rằng mỗi một trong $p$ họ được tạo bởi các tọa độ của các điểm $f(x_\lambda, y_\mu)$ trong $\mathbf{R}^n$ là khả tổng: nói cách khác, ta có thể hạn chế vào trường hợp $f$ là một *dạng* song tuyến tính; nhưng đối với một dạng như vậy $f$ ta có

$$
f(x, y) = \sum_{i, j} a_{ij} x_i y_j,
$$

và do đó ta quy về trường hợp $f(x, y) = x_i y_j$, và trong trường hợp này kết quả đã được chứng minh (Chương IV, § 7, no. 3, Mệnh đề 1).

Bằng cách chuyên biệt hóa hàm $f$, ta thu được đặc biệt các hệ quả sau:

#### Hệ quả 1 {#top-vii-s3-prop-3-cor-1 .statement}

*Nếu* $(a_\lambda)_{\lambda \in L}$ *là một họ khả tổng các số thực và nếu* $(x_\mu)_{\mu \in M}$ *là một họ khả tổng các điểm của* $\mathbf{R}^n$, *thì họ* $(a_\lambda x_\mu)_{(\lambda, \mu) \in L \times M}$ *là khả tổng và ta có*

$$
\sum_{(\lambda, \mu) \in L \times M} a_\lambda x_\mu = \left( \sum_{\lambda \in L} a_\lambda \right) \left( \sum_{\mu \in M} x_\mu \right).
$$

#### Hệ quả 2 {#top-vii-s3-prop-3-cor-2 .statement}

*Nếu* $(x_\lambda)_{\lambda \in L}$ *và* $(y_\mu)_{\mu \in M}$ *là hai họ điểm khả tổng của* $\mathbf{R}^n$, *thì họ* $(x_\lambda | y_\mu)$ *(xem Chương VI, § 2, no. 2)* *là khả tổng trong* $\mathbf{R}$, *và ta có*

$$
\sum_{(\lambda, \mu) \in L \times M} (x_\lambda | y_\mu) = \left( \sum_{\lambda \in L} x_\lambda \middle| \sum_{\mu \in M} y_\mu \right).
$$

### 2. CHUỖI TRONG $\mathbf{R}^n$

Một chuỗi có số hạng tổng quát là $x_m = (x_{mi})_{1 \leq i \leq n}$ hội tụ trong $\mathbf{R}^n$ khi và chỉ khi mỗi trong số $n$ chuỗi $(x_{mi})_{m \in \mathbf{N}}$ hội tụ trong $\mathbf{R}$.

#### Định nghĩa 1 {#top-vii-s3-def-1 .statement}

*Một chuỗi các điểm của* $\mathbf{R}^n$ *được gọi là hội tụ tuyệt đối nếu chuỗi các chuẩn Euclid của các số hạng của nó hội tụ.*

#### Mệnh đề 4 {#top-vii-s3-prop-4 .statement}

*Một chuỗi các điểm của* $\mathbf{R}^n$ *được gọi là hội tụ giao hoán khi và chỉ khi nó hội tụ tuyệt đối.*

Đây là một hệ quả của Mệnh đề 9 của Chương III, § 5, no. 7 và Định lý 1 ở trên.

Các ví dụ được cho trong Chương IV, § 7 cho thấy một chuỗi trong $\mathbf{R}^n$ có thể *hội tụ* mà không *hội tụ tuyệt đối*.

### Bài tập {#top-vii-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).

==========

Đó là toàn bộ đoạn văn. Hãy viết bản dịch của mọi thứ giữa hai dòng, rồi dừng lại.
