---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 8
section_title: Semisimple Rings
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.135-A VIII.150
pdf_pages: 0152-0167
extraction: native
subsections:
    - "no": 1
      title: Semisimple Rings
      page: 135
      pdf_page: 152
    - "no": 2
      title: Modules over a Semisimple Ring
      page: 138
      pdf_page: 155
    - "no": 3
      title: Factors of a Semisimple Ring
      page: 141
      pdf_page: 158
    - "no": 4
      title: Idempotents and Semisimple Rings
      page: 145
      pdf_page: 162
statements: 30
exercises: 6
content_sha256: e0c2f8998f17a3c7ce83c664acdf2cc2b20092d33ab8879db4acdfe2c9928875
translated_from: content/en/alg/VIII/08_s8_semisimple_rings.md
source_content_sha256: c3520cd3a5b6efacdd841870c3c2e342b0341edbd32074687bd212bc32731ee7
translation_model: gpt-5.4
translation_run: translate-vi-d30757fd
glossary_version: 34
glossary_terms_sha256: 2d8d8d7fc1558db5b144582dae78cd4a3f865c76b788594c608d464d0db2b8a3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. VÀNH NỬA ĐƠN

### 1. Vành Nửa Đơn

#### Định lý 1 (Wedderburn) {#alg-viii-s8-thm-1 .statement tag=00S4}

Cho A là một vành. Các tính chất sau là tương đương:

(i) A-môđun $A_s$ là nửa đơn.

(ii) Với mọi iđêan trái $\mathfrak{a}$ của A, tồn tại một iđêan trái $\mathfrak{b}$ của A sao cho $A_s$ là tổng trực tiếp của $\mathfrak{a}$ và $\mathfrak{b}$.

(iii) Vành A là Artin trái, và song môđun $(A,A)$ $_sA_d$ là nửa đơn.

(iv) Vành A đẳng cấu với tích của một họ hữu hạn các vành đơn.

(v) Tồn tại một số nguyên $s\geqslant$ 0, các trường $D_1, . . . ,D_s$, và các số nguyên $r_1\geqslant 1, . . .,r_s\geqslant 1$ sao cho vành A đẳng cấu với tích của các vành ma trận $\mathbf{M}_{r_i}(D_i)$.

(vi) Vành A là Artin trái, và tồn tại một A-môđun trái trung thành và nửa đơn.

Sự tương đương của (i) và (ii) suy ra từ Hệ quả 2 của VIII, p. 56, và sự tương đương của (iv) và (v) suy ra từ Định lý 1 của VIII, p. 120.

A-môđun $A_s$ sinh hữu hạn. Nếu nó nửa đơn, thì nó là Artin trái (VIII, p. 71, Mệnh đề 10). Vì A-môđun $A_s$ là trung thành, điều này chứng minh rằng (i) kéo theo (vi). Ngược lại, giả sử rằng tính chất (vi) được thỏa mãn; đặt M là một A-môđun nửa đơn trung thành. Tồn tại một số nguyên $m\geqslant 1$ sao cho $A_s$ đẳng cấu với một môđun con của $M^m$ (VIII, p. 50, Mệnh đề 5, a)); vì M là nửa đơn, điều tương tự cũng đúng với $A_s$. Vậy chúng ta đã chứng minh được sự tương đương của (i) và (vi).

Hãy chứng minh rằng (i) kéo theo (iii). Giả sử rằng vành A có tính chất (i); ta đã nhận thấy rằng khi đó A là Artin trái. Bây giờ, các nội cấu của A-môđun trái $A_s$ là các phép nhân bên phải bởi các phần tử của A. Từ đó suy ra rằng $(A$, A)-song môđun $_sA_d$ là nửa đơn theo Mệnh đề 6 của VIII, p. 86.

Ta hãy chỉ ra rằng (iii) suy ra (iv). Giả sử rằng song môđun $(A$, A) $_sA_d$ là nửa đơn. Nó sinh hữu hạn, nên tồn tại một họ hữu hạn $(\mathfrak{a}_i)_{i\in I}$ các môđun con đơn $(A$, A)-song môđun có tổng trực tiếp là $_sA_d$. Nói cách khác, các $\mathfrak{a}_i$ là các iđêan hai phía khác không của A, nhóm cộng của A là tổng trực tiếp của các $\mathfrak{a}_i$, và với mọi $i\in I$, mọi iđêan hai phía của A được chứa trong $\mathfrak{a}_i$ thì bằng 0 hoặc $\mathfrak{a}_i$. Đặt $\mathfrak{b}_i=\sum_{j\not=i}\mathfrak{a}_j$ với mọi $i\in I$; đây là một iđêan hai phía của A. Ánh xạ $a\mapsto (a+\mathfrak{b}_i)_{i\in I}$ là một đẳng cấu từ vành A lên tích các vành $A/\mathfrak{b}_i$. Các $(A$, A)-song môđun $\mathfrak{a}_i$ và $A/\mathfrak{b}_i$ là đẳng cấu, nên mọi iđêan hai phía của $A/\mathfrak{b}_i$ đều bằng 0 hoặc $A/\mathfrak{b}_i$. Nếu vành A là Artin trái, thì điều tương tự cũng đúng đối với các vành $A/\mathfrak{b}_i$, do đó chúng là đơn (VIII, p. 120, Định nghĩa 1).

Cuối cùng, hãy chứng minh rằng (iv) kéo theo (i). Giả sử rằng A là tích của một họ hữu hạn $(A_i)_{i\in I}$ các vành đơn. Ký hiệu bởi $\pi_i$ phép chiếu có chỉ số $i$ từ A lên $A_i$ và bởi $M_i$ A-môđun có nhóm cộng nền là $A_i$ và luật tác động $(a, x)\mapsto \pi_i(a)x$. Vì vành $A_i$ là đơn, $A_i$-môđun $(A_i)_s$ là nửa đơn, nên A-môđun $M_i$ là nửa đơn. Vì A-môđun $A_s$ không là gì khác ngoài tích $\prod_{i\in I}M_i$, nên nó là nửa đơn.

#### Định nghĩa 1 {#alg-viii-s8-def-1 .statement tag=0093}

Ta nói rằng một vành A là nửa đơn nếu nó có các tính chất tương đương (i) đến (vi) của Định lý 1. Một đại số A trên một vành giao hoán $k$ là một đại số nửa đơn nếu vành nền của A là nửa đơn.

#### Mệnh đề 1 {#alg-viii-s8-prop-1 .statement tag=0094}

