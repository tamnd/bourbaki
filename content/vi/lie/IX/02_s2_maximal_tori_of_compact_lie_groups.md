---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 2
section_title: Maximal tori of compact Lie groups
lang: vi
source: lie-vii-ix
book_pages: 287-295, 391-394
pdf_pages: 0294-0302, 0398-0401
extraction: native+ocr
subsections:
    - "no": 1
      title: CARTAN SUBALGEBRAS OF COMPACT ALGEBRAS
      page: 287
      pdf_page: 294
    - "no": 2
      title: MAXIMAL TORI
      page: 288
      pdf_page: 295
    - "no": 3
      title: MAXIMAL TORI OF SUBGROUPS AND QUOTIENT GROUPS
      page: 291
      pdf_page: 298
    - "no": 4
      title: SUBGROUPS OF MAXIMAL RANK
      page: 292
      pdf_page: 299
    - "no": 5
      title: WEYL GROUP
      page: 293
      pdf_page: 300
    - "no": 6
      title: MAXIMAL TORI AND COVERING OF HOMOMORPHISMS
      page: 295
      pdf_page: 302
statements: 32
exercises: 11
content_sha256: d0979066547d5133e3be9b94ad6495d07899a2fa10e910bac103db69d609f90c
translated_from: content/en/lie/IX/02_s2_maximal_tori_of_compact_lie_groups.md
source_content_sha256: c325701fafe83ff98a87561b934f3da09b5a895b57956ea7453a3b2a69d0d21c
translation_model: gpt-5-6, gpt-5.4
translation_run: translate-vi-fac2a5a0
glossary_version: 34
glossary_terms_sha256: f6ecd22ba693f38195d7935f75bc35044e2515d97236c8670490eaa5f4d6f562
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC TORI CỰC ĐẠI CỦA CÁC NHÓM LIE COMPACT

### 1. CÁC ĐẠI SỐ CARTAN CỦA CÁC ĐẠI SỐ COMPACT

#### Bổ đề 1 {#lie-ix-s2-lem-1 .statement tag=019Z}

Cho G là một nhóm Lie, K là một nhóm con compact của G, và F là một dạng song tuyến tính bất biến trên L(G). Cho $x, y\in L(G)$. Tồn tại một phần tử $k$ của K sao cho $F(u$,[(Ad $k$)$(x), y]) = 0$ với mọi $u\in L(K)$.

Hàm $v \rightarrow$ F((Ad $v$)$(x), y$) từ K vào $\mathbf{R}$ là liên tục, và do đó đạt giá trị nhỏ nhất tại một điểm $k\in K$. Cho $u\in L(K)$ và đặt

$h(t) =$ F((Ad exp($tu$)$.k$)$(x), y$)$,t\in \mathbf{R}$.

Ta có $h(t)\geq h(0)$ với mọi $t$; hơn nữa, theo Ch. III, §3, no. 12, Mệnh đề 44,

$\frac{dh}{dt}(0) = F([u$,(Ad $k$)$(x)], y) = F(u$,[(Ad $k$)$(x), y])$,

do đó bổ đề được chứng minh (Hàm của một Biến Thực, Ch. I, §1, no. 7, Mệnh đề 7).

#### Định lý 1 {#lie-ix-s2-thm-1 .statement tag=01A0}

Cho $\mathfrak{g}$ là một đại số Lie compact. Các đại số con Cartan của $\mathfrak{g}$ (Chương VII, §2, no. 1, Định nghĩa 1) là các đại số con giao hoán cực đại của nó; đặc biệt, $\mathfrak{g}$ là hợp của các đại số con Cartan của nó. Nhóm Int($\mathfrak{g}$) tác dụng bắc cầu trên tập hợp các đại số con Cartan của $\mathfrak{g}$.

Vì $\mathfrak{g}$ là khả quy, các đại số con Cartan của nó là giao hoán (Chương VII, §2, no. 4, Hệ quả 3 của Định lý 2). Ngược lại, cho $\mathfrak{t}$ là một đại số con giao hoán của $\mathfrak{g}$. Theo §1, no. 3, Mệnh đề 1, ad $x$ là nửa đơn với mọi $x\in \mathfrak{t}$; theo Chương VII, §2, no. 3, Mệnh đề 10, tồn tại một đại số con Cartan của $\mathfrak{g}$ chứa $\mathfrak{t}$. Điều này chứng minh mệnh đề thứ nhất của định lý.

