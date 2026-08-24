---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 1
section_title: Principal ideal domains
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0360-0365, 0407-0413
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a principal ideal domain
      page: 0
      pdf_page: 360
    - "no": 2
      title: Divisibility in principal ideal domains
      page: 0
      pdf_page: 360
    - "no": 3
      title: Decomposition into irreducible factors in principal ideal domains
      page: 3
      pdf_page: 362
    - "no": 4
      title: Divisibility of rational integers
      page: 5
      pdf_page: 364
    - "no": 5
      title: Divisibility of polynomials in one indeterminate over a field
      page: 5
      pdf_page: 364
statements: 15
exercises: 15
content_sha256: 08d815cfc6afa0e0039382903df40d8ea1c3ebe63a638de1a92a19e384327812
translated_from: content/en/alg/VII/01_s1_principal_ideal_domains.md
source_content_sha256: 4d2e8685293c5e563dc0126488613d8ea1302d51c77a7dce89470fb01bc5d9c2
translation_model: gpt-5.4
translation_run: translate-vi-a52a80a1
glossary_version: 34
glossary_terms_sha256: f0394aede1ac5204d08ae33f14962c83a4670c4314b118cb2fec8191e1bfbe50
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. MIỀN IĐÊAN CHÍNH

### 1. Định nghĩa miền iđêan chính

Nhắc lại (I, p. 104) rằng một iđêan của một vành giao hoán $ A $ được gọi là *chính* nếu nó có dạng $ (a) = Aa $ với một $ a \in A $ nào đó.

#### Định nghĩa 1 {#alg-vii-s1-def-1 .statement}

*Miền iđêan chính là một miền nguyên (I, p. 116) trong đó mọi iđêan đều là chính.*

#### Ví dụ {#alg-vii-s1-n1-exa-1 .statement}

— Vành $ \mathbf{Z} $ các số nguyên hữu tỉ là một miền iđêan chính (I, p. 111). Nếu $ K $ là một trường giao hoán, thì vành đa thức $ K[X] $ theo một ẩn trên $ K $ là một miền iđêan chính (IV, p. 11, Prop. 11); điều tương tự cũng đúng với vành chuỗi lũy thừa hình thức $ K[[X]] $, vì mọi iđêan của vành này đều có dạng $ (X^n) $ (IV, p. 38, Prop. 12). \* Vành các số nguyên trong một trường p-adic là một miền iđêan chính. \*

Nếu $ \mathbf{Q}(i) $ ký hiệu trường thu được từ trường $ \mathbf{Q} $ các số hữu tỉ bằng cách kề thêm một nghiệm $ i $ của đa thức bất khả quy $ X^2 + 1 $, thì các phần tử $ a + bi $ của $ \mathbf{Q}(i) $, trong đó $ a $ và $ b $ là các số nguyên, tạo thành một vành con $ \mathbf{A} $ của $ \mathbf{Q}(i) $, được gọi là « các số nguyên Gauss », là một miền iđêan chính (VII, p. 50, Bài tập 7). Trái lại, trong trường $ \mathbf{Q}(\rho) $, trong đó $ \rho $ là một nghiệm của $ X^2 + 5 $, vành con $ B $ gồm các phần tử $ a + bp $ (a và b là các số nguyên) không phải là một miền iđêan chính (VII, p. 51, Bài tập 12).

Vành đa thức $ K[X, Y] $ theo hai bất định trên một trường $ K $ không phải là một miền iđêan chính. Thật vậy, các hằng số khác không là những phần tử duy nhất chia hết cả $ X $ và $ Y $, và không phần tử nào trong chúng sinh ra iđêan được sinh bởi $ X $ và $ Y $.

### 2. Tính chia hết trong các miền iđêan chính

Cho $ A $ là một miền iđêan chính và $ K $ là trường phân thức của nó (I, p. 116); ta sẽ thấy rằng nhóm có thứ tự $ \mathcal{P}^* $ các iđêan phân thức chính (*VI*, p. 6) của $ K $ là một dàn có thứ tự; chính xác hơn:

