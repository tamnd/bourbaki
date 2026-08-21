---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 13
section_title: Absolutely Semisimple Algebras
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.229-A VIII.249
pdf_pages: 0246-0266
extraction: native
subsections:
    - "no": 1
      title: Absolutely Semisimple Modules
      page: 229
      pdf_page: 246
    - "no": 2
      title: Algebras over Separably Closed Fields
      page: 230
      pdf_page: 247
    - "no": 3
      title: Absolutely Semisimple Algebras
      page: 231
      pdf_page: 248
    - "no": 4
      title: Characterization of Absolutely Semisimple Modules
      page: 235
      pdf_page: 252
    - "no": 5
      title: Derivations on Semisimple Algebras
      page: 236
      pdf_page: 253
    - "no": 6
      title: Cohomology of Algebras
      page: 239
      pdf_page: 256
    - "no": 7
      title: Cohomology of Absolutely Semisimple Algebras
      page: 241
      pdf_page: 258
    - "no": 8
      title: The Splitting of Artinian Algebras
      page: 243
      pdf_page: 260
statements: 33
exercises: 12
content_sha256: 30d5171000c7efa2cfb7a1d39040a22b486044a886a38f980db9edf184fe40c3
translated_from: content/en/alg/VIII/13_s13_absolutely_semisimple_algebras.md
source_content_sha256: 4c6d4e2ca3db7df962893b91ae11c5bedee5ed2c441f889a9973255356caf0c0
translation_model: gpt-5.4
translation_run: translate-vi-74c08a00
glossary_version: 34
glossary_terms_sha256: f2ea25018ffab9f6a17873f325d39a4f13246b1f740fa199c38f9aa492448a54
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 13. ĐẠI SỐ NỬA ĐƠN TUYỆT ĐỐI

### 1. Môđun Nửa Đơn Tuyệt Đối

#### Định nghĩa 1 {#alg-viii-s13-def-1 .statement tag=00F9}

Cho K là một trường giao hoán và A là một đại số trên K. Ta gọi một A-môđun M là nửa đơn tuyệt đối nếu $A_{(L)}$-môđun $M_{(L)}$ là nửa đơn đối với mọi mở rộng L của K.

Mọi môđun nửa đơn tuyệt đối đều là nửa đơn. Ngược lại, nếu trường K là hoàn hảo, thì mọi A-môđun nửa đơn hữu hạn chiều trên K đều là nửa đơn tuyệt đối (VIII, p. 222, Hệ quả 1, a)) vì mọi mở rộng của một trường hoàn hảo đều tách được (V, §7, No. 1, p. 36, Mệnh đề 2).

#### Mệnh đề 1 {#alg-viii-s13-prop-1 .statement tag=00FA}

Cho K là một trường giao hoán và A là một đại số trên K.

a) Mọi tổng trực tiếp của các A-môđun nửa đơn tuyệt đối đều là một A-môđun nửa đơn tuyệt đối. Mọi môđun con và môđun thương của một môđun nửa đơn tuyệt đối đều là nửa đơn tuyệt đối.

b) Cho M là một A-môđun và L là một mở rộng của trường K. A-môđun M là nửa đơn tuyệt đối khi và chỉ khi $A_{(L)}$-môđun $M_{(L)}$ là nửa đơn tuyệt đối.

Mệnh đề a) suy ra từ mệnh đề tương tự đối với các môđun nửa đơn (VIII, p. 56, Hệ quả 1 và 3).

Giả sử A-môđun M là nửa đơn tuyệt đối, và cho $L'$ là một mở rộng của L. Với cấu trúc $A_{(L')}$-môđun, $L'\otimes_LM_{(L)}$ đẳng cấu với $M_{(L')}$ (II, §5, No. 1, p. 273, Mệnh đề 2); do đó nó là một môđun nửa đơn. Điều này chứng tỏ rằng $M_{(L)}$ là nửa đơn tuyệt đối.

Ngược lại, giả sử rằng $M_{(L)}$ là nửa đơn tuyệt đối. Cho $L'$ là một mở rộng của K. Tồn tại một mở rộng hợp thành $(\Omega , u, v)$ của L và $L'$ (V, §2, No. 4, p. 13, Hệ quả); ta đồng nhất L và $L'$ với các mở rộng con của Ω. $A_{(\Omega )}$-môđun $M_{(\Omega )}$ đẳng cấu với $(M_{(L)})_{(\Omega )}$; do đó nó là nửa đơn. Nhưng $M_{(\Omega )}$ cũng đẳng cấu với $(M_{(L')})_{(\Omega )}$, và Mệnh đề 8, a) của VIII, p. 222 suy ra rằng $M_{(L')}$ là nửa đơn. Vậy M là nửa đơn tuyệt đối.

#### Mệnh đề 2 {#alg-viii-s13-prop-2 .statement tag=00FB}

Cho K là một trường giao hoán, A là một đại số trên K, và M là một A-môđun hữu hạn chiều trên K. Các tính chất sau là tương đương:

(i) A-môđun M là nửa đơn tuyệt đối.

(ii) Tồn tại một mở rộng P của K là một trường hoàn hảo sao cho $A_{(P)}$-môđun $M_{(P)}$ là nửa đơn.

(iii) A-môđun M là nửa đơn, và tâm của hoán tập của nó là một đại số étale trên trường K.

Rõ ràng là (i) kéo theo (ii). Giả sử rằng (ii) đúng; khi đó $A_{(P)}$-môđun $M_{(P)}$ là nửa đơn tuyệt đối theo Hệ quả 1, a) của VIII, p. 222. Theo Mệnh đề 1, b), khi đó M là nửa đơn tuyệt đối. Vậy (ii) kéo theo (i).

Giả sử rằng M là nửa đơn. Gọi Z là tâm của hoán tập của M; đó là một đại số giao hoán bậc hữu hạn trên trường K. Nếu L là một mở rộng của K, thì theo Mệnh đề 8, b) của VIII, p. 222, $A_{(L)}$-môđun $M_{(L)}$ là nửa đơn khi và chỉ khi vành $Z_{(L)}$ là rút gọn. Do đó tính tương đương của (i) và (iii) suy ra từ Định lý 4 của V, §6, No. 7, p. 34.

### 2. Các đại số trên các trường đóng tách được

#### Bổ đề 1 {#alg-viii-s13-lem-1 .statement tag=00FC}

Cho D là một trường và Z là tâm của nó. Ký hiệu đặc số mũ của Z là $p$. Giả sử rằng với mọi phần tử $a$ của D, tồn tại một số nguyên $m\geqslant 0$ sao cho $a^{p^m}$ thuộc về Z. Khi đó trường D là giao hoán.

Nếu $p= 1$, thì D = Z. Vì vậy ta giả sử $p >1$.

Hãy đưa ra một chứng minh phản chứng và giả sử rằng D không giao hoán. Cho $a$ là một phần tử của D- Z và $q$ là một lũy thừa của $p$ sao cho $a^q$ thuộc Z. Ký hiệu ánh xạ đồng nhất trên D bởi I và tự đẳng cấu trong $x\mapsto axa^{-1}$ từ D đến D liên kết với $a$ bởi $\sigma$; ta có $\sigma^q= I$ vì $a^q$ thuộc Z. Ta có $\sigma -I\not= 0$ vì $a$ không thuộc Z, và ta có $(\sigma -I)^q=\sigma^q-I = 0$ vì Z có đặc số $p$. Cho $f$ là số tự nhiên lớn nhất sao cho $(\sigma -I)^f\not= 0$; ta có $f\geqslant 1$. Chọn một phần tử $c$ của D sao cho $(\sigma -I)^f(c)\not= 0$, và đặt

