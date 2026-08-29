---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 15
section_title: Separable extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.118-A V.126, A V.175-A V.177
pdf_pages: 0232-0240, 0289-0291
extraction: ocr
subsections:
    - "no": 1
      title: Characterization of the nilpotent elements of a ring
      page: 118
      pdf_page: 232
    - "no": 2
      title: Separable algebras
      page: 119
      pdf_page: 233
    - "no": 3
      title: Separable extensions
      page: 121
      pdf_page: 235
    - "no": 4
      title: Mac Lane's separability criterion
      page: 122
      pdf_page: 236
    - "no": 5
      title: Extensions of a perfect field
      page: 125
      pdf_page: 239
    - "no": 6
      title: The characterization of separability by automorphisms
      page: 125
      pdf_page: 239
statements: 21
exercises: 12
content_sha256: 02e6dd31d2fc0304c2d4f506648bfb0babb58cbab337bfa44f53b7b9611c9102
translated_from: content/en/alg/V/15_s15_separable_extensions.md
source_content_sha256: cd3cc2bd76e6784392d91069b887e2344baeedd432fedf2725695282c5095d73
translation_model: gpt-5.4
translation_run: translate-vi-7c87708d
glossary_version: 34
glossary_terms_sha256: 7b799be992568e8a07853ef472611368f6cee4e0f379d2a0ce3e46fbaeed3c2e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 15. MỞ RỘNG TÁCH ĐƯỢC

### 1. Đặc trưng hóa các phần tử lũy linh của một vành

#### Mệnh đề 1 {#alg-v-s15-prop-1 .statement}

— *Cho A là một vành giao hoán và x là một phần tử của A. Để x là lũy linh thì điều kiện cần và đủ là $1 - xT$ khả nghịch trong vành $A[T]$.*

Ta chú ý rằng $A[T]$ là một vành con của vành các chuỗi lũy thừa hình thức $A[[T]]$ và $1 - xT$ có trong $A[[T]]$ nghịch đảo là $\sum_{n=0}^{\infty} x^n T^n$ (IV, p. 30, Mệnh đề 5). Để $1 - xT$ khả nghịch trong $A[T]$ thì điều kiện cần và đủ là $\sum_{n=0}^{\infty} x^n T^n$ là một đa thức, nghĩa là x là lũy linh.

#### Mệnh đề 2 {#alg-v-s15-prop-2 .statement}

— *Cho A là một vành giao hoán. Tập hợp các phần tử lũy linh của A là một iđêan của A, bằng giao của tập hợp mọi iđêan nguyên tố của A.*

Cho x là một phần tử lũy linh của A và p là một iđêan nguyên tố. Lớp thặng dư của $x \mod p$ là một phần tử lũy linh của miền nguyên $A/p$, do đó bằng không; vậy ta có $x \in p$.

Cho x là một phần tử không lũy linh của A. Theo Mệnh đề 1, iđêan chính $(1 - xT)$ của $A[T]$ phân biệt với $A[T]$. Theo định lý Krull (I, p. 104), tồn tại một iđêan cực đại m của $A[T]$ chứa $1 - xT$. Khi đó m là một iđêan nguyên tố của $A[T]$, do đó $p = A \cap m$ là một iđêan nguyên tố của A. Ta có $1 \notin m$ và $1 - Tx \in m$, do đó $Tx \notin m$ và *a fortiori* $x \notin p$.

Vậy ta đã chứng tỏ rằng tập hợp $\mathfrak{n}$ các phần tử lũy linh của A là giao của tập hợp tất cả các iđêan nguyên tố của A; vì mọi giao của các iđêan đều là một iđêan, nên $\mathfrak{n}$ là một iđêan.

#### Hệ quả {#alg-v-s15-n1-cor-1 .statement}

— *Để một vành giao hoán là rút gọn* (*V*, p. 34, Định nghĩa 2) *thì điều kiện cần và đủ là nó đẳng cấu với một vành con của một tích các trường*.

Điều kiện ấy rõ ràng là đủ.

Cho $\mathbf{A}$ là thu gọn. Theo Mệnh đề 2, giao $n$ của tập hợp các iđêan nguyên tố của $\mathbf{A}$ thu về 0. Với mọi iđêan nguyên tố $\mathfrak{p}$ của $\mathbf{A}$, gọi $k(\mathfrak{p})$ là trường phân thức của $\mathbf{A}/\mathfrak{p}$ và $\varphi_n$ là đồng cấu chính tắc của $\mathbf{A}$ vào $k(\mathfrak{p})$. Gọi $\varphi$ là đồng cấu của $\mathbf{A}$ vào $\prod_{\mathfrak{p}} k(\mathfrak{p})$ mà thành phần có chỉ số $\mathfrak{p}$ là $\varphi_{\mathfrak{p}}$. Hạt nhân của $\varphi_{\mathfrak{p}}$ là $\mathfrak{p}$, do đó hạt nhân của $\varphi$ là $n = 0$; vì thế $\varphi$ là một đẳng cấu của $\mathbf{A}$ lên một vành con của $\prod_{\mathfrak{p}} k(\mathfrak{p})$.

