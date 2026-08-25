---
book: alg
book_title: Algebra
chapter: VI
chapter_title: ORDERED GROUPS AND FIELDS
section: 2
section_title: Ordered fields
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VI.37-A VI.47
pdf_pages: 0330-0341, 0348-0358
extraction: ocr
subsections:
    - "no": 1
      title: Ordered rings
      page: 19
      pdf_page: 330
    - "no": 2
      title: Ordered fields
      page: 20
      pdf_page: 331
    - "no": 3
      title: Extensions of ordered fields
      page: 21
      pdf_page: 332
    - "no": 4
      title: Algebraic extensions of ordered fields
      page: 23
      pdf_page: 334
    - "no": 5
      title: Maximal ordered fields
      page: 25
      pdf_page: 336
    - "no": 6
      title: Characterisation of maximal ordered fields. Euler-Lagrange Theorem
      page: 26
      pdf_page: 337
    - "no": 7
      title: Vector spaces over an ordered field
      page: 28
      pdf_page: 339
statements: 31
exercises: 41
content_sha256: d83ecd423c0da6302cf9c5f78a15bf49812c2a7f88ebcc5826a6322999012bd2
translated_from: content/en/alg/VI/02_s2_ordered_fields.md
source_content_sha256: a9ea185b5e464ae853d3c2d17a543197771aae8cf459215a2571972f9b8e5a6a
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-16dd10d9
glossary_version: 34
glossary_terms_sha256: 5729a03b73c13be7974b2fb8701d5076d6bce3f0b52e0c30f0152f8172c1d008
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC TRƯỜNG CÓ THỨ TỰ

### 1. Các vành có thứ tự

#### Định nghĩa 1 {#alg-vi-s2-def-1 .statement}

— Cho một vành giao hoán $ \mathbf{A} $, ta nói rằng một quan hệ thứ tự trên $ \mathbf{A} $ tương thích với cấu trúc vành của $ \mathbf{A} $ nếu nó tương thích với cấu trúc nhóm cộng của $ \mathbf{A} $, và nếu nó thỏa mãn tiên đề sau đây:
(OR) Các quan hệ $ x \geqslant 0 $ và $ y \geqslant 0 $ kéo theo $ xy \geqslant 0 $.
Vành $ \mathbf{A} $, cùng với một quan hệ thứ tự như vậy, được gọi là một vành có thứ tự.

#### Ví dụ 1 {#alg-vi-s2-n1-exa-1 .statement}

Các vành $ \mathbf{Q} $ và $ \mathbf{Z} $, với các quan hệ thứ tự thông thường, là các vành có thứ tự.
2) Tích của các vành có thứ tự, được trang bị quan hệ thứ tự tích, là một vành có thứ tự. Đặc biệt, vành $ \mathbf{A}^E $ các ánh xạ từ một tập hợp $ E $ vào một vành có thứ tự $ \mathbf{A} $ là một vành có thứ tự.
3) Một vành con của một vành có thứ tự, với quan hệ thứ tự cảm sinh, là một vành có thứ tự.

Trong một vành có thứ tự, các quan hệ $ x \geqslant y $ và $ z \geqslant 0 $ kéo theo $ xz \geqslant yz $. Thật vậy, các bất đẳng thức này lần lượt tương đương với $ x - y \geqslant 0 $, $ z \geqslant 0 $ và $ (x - y)z \geqslant 0 $.
Tương tự ta có thể chứng minh rằng các quan hệ $ x \leqslant 0 $ và $ y \geqslant 0 $ (resp. $ y \leqslant 0 $) kéo theo $ xy \leqslant 0 $ (resp. $ xy \geqslant 0 $). Các kết quả này thường được gọi dưới tên các quy tắc dấu (hai phần tử được nói là có cùng dấu nếu cả hai đều $ \geqslant 0 $ hoặc cả hai đều $ \leqslant 0 $). Chúng kéo theo rằng, nếu $ \mathbf{A} $ là một vành được sắp thứ tự toàn phần, thì mọi bình phương đều dương, và đặc biệt mọi phần tử lũy đẳng (chẳng hạn phần tử đơn vị) đều dương.

#### Ví dụ {#alg-vi-s2-n1-exa-2 .statement}

Chỉ có một cấu trúc vành được sắp thứ tự toàn phần trên $ \mathbf{Z} $: thật vậy $ 1 > 0 $, do đó $ n > 0 $ với mọi số tự nhiên $ n \neq 0 $, theo quy nạp. Trái lại tồn tại các cấu trúc vành có thứ tự trên $ \mathbf{Z} $ không được sắp thứ tự toàn phần (xem dưới đây).

Gọi $ P $ là tập hợp các phần tử dương của một vành có thứ tự $ \mathbf{A} $. Ta biết (VI, p. 3, Mệnh đề 3) rằng $ P $ xác định quan hệ thứ tự trên $ \mathbf{A} $. Nói rằng $ \mathbf{A} $ là một vành có thứ tự tương đương với nói rằng $ P $ thỏa mãn các tính chất sau:

$$
\begin{align*}
(\mathrm{AP}_I) &\quad P + P \subset P \\
(\mathrm{AP}_{II}) &\quad PP \subset P \\
(\mathrm{AP}_{III}) &\quad P \cap (-P) = \{0\}
\end{align*}
$$

Thật vậy, $ (\mathrm{AP}_I) $ và $ (\mathrm{AP}_{III}) $ phát biểu rằng nhóm cộng của $ \mathbf{A} $ là một nhóm có thứ tự (VI, p. 3, Mệnh đề 3), trong khi $ (\mathrm{AP}_{,,}) $ là một cách diễn đạt của (OR).

Nhắc lại rằng điều kiện sau là cần và đủ để quan hệ thứ tự trên $ \mathbf{A} $ là toàn phần:

$$
(\mathrm{AP}_{IV}) \quad P \cup (-P) = \mathbf{A}.
$$

#### Ví dụ {#alg-vi-s2-n1-exa-3 .statement}

Trong $ \mathbf{Z} $, nếu ta lấy $ P $ là tập hợp các số nguyên dương (theo nghĩa thông thường) chẵn, ta được một vành không được sắp thứ tự toàn phần.

Cũng nhắc lại rằng, trong một nhóm Abel được sắp thứ tự toàn phần, quan hệ $ n \cdot x = 0 $ (với một số tự nhiên $ n \neq 0 $) kéo theo $ x = 0 $ (VI, p. 4); điều này cho ta kết quả sau.

#### Mệnh đề 1 {#alg-vi-s2-prop-1 .statement}

— *Một vành được sắp thứ tự toàn phần là không xoắn với tư cách một $ \mathbf{Z} $-môđun* (II, p. 313).

### 2. Các trường có thứ tự

#### Định nghĩa 2 {#alg-vi-s2-def-2 .statement}

— Một *trường giao hoán, được trang bị một quan hệ thứ tự toàn phần, được gọi là một trường có thứ tự* nếu *quan hệ thứ tự và cấu trúc vành của nó tương thích với nhau*.

Chúng ta chỉ xét các quan hệ thứ tự *toàn phần* trên các trường vì các quan hệ khác rất « bệnh hoạn » (VI, p. 38, Bài tập 6).

*Ví dụ. — 1) Trường $ \mathbf{Q} $ các số hữu tỉ là một trường có thứ tự.
2) Một trường con của một trường có thứ tự, với quan hệ thứ tự cảm sinh, là một trường có thứ tự.
3) \* Trường các số thực là một trường có thứ tự. \*

Cho $ K $ là một trường có thứ tự. Với mọi $ x \in K $ ta đặt

$$
\begin{align*}
\operatorname{sgn}(x) &= 1 & \text{nếu } x > 0, \\
\operatorname{sgn}(x) &= -1 & \text{nếu } x < 0, \\
\operatorname{sgn}(x) &= 0 & \text{nếu } x = 0.
\end{align*}
$$

Khi đó ta có $ \operatorname{sgn}(xy) = \operatorname{sgn}(x) \operatorname{sgn}(y) $; ta gọi $ \operatorname{sgn}(x) $ là *dấu* của $ x $. Ánh xạ $ x \mapsto \operatorname{sgn}(x) $ từ $ K^* $ vào nhóm nhân $ \{-1, +1\} $ là một đồng cấu toàn ánh có hạt nhân, là tập hợp các phần tử dương ngặt của $ K $, là một nhóm con của $ K^* $ có chỉ số 2.

Ngược lại, nếu $ K $ là một trường giao hoán và $ s : K^* \to \{-1, +1\} $ là một đồng cấu toàn ánh có hạt nhân đóng dưới phép cộng, thì $ s $ là ánh xạ dấu đối với một cấu trúc trường có thứ tự duy nhất, trong đó tập hợp các phần tử dương ngặt là hạt nhân của $ s $.

Với mọi $ x $ và $ y $ trong $ K $ ta có $ x = \operatorname{sgn}(x)|x| $ và $ |xy| = |x||y| $.

Mặt khác mọi trường có thứ tự đều có đặc số không (Mệnh đề 1).

#### Mệnh đề 2 {#alg-vi-s2-prop-2 .statement}

— *Cho $ A $ là một miền nguyên được sắp thứ tự toàn phần, và cho $ K $ là trường các phân thức của nó. Khi đó tồn tại duy nhất một thứ tự trên $ K $ hạn chế thành thứ tự đã cho trên $ A $ và làm cho $ K $ là một trường có thứ tự.*

Mọi $ x \in K $ có thể được biểu diễn dưới dạng $ x = ab^{-1} $, với $ a $ và $ b $ thuộc $ A $ và $ b \neq 0 $. Nếu $ x $ là dương, thì $ a $ và $ b $ có cùng dấu, và ngược lại. Do đó ta thấy rằng, nếu tồn tại một thứ tự trên $ K $ thỏa mãn các điều kiện đã cho, thì nó là duy nhất, và tập hợp $ P $ các phần tử dương trùng với tập hợp các $ ab^{-1} $, trong đó $ a $ và $ b $ là các phần tử của $ A $ có cùng dấu, và $ b \neq 0 $. Còn lại là chứng minh rằng $ P $ thỏa mãn các điều kiện (AP$_I$), (AP$_{II}$), (AP$_{III}$) và (AP$_{IV}$). Điều này là hiển nhiên đối với (AP$_{II}$) và (AP$_{IV}$). Đối với (AP$_I$), xét $ ab^{-1} + cd^{-1} $, trong đó ta có thể giả sử rằng $a$, $b$, $c$ và $d$ là dương; tổng này là $(ad + bc)(bd)^{-1}$, và $ad + bc$ và $bd$ là dương.

Để chứng minh $(\mathrm{AP}_{III})$, xét một đẳng thức có dạng $ab^{-1} = -cd^{-1}$, sao cho $ad + bc = 0$. Nếu giả sử rằng $a$ và $b$ có cùng dấu và rằng $c$ và $d$ có cùng dấu, thì các quy tắc về dấu cho thấy rằng $ad$ và $bc$ có cùng dấu; do đó $ad = bc = 0$, nên $a = c = 0$; vì vậy $P$ thực sự thỏa mãn $(\mathrm{AP}_{III})$.

#### Ví dụ {#alg-vi-s2-n2-exa-1 .statement}

— Vì $Z$ chỉ thừa nhận một cấu trúc vành có thứ tự toàn phần duy nhất (*VI*, p. 19, *ví dụ*), trường $\mathbf{Q}$ chỉ thừa nhận một quan hệ thứ tự làm cho nó là một trường có thứ tự: đó là quan hệ thứ tự thông thường.

