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
content_sha256: 33f41886a1cb8662ca4e98d130814744e4f1327ee38d920f5fdd857601ef80f6
translated_from: content/en/alg/V/04_s4_algebraically_closed_extensions.md
source_content_sha256: 57102dadb9478828bbaf3bf1d6ad1b4a27c3a089d5abfaeca2f02ab9a7c16523
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
(AC) Mọi đa thức không hằng của K[X] đều tách trong K[X] thành một tích các đa thức bậc 1 (phân biệt hoặc không).
(AC') Mọi đa thức không hằng của K[X] đều có ít nhất một nghiệm trong K.
(AC'') Mọi đa thức bất khả quy trong K[X] đều có bậc 1.

(AC) Mọi mở rộng đại số của K đều có bậc 1 (nói cách khác, K đóng đại số tương đối trong mọi trường mở rộng của K).

Trước hết ta chứng minh tính tương đương của các tính chất (AC), (AC') và (AC''). Rõ ràng (AC) kéo theo (AC). Vì mọi đa thức không hằng của K[X] đều chia hết cho một đa thức bất khả quy (IV, p. 13, Prop. 13) và mọi đa thức bậc 1 trong K[X] rõ ràng đều nhận một nghiệm trong K, ta thấy rằng (AC) kéo theo (AC'). Điều kiện (AC') kéo theo bằng quy nạp theo n, rằng mọi đa thức bậc n trong K[X] là một tích của n đa thức bậc 1 (IV, p. 14, Prop. 1), do đó (AC') kéo theo (AC).

Còn lại là thấy rằng (AC) và (AC) là tương đương. Nếu (AC'') đúng, mọi phần tử của một trường mở rộng L của K mà đại số trên K đều có bậc 1 (V, p. 16, Th. 1), nên thuộc K, điều đó chứng minh (AC). Ngược lại, cho f là một đa thức bất khả quy bậc $n \geq 1$ trong K[X]; đại số thương K[X]/(f) có bậc n trên K và là một trường, do đó là một mở rộng đại số bậc n của K (V, p. 18, Prop. 2). Bây giờ rõ ràng rằng (AC) kéo theo (AC'').

#### Định nghĩa 1 {#alg-v-s4-def-1 .statement}

Một trường K được gọi là đóng đại số nếu nó có các tính chất (tương đương) (AC), (AC'), (AC), (AC).

\* Ví dụ 1. — Trường C các số phức là đóng đại số (Gen. Top., VIII, p. 100). \*

Một trường K đóng đại số tương đối trong một trường mở rộng E của K không nhất thiết là đóng đại số (thật vậy mọi trường đều đóng đại số tương đối trong chính nó, và tồn tại những trường không đóng đại số, chẳng hạn Q hoặc $\mathbf{F}_p$ \* hoặc R *). Tuy nhiên:

#### Mệnh đề 2 {#alg-v-s4-prop-2 .statement}

Cho $\Omega$ là một trường đóng đại số và K là một trường con của $\Omega$. Khi đó bao đóng đại số tương đối $\bar{K}$ của K trong $\Omega$ là một trường đóng đại số.

Cho f là một đa thức không hằng trong $\bar{K}[X] \subset \Omega[X]$. Vì $\Omega$ là đóng đại số, đa thức f có ít nhất một nghiệm trong $\Omega$, và vì nghiệm này là đại số trên $\bar{K}$, nó thuộc $\bar{K}$ (V, p. 19, Prop. 4). Do đó $\bar{K}$ thỏa mãn (AC').

\* Ví dụ 2. — Theo Prop. 2 tập hợp tất cả các số phức đại số trên Q (thường được gọi vắn tắt là các số đại số) là một trường đóng đại số. \*

#### Mệnh đề 3 {#alg-v-s4-prop-3 .statement}

Mọi trường đóng đại số đều vô hạn.

Cho K là một trường hữu hạn và đặt $f(X) = 1 + \prod_{a \in K} (X - a)$. Đa thức $f \in K[X]$ là không hằng và $f(a) = 1$ với mọi $a \in K$. Vậy trường K không thỏa mãn (AC') và do đó không đóng đại số.

#### Định lý 1 (Steinitz) {#alg-v-s4-thm-1 .statement}

Cho K là một trường, E là một mở rộng đại số của K và $\Omega$ là một mở rộng đóng đại số của K; khi đó tồn tại một K-đồng cấu từ E vào R.

Theo V, p. 13, Scholium, tồn tại một trường mở rộng $\Omega'$ của $\Omega$ và một K-đồng cấu u từ E vào $\Omega'$. Cho $x \in E$; vì x là đại số trên K, u(x) là đại số trên u(K) và *a fortiori* trên $\Omega$ (V, p. 17, Cor. 2); vì $\Omega$ là đóng đại số, do đó ta có $u(x) \in O$. Suy ra rằng $u$ ánh xạ $E$ vào $O$.

### 2. Các mở rộng tách

#### Định nghĩa 2 {#alg-v-s4-def-2 .statement}

*Cho K là một trường và $(f_i)_{i \in I}$ là một họ các đa thức không hằng trong $K[X]$. Bởi một mở rộng tách của $(f_i)_i$, ta hiểu một mở rộng E của $K$ có các tính chất sau :*

*a) Với mỗi $i \in I$, đa thức $f_i$ tách trong $E[X]$ thành một tích các đa thức bậc 1.*

*b) Với mỗi $i \in I$ cho $R_i$ là tập hợp các nghiệm của $f_i$ trong $E$, khi đó $E = K \left( \bigcup_{i \in I} R_i \right)$.*

Đôi khi dùng thuật ngữ « trường phân rã » thay cho « mở rộng tách ».

*Nhận xét. — 1) Với mỗi $i \in I$ cho $c_i$ là một phần tử khác không của $K$ và cho $f'_i = c_i f_i$. Khi đó rõ ràng mọi mở rộng tách của họ $(f_i)_i$, cũng là một mở rộng tách của họ $(f'_i)_{i \in I}$ và ngược lại. Đặc biệt, khi nghiên cứu các mở rộng tách ta có thể chỉ cần xét trường hợp các đa thức đơn thức đầu.*

