---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 1
section_title: Open sets, neighbourhoods, closed sets
lang: vi
source: top-i-iv
pdf_pages: 0023-0031, 0123-0125
extraction: ocr
subsections:
    - "no": 1
      title: OPEN SETS
      page: 0
      pdf_page: 23
    - "no": 2
      title: NEIGHBOURHOODS
      page: 0
      pdf_page: 24
    - "no": 3
      title: FUNDAMENTAL SYSTEMS OF NEIGHBOURHOODS; BASES OF A TOPOLOGY
      page: 0
      pdf_page: 27
    - "no": 4
      title: CLOSED SETS
      page: 0
      pdf_page: 27
    - "no": 5
      title: LOCALLY FINITE FAMILIES
      page: 0
      pdf_page: 28
    - "no": 6
      title: INTERIOR, CLOSURE, FRONTIER OF A SET; DENSE SETS
      page: 0
      pdf_page: 29
statements: 23
exercises: 9
content_sha256: b2cf6453191eb1a662fc9ef42689f97e27c83be16fad942ffc4e4ec5a274f2b4
translated_from: content/en/top/I/01_s1_open_sets_neighbourhoods_closed_sets.md
source_content_sha256: 69c33aa1b07c759c60eb28deb272aa6ed887332ba5d4aeb29cbf610ebb88696c
translation_model: gpt-5.4-mini, gpt-5-mini
translation_run: translate-vi-99db8743
glossary_version: 34
glossary_terms_sha256: bc3ab65db7b1bf5ad736731ffcae3a603e189a0204e84bc4e3d255887f41f287
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. CÁC TẬP MỞ, LÂN CẬN, CÁC TẬP ĐÓNG

### 1. CÁC TẬP MỞ

#### Định nghĩa 1 {#top-i-s1-def-1 .statement}

*Một cấu trúc tôpô* (hay ngắn gọn hơn, *một tôpô*) *trên một tập hợp* $X$ *là một cấu trúc được cho bởi một tập hợp* $\mathcal{D}$ *gồm các tập con của* $X$, *có các tính chất sau* (gọi là *các tiên đề của cấu trúc tôpô*):

(O_I) *Mọi hợp của các tập hợp thuộc* $\mathcal{D}$ *đều là một tập hợp của* $\mathcal{D}$.

(O_{II}) *Mọi giao hữu hạn của các tập hợp thuộc* $\mathcal{D}$ *đều là một tập hợp của* $\mathcal{D}$.

*Các tập hợp của* $\mathcal{D}$ *được gọi là các tập mở của cấu trúc tôpô được xác định bởi* $\mathcal{D}$ *trên* $X$.

#### Định nghĩa 2 {#top-i-s1-def-2 .statement}

*Một không gian tôpô là một tập hợp được trang bị một cấu trúc tôpô*.

Các phần tử của một không gian tôpô thường được gọi là *các điểm*. Khi một tôpô đã được xác định trên một tập hợp $X$, tập hợp này được nói là tập hợp *nền* của không gian tôpô $X$.

Tiên đề (O_I) suy ra nói riêng rằng hợp của tập con rỗng của $\mathcal{D}$, tức là *tập rỗng*, thuộc $\mathcal{D}$. Tiên đề (O_{II}) suy ra rằng giao của tập con rỗng của $\mathcal{D}$, tức là *tập hợp* $X$, thuộc $\mathcal{D}$.

Để chứng minh rằng một tập hợp $\mathcal{D}$ gồm các tập con của $X$ thỏa mãn (O_{II}), thường tiện hơn là chứng minh riêng rẽ rằng nó thỏa mãn hai tiên đề sau, mà phép hội của chúng tương đương với (O_{II}):
(O_{II\ a}) *Giao của hai tập hợp thuộc* $\mathcal{D}$ *thuộc* $\mathcal{D}$.
(O_{II\ b}) $X$ *thuộc* $\mathcal{D}$.

Ví dụ về các tôpô. Cho bất kỳ một tập hợp $X$, tập hợp các tập con của $X$ gồm $X$ và $\varnothing$ thỏa mãn các tiên đề $(O_1)$ và $(O_{II})$ và do đó xác định một tôpô trên $X$. Tập $\mathcal{P}(X)$ gồm tất cả các tập con của $X$ cũng vậy: tôpô mà nó xác định là tôpô rời rạc trên $X$, và tập hợp $X$ với tôpô này được gọi là một không gian rời rạc.

