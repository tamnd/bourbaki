---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 5
section_title: Opérateurs partiels normaux et théorème spectral
lang: vi
source: ts-iii-v-fr
book_pages: TS IV.262-TS IV.311, TS IV.352-TS IV.372
pdf_pages: 0275-0324, 0365-0385
extraction: native
subsections:
    - "no": 1
      title: Bornification
      page: 262
      pdf_page: 275
    - "no": 2
      title: Opérateurs partiels normaux et théorème spectral
      page: 265
      pdf_page: 278
    - "no": 3
      title: Calcul fonctionnel universellement mesurable
      page: 270
      pdf_page: 283
    - "no": 4
      title: Projecteurs spectraux
      page: 277
      pdf_page: 290
    - "no": 5
      title: La formule de Helffer–Sjöstrand
      page: 280
      pdf_page: 293
    - "no": 6
      title: Topologies résolvantes et continuité du calcul fonctionnel
      page: 285
      pdf_page: 298
    - "no": 7
      title: Décomposition polaire
      page: 289
      pdf_page: 302
    - "no": 8
      title: Opérateurs auto-adjoints définis par une forme hermitienne partielle positive
      page: 291
      pdf_page: 304
    - "no": 9
      title: Principes variationnels pour le spectre des opérateurs positifs
      page: 296
      pdf_page: 309
    - "no": 10
      title: Perturbation compacte et spectre essentiel
      page: 303
      pdf_page: 316
    - "no": 11
      title: Perturbation
      page: 305
      pdf_page: 318
    - "no": 12
      title: Opérateurs à résolvante compacte
      page: 307
      pdf_page: 320
statements: 75
exercises: 43
content_sha256: 51cc14d7691eab7d64b842f957a075e8a25d72b99d74140175edf323535e174b
translated_from: content/en-mt/ts/IV/05_s5_operateurs_partiels_normaux_et_theoreme.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 10dc37b619e64ee4a121601fe906832b609fb0f17e1d46252b2e1db1c97c4fb6
translation_model: gpt-5.4, gpt-5-6, gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-42beec17
glossary_version: 34
glossary_terms_sha256: 8cbf6a39a92640f3043005ec6da9392c7e16127bd3253af23951957ec0bf11ff
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. TOÁN TỬ BỘ PHẬN CHUẨN VÀ ĐỊNH LÝ PHỔ

### 1. Bị chặn hóa

Cho E là một không gian Hilbert phức. Gọi $s$ là ánh xạ unita $(x, y)\mapsto (-y, x)$ trên $E\oplus E$. Cho $u$ là một toán tử bộ phận đóng với miền xác định trù mật trên E. Toán tử bộ phận $u^*u$ là tự liên hợp và dương (Mệnh đề 12 của IV, p. 241), do đó $-1\notin$ Sp($u^*u$) (Mệnh đề 17 của IV, p. 248). Đặt $W(u) = (1_E+u^*u)^{-1}=-R(u^*u,-1)$; đó là một tự đồng cấu dương và đơn ánh của E.

Gọi $p_1$ và $p_2$ là hai phép chiếu chính tắc của $\Gamma_u$ vào E. Chúng là các phần tử của $\mathscr{L}(\Gamma_u; E)$, và ta có đẳng thức các tương ứng $p_2=u\circ p_1$. Gọi $(j,|p^*_1|)$ là phân tích cực (Định nghĩa 4 của I, p. 140) của tự đồng cấu $p^*_1\in \mathscr{L}(E; \Gamma_u)$, sao cho $p^*_1=|p^*_1| \circ j$. Ánh xạ $j$ là một đẳng cự bộ phận từ E vào $\Gamma_u$.

#### Định nghĩa 1 {#ts-iv-s5-def-1 .statement tag=0359}

Tự đồng cấu $p_2\circ j$ của E được gọi là bị chặn hóa của $u$; ta ký hiệu tự đồng cấu này là $b(u)$.

Ta có $\|b(u)\|\leqslant 1$.

#### Mệnh đề 1 {#ts-iv-s5-prop-1 .statement tag=035A}

Ta có các công thức

$$
|p^*_1|= W(u)^{1/2} \tag{1}
$$

$$
b(u) =u\circ W(u)^{1/2}=u\circ  |p^*_1| \tag{2}
$$

$$
1_E-b(u)^*b(u) = W(u) \tag{3}
$$

$$
b(u)W(u) = W(u^*)b(u),b(u)W(u)^{1/2}= W(u^*)^{1/2}b(u) \tag{4}
$$

Cho $x\in E$. Đặt $y= W(u)(x)\in$ dom($u^*u$). Ta có $y\in$ dom($u$) và $u(y)\in$ dom($u^*$). Với mọi phần tử $(y_1, u(y_1))$ của $\Gamma_u$, trong đó $y_1\in$ dom($u$), ta tính được

$$
\langle (y, u(y))|(y_1, u(y_1))\rangle =\langle y|y_1\rangle +\langle u(y)|u(y_1)\rangle
$$

$$
=\langle y+u^*u(y)|y_1\rangle =\langle x|p_1(y_1, u(y_1))\rangle
$$

Điều đó có nghĩa là $p^*_1(x) = (y, u(y))$, do đó $p_1\circ p^*_1(x) =y= W(u)(x)$. Vì thế, ta có $p_1\circ p^*_1= W(u)$, suy ra $|p^*_1|= W(u)^{1/2}$, tức là công thức (1). Đặc biệt, vì Im($p_1$) $=$ Im($|p^*_1|$) theo Hệ quả của Mệnh đề 11 của I, p. 140, suy ra dom($u$) $=$ Im($p_1$) $=$ Im(W($u$)$^{1/2}$). Vậy toán tử bộ phận $u\circ W(u)^{1/2}$ có miền xác định là toàn bộ không gian E. Khi đó quan hệ $p_1\circ j= (p^*_1)^*\circ j=|p^*_1|= W(u)^{1/2}$ (Mệnh đề 11, a) của I, p. 140) kéo theo rằng

$$
b(u) =p_2\circ j=u\circ p_1\circ j=u\circ W(u)^{1/2}
$$

đó là công thức (2).

Ta có Ker($j$) $=$ Ker($|p^*_1|$) (mệnh đề 10, b) của I, p. 139) và do đó công thức (1) suy ra rằng đẳng cự bộ phận $j: E\rightarrow \Gamma_u$ là đơn ánh, nên đẳng cự, do đó $j^*\circ j= 1_E$. Viết $j= (p_1\circ j, b(u))$, ta được

$$
1_E=j^*\circ j= (p_1\circ j)^*(p_1\circ j) +b(u)^*b(u) = W(u) +b(u)^*b(u)
$$

do đó có công thức (3).

Lấy $x\in$ dom($u$) và đặt $y= W(u)(x)$. Ta có $y\in$ dom($u$) và công thức $y+u^*u(y) =x$ suy ra rằng $u^*u(y)\in$ dom($u$). Khi đó ta có

$$
W(u^*)^{-1}(u(y)) = (1_E+uu^*)(u(y))
$$

$$
=u(y) +uu^*u(y) =u(y+u^*u(y)) =u(x)
$$

điều này có nghĩa là phép hạn chế của $u\circ W(u)$ lên miền xác định của $u$ bằng $W(u^*)\circ u$. Vì ảnh của $|p^*_1|$ bằng ảnh của $p_1$ (hệ quả của mệnh đề 11 của I, p. 140) và do đó bằng miền xác định của $u$, suy ra rằng

$$
u\circ W(u)\circ  |p^*_1|= W(u^*)\circ u\circ  |p^*_1|= W(u^*)\circ b(u)
$$

(công thức (2)). Hơn nữa, $|p^*_1|= W(u)^{1/2}$ giao hoán với $W(u)$, nên ta được

$$
b(u)\circ W(u) =u\circ  |p^*_1| \circ W(u) =u\circ W(u)\circ  |p^*_1|= W(u^*)\circ b(u)
$$

Quan hệ này suy ra rằng $b(u)\circ f(W(u)) =f(W(u^*))\circ b(u)$ đối với mọi hàm $f\in \mathscr{C}(\mathbf{R}_+)$ (mệnh đề 11 của I, p. 113), nên đặc biệt $b(u)\circ W(u)^{1/2}= W(u^*)^{1/2}\circ b(u)$. Điều này chứng minh công thức (4) và kết thúc chứng minh.

#### Hệ quả {#ts-iv-s5-n1-cor-1 .statement tag=035B}

Ta có $b(u)^*=b(u^*)$.

Gọi $q_1$ và $q_2$ là các phép chiếu $\Gamma_{u^*}\rightarrow E$ và gọi $(k,|q_1^*|)$ là phân tích cực của $q_1^*$, sao cho $b(u^*) =q_2\circ k$. Với mọi $x$ và $y$ thuộc E, ta có $j(x)\in \Gamma_u$ và $k(y)\in \Gamma_{u^*}$, và vì $\Gamma_u$ trực giao với $s(\Gamma_{u^*})$ theo mệnh đề 7 của IV, p. 236, suy ra rằng

$$
0 =\langle j(x)|s(k(y))\rangle =\langle p_1\circ j(x)| -q_2\circ k(y)\rangle +\langle p_2\circ j(x)|q_1\circ k(y)\rangle
$$

Vì $p_1\circ j=|p^*_1|$ và $q_1\circ k=|q^*_1|$ (mệnh đề 11, b) của I, p. 140) nên ta được

$$
\langle b(u)x| |q^*_1|y\rangle =\langle |p^*_1|x|b(u^*)y\rangle
$$

do đó $|q^*_1|b(u) =b(u^*)^*|p^*_1|$. Dùng các công thức (1) và (4), ta kết luận rằng $b(u)|p^*_1|=|q^*_1|b(u) =b(u^*)^*|p^*_1|$, và vì ảnh của $|p^*_1|$ là miền xác định của $u$, trù mật trong E, ta suy ra $b(u) =b(u^*)^*$.

Ta ký hiệu bởi Ω(E) tập hợp các $v\in \mathscr{L}(E)$ sao cho $1_E-v^*v$ là dương và đơn ánh. Với $v\in \Omega (E)$, tự đồng cấu Hermit $(1_E-v^*v)^{1/2}$ là đơn ánh, vì bình phương của nó có tính chất đó, và ta ký hiệu bởi $B(v)$ toán tử bộ phận $v\circ ((1_E-v^*v)^{1/2})^{-1}$.

Chú ý rằng $1_E-v^*v$ là dương khi và chỉ khi $\|v\|\leqslant 1$, vì ta có $\langle x|(1_E-v^*v)(x)\rangle =\|x\|^2- \|v(x)\|^2$ với mọi $x\in E$.

#### Bổ đề 1 {#ts-iv-s5-lem-1 .statement tag=035C}

Tập con Ω(E) là tự liên hợp trong $\mathscr{L}(E)$.

Cho $v\in \Omega (E)$. Ta có $\|v^*\|=\|v\|\leqslant 1$ nên tự đồng cấu $1_E-vv^*$ là dương. Nó là đơn ánh: nếu $x\in$ Ker(1$_E-vv^*$), ta có $vv^*(x) =x$, do đó $v^*(v(v^*(x))) =v^*(x)$ rồi $v^*(x) = 0$, vì $1_E-v^*v$ là đơn ánh, và cuối cùng $x=v(v^*(x)) = 0$. Bổ đề được chứng minh.

#### Mệnh đề 2 {#ts-iv-s5-prop-2 .statement tag=035D}

Ánh xạ $u\mapsto b(u)$ xác định một song ánh từ tập hợp các toán tử bộ phận đóng có miền xác định trù mật trên E lên tập Ω(E). Song ánh ngược được cho bởi $v\mapsto B(v)$.

Quan hệ $1_E-b(u)^*b(u) = W(u)$ (công thức (3)) suy ra $b(u)$ thuộc Ω(E) vì $W(u)$ là dương và đơn ánh. Hơn nữa, vì $b(u) =u\circ W(u)^{1/2}$ (công thức (2)), ta được

$$
u=b(u)\circ (W(u)^{1/2})^{-1}=b(u)\circ ((1-b(u)^*b(u))^{1/2})^{-1}= B(b(u))
$$

Ngược lại, cho $v\in \Omega (E)$. Đặt $w= (1_E-v^*v)^{1/2}$ và $u= B(v) =v\circ w^{-1}$. Miền xác định của $u$ là ảnh của $w$, miền này trù mật trong E vì $w$ là Hermit và đơn ánh (EVT, V, p. 41, mệnh đề 4 (i)). Với mọi $x\in$ dom($u$), ta có

$$
\|u(x)\|^2=\langle (v^*v)(w^{-1}(x))|w^{-1}(x)\rangle
$$

$$
=-\langle (1_E-v^*v)(w^{-1}(x))|w^{-1}(x)\rangle +\|w^{-1}(x)\|^2
$$

$$
=-\langle w(x)|w^{-1}(x)\rangle +\|w^{-1}(x)\|^2
$$

vì $(1_E-v^*v)\circ w^{-1}$ là hạn chế của $w$ lên miền xác định của $w^{-1}$. Vì $w$ là tự liên hợp, ta suy ra rằng

$$
\|w^{-1}(x)\|^2=\|x\|^2+\|v\circ w^{-1}(x)\|^2=\|x\|^2+\|u(x)\|^2
$$

và do đó toán tử bộ phận $B(v) =u=v\circ w^{-1}$ là đóng theo Bổ đề 2 của IV, p. 231.

Sau cùng, ta hãy chứng minh rằng $b(B(v)) =v$. Vì $u=v\circ w^{-1}$, ta có $v=u\circ w$, và do đó chỉ cần kiểm tra rằng $w= W(u)^{1/2}$ (công thức (2)), hoặc thậm chí rằng $1_E-v^*v= W(u)$.

Tự đồng cấu $v^*$ thuộc Ω(E) theo Bổ đề 1. Đặt $w'= (1_E-vv^*)^{1/2}$. Đó là một tự đồng cấu dương đơn ánh của E, và ta có $v\circ w=w'\circ v$ (mệnh đề 11 của I, p. 113). Đồ thị của $u$ là tập hợp các phần tử có dạng $(w(x), v(x))$ với $x\in E$. Theo mệnh đề 7 của IV, p. 236, đồ thị của $u^*$ là $s(\Gamma_u)^{\circ}$. Vì, với mọi $x$ và $y\in E$, ta có

$$
\langle (w'(x), v^*(x))|(-v(y), w(y))\rangle =-\langle x|w'v(y)\rangle +\langle x|vw(y)\rangle = 0
$$

đồ thị của $u^*$ chứa các phần tử dạng $(w'(x), v^*(x))$ với $x\in E$, và khi đó ta có $u^*(w'(x)) =v^*(x)$. Đặc biệt, miền xác định của $u^*$ chứa ảnh của $w'$.

Cho $x\in E$ và đặt $y=w^2(x) = (1_E-v^*v)(x)$, để rồi $x=y+v^*v(x)$. Ta có $y\in$ dom($u$) và $u(y) =v(w^{-1}(y)) =v(w(x)) =w'(v(x))$. Đặc biệt, $u(y)\in$ Im($w$)$\subset$ dom($u^*$), và $u^*(u(y)) =v^*(v(x))$. Do đó suy ra $x=y+v^*v(x) =y+u^*u(y)$, nên $y= W(u)(x)$, nghĩa là

$$
(1_E-v^*v)(x) = W(u)(x)
$$

Vậy đã chứng minh được rằng $1_E-v^*v= W(u)$, như mong muốn.

#### Hệ quả {#ts-iv-s5-n1-cor-2 .statement tag=035E}

Tự đồng cấu $b(u)$ là Hermit nếu và chỉ nếu $u$ là tự liên hợp.

Điều này suy ra từ tính đơn ánh của ánh xạ $u\mapsto b(u)$ (mệnh đề 2) và từ công thức $b(u^*) =b(u)^*$ (hệ quả của mệnh đề 1).

### 2. Toán tử bộ phận chuẩn tắc và định lý phổ

Trong số này, E là một không gian Hilbert phức.

#### Định nghĩa 2 {#ts-iv-s5-def-2 .statement tag=035F}

Cho $u$ là một toán tử bộ phận trên E. Ta nói rằng $u$ là chuẩn tắc nếu $u$ đóng với miền xác định trù mật và nếu bornification của nó $b(u)$ là một tự đồng cấu chuẩn tắc của E.

Nếu $u\in \mathscr{L}$ (E), định nghĩa này phù hợp với EVT, V, p. 42, định nghĩa 4, nhờ các công thức $1_E-b(u)^*b(u) = W(u) = (1_E+u^*u)^{-1}$ (mệnh đề 1 của IV, p. 262) và $b(u^*) =b(u)^*$ (hệ quả của loc. cit.).

Nếu $u$ là một toán tử bộ phận tự liên hợp trên E, thì $b(u)$ là Hermit (hệ quả của mệnh đề 2 của IV, p. 264), do đó $u$ là chuẩn tắc.

Cho D là đĩa đơn vị mở trong $\mathbf{C}$. Ta ký hiệu bởi $\beta$ hàm từ $\mathbf{C}$ vào D được xác định bởi $\beta (z) =z/\surd\overline{1 + |z|^2}$. Đó là một đồng phôi, mà hàm nghịch đảo thỏa $\beta^{-1}(z) =z/\surd\overline{1 - |z|^2}$ với $z\in D$.

Cho $u\in \mathscr{L}(E)$. Từ các công thức (2) và (3) của mệnh đề 1 ở IV, p. 262 suy ra rằng $u=\beta^{-1}(b(u))$, và do đó

$$
b(u) =\beta (u) \tag{5}
$$

#### Bổ đề 2 {#ts-iv-s5-lem-2 .statement tag=035G}

Cho X là một không gian tôpô địa phương compact và cho $\mu$ là một độ đo dương trên X.

a) Cho $g$ là một hàm $\mu$-đo được trên X. Toán tử phép nhân $m_g$ trên $L^2(X, \mu)$ là chuẩn tắc và $b(m_g) =m_{\beta\circ g}$;

b) Cho $h: X\rightarrow D$ là một hàm $\mu$-đo được. Tự đồng cấu $m_h$ thuộc $\Omega (L^2(X, \mu))$ và $B(m_h) =m_{\beta^{-1}\circ h}$.

Toán tử bộ phận $m_g$ là đóng với miền xác định trù mật. Vì $m^*_gm_g=$ $m_{\overline{g}}m_g=m_{|g|^2}$ (mệnh đề 23 của IV, p. 253 và mệnh đề 24 của IV, p. 255), ta có

$$
W(m_g) =-R(m_{|g|^2},-1) =m_{(1+|g|^2)^{-1}}
$$

(mệnh đề 22 của IV, p. 252). Điều này kéo theo

$$
b(m_g) =m_g\circ W(m_g)^{1/2}=m_g\circ m_{(1+|g|^2)^{-1/2}}=m_{\beta\circ g}
$$

theo công thức (2) của IV, p. 262, hệ quả của mệnh đề 6 của IV, p. 187 và bổ đề 6 của IV, p. 254. Cuối cùng, áp dụng mệnh đề 6 của IV, p. 187, ta thu được mệnh đề a).

Ta hãy chứng minh b). Vì $1- |h(x)|^2>0$ với mọi $x\in X$, ta có $m_h\in$ $\Omega (L^2(X, \mu))$ (hệ quả của Mệnh đề 6 của IV, p. 187). Vì ánh xạ $u\mapsto b(u)$ là đơn ánh (Mệnh đề 2 của IV, p. 264) và các tự đồng cấu $b(B(m_h))$ và $b(m_{\beta^{-1}\circ h})$ đều bằng $m_h$ theo mệnh đề a), suy ra $B(m_h) =m_{\beta^{-1}\circ h}$.

#### Định lý 1 (“Định lý phổ”) {#ts-iv-s5-thm-1 .statement tag=035H}

Cho $u$ là một toán tử bộ phận chuẩn tắc trên không gian Hilbert E. Tồn tại một không gian tôpô compact địa phương X, một độ đo dương $\mu$ trên X, một đẳng cấu đẳng cự $\theta$ của $L^2(X, \mu)$ lên E, và một hàm liên tục $g$ trên X, sao cho $u=\theta \circ m_g\circ \theta^{-1}$.

Theo định nghĩa, tự đồng cấu $b(u)$ của E là chuẩn tắc. Do định lý phổ cho các tự đồng cấu chuẩn tắc của E (Hệ quả 1 của IV, p. 193), vì vậy tồn tại một không gian tôpô compact địa phương $\widetilde{X}$, một độ đo dương $\mu$ trên $\widetilde{X}$, một đẳng cấu đẳng cự $\widetilde{\theta}$ của $L^2(\widetilde{X}, \mu)$ lên E, và một hàm liên tục bị chặn $h$ trên $\widetilde{X}$, sao cho $b(u)$ trùng với $\widetilde{\theta}\circ m_h\circ \widetilde{\theta}^{-1}$.

Gọi N là tập con đóng gồm các $x\in \widetilde{X}$ sao cho $|h(x)|\geqslant 1$. Vì tự đồng cấu $1-b(u)^*b(u) =\widetilde{\theta}\circ m_{1-|h|^2}\circ \widetilde{\theta}^{-1}$ là dương và đơn ánh, tập N là địa phương $\mu$-không đáng kể (Bổ đề 7 của IV, p. 186 và hệ quả của Mệnh đề 6 của IV, p. 187). Khi đó đặt $X =\widetilde{X}-$ N. Đó là một không gian compact địa phương, và sự hạn chế các hàm lên X cảm sinh một đẳng cấu đẳng cự của $L^2(\widetilde{X}, \mu)$ lên $L^2(X, \mu|X)$ (Mệnh đề 1 của IV, p. 179). Do đó hợp thành của $\widetilde{\theta}$ với sự hạn chế các hàm lên X cảm sinh một đẳng cấu đẳng cự $\theta$ của $L^2(X, \mu|X)$ lên E. Vì $b(u) =\theta \circ m_{h|X}\circ \theta^{-1}$, suy ra $u=\theta \circ m_{\beta^{-1}\circ(h|X)}\circ \theta^{-1}$ (Bổ đề 2). Định lý suy ra từ công thức này.

#### Bổ đề 3 {#ts-iv-s5-lem-3 .statement tag=035I}

Cho $u$ là một toán tử bộ phận chuẩn tắc trên E. Ta có

Sp($b(u)$)$\cap D =\beta$(Sp($u$)).

Ta có $b(u) =u\circ W(u)^{1/2}$ (Mệnh đề 1 của IV, p. 262). Tự đồng cấu $W(u)^{1/2}$ là đơn ánh và ảnh của nó là miền xác định của $u$ (công thức (1) của IV, p. 262).

Cho $\lambda \in \mathbf{C}$. Số $\lambda$ thuộc tập phân giải của $u$ khi và chỉ khi $(u-\lambda 1_E)\circ W(u)^{1/2}$ là một ánh xạ tuyến tính song ánh của E vào E (Nhận xét 3 của IV, p. 245). Mà theo công thức (3) của IV, p. 262, ta có

$$
(u-\lambda 1_E)\circ W(u)^{1/2}=b(u)-\lambda (1_E-b(u)^*b(u))^{1/2}=f_{\lambda}(b(u))
$$

