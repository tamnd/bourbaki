---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 2
section_title: Fonctions différentiables réelles
lang: vi
source: var-fr
pdf_pages: 0015-0019
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions dérivables en un point
      page: 0
      pdf_page: 15
    - "no": 2
      title: Le théorème des accroissements finis
      page: 0
      pdf_page: 15
    - "no": 3
      title: Fonctions de classe $C^r$ ($r \neq \omega$)
      page: 0
      pdf_page: 16
    - "no": 4
      title: Dérivées des fonctions de classe $C^r$
      page: 0
      pdf_page: 17
    - "no": 5
      title: Formule de Taylor
      page: 0
      pdf_page: 17
    - "no": 6
      title: Critères de dérivabilité
      page: 0
      pdf_page: 19
statements: 0
exercises: 0
content_sha256: 0f192b690e3e38950cb10334485d6a3c0684dac06bb908f1ac2492489d10785e
translated_from: content/en-mt/var/1/02_s2_fonctions_differentiables_reelles.md
source_lang: en-mt
translation_method: machine
source_content_sha256: df93b3eccc63eeaac231d190cc93798443c258ceb9af58b543930f3e95d373a4
translation_model: gpt-5-mini
translation_run: translate-vi-c4b9425c
glossary_version: 34
glossary_terms_sha256: 3ccb4099d03b5d9542c1fa94327ed2f1ee6186c433d8c8c8eb64474a6e93d7bb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. Các hàm khả vi thực

Trong đoạn này, giả sử rằng K = R. Chữ E ký hiệu một không gian vectơ chuẩn trên R; chữ F ký hiệu một không gian vectơ tôpô lồi địa phương tách được trên R.

### 2.1. Các hàm khả vi tại một điểm

2.1.1. Cho f là một hàm xác định trong một lân cận của một điểm x_0 của E và có các giá trị trong F. Cho u là một phần tử của không gian $\mathcal{L}(E; F)$ gồm các ánh xạ tuyến tính liên tục từ E vào F. Để f khả vi tại x_0 và nhận u tại đó làm đạo hàm, điều kiện cần và đủ là có
$$
\lim_{h \to 0, h \neq 0} \frac{f(x_0 + h) - f(x_0) - u(h)}{\|h\|} = 0.
$$

2.1.2. Để f khả vi chặt tại x_0, điều kiện cần và đủ là có
$$
\lim_{(h, k) \to (0, 0), h \neq k} \frac{f(x_0 + h) - f(x_0 + k) - Df(x_0) \cdot (h - k)}{\|h - k\|} = 0.
$$

2.1.3. Cho F_1 và F_2 là hai không gian lồi địa phương tách được và cho u là một ánh xạ song tuyến tính từ F_1 × F_2 vào F, thỏa mãn điều kiện liên tục sau:
(SC) Nếu ((a_n, b_n)) là một dãy các phần tử của F_1 × F_2 hội tụ đến một phần tử (a, b) ∈ F_1 × F_2, thì dãy (u(a_n, b_n)) hội tụ đến u(a, b) trong F.

Cho f_i (với i = 1, 2) là một ánh xạ từ một lân cận của một điểm x_0 của E vào F_i. Nếu f_1 và f_2 khả vi tại x_0, thì u(f_1, f_2) khả vi tại x_0 và ta có:
$$
D(u(f_1, f_2))(x_0) \cdot h = u(Df_1(x_0) \cdot h, f_2(x_0)) + u(f_1(x_0), Df_2(x_0) \cdot h)
$$
với mọi $h \in E$.

### 2.2. Định lý giá trị trung bình

2.2.1. Cho x, y thuộc E, và cho [x, y] là đoạn đóng nối hai điểm này. Hơn nữa, cho f là một ánh xạ từ một lân cận của [x, y] vào không gian F, khả vi tại mọi điểm của [x, y]. Khi đó f(x) − f(y) thuộc bao lồi đóng của tập hợp các điểm Df(z) · (x − y) với z thuộc [x, y].

2.2.2. Cho U là một tập hợp mở liên thông của E, và cho f là một ánh xạ từ U vào

F, nhận đạo hàm không tại mọi điểm của U; khi đó $f$ là hằng trong U.

2.2.3. Cho U là một tập hợp mở *lồi* của E, và cho $f$ là một ánh xạ từ U vào F, khả vi tại mọi điểm của U. Cho một bán chuẩn liên tục $\gamma$ trên F và một số thực $M \geqslant 0$, các điều kiện sau là tương đương:
    (i) Với mọi $x$ trong U, ta có $\|Df(x)\|_{\gamma} \leqslant M$.
    (ii) Với mọi $x$ và mọi $y$ trong U, ta có $\|f(x) - f(y)\|_{\gamma} \leqslant M \cdot \|x - y\|$.

