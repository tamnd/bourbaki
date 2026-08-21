---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 5
section_title: Equalitarian theories
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 44-49, 59-60
pdf_pages: 0051-0056, 0066-0067
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOMS
      page: 44
      pdf_page: 51
    - "no": 2
      title: PROPERTIES OF EQUALITY
      page: 45
      pdf_page: 52
    - "no": 3
      title: FUNCTIONAL RELATIONS
      page: 47
      pdf_page: 54
statements: 3
exercises: 7
content_sha256: f27f3dc8525c189e5ce36c948b3c3269ee7cf03154ee2eae98113330f2e28726
translated_from: content/en/ens/I/05_s5_equalitarian_theories.md
source_content_sha256: 8cbe15ed2020b27b62da706075017d090591d51c972f6b3ce0f6ebf686257ba1
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-57904e7a
glossary_version: 34
glossary_terms_sha256: 6d5da34c09c0aa03e5062d4cb5433a638d6e1e0d3b29ccd80b4ab919985dab33
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. CÁC LÝ THUYẾT BÌNH ĐẲNG

### 1. CÁC TIÊN ĐỀ

Một *lý thuyết bình đẳng* là một lý thuyết $\mathscr{T}$ có một dấu quan hệ trọng số 2, được viết là $=$ (đọc là “bằng”), trong đó các lược đồ S1 đến S5 (§§3 và 4), cùng với các lược đồ S6 và S7 dưới đây, cung cấp các tiên đề ẩn. Nếu $T$ và $U$ là các hạng trong $\mathscr{T}$, phép ghép $= TU$ là một quan hệ trong $\mathscr{T}$ (gọi là *quan hệ đẳng thức*) theo CF4; trong thực hành, nó được ký hiệu bởi $T = U$ hoặc $(T) = (U)$.

S6. *Cho $x$ là một chữ cái, cho $T$ và $U$ là các hạng tử trong $\mathscr{T}$, và cho $R\{x\}$ là một quan hệ trong $\mathscr{T}$; khi đó quan hệ $(T = U) \Rightarrow (R\{T\} \Leftrightarrow R\{U\})$ là một tiên đề.*

S7. *Nếu $R$ và $S$ là các quan hệ trong $\mathscr{T}$ và $x$ là một chữ cái, thì quan hệ $((\forall x)(R \Leftrightarrow S)) \Rightarrow (\tau_x(R) = \tau_x(S))$ là một tiên đề.*

Để chứng minh rằng quy tắc S6 là một lược đồ, cho $A$ là một tiên đề của $\mathscr{T}$, thu được bằng cách áp dụng S6; khi đó có một quan hệ $R$ trong $\mathscr{T}$, các số hạng $T$ và $U$ trong $\mathscr{T}$, và một chữ $x$, sao cho $A$ là $(T = U) \Rightarrow ((T|x)R \Leftrightarrow (U|x)R)$. Ta sẽ chứng minh rằng nếu $y$ là một chữ và $V$ là một số hạng trong $\mathscr{T}$, thì quan hệ $(V|x)A$ có thể thu được bằng cách áp dụng S6. Nhờ CS1 (§1, no. 2), ta có thể giả sử rằng $x$ phân biệt với $y$ và không xuất hiện trong $V$. Gọi $T'$, $U'$, $R'$ lần lượt là các dãy ký hiệu $(V|y)T$, $(V|y)U$, $(V|y)R$. Theo CS2 và CS5 (§1, no. 2), $(V|y)A$ đồng nhất với

$$(T' = U') \Rightarrow ((T'|x')R' \Leftrightarrow (U'|x')R')$$

và chứng minh là đầy đủ. Việc kiểm chứng rằng S7 là một lược đồ cũng tương tự.

