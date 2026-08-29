---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 2
section_title: The lift of prime ideals
lang: vi
source: ac-i-vii
book_pages: 325-344, 362-369
pdf_pages: 0344-0363, 0381-0388
extraction: ocr
subsections:
    - "no": 1
      title: THE FIRST EXISTENCE THEOREM
      page: 325
      pdf_page: 344
    - "no": 2
      title: DECOMPOSITION GROUP AND INERTIA GROUP
      page: 330
      pdf_page: 349
    - "no": 3
      title: DECOMPOSITION AND INERTIA FOR INTEGRALLY CLOSED DOMAINS
      page: 337
      pdf_page: 356
    - "no": 4
      title: THE SECOND EXISTENCE THEOREM
      page: 343
      pdf_page: 362
statements: 36
exercises: 22
content_sha256: 755e2932b4f6bd0615cef0a7ad081536ff92d337f4405f4904a2225cebc67db1
translated_from: content/en/ac/V/02_s2_the_lift_of_prime_ideals.md
source_content_sha256: 0735cbdcddf5abb906e8dd4e39035bbe753450d10e43d8bd20b9833595a17cd5
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-4c7244ec
glossary_version: 34
glossary_terms_sha256: 98d683363c712b7cdfc8148e606b0ee3d1ed71824dd7859764bba992f66768fe
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. PHÉP NÂNG CỦA CÁC IĐÊAN NGUYÊN TỐ

### 1. ĐỊNH LÝ TỒN TẠI ĐẦU TIÊN

#### Định nghĩa 1 {#ac-v-s2-def-1 .statement}