Một phủ $(U_i)_{i \in I}$ của một tập con $A$ của một không gian tôpô $X$ được gọi là mở nếu mọi $U_i$ đều mở trong $X$.

#### Định nghĩa 3 {#top-i-s1-def-3 .statement}

*Một đồng phôi của một không gian tôpô $X$ lên một không gian tôpô $X'$ là một đẳng cấu của cấu trúc tôpô của $X$ lên cấu trúc của $X'$;* tức là, theo các định nghĩa chung, *một song ánh của $X$ lên $X'$ biến tập các tập con mở của $X$ thành tập các tập con mở của $X'$*.

$X$ và $X'$ được nói là *đồng phôi* nếu có một đồng phôi của $X$ lên $X'$.

#### Ví dụ {#top-i-s1-n1-exa-1 .statement}

Nếu $X$ và $X'$ là hai không gian rời rạc, bất kỳ song ánh nào của $X$ lên $X'$ đều là một đồng phôi.

Tiêu chuẩn sau đây suy ra ngay lập tức từ định nghĩa của một đồng phôi: *đối với một song ánh $f$ của một không gian tôpô $X$ lên một không gian tôpô $X'$ là một đồng phôi, điều kiện cần và đủ là ảnh qua $f$ của mỗi tập mở trong $X$ là một tập mở trong $X'$, và ảnh ngược qua $f$ của mỗi tập mở trong $X'$ là một tập mở trong $X$*.

### 2. LÂN CẬN

#### Định nghĩa 4 {#top-i-s1-def-4 .statement}

*Cho $X$ là một không gian tôpô và $A$ là một tập con bất kỳ của $X$. Một lân cận của $A$ là một tập con bất kỳ của $X$ chứa một tập mở chứa $A$. Các lân cận của một tập con $\{ x \}$ gồm một điểm duy nhất cũng được gọi là các lân cận của điểm $x$*.

Hiển nhiên rằng mọi lân cận của một tập con $A$ của $X$ cũng là một lân cận của mỗi tập con $B \subset A$; đặc biệt, nó là một lân cận của mỗi điểm của $A$. Ngược lại, giả sử $A$ là một lân cận của mỗi điểm của một tập hợp $B$, và gọi $U$ là hợp của các tập mở được chứa trong $A$; khi đó $U \subset A$, và vì mỗi điểm của $B$ thuộc về một tập mở được chứa trong $A$, ta có $B \subset U$; nhưng $U$ là mở theo $(O_1)$, do đó $A$ là một lân cận của $B$. Đặc biệt:

#### Mệnh đề 1 {#top-i-s1-prop-1 .statement}

*Một tập hợp là lân cận của mỗi điểm của nó khi và chỉ khi nó là mở.*

Ý nghĩa thông thường của từ "lân cận" khiến cho nhiều tính chất liên quan đến ý niệm toán học về lân cận xuất hiện như là biểu hiện toán học của các tính chất trực giác; do đó việc lựa chọn thuật ngữ này có ưu điểm là làm cho ngôn ngữ biểu đạt hơn. Vì mục đích này, trong một số mệnh đề cũng được phép dùng các biểu thức "đủ gần" và "gần tùy ý". Chẳng hạn, Mệnh đề 1 có thể được phát biểu dưới dạng sau: một tập $A$ là mở khi và chỉ khi, với mỗi $x \in A$, mọi điểm *đủ gần* $x$ đều thuộc về $A$. Tổng quát hơn, ta sẽ nói rằng một tính chất đúng với mọi điểm *đủ gần* một điểm $x$, nếu nó đúng tại mọi điểm của một lân cận nào đó của $x$.

Ta ký hiệu $\mathcal{B}(x)$ là tập hợp tất cả các lân cận của $x$. Các tập $\mathcal{B}(x)$ có các tính chất sau:

(V_I) *Mọi tập con của $X$ chứa một tập thuộc về $\mathcal{B}(x)$ thì chính nó cũng thuộc về $\mathcal{B}(x)$.*

(V_{II}) *Mọi giao hữu hạn của các tập thuộc về $\mathcal{B}(x)$ đều thuộc về $\mathcal{B}(x)$.*

(V_{III}) *Phần tử $x$ thuộc về mọi tập của $\mathcal{B}(x)$.*