### 2. Các đại số tách được

#### Định nghĩa 1 {#alg-v-s15-def-1 .statement}

*Cho $\mathbf{A}$ là một đại số giao hoán trên một trường $K$. Khi đó $A$ được gọi là tách được trên $K$, hay cũng là một $K$-đại số tách được nếu vành $L \otimes_K \mathbf{A}$ là rút gọn đối với mọi mở rộng $L$ của $K$*.

Mọi đại số tách được đều rõ ràng là rút gọn. Về một đảo lại bộ phận, xem Định lý 3 (*V*, p. 125).

*Ví dụ. — 1*) Cho $\mathbf{A}$ là một đại số đa thức $K[X_i]_{i \in I}$. Với mọi mở rộng $L$ của $K$, vành $L \otimes_K \mathbf{A}$ đẳng cấu với $L[X_i]_{i \in I}$ (III, p. 449, Nhận xét 2) và do đó là một miền nguyên (*IV*, p. 9, Mệnh đề 8). Nói cách khác, mọi đại số đa thức trên một trường $K$ đều là một $K$-đại số tách được.

2) Cho $\mathbf{A}$ là một đại số giao hoán bậc hữu hạn trên một trường $K$. Để $\mathbf{A}$ tách được thì điều kiện cần và đủ là nó étale (*V*, p. 34, Định lý 4).

3) Cho $E$ là một mở rộng đại số của một trường $K$. Nếu $L$ là một mở rộng của $K$, thì vành $L \otimes_K E$ là hợp của các vành con $L \otimes_K F$ khi $F$ chạy qua tập hợp tất cả các mở rộng con bậc hữu hạn của $E$; do đó vành $L \otimes_K E$ là rút gọn nếu và chỉ nếu điều này đúng với $L \otimes_K F$ đối với mọi mở rộng con $F$ của $E$, có bậc hữu hạn trên $K$. Có tính đến Ví dụ 2, ta thấy rằng $E$ là một đại số tách được theo nghĩa của Định nghĩa 1 ở trên nếu và chỉ nếu nó là một mở rộng đại số tách được theo nghĩa của Định nghĩa 1 của *V*, p. 36.

#### Mệnh đề 3 {#alg-v-s15-prop-3 .statement}

*Cho $K$ là một trường*.

a) *Mọi đại số con của một $K$-đại số tách được đều tách được*.

b) *Mọi giới hạn trực tiếp của các $K$-đại số tách được đều tách được*.

c) *Mọi tích của các $K$-đại số tách được đều tách được*.

d) *Cho $\mathbf{A}$ là một $K$-đại số và $K'$ là một mở rộng của $K$. Để $\mathbf{A}$ tách được thì điều kiện cần và đủ là $K'$-đại số $\mathbf{A}_{(K')}$ thu được từ $\mathbf{A}$ bằng phép mở rộng vô hướng là tách được*.

Cho $L$ là một mở rộng của $K$. Cho $\mathbf{A}$ là một đại số tách được trên $K$ và $B$ là một đại số con của $\mathbf{A}$; khi đó vành $L \otimes_K \mathbf{A}$ là rút gọn, và $L \otimes_K B$ đẳng cấu với một vành con của $L \otimes_K \mathbf{A}$, nên là rút gọn. Vậy $B$ là tách được và *a)* được chứng minh. *Theo* cùng cách đó, có thể chứng minh $b$), bằng cách dùng đẳng cấu chính tắc của $L \otimes_K \varprojlim A_i$ với $\varprojlim L \otimes_K A_i$ (II, p. 290, Prop. 7), và $c$) được chứng minh bằng cách nhận thấy rằng $L \otimes_K \left( \prod_{i \in I} A_i \right)$ đẳng cấu với một vành con của $\prod_{i \in I} (L \otimes_K A_i)$ (II, p. 306, Prop. 15).

