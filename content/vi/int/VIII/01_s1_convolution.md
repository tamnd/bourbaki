---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 1
section_title: Convolution
lang: vi
source: int-vii-ix
pdf_pages: 0101-0108, 0159-0159
extraction: ocr
subsections:
    - "no": 1
      title: Definition and examples
      page: 0
      pdf_page: 101
    - "no": 2
      title: Associativity
      page: 3
      pdf_page: 103
    - "no": 3
      title: The case of bounded measures
      page: 6
      pdf_page: 106
    - "no": 4
      title: Properties concerning supports
      page: 6
      pdf_page: 106
    - "no": 5
      title: Vectorial expression of the convolution product
      page: 7
      pdf_page: 107
statements: 13
exercises: 2
content_sha256: af6788d4cd94da288168c40286951d9317eaafce16f18aedc3b366a6ed13170d
translated_from: content/en/int/VIII/01_s1_convolution.md
source_content_sha256: 05a5c461e581e8c2e10046aed639d554454123e90cb161ea1a5ac41500577113
translation_model: gpt-5.4
translation_run: translate-vi-fd094c6b
glossary_version: 34
glossary_terms_sha256: d37e69805ee6677a11d019881dc7dcc832be81a0dab9eb65cc5a171b0193ae3c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. PHÉP CHẬP

### 1. Định nghĩa và ví dụ

Nhắc lại (Ch. V, §6, Nos. 1 and 4; Ch. VI, §2, No. 10) rằng, nếu X và Y là các không gian compact địa phương, $\mu$ là một độ đo trên X, và $\varphi$ là một ánh xạ từ X vào Y, thì $\varphi$ được gọi là $\mu$-thực sự nếu: a) $\varphi$ là $\mu$-đo được; b) với mọi tập con compact K của Y, $\varphi^{-1}(K)$ là $\mu$-khả tích thiết yếu. Khi đó độ đo ảnh $\nu = \varphi(\mu)$ trên Y tồn tại và có tính chất sau: để một hàm f trên Y, nhận giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$, là khả tích thiết yếu đối với $\nu$, điều kiện cần và đủ là $f \circ \varphi$ có tính chất ấy đối với $\mu$, trong trường hợp đó,

$$
\int_Y f(y)\, d\nu(y) = \int_X f(\varphi(x)) d\mu(x).
$$

#### Định nghĩa 1 {#int-viii-s1-def-1 .statement}

*Cho $X_1, \ldots, X_n$ là các không gian compact địa phương, $\mu_i$ là một độ đo trên $X_i$ ($1 \leq i \leq n$); đặt X là tích của các $X_i$, $\mu$ là tích của các $\mu_i$. Cho $\varphi$ là một ánh xạ từ X vào một không gian compact địa phương Y. Người ta nói rằng dãy $(\mu_i)$ là $\varphi$-khả chập, hoặc rằng $\mu_1, \ldots, \mu_n$ là $\varphi$-khả chập, nếu $\varphi$ là $\mu$-thực sự; trong trường hợp đó, ảnh $\nu = \varphi(\mu)$ của $\mu$ dưới $\varphi$ được gọi là tích chập của các $\mu_i$ đối với $\varphi$, và được ký hiệu là $*_{\varphi}(\mu_i)_{1 \leq i \leq n}$, hoặc $*_{i=1}^n \mu_i$, hoặc $\mu_1 * \mu_2 * \cdots * \mu_n$.*

Hai ký hiệu sau cùng dĩ nhiên chỉ được dùng khi không thể có sự nghi ngờ nào về $\varphi$.

Cho f là một hàm trên Y, nhận giá trị trong một không gian Banach hoặc trong $\overline{\mathbf{R}}$. Điều kiện cần và đủ để f khả tích theo nghĩa thiết yếu đối với $\mu_1 * \cdots * \mu_n$ là hàm

$$
(x_1, \ldots, x_n) \mapsto f(\varphi(x_1, \ldots, x_n))
$$

khả tích theo nghĩa thiết yếu đối với $\mu_1 \otimes \mu_2 \otimes \cdots \otimes \mu_n$, và khi đó

$$
(1) \quad \int f\ d(\mu_1 * \cdots * \mu_n) = \int f(\varphi(x_1, \ldots, x_n)) d\mu_1(x_1) \ldots d\mu_n(x_n),
$$

