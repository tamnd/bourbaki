---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 2
section_title: Free Lie algebras
lang: vi
source: lie-i-iii
pdf_pages: 0140-0154, 0199-0204
extraction: ocr
subsections:
    - "no": 1
      title: REVISION OF FREE ALGEBRAS
      page: 0
      pdf_page: 140
    - "no": 2
      title: CONSTRUCTION OF THE FREE LIE ALGEBRA
      page: 0
      pdf_page: 140
    - "no": 3
      title: PRESENTATIONS OF A LIE ALGEBRA
      page: 0
      pdf_page: 142
    - "no": 4
      title: LIE POLYNOMIALS AND SUBSTITUTIONS
      page: 0
      pdf_page: 142
    - "no": 5
      title: FUNCTORIAL PROPERTIES
      page: 0
      pdf_page: 143
    - "no": 6
      title: GRADUATIONS
      page: 0
      pdf_page: 144
    - "no": 7
      title: LOWER CENTRAL SERIES
      page: 0
      pdf_page: 146
    - "no": 8
      title: DERIVATIONS OF FREE LIE ALGEBRAS
      page: 0
      pdf_page: 147
    - "no": 9
      title: ELIMINATION THEOREM
      page: 0
      pdf_page: 148
    - "no": 10
      title: HALL SETS IN A FREE MAGMA
      page: 0
      pdf_page: 150
    - "no": 11
      title: HALL BASES OF A FREE LIE ALGEBRA
      page: 0
      pdf_page: 152
statements: 32
exercises: 10
content_sha256: a31d434aa4d23e5537e3a3d9c8f7431b1b1a37a5be81e86edd7698e60d345d84
translated_from: content/en/lie/II/02_s2_free_lie_algebras.md
source_content_sha256: c45ddbecbce1fdde54f20fa9b4671c2410f21271291967870bb4c5380ec1d17b
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-9fabf02a
glossary_version: 34
glossary_terms_sha256: 31d067bae360ee1deec29930d787a2c5c1c47f54ec88186a6745151f3889ea6d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. ĐẠI SỐ LIE TỰ DO

### 1. ÔN TẬP VỀ CÁC ĐẠI SỐ TỰ DO

