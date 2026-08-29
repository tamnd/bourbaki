---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 2
section_title: Extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.9-A V.15, A V.146-A V.147
pdf_pages: 0123-0129, 0260-0261
extraction: ocr
subsections:
    - "no": 1
      title: The structure of an extension
      page: 9
      pdf_page: 123
    - "no": 2
      title: Degree of an extension
      page: 10
      pdf_page: 124
    - "no": 3
      title: Adjunction
      page: 10
      pdf_page: 124
    - "no": 4
      title: Composite extensions
      page: 12
      pdf_page: 126
    - "no": 5
      title: Linearly disjoint extensions
      page: 13
      pdf_page: 127
statements: 19
exercises: 4
content_sha256: d365417c53618df50e7c3814f418f0ba51f0f4bea2217544d230254c73e57d9e
translated_from: content/en/alg/V/02_s2_extensions.md
source_content_sha256: 577f8f2cd0d7531154d44ed4dfc254c2023dc0e83a12625db63a8875dd8f9066
translation_model: gpt-5.4
translation_run: translate-vi-2eae79d2
glossary_version: 34
glossary_terms_sha256: 2ed1114c1d780c41629263254a7bf8240470a75061124e7a1747c304d08dc626
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. MỞ RỘNG

### 1. Cấu trúc của một mở rộng

#### Định nghĩa 1 {#alg-v-s2-def-1 .statement}

— Cho K là một trường. Bởi một mở rộng của K, ta hiểu là một đại số trên K mà vành nền của nó là một trường. Bởi một mở rộng con (hay mở rộng con trên K) của mở rộng E, ta hiểu là một đại số con trên K của E mà là một trường.
Cho E là một mở rộng của K. Ánh xạ u : A ↦ λ . 1 từ K vào E là một đồng cấu vành; theo I, p. 115, u gây ra một đẳng cấu từ K lên một trường con u(K) của E.
Ngược lại, nếu K, E là các trường và u là một đồng cấu từ K vào E, thì u xác định trên E một cấu trúc mở rộng của K (III, p. 433). Do lạm dụng ngôn ngữ, đôi khi người ta nói rằng (E, u) là một mở rộng của K.
Một mở rộng được gọi là tầm thường nếu u(K) = E, nghĩa là nếu E là một không gian vectơ chiều 1 trên K.
Cho L là một trường mở rộng của K. Khi ta xét L như một mở rộng của K, ta hiểu theo đó là mở rộng (L, j) của K, trong đó j là đơn ánh chính tắc của K vào L, hoặc cũng là L với cấu trúc đại số trên K tương ứng. Khi đó các mở rộng con của L là các trường trung gian giữa K và L, nghĩa là các trường con của L chứa K. Nếu L' là một trường mở rộng khác của K, thì một K-đồng cấu từ L vào L' khi đó là một đồng cấu f từ L vào L' sao cho f(x) = x với mọi x ∈ K. Ta chú ý rằng nếu f là một tự đồng cấu bất kỳ của trường L, thì tập hợp các phần tử của L bất biến dưới f là một trường con K' của L, và khi đó f là một K'-tự đồng cấu của L.
Đặc biệt, cho P là trường con nguyên tố của một trường L. Ta có thể xét L như một mở rộng của P, và khi đó mọi tự đồng cấu của L đều là một P-tự đồng cấu.
Cho (E, u) là một mở rộng của K; vì u xác định một đẳng cấu từ K lên một trường con K_1 của E, nên nói chung không có khó khăn gì trong việc đồng nhất K với K_1 nhờ u. Một trường hợp mà ta không thể cho phép sự đồng nhất như vậy là khi K = E và do đó u là một tự đồng cấu của K; thường nhất u sẽ là một tự đẳng cấu của K, hoặc ánh xạ u ↦ u'', khi trường K có đặc số ≠ 0.
Hiển nhiên mọi mở rộng của K đều đẳng cấu với một mở rộng (L, j), trong đó L là một trường chứa K như trường con và j là đơn ánh chính tắc của K vào L.

