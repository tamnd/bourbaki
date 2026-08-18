---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 3
section_title: Simple Modules
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.45-A VIII.54
pdf_pages: 0062-0071
extraction: native
subsections:
    - "no": 1
      title: Simple Modules
      page: 45
      pdf_page: 62
    - "no": 2
      title: Schur’s Lemma
      page: 47
      pdf_page: 64
    - "no": 3
      title: Maximal Submodules
      page: 48
      pdf_page: 65
    - "no": 4
      title: Simple Modules over an Artinian Ring
      page: 50
      pdf_page: 67
    - "no": 5
      title: Classes of Simple Modules
      page: 51
      pdf_page: 68
statements: 23
exercises: 10
content_sha256: 02a9cb80ec97bc7a4a83b0a79c4843690e581796d0fc039f79a6449a8b9eb543
translated_from: content/en/alg/VIII/03_s3_simple_modules.md
source_content_sha256: 9e40062ed94f59647e41551dd0cb278c9eed5dbb96dcf569df5e17def2b733c5
translation_model: nemotron-3-ultra-free, hy3-free, gpt-5-6, laguna-s-2.1-free
translation_run: translate-vi-3cd88d6f
glossary_version: 30
glossary_terms_sha256: 93e91ec42496f45ab6dd608a04fc611155c0b48581d19d2a943fa835cce2a71a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. MÔĐUN ĐƠN

### 1. Môđun đơn

Nhắc lại định nghĩa sau (II, §1, No. 10, p. 212).

#### Định nghĩa 1 {#alg-viii-s3-def-1 .statement tag=0035}

Cho A là một vành. Một A-môđun M được gọi là đơn nếu nó khác không và không có môđun con nào phân biệt với 0 và M.

Một A-môđun M là đơn khi và chỉ khi M là một môđun đơn trên vành đồng dạng $A_M$ của nó. Mọi môđun đơn đều không phân tích được, có độ dài 1, và do đó là nguyên thủy (VIII, p. 31, Mệnh đề 4, b)).

#### Ví dụ 1 {#alg-viii-s3-n1-exa-1 .statement tag=0036}

Môđun $A_s$ là một A-môđun đơn khi và chỉ khi A là một trường (I, §9, No. 1, p. 115, Định lý 1). Các A-môđun đơn lúc này là các không gian vectơ chiều 1 trên trường A.

#### Ví dụ 2 {#alg-viii-s3-n1-exa-2 .statement tag=0037}

Cho A là một miền iđêan chính (VII, §1, No. 1, p. 1, Định nghĩa 1) mà không phải là trường. Với mọi phần tử bất khả quy $\pi$ của A, A-môđun $A_s/(\pi )$ là đơn, và mọi A-môđun đơn đều đẳng cấu với một môđun như vậy (VII, §4, No. 8, p. 25, Nhận xét 4). Với $n\geqslant 2$, A-môđun $A_s/(\pi^n)$ không phân tích được (VII, §4, No. 8, p. 24, Mệnh đề 8) nhưng không đơn.

#### Ví dụ 3 {#alg-viii-s3-n1-exa-3 .statement tag=0038}

Cho K là một trường, V là một không gian vectơ phải khác không trên trường K, và A là một vành con của vành End$_K(V)$ chứa các đồng cấu của V có hạng hữu hạn (ví dụ, A = End$_K(V))$). Chứng minh rằng V là một A-môđun đơn: cho W là một A-môđun con khác không của V và $x$ một phần tử khác không của W; tồn tại một dạng tuyến tính $\varphi$ trên V sao cho $\varphi (x)\not= 0$ (II, §7, No. 5, p. 300, Định lý 6). Với mọi $y$ trong V, ánh xạ $z\mapsto y\varphi (z)$, là tuyến tính và có hạng $\leqslant 1$, thuộc về A; do đó ta có $Ax= V$, từ đó a fortiori W = V, điều này chứng minh V là một A-môđun đơn.

#### Mệnh đề 1 {#alg-viii-s3-prop-1 .statement tag=00QZ}

Cho A là một vành.

a) Cho $\mathfrak{m}$ là một iđêan trái của A. A-môđun $A_s/\mathfrak{m}$ là đơn khi và chỉ khi $\mathfrak{m}$ là iđêan trái cực đại.