$$
x= (\sigma -I)^{f-1}(c),y= (\sigma -I)(x) = (\sigma -I)^f(c)
$$

Theo phép dựng, ta có $y\not= 0$ và $\sigma (y) =y$; nếu đặt $z=y^{-1}x$, thì suy ra rằng

$$
\sigma (z) =\sigma (y)^{-1}\sigma (x) =y^{-1}(y+x) = 1 +z
$$

và do đó $\sigma (z^{p^j}) = 1 +z^{p^j}$ với mọi số tự nhiên $j$. Chọn một số nguyên $m\geqslant 0$ sao cho $z^{p^m}$ thuộc tâm Z của D; ta có

$$
z^{p^m}=az^{p^m}a^{-1}=\sigma (z^{p^m}) = 1 +z^{p^m}
$$

Mâu thuẫn này chứng minh Bổ đề 1.

#### Mệnh đề 3 {#alg-viii-s13-prop-3 .statement tag=00FD}

Cho K là một trường đóng khả ly (V, §7, No. 8, p. 45, Định nghĩa 4), và cho D là một đại số bậc hữu hạn trên K mà là một trường. Khi đó D là giao hoán.

Ký hiệu đặc số mũ của K là $p$. Cho $a$ là một phần tử của D. Vành $K[a]$ là một mở rộng đại số của K (V, §3, No. 1, p. 17, Hệ quả 1). Vì trường K đóng khả ly, suy ra từ V, §7, No. 7, p. 44, Mệnh đề 13 rằng đại số $K[a]$ là một mở rộng căn-$p$ của K. Do đó tồn tại một số nguyên $m\geqslant 0$ sao cho $a^{p^m}$ thuộc K. Theo Bổ đề 1, vì thế trường D là giao hoán.

#### Hệ quả {#alg-viii-s13-n2-cor-1 .statement tag=00FE}

Cho K là một trường đóng khả ly và A là một đại số nửa đơn bậc hữu hạn trên K. Khi đó tồn tại một số nguyên $r\geqslant 0$, các số nguyên dương ngặt $n_1, . . . , n_r$, và các mở rộng $K_1, . . . ,K_r$ của K bậc hữu hạn sao cho A đẳng cấu với đại số $\prod_{i=1}^r\mathbf{M}_{n_i}(K_i)$.

Theo định lý cấu trúc của các đại số nửa đơn (VIII, p. 135, Định lý 1), A đẳng cấu với một đại số $\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$, trong đó $r$ là một số nguyên $\geqslant 0,n_1, . . . , n_r$ là các số nguyên dương ngặt, và $D_1, . . . ,D_r$ là các K-đại số có bậc hữu hạn và là các trường. Vì trường K đóng tách được, mỗi trường $D_i$ là giao hoán theo Mệnh đề 3; hệ quả được suy ra.

### 3. Đại số nửa đơn tuyệt đối

#### Định nghĩa 2 {#alg-viii-s13-def-2 .statement tag=00FF}

Cho K là một trường giao hoán. Ta nói rằng một K-đại số A là nửa đơn tuyệt đối nếu vành $A_{(L)}$ là nửa đơn với mọi mở rộng L của K.

Mọi đại số nửa đơn tuyệt đối đều nửa đơn. K-đại số A là nửa đơn tuyệt đối khi và chỉ khi A-môđun $A_s$ là nửa đơn tuyệt đối. Theo Mệnh đề 1 của VIII, p. 229, do đó ta thu được kết quả sau: nếu L là một mở rộng của K, thì L-đại số $A_{(L)}$ là nửa đơn tuyệt đối khi và chỉ khi K-đại số A là nửa đơn tuyệt đối.

#### Định lý 1 {#alg-viii-s13-thm-1 .statement tag=00FG}

Cho K là một trường giao hoán và A là một K-đại số. Các tính chất sau là tương đương:

(i) K-đại số A là nửa đơn tuyệt đối.

(ii) Đại số A có bậc hữu hạn trên K, và tồn tại một mở rộng P của K là một trường hoàn hảo sao cho P-đại số $A_{(P)}$ là nửa đơn.

(iii) K-đại số A là nửa đơn và có bậc hữu hạn trên K, và tâm của nó là một K-đại số étale.

(iv) Tồn tại một họ hữu hạn $(n_i,D_i)_{i\in I}$, trong đó $n_i$ là một số nguyên dương ngặt và $D_i$ là một đại số trên K có bậc hữu hạn, đồng thời là một trường, sao cho tâm $Z_i$ của $D_i$ là một mở rộng tách được của K với mọi $i\in I$ và A đẳng cấu với tích của các vành ma trận $\mathbf{M}_{n_i}(D_i)$.

(v) Tồn tại một mở rộng L của K và một họ hữu hạn các số nguyên $(n_i)_{i\in I}$ sao cho đại số trên L $A_{(L)}$ đẳng cấu với đại số $\prod_{i\in I}\mathbf{M}_{n_i}(L)$.

(vi) Tồn tại một mở rộng Galois L của K có bậc hữu hạn và một họ hữu hạn các số nguyên $(n_i)$ sao cho $A_{(L)}$ đẳng cấu với tích của các đại số ma trận $\mathbf{M}_{n_i}(L)$.

Trước hết ta chứng minh các hệ quả (v) $\Rightarrow$ (iv) $\Rightarrow$ (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i). Ký hiệu tâm của A là Z.

Nếu tính chất (v) được thỏa mãn, thì L-đại số $A_{(L)}$ là nửa đơn và có bậc hữu hạn trên L, và tâm của nó (đẳng cấu với $Z_{(L)}$, III, p. 41, Hệ quả) đẳng cấu với $L^r$ với một số nguyên nào đó $r\geqslant 0$. Theo Hệ quả 2, a) của VIII, p. 222, đại số A là nửa đơn và có bậc hữu hạn trên K. Do đó nó đẳng cấu với một tích hữu hạn các vành $\prod_{i\in I}\mathbf{M}_{n_i}(D_i)$ với $n_i\geqslant 1$ với mọi $i\in I$, trong đó trường $D_i$ là một đại số có bậc hữu hạn trên K. Tâm $Z_i$ của $D_i$ là một trường giao hoán là một mở rộng của K, và Z đẳng cấu với $\prod_{i\in I}Z_i$. Vì vậy, $Z_{(L)}$ một mặt đẳng cấu với $\prod_{i\in I}(Z_i)_{(L)}$ và mặt khác đẳng cấu với $L^r$. Nói cách khác, đại số $\prod_{i\in I}Z_i$ là étale trên trường K (V, §6, No. 3, p. 28, Định nghĩa 1), và mỗi một trong các mở rộng $Z_i$ đều tách được trên K (V, §6, No. 4, p. 31, Hệ quả, và V, §7, No. 1, p. 42). Vậy (v) suy ra (iv).

Nếu tính chất (iv) đúng, thì hiển nhiên A là một đại số nửa đơn và có bậc hữu hạn trên K. Tâm Z của nó đẳng cấu với tích $\prod_{i\in I}Z_i$ của các mở rộng tách được của K có bậc hữu hạn; do đó nó là một đại số étale (loc. cit.). Vậy (iv) suy ra (iii).

Các kéo theo (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i) suy ra từ Mệnh đề 2 của VIII, p. 230 áp dụng cho A-môđun $A_s$.

#### Bổ đề 2 {#alg-viii-s13-lem-2 .statement tag=00FH}

Cho L là một trường đóng đại số và D là một trường chứa L trong tâm của nó. Nếu D phân biệt với L, thì tồn tại một mở rộng $L'$ của L sao cho vành $D\otimes_LL'$ không là Artin trái.

