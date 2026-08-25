---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 2
section_title: Summable families of positive measures
lang: vi
source: int-i-vi
book_pages: INT V.95-INT V.96
pdf_pages: 0266-0270, 0350-0351
extraction: ocr
subsections:
    - "no": 1
      title: Definition of summable families of measures
      page: 11
      pdf_page: 266
    - "no": 2
      title: Integration with respect to a sum of positive measures
      page: 12
      pdf_page: 267
    - "no": 3
      title: Decomposition of a measure as a sum of measures with compact support
      page: 14
      pdf_page: 269
statements: 12
exercises: 4
content_sha256: ac6ca31637ea8aae30c05c45c4958de54a1d1026d67aaf4ebe1d5143fd16ca3e
translated_from: content/en/int/V/02_s2_summable_families_of_positive_measures.md
source_content_sha256: 290c436e1eb1835d7f3151eac47140087383fdc5ddbccba20fa7ed077333c707
translation_model: gpt-5.4-mini
translation_run: translate-vi-2189d355
glossary_version: 34
glossary_terms_sha256: 9e45b9ab5d7ec34ee597eee5a323354b39816f4ef806fe7f09c548167c926775
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC HỌ KHẢ TỔNG CỦA CÁC ĐỘ ĐO DƯƠNG

### 1. Định nghĩa về họ khả tổng của các độ đo

Cho $(\lambda_\alpha)_{\alpha \in A}$ là một họ các độ đo dương trên một không gian địa phương compact X; họ $(\lambda_\alpha)_{\alpha \in A}$ được gọi là *một họ độ đo khả tổng* nếu nó khả tổng trong không gian vectơ $\mathcal{M}(X)$ các độ đo thực trên X, được trang bị tôpô mơ hồ (GT, III, §5, No. 1). Điều này tương đương với việc nói rằng với mọi hàm $f \in \mathcal{K}(X)$, họ các số $\lambda_\alpha(f)$ khả tổng trong $\mathbf{R}$. Thật vậy, điều kiện này hiển nhiên là cần thiết; ngược lại, nếu nó được thỏa mãn thì dạng tuyến tính $f \mapsto \sum_{\alpha \in A} \lambda_\alpha(f)$ trên $\mathcal{K}(X)$ là dương, do đó là một độ đo dương $\nu$ (Chương III, §1, No. 5, Định lý 1), và ta kiểm tra ngay lập tức rằng các tổng riêng hữu hạn của họ $(\lambda_\alpha)$ hội tụ mơ hồ đến $\nu$, theo bộ lọc tiết diện của tập hợp các tập con hữu hạn của A (GT, III, §5, No. 1, Định nghĩa 1).

Vì mỗi phần tử của $\mathcal{K}(X)$ là hiệu của hai phần tử của $\mathcal{K}_+(X)$, họ $(\lambda_\alpha)$ khả tổng nếu và chỉ nếu
$$
\sum_{\alpha \in A} \lambda_\alpha(f) < +\infty
$$

với mọi hàm $f \in \mathcal{K}_+(X)$. Điều kiện này cũng tương đương với điều sau đây:

(2)
$$
\sum_{\alpha \in A} \lambda_\alpha(K) < +\infty
$$
với mọi tập compact $K \subset X$.

Thật vậy, (2) suy ra (1) vì $f \leq \|f\| \cdot \varphi_S$, trong đó S ký hiệu giá đỡ compact của $f$. Ngược lại, nếu K là một tập compact, tồn tại một hàm $f \in \mathcal{K}_+(X)$ sao cho $\varphi_K \leq f$ (Chương III, §1, No. 2, Bổ đề 1), và suy ra rằng (1) suy ra (2).

#### Nhận xét 1 {#int-v-s2-n1-rem-1 .statement}

Ngay lập tức thấy rằng, khi họ $(\lambda_\alpha)_{\alpha \in A}$ khả tổng, tổng của nó là cận trên đúng trong $\mathcal{M}_+(X)$ của các tổng riêng hữu hạn $\sum_{\alpha \in J} \lambda_\alpha$, trong đó J chạy qua tập hợp các tập con hữu hạn của A.

