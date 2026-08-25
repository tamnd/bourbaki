---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 3
section_title: Subspaces, quotient spaces
lang: vi
source: top-i-iv
pdf_pages: 0041-0049, 0128-0131
extraction: ocr
subsections:
    - "no": 1
      title: SUBSPACES OF A TOPOLOGICAL SPACE
      page: 0
      pdf_page: 41
    - "no": 2
      title: CONTINUITY WITH RESPECT TO A SUBSPACE
      page: 0
      pdf_page: 43
    - "no": 3
      title: LOCALLY CLOSED SUBSPACES
      page: 0
      pdf_page: 44
    - "no": 4
      title: QUOTIENT SPACES
      page: 0
      pdf_page: 45
    - "no": 5
      title: CANONICAL DECOMPOSITION OF A CONTINUOUS MAPPING
      page: 0
      pdf_page: 46
    - "no": 6
      title: QUOTIENT SPACE OF A SUBSPACE
      page: 0
      pdf_page: 48
statements: 24
exercises: 16
content_sha256: d0e856e842a1876058c3fc70e0aaaaaa9ed8fc5bdf1f53bdef3889f3c37eea6a
translated_from: content/en/top/I/03_s3_subspaces_quotient_spaces.md
source_content_sha256: 862adf5542a6bab731b539625326a928f16445b7d34d1aa5bea00e0a31df6348
translation_model: gpt-5.4
translation_run: translate-vi-254c0b55
glossary_version: 34
glossary_terms_sha256: 76680d77f2b5caefd0ac7839e4275960fa4c26b492545f31a63004a06baa41b6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. KHÔNG GIAN CON; KHÔNG GIAN THƯƠNG

### 1. KHÔNG GIAN CON CỦA MỘT KHÔNG GIAN TÔPÔ

Cho $A$ là một tập con của một không gian tôpô $X$. Ta đã định nghĩa *tôpô cảm sinh* trên $A$ bởi tôpô của $X$ là ảnh ngược của tôpô sau qua đơn ánh chính tắc $A \to X$ (\S 2, no. 3, Ví dụ 1). Một định nghĩa tương đương như sau:

#### Định nghĩa 1 {#top-i-s3-def-1 .statement}

Cho $A$ là một tập con của một không gian tôpô $X$. Tôpô cảm sinh trên $A$ bởi tôpô của $X$ là tôpô trong đó các tập mở là các giao với $A$ của các tập mở của $X$. Tập hợp $A$ với tôpô này được gọi là một không gian con của $X$.

#### Ví dụ {#top-i-s3-n1-exa-1 .statement}

