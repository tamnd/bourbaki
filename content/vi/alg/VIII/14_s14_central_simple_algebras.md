---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 14
section_title: Central Simple Algebras
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.251-A VIII.276
pdf_pages: 0268-0293
extraction: native
subsections:
    - "no": 1
      title: Central Simple Algebras
      page: 251
      pdf_page: 268
    - "no": 2
      title: Two Lemmas on Bimodules
      page: 254
      pdf_page: 271
    - "no": 3
      title: Conjugacy Theorems
      page: 256
      pdf_page: 273
    - "no": 4
      title: Automorphisms of Semisimple Algebras
      page: 257
      pdf_page: 274
    - "no": 5
      title: Simple Subalgebras of Simple Algebras
      page: 259
      pdf_page: 276
    - "no": 6
      title: Maximal Commutative Subalgebras
      page: 261
      pdf_page: 278
    - "no": 7
      title: Maximal Étale Subalgebras
      page: 264
      pdf_page: 281
    - "no": 8
      title: Diagonalizable Subalgebras of Simple Algebras
      page: 266
      pdf_page: 283
statements: 36
exercises: 19
content_sha256: f0fd5a8cda83593f9f7e976ecb732072cf8a9b0ec0c2e5344da1de3a9fd32e51
translated_from: content/en/alg/VIII/14_s14_central_simple_algebras.md
source_content_sha256: 6b4399d77699c060fb6846778021967e62ae015f18624ee87348066955fdf6f2
translation_model: gpt-5.4
translation_run: translate-vi-1732bc39
glossary_version: 34
glossary_terms_sha256: decb02e849ddd4d5ad208807d044d88052d476b636f8b7f782820b81a4aa25a7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 14. CÁC ĐẠI SỐ ĐƠN TÂM

Trong tiết này, K là một trường giao hoán.

### 1. Các Đại Số Đơn Tâm

#### Định nghĩa 1 {#alg-viii-s14-def-1 .statement tag=00GE}

Ta nói rằng một đại số A trên trường K là trung tâm nếu ánh xạ $\lambda \mapsto \lambda 1$ là một song ánh từ K lên tâm của A.

Một đại số trung tâm không phải là 0. Với mọi số nguyên $n\geqslant 1$, đại số ma trận trên K $\mathbf{M}_n(K)$ là trung tâm (VIII, p. 83, Hệ quả 2) và đơn (VIII, p. 120, Định lý 1). Nói chung hơn, cho D là một đại số trung tâm trên K bậc hữu hạn; khi đó $\mathbf{M}_n(D)$ cũng là trung tâm. Cho A là một vành đơn; tâm của nó Z là một trường (VIII, p. 121, Hệ quả 1), và do đó A là một đại số đơn tâm trên Z. Nếu trường K đóng đại số, thì một đại số đơn bậc hữu hạn trên K là trung tâm (VIII, p. 122, Hệ quả 3). Đại số đối của một đại số đơn tâm là đơn tâm.

#### Nhận xét 1 {#alg-viii-s14-n1-rem-1 .statement tag=00GF}

Cho A và B là các đại số trên K. Nếu $A\otimes_KB$ là một đại số đơn tâm, thì A và B cũng vậy (III, §4, No. 4, p. 468, Hệ quả của Mệnh đề 6 và VIII, p. 221, Mệnh đề 6). Ngược lại, nếu A và B là các đại số đơn tâm và nếu một trong hai có bậc hữu hạn trên K, thì $A\otimes_KB$ là một đại số đơn tâm (III, §4, No. 4, p. 468, Hệ quả của Mệnh đề 6 và VIII, p. 222, Hệ quả 2).

#### Nhận xét 2 {#alg-viii-s14-n1-rem-2 .statement tag=00GG}

Cho A là một đại số trên K và L là một mở rộng của trường K. Nếu đại số trên L $A_{(L)}$ là đơn tâm, thì đại số trên K A là đơn tâm. Ngược lại, nếu một trong hai bậc [A : K] và [L : K] là hữu hạn và nếu A là một đại số đơn tâm trên K, thì đại số trên L $A_{(L)}$ là đơn tâm. Điều này suy ra từ Hệ quả 2 của VIII, p. 222.

#### Nhận xét 3 {#alg-viii-s14-n1-rem-3 .statement tag=00GH}

Cho A và B là các đại số trên K tương đương Morita. Đại số A là đơn tâm khi và chỉ khi B là đơn tâm (VIII, p. 105, Mệnh đề 6; p. 111, Hệ quả; và p. 102, Hệ quả 1).

#### Nhận xét 4 {#alg-viii-s14-n1-rem-4 .statement tag=00GI}

Đặc biệt, nếu A là một đại số đơn tâm trên K và $n\geqslant 1$, thì $\mathbf{M}_n(A)$ là một đại số đơn tâm trên K (VIII, p. 102, Ví dụ 1).

#### Định lý 1 {#alg-viii-s14-thm-1 .statement tag=00GJ}

Cho A là một đại số trên K bậc hữu hạn. Các tính chất sau là tương đương:

(i) Đại số A là đơn tâm.

(ii) Đại số A là trung tâm và không có căn.

(iii) Đồng cấu chính tắc từ đại số trên K $A\otimes_KA^o$ vào đại số trên K End$_K(A)$ gửi $a\otimes a'$ lên ánh xạ K-tuyến tính $x\mapsto axa'$ từ A vào A là song ánh.

(iv) Tồn tại một mở rộng L của trường K và một số nguyên $n\geqslant 1$ sao cho các đại số trên L $A_{(L)}$ và $\mathbf{M}_n(L)$ là đẳng cấu.

