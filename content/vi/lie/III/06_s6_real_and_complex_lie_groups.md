---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 6
section_title: Real and complex Lie groups
lang: vi
source: lie-i-iii
pdf_pages: 0322-0344, 0401-0409
extraction: ocr
subsections:
    - "no": 1
      title: PASSAGE FROM LIE ALGEBRA MORPHISMS TO LIE GROUP MORPHISMS
      page: 0
      pdf_page: 322
    - "no": 2
      title: INTEGRAL SUBGROUPS
      page: 0
      pdf_page: 324
    - "no": 3
      title: PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS
      page: 0
      pdf_page: 328
    - "no": 4
      title: EXPONENTIAL MAPPING
      page: 0
      pdf_page: 329
    - "no": 5
      title: APPLICATION TO LINEAR REPRESENTATIONS
      page: 0
      pdf_page: 333
    - "no": 6
      title: NORMAL INTEGRAL SUBGROUPS
      page: 0
      pdf_page: 334
    - "no": 7
      title: PRIMITIVES OF DIFFERENTIAL FORMS WITH VALUES IN A LIE ALGEBRA
      page: 0
      pdf_page: 336
    - "no": 8
      title: PASSAGE FROM LAWS OF INFINITESIMAL OPERATION TO LAWS OF OPERATION
      page: 0
      pdf_page: 336
    - "no": 9
      title: EXPONENTIAL MAPPING IN THE LINEAR GROUP
      page: 0
      pdf_page: 338
    - "no": 10
      title: COMPLEXIFICATION OF A FINITE-DIMENSIONAL REAL LIE GROUP
      page: 0
      pdf_page: 340
statements: 71
exercises: 30
content_sha256: e4308513eafcf831627a9b6c2757f3a2479509353ab2123d2fedc562061949e7
translated_from: content/en/lie/III/06_s6_real_and_complex_lie_groups.md
source_content_sha256: 803604a811504c87fc4ceb1081eed8c02ca8766e1a5c157c84f5f0928a9452b5
translation_model: gpt-5-6-mini, gpt-5.4-mini, gpt-5-6, gpt-5-mini
translation_run: translate-vi-f0c4fab8
glossary_version: 34
glossary_terms_sha256: 267ec776a304f8303fdfdb5ebe87a442a48bcab775053d5e0fea9480d29243d5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. CÁC NHÓM LIE THỰC VÀ PHỨC

Trong đoạn này, giả sử K bằng $\mathbf{R}$ hoặc $\mathbf{C}$.

### 1. CHUYỂN TỪ CÁC CẤU XẠ ĐẠI SỐ LIE SANG CÁC CẤU XẠ NHÓM LIE

#### Bổ đề 1 {#lie-iii-s6-lem-1 .statement}

*Cho G là một nhóm tôpô liên thông đơn†, W là một lân cận mở liên thông đối xứng của e, H là một nhóm và f là một ánh xạ từ $W^3$ vào H sao cho*

$$
f(xyz) = f(x)f(y)f(z)
$$

*đối với x, y, z trong W. Tồn tại một cấu xạ $f'$ từ G vào H sao cho $f' \mid W = f \mid W$.*

Với $(g, h) \in G \times H$ và U là một lân cận mở của e trong W, ký hiệu $A(g, h, U)$ là tập hợp các $(gu, hf(u)) \in G \times H$ với $u \in U$. Khi đó $(g, h) \in A(g, h, U)$ và $A(g, h, U_1) \cap A(g, h, U_2) = A(g, h, U_1 \cap U_2)$. Cho $(s, t) \in A(g, h, U)$; khi đó $s = gu$ và $t = hf(u)$ với $u \in U$; tồn tại một lân cận mở $U'$ của e trong W sao cho $uU' \in U$; khi đó, với $u' \in U'$,

$$
(su', tf(u')) = (guu', hf(uu')) \in A(g, h, U)
$$

† Xem Chương XI của *Tôpô đại cương* (sắp xuất hiện). Trong chương này đã chứng minh rằng nếu $G_1, G_2$ là các nhóm tôpô liên thông, $\phi$ là một đồng cấu liên tục mở từ $G_1$ lên $G_2$ có hạt nhân rời rạc và $G_2$ liên thông đơn, thì $\phi$ là một phép đồng phôi. Mặt khác, nhắc lại rằng một không gian liên thông đơn là liên thông.

và do đó $A(s, t, U') \subset A(g, h, U)$. Suy ra rằng các $A(g, h, U)$ tạo thành cơ sở của một tôpô trên $G \times H$. Ta sẽ ký hiệu bởi $Y$ tập hợp $G \times H$ với tôpô này và ký hiệu bởi $p$ phép chiếu chính tắc của $Y$ lên $G$, là mở. Hạn chế của $p$ trên $A(g, h, U)$ là một phép đồng phôi từ $A(g, h, U)$ lên $gU$. Do đó $(Y, p)$ là một không gian phủ của $G$. Cho $Y_0$ là nhóm con của $Y$ sinh bởi $A(e, e, W)$ và cho $\mathfrak{B}$ là tập hợp các $A(e, e, U)$. Rõ ràng $\mathfrak{B}$ thỏa mãn các điều kiện (GV$_1'$) và (GV$_1''$) của *Tôpô đại cương*, Chương III, § 1, no. 2. Tập hợp $Y_0'$ gồm các $y \in Y_0$ sao cho các ánh xạ $z \mapsto yzy^{-1}$ và $z \mapsto y^{-1}zy$ từ $Y_0$ vào $Y_0$ là liên tục tại $(e, e)$ là một nhóm con của $Y_0$. Cho $w \in W$. Ánh xạ $w' \mapsto ww'w^{-1}$ từ $W$ vào $G$ là liên tục và do đó ánh xạ

$$
(w', f(w')) \mapsto (ww'w^{-1}, f(ww'w^{-1}))
$$

của $A(e, e, W)$ vào $Y$ liên tục tại $(e, e)$. Bây giờ $f(ww'w^{-1}) = f(w)f(w')f(w^{-1})$ và do đó $(ww'w^{-1}, f(ww'w^{-1})) = (w, f(w))(w', f(w'))(w, f(w))^{-1}$.

Vì $w^{-1} \in W$, ta thấy rằng $(w, f(w)) \in Y_0'$. Do đó, $A(e, e, W) \subset Y_0'$, suy ra $Y_0' = Y_0$. Nhóm $Y_0$, với cơ sở lọc $\mathfrak{B}$, vì vậy thỏa mãn điều kiện (GV$_{III}'$) của *Tôpô học tổng quát*, Chương III, § 1, no. 2. Vì

$$
(g, h).A(e, e, U) = A(g, h, U),
$$

$Y_0$ là một nhóm tôpô liên thông vì $A(e, e, W)$ liên thông. Khi đó $p(Y_0)$ là một nhóm con mở của $G$, do đó $p(Y_0) = G$ vì $G$ liên thông. Hạt nhân của $p \mid Y_0$ là rời rạc. Vì $G$ đơn liên, $p \mid Y_0$ là một đồng phôi của $Y_0$ lên $G$. Do đó $Y_0$ là đồ thị của một cấu xạ $f'$ của $G$ vào $H$. Với $g \in W$, $(g, f(g)) \in A(e, e, W) \subset Y_0$, do đó $f'(g) = f'(g)$.

#### Định lý 1 {#lie-iii-s6-thm-1 .statement}

*Cho $G$ và $H$ là các nhóm Lie và $h$ là một cấu xạ liên tục của $L(G)$ vào $L(H)$. Giả sử rằng $G$ đơn liên. Khi đó tồn tại duy nhất một cấu xạ nhóm Lie $\phi$ của $G$ vào $H$ sao cho $h = L(\phi)$.*

Sự tồn tại của $\phi$ theo từ Bổ đề 1 và § 4, no. 1, Định lý 1 (i). Tính duy nhất của $\phi$ theo từ § 4, no. 1, Định lý 1 (ii) và तथ्य rằng $G$ liên thông.

#### Hệ quả {#lie-iii-s6-n1-cor-1 .statement}

*Cho $G$ là một nhóm Lie đơn liên hữu hạn chiều. Tồn tại một biểu diễn tuyến tính giải tích hữu hạn chiều của $G$ có hạt nhân rời rạc.*

Có (Chương I, § 7, Định lý 2) một không gian vectơ hữu hạn chiều $E$ và một cấu xạ đơn ánh $h$ của $L(G)$ vào đại số Lie $\mathrm{End}(E)$. Theo Định lý 1, tồn tại một cấu xạ $\phi$ của $G$ vào $\mathbf{GL}(E)$ sao cho $L(\phi) = h$. Do đó $\phi$ là một phép ngâm và vì thế hạt nhân của nó là rời rạc.

#### Nhận xét {#lie-iii-s6-n1-rem-1 .statement}

(1) Có những nhóm Lie đơn liên hữu hạn chiều không có biểu diễn tuyến tính giải tích đơn ánh hữu hạn chiều nào (Bài tập 2).

(2) Có những nhóm Lie liên thông hữu hạn chiều $G$ sao cho mọi biểu diễn tuyến tính giải tích hữu hạn chiều của $G$ đều có hạt nhân không rời rạc (Bài tập 3 và 4).

### 2. CÁC NHÓM CON TÍCH PHÂN

#### Định nghĩa 1 {#lie-iii-s6-def-1 .statement}

Cho G là một nhóm Lie. Một nhóm con tích phân của G là một nhóm con H với một cấu trúc nhóm Lie liên thông sao cho đơn ánh chính tắc của H vào G là một phép ngâm.

Một nhóm con một tham số của G là một nhóm con tích phân 1 chiều của G.

Cho H là một nhóm con tích phân của G và i là đơn ánh chính tắc của H vào G. Khi đó L(i) xác định một đẳng cấu của L(H) lên một đại số con Lie của L(G) chấp nhận một phần bù tôpô. L(H) được đồng nhất với ảnh của nó qua L(i).

#### Ví dụ {#lie-iii-s6-n2-exa-1 .statement}

(1) Một nhóm con Lie liên thông của G là một nhóm con tích phân của G.

(2) Giả sử rằng G hữu hạn chiều. Cho H là một nhóm con của G; ta trang bị cho nó cấu trúc cảm sinh bởi cấu trúc nhóm Lie trên G (§ 4, no. 5, Định nghĩa 3). Khi đó thành phần liên thông đơn vị H_0 của nó là một nhóm con tích phân của G và đại số con tiếp tuyến với H tại e là L(H_0) (§ 4, no. 5, Mệnh đề 9 (ii)).

(3) Cho G là một nhóm Lie phức, H là một nhóm con tích phân của G và G_1 (tương ứng H_1) là nhóm Lie thực nền của G (tương ứng H). Khi đó H_1 là một nhóm con tích phân của G_1 và L(H_1) là đại số Lie thực nền của L(H).

#### Định lý 2 {#lie-iii-s6-thm-2 .statement}

Cho G là một nhóm Lie.

(i) Ánh xạ H ↦ L(H) là một song ánh từ tập hợp các nhóm con tích phân của G lên tập hợp các đại số con Lie của L(G) chấp nhận một phần bù tôpô.

(ii) Cho H là một nhóm con tích phân của G. Mọi mầm nhóm con Lie liên thông của G có đại số Lie L(H) là một đa tạp con mở của H và sinh ra H.

(a) Cho h là một đại số con Lie của L(G) chấp nhận một phần bù tôpô. Cho H_1 là một mầm nhóm con Lie của G sao cho L(H_1) = h (§ 4, Định lý 3). Có thể chọn H_1 sao cho nó liên thông. Cho H là nhóm con của G sinh bởi H_1. Có (§ 1, Hệ quả của Mệnh đề 22) một cấu trúc nhóm Lie trên H sao cho H_1 là một đa tạp con mở của H và đơn ánh chính tắc của H vào G là một phép ngâm. Vì H_1 liên thông, H liên thông và do đó là một nhóm con tích phân của G. Khi đó L(H) = L(H_1) = h. Điều này chứng tỏ rằng ánh xạ xét trong (i) là toàn ánh.