Cho $x$ là một phần tử của D - L; vì L đóng đại số, mở rộng $L'= L(x)$ của L không là đại số và $x$ siêu việt trên L. Khi đó vành $B = L'\otimes_LL'$ là một miền nguyên theo Mệnh đề 5 của V, §17, No. 4, p. 141.

Phần tử $y=x\otimes 1-1\otimes x$ của B khác không, nhưng nếu $\varphi$ là đồng cấu từ B vào $L'$ gửi $\xi \otimes \eta$ tới $\xi \eta$, thì ta có $\varphi (y) = 0$, do đó $y$ không khả nghịch trong B. Ta xem vành $C = D\otimes_LL'$ như một môđun phải trên vành con B của nó; đó là một môđun tự do vì D là một không gian vectơ phải trên trường con $L'$ của nó. Vì $y$ là một phần tử khác không và không khả nghịch của miền nguyên B, nên phép nhân phải bởi $y$ trong C là một ánh xạ $R_y$ đơn ánh nhưng không song ánh. Bây giờ, $R_y$ là một tự đồng cấu của C-môđun trái $C_s$; do đó (VIII, p. 28, Hệ quả 1), vành C không phải là Artin trái.

Bây giờ ta chứng minh rằng (i) suy ra (v). Đây là một hệ quả của bổ đề sau.

#### Bổ đề 3 {#alg-viii-s13-lem-3 .statement tag=00FI}

Cho A là một đại số trên K nửa đơn tuyệt đối và L là một mở rộng đóng đại số của K. Khi đó đại số $A_{(L)}$ đẳng cấu với một tích của hữu hạn đại số ma trận trên L.

L-đại số $A_{(L)}$ là nửa đơn; do đó nó đẳng cấu với một tích của hữu hạn nhiều đại số dạng $\mathbf{M}_{n_i}(D_i)$, trong đó $D_i$ là một trường chứa L trong tâm của nó và $n_i$ là một số nguyên $\geqslant 1$ (VIII, p. 137, Nhận xét 1).

Cho $L'$ là một mở rộng của L. Vì K-đại số A là nửa đơn tuyệt đối, vành $A_{(L')}$ là nửa đơn và do đó là Artin trái. Mặt khác, vành $A_{(L')}$ đẳng cấu với $L'\otimes_LA_{(L)}$, nên đẳng cấu với $\prod_{i\in I}\mathbf{M}_{n_i}(L'\otimes_LD_i)$; theo Mệnh đề 5 của VIII, p. 7, do đó mỗi vành $\mathbf{M}_{n_i}(L'\otimes_LD_i)$ đều là Artin trái.

Cho $n\geqslant 1$ là một số nguyên và B là một vành. Cho $(\mathfrak{b}_r)_{r\geqslant 0}$ là một dãy giảm các iđêan trái của B; ký hiệu bởi $\mathfrak{c}_r$ tập hợp các ma trận vuông cấp $n$ với các phần tử thuộc $\mathfrak{b}_r$. Khi đó $(\mathfrak{c}_r)_{r\geqslant 0}$ là một dãy giảm các iđêan trái của $\mathbf{M}_n(B)$. Đặc biệt, nếu vành $\mathbf{M}_n(B)$ là Artin trái, thì B cũng vậy.

Theo điều trên, với mọi $i\in I$ và mọi mở rộng $L'$ của L, vành $D_i\otimes_LL'$ là Artin trái. Theo Bổ đề 2, ta có $D_i= L$ với mọi $i\in I$, điều này suy ra Bổ đề 3.

Chúng ta sẽ dùng bổ đề sau để chứng minh suy ra (i)$\Rightarrow$(vi).

#### Bổ đề 4 {#alg-viii-s13-lem-4 .statement tag=00FJ}

Cho A và B là các đại số trên trường K có các tập sinh hữu hạn, và cho $K'$ là một mở rộng của K. Nếu các $K'$-đại số $A_{(K')}$ và $B_{(K')}$ đẳng cấu, thì tồn tại một mở rộng con L của $K'$, sinh hữu hạn trên K, sao cho các L-đại số $A_{(L)}$ và $B_{(L)}$ đẳng cấu.

Cho $(e_i)_{i\in I}$ và $(f_j)_{j\in J}$ lần lượt là các tập sinh hữu hạn của các đại số A và B. Cho $u$ là một đẳng cấu từ $A_{(K')}$ lên $B_{(K')}$ và $v$ là đẳng cấu nghịch đảo; tồn tại một mở rộng con L của $K'$, sinh hữu hạn trên K, sao cho ta có $u(1\otimes e_i)\in B_{(L)}$ với mọi $i\in I$ và $v(1\otimes f_j)\in A_{(L)}$ với mọi $j\in J$. Do đó, $u$ biến $A_{(L)}$ vào $B_{(L)}$, và $v$ biến $B_{(L)}$ vào $A_{(L)}$. Các ánh xạ cảm sinh $u': A_{(L)}\rightarrow B_{(L)}$ và $v': B_{(L)}\rightarrow A_{(L)}$ là các đồng cấu vành; chúng là những song ánh nghịch đảo của nhau.

Hãy hoàn tất chứng minh của hàm ý (i)$\Rightarrow$(vi). Gọi $K'$ là một bao đóng tách được của K (V, §7, No. 8, p. 45). Khi đó $A_{(K')}$ là một đại số nửa đơn tuyệt đối trên $K'$. Theo hàm ý (i)$\Rightarrow$(iv), đại số trên $K'$ $A_{(K')}$ đẳng cấu với một tích $\mathbf{M}_{n_1}(D_1)\times \cdots \times \mathbf{M}_{n_r}(D_r)$, trong đó $D_i$ là một đại số trên $K'$ có bậc hữu hạn, là một trường mà tâm $Z_i$ của nó là một mở rộng tách được của $K'$. Vì $K'$ là đóng tách được, ta có $Z_i= K'$. Theo Mệnh đề 3 của VIII, p. 231, trường $D_i$ là giao hoán. Do đó suy ra $D_i= K'$. Ta ký hiệu đại số trên K $\mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$ là B. Theo trên, các đại số trên $K'$ $A_{(K')}$ và $B_{(K')}$ là đẳng cấu. Mọi mở rộng con của $K'$ sinh hữu hạn trên K đều tách được và có bậc hữu hạn trên K, do đó được chứa trong một mở rộng con L của $K'$ vừa là Galois vừa có bậc hữu hạn trên K (V, §10, No. 1, p. 57, Mệnh đề 2). Vì vậy hàm ý suy ra từ Bổ đề 4.

Hàm ý (vi)$\Rightarrow$(v) là ngay lập tức.

#### Hệ quả 1 {#alg-viii-s13-lem-4-cor-1 .statement tag=00FK}

Cho K là một trường giao hoán, và cho $A_1$ và $A_2$ là các K-đại số. Giả sử rằng $A_1$ là nửa đơn tuyệt đối.

a) Nếu $A_2$ là nửa đơn, thì $A_1\otimes_KA_2$ cũng vậy.

b) Nếu $A_2$ là nửa đơn tuyệt đối, thì $A_1\otimes_KA_2$ cũng vậy.

Ký hiệu tâm của $A_1$ là $Z_1$ và tâm của $A_2$ là $Z_2$. Tâm Z của $A_1\otimes_KA_2$ bằng $Z_1\otimes_KZ_2$ theo hệ quả của III, §4, No. 4, p. 468. Giả sử rằng $A_2$ là nửa đơn; khi đó $Z_2$ là một đại số rút gọn (VIII, p. 137, Mệnh đề 2 và 3). Theo Định lý 1, $Z_1$ là một đại số trên K étale và do đó tách được. Theo Mệnh đề 5 của V, §15, No. 2, p. 120, vành $Z = Z_1\otimes_KZ_2$ là rút gọn; vì $A_1$ có bậc hữu hạn trên K (Định lý 1), suy ra từ Mệnh đề 7 của VIII, p. 221 rằng vành $A_1\otimes_KA_2$ là nửa đơn.

