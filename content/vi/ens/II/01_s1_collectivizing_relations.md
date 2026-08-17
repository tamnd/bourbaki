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
content_sha256: 95a46ce45a3b354fbacb62fd6f63e02a9e54eba4a0947cad6928bd4905406cd7
translated_from: content/en/ens/II/01_s1_collectivizing_relations.md
source_content_sha256: f27c098283cf976dbfe884a6515c10d42a193eed1659b1a36d768d136ab18309
translation_model: hy3-free, nemotron-3.5-lightning-free, laguna-s-2.1-free, gpt-5-6, nemotron-3-ultra-free, gpt-5.4-mini
translation_run: translate-vi-99f70c1a
glossary_version: 27
glossary_terms_sha256: 373349ade6facbcaa71cd68a2853401fe6a7bccb4adc757b392eca56649cdd21
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. Các quan hệ xác định tập

### 1. LÝ THUYẾT TẬP HỢP

Lý thuyết tập hợp là một lý thuyết chứa các dấu quan hệ $=$, $\in$ và dấu thực thể $\supset$ (tất cả các dấu này đều có trọng số 2); ngoài các lược đồ S1 đến S7 đã cho trong Chương I, nó chứa lược đồ S8, sẽ được đưa vào ở no. 6, và các tiên đề tường minh A1 (no. 3.) A2 (no. 5), A3 (§ 2, no. 1), A4 (§ 5, no. 1), và A5 (Chương III, § 6, no. 1), Các tiên đề tường minh này không chứa chữ cái nào; nói cách khác, lý thuyết tập hợp là một lý thuyết *không có hằng số*.

Vì lý thuyết tập hợp là một lý thuyết bình đẳng, các kết quả của Chương I có thể áp dụng.

¶ Từ nay về sau, trừ khi điều ngược lại được phát biểu rõ ràng, chúng ta sẽ luôn lập luận trong một lý thuyết mạnh hơn (Chương I, § 2, no. 4) lý thuyết tập hợp; nếu lý thuyết không được nhắc đến, thì được giả định rằng lý thuyết tập hợp được ngụ ý. Sẽ thấy rõ trong nhiều trường hợp rằng giả thiết này là dư thừa, và độc giả không nên gặp khó khăn trong việc xác định trong lý thuyết nào yếu hơn lý thuyết tập hợp các kết quả đã phát biểu là có hiệu lực.

Nếu $T$ và $U$ là các số hạng, thì tổ hợp $\in TU$ là một quan hệ (được gọi là *quan hệ thuộc*) mà trong thực hành chúng ta viết theo một trong các cách sau : $T \in U$, $(T) \in (U)$, "$T$ thuộc $U$", "$T$ là một phần tử của $U$". Quan hệ "không $(T \in U)$" được viết là $T \notin U$.

Từ quan điểm "ngây thơ", nhiều thực thể toán học có thể được coi là các tập hợp hoặc "tập hợp" của các đối tượng. Chúng ta không tìm cách hình thức hóa khái niệm này, và trong cách diễn giải hình thức của những gì tiếp theo, từ "tập hợp" phải được coi là đồng nghĩa chặt chẽ với "số hạng". Cụ thể, các cụm từ như "cho X là một tập hợp" về nguyên tắc là khá dư thừa, vì mọi chữ cái đều là một số hạng. Các cụm từ như vậy được đưa vào chỉ để hỗ trợ cách diễn giải trực quan của văn bản.

### 2. Bao hàm

#### Định nghĩa 1 {#ens-ii-s1-def-1 .statement tag=03H5}

*Quan hệ được ký hiệu bởi* $(\forall z)((z \in x) \Rightarrow (z \in y))$, *trong đó chỉ có các chữ cái $x$ và $y$ xuất hiện, được viết theo một trong các cách sau :* $x \subset y$, $y \supset x$, *"$x$ được chứa trong $y$", "$y$ chứa $x$", "$x$ là một tập con của $y$". Quan hệ* "không $(x \subset y)$" *được viết* $x \not\subset y$ *hoặc* $y \not\supset x$.