#### Mệnh đề 1 {#alg-vii-s1-prop-1 .statement}

*Cho $ K $ là trường phân thức của một miền iđêan chính $ A $, và cho $ (x_i)_{i \in I} $ là một họ các phần tử của $ K $ có một mẫu số chung $ b \in K^* $ (nói cách khác $ bx_i \in A $ với mọi $ i $). Khi đó:*

a) Họ $ (x,) $ có một ước chung lớn nhất trong $ K $.
b) Mọi ước chung lớn nhất của $ (x,) $ đều có thể được biểu diễn dưới dạng $ d = \sum a_i x_i $, trong đó các $ a_i $ là những phần tử của $ A $, và tất cả trừ hữu hạn phần tử trong số đó đều bằng không.

Thật vậy, iđêan $ \sum Abx $, của $ A $ là chính, nên có dạng $ Ad' $. Đặt $ d' = bd \ (d \in K) $. Từ quan hệ $ d' = \sum a_i b x_i $, suy ra $ d = \sum a_i x_i $, trong đó $ a_i \in A $. Do đó mọi ước chung của các $ x_i $ đều chia $ d $. Mặt khác, vì $ bd $ là một ước chung của các $ bx $, theo phép dựng, nên suy ra $ d $ là một ước chung của các $ x_i $.

#### Nhận xét {#alg-vii-s1-n2-rem-1 .statement}

— Mệnh đề 1 áp dụng không có hạn chế nào cho một họ tùy ý $ (x,) $ các phần tử của $ A $ (lấy $ b = 1 $), và cũng áp dụng cho mọi họ hữu hạn $ (x,) $ các phần tử của $ K $ (nếu $ x_i = c_i b_i $ với $ c_i \in A $ và $ b_i \in A $, thì lấy $ b $ là tích của các $ b_i $).

#### Hệ quả {#alg-vii-s1-n2-cor-1 .statement}

— Cho $ (x,) $ là một họ tùy ý các phần tử của một miền iđêan chính $ A $ được chứa như một vành con trong một miền nguyên $ B $, và cho $ d $ là một ước chung lớn nhất của họ $ (x,) $ trong $ A $. Khi đó họ $ (x,) $ có các ước chung lớn nhất trong $ B $, và $ d $ là một trong số đó.

Thật vậy, $ d $ là một ước chung của các $ x_i $ trong $ B $. Mặt khác, quan hệ $ d = \sum a_i x_i $ cho thấy rằng mọi ước chung của các $ x_i $ trong $ B $ đều là ước của $ d $.

Một ứng dụng quan trọng của hệ quả này là trường hợp $ A = K[X] $ và $ B = E[X] $, trong đó $ K $ là một trường và $ E $ là một mở rộng của $ K $ (IV, p. 12, Hệ quả 1).

Mệnh đề đầu tiên của Mệnh đề 1 cho thấy rằng nhóm có thứ tự $ \mathcal{P}^* $ là một dàn có thứ tự ($ VI, $ p. 10). Đặc biệt, mọi họ hữu hạn các phần tử của $ K $ đều có một bội chung nhỏ nhất. Do đó ta có thể áp dụng các kết quả ký hiệu là (DIV) trong $ VI $, pp. 10 to 17 cho các miền iđêan chính.

Kết quả sau đây là một hệ quả của mệnh đề thứ hai của Mệnh đề I :

#### Định lý 1 (« đồng nhất thức Bezout ») {#alg-vii-s1-thm-1 .statement}

— Các phần tử $ x_i \ (i \in I) $ của một miền iđêan chính $ A $ nguyên tố cùng nhau từng đôi một khi và chỉ khi tồn tại các phần tử $ a_i \ (i \in I) $ của $ A $, tất cả trừ hữu hạn phần tử đều bằng không, sao cho $ \sum a_i x_i = 1 $.