(v) Với mọi bao đóng tách được $K'$ của K, tồn tại một số nguyên $n\geqslant 1$ sao cho các đại số trên $K'$ $A_{(K')}$ và $\mathbf{M}_n(K')$ là đẳng cấu.

(vi) Tồn tại một mở rộng Galois L của trường K có bậc hữu hạn và một số nguyên $n\geqslant 1$ sao cho các đại số trên L $A_{(L)}$ và $\mathbf{M}_n(L)$ là đẳng cấu.

(vii) Tồn tại một đại số trên K có bậc hữu hạn D là một trường có tâm là K và một số nguyên $n\geqslant 1$ sao cho đại số A đẳng cấu với đại số $\mathbf{M}_n(D)$.

Một vành là đơn khi và chỉ khi nó là nửa đơn và tâm của nó là một trường (VIII, p. 143, Hệ quả của Mệnh đề 10). Vì A là một đại số có bậc hữu hạn trên trường K, nó là một vành Artin trái; do đó nó là nửa đơn khi và chỉ khi nó không có căn (VIII, p. 154, Mệnh đề 4). Suy ra tính tương đương của (i) và (ii).

Đặt $E = A\otimes_KA^o$ và F = End$_K(A)$; ký hiệu bởi $\varphi$ đồng cấu chính tắc từ E vào F được xác định bởi quan hệ $\varphi (a\otimes a')(x) =axa'$ với $x, a, a'$ trong A. Nếu đại số A là đơn tâm, thì $A^o$ cũng vậy và do đó E cũng vậy (Nhận xét 1), nên $\varphi$ là đơn ánh. Bây giờ, ta có $[E : K] = [A : K]^2= [F : K]$, nên $\varphi$ là song ánh. Đảo lại, giả sử rằng $\varphi$ là song ánh; vì đại số F là đơn tâm (bởi vì nó đẳng cấu với một đại số ma trận $\mathbf{M}_m$(K)), nên E cũng vậy, và do đó A cũng vậy (Nhận xét 1). Như vậy ta đã chứng minh được tính tương đương của (i) và (iii).

Theo Nhận xét 4, mệnh đề (vii) kéo theo mệnh đề (i). Hàm ý đảo lại suy ra từ Hệ quả 3 của VIII, p. 122 và Hệ quả 2 của VIII, p. 83.

Hiển nhiên là (vi) kéo theo (iv), và (iv) kéo theo (i) theo Nhận xét 2.

Còn phải chứng minh các kéo theo (i)$\Rightarrow$(v)$\Rightarrow$(vi). Giả sử rằng A là đơn tâm, và gọi $K'$ là một bao đóng tách được của K (V, §7, No. 8, p. 45) . Khi đó $A_{(K')}$ là một đại số đơn tâm bậc hữu hạn trên $K'$ (VIII, p. 251, Nhận xét 2). Theo hệ quả ở VIII, p. 231, do đó tồn tại một số nguyên $n\geqslant 1$ và một đẳng cấu các $K'$-đại số từ $A_{(K')}$ lên $\mathbf{M}_n(K')$; lưu ý rằng các $K'$-đại số $\mathbf{M}_n(K')$ và $\mathbf{M}_n(K)_{(K')}$ là đẳng cấu. Theo Bổ đề 4 của VIII, p. 234, tồn tại một mở rộng con L của $K'$, sinh hữu hạn trên K, sao cho các L-đại số $A_{(L)}$ và $\mathbf{M}_n(K)_{(L)}$ là đẳng cấu. Khi đó L là tách được và có bậc hữu hạn trên K, nên được chứa trong một mở rộng con $L'$ của $K'$ vừa Galois vừa có bậc hữu hạn trên K (V, §10, No. 1, p. 57, Mệnh đề 2). Khi đó các $L'$-đại số $A_{(L')}$ và $\mathbf{M}_n(L')$ là đẳng cấu.

#### Hệ quả 1 {#alg-viii-s14-thm-1-cor-1 .statement tag=00GK}

Cho A là một đại số đơn tâm bậc hữu hạn trên một trường đóng tách được K. Tồn tại một số nguyên $n\geqslant 1$ sao cho A đẳng cấu với đại số ma trận $\mathbf{M}_n(K)$.

Thật vậy, mọi mở rộng Galois của K đều bằng K; chỉ cần áp dụng sự tương đương giữa các tính chất (i) và (v) của Định lý 1.

#### Hệ quả 2 {#alg-viii-s14-thm-1-cor-2 .statement tag=00GL}

Cho A là một đại số đơn tâm bậc hữu hạn trên K (chẳng hạn, một trường bậc hữu hạn trên K có tâm là K). Tồn tại một số nguyên $n\geqslant 1$ sao cho $[A : K] =n^2$.

Cho L là một mở rộng của K và $n$ là một số nguyên dương sao cho các L-đại số $A_{(L)}$ và $\mathbf{M}_n(L)$ đẳng cấu. Ta có

$$
[A : K] = [A_{(L)}: L] = [\mathbf{M}_n(L) : L] =n^2
$$

Theo ký hiệu của Hệ quả 2, số nguyên $n$ được gọi là bậc thu gọn của A.

#### Nhận xét 5 {#alg-viii-s14-n1-rem-5 .statement tag=00GM}

Cho A là một đại số đơn tâm bậc hữu hạn trên K mà bậc thu gọn là một số nguyên tố $\ell$. Khi đó hoặc A là một trường, hoặc A đẳng cấu với $\mathbf{M}_{\ell}(K)$. Thật vậy, A đẳng cấu với một đại số dạng $\mathbf{M}_n$(D), trong đó D là một trường có tâm là K, và ta có

$$
\ell^2= [A : K] =n^2[D : K]
$$

nếu A không phải là một trường, thì $n\not= 1$, do đó $n=\ell$ và D = K.

### 2. Hai bổ đề về song môđun

Cho A và B là các vành. Với mọi đồng cấu $f$ từ B vào A, ta ký hiệu bởi $A^f$ $(B$, A)-song môđun có A-môđun phải nền tảng là $A_d$ và phép toán ngoài cho cấu trúc B-môđun trái của nó được cho bởi $(b, a)\mapsto f(b)a$.

#### Bổ đề 1 {#alg-viii-s14-lem-1 .statement tag=00GN}

Cho $f$ và $g$ là các đồng cấu từ B vào A. Các điều kiện sau là tương đương:

(i) Các $(B,A)$-song môđun $A^f$ và $A^g$ là đẳng cấu.

(ii) Tồn tại một tự đẳng cấu trong (I, §8, No. 4, p. 102, Ví dụ 2) $\theta$ của A sao cho $g=\theta \circ f$.

Các tự đẳng cấu của A-môđun phải $A_d$ là các ánh xạ $x\mapsto ax$, trong đó $a$ là một phần tử khả nghịch của A. Một tự đẳng cấu như thế là một ánh xạ B-tuyến tính từ $A^f$ đến $A^g$ khi và chỉ khi ta có

$$
g(b)ax=af(b)x
$$

với mọi $x$ trong A và mọi $b$ trong B. Quan hệ này tương đương với $g(b) =af(b)a^{-1}$ với mọi $b$ trong B, tức là tương đương với $g=\theta \circ f$, trong đó $\theta$ là tự đẳng cấu trong $x\mapsto axa^{-1}$ của A.

#### Bổ đề 2 {#alg-viii-s14-lem-2 .statement tag=00GO}

Giả sử rằng B là một vành nửa đơn là một môđun hữu hạn sinh trên tâm Z của nó. Cho M và N là các song môđun $(B,A)$. Giả sử rằng chúng có độ dài hữu hạn (điều này, đặc biệt, đúng khi chúng là các A-môđun phải có độ dài hữu hạn). Nếu M và N đẳng cấu như các song môđun $(Z,A)$, thì chúng đẳng cấu như các song môđun $(B,A)$.

A) Trước hết xét trường hợp khi B là vành tự đồng cấu của một không gian vectơ S có số chiều hữu hạn $d$ trên một trường giao hoán L. Khi đó ta có Z = L; ta xem S như một song môđun $(B$, Z). Vành B là đơn, S là một B-môđun đơn, và Z là hoán tập của S; mọi B-môđun đều đẳng kiểu kiểu S (VIII, p. 122, Mệnh đề 2 a)). Gọi $(V, \alpha )$ (tương ứng $(W, \beta )$) là một mô tả của B-môđun M (tương ứng N). Tập hợp V (tương ứng W) được trang bị một cấu trúc song môđun $(Z$, A) sao cho $\alpha$ (tương ứng $\beta$ ) là một đẳng cấu của các song môđun $(B$, A) (VIII, p. 64, Nhận xét 2). Với tư cách là các song môđun $(Z$, A), M đẳng cấu với $V^d$ và N đẳng cấu với $W^d$, và tồn tại một đẳng cấu từ tập hợp các song môđun con $(Z$, A) của V, được sắp thứ tự bởi quan hệ bao hàm, lên tập hợp các song môđun con $(B$, A) của M (loc. cit.). Do đó V là một song môđun $(Z$, A) có độ dài hữu hạn, và W cũng vậy. Vì các song môđun $(Z,A)$ $V^d$ và $W^d$ đẳng cấu, các song môđun $(Z$, A) V và W đẳng cấu theo Định lý 2, d) của VIII, p. 37 áp dụng cho vành $Z\otimes_{\mathbf{Z}}A^o$. Cuối cùng, các song môđun $(B$, A) M và N đẳng cấu.

