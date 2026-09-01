---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 4
section_title: Opérateurs partiels
lang: vi
source: ts-iii-v-fr
book_pages: TS IV.224-TS IV.261, TS IV.344-TS IV.352
pdf_pages: 0237-0274, 0357-0365
extraction: native
subsections:
    - "no": 1
      title: Opérateurs partiels
      page: 224
      pdf_page: 237
    - "no": 2
      title: Opérateurs fermés, fermables et à domaine dense
      page: 227
      pdf_page: 240
    - "no": 3
      title: Exemples d’opérateurs partiels
      page: 231
      pdf_page: 244
    - "no": 4
      title: Adjoint
      page: 235
      pdf_page: 248
    - "no": 5
      title: Critères élémentaires pour les opérateurs auto-adjoints
      page: 239
      pdf_page: 252
    - "no": 6
      title: Opérateurs différentiels
      page: 242
      pdf_page: 255
    - "no": 7
      title: Spectre et résolvante
      page: 243
      pdf_page: 256
    - "no": 8
      title: Pseudo-spectre
      page: 250
      pdf_page: 263
    - "no": 9
      title: Opérateurs de multiplication
      page: 252
      pdf_page: 265
    - "no": 10
      title: Extensions auto-adjointes d’un opérateur symétrique
      page: 255
      pdf_page: 268
statements: 74
exercises: 24
content_sha256: c50c9e22cd616e1f241c630b5f2a59cb26e2f83ea28cb1bb0df5add267284c15
translated_from: content/en-mt/ts/IV/04_s4_operateurs_partiels.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 0dde724b75a1681dcc83ba3a9f7f0d845b34c1b80f481582d556c63070e9f580
translation_model: gpt-5.4
translation_run: translate-vi-3e192f17
glossary_version: 34
glossary_terms_sha256: 08c378adb2994133e7f03abf5c681dbaf66a8afd386e1989fa17af3131980d8e
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. TOÁN TỬ BỘ PHẬN

### 1. Toán tử bộ phận

Trong số này, K là một trường giao hoán.

Ta nhắc lại (E, II, §3, p. 9–10) rằng một đồ thị[^1] là một tập hợp mà mọi phần tử đều là các cặp. Nếu A và B là các tập hợp, một sự tương ứng giữa A và B là một bộ ba $(\Gamma ,A,B)$, trong đó Γ là một đồ thị được chứa trong $A\times B$; tập xác định của nó (cũng gọi là miền của nó) là pr$_1$(Γ), và tập hợp các giá trị của nó là pr$_2(\Gamma )$. Một sự tương ứng là một hàm (E, II, p. 13, def. 9) nếu đồ thị của nó là phiếm hàm và nếu tập hợp ban đầu của nó trùng với tập xác định của nó. Mọi tập con của một đồ thị phiếm hàm đều là một đồ thị phiếm hàm.

#### Định nghĩa 1 {#ts-iv-s4-def-1 .statement tag=032J}

Cho E và F là các không gian vectơ trên K. Một toán tử bộ phận $u$ từ E vào F là một sự tương ứng $(\Gamma ,E,F)$ giữa E và F thỏa mãn các điều kiện sau:

(i) Đồ thị Γ là một không gian con vectơ của $E\times F$;

(ii) Đồ thị Γ là phiếm hàm.

Nếu E = F, ta nói rằng $u$ là một toán tử bộ phận trên E.

Cho $u$ là một toán tử bộ phận từ E vào F. Đồ thị Γ của sự tương ứng $u$ được gọi là đồ thị của toán tử bộ phận $u$, và cũng được ký hiệu bởi $\Gamma_u$. Ta ký hiệu bởi $\mathscr{P}(E; F)$ tập hợp các toán tử bộ phận từ E vào F; ta viết đơn giản $\mathscr{P}(E) =\mathscr{P}(E; E)$.

Cho một toán tử bộ phận từ E vào F tương đương với việc cho một không gian con vectơ D của E và một ánh xạ tuyến tính $u$ từ D vào F, toán tử bộ phận liên kết là sự tương ứng $(\Gamma ,E,F)$ trong đó $\Gamma \subset D\times F$ là đồ thị của $u$.

Miền xác định của một toán tử bộ phận $u$ được gọi đơn giản là miền của $u$, và được ký hiệu bởi dom($u$).

Mọi ánh xạ tuyến tính $u$ từ E vào F đều là một toán tử bộ phận từ E vào F.

Nếu $D\subset E$ là một không gian con vectơ, ta sẽ ký hiệu bởi $1_D$ toán tử bộ phận có miền là D mà là ánh xạ đồng nhất trên D, nghĩa là, sự tương ứng $(\Delta_D,E,E)$ trong đó $\Delta_D$ là đường chéo của $D\times D$ (E, II, p. 13, def. 8). Ta sẽ ký hiệu bởi $0_D$ toán tử bộ phận có miền là D mà bằng không trên D, nghĩa là, sự tương ứng $(D\times  \{0\},E,F)$.

Hai toán tử bộ phận $u= (\Gamma ,E,F)$ và $u'= (\Gamma ',E,F)$ từ E vào F là bằng nhau nếu và chỉ nếu dom($u$) $=$ dom($u'$) và nếu các ánh xạ tuyến tính $u$ và $u'$ từ dom($u$) vào F trùng nhau.

Theo E, II, §3, ta định nghĩa các khái niệm sau:

(i) Cho $u$ là một toán tử bộ phận từ E vào F; cho D là miền của nó và $u: D\rightarrow F$ là ánh xạ tuyến tính liên kết. Ảnh của một tập con A của E bởi $u$ là tập con $u(A\cap D)$ của F; nó được ký hiệu đơn giản bởi $u(A)$. Ảnh ngược bởi $u$ của một tập con B của F bởi $u$ là tập con $\overset{-1}{u}(B)$ của D.

Nếu A (resp. B) là một không gian con vectơ của E (resp. của F), thì ảnh của nó bởi $u$ (resp. ảnh ngược của nó) là một không gian con vectơ của F (resp. của E).

Ảnh của $u$ là không gian con vectơ $u(D)$ của F, cũng được ký hiệu bởi Im($u$). Ta nói rằng $u$ là một toán tử bộ phận toàn ánh nếu Im($u$) $= F$. Hạt nhân của $u$ là không gian con vectơ $\overset{-1}{u}(\{0\})$ của E, cũng được ký hiệu bởi Ker($u$). Hạt nhân của $u$ thu về 0 nếu và chỉ nếu ánh xạ tuyến tính $u$ từ dom($u$) vào F là đơn ánh. Khi đó ta nói rằng $u$ là đơn ánh. Nếu $u$ là đơn ánh và toàn ánh, ta nói rằng nó là song ánh.

(ii) Nếu E, F và G là các không gian vectơ trên K và $u= (\Gamma ,E,F)$, $v= (\Gamma ',F,G)$ là các toán tử bộ phận từ E vào F và từ F vào G, tương ứng, thì sự tương ứng hợp thành $v\circ u= (\Gamma '\circ \Gamma ,E,G)$ là một toán tử bộ phận từ E vào G. Miền xác định của nó là $\overset{-1}{u}$(dom($v$)). Nếu H là một không gian vectơ trên K và $w= (\Gamma '',G,H)$ là một toán tử bộ phận từ G vào H, ta có $w\circ (v\circ u) = (w\circ v)\circ u$. Đôi khi người ta sẽ viết $vu$ thay cho $v\circ u$.

(iii) Đặc biệt, với mọi toán tử bộ phận $u$ từ E vào F và mọi $a\in K$, các toán tử bộ phận $au= (a1_F)\circ u$ và $ua=u\circ (a1_E)$ được xác định. Chúng bằng nhau nếu $a\not = 0$, hoặc nếu miền xác định của $u$ bằng E; ta có $u0 = 0_E$ và $0u= 0_{dom(u)}$.

Cho E là một không gian vectơ. Từ những điều nói trên, tập hợp $\mathscr{P}$(E), được trang bị luật hợp thành xác định bởi $(u, v)\mapsto u\circ v$, là một magma kết hợp có đơn vị (A, I, p. 4, Def. 5 and A, I, p. 12, Def. 2) với phần tử đơn vị $1_E$. Với mọi $n\in \mathbf{N}$, người ta ký hiệu bởi $u^n$ hợp thành $\overset{n}{\circ}u$ (A, I, p. 13).

Hơn nữa, người ta định nghĩa các khái niệm sau:

(i) Nếu $u= (\Gamma ,E,F)$ là một toán tử bộ phận từ E vào F, và nếu G là một không gian con của E, thì sự thu gọn của $u$ lên G là toán tử bộ phận $(\Gamma \cap (G\times F),E,F)$ từ E vào F. Miền xác định của nó là dom($u$)$\cap G$; đôi khi người ta sẽ ký hiệu nó bởi $u|G$, khi không sợ nhầm lẫn với sự hạn chế của $u$ lên không gian con G.

(ii) Cho $v$ là một toán tử bộ phận đơn ánh từ F vào E. Khi đó sự tương ứng nghịch đảo $v^{-1}= (\Gamma^{-1},E,F)$ của $v$ là một toán tử bộ phận sao cho dom($v^{-1}$) $=$ Im($v$). Người ta nói rằng $v^{-1}$ là toán tử bộ phận nghịch đảo của $v$. Ta có các đẳng thức $v\circ v^{-1}= 1_{dom(v^{-1})}$ trong $\mathscr{P}(E)$ và $v^{-1}\circ v= 1_{dom(v)}$ trong $\mathscr{P}(F)$. Toán tử bộ phận $v^{-1}$ là đơn ánh và ta có $(v^{-1})^{-1}=v$.

(iii) Cho E, F và G là các không gian vectơ. Cho $u$ (tương ứng $v$) là một toán tử bộ phận đơn ánh từ E vào F (tương ứng từ F vào G). Khi đó toán tử bộ phận $v\circ u$ là đơn ánh và $(v\circ u)^{-1}=u^{-1}\circ v^{-1}$.

(iv) Nếu $u$ và $v$ là các toán tử bộ phận từ E vào F, ta nói rằng $v$ là một mở rộng của $u$, và viết $u\subset v$, nếu đồ thị của $u$ được chứa trong đồ thị của $v$. Điều này kéo theo dom($u$)$\subset$ dom($v$) và $u$ là hạn chế của $v$ trên dom($u$). Quan hệ “ $u\subset v$ ” là một quan hệ thứ tự trong $\mathscr{P}(E; F)$. Ví dụ, ta có $au\subset ua$ với mọi $a\in K$ và mọi $u\in \mathscr{P}(E; F)$.

(v) Cho E là một không gian vectơ trên K và $(F_i)_{i\in I}$ một họ các không gian vectơ trên K. Với $i\in I$, cho $u_i$ là một toán tử bộ phận từ E vào $F_i$. Toán tử bộ phận tích của các $u_i$ là toán tử bộ phận từ E vào không gian vectơ tích của các không gian $F_i$ có miền xác định là giao D của các không gian dom($u_i$) và gán cho $x\in D$ họ $(u_i(x))_{i\in I}$. Nó được ký hiệu bởi $(u_i)_{i\in I}$.

(vi) Cho $A : F\times F\rightarrow F$ là ánh xạ tuyến tính $(x, y)\mapsto x+y$. Cho $u$ và $v$ là các toán tử bộ phận từ E vào F. Tổng $u+v$ là toán tử bộ phận $A\circ (u, v)$ từ E vào F. Miền xác định của nó là dom($u$)$\cap$ dom($v$). Với $u,v,w$ trong $\mathscr{P}(E; F)$, ta có $(u+v) +w=u+ (v+w)$.

Cho G là một không gian vectơ trên K. Với mọi $u$ và $v$ trong $\mathscr{P}(E; F)$ và mọi $w\in \mathscr{P}(F; G)$, ta có $w\circ u+w\circ v\subset w\circ (u+v)$. Nói chung, không có đẳng thức trong công thức này (bài tập 1 của IV, p. 344), nhưng điều đó xảy ra khi miền xác định của $w$ bằng F. Với $w\in \mathscr{P}(G; E)$, ta có $u\circ w+v\circ w= (u+v)\circ w$.

(vii) Cho L là một mở rộng của trường K. Cho E và F là các không gian vectơ trên K và $E_{(L)}= L\otimes_KE, F_{(L)}= L\otimes_KF$ là các không gian vectơ trên L thu được bằng phép mở rộng vô hướng từ K đến L (A, II, p. 82). Với mỗi toán tử bộ phận $u$ từ E vào F, ký hiệu $u_{(L)}$ là toán tử bộ phận từ $E_{(L)}$ vào $F_{(L)}$ mà đồ thị là không gian con vectơ $L\otimes_K\Gamma_u$ của $E_{(L)}\times F_{(L)}$; miền xác định của nó là $L\otimes_K$ dom($u$), và trên miền này nó trùng với ánh xạ tuyến tính duy nhất biến $1\otimes x$ thành $1\otimes u(x)$ với mọi $x\in$ dom($u$).

Cho $v$ là một toán tử bộ phận từ E vào F. Ta có $u\subset v$ khi và chỉ khi $u_{(L)}\subset v_{(L)}$.

(viii) Cho $E_1, F_1, E_2, F_2$ là các không gian vectơ trên K. Cho $u$ (tương ứng $v$) là một toán tử bộ phận từ $E_1$ vào $F_1$ (tương ứng từ $E_2$ vào $F_2$). Ký hiệu $u\otimes v$ là toán tử bộ phận từ $E_1\otimes F_1$ vào $E_2\otimes F_2$ có miền xác định là dom($u$)$\otimes$dom($v$) sao cho $(u\otimes v)(x\otimes y) =u(x)\otimes v(y)$ với mọi $(x, y)\in E_1\times E_2$.

### 2. Các toán tử đóng, các toán tử có thể đóng, và các toán tử có miền xác định trù mật

Trong số này, K ký hiệu một trường tôpô giao hoán (TG, III, p. 54).

#### Định nghĩa 2 {#ts-iv-s4-def-2 .statement tag=032K}

Cho E và F là các không gian vectơ tôpô trên K (EVT, I, p. 1, def. 1). Cho $u\in \mathscr{P}(E; F)$ là một toán tử bộ phận từ E vào F.

Ta nói rằng $u$ là một toán tử có miền xác định trù mật nếu miền xác định của $u$ là trù mật trong E.

Ta nói rằng $u$ là đóng nếu đồ thị của $u$ là đóng trong không gian vectơ tôpô $E\times F$. Ta nói rằng $u$ có thể đóng nếu nó có một mở rộng đóng.

Cho E, F và G là các không gian vectơ tôpô trên K. Mọi mở rộng của một toán tử $u\in \mathscr{P}(E; F)$ có miền xác định trù mật đều có miền xác định trù mật. Hơn nữa, nếu $v\in \mathscr{L}(E; F)$, thì $u+v$ là một toán tử có miền xác định trù mật. Nếu $v: F\rightarrow G$ (tương ứng $w: G\rightarrow E$) là một đẳng cấu của các không gian vectơ tôpô, thì $v\circ u$ (tương ứng $u\circ w$) là một toán tử có miền xác định trù mật.

#### Ví dụ {#ts-iv-s4-n2-exa-1 .statement tag=032L}

Cho E và F là các không gian vectơ tôpô trên K.

1) Giả sử không gian F tách biệt. Cho $u$ là một ánh xạ tuyến tính từ E vào F. Nếu $u$ liên tục, thì toán tử bộ phận $u$ là đóng (TG, I, p. 53, Hệ quả 2). Giả sử thêm rằng K là một trường định giá không rời rạc và E và F là các không gian vectơ tôpô đầy đủ khả mêtric trên K. Theo định lý đồ thị đóng (EVT, I, p. 19, Hệ quả 5), toán tử bộ phận được xác định bởi $u$ khi đó là đóng khi và chỉ khi $u$ liên tục.

2) Giả sử không gian E tách biệt. Cho $v$ là một ánh xạ tuyến tính liên tục đơn ánh từ F vào E. Khi đó toán tử bộ phận $v^{-1}\in \mathscr{P}(E; F) ($xem IV, p. 226) là đóng, vì đồ thị của nó là ảnh của đồ thị của $v$, vốn đóng, dưới đẳng cấu của các không gian vectơ tôpô từ $F\times E$ lên $E\times F$ được xác định bởi $(y, x)\mapsto (x, y)$.

#### Mệnh đề 1 {#ts-iv-s4-prop-1 .statement tag=032M}

Cho E và F là các không gian vectơ tôpô trên K. Một toán tử bộ phận $u$ từ E vào F là có thể đóng được nếu và chỉ nếu bao đóng của đồ thị $\Gamma_u$ của $u$ trong $E\times F$ là một đồ thị phiếm hàm. Khi đó tồn tại duy nhất một toán tử bộ phận $v$ từ E vào F có đồ thị là $\overline{\Gamma}_u$, và nó là mở rộng đóng nhỏ nhất của $u$.

Nếu bao đóng của đồ thị của $u$ trong $E\times F$ là một đồ thị phiếm hàm, thì đó là đồ thị của một toán tử bộ phận, và toán tử này là một mở rộng đóng của $u$, nên $u$ là có thể đóng được. Đảo lại, giả sử rằng $u\subset w$ với $w$ đóng. Bao đóng $\overline{\Gamma}_u$ của đồ thị của $u$ trong $E\times F$ được chứa trong $\Gamma_w$, do đó $\Gamma_u$ là một đồ thị phiếm hàm.

Khẳng định cuối cùng suy ra từ sự kiện là nếu $w$ là một mở rộng đóng của $u$, thì đồ thị của $w$ chứa $\overline{\Gamma}_u$.

#### Định nghĩa 3 {#ts-iv-s4-def-3 .statement tag=032N}

Cho E và F là các không gian vectơ tôpô trên K. Cho $u$ là một toán tử có thể đóng được từ E vào F. Toán tử đóng có đồ thị là $\Gamma_u$ được gọi là bao đóng của $u$. Nó được ký hiệu là $\overline{u}$.

#### Nhận xét {#ts-iv-s4-n2-rem-1 .statement tag=032O}

