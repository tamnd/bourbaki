---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 4
section_title: Regular elements of a Lie group
lang: vi
source: lie-vii-ix
book_pages: 27-34, 63
pdf_pages: 0037-0044, 0072-0072
extraction: native
subsections:
    - "no": 1
      title: REGULAR ELEMENTS FOR A LINEAR REPRESENTATION
      page: 27
      pdf_page: 37
    - "no": 2
      title: REGULAR ELEMENTS OF A LIE GROUP
      page: 29
      pdf_page: 39
    - "no": 3
      title: RELATIONS WITH REGULAR ELEMENTS OF THE LIE ALGEBRA
      page: 31
      pdf_page: 41
    - "no": 4
      title: APPLICATION TO ELEMENTARY AUTOMORPHISMS
      page: 34
      pdf_page: 44
statements: 18
exercises: 4
content_sha256: 28bc628f68c7062acf4f3714d0b9cc6721cba8dda2a2c6091061429952fc42bb
translated_from: content/en/lie/VII/04_s4_regular_elements_of_a_lie_group.md
source_content_sha256: 6ccb9b5f7ffcd786b5afdaf81ccab18f695f9b397ae110709debf0e21b1adfe3
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-4e40ff51
glossary_version: 34
glossary_terms_sha256: 459d924d82c881b47ebbf1727666c56ad90aa8c8e6e8738ed35efacfc12bfd59
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CÁC PHẦN TỬ CHÍNH QUY CỦA MỘT NHÓM LIE

Trong các số 1, 2 và 3 của đoạn này, ta giả sử rằng $k$ là $\mathbf{R},\mathbf{C}$ hoặc một trường ultramêtric đầy đủ rời rạc có đặc số 0. Ta ký hiệu G là một nhóm Lie hữu hạn chiều trên $k$, $\mathfrak{g}$ là đại số Lie của nó, và $e$ là phần tử đơn vị của nó. Nếu $a\in G$, ta ký hiệu $\mathfrak{g}^1(a)$ là không gian nil của Ad $(a)-1$, nói cách khác là không gian $\mathfrak{g}^1$(Ad($a$)) (xem §1, no. 1).

### 1. CÁC PHẦN TỬ CHÍNH QUY ĐỐI VỚI MỘT BIỂU DIỄN TUYẾN TÍNH

#### Bổ đề 1 {#lie-vii-s4-lem-1 .statement tag=00VU}

Cho M là một đa tạp giải tích trên $k$ và $a= (a_0, . . . , a_{n-1}, a_n= 1)$ là một dãy các hàm giải tích trên M. Với mọi $x\in M$, gọi $r_a(x)$ là cận trên của các $i\in 0, n$ sao cho $a_j(x) = 0$ với $j < i$ và gọi $r_a^0(x)$ là cận trên của các $i\in 0, n$ sao cho $a_j$ là không trên một lân cận của $x$ với $j < i$.

(i) Hàm $r_a$ là nửa liên tục trên.

(ii) Với mọi $x\in M,r_a^0(x) =$ lim inf$_{y\rightarrow x}r_a(y)$.

(iii) Hàm $r_a^0$ là hằng địa phương.

(iv) Tập hợp các điểm $x\in M$ sao cho $r^0_a(x) =r_a(x)$ là tập hợp các điểm của M mà trên một lân cận của chúng $r_a$ là hằng. Đây là một tập con mở trù mật của M. Nếu $k=\mathbf{C}$ và M hữu hạn chiều và liên thông, nó là mở và liên thông.

(i) Nếu $r_a(x) =i$, thì $a_i(x)\not= 0$ và, với mọi $y$ trong một lân cận của $x$, ta có $a_i(y)\not= 0$, do đó $r_a(y)\leq i$.

(ii) Nếu $r^0_a(x) =i$, các hàm $a_0, . . . , a_{i-1}$ là không trên một lân cận của $x$ và, với mọi $y$ trong lân cận này, $r_a(y)\geq i$. Do đó, lim inf$_{y\rightarrow x}r_a(y)\geq i$. Mọi lân cận của $x$ chứa một điểm $y$ sao cho $a_i(y)\not= 0$ và vì vậy $r_a(y)\leq i$. Vậy lim inf$_{y\rightarrow x}r_a(y) =i$.

(iii) Đặt $i=r_a^0(x)$ và gọi V là một lân cận của $x$ sao cho $a_j(y) = 0$ với mọi $y\in V$ và mọi $j < i$. Khi đó $x\in M$**--** Z, trong đó Z ký hiệu tập hợp các điểm của M mà trên một lân cận của chúng hàm $a_i$ là không. Vì Z là đóng trong M (Differentiable and Analytic Manifolds, Results$, 5.3.5$)$, V\cap (M$ **--** Z) là một lân cận của $x$. Với mọi điểm $y$ trong lân cận này, $r_a^0(y) =i$.