Bây giờ cho $\mathfrak{t}$ và $\mathfrak{t}'$ là hai đại số con Cartan của $\mathfrak{g}$. Ta chứng minh rằng tồn tại $u\in$ Int($\mathfrak{g}$) sao cho $u(\mathfrak{t}) =\mathfrak{t}'$. Theo Mệnh đề 1 của §1, no. 3, ta có thể giả sử rằng $\mathfrak{g}$ có dạng L(G), trong đó G là một nhóm Lie compact liên thông, và có thể chọn một dạng song tuyến tính đối xứng bất biến phân ly F trên $\mathfrak{g}$. Cho $x$ (resp. $x'$) là một phần tử chính quy của $\mathfrak{g}$ sao cho $\mathfrak{t}=\mathfrak{g}^0(x)$ (resp. $\mathfrak{t}'=\mathfrak{g}^0(x')$) (Chap. VII, §3, no. 3, Định lý 2). Áp dụng Bổ đề 1 với K = G, ta thấy rằng tồn tại $k\in G$ sao cho [(Ad $k$)$(x), x']$ trực giao với $\mathfrak{g}$ đối với F, và do đó bằng không; khi đó (Ad $k$)$(x)\in \mathfrak{g}^0(x') =\mathfrak{t}'$, nên $\mathfrak{g}^0$((Ad $k$)$(x)$) $=\mathfrak{t}'$ vì (Ad $k$)$(x)$ là chính quy. Ta kết luận rằng (Ad $k$)$(\mathfrak{t}) =\mathfrak{t}'$, do đó được định lý.

#### Hệ quả {#lie-ix-s2-n1-cor-1 .statement tag=01A1}

Cho $\mathfrak{t}$ và $\mathfrak{t}'$ là các dưới đại số Cartan của $\mathfrak{g},\mathfrak{a}$ là một tập con của $\mathfrak{t}$, và $u$ là một tự đẳng cấu của $\mathfrak{g}$ đưa $\mathfrak{a}$ vào $\mathfrak{t}'$. Tồn tại một phần tử $v$ của Int($\mathfrak{g}$) sao cho $u\circ v$ đưa $\mathfrak{t}$ lên $\mathfrak{t}'$, và trùng với $u$ trên $\mathfrak{a}$.

Đặt G = Int($\mathfrak{g}$), và xét bộ cố định $Z_G(\mathfrak{a})$ của $\mathfrak{a}$ trong G; đó là một nhóm con Lie của G, mà đại số Lie $\mathfrak{z}_{\mathfrak{g}}(\mathfrak{a})$ của nó gồm các phần tử của $\mathfrak{g}$ giao hoán với mọi phần tử của $\mathfrak{a}$ (Chương III, §9, no. 3, Mệnh đề 7). Khi đó $\mathfrak{t}$ và $u^{-1}(\mathfrak{t}')$ là hai đại số con Cartan của đại số Lie compact $\mathfrak{z}_{\mathfrak{g}}(\mathfrak{a})$. Theo Định lý 1, tồn tại một phần tử $v$ của $Z_G(\mathfrak{a})$ sao cho $v(\mathfrak{t}) =u^{-1}(\mathfrak{t}')$; mọi phần tử như vậy đều có các tính chất cần có.

### 2. CÁC XUYẾN CỰC ĐẠI

Cho G là một nhóm Lie. Một xuyến của G là một nhóm con đóng là một xuyến (§1, no. 2), nói cách khác là một nhóm con giao hoán compact liên thông bất kỳ. Các phần tử cực đại của tập hợp các xuyến của G, có thứ tự bởi quan hệ bao hàm, được gọi là các xuyến cực đại của G.

#### Định lý 2 {#lie-ix-s2-thm-2 .statement tag=01A2}

Cho G là một nhóm Lie compact liên thông.

a) Các đại số Lie của các xuyến cực đại của G là các đại số con Cartan của L(G).

b) Cho $T_1$ và $T_2$ là hai xuyến cực đại của G. Tồn tại $g\in G$ sao cho $T_2=gT_1g^{-1}$.

c) G là hợp của các xuyến cực đại của nó.

Cho $\mathfrak{t}$ là một đại số con Cartan của L(G); nhóm con nguyên của G có đại số Lie là $\mathfrak{t}$ thì đóng (Chương VII, §2, no. 1, Hệ quả 4 của Mệnh đề 4) và giao hoán (Định lý 1), và do đó là một xuyến của G. Nếu T là một xuyến cực đại của G, thì đại số Lie của nó là giao hoán, nên được chứa trong một đại số con Cartan của L(G) (Định lý 1). Suy ra các xuyến cực đại của G chính là các nhóm con nguyên của G liên kết với các đại số con Cartan của L(G), do đó $a)$. Mệnh đề $b)$ suy ra từ Định lý 1, vì đồng cấu chính tắc $G\rightarrow$ Int(L(G)) là toàn ánh (Chương III, §6, no. 4, Hệ quả 4 của Mệnh đề 10).

Ký hiệu X là hợp của các xuyến cực đại của G, và cho T là một xuyến cực đại của G. Ánh xạ liên tục $(g, t) \rightarrow gtg^{-1}$ từ $G\times T$ vào G có ảnh là X, vì thế X đóng trong G; do đó, để chứng minh $c)$, chỉ cần chứng minh rằng X mở trong G; vì X là bất biến dưới các tự đẳng cấu nội, chỉ cần chỉ ra rằng, với mọi $a\in T, X$ là một lân cận của $a$. Ta lập luận bằng quy nạp theo chiều của G và phân biệt hai trường hợp:

$1)a$ không thuộc tâm của G. Gọi H là thành phần đơn vị của tập trung hóa của $a$ trong G; đó là một nhóm con compact liên thông của G, phân biệt với G, chứa T, và do đó chứa $a$. Vì Ad $a$ là nửa đơn (§1, no. 1), đại số Lie của H là không gian-không của Ad $a-1$; từ Chap. VII, §4, no. 2, Prop. 4, suy ra rằng hợp Y của các liên hợp của H là một lân cận của $a$. Theo giả thiết quy nạp, $H\subset X$, và do đó $Y\subset X$; vì vậy, X là một lân cận của $a$.

