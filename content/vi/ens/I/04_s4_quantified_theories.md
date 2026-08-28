---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 4
section_title: Quantified theories
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 36-44, 58-59
pdf_pages: 0043-0051, 0065-0066
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF QUANTIFIERS
      page: 36
      pdf_page: 43
    - "no": 2
      title: AXIOMS OF QUANTIFIED THEORIES
      page: 37
      pdf_page: 44
    - "no": 3
      title: PROPERTIES OF QUANTIFIERS
      page: 38
      pdf_page: 45
    - "no": 4
      title: TYPICAL QUANTIFIERS
      page: 41
      pdf_page: 48
statements: 0
exercises: 8
content_sha256: 624620524dc56562f360419349b801cb616480461522f91e89d9e1d2284ab7ef
translated_from: content/en/ens/I/04_s4_quantified_theories.md
source_content_sha256: 07568a80b2b793e5dd22b88d7dc9caf03ded631f676da9f844c975c64e8b5a2c
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-c460cede
glossary_version: 34
glossary_terms_sha256: 68fec265884abb3b75a11363ed7daaa48843d2c8546170ee0b7e4a0418566388
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 4. CÁC LÝ THUYẾT CÓ LƯỢNG TỪ

### 1. ĐỊNH NGHĨA CÁC LƯỢNG TỪ

Các dấu lôgic duy nhất đã đóng vai trò trong § 3 là $\neg$ và $\vee$. Các quy tắc mà ta sẽ phát biểu bây giờ chủ yếu liên quan đến việc sử dụng các dấu lôgic $\tau$ và $\square$.

¶ Nếu $R$ là một tập hợp và $x$ là một chữ cái, tập hợp $(\tau_x(R)|x)R$ được ký hiệu bằng "tồn tại $x$ sao cho $R$", hoặc bằng $(\exists x)R$. Tập hợp

$$\text{"không } ((\exists x) \text{ không } R)\text{"}$$

được ký hiệu là "với mọi $x$, $R$", hoặc là "với mỗi $x$, $R$", hoặc bởi $(\forall x)R$. Các ký hiệu viết tắt $\exists$ và $\forall$ lần lượt được gọi là *lượng từ tồn tại* và *lượng từ phổ quát*. Chữ cái $x$ không xuất hiện trong dãy ký hiệu được ký hiệu bởi $\tau_x(R)$ *và do đó không xuất hiện* trong các dãy ký hiệu được ký hiệu bởi $(\exists x)R$ và $(\forall x)R$.

