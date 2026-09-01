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
content_sha256: d8337b84df2ee9c22ce9d881ed6e2f4beb99fb0856ee98e94ba808e1615dc707
translated_from: content/en/alg/V/06_s6_etale_algebras.md
source_content_sha256: 1c0ff6eab8a369a6cc0ba7a81f2a00f665a45cec046137d9abeebe3c7a4842b7
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-1025ba98
glossary_version: 34
glossary_terms_sha256: 3592a12f8526cc690d835d3e9c257b52c4d60c679e2831e9928b5713568599f7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. ĐẠI SỐ ÉTALE

Trong toàn bộ đoạn này K ký hiệu một trường.

### 1. Độc lập tuyến tính của các đồng cấu

Cho L là một mở rộng của K và V là một không gian vectơ trên K. Trong đoạn này ta sẽ ký hiệu bởi $\operatorname{Hom}_K(V, L)$ tập hợp tất cả các ánh xạ K-tuyến tính từ V vào L, được trang bị cấu trúc không gian vectơ trên L sao cho:

(1) $$(f + g)(x) = f(x) + g(x)\,,\quad (\alpha f)(x) = \alpha f(x)$$

với $x \in V,\ a \in L$ và $f,\ g$ thuộc $\mathrm{Hom}_K(V, L)$. Gọi $V_{(L)} = L \otimes_K V$ là không gian vectơ trên L dẫn xuất từ V bằng mở rộng vô hướng, và $(V_{(L)})^*$ là không gian đối ngẫu của nó. Theo II, p. 277 ta có một đẳng cấu chính tắc $u \mapsto 3$ của các không gian L-vectơ từ $(V_{(L)})^*$ lên $\mathrm{Hom}_K(V, L)$ sao cho $\tilde{u}(x) = u(1 \otimes x)$ với $x \in V$ và $u$ thuộc $(V_{(L)})^*$. Nếu V có chiều *hữu hạn* $n$ trên $K$, không gian vectơ $(V_{(L)})$ trên $L$ có chiều $n$, cũng như đối ngẫu của nó $(V_{(L)})^* = V_{(\bar{L})}^*$, do đó công thức

(2) $$[\mathrm{Hom}_K(V, L) : L] = [V : K]$$

#### Định lý 1 {#alg-v-s6-thm-1 .statement}

— *Cho L là một mở rộng của một trường K và A là một đại số trên K; gọi $\mathcal{H}$ là tập hợp tất cả các đồng cấu K-đại số từ A vào L. Khi đó $\mathcal{H}$ là một tập con tự do của không gian vectơ $\mathrm{Hom}_K(A, L)$ trên L.*

Ta chứng minh bằng quy nạp theo số nguyên $n \geq 0$ rằng mọi dãy $(u_1, \ldots, u_n)$ gồm các phần tử phân biệt của $\mathcal{H}$ là tự do. Trường hợp $n = 0$ là tầm thường, do đó từ nay ta có thể giả sử rằng $n \geq 1$; cho $a_1, \ldots, a_n$ là các phần tử của L sao cho $$\sum_{i=1}^n \alpha_i u_i = 0.$$ Với $x,\ y$ thuộc A ta có
$$
\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i(y) = \sum_{i=1}^n \alpha_i u_i(xy) - u_n(x) \sum_{i=1}^n \alpha_i u_i(y) = 0,
$$
do đó $$\sum_{i=1}^{n-1} \alpha_i [u_i(x) - u_n(x)] \cdot u_i = 0.$$ Theo giả thiết quy nạp, các phần tử $u_1, \ldots, u_{n-1}$ của $\mathcal{H}$ độc lập tuyến tính, do đó $\alpha_i [u_i(x) - u_n(x)] = 0$ với $1 \leq i \leq n-1$ và với mọi $x$ thuộc A. Vì các $u_i$ phân biệt, điều này suy ra rằng $\alpha_i = 0$ với $i \neq n$, do đó $\alpha_n u_n = 0$ và vì vậy $\alpha_n = \alpha_n u_n(1) = 0$ (bằng cách ký hiệu phần tử đơn vị của A là 1). Ta đã chứng minh rằng $a_1, \ldots, a_{n-1}, \alpha_n$ đều bằng không, và điều này chứng minh định lý.

#### Hệ quả 1 {#alg-v-s6-thm-1-cor-1 .statement}

— *Cho $\Gamma$ là một nửa nhóm, L là một trường và X là một tập hợp các đồng cấu từ $\Gamma$ vào nửa nhóm nhân của L. Khi đó X là một tập con tự do của không gian L-vectơ $L^\Gamma$ gồm các ánh xạ từ $\Gamma$ vào L.*

Cho A là đại số của nửa nhóm $\Gamma$ với các hệ số trong L và $(e,)_{\gamma}$, cơ sở chính tắc của A trên L (III, p. 446). Với mỗi ánh xạ L-tuyến tính $u$ từ A vào L, ta viết $\tilde{u}(\gamma) = u(e,\gamma)$ (với $\gamma \in \Gamma$); khi đó ánh xạ $u \mapsto 3$ là một đẳng cấu của các không gian L-vectơ của $\mathrm{Hom}_L(A, L)$ lên $L^\Gamma$, ánh xạ X lên tập hợp các đồng cấu L-đại số từ A vào L. Bây giờ chỉ cần áp dụng Định lý 1 với $K = L$.

