---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 5
section_title: Algèbres de Banach commutatives régulières
lang: vi
source: ts-i-ii-fr
book_pages: TS I.88-TS I.95, TS I.178-TS I.180
pdf_pages: 0101-0108, 0191-0193
extraction: native
subsections:
    - "no": 1
      title: Définition
      page: 88
      pdf_page: 101
    - "no": 2
      title: Synthèse harmonique
      page: 91
      pdf_page: 104
statements: 16
exercises: 7
content_sha256: 41f8f9c82690f4d91b1e04d2812fb2dc90299e723f41db081f71a90b74acbf2b
translated_from: content/en-mt/ts/I/05_s5_algebres_de_banach_commutatives.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 8dd593cbb4218fac0351469777486cdf7a8f4d3e8dc8f530061b40e9ef71c147
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-746f338b
glossary_version: 34
glossary_terms_sha256: e0140bae785a57b3067923015fc6db86758ed3f95b9971419f7e58ed74e08ff5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC ĐẠI SỐ BANACH GIAO HOÁN CHÍNH QUY

Trong tiết diện này, trường cơ sở là $\mathbf{C}$.

### 1. Định nghĩa

#### Mệnh đề 1 {#ts-i-s5-prop-1 .statement tag=02BV}

Cho A là một đại số Banach giao hoán. Các điều kiện sau là tương đương:

(i) Tôpô yếu và tôpô Jacobson trên $\mathsf{X}(A)$ trùng nhau ;

(ii) Với mọi $\chi \in \mathsf{X}(A)$ và mọi tập con F đóng yếu của $\mathsf{X}(A)$ sao cho $\chi \notin F$, tồn tại một $x\in A$ sao cho $\mathscr{G}(x)$ bằng 1 tại $\chi$ và bằng 0 trên F;

(iii) Với mọi tập con K compact yếu và mọi tập con F đóng yếu của $\mathsf{X}(A)$ sao cho $K\cap F =\emptyset$, tồn tại một phần tử $x\in A$ sao cho $\mathscr{G}(x)$ bằng 1 trên K và bằng 0 trên F.

Cho $M\subset \mathsf{X}(A)$. Nói rằng M đóng đối với tôpô Jacobson có nghĩa là, với mọi $\chi \in \mathsf{X}(A)$ - M, tồn tại một $x\in A$ sao cho $\mathscr{G}(x)$ triệt tiêu trên M nhưng không triệt tiêu tại $\chi$ (bổ đề 2 của I, p. 39). Do đó, điều kiện (ii) có nghĩa là mọi tập con đóng yếu của $\mathsf{X}(A)$ đều đóng đối với tôpô Jacobson, từ đó suy ra (ii) $=\Rightarrow$ (i). Hơn nữa (iii) $=\Rightarrow$ (ii) vì tập con $\{\chi \}$ là compact yếu trong $\mathsf{X}(A)$. Cuối cùng (i) $=\Rightarrow$ (iii) theo hệ quả của mệnh đề 15 của I, p. 81.

#### Định nghĩa 1 {#ts-i-s5-def-1 .statement tag=02BW}

Cho A là một đại số Banach giao hoán. Ta nói A là chính quy nếu nó thỏa mãn các điều kiện tương đương của Mệnh đề 1.

#### Nhận xét {#ts-i-s5-n1-rem-1 .statement tag=02BX}

Cho $\widetilde{A}$ là đại số Banach suy ra từ A bằng phép nối một phần tử đơn vị $e$. Điều kiện (ii) của mệnh đề 1 cho thấy nếu $\widetilde{A}$ là chính quy thì A là chính quy. Giả sử A là chính quy và hãy chứng minh rằng $\widetilde{A}$ là chính quy. Xét các tập con F và $F'$ của $\mathsf{X}(\widetilde{A})$ rời nhau và đóng yếu (do đó compact yếu), và xây dựng một $x\in \widetilde{A}$ sao cho $\mathscr{G}(x)$ triệt tiêu trên F và bằng 1 trên $F'$. Gọi $\chi_0\in \mathsf{X}(\widetilde{A})$ là đặc trưng bằng không trên A. Nếu $\chi_0\notin F'$, theo điều kiện (iii) của mệnh đề 1 và giả thiết về A, tồn tại một phần tử $x\in A$ sao cho $\mathscr{G}(x)$ triệt tiêu trên F và bằng 1 trên $F'$. Nếu $\chi_0\in F'$, ta có $\chi_0\notin F$; do đó tồn tại một phần tử $y\in A$ sao cho $\mathscr{G}(y)$ triệt tiêu trên $F'$ và bằng 1 trên F. Khi đó phần tử $x=e-y$ của $\widetilde{A}$ có tính chất cần có.