### 3. Các mở rộng của trường có thứ tự

#### Định nghĩa 3 {#alg-vi-s2-def-3 .statement}

*Cho $K$ là một trường có thứ tự. Một mở rộng có thứ tự của $K$ là một cặp $(E, u)$, trong đó $E$ là một trường có thứ tự và $u$ là một đồng cấu tăng từ $K$ vào $E$.*

Cho $K$ là một trường, cho $E$ là một trường có thứ tự và cho $u : K \to E$ là một đồng cấu. Quan hệ
$$
x \leq y \quad \text{nếu} \quad u(x) \leq u(y)
$$
là một quan hệ thứ tự toàn phần trên $K$ cho nó một cấu trúc trường có thứ tự, được gọi là *cảm sinh* bởi cấu trúc của $E$. Nếu $K$ và $E$ là các trường có thứ tự, thì một đồng cấu $u : K \to E$ là tăng khi và chỉ khi cấu trúc trường có thứ tự của $K$ được cảm sinh bởi cấu trúc của $E$. Ta thường đồng nhất $K$ với ảnh của nó trong $E$ qua $u$.

#### Ví dụ {#alg-vi-s2-n3-exa-1 .statement}

— 1) Mọi trường có thứ tự $K$ đều là một mở rộng có thứ tự của $\mathbf{Q}$. Thật vậy $K$ là một mở rộng của $\mathbf{Q}$, vì nó có đặc số không, và mặt khác $\mathbf{Q}$ chỉ có thể được sắp thứ tự theo một cách duy nhất, như ta vừa thấy.

2) Cho $K$ là một trường có thứ tự, và cho $K(X)$ là trường các hàm hữu tỉ theo một bất định trên $K$. Hãy định nghĩa một quan hệ thứ tự trên vành đa thức $K[X]$ bằng cách lấy các phần tử dương là $0$ và các đa thức có hệ số dẫn đầu dương. Bằng cách này ta thu được một vành được sắp thứ tự toàn phần có quan hệ thứ tự mở rộng quan hệ thứ tự của $K$. Bằng cách áp dụng Mệnh đề 2 ta cho $K(X)$ cấu trúc của một mở rộng có thứ tự của $K$. *Đối với $K = \mathbf{R}$ có thể chứng minh rằng quan hệ thứ tự được định nghĩa trên $K(X)$ theo cách này là quan hệ của sự tăng trưởng gần $+\infty$ (xem *VI*, p. 24, Mệnh đề 4).*

#### Định lý 1 {#alg-vi-s2-thm-1 .statement}

*Để một mở rộng $E$ của $K$ mang cấu trúc của một mở rộng có thứ tự của $K$, điều kiện sau là cần và đủ:*
*(OE)* *Quan hệ $p_1 x_1^2 + \ldots + p_n x_n^2 = 0$ kéo theo*
$$
p_1 x_1 = \ldots = p_n x_n = 0
$$
*đối với mọi dãy hữu hạn $(x_i, p_i)$ gồm các cặp phần tử $x$ của $E$ và các phần tử dương $p_i$ của $K$.*