**HỆ QUẢ 2** (Định lý Dedekind). — *Cho E và L là hai mở rộng của K. Tập hợp các K-đồng cấu từ E vào L là tự do trên L. Nếu E có bậc hữu hạn trên K, số các K-đồng cấu từ E vào L nhiều nhất bằng $[E : K]$.*

Khẳng định cuối cùng suy ra từ khẳng định đầu tiên, có tính đến Công thức (2).

### 2. Độc lập đại số của các đồng cấu

#### Định lý 2 {#alg-v-s6-thm-2 .statement}

— *Cho K là một trường vô hạn, L là một mở rộng của K và A là một đại số trên K. Cho $u_1, \ldots, u_n$ là các đồng cấu K-đại số phân biệt từ A vào L và f là một đa thức trong $L[X_1, \ldots, X_n]$. Nếu ta có $f(u_1(x), \ldots, u_n(x)) = 0$ với mọi $x \in A$, thì $f = 0$.*

Cho B là tập hợp các phần tử của $L^n$ có dạng $(u_1(x), \ldots, u_n(x))$ với $x \in A$. Theo Định lý 1, không tồn tại dãy $(\alpha_1, \ldots, \alpha_n)$ gồm các phần tử không đồng thời bằng không trong L sao cho $\sum_{i=1}^n \alpha_i u_i(x) = 0$ với mọi $x \in A$; do đó (II, p. 301, Định lý 7) B sinh ra không gian vectơ $L^n$ trên L. Vậy tồn tại các phần tử $a_1, \ldots, a_n$ của $A$ sao cho ma trận $(u_i(a_j))_{1 \leq i,j \leq n}$ là khả nghịch.

Ta định nghĩa đa thức $g \in L[Y_1, \ldots, Y_n]$ bởi
$$
g(Y_1, \ldots, Y_n) = f \left( \sum_{j=1}^n u_1(a_j) Y_j, \ldots, \sum_{j=1}^n u_n(a_j) Y_j \right).
$$
Cho $y_1, \ldots, y_n$ thuộc $K$; đặt $x = \sum_{i=1}^n y_i a_i$, ta có
$$
g(y_1, \ldots, y_n) = f(u_1(x), \ldots, u_n(x)),
$$
từ đó $g(y_1, \ldots, y_n) = 0$
theo giả thiết về $f$. Vì trường $K$ là vô hạn, ta có $g = 0$ (IV, p. 18, Hệ quả 2); mặt khác ma trận $(u_i(a_j))$ có nghịch đảo $(b_{ij})$ và ta có
$$
f(X_1, \ldots, X_n) = g \left( \sum_{j=1}^n b_{1j} X_j, \ldots, \sum_{j=1}^n b_{nj} X_j \right),
$$
từ đó $f = 0$.

Định lý 2 không có tương tự cho các trường hữu hạn. Chẳng hạn cho $K$ là một trường hữu hạn có q phần tử, $A = L = K$ và $f(X) = X^q - X$. Ta có $x^q = x$ với mọi $x \in K$ (V, p. 93, Mệnh đề 2); do đó nếu $u$ là tự đẳng cấu đồng nhất của $K$, ta có $f(u(x)) = 0$ với mọi $x \in K$, mặc dù $f$ không bằng không.

### 3. Các đại số chéo hóa được và các đại số etale

#### Định nghĩa 1 {#alg-v-s6-def-1 .statement}

— Cho A là một đại số trên K; khi đó ta nói A là chéo hóa được nếu tồn tại một số nguyên $n \geq 0$ sao cho A đẳng cấu với đại số tích $K^n$. Ta nói A được chéo hóa bởi một mở rộng L của K nếu đại số $A_{(L)}$ trên L thu được từ A bằng mở rộng vô hướng là chéo hóa được. Ta sẽ nói A là etale nếu tồn tại một mở rộng của K làm chéo hóa A.

Ta nhắc lại rằng đại số tích $K''$ là không gian vectơ $K''$ được trang bị phép nhân được xác định bởi

$$
(x_1, \ldots, x_n) \cdot (y_1, \ldots, y_n) = (x_1 y_1, \ldots, x_n y_n)
$$

Nếu $\varepsilon_1, \ldots, \varepsilon_n$ là cơ sở chính tắc của $K^n$, ta có

$$
\varepsilon_i^2 = \varepsilon_i , \quad \varepsilon_i \varepsilon_j = 0 \quad \text{nếu} \quad i \neq j
$$

và $1 = \varepsilon_1 + \ldots + \varepsilon_n$.

Mọi đại số etale trên $\mathbf{K}$ đều *giao hoán* và có *bậc hữu hạn* trên $K$.

#### Mệnh đề 1 {#alg-v-s6-prop-1 .statement}

*Cho A là một đại số bậc hữu hạn n trên trường K ; khi đó các điều kiện sau là tương đương :*
  *a)* *Đại số A là chéo hóa được.*
  *b)* *Tồn tại một cơ sở $(e_1, \ldots, e_n)$ của A sao cho $e_i^2 = e_i$ và $e_i e_j = 0$ với $i \neq j$.*
  *c)* *Các đồng cấu K-đại số của A vào $\mathbf{K}$ sinh đối ngẫu của không gian vectơ A trên K.*
  *d)* *Mọi A-môđun đều là tổng trực tiếp của các môđun con có chiều 1 trên K.*

