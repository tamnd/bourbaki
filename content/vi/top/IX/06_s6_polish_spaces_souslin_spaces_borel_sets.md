---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 6
section_title: Polish spaces, Souslin spaces, Borel sets
lang: vi
source: top-v-x
pdf_pages: 0201-0216, 0264-0273
extraction: ocr
subsections:
    - "no": 1
      title: POLISH SPACES
      page: 0
      pdf_page: 201
    - "no": 2
      title: SOUSLIN SPACES
      page: 0
      pdf_page: 203
    - "no": 3
      title: BOREL SETS
      page: 0
      pdf_page: 205
    - "no": 4
      title: ZERO-DIMENSIONAL SPACES AND LUSIN SPACES
      page: 0
      pdf_page: 206
    - "no": 5
      title: SIEVES
      page: 0
      pdf_page: 208
    - "no": 6
      title: SEPARATION OF SOUSLIN SETS
      page: 0
      pdf_page: 210
    - "no": 7
      title: LUSIN SPACES AND BOREL SETS
      page: 0
      pdf_page: 211
    - "no": 8
      title: BOREL SECTIONS
      page: 0
      pdf_page: 212
    - "no": 9
      title: CAPACITABILITY OF SOUSLIN SETS
      page: 0
      pdf_page: 214
statements: 48
exercises: 1
content_sha256: c6619e27b695d63037d60790ef2c3010d9a7f6c6b9dc04eb3ce4c18a153b8488
translated_from: content/en/top/IX/06_s6_polish_spaces_souslin_spaces_borel_sets.md
source_content_sha256: e046d099601541d21ad34ac061ae4087de467970508dacf68d145d8e9e3c6f51
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-15a9d5c4
glossary_version: 34
glossary_terms_sha256: 66cc3074eb1ef5ab8adea9a83758ac0c92be8df5691ad0972d28670b85dd8afa
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 6. CÁC KHÔNG GIAN POLISH, CÁC KHÔNG GIAN SOUSLIN, CÁC TẬP BOREL

### 1. CÁC KHÔNG GIAN POLISH

#### Định nghĩa 1 {#top-ix-s6-def-1 .statement}

*Một không gian tôpô* $X$ *được gọi là Polish nếu nó mêtric hóa được kiểu đếm được* ($\S 2$, no. 8) *và nếu tồn tại một mêtric tương thích với tôpô của* $X$, *đối với mêtric đó* $X$ *là đầy đủ*.

#### Mệnh đề 1 {#top-ix-s6-prop-1 .statement}

a) *Mọi không gian con đóng của một không gian Polish đều là Polish*.
b) *Tích của một họ đếm được các không gian Polish là Polish*.
c) *Tổng của một họ đếm được các không gian Polish là Polish*.

Mọi không gian con của một không gian mêtric hóa được kiểu đếm được đều mêtric hóa được kiểu đếm được, và mọi không gian con đóng của một không gian đầy đủ đều đầy đủ; (Chương II, § 3, no. 4, Mệnh đề 8). Mọi tích đếm được của các không gian mêtric hóa được kiểu đếm được lại là mêtric hóa được kiểu đếm được: ($\S 2$, no. 8), và mọi tích đếm được của các không gian mêtric đầy đủ là một không gian mêtric đầy đủ đối với một mêtric tương thích với tôpô của nó (Chương II, § 3, no. 5, Mệnh đề 10 và Chương IX, § 2, no. 4, Định lý 1, Hệ quả 2). Cuối cùng, cho $(X_n)$ là một dãy các không gian Polish khác rỗng, và xét không gian tích $Y = \mathbf{N} \times \prod_n X_n$, trong đó $\mathbf{N}$ mang tôpô rời rạc; $Y$ là một không gian Polish theo những gì đã được chứng minh. Mặt khác, cho $a_n$ là một điểm của $X_n$ với mỗi $n$, và cho $f_n$ là ánh xạ từ $X_n$ vào $Y$ sao cho với mỗi $x \in X_n$ ta có

$$
f_n(x) = (n, (y_p)),
$$

trong đó $y_p = a_p$ nếu $p \neq n$ và $y_n = x$. Nếu $X$ là tổng tôpô của các $X_n$, hiển nhiên rằng ánh xạ $f$ từ $X$ vào $Y$ trùng với $f_n$ trên $X_n$ với mỗi $n$ là một đồng phôi của $X$ lên $f(X)$; ngoài ra, với mỗi $n$, $f_n(X_n)$ là đóng trong $Y$, và họ $(f_n(X_n))$ là hữu hạn địa phương vì $\mathbf{N}$ là rời rạc; do đó $f(X) = \bigcup_n f_n(X_n)$ là đóng trong $Y$ (Chương I, § 1, no. 5, Mệnh đề 4), và vì thế $f(X)$ là một không gian Polish, theo a).

#### Mệnh đề 2 {#top-ix-s6-prop-2 .statement}

Mọi không gian con mở của một không gian Polish đều là Polish.

Cho $X$ là một không gian Polish, cho $d$ là một mêtric trên $X$ tương thích với tôpô của nó, và cho $U \neq X$ là một tập con mở của $X$. Cho $V$ là tập con của $\mathbf{R} \times X$ gồm tất cả các điểm $(t, x)$ sao cho
$$
t \cdot d(x, X - U) = 1;
$$
$V$ là đóng theo Mệnh đề 3 của § 2, no. 2 và do đó là Polish (Mệnh đề 1). Vì hạn chế trên $V$ của phép chiếu $\mathrm{pr}_2 : \mathbf{R} \setminus X \to X$ là một đồng phôi của $V$ lên $U$ ($\S 2,$ no. 2, Mệnh đề 3), nên $U$ là một không gian con Polish của $X$.

#### Hệ quả {#top-ix-s6-n1-cor-1 .statement}

Mọi không gian mêtric hóa được địa phương compact $X$ đều là Polish.

Cho $X$ là không gian compact thu được bằng cách ghép thêm một điểm ở vô tận vào $X$; $X'$ là mêtric được và có kiểu đếm được ($\S 2,$ no. 9, Hệ quả của Mệnh đề 16), và $X$ là đầy đủ đối với tôpô đều duy nhất của nó (chương II, $\S 4,$ no. 1, Định lý 1). Do đó $X$ là một không gian Polish; vì $X$ là mở trong $X'$, suy ra $X$ là Polish.

#### Mệnh đề 3 {#top-ix-s6-prop-3 .statement}

Cho $X$ là một không gian tôpô Hausdorff. Khi đó giao của một dãy $(A_n)$ các không gian con Polish của $X$ là một không gian con Polish.