(iv) Hàm $r_a-r_a^0$ là nửa liên tục trên và giá trị của nó tại mọi điểm là $\geq 0$. Nếu $r_a(x) =r^0_a(x),r_a-r^0_a$ bằng không trên một lân cận của $x$, điều này cho thấy rằng $r_a$ là hằng trên một lân cận của $x$ theo (iii). Ngược lại, nếu $r_a$ là hằng trên một lân cận của $x$, thì $r_a^0(x) =r_a(x)$ theo (ii). Tập hợp các điểm $x\in M$ sao cho $r_a^0(x) =r_a(x)$ do đó là một tập con mở $\Omega$ của M. Nếu $x\in M$ và nếu $r^0_a(x)< r_a(x)$, mọi lân cận của $x$ chứa một điểm $y$ sao cho $r_a(y)< r_a(x)$ và $r^0_a(y) =r_a^0(x)$. Mọi lân cận của $x$ do đó chứa một điểm $y$ sao cho

$$
r_a(y)-r^0_a(y)< r_a(x)-r^0_a(x)
$$

Suy ra rằng $\Omega$ là trù mật trong M.

Nếu M liên thông và nếu $p$ là giá trị của $r_a^0$ trên M, các điểm của $\Omega$ là các điểm $x\in M$ sao cho $a_p(x)\not= 0$. Nếu $k=\mathbf{C}$, điều này suy ra rằng $\Omega$ liên thông theo Bổ đề 3 của Phụ lục II.

Cho $\rho$ là một biểu diễn tuyến tính giải tích của G trên một không gian vectơ V có số chiều hữu hạn $n$ trên $k$. Đặt

det(T $-\rho (g) + 1$) $=a_0(g) +a_1(g)T +\cdots +a_{n-1}(g)T^{n-1}+ T^n$.

Các hàm $r_a$ và $r_a^0$ liên kết với dãy $(a_0, a_1, . . . , a_{n-1},1)$ sẽ được ký hiệu lần lượt bởi $r_{\rho}$ và $r^0_{\rho}$. Khi đó, với mọi $g\in G$,

$r_{\rho}(g) =$ dim $V^1(\rho (g))$

$r_{\rho}^0(g) =$ lim inf$_{g'\rightarrow g}$ dim $V^1(\rho (g'))$.

#### Bổ đề 2 {#lie-vii-s4-lem-2 .statement tag=00VV}

Cho $0\rightarrow V'\rightarrow V\rightarrow V''\rightarrow 0$ là một dãy khớp của các G-môđun được xác định bởi các biểu diễn tuyến tính giải tích $\rho ', \rho , \rho ''$ của G, tương ứng. Khi đó:

$r_{\rho}=r_{\rho'}+r_{\rho''}$, và $r^0_{\rho}=r^0_{\rho'}+r^0_{\rho''}$.

Thật vậy, với mọi $g\in G$, có (§1, no. 1, Hệ quả 3 của Định lý 1 ) một dãy khớp

$$
0\rightarrow (V')^1(\rho '(g))\rightarrow V^1(\rho (g))\rightarrow (V'')^1(\rho ''(g))\rightarrow 0
$$

chứng minh mệnh đề đầu tiên. Mệnh đề thứ hai suy ra từ đó vì, theo Bổ đề 1 (iv), $r^0_{\rho}=r_{\rho}, r^0_{\rho'}=r_{\rho'}$ và $r_{\rho''}^0=r_{\rho''}$ trên một tập con mở trù mật của G.

#### Định nghĩa 1 {#lie-vii-s4-def-1 .statement tag=00VW}

Một phần tử $g\in G$ được gọi là chính quy đối với biểu diễn tuyến tính $\rho$ nếu $r_{\rho}(g) =r^0_{\rho}(g)$.

#### Mệnh đề 1 {#lie-vii-s4-prop-1 .statement tag=00VX}

Các điểm chính quy đối với một biểu diễn tuyến tính giải tích $\rho$ của G là các điểm của G mà trên một lân cận của chúng $r_{\rho}$ là hằng. Chúng tạo thành một tập con mở trù mật của G. Nếu $k=\mathbf{C}$ và G liên thông, tập hợp các điểm chính quy đối với $\rho$ là liên thông.

Điều này suy ra từ Bổ đề 1 (iv).

#### Nhận xét {#lie-vii-s4-n1-rem-1 .statement tag=00VY}

Cho $G^*$ là một nhóm con mở của G. Một phần tử $a\in G^*$ là một phần tử chính quy của G đối với biểu diễn tuyến tính $\rho$ của G khi và chỉ khi nó là một phần tử chính quy của $G^*$ đối với biểu diễn tuyến tính $\rho |G^*$.

### 2. CÁC PHẦN TỬ CHÍNH QUY CỦA MỘT NHÓM LIE

