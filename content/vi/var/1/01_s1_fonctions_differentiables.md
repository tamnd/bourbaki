---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 1
section_title: Fonctions différentiables
lang: vi
source: var-fr
pdf_pages: 0009-0014
extraction: ocr
subsections:
    - "no": 1
      title: Ordre de contact de deux fonctions en un point
      page: 0
      pdf_page: 9
    - "no": 2
      title: Fonctions dérivables en un point
      page: 0
      pdf_page: 10
    - "no": 3
      title: Composition des fonctions dérivables
      page: 0
      pdf_page: 11
    - "no": 4
      title: Produit de fonctions dérivables
      page: 0
      pdf_page: 12
    - "no": 5
      title: Premières variantes du théorème des fonctions implicites
      page: 0
      pdf_page: 12
    - "no": 6
      title: Dérivées partielles
      page: 0
      pdf_page: 13
    - "no": 7
      title: Dérivées itérées
      page: 0
      pdf_page: 13
statements: 0
exercises: 0
content_sha256: 21019f772c273f98ac6f8a2a59e98f287424f43a50fa8aeb1a09cf12d66b356c
translated_from: content/en-mt/var/1/01_s1_fonctions_differentiables.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 0bf1c162534d51cfbef5c8dce9da23d0a8b404d715eeb87130dd56ee29844bbe
translation_model: gpt-5.4
translation_run: translate-vi-7f78aa23
glossary_version: 34
glossary_terms_sha256: a6eb52a6a6ec01ac4e9de499429dde56dd02b93efc81aaa6942898d7bd367a8b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. Hàm khả vi

Trong đoạn này, chữ E ký hiệu một không gian vectơ tôpô khả chuẩn hóa trên K; chữ F ký hiệu một không gian đa chuẩn tách trên K.

### 1.1 Cấp tiếp xúc của hai hàm tại một điểm

1.1.1. Cho X là một không gian tôpô và $\theta$ là một hàm số dương xác định trên một lân cận của một điểm $x_0$ của X. Ta nói rằng một hàm $f$, xác định trên một lân cận của $x_0$ và nhận giá trị trong F, là không đáng kể đối với $\theta$ tại $x_0$ nếu điều kiện sau được thỏa mãn:

Với mọi $\varepsilon > 0$ và với mọi nửa chuẩn liên tục $\gamma$ trên F, tồn tại một lân cận V của $x_0$ trên đó $f$ và $\theta$ được xác định và sao cho

$$
\| f(x) \|_{\gamma} \leq \varepsilon \theta(x) \quad \text{với mọi } x \in V.
$$

Để $f$ là không đáng kể đối với $\theta$, chỉ cần điều kiện này được thỏa mãn đối với một họ các nửa chuẩn $\gamma$ xác định tôpô của F. Việc $f$ có hay không là không đáng kể đối với $\theta$ tại $x_0$ chỉ phụ thuộc vào các mầm của $f$ và của $\theta$ tại $x_0$. Ta ký hiệu bởi $o_{x_0}(\theta)$ (hoặc $o(\theta)$ khi không có sự nhập nhằng về $x_0$) tập hợp các mầm tại $x_0$ của những hàm không đáng kể đối với $\theta$ tại $x_0$: đó là một không gian con vectơ của không gian các mầm tại $x_0$ của các ánh xạ nhận giá trị trong F. Nếu $f$ là không đáng kể đối với $\theta$, thì theo lạm dụng ký hiệu, ta viết $f \in o_{x_0}(\theta)$ hoặc cũng viết $f(x) \in o(\theta(x))$ khi $x$ tiến tới $x_0$.

Nếu $f$ và $g$ là hai ánh xạ từ một lân cận của $x_0$ vào F, ta cũng viết $f \equiv g \mod o(\theta)$ nếu $f - g$ là không đáng kể đối với $\theta$.