trong đó $f_{\lambda}$ là hàm liên tục được xác định trên $\overline{D}$ bởi $z\mapsto z-\lambda (1- |z|^2)^{1/2}$. Tự đồng cấu $f_{\lambda}(b(u))$ là song ánh khi và chỉ khi phổ của nó không chứa 0. Vì Sp($f_{\lambda}(b(u))$) $=f_{\lambda}$(Sp($b(u)$)) (Hệ quả 2 của Mệnh đề 7 của I, p. 111), điều này xảy ra khi và chỉ khi 0 không thuộc tập hợp $f_{\lambda}$(Sp($b(u)$)). Do đó, $\lambda \in$ Sp($u$) khi và chỉ khi tồn tại $z\in$ Sp($b(u)$)$\cap D$ sao cho

$$
z-\lambda (1- |z|^2)^{1/2}= 0
$$

Đẳng thức này, nếu đúng, suy ra rằng $z\in D$, và có nghĩa là $\lambda =\beta^{-1}(z)$. Suy ra Sp($u$) $=\beta^{-1}$(Sp($b(u)$)$\cap D$), như đã phát biểu.

Cho $u$ là một toán tử riêng phần chuẩn tắc trên E. Cho $f\in \mathscr{K}$ (Sp($u$)). Ánh xạ $z\mapsto f(\beta^{-1}(z))$ từ Sp($b(u)$)$\cap D$ vào $\mathbf{C}$ là liên tục và có giá compact; do đó ánh xạ duy nhất $f_{\beta}$ từ Sp($b(u)$) vào $\mathbf{C}$ kéo dài nó bằng không là liên tục.

#### Định nghĩa 3 {#ts-iv-s5-def-3 .statement tag=035J}

Với mọi hàm $f\in \mathscr{K}$ (Sp($u$)), ta định nghĩa tự đồng cấu $f(u)$ của E bởi $f(u) =f_{\beta}(b(u))$.

Ánh xạ $f\mapsto f_{\beta}$ là một cấu xạ đại số phức từ $\mathscr{K}$ (Sp($u$)) vào $\mathscr{C}$(Sp($b(u)$)), do đó ánh xạ $f\mapsto f(u)$ là một cấu xạ đại số phức từ $\mathscr{K}$ (Sp($u$)) vào $\mathscr{L}(E)$. Ta có $\overline{f}(u) =f(u)^*$ vì $\overline{f}_{\beta}=\overline{f_{\beta}}$. Nếu $f\geqslant 0$ thì $f_{\beta}\geqslant 0$, do đó $f(u)$ là một tự đồng cấu dương của E.

#### Nhận xét {#ts-iv-s5-n2-rem-3 .statement tag=035K}

Giả sử rằng $u$ là một tự đồng cấu chuẩn của E, sao cho Sp($u$) là một tập con compact của $\mathbf{C}$. Vì biến đổi bị chặn $b(u)$ trùng với $\beta (u)$ (công thức (5)), và Sp($b(u)$) $=\beta$(Sp($u$)) (Hệ quả 2 của Mệnh đề 7 của I, p. 111), phổ của $b(u)$ là một tập con compact của D. Với mọi hàm liên tục $f\in \mathscr{C}$ (Sp($u$)), hàm $f_{\beta}$ trùng với hạn chế của $f\circ \beta^{-1}$ lên Sp($u$). Do đó, $f_{\beta}(\beta (u))$ trùng với tự đồng cấu $f(u)$ được xác định bởi phép tính phiếm hàm liên tục của $u$. Định nghĩa trên do đó tương thích với định nghĩa của phép tính phiếm hàm liên tục của đại số đối hợp $\mathscr{L}(E)$.

Cho $f\in \mathscr{K}$ (Sp($u$)). Ta có

$$
\|f(u)\|\leqslant \|f_{\beta}\|_{\infty}=\|f\|_{\infty}
$$

sao cho, với mọi $x$ và $y$ trong E, ta thu được bất đẳng thức $|\langle x|f(u)y\rangle |\leqslant \|x\| \|y\| \|f\|_{\infty}$. Ánh xạ $f\mapsto  \langle x|f(u)y\rangle$ do đó là một độ đo bị chặn trên Sp($u$), có khối lượng toàn phần $\leqslant \|x\|\|y\|$ (INT, IV, p. 154, § 4, n$^o7$). Nếu $x=y$, nó là một độ đo dương, vì $f(u)$ là dương khi $f\geqslant 0$.

#### Định nghĩa 4 {#ts-iv-s5-def-4 .statement tag=035L}

Cho $u$ là một toán tử từng phần chuẩn trên một không gian Hilbert phức E. Cho $x$ và $y$ thuộc E. Độ đo bị chặn trên Sp($u$) được xác định bởi $f\mapsto  \langle x|f(u)y\rangle$ với $f\in \mathscr{K}$ (Sp($u$)) được gọi là độ đo phổ của $(x, y)$ đối với $u$. Khi $x=y$, người ta nói rằng đó là độ đo phổ của $x$ đối với $u$.

#### Nhận xét 1 {#ts-iv-s5-n2-rem-1 .statement tag=035M}

Khi $u$ là liên tục, định nghĩa này trùng với định nghĩa của Định nghĩa 2 của IV, p. 190.

#### Nhận xét 2 {#ts-iv-s5-n2-rem-2 .statement tag=035N}

Cho $j$ là phép nhúng chính tắc của Sp($u$) vào $\mathbf{C}$. Vì Sp($u$) là đóng, ánh xạ $j$ là $\mu$-thực sự đối với mọi độ đo bị chặn $\mu$ trên Sp($u$) (INT, V, p. 68, § 6, n$^o1$, Mệnh đề 1). Người ta thường đồng nhất các độ đo phổ của $u$ với các độ đo trên $\mathbf{C}$ là ảnh của chúng qua $j($cf. INT, V, p. 84, § 7, n$^o2)$.

Ánh xạ của $E\times E$ vào không gian Banach $\mathscr{M}^1$(Sp($u$)) gán cho $(x, y)$ độ đo phổ của $(x, y)$ tương đối với $u$ là sesqui tuyến tính và liên tục có chuẩn $\leqslant 1$.

#### Bổ đề 4 {#ts-iv-s5-lem-4 .statement tag=035O}

Cho X là một không gian tôpô compact địa phương, cho $\mu$ là một độ đo dương trên X, và cho $g$ là một hàm $\mu$-đo được trên X. Gọi $m_g$ là toán tử của phép nhân bởi $g$ trên $L^2(X, \mu)$.

a) Ánh xạ $f\mapsto f(m_g)$ của $\mathscr{K}$ (Sp($m_g$)) vào $\mathscr{L}(L^2(X, \mu))$ được cho bởi $f\mapsto m_{f\circ g}$;

b) Với $f_1$ và $f_2$ thuộc $\mathscr{L}^2(X, \mu)$ có các lớp $\widetilde{f}_1$ và $\widetilde{f}_2$ trong $L^2(X, \mu)$, độ đo phổ suy ra từ độ đo ảnh $g(\frac{(}{f}\widetilde{f}_{11}f,_2\widetilde{f}\cdot^2\mu)$ )tương đối với. $m_g$ là hạn chế tới Sp($m_g$)

Toán tử từng phần $m_g$ là chuẩn và $b(m_g) =m_{\beta\circ g}=m_{g(1+|g|^2)^{-1/2}}$ (bổ đề 2). Hơn nữa $\beta (g(x))$ thuộc Sp($m_{\beta\circ g}$) với mọi $x$ bên ngoài một tập hợp không đáng kể địa phương đối với $\mu$ $Y\subset X$ (mệnh đề 22 của IV, p. 252 và bổ đề 1 của IV, p. 181). Vì $f_{\beta}(\beta (g(x))) =f(g(x))$ với mọi $x\in X$ - Y, suy ra rằng $f(m_g) =m_{f\circ g}$ từ định nghĩa 3 và hệ quả của mệnh đề 6 của IV, p. 187.

Cho $f_1$ và $f_2$ thuộc $\mathscr{L}^2(X, \mu)$ có các lớp $\widetilde{f}_1$ và $\widetilde{f}_2$ trong $L^2(X, \mu)$. Vì độ đo $\nu =f_1f_2\cdot \mu$ bị chặn, độ đo ảnh $g(\nu )$ được xác định (INT, V, p. 69, § 6, n$^o1$, nhận xét. 1). Cho $f\in \mathscr{K}$ (Sp($m_g$)). Ta có $f(m_g) =m_{f\circ g}$ theo a), do đó

$$
\langle \widetilde{f}_1|f(m_g)\widetilde{f}_2\rangle =\int_X\overline{f}_1(f\circ g)f_2d\mu=\int_X(f\circ g) (\overline{f}_1f_2d\mu) =\int_{\mathbf{C}}f d\nu
$$

(INT, V, p. 69, § 6, n$^o1$, công thức (1)), điều này chứng minh mệnh đề b).

#### Ví dụ {#ts-iv-s5-n2-exa-1 .statement tag=035P}

Cho $n\in \mathbf{N}$. Ta trang bị cho $\mathbf{R}^n$ độ đo Lebesgue, và ta đồng nhất $\mathbf{R}^n$ và nhóm đối ngẫu của nó như trong hệ quả 3 của II, p. 236. Gọi N là chuẩn Euclid trên $\mathbf{R}^n$ và $\mathscr{F}$ là biến đổi Fourier trên $\mathscr{S}(\mathbf{R}^n)$ và trên $\mathscr{S}'(\mathbf{R}^n)$ (n$^o12$ của IV, p. 217).

Cho $\Delta_{\mathscr{S}}$ là toán tử bộ phận trên $L^2(\mathbf{R}^n)$ có miền xác định là không gian $\mathscr{S}(\mathbf{R}^n)$ và sao cho

$$
\Delta_{\mathscr{S}}(\varphi ) =-\sum_{i=1}^n\partial_i^2\varphi
$$

với mọi $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Khi đó ta có $\mathscr{F}(\Delta_{\mathscr{S}}(\varphi )) = 4\pi^2N^2\mathscr{F}(\varphi )$ với mọi hàm $\varphi \in \mathscr{S}(\mathbf{R}^n)$ (nhận xét 12 của IV, p. 220). Vì biến đổi Fourier là một tự đẳng cấu của $\mathscr{S}(\mathbf{R}^n)$ (mệnh đề 18 của IV, p. 219), điều này có nghĩa là toán tử bộ phận $u=\mathscr{F}\circ \Delta_{\mathscr{S}}\circ \mathscr{F}^{-1}$ là hạn chế của toán tử phép nhân $m_{4\pi^2N^2}$ lên không gian $\mathscr{S}(\mathbf{R}^n)$. Toán tử bộ phận $u$ là đóng được và đối xứng; bao đóng của nó là toán tử bộ phận tự liên hợp dương $m_{4\pi^2N^2}$ (mệnh đề 6 của IV, p. 232, áp dụng cho không gian $\mathscr{D}(\mathbf{R}^n)\subset \mathscr{S}(\mathbf{R}^n)$ với sự trợ giúp của mệnh đề 4 của IV, p. 202). Do đó, toán tử bộ phận $\Delta_{\mathscr{S}}$ là tự liên hợp cơ bản. Bao đóng của nó được ký hiệu bởi Δ; nó là một toán tử tự liên hợp dương, và nó là toán tử Laplace duy nhất trên $\mathbf{R}^n($xem ví dụ của No.$^o6$ của IV, p. 243 và hệ quả của mệnh đề 26 của IV, p. 257).

Theo mệnh đề 21 của IV, p. 223, không gian Sobolev $H^2(\mathbf{R}^n)$ là tập hợp các $f\in L^2(\mathbf{R}^n)$ sao cho $(1 + N^2)\mathscr{F}(f)$ thuộc $L^2(\mathbf{R}^n)$, nghĩa là sao cho $\mathscr{F}(f)$ thuộc miền xác định của $m_{4\pi^2N^2}$. Vì biến đổi Fourier là một đẳng cấu đẳng cự của không gian $L^2(\mathbf{R}^n)$ lên chính nó (định lý 1 của II, p. 215), miền xác định của toán tử Laplace Δ là $H^2(\mathbf{R}^n)$. Ta có $\Delta  =\mathscr{F}^{-1}\circ m_{4\pi^2N^2}\circ \mathscr{F}$. Đặc biệt, phổ của Δ bằng $\mathbf{R}_+$.

### 3. Phép tính phiếm hàm đo được phổ quát

Trong No. này, các không gian Hilbert được xét là phức.

Cho $u$ là một toán tử bộ phận chuẩn trên một không gian Hilbert E. Ký hiệu $\mu_{x,y}$ (tương ứng $\mu_y$) là độ đo phổ của $(x, y)\in E\times E$ (tương ứng của $y$) đối với $u$.

Cho $y\in E$. Ánh xạ $\mathscr{K}$ (Sp($u$))$\rightarrow E$ xác định bởi $f\mapsto f(u)(y)$ thỏa mãn

$$
\|f(u)(y)\|^2=\int|f|^2\mu_y=\|f\|^2_{\mathscr{L}^2(Sp(u),\mu_y)}
$$

Sp($u$)

Do đó tồn tại một ánh xạ tuyến tính đẳng cự duy nhất ev$_y$ của không gian $L^2$(Sp($u$)$, \mu_y$) vào E sao cho ev$_y(\widetilde{f}) =f(u)(y)$ nếu $\widetilde{f}$ là lớp của một hàm $f\in \mathscr{K}$ (Sp($u$)).

Cho $f$ là một hàm đo được phổ quát xác định trên phổ của $u$. Ký hiệu $D_f$ là tập hợp các phần tử $y\in E$ sao cho $f$ thuộc $\mathscr{L}^2$(Sp($u$)$, \mu_y$).

#### Mệnh đề 3 {#ts-iv-s5-prop-3 .statement tag=035Q}

Cho $f$ là một hàm đo được phổ quát được xác định trên phổ của $u$. Tập hợp $D_f$ là một không gian con vectơ trù mật của E. Ánh xạ $y\mapsto$ ev$_y(f)$ là một toán tử từng phần chuẩn trên E có miền xác định là $D_f$, và được ký hiệu là $f(u)$.

Với mọi $x\in E$ và mọi $y\in D_f$, ta có $f\in \mathscr{L}^1$(Sp($u$)$, \mu_{x,y}$) và

$$
\langle x|f(u)y\rangle =\int f \mu_{x,y} \tag{6}
$$

Sp($u$)

Ta sẽ chứng minh mệnh đề chính xác hơn sau đây:

#### Mệnh đề 4 {#ts-iv-s5-prop-4 .statement tag=035R}

Cho $f$ là một hàm đo được phổ quát trên phổ của $u$.

a) Tập hợp $D_f$ là một không gian con vectơ trù mật của E. Ánh xạ $f(u) :y\mapsto$ ev$_y(f)$ từ $D_f$ vào E là tuyến tính và trùng với $1_E$ nếu $f= 1$;

b) Cho $g\in \mathscr{L}_u$(Sp($u$)). Với mọi $y\in D_f$ và mọi $x\in D_g$, ta có $f g\in \mathscr{L}^1$(Sp($u$)$, \mu_{x,y}$), và

$$
\langle g(u)x|f(u)y\rangle =\int gf \mu_{x,y} \tag{7}
$$

Sp($u$)

c) Giả sử rằng $E = L^2(X, \mu)$ trong đó X là một không gian tôpô compact địa phương và $\mu$ là một độ đo dương trên X, và $u=m_h$, trong đó $h: X\rightarrow \mathbf{C}$ là $\mu$-đo được. Ta có $f(m_h) =m_{f\circ h}$.

Theo Định lý 1 của IV, p. 266, ta có thể giả sử rằng ta ở trong tình huống của mệnh đề c), nghĩa là $E = L^2(X, \mu)$ và $u=m_h$, trong đó X là một không gian tôpô compact địa phương, $\mu$ là một độ đo dương trên X và $h: X\rightarrow \mathbf{C}$ là $\mu$-đo được. Ta sẽ ký hiệu bởi $\widetilde{\varphi}$ lớp trong $L^2(X, \mu)$ của một hàm $\varphi \in \mathscr{L}^2(X, \mu)$.

Đặt S = Sp($m_h$). Ta ký hiệu bởi $\mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2}$ (tương ứng. $\mu_{\widetilde{\varphi}}$) độ đo phổ của $(\widetilde{\varphi}_1,\widetilde{\varphi}_2)$ (tương ứng. của $\widetilde{\varphi}$) đối với $m_h$ với mọi $(\varphi_1, \varphi_2)\in \mathscr{L}^2(X, \mu)^2$ (tương ứng. mọi $\varphi \in \mathscr{L}^2(X, \mu)$).

Cho $\varphi \in \mathscr{L}^2(X, \mu)$. Độ đo phổ $\mu_{\widetilde{\varphi}}$ bằng độ đo ảnh $h(|\varphi |^2\cdot \mu)$ trên S (Bổ đề 4 của IV, p. 269). Vì hàm $f$ là $\mu_{\varphi}$-đo được, ta có $\varphi \in D_f$ khi và chỉ khi các tích phân

$$
\int_S^*|f|^2d\mu_{\widetilde{\varphi}}=\int_S^*|f|^2h(|\varphi |^2d\mu) =\int_X^*|f\circ h|^2|\varphi |^2d\mu
$$

là hữu hạn (INT, V, p. 70, § 6, n$^o2$, Mệnh đề 2). Điều này có nghĩa là $D_f$ là miền của toán tử phép nhân $m_{f\circ h}$, là một không gian con trù mật của E (Mệnh đề 5 của IV, p. 232).

Hạn chế của ev$_{\widetilde{\varphi}}$ trên các lớp của các hàm $g\in \mathscr{K}(S)$ là ánh xạ gán cho một lớp $\widetilde{g}$ phần tử $g(m_h)(\widetilde{\varphi}) =m_{g\circ h}(\widetilde{\varphi})$ (Bổ đề 4 của IV, p. 269). Ánh xạ ev$_{\varphi}$ do đó trùng với ánh xạ đẳng cự từ $L^2(S, \mu_{\varphi})$ vào $L^2(X, \mu)$ suy ra bằng cách chuyển qua các thương từ ánh xạ $g\widetilde{\mapsto}(g\circ h)\cdot \varphi$ của $\mathscr{L}^2(S, \mu_{\widetilde{\varphi}})$ vào $\mathscr{L}^2(X, \mu)$.

Đặc biệt, do đó, ta có ev$_{\varphi}(f) =m_{f\circ h}(\widetilde{\varphi})$, sao cho ánh xạ $f(m_h)$ từ $D_f$ vào E trùng với toán tử từng phần $m_{f\circ h}$. Điều này chứng minh mệnh đề c); nếu $f= 1$, ta tìm được ev$_{\varphi}(1) =\widetilde{\varphi}$, điều này cũng kết thúc chứng minh của a).

Ta chứng minh mệnh đề b). Cho $\varphi_1$ và $\varphi_2$ là các hàm sao cho $\widetilde{\varphi}_1\in D_f$ và $\widetilde{\varphi}_2\in D_g$. Khi đó ta có (INT, V, tại chỗ đã dẫn)

$$
\int_S^*|f g| |\mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2}|=\int_X^*|(f\circ h)(g\circ h)\varphi_1\varphi_2|d\mu
$$

$$
\leqslant \|(f\circ h)\varphi_1\| \|(g\circ h)\varphi_2\|
$$

là hữu hạn; do đó $f g\in \mathscr{L}^1(S, \mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2})$. Hơn nữa, khi đó ta có

$$
\langle g(m_h)(\widetilde{\varphi}_2)|f(m_h)(\widetilde{\varphi}_1)\rangle =\int_X\overline{(g\circ h) \varphi_2}(f\circ h)\varphi_1d\mu
$$

$$
=\int_Sgf d\mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2}
$$

điều này kết thúc chứng minh.

#### Định nghĩa 5 {#ts-iv-s5-def-5 .statement tag=035S}

Ánh xạ $f\mapsto f(u)$ của $\mathscr{L}_u$(Sp($u$)) vào tập hợp các toán tử từng phần chuẩn tắc trên E được xác định bởi Mệnh đề 3 của IV, p. 271 được gọi là ánh xạ phép tính phiếm hàm đo được phổ quát liên kết với $u$.

Nói chung hơn, cho T là một tập hợp và $g:$ Sp($u$)$\times T\rightarrow \mathbf{C}$ là một ánh xạ; cho $t\in T$ sao cho hàm $g_t:z\mapsto g(z, t)$ là đo được phổ quát trên Sp($u$). Khi đó ta viết $g(u, t) =g_t(u)$.

Công thức (7) suy ra đặc biệt rằng (8) $\|f(u)(y)\|^2=\int|f|^2\mu_y$

Sp($u$)

với mọi $f\in \mathscr{L}_u$(Sp($u$)) và mọi $y\in D_f$. Lấy $f= 1$, ta suy ra rằng $\mu_y$ là một độ đo dương có khối lượng toàn phần $\|y\|^2$.

Nếu $u$ là một toán tử từng phần chuẩn tắc trên một không gian Hilbert E và $f\in \mathscr{K}$ (Sp($u$)), thì $D_f= E$ và toán tử từng phần $f(u)$ khi đó là liên tục, vì

$$
\|f(u)y\|\leqslant \|f\|_{\infty}\|y\|
$$

với mọi $y\in E$ theo (8). Tự đồng cấu $f(u)$ trùng với tự đồng cấu trong Định nghĩa 3 của IV, p. 268.

#### Hệ quả 1 {#ts-iv-s5-def-5-cor-1 .statement tag=035T}

a) Với mọi $f\in \mathscr{L}_u$(Sp($u$)), toán tử bộ phận $f(u)$ là chuẩn và $f(u)^*=\overline{f}(u)$. Hơn nữa, $f(u)$ là dương nếu $f\geqslant 0$, và tự liên hợp nếu $f$ là hàm thực;

b) Cho $k\in \mathbf{N}$ và $f(z) =z^k$ với $z\in$ Sp($u$). Khi đó $f(u) =u^k$;

c) Cho $\lambda \in \mathbf{C}-$ Sp($u$) và $f(z) = (\lambda -z)^{-1}$ với $z\in$ Sp($u$). Khi đó $f(u) = R(u, \lambda )$;

d) Ta có $\beta (u) =b(u)$;

e) Cho $f\in \mathscr{L}_u$(Sp($u$)) và $g\in \mathscr{L}_u$(Sp($u$)) sao cho $|g|\leqslant 1 +|f|$. Miền xác định của $g(u)$ là một lõi của $f(u)$.

Theo định lý phổ (định lý 1 của IV, p. 266), điều này suy ra từ mệnh đề trước đó kết hợp tương ứng với:

a) bổ đề 2, a) của IV, p. 266, mệnh đề 23 của IV, p. 253, và hệ quả của nó;

b) mệnh đề 24, b) của IV, p. 255;

c) mệnh đề 22, b) của IV, p. 252;

d) bổ đề 2, a) của IV, p. 266;

e) mệnh đề 6, b) của IV, p. 232.

#### Nhận xét {#ts-iv-s5-n3-rem-1 .statement tag=035U}

