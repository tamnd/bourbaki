---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 14
section_title: Transcendental extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.106-A V.118, A V.171-A V.175
pdf_pages: 0220-0232, 0285-0289
extraction: ocr
subsections:
    - "no": 1
      title: Algebraically free families. Pure extensions
      page: 106
      pdf_page: 220
    - "no": 2
      title: Transcendence bases
      page: 107
      pdf_page: 221
    - "no": 3
      title: The transcendence degree of an extension
      page: 110
      pdf_page: 224
    - "no": 4
      title: Extension of isomorphisms
      page: 111
      pdf_page: 225
    - "no": 5
      title: Algebraically disjoint extensions
      page: 112
      pdf_page: 226
    - "no": 6
      title: Algebraically free families of extensions
      page: 115
      pdf_page: 229
    - "no": 7
      title: Finitely generated extensions
      page: 117
      pdf_page: 231
statements: 51
exercises: 20
content_sha256: 23ff307b952da78cbece2bd1ffac7b19c9d0c9a93bac2afc3f1a4f9965d45ca1
translated_from: content/en/alg/V/14_s14_transcendental_extensions.md
source_content_sha256: 96acc445fe1ac21789277cae9b626dfd3b7587df6b094c92c7477d5a1cf37432
translation_model: gpt-5.4-mini
translation_run: translate-vi-22b61d8f
glossary_version: 34
glossary_terms_sha256: 2a89215a3b0ea0d688420ef4c564c2ce2bee84d6f525c863faf7f8a733de8a6f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 14. MỞ RỘNG SIÊU VIỆT

### 1. Các họ độc lập đại số. Mở rộng thuần

Nhắc lại (IV, p. 4) định nghĩa sau:

#### Định nghĩa 1 {#alg-v-s14-def-1 .statement}

*Cho E là một mở rộng của một trường K; một họ $\mathbf{x} = (x_i)_{i \in I}$ các phần tử của E được gọi là độc lập đại số trên K nếu các đơn thức $\mathbf{x}^a = \prod_{i \in I} x_i^{a_i}$ theo các $x_i$ (với $a = (\alpha_i)_{i \in I}$, trong $\mathbf{N}^{(1)}$) độc lập tuyến tính trên K. Trong trường hợp ngược lại, họ đó được gọi là liên hệ đại số trên K.*

Định nghĩa 1 cũng có thể được phát biểu như sau:

#### Mệnh đề 1 {#alg-v-s14-prop-1 .statement}

*Để một họ $(x_i)_{i \in I}$ các phần tử của một mở rộng E của một trường K là độc lập đại số trên K thì điều kiện cần và đủ là quan hệ $f((x_i)) = 0$, trong đó $f$ là một đa thức trong $K[X_i]_{i \in I}$, suy ra $f = 0$.*

#### Định nghĩa 2 {#alg-v-s14-def-2 .statement}

*Cho E là một mở rộng của một trường K. Một họ $(x_i)_{i \in I}$ các phần tử của E được gọi là một cơ sở thuần của E (trên K) nếu nó độc lập đại số và $E = K(x_i)_{i \in I}$. Mở rộng E của K cũng được gọi là thuần nếu nó có một cơ sở thuần.*

Họ rỗng là độc lập đại số, do đó K là một mở rộng thuần của chính nó. Với ký hiệu của ĐN. 2, mỗi phần tử $x_i$ đều siêu việt trên K; nếu $I$ không rỗng, thì E do đó là một mở rộng siêu việt của K.

#### Mệnh đề 2 {#alg-v-s14-prop-2 .statement}

*Cho E và $E'$ là hai trường và u là một đẳng cấu của một trường con K của E lên một trường con $K'$ của $E'$. Cho $\mathbf{x} = (x_i)_{i \in I}$ (tương ứng $\mathbf{x}' = (x'_i)_{i \in I}$) là một họ các phần tử của E (tương ứng $E'$) độc lập đại số trên K (tương ứng $K'$). Khi đó tồn tại duy nhất một đẳng cấu $v$ của $L = K(x_i)_{i \in I}$ lên $L' = K'(x'_i)_{i \in I}$, đẳng cấu này cảm sinh u trên K và gửi $x_i$ tới $x'_i$ với mỗi $i \in I$.*

Tính duy nhất của $v$ là hiển nhiên. Đặt $A = K[x_i]_{i \in I}$ và $A' = K'[x'_i]_{i \in I}$. Theo giả thiết, các đơn thức $x'' = \prod_{i \in I} x_i^{\alpha_i}$ (với $\alpha = (\alpha_i)_{i \in I}$, trong $\mathbf{N}^{(I)}$) lập thành một cơ sở của không gian vectơ trên K $A$ và $A'$ cũng có tính chất tương tự. Do đó tồn tại một đẳng cấu vành $w : A \to A'$ gửi mỗi phần tử $\sum_{\alpha \in \mathbf{N}^{(I)}} c_\alpha x^\alpha$ tới $\sum_{\alpha \in \mathbf{N}^{(I)}} u(c_\alpha) {x'}^\alpha$. Vì $L$ là trường phân thức của $A$ và $L'$ là trường phân thức của $A'$, nên đẳng cấu $w$ mở rộng thành một đẳng cấu $v$ của trường $L$ lên trường $L'$.

#### Hệ quả {#alg-v-s14-n1-cor-1 .statement}

— *Để một mở rộng E của một trường K là thuần thì điều kiện cần và đủ là E K-đẳng cấu với một trường phân thức hữu tỉ trên K. Chính xác hơn, nếu họ $(x_i)_{i \in I}$ là một cơ sở thuần của E, thì tồn tại duy nhất một K-đẳng cấu của $K(X_i)_{i \in I}$ lên E, đẳng cấu này gửi $X_i$ tới $x_i$ với mỗi $i \in I$.*

#### Nhận xét {#alg-v-s14-n1-rem-1 .statement}

Rõ ràng rằng trong một mở rộng E của K, một họ độc lập đại số trên K gồm các phần tử *độc lập tuyến tính* trên $K$ (do đó phân biệt từng đôi một); nói cách khác, nó cũng là một họ độc lập tuyến tính đối với cấu trúc *không gian vectơ* của E (theo K). Nhưng chiều đảo lại là sai, vì nếu E là một mở rộng đại số của K, thì bất kỳ họ không rỗng nào gồm các phần tử của E (và *a fortiori* một họ không rỗng gồm các phần tử độc lập tuyến tính trên K) đều không bao giờ độc lập đại số trên K. Khi có nguy cơ nhầm lẫn, ta sẽ nói rằng một tập con của một mở rộng E của K, tự do đối với cấu trúc không gian vectơ của E theo K, là *tự do tuyến tính* trên K.