Điều kiện (OE) rõ ràng tương đương với:
(OE') *Phần tử – 1 không là một tổng của các phần tử có dạng* $ px^2 $ ($ x \in E, p \in K, p \geq 0 $).

Điều kiện (OE) là cần thiết: nếu E là một mở rộng có thứ tự của K thì các phần tử $ p_i x_i^2 $ là dương trong E, do đó bằng không nếu tổng của chúng bằng không. Mặt khác $ p_i x_i^2 = 0 $ tương đương với $ p_i x_i = 0 $.

Ngược lại, giả sử điều kiện (OE) được thỏa mãn, khi đó ta sẽ định nghĩa một thứ tự trên E bằng cách xây dựng một tập con P của E thỏa mãn các điều kiện (AP,,), (APII), (AP,,,) và (APIV), và chứa tập hợp $ K_+ $ các phần tử dương của K. Một tập con P như vậy chắc chắn sẽ làm cho E trở thành một mở rộng có thứ tự của K, vì ta có $ K \cap P = K_+ $; thật vậy, nếu P chứa một phần tử $ -a < 0 $ của K, thì a sẽ thuộc $ P \cap (-P) $, trái với (APIII).

Để định nghĩa P, ta xét tập hợp $ \mathcal{M} $ các tập con của E thỏa mãn (API), (AP,,) và (AP,,,), và chứa hợp của $ K_+ $ với tập hợp C các bình phương của các phần tử của E. Tập hợp $ \mathcal{M} $ khác rỗng, vì nó chứa tập hợp $ P_0 $ gồm các phần tử có dạng $ \sum p_i x_i^2 $ (việc $ P_0 $ thỏa mãn (AP,,,) suy ra ngay lập tức từ (OE)).

Hơn nữa $ \mathcal{M} $ là quy nạp (*Set Theory*, III, p. 154, Def. 3). Do đó, theo Định lý 2 của *Set Theory*, III, p. 154, tồn tại một phần tử cực đại trong $ \mathcal{M} $, và điều còn lại đối với chúng ta là chứng minh rằng nó thỏa mãn (APIV); điều này suy ra từ bổ đề sau:

#### Bổ đề {#alg-vi-s2-n3-lem-1 .statement}

— *Cho* $ P \in \mathcal{M} $ *và* $ x \notin P $; *khi đó tồn tại* $ P' \in \mathcal{M} $ *sao cho* $ P \subset P' $ *và* $ -x \in P' $.

Đặt $ P' = P - xP $, và kiểm tra rằng $ P' $ có các tính chất cần thiết. Vì $ 0 \in C \subset P $, ta có $ P \subset P' $. Do đó $ C \subset P' $ và $ K_+ \subset P' $. Vì $ 1 \in C \subset P $ nên ta có $ -x \in P' $. Ta có
$$
P' + P' = P - xP + P - xP = P + P - x(P + P) \subset P - xP = P',
$$
do đó (API). Ta có
$$
P'P' = (P - xP)(P - xP) \subset \\
\quad \subset PP + x^2PP - x(PP + PP) \subset P + CP - xP \subset P - xP = P',
$$
do đó (AP,,,) Cuối cùng, hãy kiểm tra (APIII): giả sử có một đẳng thức dạng $ p - xq = -(r - xs) $ trong đó $ p, q, r, s $ thuộc P; ta suy ra từ đó quan hệ $ x(s + q) = p + r $; nếu $ s + q \neq 0 $ thì ta có
$$
x = (s + q)^{-2}(s + q)(p + r) \in CPP \subset P,
$$
trái với giả thiết; do đó $ s + q = 0 $, suy ra $ p + r = 0 $; vì P thỏa mãn (AP,,,) ta suy ra $ s = q = r = p = 0 $, điều này hoàn tất chứng minh.

#### Hệ quả 1 (*« Định lý Artin-Schreier »*) {#alg-vi-s2-thm-1-cor-1 .statement}

— *Điều kiện cần và đủ để tồn tại một thứ tự trên một trường giao hoán* E *làm cho nó trở thành một trường có thứ tự là quan hệ* $ x_1^2 + \ldots + x_n^2 = 0 $ *phải kéo theo* $ x_1 = \ldots = x_n = 0 $.

Tính cần thiết là hiển nhiên. Ngược lại, điều kiện đã nêu kéo theo rằng E có đặc số không, do đó là một mở rộng của Q; khi đó điều kiện $(OE)$ được thỏa mãn, và Định lý 1 cho thấy trên E tồn tại cấu trúc của một mở rộng có thứ tự của Q, tức là một cấu trúc trường có thứ tự.

Không tồn tại cấu trúc trường có thứ tự nào trên một trường E trong đó $-1$ là một bình phương, đặc biệt là trên một trường đóng đại số.

#### Hệ quả 2 {#alg-vi-s2-thm-1-cor-2 .statement}

*Cho E là một mở rộng của K mang cấu trúc của một mở rộng có thứ tự của K. Đối với một phần tử $x \in E$, để x dương dưới mọi cấu trúc như vậy trên E, điều kiện cần và đủ là x có dạng $\sum_i p_i x_i^2$, trong đó $x_i \in E$ và các $p_i$ là các phần tử dương của K.*

Điều kiện đó hiển nhiên là đủ; nó cũng là cần thiết, vì (theo ký hiệu trong chứng minh của Định lý 1), nếu $x \notin P_0$ thì tồn tại một phần tử cực đại P của $\mathcal{M}$ sao cho $x \notin P$; khi đó $-x \in P$ theo Bổ đề, và x không dương theo thứ tự được xác định bởi P, vì $x \neq 0$.

### 4. Mở rộng đại số của các trường có thứ tự

Cho K là một trường có thứ tự, và f là một đa thức trong K[X]. Ta sẽ nói rằng *f đổi dấu trong K* nếu tồn tại hai phần tử a và b trong K sao cho $f(a) f(b) < 0$; khi đó ta nói rằng *f đổi dấu giữa a và b*.

#### Mệnh đề 3 {#alg-vi-s2-prop-3 .statement}

*Cho K là một trường có thứ tự và f là một đa thức bất khả quy trên K đổi dấu giữa a và b trong K. Khi đó mở rộng $E = K[X]/(f)$ của K mang cấu trúc của một mở rộng có thứ tự.*

Ta sẽ chứng minh bằng quy nạp theo bậc n của f. Với $n = 1$ thì chứng minh là tầm thường. Giả sử kết quả đúng cho các bậc $\leq n - 1$, và ta hãy chứng minh nó cho bậc n bằng phản chứng; theo Định lý 1, do đó ta đang giả sử một quan hệ có dạng

$$
1 + \sum_i p_i f_i^2(X) \equiv 0 \pmod{f(X)}, \quad \text{where } f_i \in K[X], \quad p_i \in K \quad \text{and} \quad p_i \geq 0
$$

Không mất tính tổng quát, ta có thể giả sử rằng các $f_i$ có bậc $\leq n - 1$ (*IV*, p. 11, Hệ quả). Khi đó

$$
1 + \sum_i p_i f_i^2(X) = h(X) f(X)
$$

trong đó $h \neq 0$ có bậc nhiều nhất là $n - 2$. Thay X bởi a và b trong bất đẳng thức trên, ta thấy rằng $h(a) f(a) > 0$ và $h(b) f(b) > 0$. Vì f đổi dấu giữa a và b theo giả thiết, ta kết luận rằng $h(a) h(b) < 0$. Khi đó ta có một bất đẳng thức tương tự cho một trong các thừa số bất khả quy $ g(X) $ của $ h(X) $: tức là $ g(a)\ g(b) < 0 $. Nhưng $ 1 + \sum_i P_i f_i^2(X) \equiv 0 \pmod{g(X)} $, điều đó cho thấy rằng trường $ K[X]/(g) $ không thể là một mở rộng có thứ tự của $ K $ (Định lý 1), trái với giả thiết quy nạp.

#### Nhận xét {#alg-vi-s2-n4-rem-1 .statement}

Tồn tại các đa thức bất khả quy $ f $ trên một trường có thứ tự $ K $ không đổi dấu trong $ K $, nhưng sao cho $ K[X]/(f) $ mang cấu trúc của một mở rộng có thứ tự của $ K $ (xem VI, p. 43, Bài tập 26, c)).

