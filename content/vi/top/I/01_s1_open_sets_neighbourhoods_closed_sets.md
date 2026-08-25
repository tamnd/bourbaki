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
content_sha256: 94b46d9197c73e1c798e830c55af8d28db72b1a625d38edf824c12af35a53d4d
translated_from: content/en/top/I/01_s1_open_sets_neighbourhoods_closed_sets.md
source_content_sha256: caad119969fe95e177cdfb89bfa13ff8d0159e399ab5d7c4149c74762c8819a5
translation_model: gpt-5.4
translation_run: translate-vi-99db8743
glossary_version: 34
glossary_terms_sha256: bc3ab65db7b1bf5ad736731ffcae3a603e189a0204e84bc4e3d255887f41f287
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. TẬP HỢP MỞ, LÂN CẬN, TẬP HỢP ĐÓNG

### 1. TẬP HỢP MỞ

#### Định nghĩa 1 {#top-i-s1-def-1 .statement}

*Một cấu trúc tôpô* (hay ngắn gọn hơn, *một tôpô*) *trên một tập hợp* $ X $ *là một cấu trúc được cho bởi một tập hợp* $ \mathcal{D} $ *các tập con của* $ X $, *có các tính chất sau* (gọi là *các tiên đề của cấu trúc tôpô*):

(O_I) *Mọi hợp của các tập hợp thuộc* $ \mathcal{D} $ *đều là một tập hợp thuộc* $ \mathcal{D} $.

(O_{II}) *Mọi giao hữu hạn của các tập hợp thuộc* $ \mathcal{D} $ *đều là một tập hợp thuộc* $ \mathcal{D} $.

*Các tập hợp của* $ \mathcal{D} $ *được gọi là các tập hợp mở của cấu trúc tôpô được xác định bởi* $ \mathcal{D} $ *trên* $ X $.

#### Định nghĩa 2 {#top-i-s1-def-2 .statement}

*Một không gian tôpô là một tập hợp được trang bị một cấu trúc tôpô*.

Các phần tử của một không gian tôpô thường được gọi là *điểm*. Khi một tôpô đã được xác định trên một tập hợp $ X $, tập hợp này được gọi là tập hợp *nền* của không gian tôpô $ X $.

Tiên đề (O_I) đặc biệt hàm ý rằng hợp của tập con rỗng của $ \mathcal{D} $, tức là *tập rỗng*, thuộc $ \mathcal{D} $. Tiên đề (O_{II}) hàm ý rằng giao của tập con rỗng của $ \mathcal{D} $, tức là *tập hợp* $ X $, thuộc $ \mathcal{D} $.

Để chỉ ra rằng một tập hợp $ \mathcal{D} $ các tập con của $ X $ thỏa mãn (O_{II}), thường thuận tiện khi chứng minh riêng rẽ rằng nó thỏa mãn hai tiên đề sau đây, mà phép hội của chúng tương đương với (O_{II}):
(O_{II\ a}) *Giao của hai tập hợp thuộc* $ \mathcal{D} $ *thuộc* $ \mathcal{D} $.
(O_{II\ b}) $ X $ *thuộc* $ \mathcal{D} $.

Ví dụ về các tôpô. Cho một tập hợp bất kỳ $ X $, tập hợp các tập con của $ X $ gồm $ X $ và $ \varnothing $ thỏa mãn các tiên đề $ (O_1) $ và $ (O_{II}) $ và do đó xác định một tôpô trên $ X $. Tập hợp tất cả các tập con $ \mathcal{P}(X) $ của $ X $ cũng vậy: tôpô mà nó xác định là tôpô rời rạc trên $ X $, và tập hợp $ X $ với tôpô này được gọi là một không gian rời rạc.

Một phủ $ (U_i)_{i \in I} $ của một tập con $ A $ của một không gian tôpô $ X $ được gọi là mở nếu mọi $ U_i $ đều mở trong $ X $.

#### Định nghĩa 3 {#top-i-s1-def-3 .statement}