(b) Cho H là một nhóm con tích phân của G và N_1 là một mầm nhóm con Lie liên thông của G có đại số Lie L(H). Vì đơn ánh chính tắc của H vào G là một phép ngâm, tồn tại một mầm nhóm con mở H_1 của H đồng thời là một đa tạp con của G và vì thế là một mầm nhóm con Lie của G có đại số Lie L(H). Mặt khác, cho N là nhóm con của G sinh bởi N_1; theo phần (a) của chứng minh, nó có cấu trúc của một nhóm con tích phân của G sao cho N_1 là một đa tạp con mở của N. Theo § 4, Định lý 3, H_1 ∩ N_1 là mở trong H_1 và N_1. Vì thế nhóm con của G sinh bởi H_1 ∩ N_1 bằng, một mặt, H và mặt khác, N. Do đó các nhóm Lie H và N bằng nhau. Điều này chứng tỏ (ii) và cũng chứng tỏ rằng ánh xạ xét trong (i) là đơn ánh.

#### Nhận xét 1 {#lie-iii-s6-n2-rem-1 .statement}

Cho H là một nhóm con nguyên của G. Cho Y là phân lá trái của G liên kết với L(H). Nếu $g \in G$, cho $gH$ mang cấu trúc đa tạp suy ra từ cấu trúc trên H bởi $\gamma(g)$. Theo Đa tạp khả vi và giải tích, R, 9.3.2, đơn ánh chính tắc của $gH$ vào Y là một cấu xạ. Cấu xạ này là étale. Do đó các lá liên thông cực đại của Y là các lớp kề trái modulo H.

#### Mệnh đề 1 {#lie-iii-s6-prop-1 .statement}

*Cho G và M là các nhóm Lie, H là một nhóm con nguyên của G và $\phi$ là một cấu xạ từ M vào G sao cho $L(\phi)(L(M)) \subset L(H)$. Giả sử rằng M liên thông. Khi đó $\phi(M) \subset H$ và $\phi$, được xem như một ánh xạ từ M vào H, là một cấu xạ nhóm Lie.*

Trong ký hiệu của Nhận xét 1, $\phi$ là một cấu xạ từ M vào Y (*Đa tạp khả vi và giải tích*, R, 9.3.2) và do đó $\phi(M) \subset H$ vì M liên thông.

#### Hệ quả 1 {#lie-iii-s6-prop-1-cor-1 .statement}

*Cho G và H là các nhóm Lie, $\phi$ là một cấu xạ nhóm Lie từ G vào H, N là hạt nhân của $\phi$ và $h = L(\phi)$. Giả sử rằng G liên thông và H hữu hạn chiều.*
(i) *N là một nhóm con Lie của G và $L(N) = \mathrm{Ker}\ h$.*
(ii) *Cho H' là nhóm con nguyên của H với đại số Lie Im h. Khi đó $\phi(G) = H'$.*
(iii) *Ánh xạ từ G/N vào H' suy ra từ $\phi$ khi chuyển qua thương là một đẳng cấu nhóm Lie.*

(i) đã được chứng minh (\S 3, no. 8, Mệnh đề 28).

Cho $\psi$ là cấu xạ nhóm Lie từ G/N vào H suy ra từ $\phi$ khi chuyển qua thương; nó là một phép nhúng (\S 3, no. 8, Mệnh đề 28). Theo Mệnh đề 1, $\psi$ là một cấu xạ nhóm Lie từ G/N vào H'. Cấu xạ này là étale và do đó $\psi(G/N) = H'$ vì H' liên thông; điều này chứng minh (ii). Khi đó $\psi : G/N \to H'$ là song ánh và là một đẳng cấu nhóm Lie, điều này chứng minh (iii).

#### Hệ quả 2 {#lie-iii-s6-prop-1-cor-2 .statement}

*Cho G là một nhóm Lie và H_1 và H_2 là các nhóm con nguyên của G. Nếu $L(H_2) \subset L(H_1)$, thì H_2 là một nhóm con nguyên của H_1.*

Cho $i_1 : H_1 \to G, i_2 : H_2 \to G$ là các đơn ánh chính tắc. Khi đó
$$
L(i_2)(L(H_2)) = L(H_2) \subset L(H_1).
$$
Theo Mệnh đề 1, $i_2$ là một ánh xạ giải tích từ $H_2$ vào $H_1$ và thậm chí là một phép nhúng từ $H_2$ vào $H_1$ vì $L(i_2)$ là một đẳng cấu của $L(H_2)$ lên một đại số con của $L(H_1)$ nhận một phần bù tôpô.

#### Hệ quả 3 {#lie-iii-s6-prop-1-cor-3 .statement}

*Cho G là một nhóm Lie hữu hạn chiều và $(H_i)_{i \in I}$ là một họ các nhóm con Lie của G. Khi đó $H = \bigcap_{i \in I} H_i$ là một nhóm con Lie của G và*
$$
L(H) = \bigcap_{i \in I} L(H_i).
$$
Tồn tại một tập con hữu hạn J của I sao cho $\bigcap_{i \in J} L(H_i)$ bằng giao M của tất cả các L(H_i). Ta biết rằng H^* = \bigcap_{i \in J} H_i là một nhóm con Lie sao cho L(H^*) = M (\S 3, no. 8, Hệ quả 2 của Mệnh đề 29). Cho H_0 là thành phần đơn vị của H^*. Nó là một nhóm con Lie của G và L(H_0) = M. Theo Hệ quả 2, H_0 \subset H_i với mọi i và do đó H_0 \subset H \subset H^*, do đó có hệ quả.

#### Hệ quả 4 {#lie-iii-s6-prop-1-cor-4 .statement}

*Cho G là một nhóm Lie liên thông hữu hạn chiều. Các điều kiện sau là tương đương:*
(i) *G là đơn môđula* (Tích phân, Chương VII, \S 1, no. 3, Định nghĩa 3);
(ii) *det Ad g = 1 với mọi g \in G*;
(iii) *Tr ad a = 0 với mọi a \in L(G)*.

Ánh xạ g \mapsto det Ad g là một cấu xạ $\phi$ từ G vào K*. Theo \S 3, Mệnh đề 35 (no. 10) và 44 (no. 12), $L(\phi)a = Tr\ ad\ a$ với mọi $a \in L(G)$. Rõ ràng Im $L(\phi) = \{0\}$ hoặc K. Trong trường hợp thứ nhất (tương ứng thứ hai), Im $\phi = \{1\}$ (tương ứng Im $\phi = K^*$) theo Hệ quả 1 và do đó G là đơn môđula (tương ứng không đơn môđula) theo \S 3, no. 16, Hệ quả của Mệnh đề 55.

#### Mệnh đề 2 {#lie-iii-s6-prop-2 .statement}

*Cho G là một nhóm Lie hữu hạn chiều và H là một nhóm con nguyên của G. Các điều kiện sau là tương đương:*
(i) *H đóng*;
(ii) *tôpô trên H là tôpô cảm sinh bởi tôpô trên G*;
(iii) *H là một nhóm con Lie của G*.
(i) $\Rightarrow$ (iii): điều này suy ra từ \S 1, các Mệnh đề 2 (iv) (no. 1) và 14 (iii) (no. 7).
(iii) $\Rightarrow$ (ii): hiển nhiên.
(ii) $\Rightarrow$ (i): nếu tôpô trên H là tôpô cảm sinh bởi tôpô trên G, H đóng vì H đầy đủ (\S 1, no. 1, Mệnh đề 1).

#### Mệnh đề 3 {#lie-iii-s6-prop-3 .statement}

*Cho G là một nhóm Lie, H là một nhóm con nguyên của G, M là một đa tạp giải tích liên thông không rỗng, f là một ánh xạ từ M vào G và r \in N_K. Xét các điều kiện sau:*
(i) *f thuộc lớp C^r và f(M) \subset H*;
(ii) *f(M) \subset H và f, được xem như một ánh xạ từ M vào H, thuộc lớp C^r*;
(iii) *f thuộc lớp C^r, f(M) giao H và ảnh của T_m(M) được chứa trong f(m).L(H) với mọi m \in M*.

*(ii) $\Leftrightarrow$ (iii) $\Rightarrow$ (i). Nếu tôpô trên H nhận một cơ sở đếm được, thì ba điều kiện là tương đương.*
(ii) $\Rightarrow$ (i) và (ii) $\Rightarrow$ (iii): hiển nhiên.
(iii) $\Rightarrow$ (ii): giả sử điều kiện (iii) đúng. Theo *Đa tạp khả vi và giải tích*, R, 9.2.8, f là một cấu xạ lớp C^r từ M vào phân lá trái liên kết với L(H). Vì M liên thông, f(M) \subset H.

Nếu tôpô trên H nhận một cơ sở đếm được, điều kiện (i) kéo theo rằng f là một ánh xạ lớp C^r từ M vào H (*Đa tạp khả vi và giải tích*, R, 9.2.8); do đó (i) $\Rightarrow$ (ii).

#### Hệ quả 1 {#lie-iii-s6-prop-3-cor-1 .statement}

Cho G là một nhóm Lie hữu hạn chiều và H là một nhóm con nguyên của G. Khi đó đại số Lie tiếp xúc với H tại e (\S 4, no. 5, các Định nghĩa 2 và 3) là L(H) và cấu trúc nhóm Lie trên H là cấu trúc cảm sinh bởi cấu trúc trên G.

Vì H liên thông và hữu hạn chiều, tôpô của nó nhận một cơ sở đếm được.

#### Hệ quả 2 {#lie-iii-s6-prop-3-cor-2 .statement}

Cho G là một nhóm Lie và H_1 và H_2 là các nhóm con nguyên của G. Giả sử rằng tôpô trên H_1 nhận một cơ sở đếm được. Khi đó

$$
H_2 \subset H_1 \Leftrightarrow L(H_2) \subset L(H_1)
$$

và, nếu các điều kiện này thỏa mãn, H_2 là một nhóm con nguyên của H_1.

Khẳng định cuối cùng và kéo theo $L(H_2) \subset L(H_1) \Rightarrow H_2 \subset H_1$ suy ra từ Hệ quả 2 của Mệnh đề 1. Kéo theo đảo lại suy ra từ Mệnh đề 3.

#### Hệ quả 3 {#lie-iii-s6-prop-3-cor-3 .statement}

Cho G là một nhóm Lie và H_1 và H_2 là các nhóm con nguyên của G mà tôpô của chúng có một cơ sở đếm được. Nếu H_1 và H_2 có cùng tập nền, thì các cấu trúc nhóm Lie trên H_1 và H_2 là như nhau.

Điều này suy ra từ Hệ quả 2.

#### Nhận xét 2 {#lie-iii-s6-n2-rem-2 .statement}

Cho G là một nhóm Lie hữu hạn chiều. Cho H là một nhóm con của G. Ta sẽ nói, do sự lạm dụng ngôn ngữ, rằng H là một nhóm con nguyên của G nếu tồn tại một cấu trúc nhóm Lie S trên H sao cho H, cùng với S, là một nhóm con nguyên của G. Theo Hệ quả 3 của Mệnh đề 3, nếu S tồn tại, S là duy nhất.

#### Nhận xét 3 {#lie-iii-s6-n2-rem-3 .statement}

Cho V là một đa tạp lớp C^r. Cho M là một tập con của V và x và y là các phần tử của M. Xét tính chất sau:

P_{M, x, y}: tồn tại I, x_0, x_1, \ldots, x_n, f_1, \ldots, f_n sao cho: (a) I là một tập con mở liên thông của \mathbf{K}; (b) x_0, \ldots, x_n thuộc M, x_0 = x, x_n = y; (c) với 1 \leq i \leq n, f_i là một ánh xạ lớp C^r từ I vào V lấy các giá trị x_{i-1} và x_i và f_i(I) \subset M.

Ta sẽ nói rằng M là một tập con C^r-liên thông của V nếu, với mọi phần tử x, y của M, tính chất P_{M, x, y} đúng.

#### Mệnh đề 4 {#lie-iii-s6-prop-4 .statement}

Cho G là một nhóm Lie hữu hạn chiều và H là một nhóm con của G. Cho r \in \mathbf{N}_\mathbf{K}. Các điều kiện sau là tương đương:
(i) H là một nhóm con nguyên của G;
(ii) với cấu trúc nhóm Lie cảm sinh bởi cấu trúc trên G, H là liên thông;
(iii) H là C^r-liên thông.
(iii) \Rightarrow (i): hiển nhiên.
(i) \Rightarrow (iii): giả sử rằng H có một cấu trúc nhóm Lie sao cho H là một nhóm con nguyên của G. Sử dụng ký hiệu của Nhận xét 3, tập hợp các y \in H sao cho tính chất P_{H, e, y} đúng là một nhóm con mở của H. Vì H liên thông, nhóm con này bằng H và do đó điều kiện (iii) được thỏa mãn.