Cho E là một mở rộng của một trường K. Một tập con S của E được gọi là *độc lập đại số* (trên $K$) nếu họ do ánh xạ đồng nhất của S lên chính nó xác định là độc lập đại số. Các phần tử của một tập con độc lập đại số của E còn được gọi là *độc lập đại số*. Nếu một tập con của E không độc lập đại số, ta nói rằng nó *liên hệ đại số* và các phần tử của nó là *phụ thuộc đại số*. Để một họ $(x_i)_{i \in I}$ các phần tử của E độc lập đại số thì điều kiện cần và đủ là $i \mapsto x_i$ là một song ánh từ I lên một tập con độc lập đại số của E.

Mọi tập con của một tập độc lập đại số đều độc lập đại số. Hơn nữa:

#### Mệnh đề 3 {#alg-v-s14-prop-3 .statement}

— *Để một họ $(x_i)_{i \in I}$ các phần tử của một mở rộng E của một trường K là độc lập đại số trên K thì điều kiện cần và đủ là mọi họ con hữu hạn của $(x_i)_{i \in I}$ đều độc lập đại số trên K.*

Mệnh đề này suy ra ngay từ Định nghĩa 1.

### 2. Cơ sở siêu việt

#### Mệnh đề 4 {#alg-v-s14-prop-4 .statement}

— *Cho E là một mở rộng của trường K và S, T là hai tập con của E. Khi đó các tính chất sau là tương đương:
a) $S \cup T$ là độc lập đại số trên K và $S \cap T = \varnothing$.*

Hiển nhiên chỉ cần chứng minh rằng a) và b) là tương đương.

$a) \Rightarrow b)$: Giả sử rằng a) đúng. Vì $S$ được chứa trong $S \cup T$, nên $S$ độc lập đại số trên $K$. Nếu $T$ không độc lập đại số trên $K(S)$, thì tồn tại (Mệnh đề 3) một họ hữu hạn $(y_j)_{1 \leq j \leq n}$ gồm các phần tử phân biệt của $T$ phụ thuộc đại số trên $K(S)$. Do đó tồn tại một đa thức khác không $f$ trong vành $K(S)[Y_1, ..., Y_n]$ sao cho $f(y,, ..., y,) = 0$; sau khi nhân $f$ nếu cần với một phần tử khác không của $K[S]$ ta có thể giả sử rằng mọi hệ số của f đều thuộc $K[S]$. Các hệ số của f là các đa thức trong một số hữu hạn các phần tử phân biệt $x_i \ (1 \leq i \leq m )$ của $S$, với hệ số trong $K$. Các phần tử $x_1, ..., x,, y_1, ..., y,$ từng đôi một phân biệt vì $S \cap T = (21$. Quan hệ $f(y,, ..., y,) = 0$ vì thế có thể viết thành

$$
g(x_1, ..., x_m ; y_1, ..., y_n) = 0 ,
$$

trong đó $g$ là một đa thức khác không của $K[X_1, ..., X_m, Y_1, ..., Y_n]$, và một quan hệ như vậy mâu thuẫn với giả thiết rằng $S \cup T$ là độc lập đại số.

$b) \Rightarrow a)$: Giả sử b) đúng. Trước hết, hiển nhiên là $T \cap K(S) = \varnothing$ và $a fortiori \ S \cap T = (21$. Chỉ cần chứng minh rằng nếu $x_i \ (1 \leq i \leq m )$ là các phần tử phân biệt của $S$, hữu hạn về số lượng, và $y_j \ (1 \leq j \leq n )$ là các phần tử phân biệt của $T$, hữu hạn về số lượng, thì tập hợp các $x_i$ và $y,$ là độc lập đại số trên $K$ (Mệnh đề 3). Xét một đa thức $f \in K[X_1, ..., X,, Y_1, ..., Y_n]$ sao cho $f(x_1, ..., x_m, y_1, ..., y,) = 0$ và đặt $f = \sum \varphi_\alpha Y_1^{\alpha_1} ... Y_n^{\alpha_n}$ với $\varphi_\alpha \in K[X_1, ..., X_m]$ cho mọi $\alpha = (\alpha,, ..., \alpha_n) \in \mathbf{N}^n$. Đặt $g = f(x,, ..., x,, Y_1, ..., Y,)$; khi đó $g$ là một đa thức trong vành $K[S][Y_1, ..., Y,]$ và đẳng thức $f(x_1, ..., x_m, y_1, ..., y,) = 0$ có thể viết thành $g(y_1, ..., y,) = 0$. Vì $T$ độc lập đại số trên $K(S)$, mỗi hệ số $\varphi_\alpha(x_1, ..., x,)$ của $g$ đều bằng không; vì $S$ độc lập đại số trên $K$, ta có $\varphi_\alpha = 0$ với mọi $\alpha \in \mathbf{N}^n$, và do đó $f = 0$.

#### Hệ quả {#alg-v-s14-n2-cor-1 .statement}

— *Cho E là một mở rộng của một trường K và S là một tập con của E độc lập đại số trên K. Nếu $x \in E$ là siêu việt trên $K(S)$, thì S U {x} độc lập đại số trên K.*

#### Mệnh đề 5 {#alg-v-s14-prop-5 .statement}

— *Cho E là một mở rộng của trường K. Để một tập con S của E độc lập đại số trên K thì cần và đủ rằng với mỗi $x \in S$, phần tử x phải siêu việt trên trường $K(S - {x})$.*

Điều kiện đó là cần thiết theo Mệnh đề 4.

Để chứng minh điều kiện đủ, chỉ cần (Mệnh đề 3) chứng minh rằng mọi dãy hữu hạn $(x_1, ..., x,)$ gồm các phần tử phân biệt của $S$ đều độc lập đại số. Nay theo giả thiết, $x_i$ siêu việt trên $K(x_1, ..., x_{i-1})$ với $1 \leq i \leq n$, và khi đó mệnh đề của ta suy ra bằng quy nạp theo $n$ từ Hệ quả của Mệnh đề 4.

#### Mệnh đề 6 {#alg-v-s14-prop-6 .statement}

— *Cho E là một mở rộng của một trường K và X là một tập con độc lập đại số của E trên K. Nếu $K' \subset E$ là một mở rộng đại số của K thì X độc lập đại số trên K'.*

Lập luận bằng phản chứng, giả sử X phụ thuộc đại số trên K'. Theo Mệnh đề 5 tồn tại một phần tử $x \in X$ đại số trên trường $K'(M)$, với $M = X - \{x\}$. Vì $K'(M) = K(M)(K')$ và $K'$ là đại số trên K, Hệ quả 2 của V, p. 18 cho thấy rằng $K'(M)$ là đại số trên $K(M)$; vì $x$ đại số trên $K'(M)$, nên do đó nó đại số trên $K(M) = K(X - \{x\})$, theo Mệnh đề 3 của V, p. 19. Nay Mệnh đề 5 cho thấy X phụ thuộc đại số trên K và ta có mâu thuẫn.

