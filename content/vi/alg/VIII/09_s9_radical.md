---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 9
section_title: Radical
lang: vi
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.151-A VIII.172
pdf_pages: 0168-0189
extraction: native
subsections:
    - "no": 1
      title: The Radical of a Module
      page: 151
      pdf_page: 168
    - "no": 2
      title: The Radical of a Ring
      page: 154
      pdf_page: 171
    - "no": 3
      title: Nakayama’s Lemma
      page: 158
      pdf_page: 175
    - "no": 4
      title: Lifts of Idempotents
      page: 159
      pdf_page: 176
    - "no": 5
      title: Projective Cover of a Module
      page: 161
      pdf_page: 178
statements: 49
exercises: 31
content_sha256: d927788df931de19c3eba9cc906f4f807c299e0a45dfb121d1c5af76c3c758d7
translated_from: content/en/alg/VIII/09_s9_radical.md
source_content_sha256: 89095724e574bba079cd13ef874a02941adc59513c6a22e5a09bd9f01b4fa6cc
translation_model: gpt-5.4
translation_run: translate-vi-1732bc39
glossary_version: 34
glossary_terms_sha256: 0925f2c9d839575a0323636a6ad5ddbeddde00f15acbf6202b63afbea71c8d27
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. CĂN

### 1. Căn của một môđun

#### Định nghĩa 1 {#alg-viii-s9-def-1 .statement tag=00A1}

Cho A là một vành. Căn của một A-môđun M là môđun con được định nghĩa như là giao của các môđun con cực đại của M (VIII, p. 48, Định nghĩa 2) hoặc, tương đương, là tập hợp các phần tử của M bị triệt tiêu bởi mọi đồng cấu từ M đến một A-môđun đơn.

Trong phần còn lại của chương này, ta ký hiệu căn của một A-môđun M bởi $\mathfrak{R}_A(M)$ hoặc đơn giản là $\mathfrak{R}(M)$.

Cho A là một vành. Căn của một A-môđun M thu về 0 (trong trường hợp đó, do lạm dụng ngôn ngữ, ta nói rằng M không có căn) khi và chỉ khi tồn tại một họ $(S_i)_{i\in I}$ các A-môđun đơn và một họ $(f_i)_{i\in I}$ các ánh xạ A-tuyến tính $f_i: M\rightarrow S_i$ sao cho ta có $\cap_{i\in I}$ Ker($f_i$) $= 0$. Điều này tương đương với việc M đẳng cấu với một môđun con của một tích các A-môđun đơn.

#### Ví dụ 1 {#alg-viii-s9-n1-exa-1 .statement tag=00A2}

Cho $\mathfrak{a}$ là một iđêan trái của A. Căn của A-môđun $A_s/\mathfrak{a}$ bằng $\mathfrak{a}'/\mathfrak{a}$, trong đó $\mathfrak{a}'$ là giao của các iđêan trái cực đại của A chứa $\mathfrak{a}$. Đặc biệt, căn của $\mathbf{Z}$-môđun $\mathbf{Z}$ thu về 0, và căn của $\mathbf{Z}$-môđun $\mathbf{Z}/p^n\mathbf{Z}$ bằng $p\mathbf{Z}/p^n\mathbf{Z}$ với mọi số nguyên tố $p$ và mọi số nguyên $n\geqslant 1$.

#### Ví dụ 2 {#alg-viii-s9-n1-exa-2 .statement tag=00A3}

Cho A là một miền iđêan chính không phải là một trường, và K là trường phân thức của nó. Với tư cách là một K-môđun, K không có căn. Hãy chứng minh rằng căn của K, được xem như một A-môđun, bằng K; tương đương, phải chứng minh rằng mọi ánh xạ A-tuyến tính $f$ từ K đến một A-môđun đơn S đều bằng không. Theo VII, §4, No. 8, p. 25, ta có thể giả sử rằng S bằng $A/(\pi )$, trong đó $\pi$ là một phần tử bất khả quy của A. Ta có $f(x) =f(\pi \frac{x}{\pi})=\pi f(\frac{x}{\pi})= 0$ với mọi $x\in K$ vì $\pi S = 0$.

#### Mệnh đề 1 {#alg-viii-s9-prop-1 .statement tag=00A4}

Cho M và N là các A-môđun và $f$ là một đồng cấu từ M đến N. Ta có $f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$, và thậm chí còn có đẳng thức nếu $f$ là toàn ánh và hạt nhân của $f$ được chứa trong căn của M.

Cho $g$ là một đồng cấu từ N vào một A-môđun đơn; khi đó $\mathfrak{R}(M)$ được chứa trong hạt nhân của $g\circ f$, nên $f(\mathfrak{R}(M))$ được chứa trong hạt nhân của $g$. Do đó ta có $f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$. Bây giờ giả sử rằng $f$ là toàn ánh và hạt nhân của nó được chứa trong $\mathfrak{R}(M)$. Cho $y$ là một phần tử của $\mathfrak{R}$(N), và cho $x$ là một phần tử của ảnh ngược của $y$. Nếu $g$ là một đồng cấu từ M vào một A-môđun đơn S, thì hạt nhân của nó chứa căn của M, do đó chứa hạt nhân của $f$. Vì đồng cấu $f$ là toàn ánh, tồn tại một đồng cấu $h$ từ N vào S sao cho $g=h\circ f$. Vì $y=f(x)$ thuộc $\mathfrak{R}$(N), ta có $h(f(x)) = 0$, nghĩa là $g(x) = 0$; do đó $x$ thuộc $\mathfrak{R}$(M), điều này chứng minh bao hàm $\mathfrak{R}(N)\subset f(\mathfrak{R}(M))$.

#### Hệ quả 1 {#alg-viii-s9-prop-1-cor-1 .statement tag=00A5}

Cho M là một A-môđun và N là một môđun con của M.

a) Ta có $\mathfrak{R}(N)\subset \mathfrak{R}(M)\cap N$.

b) Ta có $(\mathfrak{R}(M) + N)/N\subset \mathfrak{R}(M/N)$. Nếu N được chứa trong $\mathfrak{R}(M)$, thì ta có đẳng thức $\mathfrak{R}(M/N) =\mathfrak{R}(M)/N$.

c) Môđun $M/\mathfrak{R}(M)$ không có căn. Nếu môđun $M/N$ không có căn, thì ta có $\mathfrak{R}(M)\subset N$.

Mệnh đề a) suy ra từ Mệnh đề 1 áp dụng cho đơn ánh chính tắc từ N vào M, và mệnh đề b) suy ra từ Mệnh đề 1 áp dụng cho ánh xạ chính tắc từ M vào $M/N$. Từ b), ta suy ra rằng $M/N$ không có căn nếu $N =\mathfrak{R}(M)$ và rằng ta có $\mathfrak{R}(M)\subset N$ nếu $M/N$ không có căn.

Từ Ví dụ 1 suy ra rằng có thể tồn tại những môđun con N chứa $\mathfrak{R}(M)$ sao cho căn của $M/N$ không bằng không.

#### Hệ quả 2 {#alg-viii-s9-prop-1-cor-2 .statement tag=00A6}

Cho $(M_i)_{i\in I}$ là một họ các A-môđun, P là tích của nó, và S là tổng trực tiếp của nó. Ta có $\mathfrak{R}(P)\subset \prod_{i\in I}\mathfrak{R}(M_i)$ và $\mathfrak{R}(S) =\bigoplus_{i\in I}\mathfrak{R}(M_i)$.