$2)a$ là trung tâm trong G. Chỉ cần chứng minh rằng $a$ exp $x$ thuộc về X với mọi $x$ trong L(G). Bây giờ mọi phần tử $x$ của L(G) đều thuộc một đại số con Cartan của G (Định lý 1); nhóm con nguyên tương ứng $T'$ chứa exp $x$; vì nó liên hợp với T, nó chứa $a$ và do đó chứa $a$ exp $x$, như phải chứng minh.

#### Hệ quả 1 {#lie-ix-s2-thm-2-cor-1 .statement tag=01A3}

a) Ánh xạ mũ của G là toàn ánh.

b) Với mọi $n\geq 1$, ánh xạ $g \rightarrow g^n$ từ G vào chính nó là toàn ánh.

Thật vậy, exp(L(G)) chứa mọi xuyến cực đại của G, do đó có $a)$. Mệnh đề $b)$ suy ra từ công thức (exp $x$)$^n=$ exp $nx$ với $x$ thuộc L(G).

#### Nhận xét 1 {#lie-ix-s2-n2-rem-1 .statement tag=01A4}

Tồn tại một tập con compắc K của L(G) sao cho exp$_G(K) = G$. Thật vậy, nếu T là một xuyến cực đại của G, thì tồn tại một tập con compắc $C\subset L(T)$ sao cho exp$_T(C) = T$; chỉ cần lấy $K =\bigcup_{g\in G}$(Ad $g$)$(C)$.

#### Hệ quả 2 {#lie-ix-s2-thm-2-cor-2 .statement tag=01A5}

Giao của các xuyến cực đại của G là tâm của G.

Cho $x$ là một phần tử của tâm của G; theo Định lý $2c)$, tồn tại một xuyến cực đại T của G chứa $x$; khi đó $x$ thuộc mọi liên hợp của T, do đó thuộc mọi xuyến cực đại của G. Ngược lại, nếu $x$ thuộc mọi xuyến cực đại của G, thì nó giao hoán với mọi phần tử của G theo Định lý $2c)$.

#### Hệ quả 3 {#lie-ix-s2-thm-2-cor-3 .statement tag=01A6}

Cho $g\in G$, và gọi C là trung tâm hoá tử của nó. Khi đó $g$ thuộc $C_0$; nhóm $C_0$ là hợp của các xuyến cực đại của G chứa $g$.

Tồn tại một xuyến cực đại T của G chứa $g$ (Định lý $2c$)$)$, và do đó được chứa trong $C_0$. Hơn nữa, nhóm $C_0$ là một nhóm Lie compact liên thông, và do đó là hợp của các xuyến cực đại của nó (Định lý $2c$)$)$; tất cả các xuyến này đều chứa $g$ (Hệ quả 2), do đó chính là các xuyến cực đại của G chứa $g$.

#### Hệ quả 4 {#lie-ix-s2-thm-2-cor-4 .statement tag=01A7}

Cho $g\in G$. Nếu $g$ là chính quy (Chap. VII, §4, no. 2, Định nghĩa 2), nó thuộc về một xuyến cực đại duy nhất, xuyến này là thành phần đơn vị của trung tâm hóa tử của nó. Nếu không, nó thuộc về vô hạn xuyến cực đại.

Vì Ad $g$ là nửa đơn, nên chiều của không gian riêng không của Ad $g-1$ cũng là chiều của bộ tập trung hóa C của $g$. Theo loc. cit., Mệnh đề 8, và Định lý $1,g$ là chính quy khi và chỉ khi $C_0$ là một xuyến cực đại của G. Kết luận bây giờ suy ra từ Hệ quả 3.

#### Hệ quả 5 {#lie-ix-s2-thm-2-cor-5 .statement tag=01A8}

a) Cho S là một xuyến của G. Bộ tập trung hóa của S là liên thông; nó là hợp của các xuyến cực đại của G chứa S.

b) Cho $\mathfrak{s}$ là một đại số con giao hoán của L(G). Bộ bất động của $\mathfrak{s}$ trong G là liên thông; nó là hợp của các xuyến cực đại của G mà các đại số Lie của chúng chứa $\mathfrak{s}$.

Để chứng minh $a)$, chỉ cần chứng minh rằng nếu một phần tử $g$ của G tập trung hóa S thì tồn tại một xuyến cực đại của G chứa S và $g$. Bây giờ, nếu C là bộ tập trung hóa của $g$, thì ta có $g\in C_0$ (Hệ quả 3) và $S\subset C_0$; nếu T là một xuyến cực đại của nhóm Lie compact liên thông $C_0$ chứa S, thì ta có $g\in T$ (Hệ quả 2), do đó suy ra $a)$. Mệnh đề $b)$ suy ra từ $a)$ khi áp dụng cho bao đóng của nhóm con nguyên có đại số Lie là $\mathfrak{s}$, theo Chương III, §9, no. 3, Mệnh đề 9.

#### Nhận xét 2 {#lie-ix-s2-n2-rem-2 .statement tag=01A9}

Từ Hệ quả 5 suy ra rằng một xuyến cực đại của G là một nhóm con giao hoán cực đại. Đảo lại là không đúng: chẳng hạn, trong nhóm $\mathbf{S}\mathbf{O}(3,\mathbf{R})$, các xuyến cực đại có chiều 1, và do đó không thể chứa nhóm con các ma trận đường chéo, nhóm này đẳng cấu với $(\mathbf{Z}/2\mathbf{Z})^2$. Hơn nữa, nếu $g\in \mathbf{S}\mathbf{O}(3,\mathbf{R})$ là một ma trận đường chéo không vô hướng, thì $g$ là một phần tử chính quy của $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ mà bộ trung tâm hóa không liên thông (xem Hệ quả 4).

