---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 1
section_title: Compact Lie algebras
lang: vi
source: lie-vii-ix
book_pages: 281-287, 389-391
pdf_pages: 0288-0294, 0396-0398
extraction: native
subsections:
    - "no": 1
      title: INVARIANT HERMITIAN FORMS
      page: 281
      pdf_page: 288
    - "no": 2
      title: CONNECTED COMMUTATIVE REAL LIE GROUPS
      page: 282
      pdf_page: 289
    - "no": 3
      title: COMPACT LIE ALGEBRAS
      page: 283
      pdf_page: 290
    - "no": 4
      title: GROUPS WHOSE LIE ALGEBRA IS COMPACT
      page: 284
      pdf_page: 291
statements: 13
exercises: 9
content_sha256: 7ecf9dfec17f9e76d10891d85b5a309b792020b218aeb9590b60a867e4943634
translated_from: content/en/lie/IX/01_s1_compact_lie_algebras.md
source_content_sha256: 944894592e14a8d7609536ce9e49868c10534458947d804a90800246f3db6c8b
translation_model: gpt-5-6, gpt-5.4
translation_run: translate-vi-115a3f5d
glossary_version: 34
glossary_terms_sha256: ce05b13a8b55522a86c40dea681dac6f1ac04343dfd67b1206fae97910c7b783
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐẠI SỐ LIE COMPACT

### 1. CÁC DẠNG HERMITE BẤT BIẾN

Trong mục này, chữ $k$ ký hiệu trường $\mathbf{R}$ hoặc $\mathbf{C}$. Cho V là một không gian vectơ $k$ hữu hạn chiều, $\Phi$ là một dạng Hermit dương tách được$^2$ trên V, G là một nhóm, $\mathfrak{g}$ là một đại số Lie $\mathbf{R}$, $\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ là một đồng cấu nhóm, $\varphi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ là một đồng cấu của các đại số Lie $\mathbf{R}$.

a) Dạng $\Phi$ là bất biến dưới G (hoặc $\mathfrak{g}$) nếu và chỉ nếu $\rho (g)$ là unita đối với $\Phi$ với mọi $g\in G$ (hoặc $\varphi (x)$ là phản Hermit$^3$ đối với $\Phi$ với mọi $x\in \mathfrak{g}$). Thật vậy, ký hiệu bởi $a^*$ liên hợp của một tự đồng cấu $a$ của V đối với $\Phi$; với $g$ trong $G,x$ trong $\mathfrak{g},u$ và $v$ trong V, ta có

$$
\Phi (\rho (g)u, \rho (g)v) =\Phi (\rho (g)^*\rho (g)u, v)
$$

$$
\Phi (\varphi (x)u, v) +\Phi (u, \varphi (x)v) =\Phi ((\varphi (x) +\varphi (x)^*).u, v)
$$

$^1$ Trong suốt chương này, các tham chiếu đến Đại số, Chương VIII, là đến ấn bản mới

(đang được chuẩn bị)

$^2$ Nhắc lại (Đại số, Chương IX, đang được chuẩn bị) rằng một dạng Hermit H trên V được gọi

là phân ly (hoặc không suy biến) nếu, với mọi phần tử khác không $u$ của V, luôn

tồn tại $v\in V$ sao cho $H(u, v)\not= 0$.

$^3$ Một phần tử $a\in$ End(V) được gọi là phản Hermit đối với $\Phi$ nếu the

liên hợp $a^*$ của $a$ đối với $\Phi$ bằng $-a$. Khi $k=\mathbf{C}$ (resp. $k=\mathbf{R}$) điều này

