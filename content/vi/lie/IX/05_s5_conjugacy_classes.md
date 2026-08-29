---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 5
section_title: Conjugacy classes
lang: vi
source: lie-vii-ix
book_pages: 324-333, 405-409
pdf_pages: 0331-0340, 0412-0416
extraction: native
subsections:
    - "no": 1
      title: REGULAR ELEMENTS
      page: 324
      pdf_page: 331
    - "no": 2
      title: CHAMBERS AND ALCOVES
      page: 325
      pdf_page: 332
    - "no": 3
      title: AUTOMORPHISMS AND REGULAR ELEMENTS
      page: 327
      pdf_page: 334
    - "no": 4
      title: THE MAPS (G$\boldsymbol{/}$T) $\times \mathbf{T}\rightarrow$ G AND (G$\boldsymbol{/}$T) $\times \mathbf{A}\rightarrow \mathbf{G}_{\boldsymbol{r}}$
      page: 331
      pdf_page: 338
statements: 26
exercises: 12
content_sha256: c7b456f1bdc883a294652b92b5aac36bdf6cbf26d9e5edae61ca81ad69d3af5e
translated_from: content/en/lie/IX/05_s5_conjugacy_classes.md
source_content_sha256: 67b7c3bf0335e1b8bfbe872472e7bd56c7dbf0d52741cf029286e2edabbf3e06
translation_model: gpt-5.4-mini, gpt-5-mini
translation_run: translate-vi-21aa148a
glossary_version: 34
glossary_terms_sha256: d02d145ec8f8c723e93d877e1595b1a82c76d8d538be089a02bbdc06ded6664b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC LỚP LIÊN HỢP

Ta giữ các ký hiệu của §4.

### 1. CÁC PHẦN TỬ CHÍNH QUY

Theo Hệ quả 4 của Định lý 2 của §2, no. 2, các phần tử chính quy $g$ của G có thể được đặc trưng bởi một trong hai tính chất sau:

a) Đại số con của $\mathfrak{g}$ được Ad $g$ cố định là một đại số con Cartan.

$b) Z(g)_0$ là một xuyến cực đại của G.

Tập hợp các phần tử chính quy của G là mở và trù mật trong G.

Trong phần còn lại của đoạn này, ta ký hiệu $G_r$ (resp. $T_r$) là tập các điểm của G (resp. T) chính quy trong G. Một phần tử $g$ của G thuộc $T_r$ khi và chỉ khi $Z(g)_0$ bằng T; mọi phần tử của $G_r$ đều liên hợp với một phần tử của $T_r($§2, no. 2, Th. 2).

Một phần tử $t$ của T thuộc $T_r$ khi và chỉ khi $t^{\alpha}\not= 1$ với mọi nghiệm $\alpha \in R(G,T)$; do đó, T **--** $T_r$ là hợp của các xuyến con Ker $\alpha$ với $\alpha$ trong $R(G,T)$.

#### Mệnh đề 1 {#lie-ix-s5-prop-1 .statement tag=01DV}

Đặt $n=$ dim G. Tồn tại một đa tạp giải tích thực compact V có chiều $n-3$ và một ánh xạ giải tích $\varphi : V\rightarrow G$ có ảnh là G **--** $G_r$.

Cho $\alpha \in R(G,T)$; đặt $V_{\alpha}= (G/$Z(Ker$\alpha$ ))$\times$ (Ker$\alpha$ ), và cho $\varphi_{\alpha}$ là cấu xạ từ $V_{\alpha}$ đến G sao cho, với mọi $g\in G$ và mọi $t\in$ Ker $\alpha$, ta có $\varphi_{\alpha}(\overline{g}, t) =gtg^{-1}$ (ta ký hiệu $\overline{g}$ là lớp ghép của $g$ theo modulo Z(Ker$\alpha$ )). Khi đó $V_{\alpha}$ là một đa tạp giải tích thực compact có chiều

dim $V_{\alpha}=$ dim $G-$ dim Z(Ker $\alpha$ ) $+$ dim Ker$\alpha$

$=n-$ (dim T + 2) + (dim $T-1$) $=n-3$

(§4, no. 5, Th. $1$)$;\varphi_{\alpha}$ là một cấu xạ của các đa tạp giải tích thực, và ảnh của $\varphi_{\alpha}$ gồm các phần tử của G liên hợp với một phần tử của Ker $\alpha$. Bây giờ chỉ cần lấy V là tổng của các đa tạp $V_{\alpha}$, và $\varphi$ là cấu xạ cảm sinh $\varphi_{\alpha}$ trên mỗi $V_{\alpha}$.

#### Nhận xét {#lie-ix-s5-n1-rem-1 .statement tag=01DW}

Một phần tử $g$ của G được gọi là rất chính quy nếu $Z(g)$ là một xuyến cực đại của G. Nếu $g\in T,g$ rất chính quy khi và chỉ khi $w(g)\not=g$ với mọi phần tử khác phần tử đơn vị $w$ của $W_G(T)$ (§4, no. 7, Mệnh đề 14). Do đó, tập hợp các phần tử rất chính quy là một tập con trù mật mở của G (§2, no. 5, Hệ quả 2 của Mệnh đề 5).

### 2. CÁC BUỒNG VÀ CÁC Ô