Cho E và F là các không gian vectơ tôpô trên K. Cho $u$ là một toán tử có thể đóng được từ E vào F. Miền xác định của bao đóng của $u$ được chứa trong bao đóng của miền xác định của $u$ trong E. Nói chung, nó phân biệt với bao đóng này (bài tập 1 của IV, p. 344, b)).

Nếu $u\in \mathscr{P}(E; F)$ là có thể đóng được và dom($u$) $= E$, thì $u=\overline{u}$ là đóng, vì khi đó dom($\overline{u}$) $=$ dom($u$).

#### Mệnh đề 2 {#ts-iv-s4-prop-2 .statement tag=032P}

Cho $K =\mathbf{R}$ và cho E và F là các không gian vectơ tôpô trên $\mathbf{R}$. Cho $u$ là một toán tử bộ phận từ E vào F. Khi đó $u$ có miền xác định trù mật (tương ứng là đóng, là có thể đóng được) nếu và chỉ nếu $u_{(\mathbf{C})}$ có miền xác định trù mật (tương ứng là đóng, là có thể đóng được).

Giả sử rằng miền xác định của $u$ là trù mật trong E. Mọi lân cận của 0 trong $E_{(\mathbf{C})}$ đều chứa một lân cận dạng $V +iV$ (TVS, II, p. 65), trong đó V là một lân cận của 0 trong E, và do đó chứa một phần tử của miền xác định của $u_{(\mathbf{C})}$; vì thế toán tử bộ phận này có miền xác định trù mật. Đảo lại cũng đúng vì ánh xạ từ $E_{(\mathbf{C})}$ vào E gắn $x$ với $x+iy$ với mọi $(x, y)\in E\times E$ là liên tục và toàn ánh.

Đồ thị của $u_{(\mathbf{C})}$ được đồng nhất với không gian vectơ tôpô phức hoá của đồ thị của $u$. Do đó nó là đóng trong $E_{(\mathbf{C})}\times E_{(\mathbf{C})}$ nếu đồ thị của $u$ là đóng trong $E\times E$. Đảo lại, ta có $\Gamma_u= \Gamma_{u_{(\mathbf{C})}}\cap (E\times E)$ trong $E_{(\mathbf{C})}\times E_{(\mathbf{C})}$; vì $E\times E$ là đóng trong $E_{(\mathbf{C})}\times E_{(\mathbf{C})}$, toán tử bộ phận $u$ là đóng khi $u_{(\mathbf{C})}$ là đóng.

Một toán tử bộ phận $v$ từ E vào F là một mở rộng của $u$ khi và chỉ khi $v_{(\mathbf{C})}$ là một mở rộng của $u_{(\mathbf{C})}$, do đó toán tử bộ phận $u_{(\mathbf{C})}$ là khả đóng nếu $u$ là khả đóng. Ngược lại, nếu $u_{(\mathbf{C})}$ là khả đóng, thì toán tử bộ phận $u$ cũng vậy, vì $\Gamma_u= \Gamma_{u_{(\mathbf{C})}}\cap (E\times E)$, khi đó là đồ thị của một phiếm hàm (mệnh đề 1).

#### Bổ đề 1 {#ts-iv-s4-lem-1 .statement tag=032Q}

Cho E, F và G là các không gian vectơ tôpô trên K. Cho $u$ là một toán tử đóng từ E vào F.

a) Với mọi $v\in \mathscr{L}(E; F)$, toán tử bộ phận $u+v$ là đóng.

b) Với mọi $v\in \mathscr{L}(G; E)$, toán tử bộ phận $u\circ v$ là đóng.

Ta chứng minh a). Cho $\gamma$ là ánh xạ $(x, y)\mapsto (x, y-v(x))$ từ $E\times F$ vào chính nó; nó liên tục. Với mọi $(x, y)\in E\times F$, ta có $\gamma (x, y)\in \Gamma_u$ khi và chỉ khi $x\in$ dom($u$) và $y=u(x) +v(x)$, nghĩa là $\overset{-1}{\gamma}(\Gamma_u) = \Gamma_{u+v}$. Mệnh đề được suy ra.

Ta chứng minh b). Ánh xạ $\eta = (v,1_F)$ từ $G\times F$ vào $E\times F$ là liên tục; với mọi $(z, y)\in G\times F$, ta có $\eta (z, y) = (v(z), y)$, do đó $\overset{-1}{\eta}(\Gamma_u) = \Gamma_{u\circ v}$. Mệnh đề được suy ra.

Cho E và F là các không gian vectơ tôpô trên K, với F tách biệt. Cho $a\in K$. Nếu $u\in \mathscr{P}(E; F)$ là khả đóng, thì $au$ cũng vậy. Nếu $a\not = 0$, ta có $\overline{au}=au$, và $u$ đóng khi và chỉ khi $au$ đóng. Nếu $a= 0$, bao đóng của $au$ là $0_{\overline{dom(u)}}$, và $au$ bằng $0_{dom(\overline{u})}$; vì vậy có thể xảy ra trường hợp $u$ đóng nhưng $au$ thì không.

#### Mệnh đề 3 {#ts-iv-s4-prop-3 .statement tag=032R}

Cho E và F là các không gian vectơ tôpô trên K, với F tách biệt. Cho $u$ là một toán tử bộ phận đóng từ E vào F. Hạt nhân của $u$ là một không gian con đóng của E.

Thật vậy, hạt nhân của $u$ là ảnh ngược của không gian con đóng $\Gamma_u\cap (E\times  \{0\})$ của $E\times F$ bởi ánh xạ tuyến tính liên tục $x\mapsto (x,0)$ từ E vào $E\times F$.

Trong phần còn lại của No. này, giả sử K là một trường có trị không rời rạc.

#### Định nghĩa 4 {#ts-iv-s4-def-4 .statement tag=032S}

Cho E và F là các không gian chuẩn trên K và cho $u$ là một toán tử bộ phận từ E vào F. Với $x$ trong dom($u$), ta viết

$$
\|x\|_u= (\|x\|^2_E+\|u(x)\|^2_F)^{1/2}
$$

Ánh xạ $x\mapsto  \|x\|_u$ thu được là một chuẩn trên dom($u$). Không gian chuẩn do đó thu được được ký hiệu là $E_u$.

#### Nhận xét {#ts-iv-s4-n2-rem-2 .statement tag=032T}

Cho E và F là các không gian chuẩn trên K và cho $u$ là một toán tử bộ phận từ E vào F.

1) Đơn ánh chính tắc của $E_u$ vào E là liên tục vì ta có $\|x\|\leqslant \|x\|_u$ với mọi $x\in E$. Đặc biệt, mọi không gian con của dom($u$) đóng trong E đều đóng trong $E_u$.

2) Nếu E và F là các không gian Hilbert, thì không gian $E_u$ là một không gian tiền Hilbert, vì chuẩn trên $E_u$ xuất phát từ dạng Hermit dương

$$
(x, y)\mapsto (x|y)_u=\langle x|y\rangle +\langle u(x)|u(y)\rangle
$$

trên dom($u$).

#### Mệnh đề 4 {#ts-iv-s4-prop-4 .statement tag=032U}

Cho E và F là các không gian Banach (tương ứng, các không gian Hilbert), và cho $u$ là một toán tử bộ phận từ E vào F. Khi đó $u$ đóng khi và chỉ khi không gian định chuẩn $E_u$ là một không gian Banach (tương ứng, một không gian Hilbert).

Chỉ cần xét trường hợp các không gian Banach. Chuẩn của $E_u$ thu được, bằng phép chuyển cấu trúc nhờ ánh xạ tuyến tính song ánh $(x, y)\mapsto x$ từ $\Gamma_u$ lên dom($u$), từ chuẩn thu được bằng cách hạn chế lên không gian con $\Gamma_u$ của chuẩn $(x, y)\mapsto (\|x\|^2_E+\|y\|^2_F)^{1/2}$ trên không gian Banach $E\oplus F$. Vì vậy không gian $E_u$ là một không gian Banach khi và chỉ khi không gian con $\Gamma_u$ của $E\oplus F$ là đóng.

Nếu $u$ và $v$ lần lượt là các toán tử bộ phận từ E vào F và từ F vào G, và nếu $u$ đóng, thì toán tử bộ phận $v\circ u$ nói chung không đóng, ngay cả khi $v$ liên tục (bài tập 1 của IV, p. 344, c)). Tuy vậy ta có điều kiện đủ sau đây:

#### Bổ đề 2 {#ts-iv-s4-lem-2 .statement tag=032V}

Cho E, F và G là các không gian định chuẩn trên K, với F là một không gian Banach. Cho $u$ là một toán tử bộ phận đóng từ E vào F và cho $v\in \mathscr{L}(F; G)$. Nếu tồn tại $C\in \mathbf{R}_+$ sao cho

$$
\|u(x)\|\leqslant C(\|x\|+\|(v\circ u)(x)\|)
$$

với mọi $x\in$ dom($v\circ u$) $=$ dom($u$), nghĩa là, nếu ánh xạ tuyến tính $x\mapsto u(x)$ từ $E_{v\circ u}$ vào F là liên tục, thì $v\circ u$ đóng.

Đặt $w=v\circ u$. Cho $(x_n, w(x_n))_{n\in\mathbf{N}}$ là một dãy trong đồ thị của $w$ hội tụ trong $E\times G$. Gọi $x$ là giới hạn của dãy $(x_n)$. Giả thiết suy ra rằng khi đó dãy $(u(x_n))_{n\in\mathbf{N}}$ là một dãy Cauchy trong F; nó hội tụ đến một phần tử $y$ của F. Vì $u$ đóng, do đó ta có $x\in$ dom($u$) và $y=u(x)$. Khi ấy $w(x_n) =v(u(x_n))$ tiến tới $v(y) =$ $v(u(x))$ vì $v$ liên tục, do đó đồ thị của $w$ là đóng.

Cho $u$ là một toán tử bộ phận đóng trên một không gian Banach E và F là một không gian con của dom($u$). Nếu F trù mật trong không gian Banach $E_u$, thì hạn chế của $u$ lên F là có thể đóng được, và bao đóng của nó bằng $u$. Khi đó người ta nói rằng F là một lõi của $u$.

### 3. Ví dụ về các toán tử bộ phận

Trong số này, $K =\mathbf{R}$ hoặc $\mathbf{C}$.

#### Ví dụ 1 {#ts-iv-s4-n3-exa-1 .statement tag=032W}

Cho X là một không gian tôpô compact địa phương và cho $\mu$ là một độ đo dương trên X. Cho $p_1$ và $p_2$ là các phần tử cố định của $[1,+\infty [$.

Cho $g$ là một hàm $\mu$-đo được trên X nhận giá trị trong K. Gọi D là không gian con của $\mathscr{L}_K^{p_1}(X, \mu)$ gồm các hàm $f$ trong $\mathscr{L}_K^{p_1}(X, \mu)$ sao cho $gf\in \mathscr{L}_K^{p_2}(X, \mu)$. Ánh xạ tuyến tính từ D vào $\mathscr{L}_K^{p_2}(X, \mu)$ được định nghĩa bởi $f\mapsto gf$ xác định một toán tử bộ phận từ $\mathscr{L}_K^{p_1}(X, \mu)$ vào $\mathscr{L}_K^{p_2}(X, \mu)$, được ký hiệu là $m_g$.

Không gian con vectơ các hàm $\mu$-không đáng kể trong $\mathscr{L}_K^{p_1}(X, \mu)$ được chứa trong D, và ảnh dưới $m_g$ của một hàm $\mu$-không đáng kể lại là $\mu$-không đáng kể. Ta sẽ ký hiệu bởi $\widetilde{m}_g$ toán tử bộ phận từ $L^{p_1}_K(X, \mu)$ vào $L^{p_2}_K(X, \mu)$ suy ra từ $m_g$ bằng cách chuyển qua thương. Nó được gọi là toán tử phép nhân bởi $g$ từ $L^{p_1}_K(X, \mu)$ vào $L^{p_2}_K(X, \mu)$. Các hàm $g_1$ và $g_2$ địa phương bằng nhau $\mu$-hầu khắp nơi xác định cùng một toán tử phép nhân.

#### Mệnh đề 5 {#ts-iv-s4-prop-5 .statement tag=032X}

Toán tử phép nhân $\widetilde{m}_g$ từ $L^{p_1}_K(X, \mu)$ vào $L^{p_2}_K(X, \mu)$ là một toán tử đóng với miền xác định trù mật.

Trước hết ta chứng minh rằng toán tử bộ phận $\widetilde{m}_g$ là đóng. Cho $(f_n, h_n)_{n\in\mathbf{N}}$ là một dãy trong $\mathscr{L}_K^{p_1}(X, \mu)\times \mathscr{L}_K^{p_2}(X, \mu)$ sao cho dãy $(f_{\widetilde{n}},\widetilde{h}_n)$ các lớp của $f_n$ và $h_n$ thuộc đồ thị của $\widetilde{m}_g$ và hội tụ trong $L^{p_1}_K(X, \mu)\times L^{p_2}_K(X, \mu)$ khi $n$ tiến ra vô cùng. Cho $(f, h)$ là một cặp trong $\mathscr{L}_K^{p_1}(X, \mu)\times \mathscr{L}_K^{p_2}(X, \mu)$ sao cho cặp $(\widetilde{f} ,\widetilde{h})$ các lớp của chúng là giới hạn của $(\widetilde{f}_n,\widetilde{h}_n)$.

Tồn tại một dãy $(f_{n_k})_{k\in\mathbf{N}}$ rút ra từ dãy $(f_n)_n$ sao cho $f_{n_k}(x)$ hội tụ tới $f(x)$ với $\mu$-gần như mọi $x$ (INT, IV, p. 131, § 3, n$^o4$, th. 3). Điều này kéo theo $h_{n_k}(x) =g(x)f_{n_k}(x)$ hội tụ $\mu$-gần như khắp nơi tới $g(x)f(x)$. Hơn nữa dãy $(h_{n_k})$ hội tụ tới $h$ trong không gian $\mathscr{L}_K^{p_2}(X, \mu)$. Do đó các hàm $h$ và $gf$ bằng nhau $\mu$-gần như khắp nơi (loc. cit.). Vậy $\widetilde{f}$ thuộc miền xác định của $\widetilde{m}_g$ và $\widetilde{h}=\widetilde{m}_g(\widetilde{f})$. Điều này chứng tỏ rằng $\widetilde{m}_g$ đóng.

Ta hãy chứng minh rằng miền xác định của $\widetilde{m}_g$ là trù mật trong $L^{p_1}_K(X, \mu)$. Chỉ cần kiểm tra rằng các lớp của những hàm $f\in \mathscr{K}(X; K)$ thuộc bao đóng của miền xác định của $\widetilde{m}_g$ trong $L^{p_1}_K(X, \mu)$. Cho $f\in \mathscr{K}(X; K)$ và gọi $\widetilde{f}$ là lớp của nó trong $L^{p_1}_K(X, \mu)$. Với mọi số nguyên $n\in \mathbf{N}$, gọi $\varphi_n$ là hàm đặc số của tập hợp các phần tử $x\in X$ sao cho $|g(x)|\leqslant n$, và đặt $f_n=f \varphi_n$. Khi đó $|gf_n|\leqslant n|f|$, mà hàm này thuộc $\mathscr{L}_K^{p_2}(X, \mu)$, nên $f_n$ thuộc miền xác định của $\widetilde{m}_g$. Với mọi phần tử $x$ của X, dãy $(f_n(x))_{n\in\mathbf{N}}$ hội tụ tới $f(x)$ khi $n\rightarrow +\infty$; hơn nữa, ta có $|f_n|\leqslant |f|$, mà hàm này thuộc $\mathscr{L}_K^{p_1}(X, \mu)$. Theo định lý Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6), dãy các lớp của $f_n$ hội tụ tới $\widetilde{f}$ trong $L^{p_1}_K(X, \mu)$. Vậy lớp của $f$ thuộc bao đóng của miền xác định của $\widetilde{m}_g$.

Trong mệnh đề sau, giả sử rằng $p_1=p_2= 2$.

#### Mệnh đề 6 {#ts-iv-s4-prop-6 .statement tag=032Y}

a) Cho $g'$ là một hàm $\mu$-đo được trên X sao cho $|g|\leqslant |g'|$. Ta có dom($\widetilde{m}_{g'}$)$\subset$ dom($\widetilde{m}_g$) và dom($\widetilde{m}_{g'}$) là một lõi của toán tử bộ phận $\widetilde{m}_g$;

b) Cho F là một không gian con của $\mathscr{L}_K^2(X, \mu)$ mà giao của nó với $\mathscr{K}(X; K)$ là trù mật trong $\mathscr{K}(X; K)$ và mà ảnh G của nó trong $L^2_K(X, \mu)$ được chứa trong dom($\widetilde{m}_g$). Nếu $|g|^2$ địa phương $\mu$-khả tích, thì $\mathscr{K}(X; K)$ được chứa trong miền xác định của $\widetilde{m}_g$ và G là một lõi của $m_g$.

