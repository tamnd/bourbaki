---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 3
section_title: Groupes de Poincaré des groupes topologiques
lang: vi
source: ta-i-iv-fr
book_pages: TA IV.369-TA IV.382, TA IV.459-TA IV.461
pdf_pages: 0385-0398, 0475-0477
extraction: native
subsections:
    - "no": 1
      title: Prolongement des homomorphismes locaux de groupes
      page: 369
      pdf_page: 385
    - "no": 2
      title: Espaces de Hopf
      page: 373
      pdf_page: 389
    - "no": 3
      title: Groupe de Poincaré des groupes topologiques
      page: 375
      pdf_page: 391
    - "no": 4
      title: Revêtements des groupes topologiques
      page: 375
      pdf_page: 391
    - "no": 5
      title: Revêtement universel d’un groupe topologique délaçable
      page: 379
      pdf_page: 395
statements: 21
exercises: 10
content_sha256: 203e5d5d0eceab5aef1b6323c7fb262128d7a978b41b7fa3845c00cd118b9800
translated_from: content/en-mt/ta/IV/03_s3_groupes_de_poincare_des_groupes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: db277372c3e796b13b34997012f2dcc46e40c38ba1cb2d96cac245fe466f7b8f
translation_model: gpt-5-6-mini
translation_run: translate-vi-f5ec005d
glossary_version: 34
glossary_terms_sha256: 91c83f397bdf363c75055213a54e7366f00d0659792f04c665068110a0c1a4ea
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC NHÓM POINCARÉ CỦA CÁC NHÓM TÔPÔ

### 1. Mở rộng các đồng cấu nhóm địa phương

#### Định nghĩa 1 {#ta-iv-s3-def-1 .statement tag=021M}

Cho một nhóm tôpô G và một nhóm $G'$, một đồng cấu địa phương của G vào $G'$ có nghĩa là một ánh xạ $f$ của một lân cận V của phần tử đơn vị của G vào $G'$ sao cho, với mọi cặp điểm $x,y$ của V sao cho $xy\in V$, ta có $f(xy) =f(x)f(y)$.

Nếu $G'$ là một nhóm tôpô và nếu $f$ là một ánh xạ liên tục, ta nói rằng $f$ là một đồng cấu địa phương liên tục (hoặc cấu xạ địa phương của các nhóm tôpô).

Nếu G và $G'$ là các nhóm tôpô, khái niệm đẳng cấu địa phương của G lên $G'$ đã được định nghĩa (TG, III, p. 6, Def. 2). Một đẳng cấu địa phương của G lên $G'$ là một đồng phôi $f$ của một lân cận V của phần tử đơn vị của G lên một lân cận $V'$ của phần tử đơn vị của $G'$ sao cho $f$ và ánh xạ nghịch đảo của $f$ là các đồng cấu địa phương.

#### Mệnh đề 1 {#ta-iv-s3-prop-1 .statement tag=021N}

Cho G và $G'$ là các nhóm tôpô và cho $p: G\rightarrow G'$ là một đồng cấu nhóm. Để $p$ làm cho G là một phủ của $G'$, điều kiện cần và đủ là hạn chế của $p$ trên một lân cận thích hợp của phần tử đơn vị của G phải là một đẳng cấu địa phương của G lên $G'$.

Điều kiện là cần thiết theo Mệnh đề 3 của TG, III, p. 6. Ngược lại, giả sử rằng $p$ cảm sinh một đồng phôi của một lân cận mở V của phần tử đơn vị $e$ của G lên một lân cận $V'$ của phần tử đơn vị của $G'$. Khi đó ánh xạ $p$ là liên tục (TG, III, p. 15, Prop. 23) và mở (TG, III, p. 16, Prop. 24). Ảnh H của $p$ là một nhóm con của $G'$ chứa V, do đó mở và đóng trong $G'$ (TG, III, p. 7, Hệ quả). Gọi N là hạt nhân của $p$; ta có $N\cap V =\{e\}$, do đó N là rời rạc (loc. cit., Prop. 5). Do đó, $p$ làm cho G là một phủ chính của H, với nhóm N (I, p. 100, Hệ quả 3 của Định lý 1). Vì H mở và đóng trong $G'$, không gian $G'$- $(G, p)$ là một phủ.

#### Mệnh đề 2 {#ta-iv-s3-prop-2 .statement tag=021O}

Cho G là một nhóm tôpô liên thông, cho $G'$ là một nhóm và cho $f: V\rightarrow G'$ là một đồng cấu địa phương của G vào $G'$, trong đó V là một lân cận liên thông của phần tử đơn vị của G. Khi đó tồn tại một nhóm tôpô liên thông H, một cấu xạ của các nhóm tôpô $p: H\rightarrow G$ sao cho $(H, p)$ là một phủ của G, và một đồng cấu nhóm $\varphi : H\rightarrow G'$ sao cho tập hợp của $y\in \overset{-1}{p}(V)$ thỏa mãn $f(p(y)) =\varphi (y)$ là một lân cận của phần tử đơn vị trong H.

Nếu $G'$ là một nhóm tôpô và nếu ánh xạ $f$ là liên tục, một đồng cấu như vậy $\varphi$ là liên tục.

#### Bổ đề 1 {#ta-iv-s3-lem-1 .statement tag=021P}

Cho G là một nhóm tôpô và cho V là một lân cận liên thông của phần tử đơn vị $e$ của G. Với mọi lân cận U của $e$ trong G và mọi $x\in V$, tồn tại một số nguyên $n\in \mathbf{N}$ và các phần tử $u_1, . . . , u_n$ trong U sao cho $u_1. . . u_n=x$ và $u_1. . . u_k\in V$ với mọi số nguyên $k$ sao cho $1\leqslant k\leqslant n$.

Có thể giả sử rằng U mở và được chứa trong V. Ký hiệu A là tập hợp các $x\in V$ thỏa mãn điều kiện của bổ đề. Nếu $x\in A$ và $y\in xU\cap V$, thì $y\in A$, do đó AU $\cap V\subset A$; điều này cho thấy A là mở trong V. Cho $x\in V$ sao cho $xU^{-1}\cap A=\not\emptyset$; khi đó $x\in$ AU$\cap V$, do đó $x\in A$. Do đó, nếu $x\in V$ và $x\notin A,xU^{-1}\cap A =\emptyset$ và A là đóng trong V. Vì $e\in A$ và V liên thông, suy ra A = V.

Bây giờ chứng minh mệnh đề. Cho $j$ là ánh xạ $g\mapsto$ $(g, f(g))$ của V vào $G\times G'$ và cho H là nhóm con của $G\times G'$ sinh bởi $j(V)$.

