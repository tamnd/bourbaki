---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 7
section_title: Simple Rings
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.119-A VIII.133
pdf_pages: 0136-0150
extraction: native
subsections:
    - "no": 1
      title: Simple Rings
      page: 119
      pdf_page: 136
    - "no": 2
      title: Modules over a Simple Ring
      page: 122
      pdf_page: 139
    - "no": 3
      title: Degrees
      page: 124
      pdf_page: 141
    - "no": 4
      title: Ideals of Simple Rings
      page: 126
      pdf_page: 143
statements: 24
exercises: 16
content_sha256: ce6c5e094cacb88fa60fb1652a895be75d4038f096f6516321ad03baa9d458fd
translated_from: content/en/alg/VIII/07_s7_simple_rings.md
source_content_sha256: 0477da2a1cd441904c225c6cad3222346fc38778e44066ddeda16e447e7b81dd
translation_model: gpt-5.4
translation_run: translate-vi-d30757fd
glossary_version: 34
glossary_terms_sha256: fed7d10bd233e763c14bb483e93a9b5d64d38fa73c27862583a2dc464ac24647
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. VÀNH ĐƠN

### 1. Vành đơn

#### Mệnh đề 1 {#alg-viii-s7-prop-1 .statement tag=0081}

Cho A là một vành khác không. Các điều kiện sau là tương đương:

(i) A-môđun $A_s$ là đẳng kiểu.

(ii) Vành A là Artin trái, và mọi iđêan hai phía của A đều bằng 0 hoặc A.

(iii) Vành A là Artin trái, và tồn tại một A-môđun trái S vừa đơn vừa trung thành.

Nếu các điều kiện ấy được thỏa mãn, thì A-môđun $A_s$ có độ dài hữu hạn và là đẳng kiểu kiểu S, và mọi A-môđun đơn đều đẳng cấu với S.

Ta chứng minh rằng (i) suy ra (ii). Giả sử (i) được thỏa mãn. Khi đó A-môđun hữu hạn sinh $A_s$ là nửa đơn, nên có độ dài hữu hạn và là Artin (VIII, p. 71, Mệnh đề 10); do đó vành A là Artin trái. Các nội đồng cấu của A-môđun trái $A_s$ là các phép nhân bên phải bởi các phần tử của A. Vì A-môđun trái $A_s$ là đẳng kiểu, theo Mệnh đề 6, b) của VIII, p. 86 suy ra song môđun $(A$, A) $_sA_d$ là đơn. Các môđun con song môđun của $_sA_d$ là các iđêan hai phía của A, nên (i) suy ra (ii).

Ta chứng minh rằng (ii) suy ra (iii). Vành A không thu về 0; do đó tồn tại một A-môđun đơn S. Linh hóa tử của S là một iđêan hai phía thực sự của A. Nếu giả sử (ii) được thỏa mãn, thì linh hóa tử ấy bằng 0. Khi đó A-môđun S là trung thành, và (ii) suy ra (iii).

Ta chứng minh rằng (iii) suy ra (i). Giả sử (iii) được thỏa mãn. Khi đó tồn tại một số nguyên $m\geqslant 1$ sao cho $A_s$ đẳng cấu với một môđun con của $S^m$ (VIII, p. 50, Mệnh đề 5, a)). Vì $S^m$ là một A-môđun đẳng kiểu kiểu S, nên điều ấy cũng đúng với $A_s$ (VIII, p. 61, Mệnh đề 2); do đó, (iii) suy ra (i).

Giả sử các điều kiện từ (i) đến (iii) được thỏa mãn. Ta đã thấy ở trên rằng A-môđun $A_s$ có độ dài hữu hạn và là đẳng kiểu kiểu S. Mọi A-môđun đơn trái đều đẳng cấu với một thương của $A_s$, nên đẳng cấu với S.

#### Định nghĩa 1 {#alg-viii-s7-def-1 .statement tag=0082}

Ta nói rằng một vành A là đơn nếu nó thỏa mãn các điều kiện tương đương (i), (ii) và (iii) của Mệnh đề 1. Cho K là một trường giao hoán; một đại số trên K được gọi là đơn nếu vành nền của nó là đơn.

#### Nhận xét 1 {#alg-viii-s7-n1-rem-1 .statement tag=0083}