Sự tương đương của *a)* và *b)* suy ra từ Công thức (6); mặt khác n phép chiếu $K^n \to K$ là các đồng cấu đại số, do đó *a)* suy ra *c)*. Nếu *c)* đúng, thì các đồng cấu đại số của A vào $\mathbf{K}$ tạo thành một cơ sở của không gian đối ngẫu của A (*V*, p. 27, Định lý 1), ta ký hiệu chúng bởi $u_1, \ldots, u_n$; khi đó $a \mapsto (u_i(a))$ là một đẳng cấu của A onto đại số $K''$, suy ra *a)*. Vậy ta đã thiết lập được sự tương đương của các điều kiện *a)*, *b)* và *c)*.

Giả sử *b)* đúng và cho M là một A-môđun; khi đó các phép vị tự $(e_i)_M$ có tỉ số $e_i$ là các phép chiếu của M, và M là một tổng trực tiếp của các $e_i M$, là các A-môđun con. Do đó ta có thể giả sử rằng tồn tại một chỉ số $i$ sao cho $(e_j)_M = 0$ với $j \neq i$. Suy ra mọi không gian con vectơ của M đều là một A-môđun con, do đó *d)*.

Ngược lại, giả sử *d)* đúng và xét A-môđun A,. Khi đó tồn tại một cơ sở $(f_i)$ của không gian K-vectơ A sao cho $Af_i = Kf_i$ với $i = 1, \ldots, n$. Sau khi thay thế mỗi $f_i$ bởi một bội vô hướng thích hợp, nếu cần, ta có thể giả sử rằng $1 = f_i + \ldots + f_n$. Nếu $i \neq j$, thì $f_i f_j$ thuộc $Af_i \cap Af_j = Kf_i \cap Kf_j$ do đó nó bằng không. Bây giờ $f_i = f_i f_1 + \ldots + f_i f_n = f_i^2$, suy ra *b)*.

#### Hệ quả {#alg-v-s6-n3-cor-1 .statement}

*Cho L là một mở rộng của K và $\mathcal{H}$ là tập các đồng cấu đại số của A vào L. Ta có Card $\mathcal{H} \leq [A : K]$, với đẳng thức khi và chỉ khi A được L chéo hóa. Nếu A được L chéo hóa, thì $\mathcal{H}$ là một cơ sở của không gian L-vectơ $\mathrm{Hom}_K(A, L)$.*

Không gian vectơ $\mathrm{Hom}_K(A, L)$ trên L có chiều $[A : K]$, theo Công thức (2), và $\mathcal{H}$ là một tập con tự do của $\mathrm{Hom}_K(A, L)$ theo Định lý 1 (*V*, p. 27). Do đó ta có Card $\mathcal{H} \leq [A : K]$ với đẳng thức khi và chỉ khi $\mathcal{H}$ là một cơ sở của $\mathrm{Hom}_K(A, L)$. Tồn tại một đẳng cấu của các không gian L-vectơ, ký hiệu là $\pi : \mathrm{Hom}_K(A, L) \to A_{(L)}^*$, được đặc trưng bởi $u(x) = (\pi u)(1 \otimes x)$ với $x \in A$, và $\pi$ ánh xạ $\mathcal{H}$ lên tập $\mathcal{H}_L$ gồm các đồng cấu đại số L của $A(\cdot)$ vào L. Cuối cùng, sự tương đương của a) và c) trong Mệnh đề 1 cho thấy đại số $A_{(L)}$ trên L chéo hóa được khi và chỉ khi $\mathcal{H}_L$ sinh ra không gian vectơ $A_{(L)}^*$ trên L. Điều này hoàn tất chứng minh của Hệ quả.

#### Mệnh đề 2 {#alg-v-s6-prop-2 .statement}

— *Cho A là một đại số trên K và $\Omega$ là một mở rộng đóng đại số của K. Các mệnh đề sau là tương đương*:

a) *Đại số A là etale*.
b) *Tồn tại một mở rộng bậc hữu hạn chéo hóa A*.
c) *Mở rộng $\Omega$ của K chéo hóa A*.

Giả sử A là etale. Gọi $n$ là bậc của A trên K, gọi L là một mở rộng của K chéo hóa A và gọi $\mathcal{H}$ là tập các đồng cấu đại số của A vào L. Theo Hệ quả của Mệnh đề 1 ta có Card $\mathcal{H} = n$. Mặt khác, với mỗi $u \in \mathcal{H}$, ta có $[u(A):K] \leq n$. Theo V, p. 18, Định lý 2, mở rộng con L' của L được sinh bởi các ảnh của các phần tử của $\mathcal{H}$ có bậc hữu hạn trên K. Vì tồn tại $n$ đồng cấu phân biệt của A vào L', nên mở rộng L' chéo hóa A, theo Hệ quả 1 của Mệnh đề 1. Điều này cho thấy a) suy ra b).

Vì mọi mở rộng bậc hữu hạn của K đều đẳng cấu với một mở rộng con của $\Omega$ (V, p. 20, Định lý 1), nên b) suy ra c). Cuối cùng c) rõ ràng suy ra a).

