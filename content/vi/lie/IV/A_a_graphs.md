---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 0
section_title: Graphs
appendix: true
lang: vi
source: lie-iv-vi
pdf_pages: 0040-0043
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITIONS
      page: 0
      pdf_page: 40
    - "no": 2
      title: CONNECTED COMPONENTS OF A GRAPH
      page: 0
      pdf_page: 40
    - "no": 3
      title: FORESTS AND TREES
      page: 0
      pdf_page: 42
statements: 6
exercises: 0
content_sha256: 4853ee9340ab9b11e2c135d73fe1a91dfe0af274b213a577c6d705eaa5476caa
translated_from: content/en/lie/IV/A_a_graphs.md
source_content_sha256: eac22a0040474678cfb62df408ef3ef6cb1dc27c07113e0e6b8e5da22b5af9c4
translation_model: gpt-5.4
translation_run: translate-vi-23269868
glossary_version: 34
glossary_terms_sha256: a89f9690ed2243cd33eb088f5f45bbb7c6744c189ab69f76b43e9bf2ac2bf878
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC
# ĐỒ THỊ

### 1. ĐỊNH NGHĨA

#### Định nghĩa 1 {#lie-iv-a0-def-1 .statement}

*Một đồ thị tổ hợp (hay đơn giản là một đồ thị, nếu không có nguy cơ nhầm lẫn) là một cặp* $(\mathbf{A}, S)$, *trong đó S là một tập hợp và A là một tập con của $\mathfrak{P}(S)$ gồm các tập hợp có hai phần tử.*

Cho $\Gamma = (\mathbf{A}, S)$ là một đồ thị. Các phần tử của $\mathbf{A}$ được gọi là các *cạnh* và các phần tử của S được gọi là các *đỉnh* của $\Gamma$; hai đỉnh được gọi là *nối với nhau* nếu $\{x, y\}$ là một cạnh. Một đỉnh được gọi là *đầu mút* nếu nó nối với nhiều nhất một đỉnh, và là một *điểm phân nhánh* nếu nó nối với ít nhất ba đỉnh.

Phù hợp với các định nghĩa tổng quát (*Tập hợp R*, §8), một *đẳng cấu* từ đồ thị $\Gamma$ đến một đồ thị $\Gamma' = (\mathbf{A}', S')$ là một song ánh từ S đến S' biến $\mathbf{A}$ thành $\mathbf{A}'$. Một đồ thị $\Gamma' = (\mathbf{A}', S')$ được gọi là một *đồ thị con* của $\Gamma$ nếu $S' \subset S$ và $\mathbf{A}' \subset \mathbf{A}$; $\Gamma$ được gọi là một *đồ thị con đầy* của $\Gamma$ nếu $S' \subset S$ và $\mathbf{A}' = \mathbf{A} \cap \mathfrak{P}(S)$. Rõ ràng là mọi tập con của S đều là tập hợp các đỉnh của đúng một đồ thị con đầy của $\Gamma$.

Để cho các lập luận dễ theo dõi hơn, ta biểu diễn một đồ thị bằng một biểu đồ gồm các điểm tương ứng với các đỉnh, hai điểm được nối với nhau bằng một đường khi và chỉ khi các đỉnh mà chúng biểu diễn được nối với nhau trong đồ thị. Ví dụ, biểu đồ