### 2. Bậc của một mở rộng

Cho $A$ là một đại số trên một trường $K$. Khi đó đặc biệt nó là một không gian vectơ trên $K$; chiều của không gian vectơ này được gọi là bậc của $A$ trên $K$ và được viết là $[A : K]$ (II, p. 293). Theo định nghĩa, $[A : K]$ do đó là lực lượng của mọi cơ sở của $A$ trên $K$. Định nghĩa này đặc biệt áp dụng cho trường hợp các mở rộng của $K$.

Một mở rộng bậc 1 là tầm thường. Một mở rộng bậc 2 (resp. 3 etc.) được gọi là bậc hai (resp. bậc ba etc.). Một mở rộng bậc hữu hạn đôi khi được gọi, do lạm dụng ngôn ngữ, là một mở rộng hữu hạn.

#### Định lý 1 {#alg-v-s2-thm-1 .statement}

*Cho $E$ là một mở rộng của $K$ và $A$ là một đại số trên $E$. Khi đó ta có $[A : K] = [A : E] \cdot [E : K]$. Đặc biệt, nếu $F$ là một mở rộng của $E$, ta có*

$$
[F : K] = [F : E] \cdot [E : K].
$$

Định lý này chỉ là một trường hợp riêng của II, p. 222, Prop. 25; chính xác hơn, nếu $(a_i)$, , , là một cơ sở của $A$ trên $E$ và $(b_j)$, $\in M$ là một cơ sở của $E$ trên $K$, thì họ $(a_\lambda b_\mu)_{(\lambda,\mu) \in L \times J}$ là một cơ sở của $A$ trên $K$.

#### Hệ quả 1 {#alg-v-s2-thm-1-cor-1 .statement}

*Cho $K, E, F$ là ba trường sao cho $K \subset E \subset F$ và $[F : K]$ là hữu hạn. Khi đó các bậc $[E : K]$ và $[F : E]$ là các ước của $[F : K]$.

Do đó, nếu bậc $[F : K]$ là nguyên tố, thì không có mở rộng con nào của $F$ ngoài $K$ và $F$. Nhưng chú ý rằng khi $[F : K]$ không nguyên tố, không nhất thiết có một mở rộng con của $F$ khác $K$ và $F$ (x. V, p. 146, Bài tập 1).*

#### Hệ quả 2 {#alg-v-s2-thm-1-cor-2 .statement}

*Cho $K, E$ và $F$ là ba trường sao cho $K \subset E \subset F$. Giả sử rằng $[F : K]$ là hữu hạn, khi đó quan hệ $[E : K] = [F : K]$ là tương đương với $E = F$ và quan hệ $[F : E] = [F : K]$ là tương đương với $E = K$.

Thật vậy, nếu $L$ là một trường mở rộng của $L'$ thì $[L : L'] = 1$ là tương đương với $L' = L$.*

#### Mệnh đề 1 {#alg-v-s2-prop-1 .statement}

*Cho $A$ là một đại số bậc hữu hạn trên một trường $K$. Nếu một phần tử $a \in A$ không phải là một ước trái (resp. phải) của không trong $A$, thì nó khả nghịch trong $A$.

Vì không gian vectơ $A$ trên $K$ có số chiều hữu hạn, theo giả thiết, và ánh xạ tuyến tính $x \mapsto ax$ (resp. $x \mapsto xa$) từ $A$ vào $A$ là đơn ánh; do đó nó song ánh (II, p. 298, Hệ quả) và vì thế (I, p. 16, Nhận xét) $a$ khả nghịch trong $A$.*

#### Hệ quả {#alg-v-s2-n2-cor-1 .statement}

*Cho $A$ là một đại số giao hoán bậc hữu hạn trên một trường $K$. Nếu $A$ là một miền nguyên, thì nó là một trường.*