Thật vậy, ba tính chất này là những hệ quả ngay lập tức của Định nghĩa 4 và tiên đề (O_{II}).

(V_{IV}) *Nếu $V$ thuộc về $\mathcal{B}(x)$, thì tồn tại một tập $W$ thuộc về $\mathcal{B}(x)$ sao cho, với mỗi $y \in W$, $V$ thuộc về $\mathcal{B}(y)$.*

Theo Mệnh đề 1, ta có thể lấy $W$ là bất kỳ tập mở nào chứa $x$ và được chứa trong $V$.

This property may be expressed in the form that *một lân cận của $x$ cũng là một lân cận của mọi điểm đủ gần $x$*.

Bốn tính chất này của các tập $\mathcal{B}(x)$ là *đặc trưng*. Cụ thể, ta có:

#### Mệnh đề 2 {#top-i-s1-prop-2 .statement}

*Nếu với mỗi phần tử $x$ của một tập $X$ ta tương ứng một tập $\mathcal{B}(x)$ gồm các tập con của $X$ sao cho các tính chất (V_I), (V_{II}), (V_{III}) và (V_{IV}) được thỏa mãn, thì tồn tại một cấu trúc tôpô duy nhất trên $X$ sao cho, với mỗi $x \in X$, $\mathcal{B}(x)$ là tập các lân cận của $x$ trong tôpô này.*

Theo Mệnh đề 1, nếu có một tôpô trên $X$ thỏa mãn các điều kiện này, thì tập các tập mở của tôpô này tất yếu là tập $\mathcal{D}$ gồm các tập con $A$ của $X$ sao cho *với mỗi $x \in A$ ta có $A \in \mathcal{B}(x)$*; do đó là *tính duy nhất* của tôpô này nếu nó tồn tại.

Tập $\mathcal{D}$ hiển nhiên thỏa mãn các tiên đề (O_I) và (O_{II}): đối với (O_I), điều này suy ra ngay lập tức từ (V_I), và đối với (O_{II}), từ (V_{II}). Nó