Chúng ta sẽ dùng ký hiệu của $d$). Với mọi mở rộng $L'$ của $K'$, các vành $L' \otimes_{K'} A_{(K')}$ và $L' \otimes_K A$ là đẳng cấu (II, p. 278, Prop. 2). Ta kết luận rằng nếu $A$ là một $K$-đại số tách được, thì $A_{(K')}$ là một $K'$-đại số tách được. Ngược lại, giả sử rằng $A_{(K')}$ là một $K'$-đại số tách được; nhận xét trước cho thấy rằng $L' \otimes_K A$ là rút gọn với mọi mở rộng $L'$ của $K$ chứa $K'$ như một mở rộng con. Cho $L$ là một mở rộng của $K$; theo Chú giải (V, p. 13) tồn tại một mở rộng $L'$ của $K$ chứa $K'$ như một mở rộng con và một $K$-đồng cấu từ $L$ vào $L'$; do đó vành $L \otimes_K A$ đẳng cấu với một vành con của $L' \otimes_K A$ và vì thế là rút gọn. Điều này chứng minh rằng $A$ là một $K$-đại số tách được.

#### Mệnh đề 4 {#alg-v-s15-prop-4 .statement}

— *Cho $A$ là một đại số tách được trên một trường $K$ và cho $B$ là vành phân thức toàn phần của $A$; khi đó $K$-đại số $B$ là tách được.*

Gọi $S$ là tập hợp các phần tử giản ước được của $A$. Ta đã đồng nhất $A$ với một vành con của $B$ (I, p. 113); hơn nữa, mọi phần tử của $S$ đều khả nghịch trong $B$ và mọi phần tử của $B$ đều có dạng $a s^{-1}$ với $a \in A$ và $s \in S$. Cho $L$ là một mở rộng của $K$ và $x$ là một phần tử lũy linh của $L \otimes_K B$. Khi đó $x$ có thể được viết dưới dạng
$$
x = \sum_{i=1}^n y_i \otimes a_i s_i^{-1}
$$
với $y_i \in L, a_i \in A, s_i \in S$ đối với $1 \leq i \leq n$. Nếu ta đặt $s = s_1 \ldots s_n$
thì $x(1 \otimes s)$ thuộc vành con $L \otimes_K A$ của $L \otimes_K B$; vì $x(1 \otimes s)$ là lũy linh và $A$ tách được trên $K$, ta có $x(1 \otimes s) = 0$, và vì $s$ khả nghịch trong $B$ nên do đó suy ra $x = 0$. Điều này chứng minh rằng vành $L \otimes_K B$ là rút gọn, do đó suy ra mệnh đề.

#### Mệnh đề 5 {#alg-v-s15-prop-5 .statement}

— *Cho $K$ là một trường và $A, B$ là các $K$-đại số giao hoán. Nếu $A$ là rút gọn và $B$ tách được thì $A \otimes_K B$ là rút gọn.*

Theo Hệ quả của Mệnh đề 2 (V, p. 119) $A$ đẳng cấu với một đại số con của một tích $\prod_{i \in I} L_i$ trong đó $L_i$ là một mở rộng của $K$ với $i \in I$. Do đó $A \otimes_K B$ đẳng cấu với một vành con của $\left( \prod_{i \in I} L_i \right) \otimes_K B$ và vành sau này đẳng cấu với một vành con của $\prod_{i \in I} (L_i \otimes_K B)$ (II, p. 306, Mệnh đề 15). Vì $B$ tách được, mỗi vành $L_i \otimes_K B$ đều là rút gọn, và do đó $\prod_{i \in I} (L_i \otimes_K B)$ cũng vậy, và *a fortiori* $A \otimes_K B$ cũng vậy.

#### Hệ quả 1 {#alg-v-s15-prop-5-cor-1 .statement}

— *Cho $K$ là một trường, $L$ là một mở rộng tách được của $K$ và $f$ là một đa thức trong $K[X]$. Nếu $f$ không có nhân tử bội trong $K[X]$, thì nó cũng không có nhân tử bội trong $L[X]$.*

Nếu $f$ không có nhân tử bội trong $K[X]$, vành thương $K[X]/(f)$ là thu gọn; thật vậy, $f$ là tích của các đa thức bất khả quy $f_i$ nguyên tố cùng nhau từng đôi một, nên

K[X]/(f) đẳng cấu, theo I, p. 110, Prop. 9, với tích của các trường K[X]/(f_i). Theo Mệnh đề 5, vành L[X]/(f), đẳng cấu với L ⊗_K K[X]/(f ), là thu gọn; nếu g là một đa thức không hằng của L[X] sao cho g^2 chia hết f, thì lớp thặng dư của fg^{-1} trong L[X]/(f) là một phần tử lũy linh khác không; do đó f không có nhân tử bội trong L[X].

#### Hệ quả 2 {#alg-v-s15-prop-5-cor-2 .statement}

— Cho A và B là hai đại số giao hoán trên K. *Nếu* A và B tách được, thì A ⊗_K B cũng vậy.

Cho L là một mở rộng của K. Vành L ⊗_K A là thu gọn vì A tách được; bây giờ Mệnh đề 5 cho thấy vành (L ⊗_K A) ⊗_K B (đẳng cấu với L ⊗_K (A ⊗_K B)) là thu gọn, do đó suy ra Hệ quả.

### 3. Mở rộng tách được

Cho K là một trường. Vì mọi mở rộng của K đều là một đại số trên K, khái niệm tính tách được đưa vào trong Định nghĩa 1 (V, p. 119) áp dụng đặc biệt cho trường hợp các mở rộng của K. Theo ví dụ 3 (V, p. 119), định nghĩa ấy về tính tách được trùng, trong trường hợp các mở rộng đại số, với định nghĩa ở § 7 (V, p. 36, Định nghĩa 1).

#### Mệnh đề 6 {#alg-v-s15-prop-6 .statement}

— Mọi mở rộng thuần của một *trường* K đều tách được.
Điều này suy ra ngay từ Ví dụ 1 (V, p. 119) và Mệnh đề 4 (V, p. 120).

#### Mệnh đề 7 {#alg-v-s15-prop-7 .statement}

— Cho E là một trường, G là một nhóm các *tự đẳng cấu* của E và K là *trường con* của E gồm các phần tử bất biến của G. Khi đó E là một mở rộng tách được của K.

Cho L là một mở rộng của K; tồn tại một mở rộng đóng đại số Ω của L mà bậc siêu việt trên K ít nhất bằng bậc siêu việt của E trên K. Theo Hệ quả 1 (V, p. 117) tồn tại một K-đồng cấu u của E vào R. Ta ký hiệu bởi v đồng cấu đại số trên Ω của A = Ω ⊗_K E vào Ω ánh xạ λ ⊗ x thành λ . u(x) với λ ∈ Ω và x ∈ Ω; ta viết a cho hạt nhân của v.

Với mỗi s ∈ G, cho h_s là tự đẳng cấu Id, ⊗ s của 0-đại số A; hạt nhân của đồng cấu v ∘ h_s từ A vào Ω là iđêan nguyên tố a_s = h_s^{-1}(a) của A. Rõ ràng iđêan b = ⋂_{s ∈ G} a_s của A là ổn định dưới các tự đẳng cấu h_s. Vì thế (V, p. 63, Hệ quả) iđêan b có dạng c ⊗_K E, trong đó c là một iđêan của Ω. Bây giờ b ⊂ a ≠ A, nên c ≠ Ω; vì Ω là một trường, ta có c = 0, do đó b = 0.

Vậy họ các iđêan nguyên tố (a_s), _s ∈ G của A có giao bằng không. Theo Mệnh đề 2 (V, p. 118) vành A là thu gọn, và a fortiori điều này cũng đúng với vành con L ⊗_K E của A. Vì L là một mở rộng tùy ý của K, điều đó chứng tỏ rằng E tách được trên K.

#### Mệnh đề 8 {#alg-v-s15-prop-8 .statement}

— Cho L là một mở rộng của một trường K. Nếu L tách được trên K, thì mọi mở rộng con của L đều tách được trên K. Ngược lại, nếu mọi mở rộng con sinh hữu hạn của L đều tách được trên K, thì L tách được trên K.

Điều này suy ra ngay từ Mệnh đề 3, a) và b) (V, p. 119).

Vì vậy tính tách được có thể được gọi là một tính chất « đặc trưng hữu hạn ».

#### Mệnh đề 9 {#alg-v-s15-prop-9 .statement}

— Cho L là một mở rộng của một trường K và M là một đại số giao hoán trên L (chẳng hạn, một mở rộng của L). Nếu M tách được trên L và L tách được trên K, thì M tách được trên K.

Cho K' là một mở rộng của K. Vì L là một mở rộng tách được của K, vành $K' \otimes_K L$ là rút gọn; vì M là một đại số trên L tách được, Mệnh đề 5 (V, p. 120) cho thấy vành $(K' \otimes_K L) \otimes_L M$ là rút gọn. Bây giờ vành $K' \otimes_K M$ đẳng cấu với $(K' \otimes_K L) \otimes_L M$ (II, p. 278, Mệnh đề 2), nên là rút gọn. Điều này chứng tỏ rằng M tách được trên K.

Nếu mở rộng M tách được trên K, thì không nhất thiết tách được trên L (xem tuy nhiên V, p. 124, Hệ quả 3). Chẳng hạn, nếu p là một số nguyên tố, trường $F_p(X)$ các phân thức hữu tỉ theo một bất định X trên $F_p$ là tách được trên $F_p$ (V, p. 121, Mệnh đề 6) nhưng nó là một mở rộng đại số căn-p của $F_p(X^p)$; đặc biệt $F_p(X)$ không tách được trên $F_p(X^p)$.

Sau này (V, p. 137 Mệnh đề 5) chúng ta sẽ nghiên cứu tính tách được của các mở rộng hợp thành.

### 4. Tiêu chuẩn tách được của Mac Lane

#### Định lý 1 {#alg-v-s15-thm-1 .statement}

— Cho K là một trường có đặc số 0. Mọi đại số trên K rút gọn, và đặc biệt mọi mở rộng của K, đều tách được trên K.

Trước hết ta chứng minh rằng mọi mở rộng L của K đều tách được. Gọi B là một cơ sở siêu việt của L trên K (V, p. 109, Định lý 1) và đặt $L_1 = K(B)$. Khi đó $L_1$ tách được trên K (V, p. 121, Mệnh đề 6). Hơn nữa, L là một mở rộng đại số của $L_1$ và $L_1$ là một trường có đặc số 0; do đó L tách được trên $L_1$ (V, p. 37, Hệ quả). Theo Mệnh đề 9, suy ra L tách được trên K.

Bây giờ giả sử A là một đại số rút gọn trên trường K. Theo Hệ quả của Mệnh đề 2 (V, p. 119), tồn tại một họ $(L_i)_{i \in I}$ các mở rộng của K sao cho A đẳng cấu với một đại số con của $\prod_{i \in I} L_i$. Mỗi đại số $L_i$ đều tách được trên K theo điều đã nói ở trên, nên A cũng có cùng tính chất đó, theo Mệnh đề 3 a) và c) (V, p. 119).

#### Định lý 2 {#alg-v-s15-thm-2 .statement}

— Cho K là một trường có đặc số $p \neq 0$, $K^{p^{-\infty}}$ là một bao đóng hoàn hảo của K và A là một đại số giao hoán trên K. Các tính chất sau là tương đương:
a) A là tách được.
b) Tồn tại một mở rộng K' của K sao cho K' là hoàn hảo và $K' \otimes_K A$ là rút gọn.
c) Vành $K^{p^{-\infty}} \otimes_K A$ là rút gọn.

d) *Vành* $K' \otimes_K A$ *là rút gọn đối với mọi mở rộng* $K'$ *của* $K$ *có bậc hữu hạn và* $p$*-căn với chiều cao* $\leqslant 1$.