Với $i\in I$, gọi $\pi_i$ là phép chiếu chỉ số $i$ từ P lên $M_i$. Theo Mệnh đề 1, ta có $\pi_i(\mathfrak{R}(P))\subset \mathfrak{R}(M_i)$ với mọi $i\in I$; điều này chứng minh mệnh đề thứ nhất. Ta có $S\subset P$, do đó

$$
\mathfrak{R}(S)\subset S\cap \mathfrak{R}(P)\subset S\cap \prod_{i\in I}\mathfrak{R}(M_i) =\bigoplus_{i\in I}\mathfrak{R}(M_i)
$$

Hơn nữa, ta có $M_i\subset S$ và vì vậy $\mathfrak{R}(M_i)\subset \mathfrak{R}(S)$ với mọi $i\in I$, và do đó $\oplus_{i\in I}\mathfrak{R}(M_i)\subset \mathfrak{R}(S)$.

Tồn tại những họ môđun sao cho căn của tích không đẳng cấu với tích của các căn (Bài tập 3 của VIII, p. 166).

#### Mệnh đề 2 {#alg-viii-s9-prop-2 .statement tag=00A7}

Cho M là một A-môđun hữu hạn sinh.

a) Nếu M không thu về 0, thì ta có $\mathfrak{R}(M)\not= M$.

b) Nếu N là một môđun con của M sao cho $N +\mathfrak{R}(M) = M$, thì ta có N = M.

Cho N là một môđun con thực sự của M. Theo Mệnh đề 3 của VIII, p. 49, tồn tại một môđun con cực đại L của M chứa N. Ta có $N +\mathfrak{R}(M)\subset L$, và a fortiori $N +\mathfrak{R}(M)\not= M$. Điều này chứng minh b); trường hợp riêng N = 0 cho mệnh đề a).

#### Hệ quả {#alg-viii-s9-n1-cor-1 .statement tag=00A8}

Cho M là một A-môđun, $(x_i)_{i\in I}$ một họ sinh của M, và $x$ một phần tử của M. Các tính chất sau là tương đương:

(i) Ta có $x\in \mathfrak{R}(M)$.

(ii) Mọi môđun con N của M sao cho $N + Ax= M$ đều bằng M.

(iii) Với mọi họ $(a_i)_{i\in I}$ các phần tử của A, họ $(x_i+a_ix)_{i\in I}$ sinh A-môđun M.

(i) $\Rightarrow$ (ii): Giả sử rằng $x$ thuộc $\mathfrak{R}(M)$. Gọi N là một môđun con của M sao cho $N + Ax= M$. Ta có $N +\mathfrak{R}(M) = M$; do đó A-môđun $M/N$ bằng căn của nó (Hệ quả 1, b) của Mệnh đề 1). Vì nó là đơn sinh, nên nó bằng không (Mệnh đề 2), và ta có M = N.

(ii) $\Rightarrow$ (iii): Cho $(a_i)_{i\in I}$ là một họ các phần tử của A. Ký hiệu bởi N môđun con của M được sinh bởi họ $(x_i+a_ix)_{i\in I}$. Ta có $x_i\in N + Ax$ với mọi $i\in I$, do đó $N + Ax= M$. Nếu tính chất (ii) đúng, thì N bằng M.

(iii) $\Rightarrow$ (i): Giả sử rằng $x$ không thuộc $\mathfrak{R}(M)$. Khi đó tồn tại một môđun con cực đại N của M không chứa $x$. Vì N là cực đại, ta có $N + Ax= M$; do đó mỗi phần tử $x_i$ đều có thể viết được dưới dạng $y_i-a_ix$ với $y_i\in N$ và $a_i\in A$. Họ $(x_i+a_ix)_{i\in I}$ được chứa trong N, nên không sinh ra M.

#### Mệnh đề 3 {#alg-viii-s9-prop-3 .statement tag=00A9}

a) Một môđun nửa đơn không có căn.

b) Một môđun là nửa đơn và sinh hữu hạn khi và chỉ khi nó không có căn và Artin.

Theo định nghĩa, căn của một môđun đơn thu về 0. Nếu môđun M là nửa đơn, thì nó là tổng trực tiếp của một họ $(S_i)_{i\in I}$ các môđun con đơn, và ta có $\mathfrak{R}(M) =\bigoplus_{i\in I}\mathfrak{R}(S_i)$ theo Hệ quả 2 của Mệnh đề 1 ở trên, do đó $\mathfrak{R}(M) = 0$.

Nếu hơn nữa M sinh hữu hạn, thì nó là Artin theo Mệnh đề 10 của VIII, p. 71.

Ngược lại, giả sử rằng M là Artin và không có căn. Theo VIII, p. 2 áp dụng cho tập hợp các môđun con cực đại của M, tồn tại một họ hữu hạn $(N_i)_{i\in I}$ các môđun con cực đại của M mà giao của chúng thu về 0. Khi đó M đẳng cấu với một môđun con của $\bigoplus_{i\in I}(M/N_i)$. Do đó, nó là nửa đơn và có độ dài hữu hạn, và a fortiori sinh hữu hạn.

### 2. Căn của một vành

#### Định nghĩa 2 {#alg-viii-s9-def-2 .statement tag=00AA}

Căn Jacobson (hay đơn giản là căn) của một vành A, ký hiệu là $\mathfrak{R}(A)$, là căn của A-môđun $A_s$, tức là giao của các iđêan trái cực đại của A.

Theo lối nói lạm dụng, ta nói rằng vành A không có căn nếu ta có $\mathfrak{R}(A) = 0$.

#### Mệnh đề 4 {#alg-viii-s9-prop-4 .statement tag=00AB}

Một vành A là nửa đơn khi và chỉ khi nó là Artin trái và không có căn.

Điều này suy ra từ Mệnh đề 3, b), áp dụng cho A-môđun $A_s$.

#### Ví dụ 1 {#alg-viii-s9-n2-exa-1 .statement tag=00AC}

Nếu A là một vành địa phương, thì nó có một iđêan trái cực đại duy nhất $\mathfrak{r}$, gồm các phần tử không khả nghịch của A (VIII, p. 25, Mệnh đề 1); do đó $\mathfrak{r}$ là căn của A. Đặc biệt, một trường không có căn.

#### Ví dụ 2 {#alg-viii-s9-n2-exa-2 .statement tag=00AD}

Cho K là một trường giao hoán và E là đại số $K[[X_i]]_{i\in I}$ của các chuỗi lũy thừa hình thức theo các biến $X_i$ với hệ số trong K. Theo ví dụ trước và Ví dụ 4 của VIII, p. 26, căn của E gồm các chuỗi lũy thừa hình thức có số hạng hằng bằng không. Nhận thấy rằng vành E là một miền nguyên và căn của nó không thu về 0, mặc dù E là một vành con của trường phân thức của nó, vốn không có căn.

#### Ví dụ 3 {#alg-viii-s9-n2-exa-3 .statement tag=00AE}

Giả sử rằng A là một miền iđêan chính, và cho P là một hệ đại diện gồm các phần tử bất khả quy (VII, §1, No. 3, p. 3). Nếu A là một trường, thì nó không có căn theo Ví dụ 1. Nếu tập hợp P là vô hạn, thì giao của các iđêan cực đại $Ap$ của A thu về 0, nên A không có căn. Nhưng nếu P là hữu hạn và khác rỗng, và nếu đặt $x=\prod_{p\in P}p$, thì căn của A bằng $\cap_{p\in P}Ap= Ax$ (VII, §1, No. 2, p. 3, Mệnh đề 4), do đó không thu về 0.

