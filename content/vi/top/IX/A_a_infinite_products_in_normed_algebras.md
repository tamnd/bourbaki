---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 0
section_title: Infinite products in normed algebras
appendix: true
lang: vi
source: top-v-x
book_pages: 268-270
pdf_pages: 0217-0223, 0274-0276
extraction: ocr
subsections:
    - "no": 1
      title: MULTIPLIABLE SEQUENCES IN A NORMED ALGEBRA
      page: 0
      pdf_page: 217
    - "no": 2
      title: MULTIPLIABILITY CRITERIA
      page: 0
      pdf_page: 218
    - "no": 3
      title: INFINITE PRODUCTS
      page: 0
      pdf_page: 221
statements: 16
exercises: 1
content_sha256: 209779b732cb212fe908441aaa61aae526eacb7379ef6285df344545c728f22c
translated_from: content/en/top/IX/A_a_infinite_products_in_normed_algebras.md
source_content_sha256: 8ac8a39858022c80b0d394946d918655525055ba0ae1ab6a174d3924458ebb1b
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-158509e9
glossary_version: 34
glossary_terms_sha256: 0fbd376d67ac74e0903e4c1a85d10298ff074adfb7825a70b05a649536bb8697
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

==========

## PHỤ LỤC

# TÍCH VÔ HẠN TRONG CÁC ĐẠI SỐ CHUẨN HÓA

### 1. CÁC DÃY KHẢ NHÂN TRONG MỘT ĐẠI SỐ CHUẨN HÓA

Cho $A$ là một đại số chuẩn hóa trên một trường có định giá không rời rạc $K$ (Chương IX, § 3, no. 7, Định nghĩa 9); ta sẽ ký hiệu chuẩn của một phần tử $x \in A$ là $||x||$, và ta giả sử rằng chuẩn này thỏa mãn bất đẳng thức $||xy|| \leq ||x|| \cdot ||y||$; đồng thời ta giả sử rằng $A$ có một phần tử đơn vị $e$.

Cho $(x_n)_{n \in \mathbf{N}}$ là một dãy vô hạn các điểm của $A$. Mọi tập con hữu hạn $J$ của $\mathbf{N}$, được sắp thứ tự tuyến tính theo thứ tự của $\mathbf{N}$, xác định một dãy $(x_n)_{n \in J}$ các điểm của $A$, và ta định nghĩa tích

$$
p_J = \prod_{n \in J} x_n
$$

của dãy này; tích này được gọi là tích từng phần hữu hạn của dãy $(x_n)_{n \in \mathbf{N}}$, tương ứng với tập con hữu hạn $J$ của $\mathbf{N}$ (nhắc rằng nếu $J = \varnothing$ thì ta đặt $\prod_{n \in \varnothing} x_n = e$).

#### Định nghĩa 1 {#top-ix-a0-def-1 .statement}

*Dãy* $(x_n)_{n \in \mathbf{N}}$ *được gọi là khả nhân trong đại số chuẩn hóa* $A$ *nếu ánh xạ* $J \to p_J$ *có một giới hạn đối với lọc các phần của tập* $\mathfrak{F}(\mathbf{N})$ *gồm các tập con hữu hạn của* $\mathbf{N}$, *được sắp theo quan hệ* $\subset$; *giới hạn này được gọi là tích của dãy* $(x_n)_{n \in \mathbf{N}}$, *và được ký hiệu bởi* $\prod_{n \in \mathbf{N}} x_n$ *(hoặc đơn giản* $\prod_n x_n$); *các* $x_n$ *được gọi là các thừa số của tích này.*

Định nghĩa 1 tương đương với mệnh đề sau: *dãy* $(x_n)$ *là khả nhân và tích của nó là* $p$ *nếu với mỗi* $\varepsilon > 0$ *tồn tại một tập con hữu hạn* $J_0$ *của* $\mathbf{N}$ *sao cho, với mọi tập con hữu hạn* $J \supset J_0$ *của* $\mathbf{N}$, *ta có* $||p_J - p|| \leq \varepsilon$.

#### Nhận xét 1 {#top-ix-a0-n1-rem-1 .statement}