### 3. Phép nối

Cho $E$ là một mở rộng của một trường $K$. Với một họ $x = (x_i)_{i \in I}$ các phần tử của $E$, ta ký hiệu bởi $K(x_i)_{i \in I}$ (hoặc $K(x)$ hoặc cũng $K(x_1, \ldots, x_r)$ khi $I$ là khoảng (1, n) của N) mở rộng con nhỏ nhất của E chứa các phần tử của họ $(x_i)_i$; ta nói rằng $K(x_i)_i \in I$ thu được bằng phép nối vào K các phần tử của họ $(x_i)_i, I$ và rằng họ $(x_i)_i, I$ (hoặc tập hợp các phần tử của nó) là một họ sinh của $K(x_i)_i \in I$ đối với K (hoặc trên K). Trường $K(x_i)_i \in I$ chỉ phụ thuộc vào tập hợp A các phần tử của họ $(x_i)_i \in I$; ta cũng ký hiệu nó bởi $K(A)$. Đặc biệt ta có $K(E) = E$ và $K(\emptyset) = K . 1$. Tất cả những điều đã nói đều áp dụng đặc biệt khi E là một trường chứa K như một trường con.

Cần nhận thấy rằng nhìn chung A không phải là một tập sinh của đại số $K(A)$, nói cách khác $K(A) \neq K[A]$. "Tuy nhiên ta sẽ thấy rằng $K(A) = K[A]$ khi $K(A)$ là một mở rộng đại số của K (V, p. 18, Hệ quả 1). \*

#### Mệnh đề 2 {#alg-v-s2-prop-2 .statement}

— *Nếu M và N là hai tập con bất kỳ của một mở rộng của một trường K, thì* $K(M \cup N) = K(M)(N) = K(N)(M)$.

Vì $K(M \cup N)$ chứa $K(M)$ và N nên chứa $K(M)(N)$; do $K(M)(N)$ là một trường chứa $K \cup M \cup N$, nên nó chứa $K(M \cup N)$, do đó suy ra mệnh đề.

Đôi khi chúng tôi sẽ viết $K(M, N)$ thay cho $K(M \cup N)$.

#### Nhận xét {#alg-v-s2-n3-rem-1 .statement}

— Gọi P là trường con nguyên tố của một trường E (V, p. 2); với mọi tập con A của E, $P(A)$ là trường con nhỏ nhất của E chứa A. Đặc biệt nếu K là một trường con của E, ta có $P(K \cup A) = K(A)$. Nếu K và K' là hai trường con của E, do đó ta có $P(K \cup K') = K(K') = K'(K)$; trường này là trường con nhỏ nhất của E chứa K hoặc K', hay cũng là cận trên của K và K' trong tập hợp các trường con của E, có thứ tự bởi quan hệ bao hàm; đôi khi ta nói rằng trường này là trường sinh bởi K và K' trong E.

#### Mệnh đề 3 {#alg-v-s2-prop-3 .statement}

— *Cho $\mathcal{F}$ là một tập hợp các trường con của một trường E, có hướng đối với quan hệ $\subset$. Hợp L của các trường thuộc $\mathcal{F}$ là một trường.*

Thật vậy, nếu x và y là hai phần tử của L, thì tồn tại hai trường R, S thuộc $\mathcal{F}$ sao cho $x \in R,\ y \in S$; gọi T là một trường của $\mathcal{F}$ chứa R và S; khi đó $x \in T,\ y \in T$, do đó $x + y,\ xy$ và $x^{-1}$ (nếu $x \neq 0$) thuộc T, nên thuộc L.

#### Hệ quả {#alg-v-s2-n3-cor-1 .statement}

— *Cho E là một mở rộng của một trường K và $A \subset E$. Trường $K(A)$ là hợp của các trường $K(F)$ khi F chạy qua tập hợp mọi tập con hữu hạn của A.*

Vì tập hợp các trường $K(F)$ có hướng bởi quan hệ $\subset$, bởi lẽ $F \subset F'$ kéo theo $K(F) \subset K(F')$. Do đó hợp L của các trường ấy là một trường chứa $K \cup A$ và được chứa trong $K(A)$, vì thế đồng nhất với $K(A)$.

