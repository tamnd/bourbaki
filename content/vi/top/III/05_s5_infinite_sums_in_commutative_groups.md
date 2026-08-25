---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 5
section_title: Infinite sums in commutative groups
lang: vi
source: top-i-iv
pdf_pages: 0267-0276, 0320-0321
extraction: ocr
subsections:
    - "no": 1
      title: SUMMABLE FAMILIES IN A COMMUTATIVE GROUP
      page: 0
      pdf_page: 267
    - "no": 2
      title: CAUCHY'S CRITERION
      page: 0
      pdf_page: 268
    - "no": 3
      title: PARTIAL SUMS ; ASSOCIATIVITY
      page: 0
      pdf_page: 270
    - "no": 4
      title: SUMMABLE FAMILIES IN A PRODUCT OF GROUPS
      page: 0
      pdf_page: 272
    - "no": 5
      title: IMAGE OF A SUMMABLE FAMILY UNDER A CONTINUOUS HOMOMORPHISM
      page: 0
      pdf_page: 273
    - "no": 6
      title: SERIES
      page: 0
      pdf_page: 273
    - "no": 7
      title: COMMUTATIVELY CONVERGENT SERIES
      page: 0
      pdf_page: 275
statements: 19
exercises: 7
content_sha256: 28d0aed7fca46a96e282b825a72559467ca2eb7b27f712e5b171b5ff245ce778
translated_from: content/en/top/III/05_s5_infinite_sums_in_commutative_groups.md
source_content_sha256: f00a62c711a69bc585307c0d066a454a7861d0dd7f4d8b9f20e4756943cb0eda
translation_model: gpt-5.4
translation_run: translate-vi-6128758a
glossary_version: 34
glossary_terms_sha256: d3c3313ce9b15a2644d70168a9ee0e95fb180d6d18ba55500e69bffe74178fa9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. TỔNG VÔ HẠN TRONG CÁC NHÓM GIAO HOÁN

### 1. CÁC HỌ KHẢ TỔNG TRONG MỘT NHÓM GIAO HOÁN

Trong tiết này, chúng tôi sẽ chỉ xét các *nhóm tôpô giao hoán Hausdorff*, mà luật hợp thành của chúng được viết theo *ký hiệu cộng*. Chỉ những kết quả quan trọng nhất mới được chuyển sang ký hiệu nhân.

Cho $G$ là một nhóm giao hoán Hausdorff, cho $I$ là một tập chỉ số bất kỳ và cho $(x_i)_{i \in I}$ là một họ các điểm của $G$, được đánh chỉ số bởi $I$. Với mỗi tập con *hữu hạn* $J$ của $I$ ta gắn phần tử $s_J = \sum_{i \in J} x_i$ của $G$, mà ta gọi là *tổng riêng phần hữu hạn của họ* $(x_i)_{i \in I}$, tương ứng với tập $J$. Nếu $\mathfrak{F}(I)$ ký hiệu *tập hợp các tập con hữu hạn* của $I$, như vậy ta có một ánh xạ $J \to s_J$ từ $\mathfrak{F}(I)$ vào $G$. Khi đó $\mathfrak{F}(I)$ là một tập *có hướng* đối với quan hệ $\subset$; vì nếu $J$ và $J'$ là hai phần tử của $\mathfrak{F}(I)$, thì $J \subset J \cup J'$ và $J' \subset J \cup J'$, và $J \cup J'$ là một tập con hữu hạn của $I$. Gọi $\Phi$ là *bộ lọc tiết diện* của tập có hướng $\mathfrak{F}(I)$ (Chương I, § 6, no. 3).

#### Định nghĩa 1 {#top-iii-s5-def-1 .statement}

Cho $(x_i)_{i \in I}$ là một họ các điểm của một nhóm giao hoán Hausdorff $G$; gọi $\mathcal{F}(I)$ là tập hợp các tập con hữu hạn của tập hợp chỉ số $I$, và với mỗi tập con hữu hạn $J$ của $I$, gọi $s_J$ là tổng của các $x_i$ sao cho $i \in J$. Họ $(x_i)_{i \in I}$ được gọi là khả tổng nếu ánh xạ $J \to s_J$ có một giới hạn đối với bộ lọc tiết diện $\Phi$ của tập hợp $\mathcal{F}(I)$ có hướng bởi quan hệ $\subset$; khi đó giới hạn này được gọi là tổng của họ $(x_i)_{i \in I}$ và được ký hiệu là $\sum_{i \in I} x_i$ (hoặc đơn giản là $\sum_i x_i$, hay thậm chí $\sum x_i$, khi không có nguy cơ nhập nhằng).