Tính cần thiết của điều kiện chỉ là Mệnh đề 1. Ngược lại, nếu $ \sum a_i x_i = 1 $ thì mọi ước chung của các $ x_i $ đều chia hết 1, và do đó 1 là một ước chung lớn nhất của các $ x_i $.

#### Mệnh đề 2 {#alg-vii-s1-prop-2 .statement}

— Cho $ a, b, d, m $ và $ p $ là các phần tử của trường phân thức $ K $ của một miền iđêan chính $ A $.
a) « $ d $ là một ước chung lớn nhất của $ a $ và $ b $ » tương đương với « $ (d) = (a) + (b) $ ».
b) « $ m $ là một bội chung nhỏ nhất của $ a $ và $ b $ » tương đương với « $ m = (a) \cap (b) $ ».
c) « $ p $ là một phần tử bất khả quy của $ A $ » tương đương với « $ (p) $ là một iđêan cực đại khác không của $ A $ » và với « $ (p) $ là một iđêan nguyên tố khác không của $ A $ ».

Chúng tôi đã chứng minh $a)$ (Mệnh đề *1*). Vì các bội chung của $a$ và $b$ là các phần tử của $(a) \cap (b)$, và vì, theo giả thiết, iđêan $(a) \cap (b)$ là chính, giả sử $(a) \cap (b) = (m)$, suy ra $m$ là một Icm của $a$ và $b$, điều này chứng minh $b)$. Cuối cùng, nói rằng $p \neq 0$ là một phần tử bất khả quy của $A$ theo định nghĩa (VI, p. *17*) có nghĩa là $(p)$ là một phần tử cực đại của họ các iđêan chính $\neq A$ của $A$, có thứ tự bởi bao hàm; vì $A$ không có iđêan nào khác ngoài các iđêan chính, điều đó có nghĩa là $(p)$ là một iđêan cực đại của $A$, do đó có $c)$, theo nhận xét ở VI, p. 17.

Trong một miền iđêan chính $A$, tổng (resp. giao) của một số hữu hạn iđêan cũng được gọi là gcd (resp. lcm) của các iđêan ấy.

#### Mệnh đề 3 {#alg-vii-s1-prop-3 .statement}

*Cho $a, b, c$ là các phần tử của trường phân thức của một miền iđêan chính $A$, và $d$ là một gcd của $a$ và $c$; khi đó đồng dư thức $ax \equiv b \pmod{c}$ có một nghiệm $x_0 \in A$ nếu và chỉ nếu $d$ chia hết $b$; trong trường hợp này các phần tử $x$ của $A$ thỏa mãn $ax \equiv b \pmod{c}$ chính xác là những phần tử thỏa mãn $x \equiv x_0 \pmod{cd}$*.

Nếu $ax \equiv b \pmod{c}$, với $x \in A$, thì tồn tại $y \in A$ sao cho $b = ax + cy$, nên $d$ chia hết $b$. Ngược lại, nếu $d$ chia hết $b$ thì $b = ax_0 + cy_0$ với $x_0, y_0 \in A$ (Mệnh đề *1*), nên $ax_0 \equiv b \pmod{c}$; hơn nữa, quan hệ $ax \equiv b \pmod{c}$ khi đó tương đương với $a(x - x_0) \equiv 0 \pmod{c}$; đặt $a = da'$ và $c = dc'$, thì điều sau trở thành $a'(x - x_0) \equiv 0 \pmod{c'}$. Nhưng điều này tương đương (với $x \in A$) với $x - x_0 \equiv 0 \pmod{c'}$, vì $a'$ và $c'$ nguyên tố cùng nhau (VI, p. 14, Mệnh đề *10* (DIV) và VI, p. 15, Hệ quả 2 của Mệnh đề 11 (DIV)).

#### Mệnh đề 4 {#alg-vii-s1-prop-4 .statement}

*Cho $(a_i)$, $i \leq n$ là một họ hữu hạn các phần tử nguyên tố cùng nhau từng đôi một của miền iđêan chính $A$. Khi đó đồng cấu chính tắc (I, p. 110) từ $A / \left( \prod_{r=1}^n a_r \right)$ vào tích $\prod_{r=1}^n A/(a_r)$ là một đẳng cấu các $A$-đại số.*

Điều này suy ra từ I, p. 110, Prop. 9 và từ Mệnh đề 2 *a)*.