Cho U là một lân cận của $e$ trong G, được chứa trong V. Cho $x\in V$; theo bổ đề 1, tồn tại $u_1, . . . , u_n\in U$ sao cho $x=u_1. . . u_n$ và sao cho $u_1. . . u_k\in V$ với mọi số nguyên $k$ sao cho $1\leqslant k\leqslant n$. Theo quy nạp, ta có $f(u_1. . . u_k) =f(u_1). . . f(u_k)$ với mọi số nguyên $k,1\leqslant k\leqslant n$. Đặc biệt, $j(x)$ thuộc nhóm con sinh bởi $j(U)$. Suy ra H được sinh bởi $j(U)$.

Cho $\mathscr{B}$ là tập hợp các tập con của H có dạng $j(U)$, trong đó U là một lân cận của $e$ trong V. Ta hãy chỉ ra rằng tồn tại duy nhất một tôpô trên H, tương thích với cấu trúc nhóm của nó, sao cho $\mathscr{B}$ là một cơ sở của bộ lọc các lân cận của phần tử đơn vị. Vì vậy, chỉ cần chứng minh rằng tập hợp $\mathscr{B}$ thỏa mãn các điều kiện (GV$'_I$), (GV$'_{II}$) và (GV$'_{III}$) của III, p. 4.

Do đó, cho U là một lân cận của $e$ trong G, được chứa trong V; tồn tại một lân cận $U'$ của $e$ sao cho $U'\cdot U'\subset U$. Với mọi cặp $x, y$ các điểm của $U'$, ta có $xy\in V$ và $f(xy) =f(x)f(y)$. Do đó $j(U')\in \mathscr{B}$ và $j(U')\cdot j(U')\subset j(U)$. Điều này cho thấy điều kiện (GV$'_I$) được thỏa mãn.

Tập hợp $U''= V\cap U^{-1}$ khi đó là một lân cận của $e$ trong V và, với $x\in U''$, ta có $x^{-1}\in U$ và $f(x^{-1}) =f(x)^{-1}$. Do đó $j(U'')^{-1}\subset j(U)$, điều này cho thấy điều kiện (GV$'_{II}$).

Cuối cùng, ta cố định một lân cận U của $e$ trong V sao cho $U = U^{-1}$ và $U^3\subset V$. Gọi W là một lân cận của $e$ trong U và gọi $h= (g, f(g))$ là một phần tử của $j(U)$. Tồn tại một lân cận $W'$ của $e$ được chứa trong W sao cho $gW'g^{-1}\subset W$. Khi đó $j(W')\in \mathscr{B}$ và $hj(W')h^{-1}\subset j(W)$, vì ta có $f(gxg^{-1}) =f(g)f(x)f(g^{-1})$, với $x\in W'$.

Cho $h\in H$. Vì U là một lân cận của $e$ được chứa trong V$,j(U)$ sinh ra H; vì U đối xứng, tồn tại các phần tử $u_1, . . . , u_n$ trong U sao cho $h=j(u_1). . . j(u_n)$. Theo quy nạp theo $n$, tồn tại một lân cận $W'$ của $e$ được chứa trong W sao cho $hj(W')h^{-1}\subset j(W)$. Do đó, điều kiện (GV$'_{III}$) được thỏa mãn.

Sau đó, ta trang bị cho nhóm G tôpô này.

Ta ký hiệu bởi $p: H\rightarrow$ G hạn chế của phép chiếu thứ nhất $G\times G'\rightarrow G$ lên H. Đây là một đồng cấu nhóm. Với mọi lân cận U của $e$ được chứa trong V, tập hợp $\overset{-1}{p}(U)$ chứa lân cận $j(U)$ của phần tử đơn vị của H; do đó $p$ là một đồng cấu liên tục của các nhóm tôpô. Với mọi lân cận U của $e$ được chứa trong V, ta có $p(j(U)) = U$, do đó $p$ là một ánh xạ mở. Vì G liên thông, $p$ là toàn ánh. Hạt nhân của nó là rời rạc vì nó chỉ gặp $j(V)$ tại phần tử đơn vị. Khi đó suy ra từ Hệ quả 3 (I, p. 100) rằng không gian G $(H, p)$ là một phủ.

Gọi $\varphi$ là hạn chế của phép chiếu thứ hai $G\times G'\rightarrow G'$ lên H. Nếu $g\in V$, ta có $(g, f(g)) =j(g)\in j(V)$ và $\varphi (g, f(g)) =f(g)$, do đó $\varphi (y) =f(p(y))$ với $y\in j(V)$.

Hơn nữa, giả sử rằng $G'$ là một nhóm tôpô và ánh xạ $f$ liên tục tại $e$. Khi đó đồng cấu $\varphi$ liên tục tại phần tử đơn vị của H, và do đó là liên tục (TG, III, p. 15, Mệnh đề 23).

#### Hệ quả 1 {#ta-iv-s3-lem-1-cor-1 .statement tag=021Q}

Cho G là một nhóm tôpô đơn liên thông và cho $G'$ là một nhóm. Cho V là một lân cận liên thông của phần tử đơn vị trong G và cho $f: V\rightarrow G'$ là một đồng cấu địa phương. Tồn tại một đồng cấu nhóm duy nhất $h: G\rightarrow G'$ mở rộng $f$. Nếu $G'$ là một nhóm tôpô và nếu ánh xạ $f$ liên tục, thì đồng cấu $h$ liên tục.

Nhóm G liên thông. Cho H$,\varphi$ và $p$ như trong mệnh đề 2. Vì G đơn liên, H là một phủ tầm thường hóa được của G (I, p. 124, định nghĩa 3); vì H liên thông và khác rỗng, ánh xạ $p$ là một đẳng cấu của các nhóm tôpô. Đặt $h=\varphi \circ p^{-1}$; ánh xạ $h$ là một đồng cấu nhóm và tồn tại một lân cận mở U của phần tử đơn vị $e$ của G được chứa trong V sao cho $f|U =h|U$. Từ bổ đề 1 suy ra rằng $f$ và $h$ trùng nhau trên V. Nói cách khác, ánh xạ $h$ mở rộng ánh xạ $f$.

Nếu $G'$ là một nhóm tôpô và nếu ánh xạ $f$ liên tục, thì đồng cấu $\varphi$ liên tục, do đó $h$ cũng vậy.

Hãy chứng minh tính duy nhất của một mở rộng như vậy. Tập hợp các điểm của G tại đó hai đồng cấu của G vào $G'$ trùng nhau là một nhóm con của G. Vì nhóm G liên thông, mọi nhóm con của G chứa một lân cận của phần tử đơn vị đều bằng G (TG, III, p. 8, mệnh đề 6). Tính duy nhất của $h$ được suy ra.

#### Nhận xét 1 {#ta-iv-s3-n1-rem-1 .statement tag=021R}

Khi $G =\mathbf{R}$, hệ quả này suy ra từ mệnh đề 6 của TG, V, p. 3.

#### Hệ quả 2 {#ta-iv-s3-lem-1-cor-2 .statement tag=021S}

Hai nhóm tôpô liên thông địa phương và đơn liên từng địa phương đẳng cấu là đẳng cấu.

Cho G và $G'$ là các nhóm tôpô liên thông địa phương, cho V và $V'$ lần lượt là các lân cận liên thông của phần tử đơn vị của G và của $G'$, và cho $f: V\rightarrow V'$ là một đồng phôi là một đẳng cấu địa phương của G lên $G'$. Theo hệ quả 1, tồn tại một đồng cấu nhóm liên tục duy nhất $\varphi : G\rightarrow G'$ mở rộng $f$ và một đồng cấu nhóm liên tục duy nhất $\varphi ': G'\rightarrow$ G mở rộng $f^{-1}$. Các đồng cấu $\varphi '\circ \varphi$ và Id$_G$ trùng nhau trên một lân cận của $e$ trong G, do đó bằng nhau, vì G liên thông. Tương tự, $\varphi \circ \varphi '=$ Id$_{G'}$, do đó có hệ quả.

#### Hệ quả 3 {#ta-iv-s3-lem-1-cor-3 .statement tag=021T}

Cho G là một nhóm tôpô đơn liên và cho V là một lân cận liên thông của phần tử đơn vị của G. Ta xác định một phép trình bày của G bằng cách lấy làm tập hợp phần tử sinh tập hợp V và làm tập hợp $\mathbf{r}$ các quan hệ họ của các $xyz^{-1}$, trong đó $(x, y, z)$ chạy qua các bộ ba phần tử của V sao cho $xy=z$.

Cho $F(V,\mathbf{r})$ là nhóm thương của nhóm tự do F(V) bởi nhóm con chuẩn nhỏ nhất chứa các phần tử $xyz^{-1}$, trong đó $(x, y, z)\in V\times$ $V\times V$ và $xy=z$ (A, I, p. 86). Ta ký hiệu bởi $f: V\rightarrow F(V,\mathbf{r})$ và $g: F(V,\mathbf{r})\rightarrow G$ các ánh xạ chính tắc. Theo phép dựng, ánh xạ $f$ là một đồng cấu địa phương của G vào $F(V,\mathbf{r})$. Theo hệ quả 1, tồn tại một đồng cấu nhóm duy nhất $\overline{f}: G\rightarrow F(V,\mathbf{r})$ mở rộng $f$. Vì nhóm $F(V,\mathbf{r})$ được sinh bởi $f(V)$, đồng cấu $\overline{f}$ là toàn ánh. Với $x\in V$, ta có $g(\overline{f}(x)) =g(f(x)) =x$; vì V sinh G$,g\circ \overline{f}=$ Id$_G$, điều này chứng minh rằng $\overline{f}$ là đơn ánh. Do đó nó là một đẳng cấu.

### 2. Không gian Hopf

#### Định nghĩa 2 {#ta-iv-s3-def-2 .statement tag=021U}

Một không gian tôpô có điểm cơ sở $(X, e)$ được trang bị một luật hợp thành liên tục $m: X\times X\rightarrow X$ được gọi là một không gian Hopf, sao cho

(i) $m(e, e) =e$;

(ii) tồn tại các đồng luân điểm tại $e$ nối các ánh xạ $x\mapsto m(x, e)$ và $x\mapsto m(e, x)$ với ánh xạ Id$_X$.

Các tính chất (i) và (ii) đôi khi được diễn đạt bằng cách nói rằng $e$ là một phần tử đơn vị sai khác một đồng luân đối với luật hợp thành $m$.

Cần lưu ý rằng có thể tồn tại nhiều phần tử đơn vị sai khác một đồng luân đối với một luật hợp thành liên tục $m$ trên một không gian tôpô X. Ví dụ, với $X =\mathbf{R}$ và $m(x, y) = (x+y)/2$, mọi $x\in \mathbf{R}$ đều là một phần tử đơn vị sai khác một đồng luân.

#### Ví dụ 1 {#ta-iv-s3-n2-exa-1 .statement tag=021V}

Cho G là một nhóm tôpô và $m$ là luật hợp thành của nó. Phần tử đơn vị $e$ của G là một phần tử đơn vị sai khác một đồng luân và $(G, e)$ là một không gian Hopf.

#### Ví dụ 2 {#ta-iv-s3-n2-exa-2 .statement tag=021W}

Cho X là một không gian tôpô và $x$ là một điểm của X. Được trang bị phép ghép các vòng tại $x$, không gian có điểm $(\Omega_x(X), e_x)$ là một không gian Hopf. Thật vậy, trước hết ta có $e_x*e_x=e_x$. Mặt khác, cho $\psi :\mathbf{I}\rightarrow \mathbf{I}$ là hàm được xác định bởi $\psi (t) = 2t$ với $0\leqslant t\leqslant \frac{1}{2}$ và $\psi (t) = 1$ với $\frac{1}{2}\leqslant t\leqslant 1$ (cf. III, p. 291), và cho $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow \mathbf{I}$ là một đồng luân ngặt nối $\psi$ với Id$_{\mathbf{I}}($III, p. 289, ví dụ). Khi đó, với mọi vòng $c\in \Omega_x(X)$, ánh xạ $c\circ \sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ là một đồng luân ngặt nối $c*e_x$ với $c$ trong $\Omega_x(X)$.

Cho $\tau$ là ánh xạ $\Omega_x(X)\times \mathbf{I}\rightarrow \Omega_x(X)$ được xác định bởi $\tau (c, s)(t) =$ $c\circ \sigma (s, t)$. Bây giờ chứng minh rằng $\tau$ liên tục. Theo mệnh đề 1 của III, p. 257, chỉ cần chứng minh rằng ánh xạ $(c, s, t)\mapsto c(\sigma (s, t))$ từ $\Omega_x(X)\times \mathbf{I}\times \mathbf{I}$ vào X là liên tục, hay tương đương, vì $\mathbf{I}\times \mathbf{I}$ là compact, rằng ánh xạ $c\mapsto c\circ \sigma$ từ $\mathscr{C}_c(\mathbf{I}; X)$ vào $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ là liên tục. Khẳng định cuối cùng này suy ra từ bổ đề, I, p. 132, b). Do đó ánh xạ $\tau$ là một đồng luân nối ánh xạ $c\mapsto c*e_x$ với ánh xạ đồng nhất của $\Omega_x(X)$. Ta có $\tau (e_x, s)(t) =x$ với mọi $s,t\in \mathbf{I}$; do đó $\tau$ là một đồng luân điểm tại $e_x$. Ta lập luận tương tự đối với ánh xạ $c\mapsto e_x*c$.

#### Mệnh đề 3 {#ta-iv-s3-prop-3 .statement tag=021X}

Cho $(X, e)$ là một không gian Hopf và $m: X\times X\rightarrow X$ là luật hợp thành của nó. Với mọi vòng $c,c'$ của X tại $e$, ta có:

$$
c'*c\sim c*c'\sim m\circ (c, c')
$$

trong đó $\sim$ ký hiệu quan hệ đồng luân ngặt. Luật hợp thành của nhóm $\pi_1(X, e)$ là đồng cấu thu được bằng cách lấy hợp thành của đẳng cấu chính tắc $\pi_1(X, e)\times \pi_1(X, e)\rightarrow \pi_1(X\times X,(e, e))$ (III, p. 297, hệ quả) và đồng cấu $\pi_1(m,(e, e))$ của $\pi_1(X\times X,(e, e))$ vào $\pi_1(X, e)$. Nhóm $\pi_1(X, e)$ là giao hoán.

Cho $\mu:\pi_1(X, e)\times \pi_1(X, e)\rightarrow \pi_1(X, e)$ là đồng cấu nhóm thu được bằng cách lấy hợp thành của đẳng cấu chính tắc của $\pi_1(X, e)\times \pi_1(X, e)$ lên $\pi_1(X\times$ $X,(e, e))$ và đồng cấu $\pi_1(m,(e, e))$. Ta phải chứng minh rằng

$$
\mu(\gamma , \gamma ') =\gamma \gamma '=\gamma '\gamma \tag{1}
$$

với mọi $\gamma ,\gamma '\in \pi_1(X, e)$. Theo Nhận xét 2 của III, p. 297, ta có:

$$
\mu(\gamma , \gamma ') =\mu(\gamma , \varepsilon_e)\mu(\varepsilon_e, \gamma ') =\mu(\varepsilon_e, \gamma ')\mu(\gamma , \varepsilon_e) \tag{2}
$$

Cho $c\in \Omega_e(X)$ là một đường kín thuộc lớp $\gamma$; ký hiệu $m_1: X\rightarrow X$ là ánh xạ xác định bởi $m_1(x) =m(x, e)$; khi đó $\mu(\gamma , \varepsilon_e)$ là lớp của $m_1\circ c$. Theo định nghĩa của một không gian Hopf, các ánh xạ giữ điểm gốc tại $e$, $m_1$ và Id$_X$, có cùng lớp đồng luân giữ điểm gốc tại $e$. Do đó, các đường kín tại $e$, $m_1\circ c$ và $c$, là đồng luân ngặt (III, p. 296, Hệ quả 1 của Mệnh đề 3) và ta có $\mu(\gamma , \varepsilon_e) =\gamma$. Tương tự, ta chứng minh được $\mu(\varepsilon_e, \gamma ') =\gamma '$. Quan hệ (1) suy ra từ quan hệ (2).

#### Nhận xét {#ta-iv-s3-n2-rem-1 .statement tag=021Y}

Cho $(X, e)$ là một không gian Hopf. Theo Mệnh đề 3, ánh xạ hợp thành các lớp đường, $\pi_1(X, e)\times \pi_1(X, e)\rightarrow$ $\pi_1(X, e)$ là liên tục nếu $\pi_1(X, e)$ được trang bị tôpô thương của tôpô hội tụ đều trên $\Lambda_e(X)$. Thực ra, nó là hợp thành của đẳng cấu liên tục $\pi_1(X, e)\times \pi_1(X, e)\rightarrow \pi_1(X\times X,(e, e))$ (III, p. 298, Nhận xét 3) và ánh xạ liên tục $m_*:\pi_1(X\times X,(e, e))\rightarrow$ $\pi_1(X, e)$ (III, p. 294, Nhận xét 1).

### 3. Nhóm Poincaré của các nhóm tôpô

Nếu G là một nhóm tôpô, với mọi $g\in G$, phép tịnh tiến trái $x\mapsto gx$ là một phép đồng phôi của G lên chính nó (TG, III, p. 2) và nó cảm sinh một đẳng cấu từ $\pi_1(G, e)$ lên $\pi_1(G, g)$.

Cho G là một nhóm tôpô, cho $e$ là phần tử đơn vị của nó và ký hiệu $G_0$ là thành phần liên thông đường của $e$ trong G. Ký hiệu R là quan hệ tương đương trong G mà các lớp tương đương của nó là các thành phần liên thông đường của G, và cho $p: G\rightarrow \pi_0(G)$ là ánh xạ chính tắc. Vì mọi phép tịnh tiến, trái hoặc phải, đều là một phép đồng phôi của G, quan hệ R tương thích bên trái và bên phải với luật nhóm của G. Theo Định lý 2 của A, I, p. 35, nhóm $G_0$ là một nhóm con chuẩn tắc của G, nhóm thương $G/G_0$ bằng $\pi_0(G)$ được trang bị luật hợp thành thương cảm sinh bởi luật của G, và ánh xạ $p$ là một đồng cấu nhóm.

Nhóm $\pi_1(G, e)$ được gọi là nhóm Poincaré của G, và được ký hiệu bởi $\pi_1(G)$. Đơn ánh chính tắc của $G_0$ vào G cảm sinh một đẳng cấu từ $\pi_1(G_0)$ lên $\pi_1(G)$ (III, p. 293, Nhận xét 2).

Cho $g$ là một phần tử của G; phép tịnh tiến phải $\boldsymbol{\delta }_g:x\mapsto xg$ cảm sinh một đẳng cấu $(\boldsymbol{\delta }_g)_*:\pi_1(G)\rightarrow \pi_1(G, g)$. Giả sử rằng $g$ thuộc $G_0$ và cho $b$ là một đường nối $e$ với $g$. Ánh xạ $\sigma : G\times \mathbf{I}\rightarrow G$ xác định bởi $\sigma (x, t) =xb(t)$ là một phép đồng luân nối Id$_G$ với $\boldsymbol{\delta }_g$. Theo mệnh đề 3 của III, p. 295, do đó, với mọi $\alpha \in \pi_1(G)$, ta có $(\boldsymbol{\delta }_g)_*(\alpha ) =$ $\beta^{-1}\alpha \beta$, trong đó $\beta \in \varpi_{e,g}(G)$ là lớp của đường $b$. Nếu $\boldsymbol{\gamma }_g$ ký hiệu phép tịnh tiến trái, $x\mapsto gx$, thì tương tự ta có $(\boldsymbol{\gamma }_g)_*(\alpha ) =\beta^{-1}\alpha \beta$.

Với mọi $g\in G$, ánh xạ Int($g$)$: G\rightarrow G$ cảm sinh một tự đẳng cấu $\pi_1$(Int($g$)) của $\pi_1(G)$. Do đó ta định nghĩa một luật phép toán của G trên $\pi_1(G)$. Với mọi $g\in G$, ta có $\pi_1$(Int($g$)) $= (\boldsymbol{\gamma }_{g^{-1}})_*\circ (\boldsymbol{\delta }_g)_*$, nên nhóm con $G_0$ tác động tầm thường; suy ra rằng có một luật phép toán của $\pi_0(G)$ trên $\pi_1(G)$. Khi G là một nhóm giao hoán, phép toán này là tầm thường, nhưng điều này không phải luôn luôn đúng (IV, p. 459, exerc. 1).

### 4. Các phủ của các nhóm tôpô

#### Mệnh đề 4 {#ta-iv-s3-prop-4 .statement tag=021Z}

Cho $(X, e)$ là một không gian Hopf (IV, p. 373, định nghĩa 2) và cho $m: X\times X\rightarrow X$ là luật hợp thành của nó. Giả sử rằng không gian X là liên thông và liên thông cung địa phương. Cho $X'$ là một phủ liên thông của X; ký hiệu $p$ là phép chiếu của nó và cho $e'$ là một điểm của thớ $X'_e$.

a) Phủ $X'$ là Galois và nhóm các tự đẳng cấu của nó là giao hoán.

b) Tồn tại một luật hợp thành liên tục $m': X'\times X'\rightarrow X'$ và chỉ có một luật như vậy sao cho có $p\circ m'=m\circ (p, p)$ và $m'(e', e') =e'$. Được trang bị luật hợp thành này, không gian có điểm $(X', e')$ là một không gian Hopf.

c) Được trang bị luật hợp thành cảm sinh bởi $m'$, thớ $X'_e$ là một nhóm với phần tử đơn vị $e'$. Ánh xạ của $\pi_1(X, x)$ vào $X'_e$ cho bởi $\gamma \mapsto e'\cdot \gamma$ là một đồng cấu nhóm toàn ánh với hạt nhân $p_*(\pi_1(X', e'))$. Ánh xạ $g\mapsto g(e')$ là một đẳng cấu của nhóm Aut$_X(X')$ lên nhóm $X'_e$.

a) Nhóm $\pi_1(X, e)$ là giao hoán (mệnh đề 3). Vì phủ $X'$ của X là liên thông, nên nó là một phủ Galois và nhóm Aut$_X(X')$ là đẳng cấu với nhóm thương $\pi_1(X, e)/p_*(\pi_1(X', e'))$ (III, p. 312, hệ quả 4 của mệnh đề 2); nhóm này là giao hoán.

b) Ký hiệu $q: X'\times X'\rightarrow X$ là ánh xạ $m\circ (p, p)$. Ánh xạ cần tìm $m'$ là một phép nâng liên tục của $q$ lên $X'$ sao cho $m'(e', e') =e'$. Không gian $X'\times X'$ là liên thông địa phương theo cung; do đó, để chứng minh sự tồn tại của một phép nâng liên tục như vậy, chỉ cần kiểm tra rằng $q_*(\pi_1(X'\times X',(e', e')))$ được chứa trong $p_*(\pi_1(X', e'))$ (III, p. 308, prop. 1). Theo prop. 3, ánh xạ $\pi_1(m,(e, e))$ đồng nhất với luật hợp thành của nhóm $\pi_1(X, e)$ khi đồng nhất $\pi_1(X\times X,(e, e))$ với $\pi_1(X, e)\times \pi_1(X, e)$. Nhóm $q_*(\pi_1(X'\times X',(e', e')))$ do đó bằng nhóm $p_*(\pi_1(X', e'))$, do đó có sự tồn tại của $m'$. Vì $X'\times X'$ là liên thông, tính duy nhất của $m'$ suy ra từ I, p. 34, hệ quả 1 của prop. 11.

