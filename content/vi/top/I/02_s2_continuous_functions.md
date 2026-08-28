---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 2
section_title: Continuous functions
lang: vi
source: top-i-iv
pdf_pages: 0031-0041, 0125-0128
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS FUNCTIONS
      page: 0
      pdf_page: 31
    - "no": 2
      title: COMPARISON OF TOPOLOGIES
      page: 0
      pdf_page: 34
    - "no": 3
      title: INITIAL TOPOLOGIES
      page: 0
      pdf_page: 36
    - "no": 4
      title: FINAL TOPOLOGIES
      page: 0
      pdf_page: 38
    - "no": 5
      title: PASTING TOGETHER OF TOPOLOGICAL SPACES
      page: 0
      pdf_page: 40
statements: 26
exercises: 10
content_sha256: 5562b4681c83c20050e0ed264482614f3e968e4e9928eaf76464b16d881221e1
translated_from: content/en/top/I/02_s2_continuous_functions.md
source_content_sha256: 16e7ac6daa7f6e8d5016ffb450612e74265560ae6512c3a4b479d5b88d5f0cf7
translation_model: gpt-5.4
translation_run: translate-vi-a475e41b
glossary_version: 34
glossary_terms_sha256: 56b439a9c9c1d57b95205785c0994cfab9f3d993b18893608fb4cb7f4c7594a3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. HÀM LIÊN TỤC

### 1. HÀM LIÊN TỤC

#### Định nghĩa 1 {#top-i-s2-def-1 .statement}

Một ánh xạ $f$ từ một không gian tôpô $X$ vào một không gian tôpô $X'$ được gọi là liên tục tại một điểm $x_0 \in X$ nếu, với mọi lân cận $V'$ của $f(x_0)$ trong $X'$, tồn tại một lân cận $V$ của $x_0$ trong $X$ sao cho quan hệ $x \in V$ kéo theo $f(x) \in V'$.

Định nghĩa 1 có thể được phát biểu lại dưới dạng trực quan hơn sau đây: nói rằng $f$ liên tục tại điểm $x_0$ có nghĩa là $f(x)$ gần $f(x_0)$ đến mức tùy ý mỗi khi $x$ đủ gần $x_0$.

Quan hệ "với mỗi $x \in V, f(x) \in V'$" là tương đương với $f(V) \subset V'$ hoặc cũng tương đương với $V \subset \overline{f}^{-1}(V')$; xét theo tiên đề lân cận ($V_I$), ta thấy rằng Định nghĩa 1 tương đương với điều sau đây: $f : X \to X'$ được gọi là liên tục tại điểm $x_0$ nếu, với mỗi lân cận $V'$ của $f(x_0)$ trong $X'$, $\overline{f}^{-1}(V')$ là một lân cận của $x_0$ trong $X$. Hơn nữa, chỉ cần $\overline{f}^{-1}(V')$ là một lân cận của $x_0$ đối với mỗi lân cận $V'$ thuộc một hệ lân cận cơ bản của $f(x_0)$ trong $X'$ ($§ 1$, no. 3).

#### Mệnh đề 1 {#top-i-s2-prop-1 .statement}

Cho $f$ là một ánh xạ từ một không gian tôpô $X$ vào một không gian tôpô $X'$. Nếu $f$ liên tục tại $x$, và nếu $x$ nằm trong bao đóng của một tập con $A$ của $X$, thì $f(x)$ nằm trong bao đóng của $f(A)$.

Cho $V'$ là một lân cận của $f(x)$ trong $X'$. Vì $f$ liên tục tại $x$, $\overline{f}^{-1}(V')$ là một lân cận của $x$ trong $X$. Do đó $\overline{f}^{-1}(V')$ giao với $A$, suy ra $V'$ giao với $f(A)$, và vì thế $f(x)$ thuộc bao đóng của $f(A)$.

#### Mệnh đề 2 {#top-i-s2-prop-2 .statement}

Cho $X, X', X''$ là ba không gian tôpô; cho $f$ là một ánh xạ từ $X$ vào $X'$, liên tục tại $x \in X$; cho $g$ là một ánh xạ từ $X'$ vào $X''$, liên tục tại $f(x)$. Khi đó hợp thành $h = g \circ f : X \to X''$ liên tục tại $x$.

Cho $V''$ là một lân cận của $h(x) = g(f(x))$ trong $X''$. Vì $g$ liên tục tại $f(x)$ nên suy ra $\overline{g}^{-1}(V'')$ là một lân cận của $f(x)$ trong $X'$. Nhưng $f$ liên tục tại $x$, do đó $\overline{f}^{-1}(\overline{g}^{-1}(V'')) = \overline{h}^{-1}(V'')$ là một lân cận của $x$ trong $X$, và vì thế $h$ liên tục tại $x$.

#### Định nghĩa 2 {#top-i-s2-def-2 .statement}

Một ánh xạ từ một không gian tôpô $X$ vào một không gian tôpô $X'$ được gọi là liên tục trên $X$ (hoặc đơn giản là liên tục) nếu nó liên tục tại mọi điểm của $X$.

#### Ví dụ 1 {#top-i-s2-n1-exa-1 .statement}

Ánh xạ đồng nhất của một không gian tôpô $X$ lên chính nó là liên tục.
2) Một ánh xạ hằng từ một không gian tôpô vào một không gian tôpô là liên tục.
3) Mọi ánh xạ từ một không gian rời rạc vào một không gian tôpô đều liên tục.

#### Định lý 1 {#top-i-s2-thm-1 .statement}

Cho $f$ là một ánh xạ từ một không gian tôpô $X$ vào một không gian tôpô $X'$. Khi đó các mệnh đề sau là tương đương:

a) $f$ liên tục trong $X$.

b) Với mọi tập con $A$ của $X$, $f(\overline{A}) \subset \overline{f(A)}$.