Kết luận của Mệnh đề 4 không còn đúng nếu không giả thiết rằng các $a_i$ nguyên tố cùng nhau từng đôi một (xem VII, p. 24, Prop. 9).

### 3. Phân tích thành các thừa số bất khả quy trong các miền iđêan chính

Bây giờ ta sẽ áp dụng cho các miền iđêan chính các kết quả của VI, p. *18*, liên quan đến sự phân tích thành các phần tử bất khả quy. Theo Mệnh đề 2, một phần tử $p \neq 0$ của $A$ là bất khả quy khi và chỉ khi vành $A/(p)$ là một trường (I, p. *115*, Hệ quả 1), nghĩa là khi và chỉ khi đồng dư $ax \equiv b \pmod{p}$ có một nghiệm trong $A$ với mọi $b \in A$ và với mọi $a \in A$ không là bội của $p$.

#### Định nghĩa 2 {#alg-vii-s1-def-2 .statement}

*Cho $A$ là một miền nguyên. Một hệ các đại diện của các phần tử bất khả quy của $A$ là một họ $(p_\alpha)$ các phần tử bất khả quy của $A$ sao cho mọi phần tử bất khả quy của $A$ đều liên kết với chính xác một $p_\alpha$.*

#### Định lý 2 {#alg-vii-s1-thm-2 .statement}

— Cho $ \mathbf{A} $ là một miền iđêan chính và cho $ (p,) $ là một hệ các đại diện của các phần tử bất khả quy của $ \mathbf{A} $. Khi đó mọi phần tử khác không $ x $ của trường phân thức của $ A $ đều có thể được biểu diễn duy nhất dưới dạng

$$
x = u \prod_{\alpha} p_{\alpha}^{n_{\alpha}},
$$

trong đó $ u $ là một phần tử khả nghịch của $ \mathbf{A} $, và trong đó các $ n_{\alpha} $ là các số nguyên mà tất cả trừ hữu hạn số đều bằng không. Để $ x $ thuộc $ \mathbf{A} $ thì điều kiện cần và đủ là mọi $ n_{\alpha} $ đều dương.

Chúng ta sẽ dùng định lý về phân tích thành tổng các phần tử bất khả quy (VI, p. 18, Đl. 2), mà mệnh đề trên chỉ là một bản dịch. Vì $ \mathcal{P}^* $ là một nhóm có thứ tự dàn, với chúng ta sẽ đủ để chứng minh rằng mọi tập hợp khác rỗng các iđêan chính của $ \mathbf{A} $ đều chứa một phần tử cực đại, để kiểm tra rằng các giả thiết của định lý này quả thật được thỏa mãn; điều này suy ra từ Bổ đề sau đây:

#### Bổ đề 1 {#alg-vii-s1-lem-1 .statement}

— Cho $ A $ là một vành sao cho mọi iđêan trái của $ A $ đều sinh hữu hạn. Khi đó mọi tập hợp khác rỗng $ \Phi $ gồm các iđêan trái của $ \mathbf{A} $, có thứ tự bởi bao hàm, đều có một phần tử cực đại.

Theo Bổ đề Zorn (Lý thuyết tập hợp, III, p. 154, Th. 2), chỉ cần chứng minh rằng $ \Phi $ là quy nạp. Bây giờ nếu $ (a,) $ là một họ được sắp thứ tự toàn phần gồm các phần tử của $ \Phi $ thì hợp $ a $ của các iđêan $ a_i $ là một iđêan trái của $ \mathbf{A} $, và do đó thừa nhận một hệ hữu hạn các phần tử sinh $ (a_i)_{1 \leq i \leq n} $. Vì mỗi $ a_i $ thuộc một iđêan $ a_{,,} $, và vì họ $ (a,) $ được sắp thứ tự toàn phần, nên các $ a_i $ đều thuộc iđêan lớn nhất trong các iđêan $ a_{\lambda_i} $, giả sử là $ a_1 $. Khi đó $ a = a_1 $ thuộc $ \Phi $, do đó quả thật là một tập quy nạp.

