---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 6
section_title: Extension des scalaires dans les algèbres régulières
lang: vi
source: ac-x-fr
pdf_pages: 0070-0081, 0168-0169
extraction: ocr
subsections:
    - "no": 1
      title: Algèbres essentiellement de type fini
      page: 0
      pdf_page: 70
    - "no": 2
      title: Produits tensoriels d’algèbres de Macaulay ou de Gorenstein
      page: 72
      pdf_page: 71
    - "no": 3
      title: Extension séparable du corps de base dans les algèbres régulières¹ ou normales
      page: 74
      pdf_page: 73
    - "no": 4
      title: Algèbres absolument régulières ou absolument normales
      page: 75
      pdf_page: 74
    - "no": 5
      title: Caractérisations des algèbres absolument régulières
      page: 78
      pdf_page: 77
statements: 33
exercises: 7
content_sha256: be4a111d950c5ccaf82427db21cbfb5efa205eb1c52d608fb70042fb648d7fd4
translated_from: content/en-mt/ac/X/06_s6_extension_des_scalaires_dans_les.md
source_lang: en-mt
translation_method: machine
source_content_sha256: c84daa7dbe6aa93123acfe74543d04724270297c2378e2fea903940e90f83dcc
translation_model: gpt-5.4
translation_run: translate-vi-ae6330f9
glossary_version: 34
glossary_terms_sha256: 3d72ee54af1b877f2329974a30b75f034c5cdd2d21be4ba4d2abb62e57beb8b2
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. MỞ RỘNG VÔ HƯỚNG TRONG CÁC ĐẠI SỐ CHÍNH QUY

### 1. Các đại số cốt yếu kiểu hữu hạn

Cho $k$ là một vành. Cho $A$ là một $k$-đại số và $x = (x_i)_{i \in I}$ một họ các phần tử của $A$; ký hiệu $A'$ là đại số con của $A$ sinh bởi các $x_i$. Ta sẽ nói rằng $x$ là một họ sinh cốt yếu của $k$-đại số $A$ nếu, với mọi phần tử $a$ của $A$, tồn tại một phần tử $s$ của $A'$, khả nghịch trong $A$, sao cho $sa$ thuộc $A'$. Điều này tương đương với việc nói rằng, với mọi $a \in A$, tồn tại các đa thức $P$ và $Q$ trong $k[(X_i)_{i \in I}]$ sao cho $Q(x)$ khả nghịch trong $A$ và ta có $a = P(x)Q(x)^{-1}$.

Ta sẽ nói rằng một $k$-đại số $A$ là cốt yếu kiểu hữu hạn nếu nó nhận một họ sinh cốt yếu hữu hạn. Điều này tương đương với việc nói rằng tồn tại một $k$-đại số $A'$ kiểu hữu hạn và một tập con nhân tính $S$ của $A'$ sao cho $k$-đại số $A$ đẳng cấu với $S^{-1}A'$.

#### Ví dụ 1 {#ac-x-s6-n1-exa-1 .statement}

Nói rằng một mở rộng $L$ của một trường $K$ là một $K$-đại số cốt yếu kiểu hữu hạn có nghĩa là nó là một mở rộng kiểu hữu hạn theo nghĩa của A, V, p. 11, Def. 2. $K$-đại số $L$ chỉ là kiểu hữu hạn nếu nó là một mở rộng bậc hữu hạn của $K$ (V, § 3, No. 4, Hệ quả 3 of Định lý 3).

#### Ví dụ 2 {#ac-x-s6-n1-exa-2 .statement}

Để một $k$-đại số địa phương là cốt yếu kiểu hữu hạn, điều kiện cần và đủ là nó đẳng cấu với một $k$-đại số dạng $A_p$, trong đó $A$ là một $k$-đại số kiểu hữu hạn và $p$ là một iđêan nguyên tố của $A$ (x. II, § 2, No. 5, Prop. 11 (iii)).

#### Mệnh đề 1 {#ac-x-s6-prop-1 .statement}

Nếu vành $k$ là Noether, mọi $k$-đại số cốt yếu kiểu hữu hạn đều là một vành Noether.

Điều này suy ra từ III, § 2, No. 10, Cor. 3 of Th. 2 và II, § 2, No. 4, Cor. 2 of Prop. 10.

Các tính chất sau được suy ra từ định nghĩa:

#### Mệnh đề 2 {#ac-x-s6-prop-2 .statement}

a) Mọi đại số thương của một $k$-đại số cốt yếu kiểu hữu hạn đều là cốt yếu kiểu hữu hạn.

b) Mọi vành phân thức của một $k$-đại số cốt yếu kiểu hữu hạn đều là một $k$-đại số cốt yếu kiểu hữu hạn.

c) $k$-đại số tích của một họ hữu hạn các $k$-đại số cốt yếu kiểu hữu hạn là cốt yếu kiểu hữu hạn.

d) Cho $k \to k'$ là một đồng cấu các vành; với mọi $k$-đại số $A$ cốt yếu kiểu hữu hạn, $k'$-đại số $A_{(k')} = k' \otimes_k A$ là cốt yếu kiểu hữu hạn.

#### Hệ quả {#ac-x-s6-n1-cor-1 .statement}

Cho $A$ là một $k$-đại số về cơ bản thuộc kiểu hữu hạn và $B$ là một $k$-đại số Noether. Khi đó vành $A \otimes_k B$ là Noether.

Thật vậy, nó là một $B$-đại số về cơ bản thuộc kiểu hữu hạn (mệnh đề 2, d)), và áp dụng Mệnh đề 1.

#### Mệnh đề 3 {#ac-x-s6-prop-3 .statement}

Cho $k$ là một vành, $A$ là một $k$-đại số và $B$ là một $A$-đại số. Nếu $A$ về cơ bản thuộc kiểu hữu hạn trên $k$ và $B$ về cơ bản thuộc kiểu hữu hạn trên $A$, thì $B$ về cơ bản thuộc kiểu hữu hạn trên $k$.

Ký hiệu $\rho : A \to B$ là ánh xạ chính tắc. Cho $x = (x_i)_{i \in I}$ là một họ sinh về cơ bản hữu hạn của $k$-đại số $A$, và gọi $A'$ là đại số con sinh bởi họ đó; cho $y = (y_j)_{j \in J}$ là một họ sinh về cơ bản hữu hạn của $A$-đại số $B$. Ký hiệu $B'$ là $k$-đại số con của $B$ sinh bởi các $\rho(x_i)$ và các $y_j$. Cho $b \in B$; theo giả thiết tồn tại các đa thức $P$ và $Q$ trong $A[(Y_j)_{j \in J}]$ sao cho $Q(y)$ khả nghịch trong $B$ và sao cho ta có $Q(y) b = P(y)$. Các hệ số khác không của $P$ và $Q$ là hữu hạn về số lượng; tồn tại một đa thức $R \in k[(X_i)_{i \in I}]$ sao cho $R(x)$ khả nghịch trong $A$ và sao cho $R(x) P$ và $R(x) Q$ thuộc $A'[(Y_j)_{j \in J}]$. Khi đó $\rho(R(x)) Q(y)$ khả nghịch trong $B$, và ta có

$$
\rho(R(x)) Q(y) b = \rho(R(x)) P(y) \in B'.
$$

Vậy các phần tử $\rho(x_i)$ với $i \in I$ và $y_j$ với $j \in J$ tạo thành một họ sinh về cơ bản hữu hạn của $k$-đại số $B$.

#### Hệ quả {#ac-x-s6-n1-cor-2 .statement}

Tích tenxơ của hai $k$-đại số về cơ bản thuộc kiểu hữu hạn là một $k$-đại số về cơ bản thuộc kiểu hữu hạn.

Vì giả sử $A$ và $B$ là hai $k$-đại số về cơ bản thuộc kiểu hữu hạn. Khi đó $A \otimes_k B$ về cơ bản thuộc kiểu hữu hạn trên $A$ (Mệnh đề 2, d)), nên cũng vậy trên $k$ (Mệnh đề 3).

