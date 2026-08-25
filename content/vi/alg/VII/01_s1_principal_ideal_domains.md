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
content_sha256: d364c69f5c34457fb64557d886d54b80b00289ea706d8ac77d126aaae5bdd554
translated_from: content/en/alg/VII/01_s1_principal_ideal_domains.md
source_content_sha256: 8391d460561adeb449ac1dffa38cdbf8ce479bf1cd6f9f8c60527fcfd05e8a6f
translation_model: gpt-5-6-mini
translation_run: translate-vi-a52a80a1
glossary_version: 34
glossary_terms_sha256: f0394aede1ac5204d08ae33f14962c83a4670c4314b118cb2fec8191e1bfbe50
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. MIỀN IĐÊAN CHÍNH

### 1. Định nghĩa miền iđêan chính

Nhắc lại (I, p. 104) rằng một iđêan của một vành giao hoán $A$ được gọi là *chính* nếu nó có dạng $(a) = Aa$ với một $a \in A$ nào đó.

#### Định nghĩa 1 {#alg-vii-s1-def-1 .statement}

*Một miền iđêan chính là một miền nguyên (I, p. 116) trong đó mọi iđêan đều là chính.*

#### Ví dụ {#alg-vii-s1-n1-exa-1 .statement}

Vành $\mathbf{Z}$ của các số nguyên hữu tỉ là một miền iđêan chính (I, p. 111). Nếu $K$ là một trường giao hoán, thì vành đa thức $K[X]$ theo một bất định trên $K$ là một miền iđêan chính (IV, p. 11, Mđề 11); điều tương tự đúng với vành các chuỗi lũy thừa hình thức $K[[X]]$, vì mọi iđêan của vành này có dạng $(X^n)$ (IV, p. 38, Mđề 12). \* Vành các số nguyên trong một trường p-adic là một miền iđêan chính. \*

Nếu $\mathbf{Q}(i)$ kí hiệu trường thu được từ trường $\mathbf{Q}$ các số hữu tỉ bằng cách ghép thêm một nghiệm $i$ của đa thức bất khả quy $X^2 + 1$, thì các phần tử $a + bi$ của $\mathbf{Q}(i)$, trong đó $a$ và $b$ là các số nguyên hữu tỉ, tạo thành một vành con $\mathbf{A}$ của $\mathbf{Q}(i)$, được gọi là « các số nguyên Gaussian », là một miền iđêan chính (VII, p. 50, Bài tập 7). Trái lại, trong trường $\mathbf{Q}(\rho)$, trong đó $\rho$ là một nghiệm của $X^2 + 5$, vành con $B$ gồm các phần tử $a + bp$ (a và b là các số nguyên hữu tỉ) không phải là một miền iđêan chính (VII, p. 51, Bài tập 12).

Vành đa thức $K[X, Y]$ theo hai bất định trên một trường $K$ không phải là một miền iđêan chính. Thật vậy, các hằng số khác không là những phần tử duy nhất chia hết cả $X$ lẫn $Y$, và không phần tử nào trong số chúng sinh ra iđêan sinh bởi $X$ và $Y$.

### 2. Tính chia hết trong các miền iđêan chính

Cho $A$ là một miền iđêan chính và cho $K$ là trường các phân thức của nó (I, p. 116); ta sẽ thấy rằng nhóm có thứ tự $\mathcal{P}^*$ của các iđêan phân thức chính (*VI*, p. 6) của $K$ là có thứ tự dàn; chính xác hơn:

#### Mệnh đề 1 {#alg-vii-s1-prop-1 .statement}

*Cho $K$ là trường các phân thức của một miền iđêan chính $A$, và cho $(x_i)_{i \in I}$ là một họ các phần tử của $K$ có một mẫu số chung $b \in K^*$ (nói cách khác $bx_i \in A$ với mọi $i$). Khi đó:*

a) Họ $(x,)$ có một ước chung lớn nhất trong $K$.
b) Mọi ước chung lớn nhất của $(x,)$ đều có thể được biểu diễn dưới dạng $d = \sum a_i x_i$, trong đó các $a_i$ là các phần tử của $A$, tất cả trừ một số hữu hạn trong chúng là không.

Thật vậy, iđêan $\sum Abx$, của $A$ là chính, và do đó có dạng $Ad'$. Đặt $d' = bd \ (d \in K)$. Từ quan hệ $d' = \sum a_i b x_i$, ta suy ra $d = \sum a_i x_i$, trong đó $a_i \in A$. Do đó mọi ước chung của các $x_i$ đều chia hết $d$. Mặt khác, vì $bd$ là một ước chung của các $bx$, theo phép dựng, nên suy ra $d$ là một ước chung của các $x_i$.