#### Ví dụ {#ts-i-s5-n1-exa-1 .statement tag=02BY}

Ta xét lại các ví dụ của n$^o2$ trong I, p. 17.

Đại số các hàm liên tục với giá trị phức tiến tới 0 ở vô cực trên một không gian địa phương compact X (ví dụ 3 của I, p. 17) là chính quy (xem I, p. 36, ví dụ 1).

Đại số các hàm khả vi $n$ lần trên $[0,1]$ (ví dụ 4 của I, p. 18) là chính quy (xem I, p. 36, ví dụ 2).

Nếu G là một nhóm địa phương compact giao hoán và $\mu$ là một độ đo Haar trên G, thì đại số $L^1(G, \mu)$ (ví dụ 7 của I, p. 19) là chính quy (xem II, p. 219, hệ quả 2).

Đại số các hàm liên tục trong đĩa $|z|\leqslant 1$ và giải tích trong phần trong (ví dụ 9 của I, p. 20) không chính quy (xem I, p. 193, bài tập 6).

#### Mệnh đề 2 {#ts-i-s5-prop-2 .statement tag=02BZ}

Cho A là một đại số Banach giao hoán chính quy có đơn vị. Cho $n\geqslant 1$ là một số nguyên và $(U_1, . . . ,U_n)$ là một phủ mở của $\mathsf{X}(A)$. Tồn tại các phần tử $x_1, . . . , x_n$ của A có tổng bằng 1 sao cho Supp($\mathscr{G}(x_i)$)$\subset U_i$ với $i= 1, . . . ,n$.

Hãy chứng minh mệnh đề bằng quy nạp theo $n$. Mệnh đề đúng nếu $n= 1$. Giả sử rằng $n\geqslant 2$ và mệnh đề đã được thiết lập với $n-1$.

Tồn tại một phủ mở $(V_1, . . . ,V_n)$ của $\mathsf{X}(A)$ sao cho $\overline{V}_i\subset$ $U_i$ với mọi $i$. Theo giả thiết quy nạp, tồn tại các phần tử $x, x_3, . . . , x_n\in A$ sao cho $x+x_3+\cdots +x_n= 1$ và Supp($\mathscr{G}(x)$)$\subset V_1\cup V_2$, Supp($\mathscr{G}(x_i)$)$\subset V_i$ với $i\geqslant 3$. Đặt K = Supp($\mathscr{G}(x)$)$\subset V_1\cup V_2$. Gọi $K_1$ (tương ứng $K_2$) là tập hợp các phần tử của K không thuộc $V_1$ (tương ứng $V_2$). Khi đó $K_1$ và $K_2$ là các tập con compact rời nhau của K. Vì đại số Banach A là chính quy, do đó tồn tại $y\in A$ sao cho $\mathscr{G}(y) = 1$ trên $K_1$ và $\mathscr{G}(y) = 0$ trên $K_2$. Khi đó $\mathscr{G}(xy)$ bằng không trên $\mathsf{X}(A)-K$ và trên $K_2$, do đó Supp $\mathscr{G}(xy)\subset \overline{V}_2\subset U_2$. Tương tự, $\mathscr{G}(x(1-y))$ bằng không trên $\mathsf{X}(A)$ - K và trên $K_1$, do đó Supp $\mathscr{G}(x(1-y))\subset \overline{V}_1\subset U_1$. Các phần tử $x_1=x(1-y),x_2=xy$, và $x_3, . . . ,x_n$ khi đó thỏa mãn các tính chất của mệnh đề.

#### Hệ quả 1 {#ts-i-s5-prop-2-cor-1 .statement tag=02C0}

Cho A là một đại số Banach giao hoán chính quy có đơn vị, I là một iđêan của A và $f:\mathsf{X}(A)\rightarrow \mathbf{C}$ là một hàm liên tục. Giả sử rằng, với mọi $\chi \in \mathsf{X}(A)$, tồn tại một phần tử $y_{\chi}\in I$ sao cho $f=\mathscr{G}(y_{\chi})$ trong một lân cận của $\chi$. Khi đó tồn tại một phần tử $y\in I$ sao cho $f=\mathscr{G}(y)$.

