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
content_sha256: f5bbf6025d97ce624809dc360e0715f868a87c03e3884ea9dfca7ccbb9f6f1a8
translated_from: content/en/alg/V/06_s6_etale_algebras.md
source_content_sha256: 863fd69f4b466e7c901a8b089c5a10ba6ecad623ef3ce2dfc09bc3e6ab33fc75
translation_model: gpt-5-6-mini
translation_run: translate-vi-1025ba98
glossary_version: 34
glossary_terms_sha256: 3592a12f8526cc690d835d3e9c257b52c4d60c679e2831e9928b5713568599f7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. ĐẠI SỐ ÉTALE

Trong toàn bộ đoạn này K ký hiệu một trường.

### 1. Tính độc lập tuyến tính của các đồng cấu

Cho L là một mở rộng của K và V là một không gian vectơ trên K. Trong đoạn này ta sẽ ký hiệu bởi $ \operatorname{Hom}_K(V, L) $ tập hợp tất cả các ánh xạ K-tuyến tính từ V vào L, được trang bị cấu trúc không gian vectơ trên L sao cho:

(1) $$(f + g)(x) = f(x) + g(x)\,,\quad (\alpha f)(x) = \alpha f(x)$$

với $x \in V,\ a \in L$ và $f,\ g$ thuộc $\mathrm{Hom}_K(V, L)$. Cho $V_{(L)} = L \otimes_K V$ là không gian vectơ trên L dẫn xuất từ V bằng mở rộng vô hướng, và $(V_{(L)})^*$ là đối ngẫu của nó. Theo II, p. 277 ta có một đẳng cấu chính tắc $u \mapsto 3$ của các không gian vectơ L từ $(V_{(L)})^*$ lên $\mathrm{Hom}_K(V, L)$ sao cho $\tilde{u}(x) = u(1 \otimes x)$ với $x \in V$ và $u$ thuộc $(V_{(L)})^*$. Nếu V có chiều *hữu hạn* $n$ trên $K$, không gian vectơ $(V_{(L)})$ trên $L$ có chiều $n$, cũng như đối ngẫu của nó $(V_{(L)})^* = V_{(\bar{L})}^*$, do đó có công thức

(2) $$[\mathrm{Hom}_K(V, L) : L] = [V : K]$$

#### Định lý 1 {#alg-v-s6-thm-1 .statement}

— *Cho L là một mở rộng của một trường K và A là một đại số trên K; cho $\mathcal{H}$ là tập hợp tất cả các đồng cấu đại số K từ A vào L. Khi đó $\mathcal{H}$ là một tập con tự do của không gian vectơ $\mathrm{Hom}_K(A, L)$ trên L.*

Ta hãy chứng minh bằng quy nạp theo số nguyên $n \geq 0$ rằng mọi dãy $(u_1, \ldots, u_n)$ gồm các phần tử phân biệt của $\mathcal{H}$ là tự do. Trường hợp $n = 0$ là tầm thường, từ nay ta có thể giả sử rằng $n \geq 1$; cho $a_1, \ldots, a_n$ là các phần tử của L sao cho $$\sum_{i=1}^n \alpha_i u_i = 0.$$ Với $x,\ y$ trong A ta có
$$
\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i(y) = \sum_{i=1}^n \alpha_i u_i(xy) - u_n(x) \sum_{i=1}^n \alpha_i u_i(y) = 0,
$$
do đó $$\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i = 0.$$ Theo giả thiết quy nạp, các phần tử $u_1, \ldots, u_{n-1}$ của $\mathcal{H}$ độc lập tuyến tính, do đó $\alpha_i [u_i(x) - u_n(x)] = 0$ với $1 \leq i \leq n-1$ và với mọi $x$ trong A. Vì các $u_i$ phân biệt, điều này suy ra rằng $\alpha_i = 0$ với $i \neq n$, do đó $\alpha_n u_n = 0$ và vì thế $\alpha_n = \alpha_n u_n(1) = 0$ (với 1 ký hiệu phần tử đơn vị của A). Như vậy ta đã chỉ ra rằng $a_1, \ldots, a_{n-1}, \alpha_n$ bằng không, và điều này chứng minh định lý.