*Một đồng phôi của một không gian tôpô $ X $ lên một không gian tôpô $ X' $ là một đẳng cấu của cấu trúc tôpô của $ X $ lên cấu trúc tôpô của $ X' $;* nghĩa là, phù hợp với các định nghĩa tổng quát, *một song ánh của $ X $ lên $ X' $ biến tập hợp các tập con mở của $ X $ thành tập hợp các tập con mở của $ X' $*.

$ X $ và $ X' $ được gọi là *đồng phôi* nếu có một đồng phôi từ $ X $ lên $ X' $.

#### Ví dụ {#top-i-s1-n1-exa-1 .statement}

Nếu $ X $ và $ X' $ là hai không gian rời rạc, mọi song ánh từ $ X $ lên $ X' $ đều là một đồng phôi.

Tiêu chuẩn sau đây suy ra ngay lập tức từ định nghĩa của một đồng phôi: *để một song ánh $ f $ từ một không gian tôpô $ X $ lên một không gian tôpô $ X' $ là một đồng phôi, điều kiện cần và đủ là ảnh qua $ f $ của mỗi tập hợp mở trong $ X $ là một tập hợp mở trong $ X' $, và ảnh ngược qua $ f $ của mỗi tập hợp mở trong $ X' $ là một tập hợp mở trong $ X $*.

### 2. LÂN CẬN

#### Định nghĩa 4 {#top-i-s1-def-4 .statement}

*Cho $ X $ là một không gian tôpô và $ A $ là một tập con bất kỳ của $ X $. Một lân cận của $ A $ là mọi tập con của $ X $ chứa một tập mở chứa $ A $. Các lân cận của một tập con $ \{ x \} $ gồm một điểm duy nhất cũng được gọi là các lân cận của điểm $ x $*

Rõ ràng là mọi lân cận của một tập con $ A $ của $ X $ cũng là một lân cận của mỗi tập con $ B \subset A $; đặc biệt, đó là một lân cận của mỗi điểm của $ A $. Ngược lại, giả sử $ A $ là một lân cận của mỗi điểm của một tập hợp $ B $, và gọi $ U $ là hợp của các tập mở được chứa trong $ A $; khi đó $ U \subset A $, và vì mỗi điểm của $ B $ thuộc về một tập mở được chứa trong $ A $, nên ta có $ B \subset U $; nhưng $ U $ là mở theo $ (O_1) $, do đó $ A $ là một lân cận của $ B $. Đặc biệt:

#### Mệnh đề 1 {#top-i-s1-prop-1 .statement}

*Một tập hợp là một lân cận của mỗi điểm của nó khi và chỉ khi nó là mở.*

Nghĩa thông thường của từ "lân cận" là như vậy nên nhiều tính chất có liên quan đến ý niệm toán học về lân cận xuất hiện như sự diễn đạt toán học của các tính chất trực giác; vì thế việc lựa chọn số hạng này có ưu điểm là làm cho ngôn ngữ có sức diễn đạt hơn. Với mục đích đó, trong một số mệnh đề cũng cho phép dùng các cách nói "đủ gần" và "gần tùy ý" . Chẳng hạn, Mệnh đề 1 có thể được phát biểu dưới dạng sau: một tập hợp $ A $ là mở khi và chỉ khi, với mỗi $ x \in A $, mọi điểm *đủ gần* $ x $ đều thuộc $ A $. Nói chung, ta sẽ nói rằng một tính chất đúng tại mọi điểm *đủ gần* một điểm $ x $, nếu nó đúng tại mọi điểm của một lân cận nào đó của $ x $.

Ta ký hiệu bởi $ \mathcal{B}(x) $ tập hợp tất cả các lân cận của $ x $. Các tập hợp $ \mathcal{B}(x) $ có các tính chất sau:

(V_I) *Mọi tập con của $ X $ chứa một tập hợp thuộc $ \mathcal{B}(x) $ thì tự nó cũng thuộc $ \mathcal{B}(x) $.*