c) Ảnh ngược theo $f$ của mọi tập con đóng của $X'$ là một tập con đóng của $X$.

d) Ảnh ngược theo $f$ của mọi tập con mở của $X'$ là một tập con mở của $X$.

Chúng ta đã thấy rằng a) kéo theo b) (Mệnh đề 1). Để chỉ ra rằng b) kéo theo c), lấy $F'$ là một tập con đóng của $X'$ và đặt $F = \overline{f^{-1}(F')}$; khi đó theo giả thiết $f(\overline{F}) \subset \overline{f(F)} \subset \overline{F'} = F'$, do đó $\overline{F} \subset \overline{f^{-1}(F')} = F \subset \overline{F}$, suy ra $F = \overline{F}$ và $F$ là đóng. Nhờ quan hệ $\overline{f^{-1}(A')} = \overline{f^{-1}(CA')}$ với mọi tập con $A'$ của $X'$, c) kéo theo d). Cuối cùng, giả sử rằng d) được thỏa mãn. Lấy $x$ là một điểm bất kỳ của $X$ và $V'$ là một lân cận bất kỳ của $f(x)$ trong $X'$; khi đó tồn tại một tập hợp mở $A'$ trong $X'$ sao cho

$$
f(x) \in A' \subset V'
$$

và do đó $x \in \overline{f^{-1}(A')} \subset \overline{f^{-1}(V')}$. Theo giả thiết, $\overline{f^{-1}(A')}$ là mở trong $X$, nên $\overline{f^{-1}(V')}$ là một lân cận của $x$ trong $X$. Vậy d) suy ra a).

Nhận xét. 1) Cho $\mathcal{B}$ là một cơ sở (§ 1, no. 3) của tôpô của $X'$; khi đó để $f : X \to X'$ liên tục, điều kiện cần và đủ là $\overline{f^{-1}(U')}$ mở trong $X$ với mọi $U' \in \mathcal{B}$.

#### Ví dụ {#top-i-s2-n1-exa-2 .statement}

Cho $a$ là một số hữu tỉ bất kỳ. Ánh xạ $x \to a + x$ của đường thẳng hữu tỉ $\mathbf{Q}$ vào chính nó là liên tục trên $\mathbf{Q}$, vì ảnh ngược theo ánh xạ này của một khoảng mở $]b, c[$ là khoảng mở

$$
]b - a, c - a[.
$$

Tương tự, ánh xạ $x \to ax$ là liên tục trên $\mathbf{Q}$; điều này là hiển nhiên nếu $a = 0$, vì khi đó $ax = 0$ với mọi $x$; nếu $a \neq 0$ thì ảnh ngược theo ánh xạ này của khoảng mở $]b, c[$ là khoảng mở có các đầu mút là $b/a$ và $c/a$.

2) Ảnh trực tiếp của một tập mở (tương ứng, đóng) của $X$ dưới một ánh xạ liên tục $f : X \to X'$ không nhất thiết là mở (tương ứng, đóng) trong $X'$ (xem § 5).

#### Ví dụ {#top-i-s2-n1-exa-3 .statement}

\* Ánh xạ $f : x \to 1/(1 + x^2)$ từ $\mathbf{R}$ vào chính nó là liên tục, nhưng $f(\mathbf{R})$ là khoảng nửa mở $]0, 1]$, không mở cũng không đóng trong $\mathbf{R}$. \*

#### Định lý 2 {#top-i-s2-thm-2 .statement}

1) Nếu $f : X \to X'$ và $g : X' \to X''$ là hai ánh xạ liên tục, thì $g \circ f : X \to X''$ là liên tục.

2) Để một song ánh $f$ của một không gian tôpô $X$ lên một không gian tôpô $X'$ là một đồng phôi, điều kiện cần và đủ là $f$ và nghịch đảo của $f$ đều liên tục (hay, như người ta cũng nói, là $f$ song liên tục).

Mệnh đề thứ nhất là một hệ quả ngay lập tức của Mệnh đề 2; mệnh đề thứ hai suy ra từ Định lý 1, d) và định nghĩa của một đồng phôi (§ 1, no. 1).

#### Nhận xét 1 {#top-i-s2-n1-rem-1 .statement}

Có thể có một song ánh liên tục của một không gian tôpô $X$ lên một không gian tôpô $X'$ mà không song liên tục: chẳng hạn, lấy $X'$ là đường thẳng hữu tỉ $\mathbf{Q}$, và $X$ là tập hợp $\mathbf{Q}$ với tôpô rời rạc; khi đó ánh xạ đồng nhất $X \to X'$ là liên tục nhưng không phải là một đồng phôi.

#### Nhận xét 2 {#top-i-s2-n1-rem-2 .statement}

Để kiểm tra rằng một song ánh liên tục $f : X \to X'$ là một đồng phôi, chỉ cần chứng minh rằng với mỗi $x \in X$ và mỗi lân cận $V$ của $x$, $f(V)$ là một lân cận của $f(x)$ trong $X'$.

#### Nhận xét 3 {#top-i-s2-n1-rem-3 .statement}