Ta hãy chứng minh rằng ánh xạ $m'$ trang bị cho không gian có điểm đánh dấu $(X', e')$ một cấu trúc của không gian Hopf. Cho $m_1: X\rightarrow X$ là ánh xạ $g\mapsto m(g, e)$ và cho $\sigma_1: X\times \mathbf{I}\rightarrow X$ là một đồng luân có điểm đánh dấu tại $x$ nối $m_1$ với Id$_X$. Đặt $\tau =\sigma_1\circ (p$, Id$_{\mathbf{I}}): X'\times \mathbf{I}\rightarrow X$. Ánh xạ $m'_1: X'\rightarrow X'$ xác định bởi $h\mapsto m'(h, e')$ nâng ánh xạ $\tau (\cdot ,0)$; gọi $\tau ': X'\times \mathbf{I}\rightarrow X'$ là phép nâng của $\tau$ là một đồng luân với điểm gốc $m'_1($III, p. 301, prop. 2). Ánh xạ $t\mapsto \tau '(e', t)$ là một phép nâng lên $X'$ của ánh xạ hằng $t\mapsto e$; vì $\tau '(e',0) =e'$, do đó ta có $\tau '(e', t) =e'$ với mọi $t\in \mathbf{I}$. Ánh xạ $\tau '(\cdot ,1)$ khi đó là một phép nâng lên $X'$ của ánh xạ $p$ biến $e'$ thành $e'$. Vì $X'$ là liên thông, Id$_{X'}$ là cấu xạ X duy nhất của $X'$ vào chính nó giữ điểm $e'$ bất động; do đó ta có $\tau '(\cdot ,1) =$ Id$_{X'}$. Điều này chỉ ra rằng $\tau '$ là một đồng luân có điểm đánh dấu tại $e'$ nối ánh xạ $m'_1$ với ánh xạ Id$_{X'}$. Tương tự, tồn tại một đồng luân có điểm đánh dấu tại $e'$ nối ánh xạ $m'_2:h\mapsto m'(e', h)$ với ánh xạ Id$_{X'}$. Điều này chứng minh rằng không gian có điểm đánh dấu $(X', e')$, được trang bị luật hợp thành $m'$, là một không gian Hopf.

c) Vì $X'$ là một phủ liên thông của X, ánh xạ quỹ đạo của $e'$ cảm sinh bởi phép toán của $\pi_1(X, e)$ trên $X'_e$ là toàn ánh và cảm sinh một song ánh của $\pi_1(X, e)/p_*(\pi_1(X', e'))$ lên $X'_e($III, p. 305, Định lý 1).