Khi $A$ là một đại số giao hoán, Định nghĩa 1 trùng với định nghĩa đã cho trong Chương III, § 5, no. 1, Nhận xét 3; nhưng khi $A$ không giao hoán, cấu trúc thứ tự của tập chỉ số $\mathbf{N}$ là một yếu tố thiết yếu trong Định nghĩa 1. Nếu $\sigma$ là một phép hoán vị tùy ý của $\mathbf{N}$, nói chung ta không thể khẳng định rằng dãy $(x_{\sigma(n)})$ là khả nhân nếu dãy $(x_n)$ là khả nhân; và nếu cả hai dãy đều khả nhân, thì các tích của chúng nói chung sẽ khác nhau.

#### Nhận xét 2 {#top-ix-a0-n1-rem-2 .statement}

Định nghĩa 1 có thể được mở rộng ngay lập tức sang trường hợp của một họ $(x_n)_{n \in I}$ mà tập chỉ số $I$ là một tập con của $\mathbf{Z}$ (được sắp thứ tự tuyến tính theo thứ tự cảm sinh bởi thứ tự của $\mathbf{Z}$). Chúng tôi để cho bạn đọc mở rộng các kết quả dưới đây sang trường hợp này (xem các Bài tập 1 và 2).

### 2. CÁC TIÊU CHUẨN KHẢ NHÂN

Từ nay trở đi ta giả sử rằng đại số chuẩn hóa $A$ là đầy đủ.

#### Định lý 1 {#top-ix-a0-thm-1 .statement}

Cho $(x_n)_{n \in \mathbf{N}}$ là một dãy các điểm trong một đại số chuẩn hóa đầy đủ $A$.
a) Nếu $(x_n)$ khả nhân và nếu tích của nó là một phần tử khả nghịch của $A$, thì với mỗi $\varepsilon > 0$ tồn tại một tập con hữu hạn $J_0$ của $\mathbf{N}$ sao cho, với mọi tập con hữu hạn $L$ của $\mathbf{N}$ không giao với $J_0$, ta có $\|e - p_L\| \leq \varepsilon$.
b) Ngược lại, nếu dãy $(x_n)$ thỏa mãn điều kiện này, thì nó khả nhân. Hơn nữa, nếu mỗi $x_n$ đều là một phần tử khả nghịch, thì $\prod_{n \in \mathbf{N}} x_n$ là một phần tử khả nghịch.

==========

a) Cho p là tích của dãy nhân được $(x_n)$, và giả sử rằng p là một phần tử khả nghịch trong A; khi đó (Chương IX, § 3, no. 7, Mệnh đề 13) tồn tại $\alpha > 0$ và $a > 0$ sao cho, với mọi $y \in A$ thỏa
$$
\|y - p\| \leq \alpha,
$$
thì y là một phần tử khả nghịch và $\|y^{-1}\| \leq a$. Theo giả thiết, với mọi $\varepsilon$ sao cho $0 < \varepsilon < \alpha$, tồn tại một tập con hữu hạn H_0 của \mathbf{N} sao cho, với mọi tập con hữu hạn H của \mathbf{N} chứa H_0, ta có $\|p_H - p\| \leq \varepsilon$. Đặt $J_0 = [0, m]$ là một khoảng của \mathbf{N} chứa H_0; với mỗi tập con hữu hạn L của \mathbf{N} không giao với $J_0$, các số nguyên thuộc L đều lớn hơn các số nguyên thuộc H_0; do đó, nếu $H = H_0 \cup L$, ta có $p_H = p_{H_0} p_L$. Bây giờ, vì $\|p_{H_0} - p\| \leq \varepsilon \leq \alpha$, $p_{H_0}$ là một phần tử khả nghịch, và
$$
\|e - p_{H_0}^{-1} p\| \leq \varepsilon \|p_{H_0}^{-1} p\| \leq a \varepsilon;
$$
vì $\|p_{H_0} p_L - p\| \leq \varepsilon$, ta suy ra
$$
\|p_L - p_{H_0}^{-1} p\| \leq \varepsilon \|p_{H_0}^{-1}\| \leq a \varepsilon,
$$
và cuối cùng $\|e - p_L\| \leq 2a \varepsilon$.