Tôpô cảm sinh trên tập hợp $\mathbf{Z}$ các số nguyên bởi tôpô của đường thẳng hữu tỉ là tôpô rời rạc, vì giao của $\mathbf{Z}$ với khoảng mở $]n - 1/2, n + 1/2[$ là tập hợp $\{ n \}$.

Theo Mệnh đề 5 của § 2, no. 3 (hoặc trực tiếp từ Định nghĩa 1), ta thấy rằng, nếu $B \subset A \subset X$, không gian con $B$ của $X$ đồng nhất với không gian con $B$ của không gian con $A$ của $X$ (tính bắc cầu của các tôpô cảm sinh). Nếu $\mathcal{G}$ là một cơ sở con (resp. một cơ sở) của tôpô của $X$ ($\S 2$, no. 3, Ví dụ 3) thì vết $\mathcal{G}_A$ của nó trên $A$ là một cơ sở con (resp. một cơ sở) của tôpô cảm sinh trên $A$.

Trong mọi câu hỏi có liên quan đến các phần tử hoặc các tập con của $A$, điều cốt yếu là phải phân biệt cẩn thận giữa các tính chất của chúng như những điểm (tương ứng, những tập con) của $X$, và các tính chất của chúng như những điểm (tương ứng, những tập con) của không gian con $A$. Ta sẽ thực hiện sự phân biệt này bằng cách dùng các cụm từ "trong $A$", "đối với $A$", hoặc "tương đối đối với $A$" để chỉ các tính chất thuộc loại sau (có thể đối chiếu chúng với các cụm từ "trong $X$", "đối với $X$", "tương đối đối với $X$").

Một tập mở của không gian con $A$ không nhất thiết mở trong $X$; để mọi tập hợp mở trong $A$ đều mở trong $X$ thì điều kiện cần và đủ là $A$ mở trong $X$. Điều kiện đó là cần, vì $A$ mở trong $A$, và là đủ theo $(O_{II})$ và Định nghĩa 1.

Các tập hợp đóng trong $A$ là các giao với $A$ của những tập hợp đóng trong $X$ ($\S 2$, no. 3, ví dụ 1); như trên ta thấy rằng mọi tập hợp đóng trong $A$ đều đóng trong $X$ khi và chỉ khi $A$ đóng trong $X$.

Các lân cận của một điểm $x \in A$ tương đối với $A$ là các giao với $A$ của những lân cận của $x$ tương đối với $X$. Mọi lân cận của $x$ tương đối với $A$ đều là một lân cận của $x$ tương đối với $X$ khi và chỉ khi $A$ là một lân cận của $x$ trong $X$.

#### Mệnh đề 1 {#top-i-s3-prop-1 .statement}

Nếu $A$ và $B$ là hai tập con của một không gian tôpô $X$, và $B \subset A$, thì bao đóng của $B$ trong không gian con $A$ là giao với $A$ của bao đóng $\overline{B}$ của $B$ trong $X$.

Nếu $x \in A$, mọi lân cận của $x$ trong $A$ đều có dạng $V \cap A$, trong đó $V$ là một lân cận của $x$ trong $X$. Vì $V \cap B = (V \cap A) \cap B$, suy ra $x$ thuộc bao đóng của $B$ đối với $A$ khi và chỉ khi $x$ thuộc bao đóng của $B$ đối với $X$.

#### Hệ quả {#top-i-s3-n1-cor-1 .statement}

Một tập con $B$ của $A$ là trù mật trong $A$ khi và chỉ khi $\overline{B} = \overline{A}$ trong $X$ (tức là khi và chỉ khi $A \subset \overline{B}$).

Suy ra rằng nếu $A, B, C$ là ba tập con của $X$ sao cho $A \supset B \supset C$, và nếu $B$ trù mật trong $A$, và $C$ trù mật trong $B$, thì $C$ trù mật trong $A$ (*tính bắc cầu* của mật độ), vì ta có $\overline{A} = \overline{B} = \overline{C}$ trong $X$.

#### Mệnh đề 2 {#top-i-s3-prop-2 .statement}

*Cho $A$ là một tập con trù mật của một không gian tôpô $X$; khi đó, với mỗi $x \in A$ và mỗi lân cận $V$ của $x$ đối với $A$, bao đóng $\overline{V}$ của $V$ trong $X$ là một lân cận của $x$ trong $X$.*

Vì $V$ chứa $U \cap A$, trong đó $U$ là một tập con mở của $X$ chứa $x$, nên $\overline{V}$ chứa $U \cap \overline{A} = U$ (\S 1, no. 6, Mệnh đề 5).

#### Mệnh đề 3 {#top-i-s3-prop-3 .statement}

*Cho $(A_i)_{i \in I}$ là một họ các tập con của một không gian tôpô $X$, sao cho một trong các tính chất sau được thỏa mãn:
a) Các phần trong của các $A_i$ phủ $X$.
b) $(A_i)_{i \in I}$ là một phủ đóng hữu hạn địa phương của $X$ (\S 1, no. 5).*

*Trong các điều kiện này, một tập con $B$ của $X$ là mở (tương ứng, đóng) trong $X$ khi và chỉ khi mỗi tập $B \cap A_i$ là mở (tương ứng, đóng) trong $A_i$.*

