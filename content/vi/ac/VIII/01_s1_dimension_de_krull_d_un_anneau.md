---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 1
section_title: Dimension de Krull d’un anneau
lang: vi
source: ac-viii-ix-fr
book_pages: AC VIII.81-AC VIII.83
pdf_pages: 0005-0017, 0085-0087
extraction: ocr
subsections:
    - "no": 1
      title: Dimension de Krull d’un espace topologique
      page: 0
      pdf_page: 5
    - "no": 2
      title: Codimension d’une partie fermée
      page: 4
      pdf_page: 8
    - "no": 3
      title: Dimension d’un anneau, hauteur d’un idéal
      page: 6
      pdf_page: 10
    - "no": 4
      title: Dimension d’un module de type fini
      page: 10
      pdf_page: 14
    - "no": 5
      title: Cycles associés à un module
      page: 11
      pdf_page: 15
statements: 48
exercises: 17
content_sha256: 3d7038bd986edd139f48684d8d078d0c2177b5d3176d344b00a3df8d59685ab8
translated_from: content/en-mt/ac/VIII/01_s1_dimension_de_krull_d_un_anneau.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 4ad0eb0f476452fa6aae6b7aefc9c174eae5e33a449664a5e3bb8d39db37c88d
translation_model: gpt-5.4
translation_run: translate-vi-27d9b9c6
glossary_version: 34
glossary_terms_sha256: 46d3f01e779e3701c60cd4cabddba06534e260fc164c4ae8d2a5492b0b753fb6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. CHIỀU KRULL CỦA MỘT VÀNH

### 1. Chiều Krull của một Không gian Tôpô

#### Định nghĩa 1 {#ac-viii-s1-def-1 .statement}

Cho $I$ là một tập hợp có thứ tự. Một tập con hữu hạn khác rỗng được sắp thứ tự toàn phần của $I$ được gọi là một xích trong $I$. Cho $c$ là một xích trong $I$; phần tử nhỏ nhất và phần tử lớn nhất của $c$ được gọi là các đầu mút của $c$. Số nguyên $\mathrm{Card}(c) - 1$ được gọi là độ dài của $c$. Quan hệ bao hàm trong tập hợp các tập con của $I$ sinh ra một quan hệ thứ tự trong tập hợp các xích trong $I$. Một xích $c$ trong $I$ được gọi là bão hòa nếu nó là cực đại trong số các xích trong $I$ có cùng các đầu mút với $c$.

Để chỉ một xích c có độ dài n, ta sẽ thường viết: “xích $i_0 < \cdots < i_n$”, trong đó các $i_k$ là các phần tử của c được đánh số theo thứ tự tăng ngặt bởi các số nguyên từ 0 đến n.

Cho X là một không gian tôpô. Ta trang bị tập hợp các tập con đóng bất khả quy của X (II, § 4, No. 1, Def. 1) với quan hệ thứ tự được xác định bởi bao hàm. Mỗi khi ta nói đến một xích các tập con đóng bất khả quy của X, điều đó luôn luôn có nghĩa là một xích đối với quan hệ thứ tự này.

#### Định nghĩa 2 {#ac-viii-s1-def-2 .statement}

Chiều Krull của không gian tôpô X, theo định nghĩa, được ký hiệu là dim kr(X), hoặc đơn giản là dim(X), là cận trên nhỏ nhất trong $\overline{\mathbf{R}}$ của tập hợp các độ dài của các xích các tập con đóng bất khả quy của X.
Với mọi điểm x của X, chiều Krull của X tại x, theo định nghĩa, được ký hiệu là $\dim_x(X)$, là cận dưới lớn nhất của các chiều của các lân cận mở của x.

Ta có $\dim(\varnothing) = -\infty$. Mặt khác, nếu X khác rỗng, bao đóng của mọi điểm của X là một tập con đóng bất khả quy của X (II, § 4, No. 1, Prop. 2), và do đó chiều của X hoặc là $+\infty$ hoặc là một số nguyên dương. Giả sử rằng X tách và khác rỗng; khi đó mọi tập con bất khả quy của X đều thu về một điểm, và X có chiều 0.
Do đó định nghĩa chiều Krull là không có mấy ý nghĩa đối với các không gian tách, nhưng nó đặc biệt thích nghi với các không gian tôpô gặp trong Đại số giao hoán (phổ của các vành, \* lược đồ *, ...). Trong chương này, không có sự lẫn lộn nào phải e ngại với các khái niệm khác về chiều của các không gian tôpô (chẳng hạn khái niệm của Lebesgue), và ta sẽ đơn giản nói “chiều” thay cho “chiều Krull”.

#### Mệnh đề 1 {#ac-viii-s1-prop-1 .statement}

Cho X là một không gian tôpô.
a) Nếu Y là một không gian con của X, thì $\dim(Y) \leq \dim(X)$, và $\dim_y(Y) \leq \dim_y(X)$ với mọi điểm y của Y.
b) Cho x là một điểm của X và V là một lân cận của x trong X. Khi đó $\dim_x(X) = \dim_x(V)$.
c) Cho $(X_i)_{i \in I}$ là một họ hữu hạn các tập con đóng của X sao cho $X = \bigcup_{i \in I} X_i$. Khi đó $\dim(X) = \sup_{i \in I} \dim(X_i)$ và, với mọi điểm x của X, ta có $\dim_x(X) = \sup_{i \in J_x} \dim_x(X_i)$, trong đó $J_x$ chỉ tập hợp các $i \in I$ sao cho $x \in X_i$.

Hãy chứng minh a). Nếu Z là một tập con đóng bất khả quy của Y, thì bao đóng $\overline{Z}$ của nó trong X là bất khả quy (II, § 4, No. 1, Prop. 2), và ta có $\overline{Z} \cap Y = Z$. Do đó mỗi xích c của các tập con đóng bất khả quy của Y xác định, bằng cách chuyển qua bao đóng trong X, một xích các tập con đóng bất khả quy của X, có cùng độ dài như c. Bất đẳng thức $\dim(Y) \leq \dim(X)$ suy ra từ đó. Nếu U là một tập con mở của X chứa một điểm y của Y, thì do đó $\dim(U \cap Y) \leq \dim(U)$, do đó $\dim_y(Y) \leq \dim_y(X)$.
Hãy chứng minh b). Theo định nghĩa ta có $\dim_x(X) \leq \dim_x(V)$, và bất đẳng thức ngược lại suy ra từ a).
Hãy chứng minh c). Cho $Z_0 \subset \ldots \subset Z_n$ là một xích các tập con đóng bất khả quy của X. Ta có $Z_n = \bigcup_{i \in I} (Z_n \cap X_i)$ và mỗi tập hợp $Z_n \cap X_i$ đều đóng trong $Z_n$;

vì I là hữu hạn, $Z_n$ được chứa trong một trong các $X_i$. Do đó, ta có $\dim(X) \leq \sup_{i} \dim(X_i)$, do đó có đẳng thức theo *a*).