B) Bây giờ xét trường hợp B là một vành đơn được sinh hữu hạn như một Z-môđun. Khi đó Z là một trường, và B là một đại số đơn tâm bậc hữu hạn trên trường Z. Theo Định lý 1 của VIII, p. 252, tồn tại một mở rộng $Z'$ của Z có bậc hữu hạn trên Z sao cho $Z'$-đại số $B'= B_{(Z')}$ đẳng cấu với đại số tự đồng cấu của một $Z'$-không gian vectơ hữu hạn chiều. Đặt $M'= M_{(Z')}$ và $N'= N_{(Z')}$. Khi đó $M'$ và $N'$ là các $(B'$, A)-song môđun có độ dài hữu hạn; được xem như các $(Z'$, A)-song môđun, $M'$ và $N'$ là đẳng cấu. Theo trường hợp đã xét trong $A), M'$ và $N'$ đẳng cấu như các $(B'$, A)-song môđun và a fortiori như các $(B$, A)-song môđun. Đặt $r= [Z': Z]$. $(B$, A)-song môđun $M'= Z'\otimes_ZM$ đẳng cấu với $M^r$, và tương tự, $(B$, A)-song môđun $N'$ đẳng cấu với $N^r$. Vì M và N là các $(B$, A)-song môđun có độ dài hữu hạn, suy ra từ Định lý 2, d) của VIII, p. 37 rằng các $(B$, A)-song môđun M và N là đẳng cấu.

C) Sau cùng, xét trường hợp tổng quát, khi B là một vành nửa đơn sinh hữu hạn như một Z-môđun. Gọi $\mathscr{S}$ là tập hợp các lớp của các B-môđun đơn; nó là hữu hạn (VIII, p. 136, Mệnh đề 1). Với mọi $\lambda \in \mathscr{S}$, ký hiệu bởi $M_{\lambda}$ (tương ứng $N_{\lambda}$) thành phần đẳng kiểu kiểu $\lambda$ của B-môđun M (tương ứng N); đó là một môđun con song $(B$, A) của M (tương ứng N) (Nhận xét, VIII, p. 67). Với $\lambda \in \mathscr{S}$, ký hiệu linh hóa tử của B-môđun $\lambda$ bởi $\mathfrak{b}_{\lambda}$, và đặt $B_{\lambda}= B/\mathfrak{b}_{\lambda}$; gọi $Z_{\lambda}$ là tâm của $B_{\lambda}$. Với $\lambda \in \mathscr{S}$, các song môđun $(B_{\lambda}$, A) $M_{\lambda}$ và $N_{\lambda}$ có độ dài hữu hạn. Khi đó có thể đồng nhất B với tích của các vành đơn $B_{\lambda}$ và Z với tích của các $Z_{\lambda}$ (VIII, p. 141, Mệnh đề 8). Hơn nữa, có thể đồng nhất M với $\prod_{\lambda\in\mathscr{S}}M_{\lambda}$ và N với $\prod_{\lambda\in\mathscr{S}}N_{\lambda}$. Theo giả thiết, M và N đẳng cấu như các song môđun $(Z$, A); suy ra rằng với $\lambda \in \mathscr{S}, M_{\lambda}$ và $N_{\lambda}$ là các song môđun $(Z_{\lambda}$, A) đẳng cấu. Theo trường hợp đã xét ở B), các song môđun $(B_{\lambda}$, A) $M_{\lambda}$ và $N_{\lambda}$ là đẳng cấu, và do đó các song môđun $(B$, A) M và N là đẳng cấu.

#### Nhận xét {#alg-viii-s14-n2-rem-1 .statement tag=00GP}

Từ chứng minh của Bổ đề 2 suy ra rằng M và N là các $(Z,A)$-song môđun có độ dài hữu hạn. Do đó, nếu B và A là hai vành nửa đơn là các môđun sinh hữu hạn trên các tâm tương ứng Z(B) và Z(A) của chúng, thì hai $(B$, A)-song môđun có độ dài hữu hạn đẳng cấu như các (Z(B),Z(A))-song môđun là đẳng cấu.

### 3. Các định lý liên hợp

#### Định lý 2 {#alg-viii-s14-thm-2 .statement tag=00GQ}

Cho B là một vành nửa đơn và Z là tâm của nó; giả sử rằng B là một Z-môđun sinh hữu hạn. Cho A là một vành Artin phải, và $f$ và $g$ là các đồng cấu vành từ B vào A; ký hiệu $f_Z$ và $g_Z$ là các hạn chế của $f$ và $g$ lên Z. Các tính chất sau là tương đương:

(i) Tồn tại một tự đẳng cấu trong $\theta$ của A sao cho $g=\theta \circ f$.

(ii) Tồn tại một tự đẳng cấu trong $\theta$ của A sao cho $g_Z=\theta \circ f_Z$.

Vì vành A là Artin phải, $A_d$ là một A-môđun phải có độ dài hữu hạn (VIII, p. 6, Định lý 1). Do đó $A^f$ và $A^g$ là các $(B$, A)-song môđun có độ dài hữu hạn. Theo Bổ đề 1 (VIII, p. 254), mệnh đề (i) có nghĩa là $A^f$ và $A^g$ là các $(B$, A)-song môđun đẳng cấu, và mệnh đề (ii) có nghĩa là chúng là các $(Z,A)$-song môđun đẳng cấu. Vì thế, tính tương đương của (i) và (ii) suy ra từ Bổ đề 2 (VIII, p. 254).

#### Hệ quả {#alg-viii-s14-n3-cor-1 .statement tag=00GR}

Cho A và B là các đại số trên trường K. Giả sử rằng B là đơn tâm và có bậc hữu hạn, và rằng A là Artin phải. Cho $f$ và $g$ là các đồng cấu đại số trên K từ B vào A. Tồn tại một tự đẳng cấu trong $\theta$ của A sao cho $g=\theta \circ f$.

Theo ký hiệu của Định lý 2, ta có Z = K và do đó $f_Z= 1_Z=g_Z$.

#### Định lý 3 (Skolem–Noether) {#alg-viii-s14-thm-3 .statement tag=00S9}

Cho A và B là các đại số đơn trên K và Z(A) và Z(B) là các tâm của chúng. Giả sử rằng đại số B có bậc hữu hạn trên K và rằng đại số $Z(A)\otimes_KZ(B)$ là một trường (điều này, đặc biệt, xảy ra khi A hoặc B là trung tâm). Cho $f$ và $g$ là các đồng cấu đại số trên K từ B vào A. Tồn tại một tự đẳng cấu trong $\theta$ của A sao cho $g=\theta \circ f$.

Theo Bổ đề 1 của VIII, p. 254, chỉ cần chứng minh rằng các $(B,A)$-song môđun $A^f$ và $A^g$ là đẳng cấu. Bây giờ, ta có thể xem $A^f$ và $A^g$ như các môđun trái trên đại số $C = B\otimes_KA^o$, đại số này là đơn theo Mệnh đề 7 của VIII, p. 221. Với tư cách các A-môđun phải, $A^f$ và $A^g$ đẳng cấu với $A_d$, nên có độ dài hữu hạn vì vành A là đơn (VIII, p. 121, Hệ quả 1). A fortiori, $A^f$ và $A^g$ là các C-môđun có độ dài hữu hạn. Gọi S là một C-môđun đơn; tồn tại các số nguyên dương ngặt $m$ và $n$ sao cho $A^f$ đẳng cấu với $S^m$ và $A^g$ với $S^n$. Khi đó A-môđun phải S có độ dài hữu hạn khác không. Vì các A-môđun phải nền tảng của $A^f$ và $A^g$ là đẳng cấu, chúng có cùng độ dài; do đó ta có $m=n$, suy ra các C-môđun $A^f$ và $A^g$ là đẳng cấu.

#### Hệ quả 1 {#alg-viii-s14-thm-3-cor-1 .statement tag=00GS}

Cho A là một đại số đơn tâm trên K, và L là một mở rộng của K có bậc hữu hạn. Nếu $f$ và $g$ là các đồng cấu đại số trên K từ L vào A, thì tồn tại một tự đẳng cấu trong $\theta$ của A sao cho $g=\theta \circ f$.

#### Hệ quả 2 {#alg-viii-s14-thm-3-cor-2 .statement tag=00GT}

Cho A là một đại số đơn tâm trên K, và L là một đại số con của A là một trường. Mọi đồng cấu đại số trên K từ L vào A đều mở rộng thành một tự đẳng cấu trong của A.

#### Hệ quả 3 {#alg-viii-s14-thm-3-cor-3 .statement tag=00GU}

Cho D là một trường có bậc hữu hạn trên K và có tâm là K. Mọi phần tử của D đều đại số trên K. Cho $x$ và $y$ là các phần tử của D; tồn tại một phần tử $a$ của $D^*$ sao cho $y=axa^{-1}$ khi và chỉ khi $x$ và $y$ có cùng đa thức tối tiểu trên K.

Mệnh đề thứ nhất suy ra từ Hệ quả 1 của V, §3, No. 1, p. 17.

Giả sử rằng tồn tại một phần tử $a$ của $D^*$ sao cho $y=axa^{-1}$; với mọi đa thức P của K[X], ta có $P(y) =aP(x)a^{-1}$, và, đặc biệt, ta có $P(x) = 0$ khi và chỉ khi $P(y) = 0$. Do đó, $x$ và $y$ có cùng đa thức tối tiểu trên K (V, §3, No. 1, p. 16, Định lý 1).

Ngược lại, giả sử rằng $x$ và $y$ có cùng đa thức tối tiểu. Theo loc. cit., tồn tại một K-đẳng cấu $u$ từ $K[x]$ đến $K[y]$ sao cho $u(x) =y$, và $K[x]$ là một trường. Theo Hệ quả 2$,u$ kéo dài thành một tự đẳng cấu trong $\theta :z\mapsto aza^{-1}$ của D, và do đó ta có $y=\theta (x) =axa^{-1}$.

#### Mệnh đề 1 {#alg-viii-s14-prop-1 .statement tag=00GV}

Cho A là một đại số đơn tâm bậc hữu hạn trên K. Cho B là một đại số trên K, và cho $f$ và $g$ là các đồng cấu đại số từ B vào A. Các tính chất sau là tương đương:

(i) Tồn tại một tự đẳng cấu trong $\theta$ của A sao cho $g=\theta \circ f$.

(ii) Với tư cách là các B-môđun trái, $A^f$ và $A^g$ là đẳng cấu.

Theo Bổ đề 1 (VIII, p. 254), tính chất (i) tương đương với việc $A^f$ và $A^g$ là đẳng cấu như các song môđun $(B$, A). Vì A là hữu hạn chiều trên $K, A^f$ và $A^g$ là các B-môđun có độ dài hữu hạn. Vì tâm của A bằng K, suy ra tính tương đương của (i) và (ii) từ Bổ đề 2 của VIII, p. 254 áp dụng cho các song môđun $(A^o,B^o$) $A^f$ và $A^g$.

### 4. Tự đẳng cấu của các đại số nửa đơn

#### Định lý 4 {#alg-viii-s14-thm-4 .statement tag=00GW}

Cho A là một vành nửa đơn, Z là tâm của nó, và $u$ là một tự đẳng cấu của A. Giả sử rằng A là một Z-môđun sinh hữu hạn và ta có $u(z) =z$ với mọi $z$ trong Z. Khi đó $u$ là một tự đẳng cấu trong.

Điều này suy ra từ Định lý 2 của VIII, p. 256 áp dụng với $f=$ Id$_A$ và $g=u$.

#### Ví dụ {#alg-viii-s14-n4-exa-1 .statement tag=00RH}

Định lý 4 áp dụng được trong hai trường hợp riêng sau đây:

a) Cho D là một trường và Z là tâm của nó. Nếu D có bậc hữu hạn trên Z, thì mọi tự đẳng cấu của D cố định các phần tử của Z đều là một tự đẳng cấu trong. Giả thiết D có bậc hữu hạn trên Z là cốt yếu (VIII, p. 269, Bài tập 4).