(V_{II}) *Mọi giao hữu hạn của các tập hợp của $ \mathcal{B}(x) $ đều thuộc $ \mathcal{B}(x) $.*

(V_{III}) *Phần tử $ x $ thuộc mọi tập hợp của $ \mathcal{B}(x) $.*

Thật vậy, ba tính chất này là những hệ quả ngay lập tức của Định nghĩa 4 và tiên đề (O_{II}).

(V_{IV}) *Nếu $ V $ thuộc $ \mathcal{B}(x) $, thì tồn tại một tập hợp $ W $ thuộc $ \mathcal{B}(x) $ sao cho, với mỗi $ y \in W $, $ V $ thuộc $ \mathcal{B}(y) $.*

Theo Mệnh đề 1, ta có thể lấy $ W $ là bất kỳ tập hợp mở nào chứa $ x $ và được chứa trong $ V $.

Tính chất này có thể được phát biểu dưới dạng *một lân cận của $ x $ cũng là một lân cận của mọi điểm đủ gần $ x $*.

Bốn tính chất này của các tập hợp $ \mathcal{B}(x) $ là *đặc số*. Chính xác hơn, ta có:

#### Mệnh đề 2 {#top-i-s1-prop-2 .statement}

*Nếu với mỗi phần tử $ x $ của một tập hợp $ X $ ta gán một tập hợp $ \mathcal{B}(x) $ gồm các tập con của $ X $ sao cho các tính chất (V_I), (V_{II}), (V_{III}) và (V_{IV}) được thỏa mãn, thì tồn tại một cấu trúc tôpô duy nhất trên $ X $ sao cho, với mỗi $ x \in X $, $ \mathcal{B}(x) $ là tập hợp các lân cận của $ x $ trong tôpô này.*

Theo Mệnh đề 1, nếu có một tôpô trên $ X $ thỏa mãn các điều kiện này, thì tập hợp các tập mở đối với tôpô này tất yếu là tập hợp $ \mathcal{D} $ gồm các tập con $ A $ của $ X $ sao cho *với mỗi $ x \in A $ ta có $ A \in \mathcal{B}(x) $*; do đó có *tính duy nhất* của tôpô này nếu nó tồn tại.

Tập hợp $ \mathcal{D} $ chắc chắn thỏa mãn các tiên đề (O_I) và (O_{II}): đối với (O_I), điều này suy ra ngay lập tức từ (V_I), và đối với (O_{II}), từ (V_{II}). Nó