Bây giờ cho $x$ là một điểm của $X$ và $n = \sup_{i \in J_x} \dim_x(X_i)$, trong đó $J_x$ như trong mệnh đề. Ta có $\dim_x(X) \geq n$ theo *a*), và, để thiết lập đẳng thức, có thể giả sử $n$ hữu hạn. Với mọi $i \in J_x$, cho $U_i$ là một lân cận mở của $x$ trong $X$, sao cho $\dim(U_i \cap X_i) \leq n$. Đặt $U = (\bigcap_{i \in J_x} U_i) \cap (\bigcap_{i \in I - J_x} \mathcal{C} X_i)$; tập hợp $U$ là mở trong $X$. Hơn nữa, ta có $\dim(U) = \sup_{i \in J_x} \dim(U \cap X_i) \leq n$ theo đoạn trước, nên $\dim_x(X) \leq n$.

#### Hệ quả {#ac-viii-s1-n1-cor-1 .statement}

*a*) *Chiều của không gian tôpô $X$ là cận trên nhỏ nhất của các chiều của các thành phần bất khả quy của nó* (II, § 4, No. 1, Def. 2).

*b*) *Cho $x$ là một điểm của $X$. Khi đó $\dim_x(X) \geq \sup \dim_x(X_i)$, trong đó $X_i$ chạy qua họ các thành phần bất khả quy của $X$ chứa $x$; có đẳng thức nếu $x$ có một lân cận $V$ chỉ có một số hữu hạn thành phần bất khả quy (chẳng hạn đó là trường hợp khi $V$ là Noether)*.

Mệnh đề thứ nhất là ngay lập tức vì các chuỗi tập con đóng bất khả quy của $X$ chính là các chuỗi tập con đóng bất khả quy của các thành phần bất khả quy của $X$ (II, § 4, No. 1, Prop. 5). Bất đẳng thức $\dim_x(X) \geq \sup_{i} \dim_x(X_i)$ suy ra từ Mệnh đề 1, *a*). Cho $V$ là một lân cận của $x$ chỉ có một số hữu hạn thành phần bất khả quy, và gọi $(V_j)_{j \in J}$ là họ các thành phần bất khả quy của $V$ chứa $x$. Từ Mệnh đề 1, *b*) và *c*) suy ra rằng ta có
$$
\dim_x(X) = \dim_x(V) = \sup_{j \in J} \dim_x(V_j);
$$
ta kết luận bằng cách nhận thấy rằng mỗi $V_j$ được chứa trong một trong các $X_i$, $i \in J_x$, và do đó ta có $\sup_{j \in J} \dim_x(V_j) \leq \sup_{i \in J_x} \dim_x(X_i)$.

#### Mệnh đề 2 {#ac-viii-s1-prop-2 .statement}

*Cho $X$ là một không gian tôpô. Khi đó $\dim(X) = \sup_{x \in X} \dim_x(X)$*.

Thật vậy, theo định nghĩa ta có $\dim(X) \geq \dim_x(X)$ với mọi $x \in X$. Mặt khác, nếu $Z_0 \subset ... \subset Z_n$ là một chuỗi tập con đóng bất khả quy của $X$, thì với mọi $x \in Z_0$ và mọi lân cận mở $U$ của $x$, các tập hợp $Z_0 \cap U, ..., Z_n \cap U$ tạo thành một chuỗi tập con đóng bất khả quy của $U$ (II, § 4, No. 1, Prop. 7). Do đó $\dim_x(X) \geq n$, suy ra $\dim(X) \leq \sup_{x \in X} \dim_x(X)$.

#### Hệ quả {#ac-viii-s1-n1-cor-2 .statement}

*Nếu $(X_\alpha)_{\alpha \in A}$ là một phủ mở, hoặc một phủ đóng hữu hạn địa phương, của một không gian tôpô $X$, thì ta có*
$$
\dim(X) = \sup_{\alpha \in A} \dim(X_\alpha).
$$

Chỉ cần chứng minh rằng, với mọi điểm $x$ của $X$, ta có $\dim_x(X) = \sup_{\alpha \in A_x} \dim_x(X_\alpha)$, trong đó $A_x$ là tập hợp các $\alpha \in A$ sao cho $x \in X_\alpha$. Điều này là hiển nhiên trong trường hợp một phủ mở, và suy ra từ Mệnh đề 1, c), trong trường hợp một phủ đóng hữu hạn địa phương.

### 2. Đối chiều của một tập con đóng

#### Định nghĩa 3 {#ac-viii-s1-def-3 .statement}

Cho X là một không gian tôpô.

a) Nếu Y là một tập con đóng bất khả quy của X, đối chiều của Y trong X được định nghĩa là cận trên nhỏ nhất trong $\overline{\mathbf{R}}$ của các độ dài những chuỗi tập con đóng bất khả quy của X mà trong đó Y là phần tử nhỏ nhất.

b) Nếu Y là một tập con đóng của X, đối chiều của Y trong X được định nghĩa là cận dưới lớn nhất trong $\overline{\mathbf{R}}$ của các đối chiều, trong X, của các thành phần bất khả quy của Y, và được ký hiệu là $\operatorname{codim}(Y, X)$.

#### Nhận xét 1 {#ac-viii-s1-n2-rem-1 .statement}

Đối chiều của một tập con đóng Y của X vì thế là cận dưới lớn nhất của các đối chiều của các tập con đóng bất khả quy của Y. Ta có $\operatorname{codim}(\varnothing, X) = +\infty$ và, nếu X không rỗng, $\operatorname{codim}(X, X) = 0$. Mọi tập con đóng khác rỗng của X đều chứa một tập con đóng bất khả quy (II, § 4, No. 1, Prop. 5); vì thế đối chiều trong X của một tập con đóng Y luôn luôn là một số nguyên dương hoặc $+\infty$; nó bằng không khi và chỉ khi Y chứa một thành phần bất khả quy của X.

#### Nhận xét 2 {#ac-viii-s1-n2-rem-2 .statement}

Nếu Y là một tập con đóng khác rỗng của X, ta có $\operatorname{codim}(Y, X) \leq \dim(X)$. Ta có $\dim(X) = \sup_Y \operatorname{codim}(Y, X)$, trong đó Y chạy qua tập hợp các tập con đóng bất khả quy của X. Nếu Y và Y’ là hai tập con đóng của X sao cho $Y' \subset Y$, ta có $\operatorname{codim}(Y, X) \leq \operatorname{codim}(Y', X)$.

#### Nhận xét 3 {#ac-viii-s1-n2-rem-3 .statement}

Cho $Y$ là một tập con đóng của không gian tôpô $X$ và $(X_\alpha)_{\alpha \in A}$ (resp. $(Y_\beta)_{\beta \in B}$) là họ các thành phần bất khả quy của $X$ (resp. của $Y$). Với mỗi $\beta \in B$, ký hiệu $A(\beta)$ là tập hợp các $\alpha \in A$ sao cho $Y_\beta \subset X_\alpha$. Vì mọi tập con bất khả quy của $X$ đều được chứa trong một trong các $X_\alpha$ (II, § 4, No. 1, Mệnh đề 5), suy ra từ Định nghĩa 3 rằng ta có:

$$
\operatorname{codim}(Y, X) = \inf_{\beta \in B} \sup_{\alpha \in A(\beta)} \operatorname{codim}(Y_\beta, X_\alpha).
$$

#### Nhận xét 4 {#ac-viii-s1-n2-rem-4 .statement}

Cho $(Y_i)_{i \in I}$ là một họ hữu hạn các tập con đóng của $X$ và $Y = \bigcup_{i \in I} Y_i$; ta có

$$
\operatorname{codim}(Y, X) = \inf_{i \in I} \operatorname{codim}(Y_i, X).
$$

Thật vậy, mọi thành phần bất khả quy của $Y$ đều được chứa trong một trong các $Y_i$.

#### Mệnh đề 3 {#ac-viii-s1-prop-3 .statement}

Cho $X$ là một không gian tôpô.

a) Với mọi tập con đóng khác rỗng $Y$ của $X$, ta có

$$
\dim(Y) + \operatorname{codim}(Y, X) \leq \dim(X).
$$

b) Nếu $Y, Z, T$ là các tập con đóng của $X$ sao cho $Y \subset Z \subset T$, ta có

$$
\operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T) \leq \operatorname{codim}(Y, T).
$$

Chỉ cần chứng minh mệnh đề a) trong trường hợp $\dim(X)$ là hữu hạn. Trong trường hợp này, $\dim(Y)$ và $\operatorname{codim}(Y, X)$ là hữu hạn. Tồn tại một chuỗi $Y_0 \subset ... \subset Y_n$ các tập con đóng bất khả quy của $Y$, có độ dài $n = \dim(Y)$, và một chuỗi $Y_n \subset ... \subset Y_{n+p}$ các tập con đóng bất khả quy của $X$, có độ dài $p \geq \operatorname{codim}(Y, X)$. Suy ra $\dim(X) \geq n + p$, do đó a). Để thiết lập b), có thể giả sử $Y$ là bất khả quy. Vì ta có $\operatorname{codim}(Y, Z) \leq \operatorname{codim}(Y, T)$, bất đẳng thức được chứng minh nếu $\operatorname{codim}(Y, Z) = +\infty$. Nếu không, gọi $Z_0$ là một thành phần bất khả quy của $Z$ chứa $Y$ và sao cho $\operatorname{codim}(Y, Z) = \operatorname{codim}(Y, Z_0)$. Ta có $\operatorname{codim}(Z, T) \leq \operatorname{codim}(Z_0, T)$, và ta thấy, như trên, rằng $\operatorname{codim}(Y, Z_0) + \operatorname{codim}(Z_0, T) \leq \operatorname{codim}(Y, T)$, do đó b).

#### Định nghĩa 4 {#ac-viii-s1-def-4 .statement}

Một không gian tôpô $X$ được gọi là catenaire nếu, với mọi cặp $(Y, Z)$ các tập con đóng bất khả quy của $X$ sao cho $Y \subset Z$, mọi chuỗi bão hòa các tập con đóng bất khả quy với hai đầu mút là $Y$ và $Z$ đều có độ dài $\operatorname{codim}(Y, Z)$.

Nói rằng, với mọi cặp $(Y, Z)$ các tập con đóng bất khả quy của $X$ sao cho $\operatorname{codim}(Y, Z)$ là hữu hạn, mọi chuỗi bão hòa có các đầu mút $Y$ và $Z$ đều có cùng độ dài, và nói rằng, với mọi cặp $(Y, Z)$ sao cho $\operatorname{codim}(Y, Z) = +\infty$, không tồn tại chuỗi bão hòa nào có các đầu mút $Y$ và $Z$, là tương đương nhau.

Mọi không gian con đóng của một không gian catenary đều là catenary. Để một không gian là catenary, điều kiện cần và đủ là mọi thành phần bất khả quy của nó đều như vậy.

#### Mệnh đề 4 {#ac-viii-s1-prop-4 .statement}

Cho $X$ là một không gian tôpô. Để $X$ là catenary, điều kiện cần và đủ là, với mọi bộ ba $(Y, Z, T)$ các tập con đóng bất khả quy của $X$ sao cho $Y \subset Z \subset T$, ta có:

$$
\operatorname{codim}(Y, T) = \operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T)
$$

Giả sử $X$ là catenary. Theo Mệnh đề 3, b), chỉ cần chứng minh hệ thức khi $\operatorname{codim}(Y, Z)$ và $\operatorname{codim}(Z, T)$ là hữu hạn. Bằng cách nối đuôi một chuỗi bão hòa các tập con đóng bất khả quy có các đầu mút $Y$ và $Z$, độ dài $\operatorname{codim}(Y, Z)$, với một chuỗi bão hòa các tập con đóng bất khả quy có các đầu mút $Z$ và $T$, độ dài $\operatorname{codim}(Z, T)$, ta thu được một chuỗi bão hòa có các đầu mút $Y$ và $T$, độ dài $\operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T)$. Nhưng vì $X$ là catenary, độ dài này tất yếu bằng $\operatorname{codim}(Y, T)$.

Ngược lại, giả sử rằng ta có $\operatorname{codim}(Y, T) = \operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T)$ với mọi tập con đóng bất khả quy $Y, Z, T$ của $X$ sao cho $Y \subset Z \subset T$, và hãy chứng minh rằng $X$ là catenary. Để làm điều đó, ta chứng minh bằng quy nạp theo số nguyên $n \geq 0$ rằng, với mọi chuỗi bão hòa $Z_0 \subset ... \subset Z_n$ các tập con đóng bất khả quy của $X$, ta có $\operatorname{codim}(Z_0, Z_n) = n$. Nếu $n = 0$, điều này là hiển nhiên. Cho $n > 0$, và giả sử tính chất đúng với các chuỗi có độ dài $\leq n - 1$. Nếu $Z_0 \subset ... \subset Z_n$ là một chuỗi bão hòa độ dài $n$, thì $Z_0 \subset ... \subset Z_{n-1}$ là một chuỗi bão hòa độ dài $n - 1$, do đó $\operatorname{codim}(Z_0, Z_{n-1}) = n - 1$. Theo giả thiết đặt ra trên $X$, ta có $\operatorname{codim}(Z_0, Z_n) = \operatorname{codim}(Z_0, Z_{n-1}) + \operatorname{codim}(Z_{n-1}, Z_n) = (n - 1) + 1 = n$.

#### Hệ quả {#ac-viii-s1-n2-cor-1 .statement}

Cho X là một không gian tôpô bất khả quy có số chiều hữu hạn. Để X là catenary, điều kiện cần và đủ là, với mọi cặp (Y, Z) các tập con đóng bất khả quy của X sao cho Y ⊂ Z, ta có codim(Y, X) = codim(Y, Z) + codim(Z, X).