Kí hiệu $\mathfrak{t}_r$ là tập hợp các phần tử $x\in \mathfrak{t}$ sao cho exp $x$ là chính quy, nói cách khác thuộc $T_r$. Một phần tử $x$ của $\mathfrak{t}$ thuộc $\mathfrak{t}$ **--** $\mathfrak{t}_r$ khi và chỉ khi tồn tại một nghiệm $\alpha \in R(G,T)$ sao cho $\delta (\alpha )(x)\in 2\pi i\mathbf{Z}$. Với mỗi nghiệm $\alpha \in R(G,T)$ và mỗi số nguyên $n$, kí hiệu $H_{\alpha ,n}$ là tập hợp các $x\in \mathfrak{t}$ sao cho $\delta (\alpha )(x) = 2\pi in$. Các $H_{\alpha ,n}$ được gọi là các siêu phẳng kỳ dị của $\mathfrak{t}$, và $\mathfrak{t}$ **--** $\mathfrak{t}_r$ là hợp của các siêu phẳng kỳ dị. Các alcove của $\mathfrak{t}$ là các thành phần liên thông của $\mathfrak{t}_r$, và các buồng là các thành phần liên thông của phần bù trong $\mathfrak{t}$ của hợp các siêu phẳng kỳ dị đi qua gốc tọa độ (tức là, các $H_{\alpha ,0}=$ Ker$\delta (\alpha ),\alpha \in R(G,T)$).

Ta có $\Gamma (T)\subset \mathfrak{t}$**--** $\mathfrak{t}_r$; kí hiệu $N(G,T)$ là nhóm con của $\Gamma (T)$ được sinh bởi các vectơ nút (§4, no. 5); theo Mệnh đề 11 của §4, no. 6, thương $\Gamma (T)/N(G,T)$ có thể được đồng nhất với nhóm cơ bản của G.

Cuối cùng, kí hiệu W là nhóm Weyl của G đối với T, xét như một nhóm các tự đẳng cấu của T và của $\mathfrak{t}$, và kí hiệu $W_a$ (tương ứng $W'_a$) là nhóm các tự đẳng cấu của không gian afin $\mathfrak{t}$ được sinh bởi W và các phép tịnh tiến $t_{\gamma}:x \rightarrow x+\gamma$ với $\gamma \in N(G,T)$ (tương ứng với $\gamma \in \Gamma (T)$).

Cho $w\in W,\gamma \in \Gamma$ (T), $\alpha \in R(G,T)$ và $n\in \mathbf{Z}$. Ta có:

$$
w(H_{\alpha ,n}) = H_{w\alpha ,n},t_{\gamma}(H_{\alpha ,n}) = H_{\alpha ,n+\langle\gamma ,\alpha\rangle}
$$

Suy ra rằng, với mọi buồng C và mọi $w\in W,w(C)$ là một buồng và rằng với mọi alcove A và mọi $w\in W'_a,w(A)$ là một alcove. Chú ý rằng, khi $X(T)\otimes \mathbf{R}$ được đồng nhất với $\mathfrak{t}^*$ qua đẳng cấu $(2\pi i)^{-1}\delta$, thì các alcove của $\mathfrak{t}$ và nhóm $W_a$ là các alcove và nhóm Weyl afin liên kết với hệ nghiệm $R(G,T)$ (Ch. VI, §2, no. 1).

#### Mệnh đề 2 {#lie-ix-s5-prop-2 .statement tag=01DX}

a) Nhóm $W_a$ (tương ứng $W'_a$) là tích nửa trực tiếp của W bởi $N(G,T)$ (tương ứng $\Gamma (T)$); nhóm con $W_a$ của $W'_a$ là chuẩn tắc.

b) Nhóm W (tương ứng $W_a$) tác động đơn bắc cầu lên tập hợp các buồng (tương ứng các ô).

c) Cho C là một buồng và A là một ô. Khi đó $\overline{C}$ (tương ứng A, tương ứng A) là một miền cơ bản cho tác động của W lên $\mathfrak{t}$ (tương ứng của $W_a$ lên $\mathfrak{t}$, tương ứng của $W_a$ lên $\mathfrak{t}$**--** $\mathfrak{t}_r$). Nếu $x\in \mathfrak{t}_r$ và $w\in W_a$ sao cho $w(x) =x$, thì $w=$ Id.

d) Với mỗi buồng C, tồn tại duy nhất một ô A sao cho $A\subset C$ và$\gamma \in \frac{0}{A}.\in \overline{A}$. Với mỗi ô A, tồn tại duy nhất $\gamma \in N(G,T)$ sao cho

Nếu $w\in W$ và $\gamma \in \Gamma$(T), thì $wt_{\gamma}w^{-1}=t_{w(\gamma)}$ và $wt_{\gamma}w^{-1}t^{-1}_{\gamma}=t_{w(\gamma)-\gamma}$, với $w(\gamma )-\gamma \in N(G,T)$; điều này ngay lập tức suy ra a). Phần còn lại của mệnh đề suy ra từ Chương VI, §1, no. 5 và §2, các số 1 và 2.

#### Hệ quả 1 {#lie-ix-s5-prop-2-cor-1 .statement tag=01DY}

Cho A là một ô của $\mathfrak{t},\overline{A}$ phần bao đóng của nó, và $H_A$ là nhóm ổn định của A trong $W'_a$.

a) Nhóm $W'_a$ là tích bán trực tiếp của $H_A$ bởi $W_a$.

b) Ánh xạ mũ $\overline{A}\rightarrow T$ và đơn ánh chính tắc $T\rightarrow G$ cảm sinh, khi qua các thương và các tập con, các đồng phôi

$\overline{A}/H_A\rightarrow T/W\rightarrow G/$Int(G)

$A/H_A\rightarrow T_r/W\rightarrow G_r/$Int(G).

Cho $w'\in W'_a$; khi đó $w'(A)$ là một ô của $\mathfrak{t}$, và tồn tại (Mệnh đề $2b$)$)$ một phần tử duy nhất $w$ của $W_a$ sao cho $w(A) =w'$(A), tức là $w^{-1}w'\in H_A$. Vì $W_a$ là chuẩn tắc trong $W'_a$, nên điều này chứng minh a).

