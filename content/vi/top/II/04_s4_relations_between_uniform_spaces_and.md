---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 4
section_title: Relations between uniform spaces and compact spaces
lang: vi
source: top-i-iv
pdf_pages: 0204-0211, 0215-0221
extraction: ocr
subsections:
    - "no": 1
      title: UNIFORMITY OF COMPACT SPACES
      page: 0
      pdf_page: 204
    - "no": 2
      title: COMPACTNESS OF UNIFORM SPACES
      page: 0
      pdf_page: 207
    - "no": 3
      title: COMPACT SETS IN A UNIFORM SPACE
      page: 0
      pdf_page: 209
    - "no": 4
      title: CONNECTED SETS IN A COMPACT SPACE
      page: 0
      pdf_page: 210
statements: 24
exercises: 23
content_sha256: 8532592a23ab0a39800e8bf3cb4a898eaf0000219277ceecb45e960de152569f
translated_from: content/en/top/II/04_s4_relations_between_uniform_spaces_and.md
source_content_sha256: 33d413c1fed78b55146ebc22613f337b5e448d7bf43b8d118b1324178c5c0724
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-45b98c8e
glossary_version: 34
glossary_terms_sha256: ab1b68faef46a7544409840d45b4a68c3cc03a3bcfd87098ffa16f33e62f4110
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. CÁC QUAN HỆ GIỮA CÁC KHÔNG GIAN ĐỀU VÀ CÁC KHÔNG GIAN COMPACT

### 1. CẤU TRÚC ĐỀU CỦA CÁC KHÔNG GIAN COMPACT

#### Định nghĩa 1 {#top-ii-s4-def-1 .statement}

*Một cấu trúc đều trên một không gian tôpô $X$ được gọi là tương thích với tôpô của $X$ nếu tôpô sau trùng với tôpô do cấu trúc đều cảm sinh.*

Một không gian tôpô được gọi là đều hóa được, và tôpô của nó được gọi là đều hóa được, nếu tồn tại một cấu trúc đều trên không gian tương thích với tôpô của nó.

Có những không gian tôpô không đều hóa được, chẳng hạn mọi không gian không thỏa mãn tiên đề $(O_{III})$ ($\S 1$, no. 2, Hệ quả 3 của Mệnh đề 2); do đó nảy sinh câu hỏi xác định những điều kiện mà dưới đó một không gian tôpô là đều hóa được.

Chúng tôi sẽ không đưa ra một câu trả lời đầy đủ cho câu hỏi này trước Chương IX, $\S 1$. Trong tiết này chúng tôi chỉ khảo sát một trường hợp riêng quan trọng, đó là trường hợp $X$ compact. Khi đó ta có định lý sau:

#### Định lý 1 {#top-ii-s4-thm-1 .statement}

*Trên một không gian compact $X$ có đúng một cấu trúc đều tương thích với tôpô của $X$; các entourage của cấu trúc đều này là tất cả các lân cận của đường chéo $\Delta$ trong $X \times X$. Hơn nữa, $X$ được trang bị cấu trúc đều này là một không gian đều đầy đủ.*

Phần cuối của định lý là hiển nhiên; vì mọi bộ lọc Cauchy trên $X$ đều có một điểm tụ [tiên đề (C)] và do đó hội tụ ($\S 3$, no. 2, Mệnh đề 5, Hệ quả 2).

