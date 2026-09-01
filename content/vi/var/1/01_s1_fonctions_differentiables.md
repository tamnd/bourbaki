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
content_sha256: 8865f88285001370ed01e279358f4f88307d493b26fb6e0ad813822feb3140c3
translated_from: content/en-mt/var/1/01_s1_fonctions_differentiables.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 0bf1c162534d51cfbef5c8dce9da23d0a8b404d715eeb87130dd56ee29844bbe
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-7f78aa23
glossary_version: 34
glossary_terms_sha256: a6eb52a6a6ec01ac4e9de499429dde56dd02b93efc81aaa6942898d7bd367a8b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. Hàm khả vi

Trong đoạn này, chữ E ký hiệu một không gian vectơ tôpô chuẩn được trên K; chữ F ký hiệu một không gian đa chuẩn tách được trên K.

### 1.1 Cấp tiếp xúc của hai hàm tại một điểm

1.1.1. Cho X là một không gian tôpô và $\theta$ là một hàm số dương xác định trong một lân cận của một điểm $x_0$ của X. Ta nói rằng một hàm $f$, xác định trong một lân cận của $x_0$ và có các giá trị trong F, là không đáng kể đối với $\theta$ tại $x_0$ nếu điều kiện sau được thỏa mãn:

Với mọi $\varepsilon > 0$ và với mọi chuẩn con liên tục $\gamma$ trên F, tồn tại một lân cận V của $x_0$ trên đó $f$ và $\theta$ được xác định và sao cho

$$
\| f(x) \|_{\gamma} \leq \varepsilon \theta(x) \quad \text{với mọi } x \in V.
$$

Để $f$ không đáng kể đối với $\theta$, chỉ cần điều kiện này được thỏa mãn đối với một họ các chuẩn con $\gamma$ xác định tôpô của F. Việc $f$ có hoặc không không đáng kể đối với $\theta$ tại $x_0$ chỉ phụ thuộc vào các mầm của $f$ và của $\theta$ tại $x_0$. Người ta ký hiệu bởi $o_{x_0}(\theta)$ (hoặc $o(\theta)$ khi không có sự nhập nhằng về $x_0$) tập hợp các mầm tại $x_0$ của các hàm không đáng kể đối với $\theta$ tại $x_0$: đó là một không gian con của không gian các mầm tại $x_0$ của các ánh xạ có giá trị trong F. Nếu $f$ không đáng kể đối với $\theta$, người ta viết, do lạm dụng ký hiệu, $f \in o_{x_0}(\theta)$ hoặc cũng viết $f(x) \in o(\theta(x))$ khi $x$ tiến tới $x_0$.

Nếu $f$ và $g$ là hai ánh xạ từ một lân cận của $x_0$ vào F, người ta cũng viết $f \equiv g \mod o(\theta)$ nếu $f - g$ là không đáng kể đối với $\theta$.

Giả sử rằng K bằng $\mathbf{R}$ hoặc $\mathbf{C}$ và rằng $x_0$ dính với tập hợp Y gồm các điểm của X tại đó $\theta$ được xác định và khác không. Khi đó quan hệ $f \in o(\theta)$ có nghĩa là $f(x)/\theta(x)$ tiến tới 0 khi $x$ tiến tới $x_0$ trong khi vẫn thuộc Y, và rằng $\theta(x) = 0$ kéo theo $f(x) = 0$.

1.1.2. Cho $f$ và $g$ là hai hàm có giá trị trong F, xác định trong một lân cận của một điểm $x_0$ của E. Nếu $m$ là một số nguyên dương, ta nói rằng $f$ và $g$ có tiếp xúc cấp $\geq m$ tại $x_0$ nếu ta có:

$$
f(x) - g(x) \in o(\| x - x_0 \|^{m}) \quad \text{khi } x \text{ tiến tới } x_0
$$

với bất kỳ chuẩn nào được chọn để xác định tôpô của E. Để được như vậy, chỉ cần quan hệ trước đó được kiểm chứng đối với một chuẩn xác định tôpô của E. Nếu điều này xảy ra, ta có $f(x_0) = g(x_0)$.

Nếu $f$ và $g$ nhận cùng một giá trị tại $x_0$, cận trên của các số nguyên $m$ (hữu hạn hoặc bằng $+\infty$) sao cho $f$ và $g$ có tiếp xúc cấp $\geq m$ tại $x_0$ được gọi là cấp tiếp xúc của $f$ và $g$ tại $x_0$.