Cho X là một tập hợp. Nhắc lại phép dựng nửa nhóm tự do M(X) được dựng trên X (Đại số, Chương I, § 7, no. 1). Bằng quy nạp theo số nguyên $n \geqslant 1$, ta định nghĩa các tập hợp $X_n$ bằng cách đặt $X_1 = X$ và lấy $X_n$ là tập hợp tổng của các tập hợp $X_p \times X_{n-p}$ với $p = 1, 2, \ldots, n-1$; nếu X là hữu hạn thì mỗi $X_n$ cũng hữu hạn. Tập hợp tổng của họ $(X_n)_{n \geqslant 1}$ được ký hiệu là M(X); mỗi tập hợp $X_n$ (và đặc biệt là X) được đồng nhất với một tập con của M(X). Cho w và $w'$ thuộc M(X); gọi p và q là các số nguyên sao cho $w \in X_p$ và $w' \in X_q$ và đặt $n = p + q$; ảnh của cặp có thứ tự $(w, w')$ qua đơn ánh chính tắc của $X_p \times X_{n-p}$ vào $X_n$ được ký hiệu là $w.w'$ và được gọi là tích của w và $w'$. Mọi ánh xạ từ X vào một nửa nhóm M đều có thể được mở rộng duy nhất thành một đồng cấu nửa nhóm từ M(X) vào M.

Cho w thuộc M(X); số nguyên duy nhất n sao cho $w \in X_n$ được gọi là độ dài của w và ký hiệu là $l(w)$. Khi đó $l(w.w') = l(w) + l(w')$ đối với w, $w'$ thuộc M(X). Tập hợp X là tập con của M(X) gồm các phần tử có độ dài 1. Mọi phần tử w có độ dài $\geqslant 2$ đều có thể được viết duy nhất dưới dạng $w = w'.w''$.

Đại số của nửa nhóm M(X) với các hệ số trong vành K được ký hiệu là Lib(X), hoặc Lib_K(X) khi cần chỉ ra vành K. Tập hợp M(X) là một cơ sở của K-môđun Lib(X) và do đó X sẽ được đồng nhất với một tập con của Lib(X). Nếu A là một đại số, mọi ánh xạ từ X vào A đều có thể được mở rộng duy nhất thành một đồng cấu từ Lib(X) vào A (Đại số, Chương III, § 2, no. 7, Mệnh đề 7).

### 2. PHÉP DỰNG ĐẠI SỐ LIE TỰ DO

#### Định nghĩa 1 {#lie-ii-s2-def-1 .statement}

*Đại số Lie tự do trên tập hợp X là đại số thương*
$$
L(X) = \mathrm{Lib}(X)/a,
$$
trong đó a là iđêan hai phía của Lib(X) sinh bởi các phần tử có một trong các dạng
(1)
$$
Q(a) = a.a \quad \text{cho } a \text{ trong } \mathrm{Lib}(X),
$$
(2)
$$
J(a, b, c) = a.(b.c) + b.(c.a) + c.(a.b)
$$
với $a, b, c$ trong $\mathrm{Lib}(X)$.

Rõ ràng $L(X)$ là một đại số Lie K; hợp thành của hai phần tử $u, v$ của $L(X)$ sẽ được ký hiệu là $[u, v]$. Khi cần chỉ ra vành K, ta viết $L_K(X)$ cho $L(X)$.

Mệnh đề sau đây giải thích tên gọi *tự do* của đại số Lie $L(X)$.

#### Mệnh đề 1 {#lie-ii-s2-prop-1 .statement}

*Cho $\psi$ là ánh xạ chính tắc của Lib(X) lên $L(X)$ và $\phi$ là hạn chế của $\psi$ trên X. Với mọi ánh xạ f từ X vào một đại số Lie $g$, tồn tại duy nhất một đồng cấu F: $L(X) \to g$ sao cho $f = F \circ \phi$.*

(a) *Sự tồn tại của F*: cho h là đồng cấu từ Lib(X) vào $g$ mở rộng f (no. 1). Với mọi $a$ trong Lib(X), $h(Q(a)) = h(a.a) = [h(a), h(a)] = 0$; tương tự, đồng nhất thức Jacobi thỏa mãn bởi $g$ kéo theo rằng $h(J(a, b, c)) = 0$ với $a, b, c$ trong Lib(X). Suy ra rằng $h(a) = 0$, do đó tồn tại một đồng cấu F từ $L(X)$ vào $g$ sao cho $h = F \circ \psi$. Bằng cách hạn chế trên X, ta thu được $f = F \circ \phi$.

(b) *Tính duy nhất của F*: cho $F': L(X) \to g$ là một đồng cấu sao cho $f = F' \circ \phi$. Các đồng cấu $F \circ \psi$ và $F' \circ \psi$ từ Lib(X) vào $g$ trùng nhau trên X và do đó bằng nhau; vì $\psi$ là toàn ánh, $F = F'$.

#### Hệ quả 1 {#lie-ii-s2-prop-1-cor-1 .statement}

*Họ $(\phi(x))_{x \in X}$ là tự do trên K trong $L(X)$.*

Cho $x_1, x_2, \ldots, x_n$ là các phần tử phân biệt của X và $\lambda_1, \ldots, \lambda_n$ là các phần tử của K sao cho

$$
\lambda_1 \cdot \phi(x_1) + \cdots + \lambda_n \cdot \phi(x_n) = 0.
$$

Cho $g$ là đại số Lie giao hoán có K làm môđun nền. Với $i = 1, 2, \ldots, n$, tồn tại một đồng cấu $F_i$ từ $L(X)$ vào $g$ sao cho $F_i(\phi(x_i)) = 1$ và $F_i(\phi(x)) = 0$ với $x \neq x_i$ (Mệnh đề 1); áp dụng $F_i$ vào quan hệ (3), ta thu được $\lambda_i = 0$.

#### Hệ quả 2 {#lie-ii-s2-prop-1-cor-2 .statement}

*Cho $a$ là một đại số Lie. Mọi mở rộng của $L(X)$ bởi $a$ đều là không thiết yếu.*

Cho $a \xrightarrow{\lambda} g \xrightarrow{\mu} L(X)$ là một mở rộng như vậy (Chương I, § 1, no. 7). Vì $\mu$ là toàn ánh, tồn tại một ánh xạ f từ X vào $g$ sao cho $\phi = \mu \circ f$. Cho F là đồng cấu từ $L(X)$ vào $g$ sao cho $f = F \circ \phi$ (Mệnh đề 1). Khi đó $(\mu \circ F) \circ \phi = \mu \circ f = \phi$ và Mệnh đề 1 cho thấy rằng $\mu \circ F$ là tự đẳng cấu đồng nhất của $L(X)$. Do đó mở rộng đã cho là không thiết yếu (Chương I, § 1, no. 7, Mệnh đề 6 và Định nghĩa 6).

Vì vành K là khác không, Hệ quả 1 của Mệnh đề 1 cho thấy rằng $\phi$ là đơn ánh. *Do đó tập hợp X có thể được đồng nhất bằng $\phi$ với ảnh của nó trong $L(X)$*; với quy ước này, X sinh $L(X)$ và mọi ánh xạ từ X vào một đại số Lie $g$ *có thể được mở rộng* thành một đồng cấu đại số Lie từ $L(X)$ vào $g$.

#### Nhận xét {#lie-ii-s2-n2-rem-1 .statement}

Khi X là rỗng, $M(X)$ là rỗng và do đó $L(X) = \{0\}$. Nếu X gồm một phần tử duy nhất $x$, môđun con $K.x$ của $L(X)$ là một đại số con Lie của

L(X); vì X sinh $L(X)$, Hệ quả 1 của Mệnh đề 1 cho thấy rằng L(X) là một môđun tự do với cơ sở {x}.

### 3. CÁC BIỂU DIỄN CỦA MỘT ĐẠI SỐ LIE

Cho g là một đại số Lie và $a = (a_i)_{i \in I}$ là một họ các phần tử của g. Cho $f_a$ là đồng cấu từ $L(I)$ vào g ánh xạ mỗi $i \in I$ thành $a_i$. Ảnh của $f_a$ là đại số con của g sinh bởi a; các phần tử của hạt nhân của $f_a$ được gọi là các quan hệ của họ a. Họ a được gọi là sinh (tương ứng tự do, cơ bản) nếu $f_a$ là toàn ánh (tương ứng đơn ánh, song ánh).

Cho g là một đại số Lie. Một *trình bày* của g là một cặp có thứ tự $(a, r)$ gồm một họ sinh $a = (a_i)_{i \in I}$ và một họ $r = (r_j)_{j \in J}$ các quan hệ của $a$ sinh iđêan của $L(I)$ là hạt nhân của $f_a$. Ta cũng nói rằng g được trình bày bởi họ $a$ liên quan bởi các quan hệ $r_j$ ($j \in J$).

Cho I là một tập hợp và $r = (r_j)_{j \in J}$ là một họ các phần tử của đại số Lie tự do $L(I)$; gọi $a_r$ là iđêan của $L(I)$ sinh bởi $r$. Đại số thương $L(I, r) = L(I)/a_r$ được gọi là đại số Lie được xác định bởi I và họ các quan hệ $(r_j)_{j \in J}$; ta cũng nói rằng $L(I, r)$ được xác định bởi trình bày (I, r), hoặc cũng bởi $(I; (r_j = 0)_{j \in J})$. Khi họ $r$ rỗng, $L(I, r) = L(I)$.

Cho I và $r$ như trên; gọi $\xi_i$ là ảnh của i trong $L(I, r)$. Họ sinh $\xi = (\xi_i)_{i \in I}$ và họ các quan hệ $r$ lập thành một trình bày của $L(I, r)$. Ngược lại, nếu g là một đại số Lie và $(a, r)$, trong đó $a = (a_i)_{i \in I}$, là một trình bày của g, thì tồn tại duy nhất một đẳng cấu $u : L(I, r) \to g$ sao cho $u(\xi_i) = a_i$ với mọi $i \in I$.

### 4. ĐA THỨC LIE VÀ PHÉP THẾ

Cho I là một tập hợp. Gọi $T_i$ là ảnh chính tắc của phần tử i của I trong $L(I)$ (đôi khi cũng được ký hiệu bởi $L((T_i)_{i \in I})$); các phần tử của $L(I)$ được gọi là *đa thức Lie* theo các bất định $(T_i)_{i \in I}$.

Cho g là một đại số Lie. Nếu $t = (t_i)_{i \in I}$ là một họ các phần tử của g, gọi $f_t$ là đồng cấu từ $L(I)$ vào g sao cho $f_t(T_i) = t_i$ với $i \in I$ (no. 2, Mệnh đề 1). Ảnh qua $f_t$ của phần tử P của $L(I)$ được ký hiệu bởi $P((t_i)_{i \in I})$. Đặc biệt, $P((T_i)_{i \in I}) = P$; phần tử $P((t_i)_{i \in I})$ nói trên đôi khi được gọi là phần tử của g thu được bằng cách thế các $t_i$ cho các $T_i$ trong đa thức Lie $P((T_i)_{i \in I})$.

Cho $\sigma : g \to g'$ là một đồng cấu đại số Lie. Với mọi họ $t = (t_i)_{i \in I}$ các phần tử của g và mọi $P \in L(I)$,

$$
\sigma(P((t_i)_{i \in I})) = P((\sigma(t_i))_{i \in I}),
$$

vì $\sigma \circ f_t$ biến $T_i$ thành $\sigma(t_i)$ với $i \in I$.

Cho $(Q_j)_{j \in J}$ là một họ các phần tử của $L(I)$ và cho $P \in L(J)$. Bằng cách thế các $Q_j$ cho các $T_j$ trong P, ta thu được một đa thức Lie R = P((Q_j)_{j \in J}) \in L(I). Khi đó

(5)
$$
R((t_i)_{i \in I}) = P((Q_j((t_i)_{i \in I}))_{j \in J})
$$
với mọi họ $t = (t_i)_{i \in I}$ các phần tử của một đại số Lie g, như thấy được bằng cách tác động đồng cấu $f_t$ lên đẳng thức $R = P((Q_j)_{j \in J})$ và sử dụng (4).

Cho g là một đại số Lie, I là một tập hợp hữu hạn và $P \in L(I)$. Giả sử rằng g là một K-môđun tự do. Ánh xạ
$$
\tilde{P} : g^I \to g
$$
được xác định bởi $\tilde{P}((t_i)_{i \in I}) = P((t_i)_{i \in I})$ khi đó là *đa thức.*† Đối với tập hợp F các ánh xạ từ $g^I$ vào g là một đại số Lie với móc được xác định bởi
$$
[\phi, \psi](t) = [\phi(t), \psi(t)];
$$
tập hợp F' các ánh xạ đa thức từ $g^I$ vào g là một đại số con Lie của F do tính song tuyến tính của móc. Mệnh đề của chúng ta khi đó suy ra từ sự kiện rằng ánh xạ $P \mapsto \tilde{P}$ là một đồng cấu đại số Lie và $\tilde{T}_i = \mathrm{pr}_i \in F'$ với mọi i.

### 5. CÁC TÍNH CHẤT HÀM TỬ

#### Mệnh đề 2 {#lie-ii-s2-prop-2 .statement}

Cho X và Y là hai tập hợp. Mọi ánh xạ $u : X \to Y$ có thể được mở rộng duy nhất thành một đồng cấu đại số Lie $L(u) : L(X) \to L(Y)$. Với mọi ánh xạ $v : Y \to Z$, $L(v \circ u) = L(v) \circ L(u)$.

Sự tồn tại và tính duy nhất của $L(u)$ suy ra từ Mệnh đề 1 của No. 2. Các đồng cấu $L(v \circ u)$ và $L(v) \circ L(u)$ có cùng hạn chế lên X và do đó bằng nhau (Mệnh đề 1).

#### Hệ quả {#lie-ii-s2-n5-cor-1 .statement}

Nếu u là đơn ánh (tương ứng toàn ánh, song ánh), thì $L(u)$ cũng vậy.

Vì mệnh đề là tầm thường đối với $X = \varnothing$, ta giả sử $X \neq \varnothing$. Nếu u là đơn ánh thì tồn tại một ánh xạ v từ Y vào X sao cho $v \circ u$ là ánh xạ đồng nhất của X; theo Mệnh đề 2, $L(v) \circ L(u)$ là tự đẳng cấu đồng nhất của $L(X)$ và do đó $L(u)$ là đơn ánh. Khi u là toàn ánh, tồn tại một ánh xạ w từ Y vào X sao cho $u \circ w$ là ánh xạ đồng nhất của Y; khi đó $L(u) \circ L(w)$ là ánh xạ đồng nhất của $L(Y)$, điều này chứng minh rằng $L(u)$ là toàn ánh.

† Nhắc lại (Đại số, Chương IV, § 5, No. 10) định nghĩa của các ánh xạ đa thức từ một môđun tự do M vào một môđun N: nếu q là một số nguyên $\geq 0$, một ánh xạ $f : M \to N$ được gọi là *đa thức thuần nhất bậc* q nếu tồn tại một ánh xạ đa tuyến tính u từ $M^q$ vào N sao cho
$$
f(x) = u(x, \ldots, x) \quad \text{với mọi } x \in M.
$$
Một ánh xạ từ M vào N được gọi là *đa thức* nếu nó là một tổng hữu hạn của các ánh xạ đa thức thuần nhất với các bậc thích hợp.

Cho X là một tập hợp và S là một tập con của X. Hệ quả trên cho thấy rằng đơn ánh chính tắc của S vào X có thể được mở rộng thành một đẳng cấu $\alpha$ từ $L(S)$ lên đại số con Lie $L'(S)$ của $L(X)$ được sinh bởi S; *ta sẽ đồng nhất* $L(S)$ *và* $L'(S)$ *bằng cách sử dụng* $\alpha$.

Cho $(S_\alpha)_{\alpha \in I}$ là một *họ có hướng phải* các tập con của X có hợp là S. Quan hệ $S_\alpha \subset S_\beta$ kéo theo $L(S_\alpha) \subset L(S_\beta)$ và do đó họ các đại số con Lie $L(S_\alpha)$ của $L(X)$ là có hướng phải. Vì vậy $g = \bigcup_{\alpha \in I} L(S_\alpha)$ là một đại số con Lie của $L(X)$; khi đó $S \subset g$, do đó $L(S) \subset g$, và, vì $L(S_\alpha) \subset L(S)$ với mọi $\alpha \in I$, ta có $g \subset L(S)$. Suy ra

$$
L\left( \bigcup_{\alpha \in I} S_\alpha \right) = \bigcup_{\alpha \in I} L(S_\alpha)
$$

với mọi *họ có hướng phải* $(S_\alpha)_{\alpha \in I}$ các tập con của X.

Áp dụng điều trên cho họ các tập con hữu hạn của X, ta thấy rằng mọi phần tử của $L(X)$ đều có dạng $P(x_1, \ldots, x_n)$ trong đó P là một đa thức Lie theo n biến không xác định và $x_1, \ldots, x_n$ là các phần tử của X.

#### Mệnh đề 3 {#lie-ii-s2-prop-3 .statement}

*Cho $K'$ là một vành giao hoán khác không và $u : K \to K'$ là một đồng cấu vành. Với mọi tập hợp X tồn tại duy nhất một đồng cấu đại số Lie $K'$*

$$
v : L_K(X) \otimes K' \to L_{K'}(X)
$$

