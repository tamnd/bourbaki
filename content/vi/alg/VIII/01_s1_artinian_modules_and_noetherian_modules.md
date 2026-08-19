---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 1
section_title: Artinian Modules and Noetherian Modules
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.1-A VIII.23
pdf_pages: 0018-0040
extraction: native
subsections:
    - "no": 1
      title: Artinian Modules and Noetherian Modules
      page: 1
      pdf_page: 18
    - "no": 2
      title: Artinian Rings and Noetherian Rings
      page: 4
      pdf_page: 21
    - "no": 3
      title: Countermodule
      page: 8
      pdf_page: 25
    - "no": 4
      title: Polynomials with Coefficients in a Noetherian Ring
      page: 9
      pdf_page: 26
statements: 36
exercises: 28
content_sha256: 462ba13b60b1c7f227a5d1eb06c04cfc95102bc0fe3f654f53c9da5770112831
translated_from: content/en/alg/VIII/01_s1_artinian_modules_and_noetherian_modules.md
source_content_sha256: d64719b4a6721ac9031c6bccd67b196cb6dafe3fc596f4fdebd425f00893c469
translation_model: hy3-free, gpt-5-6, nemotron-3-ultra-free, laguna-s-2.1-free, gpt-5-6-mini
translation_run: translate-vi-033a62f7
glossary_version: 30
glossary_terms_sha256: 0d3e36173b74a7028533a2401a9a858e4f434a5b11e12d76c45aeb4d098320c6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. Môđun Artin và môđun Noether

### 1. Môđun Artin và môđun Noether

#### Định nghĩa 1 {#alg-viii-s1-def-1 .statement tag=0001}

Cho A là một vành. Chúng ta gọi một A-môđun M là Artin (resp. Noether) nếu nó thỏa mãn các điều kiện tương đương sau:

(i) Mọi tập hợp khác rỗng các môđun con của M, được sắp thứ tự bởi sự bao hàm, có một phần tử cực tiểu (resp. cực đại).

(ii) Mọi dãy giảm (resp. tăng) các môđun con của M đều dừng.

Sự tương đương của các điều kiện (i) và (ii) suy ra từ Lý thuyết Tập hợp, III, §6, No. 5, p. 190, Mệnh đề 6.

Một A-môđun M là Artin (resp. Noether) khi và chỉ khi M, được xem như một môđun trên vành các phép đồng dạng $A_M$, là Artin (resp. Noether).

Cho M là một A-môđun Artin (resp. Noether). Mọi tập hợp khác rỗng các môđun con của M, được sắp thứ tự bởi sự bao hàm, mà có hướng trái (resp. có hướng phải) thì có một phần tử nhỏ nhất (resp. một phần tử lớn nhất) (Lý thuyết Tập hợp, III, §1, No. 10, p. 145, Mệnh đề 10).

Cho M là một A-môđun Artin (resp. Noether) và $(M_i)_{i\in I}$ một họ các môđun con của M. Các giao (resp. tổng) của các họ con hữu hạn của họ $(M_i)_{i\in I}$ tạo thành một tập hợp khác rỗng có hướng trái (resp. phải) các môđun con của M. Do đó, tồn tại một tập con hữu hạn J của I sao cho $\bigcap_{i\in I}M_i=\bigcap_{i\in J}M_i$ (resp. $\sum_{i\in I}M_i=\sum_{i\in J}M_i$)).

#### Ví dụ 1 {#alg-viii-s1-n1-exa-1 .statement tag=0002}

Một không gian vectơ hữu hạn chiều trên một trường là Artin và Noether.

#### Ví dụ 2 {#alg-viii-s1-n1-exa-2 .statement tag=0003}

Cho M là một A-môđun. Nếu tồn tại một họ vô hạn $(M_i)_{i\in I}$ các môđun con khác không của M mà tổng của chúng là trực tiếp, thì M không là Artin cũng không là Noether: thực vậy, với mọi dãy vô hạn giảm nghiêm ngặt (resp. tăng ngặt) $(J_n)$ các tập con của I, dãy vô hạn $(\sum_{i\in J_n}M_i)$ các môđun con của M là giảm nghiêm ngặt (resp. tăng ngặt). Đặc biệt, một không gian vectơ vô hạn chiều trên một trường không là Artin cũng không là Noether.

#### Ví dụ 3 {#alg-viii-s1-n1-exa-3 .statement tag=0004}

Chúng ta sẽ thấy ở phần sau rằng $\mathbf{Z}$-môđun $\mathbf{Z}$ là Noether nhưng không phải là

Artin (VIII, p. 5, Ví dụ 3)$.*$

#### Ví dụ 4 {#alg-viii-s1-n1-exa-4 .statement tag=0005}

Cho $p$ là một số nguyên tố và $M_p$ là thành phần nguyên sơ $p$ của môđun xoắn $\mathbf{Z}$-môđun $\mathbf{Q}/\mathbf{Z}$ (VII, §2, No. 2, p. 7). Mọi môđun con của $M_p$ bằng hoặc là $M_p$ hoặc là $p^{-n}\mathbf{Z}/\mathbf{Z}$ với một số nguyên $n\in \mathbf{N}$ (VII, §2, p. 54, Bài tập 3). Do đó, $M_p$ là Artin nhưng không phải Noether $\mathbf{Z}$-môđun.

#### Mệnh đề 1 {#alg-viii-s1-prop-1 .statement tag=0006}