b) Cho M là một A-môđun đơn, và cho $x$ là một phần tử khác không của M. Ta có đẳng thức $M = Ax$, linh hóa tử $\mathfrak{m}$ của $x$ là một iđêan trái cực đại của A, và ánh xạ $a\mapsto ax$ xác định, bằng cách chuyển qua thương, một đẳng cấu từ $A_s/\mathfrak{m}$ đến M.

c) Cho M là một A-môđun khác không. Nếu ta có $M = Ax$ với mọi phần tử khác không $x$ của M, thì M là đơn.

Các môđun con của $A_s/\mathfrak{m}$ có dạng $\mathfrak{n}/\mathfrak{m}$, trong đó $\mathfrak{n}$ là một iđêan trái của A chứa $\mathfrak{m}$ (I, §4, No. 6, p. 41, Định lý 4); do đó, A-môđun $A_s/\mathfrak{m}$ là đơn khi và chỉ khi ta có $\mathfrak{m}\not= A$ và mọi iđêan trái $\mathfrak{n}$ của A chứa $\mathfrak{m}$ thỏa mãn $\mathfrak{n}/\mathfrak{m}= 0$ hoặc $\mathfrak{n}/\mathfrak{m}= A_s/\mathfrak{m}$, tức là, $\mathfrak{n}=\mathfrak{m}$ hoặc $\mathfrak{n}= A$. Điều này chứng minh a).

Theo các giả thiết của b), $Ax$ là một môđun con khác không của M, do đó bằng M. Do đó, ánh xạ $a\mapsto ax$ xác định, bằng cách chuyển qua thương, một đẳng cấu từ $A_s/\mathfrak{m}$ đến M; vì vậy A-môđun $A_s/\mathfrak{m}$ là đơn, và iđêan trái $\mathfrak{m}$ là cực đại theo a). Điều này chứng minh b).

Theo các giả thiết của c), cho N là một môđun con khác không của M. Nếu $x$ là một phần tử khác không của N, thì ta có $Ax\subset N$ và $Ax= M$, do đó M = N. Suy ra M là đơn.

#### Hệ quả 1 {#alg-viii-s3-prop-1-cor-1 .statement tag=0039}

Nếu vành A không rút gọn về 0, thì tồn tại các A-môđun đơn.

Thật vậy, theo định lý Krull (I, §8, No. 6, p. 104, Định lý 1), tồn tại các iđêan trái cực đại của A.

#### Hệ quả 2 {#alg-viii-s3-prop-1-cor-2 .statement tag=003A}

Cho A là một vành địa phương (VIII, p. 26, Định nghĩa 1) và $\mathfrak{r}$ là iđêan cực đại của nó. A-môđun $A_s/\mathfrak{r}$ là đơn, và mọi A-môđun đơn đều đẳng cấu với $A_s/\mathfrak{r}$.

#### Nhận xét 1 {#alg-viii-s3-n1-rem-1 .statement tag=003B}

Cho A là một vành giao hoán và $\mathfrak{m}$ là một iđêan của A. Khi đó $\mathfrak{m}$ là linh hóa tử (II, §1, No. 12, p. 219, Định nghĩa 11) của A-môđun $A_s/\mathfrak{m}$. Do đó, nếu $\mathfrak{m}$ và $\mathfrak{m}'$ là hai iđêan phân biệt của A, thì các A-môđun $A_s/\mathfrak{m}$ và $A_s/\mathfrak{m}'$ không đẳng cấu. Tồn tại một A-môđun đơn trung thành (II, §1, No. 12, p. 219) nếu và chỉ nếu (0) là một iđêan cực đại của A, tức là A là một trường.

#### Nhận xét 2 {#alg-viii-s3-n1-rem-2 .statement tag=003C}

Chúng ta có thể đưa ra một ví dụ về một vnh không giao hoán A và hai iđêan cực đại trái phân biệt $\mathfrak{m}$ và $\mathfrak{m}'$ của A sao cho các A-môđun $A_s/\mathfrak{m}$ và $A_s/\mathfrak{m}'$ đẳng cấu (VIII, p. 52, Bài tập 3).

### 2. Bổ đề Schur

#### Mệnh đề 2 {#alg-viii-s3-prop-2 .statement tag=003D}

Cho A là một vnh, M và N là hai A-môđun, và $f$ là một đồng cấu khác không từ M tới N.