(iii) ⇒ (ii): giả sử rằng điều kiện (iii) được thỏa mãn và cho H cấu trúc cảm sinh bởi cấu trúc nhóm Lie trên G. Gọi h là đại số con tiếp xúc với H tại e. Thành phần liên thông đơn vị H_0 của H là một nhóm con nguyên của G sao cho L(H_0) = h. Ta chứng minh rằng H = H_0. Chỉ cần chứng minh điều sau: cho I là một tập con mở liên thông của K, f là một ánh xạ lớp C^r từ I vào G sao cho f(I) \subset H và λ và μ là hai điểm của I; nếu f(λ) ∈ H_0, thì f(μ) ∈ H_0. Nhưng, với mọi v ∈ I, (T_v f)(K) ⊂ f(v)h theo định nghĩa của h, do đó khẳng định của ta suy ra từ Mệnh đề 3.

#### Nhận xét 4 {#lie-iii-s6-n2-rem-4 .statement}

Nếu K = R, các nhóm con nguyên của G cũng có thể được đặc trưng là các nhóm con mà, với tôpô cảm sinh bởi tôpô trên G, là liên thông theo cung (§ 8, Bài tập 4). Tuy nhiên, các nhóm con có thể liên thông nhưng không nguyên (Đại số giao hoán, Chương VI, § 9, Bài tập 2).

#### Hệ quả {#lie-iii-s6-n2-cor-1 .statement}

Cho G là một nhóm Lie hữu hạn chiều và H_1 và H_2 là hai nhóm con nguyên của G. Nhóm con của G được sinh bởi H_1 và H_2 và nhóm con (H_1, H_2) của G là các nhóm con nguyên của G.

Nhóm con (G, G) của G không phải lúc nào cũng đóng (§ 9, Bài tập 6).

Nhắc lại (§ 3, no. 11, Hệ quả 5 của Mệnh đề 41) rằng nếu a là một đại số hữu hạn chiều, Aut(a) là một đại số con Lie của GL(a) và rằng L(Aut(a)) là đại số Lie của các đạo hàm của a.

#### Định nghĩa 2 {#lie-iii-s6-def-2 .statement}

Cho a là một đại số Lie hữu hạn chiều. Gọi Ad(a) hoặc Int(a) là nhóm con nguyên của Aut(a) có đại số Lie ad(a). Các phần tử của nhóm này được gọi là các tự đẳng cấu nội của a.

Bằng phép chuyển cấu trúc, ad(a) là bất biến dưới Aut(a) và do đó Int(a) là chuẩn trong Aut(a). Theo § 4, no. 4, Hệ quả 1 của Mệnh đề 8 và sự kiện rằng Int(a) là liên thông, các phần tử của Int(a) là các tích hữu hạn của các tự đẳng cấu dạng exp ad x trong đó x ∈ a. Nói chung, Int(a) không phải là một nhóm con Lie của Aut(a) (Bài tập 14).

### 3. CHUYỂN TỪ CÁC ĐẠI SỐ LIE SANG CÁC NHÓM LIE

#### Định lý 3 {#lie-iii-s6-thm-3 .statement}

(i) Nếu L là một đại số Lie hữu hạn chiều, tồn tại một nhóm Lie đơn liên G sao cho L(G) đẳng cấu với L.

(ii) Cho G_1 và G_2 là hai nhóm Lie liên thông, với G_1 đơn liên. Cho f là một đẳng cấu của L(G_1) lên L(G_2), φ là cấu xạ của G_1 vào G_2 sao cho L(φ) = f và N là hạt nhân của φ. Khi đó N là một nhóm con rời rạc của tâm của G_1 và cấu xạ của G_1/N vào G_2 dẫn xuất từ φ là một đẳng cấu nhóm Lie. Nếu G_2 đơn liên, φ là một đẳng cấu.

Cho L là một đại số Lie hữu hạn chiều. Tồn tại một không gian vectơ hữu hạn chiều E sao cho L có thể được đồng nhất với một đại số con Lie của End(E) (Chương I, § 7, Định lý 2). Cho H là nhóm con nguyên của GL(E) với

đại số Lie L. Cho $\hat{H}$ là phủ phổ quát của nó ($\S 1$, no. 9, *Nhận xét*). Khi đó $L(\hat{H})$ đẳng cấu với L, do đó (i).

Cho $G_1, G_2, f, \phi, N$ như trong (ii). Khi đó $\phi$ là étale, do đó $\phi(G_1)$ là một nhóm con mở của $G_2$ và vì thế $\phi(G_1) = G_2$. Mặt khác, N là rời rạc và do đó được chứa trong tâm của $G_1$ (*Integration*, Chương VII, $\S 3$, Bổ đề 4). Rõ ràng cấu xạ của $G_1/N$ lên $G_2$ dẫn xuất từ $\phi$ là một đẳng cấu nhóm Lie. Nếu $G_2$ đơn liên, mọi ánh xạ étale của $G_1$ lên $G_2$ là đơn ánh và do đó $N = \{e\}$.

#### Mệnh đề 5 {#lie-iii-s6-prop-5 .statement}

*Cho G là một nhóm Lie thực liên thông. Giả sử rằng $L(G)$ có một cấu trúc đại số Lie phức chuẩn hóa được $L'$ tương thích với cấu trúc đại số Lie thực chuẩn hóa được của nó. Tồn tại trên G duy nhất một cấu trúc nhóm Lie phức tương thích với cấu trúc nhóm Lie thực và với đại số Lie $L'$.*

Theo $\S 4$, no. 2, Hệ quả 2 của Định lý 2, chỉ cần chứng minh rằng cấu trúc của $L'$ là bất biến dưới Ad G. Cho $\phi$ là một ánh xạ mũ của G. Theo $\S 4$, no. 4, Hệ quả 3 (i) của Mệnh đề 8, tồn tại một lân cận V của 0 trong $L(G)$ sao cho cấu trúc của $L'$ là bất biến dưới Ad $\phi(V)$. Nhưng Ad $\phi(V)$ sinh ra G vì G liên thông.

Kết luận của Mệnh đề 5 không nhất thiết đúng nếu không giả sử G liên thông (Bài tập 7).

#### Mệnh đề 6 {#lie-iii-s6-prop-6 .statement}

*Cho G là một nhóm Lie phức liên thông. Nếu G compact, G giao hoán.*

Ánh xạ chỉnh hình $g \mapsto \mathrm{Ad}\,g$ của G vào $\mathcal{L}(L(G))$ là hằng (*Differentiable and Analytic Manifolds*, R, 3.3.7) và do đó $\mathrm{ad}\,a = 0$ với mọi $a \in L(G)$ ($\S 3$, no. 12, Mệnh đề 44). Suy ra G giao hoán ($\S 4$, Hệ quả 3 của Định lý 1).

### 4. ÁNH XẠ MŨ

#### Định lý 4 {#lie-iii-s6-thm-4 .statement}

*Cho G là một nhóm Lie. Tồn tại duy nhất một ánh xạ mũ của G được xác định trên $L(G)$.*