e) *Với mọi họ* $(a_i)_{i \in I}$, *các phần tử của* $A$ *tự do tuyến tính trên* $K$, *họ* $(a_i^p)_{i \in I}$, *tự do tuyến tính trên* $K$.

f) *Tồn tại một cơ sở* $(a_i)_{i \in I}$, *của không gian vectơ* $K$*-*không gian $A$ *sao cho họ* $(a_i^p)_{i \in I}$, *tự do tuyến tính trên* $K$.

Nếu một mở rộng $K'$ của $K$ là một trường hoàn hảo, thì nó chứa một mở rộng con $K$-đẳng cấu với $K^{p^{-\infty}}$ ($V$, p. 6, Prop. 3); hơn nữa, mọi mở rộng căn theo $p$ của $K$ đều đẳng cấu với một mở rộng con của $K^{p^{-\infty}}$ ($V$, p. 26, Prop. 3). Những nhận xét này cho thấy các suy ra $a) \Rightarrow b) \Rightarrow c) \Rightarrow d)$.

Ta hãy chứng minh rằng d) suy ra e). Cho $(a_i)_{i \in I}$, là một họ tự do tuyến tính trong $A$ và cho $(A_i)_{i \in I}$, là một họ giá hữu hạn trong $K$ sao cho $\sum \lambda_i a_i^p = 0$. Gọi $K'$ là mở rộng con của $K^{p^{-\infty}}$ sinh bởi các phần tử $\lambda_i^{p^{-1}}$; nó có bậc hữu hạn và chiều cao $\leqslant 1$. Đặt $x = \sum_{i \in I} \lambda_i^{p^{-1}} \otimes a_i$ trong $K' \otimes_K A$; ta có

