---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 1
section_title: Compléments d’algèbre linéaire
lang: vi
source: alg-x-fr
book_pages: A X.168-A X.173
pdf_pages: 0007-0029, 0174-0179
extraction: ocr
subsections:
    - "no": 1
      title: Diagrammes commutatifs
      page: 0
      pdf_page: 7
    - "no": 2
      title: Le diagramme du serpent
      page: 3
      pdf_page: 9
    - "no": 3
      title: Modules plats
      page: 8
      pdf_page: 14
    - "no": 4
      title: Modules de présentation finie
      page: 10
      pdf_page: 16
    - "no": 5
      title: Homomorphismes d’un module de présentation finie
      page: 12
      pdf_page: 18
    - "no": 6
      title: Structure des modules plats
      page: 13
      pdf_page: 19
    - "no": 7
      title: Modules injectifs
      page: 15
      pdf_page: 21
    - "no": 8
      title: Modules cogénérateurs injectifs
      page: 18
      pdf_page: 24
    - "no": 9
      title: Enveloppes injectives
      page: 19
      pdf_page: 25
    - "no": 10
      title: Structure des modules injectifs
      page: 22
      pdf_page: 28
statements: 55
exercises: 17
content_sha256: 49e7436011e7f32af9addf980a5e88602087a1f4ed9ad4492e141aa91ddd8825
translated_from: content/en-mt/alg/X/01_s1_complements_d_algebre_lineaire.md
source_lang: en-mt
translation_method: machine
source_content_sha256: f55d142614aa6d7f23af6851df91ee735ca380fab8afe681cb5dd6ea12aba4d1
translation_model: gpt-5.4
translation_run: translate-vi-ee54513d
glossary_version: 34
glossary_terms_sha256: 914d953be395edd5935ff877314a76fcec80f529f11b8efd3106a9d0a40e5ac1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. BỔ SUNG ĐẠI SỐ TUYẾN TÍNH

Trong đoạn này, chữ cái $\mathbf{A}$ ký hiệu một vành. Trừ khi nói rõ ngược lại, mọi môđun được xét đều là môđun trái, mọi iđêan được xét đều là iđêan trái.

Các định nghĩa và kết quả áp dụng được cho các môđun phải, bằng cách xét chúng như các môđun trái trên vành đối.

Nếu $\mathbf{M}$ là một $\mathbf{A}$-môđun và nếu $a \in \mathbf{A}$, ta ký hiệu bởi $a_M$ phép vị tự $x \mapsto ax$ của $\mathbf{M}$. Do đó ta có $1_M = \mathrm{Id}_M$ (ánh xạ đồng nhất của $\mathbf{M}$); khi không thể có sự nhập nhằng nào, đôi khi người ta chỉ viết đơn giản $1$ thay cho $1_M$.

Sau cùng, ta ký hiệu bởi $0$ một $\mathbf{A}$-môđun rút gọn vào phần tử đơn vị của nó, được chọn một lần cho tất cả (xem II, p. 8).

### 1. Các biểu đồ giao hoán

Chẳng hạn, cho B, C, D, E, F là năm tập hợp, và cho $f$ là một ánh xạ từ E vào F, $g$ một ánh xạ từ B vào C, $h$ một ánh xạ từ D vào E, $u$ một ánh xạ từ B vào D và $v$ một ánh xạ từ C vào E. Để tóm tắt một tình huống như vậy, người ta thường dùng các biểu đồ; chẳng hạn, tình huống nói trên sẽ được tóm tắt bởi biểu đồ sau (E, II, p. 14):

$$
\begin{array}{ccc}
B & \xrightarrow{g} & C \\
u \downarrow & & v \downarrow \\
D & \xrightarrow{h} & E \xrightarrow{f} F .
\end{array}
$$

Trong một biểu đồ như vậy, nhóm dấu $E \xrightarrow{f} F$ sơ đồ hóa việc $f$ là một ánh xạ từ E vào F. Khi không thể có sự nhập nhằng nào về $f$, chữ $f$ được lược bỏ, và người ta chỉ đơn giản viết $E \to F$.

Khi B, C, D, E, F là các nhóm (tương ứng, các $\mathbf{A}$-môđun) và $f, g, h, u, v$ là các đồng cấu nhóm (tương ứng, các đồng cấu A-môđun), nói gọn rằng biểu đồ (1) là một *biểu đồ các nhóm* (tương ứng, các A-môđun).

Về nguyên tắc, một biểu đồ không phải là một đối tượng toán học, mà chỉ là một *hình*, nhằm làm dễ việc đọc một lập luận. Trong thực hành, các biểu đồ thường được dùng như những *ký hiệu viết tắt*, giúp tránh phải gọi tên mọi tập hợp và mọi ánh xạ mà người ta muốn xét; do đó người ta nói “xét biểu đồ (1)” thay cho việc nói: “cho B, C, D, E, F là năm tập hợp... và $v$ là một ánh xạ từ C vào E”; xem chẳng hạn mệnh đề 1 của No. 2.

Chẳng hạn, xét biểu đồ sau:

$$
\begin{array}{ccccccc}
B & \xrightarrow{\ f\ } & C & \xrightarrow{\ g\ } & D & \xrightarrow{\ h\ } & E\\
{\scriptstyle b}\downarrow && {\scriptstyle c}\downarrow && {\scriptstyle d}\downarrow && {\scriptstyle e}\downarrow\\
B' & \xrightarrow{\ f'\ } & C' & \xrightarrow{\ g'\ } & D' & \xrightarrow{\ h'\ } & E'
\end{array}
\tag{2}
$$

Với mỗi đường đi gồm một số nhất định các đoạn của biểu đồ được đi theo chiều chỉ bởi các mũi tên, ta cho tương ứng một ánh xạ từ tập hợp được biểu diễn bởi gốc của đoạn thứ nhất vào tập hợp được biểu diễn bởi đầu mút của đoạn cuối cùng, tức là hợp thành của các ánh xạ được biểu diễn bởi các đoạn khác nhau đã đi qua. Với mỗi đỉnh của biểu đồ, chẳng hạn C, ta quy ước rằng có một đường đi rút gọn vào C và ta cho tương ứng với nó ánh xạ đồng nhất $1_C$.

Trong (2), chẳng hạn có ba đường đi bắt đầu từ B và kết thúc tại D$'$; các ánh xạ tương ứng là $d\circ g\circ f$, $g'\circ c\circ f$ và $g'\circ f'\circ b$. Một biểu đồ được gọi là *giao hoán* nếu, với mọi cặp đường đi của biểu đồ có cùng gốc và cùng đầu mút, hai ánh xạ tương ứng là bằng nhau; đặc biệt nếu một đường đi có đầu mút trùng với gốc của nó, thì ánh xạ tương ứng phải là đồng nhất.

Để biểu đồ (2) là giao hoán, điều kiện cần và đủ là các hệ thức sau đúng:

$$
\tag{3}
f'\circ b=c\circ f,\qquad
g'\circ c=d\circ g,\qquad
h'\circ d=e\circ h ;
$$

nói cách khác, điều kiện cần và đủ là ba biểu đồ hình vuông trích ra từ (2) đều giao hoán. Thật vậy, các hệ thức (3) kéo theo $d\circ g\circ f=g'\circ c\circ f$ vì $d\circ g=g'\circ c$, và $g'\circ c\circ f=g'\circ f'\circ b$ vì $c\circ f=f'\circ b$; do đó ba đường đi bắt đầu từ B và kết thúc tại D$'$ cho cùng một ánh xạ. Người ta kiểm tra tương tự rằng bốn đường đi bắt đầu từ B và kết thúc tại E$'$ (tương ứng, ba đường đi bắt đầu từ C và kết thúc tại E$'$) cho cùng một ánh xạ. Các hệ thức (3) có nghĩa là hai đường đi bắt đầu từ B (tương ứng, C, D) và kết thúc tại C$'$ (tương ứng, D$'$, E$'$) cho cùng một ánh xạ. Mọi cặp đỉnh khác của (2) đều có thể được nối với nhau bởi nhiều nhất một đường đi, và do đó biểu đồ (2) quả thật là giao hoán.

Trong phần sau, chúng tôi để cho người đọc phát biểu và kiểm tra các kết quả tương tự đối với những kiểu biểu đồ khác.

### 2. Biểu đồ con rắn

#### Mệnh đề 1 {#alg-x-s1-prop-1 .statement}

Xét một biểu đồ giao hoán các A-môđun

$$
\tag{4}
\begin{array}{ccccc}
M & \xrightarrow{u} & N & \xrightarrow{v} & P\\
\downarrow f & & \downarrow g & & \downarrow h\\
M' & \xrightarrow{u'} & N' & \xrightarrow{v'} & P'
\end{array}
$$

Giả sử rằng hai hàng của (4) là khớp. Khi đó:

(i) Nếu $h$ là đơn ánh, ta có

$$
\tag{5}
\operatorname{Im}(g)\cap\operatorname{Im}(u')=\operatorname{Im}(u'\circ f)=\operatorname{Im}(g\circ u).
$$

(ii) Nếu $f$ là toàn ánh, ta có

$$
\tag{6}
\operatorname{Ker}(g)+\operatorname{Im}(u)=\operatorname{Ker}(v'\circ g)=\operatorname{Ker}(h\circ v).
$$

Hãy chứng minh (i). Hiển nhiên là ta có

$$
\operatorname{Im}(u'\circ f)=\operatorname{Im}(g\circ u)\subset\operatorname{Im}(g)\cap\operatorname{Im}(u').
$$

Chiều ngược lại, lấy $y'\in\operatorname{Im}(g)\cap\operatorname{Im}(u')$. Tồn tại $y\in N$ sao cho $y'=g(y)$. Vì $v'\circ u'=0$, ta có $0=v'(y')=v'(g(y))=h(v(y))$, do đó $v(y)=0$ vì $h$ là đơn ánh. Vì $(u,v)$ là một dãy khớp, tồn tại $x\in M$ sao cho $y=u(x)$, do đó $y'=g(u(x))$.

Hãy chứng minh (ii). Vì $v\circ u=0$ và $v'\circ u'=0$, hiển nhiên là

$$
\operatorname{Ker}(g)+\operatorname{Im}(u)\subset\operatorname{Ker}(v'\circ g)=\operatorname{Ker}(h\circ v).
$$

Ngược lại, lấy $y\in\operatorname{Ker}(v'\circ g)$. Khi đó $g(y)\in\operatorname{Ker}(v')$, và tồn tại $x'\in M'$ sao cho $u'(x')=g(y)$ vì dãy $(u',v')$ là khớp. Vì $f$ là toàn ánh, tồn tại $x\in M$ sao cho $f(x)=x'$, do đó $g(y)=u'(f(x))=g(u(x))$; ta kết luận rằng $y-u(x)\in\operatorname{Ker}(g)$, điều này hoàn tất chứng minh.

#### Bổ đề 1 {#alg-x-s1-lem-1 .statement}

Xét một biểu đồ giao hoán các A-môđun

$$
\tag{7}
\begin{array}{ccc}
M & \xrightarrow{u} & N\\
\downarrow f & & \downarrow g\\
M' & \xrightarrow{u'} & N'
\end{array}
$$

Khi đó tồn tại một và chỉ một đồng cấu $u_1:\operatorname{Ker}(f)\to\operatorname{Ker}(g)$, và một và chỉ một đồng cấu $u_2:\operatorname{Coker}(f)\to\operatorname{Coker}(g)$, sao cho các biểu đồ

$$
\tag{8}
\begin{array}{ccc}
\operatorname{Ker}(f) & \xrightarrow{u_1} & \operatorname{Ker}(g)\\
\downarrow i & & \downarrow j\\
M & \xrightarrow{u} & N
\end{array}
$$

và

$$
\begin{array}{ccc}
M' & \xrightarrow{u'} & N' \\
p \downarrow & & q \downarrow \\
\text{Coker } (f) & \xrightarrow{u_2} & \text{Coker } (g)
\end{array}
$$

là giao hoán, trong đó $i$ và $j$ ký hiệu các đơn ánh chính tắc, $p$ và $q$ các toàn ánh chính tắc.

