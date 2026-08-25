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
statements: 19
exercises: 2
content_sha256: 211a74de9d5cbc6f16445b735f526acb2aaf2f640c3995833c7acbf290e3a934
translated_from: content/en/alg/V/04_s4_algebraically_closed_extensions.md
source_content_sha256: 262fb2a6545dfb8cf6bd0155bed883d88156439e3210ddd756de34fd99622eab
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-e35f2d1f
glossary_version: 34
glossary_terms_sha256: bfd7d47a310724b7cbb9da44ea827216a62a7b066ad66fabd350b2c3c88863f1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. MỞ RỘNG ĐÓNG ĐẠI SỐ

### 1. Các trường đóng đại số

#### Mệnh đề 1 {#alg-v-s4-prop-1 .statement}

— Cho K là một trường; thì các tính chất sau là tương đương:
(AC) Mọi đa thức không hằng của K[X] tách trong K[X] thành một tích các đa thức bậc 1 (phân biệt hay không).
(AC') Mọi đa thức không hằng của K[X] có ít nhất một nghiệm trong K.
(AC'') Mọi đa thức bất khả quy trong K[X] đều có bậc 1.

(AC) Mọi mở rộng đại số của K đều có bậc 1 (nói cách khác, K là đóng đại số tương đối trong mọi trường mở rộng của K).

Trước hết ta hãy chứng minh tính tương đương của các tính chất (AC), (AC') và (AC''). Rõ ràng (AC) suy ra (AC). Vì mọi đa thức không hằng của K[X] đều chia hết cho một đa thức bất khả quy (IV, p. 13, Prop. 13) và mọi đa thức bậc 1 trong K[X] rõ ràng có một nghiệm trong K, ta thấy rằng (AC) suy ra (AC'). Điều kiện (AC') suy ra, bằng quy nạp theo n, rằng mọi đa thức bậc n trong K[X] là một tích của n đa thức bậc 1 (IV, p. 14, Prop. 1), do đó (AC') suy ra (AC).

Còn lại phải thấy rằng (AC) và (AC) là tương đương. Nếu (AC'') đúng, thì mọi phần tử của một trường mở rộng L của K mà đại số trên K đều có bậc 1 (V, p. 16, Th. 1), do đó thuộc K, điều này thiết lập (AC). Chiều ngược lại, xét f là một đa thức bất khả quy bậc $ n \geq 1 $ trong K[X]; đại số thương K[X]/(f) có bậc n trên K và là một trường, do đó là một mở rộng đại số bậc n của K (V, p. 18, Prop. 2). Bây giờ rõ ràng (AC) suy ra (AC'').

#### Định nghĩa 1 {#alg-v-s4-def-1 .statement}

Một trường K được gọi là đóng đại số nếu nó có các tính chất (tương đương) (AC), (AC'), (AC), (AC).

\* Ví dụ 1. — Trường C của các số phức là đóng đại số (Gen. Top., VIII, p. 100). \*

Một trường K đóng đại số tương đối trong một trường mở rộng E của K không nhất thiết là đóng đại số (thực ra mọi trường đều đóng đại số tương đối trong chính nó, và tồn tại các trường không đóng đại số, chẳng hạn Q hoặc $ \mathbf{F}_p $ \* hoặc R *). Tuy nhiên:

#### Mệnh đề 2 {#alg-v-s4-prop-2 .statement}

Cho $ \Omega $ là một trường đóng đại số và K là một trường con của $ \Omega $. Khi đó bao đóng đại số tương đối $ \bar{K} $ của K trong $ \Omega $ là một trường đóng đại số.

Cho f là một đa thức không hằng trong $ \bar{K}[X] \subset \Omega[X] $. Vì $ \Omega $ đóng đại số, đa thức f có ít nhất một nghiệm trong $ \Omega $, và vì nghiệm này đại số trên $ \bar{K} $, nên nó thuộc $ \bar{K} $ (V, p. 19, Mệnh đề 4). Do đó $ \bar{K} $ thỏa mãn (AC').

\* Ví dụ 2. — Theo Mệnh đề 2, tập hợp tất cả các số phức đại số trên Q (thường gọi ngắn gọn là các số đại số) là một trường đóng đại số. \*

#### Mệnh đề 3 {#alg-v-s4-prop-3 .statement}

Mọi trường đóng đại số đều vô hạn.

Cho K là một trường hữu hạn và đặt $ f(X) = 1 + \prod_{a \in K} (X - a) $. Đa thức $ f \in K[X] $ là không hằng và $ f(a) = 1 $ đối với mọi $ a \in K $. Vậy trường K không thỏa mãn (AC') và do đó không đóng đại số.

#### Định lý 1 (Steinitz) {#alg-v-s4-thm-1 .statement}

Cho K là một trường, E là một mở rộng đại số của K và $ \Omega $ là một mở rộng đóng đại số của K; khi đó tồn tại một K-đồng cấu của E vào R.

Theo V, p. 13, Chú giải, tồn tại một trường mở rộng $ \Omega' $ của $ \Omega $ và một K-đồng cấu u của E vào $ \Omega' $. Cho $ x \in E $; vì x đại số trên K, nên u(x) đại số trên u(K) và *a fortiori* trên $ \Omega $ (V, p. 17, Hệ quả 2); vì $ \Omega $ đóng đại số, nên ta có $ u(x) \in O $. Suy ra $ u $ ánh xạ $ E $ vào $ O $.

### 2. Mở rộng tách

#### Định nghĩa 2 {#alg-v-s4-def-2 .statement}

*Cho K là một trường và $ (f_i)_{i \in I} $ là một họ các đa thức không hằng trong $ K[X] $. Ta hiểu mở rộng tách của $ (f_i)_i $ là bất kỳ mở rộng $ E $ nào của K có các tính chất sau :*

*a) Với mỗi $ i \in I $, đa thức $ f_i $ tách trong $ E[X] $ thành một tích các đa thức bậc 1.*

*b) Với mỗi $ i \in I $, gọi $ R_i $ là tập các nghiệm của $ f_i $ trong $ E $, thì $ E = K \left( \bigcup_{i \in I} R_i \right) $.*

Đôi khi thuật ngữ « trường phân rã » được dùng thay cho « mở rộng tách ».

*Nhận xét. — 1) Với mỗi $ i \in I $, gọi $ c_i $ là một phần tử khác không của $ K $ và $ f'_i = c_i f_i $. Khi đó rõ ràng mọi mở rộng tách của họ $ (f_i)_i $, cũng là một mở rộng tách của họ $ (f'_i)_{i \in I} $ và ngược lại. Đặc biệt, khi nghiên cứu các mở rộng tách, ta có thể chỉ xét trường hợp các đa thức đơn.*