Về trực giác, lược đồ S6 có nghĩa là nếu hai đối tượng bằng nhau thì chúng có cùng các tính chất. Lược đồ S7 xa rời trực giác thông thường hơn; nó có nghĩa là nếu hai tính chất $R$ và $S$ của một đối tượng $x$ là tương đương, thì các đối tượng được phân biệt $\tau_x(R)$ và $\tau_x(S)$ (lần lượt được chọn từ các đối tượng thỏa mãn $R$, và những đối tượng thỏa mãn $S$, nếu có những đối tượng như vậy) là bằng nhau. Người đọc sẽ lưu ý rằng sự có mặt của lượng từ $\forall x$ trong S7 là cốt yếu (cf. Bài tập 7).

Phủ định của quan hệ $= TU$ được ký hiệu bởi $T \neq U$ hoặc $(T) \neq (U)$ (trong đó dấu $\neq$ được đọc là "khác với").

¶ Từ S6 ta suy ra tiêu chuẩn sau:

C43. *Cho $x$ là một chữ cái, cho $T$ và $U$ là các hạng trong $\mathscr{T}$, và cho $R\{x\}$ là một quan hệ trong $\mathscr{T}$. Khi đó các quan hệ*

$$(T = U \text{ và } R\{T\}), \qquad (T = U \text{ và } R\{U\})$$

*là tương đương.*

Bởi nếu ta thêm các giả thiết $T = U$ và $R\{T\}$, thì $R\{U\}$ đúng theo S6; do đó $(T = U$ và $R\{U\})$ là đúng.

Khi một quan hệ có dạng $T = U$ đã được chứng minh trong một lý thuyết $\mathscr{T}$, người ta thường nói (lạm dụng ngôn ngữ) rằng $T$ và $U$ “là như nhau” hoặc “đồng nhất”. Tương tự, khi $T \neq U$ đúng trong $\mathscr{T}$, ta nói rằng $T$ và $U$ “phân biệt” thay vì nói rằng $T$ khác $U$.

### 2. CÁC TÍNH CHẤT CỦA ĐẲNG THỨC

Từ nay chúng ta sẽ chỉ xét các lý thuyết bình đẳng. Cho $\mathscr{T}$ là một lý thuyết như vậy, và cho $\mathscr{T}_0$ là lý thuyết có các dấu là những dấu của $\mathscr{T}$ và có các tiên đề duy nhất là những tiên đề được cung cấp bởi các sơ đồ S1 đến S7. Lý thuyết $\mathscr{T}_0$ yếu hơn $\mathscr{T}$ (§2, no. 4) và không có hằng. Ba định lý sau đây là các định lý trong $\mathscr{T}_0$.

#### Định lý 1 {#ens-i-s5-thm-1 .statement tag=03P3}

$x = x$.

Cho $S$ là quan hệ $x = x$ trong $\mathscr{T}_0$. Theo C27 (§4, no. 1), với mọi quan hệ $R$ trong $\mathscr{T}_0$, $(\forall x)(R \Leftrightarrow R)$ là một định lý trong $\mathscr{T}_0$, và do đó, theo S7, $\tau_x(R) = \tau_x(R)$, nghĩa là $(\tau_x(R)|x)S$, là một định lý trong $\mathscr{T}_0$. Lấy $R$ là quan hệ "không $S$" và xét C26 (§4, no. 1), ta thấy rằng $(\forall x)S$ là một định lý trong $\mathscr{T}_0$. Theo C30 (§4, no. 3), $S$ do đó là một định lý trong $\mathscr{T}_0$.

Quan hệ $(\forall x)(x = x)$ cũng là một định lý trong $\mathscr{T}_0$; và nếu $T$ là một số hạng trong $\mathscr{T}_0$, thì $T = T$ là một định lý trong $\mathscr{T}_0$ (xem §4, no. 3). Có thể sau này biến đổi các định lý khác theo cùng một cách thành các định lý trong đó không xuất hiện chữ cái nào hoặc thành các tiêu chuẩn siêu toán học. Từ nay về sau chúng ta sẽ không tường minh thực hiện các biến đổi này, nhưng chúng ta sẽ thường ngầm sử dụng chúng.

#### Định lý 2 {#ens-i-s5-thm-2 .statement tag=03P4}

$(x = y) \Leftrightarrow (y = x)$.

Giả sử rằng quan hệ $x = y$ là đúng. Theo S6, quan hệ