Cho $X$ là một không gian tôpô, và với mỗi $x \in X$ gọi $\mathcal{B}(x)$ là tập hợp tất cả các lân cận của $x$. Cho $x_0$ là một điểm của $X$; với mỗi $x \in X$, định nghĩa một tập hợp $\mathcal{B}_0(x)$ gồm các tập hợp con của $X$ như sau: $\mathcal{B}_0(x_0) = \mathcal{B}(x_0)$, và nếu $x \neq x_0$ thì $\mathcal{B}_0(x)$ là tập hợp tất cả các tập hợp con của $X$ chứa $x$. Kiểm tra ngay lập tức được (§ 1, no. 2, Mệnh đề 2) rằng các tập hợp $\mathcal{B}_0(x)$ là các hệ lân cận của các điểm của $X$ đối với một tôpô trên $X$; gọi $X_0$ là không gian tôpô nhận được như vậy, và gọi $j : X_0 \to X$ là ánh xạ đồng nhất, liên tục nhưng nói chung không song liên tục. Một ánh xạ $f$ từ $X$ vào một không gian tôpô $X'$ là liên tục tại điểm $x_0$ nếu và chỉ nếu hợp thành $X_0 \xrightarrow{j} X \xrightarrow{f} X'$ là liên tục trên $X_0$; điều này suy ra ngay lập tức từ các định nghĩa.

### 2. SO SÁNH CÁC TÔPÔ

Định lý 2 của no. 1 cho thấy rằng ta có thể lấy các ánh xạ liên tục làm các cấu xạ của các cấu trúc tôpô (Lý thuyết tập hợp, Chương IV, § 2, no. 1); từ nay về sau, ta sẽ giả sử rằng ta đã thực hiện lựa chọn các cấu xạ này. Phù hợp với các định nghĩa tổng quát (Lý thuyết tập hợp, Chương IV, § 2, no. 2), điều đó cho phép ta định nghĩa một thứ tự trên tập hợp các tôpô trên một tập hợp đã cho $X$:

#### Định nghĩa 3 {#top-i-s2-def-3 .statement}

Cho hai tôpô $\mathcal{T}_1, \mathcal{T}_2$ trên cùng một tập hợp $X$, ta nói rằng $\mathcal{T}_1$ mịn hơn $\mathcal{T}_2$ (và $\mathcal{T}_2$ thô hơn $\mathcal{T}_1$) nếu, ký hiệu bởi $X_i$ tập hợp $X$ được trang bị tôpô $\mathcal{T}_i$ ($i = 1, 2$), ánh xạ đồng nhất $X_1 \to X_2$ là liên tục. Nếu thêm nữa $\mathcal{T}_1 \neq \mathcal{T}_2$, ta nói rằng $\mathcal{T}_1$ mịn hơn thực sự $\mathcal{T}_2$ (và $\mathcal{T}_2$ thô hơn thực sự $\mathcal{T}_1$).

Hai tôpô, trong đó một tôpô mịn hơn tôpô kia, được gọi là so sánh được.

Các tiêu chuẩn để một ánh xạ được liên tục (no. 1, Định nghĩa 1 và Định lý 1) cho mệnh đề sau:

#### Mệnh đề 3 {#top-i-s2-prop-3 .statement}

Cho hai tôpô $\mathcal{T}_1, \mathcal{T}_2$ trên một tập hợp $X$, các mệnh đề sau là tương đương:
a) $\mathcal{T}_1$ mịn hơn $\mathcal{T}_2$.
b) Với mỗi $x \in X$, mọi lân cận của $x$ đối với $\mathcal{T}_2$ đều là một lân cận của $x$ đối với $\mathcal{T}_1$.
c) Với mỗi tập con $A$ của $X$, bao đóng của $A$ trong tôpô $\mathcal{T}_1$ được chứa trong bao đóng của $A$ trong tôpô $\mathcal{T}_2$.
d) Mọi tập con của $X$ đóng trong $\mathcal{T}_2$ đều đóng trong $\mathcal{T}_1$.
e) Mọi tập con của $X$ mở trong $\mathcal{T}_2$ đều mở trong $\mathcal{T}_1$.

#### Ví dụ {#top-i-s2-n2-exa-1 .statement}

\* Trong không gian Hilbert $H$ gồm các dãy $x = (x_n)$ các số thực sao cho
$$
\|x\|^2 = \sum_{n=0}^\infty x_n^2 < +\infty,
$$
các lân cận của một điểm $x_0$ trong tôpô mạnh trên $H$ là các tập hợp chứa một quả cầu mở $\|x - x_0\| < \alpha$ có tâm tại $x_0$; các lân cận của $x_0$ trong tôpô yếu trên $H$ là các tập hợp chứa một tập hợp được xác định bởi một quan hệ có dạng $\sup_{1 \leq i \leq n} |(x - x_0|a_i)| \leq 1$, trong đó các $a_i$ là những điểm của $H$ và
$$
(x|y) = \sum_{n=0}^\infty x_n y_n
$$
nếu $x = (x_n)$ và $y = (y_n)$. Bây giờ nếu $\beta = \sup_{1 \leq i \leq n} \|a_i\|$, thì quan hệ $\|x - x_0\| \leq 1 / \beta$ suy ra $|(x - x_0|a_i)| \leq \|x - x_0\| \cdot \|a_i\| \leq 1$ với $1 \leq i \leq n$; do đó tôpô mạnh trên $H$ mịn hơn tôpô yếu. Mặt khác, với mọi họ hữu hạn $(a_i)_{1 \leq i \leq n}$ gồm các điểm của $H$, có những điểm $x$ trong $H$ sao cho $(x - x_0|a_i) = 0$ với $1 \leq i \leq n$ và sao cho $\|x - x_0\|$ lớn tùy ý; điều này cho thấy tôpô mạnh là mịn hơn thực sự so với tôpô yếu. \*

#### Nhận xét 1 {#top-i-s2-n2-rem-1 .statement}

Trong tập hợp có thứ tự của mọi tôpô trên một tập hợp $X$, tôpô mà các tập hợp mở duy nhất là $\varnothing$ và $X$ là thô nhất, và tôpô rời rạc là mịn nhất.
2) Tôpô càng mịn thì càng có nhiều tập hợp mở, tập hợp đóng và lân cận; tôpô càng mịn thì bao đóng của một tập hợp càng nhỏ (tương ứng, phần trong của nó càng lớn); tôpô càng mịn thì càng có ít tập hợp trù mật.
3) Nếu $f : X \to X'$ là một ánh xạ liên tục, thì nó vẫn liên tục nếu tôpô của $X$ được thay bằng một tôpô mịn hơn và tôpô của $X'$ được thay bằng một tôpô thô hơn (no. 1, Định lý 2). Nói cách khác, tôpô của $X$ càng mịn và tôpô của $X'$ càng thô thì càng có nhiều ánh xạ liên tục từ $X$ vào $X'$.