Giả sử K bằng $\mathbf{R}$ hoặc $\mathbf{C}$ và $x_0$ là điểm dính của tập Y các điểm của X tại đó $\theta$ được xác định và khác không. Khi đó quan hệ $f \in o(\theta)$ có nghĩa là $f(x)/\theta(x)$ tiến tới 0 khi $x$ tiến tới $x_0$ mà vẫn nằm trong Y, và $\theta(x) = 0$ kéo theo $f(x) = 0$.

1.1.2. Cho $f$ và $g$ là hai hàm nhận giá trị trong F, xác định trên một lân cận của một điểm $x_0$ của E. Nếu $m$ là một số nguyên dương, ta nói rằng $f$ và $g$ có tiếp xúc cấp $\geq m$ tại $x_0$ nếu có:

$$
f(x) - g(x) \in o(\| x - x_0 \|^{m}) \quad \text{khi } x \text{ tiến tới } x_0
$$

bất kể chuẩn nào được chọn để xác định tôpô của E. Để được như vậy, chỉ cần quan hệ trên được kiểm tra đối với một chuẩn xác định tôpô của E. Nếu đúng như thế, thì ta có $f(x_0) = g(x_0)$.

Nếu $f$ và $g$ nhận cùng một giá trị tại $x_0$, cận trên bé nhất (hữu hạn hoặc bằng $+\infty$) của các số nguyên $m$ sao cho $f$ và $g$ có tiếp xúc cấp $\geq m$ tại $x_0$ được gọi là cấp tiếp xúc của $f$ và $g$ tại $x_0$.

1.1.3. Cấp tiếp xúc của $f$ và $g$ tại $x_0$ chỉ phụ thuộc vào các mầm của các hàm này tại điểm $x_0$. Do đó có thể nói đến cấp tiếp xúc của hai mầm $\varphi$ và $\psi$ của các ánh xạ từ E vào F tại điểm $x_0$. Quan hệ “ $\varphi$ và $\psi$ có tiếp xúc cấp $\geq m$ ” là một quan hệ tương đương tương thích với cấu trúc không gian vectơ.

### 1.2. Hàm khả vi tại một điểm

1.2.1. Cho $f$ là một hàm được xác định trong một lân cận của điểm $x_0$ của E và nhận giá trị trong F. Ta nói rằng $f$ khả vi tại $x_0$ nếu tồn tại một hàm afin liên tục $v$ từ E vào F có tiếp xúc cấp $\geq 1$ với $f$ tại $x_0$. Ánh xạ $v$ này là duy nhất; tồn tại một và chỉ một ánh xạ tuyến tính liên tục, ký hiệu là $Df(x_0)$, từ E vào F sao cho:

$$
v(x) = v(x_0) + Df(x_0) \cdot (x - x_0).
$$

Nếu chọn một chuẩn trên E, điều này tương đương với:

$$
f(x_0 + h) \equiv f(x_0) + Df(x_0) \cdot h \mod o(\|h\|) \quad \text{với } h \text{ tiến tới } 0,
$$

cũng có thể viết dưới dạng:

$$
\lim_{h \to 0, h \neq 0} \frac{\| f(x_0 + h) - f(x_0) - Df(x_0) \cdot h \|_\gamma}{\| h \|} = 0
$$

đối với mọi nửa chuẩn liên tục $\gamma$ trên F.

Phần tử $Df(x_0)$ của $\mathcal{L}(E, F)$ được gọi là đạo hàm của $f$ tại $x_0$. Đôi khi người ta viết $D_h f(x_0)$ thay cho $Df(x_0) \cdot h$; đó là một phần tử của F được xác định bởi hệ thức:

$$
D_h f(x_0) = \lim_{t \to 0, t \neq 0} \frac{f(x_0 + th) - f(x_0)}{t}.
$$

1.2.2. Ta nói rằng một hàm $f$ khả vi chặt tại $x_0$ nếu nó khả vi tại $x_0$ và nếu ta có, đối với mọi chuẩn xác định tôpô của E, hệ thức:

$$
f(y) - f(z) \equiv Df(x_0) \cdot (y - z) \mod o(\| y - z \| )
$$

khi $(y, z)$ tiến tới $(x_0, x_0)$ trong $E \times E$. Để được điều này, chỉ cần điều kiện ấy được thỏa mãn đối với một chuẩn xác định tôpô của E. Giả sử thêm rằng E và F là các không gian định chuẩn; khi đó, với mọi số $c > \| Df(x_0) \|$, tồn tại một lân cận V của $x_0$ sao cho $\| f(y) - f(z) \| \leq c. \| y - z \|$ với $y, z$ thuộc V; điều này suy ra rằng $f$ liên tục đều trong V.

1.2.3. Việc một hàm $f$ khả vi hay khả vi chặt tại $x_0$ chỉ phụ thuộc vào mầm của $f$ tại $x_0$. Các mầm của những hàm khả vi tại $x_0$ tạo thành một không gian con vectơ $\mathcal{V}$ của không gian tất cả các mầm, và ánh xạ $f \mapsto Df(x_0)$ từ $\mathcal{V}$ vào $\mathcal{L}(E; F)$ là tuyến tính. Các mầm của những hàm khả vi chặt tại $x_0$ tạo thành một không gian con vectơ của $\mathcal{V}$.

1.2.4. Một hàm khả vi tại $x_0$ thì liên tục tại $x_0$.

1.2.5. Khi $E = K$, ánh xạ $u \mapsto u(1)$ là một đẳng cấu của $\mathcal{L}(E; F)$ lên $F$; nếu hàm $f$ khả vi tại $x_0$, phần tử

$$
f'(x_0) = Df(x_0) \cdot 1
$$

không gì khác hơn là đạo hàm của $f$ tại $x_0$ theo nghĩa đã cho trong Fonct. Var. Réelle, chap. I, § 1, n° 6, nhận xét 2.

### 1.3. Hợp thành của các ánh xạ khả vi

1.3.1. Giả sử rằng F khả chuẩn hóa được. Cho $x_0 \in E$ và $y_0 \in F$, U là một lân cận của $x_0$ và V là một lân cận của $y_0$; sau cùng, cho $f$ là một ánh xạ từ U vào V, khả vi tại $x_0$, với $f(x_0) = y_0$. Nếu $g$ là một ánh xạ từ V vào một không gian vectơ đa chuẩn tách được G, khả vi tại $y_0$, thì ánh xạ $g \circ f$ từ U vào G là khả vi tại $x_0$, và ta có:

(1)
$$
D(g \circ f)(x_0) = Dg(y_0) \circ Df(x_0).
$$
Nếu $f$ và $g$ khả vi chặt, thì $g \circ f$ cũng vậy.

1.3.2. Cho $f$ là một ánh xạ xác định trong một lân cận của một điểm $x_0$ của E và nhận giá trị trong F, khả vi tại $x_0$; nếu $u$ là một ánh xạ tuyến tính liên tục từ F vào một không gian đa chuẩn tách được G, thì hàm $u \circ f$ khả vi tại $x_0$ và ta có:

(2)
$$
D(u \circ f)(x_0) = u \circ Df(x_0).
$$

1.3.3. Giả sử rằng F là tích của một họ $(F_i)_{i \in I}$ các không gian vectơ đa chuẩn tách được; với mỗi $i$ trong I, cho $f_i$ là một ánh xạ xác định trong một lân cận U của một điểm $x_0$ của E và nhận giá trị trong F và đặt $f = (f_i)_{i \in I}$. Để $f$ khả vi (tương ứng, khả vi chặt) tại $x_0$, điều kiện cần và đủ là mọi $f_i$ đều như vậy; ta có:

(3)
$$
D_h f(x_0) = (D_h f_i(x_0))_{i \in I} \quad \text{với mọi } h \text{ trong } E.
$$

1.3.4. Nếu $E = K$, có thể thay $Df(x_0)$ bằng $f'(x_0)$ và $D_h f_i(x_0)$ bằng $f'_i(x_0)$ trong các công thức (1) và (3).

### 1.4. Tích của các ánh xạ khả vi

1.4.1. Cho $F_1, \ldots, F_m$ là các không gian chuẩn đa tách được và $u$ là một ánh xạ $m$-tuyến tính liên tục từ $F_1 \times \cdots \times F_m$ vào $F$. Cho $U$ là một lân cận của một điểm $x_0$ của $E$, và $f_i$ là một ánh xạ từ $U$ vào $F_i$ (với $1 \leq i \leq m$). Nếu các $f_i$ khả vi (resp. khả vi chặt) tại $x_0$, thì điều đó cũng đúng đối với $u(f_1, \ldots, f_m) = g$, và ta có:

(4) $D_hg(x_0) = \sum_{j=1}^m u(f_1(x_0), \ldots, D_hf_j(x_0), \ldots, f_m(x_0))$ với mọi $h$ trong $E$,

điều này sẽ được viết gọn hơn:

(5) $Dg = \sum_{j=1}^m u(f_1, \ldots, Df_j, \ldots, f_m)$.

Đặc biệt, với $m = 2$, ta có:

(6) $Du(f_1, f_2) = u(Df_1, f_2) + u(f_1, Df_2)$.

Với $m = 1$, điều này lại cho 1.3.2.

1.4.2. Khi $E = K$, có thể thay thế $Dg$ bởi $g'$ và $Df_j$ bởi $f'_j$ trong các công thức (4) đến (6).

### 1.5. Những biến thể đầu tiên của định lý hàm ẩn

Giả sử $E$ và $F$ là các không gian Banach, và cho $x_0$ là một điểm của $E$, $U$ là một lân cận của $x_0$ và $f$ là một ánh xạ từ $U$ vào $F$. Giả sử thêm rằng $f$ khả vi chặt tại $x_0$.

1.5.1. Nếu $Df(x_0)$ là một đẳng cấu từ $E$ lên $F$, thì tồn tại một lân cận mở $U_0$ của $x_0$ được chứa trong $U$ và một lân cận mở $V_0$ của $f(x_0)$ sao cho $f|U_0$ là một đồng phôi từ $U_0$ lên $V_0$. Ánh xạ $g : V_0 \to U_0$ nghịch đảo của $f|U_0$ khả vi chặt tại điểm $f(x_0)$, và ta có:

$$
Dg(f(x_0)) = Df(x_0)^{-1}.
$$

1.5.2. Nếu $Df(x_0)$ là một ánh xạ toàn ánh từ $E$ lên $F$, thì tồn tại một lân cận mở $U_0$ của $x_0$ được chứa trong $U$, sao cho $f|U_0$ là một ánh xạ mở.

1.5.3. Nếu $Df(x_0)$ là đơn ánh và có ảnh đóng, thì tồn tại một lân cận đóng $U_0$ của $x_0$ được chứa trong $U$, sao cho $f|U_0$ là một đồng phôi từ $U_0$ lên một tập con đóng của $F$.

### 1.6. Đạo hàm riêng

1.6.1. Cho $f$ là một hàm xác định trong một lân cận $U$ của điểm $x_0$ của $E$ và nhận giá trị trong $F$. Cho $X$ là một không gian vectơ và $V$ là tập hợp các điểm $x$ của $X$ sao cho $x_0 + x \in U$; đặt $g(x) = f(x_0 + x)$ với $x \in V$. Ta nói rằng $f$ thừa nhận một *đạo hàm riêng theo* $X$ *tại* $x_0$ nếu $g$ thừa nhận đạo hàm tại $0$; đạo hàm này được ký hiệu bởi $D_X f(x_0)$; đó là một ánh xạ tuyến tính liên tục từ $X$ vào $F$. Nếu $f$ khả vi tại $x_0$, thì nó thừa nhận một đạo hàm riêng theo $X$ tại $x_0$, và đạo hàm riêng này là hạn chế của $Df(x_0)$ lên $X$.