Vì $\mathsf{X}(A)$ là compact, tồn tại một phủ mở hữu hạn $(U_1, . . . ,U_n)$ của $\mathsf{X}(A)$, và các phần tử $y_1, . . . , y_n$ của I sao cho $f=\mathscr{G}(y_i)$ trên $U_i$. Theo mệnh đề 2, tồn tại các phần tử $x_1, . . . , x_n$ của A có tổng bằng 1 sao cho Supp($\mathscr{G}(x_i)$)$\subset U_i$ với mọi $i$. Đặt $y=x_1y_1+\cdots +$ $x_ny_n$. Đây là một phần tử của I có tính chất cần có. Thật vậy, lấy $\chi \in \mathsf{X}(A)$. Với $1\leqslant i\leqslant n$, ta có $\mathscr{G}(x_i)(\chi )\mathscr{G}(y_i)(\chi ) =\mathscr{G}(x_i)(\chi )f(\chi )$ vì $\mathscr{G}(y_i)(\chi ) =f(\chi )$ nếu $\chi \in U_i$, và $\mathscr{G}(x_i)(\chi ) = 0$ nếu $\chi  \notin U_i$. Do đó

$$
\mathscr{G}(y)(\chi ) =\sum_{i=1}^n\mathscr{G}(x_i)(\chi )\mathscr{G}(y_i)(\chi ) =f(\chi )\sum_{i=1}^n\mathscr{G}(x_i)(\chi ) =f(\chi )
$$

#### Hệ quả 2 {#ts-i-s5-prop-2-cor-2 .statement tag=02C1}

Cho A là một đại số Banach giao hoán chính quy, I một iđêan của A và $f:\mathsf{X}'(A)\rightarrow \mathbf{C}$ một hàm liên tục. Giả sử rằng, với mọi $\chi \in \mathsf{X}'(A)$, tồn tại một phần tử $y_{\chi}\in I$ sao cho $f=\mathscr{G}'(y_{\chi})$ trong một lân cận của $\chi$. Khi đó tồn tại một phần tử $y\in I$ sao cho $f=\mathscr{G}'(y)$.

Gọi $\widetilde{A}$ là đại số Banach thu được từ A bằng phép nối một phần tử đơn vị. Khi đó $\widetilde{A}$ là chính quy (nhận xét 1), và $\mathsf{X}'(A) =\mathsf{X}(\widetilde{A})$; do đó chỉ cần áp dụng hệ quả 1 cho $\widetilde{A}$ và iđêan I.

Nếu I là một iđêan của một đại số Banach giao hoán, hãy nhắc lại rằng (xem I, p. 30) ta ký hiệu V(I) là tập hợp các $\chi \in \mathsf{X}(A)$ mà hạt nhân chứa I, nói cách khác là tập hợp các $\chi \in \mathsf{X}(A)$ tại đó mọi hàm $\mathscr{G}(x)$ đều triệt tiêu với $x\in I$. Nó là một tập con đóng của $\mathsf{X}(A)$ đối với tôpô Jacobson.

#### Mệnh đề 3 {#ts-i-s5-prop-3 .statement tag=02C2}

Cho A là một đại số Banach giao hoán chính quy, I một iđêan của A và K một tập con compact của $\mathsf{X}(A)$ rời nhau với V(I). Tồn tại một phần tử $x\in I$ sao cho $\mathscr{G}(x) = 1$ với mọi $x$ trong K.

Đây là một trường hợp đặc biệt của mệnh đề 15 của I, p. 81, có tính đến sự kiện rằng tôpô Jacobson trùng với tôpô yếu trên $\mathsf{X}(A)$.

### 2. Tổng hợp điều hòa

Cho A là một đại số Banach giao hoán. Nhắc lại rằng nếu M là một tập con của $\mathsf{X}(A)$, ta ký hiệu Υ(M) là giao của các hạt nhân của các phần tử của M (xem I, p. 30); nó là một iđêan của A.

#### Mệnh đề 4 {#ts-i-s5-prop-4 .statement tag=02C3}

Cho A là một đại số Banach giao hoán chính quy không có căn. Cho F là một tập con đóng của $\mathsf{X}(A)$. Tập hợp các iđêan I của A sao cho V(I) = F, có thứ tự theo quan hệ bao hàm, có một phần tử lớn nhất, đó là Υ(F), và một phần tử nhỏ nhất, đó là tập hợp J gồm các $x\in A$ sao cho $\mathscr{G}(x)$ có giá compact rời nhau với F.