Cho $y$ là một phần tử khác không của A; ta viết nó dưới dạng $y=up^{i_1}_1\cdots p^{i_r}_r$, trong đó $u$ khả nghịch trong $A,p_1, . . . , p_r$ là các phần tử của P từng đôi một phân biệt, và $i_1, . . . , i_r$ là các số nguyên dương ngặt. Các iđêan cực đại của vành $A/Ay$ là các iđêan $Ap_1/Ay, . . . ,Ap_r/Ay$; do đó căn của vành $A/Ay$ là iđêan $Ap_1\cdots p_r/Ay$. Đặc biệt, vành $A/Ay$ không có căn khi và chỉ khi ta có $i_1=\cdots =i_r= 1$; trong trường hợp này, ta nói rằng $y$ không có thừa số bội.

#### Mệnh đề 5 {#alg-viii-s9-prop-5 .statement tag=00AF}

a) Căn của một vành A là giao của các linh hóa tử của các A-môđun đơn; nó cũng là linh hóa tử nhỏ nhất của một A-môđun nửa đơn. Đặc biệt, nó là một iđêan hai phía của A. Nếu A không thu về 0, thì căn của A phân biệt với A.

b) Cho $\mathfrak{a}$ là một iđêan hai phía của A. Ta có $(\mathfrak{R}(A) +\mathfrak{a})/\mathfrak{a}\subset \mathfrak{R}(A/\mathfrak{a})$. Nếu $\mathfrak{a}$ được chứa trong $\mathfrak{R}(A)$, thì ta có $\mathfrak{R}(A/\mathfrak{a}) =\mathfrak{R}(A)/\mathfrak{a}$.

c) Vành $A/\mathfrak{R}(A)$ không có căn; ngược lại, mọi iđêan hai phía $\mathfrak{a}$ của A sao cho $A/\mathfrak{a}$ không có căn đều chứa $\mathfrak{R}(A)$.

d) Căn của A được chứa trong giao của các iđêan hai phía cực đại của A.

Cho $x\in A$. Nói rằng $x$ thuộc linh hóa tử của mọi A-môđun đơn là tương đương với nói rằng $x$ thuộc linh hóa tử của mọi phần tử của mọi A-môđun đơn, nói cách khác (VIII, p. 46, Mệnh đề 1), của mọi iđêan trái cực đại của A.

Cho M là một A-môđun nửa đơn. Linh hóa tử của nó là giao của các linh hóa tử của các môđun con đơn của M, nên nó chứa $\mathfrak{R}(A)$. Hơn nữa, nếu $\mathscr{S}$ là tập hợp các lớp của các A-môđun đơn (VIII, p. 51), thì tổng trực tiếp $\oplus_{\lambda\in\mathscr{S}}\lambda$ là một A-môđun nửa đơn mà linh hóa tử là $\mathfrak{R}(A)$. Giả sử A không quy về 0; quan hệ $\mathfrak{R}(A)\not= A$ suy ra từ Mệnh đề 2, a) của VIII, p. 153 áp dụng cho A-môđun $A_s$. Ta đã chứng minh a).

Cho $\mathfrak{a}$ là một iđêan hai phía của A. Các iđêan trái cực đại của $A/\mathfrak{a}$ là các iđêan dạng $\mathfrak{m}/\mathfrak{a}$, trong đó $\mathfrak{m}$ là một iđêan trái cực đại của A chứa $\mathfrak{a}$. Do đó, căn của vành $A/\mathfrak{a}$ bằng căn của A-môđun $A_s/\mathfrak{a}$. Các khẳng định b) và c) do đó suy ra từ Hệ quả 1 của VIII, p. 152.

Cho $\mathfrak{a}$ là một iđêan hai phía tối đại của A. Trong vành $A/\mathfrak{a}$, các iđêan hai phía duy nhất là 0 và $A/\mathfrak{a}$. Vì vành $A/\mathfrak{a}$ không bị quy về 0, nên căn của nó không bằng $A/\mathfrak{a}$. Vậy vành $A/\mathfrak{a}$ không có căn, và ta có $\mathfrak{R}(A)\subset \mathfrak{a}$ theo c). Điều đó chứng minh d).

Ta nói rằng một iđêan trái (hoặc phải) của A là một iđêan nil nếu nó gồm các phần tử lũy linh. Ta nói rằng một iđêan hai phía $\mathfrak{a}$ của A là lũy linh nếu tồn tại một số nguyên $n\geqslant 1$ sao cho $\mathfrak{a}^n= 0$, nghĩa là (I, §8, No. 9, p. 107), sao cho ta có $x_1\cdots x_n= 0$ đối với mọi dãy $(x_1, . . . , x_n)$ các phần tử của $\mathfrak{a}$. Mọi iđêan hai phía lũy linh đều là iđêan nil, nhưng có thể tồn tại những iđêan nil không được chứa trong một iđêan hai phía lũy linh nào cả (VIII, p. 167, Bài tập 9).

#### Định lý 1 (Jacobson) {#alg-viii-s9-thm-1 .statement tag=00S5}

Căn của một vành A gồm các phần tử $x\in A$ sao cho $1 +ax$ là khả nghịch trái (I, §2, No. 3, p. 15) với mọi $a\in A$. Nó cũng là iđêan hai phía lớn nhất $\mathfrak{a}$ sao cho $1 +x$ là khả nghịch với mọi $x\in \mathfrak{a}$. Căn của A chứa mọi iđêan nil trái của A.

Phần tử 1 sinh ra A-môđun $A_s$, và $1 +ax$ là khả nghịch trái khi và chỉ khi nó sinh ra A-môđun $A_s$. Do đó mệnh đề thứ nhất của Định lý 1 là một trường hợp riêng của hệ quả của Mệnh đề 2 (VIII, p. 153).

Cho $x\in \mathfrak{R}(A)$. Theo điều trên, $1 +x$ là khả nghịch trái; gọi $y$ là một phần tử của A sao cho $y(1 +x) = 1$. Khi đó ta có $1-y=yx$, nên $1-y$ thuộc $\mathfrak{R}(A)$; do đó $y$ là khả nghịch trái. Vì $y$ cũng khả nghịch phải, nên nó khả nghịch (I, §2, No. 3, p. 16, Mệnh đề 3), và nghịch đảo phải của nó là $1 +x$ cũng vậy.

Cho $\mathfrak{a}$ là một iđêan trái của A sao cho $1 +x$ là khả nghịch với mọi $x\in \mathfrak{a}$. Điều này đúng, chẳng hạn, khi $\mathfrak{a}$ là một iđêan nil vì quan hệ $x^n= 0$ kéo theo rằng $1-x+\cdots + (-x)^{n-1}$ là nghịch đảo của $1 +x$. Cho $x\in \mathfrak{a}$. Với mọi $a\in A$, ta có $ax\in \mathfrak{a}$, nên $1 +ax$ là khả nghịch; do đó, ta có $x\in \mathfrak{R}(A)$. Suy ra $\mathfrak{a}$ được chứa trong $\mathfrak{R}(A)$.

#### Hệ quả 1 {#alg-viii-s9-thm-1-cor-1 .statement tag=00AG}

