---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 6
section_title: Etale algebras
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.26-A V.36, A V.151
pdf_pages: 0140-0150, 0265-0265
extraction: ocr
subsections:
    - "no": 1
      title: Linear independence of homomorphisms
      page: 26
      pdf_page: 140
    - "no": 2
      title: Algebraic independence of homomorphisms
      page: 28
      pdf_page: 142
    - "no": 3
      title: Diagonalizable algebras and etale algebras
      page: 28
      pdf_page: 142
    - "no": 4
      title: Subalgebras of an etale algebra
      page: 30
      pdf_page: 144
    - "no": 5
      title: Separable degree of a commutative algebra
      page: 31
      pdf_page: 145
    - "no": 6
      title: Differential characterization of etale algebras
      page: 33
      pdf_page: 147
    - "no": 7
      title: Reduced algebras and etale algebras
      page: 34
      pdf_page: 148
statements: 22
exercises: 2
content_sha256: 6814b730df6c63dfd0d4e93489f1f8c857559d4e7f4835dc7114ee0650466db0
translated_from: content/en/alg/V/06_s6_etale_algebras.md
source_content_sha256: 1e1d8007a12d561b9aab4fe1f0fdc218310c13da2cf43b259e24998de8869633
translation_model: gpt-5.4
translation_run: translate-vi-1025ba98
glossary_version: 34
glossary_terms_sha256: 3592a12f8526cc690d835d3e9c257b52c4d60c679e2831e9928b5713568599f7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. ĐẠI SỐ ETALE

Trong suốt đoạn này, K ký hiệu một trường.

### 1. Tính độc lập tuyến tính của các đồng cấu

Cho L là một mở rộng của K và V là một không gian vectơ trên K. Trong đoạn này, ta sẽ ký hiệu bởi $ \operatorname{Hom}_K(V, L) $ tập hợp tất cả các ánh xạ K-tuyến tính từ V vào L, được trang bị cấu trúc không gian vectơ trên L sao cho:

(1) $$(f + g)(x) = f(x) + g(x)\,,\quad (\alpha f)(x) = \alpha f(x)$$

với $x \in V,\ a \in L$ và $f,\ g$ trong $\mathrm{Hom}_K(V, L)$. Đặt $V_{(L)} = L \otimes_K V$ là không gian vectơ trên L dẫn xuất từ V bởi mở rộng vô hướng, và $(V_{(L)})^*$ là không gian đối ngẫu của nó. Theo II, p. 277 ta có một đẳng cấu chính tắc $u \mapsto 3$ của các không gian vectơ trên L từ $(V_{(L)})^*$ lên $\mathrm{Hom}_K(V, L)$ sao cho $\tilde{u}(x) = u(1 \otimes x)$ với $x \in V$ và $u$ trong $(V_{(L)})^*$. Nếu V có chiều *hữu hạn* $n$ trên $K$, thì không gian vectơ $(V_{(L)})$ trên $L$ có chiều $n$, cũng như không gian đối ngẫu của nó $(V_{(L)})^* = V_{(\bar{L})}^*$, do đó có công thức

(2) $$[\mathrm{Hom}_K(V, L) : L] = [V : K]$$

#### Định lý 1 {#alg-v-s6-thm-1 .statement}

— *Cho L là một mở rộng của một trường K và A là một đại số trên K; gọi $\mathcal{H}$ là tập hợp tất cả các đồng cấu K-đại số từ A vào L. Khi đó $\mathcal{H}$ là một tập con tự do của không gian vectơ $\mathrm{Hom}_K(A, L)$ trên L.*

Ta sẽ chứng minh bằng quy nạp theo số nguyên $n \geq 0$ rằng mọi dãy $(u_1, \ldots, u_n)$ gồm các phần tử phân biệt của $\mathcal{H}$ là tự do. Trường hợp $n = 0$ là tầm thường, nên từ đây ta có thể giả sử rằng $n \geq 1$; gọi $a_1, \ldots, a_n$ là các phần tử của L sao cho $$\sum_{i=1}^n \alpha_i u_i = 0.$$ Với $x,\ y$ trong A ta có
$$
\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i(y) = \sum_{i=1}^n \alpha_i u_i(xy) - u_n(x) \sum_{i=1}^n \alpha_i u_i(y) = 0,
$$
do đó $$\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i = 0.$$ Theo giả thiết quy nạp, các phần tử $u_1, \ldots, u_{n-1}$ của $\mathcal{H}$ độc lập tuyến tính, do đó $\alpha_i [u_i(x) - u_n(x)] = 0$ với $1 \leq i \leq n-1$ và với mọi $x$ trong A. Vì các $u_i$ phân biệt, điều này kéo theo $\alpha_i = 0$ với $i \neq n$, do đó $\alpha_n u_n = 0$ và vậy $\alpha_n = \alpha_n u_n(1) = 0$ (ở đây ký hiệu 1 là phần tử đơn vị của A). Vậy ta đã chứng minh rằng $a_1, \ldots, a_{n-1}, \alpha_n$ bằng không, và điều này chứng minh định lý.

#### Hệ quả 1 {#alg-v-s6-thm-1-cor-1 .statement}

— *Cho $\Gamma$ là một monoid, L một trường và X một tập hợp các đồng cấu từ $\Gamma$ vào monoid nhân của L. Khi đó X là một tập con tự do của không gian vectơ trên L $L^\Gamma$ gồm các ánh xạ từ $\Gamma$ vào L.*