2.2.4. Cho U là một lân cận của một điểm $x_0$ của E và cho $f$ là một hàm xác định trong phần bù của $x_0$ trong U, với các giá trị trong F. Giả sử rằng $f$ nhận một đạo hàm $Df(x)$ tại mọi điểm $x$ của U, $x \neq x_0$, và rằng hàm $x \mapsto Df(x)$ nhận một giới hạn $D_0$ khi $x$ tiến tới $x_0$. Khi đó, nếu $\dim(E) \geqslant 2$, $f$ có một giới hạn tại $x_0$ và hàm $f$ được mở rộng bởi tính liên tục tới toàn bộ U là khả vi với đạo hàm $D_0$ tại $x_0$; điều tương tự cũng đúng nếu $\dim(E) = 1$ và giả sử rằng $f$ có một giới hạn tại $x_0$.

### 2.3. Các hàm thuộc lớp $C^r$ ($r \neq \omega$)

2.3.1. Cho U là một tập hợp mở của E và cho $f$ là một ánh xạ từ U vào F. Ta định nghĩa quan hệ “$f$ thuộc lớp $C^r$” (với $r \in \mathbf{N}$) bằng quy nạp theo $r$ theo cách sau:
    1) $f$ thuộc lớp $C^0$ khi và chỉ khi nó liên tục;
    2) nếu $r$ là một số nguyên $\geqslant 1$, hàm $f$ thuộc lớp $C^r$ khi và chỉ khi nó khả vi tại mọi điểm của U và ánh xạ đạo hàm $Df$ từ U vào $\mathcal{L}(E; F)$ thuộc lớp $C^{r-1}$.

Các hàm thuộc lớp $C^r$ còn được gọi là *các hàm khả vi liên tục r lần*.

Ta nói rằng $f$ *thuộc lớp $C^{\infty}$* (hay *khả vi vô hạn*) nếu nó thuộc lớp $C^r$ với mọi số nguyên $r$.

Nếu $f$ thuộc lớp $C^r$ trong U, thì $f$ khả vi $p$ lần với mọi số nguyên $p \leqslant r$ và hàm $D^p f$ thuộc lớp $C^{r-p}$.

2.3.2. Các ánh xạ thuộc lớp $C^r$ từ một tập hợp mở U của E vào F tạo thành một không gian con vectơ $\mathcal{C}^r(U; F)$ của không gian gồm tất cả các ánh xạ từ U vào F. Ta có $\mathcal{C}^s(U; F) \subset \mathcal{C}^r(U; F)$ với $s \geqslant r$.

2.3.3. Để một hàm $f$ thuộc lớp $C^1$ trong một tập hợp mở U của E, điều kiện cần và đủ là nó khả vi nghiêm ngặt tại mọi điểm của U.

Nếu E là một tích của các không gian định chuẩn $E_i$, một ánh xạ $f$ từ một tập hợp mở V của E vào F thuộc lớp $C^r$ khi và chỉ khi $f$ có các đạo hàm riêng lặp liên tục $D_{i_1} \ldots D_{i_m} f$ với mọi số nguyên $m \leqslant r$.

2.3.4. Cho G là một không gian định chuẩn và cho U là một tập hợp mở của E. Cho V là một tập hợp mở của G, $g \in \mathcal{C}^r(U; G)$ và $f \in \mathcal{C}^r(V; F)$. Nếu $g(U) \subset V$, ánh xạ $f \circ g$ từ U vào F thuộc lớp $C^r$.

Cho $F_1$ và $F_2$ là hai không gian lồi địa phương tách được và cho $u$ là một ánh xạ song tuyến tính từ $F_1 \times F_2$ vào F, nửa liên tục đều đối với tập hợp các phần bị chặn của $F_1$ (tương ứng $F_2$) (Esp. Vect. Top., ch. III, § 4, n° 2). Cho U là một tập hợp mở của E và $f_i \in \mathcal{C}^r(U; F_i)$ (với $i = 1, 2$). Khi đó hàm $u(f_1, f_2)$ thuộc về $\mathcal{C}^r(U; F)$. Nếu E có số chiều hữu hạn, chỉ cần giả sử rằng $u$ thỏa mãn điều kiện (SC) của n° 2.1.3.

2.3.5. Nếu E là một tích của các không gian định chuẩn $E_i$ ($1 \leq i \leq n$) và nếu $f$ là một ánh xạ $n$-tuyến tính liên tục từ E vào F, thì $f$ thuộc lớp $C^\infty$ và ta có $D^p f = 0$ với $p \geq n + 1$.