$$(x = y) \Rightarrow ((x|y)(y = x) \Leftrightarrow (y|y)(y = x)),$$

nghĩa là

$$(x = y) \Rightarrow ((x = x) \Leftrightarrow (y = x)),$$

là đúng. Do đó $(x = x) \Leftrightarrow (y = x)$ là đúng. Theo Định lý 1 suy ra rằng $y = x$ là đúng, và định lý được chứng minh.

#### Định lý 3 {#ens-i-s5-thm-3 .statement tag=03P5}

$((x = y) \text{ và } (y = z)) \Rightarrow (x = z)$.

Ta thêm các giả thiết $x = y$, $y = z$ vào các tiên đề của $\mathscr{T}_0$. Theo S6, quan hệ $(x = y) \Rightarrow ((x = z) \Leftrightarrow (y = z))$ là đúng. Do đó

$$(x = z) \Leftrightarrow (y = z),$$

và do đó $x = z$, là đúng.

C44. *Cho $x$ là một chữ cái và cho $T$, $U$, $V\{x\}$ là các hạng trong $\mathscr{T}_0$. Khi đó quan hệ $(T = U) \Rightarrow (V\{T\} = V\{U\})$ là một định lý trong $\mathscr{T}_0$.*

Cho $y$ và $z$ là hai chữ phân biệt phân biệt với $x$ và với các chữ xuất hiện trong $T$, $U$, $V$. Thêm giả thiết $y = z$. Khi đó, theo S6,

$$((Y|z)(V\{y\} = V\{z\})) \Leftrightarrow (V\{y\} = V\{z\}),$$

nghĩa là $(V\{y\} = V\{y\}) \Leftrightarrow (V\{y\} = V\{z\})$, là đúng. Bây giờ, $V\{y\} = V\{y\}$ là đúng theo Định lý 1; do đó $V\{y\} = V\{z\}$ là đúng.

Từ tất cả những điều này suy ra rằng $(y = z) \Rightarrow (V\{y\} = V\{z\})$ là một định lý trong $\mathscr{T}_0$, ký hiệu là $A$. Nhưng $(T|y)(U|z)A$ chính xác là

$$(T = U) \Rightarrow (V\{T\} = V\{U\}).$$

¶ Một quan hệ có dạng $T = U$, trong đó $T$ và $U$ là các số hạng trong $\mathscr{T}$, được gọi là một *phương trình*; một *nghiệm* (trong $\mathscr{T}$) của quan hệ $T = U$, được xem như một phương trình theo một chữ cái $x$, do đó là (§2, no. 2) một số hạng $V$ trong $\mathscr{T}$ sao cho $T\{V\} = U\{V\}$ là một định lý trong $\mathscr{T}$.

¶ Cho $T$ và $U$ là hai thuật ngữ trong $\mathscr{T}$, và cho $x_1$, $x_2$, ..., $x_n$ là các chữ cái xuất hiện trong $T$ nhưng không trong $U$. Nếu quan hệ

$$(\exists x_1)\ldots(\exists x_n)(T = U)$$

là một định lý trong $\mathscr{T}$, ta nói rằng *U có thể được đặt dưới dạng* $T$ (trong $\mathscr{T}$). Cho $R$ là một quan hệ trong $\mathscr{T}$ và cho $y$ là một chữ cái. Cho $V$ là một nghiệm (trong $\mathscr{T}$) của $R$, được xem như một quan hệ theo $y$. Nếu mọi nghiệm (trong $\mathscr{T}$) của $R$, được xem như một quan hệ theo $y$, đều có thể được đặt dưới dạng $V$, thì $V$ được gọi là *nghiệm đầy đủ* (hay *nghiệm tổng quát*) của $R$ (trong $\mathscr{T}$).

### 3. CÁC QUAN HỆ PHIẾM HÀM

Cho $R$ là một dãy ký hiệu và $x$ là một chữ cái. Cho $y$ và $z$ là các chữ cái phân biệt, phân biệt với $x$ và không xuất hiện trong $R$. Cho $y'$, $z'$ là hai chữ cái khác có cùng các tính chất đó. Theo CS8, CS9 (§4, no. 1), CS2, CS5 (§1, no. 2), và CS6 (§3, no. 4), các dãy ký hiệu