b) Cho V là một không gian vectơ hữu hạn chiều trên trường K. Mọi tự đẳng cấu của đại số trên K End$_K(V)$ đều là một tự đẳng cấu trong; kết quả này mở rộng cho trường hợp không gian V không hữu hạn chiều trên K (VIII, p. 272, Bài tập 13).

Đặc biệt, mọi tự đẳng cấu của một đại số ma trận $\mathbf{M}_n(K)$ (với $n\geqslant$ 1) đều là một tự đẳng cấu trong. Kết quả này có phép tổng quát hóa sau đây.

#### Mệnh đề 2 {#alg-viii-s14-prop-2 .statement tag=00GX}

Cho L là một vành giao hoán và V là một L-môđun tự do có chiều $m$. Giả sử rằng mọi L-môđun M sao cho $M^m$ đẳng cấu với $L^m$ đều đẳng cấu với L. Khi đó mọi tự đẳng cấu của đại số trên L End$_L(V)$ đều là một tự đẳng cấu trong.

Đặt B = End$_L(V)$. Cho $u$ là một tự đẳng cấu của đại số trên L B. Ta xem V như một B-môđun trái; gọi $u_*(V)$ là B-môđun trái liên kết với $u$, với phép toán ngoài $(b, v)\mapsto u(b)(v)$ (II, §1, No. 13, p. 221). Gọi $(e_1, . . . , e_m)$ là một cơ sở của L-môđun V; với các phần tử $v_1, . . . , v_m$ của V đã cho, tồn tại một phần tử duy nhất $b$ của B sao cho ta có $b(e_i) =v_i$ với $1\leqslant i\leqslant m$. Nói cách khác, phần tử $e= (e_1, . . . , e_m)$ của $V^m$ xác định một cơ sở của B-môđun $V^m$. Vì $u$ là một tự đẳng cấu, $e$ cũng xác định một cơ sở của B-môđun $u_*(V^m) =u_*(V)^m$, do đó môđun này đẳng cấu với $V^m$. Song môđun $(B$, L)-môđun V là khả nghịch (VIII, p. 102, Ví dụ 1). Theo Định lý 2, b) của VIII, p. 103, do đó tồn tại một L-môđun M sao cho B-môđun $u_*(V)$ đẳng cấu với $V\otimes_LM$. Các B-môđun $V\otimes_LL^m$ và $V\otimes_LM^m$, lần lượt đẳng cấu với $V^m$ và $u_*(V)^m$, vì vậy là đẳng cấu với nhau. Theo chỗ đã dẫn, các L-môđun $L^m$ và $M^m$ là đẳng cấu. Theo giả thiết, M đẳng cấu với L; do đó, B-môđun $u_*$(V), vốn đẳng cấu với $V\otimes_LM$, là đẳng cấu với V. Gọi $h$ là một đẳng cấu B-môđun từ V lên $u_*(V)$; đặc biệt, đó là một tự đẳng cấu của L-môđun V, tức là một phần tử khả nghịch của B. Với $b$ trong B và $v$ trong V, ta có $h(b(v)) =u(b)(h(v))$ và do đó $u(b) =hbh^{-1}$.

Các điều kiện của Mệnh đề 2, đặc biệt, được thỏa mãn khi vành giao hoán L là một miền iđêan chính (VII, §3, p. 15, Hệ quả 3) hoặc là Artin (VIII, p. 37, Định lý 2, d)) hoặc địa phương (VIII, p. 36, Hệ quả 6).

### 5. Các Đại Số Con Đơn Của Các Đại Số Đơn

#### Định lý 5 {#alg-viii-s14-thm-5 .statement tag=00GY}

Cho A là một đại số đơn tâm trên K, và B là một đại số con nửa đơn của A có bậc hữu hạn trên K.

a) Hoán tập $B'$ của B trong A là một đại số con đơn, và B là hoán tập của $B'$ trong A. Hơn nữa, đại số $B\cap B'$ là một đại số giao hoán nửa đơn có bậc hữu hạn trên K; nó là tâm chung của B và $B'$.

b) Giả sử B là đơn. Khi đó $B'$ là đơn, và ta có các đẳng thức