Căn của A bằng căn của vành đối $A^o$, nghĩa là bằng giao của các iđêan phải cực đại của A.

Với mọi $x\in \mathfrak{R}$(A), $1 +x$ là khả nghịch trong vành A, do đó cũng khả nghịch trong vành $A^o$. Vì $\mathfrak{R}(A)$ là một iđêan hai phía của $A^o$, nên ta có $\mathfrak{R}(A)\subset \mathfrak{R}(A^o)$. Đẳng thức suy ra bằng cách đổi chỗ vai trò của A và $A^o$.

#### Hệ quả 2 {#alg-viii-s9-thm-1-cor-2 .statement tag=00AH}

Một phần tử của A là khả nghịch khi và chỉ khi ảnh chính tắc của nó trong vành $A/\mathfrak{R}(A)$ là khả nghịch.

Điều kiện này hiển nhiên là cần thiết. Hãy chứng minh rằng nó là đủ. Gọi $x$ là một phần tử của A mà ảnh chính tắc của nó trong vành $A/\mathfrak{R}(A)$ là khả nghịch. Khi đó tồn tại một phần tử $y$ của A sao cho $xy$ thuộc $1 +\mathfrak{R}(A)$. Theo Định lý 1$,xy$ là khả nghịch; do đó $x$ khả nghịch phải. Chứng minh rằng $x$ khả nghịch trái là tương tự.

#### Hệ quả 3 {#alg-viii-s9-thm-1-cor-3 .statement tag=00AI}

Căn của tích của một họ các vành $(A_i)_{i\in I}$ là tích của các $\mathfrak{R}(A_i)$.

Cho $x= (x_i)_{i\in I}$ là một phần tử của $\prod_{i\in I}A_i$. Với mọi phần tử $a= (a_i)_{i\in I}$ của $\prod_{i\in I}A_i$, phần tử $1 +ax$ là khả nghịch trái nếu và chỉ nếu $1 +a_ix_i$ là khả nghịch trái trong $A_i$ với mọi $i\in I$. Suy ra Hệ quả 3.

#### Hệ quả 4 {#alg-viii-s9-thm-1-cor-4 .statement tag=00AJ}

Vành A là địa phương nếu và chỉ nếu vành $A/\mathfrak{R}(A)$ là một trường. Nếu đúng như vậy, thì $\mathfrak{R}(A)$ là tập hợp các phần tử không khả nghịch của A.

Ký hiệu tập hợp các phần tử không khả nghịch của A là $\mathfrak{r}$. Nếu vành A là địa phương, thì căn của nó bằng $\mathfrak{r}$ (VIII, p. 154, Ví dụ 1) và vành $A/\mathfrak{r}$ là một trường (VIII, p. 26). Ngược lại, giả sử rằng vành $A/\mathfrak{R}(A)$ là một trường. Theo Hệ quả 2, ta có $\mathfrak{r}=\mathfrak{R}$(A), nên $\mathfrak{r}$ là một iđêan hai phía của A. Suy ra vành A là địa phương (VIII, p. 26, Định nghĩa 1).

#### Ví dụ 4 {#alg-viii-s9-n2-exa-4 .statement tag=00AK}

Cho K là một miền nguyên, I một tập hợp khác rỗng, và A là vành đa thức $K[X_i]_{i\in I}$. Ta sẽ chứng minh rằng vành A không có căn. Các phần tử khả nghịch duy nhất của A là các phần tử khả nghịch của K (IV, §1, No. 5, p. 9, Hệ quả 2). Cho $f\in \mathfrak{R}(A)$. Chọn một phần tử $i\in I$. Khi đó $1 +fX_i$ là khả nghịch (Định lý 1), điều này kéo theo $f= 0$.

Chú ý rằng khi K là một trường giao hoán, vành $A = K[X_i]_{i\in I}$ là một vành con của $B = K[[X_i]]_{i\in I}$ và ta có $\mathfrak{R}(A) = 0$ và $A\cap \mathfrak{R}(B)\not= 0$ (x. VIII, p. 154, Ví dụ 2).

#### Ví dụ 5 {#alg-viii-s9-n2-exa-5 .statement tag=00AL}

Cho $\mathfrak{a}$ là một iđêan hai phía của A. Tôpô $\mathfrak{a}$-adic trên A là tôpô, tương thích với cấu trúc vành của A, sao cho các iđêan $\mathfrak{a}^n$ (với $n\geqslant 1$) tạo thành một hệ cơ bản các lân cận của 0 (Gen. Top., III, §6, No. 3, p. 275, Ví dụ 3). Giả sử rằng vành A là Hausdorff và đầy đủ (Gen. Top., III, §6, No. 5, p. 276) đối với tôpô này; chẳng hạn điều đó xảy ra khi iđêan $\mathfrak{a}$ là lũy linh. Khi đó, với mọi $x\in \mathfrak{a}$, chuỗi $\sum^{\infty}_{n=0}(-x)^n$ hội tụ. Gọi $y$ là tổng của nó. Ta có $y-1 =\sum^{\infty}_{n=1}(-x)^n=-xy$, do đó $(1 +x)y= 1$. Tương tự, ta có $y(1 +x) = 1$, nên $1 +x$ khả nghịch. Theo Định lý 1, suy ra iđêan $\mathfrak{a}$ được chứa trong căn của A.

#### Nhận xét 1 {#alg-viii-s9-n2-rem-1 .statement tag=00AM}

Theo Định lý 1, mọi iđêan nil trái của một vành A đều được chứa trong

căn của nó. Cho $x$ là một phần tử lũy linh và trung tâm của A; khi đó $Ax$ là một iđêan nil của A, nên $x$ thuộc căn của A. Tuy nhiên, có thể xảy ra rằng tồn tại các phần tử lũy linh khác không của A nhưng A lại không có căn. Chẳng hạn, với mọi số nguyên $n\geqslant 2$, vành ma trận $\mathbf{M}_n(K)$ trên một trường K là đơn, do đó không có căn (VIII, p. 154, Mệnh đề 4), và nó chứa các phần tử lũy linh, chẳng hạn các đơn vị ma trận $E_{ij}$ với $i\not=j$.

#### Nhận xét 2 {#alg-viii-s9-n2-rem-2 .statement tag=00AN}

Cho A là một vành giao hoán. Tập hợp các phần tử lũy linh $a$ của A là một iđêan $\mathfrak{N}(A)$ của A, được gọi là căn lũy linh của A; nó là giao của các iđêan nguyên tố của A (V, §15, No. 1, p. 118, Mệnh đề 2). Ta có $\mathfrak{N}(A)\subset \mathfrak{R}(A)$; $*$ta có đẳng thức nếu A là một vành Artin (VIII, p. 173, Hệ quả 2) hoặc một đại số giao hoán sinh hữu hạn trên một trường giao hoán (Comm. Alg., V, § 3, n$^{\circ}4$, Định lý $3$)$*$. Hoàn toàn có thể có $\mathfrak{N}(A)\not=\mathfrak{R}(A)$. Đó là trường hợp khi A là vành K[[X]], trong đó K là một trường giao hoán: khi đó ta có $\mathfrak{N}(A) = 0$ và $\mathfrak{R}(A) =$ AX (VIII, p. 154, Ví dụ 2).

### 3. Bổ đề Nakayama

#### Mệnh đề 6 {#alg-viii-s9-prop-6 .statement tag=00AO}