### 4. Các đại số con của một đại số etale

#### Mệnh đề 3 {#alg-v-s6-prop-3 .statement}

— *Cho A là một đại số etale trên K. Chỉ có hữu hạn số đại số con và iđêan của A. Hơn nữa, mọi mở rộng của K chéo hóa A cũng chéo hóa mọi đại số con và mọi đại số thương của A; đặc biệt, các đại số này là etale*.

Chỉ cần chứng minh rằng một đại số $K^n$ chỉ có hữu hạn nhiều đại số con và iđêan, và rằng các đại số con và các đại số thương của $K^n$ là chéo hóa được. Ta ký hiệu $(\varepsilon_1, \ldots, \varepsilon_n)$ là cơ sở chính tắc của $K^n$.

Cho A là một đại số con của $K^n$ và cho $v_1, \ldots, v_n$ là các hạn chế lên A của n phép chiếu $K^n \to K$. Vì giao của các hạt nhân của các $v_i$ rõ ràng bằng 0, nên các $v_i$ sinh ra không gian $K$-vectơ đối ngẫu của A (II, p. 302, Hệ quả 1); do đó A là một đại số trên $K$ chéo hóa được (V, p. 29, Mệnh đề 1).

Với mọi tập con I của $\{1, 2, \ldots, n\}$, đặt $\varepsilon_I = \sum_{i \in I} \varepsilon_i$. Rõ ràng các phần tử $\varepsilon_I$ là các phần tử luỹ đẳng của $K^n$; ta có $\varepsilon_I = 0$ khi và chỉ khi I là rỗng, và $\varepsilon_I \varepsilon_J = \varepsilon_{I \cap J}$. Theo những gì đã nói, mọi đại số con A của $K^n$ đều chéo hóa được; bởi điều kiện b) của Mệnh đề 1 mọi đại số con A của $K^n$ do đó thừa nhận một cơ sở $(\varepsilon_{I_1}, \ldots, \varepsilon_{I_p})$, trong đó $(I_1, \ldots, I_p)$ là một phân hoạch của $\{1, 2, \ldots, n\}$, và chỉ có hữu hạn nhiều đại số con như vậy.

Với mọi tập con I của $(1, 2, \ldots, n)$, hãy để $a_i$ là không gian con vectơ của $K^n$ có cơ sở là các phần tử luỹ đẳng $\varepsilon_i$ với $i \in I$; khi đó rõ ràng $a_i$ là một iđêan của $K^n$; hơn nữa nếu $J = (1, 2, \ldots, n) - I$, thì các lớp thặng dư $\overline{\varepsilon}_j$ của $\varepsilon_j$ modulo $a_i$, với $j \in J$, lập thành một cơ sở của $K^n / a_i$. Ta có $\overline{\varepsilon}_j^2 = \overline{\varepsilon}_j$ và $\overline{\varepsilon}_j \overline{\varepsilon}_k = 0$ nếu $j \neq k$, do đó đại số $K^n / a_I$ là chéo hóa được, theo Mệnh đề 1 của V, p. 29.

Còn lại phải chứng minh rằng mọi iđêan của $K^n$ đều có dạng $a_I$. Gọi I là tập các số nguyên $i$ sao cho $1 \leq i \leq n$ và $\varepsilon_i \in a$, khi đó $a_i \subset a$. Cho $x = x_1 \varepsilon_1 + \cdots + x_n \varepsilon_n$ là một phần tử của a (với $x_1, \ldots, x_n$ trong $K$) và cho $i$ thuộc $(1, 2, \ldots, n) - I$. Ta có $x_i \varepsilon_i = x \varepsilon_i \in a_i$, và $\varepsilon_i \notin a$, do đó $x_i = 0$. Vậy $x = \sum_{i \in I} x_i \varepsilon_i$ và điều này cho thấy rằng $x \in a_i$. Nay ta đã chứng minh $a \subset a_I$, do đó cuối cùng $a = a_i$.

#### Hệ quả {#alg-v-s6-n4-cor-1 .statement}

— *Cho $A_1, \ldots, A_r$ là các đại số trên $K$ và $A = A_1 \times \cdots \times A_r$. Để $A$ là étale thì cần và đủ rằng $A_1, \ldots, A_r$ là étale.*

Giả sử rằng $A$ là étale; mỗi đại số $A_1, \ldots, A_r$ đẳng cấu với một đại số thương của $A$, và do đó là étale theo Mệnh đề 3. Ngược lại, mọi mở rộng của $K$ chéo hóa $A_1, \ldots, A_r$ rõ ràng cũng chéo hóa $A$.

### 5. Bậc tách được của một đại số giao hoán

Cho $A$ là một đại số giao hoán có bậc hữu hạn $n$ trên $K$. Với mọi mở rộng $L$ của $K$, số $h(L)$ các đồng cấu đại số của $A$ vào $L$ là hữu hạn và bị chặn trên bởi $n$ (V, p. 29, Hệ quả).

#### Bổ đề 1 {#alg-v-s6-lem-1 .statement}

— *Cho $\Omega$ là một bao đóng đại số của $K$; khi đó ta có $h(L) \leq h(\Omega)$ đối với mọi mở rộng $L$ của $K$, với đẳng thức khi $L$ là đóng đại số.*