Rõ ràng nếu $B$ là mở (tương ứng, đóng) trong $X$, thì $B \cap A_i$ là mở (tương ứng, đóng) trong $A_i$. Ngược lại, trước hết giả sử rằng điều kiện a) được thỏa mãn; vì $(\complement B) \cap A_i = A_i - (B \cap A_i)$, theo tính đối ngẫu, chỉ cần xét trường hợp trong đó mỗi $B \cap A_i$ là *mở* đối với $A_i$. Trong trường hợp này, $B \cap \dot{A}_i$ là mở trong $\dot{A}_i$ với mọi $i \in I$, và do đó mở trong $X$; và vì $B = \bigcup_i (B \cap \dot{A}_i)$ theo giả thiết, suy ra $B$ là mở trong $X$.

Bây giờ giả sử rằng b) được thỏa mãn; lại do tính đối ngẫu, ta chỉ cần xét trường hợp trong đó mỗi $B \cap A_i$ là *đóng* trong $A_i$, và do đó đóng trong $X$. Vì họ $(B \cap A_i)$ là hữu hạn địa phương và $B = \bigcup_i (B \cap A_i)$, nên theo \S 1, no. 5, Mệnh đề 4 suy ra $B$ là đóng trong $X$.

#### Nhận xét {#top-i-s3-n1-rem-1 .statement}

Cho $(U_i)_{i \in I}$ là một phủ *mở* của một không gian tôpô $X$, và với mỗi $i \in I$ cho $\mathcal{B}_i$ là một *cơ sở* của tôpô của không gian con $U_i$ của $X$; khi đó hiển nhiên là $\mathcal{B} = \bigcup_{i \in I} \mathcal{B}_i$ là một *cơ sở* của tôpô của $X$.

### 2. TÍNH LIÊN TỤC ĐỐI VỚI MỘT KHÔNG GIAN CON

Cho $X$ và $Y$ là hai không gian tôpô, $f$ là một ánh xạ từ $X$ vào $Y$, $B$ là một tập con của $Y$ chứa $f(X)$. Định nghĩa của tôpô cảm sinh như một tôpô ban đầu (\S 2, no. 3, Mệnh đề 4) cho thấy rằng $f$ liên tục tại $x \in X$ khi và chỉ khi ánh xạ từ $X$ vào *không gian con* $B$ của $Y$, có cùng đồ thị như $f$, là liên tục tại $x$.

Bây giờ, cho $A$ là một tập con của $X$; nếu $f$ liên tục tại $x \in A$ (resp. liên tục trên $X$), thì hạn chế $f|A$ của nó là một ánh xạ từ không gian con $A$ vào $Y$, liên tục tại $x$ (resp. liên tục trên $A$) theo Mệnh đề 2 của § 2, no. 1. Đôi khi, ta sẽ nói rằng một ánh xạ $f : X \to Y$ là *liên tục tương đối đối với $A$ tại $x \in A$* (resp. *liên tục tương đối đối với $A$*) nếu hạn chế $f|A$ của nó liên tục tại $x$ (resp. liên tục trên $A$).

Cần lưu ý rằng $f|A$ có thể liên tục mà $f$ lại không liên tục tại bất kỳ điểm nào của $X$; một ví dụ của hiện tượng này được cho bởi hàm đặc số $\varphi_A$ của một tập con $A$ của $X$ sao cho cả $A$ lẫn phần bù của nó đều trù mật trong $X$ ($\S 2$, Bài tập 11), khi $\varphi_A$ được xem như một ánh xạ từ $X$ vào không gian rời rạc $\{0, 1\}$. $\varphi_A$ không liên tục tại bất kỳ điểm nào của $X$, nhưng hạn chế của nó trên $A$ là hằng và do đó liên tục.

Nếu $A$ là một lân cận trong $X$ của một điểm $x \in A$, và nếu $f : X \to Y$ sao cho $f|A$ liên tục tại $x$, thì $f$ liên tục tại $x$; vì mỗi lân cận của $x$ trong $A$ là một lân cận của $x$ trong $X$ (đặc trưng *địa phương* của tính liên tục).