![Biểu đồ biểu diễn các tập hợp V, U, W và các điểm x, y, z](https://i.imgur.com/3Q5z5QG.png)

Hình 1.

còn phải chỉ ra rằng, trong tôpô được xác định bởi $ \mathcal{D} $, $ \mathcal{B}(x) $ là tập các lân cận của $ x $ với mỗi $ x \in X $. Từ (V_I) suy ra rằng mọi lân cận của $ x $ đều thuộc $ \mathcal{B}(x) $. Ngược lại, cho $ V $ là một tập hợp thuộc $ \mathcal{B}(x) $, và cho $ U $ là tập hợp các điểm $ y \in X $ sao cho $ V \in \mathcal{B}(y) $; nếu ta có thể chỉ ra rằng $ x \in U, U \subset V $ và $ U \in \mathcal{D} $, thì chứng minh sẽ hoàn tất. Ta có $ x \in U $ vì $ V \in \mathcal{B}(x) $; hơn nữa $ U \subset V $, vì mọi điểm $ y \in U $ đều thuộc $ V $ theo (V_III) và giả thiết $ V \in \mathcal{B}(y) $. Còn phải chỉ ra rằng $ U \in \mathcal{D} $, nghĩa là $ U \in \mathcal{B}(y) $ với mỗi $ y \in U $; nay (Hình 1) nếu $ y \in U $ thì theo (V_IV) tồn tại một tập hợp $ W $ sao cho với mỗi $ z \in W $ ta có $ V \in \mathcal{B}(z) $; vì $ V \in \mathcal{B}(z) $ có nghĩa là $ z \in U $, suy ra $ W \subset U $, và do đó, theo (V_I), $ U \in \mathcal{B}(y) $.

Điều phải chứng minh.

Mệnh đề 2 cho thấy rằng một tôpô trên $ X $ có thể được xác định bằng các tập lân cận $ \mathcal{B}(x) $ của các điểm của $ X $, chỉ với điều kiện là Các tiên đề (V_I), (V_II), (V_III) và (V_IV) được thỏa mãn.

#### Ví dụ {#top-i-s1-n2-exa-1 .statement}

Ta có thể định nghĩa một tôpô trên tập hợp $ Q $ các số hữu tỉ bằng cách lấy làm các tập mở mọi hợp của các khoảng mở bị chặn; tập hợp các tập con này hiển nhiên thỏa mãn (O_I), và để thấy rằng nó thỏa mãn (O_II) thì chỉ cần nhận xét rằng nếu giao của hai khoảng mở $ ]a, b[ $ và $ ]c, d[ $ là không rỗng, thì đó là khoảng $ ]\alpha, \beta[ $, trong đó $ \alpha = \sup(a, c) $ và $ \beta = \inf(b, d) $. Ta cũng thu được cùng một tôpô ấy bằng cách định nghĩa, với mỗi $ x \in Q $, tập $ \mathcal{B}(x) $ các lân cận của $ x $ là tập hợp các tập con chứa một khoảng mở mà $ x $ thuộc vào. Không gian tôpô thu được khi gán tôpô này cho $ Q $ được gọi là đường thẳng hữu tỉ (xem Chương IV, § 1, no. 2). Chú ý rằng trong không gian này mọi khoảng mở đều là một tập mở. \* Ta có thể định nghĩa một tôpô trên tập hợp $ R $ các số thực theo cùng cách đó; $ R $ cùng với tôpô này được gọi là đường thẳng thực (xem § 2, Bài tập 5 và Chương IV, § 1, no. 3). \*

### 3. HỆ CƠ BẢN CÁC LÂN CẬN; CÁC CƠ SỞ CỦA MỘT TÔPÔ

#### Định nghĩa 5 {#top-i-s1-def-5 .statement}

Trong một không gian tôpô $ X $, một hệ cơ bản các lân cận của một điểm $ x $ (tương ứng, của một tập con $ A $ của $ X $) là bất kỳ tập hợp nào $ \mathcal{G} $ gồm các lân cận của $ x $ (tương ứng, $ A $) sao cho với mỗi lân cận $ V $ của $ x $ (tương ứng, $ A $) tồn tại một lân cận $ W \in \mathcal{G} $ sao cho $ W \subset V $.

Nếu $ \mathcal{G} $ là một hệ cơ bản các lân cận của một tập con $ A $ của $ X $, thì mọi giao hữu hạn của các tập hợp thuộc $ \mathcal{G} $ đều chứa một tập hợp thuộc $ \mathcal{G} $.

Ví dụ. 1) Trong một không gian rời rạc (no. 1), chỉ riêng tập hợp $ \{ x \} $ đã tạo thành một hệ cơ bản các lân cận của điểm $ x $.
2) Trên đường thẳng hữu tỉ $ \mathbf{Q} $ tập hợp tất cả các khoảng mở chứa một điểm $ x $ là một hệ cơ bản các lân cận của điểm này. Tập hợp các khoảng mở $ ]x - 1/n, x + 1/n[ $, và tập hợp các khoảng đóng $ [x - 1/n, x + 1/n] $, trong đó $ n $ chạy qua mọi số nguyên $ > 0 $, hoặc qua bất kỳ dãy tăng ngặt vô hạn nào của các số nguyên $ > 0 $, cũng vậy.
\* Có những kết quả tương tự đối với đường thẳng thực. \*

#### Định nghĩa 6 {#top-i-s1-def-6 .statement}

Một cơ sở của tôpô của một không gian tôpô $ X $ là bất kỳ tập hợp nào $ \mathcal{B} $ gồm các tập con mở của $ X $ sao cho mọi tập con mở của $ X $ đều là hợp của các tập hợp thuộc $ \mathcal{B} $.

#### Mệnh đề 3 {#top-i-s1-prop-3 .statement}

Nếu $ X $ là một không gian tôpô, thì để một tập hợp $ \mathcal{B} $ các tập con mở của $ X $ là một cơ sở của tôpô của $ X $, điều kiện cần và đủ là với mỗi $ x \in X $ tập hợp các $ V \in \mathcal{B} $ sao cho $ x \in V $ là một hệ cơ bản các lân cận của $ x $.

Rõ ràng điều kiện là cần thiết. Ngược lại, nếu điều kiện ấy được thỏa mãn, thì với mọi tập mở $ U $ và mọi $ x \in U $ đều có một tập mở $ V_x \in \mathcal{B} $ sao cho $ x \in V_x \subset U $. Do đó hợp của các tập $ V_x $ với $ x \in U $ bằng $ U $. Điều này hoàn tất chứng minh.

#### Ví dụ 1 {#top-i-s1-n3-exa-1 .statement}

Tôpô rời rạc có một cơ sở là tập hợp các tập con của $ X $ chỉ gồm một điểm.
2) Theo định nghĩa, tập hợp các khoảng mở bị chặn là một cơ sở của tôpô trên đường thẳng hữu tỉ (no. 2). \* Tương tự, tập hợp các khoảng mở bị chặn là một cơ sở của tôpô trên đường thẳng thực. \*