Định nghĩa 1 tương đương với phát biểu sau: *họ* $(x_i)$ *là khả tổng và tổng của nó là* $s$ *nếu, với mỗi lân cận* $V$ *của phần tử không trong* $G$, *tồn tại một tập con hữu hạn* $J_0$ *của* $I$ *sao cho với mỗi tập con hữu hạn* $J \supset J_0$ *của* $I$ *ta có* $s_J \in s + V$.

Nếu $G$ được viết theo lối *nhân*, và nếu ta đặt $p_J = \prod_{i \in J} x_i$ với mỗi tập con hữu hạn $J$ của $I$, thì họ $(x_i)$ được gọi là *nhân được* nếu ánh xạ $J \to p_J$ có một giới hạn đối với bộ lọc $\Phi$; giới hạn này được gọi là *tích* của họ $(x_i)$, và được ký hiệu bởi $\prod_{i \in I} x_i$.

#### Nhận xét 1 {#top-iii-s5-n1-rem-1 .statement}

Khi $I$ là *hữu hạn*, Định nghĩa 1 quy về định nghĩa thông thường của tổng của một họ hữu hạn. Nói chung hơn, nếu $I$ là tùy ý và $x_i = 0$ trừ khi chỉ số $i$ thuộc về một tập con *hữu hạn* $J$ của $I$, thì tổng $\sum_{i \in I} x_i$ bằng $\sum_{i \in J} x_i$.

#### Nhận xét 2 {#top-iii-s5-n1-rem-2 .statement}

Định nghĩa của một họ khả tổng không liên quan đến bất kỳ *thứ tự hóa* nào của tập hợp chỉ số $I$, và vì vậy ta có thể nói rằng khái niệm tổng được định nghĩa như thế là *giao hoán*. Chính xác hơn, ta có tính chất sau: cho $(x_i)_{i \in I}$ là một họ khả tổng và cho $\varphi$ là một ánh xạ song ánh từ một tập hợp chỉ số $K$ lên tập hợp $I$; khi đó nếu đặt $y_x = x_{\varphi(x)}$, thì họ $(y_x)_{x \in K}$ là khả tổng và có cùng tổng với $(x_i)$. Thật vậy, nếu $s = \sum_{i \in I} x_i$, và nếu $\sum_{i \in J} x_i \in s + V$ với mọi tập con hữu hạn $J$ chứa tập con hữu hạn $J_0$, thì ta sẽ có $\sum_{x \in L} y_x \in s + V$ với mọi tập con hữu hạn $L$ của $K$ chứa $\overline{\varphi}(J_0)$.

#### Nhận xét 3 {#top-iii-s5-n1-rem-3 .statement}

Định nghĩa 1 còn áp dụng, nói chung, cho mọi họ điểm trong một *không gian tôpô Hausdorff* $X$ mà trên đó đã xác định một *luật hợp thành kết hợp và giao hoán*, được viết theo lối cộng; vì nó không dùng đến các tiên đề của các nhóm tôpô.

### 2. TIÊU CHUẨN CAUCHY

Cho $(x_i)_{i \in I}$ là một họ khả tổng trong $G$. Khi đó, với mỗi lân cận $V$ của gốc trong $G$ đều tồn tại một tập con hữu hạn $J_0$ của $I$ sao cho, với mỗi tập con hữu hạn $K$ của $I$ *không giao với* $J_0$, ta có $s_K \in V$. Vì $J = J_0 \cup K$ là một tập con hữu hạn tùy ý chứa $J_0$; đặt $s = \sum_{i \in J} x_i$ và đặt $W$ là một lân cận đối xứng của $o$ sao cho $W + W \subset V$; khi đó, theo Định nghĩa 1, ta có thể chọn $J_0$ sao cho $s_J \in s + W$ và $s_{J_0} \in S + W$, điều đó có nghĩa là $s_K = s_J - s_{J_0} \in W + W \subset V$.

Ngược lại, giả sử rằng họ $(x_i)$ có tính chất này. Khi đó ảnh của bộ lọc $\Phi$, dưới ánh xạ $J \to s_J$, là một *cơ sở bộ lọc Cauchy* trong $G$. Thật vậy, nếu $J$ là một tập con hữu hạn chứa $J_0$, và nếu $K$ ký hiệu $J \cap C J_0$, thì $K \cap J_0 = \varnothing$ và $s_K = s_J - s_{J_0}$, nên $s_J \in s_{J_0} + V$. Nếu $J'$ là một tập con hữu hạn khác chứa $J_0$, thì $s_J - s_{J'} \in V + V$, và kết quả suy ra. Do đó:

#### Định lý 1 (tiêu chuẩn Cauchy) {#top-iii-s5-thm-1 .statement}

*Trong một nhóm giao hoán Hausdorff* $G$, *để một họ* $(x_i)_{i \in I}$ *là khả tổng thì cần rằng, với mỗi lân cận* $V$ *của phần tử không trong* $G$, *tồn tại một tập con hữu hạn* $J_0$ *của* $I$ *sao cho* $\sum_{i \in K} x_i \in V$ *với mọi tập con hữu hạn* $K$ *của* $I$ *không giao với* $J_0$. *Điều kiện cần này cũng là điều kiện đủ nếu* $G$ *là đầy đủ*.

Như vậy, bằng cách bỏ đi một số hữu hạn số hạng (đủ lớn) khỏi họ $(x_i)$, mọi *tổng riêng hữu hạn* của họ con còn lại đều phải *gần* $o$ tùy ý.

Một hệ quả ngay lập tức của phần thứ nhất của Định lý 1 là mệnh đề sau:

#### Mệnh đề 1 {#top-iii-s5-prop-1 .statement}

*Nếu họ* $(x_i)$ *là khả tổng, thì mọi lân cận của* $o$ *đều chứa tất cả các* $x_i$ *trừ ra một họ con hữu hạn* (nói cách khác, nếu $I$ là vô hạn, thì ta có $\lim x_i = o$ đối với *bộ lọc các phần bù của các tập con hữu hạn của* $I$).

Điều kiện *cần* này để một họ $(x_i)$ là khả tổng *hoàn toàn không đủ* nói chung, ngay cả khi $G$ là đầy đủ; về sau chúng ta sẽ thấy nhiều ví dụ (xem Chương IV, § 7).

#### Hệ quả {#top-iii-s5-n2-cor-1 .statement}

*Cho* $(x_i)_{i \in I}$ *là một họ khả tổng trong một nhóm giao hoán mà phần tử đơn vị có một hệ cơ bản đếm được các lân cận. Khi đó tập hợp các chỉ số* $i$ *sao cho* $x_i \neq o$ *là đếm được*.

Cho $(V_n)$ là một hệ cơ bản đếm được các lân cận của $o$. Nếu $H_n$ là tập hợp tất cả các chỉ số $i$ sao cho $x_i \notin V_n$, thì tập hợp $H$ các chỉ số $i$ sao cho $x_i \neq o$ là hợp của các tập hợp $H_n$, và mỗi $H_n$ đều là *hữu hạn* theo Mệnh đề 1.

#### Nhận xét {#top-iii-s5-n2-rem-1 .statement}

Khi G được viết theo lối nhân, tiêu chuẩn Cauchy có dạng sau: để họ $(x_i)_{i \in I}$ là khả nhân thì cần rằng, với mỗi lân cận V của phần tử đơn vị, tồn tại một tập con hữu hạn $J_0$ của I sao cho, với mỗi tập con hữu hạn K của I không giao với $J_0$, ta có $\prod_{i \in K} x_i \in V$; và điều kiện này là đủ với điều kiện G đầy đủ. Ta suy ra rằng nếu I là vô hạn và $(x_i)$ là khả nhân, thì $\lim x_i = 1$ đối với bộ lọc các phần bù của các tập con hữu hạn của I; nếu thêm nữa phần tử đơn vị có một hệ cơ sở đếm được các lân cận, thì tập hợp các chỉ số i sao cho $x_i \neq 1$ là đếm được.

### 3. TỔNG BỘ PHẬN ; TÍNH KẾT HỢP

#### Mệnh đề 2 {#top-iii-s5-prop-2 .statement}

Trong một nhóm đầy đủ G, mọi họ con của một họ khả tổng đều khả tổng.

Thật vậy, nếu tiêu chuẩn Cauchy được thỏa mãn bởi một họ $(x_i)_{i \in I}$, thì hiển nhiên nó được thỏa mãn bởi mọi họ con.

Vì vậy, nếu $(x_i)_{i \in I}$ khả tổng, thì suy ra tổng $\sum_{i \in J} x_i$ được xác định với mọi tập con J của I, hữu hạn hay không: nó cũng được gọi là tổng bộ phận của họ $(x_i)$, tương ứng với tập con J của tập hợp chỉ số. Tập hợp các tổng bộ phận của một họ khả tổng hiển nhiên được chứa trong bao đóng của tập hợp các tổng bộ phận hữu hạn.

#### Định lý 2 (Tính kết hợp của tổng) {#top-iii-s5-thm-2 .statement}