Với $f=$ Id$_{Sp(u)}$, ta có $f(u) =u$ (mệnh đề b) với $k= 1$). Do đó miền xác định của $u$ trùng với tập hợp các $x\in E$ sao cho hàm đồng nhất của Sp($u$) thuộc về $\mathscr{L}^2$(Sp($u$)$, \mu_x$); đặc biệt nó chứa các phần tử $x\in E$ sao cho độ đo $\mu_x$ có giá compact.

Hệ quả sau đây tổng quát hóa hệ quả của mệnh đề 16 của IV, p. 247 và mệnh đề 17 của IV, p. 248.

#### Hệ quả 2 {#ts-iv-s5-def-5-cor-2 .statement tag=035V}

Cho $u$ là một toán tử bộ phận chuẩn trên không gian Hilbert E. Giả sử rằng E là khác không.

a) Phổ của $u$ là khác rỗng;

b) Với mọi $\lambda \in \mathbf{C}-$ Sp($u$), chuẩn của giải thức $R(u, \lambda )$ bằng $1/\delta$, trong đó $\delta  >0$ là khoảng cách trong $\mathbf{C}$ từ $\lambda$ đến phổ của $u$.

c) Với mọi $\varepsilon  >$ 0, giả phổ $\varepsilon$ PSp$_{\varepsilon}(u)$ là tập hợp các $\lambda \in \mathbf{C}$ ở khoảng cách $< \varepsilon$ từ Sp($u$).

Giả sử phổ của $u$ là rỗng. Khi đó $u$ là đơn ánh, và tự đồng cấu $u^{-1}=-R(u,0)$ là chuẩn (hệ quả 1, c) và a)). Ta có Sp($u^{-1}$)$\subset  \{0\}$ (mệnh đề 15, a)), do đó Sp($u^{-1}$) $=\{0\}($I, p. 26, hệ quả 1). Vì $u^{-1}$ là chuẩn, điều này suy ra $u^{-1}= 0 ($I, p. 110, ví dụ 1), điều này mâu thuẫn vì E không là không.

Để chứng minh b), ta có thể giả sử rằng $u$ là toán tử phép nhân $m_g$ trên $L^2(X, \mu)$, trong đó $g$ là một hàm liên tục trên một không gian tôpô compact địa phương X được trang bị một độ đo dương $\mu$ (định lý 1 của IV, p. 266). Cho $\lambda \in \mathbf{C}-$ Sp($u$) và cho $\delta  >0$ là khoảng cách từ $\lambda$ đến phổ của $u$. Để chứng minh rằng $\|R(u, \lambda )\|=\delta^{-1}$, ta quy về trường hợp $\lambda = 0$ bằng cách thay thế $u$ bởi $u-\lambda 1_E$. Số thực $\delta$ khi đó là khoảng cách từ 0 đến phổ của $m_g$. Vì phổ sau cùng trùng với ảnh $\mu$-cốt yếu của $g$, kết quả là một hệ quả của bổ đề 3 của IV, p. 182.

Cuối cùng, mệnh đề c) suy ra từ b) và từ định nghĩa của PSp$_{\varepsilon}(u)$ (IV, p. 250, định nghĩa 9).

#### Hệ quả 3 {#ts-iv-s5-def-5-cor-3 .statement tag=035W}

Cho $u$ là một toán tử chuẩn bộ phận trên một không gian Hilbert E. Cho $f\in \mathscr{L}_u$(Sp($u$)). Với mọi $x$ và $y$ trong E, độ đo phổ của $(x, y)$ đối với $f(u)$ là độ đo ảnh $f(\mu)$, trong đó $\mu$ là độ đo phổ của $(x, y)$ đối với $u$.

Theo định lý phổ (định lý 1 của IV, p. 266), ta có thể giả sử rằng $u$ là toán tử phép nhân $m_g$ trên $L^2(X, \mu)$, trong đó X là một không gian tôpô compact địa phương, $\mu$ là một độ đo dương trên X và $g\in \mathscr{C}(X)$. Cho $f_1$ và $f_2$ thuộc $\mathscr{L}^2(X, \mu)$, với các lớp $\widetilde{f}_1$ và $\widetilde{f}_2$ trong $L^2(X, \mu)$. Vì $f(m_g) =m_{f\circ g}$ (mệnh đề 4, c)), độ đo phổ của $(\widetilde{f}_1,\widetilde{f}_2)$ đối với $f(m_g)$ là độ đo ảnh $(f\circ g)(\overline{f}_1f_2\cdot \mu)$ (bổ đề 4, b) của IV, p. 269). Độ đo này bằng độ đo ảnh $f(g(f_1f_2\cdot \mu))$ (INT, V, p. 72, § 6, n$^o4$, mệnh đề 4, a)), do đó có mệnh đề cần chứng minh (bổ đề 4, b) của IV, p. 269).

#### Hệ quả 4 {#ts-iv-s5-def-5-cor-4 .statement tag=035X}

Cho $g\in \mathscr{L}_u$(Sp($f(u)$)). Ta có $g(f(u)) = (g\circ f)(u)$.

Ta có $g\circ f\in \mathscr{L}_u$(Sp($u$)) (bổ đề 5 của IV, p. 184). Với mọi $x$ và $y$ trong E, ký hiệu $\mu'_{x,y}$ là độ đo phổ của $(x, y)$ đối với $f(u)$. Theo hệ quả trước và INT, V, p. 71, § 6, No. 2, đl. 1, ta có $g\in \mathscr{L}^2$(Sp($f(u)$)$, \mu'_{x,y}$) khi và chỉ khi $g\circ f\in \mathscr{L}^2$(Sp($u$)$, \mu_{x,y}$), do đó miền xác định của $g(f(u))$ bằng miền xác định của $(g\circ f)(u)$. Với mọi $x\in E$ và $y\in$ dom($g(f(u))$), khi đó ta có công thức

$$
\langle x|g(f(u))y\rangle =\int g \mu'_{x,y}
$$

Sp($f(u)$)

$=\int g f(\mu_{x,y}) =\langle x|(g\circ f)y\rangle$

Sp($f(u)$)

(đã dẫn), do đó $g(f(u)) = (g\circ f)(u)$.

#### Mệnh đề 5 {#ts-iv-s5-prop-5 .statement tag=035Y}

Cho $u$ là một toán tử bộ phận chuẩn trên một không gian Hilbert E.

a) Nếu $f\in \mathscr{L}_u^{\infty}$(Sp($u$)), thì $f(u)\in \mathscr{L}(E)$;

b) Nếu $f\in \mathscr{L}_u^{\infty}$(Sp($u$)) và $g\in \mathscr{L}_u$(Sp($u$)), thì $f(u)\circ g(u)\subset (f g)(u)$;

c) Ánh xạ $f\mapsto f(u)$ của $\mathscr{L}_u^{\infty}$(Sp($u$)) vào $\mathscr{L}(E)$ là một cấu xạ liên tục có đơn vị của các đại số có đối hợp. Đặc biệt, ta có $\|f(u)\|\leqslant \|f\|_{\infty}$ với $f\in \mathscr{L}_u^{\infty}$(Sp($u$));

d) Nếu $u\in \mathscr{L}(E)$, thì với mọi $f\in \mathscr{L}_u^{\infty}$(Sp($u$)), tự đồng cấu $f(u)$ thuộc đối giao hoán tử kép của $u$ trong $\mathscr{L}(E)$.

Cho $f\in \mathscr{L}_u^{\infty}$(Sp($u$)). Ta có $D_f= E$ và $f(u)$ là một tự đồng cấu liên tục của E theo công thức (8), p. 272, do đó mệnh đề a).

Cho $g\in \mathscr{L}_u$(Sp($u$)). Cho $y\in D_g$. Ta có $y\in D_{f g}$ và, với mọi $x\in E$, suy ra $\langle \overline{f}(u)x|g(u)y\rangle =\langle x|(f g)(u)y\rangle$ theo công thức (7), p. 271, do đó $f(u)(g(u)y) = (f g)(u)(y)$, điều này chứng minh b).

Từ a) và b), ánh xạ $f\mapsto f(u)$ của $\mathscr{L}_u^{\infty}$(Sp($u$)) vào $\mathscr{L}(E)$ là một cấu xạ có đơn vị của các đại số có đối hợp; do đó, nó là một cấu xạ liên tục có chuẩn $\leqslant 1$(I, p. 104, mệnh đề 2), do đó mệnh đề c).

Giả sử rằng $u$ là một tự đồng cấu của E. Cho $v\in \mathscr{L}(E)$ hoán vị được với $u$. Khi đó ta có $v\circ f(u) =f(u)\circ v$ với $f\in \mathscr{C}$ (Sp($u$)) theo các tính chất của phép tính phiếm hàm liên tục (I, p. 110, nhận xét). Cho $x$ và $y$ thuộc E. Các công thức

$$
\langle x|(v\circ f(u))y\rangle =\langle x|(f(u)\circ v)y\rangle \tag{9}
$$

đúng với mọi hàm $f\in \mathscr{C}$ (Sp($u$)), có nghĩa là các độ đo phổ của $(v^*(x), y)$ và của $(x, v(y))$ đối với $u$ là bằng nhau. Theo công thức (6), p. 271, đẳng thức này kéo theo rằng công thức (9) đúng với mọi $f\in \mathscr{L}_u^{\infty}$(Sp($u$)). Do đó $v\circ f(u) =f(u)\circ v$.

#### Hệ quả {#ts-iv-s5-n3-cor-1 .statement tag=035Z}

Cho $f$ và $g$ thuộc $\mathscr{L}_u$(Sp($u$)) và cho $(x, y)\in D_f\times D_g$. Độ đo phổ của $(f(u)x, g(u)y)$ đối với $u$ là độ đo $f g\cdot \mu_{x,y}$, trong đó $\mu_{x,y}$ là độ đo phổ của $(x, y)$ đối với $u$.

Gọi $\nu$ là độ đo phổ của $(f(u)x, g(u)y)$ đối với $u$. Với mọi hàm $\varphi \in \mathscr{K}$ (Sp($u$)), ta có

$$
\int\varphi  \nu =\langle f(u)x|\varphi (u)(g(u)y)\rangle
$$

Sp($u$)

$=\langle f(u)x|(\varphi g)(u)y\rangle =\int f \varphi g \mu_{x,y}$,

Sp($u$)

(mệnh đề 5, b)), do đó $\nu =f g\cdot \mu_{x,y}$.

#### Mệnh đề 6 {#ts-iv-s5-prop-6 .statement tag=0360}

Cho $u$ là một toán tử từng phần chuẩn tắc trên một không gian Hilbert E. Cho $(f_n)_{n\in\mathbf{N}}$ là một dãy trong $\mathscr{L}_u$(Sp($u$)) hội tụ đơn giản đến $f\in \mathscr{L}_u$(Sp($u$)) và sao cho tồn tại $g\in \mathscr{L}_u$(Sp($u$)) thỏa mãn $|f_n|\leqslant g$ với mọi $n\in \mathbf{N}$. Khi đó dom($g(u)$)$\subset$ dom($f_n(u)$) với mọi $n\in \mathbf{N}$ và dom($g(u)$)$\subset$ dom($f(u)$). Hơn nữa, với mọi phần tử $y$ của miền xác định của $g(u)$, ta có

$f(u)(y) =$ lim$_{n\rightarrow+\infty}f_n(u)(y)$.

Đặc biệt, nếu $f_n\in \mathscr{L}_u^{\infty}$(Sp($u$)) với mọi $n\in \mathbf{N}$ và nếu các hàm $f_n$ bị chặn đều, thì $f_n(u)$ hội tụ đến $f(u)$ trong không gian $\mathscr{L}(E)$ được trang bị tôpô của sự hội tụ đơn giản.

Ta ký hiệu $\mu_{x,y}$ (resp. $\mu_x$) là độ đo phổ của $(x, y)$ (resp. của $x$) tương ứng với $u$.

Cho $y\in$ dom($g(u)$), sao cho $g\in \mathscr{L}^2$(Sp($u$)$, \mu_y$). Điều kiện $|f_n|\leqslant g$ kéo theo rằng $f_n\in \mathscr{L}^2$(Sp($u$)$, \mu_y$), do đó $y\in$ dom($f_n(u)$).

Vì $(f_n)$ hội tụ đơn giản đến $f$ và $|f_n|\leqslant g$, ta có $f\in \mathscr{L}^2$(Sp($u$)$, \mu_y$) theo định lý Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6), do đó $y\in$ dom($f(u)$). Hơn nữa, dãy $(f_n)$ hội tụ đến $f$ trong $\mathscr{L}^2$(Sp($u$)$, \mu_y$), do đó chuẩn của $f_n(u)y$ hội tụ đến chuẩn của $f(u)y$.

Cho $x\in E$. Các hàm $f$ và $g$, cũng như các hàm $f_n$ với mọi $n\in \mathbf{N}$, thuộc $\mathscr{L}^1$(Sp($u$)$, \mu_{x,y}$) (mệnh đề 3). Theo định lý Lebesgue (INT, IV, loc. cit.), dãy $(f_n)$ hội tụ đến $f$ trong $\mathscr{L}^1$(Sp($u$)$, \mu_{x,y}$), do đó

$$
\langle x|f_n(u)y\rangle =\int f_n\mu_{x,y}\rightarrow \int f \mu_{x,y}=\langle x|f(u)y\rangle
$$

Sp($u$) Sp($u$)

Suy ra $f_n(u)(y)$ hội tụ đến $f(u)(y)$ (EVT, V, p. 17, mệnh đề 10).

#### Mệnh đề 7 {#ts-iv-s5-prop-7 .statement tag=0361}

Cho X là một không gian tôpô compact địa phương và $\nu$ là một độ đo trên X. Cho $g:\mathbf{C}\times X\rightarrow \mathbf{C}$ là một hàm liên tục có giá compact. Với $z\in \mathbf{C}$, đặt

$$
h(z) =\int_Xg(z, x)d\nu (x)
$$

a) Ánh xạ $h$ từ $\mathbf{C}$ vào $\mathbf{C}$ là liên tục và bị chặn;

b) Ánh xạ từ X vào $\mathscr{L}(E)$ được xác định bởi $x\mapsto g(u, x)$ là $\nu$-khả tích và ta có

$$
h(u) =\int_Xg(u, x)d\nu (x)
$$

Hàm $h$ bị chặn vì $g$ liên tục có giá compact, và nó liên tục theo INT, IV, p. 144, § 4, n$^o3$, hệ quả 1. Vì $g$ liên tục và có giá compact, ánh xạ $x\mapsto g(u, x)$ là liên tục từ X vào $\mathscr{L}(E)$ (TG, X, p. 28, th. 3 và mệnh đề 5, c)). Ánh xạ này có giá compact, do đó bị chặn và khả tích trên X đối với $\nu$. Ta viết

$$
v=\int_Xg(u, x)d\nu (x)\in \mathscr{L}(E)
$$

Cho $y$ và $z$ là các phần tử của E và $\mu$ là độ đo phổ của $(y, z)$ tương ứng với $u$. Ta có

$$
\langle y|v(z)\rangle =\int\langle y|g(u, x)z\rangle d\nu (x) =\int(\int g(\lambda , x)d\mu(\lambda ))d\nu (x)
$$

X X Sp($u$)

(công thức (6), p. 271). Vì $g\in \mathscr{K}(\mathbf{C}\times X)$, suy ra

$$
\langle y|v(z)\rangle =\int_{Sp(u)}(\int_Xg(\lambda , x)d\nu (x))d\mu(\lambda ) =\langle y|h(u)z\rangle
$$

theo INT, III, p. 84, § 4, n$^o1$, th. 2 và công thức (6), p. 271. Điều này chứng minh rằng $v=h(u)$, như cần chứng minh.

### 4. Các phép chiếu phổ

Cho $u$ là một toán tử chuẩn bộ phận trên một không gian Hilbert phức E. Cho A là một tập con đo được phổ quát của Sp($u$) và $\varphi_A$ là hàm đặc trưng của nó. Vì $\varphi_A$ bị chặn và thỏa mãn $\varphi^2_A=\varphi_A$, tự đồng cấu $\varphi_A(u)$ của E là một phép chiếu trực giao của E. Nó được gọi là phép chiếu phổ của $u$ xác định bởi A. Ta ký hiệu nó bởi $p_A=\varphi_A(u)$. Ta có $p_{\emptyset}= 0$ và $p_{Sp(u)}= 1_E$.

Cho A là một tập con đo được phổ quát của $\mathbf{C}$. Phép chiếu phổ của $u$ xác định bởi A là phép chiếu phổ $p_{Sp(u)\cap A}$. Nó cũng được ký hiệu đơn giản là $p_A$. Với mọi hàm $f\in \mathscr{L}_u$(Sp($u$)), mọi $x\in E$ và mọi $y\in$ dom($f(u)$), ta có công thức

$$
\langle p_A(x)|f(u)y\rangle =\int f d\mu \tag{10}
$$

Sp($u$)$\cap A$

trong đó $\mu$ là độ đo phổ của $(x, y)$ đối với $u$ (công thức (7), p. 271).

Cho A và B là các tập con đo được phổ quát của Sp($u$). Vì $\varphi_A\varphi_B=\varphi_{A\cap B}$, nên có $p_A\circ p_B=p_{A\cap B}$ (mệnh đề 5 của IV, p. 275, c)). Đặc biệt, nếu A và B rời nhau, các ảnh của $p_A$ và của $p_B$ là trực giao.

#### Mệnh đề 8 {#ts-iv-s5-prop-8 .statement tag=0362}

Cho $(A_i)_{i\in I}$ là một họ đếm được từng đôi một rời nhau gồm các tập con đo được phổ quát của Sp($u$), và cho $p_i$ là phép chiếu phổ của $u$ xác định bởi $A_i$. Hợp A của các tập $A_i$ là một tập con đo được phổ quát của Sp($u$), và chuỗi $\sum_ip_i$ hội tụ đến $p_A$ trong $\mathscr{L}(E)$ được trang bị tôpô của sự hội tụ đơn giản.

Tập A là đo được phổ quát theo INT, IV, p. 177, § 5, n$^o4$, hệ quả 2. Chuỗi $\sum_i\varphi_{A_i}$ hội tụ đơn giản đến $\varphi_A$ và các tổng riêng phần của nó bị chặn bởi 1. Do đó, mệnh đề suy ra từ mệnh đề 6 của IV, p. 276.

#### Mệnh đề 9 {#ts-iv-s5-prop-9 .statement tag=0363}

Cho A là một tập con đóng của Sp($u$). Cho $\varphi_A$ là hàm đặc số của A và $p_A=\varphi_A(u)$ là phép chiếu phổ của $u$ xác định bởi A. Ta ký hiệu $E_A$ là ảnh của $p_A$. Nó là một không gian con đóng của E.

a) Không gian con $E_A$ là không gian của các $x\in E$ sao cho giá của độ đo phổ của $x$ đối với $u$ được chứa trong A;

b) Nếu A bị chặn trong $\mathbf{C}$, thì $E_A$ được chứa trong miền xác định của $u$;

c) Với mọi $x$ thuộc miền xác định của $u$, ta có $p_A(x)\in$ dom($u$) và $u(p_A(x))\in E_A$, đặc biệt $u(x)\in E_A$ nếu $x\in$ dom($u$)$\cap E_A$.

Với $x$ trong E, người ta ký hiệu $\mu_x$ là độ đo phổ của $x$ đối với $u$.

Chứng minh a). Cho $x$ là một phần tử của $E_A$. Cho $z\in \mathbf{C}-$ A và U là một lân cận mở tương đối compact của $z$ không gặp A. Với mọi hàm $f\in \mathscr{K}(\mathbf{C})$ có giá được chứa trong U, ta có

$$
\int f \mu_x=\langle x|f(u)x\rangle =\langle p_A(x)|f(u)x\rangle =\int f \mu_x= 0
$$

Sp($u$) Sp($u$)$\cap A$ theo công thức (10). Điều này có nghĩa là $z$ không thuộc giá của $\mu_x$. Do đó, giá của $\mu_x$ được chứa trong A.

Ngược lại, cho $x\in E$ sao cho giá của $\mu_x$ được chứa trong A. Ta có

$$
\langle x|p_A(x)\rangle =\int\mu_x=\int\mu_x=\langle x|x\rangle
$$

Sp($u$)$\cap A$ Sp($u$)

(loc. cit.) do đó $\|p_A(x)-x\|^2=\|p_A(x)\|^2- \|x\|^2\leqslant 0$ và do đó $p_A(x) =x$, nghĩa là $x\in E_A$.

Mệnh đề b) suy ra từ a) và từ nhận xét trong IV, p. 273.

Chứng minh c). Miền xác định của $u$ là tập hợp các $x\in E$ sao cho hàm đồng nhất của Sp($u$) thuộc $\mathscr{L}^2$(Sp($u$)$, \mu_x$) $($loc. cit.). Vì $\mu_{p_A(x)}=\varphi_A\cdot \mu_x$ với $x\in E$ (hệ quả của Prop. 5 của IV, p. 275), ta có $p_A(x)\in$ dom($u$) nếu $x\in$ dom($u$).

Cho $x\in$ dom($u$) và $y=p_A(x)$; ta có $y\in$ dom($u$)$\cap E_A$ theo c). Độ đo phổ của $u(y)$ tương đối với $u$ là $|$Id$_{Sp(u)}|^2\cdot \mu_y($loc. cit.). Vì $\mu_y$ có giá trong A, điều tương tự cũng đúng với $\mu_{u(y)}$, do đó $u(y)\in E_A$ theo a).

#### Hệ quả {#ts-iv-s5-n4-cor-1 .statement tag=0364}

Cho $\lambda \in$ Sp($u$). Ảnh của $p_{\{\lambda\}}$ là không gian con thực sự của $u$ tương đối với $\lambda$.

Cho $x\in$ dom($u$). Gọi $\mu$ (tương ứng $\nu$ ) là độ đo phổ của phần tử $x$ đối với $u$ (tương ứng là độ đo phổ của $(x, u(x))$ đối với $u$). Ta có $\nu =$ Id$_{Sp(u)}\cdot \mu$ (Hệ quả của Mệnh đề 5 của IV, p. 275). Nếu $u(x) =\lambda x$, ta cũng có $\nu =\lambda \mu$, do đó có đẳng thức Id$_{Sp(u)}\cdot \mu=\lambda \mu$. Điều này suy ra rằng giá của $\mu$ được chứa trong $\{\lambda \}($xem INT, V, p. 46, § 5, n$^o3$, Hệ quả 2) và do đó $x$ thuộc ảnh của $p_{\{\lambda\}}$ (Mệnh đề 9, a)).

Ngược lại, giả sử rằng $x$ thuộc ảnh $E_{\lambda}$ của $p_{\{\lambda\}}$. Khi đó $x$ thuộc dom($u$) và $u(x)$ cũng thuộc $E_{\lambda}($loc. cit., b)). Vì $\varphi_{\{\lambda\}}\cdot$ (Id$_{Sp(u)}-\lambda$ ) $= 0$, ta có quan hệ $p_{\{\lambda\}}\circ (u-\lambda 1_E)\subset 0$ (Mệnh đề 5 của IV, p. 275, c)), do đó $0 =p_{\{\lambda\}}(u(x))-\lambda p_{\{\lambda\}}(x) =u(x)-\lambda x$.