### 2. Tích tenxơ của các đại số Macaulay hoặc Gorenstein

#### Mệnh đề 4 {#ac-x-s6-prop-4 .statement}

Cho $k$ là một trường, $A$ là một $k$-đại số về cơ bản thuộc kiểu hữu hạn và $B$ là một $k$-đại số.

a) Nếu $A$ và $B$ là các vành Macaulay, thì $A \otimes_k B$ cũng vậy.

b) Nếu $A$ và $B$ là các vành Gorenstein, thì $A \otimes_k B$ cũng vậy.

Giả sử rằng $A$ và $B$ là các vành Macaulay (tương ứng, các vành Gorenstein), và hãy chứng minh rằng $A \otimes_k B$ cũng vậy. Vành $A \otimes_k B$ là Noether (No. 1, hệ quả của Mệnh đề 2). A-môđun $A \otimes_k B$ là tự do, nên phẳng. Theo Mệnh đề 10 của § 2, No. 7 (tương ứng, Hệ quả 1 của Mệnh đề 12 của § 3, No. 8), chỉ cần chứng minh rằng $\kappa(p) \otimes_k B$ là một vành Macaulay (tương ứng, một vành Gorenstein) với mọi iđêan nguyên tố $p$ của $A$. Mở rộng $\kappa(p)$ của $k$ thuộc kiểu hữu hạn (No. 1, Mệnh đề 2 và Ví dụ 1); do đó ta được rút gọn về việc chứng minh mệnh đề trong trường hợp $k$-đại số $A$ là một mở rộng $K$ thuộc kiểu hữu hạn của $k$.

Khi đó vành $K \otimes_k B$ là một B-môđun tự do hạng hữu hạn, nên là một B-môđun Macaulay. Theo § 2, No. 6, Hệ quả 1 của Mệnh đề 8, nó là một vành Macaulay, điều này chứng minh a). Bây giờ giả sử rằng $B$ là một vành Gorenstein. Tồn tại các mở rộng trung gian $K_i,\ 0 \leq i \leq m$, của $K$ sao cho

$$
k = K_0 \subset K_1 \subset \cdots \subset K_m = K
$$

và sao cho $K_i$ là một $K_{i-1}$-đại số đơn sinh với $i = 1, \ldots, m$; điều này cho phép ta rút gọn về trường hợp mở rộng $K$ của $k$ là đơn sinh (bậc hữu hạn). Đồng cấu chính tắc $B \to K \otimes_k B$ biến $K \otimes_k B$ thành một B-đại số phẳng và, với mọi $q \in \mathrm{Spec}(B)$, vành $(K \otimes_k B) \otimes_B \kappa(q)$, đẳng cấu với $K \otimes_k \kappa(q)$, là một $\kappa(q)$-đại số đơn sinh, nên là một vành Gorenstein ($§ 3$, n° 9, ví dụ 5). Do đó $K \otimes_k B$ là một vành Gorenstein ($§ 3$, n° 8, hệ quả 1 của Mệnh đề 12), điều này hoàn tất chứng minh của b).

#### Hệ quả 1 {#ac-x-s6-prop-4-cor-1 .statement}

Cho $k$ là một trường, $K$ là một mở rộng của $k$ và $\Lambda$ là một $k$-đại số về cơ bản thuộc kiểu hữu hạn. Để $A_{(K)}$ là một vành Macaulay (tương ứng một vành Gorenstein), điều kiện cần và đủ là điều đó cũng đúng với $A$.

Nếu $A$ là một vành Macaulay (tương ứng một vành Gorenstein), thì $A_{(K)}$ cũng vậy theo Mệnh đề 4. Vì $A_{(K)}$ là một A-môđun phẳng trung thành, mệnh đề đảo lại suy ra từ Mệnh đề 10 của § 2, No. 7 (tương ứng Hệ quả 1 của Mệnh đề 12 của § 3, No. 8).

#### Hệ quả 2 {#ac-x-s6-prop-4-cor-2 .statement}

Cho $k$ là một vành Noether, $A$ và $B$ là các $k$-đại số. Giả sử rằng $A$ là phẳng và về cơ bản thuộc kiểu hữu hạn trên $k$. Nếu $A$ và $B$ là các vành Macaulay (tương ứng các vành Gorenstein), thì $A \otimes_k B$ là một vành Macaulay (tương ứng một vành Gorenstein).

Trước hết giả sử rằng $B$ là một trường; gọi $\varphi$ là đồng cấu chính tắc từ $k$ vào $B$, và $r$ là hạt nhân của nó. Đồng cấu $\varphi$ cảm sinh một đồng cấu từ trường phân thức $\kappa(r)$ của $k/r$ vào $B$. Khi đó $A \otimes_k B$ được đồng nhất với $(A \otimes_k \kappa(r)) \otimes_{\kappa(r)} B$; vì $\varphi^{-1}(0) = r$, vành $A \otimes_k \kappa(r)$ là một vành Macaulay (tương ứng một vành Gorenstein) theo Mệnh đề 10 của § 2, No. 7 (tương ứng Hệ quả 1 của Mệnh đề 12 của § 3, No. 8). Khi đó trong trường hợp này mệnh đề suy ra từ Hệ quả 1.

Ta chuyển sang trường hợp tổng quát. $B$-đại số $A \otimes_k B$ là phẳng, và Noether theo hệ quả của Mệnh đề 2 ở No. 1. Với mỗi iđêan nguyên tố $q$ của $B$, vành $(A \otimes_k B) \otimes_B \kappa(q)$, được đồng nhất với $A \otimes_k \kappa(q)$, là một vành Macaulay (tương ứng một vành Gorenstein) theo điều vừa nói trên. Ta kết luận bằng cách áp dụng Mệnh đề 10 của § 2, No. 7 (tương ứng Hệ quả 1 của Mệnh đề 12 của § 3, No. 8).

### 3. Mở rộng tách được của trường cơ sở trong các đại số chính quy¹ hoặc nguyên

#### Bổ đề 1 {#ac-x-s6-lem-1 .statement}

Cho $A$ là một vành Noether, là hợp của một họ lọc tăng $(A_\alpha)_{\alpha \in I}$ các vành con Noether.

a) Nếu các vành $A_\alpha$ là chính quy và nếu $A$ là một A_\alpha-môđun phẳng với mọi $\alpha \in I$, thì vành $A$ là chính quy.

b) Nếu các vành $A_\alpha$ là nguyên ($§ 1$, No. 8), thì $A$ là nguyên.

