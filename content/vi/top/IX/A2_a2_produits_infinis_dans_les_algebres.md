---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 2
section_title: Produits infinis dans les algèbres normées
appendix: true
lang: vi
source: top-v-x-fr
book_pages: TG IX.125-TG IX.126
pdf_pages: 0198-0204, 0245-0246
extraction: ocr
subsections:
    - "no": 1
      title: Suites multipliables dans une algèbre normée
      page: 0
      pdf_page: 198
    - "no": 2
      title: Critères de multipliabilité
      page: 79
      pdf_page: 199
    - "no": 3
      title: Produits infinis
      page: 82
      pdf_page: 202
statements: 16
exercises: 8
content_sha256: b1bfc94a8b240499291e6fe0f86be9bbcaa859a864cf08b41dba589fd8eaa4b4
translated_from: content/en-mt/top/IX/A2_a2_produits_infinis_dans_les_algebres.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 15e574616b9216e369d5739775c51f5a56269afe461ad7819939a1d7fc3a9931
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-1f1a38a2
glossary_version: 34
glossary_terms_sha256: cba4fc77be77e2d0dab7d897239217140ec6cb00aeed7c0be5eaed397bd73c2b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC 2

# CÁC TÍCH VÔ HẠN TRONG CÁC ĐẠI SỐ ĐỊNH CHUẨN

### 1. Các dãy khả tích trong một đại số định chuẩn

Cho $A$ là một đại số định chuẩn trên một trường định giá giao hoán rời rạc (IX, p. 37, def. 9); ta sẽ ký hiệu $\|x\|$ là chuẩn của một phần tử $x \in A$, và ta còn giả sử rằng $A$ nhận một phần tử đơn vị $e$.

Cho $(x_n)_{n \geq N}$ là một dãy vô hạn các điểm của $A$; mỗi tập con hữu hạn $J$ của $\mathbf{N}$, được sắp thứ tự toàn phần bởi cấp của $\mathbf{N}$, xác định một dãy (A, I, p. 3) $(x_n)_{n \in J}$ các điểm của $A$; trong Đại số (A, I, p. 3), tích $p_J = \prod_{n \in J} x_n$ của dãy này đã được định nghĩa, mà ta sẽ gọi là tích riêng phần hữu hạn của dãy $(x_n)_{n \in \mathbf{N}}$, tương ứng với tập con hữu hạn $J$ của $\mathbf{N}$ (nhắc lại rằng, với $J = \varnothing$, ta đặt $\prod_{n \in \varnothing} x_n = e$).

#### Định nghĩa 1 {#top-ix-a2-def-1 .statement}

Ta nói rằng dãy $(x_n)_{n \geq N}$ là khả tích trong đại số định chuẩn $A$ nếu ánh xạ $J \mapsto p_J$ có một giới hạn theo bộ lọc các thiết diện của tập hợp $\mathcal{F}(\mathbf{N})$ các tập con hữu hạn của $\mathbf{N}$, được sắp thứ tự bởi quan hệ $\subset$; giới hạn này được gọi là tích của dãy $(x_n)_{n \in \mathbf{N}}$, và được ký hiệu $\prod_{n \in \mathbf{N}} x_n$ (hoặc đơn giản là $\prod_n x_n$); các $x_n$ được gọi là các thừa số của tích này.

Định nghĩa 1 tương đương với định nghĩa sau: dãy $(x_n)$ là khả tích và có tích $p$ nếu, với mọi $\varepsilon > 0$, tồn tại một tập con hữu hạn $J_0$ của $\mathbf{N}$ sao cho, với mọi tập con hữu hạn $J \supset J_0$ của $\mathbf{N}$, ta có $\|p_J - p\| \leq \varepsilon$.

#### Nhận xét 1 {#top-ix-a2-n1-rem-1 .statement}

Khi $A$ là một đại số giao hoán, định nghĩa 1 trùng với định nghĩa đã được cho trong III, p. 37 (Nhận xét 3); nhưng khi $A$ không giao hoán, cấu trúc cấp của tập các chỉ số $\mathbf{N}$ can thiệp một cách cốt yếu vào định nghĩa 1; nếu $\sigma$ là một phép hoán vị bất kỳ của $\mathbf{N}$, không có gì cho phép ta khẳng định nói chung rằng dãy $(\mathbf{x}_{\sigma(n)})$ là khả tích khi dãy $(\mathbf{x}_n)$ là khả tích; hơn nữa, khi hai dãy này là khả tích, các tích của chúng nói chung là khác nhau.