Nhắc lại rằng theo Định lý 1 của II, §9, No. 1, p. 115, các tính chất sau là tương đương:

(i) A-môđun $A_s$ là đơn.

(ii) Vành A không bị thu về 0, và không có iđêan trái nào của A khác 0 hoặc A.

(iii) Vành A là một trường.

Do đó, theo Mệnh đề 1 (điều kiện (ii)), các vành đơn giao hoán không là gì khác ngoài các trường giao hoán.

#### Nhận xét 2 {#alg-viii-s7-n1-rem-2 .statement tag=0084}

Đôi khi ta nói rằng một vành A là gần đơn nếu nó không bị thu về 0 và nếu các iđêan hai phía duy nhất của nó là 0 và A. Ta nói rằng A là nguyên thủy nếu nó thừa nhận một môđun đơn trung thành. Theo Mệnh đề 1, mọi vành đơn đều là gần đơn. Vì mọi vành khác không đều thừa nhận một môđun đơn và linh hóa tử của một môđun đơn là một iđêan hai phía, ta thấy rằng mọi vành gần đơn đều là nguyên thủy. Tuy nhiên, tồn tại các vành gần đơn không đơn và các vành nguyên thủy không gần đơn (VIII, p. 128, Bài tập 2); các vành như thế không là Artin trái.

#### Định lý 1 (Wedderburn) {#alg-viii-s7-thm-1 .statement tag=00S3}

Một vành là đơn khi và chỉ khi nó đẳng cấu với một vành ma trận $\mathbf{M}_r(D)$, trong đó $r\geqslant 1$ là một số nguyên và D là một trường.

#### Bổ đề 1 {#alg-viii-s7-lem-1 .statement tag=0085}

Cho A là một vành đơn, S một A-môđun trái đơn, và D là vành đối của trường End$_A(S)$. Khi đó S là một song môđun $(A,D)$ khả nghịch. Nó cũng là một không gian vectơ phải hữu hạn chiều trên D, và ánh xạ $a\mapsto a_S$ là một đẳng cấu vành từ A lên End$_D(S)$.

Theo Mệnh đề 1, A-môđun $A_s$ có độ dài hữu hạn và đẳng kiểu kiểu S. Do đó, tồn tại một số nguyên $m\geqslant 1$ sao cho các A-môđun $A_s$ và $S^m$ là đẳng cấu. Khi đó A-môđun S là xạ ảnh và sinh hữu hạn. Nó sinh (VIII, p. 80, Định lý 1), và Bổ đề 1 suy ra từ Định lý 1 của VIII, p. 101, (ii)$\Rightarrow$(i) và (ii)$\Rightarrow$(iii) áp dụng cho song môđun $(A,D)_{\mathbf{Z}}$ S.

#### Bổ đề 2 {#alg-viii-s7-lem-2 .statement tag=00R7}

Cho D là một trường và V là một không gian vectơ phải trên D có số chiều hữu hạn $r\geqslant 1$. Khi đó V là một môđun đơn trên vành E = End$_D(V)$, và hoán tập của nó bằng $D_V$. Vành E là đơn, và độ dài trái của nó bằng $r$.

Ta biết rằng V là một E-môđun đơn (VIII, p. 45, Ví dụ 3) và hoán tập của nó bằng $D_V$ (VIII, p. 82, Hệ quả 1). Gọi $(x_i)_{1\leqslant i\leqslant r}$ là một cơ sở của V trên trường D. Ánh xạ $u\mapsto (u(x_i))_{1\leqslant i\leqslant r}$ là một đẳng cấu từ E-môđun $E_s$ tới E-môđun $V^r$; do đó, E-môđun $E_s$ là đẳng kiểu có độ dài $r$, nên vành E là đơn.

Bây giờ ta chứng minh Định lý 1. Nhắc lại rằng (II, §10, No. 7, p. 349) vành $\mathbf{M}_r(D)$ có thể được đồng nhất với vành tự đồng cấu của không gian vectơ phải trên D $D^r_d$; hơn nữa, mọi không gian vectơ phải có số chiều hữu hạn $r$ trên một trường D đều đẳng cấu với $D^r_d$ (II, §7, No. 1, p. 292). Do đó Định lý 1 suy ra từ Bổ đề 1 và 2.

#### Nhận xét 3 {#alg-viii-s7-n1-rem-3 .statement tag=0086}