Điều kiện này là cần theo Mệnh đề 4. Ngược lại, giả sử nó được thỏa mãn, và ký hiệu bởi c(Z) số nguyên codim(Z, X) với mọi tập con đóng bất khả quy Z của X. Nếu Y, Z, T là ba tập con đóng bất khả quy của X sao cho Y ⊂ Z ⊂ T, ta có
$$
\begin{align*}
\operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T) &= (c(Y) - c(Z)) + (c(Z) - c(T)) \\
&= c(Y) - c(T) \\
&= \operatorname{codim}(Y, T),
\end{align*}
$$
và X là catenary theo Mệnh đề 4.

#### Mệnh đề 5 {#ac-viii-s1-prop-5 .statement}

Cho X là một không gian tôpô có số chiều hữu hạn. Giả sử rằng mọi chuỗi cực đại các tập con đóng bất khả quy của X đều có cùng độ dài. Khi đó X là catenary; với mọi tập con đóng bất khả quy Z của X, ta có
$$
\operatorname{codim}(Z, X) = \dim(X) - \dim(Z);
$$
với mọi cặp (Y, Z) các tập con đóng bất khả quy của X sao cho Y ⊂ Z, ta có
$$
\operatorname{codim}(Y, Z) = \dim(Z) - \dim(Y).
$$

Cho Y và Z là hai tập con đóng bất khả quy của X sao cho Y ⊂ Z. Cho $Y_0 \subset ... \subset Y_p$ là một chuỗi sao cho $Y_p = Y$ và p = \dim(Y), $Z_0 \subset ... \subset Z_q$ một chuỗi sao cho $Z_0 = Z$ và q = \operatorname{codim}(Z, X). Với mọi chuỗi bão hòa $T_0 \subset ... \subset T_r$ sao cho $T_0 = Y$ và $T_r = Z$, chuỗi
$$
Y_0 \subset ... \subset Y_{p-1} \subset T_0 \subset ... \subset T_r \subset Z_1 ... \subset Z_q
$$
là cực đại, và có độ dài p + q + r; do giả thiết đặt ra trên X, vì vậy ta có p + q + r = \dim(X), tức là r = \dim(X) - \dim(Y) - \operatorname{codim}(Z, X). Suy ra X là catenary và rằng, với Y và Z như trên, ta có
$$
\dim(Y) + \operatorname{codim}(Y, Z) = \dim(X) - \operatorname{codim}(Z, X).
$$
Lấy Y = Z, ta thấy vế thứ hai bằng \dim(Z), do đó có mệnh đề.

### 3. Chiều của một vành, độ cao của một iđêan

#### Định nghĩa 5 {#ac-viii-s1-def-5 .statement}

Chiều Krull, hay đơn giản là chiều, của một vành A (giao hoán) theo định nghĩa là chiều Krull của không gian tôpô Spec(A) (II, § 4, No. 3, Định nghĩa 4); nó được ký hiệu bởi \dim(A). Nếu p là một iđêan nguyên tố của A, chiều của A tại p theo định nghĩa là số \dim_p(\operatorname{Spec}(A)); nó được ký hiệu bởi \dim_p(A).

Ánh xạ $p \mapsto V(p)$ là một song ánh giảm từ tập hợp các iđêan nguyên tố của $A$ lên tập hợp các tập con đóng bất khả quy của $\mathrm{Spec}(A)$ (*loc. cit.*, Hệ quả 2 của Mệnh đề 14). *Do đó chiều của $A$ là cận trên bé nhất của tập hợp các độ dài của các chuỗi iđêan nguyên tố của $A$*; nó bằng $-\infty, +\infty$ hoặc bằng một số nguyên dương.

Cho $p \in \mathrm{Spec}(A)$; các tập hợp $\mathrm{Spec}(A)_f$, khi $f$ chạy qua $A$, lập thành một cơ sở của tôpô trên $\mathrm{Spec}(A)$, và $p$ thuộc tập hợp mở $\mathrm{Spec}(A)_f$ khi và chỉ khi $f$ không thuộc $p$. Do đó, $\dim_p(A)$ là cận dưới lớn nhất của các số $\dim(A_f)$, khi $f$ chạy qua $A - p$ (II, § 5, No. 1, Mệnh đề 1).

#### Ví dụ 1 {#ac-viii-s1-n3-exa-1 .statement}

Ta có $\dim(A) < 0$ khi và chỉ khi $A$ thu về 0. Để có $\dim(A) \leqslant 0$, điều kiện cần và đủ là mọi iđêan nguyên tố của $A$ đều cực đại. Các vành nguyên có chiều 0 là các trường. Một vành Noether có chiều $\leqslant 0$ khi và chỉ khi nó là Artin (IV, § 2, No. 5, mệnh đề 9).

#### Ví dụ 2 {#ac-viii-s1-n3-exa-2 .statement}

Các vành Dedekind là các vành Noether nguyên đóng có chiều $\leqslant 1$ (VII, § 2, No. 2, định lý 1). Nói chung hơn, theo V, § 1, No. 2, hệ quả 2 của mệnh đề 9, một vành là một tích hữu hạn các vành Dedekind khi và chỉ khi nó là Noether, thu gọn, nguyên đóng trong vành phân thức toàn phần của nó, và có chiều $\leqslant 1$.

#### Ví dụ 3 {#ac-viii-s1-n3-exa-3 .statement}

Nếu $A$ là một vành định giá (VI, § 1, No. 2, định nghĩa 2), thì chiều của nó bằng với chiều cao của định giá (VI, § 4, No. 4, mệnh đề 5).

#### Ví dụ 4 {#ac-viii-s1-n3-exa-4 .statement}

Cho $A$ là một vành. Ta có
$$
\dim(A[X]) \geqslant \dim(A) + 1 .
$$
Thật vậy, nếu $p_0 \subset ... \subset p_n$ là một chuỗi các iđêan nguyên tố của $A$, có độ dài $n$, thì ta thu được một chuỗi $p'_0 \subset ... \subset p'_{n+1}$ các iđêan nguyên tố của $A[X]$, có độ dài $n + 1$, bằng cách đặt $p'_i = p_i A[X]$ với $0 \leq i \leq n$, và $p'_{n+1} = p_n A[X] + XA[X]$.

Bằng cùng một lập luận, ta chứng minh được bất đẳng thức $\dim(A[[X]]) \geqslant \dim(A) + 1$. Bằng quy nạp suy ra các bất đẳng thức
$$
\dim(A[X_1, ..., X_n]) \geqslant \dim(A) + n ,
$$
$$
\dim(A[[X_1, ..., X_n]]) \geqslant \dim(A) + n .
$$

Sau này chúng tôi sẽ chứng minh (§ 3, No. 4, hệ quả 3 của mệnh đề 7 và hệ quả 3 của mệnh đề 8) rằng ta có đẳng thức trong hai công thức trước khi $A$ là Noether.

#### Ví dụ 5 {#ac-viii-s1-n3-exa-5 .statement}

Cho $X$ là một đa tạp giải tích phức. Nếu $X$ có chiều phức $n$ tại một điểm $x$ của $X$, thì vành địa phương của các mầm tại $x$ của các hàm giải tích trên $X$ có chiều $n$. \*

#### Ví dụ 6 {#ac-viii-s1-n3-exa-6 .statement}