Cho A là một vành nửa đơn. Tồn tại một họ hữu hạn $(\mathfrak{m}_i)_{i\in I}$ các iđêan trái cực tiểu của A sao cho $A_s=\oplus_{i\in I}\mathfrak{m}_i$. Nếu $(\mathfrak{m}_i)_{i\in I}$ là một họ như vậy, thì mọi A-môđun đơn đều đẳng cấu với một trong các $\mathfrak{m}_i$. Tập hợp các lớp của các A-môđun đơn là hữu hạn.

Mệnh đề thứ nhất suy ra từ sự kiện là A-môđun $A_s$ là nửa đơn và sinh hữu hạn. Mọi môđun đơn đều đẳng cấu với một thương của $A_s$ (VIII, p. 46, Mệnh đề 1). Mệnh đề thứ hai khi đó suy ra từ Hệ quả 3 của VIII, p. 56, và mệnh đề thứ ba là một hệ quả ngay lập tức của mệnh đề thứ hai.

#### Ví dụ {#alg-viii-s8-n1-exa-1 .statement tag=0095}

Cho G là một nhóm hữu hạn và K là một trường giao hoán. $*$Ta sẽ thấy về sau (VIII, p. 401, Hệ quả 1) rằng đại số K[G] của nhóm G trên trường K là một vành nửa đơn khi và chỉ khi số mũ đặc số của K nguyên tố cùng nhau với cấp của $G.*$

#### Nhận xét 1 {#alg-viii-s8-n1-rem-1 .statement tag=0096}

Cho K là một trường giao hoán, và cho A là một đại số nửa đơn trên K. Khi đó tồn tại các đại số trên K $D_1, . . . ,D_s$ là các trường và các số nguyên $r_1\geqslant 1, . . . , r_s\geqslant 1$ sao cho đại số trên K A đẳng cấu với tích $\prod^s_{i=1}\mathbf{M}_{r_i}(D_i)$.

#### Nhận xét 2 {#alg-viii-s8-n1-rem-2 .statement tag=0097}

Cho K là một trường đóng đại số, và cho A là một đại số bậc hữu hạn trên K. Theo Nhận xét 4 của VIII, p. 122, đại số A là nửa đơn khi và chỉ khi tồn tại các số nguyên $n_1\geqslant 1, . . . , n_r\geqslant 1$ sao cho A đẳng cấu với đại số $\mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$.

#### Mệnh đề 2 {#alg-viii-s8-prop-2 .statement tag=0098}

a) Tâm của một vành nửa đơn là nửa đơn.

b) Vành đối của một vành nửa đơn là nửa đơn.

c) Thương của một vành nửa đơn theo một iđêan hai phía là một vành nửa đơn.

d) Tích của một họ hữu hạn các vành nửa đơn là một vành nửa đơn.

Cho A là một vành nửa đơn. Nó đẳng cấu với tích của một họ hữu hạn $(A_i)_{i\in I}$ các vành đơn. Tâm của A đẳng cấu với tích của các tâm của các $A_i$, và $A^o$ đẳng cấu với vành tích của các $A^o_i$. Do đó các mệnh đề a) và b) suy ra từ Hệ quả 1 của VIII, p. 121.

Cho $\mathfrak{a}$ là một iđêan hai phía của A. A-môđun $A_s/\mathfrak{a}$, là thương của A-môđun nửa đơn $A_s$, là nửa đơn. Do đó $(A/\mathfrak{a}$)-môđun $A_s/\mathfrak{a}$ là nửa đơn; suy ra mệnh đề c).

Một vành là nửa đơn khi và chỉ khi nó đẳng cấu với tích của một họ hữu hạn các vành đơn; suy ra mệnh đề d).

#### Mệnh đề 3 {#alg-viii-s8-prop-3 .statement tag=0099}

Cho A là một vành giao hoán. Các tính chất sau là tương đương:

(i) Vành A là nửa đơn.

(ii) Vành A là Artin và rút gọn (V, §6, No. 7, p. 34).

(iii) Vành A đẳng cấu với tích của một họ hữu hạn các trường giao hoán.

Các vành đơn giao hoán là các trường giao hoán (VIII, p. 120, Nhận xét 1). Vậy (i) tương đương với (iii).

Hiển nhiên là (iii) suy ra (ii). Ngược lại, giả sử rằng vành A là Artin và không có phần tử lũy linh khác 0. Giao của tập hợp các iđêan nguyên tố của A gồm các phần tử lũy linh của A (V, §15, No. 1, p. 118, Mệnh đề 2), do đó thu về 0 vì A không có phần tử lũy linh khác 0. Theo VIII, p. 2, khi đó tồn tại các iđêan nguyên tố phân biệt $\mathfrak{p}_1, . . . ,\mathfrak{p}_r$ của A sao cho ta có $\mathfrak{p}_1\cap  \cdots  \cap \mathfrak{p}_r= 0$. Theo hệ quả ở VIII, p. 8, mỗi iđêan nguyên tố $\mathfrak{p}_i$ của vành Artin A là cực đại; do đó ta có $\mathfrak{p}_i+\mathfrak{p}_j= A$ mỗi khi $i$ và $j$ phân biệt. Theo Mệnh đề 9 của I, §8, No. 11, p. 110, đồng cấu chính tắc từ A vào vành $\prod^r_{i=1}(A/\mathfrak{p}_i)$ là một đẳng cấu. Vành $A/\mathfrak{p}_i$ là một trường với mọi $i$, và vì thế (ii) suy ra (iii).

Một đại số giao hoán bậc hữu hạn trên một trường là một vành giao hoán Artin. Do đó Mệnh đề 3 khái quát hóa Mệnh đề 5 của V, §6, No. 7, p. 34.

### 2. Các môđun trên vành nửa đơn

#### Mệnh đề 4 {#alg-viii-s8-prop-4 .statement tag=009A}

Cho A là một vành. Các tính chất sau là tương đương:

(i) Vành A là nửa đơn.

(ii) Mọi A-môđun đều là nửa đơn.

(iii) Tồn tại một A-môđun vừa sinh vừa nửa đơn.

(iv) Tồn tại một A-môđun trung thành và nửa đơn có môđun đối sinh hữu hạn.

(v) Mọi A-môđun đều xạ ảnh.

(vi) Mọi A-môđun đơn sinh đều xạ ảnh.

$*$Để có các đặc trưng khác của các vành nửa đơn, xem Mệnh đề 6 của X, §8, n$^o4$, p. $140.*$

Trước hết hãy chứng minh rằng (i) kéo theo (ii) và (v). Giả sử rằng vành A là nửa đơn, và xét một A-môđun trái M. Theo giả thiết, A-môđun $A_s$ là nửa đơn, nên mọi A-môđun tự do đều là nửa đơn. Theo Mệnh đề 20 của II, §1, No. 11, p. 218, tồn tại một A-môđun tự do L và một ánh xạ A-tuyến tính toàn ánh $u$ từ L lên M. Gọi N là hạt nhân của $u$. Vì A-môđun L là nửa đơn, nên tồn tại một môđun con nửa đơn $N'$ bù cho N trong L (VIII, p. 56, Định lý 1). A-môđun $N'$ là xạ ảnh, và $u$ cảm sinh một đẳng cấu từ $N'$ lên M. Do đó, M là nửa đơn và xạ ảnh.

