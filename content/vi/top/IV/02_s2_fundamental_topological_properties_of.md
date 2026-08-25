---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 2
section_title: Fundamental topological properties of the real line
lang: vi
source: top-i-iv
pdf_pages: 0340-0345, 0387-0393
extraction: ocr
subsections:
    - "no": 1
      title: ARCHIMEDES' AXIOM
      page: 0
      pdf_page: 340
    - "no": 2
      title: COMPACT SUBSETS OF $\mathbf{R}$
      page: 0
      pdf_page: 341
    - "no": 3
      title: LEAST UPPER BOUND OF A SUBSET OF $\mathbf{R}$
      page: 0
      pdf_page: 341
    - "no": 4
      title: CHARACTERIZATION OF INTERVALS
      page: 0
      pdf_page: 342
    - "no": 5
      title: CONNECTED SUBSETS OF $\mathbf{R}$
      page: 0
      pdf_page: 342
    - "no": 6
      title: HOMEOMORPHISMS OF AN INTERVAL ONTO AN INTERVAL
      page: 0
      pdf_page: 344
statements: 15
exercises: 16
content_sha256: 35c6486ac1a3fa336ad8eb84fdd613f3a737c0ba448469612b56d2e4a70ae008
translated_from: content/en/top/IV/02_s2_fundamental_topological_properties_of.md
source_content_sha256: 6696bb5fa08accd0b6144828d1d539cb5024a066162e459953b37132c7805a3d
translation_model: gpt-5.4
translation_run: translate-vi-264ae25a
glossary_version: 34
glossary_terms_sha256: 784d062be9ed364f2ca6c18d4e6ca42fa119aa2c307f3f3dfd50ff77607550d6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. CÁC TÍNH CHẤT TÔPÔ CƠ BẢN CỦA ĐƯỜNG THẲNG THỰC

### 1. TIÊN ĐỀ ARCHIMEDES

Các tính chất tôpô của đường thẳng thực là đối tượng của tiết này đều là hệ quả của định lý sau đây:

#### Định lý 1 {#top-iv-s2-thm-1 .statement}

*Nếu $x$ và $y$ là hai số thực bất kỳ > 0, thì tồn tại một số nguyên $n > 0$ sao cho $y < nx$.*

Tồn tại hai số hữu tỉ $p/q$ và $r/s$ sao cho $0 < p/q < x$ và $y < r/s$, vì các khoảng mở ]$0, x$ và ]$y, \to$ là không rỗng ($\S$ I, no. 4, Mệnh đề 4); lấy $n$ sao cho $nps > qr$, và ta có $y < nx$.

#### Nhận xét {#top-iv-s2-n1-rem-1 .statement}

Một phép dựng tiên đề của lý thuyết số thực sẽ được trình bày trong Chương V, $\S$ 2, trong đó Định lý 1 xuất hiện như một tiên đề; để biết thêm chi tiết về tiên đề này, xem Ghi chú lịch sử của Chương IV.

### 2. CÁC TẬP CON COMPACT CỦA $\mathbf{R}$

#### Định lý 2 (Borel-Lebesgue) {#top-iv-s2-thm-2 .statement}

Điều kiện cần và đủ để một tập con của đường thẳng thực $\mathbf{R}$ là compact là nó đóng và bị chặn.

1) Điều kiện là cần thiết. Cho $A$ là một tập con compắc của $\mathbf{R}$ và cho $a$ là một số thực $> 0$. Tập hợp $A$ là đóng (Chương I, $\S$ 9, no. 3, Mệnh đề 4) và tồn tại một số hữu hạn điểm $x_i$ ($1 \leq i \leq n$) của $\mathbf{R}$ sao cho $A$ được chứa trong hợp của các lân cận $[x_i - a, x_i + a]$ (Chương I, $\S$ 9, no. 3). Gọi $b$ là giá trị lớn nhất của các số $|x_i|$; khi đó ta có $A \subset [-b - a, b + a]$.