cũng có nghĩa là tự đồng cấu $ia$ của V (resp. của $\mathbf{C}\otimes_{\mathbf{R}}V$) là Hermit. do đó, $\Phi (\rho (g)u, \rho (g)v) =\Phi (u, v)$ với mọi $u, v$ trong V khi và chỉ khi $\rho (g)^*\rho (g) =$ Id$_V$; tương tự, $\Phi (\varphi (x)u, v) +\Phi (u, \varphi (x)v) = 0$ với mọi $u, v$ trong V khi và chỉ khi $\varphi (x) +\varphi (x)^*= 0$, do đó có mệnh đề đã nêu.

b) Nếu dạng $\Phi$ là bất biến dưới G (resp. $\mathfrak{g}$), phần bù trực giao của một không gian con ổn định của V là ổn định; đặc biệt, khi đó biểu diễn $\rho$ (resp. $\varphi$ ) là nửa đơn (xem Đại số, Chương IX); hơn nữa, với mọi $g\in G$ (resp. $x\in \mathfrak{g}$), tự đồng cấu $\rho (g)$ (resp. $\varphi (x)$) của V khi đó là nửa đơn, với các giá trị riêng có giá trị tuyệt đối bằng 1 (resp. với các giá trị riêng thuần ảo); thật vậy $\rho (g)$ là unita (resp. $i\varphi (x)$ là Hermit, xem Đại số, Chương IX).

c) Giả sử rằng $k=\mathbf{R}$. Nếu G là một nhóm Lie liên thông, $\rho$ là một cấu xạ của các nhóm Lie, $\mathfrak{g}$ là đại số Lie của G và $\varphi$ là đồng cấu cảm sinh bởi $\rho$, thì $\Phi$ là bất biến dưới G khi và chỉ khi nó là bất biến dưới $\mathfrak{g}$ (Chap. III, §6, no. 5, Cor. 3).

d) Tồn tại một dạng Hermit dương phân ly trên V bất biến dưới G khi và chỉ khi nhóm con $\rho (G)$ của $\mathbf{G}\mathbf{L}(V)$ là tương đối compact (Integration, Chap. VII, §3, no. 1, Prop. 1).

### 2. NHÓM LIE THỰC GIAO HOÁN LIÊN THÔNG

Cho G là một nhóm Lie (thực) giao hoán liên thông. Ánh xạ mũ

exp$_G: L(G)\rightarrow G$

là một cấu xạ của các nhóm Lie, toàn ánh với hạt nhân rời rạc (Chap. III, §6, no. 4, Prop. 11), do đó L(G) là một phủ liên thông của G.

a) Các điều kiện sau là tương đương: G là đơn liên, exp$_G$ là một đẳng cấu, G đẳng cấu với $\mathbf{R}^n(n=$ dim G). Trong trường hợp đó, chuyển cấu trúc không gian vectơ của L(G) sang G bởi đẳng cấu exp$_G$ cho một cấu trúc không gian vectơ trên G, và đó là cấu trúc duy nhất tương thích với cấu trúc nhóm tôpô của G. Các nhóm Lie giao hoán đơn liên được gọi là các nhóm vectơ (Lie); trừ khi nói rõ khác đi, chúng luôn luôn được trang bị cấu trúc $\mathbf{R}$-không gian vectơ được định nghĩa ở trên.

b) Ký hiệu $\Gamma (G)$ là hạt nhân của exp$_G$. Theo Tôpô đại cương, Chương VII, §1, no. 1, Định lý 1, nhóm G là compắc nếu và chỉ nếu $\Gamma (G)$ là một dàn trong L(G), nói cách khác (loc. cit.) nếu hạng của $\mathbf{Z}$-môđun tự do $\Gamma (G)$ bằng chiều của G. Ngược lại, nếu L là một $\mathbf{R}$-không gian vectơ hữu hạn chiều và $\Gamma$ là một dàn trong L, thì nhóm tôpô thương $L/\Gamma$ là một nhóm Lie giao hoán liên thông compắc.

Các nhóm Lie giao hoán liên thông compắc được gọi là các xuyến thực, hoặc (trong chương này) các xuyến.