Với mọi A-môđun M, ta có $\mathfrak{R}(A)M\subset \mathfrak{R}(M)$. Ta có đẳng thức nếu A-môđun M là xạ ảnh.

Cho P là một môđun con cực đại của M; A-môđun $M/P$ là đơn, nên bị triệt tiêu bởi $\mathfrak{R}(A)$ theo Mệnh đề 5 của VIII, p. 155. Do đó ta có $\mathfrak{R}(A)M\subset P$ với mọi môđun con cực đại P của M, suy ra $\mathfrak{R}(A)M\subset \mathfrak{R}(M)$.

Ta rõ ràng có $\mathfrak{R}(A_s) =\mathfrak{R}(A)A_s$. Nếu A-môđun M là xạ ảnh, thì tồn tại một A-môđun N sao cho $M\oplus N$ là tự do, tức là, tổng trực tiếp của một họ $(L_i)_{i\in I}$ các môđun đẳng cấu với $A_s$. Theo Hệ quả 2 của VIII, p. 152, ta có $\mathfrak{R}(M\oplus N) =\mathfrak{R}(M)\oplus \mathfrak{R}(N)$ và $\mathfrak{R}(\bigoplus_{i\in I}L_i)=\bigoplus_{i\in I}\mathfrak{R}(L_i)$. Khi đó ta suy ra $\mathfrak{R}(M) =\mathfrak{R}(A)M$ từ đẳng thức $\mathfrak{R}(L_i) =\mathfrak{R}(A)L_i$.

#### Định lý 2 (“Bổ đề Nakayama”) {#alg-viii-s9-thm-2 .statement tag=00S6}

Cho M là một A-môđun và $\mathfrak{a}$ là một iđêan hai phía của A. Giả sử rằng một trong các điều kiện sau được thỏa mãn:

(i) A-môđun M sinh hữu hạn, và $\mathfrak{a}$ được chứa trong căn của A.

(ii) Iđêan $\mathfrak{a}$ lũy linh.

Nếu N là một môđun con của M sao cho $M = N +\mathfrak{a}M$, thì ta có N = M. Đặc biệt, nếu môđun M khác không, thì ta có $M\not=\mathfrak{a}M$.

Giả sử rằng M là sinh hữu hạn và ta có $\mathfrak{a}\subset \mathfrak{R}(A)$. Gọi N là một môđun con của M sao cho $M = N +\mathfrak{a}M$. Theo Mệnh đề 6, ta có $M = N +\mathfrak{R}$(M), do đó M = N theo Mệnh đề 2, b) của VIII, p. 153.

Bây giờ giả sử rằng $\mathfrak{a}$ là lũy linh, và gọi N là một môđun con của M sao cho $M = N +\mathfrak{a}M$. Bằng quy nạp theo số nguyên $n\geqslant 0$, ta thiết lập quan hệ $M = N +\mathfrak{a}^nM$. Theo giả thiết, tồn tại một số nguyên $n\geqslant 0$ sao cho $\mathfrak{a}^n= 0$; do đó M = N.

Khẳng định cuối cùng của định lý suy ra từ điều trên bằng cách lấy N bằng 0.

#### Hệ quả 1 {#alg-viii-s9-thm-2-cor-1 .statement tag=00R9}

Ta giữ nguyên các giả thiết của Định lý 2. Cho $(x_i)_{i\in I}$ là một họ các phần tử của M, và cho $\overline{x}_i$ là ảnh chính tắc của $x_i$ trong $M/\mathfrak{a}M$. Nếu họ $(\overline{x}_i)_{i\in I}$ sinh $(A/\mathfrak{a})$-môđun $M/\mathfrak{a}M$, thì họ $(x_i)_{i\in I}$ sinh A-môđun M.

Điều này suy ra từ Định lý 2 áp dụng cho môđun con N của M được sinh bởi họ $(x_i)_{i\in I}$.

#### Hệ quả 2 {#alg-viii-s9-thm-2-cor-2 .statement tag=00AP}

Ta giữ các giả thiết của Định lý 2. Ngoài ra, cho $M'$ là một A-môđun và $u: M'\rightarrow M$ là một đồng cấu. Nếu đồng cấu $\overline{u}$ từ $M'/\mathfrak{a}M'$ đến $M/\mathfrak{a}M$ suy ra từ $u$ bằng cách chuyển qua các thương là toàn ánh, thì $u$ là toàn ánh.

Chỉ cần áp dụng Định lý 2 cho ảnh N của $u:$ thật vậy, ảnh của $\overline{u}$ là $(N +\mathfrak{a}M)/\mathfrak{a}M$, nên $\overline{u}$ là toàn ánh khi và chỉ khi ta có $N +\mathfrak{a}M = M$.

### 4. Nâng các phần tử lũy đẳng

#### Bổ đề 1 {#alg-viii-s9-lem-1 .statement tag=00AQ}

Cho $a$ là một phần tử của một vành A sao cho $a-a^2$ là lũy linh. Tồn tại một đa thức P trong $X + (X-X^2)\mathbf{Z}[X]$ sao cho $P(a)$ là lũy đẳng trong A.

Cho $n$ là một số nguyên dương ngặt sao cho $(a-a^2)^n= 0$. Đặt P(X) = $1-(1-X^n)^n$. Đa thức P(X) là một bội của $X^n$, và đa thức $1-P(X)$ là một bội của $(1-X)^n$, nên $P(X)-P(X)^2$ là một bội của $(X-X^2)^n$, và ta có $P(a) = P(a)^2$. Hơn nữa, $X-P(X)$ là một bội của X và $1-X$, do đó là một bội của $X-X^2$.

#### Mệnh đề 7 {#alg-viii-s9-prop-7 .statement tag=00AR}

Cho $\mathfrak{a}$ là một iđêan lũy linh hai phía của A, và cho $\overline{e}$ là một phần tử lũy đẳng trong vành $A/\mathfrak{a}$. Tồn tại một phần tử lũy đẳng $e$ trong A mà ảnh chính tắc của nó trong $A/\mathfrak{a}$ bằng $\overline{e}$.

Cho $a$ là một đại diện tùy ý của $\overline{e}$ trong A. Phần tử $a-a^2$ của A là lũy linh vì nó thuộc $\mathfrak{a}$. Chọn một đa thức $P\in \mathbf{Z}[X]$ thỏa mãn các điều kiện của Bổ đề 1. Ta có $a-P(a)\in A(a-a^2)$, nên phần tử $e= P(a)$ của A có tính chất mong muốn.

Giả sử rằng $\overline{e}$ thuộc tâm của vành $A/\mathfrak{a}$. Không nhất thiết tồn tại một phần tử lũy đẳng $e$ trong tâm Z của A nâng $\overline{e}$ lên (VIII, p. 172, Bài tập 31). Tuy nhiên, nếu $\overline{e}$ thuộc ảnh của Z trong $A/\mathfrak{a}$, thì nó nâng thành một phần tử lũy đẳng trong Z vì $Z\cap \mathfrak{a}$ là một iđêan nil của Z.

#### Hệ quả 1 {#alg-viii-s9-prop-7-cor-1 .statement tag=00AS}