Cho $f$ là ánh xạ đường chéo của $X$ vào $X^\mathbf{N}$ ([Lý thuyết tập hợp, chương II, $\S 5,$ no. 3; hãy nhớ rằng $f(x) = (x, x, \ldots)$ trong đó $x_n = x$ với mọi $n \in \mathbf{N}$]. Ta sẽ sử dụng bổ đề sau:

#### Bổ đề 1 {#top-ix-s6-lem-1 .statement}

Cho $(A_n)$ là một dãy các tập con của một không gian tôpô Hausdorff $X$. Khi đó hạn chế của ánh xạ đường chéo $f : X \to X^\mathbf{N}$ lên không gian con $\bigcap_n A_n$ của $X$ là một đồng phôi của $\bigcap_n A_n$ vào một không gian con đóng của $\prod_n A_n$.

Ảnh này là giao của $\prod_n A_n$ và đường chéo $\Delta = f(X)$, là tập đóng trong $X^\mathbf{N}$ vì $X$ là Hausdorff (chương I, $\S 8,$ no. 1); và $f$ là một đồng phôi của $X$ lên $\Delta$.

Với các giả thiết của Mệnh đề 3, $\prod_n A_n$ là một không gian Polish (Mệnh đề 1), do đó $\bigcap_n A_n$ là Polish theo Bổ đề 1 và Mệnh đề 1.

#### Hệ quả {#top-ix-s6-n1-cor-2 .statement}

Tập hợp các số vô tỉ, được trang bị tôpô cảm sinh bởi tôpô của đường thẳng thực $\mathbf{R}$, là một không gian Polish.

Nó là giao của một họ đếm được các tập mở trong $\mathbf{R}$, cụ thể là các phần bù của các tập hợp gồm một số hữu tỉ duy nhất.

#### Định lý 1 {#top-ix-s6-thm-1 .statement}

*Một không gian con* $Y$ *của một không gian Polish* $X$ *là Polish khi và chỉ khi* $Y$ *là giao của một họ đếm được các tập mở trong* $X$.

Sự đủ của điều kiện suy ra ngay lập tức từ các Mệnh đề 2 và 3. Để chứng minh sự cần thiết, cho $d$ là một mêtric tương thích với tôpô của $Y$ và đối với nó $Y$ là đầy đủ. Cho $\overline{Y}$ là bao đóng của $Y$ trong $X$. Với mỗi số nguyên $n > 0$, cho $Y_n$ là tập hợp tất cả các $x \in \overline{Y}$ có một lân cận mở $U$ sao cho đường kính của $U \cap Y$ (đối với mêtric $d$) là $\leq 1/n$. Rõ ràng $Y_n$ là mở trong $\overline{Y}$ và chứa $Y$. Cho $x \in \bigcap_n Y_n$; khi đó $x \in \overline{Y}$, và vết trên $Y$ của bộ lọc lân cận của $x$ trong $X$ là một bộ lọc Cauchy (đối với $d$); do đó bộ lọc này hội tụ đến một điểm của $Y$, và vì vậy $x \in Y$. Suy ra $Y = \bigcap_n Y_n$.

Với mỗi $n$, cho $H_n$ là một tập con mở của $X$ sao cho $H_n \cap \overline{Y} = Y_n$, và cho $(U_m)$ là một dãy các tập con mở của $X$ sao cho $\overline{Y} = \bigcap_m U_m$ (\S 2, no. 5, Mệnh đề 7); khi đó $Y$ là giao của họ đếm được các tập mở $(H_n \cap U_m)$.

#### Hệ quả 1 {#top-ix-s6-thm-1-cor-1 .statement}

*Một không gian* $X$ *là Polish khi và chỉ khi nó đồng phôi với một giao đếm được của các tập mở trong lập phương* $\mathbf{I}^{\mathbf{N}}$, *trong đó* $\mathbf{I}$ *là khoảng* $[0, 1]$ *của* $\mathbf{R}$.

Điều kiện rõ ràng là đủ, và nó là cần thiết vì mọi không gian mêtric hóa được kiểu đếm được đều đồng phôi với một không gian con của $\mathbf{I}^{\mathbf{N}}$ (\S 2, no. 8, Mệnh đề 12).

#### Hệ quả 2 {#top-ix-s6-thm-1-cor-2 .statement}

*Cho* $X$ *và* $Y$ *là hai không gian Polish và cho* $f : X \to Y$ *là một ánh xạ liên tục. Nếu* $Z$ *là một không gian con Polish của* $Y$, *thì* $\overline{f}^{-1}(Z)$ *là một không gian con Polish của* $X$.

Với $Z = \bigcap_n Z_n$, trong đó các $Z_n$ là các tập con mở của $Y$; do đó
$$
\overline{f}^{-1}(Z) = \bigcap_n \overline{f}^{-1}(Z_n),
$$
và các tập hợp $\overline{f}^{-1}(Z_n)$ là mở trong $X$.

### 2. CÁC KHÔNG GIAN SOUSLIN

#### Định nghĩa 2 {#top-ix-s6-def-2 .statement}

*Một không gian tôpô* $X$ *được gọi là một không gian Souslin nếu nó mêtric hóa được và nếu tồn tại một không gian Polish* $P$ *và một ánh xạ liên tục từ* $P$ *lên* $X$. *Một tập con* $A$ *của một không gian tôpô* $X$ *được gọi là một tập Souslin nếu không gian con* $A$ *là một không gian Souslin.*

Rõ ràng mọi không gian Polish đều là Souslin, và ảnh của một không gian Souslin $X$ qua một ánh xạ liên tục của $X$ vào một không gian mêtric hóa $Y$ là một không gian Souslin.

#### Mệnh đề 4 {#top-ix-s6-prop-4 .statement}

*Mọi không gian Souslin $X$ đều có kiểu đếm được.*

Cho $P$ là một không gian Polish và $f$ là một ánh xạ liên tục của $P$ lên $X$. Khi đó ảnh qua $f$ của một tập con trù mật đếm được của $P$ là một tập con trù mật đếm được của $X$.

#### Mệnh đề 5 {#top-ix-s6-prop-5 .statement}

*Mọi không gian con đóng (resp. mở) của một không gian Souslin $X$ đều là Souslin.*

Vì nếu $f$ là một ánh xạ liên tục của một không gian Polish $P$ lên $X$, thì ảnh ngược qua $f$ của một tập con đóng (resp. mở) của $X$ là một tập con đóng (resp. mở) của $P$, do đó là một không gian con Polish của $P$ (no. 1, Mệnh đề 1 và 2).

#### Mệnh đề 6 {#top-ix-s6-prop-6 .statement}

*Cho $X$ là một không gian Souslin, cho $Y$ là một không gian Hausdorff và cho $f : X \to Y$ là một ánh xạ liên tục. Khi đó ảnh ngược qua $f$ của một không gian con Souslin $A$ của $Y$ là một không gian con Souslin của $X$.*

Cho $P, Q$ là các không gian Polish, cho $g$ là một ánh xạ liên tục của $P$ lên $X$ và cho $h$ là một ánh xạ liên tục của $Q$ lên $A$. Cho $R$ là tập hợp của tất cả các $(x, y) \in P \times Q$ sao cho $f(g(x)) = h(y)$; $R$ là đóng trong $P \times Q$ và do đó là một không gian con Polish của $P \times Q$ (no. 1, Mệnh đề 1). Cho $\varphi$ là hạn chế vào $R$ của phép chiếu $pr_1$. Khi đó không gian con $\overline{f}^{-1}(A)$ của $X$ là ảnh của $R$ qua ánh xạ liên tục $g \circ \varphi$ và do đó là một không gian Souslin.

#### Mệnh đề 7 {#top-ix-s6-prop-7 .statement}

*Tích và tổng của một họ đếm được các không gian Souslin là các không gian Souslin.*

Với mỗi số nguyên $n$, cho $X_n$ là một không gian mêtric hóa, $P_n$ là một không gian Polish, và $f_n$ là một ánh xạ liên tục của $P_n$ lên $X_n$. Tích (resp. tổng) của các không gian $P_n$ là Polish (no. 1, Mệnh đề 1), và ảnh của không gian này qua ánh xạ là tích của các $f_n$ (resp. ánh xạ trùng với $f_n$ trên $P_n$ với mọi $n$) là tích (resp. tổng) của các không gian $X_n$; không gian sau là mêtric hóa được, và do đó là một không gian Souslin.

#### Mệnh đề 8 {#top-ix-s6-prop-8 .statement}

*Cho $X$ là một không gian khả metric và cho $(A_n)$ là một dãy các không gian con Souslin của $X$. Khi đó hợp và giao của các $A_n$ là các không gian Souslin.*

Các không gian con này chắc chắn là khả metric. Sự tồn tại của ánh xạ chính tắc từ tổng của các $A_n$ lên không gian con $\bigcup_n A_n$ của $X$ cho thấy không gian sau là một không gian Souslin; và $\bigcap_n A_n$ là Souslin theo các Mệnh đề 5 và 7 và Bổ đề 1 của no. 1.

Nói chung, ngay cả trong một không gian Polish, phần bù của một không gian con Souslin không nhất thiết là Souslin (xem Bài tập 6); xem, tuy nhiên, no. 6, Hệ quả của Định lý 2.

#### Mệnh đề 9 {#top-ix-s6-prop-9 .statement}

*Cho $X$ là một không gian khả metric, và cho $A$ là một không gian con Souslin tương đối compact của $X$. Khi đó tồn tại một không gian khả metric compact $K$, một dãy giảm $(B_n)$ các tập con của $K$, mỗi tập là một hợp đếm được của các tập compact, và một ánh xạ liên tục $f : K \to X$, sao cho $A = f\left(\bigcap_n B_n\right)$. \*

Nếu cần, thay $X$ bởi $\overline{A}$, ta có thể giả sử rằng $X$ là compact và $A$ trù mật trong $X$. Vì $A$ là một không gian Souslin, nên tồn tại một không gian Polish $P$ và một ánh xạ liên tục $g : P \to X$ sao cho $g(P) = A$. Theo no. 1, Định lý 1, Hệ quả 1, ta có thể giả sử rằng $P$ là giao của một dãy giảm $(U_n)$ các tập con mở của khối lập phương $I^\mathbf{N}$. Cho $K$ là không gian $I^\mathbf{N} \times X$, không gian này compact và khả metric (\S 2, no. 4, Định lý 1, Hệ quả 2). Cho $G \subset P \times X$ là đồ thị của g, cho $\overline{G}$ là bao đóng của G trong $K$, và cho f là phép chiếu của $K = I^\mathbf{N} \times X$ lên $X$; khi đó rõ ràng ta có $f(G) = A$. Vì g liên tục, G đóng trong $P \times X$ (Chương I, \S 8, no. 1, Mệnh đề 2, Hệ quả 2) và $G = \overline{G} \cap (P \times X)$; do đó $G = \bigcap_n B_n$, trong đó

$$
B_n = \overline{G} \cap (U_n \times X).
$$

Vì mỗi $U_n$ là một hợp đếm được của các tập đóng trong $I^\mathbf{N}$ (\S 2, no. 5, Mệnh đề 7), nên mỗi $B_n$ là một hợp đếm được của các tập compact và chứng minh là xong.

### 3. CÁC TẬP BOREL

#### Định nghĩa 3 {#top-ix-s6-def-3 .statement}

*Cho $X$ là một tập hợp và cho $\mathfrak{L}$ là một tập các tập con của $X$. $\mathfrak{L}$ được gọi là một $\sigma$-đại số trên $X$ nếu các điều kiện sau được thỏa mãn:

a) *Phần bù của mọi tập thuộc $\mathfrak{L}$ lại thuộc $\mathfrak{L}$*.