(ii) $\Rightarrow$ (iii): Nếu mọi A-môđun đều là nửa đơn, thì A-môđun $A_s$ là nửa đơn; hơn nữa nó còn sinh.

(iii) $\Rightarrow$ (iv): Nếu M là một A-môđun sinh, thì nó trung thành (VIII, p. 80, Hệ quả của Định lý 1), và môđun đối của nó sinh hữu hạn (VIII, p. 99, Hệ quả 1).

(iv) $\Rightarrow$ (i): Cho M là một A-môđun trung thành và nửa đơn có môđun đối sinh hữu hạn. Theo Bổ đề 4 của VIII, p. 8, tồn tại một số tự nhiên $m$ sao cho $A_s$ đẳng cấu với một môđun con của $M^m$. A-môđun $M^m$ là nửa đơn, và do đó $A_s$ cũng vậy.

Suy ra (v) $\Rightarrow$ (vi) là ngay lập tức.

(vi) $\Rightarrow$ (i): Giả sử rằng mọi A-môđun đơn sinh đều xạ ảnh. Gọi $\mathfrak{a}$ là một iđêan trái của A. Vì A-môđun $A_s/\mathfrak{a}$ là xạ ảnh, tồn tại một iđêan trái $\mathfrak{b}$ của A sao cho $A_s$ là tổng trực tiếp của $\mathfrak{a}$ và $\mathfrak{b}$ (II, §2, No. 2, p. 231, Mệnh đề 4). Do đó, vành A là nửa đơn (VIII, p. 135, Định lý 1).

#### Bổ đề 1 {#alg-viii-s8-lem-1 .statement tag=009B}

Cho A là một vành Artin trái, và gọi M là một A-môđun đơn. Khi đó vành $A_M$ là đơn.

Vì vành A là Artin trái nên điều đó cũng đúng đối với vành $A_M$, theo Mệnh đề 5 của VIII, p. 7. Bây giờ, M là một $A_M$-môđun trung thành và đơn, nên vành $A_M$ là đơn (VIII, p. 119, Mệnh đề 1).

#### Mệnh đề 5 {#alg-viii-s8-prop-5 .statement tag=009C}

Giả sử vành A là nửa đơn. Cho M là một A-môđun trái. Môđun đối của M là sinh hữu hạn, và ta có $A_M= A''_M$.

Trước hết xét trường hợp M là một A-môđun đơn. Theo Bổ đề 1, vành $A_M$ là đơn. Khi đó Mệnh đề 5 suy ra từ Bổ đề 1 của VIII, p. 120.

Bây giờ xét trường hợp tổng quát. Tập hợp $\mathscr{S}$ các lớp của các A-môđun đơn là hữu hạn (VIII, p. 136, Mệnh đề 1). Với mỗi $\lambda \in \mathscr{S}$, chọn một A-môđun $S_{\lambda}$ thuộc lớp $\lambda$, và ký hiệu trường đối của hoán tập của $S_{\lambda}$ là $D_{\lambda}$. Theo Bổ đề 1 áp dụng cho vành đơn $A_{S_{\lambda}}, S_{\lambda}$ là một không gian vectơ hữu hạn chiều trên trường $D_{\lambda}$; ký hiệu chiều của nó là $m(\lambda )$. Gọi B là vành đối của vành các tự đồng cấu của M. Ta đã thấy ở VIII, p. 84 rằng tồn tại các $(D_{\lambda}$, B)-song môđun $V_{\lambda}$ đơn như các B-môđun và một đẳng cấu các $(A$, B)-song môđun từ M tới $\oplus_{\lambda\in\mathscr{S}}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$. Như một B-môđun, M đẳng cấu với $\oplus_{\lambda\in\mathscr{S}}V^{m(\lambda)}_{\lambda}$. Vì $\mathscr{S}$ và các $m(\lambda )$ là hữu hạn, M là một B-môđun sinh hữu hạn.

A-môđun M là nửa đơn, và môđun đối của nó sinh hữu hạn. Vậy ta có $A_M= A''_M$ theo Mệnh đề 4 của VIII, p. 83.

#### Mệnh đề 6 {#alg-viii-s8-prop-6 .statement tag=009D}

Cho M là một A-môđun nửa đơn sinh hữu hạn. Ký hiệu giá của nó (VIII, p. 66) là $\mathscr{S}_M$ và vành tự đồng cấu của nó là B. Với mọi $\lambda \in \mathscr{S}_M$, chọn một A-môđun đơn $S_{\lambda}$ thuộc lớp $\lambda$, và ký hiệu B-môđun trái Hom$_A(S_{\lambda},M)$ là $V_{\lambda}$.

a) Vành B là nửa đơn.

b) Ánh xạ $\lambda \mapsto$ cl(V$_{\lambda}$) là một song ánh từ giá $\mathscr{S}_M$ của M lên tập hợp các lớp của các B-môđun đơn.

c) Với mọi $\lambda \in \mathscr{S}_M$, thành phần đẳng kiểu kiểu $\lambda$ của A-môđun M bằng thành phần đẳng kiểu kiểu $V_{\lambda}$ của B-môđun M.

Được xem như một B-môđun, M là nửa đơn (VIII, p. 85, Mệnh đề 5) và trung thành. Môđun đối của nó là sinh hữu hạn vì ta có $A_M\subset$ End$_B(M)$. Do đó, vành B là nửa đơn (Mệnh đề 4). Nếu $(x_1, . . . , x_r)$ là một dãy sinh của A-môđun M, thì ánh xạ $b\mapsto (bx_1, . . . , bx_r)$ từ $B_s$ vào $M^r$ là B-tuyến tính và đơn ánh. Mọi B-môđun đơn đều đẳng cấu với một môđun con của $B_s$ (VIII, p. 136, Mệnh đề 1), do đó với một B-môđun con của M. Khi đó mệnh đề suy ra ngay lập tức từ Mệnh đề 5 của VIII, p. 85.

#### Mệnh đề 7 {#alg-viii-s8-prop-7 .statement tag=009E}

Cho A là một vành nửa đơn.

a) Mọi A-môđun hữu hạn sinh đều phản xạ (II, §2, No. 7, p. 239).