Bây giờ ta hãy chỉ ra rằng nếu có một cấu trúc đều trên $X$ tương thích với tôpô của $X$, thì tập hợp $U$ các lân cận của cấu trúc đều này là tập hợp mọi lân cận của $\Delta$. Ta đã biết rằng mọi lân cận đều là một lân cận của $\Delta$ ($\S 1$, no. 2, Mệnh đề 2), vì thế ta phải chỉ ra rằng ngược lại mọi lân cận của $\Delta$ đều thuộc $U$. Giả sử có một lân cận $U$ của $\Delta$ không thuộc $U$; khi đó các tập hợp $V \cap C_U$, khi $V$ chạy qua $U$, tạo thành một cơ sở của một bộ lọc $G$ trên không gian compact $X \times X$; do đó $G$ có một điểm tụ $(a, b)$ không thuộc $\Delta$. Vì $U$ là một bộ lọc thô hơn $G$, nên $(a, b)$ cũng là một điểm tụ của $U$. Nhưng cấu trúc đều xác định bởi $U$ là Hausdorff theo giả thiết; vì thế giao của các bao đóng của các tập hợp thuộc $U$ là $\Delta$ ($\S 1$, no. 2, Hệ quả 2 của Mệnh đề 2 và Mệnh đề 3); do đó ta đi đến một mâu thuẫn.

Vậy do đó còn phải chỉ ra rằng tập hợp $B$ các lân cận của $\Delta$ trong $X \times X$ là tập hợp các entourage của một cấu trúc đều tương thích với tôpô của $X$. Muốn vậy, chỉ cần chỉ ra rằng $B$ là tập hợp các entourage của một cấu trúc đều *Hausdorff* trên $X$; vì khi đó tôpô cảm sinh bởi cấu trúc đều này sẽ *thô hơn* tôpô của $X$ (Chương I, $\S 2$, no. 2, Mệnh đề 3) và do đó phải trùng nhau với tôpô sau (Chương I, $\S 9$, no. 4, Định lý 2, Hệ quả 3).

$B$ rõ ràng thỏa mãn các tiên đề $(F_I)$ và $(F_{II})$. Hãy chỉ ra rằng các tiên đề $(U_{II})$ và $(U_{III})$ cũng được thỏa mãn và rằng $\Delta$ là giao của các tập hợp của $B$. Trước hết xét điểm cuối cùng: mọi tập hợp gồm một điểm duy nhất $(x, y) \in X \times X$ đều đóng, vì $X$ là Hausdorff; do đó nếu $x \neq y$, phần bù của $(x, y)$ trong $X \times X$ là một lân cận của $\Delta$. Vì phép đối xứng $(x, y) \to (y, x)$ là một đồng phôi của $X \times X$ lên chính nó,

$$
W = \bigcup_{i=1,2,3} (U_i \times U_i) \text{ của } \Delta \text{ trong } X \times X.
$$

Từ các định nghĩa này suy ra ngay lập tức rằng nếu $(u, v) \in W$ và $u \in V_1$ (resp. $u \in U_1$), thì tất phải có $v \in U_1$ (resp. $v \in U_1 \cup U_3 = \mathcal{C}V_2$); do đó lân cận $V_1 \times V_2$ của $(x, y)$ trong $X \times X$ không giao với $\hat{W}$, và ta được một mâu thuẫn. Điều này kết thúc chứng minh.

#### Nhận xét 1 {#top-ii-s4-n1-rem-1 .statement}

Với mọi *phủ mở hữu hạn* $\mathcal{R} = (U_i)_{1 \leq i \leq n}$ của $X$, tập hợp

$$
V_{\mathcal{R}} = \bigcup_{i=1}^n (U_i \times U_i)
$$

là một lân cận của $\Delta$ trong $X \times X$, và các tập hợp này $V_{\mathcal{R}}$ tạo thành một *hệ lân cận cơ bản* của $\Delta$ (và do đó là một *hệ entourage cơ bản* của cấu trúc đều duy nhất trên $X$). Cho $W$ là một lân cận bất kỳ của $\Delta$ trong $X \times X$; khi đó với mỗi $x \in X$ đều tồn tại một lân cận mở $U_x$ của $x$ trong $X$ sao cho $U_x \times U_x \subset W$. Vì các $U_x$ ($x \in X$) tạo thành một phủ mở của $X$, nên tồn tại một số hữu hạn điểm $x_i$ ($1 \leq i \leq n$) sao cho các $U_{x_i}$ ($1 \leq i \leq n$) tạo thành một phủ $\mathcal{R}$ của $X$. Khi đó ta có $V_{\mathcal{R}} \subset W$, điều này chứng minh mệnh đề.