a) Nếu M là đơn, thì $f$ là đơn ánh.

b) Nếu N là đơn, thì $f$ là toàn ánh.

c) Nếu M và N là đơn, thì $f$ là một đẳng cấu.

Hạt nhân của $f$ là một môđun con thực sự của M, và ảnh của $f$ là một môđun con khác không của N.

a) Nếu M là đơn, thì ta có Ker($f$) $= 0$, nên $f$ là đơn ánh.

b) Nếu N là đơn, thì ta có Im($f$) $= N$, nên $f$ là toàn ánh.

c) Nếu M và N đều đơn, thì $f$ vừa đơn ánh vừa toàn ánh.

#### Hệ quả (Bổ đề Schur) {#alg-viii-s3-n2-cor-1 .statement tag=00RZ}

Vành tự đồng cấu của một môđun đơn là một trường.

Nếu M là một A-môđun đơn, thì mọi phần tử khác không của vành khác không End$_A(M)$ đều khả nghịch (Mệnh đề 2, c)), nên End$_A(M)$ là một trường.

#### Định lý 1 {#alg-viii-s3-thm-1 .statement tag=003E}

Cho K là một trường giao hoán đóng đại số, A là một đại số trên K, và M là một A-môđun đơn. Giả sử chiều của M như một không gian vectơ trên K là hữu hạn hoặc, nói chung, nhỏ hơn chặt lực lượng của K. Khi đó vành tự đồng cấu của A-môđun M bao gồm các đồng biến $\alpha_M$ với $\alpha \in K$.

Cho E là vành tự đồng cấu của A-môđun M; theo hệ quả của Mệnh đề 2, nó là một trường và là một đại số trên trường K. Nếu xem M như một không gian vectơ trái trên trường E, thì ta có dim$_KM =$ (dim$_EM)[E : K]$ theo Mệnh đề 25 của II, §1, No. 13, p. 222, do đó dim$_KM\geqslant [E : K]$. Vì dim$_KM<$ Card(K) theo giả thiết, đẳng thức $E = K\cdot 1_M$ là hệ quả của bổ đề sau.

#### Bổ đề 1 {#alg-viii-s3-lem-1 .statement tag=003F}

Cho E là một trường và K là một trường con của tâm của E, khác E. Nếu trường K đóng đại số, thì ta có $[E : K]\geqslant$ Card(K).

Cho $x$ là một phần tử của E - K và L là trường con (giao hoán) của E sinh bởi $K\cup  \{x\}$. Vì K đóng đại số, $x$ là siêu việt trên K. Theo VII, §2, No. 3, p. 10, Định lý 2 và p. 11, các phần tử $(x-\alpha )^{-1}$ của L, trong đó $\alpha$ chạy qua K, độc lập tuyến tính trên K. Do đó ta có $[E : K]\geqslant [L : K]\geqslant$ Card(K).

#### Ví dụ {#alg-viii-s3-n2-exa-1 .statement tag=003G}

$*$ Cho A là một đại số $\mathbf{C}$ được sinh bởi một họ đếm được các phần tử; nó có chiều đếm được trên $\mathbf{C}$. Cho M là một A-môđun đơn; nó là đơn sinh, nên có một cơ sở đếm được trên $\mathbf{C}$. Vì trường $\mathbf{C}$ không đếm được (Gen. Top., IV, §4, No. 1, p. 44), ta có $[M :\mathbf{C}]<$ Card($\mathbf{C}$). Do đó các tự đồng cấu của A-môđun M là các phép tỉ lệ $\alpha_M$ với $\alpha \in \mathbf{C}$. Điều này áp dụng, cụ thể, khi A là đại số bao trùm phổ quát của một đại số Lie hữu hạn chiều trên $\mathbf{C}($Lie, I, §2, No. 7, p. 21, Hệ quả $3).*$

#### Hệ quả 1 {#alg-viii-s3-lem-1-cor-1 .statement tag=003H}

Giữ các giả thiết của Định lý 1, và giả sử, hơn nữa, rằng đại số A là giao hoán. Khi đó M có chiều 1 trên K.

Vì vành A là giao hoán, $a_M$ là một tự đồng cấu của A-môđun M với mọi $a\in A$. Theo Định lý 1, ta có $A_M= K\cdot 1_M$, và M là một K-môđun đơn, tức là một không gian vectơ 1 chiều trên trường K.

