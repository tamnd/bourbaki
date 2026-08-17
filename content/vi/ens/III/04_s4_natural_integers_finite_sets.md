---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 4
section_title: Natural integers. Finite sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 166-171, 230-234
pdf_pages: 0172-0177, 0236-0240
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF INTEGERS
      page: 166
      pdf_page: 172
    - "no": 2
      title: INEQUALITIES BETWEEN INTEGERS
      page: 166
      pdf_page: 172
    - "no": 3
      title: THE PRINCIPLE OF INDUCTION
      page: 168
      pdf_page: 174
    - "no": 4
      title: FINITE SUBSETS OF ORDERED SETS
      page: 170
      pdf_page: 176
    - "no": 5
      title: PROPERTIES OF FINITE CHARACTER
      page: 170
      pdf_page: 176
statements: 15
exercises: 11
content_sha256: c8023c57604e2fdb0a3fc202eabd01afd40a23eab6fb7297cfedb39c9588a207
translated_from: content/en/ens/III/04_s4_natural_integers_finite_sets.md
source_content_sha256: a6f2479eb99b8adca6c4e3e15057c1b81700e121b4ca8926b4c22732686f3d98
translation_model: gpt-5-6, gpt-5.4
translation_run: translate-vi-ebf13ef0
glossary_version: 29
glossary_terms_sha256: 5aa0d707f033e6cae3aa046c7b7600f4a480387eb9ac590dfec826249dcda422
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. SỐ NGUYÊN TỰ NHIÊN. TẬP HỮU HẠN

### 1. ĐỊNH NGHĨA CÁC SỐ NGUYÊN

#### Định nghĩa 1 {#ens-iii-s4-def-1 .statement tag=03R9}

*Một lực lượng $\alpha$ được gọi là hữu hạn nếu $\alpha \ne \alpha + 1$. Một lực lượng hữu hạn còn được gọi là số nguyên tự nhiên (hoặc đơn giản là số nguyên nếu không có nguy cơ nhầm lẫn [^1]). Một tập hợp $E$ được gọi là hữu hạn nếu $\operatorname{Card}(E)$ là một lực lượng hữu hạn; và khi đó $\operatorname{Card}(E)$ được gọi là số phần tử của $E$.*

Một họ (Chương II, § 3, no. 4) được gọi là *hữu hạn* nếu tập hợp chỉ số của nó là hữu hạn.

*Khi ta nói rằng số các đối tượng thuộc một kiểu nào đó là một số nguyên $m$, ta có nghĩa rằng các đối tượng này là các phần tử của một tập hợp hữu hạn có số phần tử là $m$. Một tập hợp có số phần tử là $m$ cũng được gọi là một tập hợp gồm $m$ phần tử.*

#### Mệnh đề 1 {#ens-iii-s4-prop-1 .statement tag=03RA}

*Một lực lượng $\alpha$ là hữu hạn khi và chỉ khi $\alpha + 1$ là hữu hạn.*

Các quan hệ $\alpha = \mathfrak{b}$ và $\alpha + 1 = \mathfrak{b} + 1$ giữa các lực lượng $\alpha$ và $\mathfrak{b}$ là tương đương (§ 3, no. 4, Mệnh đề 8); do đó, các quan hệ $\alpha \ne \alpha + 1$ và $\alpha + 1 \ne (\alpha + 1) + 1$ là tương đương.

¶ Hiển nhiên $0 \ne 1$; do đó $0$ là một số nguyên. Suy ra $1$ và $2$ là các số nguyên. Các lực lượng $2 + 1$ và $(2 + 1) + 1$ là các số nguyên, lần lượt được ký hiệu là $3$ và $4$.

### 2. CÁC BẤT ĐẲNG THỨC GIỮA CÁC SỐ NGUYÊN

#### Mệnh đề 2 {#ens-iii-s4-prop-2 .statement tag=03RB}

*Cho $n$ là một số nguyên. Khi đó mọi lực lượng $\alpha$ sao cho $\alpha \le n$ đều là một số nguyên. Nếu $n \ne 0$, tồn tại duy nhất một số nguyên $m$ sao cho $n = m + 1$, và quan hệ $\alpha < n$ tương đương với $\alpha \le m$.*

Nếu $\alpha \le n$, tồn tại một lực lượng $\mathfrak{b}$ sao cho $n = \alpha + \mathfrak{b}$ (§ 3, no. 6, Mệnh đề 13). Khi đó $(\alpha + 1) + \mathfrak{b} = (\alpha + \mathfrak{b}) + 1 = n + 1$ (§ 3, no. 3, Mệnh đề 5, Hệ quả); và vì $n \ne n + 1$, ta có