Vì lý do này, cấu trúc đều duy nhất trên $X$ thường được gọi là *cấu trúc đều của các phủ mở hữu hạn* (xem Chương IX, § 4, Bài tập 17).

#### Hệ quả 1 {#top-ii-s4-thm-1-cor-1 .statement}

*Mọi không gian con của một không gian compac đều có thể trang bị một cấu trúc đều.*

#### Hệ quả 2 {#top-ii-s4-thm-1-cor-2 .statement}

*Mọi không gian compact địa phương đều có thể trang bị một cấu trúc đều.*

Thật vậy, theo định lý của Alexandroff (Chương I, § 9, no. 8, Định lý 4), một không gian compact địa phương là đồng phôi với một không gian con của một không gian compac.

#### Nhận xét 2 {#top-ii-s4-n1-rem-2 .statement}

Có thể xảy ra rằng có nhiều cấu trúc đều phân biệt cùng tương thích với tôpô của một không gian compact địa phương.

Ví dụ, ta đã thấy rằng trên một không gian rời rạc vô hạn có nhiều cấu trúc đều phân biệt cùng tương thích với tôpô rời rạc (§ 2, no. 2, Nhận xét).

Tuy nhiên, không phải tính duy nhất của cấu trúc đều tương thích với tôpô của một không gian có thể trang bị cấu trúc đều là một tính chất đặc trưng cho các không gian compac; có những không gian compact địa phương không compac nhưng có cấu trúc đều duy nhất (Bài tập 4).

#### Định lý 2 {#top-ii-s4-thm-2 .statement}

Mọi ánh xạ liên tục $f$ từ một không gian compac $X$ vào một không gian đều $X'$ đều liên tục đều.