Gọi A là đại số của monoid $\Gamma$ với hệ số trong L và $(e,)_{\gamma}$ là cơ sở chính tắc của A trên L (III, p. 446). Với mọi ánh xạ L-tuyến tính $u$ từ A vào L, viết $\tilde{u}(\gamma) = u(e,\gamma)$ (với $\gamma \in \Gamma$); khi đó ánh xạ $u \mapsto 3$ là một đẳng cấu của các không gian vectơ trên L từ $\mathrm{Hom}_L(A, L)$ lên $L^\Gamma$, và biến tập hợp các đồng cấu L-đại số từ A vào L thành X. Bây giờ chỉ cần áp dụng Định lý 1 với $K = L$.

**HỆ QUẢ 2** (định lý của Dedekind). — *Cho E và L là hai mở rộng của K. Tập hợp các K-đồng cấu từ E vào L là tự do trên L. Nếu E có bậc hữu hạn trên K thì số các K-đồng cấu từ E vào L không vượt quá $[E : K]$.*

Khẳng định cuối cùng suy ra từ khẳng định thứ nhất, có tính đến Công thức (2).

### 2. Tính độc lập đại số của các đồng cấu

#### Định lý 2 {#alg-v-s6-thm-2 .statement}

— Cho K là một trường vô hạn, L là một mở rộng của K và A là một đại số trên K. Gọi $ u_1, \ldots, u_n $ là các đồng cấu K-đại số phân biệt của A vào L và f là một đa thức trong $ L[X_1, \ldots, X_j] $. Nếu ta có $ f(u_1(x), \ldots, u_n(x)) = 0 $ với mọi $ x \in A $, thì $ f = 0 $.

Gọi B là tập hợp các phần tử của $ L^n $ có dạng $ (u_1(x), \ldots, u_n(x)) $ với $ x \in A $. Theo Định lý 1, không tồn tại dãy $ (a,, \ldots, a,) $ các phần tử không đồng thời bằng không của L sao cho $ \sum_{i=1}^n \alpha_i u_i(x) = 0 $ với mọi $ x \in A $; do đó (II, p. 301, Định lý 7) B sinh ra không gian vectơ $ L^n $ trên L. Vậy tồn tại các phần tử $ a,, \ldots, a, $ của $ A $ sao cho ma trận $ (u_i(a_j))_{1 \leq i,j \leq n} $ là khả nghịch.

Hãy định nghĩa đa thức $ g \in L[Y_1, \ldots, Y_n] $ bởi
$$
g(Y_1, \ldots, Y_n) = f \left( \sum_{j=1}^n u_1(a_j) Y_j, \ldots, \sum_{j=1}^n u_n(a_j) Y_j \right).
$$
Cho $ y_1, \ldots, y, $ thuộc $ K $; viết $ x = \sum_{i=1}^n y_i a_i $, ta có
$$
g(y_1, \ldots, y_n) = f(u_1(x), \ldots, u_n(x)),
$$
do đó $ g(y_1, \ldots, y_n) = 0 $
theo giả thiết trên $ f $. Vì trường $ K $ là vô hạn, ta có $ g = 0 $ (IV, p. 18, Hệ quả 2); bây giờ ma trận $ (u_i(a_j)) $ có ma trận nghịch đảo $ (b_{ij}) $ và ta có
$$
f(X_1, \ldots, X_n) = g \left( \sum_{j=1}^n b_{1j} X_j, \ldots, \sum_{j=1}^n b_{nj} X_j \right),
$$
do đó $ f = 0 $.

Định lý 2 không có mệnh đề tương tự đối với các trường hữu hạn. Do đó cho $ K $ là một trường hữu hạn có q phần tử, $ A = L = K $ và $ f(X) = X^q - X $. Ta có $ x^q = x $ với mọi $ x \in K $ (V, p. 93, Mệnh đề 2); vì vậy nếu $ u $ là tự đẳng cấu đồng nhất của $ K $, thì $ f(u(x)) = 0 $ với mọi $ x \in K $, mặc dù $ f $ khác không.

### 3. Đại số chéo hóa được và đại số étale

#### Định nghĩa 1 {#alg-v-s6-def-1 .statement}

— Cho A là một đại số trên K; khi đó A được gọi là chéo hóa được nếu tồn tại một số nguyên $ n \geq 0 $ sao cho A đẳng cấu với đại số tích $ K^n $. Ta nói rằng A được chéo hóa bởi một mở rộng L của K nếu đại số trên L $ A_{(L)} $ dẫn xuất từ A bằng mở rộng vô hướng là chéo hóa được. Ta sẽ nói rằng A là étale nếu tồn tại một mở rộng của K chéo hóa A.

Ta nhắc lại rằng đại số tích $ K'' $ là không gian vectơ $ K'' $ được trang bị phép nhân xác định bởi

$$
(x_1, \ldots, x_n) \cdot (y_1, \ldots, y_n) = (x_1 y_1, \ldots, x_n y_n)
$$

Nếu $ \varepsilon_1, \ldots, \varepsilon_n $ là cơ sở chính tắc của $ K^n $, ta có

$$
\varepsilon_i^2 = \varepsilon_i , \quad \varepsilon_i \varepsilon_j = 0 \quad \text{nếu} \quad i \neq j
$$

và $ 1 = \varepsilon_1 + \ldots + \varepsilon_n $.

Mọi đại số etale trên $ \mathbf{K} $ đều *giao hoán* và có *bậc hữu hạn* trên $ K $.

#### Mệnh đề 1 {#alg-v-s6-prop-1 .statement}