#### Định nghĩa 3 {#alg-v-s14-def-3 .statement}

*Một tập con B của một mở rộng E của một trường K là một cơ sở siêu việt của E (trên K) nếu B độc lập đại số trên K và E là đại số trên K(B).*

#### Ví dụ {#alg-v-s14-n2-exa-1 .statement}

— *Một cơ sở thuần là một cơ sở siêu việt. Mặt khác, nếu E là một mở rộng thuần của K, thì một cơ sở siêu việt của E trên K không phải lúc nào cũng là một cơ sở thuần của E. Chẳng hạn, trong $K(X)$, $\{X^2\}$ là một cơ sở siêu việt nhưng không sinh $K(X)$. \*

#### Mệnh đề 7 {#alg-v-s14-prop-7 .statement}

*Mỗi cơ sở siêu việt của E là một phần tử cực đại của tập hợp (được sắp theo quan hệ bao hàm) các tập con của E độc lập đại số trên K. Ngược lại, nếu S là một tập con của E sao cho E là đại số trên $K(S)$, thì mọi tập con độc lập đại số cực đại của S là một cơ sở siêu việt của E.*

Cho B là một cơ sở siêu việt của E trên K và $x \in E - B$. Khi đó $x$ là đại số trên $K(B)$; theo V, p. 107, Mệnh đề 4, tập con $B \cup \{x\}$ của E không tự do đại số trên K, do đó có phần thứ nhất của mệnh đề. Thứ hai, nếu E là đại số trên $K(S)$ và B là một phần tự do đại số cực đại của S, thì từ Hệ quả của Mệnh đề 4 suy ra mọi $x \in S$ đều đại số trên $K(B)$; do đó (V, p. 18, Hệ quả 1) $K(S)$ là đại số trên $K(B)$, và vì vậy (V, p. 19, Mệnh đề 3), E là đại số trên $K(B)$.

#### Định lý 1 (Steinitz) {#alg-v-s14-thm-1 .statement}

— *Mọi mở rộng E của một trường K đều thừa nhận một cơ sở siêu việt trên K. Nói cách khác, mọi mở rộng của một trường K đều là một mở rộng đại số của một mở rộng thuần của K.*

Ngược lại, một mở rộng không phải lúc nào cũng là một mở rộng thuần của một mở rộng đại số (V, p. 171, Bài tập 2).

Định lý này là hệ quả của kết quả chính xác hơn sau đây:

#### Định lý 2 {#alg-v-s14-thm-2 .statement}

*Cho E là một mở rộng của một trường K, S là một tập con của E sao cho E là đại số trên $K(S)$ và T là một tập con của S tự do đại số trên K; khi đó tồn tại một cơ sở siêu việt B của E trên K sao cho $T \subset B \subset S$.*

Thật vậy, tập các tập con tự do đại số của S, được sắp thứ tự bởi quan hệ bao hàm, là một tập có đặc trưng hữu hạn (E, III, p. 34) theo Mệnh đề 3. Theo Định lý 1 của E, III, p. 35, nó có một phần tử cực đại B chứa T, và B là một cơ sở siêu việt của E trên K, theo Mệnh đề 7.

#### Hệ quả (« Định lý trao đổi ») {#alg-v-s14-n2-cor-2 .statement}

— Cho E là một mở rộng của K, S là một tập con của E sao cho E là đại số trên K(S), T là một tập con của E tự do đại số trên K; khi đó tồn tại một tập con S' của S sao cho T \cup S' là một cơ sở siêu việt của E trên K và $T \cap S' = \varnothing$.

Vì E là đại số trên K(T U S) và ta có $T \subset T U S$.

### 3. Bậc siêu việt của một mở rộng

#### Định lý 3 {#alg-v-s14-thm-3 .statement}

— Cho E là một mở rộng của một trường K. Mọi cơ sở siêu việt của E trên K đều có cùng lực lượng.

