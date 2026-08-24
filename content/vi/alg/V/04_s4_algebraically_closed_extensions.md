---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 4
section_title: Algebraically closed extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.19-A V.24, A V.150
pdf_pages: 0133-0138, 0264-0264
extraction: ocr
subsections:
    - "no": 1
      title: Algebraically closed fields
      page: 19
      pdf_page: 133
    - "no": 2
      title: Splitting extensions
      page: 21
      pdf_page: 135
    - "no": 3
      title: Algebraic closure of a field
      page: 22
      pdf_page: 136
statements: 14
exercises: 2
content_sha256: af083a916a78ebc4ab059c6576650119f234f4edf9f2df0a3e92430e4fc5d2a7
translated_from: content/en/alg/V/04_s4_algebraically_closed_extensions.md
source_content_sha256: 9d6d7fa70f7929549a2c8e43cd77e6ece671a7036f47fbeaed414983bf08cec1
translation_model: gpt-5.4
translation_run: translate-vi-e35f2d1f
glossary_version: 34
glossary_terms_sha256: bfd7d47a310724b7cbb9da44ea827216a62a7b066ad66fabd350b2c3c88863f1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CÁC MỞ RỘNG ĐÓNG ĐẠI SỐ

### 1. Các trường đóng đại số

#### Mệnh đề 1 {#alg-v-s4-prop-1 .statement}