#### Nhận xét {#alg-vii-s1-n2-rem-1 .statement}

Mệnh đề 1 áp dụng không có hạn chế nào cho một họ tùy ý $(x,)$ các phần tử của $A$ (lấy $b = 1$), và cũng cho mọi họ hữu hạn $(x,)$ các phần tử của $K$ (nếu $x_i = c_i b_i$ với $c_i \in A$ và $b_i \in A$, thì lấy $b$ là tích của các $b_i$).

#### Hệ quả {#alg-vii-s1-n2-cor-1 .statement}

— Cho $(x,)$ là một họ tùy ý các phần tử của một miền iđêan chính $A$ được chứa như một vành con trong một miền nguyên $B$, và cho $d$ là một ước chung lớn nhất của họ $(x,)$ trong $A$. Khi đó họ $(x,)$ có các ước chung lớn nhất trong $B$, và $d$ là một trong số chúng.

Thật vậy $d$ là một ước chung của các $x_i$ trong $B$. Mặt khác quan hệ $d = \sum a_i x_i$ cho thấy rằng mọi ước chung của các $x_i$ trong $B$ đều chia hết $d$.

Một áp dụng quan trọng của hệ quả này là khi $A = K[X]$ và $B = E[X]$, trong đó $K$ là một trường và $E$ là một mở rộng của $K$ (IV, p. 12, Hệ quả 1).

Mệnh đề đầu tiên của Mệnh đề 1 cho thấy rằng nhóm có thứ tự $\mathcal{P}^*$ là có thứ tự dàn ($VI,$ p. 10). Đặc biệt mọi họ hữu hạn các phần tử của $K$ đều có bội chung nhỏ nhất. Do đó ta có thể áp dụng các kết quả được ký hiệu (DIV) trong $VI$, pp. 10 đến 17 cho các miền iđêan chính.

Kết quả sau đây là một hệ quả của mệnh đề thứ hai của Mệnh đề I :

#### Định lý 1 (« đồng nhất thức Bezout ») {#alg-vii-s1-thm-1 .statement}

— Các phần tử $x_i \ (i \in I)$ của một miền iđêan chính $A$ là nguyên tố cùng nhau theo tập khi và chỉ khi tồn tại các phần tử $a_i \ (i \in I)$ của $A$, tất cả trừ một số hữu hạn trong chúng là không, sao cho $\sum a_i x_i = 1$.

Tính cần thiết của điều kiện chỉ là Mệnh đề 1. Ngược lại, nếu $\sum a_i x_i = 1$ thì mọi ước chung của các $x_i$ đều chia hết 1, và do đó 1 là một ước chung lớn nhất của các $x_i$.

#### Mệnh đề 2 {#alg-vii-s1-prop-2 .statement}

— Cho $a, b, d, m$ và $p$ là các phần tử của trường phân thức $K$ của một miền iđêan chính $A$.
a) « $d$ là một ước chung lớn nhất của $a$ và $b$ » tương đương với « $(d) = (a) + (b)$ ».
b) « $m$ là một bội chung nhỏ nhất của $a$ và $b$ » tương đương với « $m = (a) \cap (b)$ ».
c) « $p$ là một phần tử bất khả quy của $A$ » tương đương với « $(p)$ là một iđêan cực đại khác không của $A$ » và với « $(p)$ là một iđêan nguyên tố khác không của $A$ ».

Ta đã chứng minh $a)$ (Mệnh đề *1*). Vì các bội chung của $a$ và $b$ là các phần tử của $(a) \cap (b)$, và vì, theo giả thiết, iđêan $(a) \cap (b)$ là chính, giả sử $(a) \cap (b) = (m)$, nên suy ra rằng $m$ là một bội chung nhỏ nhất của $a$ và $b$, điều này chứng minh $b)$. Cuối cùng, nói rằng $p \neq 0$ là một phần tử bất khả quy của $A$ có nghĩa theo định nghĩa (VI, p. *17*) rằng $(p)$ là một phần tử cực đại của họ các iđêan chính $\neq A$ của $A$, có thứ tự bởi quan hệ bao hàm; vì $A$ không có iđêan nào khác ngoài các iđêan chính, điều này có nghĩa rằng $(p)$ là một iđêan cực đại của $A$, do đó có $c)$, theo nhận xét trong VI, p. 17.

Trong một miền iđêan chính $A$, tổng (tương ứng, giao) của một số hữu hạn các iđêan cũng được gọi là gcd (tương ứng, lcm) của các iđêan này.