2.3.6. Giả sử rằng E và F là các không gian Banach. Cho $f$ là một hàm thuộc lớp $C^r$ (với $r \geq 1$) được xác định trong một lân cận của một điểm $x_0$ của E và có các giá trị trong F. Cho $y_0 = f(x_0)$ và giả sử rằng $Df(x_0)$ là một đẳng cấu của E lên F. Khi đó $f$ cảm sinh một đồng phôi $g$ của một lân cận của $x_0$ lên một lân cận của $y_0$ (1.5) và ánh xạ nghịch đảo của $g$ thuộc lớp $C^r$ trong một lân cận của $y_0$.

### 2.4. Các đạo hàm của các hàm thuộc lớp $C^r$

2.4.1. Cho $f$ là một ánh xạ thuộc lớp $C^r$ của một tập mở U của E vào F. Với mọi $x \in U$, và mọi số nguyên $s$ với $s \leq r$, ánh xạ đa tuyến tính $D^s f(x)$ là đối xứng.

2.4.2. Giả sử thêm rằng E là hữu hạn chiều và cho $(e_1, \ldots, e_n)$ là một cơ sở của E. Các đạo hàm riêng $\partial_{i_1} \ldots \partial_{i_s} f$ phụ thuộc đối xứng vào các chỉ số $i_1, \ldots, i_s$. Gọi $\alpha_k$ là số lần chỉ số $k$ xuất hiện trong dãy $i_1, \ldots, i_s$ và gọi $\alpha = (\alpha_1, \ldots, \alpha_n)$. Khi đó ta đặt:

$$
\partial^{\alpha} f = \partial_1^{\alpha_1} \ldots \partial_n^{\alpha_n} f = \partial_{i_1} \ldots \partial_{i_s} f
$$

Khi các tọa độ đối với cơ sở $(e_1, \ldots, e_n)$ được ký hiệu bởi $x_1, \ldots, x_n$, ta cũng viết $\partial^{\alpha} f$ dưới dạng:

$$
\frac{\partial^{|\alpha|} f}{\partial x_1^{\alpha_1} \ldots \partial x_n^{\alpha_n}}
$$

### 2.5. Công thức Taylor

2.5.1. Cho $r$ là một số nguyên $\geq 1$ và cho $f$ là một ánh xạ thuộc lớp $C^r$ của một tập mở U của E vào F. Với $x \in U$, $h \in E$ và $p \leq r$, ta quy ước viết $D^p f(x_0) \cdot h^p$ thay cho $D^p f(x_0) \cdot (h, \ldots, h)$. Nếu đoạn $[x, x + h]$ được chứa trong U, ta có công thức (“công thức Taylor”):

$$
f(x + h) = \sum_{p=0}^{r-1} \frac{1}{p!} D^p f(x) \cdot h^p + v_r(x; h)
$$

trong đó “số dư” $v_r(x; h)$ được cho bởi:

$$
v_r(x; h) = \int_0^1 \frac{(1-t)^{r-1}}{(r-1)!} D^r f(x + th) \cdot h^r \, dt
$$

Ta có:

$$
v_r(x; h) \equiv \frac{1}{r!} D^r f(x) \cdot h^r \quad \text{mod } o(\|h\|^r) \quad \text{khi } h \text{ tiến tới } 0
$$

và

$$
f(x + h) \equiv \sum_{p=0}^r \frac{1}{p!} D^p f(x) \cdot h^p \quad \text{mod } o(\|h\|^r)
$$

khi $h$ tiến tới không.

2.5.2. Giả sử thêm rằng $\gamma$ là một nửa chuẩn liên tục trên F; nếu ta có $\|D^r f(z)\|_\gamma \leq M$ với mọi điểm $z$ của đoạn $[x, x + h]$, thì ta có:

$$
\|v_r(x; h)\|_\gamma \leq \frac{M}{r!} \|h\|^r
$$

2.5.3. Giả sử thêm rằng $E = \mathbf{R}^n$. Khi đó ta có:

$$
f(x + h) \equiv \sum_{|\alpha| \leq r} \Delta^\alpha f(x) h^\alpha \quad \text{mod } o(\|h\|^r) \quad \text{khi } h \text{ tiến tới } 0
$$

với:

$$
\Delta^\alpha f(x) = \frac{1}{\alpha!} \partial^\alpha f(x)
$$

2.5.4. Cho $f$ và $g$ là hai hàm thuộc lớp $C^r$ trên một tập con mở $U$ của $E$, với các giá trị trong $F$. Để $f$ và $g$ có tại một điểm $x$ của $U$ một sự tiếp xúc cấp $\geq r$, điều kiện cần và đủ là có $D^p f(x) = D^p g(x)$ với mọi số nguyên $p$ thỏa mãn $0 \leq p \leq r$. Khi $E$ là hữu hạn chiều, điều này tương đương với việc nói rằng các đạo hàm riêng lặp của cấp $\leq r$ của $f$ và $g$ (đối với một cơ sở của $E$) bằng nhau tại điểm $x$.