Đơn ánh chính tắc của $\overline{A}$ vào $\mathfrak{t}$ cảm sinh một song ánh liên tục $\theta :\overline{A}\rightarrow$ $\mathfrak{t}/W_a$ (Mệnh đề $2c$)$)$, và đây là một đồng phôi vì A là compact. Vì $W_a$ là nhóm con chuẩn trong $W'_a$, nhóm $H_A$ tác động một cách chính tắc trên $\mathfrak{t}/W_a($Đại số, Chương I, §5, no. 4) và $\mathfrak{t}/W'_a$ có thể được đồng nhất với thương $(\mathfrak{t}/W_a)/H_A$; ánh xạ $\theta$ tương thích với các tác động của $H_A$, nên cảm sinh, qua thương, một đồng phôi $A/H_A\rightarrow \mathfrak{t}/W'_a$. Hơn nữa, exp$_{\Gamma}$ cảm sinh một đồng phôi từ $\mathfrak{t}/\Gamma (T)$ đến T, nên cũng cảm sinh một đồng phôi từ $\mathfrak{t}/W'_a$ đến $T/W$. Khẳng định b) suy ra từ đó và Hệ quả 1 của Mệnh đề 5 của §2, no. 4.

#### Nhận xét 1 {#lie-ix-s5-n2-rem-1 .statement tag=01DZ}

Nhóm $H_A$ có thể được đồng nhất một cách tự nhiên với $\Gamma (T)/N(G,T)$, nên cũng với $\pi_1(G)$. Vì vậy, nó thu về phần tử đơn vị khi G là liên thông đơn.

#### Nhận xét 2 {#lie-ix-s5-n2-rem-2 .statement tag=01E0}

Cho $x\in A$; khi đó exp $x\in T_r$, nên Z(exp $x$)$_0= T$. Hơn nữa, exp $x$ rất chính quy (no. 1, Nhận xét) khi và chỉ khi $w(x)\not=x$ với mọi $w\in W'_a$ khác với phần tử đơn vị. Theo Hệ quả 1, điều này cũng có nghĩa là $h(x)\not=x$ với mọi $h\in H_A$ khác với phần tử đơn vị. Đặc biệt, nếu G là liên thông đơn, thì $Z_G(t) = T$ với mọi $t\in T_r$, và mọi phần tử chính quy của G đều rất chính quy.

#### Nhận xét 3 {#lie-ix-s5-n2-rem-3 .statement tag=01E1}

Các điểm đặc biệt của $W_a$ (Chương VI, §2, no. 2) là các phần tử $x$ của $\mathfrak{t}$ sao cho $\delta (\alpha )(x)\in 2\pi i\mathbf{Z}$ với mọi $\alpha \in R(G,T)$ (loc. cit., Mệnh đề 3), tức là sao cho exp $x\in C(G)$ (§4, no. 4, Mệnh đề 8). Với phần tử $x$ như thế ta có $wx-x\in N(G,T)$ với mọi $w\in W$ (Chương VI, §1, no. 9, Mệnh đề 27), nên các nhóm ổn định của $x$ trong $W_a$ và $W'_a$ trùng nhau. Cho S là tập hợp các điểm đặc biệt của A; từ điều trên và Hệ quả 1 suy ra rằng nhóm $H_A$ tác động tự do trên S, và ánh xạ mũ cảm sinh một song ánh từ $S/H_A$ đến C(G).

#### Hệ quả 2 {#lie-ix-s5-prop-2-cor-2 .statement tag=01E2}

Cho C là một buồng của $\mathfrak{t}$ và $\overline{C}$ là bao đóng của nó. Các đơn ánh chính tắc $\overline{C}\rightarrow \mathfrak{t}\rightarrow \mathfrak{g}$ cảm sinh, qua thương, các đồng phôi

$\overline{C}\rightarrow \mathfrak{t}/W\rightarrow \mathfrak{g}/$Ad(G).

Các ánh xạ chính tắc $\overline{C}\rightarrow \mathfrak{t}$ và $\mathfrak{t}\rightarrow \mathfrak{t}/W$ là proper (Tôpô tổng quát, Chương III, §4, no. 1, Mệnh đề $2c$)$)$. Ánh xạ $\overline{C}\rightarrow \mathfrak{t}/W$ liên tục, proper và song ánh (Mệnh đề $2c$)$)$; do đó, nó là một đồng phôi, suy ra hệ quả theo Hệ quả của Mệnh đề 6 của §2, no. 5.

#### Nhận xét 4 {#lie-ix-s5-n2-rem-4 .statement tag=01E3}

Ký hiệu $\mathfrak{g}_{reg}$ là tập hợp các phần tử chính quy của $\mathfrak{g}$ (Chương VII, §2, no. 2, Định nghĩa 2) và đặt $\mathfrak{t}_{reg}=\mathfrak{t}\cap \mathfrak{g}_{reg}$. Với $x\in \mathfrak{t}$, ta có

det(X $-$ ad$_{\mathfrak{g}}x$) $= X^{dim}\prod_{\alpha\in R(G,T)}^{\mathfrak{t}}(X-\delta (\alpha )(x))$,

và do đó $\mathfrak{t}_{reg}$ là tập hợp các phần tử $x$ của $\mathfrak{t}$ sao cho $\delta (\alpha )(x)\not= 0$ với mọi $\alpha \in R(G,T)$, nghĩa là hợp của các buồng của $\mathfrak{t}$ (vì vậy $\mathfrak{t}_r\subset \mathfrak{t}_{reg}$). Do đó $C\cap \mathfrak{t}_{reg}= C$, nên ta có các phép đồng phôi

$C\rightarrow \mathfrak{t}_{reg}/W\rightarrow \mathfrak{g}_{reg}/$Ad(G).