Cho $k$ là một trường và $A$ là một $k$-đại số nguyên khác không. Khi đó ta có $\dim(A) = 0$. Điều này suy ra từ hệ quả 1 của mệnh đề 1 trong V, § 2, No. 1, và từ sự kiện $\dim(k) = 0$.

#### Ví dụ 7 {#ac-viii-s1-n3-exa-7 .statement}

Nếu $\mathfrak{n}$ là một iđêan lũy linh của $A$, thì $\mathrm{Spec}(A)$ đồng phôi với $\mathrm{Spec}(A/\mathfrak{n})$ (II, § 4, No. 3, nhận xét). Vì vậy ta có $\dim(A/\mathfrak{n}) = \dim(A)$; đặc biệt, ta có $\dim(A) = \dim(A_{\mathrm{red}})$ trong đó $A_{\mathrm{red}}$ là thương của vành $A$ theo căn lũy linh của nó.

#### Ví dụ 8 {#ac-viii-s1-n3-exa-8 .statement}

Tồn tại các vành Noether có chiều vô hạn (p. 83, bài tập 13). Dưới đây chúng ta sẽ thấy (§ 3, No. 1, hệ quả 1 của mệnh đề 2) rằng mọi vành địa phương Noether đều có chiều hữu hạn.

#### Mệnh đề 6 {#ac-viii-s1-prop-6 .statement}

Cho A là một vành.
a) Nếu a là một iđêan của A, ta có dim(A/a) $\leq$ dim(A).
b) Nếu S là một tập hợp nhân của A, ta có dim(S$^{-1}$A) $\leq$ dim(A).
c) Ta có dim(A) = sup dim(A/p), trong đó p chạy qua tập hợp các iđêan nguyên tố cực tiểu của A.
d) Nếu A chỉ có một số hữu hạn các iđêan nguyên tố cực tiểu (chẳng hạn nếu A là Noether (II, § 4, No. 3, hệ quả 3 của mệnh đề 14)) và nếu p là một iđêan nguyên tố của A, ta có
$$
\dim_p(A) = \sup_q \dim_{p/q}(A/q),
$$
trong đó q chạy qua tập hợp các iđêan nguyên tố cực tiểu của A được chứa trong p.
e) Cho a là một iđêan của A không được chứa trong bất kỳ iđêan nguyên tố cực tiểu nào của A; khi đó ta có dim(A) $\geq$ dim(A/a) + 1. Đặc biệt, nếu A là nguyên, thì ta có dim(A) $\geq$ dim(A/a) + 1 với mọi iđêan khác không a của A.

Theo nhận xét của II, § 4, No. 3, nếu a là một iđêan của A, không gian tôpô Spec(A/a) đồng phôi với không gian con đóng V(a) của Spec(A). Mệnh đề a) suy ra từ điều này và từ mệnh đề 1, a) của No. 1. Mệnh đề b) suy ra từ loc. cit., hệ quả của mệnh đề 13. Theo loc. cit., hệ quả 2 của mệnh đề 14, các thành phần bất khả quy của Spec(A) đồng phôi với các không gian Spec(A/p), trong đó p là một iđêan nguyên tố cực tiểu của A, và mệnh đề c) suy ra từ hệ quả của mệnh đề 1 của No. 1. Dưới giả thiết của d), không gian Spec(A) chỉ có một số hữu hạn các thành phần bất khả quy; các thành phần bất khả quy của Spec(A) chứa p là các tập hợp V(q), trong đó q là một iđêan nguyên tố cực tiểu được chứa trong p. Khi đó mệnh đề d) suy ra từ hệ quả, b) của mệnh đề 1 của No. 1.

Sau cùng, hãy chứng minh e). Vấn đề là chứng minh rằng, với mọi dãy $p_0 \subset ... \subset p_n$ các iđêan nguyên tố của A sao cho $a \subset p_0$, ta có dim(A) $\geq n + 1$. Do giả thiết đặt trên a, tồn tại một iđêan nguyên tố $p_{-1}$ của A được chứa trong $p_0$, phân biệt với $p_0$, và $p_{-1} \subset p_0 \subset ... \subset p_n$ là một dãy các iđêan nguyên tố của A, có độ dài $n + 1$.

#### Nhận xét 1 {#ac-viii-s1-n3-rem-1 .statement}

Cho $\rho : A \to B$ là một đồng cấu vành. Khi đó dim(B) là cận trên bé nhất của các số dim(B/$\rho(p)$.B), trong đó p chạy qua tập hợp các iđêan nguyên tố cực tiểu của A: thật vậy, với mọi iđêan nguyên tố cực tiểu q của B, tồn tại một iđêan nguyên tố cực tiểu p của A được chứa trong $\rho^{-1}(q)$ (II, § 2, No. 6, Bổ đề 2), và ta có
$$
\dim(B/q) \leq \dim(B/\rho(p).B) \leq \dim(B)
$$
theo Mệnh đề 6, a); suy ra kết luận nhờ Mệnh đề 6, c).

#### Định nghĩa 6 {#ac-viii-s1-def-6 .statement}

Cho a là một iđêan của một vành A. Đối chiều của V(a) trong Spec(A) được gọi là chiều cao của iđêan a và được ký hiệu là ht(a).

Giả sử A là một miền nguyên. Khi đó các iđêan nguyên tố có chiều cao 1 của A theo nghĩa của Định nghĩa 4 của VII, § 1, No. 6 là các iđêan nguyên tố có chiều cao 1 theo nghĩa của định nghĩa trên.

#### Mệnh đề 7 {#ac-viii-s1-prop-7 .statement}

a) Chiều cao của một iđêan nguyên tố p của A là cận trên bé nhất của các độ dài của những dãy iđêan nguyên tố $p_0 \subset ... \subset p_n$ sao cho $p_n = p$.

b) Cho p là một iđêan nguyên tố của A và a là một iđêan của A. Khi đó ta có $\dim(A_p/aA_p) = -\infty$ nếu a không được chứa trong p, và $\dim(A_p/aA_p) = \operatorname{codim}(V(p), V(a))$ nếu a được chứa trong p. Đặc biệt, nếu p là một iđêan nguyên tố của A, ta có $\dim(A_p) = \operatorname{ht}(p)$.

c) Nếu a là một iđêan của A, ta có $\operatorname{ht}(a) = \inf_{p} \operatorname{ht}(p) = \inf_{p} \dim(A_p)$ trong đó p chạy qua tập hợp các iđêan nguyên tố của A chứa a.

Mệnh đề a) là bản dịch của Định nghĩa 3, a) của No. 2. Mệnh đề b) suy ra từ việc ánh xạ $q \mapsto q(A_p/aA_p)$ là một đẳng cấu tăng của tập hợp các iđêan nguyên tố q của A sao cho $a \subset q \subset p$ lên tập hợp các iđêan nguyên tố của vành địa phương $A_p/aA_p$ (II, § 2, No. 5, Mệnh đề 11). Cho a là một iđêan của A; các tập con đóng bất khả quy của $V(a)$ là các tập hợp $V(p)$, trong đó p là một iđêan nguyên tố của A chứa a. Do đó mệnh đề c) suy ra từ Nhận xét 1 của No. 2.

