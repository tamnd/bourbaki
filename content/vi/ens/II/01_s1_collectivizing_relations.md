---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 1
section_title: Collectivizing relations
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 65-72, 123
pdf_pages: 0072-0079, 0130-0130
extraction: ocr
subsections:
    - "no": 1
      title: THE THEORY OF SETS
      page: 65
      pdf_page: 72
    - "no": 2
      title: INCLUSION
      page: 66
      pdf_page: 73
    - "no": 3
      title: THE AXIOM OF EXTENT
      page: 67
      pdf_page: 74
    - "no": 4
      title: COLLECTIVIZING RELATIONS
      page: 67
      pdf_page: 74
    - "no": 5
      title: THE AXIOM OF THE SET OF TWO ELEMENTS
      page: 69
      pdf_page: 76
    - "no": 6
      title: THE SCHEME OF SELECTION AND UNION
      page: 69
      pdf_page: 76
    - "no": 7
      title: COMPLEMENT OF A SET. THE EMPTY SET
      page: 71
      pdf_page: 78
statements: 10
exercises: 6
content_sha256: 1eaef683997096345c904314f8d9802acd2423cbc0d921eb3e1da818b64f6ec3
translated_from: content/en/ens/II/01_s1_collectivizing_relations.md
source_content_sha256: f27c098283cf976dbfe884a6515c10d42a193eed1659b1a36d768d136ab18309
translation_model: gpt-5.4
translation_run: translate-vi-f3bb3512
glossary_version: 29
glossary_terms_sha256: 373349ade6facbcaa71cd68a2853401fe6a7bccb4adc757b392eca56649cdd21
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. CÁC QUAN HỆ XÁC ĐỊNH TẬP

### 1. LÝ THUYẾT TẬP HỢP

*lý thuyết tập hợp* là một lý thuyết chứa các dấu quan hệ $=$, $\in$ và dấu danh hóa $\supset$ (tất cả các dấu này đều có trọng số 2); ngoài các lược đồ S1 đến S7 đã cho ở Chương I, nó còn chứa lược đồ S8, sẽ được đưa vào ở no. 6, và các tiên đề tường minh A1 (no. 3.) A2 (no. 5), A3 (§ 2, no. 1), A4 (§ 5, no. 1), và A5 (Chương III, § 6, no. 1), Các tiên đề tường minh này không chứa chữ cái nào; nói cách khác, lý thuyết tập hợp là một lý thuyết *không có hằng*.

Vì lý thuyết tập hợp là một lý thuyết bình đẳng, các kết quả của Chương I đều áp dụng được.

¶ Từ nay về sau, trừ khi có phát biểu minh nhiên ngược lại, ta sẽ luôn luôn lập luận trong một lý thuyết mạnh hơn (Chương I, § 2, no. 4) lý thuyết tập hợp; nếu không nói rõ lý thuyết nào, thì phải hiểu là lý thuyết tập hợp được ngầm định. Trong nhiều trường hợp, sẽ hiển nhiên là giả thiết này là thừa, và độc giả hẳn sẽ không gặp khó khăn gì trong việc xác định các kết quả đã phát biểu là đúng trong lý thuyết nào yếu hơn lý thuyết tập hợp.

Nếu $T$ và $U$ là các số hạng, thì biểu thức $\in TU$ là một quan hệ (gọi là *quan hệ thuộc*) mà trong thực hành ta viết theo một trong các cách sau: $T \in U$, $(T) \in (U)$, "$T$ thuộc $U$", "$T$ là một phần tử của $U$". Quan hệ "không $(T \in U)$" được viết là $T \notin U$.

Theo một quan điểm "ngây thơ", nhiều thực thể toán học có thể được xem như những sưu tập hay những "tập hợp" các đối tượng. Chúng tôi không tìm cách hình thức hóa khái niệm này, và trong lối giải thích hình thức của phần sau, từ "tập hợp" phải được coi là đồng nghĩa nghiêm ngặt với "số hạng". Đặc biệt, những cụm từ như "cho X là một tập hợp", về nguyên tắc, là hoàn toàn thừa, vì mọi chữ cái đều là một số hạng. Những cụm từ như vậy chỉ được đưa vào để giúp cho cách hiểu trực quan của văn bản.

