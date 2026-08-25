---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 4
section_title: Normal spaces
lang: vi
source: top-v-x
pdf_pages: 0185-0196, 0245-0255
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF NORMAL SPACES
      page: 0
      pdf_page: 185
    - "no": 2
      title: EXTENSION OF A CONTINUOUS REAL-VALUED FUNCTION
      page: 0
      pdf_page: 188
    - "no": 3
      title: LOCALLY FINITE OPEN COVERINGS OF A CLOSED SET IN A NORMAL SPACE
      page: 0
      pdf_page: 191
    - "no": 4
      title: PARACOMPACT SPACES
      page: 0
      pdf_page: 193
    - "no": 5
      title: PARACOMPACTNESS OF METRIZABLE SPACES
      page: 0
      pdf_page: 194
statements: 24
exercises: 7
content_sha256: f0b9f53e5659d1d8f7bebf119767a2e4b3e4aa7824078538581ddf1e20494b05
translated_from: content/en/top/IX/04_s4_normal_spaces.md
source_content_sha256: 5a6d198ba815a6b655dfe1a7d2ffc8cb1105b770a7bb04499c7a43e1d1d1167e
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4-mini
translation_run: translate-vi-fbd3e0f2
glossary_version: 34
glossary_terms_sha256: 63609fbbfb4f2ece843d1ccf91b16136b7ccb069d4ec4a57869255546f7cdfb3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. KHÔNG GIAN CHÍNH QUY

### 1. ĐỊNH NGHĨA CÁC KHÔNG GIAN CHÍNH QUY

Tiên đề ($O_{IV}$) đối với các không gian đồng nhất hóa được ($\S 1$, no. 5) có thể được phát biểu dưới dạng sau: *với mọi tập đóng* $A$ *và mọi điểm* $x \in \mathbf{C}A$, *có một ánh xạ liên tục từ* $X$ *vào* $[0, 1]$ *bằng* 0 *tại* $x$ *và bằng* 1 *tại mọi điểm của* $A$; tính chất này lại có thể được biểu diễn bằng cách nói rằng trong một không gian đồng nhất hóa được ta có thể phân tách một điểm và một tập đóng (không chứa điểm đó) bằng một hàm thực liên tục.

Bây giờ ta sẽ nghiên cứu các không gian trong đó có thể, theo cùng một cách, phân tách hai tập đóng rời nhau bằng một hàm thực liên tục:

#### Định nghĩa 1 {#top-ix-s4-def-1 .statement}

*Một không gian tôpô $X$ được gọi là chính quy nếu nó là Hausdorff và thỏa mãn tiên đề sau:*

$(O_v)$ *Nếu $A$ và $B$ là hai tập con đóng bất kỳ rời nhau của $X$, thì tồn tại một ánh xạ liên tục từ $X$ vào $[0, 1]$ bằng $0$ tại mọi điểm của $A$ và bằng $1$ tại mọi điểm của $B$.*

Rõ ràng mọi không gian chính quy đều hoàn toàn chính quy; nhưng có những không gian hoàn toàn chính quy không chính quy (xem các Bài tập 9, 10, 13, 26 và § 5, các Bài tập 15 và 16).

Phát biểu của Tiên đề $(O_v)$, cũng như của $(O_{IV})$, chứa đường thẳng thực $\mathbf{R}$ như một tập hợp phụ trợ. Nhưng có một điều kiện tương đương với $(O_v)$ không chứa tập hợp phụ trợ nào:

#### Định lý 1 (Urysohn) {#top-ix-s4-thm-1 .statement}

*Tiên đề $(O_v)$ tương đương với điều sau:*