Cho A là một vành đơn, S là một A-môđun đơn, và D là vành đối của trường End$_A(S)$. Khi đó A-môđun $A_s$ có độ dài hữu hạn, và dim$_D(S)$ bằng long(A). Thật vậy, theo Bổ đề 1, vành A đẳng cấu với End$_D(S)$; khi đó ta áp dụng Bổ đề 2.

#### Hệ quả 1 {#alg-viii-s7-lem-2-cor-1 .statement tag=0087}

a) Tâm của một vành đơn là một trường.

b) Vành đối của một vành đơn là đơn.

c) Độ dài trái của một vành đơn bằng độ dài phải của nó.

Cho D là một trường, Z là tâm của nó, và V là một không gian vectơ phải trên D có số chiều hữu hạn $r\geqslant 1$. Ta ký hiệu vành tự đồng cấu của V là E.

Ánh xạ $z\mapsto z_V$ là một đẳng cấu từ Z lên tâm của E theo Hệ quả 2 của VIII, p. 83. Mệnh đề a) suy ra từ đó. Đối ngẫu $V^*$ của V là một không gian vectơ phải trên trường đối $D^o$ của D, và chiều của nó bằng $r$. Ánh xạ $u\mapsto^tu$ là một đẳng cấu từ vành đối $E^o$ của E lên vành End$_{D^o}(V^*)$. Do đó, vành $E^o$ là đơn, và các vành E và $E^o$ có cùng độ dài trái, bằng $r$ (Bổ đề 2).

#### Hệ quả 2 {#alg-viii-s7-lem-2-cor-2 .statement tag=0088}

Cho $r$ và $r'$ là các số nguyên dương ngặt, và cho D và $D'$ là các trường. Các vành $\mathbf{M}_r(D)$ và $\mathbf{M}_{r'}(D')$ đẳng cấu khi và chỉ khi ta có $r=r'$ và các trường D và $D'$ đẳng cấu.

Điều kiện ấy hiển nhiên là đủ.

Ngược lại, giả sử rằng các vành $B =\mathbf{M}_r(D)$ và $B'=\mathbf{M}_{r'}(D')$ là đẳng cấu. Vì $r$ là độ dài của $B_s$ và $r'$ là độ dài của $B'_s$ (Bổ đề 2), ta có $r=r'$. Hơn nữa, B tương đương Morita với D và $B'$ tương đương Morita với $D'$ (VIII, p. 102, Ví dụ 1). Do đó, các trường D và $D'$ tương đương Morita, nên đẳng cấu (VIII, p. 111, Mệnh đề 13, c)).

#### Hệ quả 3 {#alg-viii-s7-lem-2-cor-3 .statement tag=0089}

Cho K là một trường giao hoán, và cho A là một đại số trên K bậc hữu hạn có vành nền đơn. Tồn tại một số nguyên $r$ và một đại số trên K D có bậc hữu hạn trên K, là một trường, sao cho A đẳng cấu với $M_r(D)$. Đặc biệt, nếu K đóng đại số, thì A đẳng cấu với một đại số ma trận trên K.

Cho S là một A-môđun trái đơn; nó là một không gian vectơ trên K hữu hạn chiều. Hoán tập của nó do đó là một đại số bậc hữu hạn trên K. Mệnh đề thứ nhất khi đó suy ra từ Bổ đề 1. Nếu K đóng đại số, thì D = K theo Định lý 1 của VIII, p. 47.

#### Nhận xét 4 {#alg-viii-s7-n1-rem-4 .statement tag=008A}

Cho K là một trường giao hoán đóng đại số, và cho A là một đại số bậc hữu hạn trên K. Đại số A là đơn khi và chỉ khi tồn tại một số nguyên $n\geqslant 1$ sao cho A đẳng cấu với $M_n(K)$. Tâm của nó khi đó đẳng cấu với K.

### 2. Các môđun trên vành đơn

#### Bổ đề 3 {#alg-viii-s7-lem-3 .statement tag=008B}

Cho A là một vành đơn, và cho S là một A-môđun đơn. Ký hiệu trường đối của hoán tập của S là D. Mọi A-môđun đều đẳng cấu với một A-môđun có dạng $S\otimes_DV$, trong đó V là một không gian vectơ trái trên trường D.

Điều này suy ra từ Bổ đề 1 của VIII, p. 120 và định lý Morita (VIII, p. 103).

#### Mệnh đề 2 {#alg-viii-s7-prop-2 .statement tag=008C}

Cho A là một vành đơn và S là một A-môđun đơn.

a) Mọi A-môđun đều xạ ảnh và đẳng kiểu kiểu S, do đó nửa đơn. Nếu nó có độ dài $\mathfrak{a}$, thì nó đẳng cấu với $S^{(\mathfrak{a})}$.