*Cho A là một đại số bậc hữu hạn n trên trường K ; khi đó các điều kiện sau là tương đương :*
  *a)* *Đại số A chéo hóa được.*
  *b)* *Tồn tại một cơ sở $ (e_1, \ldots, e_n) $ của A sao cho $ e_i^2 = e_i $ và $ e_i e_j = 0 $ với $ i \neq j $.*
  *c)* *Các đồng cấu đại số trên K từ A vào $ \mathbf{K} $ sinh ra đối ngẫu của không gian vectơ trên K A.*
  *d)* *Mọi A-môđun đều là tổng trực tiếp của các môđun con có chiều bằng 1 trên K.*

Sự tương đương của *a)* và *b)* suy ra từ Công thức (6); mặt khác, n phép chiếu $ K^n \to K $ là các đồng cấu đại số, do đó *a)* kéo theo *c)*. Nếu *c)* đúng, các đồng cấu đại số của A vào $ \mathbf{K} $ lập thành một cơ sở của đối ngẫu của A (*V*, p. 27, Đl. 1), ta ký hiệu chúng bởi $ u_1, \ldots, u_n $; khi đó $ a \mapsto (u_i(a)) $ là một đẳng cấu của A lên đại số $ K'' $, do đó *a)*. Như vậy ta đã thiết lập được sự tương đương của các điều kiện *a)*, *b)* và *c)*.

Giả sử *b)* đúng và cho M là một A-môđun; khi đó các phép vị tự $ (e_i)_M $ với tỉ số $ e_i $ là các phép chiếu của $ M $, và $ M $ là tổng trực tiếp của các $ e_i M $, là những A-môđun con. Do đó ta có thể giả sử rằng tồn tại một chỉ số $ i $ sao cho $ (e_j)_M = 0 $ với $ j \neq i $. Khi đó mọi không gian con vectơ của $ M $ đều là một A-môđun con, do đó *d)*.

Ngược lại, giả sử *d)* được thỏa mãn và xét A-môđun A,. Khi đó tồn tại một cơ sở $ (f_i) $ của không gian vectơ A trên K sao cho $ Af_i = Kf_i $ với $ i = 1, \ldots, n $. Sau khi thay thế mỗi $ f_i $ bằng một bội vô hướng thích hợp, nếu cần, ta có thể giả sử rằng $ 1 = f_i + \ldots + f_n $. Nếu $ i \neq j $, thì $ f_i f_j $ thuộc $ Af_i \cap Af_j = Kf_i \cap Kf_j $, nên nó bằng không. Bây giờ $ f_i = f_i f_1 + \ldots + f_i f_n = f_i^2 $, do đó *b)*.

#### Hệ quả {#alg-v-s6-n3-cor-1 .statement}

*Cho L là một mở rộng của K và $ \mathcal{H} $ là tập hợp các đồng cấu đại số từ A vào L. Ta có Card $ \mathcal{H} \leq [A : K] $, với đẳng thức khi và chỉ khi A được chéo hóa bởi L. Nếu A được chéo hóa bởi L, thì $ \mathcal{H} $ là một cơ sở của không gian vectơ L $ \mathrm{Hom}_K(A, L) $.*

Không gian vectơ $ \mathrm{Hom}_K(A, L) $ trên L có chiều $ [A : K] $, theo Công thức (2), và $ \mathcal{H} $ là một tập con tự do của $ \mathrm{Hom}_K(A, L) $ theo Định lý 1 (*V*, p. 27). Do đó ta có Card $ \mathcal{H} \leq [A : K] $ với đẳng thức xảy ra khi và chỉ khi $ \mathcal{H} $ là một cơ sở của $ \mathrm{Hom}_K(A, L) $. Tồn tại một đẳng cấu giữa các không gian vectơ trên L, chẳng hạn $ \pi : \mathrm{Hom}_K(A, L) \to A_{(L)}^* $, được đặc trưng bởi $ u(x) = (\pi u)(1 \otimes x) $ với $ x \in A $, và $ \pi $ ánh xạ $ \mathcal{H} $ lên tập $ \mathcal{H}_L $ các đồng cấu đại số trên L của $ A(\cdot) $ vào L. Sau cùng, sự tương đương của $ a) $ và $ c) $ trong Mệnh đề 1 cho thấy rằng đại số $ A_{(L)} $ trên L là chéo hóa được khi và chỉ khi $ \mathcal{H}_L $ sinh ra không gian vectơ $ A_{(L)}^* $ trên L. Điều này hoàn tất chứng minh của Hệ quả.

#### Mệnh đề 2 {#alg-v-s6-prop-2 .statement}

— *Cho A là một đại số trên K và $ \Omega $ là một mở rộng đóng đại số của K. Các mệnh đề sau là tương đương*:

$ a) $ *Đại số A là etale*.
$ b) $ *Tồn tại một mở rộng bậc hữu hạn chéo hóa A*.
$ c) $ *Mở rộng $ \Omega $ của K chéo hóa A*.

Giả sử rằng A là etale. Gọi $ n $ là bậc của A trên K, gọi L là một mở rộng của K chéo hóa A và gọi $ \mathcal{H} $ là tập hợp các đồng cấu đại số của A vào L. Theo Hệ quả của Mệnh đề 1 ta có Card $ \mathcal{H} = n $. Mặt khác, với mỗi $ u \in \mathcal{H} $, ta có $[u(A):K] \leq n$. Theo V, p. 18, Định lý 2, mở rộng con L' của L được sinh bởi các ảnh của các phần tử của $ \mathcal{H} $ có bậc hữu hạn trên K. Vì tồn tại $ n $ đồng cấu phân biệt của A vào L', nên mở rộng L' chéo hóa A, theo Hệ quả 1 của Mệnh đề 1. Điều đó chứng tỏ rằng a) suy ra b).