c) Trong trường hợp tổng quát, gọi E là không gian con vectơ của L(G) sinh bởi $\Gamma$ (G), và gọi V là một không gian con bù. Khi đó G là tích trực tiếp của các nhóm con Lie exp(E) và exp(V); nhóm thứ nhất là một xuyến, nhóm thứ hai là vectơ. Sau hết, mọi nhóm con compact của G đều được chứa trong exp(E) (vì phép chiếu của nó lên exp(V) tất yếu thu về phần tử đơn vị); do đó, nhóm con exp(E) là nhóm con compact cực đại duy nhất của G.

Ví dụ, lấy $G = C^*$; đồng nhất L(G) với $\mathbf{C}$ sao cho ánh xạ mũ của G là $x \rightarrow e^x$. Khi đó $\Gamma (G) = 2\pi i\mathbf{Z},E =i\mathbf{R}$, và do đó exp(E) $=\mathbf{U}$; nếu lấy $V =\mathbf{R}$, thì exp(V) $=\mathbf{R}^*_+$ và ta thu lại đẳng cấu $\mathbf{C}^*\rightarrow \mathbf{U}\times \mathbf{R}^*_+$ được xây dựng trong Tôpô đại cương, Chương VIII, §1, no. 3, Mệnh đề 1.

d) Chú ý sau hết rằng exp$_G: L(G)\rightarrow G$ là một phủ phổ quát của G, do đó $\Gamma (G)$ có thể được đồng nhất một cách tự nhiên với nhóm cơ bản của G.

### 3. ĐẠI SỐ LIE COMPACT

#### Mệnh đề 1 {#lie-ix-s1-prop-1 .statement tag=019D}

Cho $\mathfrak{g}$ là một đại số Lie (thực). Các điều kiện sau là tương đương:

(i) $\mathfrak{g}$ đẳng cấu với đại số Lie của một nhóm Lie compact.

(ii) Nhóm Int($\mathfrak{g}$) (Chương III, §6, no. 2, Định nghĩa 2) là compact.

(iii) $\mathfrak{g}$ có một dạng song tuyến tính bất biến (Chương I, §3, no. 6) đối xứng, dương và phân biệt.

(iv) $\mathfrak{g}$ là khả quy (Chương I, §6, no. 4, Định nghĩa 4); với mọi $x\in \mathfrak{g}$, tự đồng cấu ad $x$ là nửa đơn, với các trị riêng thuần ảo.

(v) $\mathfrak{g}$ là khả quy và dạng Killing B của nó là âm.

(i) $=\Rightarrow$ (ii): nếu $\mathfrak{g}$ là đại số Lie của một nhóm Lie compact G, thì nhóm Int($\mathfrak{g}$) là tách biệt và đẳng cấu với một thương của nhóm compact $G_0$ (Chương III, §6, no. 4, Hệ quả 4), do đó là compact.

(ii) $=\Rightarrow$ (iii): nếu nhóm Int($\mathfrak{g}$) là compact, thì tồn tại trên $\mathfrak{g}$ một dạng song tuyến tính đối xứng, dương, phân biệt và bất biến dưới Int($\mathfrak{g}$) (no. 1), do đó cũng bất biến dưới biểu diễn kề của $\mathfrak{g}$.

(iii) $=\Rightarrow$ (iv): nếu (iii) được thỏa mãn thì biểu diễn phụ hợp của $\mathfrak{g}$ là nửa đơn (no. 1), do đó $\mathfrak{g}$ là khả quy; hơn nữa, các nội cấu ad $x$, với $x\in \mathfrak{g}$, có các tính chất đã nêu (no. 1).

(iv) $=\Rightarrow$ (v): với mọi $x\in \mathfrak{g}, B(x, x) =$ Tr((ad $x$)$^2$); do đó, $B(x, x)$ là tổng các bình phương của các giá trị riêng của ad $x$, và vì thế là âm nếu các giá trị riêng ấy thuần túy ảo.