#### Định nghĩa 2 {#lie-vii-s4-def-2 .statement tag=00VZ}

Một phần tử của G được gọi là chính quy nếu nó chính quy đối với biểu diễn phụ hợp của G.

Nói cách khác (Mệnh đề 1), một phần tử $g\in G$ là chính quy nếu, với mọi phần tử $g'$ trong một lân cận của $g$ trong G, chiều của không gian không của Ad($g'$)$-1$ bằng chiều của không gian không của Ad($g$)$-1$.

#### Mệnh đề 2 {#lie-vii-s4-prop-2 .statement tag=00W0}

Cho $G'$ là một nhóm Lie hữu hạn chiều trên $k$ và $f$ là một cấu xạ mở từ G vào $G'$. Ảnh qua $f$ của một phần tử chính quy của G là một phần tử chính quy của $G'$. Nếu hạt nhân của $f$ được chứa trong tâm của G, một phần tử $g\in G$ là chính quy khi và chỉ khi $f(g)$ là chính quy.

Thật vậy, gọi $\mathfrak{g}'$ là đại số Lie của $G'$ và $\mathfrak{h}$ là iđêan trong $\mathfrak{g}$ cho bởi hạt nhân của $Tf|\mathfrak{g}$. Gọi $\rho$ là biểu diễn tuyến tính của G trên $\mathfrak{h}$ được định nghĩa bởi $\rho (g) =$ Ad $g|\mathfrak{h}$ với mọi $g\in G$, và gọi Ad $\circ f$ là biểu diễn tuyến tính của G trên $\mathfrak{g}'$ cho bởi hợp thành của $f$ với biểu diễn phụ hợp của $G'$. Các biểu diễn tuyến tính này xác định một dãy khớp của các G-môđun:

$$
0\rightarrow \mathfrak{h}\rightarrow \mathfrak{g}\rightarrow \mathfrak{g}'\rightarrow 0
$$

Theo Bổ đề $2,r_{Ad}=r_{\rho}+r_{Ad\circ f}$. Vì $r_{Ad\circ f}=r_{Ad}\circ f$ và vì $f$ là một ánh xạ mở, $r_{Ad\circ f}^0=r_{Ad}^0\circ f$. Do đó:

$$
r_{Ad}-r^0_{Ad}=r_{\rho}-r_{\rho}^0+ (r_{Ad}-r_{Ad}^0)\circ f
$$

Vậy, nếu $g$ là chính quy, $(r_{Ad}-r^0_{Ad})(f(g)) = 0$, điều này có nghĩa là $f(g)$ là chính quy. Nếu hạt nhân của $f$ được chứa trong tâm của G,

$r_{\rho}(g) =r_{\rho}^0(g) =$ dim$\mathfrak{h}$ với mọi $g\in G$. Do đó, nếu $f(g)$ là chính quy, $r_{Ad}(g) =r_{Ad}^0(g)$, nói cách khác, $g$ là chính quy.

#### Mệnh đề 3 {#lie-vii-s4-prop-3 .statement tag=00W1}

Cho $G_1$ và $G_2$ là hai nhóm Lie hữu hạn chiều trên $k$. Một phần tử $(g_1, g_2)$ của $G_1\times G_2$ là chính quy khi và chỉ khi $g_1$ và $g_2$ lần lượt là các phần tử chính quy của $G_1$ và $G_2$.

Điều kiện này là cần thiết theo Mệnh đề 2. Ta chứng minh rằng nó là đủ. Với mọi $g= (g_1, g_2)\in G_1\times G_2,r_{Ad}(g) =r_{Ad}(g_1) +r_{Ad}(g_2)$. Theo Bổ đề 1 (ii), suy ra rằng $r^0_{Ad}(g) =r^0_{Ad}(g_1) +r_{Ad}^0(g_2)$. Nếu $g_1$ và $g_2$ là chính quy, thì $r^0_{Ad}(g_1) =$ $r_{Ad}(g_1)$ và $r^0_{Ad}(g_2) =r_{Ad}(g_2)$, do đó $r^0_{Ad}(g) =r_{Ad}(g)$, điều này có nghĩa là $g$ là chính quy.

#### Bổ đề 3 {#lie-vii-s4-lem-3 .statement tag=00W2}

Cho $a\in G$ và cho $\mathfrak{m}$ là một phần bù của $\mathfrak{g}^1(a)$ trong $\mathfrak{g}$. Cho U là một lân cận của 0 trong $\mathfrak{g}$ và exp là một ánh xạ mũ từ U vào G. Ánh xạ

$f: (x, y) \rightarrow$ (exp $y$)$a$(exp $x$)(exp $y$)$^{-1}$

từ $(\mathfrak{g}^1(a)\times \mathfrak{m})\cap U$ vào G là étale tại $(0,0)$.