#### Hệ quả 3 {#lie-ix-s5-prop-2-cor-3 .statement tag=01E4}

Giả sử rằng G đơn liên; cho $g$ là một phần tử chính quy của G. Tồn tại một xuyến cực đại S của G, và một miền cơ bản A của L(S), cả hai được xác định duy nhất, sao cho $g\in$ exp(A) và $0\in \overline{A}$.

Ta có thể giả sử rằng $g$ thuộc $T_r($§2, no. 2, Định lý 2). Gọi $x$ là một phần tử của $\mathfrak{t}_r$ sao cho exp $x=g$, và gọi $A'$ là miền cơ bản của $\mathfrak{t}$ chứa $x$. Các miền cơ bản A của $\mathfrak{t}$ sao cho $g\in$ exp(A) là các miền cơ bản $A'-\gamma$ với $\gamma \in \Gamma (T)$; do đó, mệnh đề suy ra từ Mệnh đề $2d)$.

### 3. TỰ ĐẲNG CẤU VÀ CÁC PHẦN TỬ CHÍNH QUY

#### Bổ đề 1 {#lie-ix-s5-lem-1 .statement tag=01E5}

Cho $u$ là một tự đẳng cấu của G, và H là tập hợp các điểm bất động của nó.

a) H là một nhóm con đóng của G.

b) Nếu $H_0$ là trung tâm trong G, thì G là giao hoán (vì vậy G = T).

Khẳng định a) là rõ ràng. Để chứng minh b), ta có thể thay thế G bởi D(G) (§1, Hệ quả 1 của Mệnh đề 4), và do đó có thể giả sử rằng G là nửa đơn. Khi đó, nếu $H_0$ là trung tâm trong G, ta có $L(H) =\{0\}$, nên tự đồng cấu $L(u)-$Id của $\mathfrak{g}$ là song ánh. Gọi $f$ là ánh xạ của đa tạp G được xác định bởi $f(g) =u(g)^{-1}g$ với $g\in G$; nó là étale, vì nếu $g\in G$ và $x\in \mathfrak{g}$, ta có $T(f)(xg) =u(g)^{-1}(x-L(u)(x))g$, do đó ánh xạ tiếp xúc của $f$ tại $g$ là song ánh. Suy ra ảnh của $f$ là mở và compact, vì vậy trùng với G vì G liên thông. Bây giờ cho E là một khung của G (§4, no. 10, Định nghĩa 3) và $u(E)$ là ảnh của nó qua $u$. Theo Mệnh đề 19 của tài liệu đã dẫn, tồn tại một phần tử $h$ của G sao cho (Int $h$)$(E) =u(E)$. Gọi $g\in G$ là phần tử sao cho $h=f(g) =u(g)^{-1}g$; khi đó

$u\circ$ Int $g=$ (Int $u(g)$)$\circ u=$ Int $g\circ$ (Int $h$)$^{-1}\circ u$,

nên khung (Int $g$)$(E)$ ổn định dưới $u$. Nếu (Int $g$)$(E) = (T_1,B,(U_{\alpha})_{\alpha\in B})$, thì $\sum U_{\alpha}\in L(H)$; vì $L(H) =\{0\}$, điều này suy ra rằng $B =\emptyset$, do đó $G = T_1$, và G giao hoán.

#### Bổ đề 2 {#lie-ix-s5-lem-2 .statement tag=01E6}

Cho $x$ là một phần tử của T và S là một xuyến con của T. Nếu thành phần liên thông chứa đơn vị của $Z(x)\cap Z(S)$ bằng T, thì tồn tại một phần tử $s$ của S sao cho $xs$ là chính quy.

Với mọi $\alpha \in R(G,T)$, cho $S_{\alpha}$ là đa tạp con của S gồm các phần tử $s$ của S sao cho $(xs)^{\alpha}= 1$. Nếu không có phần tử $s$ nào của S sao cho $xs$ là chính quy, thì S là hợp các đa tạp con $S_{\alpha}$, do đó bằng một trong số đó. Vậy tồn tại $\alpha$ trong $R(G,T)$ sao cho $(xs)^{\alpha}= 1$ với mọi $s\in S$; nhưng điều này suy ra rằng $x^{\alpha}= 1$ và $\alpha |S = 1$, nên $Z(x)\cap Z(S)\supset$ Z(Ker $\alpha$ ), suy ra bổ đề.

#### Bổ đề 3 {#lie-ix-s5-lem-3 .statement tag=01E7}

Giả sử G là đơn liên. Cho C là một buồng của $\mathfrak{t}$, và $u$ là một tự đẳng cấu của G sao cho T và C ổn định dưới $u$. Khi đó tập các điểm của T cố định bởi $u$ là liên thông.

Vì G là đơn liên, $\Gamma (T)$ được sinh bởi các vectơ nút $K_{\alpha}$ $(\alpha \in R(G,T))$, và do đó có một cơ sở gồm họ các $K_{\alpha}$ sao cho $\alpha$ thuộc cơ sở B(C) được xác định bởi C (Chương VI, §1, no. 10). Vì vậy, chỉ cần chứng minh rằng, nếu $\varphi$ là một tự đẳng cấu của xuyến T giữ ổn định một cơ sở của $\Gamma$(T), thì tập các điểm cố định của $\varphi$ là liên thông. Phân tích cơ sở này thành hợp rời nhau các quỹ đạo của nhóm sinh bởi $\varphi$, ta quy về trường hợp $T =\mathbf{U}^n$ và $\varphi$ là tự đẳng cấu $(z_1, . . . , z_n) \rightarrow (z_2, . . . , z_n, z_1)$; trong trường hợp này các điểm cố định của $\varphi$ là các điểm $(z, z, . . . , z)$ với $z\in \mathbf{U}$, và chúng tạo thành một nhóm con liên thông của T.