Theo các quy định đã nêu trong Chương I, § 1, no. 1, định nghĩa này đưa ra quy ước métamatemat sau: Cho $T$ và $U$ là các dãy ký hiệu; nếu chúng ta thay thế $T$ cho $x$ và $U$ cho $y$ trong dãy $x \subset y$, chúng ta được ký hiệu bởi $T \subset U$; nếu chúng ta ký hiệu bởi $\mathbf{x}$, $\mathbf{y}$ các ký tự phân biệt từ $x$, $y$ và phân biệt với nhau, và xuất hiện không trong $T$ cũng như không trong $U$, dãy $T \subset U$ là thì bằng $(T|\mathbf{x})(U|\mathbf{y})(\mathbf{x}|x)(\mathbf{y}|y)(x \subset y,)$ và theo sau bởi CS8, CS9 (Chương I, § 4, no. 1), và CS5 (Chương I, § 1, no. 2) với $(\forall z)((z \in T) \Rightarrow (z \in U))$, mà $z$ là ký tự xuất hiện không trong $T$ cũng như không trong $U$.

Từ nay về sau, mỗi khi chúng ta phát biểu một định nghĩa toán học, chúng ta sẽ không nhắc đến quy ước siêu toán học mà nó kéo theo.

CS12. *Cho $T$, $U$, $V$ là các dãy ký hiệu và cho $x$ là một chữ cái. Khi đó dãy ký hiệu $(V|x)(T \subset U)$ đồng nhất với $(V|x)T \subset (V|x)U$.*

Điều này suy ra ngay lập tức từ CS9 (Chương I, § 4, no. 1) và CS5 (Chương I, § 1, no. 2).

CF13. *Nếu $T$ và $U$ là các thuật ngữ, thì $T \subset U$ là một quan hệ.*

Điều này suy ra ngay lập tức từ CF8 (Chương I, § 1, no. 4).

¶ Mọi quan hệ có dạng $T \subset U$ (trong đó $T$ và $U$ là các thuật ngữ) được gọi là *quan hệ bao hàm*.

Từ nay về sau, chúng ta sẽ không còn viết tường minh các tiêu chuẩn thế và các tiêu chuẩn kiến tạo theo sau các định nghĩa nữa. Tuy nhiên, cần lưu ý rằng các tiêu chuẩn này sẽ thường được sử dụng một cách ngầm trong các chứng minh.

Để chứng minh quan hệ $x \subset y$ trong một lý thuyết $\mathscr{T}$, đủ để, theo C27 (Chương I, § 4, no. 1), chứng minh rằng $z \in y$ trong lý thuyết được tạo ra bằng cách thêm $z \in x$ vào các tiên đề của $\mathscr{T}$, trong đó $z$ là một ký tự phân biệt với $x$, $y$ và các hằng của lý thuyết. Trong thực hành, chúng ta sẽ nói « giả sử $z$ là phần tử của $x$ », và chúng ta sẽ cố gằng chứng minh $z \in y$.

#### Mệnh đề 1 {#ens-ii-s1-prop-1 .statement tag=03P9}

$x \subset x$.

Hiển nhiên.

#### Mệnh đề 2 {#ens-ii-s1-prop-2 .statement tag=03PA}

$(x \subset y$ và $y \subset z) \Rightarrow (x \subset z)$.

Ghép thêm các giả thiết $x \subset y$, $y \subset z$, và $u \in x$. Khi đó các quan hệ

$$(u \in x) \Rightarrow (u \in y), \qquad (u \in y) \Rightarrow (u \in z),$$

là đúng, và do đó quan hệ $u \in z$ là đúng.

### 3. TIÊN ĐỀ NGOẠI DIÊN

*Tiên đề ngoại diên* là tiên đề sau đây :

A1. $\qquad (\forall x)(\forall y)((x \subset y \text{ và } y \subset x) \Rightarrow (x = y))$.

Về mặt trực giác, tiên đề này diễn đạt sự kiện rằng hai tập hợp có cùng các phần tử thì bằng nhau.

Để chứng minh rằng $x = y$, do đó chỉ cần chứng minh $z \in y$ trong lý thuyết thu được bằng cách thêm giả thiết $z \in x$, và $z \in x$ trong lý thuyết thu được bằng cách thêm giả thiết $z \in y$, trong đó $z$ là một chữ cái phân biệt với $x$, $y$, và các hằng.

C48. *Cho $\mathbf{R}$ là một quan hệ, $x$ một chữ cái, và $y$ một chữ cái phân biệt với $x$ mà không xuất hiện trong $\mathbf{R}$. Khi đó quan hệ $(\forall x)((x \in y) \Leftrightarrow \mathbf{R})$ là đơn trị theo $y$.*

Cho $z$ là một chữ cái phân biệt với $x$ mà không xuất hiện trong $\mathbf{R}$. Thêm các giả thiết