#### Định nghĩa 2 {#alg-v-s2-def-2 .statement}

— *Một mở rộng E của một trường K được gọi là sinh hữu hạn nếu nó có một họ sinh hữu hạn. Nó được gọi là đơn sinh nếu tồn tại x trong E sao cho* $E = K(x)$.

Hệ quả của Mệnh đề 3 cho thấy rằng mọi mở rộng E của một trường K đều là một hợp có hướng của các mở rộng sinh hữu hạn được chứa trong E. Hiển nhiên là mọi mở rộng E của K có bậc hữu hạn cũng đều sinh hữu hạn vì một cơ sở của E (xét như không gian vectơ trên K) cũng là một họ sinh của E trên K; ta sẽ thấy sau này rằng đảo lại thì không đúng.

### 4. Mở rộng hợp thành

Cho E và F là hai mở rộng của một trường K. Ta hiểu một mở rộng hợp thành của $E$ và F là mọi bộ ba $(L, u, v)$, trong đó L là một mở rộng của K, $u$ là một K-đồng cấu của E vào L và $v$ là một K-đồng cấu của F vào L, và trong đó trường L được sinh bởi $u(E) \cup v(F)$ (x. Hình 1).

![Sơ đồ biểu diễn các mở rộng E, F, K, L, các đồng cấu u, v, r](../images/fig_1.png)

Hình 1.

Phù hợp với các định nghĩa tổng quát (E, IV, p. 6), một đẳng cấu của một mở rộng hợp thành $(L, u, v)$ của E và F lên một mở rộng hợp thành $(L', u', v')$ của E và F là một K-đẳng cấu $\varphi$ của L lên $L'$ sao cho $u' = \varphi \circ u$ và $v' = \varphi \circ v$.

Cho $(L, u, v)$ là một mở rộng hợp thành của E và F. Ánh xạ K-tuyến tính $w$ từ $E \otimes_K F$ vào L, ánh xạ $x \otimes y$ thành $u(x)v(y)$, là một đồng cấu đại số trên K; trong số này chúng tôi sẽ ký hiệu nó bởi $u * v$. Ảnh của nó là vành con của L sinh bởi $u(E) \cup v(F)$.

#### Mệnh đề 4 {#alg-v-s2-prop-4 .statement}

— Cho E, F là hai mở rộng của K.

a) Cho $(L, u, v)$ là một mở rộng hợp thành của E và F; khi đó hạt nhân p của đồng cấu $u * v$ từ $E \otimes_K F$ vào L là một iđêan nguyên tố.

b) Cho p là một iđêan nguyên tố của $E \otimes_K F$; khi đó tồn tại một mở rộng hợp thành $(L, u, v)$ của E và F sao cho p là hạt nhân của $u * v$, và hai mở rộng hợp thành như vậy bất kỳ đều đẳng cấu.

Mệnh đề a) suy ra từ sự kiện là hạt nhân của một đồng cấu từ một vành vào một trường là một iđêan nguyên tố (I, p. 116-117).

Cho p là một iđêan nguyên tố của $E \otimes_K F$, A là vành thương $(E \otimes_K F)/p$ và L là trường phân thức của A. Với $x \in E$ (tương ứng $y \in F$) ta ký hiệu bởi $u(x)$ (tương ứng $v(y)$) lớp thặng dư mod p của $x \otimes 1$ (tương ứng $1 \otimes y$). Khi đó $u$ (tương ứng $v$) là một K-đồng cấu từ E (tương ứng F) vào L và $u(E) \cup v(F)$ sinh ra A như một vành, do đó sinh ra L như một trường. Vì vậy $(L, u, v)$ là một mở rộng hợp thành của E và F; ta thấy ngay rằng $u * v$ là đồng cấu chính tắc từ $E \otimes_K F$ vào L, và vì thế hạt nhân của nó bằng p.