Một A-môđun M có độ dài hữu hạn (II, §1, No. 10, p. 212) khi và chỉ khi nó vừa là Artin vừa là Noether.

Giả sử rằng M có độ dài hữu hạn $d$. Khi đó mọi dãy tăng ngặt hoặc giảm nghiêm ngặt của các môđun con của M có nhiều nhất $d+ 1$ số hạng (I, §4, No. 7, p. 44). Do đó, M là Artin và Noether.

Ngược lại, giả sử M là Artin và Noether. Cho $\mathscr{S}$ là tập hợp các môđun con của M có độ dài hữu hạn. Môđun con không là một phần tử của $\mathscr{S}$, và vì M là Noether, $\mathscr{S}$ có một phần tử cực đại N. Hãy cho một chứng minh bằng phản chứng và giả sử rằng $M\not= N$. Tập hợp các môđun con của M phân biệt với N và chứa N khi đó có một phần tử cực tiểu P vì M là Artin. Môđun $P/N$ có độ dài 1, và vì N là một môđun có độ dài hữu hạn, điều tương tự cũng đúng cho P (II, §1, No. 10, p. 212, Mệnh đề 16). Điều này mâu thuẫn với định nghĩa của N.

#### Mệnh đề 2 {#alg-viii-s1-prop-2 .statement tag=0007}

Một A-môđun M là Noether nếu và chỉ nếu mọi môđun con của M đều sinh hữu hạn.

Bắt đầu bằng cách giả sử mọi môđun con của M đều sinh hữu hạn. Cho $(P_n)_{n\in\mathbf{N}}$ là một dãy tăng của các môđun con của M, và cho P là hợp của chúng. Đây là một môđun con của M. Theo giả thiết, tồn tại một tập con hữu hạn F của M sinh môđun P; cho $n\in \mathbf{N}$ là một số nguyên sao cho $F\subset P_n$. Khi đó ta có $P_n= P$, và dãy $(P_n)_{n\in\mathbf{N}}$ là dừng. Điều này chứng minh rằng môđun M là Noether.

Đảo lại là một hệ quả của mệnh đề chính xác hơn sau đây.

#### Bổ đề 1 {#alg-viii-s1-lem-1 .statement tag=0008}

Cho M là một A-môđun Noether và E một tập con của M. Tồn tại một tập con hữu hạn F của E sinh cùng một môđun con như E.

Thật vậy, theo VIII, p. 2, tồn tại một tập con hữu hạn F của E sao cho $\sum_{x\in E}Ax=\sum_{x\in F}Ax$.

#### Mệnh đề 3 {#alg-viii-s1-prop-3 .statement tag=0009}

Cho M là một A-môđun và N một môđun con của M. Khi đó M là Artin (tương ứng Noether) nếu và chỉ nếu N và $M/N$ là như vậy.

Ta sẽ đưa ra chứng minh trong trường hợp các môđun Artin; trường hợp các môđun Noether là tương tự.

Giả sử M là Artin. Vì mỗi môđun con của N là môđun con của M, do đó môđun N là Artin. Đặt $(P_n)_{n\in\mathbf{N}}$ là một dãy giảm các môđun con của $M/N$. Tồn tại một dãy giảm $(Q_n)_{n\in\mathbf{N}}$ của các môđun con của M chứa N sao cho $P_n= Q_n/N$ với mỗi $n\in \mathbf{N}$ (I, §4, No. 6, p. 41, Định lý 4). Vì M là Artin, dãy $(Q_n)$ dừng, do đó dãy $(P_n)$ cũng dừng. Do đó, môđun $M/N$ là Artin.

Ngược lại, giả sử các môđun N và $M/N$ là Artin, và xét một dãy giảm $(P_n)$ của các môđun con của M. Dãy $P'_n= N\cap P_n$ của các môđun con của N là dừng. Tương tự, dãy $P''_n= (N + P_n)/N$ của các môđun con của $M/N$ là dừng. Do đó, tồn tại một số nguyên $m\in \mathbf{N}$ sao cho ta có $P'_n= P'_m$ và $P''_n= P''_m$ với mọi số nguyên $n\geqslant m$. Khi đó dãy $(P_n)$ là dừng nhờ bổ đề sau.

#### Bổ đề 2 {#alg-viii-s1-lem-2 .statement tag=00QV}

Cho M là một A-môđun và N, P, Q là các môđun con của M. Giả sử ta có $P\subset Q$, $N\cap P = N\cap Q$, và N + P = N + Q. Khi đó ta có P = Q.

Cho $x$ là một phần tử của Q. Nó thuộc N + P; do đó, tồn tại một phần tử $y$ của P sao cho $x-y\in N$. Vì Q chứa P, hiệu $x-y$ thuộc $N\cap Q$ và do đó thuộc P. Do đó, $x$ thuộc P.

#### Hệ quả {#alg-viii-s1-n1-cor-1 .statement tag=000A}

Cho M là một A-môđun và $(M_i)_{i\in I}$ là một họ hữu hạn các môđun con của M.

a) Nếu các môđun $M_i$ là Artin (resp. Noether), thì tổng $\sum_{i\in I}M_i$ của chúng cũng là Artin (resp. Noether).

b) Nếu các môđun $M/M_i$ là Artin (resp. Noether), thì môđun $M/\bigcap_{i\in I}M_i$ cũng là Artin (resp. Noether).