b) Giả sử rằng, với mỗi $\varepsilon > 0$, tồn tại một tập con hữu hạn J_0 của \mathbf{N} sao cho, với mọi tập con hữu hạn L của \mathbf{N} không giao với J_0, ta có $\|e - p_L\| \leq \varepsilon$. Đặt $H_0 = [0, p]$ là một khoảng của \mathbf{N} chứa J_0; khi đó mọi tập con hữu hạn H của \mathbf{N} chứa H_0 đều có thể viết dưới dạng $H_0 \cup L$, trong đó các số nguyên trong L đều lớn hơn các số nguyên trong H_0; do đó ta có $p_H = p_{H_0} p_L$, và vì L không giao với J_0, $\|p_H - p_{H_0}\| \leq \varepsilon \|p_{H_0}\|$, và do đó $\|p_H\| = (1 + \varepsilon)\|p_{H_0}\|$. Nếu $p_{H_0} = 0$, thì dãy $(x_n)$ hiển nhiên là nhân được và tích của nó bằng 0; loại trừ trường hợp tầm thường này, tồn tại một khoảng $H_1 = [0, q]$ chứa $H_0$ và sao cho, với mọi tập con hữu hạn L của \mathbf{N} không giao với $H_1$, ta có $\|e - p_L\| \leq \varepsilon (\|p_{H_0}\|)^{-1}$. Như trên, suy ra rằng, với mỗi tập con hữu hạn H $\supset H_1$,

$$
\|p_H - p_{H_1}\| \leq (\|p_{H_0}\|)^{-1}\|p_{H_1}\|\varepsilon \leq \varepsilon (1 + \varepsilon).
$$

Do đó, tiêu chuẩn Cauchy cho thấy $J \to p_J$ có một giới hạn trong A đối với tập có hướng $\mathfrak{F}(\mathbf{N})$.

Nếu mọi $x_n$ đều là phần tử khả nghịch, thì mọi tích từng phần hữu hạn $p_J$ cũng vậy; do đó với mỗi tập con hữu hạn H chứa H_0 ta có

$$
\|e - p_{H_0}^{-1}p_H\| \leq \varepsilon,
$$

và điều này cho thấy rằng, trong nhóm nhân $G$ của các phần tử khả nghịch của A, ảnh của lọc mặt cắt của $\mathfrak{F}(\mathbf{N})$ qua ánh xạ $J \to p_J$ là một cơ sở lọc Cauchy đối với cấu trúc đều trái của G; nhưng vì G là *đầy đủ* (Chương IX, § 3, no. 7, Mệnh đề 13), giới hạn của ánh xạ $J \to p_J$ thuộc G.

#### Nhận xét {#top-ix-a0-n2-rem-1 .statement}

Nếu $(x_n)$ là nhân được và tích của nó không phải là một phần tử khả nghịch, thì điều kiện của Định lý 1 không nhất thiết thỏa mãn: ví dụ, nếu mọi $x_n$ đều bằng cùng một phần tử $x$, với $\|x\| < 1$, thì dãy $(x_n)$ là nhân được và tích của nó bằng 0, và với mỗi tập con hữu hạn không rỗng $H$ của \mathbf{N}, ta có $\|p_H\| \leq \|x\| < 1 \leq \|e\|$.

#### Hệ quả 1 {#top-ix-a0-thm-1-cor-1 .statement}

*Nếu* $(x_n)$ *là một dãy nhân được có tích là một phần tử khả nghịch của* $A$, *thì* $\lim_{n \to \infty} x_n = e$.

#### Hệ quả 2 {#top-ix-a0-thm-1-cor-2 .statement}

*Nếu* $(x_n)$ *là một dãy nhân được có tích là một phần tử khả nghịch của* $A$, *thì mọi dãy con* $(x_{n_k})_{k \in \mathbf{N}}$ *của* $(x_n)$ *[$(n_k)$ là một dãy số nguyên tăng ngặt]* *đều nhân được*.

Điều này suy ra ngay lập tức từ tiêu chuẩn của Định lý 1.

#### Định lý 2 {#top-ix-a0-thm-2 .statement}