$$(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\forall x)((x \in z) \Leftrightarrow \mathbf{R}).$$

Khi đó ta có lần lượt các định lý

$$(\forall x)(((x \in y) \Leftrightarrow \mathbf{R}) \text{ và } ((x \in z) \Leftrightarrow \mathbf{R})),$$
$$(\forall x)((x \in y) \Leftrightarrow (x \in z)),$$
$$y \subset z, \qquad z \subset y.$$

Theo A1 ta có khi đó $y = z$. Điều này chứng minh C48.

### 4. Các quan hệ xác định tập

Cho $\mathbf{R}$ là một quan hệ và cho $x$ là một chữ cái. Nếu $y$ và $y'$ ký hiệu các chữ cái phân biệt với $x$ *mà không xuất hiện trong $\mathbf{R}$*, thì các quan hệ

$$(\exists y)(\forall x)((x \in y) \Leftrightarrow \mathbf{R}), \ (\exists y')(\forall x)((x \in y') \Leftrightarrow \mathbf{R})$$

là giống nhau theo CS8 (Chương I, §4, số 1). Quan hệ được định nghĩa như vậy (mà không chứa $x$) được ký hiệu bởi $\operatorname{Coll}_xR$.

¶ Nếu $\operatorname{Coll}_xR$ là một định lý trong một lý thuyết $\mathscr{T}$, thì $R$ được gọi là *xác định tập theo $x$* trong $\mathscr{T}$. Khi đó, ta có thể giới thiệu một hằng số phụ $a$, phân biệt với $x$ và các hằng số của $\mathscr{T}$, và không xuất hiện trong $R$, cùng với tiên đề mở đầu $(\forall x)((x \in a) \Longleftrightarrow R)$, hay tương đương (nếu $x$ không phải là một hằng số của $\mathscr{T}$) $(x \in a) \Longleftrightarrow R$.

Trực quan, nói rằng $R$ xác định tập trong $x$ là nói rằng tồn tại một tập hợp $a$ sao cho các đối tượng $x$ có tính chất $R$ chính xác là các phần tử của $a$.

*Ví dụ*

#### Ví dụ 1 {#ens-ii-s1-n4-exa-1 .statement tag=03RZ}

Quan hệ $x \in y$ rõ ràng là xác định tập trong $x$.

#### Ví dụ 2 {#ens-ii-s1-n4-exa-2 .statement tag=03S0}

Quan hệ $x \neq x$ *không xác định tập trong $x$*; nói cách khác, (không $\operatorname{Coll}_x(x \neq x)$) là một định lý. Hãy lập luận bằng phản chứng và giả sử rằng $x \neq x$ xác định tập. Cho $a$ là một hằng số phụ, phân biệt với $x$ và các hằng số của lý thuyết, với tiên đề giới thiệu

$$
(\forall x)((x \neq x) \Longleftrightarrow (x \in a)).
$$

Khi đó quan hệ

$$
(a \neq a) \Longleftrightarrow (a \in a)
$$

đúng theo C30 (chương I, §4, no. 3). Phương pháp phân chia trường hợp (chương I, §3, no. 3) trước hết cho thấy quan hệ $a \neq a$ là đúng, rồi cho thấy quan hệ $a \in a$ là đúng, điều này là vô lý.

**C49.** *Cho $R$ là một quan hệ và $x$ là một ký hiệu. Nếu $R$ là xác định tập theo $x$, quan hệ $(\forall x)((x \in y) \Longleftrightarrow R)$, trong đó $y$ là một ký hiệu phân biệt với $x$ và không xuất hiện trong $R$, là phiếm hàm theo $y$.*

Điều này suy ra ngay lập tức từ C48.

Rất thường trong phần tiếp theo, ta sẽ có trong tay một định lý có dạng $\operatorname{Coll}_xR$. Để biểu diễn số hạng

$$
\tau_y(\forall x)((x \in y) \Longleftrightarrow R),
$$

không phụ thuộc vào lựa chọn chữ $y$ (phân biệt với $x$ và không xuất hiện trong $R$), ta sẽ giới thiệu một ký hiệu phiếm hàm $\mathcal{E}_x(R)$; số hạng tương ứng không chứa $x$. Số hạng này được gọi là “tập hợp tất cả các $x$ sao cho $R$”. Theo định nghĩa (Chương I, §4, no. 1), quan hệ

$$
(\forall x)((x \in \mathcal{E}_x(R)) \Longleftrightarrow R)
$$