b) Với mọi A-môđun trái đơn S, A-môđun phải đối ngẫu $S^*$ của S là đơn, và ánh xạ $\lambda \mapsto$ cl($\lambda^*$) xác định một song ánh từ tập hợp các lớp của các A-môđun đơn lên tập hợp các lớp của các A-môđun phải đơn.

c) Cho M là một A-môđun trái hữu hạn sinh. A-môđun phải đối ngẫu $M^*$ của M là sinh hữu hạn và có cùng độ dài như M. Hơn nữa, ta có $[M : S] = [M^*: S^*]$ với mọi A-môđun đơn S.

Cho M là một A-môđun hữu hạn sinh.

Theo Mệnh đề 4 của VIII, p. 138, A-môđun M là sinh hữu hạn và xạ ảnh; do đó nó phản xạ theo Hệ quả 4 của II, §2, No. 7, p. 240. Đặc biệt, mọi A-môđun đơn đều phản xạ. Cũng suy ra rằng hai môđun trái hữu hạn sinh là đẳng cấu khi và chỉ khi các đối ngẫu của chúng là đẳng cấu.

Cho S là một A-môđun trái đơn. Cho $(T_i)_{i\in I}$ là một họ các A-môđun phải đơn có tổng trực tiếp là đối ngẫu $S^*$ của S. Vì S là phản xạ, nó đẳng cấu với $(S^*)^*$ và do đó với $\prod_{i\in I}T^*_i$. Mỗi môđun $T_i$ đều phản xạ; đặc biệt, ta có $T^*_i\not= 0$ với mọi $i\in I$. Vì môđun đơn S đẳng cấu với $\prod_{i\in I}T^*_i$, tập hợp I chỉ có một phần tử, nên $S^*$ là đơn.

Vì M là nửa đơn và sinh hữu hạn, nó là tổng trực tiếp của các môđun con đơn $S_1, . . . ,S_r$. Khi đó $M^*$ đẳng cấu với tổng trực tiếp của họ $S^*_1, . . . ,S^*_r$, và ta vừa thấy rằng các môđun $S^*_i$ là đơn. Mệnh đề c) suy ra ngay lập tức.

### 3. Các nhân tử của một vành nửa đơn

Trong tiểu mục này, ta xét một vành nửa đơn A.

Ta ký hiệu tập hợp các lớp của các A-môđun đơn trái bởi $\mathscr{S}$ (VIII, p. 51); nó là hữu hạn (VIII, p. 136, Mệnh đề 1). Với mọi $\lambda \in \mathscr{S}$, ta chọn một A-môđun đơn $S_{\lambda}$ thuộc lớp $\lambda$. Ta ký hiệu linh hóa tử của nó bởi $\mathfrak{b}_{\lambda}$ và trường đối của hoán tập End$_A(S_{\lambda})$ của nó bởi $D_{\lambda}$.

#### Mệnh đề 8 {#alg-viii-s8-prop-8 .statement tag=009F}

a) Với mọi $\lambda \in \mathscr{S},S_{\lambda}$ là một không gian vectơ phải hữu hạn chiều trên trường $D_{\lambda}$. Khi chuyển qua thương, ánh xạ $a\mapsto a_{S_{\lambda}}$ xác định một đẳng cấu vành từ $A/\mathfrak{b}_{\lambda}$ lên End$_{D_{\lambda}}(S_{\lambda})$.

b) Với mọi $\lambda \in \mathscr{S}$, vành $A/\mathfrak{b}_{\lambda}$ là đơn, và đồng cấu chính tắc $\psi$ từ A đến $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ là một đẳng cấu vành.

Vành $A/\mathfrak{b}_{\lambda}$ đẳng cấu với $A_{S_{\lambda}}$. Theo Bổ đề 1 của VIII, p. 139, vành này là đơn. Ánh xạ đã cho từ $A/\mathfrak{b}_{\lambda}$ đến End$_{D_{\lambda}}(S_{\lambda})$ có thể được đồng nhất với ánh xạ từ $A_{S_{\lambda}}$ đến $A''_{S_{\lambda}}$. Theo Mệnh đề 5 của VIII, p. 139, đó là một đẳng cấu.

A-môđun $A_s$ là nửa đơn, trung thành và cân bằng. Đồng cấu $\psi$ có thể được đồng nhất với cấu xạ từ đối giao hoán tử kép của $A_s$ đến $\prod_{\lambda\in\mathscr{S}}$ End$_{D_{\lambda}}(S_{\lambda})$, cấu xạ này là một đẳng cấu (VIII, p. 86, Mệnh đề 7, c)).

Vành đơn $A/\mathfrak{b}_{\lambda}$ được gọi là thừa số đơn của A kiểu $\lambda$.

#### Ví dụ {#alg-viii-s8-n3-exa-1 .statement tag=009G}

Cho K là một trường giao hoán đóng đại số, và cho A là một đại số nửa đơn bậc hữu hạn trên K. Cho $(V_i)_{i\in I}$ là một họ các A-môđun đơn sao cho mọi A-môđun đơn đều đẳng cấu với một $V_i$ duy nhất. Khi đó I là một tập hợp hữu hạn (VIII, p. 136, Mệnh đề 1), các không gian vectơ $V_i$ là hữu hạn chiều trên trường K, hoán tập của $V_i$ bằng $K\cdot 1_{V_i}$ (VIII, p. 47, Định lý 1), và ánh xạ $a\mapsto (a_{V_i})_{i\in I}$ là một đẳng cấu đại số từ A lên $\prod_{i\in I}$ End$_K(V_i)$ (Mệnh đề 8).

Chúng tôi đã định nghĩa (VIII, p. 50) một iđêan hai phía tối tiểu là một phần tử cực tiểu của tập hợp các iđêan hai phía khác không, có thứ tự theo bao hàm. Nói cách khác, một iđêan hai phía tối tiểu $\mathfrak{a}$ của A là một môđun con song đơn $(A$, A) của $_sA_d$. Tương tự, chúng tôi định nghĩa một iđêan hai phía tối đại của A là một phần tử cực đại của tập hợp các iđêan hai phía thực sự của A. Một iđêan hai phía tối đại $\mathfrak{a}$ của A đơn giản là một môđun con song $(A$, A) cực đại của $_sA_d$ (VIII, p. 48, Định nghĩa 2). Nếu vành A là đơn, thì iđêan 0 là một iđêan hai phía tối đại của A và A là một iđêan hai phía tối tiểu.

Với mọi $\lambda \in \mathscr{S}$, ta ký hiệu thành phần đẳng kiểu kiểu $\lambda$ của A-môđun $A_s$ bởi $\mathfrak{a}_{\lambda}$. Với mọi tập con Λ của $\mathscr{S}$, ta đặt $\mathfrak{a}_{\Lambda}=\sum_{\lambda\in\Lambda}\mathfrak{a}_{\lambda}$.