#### Hệ quả 6 {#lie-ix-s2-thm-2-cor-6 .statement tag=01AA}

Các xuyến cực đại của G là bộ trung tâm hóa của chính mình, và là bộ cố định của các đại số Lie của chúng.

Cho T là một xuyến cực đại của G và C là bộ trung tâm hóa của nó; vì L(T) là một đại số con Cartan của L(G), nên ta có L(T) = L(C), do đó C = T vì C liên thông (Hệ quả 5).

#### Hệ quả 7 {#lie-ix-s2-thm-2-cor-7 .statement tag=01AB}

Cho T và $T'$ là hai xuyến cực đại của G, A là một tập con của T và $s$ là một tự đẳng cấu của G biến A vào $T'$. Tồn tại $g\in G$ sao cho $s\circ$ (Int $g$) biến T thành $T'$ và trùng với $s$ trên A.

Cho C là bộ tập trung của A. Khi đó T và $s^{-1}(T')$ là hai xuyến cực đại của $C_0$; mọi phần tử $g$ của $C_0$ sao cho (Int $g$)$(T) =s^{-1}(T')$ đều có các tính chất mong muốn.

#### Hệ quả 8 {#lie-ix-s2-thm-2-cor-8 .statement tag=01AC}

Cho H là một nhóm Lie compact, T một xuyến cực đại của H. Khi đó $H = N_H(T).H_0$, và đơn ánh của $N_H(T)$ vào H cảm sinh một đẳng cấu từ $N_H(T)/N_{H_0}(T)$ đến $H/H_0$.

Cho $h\in H$. Khi đó $h^{-1}Th$ là một xuyến cực đại của $H_0$, do đó (Đl. 2) tồn tại $g\in H_0$ sao cho $hg\in N_H(T)$; vì thế $h$ thuộc $N_H(T).H_0$, suy ra mệnh đề thứ nhất. Mệnh đề thứ hai suy ra ngay lập tức.

#### Nhận xét 3 {#lie-ix-s2-n2-rem-3 .statement tag=01AD}

Cho G là một nhóm Lie liên thông mà đại số Lie của nó là compact. Các nhóm con Cartan của G là các nhóm con nguyên có đại số Lie là các đại số con Cartan của L(G) (do đó các nhóm con Cartan của một nhóm compact liên thông chính là các xuyến cực đại của nó). Định lý 2 và các hệ quả của nó vẫn còn đúng cho G, nếu ở mọi chỗ ta thay thế cụm từ “xuyến cực đại” bằng “nhóm con Cartan”. Điều này suy ra ngay lập tức từ sự kiện rằng, theo Mệnh đề 5 của §1, no. 4, G là tích trực tiếp của một nhóm vectơ V và một nhóm compact liên thông K, và các nhóm con Cartan của G là các tích của V với các xuyến cực đại của K. Hơn nữa, chú ý rằng từ Hệ quả 6 ở trên cũng suy ra rằng các nhóm con Cartan của G cũng có thể được định nghĩa như các bộ cố định của các đại số con Cartan của L(G).

$^*4)$ Phần $c)$ của Định lý 2 cũng có thể được chứng minh theo cách sau. Trang bị cho G một metric Riemann bất biến (§1, no. 3, Mệnh đề 3). Khi đó, với mọi phần tử $g$ của G, tồn tại một đường trắc địa cực đại đi qua $g$ và phần tử đơn vị của G (định lý Hopf-Rinow), và có thể kiểm tra rằng bao đóng của một đường trắc địa như vậy là một xuyến con của $G._*$

### 3. XUYẾN CỰC ĐẠI CỦA CÁC NHÓM CON VÀ CÁC NHÓM THƯƠNG

#### Mệnh đề 1 {#lie-ix-s2-prop-1 .statement tag=01AE}

Cho G và $G'$ là hai nhóm Lie compact liên thông.

a) Cho $f: G\rightarrow G'$ là một cấu xạ toàn ánh của các nhóm Lie. Các xuyến cực đại của $G'$ là các ảnh của các xuyến cực đại của G qua $f$. Nếu hạt nhân của $f$ là trung tâm trong G (chẳng hạn rời rạc), thì các xuyến cực đại của G là các ảnh nghịch qua $f$ của các xuyến cực đại của $G'$.

b) Cho H là một nhóm con đóng liên thông của G. Mọi xuyến cực đại của H đều là giao với H của một xuyến cực đại của G.

c) Cho H là một nhóm con đóng chuẩn tắc liên thông của G. Các xuyến cực đại của H là các giao với H của các xuyến cực đại của G.

$a)$ Cho T là một xuyến cực đại của G; khi đó L(T) là một đại số con Cartan của L(G) (no. 2, Định lý $2a$)$)$, nên $L(f(T))$ là một đại số con Cartan của $L(G')$ (Chương VII, §2, no. 1, Hệ quả 2 của Mệnh đề 4); do đó $f(T)$ là một xuyến cực đại của $G'$ (no. 2, Định lý $2a$)$)$. Nếu Ker $f$ là trung tâm trong G, thì nó được chứa trong T (Hệ quả 2 của Định lý 2), nên $T =f^{-1}(f(T))$.