Đặt $g = f \times f$, khi đó $g$ liên tục trên $X \times X$ (Chương I, § 4, no. 1, Mệnh đề 1, Hệ quả 1); do đó với mỗi entourage mở $V'$ của $X'$, $\overline{g^{-1}}(V')$ là một tập con mở của $X \times X$, hiển nhiên chứa đường chéo. Từ đó định lý suy ra từ Định lý 1, vì các entourage mở của $X'$ tạo thành một hệ cơ bản các entourage (§ 1, no. 2, Mệnh đề 2, Hệ quả 2).

Dưới các giả thiết của Định lý 2, hạn chế của $f$ lên mọi không gian con $A$ của $X$ là liên tục đều; do đó (§ 3, no. 6, Định lý 2):

#### Hệ quả {#top-ii-s4-n1-cor-1 .statement}

Cho $A$ là một không gian con trù mật của một không gian compact $X$, và cho $f$ là một ánh xạ từ $A$ vào một không gian đều Hausdorff đầy đủ $X'$. Khi đó $f$ có thể được mở rộng liên tục ra toàn bộ $X$ khi và chỉ khi $f$ là liên tục đều.

### 2. TÍNH COMPACT CỦA CÁC KHÔNG GIAN ĐỀU

#### Định nghĩa 2 {#top-ii-s4-def-2 .statement}

Một không gian đều $X$ được gọi là tiền compact nếu hoàn thành Hausdorff $\hat{X}$ của nó là compact. Một tập con $A$ của một không gian đều $X$ được gọi là một tập con tiền compact nếu không gian con đều $A$ của $X$ là tiền compact.

Do đó một tập con $A$ của một không gian đều $X$ là tiền compắc nếu và chỉ nếu bao đóng của $i(A)$ trong $\hat{X}$ là compắc ($i : X \to \hat{X}$ là ánh xạ chính tắc) (§ 3, no. 9, Mệnh đề 18, Hệ quả 1).

#### Ví dụ {#top-ii-s4-n2-exa-1 .statement}

Trong mọi không gian đều $X$, tập hợp các điểm của một dãy Cauchy $(x_n)$ là tiền compắc. Vì các ảnh của các $x_n$ trong $\hat{X}$ lại tạo thành một dãy Cauchy, ta có thể giả sử rằng $X$ là Hausdorff; khi đó bao đóng trong $\hat{X}$ của tập hợp các điểm $x_n$ gồm các điểm $x_n$ và $\lim_{n \to \infty} x_n$ và do đó là compắc (Chương I, § 9, no. 3, Ví dụ 2).

#### Định lý 3 {#top-ii-s4-thm-3 .statement}

Một không gian đều $X$ là tiền compact nếu và chỉ nếu, với mỗi lân cận $V$ của $X$, tồn tại một phủ hữu hạn của $X$ bởi các tập hợp $V$-nhỏ.

Ta có thể diễn đạt điều kiện này một cách trực giác hơn bằng cách nói rằng $X$ có thể được phủ bởi một số hữu hạn tập hợp nhỏ tùy ý.

Cho $i : X \to \hat{X}$ là ánh xạ chính tắc, khi đó các entourage của $X$ là các ảnh ngược qua $i \times i$ của các entourage của $\hat{X}$ (\S 3, no. 7, Mệnh đề 12). Giả sử $X$ là tiền compắc, và cho $U$ là một entourage bất kỳ của $\hat{X}$; khi đó tồn tại một entourage đối xứng $U'$ của $\hat{X}$ sao cho $\hat{U}' \subset U$. Vì $\hat{X}$ là compắc, tồn tại một số hữu hạn các điểm $x_j \in \hat{X}$ sao cho các $U'(x_j)$ (là các tập $U$-nhỏ) phủ $\hat{X}$. Nếu $V$ là ảnh ngược của $U$ bởi $i \times i$, thì các tập $i^{-1}(U'(x_j))$ là $V$-nhỏ và phủ $X$. Ngược lại, giả sử rằng với mỗi entourage $V$ của $X$ đều có một phủ hữu hạn của $X$ bởi các tập $V$-nhỏ. Ta phải chứng minh rằng mọi siêu bộ lọc $\mathfrak{F}$ trên $\hat{X}$ đều hội tụ; vì $\hat{X}$ là đầy đủ, chỉ cần chứng minh rằng $\mathfrak{F}$ là một *bộ lọc Cauchy*, nghĩa là với mỗi entourage *đóng* $U$ của $\hat{X}$ đều có một tập $U$-nhỏ thuộc $\mathfrak{F}$ (\S 1, no. 2, Mệnh đề 2, Hệ quả 2). Cho $V$ là ảnh ngược của $U$ qua $i \times i$, và cho $(B_j)$ là một phủ hữu hạn của $X$ bởi các tập $V$-nhỏ; khi đó các tập $C_j = i(B_j)$ là $U$-nhỏ và phủ $i(X)$, do đó
$$
\hat{X} = \bigcup_j \overline{C}_j.
$$
Mặt khác, vì $C_j \times C_j \subset U$, và $U$ đóng trong $\hat{X} \times \hat{X}$, nên ta có $\overline{C}_j \times \overline{C}_j \subset U$, do đó các $\overline{C}_j$ cũng là $U$-nhỏ. Vì $\mathfrak{F}$ là một siêu bộ lọc, nên một trong các $\overline{C}_j$ thuộc $\mathfrak{F}$ (Chương I, \S 6, no. 4, Hệ quả của Mệnh đề 5).

Điều phải chứng minh.

#### Hệ quả {#top-ii-s4-n2-cor-1 .statement}

*Một không gian đều $X$ là compact nếu và chỉ nếu nó là Hausdorff và đầy đủ và có thể được phủ bởi một số hữu hạn các tập $V$-nhỏ, trong đó $V$ là một entourage bất kỳ của $X$.*

Điều này suy ra từ Định lý 3 và Định lý 1 của no. 1.

#### Nhận xét 1 {#top-ii-s4-n2-rem-1 .statement}

Một không gian *giả compact* không Hausdorff không nhất thiết là đều hóa được, vì nó không cần thỏa mãn tiên đề $(O_{III})$ (xem Chương I, \S 9, no. 2); chẳng hạn, phần lớn các không gian giả compact không Hausdorff xuất hiện trong hình học đại số đều không thỏa mãn tiên đề $(O_{III})$ (xem Bài tập 2).