#### Mệnh đề 4 {#top-i-s3-prop-4 .statement}

*Cho* $(A_i)_{i \in I}$ *là một họ các tập con của một không gian tôpô* $X$ *mà các phần trong của chúng phủ* $X$, *hoặc tạo thành một phủ đóng hữu hạn địa phương của* $X$. *Cho* $f$ *là một ánh xạ từ* $X$ *vào một không gian tôpô* $X'$. *Nếu hạn chế của* $f$ *trên mỗi không gian con* $A_i$ *là liên tục, thì* $f$ *là liên tục.*

Thật vậy, nếu $F'$ là một tập con đóng của $X'$ và nếu $F = \overline{f}(F')$, thì $F \cap A_i$ đóng trong $A_i$ với mỗi $i \in I$ ($\S 2$, no. 1, Định lý 1) và do đó $F$ đóng trong $X$ theo Mệnh đề 3 của no. 1; kết quả bây giờ suy ra từ Định lý 1 của $\S 2$, no. 1.

### 3. KHÔNG GIAN CON ĐÓNG ĐỊA PHƯƠNG

#### Định nghĩa 2 {#top-i-s3-def-2 .statement}

*Một tập con* $L$ *của một không gian tôpô* $X$ *được gọi là địa phương đóng tại một điểm* $x \in L$ *nếu tồn tại một lân cận* $V$ *của* $x$ *trong* $X$ *sao cho* $L \cap V$ *là một tập con đóng của không gian con* $V$. *L được gọi là địa phương đóng trong* $X$ *nếu nó địa phương đóng tại mỗi* $x \in L$.

#### Nhận xét {#top-i-s3-n3-rem-1 .statement}

Cho $F$ là một tập con của $X$ sao cho *với mỗi điểm* $x$ *của* $X$ *đều có một lân cận* $V$ *của* $x$ *sao cho* $V \cap F$ *đóng trong không gian con* $V$; *khi đó suy ra từ Mệnh đề 3 của no. 1 rằng* $F$ *đóng trong* $X$. *Mặt khác, Mệnh đề 5 dưới đây cho thấy rằng nói chung có những tập hợp đóng địa phương mà không đóng trong* $X$.

#### Mệnh đề 5 {#top-i-s3-prop-5 .statement}

*Đối với một tập con* $L$ *của một không gian tôpô* $X$, *các tính chất sau là tương đương*:

a) $L$ *đóng địa phương trong* $X$.

b) $L$ là giao của một tập con mở và một tập con đóng của $X$.

c) $L$ là mở trong bao đóng của nó $\overline{L}$ trong $X$.

Nếu $L$ đóng địa phương, thì với mỗi $x \in L$, tồn tại một lân cận mở $V_x$ của $x$ trong $X$ sao cho $L \cap V_x$ đóng trong $V_x$; $U = \bigcup_{x \in L} V_x$ mở trong $X$, và Mệnh đề 3 của no. 1 cho thấy rằng $L$ đóng trong $U$; do đó a) suy ra b). Nếu $L = U \cap F$, trong đó $U$ mở và $F$ đóng trong $X$, thì ta có $L \subset F$; vì thế $L \subset U \cap L \subset U \cap F = L$, điều này cho thấy $L = U \cap L$ mở trong $L$, nên b) suy ra c). Sau cùng, nếu $L = U \cap L$, trong đó $U$ mở trong $X$, thì $L$ đóng trong $U$, do đó đóng địa phương, và vì vậy c) suy ra a).

#### Hệ quả {#top-i-s3-n3-cor-1 .statement}

*Cho $f : X \to X'$ là một ánh xạ liên tục và $L'$ là một tập con đóng địa phương của $X'$; khi đó $f^{-1}(L')$ là đóng địa phương trong $X$*.