Cho $(x_i)_{i \in I}$ là một họ khả tổng trong một nhóm đầy đủ G, và cho $(I_\lambda)_{\lambda \in L}$ là một phân hoạch tùy ý của I. Nếu $s_\lambda$ ký hiệu $\sum_{i \in I_\lambda} x_i$, thì họ $(s_\lambda)_{\lambda \in L}$ là khả tổng và có cùng tổng như họ $(x_i)_{i \in I}$.

Vì thế, nếu ta có một họ khả tổng trong một nhóm đầy đủ, thì ta có thể nhóm các hạng của nó một cách tùy ý thành các họ con và lập tổng của mỗi họ con thu được như vậy; họ các tổng bộ phận này lại khả tổng và tổng của nó bằng tổng của họ đã cho.

Đặt $s = \sum_{i \in I} x_i$, và cho $V$ là một lân cận *đóng* bất kỳ của 0 trong $G$. Khi đó tồn tại một tập con hữu hạn $J_0$ của $I$ sao cho, với mỗi tập con hữu hạn $J$ của $I$ chứa $J_0$, ta có $\sum_{i \in J} x_i \in s + V$. Gọi $K_0$ là tập con của $L$ gồm các chỉ số $\lambda$ sao cho $J_\lambda = I_\lambda \cap J_0$ *không rỗng*: $K_0$ rõ ràng là hữu hạn. Cho $K$ là một tập con hữu hạn bất kỳ của $L$ chứa $K_0$; ta sẽ chứng minh rằng $\sum_{\lambda \in K} s_\lambda \in s + V$, điều này sẽ thiết lập định lý.

Bây giờ $s_\lambda$ rất gần với một tổng từng phần hữu hạn của $(x_i)$, mà các chỉ số của nó đều thuộc $I_\lambda$; chính xác hơn, với mọi lân cận đối xứng $W$ của 0, tồn tại với mỗi $\lambda \in K$ một tập con hữu hạn $H_\lambda$ của $I_\lambda$, *chứa* $J_\lambda$ và sao cho $s_\lambda - \sum_{i \in H_\lambda} x_i \in W$. Đặt $J = \sum_{\lambda \in K} H_\lambda$; khi đó $J$ là một tập con hữu hạn của $I$ chứa $J_0$, và ta có

$$
\sum_{i \in J} x_i = \sum_{i \in \bigcup_{\lambda \in K} H_\lambda} x_i = \sum_{\lambda \in K} (\sum_{i \in H_\lambda} x_i)
$$

theo tính kết hợp của các tổng hữu hạn. Do đó do cách lựa chọn $J_0$ và các $H_\lambda$, ta có

$$
\sum_{\lambda \in K} s_\lambda \in s + V + nW
$$

trong đó $n$ là số phần tử của $K$; quan hệ này đúng với mọi $W$, nên cũng có $\sum_{\lambda \in K} s_\lambda \in s + V$, vì $V$ (do đóng) là giao của các lân cận $V + nW$ [§ 3, no. 1, công thức (1)].

Vì thế ta có thể viết *công thức tính kết hợp* đối với các tổng:

(I)

$$
\sum_{\lambda \in L} (\sum_{i \in I_\lambda} x_i) = \sum_{i \in \bigcup_{\lambda \in L} I_\lambda} x_i,
$$

công thức này đúng mỗi khi họ $(I_\lambda)$ là một *phân hoạch* của hợp của chúng và vế phải được xác định. Đặc biệt, nếu tập chỉ số là một *tích* $I = L \times M$, và nếu họ "kép" $(x_{\lambda \mu})_{(\lambda, \mu) \in L \times M}$ là *khả tổng*, thì ta có *công thức thay đổi thứ tự lấy tổng*

(2)

$$
\sum_{(\lambda, \mu) \in L \times M} x_{\lambda \mu} = \sum_{\lambda \in L} (\sum_{\mu \in M} x_{\lambda \mu}) = \sum_{\mu \in M} (\sum_{\lambda \in L} x_{\lambda \mu}).
$$

Cần nhận xét rằng *vế trái* của (1) có thể có nghĩa mà vế phải không được xác định. Chẳng hạn, xét trường hợp $I = LX \{1, 2\}$ và $L$ là vô hạn, và $I_\lambda$ gồm hai phần tử $(\lambda, 1)$ và $(\lambda, 2)$; nếu lấy $x_{\lambda, 1} = a,\ x_{\lambda, 2} = -a$, trong đó $a$ là một phần tử khác không bất kỳ của $G$, thì mọi tổng bộ phận tương ứng với các $I_\lambda$ đều bằng không, và do đó vế trái của (1) được xác định và bằng 0, trong khi vế phải của (1) không có nghĩa, như Mệnh đề 1 cho thấy.