### 4. TẬP HỢP ĐÓNG

#### Định nghĩa 7 {#top-i-s1-def-7 .statement}

Trong một không gian tôpô $ X $, các phần bù của các tập mở của $ X $ được gọi là các tập hợp đóng.

Lấy phần bù, ta thấy rằng các tiên đề $(O_I)$ và $(O_{II})$ có dạng sau:

$(O'_I)$ *Mọi giao của các tập hợp đóng đều là một tập hợp đóng.*

$(O'_{II})$ *Mọi hợp hữu hạn của các tập hợp đóng đều là một tập hợp đóng.*

Tập rỗng và toàn bộ không gian $X$ là đóng (và do đó *vừa mở vừa đóng*; xem § 11).

Trên đường thẳng hữu tỉ, mọi khoảng có dạng $[a, \rightarrow[$ đều là một tập hợp đóng, vì phần bù của nó ]\leftarrow, a[ là mở; tương tự, mọi khoảng có dạng ]\leftarrow, a] đều là một tập hợp đóng; do đó mọi khoảng đóng bị chặn $[a, b]$ cũng là một tập hợp đóng, vì nó là giao của các khoảng $[a, \rightarrow[$ và ]\leftarrow, b].

Tập hợp $Z$ các số nguyên là đóng trong đường thẳng hữu tỉ, vì phần bù của nó $\bigcup_{n \in Z} ]n, n+1[$ là mở.

Một *phủ* $(F_i)_{i \in I}$ của một tập con $A$ của một không gian tôpô $X$ được gọi là *đóng* nếu mỗi $F_i$ đều đóng trong $X$.

Một *đẳng cấu đồng phôi* $f$ của một không gian tôpô $X$ lên một không gian tôpô $X'$ (no. 1) có thể được đặc trưng như là một song ánh từ $X$ lên $X'$ *sao cho ảnh theo $f$ của mọi tập con đóng của $X$ là một tập con đóng của $X'$ và ảnh ngược theo $f$ của mọi tập con đóng của $X'$ là một tập con đóng của $X$*.

### 5. CÁC HỌ HỮU HẠN ĐỊA PHƯƠNG

#### Định nghĩa 8 {#top-i-s1-def-8 .statement}

*Một họ $(A_i)_{i \in I}$ các tập con của một không gian tôpô $X$ được gọi là hữu hạn địa phương nếu với mỗi $x \in X$ tồn tại một lân cận $V$ của $x$ sao cho $V \cap A_i = \varnothing$ với mọi chỉ số trừ ra một số hữu hạn chỉ số $i \in I$. Một tập hợp $\mathcal{S}$ các tập con của $X$ được gọi là hữu hạn địa phương nếu họ các tập con được xác định bởi ánh xạ đồng nhất của $\mathcal{S}$ lên chính nó là hữu hạn địa phương.*

Hiển nhiên là nếu $(A_i)_{i \in I}$ là một họ hữu hạn địa phương các tập con và nếu $B_i \subset A_i$ với mỗi $i \in I$, thì họ $(B_i)_{i \in I}$ là hữu hạn địa phương.

Mọi họ *hữu hạn* các tập con của một không gian tôpô $X$ đều hiển nhiên là hữu hạn địa phương; đảo lại thì nói chung không đúng.

\* Ví dụ, trong $\mathbf{R}$, phủ mở tạo bởi khoảng ]\leftarrow, 1[ và các khoảng ]$n, \rightarrow[$ với mỗi số nguyên $n \geqslant 0$ là hữu hạn địa phương; và mỗi khoảng ]$n, \rightarrow[$ gặp một số vô hạn các tập hợp của phủ này. \*

#### Mệnh đề 4 {#top-i-s1-prop-4 .statement}

*Hợp của một họ hữu hạn địa phương các tập hợp con đóng của một không gian tôpô $X$ là đóng trong $X$.*

Cho $ (F_i)_{i \in I} $ là một họ hữu hạn địa phương các tập con đóng của $ X $, và giả sử rằng $ x \in X $ không thuộc $ F = \bigcup_{i \in I} F_i $; khi đó $ x $ có một lân cận $ V $ chỉ gặp những $ F_i $ mà các chỉ số của chúng thuộc một tập con *hữu hạn* $ J $ của $ I $. Với mỗi $ i \in J $ gọi $ U_i $ là phần bù của $ F_i $; khi đó $ \complement F $ chứa tập $ V \cap \bigcap_{i \in J} U_i $, tập này là một lân cận của $ x $ vì mỗi $ U_i $ đều mở và chứa $ x $. Do đó, theo Mệnh đề 1 của no. 2, $ \complement F $ là mở và vì thế $ F $ là đóng trong $ X $.

Ta chú ý rằng hợp của một họ *tùy ý* các tập con đóng của $ X $ không nhất thiết là đóng; ví dụ, trên đường thẳng hữu tỉ $ \mathbf{Q} $, tập hợp $ ]2, 1[ $ là hợp của các tập đóng
$$
\left[ \frac{1}{n}, 1 - \frac{1}{n} \right] \quad \text{với } n > 2,
$$
nhưng không đóng.

### 6. PHẦN TRONG, BAO ĐÓNG, BIÊN CỦA MỘT TẬP HỢP; CÁC TẬP HỢP TRÙ MẬT

#### Định nghĩa 9 {#top-i-s1-def-9 .statement}

*Trong một không gian tôpô $ X $, một điểm $ x $ được gọi là một điểm trong của một tập con $ A $ của $ X $ nếu $ A $ là một lân cận của $ x $. Tập hợp các điểm trong của $ A $ được gọi là phần trong của $ A $ và được ký hiệu bởi $ \dot{A} $.*

Theo các Định nghĩa 9 và 4, một điểm $ x $ là một điểm trong của $ A $ nếu có một tập hợp mở được chứa trong $ A $ và chứa $ x $; suy ra $ \dot{A} $ là hợp của mọi tập hợp mở được chứa trong $ A $, và do đó là *tập hợp mở lớn nhất được chứa trong* $ A $: nói cách khác, nếu $ B $ là một tập hợp *mở* được chứa trong $ A $, thì $ B \subset \dot{A} $. Do đó, nếu $ A $ và $ B $ là hai tập con của $ X $ sao cho $ B \subset A $, thì $ \dot{B} \subset \dot{A} $; và $ A $ là một lân cận của $ B $ khi và chỉ khi $ B \subset \dot{A} $.

#### Nhận xét {#top-i-s1-n6-rem-1 .statement}

Phần trong của một tập hợp không rỗng có thể rỗng; đó là trường hợp của một tập hợp gồm một điểm duy nhất mà không mở, ví dụ trên đường thẳng hữu tỉ \* (hoặc đường thẳng thực) *.

Mệnh đề 1 của no. 2 có thể được phát biểu lại như sau:

*Một tập hợp là mở khi và chỉ khi nó trùng với phần trong của nó.*

Tính chất $ (V_{II}) $ của no. 2 kéo theo rằng mọi điểm là điểm trong của mỗi một trong hai tập con $ A $ và $ B $ đều là một điểm trong của $ A \cap B $; do đó
$$(1)$$ $$
\dot{A} \cap \dot{B} = \dot{A} \cap \dot{B}.
$$

Mọi điểm nằm trong phần trong của phần bù của một tập hợp $ A $ được gọi là một điểm *ngoài* của $ A $, và tập hợp các điểm ấy được gọi là *phần ngoài* của $ A $ trong $ X $; vì vậy một điểm $ x \in X $ là một điểm ngoài của $ A $ được đặc trưng bởi tính chất rằng *$ x $ có một lân cận không giao với* $ A $.

#### Định nghĩa 10 {#top-i-s1-def-10 .statement}

*Sự bao đóng của một tập con* $ A $ *của một không gian tôpô* $ X $ *là tập hợp mọi điểm* $ x \in X $ *sao cho mọi lân cận của* $ x $ *đều gặp* $ A $, *và được ký hiệu là* $ \overline{A} $.

Định nghĩa này có thể được phát biểu lại bằng cách nói rằng một điểm $ x $ nằm trong sự bao đóng của một tập hợp $ A $ nếu có những điểm của $ A $ *ở gần* $ x $ *tùy ý*.

Mọi điểm không thuộc sự bao đóng của $ A $ đều ở ngoài $ A $, và ngược lại; do đó ta có các công thức (đối ngẫu của nhau)

$$(2)$$
$$
\mathcal{C}\overline{A} = \widehat{\mathcal{C}}A,\qquad \mathcal{C}\dot{A} = \overline{\mathcal{C}}A.
$$

Do đó, với mọi mệnh đề về các nội của tập hợp, theo *đối ngẫu* có một mệnh đề tương ứng về các bao đóng, và ngược lại. Đặc biệt, bao đóng của một tập hợp $ A $ là *tập hợp đóng nhỏ nhất chứa* $ A $; nói cách khác, nếu $ B $ là một tập hợp đóng sao cho $ A \subset B $, thì $ \overline{A} \subset B $. Nếu $ A $ và $ B $ là hai tập con của $ X $ sao cho $ A \subset B $, thì $ \overline{A} \subset \overline{B} $.

*Một tập hợp là đóng khi và chỉ khi nó trùng với bao đóng của nó*.

Đối ngẫu của công thức (1) là

$$(3)$$
$$
\overline{A \cup B} = \overline{A} \cup \overline{B}.
$$

#### Mệnh đề 5 {#top-i-s1-prop-5 .statement}

*Cho* $ A $ *là một tập mở trong* $ X $; *khi đó với mọi tập con* $ B $ *của* $ X $ *ta có*

$$(4)$$
$$
A \cap \overline{B} \subset \overline{A \cap B}.
$$

Thật vậy, giả sử $ x \in A \cap \overline{B} $; khi đó nếu $ V $ là một lân cận bất kỳ của $ x $, thì $ V \cap A $ là một lân cận của $ x $, vì $ A $ là mở; do đó $ V \cap A \cap B $ không rỗng và vì thế $ x $ thuộc bao đóng của $ A \cap B $.

Nếu $ x $ nằm trong bao đóng của $ A $ nhưng không thuộc $ A $, thì mọi lân cận của $ x $ đều chứa một điểm của $ A $ *khác với* $ x $; nhưng nếu $ x \in A $ thì có thể xảy ra trường hợp $ x $ có một lân cận không chứa điểm nào của $ A $ ngoài $ x $. Khi đó ta nói rằng $ x $ là một *điểm cô lập* của $ A $. Đặc biệt, $ x $ cô lập trong toàn bộ không gian $ X $ khi và chỉ khi $ \{x\} $ là một tập hợp mở.

Một tập hợp đóng không có điểm cô lập nào được gọi là một tập hợp *hoàn hảo*.

#### Định nghĩa 11 {#top-i-s1-def-11 .statement}

Trong một không gian tôpô $ X $, một điểm $ x $ được gọi là một điểm biên của một tập hợp $ A $ nếu $ x $ nằm trong bao đóng của $ A $ và trong bao đóng của $ \overline{CA} $. Tập hợp các điểm biên của $ A $ được gọi là biên của $ A $.

Biên của $ A $ vì thế là tập $ \overline{A} \cap \overline{\overline{CA}} $, tập này đóng. Một điểm biên $ x $ của $ A $ được đặc trưng bởi tính chất là mọi lân cận của $ x $ đều chứa ít nhất một điểm của $ A $ và ít nhất một điểm của $ \overline{CA} $; $ x $ có thể thuộc hoặc không thuộc $ A $. Biên của $ A $ cũng chính là biên của $ \overline{CA} $. Phần trong của $ A $, phần ngoài của $ A $ và biên của $ A $ đôi một rời nhau và hợp của chúng là toàn bộ không gian $ X $.

#### Định nghĩa 12 {#top-i-s1-def-12 .statement}

Một tập con $ A $ của một không gian tôpô $ X $ được gọi là trù mật trong $ X $ (hoặc đơn giản là trù mật, nếu không có sự mơ hồ nào về $ X $) nếu $ \overline{A} = X $, nghĩa là nếu mọi tập mở không rỗng $ U $ của $ X $ đều giao với $ A $.

#### Ví dụ {#top-i-s1-n6-exa-1 .statement}

* Ta sẽ thấy ở Chương IV, § 1 rằng tập hợp các số hữu tỉ và phần bù của nó là trù mật trên đường thẳng thực. *
Trong một không gian rời rạc $ X $ thì tập con trù mật duy nhất của $ X $ là chính $ X $. Mặt khác, mọi tập con không rỗng của $ X $ đều trù mật đối với tôpô trên $ X $ mà trong đó các tập mở duy nhất là $ \varnothing $ và $ X $.

#### Mệnh đề 6 {#top-i-s1-prop-6 .statement}

Nếu $ \mathcal{B} $ là một cơ sở của tôpô của một không gian tôpô $ X $, thì tồn tại một tập hợp trù mật $ D $ trong $ X $ sao cho $ \mathrm{Card}(D) \leq \mathrm{Card}(\mathcal{B}) $.

Ta có thể quy về trường hợp không tập hợp nào của $ \mathcal{B} $ là rỗng (các tập hợp không rỗng của $ \mathcal{B} $ đã tạo thành một cơ sở của tôpô của $ X $). Với mỗi $ U \in \mathcal{B} $, gọi $ x_V $ là một điểm của $ U $; suy ra từ Mệnh đề 3 của no. 3 rằng tập hợp $ D $ gồm các điểm $ x_U $ là trù mật trong $ X $, và ta có $ \mathrm{Card}(D) \leq \mathrm{Card}(\mathcal{B}) $ (Lý thuyết tập hợp, Chương III, § 3, no. 2, Mệnh đề 3).

### Bài tập {#top-i-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