#### Mệnh đề 3 {#lie-ix-s5-prop-3 .statement tag=01E8}

Cho $u$ là một tự đẳng cấu của G, và cho $x$ là một điểm của G cố định bởi $u$.

a) Tồn tại một phần tử $a$ của $\mathfrak{g}$, được $L(u)$ và Ad $x$ cố định, sao cho $x$ exp $a$ là chính quy.

b) Tồn tại một phần tử chính quy $g$ của G được $u$ cố định và giao hoán với $x$.

Cho H là nhóm các điểm bất động của u, S là một xuyến cực đại của $Z(x)\cap H$, và K là thành phần liên thông đơn vị của $Z(S)\cap Z(x)$. Đó là một nhóm con đóng liên thông của G; hơn nữa, theo Hệ quả 5 của Định lý 2 của §2, no. 2, tồn tại các xuyến cực đại của G chứa S và x, do đó K có hạng cực đại và chứa S và x. Mặt khác, K ổn định dưới u vì S và x đều vậy; ký hiệu V là tập các điểm bất động của u trong K. Khi đó

$$
S\subset V_0\subset K\cap H\subset Z(S)\cap Z(x)\cap H
$$

suy ra $V_0$ được chứa trong bộ trung tâm hóa của S trong $(Z(x)\cap H)_0$; nhưng bộ sau trùng với S (loc. cit., Hệ quả 6), do đó cuối cùng $V_0= S$. Bổ đề 1 suy ra ngay K giao hoán, vì vậy là một xuyến cực đại của G (vì nó liên thông và có hạng cực đại). Nó chứa S và x, và bằng thành phần liên thông đơn vị của $Z(S)\cap Z(x)$; mệnh đề a) theo đó suy ra từ Bổ đề 2. Suy ra b) bằng cách lấy $g=x$ exp $a$.

#### Hệ quả {#lie-ix-s5-n3-cor-1 .statement tag=01E9}

Cho $\mathfrak{s}$ là một đại số Lie compact, và cho $\varphi$ là một tự đẳng cấu của $\mathfrak{s}$. Tồn tại một phần tử chính quy của $\mathfrak{s}$ được $\varphi$ cố định.

Thay $\mathfrak{s}$ bởi $\mathscr{D}\mathfrak{s}$, ta có thể giả sử rằng $\mathfrak{s}$ là nửa đơn. Cho S là một nhóm Lie compact đơn liên với đại số Lie $\mathfrak{s}$, và cho u là tự đẳng cấu của S sao cho $L(u) =\varphi$. Mệnh đề 3 suy ra sự tồn tại của một phần tử $a$ của $\mathfrak{s}$, được $\varphi$ cố định, sao cho exp $a$ là chính quy trong S; nói riêng, $a$ là chính quy trong $\mathfrak{s}$ (no. 2, nhận xét 4).

#### Định lý 1 {#lie-ix-s5-thm-1 .statement tag=01EA}

Cho $u$ là một tự đẳng cấu của một nhóm Lie compact liên thông G.

a) Thành phần liên thông đơn vị của nhóm các điểm bất động của $u$ chứa một phần tử chính quy của G.

b) Tồn tại một xuyến cực đại K của G và một buồng của L(K) ổn định dưới $u$.

c) Nếu G là đơn liên, tập các điểm bất động của $u$ liên thông.

Mệnh đề a) là trường hợp riêng $x=e$ của Mđề. 3. Giờ ta giả sử rằng G là đơn liên và chứng minh b) và c). Cho $x$ là một phần tử của G được $u$ cố định, và cho $g$ là một phần tử chính quy của G, được $u$ cố định và giao hoán với $x$ (Mđề. 3). Bộ trung tâm của $g$ là một xuyến cực đại của G (mục 2, Nhận xét 2), ổn định dưới $u$, và chứa $x$ và $g$. Theo Hệ quả 3 của Mđề. 2 của mục 2, tồn tại một alcove duy nhất A của L(K) sao cho $g\in$ exp A và $0\in A$; vì $g$ được cố định bởi $u, L(u)$ để lại A, và do đó cũng để lại buồng của L(K) chứa A, ổn định. Điều này chứng minh b); hơn nữa, tập hợp các điểm của K được $u$ cố định là liên thông (Bổ đề 3) và chứa $x$ và $e$, suy ra c) (Tôpô học Đại cương, Ch. I, §11, mục 1, Mđề. 2).

Còn phải chứng minh b) trong trường hợp tổng quát. Bây giờ, nếu $\widetilde{D}(G)$ là bao phủ phổ quát của D(G), và nếu $f: \widetilde{D}(G)\rightarrow G$ là cấu xạ chính tắc, thì tồn tại một tự đẳng cấu $\widetilde{u}$ của $\widetilde{D}(G)$ sao cho $f\circ \widetilde{u}=u\circ f$. Nếu $\widetilde{K}$ là một xuyến cực đại của $\widetilde{D}(G)$ và $\widetilde{C}$ một buồng của $L( \widetilde{K})$, ổn định dưới $\widetilde{u}$ (điều này tồn tại theo những gì đã được chứng minh), thì tồn tại (§2, mục 3, Nhận xét 2) một xuyến cực đại duy nhất K của G và một buồng duy nhất C của L(K) sao cho $\widetilde{K} =f^{-1}(K)$ và $\widetilde{C} = L(f)^{-1}$(C), và ta thấy ngay rằng K và C ổn định dưới $u$, do đó mệnh đề b) trong trường hợp tổng quát.

#### Hệ quả 1 {#lie-ix-s5-thm-1-cor-1 .statement tag=01EB}

Giả sử rằng $\mathbf{Z}$-môđun $\pi_1(G)$ là không xoắn.