Bằng quy nạp, đủ để xét trường hợp khi $I =\{1,2\}$. Môđun $M_2/(M_1\cap M_2)$, thương của $M_2$, đẳng cấu với môđun con $(M_1+M_2)/M_1$ của $M/M_1$ (I, §4, No. 6, p. 41, Định lý 4).

Trong phần a), chúng ta giả sử $M_1$ và $(M_1+ M_2)/M_1$ là Artin (tương ứng Noether); khi đó điều tương tự cũng đúng cho $M_1+ M_2$ (Mệnh đề 3).

Trong phần b), chúng ta giả sử $M/M_2$ và $M_2/(M_1\cap M_2)$ là Artin (tương ứng Noether); khi đó điều tương tự cũng đúng cho $M/(M_1\cap M_2)$ (nơi trên).

#### Ví dụ 5 {#alg-viii-s1-n1-exa-5 .statement tag=000B}

Cho $(M_i)_{i\in I}$ là một họ hữu hạn của các A-môđun. Nếu các môđun $M_i$ là Artin (tương ứng Noether), thì tổng trực tiếp $\bigoplus_{i\in I}M_i$ cũng vậy.

#### Nhận xét {#alg-viii-s1-n1-rem-1 .statement tag=000C}

Các định nghĩa và kết quả của tiể mục này mở rộng sang các nhóm Abel tùy ý với các phép toán bằng cách thay thế các môđun con trong các mệnh đề bằng các nhóm phụ ổn định.

### 2. Vành Artin và Vành Noether

#### Định nghĩa 2 {#alg-viii-s1-def-2 .statement tag=000D}

Một vành A được gọi là Artin trái (resp. Noether trái) nếu A-môđun trái $A_s$ là Artin (resp. Noether). Tương tự, một vành A được gọi là Artin phải (resp. Noether phải) nếu A-môđun phải $A_d$ là Artin (resp. Noether).

Một vành A là Artin phải (resp. Noether phải) khi và chỉ khi vành đối $A^o$ của nó là Artin trái (resp. Noether trái). Với một vành giao hoán A, các tính chất là Artin trái và là Artin phải trùng nhau, và khi chúng đúng, ta nói rằng vành A là Artin; ta áp dụng một quy ước tương tự cho “Noether”. Tồn tại các vành không giao hoán là Artin trái nhưng không phải Artin phải, và các vành không giao hoán là Noether trái nhưng không phải Noether phải (VIII, p. 14, Bài tập 3).

Cho A là một vành. Theo định nghĩa, các tính chất sau là tương đương:

(i) Vành A là Artin trái.

(ii) Mọi tập hợp khác rỗng các iđêan trái của A, có thứ tự bởi bao hàm, đều có một phần tử cực tiểu.

(iii) Mọi dãy giảm các iđêan trái của A là dừng.

Do Mệnh đề 2 của VIII, p. 3, các tính chất sau là tương đương:

(i) Vành A là Noether trái.

(ii) Mọi tập hợp khác rỗng các iđêan trái của A, có thứ tự bởi bao hàm, đều có một phần tử cực đại.

(iii) Mọi dãy tăng các iđêan trái của A là dừng.

(iv) Mọi iđêan trái của A được sinh bởi một tập con hữu hạn của A.

#### Ví dụ 1 {#alg-viii-s1-n2-exa-1 .statement tag=000E}

Một trường là một vành vừa là Artin trái và phải, vừa là Noether.

#### Ví dụ 2 {#alg-viii-s1-n2-exa-2 .statement tag=000F}

Cho A là một vành và D là một vành con của A. Giả sử rằng D là một trường và A là một không gian vectơ trái hữu hạn chiều trên D. Khi đó vành A là Artin trái và Noether trái bởi vì mọi iđêan trái của A đều là một không gian con vectơ D của A. Đặc biệt, một đại số hữu hạn chiều trên một trường giao hoán là một vành vừa là Artin trái và phải, vừa là Noether.

#### Ví dụ 3 {#alg-viii-s1-n2-exa-3 .statement tag=000G}

Một miền iđêan chính (VII, §1, No. 1, p. 1, Định nghĩa 1) là Noether. Một miền nguyên A không là trường thì không phải là một vành Artin: với mọi phần tử khác không không khả nghịch $a$ của A, dãy các iđêan $a^nA$ (for $n\in \mathbf{N}$) là giảm nghiêm ngặt. Cụ thể, vành $\mathbf{Z}$ các số nguyên là Noether nhưng không phải Artin.

#### Ví dụ 4 {#alg-viii-s1-n2-exa-4 .statement tag=000H}

Cho M là một A-môđun là tổng trực tiếp của một họ vô hạn $(M_i)_{i\in I}$ các môđun con khác không. Cho E là vành tự đồng cấu của M. Với mọi $i\in I$, đặt $\mathfrak{a}_i$ (resp. $\mathfrak{b}_i$) là tập hợp các phần tử của E có hạt nhân chứa $\sum_{j\not=i}M_j$ (resp. có ảnh được chứa trong $M_i$). Khi đó $(\mathfrak{a}_i)$ là một họ vô hạn các iđêan trái khác không của E có tổng trực tiếp, và $(\mathfrak{b}_i)$ là một họ vô hạn các iđêan phải khác không của E có tổng trực tiếp. Do đó, vành E không là Artin trái cũng như không là Artin phải (resp. Noether) (VIII, p. 2, Ví dụ 2). Cụ thể, vành tự đồng cấu của một không gian vectơ vô hạn chiều không là Artin trái cũng như không là Artin phải (resp. Noether).