a) Cho $m$ là một iđêan cực đại của $A$; với mỗi $\alpha \in I$, ký hiệu $m_\alpha$ là iđêan $m \cap A_\alpha$ của $A_\alpha$. Vì $A$ là Noether, $m$ là kiểu hữu hạn và tồn tại một phần tử $\alpha$ của $I$ sao cho $m = A m_\alpha$, do đó A-môđun $(A_\alpha / m_\alpha) \otimes_{A_\alpha} A$ đẳng cấu với $A / m$. Vì $A$ là phẳng trên $A_\alpha$, ta có $\mathrm{dp}_A(A/m) \leq \mathrm{dp}_{A_\alpha}(A_\alpha / m_\alpha)$ (A, X, p. 141, Bổ đề 2). Vì các vành $A_\alpha$ là chính quy, suy ra $A$ là chính quy ($§ 4$, No. 2, Mệnh đề 4).

b) Vì các $A_\alpha$ là rút gọn, $A$ là rút gọn. Cho $a$ và $b$ là các phần tử của $A$ sao cho $b$ không phải là một ước của không và phần tử $a/b$ của vành phân thức toàn phần của $A$ là nguyên trên $A$. Tồn tại một đa thức đơn khởi $P \in A[X]$ sao cho $P(a/b) = 0$. Cho $\alpha$ là một phần tử của $I$ sao cho vành $A_\alpha$ chứa $a$, $b$ và các hệ số của $P$. Vì $A_\alpha$ là chuẩn tắc, tồn tại $c \in A_\alpha$ sao cho $a = bc$. Do đó $a/b = c$ thuộc $A$ và $A$ là chuẩn tắc.

#### Bổ đề 2 {#ac-x-s6-lem-2 .statement}

Cho $k$ là một trường, và cho $K$ và $L$ là các mở rộng của $k$. Giả sử rằng $K$ là kiểu hữu hạn và một trong hai mở rộng $K$ hoặc $L$ là tách được. Khi đó vành $K \otimes_k L$ là chính quy.

Ký hiệu $A$ là vành $K \otimes_k L$; nó là Noether theo hệ quả của mệnh đề 2 (No. 2). Trước hết giả sử rằng mở rộng $K$ là tách được. Theo A, V, p. 130, hệ quả, tồn tại một cơ sở siêu việt $t = (t_1, \ldots, t_n)$ của $K$ sao cho $K$ là một mở rộng tách được hữu hạn của mở rộng thuần túy $k(t)$. Vành $E = k(t) \otimes_k L$, đẳng cấu với một vành phân thức của một vành đa thức trên $L$, là chính quy ($§ 4$, No. 2, hệ quả 5 của mệnh đề 4); với mọi iđêan nguyên tố $p$ của $E$, vành $\kappa(p) \otimes_E A$ đẳng cấu với $\kappa(p) \otimes_{k(t)} K$, do đó đẳng cấu với một tích hữu hạn các trường (A, V, p. 35, định nghĩa 1, p. 34, định lý 4, và p. 33, mệnh đề 5). Vì $A$ là một E-môđun tự do, nó là một vành chính quy theo hệ quả của mệnh đề 9 của $§ 4$, No. 5.

Bây giờ giả sử rằng $L$ tách được trên $k$. Theo phần đầu của chứng minh, vành $K \otimes_k L'$ là chính quy với mọi mở rộng con kiểu hữu hạn $L'$ của $L$. Kết luận bằng cách áp dụng bổ đề 1.

#### Mệnh đề 5 {#ac-x-s6-prop-5 .statement}

Cho $k$ là một trường, $A$ một $k$-đại số và $K$ một mở rộng của $k$. Giả sử rằng $A$ là cốt yếu kiểu hữu hạn hoặc mở rộng $K$ là kiểu hữu hạn.

¹ Trong số này, một đại số trên một trường $k$ được gọi là chính quy nếu nó là một vành chính quy. Đặc biệt, mọi mở rộng của $k$ đều là một đại số chính quy. Cần chú ý không nhầm khái niệm này với khái niệm mở rộng chính quy, được đưa vào trong A, V, p. 135, định nghĩa 2, khái niệm này sẽ không xuất hiện ở đây.

a) Nếu vành $A_{(K)}$ là chính quy (tương ứng chuẩn tắc), thì vành $A$ là chính quy (tương ứng chuẩn tắc).

b) Nếu vành $A$ là chính quy (tương ứng chuẩn tắc) và nếu mở rộng $K$ của $k$ là tách được, thì vành $A_{(K)}$ là chính quy (tương ứng chuẩn tắc).

A-môđun $A_{(K)}$ là tự do, do đó phẳng trung thành; vì vậy mệnh đề a) suy ra từ hệ quả của mệnh đề 8 của I, § 3, No. 5 và từ mệnh đề 8 của § 4, No. 5 (tương ứng hệ quả 2 của định lý 4 của § 1, No. 10). Dưới các giả thiết của b), với mọi iđêan nguyên tố $\mathfrak{p}$ của $A$, vành $\kappa(\mathfrak{p}) \otimes_k K$ là chính quy (bổ đề 2), và $a fortiori$ chuẩn tắc (§ 4, No. 2, hệ quả 2 của mệnh đề 4). Vì vậy mệnh đề b) suy ra từ hệ quả của mệnh đề 9 của § 4, No. 5 (tương ứng hệ quả 3 của định lý 4 của § 1, No. 10).

### 4. Các đại số tuyệt đối chính quy hoặc tuyệt đối chuẩn tắc

#### Định nghĩa 1 {#ac-x-s6-def-1 .statement}

Cho $k$ là một trường và $A$ một $k$-đại số. Ta nói rằng $A$ là tuyệt đối chính quy (tương ứng tuyệt đối chuẩn tắc)$^1$ nếu vành $A_{(k')}$ là chính quy (tương ứng chuẩn tắc) với mọi mở rộng radicial $k'$ bậc hữu hạn của $k$.

Mọi $k$-đại số tuyệt đối chính quy (tương ứng tuyệt đối chuẩn tắc) đều chính quy (tương ứng chuẩn tắc), như thấy được bằng cách lấy $k' = k$ trong định nghĩa 1. Nhắc lại rằng các $k$-đại số $A$ sao cho vành $A_{(k')}$ là rút gọn với mọi mở rộng radicial $k'$ bậc hữu hạn của $k$ là các $k$-đại số tách được (A, V, p. 117, định lý 2).

#### Ví dụ 1 {#ac-x-s6-n4-exa-1 .statement}

Nếu $k$ là hoàn hảo, mọi đại số trên $k$ chính quy (tương ứng chuẩn tắc) đều là tuyệt đối chính quy (tương ứng tuyệt đối chuẩn tắc).

#### Ví dụ 2 {#ac-x-s6-n4-exa-2 .statement}

Cho $A$ là một đại số trên $k$ Artin. Nếu $A$ là chuẩn tắc thì nó là rút gọn, do đó đẳng cấu với một tích hữu hạn các mở rộng của $k$ (A, VIII, § 8, No. 1, mệnh đề 2). Các điều kiện sau là tương đương:

A là tách được;
— A là tuyệt đối chính quy;
— A là tuyệt đối chuẩn tắc.

Thật vậy, nếu $A$ là tuyệt đối chuẩn tắc thì nó tách được; nếu $A$ tách được thì, với mọi mở rộng hữu hạn $k'$ của $k$, vành $A_{(k')}$ là rút gọn và Artin, do đó đẳng cấu với một tích các trường, và vì thế chính quy, nên $A$ là tuyệt đối chính quy.