#### Nhận xét 2 {#top-ix-a2-n1-rem-2 .statement}

Định nghĩa 1 tổng quát hóa ngay lập tức cho trường hợp một họ $(\mathbf{x}_n)_{n \in I}$ mà tập các chỉ số $I$ là một tập con của $\mathbf{Z}$ (được sắp thứ tự toàn phần bởi cấp cảm sinh bởi cấp của $\mathbf{Z}$); ta để cho người đọc nhiệm vụ mở rộng sang trường hợp này các tính chất sau đây (xem IX, p. 125, bài tập 1 và 2).

### 2. Các tiêu chuẩn về tính khả tích

Từ nay về sau ta sẽ tự hạn chế vào trường hợp đại số định chuẩn $A$ là đầy đủ.

#### Định lý 1 {#top-ix-a2-thm-1 .statement}

Cho $(\mathbf{x}_n)_{n \in \mathbf{N}}$ là một dãy các điểm của một đại số định chuẩn đầy đủ $A$.

a) Nếu $(\mathbf{x}_n)$ là khả tích và có tích là một phần tử khả nghịch của $A$, thì, với mọi $\varepsilon > 0$, tồn tại một tập con hữu hạn $J_0$ của $\mathbf{N}$ sao cho, với mọi tập con hữu hạn $L$ của $\mathbf{N}$ không giao với $J_0$, ta có $\| \mathbf{e} - \mathbf{p}_L \| \leq \varepsilon$.

b) Ngược lại, nếu dãy $(\mathbf{x}_n)$ thỏa mãn điều kiện này, thì nó có thể nhân được. Hơn nữa, nếu mỗi $\mathbf{x}_n$ là khả nghịch, $\prod_{n \in \mathbf{N}} \mathbf{x}_n$ là khả nghịch.

a) Gọi $\mathbf{p}$ là tích của dãy có thể nhân được $(\mathbf{x}_n)$, và giả sử rằng $\mathbf{p}$ là khả nghịch trong $A$; khi đó (IX, p. 40, mệnh đề 14), tồn tại $\alpha > 0$ và $a > 0$ sao cho, với mọi $y \in A$ thỏa mãn $\| y - \mathbf{p} \| \leq \alpha$, $y$ là khả nghịch, và $\| y^{-1} \| \leq a$. Theo giả thiết, với mọi $\varepsilon$ sao cho $0 < \varepsilon < \alpha$, tồn tại một tập con hữu hạn $H_0$ của $\mathbf{N}$ sao cho, với mọi tập con hữu hạn $H$ của $\mathbf{N}$ chứa $H_0$, ta có $\| \mathbf{p}_H - \mathbf{p} \| \leq \varepsilon$. Gọi $J_0 = \{0, m\}$ là một khoảng của $\mathbf{N}$ chứa $H_0$; với mọi tập con hữu hạn $L$ của $\mathbf{N}$ không gặp $J_0$, các số nguyên thuộc $L$ đều lớn hơn các số nguyên thuộc $H_0$; do đó, nếu đặt $H = H_0 \cup L$, ta có $\mathbf{p}_H = \mathbf{p}_{H_0} \mathbf{p}_L$. Bây giờ, vì $\| \mathbf{p}_{H_0} - \mathbf{p} \| \leq \varepsilon \leq \alpha$, $\mathbf{p}_{H_0}$ là khả nghịch, và ta có $\| \mathbf{e} - \mathbf{p}_{H_0}^{-1} \mathbf{p} \| \leq \varepsilon \| \mathbf{p}_{H_0}^{-1} \| \leq a \varepsilon$; từ quan hệ $\| \mathbf{p}_{H_0} \mathbf{p}_L - \mathbf{p} \| \leq \varepsilon$, suy ra $\| \mathbf{p}_L - \mathbf{p}_{H_0}^{-1} \mathbf{p} \| \leq \varepsilon \| \mathbf{p}_{H_0}^{-1} \| \leq a \varepsilon$ và cuối cùng $\| \mathbf{e} - \mathbf{p}_L \| \leq 2a \varepsilon$.