2) Điều kiện là đủ. Chỉ cần chứng tỏ rằng mọi khoảng $[ -a, +a ]$ ($a > 0$) đều compắc, và vì khoảng này là một tập con đóng của một không gian đều đầy đủ, chỉ cần chứng tỏ rằng, với mỗi $b > 0$, ta có thể phủ $[ -a, +a ]$ bởi một số hữu hạn các khoảng có dạng $[x - b, x + b]$ (Chương II, $\S$ 4, no. 2, Hệ quả của Định lý 3). Bây giờ, cho $n$ là một số nguyên $> 0$ sao cho $a < nb$; nếu $x \in [ -a, +a ]$ và nếu $m$ là số nguyên lớn nhất (dương hoặc âm) sao cho $mb \leq x$, thì ta có $-n \leq m \leq n$ và $mb \leq x \leq (m + 1)b$. Do đó $2n + 1$ khoảng $[ (k - 1)b, (k + 1)b ]$ ($-n \leq k \leq n$) lập thành một phủ thuộc kiểu đã yêu cầu.

#### Hệ quả 1 {#top-iv-s2-thm-2-cor-1 .statement}

Một tập con của đường thẳng thực $\mathbf{R}$ là compact tương đối nếu và chỉ nếu nó bị chặn.

#### Hệ quả 2 {#top-iv-s2-thm-2-cor-2 .statement}

Đường thẳng thực là một không gian compact địa phương và không compact.

#### Nhận xét {#top-iv-s2-n2-rem-1 .statement}

Định lý 2 thường được gọi là "Định lý Heine-Borel"; xem các Ghi chú lịch sử của Chương II và IV.

### 3. CẬN TRÊN BÉ NHẤT CỦA MỘT TẬP CON CỦA $\mathbf{R}$

#### Định lý 3 {#top-iv-s2-thm-3 .statement}

Mọi tập con không rỗng của đường thẳng thực bị chặn trên (resp. bị chặn dưới) đều có một cận trên bé nhất (resp. cận dưới lớn nhất).