#### Mệnh đề 1 {#top-ii-s4-prop-1 .statement}

*Trong một không gian đều, mọi tập con của một tập tiền compact, mọi hợp hữu hạn của các tập tiền compact và bao đóng của mọi tập tiền compact đều là tiền compact.*

Hai khẳng định đầu là những hệ quả ngay lập tức của Định lý 3. Cho $X$ là một không gian đều, $A$ là một tập con tiền compact của $X$, và gọi $i : X \to \hat{X}$ là ánh xạ chính tắc. $i(\overline{A})$ được chứa trong bao đóng của $i(A)$ trong $\hat{X}$ (Chương I, \S 2, no. 1, Định lý 1), do đó bao đóng của $i(\overline{A})$ trong $\hat{X}$ được chứa trong một tập compact và vì vậy là compact.

#### Nhận xét 2 {#top-ii-s4-n2-rem-2 .statement}

Trong một không gian đều $X$, một tập hợp $A$ *tương đối compact* là *tiền compact*, vì $A$ được chứa trong một tập compact. Mặt khác, ngay cả khi $X$ là Hausdorff, một tập hợp tiền compact *không nhất thiết là tương đối compact* trong $X$, như được chỉ ra bởi trường hợp mà chính $X$ là tiền compact nhưng không compact.

#### Mệnh đề 2 {#top-ii-s4-prop-2 .statement}

*Cho $f : X \to Y$ là một ánh xạ liên tục đều. Nếu $A$ là một tập con tiền compact bất kỳ của $X$, thì $f(A)$ là một tập con tiền compact của $Y$.*

Vì nếu $i : X \to \hat{X}$ và $j : Y \to \hat{Y}$ là các ánh xạ chính tắc, thì ta có $j(f(A)) = \hat{f}(i(A))$ (\S 3, no. 7, Mệnh đề 15) và do đó $j(f(A))$ là tương đối compact trong $\hat{Y}$ (Chương I, \S 9, no. 4, Định lý 2, Hệ quả 1).

#### Mệnh đề 3 {#top-ii-s4-prop-3 .statement}

*Cho $X$ là một tập hợp, cho $(Y_\lambda)_{\lambda \in L}$ là một họ các không gian đều, và với mỗi $\lambda \in L$ cho $f_\lambda$ là một ánh xạ của $X$ vào $Y_\lambda$. Trang bị cho $X$ cấu trúc đều thô nhất sao cho các $f_\lambda$ là liên tục đều. Khi đó một tập con $A$ của $X$ là tiền compắc nếu và chỉ nếu $f_\lambda(A)$ là một tập con tiền compắc của $Y_\lambda$ với mỗi $\lambda \in L$.*

Điều kiện đó là cần, theo Mệnh đề 2. Tính đủ suy ra từ sự đặc trưng hóa của bổ sung Hausdorff của $X$ được cho trong \S 3, no. 9, Mệnh đề 18, và định lý Tychonoff (Chương I, \S 9, Định lý 3, Hệ quả).

### 3. CÁC TẬP HỢP COMPẮC TRONG MỘT KHÔNG GIAN ĐỀU

Mệnh đề sau đây đối với một không gian đều tùy ý là một dạng sắc bén hơn của Mệnh đề 2 của Chương I, \S 9, no. 2 đối với các không gian compắc.

#### Mệnh đề 4 {#top-ii-s4-prop-4 .statement}

*Trong một không gian đều $X$, cho $A$ là một tập compact và $B$ là một tập đóng sao cho $A \cap B = \varnothing$. Khi đó tồn tại một lân cận đều $V$ của $X$ sao cho $V(A)$ và $V(B)$ không giao nhau.*