Điều này suy ra ngay lập tức từ Mệnh đề 5 ở trên và Định lý 1 của § 2, no. 1.

### 4. CÁC KHÔNG GIAN THƯƠNG

#### Định nghĩa 3 {#top-i-s3-def-3 .statement}

*Cho $X$ là một không gian tôpô, $R$ là một quan hệ tương đương trên $X$. Không gian thương của $X$ theo $R$ là tập thương $X/R$ được trang bị tôpô là thương của tôpô của $X$ theo quan hệ $R$ (\S 2, no. 4, Ví dụ 1)*.

Trừ khi có nói rõ điều trái lại, mỗi khi ta nói về $X/R$ như một không gian tôpô, phải hiểu rằng ta muốn nói đến không gian thương của $X$ theo $R$. Ta sẽ thường nói rằng không gian tôpô này là không gian thu được bằng cách đồng nhất các điểm của $X$ thuộc cùng một lớp tương đương mod $R$.

Gọi $\varphi$ là ánh xạ chính tắc $X \to X/R$. Theo định nghĩa (\S 2, no. 4, Mệnh đề 6 và hệ quả của nó), các tập mở (tương ứng, đóng) trong $X/R$ là các tập $A$ sao cho $\varphi^{-1}(A)$ mở (tương ứng, đóng) trong $X$; nói cách khác, các tập mở (tương ứng, đóng) trong $X/R$ tương ứng một-một với các tập con mở (tương ứng, đóng) của $X$ bão hòa đối với $R$ và là các ảnh chính tắc của các tập con ấy.

#### Mệnh đề 6 {#top-i-s3-prop-6 .statement}

*Cho $X$ là một không gian tôpô, $R$ là một quan hệ tương đương trên $X$, $\varphi$ là ánh xạ chính tắc từ $X$ lên $X/R$; khi đó một ánh xạ $f$ từ $X/R$ vào một không gian tôpô $Y$ là liên tục khi và chỉ khi $f \circ \varphi$ liên tục trên $X$*.

Đây là một trường hợp riêng của \S 2, no. 4, Mệnh đề 6; nó biểu thị sự kiện rằng tôpô thương là tôpô cuối đối với ánh xạ $\varphi$.

Mệnh đề 6 cho thấy rằng có một sự tương ứng một-một giữa các ánh xạ liên tục của $X/R$ vào $Y$ và các ánh xạ liên tục của $X$ vào $Y$ *hằng trên mỗi lớp tương đương mod $R$*.

#### Ví dụ {#top-i-s3-n4-exa-1 .statement}

*Xét quan hệ tương đương $x \equiv y \pmod{1}$ trên đường thẳng thực $\mathbf{R}$; không gian thương của $\mathbf{R}$ theo quan hệ này được gọi là *xuyến một chiều* và được ký hiệu bởi $T$. Lớp tương đương của một điểm $x \in \mathbf{R}$ gồm tất cả các điểm $x + n$, trong đó $n$ chạy qua tập hợp $\mathbf{Z}$ các số nguyên. Theo Mệnh đề 6 có một sự tương ứng một-một giữa các hàm liên tục trên $T$ và các hàm liên tục trên $\mathbf{R}$ mà *tuần hoàn* với chu kỳ 1. Chúng ta sẽ trở lại ví dụ quan trọng này trong Chương V, § 1.*

#### Hệ quả {#top-i-s3-n4-cor-1 .statement}

*Cho $X, Y$ là hai không gian tôpô, $R$ (tương ứng $S$) là một quan hệ tương đương trên $X$ (tương ứng $Y$), và cho $f : X \to Y$ là một ánh xạ liên tục tương thích với các quan hệ tương đương $R$ và $S$ (Lý thuyết tập hợp R, § 5, no. 8); khi đó ánh xạ $g : X/R \to Y/S$ cảm sinh bởi $f$ (Lý thuyết tập hợp R, § 5, no. 8) là liên tục.*