*2) Giả sử rằng I là hữu hạn và đặt $f = \prod_{i \in I} f_i$. Dùng tính duy nhất của phân tích một đa thức thành các nhân tử bất khả quy trong $E[X]$ (IV, p. 13, Prop. 13), ta dễ dàng chứng minh rằng một mở rộng tách của đa thức $f$ là một mở rộng tách của họ $(f_i)_i$, và ngược lại. Nói cách khác, trường hợp một họ hữu hạn có thể quy về trường hợp một đa thức duy nhất.*

*3) Cho $f \in K[X]$ là một đa thức bậc $\geq 1$ và cho $E$ là một mở rộng tách của $f$. Nếu $x_1, \ldots, x_n$ là các nghiệm của $f$ trong $E$, thì do đó ta có $E = K(x_1, \ldots, x_n)$ và $[E : K]$ là hữu hạn ($V$, p. 18, Th. 2); nhưng có thể xảy ra rằng $E$ phân biệt với các trường con $K(x_1), \ldots, K(x_n)$ được sinh bởi một nghiệm duy nhất; điều này có thể xảy ra ngay cả khi $f$ là bất khả quy$^1$. Tuy nhiên, ta lưu ý rằng khi $f$ là bất khả quy, các trường $K(x_i)$ đều có cùng bậc $n$ trên $K$, và mỗi khi $E$ bằng một trong các trường đó, ta có $[E : K] = n$ và do đó $E = K(x_1) = \cdots = K(x_n)$.*

#### Mệnh đề 4 {#alg-v-s4-prop-4 .statement}

*Cho K là một trường và $(f_i)_{i \in I}$ là một họ các đa thức không hằng trong $K[X]$; khi đó tồn tại một mở rộng tách đối với họ $(f_i)_{i \in I}$.*

Ta có thể lấy các đa thức $f_i$ là đơn nhất (Nhận xét 1). Cho $i \in I$ và cho bậc của $f_i$ là $d_i$. Theo IV, p. 73, Prop. 5, tồn tại một đại số giao hoán $A$, trên $K$, không thu về 0, và các phần tử $\xi_{i,1}, \ldots, \xi_{i,d_i}$ của $A_i$ sao cho:

*a) đại số $A_i$ được sinh bởi $(\xi_{i,1}, \ldots, \xi_{i,d_i})$;*

(1) Chẳng hạn lấy $K = \mathbf{Q}$ và $f = X^3 - 2$.

b) ta có $f_i(X) = \prod_{k=1}^{d_i} (X - \xi_{i,k})$ trong $A_i[X]$.

Gọi $A$ là tích tenxơ của họ các đại số $(A,)_{i}$, và gọi $\varphi_i$ là đồng cấu chính tắc của $A_i$ vào $A$ (III, p. 470). Khi đó đại số $A$ là giao hoán và không thu về 0; bởi định lý của Krull (I, p. 104), do đó tồn tại một iđêan cực đại $a$ trong $A$ và $E = A/a$ là một mở rộng của trường $K$.