Các ánh xạ tuyến tính tiếp xúc tại 0 của các ánh xạ $x \rightarrow a$(exp $x$) và $y \rightarrow$ (exp $y$)$a$(exp $y$)$^{-1}$ là các ánh xạ $x \rightarrow ax$ và $y \rightarrow ya-ay=a(a^{-1}ya-y)$ từ $\mathfrak{g}$ vào $T_aG =a\mathfrak{g}$ (Chap. III, §3, no. 12, Mệnh đề 46). Do đó, ánh xạ tiếp xúc của $f$ tại $(0,0)$ là ánh xạ $(x, y) \rightarrow ax+a(a^{-1}ya-y) =a(x+a^{-1}ya-y)$ từ $\mathfrak{g}^1(a)\times \mathfrak{m}$ vào $a\mathfrak{g}$. Ánh xạ này là đơn ánh. Thật vậy, nếu $x\in \mathfrak{g}^1(a), y\in \mathfrak{m}$ và nếu $x+a^{-1}ya-y$ = 0, thì (Ad($a$)$-1$)$y$ = Ad($a$)$x\in \mathfrak{g}^1(a)$ vì Ad($a$)$\mathfrak{g}^1(a)\subset \mathfrak{g}^1(a)$. Điều này kéo theo rằng $y\in \mathfrak{g}^1(a)$ và do đó $y$ = 0. Vì Ad($a$) đơn ánh trên $\mathfrak{g}^1(a)$, suy ra rằng $x$ = 0. Vì dim $\mathfrak{g}=$ dim$\mathfrak{g}^1(a) +$ dim $\mathfrak{m}$, điều này chứng minh rằng $f$ là étale tại $(0,0)$.

#### Mệnh đề 4 {#lie-vii-s4-prop-4 .statement tag=00W3}

Cho $a\in G$ và H là một mầm nhóm con Lie của G với đại số Lie $\mathfrak{g}^1(a)$. Ánh xạ $(b, c) \rightarrow cabc^{-1}$ từ $H\times G$ vào G là một ánh xạ toàn phân tại $(e, e)$.

Thật vậy, gọi $\mathfrak{m}$ là một phần bù của $\mathfrak{g}^1(a)$ trong $\mathfrak{g}$ và exp là một ánh xạ mũ của G được xác định trên một lân cận mở U của 0 trong $\mathfrak{g}$. Ta có thể chọn U sao cho exp(U $\cap \mathfrak{g}^1(a)$)$\subset H$. Ánh xạ $f: (x, y) \rightarrow$ (exp $x$, exp $y$) là một ánh xạ giải tích trên một lân cận của $(0,0)$ trong $\mathfrak{g}^1(a)\times \mathfrak{m}$ với giá trị trong $H\times G$. Theo Bổ đề 3, ánh xạ hợp của $f$ với ánh xạ $\varphi : (b, c) \rightarrow cabc^{-1}$ là étale tại $(0,0)$. Suy ra rằng $\varphi$ là một ánh xạ toàn phân tại $f(0,0) = (e, e)$.

#### Mệnh đề 5 {#lie-vii-s4-prop-5 .statement tag=00W4}

Cho $a\in G$ và cho W là một lân cận của $e$ trong G. Tồn tại một lân cận V của $a$ có tính chất sau: với mọi $a'\in V$, tồn tại một phần tử $g\in W$ sao cho $\mathfrak{g}^1(a')\subset$ Ad($g$)$\mathfrak{g}^1(a)$.

Đặt $\mathfrak{g}^1=\mathfrak{g}^1(a)$ và cho $\mathfrak{g}=\mathfrak{g}^1+\mathfrak{g}^+$ là phân rã Fitting của Ad($a$)$-1 ($§1, no. 1). Cho H là một mầm nhóm con Lie của G với đại số Lie $\mathfrak{g}^1$. Với mọi $h\in H$, Ad($h$)$\mathfrak{g}^1\subset \mathfrak{g}^1$. Vì $[\mathfrak{g}^1,\mathfrak{g}^+]\subset \mathfrak{g}^+$, tồn tại một lân cận U của $e$ trong H sao cho Ad($h$)$\mathfrak{g}^+\subset \mathfrak{g}^+$ với mọi $h\in H$. Vì hạn chế của Ad($a$)$-1$ lên $\mathfrak{g}^+$ là song ánh, U có thể được chọn sao cho hạn chế của Ad($ah$)$-1$ lên $\mathfrak{g}^+$ là song ánh với mọi $h\in U$. Khi đó $\mathfrak{g}^1(ah)\subset \mathfrak{g}^1(a) =\mathfrak{g}^1$ với mọi $h\in U$. Theo Mệnh đề 4, Int(W)($aU$) là một lân cận của $a$ trong G. Nếu $a'\in$ Int(W)($aU$), thì $a'=g(ah)g^{-1}$ với $g\in W$ và $h\in U$; suy ra rằng $\mathfrak{g}^1(a') =$ Ad($g$)$\mathfrak{g}^1(ah)\subset$ Ad($g$)$\mathfrak{g}^1(a)$.

#### Hệ quả {#lie-vii-s4-n2-cor-1 .statement tag=00W5}

Cho $G^*$ là một nhóm con mở của G. Nếu $a\in G$ là chính quy, tồn tại một lân cận V của $a$ sao cho, với mọi $a'\in V,\mathfrak{g}^1(a')$ là liên hợp với $\mathfrak{g}^1(a)$ dưới Ad(G$^*$).