Tồn tại một lân cận mở lồi U của 0 trong $L(G)$ và một ánh xạ mũ của G được xác định trên U. Có thể giả sử, bằng cách chọn U đủ nhỏ, rằng
$$
\phi((\lambda + \lambda')a) = \phi(\lambda a)\phi(\lambda'a)
$$
với $a \in L(G)$, $\lambda, \lambda'$ trong K, $\lambda a, \lambda'a, (\lambda + \lambda')a$ trong U.

Cho $a \in L(G)$. Tồn tại một số nguyên $n > 0$ sao cho $\frac{1}{n} a \in U$. Nếu m là một số nguyên khác sao cho $\frac{1}{m} a \in U$, thì $\frac{1}{nm} a \in U$ và theo hệ thức (1) suy ra
$$
\phi\left(\frac{1}{n} a\right) = \left(\phi\left(\frac{1}{nm} a\right)\right)^m, \quad \phi\left(\frac{1}{m} a\right) = \left(\phi\left(\frac{1}{nm} a\right)\right)^n;
$$

do đó $\left( \phi \left( \frac{1}{n} a \right) \right)^n = \left( \phi \left( \frac{1}{m} a \right) \right)^m$. Tồn tại một mở rộng $\psi : L(G) \to G$ của $\phi$ sao cho $\psi(a) = \left( \phi \left( \frac{1}{n} a \right) \right)^n$ với $a \in L(G)$ và $n$ là một số nguyên $> 0$ sao cho $\frac{1}{n} a \in U$. Rõ ràng $\psi$ là giải tích và là một ánh xạ mũ của G. Nếu $\psi' : L(G) \to G$ là một ánh xạ mũ của G, thì $\psi$ và $\psi'$ trùng nhau trên một lân cận của 0 và do đó bằng nhau vì $L(G)$ liên thông.

Từ nay về sau, khi nói đến *ánh xạ mũ* của G, ta hiểu là ánh xạ được xét trong Định lý 4. Nó sẽ được ký hiệu bởi $\exp_G$ hoặc $\exp$ nếu không có nguy cơ nhầm lẫn.

#### Ví dụ {#lie-iii-s6-n4-exa-1 .statement}

Cho $A$ là một đại số chuẩn đầy đủ có đơn vị, kết hợp. Khi đó $\exp_{A^*}$ là ánh xạ mũ được định nghĩa trong Chương II, § 7, no. 3.

#### Mệnh đề 7 {#lie-iii-s6-prop-7 .statement}

*Cho G là một nhóm Lie và $a$ là một phần tử của $L(G)$. Ánh xạ $\lambda \mapsto \exp(\lambda a)$ của K vào G là cấu xạ duy nhất $\phi$ của nhóm Lie K vào G sao cho $(T_0 \phi)1 = a$.*

Các ánh xạ $(\lambda, \lambda') \mapsto \exp(\lambda a) \exp(\lambda' a)$ và $(\lambda, \lambda') \mapsto \exp(\lambda + \lambda') a$ từ $K \times K$ vào $G$ là giải tích và trùng nhau trên một lân cận của $(0, 0)$. Vì $K \times K$ liên thông, các ánh xạ này bằng nhau. Do đó $\phi : \lambda \mapsto \exp(\lambda a)$ là một cấu xạ nhóm Lie từ $K$ vào $G$. Ánh xạ tiếp xúc tại 0 của $\lambda \mapsto \lambda a$ là ánh xạ $\lambda \mapsto \lambda a$; và $T_e(\exp) = \mathrm{Id}_{L(G)}$; do đó $(T_0 \phi)1 = a$. Mệnh đề về tính duy nhất của mệnh đề suy ra từ Định lý 1.*

#### Mệnh đề 8 {#lie-iii-s6-prop-8 .statement}

*Cho $G$ là một nhóm Lie. Với mọi $x, y$ trong $L(G)$ và $n$ là một số nguyên,

$$
\exp(x + y) = \lim_{n \to + \infty} \left( \left( \exp \frac{1}{n} x \right) \left( \exp \frac{1}{n} y \right) \right)^n
$$

$$
\exp[x, y] = \lim_{n \to + \infty} \left( \left( \exp \frac{1}{n} x \right) \left( \exp \frac{1}{n} y \right) \left( \exp \frac{1}{n} x \right)^{-1} \left( \exp \frac{1}{n} y \right)^{-1} \right)^{n^2}.
$$

Theo Mệnh đề 7, điều này suy ra từ Mệnh đề 4 của § 4, no. 3, lấy $\lambda = \frac{1}{n}$.

#### Mệnh đề 9 {#lie-iii-s6-prop-9 .statement}

*Cho $G$ là một nhóm Lie phức và $G'$ là nhóm Lie thực cơ sở tương ứng. Khi đó $\exp_G = \exp_{G'}$.

Điều này suy ra từ Mệnh đề 5 của § 4, no. 3 và tính giải tích của $\exp_G$ và $\exp_{G'}$.

#### Mệnh đề 10 {#lie-iii-s6-prop-10 .statement}

*Cho $G$ và $H$ là các nhóm Lie và $\phi$ là một cấu xạ từ $G$ vào $H$.
(i) $\phi \circ \exp_G = \exp_H \circ L(\phi)$.
(ii) *Nếu $G$ là một nhóm con nguyên của $H$, thì $\exp_G = \exp_H | L(G)$.*

Ánh xạ mũ

Hai vế của đẳng thức (i) là các ánh xạ giải tích từ $L(G)$ vào $H$ trùng nhau trong một lân cận của 0 ($\S 4$, Mệnh đề 8, no. 4) và do đó bằng nhau. Mệnh đề (ii) là một trường hợp đặc biệt của (i).

#### Hệ quả 1 {#lie-iii-s6-prop-10-cor-1 .statement}

*Cho $G$ là một nhóm Lie, $G'$ là một nhóm con Lie của $G$ và $a \in L(G)$. Các điều kiện sau là tương đương*:
(i) $a \in L(G')$;
(ii) $\exp(\lambda a) \in G'$ với mọi $\lambda \in K$ và $|\lambda|$ đủ nhỏ;
(iii) $\exp(\lambda a) \in G$ với mọi $\lambda \in K$.
Lập luận cũng như trong $\S 4$, no. 4, Hệ quả 1 của Mệnh đề 8.

#### Hệ quả 2 {#lie-iii-s6-prop-10-cor-2 .statement}

*Cho $G$ là một nhóm Lie, $H$ là một nhóm con nguyên của $G$ và $a \in L(G)$. Xét các điều kiện sau*:
(i) $a \in L(H)$;
(ii) $\exp_G(\lambda a) \in H$ với mọi $\lambda \in K$.
*Khi đó (i) $\Rightarrow$ (ii). Nếu tôpô của $H$ có một cơ sở đếm được, thì (i) $\Leftrightarrow$ (ii)*.
Cho $i$ là đơn ánh chính tắc của $H$ vào $G$. Nếu $a \in L(H)$, thì
$$
\exp_G(\lambda a) = (\exp_G \circ L(i))(\lambda a) = (i \circ \exp_H)(\lambda a) \in H.
$$
Do đó (i) $\Rightarrow$ (ii). Đảo lại khi $H$ có một cơ sở đếm được suy ra từ Mệnh đề 3.

#### Hệ quả 3 {#lie-iii-s6-prop-10-cor-3 .statement}

*Cho $G$ là một nhóm Lie, $\rho$ là một biểu diễn tuyến tính giải tích của $G$, $x \in L(G)$ và $g \in G$.
(i) $\rho(\exp x) = \exp L(\rho)x$;
(ii) $\mathrm{Ad}(\exp x) = \exp \mathrm{ad}\, x$;
(iii) $g(\exp x)g^{-1} = \exp(\mathrm{Ad}\, g.x)$.
Lập luận giống như trong $\S 4$, no. 4, các Hệ quả 2 và 3 đối với Mệnh đề 8.*

#### Hệ quả 4 {#lie-iii-s6-prop-10-cor-4 .statement}

*Cho $G$ là một nhóm Lie liên thông hữu hạn chiều*.
(i) $\mathrm{Int}(L(G)) = \mathrm{Ad}(G)$.
(ii) *Cho $Z$ là tâm của $G$. Khi đó $Z$ là một nhóm con Lie của $G$ có đại số Lie là tâm của $L(G)$. Ánh xạ của $G/Z$ vào $\mathrm{Int}\, L(G)$ dẫn xuất từ $g \mapsto \mathrm{Ad}\, g$ khi chuyển qua thương là một đẳng cấu nhóm Lie*.
Mệnh đề (i) suy ra từ Hệ quả 3 (ii) và các nhận xét sau Định nghĩa 2. Cho $g \in G$. Để có $\mathrm{Ad}\, g = \mathrm{Id}_{L(G)}$, điều kiện cần và đủ là $\mathrm{Int}\, g$ trùng với $\mathrm{Id}_G$ trên một lân cận của $e$ ($\S 4$, no. 1, Định lý 1 (ii)) và do đó trên toàn bộ $G$; nói cách khác, điều kiện cần và đủ là $g \in Z$. Khi đó (ii) suy ra từ Hệ quả 1 đối với Mệnh đề 1.

#### Định nghĩa 3 {#lie-iii-s6-def-3 .statement}

*Cho $G$ là một nhóm Lie liên thông hữu hạn chiều. Nhóm Lie $\mathrm{Int}(L(G)) = \mathrm{Ad}(G)$ được gọi là nhóm phụ hợp của $G$*.

#### Mệnh đề 11 {#lie-iii-s6-prop-11 .statement}

*Cho $G$ là một nhóm Lie giao hoán liên thông*.
(i) *exp là một cấu xạ étale của nhóm Lie cộng tính $L(G)$ lên $G$*.

(ii) *Nếu K = \mathbf{R} và G là hữu hạn chiều, G đẳng cấu với một nhóm Lie có dạng $\mathbf{R}^p \times \mathbf{T}^q$ ($p, q$ là các số nguyên $\geqslant 0$).*

Theo công thức Hausdorff, $(\exp x)(\exp y) = \exp(x + y)$ với $x, y$ đủ gần 0 và do đó với mọi $x, y$ trong $L(G)$ nhờ tiếp tục giải tích. Vì vậy $\exp$ là một đồng cấu nhóm và là étale vì

$$
T_e(\exp) = \mathrm{Id}_{L(G)}.
$$

Do đó có (i). Mệnh đề (ii) suy ra từ (i) và *Tôpô đại cương*, Chương VII, § 1, Mệnh đề 9.

#### Mệnh đề 12 {#lie-iii-s6-prop-12 .statement}

*Cho G là một nhóm Lie và $L = L(G)$. Với mọi $x \in L$, cho $T_x(L)$ được đồng nhất với $L$, sao cho vi phân phải $\varpi(x)$ của $\exp$ tại $x$ là một ánh xạ tuyến tính từ $L$ vào $L$. Với mọi $x \in L$,

$$
\varpi(x) = \sum_{n \geqslant 0} \frac{1}{(n + 1)!} (\mathrm{ad}\ x)^n.
$$

Hai vế là các hàm giải tích của $x$ và bằng nhau đối với $x$ đủ gần 0 (§ 4, no. 3, Mệnh đề 6).

#### Nhận xét {#lie-iii-s6-n4-rem-1 .statement}

$\varpi(x) \cdot (\mathrm{ad}\ x) = \exp \mathrm{ad}\ x - 1$. Ta viết, do lạm dụng ký hiệu,

$$
\varpi(x) = \frac{\exp \mathrm{ad}\ x - 1}{\mathrm{ad}\ x}.
$$

#### Hệ quả {#lie-iii-s6-n4-cor-1 .statement}

*Cho G là một nhóm Lie phức và $x \in L(G)$. Ánh xạ tiếp tuyến tại $x$ của $\exp_G$ có hạt nhân $\bigoplus_{n \in \mathbf{Z} - \{0\}} \mathrm{Ker}(\mathrm{ad}\ x - 2i\pi n)$.

Hàm nguyên $z \mapsto \sum_{n \geqslant 0} \frac{1}{(n + 1)!} z^n$, bằng $\frac{e^z - 1}{z}$ với $z \neq 0$, nhận các điểm của $2\pi i \mathbf{Z} - \{0\}$ làm các không điểm, tất cả đều là các không điểm đơn. Hệ quả khi đó suy ra từ Mệnh đề 12 và bổ đề sau:

#### Bổ đề 2 {#lie-iii-s6-lem-2 .statement}

*Cho E là một không gian Banach phức, u là một phần tử của $\mathcal{L}(E)$, S là phổ của u trong $\mathcal{L}(E)$ (Spectral Theories, Chương I, § 1, no. 2) và f là một hàm phức chỉnh hình trên một lân cận mở $\Omega$ của S. Giả sử rằng f trong $\Omega$ chỉ có một số hữu hạn các không điểm phân biệt $z_1, \ldots, z_n$, với các bội $h_1, \ldots, h_n$. Khi đó $\mathrm{Ker}\ f(u)$ là tổng trực tiếp của các $\mathrm{Ker}(u - z_i)^{h_i}$ với $1 \leqslant i \leqslant n$.

(Để biết định nghĩa của $f(u)$, xem Spectral Theories, Chương I, § 4, no. 8.)

Tồn tại một hàm chỉnh hình g trên $\Omega$, khác không ở mọi nơi, sao cho $f(z) = (z - z_1)^{h_1} \ldots (z - z_n)^{h_n} g(z)$. Khi đó $g(u)g^{-1}(u) = g^{-1}(u)g(u) = 1$ và do đó $\mathrm{Ker}\ f(u) = \mathrm{Ker} \prod_{i=1}^n (u - z_i)^{h_i}$. Xét $\mathrm{Ker}\ f(u)$ như một môđun $\mathbf{C}[X]$ bằng phép toán ngoài $(h, x) \mapsto h(u)x$ với $h \in \mathbf{C}[X]$, $x \in \mathrm{Ker}\ f(u)$, ta thấy rằng Ker $f(u)$ là tổng trực tiếp của các $\mathrm{Ker}(u - z_i)^{n_i}$, sử dụng *Algebra*, Chương VII, § 2, no. 1, Mệnh đề 1.

### 5. ÁP DỤNG VÀO CÁC BIỂU DIỄN TUYẾN TÍNH

#### Mệnh đề 13 {#lie-iii-s6-prop-13 .statement}

*Cho $G$ là một nhóm Lie liên thông và $\varphi$ là một biểu diễn tuyến tính giải tích của $G$ trên một không gian vectơ đầy đủ khả chuẩn $E$. Cho $E_1, E_2$ là hai không gian vectơ con đóng của $E$ sao cho $E_2 \subset E_1$. Các điều kiện sau là tương đương:*

(i) $\varphi(g)x \equiv x \pmod{E_2}$ với mọi $g \in G$ và mọi $x \in E_1$;
(ii) $L(\varphi)(L(G))$ ánh xạ $E_1$ vào $E_2$.

$$
\begin{align*}
&\varphi(g)x \equiv x \quad (\text{mod } E_2) \quad \text{với mọi } g \in G \text{ và mọi } x \in E_1 \\
\Leftrightarrow &\varphi(\exp a)x \equiv x \quad (\text{mod } E_2) \quad \text{với mọi } a \in L(G) \text{ và mọi } x \in E_1 \\
\Leftrightarrow &(\exp L(\varphi)a)x \equiv x \quad (\text{mod } E_2) \quad \text{với mọi } a \in L(G) \text{ và mọi } x \in E_1.
\end{align*}
$$

Mặt khác, nếu $u \in \mathcal{L}(E)$, thì

$$
\begin{align*}
&\exp(\lambda u)x \equiv x \quad (\text{mod } E_2) \quad \text{với mọi } \lambda \in K \text{ và mọi } x \in E_1 \\
\Leftrightarrow &u(E_1) \subset E_2
\end{align*}
$$

do đó có mệnh đề.

#### Hệ quả 1 {#lie-iii-s6-prop-13-cor-1 .statement}

*Để $E_1$ ổn định dưới $\varphi$, điều kiện cần và đủ là $E_1$ ổn định dưới $L(\varphi)$.*

Chỉ cần lấy $E_1 = E_2$ trong Mệnh đề 13.

#### Hệ quả 2 {#lie-iii-s6-prop-13-cor-2 .statement}

*Giả sử rằng $\varphi$ là hữu hạn chiều. Để $\varphi$ là đơn (tương ứng nửa đơn), điều kiện cần và đủ là $L(\varphi)$ là đơn (tương ứng nửa đơn).*

Điều này suy ra từ Hệ quả 1.

#### Hệ quả 3 {#lie-iii-s6-prop-13-cor-3 .statement}

*Cho $x \in E$. Để $x$ bất biến dưới $\varphi(G)$, điều kiện cần và đủ là $x$ bị triệt tiêu bởi $L(\varphi)(L(G))$ (nghĩa là $x$ bất biến dưới $L(\varphi)$ theo nghĩa của Chương I, § 3, Định nghĩa 3).*

Chỉ cần lấy $E_1 = Kx$ và $E_2 = 0$ trong Mệnh đề 13.

#### Hệ quả 4 {#lie-iii-s6-prop-13-cor-4 .statement}

*Cho $\varphi'$ là một biểu diễn tuyến tính giải tích khác của $G$ trên một không gian khả chuẩn đầy đủ $E'$. Cho $T \in \mathcal{L}(E, E')$. Các điều kiện sau là tương đương:*

(i) $T\varphi(g) = \varphi'(g)T$ với mọi $g \in G$;
(ii) $TL(\varphi)(a) = L(\varphi')(a)T$ với mọi $a \in L(G)$.

Cho $\sigma$ là biểu diễn tuyến tính của $G$ trên $\mathcal{L}(E, E')$ dẫn xuất từ $\varphi$ và $\varphi'$ (§ 3, no. 11, Hệ quả 1 của Mệnh đề 41). Điều kiện (i) có nghĩa là $T$ bất biến dưới $\sigma(G)$. Điều kiện (ii) có nghĩa là $T$ bị triệt tiêu bởi $L(\sigma)(L(G))$. Khi đó chỉ cần áp dụng Hệ quả 3.

#### Hệ quả 5 {#lie-iii-s6-prop-13-cor-5 .statement}

Giả sử rằng $\rho$ và $\rho'$ là hữu hạn chiều. Để $\rho$ và $\rho'$ tương đương, điều kiện cần và đủ là $L(\rho)$ và $L(\rho')$ tương đương.

Đây là một trường hợp đặc biệt của Hệ quả 4.

#### Hệ quả 6 {#lie-iii-s6-prop-13-cor-6 .statement}

Giả sử rằng $G$ là hữu hạn chiều. Cho $t \in U(G)$. Để $L_t$ (tương ứng $R_t$) bất biến phải (tương ứng trái), điều kiện cần và đủ là $t$ thuộc tâm của $U(G)$.

Để $L_t$ (tương ứng $R_t$) bất biến phải (tương ứng trái), điều kiện cần và đủ là $\varepsilon_g * t = t * \varepsilon_g$ với mọi $g \in G$, nghĩa là $(\mathrm{Int}\, g)_* t = t$. Có một số nguyên $n$ sao cho $t \in U_n(G)$. Theo Hệ quả 3 và Mệnh đề 45 của § 3, no. 12, $(\mathrm{Int}\, g)_* t = t$ với mọi $g \in G$ khi và chỉ khi $[a, t] = 0$ với mọi $a \in L(G)$, nghĩa là khi và chỉ khi $t$ giao hoán với $U(G)$.

### 6. CÁC NHÓM CON NGUYÊN CHUẨN

#### Bổ đề 3 {#lie-iii-s6-lem-3 .statement}

Cho $G$ là một nhóm Lie, $H_1$ và $H_2$ là các nhóm con nguyên mà tôpô của chúng thừa nhận một cơ sở đếm được và $g \in G$. Khi đó

$$
g H_1 g^{-1} = H_2 \Leftrightarrow (\mathrm{Ad}\, g)(L(H_1)) = L(H_2).
$$

$\mathrm{Ad}\, g = T_e(\mathrm{Int}\, g)$. Do đó, bằng phép chuyển cấu trúc, $(\mathrm{Int}\, g)(H_1)$ có đại số Lie $(\mathrm{Ad}\, g)(L(H_1))$. Vì $H_1$ và $H_2$ có các cơ sở đếm được, nói rằng các tập hợp $H_2$ và $(\mathrm{Int}\, g)(H_1)$ bằng nhau cũng chính là nói rằng các nhóm con nguyên $H_2$ và $(\mathrm{Int}\, g)(H_1)$ bằng nhau (no. 2, Hệ quả 3 của Mệnh đề 3). Khi đó bổ đề suy ra từ Định lý 2 (i).

#### Mệnh đề 14 {#lie-iii-s6-prop-14 .statement}

Cho $G$ là một nhóm Lie và $H$ là một nhóm con nguyên mà tôpô của nó thừa nhận một cơ sở đếm được. Các điều kiện sau là tương đương:
(i) $H$ là chuẩn tắc trong $G$;
(ii) $L(H)$ là bất biến dưới $\mathrm{Ad}(G)$.
Nếu thêm rằng $G$ liên thông, các điều kiện này tương đương với điều kiện sau:
(iii) $L(H)$ là một iđêan của $L(G)$.
Nếu thêm rằng $G$ đơn liên và $L(H)$ có đối chiều hữu hạn trong $L(G)$, các điều kiện này kéo theo rằng $H$ là một nhóm con Lie của $G$ và rằng $G/H$ là đơn liên.

Sự tương đương (i) $\Leftrightarrow$ (ii) suy ra từ Bổ đề 3. Nếu thêm rằng $G$ liên thông, điều kiện (ii) tương đương với việc nói rằng $L(H)$ ổn định dưới $\mathrm{ad}\, L(G)$ (no. 5, Hệ quả 1 của Mệnh đề 13 và § 3, no. 12, Mệnh đề 44).

Giả sử rằng $G$ đơn liên và rằng $L(H)$ là một iđêan có đối chiều hữu hạn trong $L(G)$. Theo Định lý 3 của no. 3, tồn tại một nhóm Lie đơn liên $G'$ sao cho $L(G')$ đẳng cấu với $L(G)/L(H)$. Tồn tại một cấu xạ liên tục $f$ của $L(G)$ lên $L(G')$ có hạt nhân $L(H)$. Theo Định lý 1 của no. 1, tồn tại một cấu xạ $\phi$ của $G$ vào $G'$ sao cho $L(\phi) = f$. Cấu xạ này là một phép chìm và do đó hạt nhân của nó $N$ là một nhóm con Lie của $G$ sao cho $L(N) = \mathrm{Ker}\, f = L(H)$. Do đó $H$ là thành phần đơn vị của $N$ và vì thế là một nhóm con Lie của G. Gọi $\psi$ là cấu xạ của $G/H$ vào $G'$ dẫn xuất từ $\phi$ khi chuyển qua thương. Cấu xạ này là étale; vì G đơn liên, $\psi$ là một đẳng cấu của $G/H$ lên $G'$.

#### Hệ quả 1 {#lie-iii-s6-prop-14-cor-1 .statement}

*Cho G là một nhóm Lie đơn liên hữu hạn chiều. Cho m, h là các đại số Lie con của L(G) sao cho L(G) là tích nửa trực tiếp của m bởi h. Cho M, H là các đại số con nguyên tương ứng của G. Khi đó M và H là các nhóm con Lie đơn liên của G và, như một nhóm Lie, G là tích nửa trực tiếp của M bởi H.*

Theo Mệnh đề 14, H là một nhóm con Lie chuẩn tắc của G và nhóm Lie G/H là đơn liên thông. Gọi $\pi$ là cấu xạ chính tắc của G lên G/H. Tồn tại một cấu xạ $\theta$ của G/H vào M sao cho $L(\theta)$ là đẳng cấu chính tắc của $L(G)/L(H) = L(G)/h$ lên $L(M) = m$. Khi đó

$$
L(\pi \circ \theta) = L(\pi) \circ L(\theta) = \mathrm{Id}_{L(G/H)}
$$

và do đó $\pi \circ \theta = \mathrm{Id}_{G/H}$. Theo no. 1, Hệ quả 1 của Mệnh đề 1, $\theta(G/H) = M$. Theo Mệnh đề 8 của § 1, no. 4, M là một nhóm con Lie của G và nhóm Lie G là tích nửa trực tiếp của M bởi H.

#### Hệ quả 2 {#lie-iii-s6-prop-14-cor-2 .statement}

*Cho G là một nhóm Lie liên thông đơn liên thông hữu hạn chiều, H là một nhóm con Lie liên thông chuẩn tắc của G và $\pi$ là cấu xạ chính tắc của G lên G/H.

(i) Tồn tại một ánh xạ giải tích $\varphi$ của G/H vào G sao cho $\pi \circ \varphi = \mathrm{Id}_{G/H}$.

(ii) Với mọi ánh xạ $\varphi$ có các tính chất của (i), ánh xạ $(h, m) \mapsto h \varphi(m)$ của $H \times (G/H)$ vào G là một đẳng cấu của các đa tạp giải tích.

(iii) H và G/H là đơn liên thông.

Đặt $n = \dim G - \dim H$. Hệ quả là hiển nhiên đối với $n = 0$. Ta lập luận bằng quy nạp theo n.

Giả sử tồn tại một iđêan của L(G) chứa L(H) phân biệt với L(G) và L(H). Gọi H' là nhóm con Lie liên thông tương ứng của G. Gọi $\pi_1 : G \to G/H'$ và $\pi_2 : H' \to H'/H$ là các cấu xạ chính tắc. Theo giả thiết quy nạp, tồn tại các ánh xạ giải tích $\rho_1 : G/H' \to G$, $\rho_2 : H'/H \to H'$ sao cho $\pi_1 \circ \rho_1 = \mathrm{Id}_{G/H'}$, $\pi_2 \circ \rho_2 = \mathrm{Id}_{H'/H}$. Gọi

$$
\pi_3 : G/H \to G/H'
$$

là cấu xạ chính tắc. Nếu $x \in G/H$ và y là một đại diện của x trong G, y và $\rho_1(\pi_3(x))$ có cùng ảnh chính tắc modulo H' và do đó $x^{-1} \pi(\rho_1(\pi_3(x))) \in H'/H$. Đặt

$$
\rho(x) = \rho_1(\pi_3(x)) \rho_2(\pi(\rho_1(\pi_3(x))))^{-1} x \in G.
$$

Rõ ràng $\rho$ là một ánh xạ giải tích của G/H vào G và

$$
\pi(\rho(x)) = \pi(\rho_1(\pi_3(x))) \pi_2(\rho_2(\pi(\rho_1(\pi_3(x))))^{-1} x)) \\
= \pi(\rho_1(\pi_3(x))) \pi(\rho_1(\pi_3(x)))^{-1} x = x.
$$

Nếu bây giờ các iđêan duy nhất của L(G) chứa L(H) là L(G) và L(H), đại số Lie $L(G)/L(H)$ hoặc là 1-chiều hoặc là đơn. Trong cả hai trường hợp, $L(G)$ là tích nửa trực tiếp của một đại số con bởi $L(H)$; điều này là hiển nhiên trong trường hợp thứ nhất và trong trường hợp thứ hai điều này suy ra từ Chương I, § 6, Hệ quả 3 của Định lý 5. Mệnh đề (i) sau đó suy ra từ Hệ quả 1.

Mệnh đề (ii) là hiển nhiên. Mệnh đề (iii) suy ra từ (i) và (ii).

Các kết luận của Hệ quả 2 không còn nhất thiết đúng khi G là vô hạn chiều hoặc khi H không chuẩn tắc (Các Bài tập 8 và 15).

#### Hệ quả 3 {#lie-iii-s6-prop-14-cor-3 .statement}

*Cho G là một nhóm Lie liên thông hữu hạn chiều và H là một nhóm con Lie liên thông chuẩn tắc của G. Cấu xạ chính tắc của $\pi_1(H)$ vào $\pi_1(G)$ là đơn ánh.*

Gọi $G_1$ là phủ phổ quát của G và $\lambda$ là ánh xạ chính tắc của $G_1$ lên G. Đại số Lie của $G_1$ được đồng nhất với $L(G)$. Nhóm con Lie $\lambda^{-1}(H)$ của $G_1$ là chuẩn tắc trong $G_1$ và đại số Lie của nó là $L(H)$. Gọi $H_1$ là thành phần đơn vị của $\lambda^{-1}(H)$ và $\lambda_1 = \lambda | H_1$. Khi đó $L(H_1) = L(H)$ và do đó $\lambda_1$ là một cấu xạ étale của $H_1$ lên H. Mặt khác, $H_1$ là đơn liên thông (Hệ quả 2) và do đó được đồng nhất với phủ phổ quát của H. Khi đó, theo *Tôpô đại cương*, Chương XI, cấu xạ chính tắc của $\pi_1(H)$ vào $\pi_1(G)$ được đồng nhất với đơn ánh chính tắc của Ker $\lambda_1$ vào Ker $\lambda$.

### 7. NGHIỆM NGUYÊN CỦA CÁC DẠNG VI PHÂN VỚI GIÁ TRỊ TRONG MỘT ĐẠI SỐ LIE

#### Mệnh đề 15 {#lie-iii-s6-prop-15 .statement}

*Cho G là một nhóm Lie, M là một đa tạp lớp $C^r$ ($r \geq 2$) và $\alpha$ là một dạng vi phân lớp $C^{r-1}$ và bậc 1 trên M với giá trị trong L(G), sao cho $d\alpha + [\alpha]^2 = 0$. Giả sử rằng M liên thông đơn. Với mọi $x \in M$ và mọi $s \in G$, tồn tại duy nhất một ánh xạ f lớp $C^{r-1}$ từ M vào G sao cho $f(x) = s$ và $f^{-1} \cdot df = \alpha$.*

Tính duy nhất của f suy ra từ § 3, no. 17, Hệ quả 2 của Mệnh đề 59 và तथ्य M liên thông. Ta chứng minh sự tồn tại của f. Tồn tại một phủ mở $(U_i)_{i \in I}$ của M và, với mọi $i \in I$, một ánh xạ $g_i : U_i \to G$ lớp $C^{r-1}$ sao cho $g_i^{-1} \cdot dg = \alpha$ trên $U_i$ (§ 4, no. 6, Định lý 5). Theo § 3, no. 17, Hệ quả 2 của Mệnh đề 59, $g_i g_j^{-1}$ là hằng địa phương trên $U_i \cap U_j$. Đặt $g_i g_j^{-1} = g_{ij}$. Cho $G_d$ là nhóm G với tôpô rời rạc. Các $g_{ij} : U_i \cap U_j \to G_d$ là liên tục và $g_{ij} g_{jk} = g_{ik}$ trên $U_i \cap U_j \cap U_k$. Vì M liên thông đơn, tồn tại các ánh xạ liên tục $\lambda_i : U_i \to G_d$ sao cho $g_i g_j^{-1} = \lambda_i \lambda_j^{-1}$ trên $U_i \cap U_j$. Đặt g là ánh xạ của M vào G có hạn chế lên $U_i$ là $\lambda_i^{-1} g_i$ với mọi $i \in I$. Ánh xạ này có lớp $C^{r-1}$ và $g^{-1} dg = \alpha$. Ánh xạ f của M vào G được xác định bởi $f = s(g(x))^{-1} g$ thỏa các điều kiện $f^{-1} \cdot df = \alpha$ và $f(x) = s$.

### 8. CHUYỂN TỪ LUẬT CỦA PHÉP TOÁN VI PHÂN SANG LUẬT PHÉP TOÁN

#### Bổ đề 4 {#lie-iii-s6-lem-4 .statement}

*Cho G là một nhóm tôpô liên thông, X là một không gian tôpô Hausdorff và $f_1, f_2$ là các luật phép toán trái (tương ứng phải) của G trên X sao cho, với mọi $x \in X$, các ánh xạ* s \mapsto f_1(s, x),\ s \mapsto f_2(s, x) \text{ của } G \text{ vào } X \text{ là liên tục. Giả sử rằng tồn tại một lân cận } V \text{ của } \{e\} \times X \text{ trong } G \times X \text{ sao cho } f_1 \text{ và } f_2 \text{ trùng nhau trên } V. \text{ Khi đó } f_1 = f_2.

Với $x \in X$ và $A$ là tập hợp các $g \in G$ sao cho $f_1(g, x) = f_2(g, x)$. Khi đó $A$ là đóng trong G. Mặt khác, lấy $g \in A$; ta viết $y = f_1(g, x) = f_2(g, x)$. Tồn tại một lân cận $U$ của $e$ trong G sao cho $f_1(t, y) = f_2(t, y)$ với $t \in U$, nói cách khác sao cho $f_1(t', x) = f_2(t', x)$ với $t' \in Ug$ (tương ứng $gU$). Do đó $A$ là mở trong G và vì thế $A = G$.

#### Mệnh đề 16 {#lie-iii-s6-prop-16 .statement}

Cho G là một nhóm Lie liên thông, X là một đa tạp Hausdorff lớp $C^r$ và $f_1, f_2$ là các luật phép toán trái (tương ứng phải) lớp $C^r$ của G trên X. Nếu các luật của phép toán vi phân liên kết với $f_1$ và $f_2$ bằng nhau, thì $f_1 = f_2$.

Theo § 4, no. 7, Hệ quả của Mệnh đề 11, tồn tại một lân cận V của \{e\} \times X trong G \times X sao cho $f_1$ và $f_2$ trùng nhau trên V. Do đó $f_1 = f_2$ (Bổ đề 4).

#### Bổ đề 5 {#lie-iii-s6-lem-5 .statement}

Cho G là một nhóm tôpô liên thông đơn, X là một không gian tôpô Hausdorff, U là một lân cận mở của e trong G và $\psi$ là một ánh xạ liên tục từ $U \times X$ vào X sao cho $\psi(e, x) = x$ và $\psi(s, \psi(t, x)) = \psi(st, x)$ với mọi $x \in X$ và mọi s, t trong U sao cho $st \in U$. Cho W là một lân cận mở, liên thông, đối xứng của e sao cho $W^3 \subset U$. Tồn tại duy nhất một luật phép toán trái liên tục $\psi'$ của G trên X sao cho $\psi'$ và $\psi$ trùng nhau trên $W \times X$. Nếu G là một nhóm Lie và X là một đa tạp lớp $C^r$ và $\psi$ có lớp $C^r$, thì $\psi'$ có lớp $C^r$.

Tính duy nhất của $\psi$ suy ra từ Bổ đề 4. Cho P là nhóm phép hoán vị của X. Với $u \in W^3$, ánh xạ $x \mapsto \psi(u, x)$ là một phần tử f(u) của P và

$$ f(u_1u_2u_3) = f(u_1)f(u_2)f(u_3) $$

với $u_1, u_2, u_3$ trong W. Áp dụng Bổ đề 1 của no. 1, ta thu được một cấu xạ f' của G vào P mở rộng $f|W$. Đặt $\psi'(g, x) = f'(g)(x)$ với mọi $(g, x) \in G \times X$. Khi đó $\psi'$ là một luật phép toán trái của G trên X và trùng với $\psi$ trên $W \times X$. Vì $\psi'(g, \psi'(g', x)) = \psi'(gg', x)$ với $(g, g', x) \in G \times G \times X$, tính liên tục của $\psi$ trên $W \times X$ suy ra tính liên tục của $\psi'$ trên $gW \times X$ với mọi $g \in G$. Do đó $\psi'$ liên tục. Nếu $\psi'$ có lớp $C^r$, ta thấy tương tự rằng $\psi'$ có lớp $C^r$.

#### Định lý 5 {#lie-iii-s6-thm-5 .statement}

Cho G là một nhóm Lie liên thông đơn, X là một đa tạp compact lớp $C^r$ ($r \geq 2$) và $a \mapsto D_a$ là một luật của phép toán vi phân trái (tương ứng phải) lớp $C^{r-1}$ của L(G) trên X. Tồn tại duy nhất một luật phép toán trái (tương ứng phải) lớp $C^{r-1}$ của G trên X sao cho luật của phép toán vi phân liên kết là $a \mapsto D_a$.

Tính duy nhất suy ra từ Mệnh đề 16. Theo § 4, no. 7, Hệ quả 1 của Định lý 6, tồn tại một lân cận V của \{e\} \times X trong G \times X và một mảnh luật phép toán trái (tương ứng phải) lớp $C^{r-1}$ của G trên X, được xác định trên V, sao cho luật của phép toán vi phân liên kết là $a \mapsto D_a$. Vì X compact, có thể giả sử V có dạng $U \times X$, trong đó U là một lân cận mở của e trong G. Khi đó chỉ cần áp dụng Bổ đề 5.

### 9. ÁNH XẠ MŨ TRONG NHÓM TUYẾN TÍNH

#### Mệnh đề 17 {#lie-iii-s6-prop-17 .statement}

Cho $\Delta$ là tập các $z \in C$ sao cho $-\pi < J(z) < \pi$ và $\Delta'$ là tập các $z \in C$ không phải là số thực $\leq 0$. Cho E là một không gian chuẩn hoá đầy đủ trên C và A (tương ứng A') là tập các $x \in L(E)$ có phổ Sp(x) được chứa trong $\Delta$ (tương ứng $\Delta'$). Khi đó A (tương ứng A') là một tập con mở của L(E) (tương ứng GL(E)) và các ánh xạ exp: A → A' và log: A' → A (Spectral Theories, Chương I, § 4, no. 9) là các đẳng cấu nghịch đảo của các đa tạp giải tích.

Điều này suy ra từ Spectral Theories, Chương I, § 4, Mệnh đề 10 và no. 9.

#### Định lý 6 {#lie-iii-s6-thm-6 .statement}

Cho $E$ là một không gian Hilbert thực hoặc phức và $U$ là nhóm unita của $E$.

(i) Tập $H$ gồm các phần tử Hermit của $L(E)$ là, với cấu trúc không gian định chuẩn thực, một không gian con vectơ đóng của $L(E)$ thừa nhận một phần bù tôpô.

(ii) Tập $H'$ gồm các phần tử $\ge 0$ của $GL(E)$ là một đa tạp con giải tích thực của $GL(E)$.

(iii) Hạn chế của ánh xạ exp lên $H$ là một đẳng cấu của các đa tạp giải tích thực từ $H$ lên $H'$.

(iv) Ánh xạ $(h, u) \mapsto (\exp h)u$ từ $H \times U$ vào $GL(E)$ là một đẳng cấu của các đa tạp giải tích thực.

Nhắc lại rằng, nếu $x \in L(E)$, thì $x^*$ ký hiệu toán tử liên hợp của $x$. Gọi $H_1$ là tập các $x \in L(E)$ sao cho $x^* = -x$. Công thức $x = \frac{1}{2}(x + x^*) + \frac{1}{2}(x - x^*)$ chứng tỏ rằng, với cấu trúc không gian định chuẩn thực của nó, $L(E)$ là tổng trực tiếp tôpô của $H$ và $H_1$, do đó (i).

Giả sử $K = C$. Theo ký hiệu của Mệnh đề 17, $H'$ là tập các $h \in H \cap A'$ sao cho $Sp h \subset R^*_+$. Vì $\exp(R) = R^*_+$, nên (ii) và (iii) suy ra từ Mệnh đề 17 và Spectral Theories, Chương I, § 4, Mệnh đề 8 và § 6, no. 5. Ánh xạ $(h, u) \mapsto y = (exp h)u$ từ $H \times U$ vào $GL(E)$ là song ánh theo Spectral Theories, Chương I, § 6, Mệnh đề 15. Nó giải tích thực theo trên. Ánh xạ $y \mapsto h = \frac{1}{2} \log(y y^*)$ là giải tích thực và do đó ánh xạ $y \mapsto u = (exp h)^{-1}y$ cũng vậy. Do đó (iv).

Giả sử $K = R$. Gọi Ē là không gian Hilbert phức hoá của $E$ và $J$ là ánh xạ $\xi + i\eta \mapsto \xi - i\eta$ (với $\xi, \eta$ trong $E$) của Ē vào Ē. Gọi Ũ, Ũ', Ũ là các tập được định nghĩa cho Ē như $H$, $H'$, $U$ đối với $E$. Khi đó $H$ (tương ứng $H'$, $U$) được đồng nhất với tập các $x \in Ũ$ (tương ứng Ũ', Ũ) sao cho $JxJ^{-1} = x$. Các tính chất (ii), (iii) và (iv) khi đó suy ra dễ dàng từ (i) và các tính chất tương tự trong trường hợp phức.

#### Mệnh đề 18 {#lie-iii-s6-prop-18 .statement}

Cho $E$ là một không gian khả chuẩn đầy đủ trên $\mathbf{C}$, $v \in \mathcal{L}(E)$ và $g = exp v$. Giả sử $Sp(v)$ không chứa điểm nào trong các điểm $2i\pi n$ với $n \in \mathbf{Z} - \{0\}$. Khi đó, với mọi $x \in E$, các điều kiện $vx = 0$ và $gx = x$ là tương đương.

Điều này suy ra từ Bổ đề 2 của no. 4, áp dụng cho hàm $z \mapsto e^z - 1$.

#### Hệ quả 1 {#lie-iii-s6-prop-18-cor-1 .statement}

*Cho $E$ là một không gian khả chuẩn đầy đủ trên $\mathbf{C}$ và $F$ là không gian các ánh xạ n-tuyến tính liên tục từ $E^n$ vào $E$. Với mọi $v \in \mathcal{L}(E)$, ký hiệu $\sigma(v)$ là phần tử của $\mathcal{L}(F)$ được định nghĩa bởi*

$$
(\sigma(v)f)(x_1, \ldots, x_n) = v(f(x_1, \ldots, x_n)) - \sum_{i=1}^n f(x_1, \ldots, vx_i, \ldots, x_n).
$$

*Với mọi $g \in \mathbf{GL}(E)$, ký hiệu $\rho(g)$ là phần tử của $\mathbf{GL}(F)$ được định nghĩa bởi*

$$
(\rho(g)f)(x_1, \ldots, x_n) = g(f(g^{-1}x_1, \ldots, g^{-1}x_n)).
$$

*Cho $u \in \mathcal{L}(E)$ sao cho mọi $z \in \mathrm{Sp}\,u$ đều thỏa $|\mathcal{J}(z)| < \frac{2\pi}{n+1}$. Khi đó, với mọi $f \in F$, các điều kiện $\sigma(u)f = 0$ và $\rho(\exp u)f = f$ là tương đương.*

$\mathbf{L}(\rho) = \sigma$ (\S 3, no. 11, Hệ quả 1 của Mệnh đề 41) và do đó

$$
\rho(\exp u) = \exp \sigma(u)
$$

(no. 4, Hệ quả 3 của Mệnh đề 10). Theo Mệnh đề 18 thì chỉ cần chứng minh rằng $\mathrm{Sp}\,\sigma(u)$ không giao với $2i\pi(\mathbf{Z} - \{0\})$. Nhưng điều này suy ra từ bổ đề sau:

*Bổ đề 6. Nếu $v \in \mathcal{L}(E)$, thì $\mathrm{Sp}\,\sigma(v) \subset \mathrm{Sp}\,v + \mathrm{Sp}\,v + \cdots + \mathrm{Sp}\,v$, trong đó tổng gồm $n+1$ số hạng.*

Ta định nghĩa các phần tử $v_0, v_1, \ldots, v_n$ của $\mathcal{L}(F)$ bằng cách viết, với mọi $f \in F$,

$$
\begin{align*}
(v_0f)(x_1, \ldots, x_n) &= v(f(x_1, \ldots, x_n)) \\
(v_if)(x_1, \ldots, v_n) &= -f(x_1, \ldots, vx_i, \ldots, x_n) \quad \text{với } 1 \leq i \leq n.
\end{align*}
$$

Khi đó $\sigma(v) = \sum_{i=0}^n v_i$ và các $v_i$ giao hoán từng đôi một. Gọi $A$ là đại số con đóng sinh bởi các $v_i$ trong $\mathcal{L}(F)$; nó giao hoán (*Spectral Theories*, Chương I, \S 1, no. 4) và $\mathrm{Sp}_{\mathcal{L}(F)} v' = \mathrm{Sp}_A v' \subset \sum_{i=0}^n \mathrm{Sp}\,v_i$ (*Spectral Theories*, Chương I, \S 3, Mệnh đề 3 (ii)). Bây giờ, nếu $\lambda \in \mathbf{C}$ sao cho $v - \lambda$ khả nghịch, thì rõ ràng $v_i - \lambda_i$ khả nghịch và do đó $\mathrm{Sp}\,v_i \subset \mathrm{Sp}\,v$ với mọi $i$.

#### Hệ quả 2 {#lie-iii-s6-prop-18-cor-2 .statement}

*Cho $E$ là một đại số khả chuẩn đầy đủ trên $\mathbf{C}$ và $w \in \mathcal{L}(E)$. Giả sử mọi $z \in \mathrm{Sp}\,w$ đều thỏa $|\mathcal{J}(z)| < \frac{2\pi}{3}$. Các điều kiện sau là tương đương:*
(i) *$w$ là một đạo hàm của $E$;*
(ii) *exp w là một tự đẳng cấu của $E$.*
Điều này suy ra từ Hệ quả 1 với $n = 2$ và $f$ là phép nhân của $E$.

#### Mệnh đề 19 {#lie-iii-s6-prop-19 .statement}

Cho $E$ là một không gian khả chuẩn đầy đủ trên $\mathbf{C}$, $v \in \mathcal{L}(E)$ và $g = \exp v$. Giả sử mọi $z \in \mathrm{Sp}\, v$ đều thỏa $-\pi < \mathscr{J}(z) < \pi$. Khi đó, với mọi không gian con vectơ đóng $E'$ của $E$, các điều kiện $v(E') \subset E'$ và $g(E') = E'$ là tương đương.

Điều kiện $v(E') \subset E'$ suy ra $g(E') \subset E'$ và $g^{-1}(E') \subset E'$ và do đó $g(E') = E'$. Giả sử rằng $g(E') = E'$. Ta sử dụng ký hiệu $\Delta, \Delta'$ của Mệnh đề 17. Vì $\mathrm{Sp}\, v$ là một tập con compact của $\Delta$, tồn tại một hình chữ nhật compact $Q = (a, b) \times (a', b')$ sao cho $\mathrm{Sp}\, v \subset Q \subset \Delta$. Tập hợp $\Delta - Q$ là liên thông. Do đó $\mathrm{Sp}\, g \subset \exp Q \subset \Delta'$, tập hợp $\exp Q$ là compact và tập hợp $\Delta' - \exp Q$ là liên thông. Bao đóng của tập hợp sau chứa $]-\infty, 0]$ và do đó

$$
(\Delta' - \exp Q) \cup ]-\infty, 0] = \mathbf{C} - \exp Q
$$

là liên thông. Khi đó $\exp Q$ là lồi đa thức (*Spectral Theories*, Chương I, § 3, Hệ quả 2 của Mệnh đề 9) và do đó hàm $\log$, được xác định trên $\Delta'$, là giới hạn trong $\mathcal{O}(\exp Q)$ của các hàm đa thức (*Spectral Theories*, Chương I, § 4, Mệnh đề 3). Do đó $v = \log g$ là giới hạn trong $\mathcal{L}(E)$ của các phần tử có dạng $P(g)$, trong đó $P$ là một đa thức (*Spectral Theories*, Chương I, § 4, Định lý 3). Vì $P(g)(E') \subset E'$, suy ra rằng $v(E') \subset E'$.

#### Hệ quả {#lie-iii-s6-n9-cor-1 .statement}

Cho E là một không gian chuẩn đầy đủ trên $\mathbf{C}$, $v \in \mathcal{L}(E)$ và $g = \exp v$. Giả sử rằng mọi $z \in \mathrm{Sp}\, v$ thỏa mãn $-\frac{\pi}{2} < \mathscr{J}(z) < \frac{\pi}{2}$. Khi đó, với mọi không gian con vectơ đóng M của $\mathcal{L}(E)$, các điều kiện $gMg^{-1} = M$ và $[v, M] \subset M$ là tương đương.

Đặt $F = \mathcal{L}(E)$, $g'$ là ánh xạ $f \mapsto gfg^{-1}$ của F vào F và $v'$ là ánh xạ $f \mapsto [v, f]$ của F vào F. Khi đó $g' = \exp v'$ (no. 4, Hệ quả 3 của Mệnh đề 10 và § 3, no. 11, Hệ quả 1 của Mệnh đề 41). Bổ đề 6 chứng minh rằng $-\pi < \mathscr{J}(z) < \pi$ với mọi $z \in \mathrm{Sp}\, v'$. Khi đó chỉ cần áp dụng Mệnh đề 19.

### 10. PHỨC HÓA CỦA MỘT NHÓM LIE THỰC HỮU HẠN CHIỀU

#### Bổ đề 7 {#lie-iii-s6-lem-7 .statement}

Cho B là một nhóm, A là một nhóm con chuẩn tắc của B, C là nhóm $B/A$ và $i : A \to B$ và $p : B \to C$ là các cấu xạ chính tắc. Cho $A'$ là một nhóm và $f$ là một đồng cấu của A vào $A'$. Cho $\omega$ là một cấu xạ của B vào nhóm tự đẳng cấu của $A'$. Giả sử rằng, với $a \in A'$, $a' \in A'$, $b \in B$,

$$
f\left(bab^{-1}\right) = \omega(b)f(a), \quad \omega(a)a' = f(a)a'f(a)^{-1}.
$$

Cho $B''$ là tích nửa trực tiếp của B bởi $A'$ ứng với $\omega$ và q là cấu xạ chính tắc của $B''$ lên B.

(i) Ánh xạ $a \mapsto (f(a^{-1}), i(a))$ của A vào $B''$ là một cấu xạ của A lên một nhóm con chuẩn D của $B''$. Đặt $B' = B''/D$ và $i' : A' \to B'$, $g : B \to B'$ là các cấu xạ của $A'$ và B vào $B'$ dẫn xuất khi lấy thương từ các phép đơn ánh chính tắc của $A'$ và B vào $B''$.

(ii) Cấu xạ $p \circ q$ của $B''$ vào C xác định khi chuyển qua thương một cấu xạ của $B'$ vào C.

(iii) $i'$ là đơn ánh, $p'$ là toàn ánh, $\mathrm{Ker}(p') = \mathrm{Im}(i')$ và biểu đồ sau là giao hoán

$$
\begin{array}{ccc}
A & \xrightarrow{i} & B \xrightarrow{p} C \\
f \downarrow & & g \downarrow \mathrm{Id}_C \\
A' & \xrightarrow{i'} & B' \xrightarrow{p'} C.
\end{array}
$$

(iv) *Nếu* $b \in B$ và $a' \in A'$, thì
$$
g(b)i'(a')g(b)^{-1} = i'(\omega(b)a').
$$

(i) Với $a_1, a_2$ thuộc $A$, ta có, trong $B''$,
$$
(f(a_1^{-1}), i(a_1))(f(a_2^{-1}), i(a_2)) = (f(a_1^{-1})(\omega(a_1)f(a_2^{-1})), i(a_1)i(a_2))
= (f(a_1^{-1})f(a_1a_2^{-1}a_1^{-1}), i(a_1a_2))
= (f((a_1a_2)^{-1}, i(a_1a_2))
$$
và do đó $a \mapsto (f(a^{-1}), i(a))$ là một đồng cấu $h$ của $A$ vào $B''$. Cho $a \in A$, $a' \in A'$, $b \in B$; khi đó, trong $B''$,
$$
bh(a)b^{-1} = bf(a^{-1})ab^{-1} = (\omega(b)f(a^{-1}))(bab^{-1})
= f(ba^{-1}b^{-1})(bab^{-1}) = h(bab^{-1})
$$
$$
a'h(a){a'}^{-1} = a'f(a^{-1})a{a'}^{-1} = a'f(a^{-1})(\omega(a){a'}^{-1})a
= a'f(a^{-1})f(a){a'}^{-1}f(a^{-1})a = h(a)
$$
và do đó $h(A) = D$ là chuẩn trong $B''$.