2.5.5. Cho $U$ là một tập con mở của $E \times \mathbf{R}^n$ có dạng $V \times I_1 \times \cdots \times I_n$, trong đó $V$ là một tập con mở của $E$ và $I_1, \ldots, I_n$ là các khoảng mở của $\mathbf{R}$ chứa 0. Đặt $U_0 = V$ và $U_j = V \times I_1 \times \cdots \times I_j$ với $1 \leq j \leq n$. Cho một hàm $f \in \mathcal{C}^r(U; F)$ (với $1 \leq r \leq \infty$), tồn tại một và chỉ một dãy các hàm $f_j \in \mathcal{C}^{r-1}(U_j; F)$ (với $0 \leq j \leq n$) sao cho:

$$
f(x, t_1, \ldots, t_n) = f_0(x) + \sum_{j=1}^n t_j f_j(x, t_1, \ldots, t_j)
$$

với $x \in V$ và $t_j \in I_j$. Ta có:

$$
f_0(x) = f(x, 0, \ldots, 0)
$$
$$
f_j(x, t_1, \ldots, t_j) = \int_0^1 \partial_j f(x, t_1, \ldots, t_{j-1}, t_j u, 0, \ldots, 0) du
$$

với $1 \leq j \leq n$. Trong công thức cuối này, $\partial_j f$ ký hiệu đạo hàm riêng thứ $j$ của hàm $(t_1, \ldots, t_n) \mapsto f(x, t_1, \ldots, t_n)$.

### 2.6. Các tiêu chuẩn về khả vi

2.6.1. Giả sử rằng $F$, ngoài tôpô $\mathcal{T}$ của nó, còn được trang bị một tôpô kém mịn hơn $\mathcal{T}'$, tôpô này cũng làm cho $F$ trở thành một không gian lồi địa phương tách được. Hơn nữa, giả sử rằng $\mathcal{T}$ và $\mathcal{T}'$ thỏa mãn điều kiện sau:
(S) Với mỗi lân cận $V$ của 0 đối với tôpô $\mathcal{T}$, tồn tại một lân cận $W$ của 0 đối với $\mathcal{T}$ sao cho bao lồi đóng đối với $\mathcal{T}'$ của mỗi tập con compact đối với $\mathcal{T}$ của $W$ được chứa trong $V$.

Cho $f$ là một ánh xạ từ một tập hợp mở $U$ của $E$ vào $F$. Giả sử rằng $f$ thuộc lớp $C^r$ ($1 \leq r \leq \infty$) khi $F$ được trang bị tôpô $\mathcal{T}'$, rằng $D^m f(x)$ là, với mọi $x$ của $U$, và mọi số nguyên $m \leq r$, một ánh xạ đa tuyến tính liên tục từ $E^m$ vào $F$ được trang bị tôpô $\mathcal{T}$ và rằng ánh xạ $x \mapsto D^m f(x)$ là liên tục từ $U$ vào $\mathcal{L}_m(E; F)$ ($F$ được trang bị tôpô $\mathcal{T}$). Khi đó $f$ thuộc lớp $C^r$ khi $F$ được trang bị tôpô $\mathcal{T}$ và các đạo hàm $D^m f$ của nó là như nhau đối với $\mathcal{T}$ và đối với $\mathcal{T}'$.

Điều kiện (S) đặc biệt được thỏa mãn nếu tồn tại một hệ cơ bản các lân cận của 0 đối với tôpô $\mathcal{T}$ đóng đối với tôpô $\mathcal{T}'$: đây là trường hợp nếu đối ngẫu của $F$ được trang bị $\mathcal{T}$ đồng nhất với đối ngẫu của $F$ được trang bị $\mathcal{T}'$. Điều kiện (S) cũng được thỏa mãn nếu $F$ được trang bị tôpô $\mathcal{T}$ là gần đầy đủ (*Esp. Vect. Top.*, Ch. III, § 2, No. 5).

2.6.2. Cho $f$ là một ánh xạ từ một tập hợp mở $U$ của $E$ vào $F$. Nếu $f$ thuộc lớp $C^r$ (với $0 \leq r \leq \infty$), các hàm vô hướng $u \circ f$ thuộc lớp $C^r$ với mọi dạng tuyến tính liên tục $u$ trên $F$. Ngược lại nếu $F$ là gần đầy đủ và nếu các hàm $u \circ f$ thuộc lớp $C^{r+1}$ với mọi $u \in F'$, thì $f$ thuộc lớp $C^r$.