Theo phép dựng, Υ(F) là một iđêan của A sao cho V(Υ(F)) chứa F, và nó là iđêan lớn nhất của A có tính chất này. Vì F đóng, tồn tại một iđêan I của A sao cho V(I) = F; do đó $I\subset \Upsilon (F)$, do đó $V(\Upsilon (F))\subset V(I) = F$, suy ra V(Υ(F)) = F. Điều này chứng minh mệnh đề đầu tiên.

Tập hợp J là một iđêan của A và V(J) chứa F. Ta hãy chứng minh rằng V(J) = F. Lấy $\chi \in \mathsf{X}(A)$ không thuộc F. Gọi U là một lân cận compact của $\chi$ không gặp F (TG, I, p. 65, hệ quả của mệnh đề 9). Theo mệnh đề (ii) của mệnh đề 1 của I, p. 88, tồn tại $x\in A$ sao cho $\mathscr{G}(x)$ bằng 1 tại $\chi$ và bằng 0 bên ngoài U. Khi đó $x\in J$ và do đó $\chi \notin V(J)$. Điều này cho thấy $V(J)\subset F$ và do đó V(J) = F.

Cuối cùng, cho I là một iđêan của A sao cho V(I) = F. Ta hãy chứng minh rằng $J\subset I$. Cho $x\in J$ và C là giá của $\mathscr{G}(x)$; tập con C là một tập con compact của $\mathsf{X}(A)$ rời nhau với F. Theo Mệnh đề 3, tồn tại một phần tử $u\in I$ sao cho $\mathscr{G}(u) = 1$ trên C. Khi đó ta có $\mathscr{G}(x) =\mathscr{G}(ux)$, và do đó $x=ux$ vì A không có căn (Mệnh đề 8 của I, p. 38). Do đó, ta có $x\in I$, điều này chứng tỏ rằng $J\subset I$.

#### Hệ quả 1 {#ts-i-s5-prop-4-cor-1 .statement tag=02C4}

Cho A là một đại số Banach giao hoán chính quy không có căn. Cho J là tập hợp các $x\in A$ sao cho $\mathscr{G}(x)$ có giá compact. Giả sử rằng J = A. Khi đó mọi iđêan đóng của A phân biệt với A đều được chứa trong một iđêan cực đại chính quy.

Nếu I là một iđêan đóng của A không được chứa trong bất kỳ iđêan cực đại chính quy nào, thì $V(I) =\emptyset$, do đó $I\supset J$ (Mệnh đề 4 áp dụng cho F = $\emptyset$ ), do đó $I\supset \overline{J}= A$.

#### Hệ quả 2 {#ts-i-s5-prop-4-cor-2 .statement tag=02C5}

Cho A là một đại số Banach giao hoán chính quy không có căn. Cho $x, y\in A$. Nếu giá của $\mathscr{G}(x)$ là compact và được chứa trong tập hợp các đặc trưng $\chi$ sao cho $\mathscr{G}(y)(\chi )\not= 0$, thì $x$ là một bội của $y$ trong A.

Cho I là iđêan $Ay$ của A. Khi đó V(I) là tập hợp các không điểm của $\mathscr{G}(y)$. Vì giá F của $\mathscr{G}(x)$ là compact và rời nhau với V(I), ta có $x\in I$ (Mệnh đề 4 áp dụng cho F).

#### Định nghĩa 2 {#ts-i-s5-def-2 .statement tag=02C6}

Cho A là một đại số Banach giao hoán.

Cho I là một iđêan của A$,x\in A$, và $\chi \in \mathsf{X}'(A)$. Ta nói rằng x thuộc I trong một lân cận của $\chi$ nếu tồn tại một phần tử $y\in I$ sao cho $\mathscr{G}'(y)$ và $\mathscr{G}'(x)$ trùng nhau trong một lân cận của $\chi$.

Ta nói rằng A thỏa mãn điều kiện Ditkin nếu, với mọi $\chi \in \mathsf{X}'(A)$ và mọi $x\in A$ sao cho $\mathscr{G}'(x)$ triệt tiêu tại $\chi$, tồn tại một dãy $(x_n)$ trong A sao cho $x=$ lim$_{n\rightarrow \infty}x_nx$ và sao cho mỗi $\mathscr{G}'(x_n)$ triệt tiêu trong một lân cận $V_n$ của $\chi$.

#### Nhận xét {#ts-i-s5-n2-rem-1 .statement tag=02C7}

Cho A là một đại số Banach giao hoán.