Bây giờ giả sử rằng $A_2$ là nửa đơn tuyệt đối. Cho L là một mở rộng của K. Khi đó đại số $A_{1(L)}$ là nửa đơn tuyệt đối, và đại số $A_{2(L)}$ là nửa đơn. Do đó, theo a), đại số $A_1\otimes_KA_{2(L)}$ là nửa đơn.

#### Hệ quả 2 {#alg-viii-s13-lem-4-cor-2 .statement tag=00FL}

Cho K là một trường đóng tách được, và cho A là một đại số trên K nửa đơn tuyệt đối. Khi đó tồn tại một số nguyên $r\geqslant 0$ và các số nguyên dương ngặt $n_1, . . . , n_r$ sao cho đại số A đẳng cấu với đại số $\prod_{i=1}^r\mathbf{M}_{n_i}(K)$.

Theo Định lý 1, A đẳng cấu với một đại số dạng $\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$ với một số nguyên $r\geqslant 0$, các số nguyên $n_1, . . . , n_r$, và các đại số trên K bậc hữu hạn $D_1, . . . ,D_r$ là các trường và có tâm là những mở rộng tách được của K, do đó bằng K. Theo Mệnh đề 3 của VIII, p. 231, ta có $D_i= K$ với $i\in [1, r]$.

#### Ví dụ {#alg-viii-s13-n3-exa-1 .statement tag=00FM}

Một đại số giao hoán trên K là nửa đơn tuyệt đối khi và chỉ khi nó là étale: điều này suy ra từ định nghĩa (V, §6, No. 3, p. 28, Định nghĩa 1) và từ tính tương đương của các tính chất (i) và (v) của Định lý 1.

### 4. Đặc trưng hóa các môđun nửa đơn tuyệt đối

#### Mệnh đề 4 {#alg-viii-s13-prop-4 .statement tag=00FN}

Cho K là một trường giao hoán và A là một đại số trên K.

a) Cho M là một A-môđun nửa đơn. A-môđun M là nửa đơn tuyệt đối khi và chỉ khi mọi môđun đơn thuộc giá của M đều như vậy.

b) Cho S là một A-môđun đơn, và cho D là hoán tập của nó. Các tính chất sau là tương đương:

(i) A-môđun S là nửa đơn tuyệt đối.

(ii) Đại số trên K D là nửa đơn tuyệt đối.

(iii) Đại số trên K D là một trường, có bậc hữu hạn trên K, và

tâm của nó là một mở rộng tách được của K.

Mệnh đề a) suy ra từ Mệnh đề 1, a) của VIII, p. 229. Cho S và D như trong b), và cho L là một mở rộng của K. A-môđun $A_{(L)}$ $S_{(L)}$ là nửa đơn khi và chỉ khi vành $D_{(L)}$ là nửa đơn (VIII, p. 222, Mệnh đề 8, c)). Điều này chứng minh tính tương đương của (i) và (ii), còn tính tương đương của (ii) và (iii) suy ra từ Định lý 1 vì D là một trường.

#### Hệ quả {#alg-viii-s13-n4-cor-1 .statement tag=00RF}

Cho K là một trường giao hoán, cho $A_1$ và $A_2$ là các K-đại số, và cho $M_1$ là một $A_1$-môđun nửa đơn tuyệt đối còn $M_2$ là một $A_2$-môđun nửa đơn. Khi đó $M_1\otimes_KM_2$ là một môđun nửa đơn trên vành $A_1\otimes_KA_2$.

Môđun $M_1$ là tổng trực tiếp của các $A_1$-môđun đơn nửa đơn tuyệt đối (Mệnh đề 4). Vì vậy, chỉ cần chứng minh mệnh đề trong trường hợp các môđun $M_1$ và $M_2$ là đơn. Ký hiệu các vành giao hoán tử của chúng là $D_1$ và $D_2$. Đại số trên K $D_1$ là nửa đơn tuyệt đối (loc. cit.); theo Hệ quả 1 của VIII, p. 234, đại số trên K $D_1\otimes_KD_2$ là nửa đơn. Khi đó suy ra từ Hệ quả 1 của VIII, p. 215 rằng môđun $(A_1\otimes_KA_2$)-môđun $M_1\otimes_KM_2$ là nửa đơn.

### 5. Các đạo hàm trên các đại số nửa đơn

Trong tiểu mục này và các tiểu mục tiếp theo, K là một vành giao hoán, A là một đại số trên K, B là đại số trên K $A\otimes_KA^o$, và $\varepsilon$ là ánh xạ K-tuyến tính từ B vào A được xác định bởi $\varepsilon (x\otimes y) =xy$ với $x, y$ trong A.

Nhắc lại (III, §4, No. 3, p. 467) rằng mọi $(A$, A)-song môđun P đều có thể được xem như một B-môđun trái, với phép toán ngoài được cho bởi $(a\otimes a')p=apa'$ với $a, a'$ thuộc A và $p$ thuộc P. Ngược lại, mọi B-môđun đều có thể được xem như một $(A,A)$-song môđun. Ta trang bị cho A cấu trúc $(A$, A)-song môđun chính tắc của nó và cấu trúc B-môđun tương ứng; ta trang bị cho B cấu trúc $(A$, A)-song môđun tương ứng với B-môđun $B_s$. Do đó ta có

$$
a(x\otimes y)a'= (a\otimes a')(x\otimes y) =ax\otimes ya'
$$

với $a, a', x, y$ thuộc A, trong đó tích $ya'$ được tính trong đại số A.

Ánh xạ K-tuyến tính $\varepsilon$ là một đồng cấu của các $(A$, A)-song môđun.

#### Mệnh đề 5 {#alg-viii-s13-prop-5 .statement tag=00FO}

Các tính chất sau là tương đương:

(i) B-môđun A là xạ ảnh.

(ii) Tồn tại một phần tử $e$ của song môđun $(A,A)$ B thỏa mãn hai điều kiện sau: $\varepsilon (e) = 1$ và $ae=ea$ với mọi $a\in A$.

Ánh xạ $\varepsilon : B\rightarrow A$ là toàn ánh vì ta có $\varepsilon (a\otimes 1) =a$ với mọi $a\in A$; nó là một đồng cấu của các $(A$, A)-môđun, do đó là một ánh xạ B-tuyến tính. Nếu B-môđun A là xạ ảnh, thì tồn tại một tiết diện $s$ của $\varepsilon$ (II, §2, No. 2, p. 231, Mệnh đề 4); nó là một đồng cấu của các $(A$, A)-hai môđun từ A tới B. Nếu đặt $e=s$(1), thì ta có $\varepsilon (e) =\varepsilon (s(1)) = 1$ và $ae=s(a) =ea$ với mọi $a\in A$. Vậy (i) kéo theo (ii).

Ngược lại, cho $e$ là một phần tử của B thỏa mãn các điều kiện trong mục (ii). Định nghĩa một ánh xạ $s$ từ A tới B bởi công thức

$$
s(a) =ae=ea \tag{1}
$$

Đó là một đồng cấu của các $(A$, A)-môđun, và ta có $\varepsilon \circ s= 1_A$; nói cách khác, $s$ là một tiết diện B-tuyến tính của ánh xạ toàn ánh $\varepsilon$. Do đó, B-môđun A đẳng cấu với môđun con hạng tử trực tiếp $s(A)$ của $B_s$ (II, §1, No. 9, p. 211, Mệnh đề 15) và vì thế là xạ ảnh (II, §2, No. 2, p. 231, Mệnh đề 4). Điều này chứng tỏ rằng (ii) kéo theo (i).