$$
[A : B']_s= [B : K],[A : B]_s= [B': K],[A : K] = [B : K][B': K]
$$

(Xem VIII, p. 124, Định nghĩa 2 để biết định nghĩa của bậc trái $[A : B]_s.$)

K-đại số $A^o$ là đơn tâm, và K-đại số B là nửa đơn và có bậc hữu hạn. Theo Hệ quả 1 của VIII, p. 221, đại số $C = B\otimes_KA^o$ là nửa đơn. Cho M là C-môđun có cùng nhóm cộng với A và có phép toán ngoài được cho bởi công thức $(b\otimes a)a'=ba'a$ với $a, a'$ trong A và $b$ trong B. Cho $u$ là một phần tử của End$_{\mathbf{Z}}(A)$. Khi đó $u$ thuộc hoán tập $C'_M$ của C-môđun M khi và chỉ khi $u$ là A-tuyến tính phải và B-tuyến tính trái, nói cách khác, khi và chỉ khi $u$ thuộc hoán tập của $B_M$ trong vành các phép vị tự của A-môđun $A_s$. Do đó ta định nghĩa một đẳng cấu $\gamma$ từ $B'$ lên $C'_M$ bởi quan hệ $\gamma (b')(x) =b'x$ với $b'$ trong $B'$ và $x$ trong M. Bây giờ, vành C là nửa đơn, và C-môđun M được sinh bởi phần tử 1 của A. Theo Mệnh đề 6 của VIII, p. 139, vành $C'_M$ là nửa đơn, nên đại số $B'$ là nửa đơn.

Cho $\varphi$ là đồng cấu đại số trên K từ $A\otimes_KA^o$ vào End$_K(M)$ biến $a\otimes a'$ thành ánh xạ K-tuyến tính $x\mapsto axa'$ từ M vào M. Vì các đại số trên K A và $A^o$ là đơn tâm, các iđêan hai phía duy nhất của $A\otimes_KA^o$ là 0 và $A\otimes_KA^o$ (VIII, p. 218, Hệ quả). Ta có $C_M=\varphi (B\otimes A^o)$ và $C'_M=\varphi (B'\otimes K)$. Đồng cấu $\varphi$ khác không; do đó nó là đơn ánh. Vì vành C là nửa đơn, ta có $C''_M= C_M$ theo Mệnh đề 5 của VIII, p. 139. Suy ra đại số con $B\otimes_KA^o$ của $A\otimes_KA^o$ là hoán tập của đại số con $B'\otimes_KK$. Vậy hoán tập của $B'\otimes_KK$ trong $A\otimes_KK$ bằng $(B\otimes_KA^o)\cap (A\otimes_KK)$, tức là bằng $B\otimes K$ theo Mệnh đề 19 của II, §7, No. 9, p. 311. Do đó hoán tập của $B'$ trong A bằng B. Đại số $L = B\cap B'$ là tâm của B. Vì B là một đại số nửa đơn bậc hữu hạn trên K, đại số L là giao hoán và nửa đơn và có bậc hữu hạn trên K. Vì B là hoán tập của $B'$ trong A, tâm của $B'$ cũng bằng $L = B\cap B'$ (VIII, p. 77). Ta đã chứng minh a).

Bây giờ giả sử rằng đại số B là đơn. Theo Hệ quả 2 của VIII, p. 222, vành C là đơn. Theo Mệnh đề 4 của VIII, p. 123 áp dụng cho C-môđun M, mà hoán tập của nó đẳng cấu với $B'$, vành $B'$ là đơn và M là một $B'$-môđun có độ dài hữu hạn. Nói cách khác, $B'$ là một vành con đơn của vành đơn A, và bậc trái $[A : B']_s$ là một số nguyên $m\geqslant 1$. Được xem như một $B'$-môđun trái, A có một cơ sở hữu hạn $(a_1, . . . , a_m)$. Hơn nữa (loc. cit.), $\varphi$ cảm sinh, qua hạn chế, một đẳng cấu từ C lên $C''_M=$ End$_{B'}$(A), và do đó ánh xạ $c\mapsto (ca_1, . . . , ca_m)$ từ C vào $A^m$ là song ánh. Do đó, C là một A-môđun phải tự do có chiều $m$. Bây giờ, ta có $C = B\otimes A^o$, nên C là một A-môđun phải tự do có chiều [B : K]; suy ra $[A : B']_s=m= [B : K]$. Từ Mệnh đề 6 của VIII, p. 125, ta suy ra

$$
[A : K] = [A : B']_s[B': K] = [B : K] [B': K]
$$

vì ta cũng có

$$
[A : K] = [A : B]_s[B : K]
$$

và [B : K] là hữu hạn và khác không, ta kết luận rằng ta có đẳng thức $[A : B]_s= [B': K] ($Lý thuyết tập hợp, III, §6, No. 3, p. 188, Hệ quả 3). Ta đã chứng minh b).

Cho A là một đại số đơn tâm trên K có bậc hữu hạn. Có thể tồn tại các đại số con giao hoán nửa đơn B của A thỏa mãn $[A : K]\not=$ $[B : K] [B': K]$ (Bài tập 1 của VIII, p. 269).

#### Định lý 6 {#alg-viii-s14-thm-6 .statement tag=00GZ}

Cho A là một đại số đơn tâm trên K, B là một đại số con của A có bậc hữu hạn, và $B'$ là hoán tập của nó trong A.

a) Giả sử rằng B là đơn tâm. Khi đó $B'$ là đơn tâm, và đồng cấu đại số trên K $\theta : B\otimes_KB'\rightarrow A$ biến $b\otimes b'$ thành $bb'$ là một đẳng cấu.

b) Giả sử rằng B là nửa đơn, và đặt $L = B\cap B'$. Khi đó $B'$ là một đại số nửa đơn. Hoán tập $L'$ của L trong A là một vành nửa đơn có tâm là L, và đồng cấu vành $\psi : B\otimes_LB'\rightarrow L'$ gửi $b\otimes b'$ tới $bb'$ là một đẳng cấu.

Hãy chứng minh a). Nếu B là đơn tâm, thì $B'$ là đơn tâm theo Định lý 5 của VIII, p. 259. Do đó K-đại số $B\otimes_KB'$ là đơn (VIII, p. 222, Hệ quả 2), và đồng cấu $\theta : B\otimes_KB'\rightarrow A$ là đơn ánh. Bây giờ, theo đẳng thức của $[A : B']_s$ và [B : K] (Định lý 5), các $B'$-môđun trái $B\otimes_KB'$ và A là các môđun tự do có cùng số chiều hữu hạn; vì thế chúng là các $B'$-môđun có cùng độ dài hữu hạn. Theo Hệ quả 2 của II, §1, No. 10, p. $213,\theta$ là song ánh.

Hãy chứng minh b). Theo Định lý 5, đại số L là giao hoán, có bậc hữu hạn trên K, và nửa đơn. Theo chỗ đã dẫn áp dụng cho L, hoán tập $L'$ của nó trong A là một đại số nửa đơn, và L là hoán tập của $L'$ trong A, nên L là tâm của $L'$. Vì L là tâm của các vành nửa đơn $L', B$, và $B'$, ta có thể đồng nhất $L'$ với một tích hữu hạn các vành đơn $L'_i$ (với $i\in I$), sao cho ta có

$$
L =\prod_{i\in I}L_i,B =\prod_{i\in I}B_i,B'=\prod_{i\in I}B'_i
$$

trong đó $L_i$ là tâm của $L'_i$ và $B_i$ và $B'_i$ là các đại số con của $L'_i$ có tâm là $L_i$ và là các đối giao hoán tử của nhau trong $L'_i$. Ta xem $L'_i$ như một đại số đơn tâm trên trường giao hoán $L_i$ và $B_i$ như một $L_i$-đại số đơn tâm bậc hữu hạn. Theo mệnh đề a), ánh xạ chính tắc $\psi_i: B_i\otimes_{L_i}B'_i\rightarrow L'_i$ biến $b_i\otimes b'_i$ thành $b_ib'_i$ là một đẳng cấu vành. Bây giờ, ta có thể đồng nhất $B\otimes_LB'$ với $\prod_{i\in I}(B_i\otimes_{L_i}B'_i)$, sao cho $\psi$ là tích của họ các ánh xạ $(\psi_i)_{i\in I}$. Do đó, $\psi$ là một đẳng cấu vành.

#### Hệ quả {#alg-viii-s14-n5-cor-1 .statement tag=00H0}

Giả sử trường K là đóng đại số và A là một đại số đơn bậc hữu hạn trên K. Cho B là một đại số con đơn của A, và gọi $B'$ là hoán tập của B trong A. Khi đó $B'$ là một đại số đơn trên K, B là hoán tập của $B'$, ta có $[A : K] = [B : K][B': K]$, và đồng cấu chính tắc từ $B\otimes_KB'$ vào A là một đẳng cấu đại số trên K.

Vì mọi đại số đơn bậc hữu hạn trên K đều là trung tâm, hệ quả suy ra từ Định lý 5 và 6.

### 6. Các Đại Số Con Giao Hoán Cực Đại

Ta nói rằng một đại số con của một đại số trên K A là một đại số con giao hoán cực đại của A nếu nó là một phần tử cực đại của tập hợp các đại số con giao hoán của A.

#### Bổ đề 3 {#alg-viii-s14-lem-3 .statement tag=00H1}

Cho A là một đại số trên K và L là một đại số con của A.

a) Đại số L là một đại số con giao hoán cực đại của A khi và chỉ khi L bằng hoán tập của nó $L'$ trong A.

b) Cho $K'$ là một đại số giao hoán trên K khác không. Khi đó L là một đại số con giao hoán cực đại của A khi và chỉ khi $L_{(K')}$ là một đại số con giao hoán cực đại của $A_{(K')}$.

Ta hãy chứng minh a). Trước hết giả sử rằng L bằng $L'$. Khi đó L là giao hoán; nếu M là một đại số con giao hoán của A chứa L, thì ta có $xy=yx$ với $x$ thuộc L và $y$ thuộc M, nên $M\subset L'$ và do đó M = L. Vậy L là một đại số con giao hoán cực đại của A.

Ngược lại, giả sử rằng L là một đại số con giao hoán cực đại của A, và gọi $x$ là một phần tử của $L'$. Khi đó đại số con M của A sinh bởi $L\cup  \{x\}$ là giao hoán và chứa L. Vì L là cực đại, ta có M = L, do đó $x\in L$ và cuối cùng $L = L'$, điều này cho a).