#### Hệ quả 1 {#alg-v-s6-thm-1-cor-1 .statement}

— *Cho $\Gamma$ là một nửa nhóm, L là một trường và X là một tập hợp các đồng cấu của $\Gamma$ vào nửa nhóm nhân của L. Khi đó X là một tập con tự do của không gian L-vectơ $L^\Gamma$ gồm các ánh xạ từ $\Gamma$ vào L.*

Cho A là đại số của nửa nhóm $\Gamma$ với các hệ số trong L và $(e,)_{\gamma}$, cơ sở chính tắc của A trên L (III, p. 446). Với mọi ánh xạ L-tuyến tính $u$ từ A vào L, ta viết $\tilde{u}(\gamma) = u(e,\gamma)$ (với $\gamma \in \Gamma$); khi đó ánh xạ $u \mapsto 3$ là một đẳng cấu của các không gian L-vectơ của $\mathrm{Hom}_L(A, L)$ lên $L^\Gamma$ ánh xạ lên X tập hợp các đồng cấu đại số L từ A vào L. Bây giờ chỉ cần áp dụng Đl. 1 với $K = L$.

**HỆ QUẢ 2** (định lý Dedekind). — *Cho E và L là hai mở rộng của K. Tập hợp các K-đồng cấu từ E vào L là tự do trên L. Nếu E có bậc hữu hạn trên K, số các K-đồng cấu từ E vào L nhiều nhất bằng $[E : K]$.*

Khẳng định cuối cùng suy ra từ khẳng định thứ nhất, có tính đến Công thức (2).

### 2. Tính độc lập đại số của các đồng cấu

#### Định lý 2 {#alg-v-s6-thm-2 .statement}

— Cho K là một trường vô hạn, L là một mở rộng của K và A là một đại số trên K. Cho $ u_1, \ldots, u_n $ là các đồng cấu đại số trên K phân biệt từ A vào L và f là một đa thức trong $ L[X_1, \ldots, X_j] $. Nếu ta có $ f(u_1(x), \ldots, u_n(x)) = 0 $ với mọi $ x \in A $, thì $ f = 0 $.

Gọi B là tập hợp các phần tử của $ L^n $ có dạng $ (u_1(x), \ldots, u_n(x)) $ với $ x \in A $. Theo Định lý 1, không có dãy $ (a,, \ldots, a,) $ các phần tử không phải tất cả đều bằng không trong L sao cho $ \sum_{i=1}^n \alpha_i u_i(x) = 0 $ với mọi $ x \in A $; do đó (II, p. 301, Định lý 7) B sinh không gian vectơ $ L^n $ trên L. Vì vậy tồn tại các phần tử $ a,, \ldots, a, $ của A sao cho ma trận $ (u_i(a_j))_{1 \leq i,j \leq n} $ là khả nghịch.

Ta định nghĩa đa thức $ g \in L[Y_1, \ldots, Y_n] $ bởi
$$
g(Y_1, \ldots, Y_n) = f \left( \sum_{j=1}^n u_1(a_j) Y_j, \ldots, \sum_{j=1}^n u_n(a_j) Y_j \right).
$$
Cho $ y_1, \ldots, y, $ thuộc K; viết $ x = \sum_{i=1}^n y_i a_i $, ta có
$$
g(y_1, \ldots, y_n) = f(u_1(x), \ldots, u_n(x)),
$$
do đó $ g(y_1, \ldots, y_n) = 0 $
theo giả thiết về $ f $. Vì trường $ K $ là vô hạn, ta có $ g = 0 $ (IV, p. 18, Hệ quả 2); khi đó ma trận $ (u_i(a_j)) $ có nghịch đảo $ (b_{ij}) $ và ta có
$$
f(X_1, \ldots, X_n) = g \left( \sum_{j=1}^n b_{1j} X_j, \ldots, \sum_{j=1}^n b_{nj} X_j \right),
$$
do đó $ f = 0 $.