### 3. TÔPÔ BAN ĐẦU

#### Mệnh đề 4 {#top-i-s2-prop-4 .statement}

Cho $X$ là một tập hợp, cho $(Y_i)_{i \in I}$ là một họ các không gian tôpô, và với mỗi $i \in I$ cho $f_i$ là một ánh xạ từ $X$ vào $Y_i$. Gọi $\mathcal{S}$ là tập hợp các tập con của $X$ có dạng $\overline{f}_i^{-1}(U_i)$ ($i \in I$, $U_i$ mở trong $Y_i$), và gọi $\mathcal{B}$ là tập hợp các giao hữu hạn của các tập hợp thuộc $\mathcal{S}$. Khi đó $\mathcal{B}$ là một cơ sở của một tôpô $\mathcal{T}$ trên $X$, tôpô này là cấu trúc tôpô ban đầu trên $X$ đối với họ $(f_i)$ (Lý thuyết tập hợp, Chương IV, § 2, no. 3) và đặc biệt là tôpô thô nhất trên $X$ mà đối với nó các ánh xạ $f_i$ là liên tục. Chính xác hơn, nếu $g$ là một ánh xạ từ một không gian tôpô $Z$ vào $X$, thì $g$ liên tục tại một điểm $z \in Z$ (X mang tôpô $\mathcal{T}$) khi và chỉ khi mỗi ánh xạ hợp thành $f_i \circ g$ đều liên tục tại $z$.

Gọi $\mathcal{D}$ là tập hợp của mọi hợp của các tập hợp thuộc $\mathcal{B}$; rõ ràng $\mathcal{D}$ thỏa mãn tiên đề $(O_1)$ vì phép lập hợp là kết hợp; và $\mathcal{D}$ thỏa mãn tiên đề $(O_{II})$ do định nghĩa của $\mathcal{B}$ và việc giao hữu hạn có tính phân phối đối với hợp tùy ý [Lý thuyết tập hợp, R § 4, công thức (37)]. Vậy $\mathcal{D}$ là tập hợp các tập con mở của $X$ đối với một tôpô $\mathcal{T}$ mà $\mathcal{B}$ là một cơ sở. Ta sẽ chứng minh khẳng định cuối cùng của mệnh đề, điều này suy ra các khẳng định khác do các tính chất tổng quát của các cấu trúc ban đầu (Lý thuyết tập hợp, Chương IV, § 2, no. 3, tiêu chuẩn CST 9). Trước hết, định nghĩa của $\mathcal{S}$ cho thấy các $f_i$ liên tục trên $X$ (no. 1, Định lý 1); do đó, nếu $g$ liên tục tại $z$, thì các ánh xạ $f_i \circ g$ cũng vậy (no. 1, Mệnh đề 2). Ngược lại, giả sử rằng mọi ánh xạ $f_i \circ g$ đều liên tục tại $z$, và gọi $V$ là một lân cận của $g(z)$ trong $X$; theo định nghĩa, tồn tại một tập con hữu hạn $J$ của $I$, và với mỗi $i \in J$ một tập con mở $U_i$ của $Y_i$ sao cho $V$ chứa tập hợp $\bigcap_{i \in J} \overline{f}_i^{-1}(U_i)$ và $g(z)$ thuộc tập hợp này. Suy ra rằng
$$
\overline{g}^{-1}(V) \supset \bigcap_{i \in J} \overline{g}^{-1}(\overline{f}_i^{-1}(U_i)),
$$
và giả thiết kéo theo rằng mỗi tập hợp $\overline{g}^{-1}(\overline{f}_i^{-1}(U_i))$ là một lân cận của $z$ trong $Z$; do đó $\overline{g}^{-1}(V)$ cũng là một lân cận của $z$ trong $Z$. Điều này hoàn tất chứng minh.

Cho $\mathcal{B}_i$ là một cơ sở của tôpô của $Y_i (i \in I)$; gọi $\mathcal{S}'$ là tập hợp các tập con của $X$ có dạng $\overline{f}_i^{-1}(U_i)$ với $i \in I$ và $U_i \in \mathcal{B}_i$ đối với mỗi $i \in I$; nếu $\mathcal{B}'$ là tập hợp các giao hữu hạn của các tập thuộc $\mathcal{S}'$, thì hiển nhiên $\mathcal{B}'$ là một cơ sở của tôpô $\mathcal{T}$.

Các tính chất tổng quát của các cấu trúc ban đầu (Lý thuyết tập hợp, Chương IV, § 2, no. 3, tiêu chuẩn CST 10) đặc biệt kéo theo tính chất bắc cầu sau đây (mà chứng minh trực tiếp của nó khá dễ dàng):

#### Mệnh đề 5 {#top-i-s2-prop-5 .statement}

Cho $X$ là một tập hợp, $(Z_i)_{i \in I}$ là một họ các không gian tôpô, $(J_\lambda)_{\lambda \in L}$ là một phân hoạch của $I$ và $(Y_\lambda)_{\lambda \in L}$ là một họ các tập hợp được đánh chỉ số bởi $L$. Với mỗi $\lambda \in L$, cho $h_\lambda$ là một ánh xạ từ $X$ vào $Y_\lambda$; với mỗi $\lambda \in L$ và mỗi $i \in J_\lambda$, cho $g_{i\lambda}$ là một ánh xạ từ $Y_\lambda$ vào $Z_i$, và đặt $f_i = g_{i\lambda} \circ h_\lambda$. Nếu mỗi $Y_\lambda$ được trang bị tôpô thô nhất sao cho các ánh xạ $g_{i\lambda} (i \in J_\lambda)$ đều liên tục, thì tôpô thô nhất trên $X$ sao cho các $f_i$ liên tục cũng chính là tôpô thô nhất sao cho các $h_\lambda$ liên tục.