$$
(\alpha + 1) + \mathfrak{b} \ne \alpha + \mathfrak{b}.
$$

Do đó $\alpha + 1 \ne \alpha$, điều này có nghĩa là $\alpha$ là một số nguyên. Nếu $n \ne 0$, ta có $n \ge 1$ (§ 3, no. 2), và do đó tồn tại một lực lượng duy nhất $m$ such

rằng $n = m + 1$ (§ 3, no. 6, Mệnh đề 13 và no. 4, Mệnh đề 8). Vì $m \leqslant n$, nên $m$ là một số nguyên, theo điều đã chứng minh. Cuối cùng, nếu một số nguyên $a$ sao cho $a < n$, thì ta có $n = a + b$, với $b \neq 0$ (§ 3, no. 6, Mệnh đề 13); vì $b$ là một số nguyên, nên ta có $b = c + 1$ và $n = m + 1 = (a + c) + 1$. Suy ra $m = a + c$ (§ 3, no. 4, Mệnh đề 8), do đó $a \leqslant m$. Ngược lại, nếu $a \leqslant m$, thì ta có

$$a \leqslant m + 1 = n;$$

và nếu $a = n = m + 1$, ta sẽ có $a > m$, trái với giả thiết.

#### Hệ quả 1 {#ens-iii-s4-prop-2-cor-1 .statement tag=03RC}

*Mọi tập con của một tập hợp hữu hạn đều hữu hạn.*

#### Hệ quả 2 {#ens-iii-s4-prop-2-cor-2 .statement tag=03RD}

*Nếu* X *là một tập con của một tập hợp hữu hạn* E *và* X $\neq$ E, *thì*

$$\mathrm{Card}\ (\mathrm{X})\ <\ \mathrm{Card}\ (\mathrm{E}).$$

Thật vậy, X được chứa trong phần bù X$'$ của một tập con của E gồm một phần tử duy nhất; ta có $\mathrm{Card}\,(\mathrm{X}) \leqslant \mathrm{Card}\,(\mathrm{X}')$ và $\mathrm{Card}\,(\mathrm{E}) = \mathrm{Card}\,(\mathrm{X}') + 1$, do đó (Mệnh đề 2) $\mathrm{Card}\,(\mathrm{X}') < \mathrm{Card}\,(\mathrm{E})$ và *a fortiori* $\mathrm{Card}\,(\mathrm{X}) < \mathrm{Card}\,(\mathrm{E})$.

Định nghĩa 1 cho thấy rằng, ngược lại, nếu E là một tập hợp sao cho

$$\mathrm{Card}\ (\mathrm{X}) < \mathrm{Card}\ (\mathrm{E})$$

đối với mọi tập con X của E sao cho X $\neq$ E, thì E là hữu hạn.

#### Hệ quả 3 {#ens-iii-s4-prop-2-cor-3 .statement tag=03RE}

*Nếu* $f$ *là một ánh xạ của một tập hợp hữu hạn* E *vào một tập hợp* F, *thì* $f(\mathrm{E})$ *là một tập con hữu hạn của* F.

Thật vậy $\mathrm{Card}\ (f(\mathrm{E})) \leqslant \mathrm{Card}\ (\mathrm{E})$ (§ 3, no. 2, Mệnh đề 3).

#### Hệ quả 4 {#ens-iii-s4-prop-2-cor-4 .statement tag=03RF}

*Cho* E *và* F *là hai tập hợp hữu hạn có cùng số phần tử, và cho* $f$ *là một ánh xạ của* E *vào* F. *Khi đó các mệnh đề sau là tương đương :*

(a) $f$ *là một đơn ánh*;
(b) $f$ *là một toàn ánh*;
(c) $f$ *là một song ánh.*