Ta hãy chứng minh a). Nếu $f\in \mathscr{L}_K^2(X, \mu)$ thuộc miền xác định của $m_{g'}$, sao cho $f g'\in \mathscr{L}_K^2(X, \mu)$, thì giả thiết suy ra rằng $f g\in \mathscr{L}_K^2(X, \mu)$, do đó có kết quả.

Ta hãy chứng minh rằng dom($\widetilde{m}_{g'}$) là một lõi của $\widetilde{m}_g$, nghĩa là miền xác định của $\widetilde{m}_{g'}$ là trù mật trong không gian Hilbert $E_{\widetilde{m}_g}$. Cho $h\in \mathscr{L}_K^2(X, \mu)$

mà lớp $\widetilde{h}$ của nó thuộc $E_{\widetilde{m}_g}$ và trực giao với dom($\widetilde{m}_{g'}$). Điều đó có nghĩa là

$$
(\widetilde{h}|\widetilde{h}')_{\widetilde{m}_g}=\int_Xh h'(1 +|g|^2)d\mu= 0
$$

đối với mọi hàm $h'\in \mathscr{L}_K^2(X, \mu)$ mà lớp $\widetilde{h}'$ của nó thuộc dom($\widetilde{m}_{g'}$).

Cho C là một tập con compact của X và $\varphi$ là hàm đặc trưng của nó. Cho $n\in \mathbf{N}$. Ký hiệu bởi $\varphi_n$ hàm đặc trưng của tập $\mu$-khả tích $C_n$ gồm các $x\in C$ sao cho $|h(x)|\leqslant n$ và đặt $h'_n=\varphi_nh$. Lớp của $h'_n$ thuộc miền xác định của $\widetilde{m}_{g'}$ vì $|g'h'_n|\leqslant n\varphi$; do đó

$$
0 =\int_X\overline{h}h'_n(1 +|g|^2)d\mu=\int_X|h|^2\varphi_n(1 +|g|^2)d\mu
$$

Điều này suy ra rằng $h$ bằng không với $\mu$-gần khắp mọi $x\in C_n$ và vì thế, do $n$ là tùy ý, rằng $h$ bằng không với $\mu$-gần khắp mọi $x\in C$. Cuối cùng suy ra rằng $h$ bằng không $\mu$-gần khắp nơi, vì C là tùy ý và $h$ là vừa phải (INT, V, p. 9, § 1, n$^o3$, cor.).

Bây giờ ta xét mệnh đề b). Vì $|g|^2$ địa phương $\mu$-khả tích, hàm $f g$ thuộc $\mathscr{L}_K^2(X, \mu)$ nếu $f\in \mathscr{K}(X; K)$, do đó $\mathscr{K}(X; K)$ được chứa trong miền xác định của $\widetilde{m}_g$.

Cho $h\in \mathscr{L}_K^2(X, \mu)$ mà lớp $\widetilde{h}$ của nó thuộc $E_{m_g}$ và trực giao với G. Khi đó ta có

$$
0 = (\widetilde{h}|\widetilde{h}')_{\widetilde{m}_g}=\int_Xh\overline{h}'(1 +|g|^2)d\mu
$$

đối với mọi $h'\in F$ có lớp $\widetilde{h}'$. Theo giả thiết về F, điều này có nghĩa là độ đo $h(1 +|g|^2)\cdot \mu$ bằng không, do đó $h$ bằng không $\mu$-hầu khắp mọi nơi vì $h$ là vừa phải.

Cho $p$ là một số thực $\geqslant 1$. Cho $h$ là một phần tử của $\mathscr{L}_K^{\infty}(X, \mu)$. Toán tử phép nhân $\widetilde{m}_h$ bởi $h$ là một tự đồng cấu của $L^p_K(X, \mu)$(IV, p. 186, No.$^o5$). Giả sử rằng tập Y gồm các $x\in X$ sao cho $h(x) = 0$ là địa phương $\mu$-không đáng kể. Khi đó tự đồng cấu $\widetilde{m}_h$ là đơn ánh (Bổ đề 7 của IV, p. 186). Ta ký hiệu bởi $h^{-1}$ hàm trên X bằng 0 trên Y và bằng $x\mapsto 1/h(x)$ trên X- Y. Toán tử bộ phận nghịch đảo $\widetilde{m}^{-1}_h$ là toán tử phép nhân bởi $h^{-1}$ từ $L^p_K(X, \mu)$ vào $L^p_K(X, \mu)$, nghĩa là, $\widetilde{m}^{-1}_h=\widetilde{m}_{h^{-1}}$. Thật vậy, ảnh của $\widetilde{m}_h$ là không gian các lớp của các hàm $g\in \mathscr{L}_K^p(X, \mu)$ có dạng $g=hf$ với $f\in \mathscr{L}_K^p(X, \mu)$. Điều kiện này tương đương với $g(x)/h(x) =f(x)$ đối với mọi $x\in X$- Y và $g(x) = 0$ nếu $x\in Y$. Điều này kéo theo rằng miền xác định của $\widetilde{m}^{-1}_h$ trong $L^p_K(X, \mu)$ là miền xác định của $\widetilde{m}_{h^{-1}}$, và đẳng thức $\widetilde{m}^{-1}_h=\widetilde{m}_{h^{-1}}$ là đúng.

Trong phần sau, đôi khi ta sẽ ký hiệu đơn giản bởi $m_h$ toán tử phép nhân bộ phận bởi $h$ từ $L^{p^1}_K(X, \mu)$ vào $L^{p_2}_K(X, \mu)$.

#### Ví dụ 2 {#ts-iv-s4-n3-exa-2 .statement tag=032Z}

Cho E là một không gian Hilbert trên K và $B = (e_i)_{i\in I}$ là một cơ sở trực chuẩn của E. Cho $(\lambda_i)_{i\in I}$ là một họ các phần tử của K. Cho D là không gian con vectơ của E gồm các phần tử $x\in E$ sao cho họ $(\lambda_i\langle e_i|x\rangle )_{i\in I}$ là khả tổng bình phương trong K. Không gian D là trù mật trong E vì nó chứa vectơ $e_i$ đối với mọi $i\in I$. Toán tử bộ phận $u$ có miền xác định D cho bởi

$$
x\mapsto \sum_{i\in I}\lambda_i\langle e_i|x\rangle e_i
$$

được gọi là một toán tử bộ phận đường chéo trong cơ sở B, và $(\lambda_i)_{i\in I}$ được gọi là họ các giá trị riêng của $u$.

Toán tử $u$ là đóng. Thật vậy, cho $(x_n, u(x_n))_{n\in\mathbf{N}}$ là một dãy các phần tử của đồ thị của $u$ hội tụ trong $E\times E$, và cho $(x, y)$ là giới hạn của nó. Khi đó $\langle e_i|x_n\rangle  \rightarrow  \langle e_i|x\rangle$ đối với mọi $i\in I$ và

$$
\langle e_i|u(x_n)\rangle =\lambda_i\langle e_i|x_n\rangle  \rightarrow  \langle e_i|y\rangle
$$

với mọi $i\in I$. Do đó, $\lambda_i\langle e_i|x\rangle =\langle e_i|y\rangle$ với mọi $i\in I$, điều đó chứng tỏ rằng $x\in D$ và $u(x) =y$, nghĩa là $u$ là đóng.

Ví dụ này thực ra là một trường hợp riêng của ví dụ trước, áp dụng cho không gian tôpô X = I được trang bị tôpô rời rạc và độ đo đếm $\mu$, vì E được đồng nhất với không gian $\ell^2(I) = L^2(I, \mu)$ bởi ánh xạ $x\mapsto (\langle e_i|x\rangle )_{i\in I}$ (EVT, V, p. 23, hệ quả 2) và khi đó $u$ được đồng nhất với toán tử phép nhân $m_{\lambda}$, trong đó $\lambda$ là hàm $i\mapsto \lambda_i$.

#### Ví dụ 3 {#ts-iv-s4-n3-exa-3 .statement tag=0330}

Tập hợp $\mathbf{N}_{\mathbf{R}}=\mathbf{N}\cup  \{\infty , \omega \}$ được trang bị thứ tự toàn phần được mô tả trong VAR, R2, p. 10, sao cho $n <\infty < \omega$ với mọi $n\in \mathbf{N}$. Cho $r\in \mathbf{N}_{\mathbf{R}}$. Cho $n\in \mathbf{N}$ và cho U là một tập con mở của $\mathbf{R}^n$. Cho $k\in \mathbf{N}$ sao cho $k\leqslant r$. Cho $(n_{\alpha})_{|\alpha|\leqslant k}$ là một họ các phần tử của $\mathscr{C}^r$(U), trong đó các đa chỉ số được xét thuộc $\mathbf{N}^n$. Họ $(n_{\alpha})$ xác định một toán tử vi phân vô hướng D cấp $\leqslant k$ trên U (xem VAR, R2, 14.1.6, 14.1.4). Với mọi số nguyên $m$ sao cho $k\leqslant m\leqslant r$, toán tử vi phân D xác định một ánh xạ tuyến tính từ $C^m(U)$ vào $C^{m-k}(U)$ biến $f\in C^m(U)$ thành

$$
D(f) =\sum_{|\alpha|\leqslant k}n_{\alpha}\partial^{\alpha}(f)
$$

Cùng công thức đó xác định một ánh xạ tuyến tính liên tục từ $\mathscr{D}(U)$ vào $\mathscr{D}'(U)$ (định nghĩa 2 của IV, p. 208).

#### Định nghĩa 5 {#ts-iv-s4-def-5 .statement tag=0331}

Cho E là một không gian con vectơ của $\mathscr{D}'(U)$ chứa $\mathscr{D}(U)$. Một toán tử vi phân liên kết với D trên E là bất kỳ toán tử bộ phận nào trên E là một mở rộng của toán tử bộ phận có miền xác định $\mathscr{D}(U)$ được xác định bởi $\varphi \mapsto D(\varphi )$.

Chẳng hạn, giả sử rằng các hệ số $n_{\alpha}$ là các hàm bị chặn trên U. Cho $\mu$ là độ đo Lebesgue trên U. Nếu $p$ là một phần tử của $[1,+\infty [$, khi đó có thể định nghĩa trên $L^p(U)$ một toán tử vi phân liên kết với D có miền xác định là không gian Sobolev $W^{k,p}(U)$ (No. 14 của IV, p. 221), vì trong trường hợp này ta có $n_{\alpha}\partial^{\alpha}(f)\in L^p(U)$ với mọi $f\in W^{k,p}(U)$ và mọi $|\alpha |\leqslant k$.

### 4. Liên hợp

Trong số này, K là một trong các trường $\mathbf{R}$ hoặc $\mathbf{C}$, và E và F chỉ các không gian Hilbert trên K.

Cho $u$ là một toán tử có miền xác định trù mật từ E vào F. Gọi D là miền xác định của $u$. Với $y\in F$, gọi $\lambda_y$ là dạng tuyến tính trên D sao cho $\lambda_y(x) =\langle y|u(x)\rangle$ với mọi $x\in D$. Ta ký hiệu bởi $D^*$ tập hợp các vectơ $y\in F$ sao cho $\lambda_y$ liên tục trên D. Đó là một không gian con vectơ của F. Cho $y\in D^*$; vì D trù mật trong E, dạng tuyến tính $\lambda_y$ kéo dài theo một cách duy nhất thành một dạng tuyến tính liên tục trên E, mà ta vẫn ký hiệu là $\lambda_y$. Theo EVT, V, p. 15, Định lý 3, tồn tại một phần tử duy nhất $u^*(y)$ trong E sao cho $\lambda_y(x) =\langle u^*(y)|x\rangle$ với mọi $x\in E$. Ánh xạ $y\mapsto u^*(y)$ là tuyến tính từ $D^*$ vào E.

#### Định nghĩa 6 {#ts-iv-s4-def-6 .statement tag=0332}

Toán tử bộ phận từ F vào E, có miền xác định là $D^*$ và được xác định bởi $y\mapsto u^*(y)$, được gọi là liên hợp của $u$. Nó được ký hiệu là $u^*$.

#### Nhận xét {#ts-iv-s4-n4-rem-9 .statement tag=0333}

Như vậy $y\in D^*$ khi và chỉ khi tồn tại $c\in \mathbf{R}_+$ sao cho $|\langle y|u(x)\rangle |\leqslant c\|x\|$ với mọi $x\in D$. Khi đó phần tử $u^*(y)$ được đặc trưng bởi quan hệ

$$
\langle y|u(x)\rangle =\langle u^*(y)|x\rangle \tag{1}
$$

với mọi $x\in D$. Khi đó ta có $|\langle y|u(x)\rangle |\leqslant \|u^*(y)\| \|x\|$ với mọi $x\in D$.

Trong trường hợp $u$ là một ánh xạ tuyến tính liên tục từ E vào F, liên hợp của nó theo nghĩa của định nghĩa trước trùng với liên hợp được định nghĩa trong EVT, V, p. 38, Định nghĩa 1, vì trong trường hợp này $D^*$ bằng F.

Cho $v\in \mathscr{P}(E; F)$ sao cho $u\subset v$. Khi đó $v^*\subset u^*$.

Cho $v\in \mathscr{P}(E; F)$ sao cho $u+v$ có miền xác định trù mật. Khi đó toán tử bộ phận $v$ có miền xác định trù mật và ta có $u^*+v^*\subset (u+v)^*$. Nói chung không có đẳng thức (bài tập 9 của IV, p. 347). Nếu $v\in \mathscr{L}(E; F)$, thì $u+v$ có miền xác định trù mật và $(u+v)^*=u^*+v^*$. Điều này xảy ra, chẳng hạn, nếu F = E và nếu $v=\lambda 1_E$ với $\lambda \in K$.

Cho G là một không gian Hilbert trên K và cho $v\in \mathscr{P}(F; G)$ là một toán tử có miền xác định trù mật. Nếu $v\circ u$ có miền xác định trù mật, thì $u^*\circ v^*\subset (v\circ u)^*$. Nói chung không có đẳng thức (loc. cit.). Nếu $u$ (tương ứng $v$) là một đẳng cấu, thì $v\circ u$ có miền xác định trù mật và ta có $(v\circ u)^*=u^*\circ v^*$. Điều này xảy ra, chẳng hạn, nếu E = F (tương ứng F = G) và $u=\lambda 1_E$ (tương ứng $v=\lambda 1_F$) với $\lambda \in K^*$.

Gọi $s$ là đẳng cấu đẳng cự của các không gian Hilbert từ $E\oplus F$ vào $F\oplus E$ được xác định bởi $s(x, y) = (-y, x)$ với mọi $(x, y)\in E\oplus F$.

#### Mệnh đề 7 {#ts-iv-s4-prop-7 .statement tag=0334}

Cho $u$ là một toán tử bộ phận có miền xác định trù mật từ E vào F.

a) Đồ thị của $u^*$ bằng $s(\Gamma^{\circ}_u) =s(\Gamma_u)^{\circ}$;

b) Toán tử bộ phận $u^*$ là đóng;

c) Hạt nhân của $u^*$ là trực giao của ảnh của $u$.

Đặt $W =s(\Gamma_u)^{\circ}$. Vì ánh xạ tuyến tính $s$ là unita, ta có $W =s(\Gamma^{\circ}_u)$.

Ta có $(y, x)\in W$ khi và chỉ khi

$$
\langle (y, x)|(-u(x'), x')\rangle = 0
$$

với mọi $x'\in$ dom($u$), nghĩa là, khi

$$
\langle y|u(x')\rangle =\langle x|x'\rangle
$$

với mọi $x'\in$ dom($u$). Khi $y\in$ dom($u^*$) và $x=u^*(y)$, tính chất này được thỏa mãn (x. công thức (1), p. 236). Ngược lại, nếu điều kiện này được thỏa mãn, suy ra $|\langle y|u(x')\rangle |\leqslant \|x\| \|x'\|$ với mọi $x'\in$ dom($u$), do đó suy ra $y$ thuộc dom($u^*$); khi đó ta có $u^*(y) =x$. Vậy $W = \Gamma_{u^*}$.

Toán tử $u^*$ là đóng, vì không gian $s(\Gamma_u)^{\circ}$ là đóng trong $F\oplus E$.

Hãy chứng minh mệnh đề c). Nếu $y$ trực giao với ảnh của $u$, thì dạng tuyến tính $\lambda_y:x\mapsto  \langle y|u(x)\rangle$ trên D bằng không, do đó $y\in$ dom($u^*$) và $u^*(y) = 0$. Ngược lại, giả sử $y\in$ dom($u^*$). Khi đó $u^*(y) = 0$ khi và chỉ khi $y$ trực giao với $u(x)$ với mọi $x\in D$ (công thức (1), p. 236).

#### Mệnh đề 8 {#ts-iv-s4-prop-8 .statement tag=0335}

Cho $u$ là một toán tử có miền xác định trù mật từ E vào F. Khi đó $u^*$ có miền xác định trù mật khi và chỉ khi $u$ là khả đóng. Trong trường hợp này, bao đóng $\overline{u}$ của $u$ bằng $u^{**}$, và toán tử liên hợp của $\overline{u}$ bằng $u^*$.

Theo Mệnh đề 7, toán tử bộ phận $u^*$ là đóng. Giả sử rằng miền xác định $D^*$ của $u^*$ là trù mật trong F. Gọi $u^{**}$ là toán tử liên hợp của $u^*$; đó là một toán tử bộ phận đóng từ E vào F. Ta sẽ chứng minh rằng $u\subset u^{**}$, điều này sẽ kéo theo rằng $u$ là khả đóng. Cho $x\in$ dom($u$). Theo định nghĩa của $u^*$, các dạng tuyến tính trên $D^*$ được cho bởi $y\mapsto  \langle x|u^*(y)\rangle$ và $y\mapsto  \langle u(x)|y\rangle$ là bằng nhau; do đó $x\in$ dom($u^{**}$) và $u^{**}(x) =u(x)$, do đó có mệnh đề cần chứng minh.

Ngược lại, giả sử rằng $u$ là khả đóng; ta có $\Gamma_{\overline{u}}=\overline{\Gamma}_u$ (Mệnh đề 1 của IV, p. 228). Cho $y\in F$ là một vectơ trực giao với dom($u^*$). Khi đó phần tử $(y,0)$ của $F\oplus E$ thuộc phần bù trực giao của đồ thị của $u^*$. Nhưng, theo Mệnh đề 7, a), ta có

$$
\Gamma^{\circ}_{u^*}= (s(\Gamma_u)^{\circ})^{\circ}=s(\Gamma_u) =s(\Gamma_u)
$$

Vậy suy ra rằng $(0, y)\in \Gamma_{\overline{u}}$, do đó $y=\overline{u}(0) = 0$. Vì phần bù trực giao của dom($u^*$) thu về 0, không gian dom($u^*$) là trù mật trong F.

Sau cùng, Mệnh đề 7, áp dụng cho $u^*$, kéo theo rằng

$$
\Gamma_{u^{**}}=s^{-1}(\Gamma^{\circ}_{u^*}) =s^{-1}(s(\Gamma^{\circ \circ}_u)) =\overline{\Gamma}_u
$$

do đó $u^{**}=\overline{u}$, rồi $\overline{u}^*= (u^*)^{**}=\overline{u^*}=u^*$ vì $u^*$ là đóng.

#### Hệ quả {#ts-iv-s4-n4-cor-1 .statement tag=0336}

Nếu $u$ là một toán tử bộ phận đóng với miền xác định trù mật từ E vào F, thì $u^*$ có miền xác định trù mật và ta có $u^{**}=u$.

#### Định nghĩa 7 {#ts-iv-s4-def-7 .statement tag=0337}

Cho $u$ là một toán tử bộ phận trên E. Ta nói rằng $u$ là đối xứng nếu $u$ có miền xác định trù mật và nếu $u^*$ là một mở rộng của $u$. Ta nói rằng $u$ là tự liên hợp nếu $u$ có miền xác định trù mật và $u^*=u$. Ta nói rằng $u$ là cốt yếu tự liên hợp nếu nó là khả đóng và nếu bao đóng $\overline{u}$ của $u$ là tự liên hợp.

Ta nói rằng $u$ là một toán tử bộ phận bị chặn dưới nếu $u$ là đối xứng và nếu tồn tại một số thực $c$ sao cho $\langle x|u(x)\rangle \geqslant c\|x\|^2$ với mọi $x$ thuộc miền xác định của $u$. Khi đó ta nói rằng $c$ là một cận dưới của $u$. Nếu $c= 0$, ta cũng nói rằng $u$ là một toán tử bộ phận dương.

Ta ký hiệu bởi $\mathscr{A}(E)$ tập hợp các toán tử bộ phận tự liên hợp trên E.

#### Nhận xét 1 {#ts-iv-s4-n4-rem-1 .statement tag=0338}

Để một toán tử $u$ với miền xác định trù mật trên E là đối xứng, điều kiện cần và đủ là có

$$
\langle x|u(y)\rangle =\langle u(x)|y\rangle \tag{2}
$$

với mọi $(x, y)\in$ dom($u$)$^2$. Thực ra công thức này cho thấy miền xác định của $u$ được chứa trong miền xác định của $u^*$, và khi đó $u^*$ và $u$ trùng nhau trên miền xác định của $u$. Đặc biệt, suy ra rằng $\langle x|u(x)\rangle  \in \mathbf{R}$ với mọi $x\in$ dom($u$).

Như sẽ thấy trong các ví dụ khác nhau, công thức (2) thường có thể được kiểm tra bằng một phép tính trực tiếp. Mặt khác, việc xác định chính xác miền xác định của toán tử liên hợp, điều duy nhất cho phép biết một toán tử đối xứng có tự liên hợp hay không, có thể rất tinh tế.

#### Nhận xét 2 {#ts-iv-s4-n4-rem-2 .statement tag=0339}

Một toán tử bộ phận tự liên hợp là tự liên hợp cốt yếu (xem mệnh đề 8).

#### Nhận xét 3 {#ts-iv-s4-n4-rem-3 .statement tag=033A}

Cho $u$ là một toán tử bộ phận đối xứng trên E. Toán tử $u$ là khả đóng (mệnh đề 7, b)). Nó thỏa mãn dom($u$)$\subset$ dom($u^*$), và $u$ là tự liên hợp khi và chỉ khi dom($u$) $=$ dom($u^*$). Hơn nữa, bao đóng $\overline{u}$ của $u$ là đối xứng vì $\overline{u}\subset u^*=\overline{u}^*$ (mệnh đề 8).

#### Nhận xét 4 {#ts-iv-s4-n4-rem-4 .statement tag=033B}

Giả sử $K =\mathbf{C}$. Cho $u\in \mathscr{P}(E; E)$ là một toán tử bộ phận có miền xác định trù mật. Điều kiện $\langle x|u(x)\rangle  \in \mathbf{R}$ với mọi $x\in$ dom($u$) kéo theo rằng $u$ là đối xứng (EVT, V, p. 2, nhận xét); đặc biệt, nếu $\langle x|u(x)\rangle  \in \mathbf{R}_+$ với mọi $x\in$ dom($u$), thì $u$ là dương.

#### Nhận xét 5 {#ts-iv-s4-n4-rem-5 .statement tag=033C}

Cho $u$ và $v$ là các toán tử bộ phận đối xứng trên E. Nếu $u$ là tự liên hợp và nếu $u\subset v$, thì $v\subset v^*\subset u^*=u$, do đó $u=v$.

#### Nhận xét 6 {#ts-iv-s4-n4-rem-6 .statement tag=033D}

Một toán tử bộ phận tự liên hợp cốt yếu $u$ là đối xứng, vì $u\subset \overline{u}$ kéo theo $\overline{u}=\overline{u}^*\subset u^*$, do đó $u\subset u^*$.

#### Nhận xét 7 {#ts-iv-s4-n4-rem-7 .statement tag=033E}

Cho $u$ và $v$ là các toán tử bộ phận đối xứng trên E. Nếu $u+v$ có miền xác định trù mật, chẳng hạn nếu $u$ hoặc $v$ thuộc $\mathscr{L}$ (E), thì $u+v$ là đối xứng. Nói chung, toán tử bộ phận $u+v$ không tự liên hợp, ngay cả nếu $u$ và $v$ đều như vậy (bài tập 9 của IV, p. 347).

#### Nhận xét 8 {#ts-iv-s4-n4-rem-8 .statement tag=033F}

Cho $u$ là một toán tử bộ phận đối xứng trên E. Một số thực $c$ là một cận dưới của $u$ khi và chỉ khi toán tử $u-c\cdot 1_E$ là dương.

#### Bổ đề 3 {#ts-iv-s4-lem-3 .statement tag=033G}

Giả sử rằng $K =\mathbf{R}$. Cho $u$ là một toán tử bộ phận có miền xác định trù mật từ E vào F.

a) Liên hợp của $u_{(\mathbf{C})}$ là $(u^*)_{(\mathbf{C})}$;

b) Giả sử E = F; toán tử bộ phận $u$ là đối xứng (resp. tự liên hợp) khi và chỉ khi toán tử bộ phận $u_{(\mathbf{C})}$ là đối xứng (resp. tự liên hợp).

Ta hãy chứng minh a). Cho $y\in F_{(\mathbf{C})}$ và viết $y=y_1+iy_2$ với $y_1,y_2\in F$. Với mọi $(x_1, x_2)\in E\times E$, ta có

$$
\langle u_{(\mathbf{C})}(x_1+ix_2)|y\rangle =\langle u(x_1)|y_1\rangle +i\langle u(x_1)|y_2\rangle
$$

$$
-i\langle u(x_2)|y_1\rangle +\langle u(x_2)|y_2\rangle
$$

Nếu $y\in$ dom($u^*$)$_{(\mathbf{C})}$, suy ra $y\in$ dom(($u_{(\mathbf{C})}$)$^*$) và $u^*_{(\mathbf{C})}(y) = (u_{(\mathbf{C})})^*(y)$, do đó $u^*_{(\mathbf{C})}\subset (u_{(\mathbf{C})})^*$.

Ngược lại, giả sử rằng $y$ thuộc dom(($u_{(\mathbf{C})}$)$^*$). Lấy $x_2= 0$ (resp. $x_1= 0$) trong công thức trên, ta kiểm tra được rằng $y_1\in$ dom($u^*$) (resp. rằng $y_2\in$ dom($u^*$)), do đó $y\in$ dom($u^*$)$_{(\mathbf{C})}$.

Mệnh đề a) suy ra rằng $u_{(\mathbf{C})}$ là đối xứng (resp. tự liên hợp) nếu $u$ là như vậy.

Ngược lại, giả sử rằng $u_{(\mathbf{C})}$ là đối xứng. Quan hệ $\langle u(x)|y\rangle =\langle x|u(y)\rangle$ với mọi $(x, y)\in$ dom($u_{(\mathbf{C})}$)$\times$ dom($u_{(\mathbf{C})}$) suy ra rằng $u$ là đối xứng khi lấy $x$ và $y$ trong không gian con dom($u$) của dom($u_{(\mathbf{C})}$). Nếu $u_{(\mathbf{C})}$ là tự liên hợp, điều vừa nói trên chứng minh rằng $u$ là đối xứng; vì dom($u^*$) $=$ dom($u^*_{(\mathbf{C})}$)$\cap F$, mệnh đề a) suy ra rằng dom($u^*$) $=$ dom($u_{(\mathbf{C})}$)$\cap F =$ dom($u$), vậy nên $u$ là tự liên hợp.