$$(\forall y)(\forall z)(((y|x)R \text{ và } (z|x)R) \Rightarrow (y = z))$$

và

$$(\forall y')(\forall z')(((y'|x)R \text{ và } (z'|x)R) \Rightarrow (y' = z'))$$

là đồng nhất. Nếu $R$ là một quan hệ trong $\mathscr{T}$, phép lắp ghép được xác định như vậy là một quan hệ trong $\mathscr{T}$ được ký hiệu bởi "tồn tại nhiều nhất một $x$ sao cho $R$"; chữ $x$ không xuất hiện trong quan hệ này. Khi quan hệ này là một định lý trong $\mathscr{T}$, $R$ được gọi là *đơn trị* trong $X$ trong $\mathscr{T}$. Để chứng minh rằng $R$ là đơn trị trong lý thuyết $\mathscr{T}$, chỉ cần chứng minh $y = z$ trong lý thuyết thu được bằng cách thêm vào $\mathscr{T}$ các tiên đề $(y|x)R$ và $(z|x)R$, trong đó $y$ và $z$ là các chữ phân biệt và phân biệt với $x$, đồng thời không xuất hiện trong $R$ cũng như trong các tiên đề tường minh của $\mathscr{T}$.

C45. *Cho $R$ là một quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ không phải là hằng của $\mathscr{T}$. Nếu $R$ đơn trị theo $x$ trong $\mathscr{T}$, thì $R \Rightarrow (x = \tau_x(R))$ là một định lý trong $\mathscr{T}$. Ngược lại, nếu với một số số hạng $T$ trong $\mathscr{T}$ không chứa $x$, $R \Rightarrow (x = T)$ là một định lý trong $\mathscr{T}$, thì $R$ đơn trị theo $x$ trong $\mathscr{T}$.*

Giả sử $R$ đơn trị theo $x$ trong $\mathscr{T}$, ta hãy chứng minh rằng

$$R \Rightarrow (x = \tau_x(R))$$

là một định lý trong $\mathscr{T}$. Thêm giả thiết $R$. Khi đó $(\tau_x(R)|x)R$ là đúng theo S5, và do đó "$R$ và $(\tau_x(R)|x)R$" là đúng. Bây giờ, vì $R$ đơn trị theo $x$,

$$(R \text{ và } (\tau_x(R)|x)R) \Rightarrow (x = \tau_x(R))$$

là một định lý trong $\mathscr{T}$ theo C30 (§4, no. 3). Do đó $x = \tau_x(R)$ là đúng.

¶ Ngược lại, giả sử rằng $R \Rightarrow (x = T)$ là một định lý trong $\mathscr{T}$. Cho $y$, $z$ là các chữ cái phân biệt phân biệt với $x$ và không xuất hiện trong $R$ cũng như trong các tiên đề tường minh của $\mathscr{T}$. Vì $x$ không phải là một hằng của $\mathscr{T}$ và không xuất hiện trong $T$, các quan hệ

$$(y|x)R \Rightarrow (y = T), \qquad (z|x)R \Rightarrow (z = T)$$

là các định lý trong $\mathscr{T}$. Bổ sung các giả thuyết $(y|x)R$ và $(z|x)R$. Khi đó $y = T$ và $z = T$ là đúng, do đó $y = z$ là đúng.

¶ Cho $R$ là một quan hệ trong $\mathscr{T}$. Quan hệ

$$\text{“}(\exists x)R \text{ và tồn tại nhiều nhất một } x \text{ sao cho } R\text{”}$$

được ký hiệu bởi "tồn tại duy nhất một $x$ sao cho $R$". Nếu quan hệ này là một định lý trong $\mathscr{T}$, thì $R$ được gọi là một *quan hệ phiếm hàm theo* $x$ trong lý thuyết $\mathscr{T}$.