Theo Mệnh đề 6 của III, §4, No. 4, p. 468, hoán tập của $L_{(K')}$ trong $A_{(K')}$ là $L'_{(K')}$. Vì các đẳng thức $L = L'$ và $L_{(K')}= L'_{(K')}$ là tương đương (II, §7, No. 9, p. 311, Mệnh đề 19), mệnh đề b) suy ra từ a).

#### Mệnh đề 3 {#alg-viii-s14-prop-3 .statement tag=00H2}

Cho A là một đại số đơn tâm trên K có bậc hữu hạn, và L là một đại số con giao hoán nửa đơn của A. Các tính chất sau là tương đương:

(i) Đại số L là một đại số con giao hoán cực đại của A.

(ii) L-môđun trái A là tự do, có chiều [L : K].

(iii) Ta có $[A : K] = [L : K]^2$.

Giả sử thêm rằng A là đại số End$_K(V)$, trong đó V là một không gian vectơ có chiều hữu hạn khác không trên K. Khi đó các tính chất trên cũng tương đương với tính chất sau:

(iv) V là một L-môđun tự do có chiều 1.

A) Giả sử rằng A có dạng End$_K$(V), trong đó V là một không gian vectơ có chiều hữu hạn khác không trên trường K. Ta sẽ thiết lập tính tương đương của các điều kiện (i) đến (iv) theo biểu đồ

(i) $=\Rightarrow$ (iv) $=\Rightarrow$ (ii) $=\Rightarrow$ (iii) $=\Rightarrow$ (i) .

Vì L là một đại số giao hoán nửa đơn bậc hữu hạn trên K, ta có thể đồng nhất nó với một tích hữu hạn $\prod_{i\in I}L_i$ của các mở rộng của K bậc hữu hạn (VIII, p. 137, Mệnh đề 3). Với mọi $i\in I$, gọi $V_i$ là thành phần đẳng kiểu kiểu $L_i$ của L-môđun V; đó là một không gian vectơ có số chiều hữu hạn khác không trên $L_i$ vì V là một L-môđun trung thành (VIII, p. 144, Hệ quả). Khi đó ta có thể đồng nhất V với $\prod_{i\in I}V_i$. Trong những điều kiện này, hoán tập $L'$ của L trong A, vốn chính là đại số End$_L$(V), có thể được đồng nhất với tích $\prod_{i\in I}$ End$_{L_i}(V_i)$.

Giả sử rằng L là một đại số con giao hoán cực đại của End$_K(V)$. Theo Bổ đề 3, a), ta có $L = L'$, nên $L'$ giao hoán và ta có dim$_{L_i}(V_i) = 1$ với mọi $i\in I$. Do đó (i) suy ra (iv).

Giả sử L-môđun V là tự do chiều 1. Gọi $(e_1, . . . , e_r)$ là một cơ sở của V trên K. Ánh xạ $a\mapsto (ae_1, . . . , ae_r)$ là một đẳng cấu của các A-môđun trái và do đó của các L-môđun từ A đến $V^r$. Do đó, A là một L-môđun trái tự do chiều $r$, và ta có $r=$ dim$_K(V) = [L : K]$. Vậy (iv) suy ra (ii).

Rõ ràng là (i) suy ra (iii).

Cuối cùng, giả sử rằng ta có $[A : K] = [L : K]^2$, nói cách khác, dim$_K(V) = [L : K]$. Khi đó ta có $\sum_i$ dim$_{L_i}(V_i)[L_i: K] =\sum_i[L_i: K]$, do đó $V_i$ có chiều bằng 1 trên $L_i$ với mọi $i$. Khi đó ta có End$_{L_i}(V_i) = L_i$ với mọi $i$, và vì thế $L'= L$. Theo Bổ đề 3, a), L là một đại số con giao hoán cực đại của A. Vậy (iii) suy ra (i).

B) Ta tiếp tục với trường hợp tổng quát. Theo Định lý 1 của VIII, p. 252, tồn tại một mở rộng tách được $K'$ của K có bậc hữu hạn sao cho $K'$-đại số $A_{(K')}$ đẳng cấu với một đại số End$_{K'}(V')$, trong đó $V'$ là một không gian vectơ có chiều hữu hạn khác không trên $K'$. Khi đó $K'$-đại số $L_{(K')}$ là giao hoán và nửa đơn (VIII, p. 222, Hệ quả 2). Theo phần đầu của chứng minh, các tính chất sau là tương đương:

(i$'$) Đại số $L_{(K')}$ là một đại số con giao hoán cực đại của $A_{(K')}$.

(ii$'$) Môđun trái $L_{(K')}$-môđun $A_{(K')}$ là tự do, có chiều $[L_{(K')}: K']$.

(iii$'$) Ta có $[A_{(K')}: K'] = [L_{(K')}: K']^2$.

Theo Bổ đề 3, b), các tính chất (i) và (i’) là tương đương.