Cho $(L', u', v')$ là một mở rộng hợp thành của E và F sao cho hạt nhân của $u' * v'$ bằng p. Vì $u * v$ và $u' * v'$ có cùng hạt nhân, tồn tại một đẳng cấu $\psi$ của A lên ảnh $A'$ của $u' * v'$, được xác định bởi $u' * v' = \psi \circ (u * v)$. Nhưng $A'$ là vành con của $L'$ sinh bởi $u'(E) \cup v'(F)$, do đó L' là trường phân thức của A'. Vậy $\psi$ mở rộng thành một đồng cấu $\varphi$ từ L vào L' và hiển nhiên $\varphi$ là một đẳng cấu từ $(L, u, v)$ lên $(L', u', v')$.

#### Nhận xét {#alg-v-s2-n4-rem-1 .statement}

— Nếu $p$ và $p'$ là hai iđêan nguyên tố phân biệt của $E \otimes_K F$, thì các *mở rộng hợp thành* tương ứng của $E$ và $F$ (được xây dựng bằng thủ tục của chứng minh trên) không đẳng cấu. Tuy nhiên, chúng vẫn có thể đẳng cấu như những *mở rộng* của K (*V*, p. 146, Bài tập 2).

#### Hệ quả {#alg-v-s2-n4-cor-1 .statement}

*Các mở rộng hợp thành của E và F tồn tại*.

Thật vậy, vì vành giao hoán $E \otimes_K F$ không bị thu về 0, nên nó có các iđêan nguyên tố: định lý Krull (*I*, p. 104) chứng minh sự tồn tại của các iđêan cực đại, và mọi iđêan cực đại đều là nguyên tố.

Ta có thể làm cho hệ quả này chính xác hơn như sau. Cho $(E, u)$ và $(F, v)$ là hai mở rộng của K ; chọn một iđêan cực đại m của vành giao hoán $E \otimes_K F$ và đặt $L = (E \otimes_K F)/m$; khi đó L là một mở rộng của K. Với $x \in E$ viết $u'(x)$ cho lớp thặng dư của $x \otimes 1$ mod m và tương tự đặt $v'(y)$ cho lớp thặng dư của $1 \otimes y$ mod $m$ với mọi $y \in F$. Khi đó ta có một biểu đồ giao hoán các đồng cấu trường