#### Hệ quả {#ac-viii-s1-n3-cor-1 .statement}

Cho p là một iđêan nguyên tố của A và S là một tập hợp nhân của A không giao với p. Khi đó $\operatorname{ht}(p) = \operatorname{ht}(S^{-1}p)$.

Điều này suy ra từ Mệnh đề 7, a), và từ II, § 2, No. 5, Mệnh đề 11.

#### Mệnh đề 8 {#ac-viii-s1-prop-8 .statement}

Cho A là một vành.

a) Ta có $\dim(A) = \sup_m \dim(A_m) = \sup_m \operatorname{ht}(m)$, trong đó m chạy qua tập hợp các iđêan cực đại (resp. nguyên tố) của A.

b) Cho b là một iđêan của A phân biệt với A, và a là một iđêan của A được chứa trong b. Khi đó ta có $\operatorname{codim}(V(b), V(a)) + \dim(A/b) \leq \dim(A/a)$. Đặc biệt, với mọi iđêan b của A phân biệt với A, ta có bất đẳng thức $\operatorname{ht}(b) + \dim(A/b) \leq \dim(A)$.

Mệnh đề thứ nhất suy ra từ Nhận xét 2 của No. 2 và từ Mệnh đề 7, b). Mệnh đề thứ hai suy ra từ Mệnh đề 3, a) của No. 2 và từ các hệ thức $\dim(A/b) = \dim(V(b))$, $\dim(A/a) = \dim(V(a))$.

#### Định nghĩa 7 {#ac-viii-s1-def-7 .statement}

Một vành A được gọi là catenary nếu không gian tôpô Spec(A) là catenary (No. 2, Định nghĩa 4).

Do đó điều này có nghĩa là, với mọi cặp (p, q) các iđêan nguyên tố của A sao cho $q \subset p$, mọi dãy bão hòa các iđêan nguyên tố của A với các đầu mút p và q đều có độ dài $\operatorname{codim}(V(p), V(q)) = \dim(A_p/qA_p)$.

#### Nhận xét 2 {#ac-viii-s1-n3-rem-2 .statement}

Mọi vành thương của một vành catenary đều là catenary. Để vành A là catenary, điều kiện cần và đủ là, với mọi iđêan nguyên tố p của A, vành $A_p$ là catenary.

#### Nhận xét 3 {#ac-viii-s1-n3-rem-3 .statement}

Theo Mệnh đề 7, b) và Mệnh đề 4 của No. 2, vành A là catenary khi và chỉ khi, với mọi bộ ba (p, q, r) các iđêan nguyên tố của A sao cho $r \subset q \subset p$, ta có dim(A_p/qA_p) + dim(A_q/rA_q) = dim(A_p/rA_p). Nếu A là một miền nguyên và có số chiều hữu hạn, thì A là catenary khi và chỉ khi ta có ht(q) + dim(A_p/qA_p) = ht(p) với mọi cặp (p, q) các iđêan nguyên tố của A sao cho q ⊂ p. Thật vậy, khi đó không gian tôpô Spec(A) là bất khả quy và có số chiều hữu hạn, và ta áp dụng Hệ quả của Mệnh đề 4 của No. 2.

#### Nhận xét 4 {#ac-viii-s1-n3-rem-4 .statement}

Cho A là một vành có số chiều hữu hạn mà mọi chuỗi cực đại các iđêan nguyên tố đều có cùng độ dài. Khi đó A là catenary, ta có ht(p) + dim(A/p) = dim(A) với mọi iđêan nguyên tố p của A, và dim(A_p/qA_p) + dim(A/p) = dim(A/q) với mọi cặp (p, q) các iđêan nguyên tố của A sao cho q ⊂ p (No. 2, Mệnh đề 5).

#### Nhận xét 5 {#ac-viii-s1-n3-rem-5 .statement}

Ta sẽ thấy ở § 2, No. 4, rằng mọi đại số hữu hạn sinh trên một trường đều là một vành catenary. Có những vành địa phương Noether không catenary (p. 83, Bài tập 16).

### 4. Chiều của một môđun hữu hạn sinh

#### Định nghĩa 8 {#ac-viii-s1-def-8 .statement}

Cho A là một vành và M là một A-môđun hữu hạn sinh. Chiều Krull (hay đơn giản là chiều $^1$) của A-môđun M là chiều Krull của giá đỡ của M (II, § 4, No. 4, Định nghĩa 5); nó được ký hiệu là $\dim_A(M)$ (hay $\dim(M)$ nếu không có sự nhập nhằng).

Giá đỡ của A-môđun A là Spec(A); do đó chiều của A-môđun A bằng chiều của vành A.

Cho M là một A-môđun hữu hạn sinh và α là linh hóa tử của nó; ta có

$$
\operatorname{Supp}(M) = V(\alpha) = \operatorname{Supp}(A/\alpha)
$$

(II, § 4, n° 4, prop. 17). Do đó chiều của A-môđun M, chiều của A-môđun A/α, chiều của vành A/α và chiều của (A/α)-môđun M đều trùng nhau; đó là cận trên bé nhất của tập hợp các độ dài của những chuỗi $p_0 \subset ... \subset p_n$ các iđêan nguyên tố của A sao cho $\alpha \subset p_0$. Theo prop. 6, c) của n° 3, chiều của M cũng là cận trên bé nhất của các chiều của các vành (hay của các A-môđun) A/p, trong đó p chạy trên tập hợp các iđêan nguyên tố của A cực tiểu trong số những iđêan chứa α.

#### Nhận xét 1 {#ac-viii-s1-n4-rem-1 .statement}

Cho A là một vành Noether và M là một A-môđun hữu hạn sinh. Việc nói rằng $\dim_A(M) \leq 0$, hay rằng các phần tử của Supp(M) là các iđêan cực đại của A, hay rằng M có độ dài hữu hạn, là tương đương (IV, § 2, n° 5, prop. 7).

#### Nhận xét 2 {#ac-viii-s1-n4-rem-2 .statement}

Nếu M là một môđun hữu hạn sinh trên một vành Noether A, thì $\dim_A(M)$ là cận trên bé nhất của các số $\dim(A/p)$, trong đó p chạy trên tập $\operatorname{Ass}_A(M)$ các iđêan nguyên tố của A liên kết với M (IV, § 1, n° 4, th. 2).

1 Nếu A là một trường, chiều Krull của M là $\leq 0$. Cần chú ý không được nhầm chiều Krull của M với chiều (hay hạng) của không gian vectơ M trên trường A (A, II, p. 97, déf. 1).

#### Mệnh đề 9 {#ac-viii-s1-prop-9 .statement}

Cho $A$ là một vành và $M$ là một $A$-môđun hữu hạn sinh.

a) Với mọi $p \in \mathrm{Supp}(M)$, ta có $\dim_{A_p}(M_p) = \mathrm{codim}(V(p), \mathrm{Supp}(M))$.