*có tính chất* $v(x \otimes 1) = x$ *với* $x \in X$. *Hơn nữa, v là một đẳng cấu.*

Áp dụng Mệnh đề 1 cho $g = L_{K'}(X)$ được xét như một đại số Lie trên K và ánh xạ $x \mapsto x$ của X vào g, ta thu được một K-đồng cấu $L_K(X) \to L_{K'}(X)$, do đó tồn tại một $K'$-đồng cấu $v : L_K(X) \otimes K' \to L_{K'}(X)$. Sự kiện v là duy nhất và là một đẳng cấu suy ra từ sự kiện rằng cặp có thứ tự $(L_K(X) \otimes K', x \mapsto x \otimes 1)$ là một nghiệm của cùng một bài toán ánh xạ phổ quát như cặp có thứ tự $(L_{K'}(X), x \mapsto x)$.

#### Nhận xét {#lie-ii-s2-n5-rem-1 .statement}

Cho $\mathfrak{h}'$ là một đại số Lie trên $K'$ và $\mathfrak{h}$ là đại số Lie trên K dẫn xuất từ $\mathfrak{h}'$ bằng cách hạn chế vành các vô hướng. Nếu $P \in L_K(X)$, ta có thể định nghĩa $\tilde{P} : \mathfrak{h}^X \to \mathfrak{h}$ (no. 4). Ta thấy ngay lập tức rằng

$$
\tilde{P} = (v(P \otimes 1))^{-}.
$$

### 6. PHÂN BẬC

Cho $\Delta$ là một nửa nhóm giao hoán, được viết cộng. Gọi $\phi_0$ là một ánh xạ của X vào $\Delta$ và $\phi$ là đồng cấu của magma tự do $M(X)$ vào $\Delta$ mở rộng $\phi_0$. Với mọi $\delta \in \Delta$, gọi $\mathrm{Lib}^\delta(X)$ là môđun con của $\mathrm{Lib}(X)$ có cơ sở là tập con $\phi^{-1}(\delta)$ của $M(X)$. Họ $(\mathrm{Lib}^\delta(X))_{\delta \in \Delta}$ là một phân bậc của đại số $\mathrm{Lib}(X)$, nghĩa là

$$
\mathrm{Lib}(X) = \bigoplus_{\delta \in \Delta} \mathrm{Lib}^\delta(X)
$$
$$
\mathrm{Lib}^\delta(X) \cdot \mathrm{Lib}^{\delta'}(X) \subset \mathrm{Lib}^{\delta + \delta'}(X) \quad \text{cho } \delta, \delta' \text{ trong } \Delta
$$

#### Bổ đề 1 {#lie-ii-s2-lem-1 .statement}

Iđêan $a$ của Định nghĩa 1 là phân bậc.
Với $a, b$ trong Lib(X), đặt $B(a, b) = a.b + b.a$. Các công thức
$$
(10)\quad B(a, b) = Q(a + b) - Q(a) - Q(b)
$$
$$
(11)\quad Q(\lambda_1.w_1 + \cdots + \lambda_n.w_n) = \sum_i \lambda_i^2 Q(w_i) + \sum_{i < j} \lambda_i \lambda_j B(w_i, w_j)
$$
với $w_1, \ldots, w_n$ trong $M(X)$ và $\lambda_1, \ldots, \lambda_n$ trong $K$, chỉ ra rằng các họ $(Q(a))_{a \in \mathrm{Lib}(X)}$ và $(Q(w), B(w, w'))_{w, w' \in M(X)}$ sinh cùng một môđun con của $\mathrm{Lib}(X)$. Vì J là tam tuyến tính nên iđêan $a$ được sinh bởi các phần tử thuần nhất $Q(w), B(w, w')$ và $J(w, w', w'')$, trong đó $w, w', w''$ trong $M(X)$, và do đó là phân bậc (Algebra, Chapter III, § 3, no. 3, Proposition 1).

Cho đại số Lie $L(X) = \mathrm{Lib}(X)/a$ được trang bị phân bậc thương. Thành phần thuần nhất của $L(X)$ có bậc $\delta$ được ký hiệu bởi $L^\delta(X)$; nó là môđun con của $L(X)$ được sinh bởi các ảnh của các phần tử $w \in M(X)$ sao cho $\phi(w) = \delta$.

Chúng ta sẽ sử dụng đặc biệt hai trường hợp sau:
(a) *Phân bậc toàn phần*: ta lấy $\Delta = \mathbf{N}$ và $\phi_0(x) = 1$ với mọi $x \in X$, do đó $\phi(w) = l(w)$ đối với $w$ trong $M(X)$. K-môđun $L^n(X)$ được sinh bởi các ảnh của các phần tử có độ dài $n$ trong $M(X)$, mà ta sẽ gọi là *các phần tử xen kẽ có bậc n*. Sau này ta sẽ thấy rằng môđun $L^n(X)$ là tự do và nhận một cơ sở gồm các phần tử xen kẽ có bậc $n$ (no. 11, Định lý 1). Khi đó $L(X) = \bigoplus_{n \geq 1} L^n(X)$ và $L^1(X)$ nhận $X$ làm cơ sở (no. 2, Hệ quả 1 đối với Mệnh đề 1). Theo phép dựng $M(X)$,
$$
(12)\quad L^n(X) = \sum_{p=1}^{n-1} [L^p(X), L^{n-p}(X)]
$$
và đặc biệt
$$
(13)\quad [L^m(X), L^n(X)] \subset L^{m+n}(X).
$$

(b) *Phân bậc đa*: ta lấy $\Delta$ là nửa nhóm giao hoán tự do $\mathbf{N}^{(X)}$ được dựng trên $X$. Ánh xạ $\phi_0$ từ $X$ vào $\Delta$ được xác định bởi $(\phi_0(x))(x') = \delta_{xx'}$, trong đó $\delta_{xx'}$ là ký hiệu Kronecker. Đối với $w \in M(X)$ và $x \in X$, số nguyên $(\phi(w))(x)$ là "số lần xuất hiện của chữ cái $x$ trong $w$". Đối với $\alpha$ trong $\mathbf{N}^{(X)}$, ta viết $|\alpha| = \sum_{x \in X} \alpha(x)$, do đó $|\phi(w)| = l(w)$ với mọi $w$ trong $M(X)$. Suy ra rằng
$$
(14)\quad L^n(X) = \bigoplus_{|\alpha|=n} L^\alpha(X);
$$
hiển nhiên
$$
(15)\quad [L^\alpha(X), L^\beta(X)] \subset L^{\alpha+\beta}(X) \quad \text{đối với } \alpha, \beta \text{ trong } \mathbf{N}^{(X)}.
$$

#### Mệnh đề 4 {#lie-ii-s2-prop-4 .statement}

Cho S là một tập con của X. Nếu $\mathbf{N}^{(S)}$ được đồng nhất với ảnh chính tắc của nó trong $\mathbf{N}^{(X)}$ (Algebra, Chapter I, § 7, no. 7), thì $L(S) = \sum_{\alpha \in \mathbf{N}^{(S)}} L^\alpha(X)$. Hơn nữa, với mọi $\alpha \in \mathbf{N}^{(S)}$, thành phần thuần nhất có bậc $\alpha$ dưới phép phân bậc đa trên $L(S)$ bằng $L^\alpha(X)$.

Cho $\alpha \in \mathbf{N}^{(S)}$. Môđun $L^\alpha(S)$ được sinh bởi các ảnh trong $L(X)$ của các phần tử $w$ trong $M(S)$ sao cho $\phi(w) = \alpha$, nghĩa là (Algebra, § 7, no. 9, các công thức (23) và (24)) tập hợp các $w$ trong $M(X)$ sao cho $\phi(w) = \alpha$. Do đó $L^\alpha(S) = L^\alpha(X)$.

Mệnh đề suy ra từ điều này và quan hệ $L(S) = \sum_{\alpha \in \mathbf{N}^{(S)}} L^\alpha(S)$.

#### Hệ quả {#lie-ii-s2-n6-cor-1 .statement}

Với mọi họ $(S_i)_{i \in I}$ các tập con của X,
$$
L\left(\bigcap_{i \in I} S_i\right) = \bigcap_{i \in I} L(S_i).
$$
Điều này suy ra từ Mệnh đề 4 và công thức hiển nhiên
$$
\mathbf{N}^{(S)} = \bigcap_{i \in I} \mathbf{N}^{(S_i)}
$$
trong đó ta đã viết $S = \bigcap_{i \in I} S_i$.

### 7. CHUỖI TRUNG TÂM DƯỚI

#### Mệnh đề 5 {#lie-ii-s2-prop-5 .statement}

Cho $g$ là một đại số Lie và $P$ là một môđun con của $g$. Ta định nghĩa các môđun con $P_n$ của $g$ bởi các công thức $P_1 = P$ và $P_{n+1} = [P, P_n]$ với $n \geq 1$. Khi đó
$$
[P_m, P_n] \subset P_{m+n},
$$
$$
P_n = \sum_{p=1}^{n-1} [P_p, P_{n-p}] \quad \text{với } n \geq 2.
$$
Ta chứng minh (18) bằng quy nạp theo $m$. Trường hợp $m = 1$ là hiển nhiên. Theo đồng nhất thức Jacobi,
$$
[[P, P_m], P_n] \subset [P_m, [P, P_n]] + [P, [P_m, P_n]],
$$
nghĩa là
$$
[P_{m+1}, P_n] \subset [P_m, P_{n+1}] + [P, [P_m, P_n]].
$$
Giả thiết quy nạp suy ra rằng $[P_m, P_{n+1}] \subset P_{m+n+1}$ và $[P_m, P_n] \subset P_{m+n}$, do đó
$$
[P_{m+1}, P_n] \subset P_{m+n+1} + [P, P_{m+n}] = P_{m+n+1}.
$$
Theo công thức (18), $P_n \supset \sum_{p=1}^{n-1} [P_p, P_{n-p}] \supset [P_1, P_{n-1}] = P_n$, do đó (19).

Khi ta lấy $P = g$, dãy $(P_n)$ là chuỗi trung tâm dưới ($\mathcal{C}^n g$) của $g$ (Chương I, § 1, no. 5). Do đó:

#### Mệnh đề 6 {#lie-ii-s2-prop-6 .statement}

Cho $g$ là một đại số Lie và $(\mathcal{C}^n g)_{n \geq 1}$ là chuỗi trung tâm dưới của $g$. Khi đó
$$
[\mathcal{C}^m g, \mathcal{C}^n g] \subset \mathcal{C}^{m+n} g \quad \text{với } m \geq 1 \text{ và } n \geq 1.
$$

Tổng quát hóa Định nghĩa 1 của Chương I, § 4, no. 1, ta sẽ nói rằng một đại số Lie $g$ là *lũy linh* nếu $\mathcal{C}^n g = \{0\}$ với $n$ đủ lớn. *Lớp lũy linh* của một đại số Lie lũy linh $g$ là số nguyên nhỏ nhất $n$ sao cho $\mathcal{C}^{n+1} g = \{0\}$.

#### Mệnh đề 7 {#lie-ii-s2-prop-7 .statement}

Cho $X$ là một tập hợp và $n$ là một số nguyên $\geq 1$.
(a) $L^{n+1}(X) = [L^1(X), L^n(X)]$.
(b) *Môđun* $L^n(X)$ *được sinh bởi các phần tử* $[x_1, [x_2, \ldots, [x_{n-1}, x_n] \ldots]]$
*trong đó* $(x_1, \ldots, x_n)$ *chạy qua tập hợp các dãy gồm* $n$ *phần tử của* $X$.
(c) *Chuỗi trung tâm dưới của* $L(X)$ *được cho bởi* $\mathcal{C}^n(L(X)) = \sum_{p \geq n} L^p(X)$.

(a) Ta áp dụng Mệnh đề 5 với $g = L(X)$ và $P = L^1(X)$. Bằng quy nạp theo $n$, từ (12) (no. 6) và (19) ta suy ra đẳng thức $P_n = L^n(X)$. Quan hệ cần chứng minh khi đó tương đương với định nghĩa $[P, P_n] = P_{n+1}$.
(b) Điều này suy ra từ (a) bằng quy nạp theo $n$.
(c) Cho $g = L(X)$ và $g_n = \sum_{p \geq n} L_p(X)$. Khi đó $g = g_1$ và công thức (13) của no. 6 suy ra $[g_n, g_m] \subset g_{n+m}$ và đặc biệt $[g, g_n] \subset g_{n+1}$. Bằng quy nạp theo $n$, $\mathcal{C}^n g \subset g_n$. Mặt khác, từ (a) ta suy ra $L^n(X) \subset \mathcal{C}^n g$ bằng quy nạp theo $n$. Vì $\mathcal{C}^n g$ là một iđêan của $g$, quan hệ $L^p(X) \subset \mathcal{C}^n g$ suy ra rằng
$$
L^{p+1}(X) = [L^1(X), L^p(X)] \subset \mathcal{C}^n g
$$
theo (a). Do đó $L^p(X) \subset \mathcal{C}^n g$ với $p \geq n$, do đó $g_n \subset \mathcal{C}^n g$.

#### Hệ quả {#lie-ii-s2-n7-cor-1 .statement}

Cho $g$ là một đại số Lie và $(x_i)_{i \in I}$ là một họ sinh của $g$. Số hạng thứ $n$ $\mathcal{C}^n g$ của chuỗi tâm dưới của $g$ là môđun sinh bởi các ngoặc lồng nhau $[x_{i_1}, [x_{i_2}, \ldots, [x_{i_{p-1}}, x_{i_p}] \ldots]]$ với $p \geq n$, và $i_1, \ldots, i_p$ thuộc $I$.
Cho $f$ là đồng cấu từ $L(I)$ vào $g$ sao cho $f(i) = x_i$ với mọi $i \in I$. Vì $(x_i)_{i \in I}$ sinh $g$, nên $g = f(L(I))$, do đó $\mathcal{C}^n g = f(\mathcal{C}^n(L(I)))$ theo Mệnh đề 4 của Chương I, § 1, no. 5. Hệ quả suy ra từ các khẳng định (b) và (c) của Mệnh đề 7.

### 8. CÁC ĐẠO HÀM CỦA CÁC ĐẠI SỐ LIE TỰ DO

#### Mệnh đề 8 {#lie-ii-s2-prop-8 .statement}

Cho $X$ là một tập hợp, $M$ là một $L(X)$-môđun và $d$ là một ánh xạ từ $X$ vào $M$. Tồn tại duy nhất một ánh xạ tuyến tính $D$ từ $L(X)$ vào $M$ mở rộng $d$ và thỏa mãn quan hệ:
$$
D([a, a']) = a.D(a') - a'.D(a) \quad \text{với } a, a' \text{ trong } L(X).
$$
Ta định nghĩa một đại số Lie $g$ với môđun cơ sở $M \times L(X)$ bằng ngoặc
$$
[(m, a), (m', a')] = (a.m' - a'.m, [a, a']),
$$

với $a, a'$ thuộc $L(X)$ và $m, m'$ thuộc $M$ (Chương I, § 1, No. 8). Cho $f$ là đồng cấu của $L(X)$ vào $g$ sao cho $f(x) = (d(x), x)$ với mọi $x$ thuộc $X$; cho $f(a) = (D(a), u(a))$ với mọi $a$ thuộc $L(X)$. Theo công thức (21), $u$ là một đồng cấu của $L(X)$ vào chính nó; vì $u(x) = x$ với $x$ thuộc $X$, nên $u(a) = a$ với mọi $a$ thuộc $L(X)$, do đó

$$(22)$$
$$f(a) = (D(a), a).$$

Theo (21) và (22), quan hệ (20) suy ra từ $f([a, a']) = [f(a), f(a')]$.

Ngược lại, cho $D'$ là một ánh xạ của $L(X)$ vào $M$ thỏa mãn quan hệ (20') tương tự như (20) và mở rộng $d$. Cho $f'(a) = (D'(a), a)$ với $a \in L(X)$; theo (20') và (21), $f'$ là một đồng cấu của $L(X)$ vào $g$, trùng với $f$ trên $X$, do đó $f' = f$ và $D' = D$.

#### Hệ quả {#lie-ii-s2-n8-cor-1 .statement}

*Mọi ánh xạ của $X$ vào $L(X)$ đều mở rộng duy nhất thành một đạo hàm của $L(X)$*.

Khi $M$ bằng $L(X)$ với biểu diễn phụ hợp, quan hệ (20) có nghĩa là $D$ là một đạo hàm.

### 9. ĐỊNH LÝ LOẠI BỎ

#### Mệnh đề 9 {#lie-ii-s2-prop-9 .statement}

*Cho $S_1$ và $S_2$ là hai tập hợp rời nhau và $d$ là một ánh xạ của $S_1 \times S_2$ vào $L(S_2)$. Cho $g$ là đại số Lie thương của $L(S_1 \cup S_2)$ theo iđêan sinh bởi các phần tử $[s_1, s_2] - d(s_1, s_2)$ với $s_1 \in S_1, s_2 \in S_2$; cho $\psi$ là ánh xạ chính tắc của $L(S_1 \cup S_2)$ lên $g$.*

(a) *Với $i = 1, 2$, hạn chế $\phi_i$ của $\psi$ trên $S_i$ có thể được mở rộng thành một đẳng cấu của $L(S_i)$ lên một đại số con $a_i$ của $g$.

(b) $g = a_1 + a_2, a_1 \cap a_2 = \{0\}$ và $a_2$ là một iđêan của $g$.

Với $i = 1, 2$, ký hiệu $\psi_i$ là đồng cấu của $L(S_i)$ vào $g$ mở rộng $\phi_i$ và $a_i$ là ảnh của nó. Rõ ràng $\phi_i(S_i)$ sinh $a_i$.

Cho $s_1 \in S_1$; ta viết $D = \operatorname{ad} \phi_1(s_1)$. Đạo hàm $D$ của $g$ ánh xạ $\phi_2(S_2)$ vào $a_2$ theo quan hệ

$$
[\phi_1(s_1), \phi_2(s_2)] = \psi_2(d(s_1, s_2)) \quad \text{cho } s_2 \in S_2;
$$

vì đại số con $a_2$ của $g$ được sinh bởi $\phi_2(S_2)$, do đó $D(a_2) \subset a_2$. Tập hợp các $x \in g$ sao cho $\operatorname{ad} x$ giữ $a_2$ bất biến là một đại số Lie con của $g$ chứa $\phi_1(S_1)$ theo điều trên và vì thế cũng chứa $a_1$. Do đó

$$(23)$$
$$[a_1, a_2] \subset a_2.$$

Do đó $a_1 + a_2$ là một đại số Lie con của $g$ và, vì nó chứa tập hợp sinh $\phi_1(S_1) \cup \phi_2(S_2)$,

$$(24)$$
$$a_1 + a_2 = g.$$

Với mọi $s_1 \in S_1$ tồn tại một đạo hàm $D_{s_1}$ của $L(S_2)$ sao cho

$$
D_{s_1}(s_2) = d(s_1, s_2)
$$

với mọi $s_2$ trong $S_2$ (no. 8, Hệ quả của Mệnh đề 8). Ánh xạ $s_1 \mapsto D_{s_1}$ có thể được mở rộng thành một đồng cấu $D$ của $L(S_1)$ vào đại số Lie của các đạo hàm của $L(S_2)$. Gọi $\mathfrak{h}$ là tích nửa trực tiếp của $L(S_1)$ bởi $L(S_2)$ tương ứng với $D$ (Chương I, § 1, no. 8). Với tư cách là một môđun, $\mathfrak{h}$ bằng $L(S_1) \times L(S_2)$ và đặc biệt

$$
[(s_1, 0), (0, s_2)] = (0, d(s_1, s_2))
$$

for $s_1 \in S_1$ và $s_2 \in S_2$.

Từ (25) ta suy ra sự tồn tại của một đồng cấu $f$ của $g$ vào $\mathfrak{h}$ sao cho $f(\phi_1(s_1)) = (s_1, 0)$ và $f(\phi_2(s_2)) = (0, s_2)$ với $s_1 \in S_1$ và $s_2 \in S_2$. Ta suy ra ngay lập tức quan hệ

$$
f(\psi_1(a_1) + \psi_2(a_2)) = (a_1, a_2)
$$

với $a_1 \in L(S_1)$ và $a_2 \in L(S_2)$.

Quan hệ (26) cho thấy rằng $\psi_1$ và $\psi_2$ là đơn ánh và $a_1 \cap a_2 = \{0\}$. Các công thức (23) và (24) khi đó suy ra mệnh đề.

#### Mệnh đề 10 (định lý khử) {#lie-ii-s2-prop-10 .statement}

*Cho X là một tập hợp, S là một tập con của X và T là tập hợp các dãy $(s_1, \ldots, s_n, x)$ với $n \geq 0, s_1, \ldots, s_n$ thuộc S và x thuộc X $- S.$*†

(a) *Môđun $L(X)$ là tổng trực tiếp của đại số con $L(S)$ của $L(X)$ và iđêan $a$ của $L(X)$ sinh bởi $X - S$.*

(b) *Tồn tại một đẳng cấu đại số Lie $\phi$ của $L(T)$ lên $a$ ánh xạ $(s_1, \ldots, s_n, x)$ thành $(\operatorname{ad} s_1 \circ \cdots \circ \operatorname{ad} s_n)(x)$.*

Cho $g$ là đại số Lie được xây dựng như trong Mệnh đề 9 với

$$
S_1 = S, \quad S_2 = T, \quad d(s, t) = (s, s_1, \ldots, s_n, x) \in T \subset L(T)
$$

với $t = (s_1, \ldots, s_n, x)$ thuộc T và $s \in S_1$. Ta đồng nhất $L(S)$ và $L(T)$ với các ảnh chính tắc của chúng trong $g$ (Mệnh đề 9 (a)).

Cho $\psi$ là ánh xạ $(s_1, \ldots, s_n, x) \mapsto (\operatorname{ad} s_1 \circ \cdots \circ \operatorname{ad} s_n)(x)$ của T vào $L(X)$. Hiển nhiên $\psi(d(s, t)) = [s, \psi(t)]$ với $s \in S$ và $t \in T$ và do đó tồn tại một đồng cấu $\alpha : g \to L(X)$ mà hạn chế của nó lên S là đồng nhất và hạn chế của nó lên T là $\psi$. Bây giờ $X - S \subset T$, do đó có một đồng cấu $\beta : L(X) \to g$ mà hạn chế của nó lên $X = S \cup (X - S)$ là đồng nhất.

Ta chứng minh rằng $\alpha$ là một đẳng cấu và $\beta$ là đẳng cấu nghịch đảo. Vì $\psi(x) = x$ với $x$ thuộc $X - S$, ta thấy rằng $\alpha \circ \beta$ trùng với đồng nhất trên X, do đó $\alpha \circ \beta = \mathrm{Id}_{L(X)}$. Mặt khác, $[s, t] = d(s, t)$ trong $g$ với $s \in S, t \in T$ theo phép dựng; suy ra $t = (s_1, \ldots, s_n, x)$ bằng trong $g$ với $(\operatorname{ad} s_1 \circ \cdots \circ \operatorname{ad} s_2)(x)$, do đó $t = \beta(\alpha(t))$. Vì $\beta(\alpha(s)) = s$ với $s \in S$ và $S \cup T$ sinh ra $g$, nên $\beta \circ \alpha = \mathrm{Id}_g$.

Vì $\alpha$ là một đẳng cấu của $g$ lên $L(X)$, Mệnh đề 9 cho thấy rằng phép hạn chế

† Với $n = 0$, ta thu được các phần tử của $X - S$, do đó $X - S \subset T$.

của $\alpha$ lên $L(T)$ là một đẳng cấu $\phi$ của $L(T)$ lên một iđêan $b$ của $L(X)$ sao cho môđun $L(X)$ là tổng trực tiếp của $L(S)$ và $b$. Hiển nhiên
$$
\phi(s_1, \ldots, s_n, x) = (\mathrm{ad}\ s_1 \circ \cdots \circ \mathrm{ad}\ s_n)(x)
$$
với $(s_1, \ldots, s_n, x)$ thuộc $T$.

Do đó $\phi(T) \subset a$, trong khi $b \subset a$ vì $\phi(T)$ sinh ra đại số con $b$ của $L(X)$. Nhưng $b$ là một iđêan và $X - S \subset \phi(T) \subset b$, do đó $a \subset b$.

#### Hệ quả {#lie-ii-s2-n9-cor-1 .statement}

*Cho $y \in X$. Đại số Lie tự do $L(X)$ là tổng trực tiếp của môđun con tự do $K.y$ và đại số con Lie có họ cơ sở là họ của $((\mathrm{ad}\ y)^n, z)$ với $n \geqslant 0$ và $z \in X - \{y\}$.*

Chỉ cần đặt $S = \{y\}$ trong Mệnh đề 10.

### 10. CÁC HỌ HALL TRONG MỘT MAGMA TỰ DO

Cho $X$ là một tập hợp, $M(X)$ là magma tự do được xây dựng trên $X$ và $M^n(X)$, với $n \in \mathbf{N}^*$, là tập hợp các phần tử của $M(X)$ có độ dài $n$ (no. 1). Nếu $w \in M(X)$ và $l(w) \geqslant 2$, ký hiệu $\alpha(w)$ và $\beta(w)$ là các phần tử của $M(X)$ được xác định bởi quan hệ $w = \alpha(w)\beta(w)$; khi đó $l(\alpha(w)) < l(w)$, $l(\beta(w)) < l(w)$. Cuối cùng, với $u, v$ trong $M(X)$, ký hiệu $u^mv$ là phần tử được xác định bằng quy nạp theo số nguyên $m \geqslant 0$ bởi $u^0v = v$ và $u^{m+1}v = u(u^mv)$.

#### Định nghĩa 2 {#lie-ii-s2-def-2 .statement}

*Một tập Hall tương đối với $X$ là bất kỳ tập con được sắp thứ tự toàn phần $H$ của $M(X)$ thỏa mãn các điều kiện sau:*
(A) *Nếu $u \in H, v \in H$ và $l(u) < l(v)$, thì $u < v$.*
(B) *$X \subset H$ và $H \cap M^2(X)$ gồm các tích $xy$ với $x, y$ trong $X$ và $x < y$.*
(C) *Một phần tử $w$ của $M(X)$ có độ dài $\geqslant 3$ thuộc $H$ khi và chỉ khi nó có dạng $a(bc)$ với $a, b, c$ trong $H$, $bc \in H$, $b \leqslant a < bc$ và $b < c$.*

#### Mệnh đề 11 {#lie-ii-s2-prop-11 .statement}

*Có tồn tại một tập Hall tương đối với $X$.*

Ta xây dựng bằng quy nạp theo số nguyên $n$ các tập hợp $H_n \subset M^n(X)$ và một thứ tự toàn phần trên các tập hợp này:
(a) Ta viết $H_1 = X$ và trang bị cho nó một thứ tự toàn phần.
(b) Tập hợp $H_2$ gồm các tích $xy$ với $x, y$ thuộc $X$ và $x < y$. Ta trang bị cho nó một thứ tự toàn phần.
(c) Cho $n \geqslant 3$ là sao cho các tập hợp có thứ tự toàn phần $H_1, \ldots, H_{n-1}$ đã được định nghĩa. Tập hợp $H'_{n-1} = H_1 \cup \cdots \cup H_{n-1}$ có một thứ tự toàn phần cảm sinh các quan hệ đã cho trên $H_1, \ldots, H_{n-1}$ và sao cho $w < w'$ nếu $l(w) < l(w')$. Ta định nghĩa $H_n$ là tập hợp các tích $a(bc) \in M^n(X)$ với $a, b, c$ thuộc $H'_{n-1}$ thỏa mãn các quan hệ $bc \in H'_{n-1}$, $b \leqslant a < bc$, $b < c$ và trang bị cho $H_n$ một thứ tự toàn phần.

Ta viết $H = \bigcup_{n \geqslant 1} H_n$; ta trang bị cho $H$ thứ tự toàn phần được định nghĩa như sau: $w \leqslant w'$ khi và chỉ khi $l(w) < l(w')$ hoặc $l(w) = l(w') = n$ và $w \leqslant w'$ trong tập hợp $H_n$. Ngay lập tức có rằng $H$ là một tập hợp Hall tương đối với $X$.

Với mọi tập con S của X, ta đồng nhất magma tự do M(S) với ảnh chính tắc của nó trong M(X).

#### Mệnh đề 12 {#lie-ii-s2-prop-12 .statement}

Cho H là một tập hợp Hall tương đối với X và cho x, y thuộc X.
(a) $H \cap M(\{x\}) = \{x\}$.
(b) Giả sử rằng $x < y$ và cho $d_y$ là đồng cấu từ $M(X)$ vào $\mathbf{N}$ sao cho $d_y(y) = 1$ và $d_y(z) = 0$ với $z \in X, z \neq y$. Tập hợp các phần tử $w \in H \cap M(\{x, y\})$ sao cho $d_y(w) = 1$ gồm các phần tử $x^n y$ với n là một số nguyên $\geq 0$.

Theo Định nghĩa 2 (B), $x \in H$ và $H \cap M^2(\{x\}) = \varnothing$. Nếu $w \in H \cap M(\{x\})$, trong đó $n = l(w) \geq 3$, các phần tử $\alpha(w)$ và $\beta(w)$ cũng thuộc $H \cap M(\{x\})$ theo Định nghĩa 2 (C). Suy ra ngay lập tức bằng quy nạp theo $n$ rằng $H \cap M^n(\{x\}) = \varnothing$ với $n \geq 2$, do đó có (a).

Bây giờ chứng minh (b). Theo Định nghĩa 2 (B), $y \in H$ và $xy \in H$. Ta chứng minh bằng quy nạp theo $n$ rằng $x^n y \in H$ với $n$ là một số nguyên $\geq 2$. Bây giờ $x^n y = x(x(x^{n-2}y))$ và giả thiết quy nạp suy ra rằng $x^{n-2}y \in H$. Bây giờ $l(x) < l(x^{n-2}y)$ với $n > 2$ và $x < y$, do đó $x < x^{n-2}y$ trong mọi trường hợp; điều kiện (C) của Định nghĩa 2 cho thấy rằng $x^n y \in H$. Mặt khác, hiển nhiên $d_y(x^n y) = 1$. Ngược lại, cho $w \in H \cap M(\{x, y\})$, với $d_y(w) = 1$. Nếu $l(w) = 1$, thì $w = y$; nếu $l(w) = 2$, thì $w = xy$ theo Định nghĩa 2 (B). Nếu $l(w) \geq 3$, thì $w = a(bc)$, với $a, b, c, bc$ thuộc $H \cap M(\{x, y\})$ (Định nghĩa 2 (C)). $d_y(bc) = 0$ là không thể, vì điều này sẽ kéo theo $bc \in M(\{x\})$, điều này là không thể theo (a). Do đó $d_y(bc) = 1$ và $d_y(a) = 0$, do đó $a = x$ theo (a). Suy ra ngay lập tức bằng quy nạp theo $n = l(w)$ rằng $w = x^{n-1}y$, điều này hoàn tất chứng minh (b).

#### Hệ quả {#lie-ii-s2-n10-cor-1 .statement}

Nếu Card X $\geq 2$, thì $H \cap M^n(X) \neq \varnothing$ với mọi số nguyên $n \geq 1$.

#### Mệnh đề 13 {#lie-ii-s2-prop-13 .statement}

Cho X là một tập hợp hữu hạn có ít nhất hai phần tử. Gọi H là một tập Hall tương đối với X. Khi đó tồn tại một song ánh tăng ngặt $p \mapsto w_p$ của $\mathbf{N}$ lên H và một dãy $(P_p)_{p \in \mathbf{N}}$ các tập con của H có các tính chất sau:
(a) $P_0 = X$.
(b) Với mọi số nguyên $p \geq 0$, $w_p \in P_p$.
(c) Với mọi số nguyên $n \geq 1$, tồn tại một số nguyên $p(n)$ sao cho mọi phần tử của $P_p$ đều có độ dài $> n$ với mọi $p \geq p(n)$.
(d) Với mọi số nguyên $p \geq 0$, tập hợp $P_{p+1}$ gồm các phần tử có dạng $w_p^i w$, trong đó $i \geq 0$, $w \in P_p$ và $w \neq w_p$.

Vì X là hữu hạn, mỗi tập hợp $M^n(X)$ là hữu hạn. Đặt $H_n = H \cap M^n(X)$ với mọi $n \geq 1$. Hệ quả của Mệnh đề 12 cho thấy tập hợp hữu hạn $H_n$ là không rỗng. Gọi $u_n$ là lực lượng của $H_n$; đặt $v_0 = 0$ và $v_n = u_1 + \cdots + u_n$ với $n \geq 1$. Vì $H_n$ là một tập hợp hữu hạn được sắp thứ tự toàn phần, tồn tại một song ánh tăng ngặt $p \mapsto w_p$ của khoảng $[v_{n-1}, v_n - 1]$ của $\mathbf{N}$ lên $H_n$. Ngay lập tức thấy rằng $p \mapsto w_p$ là một song ánh tăng ngặt của $\mathbf{N}$ lên H.

Đặt $P_0 = X$ và với mỗi số nguyên $p \geq 1$ gọi $P_p$ là tập hợp các phần tử $w$ của H sao cho $w \geq w_p$, và hoặc $w \in X$, hoặc $\alpha(w) < w_p$ (chú ý rằng nếu $w$ có độ dài $\geq 2$ thì quan hệ $w \in H$ kéo theo $\alpha(w) \in H$ theo điều kiện (C) của Định nghĩa 2). Khi đó $w_p \in P_p$; điều này là hiển nhiên nếu $w_p \in X$ và suy ra từ bất đẳng thức $l(\alpha(w_p)) < l(w_p)$ và điều kiện (A) của Định nghĩa 2 khi $w_p \notin X$.

Do đó các điều kiện (a) và (b) được thỏa mãn.

Cho $n$ là một số nguyên $\geq 1$ và cho $p \geq v_n$. Với mọi $w \in P_p, l(w) \geq l(w_p) > n$ theo đúng định nghĩa của ánh xạ $p \mapsto w_p$. Điều này chứng minh (c).

Bây giờ ta chứng minh rằng mọi phần tử có dạng $u = w_p^i w$ với $i \geq 0, w \in P_p$ và $w \neq w_p$ đều thuộc $P_{p+1}$. Nếu $i \neq 0$, thì $l(u) > l(w_p)$, do đó $u > w_p$ và $u \geq w_{p+1}$; khi đó $u \notin X$ và $\alpha(u) = w_p < w_{p+1}$, do đó $u \in P_{p+1}$. Nếu $i = 0$, thì $u \in P_p$ và $u \neq w_p$; khi đó $u > w_p$, do đó $u \geq w_{p+1}$; nếu $u$ không thuộc $X$, thì $\alpha(w) < w_p$, do đó $\alpha(w) < w_{p+1}$; khi đó một lần nữa $u \in P_{p+1}$.

Ngược lại, cho $u \in P_{p+1}$. Ta phân biệt hai trường hợp:

(α) Không tồn tại phần tử $v$ của $M(X)$ sao cho $u = w_p v$. Theo định nghĩa của $P_{p+1}$, $u > w_p$. Hơn nữa, nếu $u \notin X$, thì $\alpha(u) \neq w_p$ theo giả thiết đã cho và $\alpha(u) < w_{p+1}$ vì $u \in P_{p+1}$; do đó $\alpha(u) < w_p$. Vậy $u \in P_p$ và $u \neq w_p$.

(β) Tồn tại $v$ trong $M(X)$ sao cho $u = w_p v$. Theo Định nghĩa 2, tất yếu, hoặc là $w_p \in X, v \in X$ và $w_p < v$, hoặc là $v \notin X$ và $\alpha(v) \leq w_p < v$. Trong cả hai trường hợp, $v \in P_{p+1}$.

Khi đó tồn tại một số nguyên $i \geq 0$ và một phần tử $w$ của $M(X)$ sao cho $u = w_p^i w$, và hoặc là $w \in X$ hoặc là $w \notin X$ và $\alpha(w) \neq w_p$. Nếu $i = 0$, ta có trường hợp (α) ở trên, do đó $w \in P_p$ và $w \neq w_p$. Nếu $i > 0$, chứng minh của (β) ở trên thiết lập, bằng quy nạp theo $i$, các hệ thức $w \in P_{p+1}$ và $w \neq w_p$. Giả sử $w \notin X$; từ $w \in P_{p+1}$ suy ra $\alpha(w) \leq w_p$ và vì $\alpha(w) \neq w_p$, ta kết luận rằng $w \in P_p$. Điều này hoàn thành chứng minh của (d).

#### Ví dụ {#lie-ii-s2-n10-exa-1 .statement}

Giả sử rằng $X$ có hai phần tử $x, y$; hãy cho $X$ có thứ tự sao cho $x < y$. Phép dựng được cho trong chứng minh của Mệnh đề 11 cho một tập hợp $H$ có 14 phần tử có độ dài $\leq 5$ được cho trong bảng sau:

$$
\begin{array}{ll}
H_1 & w_1 = x \\
H_2 & w_3 = (xy) \\
H_3 & w_4 = (x(xy)) & w_5 = (y(xy)) \\
H_4 & w_6 = (x(x(xy)))) & w_7 = (y(x(xy)))) & w_8 = (y(y(xy)))) \\
H_5 & w_9 = (x(x(x(xy)))) & w_{10} = (y(x(x(xy)))) & w_{11} = (y(y(x(xy))))) \\
& w_{12} = (y(y(y(xy)))) & w_{13} = ((xy)(x(xy))) & w_{14} = ((xy)(y(xy))).
\end{array}
$$

(Các phần tử của $H$ đã được đánh số theo thứ tự toàn phần được chọn trên mỗi $H_n$.)

### 11. CÁC CƠ SỞ HALL CỦA MỘT ĐẠI SỐ LIE TỰ DO

Ta giữ lại ký hiệu của số trước.

#### Định lý 1 {#lie-ii-s2-thm-1 .statement}

Cho $H$ là một tập hợp Hall đối với $X$ và $\Psi$ là ánh xạ chính tắc của $M(X)$ vào đại số Lie tự do $L(X)$. Hạn chế của $\Psi$ trên $H$ là một cơ sở của môđun $L(X)$.

Với mọi phần tử $w$ của $H$ ta viết $\bar{w} = \Psi(w)$.

(A) *Trường hợp $X$ là hữu hạn.*

Nếu $X$ là rỗng thì $M(X)$ cũng rỗng và do đó $H$ và $L(X)$ là không. Nếu $X$ có một phần tử duy nhất $x$, $H \cap M^n(X)$ là rỗng với $n \geq 2$ (Mệnh đề 12 (a)). Do đó, $H = \{x\}$; ta cũng biết (no. 2, *Nhận xét*) rằng môđun $L(X)$ là tự do và có cơ sở $\{\bar{x}\}$. Vì vậy định lý đúng khi $X$ có nhiều nhất một phần tử.

Từ đây giả sử rằng $X$ có ít nhất hai phần tử; chọn các dãy $(w_p)$ và $(P_p)$ với các tính chất đã nêu trong Mệnh đề 13. Với mỗi số nguyên $p \geq 0$, ký hiệu $L_p$ là môđun con của $L(X)$ được sinh bởi các phần tử $\bar{w}_i$ với $0 \leq i < p$ và $g_p$ là đại số Lie con của $L(X)$ được sinh bởi họ $(\bar{u})_{u \in P_p}$.

#### Bổ đề 2 {#lie-ii-s2-lem-2 .statement}

*Với mỗi số nguyên $p \geq 0$, môđun $L_p$ nhận họ $(\bar{w}_i)_{0 \leq i < p}$ làm cơ sở, đại số Lie $g_p$ nhận $(\bar{u})_{u \in P_p}$ làm họ cơ sở và môđun $L(X)$ là tổng trực tiếp của $L_p$ và $g_p$.*

$L_0 = \{0\}$ và $g_0 = L(X)$ và bổ đề đúng với $p = 0$. Ta lập luận bằng quy nạp theo $p$. Giả sử khi đó bổ đề đúng với một số nguyên $p \geq 0$. Đặt $u_i, w = (\mathrm{ad}\ \bar{w}_p)^i.\bar{w} = \Psi(w_p^i w)$ với $i \geq 0, w \in P_p, w \neq w_p$. Theo Hệ quả của Mệnh đề 10 của no. 9, đại số Lie tự do $g_p$ là tổng trực tiếp của môđun $T_p$ có cơ sở $\{\bar{w}_p\}$ và một đại số Lie con $h_p$ nhận

$$
\mathcal{F} = (u_i, w)_{i \geq 0,\ w \in P_p,\ w \neq w_p}
$$

làm họ cơ sở. Theo Mệnh đề 13 (d), họ $(\bar{u})_{u \in P_{p+1}}$ bằng $\mathcal{F}$ và do đó là một họ cơ sở của $h_p = g_{p+1}$. Vì thế $L(X) = L_p \oplus T_p \oplus g_{p+1}$ và, do $L_{p+1} = L_p + T_p$, $L(X) = L_{p+1} \oplus g_{p+1}$ và $(\bar{w}_0, \bar{w}_1, \ldots, \bar{w}_{p-1}, \bar{w}_p)$ là một cơ sở của môđun $L_{p+1}$.

Cho $n$ là một số nguyên dương. Theo Mệnh đề 13 (c), tồn tại một số nguyên $p(n)$ sao cho $P_p$ chỉ có các phần tử có độ dài $> n$ đối với $p \geq p(n)$. Với $p \geq p(n)$, đại số con Lie $g_p$ của $L(X)$ được sinh bởi các phần tử có bậc $> n$ và do đó $L^n(X) \cap g_p = \{0\}$. Mặt khác, các phần tử $\bar{w}_i$ của $L(X)$ là thuần nhất và họ $(w_i)_{0 \leq i < p}$ là một cơ sở của một môđun bù của $g_p$. Suy ra ngay lập tức rằng họ các phần tử $\bar{w}_i$ có bậc $n$ là một cơ sở của môđun $L^n(X)$ và rằng dãy $(\bar{w}_i)_{i \geq 0}$ là một cơ sở của môđun $L(X)$.

(B) *Trường hợp tổng quát.*

Nếu $S$ là một tập con của $X$, nhắc lại rằng $M(S)$ được đồng nhất với magma con của $M(X)$ được sinh bởi $S$ và $L(S)$ được đồng nhất với đại số con Lie của $L(X)$ được sinh bởi $S$; ta đã thấy rằng nếu $w \in M(S)$ có độ dài $\geq 2$ thì $\alpha(w) \in M(S)$ và $\beta(w) \in M(S)$. Suy ra ngay lập tức rằng $H \cap M(S)$ là một tập Hall đối với $S$.

Với mọi tập con hữu hạn $\Phi$ của $H$ tồn tại một tập con hữu hạn $S$ của $X$ sao cho

Φ ⊂ M(S). Trường hợp (A) cho thấy rằng các phần tử $\bar{w}$ với $w \in \Phi$ là độc lập tuyến tính trong $L(S)$ và do đó trong $L(X)$. Vì vậy họ $(\bar{w})_{w \in H}$ là tự do.

Với mọi phần tử $a$ của $L(X)$ tồn tại một tập con hữu hạn $S$ của $X$ sao cho $a \in L(S)$. Theo trường hợp (A), tập con $\Psi'(H \cap M(S))$ của $\Psi'(H)$ sinh môđun $L(S)$ và do đó $a$ là một tổ hợp tuyến tính của các phần tử của $\Psi'(H)$. Vì vậy $\Psi'(H)$ sinh môđun $L(X)$, điều này hoàn thành chứng minh.

#### Hệ quả {#lie-ii-s2-n11-cor-1 .statement}

*Môđun* $L(X)$ *là tự do và mỗi môđun con* $L^\alpha(X)$ *với* $\alpha \in \mathbf{N}^{(X)}$ *và* $L^n(X)$ *với* $n \in \mathbf{N}$ *cũng vậy*. *Các môđun* $L^\alpha(X)$ *có hạng hữu hạn và các môđun* $L^n(X)$ *cũng có hạng hữu hạn nếu* $X$ *là hữu hạn*.

Tồn tại một tập Hall $H$ đối với $X$ (Mệnh đề 11). Với mọi $w \in H$, phần tử $\Psi'(w)$ của $L(X)$ thuộc một trong các môđun $L^\alpha(X)$ (với $\alpha \in \mathbf{N}^{(X)}$) và môđun $L(X)$ là tổng trực tiếp của các môđun con $L^\alpha(X)$. Hơn nữa, với mọi $\alpha \in \mathbf{N}^{(X)}$, tập hợp các phần tử của $M(X)$ mà ảnh chính tắc của chúng trong $\mathbf{N}^{(X)}$ bằng $\alpha$ là hữu hạn; điều này cho thấy mỗi môđun $L^\alpha(X)$ là tự do và có hạng hữu hạn, và $L(X)$ là tự do. Bây giờ $L^n(X) = \sum_{|\alpha|=n} L^\alpha(X)$ và do đó $L^n(X)$ là tự do; khi $X$ là hữu hạn, tập hợp các $\alpha \in \mathbf{N}^{(X)}$ sao cho $|\alpha|=n$ là hữu hạn và do đó khi ấy $L^n(X)$ có hạng hữu hạn.

#### Định nghĩa 3 {#lie-ii-s2-def-3 .statement}

*Một cơ sở Hall của một đại số Lie tự do* $L(X)$ *là bất kỳ cơ sở nào của* $L(X)$ *là ảnh chính tắc của một tập Hall đối với* $X$.

#### Nhận xét {#lie-ii-s2-n11-rem-1 .statement}

Giả sử $X$ gồm hai phần tử phân biệt $x$ và $y$ và gọi $L^{(\cdot,1)}$ là môđun con của $L(X)$ là tổng của các $L^\alpha(X)$ trong đó $\alpha \in \mathbf{N}^X$ và $\alpha(y)=1$. Suy ra ngay lập tức từ Định lý 1 và Mệnh đề 12 của no. 10 rằng các phần tử $(\mathrm{ad}\,x)^n.y$ trong đó $n$ là một số nguyên $\geqslant 0$ tạo thành một *cơ sở* của môđun con $L^{(\cdot,1)}$. Suy ra rằng *hạn chế của ánh xạ ad* $x$ *trên* $L^{(\cdot,1)}$ *là đơn ánh*.

### Bài tập {#lie-ii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