Tương tự, có thể xảy ra việc vế trái của (2) không được xác định nhưng mỗi một trong hai "tổng kép" trong (2) lại có nghĩa; và các phần tử của $G$ mà chúng biểu diễn không nhất thiết phải bằng nhau (xem Chương IV, § 7, Bài tập 17).

Vì vậy, mặc dù luôn luôn có thể "nhóm" các hạng của một tổng, nhưng ngược lại không thể "tách" thành các phần tử của chúng những hạng của một tổng mà bản thân chúng lại xuất hiện như những tổng. Tuy nhiên, phép toán này là hợp thức mỗi khi số các hạng có thể "tách" ấy là hữu hạn.

#### Mệnh đề 3 {#top-iii-s5-prop-3 .statement}

Cho $(x_i)_{i \in I}$ là một họ các điểm của một nhóm $G$, và cho $(I_\lambda)_{\lambda \in L}$ là một phân hoạch hữu hạn của $I$. Nếu mỗi họ con $(x_i)_{i \in I_\lambda}$ đều khả tổng, thì họ $(x_i)_{i \in I}$ là khả tổng và công thức (1) là đúng.

Chỉ cần chứng minh mệnh đề khi $L = (1,2)$; sau khi đã làm xong điều đó, ta khi đó tiến hành bằng quy nạp theo số phần tử của $L$. Đặt $s_1 = \sum_{i \in I_1} x_i$ và $s_2 = \sum_{i \in I_2} x_i$. Với mỗi lân cận $V$ của gốc, tồn tại một tập con hữu hạn $J_1$ (resp. $J_2$) của $I_1$ (resp. $I_2$) sao cho, với mỗi tập con hữu hạn $H_1$ (resp. $H_2$) của $I_1$ (resp. $I_2$) chứa $J_1$ (resp. $J_2$), ta có $\sum_{i \in H_1} x_i \in S_1 + V$ (resp. $\sum_{i \in H_2} x_i \in s_2 + V$). Nếu đặt $J_0 = J_1 \cup J_2$, thì suy ra rằng, với mỗi tập con hữu hạn $H$ của $I$ chứa $J_0$, ta có $\sum_{i \in H} x_i \in S_1 + s_2 + V + V$, và kết quả được suy ra.

### 4. CÁC HỌ KHẢ TỔNG TRONG MỘT TÍCH CỦA CÁC NHÓM

#### Mệnh đề 4 {#top-iii-s5-prop-4 .statement}

Cho $G = \prod_{\lambda \in L} G_\lambda$ là tích của một họ các nhóm giao hoán Hausdorff. Khi đó một họ $(x_i)_{i \in I}$ các điểm của $G$ là khả tổng nếu và chỉ nếu, với mỗi $\lambda \in L$, họ $(\mathrm{pr}_\lambda x_i)_{i \in I}$ là khả tổng; và nếu $s_\lambda$ là tổng của họ này, thì $s = (s_\lambda)$ là tổng của họ $(x_i)$.

Điều này suy ra ngay lập tức từ điều kiện hội tụ, đối với một bộ lọc, của một hàm nhận giá trị trong một không gian tích (Chương I, § 1, no. 6, Hệ quả 1 của Mệnh đề 10); thật vậy, với mỗi tập con hữu hạn $J$ của $I$, ta có

$$
\mathrm{pr}_\lambda \left( \sum_{i \in J} x_i \right) = \sum_{i \in J} \mathrm{pr}_\lambda x_i.
$$

### 5. ẢNH CỦA MỘT HỌ KHẢ TỔNG QUA MỘT ĐỒNG CẤU LIÊN TỤC

#### Mệnh đề 5 {#top-iii-s5-prop-5 .statement}

Cho $f$ là một đồng cấu liên tục của một nhóm giao hoán $G$ vào một nhóm giao hoán $G'$. Nếu $(x_i)$ là một họ cộng được trong $G$, thì $(f(x_i))$ là một họ cộng được trong $G'$, và ta có

$$
\Sigma f(x_i) = f(\Sigma x_i).
$$

Nếu $J$ là một tập con hữu hạn bất kỳ của tập chỉ số, thì $f \left( \sum_{i \in J} x_i \right) = \sum_{i \in J} f(x_i)$, và ảnh qua $f$ của một cơ sở bộ lọc hội tụ là một cơ sở bộ lọc hội tụ (Chương I, § 7, no. 4, Hệ quả 1 của Mệnh đề 9).

#### Mệnh đề 6 {#top-iii-s5-prop-6 .statement}