*Cho* $A$ *là một đại số chuẩn đầy đủ*. *Nếu* $(u_n)$ *là một chuỗi hội tụ tuyệt đối của các phần tử của* $A$, *thì dãy* $(e + u_n)$ *nhân được trong* $A$; *và nếu mọi phần tử* $e + u_n$ *đều là phần tử khả nghịch trong* $A$, *thì* $\prod_{n \in \mathbf{N}} (e + u_n)$ *cũng vậy*.

Hãy áp dụng tiêu chuẩn của Định lý 1. Với mọi tập con hữu hạn $L$ của $\mathbf{N}$, ta có $p_L - e = \prod_{n \in L} (e + u_n) - e = \sum_M \left( \prod_{n \in M} u_n \right)$, trong đó $M$ chạy qua tập hợp tất cả các tập con khác rỗng của $L$ (được sắp thứ tự tuyến tính theo thứ tự cảm sinh). Vì $\prod_{n \in M} u_n \leq \prod_{n \in M} |u_n|$, ta có thể viết

$$
||p_1 - e|| = \sum_M (\prod_{n \in M} u_n) \cdot \prod_{i \in I} (1 + |u_i|) - 1.
$$

Bây giờ, vì chuỗi có số hạng tổng quát là $|u_n|$ hội tụ theo giả thiết, nên dãy $1 - |u_n|$ nhân được trong $\mathbf{R}_+^*$ (Chương IV, § 7, no. 4, Định lý 4). Do đó, với mỗi $\varepsilon > 0$ tồn tại một tập con hữu hạn $J_0$ của $\mathbf{N}$ sao cho, với mọi tập con hữu hạn $L$ của $\mathbf{N}$ không giao với $J_0$, ta có $\left| \prod_{n \in L} (1 + ||u_n||) - 1 \right| \leq \varepsilon$; suy ra kết quả.

#### Hệ quả {#top-ix-a0-n2-cor-1 .statement}

*Nếu chuỗi có số hạng tổng quát là* $u_n$ *hội tụ tuyệt đối, và nếu không một phần tử nào trong các phần tử* $e - u_n$ *là ước của không trong* $A$, *thì tích* $\prod_{n \in \mathbf{N}} (e + u_n)$ *không là ước của không trong* $A$.*

Chỉ có hữu hạn số nguyên $n$ sao cho $|u_n| > 1$. Hãy đặt $J = [a, m]$ là một khoảng của $\mathbf{N}$ chứa tất cả các số nguyên này. Tích của dãy $(e + u_n)$ là tích của $p_J$ và phần tử $\prod_{n \notin J} (e - u_n)$, mà mọi thừa số của nó đều là các phần tử khả nghịch (Chương IX, § 3, no. 7, Hệ quả của Mệnh đề 12), và do đó bản thân nó là một phần tử khả nghịch; vì $p_J$ là tích của một số hữu hạn các phần tử không là ước của không, nên nó không là ước của không, và do đó $\prod_{n \in \mathbf{N}} (e + u_n)$ không là ước của không.

Điều kiện đủ để nhân được do Định lý 2 cho không phải nói chung là cần thiết (xem Bài tập 6). Tuy nhiên, nó là cần thiết trong trường hợp quan trọng khi $A$ là một đại số có hạng hữu hạn trên trường $\mathbf{R}$ (tức là $A$ hữu hạn chiều như một không gian vectơ trên $\mathbf{R}$); đặc biệt đây là trường hợp nếu $A$ là vành chia quaternion $\mathbf{H}$, hoặc một đại số ma trận $\mathbf{M}_n(\mathbf{R})$:

#### Mệnh đề 1 {#top-ix-a0-prop-1 .statement}

*Cho* $A$ *là một đại số chuẩn hạng hữu hạn trên* $\mathbf{R}$. *Nếu* $(e + u_n)$ *là một dãy nhân được trong* $A$, *có tích là một phần tử khả nghịch của* $A$, *thì chuỗi có số hạng tổng quát là* $u_n$ *hội tụ tuyệt đối.*

Từ Chương VII, § 3, no. 1, Mệnh đề 2, tồn tại một số $c > 0$ sao cho, với mọi họ hữu hạn $(x_i)_{i \in I}$ gồm các phần tử của $A$, ta có