Để áp dụng mệnh đề trước, ta cần kết quả sau:

#### Mệnh đề 4 {#alg-vi-s2-prop-4 .statement}

— *Cho $ K $ là một trường có thứ tự và cho $ f \in K[X] $. Tồn tại một khoảng trong $ K $, ngoài khoảng đó $ f $ nhận cùng dấu với số hạng bậc cao nhất của nó.*

Ta có thể ngay lập tức rút gọn về trường hợp của một đa thức đơn khởi; khi đó ta có thể viết $ f(x) = x^n(1 + a_1 x^{-1} + \ldots + a_n x^{-n}) $ với $ x \neq 0 $. Đặt

$$
M = \sup (1, |a_1| + \cdots + |a_n|).
$$

Với $ |x| > M $ ta có $ 1 + a_1 x^{-1} + \ldots + a_n x^{-n} > 0 $, điều này hoàn thành chứng minh của mệnh đề.

#### Hệ quả 1 {#alg-vi-s2-prop-4-cor-1 .statement}

— *Mọi mở rộng của một trường có thứ tự có bậc hữu hạn lẻ đều mang cấu trúc của một mở rộng có thứ tự.*

Mở rộng như vậy, vì là đơn sinh (V, p. 40, Định lý 1), thì đẳng cấu với $ K[X]/(f) $, trong đó $ f $ là một đa thức bất khả quy bậc lẻ. Khi đó chỉ cần chứng minh rằng $ f $ đổi dấu trong $ K $ (Mệnh đề 3), điều này suy ra ngay lập tức từ Mệnh đề 4.

#### Hệ quả 2 {#alg-vi-s2-prop-4-cor-2 .statement}

— *Nếu $ a $ là một phần tử dương của một trường có thứ tự $ K $, thì mọi trường phân rã $ E $ của đa thức $ X^2 - a $ đều mang cấu trúc của một mở rộng có thứ tự của $ K $.*

Kết quả là tầm thường nếu $ a $ là một bình phương trong $ K $. Ngược lại, đa thức $ f(X) = X^2 - a $ là bất khả quy và đổi dấu, vì $ f(0) < 0 $ và $ f(x) $ có cùng dấu với $ x^2 $, nên dương, khi $ x $ nằm ngoài một khoảng nào đó của $ K $. Bây giờ ta có thể hoàn thành chứng minh bằng cách áp dụng Mệnh đề 3.

#### Nhận xét {#alg-vi-s2-n4-rem-2 .statement}

Khi trường có thứ tự $ K $ chứa các « căn bậc hai » của một phần tử dương $ a $ của $ K $ (nghiệm của đa thức $ X^2 - a $) thì ký hiệu $ \sqrt{a} $ nói chung được dành cho căn bậc hai *dương*. Nếu $ K $ *không* chứa các căn bậc hai $ b $ và $ -b $ của $ a $ trong trường $ E $, thì trường sau có thể được làm thành một mở rộng có thứ tự của $ K $ theo *hai* cách, mỗi cách được cảm sinh từ cách kia *qua* tự đẳng cấu $ K $ biến $ b $ thành $ -b $; lựa chọn một trong các thứ tự này xác định $ \sqrt{a} $: đó là phần tử nào trong hai phần tử $ b $ và $ -b $ là dương.

Nếu $ a $ và $ a' $ là hai phần tử dương của $ K $, có các căn bậc hai thuộc $ K $, thì $ \sqrt{aa'} = \sqrt{a} \sqrt{a'} $, điều này suy ra từ định nghĩa của $ \sqrt{a} $ và quy tắc về dấu.

### 5. Các trường có thứ tự cực đại

#### Định nghĩa 4 {#alg-vi-s2-def-4 .statement}

— *Một trường có thứ tự K là cực đại nếu mọi mở rộng đại số có thứ tự của K đều là tầm thường.*

#### Ví dụ {#alg-vi-s2-n5-exa-1 .statement}

*Sau này (Gen. Top., VIII, p. 1) chúng ta sẽ thấy rằng trường R các số thực là một trường có thứ tự cực đại.*

Sự tồn tại của các trường có thứ tự cực đại là một hệ quả của định lý sau:

#### Định lý 2 {#alg-vi-s2-thm-2 .statement}

— *Mọi trường có thứ tự K đều có một mở rộng đại số có thứ tự là một trường có thứ tự cực đại.*

Có thể chứng minh rằng mở rộng có thứ tự này là duy nhất tới đẳng cấu K (VI, p. 40, Ex. 15).

Cho $ \Omega $ là một bao đóng đại số của K, và cho $ \mathfrak{N} $ là tập hợp các cặp $(A, w)$, trong đó $A$ là một mở rộng con trên K của $ \Omega $, và $w$ là một thứ tự trên $A$ làm cho $A$ trở thành một mở rộng có thứ tự của $K$. Sắp thứ tự $ \mathfrak{N} $ theo quan hệ « L là một mở rộng có thứ tự của M » giữa M và $L$. Được trang bị thứ tự này, $ \mathfrak{N} $ là một tập hợp có thứ tự *quy nạp*: thật vậy, nếu $(L_i)$ là một họ được sắp thứ tự toàn phần các phần tử của $ \mathfrak{N} $, thì trường $L = \bigcup L_i$, được sắp thứ tự bằng cách lấy $L_1 = \bigcup (L_i)_1$, là một cận trên của các $L_i$. Khi đó $ \mathfrak{N} $ có một phần tử cực đại, theo *Lý thuyết Tập hợp*, III, p. 154, Th. 2, điều này hoàn tất chứng minh.

#### Mệnh đề 5 {#alg-vi-s2-prop-5 .statement}

— *Cho K là một trường có thứ tự cực đại, và cho f là một đa thức trong K[X] đổi dấu giữa hai phần tử a và b của K (với $a < b$). Khi đó f có một nghiệm x trong K sao cho $a < x < b$.*

Ít nhất một trong các nhân tử bất khả quy của f, chẳng hạn $h$, đổi dấu giữa $a$ và $b$. Khi đó trường $K[X]/(h)$ có cấu trúc của một mở rộng có thứ tự của $K$ (VI, p. 23, Prop. 3), và $h$ có bậc 1 (Định nghĩa 4). Vì $h(a) h(b) < 0$, nghiệm duy nhất $x$ của $h$ thỏa mãn $a < x < b$, vì một hàm đa thức bậc 1 là đơn điệu.

#### Mệnh đề 6 {#alg-vi-s2-prop-6 .statement}

— *Mọi phần tử dương của một trường có thứ tự cực đại K đều có căn bậc hai trong K. Mọi đa thức bậc lẻ trong K[X] đều có ít nhất một nghiệm trong K.*

Điều này suy ra ngay lập tức từ Hệ quả 2 và 1 của Mệnh đề 4 trong VI, p. 24.

#### Hệ quả {#alg-vi-s2-n5-cor-1 .statement}

— *Trên một trường có thứ tự cực đại K chỉ tồn tại duy nhất một thứ tự tương thích với cấu trúc trường.*

Thật vậy, các phần tử dương của K được xác định bởi cấu trúc đại số của nó: chúng là các bình phương.

### 6. Đặc trưng của các trường có thứ tự cực đại. Định lý Euler-Lagrange

Tính chất được phát biểu trong Mệnh đề 6 của VI, p. 25 đặc trưng cho các trường có thứ tự cực đại. Chính xác hơn:

#### Định lý 3 (Euler-Lagrange) {#alg-vi-s2-thm-3 .statement}

— Cho K là một trường có thứ tự. Khi đó ba tính chất sau là tương đương:
a) Trường $ K(i) $ là đóng đại số (trong đó i ký hiệu một căn bậc hai của -1).
b) Trường có thứ tự K là cực đại.
c) Mọi phần tử dương của K là một bình phương, và mọi đa thức bậc lẻ trong $ K[X] $ đều có một nghiệm trong K.