Đặt $n= [L : K]$; khi đó $n= [L_{(K')}: K']$. Tính chất (ii) có nghĩa là các L-môđun trái A và $L^n$ là đẳng cấu; theo Định lý 3 của VIII, p. 37, điều này tương đương với việc các $L_{(K')}$-môđun $A_{(K')}$ và $(L_{(K')})^n$ là đẳng cấu. Suy ra tính tương đương của (ii) và (ii$'$).

Sau cùng, ta có $[A : K] = [A_{(K')}: K']$ và $[L : K] = [L_{(K')}: K']$, từ đó suy ra tính tương đương của các tính chất (iii) và (iii$'$). Như vậy ta đã chứng minh được tính tương đương của các tính chất (i), (ii), và (iii).

#### Hệ quả {#alg-viii-s14-n6-cor-1 .statement tag=00H3}

Cho A là một đại số đơn tâm bậc hữu hạn trên K, và cho L là một đại số giao hoán trên K nửa đơn sao cho [A : K] bằng $[L : K]^2$. Cho $f$ và $g$ là các đồng cấu đơn ánh từ L vào A. Tồn tại một tự đẳng cấu trong $\theta$ của A sao cho $g=\theta \circ f$.

Đặt $n= [L : K]$. Khi được xem như một môđun trái trên vành con $f$(L), A là tự do chiều $n$; điều này suy ra từ tính tương đương của các tính chất (ii) và (iii) của Mệnh đề 3. Vì $f$ là một đẳng cấu từ L lên $f$(L), L-môđun trái $A^f$ (mà luật tác động được cho bởi $(x, a)\mapsto f(x)a$) là tự do chiều $n$. Điều tương tự cũng đúng với $A^g$, do đó nó đẳng cấu với $A^f$. Ta kết luận bằng cách sử dụng tính tương đương của các tính chất (i) và (ii) của Mệnh đề 1 (VIII, p. 257).

Giả sử rằng A là một đại số đơn tâm bậc hữu hạn trên K. Có thể tồn tại các đại số con giao hoán cực đại L của A không nửa đơn và sao cho $[A : K]\not= [L : K]^2$ (VIII, p. 270, Bài tập 5).

### 7. Các Đại Số Con Étale Cực Đại

#### Bổ đề 4 {#alg-viii-s14-lem-4 .statement tag=00H4}

Cho A là một đại số đơn tâm bậc hữu hạn trên K, khác K. Tồn tại một đại số con étale (V, §6, No. 3, p. 28, Định nghĩa 1) của A khác K.

Theo định lý của Wedderburn (VIII, p. 120, Định lý 1), ta có thể giả sử rằng A có dạng $\mathbf{M}_n$(D), trong đó $n$ là một số nguyên dương ngặt và D là một trường có tâm là K.

Giả sử $n >1$. Đại số các ma trận đường chéo với các phần tử thuộc K là một đại số con étale của A khác K.

Giả sử $n= 1$. Gọi $p$ là số mũ của đặc số của D. Theo Bổ đề 1 của VIII, p. 230, tồn tại một phần tử $a$ của D sao cho $a^{p^m}$ không thuộc K với bất kỳ số tự nhiên $m$ nào. Vậy, với $m$ đủ lớn, phần tử $x=a^{p^m}$ là tách được trên K (V, §7, No. 7, p. 44, Mệnh đề 13), nhưng nó không thuộc K. Đại số con $K(x)$ của A là một mở rộng tách được của trường K với bậc hữu hạn, do đó là một đại số con étale trên K; nó khác K.

#### Mệnh đề 4 {#alg-viii-s14-prop-4 .statement tag=00H5}

Cho A là một đại số đơn tâm bậc hữu hạn trên K. Gọi L là một đại số con của A, và gọi $L'$ là hoán tập của L trong A.

a) Nếu L là cực đại trong số các đại số con giao hoán nửa đơn của A, thì ta có $L = L'$, và L là một đại số con giao hoán cực đại của A.

b) Nếu L là cực đại trong số các đại số con étale của A, thì ta có $L = L'$, và L là một đại số con giao hoán cực đại của A.

Ta biết rằng quan hệ $L = L'$ có nghĩa là L là một đại số con giao hoán cực đại của A (VIII, p. 261, Bổ đề 3, a)). Giả sử rằng L là nửa đơn, giao hoán, và phân biệt với $L'$. Theo Định lý 5 của VIII, p. 259$, L'$ là nửa đơn, và L là hoán tập của $L'$ và do đó là tâm của $L'$; do đó, $L'$ không giao hoán. Chỉ cần chứng minh rằng tồn tại một đại số con giao hoán nửa đơn M của A, phân biệt với L và chứa L, và étale nếu L là étale.

Theo định lý cấu trúc của các vành nửa đơn (VIII, p. 135, Định lý 1), tồn tại các vành đơn $B_1, . . . ,B_r$ và một đẳng cấu $\varphi$ từ $L'$ lên $B_1\times  \cdots  \times B_r$. Với $1\leqslant i\leqslant r$, ký hiệu tâm của $B_i$ là $E_i$; khi đó ta có $\varphi (L) = E_1\times  \cdots  \times E_r$. Vì $L'$ không giao hoán, chẳng hạn, ta có thể giả sử rằng $B_1$ không giao hoán; do đó $B_1\not= E_1$, và, theo Bổ đề 4, tồn tại một đại số con $M_1$ của $B_1$ giao hoán, phân biệt với $E_1$, và étale trên $E_1$. Đặt $M =\varphi^{-1}(M_1\times E_2\times  \cdots  \times E_r)$; đó là một đại số con giao hoán nửa đơn của A chứa L và phân biệt với L. Giả sử rằng L là étale trên K; hãy chứng minh rằng M là étale. Các mở rộng $E_i$ của K là tách được (V, §6, No. 4, p. 30, Mệnh đề 3). Hơn nữa, vì đại số trên $E_1$ là $M_1$ và đại số trên K là $E_1$ đều là étale, nên đại số trên K là $M_1$ cũng là étale (V, §6, No. 5, p. 32, Hệ quả 2). Do đó đại số trên K $M_1\times E_2\times  \cdots  \times E_r$ là étale, và vì thế M cũng vậy.

Cho A là một đại số đơn tâm bậc hữu hạn trên K. Một đại số con của A cực đại trong số các đại số con giao hoán nửa đơn của A được gọi là một đại số con giao hoán nửa đơn cực đại của A. Theo Mệnh đề 4, thuật ngữ “cực đại” quy chiếu đến tính chất giao hoán, hoặc đến tính chất vừa nửa đơn vừa giao hoán. Một đại số con của A cực đại trong số các đại số con étale của A được gọi là một đại số con étale cực đại của A.

#### Hệ quả 1 {#alg-viii-s14-prop-4-cor-1 .statement tag=00H6}

Cho A là một đại số đơn tâm trên K bậc hữu hạn. Mọi đại số con giao hoán nửa đơn (tương ứng, étale) của A đều được chứa trong một đại số con giao hoán cực đại của A mà nửa đơn (tương ứng, étale).

#### Hệ quả 2 {#alg-viii-s14-prop-4-cor-2 .statement tag=00H7}

Cho D là một trường bậc hữu hạn trên K có tâm là K.

a) Các trường con giao hoán cực đại của D là các đại số con giao hoán cực đại của D và cũng là các đại số con giao hoán nửa đơn cực đại của D. Mọi trường con giao hoán L của D đều được chứa trong một trường con giao hoán cực đại.

b) Cho L là một trường con giao hoán của D là một mở rộng tách được của K; nó được chứa trong một trường con giao hoán cực đại của D là một mở rộng tách được của K.

c) Cho L là một trường con giao hoán của D. Khi đó L là một trường con giao hoán cực đại của D nếu và chỉ nếu ta có $[D : K] = [L : K]^2$.

Một đại số con của D là một trường (V, §2, No. 2, p. 10, Mệnh đề 1), do đó là nửa đơn. Hơn nữa, một trường con giao hoán cực đại của D chứa K. Các mệnh đề a) và b) khi đó suy ra từ Hệ quả 1 và mệnh đề c) của Mệnh đề 3 (VIII, p. 262).

#### Mệnh đề 5 {#alg-viii-s14-prop-5 .statement tag=00H8}

Cho A là một đại số đơn tâm bậc hữu hạn trên K. Cho B là một đại số con nửa đơn của A, và gọi $B'$ là hoán tập của B.

a) Đại số B chứa một đại số con giao hoán nửa đơn cực đại của A nếu và chỉ nếu B chứa $B'$.

b) Giả sử B chứa $B'$, và cho $g$ là một đồng cấu đại số trên K từ B vào A. Tồn tại một tự đẳng cấu trong $\theta$ của A trùng với $g$ trên B.

Cho L là một đại số con giao hoán cực đại của A; theo Bổ đề 3 của VIII, p. 261, L bằng hoán tập $L'$ của nó trong A. Nếu B chứa L, thì hoán tập $B'$ của nó được chứa trong $L'$, và do đó trong B.

Ngược lại, giả sử rằng $B'$ được chứa trong B. Khi đó $B'$ là tâm của B, và nó là một đại số giao hoán nửa đơn (VIII, p. 137, Mệnh đề 2). Theo Hệ quả 1, tồn tại một đại số con giao hoán nửa đơn cực đại L của A chứa $B'$. Hoán tập của L là L (VIII, p. 261, Bổ đề 3, a)), và hoán tập của $B'$ bằng B (VIII, p. 259, Định lý 5). Do đó quan hệ $L\supset B'$ kéo theo $L\subset B$. Ta đã chứng minh a).

Ta hãy chứng minh b). Giả sử rằng B chứa $B'$, và chọn một đại số con giao hoán nửa đơn cực đại L của A được chứa trong B, mà sự tồn tại được bảo đảm bởi a). Cho $g$ là một đồng cấu từ B vào A. Theo Mệnh đề 3 của VIII, p. 262, ta có đẳng thức $[A : K] = [L : K]^2$; theo hệ quả của VIII, p. 263, tồn tại một tự đẳng cấu trong $\theta_1$ của A trùng với $g$ trên L. Nếu $f$ là đơn ánh chính tắc của B vào A, thì các đồng cấu $g$ và $\theta_1\circ f$ có cùng hạn chế lên tâm $B'$ của B vì $B'$ được chứa trong L. Theo Định lý 2 của VIII, p. 256, tồn tại một tự đẳng cấu trong $\theta$ của A sao cho $g=\theta \circ f$; nói cách khác, $\theta$ mở rộng $g$.

### 8. Các Đại số con Chéo hóa được của các Đại số Đơn

Cho D là một đại số trên K đồng thời là một trường, và cho V là một không gian vectơ phải hữu hạn chiều trên D. Cho L là một đại số con trên K của End$_D(V)$ mà là một đại số trên K chéo hóa được (V, §6, No. 3, p. 28). Theo định nghĩa, L có bậc hữu hạn trên K, và tồn tại một cơ sở $(\varepsilon_i)_{i\in I}$ của L trên K có các tính chất sau:

$\varepsilon^2_i=\varepsilon_i, \varepsilon_i\varepsilon_j= 0$ if $i\not=j ,\sum_{i\in I}\varepsilon_i= 1$.