Ký hiệu $\psi$ là đồng cấu chính tắc của $A$ vào $E$ và đặt $x_{i,k} = \psi(\varphi_i(\xi_{i,k}))$ với $i \in I$ và $l \leq k \leq d_i$. Vì đại số $A$ được sinh bởi $\bigcup \varphi_i(A_i)$, mở rộng $E$ được sinh bởi họ $(x_{i,k})$. Hơn nữa, ta có $i \in I$

$$
f_i(X) = \prod_{k=1}^{d_i} (X - x_{i,k}) \text{ trong } E[X]. $$

Do đó $E$ là một mở rộng tách của họ $(f_i)_{i \in I}$.

#### Mệnh đề 5 {#alg-v-s4-prop-5 .statement}

— *Cho K là một trường, $(f_i)_{i \in I}$ là một họ các đa thức không hằng trong $K[X]$, E là một mở rộng của K, và F, F' là các mở rộng con của E mà mỗi mở rộng đều là một mở rộng tách của $(f_i)_{i \in I}$. Khi đó $F = F'$.

Gọi $R_i$ là tập hợp các nghiệm của $f_i$ trong E và $R = \bigcup_{i \in I} R_i$. Vì $f_i$ là một tích các đa thức bậc nhất nằm trong $F[X]$, ta có $R_i \subset F$. Theo Định nghĩa 2, ta có $F = K(R)$; theo cùng cách đó ta thấy rằng $F = K(R)$.

#### Hệ quả {#alg-v-s4-n2-cor-1 .statement}

— *Cho K là một trường, $(f_i)_{i \in I}$, là một họ các đa thức không hằng trong $K[X]$ và F, F' là các mở rộng tách của $(f_i)_{i \in I}$. Khi đó tồn tại một K-đẳng cấu của F lên F.

Điều này suy ra từ Mệnh đề 5 và V, p. 13, Hệ quả của Mệnh đề 4.

### 3. Bao đóng đại số của một trường

#### Định nghĩa 3 {#alg-v-s4-def-3 .statement}

— *Cho K là một trường. Ta hiểu một bao đóng đại số của K là bất kỳ mở rộng nào của K vừa đại số vừa đóng đại số.

#### Ví dụ 1 {#alg-v-s4-n3-exa-1 .statement}

Trường C các số phức là một bao đóng đại số của trường R các số thực (Gen. Top., VIII, p. 100) \*
2) Cho K là một trường và $\Omega$ là một mở rộng đóng đại số của K. Nếu $\overline{K}$ là bao đóng đại số tương đối của K trong $\Omega$, thì theo V, p. 20, Mệnh đề 2, K là một bao đóng đại số của K. \* Đặc biệt, trường của mọi số đại số (V, p. 20, Ex. 2) là một bao đóng đại số của trường Q các số hữu tỉ. \*

#### Mệnh đề 6 {#alg-v-s4-prop-6 .statement}

— *Cho $\Omega$ là một mở rộng của một trường K. Để $\Omega$ là một bao đóng đại số của K, điều kiện cần và đủ là nó phải đại số và mọi đa thức không hằng trong $K[X]$ đều phải tách trong $\Omega[X]$ thành một tích các nhân tử bậc 1.

Điều kiện là cần theo (AC). Ngược lại, giả sử rằng $\Omega$ đại số trên $K$ và mọi đa thức không hằng trên $K[X]$ đều là một tích trong $\Omega[X]$ của các nhân tử bậc 1. Gọi $\Omega'$ là một mở rộng đại số của $\Omega$ và gọi $x \in \Omega'$. Vì $x$ đại số trên $\Omega$ và $\Omega$ đại số trên $K$, nên $x$ đại số trên $K$ (V, p. 19, Mệnh đề 3). Gọi $f$ là đa thức tối tiểu của $x$ trên $K$. Theo giả thiết đa thức $f \in K[X]$ tách trong $\Omega[X]$ thành một tích các nhân tử bậc 1, do đó $x \in \Omega$. Vậy ta có $\Omega' = \Omega$ và $\Omega$ đóng đại số vì nó thỏa mãn (AC).

#### Nhận xét 1 {#alg-v-s4-n3-rem-1 .statement}

Nếu $\Omega$ đại số trên $K$ và nếu mọi đa thức không hằng của $K[X]$ đều có một nghiệm trong $\Omega$ thì $\Omega$ là một bao đóng đại số của $K$ (V, p. 156, Ex. 20).

