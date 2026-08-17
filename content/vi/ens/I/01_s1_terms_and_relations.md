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
content_sha256: 9176862b6e452e6b05eb4ed3c1c2e7b2babcf5b241c0b606d89e566871a571e8
translated_from: content/en/ens/I/01_s1_terms_and_relations.md
source_content_sha256: bb554ed20fc7b3ab48f1b03434cd7587a6cfd49400a7649f457fd3f4a1a8215b
translation_model: laguna-s-2.1-free, hy3-free, gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-66ad11cf
glossary_version: 27
glossary_terms_sha256: 25122c96bfa9d8a032dfb8e55b05b20a93efc18edc9882a1c242315ba2be45a5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. THUẬT NGỮ VÀ QUAN HỆ

### 1. DẤU VÀ CÁC DÃY KÝ HIỆU

Các *dấu* của một lý thuyết toán học $\mathscr{T}$ (*)[^1] là như sau :

(1) Các *dấu lôgic* (†)[^2] : $\square$, $\tau$, $\vee$, $\neg$.
(2) Các *chữ cái*.

Bằng các chữ cái chúng tôi muốn các chữ cái La Tinh viết hoa và thường, có hoặc không dấu phụ. Vì vậy $A$, $A'$, $A''$, $A'''$, ... là các chữ cái. Ở bất kỳ nơi nào trong văn bản cũng có thể giới thiệu các chữ cái khác ngoài những chữ cái đã xuất hiện trong các lập luận trước đó.

(3) Các *dấu cụ thể*, phụ thuộc vào lý thuyết đang được xét đến.

Trong lý thuyết tập hợp chúng tôi chỉ sử dụng ba dấu cụ thể sau: $=$, $\in$, $\supset$.

Một *dãy ký hiệu* trong $\mathscr{T}$ là một dãy liên tiếp các dấu của $\mathscr{T}$ được viết cạnh nhau; một số dấu, ngoại trừ các chữ cái, có thể được nối thành các cặp bằng các thanh ngang phía trên, gọi là *liên kết*. \*Ví dụ, trong Lý thuyết Tập hợp, trong đó $\in$ là một dấu cụ thể,