b) Mọi A-môđun khác không đều sinh.

c) Hai A-môđun là đẳng cấu nếu và chỉ nếu chúng có cùng độ dài.

Ký hiệu trường đối của hoán tập của S bởi D. Theo Bổ đề 1 của VIII, p. 120, S là một song môđun khả nghịch $(A$, D). Cho M là một A-môđun; theo Bổ đề 3, nó đẳng cấu với một môđun có dạng $S\otimes_DV$, trong đó V là một không gian vectơ trái trên trường D.

D-môđun V là xạ ảnh và đẳng kiểu kiểu $D_s$; nó sinh nếu và chỉ nếu nó không thu về 0. Sau cùng, độ dài của $S\otimes_DV$ bằng chiều của không gian vectơ trên D V, và hai không gian vectơ là đẳng cấu nếu và chỉ nếu chúng có cùng chiều. Mệnh đề 2 nay suy ra theo Mệnh đề 10 của VIII, p. 109 và 12 của VIII, p. 110.

Cho $r\geqslant 1$ là một số nguyên. Ta nói rằng một lực lượng $\mathfrak{a}$ chia được cho $r$ nếu tồn tại một lực lượng $\mathfrak{b}$ sao cho $\mathfrak{a}=r\mathfrak{b}$. Điều này xảy ra nếu $\mathfrak{a}$ là vô hạn vì ta có $r\mathfrak{a}=\mathfrak{a}($Lý thuyết tập hợp, III, §6, No. 3, p. 188, Hệ quả 3). Từ nhận xét này suy ra rằng nếu lực lượng $\mathfrak{a}$ chia được cho $r$, thì tồn tại một lực lượng duy nhất $\mathfrak{b}$ sao cho $\mathfrak{a}=r\mathfrak{b}$.

#### Hệ quả {#alg-viii-s7-n2-cor-1 .statement tag=008D}

Cho $k$ là một trường giao hoán, và A là một $k$-đại số đơn có bậc hữu hạn trên $k$. Mọi A-môđun đơn đều hữu hạn chiều trên $k$. Hai A-môđun là đẳng cấu nếu và chỉ nếu các số chiều của chúng trên $k$ bằng nhau.

Mọi A-môđun đơn đều đẳng cấu với một thương của $A_s$, do đó hữu hạn chiều trên $k$. Hệ quả khi đó suy ra từ Mệnh đề 2, c).

#### Mệnh đề 3 {#alg-viii-s7-prop-3 .statement tag=008E}

Cho A là một vành đơn. Một A-môđun M là tự do nếu và chỉ nếu độ dài của nó chia được cho độ dài của A. Nếu điều đó đúng, thì mọi cơ sở của M đều có cùng một lực lượng, được ký hiệu bởi dim$_A(M)$ (II, §7, No. 3, p. 294, Nhận xét 2) và được xác định bởi quan hệ

(1) long$_A(M) =$ long(A) $\cdot$ dim$_A(M)$.

Giả sử rằng M là tự do, và gọi $(e_i)_{i\in I}$ là một cơ sở của M. A-môđun M là tổng trực tiếp của các A-môđun $Ae_i$, mỗi môđun này đều đẳng cấu với $A_s$. Đặt $r=$ long$_A(A_s)$; đây là một số nguyên lớn hơn hoặc bằng 1 (VIII, p. 119, Mệnh đề 1). Ta có long$_A(M) =r$ Card(I) theo công thức (13) của VIII, p. 73.

Ngược lại, giả sử rằng lực lượng long$_A(M)$ chia được cho $r$. Gọi $\mathfrak{a}$ là lực lượng sao cho long$_A(M) =r\mathfrak{a}$. Khi đó A-môđun M có cùng độ dài với $A^{(\mathfrak{a})}_s$, do đó đẳng cấu với môđun này theo Mệnh đề 2. Điều này chứng tỏ rằng M là tự do.