(ii) Với $a \in A$,
$$
(p \circ q)(h(a)) = p(q(f(a^{-1})a)) = p(a) = e
$$
và do đó $p \circ q$ là tầm thường trên $D$.

(iii) Cho $a' \in A'$ sao cho $i'(a') = e$; khi đó $a' \in D$ và do đó tồn tại $a \in A$ sao cho $a' = f(a^{-1})a$; điều này suy ra $a = e$, do đó $a' = e$; vì vậy $i'$ là đơn ánh. Vì $p$ và $q$ là toàn ánh, $p'$ là toàn ánh.

#### Mệnh đề 20 {#lie-iii-s6-prop-20 .statement}

*Cho G là một nhóm Lie thực hữu hạn chiều.*

(i) *Tồn tại một nhóm Lie phức $\tilde{G}$ và một cấu xạ $\mathbf{R}$-giải tích $\gamma$ của G vào $\tilde{G}$ với các tính chất sau: với mọi nhóm Lie phức H và mọi cấu xạ $\mathbf{R}$-giải tích $\phi$ của G vào H, tồn tại duy nhất một cấu xạ $\mathbf{C}$-giải tích $\psi$ của $\tilde{G}$ vào H sao cho $\phi = \psi \circ \gamma$.*

(ii) *Nếu $(\tilde{G}', \gamma')$ có cùng các tính chất như $(\tilde{G}, \gamma)$, thì tồn tại duy nhất một đẳng cấu $\theta$ từ $\tilde{G}$ lên $\tilde{G}'$ sao cho $\theta \circ \gamma = \gamma'$.*