Cho $c$ và $d$ là các vòng trong X tại $e$, và cho $\gamma$ và $\delta \in \pi_1(X, e)$ là các lớp của chúng. Cho $c'$ và $d'$ là các đường đi có gốc $e'$ trong $X'$ nâng $c$ và $d$. Ta có $e'\cdot \gamma =c'(1)$ và $e'\cdot \delta =d'(1)$ (III, p. 304). Theo Mệnh đề 3 của IV, p. 374, vòng $m\circ (c, d)$ đồng luân chặt với vòng $c*d$; do đó ta có $e'\cdot (\gamma \delta ) =e'\cdot (m\circ (c, d))$. Bây giờ, đường đi $m'\circ (c', d')$ là một nâng có gốc $e'$ của đường đi $m\circ (c, d)$; do đó ta có

$$
e'\cdot (\gamma \delta ) =m'(c'(1), d'(1)) =m'(e'\cdot \gamma , e'\cdot \delta )
$$

Ánh xạ $\gamma \mapsto e'\cdot \gamma$ do đó là một đồng cấu nhóm từ $\pi_1(X, e)$ vào tập hợp $X'_e$ được trang bị luật hợp thành cảm sinh bởi $m'$. Do đó, $X'_e$ là một nhóm đối với luật hợp thành cảm sinh bởi $m'$, và ánh xạ quỹ đạo của $e'$ là một đẳng cấu của nhóm thương $\pi_1(X, e)/p_*(\pi_1(X', e'))$ lên $X'_e$.