Chỉ cần chứng minh bất đẳng thức Card(B) ≥ Card(B'), khi B và B' là hai cơ sở siêu việt của E trên K, và ta có thể giả sử rằng B' không rỗng. Trước hết, giả sử B là hữu hạn và dùng quy nạp theo lực lượng n của nó; với n = 0, E là đại số trên K và B' rỗng. Giả sử bây giờ n ≥ 1; cho x ∈ B', định lý trao đổi cung cấp một tập con C của B sao cho x ∉ C và {x} U C là một cơ sở siêu việt của E trên K; ta có C ≠ B theo Mệnh đề 7, do đó Card C < n. Đặt K_1 = K(x) và C' = B' - {x}; khi đó C và C' tự do đại số trên trường K_1 (V, p. 107, Mệnh đề 4) và E là đại số cả trên K_1(C) = K(C U {x})) và K_1(C') = K(B'). Nói cách khác, C và C' là hai cơ sở siêu việt của E trên K_1. Vì Card(C) < n, giả thiết quy nạp suy ra bất đẳng thức Card(C') ≤ Card(C) ≤ n - 1, do đó Card(B') ≤ n = Card(B).

Giả sử bây giờ B là vô hạn. Mọi x ∈ B đều đại số trên K(B') và do đó tồn tại một tập con hữu hạn S(x) của B' sao cho x đại số trên K(S(x)). Đặt S = U_{x ∈ B} S(x), khi đó S ⊂ B' và vì B là vô hạn, ta có Card(S) ≤ Card(B) (E, III, p. 49, Hệ quả 3). Nhưng vì mọi phần tử của B đều đại số trên K(S) và E là đại số trên K(B), suy ra E là đại số trên K(S) (V, p. 19, Mệnh đề 3). Bây giờ Mệnh đề 7 suy ra rằng S = B', do đó bất đẳng thức cần chứng minh Card(B') ≤ Card(B).

#### Định nghĩa 4 {#alg-v-s14-def-4 .statement}

— Cho E là một mở rộng của một trường K. Lực lượng của mọi cơ sở siêu việt của E trên K được gọi là bậc siêu việt của E trên K và được ký hiệu tr. deg_K E.

Định lý 2 và 3 cùng Định nghĩa 4 suy ra các hệ quả sau đây, trong đó E ký hiệu một mở rộng của một trường K, có bậc siêu việt hữu hạn n.

#### Hệ quả 1 {#alg-v-s14-def-4-cor-1 .statement}

— Cho S là một tập con của E sao cho E là đại số trên K(S). Khi đó Card(S) ≥ n; nếu lực lượng của S bằng n, thì S tự do đại số trên K (do đó khi ấy nó là một cơ sở siêu việt của E trên K).

#### Hệ quả 2 {#alg-v-s14-def-4-cor-2 .statement}

— Giả sử E = K(x_1, ..., x_m), thì m ≥ n; nếu hơn nữa m = n, thì (x_1, ..., x_m) là một cơ sở thuần của E trên K, và khi đó E là một mở rộng thuần của K.

#### Hệ quả 3 {#alg-v-s14-def-4-cor-3 .statement}

— Mọi tập con của $E$ tự do đại số trên $K$ có nhiều nhất $n$ phần tử, và nếu nó có đúng $n$ phần tử, thì nó là một cơ sở siêu việt của $E$ trên $K$.

#### Định lý 4 {#alg-v-s14-thm-4 .statement}

— Cho $K, E$ và $F$ là ba trường sao cho $K \subset E \subset F$. Nếu $S$ là một cơ sở siêu việt của $E$ trên $K$ và $T$ là một cơ sở siêu việt của $F$ trên $E$, thì $S \cap T$ rỗng và $S \cup T$ là một cơ sở siêu việt của $F$ trên $K$.

Vì $F$ là đại số trên $E(T)$; hơn nữa, $E(T)$ là đại số trên trường $K(S \cup T) = K(S)(T)$, vì $E$ là đại số trên $K(S)$ ($V$, p. 18, Hệ quả 2); do đó ($V$, p. 19, Mệnh đề 3) $F$ là đại số trên $K(S \cup T)$. Mặt khác, vì $T$ tự do đại số trên $E$ nên a fortiori cũng vậy trên $K(S)$, do đó ($V$, p. 107, Mệnh đề 4) $S \cup T$ tự do đại số trên $K$ và $S \cap T = \varnothing$.

#### Hệ quả {#alg-v-s14-n3-cor-1 .statement}

— Cho $K, E$ và $F$ là ba trường sao cho $K \subset E \subset F$. Khi đó ta có
$$
\text{tr. deg}_K F = \text{tr. deg}_K E + \text{tr. deg}_E F
$$

### 4. Mở rộng các đẳng cấu

#### Mệnh đề 8 {#alg-v-s14-prop-8 .statement}

— Cho $\Omega$ là một mở rộng đóng đại số của một trường $K$, $E$ và $F$ là hai mở rộng con của $\Omega$ và $u$ là một $K$-đẳng cấu của $E$ lên $F$. Để tồn tại một $K$-tự đẳng cấu $v$ của $O$ mở rộng $u$, thì cần và đủ rằng $\Omega$ có cùng bậc siêu việt trên $E$ và $F$.

Điều kiện đó hiển nhiên là cần.

Giả sử $\Omega$ có cùng bậc siêu việt trên $E$ và $F$ và hãy chọn một cơ sở siêu việt $B$ của $\Omega$ trên $E$ và một cơ sở siêu việt $C$ của $\Omega$ trên $F$. Vì $B$ và $C$ có cùng lực lượng, Mệnh đề 2 ($V$, p. 106) cho thấy $u$ kéo dài thành một $K$-đẳng cấu $u'$ của $E(B)$ lên $F(C)$. Vì $C?$ là một bao đóng đại số của $E(B)$ và $F(C)$, hệ quả của $V$, p. 23 cho thấy $u'$ kéo dài thành một tự đẳng cấu $v$ của $\Omega$.

#### Hệ quả 1 {#alg-v-s14-prop-8-cor-1 .statement}

— Cho $O$ là một mở rộng đóng đại số của một trường $K$ và $E$ là một mở rộng con của $\Omega$. Mọi $K$-tự đẳng cấu của $E$ đều kéo dài thành một $K$-tự đẳng cấu của $\Omega$.

#### Hệ quả 2 {#alg-v-s14-prop-8-cor-2 .statement}

Ký hiệu $n, d(E)$ và $d(F)$ lần lượt là các bậc siêu việt của $E$ trên $K$, của $O$ trên $E$ và của $C?$ trên $F$. Sự tồn tại của $K$-đẳng cấu $u$ cho thấy bậc siêu việt của $F$ trên $K$ bằng $n$. Theo Hệ quả của Định lý 4 bậc siêu việt của $\Omega$ trên $K$ bằng $d(E) + n$ và cũng bằng $d(F) + n$. Do đó (E, III, p. 28, Mệnh đề 8) ta có $d(E) = d(F)$ và ta có thể áp dụng Mệnh đề 8.

#### Mệnh đề 9 {#alg-v-s14-prop-9 .statement}

— Cho $K$ là một trường và $\Omega$ là một mở rộng đóng đại số của $K$. Giả sử $\Omega$ không đại số trên $K$; khi đó tập hợp các phần tử của $\Omega$ siêu việt trên $K$ là vô hạn. Hơn nữa, nếu $x$ và $y$ là hai phần tử của $\Omega$ siêu việt trên $K$, thì tồn tại một tự đẳng cấu $u$ của $\Omega$ trên $K$ sao cho $u(x) = y$.

Vì $\Omega$ không đại số trên $K$, tồn tại một phần tử $x$ của $\Omega$ siêu việt trên $K$; khi đó các phần tử $x^n$ ($n \in \mathbf{N}$) phân biệt và siêu việt trên $K$. Giả sử rằng $x$ và $y$ phân biệt và siêu việt trên $K$; theo Mệnh đề 2 (V, p. 106) tồn tại một $K$-đẳng cấu $\tilde{u}$ của $K(x)$ lên $K(y)$ sao cho $\tilde{u}(x) = y$; vì $K(x)$ có bậc siêu việt 1 trên $K$, Hệ quả 2 của Mệnh đề 8 cho thấy rằng $\tilde{u}$ mở rộng thành một $K$-tự đẳng cấu $u$ của $\Omega$.

#### Mệnh đề 10 {#alg-v-s14-prop-10 .statement}

— Cho $K$ là một trường, $\Omega$ là một mở rộng đóng đại số của $K$ và $G$ là nhóm các $K$-tự đẳng cấu của $\Omega$. Cho $x \in \Omega$.

a) Để $x$ đại số trên $K$ thì cần và đủ rằng tập hợp các phần tử $u(x)$ khi $u$ chạy qua $G$ là hữu hạn,

b) Để $x$ là p-căn trên $K$ thì cần và đủ rằng $u(x) = x$ với mọi $u \in G$.

Đặc biệt nếu $K$ là hoàn hảo, thì tập hợp các bất biến của nhóm $G$ bằng $K$.

Giả sử trước hết rằng $x$ là siêu việt. Theo Mệnh đề 9, tập hợp $T$ các phần tử của $\Omega$ siêu việt trên $K$ là vô hạn, và với mỗi $y \in T$ đều tồn tại $u \in G$ sao cho $u(x) = y$. Do đó tập hợp các phần tử $u(x)$ khi $u$ chạy trên $G$ là vô hạn.

Giả sử bây giờ rằng $x$ là đại số trên $K$ và ký hiệu đa thức tối tiểu của nó trên $K$ là $f$; tập hợp các nghiệm của $f$ trong $\Omega$ là hữu hạn và với mỗi $u \in G$ ta có $f(u(x)) = u(f(x)) = 0$. Do đó tập hợp các phần tử $u(x)$ khi $u$ chạy trên $G$ là hữu hạn. Điều đó chứng minh a).