#### Mệnh đề 4 {#alg-viii-s7-prop-4 .statement tag=008F}

Cho A là một vành đơn và M là một A-môđun khác không. Ký hiệu vành tự đồng cấu của A-môđun M bởi B, và xem M như một B-môđun trái.

a) Ánh xạ $a\mapsto a_M$ là một đẳng cấu từ A lên vành tự đồng cấu của B-môđun M.

b) Giả sử rằng M có độ dài hữu hạn như một A-môđun. Khi đó vành B là đơn, và ta có

(2) long$_A(M) =$ long(B) and long$_B(M) =$ long(A).

A-môđun M là sinh theo Mệnh đề 2 của VIII, p. 122. Theo định nghĩa, ta có $B = A'_M$, và do đó mệnh đề a) suy ra từ Định lý 2 của VIII, p. 82.

Giả sử M là một A-môđun có độ dài hữu hạn. Chọn một A-môđun đơn S, và gọi D là trường đối của vành các tự đồng cấu của S. Theo Bổ đề 3, A-môđun M đẳng cấu với một môđun dạng $S\otimes_DV$, trong đó V là một không gian vectơ trái trên trường D. Không gian vectơ V là hữu hạn chiều. Theo Định lý 3 của VIII, p. 64, vành B đẳng cấu với End$_D(V)$; theo Bổ đề 2 (VIII, p. 121), do đó vành B là đơn. Có tính đến Nhận xét 1 của VIII, p. 63, ta thu được các đẳng thức

long(B) = dim$_D(V) =$ long$_A(M)$.

Theo các Nhận xét 1 của VIII, p. 63 và 3 của VIII, p. 121, ta có các quan hệ

long$_B(M) =$ long$_{End_D(V)}(S\otimes_DV) =$ dim$_D(S) =$ long(A),

điều này cho quan hệ cuối cùng.

### 3. Bậc

Xét một vành B và một vành con A của B. Trang bị cho B cấu trúc song môđun $(A$, A) suy ra bằng hạn chế vô hướng từ cấu trúc song môđun $(B$, B) trên $_sB_d$.

#### Mệnh đề 5 {#alg-viii-s7-prop-5 .statement tag=008G}

Cho B là một vành, A là một vành con đơn của B, và S là một A-môđun trái đơn. Khi đó B là một A-môđun trái tự do có chiều long$_A(B\otimes_AS)$.

Gọi $r$ là độ dài của A; A-môđun $A_s$ đẳng cấu với $S^r$. Bây giờ, A-môđun trái B đẳng cấu với $B\otimes_AA_s$ (II, §3, No. 4, p. 249), do đó đẳng cấu với $(B\otimes_AS)^r$ (II, §3, No. 7, p. 255, Mệnh đề 7). Vậy ta có long$_A(B) =r$ long$_A(B\otimes_AS)$, và Mệnh đề 5 suy ra từ Mệnh đề 3 của VIII, p. 123.

#### Định nghĩa 2 {#alg-viii-s7-def-2 .statement tag=008H}

Cho B là một vành và A là một vành con đơn của B. Chiều của A-môđun trái tự do B được gọi là bậc (trái) của B trên A và được ký hiệu bởi[^1] $[B : A]_s$.

Bằng cách thay thế A và B bằng các vành đối, từ trên đây suy ra rằng B là một A-môđun phải tự do. Ta ký hiệu chiều của nó bởi $[B : A]_d$ và gọi đó là bậc phải của B trên A.

Ta có thể cho một ví dụ về một trường B và một trường con A sao cho các bậc $[B : A]_s$ và $[B : A]_d$ khác nhau.[^2]

Cho B là một vành, A là một vành con đơn của B, và S là một A-môđun trái đơn. Cho M là một A-môđun và $\mathfrak{a}$ là độ dài của nó. Các A-môđun M và $S^{(\mathfrak{a})}$ đẳng cấu (VIII, p. 122, Mệnh đề 2), do đó các B-môđun $B\otimes_AM$ và $(B\otimes_AS)^{(\mathfrak{a})}$ cũng đẳng cấu. Quan hệ

(3) long$_A(B\otimes_AM) = [B : A]_s$ long$_A(M)$