Nếu hơn nữa đại số trên $k$ $A$ có bậc hữu hạn, thì các điều kiện trên còn tương đương với việc nói rằng $A$ là étale (A, V, p. 34, định lý 4).

#### Ví dụ 3 {#ac-x-s6-n4-exa-3 .statement}

Cho $A$ là một đại số trên $k$ địa phương chính quy. Nếu mở rộng $\kappa_A$ của $k$ là tách được thì đại số $A$ là tuyệt đối chính quy. Thật vậy, cho $k'$ là một mở rộng bậc hữu hạn của $k$. A-môđun $A_{(k')}$ là tự do. Vì nó có kiểu hữu hạn, mọi iđêan cực đại của $A_{(k')}$ đều nằm trên $\mathfrak{m}_A$ (V, § 2, No. 1, mệnh đề 1). Vành $\kappa_A \otimes_A A_{(k')}$, đẳng cấu với $\kappa_A \otimes_k k'$, là chính quy (No. 3, bổ đề 2). Theo hệ quả của mệnh đề 9 của § 4, No. 5, vành $A_{(k')}$ là chính quy, điều đó chứng tỏ rằng đại số trên $k$ $A$ là tuyệt đối chính quy.

$^1$ Một số tác giả dùng thuật ngữ “chính quy hình học” (tương ứng “chuẩn tắc hình học”.

#### Mệnh đề 6 {#ac-x-s6-prop-6 .statement}

Cho k là một trường và A là một đại số trên k Noether.

a) Nếu A là tuyệt đối chính quy (tương ứng tuyệt đối chuẩn tắc, tương ứng tách được), thì điều đó cũng đúng với S$^{-1}$A đối với mọi tập con nhân tính S của A.

b) Nếu $A_m$ là tuyệt đối chính quy (tương ứng tuyệt đối chuẩn tắc, tương ứng tách được), với mọi iđêan cực đại m của A, thì A là tuyệt đối chính quy (tương ứng tuyệt đối chuẩn tắc, tương ứng tách được).

a) Điều này suy ra từ sự kiện rằng vành $(S^{-1}A)_{(k')}$ đẳng cấu với một vành phân thức của vành $A_{(k')}$ đối với mọi mở rộng $k'$ của k.

b) Giả sử rằng $A_m$ là tuyệt đối chính quy (tương ứng tuyệt đối chuẩn tắc, tương ứng tách được) với mọi iđêan cực đại m của A. Cho $k'$ là một mở rộng không tách được thuần túy của k có bậc hữu hạn và cho $m'$ là một iđêan cực đại của $A_{(k')}$. Còn phải kiểm tra rằng vành địa phương $(A_{(k')})_{m'}$ là chính quy (tương ứng chuẩn tắc, tương ứng rút gọn).

Đồng cấu chính tắc $A \to A_{(k')}$ làm cho $A_{(k')}$ thành một đại số trên A hữu hạn. Iđêan $m'$ nằm trên một iđêan cực đại m của A (V, § 2, No. 1, mệnh đề 1), và $(A_{(k')})_{m'}$ đẳng cấu với một vành phân thức của vành chính quy (tương ứng chuẩn tắc, tương ứng rút gọn) $(A_m)_{(k')}$, và do đó là chính quy (tương ứng chuẩn tắc, tương ứng rút gọn).

#### Bổ đề 3 {#ac-x-s6-lem-3 .statement}

Cho k là một trường và K là một mở rộng kiểu hữu hạn của k. Tồn tại một mở rộng L của K, có bậc hữu hạn, và một mở rộng con $k'$ của L trên k, không tách được thuần túy và có bậc hữu hạn trên k, sao cho mở rộng L của $k'$ là tách được.

Hãy chọn một mở rộng hợp thành E của K và của một bao đóng hoàn hảo $\hat{k}$ của k, và các phần tử $(t_1, \ldots, t_n)$ của E sao cho E là một mở rộng đại số tách được của $\hat{k}(t_1, \ldots, t_n)$ (A, V, p. 130, hệ quả). Gọi I là một tập con sinh hữu hạn của K trên k. Trường $\hat{k}(t_1, \ldots, t_n)$ (resp. $\hat{k}K$) là hợp của các trường con $k'(t_1, \ldots, t_n)$ (resp. $k'K$), trong đó $k'$ chạy qua tập hợp các mở rộng con của $\hat{k}$ có bậc hữu hạn trên k; do đó có thể tìm được một mở rộng con như vậy $k'$ sao cho các phần tử $t_1, \ldots, t_n$ của E = $\hat{k}K$ thuộc $k'K$ và mỗi phần tử của I là đại số và tách được trên $k'(t_1, \ldots, t_n)$. Khi đó L = $k'K$ là một mở rộng tách được của $k'$, có bậc hữu hạn trên K, và $k'$ là một mở rộng xuyên căn hữu hạn của k.

#### Mệnh đề 7 {#ac-x-s6-prop-7 .statement}

Cho k là một trường, A và B là hai đại số trên k, một trong hai đại số đó về cơ bản là kiểu hữu hạn. Giả sử A là chính quy tuyệt đối (resp. chuẩn tắc tuyệt đối). Nếu vành B là chính quy (resp. chuẩn tắc), thì vành $A \otimes_k B$ cũng vậy.

Cho K là một mở rộng kiểu hữu hạn của k; hãy chứng minh rằng vành $A_{(K)}$ là chính quy (resp. chuẩn tắc). Thật vậy, hãy xét các mở rộng L và $k'$ có các tính chất của bổ đề 3. Khi đó vành $A_{(k')}$ là chính quy (resp. chuẩn tắc) theo định nghĩa, và vành $A_{(L)}$, được đồng nhất với $A_{(k')} \otimes_{k'} L$, là chính quy (resp. chuẩn tắc) theo Mệnh đề 5, b) của No. 3. Do đó, $A_{(K)}$ là chính quy (resp. chuẩn tắc) theo Mệnh đề 5, a).

Giả sử vành B là chính quy (resp. chuẩn tắc), và hãy chứng minh mệnh đề. Đồng cấu chính tắc $B \to A \otimes_k B$ làm cho $A \otimes_k B$ thành một B-môđun tự do. Với mọi iđêan nguyên tố $p$ của B, vành $(A \otimes_k B) \otimes_B \kappa(p)$ được đồng nhất với $A \otimes_k \kappa(p)$; theo hệ quả của Mệnh đề 9 của § 4, No. 5 (resp. Hệ quả 3 của Định lý 4 của § 1, No. 10), chỉ cần chứng minh rằng $A \otimes_k \kappa(p)$ là chính quy (resp. chuẩn tắc) với mọi iđêan nguyên tố $p$ của B.

Nếu đại số trên $k$ B về cơ bản là kiểu hữu hạn, thì mở rộng $\kappa(p)$ của $k$ là kiểu hữu hạn và vành $A \otimes_k \kappa(p)$ là chính quy (resp. chuẩn tắc) theo điều đã thấy ở trên. Bây giờ giả sử đại số trên $k$ A về cơ bản là kiểu hữu hạn; vành $A \otimes_k \kappa(p)$ là Noether và là hợp của họ tăng lọc các vành con Noether $\Lambda \otimes_k K$, trong đó $K$ chạy qua các mở rộng con kiểu hữu hạn của $\kappa(p)$. Các vành sau cùng này là chính quy (resp. chuẩn tắc), và ta áp dụng bổ đề 1 của No. 3.