Gọi $L'$ là bao đóng đại số của $K$ trong $L$. Với mọi đồng cấu $u$ của $A$ vào $L$ ta có $[u(A) : K] \leq n$, do đó $u(A) \subset L'$ theo V, p. 18, Mệnh đề 2; vì vậy ta có $h(L') = h(L)$. Vì mở rộng $L'$ của $K$ đẳng cấu với một mở rộng con của $\Omega$ (V, p. 20, Định lý 1), ta có $h(L') \leq h(\Omega)$. Nếu $L$ là đóng đại số, thì $L'$ là một bao đóng đại số của $K$; các mở rộng $L'$ và $\Omega$ của $K$ khi đó đẳng cấu với nhau (V, p. 23, Định lý 2) và do đó $h(L') = h(\Omega)$; Bổ đề suy ra trực tiếp từ điều này.

Theo Bổ đề 1, số $h(L)$ có cùng giá trị đối với mọi mở rộng đóng đại số $L$ của $K$; số này sẽ được ký hiệu là $[A : K]$, và được gọi là *bậc tách được* của $A$.

Cho $A$ và $B$ là hai đại số giao hoán có bậc hữu hạn trên $K$. Ta sẽ thiết lập công thức

$$
[A \otimes_K B : K]_s = [A : K]_s \cdot [B : K]_s .
$$

Cho $L$ là một mở rộng đóng đại số của $K$ và ký hiệu $\mathcal{H}(A)$ là tập hợp các đồng cấu đại số từ $A$ vào $L$, và tương tự định nghĩa $\mathcal{H}(B)$ và $\mathcal{H}(A \otimes_K B)$. Theo định nghĩa ta có Card $\mathcal{H}(A) = [A : K]$, và các công thức tương ứng cho [B : K], và [A \otimes_K B : K]. Hơn nữa (III, p. 465, Công thức (6)), công thức $(u * v)(a \otimes b) = u(a)v(b)$ xác định một song ánh $(u, v) \mapsto u * v$ của $\mathcal{H}(A) \times \mathcal{H}(B)$ lên $\mathcal{H}(A \otimes_K B)$, do đó Công thức (7) suy ra.

Cho $K'$ là một mở rộng của $K$; ta sẽ chứng minh công thức
$$
[A_{(K')}: K'], = [A: K], .
$$
Thật vậy, lấy $L$ là một bao đóng đại số của $K'$. Công thức $\tilde{u}(x) = u(1 \otimes x)$ (với $x \in A$) xác định một song ánh $u \mapsto \tilde{u}$ giữa tập hợp các $K'$-đồng cấu của $A_{(K')}$ vào $L$ và tập hợp các $K$-đồng cấu của $A$ vào $L$, do đó (8).

Cuối cùng, giả sử rằng $K'$ là một mở rộng bậc hữu hạn của $K$; nếu $A'$ là một đại số giao hoán $K'$ bậc hữu hạn, thì nó cũng là một đại số giao hoán $K$ bậc hữu hạn và ta có $[A': K] = [A': K'] \cdot [K': K]$ (V. p. 10, ĐL. 1). Ta sẽ chứng minh công thức
$$
[A': K], = [A': K']_s \cdot [K': K], .
$$
Cho $S$ (tương ứng $T$) là tập hợp các $K$-đồng cấu của $K'$ (tương ứng $A'$) vào một bao đóng đại số $L$ của $K$; với mọi $\sigma \in S$ ta ký hiệu $T_\sigma$ là tập hợp các phần tử $f$ của $T$ sao cho $f(a \cdot 1) = \sigma(a)$ với mọi $a \in K'$. Khi đó họ $(T_\sigma)_\sigma$ là một phân hoạch của $T$ và ta có Card $S = [K': K]$; nay với mỗi $\sigma \in S$ tập hợp $T_\sigma$ gồm các $K'$-đồng cấu của $A'$ vào mở rộng đóng đại số $(L, \sigma)$ của $K'$, do đó Card $T_\sigma = [A': K']_s$, và vì vậy ta đã chứng minh (9).

#### Mệnh đề 4 {#alg-v-s6-prop-4 .statement}

— Cho $A$ là một đại số giao hoán bậc hữu hạn trên $K$; khi đó $[A: K], \leq [A: K]$ với dấu bằng khi và chỉ khi $A$ là étale.

Cho $\Omega$ là một bao đóng đại số của $K$ và $A?$ là tập các đồng cấu đại số của $A$ vào $\mathbf{R}$. Ta có Card $A? = [A: K]$, và $A$ là étale khi và chỉ khi $A$ được chéo hóa bởi mở rộng $\Omega$ của $K$ (V, p. 30, Mệnh đề 2). Vì vậy Mệnh đề 4 suy ra từ Hệ quả của V, p. 29.

#### Hệ quả 1 {#alg-v-s6-prop-4-cor-1 .statement}

— Cho $A, B$ là hai đại số giao hoán trên $K$, có bậc hữu hạn khác 0. Khi đó, để đại số $C = A \otimes_K B$ là étale thì cần và đủ rằng $A$ và $B$ là étale.

Ta có $[C: K] = [A: K] \cdot [B: K]$ và Công thức (7) tương ứng cho các bậc tách được. Hơn nữa ta có $[A: K], \leq [A: K]$ và các công thức tương ứng cho $B$ và $C$. Suy ra rằng $[C: K] = [C: K]$, khi và chỉ khi ta có cả $[A: K] = [A: K]$ và $[B: K] = [B: K]$; lúc này chỉ cần áp dụng Mệnh đề 4.

#### Hệ quả 2 {#alg-v-s6-prop-4-cor-2 .statement}

— Cho $K'$ là một mở rộng của $K$.

a) Để một $K$-đại số $A$ là étale, điều kiện cần và đủ là $K'$-đại số $A_{(K')}$ phải là étale.