Cho M và P là các A-môđun và $u$ là một ánh xạ A-tuyến tính toàn ánh từ P lên M. Giả sử rằng P là xạ ảnh và tồn tại một iđêan hai phía lũy linh $\mathfrak{a}$ của A sao cho hạt nhân N của $u$ được chứa trong $\mathfrak{a}P$. Cho $M'$ và $M''$ là các môđun con của M mà tổng trực tiếp của chúng là M. Khi đó P là tổng trực tiếp của các môđun con $P'$ và $P''$ sao cho $u(P') = M'$ và $u(P'') = M''$.

Ký hiệu B là vành con của End$_A(P)$ gồm các tự đồng cấu $f$ của P sao cho $f(N)\subset N$. Gọi $\overline{B}$ là vành các tự đồng cấu của M. Với $f\in B$, gọi $\overline{f}$ là tự đồng cấu duy nhất của M sao cho $\overline{f}\circ u=u\circ f$. Ánh xạ $f\mapsto \overline{f}$ là một đồng cấu vành từ B vào B. Vì môđun P là xạ ảnh, đồng cấu này là toàn ánh; hạt nhân của nó $\mathfrak{b}$ gồm các tự đồng cấu $f\in B$ sao cho $f(P)\subset N$. Gọi $n$ là một số tự nhiên sao cho $\mathfrak{a}^n= 0$. Ta có

$$
P =\mathfrak{a}^0P\supset \mathfrak{a}^1P\supset  \cdots  \supset \mathfrak{a}^{n-1}P\supset \mathfrak{a}^nP = 0
$$

và, với mọi $f\in \mathfrak{b}$ và mọi số nguyên $j\geqslant 0$,

$$
f(\mathfrak{a}^jP) =\mathfrak{a}^jf(P)\subset \mathfrak{a}^jN\subset \mathfrak{a}^{j+1}P
$$

vì $N\subset \mathfrak{a}P$ theo giả thiết. Do đó ta có $f(P)\subset \mathfrak{a}^jP$ với mọi số tự nhiên $j$ và mọi $f\in \mathfrak{b}^j$. Đặc biệt, ta có $\mathfrak{b}^n= 0$.

Cho $\varepsilon '$ là phép chiếu của M có ảnh $M'$ và hạt nhân $M''$. Theo Mệnh đề 7 áp dụng cho vành B và iđêan hai phía lũy linh $\mathfrak{b}$, tồn tại một lũy đẳng $e'$ trong B sao cho $\overline{e'}=\varepsilon '$, tức là, $\varepsilon '\circ u=u\circ e'$. Đặt $e''= 1-e'$, $\varepsilon ''=\overline{e''}, P'=e'$(P), và $P''=e''(P)$. Khi đó P là tổng trực tiếp của các môđun con $P'$ và $P''$, và ta có

$$
u(P') =u(e'(P)) =\varepsilon '(u(P)) =\varepsilon '(M) = M'
$$

đẳng thức $u(P'') = M''$ được chứng minh tương tự.

#### Hệ quả 2 {#alg-viii-s9-prop-7-cor-2 .statement tag=00AT}

Cho A là một vành, và cho $\mathfrak{a}$ là một iđêan hai phía lũy linh của A. Nếu P là một A-môđun xạ ảnh, thì $P/\mathfrak{a}P$ là một môđun xạ ảnh trên $A/\mathfrak{a}$, và A-môđun P không phân tích được khi và chỉ khi $A/\mathfrak{a}$-môđun $P/\mathfrak{a}P$ không phân tích được.

Cho P là một A-môđun xạ ảnh, và gọi $\overline{P}$ là $A/\mathfrak{a}$-môđun $P/\mathfrak{a}P$. A-môđun P là không khi và chỉ khi $\overline{P}$ là không (Định lý 2 của VIII, p. 158). Bây giờ giả sử $P\not= 0$. Vì $A/\mathfrak{a}$-môđun P đẳng cấu với $\overline{A}\otimes_AP$, nên nó là xạ ảnh (II, §5, No. 1, p. 279, Hệ quả của Mệnh đề 4). Nếu P không phân tích được, thì $\overline{P}$ cũng vậy theo Hệ quả 1. Ngược lại, giả sử rằng P phân tích được và khác không, và gọi $P'$ và $P''$ là hai môđun con khác không của P sao cho $P = P'\oplus P''$. Theo bổ đề Nakayama (VIII, p. 158, Định lý 2), ta có $P'+\mathfrak{a}P\not= P$ và $P''+\mathfrak{a}P\not= P$; nếu $\overline{P}'$ và $\overline{P}''$ là các ảnh chính tắc của $P'$ và $P''$ trong P, thì ta có $\overline{P}'\not= P,\overline{P}''\not= P$, và $\overline{P}=\overline{P}'\oplus \overline{P}''$. Điều đó chứng tỏ rằng $\overline{P}$ là phân tích được.

### 5. Bao xạ ảnh của một môđun

#### Định nghĩa 3 {#alg-viii-s9-def-3 .statement tag=00AU}

Cho A là một vành, và M là một A-môđun. Một bao xạ ảnh của M là một cặp $(P, u)$, trong đó P là một A-môđun xạ ảnh và $u$ là một đồng cấu toàn ánh từ P đến M sao cho ta có $u(P')\not= M$ với mọi A-môđun con thực sự $P'$ của P.

#### Nhận xét 1 {#alg-viii-s9-n5-rem-1 .statement tag=00AV}

Với mọi A-môđun xạ ảnh M, cặp $(M,1_M)$ là một bao xạ ảnh của M.

#### Nhận xét 2 {#alg-viii-s9-n5-rem-2 .statement tag=00AW}

Giả sử rằng $(P, u)$ là một bao xạ ảnh của A-môđun M. Cho $(x_i)_{i\in I}$ là một họ các phần tử của P, và gọi $P'$ là môđun con của P do họ đó sinh; khi đó $u(P')$ được sinh bởi họ $(u(x_i))_{i\in I}$. Do đó, họ $(x_i)_{i\in I}$ sinh A-môđun P khi và chỉ khi họ $(u(x_i))_{i\in I}$ sinh A-môđun M. Đặc biệt, P sinh hữu hạn khi và chỉ khi M sinh hữu hạn.

#### Mệnh đề 8 {#alg-viii-s9-prop-8 .statement tag=00AX}

Cho M và $M'$ là các A-môđun, $(P, u)$ và $(P', u')$ lần lượt là các bao xạ ảnh của M và $M'$, và $g: M\rightarrow M'$ là một ánh xạ A-tuyến tính.

a) Tồn tại một ánh xạ A-tuyến tính $f: P\rightarrow P'$ sao cho $u'\circ f=g\circ u$.

b) Cho $f$ là một ánh xạ như vậy. Nếu $g$ là toàn ánh (resp. song ánh), thì $f$ là toàn ánh (resp. song ánh). Nếu $g$ là đơn ánh và ảnh của nó là một nhân tử trực tiếp của $M'$, thì $f$ là đơn ánh và ảnh của nó là một nhân tử trực tiếp của $P'$.

Theo giả thiết, A-môđun P là xạ ảnh và ánh xạ $u'$ là toàn ánh. Do đó, tồn tại một ánh xạ A-tuyến tính $f: P\rightarrow P'$ sao cho $g\circ u=u'\circ f$ (II, §2, No. 2, p. 231, Mệnh đề 4). Mệnh đề a) được suy ra.