### 3. QUAN HỆ VỚI CÁC PHẦN TỬ CHÍNH QUY CỦA ĐẠI SỐ LIE

#### Mệnh đề 6 {#lie-vii-s4-prop-6 .statement tag=00W6}

Cho V là một nhóm con mở của $\mathfrak{g}$ và cho exp$: V\rightarrow G$ là một ánh xạ hàm mũ được xác định trên V.

(i) Tồn tại một lân cận W của 0 trong V sao cho $\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^0(x)$ với mọi $x\in W$.

(ii) Nếu $k=\mathbf{R}$ hoặc $\mathbf{C},\mathfrak{g}^1$(exp $x$)$\supset \mathfrak{g}^0(x)$ với mọi $x\in \mathfrak{g}$.

Theo Hệ quả 3 của Mệnh đề 8 của Chương III, §4, no. 4, tồn tại một lân cận $V'$ của 0 trong V sao cho, với mọi $x\in V'$, exp(ad($x$)) $=\sum_{n=0}^{\infty}\frac{1}{n!}$ ad($x$)$^n$ được xác định và Ad(exp $x$) $=$ exp(ad($x$)). Nếu $P\in k[X]$ và $\alpha \in$ End($\mathfrak{g}$), thật dễ kiểm tra rằng $\mathfrak{g}^{\lambda}(\alpha )\subset \mathfrak{g}^{P(\lambda)}(P(\alpha ))$ với mọi $\lambda \in k$. Do đó,

$\mathfrak{g}^0$(ad($x$))$\subset \mathfrak{g}^1$(exp(ad($x$))) $=\mathfrak{g}^1$(Ad(exp $x$)) $=\mathfrak{g}^1$(exp $x$)

với mọi $x\in V'$. Nếu $k=\mathbf{R}$ hoặc $\mathbf{C}, V =\mathfrak{g}$ và ta có thể lấy $V'$ = V, điều này chứng minh (ii). Ta chứng minh (i). Cho U là một lân cận của 0 trong End($\mathfrak{g}$) sao cho Log(1 $+\alpha$ ) $=\sum_{n>0}(-1)^{n+1 1}_{\overline{n}}\alpha^n$ được xác định với mọi $\alpha \in U$. Khi đó Log $\circ$ exp = 1 trên một lân cận của 0 và $\mathfrak{g}^1(1 +\alpha )\subset \mathfrak{g}^0$(Log(1 $+\alpha$ )) với mọi $\alpha \in U$. Gọi W là lân cận của 0 trong $\mathfrak{g}$ gồm các $x\in V'$ sao cho exp ad $x\in 1 + U$ và

Log(exp(ad($x$))) $=$ ad($x$).

Khi đó, với mọi $x\in W$,

$\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^1$(Ad(exp $x$)) $=\mathfrak{g}^1$(exp(ad($x$)))

$\subset \mathfrak{g}^0$(Log(exp(ad($x$)))) $=\mathfrak{g}^0$(ad($x$)) $=\mathfrak{g}^0(x)$.

Điều này chứng tỏ rằng $\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^0(x)$ với mọi $x\in W$.

#### Bổ đề 4 {#lie-vii-s4-lem-4 .statement tag=00W7}

Cho U là một lân cận của 0 trong $\mathfrak{g}$ và exp là một ánh xạ mũ từ U vào G, étale tại mọi điểm của U và sao cho $\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^0(x)$ với mọi $x\in U$.

(i) Hàm $r^0_{Ad}$ là hằng và bằng hạng của $\mathfrak{g}$ trên exp(U).

(ii) Nếu $x\in U$, exp $x$ là chính quy khi và chỉ khi $x$ là một phần tử chính quy của $\mathfrak{g}$.

(iii) Một phần tử $a\in$ exp(U) là chính quy khi và chỉ khi $\mathfrak{g}^1(a)$ là một đại số con Cartan của $\mathfrak{g}$.

Cho $l=$ rk($\mathfrak{g}$). Nếu $x\in U$ là một phần tử chính quy của $\mathfrak{g}$,

$r_{Ad}$(exp $x$) $=$ dim$\mathfrak{g}^1$(exp $x$) $=$ dim$\mathfrak{g}^0(x) =l$.