Cho $(x_i), (y_i)$ là hai họ khả tổng, với cùng tập chỉ số, trong một nhóm $G$. Khi đó các họ $(-x_i), (nx_i)$ ($n \in \mathbf{Z}$), $(x_i + y_i)$ đều khả tổng, và ta có

$$
\begin{align*}
\Sigma(-x_i) &= -\Sigma x_i, \\
\Sigma(nx_i) &= n\Sigma x_i, \\
\Sigma(x_i + y_i) &= \Sigma x_i + \Sigma y_i.
\end{align*}
$$

Vì $x \to -x$ và $x \to nx$ là các đồng cấu liên tục từ $G$ vào $G$; mặt khác, nếu $(x_i)$ và $(y_i)$ là khả tổng, thì họ $(x_i, y_i)$ là khả tổng trong $G \times G$, và vì $(x, y) \to x + y$ là một đồng cấu liên tục từ $G \times G$ vào $G$, ta suy ra (6).

#### Nhận xét {#top-iii-s5-n5-rem-1 .statement}

Mệnh đề 4 và 5 lại áp dụng được cho trường hợp, đã được nhắc đến trước đó, của các họ khả tổng trong một không gian tôpô $X$ có một luật hợp thành kết hợp và giao hoán; điều tương tự cũng đúng với Mệnh đề 3 và công thức (6) nếu ta giả thiết thêm rằng $x + y$ liên tục trên $X \times X$.

### 6. CHUỖI

Xét một dãy các điểm $(x_n)_{n \in \mathbf{N}}$ trong một nhóm giao hoán Hausdorff, và lập dãy các *tổng riêng phần* $s_n = \sum_{p=0}^n x_p$ ($n \in \mathbf{N}$). Ánh xạ $(x_n) \to (s_n)$ là một *song ánh* của tập hợp $G^\mathbf{N}$ gồm các dãy $(x_n)$ các điểm của $G$ lên chính nó; vì nếu dãy $(s_n)$ được cho, thì dãy $(x_n)$ được xác định bởi các hệ thức $x_0 = s_0, x_n = s_n - s_{n-1}$ ($n \geq 1$).

*Chuỗi được xác định bởi dãy* $(x_n)$, hoặc *chuỗi có số hạng tổng quát* là $x_n$ [hoặc đơn giản là *chuỗi* $(x_n)$, do lạm dụng ngôn ngữ, nếu không có nguy cơ nhầm lẫn] được định nghĩa là *cặp* các dãy $(x_n)$ và $(s_n)$ do đó liên kết với nhau. Chuỗi được xác định bởi dãy $(x_n)$ được gọi là *hội tụ* nếu dãy $(s_n)$ hội tụ; giới hạn của dãy này được gọi là *tổng của chuỗi* và được viết là $\sum_{n=0}^\infty x_n$ (hoặc $\sum_{n=0}^\infty x_n$, do lạm dụng ký hiệu).

Nếu chuỗi có số hạng tổng quát là $x_n$ là *hội tụ*, đôi khi chúng tôi sẽ cho phép mình, do lạm dụng ngôn ngữ, gọi nó là "chuỗi $\sum_{n=0}^\infty x_n$" hoặc "chuỗi $x_0 + x_1 + \cdots + x_n + \cdots$".

Một điều kiện *cần* để chuỗi có số hạng tổng quát là $x_n$ hội tụ là dãy $(s_n)$ phải là một *dãy Cauchy*, nghĩa là, với mỗi lân cận $V$ của gốc trong $G$ tồn tại một số nguyên $n_0$ sao cho với mỗi cặp số nguyên $n \geq n_0,\ p > 0$, ta có
$$
s_{n+p} - s_n = \sum_{i=n+1}^{n+p} x_i \in V.
$$
Nếu $G$ là *đầy đủ*, thì điều kiện này cũng là *đủ* (*tiêu chuẩn Cauchy cho chuỗi*).

Nếu chuỗi có số hạng tổng quát là $x_n$ hội tụ, thì đặc biệt ta có $\lim_{n \to \infty} (s_n - s_{n-1}) = \lim_{n \to \infty} x_n = 0$; nhưng điều kiện *cần* này của sự hội tụ tuyệt nhiên không đủ trong trường hợp tổng quát, ngay cả khi $G$ là đầy đủ (xem Chương IV, § 7).

#### Mệnh đề 7 {#top-iii-s5-prop-7 .statement}