Thật vậy, nếu $x \in \text{Ker } (f)$, ta có $f(\bar{x}) = 0$ và $g(u(x)) = u'(f(x)) = 0$, nên $u(x) \in \text{Ker } (g)$, và do đó sự tồn tại và tính duy nhất của $u_1$ là ngay lập tức. Tương tự, ta có
$$
u'(f(M)) = g(u(M)) \subset g(N),
$$
nên $u'$ cho, bằng cách chuyển qua các thương, một đồng cấu
$$
u_2 : \text{Coker } (f) \to \text{Coker } (g),
$$
là đồng cấu duy nhất mà đối với nó (9) là giao hoán.

Bây giờ ta xuất phát từ một biểu đồ giao hoán (4) của các A-môđun; nhờ Bổ đề 1, với nó tương ứng một biểu đồ giao hoán

$$
\begin{array}{ccccccccc}
\text{Ker } (f) & \xrightarrow{u_1} & \text{Ker } (g) & \xrightarrow{v_1} & \text{Ker } (h) \\
i \downarrow & & j \downarrow & & k \downarrow \\
M & \xrightarrow{u} & N & \xrightarrow{v} & P \\
f \downarrow & & g \downarrow & & h \downarrow \\
M' & \xrightarrow{u'} & N' & \xrightarrow{v'} & P' \\
p \downarrow & & q \downarrow & & r \downarrow \\
\text{Coker } (f) & \xrightarrow{u_2} & \text{Coker } (g) & \xrightarrow{v_2} & \text{Coker } (h)
\end{array}
$$

trong đó $i, j, k$ là các đơn ánh chính tắc, $p, q, r$ là các toàn ánh chính tắc, $u_1, u_2$ (tương ứng $v_1, v_2$) là các đồng cấu suy ra từ $u, u'$ (tương ứng từ $v, v'$) theo Bổ đề 1.

#### Mệnh đề 2 {#alg-x-s1-prop-2 .statement}

Giả sử rằng trong biểu đồ giao hoán (4), các dãy $(u, v)$ và $(u', v')$ là khớp. Khi đó:
(i) Ta có $v_1 \circ u_1 = 0$; nếu $u'$ là đơn ánh, dãy $(u_1, v_1)$ là khớp.
(ii) Ta có $v_2 \circ u_2 = 0$; nếu $v$ là toàn ánh, dãy $(u_2, v_2)$ là khớp.
(iii) Giả sử rằng $u'$ là đơn ánh và $v$ là toàn ánh. Khi đó tồn tại một và chỉ một đồng cấu $d : \text{Ker } (h) \to \text{Coker } (f)$ có tính chất sau: nếu $z \in \text{Ker } (h), y \in N$ và $x' \in M'$ thỏa mãn các hệ thức $v(y) = k(z)$ và $u'(x') = g(y)$, thì ta có $d(z) = p(x')$. Hơn nữa dãy
(*) $\text{Ker } (f) \xrightarrow{u_1} \text{Ker } (g) \xrightarrow{v_1} \text{Ker } (h) \xrightarrow{d} \text{Coker } (f) \xrightarrow{u_2} \text{Coker } (g) \xrightarrow{v_2} \text{Coker } (h)$
là khớp.

$$
\begin{array}{ccccc}
\operatorname{Ker}(f)&\xrightarrow{u_1}&\operatorname{Ker}(g)&\xrightarrow{v_1}&\operatorname{Ker}(h)\\
\downarrow\scriptstyle i&&\downarrow\scriptstyle j&&\downarrow\scriptstyle k\\
M&\xrightarrow{u}&N&\xrightarrow{v}&P\\
\downarrow\scriptstyle f&&\downarrow\scriptstyle g&&\downarrow\scriptstyle h\\
M'&\xrightarrow{u'}&N'&\xrightarrow{v'}&P'\\
\downarrow\scriptstyle p&&\downarrow\scriptstyle q&&\downarrow\scriptstyle r\\
\operatorname{Coker}(f)&\xrightarrow{u_2}&\operatorname{Coker}(g)&\xrightarrow{v_2}&\operatorname{Coker}(h)
\end{array}
$$

Ta hãy chứng minh (i). Vì $u_1$ và $v_1$ có cùng đồ thị như các hạn chế của $u$ và $v$ trên $\operatorname{Ker}(f)$ và $\operatorname{Ker}(g)$ tương ứng, nên ta có $v_1\circ u_1=0$. Ta có

$$
\operatorname{Ker}(v_1)=\operatorname{Ker}(g)\cap\operatorname{Ker}(v)=\operatorname{Ker}(g)\cap\operatorname{Im}(u)=\operatorname{Im}(j)\cap\operatorname{Im}(u).
$$

Nhưng theo mệnh đề 1 (i), ta có $\operatorname{Ker}(v_1)=\operatorname{Im}(j\circ u_1)=\operatorname{Im}(u_1)$ nếu $u'$ là đơn ánh.

Ta hãy chứng minh (ii). Vì $u_2$ và $v_2$ thu được từ $u$ và $v$ bằng cách chuyển qua các thương, nên hiển nhiên là $v_2\circ u_2=0$. Giả sử rằng $v$ là toàn ánh; vì $q$ và $p$ là toàn ánh, theo các giả thiết và mệnh đề 1 (ii) ta có