là *đồng nhất* với $\mathrm{Coll}_x R$; do đó quan hệ $R$ *tương đương* với

$$x \in \mathscr{E}_x(R).$$

C50. *Cho $R$, $S$ là hai quan hệ và cho $x$ là một chữ cái. Nếu $R$ và $S$ xác định tập trong $x$, thì quan hệ $(\forall x)(R \Rightarrow S)$ tương đương với*

$$\mathscr{E}_x(R) \subset \mathscr{E}_x(S),$$

*và quan hệ $(\forall x)(R \Leftrightarrow S)$ tương đương với $\mathscr{E}_x(R) = \mathscr{E}_x(S)$.*

Điều này suy ra ngay lập tức từ chú ý trước đó và từ định nghĩa 1 và tiên đề A1.

### 5. TIỀN ĐỀ CỦA TẬP HỢP HAI PHẦN TỬ

A2. $\qquad\qquad (\forall x)(\forall y)\ \mathrm{Coll}_z(z = x \text{ hoặc } z = y).$

Tiên đề này nói rằng nếu $x$ và $y$ là các đối tượng, thì tồn tại một tập hợp mà các phần tử duy nhất của nó là $x$ và $y$.

#### Định nghĩa 2 {#ens-ii-s1-def-2 .statement tag=03H6}

*Tập hợp $\mathscr{E}_z (z = x \text{ hoặc } z = y)$, mà các phần tử duy nhất của nó là $x$ và $y$, được ký hiệu bởi $\{x, y\}$.*

Quan hệ $z \in \{x, y\}$ do đó tương đương với "$z = x$ hoặc $z = y$"; suy ra từ C50 rằng $\{y, x\} = \{x, y\}$.

Cho $R\{z\}$ là một quan hệ và cho $x, y$ là các chữ cái phân biệt từ $z$. Từ các tiêu chuẩn C32, C33 (Chương I, §4, no. 3), và C43 (Chương I, §5, no. 1) dễ dàng suy ra rằng mệnh đề $(\exists z)((z \in \{x, y\})$ and $R\{z\})$ là tương đương với "$R\{x\}$ hoặc $R\{y\}$"; do đó mệnh đề $(\forall z)((z \in \{x, y\}) \Rightarrow R\{z\})$ là tương đương với "$R\{x\}$ và $R\{y\}$".

Tập hợp $\{x, x\}$, được ký hiệu đơn giản bằng $\{x\}$, được gọi là *tập hợp có phần tử duy nhất là $x$*; quan hệ $z \in \{x\}$ tương đương với $z = x$, và quan hệ $x \in \mathrm{X}$ tương đương với $\{x\} \subset \mathrm{X}$.

### 6. LƯỢC ĐỒ CHỌN VÀ HỢP

*Lược đồ chọn và hợp* là như sau :

S8. *Cho $R$ là một quan hệ, cho $x$ và $y$ là các chữ cái phân biệt, và cho $X$ và $Y$ là các chữ cái phân biệt với $x$ và $y$ mà không xuất hiện trong $R$. Khi đó quan hệ*

(1) $\quad (\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ và } R))$

*is an axiom.*

Trước hết, ta hãy chỉ ra rằng quy tắc này thực sự là một lược đồ. Cho $S$ ký hiệu quan hệ (1), và ta hãy thay thế một số hạng $T$ cho một chữ cái $z$ trong $S$; theo CS8 (Chương I, §4, no. 1) ta có thể giả sử rằng $x$, $y$, $X$, $Y$ phân biệt với $z$ và không xuất hiện trong $T$. Khi đó $(T|z)S$ đồng nhất với

$$(\forall y)(\exists X)(\forall x)(R' \Rightarrow (x \in X)) \Rightarrow (\forall Y)\ \mathrm{Coll}_X((\exists y)((y \in Y) \text{ và } R')),$$

trong đó $R'$ là $(T|z)R$.