Vì các phần tử chính quy của $\mathfrak{g}$ thuộc U tạo thành một lân cận của $x$ và exp là étale tại $x$, điều này cho thấy exp $x$ là chính quy và $r^0_{Ad}$(exp $x$) $=l$. Các phần tử chính quy của $\mathfrak{g}$ thuộc U là trù mật trong U, ta có $r^0_{Ad}(a) =$ $l$ với mọi $a\in$ exp(U). Cho $a\in$ exp(U) là một phần tử chính quy của G và cho $x\in U$ sao cho $a=$ exp $x$. Vì $\mathfrak{g}^0(x) =\mathfrak{g}^1(a)$, dim $\mathfrak{g}^0(x) =r^0_{Ad}(a) =l$. Do đó, $x$ là một phần tử chính quy của $\mathfrak{g}$ và $\mathfrak{g}^1(a)$ là một đại số con Cartan của $\mathfrak{g}$. Cuối cùng, nếu $a\in$ exp(U) và $\mathfrak{g}^1(a)$ là một đại số con Cartan của $\mathfrak{g}$,

$r_{Ad}(a) =$ dim$\mathfrak{g}^1(a) =l=r_{Ad}^0(a)$,

thì $a$ là chính quy.

#### Mệnh đề 7 {#lie-vii-s4-prop-7 .statement tag=00W8}

Cho V là một lân cận của $e$ trong G. Mọi đại số con Cartan của $\mathfrak{g}$ đều có dạng $\mathfrak{g}^1(a)$ trong đó $a$ là một phần tử chính quy của G thuộc V.

Theo Mệnh đề 6, tồn tại một lân cận mở U của 0 trong $\mathfrak{g}$ và một ánh xạ mũ exp$: U\rightarrow G$ thỏa mãn các điều kiện của Bổ đề 4. Nếu $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$, tồn tại một phần tử chính quy $x\in \mathfrak{h}$ sao cho $\mathfrak{h}=\mathfrak{g}^0(x) ($§3, Định lý 2). Mặt khác, tồn tại một phần tử $t\in k^*$ sao cho $tx\in U$ và exp($tx$)$\in V$. Khi đó $\mathfrak{h}=\mathfrak{g}^0(x) =\mathfrak{g}^0(tx) =\mathfrak{g}^1$(exp($tx$)), và theo Bổ đề 4 (ii), exp($tx$) là một phần tử chính quy của G.

#### Mệnh đề 8 {#lie-vii-s4-prop-8 .statement tag=00W9}

Cho $l$ là hạng của $\mathfrak{g}$. Tồn tại một nhóm con mở $G^*$ của G sao cho:

(i) hàm $r^0_{Ad}$ là hằng trên $G^*$ và giá trị của nó là $l$;

(ii) một phần tử $a\in G^*$ là chính quy khi và chỉ khi $\mathfrak{g}^1(a)$ là một đại số con Cartan của $\mathfrak{g}$;

(iii) nếu $a\in G^*$, mọi đại số con Cartan của $\mathfrak{g}^1(a)$ là một đại số con Cartan của $\mathfrak{g}$.

(i) Theo Mệnh đề 6, tồn tại một lân cận mở U của 0 trong $\mathfrak{g}$ và một ánh xạ mũ exp từ U vào G thỏa mãn các điều kiện của Bổ đề 4. Trong phần tiếp theo, $G^*$ sẽ kí hiệu thành phần đơn vị của G nếu $k=\mathbf{R}$ hoặc $\mathbf{C}$ và một nhóm con mở của G được chứa trong exp(U) nếu $k$ là siêu mêtric. Vì $r_{Ad}^0$ là hằng địa phương và giá trị của nó tại mọi điểm của exp(U) là $l$ (Bổ đề 4 (i)), suy ra rằng $r_{Ad}^0$ là hằng và bằng $l$ trên $G^*$.

(ii) Gọi $R^*$ (tương ứng $S^*$) là tập hợp các phần tử chính quy của $G^*$ (tương ứng tập hợp các phần tử $a\in G^*$ sao cho $\mathfrak{g}^1(a)$ là một đại số con Cartan của $\mathfrak{g}$). Khi đó $S^*\subset R^*$. Thật vậy, nếu $a\in S^*$, thì $r_{Ad}(a) =l=r^0_{Ad}(a)$. Ta chứng minh rằng $R^*\subset S^*$. Nếu $k$ là siêu trị ultrametric, điều này suy ra từ bao hàm $G^*\subset$ exp(U) và Bổ đề 4 (iii). Giả sử rằng $k=\mathbf{C}$. Theo Hệ quả của Mệnh đề 5, nếu $a\in R^*$, thì với mọi $a'$ thuộc một lân cận của $a,\mathfrak{g}^1(a')$ liên hợp với $\mathfrak{g}^1(a)$ bởi một tự đẳng cấu của $\mathfrak{g}$. Điều này chứng minh rằng $S^*$ và $R^*$ **--** $S^*$ là các tập con mở của $G^*$. Ta đã thấy rằng $S^*$ chứa tất cả các phần tử chính quy trong một lân cận của $e$ (Bổ đề 4 (iii)); do đó, $S^*$ là khác rỗng. Vì $G^*$ liên thông, nên $R^*$ cũng vậy (Mệnh đề 1) và do đó $S^*= R^*$.