#### Ví dụ 1 {#top-i-s2-n3-exa-1 .statement}

Ảnh ngược của một tôpô. Cho $X$ là một tập hợp, $Y$ là một không gian tôpô, $f$ là một ánh xạ từ $X$ vào $Y$; tôpô thô nhất $\mathcal{T}$ trên $X$ sao cho $f$ liên tục được gọi là ảnh ngược theo $f$ của tôpô của $Y$. Suy ra từ Mệnh đề 4 và các công thức về ảnh ngược của một hợp và một giao [Lý thuyết tập hợp, R, § 4, các công thức (34) và (46)] rằng các tập hợp mở (tương ứng đóng) trong tôpô $\mathcal{T}$ là các ảnh ngược theo $f$ của các tập hợp mở (tương ứng đóng) của $Y$; do đó, với mỗi $x \in X$, các tập hợp $f^{-1}(W)$, trong đó $W$ chạy qua một hệ cơ bản các lân cận của $f(x)$ trong $Y$, tạo thành một hệ cơ bản các lân cận của $x$ trong tôpô $\mathcal{T}$. Trong § 3 chúng ta sẽ nghiên cứu, dưới tên gọi tôpô cảm sinh, trường hợp riêng trong đó $X$ là một tập con của $Y$ và $f$ là đơn ánh chính tắc $X \to Y$; khi đó $X$, với tôpô cảm sinh, được gọi là một không gian con của $Y$.

Để một ánh xạ $f$ từ một không gian tôpô $X$ vào một không gian tôpô $X'$ là liên tục thì điều kiện cần và đủ là tôpô của $X$ mịn hơn ảnh ngược theo $f$ của tôpô của $X'$.

#### Ví dụ 2 {#top-i-s2-n3-exa-2 .statement}

Cận trên bé nhất của một tập hợp các tôpô. Mọi họ $(\mathcal{T}_i)_{i \in I}$ các tôpô trên một tập hợp $X$ đều có một cận trên bé nhất $\mathcal{T}$ trong tập hợp có thứ tự của mọi tôpô trên $X$, tức là tồn tại một tôpô trên $X$ là thô nhất trong tất cả các tôpô trên $X$ mịn hơn mỗi $\mathcal{T}_i$. Để thấy điều này, ta có thể áp dụng Mệnh đề 4, lấy $Y_i$ là tập hợp $X$ với tôpô $\mathcal{T}_i$, và $f_i$ là ánh xạ đồng nhất $X \to Y_i$; $\mathcal{T}$ là tôpô thô nhất sao cho mọi ánh xạ $f_i$ đều liên tục.

Cho $\mathfrak{S}$ là một tập hợp tùy ý các tập hợp con của một tập hợp $X$; trong các tôpô $\mathcal{T}$ trên $X$ mà đối với chúng các tập hợp của $\mathfrak{S}$ là mở, có một tôpô $\mathcal{T}_0$ thô hơn tất cả các tôpô khác và được gọi là tôpô sinh bởi $\mathfrak{S}$. Với mỗi tập hợp $U \in \mathfrak{S}$ gọi $\mathcal{T}_U$ là tôpô mà các tập hợp mở là $\varnothing, U$ và $X$ [rõ ràng tập hợp này các tập hợp con của $X$ thỏa mãn (O_I) và (O_{II})]; khi đó $\mathcal{T}_0$ chính là cận trên bé nhất của các tôpô $\mathcal{T}_U$. Theo Mệnh đề 4, nếu $\mathfrak{B}$ là tập hợp các giao hữu hạn của các tập hợp thuộc $\mathfrak{S}$, thì $\mathfrak{B}$ là một cơ sở của tôpô $\mathcal{T}_0$. Ta nói rằng $\mathfrak{S}$ là một tiền cơ sở của $\mathcal{T}_0$.

#### Ví dụ 3 {#top-i-s2-n3-exa-3 .statement}

Tôpô tích. Cho $(X_i)_{i \in I}$ là một họ các không gian tôpô. Tôpô thô nhất trên tập tích $X = \prod_{i \in I} X_i$ mà đối với nó các phép chiế-

### 4. TÔPÔ CUỐI CÙNG

#### Mệnh đề 6 {#top-i-s2-prop-6 .statement}

*Cho $X$ là một tập hợp, cho $(Y_i)_{i \in I}$ là một họ các không gian tôpô, và với mỗi $i \in I$ cho $f_i$ là một ánh xạ từ $Y_i$ vào $X$. Gọi $\mathcal{D}$ là tập hợp các tập con $U$ của $X$ sao cho $\overline{f}_i^{-1}(U)$ là mở trong $Y_i$ với mọi $i \in I$; khi đó $\mathcal{D}$ là tập hợp các tập con mở của $X$ trong một tôpô $\mathcal{T}$ trên $X$ là cấu trúc cuối cùng trên $X$ đối với họ $(f_i)$ (Lý thuyết tập hợp, Chương IV, § 2, no. 5), và đặc biệt $\mathcal{T}$ là tôpô mịn nhất trên $X$ sao cho các ánh xạ $f_i$ là liên tục. Nói cách khác, nếu $g$ là một ánh xạ từ $X$ vào một không gian tôpô $Z$, thì $g$ là liên tục ($X$ mang tôpô $\mathcal{T}$) khi và chỉ khi mỗi ánh xạ $g \circ f_i$ là liên tục.*