### 5. Các Tiêu chuẩn Sơ cấp cho các Toán tử Tự Liên hợp

#### Mệnh đề 9 {#ts-iv-s4-prop-9 .statement tag=033H}

Cho $v\in \mathscr{L}(F; E)$ là một ánh xạ tuyến tính liên tục đơn ánh từ F vào E mà ảnh là trù mật trong E. Liên hợp của $v$ là một ánh xạ tuyến tính liên tục đơn ánh từ E vào F và ta có $(v^*)^{-1}= (v^{-1})^*$. Đặc biệt, nếu E = F, tự đồng cấu $v$ là Hermit khi và chỉ khi toán tử bộ phận $v^{-1}$ là tự liên hợp.

Toán tử riêng phần $v^{-1}$ là một toán tử đóng với miền xác định trù mật từ E vào F (Ví dụ 2 của IV, p. 228), và liên hợp $v^*$ của $v$ là một ánh xạ tuyến tính liên tục từ E vào F; nó đơn ánh, vì ảnh của $v$ trù mật trong E (EVT, V, p. 41, mệnh đề 4). Gọi $s$ (resp. $s'$) là đẳng cấu đẳng cự $(x, y)\mapsto (-y, x)$ từ $E\oplus F$ lên $F\oplus E$ (resp. đẳng cấu đẳng cự $(y, x)\mapsto (-x, y)$ từ $F\oplus E$ lên $E\oplus F$), và gọi $\iota$ (resp. $\iota '$) là đẳng cấu đẳng cự $(y, x)\mapsto (x, y)$ từ $F\oplus E$ lên $E\oplus F$ (resp. đẳng cấu đẳng cự $(x, y)\mapsto (y, x)$ từ $E\oplus F$ lên $F\oplus E$). Khi đó $s\circ \iota =-\iota '\circ s'$, do đó

$$
\Gamma_{(v^{-1})^*}=s(\Gamma_{v^{-1}})^{\circ}=s(\iota (\Gamma_v))^{\circ}=-\iota '(s'(\Gamma_v))^{\circ}=-\iota '(\Gamma_{v^*}) = \Gamma_{(v^*)^{-1}}
$$

theo mệnh đề 7 của IV, p. 236. Mệnh đề được suy ra.

#### Mệnh đề 10 (Hellinger–Toeplitz) {#ts-iv-s4-prop-10 .statement tag=033I}

Cho $u$ là một toán tử riêng phần đối xứng trên không gian Hilbert E. Nếu miền xác định của $u$ bằng E, thì $u\in \mathscr{L}(E)$ và $u$ là Hermit.

Thật vậy, toán tử riêng phần $u$ là có thể đóng được (mệnh đề 8 của IV, p. 237), và do đó là đóng vì miền xác định của nó là E (IV, p. 228, Nhận xét). Khi đó ta kết luận bằng cách viện dẫn EVT, I, p. 19, hệ quả 5.

#### Hệ quả {#ts-iv-s4-n5-cor-1 .statement tag=033J}

Cho $u$ là một toán tử riêng phần đối xứng trên E. Nếu toán tử riêng phần $u$ cảm sinh một ánh xạ tuyến tính song ánh từ dom($u$) lên E, thì $u$ là tự liên hợp.

Thật vậy, toán tử riêng phần nghịch đảo $u^{-1}$ của $u$ là đối xứng với miền xác định E (mệnh đề 9), nên $u^{-1}$ là một phần tử tự liên hợp của $\mathscr{L}(E)$ (mệnh đề 10), và do đó $u$ là Hermit (mệnh đề 9).

#### Mệnh đề 11 {#ts-iv-s4-prop-11 .statement tag=033K}

Cho $u$ là một toán tử riêng phần đối xứng trên E, và $\lambda \in \mathbf{C}$. Nếu $u+\lambda 1_E$ và $u+\lambda 1_E$ là toàn ánh, thì $u$ là tự liên hợp.

Chỉ cần chứng minh rằng dom($u^*$)$\subset$ dom($u$). Cho $x\in$ dom($u^*$). Theo giả thiết, tồn tại $y\in$ dom($u$) sao cho $u(y) +\lambda y=u^*(x) +\lambda x$. Ta sẽ chứng minh rằng $y=x$. Với mọi $z\in$ dom($u$), ta có

$$
\langle (u+\lambda 1_E)(z)|x\rangle =\langle z|(u^*+\overline{\lambda}1_E)(x)\rangle
$$

$$
=\langle z|(u+\overline{\lambda}1_E)(y)\rangle =\langle (u+\lambda 1_E)(z)|y\rangle
$$

vì $u$ là đối xứng. Vì toán tử $u+\lambda 1_E$ là toàn ánh, quả thật ta có $y=x$, nên $x\in$ dom($u$).

Ta sẽ thấy về sau (xem mệnh đề 17 của IV, p. 248) rằng nếu $\lambda \in \mathbf{C}-\mathbf{R}$, thì đảo lại là đúng.

#### Mệnh đề 12 {#ts-iv-s4-prop-12 .statement tag=033L}

Cho $u$ là một toán tử đóng có miền xác định trù mật từ E vào F. Toán tử bộ phận $u^*\circ u$ trên E là tự liên hợp và dương. Miền xác định của nó là một lõi đối với $u$.

Ta ký hiệu bởi $v$ toán tử bộ phận $1_E+u^*\circ u$. Miền xác định của nó là dom($u^*\circ u$), được chứa trong dom($u$). Với mọi $x\in$ dom($u$) và $y\in$ dom($v$), ta có $u(y)\in$ dom($u^*$) và

$$
\langle x|v(y)\rangle =\langle x|y\rangle +\langle x|(u^*\circ u)(y)\rangle =\langle x|y\rangle +\langle u(x)|u(y)\rangle \tag{3}
$$

$$
\langle y|v(y)\rangle =\|y\|^2+\|u(y)\|^2 \tag{4}
$$

Công thức (4) kéo theo rằng toán tử bộ phận $v$ là đơn ánh. Hơn nữa, theo mệnh đề 7 của IV, p. 236, a), ta có $F\oplus E = \Gamma_{u^*}\oplus s(\Gamma_u)$. Cho $x\in E$. Tồn tại $y'\in$ dom($u^*$) và $x'\in$ dom($u$) sao cho

$$
(0, x) = (y', u^*(y')) + (-u(x'), x') = (y'-u(x'), x'+u^*(y'))
$$

Do đó ta có $y'=u(x')$, suy ra $x'\in$ dom($u^*\circ u$) $=$ dom($v$) và