— Cho K là một trường; khi đó các tính chất sau là tương đương:
(AC) Mọi đa thức không hằng của K[X] đều phân tích trong K[X] thành một tích các đa thức bậc 1 (phân biệt hay không).
(AC') Mọi đa thức không hằng của K[X] đều có ít nhất một nghiệm trong K.
(AC'') Mọi đa thức bất khả quy trong K[X] đều có bậc 1.

(AC) Mọi mở rộng đại số của K đều có bậc 1 (nói cách khác, K đóng đại số tương đối trong mọi trường mở rộng của K).

Trước hết ta chứng minh tính tương đương của các tính chất (AC), (AC') và (AC''). Rõ ràng (AC) kéo theo (AC). Vì mọi đa thức không hằng của K[X] đều chia hết cho một đa thức bất khả quy (IV, p. 13, Mệnh đề 13) và mọi đa thức bậc 1 trong K[X] rõ ràng đều nhận một nghiệm trong K, ta thấy rằng (AC) kéo theo (AC'). Điều kiện (AC') kéo theo, bằng quy nạp theo n, rằng mọi đa thức bậc n trong K[X] là một tích của n đa thức bậc 1 (IV, p. 14, Mệnh đề 1), do đó (AC') kéo theo (AC).

Còn lại phải thấy rằng (AC) và (AC) là tương đương. Nếu (AC'') đúng, mọi phần tử của một trường mở rộng L của K mà đại số trên K đều có bậc 1 (V, p. 16, Định lý 1), do đó thuộc K, điều này thiết lập (AC). Ngược lại, cho f là một đa thức bất khả quy bậc $ n \geq 1 $ trong K[X]; đại số thương K[X]/(f) có bậc n trên K và là một trường, do đó là một mở rộng đại số bậc n của K (V, p. 18, Mệnh đề 2). Bây giờ rõ ràng là (AC) kéo theo (AC'').

Định nghĩa 1. — Một trường K được gọi là đóng đại số nếu nó có các tính chất (tương đương) (AC), (AC'), (AC), (AC).

\* Ví dụ 1. — Trường C các số phức là đóng đại số (Gen. Top., VIII, p. 100). \*

Một trường K đóng đại số tương đối trong một trường mở rộng E của K không nhất thiết là đóng đại số (thật vậy mọi trường đều đóng đại số tương đối trong chính nó, và có những trường không đóng đại số, chẳng hạn Q hoặc $ \mathbf{F}_p $ \* hoặc R *). Tuy nhiên:

Mệnh đề 2. — Cho $ \Omega $ là một trường đóng đại số và K là một trường con của $ \Omega $. Khi đó bao đóng đại số tương đối $ \bar{K} $ của K trong $ \Omega $ là một trường đóng đại số.

Cho f là một đa thức không hằng trong $ \bar{K}[X] \subset \Omega[X] $. Vì $ \Omega $ đóng đại số, đa thức f có ít nhất một nghiệm trong $ \Omega $, và vì nghiệm này đại số trên $ \bar{K} $, nó thuộc $ \bar{K} $ (V, p. 19, Mệnh đề 4). Vậy $ \bar{K} $ thỏa mãn (AC').

\* Ví dụ 2. — Theo Mệnh đề 2, tập hợp tất cả các số phức đại số trên Q (thường được gọi vắn tắt là các số đại số) là một trường đóng đại số. \*

Mệnh đề 3. — Mọi trường đóng đại số đều vô hạn.

Cho K là một trường hữu hạn và đặt $ f(X) = 1 + \prod_{a \in K} (X - a) $. Đa thức $ f \in K[X] $ không hằng và $ f(a) = 1 $ với mỗi $ a \in K $. Vậy trường K không thỏa mãn (AC') và do đó không đóng đại số.

#### Định lý 1 (Steinitz) {#alg-v-s4-thm-1 .statement}

Cho K là một trường, E là một mở rộng đại số của K và $ \Omega $ là một mở rộng đóng đại số của K; khi đó tồn tại một K-đồng cấu của E vào R.

Theo V, p. 13, Chú giải, tồn tại một trường mở rộng $ \Omega' $ của $ \Omega $ và một K-đồng cấu u của E vào $ \Omega' $. Cho $ x \in E $; vì x đại số trên K, u(x) đại số trên u(K) và *a fortiori* trên $ \Omega $ (V, p. 17, Hệ quả 2); vì $ \Omega $ đóng đại số, do đó ta có $ u(x) \in O $. Suy ra $ u $ ánh xạ $ E $ vào $ O $.

### 2. Các mở rộng tách

#### Định nghĩa 2 {#alg-v-s4-def-2 .statement}

*Cho K là một trường và $ (f_i)_{i \in I} $ là một họ các đa thức không hằng trong $ K[X] $. Bởi một mở rộng phân rã của $ (f_i)_i $, ta hiểu là mọi mở rộng $ E $ của $ K $ có các tính chất sau :*

*a) Với mỗi $ i \in I $, đa thức $ f_i $ phân rã trong $ E[X] $ thành một tích các đa thức bậc 1.*

*b) Với mỗi $ i \in I $ gọi $ R_i $ là tập hợp các nghiệm của $ f_i $ trong $ E $, khi đó $ E = K \left( \bigcup_{i \in I} R_i \right) $.*

Đôi khi thuật ngữ « trường phân rã » được dùng thay cho « mở rộng phân rã ».

*Nhận xét. — 1) Với mỗi $ i \in I $ lấy $ c_i $ là một phần tử khác không của $ K $ và đặt $ f'_i = c_i f_i $. Khi đó hiển nhiên là mọi mở rộng tách của họ $ (f_i)_i $, cũng là một mở rộng tách của họ $ (f'_i)_{i \in I} $ và ngược lại. Đặc biệt, khi nghiên cứu các mở rộng tách, ta có thể chỉ cần xét trường hợp các đa thức đơn nhất.*

*2) Giả sử rằng I là hữu hạn và đặt $ f = \prod_{i \in I} f_i $. Sử dụng tính duy nhất của phân tích một đa thức thành các nhân tử bất khả quy trong $ E[X] $ (IV, p. 13, Mệnh đề 13), ta dễ dàng chứng minh rằng một mở rộng tách của đa thức $ f $ là một mở rộng tách của họ $ (f_i)_i $, và ngược lại. Nói cách khác, trường hợp một họ hữu hạn có thể quy về trường hợp một đa thức duy nhất.*