Cho $f$ là một ánh xạ như trong a). Giả sử rằng $g$ là toàn ánh. Vì $u$ là toàn ánh, ta có $M'=g(u(P)) =u'(f(P))$. Vì $(P', u')$ là một bao xạ ảnh của M’, nên ta có $f(P) = P'$, do đó $f$ là toàn ánh. Theo chỗ đã dẫn, hạt nhân của $f$ nhận một môđun con bổ sung $P_1$, nên $f(P_1) = P'$. Bây giờ giả sử rằng $g$ là song ánh. Ta có $g(u(P_1)) =u'(f(P_1)) =u'(P') = M'$, suy ra $u(P_1) = M$. Vì $(P, u)$ là một bao xạ ảnh của M, nên ta có $P_1= P$, do đó Ker($f$) $= 0$. Vậy $f$ là đơn ánh; vì ta đã biết rằng $f$ là toàn ánh, nên $f$ là song ánh.

Để kết luận, giả sử rằng $g$ là đơn ánh và ảnh của nó là một nhân tử trực tiếp của $M'$. Khi đó tồn tại một ánh xạ A-tuyến tính $g': M'\rightarrow M$ sao cho $g'\circ g= 1_M$. Theo a), tồn tại một ánh xạ A-tuyến tính $f': P'\rightarrow P$ sao cho $u\circ f'=g'\circ u'$. Ta có $u\circ (f'\circ f) =g'\circ u'\circ f= (g'\circ g)\circ u$; theo đoạn trước, ánh xạ $f'\circ f$ là song ánh. Ký hiệu song ánh đảo lại là $h$; ta có $(h\circ f')\circ f= 1_P$, nên $f$ là đơn ánh, và ảnh của nó là một nhân tử trực tiếp của $P'$ (II, §1, No. 9, p. 212, Hệ quả 2).

#### Hệ quả 1 {#alg-viii-s9-prop-8-cor-1 .statement tag=00AY}

Cho M là một A-môđun. Cho $(P, u)$ và $(P', u')$ là các bao xạ ảnh của M. Tồn tại một đẳng cấu $f$ từ P lên $P'$ sao cho $u=u'\circ f$.

Chú ý rằng $f$ không nhất thiết được xác định duy nhất bởi quan hệ $u=u'\circ f$ (VIII, p. 170, Bài tập 21).

#### Hệ quả 2 {#alg-viii-s9-prop-8-cor-2 .statement tag=00AZ}

Cho $(P, u)$ là một bao xạ ảnh của A-môđun M. Nếu Q là một A-môđun xạ ảnh và $g: Q\rightarrow M$ là một ánh xạ tuyến tính toàn ánh, thì tồn tại một ánh xạ tuyến tính toàn ánh $f: Q\rightarrow P$ sao cho $g=u\circ f$.

#### Mệnh đề 9 {#alg-viii-s9-prop-9 .statement tag=00B0}

Cho M là một A-môđun và $(P, u)$ là một bao xạ ảnh của M. Ký hiệu căn của vành A là $\mathfrak{r}$. Đồng cấu $\overline{u}: P/\mathfrak{r}P\rightarrow M/\mathfrak{r}M$ suy ra từ $u$ bằng cách chuyển qua các thương là một đẳng cấu.

Đồng cấu $u$ là toàn ánh theo định nghĩa, nên $\overline{u}$ là toàn ánh. Ký hiệu hạt nhân của $u$ là N. Ta có $u^{-1}(\mathfrak{r}M) = N +\mathfrak{r}P$. Hãy chứng minh rằng ta có $N\subset \mathfrak{r}P$, điều này suy ra tính đơn ánh của $\overline{u}$. Với mọi môđun con cực đại $P'$ của P, ta có $u(P')\not= M$, do đó $P'+ N\not= P$; vì $P'$ là cực đại, ta có $N\subset P'$. Vậy môđun con N của P được chứa trong căn của P. Mà căn này bằng $\mathfrak{r}P$ theo Mệnh đề 6 của VIII, p. 158.

#### Hệ quả {#alg-viii-s9-n5-cor-1 .statement tag=00B1}

Nếu một A-môđun M có một phủ xạ ảnh, thì $A/\mathfrak{r}$-môđun $M/\mathfrak{r}M$ là xạ ảnh.

Thật vậy, nếu $(P, u)$ là một bao xạ ảnh của M, thì $(A/\mathfrak{r}$)-môđun $M/\mathfrak{r}M$ đẳng cấu với $P/\mathfrak{r}P$ (Mệnh đề 9). Vì A-môđun P là xạ ảnh, nên $(A/\mathfrak{r}$)-môđun $P/\mathfrak{r}P$ cũng xạ ảnh.

#### Nhận xét 3 {#alg-viii-s9-n5-rem-3 .statement tag=00B2}

Giả sử vành A không có căn. Theo Mệnh đề 9, $(P, u)$ là một bao xạ ảnh của một A-môđun M khi và chỉ khi $u$ là một đẳng cấu. Do đó, các bao xạ ảnh chỉ có thể tồn tại đối với các A-môđun xạ ảnh.

Vành $\mathbf{Z}$ không có căn (VIII, p. 154, Ví dụ 3). Cho $n\geqslant 2$ là một số nguyên. $\mathbf{Z}$-môđun $\mathbf{Z}/n\mathbf{Z}$ không xạ ảnh và vì thế không thừa nhận một bao xạ ảnh.

#### Nhận xét 4 {#alg-viii-s9-n5-rem-4 .statement tag=00B3}

Giả sử mọi A-môđun hữu hạn sinh đều có một bao xạ ảnh; khi đó thương $A'$ của A theo căn của nó là nửa đơn. Thật vậy, mọi môđun hữu hạn sinh trên vành $A'$ đều xạ ảnh theo hệ quả. Đặc biệt, với mọi iđêan trái $\mathfrak{a}$ của $A'$, $A'$-môđun $A'_s/\mathfrak{a}$ là xạ ảnh. Khi đó mệnh đề của chúng ta suy ra từ Mệnh đề 4 của VIII, p. 138.

Ta có thể cho các ví dụ về một vành giao hoán A mà đối với nó $A/\mathfrak{r}$ là nửa đơn và về một A-môđun hữu hạn sinh M không có bao xạ ảnh (VIII, p. 170, Bài tập 22).

#### Mệnh đề 10 {#alg-viii-s9-prop-10 .statement tag=00B4}

Cho M là một A-môđun, P là một A-môđun xạ ảnh, và $u: P\rightarrow M$ là một ánh xạ tuyến tính. Cho $\mathfrak{a}$ là một iđêan hai phía của A. Giả sử ánh xạ tuyến tính $\overline{u}: P/\mathfrak{a}P\rightarrow M/\mathfrak{a}M$ suy ra từ $u$ bằng cách chuyển qua các thương là song ánh và một trong các điều kiện sau được thỏa mãn:

(i) Các A-môđun M và P là hữu hạn sinh, và $\mathfrak{a}$ được chứa trong căn của A.

(ii) Iđêan $\mathfrak{a}$ là lũy linh.

Khi đó $(P, u)$ là một bao xạ ảnh của M.

Dưới các giả thiết ấy, đồng cấu $u$ là toàn ánh (VIII, p. 159, Hệ quả 2) và hạt nhân N của nó được chứa trong $\mathfrak{a}P$. Cho $P'$ là một môđun con thực sự của P. Theo Bổ đề Nakayama (VIII, p. 158, Định lý 2), ta có $P'+\mathfrak{a}P\not= P$ và do đó $u(P')\not= M$. Vậy $(P, u)$ là một bao xạ ảnh của M.

#### Hệ quả 1 {#alg-viii-s9-prop-10-cor-1 .statement tag=00B5}

Cho P là một A-môđun xạ ảnh. Giả sử rằng P sinh hữu hạn hoặc căn $\mathfrak{r}$ của A là một iđêan hai phía lũy linh. Ký hiệu ánh xạ chính tắc từ P đến $P/\mathfrak{r}P$ là $u$. Khi đó $(P, u)$ là một bao xạ ảnh của $P/\mathfrak{r}P$.

#### Hệ quả 2 {#alg-viii-s9-prop-10-cor-2 .statement tag=00B6}

Cho $\mathfrak{a}$ là một iđêan hai phía của A và M là một A-môđun sao cho $(A/\mathfrak{a})$-môđun $M/\mathfrak{a}M$ là tự do. Giả sử rằng một trong các điều kiện sau được thỏa mãn:

(i) Môđun M sinh hữu hạn, và $\mathfrak{a}$ được chứa trong căn của A.

(ii) Iđêan $\mathfrak{a}$ là lũy linh.

Khi đó M có một bao xạ ảnh.

Chính xác hơn, cho P là một A-môđun tự do, $(e_i)_{i\in I}$ là một cơ sở của P, và cho $u: P\rightarrow M$ là một đồng cấu sao cho các ảnh chính tắc của các phần tử $u(e_i)$ của $M/\mathfrak{a}M$ tạo thành một cơ sở của $(A/\mathfrak{a})$-môđun $M/\mathfrak{a}M$. Khi đó $(P, u)$ là một bao xạ ảnh của M.

$(A/\mathfrak{a}$)-môđun $P/\mathfrak{a}P$ là tự do, và đồng cấu $\overline{u}$ từ $P/\mathfrak{a}P$ đến $M/\mathfrak{a}M$ suy ra từ $u$ bằng cách chuyển qua các thương biến đổi một cơ sở của $P/\mathfrak{a}P$ thành một cơ sở của $M/\mathfrak{a}M$, do đó là song ánh.

Nếu $\mathfrak{a}$ là lũy linh, thì chỉ cần áp dụng Mệnh đề 10. Bây giờ giả sử rằng vành A khác không và rằng môđun M là môđun hữu hạn sinh; khi đó $(A/\mathfrak{a}$)-môđun $M/\mathfrak{a}M$ cũng vậy, và do đó $(A/\mathfrak{a}$)-môđun $P/\mathfrak{a}P$ cũng vậy. Khi đó mọi cơ sở của $P/\mathfrak{a}P$ đều hữu hạn. Suy ra tập hợp I là hữu hạn và A-môđun P là môđun hữu hạn sinh. Khi đó ta lại áp dụng Mệnh đề 10.

#### Hệ quả 3 {#alg-viii-s9-prop-10-cor-3 .statement tag=00B7}

Mọi môđun hữu hạn sinh trên một vành địa phương đều có một bao xạ ảnh.

Cho A là một vành địa phương và $\mathfrak{r}$ là căn của nó. Đó là một iđêan hai phía của A (VIII, p. 155, Mệnh đề 5, a)), và vành $A/\mathfrak{r}$ là một trường (VIII, p. 157, Hệ quả 4). Nếu M là một A-môđun, thì $M/\mathfrak{r}M$ là một không gian vectơ trên trường $A/\mathfrak{r}$, do đó là một $(A/\mathfrak{r}$)-môđun tự do. Khi đó chỉ cần áp dụng Hệ quả 2.

#### Nhận xét 5 {#alg-viii-s9-n5-rem-5 .statement tag=00B8}

Cho A là một vành địa phương và $\mathfrak{r}$ là căn của nó. Cho M là một A-môđun hữu hạn sinh, P là một A-môđun xạ ảnh sinh hữu hạn, và $u: P\rightarrow$ M là một đồng cấu. Theo Hệ quả 6 của VIII, p. 36, A-môđun P là tự do. Chọn một cơ sở $(e_i)_{i\in I}$ của P. Đặt $x_i=u(e_i)$, và ký hiệu ảnh chính tắc của $x_i$ trong $M/\mathfrak{r}M$ bởi $\overline{x}_i$. Các tính chất sau là tương đương:

(i) Cặp $(P, u)$ là một bao phủ xạ ảnh của M.

(ii) Họ $(x_i)_{i\in I}$ là một họ sinh cực tiểu của A-môđun M.

(iii) Họ $(\overline{x}_i)_{i\in I}$ là một cơ sở của không gian vectơ $M/\mathfrak{r}M$ trên trường $A/\mathfrak{r}$.

Ta có (i) $\Rightarrow$ (ii) theo Nhận xét 2 của VIII, p. 161 và (iii) $\Rightarrow$ (i) theo Hệ quả 2. Hơn nữa, nếu họ $(x_i)$ là một họ sinh cực tiểu của A-môđun M, thì họ $(\overline{x}_i)$ là một họ sinh cực tiểu, tức là một cơ sở, của không gian vectơ $M/\mathfrak{r}M$ trên $A/\mathfrak{r}$ (VIII, p. 158, Hệ quả 1).

#### Mệnh đề 11 {#alg-viii-s9-prop-11 .statement tag=00B9}

Cho A là một vành và $\mathfrak{a}$ là một iđêan hai phía lũy linh của A. Cho M là một $A/\mathfrak{a}$-môđun xạ ảnh. Tồn tại một A-môđun xạ ảnh P và một ánh xạ A-tuyến tính toàn ánh $u: P\rightarrow M$ có hạt nhân là $\mathfrak{a}P$.

Một cặp như vậy $(P, u)$ là một bao xạ ảnh của M được xem như một A-môđun.

Tồn tại một $A/\mathfrak{a}$-môđun $M'$ sao cho $M\oplus M'$ là một $A/\mathfrak{a}$-môđun tự do. Chọn một A-môđun tự do L và một ánh xạ A-tuyến tính toàn ánh $v: L\rightarrow M\oplus M'$ có hạt nhân là $\mathfrak{a}L$. Theo Hệ quả 1 của Mệnh đề 7 (VIII, p. 159), tồn tại một phân tích thành tổng trực tiếp $L = P\oplus P'$ sao cho $v(P) = M$ và $v(P') = M'$. A-môđun P là xạ ảnh, và ánh xạ A-tuyến tính $u$ từ P đến M trùng với $v$ trên P là toàn ánh, có hạt nhân là $\mathfrak{a}P$. Mệnh đề thứ nhất được suy ra.

Cho P là một A-môđun xạ ảnh và $u$ là một đồng cấu từ P đến M có hạt nhân là $\mathfrak{a}P$. Theo Mệnh đề 10, cặp $(P, u)$ là một phủ xạ ảnh của M.

#### Hệ quả {#alg-viii-s9-n5-cor-2 .statement tag=00RA}

Cho P và $P'$ là các A-môđun xạ ảnh. Nếu các môđun $P/\mathfrak{a}P$ và $P'/\mathfrak{a}P'$ là đẳng cấu, thì P và $P'$ là đẳng cấu.

Vì $P/\mathfrak{a}P$ và $P'/\mathfrak{a}P'$ là xạ ảnh, hệ quả suy ra từ Mệnh đề 11 và tính duy nhất của bao xạ ảnh (VIII, p. 162, Hệ quả 1).

### Bài tập {#alg-viii-s9-exercises}

Xem [bài tập của § 9](exercises/s9/).