#### Hệ quả 2 {#alg-viii-s3-lem-1-cor-2 .statement tag=003I}

Cho K là một trường giao hoán, A là một đại số trên K, và M là một A-môđun. Giả sử rằng với mỗi mở rộng L của K, $A_{(L)}$-môđun $M_{(L)}$ là đơn. Khi đó, vòng tròi tự đồng cấu của M bao gồm các đẳng tỷ $\alpha_M$ với $\alpha \in K$.

Cho I là một tập hợp có lực lượng lớn hơn nghiêm ngặt chiều của M trên K (ví dụ, tập hợp các tập con của M). Cho L là một bao đóng đại số của trường $K((X_i)_{i\in I})$ (V, §4, No. 3, p. 23, Định lý 2). Chọn một dạng K-tuyến tính $\varphi$ trên L sao cho $\varphi (1) = 1$, và cho $v: M_{(L)}\rightarrow M$ là ánh xạ K-tuyến tính được đặc trưng bởi $v(\alpha \otimes m) =\varphi (\alpha )m$. Cho $u$ là một tự đồng cấu của M. Chiều của $M_{(L)}$ trên L bằng chiều của M trên K và nhỏ hơn nghiêm ngặt lực lượng của L. Theo Định lý 1, tự đồng cấu $1_L\otimes u$ của $A_{(L)}$-môđun $M_{(L)}$ có dạng $\lambda \otimes 1_M$ với $\lambda \in L$. Với mọi $x\in M$, ta có

$$
u(x) =v(1\otimes u(x))=v((1_L\otimes u)(1\otimes x))
$$

$$
=v((\lambda \otimes 1_M)(1\otimes x))=v(\lambda \otimes x) =\varphi (\lambda )x
$$

sao cho $u$ là phép vị tự $\varphi (\lambda )_M$.

### 3. Môđun con cực đại

#### Định nghĩa 2 {#alg-viii-s3-def-2 .statement tag=003J}

Cho A là một vành và M là một A-môđun. Một môđun con cực đại của M là một phần tử cực đại, theo quan hệ chứa, của tập hợp các môđun con thực sự của M.

Một môđun con cực đại của $A_s$ đơn giản là một iđêan cực đại trái của A.

Cho N là một môđun con của M. Các môđun con của $M/N$ có dạng $P/N$, trong đó P là một môđun con của M chứa N (I, §4, No. 6, p. 41, Định lý 4). Do đó, N là một môđun con cực đại của M nếu và chỉ nếu môđun $M/N$ là đơn.

#### Mệnh đề 3 {#alg-viii-s3-prop-3 .statement tag=003K}

Cho M là một A-môđun hữu hạn sinh. Mọi môđun con thực sự của M đều được chứa trong một môđun con cực đại.

Cho N là một môđun con thực sự của M. Gọi $\mathscr{S}$ là tập hợp các môđun con thực sự của M chứa N, được sắp thứ tự bởi sự bao hàm; chúng ta chứng minh rằng $\mathscr{S}$ là quy nạp. Cho $\mathscr{F}$ là một tập con được sắp thứ tự toàn phần của $\mathscr{S}$. Nếu $\mathscr{F}$ rỗng, thì N là một cận trên cho $\mathscr{F}$ trong $\mathscr{S}$. Trong trường hợp đối, gọi Q là hợp của các phần tử của $\mathscr{F}$. Khi đó Q là một môđun con của M. Cho F là một tập con sinh hữu hạn của M. Nếu Q bằng M, thì F sẽ được chứa trong một môđun con $P\in \mathscr{F}$, điều đó ngụ ý P = M, trái với định nghĩa của $\mathscr{F}$. Do đó ta có $Q\in \mathscr{S}$, điều này chứng minh rằng $\mathscr{S}$ là quy nạp. Khi đó Mệnh đề 3 suy ra từ Hệ quả 1 của Lý thuyết Tập hợp, III, §2, No. 4, p. 155.

#### Hệ quả 1 {#alg-viii-s3-prop-3-cor-1 .statement tag=003L}

Cho M là một A-môđun hữu hạn sinh khác không. Tồn tại một iđêan hai phía $\mathfrak{a}$ của A, linh hóa tử của một A-môđun đơn, sao cho $\mathfrak{a}M$ không bằng M.