Cho $L$ là tập hợp các phần tử $y$ của $\Omega$ sao cho $u(y) = y$ với mọi $u \in G$, và cho $\bar{K}$ là bao đóng đại số tương đối của $K$ trong $\Omega$. Theo những điều đã nói, $L$ là một mở rộng trung gian của $\bar{K}$ trên $K$. Hơn nữa (Hệ quả 1 của Mệnh đề 8) mọi tự đẳng cấu của $\bar{K}$ trên $K$ đều là hạn chế lên $\bar{K}$ của một phần tử của $G$. Mệnh đề b) của Mệnh đề 10 suy ra ngay từ Hệ quả 3 của V, p. 53.

### 5. Các mở rộng rời nhau đại số

#### Định nghĩa 5 {#alg-v-s14-def-5 .statement}

— Cho $L$ là một mở rộng của một trường $K$, và $E$ và $F$ là hai mở rộng trung gian của $L$. Khi đó $E$ và $F$ được gọi là rời nhau đại số (trên $K$), và $E$ được gọi là rời nhau đại số với $F$ trên $K$, nếu với mọi tập con $A$ (tương ứng $B$) của $E$ (tương ứng $F$) tự do đại số trên $K$, thì $A$ và $B$ rời nhau và $A \cup B$ là tự do đại số trên $K$.

#### Nhận xét 1 {#alg-v-s14-n5-rem-1 .statement}

Nếu $E$ là một mở rộng trung gian của $L$ đại số trên $K$, thì nó rời nhau đại số với mọi mở rộng trung gian $F$ của $L$. Để một mở rộng của $K$ là đại số thì điều kiện cần và đủ là nó rời nhau đại số với chính nó.

#### Nhận xét 2 {#alg-v-s14-n5-rem-2 .statement}

Có thể xảy ra rằng $E$ rời nhau đại số với $F$ trên $K$, nhưng không rời nhau đại số trên một trường con $K_{\|}$ của $K$. \* Chẳng hạn $C$ rời nhau đại số với chính nó trên $R$ nhưng không trên $\mathbf{Q}$. \*

#### Nhận xét 3 {#alg-v-s14-n5-rem-3 .statement}

Rõ ràng là nếu $E$ rời nhau đại số với $F$ trên $K$, khi $E$ và $F$ được xem như các mở rộng trung gian của $L$, thì điều đó cũng đúng khi chúng được xem như các mở rộng trung gian của $K(E \cup F)$ và ngược lại.

#### Mệnh đề 11 {#alg-v-s14-prop-11 .statement}

— *Nếu $E$ và $F$ rời nhau đại số trên $K$ thì* $E \cap F$ *là đại số trên $K$*.

Điều này suy ra từ Định nghĩa 5.

#### Mệnh đề 12 {#alg-v-s14-prop-12 .statement}

— *Cho $L$ là một mở rộng của một trường $K$ và $E, F$ là các mở rộng trung gian của $L$. Khi đó các điều kiện sau là tương đương*:

a) *$E$ và $F$ rời nhau đại số*;

b) *tồn tại một cơ sở siêu việt của $E$ trên $K$ tự do đại số trên $F$*;

c) *mọi tập con của $E$ tự do đại số trên $K$ đều tự do đại số trên $F$*.

Ta đưa ra các điều kiện sau:

$b'$') *tồn tại một cơ sở siêu việt của $F$ trên $K$ tự do đại số trên $E$*;

$c'$') *mọi tập con của $F$ tự do đại số trên $K$ đều tự do đại số trên $E$*.

$a) \Rightarrow b'$') : Giả sử $E$ và $F$ rời nhau đại số. Cho $B$ (tương ứng $C$) là một cơ sở siêu việt của $E$ (tương ứng $F$) trên $K$. Khi đó $B \cap C = \varnothing$ và $B \cup C$ là tự do đại số trên $K$, suy ra $C$ là tự do đại số trên $K(B)$ (V, p. 107, Mệnh đề 4); vì $E$ là đại số trên $K(B)$, Mệnh đề 6 của V, p. 108 cho thấy $C$ là tự do đại số trên $E$.

$b'$') $\Rightarrow$ c) : Giả sử tồn tại một cơ sở siêu việt $C$ của $F$ trên $K$ tự do đại số trên $E$. Cho $A$ là một tập con của $E$ tự do đại số trên $K$. Khi đó $C$ là tự do đại số trên $K(A)$, suy ra $A$ là tự do đại số trên $K(C)$ (V, p. 107, Mệnh đề 4) và do đó trên $F$ (V, p. 108, Mệnh đề 6), vì $F$ là đại số trên $K(C)$.

c) $\Rightarrow$ a) : Điều này suy ra ngay từ Mệnh đề 4 (V, p. 107).

Các kéo theo $a) \Rightarrow b) \Rightarrow c' ) \Rightarrow a)$ có thể được chứng minh theo cùng một cách.