### 2. BAO HÀM

#### Định nghĩa 1 {#ens-ii-s1-def-1 .statement tag=03H5}

*Quan hệ được ký hiệu bởi* $(\forall z)((z \in x) \Rightarrow (z \in y))$, *trong đó chỉ các chữ cái $x$ và $y$ xuất hiện, được viết theo một trong các cách sau :* $x \subset y$, $y \supset x$, *"$x$ được chứa trong $y$", "$y$ chứa $x$", "$x$ là một tập con của $y$". Quan hệ* "không phải $(x \subset y)$" *được viết* $x \not\subset y$ *hoặc* $y \not\supset x$.

Phù hợp với các quy ước đã nêu trong Chương I, § 1, no. 1, định nghĩa này kéo theo quy ước siêu toán học sau đây. Cho $T$ và $U$ là các dãy ký hiệu; nếu ta thay $T$ cho $x$ và $U$ cho $y$ trong dãy ký hiệu $x \subset y$, ta thu được một dãy ký hiệu được ký hiệu là $T \subset U$; nếu ta ký hiệu bởi $\mathbf{x}$, $\mathbf{y}$ những chữ cái phân biệt với $x$, $y$ và phân biệt với nhau, đồng thời không xuất hiện trong $T$ cũng không xuất hiện trong $U$, thì dãy ký hiệu $T \subset U$ khi đó đồng nhất với $(T|\mathbf{x})(U|\mathbf{y})(\mathbf{x}|x)(\mathbf{y}|y)(x \subset y,)$ và do đó, theo CS8, CS9 (Chương I, § 4, no. 1), và CS5 (Chương I, § 1, no. 2), với $(\forall z)((z \in T) \Rightarrow (z \in U))$, với điều kiện rằng $z$ là một chữ cái không xuất hiện trong $T$ cũng không xuất hiện trong $U$.

Từ nay về sau, mỗi khi phát biểu một định nghĩa toán học, chúng tôi sẽ không nhắc đến quy ước siêu toán học mà nó kéo theo.

CS12. *Cho $T$, $U$, $V$ là các dãy ký hiệu và $x$ là một chữ cái. Khi đó dãy ký hiệu $(V|x)(T \subset U)$ đồng nhất với $(V|x)T \subset (V|x)U$.*

Điều này suy ra ngay lập tức từ CS9 (Chương I, § 4, no. 1) và CS5 (Chương I, § 1, no. 2).

CF13. *Nếu $T$ và $U$ là các hạng, thì $T \subset U$ là một quan hệ.*

Điều này suy ra ngay lập tức từ CF8 (Chương I, § 1, no. 4).

¶ Mọi quan hệ có dạng $T \subset U$ (trong đó $T$ và $U$ là các hạng) được gọi là một *quan hệ bao hàm*.

Từ nay về sau, chúng tôi sẽ không còn viết ra một cách tường minh các tiêu chuẩn thế và các tiêu chuẩn kiến tạo cần phải theo sau các định nghĩa. Tuy nhiên, cần lưu ý rằng các tiêu chuẩn này sẽ thường được dùng một cách ngầm định trong các chứng minh.

Để chứng minh quan hệ $x \subset y$ trong một lý thuyết $\mathscr{T}$, theo C27 (Chương I, § 4, no. 1), chỉ cần chứng minh rằng $z \in y$ trong lý thuyết thu được bằng cách thêm $z \in x$ vào các tiên đề của $\mathscr{T}$, trong đó $z$ là một chữ cái phân biệt với $x$, $y$ và các hằng của lý thuyết. Trên thực tế ta nói "cho $z$ là một phần tử của $x$", và ta cố chứng minh $z \in y$.