$$\overline{\overline{\tau \vee \neg \in \square} A' \in \square} A''$$

là một dãy ký hiệu.*

Chỉ sử dụng các dãy ký hiệu sẽ dẫn đến những khó khăn không thể vượt qua đối với cả nhà xuất bản và người đọc. Vì lý do này, các văn bản hiện tại sử dụng các ký tự viết tắt (đặc biệt là các từ của ngôn ngữ thường ngày) mà không thuộc toán học hình thức. Việc giới thiệu các ký tự như vậy là mục đích của *Định nghĩa*. Sử dụng chúng *không thiết yếu cho lý thuyết*, và thường xuyên dẫn đến nhầm lẫn mà chỉ người đọc có sự quen thuộc nhất định với môn học mới có thể tránh được.

*Ví dụ*

#### Ví dụ 1 {#ens-i-s1-n1-exa-1 .statement tag=03P0}

Dãy ký hiệu $\vee 1$ được biểu diễn bởi $\Rightarrow$.

#### Ví dụ 2 {#ens-i-s1-n1-exa-2 .statement tag=03P1}

Các ký tự sau đây biểu diễn các dãy ký hiệu (và rất dài thực sự) :

“3 và 4”

$$\varnothing$$

$$\mathbf{N}$$

$$\mathbf{Z}$$

“đường thực”

“hàm $\Gamma$”

$$f\circ g$$

$$\pi=\sqrt{2}+\sqrt{3}$$

$$1\in 2$$

“Mọi vành chia hữu hạn là trường”

“Các nghiệm của $\zeta(s)$ ngoại trừ $-2$, $-4$, $-6$, ... nằm trên dòng

$$R(s)=1/2$$.”

Nói chung, ký tự được sử dụng để biểu diễn một dãy ký hiệu chứa tất cả các chữ cái xuất hiện trong dãy ký hiệu đó. Tuy nhiên, nguyên tắc này đôi khi có thể bị vi phạm mà không gây ra rủi ro nhầm lẫn. Ví dụ, “sự hoàn thiện của X” biểu diễn một dãy ký hiệu chứa chữ cái X, nhưng cũng chứa chữ cái biểu diễn tập hợp các entourage của cấu trúc đồng nhất của X. Mặt khác,

$$\int_0^1 f(x)\,dx$$

biểu diễn một dãy ký hiệu mà trong đó chữ cái $x$ (và chữ cái $d$) không xuất hiện; và các dãy ký hiệu được biểu diễn bởi $\mathbf{N}$, $\mathbf{Z}$, “hàm $\Gamma$” không chứa bất kỳ chữ cái nào.*

Một *lý thuyết toán học* (hoặc đơn giản một *lý thuyết*) chứa các quy tắc cho phép chúng ta khẳng định rằng một số dãy ký hiệu nhất định là *các số hạng hoặc quan hệ* của lý thuyết, và các quy tắc khác cho phép chúng ta khẳng định rằng một số dãy ký hiệu là *các định lý* của lý thuyết.

Mô tả của các quy tắc này, sẽ xuất hiện trong chương này, *không thuộc về toán học hình thức*; các quy tắc liên quan đến các dãy ký hiệu hơn hoặc kém không xác định, ví dụ các chữ cái không xác định. Để

đơn giản hóa việc trình bày, thì thuận tiện khi ký hiệu các dãy ký hiệu như thế bằng các ký hiệu bớt cồng kềnh hơn. Chúng tôi sẽ dùng, đặc biệt, các tổ hợp ký hiệu (của một lý thuyết toán học), các chữ cái in nghiêng đậm (có hoặc không có chỉ số hoặc dấu phụ), và các ký hiệu đặc biệt, trong đó một số ví dụ sẽ được đưa ra. *Vì mục đích của chúng tôi chỉ là để tránh các cách nói quanh co* (xem chú ý (*), § 3, no. 1, p. 28) chúng tôi sẽ không phát biểu các quy tắc chung ngặt cho việc sử dụng các ký hiệu này; độc giả sẽ có thể tái lập không khó khăn dãy ký hiệu đang xét, trong mỗi trường hợp cụ thể. Bằng cách lạm dụng ngôn ngữ, chúng tôi thường sẽ nói rằng các ký hiệu *là* các dãy ký hiệu, hơn là chúng *ký hiệu* các dãy ký hiệu : các biểu thức như “dãy ký hiệu $A$” hoặc “chữ cái $x$”, trong các phát biểu của các quy tắc sau, do đó nên được thay bằng “dãy ký hiệu được ký hiệu bởi $A$” hoặc “chữ cái được ký hiệu bởi $x$”.

Cho $A$ và $B$ là các dãy ký hiệu. Ta sẽ ký hiệu $AB$ là dãy ký hiệu nhận được bằng cách viết dãy ký hiệu $B$ ở bên phải dãy ký hiệu $A$. Ta sẽ ký hiệu $\vee A\neg B$ là dãy ký hiệu nhận được bằng cách viết, từ trái sang phải, dấu $\vee$, dãy ký hiệu $A$, dấu $\neg$, dãy ký hiệu $B$. Và cứ thế.

Cho $A$ là một hợp thể và cho $x$ là một chữ cái. Chúng ta sẽ ký hiệu bằng $\tau_x(A)$ hợp thể được xây dựng như sau : dạng hợp thể $\tau A$, liên kết mỗi sự xuất hiện của $x$ trong $A$ với $\tau$ viết ở bên trái của $A$, và sau đó thay thế $x$ mọi nơi nó xuất hiện bằng dấu $\square$. Hợp thể ký hiệu bởi $\tau_x(A)$ do đó *không chứa* $x$.

#### Ví dụ {#ens-i-s1-n1-exa-3 .statement tag=03RY}

Ký hiệu $\tau_x(\in xy)$ biểu diễn hợp thể

$$
\tau\in\square y.
$$

Cho $A$ và $B$ là các dãy ký hiệu và $x$ là một chữ. Dãy ký hiệu thu được bằng cách thay thế $x$, tại mọi nơi nó xuất hiện trong $A$, bởi dãy ký hiệu $B$ được ký hiệu bởi $(B\mathbin{|}x)\,A$ (đọc: $B$ thay thế $x$ trong $A$). Nếu $x$ không xuất hiện trong $A$, thì $(B\mathbin{|}x)\,A$ đồng nhất với $A$; đặc biệt,

$$
(B\mathbin{|}x)\,\tau_x(A)
$$

là đồng nhất với $\tau_x(A)$.

#### Ví dụ {#ens-i-s1-n1-exa-4 .statement tag=03TO}

Nếu ta thay thế $x$ bằng $\square$ bất cứ nơi nào $x$ xuất hiện trong hợp tử $\vee\in xy=xx$, ta thu được hợp tử $\vee\in\square y=\square\square$.

Nếu $A$ là một hợp thể và chúng ta quan tâm đặc biệt đến một chữ cái $x$, hoặc hai chữ cái phân biệt $x$ và $y$ (có thể xuất hiện hoặc không xuất hiện trong $A$), chúng ta thường viết $A\{x\}$ hoặc $A\{x,y\}$. Trong trường hợp này chúng ta viết $A\{B\}$ thay vì $(B\mathbin{|}x)\,A$. Chúng ta ký hiệu bằng $A\{B,C\}$ hợp thể thu được bởi *đồng thời* thay thế $x$ bằng $B$ và $y$ bằng $C$ ở bất cứ đâu chúng xuất hiện trong $A$ (chú ý rằng $x$ và $y$ có thể xuất hiện trong $B$ và trong $C$); nếu $x'$ và $y'$ là các chữ cái phân biệt, khác với $x$ và $y$, không xuất hiện trong $A$, $B$, hay $C$, thì $A\{B,C\}$ là như nhau với $(B\mathbin{|}x')(C\mathbin{|}y')(x'\mathbin{|}x)(y'\mathbin{|}y)A$.

#### Chú ý {#ens-i-s1-n1-rem-1 .statement tag=03P2}

Khi một ký hiệu viết tắt $\Sigma$ được đưa vào, thông qua một định nghĩa, để biểu diễn một hợp thể nào đó, thì quy ước (thường ngầm) được thiết lập là biểu diễn hợp thể thu được bằng cách thay thế một hợp thể $B$ cho một chữ cái $x$ trong hợp thể ban đầu, bằng ký hiệu thu được bằng cách thay thế chữ cái $x$ trong $\Sigma$ bằng hợp thể $B$ (hoặc, thường hơn, bằng một ký hiệu viết tắt biểu diễn hợp thể $B$).

¶ *Ví dụ, sau khi đã được định nghĩa hợp thể nào được biểu diễn bởi ký hiệu $E\otimes F$, trong đó $E$ và $F$ là các chữ cái — một hợp thể, nhân tiện, chứa các chữ cái khác ngoài $E$ và $F$ — thì ký hiệu $Z\otimes F$ có thể được dùng mà không cần giải thích thêm.*

¶ Quy tắc này có thể dẫn đến những nhầm lẫn, mà những nhầm lẫn này được tránh bằng cách sử dụng các thiết bị trình bày khác nhau; cách thường thấy nhất là thay thế $x$ bằng $(B)$ thay vì $B$.

¶ *Ví dụ, $M\cap N$ biểu diễn một dãy ký hiệu chứa chữ cái $N$. Nếu ta thế $N$ bằng dãy ký hiệu được biểu diễn bởi $P\cup Q$, ta sẽ thu được một dãy ký hiệu được ký hiệu bởi $M\cap(P\cup Q)$.*

### 2. CÁC TIÊU CHUẨN THẾ

Toán học hình thức chỉ chứa các dãy ký hiệu được viết tường minh. Tuy nhiên, ngay cả khi sử dụng các bi tự viết tắt, sự phát triển của toán học theo đúng nguyên lý này sẽ dẫn đến những dãy lập luận cực kỳ dài. Vì lý do này, chúng tôi sẽ đưa ra các tiêu chuẩn liên quan đến các dãy ký hiệu không xác định; mỗi tiêu chuẩn trong số chúng sẽ mô tả một lần cho tất cả các kết quả cuối cùng của một dãy thao tác xác định trên các dãy ký hiệu đó. Những tiêu chuẩn này do đó không phải là không thể thiếu đối với lý thuyết; lý do của chúng thuộc về vi mô học.

Sự phát triển của vi mô học cũng yêu cầu, trong thực hành, sử dụng các bi tự viết tắt, một số trong số chúng đã được chỉ ra trước đó. Hầu hết các bi tự này cũng được sử dụng trong toán học.

Chúng tôi sẽ sử dụng các tiêu chuẩn sau đây, gọi là các *tiêu chuẩn thế*:

CS1. Cho $A$ và $B$ là các dãy ký hiệu và $x$ và $x'$ là các chữ cái. Nếu $x'$ không xuất hiện trong $A$, thì $(B|x)A$ giống hệt với $(B|x')(x'|x)A$.

CS2. Cho $A$, $B$ và $C$ là các dãy ký hiệu và cho $x$ và $y$ là các chữ cái phân biệt (*)[^3]. Nếu $y$ không xuất hiện trong $B$, thì $(B|x)(C|y)A$ giống hệt với

$$(C'|y)(B|x)A,$$

trong đó $C'$ là dãy ký hiệu $(B|x)C$.

CS3. *Cho $A$ là một hợp rải rác và cho $x$, $x'$ là các chữ cái. Nếu $x'$ không xuất hiện trong $A$, thì $\tau_x(A)$ giống hệt với $\tau_{x'}(A')$, trong đó $A'$ là hợp rải rác $(x'|x)\,A$.

CS4. *Cho $A$ và $B$ là các dãy ký hiệu và $x$ và $y$ là các chữ cái phân biệt. Nếu $x$ không xuất hiện trong $B$, thì $(B|y)\tau_xA$ đồng nhất với $\tau_x(A')$, trong đó $A'$ là dãy ký hiệu $(B|y)\,A$.*

CS5. *Cho $A$, $B$, $C$ là các dãy ký hiệu và cho $x$ là một ký tự. Các dãy ký hiệu $(C|x)(\neg A)$, $(C|x)(\vee AB)$, $(C|x)(\Rightarrow AB)$, $(C|x)(sAB)$ (trong đó $s$ là một dấu cụ thể) tương ứng đồng nhất với $\neg A'$, $\vee A'B'$, $\Rightarrow A'B'$, $sA'B'$, trong đó $A'$, $B'$ tương ứng là $(C|x)\,A$, $(C|x)\,B$.*

Như một ví dụ, ta hãy chỉ ra nguyên lý của việc xác minh CS2. So sánh phép toán đưa ta từ $A$ đến $(B|x)(C|y)\,A$ với phép toán đưa ta từ $A$ đến $(C|y)(B|x)\,A$. Trong mỗi phép toán, không có dấu nào xuất hiện trong $A$ và phân biệt với $x$ và $y$ bị thay đổi. Tại mỗi vị trí mà $x$ xuất hiện trong $A$, ta phải thay thế $B$ cho $x$ trong phép toán thứ nhất và trong phép toán thứ hai; điều này là rõ ràng đối với phép toán thứ nhất, và đối với phép toán thứ hai thì suy ra từ việc $y$ không xuất hiện trong $B$. Cuối cùng, tại mỗi vị trí mà $y$ xuất hiện trong $A$, phép toán thứ nhất gồm việc thay thế $C$ cho $y$, rồi $B$ cho $x$ tại mỗi vị trí mà $x$ xuất hiện trong $C$; nhưng rõ ràng rằng điều này tương đương với việc thay thế cho $y$, bất cứ nơi nào nó xuất hiện trong $A$, hợp thể $(B|x)\,C$.

### 3. PHÉP DỰNG KIẾN TẠO

Một số dấu hiệu cụ thể của một lý thuyết được gọi là *quan hệ*, và những dấu hiệu khác được gọi là *thực thể*. Với mỗi dấu hiệu cụ thể được liên kết một số tự nhiên gọi là *trọng số* (thường là số 2).

¶ Một dãy ký hiệu được gọi là *loài thứ nhất* nếu nó bắt đầu bằng một $\tau$, hoặc với một dấu hiệu *thực thể*, hay nếu nó chỉ là một ký tự đơn lẻ; nếu không thì nó là *loài thứ hai*.

¶ Một *phép dựng kiến tạo* trong một lý thuyết $\mathscr{T}$ là một dãy các dãy ký hiệu có tính chất sau : với mỗi dãy ký hiệu $A$ trong dãy, một trong các điều kiện sau được thỏa mãn :

(a) $A$ là một ký tự.

(b) Trong dãy có một dãy ký hiệu $B$ thuộc loài thứ hai, đứng trước $A$, sao cho $A$ là $\neg B$.

(c) Có hai dãy ký hiệu $B$ và $C$ thuộc loài thứ hai (phân biệt hoặc không), đứng trước $A$, sao cho $A$ là $\vee BC$.

(d) Có một dãy ký hiệu $B$ thuộc loài thứ hai, đứng trước $A$, và một chữ cái $x$ sao cho $A$ là $\tau_x(B)$.

(e) Có một ký hiệu cụ thể $s$ có trọng số $n$ (*)[^4] trong $\mathscr{T}$, và $n$ dãy ký hiệu $A_1,A_2,\ldots,A_n$ thuộc loài thứ nhất, đứng trước $A$, sao cho $A$ là $sA_1A_2\ldots A_n$.

¶ Các dãy ký hiệu thuộc loài thứ nhất (tương ứng thuộc loài thứ hai) xuất hiện trong các phép kiến tạo của $\mathscr{T}$ được gọi là các thuật hạng (tương ứng các quan hệ) trong $\mathscr{T}$.

*Ví dụ.* *Trong lý thuyết tập hợp, trong đó $\in$ là một dấu quan hệ có trọng số 2, dãy các dãy ký hiệu sau là một phép dựng kiến tạo:*

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

Do đó, dãy ký hiệu được cho làm ví dụ ở số 1 là một số hạng trong lý thuyết tập hợp.*

*Nhận xét.* Theo trực giác, các số hạng là các dãy ký hiệu biểu diễn các đối tượng, và các quan hệ là các dãy ký hiệu biểu diễn các mệnh đề có thể được đưa ra về các đối tượng này. Điều kiện (a) có nghĩa là các chữ cái biểu diễn các đối tượng. Điều kiện (b) có nghĩa là nếu $B$ là một mệnh đề, thì $\neg B$, được gọi là phủ định của $B$, là một mệnh đề (được đọc : không $B$). Điều kiện (c) có nghĩa là nếu $B$ và $C$ là các mệnh đề, thì $\vee BC$, được gọi là sự tuyển của $B$ và $C$, là một mệnh đề (được đọc : hoặc $B$ hoặc $C$); do đó $\neg\to BC$ là một mệnh đề (diễn đạt bằng lời : “hoặc không $B$, hoặc $C$”, hay “$B$ kéo theo $C$”). Điều kiện (d) có nghĩa là nếu $B$ là một mệnh đề và $x$ là một chữ cái, thì $\tau_x(B)$ là một đối tượng. Hãy xem mệnh đề $B$ như biểu đạt một tính chất của đối tượng $X$; khi đó, nếu tồn tại một đối tượng có tính chất nói trên, thì $\tau_x(B)$ biểu diễn một đối tượng đặc biệt có tính chất này; nếu không, $\tau_x(B)$ biểu diễn một đối tượng mà không có gì có thể nói về nó. Cuối cùng, điều kiện (e) có nghĩa là nếu $A_1,A_2,\ldots,A_n$ là các đối tượng, và nếu $s$ là một dấu quan hệ (resp. substantific) có trọng số $n$, thì $sA_1A_2\ldots A_n$ là một mệnh đề về các đối tượng $A_1,\ldots,A_n$ (resp. một đối tượng phụ thuộc vào $A_1,\ldots,A_n$).

*Ví dụ.* Các ký hiệu $\varnothing$, $\mathbf{N}$, “dòng thực”, “hàm $\Gamma$”, $f\circ g$ là các số hạng. Các ký hiệu $\pi=\sqrt{2}+\sqrt{3}$, $1\in2$, “mọi hữu hạn

vành chia là một trường”, “các không điểm của $\zeta(s)$ khác với $-2$, $-4$, $-6$, ... nằm trên dòng $\mathfrak{R}(s)=1/2$” là các quan hệ. Ký hiệu “3 và 4” không phải là số hạng cũng không phải là quan hệ.

Ký hiệu ban đầu của một quan hệ là $\vee$, $\neg$, hoặc một ký hiệu quan hệ. Ký hiệu ban đầu của một số hạng là $\tau$ hoặc một ký hiệu substantific, với điều kiện là số hạng đó không gồm một chữ cái đơn. Mệnh đề sau suy ra từ việc một số hạng là một dãy ký hiệu của loài thứ nhất. Nếu $A$ là một quan hệ, thì $A$ xuất hiện trong một phép dựng kiến tạo, không phải là một chữ cái, và không bắt đầu bằng $\tau$, do đó có ba trường hợp có thể : (1) $A$ đứng sau một dãy ký hiệu $B$ sao cho $A$ là $\neg B$; (2) $A$ đứng sau hai dãy ký hiệu $B$ và $C$ sao cho $A$ là $\vee BC$; (3) $A$ đứng sau các dãy ký hiệu $A_1$, $A_2$, ... $A_n$ sao cho $A$ là $sA_1A_2 ... A_n$, với $s$ là một ký hiệu quan hệ.

### 4. CÁC TIÊU CHUẨN KIẾN TẠO

CF1. Nếu $A$ và $B$ là các quan hệ trong một lý thuyết $\mathscr{T}$, thì $\vee AB$ là một quan hệ trong $\mathscr{T}$.

Xét hai phép dựng kiến tạo (trong $\mathscr{T}$), một cái chứa $A$ và cái kia chứa $B$. Xét dãy các dãy ký hiệu thu được bằng cách viết trước tiên các dãy ký hiệu của phép dựng thứ nhất, sau đó các dãy ký hiệu của phép dựng thứ hai, và cuối cùng $\vee AB$. Vì $A$ và $B$ thuộc loài thứ hai, nên ngay lập tức được xác minh rằng dãy này là một phép dựng kiến tạo của $\mathscr{T}$. Dãy ký hiệu $\vee AB$ thuộc loài thứ hai, do đó nó là một quan hệ trong $\mathscr{T}$.

Ba tiêu chuẩn sau được thiết lập tương tự :

CF2. Nếu $A$ là một quan hệ trong một lý thuyết $\mathscr{T}$, thì $\neg A$ là một quan hệ trong $\mathscr{T}$.

CF3. Nếu $A$ là một quan hệ trong một lý thuyết $\mathscr{T}$, và nếu $x$ là một chữ cái, thì $\tau_x(A)$ là một số hạng trong $\mathscr{T}$.

CF4. Nếu $A_1$, $A_2$, ..., $A_n$ là các số hạng trong một lý thuyết $\mathscr{T}$, và nếu $s$ là một dấu quan hệ (tương ứng là dấu substantific) có trọng số $n$ trong $\mathscr{T}$, thì $sA_1A_2...A_n$ là một quan hệ (tương ứng là một số hạng) trong $\mathscr{T}$.

Các tiêu chuẩn này ngay lập tức kéo theo điều sau :

CF5. Nếu $A$ và $B$ là các quan hệ trong một lý thuyết $\mathscr{T}$, thì $\Longrightarrow AB$ là một quan hệ trong $\mathscr{T}$.

CF6. Cho $A_1$, $A_2$, ..., $A_n$ là một phép dựng kiến tạo trong một lý thuyết $\mathscr{T}$, và cho $x$ và $y$ là các chữ cái. Giả sử rằng $y$ không xuất hiện trong bất kỳ $A_i$ nào. Khi đó $(y|x) A_1$, $(y|x) A_2$, ..., $(y|x) A_n$ là một phép dựng kiến tạo trong $\mathscr{T}$.

Để chứng minh CF6, cho $A'_i$ là hợp tử $(y|x)A_i$. Nếu $A_i$ là một chữ cái, thì $A'_i$ là một chữ cái. Nếu $A_i$ có dạng $\neg A_j$, với $A_j$ là một hợp tử thuộc loài thứ hai đứng trước $A_i$ trong phép dựng, thì $A'_i$ đồng nhất với $\neg A'_j$ theo CS5, và $A'_j$ là một hợp tử thuộc loài thứ hai. Lập luận đồng dạng nếu $A_i$ có dạng $\vee A_jA_k$ hoặc $sA_{j_1}A_{j_2}\ldots A_{j_m}$, với $s$ là một dấu cụ thể của $\mathscr{T}$. Cuối cùng, nếu $A_i$ có dạng $\tau_z(A_j)$, với $A_j$ là một hợp tử thuộc loài thứ hai đứng trước $A_i$ trong phép dựng, thì có nhiều trường hợp cần xét :

(a) $z$ là một chữ cái phân biệt với $x$ và $y$. Khi đó $A'_i$ đồng nhất với $\tau_z(A'_j)$ theo CS4, và $A'_j$ là một hợp tử của loài thứ hai.

(b) $z$ đồng nhất với $x$. Khi đó $A_i$ không chứa $x$, do đó $A'_i$ đồng nhất với $A_i$, tức là với $\tau_x(A_j)$; vì $y$ không xuất hiện trong $A_j$, $\tau_x(A_j)$ đồng nhất với $\tau_y(A_j)$ theo CS3.

(c) $z$ đồng nhất với $y$. Khi đó $A_i$ là hợp tử $\tau A_j$, vì $y$ không xuất hiện trong $A_j$; do đó $A'_i$ là hợp tử $\tau A'_j$, tức là $\tau_u(A'_j)$, trong đó $u$ là một chữ cái không xuất hiện trong $A'_j$.

**CF7.** *Cho $A$ là một quan hệ (resp. một số hạng) trong một lý thuyết $\mathscr{T}$, và cho $x$ và $y$ là các chữ cái. Khi đó $(y|x)A$ là một quan hệ (resp. một số hạng) trong $\mathscr{T}$.*

Cho $A_1,A_2,\ldots,A_n$ là một phép dựng kiến tạo trong đó $A$ xuất hiện. Ta sẽ chỉ ra từng bước rằng, nếu $A_i$ là một quan hệ (tương ứng, một số hạng) thì $(y|x)A_i$, mà ta sẽ ký hiệu là $A'_i$, cũng là một quan hệ (tương ứng, một số hạng). Giả sử điểm này đã được thiết lập đối với $A_1,A_2,\ldots,A_{i-1}$; ta hãy chứng minh nó đối với $A_i$. Nếu $A_i$ là một chữ cái, thì $A'_i$ là một chữ cái. Nếu trong phép dựng, $A_i$ đứng sau một quan hệ $A_j$ sao cho $A_i$ là $\neg A_j$, thì theo CS5, $A'_i$ đồng nhất với $\neg A'_j$, và $\neg A'_j$ là một quan hệ theo CF2. Lập luận cũng tương tự nếu $A_i$ đứng sau các quan hệ $A_j,A_k$ sao cho $A_i$ là $\vee A_jA_k$, hoặc nếu $A_i$ đứng sau các số hạng $A_{j_1},\ldots,A_{j_m}$ sao cho $A_i$ là $sA_{j_1}\ldots A_{j_m}$, trong đó $s$ là một dấu hiệu cụ thể của $\mathscr{T}$ có trọng số $m$. Cuối cùng, nếu $A_i$ đứng sau một quan hệ $A_j$ sao cho $A_i$ là $\tau_z(A_j)$, có nhiều trường hợp khác nhau cần xét :

(a) $z$ phân biệt với cả $x$ và $y$. Khi đó $A'_i$ đồng nhất với $\tau_z(A'_j)$ theo CS4, và ta đã biết rằng $A'_j$ là một quan hệ; do đó $A_i$ là một số hạng, theo CF3.

(b) $z$ đồng nhất với $x$. Khi đó $A_i$ không chứa $x$, vì vậy $A'_i$ đồng nhất với $A_i$, và do đó là một số hạng.

(c) $z$ đồng nhất với $y$. Khi đó, lấy $u$ là một chữ cái, phân biệt với cả $x$ và $y$, không xuất hiện trong $A_1,A_2,\ldots,A_j$. Theo CF6, dãy các dãy ký hiệu $(u|y)A_1,\ldots,(u|y)A_j$, mà ta ký hiệu bởi $A''_1,\ldots,A''_j$, tạo thành một phép dựng kiến tạo trong $\mathscr{T}$. Vì $y$ không còn xuất hiện trong phép dựng mới này, $(y|x)A''_1,\ldots,(y|x)A''_j$ là một phép dựng kiến tạo theo CF6, nên $(y|x)A''_j$ là một quan hệ trong $\mathscr{T}$; do đó $\tau_u((y|x)A''_j)$

là một số hạng của $\mathscr{T}$. Nhưng số hạng này đồng nhất với $(y|x)\tau_u(A_j'')$ theo CS4, do đó với $(y|x)\tau_y(A_j)$ theo CS3, do đó đồng nhất với $A_i$.

CF8. Cho $A$ là một quan hệ (tương ứng là một số hạng) trong một lý thuyết $\mathscr{T}$, cho $x$ là một chữ cái và $T$ là một số hạng trong $\mathscr{T}$. Khi đó $(T|x)A$ là một quan hệ (tương ứng là một số hạng) trong $\mathscr{T}$.

Cho $A_1, A_2, \ldots, A_n$ là một phép dựng kiến tạo trong đó $A$ xuất hiện. Cho $x_1, x_2, \ldots, x_p$ là các chữ cái phân biệt xuất hiện trong $T$. Hãy liên kết với mỗi chữ cái $x_i$ một chữ cái $x_i'$, phân biệt với mỗi chữ cái trong các chữ cái $x_1, \ldots, x_p$ và các chữ cái xuất hiện trong $A_1, \ldots, A_n$, sao cho các chữ cái $x_1', \ldots, x_p'$ đều phân biệt. Hợp thể

$$
(x_1'|x_1)(x_2'|x_2)\ldots(x_p'|x_p)T
$$

là một số hạng $T'$ theo CF7, và $(T|x)A$ đồng nhất với

$$
(x_1|x_1')(x_2|x_2')\ldots(x_p|x_p')(T'|x)A
$$

Bằng cách áp dụng CS1. Do đó đủ để chỉ ra rằng $(T'|x)\,A$ là một quan hệ (tương ứng một số hạng); nói cách khác, ta có thể giả sử từ nay trở đi rằng các chữ cái xuất hiện trong $T$ không xuất hiện trong $A_1, \ldots, A_n$.

¶ Chúng ta sẽ chỉ ra từng bước rằng, nếu $A_t$ là một quan hệ (tương ứng một số hạng), thì $(T|x)\,A_t$, mà chúng ta sẽ ký hiệu bởi $A_t'$, là một quan hệ (tương ứng một số hạng). Giả sử điểm này đã được thiết lập cho $A_1,A_2,\ldots,A_{i-1}$, và chúng ta hãy chứng minh nó cho $A_i$. Nếu $A_i$ là một chữ cái, thì $A_i'$ hoặc là chính chữ cái đó hoặc là $T$, và do đó là một số hạng. Nếu $A_i$ có dạng $\neg A_j$, trong đó $A_j$ là một quan hệ đi trước $A_i$ trong phép dựng, thì $A_i$ đồng nhất với $\neg A_j'$ theo CS5, và chúng ta đã biết rằng $A_j'$ là một quan hệ, suy ra $A_i'$ là một quan hệ theo CF2. Chứng minh tương tự nếu $A_i$ có dạng $\vee A_jA_k$, hoặc $sA_{j_1}\ldots A_{j_m}$. Cuối cùng, nếu $A_i$ có dạng $\tau_z(A_j)$, trong đó $A_j$ là một quan hệ đi trước $A_i$ trong phép dựng, thì có nhiều trường hợp cần xét:

(a) $z$ phân biệt với $x$ và với các chữ cái xuất hiện trong $T$. Khi đó $A_i'$ đồng nhất với $\tau_z(A_j')$ theo CS4, và ta đã biết rằng $A_j'$ là một quan hệ; do đó $A_i'$ là một số hạng theo CF3.

(b) $z$ đồng nhất với $x$. Khi đó $A_i$ không chứa $x$, vì vậy $A_i'$ đồng nhất với $A_i$ và do đó là một số hạng.

(c) $z$ xuất hiện trong $T$. Khi đó $z$ không xuất hiện trong $A_j$, do đó $A_i'$ đồng nhất với $\tau A_j'$; suy ra $A_i'$ đồng nhất với $\tau A_j'$. Nay, ta đã biết rằng $A_j'$ là một quan hệ, và $\tau A_j'$ đồng nhất với $\tau_u(A_j)$, trong đó $u$ là một chữ cái không xuất hiện trong $A_j$; theo CF3 thì $A_i'$ là một số hạng.

Một cách trực quan, nếu $A$ là một quan hệ trong $\mathscr{T}$, mà ta có thể coi là biểu thị một tính chất của một đối tượng $x$, thì mệnh đề $(B|x)\,A$ có nghĩa là nói rằng đối tượng $B$ có tính chất này. Nếu $A$ là một số hạng trong $\mathscr{T}$, nó biểu diễn một đối tượng phụ thuộc theo một cách nào đó vào đối tượng được ký hiệu bởi $x$; số hạng $(B|x)\,A$ biểu diễn đối tượng mà $A$ trở thành khi ta lấy $x$ là đối tượng $B$.

### Bài tập {#ens-i-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).

[^1]: (\*) Ý nghĩa của biểu thức này sẽ trở nên rõ ràng khi chương tiến triển.
[^2]: (†) Về các ý nghĩa trực quan của các dấu này, xem no. 3, Nhận xét.
[^3]: (*) Phù hợp với những gì đã nói ở no. 1, cụm từ “$x$ và $y$ là các chữ cái phân biệt” là một lạm dụng ngôn ngữ: nó có nghĩa là $x$ và $y$ ký hiệu các chữ cái phân biệt trong các dãy ký hiệu đang xét.
[^4]: (*) Như đã nói ở trên, sẽ có thể, cho sự phát triển của các lý thuyết toán học hiện đại, để giới hạn sự xem xét của chúng ta vào các dấu cụ thể có trọng số 2, và do đó tránh sử dụng biểu thức “số tự nhiên $n$” trong định nghĩa của một phép dựng kiến tạo.