$(O'_v)$ *Nếu $A$ và $B$ là hai tập con đóng bất kỳ rời nhau của $X$, thì tồn tại hai tập mở rời nhau $U, V$ sao cho $A \subset U$ và $B \subset V$.*

Điều này ngay lập tức suy ra rằng $(O_v)$ kéo theo $(O'_v)$, vì nếu $f$ là một ánh xạ liên tục từ $X$ vào $[0, 1]$ bằng $0$ trên $A$ và bằng $1$ trên $B$, thì các tập mở $\overline{f}^{-1}([0, 1/2[)$ và $\overline{f}^{-1}(]1/2, 1])$ lần lượt chứa $A$ và $B$ và không giao nhau.

Để chứng minh đảo lại, trước hết lưu ý rằng $(O'_v)$ tương đương với tiên đề sau:

$(O''_v)$ *Với mọi tập đóng $A$ và mọi lân cận mở $V$ của $A$, tồn tại một lân cận mở $W$ của $A$ sao cho $\overline{W} \subset V$.*

Nếu có một ánh xạ liên tục $f : X \to [-1, +1]$ bằng $-1$ trên $A$ và bằng $+1$ trên $B$, và nếu ta đặt $U(t) = \overline{f}^{-1}([-1, t[)$ với mỗi $t \in [0, 1]$, thì ta đã xác định một họ các tập mở trong $X$, được chỉ số hóa bởi $[0, 1]$, sao cho (i) $A \subset U(0)$, (ii) $B \subset \mathbf{C}U(1)$ và (iii) với mỗi cặp số thực $t, t'$ sao cho $0 \leq t < t' \leq 1$ ta có

$$(1)$$
$$
\overline{U}(t) \subset U(t');
$$

vì $U(t)$ được chứa trong tập đóng $\overline{f}^{-1}([-1, t])$. Ngược lại, giả sử rằng ta đã xác định một họ $(U(t))$ các tập mở $(0 \leq t \leq 1)$ có ba tính chất này (i), (ii) và (iii). Với mỗi $x \in X$, đặt $g(x) = 1$ nếu $x \in \mathbf{C}U(1)$, và nếu $x \in U(1)$ hãy lấy $g(x)$ là cận dưới lớn nhất của các giá trị $t$ sao cho $x \in U(t)$. Rõ ràng $0 \leq g(x) \leq 1$ với mỗi $x \in X$, $g(x) = 0$ trên $A$, $g(x) = 1$ trên $B$; ngoài ra $g$ là liên tục trên $X$, vì nếu ta đặt $g(x) = a$, ta có $|g(y) - g(x)| \leq \varepsilon$ với mọi $y \in U(a + \varepsilon) \cap \overline{\mathbf{C}U}(a - \varepsilon)$, đây là một lân cận của $x$ theo (i) [với các quy ước rằng $U(a + \varepsilon) = X$ nếu $a + \varepsilon > 1$, và $U(a - \varepsilon) = \varnothing$ nếu $a - \varepsilon < 0$].

Do đó Định lý 1 sẽ được chứng minh nếu ta có thể định nghĩa một họ $(U(t))$ các tập hợp mở thỏa mãn các điều kiện (i), (ii) và (iii) ở trên; để làm điều này ta dùng Tiên đề $(\mathrm{O}'_V)$. Lấy $U(1) = \mathbf{C}B$; vì $A \subset U(1)$ nên tồn tại một tập hợp mở $U(o)$ sao cho $A \subset U(o)$ và $U(o) \subset U(1)$ theo $(\mathrm{O}'_V)$. Giả sử khi đó rằng với mỗi số dyadic $k/2^n$ ($k = 0, 1, \ldots, 2^n$) ta đã định nghĩa một tập hợp mở $U(k/2^n)$, các tập hợp này thỏa mãn $\overline{U}(k/2^n) \subset U((k+1)/2^n)$ với $0 \leq k \leq 2^n - 1$. Với mỗi số dyadic
$$
(2k + 1)/2^{n+1} \quad (0 \leq k \leq 2^n - 1)
$$
theo $(\mathrm{O}'_V)$ tồn tại một tập hợp mở $U((2k + 1)/2^{n+1})$ sao cho
$$
\overline{U}(k/2^n) \subset U((2k + 1)/2^{n+1})
$$
và
$$
\overline{U}((2k + 1)/2^{n+1}) \subset U((k + 1)/2^n).
$$
Do đó với mỗi số dyadic $r$ sao cho $0 \leq r \leq 1$ ta có thể định nghĩa một tập hợp mở $U(r)$, sao cho $A \subset U(o)$, $B \subset \mathbf{C}U(1)$, và
$$(2)$$
$$
\overline{U}(r) \subset U(r')
$$
với mỗi cặp số dyadic $r, r'$ sao cho $0 \leq r < r' \leq 1$.

Bây giờ định nghĩa, với mỗi số thực $t \in [0, 1]$,
$$
U(t) = \bigcup_{r \leq t} U(r) \quad (r \text{ dyadic});
$$
theo (2), định nghĩa này phù hợp với định nghĩa trước đó đối với $t$ dyadic; ngoài ra, nếu $0 \leq t < t' \leq 1$, thì tồn tại hai số dyadic $r, r'$ sao cho $t \leq r < r' \leq t'$; theo (2) ta có $U(t) \subset U(r)$, do đó
$$
\overline{U}(t) \subset \overline{U}(r) \subset U(r') \subset U(t');
$$
điều này chứng minh (1) và do đó hoàn tất chứng minh.

Định lý 1 sẽ cho phép ta chỉ ra rằng hai loại quan trọng của các không gian tôpô là chuẩn tắc. Trước hết:

#### Mệnh đề 1 {#top-ix-s4-prop-1 .statement}

*Một không gian compact là chuẩn tắc.*

Một không gian compact thỏa mãn tiên đề $(\mathrm{O}'_V)$, theo Mệnh đề 2 của Chương I, § 9, no. 2.

Đối với các không gian *compact địa phương*, mỗi điểm của một không gian như vậy có một lân cận compact, là một không gian con chuẩn tắc; nhưng có những ví dụ về các không gian compact địa phương *không chuẩn tắc* (xem các Bài tập 9 và 26, và § 5, Bài tập 15).

#### Mệnh đề 2 {#top-ix-s4-prop-2 .statement}

*Một không gian mêtric hóa được là chuẩn tắc.*

Cho $X$ là một không gian mêtric hóa được và cho $d$ là một mêtric tương thích với tôpô của $X$. Cho $A, B$ là hai tập con đóng rời nhau của $X$; vì các hàm $d(x, A)$ và $d(x, B)$ là liên tục, tập hợp $U$ (tương ứng $V$) của các điểm $x$ sao cho $d(x, A) < d(x, B)$ [tương ứng $d(x, B) < d(x, A)$] là mở; rõ ràng $A \subset U$ và $B \subset V$ và $U \cap V = \varnothing$, do đó Tiên đề $(O'_V)$ được thỏa mãn.

#### Nhận xét 1 {#top-ix-s4-n1-rem-1 .statement}

Mệnh đề 2 cho một điều kiện *cần* khác cho tính mêtric hóa được; nhưng điều kiện này, ngay cả khi kết hợp với tất cả các điều kiện cần đã cho trong § 2, cũng không cho một tập hợp các điều kiện đủ cho tính mêtric hóa được (xem Bài tập 6 và § 5, Bài tập 10).
2) Có những ví dụ về các không gian chuẩn tắc không mêtric hóa được cũng không compact địa phương (xem § 5, Bài tập 16).

Theo $(O'_V)$, mọi tập hợp *đóng* của một không gian chuẩn tắc là một *không gian con chuẩn tắc*; nhưng điều này không phải lúc nào cũng đúng đối với một tập hợp *tùy ý* của một không gian chuẩn tắc.

Ví dụ, một không gian hoàn toàn chính quy không chuẩn tắc là đồng phôi với một không gian con của một không gian compact (\$ 1, no. 5, Mệnh đề 3), và không gian sau là chuẩn tắc.

Cuối cùng ta ghi nhận rằng *tích* của hai không gian chuẩn tắc không nhất thiết là chuẩn tắc (xem Bài tập 9 và § 5, Bài tập 16).

### 2. MỞ RỘNG CỦA MỘT HÀM GIÁ TRỊ THỰC LIÊN TỤC

Cho $X$ và $Y$ là hai không gian tôpô và cho $A \neq X$ là một tập con *đóng* của $X$. Nếu $f$ là một ánh xạ liên tục của $A$ vào $Y$, thì không phải lúc nào cũng có thể *mở rộng* $f$ thành một ánh xạ liên tục của toàn bộ $X$ vào $Y$. Khi $Y = \overline{\mathbf{R}}$, khả năng của một mở rộng như vậy được xác định bởi định lý sau:

#### Định lý 2 (Urysohn) {#top-ix-s4-thm-2 .statement}

*Tiên đề* $(O_V)$ *tương đương với tính chất sau*: $(O''_V)$ *Cho một tập con đóng bất kỳ* $A$ *của* $X$ *và một hàm giá trị thực liên tục bất kỳ* $f$ *(hữu hạn hoặc không)* *được xác định trên* $A$, *tồn tại một mở rộng* $g$ *của* $f$ *lên toàn bộ không gian* $X$, *là một ánh xạ liên tục của* $X$ *vào* $\overline{\mathbf{R}}$.

Dễ thấy rằng $(O''_V)$ suy ra $(O_V)$; vì nếu $B$ và $C$ là hai tập con đóng rời nhau của $X$, thì hàm bằng 0 trên $B$ và bằng $i$ trên $C$ được xác định và liên tục trên tập đóng $B \cup C$, do đó theo $(O''_{V})$ có một mở rộng liên tục $f$ lên $X$. Nếu $g = \inf (f^{+}, 1)$, thì $g$ là liên tục trên $X$, nhận các giá trị của nó trong $[0, 1]$ và bằng $o$ trên $B$ và bằng $i$ trên $C$.

Ta hãy chứng minh chiều ngược lại rằng $(O_{V})$ suy ra $(O''_{V})$. Vì $\overline{\mathbf{R}}$ và khoảng $[ -i, +i ]$ là đồng phôi, ta chỉ cần xét trường hợp ánh xạ liên tục $f : A \to \overline{\mathbf{R}}$ nhận các giá trị của nó trong $[ -i, +i ]$. Ta sẽ xây dựng một mở rộng $g$ của $f$ lên $X$ bằng cách lập một dãy $(g_{n})$ các hàm liên tục trên $X$, sao cho dãy $(g_{n}(x))$ hội tụ với mọi $x \in X$ đến một điểm của khoảng $[ -i, +i ]$; giới hạn này, theo định nghĩa, sẽ là giá trị của $g$ tại $x$, và từ sự lựa chọn các $g_{n}$ sẽ suy ra rằng hàm $g$ thỏa mãn các điều kiện yêu cầu.

Định nghĩa của $g_{n}$ dựa trên bổ đề sau:

#### Bổ đề 1 {#top-ix-s4-lem-1 .statement}

*Cho $u$ là một ánh xạ liên tục của $A$ vào $[ -i, +i ]$; khi đó tồn tại một ánh xạ liên tục $v$ của $X$ vào $[ -i/3, +i/3 ]$, sao cho $|u(x) - v(x)| \leq 2/3$ với mọi $x \in A$.*

Gọi $H$ là tập hợp tất cả các $x \in A$ sao cho $-i \leq u(x) \leq -i/3$, và gọi $K$ là tập hợp tất cả các $x \in A$ sao cho $i/3 \leq u(x) \leq i$; $H$ và $K$ là đóng trong $A$, và do đó trong $X$, và không giao nhau; vì vậy theo $(O_{V})$ tồn tại một ánh xạ liên tục $v$ của $X$ vào $[ -i/3, +i/3 ]$ bằng $-i/3$ trên $H$ và bằng $+i/3$ trên $K$. Ánh xạ $v$ thỏa mãn các điều kiện của bổ đề.

Bây giờ ta định nghĩa các hàm $g_{n}$ bằng quy nạp. Áp dụng bổ đề với $u = f$, ta định nghĩa $g_{0}$ là một ánh xạ liên tục của $X$ vào $[ -i/3, +i/3 ]$ sao cho $|f(x) - g_{0}(x)| \leq 2/3$ với mọi $x \in A$. Giả sử bây giờ rằng một ánh xạ liên tục $g_{n}$ của $X$ vào khoảng

$$
[-i + (\frac{2}{3})^{n+1}, i - (\frac{2}{3})^{n+1}]
$$

đã được định nghĩa, sao cho $|f(x) - g_{n}(x)| \leq (\frac{2}{3})^{n+1}$ với mọi $x \in A$. Áp dụng bổ đề cho hàm $u(x) = (\frac{2}{3})^{n+1} (f(x) - g_{n}(x))$, ta thấy rằng tồn tại một ánh xạ liên tục $h_{n+1}$ của $X$ vào khoảng

$$
\left[ -\frac{2^{n+1}}{3^{n+2}}, \frac{2^{n+1}}{3^{n+2}} \right]
$$

sao cho

$$
|f(x) - g_{n}(x) - h_{n+1}(x)| \leq (2/3)^{n+2}
$$

với mọi $x \in A$; phép quy nạp được hoàn thành bằng cách lấy $g_{n+1} = g_{n} + h_{n+1}$, vì hàm này thỏa mãn bất đẳng thức $|g_{n+1}(x)| \leq 1 - (2/3)^{n+2}$ với mọi $x \in X$, nhờ vào định nghĩa của $h_{n+1}$.

Từ định nghĩa này suy ra rằng, với $m \geq p$ và $n \geq p$, ta có

$$
|g_{m}(x) - g_{n}(x)| \leq \frac{2^{p+1}}{3^{p+2}} \sum_{k=0}^{\infty} (2/3)^{k} = (2/3)^{p+1}
$$

tại mỗi điểm $x \in X$; do đó dãy $(g_n(x))$ là một dãy Cauchy với mỗi $x \in X$, và vì vậy hội tụ đến một điểm $g(x)$ của khoảng $[ -1, +1 ]$; và vì $f(x) - g_n(x)$ tiến tới 0 với mọi $x \in A$ khi $n \to \infty$, $g$ là một mở rộng của $f$ lên $X$. Do đó chỉ còn phải chứng minh rằng $g$ liên tục trên $X$.

Bây giờ cho $x$ là một điểm bất kỳ của $X$; khi đó, với mọi $\varepsilon > 0$, tồn tại một số nguyên $n_0$ sao cho $|g_m(y) - g_n(y)| \leq \varepsilon$ với mọi $y \in X$ và mọi $m \geq n_0$ và mọi $n \geq n_0$; do đó, cho $m$ tiến tới $+\infty$, ta có

$$
|g(y) - g_n(y)| \leq \varepsilon.
$$

Cho $V$ là một lân cận của $x$ sao cho $|g_n(y) - g_n(x)| \leq \varepsilon$ với mọi $y \in V$; khi đó, với mỗi $y \in V$ ta sẽ có

$$
|g(y) - g(x)| \leq |g(y) - g_n(y)| + |g_n(y) - g_n(x)| + |g(x) - g_n(x)| \leq 3\varepsilon,
$$

điều này chứng tỏ rằng $g$ liên tục tại $x$, và hoàn tất chứng minh của Định lý 2. (Phần cuối của chứng minh sử dụng, trong một trường hợp riêng, ý tưởng về hội tụ đều, mà ta sẽ nghiên cứu một cách tổng quát trong Chương X, no. 1.)

#### Hệ quả {#top-ix-s4-n2-cor-1 .statement}

*Nếu $f$ là một hàm thực liên tục hữu hạn xác định trên $A$, thì tồn tại một hàm thực liên tục hữu hạn $g$ xác định trên $X$, mở rộng $f$.*

Trước hết xét trường hợp trong đó $f(x) \geq 0$ với mọi $x \in A$; khi đó có một mở rộng liên tục $g_1$ của $f$ lên $X$, nhận các giá trị của nó trong $[0, +\infty]$. Nếu đặt $B = \overline{g_1}(+\infty)$, thì $B$ là đóng và theo giả thiết không giao với $A$; do đó hàm $h$, bằng $f$ trên $A$ và bằng 0 trên $B$, là một hàm liên tục trên tập hợp đóng $A \cup B$. Cho $g_2$ là một mở rộng liên tục của $h$ lên $X$, lại nhận các giá trị của nó trong $[0, +\infty]$; khi đó hàm $g = \inf(g_1, g_2)$ là một mở rộng liên tục của $f$ lên $X$, mà các giá trị của nó là $\geq 0$ và *hữu hạn* tại mọi điểm của $X$.

Để đi tới trường hợp tổng quát, chỉ cần nhận xét rằng, nếu $f$ là hữu hạn và liên tục trên $A$, thì $f^+$ và $f^-$ cũng vậy; mở rộng $f^+$ và $f^-$ lên $X$ bằng các hàm hữu hạn liên tục $g_1$ và $g_2$ tương ứng, ta thấy rằng hàm $g_1 - g_2$ là hữu hạn và liên tục trên $X$ và mở rộng $f$.

#### Nhận xét {#top-ix-s4-n2-rem-1 .statement}

Nếu $X$ là một không gian chuẩn tắc và nếu $A$ là một tập con đóng của $X$, cũng tồn tại một mở rộng liên tục của mọi ánh xạ liên tục $f$ của $A$ vào một *khối lập phương* $K^1$ (\S 1, no. 5) lên $X$; vì khi đó ta có $f = (f_i)_{i \in I}, f_i$ là một ánh xạ liên tục của $A$ vào khoảng compact $K$ của $\mathbf{R}$; vì tồn tại một ánh xạ liên tục $g_i : X \to K$ mở rộng $f_i$, nên ánh xạ $g = (g_i)$ là một mở rộng liên tục của $f$ lên $X$.

### 3. CÁC PHỦ MỞ HỮU HẠN ĐỊA PHƯƠNG CỦA MỘT TẬP ĐÓNG TRONG MỘT KHÔNG GIAN CHUẨN TẮC

#### Định lý 3 {#top-ix-s4-thm-3 .statement}

Cho $(A_i)_{i \in I}$ là một phủ mở hữu hạn địa phương của một tập đóng $Y$ trong một không gian chuẩn tắc $X$. Khi đó tồn tại một phủ mở $(B_i)_{i \in I}$ của $Y$ sao cho $\overline{B}_i \subset A_i$ với mọi $i \in I$.

Hãy sắp thứ tự tốt tập chỉ số $I$ (Lý thuyết tập hợp, Chương III, § 2, no. 3, Định lý 1). Ta sẽ định nghĩa một họ $(B_i)_{i \in I}$ các tập mở trong $X$, bằng quy nạp siêu hạn, sao cho (i) $\overline{B}_i \subset A_i$ với mỗi $i \in I$; (ii) với mỗi $i \in I$, họ được tạo bởi các $B_\lambda$ sao cho $\lambda \leq i$ và bởi các $A_\lambda$ sao cho $\lambda > i$ là một phủ mở của $Y$. Giả sử rằng ta đã định nghĩa các $B_i$ với $i < \gamma$ sao cho (i) và (ii) được thỏa mãn với mọi $i < \gamma$, và hãy chứng minh rằng ta có thể định nghĩa $B_\gamma$ theo cách sao cho (i) và (ii) cũng được thỏa mãn đối với $i = \gamma$. Trước hết, hãy chứng minh rằng các $B_i$ với $i < \gamma$ và các $A_i$ với $i \geq \gamma$ lập thành một phủ của $Y$. Theo giả thiết, với mỗi $x \in Y$ chỉ có hữu hạn số chỉ số $\lambda \in I$ sao cho $x \in A_\lambda$, chẳng hạn $\lambda_1 < \lambda_2 < \cdots < \lambda_n$; hãy lấy $\lambda_h$ là lớn nhất trong các $\lambda_i$ sao cho $\lambda_i < \gamma$; nếu $h < n$ ta có $x \in A_{\lambda_n}$ và $\lambda_n \geq \gamma$, và nếu $h = n$ giả thiết quy nạp cho thấy rằng $x$ thuộc một $B_\lambda$ nào đó sao cho $\lambda \leq \lambda_n < \gamma$, và mệnh đề đã nêu suy ra.

Đặt $C = (\complement Y) \cup \left( \bigcup_{i < \gamma} B_i \right) \cup \left( \bigcup_{i > \gamma} A_i \right)$; $C$ là mở, và từ điều vừa nói ta có $\complement A_\gamma \subset C$; nhờ Tiên đề $(O''_V)$ đối với các không gian chuẩn tắc, do đó tồn tại một tập mở $V$ sao cho $\complement A_\gamma \subset \overline{V} \subset V \subset C$. Nếu ta đặt $B_\gamma = \complement \overline{V}$, ta có $\overline{B}_\gamma \subset \complement V \subset A_\gamma$ và $B_\gamma \cup C = X$, do đó các $B_i$ sao cho $i \leq \gamma$ và các $A_i$ sao cho $i > \gamma$ phủ $Y$.

#### Nhận xét {#top-ix-s4-n3-rem-1 .statement}

Chú ý rằng ta chỉ dùng thực tế là phủ $(A_i)$ là hữu hạn theo điểm, tức là mỗi điểm của $X$ chỉ thuộc về một số hữu hạn các tập $A_i$.

#### Định nghĩa 2 {#top-ix-s4-def-2 .statement}

Cho $X$ là một không gian tôpô và cho $f$ là một hàm giá trị thực xác định trên $X$. Giá đỡ của $f$, ký hiệu bởi $\operatorname{Supp}(f)$, là tập đóng nhỏ nhất $S$ trong $X$ sao cho $f(x) = 0$ với mọi $x \notin S$.

Nói cách khác, $\operatorname{Supp}(f)$ là bao đóng trong $X$ của tập tất cả các $x \in X$ sao cho $f(x) \neq 0$; hay một lần nữa, đó là tập tất cả các $x \in X$ sao cho mọi lân cận của $x$ đều chứa một điểm $y$ sao cho $f(y) \neq 0$.

Cho $(f_i)_{i \in I}$ là một họ các hàm giá trị thực hữu hạn trên $X$ mà các giá đỡ của chúng tạo thành một họ hữu hạn địa phương; khi đó tổng $\sum_{i \in I} f_i(x)$ được xác định với mỗi $x \in X$ (vì nó chỉ chứa hữu hạn số hạng khác không). Hàm giá trị thực hữu hạn $x \to \sum_{i \in I} f_i(x)$ được gọi là tổng của họ $(f_i)$, và được ký hiệu bởi $\sum_{i \in I} f_i$. Nếu mỗi $f_i$ đều liên tục, thì $f = \sum_{i \in I} f_i$ cũng liên tục; thật vậy, nếu $x$ là một điểm bất kỳ của $X$, thì có một lân cận $V$ của $x$ chỉ gặp một số hữu hạn các giá đỡ của các $f_i$, và do đó có một tập con hữu hạn $H$ của $I$ sao cho $f(y) = \sum_{i \in H} f_i(y)$ với mọi $y \in V$.

#### Định nghĩa 3 {#top-ix-s4-def-3 .statement}

*Cho một họ* $(A_i)_{i \in I}$ *của các tập con của một không gian tôpô* $X$, *một họ* $(f_i)_{i \in I}$ *của các hàm giá trị thực xác định trên* $X$ *được gọi là phụ thuộc vào họ* $(A_i)_{i \in I}$ *nếu ta có* $\operatorname{Supp}(f_i) \subset A_i$ *với mỗi chỉ số* $i \in I$.

*Một phân hoạch đơn vị liên tục trên* $X$ *là bất kỳ họ nào* $(f_i)_{i \in I}$ *gồm các hàm liên tục giá trị thực* $\geq 0$ *trên* $X$ *mà các giá đỡ của chúng tạo thành một họ hữu hạn địa phương và sao cho* $\sum_{i \in I} f_i(x) = 1$ *với mọi* $x \in X$.

#### Mệnh đề 3 {#top-ix-s4-prop-3 .statement}

*Cho bất kỳ một phủ mở hữu hạn địa phương nào* $(A_i)_{i \in I}$ *của một không gian chuẩn tắc* $X$, *tồn tại một phân hoạch đơn vị liên tục* $(f_i)_{i \in I}$ *trên* $X$, *phụ thuộc vào phủ* $(A_i)_{i \in I}$.

Theo Định lý 3 tồn tại một phủ mở $(B_i)_{i \in I}$ của $X$ sao cho $\overline{B}_i \subset A_i$ với mỗi $i \in I$, và rõ ràng phủ $(B_i)$ là hữu hạn địa phương. Theo tiên đề $(O''_V)$, với mỗi $i \in I$ tồn tại một tập mở $C_i$ sao cho $\overline{B}_i \subset C_i \subset \overline{C}_i \subset A_i$. Theo tiên đề $(O_V)$, với mỗi $i \in I$ tồn tại một ánh xạ liên tục $g_i$ của $X$ vào $[0,1]$, sao cho $g_i(x) = 1$ trên $\overline{B}_i$ và sao cho giá đỡ của $\overline{g}_i$ được chứa trong $\overline{C}_i$, và do đó được chứa trong $A_i$. Vì $(B_i)$ là một phủ của $X$, ta có $\sum_{i \in I} g_i(x) > 0$ với mỗi $x \in X$; nếu đặt
$$
f_i(x) = \frac{g_i(x)}{\sum_{i \in I} g_i(x)}
$$
đối với mọi $i \in I$ và mọi $x \in X$, thì các $f_i$ tạo thành một phân hoạch đơn vị liên tục phụ thuộc vào phủ $(A_i)$.

#### Hệ quả {#top-ix-s4-n3-cor-1 .statement}

*Cho bất kỳ một phủ mở hữu hạn địa phương* $(A_i)$ *của một tập đóng* $F$ *trong một không gian chuẩn tắc* $X$, *tồn tại một họ* $(f_i)$ *các hàm liên tục nhận giá trị thực* $\geq 0$ *trên* $X$, *phụ thuộc vào phủ* $(A_i)_{i \in I}$ *và sao cho* $\sum_{i \in I} f_i(x) = 1$ *với mọi* $x \in F$ *và* $\sum_{i \in I} f_i(x) \leq 1$ *với mọi* $x \in X$.

Họ các tập hợp gồm CF và các $A_i$ là một phủ mở hữu hạn địa phương của $X$. Vì vậy tồn tại một phân hoạch đơn vị liên tục phụ thuộc vào phủ này, gồm một họ $(f_i)_{i \in I}$ sao cho $\operatorname{Supp}(f_i) \subset A_i$ với mỗi $i \in I$, và một hàm $g$ có giá đỡ được chứa trong phần bù của $F$. Họ $(f_i)$ rõ ràng thỏa các điều kiện cần thiết.

### 4. CÁC KHÔNG GIAN PARACOMPACT

Ta nhắc lại (Chương I, § 9, no. 10) rằng một không gian tôpô $X$ được gọi là *paracompact* nếu nó là Hausdorff và nếu mọi phủ mở của $X$ đều có một tinh chỉnh mở hữu hạn địa phương.

#### Mệnh đề 4 {#top-ix-s4-prop-4 .statement}

*Mọi không gian paracompact đều là chuẩn tắc.*

Đây là hệ quả của bổ đề sau:

#### Bổ đề 2 {#top-ix-s4-lem-2 .statement}

*Cho $A, B$ là hai tập hợp con đóng rời nhau của một không gian paracompact $X$. Nếu với mỗi $x \in A$ có một lân cận mở $V_x$ của $x$ và một lân cận mở $W_x$ của $B$ sao cho chúng không giao nhau, thì tồn tại một lân cận mở $T$ của $A$ và một lân cận mở $U$ của $B$ sao cho chúng không giao nhau.*

Tạm thời giả sử bổ đề này đúng, ta có thể áp dụng nó trong trường hợp $B$ gồm một điểm duy nhất, vì $X$ là Hausdorff, và khi đó điều đó cho thấy $X$ là *chính quy*. Khi đó ta lại có thể áp dụng Bổ đề 2 cho bất kỳ hai tập hợp con đóng rời nhau nào của $X$, và điều này cho thấy Tiên đề $(O'_V)$ được thỏa mãn.

Để chứng minh bổ đề, xét phủ mở của $X$ gồm $CA$ và các $V_x$, với $x \in A$; hãy lấy $(T_i)_{i \in I}$ là một phủ tinh mở hữu hạn địa phương của phủ này. Khi đó, theo định nghĩa, nếu $A \cap T_i \neq \emptyset$ thì tồn tại $x_i \in A$ sao cho $T_i \subset V_{x_i}$. Cho $T$ là tập mở là hợp của các $T_i$ giao với $A$, và hãy chứng minh rằng tồn tại một lân cận mở $U$ của $B$ không giao với $T$. Với mỗi $y \in B$ có một lân cận mở $S_y$ của $y$ chỉ giao với hữu hạn tập hợp $T_i$; hãy lấy $J$ là tập con hữu hạn của $I$ gồm những chỉ số $i$ sao cho $T_i$ giao với cả $S_y$ và $A$; nếu ta đặt $U_y = S_y \cap \bigcap_{i \in J} W_{x_i}$, thì $U_y$ là một lân cận mở của $y$ không giao với bất kỳ $T_i$ nào giao với $A$, và do đó $U_y \cap T = \emptyset$. Đặt $U = \bigcup_{y \in B} U_y$; khi đó $U'$ là một lân cận mở của $B$ không giao với $T$, và bổ đề được chứng minh.

Có những không gian chuẩn tắc không paracompact (Bài tập 19).

#### Hệ quả 1 {#top-ix-s4-lem-2-cor-1 .statement}

*Cho bất kỳ phủ mở $(A_i)_{i \in I}$ nào của một không gian paracompact $X$, tồn tại một phân hoạch đơn vị liên tục $(f_i)_{i \in I}$ trên $X$, phụ thuộc vào phủ $(A_i)$.*

Cho $(U_\lambda)_{\lambda \in L}$ là một phủ mở hữu hạn địa phương của $X$ tinh hơn phủ $(A_i)_{i \in I}$; khi đó có một ánh xạ $\varphi : L \to I$ sao cho $U_\lambda \subset A_{\varphi(\lambda)}$ với mỗi $\lambda \in L$. Theo các Mệnh đề 3 và 4, tồn tại một phân hoạch đơn vị liên tục $(g_\lambda)_{\lambda \in L}$ phụ thuộc vào $(U_\lambda)$. Với mỗi $i \in I$, đặt

$$
f_i = \sum_{\varphi(\lambda) = i} g_\lambda;
$$

Tổng này được xác định và liên tục vì các giá đỡ của các $g_\lambda$ tạo thành một phủ hữu hạn địa phương; hơn nữa, hợp $B_i$ của các giá đỡ của các $g_\lambda$ sao cho $\varphi(\lambda) = i$ là đóng, theo Mệnh đề 4 của Chương I, § 1, no. 6, và được chứa trong $A_i$. Vì ta có $f_i(x) = 0$ mỗi khi $x \in \mathbf{C}B_i$, nên giá đỡ của $f_i$ được chứa trong $B_i$, và do đó trong $A_i$. Mặt khác, họ $B_i$ là hữu hạn địa phương, vì với mỗi $x \in X$ có một lân cận $V$ của $x$ và một tập con hữu hạn $H$ của $I$ sao cho $V \cap U_\lambda = \emptyset$ với mọi $\lambda \notin H$, và do đó suy ra rằng $V \cap B_i = \emptyset$ với mọi $i \notin \varphi(H)$. Cuối cùng, với mỗi $x \in X$ ta có

$$
1 = \sum_{\lambda \in L} g_\lambda(x) = \sum_{i \in I} \left( \sum_{\varphi(\lambda) = i} g_\lambda(x) \right) = \sum_{i \in I} f_i(x),
$$

và chứng minh đã hoàn tất.

#### Hệ quả 2 {#top-ix-s4-lem-2-cor-2 .statement}

*Nếu $F$ là một tập con đóng của một không gian paracompact $X$, thì mọi lân cận của $F$ trong $X$ đều chứa một lân cận đóng (và do đó paracompact) của $F$.*

Theo Mệnh đề 16 của Chương I, § 9, no. 10, mọi không gian con đóng của $X$ đều paracompact; do đó hệ quả suy ra từ Mệnh đề 4 và Tiên đề $(O_v')$.

### 5. TÍNH PARACOMPACT CỦA CÁC KHÔNG GIAN MÊTRIC HÓA

Định lý sau đây là một kết quả mạnh hơn của Mệnh đề 2 ở no. 1:

#### Định lý 4 {#top-ix-s4-thm-4 .statement}

*Mọi không gian mêtric hóa đều paracompact.*

Định lý này là hệ quả của bốn bổ đề sau đây.

#### Bổ đề 3 {#top-ix-s4-lem-3 .statement}

*Cho $\mathcal{R} = (U_\alpha)_{\alpha \in A}$ là một phủ mở của một không gian mêtric hóa X. Khi đó có một dãy $(\mathcal{G}_n)$ của các họ hữu hạn địa phương gồm các tập con mở của X, sao cho $\mathcal{S} = \bigcup_n \mathcal{S}_n$ là một phủ mở của X tinh hơn $\mathcal{R}$.

Cho $d$ là một khoảng cách trên X tương thích với tôpô của nó. Với mỗi $\alpha \in A$ và mỗi số nguyên $n$, ký hiệu $F_{n\alpha}$ là tập gồm mọi $x \in U_\alpha$ sao cho $d(x, X - U_\alpha) \geq 2^{-n}$. Vì $X - U_\alpha$ là đóng, ta có $U_\alpha = \bigcup_n F_{n\alpha}$.

Sắp thứ tự tốt tập hợp $A$; với mỗi $\alpha \in A$ và mỗi số nguyên $n$, gọi $G_{n\alpha}$ là tập hợp mọi $x \in F_{n\alpha}$ sao cho $x \notin F_{n+1,\beta}$ với mọi $\beta < \alpha$, và gọi $V_{n\alpha}$ là tập hợp mọi $y \in X$ sao cho $d(y, G_{n\alpha}) > 2^{-n-3}$. $V_{n\alpha}$ rõ ràng là một tập mở; mặt khác, $V_{n\alpha} \subset U_\alpha$, vì với mỗi $y \in V_{n\alpha}$ tồn tại $x \in G_{n\alpha}$ sao cho $d(x, y) \leq 2^{-n-1}$, và vì $x \in F_{n\alpha}$, ta có

$$
d(y, X - U_\alpha) \geq d(x, X - U_\alpha) - d(x, y) \geq 2^{-n-1},
$$

do đó $y \in U_\alpha$. Hơn nữa, với mỗi $x \in X$ hãy cho $\alpha$ là chỉ số nhỏ nhất trong $A$ sao cho $x \in U_\alpha$; khi đó tồn tại một số nguyên n sao cho $x \in F_{n\alpha}$, và theo định nghĩa của $\alpha$ suy ra $x \in G_{n\alpha}$, nên $x \in V_{n\alpha}$. Điều này cho thấy rằng nếu ta đặt $\mathfrak{S}_n = (V_{n\alpha})_{\alpha \in A}$, thì $\mathfrak{S} = \bigcup_n \mathfrak{S}_n$ là một phủ mở của $X$ tinh lọc $\mathcal{R}$; vì vậy còn phải chứng minh rằng mỗi họ $\mathfrak{S}_n$ là *hữu hạn địa phương*. Để làm điều này trước hết ta sẽ chứng minh rằng $d(G_{n\alpha}, G_{n\beta}) \geq 2^{-n-1}$ nếu $\alpha \neq \beta$. Giả sử rằng $\beta < \alpha$; khi đó nếu $x \in G_{n\alpha}$ và $y \in F_{n\beta}$ thì theo định nghĩa ta có $x \notin F_{n+1,\beta}$, do đó $d(x, X - U_\beta) < 2^{-n-1}$ và $d(y, X - U_\beta) \geq 2^{-n}$, và vì thế $d(x, y) \geq 2^{-n-1}$; vì $G_{n\beta} \subset F_{n\beta}$, mệnh đề suy ra. Từ đó suy ra ngay, dùng định nghĩa của $V_{n\alpha}$ và $V_{n\beta}$, rằng $d(V_{n\alpha}, V_{n\beta}) \geq 2^{-n-2}$. Từ bất đẳng thức sau cùng này ta suy ra rằng, với mỗi $z \in X$, quả cầu mở tâm $z$ và bán kính $2^{-n-3}$ gặp nhiều nhất một tập của họ $\mathfrak{S}_n$; do đó $\mathfrak{S}_n$ là một họ hữu hạn địa phương, và chứng minh hoàn tất.

#### Bổ đề 4 {#top-ix-s4-lem-4 .statement}

*Cho* $(\mathfrak{S}_n)$ *là một dãy các họ hữu hạn địa phương của các tập mở trong một không gian tôpô* $X$, *sao cho*
$$
\mathfrak{S} = \bigcup_n \mathfrak{S}_n
$$
*là một phủ của* $X$. *Khi đó tồn tại một phủ hữu hạn địa phương (nhưng không nhất thiết mở)* $\mathcal{B}$ *của* $X$ *tinh lọc* $\mathfrak{S}$.

Cho $E_n$ là tập hợp mở trong $X$ là hợp của tất cả các tập hợp của $\mathfrak{S}_n$; cho $U_n$ ký hiệu $\bigcup_{k=1}^n E_k$ và cho $A_n$ ký hiệu $U_n - U_{n-1}$ (với $U_0 = \varnothing$). Xét tập hợp $\mathcal{B}$ gồm các tập hợp con $V \cap A_n$, trong đó $V \in \mathfrak{S}_n$ và $n$ là bất kỳ số nguyên nào; ta sẽ chứng minh rằng $\mathcal{B}$ thỏa mãn các điều kiện của bổ đề. Với mỗi $x \in X$ có một số nguyên $n$ sao cho $x \in A_n$, vì các $A_n$ tạo thành một phân hoạch của $X$; do đó $x \in E_n$ và tồn tại $V \in \mathfrak{S}_n$ sao cho $x \in V$; suy ra $x \in V \cap A_n$, và ta đã chứng minh rằng $\mathcal{B}$ là một phủ của $X$. Rõ ràng, phủ này tinh hơn $\mathfrak{S}$. Mặt khác, với mỗi $x \in X$ tồn tại một số nguyên $n$ sao cho $x \in U_n$; vì $U_n$ là mở và các $\mathfrak{S}_m$ là các họ hữu hạn địa phương, nên với mỗi $m$ tồn tại một lân cận $W_m$ của $x$, được chứa trong $U_n$, chỉ gặp một số hữu hạn các tập hợp của $\mathfrak{S}_m$; do đó lân cận $W = \bigcap_{m=1}^n W_m$ của $x$ chỉ gặp một số hữu hạn các tập hợp của $\mathcal{B}$, vì $W \cap A_p = \varnothing$ với $p > n$. Vậy $\mathcal{B}$ là hữu hạn địa phương, và Bổ đề 4 được chứng minh.

#### Bổ đề 5 {#top-ix-s4-lem-5 .statement}

*Cho* $X$ *là một không gian chính quy sao cho, với mỗi phủ mở* $\mathcal{R}$ *của* $X$, *tồn tại một phủ (không nhất thiết mở) hữu hạn địa phương* $\mathcal{U}$ *của* $X$ *tinh hơn* $\mathcal{R}$. *Khi đó với mỗi phủ mở* $\mathcal{R}$ *của* $X$ *tồn tại một phủ đóng hữu hạn địa phương* $\mathfrak{F}$ *của* $X$ *tinh hơn* $\mathcal{R}$.

Let $\mathcal{H}$ là một phủ mở bất kỳ của $X$. Với mỗi $x \in X$ có một tập mở $U \in \mathcal{H}$ chứa $x$, và do đó (vì $X$ chính quy) có một lân cận mở $V_x$ của $x$ sao cho $\overline{V}_x \subset U$. Họ $\mathcal{B}$ được tạo bởi các $V_x$ là một phủ mở của $X$, nên theo giả thiết tồn tại một phủ hữu hạn địa phương $\mathcal{B}'$ mịn hơn $\mathcal{B}$. Gọi $\mathcal{F}$ là họ các bao đóng của các tập thuộc $\mathcal{B}$. Vì phủ $\mathcal{B}'$ được tạo bởi các $\overline{V}_x$ mịn hơn $\mathcal{H}$, và vì $\mathcal{F}$ mịn hơn $\mathcal{B}'$, suy ra $\mathcal{F}$ là một phủ đóng của $X$ mịn hơn $\mathcal{H}$. Nhưng $\mathcal{F}$ cũng là hữu hạn địa phương, vì nếu một tập mở không gặp một tập $B \in \mathcal{B}$, thì nó cũng không gặp bao đóng $\overline{B}$ của nó.

#### Bổ đề 6 {#top-ix-s4-lem-6 .statement}

*Cho $X$ là một không gian Hausdorff sao cho, với mọi phủ mở $\mathcal{H}$ của $X$, tồn tại một phủ đóng hữu hạn địa phương $\mathcal{F}$ của $X$ mịn hơn $\mathcal{H}$. Khi đó $X$ là paracompact.*

Cho $\mathcal{H}$ là một phủ mở bất kỳ của $X$. Ta phải chứng minh rằng tồn tại một phủ mở hữu hạn địa phương của $X$ tinh lọc $\mathcal{H}$. Cho $\mathcal{A}$ là một phủ hữu hạn địa phương (đóng hay không đóng) của $X$ tinh lọc $\mathcal{H}$; với mỗi $x \in X$, cho $W_x$ là một lân cận mở của $x$ chỉ giao với một số hữu hạn tập của $\mathcal{A}$. Họ $\mathcal{W}$ gồm các tập $W_x$ là một phủ mở của $X$. Cho $\mathcal{F}$ là một phủ *đóng* hữu hạn địa phương của $X$ tinh lọc $\mathcal{W}$. Với mỗi $A \in \mathcal{A}$, cho $U_A$ là một tập của $\mathcal{H}$ chứa $A$, và cho $C_A$ là hợp của các tập $F \in \mathcal{F}$ sao cho $A \cap F = \varnothing$. Vì $\mathcal{F}$ là hữu hạn địa phương, $C_A$ là đóng trong $X$ (Chương I, § 1, no. 6, Mệnh đề 4) và do đó $A' = U_A \cap (X - C_A)$ là mở. Vì ta có $A \cap C_A = \varnothing$ và $A \subset U_A$, suy ra $A \subset A'$, và họ $\mathcal{A}'$ gồm các tập $A'$, khi $A$ chạy qua $\mathcal{A}$, là một phủ mở của $X$; hơn nữa, vì $A' \subset U_A \in \mathcal{H}$, $\mathcal{A}'$ tinh lọc $\mathcal{H}$. Còn phải chứng minh rằng $\mathcal{A}'$ là *hữu hạn địa phương*. Với mỗi $x \in X$ có một lân cận $T$ của $x$ chỉ giao với một số hữu hạn tập của $\mathcal{F}$, chẳng hạn $F_1, \ldots, F_n$. Vì mỗi $F_i$ được chứa trong một tập có dạng $W_{y_i}$, nên theo định nghĩa $F_i$ chỉ giao với một số hữu hạn tập của $\mathcal{A}$; cho $A_{ij}$ ($1 \leq j \leq s_i$) là các tập ấy. Nếu $A$ là một tập của $\mathcal{A}$ khác với một trong các $A_{ij}$ ($1 \leq i \leq n,\ 1 \leq j \leq s_i$), thì từ các định nghĩa suy ra rằng $A'$ không giao với tập nào trong các $F_i$, và do đó không giao với $T \subset \bigcup_{i=1}^n F_i$. Điều đó hoàn tất chứng minh của Bổ đề 6 và của Định lý 4.

### Bài tập {#top-ix-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