Phần cuối của mệnh đề c) khi đó suy ra từ Hệ quả 3 của III, p. 311.

#### Mệnh đề 5 {#ta-iv-s3-prop-5 .statement tag=0220}

Ta giữ lại ký hiệu và các giả thiết của Mệnh đề 4.

a) Nếu $m$ là một luật hợp thành kết hợp ( resp. giao hoán), thì điều tương tự cũng đúng đối với $m'$.

b) Nếu $e$ là một phần tử đơn vị phải ( resp. trái) đối với luật $m$, thì $e'$ là một phần tử đơn vị phải ( resp. trái) đối với luật $m'$.

c) Nếu X là một nhóm tôpô, $m$ là luật hợp thành của nó và $e$ là phần tử đơn vị của nó, luật hợp thành $m'$ trang bị cho $X'$ một cấu trúc nhóm tương thích với tôpô của $X'$, mà $e'$ là phần tử đơn vị. Ánh xạ $p: X'\rightarrow X$ là một đồng cấu nhóm có hạt nhân là rời rạc và được chứa trong tâm của $X'$.

a) Giả sử luật $m$ là kết hợp. Khi đó các ánh xạ từ $X'\times X'\times X'$ vào X lần lượt biến $(h_1, h_2, h_3)$ thành $m(p(h_1), m(p(h_2), p(h_3)))$ và $m(m(p(h_1), p(h_2)), p(h_3))$ là bằng nhau. Các ánh xạ $(h_1, h_2, h_3)\mapsto m'(h_1, m'(h_2, h_3))$ và $(h_1, h_2, h_3)\mapsto m'(m'(h_1, h_2), h_3)$ từ $X'\times X'\times X'$ vào $X'$ là các phép nâng liên tục của chúng và trùng nhau tại điểm $(e', e', e')$. Vì $X'\times X'\times X'$ là liên thông, chúng bằng nhau (I, p. 34, Hệ quả 1 của Mệnh đề 11), do đó luật $m'$ là kết hợp.

Bây giờ giả sử luật $m$ là giao hoán; các ánh xạ $(h_1, h_2)\mapsto m'(h_1, h_2)$ và $(h_1, h_2)\mapsto m'(h_2, h_1)$ là các phép nâng liên tục vào $X'$ của ánh xạ $(h_1, h_2)\mapsto m(p(h_1), p(h_2))$ và trùng nhau tại điểm $(e', e')$. Vì $X'\times X'$ là liên thông, chúng bằng nhau (loc. cit.) và luật $m'$ là giao hoán.

Nếu $e$ là phần tử đơn vị phải (resp. trái) đối với luật $m$, thì ánh xạ $h\mapsto m'(h, e')$ (resp. $h\mapsto m'(e', h)$) từ $X'$ vào $X'$ là một cấu xạ X của các phủ và trùng với Id$_{X'}$ tại điểm $e'$, do đó tại mọi điểm của $X'$, vì $X'$ là liên thông (loc. cit.), do đó b).