$$
\sum_{i \in I} \|x_i\| \leq c \sup_{J \subset I} \left| \sum_{i \in J} x_i \right|.
$$

Cho $(a_i)_{i \in \mathbf{N}}$ là một dãy tùy ý các phần tử của $A$. Với mỗi tập con hữu hạn $I$ của $\mathbf{N}$, đặt

$$
p_I = \prod_{i \in I} (e + a_i), \quad s_I = \sum_{i \in I} a_i, \quad \sigma_I = \sum_{i \in I} \|a_i\|.
$$

#### Bổ đề 1 {#top-ix-a0-lem-1 .statement}

Với mỗi tập con hữu hạn $I$ của $\mathbf{N}$, đặt $\varphi(I) = \sup_{J \subset I} ||p_J - e||$. Khi đó, với mỗi tập con $J$ của $I$, ta có

$$
||p_J - e - s_J|| \leq \varphi(I)\sigma_J.
$$

Bổ đề là hiển nhiên nếu $J$ rỗng; ta sẽ chứng minh nó bằng quy nạp theo số phần tử của $J$. Cho $J = K \cup \{j\}$, trong đó $\{j\}$ lớn hơn hẳn mọi $i \in K$. Khi đó $p_J = p_K(e + a_j)$ và

$$
s_J = s_K + a_j,
$$

suy ra

$$
p_J - e - s_J = p_K - e - s_K + (p_K - e)a_j,
$$

và theo giả thiết quy nạp và định nghĩa của $\varphi(I)$, ta có

$$
||p_J - e - s_J|| \leq \varphi(I)\sigma_K + \varphi(I)||a_j|| = \varphi(I)\sigma_J,
$$

điều này chứng minh bổ đề.

#### Bổ đề 2 {#top-ix-a0-lem-2 .statement}

Nếu $I$ là một tập con hữu hạn của $\mathbf{N}$ sao cho $\varphi(I) < 1/c$, thì

$$
\sigma_I \leq c\varphi(I)/(1 - c\varphi(I)).
$$

Vì $\sigma_J \leq \sigma_I$ với mọi tập con $J$ của $I$, suy ra từ (2)

$$
||s_J|| \leq \varphi(I)\sigma_I + ||p_J - e|| \leq (1 + \sigma_I)\varphi(I);
$$

và vì cũng có $\sigma_I \leq c \cdot \sup_{J \subset I} ||s_J||$, theo (1), nên suy ra rằng

$$
\sigma_I \leq c\varphi(I)(1 + \sigma_I),
$$

điều này đưa đến kết quả.

Bây giờ cho $(e + u_n)$ là một dãy khả nhân trong $A$, có tích là một phần tử khả nghịch; theo Định lý 1 tồn tại một tập con hữu hạn $J_0$ của $\mathbf{N}$ sao cho, với mỗi tập con hữu hạn $H$ của $\mathbf{N}$ không giao với $J_0$, ta có

$$
\left| \prod_{i \in H} (e + u_i) - e \right| \leq 1/2c.
$$

Theo Bổ đề 2, suy ra $\sum_{i \in H} ||u_i|| - 1$ với mọi tập con hữu hạn $H$ của $\mathbf{N}$ không giao với $J_0$, và do đó (Chương IV, § 7, no. 1, Định lý 1) họ $(||u_n||)$ là khả tổng trong $\mathbf{R}$.

### 3. TÍCH VÔ HẠN

Với mỗi dãy $(x_n)$ các phần tử trong một đại số định chuẩn $A$, ta tương ứng dãy *các tích từng phần* $p_n = \prod_{k=0}^n x_k$; khi đó *cặp* các dãy $(x_n)$ và $(p_n)$ được gọi là tích vô hạn có nhân tử tổng quát là $x_n$. Tích vô hạn có nhân tử tổng quát $x_n$ được gọi là hội tụ nếu dãy $(p_n)$ hội tụ trong $A$; giới hạn của dãy này khi đó được gọi là tích của dãy $(x_n)$ và được ký hiệu bởi $\prod_{n=0}^\infty x_n$.