Ngược lại, cho $T'$ là một xuyến cực đại của $G'$; ta chứng minh rằng tồn tại một xuyến cực đại T của G sao cho $f(T) = T'$. Cho $T_1$ là một xuyến cực đại của G; khi đó $f(T_1)$ là một xuyến cực đại của $G'$ và tồn tại $g'\in G'$ sao cho $T'=g'f(T_1)g^{'-1}$ (Đl. $2b$)$)$; nếu $g\in G$ sao cho $f(g) =g'$, ta có $T'=f(T)$ với $T =gT_1g^{-1}$.

$b)$ Cho S là một xuyến cực đại của H; đây là một xuyến của G nên tồn tại một xuyến cực đại T của G chứa S. Khi đó $T\cap H$ là một nhóm con giao hoán của H chứa S, do đó bằng S (no. 2, Nhận xét 2).

$c)$ Theo §1, no. 3, Mệnh đề $2c), L(G)$ là tích trực tiếp của L(H) với một iđêan; vì vậy, các đại số con Cartan của L(H) là các giao với L(H) của các đại số con Cartan của L(G). Do đó, với mọi xuyến cực đại T của $G, T\cap H$ chứa một xuyến cực đại S của H và $S = T\cap H$ (no. 2, Nhận xét 2).

#### Nhận xét 1 {#lie-ix-s2-n3-rem-1 .statement tag=01AF}

Mệnh đề 1 tổng quát hóa ngay lập tức cho các nhóm liên thông có đại số Lie compact. Đặc biệt, nếu G là một nhóm Lie liên thông mà đại số Lie của nó là compact, thì các nhóm con Cartan của G (xem Nhận xét 3, no. 2) chính xác là các ảnh ngược của các xuyến cực đại của nhóm Lie compact liên thông Ad(G) (qua đồng cấu chính tắc từ G đến Ad(G)).

#### Nhận xét 2 {#lie-ix-s2-n3-rem-2 .statement tag=01AG}

Cho G là một nhóm Lie compact liên thông, $\widetilde{D}(G)$ là phủ phổ quát của nhóm D(G), và $f: \widetilde{D}(G)\rightarrow G$ là hợp thành của các cấu xạ chính tắc từ $\widetilde{D}(G)$ đến D(G) và từ D(G) đến G. Khi đó ánh xạ $T\rightarrow f^{-1}(T)$ là một song ánh từ tập hợp các xuyến cực đại của G đến tập hợp các xuyến cực đại của $\widetilde{D}(G)$; song ánh ngược gán cho một xuyến cực đại $\widetilde{T}$ của $\widetilde{D}(G)$ xuyến cực đại $C(G)_0.f( \widetilde{T})$ của G.

### 4. CÁC NHÓM CON CÓ HẠNG CỰC ĐẠI

Ta sẽ gọi hạng của một nhóm Lie liên thông G là hạng của đại số Lie của nó, và sẽ ký hiệu nó bởi rk G. Theo Định lý 2 a), hạng của một nhóm Lie compact liên thông là chiều chung của các xuyến cực đại của nó.

Cho G là một nhóm Lie compact liên thông và H là một nhóm con đóng của G. Nếu H liên thông, thì rk $H\leq$ rk G (vì các xuyến cực đại của H là các xuyến trong G). Theo Định lý 2 c), nói rằng H liên thông và có hạng cực đại (nghĩa là, có hạng rk G) có nghĩa là H là một hợp của các xuyến cực đại của G. Ta suy ra ngay lập tức từ Mệnh đề 1:

#### Mệnh đề 2 {#lie-ix-s2-prop-2 .statement tag=01AH}

Cho $f$ : G $\rightarrow G'$ là một cấu xạ toàn ánh của các nhóm Lie compact liên thông mà hạt nhân là trung tâm. Các ánh xạ $H \rightarrow f(H)$ và $H' \rightarrow f^{-1}(H')$ là các song ánh nghịch đảo giữa tập hợp các nhóm con đóng liên thông của G có hạng cực đại và tập hợp tương tự đối với $G'$.

#### Mệnh đề 3 {#lie-ix-s2-prop-3 .statement tag=01AI}

Cho G là một nhóm Lie compact liên thông, và H là một nhóm con đóng liên thông có hạng cực đại.

$a)$ Đa tạp compact $G/H$ là đơn liên.

$b)$ Đồng cấu $\pi_1(H)\rightarrow \pi_1(G)$, cảm sinh bởi đơn ánh chính tắc của H vào G, là toàn ánh.

Vì H liên thông, ta có một dãy khớp (Tôpô đại cương, Chương XI, đang chuẩn bị)

$$
\pi_1(H)\rightarrow \pi_1(G)\rightarrow \pi_1(G/H,\overline{e})\rightarrow 0
$$

trong đó $\overline{e}$ là ảnh của phần tử đơn vị của G trong $G/H$. Vì $G/H$ liên thông, điều này ngay lập tức suy ra sự tương đương của các mệnh đề $a)$ và $b)$. Hơn nữa, nếu $f: G'\rightarrow G$ là một cấu xạ toàn ánh của các nhóm Lie compact liên thông mà hạt nhân là trung tâm, thì việc chứng minh mệnh đề (dưới dạng $a$)$)$ đối với G cũng chính là việc chứng minh nó đối với $G'$ (Mệnh đề 2). Do đó, trước hết ta có thể thay thế G bằng Ad(G), rồi giả sử rằng G là nửa đơn, và sau đó, bằng cách thay thế G bởi một phủ phổ quát (§1, no. 4, Hệ quả 2), giả sử rằng G là đơn liên. Nhưng khi đó mệnh đề $b)$ là tầm thường.