$$
\begin{array}{ccc}
F & \xrightarrow{v'} & L \\
| & & | \\
K & \xrightarrow{u} & E .
\end{array}
$$

Bằng cách thay thế $(L, u')$ bởi một mở rộng đẳng cấu của E, ta có thể giả sử rằng L chứa E như một trường con và $u'$ là đơn ánh chính tắc của E vào L. Bằng cách thay đổi ký hiệu, do đó ta thu được chú giải sau đây :

#### Chú giải {#alg-v-s2-n4-sch-1 .statement}

*Cho K và E là hai trường và u là một đồng cấu của K vào E. Nếu K' là một trường chứa K như trường con, thì tồn tại một trường E' chứa E như trường con và một đồng cấu u' của K' vào E' mở rộng u*'.

### 5. Các mở rộng độc lập tuyến tính

*Trong suốt No. này, R biểu thị một mở rộng của trường K*.

Cho A và B là hai K-đại số con của R. Tồn tại một đồng cấu đại số $\varphi : A \otimes_K B \to R$ ánh xạ $x \otimes y$ thành $xy$. Ảnh của $\varphi$ là một vành con C của $\Omega$ sinh bởi A U B. Hơn nữa, theo II, p. 256, nếu $(b,)$ là một cơ sở của B trên K và $(a,)$ là một cơ sở của A trên K, thì C trùng với tập hợp các tổ hợp tuyến tính $\sum_{\mu} \alpha_{\mu} b_{\mu}$ với $\alpha_{\mu} \in A$, tập hợp mọi $\sum_{\lambda} \beta_{\lambda} a_{\lambda}$ với $\beta_{\lambda} \in B$ và cả tập hợp mọi $\sum_{\lambda,\mu} \gamma_{\lambda\mu} a_{\lambda} b_{\mu}$, trong đó $\gamma_{\lambda\mu} \in K$.

Ta sẽ nói rằng A và B *rời nhau tuyến tính trên* K, nếu $\varphi$ là một *đẳng cấu* của $A \otimes_K B$ lên C. Khi đó ta có $A \cap B = K$; mọi tập con tự do của B (resp. A) đối với K khi đó đều tự do đối với A (resp. B); ngược lại, để A và B rời nhau tuyến tính trên K, điều kiện đủ là tồn tại *một* cơ sở của B trên K (chẳng hạn) tự do đối với A (II, p. 256 and III, p. 469).

Xét riêng trường hợp A và B là các *mở rộng con* của $\Omega$.

#### Mệnh đề 5 {#alg-v-s2-prop-5 .statement}

*Cho E và F là hai mở rộng của K được chứa trong $\Omega$.*

*a)* *Nếu F có bậc hữu hạn trên K, thì vành con của $\Omega$ được sinh bởi $E \cup F$ là một trường, trùng với $E(F)$ và bậc của $E(F)$ trên E là hữu hạn; ta có* $[E(F):E] \leq [F:K]$, *với đẳng thức xảy ra khi và chỉ khi E và F rời nhau tuyến tính trên K. Trong trường hợp đó $E(F)$ E-*đẳng cấu* với $E \otimes_K F$.*

*b)* *Nếu thêm nữa E có bậc hữu hạn trên K, thì $E(F) = K(E \cup F)$ có bậc hữu hạn trên K. Ta có* $[K(E \cup F):K] \leq [E:K][F:K]$ *với đẳng thức xảy ra khi và chỉ khi E và F rời nhau tuyến tính trên K.*

Thật vậy, gọi C là vành con của $\Omega$ sinh bởi $E \cup F$; nếu $(b_j)_{1 \leq j \leq n}$ là một cơ sở của F trên K, thì C là không gian con vectơ trên E của $\Omega$ sinh bởi các $b_j$, do đó C là một đại số có hạng *hữu hạn* $\leq n$ trên E; vì vành C được chứa trong một trường, nên nó là một miền nguyên, và do đó là một *trường*, theo Hệ quả của Mệnh đề 1 (V, p. 10), suy ra $C = E(F)$ và $[E(F):E] \leq [F:K]$. Quan hệ $[E(F):E] = [F:K]$ có nghĩa là các $b_j$ độc lập tuyến tính trên E, do đó E và F độc lập tuyến tính trên K; điều này chứng minh phần *a)* của mệnh đề. Phần *b)* khi đó suy ra ngay vì $[E(F):K] = [E(F):E][E:K]$.

Cho E và F là các mở rộng của K được chứa trong $\Omega$; nếu E và F có bậc vô hạn trên K, vành con $C = K[E \cup F]$ không nhất thiết là một trường $^1$; tuy nhiên *trường phân thức* của C khi đó trùng với $K(E \cup F)$. Nói chung, cho A là một vành con của E sao cho E là trường phân thức của A, và cho B là một vành con của F sao cho F là trường phân thức của B; khi đó nếu C là vành con của $\Omega$ sinh bởi $A \cup B$, thì $K(E \cup F)$ trùng với *trường phân thức* của C, vì trường sau là trường con nhỏ nhất của $\Omega$ chứa C và nó chứa E và F. Hơn nữa:

#### Mệnh đề 6 {#alg-v-s2-prop-6 .statement}