Vì mọi mở rộng bậc hữu hạn của K đều đẳng cấu với một mở rộng con của $ \Omega $ (V, p. 20, Định lý 1), nên b) suy ra c). Sau cùng c) rõ ràng suy ra a).

### 4. Các đại số con của một đại số etale

#### Mệnh đề 3 {#alg-v-s6-prop-3 .statement}

— *Cho A là một đại số etale trên K. Chỉ có hữu hạn đại số con và iđêan của A. Hơn nữa, mọi mở rộng của K chéo hóa A cũng chéo hóa mọi đại số con và mọi đại số thương của A; đặc biệt các đại số này đều là etale*.

Chỉ cần chứng minh rằng một đại số $ K^n $ chỉ có một số hữu hạn các đại số con và iđêan, và rằng các đại số con và các đại số thương của $ K^n $ đều chéo hóa được. Ta ký hiệu bởi $ (\varepsilon_1, \ldots, \varepsilon_n) $ cơ sở chính tắc của $ K^n $.

Cho A là một đại số con của $ K^n $ và gọi $ v_1, \ldots, v_n $ là các hạn chế lên A của n phép chiếu $ K^n \to K $. Vì giao của các hạt nhân của các $ v_i $ rõ ràng là 0, các $ v_i $ sinh ra không gian vectơ đối ngẫu trên K của A (II, p. 302, Hệ quả 1); do đó K-đại số A là chéo hóa được (V, p. 29, Mệnh đề 1).

Với mọi tập con I của $ \{1, 2, \ldots, n\} $ đặt $ \varepsilon_I = \sum_{i \in I} \varepsilon_i $. Rõ ràng các phần tử $ \varepsilon_I $ là các phần tử lũy đẳng của $ K^n $; ta có $ \varepsilon_I = 0 $ khi và chỉ khi I rỗng, và $ \varepsilon_I \varepsilon_J = \varepsilon_{I \cap J} $. Theo điều đã nói ở trên, mọi đại số con A của $ K^n $ đều chéo hóa được; bởi điều kiện $ b) $ của Mệnh đề 1, do đó mọi đại số con A của $ K^n $ đều thừa nhận một cơ sở $ (\varepsilon_{I_1}, \ldots, \varepsilon_{I_p}) $, trong đó $ (I_1, \ldots, I_p) $ là một phân hoạch của $ \{1, 2, \ldots, n\} $, và chỉ có một số hữu hạn các đại số con như thế.

Với mọi tập con I của $ (1, 2, \ldots, n) $ đặt $ a_i $ là không gian con vectơ của $ K^n $ có cơ sở là các lũy đẳng $ \varepsilon_i $ với $ i \in I $; khi đó hiển nhiên $ a_i $ là một iđêan của $ K^n $; hơn nữa nếu $ J = (1, 2, \ldots, n) - I $, thì các lớp thặng dư $ \overline{\varepsilon}_j $ của $ \varepsilon_j $ mod $ a_i $, với $ j \in J $ tạo thành một cơ sở của $ K^n / a_i $. Ta có $ \overline{\varepsilon}_j^2 = \overline{\varepsilon}_j $ và $ \overline{\varepsilon}_j \overline{\varepsilon}_k = 0 $ nếu $ j \neq k $, do đó đại số $ K^n / a_I $ chéo hóa được, theo Mệnh đề 1 của V, p. 29.

Còn phải chỉ ra rằng mọi iđêan của $ K^n $ đều có dạng $ a_I $. Gọi I là tập hợp các số nguyên $ i $ sao cho $ 1 \leq i \leq n $ và $ \varepsilon_i \in a $, khi đó $ a_i \subset a $. Cho $ x = x_1 \varepsilon_1 + \cdots + x_n \varepsilon_n $ là một phần tử của $ a $ (với $ x_1, \ldots, x_n $ thuộc $ K $) và gọi $ i $ thuộc $ (1, 2, \ldots, n) - I $. Ta có $ x_i \varepsilon_i = x \varepsilon_i \in a_i $, và $ \varepsilon_i \notin a $, do đó $ x_i = 0 $. Vậy $ x = \sum_{i \in I} x_i \varepsilon_i $ và điều này cho thấy rằng $ x \in a_i $. Bây giờ ta đã chỉ ra $ a \subset a_I $, do đó cuối cùng $ a = a_i $.

#### Hệ quả {#alg-v-s6-n4-cor-1 .statement}

— *Cho $ A_1, \ldots, A_r $ là các đại số trên $ K $ và $ A = A_1 \times \cdots \times A_r $. Để $ A $ là etale thì điều kiện cần và đủ là $ A_1, \ldots, A_r $ đều etale.*

Giả sử rằng $ A $ là etale; mỗi đại số $ A_1, \ldots, A_r $ đều đẳng cấu với một thương của $ A $, và do đó là etale theo Mệnh đề 3. Ngược lại, mọi mở rộng của $ K $ làm chéo hóa $ A_1, \ldots, A_r $ rõ ràng cũng làm chéo hóa $ A $.

### 5. Bậc tách được của một đại số giao hoán

Cho $ A $ là một đại số giao hoán bậc hữu hạn $ n $ trên $ K $. Với mọi mở rộng $ L $ của $ K $, số $ h(L) $ các đồng cấu đại số từ $ A $ vào $ L $ là hữu hạn và bị chặn trên bởi $ n $ (V, p. 29, Hệ quả).

#### Bổ đề 1 {#alg-v-s6-lem-1 .statement}