1.1.3. Cấp tiếp xúc của $f$ và $g$ tại $x_0$ chỉ phụ thuộc vào các mầm của các hàm này tại điểm $x_0$. Do đó có thể nói đến cấp tiếp xúc của hai mầm $\varphi$ và $\psi$ của các ánh xạ từ E vào F tại điểm $x_0$. Quan hệ “ $\varphi$ và $\psi$ có tiếp xúc cấp $\geq m$ ” là một quan hệ tương đương tương thích với cấu trúc không gian vectơ.

### 1.2. Các hàm khả vi tại một điểm

1.2.1. Cho $f$ là một hàm được xác định trong một lân cận của điểm $x_0$ của E và nhận giá trị trong F. Ta nói rằng $f$ khả vi tại $x_0$ nếu tồn tại một hàm affine liên tục $v$ từ E vào F có tiếp xúc cấp $\geq 1$ với $f$ tại $x_0$. Ánh xạ $v$ này là duy nhất; tồn tại duy nhất một ánh xạ tuyến tính liên tục, ký hiệu bởi $Df(x_0)$, từ E vào F sao cho:

$$
v(x) = v(x_0) + Df(x_0) \cdot (x - x_0).
$$

Nếu chọn một chuẩn trên E, điều này tương đương với:

$$
f(x_0 + h) \equiv f(x_0) + Df(x_0) \cdot h \mod o(\|h\|) \quad \text{cho } h \text{ dần tới } 0,
$$

điều này cũng có thể được viết dưới dạng:

$$
\lim_{h \to 0, h \neq 0} \frac{\| f(x_0 + h) - f(x_0) - Df(x_0) \cdot h \|_\gamma}{\| h \|} = 0
$$

với mọi nửa chuẩn liên tục $\gamma$ trên F.

Phần tử $Df(x_0)$ của $\mathcal{L}(E, F)$ được gọi là đạo hàm của $f$ tại $x_0$. Đôi khi người ta viết $D_h f(x_0)$ cho $Df(x_0) \cdot h$; đây là một phần tử của F được xác định bởi quan hệ:

$$
D_h f(x_0) = \lim_{t \to 0, t \neq 0} \frac{f(x_0 + th) - f(x_0)}{t}.
$$

1.2.2. Ta nói rằng một hàm $f$ khả vi chặt tại $x_0$ nếu nó khả vi tại $x_0$ và nếu, với mọi chuẩn xác định tôpô của E, ta có quan hệ:

$$
f(y) - f(z) \equiv Df(x_0) \cdot (y - z) \mod o(\| y - z \| )
$$

khi $(y, z)$ dần tới $(x_0, x_0)$ trong $E \times E$. Đối với điều này, chỉ cần điều kiện này được thỏa mãn đối với một chuẩn xác định tôpô của E. Giả sử thêm rằng E và F là các không gian chuẩn; với mọi số $c > \| Df(x_0) \|$, khi đó tồn tại một lân cận V của $x_0$ sao cho $\| f(y) - f(z) \| \leq c. \| y - z \|$ đối với $y, z$ trong V; điều này kéo theo rằng $f$ liên tục đều trong V.

1.2.3. Việc một hàm $f$ khả vi hoặc khả vi chặt tại $x_0$ chỉ phụ thuộc vào mầm của $f$ tại $x_0$. Các mầm của các hàm khả vi tại $x_0$ tạo thành một không gian con vectơ $\mathcal{V}$ của không gian của tất cả các mầm, và ánh xạ $f \mapsto Df(x_0)$ của $\mathcal{V}$ vào $\mathcal{L}(E; F)$ là tuyến tính. Các mầm của các hàm khả vi chặt tại $x_0$ tạo thành một không gian con vectơ của $\mathcal{V}$.

1.2.4. Một hàm khả vi tại $x_0$ là liên tục tại $x_0$.

1.2.5. Khi $E = K$, ánh xạ $u \mapsto u(1)$ là một đẳng cấu của $\mathcal{L}(E; F)$ lên $F$; nếu hàm $f$ khả vi tại $x_0$, phần tử

$$
f'(x_0) = Df(x_0) \cdot 1
$$

chính là đạo hàm của $f$ tại $x_0$ theo nghĩa đã cho trong Fonct. Var. Réelle, chap. I, § 1, n° 6, nhận xét 2.

### 1.3. Hợp thành của các ánh xạ khả vi