![Biểu đồ của một đồ thị với các đỉnh a, b, c, d, e và các cạnh {a, b}, {b, c}, {c, d}, {c, e}](https://i.imgur.com/3Q5z5QG.png)

biểu diễn một đồ thị có các đỉnh là $a, b, c, d, e$ và các cạnh là $\{a, b\}, \{b, c\}, \{c, d\}$ và $\{c, e\}$.

### 2. CÁC THÀNH PHẦN LIÊN THÔNG CỦA MỘT ĐỒ THỊ

Cho $\Gamma = (\mathbf{A}, S)$ là một đồ thị. Nếu $a$ và $b$ là hai đỉnh, một *đường đi* nối $a$ và $b$ là một dãy $(x_0, \ldots, x_n)$ các đỉnh của $\Gamma$ với $x_0 = a, x_n = b$, các đỉnh $x_i$ và $x_{i+1}$ được nối với nhau với $0 \leq i < n$; số nguyên $n \geq 0$ là *độ dài* của đường đi. Đường đi $(x_0, \ldots, x_n)$ được gọi là đơn ánh nếu $x_i \neq x_j$ khi $i \neq j$. Nếu một đường đi $(x_0, \ldots, x_n)$ nối $a$ và $b$ có độ dài cực tiểu trong số các đường đi như vậy, thì nó tất yếu là đơn ánh; vì nếu không, sẽ tồn tại $i$ và $j$ với $0 \leq i < j \leq n$ và $x_i = x_j$, và khi đó dãy

$$
(x_0, \ldots, x_i, x_{j+1}, \ldots, x_n)
$$

sẽ là một đường đi có độ dài $< n$ nối $a$ và $b$.

Quan hệ "tồn tại một đường đi nối $a$ và $b$" giữa hai đỉnh $a$ và $b$ của $\Gamma$ là một quan hệ tương đương $R$ trên tập hợp $S$ các đỉnh. Các lớp tương đương của $R$ được gọi là các *thành phần liên thông* của $\Gamma$; và $\Gamma$ được gọi là *liên thông* nếu $S$ có nhiều nhất một thành phần liên thông, nghĩa là nếu bất kỳ hai đỉnh nào của $\Gamma$ đều có thể được nối với nhau bằng ít nhất một đường đi.

#### Mệnh đề 1 {#lie-iv-a0-prop-1 .statement}

*Cho $\Gamma = (A, S)$ là một đồ thị và $(S_\alpha)_{\alpha \in L}$ là họ các thành phần liên thông của nó. Ký hiệu bởi $\Gamma_\alpha$ đồ thị con đầy đủ của $\Gamma$ có $S_\alpha$ làm tập hợp các đỉnh của nó.*

(i) *Với mọi $\alpha$ trong $L$, đồ thị $\Gamma_\alpha$ là liên thông.*
(ii) *Nếu $\Gamma' = (A', S')$ là một đồ thị con liên thông của $\Gamma$, thì tồn tại $\alpha$ trong $L$ sao cho $\Gamma' \subset \Gamma_\alpha$.*
(iii) *Nếu $\alpha \neq \beta$, không phần tử nào của $S_\alpha$ được nối trong $\Gamma$ với bất kỳ phần tử nào của $S_\beta$ (tương đương, mọi cạnh của $\Gamma$ là một cạnh của một trong các $\Gamma_\alpha$).*
(iv) *Cho $(S'_\lambda)_{\lambda \in M}$ là một phân hoạch của $S$ sao cho, nếu $\lambda \neq \mu$, không phần tử nào của $S'_\lambda$ được nối trong $\Gamma$ với bất kỳ phần tử nào của $S'_\mu$; khi đó mỗi tập hợp $S'_\lambda$ là một hợp của các thành phần liên thông của $\Gamma$.*

(i) Cho $\alpha$ thuộc $L$ và $a$ và $b$ thuộc $S_\alpha$. Khi đó tồn tại một đường đi $c = (x_0, \ldots, x_n)$ nối $a$ với $b$ trong $\Gamma$. Với mọi $i$ sao cho $0 \leq i \leq n$, đường đi $(x_0, \ldots, x_i)$ nối $a$ với $x_i$ trong $\Gamma$, nên $x_i \in S_\alpha$. Do đó, $c$ là một đường đi *trong* $\Gamma_\alpha$ nối $a$ với $b$. Suy ra $\Gamma_\alpha$ là liên thông.

(ii) Cho $\Gamma' = (A', S')$ là một đồ thị con liên thông không rỗng của $\Gamma$, cho $a$ là một phần tử của $S'$ và cho $S_\alpha$ là thành phần liên thông của $S$ chứa $a$. Với mọi $b$ trong $S'$, tồn tại một đường đi $c$ nối $a$ và $b$ trong $\Gamma'$, và *a fortiori* trong $\Gamma$. Suy ra $S' \subset S_\alpha$.

(iii) Cho các phần tử phân biệt $\alpha$ và $\beta$ của $L$, và các đỉnh $a \in S_\alpha$ và $b \in S_\beta$, không có đường đi nào nối $a$ với $b$, và đặc biệt không có cạnh nào nối $a$ với $b$.

(iv) Cho $a$ thuộc $S'_\lambda$ và gọi $S_\alpha$ là thành phần liên thông của $\Gamma$ chứa $a$. Khi đó, với mọi $b$ thuộc $S_\alpha$, tồn tại một đường đi $(x_0, \ldots, x_n)$ nối $a$ với $b$ trong $\Gamma$. Nếu $i$ là một số nguyên sao cho $0 \leq i < n$ và nếu $x_i \in S'_\lambda$, thì $x_{i+1} \in S'_\lambda$ vì $x_i$ được nối với $x_{i+1}$. Suy ra bằng quy nạp rằng $x_i \in S'_\lambda$ với $0 \leq i \leq n$, và đặc biệt là $b = x_n$ thuộc $S'_\lambda$. Vậy, $S_\alpha \subset S'_\lambda$.

#### Hệ quả 1 {#lie-iv-a0-prop-1-cor-1 .statement}

*Một đồ thị $\Gamma = (A, S)$ là liên thông nếu và chỉ nếu không tồn tại một phân hoạch $(S', S'')$ của $S$ thành hai tập hợp con không rỗng sao cho không có phần tử nào của $S'$ được nối trong $\Gamma$ với bất kỳ phần tử nào của $S''$.*

Giả sử rằng $\Gamma$ không liên thông và gọi $S'$ là một trong các thành phần liên thông của nó. Tập hợp $S'' = S - S'$ là không rỗng theo Mệnh đề 1, (i) và không có phần tử nào của $S'$ được nối với bất kỳ phần tử nào của $S''$ theo Mệnh đề 1, (iii).

Giả sử bây giờ rằng $\Gamma$ là liên thông và cho $(S', S'')$ là một phân hoạch có tính chất đã nêu. Theo Mệnh đề 1, (iv), tập hợp $S'$ chứa ít nhất một thành phần liên thông, nên $S' = S$ và $S'' = \varnothing$, mâu thuẫn.

#### Hệ quả 2 {#lie-iv-a0-prop-1-cor-2 .statement}

*Một tập con $S'$ của $S$ là một hợp các thành phần liên thông khi và chỉ khi không có đỉnh nào thuộc $S'$ được nối với một đỉnh nào thuộc $S - S'$.*

Điều kiện này là đủ theo Mệnh đề 1, (iv). Nó là cần thiết theo Mệnh đề 1, (iii).

### 3. RỪNG VÀ CÂY

Cho $\Gamma = (A, S)$ là một đồ thị. Một *chu trình* của $\Gamma$ là một dãy

$$
(x_1, \ldots, x_n)
$$

của các đỉnh phân biệt của $\Gamma$ sao cho $n \geq 3$, $x_i$ được nối với $x_{i+1}$ với $1 \leq i < n$ và $x_n$ được nối với $x_1$. $\Gamma$ được gọi là một *rừng* nếu không có chu trình nào trong $\Gamma$; khi đó mọi đồ thị con của $\Gamma$ cũng là một rừng. Một rừng liên thông được gọi là một *cây*; do đó các thành phần liên thông của một rừng là các cây.

#### Mệnh đề 2 {#lie-iv-a0-prop-2 .statement}

*Cho $\Gamma = (A, S)$ là một rừng chỉ có một số hữu hạn đỉnh.*

(i) *Nếu $\Gamma$ có ít nhất một đỉnh, thì nó có một đỉnh tận cùng.*
(ii) *Nếu $\Gamma$ có ít nhất hai đỉnh, thì tồn tại một phân hoạch $(S', S'')$ của tập hợp các đỉnh của nó thành hai tập con không rỗng sao cho hai đỉnh phân biệt cùng thuộc $S'$ hoặc cùng thuộc $S''$ không bao giờ được nối với nhau.*

Giả sử rằng $\Gamma$ có ít nhất một đỉnh và cho $(x_0, \ldots, x_n)$ là một đường đi đơn ánh có độ dài cực đại trong $\Gamma$. Đỉnh $x_0$ không thể được nối với một đỉnh $y$ phân biệt với $x_0, x_1, \ldots, x_n$, vì nếu không thì sẽ tồn tại một đường đi đơn ánh trong $\Gamma$ có độ dài $n + 1$, cụ thể là $(y, x_0, \ldots, x_n)$. Đỉnh $x_0$ không được nối với bất kỳ đỉnh nào $x_i$ với $2 \leq i \leq n$, vì nếu không thì $(x_0, x_1, \ldots, x_i)$ sẽ là một chu trình trong rừng $\Gamma$. Vậy $x_0$ là đầu mút.

Ta sẽ chứng minh (ii) bằng quy nạp theo số $m$ đỉnh của $\Gamma$, trường hợp $m = 2$ là tầm thường. Giả sử khi đó $m \geq 3$ và mệnh đề (ii) đã được chứng minh cho các đồ thị có $m - 1$ đỉnh. Gọi $a$ là một đỉnh tận cùng của $\Gamma$ (x. (i)). Ta áp dụng giả thiết quy nạp cho đồ thị con đầy đủ của $\Gamma$ mà các đỉnh là các đỉnh $x \neq a$ của $\Gamma$. Do đó, tồn tại hai tập con rỗng khác nhau $S'_1$ và $S''_1$ của $S$ sao cho $S'_1 \cup S''_1 = S - \{a\}$, và sao cho hai đỉnh phân biệt của $S'_1$ (tương ứng $S''_1$) không bao giờ được nối với nhau. Vì $a$ được nối với nhiều nhất một đỉnh của $\Gamma$, chẳng hạn ta có thể giả sử rằng nó không được nối với bất kỳ đỉnh nào trong $S'_1$. Khi đó phân hoạch $(S'_1, S''_1 \cup \{a\})$ có tính chất cần có. ĐPCM.

Với mọi số nguyên $n \geq 1$, ký hiệu $A_n$ là đồ thị mà các đỉnh là các số nguyên $1, 2, \ldots, n$ và các cạnh là các cặp $\{i, j\}$ với $i - j = \pm 1$:

$$
\begin{array}{cccccc}
1 & 2 & 3 & n-1 & n \\
\circ & \circ & \circ & \cdots & \circ
\end{array}
$$

Một đồ thị $\Gamma$ được gọi là một chuỗi độ dài $m \geq 0$ nếu nó đẳng cấu với $A_{m+1}$. Điều này tương đương với sự tồn tại trong $\Gamma$ của một đường đi đơn ánh $(x_0, \ldots, x_m)$ chứa tất cả các đỉnh, trong đó các đỉnh $x_i$ và $x_j$ không được nối với nhau nếu $|i - j| > 1$.

#### Mệnh đề 3 {#lie-iv-a0-prop-3 .statement}

*Một đồ thị là một chuỗi khi và chỉ khi số đỉnh của nó là hữu hạn và khác không, và nó là một cây không có điểm phân nhánh.*

Giả sử rằng đồ thị $\Gamma$ là một xích $(x_0, \ldots, x_m)$ có các tính chất được liệt kê trước mệnh đề của Mệnh đề 3. Rõ ràng là mọi đỉnh của $\Gamma$ được nối với nhiều nhất hai đỉnh. Nếu $i < j$ thì đường đi $(x_i, \ldots, x_j)$ rút ra từ đường đi $(x_0, \ldots, x_m)$ nối $x_i$ với $x_j$; do đó $\Gamma$ là liên thông. Sau cùng, giả sử $(x_{p_1}, \ldots, x_{p_n})$ là một chu trình trong $\Gamma$, và gọi $p_k$ là số nhỏ nhất trong các số nguyên phân biệt $p_1, \ldots, p_n$. Tồn tại các chỉ số phân biệt $i$ và $j$ sao cho $x_{p_k}$ được nối với $x_{p_i}$ và $x_{p_j}$: điều này suy ra từ định nghĩa của một chu trình. Vì $p_k < p_i$ và $p_k < p_j$, tất yếu có $p_i = p_j = p_k + 1$, điều này là mâu thuẫn vì $p_1, \ldots, p_n$ là phân biệt. Vậy không có chu trình nào trong $\Gamma$.

Ngược lại, cho $\Gamma$ là một cây không có điểm phân nhánh và có số đỉnh hữu hạn khác không, và gọi $(x_0, \ldots, x_m)$ là một đường đi đơn ánh có độ dài cực đại trong $\Gamma$. Ký hiệu $T$ là tập hợp các đỉnh khác $x_0, \ldots, x_m$. Một đỉnh $b \in T$ không thể nối với một đỉnh nào $x_i$, vì khi đó ta sẽ có hoặc

a) $i = 0$, nhưng khi đó $(b, x_0, \ldots, x_m)$ sẽ là một đường đi đơn ánh có độ dài $m + 1$ trong $\Gamma$, hoặc
b) $i = m$, nhưng khi đó $(x_0, \ldots, x_m, b)$ sẽ là một đường đi đơn ánh có độ dài $m + 1$ trong $\Gamma$, hoặc
c) $0 < i < m$, nhưng khi đó $x_i$ sẽ được nối với ba đỉnh phân biệt $x_{i-1}$, $x_{i+1}$ và $b$.

Vì $\Gamma$ liên thông, $T$ rỗng theo Hệ quả 1 của Mệnh đề 1. Hơn nữa, nếu tồn tại $i, j$ sao cho $j - i > 1$ và $x_i, x_j$ được nối với nhau, thì sẽ có một chu trình $(x_i, x_{i+1}, \ldots, x_j)$ trong $\Gamma$. Do đó, $\Gamma$ là một xích. Đpcm.