#### Mệnh đề 9 {#alg-viii-s8-prop-9 .statement tag=009H}

a) Sắp thứ tự tập hợp $\mathfrak{P}(\mathscr{S})$ các tập con của $\mathscr{S}$ và tập hợp $\mathscr{B}_A$ các iđêan hai phía của A theo bao hàm. Ánh xạ $\Lambda \mapsto \mathfrak{a}_{\Lambda}$ là một đẳng cấu của các tập hợp có thứ tự từ $\mathfrak{P}(\mathscr{S})$ đến $\mathscr{B}_A$.

b) Các iđêan hai phía cực tiểu của A là các iđêan $\mathfrak{a}_{\lambda}$.

c) Ta có $\mathfrak{b}_{\lambda}=\mathfrak{a}_{\mathscr{S}-\{\lambda\}}$ với mọi $\lambda \in \mathscr{S}$, và các iđêan $\mathfrak{b}_{\lambda}$ là các iđêan hai phía cực đại của A.

d) Với mọi $\lambda \in \mathscr{S}$, ánh xạ chính tắc từ A đến $A/\mathfrak{b}_{\lambda}$ cảm sinh một đẳng cấu A-môđun từ $\mathfrak{a}_{\lambda}$ đến $A/\mathfrak{b}_{\lambda}$.

Mệnh đề a) suy ra từ Mệnh đề 8, d) của VIII, p. 87 khi áp dụng cho A-môđun $A_s$. Suy ra rằng các iđêan hai phía cực tiểu của A là các $\mathfrak{a}_{\lambda}$ và các iđêan hai phía cực đại là các iđêan $\mathfrak{c}_{\lambda}=\mathfrak{a}_{\mathscr{S}-\lambda}$ (với $\lambda \in \mathscr{S}$).

Còn phải chứng minh đẳng thức của $\mathfrak{b}_{\lambda}$ và $\mathfrak{c}_{\lambda}$ với mọi $\lambda \in \mathscr{S}$. Cho $\lambda$ và $\mu$ phân biệt trong $\mathscr{S}$. A-môđun con $\mathfrak{a}_\mu S_{\lambda}$ của $S_{\lambda}$ là hợp của các ảnh của các ánh xạ tuyến tính $a\mapsto ax$ từ $\mathfrak{a}_\mu$ đến $S_{\lambda}$ với $x\in S_{\lambda}$. Do đó, nó bằng không, và ta có $\mathfrak{a}_\mu\subset \mathfrak{b}_{\lambda}$. Vì thế ta có $\mathfrak{c}_{\lambda}\subset \mathfrak{b}_{\lambda}$, và cuối cùng $\mathfrak{c}_{\lambda}=\mathfrak{b}_{\lambda}$ vì $\mathfrak{c}_{\lambda}$ là một ideal hai phía tối đại của A và $\mathfrak{b}_{\lambda}$ phân biệt với A.

#### Hệ quả {#alg-viii-s8-n3-cor-1 .statement tag=009I}

Cho $(A_i)_{i\in I}$ là một họ hữu hạn các vành đơn và $f$ là một đẳng cấu từ A lên $\prod_{i\in I}A_i$. Với mọi $i\in I$, tồn tại một phần tử duy nhất $\varphi (i)$ của $\mathscr{S}$ sao cho hạt nhân của pr$_i\circ f$ là $\mathfrak{b}_{\varphi(i)}$. Ánh xạ $\varphi$ là một song ánh từ I lên $\mathscr{S}$; ánh xạ pr$_i\circ f$ cảm sinh một đẳng cấu $f_i$ từ $A/\mathfrak{b}_{\varphi(i)}$ lên $A_i$ với mọi $i\in I$.

Do đó, $f$ là hợp thành của đẳng cấu chính tắc từ A đến $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ và đẳng cấu từ $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ đến $\prod_{i\in I}A_i$ suy ra từ các $f_i($“tính duy nhất của phân tích một vành nửa đơn thành một tích các vành đơn”).

Ta chứng minh hệ quả. Cho $i\in I$; ký hiệu hạt nhân của pr$_i\circ f$ là $\mathfrak{b}'_i$. Vì vành đơn $A_i$ đẳng cấu với $A/\mathfrak{b}'_i$, iđêan hai phía $\mathfrak{b}'_i$ của A là cực đại. Theo Mệnh đề 8, c), do đó tồn tại một phần tử duy nhất $\varphi (i)$ của $\mathscr{S}$ sao cho ta có $\mathfrak{b}'_i=\mathfrak{b}_{\varphi(i)}$. Khi chuyển qua thương, pr$_i\circ f$ xác định một đẳng cấu $f_i$ từ $A/\mathfrak{b}_{\varphi(i)}$ đến $A_i$. Hơn nữa, ta có $\mathfrak{b}'_i+\mathfrak{b}'_j= A$ nếu $i\not=j$ và $\cap_{i\in I}\mathfrak{b}'_i= 0$ (x. I, §8, No. 11, p. 110, Mệnh đề 10). Từ điều này và Mệnh đề 8 suy ra rằng $\varphi$ là một song ánh từ I đến $\mathscr{S}$.

#### Mệnh đề 10 {#alg-viii-s8-prop-10 .statement tag=009J}

Ký hiệu tâm của A là Z. Với $\lambda \in \mathscr{S}$, gọi $Z_{\lambda}$ là tâm của trường $D_{\lambda}$.

a) Ánh xạ $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}}$ là một đẳng cấu từ vành Z lên tích $\prod_{\lambda\in\mathscr{S}}Z_{\lambda}$.

b) Sắp thứ tự tập hợp $\mathscr{I}_Z$ các iđêan của Z và tập hợp $\mathscr{B}_A$ các iđêan hai phía của A theo quan hệ bao hàm. Ánh xạ $\mathfrak{a}\mapsto \mathfrak{a}A$ là một đẳng cấu của các tập hợp có thứ tự từ $\mathscr{I}_Z$ lên $\mathscr{B}_A$. Đẳng cấu nghịch đảo biến một iđêan hai phía $\mathfrak{b}$ của A thành iđêan $\mathfrak{b}\cap Z$ của Z.

Mệnh đề này suy ra từ Mệnh đề 8 của VIII, p. 87 áp dụng cho A-môđun $A_s$, mà đối giao hoán tử kép của nó là A.

#### Hệ quả {#alg-viii-s8-n3-cor-2 .statement tag=009K}

Cho B là một vành. Các tính chất sau là tương đương:

(i) Vành B là đơn.

(ii) Vành B là nửa đơn, và tâm của nó là một trường.

(iii) Vành B là nửa đơn, và chỉ tồn tại một lớp các môđun đơn trên B.