*Nếu các chuỗi được xác định bởi các dãy* $(x_n)$ *và* $(y_n)$ *hội tụ, thì các chuỗi được xác định bởi các dãy* $(-x_n)$ *và* $(x_n + y_n)$ *cũng hội tụ, và ta có*
(7)
$$
\sum_{n=0}^\infty (-x_n) = -\sum_{n=0}^\infty x_n,
$$
(8)
$$
\sum_{n=0}^\infty (x_n + y_n) = \sum_{n=0}^\infty x_n + \sum_{n=0}^\infty y_n.
$$
Đây là một hệ quả hiển nhiên của tính liên tục của $-x$ trên $G$, và của $x + y$ trên $G \times G$.

#### Hệ quả {#top-iii-s5-n6-cor-1 .statement}

*Nếu* $(x_n), (y_n)$ *là hai dãy điểm của* $G$ *sao cho* $x_n = y_n$ *trừ một số hữu hạn chỉ số, và nếu chuỗi có số hạng tổng quát là* $x_n$ *hội tụ, thì chuỗi có số hạng tổng quát là* $y_n$ *cũng hội tụ.*

Đối với chuỗi mà số hạng tổng quát là $x_n - y_n$ thì mọi số hạng của nó đều bằng không kể từ một chỉ số nào đó trở đi.

Hệ quả này có thể được phát biểu dưới dạng *ta có thể thay đổi tùy ý một số hữu hạn số hạng của một chuỗi hội tụ mà chuỗi ấy vẫn không thôi hội tụ*.
Đặc biệt, nếu $y_n = 0$ với $n < m$, và $y_n = x_n$ với $n \geq m$, ta thấy rằng chuỗi có số hạng tổng quát là $y_n$ hội tụ khi và chỉ khi chuỗi có số hạng tổng quát là $x_n$ hội tụ; tổng của nó được ký hiệu là $\sum_{n=m}^{\infty} x_n$ và được gọi là *thặng dư* chỉ số $m$ của chuỗi $(x_n)$. Vì
$$
\sum_{n=m}^{\infty} x_n = \sum_{n=0}^{\infty} x_n - s_{m-1},
$$
thặng dư chỉ số $m$ của một chuỗi hội tụ *tiến tới* 0 khi $m$ tiến tới $+\infty$.

Nếu một dãy $(x_n)_{n \in I}$ có tập chỉ số là một tập con vô hạn $I$ của $\mathbf{N}$, và nếu $\varphi$ ký hiệu song ánh *bảo toàn thứ tự nghiêm ngặt* từ $\mathbf{N}$ lên $I$, thì chuỗi xác định bởi dãy $(x_{\varphi(n)})_{n \in \mathbf{N}}$ được gọi, do lạm dụng ngôn ngữ, là *chuỗi* xác định bởi dãy $(x_n)_{n \in I}$; nếu chuỗi này hội tụ, tổng của nó được ký hiệu là $\sum_{n \in I}^{\infty} x_n$. Ta kiểm tra ngay lập tức rằng chuỗi này hội tụ khi và chỉ khi chuỗi có số hạng tổng quát là $(z_n)$ hội tụ, trong đó $z_n = x_n$ nếu $n \in I$ và $z_n = 0$ nếu $n \in \mathbf{C} I$.

Điều quan trọng cần nhận thấy là nếu chuỗi được xác định bởi một dãy $(x_n)_{n \in \mathbf{N}}$ hội tụ, thì có thể tồn tại những tập con vô hạn $I$ của $\mathbf{N}$ sao cho chuỗi được xác định bởi dãy con $(x_n)_{n \in I}$ *không hội tụ* (xem Bài tập 5 và Chương IV, § 7).

Các mệnh đề 4 và 5 mở rộng ngay lập tức cho chuỗi, và chúng tôi để việc phát biểu chúng trong trường hợp này cho bạn đọc.

**Mệnh đề 8 (Tính kết hợp hạn chế của chuỗi).** *Cho* $(k_n)$ *là một dãy tăng ngặt các số nguyên* $\geqslant 0$. *Nếu chuỗi có số hạng tổng quát là* $x_n$ *hội tụ, và nếu đặt* $u_n = \sum_{p=k_{n-1}}^{k_n-1} x_p$, *thì chuỗi có số hạng tổng quát là* $u_n$ *hội tụ, và ta có* $\sum_{n=0}^{\infty} u_n = \sum_{n=0}^{\infty} x_n$.

Thật vậy, dãy các tổng riêng của chuỗi $(u_n)$ là một *dãy con* $(s_{k_n-1})$ của dãy $(s_n)$ các tổng riêng của chuỗi $(x_n)$.

### 7. CHUỖI HỘI TỤ GIAO HOÁN