Còn lại là nghiên cứu trường hợp $k=\mathbf{R}$. Trước hết giả sử rằng $G^*$ là một nhóm con nguyên của $\mathbf{G}\mathbf{L}(E)$ trong đó E là một không gian vectơ thực hữu hạn chiều. Gọi $G^*_c$ là nhóm con nguyên của $\mathbf{G}\mathbf{L}(E\otimes_{\mathbf{R}}\mathbf{C})$ có đại số Lie $\mathfrak{g}_c=\mathfrak{g}\otimes \mathbf{C}$. Tồn tại một hàm giải tích trên $G^*_c$ mà tập hợp các điểm không của nó là phần bù của tập mở các phần tử chính quy của $G^*_c$. Theo Các đa tạp khả vi và giải tích, Kết quả, 3.2.5, hàm này không thể triệt tiêu tại mọi điểm của $G^*$. Do đó, $G^*$ chứa một phần tử chính quy của $G^*_c$. Gọi Ad$_c$ là biểu diễn phụ hợp của $G^*_c$. Với mọi $a\in G^*,\mathfrak{g}^1_c(a) =\mathfrak{g}^1(a)\otimes \mathbf{C}$, do đó $r_{Ad_c}(a) =r_{Ad}(a)$. Nếu $a\in G^*$ là một phần tử chính quy của $G^*_c$, thì đây là một phần tử chính quy của $G^*$ và $r_{Ad}^0(a) =r_{Ad}^0(a)$. Các hàm $r^0_{Ad}$ và $r_{Ad}^0$ lần lượt là hằng trên $G^*_c$ và trên $G^{^c*}$, suy ra rằng các phần tử chính quy$^{^c}$ của $G^*$ là các phần tử chính quy của $G^*_c$ thuộc $G^*$. Từ điều trên, nếu $a$ là một phần tử chính quy của $G^*,\mathfrak{g}^1_c(a) =\mathfrak{g}^1(a)\otimes \mathbf{C}$ là một đại số con Cartan của $\mathfrak{g}_c$; điều này kéo theo rằng $\mathfrak{g}^1(a)$ là một đại số con Cartan của $\mathfrak{g}($§2, Mệnh đề 3).

Giả sử bây giờ rằng G liên thông đơn. Tồn tại một không gian vectơ thực hữu hạn chiều E và một cấu xạ étale $f$ từ G đến một nhóm con nguyên $G'$ của $\mathbf{G}\mathbf{L}(E)$ (Chương III, §6, no. 1, Hệ quả của Định lý 1). Theo Mệnh đề 2, nếu $a\in G$ là phần tử chính quy, thì $f(a)$ là chính quy. Theo phần trước, ${\mathfrak{g}'}^1(f(a))$ là một đại số con Cartan của đại số Lie $\mathfrak{g}'$ của G'. Vì ${\mathfrak{g}'}^1(f(a)) = (Tf)\mathfrak{g}^1(a)$ và $Tf$ là một đẳng cấu từ $\mathfrak{g}$ đến $\mathfrak{g}'$, điều này chứng tỏ rằng $\mathfrak{g}^1(a)$ là một đại số con Cartan của $\mathfrak{g}$.

Ta xét cuối cùng trường hợp tổng quát $(k=\mathbf{R})$. Cho $\widetilde{G}$ là một phủ phổ quát của $G^*, \widetilde{\mathfrak{g}}= L( \widetilde{G})$, và $q$ là ánh xạ chính tắc từ $\widetilde{G}$ đến $G^*$. Vì hạt nhân của $q$ được chứa trong tâm của $\widetilde{G}$, nếu $a\in G^*$ là chính quy và nếu $a'\in q^{-1}(a)$, thì $a'$ là chính quy (Mệnh đề 2). Theo phần trước, $\widetilde{\mathfrak{g}}^1(a')$ là một đại số con Cartan của $\widetilde{\mathfrak{g}}$. Vì $\mathfrak{g}^1(a) = (Tq)\widetilde{\mathfrak{g}}^1(a')$ và vì $Tq$ là một đẳng cấu từ $\widetilde{\mathfrak{g}}$ đến $\mathfrak{g}$, điều này chứng tỏ rằng $\mathfrak{g}^1(a)$ là một đại số con Cartan của $\mathfrak{g}$.

(iii) Theo Mệnh đề 5, tồn tại một lân cận V của $a$ sao cho, với mọi $a'\in V,\mathfrak{g}^1(a')$ được liên hợp với một đại số con của $\mathfrak{g}^1(a)$ bởi một tự đẳng cấu của $\mathfrak{g}$. Vì mọi lân cận của $a$ đều chứa một phần tử chính quy của $G^*$, suy ra từ (ii) rằng $\mathfrak{g}^1(a)$ chứa một đại số con Cartan của $\mathfrak{g}$. Do đó, theo Mệnh đề 3 của §3, mọi đại số con Cartan của $\mathfrak{g}^1(a)$ đều là một đại số con Cartan của $\mathfrak{g}$.