Cho $A$ là một tập con không rỗng của $\mathbf{R}$, bị chặn trên, và cho $b$ là một cận trên của $A$, sao cho $A \subset ]\leftarrow, b]$. Với mỗi $x \in A$ xét tập hợp $A_x$ gồm các số $\geqslant x$ thuộc $A$; các tập hợp $A_x$ tạo thành một cơ sở lọc $\mathcal{B}$ trên $\mathbf{R}$, vì $A_y \subset A_x$ nếu $y \geqslant x$. Cho $a$ là một điểm của $A$. Với mỗi $x \geqslant a$ thuộc $A$, $A_x$ được chứa trong khoảng compact $[a, b]$ và do đó cơ sở lọc $\mathcal{B}$ có một điểm tụ $c$. Vì các khoảng $[x, \rightarrow[$ là đóng, $c$ thuộc giao của chúng và vì vậy $c$ là một cận trên của $A$. Nhưng, mặt khác, mọi cận trên $z$ của $A$ đều $\geqslant c$, nếu không thì lân cận $]z, \rightarrow[$ của $c$ sẽ không chứa điểm nào của $A$. Vậy $c$ là cận trên bé nhất của $A$.

Ta có thể lập luận tương tự cho một tập hợp khác rỗng $B$ bị chặn dưới, hoặc đơn giản nhận xét rằng $-B$ là khác rỗng và bị chặn trên, và nếu $c$ là cận trên nhỏ nhất của $-B$, thì $-c$ là cận dưới lớn nhất của $B$.

Cận trên nhỏ nhất $c$ của $A$ có thể được đặc trưng hóa bởi hai tính chất sau:
(i) Với mỗi $x \in A, x \leqslant c_*$.
(ii) Với mỗi $a < c$, tồn tại $x \in A$ sao cho $a < x \leqslant c$.

Cận trên nhỏ nhất của một tập đóng (khác rỗng và bị chặn trên) thuộc về tập hợp đó và là phần tử lớn nhất của nó; và cận trên nhỏ nhất của mọi tập con khác rỗng $A$ của $\mathbf{R}$ bị chặn trên có thể được định nghĩa là số thực lớn nhất trong bao đóng của $A$.

### 4. ĐẶC TRƯNG HÓA CÁC KHOẢNG

#### Mệnh đề 1 {#top-iv-s2-prop-1 .statement}

*Một tập con không rỗng $A$ của $\mathbf{R}$ là một khoảng khi và chỉ khi, hễ $a$ và $b$ là hai điểm bất kỳ của $A$ sao cho $a < b$, thì khoảng đóng $[a, b]$ được chứa trong $A$*.

Điều kiện ấy rõ ràng là cần thiết. Ngược lại, giả sử rằng nó được thỏa mãn. Nếu $A$ không bị chặn trên cũng không bị chặn dưới thì nó phải là toàn bộ $\mathbf{R}$, vì nếu $x$ là một điểm bất kỳ của $\mathbf{R}$ thì khi đó có hai điểm $a, b$ của $A$ sao cho $a < x < b$. Nếu $A$ bị chặn trên nhưng không bị chặn dưới, gọi $k$ là cận trên bé nhất của nó; khi đó với mọi $x < k$ tồn tại $a$ và $b$ trong $A$ sao cho $a < x < b \leqslant k$, do đó $x \in A$, và vì thế $A$ chỉ có thể là một trong hai khoảng $]\leftarrow, k], ]\leftarrow, k[$. Lập luận cũng tương tự trong các trường hợp khác.

### 5. CÁC TẬP CON LIÊN THÔNG CỦA $\mathbf{R}$

#### Định lý 4 {#top-iv-s2-thm-4 .statement}

*Một tập con $A$ của $\mathbf{R}$ là liên thông khi và chỉ khi $A$ là một khoảng.*

i) Điều kiện là cần thiết. Giả sử $A$ liên thông: nếu $A$ chỉ gồm một điểm, thì nó là một khoảng. Nếu $A$ có nhiều hơn một điểm, lấy $a$ và $b$ là hai điểm của $A$ sao cho $a < b$; theo Mệnh đề 1 của no. 4, chỉ cần chứng minh rằng mọi $x$ sao cho $a < x < b$ đều thuộc $A$. Bây giờ, nếu $x \notin A$ thì ta sẽ có $A \subset C\{x\}$; nhưng $C\{x\}$ là hợp của hai tập mở rời nhau ]$\leftarrow, x[$ và $]x, \rightarrow[$, mà mỗi tập trong hai tập đó đều gặp $A$, và vì thế $A$ sẽ không liên thông, trái với giả thiết.

2) Điều kiện là *đủ*. Trước hết ta hãy chỉ ra rằng mọi khoảng *compắc* $[a, b]$ đều liên thông. Với mỗi số nguyên $n > 0$, gọi $V_{1/n}$ là lân cận gồm tất cả các cặp $(x, y)$ sao cho $|x - y| \leq 1/n$; theo Mệnh đề 6 của Chương II, § 4, no. 4, chỉ cần chỉ ra rằng mọi cặp điểm $x, y$ của $[a, b]$ đều có thể được nối bởi một xích $V_{1/n}$. Gọi $p$ là số nguyên lớn nhất sao cho $p/n \leq x$ và gọi $q$ là số nguyên lớn nhất sao cho $q/n \leq y$ ($p$ và $q$ tồn tại theo Định lý 1 của no. 1); khi đó $p \leq q$. Nếu $p = q$ thì $y - x < 1/n$ và các điểm $x$ và $y$ tạo thành một xích $V_{1/n}$. Nếu $q > p$, đặt $x_i = (p + i)/n$ ($i = 1, 2, \ldots, q - p$); ta có $x_1 - x \leq 1/n$, $y - x_{q-p} \leq 1/n$ và $x_{i+1} - x_i = 1/n$, do đó các điểm $x, x_1, x_2, \ldots, x_{q-p}, y$ tạo thành một xích $V_{1/n}$ nối $x$ và $y$.