— *Cho $ \Omega $ là một bao đóng đại số của $ K $; khi đó ta có $ h(L) \leq h(\Omega) $ với mọi mở rộng $ L $ của $ K $, với đẳng thức khi $ L $ đóng đại số.*

Đặt $ L' $ là bao đóng đại số của $ K $ trong $ L $. Với mọi đồng cấu $ u $ của $ A $ vào $ L $ ta có $ [u(A) : K] \leq n $, do đó $ u(A) \subset L' $ theo V, p. 18, Mệnh đề 2; vì thế ta có $ h(L') = h(L) $. Vì mở rộng $ L' $ của $ K $ đẳng cấu với một mở rộng con của $ \Omega $ (V, p. 20, Định lý 1), nên ta có $ h(L') \leq h(\Omega) $. Nếu $ L $ đóng đại số, thì $ L' $ là một bao đóng đại số của $ K $; khi đó các mở rộng $ L' $ và $ \Omega $ của $ K $ là đẳng cấu (V, p. 23, Định lý 2) và do đó $ h(L') = h(\Omega) $; Bổ đề suy ra trực tiếp từ điều này.

Theo Bổ đề 1, số $ h(L) $ có cùng giá trị đối với mọi mở rộng đóng đại số $ L $ của $ K $; số này sẽ được ký hiệu là $ [A : K] $, và được gọi là *bậc tách được* của $ A $.

Cho $ A $ và $ B $ là hai đại số giao hoán bậc hữu hạn trên $ K $. Ta sẽ thiết lập công thức

$$
[A \otimes_K B : K]_s = [A : K]_s \cdot [B : K]_s .
$$

Cho $ L $ là một mở rộng đóng đại số của $ K $ và ký hiệu bởi $ \mathcal{H}(A) $ tập hợp các đồng cấu đại số của $ A $ vào $ L $, và tương tự định nghĩa $ \mathcal{H}(B) $ và $ \mathcal{H}(A \otimes_K B) $. Theo định nghĩa ta có Card $ \mathcal{H}(A) = [A : K] $, và các công thức tương ứng cho [B : K] và [A \otimes_K B : K]. Hơn nữa (III, p. 465, Công thức (6)), công thức $(u * v)(a \otimes b) = u(a)v(b)$ định nghĩa một song ánh $(u, v) \mapsto u * v$ từ $\mathcal{H}(A) \times \mathcal{H}(B)$ lên $\mathcal{H}(A \otimes_K B)$, do đó suy ra Công thức (7).

Cho $K'$ là một mở rộng của $K$; ta sẽ chứng minh công thức
$$
[A_{(K')}: K'], = [A: K], .
$$
Thật vậy, lấy $L$ là một bao đóng đại số của $K'$. Công thức $\tilde{u}(x) = u(1 \otimes x)$ (với $x \in A$) xác định một song ánh $u \mapsto \tilde{u}$ giữa tập hợp các đồng cấu $K'$ của $A_{(K')}$ vào $L$ và tập hợp các đồng cấu $K$ của $A$ vào $L$, do đó có (8).

Cuối cùng, giả sử rằng $K'$ là một mở rộng bậc hữu hạn của $K$; nếu $A'$ là một $K'$-đại số giao hoán bậc hữu hạn, thì nó cũng là một $K$-đại số giao hoán bậc hữu hạn và ta có $[A': K] = [A': K'] \cdot [K': K]$ (V. p. 10, Th. 1). Chúng tôi sẽ chứng minh công thức
$$
[A': K], = [A': K']_s \cdot [K': K], .
$$
Thật vậy, gọi $S$ (resp. $T$) là tập hợp các $K$-đồng cấu của $K'$ (resp. $A'$) vào một bao đóng đại số $L$ của $K$; với mỗi $\sigma \in S$ ta ký hiệu bởi $T_\sigma$ tập hợp các phần tử $f$ của $T$ sao cho $f(a \cdot 1) = \sigma(a)$ với mọi $a \in K'$. Khi đó họ $(T_\sigma)_\sigma$ là một phân hoạch của $T$ và ta có Card $S = [K': K]$; mặt khác với mỗi $\sigma \in S$ tập hợp $T_\sigma$ gồm các $K'$-đồng cấu của $A'$ vào mở rộng đóng đại số $(L, \sigma)$ của $K'$, do đó Card $T_\sigma = [A': K']_s$, và vì thế ta đã chứng minh được (9).

#### Mệnh đề 4 {#alg-v-s6-prop-4 .statement}

— Cho $A$ là một đại số giao hoán bậc hữu hạn trên $K$; khi đó $[A: K], \leq [A: K]$ với đẳng thức khi và chỉ khi $A$ là etale.

Cho $\Omega$ là một bao đóng đại số của $K$ và $A?$ tập hợp các đồng cấu đại số từ $A$ vào $\mathbf{R}$. Ta có Card $A? = [A: K]$, và $A$ là etale khi và chỉ khi $A$ được chéo hoá bởi mở rộng $\Omega$ của $K$ (V, p. 30, Mệnh đề 2). Do đó Mệnh đề 4 suy ra từ Hệ quả của V, p. 29.

#### Hệ quả 1 {#alg-v-s6-prop-4-cor-1 .statement}

— Cho $A, B$ là hai đại số giao hoán trên $K$, có bậc hữu hạn khác không. Khi đó, để đại số $C = A \otimes_K B$ là étale thì điều kiện cần và đủ là $A$ và $B$ đều étale.

Ta có $[C: K] = [A: K] \cdot [B: K]$ và Công thức tương ứng (7) đối với các bậc tách được. Hơn nữa ta có $[A: K], \leq [A: K]$ và các công thức tương ứng đối với $B$ và $C$. Suy ra $[C: K] = [C: K]$ khi và chỉ khi ta đồng thời có $[A: K] = [A: K]$ và $[B: K] = [B: K]$; bây giờ chỉ cần áp dụng Mệnh đề 4.

#### Hệ quả 2 {#alg-v-s6-prop-4-cor-2 .statement}

— Cho $K'$ là một mở rộng của $K$.

a) Điều kiện cần và đủ để một $K$-đại số $A$ là étale là $K'$-đại số $A_{(K')}$ là étale.