#### Mệnh đề 3 {#alg-vii-s1-prop-3 .statement}

*Cho $a, b, c$ là các phần tử của trường phân thức của một miền iđêan chính $A$, và cho $d$ là một ước chung lớn nhất của $a$ và $c$; khi đó đồng dư thức $ax \equiv b \pmod{c}$ có một nghiệm $x_0 \in A$ khi và chỉ khi $d$ chia hết $b$; trong trường hợp này các phần tử $x$ của $A$ thỏa mãn $ax \equiv b \pmod{c}$ chính xác là các phần tử thỏa mãn $x \equiv x_0 \pmod{cd}$*.

Nếu $ax \equiv b \pmod{c}$, với $x \in A$, thì tồn tại $y \in A$ sao cho $b = ax + cy$, do đó $d$ chia hết $b$. Ngược lại, nếu $d$ chia hết $b$ thì $b = ax_0 + cy_0$ với $x_0, y_0 \in A$ (Mệnh đề *1*), do đó $ax_0 \equiv b \pmod{c}$; hơn nữa, quan hệ $ax \equiv b \pmod{c}$ khi đó tương đương với $a(x - x_0) \equiv 0 \pmod{c}$; đặt $a = da'$ và $c = dc'$, cái sau trở thành $a'(x - x_0) \equiv 0 \pmod{c'}$. Nhưng điều này tương đương (đối với $x \in A$) với $x - x_0 \equiv 0 \pmod{c'}$, vì $a'$ và $c'$ nguyên tố cùng nhau (VI, p. 14, Mệnh đề *10* (DIV) và VI, p. 15, Hệ quả 2 của Mệnh đề 11 (DIV)).

#### Mệnh đề 4 {#alg-vii-s1-prop-4 .statement}

*Cho $(a_i)$, $i \leq n$ là một họ hữu hạn các phần tử từng đôi một nguyên tố cùng nhau của miền iđêan chính $A$. Khi đó đồng cấu chính tắc (I, p. 110) từ $A / \left( \prod_{r=1}^n a_r \right)$ vào tích $\prod_{r=1}^n A/(a_r)$ là một đẳng cấu của các $A$-đại số.*

Điều này suy ra từ I, p. 110, Mệnh đề 9 và từ Mệnh đề 2 *a)*.

Kết luận của Mệnh đề 4 không còn đúng nếu không giả thiết rằng các $a_i$ từng đôi một nguyên tố cùng nhau (xem VII, p. 24, Mệnh đề 9).

### 3. Phân tích thành các nhân tử bất khả quy trong các miền iđêan chính

Bây giờ ta sẽ áp dụng các kết quả của VI, p. *18*, liên quan đến phân tích thành các phần tử bất khả quy, cho các miền iđêan chính. Theo Mệnh đề 2, một phần tử $p \neq 0$ của $A$ là bất khả quy khi và chỉ khi vành $A/(p)$ là một trường (I, p. *115*, Hệ quả 1), nghĩa là khi và chỉ khi đồng dư thức $ax \equiv b \pmod{p}$ có nghiệm trong $A$ với mỗi $b \in A$ và với mỗi $a \in A$ không phải là bội của $p$.

#### Định nghĩa 2 {#alg-vii-s1-def-2 .statement}

*Cho $A$ là một miền nguyên. Một hệ đại diện của các phần tử bất khả quy của $A$ là một họ $(p_\alpha)$ gồm các phần tử bất khả quy của $A$ sao cho mỗi phần tử bất khả quy của $A$ là phần tử liên kết với đúng một $p_\alpha$.*

#### Định lý 2 {#alg-vii-s1-thm-2 .statement}

— Cho $\mathbf{A}$ là một miền iđêan chính và cho $(p,)$ là một hệ đại diện của các phần tử bất khả quy của $\mathbf{A}$. Khi đó mọi phần tử khác không $x$ của trường phân thức của $A$ có thể được biểu diễn duy nhất dưới dạng

$$
x = u \prod_{\alpha} p_{\alpha}^{n_{\alpha}},
$$

trong đó $u$ là một phần tử khả nghịch của $\mathbf{A}$, và trong đó các $n_{\alpha}$ là các số nguyên, tất cả trừ một số hữu hạn trong chúng đều bằng không. Để $x$ thuộc $\mathbf{A}$ thì điều kiện cần và đủ là tất cả các $n_{\alpha}$ đều dương.