#### Mệnh đề 1 {#ens-ii-s1-prop-1 .statement tag=03P9}

$x \subset x$.

Hiển nhiên.

#### Mệnh đề 2 {#ens-ii-s1-prop-2 .statement tag=03PA}

$(x \subset y$ and $y \subset z) \Rightarrow (x \subset z)$.

Hãy thêm các giả thiết $x \subset y$, $y \subset z$, và $u \in x$. Khi đó các quan hệ

$$(u \in x) \Rightarrow (u \in y), \qquad (u \in y) \Rightarrow (u \in z),$$

là đúng, và do đó quan hệ $u \in z$ là đúng.

### 3. TIÊN ĐỀ NGOẠI DIÊN

*tiên đề ngoại diên* là tiên đề sau đây :

A1. $\qquad (\forall x)(\forall y)((x \subset y \text{ và } y \subset x) \Rightarrow (x = y))$.

Về mặt trực giác, tiên đề này diễn đạt rằng hai tập hợp có cùng các phần tử thì bằng nhau.

Vì thế, để chứng minh rằng $x = y$ chỉ cần chứng minh $z \in y$ trong lý thuyết thu được bằng cách thêm giả thiết $z \in x$, và $z \in x$ trong lý thuyết thu được bằng cách thêm giả thiết $z \in y$, trong đó $z$ là một chữ cái phân biệt với $x$, $y$ và các hằng.

C48. *Cho $\mathbf{R}$ là một quan hệ, $x$ là một chữ cái, và $y$ là một chữ cái phân biệt với $x$ không xuất hiện trong $\mathbf{R}$. Khi đó quan hệ $(\forall x)((x \in y) \Leftrightarrow \mathbf{R})$ là đơn trị theo $y$.*

Cho $z$ là một chữ cái phân biệt với $x$ không xuất hiện trong $\mathbf{R}$. Thêm các giả thiết

$$(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\forall x)((x \in z) \Leftrightarrow \mathbf{R}).$$

Khi đó ta lần lượt có các định lý

$$(\forall x)(((x \in y) \Leftrightarrow \mathbf{R}) \text{ và } ((x \in z) \Leftrightarrow \mathbf{R})),$$
$$(\forall x)((x \in y) \Leftrightarrow (x \in z)),$$
$$y \subset z, \qquad z \subset y.$$

Theo A1 khi đó ta có $y = z$. Điều này chứng minh C48.

### 4. CÁC QUAN HỆ XÁC ĐỊNH TẬP

Cho $\mathbf{R}$ là một quan hệ và $x$ là một chữ. Nếu $y$ và $y'$ biểu thị các chữ phân biệt với $x$ *không xuất hiện trong $\mathbf{R}$*, thì các quan hệ

$$(\exists y)(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\exists y')(\forall x)((x \in y') \Leftrightarrow \mathbf{R})$$

là đồng nhất theo CS8 (Chương I, §4, no. 1). Quan hệ do đó được định nghĩa (không chứa $x$) được ký hiệu bởi $\operatorname{Coll}_xR$.

¶ Nếu $\operatorname{Coll}_xR$ là một định lý trong một lý thuyết $\mathscr{T}$, thì người ta nói rằng $R$ là *xác định tập theo $x$* trong $\mathscr{T}$. Khi đó, ta có thể giới thiệu một hằng số phụ $a$, phân biệt với $x$ và các hằng số của $\mathscr{T}$, và không xuất hiện trong $R$, với tiên đề giới thiệu $(\forall x)((x \in a) \Longleftrightarrow R)$, hoặc tương đương (nếu $x$ không phải là một hằng số của $\mathscr{T}$) $(x \in a) \Longleftrightarrow R$.

Nói một cách trực giác, nói rằng $R$ xác định tập theo $x$ có nghĩa là tồn tại một tập hợp $a$ sao cho các đối tượng $x$ có tính chất $R$ chính xác là các phần tử của $a$.