*3) Cho $ f \in K[X] $ là một đa thức bậc $ \geq 1 $ và cho $ E $ là một mở rộng tách của $ f $. Nếu $ x_1, \ldots, x_n $ là các nghiệm của f trong $ E $, thì do đó ta có $ E = K(x_1, \ldots, x_n) $ và $ [E : K] $ là hữu hạn ($ V $, p. 18, Th. 2); nhưng có thể xảy ra rằng $ E $ phân biệt với các trường con $ K(x_1), \ldots, K(x_n) $ được sinh bởi một nghiệm duy nhất; điều này có thể xảy ra ngay cả khi $ f $ là bất khả quy$^1$. Tuy nhiên, ta chú ý rằng khi $ f $ là bất khả quy, các trường $ K(x_i) $ đều có cùng bậc $ n $ trên $ K $, và mỗi khi $ E $ bằng một trong các trường đó, ta có $ [E : K] = n $ và do đó $ E = K(x_1) = \cdots = K(x_n) $.*

#### Mệnh đề 4 {#alg-v-s4-prop-4 .statement}

*Cho K là một trường và $ (f_i)_{i \in I} $ là một họ các đa thức không hằng trong $ K[X] $; khi đó tồn tại một mở rộng tách cho họ $ (f_i)_{i \in I} $.*

Ta có thể giả sử các đa thức $ f_i $ là đơn nhất (Nhận xét 1). Cho $ i \in I $ và gọi bậc của $ f_i $ là $ d_i $. Theo IV, p. 73, Mệnh đề 5, tồn tại một đại số giao hoán $ A $ trên $ K $, không thu về 0, và các phần tử $ \xi_{i,1}, \ldots, \xi_{i,d_i} $ của $ A_i $ sao cho:

*a) đại số $ A_i $ được sinh bởi $ (\xi_{i,1}, \ldots, \xi_{i,d_i}) $;*

\footnotetext{1 Lấy chẳng hạn $ K = \mathbf{Q} $ và $ f = X^3 - 2 $.}

b) ta có $ f_i(X) = \prod_{k=1}^{d_i} (X - \xi_{i,k}) $ trong $ A_i[X] $.

Gọi $ A $ là tích tenxơ của họ các đại số $ (A,)_{i} $, và gọi $ \varphi_i $ là đồng cấu chính tắc từ $ A_i $ vào $ A $ (III, p. 470). Khi đó đại số $ A $ là giao hoán và khác 0; do đó, theo định lý Krull (I, p. 104), tồn tại một iđêan cực đại $ a $ trong $ A $ và $ E = A/a $ là một mở rộng của trường $ K $.

Ký hiệu $ \psi $ là đồng cấu chính tắc từ $ A $ vào $ E $ và đặt $ x_{i,k} = \psi(\varphi_i(\xi_{i,k})) $ với $ i \in I $ và $ l \leq k \leq d_i $. Vì đại số $ A $ được sinh bởi $ \bigcup \varphi_i(A_i) $, mở rộng $ E $ được sinh bởi họ $ (x_{i,k}) $. Hơn nữa, ta có $ i \in I $

$$
f_i(X) = \prod_{k=1}^{d_i} (X - x_{i,k}) \text{ in } E[X]. $$

Vậy $ E $ là một mở rộng tách của họ $ (f_i)_{i \in I} $.

#### Mệnh đề 5 {#alg-v-s4-prop-5 .statement}

— *Cho K là một trường, $ (f_i)_{i \in I} $ là một họ các đa thức không hằng trong $ K[X] $, E là một mở rộng của K, và F, F' là các mở rộng con của E mà mỗi cái đều là một mở rộng tách của $ (f_i)_{i \in I} $. Khi đó $ F = F' $.

Gọi $ R_i $ là tập các nghiệm của $ f_i $ trong E và $ R = \bigcup_{i \in I} R_i $. Vì $ f_i $ là một tích các đa thức bậc nhất nằm trong $ F[X] $, ta có $ R_i \subset F $. Theo Định nghĩa 2, ta có $ F = K(R) $; theo cùng cách đó, ta thấy $ F = K(R) $.