b) Cho $A'$ là một đại số trên $K'$, không rút về $0$. Để $A'$ là étale trên $K$ thì cần và đủ rằng $A'$ phải là étale trên $K'$ và $K'$ là étale trên $K$.

Ta lập luận như đối với Hệ quả 1, lần này áp dụng (8) cho a) và (9) cho b).

### 6. Đặc trưng hóa vi phân của các đại số étale

#### Định lý 3 {#alg-v-s6-thm-3 .statement}

— Cho $A$ là một đại số giao hoán có bậc hữu hạn trên $K$. Để $A$ là étale thì cần và đủ rằng môđun $\Omega_K(A)$ của các vi phân trên $K$ của $A$ phải bằng $0$.

A) Cho $L$ là một bao đóng đại số của $K$ ($V$, p. 23, Định lý 2). Để $A$ là etale thì điều kiện cần và đủ là đại số $A_{(L)}$ trên $L$ phải chéo hóa được ($V$, p. 30, Mệnh đề 2). Hơn nữa, $A$-môđun $\Omega_L(A_{(L)})$ đẳng cấu với $\Omega_K(A) \otimes_A A_{(L)}$ (III, p. 572, Mệnh đề 20), do đó đẳng cấu với $\Omega_K(A) \otimes_K L$, nhờ tính kết hợp của tích tenxơ; vì vậy $\Omega_K(A) = 0$ tương đương với $\Omega_L(A_{(L)}) = 0$. Để chứng minh Định lý 3 thì do đó đủ xét trường hợp $K$ là đóng đại số và chỉ ra rằng đại số $A$ chéo hóa được khi và chỉ khi $\Omega_K(A) = 0$.

B) Giả sử rằng $A$ là chéo hóa được; khi đó ($V$, p. 29, Mệnh đề 1), không gian vectơ $A$ được sinh bởi các lũy đẳng của $A$. Mệnh đề $\Omega_K(A) = 0$ do đó là một hệ quả của bổ đề sau:

#### Bổ đề 2 {#alg-v-s6-lem-2 .statement}

Cho $A$ là một đại số giao hoán trên $K$ và $e$ là một lũy đẳng của $A$; khi đó ta có $de = 0$ trong $\Omega_K(A)$.

Từ quan hệ $e = e^2$ ta suy ra $de = 2e \cdot de$; khi nhân với $e$ ta được $e \cdot de = 2e \cdot de$, do đó $e \cdot de = 0$, và vì thế cuối cùng, $de = 2e \cdot de = 0$.

C) Trước hết ta chứng minh hai bổ đề:

#### Bổ đề 3 {#alg-v-s6-lem-3 .statement}

Cho $A$ là một đại số giao hoán bậc hữu hạn trên trường đóng đại số $K$, sao cho $\Omega_K(A) = 0$. Khi đó ta có $m = m^2$ với mọi iđêan cực đại $m$ của $A$.

#### Bổ đề 4 {#alg-v-s6-lem-4 .statement}

Đại số $A/m$ là một mở rộng bậc hữu hạn của trường đóng đại số $K$, do đó $[A/m : K] = 1$. Vì thế với mỗi $a \in A$ tồn tại một vô hướng duy nhất $\lambda$ sao cho $a - \lambda \cdot 1 \in m$; kí hiệu $D(a)$ là lớp thặng dư của $a - \lambda \cdot 1$ theo môđun $m^2$. Hiển nhiên $D$ là một đạo hàm $K$ của $A$ vào $A$-môđun $m/m^2$. Tính chất phổ quát của $\Omega_K(A)$ (III, p. 569) và giả thiết $\Omega_K(A) = 0$ nay suy ra rằng $D = 0$, do đó $m/m^2 = 0$ và suy ra $m = m^2$.

Cho $(a,, ..., a,)$ là một hệ sinh của iđêan $a$; vì $a = a^2$, tồn tại các phần tử $x_{ij}$ trong $a$ sao cho $a_i = \sum_{j=1}^r x_{ij} a_j$ với $1 \leq i \leq r$. Kí hiệu $M$ là ma trận vuông cấp $r$ có các phần tử là $\delta_{ij} - x_{ij}$ và gọi $D$ là định thức của nó. Tồn tại (III, p. 532, Công thức (26)) một ma trận vuông cấp $r$ có các phần tử trong $A$ sao cho $N \cdot M = D \cdot I$, do đó ngay lập tức $Da_j = 0$ với $1 \leq j \leq r$ và suy ra cuối cùng $Da = 0$. Bây giờ ma trận $M$ đồng dư với $I$, theo môđun $a$, nên $D \equiv I$ theo môđun $a$. Đặt $e = 1 - D$; khi đó $e \in a$ và $ex = x$ với mọi $x \in a$. Suy ra $e$ là một phần tử lũy đẳng và $a$ bằng $Ae$.