Đặt $V_i=\varepsilon_i(V)$ với mọi $i$ trong I; khi đó $(V_i)_{i\in I}$ là một họ các không gian con tuyến tính khác không của V có tổng trực tiếp là V (II, §1, No. 8, p. 209, Mệnh đề 12). Cho $u$ là một tự đồng cấu của V; khi đó $u$ thuộc L khi và chỉ khi với mọi $i\in I$, tồn tại một phần tử $\lambda_i$ của K sao cho $u(x) =\lambda_ix$ với mọi $x\in V_i$.

Ngược lại, giả sử rằng V là tổng trực tiếp của một họ $(V_i)_{i\in I}$ các không gian con tuyến tính khác không. Với mọi phần tử $\boldsymbol{\lambda }= (\lambda_i)_{i\in I}$ của $K^I$, ký hiệu bởi $u_{\boldsymbol{\lambda }}$ tự đồng cấu của không gian vectơ trên D V sao cho $u_{\boldsymbol{\lambda }}(x) =\lambda_ix$ với $x\in V_i$. Tập hợp L các tự đồng cấu $u_{\boldsymbol{\lambda }}$ với $\boldsymbol{\lambda }\in K^I$ là một đại số con chéo hóa được của End$_D(V)$ có họ $(\varepsilon_i)_{i\in I}$ làm cơ sở, trong đó $\varepsilon_i$ là phép chiếu có ảnh là $V_i$ và hạt nhân là $\sum_{j\not=i}V_j$. Ta nói rằng L là đại số con chéo hóa được của End$_D(V)$ liên kết với phân tích thành tổng trực tiếp $V =\oplus_{i\in I}V_i$. Ta có [L : K] = Card(I) $\leqslant$ dim$_D(V)$.

#### Mệnh đề 6 {#alg-viii-s14-prop-6 .statement tag=00H9}

Cho L là đại số con chéo hóa được của End$_D(V)$ liên kết với một phân tích thành tổng trực tiếp $V =\oplus_{i\in I}V_i$.

a) Đại số L là cực đại trong các đại số con chéo hóa được của đại số trên K End$_D(V)$ khi và chỉ khi mỗi $V_i$ có chiều 1 trên D.

b) Đại số L là một đại số con giao hoán cực đại của End$_D(V)$ khi và chỉ khi ta có D = K và mỗi $V_i$ có chiều 1 trên K.

Nếu mọi không gian vectơ $V_i$ đều có chiều 1 trên D, thì ta có

[L : K] = Card(I) = dim$_D(V)$,

nên L là cực đại trong các đại số con chéo hóa được của End$_D(V)$. Trong trường hợp đối lại, tồn tại một chỉ số $j\in I$ sao cho dim$_D(V_j)\geqslant 2$. Chọn hai không gian con tuyến tính khác không $V'_j$ và $V''_j$ của $V_j$ có tổng trực tiếp là $V_j$. Đại số con chéo hóa được của End$_D(V)$ liên kết với phân tích tổng trực tiếp $V = (\oplus_{i\in I-\{j\}}V_i)\oplus V'_j\oplus V''_j$ chứa L và không bằng L; suy ra mệnh đề a).

Hoán tập $L'$ của L trong End$_D(V)$ gồm các nội cấu có dạng $(x_i)\mapsto (u_i(x_i))$, với $(u_i)\in \prod_{i\in I}$ End$_D(V_i)$. Đại số L là một đại số con giao hoán cực đại của End$_D(V)$ khi và chỉ khi ta có $L = L'$ (VIII, p. 261, Bổ đề 3, a)). Do đó quan hệ này tương đương với “End$_D(V_i) = K$ với mọi $i\in$ I”; mệnh đề b) suy ra.

#### Mệnh đề 7 {#alg-viii-s14-prop-7 .statement tag=00HA}

Cho L là một đại số giao hoán bậc hữu hạn trên K. Các tính chất sau là tương đương:

(i) Đại số L là étale.

(ii) Tồn tại một mở rộng tách được của K có bậc hữu hạn mà chéo hóa K.

Hệ quả (ii)$\Rightarrow$(i) suy ra từ V, §6, No. 3, p. 29, Mệnh đề 2.

Ta chứng minh suy ra (i)$\Rightarrow$(ii). Gọi Ω là một bao đóng tách được của K. Theo Định lý 4 của V, §6, No. 7, p. 34, tồn tại các mở rộng $L_1, . . . ,L_n$ của K có bậc hữu hạn, được chứa trong Ω, sao cho L đẳng cấu với tích $L_1\times  \cdots  \times L_n$. Lấy N là một mở rộng Galois của K chứa các $L_i$ (V, §10, No. 1, p. 58), và chứng minh rằng $L_{(N)}$ là chéo hóa được. Theo định lý phần tử nguyên thủy (V, §7, No. 4, p. 40, Định lý 1), với mọi $i\in [1, n]$, tồn tại một đa thức bất khả quy tách được $P_i\in K[X]$ sao cho $L_i$ đẳng cấu với $K[X]/(P_i)$. Vì N là một mở rộng chuẩn tắc của K trong đó $P_i$ có một nghiệm, nên đa thức $P_i$ phân tích hoàn toàn trong N[X], với các nghiệm đơn. Do đó đại số trên K $L_{i(N)}$, đẳng cấu với $N[X]/(P_i)$, đẳng cấu với $N^{[L_i:K]}$. Suy ra $L_{(N)}$ là chéo hóa được.

#### Định lý 7 {#alg-viii-s14-thm-7 .statement tag=00HB}

Cho A là một đại số đơn tâm trên K có bậc hữu hạn và L là một đại số con của A. Các tính chất sau là tương đương:

(i) Đại số L là một dưới đại số étale cực đại của A.

(ii) Tồn tại một mở rộng $K'$ của K, một số nguyên $n\geqslant 1$, và một đẳng cấu $\theta$ từ $A_{(K')}$ lên $\mathbf{M}_n(K')$ biến $L_{(K')}$ thành tập hợp các ma trận đường chéo.

(iii) Tồn tại $K',n$, và $\theta$ như trong (ii), trong đó, hơn nữa, mở rộng $K'$ được giả thiết là Galois và có bậc hữu hạn.

Rõ ràng là (iii) suy ra (ii).

Nếu tính chất (ii) được thỏa mãn, thì $L_{(K')}$ là một đại số con giao hoán cực đại của $A_{(K')}$ (Mệnh đề 6), và nó chéo hóa được. Khi đó đại số trên K L là étale (V, §6, No. 3, p. 28, Định nghĩa 1), và là một đại số con giao hoán cực đại của A (VIII, p. 261, Bổ đề 3, b)). Ta đã chứng minh rằng (ii) suy ra (i).

Giả sử rằng tính chất (i) được thỏa mãn. Vì L là étale trên K, theo Mệnh đề 7, tồn tại một mở rộng Galois $K_1$ của K có bậc hữu hạn sao cho $K_1$-đại số $L_{(K_1)}$ là chéo hóa được. Đại số A là đơn tâm; theo (VIII, p. 252, Định lý 1), tồn tại một mở rộng Galois $K_2$, một không gian vectơ V có số chiều hữu hạn $n$ trên $K_2$, và một đẳng cấu $\theta$ từ $A_{(K_2)}$ đến End$_{K_2}(V)$. Theo Mệnh đề 1 của V, p. 55, ta có thể giả sử $K_1= K_2$. Theo Mệnh đề 4, b) của VIII, p. 264 và Bổ đề 3, b) của VIII, p. 261$, L_{(K')}$ là một đại số con giao hoán cực đại của $A_{(K')}$, nên $\theta (L_{(K')})$ là một đại số con giao hoán cực đại của End$_{K'}(V')$. Hãy áp dụng Mệnh đề 6 cho đại số chéo hóa được $\theta (L_{(K')}):$ tồn tại một cơ sở $(e_1, . . . , e_n)$ của $V'$ trên $K'$ sao cho $\theta (L_{(K')})$ gồm các tự đồng cấu của $V'$ có ma trận đường chéo đối với cơ sở này. Vậy (i) suy ra (iii).

### Bài tập {#alg-viii-s14-exercises}

Xem [các bài tập cho § 14](exercises/s14/).