*2) Giả sử I hữu hạn và đặt $ f = \prod_{i \in I} f_i $. Dùng tính duy nhất của phân tích một đa thức thành các nhân tử bất khả quy trong $ E[X] $ (IV, p. 13, Mệnh đề 13), ta dễ dàng chứng minh rằng một mở rộng tách của đa thức $ f $ cũng là một mở rộng tách của họ $ (f_i)_i $, và ngược lại. Nói cách khác, trường hợp một họ hữu hạn có thể quy về trường hợp một đa thức duy nhất.*

*3) Cho $ f \in K[X] $ là một đa thức có bậc $ \geq 1 $ và cho $ E $ là một mở rộng tách của $ f $. Nếu $ x_1, \ldots, x_n $ là các nghiệm của $f$ trong $ E $, thì ta có $ E = K(x_1, \ldots, x_n) $ và $ [E : K] $ là hữu hạn ($ V $, p. 18, Th. 2); nhưng có thể xảy ra rằng $ E $ khác với các trường con $ K(x_1), \ldots, K(x_n) $ được sinh bởi một nghiệm duy nhất; điều này có thể xảy ra ngay cả khi $ f $ là bất khả quy$^1$. Tuy nhiên, ta nhận thấy rằng khi $ f $ là bất khả quy, các trường $ K(x_i) $ đều có cùng bậc $ n $ trên $ K $, và mỗi khi $ E $ bằng một trong số chúng, ta có $ [E : K] = n $ và do đó $ E = K(x_1) = \cdots = K(x_n) $.*