*Cho E và F là hai mở rộng của K được chứa trong $\Omega$, và A và B là hai đại số con của $\Omega$ trên K sao cho E là trường phân thức của A và F là trường phân thức của B. Khi đó điều kiện cần và đủ để E và F rời nhau tuyến tính trên K là A và B rời nhau tuyến tính trên K.*

Điều kiện ấy rõ ràng là cần. Ngược lại, nếu A và B rời nhau tuyến tính trên K, thì A và F cũng vậy, vì nếu một họ các phần tử của $\Omega$ là tự do đối với B, thì nó là tự do đối với trường phân thức F của B (II, p. 315, Hệ quả 1 and p. 316, Hệ quả 3); giờ đây cùng một lập luận cho thấy E và F rời nhau tuyến tính trên K.

$^1$ Chỉ cần xét chẳng hạn trường hợp $\Omega$ là trường $K(X, Y)$ các phân thức hữu tỉ theo hai bất định X và Y và $E = K(X), F = K(Y)$.

#### Mệnh đề 7 {#alg-v-s2-prop-7 .statement}

— Cho E và F là hai mở rộng của K được chứa trong $\Omega$; nếu E và F rời nhau tuyến tính trên K, thì mọi mở rộng con của E và mọi mở rộng con của F đều rời nhau tuyến tính trên K. Ngược lại, nếu với mọi cặp mở rộng con sinh hữu hạn E', F' tương ứng của E và F, E' và F' rời nhau tuyến tính trên K, thì E và F rời nhau tuyến tính trên K.

Vì điều kiện để E và F rời nhau tuyến tính trên K có thể được phát biểu như sau: nếu $(a_\alpha)$ là một họ tự do trong E và $(b_\beta)$ là một họ tự do trong F, thì quan hệ $\sum_{\alpha,\beta} \lambda_{\alpha\beta} a_\alpha b_\beta = 0$, trong đó $\lambda_{\alpha\beta} \in K$, suy ra $\lambda_{\alpha\beta} = 0$ với mỗi cặp chỉ số. Nhưng điều kiện này được thỏa mãn với mỗi cặp họ tự do nếu nó đúng với mỗi cặp họ tự do hữu hạn.

Do đó ta có thể nói, theo cách nói trực giác, rằng tính rời nhau tuyến tính là một tính chất « có đặc trưng hữu hạn ».

#### Mệnh đề 8 {#alg-v-s2-prop-8 .statement}

— Cho E, F, G là ba mở rộng của một trường K được chứa trong $\Omega$, sao cho $F \subset G$. Để E và G rời nhau tuyến tính trên K, điều kiện cần và đủ là E và F rời nhau tuyến tính trên K và E(F) và G rời nhau tuyến tính trên F.

$$
\begin{array}{ccccc}
E & \longrightarrow & E(F) \\
K & \longrightarrow & F & \longrightarrow & G.
\end{array}
$$

Hình 2.

Điều kiện là cần thiết: giả sử rằng E và G rời nhau tuyến tính trên K. Khi đó điều tương tự cũng đúng với E và F (Mệnh đề 7); mặt khác, nếu B là một cơ sở của E trên K, thì B cũng là một cơ sở của đại số F[E] trên F; vì theo giả thiết B là tự do trên G, F[E] và G rời nhau tuyến tính trên F, và điều tương tự cũng đúng với $E(F) = F(E)$ và G, theo Mệnh đề 6.

Điều kiện là đủ: với cùng ký hiệu như trên, nó suy ra rằng B là tự do trên F, do đó B là một cơ sở của F[E] trên F; vì theo giả thiết F[E] và G rời nhau tuyến tính trên F, B là tự do trên G, và điều này cho thấy rằng E và G rời nhau tuyến tính trên K.

### Bài tập {#alg-v-s2-exercises}

Xem [bài tập của § 2](exercises/s2/).