Đây là một trường hợp riêng của một tính chất tổng quát của các cấu trúc thương (Lý thuyết tập hợp, Chương IV, § 2, no. 6, tiêu chuẩn CST 20).

#### Mệnh đề 7 (Tính bắc cầu của các không gian thương) {#top-i-s3-prop-7 .statement}

*Cho $R$ và $S$ là hai quan hệ tương đương trên một không gian tôpô $X$ sao cho $R$ kéo theo $S$, và gọi $S/R$ là quan hệ tương đương thương trên không gian thương $X/R$ (Lý thuyết tập hợp R, § 5, no. 9). Khi đó song ánh chính tắc $(X/R)/(S/R) \to X/S$ là một đồng phôi.*

Đây là một trường hợp riêng của tính bắc cầu của các tôpô cuối (§ 2, no. 4, Mệnh đề 7. Xem Lý thuyết tập hợp, Chương IV, § 2, no. 3, tiêu chuẩn CST 21).

### 5. PHÂN TÍCH CHÍNH TẮC CỦA MỘT ÁNH XẠ LIÊN TỤC

Cho $X$ và $Y$ là hai không gian tôpô, $f : X \to Y$ một ánh xạ liên tục, $R$ là quan hệ tương đương $f(x) = f(y)$ trên $X$. Xét *phân tích chính tắc*

$$
f : X \xrightarrow{\varphi} X/R \xrightarrow{g} f(X) \xrightarrow{\psi} Y
$$

trong đó $\varphi$ là ánh xạ chính tắc (toàn ánh) của $X$ lên không gian thương $X/R$, $\psi$ là đơn ánh chính tắc của không gian con $f(X)$ vào $Y$, và $g$ là song ánh liên kết với $f$ (Lý thuyết tập hợp R, § 5, no. 3). Người ta thấy ngay lập tức rằng $g$ là liên tục (theo Mệnh đề 6 của no. 4); đây cũng là một trường hợp riêng của một kết quả tổng quát về các cấu trúc thương. (Xem Lý thuyết tập hợp, Chương IV, § 2, no. 6). Nhưng song ánh $g$ *không nhất thiết là một đồng phôi*.

#### Mệnh đề 8 {#top-i-s3-prop-8 .statement}

Cho $f = \psi \circ g \circ \varphi$ là phân tích chính tắc của một ánh xạ liên tục $f : X \to Y$, và gọi $R$ là quan hệ tương đương
$$
f(x) = f(y).
$$
Khi đó ba điều kiện sau là tương đương:
a) $g$ là một đồng phôi từ $X/R$ lên $f(X)$.
b) Ảnh qua $f$ của mọi tập mở bão hòa đối với $R$ là một tập mở trong không gian con $f(X)$.
c) Ảnh qua $f$ của mọi tập đóng bão hòa đối với $R$ là một tập đóng trong không gian con $f(X)$.

Vì điều kiện b) [tương ứng c)] biểu thị rằng ảnh dưới $g$ của mọi tập mở (tương ứng đóng) trong $X/R$ là một tập mở (tương ứng đóng) trong $f(X)$.

#### Ví dụ {#top-i-s3-n5-exa-1 .statement}

Cho $X$ là một không gian tôpô, $(X_i)_{i \in I}$ là một phủ của $X$, $Y$ là tổng của các không gian con $X_i$ của $X$; khi đó có một phân hoạch $(Y_i)_{i \in I}$ của $Y$ thành các không gian con vừa mở vừa đóng, và với mỗi $i \in I$ có một đồng phôi $f_i : Y_i \to X_i$. Gọi $f : Y \to X$ là ánh xạ liên tục trùng với $f_i$ trên $Y_i$ với mỗi $i \in I$, và gọi $R$ là quan hệ tương đương $f(x) = f(y)$; do đó không gian thương $Y/R$ được nhận bằng cách "dán lại với nhau" các $Y_i$ (\S 2, no. 5). Xét song ánh $g : Y/R \to X$ liên kết với $f$; nói chung $g$ không phải là một đồng phôi, như được chỉ ra bởi ví dụ trong đó mỗi $X_i$ chỉ gồm một điểm và $X$ không rời rạc. Tuy nhiên, nếu các phần trong của các $X_i$ phủ $X$, hoặc nếu $(X_i)$ là một phủ đóng hữu hạn địa phương của $X$, thì $g$ là một đồng phôi: thật vậy, nếu $U$ là một tập con mở bất kỳ của $Y$ bão hòa đối với $R$, thì với mỗi $i \in I$ tập hợp
$$
f(U) \cap X_i = f_i(U \cap Y_i)
$$
là mở trong $X_i$, và mệnh đề suy ra từ Mệnh đề 3 của no. 1.