Trực giác, quan hệ $(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$ có nghĩa là với mọi đối tượng $y$ tồn tại một tập hợp $X$ (có thể phụ thuộc vào $y$) sao cho các đối tượng $x$ có quan hệ $R$ với đối tượng $y$ đã cho là các phần tử của $X$ (nhưng không nhất thiết là toàn bộ $X$). Sơ đồ chọn và hợp khẳng định rằng nếu điều này xảy ra và nếu $Y$ là một tập hợp bất kỳ, thì tồn tại một tập hợp mà các phần tử của nó chính xác là các đối tượng $x$ có quan hệ $R$ với ít nhất một đối tượng $y$ của tập hợp $Y$.

*Cho $P$ là một quan hệ, cho $A$ là một tập hợp, và cho $x$ là một chữ cái mà không xuất hiện trong $A$. Khi đó, quan hệ "$P$ và $x \in A$" là xác định tập trong $x$.

Gọi $R$ là quan hệ "$P$ và $x = y$", trong đó $y$ là một chữ cái phân biệt với $x$ mà không xuất hiện trong $P$ cũng không xuất hiện trong $A$. Quan hệ

$$(\forall x)(R \Rightarrow (x \in \{y\}))$$

là đúng theo C27 (Chương I, §4, số 1). Cho $X$ là một chữ cái phân biệt với $x$ và $y$ mà không xuất hiện trong $P$. Quan hệ trước đó trùng với $(\{y\}|X)((\forall x)(R \Rightarrow (x \in X)))$ (bởi vì $x$ phân biệt với $y$), và do đó quan hệ $(\forall y)(\exists X)(\forall x)(R \Rightarrow (x \in X))$ là đúng nhờ S5 và C27 (Chương I, §4, số 1 và 2). Từ S8 và C30 (Chương I, §4, số 3) suy ra quan hệ

$$(A|Y)\ \mathrm{Coll}x(\exists y)(y \in Y \text{ và } R)$$

(trong đó $Y$ là một ký tự không xuất hiện trong $R$) là đúng, và quan hệ này trùng với $\mathrm{Coll}_x(\exists y)(y \in A \text{ và } R)$ (vì $x$ và $y$ đều không xuất hiện trong $A$). Cuối cùng, quan hệ "$y \in A$ và $R$" tương đương với "$x = y$ và $x \in A$ và $P$" theo C43 (Chương I, §5, số 1); vì $x$ không xuất hiện trong $P$ cũng không trong $A$, quan hệ

$$(\exists y)(x = y \text{ và } x \in A \text{ và } P)$$

là tương đương với "$((\exists y)(x = y))$ và $x \in A$ và $P$" theo C33 (Chương I, §4, no. 3) và do đó với "$P$ và $x \in A$" bởi vì $(\exists y)(x = y)$ là đúng.

Tập hợp $\mathscr{E}_x(P$ và $x \in A)$ được gọi là *tập hợp tất cả các $x \in A$ sao cho $P$* (\* như vậy chúng ta có thể nói về tập hợp tất cả các số thực sao cho $P_*$).

C52. *Cho $R$ là một quan hệ, $A$ một tập hợp, và $x$ một chữ cái không xuất hiện trong $A$. Nếu quan hệ $R \Rightarrow (x \in A)$ là một định lý, thì $R$ là xác định tập theo $x$.*

Vì $R$ khi đó tương đương với "$R$ và $x \in A$".

#### Chú ý {#ens-ii-s1-n6-rem-1 .statement tag=03H7}

Cho $R$ là một quan hệ xác định tập theo $x$, và cho $S$ là một quan hệ sao cho $(\forall x)(S \Rightarrow R)$ là một định lý. Khi đó $S$ xác định tập theo $x$; vì $R$ tương đương với $x \in \mathscr{E}_x(R)$, do đó

$$S \Rightarrow (x \in \mathscr{E}_x(R))$$

là một định lý, và mệnh đề này suy ra từ C52. Cũng lưu ý rằng trong trường hợp này ta có $\mathscr{E}_X(S) \subset \mathscr{E}_X(R)$ theo C50.

C53. *Cho $T$ là một số hạng, $A$ một tập hợp, $x$ và $y$ là các chữ cái phân biệt. Giả sử rằng $x$ không xuất hiện trong $A$ và $y$ không xuất hiện trong $A$ cũng như trong $T$. Khi đó quan hệ $(\exists x)(y = T$ và $x \in A)$ là xác định tập theo $y$.*

Cho $R$ là quan hệ $y = T$. Quan hệ $(\forall y)(R \Rightarrow (y \in \{T\}))$ là đúng, do đó $(\forall x)(\exists X)(\forall y)(R \Rightarrow (y \in X))$ cũng đúng, trong đó $X$ là một chữ cái, phân biệt với $y$, không xuất hiện trong $R$. Theo S8, quan hệ $(\exists x)(x \in A$ và $R)$ là xác định tập theo $y$, và C53 đã chứng minh.

¶ Quan hệ $(\exists x)(y = T$ và $x \in A)$ thường được đọc như sau : "$y$ có thể được đưa vào dạng $T$ với một $x$ thuộc $A$". Tập hợp

$$\mathscr{E}_y((\exists x)(y = T \text{ và } x \in A))$$

nói chung được gọi là *tập hợp các đối tượng có dạng $T$ với $x \in A$*. Hợp tử như vậy được ký hiệu không chứa $x$ cũng như $y$, và không phụ thuộc vào lựa chọn chữ cái $y$ thỏa mãn các điều kiện của C53.

### 7. PHẦN BÙ CỦA MỘT TẬP HỢP. TẬP RỖNG

Quan hệ $(x \notin \mathrm{A}$ và $x \in \mathrm{X})$ xác định tập trong $x$ bởi C51.

#### Định nghĩa 3 {#ens-ii-s1-def-3 .statement tag=03H8}

*Cho* $\mathrm{A}$ *là một tập con của một tập hợp* $\mathrm{X}$. *Tập hợp các phần tử của* $\mathrm{X}$ *mà không thuộc* $\mathrm{A}$, *tức là tập hợp* $\mathscr{E}x$ $(x \notin \mathrm{A}$ *và* $x \in \mathrm{X})$, *được gọi là phần bổ sung của* $\mathrm{A}$ *trong* $\mathrm{X}$, *và được ký hiệu bằng* $\complement_{\mathrm{X}}\mathrm{A}$ *hoặc* $\mathrm{X} - \mathrm{A}$ (hoặc bằng $\complement\mathrm{A}$ *nếu không có nguy cơ nhầm lẫn*).

Cho A là một tập con của một tập hợp X; các quan hệ "$x \in \mathrm{X}$ và $x \notin \mathrm{A}$" và $x \in \complement_{\mathrm{X}}\mathrm{A}$ thì sau đó là tương đương. Do đó, quan hệ "$x \in \mathrm{X}$ và $x \notin \complement_{\mathrm{X}}\mathrm{A}$" tương đương với "$x \in \mathrm{X}$ và $(x \notin \mathrm{X}$ hoặc $x \in \mathrm{A})$", tương đương với

$x \in A$. Nói cách khác, $A = \complement_X(\complement_X A)$ là một mệnh đề đúng. Tương tự, ta chứng minh được rằng nếu B là một tập con của X, các quan hệ $A \subset B$ và $\complement_X B \subset \complement_X A$ là tương đương.

#### Định lý 1 {#ens-ii-s1-thm-1 .statement tag=03H9}

*Quan hệ $(\forall x)(x \notin X)$ là phiếm hàm trong X.*

Đối với quan hệ $(\forall x)(x \notin X)$ suy ra $(\forall Y)(X \subset Y)$; nhờ tiên đề ngoại diên, quan hệ $(\forall x)(x \notin X)$ vì vậy là đơn trị trong X. Mặt khác, quan hệ $(\forall x)(x \notin \complement_Y Y)$ là đúng, điều này chứng minh rằng $(\exists X)(\forall x)(x \notin X)$ là đúng.

¶ Số hạng $\tau_x((\forall x)(x \notin X))$ tương ứng với quan hệ phiếm hàm này được biểu diễn bởi ký hiệu phiếm hàm $\emptyset$, và được gọi là *tập rỗng* (\*)[^1]; quan hệ $(\forall x)(x \notin X)$, mà tương đương với $X = \emptyset$, được đọc như sau: "*tập hợp* X *rỗng*". Ta có các định lý $x \notin \emptyset$, $\emptyset \subset X$, $\complement_X X = \emptyset$, $\complement_X \emptyset = X$. Quan hệ $X \subset \emptyset$ tương đương với $X = \emptyset$. Nếu $R\{x\}$ là một quan hệ, thì quan hệ $(\forall x)((x \in \emptyset) \Rightarrow R\{x\})$ là đúng.

#### Chú ý {#ens-ii-s1-n7-rem-1 .statement tag=03PB}

Không tồn tại tập hợp nào mà mọi đối tượng đều là phần tử của nó; nói cách khác, "không $(\exists X)(\forall x)(x \in X)$" là một định lý. Bởi vì nếu có tập hợp như thế, thì theo C52 mọi quan hệ đều là xác định tập. Nhưng chúng ta đã thấy (no. 4) rằng quan hệ $x \notin x$ không phải là xác định tập.

### Bài tập {#ens-ii-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).

[^1]: (\*) Số hạng được ký hiệu bởi $\emptyset$ vì vậy $\tau \neg \neg \in \tau \neg \neg \in \square\square\square$.