Rõ ràng a) kéo theo b): thật vậy, K chỉ có hai mở rộng đại số tới đẳng cấu, chính trường K và $ K(i) $, trường sau không thể có thứ tự vì -1 là một bình phương.

Việc b) kéo theo c) không gì khác ngoài Mệnh đề 6 của VI, p. 25.

Còn lại là chứng minh rằng c) kéo theo a). Điều này sẽ suy ra từ hai mệnh đề tiếp theo.

#### Mệnh đề 7 {#alg-vi-s2-prop-7 .statement}

— Cho K là một trường có thứ tự trong đó mọi phần tử dương đều là một bình phương. Khi đó mọi phần tử của $ K(i) $ đều là một bình phương, và mọi đa thức bậc 2 trên $ K(i) $ đều có một nghiệm trong $ K(i) $.

Trước hết hãy chứng minh rằng mệnh đề thứ hai quy về mệnh đề thứ nhất. Ta có thể đưa đa thức bậc hai $ aX^2 + bX + c $ ($ a \neq 0 $) về dạng sau, thường gọi là dạng tam thức chính tắc:

$$
a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2)
$$

Nếu d là một căn bậc hai của $ (b^2 - 4ac)/4a^2 $, thì $ d - (b/2a) $ là một nghiệm của đa thức bậc hai đang xét.

Bây giờ ta chứng minh rằng mọi phần tử $ a + bi $ ($ a \in K, b \in K $) đều là một bình phương; ta xét một phần tử $ x + yi $ sao cho

$$
(x + yi)^2 = a + bi;
$$

điều này tương đương với $ x^2 - y^2 = a $ và $ 2xy = b $. Từ đây ta suy ra rằng

$$
(x^2 + y^2)^2 = a^2 + b^2
$$

Gọi c là căn bậc hai dương của $ a^2 + b^2 $; khi đó $ c \geq |a|, c \geq |b| $ và $ x^2 + y^2 = c $. Do đó $ x^2 = (c + a)/2 $ và $ y^2 = (c - a)/2 $. Vì $ c \geq |a| $ nên các phương trình này giải được trong K, và nếu $ x_0 $ và $ y_0 $ là hai nghiệm thì $ x_0^2 - y_0^2 = a $ và $ 2x_0y_0 = \pm b $. Ta thu được căn bậc hai mong muốn bằng cách lấy $ x = x_0 $ và $ y = b/2x_0 $.

#### Mệnh đề 8 {#alg-vi-s2-prop-8 .statement}

— Cho K là một trường giao hoán (với đặc số tùy ý) và cho $ K' $ là một trường phân rã của đa thức $ X^2 + 1 \in K[X] $ (V, p. 21). Giả sử:
a) every polynomial in $ K[X] $ of odd degree has a root in $ K' $;

b) every polynomial in $ K'[X] $ of degree 2 has a root in $ K' $.
Thì $ K' $ là đóng đại số.

Chú ý trước hết rằng chỉ cần chứng minh mọi đa thức không hằng trong $ K[X] $ có một nghiệm trong $ K' $: điều này quả là hiển nhiên nếu $ K' = K $; nếu $ K' \neq K $ thì $[K':K] = 2$; cho $ a \mapsto a $ ký hiệu tự đẳng cấu của $ K' $ trên $ K $ duy nhất khác với ánh xạ đồng nhất; nếu $ f \in K'[X] $ và nếu $ \bar{f} $ là đa thức thu được bằng cách áp dụng $ a \mapsto \bar{a} $ lên các hệ số của $ f $, thì $ f \bar{f} \in K[X] $; nếu $ a \in K' $ là một nghiệm của $ f \bar{f} $ thì $ a $ либо là một nghiệm của $ f $ hoặc của $ \bar{f} $; do đó либо $ a $ hoặc $ a $ là một nghiệm của $ f $.