một công thức có thể được xem như *định nghĩa* của $\mu_1 * \cdots * \mu_n$ khi lấy $f \in \mathcal{K}(Y)$.

Các định nghĩa lập tức suy ra rằng các $\mu_i$ lấy tích chập được nếu và chỉ nếu các $|\mu_i|$ lấy tích chập được. Khi điều đó xảy ra,

$$
|\varphi(\mu_1 \otimes \cdots \otimes \mu_n)| \leq \varphi(|\mu_1 \otimes \cdots \otimes \mu_n|) = \varphi(|\mu_1| \otimes \cdots \otimes |\mu_n|)
$$
(Ch. VI, §2, No. 10), nghĩa là,

$$
(2) \quad |*_i \mu_i| \leq *_i |\mu_i|.
$$

Nếu các $\mu_i$ khả chập được và dương, và nếu $\nu_i$ là một độ đo trên $X_i$ sao cho $0 \leq \nu_i \leq \mu_i$, thì các $\nu_i$ khả chập được và

$$
*_i \nu_i \leq *_i \mu_i.
$$

Giả sử $\mu_1, \mu_2, \ldots, \mu_n$ khả chập được, và $\mu'_1, \mu_2, \ldots, \mu_n$ cũng khả chập được ($\mu'_1$ là một độ đo trên $X_1$). Theo Ch. V, §6, No. 3, Hệ quả 1 của Mệnh đề 6, $\mu_1 + \mu'_1, \mu_2, \ldots, \mu_n$ khả chập được và

$$
(\mu_1 + \mu'_1) * \mu_2 * \cdots * \mu_n = \mu_1 * \mu_2 * \cdots * \mu_n + \mu'_1 * \mu_2 * \cdots * \mu_n.
$$

#### Ví dụ {#int-viii-s1-n1-exa-1 .statement}

— 1) Với mọi $\varphi$, các độ đo $\varepsilon_{x_i}$, trong đó $x_i \in X_i$ với $1 \leq i \leq n$, luôn luôn khả chập và có tích chập là $\varepsilon_y$, với $y = \varphi(x_1, x_2, \ldots, x_n)$. Do đó, nếu mỗi $\mu_i$ đều có giá hữu hạn, thì các $\mu_i$ khả chập và $\mu_1 * \cdots * \mu_n$ có giá hữu hạn. Đặc biệt, cho $M$ là một monoid$^1$ được trang bị một tôpô compact địa phương; nếu lấy $\varphi$ là luật hợp thành trong $M$ thì các độ đo trên $M$ có giá hữu hạn tạo thành, đối với phép chập, một đại số không gì khác hơn là *đại số của monoid* $M$ (trên $\mathbf{R}$ hoặc trên $\mathbf{C}$, tùy theo người ta xét các độ đo thực hay phức) (A, III, §2, No. 6).

2) Cho $M$ là một monoïde được trang bị tôpô rời rạc; giả sử rằng với mỗi $m \in M$, chỉ có hữu hạn cặp $(m', m'') \in M \times M$ sao cho $m'm'' = m$; điều này có nghĩa là luật hợp thành trong $M$ là một ánh xạ thực sự từ $M \times M$ vào $M$; khi đó các độ đo trên $M$ lập thành một đại số đối với phép chập, một đại số không là gì khác ngoài đại số *toàn bộ*

(1) Monoïde, theo nghĩa của Bài tập 17 của Ch. VII, §1.

của monoïde $M$ (A, III, §2, No. 10); chúng tôi chú ý hai trường hợp đặc biệt sau:

a) $M = N$, với luật hợp thành là phép cộng. Với mỗi độ đo $\mu$ trên $N$, ta gắn cho nó chuỗi hình thức

$$
S(\mu) = \sum_{n=0}^{\infty} \mu(\{n\}) t^n
$$

trong một bất định $t$. Khi đó $S(\mu * \mu') = S(\mu)S(\mu')$. Một nhận xét tương tự cũng đúng đối với các chuỗi hình thức theo một số bất định tùy ý.

$*b)$ $M = N^*$, luật hợp thành là phép nhân. Với mỗi độ đo $\mu$ trên $N^*$, ta gắn cho nó chuỗi Dirichlet hình thức