Cho $\mathbf{A}, \mathbf{A}'$ là hai vành và $h : \mathbf{A} \to \mathbf{A}'$ là một đồng cấu vành. Một iđêan $a' \in A'$ được nói là nằm trên một iđêan $a$ của $\mathbf{A}$ nếu $a = \overline{h}^1(a')$.

Nói rằng một iđêan nguyên tố $p'$ của $A'$ nằm trên một iđêan $p$ của $\mathbf{A}$ có nghĩa là $p$ là ảnh của $p'$ qua ánh xạ liên tục "$h : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$" liên kết với $h$ (chương 11, § 4, no. 3).

Lưu ý rằng để tồn tại một iđêan của $A'$ nằm trên iđêan $(0)$ của $\mathbf{A}$, điều kiện cần và đủ là $h : \mathbf{A} \to \mathbf{A}'$ đơn ánh.

Cho $a$ là một iđêan của $\mathbf{A}$; bằng cách lấy thương, đồng cấu $h$ cho một đồng cấu $h_1 : \mathbf{A}/a \to \mathbf{A}'/a'$; nói rằng $a'$ là một iđêan của $A'$ nằm trên $a$ tương đương với nói rằng $aA' \subset a'$ và $a'/aA'$ là một iđêan của $\mathbf{A}'/aA'$ nằm trên $(0)$.

#### Bổ đề 1 {#ac-v-s2-lem-1 .statement}

Cho $h : \mathbf{A} \to \mathbf{A}'$ là một đồng cấu vành, $S$ là một tập con nhân của $\mathbf{A}$, $i = i_A^S : \mathbf{A} \to S^{-1}\mathbf{A}$, $i' = i_{A'}^{h(S)} : \mathbf{A}' \to S^{-1}\mathbf{A}' = (h(S))^{-1}\mathbf{A}'$ là các đồng cấu chính tắc và $h_1 = S^{-1}h : S^{-1}\mathbf{A} \to S^{-1}\mathbf{A}'$, sao cho có một biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathbf{A} & \xrightarrow{h} & \mathbf{A}' \\
i \downarrow & & i' \downarrow \\
S^{-1}\mathbf{A} & \xrightarrow{h_1} & S^{-1}\mathbf{A}'
\end{array}
$$

Cho $p$ là một iđêan nguyên tố của $\mathbf{A}$ sao cho $p \cap S = \varnothing$. Khi đó $a' \mapsto S^{-1}a'$ là một ánh xạ toàn ánh từ tập hợp $\mathcal{F}$ các iđêan của $\mathbf{A}'$ nằm trên $p$ lên tập hợp $\mathcal{F}_1$ các iđêan của $S^{-1}\mathbf{A}'$ nằm trên $S^{-1}p$ và ánh xạ $a'_1 \mapsto i'(a'_1)$ là một song ánh từ $\mathcal{F}_1$ lên tập hợp các iđêan thuộc $\mathcal{F}$ và bão hòa đối với $h(S)$; đặc biệt, $p' \mapsto S^{-1}p'$ là một song ánh từ tập hợp các iđêan nguyên tố của $\mathbf{A}'$ nằm trên $p$ lên tập hợp các iđêan nguyên tố của $S^{-1}\mathbf{A}'$ nằm trên $S^{-1}p$.

Ta biết rằng $S^{-1}p$ là một iđêan nguyên tố của $S^{-1}\mathbf{A}$ và $i_1(S^{-1}p) = p$ (Chương 11, § 2, no. 5, Mệnh đề 11); nếu tồn tại một iđêan $b'$ của $S^{-1}\mathbf{A}'$ nằm trên $S^{-1}p$, thì $h(i_1(b')) = i(h_1(b')) = p$; vì $S^{-1}i'(b') = b'$ (nơi đã dẫn), điều này đã cho thấy rằng ảnh của $\mathcal{F}$ qua ánh xạ $a' \mapsto S^{-1}a'$ chứa $\mathcal{F}_1$. Mặt khác, nếu $a' \in \mathcal{F}$, $a \in A$ và $s \in S$, ta có các tương đương sau

$$
h_1(a/s) \in S^{-1}a' \iff h(a)/h(s) \in S^{-1}a'
$$
$\iff$ tồn tại $t \in S$ sao cho $h(t)h(a) \in a'$
$\iff$ tồn tại $t \in S$ sao cho $ta \in \mathfrak{p}$
$\iff a/z \in S^{-1}\mathfrak{p}$.

Do đó $h_1^{-1}(S^{-1}a') = S^{-1}\mathfrak{p}$, điều này hoàn tất chứng minh rằng ảnh của $\mathcal{F}$ qua ánh xạ $a' \mapsto S^{-1}a'$ bằng $\mathcal{F}_1$; các khẳng định khác suy ra từ Chương 11, § 2, no. 5, Mệnh đề 11.

#### Mệnh đề 1 {#ac-v-s2-prop-1 .statement}

*Cho $h : A \to A'$ là một đồng cấu vành sao cho $A'$ là nguyên trên $A$, $\mathfrak{p}'$ là một iđêan nguyên tố của $A'$ và $\mathfrak{p} = h^{-1}(\mathfrak{p}')$. Để $\mathfrak{p}$ là cực đại, điều kiện cần và đủ là $\mathfrak{p}'$ cũng vậy.*

Đặt $B = A/\mathfrak{p}$, $B' = A'/\mathfrak{p}'$ và gọi $h_1 : B \to B'$ là đồng cấu dẫn xuất từ $h$ bằng cách lấy thương; $B$ và $B'$ là các miền nguyên và $B'$ là nguyên trên $B$ ($§ 1$, no. 1, Mệnh đề 2). Nói rằng $\mathfrak{p}$ (tương ứng $\mathfrak{p}'$) là cực đại có nghĩa là $B$ (tương ứng $B'$) là một trường. Khi đó mệnh đề suy ra từ bổ đề sau:

#### Bổ đề 2 {#ac-v-s2-lem-2 .statement}

*Cho $B$ là một miền nguyên và $A$ là một vành con của $B$ sao cho $B$ là nguyên trên $A$. Để $B$ là một trường, điều kiện cần và đủ là $A$ là một trường.*

Nếu $A$ là một trường, thì, với mọi $y \neq 0$ trong $B$, theo giả thiết $A[y]$ là một $A$-môđun sinh hữu hạn ($§ 1$, Định lý 1); vì $A[y]$ là một miền nguyên, nó là một trường (*Đại số*, Chương V, § 2, no. 1, Mệnh đề 1) và a fortiori $y$ khả nghịch trong $B$ và do đó $B$ là một trường. Ngược lại, giả sử rằng $B$ là một trường và lấy $z \neq 0$ trong $A$; vì $z^{-1} \in B$, $z^{-1}$ là nguyên trên $A$, nói cách khác có một phương trình phụ thuộc nguyên

$$
z^{-n} + a_1 z^{-(n-1)} + \ldots + a_n = 0
$$

trong đó các $a_i \in A$; bây giờ quan hệ này cho thấy rằng

$$
-z^{-1} = a_1 + a_2 z + \ldots + a_n z^{n-1} \in A,
$$

do đó hiển nhiên $A$ là một trường.

#### Hệ quả 1 {#ac-v-s2-lem-2-cor-1 .statement}

*Cho $h : A \to A'$ là một đồng cấu vành sao cho $A'$ là nguyên trên $A$, $\mathfrak{p}$ là một iđêan nguyên tố của $A$ và $\mathfrak{p}'$ và $a'$ là hai iđêan của $A'$ nằm trên $\mathfrak{p}$ sao cho $\mathfrak{p}' \subset a'$. Nếu $\mathfrak{p}'$ là nguyên tố, thì $a' = \mathfrak{p}'$.*

Ta viết $S = A - \mathfrak{p}$; khi đó $S^{-1}A'$ là nguyên trên $S^{-1}A$ ($§ 1$, no. 5, Mệnh đề

16), $S^{-1}p$ là một iđêan cực đại của $S^{-1}A$ (Chương 11, § 2, no. 5, Mệnh đề 11), $S^{-1}a'$ và $S^{-1}p'$ là các iđêan của $S^{-1}A'$ nằm trên $S^{-1}p$ (Bổ đề 1) và $S^{-1}a' \supseteq S^{-1}p'$. Vì $S^{-1}p'$ là nguyên tố, nó là cực đại theo Mệnh đề 1 và do đó $S^{-1}p' = S^{-1}a'$; vì vậy $a'$ được chứa trong bão hòa của $p'$ đối với $h(S)$, mà bão hòa này bằng $p'$ (Chương II, § 2, no. 5, Mệnh đề 11).

#### Hệ quả 2 {#ac-v-s2-lem-2-cor-2 .statement}

Cho $A'$ là một miền nguyên, $A$ là một vành con của $A'$ sao cho $A'$ là nguyên trên $A$ và $f$ là một đồng cấu từ $A'$ vào một vành $B$. Nếu hạn chế của $f$ lên $A$ là đơn ánh thì $f$ là đơn ánh.

Nếu $a'$ là hạt nhân của, giả thiết có nghĩa là $a' \cap A = (0)$; vì $A'$ là một miền nguyên, có thể áp dụng Hệ quả 1 bằng cách lấy $p$ và $p'$ lần lượt là iđêan (0) của $A$ và iđêan (0) của $A'$, do đó $a' = (0)$.

#### Hệ quả 3 {#ac-v-s2-lem-2-cor-3 .statement}

Cho $h : A \to A'$ là một đồng cấu vành sao cho $A'$ nguyên trên $A$ và $m$ là một iđêan cực đại của $A$, và giả sử trong $A'$ chỉ có một số hữu hạn iđêan cực đại phân biệt $m'_j$ ($1 \leq j \leq n$) nằm trên $m$. Gọi $q'_j$ là sự bão hòa của $mA'$ đối với $m'_j$ (Chương II, § 2, no. 4). Khi đó:
(i) Trong vành $A'/q'_j$, các ước của không là các phần tử của $m'_j/q'_j$ và chúng lũy linh ($1 \leq j \leq n$).
(ii) $mA' = \bigcap_j q'_j = \prod_j q'_j$.
(iii) Đồng cấu chính tắc $A'/mA' \to \prod_j (A'/q'_j)$ là song ánh.

Để một iđêan nguyên tố của $A'$ chứa $mA'$, điều kiện cần và đủ là ảnh ngược của nó qua $h$ chứa $m$ và do đó nó nằm trên $m$, vì $m$ là cực đại trong $A$; do đó các $m'_j$ là những iđêan nguyên tố duy nhất của $A'$ chứa $mA'$ (Mệnh đề 1) và vì vậy $c' = \bigcap_j m'_j$ là căn của $mA'$ (Chương II, § 2, no. 6, Hệ quả 1 của Mệnh đề 13). Theo định nghĩa của $q'_j$, lớp mod. $q'_j$ của một phần tử thuộc $A' - m'_j$ không phải là một ước của 0 trong $A'/q'_j$; mặt khác, vì các $m'_j$ là những iđêan cực đại phân biệt, với mỗi chỉ số $j$ tồn tại một phần tử $a'_j$ thuộc $\bigcap_j m'_j$ và không thuộc $m'_j$ (Chương II, § 1, no. 1, Mệnh đề 4): khi đó, với mọi $x \notin m'_j, a'_j x \in r'$, do đó lớp mod. $q'_j$ của $a'_j x$ là lũy linh và, vì lớp của $a'_j$ không phải là một ước của 0, ta kết luận rằng lớp của $x$ là lũy linh; nói cách khác, $m'_j$ là căn của $q'_j$, điều này chứng minh (i). Suy ra các $q'_j$ nguyên tố cùng nhau từng đôi một (Chương II, § 1, no. 1, Mệnh đề 3); do đó (iii) sẽ là một hệ quả của (ii), có tính đến Chương II, § 1, no. 2, Mệnh đề 5. Để thiết lập (ii), ta chú ý rằng trong vành $A'/mA'$ các $m'_j/mA'$ là những iđêan cực đại duy nhất và $q'_j/mA'$ là sự bão hòa của (0) đối với $m'_j/mA'$ (Chương 11, § 2, no. 4); do đó ta có thể giới hạn sự chú ý vào trường hợp $mA' = (0)$; mệnh đề (ii) khi đó suy ra từ Chương II, § 3, no. 3, Hệ quả 2 của Định lý 1.

Nhận xét (1) Nếu $A'$ là Noether, suy ra từ (i) và (ii) rằng $(q'_j)_{1 \leq j \leq n}$ là phân tích nguyên sơ duy nhất của $mA'$ (Chương IV, § 2, no. 3).

#### Định lý 1 {#ac-v-s2-thm-1 .statement}

Cho $h : A \to A'$ là một đồng cấu vành đơn ánh sao cho $A$ là nguyên trên $A$ và $p$ là một iđêan nguyên tố của $A$. Tồn tại một iđêan nguyên tố $p'$ của $A'$ nằm trên $p$.

Trước hết giả sử rằng $A$ là một vành địa phương và $p$ là iđêan cực đại của $A$; khi đó, với mọi iđêan cực đại $m'$ của $A'$, $h^{-1}(m')$ là một iđêan cực đại của $A$ (Mệnh đề 1) và do đó bằng $p$, điều này chứng minh định lý trong trường hợp này (vì $A'$ chứa $A$ theo giả thiết và do đó không bị rút gọn về 0). Trong trường hợp tổng quát, viết $S = A - p$; khi đó $S^{-1}A$ là một vành địa phương mà iđêan cực đại là $S^{-1}p$ (Chương 11, § 2, no. 5, Mệnh đề 11), $S^{-1}h : S^{-1}A \to S^{-1}A$, là đơn ánh (Chương II, § 2, no. 4, Định lý 1) và $S^{-1}A'$ là nguyên trên $S^{-1}A$ ($§ 1$, no. 5, Mệnh đề 16); khi đó tồn tại một iđêan nguyên tố $q'$ của $S^{-1}A'$ nằm trên $S^{-1}p$ và ta biết rằng $q' = S^{-1}p'$, trong đó $p'$ là một iđêan nguyên tố của $A'$ nằm trên $p$ (Bổ đề 1).

Nếu $h : A \to A'$ không đơn ánh, Định lý 1 không còn nhất thiết đúng nữa, như ví dụ về đồng cấu $Z \to \mathbf{Z}/n\mathbf{Z} \ (n > 1)$ cho thấy. Tuy nhiên Định lý 1 có thể được áp dụng cho đơn ánh chính tắc $h(A) \to A'$; nói cách khác, mệnh đề của Định lý 1 là đúng đối với các iđêan nguyên tố $p$ chứa $\mathrm{Ker}(h)$.

#### Hệ quả 1 {#ac-v-s2-thm-1-cor-1 .statement}

Với các giả thiết và ký hiệu của Định lý 1, $\bar{h}^{-1}(pA') = p$.

$pA' \subset p'$ và $\bar{h}(p') = p$.

#### Hệ quả 2 {#ac-v-s2-thm-1-cor-2 .statement}

Cho $h : A \to A'$ là một đồng cấu vành sao cho $A'$ là nguyên trên $A$, $a$ và $p$ là hai iđêan của $A$ sao cho $a \subset p$ và $a'$ là một iđêan của $A'$ nằm trên $a$. Giả sử rằng $p$ là nguyên tố. Khi đó tồn tại một iđêan nguyên tố $p'$ của $A'$ nằm trên $p$ và chứa $a'$.

Nếu $h_1 : A/a \to A'/a'$ là đồng cấu dẫn xuất từ $h$ bằng cách lấy thương, thì $h_1$ là đơn ánh theo giả thiết và $A'/a'$ là nguyên trên $A/a$ ($§ 1$, no. 1, Mệnh đề 2); khi đó tồn tại một iđêan nguyên tố $p'/a'$ của $A'/a'$ ($p'$ nguyên tố trong $A$) nằm trên $p/a$ (Định lý 1) và $p'$ là iđêan cần tìm.

#### Hệ quả 3 {#ac-v-s2-thm-1-cor-3 .statement}

Cho $A$ là một vành và $A'$ là một vành chứa $A$ và nguyên trên $A$. Nếu $\mathcal{R}'$ là căn Jacobson của $A'$, thì $\mathcal{R}' \cap A$ là căn Jacobson của $A$.

Cho $32$ là căn Jacobson của $A$. Với mọi iđêan cực đại $m'$ của $A'$, $m' \cap A$ là một iđêan cực đại của $A$ (Mệnh đề 1), do đó $\mathcal{R} \subset m' \cap A$ và vì thế $\mathcal{R} \subset \mathcal{R}' \cap A$ (Đại số, Chương VIII, § 5, no. 3, Định nghĩa 3). Ngược lại, lấy $x \in 32' \cap A$; với mọi iđêan cực đại $m$ của $A$, tồn tại một iđêan nguyên tố của $A'$ nằm trên $m$ (Định lý 1) và iđêan này $m'$ tất yếu là cực đại (Mệnh đề 1), do đó $x \in m' \cap A = m$ và vì thế $x \in 32$.

#### Hệ quả 4 {#ac-v-s2-thm-1-cor-4 .statement}

Cho $A$ là một vành, $A'$ là một vành chứa $A$ và nguyên trên $A$, và $f$ là một đồng cấu từ $A$ vào một trường đóng đại số $L$. Khi đó có thể mở rộng $f$ thành một đồng cấu từ $A'$ vào $L$.

Cho $\mathfrak{p}$ là hạt nhân của $f$, đây là một iđêan nguyên tố vì $f(A) \subset L$ là một miền nguyên; gọi $\mathfrak{p}'$ là một iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}$ (Định lý 1). Khi đó $A/\mathfrak{p}$ được đồng nhất một cách chính tắc với một vành con của $A'/\mathfrak{p}'$ và $A'/\mathfrak{p}'$ là nguyên trên $A/\mathfrak{p}$ ($§ 1$, no. 1, Mệnh đề 2). Đồng cấu $f$ xác định, bằng cách lấy thương, một đẳng cấu từ $A/\mathfrak{p}$ lên vành con $f(A)$ của $L$, đẳng cấu này có thể được mở rộng thành một đẳng cấu $g$ từ trường phân thức $K$ của $A/\mathfrak{p}$ lên một trường con của $L$. Vì trường phân thức $K'$ của $A'/\mathfrak{p}'$ là đại số trên $K$, nên $g$ có thể được mở rộng thành một đẳng cấu $g'$ từ $K'$ lên một trường con của $L$ (Đại số, Chương V, $§ 4$, no. 2, Hệ quả của Định lý 1); nếu $\pi': A' \to A'/\mathfrak{p}'$ là đồng cấu chính tắc, thì $g' \circ \pi'$ là một đồng cấu từ $A'$ vào $L$ mở rộng $f$.

Nhận xét (2). Cho $h : A \to A'$ là một đồng cấu vành sao cho $A'$ là nguyên trên $A$; khi đó ánh xạ liên tục liên kết $^a h : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$ là đóng. Với mọi iđêan $a'$ của $A'$, $A'/a'$ là nguyên trên $A'$, nên cũng nguyên trên $A$ ($§ 1$, no. 1, Mệnh đề 6) và $\mathrm{Spec}(A'/a')$ được đồng nhất với một không gian con đóng $V(a')$ của $\mathrm{Spec}(A')$; để chứng minh rằng $^a h$ là đóng, khi đó ta thấy (thay thế $A'$ bởi $A'/a'$) rằng chỉ cần chứng minh ảnh của $\mathrm{Spec}(A)'$ dưới $^a h$ là một tập con đóng của $\mathrm{Spec}(A)$; mà theo Định lý 1, ảnh này chính là tập hợp các iđêan nguyên tố của $A$ chứa iđêan $\mathrm{Ker}(h)$ và tập hợp này là đóng theo định nghĩa của tôpô trên $\mathrm{Spec}(A)$.

#### Mệnh đề 2 {#ac-v-s2-prop-2 .statement}

Cho $h : A \to A'$ là một đồng cấu vành sao cho $A'$ nguyên trên $A$, $\mathfrak{p}$ là một iđêan nguyên tố của $A$, $S = A - \mathfrak{p}$, $(p'_i)_{i \in I}$ là họ tất cả các iđêan nguyên tố $\mathfrak{p}$ của $A'$ nằm trên $\mathfrak{p}$ và $S' = \bigcap_{i \in I} (A' - p_i)$; khi đó $S^{-1}A' = {S'}^{-1}A'$.

Thật vậy, theo định nghĩa thì $h(S) \subset S'$ và, vì

$$
h(S)^{-1}A' = S^{-1}A',
$$

nên chỉ cần chứng minh, nhờ Chương II, $§ 2$, no. 3, Mệnh đề 8, rằng nếu một iđêan nguyên tố $q'$ của $A'$ không giao với $h(S)$ thì nó cũng không giao với $S'$. Bây giờ, giả sử $q' \cap h(S) = \varnothing$ và đặt $q = h^{-1}(q')$; khi đó $q \cap S = \varnothing$, nói cách khác $q \subset \mathfrak{p}$. Vì theo định nghĩa $q'$ nằm trên $q$, suy ra từ Hệ quả 2 của Mệnh đề 1 rằng tồn tại một chỉ số $c$ sao cho $q' \subset p'_c$ và do đó $q' \cap S' = \varnothing$, điều này hoàn tất chứng minh.

#### Mệnh đề 3 {#ac-v-s2-prop-3 .statement}

Cho $h : A \to A'$ là một đồng cấu vành sao cho $A'$ là một $A$-môđun sinh hữu hạn; khi đó, với mọi iđêan nguyên tố $\mathfrak{p}$ của $A$, tập các iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}$ là hữu hạn.

Đặt $S = A - p$; theo Bổ đề 1, ta có thể thay thế $A$ bởi $S^{-1}A$, $A'$ bởi $S^{-1}A'$ (là một $S^{-1}A$-môđun sinh hữu hạn) và $p$ bởi $S^{-1}p$; nói cách khác, ta có thể giả sử rằng $A$ là một vành địa phương và $p$ là iđêan cực đại của nó. Khi đó (theo nhận xét đã nêu ở đầu số này) có thể thay thế $A$ bởi $A/p$, $A'$ bởi $A'/pA'$ và $p$ bởi $(0)$, vì $A'/pA' = (A/p) \otimes_A A'$ là một $(A/p)$-môđun sinh hữu hạn. Vậy cuối cùng ta đã quy bài toán về việc chứng minh mệnh đề trong trường hợp $A$ là một trường và $p = (0)$; khi đó $A'$ là một $A$-đại số hạng hữu hạn và do đó là Artin, và ta biết rằng trong một đại số như vậy chỉ có hữu hạn iđêan nguyên tố (Chương IV, § 2, no. 5, Mệnh đề 9).

### 2. NHÓM PHÂN TÍCH VÀ NHÓM QUÁN TÍNH

#### Định nghĩa 2 {#ac-v-s2-def-2 .statement}

Cho $A'$ là một vành và $G$ là một nhóm tác động lên $A'$ ($§ 1$, no. 9). Với một iđêan nguyên tố $p' \subset A'$, nhóm con gồm các phần tử $\sigma \in G$ sao cho $\sigma.p' = p'$ được gọi là nhóm phân tích của $p'$ (đối với $G$) và được ký hiệu là $G^z(p')$. Vành các phần tử của $A'$ bất biến dưới $G^z(p')$ được gọi là vành phân tích của $p'$ (đối với $G$) và được ký hiệu là $A^z(p')$ (*).