b) Cho $A'$ là một đại số trên $K'$, không thu về 0. Điều kiện cần và đủ để $A'$ là étale trên $K$ là $A'$ là étale trên $K'$ và $K'$ étale trên $K$.

Ta lập luận như đối với Hệ quả 1, lần này áp dụng (8) cho $a)$ và (9) cho $b)$.

### 6. Đặc trưng hóa vi phân của các đại số étale

#### Định lý 3 {#alg-v-s6-thm-3 .statement}

— Cho $ A $ là một đại số giao hoán bậc hữu hạn trên $ K $. Để $ A $ là etale, điều kiện cần và đủ là môđun $ \Omega_K(A) $ các $ K $-vi phân của $ A $ được thu về $ 0 $.

$ A) $ Cho $ L $ là một bao đóng đại số của $ K $ ($ V $, p. 23, Định lý 2). Để $ A $ là étale thì điều kiện cần và đủ là đại số $ A_{(L)} $ trên $ L $ phải chéo hóa được ($ V $, p. 30, Mệnh đề 2). Hơn nữa, $ A $-môđun $ \Omega_L(A_{(L)}) $ đẳng cấu với $ \Omega_K(A) \otimes_A A_{(L)} $ (III, p. 572, Mệnh đề 20), do đó đẳng cấu với $ \Omega_K(A) \otimes_K L $, theo tính kết hợp của tích tenxơ; vì thế $ \Omega_K(A) = 0 $ là tương đương với $ \Omega_L(A_{(L)}) = 0 $. Vậy để chứng minh Định lý 3, do đó chỉ cần xét trường hợp $ K $ đóng đại số và chỉ ra rằng đại số $ A $ chéo hóa được khi và chỉ khi $ \Omega_K(A) = 0 $.

$ B) $ Giả sử rằng $ A $ chéo hóa được; khi đó ($ V $, p. 29, Mệnh đề 1), không gian vectơ $ A $ được sinh bởi các phần tử lũy đẳng của $ A $. Mệnh đề $ \Omega_K(A) = 0 $ vì thế là một hệ quả của bổ đề sau:

#### Bổ đề 2 {#alg-v-s6-lem-2 .statement}

— Cho $ A $ là một đại số giao hoán trên $ K $ và $ e $ là một phần tử lũy đẳng của $ A $; khi đó ta có $ de = 0 $ trong $ \Omega_K(A) $.

Từ quan hệ $ e = e^2 $ suy ra $ de = 2e \cdot de $; nhân với $ e $ ta được $ e \cdot de = 2e \cdot de $, do đó $ e \cdot de = 0 $, và cuối cùng, $ de = 2e \cdot de = 0 $.

$ C) $ Trước hết ta chứng minh hai bổ đề:

#### Bổ đề 3 {#alg-v-s6-lem-3 .statement}

— Cho $ A $ là một đại số giao hoán bậc hữu hạn trên trường đóng đại số $ K $, sao cho $ \Omega_K(A) = 0 $. Khi đó ta có $ m = m^2 $ với mọi iđêan cực đại $ m $ của $ A $.

Đại số $ A/m $ là một mở rộng bậc hữu hạn của trường đóng đại số $ K $, do đó $[A/m : K] = 1$. Vì thế với mỗi $ a \in A $ tồn tại một vô hướng duy nhất $ \lambda $ sao cho $ a - \lambda \cdot 1 \in m $; ký hiệu $ D(a) $ là lớp thặng dư của $ a - \lambda \cdot 1 $ modulo $ m^2 $. Hiển nhiên $ D $ là một $ K $-đạo hàm của $ A $ vào $ A $-môđun $ m/m^2 $. Tính chất phổ quát của $ \Omega_K(A) $ (III, p. 569) và giả thiết $ \Omega_K(A) = 0 $ nay suy ra $ D = 0 $, do đó $ m/m^2 = 0 $ và vì vậy $ m = m^2 $.

#### Bổ đề 4 {#alg-v-s6-lem-4 .statement}

— Cho $ A $ là một vành giao hoán và $ a $ là một iđêan sinh hữu hạn của $ A $ sao cho $ a = a^2 $. Khi đó tồn tại một phần tử lũy đẳng $ e $ trong $ A $ sao cho $ a = Ae $.

Cho $ (a,, ..., a,) $ là một hệ sinh của iđêan $ a $; vì $ a = a^2 $, tồn tại các phần tử $ x_{ij} $ trong $ a $ sao cho $ a_i = \sum_{j=1}^r x_{ij} a_j $ với $ 1 \leq i \leq r $. Ký hiệu $ M $ là ma trận bình phương cấp $ r $ có các phần tử là $ \delta_{ij} - x_{ij} $ và gọi $ D $ là định thức của nó. Tồn tại (III, p. 532, Công thức (26)) một ma trận bình phương $ N $ cấp $ r $ có các phần tử trong $ A $ sao cho $ N \cdot M = D \cdot I $, do đó ngay lập tức $ Da_j = 0 $ với $ 1 \leq j \leq r $ và vì vậy sau cùng $ Da = 0 $. Bây giờ ma trận $ M $ đồng dư với $ I $, mod $ a $, nên $ D \equiv I $ mod $ a $. Đặt $ e = 1 - D $; khi đó $ e \in a $ và $ ex = x $ với mọi $ x \in a $. Suy ra $ e $ là một phần tử lũy đẳng và $ a $ bằng $ Ae $.