(v) $=\Rightarrow$ (i): giả sử rằng $\mathfrak{g}$ là khả quy, do đó là tích của một đại số con giao hoán $\mathfrak{c}$ và một đại số con nửa đơn $\mathfrak{s}$ (Ch. I, §6, no. 4, Mệnh đề 5). Dạng Killing của $\mathfrak{s}$ là hạn chế của dạng B lên $\mathfrak{s}$, do đó là âm và phân ly nếu B là âm. Nhóm con Int($\mathfrak{s}$) của $\mathbf{G}\mathbf{L}(\mathfrak{s})$ là đóng (đó là thành phần đơn vị của Aut($\mathfrak{s}$), Ch. III, §10, no. 2, Hệ quả 2) và để dạng dương phân ly $-B$ bất biến; vì thế, nó là compact, và $\mathfrak{s}$ đẳng cấu với đại số Lie của nhóm Lie compact Int($\mathfrak{s}$). Hơn nữa, vì $\mathfrak{c}$ là giao hoán, nó đẳng cấu với đại số Lie của một xuyến T. Do đó $\mathfrak{g}$ đẳng cấu với đại số Lie của nhóm Lie compact Int($\mathfrak{s}$)$\times T$.

#### Định nghĩa 1 {#lie-ix-s1-def-1 .statement tag=019E}

Một đại số Lie compact$^4$ là một đại số Lie có các tính chất (i) đến (v) của Mệnh đề 1.

Do đó, các đại số Lie compact là các tích của một đại số giao hoán với một đại số nửa đơn compact. Nói cách khác, một đại số Lie là compact khi và chỉ khi nó khả quy và đại số Lie dẫn xuất của nó là compact.

Đại số Lie của một nhóm Lie compact là compact.

#### Mệnh đề 2 {#lie-ix-s1-prop-2 .statement tag=019F}

a) Tích của một số hữu hạn đại số Lie là một đại số Lie compact khi và chỉ khi mỗi nhân tử là compact.

b) Một đại số con của một đại số Lie compact là compact.

c) Cho $\mathfrak{h}$ là một iđêan của một đại số Lie compact $\mathfrak{g}$. Khi đó đại số $\mathfrak{g}/\mathfrak{h}$ là compact và mở rộng $\mathfrak{h}\rightarrow \mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{h}$ là tầm thường.

Các khẳng định a) và b) suy ra từ đặc trưng hóa (iii) của Mệnh đề 1. Phần c) suy ra từ a) và sự kiện là, trong một đại số Lie khả quy, mọi iđêan đều là một nhân tử trực tiếp (Chương I, §6, no. 4, Hệ quả của Mệnh đề 5).

#### Mệnh đề 3 {#lie-ix-s1-prop-3 .statement tag=019G}

Cho G là một nhóm Lie mà nhóm các thành phần liên thông của nó là hữu hạn. Các điều kiện sau là tương đương:

(i) Đại số Lie L(G) là compact.

(ii) Nhóm Ad(G) là compact.

(iii) Tồn tại một dạng song tuyến tính đối xứng dương phân ly trên L(G) bất biến đối với biểu diễn liên hợp của G.

$^*$(iv) G có một metric riemann bất biến dưới các phép tịnh tiến trái và phải.$_*$

(i) $=\Rightarrow$ (ii): nếu L(G) là compact, thì nhóm Ad(G$_0$) $=$ Int(L(G)) là compact; vì nó có chỉ số hữu hạn trong Ad(G), nên nhóm sau này cũng compact.

(ii) $=\Rightarrow$ (iii): điều này suy ra từ no. 1.

(iii) $=\Rightarrow$ (i): vì Int(L(G)) $\subset$ Ad(G), điều này suy ra từ đặc trưng hóa (iii) của Mệnh đề 1.

$^*$(iii) $\Leftarrow \Rightarrow$ (iv): điều này suy ra từ Chương III, §3, số $13._*$