Với các bổ đề này đã được thiết lập, ta hãy chứng minh bằng quy nạp theo bậc của $A$ rằng $A$ là chéo hóa được nếu $K$ là đóng đại số và $\Omega_K(A) = 0$. Cho $m$ là một iđêan cực đại của $A$ (I, p. 104). Theo Bổ đề 3 và 4, tồn tại một phần tử lũy đẳng $e$ sao cho $m = Ae$; ta đã thấy rằng $A/m$ có bậc 1 trên $K$. Do đó $A$ là tổng trực tiếp của các iđêan $a = (1 - e)A$ và $m$ và ta có $[a : K] = 1$, suy ra $A$ đẳng cấu với $K \times A/a$. Vì $\Omega_K(A/a)$ đẳng cấu với một thương của $\Omega_K(A)$ (III, p. 573, Mệnh đề 22), nên nó bằng không và giả thiết quy nạp cho thấy $A/a$ là chéo hóa được. Điều này suy ra $A$ là chéo hóa được.

### 7. Đại số reduced và đại số étale

#### Định nghĩa 2 {#alg-v-s6-def-2 .statement}

— *Cho $A$ là một vành giao hoán; khi đó $A$ được gọi là reduced nếu mọi phần tử lũy linh (I, p. 98) của $A$ đều là không.*

Nếu $A$ là một trường, hoặc một miền nguyên, hoặc một tích của các vành reduced, thì nó là một vành reduced. Để một vành giao hoán $A$ là reduced thì điều kiện cần và đủ là $a^2 \neq 0$ với mọi $a \neq 0$ trong $A$: vì từ đó, bằng quy nạp trên $n$, ta suy ra $a^{2^n} \neq 0$, do đó $a^n \neq 0$ với mọi $a \neq 0$ trong $A$.

Một đại số được gọi là *reduced* nếu vành nền của nó là reduced.

#### Mệnh đề 5 {#alg-v-s6-prop-5 .statement}

— *Cho $A$ là một đại số giao hoán có bậc hữu hạn trên $K$. Để $A$ là reduced thì điều kiện cần và đủ là tồn tại các mở rộng $L_1, \ldots, L_s$ có bậc hữu hạn trên $K$ sao cho $A$ $K$-đẳng cấu với $L_1 \times \cdots \times L_s$.*

Điều kiện nêu ra rõ ràng là đủ.

Ngược lại, giả sử $A$ là reduced; lập luận bằng quy nạp theo bậc của $A$ cho thấy chỉ cần chứng minh rằng nếu $A$ không phải là một trường, thì tồn tại hai đại số khác không $A_1$ và $A_2$ sao cho $A$ đẳng cấu với $A_1 \times A_2$, hay cũng có thể nói rằng trong $A$ tồn tại một phần tử lũy đẳng khác 0 và 1.

Từ đây giả sử rằng $A$ là reduced và không phải là một trường. Trong các iđêan của $A$ khác 0 và $A$, hãy lấy $a$ là một iđêan có số chiều với tư cách là không gian vectơ trên $K$ là nhỏ nhất. Với mọi $x \neq 0$ trong $a$ ta có $x^2 \neq 0$, vì $A$ là reduced, do đó $a' \neq \{0\}$. Ta có $a^2 \subset a$ và bởi tính cực tiểu của $a$ ta suy ra rằng $a' = a$. Theo Bổ đề 4 tồn tại một phần tử lũy đẳng $e$ sao cho $a = Ae$, và ta có $e \neq 0, e \neq 1$ vì $a$ khác 0 và $A$.

#### Định lý 4 {#alg-v-s6-thm-4 .statement}

— *Cho $A$ là một đại số giao hoán có bậc hữu hạn trên $K$. Khi đó các mệnh đề sau là tương đương:
a) Đại số $A$ là etale.
b) Với mọi mở rộng $L$ của $K$, vành $L \otimes_K A$ là reduced.
c) Tồn tại một trường hoàn hảo $P$ mở rộng của $K$ sao cho vành $P \otimes_K A$ là reduced.
d) Tồn tại các mở rộng đại số tách được $L_1, \ldots, L_s$ của $K$ sao cho $A$ đẳng cấu với $L_1 \times \cdots \times L_s$.*
Đặc biệt, mọi đại số etale đều là reduced.

A) Trước hết ta chứng minh sự tương đương của $a$, $b$ và $c$.

Giả sử rằng $A$ là etale và cho $L$ là một mở rộng của $K$. Cho $\Omega$ là một trường mở rộng đóng đại số của $L$ (V, p. 23, Định lý 2). Khi đó $L \otimes_K A$ đẳng cấu với một vành con của $\Omega \otimes_K A$ và vành sau đẳng cấu với một vành $\Omega^n$ theo Mệnh đề 2 (V, p. 30). Do đó vành $L \otimes_K A$ là reduced.