#### Hệ quả {#alg-v-s4-n2-cor-1 .statement}

— *Cho K là một trường, $ (f_i)_{i \in I} $, một họ các đa thức không hằng trong $ K[X] $ và F, F' là các mở rộng tách của $ (f_i)_{i \in I} $. Khi đó tồn tại một K-đẳng cấu từ F lên F.

Điều này suy ra từ Mệnh đề 5 và V, p. 13, Hệ quả của Mệnh đề 4.

### 3. Bao đóng đại số của một trường

#### Định nghĩa 3 {#alg-v-s4-def-3 .statement}

— *Cho K là một trường. Một bao đóng đại số của K được hiểu là bất kỳ mở rộng nào của K vừa đại số vừa đóng đại số.

#### Ví dụ {#alg-v-s4-n3-exa-1 .statement}

— *1) Trường C của các số phức là một bao đóng đại số của trường R của các số thực (Gen. Top., VIII, p. 100) \*
2) Cho K là một trường và $ \Omega $ là một mở rộng đóng đại số của K. Nếu $ \overline{K} $ là bao đóng đại số tương đối của K trong $ \Omega $, thì theo V, p. 20, Prop. 2, K là một bao đóng đại số của K. \* Đặc biệt, trường của mọi số đại số (V, p. 20, Ex. 2) là một bao đóng đại số của trường Q của các số hữu tỉ. \*

#### Mệnh đề 6 {#alg-v-s4-prop-6 .statement}

— *Để $ \Omega $ là một bao đóng đại số của một trường K thì điều kiện cần và đủ là $ \Omega $ là đại số và mỗi đa thức không hằng trong $ K[X] $ đều tách trong $ \Omega[X] $ thành một tích các thừa số bậc 1.

Điều kiện là cần thiết theo (AC). Ngược lại, giả sử rằng $ \Omega $ là đại số trên $ K $ và mọi đa thức không hằng của $ K[X] $ là một tích trong $ \Omega[X] $ của các nhân tử bậc 1. Gọi $ \Omega' $ là một mở rộng đại số của $ \Omega $ và lấy $ x \in \Omega' $. Vì $ x $ là đại số trên $ \Omega $ và $ \Omega $ là đại số trên $ K $, nên $ x $ là đại số trên $ K $ (V, p. 19, Mệnh đề 3). Gọi $ f $ là đa thức tối tiểu của $ x $ trên $ K $. Theo giả thiết, đa thức $ f \in K[X] $ phân tích trong $ \Omega[X] $ thành một tích các nhân tử bậc 1, do đó $ x \in \Omega $. Vậy ta có $ \Omega' = \Omega $ và $ \Omega $ là đóng đại số vì nó thỏa mãn (AC).

#### Nhận xét 1 {#alg-v-s4-n3-rem-1 .statement}

— Nếu $ \Omega $ là đại số trên $ K $ và nếu mọi đa thức không hằng của $ K[X] $ đều có một nghiệm trong $ \Omega $ thì $ \Omega $ là một bao đóng đại số của $ K $ (V, p. 156, Bài tập 20).

#### Mệnh đề 7 {#alg-v-s4-prop-7 .statement}

— *Cho $ \Omega $ là một mở rộng đại số của một trường $ K $.
a) Nếu $ \Omega $ đóng đại số, thì mọi mở rộng đại số của $ K $ đều đẳng cấu với một mở rộng con của $ \mathbf{R} $.
b) Ngược lại, giả sử rằng mọi mở rộng đại số bậc hữu hạn của $ K $ đều đẳng cấu với một mở rộng con của $ \Omega $; khi đó $ \Omega $ đóng đại số.*