$$
D(\mu) = \sum_{n=1}^{\infty} \mu(\{n\}) n^{-s}.
$$

Khi đó $D(\mu * \mu') = D(\mu)D(\mu')$.

3) Cho $X, Y, Z$ là các không gian địa phương compact, $\varphi$ là một ánh xạ liên tục từ $X \times Y$ vào $Z$. Nếu $x \in X$ và $\mu$ là một độ đo trên $Y$, thì nói rằng $\varepsilon_x$ và $\mu$ là $\varphi$-khả chập tương đương với nói rằng ánh xạ $\varphi(x, \cdot)$ từ $Y$ vào $Z$ là $\mu$-thực sự. Khi đó ta có $\varepsilon_x * \mu = \varphi(x, \cdot)(\mu)$.

### 2. Tính kết hợp

Bổ đề sau đây hoàn chỉnh Mệnh đề 11 của Ch. V, §8, No. 5:²

#### Bổ đề 1 {#int-viii-s1-lem-1 .statement}

Với $1 \leq i \leq n$, gọi $X_i, Y_i$ là hai không gian compact địa phương, $\mu_i$ là một độ đo trên $X_i$, và $\varphi_i$ là một ánh xạ liên tục từ $X_i$ vào $Y_i$. Đặt $X = \prod_i X_i$, $Y = \prod_i Y_i$, $\mu = \bigotimes_i \mu_i$, và $\varphi$ là ánh xạ từ $X$ vào $Y$ bằng tích của các $\varphi_i$. Nếu $\varphi$ là $\mu$-thực sự và $\mu_i \neq 0$ với mọi $i$, thì các $\varphi_i$ là $\mu_i$-thực sự và $\varphi(\mu) = \bigotimes_i \varphi_i(\mu_i)$.

Ta có thể giả sử rằng các $\mu_i$ là dương và $n = 2$. Cho $f_1 \in \mathcal{K}_+(Y_1)$. Vì $\mu_2 \neq 0$, tồn tại một $f_2 \in \mathcal{K}_+(Y_2)$ sao cho $f_2 \circ \varphi_2$ không phải là $\mu_2$-không đáng kể. Hàm $(x_1, x_2) \mapsto f_1(\varphi_1(x_1)) f_2(\varphi_2(x_2))$ hầu khắp khả tích đối với $\mu$ và liên tục, nên khả tích đối với $\mu$. Do đó tồn tại một $x_2 \in X_2$ sao cho $f_2(\varphi_2(x_2)) \neq 0$ và sao cho hàm $x_1 \mapsto f_1(\varphi_1(x_1)) f_2(\varphi_2(x_2))$ khả tích đối với $\mu_1$. Do đó $f_1 \circ \varphi_1$ khả tích đối với $\mu_1$,

²Bổ đề này suy ra bằng quy nạp theo phần b) của Mệnh đề 11 đã dẫn, tức là trường hợp $n = 2$; kết quả tương ứng trong ấn bản thứ nhất của Ch. V (§8, No. 3, Mệnh đề 7) không bao gồm kết quả của phần b).

điều đó chứng tỏ rằng $\varphi_1$ là $\mu_1$-thực sự. Ta lập luận tương tự đối với $\varphi_2$. Khi đó $\varphi(\mu) = \bigotimes_i \varphi_i(\mu_i)$ theo Mệnh đề 11 của Ch. V, §8, No. 5.

Bổ đề sau hoàn tất Mệnh đề 4 của Ch. V, §6, No. 3.\footnote{Mệnh đề của bổ đề này thực ra là phần *b*) của Mệnh đề 4 đã dẫn, một phần đã không được đưa vào trong ấn bản thứ nhất của Ch. V.}

#### Bổ đề 2 {#int-viii-s1-lem-2 .statement}

*Giả sử T, T', T'' là ba không gian địa phương compact, $\mu$ là một độ đo trên T, $\pi$ là một ánh xạ $\mu$-đo được từ T vào T', $\pi'$ là một ánh xạ liên tục từ T' vào T'', và $\pi'' = \pi' \circ \pi$. Nếu $\pi''$ là $\mu$-thực sự, thì $\pi$ là $\mu$-thực sự, $\pi'$ là $\pi(\mu)$-thực sự, và $\pi''(\mu) = \pi'(\pi(\mu))$.*