#### Hệ quả {#alg-v-s14-n5-cor-1 .statement}

— *Cho $E$ và $F$ rời nhau đại số trên $K$. Cho $E'$ là bao đóng đại số tương đối của $E$ trong $L$ và $F'$ là bao đóng ấy của $F$* (V, p. 19). *Khi đó $E'$ *và $F'$* rời nhau đại số trên $K$*.

Cho $B$ là một cơ sở siêu việt của $E$ trên $K$; đó cũng là một cơ sở siêu việt của $E'$ trên $K$. Vì $E$ rời nhau đại số với $F$ trên $K$, nên $B$ tự do đại số trên $F$, suy ra trên $F'$ (V, p. 108, Mệnh đề 6); bây giờ ta có thể áp dụng Mệnh đề 12.

#### Mệnh đề 13 {#alg-v-s14-prop-13 .statement}

— *Cho $L$ là một mở rộng của một trường $K$ và $E, F$ là hai mở rộng trung gian của $L$*.

a) *Ta có* $\operatorname{tr. deg}_L F(E) \leq \operatorname{tr. deg}_K E$. *Khi $E$ và $F$ rời nhau đại số trên $K$, thì mọi cơ sở siêu việt của $E$ trên $K$ đều là một cơ sở siêu việt của*

$F(E)$ trên $F$ và ta có tr . deg_F F(E) = tr . deg_K E. Ngược lại, đẳng thức này suy ra rằng $E$ và $F$ rời nhau đại số trên $K$ khi tr . deg_K E là hữu hạn.

b) Ta có tr . deg_K K(E U F) ≤ tr . deg_K E + tr . deg_K F. Khi $E$ và $F$ rời nhau đại số trên $K$, ta có tr . deg_K K(E U F) = tr . deg_K E + tr . deg_K F. Ngược lại, đẳng thức này suy ra rằng $E$ và $F$ rời nhau đại số trên $K$ khi $E$ và $F$ có bậc siêu việt hữu hạn trên $K$.

a) Cho $B$ là một cơ sở siêu việt của $E$ trên $K$; khi đó $E$ là đại số trên $K(B)$, và Hệ quả 2 của V, p. 18 cho thấy $F(E)$ là đại số trên $F(K(B)) = F(B)$. Theo Đl. 2 (V, p. 109) $B$ chứa một cơ sở siêu việt của $F(E)$ trên $F$; khi $E$ rời nhau đại số với $F$ trên $K$, thì $B$ tự do đại số trên $F$ (Mệnh đề 12) và khi đó $B$ là một cơ sở siêu việt của $F(E)$ trên $F$. Ba mệnh đề đầu của a) suy ra từ đó. Giả sử bây giờ rằng $E$ có bậc siêu việt hữu hạn trên $K$, bằng với bậc của $F(E)$ trên $F$; vì $F(E)$ là đại số trên $F(B)$ và Card $B = \text{tr . deg}_F F(E)$, Hệ quả 1 của V, p. 110 cho thấy $B$ tự do đại số trên $F$, nên $E$ rời nhau đại số với $F$ trên $K$ (Mệnh đề 12).

b) Ta có $K(E U F) = F(E)$ và do đó Hệ quả của V, p. 110 suy ra đẳng thức:

$$
\text{tr . deg}_K K(E \cup F) = \text{tr . deg}_F F(E) + \text{tr . deg}_K F .
$$

B) suy ra ngay từ a) và đẳng thức này.

#### Mệnh đề 14 {#alg-v-s14-prop-14 .statement}

— *Cho L là một mở rộng của một trường K, E và F là hai mở rộng con của L và B là một cơ sở siêu việt của E trên K. Để E và F rời nhau đại số trên K thì cần và đủ rằng K(B) và F phải rời tuyến tính trên K.*

Để E và F rời nhau đại số trên K thì cần và đủ để B tự do đại số trên F (Mệnh đề 12), tức là, các đơn thức trong các phần tử của B phải độc lập tuyến tính trên F. Vì các đơn thức này tạo thành một cơ sở của không gian K-vectơ K[B], nói rằng K[B] và F rời tuyến tính trên K cũng là nói rằng như thế. Cuối cùng, vì K(B) là trường các phân thức của K[B], Mệnh đề 6 của V, p. 14 cho thấy K[B] và F rời tuyến tính khi và chỉ khi điều đó đúng cho K(B) và F.

#### Hệ quả 1 {#alg-v-s14-prop-14-cor-1 .statement}

— *Nếu E và F rời tuyến tính, thì E rời nhau đại số với F trên K. Ngược lại, nếu E là một mở rộng thuần của K và rời nhau đại số với F trên K, thì E và F rời tuyến tính trên K.*

#### Hệ quả 2 {#alg-v-s14-prop-14-cor-2 .statement}

— *Mọi mở rộng thuần của K đều rời tuyến tính với mọi mở rộng đại số của K; đặc biệt, K là đóng đại số tương đối trong mọi mở rộng thuần của K.*

### 6. Các họ mở rộng tự do đại số

#### Định nghĩa 6 {#alg-v-s14-def-6 .statement}

— Cho $L$ là một mở rộng của một trường $K$ và $(E_i)_{i \in I}$ là một họ các mở rộng con của $L$. Họ $(E_i)_{i \in I}$ được gọi là tự do đại số nếu điều kiện sau được thỏa mãn:

(AF) Với mỗi $i \in I$ hãy lấy $A_i$ là một tập con của $E_i$ tự do đại số trên $K$. Khi đó $A_i \cap A_j = \varnothing$ đối với $i \neq j$ và $\bigcup_{i \in I} A_i$ tự do đại số trên $K$.

#### Nhận xét {#alg-v-s14-n6-rem-1 .statement}