#### Nhận xét 2 {#int-v-s2-n1-rem-2 .statement}

Cho $(\theta_\alpha)_{\alpha \in A}$ là một họ các độ đo phức trên X; họ $(\theta_\alpha)$ được gọi là *khả tổng* nếu họ $(|\theta_\alpha|)$ của các độ đo dương khả tổng; *điều này chưa đủ* để họ $(\theta_\alpha)$ khả tổng trong không gian vectơ $\mathcal{M}(X; \mathbf{C})$ được trang bị tôpô mơ hồ (xem Bài tập 3).

### 2. Tích phân đối với một tổng của các độ đo dương

*Trong suốt số này,* X ký hiệu một không gian địa phương compact, $(\lambda_\alpha)_{\alpha \in A}$ một họ khả tổng các độ đo dương trên X, và $\nu$ là độ đo $\sum_{\alpha \in A} \lambda_\alpha$.

#### Mệnh đề 1 {#int-v-s2-prop-1 .statement}

— *Cho f là một hàm số lượng dương xác định trên X. Khi đó*
$$
\nu^\bullet(f) = \sum_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

Điều này suy ra ngay từ Nhận xét 1, Mđ. 11 của §1, No. 3 và Mđ. 3 của §1, No. 1.

#### Hệ quả 1 {#int-v-s2-prop-1-cor-1 .statement}

— *Với mọi tập con compact (tương ứng mở và tương đối compact) M của X,
$$
\nu(M) = \sum_{\alpha \in A} \lambda_\alpha(M).
$$*

#### Hệ quả 2 {#int-v-s2-prop-1-cor-2 .statement}

— *Để một tập con N của X là địa phương $\nu$-không đáng kể, cần và đủ rằng, với mọi $\alpha \in A$, N là địa phương $\lambda_\alpha$-không đáng kể.*

#### Hệ quả 3 {#int-v-s2-prop-1-cor-3 .statement}

— *Với mọi hàm $f \in \mathcal{F}_+(X)$,
$$
\nu^*(f) \geq \sum_{\alpha \in A} \lambda_\alpha^*(f).
$$*

Bất đẳng thức là hiển nhiên nếu $f$ không $\nu$-điều tiết, vì khi đó $\nu^*(f) = +\infty$ ($\S 1$, No. 2, Mệnh đề 7). Nếu $f$ là $\nu$-điều tiết thì $f$ là $\lambda_\alpha$-điều tiết với mọi $\alpha \in A$, vì mọi tập mở khả tích theo $\nu$ đều khả tích theo $\lambda_\alpha$; quan hệ (4) khi đó suy ra ngay từ (3) và từ Mệnh đề 7 của $\S 1$, No. 2.

Có thể xảy ra rằng hai vế của (4) không bằng nhau, ngay cả khi A đếm được và mỗi của $\lambda_\alpha$ là một độ đo điểm ($\S 1$, Bài tập 4 a)).

#### Mệnh đề 2 {#int-v-s2-prop-2 .statement}

— *Cho $f$ là một ánh xạ từ $X$ vào một không gian tôpô $G$. Để $f$ là $\nu$-đo được, cần và đủ là $f$ là $\lambda_\alpha$-đo được với mọi $\alpha \in A$.*

Điều này suy ra ngay từ Hệ quả 2 của Mệnh đề 11 của $\S 1$.

#### Mệnh đề 3 {#int-v-s2-prop-3 .statement}

— *Để một ánh xạ $f$ từ $X$ vào một không gian Banach $F$ là khả tích thiết yếu theo $\nu$, cần và đủ là $f$ khả tích thiết yếu theo $\lambda_\alpha$ với mọi $\alpha \in A$ và*

$$
\sum_{\alpha \in A} \int^\bullet |f| \, d\lambda_\alpha < +\infty .
$$

*Họ $(\int f \, d\lambda_\alpha)_{\alpha \in A}$ khi đó là khả tổng tuyệt đối trong $F$, và*

$$
\int f \, d\nu = \sum_{\alpha \in A} \int f \, d\lambda_\alpha .
$$