#### Mệnh đề 4 {#alg-v-s4-prop-4 .statement}

*Cho K là một trường và $ (f_i)_{i \in I} $ là một họ các đa thức không hằng trong $ K[X] $; khi đó tồn tại một mở rộng tách cho họ $ (f_i)_{i \in I} $. \*

Ta có thể giả sử các đa thức $ f_i $ là đơn thức (Nhận xét 1). Cho $ i \in I $ và cho bậc của $ f_i $ là $ d_i $. Theo IV, p. 73, Mệnh đề 5, tồn tại một đại số giao hoán $ A $, trên $ K $, không thu về 0, và các phần tử $ \xi_{i,1}, \ldots, \xi_{i,d_i} $ của $ A_i $ sao cho :

*a) đại số $ A_i $ được sinh bởi $ (\xi_{i,1}, \ldots, \xi_{i,d_i}) $;*

\footnotetext{1 Chẳng hạn lấy $ K = \mathbf{Q} $ và $ f = X^3 - 2 $.}

b) ta có $ f_i(X) = \prod_{k=1}^{d_i} (X - \xi_{i,k}) $ trong $ A_i[X] $.

Cho $ A $ là tích tenxơ của họ các đại số $ (A,)_{i} $, và cho $ \varphi_i $ là đồng cấu chính tắc từ $ A_i $ vào $ A $ (III, p. 470). Khi đó đại số $ A $ là giao hoán và không thu về 0; theo định lý Krull (I, p. 104), do đó tồn tại một iđêan cực đại $ a $ trong $ A $ và $ E = A/a $ là một mở rộng của trường $ K $.

Ký hiệu $ \psi $ là đồng cấu chính tắc từ $ A $ vào $ E $ và đặt $ x_{i,k} = \psi(\varphi_i(\xi_{i,k})) $ với $ i \in I $ và $ l \leq k \leq d_i $. Vì đại số $ A $ được sinh bởi $ \bigcup \varphi_i(A_i) $, mở rộng $ E $ được sinh bởi họ $ (x_{i,k}) $. Hơn nữa, ta có $ i \in I $

$$
f_i(X) = \prod_{k=1}^{d_i} (X - x_{i,k}) \text{ in } E[X].
$$

Do đó $ E $ là một mở rộng tách của họ $ (f_i)_{i \in I} $.

#### Mệnh đề 5 {#alg-v-s4-prop-5 .statement}

— *Cho K là một trường, $ (f_i)_{i \in I} $ là một họ các đa thức không hằng trong $ K[X] $, E là một mở rộng của K, và F, F' là các mở rộng con của E, mỗi mở rộng đều là một mở rộng tách của $ (f_i)_{i \in I} $. Khi đó $ F = F' $.

Cho $ R_i $ là tập hợp các nghiệm của $ f_i $ trong E và $ R = \bigcup_{i \in I} R_i $. Vì $ f_i $ là tích của các đa thức bậc nhất thuộc $ F[X] $, nên ta có $ R_i \subset F $. Theo Định nghĩa 2, ta có $ F = K(R) $; tương tự, ta thấy rằng $ F = K(R) $.

#### Hệ quả {#alg-v-s4-n2-cor-1 .statement}