### 4. NHÓM CÓ ĐẠI SỐ LIE COMPACT

#### Định lý 1 {#lie-ix-s1-thm-1 .statement tag=019H}

(H. Weyl) Cho G là một nhóm Lie liên thông mà đại số Lie của nó là compact nửa đơn. Khi đó G là compact và tâm của nó là hữu hạn.

Vì G là nửa đơn, tâm D của nó là rời rạc. Hơn nữa, nhóm thương $G/D$ đẳng cấu với Ad(G) (Chương III, §6, no. 4, Hệ quả 4), do đó compact (Mệnh đề 3). Sau cùng, nhóm $G/D$ bằng với nhóm dẫn xuất của nó (Chương III, §9, no. 2, Hệ quả của Mệnh đề 4). Định lý nay suy ra từ Tích phân, Chương VII, §3, no. 2, Mệnh đề 5.

#### Mệnh đề 4 {#lie-ix-s1-prop-4 .statement tag=019I}

Cho G là một nhóm Lie liên thông mà đại số Lie của nó là compact. Tồn tại một xuyến T, một nhóm Lie nửa đơn compact đơn liên

$^4$ Chú ý rằng một không gian vectơ tô pô thực không thể là một không gian tô pô compact

trừ khi nó thu về 0. thông S, một nhóm vectơ V và một cấu xạ toàn ánh $f: V\times T\times S\rightarrow G$ với hạt nhân hữu hạn. Nếu G là compact, nhóm V thu về phần tử đơn vị.

Cho C (tương ứng S) là một nhóm Lie đơn liên mà đại số Lie của nó đẳng cấu với tâm (tương ứng đại số dẫn xuất) của L(G). Khi đó C là một nhóm vectơ, S là một nhóm compact có tâm hữu hạn (Định lý 1) và G có thể được đồng nhất với nhóm thương của $C\times S$ bởi một nhóm con rời rạc D, là trung tâm (Tích phân, Chương VII, §3, no. 2, Bổ đề 4). Vì ảnh của phép chiếu của D lên S là trung tâm, do đó hữu hạn, $D\cap C$ có chỉ số hữu hạn trong D. Cho $C'$ là không gian con vectơ của C sinh bởi $D\cap C$, và V là một không gian con bù. Khi đó nhóm $T = C'/(D\cap C)$ là một xuyến, và G đẳng cấu với nhóm thương của nhóm tích $V\times T\times S$ bởi một nhóm hữu hạn.

Nếu G là compact, thì $V\times T\times S ($Tôpô đại cương, Chương III, §4, no. 1, Hệ quả 2 của Mệnh đề 2) cũng compact, do đó V cũng compact, điều này kéo theo $V =\{e\}$.

#### Hệ quả 1 {#lie-ix-s1-prop-4-cor-1 .statement tag=019J}

Cho G là một nhóm Lie compact liên thông. Khi đó $C(G)_0$ là một xuyến, D(G) là một nhóm Lie nửa đơn compact liên thông và cấu xạ $(x, y) \rightarrow xy$ từ $C(G)_0\times D(G)$ vào G là một phủ hữu hạn.

Với ký hiệu của Mệnh đề 4, ta có $V =\{e\}$ và các nhóm con $f(T)$ và $f(S)$ của G là compact, do đó đóng. Vì vậy chỉ cần chứng minh rằng $f(T) =$ $C(G)_0,f(S) = D(G)$. Bây giờ, $L(G) = L(f(T))\times L(f(S))$; vì S là nửa đơn và T là giao hoán, điều này kéo theo $L(f(T)) =\mathscr{C}(L(G)) = L(C(G)_0)$ (Chương III, §9, no. 3, Mệnh đề 8) và $L(f(S)) =\mathscr{D}L(G) = L(D(G))$ (Chương III, §9, no. 2, Hệ quả của Mệnh đề 4), do đó được mệnh đề đã phát biểu.