b) Giả sử rằng, với mọi $\varepsilon > 0$, tồn tại một tập con hữu hạn $J_0$ của $\mathbf{N}$ sao cho, với mọi tập con hữu hạn $L$ của $\mathbf{N}$ không gặp $J_0$, ta có $\| \mathbf{e} - \mathbf{p}_L \| \leq \varepsilon$. Gọi $H_0 = \{0, p\}$ là một khoảng của $\mathbf{N}$ chứa $J_0$; mọi tập con hữu hạn $H$ của $\mathbf{N}$ chứa $H_0$ có thể được viết $H_0 \cup L$, trong đó các số nguyên thuộc $L$ lớn hơn các số nguyên thuộc $H_0$; do đó ta có $\mathbf{p}_H = \mathbf{p}_{H_0} \mathbf{p}_L$, và vì $L$ không gặp $J_0$, $\| \mathbf{p}_H - \mathbf{p}_{H_0} \| \leq \varepsilon \| \mathbf{p}_{H_0} \|$, và do đó $\| \mathbf{p}_H \| \leq (1 + \varepsilon) \| \mathbf{p}_{H_0} \|$. Nếu $\mathbf{p}_{H_0} = 0$, dãy $(\mathbf{x}_n)$ hiển nhiên nhân được và có tích bằng 0; loại trừ trường hợp tầm thường này, tồn tại một khoảng $H_1 = \{0, q\}$, chứa $H_0$ và sao cho, với mọi tập con hữu hạn $L$ của $\mathbf{N}$ không gặp $H_1$, ta có $\| \mathbf{e} - \mathbf{p}_L \| \leq \varepsilon (\| \mathbf{p}_{H_0} \|)^{-1}$. Ta suy ra như trên rằng, với mọi tập con hữu hạn $H \supset H_1$

$$
\| \mathbf{p}_H - \mathbf{p}_{H_1} \| \leq (\| \mathbf{p}_{H_0} \|)^{-1} \| \mathbf{p}_{H_1} \| \varepsilon \leq \varepsilon (1 + \varepsilon).
$$

Tiêu chuẩn Cauchy do đó chỉ ra rằng $J \mapsto \mathbf{p}_J$ có một giới hạn trong $A$ theo tập lọc $\mathcal{F}(\mathbf{N})$.

Nếu tất cả các $x_n$ đều khả nghịch, điều tương tự cũng đúng đối với tất cả các tích từng phần hữu hạn $p_J$; với mọi tập con hữu hạn $H$ chứa $H_0$, do đó có thể viết

$$
\| e - p_{H_0}^{-1} p_H \| \leq \varepsilon;
$$

điều này chỉ ra rằng, trong nhóm nhân $G$ của các phần tử khả nghịch của $A$, ảnh bởi ánh xạ $J \mapsto p_J$ của bộ lọc các đoạn của $\mathfrak{F}(N)$ là một cơ sở bộ lọc Cauchy đối với cấu trúc đều trái của nhóm $G$; nhưng vì $G$ là đầy đủ ($IX$, p. 40, prop. 14), giới hạn của ánh xạ $J \mapsto p_J$ thuộc $G$.

#### Nhận xét {#top-ix-a2-n2-rem-1 .statement}

Khi $(x_n)$ nhân được và có một tích không khả nghịch, điều kiện của th. 1 không còn nhất thiết được thỏa mãn; ví dụ, nếu tất cả các $x_n$ bằng cùng một phần tử $x$ sao cho $\| x \| < 1$, thì dãy $(x_n)$ nhân được và có tích bằng 0, và với mọi tập con hữu hạn khác rỗng $H$ của $N$, ta có $\| p_H \| \leq \| x \| < 1 \leq \| e \|$.

#### Hệ quả 1 {#top-ix-a2-thm-1-cor-1 .statement}

*Nếu* $(x_n)$ *là một dãy nhân được mà tích của nó khả nghịch trong* $A$, $\lim_{n \to \infty} x_n = e$.

#### Hệ quả 2 {#top-ix-a2-thm-1-cor-2 .statement}

*Nếu* $(x_n)$ *là một dãy nhân được mà tích của nó là khả nghịch trong* $A$, *thì mọi dãy* $(x_{n_k})_{k \in \mathbf{N}}$ *trích ra từ* $(x_n)$ *(($n_k$) là một dãy tăng ngặt các số nguyên) là nhân được*.