— *Cho K là một trường, $ (f_i)_{i \in I} $, một họ các đa thức không hằng trong $ K[X] $ và F, F' là các mở rộng tách của $ (f_i)_{i \in I} $. Khi đó tồn tại một đẳng cấu K của F lên F.

Điều này suy ra từ Mệnh đề 5 và V, p. 13, Hệ quả của Mệnh đề 4.

### 3. Bao đóng đại số của một trường

#### Định nghĩa 3 {#alg-v-s4-def-3 .statement}

— *Cho K là một trường. Ta gọi bao đóng đại số của K là bất kỳ mở rộng nào của K vừa đại số vừa đóng đại số.

#### Ví dụ 1 {#alg-v-s4-n3-exa-1 .statement}

Trường C các số phức là một bao đóng đại số của trường R các số thực (Gen. Top., VIII, p. 100) \*
2) Cho K là một trường và $ \Omega $ là một mở rộng đóng đại số của K. Nếu $ \overline{K} $ là bao đóng đại số tương đối của K trong $ \Omega $, thì theo V, p. 20, Mệnh đề 2, K là một bao đóng đại số của K. \* Đặc biệt, trường gồm tất cả các số đại số (V, p. 20, Bài tập 2) là một bao đóng đại số của trường Q các số hữu tỉ. \*

#### Mệnh đề 6 {#alg-v-s4-prop-6 .statement}

— *Cho $ \Omega $ là một mở rộng của trường K. Để $ \Omega $ là một bao đóng đại số của K thì điều kiện cần và đủ là nó phải đại số và mọi đa thức không hằng trong $ K[X] $ phải tách trong $ \Omega[X] $ thành tích của các nhân tử bậc 1.

Điều kiện này là cần theo (AC). Ngược lại, giả sử rằng $ \Omega $ là đại số trên $ K $ và mọi đa thức không hằng trên $ K[X] $ là tích trong $ \Omega[X] $ của các nhân tử bậc 1. Cho $ \Omega' $ là một mở rộng đại số của $ \Omega $ và cho $ x \in \Omega' $. Vì $ x $ là đại số trên $ \Omega $ và $ \Omega $ là đại số trên $ K $, nên $ x $ là đại số trên $ K $ (V, p. 19, Mệnh đề 3). Gọi $ f $ là đa thức tối tiểu của $ x $ trên $ K $. Theo giả thiết, đa thức $ f \in K[X] $ tách trong $ \Omega[X] $ thành tích của các nhân tử bậc 1, do đó $ x \in \Omega $. Vậy ta có $ \Omega' = \Omega $ và $ \Omega $ là đóng đại số vì nó thỏa mãn (AC).

#### Nhận xét 1 {#alg-v-s4-n3-rem-1 .statement}

Nếu $ \Omega $ là đại số trên $ K $ và nếu mọi đa thức không hằng của $ K[X] $ đều có một nghiệm trong $ \Omega $ thì $ \Omega $ là một bao đóng đại số của $ K $ (V, p. 156, Bài tập 20).

#### Mệnh đề 7 {#alg-v-s4-prop-7 .statement}

— *Cho $ \Omega $ là một mở rộng đại số của một trường $ K $.
a) Nếu $ \Omega $ đóng đại số, thì mọi mở rộng đại số của $ K $ đều đẳng cấu với một mở rộng con của $ \mathbf{R} $.
b) Ngược lại, giả sử rằng mọi mở rộng đại số bậc hữu hạn của $ K $ đều đẳng cấu với một mở rộng con của $ \Omega $; khi đó $ \Omega $ đóng đại số.*

Mệnh đề *a)* suy ra từ Đl. 1 (V, p. 20). Bây giờ giả sử các giả thiết của *b)* và xét một đa thức không hằng $ f \in K[X] $. Gọi E là một trường phân rã của $ f $ (V, p. 21, Mđ. 4); vì E là đại số có bậc hữu hạn trên $ K $ (V, p. 18, Đl. 2), ta có thể giả sử rằng E là một mở rộng con của $ \Omega $. Khi đó đa thức $ f $ là tích của các đa thức bậc 1 trong $ \Omega[X] $ và Mđ. 6 chỉ ra rằng $ \Omega $ là đóng đại số.