Nếu bây giờ $I$ là một khoảng bất kỳ không gồm một điểm duy nhất, và nếu $a$ và $b$ là hai điểm bất kỳ của $I$ sao cho $a < b$, thì khoảng $[a, b]$ được chứa trong $I$ và là liên thông, do đó $I$ là liên thông.

#### Hệ quả 1 {#top-iv-s2-thm-4-cor-1 .statement}

*Đường thẳng thực là một không gian liên thông và địa phương liên thông.*

#### Hệ quả 2 {#top-iv-s2-thm-4-cor-2 .statement}

*Các tập con compact liên thông duy nhất của $\mathbf{R}$ là các khoảng đóng bị chặn.*

Theo Định lý 4, một tập con của $\mathbf{R}$ không chứa bất kỳ khoảng nào gồm nhiều hơn một điểm thì *hoàn toàn không liên thông*; điều này đúng, chẳng hạn, với tập $\mathbf{Q}$ các số hữu tỉ, vì tập $C\mathbf{Q}$ các số vô tỉ là trù mật trong $\mathbf{R}$.

#### Mệnh đề 2 {#top-iv-s2-prop-2 .statement}

*Mọi tập mở không rỗng trong $\mathbf{R}$ là hợp của một họ đếm được các khoảng mở đôi một rời nhau.*

Cho $A$ là một tập hợp mở không rỗng trong $\mathbf{R}$. Vì $\mathbf{R}$ liên thông địa phương, mọi *thành phần* của $A$ là một tập hợp mở liên thông (Chương I, § 11, no. 6, Mệnh đề 11) và do đó là một *khoảng mở* theo Định lý 4. Hai khoảng mở bất kỳ trong các khoảng này là rời nhau; mặt khác, mỗi khoảng trong chúng đều chứa một số hữu tỉ; vì thế tập hợp các khoảng này có lũy thừa nhỏ hơn hoặc bằng lũy thừa của $\mathbf{Q}$, tức là *đếm được*.

Suy ra mọi tập hợp đóng trong $\mathbf{R}$ là phần bù của hợp của một dãy $(I_n)$ hữu hạn hoặc vô hạn gồm các khoảng mở đôi một rời nhau. Các khoảng này được gọi là *kề* với tập hợp đóng đang xét. Ngược lại, cho một dãy khoảng như vậy, phần bù của hợp của chúng là một tập hợp đóng mà các khoảng ấy kề với nó.

#### Ví dụ {#top-iv-s2-n5-exa-1 .statement}