suy ra từ Mệnh đề 5 và Định nghĩa 2.

#### Mệnh đề 6 {#alg-viii-s7-prop-6 .statement tag=008I}

Cho C là một vành, B là một vành con đơn của C, và A là một vành con đơn của B. Khi đó ta có $[C : A]_s= [C : B]_s[B : A]_s$.

Lấy một cơ sở $(e_i)_{i\in I}$ của C được xem như một B-môđun trái và một cơ sở $(f_j)_{j\in J}$ của B được xem như một A-môđun trái. Khi đó họ $(f_je_i)_{j\in J,i\in I}$ là một cơ sở của C được xem như một A-môđun trái (II, §1, No. 13, p. 222, Mệnh đề 25); Mệnh đề 6 được suy ra.

#### Nhận xét 1 {#alg-viii-s7-n3-rem-1 .statement tag=008J}

Giả sử A là một vành con đơn của một vành đơn B và bậc phải $[B : A]_d$ là hữu hạn. Gọi C là vành các tự đồng cấu của B được xem như một A-môđun phải; đó là một vành đơn theo Mệnh đề 4, b) của VIII, p. 123. Với mọi $b$ trong B, gọi $\gamma (b)$ là ánh xạ $x\mapsto bx$ từ B vào B; khi đó $\gamma :b\mapsto \gamma (b)$ là một đẳng cấu từ B lên một vành con của C. Hơn nữa, nếu $(x_1, . . . , x_m)$ là một cơ sở của A-môđun phải B, thì cấu xạ biến $c$ thành $(c(x_1), . . . , c(x_m))$ là một đẳng cấu của các B-môđun trái từ C lên $B^m_s$; do đó, ta có quan hệ

$$
[C :\gamma (B)]_s= [B : A]_d \tag{4}
$$

Có tính đến quan hệ (2) của VIII, p. 123 áp dụng cho A-môđun phải B, ta thấy rằng

(5) long(C) $= [B : A]_d$ long(A).

#### Nhận xét 2 {#alg-viii-s7-n3-rem-2 .statement tag=008K}

Cho K là một trường giao hoán. Nếu A là một đại số con đơn của một đại số B bậc hữu hạn trên K, thì bậc trái của B trên A thỏa mãn hệ thức $[B : A]_s[A : K] = [B : K]$ theo Mệnh đề 6 của VIII, p. 125. Tương tự, ta có $[B : A]_d[A : K] = [B : K]$. Suy ra đẳng thức $[B : A]_s= [B : A]_d$.

### 4. Các iđêan của các vành đơn

Cho D là một trường và V là một không gian vectơ phải trên D có số chiều hữu hạn $n\geqslant 1$. Xét vành đơn A = End$_D(V)$. Với mọi không gian con tuyến tính W của V, ta ký hiệu tập hợp các phần tử $a$ của A thỏa mãn $aW = 0$ (resp. $aV\subset W$) bởi $\mathfrak{a}(W)$ (resp. $\mathfrak{b}(W)$).

#### Mệnh đề 7 {#alg-viii-s7-prop-7 .statement tag=008L}

a) Ánh xạ $W\mapsto \mathfrak{a}(W)$ là một song ánh từ tập hợp các không gian con tuyến tính của V lên tập hợp các iđêan trái của A.

b) Ánh xạ $W\mapsto \mathfrak{b}(W)$ là một song ánh từ tập hợp các không gian con tuyến tính của V lên tập hợp các iđêan phải của A.

c) Cho $W_1$ và $W_2$ là các không gian con tuyến tính của V. Các quan hệ $W_1\subset W_2$, $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$, và $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$ là tương đương.

Mệnh đề b) suy ra từ Ví dụ 1, b) của VIII, p. 104 áp dụng cho song môđun khả nghịch $(D^o,A^o$)-V, cũng như tính tương đương của các quan hệ $W_1\subset W_2$ và $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$.