Bây giờ ta có thể chứng minh sự tồn tại và tính duy nhất (sai khác một đẳng cấu) của bao đóng đại số của một trường.

#### Định lý 2 (Steinitz) {#alg-v-s4-thm-2 .statement}

— *Cho $ K $ là một trường; khi đó tồn tại một bao đóng đại số của $ K $. Nếu $ \Omega $ và $ \Omega' $ là hai bao đóng đại số của $ K $, tồn tại một $ K $-đẳng cấu từ $ \Omega $ lên $ \Omega' $.*

Theo Mđ. 6, một bao đóng đại số của $ K $ không là gì khác ngoài một mở rộng tách đối với tập hợp tất cả các đa thức không hằng trong $ K[X] $. Do đó Đl. 2 suy ra từ V, p. 21, Mđ. 4 và V, p. 22, Hệ quả.

#### Hệ quả {#alg-v-s4-n3-cor-1 .statement}

— *Cho $ K $ và $ K' $ là hai trường, $ \Omega $ là một bao đóng đại số của $ K $ và $ \Omega' $ là một bao đóng đại số của $ K' $. Với mọi đẳng cấu $ u $ của $ K $ lên $ K' $, tồn tại một đẳng cấu $ v $ của $ \Omega $ lên $ \Omega' $ mở rộng $ u $.*

Chỉ cần áp dụng Đl. 2 cho các bao đóng đại số $ \Omega $ và $ (\Omega', u) $ của $ K $.

#### Nhận xét 2 {#alg-v-s4-n3-rem-2 .statement}

Theo ký hiệu của Hệ quả trước đó, nói chung tồn tại các $ K $-tự đẳng cấu của $ \Omega $ phân biệt với đẳng cấu đồng nhất. Do đó nói chung không có tính duy nhất đối với đẳng cấu $ v $ của $ \Omega $ lên $ \Omega' $ mở rộng các đẳng cấu $ u $ của $ K $ lên $ K' $. Vì những lý do tương tự, nói chung có nhiều hơn một đẳng cấu của một mở rộng tách $ E $ lên một mở rộng tách $ E' $ đối với cùng một họ $ (f_i)_{i \in I} $ các đa thức. Ta nhắc lại rằng ngược lại, đối với bao đóng hoàn hảo ta có tính duy nhất (V, p. 5).

#### Nhận xét 3 {#alg-v-s4-n3-rem-3 .statement}

Cho K là một trường và $ \Omega $ là một bao đóng đại số của $ K $. Khi đó phép dựng sau đây có thể được cho đối với một mở rộng tách của một họ $ (f_i)_{i \in I} $ các đa thức không hằng trong $ K[X] $: gọi $ R_i $ là tập hợp các nghiệm của $ f_i $ trong $ \Omega $ và gọi $ R = \bigcup_{i \in I} R_i $. Khi đó $ K(R) $ là mở rộng con duy nhất của $ \Omega $ là một mở rộng tách đối với $ (f_i)_{i \in I} $ (V, p. 22, Mđ. 5).

#### Nhận xét 4 {#alg-v-s4-n3-rem-4 .statement}

Cho K là một trường hữu hạn và $ \Omega $ là một bao đóng đại số của $ K $. Khi đó $ \Omega $ là vô hạn ($ V, $ p. 20, Mệnh đề 3); vì mọi mở rộng bậc hữu hạn của K đều là một trường hữu hạn, nên $ \Omega $ là một mở rộng đại số có *bậc vô hạn* của $ K $.

### Bài tập {#alg-v-s4-exercises}

Xem các [bài tập cho § 4](exercises/s4/).