Thật vậy, để $f$ khả tích thiết yếu theo $\nu$ (tương ứng khả tích thiết yếu theo $\lambda_\alpha$), cần và đủ là $f$ đo được theo độ đo $\nu$ (tương ứng $\lambda_\alpha$) và $\nu^\bullet(|f|) < +\infty$ (tương ứng $\lambda_\alpha^\bullet(|f|) < +\infty$), theo Mệnh đề 9 của $\S 1$, No. 3. Phần đầu của mệnh đề do đó suy ra ngay từ các Mệnh đề 2 và 1. Nếu $f$ khả tích thiết yếu theo $\nu$, bất đẳng thức

$$
\sum_{\alpha \in A} \left| \int f \, d\lambda_\alpha \right| \leq \sum_{\alpha \in A} \int |f| \, d\lambda_\alpha = \nu(|f|)
$$

suy ra rằng họ $(\int f \, d\lambda_\alpha)$ là khả tổng tuyệt đối trong $F$, và chuẩn của tổng không lớn hơn chuẩn của $f$ trong $\mathcal{L}_F^1(\nu)$. Tập hợp các $f \in \mathcal{L}_F^1(\nu)$ thỏa mãn (6) vì thế là một không gian con tuyến tính đóng $\mathcal{H}$ của $\mathcal{L}_F^1(\nu)$; mà không gian con này cũng trù mật trong $\mathcal{L}_F^1(\nu)$, vì nó chứa các hàm dạng $f \cdot a$, trong đó $a \in F$ và $f$ là một hàm dương hữu hạn khả tích (Mệnh đề 1). Do đó $\mathcal{H} = \mathcal{L}_F^1(\nu)$ và mệnh đề được chứng minh.

Mệnh đề 3 cũng có thể được suy ra từ định lý tổng quát về tích phân sẽ được chứng minh ở §3 (No. 3, Định lý 1).

#### Hệ quả 1 {#int-v-s2-prop-3-cor-1 .statement}

— Giả sử rằng $f$ là $\nu$-khả tích; khi đó $f$ là $\lambda_\alpha$-khả tích với mọi $\alpha \in A$, và công thức (6) đúng. Ngược lại, nếu tập hợp $A$ là hữu hạn và $f$ là $\lambda_\alpha$-khả tích với mọi $\alpha \in A$, thì hàm $f$ là $\nu$-khả tích.

Nếu $f$ khả tích theo $\nu$, thì $f$ khả tích thực chất theo $\nu$ và $\nu$-điều độ (\S1, No. 3, Cor. of Prop. 9); $f$ do đó khả tích thực chất theo $\lambda_\alpha$ và $\lambda_\alpha$-điều độ, suy ra $\lambda_\alpha$-khả tích, với mọi $\alpha \in A$. Ngược lại, nếu $A$ là hữu hạn và nếu $f$ là $\lambda_\alpha$-khả tích với mọi $\alpha \in A$, thì $f$ khả tích thực chất theo $\nu$ theo Prop. 3, và chỉ cần kiểm tra rằng $\nu^*(|f|) < +\infty$; điều này suy ra ngay từ quan hệ $\nu^* = \sum_{\alpha \in A} \lambda_\alpha^*$ (Ch. IV, §1, No. 3, Prop. 15).

#### Hệ quả 2 {#int-v-s2-prop-3-cor-2 .statement}

— Cho $\theta$ là một độ đo phức trên $X$; đặt $\theta_1 = (\Re \theta)^+$, $\theta_2 = (\Re \theta)^-$, $\theta_3 = (\Im \theta)^+$, $\theta_4 = (\Im \theta)^-$. Để một ánh xạ $f$ của $X$ vào một không gian tôpô $G$ (tương ứng vào một không gian Banach $F$) là đo được (tương ứng khả tích thực chất, khả tích) đối với độ đo $\theta$, điều kiện cần và đủ là nó đo được (tương ứng khả tích thực chất, khả tích) đối với từng độ đo $\theta_i$ ($i = 1, 2, 3, 4$).