Người ta kiểm tra ngay lập tức rằng $\mathcal{D}$ thỏa mãn các tiên đề $(O_I)$ và $(O_{II})$. [Lý thuyết tập hợp, R, § 4, các công thức (34) và (46)]. Ta sẽ chứng minh khẳng định cuối cùng của mệnh đề, điều này suy ra các mệnh đề khác do các tính chất tổng quát của các cấu trúc cuối cùng (Lý thuyết tập hợp, Chương IV, § 2, no. 5, tiêu chuẩn CST 18). Rõ ràng là các $f_i$ liên tục đối với tôpô $\mathcal{T}$, theo định nghĩa của $\mathcal{D}$ (no. 1, Định lý 1); do đó nếu $g$ liên tục thì mỗi ánh xạ $g \circ f_i$ cũng liên tục (no. 1, Định lý 2). Ngược lại, giả sử rằng mỗi $g \circ f_i$ đều liên tục, và gọi $V$ là một tập hợp mở trong $Z$; theo giả thiết, $\overline{f}_i^{-1}(\overline{g}^{-1}(V))$ là mở trong $Y_i$ với mọi $i \in I$; do đó $\overline{g}^{-1}(V) \in \mathcal{D}$, và chứng minh là đầy đủ.

#### Hệ quả {#top-i-s2-n4-cor-1 .statement}

*Dưới các giả thiết của Mệnh đề 6, một tập con $F$ của $X$ là đóng trong tôpô $\mathcal{T}$ khi và chỉ khi $\overline{f}_i^{-1}(F)$ là đóng trong $Y_i$ với mọi $i \in I$.*

Điều này suy ra từ định nghĩa của các tập mở trong tôpô $\mathcal{T}$ bằng cách lấy phần bù.

Các tính chất tổng quát của các cấu trúc cuối (Lý thuyết tập hợp, Chương IV, § 2, no. 5, criterion CST 19) suy ra tính chất *tính bắc cầu* sau đây (mà chứng minh trực tiếp của nó cũng là hiển nhiên):

#### Mệnh đề 7 {#top-i-s2-prop-7 .statement}

*Cho $X$ là một tập hợp, $(Z_i)_{i \in I}$ là một họ các không gian tôpô, $(J_\lambda)_{\lambda \in L}$ là một phân hoạch của $I$, và $(Y_\lambda)_{\lambda \in L}$ là một họ các tập hợp được đánh chỉ số bởi $L$. Hơn nữa, với mỗi $\lambda \in L$ gọi $h_\lambda$ là một ánh xạ từ $Y_\lambda$ vào $X$; với mỗi $\lambda \in L$ và mỗi $i \in J_\lambda$ gọi $g_{\lambda i}$ là một ánh xạ từ $Z_i$ vào $Y_\lambda$, và đặt $f_i = h_\lambda \circ g_{\lambda i}$. Nếu mỗi $Y_\lambda$ được trang bị tôpô mịn nhất sao cho các ánh xạ $g_{\lambda i} (i \in J_\lambda)$ là liên tục, thì tôpô mịn nhất trên $X$ sao cho các $f_i$ là liên tục cũng chính là tôpô mịn nhất sao cho các $h_\lambda$ là liên tục.*

Ví dụ

1) Tôpô thương. Cho $X$ là một không gian tôpô, $R$ là một quan hệ tương đương trên $X$, $Y = X/R$ là tập thương của $X$ đối với quan hệ $R$, $\varphi : X \to Y$ là ánh xạ chính tắc. Tôpô mịn nhất trên $Y$ sao cho $\varphi$ liên tục được gọi là tôpô thương của tôpô trên $X$ theo quan hệ $R$; chúng tôi sẽ nghiên cứu nó chi tiết hơn trong § 3.

2) Cận dưới lớn nhất của một tập hợp các tôpô. Mọi họ $(\mathcal{T}_i)_{i \in I}$ các tôpô trên một tập hợp $X$ đều có một cận dưới lớn nhất $\mathcal{T}$ trong tập hợp tất cả các tôpô trên $X$, tức là $\mathcal{T}$ là tôpô mịn nhất trong tất cả các tôpô trên $X$ thô hơn mỗi $\mathcal{T}_i$. Để thấy điều đó, ta có thể áp dụng Mệnh đề 6, lấy $Y_i$ là tập hợp $X$ được trang bị tôpô $\mathcal{T}_i$, và $f_i$ là ánh xạ đồng nhất $Y_i \to X$. Nếu $\mathcal{D}_i$ là tập hợp các tập con của $X$ mở trong tôpô $\mathcal{T}_i$, thì tập hợp $\bigcap_{i \in I} \mathcal{D}_i$ là tập hợp các tập con của $X$ mở trong $\mathcal{T}$. $\mathcal{T}$ cũng được gọi là giao của các tôpô $\mathcal{T}_i$.

3) Tổng của các không gian tôpô. Cho $(X_i)_{i \in I}$ là một họ các không gian tôpô, $X$ là tập hợp là tổng của các $X_i$ (Lý thuyết Tập hợp, Chương II, § 4, no. 8, Định nghĩa 8); với mỗi $i \in I$, gọi $j_i$ là ánh xạ chính tắc (đơn ánh) từ $X_i$ vào $X$. Tôpô mịn nhất $\mathcal{T}$ trên $X$ mà đối với nó các ánh xạ $j_i$ đều liên tục được gọi là tổng của các tôpô của các $X_i$, và $X$ với tôpô này được gọi là tổng của các không gian tôpô $X_i$. Đồng nhất mỗi $X_i$ với một tập con của $X$ nhờ $j_i$; khi đó một tập hợp $A \subset X$ là mở (resp. đóng) trong tôpô $\mathcal{T}$ khi và chỉ khi mỗi tập hợp $A \cap X_i$ là mở (resp. đóng) trong $X_i$. Đặc biệt, mỗi $X_i$ vừa mở vừa đóng.