#### Mệnh đề 10 {#ts-iv-s5-prop-10 .statement tag=0365}

Cho $\lambda \in \mathbf{C}$. Ta có $\lambda \in$ Sp($u$) khi và chỉ khi, với mọi lân cận mở V của $\lambda$ trong $\mathbf{C}$, phép chiếu phổ $p_V$ của $u$ đối với V là khác không.

Nếu $\lambda  \notin$ Sp($u$), thì tồn tại một lân cận mở V của $\lambda$ trong $\mathbf{C}$ không giao với Sp($u$), và khi đó $p_V=p_{\emptyset}= 0$.

Ngược lại, giả sử rằng tồn tại một lân cận mở V của $\lambda$ trong $\mathbf{C}$ sao cho $p_V= 0$. Cho $c >0$ là sao cho đĩa có tâm $\lambda$ và bán kính $c$ được chứa trong V.

Cho $x\in$ dom($u$) và gọi $\mu_x$ là độ đo phổ của $x$ đối với $u$. Vì $\mu_x(V) =\langle x|p_V(x)\rangle = 0$, ta tính được

$$
\int_{\mathbf{C}}|z-\lambda |^2d\mu_x(z) =\int_{\mathbf{C}-V}|z-\lambda |^2d\mu_x(z)
$$

$$
\geqslant c^2\int_{\mathbf{C}-V}d\mu_x(z) =c^2\int_{\mathbf{C}}d\mu_x(z) =c^2\|x\|^2
$$

Nhưng, mặt khác, ta có

$$
\|u(x)-\lambda x\|^2=\int_{\mathbf{C}}|z-\lambda |^2d\mu_x(z) =\|u^*(x)-\lambda x\|^2
$$

(công thức (8), p. 272), do đó $\|u(x)-\lambda x\|\geqslant c\|x\|$ và $\|u^*(x)-\lambda x\|\geqslant c\|x\|$. Suy ra rằng $\lambda$ thuộc tập giải thức của $u$ (Bổ đề 5 của IV, p. 248). Điều này kết thúc chứng minh.

#### Hệ quả {#ts-iv-s5-n4-cor-2 .statement tag=0366}

Cho A là một tập mở trong $\mathbf{C}$ và $n\in \mathbf{N}$. Nếu A chứa $n$ phần tử của Sp($u$), thì chiều của ảnh của phép chiếu phổ $p_A$ của $u$ tương đối với A ít nhất bằng $n$.

Cho $\lambda_1, . . .,\lambda_n$ là các phần tử phân biệt của phổ của $u$ thuộc A. Tồn tại một họ $(V_i)_{1\leqslant i\leqslant n}$ các tập mở rời nhau từng đôi một của $\mathbf{C}$ sao cho $\lambda_i\in V_i$ với $1\leqslant i\leqslant n$. Gọi B là hợp của các tập $V_i$. Ảnh của $p_A$ chứa ảnh của phép chiếu phổ $p_B$; hơn nữa $p_B$ là tổng của các phép chiếu $p_{V_i}$, và vì ảnh của $p_{V_i}$ trực giao với ảnh của $p_{V_j}$ với mọi $i\not =j$, kết quả suy ra từ Mệnh đề 10.

### 5. Công thức Helffer–Sjöstrand

Trong số này, E ký hiệu một không gian Hilbert phức. Ta sẽ thu được một công thức cho một số trường hợp của phép tính phiếm hàm của một toán tử từng phần tự liên hợp, được biểu diễn trực tiếp theo giải thức của toán tử đang xét.

Ta trang bị $\mathbf{R}$ (tương ứng $\mathbf{C}$) với độ đo Lebesgue, ký hiệu bởi $\mu$, và ta đồng nhất nhóm $\mathbf{R}$ và nhóm đối ngẫu của nó bằng ánh xạ $(x, y)\mapsto$ exp(2$i\pi xy$) $($xem Hệ quả 3 của II, p. 236).

Với mọi hàm $f$ được xác định và khả vi trên một tập mở U của $\mathbf{R}^2$, đồng nhất với $\mathbf{C}$, có các tọa độ thực $x$ và $y$, ta đặt

$$
\frac{\partial f}{\partial z}=\frac{1}{2}(\frac{\partial f}{\partial x}+i\frac{\partial f}{\partial y})
$$

(xem VAR, R2, 8.8.10, p. 24).

#### Bổ đề 5 {#ts-iv-s5-lem-5 .statement tag=0367}

Cho $f\in \mathscr{D}(\mathbf{R})$. Tồn tại một hàm $\widetilde{f}$ trong $\mathscr{D}(\mathbf{C})$ trùng với $f$ trên $\mathbf{R}$ và thỏa mãn

$$
\frac{\partial\widetilde{f}}{\partial z}(x,0) = 0 \tag{11}
$$

với mọi $x\in \mathbf{R}$. Khi đó ta có

$$
\frac{\partial\widetilde{f}}{\partial y}(x,0) =if'(x) \tag{12}
$$

với mọi $x\in \mathbf{R}$, và tồn tại một số thực $C\geqslant 0$ sao cho

$$
|\frac{\partial\widetilde{f}}{\partial z}(x, y)|\leqslant C|y| \tag{13}
$$

với mọi $(x, y)\in \mathbf{R}^2$.

Tồn tại $\varphi \in \mathscr{D}(\mathbf{R})$ có giá được chứa trong $[-2,2]$ và bằng 1 trên $[-1,1]$ (Bổ đề 1 của IV, p. 196). Đặt

$$
\widetilde{f}(x, y) =(f(x) +iyf'(x))\varphi (y)
$$

với $(x, y)\in \mathbf{R}^2$. Ta có $\widetilde{f}\in \mathscr{D}(\mathbf{C})$ và $\widetilde{f}$ trùng với $f$ trên $\mathbf{R}$. Hơn nữa, với mọi $(x, y)\in \mathbf{R}^2$, ta có được

$$
\frac{\partial\widetilde{f}}{\partial z}(x, y) =\frac{1}{2}((if(x)-yf'(x))\varphi '(y) +iyf''(x)\varphi (y))
$$

Vì hàm $\varphi$ bằng 1 trong một lân cận của 0, ta có $\varphi '(0) = 0$, do đó (11).

Cho $\widetilde{f}$ thuộc $\mathscr{D}(\mathbf{C})$ thỏa mãn (11). Công thức (12) suy ra từ điều này, và ước lượng (13) thu được nhờ định lý giá trị trung bình (FVR, I, p. 23, th. 2).

Người ta nói rằng $\widetilde{f}$ là một mở rộng gần giải tích của $f$.

#### Bổ đề 6 {#ts-iv-s5-lem-6 .statement tag=0368}

Cho $\varepsilon  >0$. Hàm $\sigma_{\varepsilon}$ được định nghĩa trên $\mathbf{R}$ bởi

$$
\sigma_{\varepsilon}(x) =\frac{2i\varepsilon x}{x^2 + \varepsilon^2}
$$

thuộc $L^2(\mathbf{R})$. Biến đổi Fourier của nó là lớp trong $L^2(\mathbf{R})$ của hàm $\eta_{\varepsilon}$ triệt tiêu tại 0 và thỏa mãn

$$
\eta_{\varepsilon}(y) =\frac{2\pi \varepsilon y}{|y|}e^{-2\pi \varepsilon|y|}
$$

với mọi $y\not = 0$.

Ta có $\sigma_{\varepsilon}\in L^2(\mathbf{R})$ theo mệnh đề 3 của IV, p. 199, và lớp của hàm $\eta_{\varepsilon}$ thuộc $L^2(\mathbf{R})\cap L^1(\mathbf{R})$. Với mọi $x\in \mathbf{R}$, ta có

$$
\overline{\mathscr{F}}(\eta_{\varepsilon})(x) = 2\pi \varepsilon \int_{\mathbf{R}_+}e^{2\pi(ix-\varepsilon)y}dy-2\pi \varepsilon \int_{\mathbf{R}_-}e^{2\pi(ix+\varepsilon)y}dy
$$

$$
=\frac{\varepsilon}{\varepsilon-ix}-\frac{\varepsilon}{\varepsilon + ix}=\frac{2i\varepsilon x}{x^2 + \varepsilon^2}
$$

do đó $\overline{\mathscr{F}}(\eta_{\varepsilon}) =\sigma_{\varepsilon}$. Kết quả khi đó suy ra từ công thức đảo Fourier trong $L^2(\mathbf{R})$ (hệ quả của định lý 2 của II, p. 220).

#### Bổ đề 7 {#ts-iv-s5-lem-7 .statement tag=0369}

Cho $f\in \mathscr{D}(\mathbf{R})$ và cho $\widetilde{f}\in \mathscr{D}(\mathbf{C})$ là một mở rộng gần giải tích của $f$. Với $\varepsilon  >0$, định nghĩa $f_{\varepsilon}$ trên $\mathbf{R}$ bởi

$$
f_{\varepsilon}(x) =-\frac{1}{2i\pi}\int_{\mathbf{R}}(\frac{\widetilde{f}(y + i\varepsilon)}{y-x + i\varepsilon}-\frac{\widetilde{f}(y-i\varepsilon)}{y-x-i\varepsilon})dy
$$

Khi đó $f_{\varepsilon}$ liên tục và bị chặn, và $f_{\varepsilon}$ hội tụ về $f$ trong $\mathscr{C}_b(\mathbf{R})$ khi $\varepsilon$ tiến tới 0.

Tính liên tục của $f_{\varepsilon}$ là một hệ quả của INT, IV, p. 144, § 4, n$^o3$, cor. 1, vì $\widetilde{f}$ có giá compact. Hơn nữa, nếu $r$ là số sao cho giá của $\widetilde{f}$ được chứa trong $[-r, r]\times \mathbf{R}$, ta có

$$
|f_{\varepsilon}(x)|\leqslant 2\|\widetilde{f}\|_{\infty}\int_{-r}^r\frac{1}{\surd(x-y)^2 + \varepsilon^2}dy\leqslant \frac{4r}{\varepsilon}\|\widetilde{f}\|_{\infty}
$$

do đó $f_{\varepsilon}$ bị chặn.

Khai triển Taylor đến cấp 1 (FVR, I, p. 30, prop. 3) và công thức (13) chứng minh rằng tồn tại $M\geqslant 0$ và một hàm $\varrho_1$ trên $\mathbf{R}^2$ sao cho

$\widetilde{f}(y+i\gamma ) =f(y) +i\gamma f'(y) +\gamma^2\varrho_1(y;\gamma )$, and $|\varrho_1(y;\gamma )|\leqslant M$,

với mọi $y\in \mathbf{R}$ và $\gamma \in \mathbf{R}$. Vì ánh xạ $y\mapsto \widetilde{f}(y+i\gamma )$ có giá được chứa trong $[-r, r]$ với mọi $\gamma \in \mathbf{R}$, ánh xạ $y\mapsto \varrho_1(y;\gamma )$ có giá được chứa trong $[-r, r]$, với mọi $\gamma \in \mathbf{R}$.

Cho $g_{\varepsilon}$ là hàm được định nghĩa trên $\mathbf{R}^2$ bởi

$$
g_{\varepsilon}(x, y) =\frac{\widetilde{f}(y + i\varepsilon)}{y-x + i\varepsilon}-\frac{\widetilde{f}(y-i\varepsilon)}{y-x-i\varepsilon}
$$

Với mọi $(x, y)\in \mathbf{R}^2$ và $\varepsilon  >0$, ta thu được

$$
g_{\varepsilon}(x, y) =-\frac{2i\varepsilon}{(x-y)^2 + \varepsilon^2}f(y) +\frac{2i\varepsilon(y-x)}{(x-y)^2 + \varepsilon^2}f'(y)
$$

$$
+\varepsilon^2(\frac{\varrho_1(y; \varepsilon)}{y-x + i\varepsilon}-\frac{\varrho_1(y;-\varepsilon)}{y-x-i\varepsilon})
$$

Cho $x\in \mathbf{R}$ và $\varepsilon  >0$. Ta có

$$
|\varepsilon^2\int_{\mathbf{R}}(\frac{\varrho_1(y;\varepsilon)}{y-x + i\varepsilon}-\frac{\varrho_1(y;-\varepsilon)}{y-x-i\varepsilon})dy|\leqslant 2M\varepsilon^2\int_{-r}^r\frac{dy}{\surd(x-y)^2 + \varepsilon^2}
$$

$$
\leqslant 4Mr\varepsilon
$$

Do đó, với mọi $x\in \mathbf{R}$, ta có

$$
f_{\varepsilon}(x) =-\frac{1}{2i\pi}\int_{\mathbf{R}}g_{\varepsilon}(x, y)dy= (f*\delta_{\varepsilon})(x)-\frac{1}{2i\pi}(f'*\sigma_{\varepsilon})(x) +k_{\varepsilon}(x)
$$

trong đó $\delta_{\varepsilon}$ và $\sigma_{\varepsilon}$ là các hàm trên $\mathbf{R}$ được xác định bởi

$$
\delta_{\varepsilon}(x) =\frac{1}{\pi}\frac{\varepsilon}{x^2 + \varepsilon^2},\sigma_{\varepsilon}(x) =\frac{2i\varepsilon x}{x^2 + \varepsilon^2}
$$

và $\|k_{\varepsilon}\|_{\infty}\leqslant 2Mr\varepsilon$.

Hàm $\mathscr{F}(f')\in \mathscr{S}(\mathbf{R})$ là khả tích (Mệnh đề 18 của IV, p. 219 và Mệnh đề 13 của IV, p. 213). Theo Bổ đề 6, ta có

$$
\int_{\mathbf{R}}|\mathscr{F}(f')(y)\mathscr{F}(\sigma_{\varepsilon})(y)|dy= 2\pi \varepsilon \int_{\mathbf{R}}|\mathscr{F}(f')(y)|e^{-2\pi \varepsilon|y|}dy
$$

$$
\leqslant 2\pi \varepsilon \int_{\mathbf{R}}|\mathscr{F}(f')(y)|dy
$$

do đó $\mathscr{F}(f')\mathscr{F}(\sigma_{\varepsilon})$ hội tụ về 0 trong $L^1(\mathbf{R})$ khi $\varepsilon$ tiến tới 0. Vì $f'$ và $\sigma_{\varepsilon}$ thuộc $L^2(\mathbf{R})$, Mệnh đề 14 của II, p. 223 suy ra rằng $f'*\sigma_{\varepsilon}=\overline{\mathscr{F}}(\mathscr{F}(f')\mathscr{F}(\sigma_{\varepsilon}))$ hội tụ về 0 trong $\mathscr{C}_b(\mathbf{R})$.

Với mọi $\varepsilon  >0$, độ đo dương $\delta_{\varepsilon}\cdot dx$ trên $\mathbf{R}$ có khối lượng toàn phần bằng 1 (xem FVR, III, p. 7). Tập hợp các độ đo $\delta_{\varepsilon}\cdot dx$ với $\varepsilon  >0$ và bộ lọc cảm sinh trên tập hợp này bởi bộ lọc các lân cận của 0 trong $\mathbf{R}_+^*$ thỏa mãn các giả thiết của Bổ đề 4 của INT, VIII, p. 137, § 2, n$^o7$. Các độ đo $\delta_{\varepsilon}\cdot dx$ do đó hội tụ trong $\mathscr{M}^1(\mathbf{R})$ tới độ đo điểm $\varepsilon_0$ khi $\varepsilon$ tiến tới 0. Suy ra $f*\delta_{\varepsilon}\rightarrow f$ trong $\mathscr{C}_b(\mathbf{R})$ (INT, VIII, p. 163, § 4, n$^o4$). Bổ đề được chứng minh.

Gọi $\mu$ là độ đo Lebesgue trên $\mathbf{C}$.

#### Định lý 2 (Helffer–Sjöstrand) {#ts-iv-s5-thm-2 .statement tag=036A}

Cho $u$ là một toán tử từng phần tự liên hợp trên E. Cho $f\in \mathscr{D}(\mathbf{R})$ và $\widetilde{f}\in \mathscr{D}(\mathbf{C})$ là một mở rộng gần giải tích của $f$. Cho $h$ là ánh xạ từ $\mathbf{C}$ vào $\mathscr{L}(E)$ được xác định bởi

$$
h(\lambda ) =\frac{\partial\widetilde{f}}{\partial z}(\lambda )R(u, \lambda )
$$

nếu $\lambda \in \mathbf{C}-\mathbf{R}$ và $h(\lambda ) = 0$ nếu $\lambda \in \mathbf{R}$. Khi đó $h$ là $\mu$-khả tích trên $\mathbf{C}$ và

$$
f(u) =-\frac{1}{\pi}\int_{\mathbf{C}}h(\lambda )d\mu(\lambda )
$$

Ánh xạ $h$ đo được và giá của nó là compact. Vì $u$ là tự liên hợp, ta có $\|R(u, \lambda )\|\leqslant |\mathscr{I}(\lambda )|^{-1}$ với mọi $\lambda \in \mathbf{C}-\mathbf{R}$ (Mệnh đề 17 của IV, p. 248). Do đó, ánh xạ $h$ bị chặn theo công thức (13), và do đó nó nguyên trên $\mathbf{C}$.

Cho $\varepsilon \in \mathbf{R}^*_+$. Ký hiệu $F^+_{\varepsilon}$ (tương ứng $F^-_{\varepsilon}$) là tập đóng trong $\mathbf{C}$ của các $\lambda \in \mathbf{C}$ sao cho $\mathscr{I}(\lambda )\geqslant \varepsilon$ (tương ứng $\mathscr{I}(\lambda )\leqslant -\varepsilon$ ). Ta có

$\int_{\mathbf{C}}h(\lambda )d\mu(\lambda ) =$ lim$_{\varepsilon\rightarrow 0}(\int_{F^+_{\varepsilon}}h(\lambda )d\mu(\lambda ) +\int_{F^-_{\varepsilon}}h(\lambda )d\mu(\lambda ))$.

Cho $r >0$ sao cho giá của $h$ được chứa trong $C = [-r, r]^2$. Ta ký hiệu $R_{\varepsilon}^+$ là hình hộp $[-2r,2r]\times [\varepsilon ,2r]$ trong $\mathbf{C}$. Nó là một tập con đa diện địa phương của $\mathbf{C}$ (VAR, R2, 11.3, p. 48). Nó thỏa mãn các điều kiện sau:

(i) Ta có $R^+_{\varepsilon}\subset 2C\cap F^+_{\varepsilon}$;

(ii) Tập hợp $R^+_{\varepsilon}$ chứa giao của $F^+_{\varepsilon}$ và giá của $h$;

(iii) Biên chính quy $\partial R^+_{\varepsilon}$ (VAR, R2, 11.3.2, p. 49) chứa đoạn $S_{\varepsilon}= [-r, r] +i\varepsilon \subset \mathbf{C}$;

(iv) Ta có $h(\lambda ) = 0$ nếu $\lambda \in \partial R_{\varepsilon}^+-S_{\varepsilon}$.

Gọi $d\lambda$ (tương ứng $d\lambda$ ) là dạng vi phân 1 trên $\mathbf{C}$ là vi phân của ánh xạ đồng nhất của $\mathbf{C}$ (tương ứng của phép liên hợp phức). Gọi $g$ là hàm trên $\mathbf{C}-\mathbf{R}$ nhận giá trị trong $\mathscr{L}(E)$ sao cho $g(\lambda ) =\widetilde{f}(\lambda )R(u, \lambda )$ với $\lambda \in \mathbf{C}-\mathbf{R}$. Đặt $\omega =g d\lambda$; nó là một dạng vi phân 1 trên $\mathbf{C}-\mathbf{R}$, có giá compact và nhận giá trị trong $\mathscr{L}(E)$. Vì giải thức của $u$ là chỉnh hình (Mệnh đề 14 của IV, p. 246), ta có

$$
d\omega =(\frac{\partial\widetilde{f}}{\partial z}(\lambda )R(u, \lambda ) +\widetilde{f}(\lambda )\frac{\partial}{\partial z}R(u, \lambda ))d\lambda \wedge d\lambda =-h(\lambda )d\lambda \wedge d\lambda
$$

Đo vectơ liên kết với $d\omega$ (VAR, R2, 10.4.3, p. 43) là đo có mật độ $-2ih$ đối với đo Lebesgue. Áp dụng công thức Stokes cho tập con đa diện địa phương $R_{\varepsilon}^+$ và cho dạng vi phân $\omega$ (VAR, R2, 11.3.4, p. 49), do đó ta thu được

$$
\frac{i}{2}\int_{R^+_{\varepsilon}}d\omega =\frac{i}{2}\int_{\partial R^+_{\varepsilon}}\omega =\frac{i}{2}\int_{S_{\varepsilon}}\omega =\frac{i}{2}\int_{-r}^r\widetilde{f}(y+i\varepsilon )R(u, y+i\varepsilon )dy
$$

do đó

$$
\int_{F^+_{\varepsilon}}h(\lambda )d\mu(\lambda ) =-\frac{i}{2}\int_{\mathbf{R}}\widetilde{f}(y+i\varepsilon )R(u, y+i\varepsilon )dy
$$

Lập luận tương tự đối với $F^-_{\varepsilon}$, ta thu được

$$
\int_{F^-_{\varepsilon}}h(\lambda )d\mu(\lambda ) =-\frac{i}{2}\int_{\mathbf{R}}\widetilde{f}(y-i\varepsilon )R(u, y-i\varepsilon )dy
$$

và ta kết luận rằng tích phân của $h$ trên $\mathbf{C}$ là giới hạn khi $\varepsilon \rightarrow 0$ của

$$
v_{\varepsilon}=\frac{i}{2}\int_{\mathbf{R}}(\widetilde{f}(y+i\varepsilon )R(u, y+i\varepsilon )-\widetilde{f}(y-i\varepsilon )R(u, y-i\varepsilon ))dy
$$

Theo Mệnh đề 7, ta có $v_{\varepsilon}=\pi f_{\varepsilon}(u)$, trong đó $f_{\varepsilon}$ là hàm xác định trên $\mathbf{R}$ bởi

$$
f_{\varepsilon}(x) =-\frac{1}{2i\pi}\int_{\mathbf{R}}(\frac{\widetilde{f}(y + i\varepsilon)}{y-x + i\varepsilon}-\frac{\widetilde{f}(y-i\varepsilon)}{y-x-i\varepsilon})dy
$$

Khi $f_{\varepsilon}\rightarrow f$ khi $\varepsilon \rightarrow 0$ trong $\mathscr{C}_b(\mathbf{R})$ (Bổ đề 7), tự đồng cấu $v_{\varepsilon}=\pi f_{\varepsilon}(u)$ hội tụ đến $\pi f(u)$ trong $\mathscr{L}(E)$ (Mệnh đề 5 của IV, p. 275). Định lý được chứng minh.

### 6. Các tôpô giải thức và tính liên tục của phép tính phiếm hàm

Trong No. này, E ký hiệu một không gian Hilbert phức. Nhắc lại rằng $\mathscr{A}(E)$ ký hiệu tập hợp các toán tử từng phần tự liên hợp trên E. Ta sẽ mở rộng sang $\mathscr{A}(E)$ các tính chất liên tục của No. 8 của IV, p. 194.

#### Định nghĩa 6 {#ts-iv-s5-def-6 .statement tag=036B}

Cho $\mathscr{T}$ là một tôpô lồi địa phương trên $\mathscr{L}(E)$. Tôpô giải thức $\mathscr{T}$ trên $\mathscr{A}(E)$ là tôpô mịn nhất sao cho các ánh xạ $u\mapsto R(u, \lambda )$ từ $\mathscr{A}(E)$ vào $\mathscr{L}(E)$ được trang bị tôpô $\mathscr{T}$ là liên tục với mọi $\lambda \in \mathbf{C}-\mathbf{R}$.

#### Mệnh đề 11 {#ts-iv-s5-prop-11 .statement tag=036C}

Cho $\mathscr{T}$ là một tôpô lồi địa phương trên $\mathscr{L}(E)$ kém mịn hơn tôpô không gian Banach của $\mathscr{L}(E)$.

a) Cho $f\in \mathscr{C}_0(\mathbf{R})$. Với mọi dãy $(u_n)_{n\in\mathbf{N}}$ trong $\mathscr{A}(E)$ hội tụ đến $u$ đối với tôpô giải thức $\mathscr{T}$, dãy $(f(u_n))_{n\in\mathbf{N}}$ hội tụ đến $f(u)$ trong không gian $\mathscr{L}(E)$ được trang bị tôpô $\mathscr{T}$;

b) Giả sử rằng mọi $u\in \mathscr{A}(E)$ thừa nhận một hệ cơ bản đếm được các lân cận đối với tôpô giải thức $\mathscr{T}$. Ánh xạ từ $\mathscr{C}_0(\mathbf{R})\times \mathscr{A}(E)$ vào không gian $\mathscr{L}(E)$ được trang bị tôpô $\mathscr{T}$ xác định bởi $(f, u)\mapsto f(u)$ là liên tục.

Ta hãy chứng minh a). Tôpô $\mathscr{T}$ trên $\mathscr{L}(E)$ là cực đại của các tôpô được xác định bởi các nửa chuẩn liên tục đối với tôpô $\mathscr{T}$ (EVT, II, p. 26, Hệ quả và nhận xét sau đó). Vì vậy chỉ cần chứng minh rằng với mọi nửa chuẩn $p$ trên $\mathscr{L}(E)$ liên tục đối với tôpô $\mathscr{T}$, dãy $p(f(u_n)-f(u))$ hội tụ đến 0 (TG, I, p. 51, Mệnh đề 10).

Cho $p$ là một nửa chuẩn như vậy. Gọi $\mathscr{L}(E)_p$ là không gian Banach tách được hoàn thành của không gian $\mathscr{L}(E)$ được trang bị nửa chuẩn $p$, và gọi $\varpi$ là ánh xạ chính tắc từ $\mathscr{L}(E)$ vào $\mathscr{L}(E)_p$; ánh xạ này liên tục, và ta có $p(u) =\|\varpi (u)\|_p$ với mọi $u\in \mathscr{L}$ (E), trong đó chuẩn là chuẩn của không gian $\mathscr{L}(E)_p$.

Vì $\mathscr{T}$ kém mịn hơn tôpô không gian Banach của $\mathscr{L}$ (E), tồn tại $c\geqslant 0$ sao cho $p(u)\leqslant c\|u\|$ với mọi $u\in \mathscr{L}(E)$.

Giả sử trước hết rằng $f\in \mathscr{D}(\mathbf{R})$. Gọi $\widetilde{f}$ là một mở rộng giải tích gần đúng của $f$. Ta ký hiệu bởi $\mu$ độ đo Lebesgue trên $\mathbf{C}$. Theo công thức Helffer–Sjöstrand (Định lý 2 của IV, p. 284), ta có

$$
\varpi (f(u_n)) =-\frac{1}{\pi}\int_{\mathbf{C}}\frac{\partial\widetilde{f}}{\partial z}(\lambda )\varpi (R(u_n, \lambda ))d\mu(\lambda ) \tag{14}
$$

với mọi $n\in \mathbf{N}$.

Cho $\lambda \in \mathbf{C}-\mathbf{R}$. Theo giả thiết, dãy các giải thức $R(u_n, \lambda )$ hội tụ đến $R(u, \lambda )$ trong $\mathscr{L}(E)$ được trang bị tôpô $\mathscr{T}$, do đó dãy $(\varpi (R(u_n, \lambda )))_n$ hội tụ đến $\varpi (R(u, \lambda ))$ trong không gian Banach $\mathscr{L}(E)_p$.

Với mọi $n\in \mathbf{N}$, ta có

$$
\|\frac{\partial\widetilde{f}}{\partial z}(\lambda )R(u_n, \lambda )\|\leqslant |\frac{1}{\mathscr{I} (\lambda)}\frac{\partial\widetilde{f}}{\partial z}(\lambda )|
$$

(Mệnh đề 17 của IV, p. 248), do đó

$$
\|\frac{\partial\widetilde{f}}{\partial z}(\lambda )\varpi (R(u_n, \lambda ))\|_p\leqslant c|\frac{1}{\mathscr{I} (\lambda)}\frac{\partial\widetilde{f}}{\partial z}(\lambda )|
$$

Đánh giá (13) của IV, p. 281 cho thấy vế phải của bất đẳng thức này là một hàm bị chặn với $\lambda \in \mathbf{C}-\mathbf{R}$; nó khả tích trên $\mathbf{C}$ vì $\widetilde{f}$ có giá compact. Từ định lý Lebesgue (INT, IV, p. 137, § 3, n$^o7$, Định lý 6) và từ công thức Helffer–Sjöstrand áp dụng cho $f$, suy ra rằng $\varpi (f(u_n))$ hội tụ đến $\varpi (f(u))$, do đó $p(f(u_n)-f(u))$ tiến tới 0.

Bây giờ giả sử rằng $f\in \mathscr{C}_0(\mathbf{R})$. Cho $\varepsilon  >0$. Tồn tại một hàm $f_{\varepsilon}$ trong $\mathscr{D}(\mathbf{R})$ sao cho $\|f_{\varepsilon}-f\|_{\infty}\leqslant \varepsilon ($cf. Mệnh đề 4, a) của IV, p. 202 và INT, III, p. 45, § 1, n$^o2$, Mệnh đề 3). Theo Mệnh đề 5, c) của IV, p. 275, khi đó ta có $\|f(u)-f_{\varepsilon}(u)\|\leqslant \varepsilon$ và $\|f(u_n)-f_{\varepsilon}(u_n)\|\leqslant \varepsilon$ với mọi $n\in \mathbf{N}$. Do đó, ta thu được