#### Định lý 1 {#alg-viii-s1-thm-1 .statement tag=00QW}

Cho A là một vành Artin trái. A-môđun $A_s$ có độ dài hữu hạn.

Ta sẽ dùng bổ đề sau trong chứng minh.

#### Bổ đề 3 {#alg-viii-s1-lem-3 .statement tag=000I}

Cho A là một vành và $n$ là một số tự nhiên. Một A-môđun Artin M là tổng của một họ các môđun con có độ dài $\leqslant n$ thì có độ dài hữu hạn.

Ta dùng quy nạp trên $n$. Đầu tiên, giả sử $n= 1$. Nếu M không có độ dài hữu hạn, thì ta có thể xây dựng một dãy $(M_m)_{m\in\mathbf{N}}$ các môđun con của M có độ dài 1 với $M_m\not\subset (\sum_{i<m}M_i)$ với mọi $m\in \mathbf{N}$. Khi đó ta sẽ có $M_m\cap \sum_{i<m}M_i= 0$ với mọi $m$, và tổng của họ $(M_m)_{m\in\mathbf{N}}$ sẽ là trực tiếp. Tuy nhiên, điều này mâu thuẫn với việc A-môđun M là Artin (VIII, p. 2, Ví dụ 2).

Giả sử $n\geqslant 2$. Cho $(M_i)_{i\in I}$ là một họ các môđun con của M có độ dài $\leqslant n$ và tổng là M. Với mỗi $i\in I$, chọn một môđun con $M'_i$ của $M_i$ có độ dài $\leqslant n-1$ sao cho $M_i/M'_i$ có độ dài $\leqslant 1$. Đặt $M'=\sum M'_i$, và ký hiệu ảnh của $M_i$ trong $M''= M/M'$ bằng $M''_i$. Các môđun $M''_i$ có độ dài $\leqslant 1$, và tổng của chúng là $M''$. Các môđun $M'$ và $M''$ là Artin (VIII, p. 3, Mệnh đề 3); theo giả thiết quy nạp, chúng có độ dài hữu hạn. Do đó, M có độ dài hữu hạn (II, §1, No. 10, p. 212, Mệnh đề 16).

Bây giờ chứng minh Định lý 1. Cho $\mathscr{S}$ biểu thị tập hợp các lý tưởng trái $\mathfrak{a}$ của A sao cho môđun $A_s/\mathfrak{a}$ có độ dài hữu hạn. Cho $(\mathfrak{a}_i)_{i\in I}$ là một họ hữu hạn các phần tử của $\mathscr{S}$. Theo Mệnh đề 1 của VIII, p. 2, A-môđun $A_s/\mathfrak{a}_i$ là Artin và Noether với mọi $i\in I$. Do đó, $A_s/\bigcap_{i\in I}\mathfrak{a}_i$ là Artin và Noether (VIII, p. 4, Hệ quả của Mệnh đề 3), do đó có độ dài hữu hạn (VIII, p. 2, Mệnh đề 1). Điều này chứng minh $\mathscr{S}$ là một tập có hướng trái theo sự bao hàm. Vì vành A là Artin trái, tập $\mathscr{S}$ có một phần tử nhỏ nhất $\mathfrak{b}$. Ta ký hiệu độ dài của A-môđun $A_s/\mathfrak{b}$ bằng $n$.

Cho $x$ là một phần tử của $A_s$ và $\mathfrak{a}$ là linh hóa tử của nó (II, §1, No. 12, p. 219). A-môđun $Ax$ đẳng cấu với $A_s/\mathfrak{a}$. Nếu $Ax$ có độ dài hữu hạn, thì $\mathfrak{a}$ thuộc $\mathscr{S}$, do đó $\mathfrak{a}$ chứa $\mathfrak{b}$ và $Ax$ có độ dài $\leqslant n$. Vậy, mọi iđêan trái đơn sinh của A có độ dài hữu hạn đều có độ dài $\leqslant n$. Gọi $\mathfrak{c}$ là tổng của các iđêan này; đây là một iđêan trái của A, có độ dài hữu hạn theo Bổ đề 3. Mọi iđêan trái của A có độ dài hữu hạn là một tổng của các iđêan trái đơn sinh có độ dài hữu hạn và vì thế được chứa trong $\mathfrak{c}$. Do đó, $\mathfrak{c}$ là iđêan trái lớn nhất của A có độ dài hữu hạn.

Nếu $\mathfrak{c}$ phân biệt với A, thì tập hợp các lý tưởng trái của A chứa $\mathfrak{c}$ và phân biệt với $\mathfrak{c}$ sẽ có một phần tử cực tiểu $\mathfrak{c}'$. A-môđun $\mathfrak{c}'/\mathfrak{c}$ khi đó sẽ có độ dài 1, và $\mathfrak{c}'$ sẽ có độ dài hữu hạn, điều này mâu thuẫn với việc $\mathfrak{c}$ là cực đại. Do đó ta có $\mathfrak{c}= A$; A-môđun $A_s$ có độ dài hữu hạn.

#### Hệ quả {#alg-viii-s1-n2-cor-1 .statement tag=000J}

Mọi vành Artin trái đều là Noether trái.

Cho A là một vành Artin trái. Theo Định lý 1, A-môđun $A_s$ có độ dài hữu hạn. Sau đó ta áp dụng Mệnh đề 1 của VIII, p. 2.