Do đó, hãy cho $ f $ là một đa thức trên $ K $ có bậc $ 2^n p $, $ p $ lẻ. *Ta* sẽ tiến hành quy nạp theo $ n $, tính chất đúng với $ n = 0 $ theo giả thiết *a)*. Cho E là một mở rộng của K trong đó $ f $ tách thành các nhân tử tuyến tính:

$$
f(X) = \prod_i (X - a_i)
$$

Cho $ b \in K $; đặt $ y_{ij} = a_i + a_j + ba_i a_j \in E $ và

$$
h(X) = \prod_{i < j} (X - y_{ij}) \in E[X].
$$

Các hệ số của đa thức này là các hàm đối xứng theo các $ a_i $, với các hệ số trong $ K $; do đó nó thuộc $ K[X] $ (IV, p. 62, Th. 1); vì nó có bậc $ 2^n p (2^n p - 1)/2 = 2^{n-1} p' $ ($ p' $ lẻ), nó có một nghiệm $ y_{} $, trong $ K' $ theo giả thiết quy nạp. Nếu ta chú ý rằng điều này đúng với mọi $ b \in K $, và rằng $ K $ là một trường vô hạn (thực vậy là một trường hữu hạn, mà có các mở rộng đơn sinh có bậc lẻ tùy ý lớn (V, p. 94, Mệnh đề 3), không thể thỏa mãn *a)*), thì ta có thể suy ra sự tồn tại của ít nhất một cặp $(i, j)$ sao cho

$$
a_i + a_j + ba_i a_j \in K' \quad \text{và} \quad a_i + a_j + b'a_i a_j \in K',
$$

với $ b \neq b' $. Khi đó $ a_i + a_j $ và $ a_i a_j $ là các phần tử của $ K' $, do đó $ a_i $ và $ a_j $ cũng vậy, vì chúng là các nghiệm của phương trình bậc hai

$$
x^2 - (a_i + a_j)x + a_i a_j = 0.
$$

Q.E.D.

Để có một tổng quát hóa và một chứng minh khác của Mệnh đề 8, dựa trên lý thuyết Galois, xem VI, p. 46, Bài tập 33.

Cho $ K $ là một trường có thứ tự và đặt $ K' = K(i) $; với mọi phần tử $ z = a + bi $ của $ K' $, chuẩn $ z \overline{z} = a^2 + b' $ của $ z $ đối với $ K $ (III, p. 544, ví dụ 1) là một phần tử dương của $ K $, triệt tiêu chỉ với $ z = 0 $. Nếu mọi phần tử dương trong $ K $ đều là một bình phương (đặc biệt nếu $ K $ là một trường có thứ tự cực đại), thì căn bậc hai dương của chuẩn $ z \overline{z} $ được gọi là giá trị tuyệt đối của $ z $, và được viết $ |z| $. Vì $ |zz'|^2 = |z|^2 |z'|^2 $ ta có $ |zz'| = |z| \cdot |z'| $.

Ngoài ra, bất đẳng thức tam giác

$$
|z + z'| \leq |z| + |z'|
$$

đúng với mọi cặp phần tử $ z, z' $ của $ K' $. Thật vậy, nếu $ z = a + bi $ và $ z' = a' + b'i $, thì bất đẳng thức này tương đương với

$$
(a + a')^2 + (b + b')^2 \leq a^2 + b^2 + {a'}^2 + {b'}^2 + 2 \sqrt{(a^2 + b^2)({a'}^2 + {b'}^2)}
$$

và do đó cũng tương đương với

$$
(aa' + bb')^2 \leq (a^2 + b^2)({a'}^2 + {b'}^2)
$$

có thể viết là $ (ab' - ba')^2 \geq 0 $.

Định lý 3 cho phép ta xác định tất cả các đa thức bất khả quy trên một trường có thứ tự cực đại:

#### Mệnh đề 9 {#alg-vi-s2-prop-9 .statement}

— *Nếu K là một trường có thứ tự cực đại, thì các đa thức bất khả quy duy nhất trong K[X] là các đa thức bậc nhất, và các đa thức bậc hai $ aX^2 + bX + c $ sao cho $ b^2 - 4ac < 0 $.*

Vì $ K(i) $ là đóng đại số, mọi mở rộng đại số của K, và do đó mọi đa thức bất khả quy trên K, đều có bậc 1 hoặc 2. Để xem các đa thức bậc hai nào là bất khả quy, chỉ cần xét dạng chính tắc $ a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2) $ (xem *VI*, p. 26, Mệnh đề 7).

#### Nhận xét {#alg-vi-s2-n6-rem-1 .statement}

— Chuyển sang dạng tam thức chính tắc cho kết quả mạnh hơn này: một điều kiện cần và đủ để đa thức $ aX^2 + bX + c $ trên một trường có thứ tự K cho trước có dấu không đổi trong K là $ b^2 - 4ac < 0 $, và khi đó dấu của đa thức là dấu của $ a $.

### 7. Các không gian vectơ trên một trường có thứ tự