a) Bộ trung tâm của mọi phần tử của G là liên thông.

b) Bất kỳ hai phần tử giao hoán của G đều thuộc cùng một xuyến cực đại.

Theo Hệ quả 3 của Mđề. 11 của §4, mục 6, D(G) là đơn liên. Ta có $G = C(G)_0.D(G)$; lấy $x\in G$; viết $x=uv$, với $u\in C(G)_0$ và $v\in D(G)$. Khi đó $Z(x) = C(G)_0.Z_{D(G)}(v)$. Theo ĐL. $1c), Z_{D(G)}(v)$ liên thông, nên $Z(x)$ liên thông, do đó a). Vậy, theo Hệ quả 3 của ĐL. 2 của §2, mục $2, Z(x)$ là hợp của các xuyến cực đại của G chứa $x$, do đó b).

#### Hệ quả 2 {#lie-ix-s5-thm-1-cor-2 .statement tag=01EC}

Cho $\Gamma$ là một nhóm con compact của Aut(G) với tính chất sau:

(*) Tồn tại các phần tử $u_1, . . . , u_n$ của $\Gamma$ sao cho, với mọi $i$, bao đóng $\Gamma_i$ của nhóm con của $\Gamma$ sinh bởi $u_1, . . . , u_i$ là một nhóm con chuẩn tắc của $\Gamma$, và $\Gamma_n=\Gamma$.

Khi đó, tồn tại một xuyến đại cực đại của G ổn định dưới phép toán của $\Gamma$.

Ta chứng minh bằng quy nạp theo chiều của G. Rõ ràng, ta có thể giả sử rằng $u_1\not=$ Id; khi đó nhóm con H gồm các điểm bất động của $u_1$ khác với G, và ổn định dưới phép toán của $\Gamma$. Hơn nữa, vì $\Gamma$ là compact, ảnh của $\Gamma$ trong Aut(H$_0$) là một thương của $\Gamma$, do đó nó cũng thỏa mãn điều kiện (*). Theo giả thiết quy nạp, tồn tại một xuyến đại cực đại S của H ổn định dưới $\Gamma$. Nhóm trung tâm hóa K của S trong G là liên thông (§2, no. 2, Hệ quả 5) và ổn định dưới $\Gamma$; đây là một xuyến đại cực đại của G, vì $H_0$ chứa một phần tử chính quy của G (Định lý $1a$)$)$ liên hợp với một phần tử của S (loc. cit., Hệ quả 4).

#### Hệ quả 3 {#lie-ix-s5-thm-1-cor-3 .statement tag=01ED}

Cho H là một nhóm Lie và $\Gamma$ là một nhóm con compact của H. Giả sử rằng $H_0$ là compact và rằng $\Gamma$ thỏa mãn điều kiện (*) của Hệ quả 2. Khi đó tồn tại một xuyến đại cực đại T của $H_0$ sao cho $\Gamma \subset N_H(T)$.

#### Hệ quả 4 {#lie-ix-s5-thm-1-cor-4 .statement tag=01EE}

Mọi nhóm con lũy linh của một nhóm Lie compact đều được chứa trong nhóm chuẩn hóa của một xuyến đại cực đại.

Cho H là một nhóm Lie compact, N là một nhóm con lũy linh của H. Khi đó bao đóng $\Gamma$ của N cũng là một nhóm lũy linh (Chap. III, §9, no. 1, Hệ quả 2 của Mệnh đề 1), và nhờ Hệ quả 3, chỉ cần chứng minh rằng $\Gamma$ thỏa mãn điều kiện (*). Bây giờ $\Gamma_0$ là một nhóm Lie compact lũy linh liên thông, do đó là một xuyến (§1, no. 4, Hệ quả 1 của Mệnh đề 4), và tồn tại một phần tử $u_1$ của $\Gamma$ sinh ra một nhóm con trù mật của $\Gamma_0$(General Topology, Chap. VII, §1, no. 3, đoạn văn đứng trước Mệnh đề 8). Nhóm hữu hạn $\Gamma /\Gamma_0$ là lũy linh và tồn tại $\widetilde{u}_2, . . . ,\widetilde{u}_n\in \Gamma /\Gamma_0$ sinh ra $\Gamma /\Gamma_0$ và sao cho nhóm con của $\Gamma /\Gamma_0$ được sinh bởi $(\widetilde{u}_2, . . . ,\widetilde{u}_r)$ là chuẩn tắc với $r= 2, . . . , n($Algebra, Chap. I, §6, no. 5, Định lý 1 và no. 7, Định lý 4). Khi đó, nếu $u_2, . . . , u_n$ là các đại diện của $\widetilde{u}_2, . . . ,\widetilde{u}_n$ trong $\Gamma$, thì dãy $(u_1, . . . , u_n)$ có các tính chất yêu cầu.

#### Ví dụ {#lie-ix-s5-n3-exa-1 .statement tag=01EF}

Xét $G =\mathbf{U}(n,\mathbf{C})$. Sau này ta sẽ thấy rằng nhóm con các ma trận đường chéo trong G là một xuyến đại cực đại của G và nhóm chuẩn hóa của nó là tập hợp các ma trận đơn thức (Algebra, Chap. II, §10, no. 7, Ví dụ II) trong G.

Suy ra rằng, nếu $\Phi$ là một dạng Hermit dương phân biệt trên một không gian vectơ phức hữu hạn chiều V và $\Gamma$ là một nhóm con lũy linh của $\mathbf{U}(\Phi )$, thì tồn tại một cơ sở của V sao cho các ma trận của các phần tử của $\Gamma$ là các ma trận đơn thức (“Định lý Blichtfeldt”).