Cho A là một vành Artin trái (resp. phải). Độ dài của A-môđun $A_s$ (resp. $A_d$) (I, §4, No. 7, p. 44) được gọi là độ dài trái (resp. phải) của vành A. Khi A là một vành Artin giao hoán, hai độ dài này trùng nhau và được gọi đơn giản là độ dài của A. Khi A là Artin trái và phải nhưng không giao hoán, các độ dài trái và phải của A không tất yếu bằng nhau (VIII, p. 14, Bài tập 3).

#### Ví dụ 5 {#alg-viii-s1-n2-exa-5 .statement tag=000K}

Các độ dài trái và phải của một trường bằng 1.

#### Mệnh đề 4 {#alg-viii-s1-prop-4 .statement tag=000L}

a) Cho A là một vành Noether trái và M là một A-môđun trái sinh hữu hạn. Môđun M là Noether, và mọi môđun con của M đều sinh hữu hạn.

b) Cho A là một vành Artin trái và M là một A-môđun trái. Các tính chất sau là tương đương: môđun M sinh hữu hạn; môđun M là Artin; môđun M có độ dài hữu hạn; môđun M là Noether.

Chúng ta chứng minh a). Mọi môđun con đơn sinh của M đều đẳng cấu với một thương của $A_s$, do đó là Noether theo Mệnh đề 3 của VIII, p. 3. Môđun M là một tổng hữu hạn của các môđun con như vậy; do đó nó là Noether theo hệ quả (VIII, p. 4) của Mệnh đề 3. Khi đó mọi môđun con của M đều sinh hữu hạn (VIII, p. 3, Mệnh đề 2)

Bây giờ, giả sử rằng vành A là Artin trái. Ta thấy, như trong tiết diện trước, rằng nếu A-môđun M sinh hữu hạn, thì nó là Artin. Nếu nó là Artin, thì nó có độ dài hữu hạn: thật vậy, các môđun con đơn sinh của nó đẳng cấu với các thương của $A_s$ và do đó có độ dài hữu hạn nhỏ hơn độ dài của $A_s$, và mệnh đề suy ra từ Bổ đề 3. Mọi môđun có độ dài hữu hạn đều là Noether, và mọi môđun Noether đều sinh hữu hạn. Điều này chứng minh b).

#### Mệnh đề 5 {#alg-viii-s1-prop-5 .statement tag=000M}

a) Cho A là một vành Artin trái (tương ứng Noether trái), và cho $\varphi : A\rightarrow B$ là một đồng cấu vành biến B thành một A-môđun trái sinh hữu hạn. Vành B là Artin trái (tương ứng Noether trái).

b) Cho A là một vành Artin trái (tương ứng Noether trái), và cho $\mathfrak{a}$ là một iđêan hai phía của A; vành $A/\mathfrak{a}$ là Artin trái (tương ứng Noether trái).

c) Cho $(A_i)_{i\in I}$ là một họ các vành Artin trái (tương ứng Noether trái). Vành $\prod_{i\in I}A_i$ là Artin trái (tương ứng Noether trái).

Chúng ta sẽ xét trường hợp các vành Artin; trường hợp các vành Noether là tương tự.

Chúng ta chứng minh a). Theo Mệnh đề 4, vành $B_s$ là một A-môđun trái Artin và a fortiori là một B-môđun trái Artin.

Mệnh đề b) suy ra từ mệnh đề a) áp dụng cho đồng cấu chính tắc từ A đến $A/\mathfrak{a}$.

Chúng ta chứng minh c). Đặt $A =\prod_{i\in I}A_i$. Theo giả thiết, $(A_i)_s$ là một $A_i$-môđun trái Artin và a fortiori là một A-môđun trái Artin. Theo Ví dụ 5 của VIII, p. 4, A-môđun $A_s$ là Artin.

#### Hệ quả {#alg-viii-s1-n2-cor-2 .statement tag=000N}

Các iđêan nguyên tố của một vành giao hoán Artin là các iđêan cực đại của nó.

Trong bất kỳ vành giao hoán nào, một iđêan cực đại là nguyên tố. Cho A là một vành giao hoán Artin. Cho $\mathfrak{p}$ là một iđêan nguyên tố của A. Vành $A/\mathfrak{p}$ là một miền nguyên và là Artin (Mệnh đề 5), do đó là một trường (VIII, p. 5, Ví dụ 3). Do đó, iđêan $\mathfrak{p}$ là cực đại.

Vành đa thức $\mathbf{Q}[(X_n)_{n\in\mathbf{N}}]$ là một miền nguyên; nó không phải là Noether (hay Artin) (VIII, p. 15, Bài tập 9). Nó là một vành con của trường phân thức của nó, trường này là một vành Artin (và Noether).

### 3. Môđun đối

#### Định nghĩa 3 {#alg-viii-s1-def-3 .statement tag=000O}

Cho A là một vành, M là một A-môđun, và E = End$_A(M)$ là vành tự đồng cấu của M. Môđun đối của M là A-môđun trái E có cùng nhóm cộng cơ sở với M và phép toán ngoài $(c, x)\mapsto c(x)$.

Cho Z là tâm của vành A. Với mọi $a\in Z$, phép vị tự $a_M$ thuộc E. Do đó, E được trang bị một cách chính tắc cấu trúc của một Z-đại số. Đặc biệt, nếu M là một Z-môđun sinh hữu hạn, thì môđun đối của M là sinh hữu hạn.