Theo Mệnh đề 3 ($V$, p. 107) chỉ cần kiểm tra điều kiện (AF) cho các tập con hữu hạn $A_i$. Vì vậy ta thu được kết quả sau: nếu $(E_i)_{i \in I}$ là một họ tự do đại số, thì điều đó vẫn đúng cho $(E'_i)_{i \in I}$ nếu $E'_i$ là một mở rộng con của $E_i$ với mỗi $i \in I$; ngược lại, nếu mọi họ $(E'_i)_{i \in I}$, trong đó $E'_i$ là một mở rộng con sinh hữu hạn của $E$ với mỗi $i \in I$, đều tự do đại số, thì $(E_i)_{i \in I}$ là tự do đại số. Mặt khác, để $(E_i)_{i \in I}$ là tự do đại số thì cần và đủ rằng $(E_i)_{i \in J}$ phải tự do đại số với mọi tập con hữu hạn $J$ của $I$. Nói một cách trực giác, ta có thể nói rằng tính độc lập đại số của các mở rộng là một tính chất «có đặc trưng hữu hạn».

#### Mệnh đề 15 {#alg-v-s14-prop-15 .statement}

— Cho $(E_i)_{i \in I}$ là một họ các mở rộng con của một mở rộng đã cho $L$ của một trường $K$. Khi đó các điều kiện sau đây là tương đương :

a) Họ $(E_i)_{i \in I}$ là tự do đại số.

b) Với mỗi $i \in I$ mở rộng $E_i$ rời nhau đại số trên $K$ với mở rộng $F_i$ được sinh bởi các $E_j$ với $j \neq i$.

c) Tồn tại một họ $(B_i)_{i \in I}$ gồm các tập con rời nhau của $L$, sao cho $B_i$ là một cơ sở siêu việt của $E_i$ trên $K$ đối với mỗi $i \in I$, và $B = \bigcup_{i \in I} B_i$ là tự do đại số trên $K$.

Rõ ràng là a) kéo theo c).

Giả sử c), ta chọn $i$ trong $I$; đặt $C_i = \bigcup_{j \neq i} B_j$. Với mỗi $j \neq i$, mọi phần tử của $E_j$ đều đại số trên $K(B_j)$ và do đó a fortiori trên $K(C_i)$. Theo Hệ quả 1 của $V$, p. 18, trường $F_i$ vì thế đại số trên $K(C_i)$. Hơn nữa, ta có $B_i \cap C_i = \varnothing$ và $B - B_i \cup C_i$ là tự do đại số trên $K$; do đó $B_i$ là tự do đại số trên $K(C_i)$ ($V$, p. 107, Mệnh đề 4), vì thế cũng tự do đại số trên $F_i$ (là đại số trên $K(C_i)$) theo Mệnh đề 6 của $V$, p. 108. Vậy ta đã chứng minh rằng $E_i$ rời nhau về đại số với $F_i$ trên $K$ ($V$, p. 113, Mệnh đề 12), do đó c) suy ra b).

Bây giờ giả sử b) và chứng minh a). Chỉ cần chứng tỏ rằng nếu $i_1, \ldots, i_n$ là các phần tử phân biệt của $I$, thì họ các mở rộng $(E_{i_1}, \ldots, E_{i_n})$ là tự do đại số; ta chứng minh bằng quy nạp theo $n$, trường hợp $n = 1$ là tầm thường. Giả sử thế thì $n > 1$ và họ $(E_{i_1}, \ldots, E_{i_{n-1}})$ là tự do đại số; với $1 \leq k \leq n$ chọn một tập con $A_k$ của $E_{i_k}$ tự do đại số trên $K$ và đặt

B = A, U ... U A_{n-1}. Theo giả thiết quy nạp, các tập con $A_1, \ldots, A_{n-1}$ đôi một rời nhau và $B$ là tự do đại số trên $K$; theo b) thì $E_{i_n}$ rời nhau về đại số với $F_i$ và vì $B$ được chứa trong $F_{i_n}$ nên ta có $B \cap A_i = \varnothing$ và $B \cup A_i = A, U ... U A_i$ là tự do đại số trên $K$. Vậy ta đã chỉ ra rằng họ $(E_{i_1}, \ldots, E_{i_n})$ là tự do đại số.

Định lý sau khái quát hóa phần b) của Mệnh đề 13 ($V$, p. 113).

#### Mệnh đề 16 {#alg-v-s14-prop-16 .statement}

— *Cho* (E_i)_{i \in I} *là một họ các mở rộng con của một mở rộng của một trường K*, và đặt E là trường sinh bởi $\bigcup_{i \in I} E_i$.

a) *Ta có* tr . deg$_K$ E $\leq \sum_{i \in I} \text{tr . deg}_K E_i$, *với đẳng thức khi họ* $(E_i)_{i \in I}$ *là tự do đại số trên K*.

b) *Ngược lại, giả sử rằng* tr . deg$_K$ E = \sum_{i \in I} \text{tr . deg}_K E_i *và* tr . deg$_K$ E *hữu hạn; khi đó họ* (E_i)_{i \in I}, *là tự do đại số trên K*.

Với mỗi $i \in I$ hãy lấy $B_i$ là một cơ sở siêu việt của $E_i$ trên $K$ và đặt $B = \bigcup_{i \in I} B_i$. Với mỗi $i \in I$, mỗi phần tử của $E_i$ đều đại số trên $K(B_i)$, nên trên $K(B)$. Bây giờ Hệ quả 1 của $V$, p. 18 cho thấy $E$ là đại số trên $K(B)$; theo $V$, p. 109, Định lý 2, $B$ do đó chứa một cơ sở siêu việt của $E$ trên $K$. Nếu hơn nữa họ $(E_i)_{i \in I}$ là tự do đại số trên $K$, thì các $B_i$ rời nhau và tập hợp $B$ là tự do đại số trên $K$. Điều này chứng minh a) (*Lý thuyết tập hợp*, III, p. 160, Hệ quả của Mệnh đề 4).

Dưới các giả thiết của b), $E$ là đại số trên $K(B)$ và có bậc siêu việt hữu hạn trên $K$, và ta có Card$(B) \leq \text{tr . deg}_K E$. Theo Hệ quả 1 của $V$, p. 110, $B$ là tự do đại số trên $K$ và các $B_i$ đôi một rời nhau. Bây giờ Mệnh đề 15 cho thấy họ $(E_i)_{i \in I}$ là tự do đại số trên $K$.

Trước khi phát biểu định lý sau, ta nhận xét rằng tồn tại các mở rộng đóng đại số của $K$ có bậc siêu việt tùy ý, chẳng hạn một bao đóng đại số của một trường phân thức hữu tỉ thích hợp.

#### Định lý 5 {#alg-v-s14-thm-5 .statement}

— *Cho* (E_i)_{i \in I}, *là một họ các mở rộng của một trường K và* $\Omega$ *là một mở rộng đóng đại số của K*. *Giả sử rằng bất đẳng thức*

$$
\text{tr . deg}_K \Omega \geq \sum_{i \in I} \text{tr . deg}_K E_i
$$

*đúng. Khi đó tồn tại một họ tự do đại số* (F_i)_{i \in I}, *gồm các mở rộng con của* $\Omega$ *sao cho* F_i *là K-đẳng cấu với* E_i *với mọi* i \in I.