Đó là điều mà tiêu chuẩn của định lý 1 ($IX$, p. 79) chỉ ra ngay lập tức.

#### Định lý 2 {#top-ix-a2-thm-2 .statement}

*Cho* $A$ *là một đại số chuẩn đầy đủ; nếu* $(u_n)$ *là một chuỗi hội tụ tuyệt đối các điểm của* $A$, *thì dãy* $(e + u_n)$ *là nhân được trong* $A$; *hơn nữa, nếu mọi phần tử* $e + u_n$ *đều khả nghịch trong* $A$, *thì điều tương tự cũng đúng với* $\prod_{n \in \mathbf{N}} (e + u_n)$.

Áp dụng tiêu chuẩn của $IX$, p. 79, định lý 1; với mọi tập con hữu hạn $L$ của $N$, ta có $p_L = e - \prod_{n \in L} (e + u_n) - e = \sum_M \left( \prod_{n \in M} u_n \right)$, $M$ chạy trên tập hợp các tập con khác rỗng của $L$ (được sắp thứ tự toàn phần bởi cấp cảm sinh). Vì $\left| \prod_{n \in M} u_n \right| \leq \prod_{n \in M} \| u_n \|$, ta có thể viết

$$
\| p_L - e \| \leq \sum_M \left( \prod_{n \in M} \| u_n \| \right) = \prod_{n \in L} (1 + \| u_n \|) - 1.
$$

Bây giờ, vì chuỗi có số hạng tổng quát $\| u_n \|$ hội tụ theo giả thiết, dãy $(1 + \| u_n \|)$ là nhân được trong $\mathbf{R}_+^*$ ($IV$, p. 35, định lý 4); với mọi $\varepsilon > 0$, do đó tồn tại một tập con hữu hạn $J_0$ của $N$ sao cho, với mọi tập con hữu hạn $L$ của $N$ không gặp $J_0$, ta có $\left| \prod_{n \in L} (1 + \| u_n \|) - 1 \right| \leq \varepsilon$; do đó có định lý.

#### Hệ quả {#top-ix-a2-n2-cor-1 .statement}

*Nếu chuỗi có số hạng tổng quát* $u_n$ *hội tụ tuyệt đối, và nếu không phần tử nào* $e + u_n$ *là một ước của 0 trong* $A$, *thì tích* $\prod_{n \in \mathbf{N}} (e + u_n)$ *không là một ước của 0 trong* $A$.

Thật vậy, chỉ có một số hữu hạn các số nguyên $n$ sao cho $\|u_n\| > 1$. Đặt $J = \{0, m\}$ là một khoảng của $\mathbf{N}$ chứa tất cả các số nguyên này. Tích của dãy $(\mathbf{e} + u_n)$ là tích của $p_J$ và của phần tử $\prod_{n > m} (\mathbf{e} + u_n)$, tất cả các thừa số của nó đều khả nghịch (IX, p. 39, hệ quả), và do đó bản thân nó cũng khả nghịch; vì $p_J$ là tích của một số hữu hạn các phần tử không là các ước của 0, nó không là một ước của 0, và điều tương tự đúng với $\prod_{n \in \mathbf{N}} (\mathbf{e} + u_n)$.

Điều kiện *đủ* cho tính nhân được cho trong định lý 2 nói chung không phải là cần thiết (xem IX, p. 126, bài tập 6). Tuy nhiên, nó là cần thiết trong trường hợp quan trọng khi $A$ là một đại số có *hạng hữu hạn* trên trường $\mathbf{R}$ (đặc biệt khi $A$ là trường các quaternion $\mathbf{K}$, hoặc một đại số ma trận $\mathbf{M}_n(\mathbf{R})$):

#### Mệnh đề 1 {#top-ix-a2-prop-1 .statement}

*Cho $A$ là một đại số chuẩn có hạng hữu hạn trên $\mathbf{R}$. Nếu $(\mathbf{e} + u_n)$ là một dãy nhân được trong* $A$, *có tích là khả nghịch, thì chuỗi có số hạng tổng quát* $u_n$ *hội tụ tuyệt đối.*