$$
\begin{aligned}
\operatorname{Ker}(v_2)&=q(\operatorname{Ker}(v_2\circ q))=q(\operatorname{Ker}(v')+\operatorname{Im}(g))=q(\operatorname{Ker}(v'))\\
&=q(\operatorname{Im}(u'))=\operatorname{Im}(q\circ u')=\operatorname{Im}(u_2\circ p)=\operatorname{Im}(u_2).
\end{aligned}
$$

Sau cùng ta hãy chứng minh (iii). Với $z\in\operatorname{Ker}(h)$, tồn tại $y\in N$ sao cho $v(y)=k(z)$ vì $v$ là toàn ánh; hơn nữa, ta có $v'(g(y))=h(k(z))=0$, và do đó tồn tại duy nhất $x'\in M'$ sao cho $u'(x')=g(y)$ vì $u'$ là đơn ánh. Ta hãy chỉ ra rằng phần tử $p(x')\in\operatorname{Coker}(f)$ là độc lập với phần tử $y\in N$ sao cho $v(y)=k(z)$. Thật vậy, nếu $y_1\in N$ là một phần tử thứ hai sao cho $v(y_1)=k(z)$, thì ta có $y_1=y+u(x)$ với $x\in M$; ta hãy chỉ ra rằng nếu $x'_1\in M'$ sao cho $u'(x'_1)=g(y_1)$, thì ta có $x'_1=x'+f(x)$; thật vậy, ta có $u'(x'+f(x))=u'(x')+u'(f(x))=g(y)+g(u(x))=g(y+u(x))=g(y_1)$. Sau cùng, ta kết luận rằng $p(x'_1)=p(x')+p(f(x))=p(x')$. Do đó ta có thể đặt $d(z)=p(x')$ và như vậy đã xác định được một ánh xạ $d:\operatorname{Ker}(h)\to\operatorname{Coker}(f)$.

Nếu bây giờ $z_1,z_2$ là các phần tử của $\operatorname{Ker}(h)$, nếu $\lambda_1,\lambda_2\in A$ và $z=\lambda_1z_1+\lambda_2z_2$, ta lấy các phần tử $y_1$ và $y_2$ của $N$ sao cho $v(y_1)=k(z_1)$ và $v(y_2)=k(z_2)$ và ta chọn cho $y\in N$ phần tử $\lambda_1y_1+\lambda_2y_2$; khi đó ngay lập tức có

$$
d(z)=\lambda_1d(z_1)+\lambda_2d(z_2),
$$

nên $d$ là một đồng cấu.

Giả sử rằng $z=v_1(t)$ với một $t\in\operatorname{Ker}(g)$ nào đó; khi đó ta lấy cho $y\in N$ phần tử $j(t)$. Vì $g(j(t))=0$, ta kết luận rằng $d(z)=0$, do đó $d\circ v_1=0$. Ngược lại, giả sử rằng $d(z)=0$. Với các ký hiệu trước đó, do đó ta có $x'=f(x)$, trong đó x ∈ M. Trong trường hợp này, ta có $g(y) = u'(f(x)) = g(u(x))$, hay tương đương $g(y - u(x)) = 0$. Do đó phần tử $y - u(x)$ có dạng $j(n)$ với $n \in \mathrm{Ker}\,(g)$, và ta có

$$
k(z) = v(y) = v(u(x) + j(n)) = v(j(n)) = k(v_1(n));
$$

vì $k$ là đơn ánh, $z = v_1(n)$, điều này chứng minh rằng dãy (*) là khớp tại $\mathrm{Ker}\,(h)$.

Cuối cùng, ta có (với cùng các ký hiệu)

$$
u_2(d(z)) = u_2(p(x')) = q(u'(x')) = q(g(y)) = 0 \quad \text{do đó} \quad u_2 \circ d = 0 .
$$

Ngược lại, giả sử rằng một phần tử $w = p(x')$ của $\mathrm{Coker}\,(f)$ sao cho

$$
u_2(w) = u_2(p(x')) = 0 \quad (\text{với } x' \in \mathbf{M}') .
$$

Do đó ta có $q(u'(x')) = 0$, và hệ quả là $u'(x') = g(y)$ với một $y \in \mathbf{N}$; vì $v'(u'(x')) = 0$, ta có $v'(g(y)) = 0$, nên $h(v(y)) = 0$, nói cách khác $v(y) = k(z)$ với một $z \in \mathrm{Ker}\,(h)$, và theo định nghĩa $w = d(z)$, điều đó cho thấy rằng dãy (*) là khớp tại $\mathrm{Coker}\,(f)$. Ta đã thấy trong (i) rằng nó khớp tại $\mathrm{Ker}\,(g)$ và trong (ii) rằng nó khớp tại $\mathrm{Coker}\,(g)$, điều đó hoàn tất việc chứng minh (iii).

#### Hệ quả 1 {#alg-x-s1-prop-2-cor-1 .statement}

Giả sử rằng biểu đồ (4) là giao hoán và có các hàng khớp. Khi đó:

(i) Nếu $u', f$ và $h$ là đơn ánh, thì $g$ là đơn ánh.
(ii) Nếu $v, f$ và $h$ là toàn ánh, thì $g$ là toàn ánh.

Mệnh đề (i) là một hệ quả của mệnh đề (i) của mệnh đề 2: thật vậy ta có $\mathrm{Ker}\,(f) = 0$ và $\mathrm{Ker}\,(h) = 0$, do đó $\mathrm{Ker}\,(g) = 0$.

Mệnh đề (ii) là một hệ quả của mệnh đề (ii) của mệnh đề 2: thật vậy, ta có $\mathrm{Coker}\,(f) = 0$ và $\mathrm{Coker}\,(h) = 0$, do đó $\mathrm{Coker}\,(g) = 0$.

#### Hệ quả 2 {#alg-x-s1-prop-2-cor-2 .statement}

Giả sử rằng biểu đồ (4) là giao hoán và có các hàng khớp. Trong các điều kiện đó:

(i) Nếu $g$ đơn ánh và nếu $f$ và $v$ toàn ánh, thì $h$ đơn ánh.
(ii) Nếu $g$ toàn ánh và nếu $h$ và $u'$ đơn ánh, thì $f$ toàn ánh.

Để chứng minh (i), xét biểu đồ

$$
\begin{array}{ccccc}
u(\mathbf{M}) & \xrightarrow{w} & \mathbf{N} & \xrightarrow{v} & \mathbf{P} \\
f' \downarrow & & g \downarrow & & h \downarrow \\
u'(\mathbf{M}') & \xrightarrow{w'} & \mathbf{N}' & \xrightarrow{v'} & \mathbf{P}'
\end{array}
$$

trong đó $f'$ là ánh xạ có cùng đồ thị với hạn chế của $g$ trên $u(\mathbf{M})$, còn $w$ và $w'$ là các đơn ánh chính tắc; hiển nhiên biểu đồ này giao hoán và có các hàng khớp. Hơn nữa $w'$ đơn ánh, và theo giả thiết $v$ toàn ánh; do đó, theo mệnh đề 2 (iii), ta có một dãy khớp

$$
\mathrm{Ker}\,(g) \longrightarrow \mathrm{Ker}\,(h) \xrightarrow{d} \mathrm{Coker}\,(f');
$$

vì $g$ đơn ánh và $f'$ toàn ánh, nên suy ra $\mathrm{Ker}\,(h) = 0$.

Để chứng minh (ii), xét biểu đồ

$$
\begin{array}{ccccc}
M&\xrightarrow{u}&N&\xrightarrow{w}&\nu(N)\\
{\scriptstyle f}\downarrow&&{\scriptstyle g}\downarrow&&{\scriptstyle h'}\downarrow\\
M'&\xrightarrow{u'}&N'&\xrightarrow{w'}&\nu'(N')
\end{array}
$$

trong đó lần này $h'$ là ánh xạ có cùng đồ thị với hạn chế của $h$ trên $\nu(N)$, và $w$ và $w'$ lần lượt có cùng đồ thị với $\nu$ và $\nu'$; biểu đồ này giao hoán và các hàng của nó là khớp. Hơn nữa $w$ toàn ánh và theo giả thiết $u'$ đơn ánh; do đó, theo mệnh đề 2 (iii), ta có một dãy khớp

$$
\operatorname{Ker}(h')\xrightarrow{d}\operatorname{Coker}(f)\longrightarrow\operatorname{Coker}(g);
$$

vì $g$ toàn ánh và $h'$ đơn ánh, nên suy ra $\operatorname{Coker}(f)=0$.

**Hệ quả 3 (Bổ đề năm).** — Xét một biểu đồ giao hoán các $A$-môđun

$$
\begin{array}{ccccccccc}
M_1&\xrightarrow{u_1}&M_2&\xrightarrow{u_2}&M_3&\xrightarrow{u_3}&M_4&\xrightarrow{u_4}&M_5\\
{\scriptstyle f_1}\downarrow&&{\scriptstyle f_2}\downarrow&&{\scriptstyle f_3}\downarrow&&{\scriptstyle f_4}\downarrow&&{\scriptstyle f_5}\downarrow\\
M'_1&\xrightarrow{u'_1}&M'_2&\xrightarrow{u'_2}&M'_3&\xrightarrow{u'_3}&M'_4&\xrightarrow{u'_4}&M'_5
\end{array}
$$

trong đó các hàng là khớp.

(i) Nếu $f_2$ và $f_4$ đơn ánh và $f_1$ toàn ánh, thì $f_3$ đơn ánh.

(ii) Nếu $f_2$ và $f_4$ toàn ánh và $f_5$ đơn ánh, thì $f_3$ toàn ánh.

Đặc biệt, nếu $f_1$, $f_2$, $f_4$ và $f_5$ là các đẳng cấu, thì $f_3$ cũng vậy.

Để chứng minh (i), đặt $\widetilde M_2=\operatorname{Coker}(u_1)$, $\widetilde M'_2=\operatorname{Coker}(u'_1)$ và ký hiệu bởi $\widetilde f_2:\widetilde M_2\to\widetilde M'_2$ ánh xạ suy ra từ $f_2$. Từ hệ quả 2 (i) suy ra rằng $\widetilde f_2$ đơn ánh. Áp dụng hệ quả 1 (i) cho biểu đồ

$$
\begin{array}{ccccc}
\widetilde M_2&\xrightarrow{\widetilde u_2}&M_3&\xrightarrow{u_3}&M_4\\
{\scriptstyle \widetilde f_2}\downarrow&&{\scriptstyle f_3}\downarrow&&{\scriptstyle f_4}\downarrow\\
\widetilde M'_2&\xrightarrow{\widetilde u'_2}&M'_3&\xrightarrow{u'_3}&M'_4
\end{array}
$$

trong đó $\widetilde u_2$ và $\widetilde u'_2$ được suy ra từ $u_2$ và $u'_2$, ta thấy rằng $f_3$ đơn ánh.

Để chứng minh (ii), đặt $\widetilde M_4=\operatorname{Ker}(u_4)$, $\widetilde M'_4=\operatorname{Ker}(u'_4)$ và ký hiệu bởi $\widetilde f_4:\widetilde M_4\to\widetilde M'_4$ ánh xạ cảm sinh bởi $f_4$. Từ hệ quả 2 (ii) suy ra rằng $\widetilde f_4$ là toàn ánh. Áp dụng hệ quả 1 (ii) cho biểu đồ

$$
\begin{array}{ccccc}
M_2&\xrightarrow{u_2}&M_3&\xrightarrow{\widetilde u_3}&\widetilde M_4\\
{\scriptstyle f_2}\downarrow&&{\scriptstyle f_3}\downarrow&&{\scriptstyle \widetilde f_4}\downarrow\\
M'_2&\xrightarrow{u'_2}&M'_3&\xrightarrow{\widetilde u'_3}&\widetilde M'_4
\end{array}
$$

trong đó $\widetilde u_3$ và $\widetilde u'_3$ có cùng đồ thị như $u_3$ và $u'_3$, ta thấy rằng $f_3$ là toàn ánh.

### 3. Môđun phẳng

#### Định nghĩa 1 {#alg-x-s1-def-1 .statement}

Người ta nói rằng a-môđun E là phẳng nếu, với mọi dãy khớp các a-môđun phải và các đồng cấu

(11) $M' \xrightarrow{u} M \xrightarrow{v} M''$,

dãy các ánh xạ $\mathbf{Z}$-tuyến tính

(12) $M' \otimes_A E \xrightarrow{u \otimes 1} M \otimes_A E \xrightarrow{v \otimes 1} M'' \otimes_A E$

là khớp.

#### Mệnh đề 3 {#alg-x-s1-prop-3 .statement}

Để a-môđun E là phẳng, điều kiện cần và đủ là với mọi A-đồng cấu đơn ánh $u : M' \to M$ của các A-môđun phải, ánh xạ $u \otimes 1 : M' \otimes_A E \to M \otimes_A E$ là đơn ánh.

Nếu E là phẳng và $u : M' \to M$ là đơn ánh, thì dãy $0 \to M' \xrightarrow{u} M$ là khớp, do đó dãy $0 \longrightarrow M' \otimes_A E \xrightarrow{u \otimes 1} M \otimes_A E$ cũng khớp, và $u \otimes 1$ là đơn ánh. Đảo lại, xét dãy khớp (11); đặt $M''_1 = v(M)$, và gọi $i : M''_1 \to M''$ là đơn ánh chính tắc và $p : M \to M''_1$ là ánh xạ $m \mapsto v(m)$. Dãy $M' \xrightarrow{u} M \xrightarrow{p} M''_1 \longrightarrow 0$ là khớp; theo II, p. 58, mệnh đề 5, do đó dãy $M' \otimes_A E \xrightarrow{u \otimes 1} M \otimes_A E \xrightarrow{p \otimes 1} M''_1 \otimes_A E$ là khớp. Hơn nữa, ta có $v = i \circ p$, nên $(v \otimes 1) = (i \otimes 1) \circ (p \otimes 1)$; nếu E thỏa mãn điều kiện của mệnh đề, thì $i \otimes 1$ là đơn ánh, nên

$$
\operatorname{Ker}(v \otimes 1) = \operatorname{Ker}(p \otimes 1) = \operatorname{Im}(u \otimes 1)
$$

và dãy (12) là khớp.

#### Mệnh đề 4 {#alg-x-s1-prop-4 .statement}

(i) Cho $(E_i)_{i \in I}$ là một họ các a-môđun, $E = \bigoplus_{i \in I} E_i$ là tổng trực tiếp của chúng. Để a-môđun E là phẳng, điều kiện cần và đủ là mỗi $E_i$ đều như vậy.

(ii) Cho I là một tập hợp tiền thứ tự lọc phải, $(E_\alpha, f_{\beta \alpha})$ là một hệ quy nạp các a-môđun đối với I, $E = \varinjlim E_\alpha$ là giới hạn quy nạp của nó. Nếu mỗi a-môđun $E_\alpha$ đều phẳng, thì E là phẳng.

Cho $M' \to M \to M''$ là một dãy khớp các a-môđun phải.

(i) Để dãy $\bigoplus_{i \in I} (M' \otimes_A E_i) \to \bigoplus_{i \in I} (M \otimes_A E_i) \to \bigoplus_{i \in I} (M'' \otimes_A E_i)$ là khớp, điều kiện cần và đủ là mỗi dãy $M' \otimes_A E_i \to M \otimes_A E_i \to M'' \otimes_A E_i$ đều như vậy (II, p. 13, mệnh đề 7), điều này chứng minh (i) vì $\bigoplus (M \otimes_A E_i)$ đồng nhất một cách chính tắc với $M \otimes_A E$ (II, p. 61, mệnh đề 7).

(ii) Theo giả thiết, mỗi dãy $M' \otimes_A E_i \to M \otimes_A E_i \to M'' \otimes_A E_i$ đều khớp, và do đó dãy $M' \otimes_A E \to M \otimes_A E \to M'' \otimes_A E$ cũng khớp, vì phép chuyển sang giới hạn quy nạp giao hoán với tích tenxơ (II, p. 93, mệnh đề 7) và bảo toàn tính khớp (II, p. 91, mệnh đề 3).

#### Ví dụ 1 {#alg-x-s1-n3-exa-1 .statement}

Hiển nhiên $A_s$ là một $A$-môđun phẳng; do đó từ mệnh đề 4 (i) suy ra rằng mọi $A$-môđun tự do, và nói chung hơn mọi $A$-môđun xạ ảnh, đều phẳng (xem thêm II, p. 63, hệ quả 6).

\* Đảo lại, mọi $A$-môđun phẳng hữu hạn trình bày đều xạ ảnh (No. 5). \*

#### Ví dụ 2 {#alg-x-s1-n3-exa-2 .statement}

Theo mệnh đề 4 (ii), mọi $A$-môđun là giới hạn quy nạp của một hệ quy nạp lọc gồm các $A$-môđun tự do đều phẳng. Ta sẽ chứng minh mệnh đề đảo lại ở No. 6.

#### Ví dụ 3 {#alg-x-s1-n3-exa-3 .statement}

Nếu $A$ là nửa đơn, mọi $A$-môđun đều xạ ảnh (VIII, § 5, No. 1, mệnh đề 1), do đó phẳng.

#### Ví dụ 4 {#alg-x-s1-n3-exa-4 .statement}

\* Nếu $A$ là một vành địa phương Artin (không nhất thiết giao hoán), một $A$-môđun là phẳng khi và chỉ khi nó là tự do (AC II, § 3, No. 2, hệ quả 2 của mệnh đề 5). \*

#### Ví dụ 5 {#alg-x-s1-n3-exa-5 .statement}

Nếu $A$ là nguyên, trường phân thức $K$ của $A$ là một $A$-môđun phẳng (II, p. 118, mệnh đề 27).

#### Ví dụ 6 {#alg-x-s1-n3-exa-6 .statement}

*Trong AC II và III, chúng tôi sẽ nghiên cứu hai ví dụ quan trọng về $A$-môđun phẳng khi $A$ giao hoán: các vành phân thức $S^{-1} A$, và, khi $A$ là Noether, các hoàn thành tách biệt của $A$ đối với các tôpô J-adic.*

#### Ví dụ 7 {#alg-x-s1-n3-exa-7 .statement}

Cho $a \in A$ sao cho ánh xạ $a_A : x \mapsto ax$ từ $A$ vào $A$ là đơn ánh (“$a$ không là ước trái của 0”). Nếu $E$ là một $A$-môđun phẳng, thì phép vị tự $a_E$ là đơn ánh, vì nó được đồng nhất với $a_A \otimes 1 : A_d \otimes_A E \to A_d \otimes_A E$. Đặc biệt, nếu $A$ là nguyên, mọi $A$-môđun phẳng đều không xoắn. Ngược lại, nếu $A$ là chính, mọi $A$-môđun không xoắn đều phẳng: thật vậy, nếu $A$-môđun $E$ không xoắn, mọi môđun con sinh hữu hạn của $E$ đều tự do (VII, § 4, No. 4, Cor. 2 to Theorem 4), và $E$ là một hợp tăng lọc của các môđun con phẳng, do đó là phẳng (Prop. 4 (ii)).

#### Ví dụ 8 {#alg-x-s1-n3-exa-8 .statement}

Cho $B$ là một vành và $\rho : A \to B$ một đồng cấu. Nếu $E$ là một $A$-môđun phẳng, thì $B$-môđun $E_{(B)} = B \otimes_A E$ là phẳng. Thật vậy, cho $u : N' \to N$ là một đơn cấu của các $B$-môđun phải; khi đó $u \otimes_B 1_{E_{(B)}}$ được đồng nhất một cách chính tắc với đồng cấu $u \otimes_A 1_E : N' \otimes_A E \to N \otimes_A E$, và đồng cấu này là đơn ánh nếu $E$ là phẳng.

#### Ví dụ 9 {#alg-x-s1-n3-exa-9 .statement}

Giả sử rằng $A = K[X, Y]$, trong đó $K$ là một trường. Khi đó iđêan cực đại $m$ sinh bởi $X$ và $Y$ là một $A$-môđun không xoắn, nhưng không phẳng. Thật vậy, xét vành $B = A/(Y)$, vành này đẳng cấu với $K[X]$, do đó nguyên. $B$-môđun $m_{(B)}$ đẳng cấu với $m/Ym = (X, Y)/(XY, Y^2)$, trong đó lớp của $Y$ là xoắn. Do đó, $m_{(B)}$ không là một $B$-môđun phẳng, vì thế $m$ không phẳng.

#### Ví dụ 10 {#alg-x-s1-n3-exa-10 .statement}

Giả sử $A$ giao hoán. Cho $B$ là đại số $A[X_1, ..., X_n]/(P)$, trong đó $P$ là một đa thức khác không. Với mọi iđêan nguyên tố $p$ của $A$, ký hiệu $\kappa(p)$ là trường phân thức của vành nguyên $A/p$, $E(p)$ là đại số $\kappa(p)[X_1, ..., X_n]$ và $P(p)$ là ảnh của $P$ trong $E(p)$ bởi ánh xạ chính tắc.

Ta có thể chứng minh rằng, để $B$ phẳng như một $A$-môđun, chỉ cần $P(p) \neq 0$ với mọi iđêan nguyên tố $p$ của $A$. Nếu $A$ là nguyên, điều kiện này là cần thiết.

\* Theo ngôn ngữ hình học, xét phép chiếu $\pi : \mathrm{Spec}(B) \to \mathrm{Spec}(A)$. Với mọi $p \in \mathrm{Spec}(A)$, thớ $\pi^{-1}(p)$ được đồng nhất với dưới đa tạp $V_p$ của không gian afin $\mathbf{A}_{\kappa(p)}^n = \mathrm{Spec}(E(p))$ được xác định bởi $P(p)$, và tập hợp $F$ của các $p$ mà đối với chúng dưới đa tạp này là toàn bộ không gian (*i.e.* mà đối với chúng $P(p) = 0$) là một tập đóng của

Spec (A). Điều kiện trên có nghĩa là tập đóng này là rỗng, nói cách khác, với mọi $p$ dưới đa tạp $V_p$ là một siêu mặt trong $\mathbf{A}_{k(p)}^n$.

#### Ví dụ 11 {#alg-x-s1-n3-exa-11 .statement}

\* Cho S và X là hai không gian giải tích phức và cho $f : X \to S$ là một cấu xạ. Ta nói rằng $f$ là phẳng tại một điểm $x$ của X nếu $\mathcal{O}_{X,x}$, được xét như $\mathcal{O}_{S,f(x)}$-môđun nhờ đồng cấu $f^* : \mathcal{O}_{S,f(x)} \to \mathcal{O}_{X,x}$, là phẳng. Tập các điểm của X mà tại đó $f$ phẳng là một tập mở của X, và hạn chế của $f$ lên tập mở này là một ánh xạ mở. Nếu X và S là các đa tạp giải tích liên thông có số chiều hữu hạn, thì $f$ là phẳng (tại mọi điểm của X) khi và chỉ khi $f(X)$ mở trong S và các thớ $f^{-1}(s)$, với $s \in f(X)$, đều có cùng chiều. \*

### 4. Môđun có trình bày hữu hạn

Một trình bày (hay trình bày có độ dài 1) của một $A$-môđun E được gọi là một dãy khớp

$$
L_1 \to L_0 \to E \to 0
$$

gồm các A-môđun trong đó $L_0$ và $L_1$ là tự do.

Mọi A-môđun E đều có một trình bày. Thật vậy, ta biết (II, p. 27, mệnh đề 20) rằng tồn tại một đồng cấu toàn ánh $u : L_0 \to E$, trong đó $L_0$ là tự do; nếu R là hạt nhân của $u$, thì tương tự tồn tại một đồng cấu toàn ánh $v : L_1 \to R$ trong đó $L_1$ là tự do. Nếu xét $v$ như một đồng cấu từ $L_1$ vào $L_0$, thì dãy $L_1 \xrightarrow{v} L_0 \xrightarrow{u} E \to 0$ là khớp theo định nghĩa, do đó có mệnh đề của chúng ta.

Nếu $\rho : A \to B$ là một đồng cấu các vành, mọi trình bày (13) của E cho một trình bày của $E_{(B)} = B \otimes_A E$:

$$
B \otimes_A L_1 \to B \otimes_A L_0 \to B \otimes_A E \to 0
$$

theo II, p. 58, mệnh đề 5 và sự kiện rằng $B \otimes_A L$ là một B-môđun tự do khi L là tự do.

Người ta nói rằng một trình bày (13) của một môđun E là hữu hạn nếu các môđun tự do $L_0$ và $L_1$ có các cơ sở hữu hạn. Rõ ràng là nếu trình bày (13) là hữu hạn thì trình bày (14) cũng vậy. Ta nói rằng E là một A-môđun hữu hạn trình bày nếu nó thừa nhận một trình bày hữu hạn.

#### Mệnh đề 5 {#alg-x-s1-prop-5 .statement}

(i) Mọi môđun thừa nhận một trình bày hữu hạn đều sinh hữu hạn.
(ii) Nếu A là một vành Noether trái thì mọi A-môđun hữu hạn sinh đều thừa nhận một trình bày hữu hạn.
(iii) Mọi môđun xạ ảnh hữu hạn sinh đều thừa nhận một trình bày hữu hạn.

Mệnh đề (i) suy ra một cách hiển nhiên từ các định nghĩa. Giả sử A là Noether trái và E là sinh hữu hạn. Khi đó tồn tại một đồng cấu toàn ánh $u : L_0 \to E$, trong đó $L_0$ là một A-môđun tự do có một cơ sở hữu hạn; hạt nhân R của $u$ là sinh hữu hạn, do đó tồn tại một đồng cấu toàn ánh $v : L_1 \to R$ trong đó $L_1$ là tự do với cơ sở hữu hạn, và dãy khớp $L_1 \xrightarrow{v} L_0 \xrightarrow{u} E \to 0$ là một trình bày hữu hạn của E; do đó có (ii).

Sau hết, giả sử E là một môđun xạ ảnh hữu hạn sinh; khi đó nó là một nhân tử trực tiếp của một môđun tự do hữu hạn sinh $L_0$ (II, p. 40, hệ quả 1); hạt nhân R của đồng cấu toàn ánh L_0 → E khi đó đẳng cấu với một thương của $L_0$, nên là sinh hữu hạn, và ta kết luận như trên.

#### Mệnh đề 6 {#alg-x-s1-prop-6 .statement}

Cho A là một vành, E là một A-môđun hữu hạn trình bày. Với mọi dãy khớp

$$
0 \to F \xrightarrow{j} G \xrightarrow{p} E \to 0
$$

trong đó G là sinh hữu hạn, môđun F là sinh hữu hạn.

Cho $L_1 \xrightarrow{r} L_0 \xrightarrow{s} E \to 0$ là một trình bày hữu hạn; nếu (e_i) là một cơ sở của L_0, thì với mỗi i tồn tại một phần tử g_i \in G sao cho p(g_i) = s(e_i) ; do đó đồng cấu u : L_0 \to G sao cho u(e_i) = g_i với mọi i thỏa mãn s = p \circ u. Vì s \circ r = 0, ta có u(r(L_1)) \subset \mathrm{Ker}\ p, và vì Ker p đẳng cấu với F, ta thấy tồn tại một đồng cấu v : L_1 \to F sao cho biểu đồ

$$
\begin{array}{ccccccc}
L_1 & \xrightarrow{r} & L_0 & \xrightarrow{s} & E & \to & 0 \\
v \downarrow & & u \downarrow & & 1_E \downarrow & & \\
F & \xrightarrow{j} & G & \xrightarrow{p} & E & \to & 0
\end{array}
$$

là giao hoán. Vì j là đơn ánh và s là toàn ánh, ta có thể áp dụng Mệnh đề 2 của X, p. 4, nói cách khác có một dãy khớp

$$
\mathrm{Ker}\ 1_E \xrightarrow{d} \mathrm{Coker}\ v \to \mathrm{Coker}\ u \to \mathrm{Coker}\ 1_E.
$$

Điều này cho thấy Coker v đẳng cấu với G/u(L_0), theo giả thiết là sinh hữu hạn. Ngoài ra ta có dãy khớp

$$
0 \to v(L_1) \to F \to \mathrm{Coker}\ v \to 0
$$

và vì v(L_1) và Coker v là sinh hữu hạn, F cũng vậy (II, p. 17, hệ quả 5).

#### Mệnh đề 7 {#alg-x-s1-prop-7 .statement}

Cho M là một A-môđun. Tồn tại một tập hợp có thứ tự I quy nạp sang phải và một hệ quy nạp các A-môđun hữu hạn trình bày $(M_\alpha, \varphi_{\beta\alpha})$ đối với I sao cho M đẳng cấu với $\lim_\alpha M_\alpha$. Nếu M có một hệ sinh gồm n phần tử, ta có thể giả sử rằng điều tương tự cũng đúng với các $M_\alpha$.

Xét một trình bày

$$
A_s^{(K)} \xrightarrow{u} A_s^{(L)} \xrightarrow{v} M \to 0 ;
$$

gọi I là tập hợp các cặp $\alpha = (K', L')$, trong đó K' (tương ứng L') là một tập con hữu hạn của K (tương ứng của L), sao cho u cảm sinh một ánh xạ u_\alpha từ môđun con $A_s^{K'}$ của $A_s^{(K)}$ vào môđun con $A_s^{L'}$ của $A_s^{(L)}$ ; với $\alpha \in I$, gọi $M_\alpha$ là đối hạt nhân của $u_\alpha$ và $v_\alpha : A_s^{L'} \to M_\alpha$ là ánh xạ chính tắc, để ta có một biểu đồ giao hoán với các hàng khớp:

$$
\begin{array}{ccccccc}
A_s^{(K)} & \xrightarrow{u} & A_s^{(L)} & \xrightarrow{l} & M & \to & 0 \\
i_\alpha \uparrow & & j_\alpha \uparrow & & f_\alpha \uparrow \\
A_s^{K'} & \xrightarrow{u_\alpha} & A_s^{L'} & \xrightarrow{v_\alpha} & M_\alpha & \to & 0 ,
\end{array}
$$

trong đó $i_\alpha$ và $j_\alpha$ là các đơn ánh chính tắc, và trong đó $f_\alpha$ được suy ra từ $j_\alpha$ bằng cách chuyển qua các thương. Ta sắp thứ tự tập hợp I bởi quan hệ

$$
\alpha = (K',L') \leq \beta = (K'',L'') \quad \text{khi}\quad K' \subset K'',\quad L' \subset L'' ;
$$

với $\alpha\leq\beta$, gọi $\varphi_{\beta\alpha}:M_\alpha\longrightarrow M_\beta$ là đồng cấu được suy ra bằng cách chuyển qua các thương từ bao hàm của $A_s^{L'}$ vào $A_s^{L''}$. Ta kiểm tra ngay lập tức rằng tập hợp có thứ tự I là quy nạp, rằng $(M_\alpha,\varphi_{\beta\alpha})$ là một hệ quy nạp các A-môđun và rằng $(\varphi_\alpha)$ là một hệ quy nạp các A-đồng cấu. Bằng cách chuyển sang giới hạn quy nạp, ta thu được một biểu đồ giao hoán

$$
\begin{array}{ccccc}
A_s^{(K)} & \xrightarrow{u} & A_s^{(L)} & \xrightarrow{v} & M \longrightarrow 0\\
\uparrow\scriptstyle i && \uparrow\scriptstyle j && \uparrow\scriptstyle\varphi\\
\underset{\longrightarrow}{\lim}\,A_s^{K'} & \longrightarrow & \underset{\longrightarrow}{\lim}\,A_s^{L'} & \longrightarrow & \underset{\longrightarrow}{\lim}\,M_\alpha \longrightarrow 0
\end{array}
\tag{15}
$$

các hàng của biểu đồ này là khớp (II, p. 91, mệnh đề 3); vì $i$ và $j$ là song ánh, $\varphi$ cũng vậy (X, p. 7, hệ quả 3), do đó có mệnh đề.

### 5. Đồng cấu của một A-môđun hữu hạn trình bày

Cho E là một A-môđun. Nếu I là một tập quy nạp tiền thứ tự và $(G_i,u_{ji})$ là một hệ quy nạp các A-môđun đối với I, thì các ánh xạ chính tắc $G_i\longrightarrow\underset{\longrightarrow}{\lim}\,G_i$ cảm sinh các đồng cấu $\operatorname{Hom}_A(E,G_i)\longrightarrow\operatorname{Hom}_A(E,\underset{\longrightarrow}{\lim}\,G_i)$, do đó một đồng cấu gọi là *chính tắc*

$$
\underset{\substack{\longrightarrow\\ i\in I}}{\lim}\operatorname{Hom}_A(E,G_i)
\longrightarrow
\operatorname{Hom}_A\left(E,\underset{\substack{\longrightarrow\\ i\in I}}{\lim}G_i\right).
\tag{16}
$$

Cho B là một vành khác, F một B-môđun, G một song môđun (A, B); một đồng cấu chính tắc đã được định nghĩa trong II, p. 75:

$$
\operatorname{Hom}_A(E,G)\otimes_B F
\longrightarrow
\operatorname{Hom}_A(E,G\otimes_B F).
\tag{17}
$$

#### Mệnh đề 8 {#alg-x-s1-prop-8 .statement}

a) *Nếu A-môđun E là kiểu hữu hạn (resp. có trình bày hữu hạn), thì đồng cấu chính tắc (16) là đơn ánh (resp. song ánh).*

*b) Giả sử rằng B-môđun F là phẳng; nếu A-môđun E là kiểu hữu hạn (resp. có trình bày hữu hạn), thì đồng cấu chính tắc (17) là đơn ánh (resp. song ánh).*

Chẳng hạn, ta hãy chứng minh b), chứng minh của a) là tương tự. Coi A, B, F, G là cố định, và, với mọi A-môđun phải E, đặt