Nếu mệnh đề là sai, thì không một tập hợp nào trong các tập hợp $A \cap \overline{V}(B)$, với $V$ chạy qua tập hợp các entourage đối xứng của $X$, là rỗng; do đó các tập hợp ấy sẽ tạo thành một cơ sở bộ lọc trên $A$, cơ sở này sẽ có một điểm bám $x_0 \in A$. Vậy đối với mỗi entourage đối xứng $V$ của $X$, $\overline{V}(x_0)$ sẽ giao với $B$ và do đó, vì $B$ là đóng, ta sẽ có $x_0 \in B$, trái với giả thiết.

#### Hệ quả {#top-ii-s4-n3-cor-1 .statement}

*Cho $A$ là một tập compact trong một không gian đều $X$; khi đó, khi $V$ chạy qua tập các entourage của $X$, các tập $V(A)$ tạo thành một hệ cơ bản các lân cận của $A$.*

Cho $U$ là một lân cận mở bất kỳ của $A$, khi đó $B = \complement U$ là đóng và không giao với $A$; do đó, theo Mệnh đề 4, tồn tại một entourage $V$ sao cho $V(A) \cap V(B) = \varnothing$, và vì vậy $V(A) \subset U$.

### 4. CÁC TẬP LIÊN THÔNG TRONG MỘT KHÔNG GIAN COMPACT

#### Định nghĩa 3 {#top-ii-s4-def-3 .statement}

*Cho $V$ là một entourage đối xứng của một không gian đều $X$. Một dãy hữu hạn $(x_i)_{0 \leq i \leq n}$ các điểm của $X$ được gọi là một $V$-chain nếu $x_i$ và $x_{i+1}$ là $V$-gần nhau với $0 \leq i < n$. Các điểm $x_0$ và $x_n$ được gọi là các đầu mút của $V$-chain, và người ta nói chúng được nối với nhau bởi $V$-chain.*

Cho một entourage đối xứng $V$, quan hệ "có một $V$-chain nối $x$ với $y$" là một quan hệ tương đương giữa $x$ và $y$ trong $X$. Gọi $A_{x, v}$ là lớp tương đương của $x$ đối với quan hệ này, tức là tập hợp mọi $y \in X$ có thể được nối với $x$ bởi một $V$-chain. Rõ ràng nếu $y \in A_{x, v}$ thì $V(y) \subset A_{x, v}$; do đó $A_{x, v}$ là mở trong $X$; và phần bù của $A_{x, v}$, vì là hợp của các lớp tương đương, cũng mở. Vậy:

#### Mệnh đề 5 {#top-ii-s4-prop-5 .statement}

*Trong một không gian đều $X$, tập hợp $A_{x, v}$ các điểm có thể được nối bằng một xích $V$ tới một điểm đã cho $x$ vừa mở vừa đóng trong $X$.*

Với mỗi $x \in X$, gọi $A_x$ là giao của các tập hợp $A_{x, v}$ khi $V$ chạy qua tập hợp các entourage đối xứng của $X$; $A_x$ là lớp tương đương của $x$ đối với quan hệ tương đương "với mọi entourage đối xứng $V$, tồn tại một $V$-dây chuyền nối $x$ với $y$".

#### Mệnh đề 6 {#top-ii-s4-prop-6 .statement}

*Trong một không gian compact $X$, thành phần của $x$, tập hợp $A_x$, và giao của các lân cận của $x$ vừa mở vừa đóng, cả ba đều trùng nhau.*

Chỉ cần chỉ ra rằng $A_x$ là *liên thông*: vì trong mọi không gian đều $X$ thành phần của $x$ được chứa trong giao của các lân cận của $x$ vừa mở vừa đóng, và giao này được chứa trong $A_x$ theo Mệnh đề 5.

Giả sử $A_x$ không liên thông. Vì $A_x$ là *đóng*, tồn tại hai tập hợp đóng không rỗng rời nhau $B$ và $C$ sao cho $B \cup C = A_x$. Theo Mệnh đề 4 của § 3, tồn tại một entourage $U$ của $X$ sao cho $U(B) \cap U(C)$ là rỗng.