Mệnh đề *a)* suy ra từ Định lý 1 (V, p. 20). Bây giờ giả sử các giả thiết của *b)* và xét một đa thức không hằng $ f \in K[X] $. Gọi E là một trường phân rã của $ f $ (V, p. 21, Mệnh đề 4); vì E là đại số bậc hữu hạn trên $ K $ (V, p. 18, Định lý 2), ta có thể giả sử rằng E là một mở rộng con của $ \Omega $. Khi đó đa thức $ f $ là một tích các đa thức bậc 1 trong $ \Omega[X] $ và Mệnh đề 6 cho thấy rằng $ \Omega $ đóng đại số.

Bây giờ ta có thể chứng minh sự tồn tại và tính duy nhất (sai khác bởi đẳng cấu) của bao đóng đại số của một trường.

#### Định lý 2 (Steinitz) {#alg-v-s4-thm-2 .statement}

— *Cho $ K $ là một trường; khi đó tồn tại một bao đóng đại số của $ K $. Nếu $ \Omega $ và $ \Omega' $ là hai bao đóng đại số của $ K $, thì tồn tại một $ K $-đẳng cấu từ $ \Omega $ lên $ \Omega' $.*

Theo Mệnh đề 6, một bao đóng đại số của $ K $ không là gì khác ngoài một mở rộng tách của tập hợp tất cả các đa thức không hằng trong $ K[X] $. Do đó Định lý 2 suy ra từ V, p. 21, Mệnh đề 4 và V, p. 22, Hệ quả.

#### Hệ quả {#alg-v-s4-n3-cor-1 .statement}

— *Cho $ K $ và $ K' $ là hai trường, $ \Omega $ là một bao đóng đại số của $ K $ và $ \Omega' $ là một bao đóng đại số của $ K' $. Với mọi đẳng cấu $ u $ của $ K $ lên $ K' $ đều tồn tại một đẳng cấu $ v $ của $ \Omega $ lên $ \Omega' $ mở rộng $ u $.*

Chỉ cần áp dụng Định lý 2 cho các bao đóng đại số $ \Omega $ và $ (\Omega', u) $ của $ K $.

#### Nhận xét {#alg-v-s4-n3-rem-2 .statement}

— 2) Theo ký hiệu của Hệ quả trước đó, nói chung tồn tại các $ K $-tự đẳng cấu của $ \Omega $ phân biệt với đồng nhất. Do đó nói chung không có tính duy nhất đối với đẳng cấu $ v $ từ $ \Omega $ lên $ \Omega' $ mở rộng các đẳng cấu $ u $ từ $ K $ lên $ K' $. Vì những lý do tương tự, nói chung có nhiều hơn một đẳng cấu từ một mở rộng tách $ E $ lên một mở rộng tách $ E' $ đối với cùng một họ $ (f_i)_{i \in I} $ các đa thức. Nhắc lại rằng trái lại, đối với bao đóng hoàn hảo thì ta có tính duy nhất (V, p. 5).

3) Cho K là một trường và $ \Omega $ là một bao đóng đại số của $ K $. Khi đó có thể cho phép dựng sau đây của một mở rộng tách cho một họ $ (f_i)_{i \in I} $ các đa thức không hằng trong $ K[X] $: gọi $ R_i $ là tập hợp các nghiệm của $ f_i $ trong $ \Omega $ và gọi $ R = \bigcup_{i \in I} R_i $. Khi đó $ K(R) $ là mở rộng con duy nhất của $ \Omega $ mà là một mở rộng tách cho $ (f_i)_{i \in I} $ (V, p. 22, Prop. 5).

4) Cho K là một trường hữu hạn và $ \Omega $ là một bao đóng đại số của $ K $. Khi đó $ \Omega $ là vô hạn ($ V, $ p. 20, Prop. 3); vì mọi mở rộng bậc hữu hạn của K đều là một trường hữu hạn, nên $ \Omega $ là một mở rộng đại số có bậc *vô hạn* của $ K $.

### Bài tập {#alg-v-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