Mệnh đề sau tổng quát hóa tình huống của Ví dụ 3:

#### Mệnh đề 8 {#top-i-s2-prop-8 .statement}

Cho $X$ là một tập hợp, $(X_\lambda)_{\lambda \in L}$ là một họ các tập hợp con của $X$. Giả sử mỗi $X_\lambda$ được trang bị một tôpô $\mathcal{T}_\lambda$ sao cho, với mỗi cặp chỉ số $(\lambda, \mu)$:
1) $X_\lambda \cap X_\mu$ là mở (tương ứng đóng) trong mỗi tôpô $\mathcal{T}_\lambda, \mathcal{T}_\mu$.
2) Các tôpô cảm sinh trên $X_\lambda \cap X_\mu$ bởi $\mathcal{T}_\lambda$ và $\mathcal{T}_\mu$ trùng nhau. Gọi $\mathcal{T}$ là tôpô mịn nhất trên $X$ mà đối với nó các ánh xạ nhúng $j_\lambda : X_\lambda \to X$ là liên tục. Khi đó, với mỗi $\lambda \in L$, $X_\lambda$ là mở (tương ứng đóng) trong $X$ đối với tôpô $\mathcal{T}$, và tôpô cảm sinh bởi $\mathcal{T}$ trên $X_\lambda$ trùng với $\mathcal{T}_\lambda$.

Xét theo Mệnh đề 6 và hệ quả của nó, chỉ cần chỉ ra rằng đối với mỗi $\lambda$ và mỗi tập con $A_\lambda$ của $X_\lambda$ thì các mệnh đề sau là tương đương:
(i) $A_\lambda$ là mở (tương ứng, đóng) trong tôpô $\mathcal{T}_\lambda$.
(ii) Với mọi $\mu \in L$, $A_\lambda \cap X_\mu$ là mở (tương ứng, đóng) trong tôpô $\mathcal{T}_\mu$.

Hiển nhiên là (ii) kéo theo (i) khi lấy $\mu = \lambda$. Ngược lại, nếu (i) được thỏa mãn, thì $A_\lambda \cap X_\mu$ là mở (tương ứng, đóng) trong $X_\lambda \cap X_\mu$ đối với tôpô $\mathcal{T}_{\lambda \mu}$ cảm sinh trên $X_{\lambda} \cap X_{\mu}$ bởi $\mathcal{T}_{\lambda}$; nhưng $\mathcal{T}_{\lambda \mu}$ cũng là tôpô cảm sinh trên $X_{\lambda} \cap X_{\mu}$ bởi $\mathcal{T}_{\mu}$; do đó $A_{\lambda} \cap X_{\mu}$ cũng là giao của $X_{\lambda} \cap X_{\mu}$ với một tập con $B_{\mu}$ của $X_{\mu}$ mở (tương ứng, đóng) trong tôpô $\mathcal{T}_{\mu}$; vì $X_{\lambda} \cap X_{\mu}$ là mở (tương ứng, đóng) trong $\mathcal{T}_{\mu}$, nên $A_{\lambda} \cap X_{\mu}$ cũng vậy. Điều này kết thúc chứng minh.

Ta nhận xét rằng nếu hợp của các $X_{\lambda}$ khác $X$, thì tôpô cảm sinh bởi $\mathcal{T}$ trên $X - \left( \bigcup_{\lambda \in L} X_{\lambda} \right)$ là *rời rạc*. Thật vậy, nếu $x \in X$ không thuộc một $X_{\lambda}$ nào, thì $\{ x \} \cap X_{\lambda} = \varnothing$ là mở trong mỗi tôpô $\mathcal{T}_{\lambda}$ và do đó $\{ x \}$ là mở trong tôpô $\mathcal{T}$.

### 5. DÁN CÁC KHÔNG GIAN TÔPÔ LẠI VỚI NHAU

Cho $(X_{\lambda})_{\lambda \in L}$ là một họ các tập hợp, và cho $X$ là tập hợp là *tổng* của các $X_{\lambda}$ (*Lý thuyết tập hợp*, Chương II, § 4, no. 8, Định nghĩa 8); ta sẽ đồng nhất mỗi $X_{\lambda}$ với một tập con của $X$ nhờ đơn ánh chính tắc $j_{\lambda} : X_{\lambda} \to X$.

Cho $R$ là một quan hệ tương đương trên $X$ sao cho *mỗi lớp tương đương của* $R$ *có nhiều nhất một phần tử trong mỗi* $X_{\lambda}$; với mỗi cặp chỉ số $(\lambda, \mu)$ đặt $A_{\lambda \mu}$ là tập con của $X_{\lambda}$ gồm các phần tử $x$ sao cho tồn tại một phần tử $y \in X_{\mu}$ thuộc lớp tương đương của $X$. Rõ ràng ứng với mỗi $x \in A_{\lambda \mu}$ có một $y \in A_{\mu \lambda}$ duy nhất đồng dư với $x$ mod $R$; các ánh xạ $h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$ được xác định như vậy thỏa mãn các điều kiện sau:

(i) Với mọi $\lambda \in L$, $h_{\lambda \lambda}$ là ánh xạ đồng nhất của $A_{\lambda \lambda} = X_{\lambda}$.

(ii) Với mỗi bộ ba chỉ số $(\lambda, \mu, \nu)$ của $L$ và mọi $x \in A_{\lambda \mu} \cap A_{\lambda \nu}$, ta có $h_{\mu \lambda}(x) \in A_{\mu \nu}$ và

$$
h_{\nu \lambda}(x) = h_{\nu \mu}(h_{\mu \lambda}(x)).
$$

