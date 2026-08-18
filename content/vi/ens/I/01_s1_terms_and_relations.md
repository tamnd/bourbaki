---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 1
section_title: Terms and relations
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 15-23, 56
pdf_pages: 0022-0030, 0063-0063
extraction: ocr
subsections:
    - "no": 1
      title: SIGNS AND ASSEMBLIES
      page: 15
      pdf_page: 22
    - "no": 2
      title: CRITERIA OF SUBSTITUTION
      page: 18
      pdf_page: 25
    - "no": 3
      title: FORMATIVE CONSTRUCTIONS
      page: 19
      pdf_page: 26
    - "no": 4
      title: FORMATIVE CRITERIA
      page: 21
      pdf_page: 28
statements: 5
exercises: 6
content_sha256: 41997a5758c0b01e294df10ba787a999831dda28eff28cfac922faae4a4c4dee
translated_from: content/en/ens/I/01_s1_terms_and_relations.md
source_content_sha256: bbd7a5190da4bab5fb7ec796a94619a8dd8c0628947bd1a6aa35eabe2daa40a0
translation_model: gpt-5.4
translation_run: translate-vi-7032b096
glossary_version: 29
glossary_terms_sha256: 25122c96bfa9d8a032dfb8e55b05b20a93efc18edc9882a1c242315ba2be45a5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. THUẬT NGỮ VÀ QUAN HỆ

### 1. CÁC DẤU VÀ CÁC DÃY KÝ HIỆU

Các *dấu* của một lý thuyết toán học $\mathscr{T}$ [^1] là như sau :

(1) Các *dấu lôgic* [^2] : $\square$, $\tau$, $\vee$, $\neg$.
(2) Các *chữ cái*.

Bởi chữ cái, ta hiểu các chữ cái Latin viết hoa và viết thường, có hoặc không có dấu phụ. Như vậy $A$, $A'$, $A''$, $A'''$, ... là các chữ cái. Ở bất kỳ chỗ nào trong văn bản cũng có thể giới thiệu những chữ cái khác với những chữ cái đã xuất hiện trong các lập luận trước đó.

(3) Các *dấu riêng*, phụ thuộc vào lý thuyết đang xét.

Trong lý thuyết tập hợp, chúng ta sẽ chỉ dùng ba dấu riêng sau đây : $=$, $\in$, $\supset$.

Một *dãy ký hiệu* trong $\mathscr{T}$ là một dãy các dấu của $\mathscr{T}$ được viết liền nhau; một số dấu, ngoài các chữ cái ra, có thể được ghép thành từng cặp bằng những gạch ở phía trên dòng, gọi là các *liên kết*. \*Ví dụ, trong lý thuyết tập hợp, trong đó $\in$ là một dấu riêng,