#### Hệ quả 2 {#lie-ix-s1-prop-4-cor-2 .statement tag=019K}

Tâm và nhóm cơ bản của một nhóm Lie nửa đơn compact liên thông là hữu hạn. Phủ phổ quát của nó là compact.

Với ký hiệu của Mệnh đề 4, các nhóm V và T được rút về phần tử đơn vị; do đó S là một phủ phổ quát của G, và nhóm cơ bản của G đẳng cấu với Ker $f$, vì thế là hữu hạn. Tâm D của G là rời rạc vì G là nửa đơn, nên D là hữu hạn.

#### Hệ quả 3 {#lie-ix-s1-prop-4-cor-3 .statement tag=019L}

Nhóm cơ bản của một nhóm Lie compact liên thông G là một $\mathbf{Z}$-môđun kiểu hữu hạn, có hạng bằng chiều của C(G).

Thật vậy, với các ký hiệu của Hệ quả 1, nhóm cơ bản của $C(G)_0$ đẳng cấu với $\mathbf{Z}^n$, với $n=$ dim $C(G)_0$, và nhóm cơ bản của D(G) là hữu hạn (Hệ quả 2).

#### Hệ quả 4 {#lie-ix-s1-prop-4-cor-4 .statement tag=019M}

Cho G là một nhóm Lie compact liên thông. Các điều kiện sau là tương đương:

(i) G là nửa đơn;

(ii) C(G) là hữu hạn;

(i) $\pi_1(G)$ là hữu hạn.

Nếu G là đơn liên, thì nó là nửa đơn.

Điều này suy ra từ các Hệ quả 1 đến 3.

#### Hệ quả 5 {#lie-ix-s1-prop-4-cor-5 .statement tag=019N}

Cho G là một nhóm Lie compact liên thông. Khi đó Int(G) là thành phần liên thông của đơn vị của nhóm Lie Aut(G) (Ch. III, §10, no. 2).

Cho $f\in$ Aut(G)$_0$. Khi đó $f$ cảm sinh một tự đẳng cấu $f_1$ của $C(G)_0$ và một tự đẳng cấu $f_2$ của D(G), và ta có $f_1\in$ Aut(C(G)$_0$)$_0, f_2\in$ Aut(D(G))$_0$. Vì Aut(C(G)$_0$) là rời rạc (Topologie générale, Chap. VII, §2, no. 4, Prop. 5), nên ta có $f_1=$ Id; vì D(G) là nửa đơn, theo Chap. III, §10, no. 2, Cor. 2 của Th. 1 tồn tại một phần tử $g$ của D(G) sao cho $f_2(x) =gxg^{-1}$ với mọi $x\in$ D(G). Với mọi $x\in C(G)_0$, ta có $gxg^{-1}=x$ = $f_1(x)$; vì $G = C(G)_0.D(G)$, suy ra $gxg^{-1}=f(x)$ với mọi $x\in G$, vậy $f=$ Int $g$.

#### Mệnh đề 5 {#lie-ix-s1-prop-5 .statement tag=019O}

Cho G là một nhóm Lie có đại số Lie compact.

a) Giả sử rằng G liên thông. Khi đó G có một nhóm con compact lớn nhất K; nó liên thông. Tồn tại một nhóm con vectơ trung tâm đóng (no. 2) N của G sao cho G là tích trực tiếp $N\times K$.

b) Giả sử rằng nhóm các thành phần liên thông của G là hữu hạn. Khi đó:

(i) Mọi nhóm con compact của G đều được chứa trong một nhóm con compact cực đại.

(ii) Nếu $K_1$ và $K_2$ là hai nhóm con compact cực đại của G, thì tồn tại $g\in G$ sao cho $K_2=gK_1g^{-1}$.

(iii) Cho K là một nhóm con compact cực đại của G. Khi đó $K\cap G_0$ bằng $K_0$; nó là nhóm con compact lớn nhất của $G_0$.