Ta sẽ sử dụng định lý về phân tích thành một tổng các phần tử bất khả quy (VI, p. 18, Định lý 2), mà mệnh đề trên chỉ là một cách phát biểu lại. Vì $\mathcal{P}^*$ là một nhóm có thứ tự dàn nên đối với chúng ta chỉ cần chứng minh rằng mọi tập hợp khác rỗng các iđêan chính của $\mathbf{A}$ đều chứa một phần tử cực đại, để kiểm tra rằng các giả thiết của định lý này thực sự được thỏa mãn; giờ đây điều này suy ra từ Bổ đề sau:

#### Bổ đề 1 {#alg-vii-s1-lem-1 .statement}

Cho $A$ là một vành sao cho mọi iđêan trái của $A$ đều sinh hữu hạn. Khi đó mọi tập hợp khác rỗng $\Phi$ các iđêan trái của $\mathbf{A}$, có thứ tự bởi quan hệ bao hàm, đều có một phần tử cực đại.

Theo Bổ đề Zorn (Lý thuyết tập hợp, III, p. 154, Đl. 2) chỉ cần chứng minh rằng $\Phi$ là quy nạp. Bây giờ nếu $(a,)$ là một họ có thứ tự toàn phần các phần tử của $\Phi$ thì hợp $a$ của các iđêan $a_i$ là một iđêan trái của $\mathbf{A}$, và do đó thừa nhận một hệ hữu hạn các phần tử sinh $(a_i)_{1 \leq i \leq n}$. Vì mỗi $a_i$ thuộc một iđêan $a_{,,}$, và vì họ $(a,)$ có thứ tự toàn phần, nên các $a_i$ đều thuộc iđêan lớn nhất trong các iđêan $a_{\lambda_i}$, chẳng hạn $a_1$. Khi đó $a = a_1$ thuộc $\Phi$, do đó đây thực sự là một tập quy nạp.

Sau này chúng ta sẽ nghiên cứu những vành $B$, được gọi là các vành Noether, sao cho mọi tập hợp khác rỗng các iđêan của $B$ đều chứa một phần tử cực đại.

#### Nhận xét {#alg-vii-s1-n3-rem-1 .statement}

Họ $(u, (n,))$ được gọi là phân tích của $x$ thành các thừa số bất khả quy; do lạm dụng ngôn ngữ, ta cũng nói rằng công thức (1) là phân tích của $x$ thành các thừa số bất khả quy. Nếu $x = u \prod_{\alpha} p_{\alpha}^{n_{\alpha}}$ và $y = v \prod_{\alpha} p_{\alpha}^{m_{\alpha}}$ là các phân tích của $x$ và $y$ thành các thừa số bất khả quy, thì một điều kiện cần và đủ để $x$ chia hết cho $y$ là $n_{\alpha} \leq m_{\alpha}$, với mọi $\alpha$; từ đó ta suy ra các công thức

$$
\gcd(x, y) = \prod_{\alpha} p_{\alpha}^{\inf(n_{\alpha}, m_{\alpha})}
$$
$$
\operatorname{lcm}(x, y) = \prod_{\alpha} p_{\alpha}^{\sup(n_{\alpha}, m_{\alpha})}
$$

Tính chất được biểu thị bởi Đl. 2 là đúng cho một lớp các vành tổng quát hơn các miền iđêan chính; sau này chúng ta sẽ nghiên cứu chúng dưới tên các miền phân tích duy nhất; và chúng ta sẽ thấy rằng các vành đa thức và các vành chuỗi lũy thừa hình thức với tùy ý nhiều bất định là các miền phân tích duy nhất (Đại số giao hoán, VII, § 3).

### 4. Tính chia hết của các số nguyên hữu tỉ

Như đã được chỉ ra trong tiết 1, vành $\mathbf{Z}$ các số nguyên hữu tỉ là một miền iđêan chính; trường các phân thức của nó là $\mathbf{Q}$. Nhóm nhân $U$ các phần tử khả nghịch của $\mathbf{Z}$ có hai phần tử 1 và $-1$. Nhóm $Q_+^*$ các số hữu tỉ $> 0$ chứa chính xác một phần tử từ mỗi lớp các phần tử liên kết của $\mathbf{Q}$; do đó nó đẳng cấu với nhóm nhân $\mathcal{P}^* = Q^*/U$ các iđêan phân thức chính của $\mathbf{Q}$, mà với nhóm này nó thường được đồng nhất. Đặc biệt, bất cứ khi nào sử dụng ước chung lớn nhất hoặc bội chung nhỏ nhất trong trường $\mathbf{Q}$ (đối với vành $\mathbf{Z}$), ta hiểu rằng đây là các phần tử $\geqslant 0$; quy ước này cho phép ta nói về ước chung lớn nhất và bội chung nhỏ nhất của một họ các số hữu tỉ.