#### Mệnh đề 4 {#lie-ix-s2-prop-4 .statement tag=01AJ}

Cho G là một nhóm Lie compact, H là một nhóm con đóng liên thông của G có hạng cực đại, và N là bộ chuẩn hoá của H trong G. Khi đó H có chỉ số hữu hạn trong N và là thành phần liên thông của đơn vị của N.

Thật vậy, đại số Lie của H chứa một đại số con Cartan của L(G). Do đó, theo Chương VII, §2, no. 1, Hệ quả 4 của Mệnh đề 4, H là thành phần liên thông của đơn vị của N. Vì N compact, H có chỉ số hữu hạn trong N.

#### Nhận xét 1 {#lie-ix-s2-n4-rem-1 .statement tag=01AK}

Mọi nhóm con nguyên H của G sao cho rk H = rk G đều đóng: thật vậy, chứng minh trên cho thấy H là thành phần liên thông của đơn vị của bộ chuẩn hoá của nó, mà bộ này là một nhóm con đóng của G.

#### Nhận xét 2 {#lie-ix-s2-n4-rem-2 .statement tag=01AL}

Với các ký hiệu của Mệnh đề 4, mọi nhóm con đóng $H'$ của G chứa H và sao cho $(H': H)$ là hữu hạn đều chuẩn hoá H, và do đó được chứa trong N; tương tự, bộ chuẩn hoá của $H'$ được chứa trong N. Đặc biệt, N là bộ chuẩn hoá của chính nó.

### 5. NHÓM WEYL

Cho G là một nhóm Lie compact liên thông và T là một xuyến cực đại của G. Ký hiệu bởi $N_G(T)$ chuẩn hóa tử của T trong G; theo Mệnh đề 4 (no. 4), nhóm thương $N_G(T)/T$ là hữu hạn. Ta ký hiệu nó bởi $W_G$(T), hoặc bởi W(T), và gọi nó là nhóm Weyl của xuyến cực đại T của G, hoặc nhóm Weyl của G đối với T. Vì T là giao hoán, phép toán của $N_G(T)$ trên T bởi các tự đẳng cấu nội của G, khi chuyển sang thương, cảm sinh một phép toán, gọi là phép toán chính tắc, của nhóm $W_G(T)$ trên nhóm Lie T. Theo Hệ quả 6 của Định lý 2 ở no. 2, phép toán này là trung thành: đồng cấu liên kết $W_G(T)\rightarrow$ Aut T là đơn ánh.

Nếu $T'$ là một xuyến cực đại khác của G và nếu $g\in G$ sao cho Int $g$ ánh xạ T lên $T'$ (no. 2, Định lý $2b$)$)$, thì Int $g$ cảm sinh một đẳng cấu $a_g$ từ $W_G(T)$ lên $W_G(T')$ và $a_g(s)(gtg^{-1}) =gs(t)g^{-1}$ với mọi $s\in W_G(T)$ và mọi $t\in T$.

#### Mệnh đề 5 {#lie-ix-s2-prop-5 .statement tag=01J9}

$a)$ Mọi lớp liên hợp của G đều cắt T.

$b)$ Các giao với T của các lớp liên hợp của G là các quỹ đạo của nhóm Weyl.

Cho $g\in G$; theo Đl. 2 của no. 2, tồn tại $h\in G$ sao cho $g\in hTh^{-1}$, do đó có $a)$. Theo định nghĩa của nhóm Weyl, hai phần tử bất kỳ trong cùng một quỹ đạo của $W_G(T)$ trên T thì liên hợp trong G; ngược lại, cho $a, b$ là hai phần tử của T liên hợp dưới tác động của G. Tồn tại $h\in G$ sao cho $b=hah^{-1}$; áp dụng Hq. 7 của Đl. 2 (no. 2) với $A =\{a\},s=$ Int $h, T'= T$, ta thấy rằng tồn tại $g\in G$ sao cho Int $hg$ biến T thành T và $a$ thành $b$. Lớp của $hg$ trong $W_G(T)$ khi đó biến $a$ thành $b$, do đó mệnh đề được chứng minh.

#### Hệ quả 1 {#lie-ix-s2-prop-5-cor-1 .statement tag=01JA}

Đơn ánh chính tắc của T vào G xác định, khi chuyển sang thương, một đồng phôi từ $T/W_G(T)$ lên không gian $G/$Int(G) các lớp liên hợp của G.

Thật vậy, đó là một ánh xạ liên tục song ánh giữa hai không gian compact (x. Tôpô đại cương, Ch. III, p. 29, Hệ quả 1).

#### Hệ quả 2 {#lie-ix-s2-prop-5-cor-2 .statement tag=01JB}

Cho E là một tập con của G ổn định dưới các tự đẳng cấu nội. Khi đó E là mở (tương ứng, đóng, tương ứng, trù mật) trong G nếu và chỉ nếu $E\cap T$ là mở (tương ứng, đóng, tương ứng, trù mật) trong T.