Ta thường viết $G^z$ và $A^z$ thay cho $G^z(p')$ và $A^z(p')$ tương ứng, khi không có sự nhập nhằng.

Với mọi $\sigma \in G^z(p')$, ta cũng ký hiệu bởi $z \mapsto \sigma.z$ tự đồng cấu của vành $A'/p'$ suy ra từ tự đồng cấu $x \mapsto \sigma.x$ của $A'$ bằng cách lấy thương; rõ ràng nhóm $G^z(p')$ tác động theo cách đó lên vành $A'/p'$.

#### Định nghĩa 3 {#ac-v-s2-def-3 .statement}

Với ký hiệu của Định nghĩa 2, nhóm con của $G^z(p')$ gồm những $\sigma$ sao cho tự đồng cấu $z \mapsto \sigma.z$ của $A'/p'$ là đồng nhất được gọi là nhóm quán tính của $p'$ (đối với $G$) và được ký hiệu là $G^T(p')$ (hoặc $G^T$). Vành các phần tử của $A'$ bất biến dưới $G^T(p')$ được gọi là vành quán tính của $p'$ (đối với $G$) và được ký hiệu là $A^T(p')$ (hoặc $A^T$) (†).

Nếu $A$ là vành con của $A'$ gồm các phần tử bất biến của $G$, thì rõ ràng

$$
A \subset A^z(p') \subset A^T(p') \subset A'.
$$

Suy ra từ các Định nghĩa 2 và 3 rằng, với mọi $p \in G$,

$$
G^z(\rho.p') = \rho G^z(p') \rho^{-1}, \quad G^T(\rho.p') = \rho G^T(p') \rho^{-1}.
$$

Nếu, với mọi $\sigma \in G^z(p')$, $\bar{\sigma}$ là tự đẳng cấu $z \mapsto \sigma.z$ của $A'/p'$, thì $\sigma \mapsto \bar{\sigma}$ là một đồng cấu (gọi là chính tắc) từ $G^z$ đến nhóm $\Gamma_0$ các tự đẳng cấu của

(*) Chữ cái $Z$ là chữ cái đầu của từ tiếng Đức "Zerlegung" có nghĩa là "phân tích."
(†) Chữ cái T là chữ cái đầu của từ tiếng Đức "Tragheit" có nghĩa là "quán tính."

A'/p' làm bất biến các phần tử của $A^{\mathbf{Z}}/(p' \cap A^{\mathbf{Z}})$ (được đồng nhất một cách chính tắc với một vành con của $A'/p'$) và theo định nghĩa $\mathcal{G}^{\Gamma}(p')$ là hạt nhân của đồng cấu chính tắc này; do đó $\mathcal{G}^{\Gamma}$ là một nhóm con chuẩn của $\mathcal{G}^{\mathbf{Z}}$. Nếu $k'$ là trường phân thức của $A'/p'$, mọi tự đẳng cấu của $A'/p'$ có thể được mở rộng duy nhất thành một tự đẳng cấu của $k'$, sao cho $\sigma \mapsto \bar{\sigma}$ có thể được xem như một đồng cấu từ $\mathcal{G}^{\mathbf{Z}}(p')$ vào nhóm các tự đẳng cấu của $k'$. Cuối cùng chú ý rằng, vì $\mathcal{G}^{\Gamma}$ là chuẩn trong $\mathcal{G}^{\mathbf{Z}}$, $A^{\Gamma}$ là ổn định dưới tác động của $\mathcal{G}^{\mathbf{Z}}$.

#### Bổ đề 3 {#ac-v-s2-lem-3 .statement}

*Cho $A'$ là một vành, $\mathcal{G}$ là một nhóm tác động trên $A'$, $A$ là vành các bất biến của $\mathcal{G}$, $p'$ là một iđêan nguyên tố của $A'$ và $S$ là một tập con nhân của $A$ không giao với $p'$. Khi đó $\mathcal{G}^{\mathbf{Z}}(S^{-1}p') = \mathcal{G}^{\mathbf{Z}}(p')$, $\mathcal{G}^{\Gamma}(S^{-1}p') = \mathcal{G}^{\Gamma}(p')$ và, nếu $\mathcal{G}$ là hữu hạn địa phương, $S^{-1}A^{\mathbf{Z}}(p') = A^{\mathbf{Z}}(S^{-1}p')$ và $S^{-1}A^{\Gamma}(p') = A^{\Gamma}(S^{-1}p')$.*

Vì các phần tử của $S$ là bất biến dưới $\mathcal{G}$, rõ ràng rằng, nếu $\sigma.p' = p'$, thì cũng có $\sigma.(S^{-1}p') = S^{-1}p'$. Ngược lại, giả sử rằng $\sigma \in \mathcal{G}$ sao cho $\sigma.(S^{-1}p') = S^{-1}p'$; khi đó, nếu $x \in p'$, $(\sigma.x)/1 \in S^{-1}p'$ và do đó tồn tại $s \in S$ sao cho $s(\sigma.x) \in p'$, do đó $\sigma.x \in p'$ vì $p'$ là nguyên tố và $s \notin p'$; điều này chứng minh rằng $\sigma.p' \subset p'$ và tương tự có thể chứng minh rằng $\sigma^{-1}.p' \subset p'$, suy ra $\sigma.p' = p'$ và $\sigma \in \mathcal{G}^{\mathbf{Z}}(p')$. Nếu $\sigma \in \mathcal{G}^{\Gamma}(p')$, thì $\sigma.x - x \in p'$ với mọi $x \in A'$, do đó cũng vậy, với mọi $s \in S$,

$$
\sigma.(x/s) - (x/s) = (O.x - x)/s \in S^{-1}p'
$$

và do đó $\sigma \in \mathcal{G}^{\Gamma}(S^{-1}p')$. Ngược lại, giả sử rằng $\sigma \in \mathcal{G}^{\Gamma}(S^{-1}p')$; khi đó, với mọi $x \in A'$, $\sigma.(x/1) - (x/1) \in S^{-1}p'$ và do đó tồn tại $s \in S$ sao cho $s(\sigma.x - x) \in p'$, do đó như trên $\sigma.x - x \in p'$, điều này chứng minh rằng $\sigma \in \mathcal{G}^{\Gamma}(p')$. Hai khẳng định cuối cùng suy ra từ § 1, no. 9, Mệnh đề 23.

#### Định lý 2 {#ac-v-s2-thm-2 .statement}

*Cho $A'$ là một vành, $\mathcal{G}$ là một nhóm hữu hạn tác động trên $A'$ và $A$ là vành các phần tử bất biến của $\mathcal{G}$, sao cho $A'$ là nguyên trên $A$ (§ 1, no. 9, Mệnh đề 22).*

(i) *Cho hai iđêan nguyên tố $p', q'$ của $A'$ nằm trên cùng một iđêan nguyên tố $p$ của $A$, tồn tại $\sigma \in \mathcal{G}$ sao cho $q' = \sigma.p'$; nói cách khác, $\mathcal{G}$ tác động bắc cầu trên tập hợp các iđêan nguyên tố của $A'$ nằm trên $p$.*

(ii) *Cho $p'$ là một iđêan nguyên tố của $A'$, $p = p' \cap A$ và $k$ (resp. $k'$) là trường phân thức của $A/p$ (resp. $A'/p'$). Khi đó $k'$ là một mở rộng quasi-Galois (*) của $k$ và đồng cấu chính tắc $\sigma \mapsto \bar{\sigma}$ từ $\mathcal{G}^{\mathbf{Z}}(p')$ vào nhóm $\Gamma$ các tự đồng cấu $k$ của $k'$ xác định, bằng cách lấy thương, một đẳng cấu của $\mathcal{G}^{\mathbf{Z}}(p')/\mathcal{G}^{\Gamma}(p')$ lên $\Gamma$.*

(*) Để tránh nhầm lẫn với các nghĩa khác của từ "normal", từ nay về sau chúng ta dùng thuật ngữ "mở rộng quasi-Galois" đồng nghĩa với thuật ngữ "mở rộng normal" được định nghĩa trong Đại số, Chương V, § 6, no. 2, Định nghĩa 2.

(i) Nếu $x \in \mathfrak{q}$ thì $\prod_{\sigma \in \mathcal{G}} \sigma.x \in q' \cap A = p \subset p'$; khi đó tồn tại $\sigma \in \mathcal{G}$ sao cho $\sigma.x \in p'$, tức là $x \in \sigma^{-1}.q'$. Ta kết luận rằng $q' \subset \bigcup_{\sigma \in \mathcal{G}} \mathfrak{s}.\mathfrak{p}'$ và do đó (vì $\mathcal{G}$ là hữu hạn và các $\mathfrak{s}.\mathfrak{p}'$ nguyên tố) tồn tại $\sigma \in \mathcal{G}$ sao cho $\mathfrak{q}' \subset \mathfrak{s}.\mathfrak{p}'$ (Chương II, § 1, no. 1, Mệnh đề 2); vì $q'$ và $\sigma.\mathfrak{p}'$ đều nằm trên $p$, nên $q' = \sigma.\mathfrak{p}'$ (no. 1, Hệ quả 1 của Mệnh đề 1).

(ii) Để thấy rằng $k'$ là một mở rộng quasi-Galois của $k$, chỉ cần chứng minh rằng mọi phần tử $\bar{x} \in A'/p'$ đều là nghiệm của một đa thức $P$ trong $k[X]$ mà tất cả các nghiệm của nó đều nằm trong $A'/p'$ (Algebra, Chương V, § 6, no. 3, Hệ quả 3 của Mệnh đề 9). Bây giờ, lấy $x \in A'$ là một đại diện của lớp $\bar{x}$; đa thức $Q(X) = \prod_{\sigma \in \mathcal{G}} (X - \sigma.x)$ có tất cả các hệ số của nó trong $A$; gọi $P(X)$ là đa thức trong $(A/p)[X]$ mà các hệ số là ảnh của các hệ số của $Q$ qua đồng cấu chính tắc $\pi : A \to A/p$. Vì $\pi$ có thể được xem là hạn chế vào $A$ của đồng cấu chính tắc $\pi' : A' \to A'/p'$, ta thấy rằng $P$ là tích trong $(A'/p')[X]$ của các nhân tử tuyến tính $X - \pi'(\sigma.x)$ và do đó giải quyết bài toán vì $\bar{x} = \pi'(x)$.

Rõ ràng, với mọi $\sigma \in \mathcal{G}^z$, $\hat{\sigma}$ là một $k$-tự đẳng cấu của $k'$; còn phải kiểm tra rằng ánh xạ $\sigma \mapsto \hat{\sigma}$ biến $\mathcal{G}^z$ lên nhóm tất cả các $k$-tự đẳng cấu của $k'$. Ta viết $S = A - p$; $k$ và $k'$ không thay đổi khi thay thế $A'$ và $p'$ lần lượt bởi $S^{-1}A'$ và $S^{-1}p'$, theo § 1, no. 9, Mệnh đề 23 và quan hệ $S^{-1}p' \cap S^{-1}A = S^{-1}(A \cap p') = S^{-1}p$ (chương 11, § 2, no. 4); từ Bổ đề 3 suy ra rằng cả $\mathcal{G}^z$ lẫn phép toán của nó trên $k'$ đều không thay đổi; do đó ta có thể chỉ xét trường hợp $p$ là cực đại, trong trường hợp này ta biết rằng $p'$ cũng vậy (no. 1, Mệnh đề 1) và mọi phần tử của $k'$ do đó đều có dạng $\pi'(x)$ với một $x \in A'$ nào đó; ở trên đã thấy rằng một phần tử như vậy là một nghiệm của một đa thức trong $k[X]$ có bậc $\leq \mathrm{Card}(\mathcal{G})$. Vì mọi mở rộng tách được hữu hạn của $k$ đều nhận một phần tử nguyên thủy (Đại số, chương V, § 7, no. 7, Mệnh đề 12 và § 11, no. 4, Mệnh đề 4), ta thấy rằng mọi mở rộng tách được hữu hạn của $k$ được chứa trong $k'$ đều có bậc $\leq \mathrm{Card}(\mathcal{G})$, do đó suy ra rằng mở rộng tách được lớn nhất $k'_s$ của $k$ được chứa trong $k'$ (Đại số, chương V, § 7, no. 6, Mệnh đề 11) có bậc $\leq \mathrm{Card}(\mathcal{G})$ (Đại số, chương V, § 3, no. 2, Nhận xét 2). Cho $y \in A'$ là một phần tử sao cho $\pi'(y)$ là một phần tử nguyên thủy của $k'_s$. Các iđêan $\sigma.p'$ với $\sigma \in \mathcal{G} - \mathcal{G}^z$ là cực đại và phân biệt với $p'$ theo định nghĩa; do đó tồn tại $x \in A'$ sao cho $x \equiv y \pmod{p'}$ và $x \in \sigma^{-1}p'$ với $\sigma \in \mathcal{G} - \mathcal{G}^z$ (chương 11, § 1, no. 2, Mệnh đề 5). Như vậy, cho $u$ là một $k$-tự đẳng cấu của $k'$ và cho $P(X) = \prod_{\sigma \in \mathcal{G}} (X - \pi'(\sigma.x))$; vì $\pi'(x)$ là một nghiệm của $P$ và $P \in k[X]$, $u(\pi'(x))$ cũng là một nghiệm của $P$ trong $k'$ và do đó tồn tại $\tau \in \mathcal{G}$ sao cho

$$
u(\pi'(x)) = \pi'(\tau.x);
$$

nhưng $u(\pi'(x)) \neq 0$ và, với $\sigma \in \mathcal{G} - \mathcal{G}^z$, $\sigma.x \in p'$ và do đó $\pi'(\sigma.x) = 0$; ta kết luận rằng tất yếu $\tau \in \mathcal{G}^z$. Nhưng vì $u$ và $\tilde{\tau}$ có cùng giá trị đối với phần tử nguyên thủy $\pi'(y) = \pi'(x)$ của $k'_s$, chúng trùng nhau trên $k'_s$ và, vì $k'$ là một mở rộng xuyên căn của $k'_s$, chúng trùng nhau trên $k'$.

#### Hệ quả {#ac-v-s2-n2-cor-1 .statement}

*Với các giả thiết và ký hiệu của Định lý 2, cho $f_1, f_2$ là hai đồng cấu của $A$ vào một trường $L$ có cùng hạn chế trên $A$. Khi đó tồn tại $\sigma \in \mathcal{G}$ sao cho*

$$
f_2(x) = f_1(\sigma.x)
$$

*đối với mọi* $x \in A'$.

Cho $p'_i$ là hạt nhân của $f_i$ ($i = 1, 2$), đó là một iđêan nguyên tố của $A'$; theo giả thiết $p'_1 \cap A = p'_2 \cap A$ và giao này là một iđêan nguyên tố $p$ của $A$; do đó tồn tại $\tau \in \mathcal{G}$ sao cho $\tau.p'_2 = p'_1$ (Định lý 2 (i)); bằng cách thay thế $f_1$ bởi đồng cấu $x \mapsto f_1(\tau.x)$ khi đó ta có thể giả sử rằng $p'_2 = p'_1$ (một iđêan mà ta sẽ ký hiệu là $p'$). Khi lấy thương, từ $f_1$ và $f_2$ ta suy ra được hai đồng cấu đơn ánh $f'_1, f'_2$ từ $A'/p'$ vào $L$, vì thế mở rộng thành hai đồng cấu đơn ánh $f''_1, f''_2$ từ trường phân thức $k'$ của $A'/p'$ vào $L$. Vì $k'$ là một mở rộng quasi-Galois của $k$, nên $k''_1 = f''_1(k')$ và $k''_2 = f''_2(k')$ cũng vậy ($k$ được đồng nhất với một trường con của $L$) và, vì có một k-đẳng cấu từ $k''_1$ lên $k''_2$, nên $k''_1 = k''_2$ (*Algebra*, Chương V, § 6, Mệnh đề 6). Do đó $f''_1 \circ {f''_2}^{-1}$ là một k-tự đẳng cấu của $k'$; bởi Định lý 2 (ii) vì thế nó có dạng 6, trong đó $\sigma \in \mathcal{G}^z(p')$. Đặc biệt, với mọi $x \in A'$ các phần tử $f_2(x)$ và $f_1(\sigma.x)$ là bằng nhau.

**Nhận xét**

(1) Chú ý rằng dưới các giả thiết của Định lý 2, $k'$ có thể là *vô hạn* trên $k$ nếu $k'$ không tách được trên $k$ (Bài tập 9).

(2) Rõ ràng $k$ là một mở rộng *Galois* của $k$ nếu trường $k$ là *hoàn hảo*. Khi đó nó hữu hạn trên $k$.

#### Mệnh đề 4 {#ac-v-s2-prop-4 .statement}

*Cho $A'$ là một vành, $\mathcal{G}$ là một nhóm hữu hạn tác động trên $A'$, $\mathcal{H}$ là một nhóm con của $\mathcal{G}$, $A$ và $B$ lần lượt là các vành bất biến của $\mathcal{G}$ và $\mathcal{H}$, và $p'$ là một iđêan nguyên tố của $A$; viết $p = A \cap p'$ và $p(B) = B \cap p'$.

(i) Để $\mathcal{H}$ được chứa trong nhóm phân tích $\mathcal{G}^z(p')$, điều kiện cần và đủ là $p'$ là iđêan nguyên tố duy nhất của $A$ nằm trên $p(B)$.

(ii) *Nếu $\mathcal{H}$ chứa $\mathcal{G}^z(p')$, thì các điều kiện sau được thỏa mãn*:
(a) *Các vành $A/p$ và $B/p(B)$ có cùng trường phân thức*.
(b) *Iđêan cực đại của vành địa phương $B_{p(B)}$ bằng $pB_{p(B)}$*.

(iii) *Giả sử thêm rằng $A'$ là một miền nguyên và $\bigcap_{n \geq 0} p^nA'_p = 0$; khi đó các điều kiện (a) và (b) của (ii) kéo theo rằng $\mathcal{G}^z(p')$ bất biến các phần tử của $B$*.

(i) Từ Định lý 2 (i) suy ra rằng các iđêan nguyên tố của $A$ nằm trên $p(B)$ là các iđêan có dạng $\sigma.p'$, trong đó $\sigma \in \mathcal{H}$; do đó ngay lập tức được (i).

(ii) Ta viết $S = A - p$; ta biết rằng các vành bất biến của $\mathcal{G}$ và $\mathcal{H}$ trong $S^{-1}A'$ lần lượt là $S^{-1}A$ và $S^{-1}B$ (§ 1, no. 9, Mệnh đề 23) và $\mathcal{G}^{\mathbf{Z}}(S^{-1}p) = \mathcal{G}^{\mathbf{Z}}(p')$ (Bổ đề 3); sau cùng $S^{-1}p(B) = S^{-1}p' \cap S^{-1}B$ (Chương II, § 2, no. 4), vành địa phương của iđêan nguyên tố $S^{-1}p(B)$ của vành $S^{-1}B$ đẳng cấu chính tắc với $B_{p(B)}$ và trường thặng dư của nó đẳng cấu với trường phân thức của $B/p(B)$ (Chương II, § 2, no. 5, Mệnh đề 11). Do đó ta có thể chứng minh (ii) bằng cách chỉ xét trường hợp $p$ là cực đại. Để thiết lập (a), sẽ đủ để chứng minh rằng

$$
B = A + p(B)
$$

vì điều này sẽ cho thấy rằng các trường $A/p$ và $B/p(B)$ là *đẳng cấu chính tắc*. Theo Định lý 2 chỉ có một số hữu hạn iđêan nguyên tố của $A'$ nằm trên $p$ và theo Định lý 1 của no. 1 thì có ít nhất một iđêan nguyên tố của $A'$ nằm trên mỗi iđêan nguyên tố của $B$; điều đó suy ra rằng chỉ có một số *hữu hạn* iđêan nguyên tố của $B$ nằm trên $p$; gọi $n_j$ ($1 \leq j \leq r$) là những iđêan trong số đó mà $\neq p(B)$. Cho $x$ là một phần tử của $B$; vì các iđêan $p(B)$ và $n_j$ đều cực đại (no. 1, Mệnh đề 1), nên tồn tại $y \in B$ sao cho $y \equiv x$ (mod. $p(B)$) và $y \in n_j$ với $1 \leq j \leq r$ (Chương 11, § 1, no. 2, Mệnh đề 5). Cho $y_1 = y, y_2, \ldots, y_q$ là các phần tử phân biệt của quỹ đạo của $y$ dưới tác động của $\mathcal{G}$; rõ ràng

$$
z = y_1 + y_2 + \cdots + y_q \in A,
$$

và để thiết lập (3), chỉ cần chỉ ra rằng $y_i \in p'$ với $i \geq 2$, vì khi đó ta sẽ suy ra rằng $z - y \in p' \cap B = p(B)$, do đó $x \in A + p(B)$ vì $x \equiv y$ (mod. $p(B)$). Xét $i \geq 2$ và $\sigma \in \mathcal{G}$ sao cho $\sigma.y = y_i$; ta chỉ ra rằng $\sigma^{-1}.p'$ không nằm trên $p(B)$. Thật vậy, nếu ngược lại thì sẽ tồn tại $\tau \in \mathcal{H}$ sao cho $\sigma^{-1}.p' = \tau.p'$ (Định lý 2 (i)), do đó $(\tau^{-1}\sigma^{-1}).p' = p'$, nói cách khác $\tau^{-1}\sigma^{-1} \in \mathcal{G}^{\mathbf{Z}} \subset \mathcal{H}$ theo giả thiết, do đó $\sigma \in \mathcal{H}$; nhưng vì $y \in B$ và $\sigma.y \neq y$, điều này là vô lý. Ta kết luận rằng $\sigma^{-1}.p'$ nằm trên một trong các iđêan $n_j$ và, vì $y \in n_j$ theo phép dựng, chắc chắn $y \in \sigma^{-1}.p'$ hay $y_i = \sigma.y \in p'$.

Để chứng minh (b), chỉ cần thiết lập rằng $p(B)$ được chứa trong *bão hòa* $q$ của iđêan $pB$ đối với $p(B)$ (Chương II, § 2, no. 4, Mệnh đề 10); vì $p(B)$ không được chứa trong iđêan nào trong các $n_j$ ($1 \leq j \leq r$), thậm chí chỉ cần chứng minh rằng

$$
p(B) \subset q \cup n_1 \cup \cdots \cup n_r
$$

theo Chương II, § 1, no. 1, Mệnh đề 2. Để làm điều này, ta xét một phần tử $u \in p(B)$ không thuộc bất kỳ $n_j$ nào ($1 \leq j \leq r$) (Chương 11, § 1, no. 1, Mệnh đề 2); gọi $u_1 = u, u_2, \ldots, u_m$ là các phần tử phân biệt của quỹ đạo của $u$ dưới tác dụng của $\mathcal{G}$; ta viết $w = u_1u_2 \ldots u_m, v = u_2 \ldots u_m$; rõ ràng $w \in A$; mặt khác, nếu $\tau \in \mathcal{H}$, thì $\tau.u = u$ và do đó tất yếu $\tau.u_i \neq u$ với $i \geq 2$, điều này cho thấy $\tau.v = v$ và vì thế $v \in B$. Có thể chứng minh như trong chứng minh của (a) rằng, nếu $\sigma \in \mathcal{G}$ sao cho $\sigma.u = u_i$ với $i \geq 2$, thì $\sigma^{-1}.p'$ nằm trên một trong các $n_j$ và, do $u \notin n_j$, nên cũng có $u \notin \sigma^{-1}.p'$, nói cách khác $u_i \notin p'$. Ta kết luận rằng $v \notin p'$ và do đó $v \notin p(B)$. Mặt khác rõ ràng $w \in p' \cap A = p$ và quan hệ $w = uv$ cho thấy rằng $u$ nằm trong bão hòa của $pB$ đối với $p(B)$ và do đó thiết lập được (4).

(iii) Giả sử rằng $A'$ là một miền nguyên, rằng $\bigcap_{n \geq 0} p^n A'_p = 0$ và các điều kiện (a) và (b) của (ii) được thỏa mãn. Với cùng ký hiệu như trong (ii), rõ ràng $S^{-1}A'$ là một miền nguyên và $S^{-1}A'_p = A'_p$; do đó có thể thay thế $A'$ và $p'$ bởi $S^{-1}A'$ và $S^{-1}p'$, nói cách khác, giả sử thêm rằng iđêan $p$ là cực đại. Khi đó các giả thiết (a) và (b) kéo theo rằng

$$
\mathbf{B}_{p(B)} = A + p \mathbf{B}_{p(B)}
$$

Bằng quy nạp theo $n$ ta suy ra rằng $\mathbf{B}_{p(B)} = A + p^n \mathbf{B}_{p(B)}$ với mọi $n > 0$. Khi đó lấy $\sigma$ là một phần tử của $\mathcal{G}^\mathbf{Z}$ và $x$ là một phần tử của $B$. Với mọi $n > 0$, tồn tại $a_n \in A$ sao cho $x - a_n \in p^n \mathbf{B}_{p(B)} \subset p^n A'_p$; vì $\sigma.a_n = a$, và $\sigma.p' = p'$, ta suy ra rằng $\sigma.x - x \in p^n A'_p$. Vì quan hệ này đúng với mọi $n$, ta kết luận từ giả thiết rằng $\sigma.x = x$.

h a r k s

(3) Nếu $A'$ là một miền nguyên và Noether, thì điều kiện $\bigcap_{n \geq 1} p^n A'_p = 0$ luôn luôn được thỏa mãn (Chương III, § 3, no. 2, Hệ quả của Mệnh đề 5). Có thể chứng minh rằng điều kiện này cũng được thỏa mãn nếu giả sử $A'$ là một miền nguyên và $A$ là Noether.

(4) Nếu $p$ không phải là một iđêan cực đại của $A$ thì quan hệ (3) không nhất thiết đúng dưới các giả thiết của (ii) và do đó $A/p$ và $B/p(B)$ không nhất thiết đẳng cấu, ngay cả nếu ta lấy $\mathcal{H} = \mathcal{G}^\mathbf{Z}$, do đó $B = A''$ (Bài tập 10).

#### Hệ quả 1 {#ac-v-s2-prop-4-cor-1 .statement}

Dưới các giả thiết của Định lý 2, các vành $A/p$ và $A^\mathbf{Z}/(p' \cap A^\mathbf{Z})$ có cùng trường phân thức và iđêan cực đại của vành địa phương $(A^\mathbf{Z})'_{p' \cap A^\mathbf{Z}}$ được sinh bởi $p$.

#### Hệ quả 2 {#ac-v-s2-prop-4-cor-2 .statement}

Cho $A'$ là một miền nguyên, $\mathcal{G}$ là một nhóm hữu hạn tác động lên $A'$, $A'$ là vành bất biến của $\mathcal{G}$ và $p'$ là một iđêan nguyên tố của $A'$; gọi $K, K^\mathbf{Z}$ và $K$ là các trường phân thức của $A, A^\mathbf{Z}$ và $A'$ tương ứng. Khi đó $K'$ là một mở rộng Galois của $K$ và các trường con $L$ của $K$ chứa $K$ và sao cho $p'$ là iđêan nguyên tố duy nhất của $A'$ nằm trên iđêan $p' \cap L$ của $A' \cap L$ chính là những trường chứa $K^\mathbf{Z}$.

$\mathcal{G}$ tác động trên $K'$ và $K$ là trường bất biến của $\mathcal{G}$ trong $K'$ (§ 1, no. 9, Mệnh đề 23 áp dụng cho $S = A - \{0\}$) và tương tự $K^\mathbf{Z}$ là trường bất biến của $\mathcal{G}^\mathbf{Z}$; do định nghĩa, $K'$ vì thế là một mở rộng Galois của $K$. Nếu nhóm con của $\mathcal{G}$ gồm những $\sigma \in \mathcal{G}$ để bất biến các phần tử của L, thì việc nói rằng L chứa $K^{\mathbf{Z}}$ có nghĩa là $\mathcal{H}$ được chứa trong $\mathcal{G}^{\mathbf{Z}}$ (Đại số, Chương V, § 10, no. 5, Định lý 3) và, vì L là trường bất biến của $\mathcal{H}$ trong $K'$, $A' \cap L$ là vành bất biến của $\mathcal{H}$ trong $A'$; khi đó mệnh đề thứ hai suy ra từ Mệnh đề 4 (i).

#### Định nghĩa 4 {#ac-v-s2-def-4 .statement}

*Với các giả thiết và ký hiệu của Hệ quả 2 của Mệnh đề 4, một iđêan nguyên tố $\mathfrak{p}$ của $A$ được gọi là phân tích hoàn toàn trong $K'$ nếu số các iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}$ bằng $[K':K]$.*

Điều đó cũng tương đương với việc nói rằng, đối với một iđêan nguyên tố $\mathfrak{p}'$ của $A'$ nằm trên $\mathfrak{p}$, nhóm con $\mathcal{G}^{\mathbf{Z}}(\mathfrak{p}')$ bằng nhóm con $\mathcal{M}$ để bất biến mọi phần tử của $A'$, hoặc rằng $A^{\mathbf{Z}}(\mathfrak{p}') = A'$, hoặc rằng $\mathcal{G}/\mathcal{M}$ tác động trung thành trên tập hợp các iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}$.

#### Hệ quả 3 {#ac-v-s2-def-4-cor-3 .statement}

*Cho $A'$ là một miền nguyên, $\mathcal{G}$ là một nhóm giao hoán hữu hạn tác động trên $A'$, $A$ là vành các phần tử bất biến của $\mathcal{G}$, $\mathfrak{p}$ là một iđêan nguyên tố của $A$ và $K$ và $K'$ lần lượt là các trường phân thức của $A$ và $A'$. Khi đó các iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}$ đều có cùng vành phân tích $A^{\mathbf{Z}}$ và trường phân thức $K^{\mathbf{Z}}$ của $A^{\mathbf{Z}}$ là trường trung gian lớn nhất giữa $K$ và $K'$ mà trong đó $\mathfrak{p}$ phân tích hoàn toàn.*

Nếu $\mathfrak{p}'$ là một iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}$, thì $\mathcal{G}^{\mathbf{Z}}(\sigma.\mathfrak{p}') = \mathcal{G}^{\mathbf{Z}}(\mathfrak{p}')$ vì $\mathcal{G}$ là giao hoán (công thức (2)); do đó (Định lý 2 (i)) tất cả các iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}$ đều có cùng nhóm phân tích $\mathcal{G}^{\mathbf{Z}}$ và vì thế cùng vành phân tích $A^{\mathbf{Z}}$; số của chúng là $(\mathcal{G}:\mathcal{G}^{\mathbf{Z}})$. Cho L là một trường trung gian giữa K và $K'$, và cho $\mathcal{H}$ là nhóm con của $\mathcal{G}$ làm bất biến các phần tử của L; nhóm phân tích của $\mathfrak{p}'$ đối với $\mathcal{H}$ là $\mathcal{G}^{\mathbf{Z}} \cap \mathcal{H}$; vì $A' \cap L$ là vành các bất biến của $\mathcal{H}$ trong $A'$, nên số các iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}' \cap L$ là $(\mathcal{H}:(\mathcal{G}^{\mathbf{Z}} \cap \mathcal{H})) = (\mathcal{H}\mathcal{G}^{\mathbf{Z}}:\mathcal{G}^{\mathbf{Z}})$ (vì $\mathcal{G}$ là giao hoán). Vậy số các iđêan nguyên tố của $A' \cap L$ nằm trên $\mathfrak{p}$ là $(\mathcal{G}:\mathcal{H}\mathcal{G}^{\mathbf{Z}})$. Để $\mathfrak{p}$ phân tích hoàn toàn trong L, điều kiện cần và đủ do đó là $(\mathcal{G}:\mathcal{H}\mathcal{G}^{\mathbf{Z}}) = [L:K] = (\mathcal{G}:\mathcal{H})$ và, vì $\mathcal{H} \subset \mathcal{H}\mathcal{G}^{\mathbf{Z}}$, điều này tương đương với $\mathcal{H}\mathcal{G}^{\mathbf{Z}} = \mathcal{H}$ hoặc cũng tương đương với $\mathcal{G}^{\mathbf{Z}} \subset \mathcal{H}$ và cuối cùng với $L \subset K^{\mathbf{Z}}$.

#### Mệnh đề 5 {#ac-v-s2-prop-5 .statement}

*Với các giả thiết và ký hiệu của Định lý 2, trường các phân thức $k^T$ của $A^T/(\mathfrak{p}' \cap A^T)$ bằng với mở rộng tách được lớn nhất $k'_s$ của $k$ được chứa trong $k'$.*

Như trong Mệnh đề 4, điều này có thể được quy về trường hợp $\mathfrak{p}$ là một iđêan cực đại của $A$, điều đó kéo theo rằng $\mathfrak{p}'$, $\mathfrak{p}' \cap A^{\mathbf{Z}}$ và $\mathfrak{p}' \cap A^T$ lần lượt là cực đại trong $A'$, $A^{\mathbf{Z}}$ và $A^T$ (no. 1, Mệnh đề 1).

Với mọi $x \in A'$, đa thức $P(X) = \prod_{\sigma \in \mathcal{G}^T} (X - \sigma.x)$ có các hệ số trong vành quán tính $A^T$ và, theo định nghĩa của $\mathcal{G}^T$, mọi nghiệm của nó trong $A'$ đều đồng dư mod. $\mathfrak{p}'$; do đó đa thức $\pi'(P)$ trên $A^T/(\mathfrak{p}' \cap A^T)$ mà các hệ số là các ảnh chính tắc của các hệ số của P dưới đồng cấu $\pi':A' \to A'/\mathfrak{p}'$ có mọi nghiệm của nó trong $A'/\mathfrak{p}'$ bằng ảnh của $x$, điều này cho thấy rằng $k'$ là một mở rộng căn của $k^T$; do đó $k'_s \subset k^T$, vì mọi phần tử của $k'_s$ đều tách được trên k và a fortiori trên $k^T$.

Ta biết rằng $k'_s$ là một mở rộng Galois của k (Đại số, Chương V, § 10, no. 9, Mệnh đề 14) và từ Định lý 2 suy ra rằng nhóm Galois của nó đẳng cấu với $\mathcal{G}' = \mathcal{G}^z / \mathcal{G}^T$. Vì $k^T$ là một mở rộng căn của $k'_s$, $k^T$ là một mở rộng giả Galois của k và nhân tử tách được của bậc của $k^T$ trên k là $q = (\mathcal{G}^z : \mathcal{G}^T )$. Còn phải thấy rằng $k^T$ là một mở rộng tách được của k. Ta đã thấy ở trên rằng $\mathcal{G}'$ được đồng nhất với một nhóm tự đẳng cấu của $A^T$ và rằng $A^z$ là vành các bất biến của $\mathcal{G}'$. Nếu $x \in A^T$, thì đa thức $Q(X) = \prod_{\sigma' \in \mathcal{G}'} (X - \sigma'(x))$ do đó có các hệ số trong $A^z$; đa thức trên $A^z / (p' \cap A^z)$ mà các hệ số là các ảnh của các hệ số của Q dưới $\pi'$ có bậc $q$ và có một nghiệm $\pi'(x) \in A^T / (p' \cap A^T )$. Vì $A^z / (p' \cap A^z) = k$ theo Mệnh đề 4 (ii), ta thấy rằng mọi phần tử của $k^T$ đều có bậc $\leq q$ trên k.

Như vậy, gọi k, là trường bất biến của nhóm các k-tự đẳng cấu của mở rộng tựa Galois $k^T$ của $k$; khi đó $[k^T : k_1] = q$ (Đại số, Chương V, § 10, no. 9, Mệnh đề 14). Gọi $u$ là một phần tử nguyên thủy của $k^T$ trên $k_1$; vì nó có bậc $q$ trên $k_1$, và có bậc $\leq q$ trên k, nên nó có bậc $q$ trên k và đa thức tối tiểu của nó trên k, có các hệ số trong $k$; điều này cho thấy rằng $u$ tách được trên k. Mặt khác, với mọi $v \in k_1$, tồn tại một lũy thừa $p'$ của số mũ đặc số p sao cho $v^{p'} \in k$. Ta kết luận rằng $k(u - v)$, chứa
$$
(u - v)^{p'} = u^{p'} - v^{p'},
$$
chứa $u^{p'}$ và do đó chứa $k(u^{p'})$. Nhưng vì $u$ tách được trên $k$, nên $k(u) = k(u^{p'})$ (Đại số, Chương V, § 8, no. 3, Mệnh đề 4), do đó $k(u) \subset k(u - v)$. Vì $u$ có bậc $q$ trên k và $u - v$ có bậc $\leq q$, suy ra $k(u) = k(u - v)$, do đó $v \in k(u)$. Điều này cho thấy rằng $v$ tách được trên k, vì thế $k_1 = k$ và $k^T$ tách được trên $k$.

#### Hệ quả {#ac-v-s2-n2-cor-2 .statement}

*Nếu cấp của nhóm quán tính $\mathcal{G}^T(p')$ nguyên tố cùng nhau với số mũ đặc số p của k, thì trường $k'$ là một mở rộng Galois của k.*

Với ký hiệu của chứng minh Mệnh đề 5, đa thức $\pi'(P)$ có các hệ số trong $k^T = k'_s$ và mọi nghiệm của nó đều bằng $\pi'(x)$; ta ngay lập tức suy ra rằng $\pi'(P)$ là một lũy thừa của một đa thức tối tiểu của $\pi'(x)$ trên $k'_s$; nhưng đa thức sau có bậc bằng một lũy thừa của p và vì thế, do bậc của $\pi'(P)$ bằng cấp của $\mathcal{G}^T$, giả thiết kéo theo $\pi'(x) \in k'_s$, nói cách khác $k'_s = k'$.

### 3. PHÂN TÍCH VÀ QUÁN TÍNH ĐỐI VỚI CÁC MIỀN ĐÓNG NGUYÊN

#### Bổ đề 4 {#ac-v-s2-lem-4 .statement}

*Cho A là một miền đóng nguyên, K là trường phân thức của nó, p là số mũ đặc số của K, K' là một mở rộng radicial của K và A' là một vành con của K' chứa A và nguyên trên A. Với mọi iđêan nguyên tố p của A, tồn tại một iđêan nguyên duy nhất* p' của $A'$ nằm trên $p$ và $p'$ là tập hợp các $x \in A'$ sao cho tồn tại một số nguyên $m \geq 0$ mà $x^{p^m} \in p$.

Sự tồn tại của $p'$ suy ra từ no. 1, Định lý 1. Nếu $x \in p'$, thì tồn tại $m \geq 0$ sao cho $x^{p^m} \in K$, do đó $x^{p^m} \in A$ vì $A$ là nguyên đóng, suy ra $x^{p^m} \in p' \cap A = p$. Ngược lại, nếu $x \in A'$ sao cho $x^{p^m} \in p \subset p'$, thì $x \in p$ vì $p'$ là nguyên tố.

Nhận xét (1). Suy ra từ § 1, no. 3, Hệ quả của Mệnh đề 11 rằng bao đóng nguyên của $A$ trong $K'$ là tập hợp các $x \in K'$ sao cho tồn tại $m \geq 0$ mà với nó $x^{p^m} \in A$ (Đại số, Chương V, § 8, no. 1, Mệnh đề 1).

#### Mệnh đề 6 {#ac-v-s2-prop-6 .statement}

Cho $A$ là một miền nguyên đóng, $K$ là trường phân thức của nó, $K'$ là một mở rộng quasi-Galois của $K$ và $A'$ là bao đóng nguyên của $A$ trong $K'$. Khi đó:

(i) Với mọi iđêan nguyên tố $p$ của $A$, nhóm $\mathcal{G}$ các $K$-tự đồng cấu của $K'$ tác động bắc cầu trên tập hợp các iđêan nguyên tố của $A'$ nằm trên $p$.

(ii) Với mọi iđêan nguyên tố $p'$ của $A'$, trường phân thức $k'$ của $A'/p'$ là một mở rộng quasi-Galois của trường phân thức $k$ của $A/(A \cap p')$ và đồng cấu chính tắc $\sigma \mapsto \tilde{\sigma}$ từ $\mathcal{G}^Z(p')$ vào nhóm $\Gamma$ các $k$-tự đồng cấu của $k'$ xác định, bằng cách lấy thương, một song ánh từ $\mathcal{G}^Z(p')/\mathcal{G}^T(p')$ lên $\Gamma$.

(A) Trước hết giả sử rằng $K'$ là một mở rộng Galois ajinite của $K$. Khi đó $A = A \cap K$ vì $A$ là nguyên đóng và do đó $A$ là vành các bất biến của $\mathcal{G}$ trong $A'$. Vì $\mathcal{G}$ là hữu hạn, mệnh đề suy ra trong trường hợp này từ no. 2, Định lý 2.

(B) Bây giờ giả sử thứ hai rằng $K'$ là một mở rộng Galois bất kỳ của $K$. Khi đó $K'$ là hợp của một họ có hướng phải $(K_\alpha)_{\alpha \in I}$ các mở rộng Galois hữu hạn của $K$. Để chứng minh (i), xét hai iđêan nguyên tố $p', q'$ của $A'$ nằm trên $p$. Với mọi $\alpha \in I$, $p' \cap K_\alpha$ và $q' \cap K_\alpha$ là hai iđêan nguyên tố của $A \cap K_\alpha$, nằm trên $p$. Vì $A' \cap K_\alpha$ là bao đóng nguyên của $A$ trong $K_\alpha$, và các hạn chế lên $K_\alpha$ của các phần tử của $\mathcal{G}$ tạo thành nhóm các tự đẳng cấu của $K$ trên $K$, nên từ trường hợp (A) suy ra rằng tồn tại $\sigma \in \mathcal{G}$ sao cho $(\sigma.(p' \cap K_\alpha)) = q' \cap K_\alpha$. Gọi $\mathcal{E}_\alpha$ là tập hợp các $\sigma \in \mathcal{G}$ có tính chất trên. Lấy $\sigma \in \mathcal{G} - 8$; khi đó, với mọi $\tau \in \mathcal{G}$ để bất biến các phần tử của $K_\alpha$, (QT) $(\sigma.(p' \cap K_\alpha)) = \varrho.(p' \cap K_\alpha) \neq q' \cap K_\alpha$, và do đó $\sigma \tau \in \mathcal{G} - b$. Suy ra $\mathcal{E}_\alpha$ là đóng trong nhóm Galois tôpô $\mathcal{G}$ (Đại số, Chương V, Phụ lục 11, no. 1) và rõ ràng họ $(\mathcal{E}_\alpha)_{\alpha \in I}$ là có hướng trái. Vì $\mathcal{G}$ là compáct (loc. cit., no. 2, Proposition 3) và các $\mathcal{E}_\alpha$ là không rỗng, nên giao $\mathcal{E}$ của họ $(8,)$ là không rỗng và $\sigma.p' = q'$ với mọi $\sigma \in \mathcal{E}$, do đó có (i).

Để chứng minh (ii), chú ý rằng $k'$ là hợp của họ có hướng phải $(k_\alpha)_{\alpha \in I}$, trong đó $k_\alpha$ là trường phân thức của $(A' \cap K_\alpha)/(p' \cap K_\alpha)$. Vì mỗi $k_\alpha$ là một mở rộng quasi-Galois của $k$ theo (A), nên $k'$ cũng vậy (*Đại số*, Chương V, § 6, no. 3, Mệnh đề 8). Mặt khác, cho $u$ là một $k$-tự đẳng cấu của $k'$ và gọi $\pi': A' \to A'/p'$ là đồng cấu chính tắc. Theo no. 2, Định lý 2 áp dụng cho $A' \cap K_\alpha$, với mọi $\alpha$ tồn tại một tập hợp không rỗng $F_\alpha$ gồm các phần tử $\sigma \in \mathcal{G}$ sao cho $\sigma.(p' \cap K_\alpha) = p' \cap K_\alpha$ và $u(\pi'(x)) = \pi'(\sigma.x)$ với mọi $x \in A' \cap K_\alpha$. Như trên, ta thấy rằng $\mathcal{F}_\alpha$ đóng trong $\mathcal{G}$ và, vì $(\mathcal{F}_\alpha)$ là một tập có hướng trái, giao của chúng $\mathcal{F}$ là không rỗng. Rõ ràng với $\alpha \in \mathcal{F}$, $\alpha \in \mathcal{G}^\mathbf{Z}(p')$ và $\tilde{\sigma} = u$, điều này hoàn tất chứng minh của (ii) trong trường hợp này.

(C) *Trường hợp tổng quát*. Trường bất biến $K_1$ của $\mathcal{G}$ là một mở rộng radiciel của $K$ (*Đại số*, Chương V, § 10, no. 9, Mệnh đề 14); do đó chỉ tồn tại một iđêan nguyên tố duy nhất $p_1$ của $A_1 = A' \cap K_1$ nằm trên $p$ (Bổ đề 4). Nếu $p'$ và $q'$ là hai iđêan nguyên tố của $A'$ nằm trên $p$, thì chúng nằm trên $p_1$; vì $K'$ là một mở rộng Galois của $K$, và $A' \cap K$, là nguyên đóng (§ 1, no. 2, Mệnh đề 7 và Hệ quả của Mệnh đề 8), nên theo (B) suy ra tồn tại $\sigma \in \mathcal{G}$ sao cho $(1.p' = q'$; do đó có (i). Mặt khác, rõ ràng trường phân thức $k$, của $A_1/p_1$ là một mở rộng radiciel của $k$ (vì A là nguyên đóng); vì $k'$ là một mở rộng quasi-Galois của $k$, theo (B), $k'$ là một mở rộng quasi-Galois của $k$, mọi $k$-đẳng cấu của $k'$ vào một mở rộng đóng đại số của $k'$ đều là một $k_1$-đẳng cấu. Nhận xét cuối cùng này cũng cho thấy, có tính đến (B), rằng mọi $k$-tự đẳng cấu của $k'$ đều có dạng $\tilde{\sigma}$ trong đó $\alpha \in \mathcal{G}^\mathbf{Z}(p')$, điều này hoàn tất chứng minh của (ii).

*Nhận xét*

(2) Giả sử rằng $K$ là một mở rộng *Galois* của $K$ và giữ các ký hiệu của chứng minh Mệnh đề 6; với mọi $a$, đặt $\mathcal{G}_a^\mathbf{Z}$ (tương ứng $\mathcal{G}_a^\mathbf{T}$) là nhóm con của $\mathcal{G}$ gồm các $\sigma$ mà hạn chế của chúng lên $A' \cap K$, thuộc $\mathcal{G}^\mathbf{Z}(p' \cap K_\alpha)$ (tương ứng $\mathcal{G}^\mathbf{T}(p' \cap K_\alpha)$). Chứng minh của Mệnh đề 6 cho thấy rằng các nhóm con này là *đóng* trong $\mathcal{G}$ và rằng
$$
\mathcal{G}^\mathbf{Z}(p') = \bigcap_a \mathcal{G}_a^\mathbf{Z} \quad \text{và} \quad \mathcal{G}^\mathbf{T}(p') = \bigcap_a \mathcal{G}_a^\mathbf{T}.
$$
Hơn nữa, tập hợp các hạn chế lên $A' \cap K$, của các phần tử của $\mathcal{G}$ (tương ứng của $\mathcal{G}_a^\mathbf{T}$) là toàn bộ nhóm $\mathcal{G}^\mathbf{Z}(p' \cap K_\alpha)$ (tương ứng $\mathcal{G}^\mathbf{T}(p' \cap K_\alpha)$), mọi tự đẳng cấu của $K$ trên $K$, đều mở rộng được thành một phần tử của $\mathcal{G}$.

Với cùng các giả thiết ấy, vành $A^\mathbf{Z}(p')$ (tương ứng $A^\mathbf{T}(p')$) là *hợp* của họ có hướng các $A^\mathbf{Z}(p' \cap K_\alpha)$ (tương ứng $A^\mathbf{T}(p' \cap K_\alpha)$); thật vậy, mọi $x \in A^\mathbf{Z}(p')$ (tương ứng mọi $x \in A^\mathbf{T}(p')$) đều thuộc một trong các $K$, và theo trên tồn tại một $\beta$ sao cho $K_\alpha \subset K_\beta$ và các hạn chế lên $A' \cap K$, của các phần tử của $\mathcal{G}^\mathbf{Z}(p')$ (tương ứng $\mathcal{G}^\mathbf{T}(p')$) cũng chính là các hạn chế lên $A' \cap K$, của các phần tử của $\mathcal{G}^\mathbf{Z}(p' \cap K_\beta)$ (tương ứng $\mathcal{G}^\mathbf{T}(p' \cap K_\beta)$), các nhóm $\mathcal{G}^\mathbf{Z}(p' \cap K_\alpha)$ và $\mathcal{G}^\mathbf{T}(p' \cap K_\beta)$ là hữu hạn; do đó $x$ thuộc $A^\mathbf{Z}(p' \cap K_\beta)$ (tương ứng $A^\mathbf{T}(p' \cap K_\beta)$).

#### Hệ quả 1 {#ac-v-s2-prop-6-cor-1 .statement}

*Dưới các giả thiết của Mệnh đề 6, cho f là một đồng cấu từ A vào một trường L và $g_1, g_2$ là hai đồng cấu từ A' vào L mở rộng f. Khi đó tồn tại một tự đẳng cấu của $K$ trên $K'$, $\sigma \in K'$, sao cho $g_1 = g_2 \circ \sigma$.*

Chứng minh suy ra từ Mệnh đề 6 giống như chứng minh của Hệ quả của Định lý 2 suy ra từ định lý sau.

#### Hệ quả 2 {#ac-v-s2-prop-6-cor-2 .statement}

*Cho A là một miền nguyên đóng, K là trường các phân thức của nó, K' là một mở rộng đại số hữu hạn của K và A' là một vành con của K' chứa A và nguyên trên A.*

(i) Với mọi iđêan nguyên tố $\mathfrak{p}$ của $A$, tập hợp các iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}$ là hữu hạn.
(ii) Nếu $\mathfrak{p}'$ là một iđêan nguyên tố của $A'$ nằm trên $\mathfrak{p}$, thì mọi phần tử của $A'/\mathfrak{p}'$ đều có bậc $\leq [\mathbf{K}':\mathbf{K}]$ trên trường các phân thức của $A/\mathfrak{p}$.

(i) Gọi $K''$ là mở rộng quasi-Galois của $K$ sinh bởi $K'$ trong một bao đóng đại số của $K'$ và $A''$ là bao đóng nguyên của $A$ trong $K''$. Trường $K''$ là một mở rộng hữu hạn của $K$ (Đại số, Chương V, § 6, no. 3, Hệ quả 1 của Mệnh đề 9) và do đó nhóm các $K$-tự đẳng cấu của nó là hữu hạn; suy ra tập hợp các iđêan nguyên tố của $A''$ nằm trên $\mathfrak{p}$ là hữu hạn (Mệnh đề 6 (i)). Mặt khác, vì $A''$ là nguyên trên $A$, ánh xạ $\mathfrak{p}'' \mapsto \mathfrak{p}'' \cap A'$ từ tập hợp các iđêan nguyên tố của $A''$ nằm trên $\mathfrak{p}$ tới tập hợp các iđêan nguyên tố của $A'$ nằm trên $x$ là toàn ánh (no. 1, Định lý 1).

(ii) Các hệ số của đa thức tối tiểu (trên $K$) của mọi phần tử $x' \in A'$ đều thuộc $A$ ($§ 1$, no. 3, Hệ quả của Mệnh đề 10); áp dụng đồng cấu chính tắc $\pi': A' \to A'/\mathfrak{p}'$ cho các hệ số của đa thức này, ta thu được đối với lớp modulo $\mathfrak{p}'$ của $x$ một phương trình phụ thuộc nguyên với các hệ số trong $A/\mathfrak{p}$ và bậc $\leq [\mathbf{K}':\mathbf{K}]$; do đó có kết luận.

#### Hệ quả 3 {#ac-v-s2-prop-6-cor-3 .statement}

Với các giả thiết và ký hiệu của Hệ quả 2, nếu $A$ là nửa địa phương thì $A'$ cũng vậy.

Với mọi iđêan cực đại $m'$ của $A'$, $m' \cap A$ là một iđêan cực đại của $A$ (no. 1, Mệnh đề 1); khi đó hệ quả suy ra từ Hệ quả 2, vì theo giả thiết tập hợp các iđêan cực đại của $A$ là hữu hạn.

#### Hệ quả 4 {#ac-v-s2-prop-6-cor-4 .statement}

Cho $A$ là một miền nguyên đóng, $K$ trường phân thức của nó, $K$ một mở rộng Galois của $K$, $A'$ là bao đóng nguyên của $A$ trong $K'$, $\mathfrak{p}'$ là một iđêan nguyên tố của $A$, $\mathfrak{p} = A \cap \mathfrak{p}'$ và $k$ và $k'$ lần lượt là các trường phân thức của $A/\mathfrak{p}$ và $A'/\mathfrak{p}'$. Khi đó:

(i) Trường phân thức của $A^{\mathbf{Z}}/(\mathfrak{p}' \cap A^{\mathbf{Z}})$ bằng $k$ và iđêan cực đại của vành địa phương của $A^{\mathbf{Z}}$ đối với $\mathfrak{p}' \cap A^{\mathbf{Z}}$ được sinh bởi $\mathfrak{p}$.

(ii) Trường phân thức $k^T$ của $A^T/(\mathfrak{p}' \cap A^T)$ là mở rộng tách được lớn nhất của $k$ được chứa trong $k'$.

Vành $A$ là vành các bất biến trong $A'$ của nhóm Galois của $K'$ trên $K$; nếu $K'$ có bậc hữu hạn trên $K$, thì hệ quả suy ra từ các Mệnh đề 4 và 5 của no. 2. Bây giờ xét trường hợp tổng quát, khi đó $K'$ là hợp của một tập có hướng phải $(K_i)$ gồm các mở rộng Galois hữu hạn của $K$. Khi đó:

(i) Nếu $x, y$ là hai phần tử của $A^{\mathbf{Z}}$, với $y \notin \mathfrak{p}'$, thì tồn tại một chỉ số $\alpha$ sao cho $x$ và $y$ thuộc $A^{\mathbf{Z}}(\mathfrak{p}' \cap K_{\alpha})$ (Nhận xét 2); theo Mệnh đề 4 của no. 2, tồn tại $x_0, y_0$ trong $A$ với $y_0 \notin \mathfrak{p}'$ sao cho $xy_0 - x_0y \in \mathfrak{p}'$, điều này chứng minh mệnh đề thứ nhất của (i); nếu thêm nữa $x \in \mathfrak{p}'$, ta có thể giả sử rằng $y_0$ thỏa mãn
$$
xy_0 \in \mathfrak{p}A^{\mathbf{Z}}(\mathfrak{p}' \cap K_{\alpha}) \subset \mathfrak{p}A^{\mathbf{Z}}(\mathfrak{p}'),
$$
điều này chứng minh mệnh đề thứ hai của (i).

(ii) Bây giờ giả sử rằng $x \in A^T$; tồn tại $\alpha$ sao cho $x \in A^T(p' \cap K,)$ (Nhận xét 2) và Mệnh đề 5 của no. 2 cho thấy rằng lớp $\bar{x}$ của $x \mod.(p' \cap K, \cap A^T)$ là đại số và tách được trên $k$; *a fortiori* lớp $\mod.(p' \cap A^T)$ của $x$ là tách được trên $k$; để hoàn tất chứng minh của hệ quả, chỉ cần chứng minh rằng $k'$ là một mở rộng *radicial* của $k^T$. Bây giờ, $k'$ là hợp của họ có hướng phải các trường phân thức $k_\alpha$ của các vành $(A' \cap K_\alpha)/(p' \cap K,)$. Do đó suy ra từ Mệnh đề 5 rằng, nếu một phần tử của $k'$ thuộc $k$, thì nó là radicial trên trường phân thức của

$$
A^T(p' \cap K_\alpha)/(p' \cap A^T(p' \cap K_\alpha))
$$

và *a fortiori* trên $k^T$ (do Nhận xét 2).

#### Định nghĩa 5 {#ac-v-s2-def-5 .statement}

*Với các giả thiết và ký hiệu của Mệnh đề 6, trường bất biến $K^Z(p')$ (resp. $K^T(p')$) của nhóm $G^Z(p')$ (resp. $G^T(p')$) trong trường $K'$ được gọi là trường phân tích* (resp. *trường quán tính*) *của $p'$ đối với $K$*.

Ta cũng viết $K^Z$ (resp. $K^T$) thay cho $K^Z(p')$ (resp. $K^T(p')$). Suy ra từ § 1, no. 9, Mệnh đề 23 rằng $K^Z$ (resp. $K^T$) là trường *phân thức* của vành $A^Z$ (resp. $A^T$); $A^Z$ (resp. $A^T$) là bao đóng nguyên của $A$ trong $K^Z$ (resp. $K^T$).

*Nhận xét*

(3) Trong các điều kiện của Hệ quả 4 của Mệnh đề 6 và giả sử rằng $[K':K]$ là *hữu hạn*, số các ideal nguyên tố phân biệt nằm trên $p$ là $[K^Z:K]$, bậc này bằng với chỉ số ('3:*G*Z*) theo lý thuyết Galois; hơn nữa, suy ra từ lý thuyết Galois rằng

$$(6)$$
$$
[K^T:K^Z] = (G^Z:G^T) = [k^T:k].
$$

(4) Cho $A$ là một miền nguyên đóng nguyên, $K$ là trường phân thức của nó, $K'$ là một mở rộng đại số *hữu hạn* của $K$ và $A'$ là bao đóng nguyên của $A$ trong $K'$. Khi đó, với mọi iđêan nguyên tố $p$ của $A$, *số* $\&$ *iđêan nguyên tố* $\&$ *của* $A'$ *nằm trên* $p$ *nhiều nhất là* $[K':K]_s$ (nhân tử tách được của bậc của $K$ trên $K$). Trước hết ta có thể chỉ xét trường hợp $K$ là một mở rộng tách được của $K$, vì trong trường hợp tổng quát $K$ là một mở rộng radicial của mở rộng tách được lớn nhất $K_0$ của $K$ được chứa trong $K'$, $[K':K]_s = [K_0:K]$ theo định nghĩa và, nếu $A$, là bao đóng nguyên của $A$ trong $K_0$, thì các iđêan nguyên tố của $A$, và $A'$ tương ứng một-một (Bổ đề 4). Do đó giả sử rằng $K$ tách được trên $K$ và gọi $N$ là mở rộng Galois của $K$ sinh bởi $K$ trong một bao đóng đại số của $K$, $G$ là nhóm Galois của nó, $B$ là bao đóng nguyên của $A$ trong $N$ và $\mathfrak{P}$ là một iđêan nguyên tố của $B$ nằm trên $p$. Gọi $\mathcal{H}$ là nhóm Galois của $N$ trên $K$ và $G^Z$ là nhóm phân tích của $\mathfrak{P}$; các iđêan nguyên tố của $B$ nằm trên $p$ là các $s.\mathfrak{P}$ với $s \in G$ (no. 2, Định lý 2) và hệ thức $s.\mathfrak{P} = s'.\mathfrak{P}$ có nghĩa là $s' = sg$ với $g \in G^Z$. Mặt khác để có $s.\mathfrak{P} \cap K' = s'.\mathfrak{P} \cap K'$, điều kiện cần và đủ là $s'.\mathfrak{P} = ts.\mathfrak{P}$, với $t \in \mathcal{H}$ (no. 2, Định lý 2), do đó cuối cùng $s' = tsg$ với $t \in \mathcal{H}$ và $g \in G^Z$. Vậy số iđêan nguyên tố của $A'$ nằm trên $p$ bằng *số các lớp của $G$ theo quan hệ tương đương* "tồn tại $t \in \mathcal{H}$ và $g \in G^{\mathbf{Z}}$ sao cho $s' = tsg$" giữa $s$ và $s'$; rõ ràng số này nhiều nhất bằng chỉ số $(G : \mathcal{H})$, số các lớp kề phải của $\mathcal{H}$ trong $G$, và $(G : \mathcal{H}) = [K' : K]$ theo lý thuyết Galois.

#### Mệnh đề 7 {#ac-v-s2-prop-7 .statement}

*Cho $A$ là một miền nguyên đóng, $K$ trường phân thức của nó, $K'$ một mở rộng Galois của $K$, $\mathcal{G}$ nhóm Galois của nó, $A'$ bao đóng nguyên của $A$ trong $K'$, $p'$ một iđêan nguyên tố của $A'$ và $p = A \cap p'$. Sau hết, cho $L$ là một trường con của $K'$ chứa $K$ và đặt $p(L) = p' \cap L$.

(i) *Trường phân tích* (resp. *trường quán tính*) *của $p'$ đối với $L$ là $L(K^{\mathbf{Z}})$ (resp. $L(K^T)$); *nếu thêm nữa $L$ là một mở rộng Galois của $K$, trường phân tích của $p(L)$ đối với $K$ là $L \cap K^{\mathbf{Z}}$.

(ii) *Nếu $L$ được chứa trong $K^{\mathbf{Z}}$, $A/p$ và $(A' \cap L)/p(L)$ có cùng trường phân thức và trong vành địa phương $A' \cap L$ tương ứng với iđêan nguyên tố $p(L)$, iđêan cực đại được sinh bởi $p$. Ngược lại, nếu hai điều kiện này được thỏa mãn và thêm nữa $\bigcap_{n > 0} p^n A'_p = 0$, thì $L$ được chứa trong $K^{\mathbf{Z}}$.

(i) Nếu $\mathcal{H}$ là nhóm con của $\mathcal{G}$ giữ bất biến các phần tử của $L$, rõ ràng nhóm phân tích (resp. nhóm quán tính) của $p'$ đối với $L$ là $G^{\mathbf{Z}} \cap \mathcal{H}$ (resp. $G^T \cap \mathcal{H}$) và mệnh đề thứ nhất suy ra từ lý thuyết Galois nếu $K'$ là một mở rộng Galois *hữu hạn* của $K$ (*Algebra*, Chương V, § 10, no. 6, Hệ quả 1 của Định lý 3); trong trường hợp tổng quát nó suy ra từ sự kiện rằng $A^{\mathbf{Z}}$ (resp. $A^T$) là hợp của các $A^{\mathbf{Z}}(p' \cap K_\alpha)$ (resp. $A^T(p' \cap K_\beta)$) theo ký hiệu của *Nhận xét 2*: mọi phần tử $x \in K'$ đều thuộc một $K$, và nếu nó bất biến dưới $G^{\mathbf{Z}}(p') \cap \mathcal{H}$ (resp. $G^T(p') \cap \mathcal{H}$) thì nó cũng bất biến dưới $G^{\mathbf{Z}}(p' \cap K_{\beta'}) \cap \mathcal{H}$ (resp. $G^T(p' \cap K_{\beta'}) \cap \mathcal{H}$) với một $\beta'$ thích hợp; do đó, theo phần đầu của lập luận, nó thuộc

$$
L(K^{\mathbf{Z}}(p' \cap K_{\alpha})) \subset L(K^{\mathbf{Z}}) \quad (\text{resp. } L(K^T(p' \cap K_{\beta})) \subset L(K^T)).
$$

Giả sử bây giờ rằng $L$ là một mở rộng Galois của $K$; khi đó hạn chế lên $L$ của mọi $\sigma \in G^{\mathbf{Z}}$ đều để bất biến $p(L) = p' \cap L$ và do đó thuộc nhóm phân tích của $p(L)$ đối với $K$. Ngược lại, giả sử $\tau$ là một tự đẳng cấu của $L$ thuộc nhóm này và giả sử $\sigma$ là một mở rộng của $\tau$ thành một $K$-tự đẳng cấu của $K'$; ta viết $q' = \sigma.p'$. Vì $p'$ và $q'$ đều nằm trên $p(L)$, tồn tại một tự đẳng cấu $\rho \in \mathcal{H}$ sao cho $q' = \rho.p'$, do đó $\rho^{-1}\sigma \in G^{\mathbf{Z}}$ và $\tau$ là hạn chế của $\rho^{-1}\sigma$ lên $L$; nói cách khác, nhóm phân tích của $p(L)$ đối với $K$ đồng nhất với nhóm các hạn chế lên $L$ của các tự đẳng cấu $\sigma \in G^{\mathbf{Z}}$, điều này chứng minh mệnh đề thứ hai.

(ii) Nói rằng $L \subset K^{\mathbf{Z}}$ có nghĩa là $\mathcal{H} \supset G^{\mathbf{Z}}$ và vì thế các mệnh đề của (ii) là những trường hợp riêng của no. 2, Mệnh đề 4 (ii) và (iii) khi $[K':K]$ là hữu hạn. Trong trường hợp tổng quát, lập luận cũng như trong chứng minh của Mệnh đề 6.

### 4. ĐỊNH LÝ TỒN TẠI THỨ HAI

#### Định lý 3 {#ac-v-s2-thm-3 .statement}

Cho $A$ là một miền nguyên đóng và $A'$ là một vành chứa $A$ và nguyên trên $A$. Giả sử rằng $0$ là phần tử duy nhất của $A$ là một ước của $0$ trong $A'$. Cho $p, q$ là hai iđêan nguyên tố của $A$ sao cho $q \supset p$ và $q'$ là một iđêan nguyên tố của $A$ nằm trên $q$. Khi đó tồn tại một iđêan nguyên tố $p'$ của $A$ nằm trên $p$ và sao cho $q' \supset p'$.

Trước hết giả sử rằng $A'$ là một miền nguyên. Gọi $K, K'$ lần lượt là các trường phân thức của $A$ và $A'$; gọi $K''$ là bao đóng đại số của $K$ và $A$ là bao đóng nguyên của $A$ trong $K''$; khi đó $A \subset A' \subset A''$. Gọi $p''$ là một iđêan nguyên tố của $A''$ nằm trên $p$ (no. 1, Định lý 1), $q''$ là một iđêan nguyên tố của $A''$ nằm trên $q$ và sao cho $p'' \subset q''$ (no. 1, Hệ quả 2 của Định lý 1), và cuối cùng $q_1''$ là một iđêan nguyên tố của $A''$ nằm trên $q'$ (no. 1, Định lý 1). Theo no. 3, Mệnh đề 6 (i), tồn tại một $K$-tự đẳng cấu $\sigma$ của $K''$ sao cho $Q.q'' = q_1''$. Khi đó $Q.p''$ là một iđêan nguyên tố của $A''$ nằm trên $p$ sao cho $Q.p'' = q_1''$, và do đó $p' = A' \cap \sigma.p''$ là một iđêan nguyên tố của $A'$ nằm trên $p$ và được chứa trong $A' \cap q_1'' = q'$.

Ta chuyển sang trường hợp tổng quát. Vì $A$ là một miền nguyên và $q'$ là nguyên tố, các tập con $A - \{0\}$ và $A' - q'$ của $A'$ là các tập hợp nhân tính; khi đó tích của chúng $S = (A - \{0\})(A' - q')$ là một tập con nhân tính của $A'$ không chứa 0 vì các phần tử khác không của $A$ không là ước của 0 trong $A'$. Khi đó tồn tại (Chương II, §2, no. 5, Hệ quả 2 của Mệnh đề 11) một iđêan nguyên tố $m'$ của $A'$ rời nhau với $S$, nói cách khác sao cho $m' \subset q'$ và $m' \cap A = 0$. Gọi $h$ là đồng cấu chính tắc $A' \to A'/m'$. Hạn chế của $h$ trên $A$ là đơn ánh và do đó $h(A)$ là nguyên đóng. Vì $m' \subset q'$, $h(q')$ là một iđêan nguyên tố của $A'/m'$ nằm trên $h(q)$; vì $A'/m'$ là một miền nguyên, phần đầu của chứng minh chứng tỏ rằng tồn tại một iđêan nguyên tố $n'$ của $A'/m'$ sao cho $n' \cap h(A) = h(p)$ và $h(q') \supset n'$. Iđêan $p' = h^{-1}(n')$ là một iđêan nguyên tố của $A'$ và $q' \supset p'$, vì $q'$ chứa hạt nhân của $h$. Vì $n' \supset h(p)$, ta có $p' \supset p$. Sau cùng, với $x \in p' \cap A$, ta có $h(x) \in n' \cap h(A) = h(p)$ và do đó $x \in p$ vì hạn chế của $h$ trên $A$ là đơn ánh; vậy $p' \cap A = p$.

#### Hệ quả {#ac-v-s2-n4-cor-1 .statement}

Dưới các giả thiết về $A$ và $A'$ của Định lý 3, cho $p$ là một iđêan nguyên tố của $A$. Các iđêan nguyên tố của $A'$ nằm trên $p$ là các phần tử cực tiểu của tập hợp $\mathcal{E}$ gồm các iđêan nguyên tố của $A'$ chứa $pA'$.

Một iđêan nguyên tố của $A'$ nằm trên $p$ là cực tiểu trong $\mathcal{E}$ theo no. 1, Hệ quả 1 của Mệnh đề 1. Ngược lại, giả sử $q'$ là một phần tử cực tiểu của $\mathcal{E}$. Vì $q' \cap A \supset p$, Định lý 3 cho thấy rằng tồn tại một iđêan nguyên tố $p'$ của $A'$ nằm trên $p$ sao cho $q' \supset p'$. Vì $p'$ chứa $pA'$, giả thiết đặt ra trên $q'$ kéo theo $q' = p'$ và do đó $q'$ nằm trên $p$.

\* Cho $V, V'$ là hai đa tạp đại số afin và $f$ là một cấu xạ từ $V'$ vào $V$ sao cho $f(V')$ trù mật trong $V$. Gọi $A$ (resp. $A'$) là vành các hàm chính quy trên $V$ (resp. $V'$); khi đã cho $f$ ta có thể đồng nhất $A$ với một vành con của $A'$; giả sử rằng $A'$ là nguyên trên $A$. Định lý 1 của no. 1 cho thấy rằng với mọi đa tạp con bất khả quy W của V tồn tại một đa tạp con bất khả quy W' của V' sao cho f(W') là một tập con trù mật của W; đặc biệt, mọi điểm của V đều là ảnh của một đa tạp con bất khả quy của V', điều đó cho thấy rằng f là toàn ánh. Tương tự, hạn chế của f lên mọi đa tạp con bất khả quy W' của V' ánh xạ W' lên một đa tạp con bất khả quy của V. Hệ quả 2 của Định lý 1, no. 1 cho thấy rằng, nếu W và X là hai đa tạp con bất khả quy của V sao cho W ⊃ X và nếu W' là một đa tạp con bất khả quy của V' sao cho f(W') = W, thì tồn tại một đa tạp con bất khả quy X' của V' được chứa trong W' và sao cho f(X') = X.

Nếu A nguyên đóng, V được gọi là chuẩn tắc. Định lý 3 cho thấy rằng, nếu V chuẩn tắc, nếu W và X là các đa tạp con bất khả quy của V sao cho W ⊃ X và nếu X' là một đa tạp con bất khả quy của V' sao cho f(X') = X, thì tồn tại một đa tạp con W' của V' chứa X' và sao cho f(W') = W. Sau cùng, Hệ quả của Định lý 3 cho thấy rằng, nếu V chuẩn tắc và W là một đa tạp con bất khả quy của V, thì các đa tạp con bất khả quy W' của V' sao cho f(W') = W chính là các thành phần bất khả quy của $\overline{f}(W)$.

### Bài tập {#ac-v-s2-exercises}

Xem [bài tập của § 2](exercises/s2/).