$$
T(E)=\operatorname{Hom}_A(E,G)\otimes_B F,\qquad
T'(E)=\operatorname{Hom}_A(E,G\otimes_B F)
$$

và ký hiệu bởi $\nu_E$ đồng cấu (17); với mọi đồng cấu $v:E\to E'$ của các A-môđun phải, đặt $T(v)=\operatorname{Hom}(v,1_G)\otimes 1_F$ và $T'(v)=\operatorname{Hom}(v,1_G\otimes 1_F)$.

Cho $L_1 \xrightarrow{v} L_0 \xrightarrow{w} E \to 0$ là một trình bày của $E$; ta giả sử môđun tự do $L_0$ (resp. các môđun tự do $L_0$ và $L_1$) *kiểu hữu hạn*. Biểu đồ

$$
\begin{array}{ccccccc}
0 & \to & T(E) & \xrightarrow{T(w)} & T(L_0) & \xrightarrow{T(v)} & T(L_1) \\
& & v_E \downarrow & & v_{L_0} \downarrow & & v_{L_1} \downarrow \\
0 & \to & T'(E) & \xrightarrow{T'(w)} & T'(L_0) & \xrightarrow{T'(v)} & T'(L_1)
\end{array}
$$

là giao hoán, và hàng thứ hai của nó là khớp (II, p. 36, đl. 1); hơn nữa, dãy