Sau khi đã thiết lập các bổ đề này, hãy chứng minh bằng quy nạp theo bậc của $ A $ rằng $ A $ chéo hóa được nếu $ K $ đóng đại số và $ \Omega_K(A) = 0 $. Gọi $ m $ là một iđêan cực đại của $ A $ (I, p. 104). Theo Bổ đề 3 và 4, tồn tại một phần tử lũy đẳng $ e $ sao cho $ m = Ae $; ta đã thấy rằng $ A/m $ có bậc 1 trên $ K $. Do đó $ A $ là tổng trực tiếp của các iđêan $ a = (1 - e)A $ và $ m $ và ta có $ [a : K] = 1 $, suy ra $ A $ đẳng cấu với $ K \times A/a $. Vì $ \Omega_K(A/a) $ đẳng cấu với một thương của $ \Omega_K(A) $ (III, p. 573, Mệnh đề 22), nên nó bằng không và giả thiết quy nạp cho thấy rằng $ A/a $ chéo hóa được. Điều này suy ra rằng $ A $ chéo hóa được.

### 7. Đại số rút gọn và đại số étale

#### Định nghĩa 2 {#alg-v-s6-def-2 .statement}

— *Cho $ A $ là một vành giao hoán; khi đó $ A $ được gọi là rút gọn nếu mọi phần tử lũy linh (I, p. 98) của $ A $ đều bằng không.*

Nếu $ A $ là một trường, hoặc một miền nguyên, hoặc một tích của các vành rút gọn, thì nó là một vành rút gọn. Để một vành giao hoán $ A $ là rút gọn, điều kiện cần và đủ là $ a^2 \neq 0 $ với mọi $ a \neq 0 $ trong $ A $: thật vậy, từ đó suy ra bằng quy nạp theo $ n $ rằng $ a^{2^n} \neq 0 $, do đó $ a^n \neq 0 $ với mọi $ a \neq 0 $ trong $ A $.

Một đại số được gọi là *rút gọn* nếu vành nền của nó là rút gọn.

#### Mệnh đề 5 {#alg-v-s6-prop-5 .statement}

— *Cho $ A $ là một đại số giao hoán bậc hữu hạn trên $ K $. Để $ A $ là rút gọn, điều kiện cần và đủ là tồn tại các mở rộng $ L_1, \ldots, L_s $ bậc hữu hạn trên $ K $ sao cho $ A $ đẳng cấu trên $ K $ với $ L_1 \times \cdots \times L_s $.*

Điều kiện đã nêu rõ ràng là đủ.

Ngược lại, giả sử rằng $ A $ là rút gọn; lập luận bằng quy nạp theo bậc của $ A $ ta thấy rằng chỉ cần chứng minh rằng nếu $ A $ không phải là một trường, thì tồn tại hai đại số khác không $ A_1 $ và $ A_2 $ sao cho $ A $ đẳng cấu với $ A_1 \times A_2 $, hay cũng vậy, rằng tồn tại trong $ A $ một phần tử lũy đẳng khác 0 và 1.

Giả sử từ nay về sau $ A $ là rút gọn và không phải là một trường. Trong các iđêan của $ A $ khác 0 và $ A $, lấy $ a $ là một iđêan có chiều như một không gian vectơ $ K $ là cực tiểu. Với mọi $ x \neq 0 $ trong $ a $ ta có $ x^2 \neq 0 $, vì $ A $ là rút gọn, do đó $ a' \neq \{0\} $. Ta có $ a^2 \subset a $ và theo tính cực tiểu của $ a $ suy ra $ a' = a $. Theo Bổ đề 4 tồn tại một phần tử lũy đẳng $ e $ sao cho $ a = Ae $, và ta có $ e \neq 0, e \neq 1 $ vì $ a $ phân biệt với 0 và $ A $.

#### Định lý 4 {#alg-v-s6-thm-4 .statement}

— *Cho $ A $ là một đại số giao hoán bậc hữu hạn trên $ K $. Khi đó các mệnh đề sau là tương đương:
a) Đại số $ A $ là étale.
b) Với mọi mở rộng $ L $ của $ K $, vành $ L \otimes_K A $ là rút gọn.
c) Tồn tại một trường mở rộng hoàn hảo $ P $ của $ K $ sao cho vành $ P \otimes_K A $ là rút gọn.
d) Tồn tại các mở rộng đại số tách được $ L_1, \ldots, L_s $ của $ K $ sao cho $ A $ đẳng cấu với $ L_1 \times \cdots \times L_s $.*
Đặc biệt, mọi đại số étale đều là rút gọn.

A) Trước hết, ta hãy chứng minh tính tương đương của $a$, $b$ và $c$.

Giả sử rằng $A$ là étale và cho $L$ là một mở rộng của $K$. Gọi $\Omega$ là một trường mở rộng đóng đại số của $L$ (V, p. 23, Th. 2). Khi đó $L \otimes_K A$ đẳng cấu với một vành con của $\Omega \otimes_K A$ và vành sau đẳng cấu với một vành $\Omega^n$ theo Prop. 2 (V, p. 30). Do đó vành $L \otimes_K A$ là rút gọn.