Mệnh đề sau cho một điều kiện đủ đơn giản để $g$ là một phép đồng phôi:

#### Mệnh đề 9 {#top-i-s3-prop-9 .statement}

Cho $f : X \to Y$ là một toàn ánh liên tục, và gọi $R$ là quan hệ tương đương $f(x) = f(y)$. Nếu tồn tại một tiết diện liên tục $s : Y \to X$ liên kết với $f$ (Lý thuyết tập hợp, Chương II, § 3, no. 8, Định nghĩa 11), thì ánh xạ $g : X/R \to Y$ liên kết với $f$ là một phép đồng phôi, và $s$ là một phép đồng phôi của $Y$ lên không gian con $s(Y)$ của $X$.

Thật vậy, nếu $\varphi : X \to X/R$ là ánh xạ chính tắc, thì $g$ và $\varphi \circ s$ là song ánh, liên tục và nghịch đảo của nhau; tương tự, $s$ và hạn chế của $f$ trên $s(Y)$ là song ánh, liên tục và nghịch đảo của nhau.

Nếu $R$ là một quan hệ tương đương trên một không gian tôpô $X$ và
$$
\varphi : X \to X/R
$$
là ánh xạ chính tắc, thì một *tiết diện liên tục* $s : X/R \to X$ liên kết với $\varphi$ cũng được gọi là một *tiết diện liên tục* của $X$ đối với $R$ (x. *Lý thuyết tập hợp*, Chương II, § 6, no. 2); khi đó không gian con $s(X/R)$ của $X$ đồng phôi với $X/R$. Nếu đã cho $s(X/R)$, thì $s$ được xác định duy nhất; $s(X/R)$ thường được gọi, do lạm dụng ngôn ngữ, là một *tiết diện* (liên tục) của $X$ đối với $R$.

Một tiết diện liên tục của một không gian tôpô đối với một quan hệ tương đương không nhất thiết phải tồn tại (Bài tập 12).

### 6. KHÔNG GIAN THƯƠNG CỦA MỘT KHÔNG GIAN CON

Cho $X$ là một không gian tôpô, $A$ là một không gian con của $X$, $R$ là một quan hệ tương đương trên $X$, $f$ là ánh xạ chính tắc $X \to X/R$, $g$ là hạn chế của $f$ lên $A$. Quan hệ tương đương $g(x) = g(y)$ trên $A$ chính là quan hệ $R_A$ được *cảm sinh* bởi $R$ trên $A$ (*Lý thuyết tập hợp* R, § 5, no. 5). Gọi $g = \psi \circ h \circ \varphi$ là phân tích chính tắc của $g$, khi đó nếu $j$ là đơn ánh chính tắc từ $A$ vào $X$ thì ta có biểu đồ giao hoán (*)

$$
\begin{array}{ccc}
A & \xrightarrow{\varphi} & A/R_A \xrightarrow{h} f(A) \xrightarrow{\psi} X/R. \\
& & \\
& \searrow_j & \nearrow_s \\
& & X
\end{array}
$$

#### Mệnh đề 10 {#top-i-s3-prop-10 .statement}

*Song ánh chính tắc* $h : A/R_A \to f(A)$ *là liên tục*. *Hơn nữa, ba mệnh đề sau là tương đương*:

a) $h$ *là một đồng phôi*.

b) *Mọi tập con mở của* $A$ *bão hòa đối với* $R_A$ *đều là giao với* $A$ *của một tập con mở của* $X$ *bão hòa đối với* $R$.

c) *Mọi tập con đóng của* $A$ *bão hòa đối với* $R_A$ *đều là giao với* $A$ *của một tập con đóng của* $X$ *bão hòa đối với* $R$.

Phần thứ nhất của mệnh đề là hệ quả ngay lập tức (no. 5). Phần thứ hai suy ra từ Mệnh đề 8 của no. 5: nếu $B$ là một tập con mở (tương ứng, đóng) của $A$ bão hòa đối với $R_A$, và $g(B) = f(B)$ là giao với $f(A)$ của một tập con mở (tương ứng, đóng) $C$ của $X/R$, thì $B$ là giao với $A$ của tập con mở (tương ứng, đóng) $f^{-1}(C)$

(*) Biểu thức này có nghĩa là $f \circ j = \psi \circ h \circ \varphi$.

của X, bão hòa đối với R; và ngược lại, nếu B là giao với A của một tập con mở (tương ứng, đóng) D bão hòa đối với R, thì $f(B)$ là giao của $f(A)$ và $f(D)$, là tập mở (tương ứng, đóng) trong $X/R$.

#### Hệ quả 1 {#top-i-s3-prop-10-cor-1 .statement}

*Nếu A là một tập con mở (tương ứng, đóng) của X bão hòa đối với R, thì ánh xạ chính tắc $h : A/R_A \to f(A)$ là một đồng phôi.*

Thật vậy, nếu A mở (tương ứng, đóng) trong X và bão hòa đối với R, và nếu $B \subset A$ mở (tương ứng, đóng) trong A và bão hòa đối với $R_A$, thì B mở (tương ứng, đóng) trong X và bão hòa đối với R.

#### Hệ quả 2 {#top-i-s3-prop-10-cor-2 .statement}

*Nếu tồn tại một ánh xạ liên tục $u : X \to A$ sao cho $u(x)$ đồng dư với $x$ mod R với mọi $x \in X$, thì $f(A) = X/R$ và ánh xạ chính tắc $h : A/R_A \to X/R$ là một đồng phôi.*

Vì mỗi lớp tương đương mod R đều gặp A, ảnh chính tắc của $A/R_A$ trong $X/R$ là toàn bộ $X/R$; mặt khác, nếu U là mở trong A và bão hòa đối với $R_A$, thì theo giả thiết $\bar{u}^1(U)$ là tập hợp thu được bằng cách bão hòa U đối với R; vì $u$ liên tục, $\bar{u}^1(U)$ là mở trong X (\S 2, no. 1, Định lý 1). Hệ quả suy ra từ sự kiện này nhờ Mệnh đề 10.

#### Ví dụ {#top-i-s3-n6-exa-1 .statement}

Gọi R là quan hệ tương đương $x \equiv y \pmod{1}$ trên đường thẳng thực $\mathbf{R}$ (no. 4, Ví dụ) và gọi A là khoảng đóng $[0, 1]$; A chứa ít nhất một điểm của mỗi lớp tương đương mod R. Ánh xạ chính tắc từ $A/R_A$ lên xuyến T là một đồng phôi; thật vậy, nếu F là đóng trong A (và do đó trong R), thì để bão hòa F đối với quan hệ R, ta phải lấy hợp của các tập hợp đóng $F + n$ (với mọi $n \in \mathbf{Z}$), rõ ràng chúng tạo thành một họ hữu hạn địa phương, nên hợp của chúng là đóng (\S 1, no. 5, Mệnh đề 4); mệnh đề suy ra từ đó. Ta nhận xét rằng $A/R_A$ thu được bằng cách đồng nhất hóa các điểm 0 và 1 trong A. \*

### Bài tập {#top-i-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