$$
x=x'+u^*(y') =x'+ (u^*\circ u)(x') =v(x')
$$

Vì vậy, toán tử bộ phận $v$ trên E là toàn ánh, và gây ra một ánh xạ tuyến tính song ánh từ dom($v$) lên E.

Cho $x\in E$ trực giao với dom($v$). Viết $x=v(x')$ với $x'\in$ dom($v$). Theo công thức (4), ta được

$$
0 =\langle x'|x\rangle =\langle x'|v(x')\rangle =\|x'\|^2+\|u(x')\|^2
$$

do đó $x'= 0$, rồi suy ra $x= 0$. Vậy miền xác định của $v$ là trù mật trong E.

Toán tử bộ phận $v$ có miền xác định trù mật; nó là song ánh và công thức (3) cho thấy nó đối xứng. Áp dụng hệ quả của mệnh đề 10, suy ra $v$ là tự liên hợp. Do đó, $u^*\circ u=v-1_E$ là tự liên hợp. Hơn nữa, công thức

$$
\langle x|(u^*\circ u)(x)\rangle =\|u(x)\|^2
$$

với mọi $x\in$ dom($u^*\circ u$) cho thấy rằng $u^*\circ u$ là dương.

Sau cùng, cho $y\in E_u$ trực giao với dom($u^*\circ u$). Tồn tại một phần tử $x$ trong miền xác định của $u^*\circ u$ sao cho $y=v(x) =x+ (u^*\circ u)(x)$. Khi đó ta có $0 = (x|y)_u=\langle y|y\rangle$, do đó $y= 0$.

### 6. Toán tử vi phân

Cho $n\in \mathbf{N}$ và U là một tập mở trong $\mathbf{R}^n$. Ta trang bị cho $\mathbf{R}^n$ và U độ đo Lebesgue ký hiệu bởi $\mu$.

Cho $k\in \mathbf{N}$ và $h\in \mathbf{N}$ sao cho $h\geqslant k$. Cho D là một toán tử vi phân vô hướng trên U cấp $\leqslant k$, với các hệ số $(n_{\alpha})_{|\alpha|\leqslant k}$ thuộc lớp $C^h$ trên U. Giả sử rằng với mọi $\alpha$ sao cho $|\alpha |\leqslant k$ và mọi $\beta$ sao cho $0\leqslant \beta \leqslant \alpha$, hàm $\partial^{\beta}n_{\alpha}$ bị chặn trên U.

Cho $^tD$ là toán tử vi phân vô hướng trên U chuyển vị của D (VAR, R2, 14.3.2); nó có cấp $\leqslant k$ và thuộc lớp $C^{h-k}$; với $\varphi \in \mathscr{D}$(U), ta có

$$
^tD(\varphi ) =\sum_{|\alpha|\leqslant k}(-1)^{|\alpha|}\partial^{\alpha}(\overline{n}_{\alpha}\varphi )
$$

(loc. cit.); đặc biệt, các hệ số của $^tD$ bị chặn trên U.

Ta ký hiệu bởi $D_-$ toán tử bộ phận trên $L^2(U)$ với miền xác định $\mathscr{D}(U)$ được xác định bởi

$$
\varphi \mapsto D(\varphi ) =\sum_{|\alpha|\leqslant k}n_{\alpha}\partial^{\alpha}\varphi \tag{5}
$$

Cho $H_D$ là không gian các $f\in L^2(U)$ sao cho phân phối

$$
D(f) =\sum_{|\alpha|\leqslant k}n_{\alpha}\partial^{\alpha}f
$$

thuộc $L^2(U)$; ta ký hiệu bởi $D_+$ toán tử bộ phận với miền xác định $H_D$ được xác định bởi $f\mapsto D(f)$.

Vì ta có $\partial^{\alpha}f\in L^2(U)$ nếu $f\in H^k(U)$ và $|\alpha |\leqslant k$, không gian Sobolev $H^k(U)$ được chứa trong $H_D$; nói chung, các không gian này phân biệt.

Ta có $D_-\subset D_+$, và đó là các toán tử vi phân liên kết với D trên $L^2(U)$ (đn. 5 của IV, p. 235).

#### Mệnh đề 13 {#ts-iv-s4-prop-13 .statement tag=033M}

Cho $u$ là một toán tử bộ phận trên $L^2(U)$. Nếu $D_-\subset u\subset D_+$, thì $u$ đóng được và $(^tD)_-\subset u^*\subset (^tD)_+$.

Cho $\varphi$ và $\psi$ thuộc $\mathscr{D}(U)$. Khi đó ta có

$$
\langle \varphi |D(\psi )\rangle =\sum_{|\alpha|\leqslant}\int_{kU}n_{\alpha}\varphi  \partial^{\alpha}\psi  d\mu
$$

$$
=\sum_{|\alpha|\leqslant k}(-1)^{|\alpha|}\langle \partial^{\alpha}(\overline{n}_{\alpha}\varphi )|\psi \rangle =\langle^tD(\varphi )|\psi \rangle
$$

(xem VAR, R2, 14.3.8). Vì $\mathscr{D}(U)$ trù mật trong $L^2(U)$ (mệnh đề 4 của IV, p. 202), điều này suy ra rằng $\varphi \in$ dom($u^*$) và $u^*(\varphi ) =^tD(\varphi )$. Do đó ta có $(^tD)_-\subset u^*$; đặc biệt, $u^*$ có miền xác định trù mật và $u$ đóng được (mệnh đề 8 của IV, p. 237).

Cho $f\in$ dom($u^*$) và $\varphi \in \mathscr{D}(U)$. Vì $\mathscr{D}(U)\subset$ dom($u$), phân phối liên kết với $u^*(f)$ thỏa mãn

$$
\langle u^*(f), \varphi \rangle =\langle \overline{\varphi}|u^*(f)\rangle =\langle u(\overline{\varphi})|f\rangle
$$

Vì $D_-\subset u$, $u(\overline{\varphi})$ được tính bằng công thức (5), do đó

$$
\langle u^*(f), \varphi \rangle =\sum_{\alpha}\langle n_{\alpha}\partial^{\alpha}\overline{\varphi}|f\rangle =\sum_{\alpha}\langle \partial^{\alpha}\overline{\varphi}|\overline{n}_{\alpha}f\rangle
$$

$$
=\sum_{\alpha}\langle \overline{n}_{\alpha}f, \partial^{\alpha}\varphi \rangle =\sum_{\alpha}(-1)^{|\alpha|}\langle \partial^{\alpha}(\overline{n}_{\alpha}f), \varphi \rangle =\langle^tD(f), \varphi \rangle
$$

Do đó các phân phối $u^*(f)$ và $^tD(f)$ bằng nhau; vì thế phân phối $f$ thuộc $H_{_tD}$ và $u^*(f) =^tD(f)$, do đó $u^*\subset (^tD)_+$.

#### Nhận xét {#ts-iv-s4-n6-rem-1 .statement tag=033N}

Mệnh đề này có nghĩa là liên hợp của một toán tử bộ phận $u$ sao cho $D_-\subset u\subset D_+$ luôn luôn có thể được tính theo nghĩa phân phối: các phần tử $f$ của miền xác định của $u^*$ là các phần tử của $L^2(U)$ sao cho phân phối $^tD(f)$ thuộc $L^2$(U), và ta có $u^*(f) =^tD(f)$.

Người ta nói rằng D là đối xứng hình thức nếu $^tD = D$ như một toán tử vi phân vô hướng. Nếu đúng như vậy thì toán tử bộ phận $D_-$ là đối xứng.

Xét trường hợp riêng của toán tử vi phân vô hướng cấp 2 được xác định bởi

$$
\Delta  =-\sum_{i=1}^n\partial_i^2
$$

Một Laplacian trên U là mọi toán tử bộ phận $u$, tự liên hợp trên $L^2$(U), sao cho $\Delta_-\subset u($xem VAR, R2, 14.4.3, p. 83). Ta sẽ thấy sau này (IV, p. 261, ví dụ) rằng luôn tồn tại ít nhất một Laplacian trên $L^2(U)$; có thể tồn tại nhiều hơn một (bài tập 17 của IV, p. 358).

### 7. Phổ và Giải thức

#### Bổ đề 4 {#ts-iv-s4-lem-4 .statement tag=033O}

Cho E là một không gian Banach phức và cho $u$ là một toán tử bộ phận đóng đơn ánh trên E sao cho $u^{-1}\in \mathscr{L}(E)$. Cho $v\in \mathscr{L}(E)$ sao cho $\|v\|<\|u^{-1}\|^{-1}$. Khi đó toán tử bộ phận $u+v$ là đơn ánh, ta có $(u+v)^{-1}\in \mathscr{L}(E)$, và

$$
(u+v)^{-1}=u^{-1}\circ \sum_{k=0}^{+\infty}(-vu^{-1})^k \tag{6}
$$

trong đó chuỗi hội tụ tuyệt đối trong $\mathscr{L}(E)$. Hơn nữa, ta có

$$
\|(u+v)^{-1}\|\leqslant \|u^{-1}\|_{-1}
$$

$$
1- \|v\| \|u\|
$$

Vì $\|v\| \|u^{-1}\|<1$, chuỗi có số hạng tổng quát $(-vu^{-1})^k$ hội tụ tuyệt đối trong $\mathscr{L}$ (E), và tổng của nó là nghịch đảo của tự đồng cấu $1_E+vu^{-1}$ (mệnh đề 2 của I, p. 22). Do đó toán tử bộ phận $(1_E+vu^{-1})\circ u=u+v($IV, p. 226, nhận xét vi) là đơn ánh và toán tử bộ phận nghịch đảo $(u+v)^{-1}=u^{-1}\circ (1_E+vu^{-1})^{-1}($IV, p. 226, nhận xét iii) thuộc $\mathscr{L}(E)$. Vì

$\|(1_E+vu^{-1})^{-1}\|\leqslant \sum^{+\infty}(\|v\| \|u^{-1}\|)^k=$ 1 $_{-1}$,

$$
1- \|v\| \|u\|
$$

$k=0$

bổ đề được chứng minh.

#### Định nghĩa 8 {#ts-iv-s4-def-8 .statement tag=033P}

Cho $u$ là một toán tử đóng có miền xác định trù mật trên một không gian Banach phức E. Tập giải thức của $u$ là tập hợp các số phức $\lambda$ sao cho toán tử bộ phận $\lambda 1_E-u$ là đơn ánh và nghịch đảo của nó $(\lambda 1_E-u)^{-1}$ thuộc $\mathscr{L}(E)$.

Phổ của $u$, ký hiệu là Sp($u$), là phần bù của tập giải thức trong $\mathbf{C}$.

Nếu $\lambda \in \mathbf{C}-$ Sp($u$), ta ký hiệu bởi $R(u, \lambda )\in \mathscr{L}(E)$ nghịch đảo của $\lambda 1_E-u$. Ánh xạ từ $\mathbf{C}-$ Sp($u$) vào $\mathscr{L}(E)$ gán $R(u, \lambda )$ cho $\lambda$ được gọi là giải thức của $u$.

#### Nhận xét {#ts-iv-s4-n7-rem-1 .statement tag=033Q}

Cho E là một không gian Banach phức và cho $u$ là một toán tử đóng có miền xác định trù mật trên E.

1) Nếu $u\in \mathscr{L}$ (E), phổ của nó trùng với phổ của phần tử $u$ của đại số $\mathscr{L}(E)$(I, p. 2, Định nghĩa 1).

2) Gọi D là miền xác định của $u$. Với mọi $\lambda \in \mathbf{C}-$ Sp($u$), ta có

$$
1_E= (\lambda 1_E-u)\circ R(u, \lambda ),1_D= R(u, \lambda )\circ (\lambda 1_E-u) \tag{7}
$$

Hơn nữa, với $\lambda_1$ và $\lambda_2$ thuộc tập chính quy của $u$, ta có

$$
R(u, \lambda_1)-R(u, \lambda_2) = (\lambda_2-\lambda_1)R(u, \lambda_2)\circ R(u, \lambda_1) \tag{8}
$$

$$
R(u, \lambda_1)\circ R(u, \lambda_2) = R(u, \lambda_2)\circ R(u, \lambda_1) \tag{9}
$$

Thật vậy, ta có

$$
R(u, \lambda_1)-R(u, \lambda_2) = R(u, \lambda_1)\circ 1_E-1_D\circ R(u, \lambda_2)
$$

Vì $1_E= (\lambda_21_E-u)\circ R(u, \lambda_2)$ và $1_D= R(u, \lambda_1)\circ (\lambda_11_E-u)$, suy ra

$$
R(u, \lambda_1)-R(u, \lambda_2) =\lambda_2R(u, \lambda_1)\circ R(u, \lambda_2)
$$

$$
-R(u, \lambda_1)\circ u\circ R(u, \lambda_2)-\lambda_1R(u, \lambda_1)\circ R(u, \lambda_2)
$$

$$
+ R(u, \lambda_1)\circ u\circ R(u, \lambda_2)
$$

do đó có công thức thứ nhất. Bằng cách đổi chỗ vai trò của $\lambda_1$ và $\lambda_2$, suy ra công thức thứ hai.

3) Cho $\lambda \in \mathbf{C}$. Theo định lý đồ thị đóng (EVT, I, p. 19, Hệ quả 5), nếu ánh xạ tuyến tính từ dom($u$) vào E xác định bởi $x\mapsto (\lambda 1_E-u)(x)$ là song ánh, thì ánh xạ nghịch đảo của nó, mà đồ thị là đóng, là liên tục từ E vào E. Vậy $\lambda$ thuộc tập chính quy của $u$ nếu và chỉ nếu ánh xạ $x\mapsto (\lambda 1_E-u)(x)$ từ dom($u$) vào E là song ánh.

4) Nếu $\lambda$ thuộc phổ của $u$, thì một trong các tính chất sau đây xảy ra:

(i) Hạt nhân của $\lambda 1_E-u$ không thu về 0; khi đó người ta nói rằng $\lambda$ là một trị riêng của $u$, và chiều của Ker($\lambda 1_E-u$) là bội số của nó;

(ii) Toán tử bộ phận $\lambda 1_E-u$ là đơn ánh và ảnh của nó không trù mật trong E; khi đó người ta nói rằng $\lambda$ thuộc phổ thặng dư của $u$;

(iii) Toán tử bộ phận $\lambda 1_E-u$ là đơn ánh, ảnh của nó trù mật trong E, nhưng $\lambda 1_E-u$ không toàn ánh; khi đó người ta nói rằng $\lambda$ thuộc phổ liên tục của $u$.

5) Cho $\lambda$ là một số phức thuộc tập giải thức của $u$. Giải thức $R(u, \lambda )$ là một ánh xạ tuyến tính đơn ánh từ E vào E; ảnh của nó là miền xác định của $u$ và $u=\lambda 1_E-R(u, \lambda )^{-1}($cf. IV, p. 226). Ngược lại, tính chất này đặc trưng tập giải thức và giải thức. Chính xác hơn, cho $\lambda \in \mathbf{C}$; nếu tồn tại một ánh xạ tuyến tính liên tục đơn ánh $w$ từ E vào E sao cho $u=\lambda 1_E-w^{-1}$, thì $\lambda$ thuộc tập giải thức của $u$ và $w= R(u, \lambda )$.

Đặc biệt, nếu $v$ là một toán tử đóng có miền xác định trù mật trên E, và nếu $\lambda \in \mathbf{C}$ là một số phức không thuộc Sp($u$)$\cup$ Sp($v$), thì đẳng thức $R(u, \lambda ) = R(v, \lambda )$ suy ra $u=v$.

6) Phổ của một toán tử bộ phận có thể đóng được định nghĩa là phổ của bao đóng của nó.

Tồn tại các toán tử đóng có phổ rỗng, hoặc có phổ bằng $\mathbf{C}$ (bài tập 12 của IV, p. 347).

Cho E là một không gian Banach phức và $u$ là một toán tử đóng có miền xác định trù mật trên E. Nếu F là một không gian Banach phức và nếu $v: E\rightarrow F$ là một đẳng cấu, thì ta có Sp($v\circ u\circ v^{-1}$) $=$ Sp($u$) và $R(v\circ u\circ v^{-1}, \lambda ) =v\circ R(u, \lambda )\circ v^{-1}$ với mọi $\lambda  \notin$ Sp($u$).

#### Mệnh đề 14 {#ts-iv-s4-prop-14 .statement tag=033R}

Cho E là một không gian Banach phức. Cho $u$ là một toán tử đóng có miền xác định trù mật trên E và U là tập giải thức của nó.

a) Với mọi $\lambda \in U$, đĩa mở trong $\mathbf{C}$ có tâm $\lambda$ và bán kính $\|R(u, \lambda )\|^{-1}$ được chứa trong U;

b) Tập hợp U là mở trong $\mathbf{C}$;

c) Giả sử rằng Sp($u$) không rỗng. Cho $\lambda \in U$ và ký hiệu bởi $\delta$ khoảng cách trong $\mathbf{C}$ từ $\lambda$ đến phổ của $u$. Ta có $\delta  >0$ và $\|R(u, \lambda )\|\geqslant 1/\delta$;

d) Ánh xạ $\lambda \mapsto R(u, \lambda )$ là một ánh xạ chỉnh hình từ U vào $\mathscr{L}(E)$. Với mọi số nguyên $k\in \mathbf{N}$ và mọi $\lambda \in U$, ta có

$\frac{\partial^k}{\partial \lambda^k}R(u, \lambda ) = (-1)^kk$!R($u, \lambda$ )$^{k+1}$.

Cho $\lambda \in U$. Với mọi $\mu\in \mathbf{C}$ sao cho $\|(\mu-\lambda )1_E\|<\|R(u, \lambda )\|^{-1}$, bổ đề 4 áp dụng cho toán tử bộ phận đơn ánh $\lambda 1_E-u$ và cho $v= (\mu-\lambda )1_E$ suy ra rằng toán tử bộ phận $\mu1_E-u=\lambda 1_E-u+v$ là đơn ánh và có nghịch đảo liên tục. Điều này suy ra a). Theo loc. cit., ta cũng có công thức

$$
R(u, \mu) = R(u, \lambda )\circ \sum_{k\in\mathbf{N}}(\lambda -\mu)^kR(u, \lambda )^k
$$

công thức này suy ra rằng giải thức của $u$ là chỉnh hình trên U.

Mệnh đề b) suy ra ngay từ a). Nếu Sp($u$) khác rỗng, khoảng cách từ $\lambda$ đến Sp($u$) là dương ngặt (TG, IX, p. 13, Mệnh đề 2), do đó c).

Phần cuối của mệnh đề d) được chứng minh bằng quy nạp theo $k$, trường hợp $k= 1$ là một hệ quả của công thức (8), p. 245.

#### Mệnh đề 15 {#ts-iv-s4-prop-15 .statement tag=033S}

Cho $u$ là một toán tử đóng có miền xác định trù mật trên một không gian Banach phức E và $\lambda$ là một số phức thuộc tập chính quy của $u$.

a) Tập con Sp(R($u, \lambda$ ))$-\{0\}$ của $\mathbf{C}$ là ảnh của phổ của $u$ qua ánh xạ $\mu\mapsto (\lambda -\mu)^{-1}$ từ $\mathbf{C}-\{\lambda \}$ vào $\mathbf{C}^*$;

b) Với mọi $\mu\not =\lambda$ trong $\mathbf{C}$, ta có

Ker($\mu1_E-u$) $=$ Ker(($\lambda -\mu$)$^{-1}1_E-R(u, \lambda )$).

Ta chứng minh mệnh đề a). Với mọi $\mu\not =\lambda$, ta tính được

$$
\mu1_E-u= (\lambda -\mu) ((\lambda -\mu)^{-1}1_E-R(u, \lambda )) (\lambda 1_E-u)
$$

Vì $\lambda  \notin$ Sp($u$) và $\mu\not =\lambda$, ánh xạ tuyến tính $(\lambda -\mu)(\lambda 1_E-u)$ là một song ánh từ dom($u$) lên E. Do đó, công thức này kéo theo rằng $\mu1_E-u$ là một song ánh từ dom($u$) lên E khi và chỉ khi $(\lambda -\mu)^{-1}1_E-R(u, \lambda )$ là một song ánh từ E lên E, điều này chứng minh mệnh đề.

Ta chứng minh b). Nếu $\mu\not =\lambda$ và $x\in$ Ker(($\lambda -\mu$)$^{-1}1_E-R(u, \lambda )$), thì $x\in$ dom($u$) và công thức $1_E= (\lambda 1_E-u)\circ R(u, \lambda )$ kéo theo rằng $x\in$ Ker($\mu1_E-u$). Ngược lại, nếu $x\in$ Ker($\mu1_E-u$) và $\mu\not =\lambda$, công thức $1_{dom(u)}= R(u, \lambda )\circ (\lambda 1_E-u)$ kéo theo $R(u, \lambda )(x) = (\lambda -\mu)^{-1}x$.

#### Mệnh đề 16 {#ts-iv-s4-prop-16 .statement tag=033T}

Cho $u$ là một toán tử đóng có miền xác định trù mật trên một không gian Hilbert phức E. Phổ của $u^*$ là ảnh của phổ của $u$ qua phép liên hợp phức và, với mọi phần tử $\lambda$ thuộc tập chính quy của $u$, ta có $R(u, \lambda )^*= R(u^*, \lambda )$. Đặc biệt, nếu $u$ là tự liên hợp, thì tự đồng cấu $R(u, \lambda )$ là chuẩn với mọi $\lambda  \notin$ Sp($u$).

Cho $\lambda \in \mathbf{C}-$ Sp($u$) là một phần tử của tập chính quy của $u$. Ta có $u=\lambda 1_E-R(u, \lambda )^{-1}$, do đó

$$
u^*=\overline{\lambda}1_E-(R(u, \lambda )^{-1})^*=\overline{\lambda}1_E-(R(u, \lambda )^*)^{-1}
$$