Điều này suy ra từ Hệ quả 1 và từ việc các ánh xạ chính tắc $\mathrm{T}\to \mathrm{T}/\mathrm{W}_{G}(\mathrm{T})$ và $\mathrm{G}\to \mathrm{G}/\mathrm{Int}(\mathrm{G})$ là mở (*Tôpô đại cương*, Ch. III, p. 10, Bổ đề 2).

Ký hiệu đại số Lie của $\mathrm{G}$ là $\mathfrak{g}$, và của $\mathrm{T}$ là $\mathfrak{t}$. Phép toán của $\mathrm{W}_{G}(\mathrm{T})$ trên $\mathrm{T}$ cảm sinh một biểu diễn, gọi là *biểu diễn chính tắc*, của nhóm $\mathrm{W}_{G}(\mathrm{T})$ trên không gian vectơ $\mathbf{R}$ $\mathfrak{t}$.

#### Mệnh đề 6 {#lie-ix-s2-prop-6 .statement tag=01JC}

$a)$ *Mọi quỹ đạo của $\mathrm{G}$ trên $\mathfrak{g}$ (đối với biểu diễn phụ hợp) đều cắt $\mathfrak{t}$.*

$b)$ *Các giao với $\mathfrak{t}$ của các quỹ đạo của $\mathrm{G}$ là các quỹ đạo của $\mathrm{W}_{G}(\mathrm{T})$ trên $\mathfrak{t}$.*

Mệnh đề $a)$ suy ra từ ĐL. 1 (no. 1). Cho $x,y$ là hai phần tử của $\mathfrak{t}$ liên hợp dưới $\mathrm{Ad}(\mathrm{G})$, và cho $h\in\mathrm{G}$ sao cho $(\mathrm{Ad}\,h)(x)=y$. Áp dụng hệ quả của ĐL. 1 (no. 1) với $\mathfrak{a}=\{x\}$, $u=\mathrm{Ad}\,h$, $\mathfrak{t}'=\mathfrak{t}$, ta thấy tồn tại $g\in\mathrm{G}$ sao cho $\mathrm{Ad}\,hg$ ánh xạ $\mathfrak{t}$ lên $\mathfrak{t}$ và $x$ lên $y$. Khi đó $hg\in\mathrm{N}_{G}(\mathrm{T})$ (Chương III, §9, no. 4, Mệnh đề 11), và lớp của $hg$ trong $\mathrm{W}_{G}(\mathrm{T})$ ánh xạ $x$ lên $y$, do đó suy ra mệnh đề.

#### Hệ quả {#lie-ix-s2-n5-cor-1 .statement tag=01JD}

*Đơn ánh chính tắc của $\mathfrak{t}$ vào $\mathfrak{g}$ xác định, bằng cách chuyển sang thương, một đồng cấu từ $\mathfrak{t}/\mathrm{W}_{G}(\mathrm{T})$ đến $\mathfrak{g}/\mathrm{Ad}(\mathrm{G})$.*

Ký hiệu ánh xạ này bởi $j$; nó song ánh và liên tục (Mệnh đề 6). Ta có một biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathfrak{t} & \xrightarrow{\ i\ } & \mathfrak{g} \\
{\scriptstyle p}\downarrow\phantom{{\scriptstyle p}} & & \phantom{{\scriptstyle q}}\downarrow{\scriptstyle q} \\
\mathfrak{t}/\mathrm{W}_{G}(\mathrm{T}) & \xrightarrow{\ j\ } & \mathfrak{g}/\mathrm{Ad}(\mathrm{G})
\end{array}
$$

trong đó $p$ và $q$ là các ánh xạ thương, và $i$ là đơn ánh chính tắc. Vì $i$ và $q$ là thực sự (*Tôpô đại cương*, Chương I, §10, no. 1, Mệnh đề 2 và *Tôpô đại cương*, Chương III, §4, no. 1, Mệnh đề 2 c)) và vì $p$ là toàn ánh, suy ra $j$ là thực sự (*Tôpô đại cương*, Chương I, §10, no. 1, Mệnh đề 5), và do đó là một đồng phôi.

#### Mệnh đề 7 {#lie-ix-s2-prop-7 .statement tag=01JE}

*Cho $H$ là một nhóm con đóng của $\mathrm{G}$ chứa $\mathrm{T}$.*

$a)$ *Ký hiệu bởi $\mathrm{W}_{H}(\mathrm{T})$ nhóm con $\mathrm{N}_{H}(\mathrm{T})/\mathrm{T}$ của $\mathrm{W}_{G}(\mathrm{T})$; nhóm $H/H_{0}$ đẳng cấu với nhóm thương $\mathrm{W}_{H}(\mathrm{T})/\mathrm{W}_{H_{0}}(\mathrm{T})$.*

$b)$ *$H$ liên thông khi và chỉ khi mọi phần tử của $\mathrm{W}_{G}(\mathrm{T})$ có một đại diện trong $H$ đều thuộc về $\mathrm{W}_{H_{0}}(\mathrm{T})$.*

Mệnh đề $a)$ suy ra từ Hệ quả 8 của Định lý 2 (no. 2), và mệnh đề $b)$ là một trường hợp riêng của $a)$.

### 6. XUYẾN CỰC ĐẠI VÀ PHỦ CỦA CÁC ĐỒNG CẤU