Chỉ cần chứng minh rằng (a) và (b) là tương đương. Nếu $f$ là đơn ánh, thì $\mathrm{Card}(f(\mathrm{E})) = \mathrm{Card}\,(\mathrm{E}) = \mathrm{Card}\,(\mathrm{F})$, do đó $f(\mathrm{E}) = \mathrm{F}$ (Hệ quả 2). Nếu $f$ không đơn ánh, lấy $x$ và $x'$ là hai phần tử của E sao cho $x \neq x'$ và $f(x) = f(x')$. Khi đó, đặt $\mathrm{E}' = \mathrm{E} - \{x\}$, ta có $f(\mathrm{E}') = f(\mathrm{E})$, do đó $\mathrm{Card}(f(\mathrm{E})) \leqslant \mathrm{Card}\,(\mathrm{E}') < \mathrm{Card}\,(\mathrm{E})$ theo Hệ quả 2; nhưng vì $\mathrm{Card}\,(\mathrm{F}) = \mathrm{Card}\,(\mathrm{E})$, suy ra $f(\mathrm{E}) \neq \mathrm{F}$.

### 3. NGUYÊN LÝ QUY NẠP

C61 (Nguyên lý quy nạp). *Cho* $R\{n\}$ *là một quan hệ trong một lý thuyết* $\mathscr{T}$ *(trong đó n không phải là một hằng số của* $\mathscr{T}$*).* *Giả sử rằng quan hệ*

$$R\{0\} \quad \text{và} \quad (\forall n)((n \text{ là một số nguyên và } R\{n\}) \Rightarrow R\{n+1\})$$

*là một định lý trong* $\mathscr{T}$. *Trong các điều kiện đó, quan hệ*

$$(\forall n)((n \text{ là một số nguyên}) \Rightarrow R\{n\})$$

*là một định lý trong* $\mathscr{T}$.

Ta sẽ lập luận bằng phản chứng. Giả sử rằng quan hệ

$$(\exists n)(n \text{ là một số nguyên và } (\text{không } R\{n\}))$$

là đúng. Cho $q$ là một số nguyên sao cho "không phải $R\{q\}$" (phương pháp hằng số phụ; xem Chương I, § 3, no. 3 và § 4, no. 1). Các số nguyên $n$ sao cho "$n \leqslant q$ và (không phải $R\{n\}$)" tạo thành một tập hợp không rỗng được sắp tốt (§ 3, no. 2, Chú ý), do đó có một phần tử bé nhất $s$. Nếu $s = 0$, thì "không phải $R\{0\}$", trái với giả thiết. Nếu $s > 0$, thì $s = s' + 1$, trong đó $s'$ là một số nguyên sao cho $s' < s$ (no. 2, Mệnh đề 2). Theo định nghĩa của $s$, ta có $R\{s'\}$, nhưng khi đó giả thiết kéo theo rằng $R\{s\}$ là đúng, trái với định nghĩa của $s$.

Để áp dụng nguyên lý quy nạp thì đặc biệt cần phải chứng minh quan hệ

$$(n \text{ là một số nguyên và } R\{n\}) \Rightarrow R\{n+1\}.$$

Vì mục đích này người ta thường dùng phương pháp giả thiết phụ (chương I, § 3, no. 3), và chính vì lý do đó mà quan hệ "$n$ là một số nguyên và $R\{n\}$" (hoặc thậm chí $R\{n\}$) được gọi là *giả thiết quy nạp*.

*Chú ý*. Có nhiều tiêu chuẩn thường được dùng dưới tên gọi "nguyên lý quy nạp". Tất cả đều có thể dễ dàng suy ra từ C61, và ở đây chúng tôi chỉ ra những tiêu chuẩn quan trọng nhất trong số đó :

(1) Cho $S\{n\}$ là quan hệ

$$(\forall p)((n \text{ là một số nguyên và } p \text{ là một số nguyên và } p < n) \Rightarrow R\{p\})$$

và giả sử rằng $S\{n\}$ *kéo theo* $R\{n\}$. Khi đó quan hệ

$$(\forall n)((n \text{ là một số nguyên}) \Rightarrow R\{n\})$$

đúng. Thật vậy, quan hệ $S\{0\}$ là đúng, và theo giả thiết $S\{n\}$ suy ra $R\{n\}$; vì quan hệ $m < n + 1$ là tương đương với $m \leqslant n$ (no. 2, Mệnh đề 2), quan hệ $S\{n + 1\}$ là tương đương với "$S\{n\}$ và $R\{n\}$", do đó $S\{n\}$ suy ra $S\{n + 1\}$. Tiêu chuẩn C61 vậy chứng minh rằng quan hệ

$$(\forall n)\ ((n \text{ là một số nguyên}) \Rightarrow S\{n\})$$

là đúng, và vì $S\{n\}$ suy ra $R\{n\}$, quan hệ

$$(\forall n)\ ((n \text{ là một số nguyên}) \Rightarrow R\{n\})$$

là đúng.

(2) Cho $k$ là một số nguyên và cho $R\{n\}$ là một quan hệ sao cho quan hệ