Hãy định nghĩa bằng quy nạp một họ đếm được $(I_{n,p})$ các khoảng mở đôi một rời nhau như sau:
Số nguyên $n$ nhận mọi giá trị $\geqslant 0$, và với mỗi giá trị của $n$, $p$ nhận các giá trị $1, 2, 3, \ldots, 2^n$. Mọi khoảng $I_{n,p}$ đều được chứa trong
$$
A = [0, 1],
$$
và ta lấy $I_{0,1} = ]1/3, 2/3[$ ("một phần ba ở giữa" của $]0, 1[$). Bây giờ giả sử rằng $2^{m+1} - 1$ khoảng $I_{n,p}$ đã được định nghĩa với $0 \leq n \leq m$ sao cho, nếu $J_m$ là hợp của chúng, thì tập hợp $A \cap \complement J_m$ là hợp của $2^{m+1}$ khoảng đóng đôi một rời nhau $K_{m,p}$ ($1 \leq p \leq 2^{m+1}$), mỗi khoảng có độ dài $\frac{1}{3^{m+1}}$. Nếu $K_{m,p} = [a, b]$ thì khi đó ta lấy $I_{m+1,p}$ là khoảng mở $\left[ a + \frac{b-a}{3}, \frac{b-a}{3} \right]$ ("một phần ba ở giữa" của khoảng $]a, b[$), và ngay lập tức kiểm tra được rằng phép quy nạp có thể tiếp tục theo cách đó (Hình 3).

![Biểu đồ cho thấy các khoảng I_{2,1}, I_{1,1}, I_{2,2}, I_{0,1}, I_{2,3}, I_{1,2}, I_{2,4} và các khoảng tương ứng K_{2,1}, K_{2,2}, K_{2,3}, K_{2,4}, K_{1,1}, K_{1,2}, K_{1,3}, K_{1,4}, K_{0,1}, K_{0,2}](https://i.imgur.com/3Q5z5QG.png)

Hình 3.

Nếu $K'$ là phần bù của hợp các $I_{n,p}$, thì tập đóng $K = A \cap K'$ được gọi là tập tam phân Cantor. Rõ ràng $K$ là compắc (no. 2, Định lý 2); hơn nữa $K$ hoàn toàn không liên thông. Thật vậy, nếu $K$ chứa một khoảng $I$ có độ dài $> 0$, thì $I$ sẽ được chứa trong một khoảng nào đó $K_{m,p}$; do đó độ dài của nó sẽ là $\leq 1/3^{m+1}$ với mọi $m$, điều này là vô lý.

### 6. ĐỒNG PHÔI CỦA MỘT KHOẢNG LÊN MỘT KHOẢNG

#### Định lý 5 {#top-iv-s2-thm-5 .statement}

*Cho I là một khoảng trong R. Khi đó một ánh xạ f từ I vào R là một đồng phôi của I lên f(I) khi và chỉ khi f đơn điệu nghiêm ngặt và liên tục trên I; và khi đó f(I) là một khoảng trong R.*

1) Điều kiện là cần thiết. Cho $a$ và $b$ là hai điểm của I sao cho $a < b$, và giả sử chẳng hạn rằng $f(a) < f(b)$. Hãy chứng minh rằng $f$ tăng ngặt trên I. Trước hết, nếu $a < c < b$ thì ta phải có $f(a) < f(c) < f(b)$; nếu, chẳng hạn, ta có $f(a) < f(b) < f(c)$

Suy ra rằng nếu $x$ và $y$ là hai điểm bất kỳ của I sao cho $x < y$, thì $f(x) < f(y)$; vì ta có $f(a) < f(x) < f(b)$ nếu $a < x < b$, $f(a) < f(b) < f(x)$ nếu $b < x$, và $f(x) < f(a) < f(b)$ nếu $x < a$; lặp lại lập luận với $a, x, y$ lần lượt thay cho $a, b, x$, ta thấy rằng $f(x) < f(y)$.

2) Điều kiện này là *đủ*. Giả sử $f$ liên tục và đơn điệu nghiêm ngặt trên I (chẳng hạn, tăng ngặt): $f(I)$ liên thông và do đó là một khoảng, và vì $f$ tăng ngặt, $f$ là một ánh xạ song ánh từ I lên $f(I)$. Hơn nữa, ảnh qua $f$ của một khoảng mở *trong* I là một khoảng mở *trong* $f(I)$, và do đó (\$1, no, 4, Mệnh đề 5) $f$ là một đồng phôi từ I lên $f(I)$.

#### Nhận xét {#top-iv-s2-n6-rem-1 .statement}

Phần đầu của chứng minh trước thực ra cho thấy rằng một ánh xạ *liên tục đơn ánh* từ I vào $\mathbf{R}$ là đơn điệu nghiêm ngặt; do phần thứ hai của chứng minh, vì thế suy ra rằng *mọi ánh xạ liên tục đơn ánh* $f$ *từ một khoảng* I *vào* $\mathbf{R}$ *đều là một đồng phôi của* I *lên* $f(I)$.

### Bài tập {#top-iv-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