Như vậy ta đã chỉ ra rằng $a)$ suy ra $b)$, và $c)$ là một trường hợp riêng của $b)$. Bây giờ giả sử rằng $c)$ đúng. Để K-đại số $A$ là etale, điều kiện cần và đủ là P-đại số $A_{(P)}$ là etale (V, p. 32, Hệ quả 2). Do đó đại số $A$ là etale theo bổ đề sau:

#### Bổ đề 5 {#alg-v-s6-lem-5 .statement}

*Cho B là một đại số rút gọn bậc hữu hạn trên một trường hoàn hảo P; khi đó B là etale.*

Theo Mệnh đề 5 tồn tại các mở rộng $L_1, \ldots, L_n$ của $P$ sao cho $B$ đẳng cấu với đại số $L, x \ldots x L_n$. Vì một tích hữu hạn của các đại số etale là etale (V, p. 31, Hệ quả) nên chỉ cần xét trường hợp $B$ là một mở rộng của $P$. Theo Định lý 3 (V, p. 33) chỉ cần chứng minh rằng $dx = 0$ trong $\Omega_P(B)$ với mọi $x \in B$.

Cho $x \in B$; vì $B$ có bậc hữu hạn trên $K$, $x$ là đại số trên $K$ (V, p. 18, Mệnh đề 2). Gọi $f$ là đa thức tối tiểu của $x$ và gọi $f'$ là đạo hàm của f. Đa thức $f$ không hằng. Giả sử rằng $f' = 0$; theo V, p. 9, Hệ quả thì trường $P$ có đặc số $p \neq 0$ và ta có $f \in P[X^p]$; vì $P$ là hoàn hảo, ta có $P[X^p] = P[X]^p$, nhưng đa thức bất khả quy $f$ không thể nằm trong $P[X]^p$.

Do đó ta có $f' \neq 0$ và vì bậc của $f'$ nhỏ hơn hẳn bậc của f, nên ta có $f'(x) \neq 0$. Bây giờ từ $f(x) = 0$ ta suy ra $f(x) \cdot dx = 0$ trong $\Omega_P(B)$, do đó $dx = 0$, như phải chứng minh.

*B) Giả sử rằng $A$ là étale; theo tính tương đương của $a)$ và $b)$ thì đại số $A$ là rút gọn, do đó tồn tại các mở rộng $L_1, \ldots, L_n$ của $K$ sao cho $A$ đẳng cấu với $L_1 \times \cdots \times L_n$ (Mệnh đề 5). Vì $A$ là étale, mỗi mở rộng $L_i$ là một đại số étale (V, p. 31, Hệ quả), và vì thế theo định nghĩa là một mở rộng đại số tách được của $K$.

Hệ quả $d) \Rightarrow a)$ suy ra từ V, p. 31, Hệ quả. \*

#### Hệ quả {#alg-v-s6-n7-cor-1 .statement}

— *Giả sử rằng $K$ có đặc số $p \neq 0$. Để $A$ là etale, điều kiện cần và đủ là $A = K[A^p]$. Khi đó, với mọi cơ sở $(a_i)_i$ của $A$ trên $K$, họ $(a_i^p)_i$ là một cơ sở của $A$ trên $K$.*

Hãy chọn một bao đóng đại số $\Omega$ của $K$. Cho hai $K$-đồng cấu $u$ và $v$ của $A$ vào $\Omega$, nếu $u$ và $v$ có cùng hạn chế trên $K[A^p]$, ta có

$$
u(x)^p = u(x^p) = v(x^p) = v(x)^p,
$$

do đó $u(x) = v(x)$

với mọi $x \in A$. Như vậy ta có bất đẳng thức $[A : K], \leq [K[A^p] : K]_s$; nếu $A$ là étale, do đó ta có

$$
[A : K] = [A : K]_s \leq [K[A^p] : K]_s \leq [K[A^p] : K],
$$

do đó $A = K[A^p]$

Ngược lại, giả sử rằng ta có $ A = K[A^p] $; gọi $ (a_i)_{i \in I} $ là một cơ sở của $ A $ trên $ K $. Theo $ V $, p. 4, Prop. 2, b), họ $ (a_i^p)_{i \in I} $ sinh ra không gian vectơ $ K $ $ K[A^p] $, và vì $ A = K[A^p] $ có số chiều hữu hạn bằng lực lượng của $ I $, họ $ (a_i^p)_{i \in I} $ là một cơ sở của $ A $ trên $ K $. Gọi $ u $ là một phần tử của $ \Omega \otimes_K A $ sao cho $ u^2 = 0 $, do đó $ u^p = 0 $; vì $ (a_i)_{i \in I} $ là một cơ sở của $ A $ trên $ K $, tồn tại một họ $ (\lambda_i)_{i \in I} $ các phần tử của $ \Omega $ sao cho $ u = \sum_{i \in I} \lambda_i \otimes a_i $, do đó $ u^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p $. Vì $ (a_i^p)_{i \in I} $ là một cơ sở của $ A $ trên $ K $ và $ u^p = 0 $, ta phải có $ \lambda_i^p = 0 $, do đó $ \lambda_i = 0 $ với mọi $ i \in I $, và vì thế $ u = 0 $. Điều này cho thấy vành $ \Omega \otimes_K A $ là rút gọn; vì $ \Omega $ là hoàn hảo, đại số $ A $ trên $ K $ là étale theo Định lý 4.

Để có một đặc trưng hóa khác của các đại số étale, xem $ V $, p. 48, Mệnh đề 1.

### Bài tập {#alg-v-s6-exercises}

Xem [bài tập của § 6](exercises/s6/).