(IV, p. 236 và mệnh đề 9 của IV, p. 239). Áp dụng nhận xét 5, ta suy ra rằng $\overline{\lambda}\in \mathbf{C}-$ Sp($u^*$) và $R(u, \lambda )^*= R(u^*, \lambda )$. Do đó, phổ của $u^*$ được chứa trong ảnh của Sp($u$) dưới phép liên hợp phức. Ta thu được đẳng thức bằng cách áp dụng tính chất này cho $u^*$, vì $u^{**}=u$ (hệ quả của mệnh đề 8 của IV, p. 237). Khi đó khẳng định cuối cùng suy ra từ công thức (9), p. 245.

#### Hệ quả {#ts-iv-s4-n7-cor-1 .statement tag=033U}

Cho $u$ là một toán tử bộ phận tự liên hợp trên một không gian Hilbert phức E. Nếu E khác không, thì phổ của $u$ không rỗng.

Giả sử rằng Sp($u$) rỗng. Khi đó $u$ là đơn ánh và $u^{-1}=-R(u,0)$ là một tự đồng cấu đơn ánh của E sao cho Sp($u^{-1}$)$\subset  \{0\}$ (mệnh đề 15, a)), do đó Sp($u^{-1}$) $=\{0\}($I, p. 26, hệ quả 1). Vì $u^{-1}$ là chuẩn (mệnh đề 16), điều này kéo theo $u^{-1}$ bằng không (I, p. 110, ví dụ 1), mâu thuẫn.

#### Bổ đề 5 {#ts-iv-s4-lem-5 .statement tag=033V}

Cho E là một không gian Hilbert phức và $u$ là một toán tử bộ phận đóng với miền xác định trù mật trên E. Cho $\lambda \in \mathbf{C}$. Giả sử rằng tồn tại một số thực $c >0$ sao cho

(10) $\|u(x)-\lambda x\|\geqslant c\|x\|$ với mọi $x\in$ dom($u$),

(11) $\|u^*(x)-\lambda x\|\geqslant c\|x\|$ với mọi $x\in$ dom($u^*$).

Khi đó $\lambda$ thuộc tập chính quy của $u$ và $\|R(u, \lambda )\|\leqslant c^{-1}$.

Giả thiết kéo theo rằng $u-\lambda 1_E$ và $u^*-\overline{\lambda}1_E$ là đơn ánh. Gọi F là ảnh của $u-\lambda 1_E$. Không gian F là trù mật trong E, vì trực giao của nó bằng Ker($u^*-\overline{\lambda}1_E$) (mệnh đề 7, c) của IV, p. 236), mà hạt nhân này bằng không.

Ta chứng minh rằng không gian F là đóng. Cho $(x_n)_{n\in\mathbf{N}}$ là một dãy trong dom($u$) sao cho dãy $(u(x_n)-\lambda x_n)_{n\in\mathbf{N}}$ hội tụ đến $y\in F$. Bất đẳng thức (10) kéo theo rằng dãy $(x_n)_{n\in\mathbf{N}}$ là một dãy Cauchy trong E. Gọi $x\in E$ là giới hạn của nó. Dãy $(x_n, u(x_n))$ hội tụ đến $(x, y+\lambda x)$ trong $E\times E$; vì đồ thị của $u$ là đóng, do đó ta có $x\in$ dom($u$) và $u(x) =y+\lambda x$, điều này chứng minh rằng $y\in F$.

Ta kết luận rằng F = E. Vậy toán tử bộ phận $u-\lambda 1_E$ là song ánh, do đó $\lambda  \notin$ Sp($u$) (nhận xét 3). Khi đó bất đẳng thức (10) kéo theo rằng $\|R(u, \lambda )\|\leqslant c^{-1}$.

#### Mệnh đề 17 {#ts-iv-s4-prop-17 .statement tag=033W}

Cho E là một không gian Hilbert phức và $u$ là một toán tử bộ phận tự liên hợp trên E.

a) Phổ của $u$ được chứa trong $\mathbf{R}$;

b) Nếu $u$ dương, thì phổ của $u$ được chứa trong $\mathbf{R}_+$;

c) Giả sử rằng E khác không. Cho $\lambda  \notin$ Sp($u$) và cho $\delta  >0$ là khoảng cách từ $\lambda$ đến phổ của $u$. Khi đó $\|R(u, \lambda )\|=\delta^{-1}$.

Cho $(a, b)\in \mathbf{R}\times \mathbf{R}$ và $\lambda =a+ib$. Cho $x\in$ dom($u$). Vì $u$ là tự liên hợp, ta có $\langle x|u(x)\rangle  \in \mathbf{R}$, do đó

$$
\|u(x)-\lambda x\|^2=\|u(x)\|^2-2a\langle x|u(x)\rangle + (a^2+b^2)\|x\|^2
$$

$$
=\|u(x)-\lambda x\|^2
$$

Giả sử rằng $b\not = 0$. Khi đó suy ra

$$
\|u(x)-\lambda x\|^2=\|u(x)-\lambda x\|^2\geqslant (\|u(x)\| -a\|x\|)^2+b^2\|x\|^2
$$

$$
\geqslant b^2\|x\|^2
$$

Theo Bổ đề 5, do đó ta có $\lambda  \notin$ Sp($u$), suy ra mệnh đề a).

Giả sử thêm rằng $u$ là dương. Nếu $b= 0$ và $a <0$, tương tự ta thu được đối với $x\in$ dom($u$) bất đẳng thức

$$
\|u(x)-\lambda x\|^2=\|u(x)-\lambda x\|^2\geqslant (\|u(x)\| -a\|x\|)^2\geqslant a^2\|x\|^2
$$

do đó $\lambda  \notin$ Sp($u$) $($loc. cit.$)$, điều này chứng minh b).

Sau cùng, hãy chứng minh c). Theo Mệnh đề 16, giải thức $R(u, \lambda )$ là một tự đồng cấu chuẩn tắc của E. Vậy chuẩn của nó bằng bán kính phổ của nó (Hệ quả 1 của I, p. 108), do đó

$\|R(u, \lambda )\|=$ sup$_{\mu\in Sp(R(u,\lambda))}|\mu|$

(Định lý 1 của I, p. 24). Phổ của $R(u, \lambda )$ không thể thu về $\{0\}$, vì trong trường hợp đó ta sẽ có $\|R(u, \lambda )\|= 0$, nên ảnh dom($u$) của $R(u, \lambda )$ sẽ bằng không, và E cũng vậy. Vậy Mệnh đề 15 suy ra rằng

$\|R(u, \lambda )\|=$ sup$_{\mu\in Sp(u)}\frac{1}{|\lambda-\mu|}=\frac{1}{\delta}$.

#### Hệ quả {#ts-iv-s4-n7-cor-2 .statement tag=033X}

Cho $u$ là một toán tử tự liên hợp trên E.

a) Phổ dư của $u$ là rỗng;

b) Với mọi $\lambda \not =\mu$ trong $\mathbf{C}$, các không gian riêng của $u$ tương ứng với $\lambda$ và $\mu$ là trực giao.

Hãy chứng minh a). Cho $\lambda$ thuộc phổ của $u$; nó là một số thực (Mệnh đề 17). Ta có Ker($\lambda 1_E-u$) $=$ Im($\lambda 1_E-u$)$^{\circ}$ (Mệnh đề 7 của IV, p. 236), do đó $\lambda$ không phải là một trị riêng của $u$ nếu toán tử bộ phận $\lambda 1_E-u$ có ảnh trù mật. Theo định nghĩa điều này hàm ý rằng phổ dư của $u$ là rỗng.

Hãy chứng minh b). Theo mệnh đề, ta có thể giả sử rằng $\lambda$ và $\mu$ là thực. Lấy $x\in$ dom($u$) sao cho $u(x) =\lambda x$ và $y\in$ dom($u$) sao cho $u(y) =\mu y$. Khi đó ta có

$$
\lambda \langle x|y\rangle =\langle u(x)|y\rangle =\langle x|u(y)\rangle =\mu\langle x|y\rangle
$$

do đó $\langle x|y\rangle = 0$.

#### Nhận xét {#ts-iv-s4-n7-rem-2 .statement tag=033Y}

Nếu $u$ là một toán tử đối xứng đóng không tự liên hợp, thì phổ của nó không được chứa trong $\mathbf{R}($xem hệ quả 10 của IV, p. 257 dưới đây), và có thể các không gian riêng của $u$ ứng với $\lambda$ và $\overline{\lambda}$ không trực giao (bài tập 11 của IV, p. 347).

### 8. Giả phổ

#### Định nghĩa 9 {#ts-iv-s4-def-9 .statement tag=033Z}

Cho E là một không gian Banach phức và $u$ là một toán tử bộ phận đóng trên E. Cho $\varepsilon$ là một số thực dương ngặt. Theo định nghĩa, $\varepsilon$-giả phổ của $u$ là hợp của phổ của $u$ và của tập hợp các số phức $\lambda$ thuộc tập chính quy của $u$ sao cho $\|R(u, \lambda )\|> \varepsilon^{-1}$. Tập hợp này được ký hiệu là PSp$_{\varepsilon}(u)$.

Một số tác giả định nghĩa $\varepsilon$-giả phổ của $u$ là tập $T_{\varepsilon}(u)$ bằng hợp của Sp($u$) và của tập các $\lambda \in \mathbf{C}-$ Sp($u$) sao cho $\|R(u, \lambda )\|\geqslant \varepsilon^{-1}$. Bao đóng của PSp$_{\varepsilon}(u)$ được chứa trong $T_{\varepsilon}(u)$, nhưng bao hàm này có thể là ngặt, ngay cả khi E là một không gian Hilbert (xem bài tập 18 của IV, p. 348 và 19 của IV, p. 349).

#### Mệnh đề 18 {#ts-iv-s4-prop-18 .statement tag=0340}

Cho E là một không gian Banach phức và $u$ là một toán tử bộ phận đóng trên E. Cho $\varepsilon \in \mathbf{R}^*_+$. Tập PSp$_{\varepsilon}(u)$ là một tập con mở của $\mathbf{C}$. Nó khác rỗng nếu E khác không.

Nếu E bằng không, thì PSp$_{\varepsilon}(u)$ là rỗng. Giả sử E khác không. Theo mệnh đề 14 của IV, p. 246, tập PSp$_{\varepsilon}(u)$ là một tập con mở của $\mathbf{C}$.

Tập PSp$_{\varepsilon}(u)$ là khác rỗng nếu phổ của $u$ khác rỗng. Nếu Sp($u$) là rỗng, thì định lý Liouville (VAR, R1, p. 29, 3.3.6) kéo theo rằng hàm chỉnh hình trên $\mathbf{C}$ được định nghĩa bởi $\lambda \mapsto R(u, \lambda )$ là không bị chặn, do đó tồn tại $\lambda$ trong $\mathbf{C}$ sao cho $\|R(u, \lambda )\|> \varepsilon^{-1}$.

#### Mệnh đề 19 {#ts-iv-s4-prop-19 .statement tag=0341}

Cho E là một không gian Banach phức và $u$ là một toán tử bộ phận đóng trên E. Ta có PSp$_{\varepsilon}(u)\subset$ PSp$_{\delta}(u)$ nếu $0< \varepsilon  < \delta$ và

$\bigcap_{\varepsilon\in\mathbf{R}^*_+}$ PSp$_{\varepsilon}(u) =$ Sp($u$).

Mệnh đề thứ nhất suy ra từ định nghĩa. Đối với mệnh đề thứ hai, phổ của $u$ được chứa trong PSp$_{\varepsilon}(u)$ với mọi $\varepsilon  >0$ theo định nghĩa, và nếu $\lambda  \notin$ Sp($u$), thì $\lambda  \notin$ PSp$_{\varepsilon}(u)$ khi $\varepsilon  <\|R(u, \lambda )\|^{-1}$.

#### Mệnh đề 20 {#ts-iv-s4-prop-20 .statement tag=0342}

Cho E là một không gian Banach phức và $u$ là một toán tử bộ phận đóng trên E. Cho $\varepsilon \in \mathbf{R}^*_+$. Với mọi $\lambda \in \mathbf{C}$, các điều kiện sau là tương đương:

(i) Ta có $\lambda \in$ PSp$_{\varepsilon}(u)$;

(ii) Hoặc $\lambda \in$ Sp($u$), hoặc tồn tại $x\in$ dom($u$) sao cho $\|x\|= 1$ và $\|(\lambda 1_E-u)(x)\|< \varepsilon$;

(iii) Tồn tại $v\in \mathscr{L}(E)$ sao cho $\|v\|< \varepsilon$ và $\lambda \in$ Sp($u+v$).

Có thể giả sử rằng E khác không. Điều kiện (ii) là một sự phát biểu lại của định nghĩa, do đó cũng là của điều kiện (i).

Giả sử điều kiện (i) được thỏa mãn và hãy chứng minh (iii). Nếu $\lambda$ thuộc phổ của $u$, ta có thể lấy $v= 0$ trong (iii).

Vậy giả sử rằng $\lambda  \notin$ Sp($u$). Theo định nghĩa của PSp$_{\varepsilon}(u)$, tồn tại $y\in E$ sao cho $\|y\|= 1$ và $\|R(u, \lambda )y\|> \varepsilon^{-1}$. Đặt $x= R(u, \lambda )y$. Ta có $x\not = 0$. Theo định lý Hahn–Banach (EVT, II, p. 67, hệ quả 2), dạng tuyến tính $\ell$ trên $\mathbf{C}x$ sao cho $\ell (x) = 1$ có một mở rộng liên tục $\ell_1\in E'$ sao cho $\|\ell_1\|=\|\ell \|$; do đó $\|\ell_1\|=\|x\|^{-1}< \varepsilon$. Với mọi $e\in E$, đặt $v(e) =\ell_1(e)y$. Ta có $v\in \mathscr{L}(E)$ và $v(x) =y$. Suy ra $(u+v)x=u(x) +y=\lambda x$, vì thế $\lambda \in$ Sp($u+v$). Hơn nữa, vì $\|v\|=\|\ell_1\|< \varepsilon$, điều kiện (iii) được thỏa mãn.

Ngược lại, cho $v\in \mathscr{L}(E)$ sao cho $\|v\|< \varepsilon$ và $\lambda \in$ Sp($u+v$). Khi đó toán tử bộ phận $\lambda 1_E-(u+v)$ không đơn ánh với một nghịch đảo liên tục; theo Bổ đề 4 của IV, p. 243, áp dụng cho toán tử bộ phận đơn ánh $\lambda 1_E-u$ và cho $-v$, do đó ta có $\|v\|\geqslant \|R(u, \lambda )\|^{-1}$. Suy ra điều kiện (iii) kéo theo (i).

#### Hệ quả {#ts-iv-s4-n8-cor-1 .statement tag=0343}

Cho E là một không gian Banach phức và $u$ là một toán tử bộ phận đóng trên E. Cho $\varepsilon  >0$.

a) Với mọi $v\in \mathscr{L}(E)$, ta có PSp$_{\varepsilon}(u)\subset$ PSp$_{\varepsilon+\|v\|}(u+v)$;

b) Cho $\delta  >0$ và gọi $D_{\delta}$ là đĩa mở tâm 0 bán kính $\delta$ trong $\mathbf{C}$. Ta có PSp$_{\varepsilon}(u) + D_{\delta}\subset$ PSp$_{\varepsilon+\delta}(u)$.

Cho $\lambda \in$ PSp$_{\varepsilon}(u)$. Tồn tại một tự đồng cấu $w\in \mathscr{L}(E)$ sao cho $\|w\|< \varepsilon$ và $\lambda \in$ Sp($u+w$) (Mệnh đề 20). Vì $u+w= (u+v)+(w-v)$ và $\|w-v\|< \varepsilon +\|v\|$, nên ta có $\lambda \in$ PSp$_{\varepsilon+\|v\|}(u+v) ($loc. cit.).

Cho $\mu\in D_{\delta}$; ta có $\lambda +\mu\in$ Sp($u+ (w+\mu1_E)$) và $\|w+\mu1_E\|< \varepsilon +\delta$, do đó $\lambda +\mu\in$ PSp$_{\varepsilon+\delta}(u) ($loc. cit.).

#### Mệnh đề 21 {#ts-iv-s4-prop-21 .statement tag=0344}

Cho E là một không gian Banach phức và $u$ là một toán tử bộ phận đóng trên E. Cho $\varepsilon \in \mathbf{R}^*_+$. Mọi thành phần liên thông bị chặn của PSp$_{\varepsilon}(u)$ đều cắt phổ của $u$.

Gọi U là một thành phần liên thông của PSp$_{\varepsilon}(u)$ không cắt Sp($u$). Tập hợp U là mở và đóng trong PSp$_{\varepsilon}(u)$, và do đó bao đóng U của nó trong $\mathbf{C}$ thỏa mãn $U\cap$ PSp$_{\varepsilon}(u) = U$.

Vì Sp($u$) được chứa trong PSp$_{\varepsilon}(u)$ và U không cắt Sp($u$), đẳng thức này chứng tỏ rằng tập hợp U rời nhau với Sp($u$), do đó được chứa trong tập chính quy của $u$. Hơn nữa, nó kéo theo rằng tập hợp $\overline{U}-$ U không cắt PSp$_{\varepsilon}(u)$.

Do đó ta có $\|R(u, \lambda )\|\leqslant \varepsilon^{-1}$ với mọi $\lambda$ trong $\overline{U}-$ U, trong khi $\|R(u, \lambda )\|> \varepsilon^{-1}$ với $\lambda \in U$. Nếu tập hợp U bị chặn thì bao đóng $\overline{U}$ của nó là compact và tồn tại $\lambda_0\in \overline{U}$ sao cho $\|R(u, \lambda )\|\leqslant \|R(u, \lambda_0)\|$ với $\lambda \in U$. Điều trên kéo theo $\lambda_0\in U$, điều này mâu thuẫn với nguyên lý cực đại (VAR, R1, p. 29, 3.3.7) vì giải thức của $u$ là chỉnh hình trên tập chính quy của $u$ (Mệnh đề 14 của IV, p. 246).

### 9. Các toán tử phép nhân