(iii) *Ánh xạ tuyến tính $\mathbf{C}$ của $L(G) \otimes \mathbf{C}$ vào $L(\tilde{G})$ mở rộng $L(\gamma)$ là toàn ánh; đặc biệt $\dim_{\mathbf{C}}(\tilde{G}) \leq \dim_{\mathbf{R}}(G)$.*

Mệnh đề (ii) là hiển nhiên. Ta chứng minh sự tồn tại của một cặp có thứ tự $(\tilde{G}, \gamma)$ với các tính chất (i) và (iii).

(a) Trước hết giả sử G liên thông. Ký hiệu $g = L(G)$, $g_C = g \otimes_{\mathbf{R}} \mathbf{C}$ là phức hóa của g, S (tương ứng, S') là nhóm Lie thực (tương ứng, phức) đơn liên với đại số Lie g (tương ứng, $g_C$), và $\sigma$ là cấu xạ $\mathbf{R}$-giải tích duy nhất của S vào S' sao cho $L(\sigma)$ là đơn ánh chính tắc của g vào $g_C$. Ký hiệu $\pi$ là cấu xạ $\mathbf{R}$-giải tích duy nhất của S lên G sao cho $L(\pi) = \mathrm{Id}_{L(G)}$ và $F = Ker \pi$.

$$
\begin{array}{ccc}
S & \xrightarrow{\sigma} & S' \\
\downarrow \pi & & \downarrow \lambda \\
G & \xrightarrow{\gamma} & G \\
& \searrow \phi & \swarrow \psi \\
& & H
\end{array}
$$

Ta ký hiệu $r$ là cấu xạ chính tắc của $B''$ lên $B'$. Cho $a' \in A'$, $b \in B$ và $b' = r(a'b)$. Nếu $b' \in \mathrm{Im}(i')$, thì tồn tại $a'_1 \in A'$ sao cho $b' = r(a'_1)$; khi đó tồn tại $a \in A$ sao cho $a'b = a'_1f(a^{-1})a$, do đó $b = a \in A$ và
$$
p'(b') = p(q(a'b)) = p(b) = e;
$$
vì vậy, $\mathrm{Im}(i') \subset \mathrm{Ker}(p')$. Ta giữ nguyên ký hiệu $a', b, b'$ nhưng giả sử rằng $b' \in \mathrm{Ker}(p')$; khi đó $e = p'(b') = p(q(a'b)) = p(b)$ và suy ra $b \in A$, do đó
$$
b' = r(a'f(b)f(b^{-1})b) = r(a'f(b)) \in \mathrm{Im}(i');
$$
vì vậy $\mathrm{Ker}(p') \subset \mathrm{Im}(i')$.

Nếu $a \in A$, thì
$$
i'(f(a)) = r(f(a)) = r(f(a)f(a^{-1})a) = r(a) = g(i(a)).
$$

Nếu $b \in B$, thì
$$
p'(g(b)) = p(b)
$$
và do đó biểu đồ (4) giao hoán.

(iv) Cho $b \in B, a' \in A'$. Khi đó
$$
g(b)i'(a')g(b)^{-1} = r(b)r(a')r(b)^{-1} = r(ba'b^{-1})
= r(\omega(b)a') = i'(\omega(b)a').
$$

Với mọi nhóm Lie phức H và mọi cấu xạ giải tích $\mathbf{R}$ $\phi$ của G vào H, $L(\phi): g \to L(H)$ có một mở rộng $\mathbf{C}$-tuyến tính duy nhất tới $g_C$ và sự mở rộng này có dạng $L(\phi^*)$, trong đó $\phi^*$ là một cấu xạ giải tích $\mathbf{C}$ của S' vào H. Khi đó
$$
L(\phi \circ \pi) = L(\phi) \circ L(\pi) = L(\phi) = L(\phi^*) \circ L(\sigma) = L(\phi^* \circ \sigma)
$$
và do đó $\phi \circ \pi = \phi^* \circ \sigma$. Vì thế $\phi^*(\sigma(F)) = \phi(\pi(F)) = \{e\}$, suy ra
$$
\sigma(F) \subset \mathrm{Ker}\, \phi^*.
$$
Cho P là giao của các $\mathrm{Ker}\, \phi^*$ khi $\phi$ biến thiên. Đây là một nhóm con Lie chuẩn tắc của S' (no. 2, Hệ quả 3 của Mệnh đề 1). Cho $\tilde{G} = S'/P$ và λ: S' → Ġ là cấu xạ chính tắc. Khi đó σ(F) ⊂ P và do đó tồn tại một và chỉ một cấu xạ giải tích $\mathbf{R}$ γ của G vào Ġ sao cho γ ∘ π = λ ∘ σ. Nếu ψ: Ġ → H ký hiệu cấu xạ dẫn xuất từ φ* khi chuyển qua thương, thì

$$(φ ∘ γ) ∘ π = ψ ∘ (λ ∘ σ) = φ^* ∘ σ = φ ∘ π$$

suy ra ψ ∘ γ = φ. Rõ ràng L(ψ), và do đó ψ, được xác định duy nhất bởi đẳng thức ψ ∘ γ = φ. Vậy ta đã chứng minh rằng cặp có thứ tự (Ḡ, γ) có các tính chất (i) và (iii).

(b) Bây giờ ta xét trường hợp tổng quát. Cho F là thành phần liên thông của đơn vị của G, M = G/F và i: F → G, p: G → M là các cấu xạ chính tắc. Ta áp dụng phần (a) của chứng minh cho F. Ta thu được một cặp có thứ tự (Ḟ, δ). Với mọi g ∈ G, Int g|F = ω'(g) là một tự đẳng cấu của F. Nhờ tính chất phổ quát của Ḟ, tồn tại một và chỉ một tự đẳng cấu ω(g) của nhóm Lie phức Ḟ sao cho δ ∘ ω'(g) = ω(g) ∘ δ. Rõ ràng ω là một cấu xạ của G vào Aut(Ḣ). Nếu g ∈ G và f ∈ F, thì

$$δ(gf g^{-1}) = (\delta ∘ ω'(g))(f) = (\omega(g) ∘ \delta)(f) = \omega(g)(\delta(f)).$$

Nếu f ∈ F, thì δ ∘ (Int_F f) = (Int_Ḟ δ(f)) ∘ δ và Int_Ḟ δ(f) là một tự đẳng cấu của nhóm Lie phức Ḟ; do đó Int_Ḟ δ(f) = ω(f).

Do đó có thể áp dụng Bổ đề 7, cho ta một biểu đồ

$$
\begin{array}{ccc}
F & \xrightarrow{i} & G & \xrightarrow{p} & M \\
\downarrow{\delta} & & \downarrow{\gamma} & & \downarrow{\mathrm{Id}} \\
Ḟ & \xrightarrow{\tilde{i}} & Ġ & \xrightarrow{\tilde{p}} & M.
\end{array}
$$

Cho Ḟ được đồng nhất với một nhóm con Lie chuẩn tắc của Ġ nhờ ī. Nhóm Ġ được sinh bởi Ḟ và γ(G); do đó các tự đẳng cấu của Ḟ được xác định bởi các phần tử của Ġ là các tự đẳng cấu của cấu trúc nhóm Lie phức. Theo § 1, no. 9, Mệnh đề 18, tồn tại một và chỉ một cấu trúc nhóm Lie phức trên Ġ sao cho Ḟ là một nhóm con Lie mở của Ġ. Từ nay về sau Ġ sẽ mang cấu trúc này. Vì δ là giải tích $\mathbf{R}$, nên γ là giải tích $\mathbf{R}$.

Cặp có thứ tự (Ḡ, γ) có tính chất (iii) của mệnh đề. Ta chứng minh rằng nó có tính chất (i). Cho H là một nhóm Lie phức và ψ là một cấu xạ giải tích $\mathbf{R}$ của G vào H. Tồn tại một cấu xạ giải tích $\mathbf{C}$ η của Ḟ vào H sao cho η ∘ δ = φ|F. Cho g ∈ G. Các ánh xạ

$$f \mapsto \eta(\omega(g)f), \quad f \mapsto \phi(g)\eta(f)\phi(g)^{-1}$$

của Ḟ vào H là các cấu xạ giải tích $\mathbf{C}$; chúng trùng nhau trên δ(F), vì nếu f' ∈ F, thì

$$\phi(g)\eta(\delta(f'))\phi(g)^{-1} = \phi(g)\phi(f')\phi(g)^{-1} = \phi(gf'g^{-1})$$
$$= \eta(\delta(gf'g^{-1})) = \eta(\omega(g)\delta(f'));$$

do đó $\eta(\omega(g)f) = \phi(g)\eta(f)\phi(g)^{-1}$ với mọi $g \in G$ và mọi $f \in \tilde{F}$. Nếu $G'$ ký hiệu tích nửa trực tiếp của $G$ bởi $\tilde{F}$ tương ứng với $\omega$, thì khi đó tồn tại một cấu xạ $\zeta$ của nhóm $G'$ vào $H$ trùng với $\phi$ trên $G$ và với $\eta$ trên $\tilde{F}$. Với $f \in F$,
$$
\zeta(\delta(f^{-1})f) = \eta(\delta(f^{-1}))\phi(f) = \phi(f^{-1})\phi(f) = e.
$$
Do đó, khi chuyển qua thương, ζ xác định một cấu xạ ψ của $\tilde{G}$ vào H. Khi đó $\psi \circ \gamma = \phi$ và $\psi \circ \tilde{i} = \eta$; đẳng thức sau suy ra rằng ψ là giải tích $\mathbf{C}$.

Cuối cùng, cho $\psi'$ là một cấu xạ giải tích $\mathbf{C}$ của $\tilde{G}$ vào H sao cho $\phi = \phi' \circ \gamma$. Khi đó
$$
\psi' \circ \tilde{i} \circ \delta = \psi' \circ \gamma \circ i = \phi \circ i = \psi \circ \tilde{i} \circ \delta
$$
và do đó $\psi' \circ \tilde{i} = \psi \circ \tilde{i}$. Vì $\tilde{G}$ được sinh bởi $\tilde{i}(\tilde{F})$ và $\gamma(G)$, nên $\psi' = \psi$.

#### Định nghĩa 4 {#lie-iii-s6-def-4 .statement}

$(G, \gamma)$, hay đơn giản là $\tilde{G}$, được gọi là phức hóa phổ quát của $G$.

#### Nhận xét {#lie-iii-s6-n10-rem-1 .statement}

(1) Cho $(\tilde{G}, \gamma)$ là phức hóa phổ quát của $G$. Cho $G_0$ (resp. $\tilde{G}_0$) là thành phần liên thông chứa đơn vị của $G$ (resp. $\tilde{G}$). Theo chứng minh của Mệnh đề 20, $(\tilde{G}_0, \gamma|G_0)$ là phức hóa phổ quát của $G_0$ và cấu xạ hợp thành
$$
G \to \tilde{G} \to \tilde{G}/\tilde{G}_0
$$
khi chuyển qua thương xác định một đẳng cấu từ $G/G_0$ lên $\tilde{G}/\tilde{G}_0$.

(2) Giả sử rằng $G$ là liên thông đơn liên. Cho $g = L(G)$, $g_C$ là phức hóa của $g$, $S'$ là nhóm Lie phức đơn liên với đại số Lie $g_C$ và $\sigma$ là cấu xạ từ $G$ vào $S'$ sao cho $L(\sigma)$ là đơn ánh chính tắc của $g$ vào $g_C$. Ta lại dùng ký hiệu trong chứng minh của Mệnh đề 20, phần (a). Nếu $H = S'$ và $\phi = \sigma$, thì $\phi^* = \mathrm{Id}_{S'}$. Do đó $(S', \sigma)$ là phức hóa phổ quát của $G$. Chú ý rằng $\sigma$ nói chung không đơn ánh (Bài tập 16); tuy nhiên *hạt nhân của nó là rời rạc* vì $L(\sigma)$ là đơn ánh. Mặt khác, hãy để $\theta$ là phép đối hợp của $g_C$ được xác định bởi $g$ và hãy để $\eta$ là tự đẳng cấu tương ứng của nhóm Lie thực nền của $S'$; hãy để ${S'}^\eta$ là tập hợp các điểm của $S'$ bất biến dưới $\eta$; đó là một nhóm con Lie thực của $S'$ với đại số Lie $g$ (\S 3, no. 8, Hệ quả 1 của Mệnh đề 29). Theo no. 1, Hệ quả 1 của Mệnh đề 1, $\sigma(G)$ là một nhóm con nguyên thực của $S'$ với đại số Lie $g$ và do đó $\sigma(G)$ *là thành phần liên thông chứa đơn vị của* ${S'}^\eta$; nói riêng $\sigma(G)$ là một nhóm con Lie thực của $S'$.

### Bài tập {#lie-iii-s6-exercises}

Xem [bài tập cho § 6](exercises/s6/).