b) *Mọi giao đếm được của các tập thuộc $\mathfrak{L}$ lại thuộc $\mathfrak{L}$*.

Nếu $\mathfrak{L}$ là một $\sigma$-đại số trên $X$, thì mọi *hợp đếm được* của các tập thuộc $\mathfrak{L}$ lại thuộc $\mathfrak{L}$ (vì phần bù của hợp này là một giao của các tập thuộc $\mathfrak{L}$).

Tập $\mathfrak{B}(X)$ gồm tất cả các tập con của $X$ hiển nhiên là một $\sigma$-đại số. Mọi giao của các $\sigma$-đại số trên $X$ đều là một $\sigma$-đại số trên $X$. Vì thế, đối với bất kỳ tập con nào của $\mathfrak{B}(X)$, luôn tồn tại một $\sigma$-đại số *nhỏ nhất* chứa $\mathfrak{F}$; nó được gọi là $\sigma$-đại số *được sinh bởi* $\mathfrak{F}$.*

#### Định nghĩa 4 {#top-ix-s6-def-4 .statement}

Trong một không gian tôpô $X$, các phần tử của $\sigma$-đại số được sinh bởi tập hợp mọi tập con đóng của $X$ được gọi là các tập Borel trong $X$.

#### Mệnh đề 10 {#top-ix-s6-prop-10 .statement}

Cho $f$ là một ánh xạ liên tục từ một không gian tôpô $X$ vào một không gian tôpô $Y$. Khi đó ảnh ngược qua $f$ của mọi tập Borel trong $Y$ là một tập Borel trong $X$.

Cho $\mathfrak{I}$ là tập hợp tất cả các tập con $A$ của $Y$ sao cho $f^{-1}(A)$ là một tập hợp Borel trong $X$. Suy ra ngay lập tức rằng $\mathfrak{I}$ là một $\sigma$-đại số chứa tất cả các tập con đóng của $Y$; do đó $\mathfrak{I}$ chứa tất cả các tập hợp Borel trong $Y$.

#### Mệnh đề 11 {#top-ix-s6-prop-11 .statement}

Trong một không gian Souslin $X$, mọi tập hợp Borel đều là một tập hợp Souslin.

Cho $\mathfrak{I}$ là tập hợp tất cả các tập con $A$ của $X$ sao cho cả $A$ và $\overline{A}$ đều là các tập hợp Souslin. Theo Mệnh đề 8 của no. 2, $\mathfrak{I}$ là một $\sigma$-đại số. Mọi tập con đóng $F$ của $X$ đều thuộc $\mathfrak{I}$, vì cả $F$ và $\overline{F}$ đều là các tập hợp Souslin (no. 2, Mệnh đề 5); do đó $\mathfrak{I}$ chứa tất cả các tập hợp Borel của $X$ (cf. no. 6, Định lý 2, Hệ quả).

#### Hệ quả {#top-ix-s6-n3-cor-1 .statement}

Cho $f$ là một ánh xạ liên tục từ một không gian Souslin $X$ vào một không gian mêtric $Y$. Nếu $B$ là một tập hợp Borel bất kỳ trong $X$, thì $f(B)$ là một tập hợp Souslin trong $Y$.

Vì $B$ là một không gian Souslin, nên $f(B)$ cũng vậy theo nhận xét sau Định nghĩa 2 (no. 2).

#### Nhận xét 1 {#top-ix-s6-n3-rem-1 .statement}

Ngay cả khi $X$ và $Y$ là các không gian Polish, nói chung không đúng rằng ảnh của một tập hợp Borel trong $X$ qua một ánh xạ liên tục từ $X$ vào $Y$ là một tập hợp Borel trong $Y$ (cf. Bài tập 6; và no. 7, Định lý 3 Hệ quả).

#### Nhận xét 2 {#top-ix-s6-n3-rem-2 .statement}

Cho $X$ là một không gian tôpô và cho $Y$ là một tập con Borel của $X$. Khi đó các tập hợp Borel của không gian $Y$ chính xác là các tập hợp Borel của $X$ được chứa trong $Y$. Vì (i) các tập hợp Borel trong $X$ được chứa trong $Y$ tạo thành một $\sigma$-đại số trên $Y$ chứa các tập hợp đóng trong $Y$ và do đó chứa tất cả các tập hợp Borel của $Y$; (ii) các tập con $A$ của $X$ sao cho $A \cap Y$ là một tập hợp Borel của $Y$ tạo thành một $\sigma$-đại số trên $X$ chứa tất cả các tập hợp đóng của $X$ và do đó chứa tất cả các tập hợp Borel của $X$.

### 4. CÁC KHÔNG GIAN KHÔNG CHIỀU VÀ CÁC KHÔNG GIAN LUSIN