Cho K' là một tập con compắc của T'. Khi đó $K'' = \pi'(K')$ là compắc, do đó $\pi''(K'')$ là khả tích thiết yếu đối với $\mu$, do đó $\pi^{-1}(K') \subset \pi''(K'')$ là khả tích thiết yếu đối với $\mu$, vì thế $\pi$ là $\mu$-thực sự. Khi đó $\pi'$ là $\pi(\mu)$-thực sự và $\pi''(\mu) = \pi'(\pi(\mu))$ theo Ch. V, §6, No. 3, Mệnh đề 4.

#### Mệnh đề 1 {#int-viii-s1-prop-1 .statement}

*Cho $X_{ij}$ ($1 \leq i \leq m, 1 \leq j \leq n_i$), $Y_i$ ($1 \leq i \leq m$), và Z là các không gian compact địa phương; với mỗi i, gọi $\varphi_i$ là một ánh xạ từ $X_i = \prod_j X_{ij}$ vào $Y_i$; gọi $\varphi$ là tích của các $\varphi_i$, ánh xạ $X = \prod_i X_i$ vào $Y = \prod_i Y_i$; gọi $\psi$ là một ánh xạ từ Y vào Z.

(i) *Cho các $\mu_{ij}$ lần lượt là những độ đo đã cho trên các $X_{ij}$, sao cho, với mỗi i, các $\mu_{ij}$ ($1 \leq j \leq n_i$) là $\varphi_i$-khả hợp, và sao cho các độ đo $*| \mu_{ij} |$ là $\psi$-khả hợp; khi đó các $\mu_{ij}$, với $1 \leq i \leq m, 1 \leq j \leq n_i$, là $(\psi \circ \varphi)$-khả hợp và*

$$
*_{i,j} \mu_{ij} = *_i \left( *_j \mu_{ij} \right).
$$

(ii) *Giả sử $\psi$ và các $\varphi_i$ liên tục, và cho các $\mu_{ij}$ là những độ đo $\neq 0$ lần lượt cho trên các $X_{ij}$ và khả hợp đối với $(\psi \circ \varphi)$; khi đó, với mỗi i, các $\mu_{ij}$ ($1 \leq j \leq n_i$) là khả hợp đối với $\varphi_i$, các độ đo $*_j |\mu_{ij}|$ là khả hợp đối với $\psi$, và công thức (3) đúng.*

Chỉ cần xét trường hợp tất cả các độ đo đang nói đến đều $\geq 0$.

Hãy đặt mình dưới các giả thiết của (i). Ánh xạ $\varphi$ là thực sự đối với $\bigotimes_{i,j} \mu_{ij}$, và

$$
\varphi \left( \bigotimes_{i,j} \mu_{ij} \right) = \bigotimes_i \varphi_i \left( \bigotimes_j \mu_{ij} \right) = \bigotimes_i \left( *_j \mu_{ij} \right)
$$

(Ch. V, §8, No. 5, Mệnh đề 11). Ánh xạ $\psi \circ \varphi$ là thực sự đối với $\bigotimes_{i,j} \mu_{ij}$, và
$$
(\psi \circ \varphi)\left( \bigotimes_{i,j} \mu_{ij} \right) = \psi\left( \bigotimes_i (*_j \mu_{ij}) \right) = *_i (*_j \mu_{ij})
$$
(Ch. V, §6, Mệnh đề 4). Do đó các $\mu_{ij}$ ($1 \leq i \leq m,\ 1 \leq j \leq n_i$) là $(\psi \circ \varphi)$-khả chập và công thức (3) đúng.

Ta đặt mình dưới các giả thiết của (ii). Trước hết, Bổ đề 2 chứng minh rằng $\varphi$ là thực sự đối với $\bigotimes_{i,j} \mu_{ij}$. Khi đó Bổ đề 1 chứng minh rằng với mọi $i$, $\varphi_i$ là thực sự đối với $\bigotimes_j \mu_{ij}$, và rằng
$$
\varphi\left( \bigotimes_{i,j} \mu_{ij} \right) = \bigotimes_i (*_j \mu_{ij}).
$$
Theo Bổ đề 2, $\psi$ là thực sự đối với $\bigotimes_i (*_j \mu_{ij})$. Do đó suy ra mệnh đề.

#### Hệ quả {#int-viii-s1-n2-cor-1 .statement}

— Cho $X_i, X'_i$ ($1 \leq i \leq n$), $Y, Y'$ là các không gian compact địa phương; cho $\varphi, \varphi'$ là các ánh xạ liên tục từ $X = \prod_i X_i$ vào $Y$ và từ $X' = \prod_i X'_i$ vào $Y'$, tương ứng; cho $f_i$ là các ánh xạ liên tục từ $X_i$ vào $X'_i$ ($1 \leq i \leq n$) và $g$ là một ánh xạ liên tục từ $Y$ vào $Y'$, sao cho $\varphi' \circ f = g \circ \varphi$, trong đó $f$ là ánh xạ từ $X$ vào $X'$ bằng tích của các $f_i$. Cho $\mu_i$ là các độ đo được cho tương ứng trên các $X_i$, tất cả đều $\neq 0$. Khi đó hai khẳng định sau là tương đương:
(i) $f_i$ là $\mu_i$-thực sự với mọi $i$, và các độ đo $f_i(|\mu_i|)$ là $\varphi'$-khả chập;
(ii) các $\mu_i$ là $\varphi$-khả chập, và $g$ là thực sự đối với $*_{\varphi}(|\mu_i|)$.

Hơn nữa, khi các khẳng định này được kiểm chứng,
$$
*_{\varphi'}(f_i(\mu_i)) = g(*_{\varphi}(\mu_i)) = *_{g \circ \varphi}(\mu_i).
$$

Thật vậy, đặt $h = \varphi' \circ f = g \circ \varphi$. Theo Mệnh đề 1, mỗi điều kiện (i) và (ii) đều tương đương với điều kiện sau:
(iii) các $\mu_i$ là $h$-khả chập.
Khi điều đó xảy ra,
$$
*_{\varphi'}(f_i(\mu_i)) = *_h(\mu_i) = g(*_{\varphi}(\mu_i)).
$$

### 3. Trường hợp các độ đo bị chặn

#### Mệnh đề 2 {#int-viii-s1-prop-2 .statement}

— Cho $X_1, \ldots, X_n, Y$ là các không gian địa phương compact, $\mu_i$ là một độ đo bị chặn trên $X_i$ ($1 \leq i \leq n$), $\mu$ là tích của các $\mu_i$, $\varphi$ là một ánh xạ $\mu$-đo được từ $\prod_{i=1}^n X_i$ vào $Y$. Khi đó các $\mu_i$ là $\varphi$-khả chập và
$$
\left\| *_{i=1}^n \mu_i \right\| \leq \prod_{i=1}^n \| \mu_i \|.
$$
Nếu hơn nữa các $\mu_i$ là dương, thì
$$
\left\| *_{i=1}^n \mu_i \right\| = \prod_{i=1}^n \| \mu_i \|.
$$
Thật vậy, $\mu'_i = |\mu_i|$ bị chặn và $\| \mu'_i \| = \| \mu_i \|$ (Ch. III, §1, No. 8, Hệ quả 1 của Mệnh đề 10). Ta có $|\mu_1 \otimes \cdots \otimes \mu_n| = \mu'_1 \otimes \cdots \otimes \mu'_n$ (Ch. III, §4, Nos. 2, 4), do đó $\mu_1 \otimes \cdots \otimes \mu_n$ bị chặn và
$$
\| \mu_1 \otimes \cdots \otimes \mu_n \| = \| \mu_1 \| \cdots \| \mu_n \|
$$
(sđd., Mệnh đề 4). Do đó $\varphi$ là $\mu$-thực sự (Ch. V, §6, No. 1, Nhận xét 1), nghĩa là các $\mu_i$ là $\varphi$-khả chập. Ta có $\| *_{i=1}^n \mu'_i \| = \| \mu'_1 \otimes \cdots \otimes \mu'_n \|$ (Ch. V, §6, No. 2, Định lý 1), do đó $\| *_{i=1}^n \mu'_i \| = \| \mu'_1 \| \cdots \| \mu'_n \|$. Sau cùng, $| *_{i} \mu_i | \leq *_{i} \mu'_i$ (No. 1, công thức (2)), do đó
$$
\left\| *_{i} \mu_i \right\| \leq \left\| *_{i} \mu'_i \right\| = \prod_{i=1}^n \| \mu_i \|.
$$

#### Mệnh đề 3 {#int-viii-s1-prop-3 .statement}

— Cho $X_1, \ldots, X_n, Y$ là các không gian compact địa phương, $\varphi$ là một ánh xạ liên tục từ $\prod_{i=1}^n X_i$ vào $Y$. Khi đó ánh xạ
$$
(\mu, \ldots, \mu_n) \mapsto *_{\varphi} (\mu_i)
$$
từ $\prod_{i=1}^n \mathcal{M}^1(X_i)$ vào $\mathcal{M}^1(Y)$ là một ánh xạ đa tuyến tính liên tục.
Điều này suy ra từ Mệnh đề 2 và những gì đã nói ở No. 1.

### 4. Các tính chất liên quan đến giá

#### Mệnh đề 4 {#int-viii-s1-prop-4 .statement}

— Cho $X_1, \ldots, X_n, Y$ là các không gian compact địa phương, $\mu_i$ là một độ đo trên $X_i$ ($1 \leq i \leq n$), $S_i$ là giá của nó, và $\varphi$ là một ánh xạ liên tục từ $\prod_i X_i$ vào $Y$ sao cho hạn chế của $\varphi$ trên $\prod_i S_i$ là thực sự. Khi đó các $\mu_i$ là $\varphi$-khả chập.

Thật vậy, cho $K$ là một tập con compact của $Y$. Giá của $\mu = \mu_1 \otimes \cdots \otimes \mu_n$ là $S = \prod_i S_i$ (Ch. III, §4, No. 2, Prop. 2). Do đó $\overline{\varphi}(K) \cap \left( \prod_i X_i - S \right)$ là $\mu$-không đáng kể. Mặt khác, $\overline{\varphi}(K) \cap S$ là compact. Vậy $\overline{\varphi}(K)$ là $\mu$-khả tích.

#### Mệnh đề 5 {#int-viii-s1-prop-5 .statement}

*Cho $X_1, \ldots, X_n, Y$ là các không gian compact địa phương, $\mu_i$ là một độ đo trên $X_i$ ($1 \leq i \leq n$), $\mu$ là tích của các $\mu_i$, $\varphi$ là một ánh xạ $\mu$-thực sự của $\prod_i X_i$ vào $Y$, và $S_i$ là giá của $\mu_i$.

a) *Giá của $*_{i} \mu_i$ được chứa trong bao đóng của $\varphi \left( \prod_i S_i \right)$.*

b) *Nếu $\varphi$ liên tục và các $\mu_i$ là dương, thì giá của $*_{i} \mu_i$ là bao đóng của $\varphi \left( \prod_i S_i \right)$.*

Đặt $S = \prod_i S_i$ là giá của $\mu$. Giá của $*_{i} \mu_i$ được chứa trong $\overline{\varphi(S)}$ theo Ch. V, §6, No. 2, Cor. 3 of Prop. 2. *Nếu $\varphi$ liên tục và các $\mu_i$ là dương, thì giá của $*_{i} \mu_i$ là $\overline{\varphi(S)}$* (*loc. cit.*, Cor. 4 of Prop. 2).

#### Hệ quả {#int-viii-s1-n4-cor-1 .statement}

*Nếu $\varphi$ liên tục và các $\mu_i$ có giá compact, thì các $\mu_i$ khả tích chập được và $*_{i} \mu_i$ có giá compact.*

### 5. Biểu thức vectơ của tích chập

#### Mệnh đề 6 {#int-viii-s1-prop-6 .statement}

*Cho $X, Y, Z$ là các không gian địa phương compact, $\varphi$ là một ánh xạ liên tục từ $X \times Y$ vào $Z$, và $\lambda, \mu$ là các độ đo trên $X, Y$. Để $\lambda$ và $\mu$ là $\varphi$-khả chập, điều kiện cần và đủ là ánh xạ $(x, y) \mapsto \varepsilon_{\varphi(x,y)} = \varepsilon_x * \varepsilon_y$ từ $X \times Y$ vào $\mathcal{M}(Z)$ là khả tích vô hướng đối với $(\lambda \otimes \mu)$ theo tôpô $\sigma(\mathcal{M}(Z), \mathcal{H}(Z))$, khi đó*

$$
\lambda * \mu = \int_{X \times Y} (\varepsilon_x * \varepsilon_y) \, d\lambda(x) \, d\mu(y).
$$

Nói rằng $\lambda$ và $\mu$ là $\varphi$-chập được có nghĩa là, với mọi $f \in \mathcal{H}(Z)$, $f \circ \varphi$ là $(\lambda \otimes \mu)$-khả tích, tức là, với mọi $f \in \mathcal{H}(Z)$ hàm $(x, y) \mapsto \langle f, \varepsilon_{\varphi(x,y)} \rangle$ là $(\lambda \otimes \mu)$-khả tích, hay lại nữa, ánh xạ $(x, y) \mapsto \varepsilon_{\varphi(x,y)}$ từ $X \times Y$ vào $\mathcal{M}(Z)$ là khả tích vô hướng theo $(\lambda \otimes \mu)$ đối với $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$. Nếu đúng như vậy, thì

$$
\langle \lambda * \mu, f \rangle = \int f(\varphi(x, y)) d\lambda(x) d\mu(y) = \int_{X \times Y} \langle \varepsilon_{\varphi(x,y)}, f \rangle d\lambda(x) d\mu(y),
$$

do đó $\lambda * \mu = \int_{X \times Y} \varepsilon_{\varphi(x,y)} d\lambda(x) d\mu(y)$.

#### Mệnh đề 7 {#int-viii-s1-prop-7 .statement}

*Cho X, Y, Z là các không gian compact địa phương, $\varphi$ là một ánh xạ liên tục từ $X \times Y$ vào Z, và $\lambda, \mu$ là các độ đo trên X, Y. Giả sử rằng với mọi $x \in X$, $\varepsilon_x$ và $\mu$ là khả chập theo $\varphi$. Để $\lambda$ và $\mu$ là khả chập theo $\varphi$, điều kiện cần và đủ là ánh xạ $x \mapsto \varepsilon_x * |\mu|$ từ X vào $\mathcal{M}(Z)$ là khả tích vô hướng theo $\lambda$ đối với tôpô $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$, khi đó $\lambda * \mu = \int_X (\varepsilon_x * \mu) d\lambda(x)$.*

Giả sử rằng $\lambda$ và $\mu$ là $\varphi$-khả chập. Với mọi $f \in \mathcal{K}(Z)$, $f \circ \varphi$ là $(|\lambda| \otimes |\mu|)$-khả tích, do đó hàm $x \mapsto \int_Y f(\varphi(x, y)) d|\mu|(y) = \langle f, \varepsilon_x * |\mu| \rangle$ (mà theo giả thiết được xác định với mọi $x \in X$) là $\lambda$-khả tích; vì thế $x \mapsto \varepsilon_x * |\mu|$ là khả tích vô hướng theo $\lambda$ đối với $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$, và

$$
\langle f, \lambda * \mu \rangle = \int_X d\lambda(x) \int_Y f(\varphi(x, y)) d\mu(y) = \int_X \langle f, \varepsilon_x * \mu \rangle d\lambda(x),
$$

do đó $\lambda * \mu = \int_X (\varepsilon_x * \mu) d\lambda(x)$. Ngược lại, giả sử rằng ánh xạ $x \mapsto \varepsilon_x * |\mu|$ từ X vào $\mathcal{M}(Z)$ là khả tích vô hướng đối với $\lambda$ cho $\sigma(\mathcal{M}(Z), \mathcal{K}(Z))$. Cho $f \in \mathcal{K}_+(Z)$. Khi đó hàm $(x, y) \mapsto f(\varphi(x, y))$ là liên tục và (Ch. V, §8, No. 3, Prop. 5)

$$
\iint^* f(\varphi(x, y)) d|\lambda|(x) d|\mu|(y) = \int^* d|\lambda|(x) \int^* f(\varphi(x, y)) d|\mu|(y)
= \int^* \langle f, \varepsilon_x * |\mu| \rangle d|\lambda|(x) < +\infty.
$$

Vậy $f \circ \varphi$ là khả tích đối với $(\lambda \otimes \mu)$, suy ra $\lambda$ và $\mu$ là $\varphi$-khả chập.

### Bài tập {#int-viii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