1) Nếu $\chi$ sao cho $\mathscr{G}'(x)$ triệt tiêu trong một lân cận của $\chi$, thì x thuộc I trong một lân cận của $\chi$.

2) Nếu x thuộc I trong một lân cận của $\chi$ và $y\in A$ là một phần tử tùy ý, thì xy thuộc I trong một lân cận của $\chi$.

3) Tập hợp các $\chi$ sao cho x thuộc I trong một lân cận của $\chi$ là mở trong $\mathsf{X}'(A)$.

4) Giả sử rằng A là chính quy và không có căn. Nếu $x$ thuộc I trong một lân cận của $\chi$ với mọi $\chi \in \mathsf{X}'(A)$, thì $x$ thuộc I (Hệ quả 2 của I, p. 91 áp dụng cho hàm $f=\mathscr{G}'(x)$ và Mệnh đề 8 của I, p. 38).

5) Giả sử rằng A là chính quy. Cho I là một iđêan của A và $\chi$ là một phần tử của $\mathsf{X}(A)$ sao cho $\chi \notin V(I)$. Khi đó mọi phần tử $x$ của A đều thuộc I trong một lân cận của $\chi$. Thật vậy, theo Định nghĩa 1 của I, p. 89, tồn tại một $z\in A$ sao cho $\mathscr{G}'(z)$ bằng 1 trong một lân cận của $\chi$, và bằng 0 trong một lân cận của V(I). Giá của $\mathscr{G}(z)$ là compact và do đó $z\in I$ (Mệnh đề 4 áp dụng cho V(I)), suy ra $xz\in I$, và $\mathscr{G}'(xz) =\mathscr{G}'(x)$ trong một lân cận của $\chi$.

Nhắc lại rằng một không gian con K của một không gian tôpô X được gọi là hoàn hảo nếu nó đóng và không có điểm cô lập (TG, I, p. 8).

#### Bổ đề 1 {#ts-i-s5-lem-1 .statement tag=02C8}

Cho A là một đại số Banach giao hoán chính quy không có căn, thỏa mãn điều kiện Ditkin. Cho I là một iđêan đóng của A và $x$ là một phần tử của Υ(V(I)). Gọi K là tập hợp các $\chi \in \mathsf{X}'(A)$ sao cho $x$ không thuộc I trong một lân cận của $\chi$. Khi đó tập hợp K là một tập con hoàn hảo của $\mathsf{X}'(A)$.

Gọi G là phần bù của K trong $\mathsf{X}'(A)$. Tập hợp G là mở trong $\mathsf{X}'(A)$ (Nhận xét 3), do đó K là đóng.

Ta tiến hành bằng phản chứng, và giả sử rằng K có một điểm cô lập $\chi_0$. Gọi U là một lân cận của $\chi_0$ sao cho U $-\{\chi_0\} \subset G$. Vì $x$ không thuộc I trong một lân cận của $\chi_0$, Nhận xét 5 cho thấy rằng $\chi_0\in V(I)$. Đặc biệt, ta có $\chi_0(x) = 0$ vì $x\in \Upsilon (V(I))$.

Ta sẽ chứng minh rằng tồn tại một phần tử $y$ của A thuộc I trong một lân cận của mọi điểm của $\mathsf{X}'(A)-\{\chi_0\}$, không thuộc I trong một lân cận của $\chi_0$, và sao cho $\chi_0(y) = 0$.

Trước hết, giả sử rằng sự tồn tại của một phần tử $y$ như vậy đã được chứng minh. Vì A thỏa mãn điều kiện Ditkin, khi đó tồn tại một dãy $(x_n)$ trong A sao cho $x_ny$ hội tụ đến $y$ và sao cho mỗi $\mathscr{G}'(x_n)$ triệt tiêu trong một lân cận của $\chi_0$. Với mọi $n$, khi đó phần tử $x_ny$ thuộc I trong một lân cận của mọi điểm của $\mathsf{X}'(A)$ (Các Nhận xét 1 và 2) và do đó $x_ny\in I$ (Nhận xét 4). Vì I là đóng, suy ra rằng $y\in I$, điều này mâu thuẫn với việc $y$ không thuộc I trong một lân cận của $\chi_0$.