#### Hệ quả 1 {#ac-x-s6-prop-7-cor-1 .statement}

Cho $k$ là một trường. Tích tenxơ của hai đại số trên $k$ chính quy tuyệt đối (resp. chuẩn tắc tuyệt đối), một trong hai đại số đó về cơ bản là kiểu hữu hạn, là một đại số trên $k$ chính quy tuyệt đối (resp. chuẩn tắc tuyệt đối).

Cho $A$ và $B$ là hai đại số trên $k$ thỏa mãn các giả thiết của hệ quả. Cho $k'$ là một mở rộng xuyên căn hữu hạn của $k$. Vành $B_{(k')}$ là chính quy (resp. chuẩn tắc); vành $A \otimes_k B_{(k')}$ là chính quy (resp. chuẩn tắc) theo Mệnh đề 7, cũng như vành $(A \otimes_k B) \otimes_k k'$ đẳng cấu với nó.

#### Hệ quả 2 {#ac-x-s6-prop-7-cor-2 .statement}

Cho $k$ là một trường, $A$ là một đại số trên $k$ chính quy tuyệt đối (resp. chuẩn tắc tuyệt đối), và $K$ là một mở rộng của $k$. Giả sử rằng $A$ về cơ bản là kiểu hữu hạn hoặc mở rộng $K$ của $k$ là kiểu hữu hạn.

a) Vành $\Lambda_{(K)}$ là chính quy (resp. chuẩn tắc).

b) Nếu mở rộng $K$ của $k$ là tách được, thì đại số trên k $A_{(K)}$ là tuyệt đối chính quy (tương ứng, tuyệt đối chuẩn tắc).

Mệnh đề a) suy ra từ mệnh đề 7; mệnh đề b) suy ra từ hệ quả 1 và ví dụ 2.

#### Hệ quả 3 {#ac-x-s6-prop-7-cor-3 .statement}

Cho $k$ là một trường, $A$ một đại số trên k, và $K$ một mở rộng của $k$. Giả sử rằng đại số trên k $A$ về bản chất thuộc kiểu hữu hạn hoặc rằng mở rộng $K$ của $k$ thuộc kiểu hữu hạn. Để đại số trên k $A$ là tuyệt đối chính quy (tương ứng, tuyệt đối chuẩn tắc), điều kiện cần và đủ là đại số trên K $A_{(K)}$ cũng như vậy.

Giả sử $A$ tuyệt đối chính quy (tương ứng, tuyệt đối chuẩn tắc) và cho $K'$ là một mở rộng thuần túy không tách được của $K$ có bậc hữu hạn. Vành $K' \otimes_K \Lambda_{(K)}$, đẳng cấu với $K' \otimes_k A$, là chính quy (tương ứng, chuẩn tắc) theo hệ quả 2.