Đã biết (VII, p. 16, mệnh đề 2) rằng tồn tại một số $c > 0$ sao cho, với mọi họ hữu hạn $(\mathbf{x}_i)_{i \in I}$ các điểm của $A$, ta có

(1)
$$
\sum_{i \in I} \|\mathbf{x}_i\| \leq c \cdot \sup_{J \subset I} \left\| \sum_{i \in J} \mathbf{x}_i \right\|.
$$

Cho $(a_n)_{n \in \mathbf{N}}$ là một dãy các phần tử của $A$ bất kỳ. Với mọi tập con hữu hạn $I$ của $\mathbf{N}$, đặt
$$
p_I = \prod_{i \in I} (\mathbf{e} + a_i) \qquad s_I = \sum_{i \in I} a_i, \qquad \sigma_I = \sum_{i \in I} \|a_i\|.
$$

#### Bổ đề 1 {#top-ix-a2-lem-1 .statement}

*Với mọi tập con hữu hạn $I$ của $\mathbf{N}$, đặt $\varphi(I) = \sup_{J \subset I} \|p_J - \mathbf{e}\|.$ Với mọi tập con $J$ của $I$, ta có*
$$
\|p_J - \mathbf{e} - s_J\| \leq \varphi(I) \sigma_J.
$$
Bổ đề là hiển nhiên nếu $J$ là rỗng; ta hãy chứng minh nó bằng quy nạp theo số phần tử của $J$. Cho $J = K \cup \{j\}$, trong đó $j$ lớn hơn nghiêm ngặt mọi phần tử của $K$; khi đó $p_J = p_K(\mathbf{e} + a_j)$ và $s_J = s_K + a_j$, do đó
$$
p_J - \mathbf{e} - s_J = (p_K - \mathbf{e} - s_K) + (p_K - \mathbf{e}) a_j
$$
và, theo giả thiết quy nạp và định nghĩa của $\varphi(I)$
$$
\|p_J - \mathbf{e} - s_J\| \leq \varphi(I) \sigma_K + \varphi(I) \|a_j\| = \varphi(I) \sigma_J
$$
điều này chứng minh bổ đề.

#### Bổ đề 2 {#top-ix-a2-lem-2 .statement}

*Nếu $I$ là một tập con hữu hạn của $\mathbf{N}$ sao cho $\varphi(I) < 1/c$, thì ta có $\sigma_I \leq \frac{c \varphi(I)}{1 - c \varphi(I)}$*.

Thật vậy, vì $\sigma_J \leq \sigma_I$ với mọi tập con $J$ của $I$, nên theo (2) ta có,
$$
\|s_J\| \leq \varphi(I) \sigma_I + \|p_J - \mathbf{e}\| \leq (1 + \sigma_I) \varphi(I);
$$

vì, theo (1), ta có $\sigma_I \leq c \cdot \sup_{J \subset I} \| s_J \|$, suy ra $\sigma_I \leq c \varphi(I)(1 + \sigma_I)$, do đó bổ đề.

Như vậy, cho $(e + u_n)$ là một dãy nhân được trong $A$, có tích khả nghịch; theo định lý 1 (IX, p. 79), tồn tại một tập con hữu hạn $J_0$ của $\mathbf{N}$ sao cho, với mọi tập con hữu hạn $H$ của $\mathbf{N}$ không gặp $J_0$, ta có
$$
\left\| \prod_{i \in H} (e + u_i) - e \right\| \leq 1/2c.
$$
Theo Bổ đề 2, suy ra $\sum_{i \in H} \| u_i \| \leq 1$ với mọi tập con hữu hạn $H$ của $\mathbf{N}$ không gặp $J_0$, điều này kéo theo rằng họ $(\| u_n \|)$ là khả tổng trong $\mathbf{R}$ (IV, p. 32, th. 1).

### 3. Các tích vô hạn

Với mọi dãy $(x_n)$ các điểm của một đại số chuẩn $A$, ta cho tương ứng dãy các *tích từng phần* $p_n = \prod_{k=0}^n x_k$; người ta gọi *tích vô hạn* với nhân tử tổng quát $x_n$, là *cặp* của các dãy $(x_n)$ và $(p_n)$. Tích vô hạn với nhân tử tổng quát $x_n$ được gọi là *hội tụ* nếu dãy $(p_n)$ hội tụ trong $A$; giới hạn của dãy này khi đó được gọi là *tích* của dãy $(x_n)$, và được ký hiệu $\prod_{n=0}^\infty x_n$.