#### Nhận xét 1 {#alg-viii-s13-n5-rem-1 .statement tag=00FP}

Cho $e=\sum^r_{i=1}a_i\otimes a'_i$ là một phần tử của B. Các điều kiện trong mục (ii) của Mệnh đề 5 được chuyển thành các công thức

$$
\sum_{i=1}^ra_ia'_i= 1 \tag{2}
$$

(3) $\sum_{i=1}^raa_i\otimes a'_i=\sum_{i=1}^ra_i\otimes a'_ia$ với mọi $a\in A$.

Khi các điều kiện ấy được thỏa mãn, $e$ là một phần tử lũy đẳng trong B. Thật vậy, khi đó ta có các hệ thức

$$
e^2=\sum_{i=1}^ra_iea'_i=\sum_{i=1}^rea_ia'_i=e
$$

#### Nhận xét 2 {#alg-viii-s13-n5-rem-2 .statement tag=00FQ}

Cho K là một trường giao hoán, A là một đại số trên K, và M là một A-môđun. Nhóm End$_K(M)$ được trang bị một cấu trúc song môđun $(A$, A) được xác định bởi

$$
aua'(x) =au(a'x)
$$

đối với mọi $a, a'\in A$, mọi $u\in$ End$_K$(M), và mọi $x\in M$. Ta trang bị cho nó cấu trúc B-môđun liên kết. Cho $e=\sum^r_{i=1}a_i\otimes a'_i$ là một phần tử của B thỏa mãn các điều kiện trong phần (ii) của Mệnh đề 5, do đó cũng thỏa mãn các hệ thức (2) và (3). Nếu $p\in$ End$_K(M)$ là một phép chiếu mà ảnh N của nó là một A-môđun con của M, thì $ep$ là một phép chiếu A-tuyến tính có cùng ảnh.

Thật vậy, ảnh của $ep$ được chứa trong N. Nếu $x$ thuộc N, thì $a'_ix$ cũng thuộc N, nên ta có $p(a'_ix) =a'_ix$ và

$$
ep(x) =\sum_{i=1}^ra_ia'_ix=x
$$

theo công thức (2). Ta suy ra từ công thức (3) rằng $aep(x) =ep(ax)$ với mọi $a\in A$ và mọi $x\in M$, điều đó chứng tỏ rằng $ep$ là A-tuyến tính.

#### Định lý 2 {#alg-viii-s13-thm-2 .statement tag=00RG}

Cho K là một trường giao hoán và A là một đại số trên K. Các tính chất sau là tương đương:

(i) Đại số trên K A là nửa đơn tuyệt đối.

(ii) Đại số trên K $B = A\otimes_KA^o$ là nửa đơn.

(iii) B-môđun A là xạ ảnh.

(iv) Tồn tại một phần tử $e$ của $(A,A)$-song môđun B thỏa mãn $\varepsilon (e) = 1$ và $ae=ea$ với mọi $a\in A$.

Giả sử đại số A là nửa đơn tuyệt đối, do đó nửa đơn. Khi đó đại số $A^o$ là nửa đơn (VIII, p. 137, Mệnh đề 2), và từ Hệ quả 1 của VIII, p. 234 suy ra rằng $B = A\otimes_KA^o$ là một đại số trên K nửa đơn. Vì vậy, (i) kéo theo (ii).

Vì mọi môđun trên một vành nửa đơn đều là xạ ảnh (VIII, p. 138, Mệnh đề 4), nên (ii) kéo theo (iii).