Cho $W$ là một entourage *mở* sao cho $\hat{W} \subset U$, và cho $H$ là tập hợp *đóng* là phần bù của $W(B) \cup W(C)$ trong $X$. Chẳng hạn giả sử rằng $x \in B$, và cho $y$ là một điểm của $C$. Khi đó đối với mỗi entourage đối xứng $V \subset W$ ta thấy ngay lập tức, bằng quy nạp theo $i$, rằng mọi $V$-chain $(x_i)_{0 \leq i \leq n}$ nối $x$ với $y$ trong $X$ đều phải có một điểm trong $H$, theo lựa chọn $W$. Vì theo giả thiết $x$ và $y$ có thể được nối bởi một $V$-chain với mỗi entourage đối xứng $V$, ta thấy rằng $H \cap A_{x, v}$ là không rỗng nếu $V \subset W$. Mặt khác, nếu $V' \subset V$ thì rõ ràng $A_{x, v'} \subset A_{x, v}$; do đó suy ra rằng, khi $V$ chạy qua tập hợp các entourage đối xứng của $X$, các tập hợp $H \cap A_{x, v}$ lập thành một cơ sở lọc gồm các tập hợp *đóng* trong không gian compact $H$. Vậy mọi tập hợp ấy đều có một điểm chung và do đó $H$ cắt $A_x$; nhưng điều này mâu thuẫn với định nghĩa của $H$.

#### Hệ quả {#top-ii-s4-n4-cor-1 .statement}

*Cho X là một không gian địa phương compact và K là một thành phần compact của X. Khi đó các lân cận của K vừa mở vừa đóng tạo thành một hệ cơ sở lân cận của K.*

Cho V là một lân cận mở tương đối compact của K trong X (Chương I, § 9, no. 7, Mệnh đề 10) và gọi F là biên của nó. Cho U ⊂ \overline{V} là một tập hợp vừa mở vừa đóng *đối với* \overline{V}. Khi đó U đóng trong X, và nếu thêm nữa U không giao với F, thì U mở trong X (vì khi đó U ⊂ V và U mở trong V). Vậy chỉ cần chứng minh rằng có một tập con của \overline{V} chứa K, không giao với F và vừa mở vừa đóng đối với \overline{V}.

Giả sử điều đó không đúng: khi đó các giao của F với các tập con của \overline{V} chứa K và vừa mở vừa đóng trong \overline{V} tạo thành một cơ sở bộ lọc gồm các tập hợp đóng trong F; F compact, nên các tập hợp ấy có một điểm chung y ∈ F. Nhưng điều này là vô lý; vì \overline{V} compact, K là một thành phần của \overline{V}, và theo Mệnh đề 6, giao của các tập hợp chứa K và vừa mở vừa đóng trong \overline{V} chính là K. Hệ quả do đó được chứng minh.

#### Mệnh đề 7 {#top-ii-s4-prop-7 .statement}

*Cho X là một không gian compact và R là quan hệ tương đương trên X mà các lớp là các thành phần của X. Khi đó không gian thương X/R là compact và hoàn toàn không liên thông.*

Ta biết từ Chương I, § II, no. 5, Mệnh đề 9 rằng X/R hoàn toàn không liên thông; vì thế ta phải chứng minh rằng X/R là *Hausdorff* (Chương I, § 10, no. 4, Mệnh đề 8.) Cho A và B là hai thành phần phân biệt của X. Theo Mệnh đề 6, có một entourage đối xứng U của X sao cho không điểm nào của A có thể được nối với bất kỳ điểm nào của B bởi một U-chain. Tập hợp V (tương ứng W) gồm các điểm của X có thể được nối với một điểm x ∈ A (tương ứng y ∈ B) bởi một U-chain thì vừa mở vừa đóng trong X (Mệnh đề 5) và chứa A (tương ứng B); do đó các tập hợp này là những lân cận mở của A và B tương ứng, bão hòa đối với R và không giao nhau. Điều đó hoàn tất chứng minh.

### Bài tập {#top-ii-s4-exercises}

Xem [bài tập cho § 4](exercises/s4/).