Cuối cùng ta chứng minh c). Giả sử rằng X là một nhóm tôpô. Từ những điều đã nêu trên, luật $m'$ là kết hợp và $e'$ là một phần tử đơn vị đối với nó. Gọi $i: X\rightarrow X$ là ánh xạ $g\mapsto g^{-1}$. Nó liên tục (TG, III, p. 1) và đồng cấu $\pi_1(i, e):\pi_1(X, e)\rightarrow \pi_1(X, e)$ chính là ánh xạ $\gamma \mapsto \gamma^{-1}($IV, p. 374, mệnh đề 3). Do đó, nhóm con $(i\circ p)_*(\pi_1(X', e'))$ bằng $p_*(\pi_1(X', e'))$. Theo mệnh đề 1 của III, p. 308, do đó tồn tại một ánh xạ liên tục $i': X'\rightarrow X'$ sao cho $p\circ i'=i\circ p$ và $i'(e') =e'$. Các ánh xạ $h\mapsto m'(h, i'(h))$ và $h\mapsto$ $m'(i'(h), h)$ từ $X'$ vào $X'$ là các nâng lên tới $X'$ của ánh xạ hằng với ảnh $e$ từ $X'$ vào X. Vì vậy chúng là hằng và ảnh của chúng là $e'=m'(e', e')$. Do đó mọi phần tử $h$ của $X'$ đều khả nghịch, với phần tử nghịch đảo là $i'(h)$, điều này chỉ ra rằng $X'$, được trang bị luật hợp thành $m'$, là một nhóm. Theo phép dựng của luật $m'$, ánh xạ $p: X'\rightarrow X$ là một đồng cấu nhóm. Vì các ánh xạ $m'$ và $i'$ liên tục, cấu trúc nhóm của $X'$ tương thích với tôpô của nó (TG, III, p. 1). Thớ $\overset{-1}{p}(e)$ là một nhóm con rời rạc của $X'$ được chứa trong tâm của $X'($I, p. 100, hệ quả 3) và X đẳng cấu với nhóm tôpô thương $X'/\overset{-1}{p}(e)$.

#### Hệ quả {#ta-iv-s3-n4-cor-1 .statement tag=0221}

Cho G là một nhóm tôpô liên thông và liên thông địa phương theo cung. Cho $G'$ là một phủ liên thông của G, cho $p$ là phép chiếu của nó và cho $e'$ là một phần tử của thớ N của phần tử đơn vị $e$ của G. Trang bị cho $G'$ luật hợp thành liên tục duy nhất $m': G'\times G'\rightarrow G'$ sao cho $p\circ m'=m\circ (p, p)$ và $m'(e', e') =e'$. Nếu $i: N\rightarrow G'$ là đơn ánh chính tắc, thì $(G', p, i)$ là một mở rộng trung tâm của G bởi N (A, I, p. 63).

### 5. Phủ phổ quát của một nhóm tôpô phủ được

Cho G là một nhóm tôpô liên thông địa phương theo cung. Các phép tịnh tiến của G là các phép đồng phôi (TG, III, p. 2). Để không gian G là phủ được (IV, p. 340, định nghĩa 2), điều kiện cần và đủ là G có tính chất sau:

Tồn tại một lân cận V của phần tử đơn vị $e$ của G sao cho ảnh của đồng cấu từ $\pi_1(V, e)$ vào $\pi_1(G, e)$ suy ra từ đơn ánh chính tắc được thu gọn thành phần tử đơn vị.

#### Mệnh đề 6 {#ta-iv-s3-prop-6 .statement tag=0222}

Cho G là một nhóm tôpô liên thông và phủ được. Tồn tại một nhóm tôpô $\widetilde{G}$, với phần tử đơn vị $\widetilde{e}$, và một đồng cấu liên tục $p:\widetilde{G}\rightarrow G$ thỏa mãn các khẳng định sau:

a) Không gian $\widetilde{G}$ đơn liên và đơn liên theo cung. Được trang bị ánh xạ $p$, không gian có điểm đặc biệt $(\widetilde{G},\widetilde{e})$ là một phủ phổ quát của không gian có điểm đặc biệt $(G, e)$.