#### Định nghĩa 5 {#top-ix-s6-def-5 .statement}

Một không gian tôpô được gọi là không chiều nếu nó là Hausdorff và nếu mọi điểm đều có một hệ cơ bản các lân cận vừa mở vừa đóng.

Mọi không gian không chiều $X$ đều hoàn toàn rời rạc; vì thành phần liên thông của một điểm $x$ được chứa trong mọi tập hợp chứa $x$ mà vừa mở vừa đóng (Chương I, § II, no. 5), và giao của các tập hợp ấy chỉ là $\{ x \}$ nếu $X$ không chiều.

Ngược lại, một không gian địa phương compact hoàn toàn rời rạc thì không chiều (Chương II, § 4, no. 4, Mệnh đề 6); nhưng tồn tại những không gian mêtric hoàn toàn rời rạc không phải là không chiều [Bài tập 3 b)].

Mọi không gian con của một không gian không chiều đều không chiều, và các tổng tôpô và tích tôpô của các không gian không chiều đều không chiều.

#### Định nghĩa 6 {#top-ix-s6-def-6 .statement}

Một không gian tôpô $X$ là một không gian Lusin nếu nó là mêtric hóa được và nếu tồn tại một không gian Polish không chiều $P$ và một ánh xạ song ánh liên tục của $P$ lên $X$.

Mọi không gian Lusin rõ ràng là một không gian Souslin.

#### Mệnh đề 12 {#top-ix-s6-prop-12 .statement}

Một không gian mêtric hóa được là một không gian Lusin nếu và chỉ nếu nó là ảnh của một không gian Polish dưới một ánh xạ song ánh liên tục.

Điều kiện ấy rõ ràng là cần thiết; ta hãy chứng minh rằng nó cũng đủ. Nếu $f$ là một song ánh liên tục của một không gian Lusin $X$ lên một không gian mêtric hóa được $Y$, thì từ Định nghĩa 6 suy ra $Y$ là một không gian Lusin. Vì thế ta chỉ cần chứng minh rằng một không gian Polish là một không gian Lusin.

Trước hết hãy chú ý rằng, nếu $X$ là một không gian Lusin, thì mọi không gian con $A$ đóng (tương ứng mở) của $X$ đều là một không gian Lusin (xem no. 7, Định lý 3); vì nếu $f$ là một song ánh liên tục của một không gian Polish không chiều $P$ lên $X$, thì $f^{-1}(A)$ đóng (tương ứng mở) trong $P$ và do đó là một không gian con Polish không chiều của $P$ (no. 1, Mệnh đề 1 và 2).

Mọi tích đếm được của các không gian Lusin đều là một không gian Lusin; điều này suy ra từ Mệnh đề 1 của no. 1 và thực tế rằng mọi tích của các không gian không chiều đều không chiều. Mọi giao đếm được của các không gian con Lusin của một không gian tôpô Hausdorff đều là một không gian con Lusin; điều này suy ra từ những nhận xét trên và từ Bổ đề 1 của no. 1. Hơn nữa:

#### Bổ đề 2 {#top-ix-s6-lem-2 .statement}

Nếu một không gian mêtric hóa được $X$ sao cho tồn tại một phân hoạch đếm được $(A_n)$ của $X$ gồm các không gian con Lusin, thì $X$ là một không gian Lusin.

Với mỗi $n$, hãy cho $P_n$ là một không gian Polish không chiều và cho $f_n$ là một song ánh liên tục của $P_n$ lên $A_n$. Nếu $P$ là tổng tôpô của các $P_n$, thì $P$ là Polish (no. 1, Mệnh đề 1) và không chiều, và ánh xạ $f : P \to X$ trùng với $f_n$ trên $P_n$ đối với mỗi $n$ là một song ánh liên tục của $P$ lên $X$; do đó suy ra kết quả.

Bây giờ ta chứng minh rằng khoảng $I = [0, 1]$ của $\mathbf{R}$ là một không gian Lusin. Hãy cho $J$ là không gian con của $I$ gồm tất cả các số vô tỉ; khi đó $J$ là Polish (no. 1, Hệ quả của Mệnh đề 3); đồng thời $J$ không chiều, vì nếu x là một điểm bất kỳ của J, thì các vết trên J của các khoảng của R có dạng ]r, s[, với r và s là hữu tỉ và r < x < s, tạo thành một hệ cơ bản các lân cận vừa mở vừa đóng của x trong J (vì các vết trên J của ]r, s[ và [r, s] là như nhau). Do đó J là một không gian con Lusin của I. Giờ thì J và các không gian con của I mà mỗi cái gồm một điểm hữu tỉ duy nhất tạo thành một phân hoạch đếm được của I, và vì thế I là một không gian Lusin theo Bổ đề 2.

Hãy cho $P$ là một không gian Polish tùy ý. Theo Hệ quả 1 của Định lý 1 (no. 1), $P$ đồng phôi với một không gian con của khối lập phương IN, là một giao đếm được của các tập hợp mở trong IN. Vì $I$ là một không gian Lusin, những nhận xét ở đầu chứng minh cho thấy rằng $P$ là một không gian Lusin, và do đó chứng minh của Mệnh đề 12 hoàn tất.

### 5. SÀNG

#### Định nghĩa 7 {#top-ix-s6-def-7 .statement}

Một sàng là một dãy C = (C_n, p_n)_{n \geq 0} sao cho, với mỗi n, C_n là một tập hợp đếm được và p_n là một toàn ánh của C_{n+1} lên C_n.

Với mỗi cặp số nguyên m, n sao cho 0 \leq m \leq n, hãy ký hiệu p_{mn} là ánh xạ đồng nhất của C_m lên chính nó nếu m = n, và là toàn ánh p_m \circ p_{m+1} \circ \cdots \circ p_{n-1} của C_n lên C_m nếu m < n. Rõ ràng p_{mq} = p_{mn} \circ p_{nq} bất cứ khi nào m \leq n \leq q, và do đó ta có thể xét giới hạn ngược L(C) của họ (C_n) đối với họ các ánh xạ (p_{mn}) (Lý thuyết tập hợp, Chương III, § 7). Nếu mỗi C_n được trang bị tôpô rời rạc, thì L(C) là một giới hạn ngược của các không gian tôpô (Chương I, § 4, no. 4); do đó, L(C) được gọi là không gian tôpô liên kết với sàng C. L(C) là một không gian con đóng của tích tôpô $\prod_n C_n$, và suy ra ngay rằng L(C) là một không gian Polish không chiều (no. 4).

Một sự sàng lọc của một không gian mêtric X gồm một sàng C = (C_n, p_n) và với mỗi số nguyên n \geq 0 một ánh xạ \varphi_n của C_n vào tập hợp các tập hợp con đóng không rỗng của X có đường kính \leq 2^{-n}, sao cho:

a) X là hợp của các tập hợp \varphi_0(c) khi c chạy qua C_0;
b) với mỗi n và mỗi c \in C_n, \varphi_n(c) là hợp của các tập hợp \varphi_{n+1}(c'), trong đó c' chạy qua p_n^{-1}(c).

Một sự sàng lọc được gọi là ngặt nếu thêm vào đó, với mỗi n, các tập hợp \varphi_n(c), khi c chạy qua C_n, rời nhau đôi một.

#### Bổ đề 3 {#top-ix-s6-lem-3 .statement}

Mọi không gian mêtric X kiểu đếm được đều có một sự sàng lọc. Nếu thêm vào đó X không chiều, thì X có một sự sàng lọc ngặt.

Lưu ý trước rằng nếu $Y$ là một không gian mêtric kiểu đếm được và nếu $\varepsilon$ là một số thực $> 0$, thì có một phủ đếm được của $Y$ bởi các tập hợp có đường kính $\leq \varepsilon$ ($\S 2$, no. 8, Mệnh đề 13). Nếu hơn nữa, $Y$ là không chiều, thì có một phủ như vậy $(V_n)$ tạo bởi các tập hợp vừa mở vừa đóng; nếu $W_n$ là giao của $V_n$ và $\bigcap_{k < n} (Y - V_k)$, ta thấy rằng các $W_n$ là đóng, có đường kính $\leq \varepsilon$, rời nhau từng đôi một và phủ $X$. Trong mọi trường hợp, các bao đóng của các tập hợp không rỗng của phủ tạo thành một phủ đếm được của $Y$ mà các phần tử của nó là các tập hợp đóng không rỗng có đường kính $\leq \varepsilon$.

Cho $X$ là một không gian mêtric kiểu đếm được. Cho $C_0$ là tập hợp các chỉ số của một phủ đếm được của $X$ tạo bởi các tập hợp đóng không rỗng có đường kính $\leq 1$, rời nhau từng đôi một nếu $X$ là không chiều; $\varphi_0$ sẽ là ánh xạ gán cho mỗi chỉ số $c \in C_0$ tập hợp tương ứng của phủ. Giả sử rằng ta đã định nghĩa các $C_i$ và các $\varphi_i$ và các ánh xạ toàn ánh $p_i : C_{i+1} \to C_i$ với $i \leq n$ theo cách sao cho điều kiện b) được thỏa mãn đối với các chỉ số này. Nếu $c \in C_n$, không gian $\varphi_n(c)$ có một phủ đếm được bởi các tập hợp đóng không rỗng có đường kính $\leq 1/2^{n+1}$, rời nhau từng đôi một nếu $X$ [và do đó $\varphi_n(c)$] là không chiều; nếu $I(c)$ chỉ tập hợp chỉ số của phủ này, ta lấy $c_{n+1}$ là tổng của các tập hợp $I(c)$ khi $c$ chạy qua $C_n$; với mỗi $c' \in C_{n+1}$, cho $p_n(c')$ là phần tử $c \in C_n$ sao cho $c' \in I(c)$, và cho $\varphi_{n+1}(c')$ là tập hợp có chỉ số $c'$ trong phủ của $\varphi_n(c)$ đang xét. Rõ ràng do đó ta định nghĩa bằng quy nạp một phép sàng lọc của $X$, và phép sàng lọc này là ngặt nếu $X$ là không chiều; do đó có Bổ đề 3.