#### Mệnh đề 11 {#alg-viii-s8-prop-11 .statement tag=009L}

Cho $\lambda \in \mathscr{S}$. Thành phần đẳng kiểu $\mathfrak{a}_{\lambda}$ của A vừa là thành phần đẳng kiểu của $A_s$ thuộc kiểu $S_{\lambda}$ vừa là thành phần đẳng kiểu của $A_d$ thuộc kiểu $S^*_{\lambda}$. Hơn nữa, ta có

(1) $[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}] =$ dim$_{D_{\lambda}}S_{\lambda}$

và

(2) long(A) = long(A$^o$) $=\sum_{\lambda\in\mathscr{S}}$ dim$_{D_{\lambda}}S_{\lambda}$.

Mệnh đề thứ nhất là trường hợp riêng $M = A_s$ của Mệnh đề 6, c) của VIII, p. 139. Đẳng thức $[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}]$ suy ra từ Mệnh đề 7 của VIII, p. 140 vì đối ngẫu của A-môđun trái $A_s$ đẳng cấu với A-môđun phải $A_d$. Theo các Mệnh đề 8, a) và 9, c), ánh xạ $a\mapsto a_{S_{\lambda}}$ xác định một đẳng cấu các A-môđun trái từ $\mathfrak{a}_{\lambda}$ lên End$_{D_{\lambda}}(S_{\lambda})$. Vì $[A_s: S_{\lambda}]$, theo định nghĩa, là độ dài của A-môđun trái $\mathfrak{a}_{\lambda}$, quan hệ $[A_s: S_{\lambda}] =$ dim$_{D_{\lambda}}S_{\lambda}$ suy ra từ Bổ đề 2 của VIII, p. 121. Sau cùng, quan hệ (2) nhận được từ (1) bằng cách lấy tổng theo $\lambda$.

#### Chú giải {#alg-viii-s8-n3-sch-1 .statement tag=009M}

Cho A là một vành nửa đơn và Z là tâm của nó. Có những song ánh chính tắc giữa các tập hợp sau đây:

a) Tập hợp $\mathscr{S}(A)$ các lớp các A-môđun trái đơn

b) Tập hợp $\mathscr{S}(A^o)$ các lớp các A-môđun phải đơn

c) Tập hợp các iđêan hai phía cực tiểu của A

d) Tập hợp các iđêan hai phía cực đại của A

e) Tập hợp $\mathscr{S}(Z)$ các lớp các Z-môđun đơn

f) Tập hợp các iđêan cực tiểu của Z

g) Tập hợp các iđêan cực đại của Z.

Vậy, với mỗi phần tử $\lambda$ của $\mathscr{S}$ (A), tương ứng lớp $\lambda^*$ của A-môđun phải đơn $S^*_{\lambda}$, đối ngẫu của $S_{\lambda}$, iđêan hai phía tối tiểu $\mathfrak{a}_{\lambda}$ của A (thành phần đẳng kiểu của $A_s$ kiểu $\lambda$ ), iđêan hai phía tối đại $\mathfrak{b}_{\lambda}$ của A (linh hóa tử của môđun đơn $S_{\lambda}$), lớp của Z-môđun đơn $Z\cap \mathfrak{a}_{\lambda}$, ideal tối tiểu $Z\cap \mathfrak{a}_{\lambda}$ của Z, và iđêan cực đại $Z\cap \mathfrak{b}_{\lambda}$ của Z.

#### Mệnh đề 12 {#alg-viii-s8-prop-12 .statement tag=009N}

Cho M là một môđun trên vành nửa đơn A và $\mathscr{S}_M\subset \mathscr{S}$ là giá của M. Khi đó linh hóa tử Ann(M) của M là iđêan hai phía $\sum_{\lambda\in\mathscr{S}-\mathscr{S}_M}\mathfrak{a}_{\lambda}$, và iđêan vết $\tau (M)$ của M là iđêan hai phía $\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}$. Đặc biệt, A là tổng trực tiếp của Ann(M) và $\tau (M)$.

Theo định nghĩa (VIII, p. 84)$,\mathscr{S}_M$ gồm các lớp của các môđun con đơn của M. Vì môđun M là nửa đơn, linh hóa tử của M là giao của các linh hóa tử $\mathfrak{b}_{\lambda}$ của các môđun thuộc lớp $\lambda$, với $\lambda$ chạy qua $\mathscr{S}_M$. Mặt khác, ta có $\mathfrak{b}_{\lambda}=\sum_{\mu\not=\lambda}\mathfrak{a}_\mu$ với mọi $\lambda \in \mathscr{S}$ (Mệnh đề 9). Vì A là tổng trực tiếp của họ $(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$, nên linh hóa tử của M quả thật bằng $\sum_{\lambda\in\mathscr{S}-\mathscr{S}_M}\mathfrak{a}_{\lambda}$.

Theo định nghĩa (VIII, p. 80), iđêan vết $\tau (M)$ là A-môđun con của $A_s$ được sinh bởi các ảnh của các ánh xạ A-tuyến tính từ M vào $A_s$. Vì M là nửa đơn, nói rằng iđêan $\tau (M)$ được sinh bởi các môđun con đơn của $A_s$ có lớp thuộc $\mathscr{S}_M$ cũng là tương đương. Do đó ta có $\tau (M) =\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}$.

#### Hệ quả {#alg-viii-s8-n3-cor-3 .statement tag=009O}

Cho M là một môđun trên vành nửa đơn A. Các tính chất sau là tương đương:

(i) A-môđun M là trung thành.

(ii) Giá của M bằng $\mathscr{S}$.

(iii) A-môđun M là sinh.

Thật vậy, nói rằng M là trung thành có nghĩa là linh hóa tử của nó thu về 0, và M là sinh khi và chỉ khi vết của nó bằng A (VIII, p. 80, Định lý 1).

### 4. Các phần tử lũy đẳng và các vành nửa đơn

Cho A là một vành. Nhắc lại rằng một phần tử $e$ của A được gọi là lũy đẳng (I, §1, No. 4, p. 7) nếu ta có $e^2=e$. Khi đó nó cũng là một phần tử lũy đẳng của vành đối $A^o$ của A.

#### Mệnh đề 13 {#alg-viii-s8-prop-13 .statement tag=009P}

a) Một iđêan trái $\mathfrak{a}$ của A có một phần bù trong $A_s$ nếu và chỉ nếu tồn tại một phần tử lũy đẳng $e$ trong A sao cho $\mathfrak{a}= Ae$. Khi đó iđêan $\mathfrak{a}$ gồm các phần tử $x$ của A sao cho $x=xe$.

b) Cho $e$ và $f$ là các phần tử lũy đẳng trong A. Ta có $Ae\subset Af$ nếu và chỉ nếu có $ef=e$.