$$\overline{\overline{\tau \vee \neg \in \square} A' \in \square} A''$$

là một dãy ký hiệu.\*

Việc chỉ dùng các dãy ký hiệu sẽ dẫn đến những khó khăn không thể vượt qua được, cả đối với người in lẫn đối với người đọc. Vì lý do đó, các văn bản hiện hành dùng những ký hiệu viết tắt (đặc biệt là những từ của ngôn ngữ thông thường) không thuộc toán học hình thức. Việc đưa vào những ký hiệu như thế là đối tượng của các *định nghĩa*. Việc dùng chúng *không phải là điều thiết yếu đối với lý thuyết*, và thường có thể dẫn đến những chỗ lẫn lộn mà chỉ một sự quen thuộc nhất định với môn học mới cho phép người đọc tránh được.

*Ví dụ*

#### Ví dụ 1 {#ens-i-s1-n1-exa-1 .statement tag=03P0}

Dãy ký hiệu $\vee 1$ được biểu diễn bởi $\Rightarrow$.

#### Ví dụ 2 {#ens-i-s1-n1-exa-2 .statement tag=03P1}

Các ký hiệu sau đây biểu diễn những dãy ký hiệu (mà lại còn là những dãy rất dài nữa):

“3 và 4”

$$\varnothing$$

$$\mathbf{N}$$

$$\mathbf{Z}$$

“đường thẳng thực”

“hàm $\Gamma$”

$$f\circ g$$

$$\pi=\sqrt{2}+\sqrt{3}$$

$$1\in 2$$

“Mọi vành có phép chia hữu hạn đều là một trường”

“Các điểm không của $\zeta(s)$ khác $-2$, $-4$, $-6$, ... nằm trên đường

$$R(s)=1/2$$.”

Nói chung, ký hiệu dùng để biểu diễn một dãy ký hiệu chứa tất cả các chữ cái xuất hiện trong dãy ký hiệu ấy. Tuy nhiên, nguyên lý này đôi khi có thể bị vi phạm mà không có nguy cơ gây lẫn lộn. *Chẳng hạn, “phần bù chỉnh của X” biểu diễn một dãy ký hiệu có chứa chữ cái X, nhưng cũng chứa chữ cái biểu diễn tập hợp các entourage của cấu trúc đều trên X. Mặt khác,

$$\int_0^1 f(x)\,dx$$

biểu diễn một dãy ký hiệu trong đó chữ cái $x$ (và chữ cái $d$) không xuất hiện; và các dãy ký hiệu được biểu diễn bởi $\mathbf{N}$, $\mathbf{Z}$, “hàm $\Gamma$” không chứa chữ cái nào.*

Một *lý thuyết toán học* (hay đơn giản là một *lý thuyết*) chứa những quy tắc cho phép ta khẳng định rằng một số dãy ký hiệu nào đó là các *hạng tử hoặc quan hệ* của lý thuyết, và những quy tắc khác cho phép ta khẳng định rằng một số dãy ký hiệu nào đó là các *định lý* của lý thuyết.

Mô tả các quy tắc ấy, sẽ xuất hiện trong chương này, *không thuộc toán học hình thức*; các quy tắc ấy liên quan đến những dãy ký hiệu ít nhiều chưa xác định, chẳng hạn những chữ cái chưa xác định. Để

đơn giản hóa cách trình bày, tiện lợi là ký hiệu những dãy ký hiệu như vậy bằng những ký hiệu đỡ cồng kềnh hơn. Đặc biệt, chúng tôi sẽ dùng các tổ hợp ký hiệu (của một lý thuyết toán học), các chữ cái in nghiêng đậm (có hoặc không có chỉ số hoặc dấu), và những ký hiệu riêng biệt, mà sẽ cho một vài ví dụ. *Vì mục đích của chúng tôi chỉ là tránh những lối diễn đạt vòng vo* (x. chú ý (*), § 3, no. 1, p. 28), chúng tôi sẽ không phát biểu những quy tắc tổng quát ngặt về cách dùng các ký hiệu ấy; người đọc sẽ có thể, không khó khăn gì, phục nguyên dãy ký hiệu được nói đến trong từng trường hợp riêng biệt. Do lạm dụng ngôn ngữ, chúng tôi sẽ thường nói rằng các ký hiệu *là* các dãy ký hiệu, thay vì nói rằng chúng *biểu thị* các dãy ký hiệu: vì vậy, trong các phát biểu của những quy tắc sau đây, những cách nói như “dãy ký hiệu $A$” hoặc “chữ cái $x$” phải được thay bằng “dãy ký hiệu được biểu thị bởi $A$” hoặc “chữ cái được biểu thị bởi $x$”.

Cho $A$ và $B$ là các dãy ký hiệu. Ta sẽ ký hiệu bởi $AB$ dãy ký hiệu thu được bằng cách viết dãy ký hiệu $B$ ở bên phải dãy ký hiệu $A$. Ta sẽ ký hiệu bởi $\vee A\neg B$ dãy ký hiệu thu được bằng cách viết, từ trái sang phải, dấu $\vee$, dãy ký hiệu $A$, dấu $\neg$, dãy ký hiệu $B$. Và cứ tiếp tục như thế.

Cho $A$ là một biểu thức và $x$ là một chữ. Ta sẽ ký hiệu bởi $\tau_x(A)$ biểu thức được xây dựng như sau : lập biểu thức $\tau A$, nối mỗi lần xuất hiện của $x$ trong $A$ với chữ $\tau$ viết ở bên trái của $A$, rồi thay thế $x$ ở mọi chỗ nó xuất hiện bằng dấu $\square$. Vậy biểu thức được ký hiệu bởi $\tau_x(A)$ *không chứa* $x$.

#### Ví dụ {#ens-i-s1-n1-exa-3 .statement tag=03RY}

Ký hiệu $\tau_x(\in xy)$ biểu diễn biểu thức

$$
\tau\in\square y.
$$

Cho $A$ và $B$ là các dãy ký hiệu và cho $x$ là một chữ cái. Dãy ký hiệu thu được bằng cách thay thế $x$, ở mọi chỗ nó xuất hiện trong $A$, bởi dãy ký hiệu $B$ được ký hiệu bởi $(B\mathbin{|}x)\,A$ (đọc là: $B$ thay thế $x$ trong $A$). Nếu $x$ không xuất hiện trong $A$, thì $(B\mathbin{|}x)\,A$ trùng với $A$; đặc biệt là,

$$
(B\mathbin{|}x)\,\tau_x(A)
$$

đồng nhất với $\tau_x(A)$.

#### Ví dụ {#ens-i-s1-n1-exa-4 .statement tag=03TO}

Nếu ta thay thế $x$ bằng $\square$ ở mọi chỗ $x$ xuất hiện trong xếp ghép $\vee\in xy=xx$, thì ta thu được xếp ghép $\vee\in\square y=\square\square$.

Nếu $A$ là một assembly và nếu ta đặc biệt quan tâm đến một chữ cái $x$, hoặc đến hai chữ cái phân biệt $x$ và $y$ (có thể xuất hiện hoặc không xuất hiện trong $A$), thì ta sẽ thường viết $A\{x\}$ hoặc $A\{x,y\}$. Trong trường hợp này ta viết $A\{B\}$ thay cho $(B\mathbin{|}x)\,A$. Ta ký hiệu bởi $A\{B,C\}$ assembly thu được bằng cách *đồng thời* thay thế $x$ bởi $B$ và $y$ bởi $C$ ở mọi chỗ chúng xuất hiện trong $A$ (chú ý rằng $x$ và $y$ có thể xuất hiện trong $B$ và trong $C$); nếu $x'$ và $y'$ là những chữ cái phân biệt, khác $x$ và $y$, không xuất hiện trong cả $A$, $B$ lẫn $C$, thì $A\{B,C\}$ cũng chính là $(B\mathbin{|}x')(C\mathbin{|}y')(x'\mathbin{|}x)(y'\mathbin{|}y)A$.

#### Nhận xét {#ens-i-s1-n1-rem-1 .statement tag=03P2}

Khi một ký hiệu viết tắt $\Sigma$ được đưa vào, bằng một định nghĩa, để biểu thị một biểu thức nào đó, thì người ta đặt ra quy ước (thường là ngầm) rằng biểu thức thu được bằng cách thay một biểu thức $B$ cho chữ $x$ trong biểu thức ban đầu sẽ được biểu thị bởi ký hiệu nhận được bằng cách thay chữ $x$ trong $\Sigma$ bởi biểu thức $B$ (hoặc, thường hơn, bởi một ký hiệu viết tắt biểu thị biểu thức $B$).

¶ *Ví dụ, sau khi đã định nghĩa biểu thức nào được biểu thị bởi ký hiệu $E\otimes F$, trong đó $E$ và $F$ là các chữ — một biểu thức mà, nhân đây nói thêm, còn chứa những chữ khác ngoài $E$ và $F$ — thì có thể dùng ký hiệu $Z\otimes F$ mà không cần giải thích thêm.*

¶ Quy tắc này có thể dẫn đến những sự lẫn lộn, được tránh bằng cách dùng nhiều cách trình bày in ấn khác nhau; cách chung nhất là thay $x$ bởi $(B)$ thay cho $B$.

¶ *Ví dụ, $M\cap N$ ký hiệu một dãy ký hiệu chứa chữ cái $N$. Nếu ta thế cho $N$ dãy ký hiệu được biểu diễn bởi $P\cup Q$, ta thu được một dãy ký hiệu được ký hiệu bởi $M\cap(P\cup Q)$.*

### 2. CÁC TIÊU CHUẨN THẾ

Toán học hình thức chỉ chứa các dãy ký hiệu được viết ra một cách tường minh. Tuy nhiên, ngay cả khi dùng các ký hiệu viết tắt, việc phát triển toán học một cách nghiêm ngặt theo nguyên lý này cũng sẽ dẫn đến những chuỗi lập luận cực kỳ dài. Vì lý do này, chúng tôi sẽ thiết lập các tiêu chuẩn liên quan đến các dãy ký hiệu bất định; mỗi tiêu chuẩn trong số đó sẽ mô tả một lần thay cho tất cả kết quả cuối cùng của một dãy xác định các phép thao tác trên các dãy ký hiệu ấy. Do đó các tiêu chuẩn này không phải là không thể thiếu đối với lý thuyết; sự biện minh của chúng thuộc về siêu toán học.

Sự phát triển của siêu toán học chính nó, trên thực tế, đòi hỏi việc dùng các ký hiệu viết tắt, một số trong đó đã được chỉ ra. Phần lớn các ký hiệu ấy cũng được dùng trong toán học.

Chúng tôi sẽ dùng các tiêu chuẩn sau đây, gọi là *các tiêu chuẩn thế* :

CS1. Cho $A$ và $B$ là các dãy ký hiệu và $x$ và $x'$ là các chữ cái. Nếu $x'$ không xuất hiện trong $A$, thì $(B|x)A$ đồng nhất với $(B|x')(x'|x)A$.

CS2. Cho $A$, $B$ và $C$ là các dãy ký hiệu và cho $x$ và $y$ là các chữ cái phân biệt [^3]. Nếu $y$ không xuất hiện trong $B$, thì $(B|x)(C|y)A$ đồng nhất với

$$(C'|y)(B|x)A,$$

trong đó $C'$ là dãy ký hiệu $(B|x)C$.

CS3. *Cho $A$ là một assemblage và $x$ và $x'$ là các chữ cái. Nếu $x'$ không xuất hiện trong $A$, thì $\tau_x(A)$ đồng nhất với $\tau_{x'}(A')$, trong đó $A'$ là assemblage $(x'|x)\,A$.*

CS4. *Cho $A$ và $B$ là các dãy ký hiệu và $x$ và $y$ là các chữ cái phân biệt. Nếu $x$ không xuất hiện trong $B$, thì $(B|y)\tau_xA$ đồng nhất với $\tau_x(A')$, trong đó $A'$ là dãy ký hiệu $(B|y)\,A$.*

CS5. *Cho $A$, $B$, $C$ là các dãy ký hiệu và $x$ là một chữ cái. Các dãy ký hiệu $(C|x)(\neg A)$, $(C|x)(\vee AB)$, $(C|x)(\Rightarrow AB)$, $(C|x)(sAB)$ (trong đó $s$ là một ký hiệu xác định) lần lượt đồng nhất với $\neg A'$, $\vee A'B'$, $\Rightarrow A'B'$, $sA'B'$, trong đó $A'$, $B'$ lần lượt là $(C|x)\,A$, $(C|x)\,B$.*

Để làm ví dụ, ta hãy chỉ ra nguyên lý của việc kiểm tra CS2. Hãy so sánh phép toán đưa ta từ $A$ đến $(B|x)(C|y)\,A$ với phép toán đưa ta từ $A$ đến $(C|y)(B|x)\,A$. Trong mỗi phép toán, không ký hiệu nào xuất hiện trong $A$ và phân biệt với $x$ và $y$ bị thay đổi. Ở mọi chỗ mà $x$ xuất hiện trong $A$, ta phải thay thế $B$ cho $x$ trong phép toán thứ nhất cũng như trong phép toán thứ hai; điều này hiển nhiên đối với phép toán thứ nhất, còn đối với phép toán thứ hai thì nó suy ra từ việc $y$ không xuất hiện trong $B$. Sau cùng, ở mọi chỗ mà $y$ xuất hiện trong $A$, phép toán thứ nhất gồm việc thay thế $C$ cho $y$, rồi thay thế $B$ cho $x$ ở mọi chỗ mà $x$ xuất hiện trong $C$; nhưng hiển nhiên điều này cũng tương đương với việc thay thế cho $y$, ở mọi chỗ nó xuất hiện trong $A$, tổ hợp $(B|x)\,C$.

### 3. CÁC PHÉP DỰNG KIẾN TẠO

Một số ký hiệu riêng của một lý thuyết được gọi là *quan hệ*, và các ký hiệu khác được gọi là *bản thể*. Với mỗi ký hiệu riêng liên kết một số tự nhiên gọi là *trọng số* của nó (trên thực tế hầu như luôn luôn là số 2).

¶ Một dãy ký hiệu được gọi là thuộc *loài thứ nhất* nếu nó bắt đầu bằng một $\tau$, hoặc bằng một ký hiệu bản thể, hoặc nếu nó chỉ gồm một chữ cái duy nhất; nếu không thì nó thuộc *loài thứ hai*.

¶ Một *phép dựng kiến tạo* trong một lý thuyết $\mathscr{T}$ là một dãy các dãy ký hiệu có tính chất sau đây : đối với mỗi dãy ký hiệu $A$ của dãy đó, một trong các điều kiện sau được thỏa mãn :

(a) $A$ là một chữ cái.

(b) Trong dãy có một dãy ký hiệu $B$ thuộc loài thứ hai, đứng trước $A$, sao cho $A$ là $\neg B$.

(c) Có hai dãy ký hiệu $B$ và $C$ thuộc loài thứ hai (phân biệt hoặc không), đứng trước $A$, sao cho $A$ là $\vee BC$.

(d) Có một dãy ký hiệu $B$ thuộc loài thứ hai, đi trước $A$, và một chữ cái $x$ sao cho $A$ là $\tau_x(B)$.

(e) Có một ký hiệu xác định $s$ có trọng số $n$ [^4] trong $\mathscr{T}$, và $n$ dãy ký hiệu $A_1,A_2,\ldots,A_n$ thuộc loài thứ nhất, đi trước $A$, sao cho $A$ là $sA_1A_2\ldots A_n$.

¶ Các dãy ký hiệu thuộc loài thứ nhất (tương ứng, thuộc loài thứ hai) xuất hiện trong các phép kiến tạo của $\mathscr{T}$ được gọi là các hạng thức (tương ứng, các quan hệ) trong $\mathscr{T}$.

*Ví dụ.* *Trong lý thuyết tập hợp, trong đó $\in$ là một dấu quan hệ có trọng số 2, dãy các dãy ký hiệu sau đây là một phép dựng kiến tạo:*

$$
\begin{array}{c}
A\\
A'\\
A''\\
\in AA'\\
\in AA''\\
\neg\in AA'\\
\vee\neg\in AA'\in AA''
\\[2pt]
\tau\vee\neg\in\square A'\in\square A''
\end{array}
$$

Do đó dãy ký hiệu được cho làm ví dụ trong no. 1 là một số hạng trong lý thuyết tập hợp.*

*Chú ý.* Theo trực giác, các hạng là các dãy ký hiệu biểu diễn các đối tượng, còn các quan hệ là các dãy ký hiệu biểu diễn các mệnh đề có thể phát biểu về các đối tượng đó. Điều kiện (a) có nghĩa là các chữ cái biểu diễn các đối tượng. Điều kiện (b) có nghĩa là nếu $B$ là một mệnh đề, thì $\neg B$, gọi là phủ định của $B$, là một mệnh đề (được đọc là: không $B$). Điều kiện (c) có nghĩa là nếu $B$ và $C$ là các mệnh đề, thì $\vee BC$, gọi là tuyển của $B$ và $C$, là một mệnh đề (được đọc là: hoặc $B$ hoặc $C$); do đó $\neg\to BC$ là một mệnh đề (nói bằng lời: “hoặc không $B$, hoặc $C$”, hoặc “$B$ kéo theo $C$”). Điều kiện (d) có nghĩa là nếu $B$ là một mệnh đề và $x$ là một chữ cái, thì $\tau_x(B)$ là một đối tượng. Hãy coi mệnh đề $B$ như biểu thị một tính chất của đối tượng $X$; khi đó, nếu tồn tại một đối tượng có tính chất đang xét, thì $\tau_x(B)$ biểu diễn một đối tượng phân biệt có tính chất ấy; nếu không, $\tau_x(B)$ biểu diễn một đối tượng mà không thể nói gì về nó. Cuối cùng, điều kiện (e) có nghĩa là nếu $A_1,A_2,\ldots,A_n$ là các đối tượng, và nếu $s$ là một dấu quan hệ (tương ứng, một dấu thực thể) có trọng số $n$, thì $sA_1A_2\ldots A_n$ là một mệnh đề về các đối tượng $A_1,\ldots,A_n$ (tương ứng, một đối tượng phụ thuộc vào $A_1,\ldots,A_n$).

*Ví dụ.* Các ký hiệu $\varnothing$, $\mathbf{N}$, “dòng thực”, “hàm $\Gamma$”, $f\circ g$ biểu diễn các số hạng. Các ký hiệu $\pi=\sqrt{2}+\sqrt{3}$, $1\in2$, “mọi vành chia hữu hạn

đều là một trường”, “các không điểm của $\zeta(s)$ ngoài $-2$, $-4$, $-6$, ... nằm trên dòng $\mathfrak{R}(s)=1/2$” biểu diễn các quan hệ. Ký hiệu “3 và 4” không biểu diễn số hạng nào cũng không biểu diễn quan hệ nào.

Ký hiệu ban đầu của một quan hệ là $\vee$, $\neg$, hoặc một dấu quan hệ. Ký hiệu ban đầu của một số hạng hoặc là $\tau$ hoặc là một dấu thực thể, nếu số hạng đó không chỉ gồm một chữ cái duy nhất. Mệnh đề sau cùng này suy ra từ việc một số hạng là một dãy ký hiệu thuộc loài thứ nhất. Nếu $A$ là một quan hệ, thì $A$ xuất hiện trong một phép dựng kiến tạo, không phải là một chữ cái, và không bắt đầu bằng $\tau$, nên có thể có ba trường hợp : (1) trước $A$ là một dãy ký hiệu $B$ sao cho $A$ là $\neg B$; (2) trước $A$ là hai dãy ký hiệu $B$ và $C$ sao cho $A$ là $\vee BC$; (3) trước $A$ là các dãy ký hiệu $A_1$, $A_2$, ... $A_n$ sao cho $A$ là $sA_1A_2 ... A_n$, trong đó $s$ là một dấu quan hệ.

### 4. CÁC TIÊU CHUẨN KIẾN TẠO

CF1. Nếu $A$ và $B$ là các quan hệ trong một lý thuyết $\mathscr{T}$, thì $\vee AB$ là một quan hệ trong $\mathscr{T}$.

Xét hai phép dựng kiến tạo (trong $\mathscr{T}$), một phép chứa $A$ và phép kia chứa $B$. Xét dãy các dãy ký hiệu thu được bằng cách viết trước hết các dãy ký hiệu của phép dựng thứ nhất, rồi các dãy ký hiệu của phép dựng thứ hai, và cuối cùng là $\vee AB$. Vì $A$ và $B$ thuộc loài thứ hai, nên ngay lập tức kiểm tra được rằng dãy này là một phép dựng kiến tạo của $\mathscr{T}$. Dãy ký hiệu $\vee AB$ thuộc loài thứ hai, do đó nó là một quan hệ trong $\mathscr{T}$.

Ba tiêu chuẩn sau đây được thiết lập tương tự :

CF2. Nếu $A$ là một quan hệ trong một lý thuyết $\mathscr{T}$, thì $\neg A$ là một quan hệ trong $\mathscr{T}$.

CF3. Nếu $A$ là một quan hệ trong một lý thuyết $\mathscr{T}$, và nếu $x$ là một chữ, thì $\tau_x(A)$ là một số hạng trong $\mathscr{T}$.

CF4. Nếu $A_1$, $A_2$, ..., $A_n$ là các số hạng trong lý thuyết $\mathscr{T}$, và nếu $s$ là một dấu quan hệ (tương ứng, dấu hàm) có trọng số $n$ trong $\mathscr{T}$, thì $sA_1A_2...A_n$ là một quan hệ (tương ứng, một số hạng) trong $\mathscr{T}$.

Các tiêu chuẩn này ngay lập tức kéo theo điều sau :

CF5. Nếu $A$ và $B$ là các quan hệ trong lý thuyết $\mathscr{T}$, thì $\Longrightarrow AB$ là một quan hệ trong $\mathscr{T}$.

CF6. Cho $A_1$, $A_2$, ..., $A_n$ là một phép dựng kiến tạo trong một lý thuyết $\mathscr{T}$, và cho $x$ và $y$ là các chữ cái. Giả sử rằng $y$ không xuất hiện trong bất kỳ $A_i$ nào. Khi đó $(y|x) A_1$, $(y|x) A_2$, ..., $(y|x) A_n$ là một phép dựng kiến tạo trong $\mathscr{T}$.

Để chứng minh CF6, đặt $A_i'$ là tổ hợp $(y|x)A_i$. Nếu $A_i$ là một chữ cái, thì $A_i'$ là một chữ cái. Nếu $A_i$ có dạng $\neg A_j$, trong đó $A_j$ là một tổ hợp của loài thứ hai đứng trước $A_i$ trong phép dựng, thì $A_i'$ đồng nhất với $\neg A_j'$ theo CS5, và $A_j'$ là một tổ hợp của loài thứ hai. Lập luận là đồng dạng nếu $A_i$ có dạng $\vee A_jA_k$ hoặc $sA_{j_1}A_{j_2}\ldots A_{j_m}$, trong đó $s$ là một dấu riêng biệt của $\mathscr{T}$. Nếu cuối cùng $A_i$ có dạng $\tau_z(A_j)$, trong đó $A_j$ là một tổ hợp của loài thứ hai đứng trước $A_i$ trong phép dựng, thì có nhiều trường hợp phải xét:

(a) $z$ là một chữ cái phân biệt với $x$ và $y$. Khi đó $A_i'$ đồng nhất với $\tau_z(A_j')$ theo CS4, và $A_j'$ là một tập hợp thuộc loài thứ hai.

(b) $z$ đồng nhất với $x$. Khi đó $A_i$ không chứa $x$, do đó $A_i'$ đồng nhất với $A_i$, nghĩa là với $\tau_x(A_j)$; vì $y$ không xuất hiện trong $A_j$, nên $\tau_x(A_j)$ đồng nhất với $\tau_y(A_j)$ theo CS3.

(c) $z$ đồng nhất với $y$. Khi đó $A_i$ là tổ hợp $\tau A_j$, vì $y$ không xuất hiện trong $A_j$; do đó $A_i'$ là tổ hợp $\tau A_j'$, tức là $\tau_u(A_j')$, trong đó $u$ là một chữ cái không xuất hiện trong $A_j'$.

CF7. *Cho $A$ là một quan hệ (tương ứng, một số hạng) trong một lý thuyết $\mathscr{T}$, và $x$ và $y$ là các chữ cái. Khi đó $(y|x)A$ là một quan hệ (tương ứng, một số hạng) trong $\mathscr{T}$.*

Cho $A_1,A_2,\ldots,A_n$ là một phép dựng kiến tạo trong đó $A$ xuất hiện. Ta sẽ chỉ ra từng bước rằng, nếu $A_i$ là một quan hệ (tương ứng, một số hạng) thì $(y|x)A_i$, mà ta sẽ ký hiệu là $A_i'$, cũng là một quan hệ (tương ứng, một số hạng). Giả sử rằng điều này đã được thiết lập cho $A_1,A_2,\ldots,A_{i-1}$; ta hãy chứng minh nó đối với $A_i$. Nếu $A_i$ là một chữ cái, thì $A_i'$ là một chữ cái. Nếu trong phép dựng, trước $A_i$ có một quan hệ $A_j$ sao cho $A_i$ là $\neg A_j$, thì $A_i'$ trùng với $\neg A_j'$ theo CS5, và $\neg A_j'$ là một quan hệ theo CF2. Lập luận là tương tự nếu trước $A_i$ có các quan hệ $A_j,A_k$ sao cho $A_i$ là $\vee A_jA_k$, hoặc nếu trước $A_i$ có các số hạng $A_{j_1},\ldots,A_{j_m}$ sao cho $A_i$ là $sA_{j_1}\cdots A_{j_m}$, trong đó $s$ là một ký hiệu riêng của $\mathscr{T}$ có trọng số $m$. Cuối cùng, nếu trước $A_i$ có một quan hệ $A_j$ sao cho $A_i$ là $\tau_z(A_j)$, thì có nhiều trường hợp phải xét:

(a) $z$ phân biệt với cả $x$ lẫn $y$. Khi đó $A_i'$ đồng nhất với $\tau_z(A_j')$ theo CS4, và ta đã biết rằng $A_j'$ là một quan hệ; suy ra $A_i$ là một số hạng, theo CF3.

(b) $z$ đồng nhất với $x$. Khi đó $A_i$ không chứa $x$, do đó $A_i'$ đồng nhất với $A_i$, và do đó là một số hạng.

(c) $z$ đồng nhất với $y$. Khi đó, lấy $u$ là một chữ cái phân biệt với cả $x$ lẫn $y$, không xuất hiện trong $A_1,A_2,\ldots,A_j$. Theo CF6, dãy các dãy ký hiệu $(u|y)A_1,\ldots,(u|y)A_j$, mà chúng tôi sẽ ký hiệu là $A_1'',\ldots,A_j''$, tạo thành một phép dựng kiến tạo trong $\mathscr{T}$. Vì $y$ không còn xuất hiện trong phép dựng mới này, $(y|x)A_1'',\ldots,(y|x)A_j''$ là một phép dựng kiến tạo theo CF6, nên $(y|x)A_j''$ là một quan hệ trong $\mathscr{T}$; do đó $\tau_u((y|x)A_j'')$

là một số hạng của $\mathscr{T}$. Nhưng số hạng này đồng nhất với $(y|x)\tau_u(A_j'')$ theo CS4, do đó với $(y|x)\tau_y(A_j)$ theo CS3, nên đồng nhất với $A_i$.

CF8. Cho $A$ là một quan hệ (tương ứng, một số hạng) trong một lý thuyết $\mathscr{T}$, $x$ là một chữ cái và $T$ là một số hạng trong $\mathscr{T}$. Khi đó $(T|x)A$ là một quan hệ (tương ứng, một số hạng) trong $\mathscr{T}$.

Cho $A_1, A_2, \ldots, A_n$ là một phép dựng kiến tạo trong đó $A$ xuất hiện. Cho $x_1, x_2, \ldots, x_p$ là các chữ cái phân biệt xuất hiện trong $T$. Hãy gắn với mỗi chữ cái $x_i$ một chữ cái $x_i'$, phân biệt với mỗi chữ cái trong các chữ cái $x_1, \ldots, x_p$ và các chữ cái xuất hiện trong $A_1, \ldots, A_n$, sao cho các chữ cái $x_1', \ldots, x_p'$ đều phân biệt. Dãy

$$
(x_1'|x_1)(x_2'|x_2)\ldots(x_p'|x_p)T
$$

là một số hạng $T'$ theo CF7, và $(T|x)A$ đồng nhất với

$$
(x_1|x_1')(x_2|x_2')\ldots(x_p|x_p')(T'|x)A
$$

bằng cách áp dụng CS1. Vì vậy chỉ cần chỉ ra rằng $(T'|x)\,A$ là một quan hệ (tương ứng, một số hạng); nói cách khác, từ nay ta có thể giả sử rằng các chữ cái xuất hiện trong $T$ không xuất hiện trong $A_1, \ldots, A_n$.

¶ Chúng ta sẽ chỉ ra từng bước rằng, nếu $A_t$ là một quan hệ (tương ứng, một số hạng), thì $(T|x)\,A_t$, mà ta sẽ ký hiệu là $A_t'$, là một quan hệ (tương ứng, một số hạng). Giả sử điểm này đã được thiết lập đối với $A_1,A_2,\ldots,A_{i-1}$, và hãy chứng minh nó đối với $A_i$. Nếu $A_i$ là một chữ cái, thì $A_i'$ hoặc là chính chữ cái đó hoặc là $T$, và do đó là một số hạng. Nếu $A_i$ có dạng $\neg A_j$, trong đó $A_j$ là một quan hệ đứng trước $A_i$ trong phép dựng, thì $A_i$ đồng nhất với $\neg A_j'$ theo CS5, và ta đã biết rằng $A_j'$ là một quan hệ, nên $A_i'$ là một quan hệ theo CF2. Chứng minh là tương tự nếu $A_i$ có dạng $\vee A_jA_k$, hoặc $sA_{j_1}\ldots A_{j_m}$. Sau cùng, nếu $A_i$ có dạng $\tau_z(A_j)$, trong đó $A_j$ là một quan hệ đứng trước $A_i$ trong phép dựng, thì có nhiều trường hợp khác nhau cần được xét:

(a) $z$ phân biệt với $x$ và với các chữ xuất hiện trong $T$. Khi đó $A_i'$ đồng nhất với $\tau_z(A_j')$ theo CS4, và ta đã biết rằng $A_j'$ là một quan hệ; vì thế $A_i'$ là một số hạng theo CF3.

(b) $z$ đồng nhất với $x$. Khi đó $A_i$ không chứa $x$, suy ra $A_i'$ đồng nhất với $A_i$ và do đó là một số hạng.

(c) $z$ xuất hiện trong $T$. Khi đó $z$ không xuất hiện trong $A_j$, do đó $A_i'$ đồng nhất với $\tau A_j'$; vì thế $A_i'$ đồng nhất với $\tau A_j'$. Bây giờ, ta đã biết rằng $A_j'$ là một quan hệ, và $\tau A_j'$ đồng nhất với $\tau_u(A_j)$, trong đó $u$ là một chữ cái không xuất hiện trong $A_j$; theo CF3 suy ra $A_i'$ là một số hạng.

Một cách trực quan, nếu $A$ là một quan hệ trong $\mathscr{T}$, mà ta có thể xem như biểu thị một tính chất của một đối tượng $x$, thì mệnh đề $(B|x)\,A$ có nghĩa là đối tượng $B$ có tính chất này. Nếu $A$ là một số hạng trong $\mathscr{T}$, nó biểu diễn một đối tượng phụ thuộc theo một cách nào đó vào đối tượng được ký hiệu bởi $x$; số hạng $(B|x)\,A$ biểu diễn đối tượng mà $A$ trở thành khi ta lấy $x$ là đối tượng $B$.

### Bài tập {#ens-i-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).

[^1]: Ý nghĩa của biểu thức này sẽ trở nên rõ ràng khi chương tiến triển.
[^2]: Về ý nghĩa trực giác của các ký hiệu này, xem no. 3, Nhận xét.
[^3]: Phù hợp với điều đã nói ở no. 1, cụm từ “$x$ và $y$ là những chữ cái phân biệt” là một sự lạm dụng ngôn ngữ: nó có nghĩa là $x$ và $y$ biểu thị những chữ cái phân biệt trong các dãy ký hiệu đang xét.
[^4]: Như đã nói ở trên, đối với sự phát triển của các lý thuyết toán học ngày nay, có thể giới hạn sự xem xét của ta vào các ký hiệu riêng biệt có trọng số 2, và do đó tránh dùng cụm từ “số tự nhiên $n$” trong định nghĩa của một phép dựng kiến tạo.