Với mỗi $i \in I$ hãy lấy $B_i$ là một cơ sở siêu việt của $E_i$ trên $K$. Hãy lấy $B$ là một cơ sở siêu việt của $\Omega$ trên $K$. Theo (2) ta có Card $B \geq \sum_{i \in I} \text{Card } B_i$; *do đó* tồn tại một họ (B'_i)_{i \in I}, *gồm các tập con đôi một rời nhau của $B$ và các song ánh* u_i : B_i \to B'_i *với* i \in I. *Theo Mệnh đề 2 của $V$, p. 106, u, mở rộng thành một K-đẳng cấu* v_i *của* K(B_i) *lên* K(B'_i); *vì* $\Omega$ *là đóng đại số và* E_i *đại số trên*

K(B_i), Hệ quả ($V$, p. 23) cho thấy rằng $v_i$ mở rộng thành một K-đẳng cấu của $E_i$ lên một mở rộng con $F_i$ của $\Omega$. Theo cách dựng $B'_i$ là một cơ sở siêu việt của $F_i$ trên $K$, và Mệnh đề 15 ($V$, p. 115) cho thấy họ $(F_i)_{i \in I}$ các mở rộng con của $\Omega$ là tự do đại số trên $K$.

#### Hệ quả 1 {#alg-v-s14-thm-5-cor-1 .statement}

— *Cho E và R là hai mở rộng của một trường K. Giả sử rằng* $\Omega$ *đóng đại số, có bậc siêu việt ít nhất bằng bậc của E. Khi đó E là K-đẳng cấu với một mở rộng con của R.*

#### Hệ quả 2 {#alg-v-s14-thm-5-cor-2 .statement}

— *Cho R là một trường đóng đại số có bậc siêu việt vô hạn trên trường con nguyên tố của nó. Khi đó mọi trường cùng đặc số với* $\Omega$ *đều là hợp có hướng tăng của các trường đẳng cấu với các trường con của R.*

Mỗi trường là hợp có hướng tăng của các trường con sinh hữu hạn trên trường con nguyên tố của nó, và bây giờ chỉ cần áp dụng Hệ quả 1.
\* Ví dụ. — Điều này áp dụng đặc biệt trong đặc số 0 khi lấy $\Omega = \mathbf{C}$ (« nguyên lý Lefschetz »). \*

### 7. Các mở rộng sinh hữu hạn

#### Mệnh đề 17 {#alg-v-s14-prop-17 .statement}

— *Cho E là một mở rộng của một trường K và B là một cơ sở siêu việt của E trên K. Để E sinh hữu hạn trên K* ($V$, p. 11, Định nghĩa 2) *cần và đủ là B hữu hạn và bậc* $[E : K(B)]$ *hữu hạn.*

Giả sử rằng E được sinh hữu hạn trên K và cho S là một tập con hữu hạn của E sao cho $E = K(S)$. Theo Định lý 2 (V, p. 109), S chứa một cơ sở siêu việt $B'$ của E trên K và cơ sở này có cùng lực lượng với B (V, p. 110, Định lý 3). Do đó B là hữu hạn. Đặt $K' = K(B)$; khi đó E là đại số trên $K'$ và ta có $E = K'(S)$; vì S hữu hạn, Định lý 2 của V, p. 18 cho thấy $[E : K']$ là hữu hạn.

Ngược lại, giả sử B là hữu hạn và $[E : K(B)]$ là hữu hạn. Nếu C là một cơ sở (hữu hạn) của không gian vectơ E trên $K(B)$, ta có $E = K(B)(C) = K(B \cup C)$ và do đó E là một mở rộng sinh hữu hạn của K.

#### Hệ quả 1 {#alg-v-s14-prop-17-cor-1 .statement}

— *Giả sử E là một mở rộng sinh hữu hạn của K, và cho $K'$ là bao đóng đại số tương đối của K trong E (V, p. 19). Khi đó $K'$ có bậc hữu hạn trên K.*

Cho B là một cơ sở siêu việt của E trên K. Theo Hệ quả 2 của V, p. 114, $K'$ tuyến tính rời nhau với $K(B)$ trên K, do đó $[K' : K] = [K'(B) : K(B)] \leq [E : K(B)]$ và bây giờ tính hữu hạn của $[K' : K]$ suy ra từ tính hữu hạn của $[E : K(B)]$.

#### Hệ quả 2 {#alg-v-s14-prop-17-cor-2 .statement}

— *Một trường được sinh hữu hạn trên trường con nguyên tố của nó chỉ chứa hữu hạn căn của đơn vị.*

Theo Hệ quả 1, ta chỉ còn phải chứng minh rằng một trường L là một mở rộng bậc hữu hạn của trường con nguyên tố của nó chỉ có hữu hạn căn của đơn vị. Điều này hiển nhiên khi L có đặc số $\neq 0$ vì khi đó L hữu hạn. Nếu L có đặc số 0 và chứa vô hạn căn của đơn vị, thì nó chứa các căn nguyên thủy của đơn vị có cấp tùy ý lớn. Theo V, p. 84, Định lý 2, do đó tồn tại vô hạn số nguyên $n > 0$ sao cho $\varphi(n) \leq [L : \mathbf{Q}]$, điều này vô lý (V, p. 80, Các công thức (2) và (3)).

#### Hệ quả 3 {#alg-v-s14-prop-17-cor-3 .statement}

— *Nếu E là một mở rộng sinh hữu hạn của một trường K, thì mọi mở rộng con E' của E đều là sinh hữu hạn.*

Cho B' là một cơ sở siêu việt của E' trên K. Theo V, p. 109, Định lý 2, B' được chứa trong một cơ sở siêu việt B của E trên K và do đó là hữu hạn, theo Mệnh đề 17. Vì E' là đại số trên K(B') và E là một mở rộng sinh hữu hạn của K(B'). Hệ quả 1 cho thấy $[E' : K(B')]$ là hữu hạn. Bây giờ Mệnh đề 17 cho thấy E' là sinh hữu hạn trên K.

Mệnh đề 17 có thể được diễn đạt lại bằng cách nói rằng một mở rộng sinh hữu hạn của K là một mở rộng đại số bậc hữu hạn của một mở rộng thuần siêu việt $K(x_1, \ldots, x_n)$.

### Bài tập {#alg-v-s14-exercises}

Xem [bài tập cho § 14](exercises/s14/).