Nếu $f$ là đo được (tương ứng khả tích thực chất, khả tích) đối với $\theta$, thì theo định nghĩa $f$ đo được (tương ứng khả tích thực chất, khả tích) đối với độ đo $|\theta|$, do đó cũng đối với các độ đo $\theta_i$, mà $\leq |\theta|$. Ngược lại, nếu $f$ đo được (tương ứng khả tích thực chất, khả tích) đối với các độ đo $\theta_i$, thì Prop. 2 (tương ứng Prop. 3, Cor. 1 of Prop. 3) suy ra rằng $f$ đo được (tương ứng khả tích thực chất, khả tích) đối với độ đo $\theta_1 + \theta_2 + \theta_3 + \theta_4$, mà $\geq |\theta|$.

### 3. Phân tích một độ đo thành tổng các độ đo có giá đỡ compact

#### Mệnh đề 4 {#int-v-s2-prop-4 .statement}

— Cho $\mu$ là một độ đo dương trên một không gian compact địa phương $T$, và cho $\mathfrak{K}$ là một tập trù mật theo $\mu$ gồm các tập con compact của $T$. Tồn tại một họ khả tổng $(\mu_\alpha)_{\alpha \in A}$ gồm các độ đo dương trên $T$ sao cho $\mu = \sum_{\alpha \in A} \mu_\alpha$, và sao cho các giá đỡ của các độ đo $\mu_\alpha$ thuộc $\mathfrak{K}$ và tạo thành một họ đếm được địa phương gồm các tập compact rời nhau từng đôi một.

Nếu độ đo $\mu$ là điều độ, thì tập chỉ số $A$ có thể lấy đếm được.

Xét một họ đếm được địa phương $(K_\alpha)_{\alpha \in A}$ gồm các phần tử của $\mathfrak{K}$ rời nhau từng đôi một sao cho tập $N = T - \bigcup_{\alpha \in A} K_\alpha$ là không đáng kể địa phương đối với $\mu$

(Ch. IV, §5, No. 9, Mệnh đề 14). Với mọi hàm $f \in \mathcal{K}(T)$, đặt
$$
\mu_\alpha(f) = \mu(f \varphi_{K_\alpha});
$$
dạng tuyến tính $\mu_\alpha$ trên $\mathcal{K}(T)$ là dương, do đó là một độ đo dương, có giá đỡ được chứa trong $K_\alpha$. Vì mọi tập compact được chứa trong một phần tử của $\mathfrak{K}$ đều thuộc $\mathfrak{K}$, nên $\operatorname{Supp}(\mu_\alpha) \in \mathfrak{K}$ với mọi $\alpha \in A$. Chỉ còn phải chứng minh rằng họ $(\mu_\alpha)$ là khả tổng và tổng của nó bằng $\mu$, nói cách khác là $\sum_{\alpha \in A} \mu_\alpha(f) = \mu(f)$ với mọi hàm $f \in \mathcal{K}_+(T)$.

Bây giờ, cho $S$ là giá đỡ compact của $f$, và cho $A'$ là tập đếm được gồm các $\alpha \in A$ sao cho $S \cap K_\alpha \neq \varnothing$. Vì tập $N \cap S$ là $\mu$-không đáng kể,
$$
\begin{align*}
\mu(f) &= \mu(f \varphi_S) = \sum_{\alpha \in A'} \mu(f \varphi_{S \cap K_\alpha}) = \sum_{\alpha \in A'} \mu(f \varphi_{K_\alpha}) \\
&= \sum_{\alpha \in A} \mu(f \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha(f).
\end{align*}
$$
Điều đó hoàn tất chứng minh của trường hợp tổng quát. Nếu $\mu$ là điều độ, thì tập $T$ là $\mu$-điều độ và do đó $T$ là hợp của một dãy $(L_n)$ các tập compact và một tập không đáng kể (\S 1, No. 2, Mệnh đề 5); cho $A'$ là tập đếm được gồm các $\alpha \in A$ sao cho $K_\alpha$ cắt một trong các $L_n$. Khi đó $\mu_\alpha = 0$ với $\alpha \notin A'$, và câu cuối cùng của mệnh đề suy ra ngay lập tức.

#### Nhận xét {#int-v-s2-n3-rem-1 .statement}

Một độ đo dương có thể là tổng của một dãy các độ đo có giá đỡ compact, mà không điều độ (xem Bài tập 4 a) của \S 1).

### Bài tập {#int-v-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