$$
0 \to \mathrm{Hom}_A(E, G) \to \mathrm{Hom}_A(L_0, G) \to \mathrm{Hom}_A(L_1, G)
$$

là khớp (*loc. cit.*), và vì $F$ là *phẳng*, nên hàng thứ nhất của (18) cũng là một dãy khớp (X, p. 8, đn. 1). Như vậy, ta biết rằng $v_{L_0}$ là song ánh (resp. rằng $v_{L_0}$ và $v_{L_1}$ là song ánh) (II, p. 75, mđ. 2). Nếu ta chỉ giả sử rằng $v_{L_0}$ là song ánh, thì suy ra từ (18) rằng $v_{L_0} \circ T(w) = T'(w) \circ v_E$ là đơn ánh, do đó $v_E$ cũng vậy. Nếu ta giả sử rằng $v_{L_0}$ và $v_{L_1}$ đều song ánh, thì ta suy ra từ hq. 2 (ii) của X, p. 6 rằng $v_E$ là toàn ánh, và vì ta vừa thấy rằng $v_E$ là đơn ánh, nên nó là song ánh.

**HỆ QUẢ. — Mọi môđun phẳng có trình bày hữu hạn đều là xạ ảnh.**

Thật vậy, cho $E$ là một A-môđun phẳng và có trình bày hữu hạn. Áp dụng (*b*) cho trường hợp $B = A, G = {}_sA_d, F = E$, ta thấy rằng đồng cấu chính tắc

$$
\mathrm{Hom}_A(E, A) \otimes_A E \to \mathrm{Hom}_A(E, E)
$$

là toàn ánh. Điều này kéo theo rằng $E$ là xạ ảnh (II, p. 77, nhận xét 1).

Theo hệ quả trước và mđ. 5 của X, p. 10, có sự đồng nhất giữa các môđun phẳng có trình bày hữu hạn và các môđun xạ ảnh kiểu hữu hạn. Mặt khác, tồn tại các môđun phẳng kiểu hữu hạn không có trình bày hữu hạn, do đó không xạ ảnh (*cf.* X, p. 170, bài tập 17, tuy nhiên xem X, p. 169, các bài tập 13 và 14).

### 6. Cấu trúc của các môđun phẳng

**Bổ đề 2. — Cho I là một tập hợp có thứ tự lọc phải, $(E_\alpha, \varphi_{\beta\alpha})$ một hệ quy nạp các tập hợp đối với I, E là giới hạn quy nạp của nó và $\varphi_\alpha : E_\alpha \to E, \alpha \in I$, các ánh xạ chính tắc. Cho $f : I \to I$ là một ánh xạ sao cho $f(\alpha) > \alpha$ với $\alpha \in I$, và giả sử rằng với mỗi $\alpha \in I$, đã cho một tập hợp $L_\alpha$ và các ánh xạ $u_\alpha : E_\alpha \to L_\alpha$ và $v_\alpha : L_\alpha \to E_{f(\alpha)}$ sao cho $v_\alpha \circ u'_\alpha = \varphi_{f(\alpha), \alpha}$. Cho J là tập hợp có thứ tự thu được bằng cách trang bị cho I quan hệ « $\alpha \leq \beta$ nếu $\alpha = \beta$ hoặc $f(\alpha) \leq \beta$ ». Nếu $\alpha, \beta \in J$ với $\alpha \leq \beta$, cho $\psi_{\beta\alpha} : L_\alpha \to L_\beta$ là ánh xạ sao cho $\psi_{\beta\alpha} = \mathrm{Id}$ nếu $\alpha = \beta$, $\psi_{\beta\alpha} = u_\beta \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha$ nếu $f(\alpha) \leq \beta$. Nếu $\alpha \in J$, cho $\psi_\alpha : L_\alpha \to E$ là ánh xạ $\varphi_{f(\alpha)} \circ v_\alpha$. Khi đó tập hợp có thứ tự J là lọc, $(L_\alpha, \psi_{\beta\alpha})$ là một hệ quy nạp đối với J, $(\psi_\alpha)$ là một hệ quy nạp các ánh xạ và ánh xạ $\psi : \lim_{\alpha \in J} L_\alpha \to E$ suy ra từ các $\psi_\alpha$ là song ánh.**

Rõ ràng J là quy nạp. Nếu $\alpha, \beta \in J$ với $\alpha < \beta$, ta có
$$
\psi_\beta \circ \psi_{\beta \alpha} = \varphi_{f(\beta)} \circ v_\beta \circ u_\beta \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha \\
= \varphi_{f(\beta)} \circ \varphi_{f(\beta), \beta} \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha = \varphi_{f(\alpha)} \circ v_\alpha = \psi_\alpha ;
$$
tương tự, nếu $\alpha, \beta, \gamma \in J$ với $\alpha < \beta < \gamma$, ta có
$$
\psi_{\gamma \beta} \circ \psi_{\beta \alpha} = u_\gamma \circ \varphi_{\gamma, f(\beta)} \circ v_\beta \circ u_\beta \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha \\
= u_\gamma \circ \varphi_{\gamma, f(\beta)} \circ \varphi_{f(\beta), \beta} \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha = u_\gamma \circ \varphi_{\gamma, f(\alpha)} \circ v_\alpha = \psi_{\gamma \alpha} .
$$
Ta chứng minh khẳng định cuối cùng: với mỗi $\alpha \in J$, ta có
$$
\psi_\alpha \circ u_\alpha = \varphi_{f(\alpha)} \circ v_\alpha \circ u_\alpha = \varphi_{f(\alpha)} \circ \varphi_{f(\alpha), \alpha} = \varphi_\alpha ,
$$
do đó $\varphi_\alpha(E_\alpha) = \psi_\alpha(u_\alpha(E_\alpha)) \subset \psi_\alpha(L_\alpha)$, và $\psi$ là toàn ánh. Lấy $\alpha \in J$ và $x, y \in L_\alpha$ sao cho $\psi_\alpha(x) = \psi_\alpha(y)$, tức là $\varphi_{f(\alpha)}(v_\alpha(x)) = \varphi_{f(\alpha)}(v_\alpha(y))$; tồn tại $\beta \in I$, $\beta \geq f(\alpha)$ sao cho
$$
\varphi_{\beta, f(\alpha)}(v_\alpha(x)) = \varphi_{\beta, f(\alpha)}(v_\alpha(y)) ,
$$
do đó
$$
\psi_{\beta, \alpha}(x) = u_\beta(\varphi_{\beta, f(\alpha)}(v_\alpha(x))) = u_\beta(\varphi_{\beta, f(\alpha)}(v_\alpha(y))) = \psi_{\beta, \alpha}(y) .
$$
và $\psi$ là đơn ánh.

#### Định lý 1 (D. Lazard) {#alg-x-s1-thm-1 .statement}

Với mọi A-môđun E, các điều kiện sau là tương đương:
(i) E là phẳng.
(ii) Với mọi A-môđun P có trình bày hữu hạn, đồng cấu chính tắc
$$
\operatorname{Hom}_A(P, A) \otimes_A E \to \operatorname{Hom}_A(P, E)
$$
là toàn ánh.
(iii) Với mọi A-môđun P có trình bày hữu hạn và mọi đồng cấu $u : P \to E$, tồn tại một A-môđun tự do L kiểu hữu hạn và các đồng cấu $v : P \to L$ và $w : L \to E$ sao cho $u = w \circ v$.
(iv) Tồn tại một tập hợp có thứ tự lọc J, một hệ quy nạp các môđun tự do kiểu hữu hạn $(L_j)_{j \in J}$ và một đẳng cấu của E lên $\lim \overrightarrow{L_j}$.
(iv) $\Rightarrow$ (i) : điều này suy ra từ mệnh đề 4 (ii) của X, p. 8.
(i) $\Rightarrow$ (ii) : điều này suy ra từ mệnh đề 8b) của X, p. 12.
(ii) $\Rightarrow$ (iii) : cho P là một A-môđun có trình bày hữu hạn và $u : P \to E$ là một đồng cấu; theo (ii), tồn tại $v_1, \ldots, v_n \in \operatorname{Hom}_A(P, A)$, $w_1, \ldots, w_n \in E$ sao cho $u(x) = \sum v_i(x) w_i$ với mọi $x \in P$; nếu $v : P \to A^n$ là đồng cấu có các thành phần $(v_i)$ và $w : A^n \to E$ là đồng cấu $(a_i) \mapsto \sum a_i w_i$, thì quả thật ta có $u = w \circ v$.
(iii) $\Rightarrow$ (iv) : giả sử (iii) được thỏa mãn, và cho $(E_\alpha, \varphi_{\beta, \alpha})$ là một hệ quy nạp, đối với một tập hợp lọc I, các A-môđun có trình bày hữu hạn, với giới hạn quy nạp E