$$
x^p = \sum_{i \in I} \lambda_i \otimes a_i^p = 1 \otimes \sum_{i \in I} \lambda_i a_i^p = 0
$$

Theo giả thiết d) ta có $x = 0$, do đó $A_i = 0$ với mọi $i \in I$.

Rõ ràng e) suy ra f) và còn lại phải chỉ ra rằng f) suy ra a). Vậy cho $(a_i)_{i \in I}$ là một cơ sở của $A$ trên $K$ sao cho họ $(a_i^p)_{i \in I}$ là tự do tuyến tính trên $K$. Gọi $L$ là một mở rộng của $K$ và gọi $x$ là một phần tử của $L \otimes_K A$ sao cho $x^p = 0$. Viết $x = \sum_{i \in I} \lambda_i \otimes a_i$ với $A_i \in L$ với mọi $i \in I$. Ta có $x^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p = 0$ và vì họ $(a_i^p)_{i \in I}$, là tự do tuyến tính trên $K$, nên ta có $\lambda_i^p = 0$, do đó $\lambda_i = 0$ với mọi $i \in I$; suy ra $x = 0$. Vậy ta đã chứng minh rằng $x^p = 0$ suy ra $x = 0$ trong $L \otimes_K A$, từ đó suy ra ngay rằng $L \otimes_K A$ là rút gọn.

#### Hệ quả 1 (Mac Lane) {#alg-v-s15-thm-2-cor-1 .statement}

— *Cho* $K$ *là một trường có số mũ đặc số* $p$, $\Omega$ *là một mở rộng hoàn hảo của* $K$ *và* $L$ *là một mở rộng con của* $\Omega$. *Khi đó các điều kiện sau là tương đương*:

a) $L$ *là tách được trên* $K$.

b) $L$ *rời nhau tuyến tính với* $K^{p^{-\infty}}$ *trên* $K$.