$$
p(f(u_n)-f(u))\leqslant 2c\varepsilon +p(f_{\varepsilon}(u_n)-f_{\varepsilon}(u))
$$

với mọi $n\in \mathbf{N}$. Vì $f_{\varepsilon}\in \mathscr{D}(\mathbf{R})$, dãy $(p(f_{\varepsilon}(u_n)-f_{\varepsilon}(u)))_{n\in\mathbf{N}}$ hội tụ đến 0 theo trường hợp trước, và do đó $p(f(u_n)-f(u))$ hội tụ đến 0. Điều này hoàn tất chứng minh a).

Ta chứng minh mệnh đề b). Dưới giả thiết liên quan đến $\mathscr{T}$, từ TG, IX, p. 17, Mệnh đề 10 và nhận xét sau đó, và từ mệnh đề a), suy ra rằng ánh xạ $u\mapsto f(u)$ từ $\mathscr{A}(E)$ vào $\mathscr{L}(E)$ là liên tục khi $f\in \mathscr{C}_0(\mathbf{R})$. Vì các ánh xạ $f\mapsto f(u)$ từ $\mathscr{C}_0(\mathbf{R})$ vào $\mathscr{L}(E)$ là liên tục với chuẩn $\leqslant 1$ đối với mọi $u\in \mathscr{A}(E)$ (Mệnh đề 5, c) của IV, p. 275), mệnh đề b) suy ra từ TG, X, p. 13, Hệ quả 3.

#### Ví dụ 1 {#ts-iv-s5-n6-exa-1 .statement tag=036D}

Cho $\mathfrak{S}$ là một tập hợp các phần bị chặn của E. Tôpô $\mathfrak{S}$ trên $\mathscr{L}(E)$ (EVT, III, p. 13) là một tôpô lồi địa phương ít tinh hơn tôpô không gian Banach của $\mathscr{L}(E)$.

#### Ví dụ 2 {#ts-iv-s5-n6-exa-2 .statement tag=036E}

Cho $\mathscr{T}_b$ là tôpô không gian Banach của $\mathscr{L}(E)$. Đối với tôpô giải thức $\mathscr{T}_b$, mọi $u\in \mathscr{A}(E)$ đều có một hệ cơ bản đếm được các lân cận.

Thực vậy, chỉ cần chứng minh rằng với mọi $\lambda \in$ **C-R** và mọi $\varepsilon  >0$, tồn tại $\lambda '\in \mathbf{Q}+i\mathbf{Q}^*$ và một số nguyên $n\geqslant 1$ sao cho mọi toán tử từng phần $v\in \mathscr{A}(E)$ thỏa mãn $\|R(v, \lambda ')-R(u, \lambda ')\|<1/n$ cũng thỏa mãn điều kiện $\|R(v, \lambda )-R(u, \lambda )\|< \varepsilon$; viết

$$
\|R(v, \lambda )-R(u, \lambda )\|\leqslant \|R(v, \lambda )-R(v, \lambda ')\|
$$

$$
+\|R(v, \lambda ')-R(u, \lambda ')\|+\|R(u, \lambda ')-R(u, \lambda )\|
$$

tính chất này suy ra từ công thức (8) của IV, p. 245, từ các ước lượng của mệnh đề 17 của IV, p. 248, và từ sự kiện rằng $\mathbf{Q}+i\mathbf{Q}^*$ là trù mật khắp nơi trong $\mathbf{C}-\mathbf{R}$.

Kết luận của mệnh đề không đúng nói chung nếu $\mathscr{C}_0(\mathbf{R})$ được thay bởi $\mathscr{C}_b(\mathbf{R})$ (bài tập 29 của IV, p. 366, e)). Tuy nhiên, ta có kết quả sau.

#### Hệ quả {#ts-iv-s5-n6-cor-1 .statement tag=036F}

Gọi $\mathscr{T}_s$ là tôpô hội tụ đơn giản trên $\mathscr{L}(E)$. Cho $f\in \mathscr{C}_b(\mathbf{R})$. Với mọi dãy $(u_n)_{n\in\mathbf{N}}$ trong $\mathscr{A}(E)$ hội tụ về $u$ đối với tôpô giải thức $\mathscr{T}_s$, dãy $(f(u_n))_{n\in\mathbf{N}}$ hội tụ về $f(u)$ trong $\mathscr{L}(E)$ được trang bị tôpô $\mathscr{T}_s$.

Cho $(u_n)$ là một dãy trong $\mathscr{A}(E)$ hội tụ về $u$ đối với tôpô giải thức $\mathscr{T}_s$. Cho $x\in E$ và cho $\varepsilon  >0$.

Với mỗi số nguyên $N\in \mathbf{N}$, cho $\varphi_N\in \mathscr{K}(\mathbf{R})$ là một hàm có giá đỡ được chứa trong $[-(N + 1),N + 1]$ sao cho $0\leqslant \varphi_N\leqslant 1$ và $\varphi_N(t) = 1$ với mọi $t\in [-N,N]$. Các hàm $\varphi_N$ hội tụ đơn giản về 1 khi N tiến tới vô hạn, và thỏa mãn $|\varphi_N|\leqslant 1$, do đó mệnh đề 6 của IV, p. 276 suy ra rằng tồn tại $N\in \mathbf{N}$ sao cho $\|\varphi_N(u)x-x\|\leqslant \varepsilon$. Đặt $f_N=f \varphi_N$.

Với mọi $n\in \mathbf{N}$, ta có

$$
\|f(u_n)x-f(u)x\|\leqslant \|f(u_n)x-f_N(u_n)x\|+ \tag{15}
$$

$$
\|f_N(u_n)x-f_N(u)x\|+\|f_N(u)x-f(u)x\|
$$

Với mọi $v\in \mathscr{A}$ (E), ta có

$$
\|f(v)x-f_N(v)x\|=\|(f(1-\varphi_N))(v)x\|
$$

$$
\leqslant \|f(v)\| \|x-\varphi_N(v)x\|\leqslant \|f\|_{\infty}\|x-\varphi_N(v)x\|
$$

(mệnh đề 5, c) của IV, p. 275). Vì $\varphi_N\in \mathscr{C}_0(\mathbf{R})$, mệnh đề a) của mệnh đề 11 áp dụng cho tôpô giải thức $\mathscr{T}_s$ suy ra rằng $\varphi_N(u_n)x$ hội tụ về $\varphi_N(u)x$ khi $n\rightarrow +\infty$. Do đó, với mọi $n$ đủ lớn, ta có

$$
\|x-\varphi_N(u_n)x\|\leqslant \|x-\varphi_N(u)x\|+\varepsilon \|x\|\leqslant (1 +\|x\|)\varepsilon
$$

Bất đẳng thức (15) khi đó trở thành

$$
\|f(u_n)x-f(u)x\|\leqslant \|f\|_{\infty}(2 +\|x\|)\varepsilon +\|f_N(u_n)x-f_N(u)x\|
$$

với mọi $n$ đủ lớn. Chứng minh được kết thúc nhờ mệnh đề a) của tài liệu đã dẫn, áp dụng cho hàm $f_N\in \mathscr{C}_0(\mathbf{R})$ và cho tôpô giải thức $\mathscr{T}_s$.

### 7. Phân tích cực

#### Bổ đề 8 {#ts-iv-s5-lem-8 .statement tag=036G}

Cho E là một không gian vectơ tôpô tách. Cho $(E_1,\|\cdot \|_1)$ và $(E_2,\|\cdot \|_2)$ là các không gian con trù mật của E được trang bị các cấu trúc không gian Hilbert sao cho các phép nhúng chính tắc của $E_1$ và $E_2$ vào E là liên tục. Cho F là một không gian con của $E_1\cap E_2$, trù mật trong $E_1$ và $E_2$ đối với các cấu trúc không gian Hilbert này. Nếu $\|x\|_1=\|x\|_2$ với mọi $x\in F$, thì $E_1= E_2$ và $\|\cdot \|_1=\|\cdot \|_2$.

Cho $x\in E_1$. Tồn tại một dãy $(x_n)_{n\in\mathbf{N}}$ trong F sao cho $x_n$ hội tụ đến $x$ trong không gian Hilbert $E_1$. Vì $\|x_n-x_m\|_2=\|x_n-x_m\|_1$ với mọi số nguyên $n$ và $m$, dãy $(x_n)$ là một dãy Cauchy trong $E_2$. Gọi $y$ là giới hạn của nó. Ta có $\|y\|_2=$ lim$\|x_n\|_2=\|x\|_1$. Vì các phép nhúng chính tắc của $E_1$ và $E_2$ vào E là liên tục, ta có $x_n\rightarrow x$ trong E và tương tự $x_n\rightarrow y$ trong E. Do đó suy ra rằng $x=y$ và $\|x\|_1=\|x\|_2$; đặc biệt, $E_1\subset E_2$. Ta kết luận bằng tính đối xứng.

Cho E là một không gian Hilbert phức. Cho $u$ là một toán tử bộ phận tự liên hợp dương trên E. Với mọi $\alpha \in \mathbf{R}_+$, ta đặt $u^{\alpha}=f(u)$, trong đó $f$ là ánh xạ liên tục $x\mapsto x^{\alpha}$ của $\mathbf{R}_+$ vào $\mathbf{R}$. Đây là một toán tử bộ phận tự liên hợp dương (Cor. 1, a) của IV, p. 273). Khi $u\in \mathscr{L}$ (E), ký hiệu này tương thích với ký hiệu liên quan đến đại số có đối hợp $\mathscr{L}(E) ($cf. Prop. 16 của I, p. 118). Nếu $\alpha$ là một số nguyên dương, toán tử bộ phận $u^{\alpha}$ trùng với toán tử bộ phận được xác định bởi hợp thành $u\circ  \cdots  \circ u$ (Cor. 1, b) của IV, p. 273).

Cho $\beta \in \mathbf{R}_+$. Ta có $u^{\alpha \beta}= (u^{\alpha})^{\beta}$ (Cor. 4 của IV, p. 274). Đặc biệt, nếu $\alpha  >0$, thì toán tử bộ phận $u^{1/\alpha}$ là toán tử bộ phận tự liên hợp dương duy nhất $v$ trên E sao cho $v^{\alpha}=u$.

Giả sử rằng $0\leqslant \alpha \leqslant \beta$. Khi đó dom($u^{\beta}$)$\subset$ dom($u^{\alpha}$) $:$ thực vậy, với mọi số thực $x\geqslant 0$, ta có $x^{\alpha}\leqslant 1 +x^{\beta}$, và kết quả khi đó suy ra từ định nghĩa của miền xác định của $u^{\alpha}($cf. Prop. 3 của IV, p. 271).

Cho $u$ là một toán tử đóng với miền xác định trù mật từ E vào một không gian Hilbert phức F. Toán tử bộ phận $u^*u$ là tự liên hợp và dương (Prop. 12 của IV, p. 241). Ta viết $|u|= (u^*u)^{1/2}$.

#### Mệnh đề 12 {#ts-iv-s5-prop-12 .statement tag=036H}

Cho $u$ là một toán tử đóng có miền xác định trù mật từ E vào một không gian Hilbert phức F.

a) Miền xác định của toán tử từng phần tự liên hợp dương $|u|$ trùng với miền xác định của $u$;

b) Tồn tại một ánh xạ tuyến tính đẳng cự từng phần duy nhất $j$ từ E vào F sao cho $u=j|u|$ và Ker($j$) $=$ Ker($u$);

c) Cho $u_1$ là một toán tử tự liên hợp dương trên E và $j_1$ là một ánh xạ tuyến tính đẳng cự từng phần từ E vào F sao cho $u=j_1u_1$ và Ker($j_1$) $=$ Ker($u_1$). Khi đó $u_1=|u|$ và $j_1=j$.

Miền xác định của $u^*u$ được chứa trong dom($u$) và trong dom($|u|$). Nó trù mật trong các không gian Hilbert $E_u($loc. cit.) và $E_{|u|}$ (Hệ quả 1, e) của IV, p. 273) và, với mọi $x\in$ dom($u^*u$), ta có

$$
\|x\|^2_u=\|x\|^2+\langle u(x)|u(x)\rangle =\|x\|^2+\langle x|(u^*u)(x)\rangle \tag{16}
$$

$$
=\|x\|^2+\langle |u|(x)| |u|(x)\rangle =\|x\|^2_{|u|}
$$

Do đó, các không gian Hilbert $E_u$ và $E_{|u|}$ là bằng nhau (Bổ đề 8), suy ra dom($u$) $=$ dom($|u|$) và $\|u(x)\|$ = $\||u|(x)\|$ với mọi $x\in$ dom($u$).

Công thức (16) suy ra rằng Ker($u$) $=$ Ker($|u|$) và tồn tại một ánh xạ tuyến tính đẳng cự duy nhất $v$ từ Im($|u|$) lên Im($u$) thỏa mãn $v(|u|(x)) =u(x)$ với mọi $x\in$ dom($|u|$). Vì $|u|$ là tự liên hợp, ta có Im($|u|$)$^{\circ}=$ Ker($|u|$) (Mệnh đề 7, c) của IV, p. 236). Do đó tồn tại một phép đẳng cự từng phần duy nhất $j$ từ E vào F mở rộng $v$ và triệt tiêu trên Ker($|u|$) $=$ Ker($u$). Vì E = Ker($u$)$\oplus$ Im($|u|$), ánh xạ này là ánh xạ tuyến tính đẳng cự từng phần duy nhất sao cho $u=j|u|$ và Ker($j$) $=$ Ker($u$).

Ta hãy chứng minh c). Ta có $u_1j_1^*j_1u_1\subset (j_1u_1)^*j_1u_1=u^*u$. Ánh xạ tuyến tính $j_1^*j_1$ là phép chiếu trực giao có hạt nhân Ker($j_1$) $=$ Ker($u_1$) (TVS, V, p. 41, Mệnh đề 5 (ii)) và do đó có ảnh Ker($u_1$)$^{\circ}=$ Im($u_1$) (Mệnh đề 7, c) của IV, p. 236). Do đó, $u^2_1\subset u^*u$, suy ra $u^2_1=u^*u$ vì hai toán tử này là tự liên hợp. Vì vậy, suy ra $u_1= (u^*u)^{1/2}$, và mệnh đề về tính duy nhất trong b) cuối cùng chứng minh rằng $j_1=j$.

#### Định nghĩa 7 {#ts-iv-s5-def-7 .statement tag=036I}

Cho $u$ là một toán tử đóng có miền xác định trù mật từ E vào một không gian Hilbert phức F. Cặp $(j,|u|)$ được xác định bởi Mệnh đề 12 được gọi là phân tích cực của $u$.

Giả sử rằng $u\in \mathscr{L}(E; F)$. Phân tích cực của nó theo nghĩa của định nghĩa này trùng với phân tích cực của Định nghĩa 4 của I, p. 140.

### 8. Các toán tử tự liên hợp được xác định bởi một dạng Hermit bộ phận dương

Trong Số này, E ký hiệu một không gian Hilbert phức.

#### Định nghĩa 8 {#ts-iv-s5-def-8 .statement tag=036J}

Cho D là một không gian con vectơ của E. Một dạng Hermit bộ phận trên E có miền xác định D là một sự tương ứng $q= (\Gamma ,E\times E,\mathbf{C})$ có miền xác định là $D\times D$, có đồ thị Γ là phiếm hàm, và sao cho ánh xạ từ $D\times D$ vào $\mathbf{C}$ được xác định bởi Γ là một dạng Hermit. Ta viết dom($q$) $= D$.

Ta nói rằng $q$ là một dạng bộ phận dương nếu dạng Hermit mà nó xác định là dương.

Cho $u$ là một toán tử bộ phận tự liên hợp trên E. Với mọi phần tử $x$ và $y$ của E, ta ký hiệu bởi $\mu_{x,y}$ (tương ứng $\mu_x$) độ đo phổ của $(x, y)$ (tương ứng của $x$) đối với $u$.

Cho $(j,|u|)$ là phân tích cực của $u$ (Định nghĩa 7 của IV, p. 290). Ta ký hiệu bởi $D'$ miền xác định của $|u|^{1/2}$. Theo định nghĩa, đây là không gian của các $x\in E$ sao cho hàm $z\mapsto  |z|$ khả tích trên Sp($u$) đối với độ đo $\mu_x$. Nó chứa dom($u$).

Cho $(x, y)\in D'\times D'$. Hàm đồng nhất trên Sp($u$) là khả tích đối với độ đo $\mu_{x,y}$ (Mệnh đề 4, b) của IV, p. 271); ta đặt