#### Nhận xét {#lie-vii-s4-n3-rem-1 .statement tag=00WA}

Nếu $k=\mathbf{C}$, các đại số con $\mathfrak{g}^1(a)$, với $a$ chính quy và thuộc một thành phần liên thông M của G, là liên hợp dưới Int($\mathfrak{g}$). Thật vậy, xét R là tập hợp các phần tử chính quy của G. Với mọi $a\in R\cap M$, đặt $M_a$ là tập hợp các $b\in R\cap M$ sao cho $\mathfrak{g}^1(a)$ là liên hợp với $\mathfrak{g}^1(a)$ dưới Int($\mathfrak{g}$). Ta có Int($\mathfrak{g}$) $=$ Ad(G$^0$), trong đó $G^0$ là thành phần liên thông đơn vị của G. Theo Hệ quả của Mệnh đề $5$, $M_a$ mở trong R. Suy ra $M_a$ vừa mở vừa đóng trong R. Vì $k=\mathbf{C}, R\cap M$ liên thông (Bổ đề 1), nên $M_a= R\cap M$.

### 4. ỨNG DỤNG CHO CÁC TỰ ĐẲNG CẤU SƠ CẤP

#### Mệnh đề 9 {#lie-vii-s4-prop-9 .statement tag=00WB}

Cho $k$ là một trường có đặc số 0 và $\mathfrak{g}$ là một đại số Lie trên $k$. Nếu $a\in$ Aut$_e(\mathfrak{g})$, thì chiều của không gian nghiệm của $a-1$ lớn hơn hoặc bằng hạng của $\mathfrak{g}$.

Theo “nguyên lý Lefschetz” (Đại số, Ch. V, §14, mục 6, Hệ quả 2 của Định lý $5$)$,k$ là một hợp có hướng tăng dần của các trường con $(k_i)_{i\in I}$ vốn nhận $\mathbf{C}$ làm trường mở rộng. Cho $(e_{\alpha})$ là một cơ sở của $\mathfrak{g}$ trên $k$ và $x_1, . . . , x_m$ là các phần tử của $\mathfrak{g}$ sao cho ad($x_1$)$, . . .$, ad($x_m$) là lũy linh và $a=e^{ad(x_1)}. . . e^{ad(x_m)}$. Kí hiệu $c^{\gamma}_{\alpha \beta}$ là các hằng số cấu trúc của $\mathfrak{g}$ đối với cơ sở $(e_{\alpha})$ và $(x^{\alpha}_r)$ là các thành phần của $x_r$ đối với cơ sở này $(1\leq r\leq m)$. Tồn tại một chỉ số $j\in I$ sao cho các $c^{\gamma}_{\alpha \beta}$ và các $x^{\alpha}_r$ đều thuộc $k_j$. Đặt $\mathfrak{g}_j=\sum_{\alpha}k_je_{\alpha}$;

đây là một đại số Lie trên $k_j$ chứa $x_1, . . . , x_m$, và sự hạn chế $a_j$ của $a$ lên $\mathfrak{g}_j$ là một tự đẳng cấu sơ cấp của $\mathfrak{g}_j$. Sự mở rộng của $a_j$ lên $\mathfrak{g}_j\otimes_{k_j}\mathbf{C}$ là một tự đẳng cấu sơ cấp $a_j\otimes 1$ của $\mathfrak{g}_j\otimes \mathbf{C}$. Vậy hãy lấy $G_j$ là một nhóm Lie phức liên thông với đại số Lie $\mathfrak{g}_j\otimes \mathbf{C}$, và $s$ là một phần tử của $G_j$ sao cho Ad($s$) $=a_j\otimes 1$. Mệnh đề 8, áp dụng cho cặp $(G_j, s)$, cho thấy nilspace của $a_j\otimes 1-1$ có chiều $n$, nên

$n\geq$ rk($\mathfrak{g}_j\otimes \mathbf{C}$) $=$ rk($\mathfrak{g}_j$) $=$ rk($\mathfrak{g}$).

Nhưng không gian này có cùng chiều với không gian của $a_j-1$ và của $a-1$. Do đó mệnh đề.

### Bài tập {#lie-vii-s4-exercises}

Các ký hiệu và giả thiết là của các số 1, 2, 3 của §4.

Xem [các bài tập cho § 4](exercises/s4/).