Cho N là một môđun con cực đại của M (Mệnh đề 3), và cho $\mathfrak{a}$ là linh hóa tử của A-môđun đơn $M/N$; nó là một iđêan hai phía của A, và ta có $\mathfrak{a}(M/N) = 0$, do đó $\mathfrak{a}M\subset N$ và do đó $\mathfrak{a}M\not= M$.

#### Hệ quả 2 {#alg-viii-s3-prop-3-cor-2 .statement tag=003M}

Cho A là một vành giao hoán và B là một đại số trên A. Cho M là một B-môđun đơn là một A-môđun hữu hạn sinh, và cho $\mathfrak{m}$ là linh hóa tử của A-môđun M. Khi đó $\mathfrak{m}$ là một iđêan cực đại của A, và M là một không gian vectơ hữu hạn chiều trên trường $A/\mathfrak{m}$.

Vì vành A là giao hoán, linh hóa tử của một A-môđun đơn là một iđêan cực đại của A (VIII, p. 46, Mệnh đề 1). Theo Hệ quả 1 áp dụng cho A-môđun M, tồn tại một iđêan cực đại $\mathfrak{a}$ của A sao cho $\mathfrak{a}M\not= M$. Nhưng $\mathfrak{a}M$ là một môđun con của B-môđun đơn M; do đó ta có $\mathfrak{a}M = 0$ và $\mathfrak{a}\subset \mathfrak{m}$. Vì iđêan $\mathfrak{m}$ phân biệt với A, nó bằng $\mathfrak{a}$, do đó $\mathfrak{m}$ là cực đại. Môđun M là một môđun hữu hạn sinh trên trường $A/\mathfrak{m}$; khẳng định cuối cùng suy ra.

### 4. Môđun đơn trên một vành Artin

Cho A là một vành. Theo cách nói lạm dụng, ta nói rằng một iđêan trái $\mathfrak{a}$ là một iđêan trái tối tiểu của A nếu nó là một phần tử tối tiểu của tập hợp các iđêan trái khác không của A, được sắp theo thứ tự bằng sự chứa. Ta định nghĩa iđêan tối tiểu phải và iđêan tối tiểu hai phía tương tự.

Cho $\mathfrak{a}$ là một iđêan trái của A. Khi đó $\mathfrak{a}$ là một A-môđun đơn nếu và chỉ nếu nó là một iđêan trái tối tiểu của A.

Mọi iđêan trái khác không của một vành Artin trái (VIII, p. 1, Định nghĩa 1) đều chứa một iđêan trái tối tiểu.

#### Mệnh đề 4 {#alg-viii-s3-prop-4 .statement tag=003N}

Cho A là một vành có một iđêan trái tối tiểu $\mathfrak{a}$. Mọi A-môđun đơn trung thành đều đẳng cấu với A-môđun $\mathfrak{a}$.

Cho M là một A-môđun đơn trung thành. Cho $\alpha$ là một phần tử khác không của $\mathfrak{a}$. Vì A-môđun M là trung thành, nên tồn tại một phần tử $x$ của M sao cho $\alpha x\not= 0$. Đồng cấu $a\mapsto ax$ từ $\mathfrak{a}$ đến M khi đó khác không; do đó nó là một đẳng cấu theo Mệnh đề 2 của VIII, p. 47.

#### Mệnh đề 5 {#alg-viii-s3-prop-5 .statement tag=003O}

Cho A là một vành Artin trái và M là một A-môđun trung thành.

a) Tồn tại một số tự nhiên $m$ và một đẳng cấu từ $A_s$ đến một môđun con của $M^m$.

b) Nếu M có một chuỗi Jordan–Hölder $(M_i)_{0\leqslant i\leqslant n}$, thì mọi A-môđun đơn đều đẳng cấu với một trong các thương $M_i/M_{i+1}$.

Theo VIII, p. 2 áp dụng cho A-môđun $A_s$ và các linh hóa tử của các phần tử của M, tồn tại các phần tử $x_1, . . . , x_m$ của M sao cho linh hóa tử của M là giao của các linh hóa tử của các $x_i$. Vì A-môđun M là trung thành, ánh xạ A-tuyến tính $a\mapsto (ax_1, . . . , ax_m)$ từ $A_s$ đến $M^m$ là đơn ánh, do đó a).