Tính tương đương của (iii) và (iv) suy ra từ Mệnh đề 5. Để hoàn tất chứng minh, ta hãy chỉ ra rằng (iv) suy ra (i). Cho $e=\sum^r_{i=1}a_i\otimes a'_i$ là một phần tử của B thỏa mãn các điều kiện trong mục (ii) của Mệnh đề 5. Cho L là một mở rộng của trường K; ta phải chứng minh rằng vành $A_{(L)}$ là nửa đơn hay, tương đương, rằng mọi $A_{(L)}$-môđun đều là nửa đơn (VIII, p. 138, Mệnh đề 4). Cho M là một $A_{(L)}$-môđun, và cho N là một môđun con của M; ta xem M như một song môđun trái $(A$, L) và N như một môđun con song (III, §4, No. 3, p. 466). Vì L là một trường, tồn tại một phép chiếu L-tuyến tính $u$ của M có ảnh là N. Vì các vị tự $a_M$ liên kết với các phần tử $a$ của A là L-tuyến tính, nên tồn tại một đồng cấu nhóm duy nhất từ $A\otimes_KA^o$ vào End$_L(M)$ gửi một phần tử $a\otimes a'$ tới ánh xạ L-tuyến tính $x\mapsto au(a'x)$. Ta ký hiệu ảnh của $e$ bởi đồng cấu này là $v$; từ Nhận xét 2 suy ra rằng $v$ là một phép chiếu $A_{(L)}$-tuyến tính có ảnh là N. Hạt nhân của $v$ là một $A_{(L)}$-môđun con của M, bổ sung với N. Theo Hệ quả 2 của VIII, p. 56, $A_{(L)}$-môđun M là nửa đơn.

#### Nhận xét 3 {#alg-viii-s13-n5-rem-3 .statement tag=00FR}

Ta biết (VIII, p. 234, Hệ quả 1) rằng tích tenxơ của hai đại số nửa đơn tuyệt đối trên một trường giao hoán là nửa đơn tuyệt đối. Do đó, nếu đại số A là nửa đơn tuyệt đối, thì đại số $B = A\otimes_KA^o$ cũng vậy.

### 6. Đối đồng điều của các đại số

Trong tiểu mục này, K là một vành giao hoán, A là một đại số trên K, B là đại số trên K $A\otimes_KA^o$, và $\varepsilon$ là ánh xạ K-tuyến tính từ B vào A được xác định bởi $\varepsilon (x\otimes y) =$ $xy$ với $x, y$ thuộc A. Với $n\in \mathbf{N}$, ta ký hiệu tích tenxơ trên K của $n+ 2$ bản sao của K-môđun A là $B_n$. Ta xem nó như một song môđun $(A$, A) (và cũng như một B-môđun); ta trang bị cho nó cấu trúc A-môđun trái suy ra từ cấu trúc A-môđun trái của nhân tử thứ nhất của tích tenxơ và cấu trúc A-môđun phải suy ra từ cấu trúc A-môđun phải của nhân tử cuối cùng. Đặc biệt, $B_0$ chỉ là song môđun $(A$, A) B.

Với mọi số nguyên $n\geqslant 1$, ta định nghĩa các đồng cấu của song môđun $d_n^i$ với $i\in [0, n]$ và $d_n$ từ $B_n$ đến $B_{n-1}$ bằng các công thức

$$
d_n^i(x_0\otimes  \cdots  \otimes x_{n+1}) =x_0\otimes  \cdots  \otimes x_ix_{i+1}\otimes  \cdots  \otimes x_{n+1} \tag{4}
$$

với $i\in [0, n]$ và

$$
d_n=\sum_{i=0}^n(-1)^id_n^i \tag{5}
$$

Ta ký hiệu ánh xạ $\varepsilon : B_0\rightarrow A$ bởi $d_0=d^0_0$.

Cho $n$ là một số nguyên $\geqslant 1$. Với $0\leqslant i < j\leqslant n$, ta có

$$
d_{n-1}^i\circ d_n^j=d_{n-1}^{j-1}\circ d_n^i \tag{6}
$$

và từ đó ta suy ra

$$
d_{n-1}\circ d_n=\sum_{0\leqslant i<j\leqslant n}(-1)^{i+j}d_{n-1}^i\circ d_n^j+\sum_{0\leqslant j\leqslant i\leqslant n-1}(-1)^{i+j}d_{n-1}^i\circ d_n^j
$$

$$
=\sum_{0\leqslant i<j\leqslant n}(-1)^{i+j}d_{n-1}^{j-1}\circ d_n^i+\sum_{0\leqslant j\leqslant i\leqslant n-1}(-1)^{i+j}d_{n-1}^i\circ d_n^j
$$

và do đó

$$
d_{n-1}\circ d_n= 0 \tag{7}
$$

Cho P là một song môđun $(A$, A). Với mọi số nguyên $n\geqslant 0$, ta ký hiệu K-môđun các ánh xạ K-đa tuyến tính từ $A^n$ vào P bởi $C^n(A,P)$. Ánh xạ $\alpha^n: C^n(A,P)\rightarrow$ Hom$_B(B_n,P)$ biến $f\in C^n(A,P)$ thành đồng cấu $\alpha^n(f)$ được đặc trưng bởi

$$
\alpha^n(f) (x_0\otimes  \cdots  \otimes x_{n+1}) =x_0f(x_1, . . . , x_n)x_{n+1} \tag{8}
$$

là một đẳng cấu của các K-môđun.

Ta ký hiệu bởi $\partial^n$ (với $n\geqslant 0$) ánh xạ K-tuyến tính duy nhất từ $C^n(A,P)$ đến $C^{n+1}(A,P)$ sao cho biểu đồ sau là giao hoán:

$C^n(A,P)\partial^{^n}$ // $C^{n+1}(A,P)$

$\alpha^n\alpha^{n+1}$

Hom$_B(B_n,P)^{Hom(d_{n+1},1_P)}/$/ Hom$_B(B_{n+1},P)$.

Theo định nghĩa, do đó ta có

$$
(\alpha^{n+1}\circ \partial^n)(f) =\alpha^n(f)\circ d_{n+1} \tag{9}
$$

với mọi $f\in C^n(A,P)$. Nói cách khác, ta có

$$
\partial^n(f) (x_0, . . . , x_n) =\alpha^n(f) (d_{n+1}(1\otimes x_0\otimes  \cdots  \otimes x_n\otimes 1))
$$

với $x_0, . . . , x_n$ trong A và $f$ trong $C^n(A,P)$, tức là,

$$
\partial^n(f)(x_0, . . . , x_n) =x_0f(x_1, . . . , x_n) \tag{10}
$$

$$
+\sum^{n-1}_{i=0}(-1)^{i+1}f(x_0, . . . , x_{i-1}, x_ix_{i+1}, x_{i+2}, . . . , x_n)
$$

$$
+ (-1)^{n+1}f(x_0, . . . , x_{n-1})x_n
$$

Theo (7) và (9), ta có

(11) $\partial^{n+1}\circ \partial^n= 0$ với mọi $n\geqslant 0$.

Ta ký hiệu K-môđun Ker $\partial^0$ bởi $H^0(A,P)$ và, với $n\geqslant 1$, K-môđun Ker $\partial^n/$ Im $\partial^{n-1}$ bởi $H^n(A,P)$. Ta đồng nhất K-môđun $C^0(A,P)$ với P, và ta có $C^1(A,P) =$ Hom$_K(A,P)$. Các ánh xạ $\partial^n$ với $n\leqslant 2$ được cho bởi các công thức

(12) $\partial^0(p)(a) =ap-pa$ với mọi $p\in P$,

(13) $\partial^1(f)(a, a') =af(a')-f(aa') +f(a)a'$ với $f\in C^1(A,P)$,

$$
\partial^2(f)(a, a', a'') =af(a', a'')-f(aa', a'') +f(a, a'a'')-f(a, a')a'' \tag{14}
$$

đối với $f\in C^2(A,P)$.

Vậy $H^0(A,P)$ là K-môđun con của P gồm các phần tử $p$ sao cho $ap=pa$ với mọi $a\in A$, và $H^1(A,P)$ là thương của K-môđun Der$_K(A,P)$ các K-phép đạo hàm từ A vào P (III, §10, No. 2, p. 553) bởi K-môđun con gồm các phép đạo hàm dạng $a\mapsto ap-pa$ với $p\in P$ (gọi là các phép đạo hàm nội).

### 7. Đối đồng điều của các đại số nửa đơn tuyệt đối

#### Mệnh đề 6 {#alg-viii-s13-prop-6 .statement tag=00FS}

Cho K là một vành giao hoán và A là một đại số trên K. Cho $e=\sum^r_{i=1}a_i\otimes a'_i$ là một phần tử của $B = A\otimes_KA^o$ thỏa mãn các điều kiện trong mục (ii) của Mệnh đề 5 của VIII, p. 236. Với mọi số nguyên $n\geqslant 1$ và mọi phần tử $f$ của $C^n(A,P)$, ta ký hiệu bởi $\gamma^n(f)$ phần tử của $C^{n-1}(A,P)$ được xác định bởi công thức

$$
\gamma^n(f)(x_1, . . . , x_{n-1}) =\sum_{i=1}^ra_if(a'_i, x_1. . . , x_{n-1}) \tag{15}
$$

Khi đó ta có

$$
\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f)) =f \tag{16}
$$

với mọi số nguyên $n\geqslant 1$ và mọi $f\in C^n(A,P)$.

#### Nhận xét 1 {#alg-viii-s13-n7-rem-1 .statement tag=00SF}

$*$Các đồng cấu $\partial^n: C^n(A,P)\rightarrow C^{n+1}(A,P)$ xác định một phức $(C(A,P), \partial )$ các K-môđun (X, §2, n$^o1$, p. 24). Do đó ánh xạ $\gamma_n$ xác định một đồng luân từ phức này đến chính nó nối 0 với Id$_{C(A,P)}$ (X, §2, n$^o4$, p. 32, định nghĩa $4$)$.*$

Ta giữ ký hiệu của No. 6. Với mọi số nguyên $n\geqslant 0$, ta định nghĩa một ánh xạ $h_n: B_n\rightarrow B_{n+1}$ bởi công thức

$$
h_n(x) =d^1_{n+2}(e\otimes x) =\sum_{i=1}^ra_i\otimes a'_ix
$$

Đó là một đồng cấu của các $(A$, A)-song môđun (công thức (3)).

#### Bổ đề 5 {#alg-viii-s13-lem-5 .statement tag=00FT}

Ta có quan hệ

$$
d_{n+1}\circ h_n+h_{n-1}\circ d_n= 1_{B_n} \tag{17}
$$

với mọi $n\geqslant 1$.

Cho $x\in B_n$; ta có

$$
(d_{n+1}\circ h_n)(x) = (d_{n+1}\circ d^1_{n+2})(e\otimes x)
$$

$$
= (d^0_{n+1}\circ d^1_{n+2})(e\otimes x)-\sum^{n+2}_{i=2}(-1)^i(d_{n+1}^{i-1}\circ d^1_{n+2})(e\otimes x)
$$

nên, theo công thức (6),

$$
(d_{n+1}\circ h_n)(x) = (d^0_{n+1}\circ d^0_{n+2})(e\otimes x)-\sum^{n+2}_{i=2}(-1)^i(d^1_{n+1}\circ d_{n+2}^i)(e\otimes x)
$$

Nhưng ta có

$$
(d^0_{n+1}\circ d^0_{n+2})(e\otimes x) =\varepsilon (e)x=x
$$

theo tính chất (ii) của Mệnh đề 5 của VIII, p. 236 và, với $i\geqslant 2$,

$$
d^i_{n+2}(e\otimes x) =e\otimes d^{i-2}_n(x)
$$

từ đó suy ra

$$
(d_{n+1}\circ h_n)(x) =x-d^1_{n+1}(e\otimes d_n(x)) =x-h_{n-1}\circ d_n(x)
$$

và do đó công thức (17).

Ta có thể hoàn tất chứng minh của Mệnh đề 6 bằng cách dùng Bổ đề 5. Cho $n$ là một số nguyên $\geqslant 1$ và $f$ là một phần tử của $C^n(A,P)$. Theo phép dựng, ta có

$$
\alpha^{n-1}(\gamma^n(f)) =\alpha^n(f)\circ h_{n-1} \tag{18}
$$

và, do đó, theo các công thức (9) và (18),

$$
\alpha^n(\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f))) =\alpha^{n-1}(\gamma^n(f))\circ d_n+\alpha^{n+1}(\partial^n(f))\circ h_n
$$