![Sơ đồ cho thấy các tập V, U, W và các điểm x, y, z](https://i.imgur.com/3Q5z5QG.png)

Hình 1.

còn phải chứng minh rằng, trong tôpô được xác định bởi $\mathcal{D}$, $\mathcal{B}(x)$ là tập các lân cận của $x$ đối với mỗi $x \in X$. Từ (V_I) suy ra rằng mọi lân cận của $x$ đều thuộc $\mathcal{B}(x)$. Ngược lại, cho $V$ là một tập thuộc $\mathcal{B}(x)$, và cho $U$ là tập các điểm $y \in X$ sao cho $V \in \mathcal{B}(y)$; nếu ta có thể chứng minh rằng $x \in U, U \subset V$ và $U \in \mathcal{D}$, thì chứng minh sẽ hoàn tất. Ta có $x \in U$ vì $V \in \mathcal{B}(x)$; đồng thời $U \subset V$, vì mọi điểm $y \in U$ đều thuộc $V$ do (V_III) và giả thiết $V \in \mathcal{B}(y)$. Còn phải chứng minh rằng $U \in \mathcal{D}$, tức là $U \in \mathcal{B}(y)$ đối với mỗi $y \in U$; giờ đây (Hình 1) nếu $y \in U$ thì theo (V_IV) tồn tại một tập $W$ sao cho với mỗi $z \in W$ ta có $V \in \mathcal{B}(z)$; vì $V \in \mathcal{B}(z)$ có nghĩa là $z \in U$, suy ra $W \subset U$, và do đó, theo (V_I), $U \in \mathcal{B}(y)$.

Q.E.D.

Mệnh đề 2 cho thấy một tôpô trên $X$ có thể được xác định bằng các tập $\mathcal{B}(x)$ gồm các lân cận của các điểm của $X$, chỉ với các tiên đề (V_I), (V_{II}), (V_{III}) và (V_{IV}).

#### Ví dụ {#top-i-s1-n2-exa-1 .statement}

We có thể định nghĩa một tôpô trên tập $Q$ của các số hữu tỉ bằng cách lấy làm các tập mở mọi hợp của các khoảng mở bị chặn; tập các tập con này chắc chắn thỏa mãn (O_I), và để thấy rằng nó thỏa mãn (O_II) chỉ cần nhận xét rằng nếu giao của hai khoảng mở $]a, b[$ và $]c, d[$ không rỗng, thì nó là khoảng $]\alpha, \beta[$, trong đó $\alpha = \sup(a, c)$ và $\beta = \inf(b, d)$. Ta thu được cùng một tôpô bằng cách định nghĩa, với mỗi $x \in Q$, tập $\mathcal{B}(x)$ các lân cận của $x$ là tập các tập con chứa một khoảng mở chứa $x$. Không gian tôpô thu được bằng cách gán tôpô này cho $Q$ được gọi là đường thẳng hữu tỉ (xem Chương IV, § 1, no. 2). Chú ý rằng trong không gian này mọi khoảng mở đều là một tập hợp mở. \* Ta có thể định nghĩa một tôpô trên tập $R$ của các số thực theo cùng cách; $R$ với tôpô này được gọi là đường thẳng thực (xem § 2, Bài tập 5 và Chương IV, § 1, no. 3). \*

### 3. HỆ THỐNG LÂN CẬN CƠ BẢN; CƠ SỞ CỦA MỘT TÔPÔ

#### Định nghĩa 5 {#top-i-s1-def-5 .statement}

Trong một không gian tôpô $X$, một hệ cơ bản các lân cận của một điểm $x$ (tương ứng của một tập con $A$ của $X$) là bất kỳ tập $\mathcal{G}$ các lân cận của $x$ (tương ứng của $A$) sao cho với mỗi lân cận $V$ của $x$ (tương ứng của $A$) đều có một lân cận $W \in \mathcal{G}$ sao cho $W \subset V$.

Nếu $\mathcal{G}$ là một hệ cơ bản các lân cận của một tập con $A$ của $X$, thì mọi giao hữu hạn của các tập trong $\mathcal{G}$ đều chứa một tập thuộc $\mathcal{G}$.

Ví dụ. 1) Trong một không gian rời rạc (no. 1), riêng tập $\{ x \}$ đã tạo thành một hệ cơ bản các lân cận của điểm $x$.
2) Trên đường thẳng hữu tỉ $\mathbf{Q}$, tập tất cả các khoảng mở chứa một điểm $x$ là một hệ cơ bản các lân cận của điểm này. Tập các khoảng mở $]x - 1/n, x + 1/n[$, và tập các khoảng đóng $[x - 1/n, x + 1/n]$, trong đó $n$ chạy qua mọi số nguyên $> 0$, hoặc qua bất kỳ dãy số nguyên tăng ngặt vô hạn nào > 0, cũng vậy.
\* Có những kết quả tương tự cho đường thẳng thực. \*

#### Định nghĩa 6 {#top-i-s1-def-6 .statement}

Một cơ sở của tôpô của một không gian tôpô $X$ là bất kỳ tập $\mathcal{B}$ nào gồm các tập con mở của $X$ sao cho mọi tập con mở của $X$ đều là hợp của các tập thuộc $\mathcal{B}$.

#### Mệnh đề 3 {#top-i-s1-prop-3 .statement}

Nếu $X$ là một không gian tôpô, thì để một tập $\mathcal{B}$ gồm các tập con mở của $X$ là một cơ sở của tôpô của $X$ thì điều kiện cần và đủ là với mỗi $x \in X$ tập các $V \in \mathcal{B}$ sao cho $x \in V$ là một hệ cơ bản các lân cận của $x$.

Điều kiện này hiển nhiên là cần thiết. Ngược lại, nếu nó được thỏa mãn, thì với bất kỳ tập mở $U$ nào và bất kỳ $x \in U$ nào cũng có một tập mở $V_x \in \mathcal{B}$ sao cho $x \in V_x \subset U$. Do đó, hợp của các tập $V_x$ với $x \in U$ bằng $U$. Điều đó hoàn tất chứng minh.

#### Ví dụ 1 {#top-i-s1-n3-exa-1 .statement}

Tôpô rời rạc có cơ sở là tập các tập con của $X$ chỉ gồm một điểm.
2) Tập các khoảng mở bị chặn là, theo định nghĩa, một cơ sở của tôpô của đường thẳng hữu tỉ (no. 2). \* Tương tự, tập các khoảng mở bị chặn là một cơ sở của tôpô của đường thẳng thực. \*

### 4. CÁC TẬP HỢP ĐÓNG

#### Định nghĩa 7 {#top-i-s1-def-7 .statement}