Dưới giả thiết của b), mọi thương đơn của $A_s$ đều đẳng cấu với một thương của một chuỗi Jordan–Hölder của $M^m$ (I, §4, No. 7, p. 43, Hệ quả), do đó đẳng cấu với một trong các môđun $M_i/M_{i+1}$ (I, §4, No. 7, p. 43, Định lý 6). Chúng ta kết luận rằng mọi A-môđun đơn đều đẳng cấu với một thương của $A_s$.

#### Nhận xét {#alg-viii-s3-n4-rem-1 .statement tag=003P}

Mệnh đề 5 áp dụng, nói riêng, cho hai trường hợp sau:

a) Cho A là một đại số trên một trường giao hoán K, và cho M là một môđun trung thành hữu hạn chiều trên K. Khi đó M là một A-môđun có độ dài hữu hạn, và môđun đối của M là sinh hữu hạn. Vành A là Artin trái (VIII, p. 9, Mệnh đề 6). Tồn tại một chuỗi Jordan–Hölder $(M_i)_{0\leqslant i\leqslant n}$ của A-môđun M, và mọi A-môđun đơn đều đẳng cấu với một trong các môđun $M_i/M_{i+1}$ với $0\leqslant i\leqslant n-1$.

b) Cho A là một vành Artin trái. Môđun $A_s$ có độ dài hữu hạn (VIII, p. 6, Định lý 1). Vì A-môđun $A_s$ có độ dài hữu hạn, tồn tại một dãy giảm $(\mathfrak{a}_i)_{0\leqslant i\leqslant n}$ các iđêan trái của A sao cho $\mathfrak{a}_0= A$ và $\mathfrak{a}_n= 0$ và các A-môđun $S_i=\mathfrak{a}_{i-1}/\mathfrak{a}_i$ là đơn với $1\leqslant i\leqslant n$. Khi đó mọi A-môđun đơn đều đẳng cấu với một trong các môđun $S_1, . . . ,S_n$.

### 5. Các lớp môđun đơn

Ký hiệu Is$_A(X,Y)$ là quan hệ

“A là một vành và $X,Y$ là các A-môđun đẳng cấu.”

Đây là một quan hệ tương đương đối với X và Y. Nếu X là một A-môđun, ta ký hiệu lớp các đối tượng tương đương với X đối với Is$_A$ bởi cl(X) và gọi đó là lớp của A-môđun X (Lý thuyết tập hợp, II, §6, No. 9, p. 122). Theo định nghĩa, cl(X) là một A-môđun đẳng cấu với X; hơn nữa, hai A-môđun X và Y đẳng cấu khi và chỉ khi ta có cl(X) = cl(Y).

Cho A là một vành. Quan hệ

“$\lambda$ là một lớp các A-môđun sinh hữu hạn”

xác định tập trong $\lambda ($Lý thuyết tập hợp, II, §1, No. 4, p. 68). Thật vậy, mọi A-môđun sinh hữu hạn đều đẳng cấu với một A-môđun có dạng $A^n_s/R$, trong đó $n$ là một số tự nhiên và R là một môđun con của $A^n_s$, do đó mệnh đề của chúng ta suy ra từ Lý thuyết tập hợp, II, §6, No. 9, p. 122.

Ta ký hiệu tập hợp các lớp của các A-môđun sinh hữu hạn bởi $\mathscr{F}(A)$. Mọi A-môđun đơn đều đơn sinh (VIII, p. 46, Mệnh đề 1), và do đó các lớp của các A-môđun đơn tạo thành một tập con của $\mathscr{F}$ (A), mà từ nay về sau ta ký hiệu là $\mathscr{S}(A)$ (hay đơn giản là $\mathscr{S})$. Khi vành A giao hoán, ánh xạ $\mathfrak{m}\mapsto$ cl(A$/\mathfrak{m})$ là một song ánh từ tập hợp các iđêan cực đại của A vào tập hợp $\mathscr{S}(A)$ (loc. cit. và VIII, p. 46, Nhận xét 1). Khi A là Artin trái, tập hợp $\mathscr{S}(A)$ là hữu hạn (VIII, p. 51, Nhận xét b)).

### Bài tập {#alg-viii-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).