(X, p. 11, mệnh đề 7). Thay thế I bằng tích từ điển I × N, với E_{(α,n)} = E_α với mọi n, ta có thể giả sử rằng I không có phần tử lớn nhất. Với mỗi α ∈ I, cho L_α là một A-môđun tự do kiểu hữu hạn và cho u_α : E_α → L_α, v'_α : L_α → E là các đồng cấu sao cho v'_α ∘ u_α là ánh xạ chính tắc φ_α của E_α vào E; vì L_α là tự do kiểu hữu hạn và I không có phần tử lớn nhất, tồn tại một chỉ số β > α và một đồng cấu v''_α : L_α → E_β sao cho v'_α = φ_β ∘ v''_α; vì φ_β ∘ v''_α ∘ u_α = φ_β ∘ φ_β,α và E_α có trình bày hữu hạn, suy ra từ mệnh đề 8a) của X, p. 12, rằng tồn tại γ ≥ β sao cho φ_{γβ} ∘ v''_α ∘ u_α = φ_{γβ} ∘ φ_{βα} = φ_{γα} ; đặt γ = f(α) và gọi v_α là đồng cấu φ_{γβ} ∘ v''_α từ L_α vào E_{f(α)} ; ta có v_α ∘ u_α = φ_{f(α),α}. Khi đó ta có thể áp dụng bổ đề 2, do đó suy ra (iv).

#### Hệ quả {#alg-x-s1-n6-cor-1 .statement}

Giả sử A giao hoán. Với mọi A-môđun phẳng E, các A-môđun T(E), S(E), Λ(E), T^n(E), S^n(E), Λ^n(E) đều phẳng.

Thật vậy, E là giới hạn quy nạp của một hệ lọc $(L_j)$ các A-môđun tự do kiểu hữu hạn, do đó T(E) (tương ứng S(E), v.v.) là giới hạn quy nạp của hệ lọc các A-môđun tự do T(L_j) (tương ứng S(L_j), v.v.), vì thế là phẳng (x. III, p. 61, mệnh đề 6, p. 62, định lý 1, p. 73, mệnh đề 8, p. 75, định lý 1, p. 83, mệnh đề 9, và p. 86, định lý 1).

#### Nhận xét {#alg-x-s1-n6-rem-1 .statement}

Xét trong (ii) một trình bày hữu hạn A_s^J \xrightarrow{c} A_s^I \to P \to 0, ta thu được điều kiện (ii’) vẫn tương đương với các điều kiện trước:

(ii’) Với mọi ma trận hữu hạn (c_{ij})_{i \in I, j \in J} gồm các phần tử của A, mọi nghiệm

$$
e = (e_i)_{i \in I} \in E^I
$$

của hệ phương trình tuyến tính thuần nhất

$$
\sum_{i \in I} c_{ij} e_i = 0,\quad j \in J,
$$

đều có thể viết thành b_1 z_1 + \cdots + b_n z_n, trong đó b_1, ..., b_n \in E và với r = 1, ..., n, z_r = (z_{r,i})_{i \in I} là một nghiệm trong A^I của hệ phương trình

$$
\sum_{i \in I} z_{r,i} c_{ij} = 0,\quad j \in J.
$$

### 7. Môđun nội xạ

#### Định nghĩa 2 {#alg-x-s1-def-2 .statement}

Ta nói rằng A-môđun E là nội xạ nếu, với mọi dãy khớp các A-môđun và các đồng cấu

(19)
$$
M' \xrightarrow{u} M \xrightarrow{v} M'',
$$
dãy các ánh xạ $\mathbf{Z}$-tuyến tính

(20)
$$
\operatorname{Hom}_A(M'', E) \xrightarrow{\operatorname{Hom}_A(v, 1)} \operatorname{Hom}_A(M, E) \xrightarrow{\operatorname{Hom}_A(u, 1)} \operatorname{Hom}_A(M', E)
$$
là khớp.

#### Bổ đề 3 {#alg-x-s1-lem-3 .statement}

*Để A-môđun E là nội xạ, điều kiện cần và đủ là, với mọi ánh xạ A-tuyến tính đơn ánh $u : M' \to M$, ánh xạ*

$$
\operatorname{Hom}_A(u,1) : \operatorname{Hom}_A(M,E) \to \operatorname{Hom}_A(M',E)
$$

*là toàn ánh.*

Nếu $E$ là đơn ánh và nếu $u : M' \to M$ là đơn ánh, thì dãy $0 \to M' \xrightarrow{u} M$ là khớp, và do đó dãy $\operatorname{Hom}(M,E) \xrightarrow{\operatorname{Hom}(u,1)} \operatorname{Hom}(M',E) \to 0$ cũng khớp, và $\operatorname{Hom}(u,1)$ là toàn ánh. Ngược lại, xét dãy khớp (19); đặt $M''_1=\nu(M)$ và gọi $i : M''_1 \to M''$ là đơn ánh chính tắc và $p : M \to M''_1$ là ánh xạ $m\mapsto \nu(m)$. Dãy $M' \xrightarrow{u} M \xrightarrow{p} M''_1 \to 0$ là khớp; theo II, p. 36, định lý 1, dãy

$$
\operatorname{Hom}_A(M''_1,E)
\xrightarrow{\operatorname{Hom}(p,1)}
\operatorname{Hom}_A(M,E)
\xrightarrow{\operatorname{Hom}(u,1)}
\operatorname{Hom}_A(M',E)
$$

là khớp. Hơn nữa, ta có $\operatorname{Hom}(\nu,1)=\operatorname{Hom}(p,1)\circ\operatorname{Hom}(i,1)$. Nếu $E$ thỏa mãn điều kiện của bổ đề, $\operatorname{Hom}(i,1)$ là toàn ánh, do đó ảnh của $\operatorname{Hom}(\nu,1)$ cũng là ảnh của $\operatorname{Hom}(p,1)$, và dãy (20) là khớp.

#### Nhận xét {#alg-x-s1-n7-rem-1 .statement}

Cho $E$ là một A-môđun đơn ánh, $u : M' \to M$ và $f : M' \to E$ là các đồng cấu của A-môđun. Nếu $\operatorname{Ker}u\subset\operatorname{Ker}f$, tồn tại một đồng cấu $g : M \to E$ sao cho $g\circ u=f$. Điều này thực vậy suy ra từ điều nói trên áp dụng cho đơn cấu $M'/\operatorname{Ker}u \to M$ suy ra từ $u$.

#### Mệnh đề 9 {#alg-x-s1-prop-9 .statement}

*Cho $(E_i)_{i\in I}$ là một họ các A-môđun, $E=\prod_{i\in I}E_i$ là tích của chúng. Để A-môđun $E$ là đơn ánh, điều kiện cần và đủ là mỗi $E_i$ đều như vậy.*

Cho $u : M' \to M$ là một đơn cấu của A-môđun. Để đồng cấu tích

$$
\prod_{i\in I}\operatorname{Hom}_A(M,E_i)
\longrightarrow
\prod_{i\in I}\operatorname{Hom}_A(M',E_i)
$$

là toàn ánh, điều kiện cần và đủ là mỗi đồng cấu $\operatorname{Hom}_A(M,E_i)\to\operatorname{Hom}_A(M',E_i)$ đều như vậy (II, p. 10, mệnh đề 5); điều này chứng minh mệnh đề vì $\prod_{i\in I}\operatorname{Hom}_A(M,E_i)$ được đồng nhất một cách chính tắc với $\operatorname{Hom}_A(M,E)$.

#### Mệnh đề 10 {#alg-x-s1-prop-10 .statement}

*Cho $E$ là một A-môđun. Để $E$ là đơn ánh, điều kiện cần và đủ là với mọi iđêan $a$ của $A$ và mọi A-đồng cấu $f : a\to E$, tồn tại $e\in E$ sao cho*

$$
f(a)=ae
$$

*với mọi $a\in a$.*

Giả sử $E$ là đơn ánh; cho $a$ là một iđêan của $A$, $f : a\to E$ là một A-đồng cấu, và ký hiệu bởi $i : a\to A$ đơn ánh chính tắc. Khi đó ánh xạ

$$
\operatorname{Hom}_A(i,1) : \operatorname{Hom}_A(A,E)\to\operatorname{Hom}_A(a,E)
$$

là toàn ánh (định nghĩa 2); nếu $g\in\operatorname{Hom}_A(A,E)$ sao cho $f=g\circ i$, ta có

$$
f(a)=g(a)=ag(1)
$$

với mọi $a\in a$.

Ngược lại, giả sử điều kiện của mệnh đề được thỏa mãn, cho $M$ là một A-môđun, $N$ là một môđun con của $M$, $u : N\to E$ là một A-đồng cấu, và chứng minh rằng tồn tại một A-đồng cấu $\bar u : M\to E$ mở rộng $u$ (x. *bổ đề* 3). Gọi $\mathcal P$ là tập hợp các cặp $(P,v)$ trong đó $P$ là một môđun con của $M$ chứa $N$ và $v$ là một đồng cấu từ $P$ vào $E$ mở rộng $u$. Tập hợp $\mathcal P$ được sắp thứ tự bởi quan hệ mở rộng là *quy nạp*: nếu $(P_j, v_j)$ là một họ được sắp thứ tự toàn phần các phần tử của $\mathcal{P}$, đặt $Q = \cup P_j$ và gọi $w : Q \to E$ là ánh xạ duy nhất cảm sinh $v_j$ trên $P_j$ với mọi $j$; khi đó $(Q, w) \in \mathcal{P}$ và $(Q, w)$ trội hơn $(P_j, v_j)$ với mọi $j$. Khi đó gọi $(P, v)$ là một phần tử cực đại của $\mathcal{P}$ (E, III, p. 20, Định lý 2); chỉ cần chứng minh rằng $P = M$. Lấy $x \in M$ và gọi $\alpha$ là iđêan của các $a \in A$ sao cho $ax \in P$; đặt $f(a) = v(ax)$ với $a \in \alpha$; таким образом thu được một A-đồng cấu $f : \alpha \to E$. Khi đó gọi $e$ là một phần tử của $E$ sao cho $f(a) = ae$ với mọi $a \in \alpha$. Đặt $P' = P + Ax$ và gọi $v' : P' \to E$ là A-đồng cấu duy nhất sao cho $v'(p + ax) = v(p) + ae$ với $p \in P, a \in A$; khi đó $(P', v')$ thuộc $\mathcal{P}$ và trội hơn $(P, v)$, do đó $P' = P$, nghĩa là $x \in P$, điều này hoàn tất chứng minh.

#### Hệ quả 1 {#alg-x-s1-prop-10-cor-1 .statement}

*Nếu vành $A$ là Noether trái, mọi tổng trực tiếp của các $A$-môđun đơn ánh đều là đơn ánh.*

Cho $(E_i)_{i \in I}$ là một họ các $A$-môđun đơn ánh, gọi $E$ là tổng trực tiếp của chúng, gọi $\alpha$ là một iđêan của $A$ và gọi $u : \alpha \to E$ là một $A$-đồng cấu. Vì $A$ là Noether, $\alpha$ là kiểu hữu hạn, và do đó ánh xạ chính tắc

$$
\varphi : \bigoplus_{i \in I} \operatorname{Hom}_A(\alpha, E_i) \to \operatorname{Hom}_A(\alpha, E)
$$

là song ánh; gọi $(u_i)$ là ảnh ngược của $u$ bởi $\varphi$. Vì mỗi $E_i$ là đơn ánh, và họ $(u_i)$ có giá hữu hạn, tồn tại một phần tử $(e_i)_{i \in I}$ của $E$ sao cho $u_i(a) = ae_i$ với mọi $a \in \alpha$ và mọi $i \in I$, do đó $u(a) = a((e_i))$ với mọi $a \in \alpha$, và $E$ là đơn ánh.

#### Nhận xét {#alg-x-s1-n7-rem-2 .statement}

Nếu mọi tổng trực tiếp của các $A$-môđun đơn ánh đều là đơn ánh, thì vành $A$ là Noether trái (X, p. 170, bài tập 21).

Giả sử $A$ là nguyên. Ta nói rằng $A$-môđun $E$ là *chia được* nếu phép vị tự $a_E$ là toàn ánh với mọi phần tử khác không $a$ của $A$.

#### Hệ quả 2 {#alg-x-s1-prop-10-cor-2 .statement}

*Giả sử $A$ là nguyên.*
  *a)* *Mọi $A$-môđun đơn ánh đều chia được.*
  *b)* *Mọi $A$-môđun không xoắn (II, p. 115) và chia được đều đơn ánh.*
  *c)* *Nếu $A$ là chính, mọi $A$-môđun chia được đều đơn ánh.*

Nếu $a \in A$ là khác không, thì $a_A$ là đơn ánh; mặt khác, với mọi $A$-môđun $E$, phép vị tự $a_E$ được đồng nhất một cách chính tắc với

$$
\operatorname{Hom}(a_A, 1) : \operatorname{Hom}_A(A, E) \to \operatorname{Hom}_A(A, E),
$$

vì thế $E$ là chia được khi và chỉ khi $\operatorname{Hom}(a_E, 1_E)$ là toàn ánh với mọi $a \in A$ khác không. Do đó mệnh đề *a)* suy ra từ Định nghĩa 2 (X, p. 15).

Cho $E$ là một A-môđun chia được; giả sử rằng $A$ là chính (resp. $E$ không xoắn) và hãy chứng minh rằng $E$ là nội xạ bằng cách áp dụng mệnh đề 10. Cho $\alpha$ là một iđêan của $A$ và $f : \alpha \to E$ là một A-đồng cấu. Lấy $x \in \alpha$ sao cho $\alpha = Ax$ (resp. sao cho $x \neq 0$ nếu $\alpha \neq 0$), và lấy $e \in E$ sao cho $xe = f(x)$. Hãy chứng minh rằng với mọi $a \in \alpha$, ta có

$$
f(a) = ae;
$$

điều này hiển nhiên nếu $a \in Ax$, do đó mệnh đề được chứng minh trong trường hợp A là chính; nếu E không xoắn và nếu $xa \in a$, ta có $xf(a) = f(ax) = axe$, do đó $f(a) = ae$ vì $x$ khác không nếu $a \neq 0$.

#### Ví dụ 1 {#alg-x-s1-n7-exa-1 .statement}

Nếu A là nguyên, trường phân thức K của A là một A-môđun nội xạ. Nếu A là chính, $K/A$ là một A-môđun nội xạ.
2) Chẳng hạn, các $\mathbf{Z}$-môđun $\mathbf{Q}$ và $\mathbf{Q}/\mathbf{Z}$ là nội xạ.
3) Cho A là một miền iđêan chính và cho $a$ là một phần tử *khác không* của A. Khi đó $A/aA$ là một $A/aA$-môđun nội xạ (X, p. 170, bài tập 20).