Cho X là một không gian compact địa phương và $\mu$ là một độ đo dương trên X. Ta xét các toán tử phép nhân trên $L^2(X, \mu)$; đó là các toán tử đóng với miền xác định trù mật (Mệnh đề 5 của IV, p. 232). Với mọi hàm $\mu$-đo được $g$ trên X, ta sẽ ký hiệu bởi $m_g$ toán tử bộ phận phép nhân bởi $g$ trên $L^2(X, \mu)$.

#### Mệnh đề 22 {#ts-iv-s4-prop-22 .statement tag=0345}

Cho $g$ là một hàm $\mu$-đo được trên X.

a) Phổ của $m_g$ là ảnh $\mu$-cốt yếu S của $g$;

b) Cho $\lambda \in \mathbf{C}-$ Sp($m_g$). Giải thức $R(m_g, \lambda )$ là toán tử phép nhân $m_h$, trong đó $h$ là hàm trên X được xác định bởi $h(x) = 0$ nếu $g(x) =\lambda$ và $h(x) = (\lambda -g(x))^{-1}$ trong các trường hợp khác.

Ta hãy chứng minh rằng $\mathbf{C}-$ S được chứa trong tập chính quy của $m_g$. Cho $\lambda \in \mathbf{C}-$ S. Tồn tại một lân cận mở U của $\lambda$ sao cho tập con $Y =\overset{-1}{g}(U)$ của X là địa phương $\mu$-không đáng kể. Khi đó hàm $k$ được xác định trên X bởi $k(x) = (\lambda -g(x))^{-1}$ nếu $x \notin Y$ và $k(x) = 0$ nếu $x\in Y$ thuộc $\mathscr{L}^{\infty}(X, \mu)$ (Bổ đề 5 của IV, p. 184); do đó toán tử phép nhân bởi $k$ là một tự đồng cấu của $L^2(X, \mu)$.

Vì $|gk|\leqslant 1 +|\lambda k|$, ta có

$$
|gkf|\leqslant |f|+|\lambda kf|
$$

với $f\in \mathscr{L}^2(X, \mu)$, điều này kéo theo rằng ảnh của $m_k$ được chứa trong miền xác định của $m_g$. Ngược lại, cho $f\in \mathscr{L}^2(X, \mu)$ mà lớp $\widetilde{f}$ của nó thuộc miền xác định của $m_g$. Bên ngoài tập địa phương $\mu$-không đáng kể Y, ta có $f(x) =k(x)(\lambda -g(x))f(x)$, do đó $\widetilde{f}$ nằm trong ảnh của $m_k$. Cùng công thức ấy chứng minh rằng $\lambda$ thuộc tập chính quy của $m_g$ và rằng $R(m_g, \lambda ) =m_k$. Vì tập Y là địa phương $\mu$-không đáng kể, toán tử phép nhân $m_k$ trùng với toán tử $m_h$ được mô tả trong mệnh đề b).

Hãy chứng minh ngược lại rằng $\mathbf{C}-$ Sp($m_g$) được chứa trong $\mathbf{C}-$ S. Lấy $\lambda \in \mathbf{C}-$ Sp($m_g$). Lấy một số thực $M>\|R(m_g, \lambda )\|$. Ký hiệu Y là tập hợp các $x\in X$ sao cho $|\lambda -g(x)|<M^{-1}$. Hãy chứng minh rằng Y là địa phương không đáng kể đối với $\mu$, điều này sẽ kéo theo rằng $\lambda$ không thuộc S, và sẽ hoàn tất chứng minh.

Lấy K là một tập con compact của X. Lấy $\varphi$ là hàm đặc số của $Y\cap K$; đó là một phần tử của $\mathscr{L}^2(X, \mu)$, và ta ký hiệu bởi $\widetilde{\varphi}$ lớp của nó trong $L^2(X, \mu)$. Lấy $\psi$ là một hàm trong $\mathscr{L}^2(X, \mu)$ mà lớp của nó trong $L^2(X, \mu)$ là $R(m_g, \lambda )(\widetilde{\varphi})$. Ta có $R(m_g, \lambda )(\widetilde{\varphi})\in$ dom($m_g$) và $(\lambda -m_g)(R(m_g, \lambda )(\widetilde{\varphi})) =\widetilde{\varphi}$, do đó $(\lambda -g(x))\psi (x) = 1$ với $\mu$-hầu khắp mọi $x\in Y\cap K$. Điều này suy ra

$$
\|R(m_g, \lambda )\|^2\|\widetilde{\varphi}\|^2\geqslant \|R(m_g, \lambda )(\widetilde{\varphi})\|^2\geqslant M^2\mu(Y\cap K) = M^2\|\widetilde{\varphi}\|^2
$$

Xét theo cách lựa chọn M, điều này có nghĩa là $\varphi$ bằng không $\mu$-hầu khắp mọi nơi. Vậy tập hợp $Y\cap K$ là không đáng kể đối với $\mu$. Do đó tập hợp Y là địa phương không đáng kể đối với $\mu$ (INT, IV, p. 172, § 5, n$^o2$, Prop. 5).

#### Mệnh đề 23 {#ts-iv-s4-prop-23 .statement tag=0346}

Cho $g$ là một hàm $\mu$-đo được trên X. Toán tử liên hợp của toán tử nhân $m_g$ là $m_{\overline{g}}$.

Với mọi số nguyên $n\geqslant$ 1, lấy $\varphi_n$ là hàm đặc số của tập hợp các phần tử $x\in$ X sao cho $|g(x)|\leqslant n$, và lấy $\widetilde{\varphi}_n$ là lớp của nó trong $L^2(X, \mu)$. Lấy $f\in \mathscr{L}^2(X, \mu)$ sao cho lớp của nó $\widetilde{f}$ thuộc dom($m^*_g$), và lấy $\psi$ là một hàm mà lớp của nó là $m^*_g(\widetilde{f})$.

Với mọi $h\in \mathscr{L}^2(X, \mu)$ mà lớp của nó $\widetilde{h}$ thuộc dom($m_g$), ta cũng có $\widetilde{h}\widetilde{\varphi}_n\in$ dom($m_g$), và do đó $\langle \widetilde{f}|m_g(\widetilde{h}\widetilde{\varphi}_n)\rangle =\langle m^*_g(\widetilde{f})|\widetilde{h}\widetilde{\varphi}_n\rangle$. Điều này cho đẳng thức

$$
\int_X\overline{(f g-\psi)}\varphi_nh d\mu= 0
$$

Vì miền xác định của $m_g$ là trù mật trong $L^2(X, \mu)$, suy ra $(f g-\psi )\varphi_n$ bằng không $\mu$-hầu khắp nơi. Vì $n$ là tùy ý, điều này có nghĩa là $m^*_g(\widetilde{f})$ là lớp của $f g$ trong $L^2(X, \mu)$. Đặc biệt, vì $m^*_g(\widetilde{f})\in L^2(X, \mu)$, suy ra $f$ thuộc miền xác định của $m_{\overline{g}}$ và $m^*_g(\widetilde{f}) =m_{\overline{g}}(\widetilde{f})$.

Vậy toán tử liên hợp của $m_g$ là một mở rộng của $m_{\overline{g}}$. Hơn nữa, ta có

$$
\langle f|m_g(h)\rangle =\int_X\overline{f}\cdot (gh)d\mu=\int_Xf\overline{g}h d\mu
$$

với mọi $f\in L^2(X, \mu)$ và $h\in$ dom($m_g$), điều này chứng minh rằng dạng tuyến tính $h\mapsto  \langle f|m_g(h)\rangle$ là liên tục mỗi khi $m_{\overline{g}}(f)g$ thuộc $L^2(X, \mu)$. Do đó miền xác định của $m_{\overline{g}}$ được chứa trong miền xác định của $m^*_g$, và điều đó kết thúc chứng minh.

#### Hệ quả {#ts-iv-s4-n9-cor-1 .statement tag=0347}

Cho $g$ là một hàm $\mu$-đo được trên X. Toán tử phép nhân $m_g$ trên $L^2(X, \mu)$ là tự liên hợp (resp. dương ) khi và chỉ khi hàm $g$ địa phương nhận giá trị thực $\mu$-hầu khắp nơi (resp. địa phương dương $\mu$-hầu khắp nơi).

Mệnh đề thứ nhất suy ra từ mệnh đề. Nếu $g$ địa phương dương $\mu$-hầu khắp nơi, ta có $\langle f|m_g(f)\rangle =\int_Xg|f|^2d\mu\geqslant 0$ với mọi $f\in L^2(X, \mu)$, do đó toán tử bộ phận $m_g$ là dương.

Ngược lại, nếu $m_g$ là dương, thì phổ của nó được chứa trong $\mathbf{R}_+$ (mệnh đề 17 của IV, p. 248); vì đây là ảnh cốt yếu $\mu$ của $g$ (mệnh đề 22, a)), điều đó có nghĩa là $g$ địa phương dương $\mu$-hầu khắp nơi.

#### Bổ đề 6 {#ts-iv-s4-lem-6 .statement tag=0348}

Cho $g_1$ và $g_2$ là các hàm $\mu$-đo được trên X.

a) Toán tử bộ phận $m_{g_1}+m_{g_2}$ là khả đóng và bao đóng của nó là toán tử phép nhân $m_{g_1+g_2}$;

b) Ta có $m_{g_1}\circ m_{g_2}\subset m_{g_1g_2}$;

c) Giả sử rằng $g_1$ bị chặn. Khi đó ta có $m_{g_2}\circ m_{g_1}=m_{g_1g_2}$. Hơn nữa, miền xác định của $m_{g_2}$ được chứa trong miền xác định của $m_{g_1g_2}$, và $m_{g_1}\circ m_{g_2}$ là hạn chế của $m_{g_1g_2}$ lên dom($m_{g_2}$).

Hiển nhiên $m_{g_1+g_2}$ là một mở rộng của $m_{g_1}+m_{g_2}$; do đó toán tử sau là khả đóng, và $\overline{m_{g_1} + m_{g_2}}\subset m_{g_1+g_2}$.

Cho $f\in \mathscr{L}^2(X, \mu)$ sao cho hàm $h= (g_1+g_2)f$ thuộc $\mathscr{L}^2(X, \mu)$. Với mọi số nguyên $n\geqslant 1$, ký hiệu $X_n$ là tập hợp các $x\in X$ sao cho $|g_1(x)|+|g_2(x)|\leqslant n$, và ký hiệu $\varphi_n$ là hàm đặc số của $X_n$. Ta có $\varphi_nf\in$ dom($m_{g_1}+m_{g_2}$). Vì $(\varphi_nf)(x)$ hội tụ đến $f(x)$ với mọi $x\in X$, và vì với mọi $n\in \mathbf{N}$ ta có $|\varphi_nf|\leqslant |f|$ và $|(g_1+g_2)\varphi_nf|\leqslant$ $|(g_1+g_2)f|=|h|$, với $h\in \mathscr{L}^2(X, \mu)$ theo giả thiết, định lý của Lebesgue (INT, IV, p. 137, § 3, No.$^o7$, Định lý 6) suy ra rằng dãy các cặp lớp trong $L^2(X, \mu)\times L^2(X, \mu)$ của $(\varphi_nf,(g_1+g_2)\varphi_nf)$, thuộc đồ thị của $m_{g_1}+m_{g_2}$, hội tụ đến cặp lớp của $(f, h)$ trong $L^2(X, \mu)$. Do đó bao đóng của $m_{g_1}+m_{g_2}$ quả thật bằng $m_{g_1+g_2}$.

Hiển nhiên là $m_{g_1}\circ m_{g_2}\subset m_{g_1g_2}$. Giả sử $g_1$ bị chặn, để $m_{g_1}$ là một ánh xạ tuyến tính liên tục trên $L^2(X, \mu)$. Khi đó miền xác định của $m_{g_2}\circ m_{g_1}$ là tập hợp các lớp của những hàm $f\in \mathscr{L}^2(X, \mu)$ sao cho $g_2(g_1f)\in \mathscr{L}^2(X, \mu)$, nghĩa là miền xác định của $m_{g_1g_2}$. Vậy $m_{g_2}\circ m_{g_1}=m_{g_1g_2}$.

Tương tự cũng hiển nhiên rằng dom($m_{g_1}\circ m_{g_2}$) $=$ dom($m_{g_2}$) được chứa trong dom($m_{g_1g_2}$), và hạn chế của $m_{g_1g_2}$ lên không gian này bằng $m_{g_1}\circ m_{g_2}$.

Cần thận trọng đừng tin rằng $m_{g_1}\circ m_{g_2}=m_{g_1g_2}$ nói chung (bài tập 10 của IV, p. 347). Tuy nhiên, ta có kết quả bộ phận sau đây:

#### Mệnh đề 24 {#ts-iv-s4-prop-24 .statement tag=0349}

Cho $g$ là một hàm $\mu$-đo được trên X.

a) Ta có $m_{\overline{g}}\circ m_g=m_{|g|^2}$;

b) Với mọi số nguyên $k, \ell \in \mathbf{N}$, ta có $m_{g^k\overline{g}^{\ell}}=m^k_gm^{\ell}_{\overline{g}}$.

Ta có $m_{\overline{g}}\circ m_g\subset m_{|g|^2}$ theo Bổ đề 6. Ngược lại, từ bất đẳng thức $|g|\leqslant 1 +|g|^2$ suy ra dom($m_{|g|^2}$) $=$ dom($m_{\overline{g}}\circ m_g$), do đó có mệnh đề thứ nhất.

Cho $k, \ell \in \mathbf{N}$. Ta có $m^k_gm^{\ell}_{\overline{g}}\subset m_{g^k\overline{g}^{\ell}}($loc. cit.). Miền xác định của $m^k_gm^{\ell}_{\overline{g}}$ là tập hợp các lớp trong $L^2(X, \mu)$ của các hàm $h\in \mathscr{L}^2(X, \mu)$ sao cho $|g|^jh$ thuộc $\mathscr{L}^2(X, \mu)$ với mọi số nguyên $j$ thỏa mãn $0\leqslant j\leqslant k+\ell$. Các bất đẳng thức

$$
|g^jh|\leqslant |h|+|g^{k+\ell}h|
$$

đúng với $0\leqslant j\leqslant k+\ell$, cho thấy dom($m^k_gm^{\ell}_{\overline{g}}$) bằng dom($m_{g^k\overline{g}^{\ell}}$), do đó có mệnh đề b).

### 10. Các mở rộng tự liên hợp của một toán tử đối xứng

Trong số này, chúng ta sẽ phân loại các mở rộng tự liên hợp của các toán tử đối xứng trên một không gian Hilbert phức, và đặc biệt xác định các điều kiện bảo đảm sự tồn tại của một mở rộng tự liên hợp của một toán tử như vậy.

Cho E là một không gian Hilbert phức. Với mọi toán tử bộ phận $u$ trên E, trong số này chúng ta sẽ viết $u+i$ và $u-i$ thay cho $u+i1_E$ và $u-i1_E$.

Cho $u$ là một toán tử đóng với miền xác định trù mật trên E. Ta nhắc lại (x. định nghĩa 4 của IV, p. 230 và mệnh đề 4 của IV, p. 230) rằng $E_u$ ký hiệu không gian Hilbert dom($u$) được trang bị dạng Hermit

$$
(x|y)_u=\langle x|y\rangle +\langle u(x)|u(y)\rangle
$$

Ta ký hiệu bởi $\|x\|_u$ chuẩn của một phần tử $x$ của không gian Hilbert $E_u$. Mọi không gian con của dom($u$) mà đóng trong E thì đóng trong $E_u($IV, p. 230, nhận xét 1).

#### Định nghĩa 10 {#ts-iv-s4-def-10 .statement tag=034A}

Cho $u$ là một toán tử đối xứng đóng trên một không gian Hilbert phức E. Đặt $E_+=$ Ker($u^*-i$) và $E_-=$ Ker($u^*+i$). Cặp $(E_+,E_-)$ các không gian con của dom($u^*$) được gọi là cặp khuyết của $u$. Các không gian con $E_+$ và $E_-$ là các không gian con đóng của E (mệnh đề 3 của IV, p. 229). Cặp (dim(E$_+$), dim(E$_-$)) các chiều Hilbert của các không gian con này được gọi là chỉ số khuyết của $u$.

#### Mệnh đề 25 {#ts-iv-s4-prop-25 .statement tag=034B}

Cho $u$ là một toán tử đối xứng đóng trên một không gian Hilbert phức E. Ta có

Ker($u^*-i$)$^{\circ}=$ Im($u+i$),

Ker($u^*+i$)$^{\circ}=$ Im($u-i$).

Theo mệnh đề 7, c) của IV, p. 236, chỉ cần chứng minh rằng ảnh của $u+i$ (tương ứng của $u-i$) là đóng trong E. Vì $u$ là đối xứng, ta có $\langle (u+i)(x)|(u+i)(y)\rangle = (x|y)_u$ với mọi $x$ và $y$ trong dom($u$). Do đó, ánh xạ $x\mapsto u(x) +ix$ từ $E_u$ vào E là đẳng cự. Ảnh của nó là đóng trong E (bổ đề 8 của I, p. 107). Vì đó cũng là ảnh của $u+i$, suy ra ảnh sau là đóng trong E. Tương tự, ảnh của $u-i$ là đóng trong E.

#### Bổ đề 7 {#ts-iv-s4-lem-7 .statement tag=034C}

Cho $u$ là một toán tử đối xứng đóng trên một không gian Hilbert phức E và $v$ là một mở rộng đối xứng đóng của $u$. Miền xác định của $u$ là một không gian con đóng của không gian Hilbert $E_v$.

Vì $v$ là một mở rộng của $u$, ta có $(x|y)_v= (x|y)_u$ với $x$ và $y$ thuộc dom($u$). Do đó đơn ánh chính tắc từ $E_u$ vào $E_v$ là đẳng cự, và kết luận suy ra (bổ đề 8 của I, p. 107).

#### Mệnh đề 26 {#ts-iv-s4-prop-26 .statement tag=034D}

Cho $u$ là một toán tử đối xứng đóng trên một không gian Hilbert phức E. Cho $(E_+,E_-)$ là cặp thiếu hụt của $u$. Các không gian $E_+,E_-$ và dom($u$) là các không gian con đóng đôi một trực giao của $E_{u^*}$ mà tổng Hilbert của chúng bằng $E_{u^*}$.