#### Mệnh đề 7 {#alg-v-s4-prop-7 .statement}

— *Cho $\Omega$ là một mở rộng đại số của một trường $K$.
a) Nếu $\Omega$ đóng đại số, thì mọi mở rộng đại số của $K$ đều đẳng cấu với một mở rộng con của $\mathbf{R}$.
b) Ngược lại, giả sử rằng mọi mở rộng đại số bậc hữu hạn của $K$ đều đẳng cấu với một mở rộng con của $\Omega$; khi đó $\Omega$ đóng đại số.*

Mệnh đề *a)* suy ra từ Định lý 1 (V, p. 20). Bây giờ giả sử các giả thiết của *b)* và xét một đa thức không hằng $f \in K[X]$. Gọi E là một trường phân rã của $f$ (V, p. 21, Mệnh đề 4); vì E là đại số bậc hữu hạn trên $K$ (V, p. 18, Định lý 2), ta có thể giả sử rằng E là một mở rộng con của $\Omega$. Khi đó đa thức $f$ là một tích của các đa thức bậc 1 trong $\Omega[X]$ và Mệnh đề 6 cho thấy rằng $\Omega$ là đóng đại số.

Bây giờ ta có thể chứng minh sự tồn tại và tính duy nhất (cho đến đẳng cấu) của bao đóng đại số của một trường.

#### Định lý 2 (Steinitz) {#alg-v-s4-thm-2 .statement}

— *Cho $K$ là một trường; khi đó tồn tại một bao đóng đại số của $K$. Nếu $\Omega$ và $\Omega'$ là hai bao đóng đại số của $K$, thì tồn tại một $K$-đẳng cấu từ $\Omega$ lên $\Omega'$.*

Theo Mệnh đề 6, một bao đóng đại số của $K$ không là gì khác hơn một mở rộng tách đối với tập hợp tất cả các đa thức không hằng trong $K[X]$. Do đó Định lý 2 suy ra từ V, p. 21, Mệnh đề 4 và V, p. 22, Hệ quả.

#### Hệ quả {#alg-v-s4-n3-cor-1 .statement}

— *Cho $K$ và $K'$ là hai trường, $\Omega$ là một bao đóng đại số của $K$ và $\Omega'$ là một bao đóng đại số của $K'$. Với mọi đẳng cấu $u$ từ $K$ lên $K'$, tồn tại một đẳng cấu $v$ từ $\Omega$ lên $\Omega'$ mở rộng $u$.*

Chỉ cần áp dụng Định lý 2 cho các bao đóng đại số $\Omega$ và $(\Omega', u)$ của $K$.

#### Nhận xét 2 {#alg-v-s4-n3-rem-2 .statement}

Theo ký hiệu của Hệ quả đứng trước, nói chung tồn tại các $K$-tự đẳng cấu của $\Omega$ phân biệt với đồng nhất. Vì thế nói chung không có tính duy nhất đối với đẳng cấu $v$ từ $\Omega$ lên $\Omega'$ mở rộng các đẳng cấu $u$ từ $K$ lên $K'$. Vì những lý do tương tự, nói chung có nhiều hơn một đẳng cấu từ một mở rộng tách $E$ lên một mở rộng tách $E'$ đối với cùng một họ $(f_i)_{i \in I}$ các đa thức. Ta nhắc lại rằng ngược lại, đối với bao đóng hoàn hảo thì ta có tính duy nhất (V, p. 5).

#### Nhận xét 3 {#alg-v-s4-n3-rem-3 .statement}

Cho K là một trường và $\Omega$ là một bao đóng đại số của $K$. Khi đó có thể cho phép dựng sau đây của một mở rộng tách đối với một họ $(f_i)_{i \in I}$ các đa thức không hằng trong $K[X]$: gọi $R_i$ là tập hợp các nghiệm của $f_i$ trong $\Omega$ và đặt $R = \bigcup_{i \in I} R_i$. Khi đó $K(R)$ là mở rộng con duy nhất của $\Omega$ mà là một mở rộng tách đối với $(f_i)_{i \in I}$ (V, p. 22, Mệnh đề 5).

#### Nhận xét 4 {#alg-v-s4-n3-rem-4 .statement}

Cho K là một trường hữu hạn và $\Omega$ là một bao đóng đại số của K. Khi đó $\Omega$ là vô hạn ($V,$ p. 20, Prop. 3); vì mọi mở rộng bậc hữu hạn của K đều là một trường hữu hạn, nên $\Omega$ là một mở rộng đại số bậc *vô hạn* của $K$.

### Bài tập {#alg-v-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