c) $L$ *rời nhau tuyến tính trên* $K$ *với mọi* $p$*-mở rộng căn của* $K$ *được chứa trong* $\Omega$, *có bậc hữu hạn và chiều cao* $\leqslant 1$.

Trường hợp $K$ có đặc số 0 là tầm thường vì khi đó $L$ tách được trên $K$ (Định lý 1) và $K^{p^{-\infty}} = K$ theo quy ước. Vậy giả sử $p \neq 1$, và trước hết hãy chỉ ra rằng a) kéo theo b). Giả sử rằng $L$ tách được trên $K$ và gọi $(a_i)_{i \in I}$, là một cơ sở của $L$ trên $K$. Gọi $(\lambda_i)_{i \in I}$ là một họ có giá hữu hạn các phần tử của $K^{p^{-\infty}}$ sao cho $\sum_{i \in I} \lambda_i a_i = 0$; tồn tại một số nguyên $f \geqslant 0$ và các phần tử μ_i của K sao cho λ_i = μ_i^{p^{-f}}. Ta có

$$
\sum_{i \in I} \mu_i a_i^{p^f} = \left( \sum_{i \in I} \lambda_i a_i \right)^{p^f} = 0
$$

và Định lý 2 suy ra, bằng quy nạp theo f, rằng họ $(a_i^{p^f})_{i \in I}$ là tự do tuyến tính trên K. Do đó ta có $\mu_i = 0$, suy ra $\lambda_i = 0$ với mọi $i \in I$. Cuối cùng L rời nhau tuyến tính với $K^{p^{-\infty}}$ trên K.

Hiển nhiên là b) suy ra c). Sau hết giả sử rằng c) đúng và cho K' là một mở rộng của K có bậc hữu hạn và p-căn có chiều cao $\leq 1$. Vành $K' \otimes_K L$ đẳng cấu với một vành con của $\Omega$, nên là vành thu gọn. Bây giờ từ Định lý 2 suy ra rằng L là tách được trên K.

#### Hệ quả 2 {#alg-v-s15-thm-2-cor-2 .statement}

— *Cho K là một trường có đặc số mũ p, $K^{p^{-\infty}}$ là một bao đóng hoàn hảo của K và L là một mở rộng tách được của K. Khi đó vành $L \otimes_K K^{p^{-\infty}}$ là một trường. Hơn nữa, nếu L là đại số trên K, thì $L \otimes_K K^{p^{-\infty}}$ là một bao đóng hoàn hảo của L.*

Trường hợp $p = 1$ là tầm thường, vậy giả sử $p \neq 1$. Gọi $\Omega$ là một bao đóng hoàn hảo của L. Theo Hệ quả 1, tồn tại một đồng cấu đại số trên K từ $L \otimes_K K^{p^{-\infty}}$ lên $L[K^{p^{-\infty}}]$ ánh xạ $x \otimes y$ thành $xy$ với $x \in L$ và $y \in K^{p^{-\infty}}$. Vì $K^{p^{-\infty}}$ là đại số trên K, vành $L[K^{p^{-\infty}}]$ là một trường con của $\Omega$ (V, p. 18, Hệ quả 1). Giả sử thêm rằng L là đại số trên K, khi đó $L[K^p]$ là một mở rộng đại số của trường hoàn hảo $K^{p^{-\infty}}$, nên nó là một trường hoàn hảo (V, p. 43, Hệ quả 1); sau cùng, vì trường $L[K^{p^{-\infty}}]$ là một mở rộng căn-p của L (V, p. 25, Hệ quả), nó là một bao đóng hoàn hảo của L.

#### Hệ quả 3 {#alg-v-s15-thm-2-cor-3 .statement}

— *Cho L là một mở rộng đại số của K và M là một đại số trên L giao hoán (chẳng hạn một mở rộng của L). Nếu M tách được trên K, thì nó tách được trên L.*

Đại số L đẳng cấu trên K với một đại số con của M, do đó L là một mở rộng tách được của K. Vì vậy (Hệ quả 2) tồn tại một đẳng cấu trên L của $L^{p^{-\infty}}$ lên $K^{p^{-\infty}} \otimes_K L$. Khi đó vành $L^{p^{-\infty}} \otimes_L M$ đẳng cấu với $(K^{p^{-\infty}} \otimes_K L) \otimes_L M$, và do đó đẳng cấu với $K^{p^{-\infty}} \otimes_K M$ (II, p. 278, Mệnh đề 2), và vành sau cùng này là rút gọn vì M tách được trên K. Vậy vành $L^{p^{-\infty}} \otimes_L M$ là rút gọn, điều này chứng tỏ rằng M tách được trên L (V, p. 122, Định lý 2).

#### Nhận xét {#alg-v-s15-n4-rem-1 .statement}

— Tiêu chuẩn của Mac Lane có thể được phát biểu mà không đưa vào bất kỳ mở rộng nào của K ngoài L. Thật vậy, theo c) của Hệ quả 1, L tách được trên K khi và chỉ khi L và $K^P$ rời nhau tuyến tính trên K. Vì ánh xạ $x \mapsto x^p$ là một đẳng cấu của L lên trường con $L^P$, ta thu được tiêu chuẩn sau (xem V, p. 177, Bài tập 11 để có một tiêu chuẩn tương tự đối với các đại số):