Vẫn còn phải chứng minh sự tồn tại của $y$. Nếu $\chi_0\not= 0$, theo mệnh đề (iii) của Mệnh đề 1 của I, p. 88, tồn tại một $u\in A$ sao cho $\mathscr{G}'(u)$ bằng 1 trong một lân cận của $\chi_0$ và bằng 0 trong một lân cận của $\mathsf{X}'(A)$ - U. Đặt $y=ux$. Vì $x$ thuộc I trong một lân cận của $\chi$ với mọi $\chi \in U-\{\chi_0\}$, điều tương tự cũng đúng đối với $y$. Hơn nữa, nếu $\chi \in \mathsf{X}'(A)$ - U, thì $\mathscr{G}'(y)$ triệt tiêu trong một lân cận của $\chi$. Do đó (Nhận xét 5) phần tử $y=ux$ thuộc I trong một lân cận của mọi $\chi \not=\chi_0$. Vì $\mathscr{G}'(y)$ trùng với $\mathscr{G}'(x)$ trong một lân cận của $\chi_0$, sự kiện $\chi_0$ thuộc K kéo theo rằng $y$ không thuộc I trong một lân cận của $\chi_0$. Cuối cùng, ta có $\chi_0(y) =\chi_0(u)\chi_0(x) = 0$.

Nếu $\chi_0= 0$, tương tự tồn tại một phần tử $v\in A$ sao cho $\mathscr{G}'(v)$ bằng không trong một lân cận của $\chi_0$ và bằng 1 trong một lân cận của $\mathsf{X}'(A)$- U; như trên, ta suy ra rằng phần tử $y=x-vx$ thuộc I trong một lân cận của mọi $\chi \not=\chi_0$, rằng nó không thuộc I trong một lân cận của $\chi_0$, và rằng $\chi_0(y) = 0$.

#### Bổ đề 2 {#ts-i-s5-lem-2 .statement tag=02C9}

Cho X là một không gian tôpô. Cho F và D là các không gian con rời nhau của X sao cho F là đóng và D rời rạc. Nếu F không chứa không gian con hoàn hảo khác rỗng nào, thì điều tương tự cũng đúng đối với $F\cup D$.

Thật vậy, giả sử rằng K là một không gian con hoàn hảo khác rỗng của $F\cup D$. Cho $x$ là một điểm của K. Nếu $x$ thuộc D, nó là cô lập trong D, do đó cũng cô lập trong $F\cup D$ vì F là đóng. Vì vậy $x$ là cô lập trong K, điều này mâu thuẫn với các giả thiết.

#### Mệnh đề 5 {#ts-i-s5-prop-5 .statement tag=02CA}

Cho A là một đại số Banach giao hoán chính quy không có căn, thỏa mãn điều kiện Ditkin. Cho I là một iđêan đóng của A sao cho biên F của V(I) không chứa tập hợp hoàn hảo khác rỗng nào. Khi đó I = Υ(V(I)), nghĩa là I là tập hợp các $x\in A$ sao cho $\mathscr{G}(x)$ triệt tiêu trên V(I). Đặc biệt, nếu V(I) thu gọn thành một điểm $\chi$, ta có I = Ker($\chi$ ).

Ta có $I\subset \Upsilon (V(I))$. Bây giờ cho $x\in \Upsilon (V(I))$. Gọi G là tập hợp các ký tự $\chi \in \mathsf{X}'(A)$ sao cho $x$ thuộc I trong một lân cận của $\chi$. Nó là mở và phần bù K của nó là hoàn hảo (Bổ đề 1). Vì $\mathscr{G}'(x)$ bằng không trên V(I), tập hợp G chứa phần trong của $V(I)\cup  \{0\}$ (Nhận xét 1). Nó cũng chứa $\mathsf{X}(A)$- V(I) theo Nhận xét 5. Do đó $K =\mathsf{X}'(A)$ - G được chứa trong biên $F_0$ của $V(I)\cup  \{0\}$. Ta có $F_0\subset F\cup  \{0\}$. Giả thiết do đó suy ra rằng $F_0$ không chứa tập hợp hoàn hảo khác rỗng nào (Bổ đề 2). Vì vậy từ Bổ đề 1 suy ra rằng tập hợp hoàn hảo K là rỗng. Do đó $x$ thuộc I trong một lân cận của mọi $\chi \in \mathsf{X}'(A)$, điều đó có nghĩa là $x\in I$ (Nhận xét 4). Như vậy $\Upsilon (V(I))\subset$ I, điều này kết thúc chứng minh.

## BÀI TẬP {#ts-i-s5-exercises}

Trong các bài tập dưới đây, tất cả các đại số được xét đều trên $\mathbf{C}$.

Xem các [bài tập cho § 5](exercises/s5/).