Định lý 2 không có tương tự cho các trường hữu hạn. Vì vậy hãy cho $ K $ là một trường hữu hạn có q phần tử, $ A = L = K $ và $ f(X) = X^q - X $. Ta có $ x^q = x $ với mọi $ x \in K $ (V, p. 93, Mệnh đề 2); do đó nếu $ u $ là tự đẳng cấu đồng nhất của $ K $, ta có $ f(u(x)) = 0 $ với mọi $ x \in K $, mặc dù $ f $ không bằng không.

### 3. Các đại số chéo hóa được và các đại số etale

#### Định nghĩa 1 {#alg-v-s6-def-1 .statement}

— Cho A là một đại số trên K; khi đó A được gọi là chéo hóa được nếu tồn tại một số nguyên $ n \geq 0 $ sao cho A đẳng cấu với đại số tích $ K^n $. Ta nói rằng A được chéo hóa bởi một mở rộng L của K nếu đại số $ A_{(L)} $ trên L dẫn xuất từ A bởi mở rộng các vô hướng là chéo hóa được. Ta nói rằng A là etale nếu tồn tại một mở rộng của K chéo hóa A.

Ta nhắc lại rằng đại số tích $ K'' $ là không gian vectơ $ K'' $ được trang bị với tích được định nghĩa bởi

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

*Cho A là một đại số bậc hữu hạn n trên trường K; khi đó các điều kiện sau là tương đương:*
  *a)* *Đại số A là chéo hóa được.*
  *b)* *Có một cơ sở $ (e_1, \ldots, e_n) $ của A sao cho $ e_i^2 = e_i $ và $ e_i e_j = 0 $ với $ i \neq j $.*
  *c)* *Các đồng cấu đại số trên K của A vào $ \mathbf{K} $ sinh đối ngẫu của không gian K-vectơ A.*
  *d)* *Mọi A-môđun là một tổng trực tiếp của các môđun con có chiều 1 trên K.*

Sự tương đương của *a)* và *b)* suy ra từ Công thức (6); mặt khác, n phép chiếu $ K^n \to K $ là các đồng cấu đại số, do đó *a)* suy ra *c)*. Nếu *c)* đúng, các đồng cấu đại số của A vào $ \mathbf{K} $ tạo thành một cơ sở của đối ngẫu của A (*V*, p. 27, Định lý 1), ta ký hiệu chúng bởi $ u_1, \ldots, u_n $; khi đó $ a \mapsto (u_i(a)) $ là một đẳng cấu của A lên đại số $ K'' $, do đó *a)*. Như vậy ta đã thiết lập được sự tương đương của các điều kiện *a)*, *b)* và *c)*.

Giả sử *b)* đúng và M là một A-môđun; khi đó các phép vị tự $ (e_i)_M $ có tỉ số $ e_i $ là các phép chiếu của $ M $, và $ M $ là một tổng trực tiếp của các $ e_i M $, là các môđun con-A. Do đó ta có thể giả sử rằng tồn tại một chỉ số $ i $ sao cho $ (e_j)_M = 0 $ với $ j \neq i $. Vậy mọi không gian con vectơ của $ M $ đều là một môđun con-A, do đó *d)*.

Ngược lại, giả sử *d)* đúng và xét A-môđun A,. Khi đó tồn tại một cơ sở $ (f_i) $ của không gian vectơ K A sao cho $ Af_i = Kf_i $ với $ i = 1, \ldots, n $. Sau khi thay thế mỗi $ f_i $ bởi một bội vô hướng thích hợp, nếu cần, ta có thể giả sử rằng $ 1 = f_i + \ldots + f_n $. Nếu $ i \neq j $, thì $ f_i f_j $ thuộc $ Af_i \cap Af_j = Kf_i \cap Kf_j $ do đó nó bằng không. Bây giờ $ f_i = f_i f_1 + \ldots + f_i f_n = f_i^2 $, do đó *b)*.