CS8. *Cho $R$ là một cấu trúc và cho $x$ và $x'$ là các chữ. Nếu $x'$ không xuất hiện trong $R$, thì $(\exists x)R$ và $(\forall x)R$ lần lượt đồng nhất với $(\exists x')R'$ và $(\forall x')R'$, trong đó $R'$ là $(x'|x)R$.*

Đối với $(\tau_x(R)|x)R$ đồng nhất với $(\tau_x(R)|x')R'$ theo CS1 (§ 1, no. 2), và $\tau_x(R)$ đồng nhất với $\tau_{x}'(R')$ theo CS3 (§ 1, no. 2). Do đó $(\exists x)R$ đồng nhất với $(\exists x')R'$. Suy ra $(\forall x)R$ đồng nhất với $(\forall x')R'$.

CS9. *Cho $R$ và $U$ là các dãy ký hiệu và cho $x$ và $y$ là các chữ cái phân biệt. Nếu $X$ không xuất hiện trong $U$, thì $(U|y)(\exists x)R$ và $(U|y)(\forall x)R$ lần lượt đồng nhất với $(\exists x)R'$ và $(\forall x)R'$, trong đó $R'$ là $(U|y)R$.*

Vì, theo CS2 (§ 1, no. 2), $(U|y)(\tau x(R)|x)R$ đồng nhất với

$$(T|x)(U|y)R,$$

trong đó $T$ là $(U|y)\tau_x(R)$, tức là $\tau_x(R')$, theo CS4 (§ 1, no. 2). Do đó $(U|y)(\exists x)R$ đồng nhất với $(\exists x)R'$, và do đó $(U|Y)(\forall x)R$ đồng nhất với $(\forall x)R'$.

CF11. *Nếu $R$ là một quan hệ trong một lý thuyết $\mathscr{T}$ và nếu $x$ là một chữ cái, thì $(\exists x)R$ và $(\forall x)R$ là các quan hệ trong $\mathscr{T}$.*

Điều này suy ra ngay lập tức từ CF3, CF8 và CF2 (§ 1, no. 4).

Xét một cách trực giác, ta hãy coi $R$ là biểu diễn một tính chất của đối tượng được ký hiệu bởi $x$. Theo ý nghĩa trực giác của số hạng $\tau_x(R)$, mệnh đề $(\exists x)R$ có nghĩa là tồn tại một đối tượng có tính chất $R$. Mệnh đề "không $(\exists x)$(không $R$)" có nghĩa là không có đối tượng nào có tính chất "không $R$", và do đó mọi đối tượng đều có tính chất $R$.

Trong một lý thuyết lôgic $\mathscr{T}$, nếu ta có một định lý có dạng $(\exists x)R$, trong đó chữ cái $x$ không phải là một hằng của $\mathscr{T}$, định lý này có thể dùng làm một định lý hợp thức hóa trong phương pháp hằng phụ (§ 3, no. 3), bởi vì nó đồng nhất với $(\tau_x(R)|x)R$. Gọi $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm $R$ vào các tiên đề của $\mathscr{T}$. Nếu ta có thể chứng minh một quan hệ $S$, trong đó $x$ không xuất hiện, trong lý thuyết $\mathscr{T}'$, thì $S$ là một định lý trong $\mathscr{T}$.

C26. *Cho $\mathscr{T}$ là một lý thuyết lôgic, cho $R$ là một quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái. Khi đó các quan hệ $(\forall x)R$ và $(\tau_x(\text{không } R)|x)R$ là tương đương trong $\mathscr{T}$.*

Vì $(\forall X)R$ đồng nhất với "không $(\tau_x(\text{không } R)|x)(\text{không } R)$" và do đó với "không không $(\tau_x(\text{không } R)|x)R$".

C27. *Nếu $R$ là một định lý trong một lý thuyết lôgic $\mathscr{T}$ trong đó chữ cái $x$ không phải là một hằng, thì $(\forall x)R$ là một định lý trong $\mathscr{T}$.*

Đối với $(\tau_x(\text{không } R)|X)R$ là một định lý trong $\mathscr{T}$, theo C3 (§ 2, no. 3).

Mặt khác, nếu $x$ là một hằng của $\mathscr{T}$, tính đúng của $R$ không kéo theo tính đúng của $(\forall x)R$. Trực giác là, sự kiện rằng $R$ là một tính chất đúng của $x$, là một đối tượng xác định của $\mathscr{T}$, rõ ràng không kéo theo rằng $R$ là một tính chất đúng của mọi đối tượng.

C28. *Cho $\mathscr{T}$ là một lý thuyết lôgic, cho $R$ là một quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái. Khi đó các quan hệ* "không $(\forall x)R$" *và $(\exists x)(\text{không } R)$ là tương đương trong $\mathscr{T}$.*

Vì "không $(\forall x)R$" đồng nhất với "không không $(\exists x)(\text{không } R)$".

### 2. TIÊN ĐỀ CỦA CÁC LÝ THUYẾT CÓ LƯỢNG TỪ

Một *lý thuyết có lượng từ* là một lý thuyết bất kỳ $\mathscr{T}$ trong đó các lược đồ S1 đến S4 (§ 3, no. 1) và lược đồ S5 dưới đây cung cấp các tiên đề ngầm.

S5. *Nếu $R$ là một quan hệ trong $\mathscr{T}$, nếu $T$ là một số hạng trong $\mathscr{T}$, và nếu $x$ là một chữ cái, thì quan hệ $(T|x)R \Rightarrow (\exists x)R$ là một tiên đề.*

Quy tắc này quả thực là một lược đồ. Vì $A$ là một tiên đề của $\mathscr{T}$ thu được bằng cách áp dụng S5; khi đó có một quan hệ $R$ trong $\mathscr{T}$, một số hạng $T$ trong $\mathscr{T}$, và một chữ cái $x$ sao cho $A$ là $(T|x)R \Rightarrow (\exists x)R$. Gọi $U$ là một số hạng trong $\mathscr{T}$ và $y$ là một chữ cái. Ta sẽ chứng minh rằng $(U|y)A$ cũng có thể thu được bằng cách áp dụng S5. Dùng CS1 (§1, no. 2) và CS8 (no. 1), ta có thể tự giới hạn vào trường hợp $x$ phân biệt với $y$ và không xuất hiện trong $U$. Gọi $R'$ là quan hệ $(U|y)R$ và $T'$ là số hạng $(U|y)T$. Các tiêu chuẩn CS2 (§1, no. 2) và CS9 (no. 1) chỉ ra rằng $(U|y)A$ đồng nhất với $(T'|x)R' \Rightarrow (\exists x)R'$.

Lược đồ S5 nói rằng nếu có một đối tượng $T$ mà đối với nó quan hệ $R$, được xem như biểu thị một tính chất của $x$, là đúng, thì $R$ là đúng đối với đối tượng $\tau_x(R)$; điều này phù hợp với ý nghĩa trực giác mà ta đã gán cho $\tau_x(R)$ (§1, no. 3, Nhận xét).

### 3. CÁC TÍNH CHẤT CỦA LƯỢNG TỪ

Từ nay về sau ta sẽ chỉ phải xét các lý thuyết có lượng từ. Trong phần còn lại của tiết này, $\mathscr{T}$ sẽ ký hiệu một lý thuyết như vậy, và $\mathscr{T}_0$ sẽ ký hiệu lý thuyết không có các tiên đề tường minh, có cùng các dấu hiệu với $\mathscr{T}$ và các lược đồ duy nhất là từ S1 đến S5. $\mathscr{T}$ mạnh hơn $\mathscr{T}_0$.

C29. *Cho $R$ là một quan hệ trong $\mathscr{T}$ và cho $x$ là một chữ cái. Khi đó các quan hệ "không $(\exists x)R$" và $(\forall x)(\text{không } R)$ là tương đương trong $\mathscr{T}$.*

Chỉ cần chứng minh tiêu chuẩn trong lý thuyết $\mathscr{T}_0$ trong đó $x$ không phải là một hằng. Định lý $R \Leftrightarrow (\text{không không } R)$ cho ta, theo C3 (§2, no. 3), các định lý
$$(\exists x)R \Rightarrow (\tau_x(R)|x)(\text{không không } R)$$
và
$$(\exists x)(\text{không không } R) \Rightarrow (\tau_x(\text{không không } R)|X)R.$$

Áp dụng S5, ta suy ra các định lý trong $\mathscr{T}_0$
$$(\exists x)R \Rightarrow (\exists x)(\text{không không } R), \quad (\exists x)(\text{không không } R) \Rightarrow (\exists x)R,$$
do đó định lý $(\exists x)R \Leftrightarrow (\exists x)(\text{không không } R)$. Bây giờ
$$(\exists x)(\text{không không } R)$$
là tương đương trong $\mathscr{T}_0$ với "không không $(\exists x)(\text{không không } R)$", nghĩa là với "không $(\forall x)(\text{không } R)$". Do đó có kết quả.

Các tiêu chuẩn C28 và C29 cho phép ta suy ra các tính chất của một trong các lượng từ từ các tính chất của lượng từ kia.

C30. *Cho $R$ là một quan hệ trong $\mathscr{T}$, cho $T$ là một số hạng trong $\mathscr{T}$, và cho $x$ là một chữ cái. Khi đó quan hệ $(\forall x)R\Longrightarrow(T|x)R$ là một định lý trong $\mathscr{T}$.*

Theo S5, $(T|x)(\text{không }R)\Longrightarrow(\tau_x(\text{không }R)|x)(\text{không }R)$ là một tiên đề. Quan hệ này đồng nhất với

$$
(\text{không }(T|x)R)\Longrightarrow\text{không}(\tau_x(\text{không }R)|x)R.
$$

Suy ra $(\tau_x(\text{không }R)|x)R\Longrightarrow(T|x)R$ là một định lý trong $\mathscr{T}$. Bây giờ dùng C26 (no. 1).

Cho $R$ là một quan hệ trong $\mathscr{T}$. Theo C26, C27 và C30, điều đó là như nhau (với điều kiện chữ cái $x$ không là một hằng của $\mathscr{T}$) dù ta phát biểu định lý $R$ trong $\mathscr{T}$, hay định lý $(\forall x)R$, hay quy tắc siêu toán học: nếu $T$ là một số hạng bất kỳ trong $\mathscr{T}$, thì $(T|x)R$ là một định lý trong $\mathscr{T}$.

C31. *Cho $R$ và $S$ là các quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái không phải là một hằng của $\mathscr{T}$. Nếu $R\Longrightarrow S$ (resp. $R\Longleftrightarrow S$) là một định lý trong $\mathscr{T}$, thì*

$$
(\forall x)R\Longrightarrow(\forall x)S,\qquad(\exists x)R\Longrightarrow(\exists x)S
$$

$$
[\text{resp. }(\forall x)R\Longleftrightarrow(\forall x)S,\qquad(\exists x)R\Longleftrightarrow(\exists x)S]
$$

*là các định lý trong $\mathscr{T}$.*

Giả sử rằng $R\Longrightarrow S$ là một định lý trong $\mathscr{T}$. Ta thêm giả thiết $(\forall x)R$ (trong đó $x$ không xuất hiện). Khi đó $R$, do đó $S$, và vì vậy cả $(\forall x)S$ cũng đúng. Do đó $(\forall x)R\Longrightarrow(\forall x)S$ là một định lý trong $\mathscr{T}$. Suy ra rằng nếu $R\Longleftrightarrow S$ là một định lý trong $\mathscr{T}$, thì cũng vậy đối với

$$
(\forall x)R\Longleftrightarrow(\forall x)S.
$$

Các quy tắc liên quan đến $\exists$ bây giờ có thể được suy ra bằng cách sử dụng C29.

C32. *Cho $R$ và $S$ là các quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái. Khi đó các quan hệ*

$$
(\forall x)(R\text{ và }S)\Longleftrightarrow((\forall x)R\text{ và }(\forall x)S),
$$

$$
(\exists x)(R\text{ hoặc }S)\Longleftrightarrow((\exists x)R\text{ hoặc }(\exists x)S)
$$

*là các định lý trong $\mathscr{T}$.*

Đủ để chứng minh các tiêu chuẩn này trong $\mathscr{T}_0$, trong đó $x$ không phải là một hằng. Nếu $(\forall x)(R\text{ và }S)$ là đúng, thì “$R$ và $S$” là đúng, và do đó mỗi quan hệ $R$, $S$ là đúng. Do đó mỗi quan hệ $(\forall x)R$, $(\forall x)S$ là đúng, và suy ra “$(\forall x)R$ và $(\forall x)S$” là đúng. Tương tự, ta chứng minh rằng nếu “$(\forall x)R$ và $(\forall x)S$” là đúng, thì $(\forall x)(R\text{ và }S)$ là đúng. Suy ra định lý thứ nhất. Định lý thứ hai suy ra bằng cách áp dụng C29.

Cần lưu ý rằng nếu $(\forall x) (R$ or S) là một định lý trong $\mathscr{T}$, ta không thể kết luận rằng $((\forall x)R$ or $(\forall x)S)$ là một định lý trong $\mathscr{T}$. Về trực giác, nói rằng quan hệ $(\forall x) (R$ or S) là đúng có nghĩa là với mỗi đối tượng $x$, ít nhất một trong các quan hệ $R$, $S$ là đúng; nhưng nói chung chỉ một trong hai quan hệ sẽ đúng, và việc đó là $R$ hay $S$ sẽ phụ thuộc vào lựa chọn của $x$. Tương tự, nếu $((\forall x)R$ and $(\exists x)S)$ là một định lý trong $\mathscr{T}$, ta không thể kết luận rằng $(\exists x)(R$ and S) là một định lý trong $\mathscr{T}$. Tuy nhiên, có tiêu chuẩn sau:

C33. *Cho $R$ và $S$ là các quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ không xuất hiện trong $R$. Khi đó các quan hệ*

$$(\forall x)(R \text{ hoặc } S) \iff (R \text{ hoặc } (\forall x)S),$$
$$(\exists x)(R \text{ và } S) \iff (R \text{ và } (\exists x)S)$$

*là các định lý trong $\mathscr{T}$.*

Chỉ cần thiết lập tiêu chuẩn trong $\mathscr{T}_0$, trong đó $x$ không phải là một hằng. Gọi $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm $(\forall x)(R$ or S) vào các tiên đề của $\mathscr{T}_0$. Trong $\mathscr{T}'$, "$R$ or $S$", và do đó (not $R$) $\Rightarrow S$, là các định lý. Nếu "not $R$" là đúng (một giả thiết trong đó $x$ không xuất hiện), thì $S$ và do đó cả $(\forall x)S$ cũng đúng. Do đó

$$(\text{không } R) \Rightarrow (\forall x)S$$

là một định lý trong $\mathscr{T}'$, và do đó $(\forall x)(R$ hoặc $S) \Rightarrow (R$ hoặc $(\forall x)S)$ là một định lý trong $\mathscr{T}_0$. Tương tự, nếu "$R$ hoặc $(\forall x)S$" là đúng, thì "$R$ hoặc $S$" và do đó $(\forall x)(R$ hoặc S) là đúng. Do đó

$$(R \text{ hoặc } (\forall x)S) \Rightarrow (\forall x)(R \text{ hoặc } S)$$

là một định lý trong $\mathscr{T}_0$. Quy tắc liên quan đến $\exists$ suy ra bằng cách áp dụng C29.

C34. *Cho $R$ là một quan hệ và cho $x$ và $y$ là các chữ. Khi đó các quan hệ*

$$(\forall x)(\forall y)R \iff (\forall y)(\forall x)R,$$
$$(\exists x)(\exists y)R \iff (\exists y)(\exists x)R,$$
$$(\exists x)(\forall y)R \implies (\forall y)(\exists x)R$$

*là các định lý trong $\mathscr{T}$.*

Chỉ cần chứng minh các định lý này trong $\mathscr{T}_0$, trong đó $x$ và $y$ không phải là các hằng. Nếu $(\forall x)(\forall y)R$ là đúng, thì $(\forall y)R$, và do đó $R$, suy ra $(\forall x)R$, suy ra $(\forall y)(\forall x)R$, đều là đúng. Tương tự, nếu $(\forall y)(\forall x)R$ là đúng, thì $(\forall x)(\forall y)R$ là đúng; và định lý thứ nhất được suy ra. Định lý thứ hai bây giờ được suy ra bằng cách sử dụng C29. Cuối cùng, vì $(\forall y)R \Rightarrow R$ là một định lý trong $\mathscr{T}_0$, nên theo C31, $(\exists x)(\forall y)R \Rightarrow (\exists x)R$ cũng là một định lý; nếu $(\exists x)(\forall y)R$ là đúng, thì $(\exists x)R$ là đúng, và do đó $(\forall y)(\exists x)R$ cũng là đúng. Suy ra định lý thứ ba.

Mặt khác, nếu $(\forall y)(\exists x)R$ là một định lý trong $\mathscr{T}$, ta không thể kết luận rằng $(\exists x)(\forall y)R$ là một định lý trong $\mathscr{T}$. Về trực giác, nói rằng quan hệ $(\forall y)(\exists x)R$ là đúng có nghĩa là, với mọi đối tượng $y$, tồn tại một đối tượng $x$ sao cho $R$ là một quan hệ đúng giữa các đối tượng $x$ và $y$. Nhưng nói chung đối tượng $x$ sẽ phụ thuộc vào lựa chọn đối tượng $y$, trong khi nói rằng $(\exists x)(\forall y)R$ là đúng có nghĩa là tồn tại một đối tượng *cố định* $x$ sao cho $R$ là một quan hệ đúng giữa đối tượng này và *mọi* đối tượng $y$.

### 4. CÁC LƯỢNG TỪ ĐIỂN HÌNH

Cho $A$ và $R$ là các dãy ký hiệu và cho $x$ là một chữ cái. Ta ký hiệu dãy ký hiệu $(\exists x)(A$ và R) bởi $(\exists_A x)R$, và dãy ký hiệu

$$\text{“không } (\exists_A x) \text{ (không } R)\text{”}$$

bởi $(\forall_A x)R$. Các ký hiệu viết tắt $\exists_A$ và $\forall_A$ được gọi là *các lượng từ điển hình*. Nhận xét rằng chữ cái $x$ không xuất hiện trong các dãy ký hiệu được ký hiệu bởi $(\exists_A x)R$, $(\forall_A x)R$.

CS10. *Cho $A$ và $R$ là các dãy ký hiệu và cho $x$ và $x'$ là các chữ cái. Nếu $x$ không xuất hiện trong $R$ cũng như trong $A$, thì $(\exists_A x)R$ và $(\forall_A x)R$ lần lượt đồng nhất với $(\exists_{A'} x')R'$ và $(\forall_{A'} x')R'$, trong đó $R'$ là $(x'|x)R$ và $A'$ là $(x'|x)A$.*

CS11. *Cho $A$, $R$, $U$ là các dãy ký hiệu, và cho $x$, $y$ là các chữ cái phân biệt. Nếu $x$ không xuất hiện trong $U$, các dãy ký hiệu $(U|y)(\exists_A x)R$ và $(U|y)(\forall_A x)R$ tương ứng đồng nhất với $(\exists_{A'} x')R'$ và $(\forall_{A'} x')R'$, trong đó $R'$ là $(U|y)R$ và $A'$ là $(U|y)A$.*

Các quy tắc này là những hệ quả ngay lập tức của các tiêu chuẩn CS8, CS9 (no. 1), CS5 (§ 1, no. 2), và CS6 (§ 3, no. 4).

CF12. *Cho $A$ và $R$ là các quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái. Khi đó*

$$(\exists_A x)R \quad \text{và} \quad (\forall_A x)R$$

*là các quan hệ trong $\mathscr{T}$.*

Điều này suy ra trực tiếp từ CF11 (no. 1), CF9 (§ 3, no. 4), và CF2 (§ 1, no. 4).

Về mặt trực giác, hãy xem $A$ và $R$ như biểu diễn các tính chất của $x$. Có thể xảy ra rằng trong một chuỗi các chứng minh, ta chỉ quan tâm đến các đối tượng thỏa mãn $A$. Nói rằng tồn tại một đối tượng thỏa mãn $A$ sao cho $R$ có nghĩa là tồn tại một đối tượng sao cho “$A$ và $R$”; do đó có định nghĩa của $\exists_A$. Nói rằng mọi đối tượng thỏa mãn $A$ đều có tính chất $R$ có nghĩa là không có đối tượng nào thỏa mãn $A$ sao cho "không $R$"; do đó có định nghĩa của $\forall_A$. Trong thực hành, các dấu này được thay thế bằng những cụm từ khác nhau, tùy theo bản chất của quan hệ $A$. \* Ví dụ : "với mọi số nguyên $x$, $R$"; "tồn tại một phần tử $x$ của tập hợp E sao cho $R$"; và vân vân. \*

C35. *Cho $A$ và $R$ là các quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái. Khi đó các quan hệ $(\forall_A x)R$ và $(\forall x)(A \Rightarrow R)$ là tương đương trong $\mathscr{T}$.*

Vì quan hệ $(\forall_A x)R$ đồng nhất với

$$\text{"không}(\exists x)(A \text{ và } (\text{không } R))\text{"}.$$

Bây giờ, "$A$ và (không $R$)" là tương đương trong $\mathscr{T}_0$ với "không $(A \Rightarrow R)$"; do đó "không $(\exists x)(A$ và (không $R$))" là tương đương trong $\mathscr{T}_0$ với

$$\text{"không } (\exists x)(\text{không } (A \Rightarrow R))\text{"},$$

theo C31 (no. 3), và quan hệ sau cùng đồng nhất với $(\forall x)(A \Rightarrow R)$. Tiêu chuẩn do đó được thiết lập trong $\mathscr{T}_0$, và do đó trong $\mathscr{T}$.

Chúng ta sẽ thường phải chứng minh các quan hệ có dạng $(\forall_A x)R$; nói chung chúng ta sẽ sử dụng một trong hai tiêu chuẩn sau đây :

C36. *Cho $A$ và $R$ là các quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái. Gọi $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm $A$ vào các tiên đề của $\mathscr{T}$. Nếu $x$ không phải là một hằng của $\mathscr{T}$, và nếu $R$ là một định lý trong $\mathscr{T}'$, thì $(\forall_A x)R$ là một định lý trong $\mathscr{T}$.*

Đối với $A \Rightarrow R$ là một định lý trong $\mathscr{T}$, theo tiêu chuẩn suy diễn, do đó $(\forall_A x)R$ là một định lý trong $\mathscr{T}$ theo C27 (no. 1) và C35.

Trong thực hành, ta chỉ ra rằng ta sẽ sử dụng quy tắc này bằng một cụm từ chẳng hạn như "Cho $x$ là một phần tử bất kỳ sao cho $A$". Trong lý thuyết $\mathscr{T}'$ được định nghĩa như vậy, ta tìm cách chứng minh $R$. Dĩ nhiên, ta không thể khẳng định rằng bản thân $R$ là một định lý trong $\mathscr{T}$.

C37. *Cho $A$ và $R$ là các quan hệ trong $\mathscr{T}$ và cho $x$ là một chữ. Cho $\mathscr{T}'$ là lý thuyết thu được bằng cách thêm các quan hệ $A$ và "không $R$" vào các tiên đề của $\mathscr{T}$. Nếu $x$ không là một hằng của $\mathscr{T}$, và nếu $\mathscr{T}'$ là mâu thuẫn, thì $(\forall_A x)R$ là một định lý trong $\mathscr{T}$.*

Đối với lý thuyết $\mathscr{T}'$, là tương đương với lý thuyết nhận được bằng cách thêm "không $(A \Rightarrow R)$" vào các tiên đề của $\mathscr{T}$. Bằng phương pháp *reductio ad absurdum*, $A \Rightarrow R$ là một định lý trong $\mathscr{T}$, và do đó $(\forall_A x)R$ cũng là như vậy theo C27 (no. 1) và C35.

Trong thực hành, ta nói: "Giả sử tồn tại một đối tượng $x$ thỏa mãn $A$ mà $R$ là sai", và tìm cách thiết lập một mâu thuẫn.

Các tính chất của các lượng từ điển hình là tương tự với các tính chất của các lượng từ:

C38. *Cho $A$ và $R$ là các quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái. Khi đó các quan hệ*

$$\text{không } (\forall_A x)R \Leftrightarrow (\exists_A x)(\text{không } R),$$
$$\text{không } (\exists_A x)R \Leftrightarrow (\forall_A x)(\text{không } R)$$

*là các định lý trong $\mathscr{T}$.*

C39. *Cho $A$, $R$, và $S$ là các quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ không phải là hằng của $\mathscr{T}$. Nếu quan hệ $A \Rightarrow (R \Rightarrow S)$ [resp. $A \Rightarrow (R \Leftrightarrow S)$] là một định lý trong $\mathscr{T}$, thì các quan hệ*

$$(\exists_A x)R \Rightarrow (\exists_A x)S, \qquad (\forall_A x)R \Rightarrow (\forall_A x)S$$
$$[\text{resp. } (\exists_A x)R \Leftrightarrow (\exists_A x)S, \qquad (\forall_A x)R \Leftrightarrow (\forall_A x)S]$$

*là các định lý trong $\mathscr{T}$.*

C40. *Cho $A$, $R$, và $S$ là các quan hệ trong $\mathscr{T}$ và cho $x$ là một chữ cái. Khi đó các quan hệ*

$$(\forall_A x)(R \text{ và } S) \Leftrightarrow ((\forall_A x)R \text{ và } (\forall_A x)S),$$
$$(\exists_A x)(R \text{ hoặc } S) \Leftrightarrow ((\exists_A x)R \text{ hoặc } (\exists_A x)S)$$

*là các định lý trong $\mathscr{T}$.*

C41. *Cho $A$, $R$, và $S$ là các quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái không xuất hiện trong $R$. Khi đó các quan hệ*

$$(\forall_A x)(R \text{ hoặc } S) \Leftrightarrow (R \text{ hoặc } (\forall_A x)S),$$
$$(\exists_A x)(R \text{ và } S) \Leftrightarrow (R \text{ và } (\exists_A x)S)$$

*là các định lý trong $\mathscr{T}$.*

C42. *Cho $A$, $B$, $R$ là các quan hệ trong $\mathscr{T}$ và cho $x$ và $y$ là các chữ cái. Nếu $x$ không xuất hiện trong $B$, và nếu $y$ không xuất hiện trong $A$, thì các quan hệ*

$$(\forall_A x)(\forall_B y)R \Leftrightarrow (\forall_B y)(\forall_A x)R,$$
$$(\exists_A)x(\exists_B y)R \Leftrightarrow (\exists_B y)(\exists_A x)R,$$
$$(\exists_A x)(\forall_B y)R \Rightarrow (\forall_B y)(\exists_A x)R$$

*là các định lý trong $\mathscr{T}$.*

Để làm ví dụ, ta hãy chứng minh một phần của C42. Quan hệ

$$(\exists_A x)(\exists_B y) R$$

trùng với $(\exists x)(A$ và $(\exists y)(B$ và $R))$, và do đó (vì $y$ không xuất hiện trong $A$) là tương đương trong $\mathscr{T}_0$ với

$$(\exists x)(\exists y)(A \text{ và } (B \text{ và } R))$$

theo C33 và C31. Tương tự, $(\exists_B x)(\exists_A y)R$ tương đương với

$$(\exists y)(\exists x)(B \text{ và } (A \text{ và } R)).$$

Bây giờ áp dụng C31 và C34 (no. 3).

\* Như một ví dụ về việc áp dụng các tiêu chuẩn này, hãy xét quan hệ sau đây: "dãy các hàm nhận giá trị thực $(f_n)$ hội tụ đều về 0 trong $[0, 1]$". Điều này có nghĩa là "với mỗi $\varepsilon > 0$ tồn tại một số nguyên $n$ sao cho với mỗi $x \in [0, 1]$ và mỗi số nguyên $m \geqslant n$ ta có $|f_m(x)| \leqslant \varepsilon$". Giả sử ta muốn lấy phủ định của quan hệ này (chẳng hạn, để có được một chứng minh bằng phản chứng); tiêu chuẩn C38 chỉ ra rằng phủ định này tương đương với quan hệ sau đây: " tồn tại một $\varepsilon > 0$ sao cho với mỗi số nguyên $n$ tồn tại một $x \in [0, 1]$ và một $m \geqslant n$ sao cho $|f_m(x)| > \varepsilon$".

### Bài tập {#ens-i-s4-exercises}

*Trong tất cả các Bài tập của* § 4, $\mathscr{T}$ *ký hiệu một lý thuyết lượng hóa.*

Xem [các bài tập của § 4](exercises/s4/).