#### Mệnh đề 2 {#top-ix-a0-prop-2 .statement}

*Cho* $(x_n)$ *là một dãy các điểm trong một đại số chuẩn đầy đủ* $A$.

a) *Nếu tích vô hạn có nhân tử tổng quát là* $x_n$ *hội tụ và nếu* $\prod_{n=0}^\infty x_n$ *là một phần tử khả nghịch trong* $A$, *thì với mỗi* $\varepsilon > 0$ *tồn tại một số nguyên* $n_0$ *sao cho*
$$
\left\| \prod_{k=m}^n x_k - e \right\| \leq \varepsilon
$$
*khi* $n_0 \leq m \leq n$.

b) *Ngược lại, nếu dãy* $(x_n)$ *thỏa mãn điều kiện này, tích vô hạn với nhân tử tổng quát* $x_n$ *hội tụ; và nếu mỗi* $x_n$ *là một phần tử khả nghịch trong* $A$, *thì* $\prod_{n=0}^\infty x_n$ *là một phần tử khả nghịch*.

Chứng minh của mệnh đề này theo từng bước chứng minh của Định lý 1, và được để lại cho người đọc (các tập con hữu hạn $L$ của $N$ trong chứng minh của Định lý 1 được thay thế bởi các khoảng).

#### Hệ quả 1 {#top-ix-a0-prop-2-cor-1 .statement}

*Nếu tích vô hạn với nhân tử tổng quát là* $x_n$ *hội tụ, và nếu* $\prod_{n=0}^\infty x_n$ *là một phần tử khả nghịch*, *thì* $\lim_{n \to \infty} x_n = e$.

#### Hệ quả 2 {#top-ix-a0-prop-2-cor-2 .statement}

*Nếu tích vô hạn với nhân tử tổng quát là* $x_n$ *hội tụ, và nếu* $\prod_{n=0}^\infty x_n$ *là một phần tử khả nghịch*, *thì tích vô hạn với nhân tử tổng quát*
$$
y_n = x_{n+h} \quad (n \geq 0)
$$
*hội tụ*.

Tích của dãy $(y_n)$ được ký hiệu bởi $\prod_{n=h}^\infty x_n$, và cũng được gọi là thặng dư chỉ số $h$ của tích vô hạn với nhân tử tổng quát $x_n$.

Vẫn dưới giả thiết rằng $\prod_{n=h}^\infty x_n$ là một phần tử khả nghịch, suy ra từ Mệnh đề 2 rằng nếu $(z_n)$ là một dãy sao cho $z_n = x_n$ với mọi chỉ số trừ một số hữu hạn chỉ số, thì tích với nhân tử tổng quát $z_n$ hội tụ.

#### Mệnh đề 3 {#top-ix-a0-prop-3 .statement}

*Cho* $(k_n)$ *là một dãy tăng ngặt các số nguyên* $\geq 0$, *sao cho* $k_0 = 0$; *nếu tích vô hạn với nhân tử tổng quát là* $x_n$ *hội tụ*, *và* nếu ta đặt

$$
u_n = \prod_{p=k_n}^{k_{n+1}-1} x_p,
$$

*thì tích vô hạn có nhân tử tổng quát là* $u_n$ *hội tụ và ta có*

$$
\prod_{n=0}^{\infty} u_n = \prod_{n=0}^{\infty} x_n.
$$

Vì dãy các tích từng phần của dãy $(u_n)$ là một dãy con của dãy các tích từng phần của dãy $(x_n)$.

Cuối cùng, cùng một lập luận như đã được dùng cho các nhóm Abel (Chương III, § 5, no. 7) cho thấy rằng nếu một dãy $(x_n)$ trong một đại số chuẩn $\mathbf{A}$ là *nhân được*, thì tích có nhân tử tổng quát là $x_n$ hội tụ, và

$$
\prod_{n=0}^{\infty} x_n = \prod_{n \in \mathbf{N}} x_n
$$

(điều này cũng được viết là $\prod_{n=0}^{\infty} x_n$); đảo lại dĩ nhiên không đúng (xem Bài tập 7).

### Bài tập {#top-ix-a0-exercises}

Xem các [bài tập của Phụ lục 0](exercises/a0/).