$$R\{k\} \text{ và } (\forall n)\ ((n \text{ là một số nguyên} \geqslant k \text{ và } R\{n\}) \Rightarrow R\{n + 1\})$$

là đúng. Khi đó quan hệ

$$(\forall n)\ ((n \text{ là một số nguyên} \geqslant k) \Rightarrow R\{n\})$$

là đúng ("*quy nạp bắt đầu từ k*"). Thật vậy, cho $S\{n\}$ là quan hệ

$$(n \geqslant k) \Rightarrow R\{n\}.$$

Khi đó bởi phương pháp phân trường hợp loại trừ, ta thấy rằng $S\{0\}$ là đúng. Mặt khác, dễ dàng kiểm tra được rằng quan hệ

$$(n \text{ là một số nguyên và } S\{n\}) \Rightarrow S\{n + 1\}$$

là đúng. Suy ra từ C61 rằng quan hệ

$$(n \text{ là một số nguyên}) \Rightarrow S\{n\}$$

là đúng, điều này chứng minh mệnh đề của chúng ta.

(3) Cho $a$ và $b$ là hai số nguyên sao cho $a \leqslant b$, và cho $R\{n\}$ là một quan hệ sao cho

$$R\{a\} \text{ và } (\forall n)((n \text{ là một số nguyên và } a \leqslant n < b \text{ và } R\{n\}) \Rightarrow R\{n + 1\}).$$

Khi đó quan hệ

$$(\forall n)((n \text{ là một số nguyên và } a \leqslant n \leqslant b) \Rightarrow R\{n\})$$

là đúng. Chứng minh tương tự như trong trường hợp trước; ta lấy $S\{n\}$ là quan hệ "$(a \leqslant n < b) \Rightarrow R\{n\}$" ("*quy nạp hạn chế trên một khoảng*").

(4) Cho $a$, $b$ là hai số nguyên sao cho $a \leqslant b$, và cho $\mathrm{R}\{n\}$ là một quan hệ sao cho

$\mathrm{R}\{b\}$ và $(\forall n)((n$ là một số nguyên và $a \leqslant n < b$ và $\mathrm{R}\{n+1\}) \Rightarrow \mathrm{R}\{n\})$.

Khi đó quan hệ

$$(\forall n)((n \text{ là một số nguyên và } a \leqslant n \leqslant b) \Rightarrow \mathrm{R}\{n\})$$

là đúng. Thật vậy, ta có quan hệ

$(n$ là một số nguyên và $a \leqslant n < b$ và (không $\mathrm{R}\{n\})) \Rightarrow$ không $\mathrm{R}\{n+1\}$.

Nếu đối với một $n$ nào đó sao cho $a \leqslant n \leqslant b$ mà ta có (không phải $\mathrm{R}\{n\}$), thì từ (3) sẽ suy ra (không phải $\mathrm{R}\{b\}$), trái với giả thiết, do đó có kết quả (*"quy nạp lùi"*).

### 4. TẬP CON HỮU HẠN CỦA CÁC TẬP HỢP CÓ THỨ TỰ

#### Mệnh đề 3 {#ens-iii-s4-prop-3 .statement tag=03L9}

*Cho* E *là một tập tiền thứ tự có hướng phải* (resp. *một dàn*, resp. *một tập hợp được sắp thứ tự toàn phần*). *Khi đó mọi tập con hữu hạn khác rỗng của* E *đều bị chặn trên* (resp. *có một cận trên bé nhất và một cận dưới lớn nhất*, resp. *có một phần tử lớn nhất và một phần tử bé nhất*).

Chứng minh bằng quy nạp theo số $n$ phần tử của tập con đang xét. Kết quả là tầm thường đối với $n = 1$. Cho X là một tập con có $n + 1$ phần tử của E (với $n \geqslant 1$), và đặt $\mathrm{X} = \mathrm{Y} \cup \{x\}$, trong đó Y có $n$ phần tử và do đó không rỗng. Giả thiết quy nạp kéo theo sự tồn tại của một cận trên (resp. cận trên bé nhất, resp. phần tử lớn nhất) $y$ của Y. Vì E là có hướng phải (resp. một dàn, resp. được sắp thứ tự toàn phần), $\{x, y\}$ có một cận trên (resp. cận trên bé nhất, resp. phần tử lớn nhất), hiển nhiên đó là một cận trên (resp. cận trên bé nhất, resp. phần tử lớn nhất) của X.

#### Hệ quả 1 {#ens-iii-s4-prop-3-cor-1 .statement tag=03LA}