$$
q_u(x, y) =\int t d\mu_{x,y}(t)
$$

Sp($u$)

Nếu $y\in$ dom($u$), ta có $q_u(x, y) =\langle x|u(y)\rangle$ theo công thức (6) của IV, p. 271. Ánh xạ $q_u$ là một dạng Hermit trên $D'$. Nó xác định một dạng Hermit bộ phận trên E, được gọi là liên kết với $u$. Nếu toán tử $u$ là dương, thì dạng $q_u$ là một dạng Hermit bộ phận dương.

#### Định nghĩa 9 {#ts-iv-s5-def-9 .statement tag=036K}

Cho $q$ là một dạng Hermit bộ phận dương trên E. Ta ký hiệu bởi $E_q$ không gian tiền Hilbert phân ly dom($q$) được trang bị tích vô hướng

$$
(x|y)_q=\langle x|y\rangle +q(x, y)
$$

Ta ký hiệu bằng $\|x\|_q$ chuẩn của $x\in E_q$. Ta nói rằng dạng $q$ là đóng nếu $E_q$ là một không gian Hilbert.

#### Mệnh đề 13 {#ts-iv-s5-prop-13 .statement tag=036L}

Cho $u$ là một toán tử từng phần tự liên hợp dương trên E. Cho $q_u$ là dạng từng phần dương liên kết.

a) Miền của $q_u$ là miền của $u^{1/2}$, và với mọi $x$ và $y$ trong dom($u^{1/2}$), ta có $q_u(x, y) =\langle u^{1/2}(x)|u^{1/2}(y)\rangle$;

b) Dạng từng phần dương $q_u$ là đóng. Miền của $u$ là một lõi của $q_u$.

Vì $u$ là dương, ta có $|u|=u$. Miền dom($|u|^{1/2}$) của $q_u$ do đó trùng với dom($u^{1/2}$), và ta có

$$
q_u(x, y) =\int t d\mu_{x,y}(t) =\int t^{1/2}\cdot t^{1/2}d\mu_{x,y}(t)
$$

Sp($u$) Sp($u$)

$$
=\langle u^{1/2}(x)|u^{1/2}(y)\rangle
$$

với $x$ và $y$ trong dom($q_u$) (mđề. 4, b) của IV, p. 271). Điều này chứng minh mệnh đề a).

Hơn nữa, không gian tiền Hilbert $E_{q_u}$ khi đó trùng với không gian tiền Hilbert $E_{u^{1/2}}$ liên kết với $u^{1/2}$ (đn. 4 của IV, p. 230). Vì $u^{1/2}$ là một toán tử từng phần đóng, không gian này là một không gian Hilbert (mđề. 4 của IV, p. 230) và dom($u$) trù mật trong $E_{u^{1/2}}$ theo mệnh đề e) của hệ quả 1 của IV, p. 273.

Cho $q$ là một dạng Hermit từng phần trên E với miền D trù mật trong E. Với $y\in D$, ta ký hiệu bằng $\lambda_y$ dạng tuyến tính $x\mapsto q(y, x)$ trên D. Ta ký hiệu bằng $\widetilde{D}$ tập hợp các $y\in D$ sao cho dạng tuyến tính $\lambda_y$ liên tục trên D.

Cho $y\in \widetilde{D}$. Vì D trù mật trong E, tồn tại một dạng tuyến tính liên tục duy nhất trên E mở rộng $\lambda_y$. Ta lại ký hiệu nó bằng $\lambda_y$. Tồn tại một phần tử duy nhất $u(y)$ trong E sao cho $\lambda_y(x) =\langle u(y)|x\rangle$ với mọi $x\in E$ (EVT, V, p. 15, đl. 3). Ánh xạ $y\mapsto u(y)$ là tuyến tính từ $\widetilde{D}$ vào E; toán tử từng phần $u$ trên E với miền $\widetilde{D}$ được gọi là toán tử từng phần biểu diễn $q$. Do đó ta có

$$
q(x, y) =\langle x|u(y)\rangle
$$

với $y\in$ dom($u$) và $x\in D$.

#### Nhận xét {#ts-iv-s5-n8-rem-1 .statement tag=036M}

Cho $q$ là một dạng bộ phận dương đóng và $q'$ là một dạng Hermit dương liên tục trên E. Dạng Hermit dương được xác định trên dom($q$) bởi $(x, y)\mapsto q(x, y) +q'(x, y)$ là một dạng Hermit dương bộ phận đóng có cùng miền với $q$. Nó được ký hiệu bởi $q+q'$.

Theo EVT, V, p. 16, Hệ quả 2, tồn tại một ánh xạ tuyến tính duy nhất $u'\in \mathscr{L}(E)$ sao cho $q'(x, y) =\langle x|u'(y)\rangle$ với mọi $(x, y)\in E\times E$. Tự đồng cấu $u'$ là dương và toán tử bộ phận biểu diễn dạng Hermit dương bộ phận đóng $q+q'$ là $u+u'$.

#### Mệnh đề 14 {#ts-iv-s5-prop-14 .statement tag=036N}

Cho $q$ là một dạng bộ phận dương đóng có miền trù mật trên E và $u$ là toán tử bộ phận biểu diễn $q$.

a) Miền của $u$ là trù mật trong không gian Hilbert $E_q$;

b) Toán tử bộ phận $u$ là tự liên hợp và dương.

Vì $q$ đóng, không gian tiền Hilbert $E_q$ của Định nghĩa 9 là một không gian Hilbert.

Hãy chứng minh rằng toán tử bộ phận $u+ 1_E$ với miền dom($u$) là song ánh. Vì

$$
\langle x|(u+ 1_E)(x)\rangle =q(x, x) +\|x\|^2\geqslant \|x\|^2
$$

với mọi $x\in$ dom($u$), toán tử bộ phận này là đơn ánh.

Cho $y\in E$. Dạng tuyến tính trên $E_q$ xác định bởi $x\mapsto  \langle y|x\rangle$ là liên tục vì $\|x\|\leqslant \|x\|_q$. Do đó tồn tại $y'\in E_q$ sao cho

$$
\langle y|x\rangle = (y'|x)_q=\langle y'|x\rangle +q(y', x)
$$

với mọi $x\in E_q$ (EVT, V, p. 15, Định lý 3). Theo định nghĩa, điều này có nghĩa là $y'$ thuộc miền của toán tử bộ phận $\widetilde{u}$ biểu diễn dạng bộ phận $(x, y)\mapsto (x|y)_q$ với miền dom($q$), và $\widetilde{u}(y') =y$. Vì $\widetilde{u}=u+ 1_E$ theo nhận xét trên, suy ra toán tử bộ phận $u+ 1_E$ cũng là toàn ánh, do đó song ánh.

Hãy chứng minh rằng miền của $u$ là trù mật trong $E_q$. Cho $y\in E_q$ vuông góc với dom($u$) trong $E_q$. Tồn tại $y'\in$ dom($u$) sao cho $u(y')+y'=y$. Khi đó ta có

$$
0 = (y|y')_q=\langle y|y'\rangle +q(y, y') =\langle y|y'+u(y')\rangle =\|y\|^2
$$

do đó $y= 0$. Mệnh đề a) vì thế được chứng minh.

Vì dom($q$) trù mật trong E và $\|x\|\leqslant \|x\|_q$ với mọi $x\in$ dom($q$), mệnh đề a) suy ra rằng dom($u$) trù mật trong E. Vì dạng $q$ là Hermit (tương ứng dương), với mọi $x$ và $y$ trong dom($u$), ta có

$$
\langle y|u(x)\rangle =q(y, x) =q(x, y) =\overline{\langle x|u(y)\rangle}=\langle u(y)|x\rangle
$$

(resp. $\langle x|u(x)\rangle =q(x, x)\geqslant 0$), sao cho $u$ là đối xứng (tương ứng, dương). Cuối cùng, toán tử riêng phần $u+ 1_E$ là tự liên hợp theo hệ quả của mệnh đề 10 của IV, p. 240, và điều tương tự cũng đúng đối với $u$.

#### Định lý 3 {#ts-iv-s5-thm-3 .statement tag=036O}

Ánh xạ liên kết với một toán tử tự liên hợp dương $u$ trên E dạng riêng phần dương $q_u$ là một song ánh giữa tập hợp các toán tử riêng phần tự liên hợp dương trên E và tập hợp các dạng riêng phần dương đóng với miền xác định trù mật trên E. Song ánh ngược liên kết với một dạng riêng phần dương $q$ toán tử riêng phần biểu diễn $q$.

Theo mệnh đề 13, b) và 14, b), các ánh xạ được mô tả trong mệnh đề là xác định tốt. Ta hãy chứng minh rằng chúng là các song ánh ngược của nhau.

Cho $u$ là một toán tử riêng phần tự liên hợp dương trên E và $q$ là dạng riêng phần dương liên kết với $u$. Gọi $v$ là toán tử tự liên hợp dương biểu diễn $q$. Cho $y\in$ dom($u$)$\subset$ dom($u^{1/2}$) $=$ dom($q$). Với mọi $x\in$ dom($q$) $=$ dom($u^{1/2}$), ta có

$$
q(y, x) =\langle u^{1/2}(y)|u^{1/2}(x)\rangle =\langle u(y)|x\rangle
$$

do đó $y$ thuộc miền xác định của $v$ và thỏa mãn $v(y) =u(y)$. Toán tử riêng phần $v$ vì vậy là một mở rộng của $u$; vì $u$ và $v$ là tự liên hợp, chúng bằng nhau.

Ngược lại, cho $q$ là một dạng riêng phần dương đóng với miền xác định trù mật và $u$ là toán tử riêng phần tự liên hợp dương biểu diễn $q$. Ta có dom($u$)$\subset$ dom($u^{1/2}$). Với $x$ và $y$ trong dom($u$), ta có

$$
q_u(x, y) =\langle u^{1/2}(x)|u^{1/2}(y)\rangle =\langle x|u(y)\rangle =q(x, y)
$$

theo mệnh đề 13, a). Như vậy, các không gian Hilbert $E_q$ và $E_{q_u}$ đều chứa dom($u$) như một không gian con trù mật (mệnh đề 14, a) và mệnh đề 13, b), tương ứng) và $\|x\|_q=\|x\|_{q_u}$ với mọi $x\in$ dom($u$). Suy ra rằng $E_q= E_{q_u}$ và $q=q_u$ (bổ đề 8).

#### Hệ quả {#ts-iv-s5-n8-cor-1 .statement tag=036P}

Cho $q$ là một dạng riêng phần dương đóng trên E và $u$ là toán tử tự liên hợp dương biểu diễn $q$. Miền xác định của $q$ bằng miền xác định của $(1_E+u)^{1/2}$, và ta có

$$
\|x\|_q=\|(1_E+u)^{1/2}x\|
$$

với mọi $x\in$ dom($q$).

Miền của $q$ bằng miền của $u^{1/2}$ (Mệnh đề 13, a)), miền này trùng với miền của $(1_E+u)^{1/2}($cf. Mệnh đề 3 của IV, p. 271). Với mọi $x\in$ dom($u$)$\subset$ dom($u^{1/2}$), ta có

$$
\|(1_E+u)^{1/2}x\|^2=\langle x|(1_E+u)(x)\rangle =\|x\|^2+\langle x|u(x)\rangle =\|x\|^2_q
$$

Vì miền của $u$ trù mật trong không gian Hilbert $E_q$ (Mệnh đề 14, a)), công thức này mở rộng theo tính liên tục tới mọi $x\in$ dom($u^{1/2}$).

#### Ví dụ {#ts-iv-s5-n8-exa-1 .statement tag=036Q}

Cho $u$ là một toán tử từng phần dương trên E, không nhất thiết đóng. Ta định nghĩa một dạng từng phần dương $q$ có miền dom($u$) bởi

$$
q(x, y) =\langle x|u(y)\rangle
$$

với $x$ và $y$ thuộc dom($u$). Gọi $E_q$ là không gian tiền-Hilbert phân tách được của Định nghĩa 9 của IV, p. 292. Gọi $\widetilde{E}_q$ là phần hoàn thiện Hilbert của $E_q$, mà tích vô hướng của nó lại được ký hiệu bởi $(x, y)\mapsto (x|y)_q$. Vì đơn ánh chính tắc $\iota$ từ $E_q$ vào E liên tục, nó có một mở rộng liên tục duy nhất, ký hiệu là $\widetilde{\iota}$, từ $\widetilde{E}_q$ vào E. Dạng Hermit $q$ liên tục trên $E_q$, và do đó cũng được mở rộng thành một dạng Hermit dương liên tục duy nhất $\widetilde{q}$ trên $\widetilde{E}_q$.

Ta hãy chứng minh rằng ánh xạ tuyến tính $\widetilde{\iota}$ là đơn ánh. Cho $x\in$ Ker($\widetilde{\iota}$). Xét một dãy $(x_n)_{n\in\mathbf{N}}$ trong $E_q$ hội tụ tới $x$ trong $\widetilde{E}_q$. Khi đó

lim$_{n\rightarrow+\infty}\iota (x_n) =\widetilde{\iota}(x) = 0$,

do đó dãy $(x_n)_{n\in\mathbf{N}}$ hội tụ tới 0 trong E. Cho $y\in E_q$. Vì $\widetilde{q}$ liên tục trên $\widetilde{E}_q$, suy ra

$(x|y)_q=$ lim$_{n\rightarrow+\infty}(x_n|y)_q=$ lim$_{n\rightarrow+\infty}(\langle x_n|y\rangle +q(x_n, y))$

= lim$_{n\rightarrow+\infty}(\langle x_n|y\rangle +\langle x_n|u(y)\rangle )= 0$.

Vì không gian $E_q$ trù mật trong $\widetilde{E}_q$, suy ra $x= 0$, như mong muốn.

Đồng nhất $\widetilde{E}_q$ với ảnh của nó qua $\widetilde{\iota}$ trong E, ta hiểu $\widetilde{q}$ như một dạng từng phần dương đóng có miền trù mật mở rộng $q$. Toán tử tự liên hợp dương liên kết với $\widetilde{q}$ là một mở rộng tự liên hợp của $u$. Nó được gọi là mở rộng Friedrichs của $u$.

#### Nhận xét {#ts-iv-s5-n8-rem-2 .statement tag=036R}

Cho $c\in \mathbf{R}_+$. Cho $q$ là một dạng Hermit bộ phận đóng với miền xác định trù mật sao cho $q(x, x)\geqslant -c\|x\|^2$ với mọi $x$ thuộc miền của $q$. Điều này có nghĩa là dạng Hermit bộ phận đóng với miền dom($q$) được xác định bởi $\widetilde{q}(x, y) =q(x, y) +c\langle x|y\rangle$ là một dạng bộ phận dương. Theo Định lý 3, các dạng như vậy do đó tương ứng với các toán tử bộ phận tự liên hợp $u$ trên E sao cho $u+c1_E$ là dương, nghĩa là sao cho $u$ bị chặn dưới (Định nghĩa 7 của IV, p. 237) bởi $-c$.

Ngược lại, cho $u$ là một toán tử bộ phận đối xứng trên E sao cho

$$
\langle x|u(x)\rangle \geqslant -c\|x\|^2 \tag{17}
$$

với mọi $x\in$ dom($u$). Khi đó $v=u+c1_E$ là một toán tử bộ phận dương trên E. Mở rộng Friedrichs của $u$ được định nghĩa là toán tử tự liên hợp $\widetilde{v}-c1_E$, trong đó $\widetilde{v}$ là mở rộng Friedrichs của $v$; nó là một mở rộng tự liên hợp của $u$, không phụ thuộc vào lựa chọn số thực $c$ thỏa mãn (17).

### 9. Các nguyên lý biến phân cho phổ của các toán tử dương

Trong No. này, E là một không gian Hilbert phức khác không.

#### Mệnh đề 15 {#ts-iv-s5-prop-15 .statement tag=036S}

Cho $u$ là một toán tử bộ phận tự liên hợp trên E. Giả sử rằng $u$ bị chặn dưới bởi $c\in \mathbf{R}$ (Định nghĩa 7 của IV, p. 237). Khi đó