#### Bổ đề 4 {#alg-viii-s1-lem-4 .statement tag=000P}

Cho M là một A-môđun trái có môđun đối sinh hữu hạn. Tồn tại một số tự nhiên $m$ và một ánh xạ tuyến tính $A_M$-đơn ánh từ $(A_M)_s$ vào $M^m$.

Đặt E = End$_A(M)$. Cho $(x_1, . . . , x_m)$ là một họ sinh hữu hạn của E-môđun M. Ánh xạ $\varphi :a\mapsto (ax_1, . . . , ax_m)$ từ $(A_M)_s$ vào $M^m$ là $A_M$-tuyến tính. Cho $a$ là một phần tử của $A_M$ sao cho $\varphi (a) = 0$. Tập hợp các phần tử $x$ của M sao cho $ax= 0$ là một môđun con E của M chứa $x_1, . . . , x_m$ và do đó bằng M, điều này suy ra $a= 0$.

#### Mệnh đề 6 {#alg-viii-s1-prop-6 .statement tag=000Q}

Cho M là một A-môđun trái Artin (tương ứng Noether) có môđun đối sinh hữu hạn. Vành các phép vị tự $A_M$ của M là Artin trái (tương ứng Noether trái).

Điều này suy ra từ Bổ đề 4 và Mệnh đề 3 của VIII, p. 3.

#### Hệ quả {#alg-viii-s1-n3-cor-1 .statement tag=000R}

Cho A là một vành giao hoán.

a) Cho M là một A-môđun Noether. Vành $A_M$ là Noether.

b) Cho M là một A-môđun có độ dài hữu hạn. Vành $A_M$ là Artin.

Cho M là một A-môđun. Dưới các giả thiết của a) hoặc b), A-môđun M là sinh hữu hạn. Vì A là giao hoán, $A_M$ được chứa trong vành End$_A$(M), do đó môđun đối của M là sinh hữu hạn. Khi đó chỉ cần áp dụng Mệnh đề 6.

#### Nhận xét {#alg-viii-s1-n3-rem-1 .statement tag=000S}

Cho A là một vành. Một A-môđun trái Artin M có môđun đối sinh hữu hạn có độ dài hữu hạn: thực vậy, vành đồng biến $A_M$ của M là Artin trái (Mệnh đề 6), và M là một môđun Artin trên $A_M$; theo VIII, p. 7, Mệnh đề 4, môđun M có độ dài hữu hạn trên $A_M$ và do đó cũng trên A.

Đặc biệt, mọi môđun Artin sinh hữu hạn trên một vành giao hoán đều có độ dài hữu hạn. Ngược lại, một môđun Artin sinh hữu hạn trên một vành không giao hoán không tất yếu có độ dài hữu hạn (VIII, p. 16, Bài tập 12).

### 4. Đa thức với hệ số trong vành Noether

Cho A là một vành, $\sigma$ là một tự đồng cấu của vành A, và $d$ là một tự đồng cấu của nhóm cộng của A thỏa mãn quan hệ

$$
d(ab) =\sigma (a)d(b) +d(a)b \tag{1}
$$

với mọi $a, b\in A$. Nói cách khác, $d$ là một đạo hàm từ vành A đến $(A$, A)-song môđun thu được bằng cách trang bị nhóm cộng của A với luật tác động trái $(a, x)\mapsto \sigma (a)x$ và luật tác động phải $(x, a)\mapsto xa$. Ta có $d(1) = 0$ (III, §10, No. 5, p. 557, Mệnh đề 3).

Nhớ lại (IV, §1, No. 1, p. 2) rằng A[X] biểu diễn cho $\mathbf{Z}$-môđun $A\otimes_{\mathbf{Z}}\mathbf{Z}[X]$ gồm các đa thức trong một biến số với hệ số thuộc A. Ta tạo cho nó cấu trúc tự nhiên của một A-môđun trái. Họ $(X^n)_{n\in\mathbf{N}}$ là một cơ sở của A[X] trên A. Ta đồng nhất A với ảnh của nó dưới ánh xạ $a\mapsto a\otimes 1$.

#### Mệnh đề 7 {#alg-viii-s1-prop-7 .statement tag=00QX}

Cho A$,\sigma ,d$ như trên. Tồn tại một cấu trúc vành duy nhất trên nhóm A[X] thoả mãn các tính chất sau:

a) Phép cộng trong vành này là phép cộng thường của A[X].

b) Phép nhân trong vành này mở rộng phép nhân của A.

c) Tích trong vành này của một dãy $(a,X, . . . ,X)$ gồm một phần tử $a$ của A được theo sau bởi $n$ số hạng bằng X, là đa thức $aX^n$.

d) Trong vành này, ta có $Xa=\sigma (a)X +d(a)$ với mọi $a\in A$.

Cho E là vành tự đồng cấu của nhóm cộng A[X]. Ánh xạ gửi $a\in A$ đến phép vị tự $a_M$ của A-môđun trái M = A[X] là một đồng cấu vành từ A đến E. Xét các phần tử $u,\sigma_M$, và $d_M$ của E được định nghĩa bởi $u(\sum b_nX^n) =\sum b_nX^{n+1},\sigma_M(\sum b_nX^n) =\sum\sigma (b_n)X^n$, $d_M(\sum b_nX^n) =\sum d(b_n)X^n$. Với mọi $a\in A$, ta có