Trong một không gian tôpô $X$, các phần bù của các tập mở của $X$ được gọi là các tập đóng.

Lấy phần bù, ta thấy rằng các tiên đề $(O_I)$ và $(O_{II})$ có dạng sau:

$(O'_I)$ *Mọi giao của các tập đóng đều là một tập đóng.*

$(O'_{II})$ *Mọi hợp hữu hạn của các tập đóng đều là một tập đóng.*

Tập rỗng và toàn bộ không gian $X$ là đóng (và do đó *vừa mở vừa đóng*; xem § 11).

Trên đường hữu tỉ, mọi khoảng có dạng $[a, \rightarrow[$ là một tập đóng, vì phần bù của nó ]\leftarrow, a[ là mở; tương tự, mọi khoảng có dạng ]\leftarrow, a] là một tập đóng; do đó mọi khoảng đóng bị chặn $[a, b]$ cũng là một tập đóng, vì nó là giao của các khoảng $[a, \rightarrow[$ và ]\leftarrow, b].

Tập $Z$ các số nguyên hữu tỉ là đóng trong đường hữu tỉ, vì phần bù của nó $\bigcup_{n \in Z} ]n, n+1[$ là mở.

Một *phủ* $(F_i)_{i \in I}$ của một tập con $A$ của một không gian tôpô $X$ được gọi là *đóng* nếu mỗi $F_i$ là đóng trong $X$.

Một *đồng phôi* $f$ của một không gian tôpô $X$ lên một không gian tôpô $X'$ (no. 1) có thể được đặc trưng như là một song ánh của $X$ lên $X'$ *sao cho ảnh theo $f$ của mọi tập con đóng của $X$ là một tập con đóng của $X'$ và ảnh ngược theo $f$ của mọi tập con đóng của $X'$ là một tập con đóng của $X$*.

### 5. HỌ HỮU HẠN ĐỊA PHƯƠNG

#### Định nghĩa 8 {#top-i-s1-def-8 .statement}

*Một họ $(A_i)_{i \in I}$ các tập con của một không gian tôpô $X$ được gọi là hữu hạn địa phương nếu với mỗi $x \in X$ tồn tại một lân cận $V$ của $x$ sao cho $V \cap A_i = \varnothing$ với tất cả trừ một số hữu hạn chỉ số $i \in I$. Một tập $\mathcal{S}$ các tập con của $X$ được gọi là hữu hạn địa phương nếu họ các tập con được xác định bởi ánh xạ đồng nhất của $\mathcal{S}$ lên chính nó là hữu hạn địa phương.*

Hiển nhiên rằng nếu $(A_i)_{i \in I}$ là một họ hữu hạn địa phương các tập con và nếu $B_i \subset A_i$ với mỗi $i \in I$, thì họ $(B_i)_{i \in I}$ là hữu hạn địa phương.

Mọi họ *hữu hạn* các tập con của một không gian tôpô $X$ hiển nhiên là hữu hạn địa phương; đảo lại không đúng nói chung.

\* Ví dụ, trong $\mathbf{R}$, phủ mở tạo bởi khoảng ]\leftarrow, 1[ và các khoảng ]$n, \rightarrow[$ với mỗi số nguyên $n \geqslant 0$ là hữu hạn địa phương; và mỗi khoảng ]$n, \rightarrow[$ gặp một số vô hạn các tập của phủ này. \*

#### Mệnh đề 4 {#top-i-s1-prop-4 .statement}

*Hợp của một họ hữu hạn địa phương các tập con đóng của một không gian tôpô $X$ là đóng trong $X$.*

Cho $(F_i)_{i \in I}$ là một họ hữu hạn địa phương các tập con đóng của $X$, và giả sử rằng $x \in X$ không thuộc $F = \bigcup_{i \in I} F_i$; khi đó $x$ có một lân cận $V$ chỉ gặp những $F_i$ mà chỉ số của chúng thuộc một tập con hữu hạn $J$ của $I$. Với mỗi $i \in J$ hãy lấy $U_i$ là phần bù của $F_i$; khi đó $\complement F$ chứa tập $V \cap \bigcap_{i \in J} U_i$, là một lân cận của $x$ vì mỗi $U_i$ đều mở và chứa $x$. Suy ra, theo Mệnh đề 1 của mục 2, $\complement F$ mở và do đó $F$ đóng trong $X$.

Chúng ta lưu ý rằng hợp của một họ *tùy ý* các tập con đóng của $X$ không nhất thiết là đóng; chẳng hạn, trên đường thẳng hữu tỉ $\mathbf{Q}$, tập $]2, 1[$ là hợp của các tập đóng
$$
\left[ \frac{1}{n}, 1 - \frac{1}{n} \right] \quad \text{cho } n > 2,
$$
nhưng không đóng.

### 6. NỘI, BAO ĐÓNG, BIÊN CỦA MỘT TẬP HỢP; CÁC TẬP TRÙ MẬT

#### Định nghĩa 9 {#top-i-s1-def-9 .statement}

*Trong một không gian tôpô $X$, một điểm $x$ được gọi là một điểm nội của một tập con $A$ của $X$ nếu $A$ là một lân cận của $x$. Tập các điểm nội của $A$ được gọi là nội của $A$ và được ký hiệu bởi $\dot{A}$.*

Theo các Định nghĩa 9 và 4, một điểm $x$ là một điểm nội của $A$ nếu có một tập mở được chứa trong $A$ và chứa $x$; suy ra $\dot{A}$ là hợp của mọi tập mở được chứa trong $A$, và do đó là *tập mở lớn nhất được chứa trong* $A$: nói cách khác, nếu $B$ là một tập *mở* được chứa trong $A$, thì $B \subset \dot{A}$. Do đó, nếu $A$ và $B$ là hai tập con của $X$ sao cho $B \subset A$, thì $\dot{B} \subset \dot{A}$; và $A$ là một lân cận của $B$ khi và chỉ khi $B \subset \dot{A}$.

#### Nhận xét {#top-i-s1-n6-rem-1 .statement}

*Nội của một tập không rỗng có thể rỗng; đây là trường hợp của một tập gồm một điểm duy nhất không mở, chẳng hạn trên đường thẳng hữu tỉ \* (hoặc đường thẳng thực) *.*

Mệnh đề 1 của mục 2 có thể được phát biểu lại như sau:

*Một tập là mở khi và chỉ khi nó trùng với nội của nó.*

Tính chất $(V_{II})$ của mục 2 suy ra rằng mọi điểm là một điểm nội của mỗi một trong hai tập con $A$ và $B$ đều là một điểm nội của $A \cap B$; do đó
$$(1)$$ $$
\dot{A} \cap \dot{B} = \dot{A} \cap \dot{B}.
$$

Mọi điểm thuộc phần trong của phần bù của một tập hợp $A$ được gọi là một *điểm ở ngoài* của $A$, và tập hợp các điểm ấy được gọi là *phần ngoài* của $A$ trong $X$; vì vậy một điểm $x \in X$ là một điểm ở ngoài của $A$ được đặc trưng bởi tính chất rằng *$x$ có một lân cận không giao với* $A$.

#### Định nghĩa 10 {#top-i-s1-def-10 .statement}

*Bao đóng của một tập con* $A$ *của một không gian tôpô* $X$ *là tập hợp tất cả các điểm* $x \in X$ *sao cho mọi lân cận của* $x$ *đều giao với* $A$, *và được ký hiệu bởi* $\overline{A}$.

Định nghĩa này có thể được phát biểu lại bằng cách nói rằng một điểm $x$ nằm trong bao đóng của một tập hợp $A$ nếu có các điểm của $A$ ở gần $x$ tùy ý.

Mọi điểm không nằm trong bao đóng của $A$ đều là điểm ở ngoài của $A$, và ngược lại; do đó ta có các công thức (là đối ngẫu của nhau)

$$(2)$$
$$
\mathcal{C}\overline{A} = \widehat{\mathcal{C}}A,\qquad \mathcal{C}\dot{A} = \overline{\mathcal{C}}A.
$$

Vì thế, với mọi mệnh đề về phần trong của các tập hợp, theo tính đối ngẫu có một mệnh đề về bao đóng, và ngược lại. Đặc biệt, bao đóng của một tập hợp $A$ là *tập đóng nhỏ nhất chứa* $A$; nói cách khác, nếu $B$ là một tập đóng sao cho $A \subset B$, thì $\overline{A} \subset B$. Nếu $A$ và $B$ là hai tập con của $X$ sao cho $A \subset B$, thì $\overline{A} \subset \overline{B}$.

*Một tập hợp là đóng khi và chỉ khi nó trùng với bao đóng của nó*.

Đối ngẫu của công thức (1) là

$$(3)$$
$$
\overline{A \cup B} = \overline{A} \cup \overline{B}.
$$

#### Mệnh đề 5 {#top-i-s1-prop-5 .statement}

*Cho* $A$ *là một tập mở trong* $X$; *khi đó với mọi tập con* $B$ *của* $X$ *ta có*

$$(4)$$
$$
A \cap \overline{B} \subset \overline{A \cap B}.
$$

Thật vậy, giả sử $x \in A \cap \overline{B}$; khi đó nếu $V$ là bất kỳ một lân cận nào của $x$, thì $V \cap A$ là một lân cận của $x$, vì $A$ là mở; do đó $V \cap A \cap B$ không rỗng và vì thế $x$ nằm trong bao đóng của $A \cap B$.

Nếu $x$ thuộc bao đóng của $A$ nhưng không thuộc $A$, thì mọi lân cận của $x$ đều chứa một điểm của $A$ *khác với* $x$; nhưng nếu $x \in A$ thì có thể xảy ra rằng $x$ có một lân cận không chứa điểm nào của $A$ ngoài $x$. Khi đó ta nói rằng $x$ là một *điểm cô lập* của $A$. Đặc biệt, $x$ cô lập trong toàn không gian $X$ khi và chỉ khi $\{x\}$ là một tập mở.

Một tập đóng không có điểm cô lập được gọi là một *tập hoàn hảo*.

#### Định nghĩa 11 {#top-i-s1-def-11 .statement}

Trong một không gian tôpô $X$, một điểm $x$ được gọi là một điểm biên của một tập $A$ nếu $x$ thuộc bao đóng của $A$ và thuộc bao đóng của $\overline{CA}$. Tập các điểm biên của $A$ được gọi là biên của $A$.

Do đó biên của $A$ là tập $\overline{A} \cap \overline{\overline{CA}}$, và đó là một tập đóng. Một điểm biên $x$ của $A$ được đặc trưng bởi tính chất rằng mọi lân cận của $x$ đều chứa ít nhất một điểm của $A$ và ít nhất một điểm của $\overline{CA}$; $x$ có thể thuộc hoặc không thuộc $A$. Biên của $A$ cũng chính là biên của $\overline{CA}$. Phần trong của $A$, phần ngoài của $A$ và biên của $A$ đôi một rời nhau và hợp của chúng là toàn bộ không gian $X$.

#### Định nghĩa 12 {#top-i-s1-def-12 .statement}

Một tập con $A$ của một không gian tôpô $X$ được gọi là trù mật trong $X$ (hay đơn giản là trù mật, nếu không có mơ hồ về $X$) nếu $\overline{A} = X$, tức là nếu mọi tập mở không rỗng $U$ của $X$ đều giao với $A$.

#### Ví dụ {#top-i-s1-n6-exa-1 .statement}

\* Chúng ta sẽ thấy ở Chương IV, § 1 rằng tập các số hữu tỉ và phần bù của nó trù mật trên đường thẳng thực. \*
Trong một không gian rời rạc $X$, tập con trù mật duy nhất của $X$ là chính $X$. Mặt khác, mọi tập con không rỗng của $X$ đều trù mật trong tôpô trên $X$ mà các tập mở duy nhất là $\varnothing$ và $X$.

#### Mệnh đề 6 {#top-i-s1-prop-6 .statement}

Nếu $\mathcal{B}$ là một cơ sở của tôpô của một không gian tôpô $X$, thì tồn tại một tập trù mật $D$ trong $X$ sao cho $\mathrm{Card}(D) \leq \mathrm{Card}(\mathcal{B})$.

Ta có thể chỉ xét trường hợp trong đó không có tập nào của $\mathcal{B}$ là rỗng (các tập không rỗng của $\mathcal{B}$ đã tạo thành một cơ sở của tôpô của $X$). Với mỗi $U \in \mathcal{B}$, cho $x_V$ là một điểm của $U$; suy ra từ Mệnh đề 3 của no. 3 rằng tập $D$ gồm các điểm $x_U$ là trù mật trong $X$, và ta có $\mathrm{Card}(D) \leq \mathrm{Card}(\mathcal{B})$ (Lý thuyết tập hợp, Chương III, § 3, no. 2, Mệnh đề 3).

### Bài tập {#top-i-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