inf(Sp($u$)) $=$ inf$_{x\in dom(u)-\{0\}}\frac{\langle x|u(x)\rangle}{\|x\|^2}\in [c,+\infty [$.

Gọi $m$ là vế phải của đẳng thức cần chứng minh. Cho $x\in E$ và gọi $\mu_x$ là độ đo phổ của $x$ đối với $u$. Ta có

$$
\langle x|u(x)\rangle =\int t d\mu_x(t)
$$

Sp($u$)

$\geqslant$ inf(Sp($u$))$\int_{Sp(u)}d\mu_x(t) =$ inf(Sp($u$))$\|x\|^2$,

(công thức (6), p. 271), do đó inf(Sp($u$))$\leqslant m$. Ngược lại, toán tử bộ phận $u-m$ là dương, do đó inf(Sp($u$))$-m=$ inf(Sp($u-m\cdot 1_E$))$\geqslant 0$ (Mệnh đề 17 của IV, p. 248).

Mệnh đề 9 của I, p. 139 tương ứng với trường hợp riêng của mệnh đề này khi $u$ là một phần tử Hermit của $\mathscr{L}$ (E), trong trường hợp đó nó nhất thiết bị chặn dưới. Trong trường hợp này, ta cũng có

sup(Sp($u$)) $=$ sup$_{x\in dom(u)-\{0\}}\frac{\langle x|u(x)\rangle}{\|x\|^2}$

(ntd.); nếu $u$ không thuộc $\mathscr{L}$ (E), thì cận trên nhỏ nhất này là $+\infty$.

#### Định nghĩa 10 {#ts-iv-s5-def-10 .statement tag=036T}

Cho $u$ là một toán tử bộ phận chuẩn tắc trên E. Một số phức $\lambda \in$ Sp($u$) thuộc phổ rời rạc của $u$ nếu $\lambda$ là cô lập trong Sp($u$) và nếu $\lambda$ là một trị riêng có bội số hữu hạn.

Ta ký hiệu Sp$_s(u)$ là phổ rời rạc của $u$. Phần bù của nó trong Sp($u$) được gọi là phổ cốt yếu của $u$ và được ký hiệu là Sp$_e(u)$.

Phổ cốt yếu của một toán tử bộ phận chuẩn tắc $u$ trên E là đóng trong $\mathbf{C}$, vì Sp($u$) là đóng trong $\mathbf{C}$ và phần bù của phổ cốt yếu là mở trong Sp($u$). Phổ rời rạc của $u$ không nhất thiết là đóng trong $\mathbf{C}$ (bài tập 36 của IV, p. 369).

#### Bổ đề 9 {#ts-iv-s5-lem-9 .statement tag=036U}

Cho E là một không gian Hilbert phức và $u$ là một toán tử bộ phận chuẩn tắc trên E. Cho $\lambda \in$ Sp($u$). Khi đó $\lambda \in$ Sp$_s(u)$ khi và chỉ khi tồn tại một lân cận mở V của $\lambda$ trong $\mathbf{C}$ sao cho phép chiếu phổ $p_V$ của $u$ xác định bởi V có hạng hữu hạn.

Cho $\lambda \in$ Sp$_s(u)$. Tồn tại một lân cận mở V của $\lambda$ trong $\mathbf{C}$ sao cho Sp($u$)$\cap V =\{\lambda \}$; khi đó phép chiếu phổ $p_V=p_{\{\lambda\}}$ có hạng hữu hạn (Hệ quả của Mệnh đề 9 của IV, p. 278).

Ngược lại, giả sử tồn tại một lân cận mở V của $\lambda$ sao cho phép chiếu phổ $p_V$ có hạng hữu hạn $n\in \mathbf{N}$. Theo Hệ quả của Mệnh đề 10 của IV, p. 279, giao $V\cap$ Sp($u$) chứa nhiều nhất $n$ phần tử, do đó $\lambda$ là cô lập trong Sp($u$). Vì vậy nó là một trị riêng của $u$ có bội số phổ không vượt quá $n$ theo Hệ quả của Mệnh đề 9 của IV, p. 278.

Trong phần còn lại của Số này, ta giả sử rằng E là vô hạn chiều; các tương tự của những kết quả dưới đây khi E là hữu hạn chiều được suy ra từ No.$^o4$ của IV, p. 153.

Cho $u$ là một toán tử tự liên hợp bị chặn dưới trên E. Cho $c$ là một cận dưới của $u$; phổ của $u$ được chứa trong $[c,+\infty [$ (Mệnh đề 15). Giả sử phổ cốt yếu của $u$ không rỗng. Khi đó ta ký hiệu $\varrho_e$ là cận dưới lớn nhất của phổ cốt yếu của $u$, sao cho $\varrho_e\geqslant c$ và $\varrho_e$ là một phần tử của phổ của $u$. Ta đặt Sp$_h(u) =$ Sp($u$)$\cap [\varrho_e,+\infty [$; đây là một tập con đóng của Sp($u$), do đó cũng của $\mathbf{C}$, sao cho inf(Sp$_h(u)$) $=\varrho_e$; nó được gọi là phần trên của phổ của $u$. Nếu phổ cốt yếu của $u$ rỗng, ta đặt Sp$_h(u) =\emptyset$ và $\varrho_e= +\infty$.

Giao Sp$_b(u) =$ Sp($u$)$\cap [0, \varrho_e[$ được chứa trong phổ rời rạc của $u$, và do đó các phần tử của nó là các trị riêng cô lập có bội số hữu hạn; nó được gọi là phần dưới của phổ của $u$. Gọi $E_b$ là không gian con đóng của E sinh bởi các không gian riêng tương ứng với các trị riêng $\lambda \in$ Sp$_b(u)$. Theo Hệ quả của Mệnh đề 9 của IV, p. 278 và Mệnh đề 8 của IV, p. 278, không gian $E_b$ là ảnh của phép chiếu phổ $p_{Sp_b(u)}$ được xác định bởi Sp$_b(u)$. Vì Sp($u$) là hợp rời nhau của Sp$_b(u)$ và Sp$_h(u)$, phần bù trực giao $E_h$ của $E_b$ là ảnh của phép chiếu phổ $p_{Sp_h(u)}$ được xác định bởi Sp$_h(u)$. Nếu Sp$_b(u)$ là hữu hạn, thì không gian $E_b$ có số chiều hữu hạn; khi đó không gian $E_h$ là khác không, vì E được giả sử là vô hạn chiều.

#### Bổ đề 10 {#ts-iv-s5-lem-10 .statement tag=036V}

Ta có

$$
\langle x|u(x)\rangle \geqslant \varrho_e\|x\|^2 \tag{18}
$$

với mọi $x\in E_h\cap$ dom($u$).

Nếu $x\in E_h\cap$ dom($u$), thì giá của độ đo phổ $\mu_x$ của $x$ đối với $u$ được chứa trong khoảng $[\varrho_e,+\infty [$ (Mệnh đề 9, a) của IV, p. 278), do đó

$$
\langle x|u(x)\rangle =\int_{\mathbf{R}}td\mu_x(t)\geqslant \varrho_e\|x\|^2
$$

#### Bổ đề 11 {#ts-iv-s5-lem-11 .statement tag=036W}

Giả sử rằng $E_b$ là hữu hạn chiều. Khi đó, với mọi số thực $\varepsilon  >$ 0, ảnh của phép chiếu phổ của $u$ được xác định bởi $[\varrho_e, \varrho_e+\varepsilon ]$ là vô hạn chiều.

Nếu $E_b$ là hữu hạn chiều, thì phổ cốt yếu của $u$ là khác rỗng, do đó $\varrho_e$ là hữu hạn và thuộc Sp$_e(u)$. Hơn nữa, phổ dưới Sp$_b(u)$ là hữu hạn, do đó tồn tại $\delta  >0$ sao cho $[\varrho_e-\delta , \varrho_e+\delta ]\cap$ Sp($u$)$\subset [\varrho_e, \varrho_e+\delta ]$. Mệnh đề này suy ra từ Bổ đề 9.

#### Mệnh đề 16 {#ts-iv-s5-prop-16 .statement tag=036X}

Tập Sp$_b(u)\subset [c, \varrho_e[$ là đếm được, rời rạc và đóng trong $[0, \varrho_e[$. Nó là tập các giá trị của một dãy tăng ngặt $(\nu_k)_{0\leqslant k<Card(Sp_b(u))}$ các số thực dương; nếu Sp$_b(u)$ là vô hạn, thì dãy $(\nu_k)$ hội tụ đến $\varrho_e$.

Đặt T = Sp$_b(u)\cap [0, \varrho_e[$. Theo định nghĩa, nó là một tập con đóng và rời rạc của $[c, \varrho_e[$. Với mọi số nguyên $i\geqslant 1$, tập Sp$_b(u)\cap [c, \varrho_e-1/i]$ là compact và rời rạc, do đó hữu hạn. Vì T là hợp của các tập hợp này với $i\geqslant 1$, tập T là đếm được.

Điều này kết thúc chứng minh nếu Sp$_b(u)$ là hữu hạn. Nếu Sp$_b(u)$ là vô hạn, ta kết luận bằng cách áp dụng Bổ đề 2 của III, p. 90 cho ảnh S của T qua ánh xạ $\lambda \mapsto \varrho_e-\lambda$.

Với mọi số nguyên $k$ sao cho $0\leqslant k <$ Card(Sp$_b(u)$), gọi $n_k\geqslant 1$ là bội số của trị riêng $\nu_k$ của $u$. Đặt $\mathbf{N}=\mathbf{N}\cup  \{+\infty \} \subset \mathbf{R}$. Gọi $M\in \overline{\mathbf{N}}$ là tổng của các bội số $n_k$. Nó là chiều Hilbert của $E_b$, nếu ta đồng ý nói rằng một không gian có chiều Hilbert vô hạn là có chiều $+\infty  \in \overline{\mathbf{N}}$.

Với mọi số nguyên $n$ sao cho $0\leqslant n <M$, người ta định nghĩa $\lambda_n(u) =\nu_k$, trong đó $k\geqslant 0$ là số nguyên duy nhất sao cho

$$
n_0+\cdots +n_{k-1}\leqslant n < n_0+\cdots +n_k
$$

Nếu $n\in \mathbf{N}$ thỏa mãn $n\geqslant M$, người ta đặt $\lambda_n(u) =\varrho_e$. Trường hợp này chỉ có thể xảy ra nếu Sp$_b(u)$ là hữu hạn, trong trường hợp đó $\varrho_e$ là hữu hạn, vì giả sử rằng E là có chiều vô hạn.

Theo phép dựng, dãy $(\lambda_n(u))_{n\in\mathbf{N}}$ là tăng và, với mọi phần tử $\lambda$ của Sp$_b(u)$, số các số nguyên $n$ sao cho $\lambda_n(u) =\lambda$ bằng bội số của $\lambda$ như một trị riêng của $u$. Dãy $(\lambda_n(u))_{n\in\mathbf{N}}$ tiến tới $+\infty$ khi và chỉ khi phổ cốt yếu của $u$ là rỗng.

Với mọi $n\in \mathbf{N}$, ký hiệu $\mathscr{F}_n$ (tương ứng $\mathscr{F}_n^u$) là tập hợp các không gian con vectơ $F\subset E$ có chiều $n$ (tương ứng tập hợp các không gian con vectơ $F\subset$ dom($u$) có chiều $n$).

Cho $n\in \mathbf{N}$ sao cho $n <M$ và cho $F\in \mathscr{F}_n^u$. Ta nói rằng F thích nghi với $u$ nếu F có một cơ sở trực chuẩn $(f_i)_{0\leqslant i\leqslant n-1}$ sao cho $u(f_i) =\lambda_i(u)f_i$ với $0\leqslant i\leqslant n-1$.

Cho $F\in \mathscr{F}_n^u$ thích nghi với $u$. Không gian F được chứa trong $E_b$; nó được sinh bởi các vectơ riêng của $u$ ứng với các trị riêng $\lambda \leqslant \lambda_{n-1}(u)$, và nó chứa các không gian riêng tương ứng với các trị riêng $\lambda  < \lambda_{n-1}(u)$. Hơn nữa, với mọi tập con A đo được phổ quát của Sp($u$), không gian F là ổn định dưới phép chiếu phổ $p_A$ được xác định bởi A (mđ. 9, c) của IV, p. 278).

#### Bổ đề 12 {#ts-iv-s5-lem-12 .statement tag=036Y}

Cho $F\in \mathscr{F}_n^u$ là một không gian con thích nghi với $u$. Mọi vectơ riêng của $u$ thuộc không gian $F^{\circ}\cap E_b$ đều có một trị riêng $\geqslant \lambda_n(u)$.

Cho $\ell$ sao cho $\lambda_{n-1}(u) =\nu_{\ell}$. Cho $x\in F^{\circ}\cap E_b$ là một vectơ riêng của $u$ ứng với một trị riêng $\lambda$, và cho $k <$ Card(Sp$_b(u)$) sao cho $\lambda =\nu_k$.

Điều kiện $k < \ell$ là không thể xảy ra, vì $\nu_k< \nu_{\ell}$, và không gian F khi đó sẽ chứa không gian con riêng ứng với trị riêng $\nu_k$, mâu thuẫn với việc $x$ trực giao với F. Nếu $k=\ell$, thì $x$ là một vectơ riêng ứng với trị riêng $\lambda_{n-1}(u)$; vì $x\in F^{\circ}$, bội số $n_k$ lớn hơn nghiêm ngặt số các số nguyên $i < n$ sao cho $\lambda_i(u) =\nu_k$, điều này suy ra rằng $\lambda_n(u) =\lambda_{n-1}(u)$. Cuối cùng, nếu $k > \ell$, ta có $\lambda =\nu_k> \nu_{\ell}=\lambda_{n-1}(u)$, do đó $\lambda \geqslant \lambda_n(u)$.

Với mọi không gian con F của E, đặt

$\widetilde{r}_F(u) =$ inf$_{x\in dom(u)\cap F^{\circ}}\frac{\langle x|u(x)\rangle}{\|x\|^2}$,

$x\not =0$

$\widetilde{R}_F(u) =$ sup $\frac{\langle x|u(x)\rangle}{2}$.

$$
_{x\in dom(u)\cap F}\|x\|
$$

$x\not =0$

#### Mệnh đề 17 {#ts-iv-s5-prop-17 .statement tag=036Z}

a) Với mọi số nguyên $n\in \mathbf{N}$, ta có

$\lambda_n(u) =$ sup$_{F\in\mathscr{F}_n}\widetilde{r}_F(u) =$ inf$_{F\in\mathscr{F}_{n+1}^u}\widetilde{R}_F(u)$;

b) Với mọi số nguyên $n <M$ và với mọi không gian con $F\in \mathscr{F}_n^u$ thích nghi với $u$, ta có $\lambda_n(u) =\widetilde{r}_F(u)$;

c) Với mọi số nguyên $n <M$ và với mọi không gian con $F\in \mathscr{F}_{n+1}^u$ thích nghi với $u$, ta có $\lambda_n(u) =\widetilde{R}_F(u)$.

Tồn tại một cơ sở trực chuẩn $(e_n)_{0\leqslant n<M}$ của không gian $E_b$ sao cho $e_n\in$ dom($u$) và $u(e_n) =\lambda_n(u)e_n$ với mọi $n$ sao cho $0\leqslant n <M$. Với mọi $x\in E_b\cap$ dom($u$), do đó ta có

$$
\langle x|u(x)\rangle =\sum_{0\leqslant n<M}\lambda_n(u)|\langle e_n|x\rangle |^2
$$

Với mọi số nguyên $n$ sao cho $1\leqslant n <M + 1$, gọi $F_n$ là không gian con có chiều $n$ của $E_b$ sinh bởi $(e_0, . . . , e_{n-1})$. Ta có $F_n\subset$ dom($u$) và $F_n$ thích nghi với $u$.

Cho $n\in \mathbf{N}$ và $F\in \mathscr{F}_n$. Ta hãy chứng minh rằng $\widetilde{r}_F(u)\leqslant \lambda_n(u)$ và, do đó, rằng

(19) Fsup$_{\in\mathscr{F}_n}\widetilde{r}_F(u)\leqslant \lambda_n(u)$.

Nếu $0\leqslant n <M$, đặc biệt nếu M là vô hạn, thì hạn chế của phép chiếu trực giao của E lên F vào $F_{n+1}$ không đơn ánh, do đó tồn tại $x\not = 0$ trong $F_{n+1}$ trực giao với F. Vì

$$
\langle x|u(x)\rangle =\sum_{0\leqslant i\leqslant n}\lambda_i(u)|\langle e_i|x\rangle |^2=\lambda_n(u)|\langle e_n|x\rangle |^2\leqslant \lambda_n(u)\|x\|^2
$$

ta có $\widetilde{r}_F(u)\leqslant \lambda_n(u)$.

Nếu $M\in \mathbf{N}$ và $n\geqslant M$, thì với mọi số thực $\varepsilon  >0$, tồn tại $x$ có chuẩn bằng 1 trong dom($u$), trực giao với F và có độ đo phổ $\mu_x$ có giá đỡ được chứa trong $[\varrho_e, \varrho_e+\varepsilon ]$ (Bổ đề 11 và Mệnh đề 9, a) của IV, p. 278), do đó

$$
\widetilde{r}_F(u)\leqslant \langle x|u(x)\rangle =\int_{Sp(u)}t d\mu_x(t)\leqslant \varrho_e+\varepsilon =\lambda_n(u) +\varepsilon
$$

theo định nghĩa. Vì $\varepsilon  >0$ là tùy ý, do đó ta có $\widetilde{r}_F(u)\leqslant \lambda_n(u)$. Bất đẳng thức (19) do đó được thiết lập.

Cho $n\in \mathbf{N}$ và $F\in \mathscr{F}_{n+1}^u$. Ta hãy chứng minh rằng $\widetilde{R}_F(u)\geqslant \lambda_n(u)$ và, do đó, rằng

(20) Finf$_{\in\mathscr{F}_{n+1}^u}\widetilde{R}_F(u)\geqslant \lambda_n(u)$.

Nếu $0\leqslant n <M$, nhận xét rằng hạn chế lên F của phép chiếu trực giao lên $F_n$ không đơn ánh, do đó tồn tại một vectơ $x\not = 0$ trong F trực giao với $F_n$. Đặt $x_b=p_{Sp_b(u)}(x)$ và $x_h=p_{Sp_h(u)}(x)$. Do đó ta có $x=x_b+x_h$. Các phần tử $x_b$ và $x_h$ thuộc miền xác định của $u$ (Mệnh đề 9, c) của IV, p. 278) và trực giao với $F_n$. Ta có cận dưới

$$
\langle x_b|u(x_b)\rangle =\sum_{i\geqslant n}\lambda_i(u)|\langle e_i|x_b\rangle |^2\geqslant \lambda_n(u)\|x_b\|^2
$$

và $\langle x_h|u(x_h)\rangle \geqslant \varrho_e\|x_h\|^2$ (công thức (18)), do đó

$$
\langle x|u(x)\rangle =\langle x_b|u(x_b)\rangle +\langle x_h|u(x_h)\rangle
$$

$$
\geqslant \lambda_n(u)\|x_b\|^2+\varrho_e\|x_h\|^2\geqslant \lambda_n(u)\|x\|^2
$$

Nếu M là hữu hạn và $n\geqslant M$, tồn tại $x\not = 0$ trong F trực giao với $E_b$, do đó $x\in E_h$, và

$$
\langle x|u(x)\rangle \geqslant \varrho_e\|x\|^2=\lambda_n(u)\|x\|^2
$$

theo (18). Bất đẳng thức (20) do đó được chứng minh.

Bây giờ ta sẽ chứng minh các mệnh đề b) và c), chúng kéo theo rằng các bất đẳng thức (19) và (20) là các đẳng thức khi $n <M$.

Ta chứng minh mệnh đề b). Cho $F\in \mathscr{F}_n^u$ là một không gian thích nghi với $u$. Ta có tổng trực tiếp Hilbert

$F^{\circ}= E_h\oplus \bigoplus_{\lambda\in Sp_b(u)}$ Ker($u-\lambda \cdot 1_E$)$\oplus (F^{\circ}\cap$ Ker($u-\lambda_{n-1}(u)\cdot 1_E$)).

$\lambda >\lambda_{n-1}(u)$

Cho $x\in F^{\circ}-\{0\}$. Viết $x=x_h+y+z$, trong đó $x_h\in E_h$ và $y$ (tương ứng $z$) thuộc không gian thứ hai (tương ứng thứ ba) của phân tích trên. Sử dụng lại (18) và sự kiện rằng mọi trị riêng $\lambda  > \lambda_{n-1}(u)$ của $u$ đều $\geqslant \lambda_n(u)$, ta thu được

$$
\langle x|u(x)\rangle =\langle x_h|u(x_h)\rangle +\langle y|u(y)\rangle +\langle z|u(z)\rangle
$$

$$
\geqslant \varrho_e\|x_h\|^2+\lambda_n(u)\|y\|^2+\lambda_{n-1}(u)\|z\|^2
$$

Nếu $z\not = 0$, thì theo Bổ đề 12, ta có $\lambda_n(u) =\lambda_{n-1}(u)$. Do đó suy ra rằng $\langle x|u(x)\rangle \geqslant \lambda_n(u)\|x\|^2$, do đó $\widetilde{r}_F(u)\geqslant \lambda_n(u)$. Kết hợp với (19), điều này kéo theo mệnh đề b).

Ta chứng minh mệnh đề c). Cho $F\in \mathscr{F}_{n+1}^u$ là một không gian con thích nghi với $u$. Cho $(f_i)_{0\leqslant i\leqslant n}$ là một cơ sở trực chuẩn của F sao cho $u(f_i) =\lambda_i(u)f_i$ với $0\leqslant i\leqslant n$. Với mọi $x\in F$, ta có

$$
\langle x|u(x)\rangle =\sum_{0\leqslant i\leqslant n}\lambda_i(u)|\langle f_i|x\rangle |^2\leqslant \lambda_n(u)\|x\|^2
$$

với đẳng thức nếu $x=f_n$, do đó $\widetilde{R}_F(u) =\lambda_n(u)$.

Cuối cùng ta chứng minh rằng (19) và (20) là các đẳng thức khi $n\geqslant M$. Trong trường hợp này, M là hữu hạn, do đó $E_b$ được chứa trong miền xác định của $u$; hơn nữa, theo định nghĩa ta có $\lambda_n(u) =\varrho_e$.

Tồn tại $F\in \mathscr{F}_n$ chứa $E_b$. Mọi phần tử $x\not = 0$ của dom($u$) trực giao với F do đó trực giao với $E_b$, và thỏa mãn

$$
\frac{\langle x|u(x)\rangle}{2}\geqslant \varrho_e
$$

$$
\|x\|
$$

(công thức (18)), do đó $\widetilde{r}_F(u)\geqslant \varrho_e=\lambda_n(u)$, và do đó

sup$_{F\in\mathscr{F}_n}\widetilde{r}_F(u)\geqslant \lambda_n(u)$.

Cho $\varepsilon  >0$. Vì $E_b$ là hữu hạn chiều, suy ra từ bổ đề 11 rằng tồn tại một họ trực chuẩn $(x_i)_{i\in I}$ gồm các phần tử của E sao cho không gian con F sinh bởi $E_b$ và $(x_i)_{i\in I}$ có chiều $n+ 1$ và được chứa trong dom($u$), và sao cho $\langle x_i|u(x_i)\rangle \leqslant \varrho_e+\varepsilon$ với mọi $i\in I$. Khi đó ta có $\widetilde{R}_F(u)\leqslant \varrho_e+\varepsilon$. Vì $\varepsilon  >0$ là tùy ý, ta kết luận rằng

inf$_{F\in\mathscr{F}_{n+1}^u}\widetilde{R}_F(u)\leqslant \varrho_e=\lambda_n(u)$.

Mệnh đề được chứng minh.

### 10. Nhiễu compact và phổ cốt yếu

Trong số này, E là một không gian Hilbert phức vô hạn chiều.

#### Bổ đề 13 {#ts-iv-s5-lem-13 .statement tag=0370}

Cho I là một họ trực chuẩn trong E. Họ I hội tụ yếu về 0 đối với bộ lọc các phần bù của các tập con hữu hạn của I.

Cho $x\in E$. Theo bất đẳng thức Bessel (EVT, V, p. 21, prop. 4) và TG, IV, p. 37, th. 1, họ $(|\langle e_i|x\rangle |^2)_{i\in I}$ là khả tổng, do đó $\langle e_i|x\rangle$ tiến tới 0 đối với bộ lọc các phần bù của các tập con hữu hạn của I (TG, III, p. 38, prop. 1).

#### Mệnh đề 18 {#ts-iv-s5-prop-18 .statement tag=0371}

Cho $u$ là một toán tử từng phần tự liên hợp trên E và $\lambda$ là một số thực. Khi đó $\lambda \in$ Sp$_e(u)$ khi và chỉ khi tồn tại một dãy trực chuẩn $(x_n)_{n\in\mathbf{N}}$ trong E sao cho $u(x_n)-\lambda x_n$ tiến tới 0 trong E.

Trước hết, giả sử rằng $\lambda \in$ Sp$_e(u)$. Nếu phép chiếu phổ của $u$ ứng với $\{\lambda \}$ có hạng vô hạn, thì mọi dãy trực chuẩn $(x_n)$ trong ảnh của nó đều trả lời câu hỏi (cf. cor. to prop. 9 of IV, p. 278). Ta sẽ giả sử trong phần tiếp theo rằng điều này không xảy ra.

Với mỗi $k\in \mathbf{N}$, cho $J_k$ là tập hợp các $t\in [\lambda -1, \lambda + 1]$ sao cho

$$
\frac{1}{k + 2}<|t-\lambda |\leqslant \frac{1}{k + 1}
$$

Các tập hợp $J_k$ rời nhau từng đôi một. Hơn nữa, với mọi số nguyên $K\in \mathbf{N}$, các tập hợp $(J_k)_{k\geqslant K}$ tạo thành một phân hoạch của tập hợp

$$
I_K= [\lambda -1/(K + 1), \lambda + 1/(K + 1)]-\{0\}
$$

Vì phép chiếu phổ của $u$ ứng với $I_K\cup  \{0\}$ có hạng vô hạn (Bổ đề 9 of IV, p. 297) và phép chiếu ứng với $\{\lambda \}$ được giả sử là có hạng hữu hạn, từ prop. 8 of IV, p. 278 ta suy ra rằng tồn tại một dãy tăng ngặt $(k_n)_{n\in\mathbf{N}}$ trong $\mathbf{N}$ sao cho phép chiếu phổ $p_n$ của $u$ ứng với $J_{k_n}$ là khác không. Cho $x_n$ là một vectơ có chuẩn 1 trong ảnh của $p_n$. Dãy $(x_n)$ là trực chuẩn, vì ảnh của $p_n$ trực giao với ảnh của $p_m$ với mọi $n\not =m$ trong $\mathbf{N}$.

Cho $n\in \mathbf{N}$. Gọi $\mu_n$ là độ đo phổ của $x_n$ ứng với $u$; giá của nó được chứa trong $J_{k_n}$ (prop. 9 of IV, p. 278). Suy ra rằng

$$
\|u(x_n)-\lambda x_n\|^2=\int|t-\lambda |^2d\mu_n(t)\leqslant 1_2
$$

$$
_{\mathbf{C}}k_n
$$

do đó dãy $(x_n)_{n\in\mathbf{N}}$ có tính chất đã yêu cầu.

Ngược lại, giả sử tồn tại một dãy trực chuẩn $(x_n)_{n\in\mathbf{N}}$ trong E sao cho $u(x_n)-\lambda x_n\rightarrow$ 0. Ký hiệu $\mu_n$ là độ đo phổ của $x_n$ đối với $u$.

Cho $\varepsilon  >0$. Ký hiệu $p_{\varepsilon}$ là phép chiếu phổ của $u$ đối với khoảng mở $I_{\varepsilon}= ]\lambda -\varepsilon , \lambda +\varepsilon [$. Với mọi $n\in \mathbf{N}$, ta có

$$
1 =\|x_n\|^2=\mu_n(I_{\varepsilon}) +\mu_n(\mathbf{R}-I_{\varepsilon})
$$

$$
\leqslant \mu_n(I_{\varepsilon}) +1_2\int|t-\lambda |^2d\mu_n(t)
$$

$$
\varepsilon_{\mathbf{R}-I_{\varepsilon}}
$$

$$
=\|p_{\varepsilon}(x_n)\|^2+\frac{1}{\varepsilon^2}\|u(x_n)-\lambda x_n\|^2
$$

Giả thiết về dãy $(x_n)$ do đó suy ra rằng chuẩn của $p_{\varepsilon}(x_n)$ không thể hội tụ về 0. Vì dãy trực chuẩn $(x_n)$ hội tụ yếu về 0 trong E (Bổ đề 13), phép chiếu $p_{\varepsilon}$ không thể compact (Hệ quả của Mệnh đề 6 của III, p. 6) và do đó có hạng vô hạn. Vì điều này đúng với mọi $\varepsilon  >0$, Bổ đề 9 của IV, p. 297 cho phép ta kết luận rằng $\lambda \in$ Sp$_e(u)$.

Định lý sau đây là tương tự của Định lý 3 của III, p. 93 đối với các toán tử bộ phận tự liên hợp.

#### Định lý 4 {#ts-iv-s5-thm-4 .statement tag=0372}

Cho $u$ là một toán tử bộ phận tự liên hợp trên E. Phổ cốt yếu của $u$ là giao của các tập Sp($u+v$), trong đó $v$ chạy qua tập các tự đồng cấu Hermit compact của E.

Toán tử bộ phận $u+v$ là tự liên hợp với mọi tự đồng cấu Hermit $v$ của E, vì $(u+v)^*=u^*+v^*($cf. IV, p. 236).

Ta chứng minh rằng nếu $v$ là compact, thì Sp$_e(u)\subset$ Sp$_e(u+v)$. Cho $\lambda \in$ Sp$_e(u)$, và cho $(x_n)_{n\in\mathbf{N}}$ là một dãy trực chuẩn trong E sao cho $u(x_n)-\lambda x_n$ hội tụ về 0 (Mệnh đề 18). Dãy $(x_n)$ hội tụ yếu về 0 trong E (Bổ đề 13), và vì tự đồng cấu $v$ là compact, dãy $(v(x_n))_{n\in\mathbf{N}}$ hội tụ về 0 trong E (Hệ quả của Mệnh đề 6 của III, p. 6). Do đó dãy $(u+v)(x_n)-\lambda x_n$ hội tụ về 0 trong E, và Mệnh đề 18 suy ra rằng $\lambda \in$ Sp$_e(u+v)$.

Phổ cốt yếu của $u$ do đó được chứa trong giao của các tập Sp($u+v$) với $v\in \mathscr{L}^c(E)$ là Hermit.

Ngược lại, cho $\lambda \in$ Sp$_s(u)$. Cho $E_{\lambda}$ là không gian con thực sự của $u$ tương ứng với $\lambda$, và $p_{\lambda}$ là phép chiếu trực giao có ảnh $E_{\lambda}$; nó là phép chiếu phổ của $u$ tương ứng với $\{\lambda \}$ (Hệ quả của Mệnh đề 9 của IV, p. 278). Theo định nghĩa của phổ nhạy, phép chiếu $p_{\lambda}$ có hạng hữu hạn, do đó compact. Đặt $w=u+p_{\lambda}$; nó là một toán tử bộ phận tự liên hợp. Để kết luận chứng minh, ta hãy kiểm tra rằng $\lambda$ thuộc tập giải của $w$.

Ta có $E_{\lambda}\subset$ dom($u$), và các không gian $E_{\lambda}$ và dom($u$)$\cap E^{\circ}_{\lambda}$ là bất biến đối với $u$ (Mệnh đề 9 của IV, p. 278).

Cho $x\in$ dom($u$). Viết $x=p_{\lambda}(x)+y$, trong đó $y\in$ dom($u$)$\cap E^{\circ}_{\lambda}$. Theo điều trên, ta có

$$
\|w(x)-\lambda x\|^2=\|p_{\lambda}(x)\|^2+\|w(y)-\lambda y\|^2 \tag{21}
$$

Cho V là một lân cận mở của $\lambda$ không gặp phổ của $u$, và cho $c >0$ sao cho đĩa có tâm $\lambda$ và bán kính $c$ được chứa trong V. Gọi $\mu_y$ là độ đo phổ của $y$ đối với $u$. Vì $y$ trực giao với $E_{\lambda}$, giá của $\mu_y$ không gặp V (ntd.). Khi đó ta có

$$
\|w(y)-\lambda y\|^2=\|u(y)-\lambda y\|^2=\int_{\mathbf{C}}|t-\lambda |^2d\mu_y(t)\geqslant c^2\|y\|^2 \tag{22}
$$

Từ (21) và (22) suy ra rằng $\|w(x)-\lambda x\|^2\geqslant$ inf($c^2,1$)$\|x\|^2$; vì $w$ là tự liên hợp và $\lambda \in \mathbf{R}$, kết luận sau đó suy ra từ Bổ đề 5 của IV, p. 248.

#### Hệ quả {#ts-iv-s5-n10-cor-1 .statement tag=0373}

Cho $u$ là một toán tử từng phần tự liên hợp trên E và $v$ là một tự đồng cấu Hermit compact của E. Khi đó Sp$_e(u+v) =$ Sp$_e(u)$.

Điều này suy ra ngay lập tức từ định lý.

### 11. Nhiễu

Trong No. này, E là một không gian Hilbert phức.

Nếu $u$ là một toán tử từng phần tự liên hợp trên E và $v\in \mathscr{L}(E)$ là một tự đồng cấu Hermit, thì $u+v$ là tự liên hợp (xem IV, p. 236). Điều này nói chung không đúng khi $v$ là một toán tử từng phần đối xứng (Bài tập 9 của IV, p. 347). Tuy nhiên trong No. này ta vẫn thu được các kết quả dương thuộc loại này.

#### Định nghĩa 11 {#ts-iv-s5-def-11 .statement tag=0374}

Cho $u$ là một toán tử từng phần trên E. Một toán tử từng phần $v$ trên E được gọi là bị chặn tương đối với $u$ nếu dom($u$)$\subset$ dom($v$) và nếu $v$ xác định, bằng cách chuyển qua không gian con, một ánh xạ tuyến tính liên tục từ $E_u$ vào E.

Cho $u$ là một toán tử từng phần trên E. Cho $v$ là một toán tử từng phần bị chặn tương đối với $u$. Tồn tại một số thực $m$ sao cho

$$
\|v(x)\|\leqslant m(\|x\|+\|u(x)\|)
$$

với mọi $x\in$ dom($u$). Cận dưới lớn nhất của các số thực $a\geqslant 0$ sao cho tồn tại một số thực $b$ sao cho

$$
\|v(x)\|\leqslant a\|u(x)\|+b\|x\|
$$

được gọi là chuẩn tương đối của $v$ đối với $u$, và được ký hiệu bởi $\|v\|_u$,

với mọi $x\in$ dom($u$). Chuẩn tương đối của $v$ do đó nhỏ hơn hoặc bằng chuẩn của hạn chế của $v$ vào không gian $E_u$.

#### Nhận xét {#ts-iv-s5-n11-rem-1 .statement tag=0375}

Cho $u$ là một toán tử từng phần trên E. Mọi tự đồng cấu $v\in \mathscr{L}(E)$ đều bị chặn tương đối đối với $u$ và chuẩn tương đối của nó bằng không, vì $\|v(x)\|\leqslant \|v\| \|x\|$ với mọi $x\in$ dom($u$), điều này cho phép lấy $a= 0$ trong bất đẳng thức trên.

#### Định lý 5 (Kato-Rellich) {#ts-iv-s5-thm-5 .statement tag=0376}

Cho $u$ là một toán tử từng phần tự liên hợp trên E và $v$ là một toán tử từng phần đối xứng bị chặn tương đối đối với $u$. Nếu chuẩn tương đối $\|v\|_u$ là $<1$, thì toán tử từng phần $u+v$ với miền dom($u$) là tự liên hợp.

Vì $\|v\|_u<1$, theo định nghĩa, tồn tại các số thực dương $a$ và $b$ sao cho $a <1$ và $\|v(x)\|\leqslant a\|u(x)\|+b\|x\|$ với mọi $x\in$ dom($u$).

Cho $t\in \mathbf{R}^*$. Đặt $w_t=v\circ R(u, it)$. Ta có dom($w_t$) $= E$ vì ảnh của $R(u, it)$ được chứa trong miền của $u$, miền này được chứa trong miền của $v$ theo giả thiết. Cho $x\in$ dom($u$). Vì $u$ là tự liên hợp, ta có

$$
\|(it-u)x\|^2=\|itx\|^2+\|u(x)\|^2-it\langle x|u(x)\rangle +it\langle u(x)|x\rangle
$$

$$
=|t|^2\|x\|^2+\|u(x)\|^2
$$

do đó các bất đẳng thức $\|u(x)\|\leqslant \|(it-u)x\|$ và $\|x\|\leqslant |t|^{-1}\|(it-u)x\|$. Nhưng khi đó ta được

$$
\|v(x)\|\leqslant (a+b|t|^{-1})\|(it-u)x\|
$$

Đặc biệt, đặt $x= R(u, it)y$ với $y\in E$; ta thu được

$$
\|w_t(y)\|\leqslant (a+b|t|^{-1})\|y\|
$$

Suy ra rằng $w_t\in \mathscr{L}(E)$ và $\|w_t\|\leqslant a+|t|^{-1}b$.

Vì $a <$ 1, tồn tại $t\in \mathbf{R}^*_+$ sao cho $a+b|t|^{-1}<1$. Khi đó $\|w_t\|<1$ và $\|w_{-t}\|<1$; các tự đồng cấu $1_E-w_t$ và $1_E-w_{-t}$ của E do đó là khả nghịch (Mệnh đề 2 của I, p. 22). Vì ta có công thức $(1_E-w_t)\circ (it-u) =it-(u+v)$, điều này suy ra rằng $u+v-it$ là toàn ánh; tương tự, toán tử từng phần $u+v+it$ là toàn ánh. Suy ra rằng $u+v$ là tự liên hợp (Mệnh đề 11 của IV, p. 240).

### 12. Các toán tử có giải thức compact

Trong số này, E ký hiệu một không gian Hilbert phức vô hạn chiều.

#### Mệnh đề 19 {#ts-iv-s5-prop-19 .statement tag=0377}

Cho $u$ là một toán tử từng phần tự liên hợp trên E. Các điều kiện sau là tương đương :

(i) Tồn tại một cơ sở trực chuẩn $B = (e_j)_{j\in J}$ của E sao cho $u$ là đường chéo trong cơ sở B và giá trị tuyệt đối của họ các trị riêng của $u$ tiến tới vô cùng theo lọc các phần bù của các tập hợp hữu hạn của J;

(ii) Với mọi $\lambda$ thuộc tập giải thức của $u$, giải thức $R(u, \lambda )$ là compact;

(iii) Tồn tại một số phức $\lambda$ thuộc tập giải thức của $u$ sao cho giải thức $R(u, \lambda )$ là compact;

(iv) Phổ của $u$ trùng với phổ điểm của $u$.

Giả sử (i) được thỏa mãn, và gọi $(\lambda_j)_{j\in J}$ là họ các trị riêng của $u$. Gọi $\mu$ là độ đo đếm trên J. Phổ của $u$ là ảnh cốt yếu-$\mu$ của họ $(\lambda_j)$ (Mệnh đề 22 của IV, p. 252); nó là tập hợp các giá trị của họ này. Với mọi $\lambda  \notin$ Sp($u$), giải thức $R(u, \lambda )$ là đường chéo trong cơ sở B và họ các trị riêng của nó là $((\lambda -\lambda_j)^{-1})_{j\in J}($loc. cit.). Vì họ này hội tụ về 0, tự đồng cấu $R(u, \lambda )$ là compact (Mệnh đề 2, (iii) của IV, p. 148). Điều này chứng minh rằng (i) kéo theo (ii).

Vì tập giải thức của $u$ là khác rỗng (xem Mệnh đề 17 của IV, p. 248), các tính chất (ii) và (iii) là tương đương theo công thức (8) của IV, p. 245 và Mệnh đề 3 của III, p. 5.

Vì $R(u, \lambda )$ là chuẩn tắc đối với $\lambda  \notin$ Sp($u$) (Mệnh đề 16 của IV, p. 247), điều kiện (iii) kéo theo (iv) theo Mệnh đề 15 của IV, p. 247 và Mệnh đề 5 của III, p. 90.

Cuối cùng ta chứng minh rằng (iv) kéo theo (i). Gọi $\mathscr{O}$ là tập hợp các tập con trực chuẩn của E gồm các vectơ riêng của $u$. Tập hợp $\mathscr{O}$, có thứ tự bởi quan hệ bao hàm, có đặc trưng hữu hạn (E, III, p. 34, Định nghĩa 2) vì O thuộc $\mathscr{O}$ khi và chỉ khi các tập hợp gồm nhiều nhất hai phần tử của O thuộc $\mathscr{O}$. Theo E, III, p. 35, Định lý 1, tồn tại một phần tử cực đại O của $\mathscr{O}$. Ký hiệu F là không gian con đóng của E sinh bởi O. Với $e\in O$, tồn tại duy nhất $\lambda (e)\in \mathbf{R}$ sao cho $u(e) =\lambda (e)e$ (Mệnh đề 17 của IV, p. 248).

Tập hợp các giá trị của ánh xạ $\lambda$ từ O vào $\mathbf{R}$ trùng với phổ của $u$. Thật vậy, một mặt tập hợp này được chứa trong phổ của $u$ và mặt khác, nếu tồn tại $\lambda_0\in$ Sp($u$) không phải là một giá trị của $\lambda$, thì $\lambda_0$ là một trị riêng của $u$ theo giả thiết. Tồn tại một vectơ $e\in$ dom($u$) có chuẩn 1 sao cho $u(e) =\lambda_0e$ và $e \notin O$; tập con $O\cup  \{e\}$ là trực chuẩn (vì các không gian riêng của $u$ ứng với các trị riêng phân biệt là trực giao theo mệnh đề b) của hệ quả của Mệnh đề 17 của IV, p. 248); nó thuộc $\mathscr{O}$, mâu thuẫn với tính cực đại của O.

Giả sử rằng $F\not = E$. Khi đó $F^{\circ}$ là khác không. Tự đồng cấu $R(u, i)$ của E là chuẩn (mệnh đề 16 của IV, p. 247). Nó giữ ổn định không gian con $F^{\circ}$ của E (bổ đề 4 của I, p. 135). Cho $v$ là tự đồng cấu của $F^{\circ}$ suy ra từ $R(u, i)$ bằng cách chuyển qua các không gian con. Nó là một tự đồng cấu liên tục và chuẩn của $F^{\circ}($loc. cit.) mà phổ của nó được chứa trong phổ của $R(u, i)$. Vì $F^{\circ}$ là khác không, phổ của $v$ là khác rỗng (hệ quả 1 của I, p. 26). Hơn nữa, phổ của $v$ không rút gọn về 0, vì tự đồng cấu chuẩn $v$ là khác không (ví dụ 1 của I, p. 110). Cho $s\in$ Sp($v$)$-\{0\}$. Vì $s$ thuộc phổ của $R(u, i)$, tồn tại $e\in O$ sao cho $s= (i-\lambda (e))^{-1}$, và $s$ là một trị riêng của $R(u, i)$ (mệnh đề 15, a) của IV, p. 247). Vì $s$ là khác không, nó là một điểm cô lập của Sp(R($u, i$)) theo giả thiết, do đó cũng là một điểm cô lập của Sp($v$). Vì vậy, $s$ là một trị riêng của $v$ (mệnh đề 5, c) của I, p. 134). Cho $e\in F^{\circ}$ là một vectơ riêng chuẩn 1 của $v$; nó cũng là một vectơ riêng của $u$ (mệnh đề 15, b) của IV, p. 247), và tập hợp $O\cup  \{e\}$ mâu thuẫn với sự kiện rằng O là cực đại trong $\mathscr{O}$. Do đó F = E.

Họ các phần tử của O vì vậy là một cơ sở trực chuẩn của E được tạo thành bởi các vectơ riêng của $u$. Phổ của $u$ là đóng trong $\mathbf{R}$, và phổ điểm là rời rạc; vì các tập hợp này trùng nhau, tập hợp các phần tử $\lambda \in$ Sp($u$) sao cho $|\lambda |\leqslant R$ là compact, do đó hữu hạn, với mọi $R>0$. Vì vậy họ các giá trị tuyệt đối của các trị riêng của $u$ tiến tới vô hạn theo lọc các phần bù của các tập hợp con hữu hạn của O. Do đó (iv) suy ra (i).

#### Định nghĩa 12 {#ts-iv-s5-def-12 .statement tag=0378}

Cho $u$ là một toán tử bộ phận tự liên hợp trên E. Ta nói rằng $u$ có resolvent compact nếu các điều kiện tương đương của mệnh đề 19 được thỏa mãn.

#### Mệnh đề 20 {#ts-iv-s5-prop-20 .statement tag=0379}

Cho $u$ là một toán tử bộ phận tự liên hợp trên E. Khi đó $u$ có resolvent compact khi và chỉ khi đơn ánh chính tắc $j$ của không gian Hilbert $E_u$ vào E là compact.

Giả sử rằng $u$ có resolvent compact. Tồn tại $\lambda  \notin$ Sp($u$) sao cho $R(u, \lambda )$ là compact (mệnh đề 19, (iii)). Cho B là quả cầu đơn vị của không gian Hilbert $E_u$. Vì $u$ là một ánh xạ tuyến tính liên tục từ $E_u$ vào E, tập con $B'= (\lambda 1_E-u)(B)$ của E là bị chặn. Vì $R(u, \lambda )$ là compact, tập con $B = R(u, \lambda )(B')$ là tương đối compact trong E (nhận xét 1 của III, p. 2). Điều này chứng minh rằng $j$ là compact.

Ngược lại, giả sử rằng ánh xạ tuyến tính $j$ là compact. Số phức $i$ thuộc tập giải thức của $u$ (Mệnh đề 17 của IV, p. 248). Ta có $u\circ R(u, i) =-1_E+iR(u, i)$. Gọi B là quả cầu đơn vị của E. Với mọi $x\in B$, ta có

$$
\|u\circ R(u, i)(x)\|=\|-x+iR(u, i)(x)\|\leqslant 1 +\|R(u, i)\|
$$

và do đó

$$
\|R(u, i)x\|^2_u=\|R(u, i)x\|^2+\|u\circ R(u, i)x\|^2
$$

$$
\leqslant \|R(u, i)\|^2+ (1 +\|R(u, i)\|)^2
$$

Ảnh C của B qua $R(u, i)$ do đó bị chặn trong $E_u$; vì $j$ là compact theo giả thiết, tập hợp $C =j(C)$ là tương đối compact trong E (III, loc. cit.). Do đó, giải thức $R(u, i)$ là compact và $u$ có giải thức compact (Mệnh đề 19, (iii)).

#### Hệ quả {#ts-iv-s5-n12-cor-1 .statement tag=037A}

Cho $q$ là một dạng riêng phần dương đóng trên E và $u$ là toán tử tự liên hợp dương biểu diễn $q$. Các điều kiện sau là tương đương:

(i) Toán tử riêng phần $u$ có giải thức compact;

(ii) Tự đồng cấu dương $\surd\overline{(1_E + u)^{-1}}= (1_E+u)^{-1/2}$ của E là compact;

(iii) Đơn ánh chính tắc $j$ của không gian Hilbert $E_q$ (Định nghĩa 9 của IV, p. 292) vào E là compact.

Vì $u$ là dương, số thực $-1$ thuộc tập giải thức của $u$ (Mệnh đề 17 của IV, p. 248), do đó tự đồng cấu dương $v=\surd\overline{(1_E + u)^{-1}}$ được xác định, và ta có $v= (1_E+u)^{-1/2}$ theo phép tính phiếm hàm.

Tự đồng cấu $v$ là compact khi và chỉ khi $v^2= (1_E+u)^{-1}$ là compact (Mệnh đề 6 của III, p. 91), nghĩa là khi và chỉ khi $u$ có giải thức compact (Mệnh đề 19, (iii)). Điều này chứng minh rằng các điều kiện (i) và (ii) là tương đương.

Giả sử rằng tự đồng cấu $v$ là compact. Gọi B là quả cầu đơn vị của không gian Hilbert $E_q$. Vì $(1_E+u)^{1/2}$ là một ánh xạ tuyến tính liên tục từ $E_q$ vào E (Hệ quả của Định lý 3 của IV, p. 294), tập con $B'= (1_E+u)^{1/2}(B)$ của E bị chặn, do đó tập con $j(B) = B =v(B')$ là tương đối compact trong E (Nhận xét 1 của III, p. 2). Điều này chứng minh rằng $j$ là compact. Vậy (ii) suy ra (iii).