(b) Hạt nhân N của $p$ là một nhóm con rời rạc của $\widetilde{G}$, được chứa trong tâm của $\widetilde{G}$. Đồng cấu nhóm $N\rightarrow$ Aut$_G(\widetilde{G})$ kết hợp, với mỗi $n\in N$, phép dịch phải trong $\widetilde{G}$, là một đẳng cấu nhóm. Đồng cấu của $\pi_1(G)$ vào N kết hợp, với mỗi $\gamma \in \pi_1(G)$, phần tử duy nhất $n$ của N sao cho $\widetilde{e}\cdot \gamma =n$, là một đẳng cấu nhóm.

(c) Nếu $G'$ là một nhóm tôpô, với phần tử đơn vị $e'$, và nếu $p': G'\rightarrow$ G là một đồng cấu nhóm biến $G'$ thành một phủ của G, thì ánh xạ liên tục duy nhất $u:\widetilde{G}\rightarrow G'$ sao cho $u(\widetilde{e}) =e'$ và $p'\circ u=p$ là một đồng cấu nhóm. Được trang bị ánh xạ $u,(\widetilde{G},\widetilde{e})$ là một phủ phổ quát của $(G', e')$.

Theo IV, p. 342, Định lý 1, tồn tại một phủ $(\widetilde{G}, p)$ của G, đơn liên và đơn liên theo cung, Galois với nhóm $\pi_1(G)^{\circ}$, và một điểm $\widetilde{e}$ của $\overset{-1}{p}(e)$ sao cho phủ có điểm $(\widetilde{G},\widetilde{e})$ là một phủ phổ quát của $(G, e)$.

Theo IV, p. 375, Mệnh đề 4 và IV, p. 377, Mệnh đề 5, trên không gian $\widetilde{G}$ tồn tại một cấu trúc nhóm duy nhất tương thích với tôpô của nó sao cho $p$ là một đồng cấu nhóm và $\widetilde{e}$ là một phần tử đơn vị. Theo Mệnh đề 4, nhóm $\widetilde{G}$ thỏa mãn các mệnh đề (a) và (b).

Ta hãy chứng minh mệnh đề (c). Cho $G'$ là một nhóm tôpô và cho $p': G'\rightarrow G$ là một đồng cấu nhóm biến $G'$ thành một phủ của G. Gọi $e'$ là phần tử đơn vị của $G'$. Sự tồn tại và tính duy nhất của một ánh xạ $u:\widetilde{G}\rightarrow G'$ sao cho $p=p'\circ u$ và $u(\widetilde{e}) =e'$ suy ra từ việc $(\widetilde{G},\widetilde{e})$ là một phủ phổ quát của không gian có điểm $(G, e)$. Vì các ánh xạ $p$ và $p'$ là các đồng cấu nhóm toàn ánh, nên $u$ là một đồng cấu nhóm. Được trang bị ánh xạ $u,\widetilde{G}$ là một phủ của $G'($I, p. 81, Mệnh đề 7), do đó $(\widetilde{G},\widetilde{e})$ là một phủ phổ quát của $(G', e')$ (IV, p. 345, Hệ quả 2 của Định lý 1).

Với các giả thiết của mệnh đề, ta sẽ gọi, theo cách nói lạm dụng, $\widetilde{G}$ là một phủ phổ quát của G.

#### Ví dụ {#ta-iv-s3-n5-exa-1 .statement tag=0223}

Mệnh đề 6 áp dụng đặc biệt khi G là một nhóm Lie liên thông trên $\mathbf{R}$ hoặc $\mathbf{C}$. Khi đó trên $\widetilde{G}$ tồn tại một cấu trúc đa tạp giải tích duy nhất sao cho phép chiếu $p:\widetilde{G}\rightarrow G$ là một cấu xạ étale của các đa tạp giải tích (VAR R, §1, 5.8.2, p. 48). Với cấu trúc đa tạp này, $\widetilde{G}$ là một nhóm Lie (LIE, III, p. 113, hệ quả).

#### Chú giải {#ta-iv-s3-n5-sch-1 .statement tag=0224}

Cho G là một nhóm tôpô liên thông và có thể làm đơn liên theo nút, cho $e$ là phần tử đơn vị của nó. Cho $\widetilde{G}$ là một nhóm tôpô đơn liên theo cung, với phần tử đơn vị $\widetilde{e}$, và $p:\widetilde{G}\rightarrow G$ là một đồng cấu nhóm biến $\widetilde{G}$ thành một phủ phổ quát của G. Ta ký hiệu N là hạt nhân của $p$.

Phép tịnh tiến phải $\boldsymbol{\delta }_h$ (tương ứng, phép tịnh tiến trái) bởi một phần tử $h\in N$ là một tự đẳng cấu G của phủ chính $\widetilde{G}$, và ánh xạ $h\mapsto \boldsymbol{\delta }_h$ là một đẳng cấu của nhóm N lên nhóm tự đẳng cấu của phủ chính này.

Với mọi nhóm con K của N, ánh xạ $p':\widetilde{G}/K\rightarrow$ G suy ra từ $p$ là một phủ Galois của G, và Aut$_G(G/K)$ được đồng nhất với nhóm $N/K$. Khi, như trên, các nhóm N và $\pi_1(G)$ được đồng nhất, nhóm $p'_*(\pi_1(\widetilde{G}/K))$ được đồng nhất với nhóm con K của N. Hơn nữa, $\widetilde{G}$ là một phủ của $\widetilde{G}/K$, vì G là liên thông địa phương (I, p. 81, mệnh đề 7).