### 4. CÁC ÁNH XẠ (G$\boldsymbol{/}$T) $\times \mathbf{T}\rightarrow$ G VÀ (G$\boldsymbol{/}$T) $\times \mathbf{A}\rightarrow \mathbf{G}_{\boldsymbol{r}}$

Ánh xạ $(g, t) \rightarrow gtg^{-1}$ từ $G\times T$ đến G cảm sinh qua phép thương một cấu xạ của các đa tạp giải tích

$$
f: (G/T)\times T\rightarrow G
$$

và là toàn ánh (§2, no. 2, Định lý 2). Bằng hạn chế, $f$ cảm sinh một cấu xạ toàn ánh

$$
f_r: (G/T)\times T_r\rightarrow G_r
$$

Bằng hợp thành với Id$_{G/T}\times$ exp$_T$, ta thu được các cấu xạ, cũng toàn ánh,

$$
\varphi : (G/T)\times \mathfrak{t}\rightarrow G
$$

$$
\varphi_r: (G/T)\times \mathfrak{t}_r\rightarrow G_r
$$

cuối cùng, nếu A là một alcove của $\mathfrak{t},\varphi_r$ cảm sinh một cấu xạ toàn ánh

$$
\varphi_A: (G/T)\times A\rightarrow G_r
$$

Ta định nghĩa một phép toán phải của $W$ trên $G/T$ như sau: cho $w\in W$ và $u\in G/T$; nâng $w$ lên thành một phần tử $n$ của $N_G(T)$ và $u$ lên thành một phần tử $g$ của G. Khi đó ảnh của $gn$ trong $G/T$ không phụ thuộc vào lựa chọn $n$ và $g$; ta ký hiệu nó là $u.w$.

Đối với phép toán này, $W$ tác động tự do trên $G/T:$ thật vậy, với các ký hiệu ở trên, giả sử rằng $u.w=u$; khi đó $gn\in gT$, suy ra $n\in T$ và $w= 1$.

Ta định nghĩa một phép toán phải của $W$ trên $(G/T)\times T$ bởi

$$
(u, t).w= (u.w, w^{-1}(t)),u\in G/T, t\in T, w\in W
$$

và một phép toán phải của $W'_a$ trên $(G/T)\times \mathfrak{t}$ bởi

$$
(u, x).\omega = (u.\omega , \omega^{-1}(x)),u\in G/T, x\in \mathfrak{t}, \omega \in W'_a
$$

trong đó $\overline{\omega}$ là ảnh của $\omega$ trong thương $W'_a/\Gamma (T) = W$.

Nếu A là một buồng của $\mathfrak{t}$, và nếu $H_A$ là nhóm con của $W'_a$ giữ ổn định A, thì bằng cách hạn chế ta thu được một phép toán của $H_A$ trên $(G/T)\times A$.

Các phép toán khác nhau này tương thích với các cấu xạ $f, \varphi$ và $\varphi_A:$ với $u\in G/T, t\in T, x\in \mathfrak{t}, y\in A, w\in W, \omega \in W'_a, h\in H_A$, ta có

$$
f((u, t).w) =f(u, t), \varphi ((u, x).\omega ) =\varphi (u, x), \varphi_A((u, y).h) =\varphi_A(u, y)
$$

#### Bổ đề 4 {#lie-ix-s5-lem-4 .statement tag=01EG}

Cho $g\in G,t\in T$, và cho $\overline{g}$ là ảnh của $g$ trong $G/T$. Đồng nhất không gian tiếp tuyến của $G/T$ (tương ứng T, tương ứng G) tại $\overline{g}$ (tương ứng $t$, tương ứng $gtg^{-1}$) với $\mathfrak{g}/\mathfrak{t}$ (tương ứng $\mathfrak{t}$, tương ứng $\mathfrak{g}$) bằng phép tịnh tiến trái $\gamma (g)$ bởi $g$ (tương ứng $t$, tương ứng $gtg^{-1}$). Khi đó ánh xạ tuyến tính tiếp tuyến của $f$ tại $(\overline{g}, t)$ được đồng nhất với ánh xạ tuyến tính $f': (\mathfrak{g}/\mathfrak{t})\times \mathfrak{t}\rightarrow \mathfrak{g}$ được định nghĩa như sau: nếu $z\in \mathfrak{g}, x\in \mathfrak{t}$, và nếu $\overline{z}$ ký hiệu ảnh của $z$ trong $\mathfrak{g}/\mathfrak{t}$, thì

$f'(\overline{z}, x) =$ (Ad $gt^{-1}$)$(z-$(Ad $t$)$z+x)$.

Cho $F$ là ánh xạ từ $G\times T$ vào T sao cho $F(g, t) =gtg^{-1}$. Vì $F\circ (\gamma (g)$, Id$_T) =$ Int $g\circ F$, ta có $T_{(g,t)}(F)(gz, tx) = T_t$(Int $g$)$\circ T_{(e,t)}(F)(z, tx)$; theo Chương III, §3, no. 12, Mệnh đề 46,

$T_{(e,t)}(F)(z, tx) =t$((Ad $t^{-1}$)$z-z$) $+tx=t$((Ad $t^{-1}$)$(z-$ (Ad $t$)$z+x$))

và do đó

$T_{(g,t)}(F)(gz, tx) =gtg^{-1}$((Ad $gt^{-1}$)$(z-$ (Ad $t$)$z+x$)).

Bổ đề suy ra ngay lập tức từ công thức này bằng cách đi qua thương.

#### Mệnh đề 4 {#lie-ix-s5-prop-4 .statement tag=01EH}

a) Cho $g\in G, t\in T, x\in \mathfrak{t}$, và cho $\overline{g}$ là ảnh của $g$ trong $G/T$. Các điều kiện sau là tương đương:

(i) $t\in T_r$ (resp. $x\in \mathfrak{t}_r$).