Ánh xạ tuyến tính $\widetilde{v}:x\mapsto (1_E+u)^{-1/2}(x)$ từ E vào $E_q$ được xác định tốt và đẳng cự (Hệ quả của Định lý 3 của IV, p. 294). Vì $v=j\circ \widetilde{v}$, điều kiện (iii) suy ra (ii) (Mệnh đề 3 của III, p. 5).

#### Ví dụ {#ts-iv-s5-n12-exa-1 .statement tag=037B}

Cho $n\in \mathbf{N}$. Cho U là một tập hợp mở trong $\mathbf{R}^n$. Trang bị cho U độ đo Lebesgue, ký hiệu bởi $\mu$. Gọi Δ là toán tử vi phân vô hướng $-\sum^n_{i=1}\partial_i^2$ trên U. Toán tử riêng phần $\Delta_-$ với miền xác định $\mathscr{D}(U)$ được xác định bởi $\varphi \mapsto \Delta (\varphi )$ là đóng được (Mệnh đề 13 của IV, p. 242) và đối xứng (IV, p. 243). Nó là dương, vì với mọi $\varphi \in \mathscr{D}$(U), ta có

$$
\langle \varphi |\Delta_-(\varphi )\rangle =\int_U\overline{\varphi}\Delta (\varphi )d\mu=-\sum_{i=1}^n\int_U\varphi  \partial_i^2\varphi  d\mu
$$

$$
=\sum_{i=1}^n\int_U\partial_i\varphi  \partial_i\varphi  d\mu=\int_U\sum_{i=1}^n|\partial_i\varphi |^2d\mu\geqslant 0
$$

Ta ký hiệu $\Delta_D$ là mở rộng Friedrichs của toán tử riêng phần đối xứng dương $\Delta_-($IV, p. 295, Ví dụ); nó là một toán tử Laplace trên U, được gọi là toán tử Laplace Dirichlet trên U.

Cho $q$ là dạng riêng phần dương liên kết với $\Delta_D$. Miền xác định của $q$ là sự hoàn thiện Hilbert của $\mathscr{D}(U)$ đối với dạng Hermit dương được xác định bởi

$$
(\varphi_1, \varphi_2)\mapsto \int_U\overline{\varphi}_1\varphi_2+\sum_{i=1}^n\int_U\overline{\partial_i\varphi_1}\partial_i\varphi_2
$$

với mọi $(\varphi_1, \varphi_2)\in \mathscr{D}(U)\times \mathscr{D}(U)$. Nói cách khác, miền xác định của $q$ là không gian Sobolev $H^1_0(U)$ (No.$^o14$ của IV, p. 221).

*Giả sử rằng U bị chặn. Đơn ánh chính tắc của $H^1_0(U)$ vào $L^2(U)$ là compact; toán tử Laplace Dirichlet trên U do đó là một toán tử có giải thức compact (Hệ quả của Mệnh đề 20). Vì không gian Hilbert $H^1_0(U)$ có kiểu đếm được (Mệnh đề 20 của IV, p. 222), và vì ảnh của $\Delta_D$ có chiều vô hạn, tồn tại một dãy tăng $(\lambda_n)_{n\geqslant 0}$ các số thực tiến tới $+\infty$ và một cơ sở trực chuẩn $(f_n)_{n\in\mathbf{N}}$ của $L^2$(U), mà các phần tử của nó thuộc miền của $\Delta_D$, sao cho $\Delta_D(f_n) =\lambda_nf_n$ với mọi $n\in \mathbf{N}$. Có thể chứng minh ("luật Weyl") rằng khi T tiến tới $+\infty$, ta có

$$
\sum_{n\in\mathbf{N}}1\sim \frac{c_n}{(2\pi)^n}mT^{n/2}
$$

$\lambda_n\leqslant T$

trong đó $c_n=\pi^{n/2}/\Gamma (1 +n/2)$ là thể tích của quả cầu đơn vị trong $\mathbf{R}^n$ (INT, V, p. 101, § 8, n$^o7$) và $m >0$ là độ đo Lebesgue của U.*

## BÀI TẬP {#ts-iv-s5-exercises}

Trừ khi có quy định khác, các không gian Hilbert dưới đây được giả sử là phức.

Xem [các bài tập cho § 5](exercises/s5/).