### 8. Các môđun đối sinh nội xạ

#### Mệnh đề 11 {#alg-x-s1-prop-11 .statement}

*Nếu B là một vành, F là một B-môđun và P là một song môđun (B, A). Nếu F là một B-môđun nội xạ và P là một A-môđun phẳng, thì $\mathrm{Hom}_B(P, F)$ là một A-môđun nội xạ.*

Cho $u : M' \to M$ là một đơn cấu của các A-môđun. Ta có một biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Hom}_A(M, \mathrm{Hom}_B(P, F)) & \xrightarrow{\mathrm{Hom}_A(u, 1)} & \mathrm{Hom}_A(M', \mathrm{Hom}_B(P, F)) \\
\beta \downarrow & & \beta' \downarrow \\
\mathrm{Hom}_B(P \otimes_A M, F) & \xrightarrow{\mathrm{Hom}(1_P \otimes u, 1_F)} & \mathrm{Hom}_B(P \otimes_A M', F)
\end{array}
$$

trong đó $\beta$ và $\beta'$ là các đẳng cấu chính tắc của II, p. 74. Vì P là phẳng trên A, đồng cấu $1_P \otimes u : P \otimes_A M' \to P \otimes_A M$ là đơn ánh. Vì F là nội xạ, $\mathrm{Hom}(1_P \otimes u, 1_F)$ là toàn ánh, do đó $\mathrm{Hom}_A(u, 1)$ cũng vậy, điều này chứng minh rằng $\mathrm{Hom}_F(P, F)$ là một A-môđun nội xạ (X, p. 16, bổ đề 3).

#### Định nghĩa 3 {#alg-x-s1-def-3 .statement}

*Người ta nói rằng A-môđun E là một đối sinh nếu, với mọi A-môđun M và mọi phần tử khác không x của M, tồn tại một A-đồng cấu $u : M \to E$ sao cho $u(x) \neq 0$.*

Người ta nói rằng A-môđun L là một *môđun sinh* nếu, với mọi A-môđun M và mọi phần tử x của M, tồn tại một A-đồng cấu $u : L \to M$ sao cho $x \in u(L)$. Chẳng hạn, A-môđun $A_s$ là một môđun sinh.

#### Mệnh đề 12 {#alg-x-s1-prop-12 .statement}

*Cho E là một A-môđun nội xạ. Để E là một đối sinh, điều kiện cần và đủ là $\mathrm{Hom}_A(S, E) \neq 0$ đối với mọi A-môđun đơn S.*

Điều kiện này hiển nhiên là cần. Ngược lại, cho M là một A-môđun và x là một phần tử khác không của M; môđun con $Ax$ của M có một thương đơn S (VIII, § 2, no 1, mệnh đề 3). Nếu $\mathrm{Hom}_A(S, E) \neq 0$, thì $\mathrm{Hom}_A(Ax, E) \neq 0$ và tồn tại một đồng cấu $f : Ax \to E$ sao cho $f(x) \neq 0$; vì E là nội xạ, $f$ kéo dài thành một đồng cấu $u$ từ M vào E và ta có $u(x) = f(x) \neq 0$.

#### Ví dụ {#alg-x-s1-n8-exa-1 .statement}

$\mathbf{Z}$-môđun đơn ánh $\mathbf{Q}/\mathbf{Z}$ (X, p. 18, ví dụ 2) là một đối sinh.
Thật vậy, mọi môđun đơn của $\mathbf{Z}$-môđun đều đẳng cấu với một môđun $\mathbf{Z}/p\mathbf{Z}$, $p\ne 0$, và $\operatorname{Hom}_{\mathbf{Z}}(\mathbf{Z}/p\mathbf{Z},\mathbf{Q}/\mathbf{Z})$ là khác không (chẳng hạn nó chứa phần tử của $\mathbf{Z}/p\mathbf{Z}$ thu được bằng cách chuyển qua thương từ đồng cấu $x\mapsto x/p$ của $\mathbf{Z}$ vào $\mathbf{Q}$).

#### Mệnh đề 13 {#alg-x-s1-prop-13 .statement}

Cho $B$ là một vành, $F$ là một $B$-môđun đơn ánh đối sinh, $P$ là một $(B,A)$-song môđun. Giả sử rằng $P$ là phẳng trên $A$ và sao cho $P\otimes_A S\ne 0$ đối với mọi $A$-môđun đơn $S$ (* nghĩa là, phẳng trung thành trên $A$ theo nghĩa của AC, I, §). Khi đó $A$-môđun $\operatorname{Hom}_B(P,F)$ là một đối sinh và đơn ánh.

Thật vậy, $\operatorname{Hom}_B(P,F)$ là đơn ánh theo mệnh đề 11. Mặt khác, với mọi $A$-môđun đơn $S$, $\operatorname{Hom}_A(S,\operatorname{Hom}_B(P,F))$ đẳng cấu với $\operatorname{Hom}_B(P\otimes_A S,F)$, do đó là khác không vì $P\otimes_A S\ne 0$ và $B$-môđun $F$ là một đối sinh; vậy $A$-môđun $\operatorname{Hom}_B(P,F)$ là một đối sinh theo mệnh đề 12.

#### Hệ quả 1 {#alg-x-s1-prop-13-cor-1 .statement}

A-môđun $E_A=\operatorname{Hom}_{\mathbf{Z}}(A,\mathbf{Q}/\mathbf{Z})$ là đơn ánh và là một đối sinh.

Ta áp dụng mệnh đề 13 với $B=\mathbf{Z}$, $F=\mathbf{Q}/\mathbf{Z}$ (ví dụ) và $P=A_d$.

Với mọi $A$-môđun $M$, đặt

$$
I^0(M)=E_A^{\operatorname{Hom}(M,E_A)}
$$

và gọi $e_M:M\to I^0(M)$ là đồng cấu gán cho $m\in M$ phần tử

$$
(\varphi(m))_{\varphi\in\operatorname{Hom}(M,E_A)}\in I^0(M).
$$

Khi đó:

#### Hệ quả 2 {#alg-x-s1-prop-13-cor-2 .statement}

A-môđun $I^0(M)$ là đơn ánh và A-đồng cấu $e_M:M\to I^0(M)$ là đơn ánh.

Thật vậy, $I^0(M)$ là đơn ánh, vì $E_A$ là đơn ánh (X, p. 16, mệnh đề 9), mặt khác $e_M$ là đơn ánh vì $E_A$ là một đối sinh.

#### Hệ quả 3 {#alg-x-s1-prop-13-cor-3 .statement}

Mọi $A$-môđun đều đẳng cấu với một môđun con của một $A$-môđun đơn ánh.

#### Hệ quả 4 {#alg-x-s1-prop-13-cor-4 .statement}

Để $A$-môđun $E$ là đơn ánh, điều kiện cần và đủ là mọi A-đồng cấu đơn ánh $f:E\to F$ đều có một phép co rút $A$-tuyến tính.

Giả sử $E$ là nội xạ và gọi $f:E\to F$ là một $A$-đồng cấu đơn cấu. Khi đó

$$
\operatorname{Hom}_A(f,1_E):\operatorname{Hom}_A(F,E)\to\operatorname{Hom}_A(E,E)
$$

là toàn ánh; do đó tồn tại $r\in\operatorname{Hom}_A(F,E)$ sao cho $r\circ f=1_E$ và $r$ là một phép co rút $A$-tuyến tính của $f$. Ngược lại, tồn tại một $A$-môđun nội xạ $I$ và một $A$-đồng cấu đơn cấu $f:E\to I$ (hệ quả 2); nếu $f$ có một phép co rút $A$-tuyến tính, thì $E$ là nội xạ theo mệnh đề 9 của X, p. 16.

### 9. Bao nội xạ

#### Định nghĩa 4 {#alg-x-s1-def-4 .statement}

Cho $M$ là một $A$-môđun. Một bao nội xạ của $M$ là một cặp $(I,i)$, trong đó $I$ là một $A$-môđun nội xạ và $i:M\to I$ là một đồng cấu có tính chất sau đây:

(E) để một môđun con P của I bằng không, điều kiện cần và đủ là i^{-1}(P) bằng không.

Chú ý rằng (E) kéo theo i là đơn ánh. Người ta thường đồng nhất M với môđun con i(M) của I, và khi đó nói rằng I là một bao nội xạ của M.

#### Ví dụ 1 {#alg-x-s1-n9-exa-1 .statement}

Giả sử rằng A nguyên và M không xoắn. Gọi K là trường các phân thức của A và gọi i : M → K ⊗_A M là đồng cấu chính tắc. Khi đó (K ⊗_A M, i) là một bao nội xạ của M (II, p. 116, mệnh đề 26 và X, p. 17, hệ quả 2).

#### Định lý 2 {#alg-x-s1-thm-2 .statement}

Cho M là một A-môđun.
a) M có các bao nội xạ.
b) Nếu (I, i) và (J, j) là hai bao nội xạ của M, thì tồn tại một đẳng cấu f : I → J sao cho f ∘ i = j.

Cần chú ý rằng đồng cấu f mà sự tồn tại được khẳng định trong b) nói chung không được xác định duy nhất.

a) Ta có thể giả sử rằng M là một môđun con của một A-môđun nội xạ E (X, p. 19, hệ quả 3). Xét tập hợp F, được sắp thứ tự bởi quan hệ bao hàm, gồm các môđun con I của E, chứa M, và sao cho đơn ánh chính tắc i : M → I thỏa mãn tính chất (E). Vì F là quy nạp, nó có một phần tử cực đại (E, III, p. 20); gọi I là một phần tử cực đại của F. Chỉ cần chứng minh rằng I là một môđun con hạng tử trực tiếp của E. Gọi N là một môđun con của E sao cho N ∩ I = 0, và là cực đại đối với tính chất này (một N như vậy tồn tại theo loc. cit.). Đồng cấu hợp thành