$$
=\alpha^n(f)\circ h_{n-1}\circ d_n+\alpha^n(f)\circ d_{n+1}\circ h_n
$$

$$
=\alpha^n(f)
$$

trong đó đẳng thức cuối cùng suy ra từ (17). Vì $\alpha^n$ là song ánh, mệnh đề được suy ra.

#### Định lý 3 {#alg-viii-s13-thm-3 .statement tag=00FU}

Cho K là một vành giao hoán, A một đại số trên K, và P một $(A,A)$-song môđun. Giả sử A-môđun $(A\otimes_KA^o)$ là xạ ảnh. Khi đó ta có $H^n(A,P) = 0$ với mọi số nguyên $n\geqslant 1$.

Ta phải chứng minh rằng với mọi số nguyên $n\geqslant 1$, mọi phần tử $f$ của $C^n(A,P)$ thỏa $\partial^n(f) = 0$ đều có dạng $\partial^{n-1}(g)$ đối với một phần tử $g$ của $C^{n-1}(A,P)$. Theo Mệnh đề 5, đây là một hệ quả ngay lập tức của Mệnh đề 6.

#### Hệ quả {#alg-viii-s13-n7-cor-1 .statement tag=00FV}

Mọi đạo hàm K từ A đến P đều là nội.

Đây là cách diễn đạt của đẳng thức $H^1(A,P) = 0$.

#### Nhận xét 2 {#alg-viii-s13-n7-rem-2 .statement tag=00FW}

Các giả thiết của Định lý 3, đặc biệt, được thỏa mãn khi K là một trường và A là một đại số trên K nửa đơn tuyệt đối (VIII, p. 238, Định lý 2).

#### Nhận xét 3 {#alg-viii-s13-n7-rem-3 .statement tag=00FX}

Giả sử K-môđun A là xạ ảnh. Định lý 3 cũng có thể được chứng minh như sau. Phức $(\bigoplus_{n\geqslant 0}B_n, d)$ và đồng cấu $\varepsilon : B_0\rightarrow A$ xác định một phân giải xạ ảnh của B-môđun A; do đó, với mọi $n\geqslant 0$, K-môđun $H^n(A,P)$ đẳng cấu với Ext$^n_B(A,P)$ (X, §6, n$^o1$, p. 100, định lý 1). Nếu B-môđun A là xạ ảnh, thì các K-môđun Ext$^n_B(A,P)$ bằng không với $n\geqslant 1$ (X, §5, n$^o3$, p. 88, hệ quả của mệnh đề 5), điều đó suy ra rằng $H^n(A,P)$ bằng không. Ngược lại, nếu $H^1(A,P)$ bằng không đối với mọi $(A$, A)-song môđun P, thì B-môđun A là xạ ảnh (X, §5, n$^o5$, p. 93, mệnh đề $10$)$.*$

### 8. Sự Tách của các Đại số Artin

Trong tiểu mục này, K là một vành giao hoán và A là một đại số trên K. Gọi $\mathfrak{r}$ là căn của A. Ta ký hiệu đại số thương $A/\mathfrak{r}$ là $\overline{A}$ và ánh xạ chính tắc từ A vào $\overline{A}$ là $\pi$. Ta quan tâm đến các đại số con S của A sao cho $A = S\oplus \mathfrak{r}$.

Ta ký hiệu bởi Σ tập hợp các tiết diện K-tuyến tính $s$ của $\pi$ thỏa mãn $s(\alpha \beta ) =$ $s(\alpha )s(\beta )$ với $\alpha , \beta$ trong A. Chú ý rằng một tiết diện như vậy tất yếu thỏa mãn $s(1) = 1$ (nói cách khác, $s$ là một đồng cấu vành): thật vậy, ta có $s(1)^2=s$(1), và $s(1)$ là khả nghịch vì nó thuộc $1 +\mathfrak{r}$ (VIII, p. 156, Định lý 1). Nếu $s$ là một phần tử của Σ, thì ảnh S của $s$ là một đại số con của A, và ta có $A = S\oplus \mathfrak{r}$. Ngược lại, nếu S là một đại số con của A sao cho $A = S\oplus \mathfrak{r}$, thì hạn chế của $\pi$ lên S là song ánh, và song ánh ngược xác định một phần tử của Σ có ảnh là S.

Theo định lý của Jacobson (loc. cit.), mọi phần tử của $1 +\mathfrak{r}$ đều khả nghịch trong A. Ta gọi một tự đẳng cấu trong của A có dạng $a\mapsto xax^{-1}$ với $x\in 1 +\mathfrak{r}$ là một tự đẳng cấu đặc biệt.

#### Mệnh đề 7 {#alg-viii-s13-prop-7 .statement tag=00FY}

Giả sử $(A\otimes_K\overline{A}^o)$-môđun $\overline{A}$ là xạ ảnh.

a) Cho $S_1$ và $S_2$ là các đại số con của A thỏa mãn $A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$. Tồn tại một tự đẳng cấu đặc biệt của A biến đổi $S_1$ thành $S_2$.

b) Giả sử $\pi$ có một tiết diện K-tuyến tính và căn $\mathfrak{r}$ của A là lũy linh. Khi đó tồn tại một đại số con S của A thỏa mãn $A = S\oplus \mathfrak{r}$.

Cho $S_1$ và $S_2$ như trong a). Gọi $s_1$ và $s_2$ là các phần tử của tập hợp Σ tương ứng với các đại số con $S_1$ và $S_2$. Gọi $\varepsilon$ là ánh xạ K-tuyến tính từ $A\otimes_KA$ vào A được xác định bởi $\varepsilon (a\otimes b) =ab$. Theo Mệnh đề 5 của VIII, p. 236 và Nhận xét 1 của VIII, p. 237, tồn tại một phần tử $e=\sum^r_{i=1}\alpha_i\otimes \alpha '_i$ của $\overline{A}\otimes_KA$ thỏa mãn $\sum^r_{i=1}\alpha_i\alpha '_i= 1$ và $\sum^r_{i=1}\alpha \alpha_i\otimes \alpha '_i=\sum^r_{i=1}\alpha_i\otimes \alpha '_i\alpha$ với mọi $\alpha \in A$. Đặt $x=\sum^r_{i=1}s_1(\alpha_i)s_2(\alpha '_i)$. Ta có $\pi (x) =\sum^r_{i=1}\alpha_i\alpha '_i= 1$ và do đó $x\in 1 +\mathfrak{r}$. Gọi $\alpha$ là một phần tử của A. Ta có

$$
s_1(\alpha )x=\sum_{i=1}^rs_1(\alpha \alpha_i)s_2(\alpha '_i) = (\varepsilon \circ (s_1\otimes s_2))(\sum_{i=1}^r\alpha \alpha_i\otimes \alpha '_i)
$$

$$
= (\varepsilon \circ (s_1\otimes s_2))(\sum_{i=1}^r\alpha_i\otimes \alpha '_i\alpha )=\sum_{i=1}^rs_1(\alpha_i)s_2(\alpha '_i\alpha ) =xs_2(\alpha )
$$

Đẳng thức $x^{-1}S_1x= S_2$ suy ra, do đó cho mệnh đề a).