Vậy ta đã chứng minh rằng a) suy ra b), và c) là một trường hợp riêng của b). Giả sử bây giờ c) đúng. Để $K$-đại số $A$ là etale thì cần và đủ rằng $P$-đại số $A_{(P)}$ phải là etale (V, p. 32, Hệ quả 2). Do đó đại số $A$ là etale theo bổ đề sau:

#### Bổ đề 5 {#alg-v-s6-lem-5 .statement}

*Cho $B$ là một đại số reduced có bậc hữu hạn trên một trường hoàn hảo $P$; khi đó $B$ là etale.*

Theo Mệnh đề 5 tồn tại các mở rộng $L_1, \ldots, L_n$ của $P$ sao cho $B$ đẳng cấu với đại số $L, x \ldots x L_n$. Vì tích hữu hạn của các đại số etale là etale (V, p. 31, Hệ quả) nên chỉ cần xét trường hợp $B$ là một mở rộng của $P$. Theo Định lý 3 (V, p. 33) chỉ cần chứng minh rằng $dx = 0$ trong $\Omega_P(B)$ với mọi $x \in B$.

Let $x \in B$; vì $B$ có bậc hữu hạn trên $K$, $x$ là đại số trên $K$ (V, p. 18, Mệnh đề 2). Gọi $f$ là đa thức tối tiểu của $x$ và gọi $f'$ là đạo hàm của $f$. Đa thức $f$ không hằng. Giả sử $f' = 0$; theo V, p. 9, hệ quả, trường $P$ có đặc số $p \neq 0$ và ta có $f \in P[X^p]$; vì $P$ hoàn hảo, ta có $P[X^p] = P[X]^p$, nhưng đa thức bất khả quy $f$ không thể nằm trong $P[X]^p$.

Vậy ta có $f' \neq 0$ và vì bậc của $f'$ nhỏ hơn hẳn bậc của $f$, ta có $f'(x) \neq 0$. Bây giờ từ $f(x) = 0$ ta suy ra $f(x) \cdot dx = 0$ trong $\Omega_P(B)$, do đó $dx = 0$, như đã phải chứng minh.

*B) Giả sử rằng $A$ là etale; theo sự tương đương của a) và b) thì đại số $A$ là một đại số rút gọn, nên tồn tại các mở rộng $L_1, \ldots, L_n$ của $K$ sao cho $A$ đẳng cấu với $L_1 \times \cdots \times L_n$ (Mệnh đề 5). Vì $A$ là etale, mỗi mở rộng $L_i$ là một đại số etale (V, p. 31, hệ quả), và do đó theo định nghĩa là một mở rộng đại số tách được của $K$.

Suy ra mệnh đề $d) \Rightarrow a)$ từ V, p. 31, hệ quả. \*

#### Hệ quả {#alg-v-s6-n7-cor-1 .statement}

— *Giả sử rằng $K$ có đặc số $p \neq 0$. Để $A$ là etale thì điều kiện cần và đủ là $A = K[A^p]$. Với mọi cơ sở $(a_i)_i$, của $A$ trên $K$, họ $(a_i^p)_i$ khi đó là một cơ sở của $A$ trên $K$.*

Hãy chọn một bao đóng đại số $\Omega$ của $K$. Cho hai đồng cấu $K$ $u$ và $v$ của $A$ vào $\Omega$, nếu $u$ và $v$ có cùng hạn chế trên $K[A^p]$, ta có

$$
u(x)^p = u(x^p) = v(x^p) = v(x)^p,
$$

do đó $u(x) = v(x)$

với mọi $x \in A$. Ta do đó có bất đẳng thức $[A : K], \leq [K[A^p] : K]_s$; nếu $A$ là etale, ta do đó có

$$
[A : K] = [A : K]_s \leq [K[A^p] : K]_s \leq [K[A^p] : K],
$$

suy ra $A = K[A^p]$

Ngược lại, giả sử rằng $A = K[A^p]$; cho $(a_i)_{i \in I}$ là một cơ sở của $A$ trên $K$. Theo V, p. 4, Mệnh đề 2, b), họ $(a_i^p)_{i \in I}$ sinh ra không gian $K$-vectơ $K[A^p]$ và vì $A = K[A^p]$ có số chiều hữu hạn bằng lực lượng của $I$, họ $(a_i^p)_{i \in I}$ là một cơ sở của $A$ trên $K$. Cho $u$ là một phần tử của $\Omega \otimes_K A$ sao cho $u^2 = 0$, do đó $u^p = 0$; vì $(a_i)_{i \in I}$ là một cơ sở của $A$ trên $K$, tồn tại một họ $(\lambda_i)_{i \in I}$ các phần tử của $\Omega$ sao cho $u = \sum_{i \in I} \lambda_i \otimes a_i$, do đó $u^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p$. Vì $(a_i^p)_{i \in I}$ là một cơ sở của $A$ trên $K$ và $u^p = 0$, ta phải có $\lambda_i^p = 0$, do đó $\lambda_i = 0$ với mọi $i \in I$, và suy ra $u = 0$. Điều này cho thấy vành $\Omega \otimes_K A$ là rút gọn; vì $\Omega$ là hoàn hảo, đại số $A$ trên $K$ là etale theo Định lý 4.

Về một đặc trưng hóa khác của các đại số etale, xem V, p. 48, Mệnh đề 1.

### Bài tập {#alg-v-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