b) $\dim_A(M)$ là cận trên bé nhất của các $\dim_{A_p}(M_p)$, trong đó $p$ chạy trên $\mathrm{Spec}(A)$ (tương ứng, trong đó $p$ chạy trên tập hợp các iđêan cực đại của $A$ thuộc $\mathrm{Supp}(M)$).

c) Cho $M'$ là một môđun con hữu hạn sinh của $M$; khi đó

$$
\dim_A(M) = \sup(\dim_A(M'), \dim_A(M/M')) .
$$

a) Cho $a$ là linh hóa tử của $M$; khi đó linh hóa tử của $A_p$-môđun $M_p$ là $aA_p$ (II, § 2, n° 4, formule (9)), do đó $\dim_{A_p}(M_p) = \dim(A_p/aA_p)$. Kết luận suy ra từ prop. 7, b) của n° 3.

b) Điều này suy ra ngay từ a) và từ sự kiện rằng $\dim_{A_p}(M_p) = -\infty$ nếu $p$ không thuộc $\mathrm{Supp}(M)$.

c) Ta có $\mathrm{Supp}(M) = \mathrm{Supp}(M') \cup \mathrm{Supp}(M/M')$ (II, § 4, n° 4, prop. 16), và ta áp dụng prop. 1 của n° 1.

#### Nhận xét 3 {#ac-viii-s1-n4-rem-3 .statement}

Trong các điều kiện của prop. 9, c), ta có $\mathrm{codim}(\mathrm{Supp}(M), \mathrm{Spec}(A)) = \inf(\mathrm{codim}(\mathrm{Supp}(M'), \mathrm{Spec}(A)), \mathrm{codim}(\mathrm{Supp}(M/M'), \mathrm{Spec}(A)))$. Điều này suy ra từ công thức $\mathrm{Supp}(M) = \mathrm{Supp}(M') \cup \mathrm{Supp}(M/M')$ và từ nhận xét 4 của n° 2.

### 5. Các chu trình liên kết với một môđun

Trong số này, $A$ ký hiệu một vành Noether.

Cho $Z(A)$ là $\mathbf{Z}$-môđun tự do có cơ sở là tập hợp các tập con đóng bất khả quy của $\mathrm{Spec}(A)$; với mọi tập con đóng bất khả quy $Y$ của $\mathrm{Spec}(A)$, ký hiệu $[Y]$ là phần tử tương ứng của $Z(A)$. Các phần tử của $Z(A)$ đôi khi được gọi là các chu trình.

Cho $M$ là một $A$-môđun hữu hạn sinh. Với mọi iđêan nguyên tố $p$ của $A$ là một phần tử cực tiểu của $\mathrm{Supp}(M)$, ta có $0 < \mathrm{long}_{A_p}(M_p) < \infty$ (IV, § 2, n° 5, cor. 2 à la prop. 7 and § 1, n° 4, th. 2); ta đặt

$$
z(M) = \sum_p \mathrm{long}_{A_p}(M_p).[V(p)] ,
$$

trong đó $p$ chạy trên tập hữu hạn các iđêan nguyên tố cực tiểu của $\mathrm{Supp}(M)$.

#### Nhận xét {#ac-viii-s1-n5-rem-1 .statement}

Với mọi $p \in \mathrm{Spec}(A)$, ta có $z(A/p) = [V(p)]$. Nói chung hơn, cho $M$ là một $A$-môđun sinh hữu hạn, và $(M_i)_{0 \leq i \leq n}$ là một dãy hợp thành của $M$ sao cho với $0 \leq i \leq n-1$, môđun $M_i/M_{i+1}$ đẳng cấu với $A/p_i$, trong đó $p_i$ là một iđêan nguyên tố của $A$ (xem IV, § 1, No. 4, Định lý 1); khi đó ta có $z(M) = \sum_{i \in J} [V(p_i)]$, trong đó $J$ là tập con của $I$ gồm các $i$ sao cho $p_i$ là một phần tử cực tiểu của $\{ p_0, ..., p_{n-1} \}$ (IV, § 1, No. 4, Định lý 2 và § 2, No. 5, Nhận xét 1).

Với mọi số nguyên $d$, ta ký hiệu bởi $Z_{\leq d}$ (resp. $Z_d$, resp. $Z^{>d}$, resp. $Z^d$) môđun con trên $\mathbf{Z}$ của $Z(A)$ sinh bởi các phần tử $[V(p)]$ trong đó $p$ là một iđêan nguyên tố của $A$ sao cho $\dim(A/p) \leq d$ (resp. $\dim(A/p) = d$, resp. $\mathrm{ht}(p) \geq d$, resp. $\mathrm{ht}(p) = d$). Các phần tử của $Z_d$ (resp. $Z^d$) được gọi là các chu trình có chiều $d$ (resp. có đối chiều $d$). Hiển nhiên ta có
$$
Z_{\leq d} = Z_{\leq d-1} \oplus Z_d,\quad Z^{>d} = Z^{>d+1} \oplus Z^d.
$$
Hơn nữa, cho $C$ là tập hợp các lớp của các $A$-môđun sinh hữu hạn (A, VIII, § 3, No. 5), và với mỗi số nguyên $d$, cho $C_{\leq d}$ (resp. $C^{>d}$) là tập con của $C$ gồm các lớp của các $A$-môđun sinh hữu hạn có chiều $\leq d$ (resp. có giá đỡ là đối chiều $\geq d$ trong $\mathrm{Spec}(A)$).

#### Bổ đề 1 {#ac-viii-s1-lem-1 .statement}

*Cho $M$ là một $A$-môđun hữu hạn sinh và $d$ là một số nguyên.*
  *a*) *Để $M$ thuộc kiểu $C_{\leq d}$, điều kiện cần và đủ là $z(M) \in Z_{\leq d}$; khi đó phép chiếu $z_d(M)$ của $z(M)$ lên $Z_d$ song song với $Z_{\leq d-1}$ được cho bởi*
$$
z_d(M) = \sum_{\dim(A/p) = d} \mathrm{long}_{A_p}(M_p).[V(p)].
$$
  *b*) *Để $M$ thuộc kiểu $C^{>d}$, điều kiện cần và đủ là $z(M) \in Z^{>d}$; khi đó phép chiếu $z^d(M)$ của $z(M)$ lên $Z^d$ song song với $Z^{>d+1}$ được cho bởi*
$$
z^d(M) = \sum_{\mathrm{ht}(p) = d} \mathrm{long}_{A_p}(M_p).[V(p)].
$$

Để $M$ thuộc kiểu $C_{\leq d}$, nghĩa là có chiều $\leq d$, điều kiện cần và đủ là với mọi iđêan nguyên tố cực tiểu $p$ của $\mathrm{Supp}(M)$, ta có $\dim(A/p) \leq d$, điều đó có nghĩa là $z(M) \in Z_{\leq d}$. Giả sử ta có $\dim(M) \leq d$, và cho $p \in \mathrm{Spec}(A)$ sao cho $\dim(A/p) = d$; khi đó либо $p \notin \mathrm{Supp}(M)$ và do đó $M_p = 0$, hoặc $p \in \mathrm{Supp}(M)$, và $p$ là một phần tử cực tiểu của $\mathrm{Supp}(M)$; trong cả hai trường hợp hệ số của $[V(p)]$ trong $z(M)$ là $\mathrm{long}_{A_p}(M_p)$, do đó *a)*. Phần *b)* được chứng minh tương tự; cần lưu ý rằng một môđun hữu hạn sinh $M$ thuộc kiểu $C^{>d}$ khi và chỉ khi ta có $M_p = 0$ với mọi iđêan nguyên tố $p$ có chiều cao $< d$.