$$
u a_M=a_Mu ,\sigma_Ma_M=\sigma (a)_M\sigma_M,d_Ma_M=\sigma (a)_Md_M+ (d(a)_M) \tag{2}
$$

Đặt

$$
X_M=\sigma_Mu+d_M \tag{3}
$$

Từ (2) suy ra rằng với mọi $a\in A$, ta có

$$
X_Ma_M=\sigma (a)_MX_M+ (d(a)_M) \tag{4}
$$

Xét ánh xạ $\varphi : A[X]\rightarrow E$ được định nghĩa bởi

$$
\varphi (\sum a_nX^n)=\sum(a_n)_M(X_M)^n \tag{5}
$$

Đây là một đồng cấu nhóm. Một lập luận quy nạp cho thấy ta có $(X_M)^n(1) = X^n$ với mọi $n\in \mathbf{N}$. Ta do đó có $\varphi (P)(1) = P$ với mọi $P\in A[X]$, điều này chứng minh rằng đồng cấu $\varphi$ là đơn ánh. Ta ký hiệu ảnh của nó bằng B. Tập hợp B là một nhóm con của E; nó chứa 1, và nó ổn định dưới phép nhân trái bởi $a_M$ với $a\in A$ và bởi $X_M$ (xem (4)). Nó do đó là một vành con của E. Cấu trúc vành duy nhất trên A[X] dẫn xuất từ cấu trúc trên B bằng chuyển cấu trúc qua $\varphi$ có các tính chất của Mệnh đề 7, trong đó tính chất d) xuất phát từ quan hệ (4).

Nếu A[X] được trang bị với một cấu trúc vành mang các tính chất của **Mệnh đề 7**, thì phép vị tự trái $\boldsymbol{\gamma }_X$ của vành này (I, §8, No. 1, p. 97) tất yếu gửi $bX^n$ đến $\sigma (b)X^{n+1}+d(b)X^n$ với $b\in A$ và $n\in \mathbf{N}$, do đó bằng $X_M$. Phép vị tự $\boldsymbol{\gamma }_a$ tất yếu bằng $a_M$ cho mọi $a\in A$. Do đó, ta có $\boldsymbol{\gamma }_P=\varphi (P)$ với mọi $P\in A[X]$; sự duy nhất trong **Mệnh đề 7** suy ra.

Tập hợp A[X], được trang bị cấu trúc vành duy nhất với các tính chất của Mệnh đề 7, được ký hiệu bởi $A[X]_{\sigma ,d}$ và được gọi là vành đa thức theo X với các hệ số trong A, tương đối với $\sigma$ và $d$. Ta đơn giản ký hiệu nó bởi $A[X]_{\sigma}$ khi $d$ là ánh xạ không và bởi A[X] khi hơn nữa, $\sigma$ là ánh xạ đồng nhất trên A. Ký hiệu này tương thích với ký hiệu đã được đưa vào trong IV, §1, No. 1, p. 1 cho một vành giao hoán A.

#### Chú ý {#alg-viii-s1-n4-rem-1 .statement tag=000T}

Vành $A[X]_{\sigma ,d}$ có tính chất phổ quát sau: cho một vành $A'$, một đồng cấu vành $f: A\rightarrow A'$, và một phần tử $x$ của $A'$ sao cho $xf(a) =f(\sigma (a))x+f(d(a))$ với mọi $a\in A$, tồn tại duy nhất một đồng cấu vành $g: A[X]_{\sigma ,d}\rightarrow A'$ mở rộng $f$ và gửi X tới $x$.

Tính duy nhất là rõ ràng. Do đó, ta hãy chỉ ra rằng ánh xạ $g: A[X]_{\sigma ,d}\rightarrow A'$ được định nghĩa bởi $g(\sum a_nX^n) =\sum f(a_n)x^n$ có các tính chất yêu cầu. Nó mở rộng $f$, ánh xạ X lên $x$, và là một đồng cấu nhóm. Ta có $g(1) = 1$. Với $a\in A$ và $Q =\sum a_nX^n$ trong $A[X]_{\sigma ,d}$, ta có

$$
g(aQ) =g(\sum aa_nX^n)=\sum f(aa_n)x^n=f(a)\sum f(a_n)x_n=g(a)g(Q)
$$

cũng như

$g$(XQ) $=g(\sum (\sigma (a_n)X^{n+1}+d(a_n)X^n))$

$$
=\sum(f(\sigma (a_n))x^{n+1}+f(d(a_n))x^n) =x\sum f(a_n)x^n=g(X)g(Q)
$$

Do đó ta có $g(P)g(Q) =g$(PQ) cho $P,Q$ trong $A[X]_{\sigma ,d}$ và do đó $g$ là một đồng cấu vành.

#### Định lý 2 {#alg-viii-s1-thm-2 .statement tag=000U}

Cho A là một vành Noether trái, và cho $\sigma$ là một tự đẳng cấu của A và $d$ là một tự đồng cấu của nhóm cộng của A thỏa mãn quan hệ (1). Vành $A[X]_{\sigma ,d}$ là Noether trái.

Đặt $B = A[X]_{\sigma ,d}$. Với mọi số nguyên $n\geqslant 0$, ta ký hiệu $B_n$ là tập hợp các phần tử của B có dạng $a_0+a_1X +\cdots +a_nX^n$. Nó là một A-môđun con trái của B. Ánh xạ $\varphi_n: B_n\rightarrow A_s$ được định nghĩa bởi $\varphi_n(a_0+a_1X +\cdots +a_nX^n) =a_n$ là A-tuyến tính.