Dưới các giả thiết của b), giả sử thêm rằng $\mathfrak{r}^2= 0$. Trong trường hợp này, $(A$, A)-song môđun $\mathfrak{r}$ bị triệt tiêu bởi $\mathfrak{r}$, và vì thế ta xem nó như một $(A$, A)-song môđun. Chọn một tiết diện K-tuyến tính $\sigma$ của $\pi$. Ta có

(19) $\alpha x=\sigma (\alpha )x$ and $x\alpha =x\sigma (\alpha )$

với $\alpha \in \overline{A}$ và $x\in \mathfrak{r}$. Đặt

$$
\varphi (\alpha , \beta ) =\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta ) \tag{20}
$$

với $\alpha , \beta \in A$. Ta có quan hệ $\pi (\varphi (\alpha , \beta )) =\alpha \beta -\alpha \beta = 0$ với $\alpha , \beta \in A$. Do đó, $\varphi$ xác định một phần tử của $C^2(A,\mathfrak{r})$. Gọi $\alpha , \beta , \gamma$ là các phần tử của A; theo (19), ta có

$$
\partial^2\varphi (\alpha , \beta , \gamma ) =\alpha \varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\gamma
$$

$$
=\sigma (\alpha )\varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\sigma (\gamma )
$$

$$
=\sigma (\alpha )(\sigma (\beta \gamma )-\sigma (\beta )\sigma (\gamma ))-\sigma (\alpha \beta \gamma ) +\sigma (\alpha \beta )\sigma (\gamma ) +\sigma (\alpha \beta \gamma )
$$

$$
-\sigma (\alpha )\sigma (\beta \gamma )-(\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta ))\sigma (\gamma )
$$

$$
= 0
$$

Theo Định lý 3 của VIII, p. 242, K-môđun $H^2(A,\mathfrak{r})$ thu về không. Vậy tồn tại một phần tử $\psi$ của $C^1(A,\mathfrak{r})$ sao cho $\partial^1\psi =\varphi$, nói cách khác, sao cho ta có

(21) $\varphi (\alpha , \beta ) =\alpha \psi (\beta )-\psi (\alpha \beta ) +\psi (\alpha )\beta$ với $\alpha , \beta$ trong $\overline{A}$.

Ta có $\psi (\alpha )\psi (\beta ) = 0$ vì $\mathfrak{r}^2$ bằng không; từ (19) và (20), do đó suy ra (22) $(\sigma +\psi )(\alpha \beta ) = (\sigma +\psi )(\alpha )(\sigma +\psi )(\beta )$,

sao cho tiết diện K-tuyến tính $\sigma +\psi$ của $\pi$ thuộc Σ. Ảnh của nó là một đại số con S của A sao cho $A = S +\mathfrak{r}$.

Bây giờ hãy chứng minh sự tồn tại của S trong trường hợp tổng quát. Ta lập luận bằng quy nạp theo số nguyên nhỏ nhất $p\geqslant 1$ sao cho $\mathfrak{r}^p= 0$; trường hợp $p= 1$ là tầm thường. Giả sử $p\geqslant 2$, và đặt $A'= A/\mathfrak{r}^{p-1}$. Căn $\mathfrak{r}'$ của $A'$ bằng $\mathfrak{r}/\mathfrak{r}^{p-1}$ (Mệnh đề 5 của VIII, p. 155), nên thỏa mãn ${\mathfrak{r}'}^{p-1}= 0$, và đại số $A'/\mathfrak{r}'$ đẳng cấu với $\overline{A}= A/\mathfrak{r}$ và do đó là nửa đơn tuyệt đối. Theo giả thiết quy nạp, tồn tại một đại số con $S'$ của $A'$ sao cho $A'= S'\oplus \mathfrak{r}'$. Khi đó $S'$ có dạng $A''/\mathfrak{r}^{p-1}$, trong đó $A''$ là một đại số con của A chứa $\mathfrak{r}^{p-1}$, và ta có

$$
A = A''+\mathfrak{r},\mathfrak{r}^{p-1}= A''\cap \mathfrak{r} \tag{23}
$$

Đại số $A''/\mathfrak{r}^{p-1}$ đẳng cấu với $A'/\mathfrak{r}'$; ta có $(\mathfrak{r}^{p-1})^2= 0$, nên $\mathfrak{r}^{p-1}$ là căn của $A''$. Theo trường hợp vừa xét, tồn tại một đại số con S của $A''$ sao cho $A''= S\oplus \mathfrak{r}^{p-1}$; từ (23) ta suy ra quan hệ $A = S\oplus \mathfrak{r}$.

#### Hệ quả 1 (định lý Wedderburn) {#alg-viii-s13-prop-7-cor-1 .statement tag=00S8}

Cho K là một trường giao hoán, A là một đại số trên K, và $\mathfrak{r}$ là căn của A. Giả sử rằng K-đại số $A/\mathfrak{r}$ là nửa đơn tuyệt đối.

a) Cho $S_1$ và $S_2$ là các đại số con của A thỏa mãn $A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$. Tồn tại một tự đẳng cấu đặc biệt của A biến $S_1$ thành $S_2$.

b) Nếu $\mathfrak{r}$ lũy linh, thì tồn tại một đại số con S của A thỏa mãn A = $S\oplus \mathfrak{r}$.

Điều này suy ra từ Mệnh đề 7 và Định lý 2 của VIII, p. 238.

#### Hệ quả 2 {#alg-viii-s13-prop-7-cor-2 .statement tag=00FZ}

Cho A là một đại số giao hoán bậc hữu hạn trên một trường hoàn hảo K, và cho $\mathfrak{r}$ là căn của nó. Tồn tại một đại số con duy nhất S của A sao cho $A = S\oplus \mathfrak{r}$. Hơn nữa, S đẳng cấu với một tích của hữu hạn nhiều mở rộng của K có bậc hữu hạn.

Đại số trên K $A/\mathfrak{r}$ là nửa đơn (VIII, p. 173, Mệnh đề 1) và có bậc hữu hạn; nó nửa đơn tuyệt đối vì trường K là hoàn hảo (VIII, p. 232, Định lý 1). Vì iđêan $\mathfrak{r}$ lũy linh và A giao hoán, nên sự tồn tại và tính duy nhất của S suy ra từ Hệ quả 1. Vì S nửa đơn, giao hoán và có bậc hữu hạn, nên khẳng định cuối cùng là hệ quả của Mệnh đề 3 của VIII, p. 137.

#### Nhận xét 1 {#alg-viii-s13-n8-rem-1 .statement tag=00G0}

Giả thiết rằng $A/\mathfrak{r}$ nửa đơn tuyệt đối là cốt yếu trong Hệ quả 1 (VIII, p. 246, Bài tập 4).

#### Nhận xét 2 {#alg-viii-s13-n8-rem-2 .statement tag=00G1}

Giả sử A là một đại số Artin trên trường K. Nếu A giao hoán, thì ta có thể chứng minh (VIII, p. 180, Bài tập 9) rằng A đẳng cấu với một tích các đại số $A_1\times  \cdots  \times A_n$ sao cho $A_i/\mathfrak{R}(A_i)$ là một trường với mọi $i$. Ngược lại, nếu A không giao hoán, thì A có thể không đẳng cấu với một tích các đại số $A_1\times  \cdots  \times A_n$ sao cho $A_i/\mathfrak{R}(A_i)$ là một vành đơn với mọi $i$ (VIII, p. 247, Bài tập 5).

### Bài tập {#alg-viii-s13-exercises}

Xem [bài tập của § 13](exercises/s13/).