1.3.1. Giả sử rằng F là chuẩn được. Cho $x_0 \in E$ và $y_0 \in F$, U là một lân cận của $x_0$ và V là một lân cận của $y_0$; cuối cùng, cho $f$ là một ánh xạ của U vào V, khả vi tại $x_0$, với $f(x_0) = y_0$. Nếu $g$ là một ánh xạ của V vào một không gian vectơ đa chuẩn tách được G, khả vi tại $y_0$, thì ánh xạ $g \circ f$ của U vào G là khả vi tại $x_0$, và ta có:

(1)
$$
D(g \circ f)(x_0) = Dg(y_0) \circ Df(x_0).
$$
Nếu $f$ và $g$ khả vi chặt, điều tương tự cũng đúng đối với $g \circ f$.

1.3.2. Cho $f$ là một ánh xạ được xác định trong một lân cận của một điểm $x_0$ của E và có các giá trị trong F, khả vi tại $x_0$; nếu $u$ là một ánh xạ tuyến tính liên tục của F vào một không gian vectơ đa chuẩn tách được G, thì hàm $u \circ f$ là khả vi tại $x_0$ và ta có:

(2)
$$
D(u \circ f)(x_0) = u \circ Df(x_0).
$$

1.3.3. Giả sử rằng F là tích của một họ $(F_i)_{i \in I}$ các không gian vectơ đa chuẩn tách được; với mỗi $i$ trong I, cho $f_i$ là một ánh xạ được xác định trong một lân cận U của một điểm $x_0$ của E và có các giá trị trong F và cho $f = (f_i)_{i \in I}$. Để $f$ khả vi (tương ứng, khả vi chặt) tại $x_0$, điều kiện cần và đủ là tất cả các $f_i$ đều có tính chất đó; ta có:

(3)
$$
D_h f(x_0) = (D_h f_i(x_0))_{i \in I} \quad \text{với mọi } h \text{trong } E.
$$

1.3.4. Nếu $E = K$, ta có thể thay $Df(x_0)$ bởi $f'(x_0)$ và $D_h f_i(x_0)$ bởi $f'_i(x_0)$ trong các công thức (1) và (3).

### 1.4. Tích của các ánh xạ khả vi

1.4.1. Cho $F_1, \ldots, F_m$ là các không gian đa chuẩn tách được và $u$ là một ánh xạ $m$-tuyến tính liên tục của $F_1 \times \cdots \times F_m$ vào $F$. Cho $U$ là một lân cận của một điểm $x_0$ của $E$, và cho $f_i$ là một ánh xạ của $U$ vào $F_i$ (với $1 \leq i \leq m$). Nếu các $f_i$ khả vi (tương ứng, khả vi chặt) tại $x_0$, thì điều tương tự cũng đúng đối với $u(f_1, \ldots, f_m) = g$, và ta có:

(4) $D_hg(x_0) = \sum_{j=1}^m u(f_1(x_0), \ldots, D_hf_j(x_0), \ldots, f_m(x_0))$ với $h$ trong $E$,

sẽ được viết ngắn gọn hơn:

(5) $Dg = \sum_{j=1}^m u(f_1, \ldots, Df_j, \ldots, f_m)$.

Đặc biệt, với $m = 2$, ta có:

(6) $Du(f_1, f_2) = u(Df_1, f_2) + u(f_1, Df_2)$.

Với $m = 1$, điều này cho lại 1.3.2.

1.4.2. Khi $E = K$, ta có thể thay $Dg$ bởi $g'$ và $Df_j$ bởi $f'_j$ trong các công thức (4) đến (6).

### 1.5. Các biến thể đầu tiên của định lý hàm ẩn

Giả sử rằng $E$ và $F$ là các không gian Banach, và cho $x_0$ là một điểm của $E$, $U$ là một lân cận của $x_0$ và $f$ là một ánh xạ của $U$ vào $F$. Giả sử thêm rằng $f$ khả vi chặt tại $x_0$.

1.5.1. Nếu $Df(x_0)$ là một đẳng cấu của $E$ lên $F$, tồn tại một lân cận mở $U_0$ của $x_0$ được chứa trong $U$ và một lân cận mở $V_0$ của $f(x_0)$ sao cho $f|U_0$ là một đồng phôi của $U_0$ lên $V_0$. Ánh xạ $g : V_0 \to U_0$ nghịch đảo của $f|U_0$ là khả vi chặt tại điểm $f(x_0)$, và ta có:

$$
Dg(f(x_0)) = Df(x_0)^{-1}.
$$

1.5.2. Nếu $Df(x_0)$ là một ánh xạ toàn ánh của $E$ lên $F$, tồn tại một lân cận mở $U_0$ của $x_0$ được chứa trong $U$, sao cho $f|U_0$ là một ánh xạ mở.

1.5.3. Nếu $Df(x_0)$ là đơn ánh và có ảnh đóng, tồn tại một lân cận đóng $U_0$ của $x_0$ được chứa trong $U$, sao cho $f|U_0$ là một phép đồng phôi của $U_0$ lên một tập con đóng của $F$.

### 1.6. Các đạo hàm riêng

1.6.1. Cho $f$ là một hàm xác định trong một lân cận $U$ của điểm $x_0$ của $E$ và có các giá trị trong $F$. Cho $X$ là một không gian vectơ và $V$ là tập hợp các điểm $x$ của $X$ sao cho $x_0 + x \in U$; đặt $g(x) = f(x_0 + x)$ với $x \in V$. Ta nói rằng $f$ có một *đạo hàm riêng theo* $X$ *tại* $x_0$ nếu $g$ có một đạo hàm tại $0$; đạo hàm này được ký hiệu là $D_X f(x_0)$; nó là một ánh xạ tuyến tính liên tục của $X$ vào $F$. Nếu $f$ khả vi tại $x_0$, nó có một đạo hàm riêng theo $X$ tại $x_0$, và đạo hàm riêng này là hạn chế của $Df(x_0)$ lên $X$.

1.6.2. Giả sử rằng $E$ là tích của một họ hữu hạn các không gian vectơ định chuẩn $E_i$ ($1 \leq i \leq n$) được đồng nhất một cách chính tắc với các không gian con của $E$; cho $x_0 = (x_0^1, \ldots, x_0^n)$ trong $E$ và cho $U$ là một lân cận của $x_0$ trong $E$; cuối cùng cho $f$ là một ánh xạ của $U$ vào $F$. Người ta ký hiệu $D_{i} f(x_0)$ là đạo hàm tại điểm $x_0^i$, nếu nó tồn tại, của ánh xạ $z_i \mapsto f(x_0^1, \ldots, z_i, \ldots, x_0^n)$ xác định trong một lân cận của $x_0^i$ trong $E_i$ và có các giá trị trong $F$. Nó là một phần tử của $\mathcal{L}(E_i; F)$ được gọi là *đạo hàm riêng thứ $i$ của* $f$ *tại* $x_0$. Nếu $f$ khả vi tại $x_0$, $n$ đạo hàm riêng tồn tại, và xác định $Df(x_0)$ bởi công thức:

$$
Df(x_0) \cdot h = \sum_{i=1}^{n} D_{i} f(x_0) \cdot h_i \quad \text{cho } h = (h_1, \ldots, h_n) \text{ trong } E.
$$

1.6.3. Cụ thể hơn, cho $E = K^n$. Nếu các đạo hàm riêng của $f$ tại $x_0$ tồn tại, người ta ký hiệu phần tử $D_{i} f(x_0) \cdot 1$ của $F$ bởi $\partial_{i} f(x_0)$. Ký hiệu sau đây thường được dùng; giả sử rằng một ký hiệu đã được chọn cho các hàm tọa độ trên $K^n$, chẳng hạn $u_i$ ký hiệu phép chiếu thứ $i$ của $K^n$ lên $K$. Khi đó người ta viết:

$$
\frac{\partial f}{\partial u_i}(x_0) \quad \text{hoặc} \quad \left. \frac{\partial f}{\partial u_i} \right|_{x = x_0}
$$

thay cho $\partial_{i} f(x_0)$.

1.6.4. Cho $E = K^n$ và $F = K^m$; giả sử rằng hàm $f = (f_1, \ldots, f_m)$ có giá trị trong $F$ khả vi tại điểm $x_0$ của $E$. Khi đó các đạo hàm riêng $a_{ji} = \partial_{i} f_j(x_0)$ tồn tại (chúng là các phần tử của $K$). Ma trận có $m$ hàng và $n$ cột được tạo bởi các $a_{ji}$ (phần tử ở hàng có chỉ số $j$ và cột có chỉ số $i$) được gọi là *ma trận Jacobian* của $f$ tại $x_0$; đó là ma trận của ánh xạ tuyến tính $Df(x_0)$ từ $K^n$ vào $K^m$ đối với các cơ sở chính tắc của các không gian này.