Sau này chúng ta sẽ nghiên cứu những vành $ B $, gọi là các vành Noether, sao cho mọi tập hợp khác rỗng các iđêan của $ B $ đều chứa một phần tử cực đại.

#### Nhận xét {#alg-vii-s1-n3-rem-1 .statement}

— Họ $ (u, (n,)) $ được gọi là phân tích của $ x $ thành các nhân tử bất khả quy; do một sự lạm dụng ngôn ngữ, ta cũng nói rằng công thức (1) là phân tích của $ x $ thành các nhân tử bất khả quy. Nếu $ x = u \prod_{\alpha} p_{\alpha}^{n_{\alpha}} $ và $ y = v \prod_{\alpha} p_{\alpha}^{m_{\alpha}} $ là các phân tích của $ x $ và $ y $ thành các nhân tử bất khả quy, thì điều kiện cần và đủ để $ x $ chia hết $ y $ là $ n_{\alpha} \leq m_{\alpha} $, với mọi $ \alpha $; từ đó suy ra các công thức

$$
\gcd(x, y) = \prod_{\alpha} p_{\alpha}^{\inf(n_{\alpha}, m_{\alpha})}
$$
$$
\operatorname{lcm}(x, y) = \prod_{\alpha} p_{\alpha}^{\sup(n_{\alpha}, m_{\alpha})}
$$

Tính chất được phát biểu bởi Định lý 2 là đúng cho một lớp vành tổng quát hơn các miền iđêan chính; chúng ta sẽ nghiên cứu chúng sau này như các miền phân tích duy nhất; và chúng ta sẽ thấy rằng các vành đa thức và các vành chuỗi lũy thừa hình thức theo một số tùy ý các ẩn là các miền phân tích duy nhất (Comm. Alg., VII, § 3).

### 4. Tính chia hết của các số nguyên hữu tỉ

Như đã được chỉ ra trong tiết diện 1, vành $ \mathbf{Z} $ các số nguyên hữu tỉ là một miền iđêan chính; trường phân thức của nó là $ \mathbf{Q} $. Nhóm nhân $ U $ của các phần tử khả nghịch của $ \mathbf{Z} $ có hai phần tử 1 và $-1$. Nhóm $ Q_+^* $ các số hữu tỉ $ > 0 $ chứa chính xác một phần tử từ mỗi lớp các phần tử liên hợp của $ \mathbf{Q} $; do đó nó đẳng cấu với nhóm nhân $ \mathcal{P}^* = Q^*/U $ của các iđêan phân thức chính của $ \mathbf{Q} $, mà người ta thường đồng nhất với nó. Đặc biệt, mỗi khi ước chung lớn nhất hoặc bội chung nhỏ nhất được dùng trong trường $ \mathbf{Q} $ (đối với vành $ \mathbf{Z} $), thì hiểu rằng đó là các phần tử $ \geqslant 0 $; quy ước này cho phép ta nói đến ước chung lớn nhất và bội chung nhỏ nhất của một họ các số hữu tỉ.

Các số nguyên bất khả quy $ > 0 $ trong $ \mathbf{Z} $ chính xác là những số mà chúng tôi đã gọi là các số nguyên tố (I, p. 50) (đôi khi chúng được gọi là các số nguyên tố hữu tỉ); do đó, mọi phần tử bất khả quy của $ \mathbf{Z} $ đều có dạng $ p $ hoặc $-p$, trong đó $ p $ là một số nguyên tố, và tập hợp $ P $ các số nguyên tố là một hệ đại diện của các phần tử bất khả quy của $ \mathbf{Z} $.