*L tách được trên K khi và chỉ khi các trường con $L^P$ và K của L rời nhau tuyến tính trên $K^P$.*

### 5. Các mở rộng của một trường hoàn hảo

Để tiện tra cứu, chúng tôi tóm tắt các tính chất chính của các mở rộng của các trường hoàn hảo:

#### Định lý 3 {#alg-v-s15-thm-3 .statement}

— Cho K là một trường hoàn hảo.
a) Mọi mở rộng đại số của K đều là một trường hoàn hảo.
b) Mọi mở rộng của K đều tách được.
c) Điều kiện cần và đủ để một đại số trên K là tách được là nó rút gọn.
d) Cho A và B là hai đại số trên K rút gọn. Khi đó $A \otimes_K B$ là rút gọn.
e) Nếu E và F là hai mở rộng của K, thì vành $E \otimes_K F$ là rút gọn.

Mệnh đề a) chỉ là Hệ quả 1 của Mệnh đề 11 (V, p. 43).
Mệnh đề b) suy ra từ Định lý 1 (V, p. 122) khi K có đặc số 0 và từ Hệ quả 1 (V, p. 123) khi K có đặc số $p \neq 0$.
Hãy chứng minh c). Trường hợp K có đặc số 0 suy ra từ Định lý 1 (V, p. 122). Vậy chỉ cần chỉ ra rằng nếu K là hoàn hảo có đặc số $p \neq 0$ và A là một đại số trên K rút gọn, thì A tách được trên K. Nhưng điều này suy ra từ tính tương đương của các điều kiện a) và b) của Định lý 2 (V, p. 122; lấy $K' = K$ trong b)).
Cuối cùng, d) suy ra từ c) và Mệnh đề 5 (V, p. 120), còn e) là một trường hợp riêng của d).

### 6. Đặc trưng hóa tính tách được bằng các tự đẳng cấu

#### Định lý 4 {#alg-v-s15-thm-4 .statement}

— Cho $\Omega$ là một mở rộng đóng đại số của một trường K và L là một mở rộng con của $\Omega$. Khi đó các điều kiện sau là tương đương:
a) L tách được trên K.
b) Giao của các hạt nhân của các đồng cấu đại số 0 của $\Omega \otimes_K L$ vào $\Omega$ được thu về 0.
c) Với mọi phần tử $a_1, \ldots, a_n$ của L độc lập tuyến tính trên K, tồn tại các K-tự đẳng cấu $\sigma_1, \ldots, \sigma_n$ của $\Omega$ sao cho $\det(\sigma_i(a_j)) \neq 0$.
d) Gọi V là một không gian vectơ con trên K của L có số chiều hữu hạn. Mọi ánh xạ K-tuyến tính từ V vào $\Omega$ là một tổ hợp tuyến tính (với các hệ số trong R) của các hạn chế trên V của các K-tự đẳng cấu của $\Omega$.

$d) \Rightarrow c)$: Cho $a_1, \ldots, a_n$ là các phần tử của L độc lập tuyến tính trên K và gọi V là không gian vectơ con trên K của L được sinh bởi $a_1, \ldots, a_n$. Ánh xạ $f \mapsto (f(a_1), \ldots, f(a_n))$ là một song ánh R-tuyến tính của $\mathrm{Hom}_K(V, R)$ lên $\Omega^n$. Giả sử d) đúng; khi đó tồn tại các K-tự đẳng cấu $a_1, \ldots, a_n$ của $\Omega$ sao cho các phần tử $(\sigma_i(a_1), \ldots, \sigma_i(a_n))$ của $\Omega^n$ (với $1 \leq i \leq n$) lập thành một cơ sở của $\Omega^n$. Do đó ta có $\det(\sigma_i(a_j)) \neq 0$, vì thế d) suy ra c).

c) $\Rightarrow$ b): Giả sử rằng c) đúng và lấy x thuộc $\Omega \otimes_K L$. Ta viết x dưới dạng $\sum_{j=1}^n x_j \otimes a_j$, với $x_1, \ldots, x_n$ thuộc $\Omega$ và các phần tử $a_1, \ldots, a_n$ của L độc lập tuyến tính trên K. Chọn các K-tự đẳng cấu $\sigma_1, \ldots, \sigma_n$ của $\Omega$ sao cho $\det \sigma_i(a_j) \neq 0$; gọi $\chi_1, \ldots, \chi_n$ là các đồng cấu R từ $\Omega \otimes_K L$ vào $\Omega$ sao cho $\chi_i(a \otimes b) = a \cdot \sigma_i(b)$ với $a \in \Omega$ và $b \in L$. Giả sử rằng $\chi_i(x) = 0$ với $1 \leq i \leq n$, nói cách khác, rằng $\sum_{j=1}^n x_j \cdot \sigma_i(a_j) = 0$ với $1 \leq i \leq n$. Vì ta đã giả sử rằng ma trận $(\sigma_i(a_j))$ có định thức khác không, suy ra $x_i = 0$ với $1 \leq i \leq n$, và do đó $x = 0$.