1.6.2. Giả sử rằng $E$ là tích của một họ hữu hạn các không gian vectơ định chuẩn $E_i$ ($1 \leq i \leq n$) được đồng nhất một cách chính tắc với các không gian con của $E$; cho $x_0 = (x_0^1, \ldots, x_0^n)$ trong $E$ và cho $U$ là một lân cận của $x_0$ trong $E$; sau cùng cho $f$ là một ánh xạ từ $U$ vào $F$. Ta ký hiệu bởi $D_{i} f(x_0)$ đạo hàm tại điểm $x_0^i$, nếu tồn tại, của ánh xạ $z_i \mapsto f(x_0^1, \ldots, z_i, \ldots, x_0^n)$ được xác định trong một lân cận của $x_0^i$ trong $E_i$ và nhận giá trị trong $F$. Đó là một phần tử của $\mathcal{L}(E_i; F)$, được gọi là *đạo hàm riêng thứ* $i$ *của* $f$ *tại* $x_0$. Nếu $f$ khả vi tại $x_0$, thì $n$ đạo hàm riêng tồn tại, và xác định $Df(x_0)$ bởi công thức:

$$
Df(x_0) \cdot h = \sum_{i=1}^{n} D_{i} f(x_0) \cdot h_i \quad \text{với } h = (h_1, \ldots, h_n) \text{ trong } E.
$$

1.6.3. Đặc biệt hơn, cho $E = K^n$. Nếu các đạo hàm riêng của $f$ tại $x_0$ tồn tại, người ta ký hiệu bởi $\partial_{i} f(x_0)$ phần tử $D_{i} f(x_0) \cdot 1$ của $F$. Ký hiệu sau đây thường được dùng; giả sử đã chọn một ký hiệu cho các hàm tọa độ trên $K^n$, chẳng hạn $u_i$ ký hiệu phép chiếu thứ $i$ của $K^n$ lên $K$. Khi đó người ta viết:

$$
\frac{\partial f}{\partial u_i}(x_0) \quad \text{hoặc} \quad \left. \frac{\partial f}{\partial u_i} \right|_{x = x_0}
$$

thay cho $\partial_{i} f(x_0)$.

1.6.4. Cho $E = K^n$ và $F = K^m$; giả sử rằng hàm $f = (f_1, \ldots, f_m)$ nhận giá trị trong $F$ khả vi tại điểm $x_0$ của $E$. Khi đó các đạo hàm riêng $a_{ji} = \partial_{i} f_j(x_0)$ tồn tại (chúng là các phần tử của $K$). Ma trận có $m$ hàng và $n$ cột tạo bởi các $a_{ji}$ (phần tử của hàng có chỉ số $j$ và của cột có chỉ số $i$) được gọi là *ma trận Jacobi* của $f$ tại $x_0$; đó là ma trận của ánh xạ tuyến tính $Df(x_0)$ từ $K^n$ vào $K^m$ đối với các cơ sở chính tắc của các không gian này.

### 1.7. Đạo hàm lặp

1.7.1. Cho $f$ là một hàm xác định trong một lân cận của một điểm $x_0$ của $E$, nhận giá trị trong $F$. Nếu $f$ khả vi trong một lân cận của $x_0$, đạo hàm của nó $Df$ là một ánh xạ từ một lân cận của $x_0$ vào không gian đa chuẩn $\mathcal{L}(E; F)$ của các ánh xạ tuyến tính liên tục từ $E$ vào $F$. Cho $p$ là một số nguyên $\geq 2$:

người ta nói rằng $f$ khả vi $p$ lần tại $x_0$ nếu $f$ khả vi trong một lân cận của $x_0$ và nếu đạo hàm của nó $Df$ khả vi $(p - 1)$ lần tại $x_0$. Khi đó người ta định nghĩa đạo hàm bậc $p$ của $f$ tại $x_0$: đó là ánh xạ $p$-tuyến tính liên tục $D^pf(x_0)$ từ $E^p$ vào $F$, được xác định bởi:

$$
D^pf(x_0) . (h_1, \ldots, h_p) = (D(D^{p-1}f)(x_0) . h_1) . (h_2, \ldots, h_p).
$$

Ta cũng đặt $D^0f = f$ và $D^1f = Df$. Nếu $f$ khả vi $p$ lần tại $x_0$ và nếu $q$ và $s$ là hai số nguyên sao cho $q + s = p$, với $s > 0$, thì $f$ khả vi $q$ lần trong một lân cận của $x_0$, hàm $D^qf$ (với giá trị trong $\mathcal{L}_q(E; F)$) khả vi $s$ lần tại $x_0$, và ta có:

$$
D^{q+s}f(x_0) . (h_1, \ldots, h_{q+s}) = (D^s(D^qf)(x_0) . (h_1, \ldots, h_s)) . (h_{s+1}, \ldots, h_{q+s})
$$

một quan hệ mà, do lạm dụng ký hiệu, được viết dưới dạng:

$$
D^{q+s}f = D^s D^qf.
$$

1.7.2. Cho $(E_i)_{1 \leq i \leq n}$ là các không gian con vectơ đóng của $E$, sao cho $E$ là tổng trực tiếp tôpô của các $E_i$. Khi đó ta định nghĩa, nếu tồn tại, đạo hàm riêng lặp $D_{i_1} \ldots D_{i_m}f$ của một ánh xạ $f$ từ một lân cận của $x_0 \in E$ vào $F$; đó là một ánh xạ đa tuyến tính liên tục từ

$$
E_{i_1} \times \cdots \times E_{i_m}
$$

vào $F$, được xác định bằng quy nạp theo số nguyên $m \geq 1$ như sau: nếu $D_{i_2} \ldots D_{i_m}f(x)$ tồn tại trong một lân cận của $x_0$ và có đạo hàm riêng đối với $E_{i_1}$, thì $D_{i_1} \ldots D_{i_m}f(x_0)$ được cho bởi:

$$
D_{i_1} \ldots D_{i_m}f(x_0) . (h_1, \ldots, h_m) = (D_{i_1}(D_{i_2} \ldots D_{i_m}f)(x_0) . h_1) . (h_2, \ldots, h_m)
$$

với $h_k \in E_{i_k}$.

Nếu $f$ khả vi $m$ lần tại $x_0$, thì đạo hàm riêng $D_{i_1} \ldots D_{i_m}f(x_0)$ tồn tại và bằng hạn chế của $D^m f(x_0)$ lên không gian con $E_{i_1} \times \cdots \times E_{i_m}$ của $E^m$. Do đó, $D^m f(x_0)$ được xác định hoàn toàn bởi các đạo hàm riêng lặp cấp $m$ tại $x_0$.

1.7.3. Giả sử rằng $E$ hữu hạn chiều và cho $(e_1, \ldots, e_n)$ là một cơ sở của $E$. Đặt $E_i = K e_i$ và cho $f$ là một ánh xạ từ một lân cận của $x_0$, với giá trị trong $F$. Nếu đạo hàm riêng $D_{i_1} \ldots D_{i_m}f(x_0)$ (với các ký hiệu của 1.7.2) tồn tại, ta đặt:

$$
\partial_{i_1} \ldots \partial_{i_m} f(x_0) = D_{i_1} \ldots D_{i_m} f(x_0) . (e_{i_1}, \ldots, e_{i_m}).
$$