Cho K là một trường có thứ tự, và cho E là một không gian vectơ trên $ K $. Quan hệ « tồn tại $ \lambda > 0 $ trong $ K $ sao cho $ y = \lambda x $ » giữa hai phần tử $ x $ và $ y $ trong tập $ E - \{0\} $ là một *quan hệ tương đương*. Các lớp tương đương theo quan hệ này được gọi là *nửa đường thẳng mở có gốc 0*; hợp của một nửa đường thẳng mở và $ \{0\} $ được gọi là một *nửa đường thẳng đóng* (hoặc đôi khi đơn giản là một *nửa đường thẳng*) có gốc 0. Mọi vectơ $ a \neq 0 $ nằm trong một nửa đường thẳng mở (tương ứng đóng) $ A $ được gọi là một *vectơ chỉ phương* của $ A $, và $ A $ là tập hợp các vectơ $ ha $ với mọi vô hướng $ A > 0 $ (tương ứng $ A \geq 0 $). Mỗi đường thẳng $ D $ qua 0 chứa đúng hai nửa đường thẳng mở (tương ứng đóng) có gốc 0 ; nếu $ A $ là một trong hai nửa đường thẳng ấy, thì $ -A $ là nửa đường thẳng kia (được gọi là *đối* của $ A $).

Giờ nếu $ F $ là một *không gian affine* trên $ K $, và E là không gian tịnh tiến của F, thì mọi tập con của F có dạng $ A = a + A_0 $, trong đó $ \Delta_0 $ là một nửa đường thẳng mở (tương ứng đóng) của E, được gọi là một *nửa đường thẳng* *mở* (tương ứng *đóng*) *có gốc* $ a \in F $. Nửa đường thẳng $ \Delta_0 $ được xác định hoàn toàn bởi $ A $ (vì nó là nửa đường thẳng có vectơ chỉ phương $ b - a $, với mọi $ b \neq a $ trong $ A $), và được gọi là *hướng* của $ A $; một vectơ chỉ phương của $ A $, cũng được gọi là một *vectơ chỉ phương* của $ A $.

Giả sử bây giờ rằng E có *chiều* *hữu hạn* $ n $ trên K ; khi đó người ta biết (III, p. 518, Hệ quả 1) rằng *lũy thừa ngoài bậc n* $ \Lambda^n E $ là một không gian vectơ có chiều 1 trên K, và do đó là hợp của hai nửa đường thẳng đóng đối nhau có gốc 0. Những nửa đường thẳng này được gọi là các định hướng của E; không gian E cùng với một trong các nửa đường thẳng ấy A được gọi là có định hướng; khi đó một n-vectơ z được gọi là dương (tương ứng âm) theo định hướng này nếu nó thuộc A (tương ứng thuộc −A); nó là âm (tương ứng dương) theo định hướng đối.

Một định hướng của một không gian affine F trên K là, theo định nghĩa, một định hướng của không gian tịnh tiến của F; không gian F, cùng với một định hướng như vậy, được gọi là một không gian affine có định hướng.

Cho E là một không gian vectơ có định hướng trên K, có chiều $ n $ ; một cơ sở có thứ tự $ (a_i)_{1 \leq i \leq n} $ của E được gọi là dương hay trực tiếp (tương ứng âm hay nghịch đảo) nếu n-vectơ $ a_1 a_2 \ldots a_n $ là dương (tương ứng âm). Nếu $ u $ là một tự đẳng cấu của không gian vectơ E thì $ (\bigwedge^n u)(z) = \det(u) \cdot z $ với mọi $ z \in \bigwedge^n E $, do đó điều kiện cần và đủ để $ \bigwedge^n u $ giữ bất biến định hướng của E (hay, như ta cũng nói, bảo toàn định hướng) là $ \det(u) > 0 $; các tự đẳng cấu có tính chất này chính xác là các tự đẳng cấu của E với tư cách là một không gian vectơ có định hướng; chúng lập thành một nhóm con chuẩn tắc $ \mathrm{GL}^+(E) $ của nhóm tuyến tính $ \mathrm{GL}(E) $, nhóm này có chỉ số 2 bất cứ khi nào $ E \neq 0 $.

Khi $ E = 0 $ thì $ \mathrm{GL}(E) = \mathrm{End}(E) $ chỉ chứa ánh xạ đồng nhất 1, và theo định nghĩa $ \det(1_E) = 1 $. Chú ý rằng $ \bigwedge^n E = \bigwedge^0 E = K $ theo định nghĩa trong trường hợp này; nửa đường thẳng của K được tạo thành bởi các vô hướng dương được gọi là định hướng chính tắc của không gian không.

Cho M và N là hai không gian con bù nhau có chiều p và $ n - p $ tương ứng trong không gian vectơ E có chiều n; nếu $ z' $ (tương ứng $ z'' $) là một vectơ khác không trong $ \bigwedge^p M $ (tương ứng $ \bigwedge^{n-p} N $), thì $ z' \wedge z'' $ là một vectơ khác không trong $ \bigwedge^n E $. Cho một định hướng trên M và một định hướng trên N, các vectơ $ z' \wedge z'' $ với $ z' $ và $ z'' $ dương tạo thành một định hướng của E, được gọi là định hướng tích của định hướng của M với định hướng của N (phụ thuộc vào thứ tự của các thừa số khi $ p(n-p) $ là lẻ). Ngược lại, cho các định hướng trên E và trên M, tồn tại một định hướng duy nhất trên N sao cho định hướng đã cho trên E là tích của định hướng đã cho trên M và định hướng này trên N (theo thứ tự đó); định hướng này được gọi là bù với định hướng của M đối với định hướng của E. Nếu $ N' $ là một không gian con bù thứ hai của M, phép chiếu chính tắc $ N \to N' $ song song với M biến định hướng bù của N thành định hướng bù của $ N' $. Ảnh của định hướng bù của N qua ánh xạ chính tắc $ N \to E/M $ do đó độc lập với lựa chọn không gian bù N; nó được gọi là định hướng thương trên E/M của định hướng của E theo định hướng của M.

Các bài tập

### Các bài tập {#alg-vi-s2-exercises}

Tất cả các vành được xét đều được giả sử là giao hoán trừ khi được nêu tường minh là khác.

Xem [các bài tập cho § 2](exercises/s2/).