Now suppose that $X$ is a complete metric space of countable type, and consider a sifting of $X$ by a sieve $C$ and mappings $\varphi_n$. If $\gamma = (c_n)$ is a point of the space $L(C)$ associated with $C$, the sequence $(\varphi_n(c_n))$ is a decreasing sequence of closed sets in $X$ whose diameters tend to 0; the intersection of this sequence of sets consists therefore of a single point, which we denote by $f(\gamma)$. Thus we have defined a mapping $f : L(C) \to X$. If two points $\gamma, \gamma'$ of $L(C)$ have the same $i$-th coordinates for $i \leq n$, it is clear that the distance between $f(\gamma)$ and $f(\gamma')$ is $\leq 1/2^n$, and therefore $f$ is continuous, by virtue of the definition of the topology of $L(C)$. For each $x \in X$ it follows from the definition of a sifting that we can define by induction on $n$ a sequence $\gamma = (c_n)$ such that $x \in \varphi_n(c_n)$ for each $n \geq 0$, and $c_n = p_n(c_{n+1})$; hence $x = f(\gamma)$ and so $f$ is surjective. Furthermore, if the sifting is strict, the sequence $\gamma = (c_n)$ such that $x = f(\gamma)$ is unique, and so in this case $f$ is bijective. $f$ is said to be the mapping induced by the sifting considered.

#### Mệnh đề 13 {#top-ix-s6-prop-13 .statement}

*Nếu $X$ là một không gian Lusin (tương ứng, Souslin) bất kỳ, thì tồn tại một sieve $C$ và một song ánh liên tục (tương ứng, toàn ánh liên tục) từ $L(C)$ lên $X$.*

Dẫn chiếu đến định nghĩa của một không gian Lusin (mục 4, Định nghĩa 6) [tương ứng, một không gian Souslin (mục 2, Định nghĩa 2)], ta rút gọn về trường hợp trong đó

X là Polish và chiều không (tương ứng, Polish), và lập luận ở trên khi đó chứng minh kết quả.

### 6. SỰ PHÂN LY CỦA CÁC TẬP SOUSLIN

#### Định lý 2 {#top-ix-s6-thm-2 .statement}

Cho X là một không gian mêtric. Nếu ta được cho một dãy $(X_n)$ gồm các không gian con Souslin rời nhau từng đôi một của X, thì tồn tại một dãy $(B_n)$ gồm các tập Borel rời nhau từng đôi một trong X sao cho $X_n \subset B_n$ với mỗi n.

Chứng minh dựa trên hai bổ đề sau:

#### Bổ đề 4 {#top-ix-s6-lem-4 .statement}

Cho $(A_n), (A'_m)$ là hai dãy các tập con của một không gian tôpô X. Giả sử rằng với mỗi cặp $(A_n, A'_m)$ có một tập Borel $B_{nm}$ của X sao cho $B_{nm} \supset A_n$ và $B_{nm} \cap A'_m = \emptyset$. Khi đó tồn tại một tập Borel B của X chứa $\bigcup_n A_n$ và không gặp $\bigcup_m A'_m$.

Thật vậy, tập Borel $B = \bigcup_n \left( \bigcap_m B_{nm} \right)$ thỏa các điều kiện này.

#### Bổ đề 5 {#top-ix-s6-lem-5 .statement}

Cho X là một không gian Hausdorff và cho A, A' là hai không gian con Souslin rời nhau của X. Khi đó tồn tại một tập Borel B của X sao cho $B \supset A$ và $B \cap A' = \emptyset$.

Theo Mệnh đề 13 của no. 5, tồn tại hai sàng C, C' và các ánh xạ liên tục f từ L(C) lên A, $f'$ từ L(C') lên A', được xây dựng theo phương pháp đã mô tả ở no. 5. Với mỗi $n \geq 0$ và mỗi $c \in C_n$, gọi $q_n(c)$ là không gian con của L(C) gồm tất cả các dãy $(c_k)_{k \geq 0}$ sao cho $c_n = c$; $q_n(c)$ là một không gian con đóng của L(C). Với mỗi $\gamma = (c_n) \in L(C)$, dãy các tập hợp đóng $q_n(c_n)$ là giảm và tạo thành một cơ sở bộ lọc với $\gamma$ làm giới hạn. Hơn nữa, với mỗi $c \in C_n$, các tập hợp $q_{n+1}(d)$, trong đó d chạy qua tập hợp $p_n^{-1}(c)$ trong $C_{n+1}$, tạo thành một phân hoạch của $q_n(c)$. Hãy đặt các định nghĩa tương ứng của ký hiệu cho sàng $c'$.

Ta sẽ lập luận bằng phản chứng và giả sử rằng mọi tập Borel chứa A đều cắt A'. Trước hết, từ Bổ đề 4 và định nghĩa của một sàng lọc suy ra rằng tồn tại $c_0 \in C_0$ và $c'_0 \in C'_0$ sao cho mọi tập Borel chứa $f(q_0(c_0))$ đều cắt $f'(q'_0(c'_0))$. Khi đó ta có thể định nghĩa, bằng quy nạp theo n,