(iv) Tồn tại một nhóm con vectơ trung tâm đóng N của $G_0$, chuẩn tắc trong G, sao cho, với mọi nhóm con compact cực đại K của G, $G_0$ là tích trực tiếp của $K_0$ với N, và G là tích nửa trực tiếp của K với N.

a) Ta giữ các ký hiệu của Mệnh đề 4. Phép chiếu của Ker $f$ lên V là một nhóm con hữu hạn của nhóm vectơ V, do đó thu về phần tử đơn vị. Suy ra Ker $f$ được chứa trong $T\times S$, và vì thế G là tích trực tiếp của nhóm vectơ $N =f(V)$ và nhóm compact $K =f(T\times S)$. Mọi nhóm con compact của G đều có một phép chiếu lên N thu về phần tử đơn vị, nên được chứa trong K. Điều này chứng minh a).

b) Bây giờ giả sử rằng $G/G_0$ là hữu hạn. Theo $a), G_0$ là tích trực tiếp của nhóm con compắc lớn nhất M của nó và một nhóm con vectơ P; nhóm con M của G rõ ràng là chuẩn tắc. Gọi $\mathfrak{n}$ là một không gian con vectơ bù của L(M) trong L(G), ổn định dưới biểu diễn phụ hợp của G (no. 1 và no. 3, Mệnh đề 3); đó là một iđêan của L(G) và ta có $L(G) = L(M)\times \mathfrak{n}$. Gọi N là nhóm con nguyên của G có đại số Lie là $\mathfrak{n}$; theo Chương III, §6, no. 6, Mệnh đề 14, nó là chuẩn tắc trong G. Phép chiếu của L(G) lên L(P) với hạt nhân L(M) gây ra một đẳng cấu từ $\mathfrak{n}$ lên L(P); suy ra rằng phép chiếu của $G_0$ lên P gây ra một cấu xạ étale từ N lên P; vì P đơn liên, đó là một đẳng cấu, và N là một nhóm vectơ. Cấu xạ $(x, y) \rightarrow xy$ từ $M\times N$ vào $G_0$ là một cấu xạ étale đơn ánh (vì $M\cap N$ thu về phần tử đơn vị), do đó là một đẳng cấu. Suy ra N là một nhóm con đóng của G và thương $G/N$ là compắc, vì $G_0/N$ là compắc và $G/G_0$ là hữu hạn (Topologie générale, Chương III, §4, no. 1, Hệ quả 2 của Mệnh đề 2).

Theo Integration, Chương VII, §3, no. 2, Mệnh đề 3, mọi nhóm con compact của G đều được chứa trong một nhóm con compact cực đại, các nhóm con này liên hợp với nhau, và với mọi nhóm con compact cực đại K của G, G là tích nửa trực tiếp của K bởi N. Vì $G_0$ chứa N nên nó là tích nửa trực tiếp của N bởi $G_0\cap K$; suy ra $G_0\cap K$ liên thông, do đó bằng $K_0$, vì $K/(G_0\cap K)$ đẳng cấu với $G/G_0$, nên hữu hạn; sau cùng, $K_0$ rõ ràng là nhóm con compact lớn nhất của $G_0$ theo a).

#### Hệ quả {#lie-ix-s1-n4-cor-1 .statement tag=019P}

Nếu N thỏa mãn các điều kiện của b) (iv), và nếu $K_1$ và $K_2$ là hai nhóm con compact cực đại của G, thì tồn tại $n\in$ N sao cho $nK_1n^{-1}= K_2$.

Thật vậy, theo (ii) tồn tại một phần tử $g\in G$ sao cho $gK_1g^{-1}= K_2$; theo (iv), tồn tại $n\in N$ và $k\in K_1$ sao cho $g=nk$. Khi đó phần tử $n$ có các tính chất cần có.

### Bài tập {#lie-ix-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