*Ví dụ*

#### Ví dụ 1 {#ens-ii-s1-n4-exa-1 .statement tag=03RZ}

Quan hệ $x \in y$ rõ ràng là xác định tập theo $x$.

#### Ví dụ 2 {#ens-ii-s1-n4-exa-2 .statement tag=03S0}

Quan hệ $x \neq x$ *không xác định tập theo $x$*; nói cách khác, (not $\operatorname{Coll}_x(x \neq x)$) là một định lý. Ta sẽ lập luận bằng phản chứng và giả sử rằng $x \neq x$ xác định tập. Gọi $a$ là một hằng số phụ, phân biệt với $x$ và với các hằng số của lý thuyết, cùng với tiên đề mở đầu

$$
(\forall x)((x \neq x) \Longleftrightarrow (x \in a)).
$$

Khi đó quan hệ

$$
(a \neq a) \Longleftrightarrow (a \in a)
$$

là đúng theo C30 (Chương I, §4, no. 3). Phương pháp tuyển của các trường hợp (Chương I, §3, no. 3) trước hết cho thấy rằng quan hệ $a \neq a$ là đúng, rồi rằng quan hệ $a \in a$ là đúng, điều này là phi lý.

**C49.** *Cho $R$ là một quan hệ và $x$ là một chữ cái. Nếu $R$ xác định tập theo $x$, thì quan hệ $(\forall x)((x \in y) \Longleftrightarrow R)$, trong đó $y$ là một chữ cái phân biệt với $x$ và không xuất hiện trong $R$, là phiếm hàm theo $y$.*

Điều này suy ra ngay lập tức từ C48.

Rất thường xuyên trong phần sau chúng ta sẽ có sẵn một định lý có dạng $\operatorname{Coll}_xR$. Để biểu diễn số hạng

$$
\tau_y(\forall x)((x \in y) \Longleftrightarrow R),
$$

mà không phụ thuộc vào sự lựa chọn chữ cái $y$ (phân biệt với $x$ và không xuất hiện trong $R$), ta sẽ giới thiệu một ký hiệu phiếm hàm $\mathcal{E}_x(R)$; số hạng tương ứng không chứa $x$. Số hạng này được ký hiệu bởi “tập hợp tất cả các $x$ sao cho $R$”. Theo định nghĩa (Chương I, §4, no. 1), quan hệ

$$
(\forall x)((x \in \mathcal{E}_x(R)) \Longleftrightarrow R)
$$

là *đồng nhất* với $\mathrm{Coll}_x R$; do đó quan hệ $R$ là *tương đương* với

$$x \in \mathscr{E}_x(R).$$

C50. *Cho $R$, $S$ là hai quan hệ và $x$ là một chữ cái. Nếu $R$ và $S$ xác định tập theo $x$, thì quan hệ $(\forall x)(R \Rightarrow S)$ tương đương với*

$$\mathscr{E}_x(R) \subset \mathscr{E}_x(S),$$

*và quan hệ $(\forall x)(R \Leftrightarrow S)$ tương đương với $\mathscr{E}_x(R) = \mathscr{E}_x(S)$.*

Điều này suy ra ngay lập tức từ chú ý trước đó, từ Định nghĩa 1 và từ tiên đề A1.

### 5. TIÊN ĐỀ VỀ TẬP HỢP GỒM HAI PHẦN TỬ

A2. $\qquad\qquad (\forall x)(\forall y)\ \mathrm{Coll}_z(z = x \text{ hoặc } z = y).$

Tiên đề này nói rằng nếu $x$ và $y$ là các đối tượng, thì tồn tại một tập hợp mà các phần tử duy nhất của nó là $x$ và $y$.

#### Định nghĩa 2 {#ens-ii-s1-def-2 .statement tag=03H6}

*Tập hợp $\mathscr{E}_z (z = x \text{ hoặc } z = y)$, mà các phần tử duy nhất là $x$ và $y$, được ký hiệu bởi $\{x, y\}$.*