Ngược lại, giả sử rằng đại số trên K $A_{(K)}$ là tuyệt đối chính quy (tương ứng, tuyệt đối chuẩn tắc), và cho $k'$ là một mở rộng thuần túy không tách được của $k$ có bậc hữu hạn. Gọi $L$ là một mở rộng hợp thành của $k'$ và $K$; khi đó vành $A_{(L)}$ có thể được đồng nhất với $L \otimes_K \Lambda_{(K)}$, do đó là chính quy (tương ứng, chuẩn tắc); do đó, vành $A_{(k')}$ là chính quy (tương ứng, chuẩn tắc) theo mệnh đề 5, a) của No. 3.

#### Hệ quả 4 {#ac-x-s6-prop-7-cor-4 .statement}

Cho $k$ là một trường, $A$ một đại số trên k về bản chất thuộc kiểu hữu hạn, và $K$ một mở rộng của $k$ là một trường hoàn hảo. Để $A$ là tuyệt đối chính quy (tương ứng, tuyệt đối chuẩn tắc), điều kiện cần và đủ là vành $A_{(K)}$ là chính quy (tương ứng, chuẩn tắc).

Điều này suy ra từ hệ quả 3 và ví dụ 1.

### 5. Các đặc trưng của các đại số tuyệt đối chính quy

#### Mệnh đề 8 {#ac-x-s6-prop-8 .statement}

Cho k là một trường và A một đại số trên k về bản chất thuộc kiểu hữu hạn. Gọi I là hạt nhân của đồng cấu các đại số trên k $\mu : A \otimes_k A \to A$ sao cho $\mu(x \otimes y) = xy$ với x và y trong A. Các điều kiện sau là tương đương:

(i) đại số trên k A là tuyệt đối chính quy;
(ii) với mọi đại số trên k chính quy C, vành $A \otimes_k C$ là chính quy;
(iii) vành $A \otimes_k A$ là chính quy;
(iv) iđêan I của $A \otimes_k A$ là hoàn toàn cát tuyến ($§ 5$, No. 1, Định nghĩa 1).

Gọi B là vành $A \otimes_k A$ và trang bị cho nó cấu trúc đại số trên A suy ra từ đồng cấu $\rho : A \to A \otimes_k A$ sao cho $\rho(x) = x \otimes 1$; khi đó $\mu$ là một đồng cấu các đại số trên A, và bằng cách chuyển qua thương, cảm sinh một đẳng cấu từ $B/I$ lên A.

(i) $\Rightarrow$ (ii): điều này suy ra từ Mệnh đề 7.
(ii) $\Rightarrow$ (iii): chỉ cần áp dụng (ii) với $C = k$, rồi với $C = \Lambda$.
(iii) $\Rightarrow$ (iv): A-môđun B là tự do, nên phẳng trung thành. Nếu vành B là chính quy thì A là chính quy ($§ 4$, No. 5, Mệnh đề 8); khi đó iđêan I là cát tuyến hoàn toàn ($§ 5$, No. 3, Mệnh đề 2).
(iv) $\Rightarrow$ (i): giả sử iđêan I là cát tuyến hoàn toàn và trước hết chứng minh rằng A là chính quy. Gọi m là một iđêan cực đại của A và gọi $\nu : (A/m) \otimes_k A \to A/m$ là đồng cấu suy ra từ $\mu$. Iđêan cực đại $n = \mathrm{Ker}\,\nu$ bằng $1((A/m) \otimes_k \Lambda)$; áp dụng Mệnh đề 6 của $§ 5$, No. 6 cho A-đại số $A' = A/m$, ta thấy iđêan n là cát tuyến hoàn toàn trong $(\Lambda/m) \otimes_k \Lambda$. Do đó ($§ 5$, No. 3, Mệnh đề 3) vành địa phương $((A/m) \otimes_k \Lambda)_n$ là chính quy. Kí hiệu bởi $j : \Lambda \to (A/m) \otimes_k A$ đồng cấu $x \mapsto 1 \otimes x$; vì $\nu \circ j$ là đồng cấu chính tắc của A vào $A/m$, ta có $j^{-1}(n) = m$. Vậy j mở rộng thành một đồng cấu địa phương của các vành địa phương từ $A_m$ vào $((A/m) \otimes_k A)_n$, khiến vành sau trở thành một $A_m$-môđun phẳng trung thành. Theo Mệnh đề 8 của $§ 4$, No. 5, do đó vành $A_m$ là chính quy. Như vậy ta đã chứng minh A là chính quy.

Bây giờ gọi $k'$ là một mở rộng của k. Hạt nhân của ánh xạ $\mu' : A_{(k')} \otimes_{k'} \Lambda_{(k')} \to A_{(k')}$ suy ra từ phép nhân của $A_{(k')}$ không gì khác hơn là $IA_{(k')}$; do đó nó là cát tuyến hoàn toàn trong $A_{(k')}$ ($§ 5$, No. 6, Mệnh đề 6). Vậy $k'$-đại số $A_{(k')}$ thỏa mãn điều kiện (iv); theo điều vừa thấy, nó là chính quy, và điều này chứng minh (i).

Nhắc lại (A, III, p. 133-134) rằng thương $I/I^2$ được trang bị cấu trúc A-môđun suy ra từ $\rho$ được kí hiệu bởi $\Omega_k(A)$ và được gọi là môđun các k-vi phân của A. Khi k-đại số A là kiểu hữu hạn về bản chất, vành $A \otimes_k A$ là Noether, nên A-môđun $\Omega_k(A)$ là hữu hạn sinh.

Người ta kí hiệu bởi $d_{A/k}$, hoặc đơn giản là d, ánh xạ K-tuyến tính từ A vào $\Omega_k(A)$ gán cho một phần tử x của A lớp của $x \otimes 1 - 1 \otimes x$ trong $\Omega_k(A)$. Ánh xạ d là một k-đạo hàm; với mọi A-môđun M và mọi k-đạo hàm D : A $\to$ M, tồn tại duy nhất một ánh xạ A-tuyến tính $g : \Omega_k(\Lambda) \to M$ sao cho $D = g \circ d$ (loc. cit., Mệnh đề 18).

Nếu S là một tập con nhân của A, ánh xạ $S^{-1}A$-tuyến tính chính tắc (loc. cit., p. 136)
$$
S^{-1}\Omega_k(A) \to \Omega_k(S^{-1}A)
$$
là song ánh: thật vậy, chỉ cần kiểm tra rằng, với mọi $S^{-1}A$-môđun M, mọi k-đạo hàm D : A \to M đều mở rộng theo một cách duy nhất thành một k-đạo hàm D : S^{-1}A \to M; nhưng điều này suy ra từ lập luận của loc. cit., p. 123, Mệnh đề 5.

Gọi k là một trường và A là một k-đại số địa phương kiểu hữu hạn về bản chất. Đặt n = \dim(A) + \deg.\mathrm{tr}_k(\kappa_A). Gọi B là một k-đại số kiểu hữu hạn và q là một iđêan nguyên tố của B sao cho k-đại số A đẳng cấu với $B_q$ (xem No. 1, Ví dụ 2); ta có n = \dim_q(B) (VIII, § 2, No. 4, Hệ quả 5 của Định lý 3). Theo loc. cit., Định lý 3, c) và Hệ quả 5, ta cũng có
$$
n = \sup \deg.\mathrm{tr}_k(\kappa(\mathfrak{p}))
$$
trong đó \mathfrak{p} chạy qua họ (hữu hạn) các iđêan nguyên tố cực tiểu của A. Nếu A là một miền nguyên, thì n do đó là bậc siêu việt của trường phân thức của A.

#### Định lý 1 {#ac-x-s6-thm-1 .statement}

*Gọi k là một trường và A là một k-đại số địa phương kiểu hữu hạn về bản chất. Đặt n = \dim(A) + \deg.\mathrm{tr}_k(\kappa_A).*

a) *Ta có [\kappa_A \otimes_A \Omega_k(A) : \kappa_A] \geq n.*

b) *Các điều kiện sau là tương đương:*
(i) *k-đại số A là chính quy tuyệt đối;*
(ii) *A-môđun \Omega_k(A) là tự do hạng n;*
(iii) *ta có [\kappa_A \otimes_A \Omega_k(A) : \kappa_A] = n.*

Xét mệnh đề
(iii') *ta có [\kappa_A \otimes_A \Omega_k(A) : \kappa_A] \leq n;*
rõ ràng là (ii) suy ra (iii) và (iii) suy ra (iii'). Để chứng minh định lý, chỉ cần chứng minh các hệ quả (i) \Rightarrow (ii) và (iii') \Rightarrow (i).

Chọn một k-đại số kiểu hữu hạn B và một iđêan nguyên tố q của B sao cho A đẳng cấu với $B_q$ (No. 1, Ví dụ 2). Ta có \dim_q(B) = n; thay thế B bằng một vành $B_f$ , với $f \in B - q$, ta có thể giả thiết rằng phổ của B là liên thông và có chiều n, và từ đây về sau ta sẽ giả sử như vậy.

(i) \Rightarrow (ii): Giả sử k-đại số A là chính quy tuyệt đối. Như trong chứng minh của Mệnh đề 8, kí hiệu bởi \mu : A \otimes_k A \to A và \nu : \kappa_A \otimes_k A \to \kappa_A các đồng cấu suy ra từ phép nhân của A; đặt I = \mathrm{Ker}(\mu) và n = \mathrm{Ker}(\nu). Iđêan I là cát tuyến hoàn toàn; iđêan n là cực đại và vành địa phương (\kappa_A \otimes_k A)_n là chính quy (loc. cit.). Theo Định lý 1 của § 5, No. 2, A-môđun hữu hạn sinh I/I^2, không gì khác hơn là \Omega_k(A), là xạ ảnh, nên tự do. Nhưng theo nhận xét của § 5, No. 6, iđêan n đồng nhất với \kappa_A \otimes_A 1, nên n/n^2 đẳng cấu với \kappa_A \otimes_A \Omega_k(A). Do đó ta có
$$
\mathrm{rg}(\Omega_k(A)) = [\kappa_A \otimes_k \Omega_k(A) : \kappa_A] = [n/n^2 : \kappa_A] = \dim(\kappa_A \otimes_k A)_n .
$$

Kí hiệu bởi B' vành \kappa_A \otimes_k B, và bởi S ảnh trong B' của B - q. Vành \kappa_A \otimes_k A đồng nhất với $B' \otimes_B B_q$, tức là với $S^{-1}B'$. Do đó tồn tại một iđêan cực đại q' của B' không cắt S sao cho ta có n = $S^{-1}q'$; khi đó vành (\kappa_A \otimes_k A)_n đẳng cấu với $B'_{q'}$ , và ta có

$$
\dim(\kappa_A \otimes_k A)_n = \dim(\kappa_A \otimes_k B)_{q'} = \dim_{q'}(\kappa_A \otimes_k B)
$$

Vì n chứa \kappa_A \otimes_k qB_q , q' chứa iđêan \kappa_A \otimes q của B' , nên ảnh ngược của nó trong B chứa q ; nó bằng q vì q' không cắt S . Theo VIII, § 2, No. 4, hệ quả của mệnh đề 5, ta có

$$
\dim_{q'}(\kappa_A \otimes_k B) = \dim_q(B) = n ,
$$

điều đó chứng minh (ii).

(iii') \Rightarrow (i) : Giả sử rằng ta có [\kappa_A \otimes_A \Omega_k(\Lambda) : \kappa_A] \leq n , tức là [\kappa(q) \otimes_B \Omega_k(B) : \kappa(q)] \leq n , và hãy chứng minh rằng đại số trên k B là tuyệt đối chính quy. Cho (x_1, \ldots , x_n) là một dãy các phần tử của B sao cho 1 \otimes dx_1, \ldots , 1 \otimes dx_n sinh không gian vectơ \kappa(q)-không gian vectơ \kappa(q) \otimes_B \Omega_k(B) . Thay thế B bằng B_f , với một phần tử thích hợp f của B - q , ta có thể giả sử rằng dx_1, \ldots , dx_n sinh B-môđun \Omega_k(B) (bổ đề Nakayama và II, § 5, No. 1, mệnh đề 2). Cho \bar{k} là một mở rộng đóng đại số của k . Chỉ cần chứng minh rằng đại số trên \bar{k} B_{(\bar{k})} là chính quy, vì điều đó sẽ kéo theo rằng B là tuyệt đối chính quy (hệ quả 4 của mệnh đề 7 ở No. 4). Với mọi nhân tử chính tắc C của B_{(k)} , các vi phân d(1 \otimes x_i) sinh C-môđun \Omega_{\bar{k}}(C) (A, III, § 10, No. 12, mệnh đề 20). Do đó định lý suy ra từ hai bổ đề sau đây:

#### Bổ đề 4 {#ac-x-s6-lem-4 .statement}

Cho k là một trường, K là một mở rộng đại số của k , B là một đại số trên k mà phổ là liên thông. Với mọi nhân tử chính tắc C của B_{(K)} , ta có \dim(C) = \dim(B) .

Trước hết hãy xét trường hợp trong đó mở rộng K có bậc hữu hạn trên k . B-môđun C là một nhân tử trực tiếp của một môđun tự do, nên xạ ảnh sinh hữu hạn. Vì hàm p \mapsto \mathrm{rg}_p C là hằng trên Spec(B) (II, § 5, No. 3), giá đỡ của B-môđun C bằng Spec(B) , do đó B-môđun C là phẳng trung thành. Điều này kéo theo \dim(C) \geq \dim(B) (VIII, § 2, No. 1, mệnh đề 2), do đó có đẳng thức cần chứng minh vì ta có \dim(C) \leq \dim(B_{(K)}) = \dim(B) (VIII, § 2, No. 4, hệ quả của mệnh đề 5).

Hãy chuyển sang trường hợp tổng quát. Cho e là phần tử lũy đẳng của B_{(K)} sao cho C = B_{(K)}/B_{(K)}e . Tồn tại một mở rộng con K' của K có bậc hữu hạn sao cho e là ảnh của một phần tử lũy đẳng e' của B_{(K')} . Đặt C' = B_{(K')}/B_{(K')}e' . Vành C' \otimes_{K'} K được đồng nhất với C , và C' là một nhân tử chính tắc của B_{(K')} . Ta có \dim(C') = \dim(B) theo trường hợp đã xét, và \dim(C') = \dim(C) theo loc. cit. , do đó bổ đề được chứng minh.

#### Bổ đề 5 {#ac-x-s6-lem-5 .statement}

Cho k là một trường đóng đại số, A là một đại số trên k sinh hữu hạn mà phổ là liên thông, n là một số nguyên và (x_1, \ldots , x_n) là một dãy hữu hạn các phần tử của A . Giả sử rằng A có chiều n và các vi phân dx_1, \ldots , dx_n sinh A-môđun \Omega_k(A) . Khi đó vành A là một miền nguyên và chính quy và A-môđun \Omega_k(A) là tự do với cơ sở (dx_1, \ldots , dx_n) .

Cho m là một iđêan cực đại của A sao cho \dim(A_m) = n . Ta có [A/m : k] = 1 (V, § 3, No. 3, mệnh đề 1 (iii)), do đó A = m \oplus k1_A . Ký hiệu p và q là các phép chiếu tương ứng. Với $a$ và $b$ trong $\Lambda$, ta có
$$
ab = (p(a)q(b) + q(a)p(b) + p(a)p(b), q(a)q(b)) ,
$$
do đó $p(ab) \equiv p(a)q(b) + q(a)p(b) \pmod{\mathfrak{m}^2}$. Vì vậy ánh xạ $\delta : \Lambda \to \mathfrak{m}/\mathfrak{m}^2$ gán cho mỗi phần tử $x$ của $\Lambda$ lớp của $p(x)$ modulo $\mathfrak{m}^2$ là một $k$-đạo hàm từ $\Lambda$ vào không gian vectơ trên $k$ $\mathfrak{m}/\mathfrak{m}^2$. Do đó tồn tại một ánh xạ tuyến tính theo $\Lambda$ $\phi : \Omega_k(\Lambda) \to \mathfrak{m}/\mathfrak{m}^2$ sao cho $\delta(x) = \phi(dx)$ với mọi $x \in \Lambda$. Vì $\delta$ là toàn ánh, các $\phi(dx_i)$ sinh không gian vectơ trên $\Lambda/\mathfrak{m}$ $\mathfrak{m}/\mathfrak{m}^2$, và ta có $[\mathfrak{m}/\mathfrak{m}^2 : \Lambda/\mathfrak{m}] \leq n = \dim(A_{\mathfrak{m}})$. Suy ra $A_{\mathfrak{m}}$ là chính quy và các ảnh của các $dx_i$ lập thành một cơ sở của không gian vectơ trên $\Lambda/\mathfrak{m}$ $\Lambda/\mathfrak{m} \otimes_A \Omega_k(\Lambda)$.

Bây giờ hãy chứng minh rằng vành $\Lambda$ là một miền nguyên và chính quy. Tồn tại một iđêan nguyên tố cực tiểu $\mathfrak{q}$ của $\Lambda$ sao cho $\dim(\Lambda/\mathfrak{q}) = n$. Với mọi iđêan cực đại $\mathfrak{m}$ của $\Lambda$ chứa $\mathfrak{q}$, ta có $\dim(A_{\mathfrak{m}}) = n$ (VIII, § 2, No. 4, hệ quả 2 của định lý 3), do đó $A_{\mathfrak{m}}$ là chính quy theo điều ta vừa thấy. Đặc biệt $A_{\mathfrak{m}}$ là một miền nguyên, điều này kéo theo $\mathfrak{q}A_{\mathfrak{m}} = 0$. Vì điều này đúng với mọi iđêan cực đại $\mathfrak{m}$ của $V(\mathfrak{q})$, ta suy ra rằng $\operatorname{Supp}(\mathfrak{q}) \cap V(\mathfrak{q}) = \varnothing$. Nhưng $\operatorname{Spec}(\Lambda)$ là liên thông, $V(\mathfrak{q})$ là khác rỗng và ta có $\operatorname{Supp}(\mathfrak{q}) \cup V(\mathfrak{q}) = \operatorname{Spec}(\Lambda)$ (II, § 4, No. 4, mệnh đề 16). Ta suy ra rằng $\operatorname{Supp}(\mathfrak{q}) = \varnothing$, do đó $\mathfrak{q} = 0$, nghĩa là $\Lambda$ là một miền nguyên. Khi đó ta có $\dim(A_{\mathfrak{m}}) = n$ với mọi iđêan cực đại $\mathfrak{m}$ của $\Lambda$; áp dụng phần đầu của chứng minh, ta suy ra rằng $\Lambda$ là chính quy.

Cuối cùng, giả sử $\sum_{i=1}^n a_i dx_i = 0$ là một quan hệ tuyến tính giữa các $dx_i$ với các hệ số trong $\Lambda$. Nếu các $a_i$ không đồng thời bằng không, thì tồn tại một chỉ số $i$ và một iđêan cực đại $\mathfrak{m}$ của $\Lambda$ sao cho $a_i$ không thuộc $\mathfrak{m}$ (V, § 3, No. 3, Prop. 1, (iii) và (iv)); nhưng điều này mâu thuẫn với sự kiện đã chứng minh ở trên rằng các lớp của $dx_i$ trong $(\Lambda/\mathfrak{m}) \otimes_A \Omega_k(\Lambda)$ là độc lập tuyến tính.

#### Ví dụ {#ac-x-s6-n5-exa-1 .statement}

Khi $\Lambda$ là một mở rộng hữu hạn kiểu của $k$, định lý 1 lại cho Hệ quả 1 của A, V, p. 128, nếu tính đến Ví dụ 2 của No. 4.

#### Hệ quả 1 {#ac-x-s6-lem-5-cor-1 .statement}

*Cho $k$ là một trường và $\Lambda$ là một $k$-đại số về bản chất là hữu hạn kiểu. Tập hợp các phần tử $\mathfrak{p}$ của $\operatorname{Spec}(\Lambda)$ sao cho $k$-đại số $\Lambda_{\mathfrak{p}}$ là chính quy tuyệt đối là một tập mở trong $\operatorname{Spec}(\Lambda)$.*

Ta có thể giả sử rằng $k$-đại số $\Lambda$ là hữu hạn kiểu. Khi đó tập hợp đang xét được tạo thành bởi các iđêan nguyên tố $\mathfrak{p}$ sao cho $[\kappa(\mathfrak{p}) \otimes_k \Omega_k(\Lambda) : \kappa(\mathfrak{p})] \leq \dim_{\mathfrak{p}}(\Lambda)$. Mà ánh xạ $\mathfrak{p} \mapsto \dim_{\mathfrak{p}}(\Lambda)$ là nửa liên tục dưới theo định nghĩa, và ánh xạ $\mathfrak{p} \mapsto [\kappa(\mathfrak{p}) \otimes_k \Omega_k(\Lambda) : \kappa(\mathfrak{p})]$ là nửa liên tục trên (bổ đề Nakayama và II, § 5, No. 1, Mệnh đề 2).

Ta sẽ thấy về sau (§ 7, No. 9, Hệ quả 4 của Định lý 3) rằng dưới các giả thiết của Hệ quả 1, tập hợp các iđêan nguyên tố $\mathfrak{p}$ của $\Lambda$ sao cho vành $\Lambda_{\mathfrak{p}}$ là chính quy là một tập mở trong $\operatorname{Spec}(\Lambda)$.

#### Hệ quả 2 {#ac-x-s6-lem-5-cor-2 .statement}

*Cho $k$ là một trường và $\Lambda$ là một $k$-đại số về bản chất là hữu hạn kiểu. Điều kiện cần và đủ để $\Lambda$ là chính quy tuyệt đối là $\Lambda$-môđun $\Omega_k(\Lambda)$ là xạ ảnh và với mọi iđêan nguyên tố cực tiểu $\mathfrak{q}$ của $\Lambda$, $k$-đại số $\Lambda_{\mathfrak{q}}$ là tách được.*

Ngược lại, giả sử rằng $A$-môđun $\Omega_k(A)$ là xạ ảnh và $k$-đại số $A_q$ là tách được đối với mọi iđêan nguyên tố cực tiểu $q$ của $A$. Cho $p$ là một iđêan nguyên tố của $A$, và $q$ là một iđêan nguyên tố cực tiểu của $A$ được chứa trong $p$. Vì $A_p$-môđun $\Omega_k(A)_p$ là tự do (II, § 3, No. 2, Hệ quả 2 của Mệnh đề 5), ta có

$$
[\kappa(p) \otimes_A \Omega_k(A) : \kappa(p)] = [\kappa(q) \otimes_A \Omega_k(A) : \kappa(q)] .
$$

$k$-đại số $A_q$ là Artin và tách được, nên chính quy tuyệt đối (No. 4, Ví dụ 2). Định lý 1 suy ra

$$
[\kappa(q) \otimes_A \Omega_k(A) : \kappa(q)] = \deg.\operatorname{tr}_k(\kappa(q)) .
$$

Khi đó từ Định lý 1 suy ra rằng $k$-đại số $A_p$ là chính quy tuyệt đối, do đó có hệ quả.

#### Nhận xét {#ac-x-s6-n5-rem-1 .statement}

Giả sử $k$-đại số $A$ là chính quy tuyệt đối. Khi đó vành phân thức toàn phần $F$ của $A$ được đồng nhất với tích của các $A_q$, trong đó $q$ chạy qua tập hợp các iđêan nguyên tố cực tiểu của $A$ (IV, § 2, No. 5, Mệnh đề 10); do đó nó là một $k$-đại số tách được. Ngược lại, giả sử rằng $F$ là một $k$-đại số tách được; với mọi iđêan nguyên tố cực tiểu $q$ của $A$, $k$-đại số $A_q$ là một vành phân thức của $F$ (IV, § 1, No. 1, Hệ quả 3 của Mệnh đề 2 và No. 3, Hệ quả 1 của Mệnh đề 7), vì thế là một $k$-đại số tách được (No. 4, Mệnh đề 6). Nếu hơn nữa $A$-môđun $\Omega_k(A)$ là xạ ảnh, thì theo Hệ quả 2 suy ra $k$-đại số $A$ là chính quy tuyệt đối.

#### Hệ quả 3 {#ac-x-s6-lem-5-cor-3 .statement}

Cho $k$ là một trường có đặc số 0 và $A$ là một $k$-đại số thiết yếu kiểu hữu hạn. Để $A$ là chính quy, điều kiện cần và đủ là $A$-môđun $\Omega_k(A)$ là xạ ảnh.

Theo Hệ quả 2, chỉ cần chứng minh rằng một $k$-đại số địa phương Artin $A$ sao cho $\Omega_k(A)$ là một $A$-môđun tự do thì là một trường. Bây giờ, theo IX, § 3, No. 3, Định lý 1, tồn tại một trường con $K$ của $A$ sao cho $A = K \oplus m_A$. Gọi $\delta : A \to m_A/m_A^2$ là ánh xạ hợp thành của phép chiếu từ $A$ lên $m_A$ và ánh xạ chính tắc $m_A \to m_A/m_A^2$. Ta kiểm tra như trong chứng minh của Bổ đề 4 rằng $\delta$ là một $k$-đạo hàm. Nhưng mọi $k$-đạo hàm từ $A$ vào một $A$-môđun đều triệt tiêu $m_A$: thật vậy, lấy $x \in m_A$, và $n$ là một số nguyên $\geq 1$ sao cho ta có $x^{n-1} \neq 0,\ x^n = 0$. Điều này kéo theo trong $A$-môđun $\Omega_k(A)$ quan hệ $nx^{n-1} dx = 0$, do đó $dx = 0$ vì $nx^{n-1} \neq 0$. Vậy $\delta(m_A) = 0$, suy ra $m_A = m_A^2$, và cuối cùng $m_A = \{0\}$.

## BÀI TẬP {#ac-x-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