#### Hệ quả {#alg-v-s6-n3-cor-1 .statement}

*Cho L là một mở rộng của K và $ \mathcal{H} $ là tập hợp các đồng cấu đại số của A vào L. Ta có Card $ \mathcal{H} \leq [A : K] $, với đẳng thức xảy ra khi và chỉ khi A được chéo hóa bởi L. Nếu A được chéo hóa bởi L, thì $ \mathcal{H} $ là một cơ sở của không gian L-vectơ $ \mathrm{Hom}_K(A, L) $.*

Không gian vectơ $ \mathrm{Hom}_K(A, L) $ trên L có chiều $ [A : K] $, theo Công thức (2), và $ \mathcal{H} $ là một tập con tự do của $ \mathrm{Hom}_K(A, L) $ theo Định lý 1 (*V*, p. 27). Do đó ta có Card $ \mathcal{H} \leq [A : K] $ với đẳng thức xảy ra khi và chỉ khi $ \mathcal{H} $ là một cơ sở của $ \mathrm{Hom}_K(A, L) $. Tồn tại một đẳng cấu của các không gian L-vectơ, ký hiệu là $ \pi : \mathrm{Hom}_K(A, L) \to A_{(L)}^* $, được đặc trưng bởi $ u(x) = (\pi u)(1 \otimes x) $ với $ x \in A $, và $ \pi $ biến $ \mathcal{H} $ lên tập hợp $ \mathcal{H}_L $ các đồng cấu đại số trên L của $ A(\cdot) $ vào L. Cuối cùng, sự tương đương của $ a) $ và $ c) $ trong Mệnh đề 1 cho thấy rằng đại số $ A_{(L)} $ trên L là chéo hóa được khi và chỉ khi $ \mathcal{H}_L $ sinh không gian vectơ $ A_{(L)}^* $ trên L. Điều này hoàn tất chứng minh của Hệ quả.

#### Mệnh đề 2 {#alg-v-s6-prop-2 .statement}

— *Cho A là một đại số trên K và $ \Omega $ là một mở rộng đóng đại số của K. Các khẳng định sau là tương đương*:

$ a) $ *Đại số A là etale*.
$ b) $ *Tồn tại một mở rộng bậc hữu hạn chéo hóa được A*.
$ c) $ *Mở rộng $ \Omega $ của K chéo hóa được A*.

Giả sử A là etale. Gọi $ n $ là bậc của A trên K, gọi L là một mở rộng của K chéo hóa được A và gọi $ \mathcal{H} $ là tập hợp các đồng cấu đại số của A vào L. Theo Hệ quả của Mệnh đề 1 ta có Card $ \mathcal{H} = n $. Mặt khác, với mỗi $ u \in \mathcal{H} $, ta có $[u(A):K] \leq n$. Theo V, p. 18, Định lý 2, mở rộng con L' của L sinh bởi các ảnh của các phần tử của $ \mathcal{H} $ có bậc hữu hạn trên K. Vì tồn tại $ n $ đồng cấu phân biệt của A vào L', mở rộng L' chéo hóa được A, theo Hệ quả 1 của Mệnh đề 1. Điều này chứng tỏ rằng a) suy ra b).

Vì mọi mở rộng bậc hữu hạn của K đều đẳng cấu với một mở rộng con của $ \Omega $ (V, p. 20, Định lý 1), b) suy ra c). Cuối cùng c) rõ ràng suy ra a).

### 4. Các đại số con của một đại số etale

#### Mệnh đề 3 {#alg-v-s6-prop-3 .statement}

— *Cho A là một đại số etale trên K. Chỉ có một số hữu hạn đại số con và iđêan của A. Hơn nữa, mọi mở rộng của K chéo hóa được A cũng chéo hóa được mọi đại số con và mọi đại số thương của A; đặc biệt các đại số này là etale*.