Vì thế, quan hệ $z \in \{x, y\}$ là tương đương với "$z = x$ hoặc $z = y$"; từ C50 suy ra rằng $\{y, x\} = \{x, y\}$.

Cho $R\{z\}$ là một quan hệ và $x, y$ là các chữ cái phân biệt với $z$. Từ các tiêu chuẩn C32, C33 (chương I, §4, no. 3), và C43 (chương I, §5, no. 1), dễ dàng suy ra rằng quan hệ $(\exists z)((z \in \{x, y\})$ and $R\{z\})$ tương đương với "$R\{x\}$ hoặc $R\{y\}$"; do đó quan hệ $(\forall z)((z \in \{x, y\}) \Rightarrow R\{z\})$ tương đương với "$R\{x\}$ và $R\{y\}$".

Tập hợp $\{x, x\}$, được ký hiệu đơn giản là $\{x\}$, được gọi là *tập hợp chỉ có một phần tử là $x$*; quan hệ $z \in \{x\}$ tương đương với $z = x$, và quan hệ $x \in \mathrm{X}$ tương đương với $\{x\} \subset \mathrm{X}$.

### 6. SƠ ĐỒ CHỌN VÀ HỢP

*Lược đồ chọn và hợp* là như sau:

S8. *Cho $R$ là một quan hệ, $x$ và $y$ là những chữ cái phân biệt, và $X$ và $Y$ là những chữ cái phân biệt với $x$ và $y$ mà không xuất hiện trong $R$. Khi đó quan hệ*

(1) $\quad (\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ và } R))$

*là một tiên đề.*

Trước hết ta hãy chỉ ra rằng quy tắc này quả thực là một lược đồ. Gọi $S$ là quan hệ (1), và hãy thay một số hạng $T$ cho một chữ cái $z$ trong $S$; theo CS8 (Chương I, §4, số 1), ta có thể giả sử rằng $x$, $y$, $X$, $Y$ phân biệt với $z$ và không xuất hiện trong $T$. Khi đó $(T|z)S$ đồng nhất với

$$(\forall y)(\exists X)(\forall x)(R' \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ và } R')),$$

trong đó $R'$ là $(T|z)R$.