$$
\gamma = (c_n) \in L(C) \quad \text{và} \quad \gamma' = (c'_n) \in L(C')
$$

như sau: giả sử rằng $c_i$ và $c'_i$ đã được định nghĩa cho $i < n$, theo cách sao cho với mỗi chỉ số $i < n$ mọi tập Borel chứa $f(q_i(c_i))$ đều cắt $f'(q'_i(c'_i))$; áp dụng Bổ đề 4 và định nghĩa của một sàng lọc cho các tập $f(q_{n-1}(c_{n-1}))$ và $f'(q'_{n-1}(c'_{n-1}))$, ta thấy tồn tại $c_n \in C_n$ và $c'_n \in C'_n$ sao cho $p_{n-1}(c_n) = c_{n-1}$ và $p_{n-1}(c'_n) = c'_{n-1}$ và sao cho mọi tập Borel chứa $f(q_n(c_n))$ đều cắt $f'(q'_n(c'_n))$. Bây giờ dãy $f(q_n(c_n))$ hội tụ đến một điểm $a = f(\gamma) \in A$, và dãy $f'(q'_n(c'_n))$ hội tụ đến một điểm $a' = f'(\gamma') \in A'$. Vì $A \cap A' = \emptyset$ và $X$ là Hausdorff, nên tồn tại một lân cận đóng $V$ của $a$ không chứa $a'$, và do đó với $n$ đủ lớn, $V$ chứa $f(q_n(c_n))$ và không cắt $f'(q'_n(c'_n))$. Điều này là một mâu thuẫn, vì $V$ là một tập Borel.