### 1.7. Các đạo hàm lặp

1.7.1. Cho $f$ là một hàm được xác định trong một lân cận của một điểm $x_0$ của $E$, có giá trị trong $F$. Nếu $f$ khả vi trong một lân cận của $x_0$, đạo hàm của nó $Df$ là một ánh xạ từ một lân cận của $x_0$ vào không gian đa chuẩn $\mathcal{L}(E; F)$ của các ánh xạ tuyến tính liên tục từ $E$ vào $F$. Cho $p$ là một số nguyên $\geq 2$:

người ta nói rằng $f$ khả vi $p$ lần tại $x_0$ nếu $f$ khả vi trong một lân cận của $x_0$ và nếu đạo hàm của nó $Df$ khả vi $(p - 1)$ lần tại $x_0$. Khi đó người ta định nghĩa đạo hàm thứ $p$ của $f$ tại $x_0$: đó là ánh xạ $p$-tuyến tính liên tục $D^pf(x_0)$ từ $E^p$ vào $F$, được xác định bởi:

$$
D^pf(x_0) . (h_1, \ldots, h_p) = (D(D^{p-1}f)(x_0) . h_1) . (h_2, \ldots, h_p).
$$

Ta cũng đặt $D^0f = f$ và $D^1f = Df$. Nếu $f$ khả vi $p$ lần tại $x_0$ và nếu $q$ và $s$ là hai số nguyên sao cho $q + s = p$, với $s > 0$, thì $f$ khả vi $q$ lần trong một lân cận của $x_0$, hàm $D^qf$ (với các giá trị trong $\mathcal{L}_q(E; F)$) khả vi $s$ lần tại $x_0$, và ta có:

$$
D^{q+s}f(x_0) . (h_1, \ldots, h_{q+s}) = (D^s(D^qf)(x_0) . (h_1, \ldots, h_s)) . (h_{s+1}, \ldots, h_{q+s})
$$

một quan hệ mà, do lạm dụng ký hiệu, được viết dưới dạng:

$$
D^{q+s}f = D^s D^qf.
$$

1.7.2. Cho $(E_i)_{1 \leq i \leq n}$ là các không gian con vectơ đóng của $E$, sao cho $E$ là tổng trực tiếp tôpô của các $E_i$. Khi nó tồn tại, ta định nghĩa đạo hàm riêng lặp $D_{i_1} \ldots D_{i_m}f$ của một ánh xạ $f$ từ một lân cận của $x_0 \in E$ vào $F$; đó là một ánh xạ đa tuyến liên tục từ

$$
E_{i_1} \times \cdots \times E_{i_m}
$$

vào $F$, được xác định bằng quy nạp theo số nguyên $m \geq 1$ như sau: nếu $D_{i_2} \ldots D_{i_m}f(x)$ tồn tại trong một lân cận của $x_0$ và có một đạo hàm riêng theo $E_{i_1}$, thì $D_{i_1} \ldots D_{i_m}f(x_0)$ được cho bởi:

$$
D_{i_1} \ldots D_{i_m}f(x_0) . (h_1, \ldots, h_m) = (D_{i_1}(D_{i_2} \ldots D_{i_m}f)(x_0) . h_1) . (h_2, \ldots, h_m)
$$

với $h_k \in E_{i_k}$.

Nếu $f$ khả vi $m$ lần tại $x_0$, thì đạo hàm riêng $D_{i_1} \ldots D_{i_m}f(x_0)$ tồn tại và bằng hạn chế của $D^m f(x_0)$ lên không gian con $E_{i_1} \times \cdots \times E_{i_m}$ của $E^m$. Do đó, $D^m f(x_0)$ được xác định hoàn toàn bởi các đạo hàm riêng lặp cấp $m$ tại $x_0$.

1.7.3. Giả sử rằng $E$ là hữu hạn chiều và cho $(e_1, \ldots, e_n)$ là một cơ sở của $E$. Đặt $E_i = K e_i$ và cho $f$ là một ánh xạ từ một lân cận của $x_0$, với các giá trị trong $F$. Nếu đạo hàm riêng $D_{i_1} \ldots D_{i_m}f(x_0)$ (với các ký hiệu của 1.7.2) tồn tại, ta đặt:

$$
\partial_{i_1} \ldots \partial_{i_m} f(x_0) = D_{i_1} \ldots D_{i_m} f(x_0) . (e_{i_1}, \ldots, e_{i_m}).
$$