#### Mệnh đề 5 {#alg-vii-s1-prop-5 .statement}

— Tập hợp các số nguyên tố là vô hạn.

Thật vậy, cho một họ hữu hạn tùy ý $ (p_i) $ ($ 1 \leq i \leq n $) các số nguyên tố phân biệt, thì mọi ước nguyên tố $ q $ của số $ \left( \prod_{i=1}^n p_i \right) + 1 $ (số này $ > 1 $) đều phân biệt với mọi $ p_i $, vì nếu không thì nó sẽ chia hết 1.

### 5. Tính chia hết của các đa thức theo một ẩn trên một trường

Vành đa thức $ K[X] $ theo một bất định trên một trường giao hoán $ K $ là một miền iđêan chính (IV, p. 11, Prop. 11). Trường phân thức của nó là trường $ K(X) $ của các hàm hữu tỉ theo $ X $ với các hệ số thuộc $ K $. Vành $ K[X] $ chứa vành con các đa thức bậc 0, tức là trường các hằng số, được đồng nhất với $ K $; các phần tử của $ K^* $ là khả nghịch trong $ K $, và do đó trong $ K[X] $; ngược lại công thức $ \deg(uv) = \deg(u) + \deg(v) $ cho thấy rằng mọi đa thức khả nghịch đều có bậc 0; do đó nhóm $ U $ của các phần tử khả nghịch của $ K[X] $ chính xác là $ K^* $. Như vậy hai đa thức liên kết chỉ khác nhau bởi một nhân tử hằng khác không; đặc biệt mỗi lớp các đa thức liên kết đều chứa một đa thức đơn khởi duy nhất. Nhóm con của nhóm nhân $ K(X)^* $ sinh bởi các đa thức đơn khởi vì thế chứa một phần tử duy nhất từ mỗi lớp các hàm hữu tỉ liên kết, và do đó đẳng cấu với nhóm

$$
\mathcal{P}^* = K(X)^*/U
$$

của các iđêan phân thức chính của $ K(X) $. Đặc biệt, mỗi khi nhắc đến gcd hoặc lcm trong trường $ K(X) $ (đối với vành $ K[X] $), thông thường sẽ hiểu rằng đó là các thương của các đa thức đơn nhất (hoặc 0); quy ước này cho phép ta nói về gcd hoặc lcm của một họ các hàm hữu tỉ.

Các phần tử bất khả quy của $ K[X] $ chính xác là các đa thức bất khả quy theo nghĩa thông thường (IV, p. 13, Def. 2), và tập hợp các đa thức bất khả quy đơn nhất là một hệ đại diện của các phần tử bất khả quy của $ K[X] $.

Một đa thức bậc nhất luôn luôn là bất khả quy. Nếu $ K $ là một trường đóng đại số thì mệnh đề đảo lại là đúng (V, p. 19, Prop. 1); do đó trong trường hợp này mọi đa thức $ p(X) $ bậc $ n $ trong $ K[X] $ đều có thể được viết duy nhất (không kể thứ tự của các thừa số) dưới dạng

$$
p(X) = c(X - a_1)(X - a_2) \ldots (X - a_n)
$$

trong đó $ c $ và các $ a_i $ là những phần tử của $ K $.

#### Mệnh đề 6 {#alg-vii-s1-prop-6 .statement}

Với mọi trường $ K $, *tập hợp* các đa thức bất khả quy đơn nhất trong $ K[X] $ là vô hạn.

Thật vậy, cho một họ hữu hạn khác rỗng tùy ý $ (p_i) $ ($ 1 \leq i \leq n $) gồm các đa thức bất khả quy đơn nhất phân biệt, đa thức $ \left( \prod_{i=1}^n p_i \right) + 1 $ không khả nghịch, và mọi nhân tử bất khả quy đơn nhất $ q $ của đa thức này tất yếu đều phân biệt với mọi $ p_i $, nếu không thì nó sẽ chia hết 1.

### Bài tập {#alg-vii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