b) $\Rightarrow$ a): Vì mọi mở rộng của một trường có đặc số 0 đều tách được (V, p. 122, Định lý 1) nên chỉ cần xét trường hợp K có đặc số $p \neq 0$. Gọi X là tập hợp mọi đồng cấu đại số trên R từ $\Omega \otimes_K L$ vào $\Omega$ và f là đồng cấu từ $\Omega \otimes_K L$ vào $\Omega^X$ được xác định bởi $f(u) = (\chi(u))_{\chi \in X}$ với $u \in \Omega \otimes_K L$. Điều kiện b) có nghĩa là f là đơn ánh và do đó suy ra vành $\Omega \otimes_K L$ là rút gọn. Vậy điều kiện b) của Định lý 2 (V, p. 122) được thỏa mãn với $K' = \Omega$, nên L tách được trên K.

a) $\Rightarrow$ d): Giả sử L tách được trên K. Cho V là một không gian con vectơ trên K của L có số chiều hữu hạn, $V_{(\Omega)} = \Omega \otimes_K V$ là không gian vectơ $\Omega$ dẫn xuất từ V bằng mở rộng vô hướng và $f_0$ là dạng tuyến tính trên $V_{(\Omega)}$ sao cho $f_0(x \otimes y) = xy$ với $x \in \Omega, y \in V$. Ký hiệu G là nhóm các K-tự đẳng cấu của $\Omega$; với $\sigma \in G$ ta đặt $\sigma_V = \sigma \otimes \mathrm{Id}_V$ và $g_\sigma = \sigma \circ f_0 \circ \sigma_V^{-1}$.

Với mỗi $\sigma \in G$ ánh xạ $g_\sigma$ từ $V_{(\Omega)}$ vào $\Omega$ là $\Omega$-tuyến tính và biến $x \otimes y$ thành $x \cdot \sigma(y)$ với $x \in \Omega, y \in V$. Do đó hạt nhân $N_\sigma$ của $g_\sigma$ là một không gian con vectơ của $V_{(\Omega)}$, và điều đó cũng đúng với $N = \cap_{\sigma \in G} N_\sigma$. Nếu p là số mũ đặc số của K, thì trường các bất biến của G trong $\Omega$ bằng $K^{p^{-\infty}}$ (V, p. 112, Mệnh đề 10). Rõ ràng ta có $\sigma_V(N) = N$ với mọi $\sigma \in G$; do đó (V, p. 63, Hệ quả) không gian vectơ N trên $\Omega$ được sinh bởi $N_0 = N \cap (K^{p^{-\infty}} \otimes V)$. Vì L tách được trên K, các trường $K^{p^{-\infty}}$ và L tuyến tính rời nhau trên K (V, p. 123, Hệ quả 1); ta có $K^{p^{-\infty}} \otimes_K V \subset K^{p^{-\infty}} \otimes_K L$ và $f_0(x \otimes y) = xy$ với $x \in \Omega$ và $y \in V$. Suy ra hạn chế của $f_0$ trên $K^{p^{-\infty}} \otimes_K V$ là đơn ánh. Bây giờ $f_0 = g_1$ bằng không trên N và a fortiori trên $N_0 \subset K^{p^{-\infty}} \otimes_K V$. Vì thế ta có $N_0 = 0$, do đó $N = 0$. Vì V có số chiều hữu hạn trên K, $V_{(\Omega)}$ có số chiều hữu hạn trên $\Omega$; giao của các hạt nhân của các dạng tuyến tính $g_\sigma$ bằng không, nên (II, p. 301, Định lý 7) họ $(g_\sigma)_{\sigma \in G}$ sinh ra đối ngẫu của $V_{(\Omega)}$. Bây giờ cho $u$ là một ánh xạ K-tuyến tính từ V vào $\Omega$; gọi $\tilde{u}$ là dạng tuyến tính trên $V_{(\Omega)}$ biến $x \otimes y$ thành $xu(y)$ với $x \in \Omega$ và $y \in V$. Theo điều đã nói, tồn tại các phần tử $\sigma_1, \ldots, \sigma_n$ của G và các phần tử $\lambda_1, \ldots, \lambda_n$ của $\Omega$ sao cho $\tilde{u} = \sum_{i=1}^n \lambda_i g_{\sigma_i}$, do đó $u(y) = \sum_{i=1}^n \lambda_i \sigma_i(y)$ với mọi $y \in V$. Vậy ta đã chỉ ra rằng a) kéo theo d).

### Bài tập {#alg-v-s15-exercises}

Xem [các bài tập cho § 15](exercises/s15/).