Để chứng minh Định lý 2, đặt $Y_n$ là hợp của các tập hợp $X_i$ sao cho $i \neq n$; khi đó $Y_n$ là một không gian con Souslin của $X$ (no. 2, Mệnh đề 8). Với mỗi chỉ số $n$, tồn tại một tập hợp Borel $B'_n$ chứa $X_n$ và không giao với $Y_n$, theo Bổ đề 5. Đặt $B_n$ là giao của $B'_n$ và $\bigcap_{i < n} (X - B'_i)$. Khi đó các $B_n$ là các tập hợp Borel, đôi một rời nhau, và sao cho $B_n \supset X_n$ với mọi $n$.

#### Hệ quả {#top-ix-s6-n6-cor-1 .statement}

*Nếu một phân hoạch đếm được của một không gian khả métr hóa gồm các tập hợp Souslin, thì các tập hợp này là các tập hợp Borel. Đặc biệt, mọi tập hợp Souslin trong một không gian khả métr hóa, mà phần bù của nó là một tập hợp Souslin, đều là một tập hợp Borel.*

### 7. CÁC KHÔNG GIAN LUSIN VÀ CÁC TẬP HỢP BOREL

#### Định lý 3 {#top-ix-s6-thm-3 .statement}

*Cho $X$ là một không gian Lusin. Khi đó một không gian con của $X$ là một không gian Lusin khi và chỉ khi nó là một tập hợp Borel.*

Định lý này là hệ quả của hai bổ đề sau:

#### Bổ đề 6 {#top-ix-s6-lem-6 .statement}

*Trong một không gian Lusin $X$, mọi tập hợp Borel đều là một không gian con Lusin của $X$.*

Đặt $\mathfrak{T}$ là tập hợp tất cả các tập con $A$ của $X$ sao cho cả $A$ và $\complement A$ đều là các không gian con Lusin của $X$. Vì mọi tập hợp đóng và mọi tập hợp mở trong $X$ đều là một không gian con Lusin của $X$ (no. 4), nên $\mathfrak{T}$ chứa mọi tập hợp con đóng của $X$, và do đó bổ đề sẽ được chứng minh nếu ta chỉ ra rằng $\mathfrak{T}$ là một $\sigma$-đại số trên $X$. Để làm điều này, chỉ cần chỉ ra rằng nếu $(A_n)$ là một dãy các tập hợp thuộc $\mathfrak{T}$, thì $\bigcap_n A_n$ và $\bigcup_n A_n$ là các không gian con Lusin của $X$. Bây giờ ta đã thấy ở no. 4 rằng mọi giao đếm được của các không gian con Lusin đều là một không gian con Lusin. Mặt khác, nếu $B_n$ là giao của $A_n$ và $\bigcap_{i < n} \complement A_i$, thì từ giả thiết và nhận xét trước đó suy ra rằng $B_n$ là một không gian con Lusin; và vì $\bigcup_n A_n = \bigcup_n B_n$, nên không gian con $\bigcup_n A_n$ là một không gian con Lusin theo Bổ đề 2 của no. 4.

#### Bổ đề 7 {#top-ix-s6-lem-7 .statement}

*Mọi không gian con Lusin $A$ của một không gian khả métr hóa $X$ đều là một tập hợp Borel trong $X$.*

Theo Mệnh đề 13 của no. 5, tồn tại một sàng $C$ và một song ánh liên tục $f$ của $L(C)$ lên $A$. Với ký hiệu của Bổ đề 5 của no. 6, với mỗi số nguyên $n$ và mỗi $c \in C_n$, hãy ký hiệu $g_n(c)$ là không gian con $f(q_n(c))$ của $X$; nó là một không gian con Lusin và do đó là một không gian con Souslin của $X$. Khi $c$ chạy qua $C_n$, các tập hợp $g_n(c)$ đôi một rời nhau, vì $f$ là song ánh; do đó, theo Định lý 2 của no. 6, tồn tại một họ $c \to g'_n(c)$ ($c \in C_n$) các tập hợp Borel trong $X$, đôi một rời nhau và sao cho $g'_n(c) \supset g_n(c)$ với mọi $c \in C_n$. Nếu cần, thay $g'_n(c)$ bằng giao của nó với bao đóng của $g_n(c)$ trong $X$, ta có thể giả sử rằng $g'_n(c) \subset g_n(c)$. Đặt $c_{n-1}, c_{n-2}, ..., c_0$ là các ảnh của $c$ trong $C_{n-1}, C_{n-2}, ..., C_0$, theo các toàn ánh

$p_{n-1,n} = p_{n-1},\ p_{n-2,n} = p_{n-2} \circ p_{n-1},\ ...,\ p_{0n} = p_0 \circ p_1 \circ ... \circ p_{n-1}$

tương ứng; và đặt $h_n(c)$ là giao của các tập hợp

$g'_n(c),\ g'_{n-1}(c_{n-1}),\ ...\ ,\ g'_0(c_0)$.

Vì $q_i(c_i) \supset q_n(c)$ với $0 \le i \le n − 1$, nên $h_n(c)$ chứa $g_n(c)$; cũng hiển nhiên rằng $h_n(c)$ là một tập hợp Borel và được chứa trong $g_n(c)$, và khi $c$ chạy qua $C_n$, các $h_n(c)$ là các tập hợp đôi một rời nhau; cuối cùng, theo cách dựng, với mỗi $c' \in C_{n+1}$ ta có $h_{n+1}(c') \subset h_n(p_n(c'))$. Khi đó đặt $B_n$ là hợp của các tập hợp $h_n(c)$ khi $c$ chạy qua $C_n$; $B_n$ là một tập hợp Borel, và $B_{n+1} \subset B_n$; đồng thời $B_n$ chứa hợp của các tập hợp $g_n(c)$ ($c \in C_n$), tức là $A$. Đặt $B$ là giao của dãy giảm các tập hợp $B_n$; $B$ là một tập hợp Borel và chứa $A$. Ta sẽ chứng minh rằng $B = A$, và điều này sẽ hoàn tất chứng minh.

Lấy $x$ là một điểm của $B$. Khi đó, với mỗi số nguyên $n$, tồn tại duy nhất $c \in C_n$ sao cho $x \in h_n(c)$; ta ký hiệu $c$ này là $c_n(x)$. Dãy $(c_n(x))_{n\ge0}$ thuộc $L(C)$. Dãy giảm $(g_n(c_n(x)))$ hội tụ theo định nghĩa đến một điểm $a \in A$; dãy các bao đóng của các tập hợp này cũng hội tụ đến $a$ trong $X$, nên a fortiori dãy $(h_n(c_n(x)))$ cũng vậy. Nay $x$ thuộc tất cả các tập hợp $h_n(c_n(x))$, do đó $x = a \in A$. Bổ đề 7 vì thế được chứng minh, và cùng với nó là Định lý 3.

#### Hệ quả {#top-ix-s6-n7-cor-1 .statement}

*Nếu $f$ là một ánh xạ đơn ánh liên tục của một không gian Lusin (hoặc, nói riêng, một không gian Polish) $X$ vào một không gian khả métr hóa $Y$, thì $f(X)$ là một tập hợp Borel trong $Y$.*

### 8. CÁC PHẦN CẮT BOREL

#### Định lý 4 {#top-ix-s6-thm-4 .statement}

*Cho $X$ là một không gian Polish và cho $R$ là một quan hệ tương đương trên $X$, sao cho các lớp tương đương modulo $R$ là đóng trong $X$ và bao hòa (theo $R$) của mỗi tập hợp đóng trong $X$ là một tập hợp Borel. Khi đó tồn tại một tập hợp Borel trong $X$ giao với mỗi lớp tương đương đúng một điểm.*

Xét một metric trên $X$ tương thích với tôpô của nó, và theo metric đó $X$ đầy đủ. Theo Bổ đề 3 của no. 5, tồn tại một phép sàng của $X$, được xác định bởi một sàng $C = (C_n, p_n)$ và một dãy các ánh xạ $(\varphi_n)$. Với mỗi $c \in C_n$, đặt $g_n(c)$ là bao hòa của tập hợp đóng $\varphi_n(c)$ theo $R$; theo giả thiết, $g_n(c)$ là một tập hợp Borel trong $X$.

Vì mỗi tập hợp $C_n$ là đếm được, ta có thể đặt một thứ tự tuyến tính trên mỗi $C_n$ sao cho tập hợp các phần tử nhỏ hơn một phần tử cho trước là hữu hạn. Với mỗi $c \in C_n$, ta định nghĩa một tập hợp $h_n(c)$ bằng quy nạp theo $n$, như sau. Trước hết, với $c \in C_0$, $h_0(c)$ là giao của $\varphi_0(c)$ và các tập hợp $X - g_0(c')$, với $c' \in C_0$ và $c' < c$. Với $c \in C_{n+1}$, $h_{n+1}(c)$ là giao của $\varphi_{n+1}(c), h_n(P_n(c))$ và các tập hợp $X - g_{n+1}(c')$ với $c' \in C_{n+1}$, $p_n(c') = p_n(c)$ và $c' < c$. Các $h_n(c)$ rõ ràng là các tập hợp Borel.

Ta sẽ chứng minh mệnh đề sau: với mỗi số nguyên $n \geq 0$ và mỗi lớp tương đương $H$ mod $R$, tồn tại một phần tử duy nhất $c \in C_n$ sao cho $h_n(c)$ giao với $H$, và ta có
$$
h(c_n) \cap H = \varphi_n(c) \cap H,
$$
và do đó là một tập *đóng*. Với $n = 0$, xét phần tử nhỏ nhất $c \in C_0$ sao cho $\varphi_0(c)$ giao với $H$; khi đó $\varphi_0(c) \cap H$ không giao với bất kỳ tập $g_0(c')$ nào với $c' \in C_0$ và $c' < c$; do đó nó được chứa trong $h_0(c) \cap H$ và suy ra bằng với tập này; hơn nữa, ta có $H \subset g_0(c)$ và vì vậy $h_0(c') \cap H$ là rỗng với $c' \in C_0$ và $c' > c$; do đó mệnh đề được chứng minh cho $n = 0$. Ta tiếp tục bằng quy nạp theo $n$: nếu tồn tại $c \in C_{n+1}$ sao cho $h_{n+1}(c)$ giao với $H$, thì từ quan hệ $h_{n+1}(c) \subset h_n(p_n(c))$ và giả thiết quy nạp suy ra rằng $p_n(c)$ là phần tử duy nhất $d \in C_n$ sao cho $h_n(d)$ giao với $H$. Hãy chú ý rằng $h_n(d)$, vốn được chứa trong $\varphi_n(d)$, được chứa trong hợp của các tập $\varphi_n(c)$ với $c \in p_n^{-1}(d)$, theo định nghĩa của một phép sàng lọc; do đó tồn tại một phần tử nhỏ nhất $c \in p_n^{-1}(d)$ sao cho $\varphi_{n+1}(c)$ giao với $H$. Vì vậy ta có
$$
\varphi_{n+1}(c) \cap H \subset \varphi_n(d) \cap H = h_n(d) \cap H
$$
theo giả thiết quy nạp. Suy ra
$$
\varphi_{n+1}(c) \cap H \subset \varphi_{n+1}(c) \cap h_n(d),
$$
và vì theo định nghĩa $\varphi_{n+1}(c) \cap H$ không giao với bất kỳ tập nào trong số các tập $g_{n+1}(c')$ với $c' \in p_n^{-1}(d)$ và $c' < c$, nên từ định nghĩa của $h_{n+1}(c)$ suy ra $\varphi_{n+1}(c) \cap H = h_{n+1}(c) \cap H$. Hơn nữa, ta có $H \subset g_{n+1}(c)$ và vì vậy, nếu $c' \in p_n^{-1}(d)$ sao cho $c' > c$, thì $h_{n+1}(c') \cap H$ là rỗng. Do đó mệnh đề được chứng minh cho mọi $n$.

Với mỗi số nguyên $n$, ký hiệu $S_n$ là hợp của các tập $h_n(c)$, khi $c$ chạy qua $C_n$. Tập $S_n$ là một tập Borel, và ta có $S_{n+1} \subset S_n$.

Đặt $S$ là giao của các tập $S_n$, vốn cũng là một tập Borel trong $X$; ta sẽ chứng minh rằng $S$ cắt mỗi lớp tương đương $H$ mod $R$ tại đúng một điểm. Với mỗi $n$, đặt $c_n(H)$ là phần tử duy nhất $c \in C_n$ sao cho $h_{c_n(H)}$ giao với $H$; khi đó $S_n \cap H = \varphi_n(c_n(H)) \cap H$, và $S \cap H$ là giao của các tập $\varphi_n(c_n(H)) \cap H$. Vì dãy $(c_n(H))$ thuộc L.C., dãy giảm của các tập đóng $\varphi_n(c_n(H))$, có đường kính tiến tới $0$, hội tụ đến một điểm $x \in X$, vì $X$ là đầy đủ. Do đó giao của các tập đóng $\varphi_n(c_n(H)) \cap H$ chỉ gồm điểm $x$, và chứng minh của Định lý 4 là hoàn tất.

#### Nhận xét {#top-ix-s6-n8-rem-1 .statement}

Đặc biệt, một quan hệ tương đương đóng $R$ thỏa mãn các giả thiết của Định lý 4. Khi $X$ là một không gian compact khả mêtric, Định lý 4 do đó áp dụng cho mọi quan hệ tương đương Hausdorff $R$, vì một quan hệ tương đương Hausdorff trên một không gian compact là đóng (Chương I, § 10, no. 4, Mệnh đề 8).

### 9. TÍNH KHẢ DUNG CỦA CÁC TẬP SOUSLIN

#### Định nghĩa 8 {#top-ix-s6-def-8 .statement}

Cho $X$ là một không gian tôpô Hausdorff. Một capacity trên $X$ là một ánh xạ $f$ của tập $\mathcal{P}(X)$ gồm mọi tập con của $X$ vào đường thẳng thực mở rộng $\overline{\mathbf{R}}$, thỏa mãn các điều kiện sau:

(CA_1) Nếu $A \subset B$, thì $f(A) \leq f(B)$.

(CA_2) Nếu $(A_n)$ là một dãy tăng bất kỳ các tập con của $X$, thì
$$
f\left(\bigcup_n A_n\right) = \sup_n f(A_n).
$$

(CA_3) Nếu $(K_n)$ là một dãy giảm bất kỳ các tập con compact của $X$, thì
$$
f\left(\bigcap_n K_n\right) = \inf_n f(K_n).
$$

#### Ví dụ {#top-ix-s6-n9-exa-1 .statement}

\* Cho $\mu$ là một độ đo dương trên một không gian địa phương compact $X$; khi đó độ đo ngoài tương ứng $\mu^*$ là một capacity trên $X$.
Có thể chứng minh rằng trong không gian Euclid $\mathbf{R}^n$ $(n \geq 3)$, "Newtonian outer capacity" là một capacity theo nghĩa của Định nghĩa 8.

#### Định nghĩa 9 {#top-ix-s6-def-9 .statement}

Cho $f$ là một capacity trên $X$; một tập con $A$ của $X$ được gọi là khả dung (đối với $f$) nếu $f(A) = \sup_k f(K)$, trong đó $K$ chạy qua tập các tập con compact của $A$.

\* Ví dụ, nếu $f$ là một độ đo ngoài $\mu^*$, thì mọi tập mở đều khả dung; các tập khả dung $A$ sao cho $\mu^*(A) < +\infty$ chính xác là các tập $\mu$-khả tích. \*

#### Mệnh đề 14 {#top-ix-s6-prop-14 .statement}

Cho $K$ là một không gian compact và cho $f$ là một dung lượng trên $K$. Nếu $A$ là giao của một dãy giảm $(A_n)$ các tập con của $K$, mỗi tập là một hợp đếm được của các tập đóng, thì $A$ là dung lượng được.

Chỉ cần chứng minh rằng, với mỗi $a < f(A)$, tồn tại một tập đóng $C \subset A$ sao cho $f(C) \geq a$. Trước hết hãy chứng minh rằng tồn tại một dãy $(B_n)_{n \geq 1}$ các tập đóng sao cho $B_n \subset A_n$ và sao cho, nếu ta định nghĩa một dãy $(C_n)$ theo quy nạp bởi các điều kiện $C_0 = A, C_n = C_{n-1} \cap B_n$ với $n \geq 1$, thì $f(C_n) > a$ với mỗi $n \geq 0$. Giả sử các $B_i$ đã được định nghĩa với $i < n$; theo giả thiết ta có $C_{n-1} \subset A \subset A_n$ và $f(C_{n-1}) > a$; vì $A_n$ là hợp của một dãy tăng các tập đóng $D_j$, suy ra từ (CAII) rằng
$$
f(C_{n-1}) = \sup_j f(C_{n-1} \cap D_j).
$$
Do đó tồn tại một chỉ số $j$ sao cho $f(C_{n-1} \cap D_j) > a$, và ta có thể lấy $B_n = D_j$.

Bây giờ đặt $C = \bigcap_n C_n$. Vì $A = \bigcap_n A_n$ và $B_n \subset A_n$, ta có
$$
C = \bigcap_n B_n;
$$
do đó tập hợp $C$ là compact và được chứa trong $A$.

Đặt $B'_n = B_1 \cap B_2 \cap \cdots \cap B_n$; $(B'_n)$ là một dãy giảm các tập con compact của $K$; vì $C_n \subset C_i \subset B_i$ với $i < n$ nên ta cũng có $C_n \subset B'_n$. Theo (CAIII), $f(C) = \inf_n f(B'_n)$, và vì $C \subset C_n \subset B'_n$ nên ta cũng có $f(C) = \inf_n f(C_n) \geq a$. Điều này hoàn tất chứng minh.