#### Mệnh đề 2 {#top-ix-a2-prop-2 .statement}

*Cho $(x_n)$ là một dãy các điểm của một đại số chuẩn đầy đủ $A$.*

(a) *Nếu tích vô hạn với nhân tử tổng quát* $x_n$ *hội tụ và nếu* $\prod_{n=0}^\infty x_n$ *khả nghịch, thì với mọi* $\varepsilon > 0$, *tồn tại* $n_0$ *sao cho, với* $n_0 \leq m \leq n$, *ta có* $\left\| \prod_{k=m}^n x_k - e \right\| \leq \varepsilon$.

(b) *Ngược lại, nếu dãy* $(x_n)$ *thỏa mãn điều kiện này, tích vô hạn với nhân tử tổng quát* $x_n$ *hội tụ; hơn nữa, nếu mỗi* $x_n$ *đều khả nghịch,* $\prod_{n=0}^\infty x_n$ *là khả nghịch.*

Ta để cho người đọc việc triển khai chứng minh của mệnh đề này, chứng minh được sao chép từng bước từ chứng minh của định lý 1 của IX, p. 79 (các phần hữu hạn $L$ của $\mathbf{N}$ xuất hiện trong chứng minh sau chỉ cần được thay thế bởi các khoảng).

#### Hệ quả 1 {#top-ix-a2-prop-2-cor-1 .statement}

*Nếu tích vô hạn với nhân tử tổng quát* $x_n$ *hội tụ, và nếu* $\prod_{n=0}^\infty x_n$ *khả nghịch,* $\lim_{n \to \infty} x_n = e$.

#### Hệ quả 2 {#top-ix-a2-prop-2-cor-2 .statement}

*Nếu tích vô hạn với nhân tử tổng quát* $x_n$ *hội tụ, và nếu* $\prod_{n=0}^\infty x_n$ *khả nghịch, tích vô hạn với nhân tử tổng quát* $y_n = x_{n+h} (n \geq 0)$ *hội tụ.*

Tích của dãy $(y_n)$ được ký hiệu là $\prod_{n=h}^\infty x_n$, và cũng được gọi là *phần dư có chỉ số h* của tích vô hạn với nhân tử tổng quát $x_n$.

Vẫn giả sử rằng $\prod_{n=0}^{\infty} x_n$ là khả nghịch, ta cũng suy ra từ mệnh đề 2 (IX, p. 82) rằng, nếu $(z_n)$ là một dãy sao cho $z_n = x_n$ ngoại trừ một số hữu hạn các chỉ số, thì tích với nhân tử tổng quát $z_n$ hội tụ.

#### Mệnh đề 3 {#top-ix-a2-prop-3 .statement}

*Cho* $(k_n)$ *là một dãy tăng ngặt các số nguyên* $\geqslant 0$ ($k_0 = 0$) : *nếu tích vô hạn với nhân tử tổng quát* $x_n$ *hội tụ, và nếu đặt* $u_n = \prod_{p=k_n}^{k_{n+1}-1} x_n$, *thì tích vô hạn với nhân tử tổng quát* $u_n$ *hội tụ, và ta có* $\prod_{n=0}^{\infty} u_n = \prod_{n=0}^{\infty} x_n$.

Thật vậy, dãy các tích từng phần của dãy $(u_n)$ được trích ra từ dãy các tích từng phần của dãy $(x_n)$.

Cuối cùng, bằng cùng một lập luận như đối với các nhóm giao hoán (III, p. 44), ta thấy rằng nếu, trong một đại số chuẩn $A$, một dãy $(x_n)$ là *nhân được*, thì tích với nhân tử tổng quát $x_n$ hội tụ, và ta có $\prod_{n=0}^{\infty} x_n = \prod_{n \in \mathbf{N}} x_n$ (cũng được viết là $\prod_{n=0}^{\infty} x_n$); đảo lại dĩ nhiên là sai (xem IX, p. 126, bài tập 7).

Bài tập

## BÀI TẬP {#top-ix-a2-exercises}

Xem [các bài tập cho Phụ lục 2](exercises/a2/).