C46. *Cho $R$ là một quan hệ trong $\mathscr{T}$, và cho $x$ là một chữ cái không phải là một hằng của $\mathscr{T}$. Nếu $R$ là phiếm hàm theo $x$ trong $\mathscr{T}$, thì $R \Leftrightarrow (x = \tau_x(R))$ là một định lý trong $\mathscr{T}$. Ngược lại, nếu với một số hạng $T$ nào đó trong $\mathscr{T}$ không chứa $x$,*

$$R \Leftrightarrow (X = T)$$

*là một định lý trong $\mathscr{T}$, thì $R$ là phiếm hàm theo $x$ trong $\mathscr{T}$.*

Giả sử $R$ là phiếm hàm theo $x$ trong $\mathscr{T}$. Khi đó $R \Rightarrow (x = \tau_x(R))$ là một định lý trong $\mathscr{T}$ theo C45. Mặt khác, $(\exists x)R$ là một định lý trong $T$. Theo S6, quan hệ

$$(x = \tau_x(R)) \Rightarrow (R \Leftrightarrow (\exists x)R)$$

là một định lý trong $\mathscr{T}$. Nếu ta thêm giả thiết $x = \tau_x(R)$, thì suy ra rằng $R$ là đúng. Do đó $(x = \tau_x(R)) \Rightarrow R$ là một định lý trong $\mathscr{T}$.

¶ Ngược lại, nếu $R \Leftrightarrow (x = T)$ là một định lý trong $\mathscr{T}$, thì $R$ là đơn trị theo $x$ trong $\mathscr{T}$, theo C45. Hơn nữa, $(T|x)R \Leftrightarrow (T = T)$ là một định lý trong $\mathscr{T}$; do đó $(T|x)R$ và vì vậy $(\exists x)R$ là các định lý trong $\mathscr{T}$.

¶ Nếu một quan hệ $R$ là phiếm hàm theo $x$ trong T, thì $R$ tương đương với quan hệ $x = \tau_x(R)$, quan hệ này thường dễ xử lý hơn. Nói chung một ký hiệu viết tắt $\Sigma$ được đưa vào để biểu diễn số hạng $\tau_x(R)$. Một ký hiệu như vậy được gọi là một *ký hiệu phiếm hàm* trong $\mathscr{T}$.

Về mặt trực giác, $\Sigma$ biểu diễn đối tượng duy nhất có tính chất được xác định bởi $R$. \* Ví dụ, trong một lý thuyết mà "$y$ là một số thực $\geqslant 0$" là một định lý, quan hệ "$x$ là một số thực $\geqslant 0$ và $y = x^2$" là phiếm hàm theo $x$. Ký hiệu phiếm hàm tương ứng được lấy là $\sqrt{y}$ hoặc $y^{1/2}$. \*

C47. *Cho $x$ là một chữ không phải là một hằng của $\mathscr{T}$, và cho $R\{x\}$ và $S\{x\}$ là hai quan hệ trong $\mathscr{T}$. Nếu $R\{x\}$ là phiếm hàm theo $x$ trong $\mathscr{T}$, thì quan hệ $S\{\tau_x(R)\}$ là tương đương với $(\exists x)(R\{x\}$ và $S\{x\})$.*

Vì suy ra từ C46 và C43 rằng $(R\{x\}$ và $S\{x\})$ là tương đương với $(R\{x\}$ và $S\{\tau_x(R)\})$; vì $S\{\tau_x(R)\}$ không chứa $x$,

$$(\exists x)(R\{x\} \ \text{ và } \ S\{\tau_x(R)\})$$

tương đương với $(S\{\tau_x(R)\}$ và $(\exists x)R)$ theo C33 (§ 4, no. 3); và kết quả suy ra từ sự kiện rằng $(\exists x)R$ là đúng, bởi vì $R$ là phiếm hàm theo $x$.

### Bài tập {#ens-i-s5-exercises}

*Trong tất cả các Bài tập của* § 5, $\mathscr{T}$ *biểu thị một lý thuyết bình đẳng.*

Xem các [bài tập của § 5](exercises/s5/).