c) Cho M là một A-môđun. Khi đó M là xạ ảnh và đơn sinh nếu và chỉ nếu tồn tại một phần tử lũy đẳng $e$ trong A sao cho M đẳng cấu với $Ae$.

Các nội cấu của A-môđun $A_s$ là các phép nhân bên phải bởi các phần tử của A. Do đó các phép chiếu trong A-môđun $A_s$ là các ánh xạ $x\mapsto xe$ trong đó $e$ là một phần tử lũy đẳng của A. Hơn nữa, các môđun con của $A_s$ là các iđêan trái, và một môđun con như vậy thừa nhận một phần bù khi và chỉ khi nó là ảnh của một phép chiếu (II, §1, No. 9, p. 211, Mệnh đề 14). Mệnh đề a) suy ra.

Quan hệ $Ae\subset Af$ tương đương với $e\in Af$. Theo a), vì thế nó tương đương với $e=ef$; mệnh đề b) suy ra.

Nếu A-môđun M là đơn sinh, thì tồn tại một ánh xạ A-tuyến tính toàn ánh $u: A_s\rightarrow M$. Nếu hơn nữa M là xạ ảnh, thì tồn tại một môđun con $\mathfrak{a}$ của $A_s$ bù với hạt nhân của $u$. Khi đó $u$ cảm sinh một đẳng cấu từ $\mathfrak{a}$ lên M. Ngược lại, nếu M đẳng cấu với một nhân tử trực tiếp của $A_s$, thì nó đơn sinh và xạ ảnh. Do đó mệnh đề c) suy ra từ a).

#### Nhận xét 1 {#alg-viii-s8-n4-rem-1 .statement tag=009Q}

Cho $\mathfrak{a}$ là một iđêan trái của A. Theo chứng minh ở trên và hệ quả của Mệnh đề 12 của II, §1, No. 8, p. 209, ánh xạ $e\mapsto A(1-e)$ xác định một song ánh từ tập hợp các phần tử lũy đẳng $e$ trong A sao cho $\mathfrak{a}= Ae$ lên tập hợp các iđêan trái $\mathfrak{b}$ của A sao cho $A_s=\mathfrak{a}\oplus \mathfrak{b}$.

#### Nhận xét 2 {#alg-viii-s8-n4-rem-2 .statement tag=009R}

Cho $e$ và $f$ là các phần tử lũy đẳng trong A. Theo Mệnh đề 13, b), ta có $Ae= Af$ khi và chỉ khi $ef=e$ và $f e=f$. Do đó, nếu vành A là giao hoán, thì quan hệ $Ae= Af$ tương đương với $e=f$. Điều này nói chung không đúng, như ví dụ $A =\mathbf{M}_2(\mathbf{Z}), e = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$, và $f = \begin{pmatrix} 1 & 0 \\ 1 & 0 \end{pmatrix}$ cho thấy.

Ta nói rằng các phần tử lũy đẳng $e$ và $e'$ trong vành A là trực giao nếu $ee'=$ $e'e= 0$. Cho $(e_i)_{i\in I}$ là một họ hữu hạn các phần tử lũy đẳng trực giao từng đôi một trong A. Vì ta có

$$
(\sum_ie_i)^2=\sum_ie^2_i+\sum_{i\not=j}e_ie_j=\sum_ie_i
$$

nên phần tử $\sum_{i\in I}e_i$ của A là lũy đẳng.

Một phân hoạch của một phần tử lũy đẳng $e$ trong A là một họ hữu hạn $(e_i)_{i\in I}$ các phần tử lũy đẳng trực giao từng đôi một trong A sao cho $e=\sum_{i\in I}e_i$. Ta nói rằng một phần tử lũy đẳng $e$ trong A là phân tích được nếu tồn tại một phân hoạch của $e$ gồm các phần tử lũy đẳng trực giao từng đôi một khác 0 và khác $e$; trong trường hợp đối lại, ta nói rằng nó là không phân tích được. Hãy nhận thấy rằng 0 là một phần tử lũy đẳng phân tích được.

#### Mệnh đề 14 {#alg-viii-s8-prop-14 .statement tag=009S}

Cho $e$ là một phần tử lũy đẳng trong A.

a) Nếu $(e_i)_{i\in I}$ là một phân hoạch của $e$, thì A-môđun $Ae$ là tổng trực tiếp của họ $(Ae_i)_{i\in I}$.

b) Cho $(\mathfrak{a}_i)_{i\in I}$ là một họ hữu hạn các iđêan trái của A có tổng trực tiếp là $Ae$. Với $i\in I$, kí hiệu thành phần của $e$ trong $\mathfrak{a}_i$ là $e_i$. Khi đó $(e_i)_{i\in I}$ là một phân hoạch của $e$, và ta có $\mathfrak{a}_i= Ae_i$ với mọi $i\in I$.

c) A-môđun $Ae$ là không phân tích được khi và chỉ khi phần tử lũy đẳng $e$ là không phân tích được.

Cho $(e_i)_{i\in I}$ là một phân hoạch của $e$. Với mọi $i\in I$, ta có

$$
e_ie=\sum_je_ie_j=e^2_i+\sum_{j\not=i}e_ie_j=e_i
$$

và do đó $Ae_i\subset Ae$. Với mọi $i\in I$, ta định nghĩa một phép chiếu A-tuyến tính $p_i$ trong $Ae$ bằng cách đặt $p_i(x) =xe_i$. Ta có $p_ip_j= 0$ nếu $i\not=j$, và với mọi $x$ trong $Ae$,

$$
x=xe=\sum_ixe_i=\sum_ip_i(x)
$$

Do đó (II, §1, No. 8, p. 20, Mệnh đề $12$)$, Ae$ là tổng trực tiếp của các ảnh của các $p_i$. Bây giờ, ta có $ee_i=e_ie=e_i$, nên ảnh của $p_i$ là $Ae_i$. Điều này chứng minh a).

Lấy các ký hiệu và giả thiết của b). Cho $i\in I$. Vì $e_i$ thuộc $Ae$, ta có $e_i=e_ie=\sum_je_ie_j$. Vì $Ae$ là tổng trực tiếp của các $\mathfrak{a}_j$ và $e_ie_j$ thuộc $\mathfrak{a}_j$ với mọi $j$, ta có $e_i=e_ie_i$ và $e_ie_j= 0$ đối với $i\not=j$. Nói cách khác, $(e_i)_{i\in I}$ là một phân hoạch của phần tử lũy đẳng $e$. Theo a), $Ae$ là tổng trực tiếp của các $Ae_i$. Theo giả thiết, ta có $Ae_i\subset \mathfrak{a}_i$, và $Ae$ là tổng trực tiếp của các $\mathfrak{a}_i$. Do đó ta có $Ae_i=\mathfrak{a}_i$ với mọi $i\in I$. Ta đã chứng minh b).