#### Định lý 5 {#top-ix-s6-thm-5 .statement}

Cho $X$ là một không gian mêtric hóa được và cho $Y$ là một không gian con Souslin tương đối compact của $X$. Khi đó $Y$ là dung lượng được đối với mọi dung lượng $f$ trên $X$.

Ta đã thấy (no. 2, Mệnh đề 9) rằng tồn tại một không gian compact $K$, một dãy giảm $(A_n)$ các tập con của $K$, mỗi tập là một hợp đếm được của các tập compact, và một ánh xạ liên tục $\varphi : K \to X$ sao cho $Y = \varphi \left( \bigcap_n A_n \right)$. Theo Mệnh đề 14, $\bigcap_n A_n$ là dung lượng được đối với mọi dung lượng trên $K$. Định lý 5 vì thế là một hệ quả của mệnh đề sau:

#### Mệnh đề 15 {#top-ix-s6-prop-15 .statement}

Cho $\varphi$ là một ánh xạ liên tục của một không gian Hausdorff $K$ vào một không gian Hausdorff $X$, và cho $f$ là một dung lượng trên $X$. Nếu với mỗi tập con $A$ của $K$ ta đặt $g(A) = f(\varphi(A))$, thì g là một dung lượng trên $K$; hơn nữa, nếu $A$ là dung lượng được đối với g, thì $\varphi(A)$ là dung lượng được đối với $f$.

Rõ ràng $g$ thỏa mãn các tiên đề $(\mathrm{CA}_I)$ và $(\mathrm{CA}_{II})$. Mặt khác, cho $(C_n)$ là một dãy giảm các tập con compact của $K$, và cho $C = \bigcap_n C_n$; các tập $\varphi(C)$ là compact, và giao của chúng là $\varphi(C)$; vì giao này chắc chắn chứa $\varphi(C)$, và nếu $x \in \varphi(C_n)$ với mọi $n$, thì các tập $\overline{\varphi^1}(x) \cap C_n$ tạo thành một dãy giảm các tập con compact không rỗng của $K$, và do đó giao của chúng không rỗng. Vì vậy ta có $f(\varphi(C)) = \inf_n f(\varphi(C_n))$, tức là $g(C) = \inf_n g(C_n)$; do đó $g$ thỏa mãn tiên đề $(\mathrm{CA}_{III})$ và vì thế là một dung lượng trên $K$.

Now let $A$ be a subset of $K$ which is capacitable with respect to $g$; if $a < f(\varphi(A)) = g(A)$, then there is a compact set $C \subset A$ such that $g(C) \geq a$; thus $\varphi(C)$ is a compact set contained in $\varphi(A)$, and $f(\varphi(C)) \geq a$. Điều này cho thấy rằng $\varphi(A)$ là capacitable đối với $f$, và hoàn tất chứng minh của Mệnh đề 15 và do đó của Định lý 5.

#### Nhận xét {#top-ix-s6-n9-rem-1 .statement}

\* Nếu $\mu$ là một độ đo dương trên một không gian địa phương compact metrizable $X$, thì mọi tập Souslin $A$ của $X$ đều là $\mu$-đo được. Vì nếu $K$ là bất kỳ tập con compact nào của $X$, $K \cap A$ là một tập Souslin tương đối compact, nên là capacitable đối với $\mu^*$ và do đó $\mu$-khả tích. Lưu ý rằng phần bù trong $X$ của một tập Souslin, tuy nói chung không phải là một tập Souslin, nhưng là $\mu$-đo được *.

### Bài tập {#top-ix-s6-exercises}

Xem [các bài tập cho § 6](exercises/s6/).