Cho $V^*$ là đối ngẫu của V, được xem như một không gian vectơ phải trên trường đối $D^o$ của D. Với mọi không gian con W của V, ký hiệu phần trực giao của W trong $V^*$ là $W'$. Ánh xạ $W\mapsto W'$ là một song ánh từ tập hợp các không gian con của V lên tập hợp các không gian con của $V^*$. Nếu $W_1$ và $W_2$ là hai không gian con của V, thì các quan hệ $W_1\subset W_2$ và $W'_1\supset W'_2$ là tương đương. Bây giờ, ánh xạ $u\mapsto^tu$ là một đẳng cấu từ A lên vành đối của End$_{D^o}(V^*)$; nó biến các iđêan trái của A thành các iđêan phải của End$_{D^o}(V^*)$ và biến $\mathfrak{a}(W)$ thành tập hợp $\mathfrak{b}(W')$ các tự đồng cấu $h$ của $V^*$ sao cho $h(V^*)\subset W'$. Mệnh đề a), cũng như tính tương đương của các quan hệ $W_1\subset W_2$ và $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$, khi đó suy ra từ mệnh đề tương tự với b) đối với đối ngẫu $V^*$ của V.

#### Hệ quả {#alg-viii-s7-n4-cor-1 .statement tag=008M}

a) Các iđêan trái cực tiểu của A là các iđêan $\mathfrak{a}(H)$, trong đó H là một siêu phẳng trong V. Các iđêan trái cực đại của A là các iđêan $\mathfrak{a}(L)$, trong đó L là một đường thẳng trong V.

b) Các iđêan phải cực tiểu của A là các iđêan $\mathfrak{b}(L)$, trong đó L là một đường thẳng trong V. Các iđêan phải cực đại của A là các iđêan $\mathfrak{b}(H)$, trong đó H là một siêu phẳng trong V.

Cho $(L_i)_{i\in I}$ là một họ các đường thẳng có tổng trực tiếp là V. Cho $(\varepsilon_i)_{i\in I}$ là họ các phép chiếu liên kết với phân tích $V =\oplus_{i\in I}L_i$. Các $\varepsilon_i$ là những phần tử lũy đẳng trong A, và ta có $\varepsilon_i\varepsilon_j= 0$ với $i\not=j$ và $\sum_{i\in I}\varepsilon_i= 1$. Ký hiệu siêu phẳng $\sum_{j\not=i}L_j$ bởi $H_i$; đó là hạt nhân của $\varepsilon_i$. Khi đó ta có

$$
\mathfrak{a}(H_i) = A\varepsilon_i,\mathfrak{b}(L_i) =\varepsilon_iA
$$

A-môđun $A_s$ là tổng trực tiếp của họ $(\mathfrak{a}(H_i))_{i\in I}$ các iđêan trái cực tiểu, và $A_d$ là tổng trực tiếp của họ $(\mathfrak{b}(L_i))_{i\in I}$ các iđêan phải cực tiểu.

Xét trường hợp riêng $V = D^n_d$, và đồng nhất A với vành ma trận $\mathbf{M}_n(D)$. Ký hiệu khoảng $[1, n]$ trong $\mathbf{N}$ bởi I và cơ sở chính tắc của V bởi $(v_i)_{i\in I}$; đặt $L_i=v_iD$, và ký hiệu bởi $E_{ij}$ các đơn vị ma trận (II, §10, No. 3, p. 341). Khi đó ta có $\varepsilon_i= E_{ii}$. Iđêan trái AE$_{ii}$ bằng DE$_{1i}+\cdots +$ DE$_{ni}$ và gồm các ma trận mà mọi cột trừ cột thứ $i$ đều bằng không. Iđêan phải $E_{ii}A$ bằng DE$_{i1}+\cdots +$ DE$_{in}$ và gồm các ma trận mà mọi hàng trừ hàng thứ $i$ đều bằng không. Ta cũng có quan hệ

$$
E_{ii}A E_{jj}= E_{ii}A\cap A E_{jj}= D E_{ij}
$$

với $i$ và $j$ nằm giữa 1 và $n$.

### Bài tập {#alg-viii-s7-exercises}

Xem [bài tập cho § 7](exercises/s7/).

[^1]: Nếu A và B là các trường giao hoán, hãy chú ý đừng nhầm bậc bằng [B : A] với bậc tách được của mở rộng B của A, được định nghĩa ở V, §6, No. 5, p. 31 và cũng được ký hiệu bởi $[B : A]_s$.
[^2]: xem A. H. Schofield, bài toán của Artin đối với các mở rộng trường lệch, Math. Proc. Cambridge Philos. Soc. **97** (1985), pp. 1–6.