Cuối cùng, c) suy ra ngay lập tức từ a) và b).

#### Nhận xét 3 {#alg-viii-s8-n4-rem-3 .statement tag=00R8}

Áp dụng các kết quả trước đó cho vành đối của A, ta thấy, đặc biệt, rằng một A-môđun phải đơn sinh M là xạ ảnh khi và chỉ khi tồn tại một lũy đẳng $e$ trong A sao cho M đẳng cấu với $eA$. Hơn nữa, $eA$ là một môđun phải không phân tích được khi và chỉ khi $e$ không phân tích được.

Bây giờ giả sử rằng vành A là nửa đơn, và ký hiệu tập hợp các lớp của các A-môđun trái đơn bởi $\mathscr{S}$. A-môđun $A_s$ là nửa đơn, và mọi môđun con của $A_s$ là một nhân tử trực tiếp. Cho $\mathfrak{a}$ là một iđêan trái của A. Theo trên, tồn tại một lũy đẳng $e$ trong A sao cho $\mathfrak{a}= Ae$, và A-môđun $\mathfrak{a}$ là đơn khi và chỉ khi nó không phân tích được, nghĩa là, khi và chỉ khi $e$ không phân tích được.

Cho $(\mathfrak{m}_i)_{i\in I}$ là một họ các iđêan trái cực tiểu của A sao cho ta có $A_s=\oplus_{i\in I}\mathfrak{m}_i$. Theo Mệnh đề 14, tồn tại một phân hoạch $(\varepsilon_i)_{i\in I}$ của 1 gồm các phần tử lũy đẳng không phân tích được sao cho $\mathfrak{m}_i= A\varepsilon_i$ với mọi $i\in I$.

Với mọi $\lambda \in \mathscr{S}$, gọi $S_{\lambda}$ là một A-môđun thuộc lớp $\lambda$, và gọi $\mathfrak{a}_{\lambda}$ là thành phần đẳng kiểu kiểu $\lambda$ của A-môđun $A_s$. Vì A là tổng trực tiếp của họ $(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$, nên tồn tại một phân hoạch $(e_{\lambda})_{\lambda\in\mathscr{S}}$ của 1 sao cho $\mathfrak{a}_{\lambda}= Ae_{\lambda}$ với mọi $\lambda \in \mathscr{S}$. Với $\lambda \in \mathscr{S}$, ký hiệu $I(\lambda )$ là tập hợp các chỉ số $i\in I$ sao cho A-môđun đơn $\mathfrak{m}_i$ thuộc kiểu $\lambda$. Theo Mệnh đề 4, b) của VIII, p. 65, ta có

$$
\mathfrak{a}_{\lambda}=\bigoplus_{i\in I(\lambda)}\mathfrak{m}_i \tag{3}
$$

Phần tử lũy đẳng $e_{\lambda}$ là thành phần của 1 trong $\mathfrak{a}_{\lambda}$, nên $e_{\lambda}=\sum_{i\in I(\lambda)}\varepsilon_i$.

#### Mệnh đề 15 {#alg-viii-s8-prop-15 .statement tag=009T}

Giả sử rằng vành A là nửa đơn.

a) Với mọi $\lambda \in \mathscr{S},e_{\lambda}$ là phần tử duy nhất của tâm Z của A thỏa mãn các hệ thức $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ và $(e_{\lambda})_{S_\mu}= 0$ với $\mu\not=\lambda$.

b) Các phần tử lũy đẳng không phân tích được trong vành Z là các $e_{\lambda}$, và các iđêan cực tiểu của Z là các $Ze_{\lambda}$ với $\lambda \in \mathscr{S}$.

c) Cho M là một A-môđun và $(M_{\lambda})_{\lambda\in\mathscr{S}}$ là họ các thành phần đẳng kiểu của nó. Họ các phép chiếu liên kết với sự phân tích của M thành tổng trực tiếp của các $M_{\lambda}$ (VIII, p. 65) là $((e_{\lambda})_M)_{\lambda\in\mathscr{S}}$, và ta có $M_{\lambda}=\mathfrak{a}_{\lambda}M$ với mọi $\lambda \in \mathscr{S}$.

Cho $\lambda$ và $\mu$ phân biệt trong $\mathscr{S}$. Ta có $e_{\lambda}\in \mathfrak{a}_{\lambda}$, và $\mathfrak{a}_{\lambda}$ được chứa trong linh hóa tử $\mathfrak{b}_\mu$ của A-môđun $S_\mu$ (VIII, p. 142, Mệnh đề 9). Do đó ta có $(e_{\lambda})_{S_\mu}= 0$. Quan hệ $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ suy ra từ việc ta có $1 =\sum_{\nu\in\mathscr{S}}e_{\nu}$. Khi đó mệnh đề a) là một hệ quả của Mệnh đề 8 của VIII, p. 141.

Cho $\lambda$ thuộc $\mathscr{S}$. Iđêan hai phía $\mathfrak{a}_{\lambda}$ của A gồm các phần tử $x$ sao cho $x=xe_{\lambda}$; do đó ta có $Z\cap \mathfrak{a}_{\lambda}= Ze_{\lambda}$, và vì thế b) theo Mệnh đề 10, b).

Ta hãy chứng minh c). Cho $x$ là một phần tử của M. Ta có $e_{\lambda}\in \mathfrak{a}_{\lambda}$ với mọi $\lambda \in \mathscr{S}$. Vì ánh xạ $a\mapsto ax$ từ $A_s$ đến M là A-tuyến tính, nên ta có $\mathfrak{a}_{\lambda}x\subset M_{\lambda}$ (VIII, p. 66, Mệnh đề 5) và, đặc biệt, $e_{\lambda}x\in M_{\lambda}$. Ta có $1 =\sum_{\lambda\in\mathscr{S}}e_{\lambda}$, do đó $x=\sum_{\lambda\in\mathscr{S}}e_{\lambda}x$. Do đó, $e_{\lambda}x$ là thành phần của $x$ trong $M_{\lambda}$.

#### Nhận xét 4 {#alg-viii-s8-n4-rem-4 .statement tag=009U}

Giả sử rằng vành A là nửa đơn. Cho $(e_i)_{i\in I}$ là một phân hoạch của 1 gồm các phần tử lũy đẳng khác không trong tâm Z của A. Nếu Card(I) = Card($\mathscr{S}$), thì các $e_i$ là các phần tử lũy đẳng không phân tích được trong Z.

### Bài tập {#alg-viii-s8-exercises}

Xem [các bài tập cho § 8](exercises/s8/).