Cho $(x_n)$ là một dãy *khả tổng* trong $G$, và đặt $s = \sum_{n \in \mathbf{N}} x_n$ là tổng của nó. Khi đó với mỗi lân cận $V$ của 0, tồn tại $J_0 \in \mathcal{F}(\mathbf{N})$ sao cho $s_J \in s + V$ mỗi khi $J \in \mathcal{F}(\mathbf{N})$ và $J_0 \subset J$. Gọi $m$ là số nguyên lớn nhất trong $J_0$; khi đó nếu $n \geqslant m$ thì ta có $s_n \in s + V$, và do đó *chuỗi* $(x_n)$ hội tụ và tổng của nó là $s$. Nhưng đảo lại là *sai*:

Hơn nữa, định nghĩa của một chuỗi hội tụ về bản chất có liên quan đến cấu trúc thứ tự của $\mathbf{N}$. Nếu chuỗi $(x_n)$ hội tụ, và nếu $\sigma$ là một phép hoán vị của $\mathbf{N}$, thì chuỗi $(x_{\sigma(n)})$ không nhất thiết hội tụ (xem Chương IV, § 7, Bài tập 15).

#### Định nghĩa 2 {#top-iii-s5-def-2 .statement}

*Một chuỗi được xác định bởi một dãy* $(x_n)$ *được gọi là hội tụ giao hoán nếu, với mỗi phép hoán vị* $\sigma$ *của* $\mathbf{N}$, *chuỗi được xác định bởi dãy* $(x_{\varphi(n)})$ *là hội tụ.*

#### Mệnh đề 9 {#top-iii-s5-prop-9 .statement}

*Chuỗi được xác định bởi dãy* $(x_n)$ *là hội tụ giao hoán nếu và chỉ nếu dãy* $(x_n)$ *là khả tổng; và khi đó, với mỗi phép hoán vị* $\sigma$ *của* $\mathbf{N}$, *ta có*

$$
\sum_{n=0}^{\infty} x_{\sigma} = \sum_{n \in \mathbf{N}} x_n.
$$

Nếu dãy là khả tổng, thì rõ ràng chuỗi là hội tụ giao hoán. Để chứng minh suy ra ngược lại, ta sẽ lập luận bằng *reductio ad absurdum* và giả sử rằng chuỗi $(x_n)$ là hội tụ giao hoán nhưng dãy $(x_n)$ không khả tổng. Khi đó ảnh của bộ lọc $\Phi$ dưới ánh xạ $H \to s_H$ không thể là một cơ sở bộ lọc Cauchy trong $G$, vì nếu không thì cơ sở bộ lọc này sẽ hội tụ, bởi theo giả thiết nó có một điểm tụ (Chương II, § 3, no. 2, Mệnh đề 5, Hệ quả 2). Do đó tồn tại một lân cận $V$ của 0 trong $G$ sao cho, với mỗi tập con hữu hạn $J$ của $\mathbf{N}$, tồn tại một tập con hữu hạn $H$ của $\mathbf{N}$ không giao với $J$ và sao cho $\sum_{n \in H} x_n \notin V$. Vì thế, bằng quy nạp, ta có thể định nghĩa một phân hoạch của $\mathbf{N}$ thành các tập con *hữu hạn* $H_k$ ($k \in \mathbf{N}$) sao cho $\sum_{n \in H_k} x_n \notin V$ với vô hạn chỉ số $k$. Rõ ràng tồn tại một phép hoán vị $\sigma$ của $\mathbf{N}$ sao cho với mỗi $k$, các giá trị của $n$ mà với chúng $\sigma(n) \in H_k$ là liên tiếp nhau. Nếu $\sigma$ là một phép hoán vị như vậy, thì chuỗi có số hạng tổng quát là $x_{\sigma(n)}$ không thể hội tụ, và ta được một mâu thuẫn.

Nếu nhóm $G$ được viết theo *ký pháp nhân*, thì *tích vô hạn xác định bởi một dãy* $(x_n)$ các điểm của $G$ (hoặc *tích vô hạn có số hạng tổng quát là* $x_n$, hoặc thậm chí *tích* $x_n$ nếu không có khả năng nhầm lẫn) được định nghĩa là cặp tạo bởi dãy $(x_n)$ và dãy các tích từng phần

$$
p_n = \prod_{k=0}^{n} x_k.
$$

Tích vô hạn được gọi là *hội tụ* nếu dãy $(p_n)$ hội tụ, và giới hạn của dãy này được ký hiệu bởi $\prod_{n=0}^{\infty} x_n$ (hoặc $\prod_{n=0}^{\infty} x_n$ do lạm dụng ký hiệu). Chúng tôi dành cho người đọc việc chép lại theo ký pháp nhân các tính chất của chuỗi mà chúng tôi đã thiết lập.

### Bài tập {#top-iii-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