*Mọi tập hữu hạn được sắp thứ tự toàn phần đều được sắp tốt và có một phần tử lớn nhất.*

#### Hệ quả 2 {#ens-iii-s4-prop-3-cor-2 .statement tag=03LB}

*Mọi tập hợp có thứ tự hữu hạn đều có một phần tử cực đại.*

Vì một tập hợp như vậy là quy nạp theo Hệ quả 1 (x. § 2, no. 4, Định lý 2).

### 5. CÁC TÍNH CHẤT CÓ ĐẶC TRƯNG HỮU HẠN

#### Định nghĩa 2 {#ens-iii-s4-def-2 .statement tag=03LC}

*Cho* E *là một tập hợp. Một tập hợp* $\mathfrak{S}$ *gồm các tập con của* E *được gọi là có đặc trưng hữu hạn nếu quan hệ* $\mathrm{X} \in \mathfrak{S}$ *tương đương với quan hệ "mọi tập con hữu hạn của* X *đều thuộc* $\mathfrak{S}$".

Một tính chất $P\{X\}$ của một tập con $X$ của một tập hợp $E$ được gọi là *có đặc trưng hữu hạn* nếu tập hợp các tập con $X$ của $E$ mà đối với chúng $P\{X\}$ là đúng có đặc trưng hữu hạn.

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s4-n5-exa-1 .statement tag=03T9}

Tập hợp các tập con được sắp thứ tự toàn phần của một tập hợp có thứ tự $E$ có đặc trưng hữu hạn. Thật vậy, một tập con $X$ của $E$ được sắp thứ tự toàn phần khi và chỉ khi mọi tập con của $X$ gồm hai phần tử đều được sắp thứ tự toàn phần.

#### Ví dụ 2 {#ens-iii-s4-n5-exa-2 .statement tag=03TA}

Tập hợp mọi tập con tự do của một môđun có đặc trưng hữu hạn. Điều đó cũng đúng với tập hợp mọi tập con tự do đại số của một mở rộng của một trường.

#### Ví dụ 3 {#ens-iii-s4-n5-exa-3 .statement tag=03TB}

Tập hợp các môđun con của một môđun $E$ không có đặc trưng hữu hạn, bởi vì một tập con hữu hạn của một môđun con của $E$ không tất yếu là một môđun con của $E$. $_*$

#### Định lý 1 {#ens-iii-s4-thm-1 .statement tag=03LD}

*Mọi tập hợp $\mathfrak{S}$ các tập con của một tập hợp $E$ có đặc trưng hữu hạn đều có một phần tử cực đại (khi được sắp thứ tự bởi quan hệ bao hàm).*

Theo Định lý 2 của § 2, no. 4, chỉ cần chứng minh rằng $\mathfrak{S}$ là quy nạp. Để làm điều đó, ta sẽ chứng minh rằng nếu $\mathfrak{G}$ là một tập con bất kỳ của $\mathfrak{S}$ được sắp thứ tự toàn phần theo bao hàm, thì hợp $X$ của các tập hợp thuộc $\mathfrak{G}$ thuộc $\mathfrak{S}$ (§ 2, no. 4, Định lý 2, Hệ quả 2). Vì $\mathfrak{S}$ có đặc trưng hữu hạn, chỉ cần chứng minh rằng mọi tập con hữu hạn $Y$ của $X$ đều thuộc $\mathfrak{S}$. Bây giờ, với mỗi $y \in Y$, tồn tại một tập hợp $Z_y \in \mathfrak{G}$ sao cho $y \in Z_y$. Vì tập hợp các tập hợp $Z_y$ $(y \in Y)$ là hữu hạn và được sắp thứ tự toàn phần theo bao hàm, nên nó có một phần tử lớn nhất $S$ (no. 4, Hệ quả 1 của Mệnh đề 3); nói cách khác, tồn tại một tập hợp $S \in \mathfrak{G}$ sao cho $Y \subset S$. Nhưng vì $S \in \mathfrak{S}$ và vì $Y$ là một tập con hữu hạn của $S$, nên ta có $Y \in \mathfrak{S}$ do $\mathfrak{S}$ có đặc trưng hữu hạn; điều này hoàn tất chứng minh.

### Bài tập {#ens-iii-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).

[^1]: Khái niệm “số nguyên” sẽ được tổng quát hóa sau này, trong Đại số, nơi ta sẽ định nghĩa *các số nguyên hữu tỉ* và *các số nguyên đại số*.