$$
I \xrightarrow{u} E \xrightarrow{v} E/N,
$$

trong đó u và v là các đồng cấu chính tắc, là đơn ánh; vì E là nội xạ, do đó tồn tại một đồng cấu w : E/N → E sao cho w ∘ v ∘ u = u, nghĩa là w ∘ v(x) = x với $x$ thuộc I. Đặt I′ = Im(w) = Im(w ∘ v) và gọi i′ : M → I′ là đơn ánh chính tắc. Khi đó I ⊂ I′; để hoàn tất chứng minh, chỉ cần chứng minh rằng i′ thỏa mãn điều kiện (E): điều này kéo theo I = I′ (do tính chất cực đại của I) và vì thế w ∘ v là một phép chiếu của E lên I.

Vậy gọi P là một môđun con của I′ sao cho P ∩ M = 0. Ta có P = w ∘ v(Q), trong đó Q là một môđun con của E chứa N; hơn nữa

$$
Q \cap M = w \circ v(Q \cap M) \subset P \cap M = 0,
$$

do đó Q ∩ I = 0 vì i : M → I có tính chất (E). Bởi tính chất cực đại của N, điều này kéo theo Q = N, nghĩa là v(Q) = 0, do đó P = 0, điều phải chứng minh.

b) Gọi (I, i) và (J, j) là hai bao nội xạ của M. Vì J là nội xạ, tồn tại một đồng cấu f : I → J sao cho f ∘ i = j; ta có

$$
i^{-1}(\mathrm{Ker}\,f') = \mathrm{Ker}\,j = 0,
$$

do đó Ker f = 0 và f là đơn ánh. Khi đó f(I) là một môđun con nội xạ của J, nên là một nhân tử trực tiếp; vì j thỏa mãn (E), điều này kéo theo f(I) = J và f là song ánh.

#### Nhận xét 1 {#alg-x-s1-n9-rem-1 .statement}

Gọi (I, i) là một bao nội xạ của M và $j : M \to J$ là một đồng cấu đơn cấu từ M vào một A-môđun nội xạ J. Theo chứng minh ở trên, tồn tại một đồng cấu *đơn cấu* $f : I \to J$ sao cho $f \circ i = j$.

#### Nhận xét 2 {#alg-x-s1-n9-rem-2 .statement}

Gọi (I, i) là một bao nội xạ của M. Đồng nhất M với môđun con $i(M)$ của I. Với mọi môđun con N của M, tồn tại một môđun con nội xạ của I là một bao nội xạ của N (áp dụng *Nhận xét* 1 cho N). Ngược lại, mọi môđun con nội xạ J của I đều là một bao nội xạ của $J \cap M$.

#### Mệnh đề 14 {#alg-x-s1-prop-14 .statement}

*Cho I là một A-môđun nội xạ khác không. Các điều kiện sau là tương đương*:
(i) *I không phân tích được* (VII, § 4, no 8, def. 3);
(ii) *0 không là giao của hai môđun con khác không của I*;
(iii) *I là bao nội xạ của mọi môđun con khác không của nó*;
(iv) *vành* $\mathrm{End}_A(I)$ *là địa phương* (VIII, § 1, no 4, def. 4).

(i) $\Rightarrow$ (iii) : gọi M là một môđun con khác không của I. Theo *Nhận xét* 2 ở trên, tồn tại một môđun con I’ của I, là một bao nội xạ của M. Vì I’ khác không và là một nhân tử trực tiếp trong I, nên ta có $I = I'$ nếu I không phân tích được.

(iii) $\Rightarrow$ (ii) : gọi E và F là hai môđun con của I, sao cho $E \cap F = 0$. Nếu $E \neq 0$, thì I là một bao nội xạ của E theo (iii), do đó « $E \cap F = 0$ » kéo theo « $F = 0$ ».

(ii) $\Rightarrow$ (i) : điều này là tầm thường.

(iv) $\Rightarrow$ (i) : điều này suy ra từ VIII, § 1, no 6, prop. 13.

(i) $\Rightarrow$ (iv) : giả sử I không phân tích được. Trước hết, chú ý rằng mọi tự đồng cấu đơn cấu $f$ của I đều là song ánh (vì khi đó $f(I)$ là một môđun con hạng tử trực tiếp khác không của I). Hơn nữa, mọi tự đồng cấu $f$ của I mà hạn chế của nó lên một môđun con khác không E của I là đơn ánh, thì đều là đơn ánh (thật vậy, vì (i) $\Rightarrow$ (iii), I là một bao nội xạ của E, do đó « $E \cap \mathrm{Ker}\ f = 0$ » kéo theo « $\mathrm{Ker}\ f = 0$ »). Như vậy, gọi $f$ là một phần tử không khả nghịch của $\mathrm{End}_A(M)$; theo VIII, § 1, no 4, prop. 9, vấn đề là chứng minh rằng $1 - f$ là khả nghịch. Vì $f$ không là đơn ánh, ta có $\mathrm{Ker}\ f \neq 0$; vì hạn chế của $1 - f$ lên $\mathrm{Ker}\ f$ là đơn ánh, nên $1 - f$ là đơn ánh, do đó là song ánh.

#### Hệ quả 1 {#alg-x-s1-prop-14-cor-1 .statement}

*Quan hệ “I là một lớp các A-môđun nội xạ không phân tích được” là xác định tập*.

Thật vậy, theo (iii), mọi A-môđun nội xạ không phân tích được đều là bao nội xạ của một A-môđun đơn sinh.

#### Hệ quả 2 {#alg-x-s1-prop-14-cor-2 .statement}

*Cho M là một A-môđun, I là một bao nội xạ của M. Để I không phân tích được, điều kiện cần và đủ là 0 không là giao của hai môđun con khác không của M*.

Điều kiện là cần theo mệnh đề 14 ((i) $\Rightarrow$ (ii)). Ngược lại, nếu I là tổng trực tiếp của các môđun con khác không $I_1$ và $I_2$, thì ta có:

$$
I_1 \cap M \neq 0,\quad I_2 \cap M \neq 0\quad \text{và}\quad (I_1 \cap M) \cap (I_2 \cap M) = 0 .
$$

#### Ví dụ 2 {#alg-x-s1-n9-exa-2 .statement}

Nếu A giao hoán và Noether, thì các A-môđun nội xạ không phân tích được chính là các bao nội xạ của các môđun A/p, trong đó p là một iđêan nguyên tố (X, p. 171, bài tập 27).

### 10. Cấu trúc của các môđun nội xạ

#### Bổ đề 4 {#alg-x-s1-lem-4 .statement}

Cho M là một A-môđun Noether khác không, I là một bao nội xạ của M. Khi đó I có một môđun con nội xạ không phân tích được.

Hiển nhiên có thể giả sử rằng M là một môđun con của I. Cho N là một môđun con của M sao cho I không là một bao nội xạ của N và là cực đại đối với tính chất này. Theo nhận xét 2 (X, p. 21), tồn tại một môđun con I₁ của I là một bao nội xạ của N; khi đó I₁ là một nhân tử trực tiếp của I, gọi J là một phần bù nhân tử trực tiếp. Ta có J ≠ 0; hãy chứng minh rằng J không phân tích được. Nếu J′ là một môđun con hạng tử trực tiếp khác không của J, thì ta có J′ ∩ M ≠ 0 và

$$(J' \cap M) \cap N \subset J' \cap I_1 = 0.$$

Môđun con N′ = (J′ ∩ M) + N của M là tổng trực tiếp của J′ ∩ M và N, nên thực sự chứa N. Hơn nữa, N′ được chứa trong môđun con J′ + I₁ của J, là tổng trực tiếp của J′ và I₁, do đó nội xạ. Theo tính chất cực đại của N, điều này kéo theo J′ + I₁ = I, do đó J′ = J, và J là không phân tích được.

Kí hiệu $\mathcal{I}$ là tập hợp (X, p. 21, hệ quả 1) các lớp các A-môđun nội xạ không phân tích được.

Nhắc lại (X, p. 17, hệ quả 1) rằng, nếu A là Noether trái, thì mọi A-môđun là tổng trực tiếp của các A-môđun nội xạ đều là nội xạ.

#### Định lý 3 {#alg-x-s1-thm-3 .statement}

Cho I là một A-môđun nội xạ.

a) Nếu I là bao nội xạ của một A-môđun Noether M, thì I là tổng trực tiếp của một họ hữu hạn các môđun con (nội xạ) không phân tích được.

b) Nếu A là Noether trái, thì I là tổng trực tiếp của một họ các môđun con (nội xạ) không phân tích được.

c) Nếu I là tổng trực tiếp của các môđun con (nội xạ) không phân tích được, thì tồn tại một và chỉ một họ các số lực lượng $(a_E)_{E \in \mathcal{I}}$ sao cho I đẳng cấu với

$$\bigoplus_{E \in \mathcal{I}} E^{(a_E)}.$$

Trước hết nhận thấy rằng c) suy ra từ mệnh đề 14 (X, p. 21) và từ VIII, § 1, No. 7, định lý 2. Hãy chứng minh a).

Cho N là một môđun con của M mà các bao nội xạ của nó là tổng trực tiếp của một họ hữu hạn các môđun con không phân tích được, và là cực đại đối với tính chất này (có ít nhất một môđun con như vậy vì M là Noether). Theo nhận xét 2 (X, p. 21), tồn tại một môđun con I₁ của I là một bao nội xạ của N. Nếu I₁ = I, thì chứng minh hoàn tất; nếu không, gọi $J$ là một phần bù nhân tử trực tiếp của $I_1$ trong $I$. Khi đó $J$ là bao nội xạ của môđun Noether $J\cap M$ (loc. cit.), nên có một môđun con nội xạ không phân tích được khác không $J'$ (bổ đề 4). Khi đó $I_1+J'$ là nội xạ, là tổng trực tiếp của một họ hữu hạn các môđun con không phân tích được, và là bao nội xạ của môđun con $(I_1+J')\cap M$ của $M$ mà thực sự chứa $N$, do đó mâu thuẫn.

Giả sử $A$ là Noether trái và hãy chứng minh b). Cho $X$ là hợp của các tập $\operatorname{Hom}_A(E,I)$ với $E\in\mathcal{J}$. Với mỗi tập con $Y$ của $X$, gán một A-môđun $E_Y$ và một A-đồng cấu $f_Y:E_Y\to I$ theo cách sau: $Y$ là hợp của một họ $(Y(E))_{E\in\mathcal{J}}$ trong đó $Y(E)\subset\operatorname{Hom}_A(E,I)$, và đặt

$$
E_Y=\bigoplus_{E\in\mathcal{J}}E^{(Y(E))}
$$

và thành phần của $f$ trên nhân tử trực tiếp của $E_Y$ tương ứng với phần tử $y$ của $Y(E)\subset\operatorname{Hom}_A(E,I)$ là $y:E\to I$. Cho $Y$ là một tập con của $X$ sao cho $f_Y$ là đơn ánh và $Y$ là cực đại đối với tính chất này (một tập con như vậy tồn tại theo E, III, p. 20); chỉ cần chứng minh rằng $f_Y$ là song ánh. Nếu không, gọi $J$ là một phần bù nhân tử trực tiếp của môđun con nội xạ $\operatorname{Im}(f_Y)$ của $I$; vì $J$ khác không, nó có một môđun con Noether khác không (vì A được giả sử là Noether), do đó cũng có một môđun con nội xạ khác không $J'$ là bao nội xạ của một môđun Noether. Theo a), $J'$ là tổng trực tiếp của một họ hữu hạn khác rỗng các môđun con không phân tích được. Do đó tồn tại một tập con hữu hạn khác rỗng $Y'$ của $X$ sao cho $f_{Y'}$ ánh xạ song ánh $E_{Y'}$ lên $J'$. Vì $\operatorname{Im}(f_Y)\cap J'=0$, ta có $Y\cap Y'=\varnothing$ và $f_{Y\cup Y'}$ là đơn ánh; điều này mâu thuẫn với tính chất cực đại của $Y$ và hoàn tất chứng minh.

## BÀI TẬP {#alg-x-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).