Ngược lại, mọi phủ liên thông khác rỗng E của G đều G-đẳng cấu với một phủ kiểu này (I, p. 113, định lý 3 và I, p. 111, mệnh đề 10). Thật vậy, xét một điểm $x$ của thớ $E_e$ và gọi $f$ là đồng cấu duy nhất từ $\widetilde{G}$ vào E ánh xạ $\widetilde{e}$ thành $x$. Được trang bị bởi $f,\widetilde{G}$ là một phủ Galois của E; nhóm con Aut$_E(\widetilde{G})$ của Aut$_G(\widetilde{G})$ được đồng nhất với $f^{-1}(x)$ và do đó là một nhóm con của N. Suy ra rằng $f$ cảm sinh một G-đẳng cấu của $\widetilde{G}/f^{-1}(x)$ lên E. Bằng phép chuyển cấu trúc, ta thu được một cấu trúc nhóm tôpô trên E trong đó $x$ là phần tử đơn vị và trong đó ánh xạ $f$ là một đồng cấu toàn ánh. Phép chiếu của G-không gian E khi đó là một đồng cấu nhóm, và luật hợp thành của E do đó là luật hợp thành được xác định bởi mệnh đề 4 của IV, p. 375.

Cho $(E, q)$ và $(E', q')$ là các phủ liên thông của G, cho $x$ là một điểm của $E_e$ và $x'$ là một điểm của $E'_e$. Để tồn tại một cấu xạ G từ E vào $E'$, điều kiện cần và đủ là $p_*(\pi_1(E, x))$ được chứa trong $p'_*(\pi_1(E', x'))$. Nếu điều kiện này được thỏa mãn, khi đó tồn tại một cấu xạ G duy nhất $f: E\rightarrow E'$ sao cho $g(x) =x'($III, p. 311, hệ quả 2 của mệnh đề 1). Nếu E và $E'$ được trang bị các luật hợp thành nhóm mà đối với chúng $q$ và $q'$ là các đồng cấu và $x$ và $x'$ là các phần tử đơn vị, thì ánh xạ $g$ là một đồng cấu nhóm. Thật vậy, $g$ được đồng nhất với đồng cấu chính tắc $\widetilde{G}/p_*(\pi_1(E, x))\rightarrow$ $\widetilde{G}/p'_*(\pi_1(E', x'))$.

#### Mệnh đề 7 {#ta-iv-s3-prop-7 .statement tag=0225}

Để hai nhóm tôpô liên thông không cuộn được là địa phương đẳng cấu, điều kiện cần và đủ là các phủ phổ quát của chúng là các nhóm tôpô đẳng cấu.

Một nhóm tôpô liên thông không cuộn được là địa phương đẳng cấu với phủ phổ quát của nó (IV, p. 369, mệnh đề 1); do đó điều kiện là đủ. Điều kiện đó là cần theo hệ quả 2 của mệnh đề 2 (IV, p. 372), vì phủ phổ quát của một nhóm tôpô liên thông không cuộn được là đơn liên (IV, p. 379, mệnh đề 6).

#### Mệnh đề 8 {#ta-iv-s3-prop-8 .statement tag=0226}

Cho G là một nhóm tôpô liên thông không cuộn được và cho $\widetilde{G}$ là một phủ phổ quát của G. Cho V là một lân cận mở liên thông của phần tử đơn vị $e$ của G sao cho ảnh của đồng cấu chính tắc của $\pi_1(V\cdot V, e)$ vào $\pi_1(G, e)$ được thu gọn thành phần tử đơn vị. Gọi $F(V,\mathbf{r})$ là nhóm được xác định bởi tập sinh V và bởi tập $\mathbf{r}$ gồm các quan hệ $xyz^{-1}$, trong đó $(x, y, z)$ chạy qua tập hợp các phần tử của $V\times V\times V$ sao cho $xy=z$. Gọi $j: V\rightarrow F(V,\mathbf{r})$ là ánh xạ chính tắc.

Tồn tại duy nhất một đẳng cấu $f$ của nhóm $F(V,\mathbf{r})$ lên $\widetilde{G}$ sao cho $f\circ j$ là một phép nâng lên $\widetilde{G}$ của đơn ánh chính tắc của V vào G.

Tập hợp $V\cdot V$ liên thông và mở, do đó liên thông cung địa phương. Gọi $p$ là phép chiếu của $\widetilde{G}$. Tồn tại một tiết diện liên tục $s$ của $p$ trên $V\cdot V$ sao cho $s(e) =\widetilde{e}$, trong đó $\widetilde{e}$ ký hiệu phần tử đơn vị của $\widetilde{G}($III, p. 308, mệnh đề 1). Đặt $\widetilde{V} =s(V)$; tập hợp $\widetilde{V}$ là một lân cận mở liên thông của $\widetilde{e}$ trong $\widetilde{G}$, và $s$ là một phép đồng phôi từ $V\cdot V$ lên $\widetilde{V}\cdot \widetilde{V}$. Các ánh xạ $(x, y)\mapsto s(x)s(y)$ và $(x, y)\mapsto s(xy)$ là các phép nâng lên $\widetilde{G}$ của ánh xạ $(x, y)\mapsto xy$ từ $V\times V$ vào G và trùng nhau tại $(e, e)$; vì $V\times V$ liên thông, chúng trùng nhau trên $V\times V$ (I, p. 34, hệ quả 1). Hơn nữa, nếu $(\widetilde{x},\widetilde{y},\widetilde{z})\in \widetilde{V}\times \widetilde{V}\times \widetilde{V}$, thì các điều kiện $\widetilde{x}\widetilde{y}=\widetilde{z}$ và $p(\widetilde{x})p(\widetilde{y}) =p(\widetilde{z})$ là tương đương. Sự tồn tại của một đẳng cấu $f: F(V,\mathbf{r})\rightarrow \widetilde{G}$ khi đó suy ra từ hệ quả 3 (IV, p. 372) của mệnh đề 2.

Cho $g$ là một đẳng cấu của $F(V,\mathbf{r})$ thỏa mãn các điều kiện của mệnh đề. Đẳng thức $e\cdot e=e$ suy ra rằng $eee^{-1}\in \mathbf{r}$, do đó $j(e)$ là phần tử đơn vị của $F(V,\mathbf{r})$. Vì V liên thông, $g\circ j$ là phép nâng liên tục duy nhất lên $\widetilde{G}$ của đơn ánh chính tắc của V vào G. Do đó, $f$ và $g$ trùng nhau trên $j(V)$. Vì $j(V)$ sinh ra nhóm $F(V,\mathbf{r})$, nên $f=g$.

## BÀI TẬP {#ta-iv-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).