Theo Mệnh đề 9, *c)* và Nhận xét 3 của No. 4, các tập hợp $C_{\leq d}$ và $C^{>d}$ là di truyền (A, VIII, § 10, No. 1, Định nghĩa 1), và ta có thể xét các nhóm Grothendieck tương ứng $K(C_{\leq d})$ và $K(C^{>d})$ (*loc. cit.*, No. 2); với mọi $A$-môđun $M$ thuộc kiểu $C_{\leq d}$ (resp. $C^{>d}$), ký hiệu $[M]_{\leq d}$ (resp. $[M]^{>d}$) phần tử liên kết trong $K(C_{\leq d})$ (resp. $K(C^{>d})$). Theo Bổ đề 1, các ánh xạ $z_d$ và $z^d$ là cộng tính; do đó tồn tại (*loc. cit.*, Mệnh đề 3) các đồng cấu
$$
\zeta_d : K(C_{\leq d}) \to Z_d,\quad \zeta^d : K(C^{>d}) \to Z^d
$$
sao cho $\zeta_d([M]_{\leq d}) = z_d(M)$ với mọi $A$-môđun $M$ thuộc kiểu $C_{\leq d}$ và $\zeta^d([N]^{>d}) = z^d(N)$ với mọi $A$-môđun $N$ thuộc kiểu $C^{>d}$. Hơn nữa, vì $C_{\leq d-1} \subset C_{\leq d}$ và $C^{>d+1} \subset C^{>d}$, ta có các đồng cấu chính tắc
$$
i_d : K(C_{\leq d-1}) \to K(C_{\leq d})\quad \text{và}\quad i^d : K(C^{>d+1}) \to K(C^{>d}).
$$
Với các ký hiệu này:

#### Mệnh đề 10 {#ac-viii-s1-prop-10 .statement}

Các dãy $\mathbf{Z}$-môđun và đồng cấu

$$
\begin{array}{cccccc}
K(\mathcal{C}_{\leq d-1}) & \xrightarrow{i_d} & K(\mathcal{C}_{\leq d}) & \xrightarrow{\zeta_d} & Z_d & \longrightarrow 0 \\
K(\mathcal{C}^{>d+1}) & \xrightarrow{i_d} & K(\mathcal{C}^{>d}) & \xrightarrow{\zeta_d} & Z^d & \longrightarrow 0
\end{array}
$$

là khớp.

Ta có $\zeta_d \circ i_d = 0$ theo Bổ đề 1. Với mọi $p \in \mathrm{Spec}(A)$ sao cho $\dim(A/p) = d$, ta có $\zeta_d([A/p]_{\leq d}) = z_d(A/p) = [V(p)]$, do đó đồng cấu $\zeta_d$ là toàn ánh. Theo IV, § 1, No. 4, Định lý 1, $K(\mathcal{C}_{\leq d})$ được sinh bởi các $[A/p]_{\leq d}$, trong đó $p \in \mathrm{Spec}(A)$ và $\dim(A/p) \leq d$; do đó, mọi phần tử $\xi$ của $K(\mathcal{C}_{\leq d})$ đều có thể viết được dưới dạng $\xi = i_d(\eta) + \sum_{i=1}^k n_i[A/p_i]_{\leq d}$, với $\eta \in K(\mathcal{C}_{\leq d-1})$, $n_i \in \mathbf{Z}$ và $\dim(A/p_i) = d$ với $1 \leq i \leq k$; ta có $\zeta_d(\xi) = \sum_{i=1}^k n_i[V(p_i)]$ và do đó $\zeta_d(\xi) = 0$ kéo theo $\xi = i_d(\eta) \in \mathrm{Im}(i_d)$, suy ra $\mathrm{Ker}(\zeta_d) = \mathrm{Im}(i_d)$.

Ta lập luận tương tự cho dãy thứ hai.

#### Ví dụ 1 {#ac-viii-s1-n5-exa-1 .statement}

Giả sử A là Noether và nguyên. Khi đó ta có $Z^0 = \mathbf{Z}.[\mathrm{Spec}(A)]$; ta có $\mathcal{C}^{>0} = \mathcal{C}$ và $z^0(M) = \mathrm{rg}(M).[Spec(A)]$. Do đó các môđun thuộc kiểu $\mathcal{C}^{>1}$ là các môđun xoắn.

#### Ví dụ 2 {#ac-viii-s1-n5-exa-2 .statement}

Giả sử A là Noether và đóng nguyên. Khi đó $Z^1$ được đồng nhất với nhóm $D(A)$ các ước tử của A được đưa vào trong Chương VII (§ 1, No. 3, Định lý 2, và No. 6, Định lý 3). Các môđun thuộc kiểu $\mathcal{C}^{>2}$ là các môđun giả-không (VII, § 4, No. 4, Định nghĩa 2); nếu M là một môđun xoắn kiểu hữu hạn, thì $z^1(M) \in Z^1 = D(A)$ là nội dung $\chi(M)$ của M (VII, § 4, No. 5, Định nghĩa 4). Do đó các Mệnh đề 10 và 11 của *loc. cit.* tương đương với tính khớp của dãy $K(\mathcal{C}^{>2}) \to K(\mathcal{C}^{>1}) \to Z^1 \to 0$.

#### Ví dụ 3 {#ac-viii-s1-n5-exa-3 .statement}

Các môđun kiểu $\mathcal{C}_{\leq 0}$ là các môđun có chiều $\leq 0$, nghĩa là các môđun có độ dài hữu hạn (No. 4, Nhận xét 1). Ta có $\mathrm{long}_A(M) = \varepsilon(z_0(M))$ với mọi A-môđun M có độ dài hữu hạn, trong đó $\varepsilon : Z_0 \to \mathbf{Z}$ gán cho tổ hợp tuyến tính $\sum_m n_m[V(m)]$ số nguyên $\sum_m n_m$ (IV, § 2, No. 5, hệ quả của Mệnh đề 8).

#### Ví dụ 4 {#ac-viii-s1-n5-exa-4 .statement}

Giả sử A là một miền nguyên và hữu hạn chiều. Đặt $d = \dim(A)$. Khi đó ta có $\mathcal{C}_{\leq d} = \mathcal{C}$, $Z_d = \mathbf{Z}.[\mathrm{Spec}(A)] = Z^0$, $z_d(M) = \mathrm{rg}(M).[Spec(A)] = z^0(M)$, và các môđun kiểu $\mathcal{C}_{\leq d-1}$ là các môđun xoắn.

## BÀI TẬP {#ac-viii-s1-exercises}

Xem [bài tập của § 1](exercises/s1/).