Cho G là một nhóm Lie compact liên thông, T một xuyến cực đại của G. Xét nhóm dẫn xuất D(G) của G và phủ phổ quát $\widetilde{D}(G)$ của nó; gọi $p: \widetilde{D}(G)\rightarrow G$ là hợp thành của các đồng cấu chính tắc $\widetilde{D}(G)\rightarrow D(G)$ và $D(G)\rightarrow G$. Khi đó $\widetilde{D}(G)$ là một nhóm Lie compact liên thông (§1, no. 4, Hệ quả 2 của Mệnh đề 4); hơn nữa, ảnh ngược $\widetilde{T}$ của T theo $p$ là một xuyến cực đại của $\widetilde{D}(G)$ (no. 3, Mệnh đề 1).

#### Bổ đề 2 {#lie-ix-s2-lem-2 .statement tag=01AO}

Cho H là một nhóm Lie, $f_T: T\rightarrow H$ và $\widetilde{f}: \widetilde{D}(G)\rightarrow H$ là các cấu xạ của nhóm Lie sao cho $f_T(p(t)) = \widetilde{f}(t)$ với mọi $t\in \widetilde{T}$. Tồn tại một cấu xạ duy nhất của nhóm Lie $f: G\rightarrow H$ sao cho $f\circ p= \widetilde{f}$ và sao cho hạn chế của $f$ trên T là $f_T$.

Đặt $Z = C(G)_0$; theo §1, no. 4, Hệ quả 1 của Mệnh đề 4, cấu xạ các nhóm Lie $g: Z\times \widetilde{D}(G)\rightarrow G$ sao cho $g(z, x) =z^{-1}p(x)$ là một phủ; hạt nhân của nó gồm các cặp $(z, x)$ sao cho $p(x) =z$, khi đó $x\in p^{-1}(Z)\subset \widetilde{T}$. Vì cấu xạ $(z, x) \rightarrow f_T(z^{-1}) \widetilde{f}(x)$ từ $Z\times \widetilde{D}(G)$ đến H ánh xạ hạt nhân của $g$ vào $\{e\}$, nên tồn tại một cấu xạ $f$ từ G đến H sao cho $f\circ p= \widetilde{f}$ và $f(z) =f_T(z)$ với $z\in Z$. Nhưng ta cũng có $f(t) =f_T(t)$ với $t\in p( \widetilde{T})$; vì $T = Z.p( \widetilde{T})$, hạn chế của $f$ trên T quả thật là $f_T$.

#### Mệnh đề 8 {#lie-ix-s2-prop-8 .statement tag=01AP}

Cho G là một nhóm Lie compact liên thông, T là một xuyến cực đại của G, H là một nhóm Lie và $\varphi : L(G)\rightarrow L(H)$ là một đồng cấu các đại số Lie. Tồn tại một cấu xạ của các nhóm Lie $f: G\rightarrow H$ sao cho $L(f) =\varphi$ khi và chỉ khi tồn tại một cấu xạ của các nhóm Lie $f_T: T\rightarrow H$ sao cho $L(f_T) =\varphi |L(T)$; khi đó $f_T=f|T$.

Nếu $f: G\rightarrow H$ là một cấu xạ của các nhóm Lie sao cho $L(f) =\varphi$, thì hạn chế $f_T$ của $f$ trên T là cấu xạ duy nhất từ T vào H sao cho $L(f_T) =\varphi |L(T)$. Ngược lại, giả sử $f_T: T\rightarrow H$ là một cấu xạ của các nhóm Lie sao cho $L(f_T) =\varphi |L(T)$. Gọi $\widetilde{D}(G)$ và $p$ như trên; ánh xạ $L(p)$ cảm sinh một đẳng cấu từ $L( \widetilde{D}(G))$ lên đại số dẫn xuất $\mathfrak{b}$ của L(G). Tồn tại một cấu xạ của các nhóm Lie $\widetilde{f}: \widetilde{D}(G)\rightarrow H$ sao cho $L( \widetilde{f}) = (\varphi |\mathfrak{b})\circ L(p)$ (Chương III, §6, no. 1, Định lý 1). Các cấu xạ $t \rightarrow \widetilde{f}(t)$ và $t \rightarrow f_T(p(t))$ từ $\widetilde{T}$ vào H cảm sinh cùng một đồng cấu của các đại số Lie, và do đó trùng nhau. Áp dụng Bổ đề 2, ta suy ra sự tồn tại của một cấu xạ $f: G\rightarrow H$ sao cho $L(f)$ và $\varphi$ trùng nhau trên L(T) và $\mathfrak{b}$. Vì $L(G) =\mathfrak{b}+ L(T)$, ta có $L(f) =\varphi$.

#### Mệnh đề 9 {#lie-ix-s2-prop-9 .statement tag=01AQ}

Cho G là một nhóm Lie compact liên thông, T là một xuyến cực đại của G, H là một nhóm Lie và $f: G\rightarrow H$ là một cấu xạ. Khi đó $f$ là đơn ánh nếu và chỉ nếu hạn chế của nó trên T là đơn ánh.

Thật vậy, theo Th. 2 (no. 2), nhóm con chuẩn tắc Ker $f$ của G rút về phần tử đơn vị nếu và chỉ nếu giao của nó với T rút về phần tử đơn vị.

### Bài tập {#lie-ix-s2-exercises}

Xem [bài tập của § 2](exercises/s2/).