Cho $\mathfrak{b}$ là một iđêan trái của B. Với mọi số nguyên $n\geqslant 0$, tập hợp $\mathfrak{a}_n=\varphi_n(\mathfrak{b}\cap B_n)$ là một iđêan trái của A. Vì ta có $Xa=\sigma (a)X +d(a)$ với mọi $a\in A$, nên ta có

(6) $\varphi_{n+1}$(XQ) $=\sigma (\varphi_n(Q))$

với mọi $Q\in B_n$ và do đó $\sigma (\mathfrak{a}_n)\subset \mathfrak{a}_{n+1}$. Do đó, dãy $\mathfrak{a}'_n=\sigma^{-n}(\mathfrak{a}_n)$ các iđêan của A là tăng. Vì vành A là Noether trái, tồn tại một số nguyên $m\geqslant 0$ sao cho $\mathfrak{a}'_n=\mathfrak{a}'_{n+1}$ với $n\geqslant m$. Vì $\sigma$ là toàn ánh, ta có quan hệ

$$
\sigma (\mathfrak{a}_n) =\mathfrak{a}_{n+1} \tag{7}
$$

với mọi số nguyên $n\geqslant m$.

Cho $\mathfrak{c}$ là iđêan trái của B sinh bởi $\mathfrak{b}\cap B_m$. Vì A-môđun trái $B_m$ sinh hữu hạn và vành A là Noether trái, A-môđun trái $\mathfrak{b}\cap B_m$ sinh hữu hạn (VIII, p. 7, Mệnh đề 4 a)). Iđêan trái $\mathfrak{c}$ do đó được sinh bởi một tập con hữu hạn của B. Rõ ràng nó được chứa trong $\mathfrak{b}$. Ta hãy chứng minh rằng nó bằng $\mathfrak{b}$ bằng cách chứng minh quy nạp rằng với mọi số nguyên $n\geqslant 0$, ta có

$$
\mathfrak{b}\cap B_n\subset \mathfrak{c} \tag{8}
$$

Quan hệ (8) đúng theo phép dựng với $n\leqslant m$. Từ đây, ta giả sử rằng $n$ là một số nguyên $\geqslant m$ sao cho $\mathfrak{b}\cap B_n\subset \mathfrak{c}$. Cho P là một phần tử của $\mathfrak{b}\cap B_{n+1}$. Khi đó $\varphi_{n+1}(P)$ thuộc $\mathfrak{a}_{n+1}=\sigma (\mathfrak{a}_n)$, và do đó tồn tại một phần tử Q của $\mathfrak{b}\cap B_n$ sao cho $\varphi_{n+1}(P) =\sigma (\varphi_n(Q))$. Đặt $R = P-$ XQ. Do quan hệ (6), ta có $\varphi_{n+1}(R) = 0$, tức là, $R\in B_n$. Vì P và Q thuộc iđêan trái $\mathfrak{b}$ của B, điều tương tự cũng đúng với R; do đó, R và Q thuộc $\mathfrak{b}\cap B_n$, là tập hợp được chứa trong iđêan $\mathfrak{c}$ theo giả thiết quy nạp. Do đó, P thuộc $\mathfrak{c}$. Điều này chứng minh rằng ta có $\mathfrak{b}\cap B_{n+1}\subset \mathfrak{c}$.

Suy ra rằng $\mathfrak{b}$ bằng $\mathfrak{c}$; do đó nó là một iđêan sinh hữu hạn của B. Điều này chứng minh rằng vành B là Noether trái.

Nếu tự đồng cấu $\sigma$ của vành A không phải là một tự đẳng cấu, thì vành $A[X]_{\sigma ,d}$ không tất yếu là Noether trái, ngay cả khi A là một vành giao hoán Noether (VIII, p. 22, Bài tập 26).

#### Hệ quả 1 (Hilbert) {#alg-viii-s1-thm-2-cor-1 .statement tag=00RW}

Cho A là một vành giao hoán Noether. Với mọi số nguyên $n\geqslant 0$, đại số đa thức $A[X_1, . . . ,X_n]$ là một vành Noether.

Điều này suy ra bằng quy nạp từ Định lý 2, có tính đến Mệnh đề 8 của III, §2, No. 9, p. 453.

#### Hệ quả 2 {#alg-viii-s1-thm-2-cor-2 .statement tag=000V}

Cho A là một vành giao hoán Noether. Một đại số trên A giao hoán được sinh bởi hữu hạn phần tử là một vành Noether.

Một đại số như vậy đẳng cấu với một đại số có dạng $A[X_1, . . . ,X_n]/\mathfrak{a}$, trong đó $n\geqslant 0$ và $\mathfrak{a}$ là một iđêan của $A[X_1, . . . ,X_n]$. Khi đó ta áp dụng Hệ quả 1 và Mệnh đề 5 của VIII, p. 7.

#### Hệ quả 3 {#alg-viii-s1-thm-2-cor-3 .statement tag=000W}

Mọi vành giao hoán đều là hợp của một họ có hướng phải gồm các vành con Noether.

Thật vậy, cho A là một vành giao hoán. Các vành con của A được sinh (với tư cách là các đại số trên $\mathbf{Z}$) bởi hữu hạn phần tử là Noether theo Hệ quả 2. Chúng tạo thành một họ có hướng phải các vành con của A, với hợp là A.

### Bài tập {#alg-viii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