Các số nguyên bất khả quy $> 0$ trong $\mathbf{Z}$ chính là những số mà ta đã gọi là các số nguyên tố (I, p. 50) (đôi khi được gọi là các số nguyên tố hữu tỉ); mọi phần tử bất khả quy của $\mathbf{Z}$ do đó có dạng $p$ hoặc $-p$, trong đó $p$ là một số nguyên tố, và tập hợp $P$ các số nguyên tố là một hệ các đại diện của các phần tử bất khả quy của $\mathbf{Z}$.

#### Mệnh đề 5 {#alg-vii-s1-prop-5 .statement}

— Tập hợp các số nguyên tố là vô hạn.

Thật vậy, cho một họ hữu hạn tùy ý $(p_i)$ ($1 \leq i \leq n$) các số nguyên tố phân biệt, mọi ước nguyên tố $q$ của số $\left( \prod_{i=1}^n p_i \right) + 1$ (lớn hơn $1$) đều phân biệt với tất cả các $p_i$, vì nếu không thì nó sẽ chia hết cho 1.

### 5. Tính chia hết của các đa thức theo một bất định trên một trường

Vành đa thức $K[X]$ theo một bất định trên một trường giao hoán $K$ là một miền iđêan chính (IV, p. 11, Mệnh đề 11). Trường phân thức của nó là trường $K(X)$ các hàm hữu tỉ theo $X$ với các hệ số trong $K$. Vành $K[X]$ chứa vành con các đa thức có bậc 0, nghĩa là trường các hằng, được đồng nhất với $K$; các phần tử của $K^*$ là khả nghịch trong $K$, và do đó trong $K[X]$; đảo lại công thức $\deg(uv) = \deg(u) + \deg(v)$ chỉ ra rằng mọi đa thức khả nghịch đều có bậc 0; nhóm $U$ các phần tử khả nghịch của $K[X]$ do đó chính xác là $K^*$. Do đó hai đa thức liên kết chỉ khác nhau bởi một nhân tử hằng khác không; đặc biệt mọi lớp các đa thức liên kết chứa một đa thức đơn khởi duy nhất. Nhóm con của nhóm nhân $K(X)^*$ được sinh bởi các đa thức đơn khởi do đó chứa một phần tử duy nhất từ mỗi lớp các hàm hữu tỉ liên kết, và do đó đẳng cấu với nhóm

$$
\mathcal{P}^* = K(X)^*/U
$$

của các iđêan phân thức chính của $K(X)$. Đặc biệt, bất cứ khi nào ước chung lớn nhất hoặc bội chung nhỏ nhất trong trường $K(X)$ (đối với vành $K[X]$) được đề cập, thông thường ta hiểu rằng đó là các thương của các đa thức đơn khởi (hoặc 0); quy ước này cho phép ta nói về ước chung lớn nhất hoặc bội chung nhỏ nhất của một họ các hàm hữu tỉ.

Các phần tử bất khả quy của $K[X]$ chính xác là các đa thức bất khả quy theo nghĩa thông thường (IV, p. 13, Định nghĩa 2), và tập hợp các đa thức bất khả quy đơn khởi là một hệ các đại diện của các phần tử bất khả quy của $K[X]$.

Một đa thức bậc một luôn là bất khả quy. Nếu $K$ là một trường đóng đại số thì đảo lại đúng (V, p. 19, Mệnh đề 1); do đó trong trường hợp này mọi đa thức $p(X)$ bậc $n$ trong $K[X]$ có thể được viết duy nhất (sai khác bởi thứ tự của các nhân tử) dưới dạng

$$
p(X) = c(X - a_1)(X - a_2) \ldots (X - a_n)
$$

trong đó $c$ và các $a_i$ là các phần tử của $K$.

#### Mệnh đề 6 {#alg-vii-s1-prop-6 .statement}

Với mọi trường $K$, *tập hợp* các đa thức bất khả quy đơn khởi trong $K[X]$ là vô hạn.

Thật vậy, cho một họ hữu hạn khác rỗng tùy ý $(p_i)$ ($1 \leq i \leq n$) gồm các đa thức bất khả quy đơn khởi phân biệt, đa thức $\left( \prod_{i=1}^n p_i \right) + 1$ không khả nghịch, và mọi nhân tử bất khả quy đơn khởi $q$ của đa thức này nhất thiết phân biệt với mọi $p_i$, nếu không nó sẽ chia hết cho 1.

### Bài tập {#alg-vii-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