Về mặt trực giác, quan hệ $(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$ có nghĩa là với mọi đối tượng $y$ đều tồn tại một tập hợp $X$ (có thể phụ thuộc vào $y$) sao cho các đối tượng $x$ có quan hệ $R$ với đối tượng $y$ đã cho là các phần tử của $X$ (nhưng không nhất thiết là toàn bộ $X$). Sơ đồ chọn và hợp khẳng định rằng nếu điều đó đúng và nếu $Y$ là một tập hợp bất kỳ, thì tồn tại một tập hợp mà các phần tử của nó chính xác là các đối tượng $x$ có quan hệ $R$ với ít nhất một đối tượng $y$ của tập hợp $Y$.

C51. *Cho $P$ là một quan hệ, $A$ là một tập hợp, và $x$ là một chữ cái không xuất hiện trong $A$. Khi đó quan hệ "$P$ và $x \in A$" là xác định tập theo $x$.*

Kí hiệu $R$ là quan hệ "$P$ và $x = y$", trong đó $y$ là một chữ cái phân biệt với $x$, không xuất hiện trong cả $P$ lẫn $A$. Quan hệ

$$(\forall x)(R \Rightarrow (x \in \{y\}))$$

là đúng theo C27 (chương I, §4, số 1). Lấy $X$ là một chữ cái phân biệt với $x$ và $y$ không xuất hiện trong $P$. Quan hệ đứng trước đồng nhất với $(\{y\}|X)((\forall x)(R \Rightarrow (x \in X)))$ (vì $x$ phân biệt với $y$), và do đó quan hệ $(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$ là đúng theo S5 và C27 (chương I, §4, các số 1 và 2). Suy ra từ S8 và C30 (chương I, §4, số 3) rằng quan hệ

$$(A|Y)\ \mathrm{Coll}x(\exists y)(y \in Y \text{ và } R)$$

(nơi $Y$ là một chữ cái không xuất hiện trong $R$) là đúng, và quan hệ này đồng nhất với $\mathrm{Coll}_x(\exists y)(y \in A \text{ và } R)$ (vì cả $x$ lẫn $y$ đều không xuất hiện trong $A$). Sau cùng, quan hệ "$y \in A$ và $R$" tương đương với "$x = y$ và $x \in A$ và $P$" theo C43 (Chương I, §5, no. 1); vì $x$ không xuất hiện trong cả $P$ lẫn $A$, quan hệ

$$(\exists y)(x = y \text{ và } x \in A \text{ và } P)$$

tương đương với "$((\exists y)(x = y))$ và $x \in A$ và $P$" theo C33 (Chương I, §4, no. 3) và do đó với "$P$ và $x \in A$" vì $(\exists y)(x = y)$ là đúng.

¶ Tập hợp $\mathscr{E}_x(P$ và $x \in A)$ được gọi là *tập hợp của mọi $x \in A$ sao cho $P$* (\* do đó ta có thể nói đến tập hợp của mọi số thực sao cho $P_*$).

C52. *Cho $R$ là một quan hệ, $A$ là một tập hợp, và $x$ là một chữ cái không xuất hiện trong $A$. Nếu quan hệ $R \Rightarrow (x \in A)$ là một định lý, thì $R$ xác định tập theo $x$.*

Thật vậy, khi đó $R$ tương đương với "$R$ và $x \in A$".

#### Nhận xét {#ens-ii-s1-n6-rem-1 .statement tag=03H7}

Cho $R$ là một quan hệ xác định tập theo $x$, và cho $S$ là một quan hệ sao cho $(\forall x)(S \Rightarrow R)$ là một định lý. Khi đó $S$ xác định tập theo $x$; vì $R$ tương đương với $x \in \mathscr{E}_x(R)$, nên

$$S \Rightarrow (x \in \mathscr{E}_x(R))$$

là một định lý, và mệnh đề suy ra từ C52. Cũng lưu ý rằng trong trường hợp này ta có $\mathscr{E}_X(S) \subset \mathscr{E}_X(R)$ theo C50.

C53. *Cho $T$ là một số hạng, $A$ là một tập hợp, $x$ và $y$ là hai chữ cái phân biệt. Giả sử rằng $x$ không xuất hiện trong $A$ và $y$ không xuất hiện trong $A$ cũng không trong $T$. Khi đó quan hệ $(\exists x)(y = T$ và $x \in A)$ là xác định tập theo $y$.*

Đặt $R$ là quan hệ $y = T$. Quan hệ $(\forall y)(R \Rightarrow (y \in \{T\}))$ là đúng, do đó $(\forall x)(\exists X)(\forall y)(R \Rightarrow (y \in X))$ cũng đúng, trong đó $X$ là một chữ cái, phân biệt với $y$, không xuất hiện trong $R$. Theo S8, quan hệ $(\exists x)(x \in A$ và $R)$ là xác định tập đối với $y$, và C53 đã được chứng minh.

¶ Quan hệ $(\exists x)(y = T$ và $x \in A)$ thường được đọc như sau: "$y$ có thể được viết dưới dạng $T$ với một $x$ nào đó thuộc $A$". Tập hợp

$$\mathscr{E}_y((\exists x)(y = T \text{ và } x \in A))$$

nói chung được gọi là *tập hợp các đối tượng có dạng $T$ với $x \in A$*. Tập hợp được ký hiệu như vậy không chứa $x$ cũng không chứa $y$, và không phụ thuộc vào lựa chọn chữ cái $y$ thỏa mãn các điều kiện của C53.

### 7. PHẦN BÙ CỦA MỘT TẬP HỢP. TẬP RỖNG

Quan hệ $(x \notin \mathrm{A}$ và $x \in \mathrm{X})$ xác định tập theo $x$ bởi C51.

#### Định nghĩa 3 {#ens-ii-s1-def-3 .statement tag=03H8}

*Cho* $\mathrm{A}$ *là một tập con của một tập hợp* $\mathrm{X}$. *Tập hợp các phần tử của* $\mathrm{X}$ *không thuộc* $\mathrm{A}$, *tức là tập hợp* $\mathscr{E}x$ $(x \notin \mathrm{A}$ *và* $x \in \mathrm{X})$, *được gọi là phần bù của* $\mathrm{A}$ *trong* $\mathrm{X}$, *và được ký hiệu bởi* $\complement_{\mathrm{X}}\mathrm{A}$ *hoặc* $\mathrm{X} - \mathrm{A}$ (hoặc bởi $\complement\mathrm{A}$ nếu không có nguy cơ nhầm lẫn).

Cho A là một tập con của một tập hợp X; khi đó các quan hệ "$x \in \mathrm{X}$ và $x \notin \mathrm{A}$" và $x \in \complement_{\mathrm{X}}\mathrm{A}$ là tương đương. Do đó quan hệ "$x \in \mathrm{X}$ và $x \notin \complement_{\mathrm{X}}\mathrm{A}$" là tương đương với "$x \in \mathrm{X}$ và $(x \notin \mathrm{X}$ hoặc $x \in \mathrm{A})$", vì thế tương đương với

$x \in A$. Nói cách khác, $A = \complement_X(\complement_X A)$ là một quan hệ đúng. Tương tự, ta chứng minh được rằng nếu B là một tập con của X, thì các quan hệ $A \subset B$ và $\complement_X B \subset \complement_X A$ là tương đương.

#### Định lý 1 {#ens-ii-s1-thm-1 .statement tag=03H9}

*Quan hệ* $(\forall x)(x \notin X)$ *là phiếm hàm theo* X.

Đối với quan hệ $(\forall x)(x \notin X)$ kéo theo $(\forall Y)(X \subset Y)$; do Tiên đề ngoại diên, quan hệ $(\forall x)(x \notin X)$ vì thế là đơn trị theo X. Mặt khác, quan hệ $(\forall x)(x \notin \complement_Y Y)$ là đúng, điều này chứng tỏ rằng $(\exists X)(\forall x)(x \notin X)$ là đúng.

¶ Số hạng $\tau_x((\forall x)(x \notin X))$ tương ứng với quan hệ phiếm hàm này được biểu diễn bởi ký hiệu phiếm hàm $\emptyset$, và được gọi là *tập rỗng* (\*)[^1]; quan hệ $(\forall x)(x \notin X)$, tương đương với $X = \emptyset$, được đọc như sau: "*tập hợp* X *là rỗng*". Ta có các định lý $x \notin \emptyset$, $\emptyset \subset X$, $\complement_X X = \emptyset$, $\complement_X \emptyset = X$. Quan hệ $X \subset \emptyset$ tương đương với $X = \emptyset$. Nếu $R\{x\}$ là một quan hệ, thì quan hệ $(\forall x)((x \in \emptyset) \Rightarrow R\{x\})$ là đúng.

#### Nhận xét {#ens-ii-s1-n7-rem-1 .statement tag=03PB}

Không tồn tại tập hợp nào mà mọi đối tượng đều là một phần tử của nó; nói cách khác, "not $(\exists X)(\forall x)(x \in X)$" là một định lý. Thật vậy, nếu có một tập hợp như vậy, thì theo C52 mọi quan hệ đều sẽ xác định tập. Nhưng ta đã thấy (no. 4) rằng quan hệ $x \notin x$ không xác định tập.

### Bài tập {#ens-ii-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).

[^1]: (\*) Số hạng được ký hiệu bởi $\emptyset$ vì thế là $\tau \neg \neg \in \tau \neg \neg \in \square\square\square$.