*Ngược lại*, giả sử rằng với mỗi cặp chỉ số $(\lambda, \mu)$ ta được cho một tập con $A_{\lambda \mu}$ của $X_{\lambda}$ và một ánh xạ $h_{\mu \lambda} : A_{\lambda \mu} \to A_{\mu \lambda}$ thỏa mãn các điều kiện (i) và (ii) ở trên. Trước hết suy ra từ (ii) áp dụng cho các bộ ba $(\lambda, \mu, \lambda)$ và $(\mu, \lambda, \mu)$ rằng $h_{\lambda \mu} \circ h_{\mu \lambda}$ (tương ứng $h_{\mu \lambda} \circ h_{\lambda \mu}$) là hạn chế của $h_{\lambda \lambda}$ (tương ứng $h_{\mu \mu}$) lên $A_{\lambda \mu}$ (tương ứng $A_{\mu \lambda}$); do đó ta suy ra từ (i) rằng $h_{\lambda \mu}$ và $h_{\mu \lambda}$ là các *song ánh* nghịch đảo của nhau. Bây giờ, gọi $R \{ x, y \}$ là quan hệ "tồn tại $\lambda, \mu$ sao cho $x \in A_{\lambda \mu}$, $y \in A_{\mu \lambda}$ và $y = h_{\mu \lambda}(x)$". Từ (i) và từ điều đi trước suy ra rằng $R$ là *phản xạ* và *đối xứng*; mặt khác, nếu $x \in A_{\lambda \mu}$,

$$
y = h_{\mu \lambda}(x) \in A_{\mu \lambda} \cap A_{\mu \nu} \quad \text{và} \quad z = h_{\nu \mu}(y),
$$

khi đó cũng có $x = h_{\lambda \mu}(y)$ và do đó, theo (ii), $x \in A_{\lambda \mu} \cap A_{\lambda \nu}$; vì thế hệ thức (i) cho thấy $R$ là *bắc cầu*, và do đó $R$ là một quan hệ tương đương trên $X$. Cũng từ (i) và từ định nghĩa của $R$ suy ra rằng mỗi lớp tương đương theo mod $R$ có nhiều nhất một phần tử trong mỗi tập hợp $X_\lambda$, và rằng $A_{\lambda \mu}$ là tập hợp của mọi $x \in X_\lambda$ sao cho tồn tại một phần tử $y \in X_\mu$ tương đương với $x$ theo mod $R$. Ta nói rằng tập thương $X/R$ thu được bằng cách *dán các* $X_\lambda$ *lại với nhau dọc theo các* $A_{\lambda \mu}$ *nhờ các song ánh* $h_{\mu \lambda}$. Nếu $\varphi : X \to X/R$ là ánh xạ chính tắc, thì hạn chế của $\varphi$ trên mỗi $X_\lambda$ là một *song ánh* từ $X_\lambda$ lên $\varphi(X_\lambda)$.

Bây giờ giả sử rằng mỗi $X_\lambda$ là một *không gian tôpô*, và gọi $\mathcal{T}_\lambda$ là tôpô của nó. Gọi $\mathcal{T}$ là tôpô mịn nhất trên tập hợp $X/R$ sao cho các ánh xạ $\varphi \circ j_\lambda$ là liên tục; $\mathcal{T}$ là thương theo $R$ của tôpô trên $X$ là *tổng* của các tôpô $\mathcal{T}_\lambda$. Ta nói rằng không gian tôpô $X/R$ (với tôpô $\mathcal{T}$) thu được bằng cách *dán các không gian tôpô* $X_\lambda$ *dọc theo các* $A_{\lambda \mu}$ *bằng các song ánh* $h_{\mu \lambda}$. Khi đó, các tập con *mở* (ứng với *đóng*) của $X/R$ là các ảnh chính tắc của các tập con $B$ của $X$ *bão hòa* đối với $R$ và sao cho $B \cap X_\lambda$ là *mở* (ứng với *đóng*) trong $X_\lambda$ với mỗi $\lambda \in L$.

Vì hạn chế của $\varphi$ trên mỗi $X_\lambda$ là một song ánh lên tập con $X'_\lambda = \varphi(X_\lambda)$ của $X/R$, ta có thể chuyển tôpô $\mathcal{T}_\lambda$ sang $X'_\lambda$ bằng song ánh này, sao cho $X'_\lambda$ mang một tôpô $\mathcal{T}'_\lambda$; và tôpô $\mathcal{T}$ trên $X/R$ là tôpô *mịn nhất* mà đối với nó các đơn ánh chính tắc $X'_\lambda \to X/R$ là liên tục. Nói chung, tôpô cảm sinh bởi $\mathcal{T}$ trên $X'_\lambda$ *thô hơn* $\mathcal{T}'_\lambda$, nhưng không đồng nhất với tôpô sau; ngay cả khi các $h_{\mu \lambda}$ là những đồng phôi (§ 3, Bài tập 15). Tuy nhiên, suy ra từ no. 4, Mệnh đề 8 rằng, với các ký hiệu trên đây:

#### Mệnh đề 9 {#top-i-s2-prop-9 .statement}

*Giả sử các* $h_{\mu \lambda}$ *là các đồng phôi và mỗi* $A_{\lambda \mu}$ *là mở (tương ứng, đóng)* *trong* $X_\lambda$; *khi đó mỗi* $\varphi(X_\lambda)$ *là mở (tương ứng, đóng)* *trong* $X/R$ *và hạn chế của* $\varphi$ *trên* $X_\lambda$ *là một đồng phôi từ* $X_\lambda$ *lên không gian con* $\varphi(X_\lambda)$ *của* $X/R$.

### Bài tập {#top-i-s2-exercises}

Xem [bài tập của § 2](exercises/s2/).