(i bis) Phần tử $f(\overline{g}, t)$ (resp. $\varphi (\overline{g}, x)$) là chính quy trong G.

(ii) Ánh xạ $f$ (resp. $\varphi$ ) là một ánh xạ chìm tại điểm $(\overline{g}, t)$ (resp. $(\overline{g}, x)$).

(ii bis) Ánh xạ $f$ (resp. $\varphi$ ) là étale tại điểm $(\overline{g}, t)$ (resp. $(\overline{g}, x)$).

b) Ánh xạ $f_r$ (resp. $\varphi_r$, resp. $\varphi_A$) làm cho $(G/T)\times T_r$ (resp. $(G/T)\times \mathfrak{t}_r$, resp. $(G/T)\times A$) thành một phủ chính của $G_r$ với nhóm W (resp. $W'_a$, resp. $H_A$).

a) Sự tương đương giữa (i) và (i bis) là rõ ràng; sự tương đương giữa (ii) và (ii bis) suy ra từ các quan hệ dim((G$/T$)$\times T$) $=$ dim((G$/T$)$\times \mathfrak{t}$) $=$ dim(G). Theo Bổ đề 4, $f$ là một submersion tại điểm $(\overline{g}, t)$ khi và chỉ khi $\mathfrak{g}=\mathfrak{t}+$ Im(Ad $t-$Id), điều này có nghĩa là $t$ là chính quy. Cuối cùng, vì $\varphi =f\circ$ (Id$_{G/T}\times$ exp$_T$)$,\varphi$ là étale tại điểm $(\overline{g}, x)$ khi và chỉ khi $f$ là étale tại điểm $(\overline{g}$, exp $x$), mà theo điều trên thì điều đó có nghĩa là $x$ thuộc $\mathfrak{t}_r$.

b) Vì thế các morphism $f_r, \varphi_r, \varphi_A$ đều là étale. Mặt khác, W tác động tự do trên $G/T$, và a fortiori trên $(G/T)\times T$. Giả sử $g, g'$ trong G và $t, t'$ trong $T_r$ sao cho $f(\overline{g}, t) =f(\overline{g}', t')$; khi đó Int $g^{-1}g'$ ánh xạ $t'$ thành $t$, và do đó chuẩn hóa T, vì $T = Z(t)_0= Z(t')_0$, và lớp $w$ của $g^{-1}g'$ trong W ánh xạ $(\overline{g}, t)$ thành $(\overline{g}', t')$. Suy ra rằng $f_r$ là một phủ chính với nhóm W; điều này ngay lập tức suy ra rằng $\varphi_r$ là một phủ chính với nhóm $W'_a$, và do đó bởi hạn chế lên thành phần liên thông $(G/T)\times A$ của $(G/T)\times \mathfrak{t}_r$, rằng $\varphi_A$ là một phủ chính với nhóm $H_A$.

#### Nhận xét 1 {#lie-ix-s5-n4-rem-1 .statement tag=01EI}

Theo Mệnh đề 3 của §2, no. 4, đa tạp $(G/T)\times A$ là đơn liên. Suy ra rằng $\varphi_A$ là một phủ phổ quát của $G_r$; vì $\pi_1(G_r)$ đẳng cấu chính tắc với $\pi_1(G)$ (no. 1, Mệnh đề 1 và Tôpô đại cương, Chương XI, đang soạn thảo), ta thu lại được sự kiện rằng $\pi_1(G)$ có thể được đồng nhất với $H_A$ (tức là với $\Gamma (T)/N(G,T)$).

#### Nhận xét 2 {#lie-ix-s5-n4-rem-2 .statement tag=01EJ}

Sự hạn chế của $\varphi_A$ lên $W\times A\subset (G/T)\times A$ làm cho $W\times A$ trở thành một phủ chính của $T_r$ với nhóm $H_A$. Do đó ta thu lại Hệ quả 1 của Mệnh đề 2 của no. 2.

#### Nhận xét 3 {#lie-ix-s5-n4-rem-3 .statement tag=01EK}

Ký hiệu $\mathfrak{g}_r$ là ảnh ngược của $G_r$ qua ánh xạ mũ và $\varepsilon :\mathfrak{g}_r\rightarrow G_r$ là ánh xạ cảm sinh bởi exp$_G$. Ánh xạ $(g, x) \rightarrow$ (Ad $g$)$(x)$ từ $G\times \mathfrak{t}_r$ đến $\mathfrak{g}_r$ xác định qua phép đi qua thương một ánh xạ $\psi_r: (G/T)\times \mathfrak{t}_r\rightarrow \mathfrak{g}_r$. Ta có $\varepsilon \circ \psi_r=\varphi_r$. Cho $w\in W, \gamma \in \Gamma (T)$ và $\omega \in W'_a$ sao cho $\omega (z) =w(z) +\gamma$ với mọi $z\in \mathfrak{t}$; khi đó $\psi_r((\overline{g}, x)\omega ) =\psi_r(\overline{g}, x)-$ (Ad $g$)$(\gamma )$ với $g\in G, x\in \mathfrak{t}_r$, do đó $\psi_r((\overline{g}, x)\omega ) =\psi_r(\overline{g}, x)$ khi và chỉ khi $\gamma = 0$. Suy ra (xem General Topology, Chương XI, đang soạn thảo) rằng $\psi_r$ là một bản phủ chính của $\mathfrak{g}_r$ với nhóm W, và rằng $\varepsilon :\mathfrak{g}_r\rightarrow G_r$ là một bản phủ liên kết với bản phủ chính $\varphi_r$, với sợi đẳng cấu với $W'_a$-tập $W'_a/W$.

### Bài tập {#lie-ix-s5-exercises}

Xem [bài tập cho § 5](exercises/s5/).