Vì $u$ là đối xứng, ta có $u\subset u^*$, nên không gian dom($u$) đóng trong $E_{u^*}$ (bổ đề 7). Các không gian con $E_+$ và $E_-$ đóng trong E và được chứa trong dom($u^*$), nên đóng trong $E_{u^*}$.

Cho $x\in E_+$. Ta có $u^*(x) =ix$, do đó $\langle x|u(y)\rangle =-i\langle x|y\rangle$ với mọi $y\in$ dom($u$). Do đó, với mọi $y\in$ dom($u$), ta có

$$
(x|y)_{u^*}=\langle x|y\rangle +\langle u^*(x)|u^*(y)\rangle =i(\langle x|u(y)\rangle  - \langle x|u^*(y)\rangle )= 0
$$

vì $u$ là đối xứng. Do đó các không gian $E_+$ và dom($u$) trực giao trong $E_{u^*}$. Tương tự, $E_-$ và dom($u$) trực giao trong $E_{u^*}$.

Cho $x\in E_+$ và $y\in E_-$. Khi đó

$$
(x|y)_{u^*}=\langle x|y\rangle +\langle u^*(x)|u^*(y)\rangle =\langle x|y\rangle  - \langle x|y\rangle = 0
$$

do đó $E_+$ và $E_-$ trực giao trong $E_{u^*}$.

Cho $x\in E_{u^*}$ trực giao với không gian con đóng dom($u$)$\oplus E_+\oplus E_-$. Với mọi $y\in$ dom($u$), ta có $u^*(y) =u(y)$ vì $u\subset u^*$, do đó

$$
0 = (x|y)_{u^*}=\langle x|y\rangle +\langle u^*(x)|u^*(y)\rangle =\langle x|y\rangle +\langle u^*(x)|u(y)\rangle
$$

Điều này kéo theo rằng $z=u^*(x)$ thuộc miền xác định của $u^*$ và thỏa mãn $u^*(z) =-x$. Đặt $x_-=z-ix$. Đây là một phần tử của dom($u^*$) thỏa mãn $u^*(x_-) =-x-iz=-ix_-$. Do đó $x_-$ thuộc $E_-$. Nhưng, với mọi $w\in E_-$, ta có

$$
-i\langle x_-|w\rangle =-i\langle z|w\rangle +\langle x|w\rangle
$$

$$
=\langle u^*(x)|u^*(w)\rangle +\langle x|w\rangle = (x|w)_{u^*}= 0
$$

Lấy $w=x_-$, ta suy ra $x_-= 0$, nghĩa là $z=ix$; vì $z=u^*(x)$, do đó ta có $x\in E_+$, suy ra $x$ = 0 vì $x$ trực giao với $E_+$ trong $E_{u^*}$. Điều này hoàn tất chứng minh rằng tổng trực tiếp dom($u$)$\oplus E_+\oplus E_-$ bằng $E_{u^*}$.

#### Hệ quả {#ts-iv-s4-n10-cor-1 .statement tag=034E}

Cho $u$ là một toán tử đối xứng đóng trên E. Khi đó $u$ là tự liên hợp nếu và chỉ nếu chỉ số thiếu hụt của $u$ bằng $(0,0)$.

Thật vậy, toán tử đối xứng $u$ là tự liên hợp nếu và chỉ nếu dom($u^*$) $=$ dom($u$); nay mệnh đề chứng minh rằng dom($u^*$) là tổng Hilbert của dom($u$) và các không gian con thiếu hụt của $u$.

Cho $u$ là một toán tử bộ phận đối xứng đóng. Phổ của $u$ được chứa trong $\mathbf{R}$ nếu và chỉ nếu $u$ là tự liên hợp. Thật vậy, đã biết rằng Sp($u$)$\subset \mathbf{R}$ nếu $u$ là tự liên hợp (Mệnh đề 17 của IV, p. 248); nếu $u$ không tự liên hợp thì một trong các không gian con Ker($u^*+i$) hoặc Ker($u^*-i$) là khác không, do đó ảnh của $u+i$ hoặc của $u-i$ là một không gian con thực sự của E (Mệnh đề 25 của IV, p. 256), vì thế $i$ hoặc $-i$ thuộc Sp($u$).

#### Định nghĩa 11 {#ts-iv-s4-def-11 .statement tag=034F}

Cho $u$ là một toán tử đối xứng đóng trên một không gian Hilbert phức E. Một điều kiện biên đối với $u$ là một ánh xạ tuyến tính đẳng cự bộ phận (TVS, V, p. 41, Định nghĩa 3) từ Ker($u^*-i$) vào Ker($u^*+i$).

Cho $u$ là một toán tử đối xứng đóng trên một không gian Hilbert phức E và $b$ là một điều kiện biên của $u$. Đặt I = Ker($b$)$^{\circ}$ là không gian con ban đầu của $b$. Ta ký hiệu bởi $u_b$ hạn chế của $u^*$ lên không gian con của dom($u^*$), là tổng trực tiếp của dom($u$) và của đồ thị trong $E_+\oplus E_-$ của hạn chế của $b$ lên I. Vì $E_{u^*}=$ dom($u$)$\oplus E_+\oplus E_-$ (Mệnh đề 26), toán tử bộ phận $u_b$ được xác định tốt.

Nói cách khác, miền xác định của $u_b$ là không gian các phần tử $x\in E$ có dạng $x=x_0+y+b(y)$, trong đó $x_0\in$ dom($u$) và $y$ thuộc không gian con ban đầu của $b$. Khi đó ta có $u_b(x_0+y+b(y)) =u(x_0) +iy-ib(y)$.

#### Định lý 1 (von Neumann) {#ts-iv-s4-thm-1 .statement tag=034G}

Cho $u$ là một toán tử đối xứng đóng trên một không gian Hilbert phức E và $(E_+,E_-)$ là cặp khuyết của nó.

a) Với mọi điều kiện biên $b$ của $u$, toán tử bộ phận $u_b$ là một mở rộng đối xứng đóng của $u$;

b) Ánh xạ $b\mapsto u_b$ là một song ánh từ tập hợp các điều kiện biên của $u$ lên tập hợp các mở rộng đối xứng đóng của $u$;

c) Với mọi điều kiện biên $b$ của $u$, ta có

Im($u_b+i$) $=$ Im($u+i$)$\oplus$ Im($b$)

Im($u_b-i$) $=$ Im($u-i$)$\oplus$ Ker($b$)$^{\circ}$;

d) Với mọi điều kiện biên $b$ của $u$, cặp khuyết của $u_b$ là (Ker($b$), Ker($b^*$)).

Cho $b$ là một điều kiện biên đối với $u$ và $I\subset E_+$ là không gian con ban đầu của nó. Hạn chế của $u^*$ lên $\Gamma_{b|I}\subset E_+\oplus E_-$ là ánh xạ tuyến tính liên tục được xác định bởi $x+b(x)\mapsto ix-ib(x)$ với $x\in I$. Đồ thị của $u_b$ là tổng trực tiếp của đồ thị của $u$ và đồ thị của ánh xạ tuyến tính này; do đó nó đóng. Toán tử đóng $u_b$ là một mở rộng của $u$ sao cho $u_b\subset u^*$.

Cho $\gamma_1$ và $\eta_1$ là các phần tử của I. Xét các phần tử

$$
\gamma =\gamma_1+b(\gamma_1),\eta =\eta_1+b(\eta_1)
$$

của đồ thị $\Gamma_{b|I}$. Ta tính được

$$
\langle \gamma |u^*(\eta )\rangle =i(\langle b(\gamma_1)|\eta_1\rangle  - \langle \gamma_1|b(\eta_1)\rangle )+i(\langle \gamma_1|\eta_1\rangle  - \langle b(\gamma_1)|b(\eta_1)\rangle )
$$

$$
=i(\langle b(\gamma_1)|\eta_1\rangle  - \langle \gamma_1|b(\eta_1)\rangle )
$$

vì $b$ là đẳng cự trên I. Suy ra ta có

$$
\langle u^*(\gamma )|\eta \rangle =\langle \gamma |u^*(\eta )\rangle \tag{12}
$$

với mọi $\gamma$ và $\eta$ trong $\Gamma_{b|I}$.

Cho $x$ và $y$ là các phần tử của dom($u$)$,\gamma$ và $\eta$ là các phần tử của $\Gamma_{b|I}$. Khi đó

$$
\langle x+\gamma |u_b(y+\eta )\rangle =\langle x|u(y)\rangle +\langle x|u^*(\eta )\rangle +\langle \gamma |u(y)\rangle +\langle \gamma |u^*(\eta )\rangle
$$

$$
=\langle u(x)|y\rangle +\langle u(x)|\eta \rangle +\langle u^*(\gamma )|y\rangle +\langle u^*(\gamma )|\eta \rangle
$$

$$
=\langle u_b(x+\gamma )|y+\eta \rangle
$$

trong đó ta đã dùng sự kiện $u$ là đối xứng và $\gamma$ và $\eta$ thuộc miền xác định của $u^*$, cũng như công thức (12). Vậy toán tử $u_b$ là một mở rộng đối xứng đóng của $u$. Mệnh đề a) được chứng minh.

Ánh xạ $b\mapsto u_b$ là đơn ánh. Thật vậy, một ánh xạ đẳng cự từng phần từ $E_+$ vào $E_-$ được xác định duy nhất bởi không gian con ban đầu của nó và bởi hạn chế của nó lên không gian con ấy. Mà miền xác định của $u_b$ xác định không gian con ban đầu I của $b$ và đồ thị của hạn chế của $b$ lên I.

Hãy chứng minh rằng ánh xạ $b\mapsto u_b$ là toàn ánh. Cho $w$ là một mở rộng đối xứng đóng của $u$. Ta có $w\subset w^*\subset u^*$. Vì vậy miền xác định của $w$ là một không gian con của dom($u^*$) chứa dom($u$), và $w$ là hạn chế của $u^*$ lên không gian con này. Cho G là giao của miền xác định của $w$ với $E_+\oplus E_-$. Đó là một không gian con đóng của $E_{u^*}$ (bổ đề 7) và ta có dom($w$) $=$ dom($u$)$\oplus G$ theo mệnh đề 26.

Cho $x\in E_+$ và $y\in E_-$ sao cho $x+y\in G$. Vì $w$ là đối xứng, và là hạn chế của $u^*$ lên dom($w$), nên ta có

$$
\langle x+y|u^*(x+y)\rangle =\langle u^*(x+y)|x+y\rangle
$$

Đẳng thức này tương đương với

$$
\langle x|ix\rangle +\langle x| -iy\rangle +\langle y|ix\rangle +\langle y| -iy\rangle
$$

$$
=\langle ix|x\rangle +\langle ix|y\rangle +\langle -iy|x\rangle +\langle -iy|y\rangle
$$

nghĩa là tương đương với $\|x\|^2=\|y\|^2$. Đặc biệt, phép chiếu chính tắc $p_+: G\rightarrow E_+$ là đơn ánh và, nếu I ký hiệu ảnh của nó, thì không gian G là đồ thị của một ánh xạ đẳng cự $b_0$ từ I vào $E_-$. Với $x$ trong I và $y$ trong $E_-$ sao cho $x+y\in G$, ta có

$$
\|x+y\|^2_{u^*}=\|x\|^2_{u^*}+\|y\|^2_{u^*}= 2(\|x\|^2+\|y\|^2)
$$

$$
= 4\|x\|^2= 4\|p_+(x+y)\|^2
$$

Do đó, khi xem G như một không gian con đóng của không gian Hilbert $E_{u^*}$, ánh xạ $x\mapsto \frac{1}{2}p_+(x)$ từ G vào I là một đẳng cự. Đặc biệt, I đóng trong $E_+$ (bổ đề 8 của I, p. 107). Khi đó tồn tại một điều kiện biên duy nhất $b$ cho $u$ mà không gian ban đầu là I và trùng với $b_0$ trên I. Ta có dom($w$) $=$ dom($u_b$), do đó $w=u_b$. Điều này thiết lập mệnh đề b).

Hãy chứng minh các mệnh đề c) và d). Cho $b$ là một điều kiện biên cho $u$ và I là không gian con ban đầu của nó. Với $x_0\in$ dom($u$) và $y\in I$, ta có

$$
u_b(x_0+y+b(y))-i(x_0+y+b(y)) = (u-i)(x_0)-2ib(y)
$$

Ta có Im($u-i$) $= E^{\circ}_-$ (mệnh đề 25). Vì ảnh của $b$ được chứa trong $E_-$, công thức này cho thấy Im($u_b-i$) $=$ Im($u-i$)$\oplus$ Im($b$). Theo loc. cit., do đó ta có Ker($u^*_b+i$) $= E_-\cap$ Im($b$)$^{\circ}=$ Ker($b^*$).

Tương tự, ta kiểm tra rằng Im($u_b+i$) $=$ Im($u+i$)$\oplus I$ và do đó (loc. cit.) rằng Ker($u^*_b-i$) $= I^{\circ}\cap E_+=$ Ker($b$).

#### Hệ quả 1 {#ts-iv-s4-thm-1-cor-1 .statement tag=034H}

Cho $u$ là một toán tử đối xứng đóng trên một không gian Hilbert phức E. Ánh xạ $b\mapsto u_b$ gây ra một song ánh từ tập hợp các đẳng cự từ Ker($u^*-i$) lên Ker($u^*+i$) lên tập hợp các mở rộng tự liên hợp của $u$. Đặc biệt, tồn tại một mở rộng tự liên hợp của $u$ khi và chỉ khi hai thành phần của chỉ số thiếu hụt của $u$ bằng nhau.

Điều này suy ra từ hệ quả của mệnh đề 26 và định lý trên, cùng với EVT, V, p. 25, cor. 2.

#### Hệ quả 2 {#ts-iv-s4-thm-1-cor-2 .statement tag=034I}

Cho E là một không gian Hilbert thực. Cho $u$ là một toán tử đối xứng đóng trên E. Toán tử bộ phận $u_{(\mathbf{C})}$ trên $E_{(\mathbf{C})}$ là đối xứng và đóng, và thừa nhận ít nhất một mở rộng tự liên hợp.

Toán tử bộ phận $u_{(\mathbf{C})}$ là đóng và đối xứng theo prop. 2 của IV, p. 228 và bổ đề 3 của IV, p. 239. Đẳng cấu $\mathbf{R}$-tuyến tính $j$ của $E_{(\mathbf{C})}$ lên $E_{(\mathbf{C})}$ sao cho $j(z\otimes x) =\overline{z}\otimes x$ với mọi $z\in \mathbf{C}$ và mọi $x\in E$ gây ra một đẳng cấu các không gian Hilbert từ Ker($u^*_{(\mathbf{C})}-i$) lên Ker($u^*_{(\mathbf{C})}+i$), và có thể áp dụng hệ quả 1.

#### Hệ quả 3 {#ts-iv-s4-thm-1-cor-3 .statement tag=034J}

Cho $u$ là một toán tử đối xứng trên E. Các điều kiện sau là tương đương:

(i) Toán tử $u$ là tự liên hợp cốt yếu;

(ii) Các không gian Ker($u^*+i$) và Ker($u^*-i$) bằng không;

(iii) Các không gian Im($u+i$) và Im($u-i$) là trù mật trong E;

(iv) Toán tử đối xứng bộ phận $u$ có một mở rộng tự liên hợp duy nhất.

Các điều kiện (ii) và (iii) là tương đương theo prop. 7, c) của IV, p. 236.

Toán tử bộ phận $u$ là tự liên hợp cốt yếu khi và chỉ khi $\overline{u}$ là tự liên hợp, nghĩa là khi Ker($\overline{u}^*-i$) $=$ Ker($\overline{u}^*+i$) $=\{0\}$ (hệ quả của prop. 26). Vì $\overline{u}^*=u^*$ (prop. 8 của IV, p. 237), nên điều kiện (i) do đó tương đương với điều kiện (ii). Hơn nữa, hệ quả trên cho thấy rằng (ii) kéo theo $u$ có một mở rộng tự liên hợp duy nhất, tức là điều kiện (iv).

Sau cùng, giả sử rằng $u$ có một mở rộng tự liên hợp duy nhất $v$. Khi đó điều tương tự cũng đúng với $\overline{u}$, vì mọi mở rộng tự liên hợp của $\overline{u}$ cũng là một mở rộng của $u$, nên bằng $v$. Theo hệ quả trên, các không gian Ker($\overline{u}^*+i$) và Ker($\overline{u}^*-i$) phải bằng không, do đó có điều kiện (ii), lại dùng $\overline{u}^*=u^*$.

#### Ví dụ {#ts-iv-s4-n10-exa-1 .statement tag=034K}

Cho U là một tập hợp mở của $\mathbf{R}^n$ được trang bị độ đo Lebesgue $\mu$. Cho Δ là toán tử vi phân vô hướng

$$
\Delta  =-\sum_{i=1}^n\partial_i^2
$$

trên U. Ta ký hiệu bởi $u$ toán tử bộ phận trên không gian Hilbert thực $L^2_{\mathbf{R}}(U, \mu)$ có miền xác định $\mathscr{D}_{\mathbf{R}}(U) ($IV, p. 201, nhận xét) được xác định bởi $\varphi \mapsto  -\sum^n_{i=1}\partial_i^2\varphi$. Ta có $u_{(\mathbf{C})}= \Delta_-$, là một toán tử bộ phận tiền đóng được (prop. 13 của IV, p. 242) và đối xứng (vì Δ đối xứng hình thức), do đó $u$ là tiền đóng được và đối xứng (mệnh đề 2 của IV, p. 228 và bổ đề 3 của IV, p. 239). Theo hệ quả trên, do đó tồn tại một mở rộng tự liên hợp của $u_{(\mathbf{C})}$. Nó là một Laplace trên U (IV, p. 243).

## BÀI TẬP {#ts-iv-s4-exercises}

Trừ khi có nói rõ khác đi, các không gian Banach và các không gian Hilbert dưới đây được giả thiết là phức.

Xem [các bài tập của § 4](exercises/s4/).

[^1]: Cần chú ý không nhầm khái niệm đồ thị được xét ở đây với khái niệm đã được đưa vào trong TA, II, p. 155, def. 1.
