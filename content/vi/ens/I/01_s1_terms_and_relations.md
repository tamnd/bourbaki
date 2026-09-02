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
content_sha256: 83fb05f03ae0fe9178ceaa09408161d84de142a688363d3cf9314bc2bc79c323
translated_from: content/en/ens/I/01_s1_terms_and_relations.md
source_content_sha256: 0ee801130c4937b60178227e19ee4a8160108632ae38780ac29f1c6072b194de
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5-mini, gpt-5.4-mini
translation_run: translate-vi-5cba219d
glossary_version: 34
glossary_terms_sha256: 94e6d486425f76b2257b42050037bcd297da3db28df6566037e6a5aea05f244b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. THUẬT NGỮ VÀ QUAN HỆ

### 1. CÁC DẤU VÀ CÁC DÃY KÝ HIỆU

Các *dấu* của một lý thuyết toán học $\mathscr{T}$ [^1] là các dấu sau đây :

(1) Các *dấu lôgic* [^2] : $\square$, $\tau$, $\vee$, $\neg$.
(2) Các *chữ*.

Các chữ là các chữ La tinh viết hoa và viết thường, có hoặc không có dấu. Như vậy $A$, $A'$, $A''$, $A'''$, ... là các chữ. Tại bất kỳ chỗ nào trong văn bản, có thể đưa vào các chữ khác với những chữ đã xuất hiện trong các lập luận trước đó.

(3) Các *dấu riêng*, phụ thuộc vào lý thuyết đang xét.

Trong lý thuyết tập hợp, ta chỉ sử dụng ba dấu riêng sau đây : $=$, $\in$, $\supset$.

Một *dãy ký hiệu* trong $\mathscr{T}$ là một dãy liên tiếp các dấu của $\mathscr{T}$ được viết cạnh nhau; một số dấu, khác với các chữ, có thể được nối từng đôi bằng các gạch ở phía trên dòng, gọi là *các liên kết*. \*Ví dụ, trong LÝ THUYẾT TẬP HỢP, trong đó $\in$ là một dấu riêng,

$$\overline{\overline{\tau \vee \neg \in \square} A' \in \square} A''$$

là một dãy ký hiệu.\*

Việc chỉ sử dụng các dãy ký hiệu sẽ dẫn đến những khó khăn không thể vượt qua cả đối với người in lẫn người đọc. Vì lý do này, các văn bản hiện nay sử dụng những ký hiệu viết tắt (đáng chú ý là các từ ngữ thông thường) không thuộc về toán học hình thức. Việc đưa vào các ký hiệu như vậy là đối tượng của các *định nghĩa*. Việc sử dụng chúng *không phải là không thể thiếu đối với lý thuyết*, và thường có thể dẫn đến sự nhầm lẫn mà chỉ một mức độ quen thuộc nhất định với chủ đề mới cho phép người đọc tránh được.

*Ví dụ*

#### Ví dụ 1 {#ens-i-s1-n1-exa-1 .statement tag=03P0}

Dãy ký hiệu $\vee 1$ được biểu diễn bởi $\Rightarrow$.

#### Ví dụ 2 {#ens-i-s1-n1-exa-2 .statement tag=03P1}

Các ký hiệu sau đây biểu diễn các dãy ký hiệu (và hơn nữa là những dãy rất dài):

“3 và 4”

$$\varnothing$$

$$\mathbf{N}$$

$$\mathbf{Z}$$

“đường thẳng thực”

“hàm $\Gamma$”

$$f\circ g$$

$$\pi=\sqrt{2}+\sqrt{3}$$

$$1\in 2$$

“Mọi vành chia hữu hạn đều là một trường”

“Các không điểm của $\zeta(s)$ khác với $-2$, $-4$, $-6$, ... nằm trên đường thẳng $R(s)=1/2$.”

Nói chung, ký hiệu được dùng để biểu diễn một dãy ký hiệu chứa tất cả các chữ cái xuất hiện trong dãy ký hiệu đó. Tuy nhiên, nguyên lý này đôi khi có thể bị vi phạm mà không có nguy cơ gây nhầm lẫn. *Chẳng hạn, “phép hoàn thiện của X” biểu diễn một dãy ký hiệu chứa chữ cái X, nhưng cũng chứa chữ cái biểu diễn tập hợp các lân cận của cấu trúc đều của X. Mặt khác,

$$\int_0^1 f(x)\,dx$$

biểu diễn một dãy ký hiệu trong đó chữ $x$ (và chữ $d$) không xuất hiện; và các dãy ký hiệu được biểu diễn bởi $\mathbf{N}$, $\mathbf{Z}$, “hàm $\Gamma$” không chứa chữ nào.*

Một *lý thuyết toán học* (hay đơn giản là một *lý thuyết*) chứa các quy tắc cho phép ta khẳng định rằng một số dãy ký hiệu nào đó là *hạng hoặc quan hệ* của lý thuyết, và các quy tắc khác cho phép ta khẳng định rằng một số dãy ký hiệu nào đó là *định lý* của lý thuyết.

*Mô tả* các quy tắc này, sẽ *xuất hiện* trong chương này, *không thuộc toán học hình thức*; các quy tắc liên quan đến những dãy ký hiệu ít nhiều chưa được xác định, chẳng hạn các chữ chưa được xác định. Để đơn giản hóa cách trình bày, thuận tiện nhất là ký hiệu các dãy ký hiệu ấy bằng những ký hiệu ít cồng kềnh hơn. Đặc biệt, ta sẽ sử dụng các tổ hợp ký hiệu (của một lý thuyết toán học), các chữ in đậm nghiêng (có hoặc không có chỉ số hoặc dấu), và các ký hiệu đặc biệt, trong đó sẽ nêu một số ví dụ. *Vì mục đích của chúng ta chỉ là tránh những cách diễn đạt vòng vo* (xem chú ý (*), § 3, no. 1, p. 28), ta sẽ không phát biểu các quy tắc tổng quát ngặt về việc sử dụng các ký hiệu này; trong từng trường hợp cụ thể, người đọc sẽ có thể dễ dàng dựng lại dãy ký hiệu đang xét. Theo lối nói không hoàn toàn chính xác, ta sẽ thường nói rằng các ký hiệu *là* các dãy ký hiệu, thay vì nói rằng chúng *biểu thị* các dãy ký hiệu: những biểu thức như “dãy ký hiệu $A$” hoặc “chữ $x$”, trong các phát biểu của những quy tắc sau đây, do đó phải được thay bằng “dãy ký hiệu được biểu thị bởi $A$” hoặc “chữ được biểu thị bởi $x$”.

Cho $A$ và $B$ là các dãy ký hiệu. Ta sẽ ký hiệu bởi $AB$ dãy ký hiệu thu được bằng cách viết dãy ký hiệu $B$ ở bên phải dãy ký hiệu $A$. Ta sẽ ký hiệu bởi $\vee A\neg B$ dãy ký hiệu thu được bằng cách viết, từ trái sang phải, dấu $\vee$, dãy ký hiệu $A$, dấu $\neg$, dãy ký hiệu $B$. Và cứ thế.

Cho $A$ là một cấu tạo và $x$ là một chữ cái. Ta sẽ ký hiệu bởi $\tau_x(A)$ cấu tạo được xây dựng như sau : tạo cấu tạo $\tau A$, nối mỗi lần xuất hiện của $x$ trong $A$ với $\tau$ được viết ở bên trái của $A$, rồi thay thế $x$ ở mọi nơi nó xuất hiện bằng dấu $\square$. Cấu tạo được ký hiệu bởi $\tau_x(A)$ do đó *không chứa* $x$.

#### Ví dụ {#ens-i-s1-n1-exa-3 .statement tag=03RY}

Ký hiệu $\tau_x(\in xy)$ biểu diễn cấu tạo

$$
\tau\in\square y.
$$

Cho $A$ và $B$ là các dãy ký hiệu và cho $x$ là một chữ cái. Dãy ký hiệu thu được bằng cách thay thế $x$, ở mọi nơi nó xuất hiện trong $A$, bằng dãy ký hiệu $B$ được ký hiệu bởi $(B\mathbin{|}x)\,A$ (đọc: $B$ thay thế $x$ trong $A$). Nếu $x$ không xuất hiện trong $A$, thì $(B\mathbin{|}x)\,A$ trùng với $A$; đặc biệt,

$$
(B\mathbin{|}x)\,\tau_x(A)
$$

là đồng nhất với $\tau_x(A)$.

#### Ví dụ {#ens-i-s1-n1-exa-4 .statement tag=03TO}

Nếu ta thay thế $x$ bởi $\square$ ở mọi nơi $x$ xuất hiện trong hệ thức $\vee\in xy=xx$, ta thu được hệ thức $\vee\in\square y=\square\square$.

Nếu $A$ là một cấu trúc và ta đặc biệt quan tâm đến một chữ cái $x$, hoặc hai chữ cái phân biệt $x$ và $y$ (có thể xuất hiện hoặc không xuất hiện trong $A$), ta thường sẽ viết $A\{x\}$ hoặc $A\{x,y\}$. Trong trường hợp này ta viết $A\{B\}$ thay cho $(B\mathbin{|}x)\,A$. Ta ký hiệu bởi $A\{B,C\}$ cấu trúc thu được bằng cách *đồng thời* thay thế $x$ bởi $B$ và $y$ bởi $C$ ở mọi nơi chúng xuất hiện trong $A$ (chú ý rằng $x$ và $y$ có thể xuất hiện trong $B$ và trong $C$); nếu $x'$ và $y'$ là các chữ cái phân biệt, khác với $x$ và $y$, không xuất hiện trong $A$, $B$, cũng như $C$, thì $A\{B,C\}$ trùng với $(B\mathbin{|}x')(C\mathbin{|}y')(x'\mathbin{|}x)(y'\mathbin{|}y)A$.

#### Nhận xét {#ens-i-s1-n1-rem-1 .statement tag=03P2}

Khi một ký hiệu viết tắt $\Sigma$ được đưa vào, bằng một định nghĩa, để biểu diễn một cấu tạo nào đó, quy ước (thường là ngầm hiểu) được đặt ra là biểu diễn cấu tạo thu được bằng cách thay thế một cấu tạo $B$ cho một chữ cái $x$ trong cấu tạo ban đầu, bằng ký hiệu thu được do thay thế chữ cái $x$ trong $\Sigma$ bằng cấu tạo $B$ (hoặc, thường hơn, bằng một ký hiệu viết tắt biểu diễn cấu tạo $B$).

¶ *Ví dụ, sau khi đã định nghĩa cấu tạo nào được biểu diễn bởi ký hiệu $E\otimes F$, trong đó $E$ và $F$ là các chữ cái — một cấu tạo mà tình cờ còn chứa các chữ cái khác ngoài $E$ và $F$ — ký hiệu $Z\otimes F$ có thể được sử dụng mà không cần giải thích thêm.*

¶ Quy tắc này có thể dẫn đến những nhầm lẫn, được tránh bằng việc sử dụng các phương tiện kiểu chữ khác nhau; phương tiện thông dụng nhất là thay $x$ bằng $(B)$ thay cho $B$.

¶ *Ví dụ, $M\cap N$ biểu thị một dãy ký hiệu chứa chữ cái $N$. Nếu ta thế vào $N$ dãy ký hiệu được biểu diễn bởi $P\cup Q$, ta được một dãy ký hiệu được biểu thị bởi $M\cap(P\cup Q)$.*

### 2. CÁC TIÊU CHUẨN THẾ

Toán học hình thức chỉ chứa các dãy ký hiệu được viết tường minh. Tuy nhiên, ngay cả khi sử dụng các ký hiệu viết tắt, sự phát triển của toán học hoàn toàn phù hợp với nguyên lý này sẽ dẫn đến những chuỗi lập luận cực kỳ dài. Vì lý do này, ta sẽ thiết lập các tiêu chuẩn liên quan đến các dãy ký hiệu bất định; mỗi tiêu chuẩn trong số này sẽ mô tả một lần cho mãi kết quả cuối cùng của một dãy phép biến đổi xác định trên các dãy ký hiệu này. Do đó, các tiêu chuẩn này không phải là thiết yếu đối với lý thuyết; sự biện minh cho chúng thuộc về siêu toán học.

Sự phát triển của chính siêu toán học, trên thực tế, đòi hỏi việc sử dụng các ký hiệu viết tắt, một số trong đó đã được chỉ ra. Phần lớn các ký hiệu này cũng được sử dụng trong toán học.

Ta sẽ sử dụng các tiêu chuẩn sau đây, được gọi là *các tiêu chuẩn thế* :

CS1. Cho $A$ và $B$ là các dãy ký hiệu và cho $x$ và $x'$ là các chữ cái. Nếu $x'$ không xuất hiện trong $A$, thì $(B|x)A$ đồng nhất với $(B|x')(x'|x)A$.

CS2. Cho $A$, $B$, và $C$ là các dãy ký hiệu và cho $x$ và $y$ là các chữ cái phân biệt [^3]. Nếu $y$ không xuất hiện trong $B$, thì $(B|x)(C|y)A$ đồng nhất với

$$(C'|y)(B|x)A,$$

trong đó $C'$ là dãy ký hiệu $(B|x)C$.

CS3. *Cho $A$ là một assembly và cho $x$ và $x'$ là các chữ. Nếu $x'$ không xuất hiện trong $A$, thì $\tau_x(A)$ đồng nhất với $\tau_{x'}(A')$, trong đó $A'$ là assembly $(x'|x)\,A$.*

CS4. *Cho $A$ và $B$ là các dãy ký hiệu và cho $x$ và $y$ là các chữ cái phân biệt. Nếu $x$ không xuất hiện trong $B$, thì $(B|y)\tau_xA$ đồng nhất với $\tau_x(A')$, trong đó $A'$ là dãy ký hiệu $(B|y)\,A$.*

CS5. *Cho $A$, $B$, $C$ là các dãy ký hiệu và cho $x$ là một chữ cái. Các dãy ký hiệu $(C|x)(\neg A)$, $(C|x)(\vee AB)$, $(C|x)(\Rightarrow AB)$, $(C|x)(sAB)$ (trong đó $s$ là một dấu hiệu cụ thể) lần lượt đồng nhất với $\neg A'$, $\vee A'B'$, $\Rightarrow A'B'$, $sA'B'$, trong đó $A'$, $B'$ lần lượt là $(C|x)\,A$, $(C|x)\,B$.*

Ví dụ, hãy chỉ ra nguyên lý kiểm chứng CS2. So sánh phép toán đưa ta từ $A$ đến $(B|x)(C|y)\,A$ với phép toán đưa ta từ $A$ đến $(C|y)(B|x)\,A$. Trong mỗi phép toán, không có dấu nào xuất hiện trong $A$ và phân biệt với $x$ và $y$ bị thay đổi. Tại mỗi chỗ $x$ xuất hiện trong $A$, ta phải thay thế $B$ cho $x$ trong phép toán thứ nhất và thứ hai; điều này hiển nhiên đối với phép toán thứ nhất, còn đối với phép toán thứ hai nó suy ra từ sự kiện rằng $y$ không xuất hiện trong $B$. Cuối cùng, tại mỗi chỗ $y$ xuất hiện trong $A$, phép toán thứ nhất gồm việc thay thế $C$ cho $y$, rồi $B$ cho $x$ tại mỗi chỗ $x$ xuất hiện trong $C$; nhưng rõ ràng điều này cũng chính là việc thay thế cho $y$, ở mọi nơi nó xuất hiện trong $A$, hợp thành $(B|x)\,C$.

### 3. CÁC PHÉP DỰNG KIẾN TẠO

Một số dấu hiệu riêng của một lý thuyết được gọi là *liên hệ*, còn các dấu hiệu khác được gọi là *thực thể*. Với mỗi dấu hiệu riêng được liên kết một số tự nhiên gọi là *trọng số* của nó (hầu như luôn luôn là số 2).

¶ Một dãy ký hiệu được nói là thuộc *loài thứ nhất* nếu nó bắt đầu bằng một $\tau$, hoặc bằng một dấu hiệu thực thể, hoặc nếu nó gồm một chữ cái duy nhất; ngược lại nó thuộc *loài thứ hai*.

¶ Một *phép dựng kiến tạo* trong một lý thuyết $\mathscr{T}$ là một dãy các dãy ký hiệu có tính chất sau đây: đối với mỗi dãy ký hiệu $A$ của dãy, một trong các điều kiện sau được thỏa mãn:

(a) $A$ là một chữ cái.

(b) Có trong dãy một dãy ký hiệu $B$ thuộc loài thứ hai, đứng trước $A$, sao cho $A$ là $\neg B$.

(c) Có hai dãy ký hiệu $B$ và $C$ thuộc loài thứ hai (phân biệt hoặc không), đứng trước $A$, sao cho $A$ là $\vee BC$.

(d) Có một dãy ký hiệu $B$ thuộc loài thứ hai, đứng trước $A$, và một chữ cái $x$ sao cho $A$ là $\tau_x(B)$.

(e) Có một dấu hiệu riêng biệt $s$ có trọng số $n$ [^4] trong $\mathscr{T}$, và $n$ dãy ký hiệu $A_1,A_2,\ldots,A_n$ thuộc loài thứ nhất, đứng trước $A$, sao cho $A$ là $sA_1A_2\ldots A_n$.

¶ Các dãy ký hiệu thuộc loài thứ nhất (tương ứng thuộc loài thứ hai) xuất hiện trong các kiến tạo của $\mathscr{T}$ được gọi là các hạng (tương ứng các quan hệ) trong $\mathscr{T}$.

*Ví dụ.* *Trong lý thuyết tập hợp, trong đó $\in$ là một dấu quan hệ có trọng số 2, dãy ký hiệu sau là một phép dựng kiến tạo:*

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

*Nhận xét.* Về trực giác, các thuật ngữ là các dãy ký hiệu biểu diễn các đối tượng, và các quan hệ là các dãy ký hiệu biểu diễn các mệnh đề có thể được phát biểu về các đối tượng này. Điều kiện (a) có nghĩa là các chữ cái biểu diễn các đối tượng. Điều kiện (b) có nghĩa là nếu $B$ là một mệnh đề, thì $\neg B$, được gọi là phủ định của $B$, là một mệnh đề (được đọc là: không $B$). Điều kiện (c) có nghĩa là nếu $B$ và $C$ là các mệnh đề, thì $\vee BC$, được gọi là phép tuyển của $B$ và $C$, là một mệnh đề (được đọc là: hoặc $B$ hoặc $C$); do đó $\neg\to BC$ là một mệnh đề (bằng lời: “hoặc không $B$, hoặc $C$”, hoặc “$B$ kéo theo $C$”). Điều kiện (d) có nghĩa là nếu $B$ là một mệnh đề và $x$ là một chữ cái, thì $\tau_x(B)$ là một đối tượng. Hãy xét mệnh đề $B$ như biểu thị một tính chất của đối tượng $X$; khi đó, nếu tồn tại một đối tượng có tính chất đang xét, $\tau_x(B)$ biểu diễn một đối tượng được phân biệt có tính chất này; nếu không, $\tau_x(B)$ biểu diễn một đối tượng mà về nó không thể nói gì cả. Cuối cùng, điều kiện (e) có nghĩa là nếu $A_1,A_2,\ldots,A_n$ là các đối tượng, và nếu $s$ là một dấu quan hệ (tương ứng dấu thực thể) có trọng số $n$, thì $sA_1A_2\ldots A_n$ là một mệnh đề về các đối tượng $A_1,\ldots,A_n$ (tương ứng một đối tượng phụ thuộc vào $A_1,\ldots,A_n$).

*Ví dụ.* Các ký hiệu $\varnothing$, $\mathbf{N}$, “đường thẳng thực”, “hàm $\Gamma$”, $f\circ g$ biểu diễn các số hạng. Các ký hiệu $\pi=\sqrt{2}+\sqrt{3}$, $1\in2$, “mọi vành chia hữu hạn là một trường”, “các không điểm của $\zeta(s)$ khác với $-2$, $-4$, $-6$, ... nằm trên đường $\mathfrak{R}(s)=1/2$” biểu diễn các quan hệ. Ký hiệu “3 và 4” không biểu diễn một số hạng cũng không biểu diễn một quan hệ.

Dấu ban đầu của một quan hệ là $\vee$, $\neg$, hoặc một dấu quan hệ. Dấu ban đầu của một số hạng là $\tau$ hoặc một dấu thực thể, với điều kiện là số hạng đó không gồm một chữ cái duy nhất. Mệnh đề sau được suy ra từ sự kiện rằng một số hạng là một dãy ký hiệu thuộc loài thứ nhất. Nếu $A$ là một quan hệ, thì $A$ xuất hiện trong một phép dựng kiến tạo, không phải là một chữ cái, và không bắt đầu bằng $\tau$, do đó có ba trường hợp có thể xảy ra : (1) $A$ đứng sau một dãy ký hiệu $B$ sao cho $A$ là $\neg B$; (2) $A$ đứng sau hai dãy ký hiệu $B$ và $C$ sao cho $A$ là $\vee BC$; (3) $A$ đứng sau các dãy ký hiệu $A_1$, $A_2$, ... $A_n$ sao cho $A$ là $sA_1A_2 ... A_n$, $s$ là một dấu quan hệ.

### 4. CÁC TIÊU CHUẨN KIẾN TẠO

CF1. Nếu $A$ và $B$ là các quan hệ trong một lý thuyết $\mathscr{T}$, thì $\vee AB$ là một quan hệ trong $\mathscr{T}$.

Xét hai phép dựng kiến tạo (trong $\mathscr{T}$), một trong hai phép dựng đó chứa $A$ và phép kia chứa $B$. Xét dãy các dãy ký hiệu thu được bằng cách viết trước hết các dãy ký hiệu của phép dựng thứ nhất, sau đó các dãy ký hiệu của phép dựng thứ hai, và cuối cùng $\vee AB$. Vì $A$ và $B$ thuộc loài thứ hai, nên ngay lập tức kiểm tra được rằng dãy này là một phép dựng kiến tạo của $\mathscr{T}$. Dãy ký hiệu $\vee AB$ thuộc loài thứ hai, do đó nó là một quan hệ trong $\mathscr{T}$.

Ba tiêu chuẩn sau đây được thiết lập tương tự :

CF2. Nếu $A$ là một quan hệ trong một lý thuyết $\mathscr{T}$, thì $\neg A$ là một quan hệ trong $\mathscr{T}$.

CF3. Nếu $A$ là một quan hệ trong một lý thuyết $\mathscr{T}$, và nếu $x$ là một chữ cái, thì $\tau_x(A)$ là một số hạng trong $\mathscr{T}$.

CF4. Nếu $A_1$, $A_2$, ..., $A_n$ là các số hạng trong một lý thuyết $\mathscr{T}$, và nếu $s$ là một dấu quan hệ (tương ứng là dấu thực thể) có trọng số $n$ trong $\mathscr{T}$, thì $sA_1A_2...A_n$ là một quan hệ (tương ứng là một số hạng) trong $\mathscr{T}$.

Các tiêu chuẩn này ngay lập tức suy ra điều sau :

CF5. Nếu $A$ và $B$ là các quan hệ trong một lý thuyết $\mathscr{T}$, thì $\Longrightarrow AB$ là một quan hệ trong $\mathscr{T}$.

CF6. Cho $A_1$, $A_2$, ..., $A_n$ là một phép dựng kiến tạo trong một lý thuyết $\mathscr{T}$, và cho $x$ và $y$ là các chữ cái. Giả sử rằng $y$ không xuất hiện trong bất kỳ $A_i$ nào. Khi đó $(y|x) A_1$, $(y|x) A_2$, ..., $(y|x) A_n$ là một phép dựng kiến tạo trong $\mathscr{T}$.

Để chứng minh CF6, đặt $A_i'$ là phép dựng $(y|x)A_i$. Nếu $A_i$ là một chữ cái, thì $A_i'$ là một chữ cái. Nếu $A_i$ có dạng $\neg A_j$, trong đó $A_j$ là một phép dựng thuộc loài thứ hai đứng trước $A_i$ trong phép dựng, thì $A_i'$ đồng nhất với $\neg A_j'$ theo CS5, và $A_j'$ là một phép dựng thuộc loài thứ hai. Lập luận cũng tương tự nếu $A_i$ có dạng $\vee A_jA_k$ hoặc $sA_{j_1}A_{j_2}\ldots A_{j_m}$, $s$ là một dấu hiệu cụ thể của $\mathscr{T}$. Cuối cùng, nếu $A_i$ có dạng $\tau_z(A_j)$, trong đó $A_j$ là một phép dựng thuộc loài thứ hai đứng trước $A_i$ trong phép dựng, thì có nhiều trường hợp cần xét:

(a) $z$ là một chữ cái phân biệt với $x$ và $y$. Khi đó $A_i'$ đồng nhất với $\tau_z(A_j')$ theo CS4, và $A_j'$ là một hợp thành của loài thứ hai.

(b) $z$ trùng với $x$. Khi đó $A_i$ không chứa $x$, do đó $A_i'$ trùng với $A_i$, nghĩa là với $\tau_x(A_j)$; vì $y$ không xuất hiện trong $A_j$, $\tau_x(A_j)$ trùng với $\tau_y(A_j)$ theo CS3.

(c) $z$ đồng nhất với $y$. Khi đó $A_i$ là phép lắp ghép $\tau A_j$, vì $y$ không xuất hiện trong $A_j$; do đó $A_i'$ là phép lắp ghép $\tau A_j'$, tức là $\tau_u(A_j')$, trong đó $u$ là một chữ cái không xuất hiện trong $A_j'$.

CF7. *Cho $A$ là một quan hệ (tương ứng một số hạng) trong một lý thuyết $\mathscr{T}$, và cho $x$ và $y$ là các chữ cái. Khi đó $(y|x)A$ là một quan hệ (tương ứng một số hạng) trong $\mathscr{T}$.*

Cho $A_1,A_2,\ldots,A_n$ là một phép dựng kiến tạo trong đó $A$ xuất hiện. Ta sẽ chứng minh từng bước rằng, nếu $A_i$ là một quan hệ (tương ứng là một số hạng) thì $(y|x)A_i$, mà ta sẽ ký hiệu là $A_i'$, cũng là một quan hệ (tương ứng là một số hạng). Giả sử rằng điểm này đã được thiết lập đối với $A_1,A_2,\ldots,A_{i-1}$; hãy chứng minh nó đối với $A_i$. Nếu $A_i$ là một chữ cái, thì $A_i'$ là một chữ cái. Nếu $A_i$ đứng trước trong phép dựng bởi một quan hệ $A_j$ sao cho $A_i$ là $\neg A_j$, thì $A_i'$ đồng nhất với $\neg A_j'$ theo CS5, và $\neg A_j'$ là một quan hệ theo CF2. Lập luận tương tự nếu $A_i$ đứng trước bởi các quan hệ $A_j,A_k$ sao cho $A_i$ là $\vee A_jA_k$, hoặc nếu $A_i$ đứng trước bởi các số hạng $A_{j_1},\ldots,A_{j_m}$ sao cho $A_i$ là $sA_{j_1}\cdots A_{j_m}$, trong đó $s$ là một dấu hiệu riêng của $\mathscr{T}$ có trọng số $m$. Cuối cùng, nếu $A_i$ đứng trước bởi một quan hệ $A_j$ sao cho $A_i$ là $\tau_z(A_j)$, có nhiều trường hợp khác nhau cần xét:

(a) $z$ phân biệt với cả $x$ và $y$. Khi đó $A_i'$ trùng với $\tau_z(A_j')$ theo CS4, và ta đã biết rằng $A_j'$ là một quan hệ; do đó $A_i$ là một số hạng, theo CF3.

(b) $z$ trùng với $x$. Khi đó $A_i$ không chứa $x$, do đó $A_i'$ trùng với $A_i$, và vì thế là một số hạng.

(c) $z$ đồng nhất với $y$. Khi đó cho $u$ là một chữ cái, phân biệt với cả $x$ và $y$, không xuất hiện trong $A_1,A_2,\ldots,A_j$. Theo CF6, dãy ký hiệu $(u|y)A_1,\ldots,(u|y)A_j$, mà ta sẽ ký hiệu bởi $A_1'',\ldots,A_j''$, tạo thành một phép dựng kiến tạo trong $\mathscr{T}$. Vì $y$ không còn xuất hiện trong phép dựng mới này, $(y|x)A_1'',\ldots,(y|x)A_j''$ là một phép dựng kiến tạo theo CF6, do đó $(y|x)A_j''$ là một quan hệ trong $\mathscr{T}$; do đó $\tau_u((y|x)A_j'')$ là một số hạng của $\mathscr{T}$. Nhưng số hạng này đồng nhất với $(y|x)\tau_u(A_j'')$ theo CS4, do đó với $(y|x)\tau_y(A_j)$ theo CS3, do đó đồng nhất với $A_i$.

CF8. Cho $A$ là một quan hệ (tương ứng là một số hạng) trong một lý thuyết $\mathscr{T}$, cho $x$ là một chữ cái và $T$ là một số hạng trong $\mathscr{T}$. Khi đó $(T|x)A$ là một quan hệ (tương ứng là một số hạng) trong $\mathscr{T}$.

Cho $A_1, A_2, \ldots, A_n$ là một phép dựng kiến tạo trong đó $A$ xuất hiện. Cho $x_1, x_2, \ldots, x_p$ là các chữ cái phân biệt xuất hiện trong $T$. Gắn với mỗi chữ cái $x_i$ một chữ cái $x_i'$, phân biệt với mỗi chữ cái trong các chữ cái $x_1, \ldots, x_p$ và các chữ cái xuất hiện trong $A_1, \ldots, A_n$, sao cho các chữ cái $x_1', \ldots, x_p'$ đều phân biệt. Phép ghép

$$
(x_1'|x_1)(x_2'|x_2)\ldots(x_p'|x_p)T
$$

là một số hạng $T'$ theo CF7, và $(T|x)A$ đồng nhất với

$$
(x_1|x_1')(x_2|x_2')\ldots(x_p|x_p')(T'|x)A
$$

do áp dụng CS1. Do đó chỉ cần chứng minh rằng $(T'|x)\,A$ là một quan hệ (tương ứng là một số hạng); nói cách khác, từ nay ta có thể giả sử rằng các chữ cái xuất hiện trong $T$ không xuất hiện trong $A_1, \ldots, A_n$.

¶ Chúng ta sẽ chứng minh từng bước rằng, nếu $A_t$ là một quan hệ (tương ứng là một số hạng), thì $(T|x)\,A_t$, mà ta sẽ ký hiệu là $A_t'$, là một quan hệ (tương ứng là một số hạng). Giả sử điểm này đã được thiết lập đối với $A_1,A_2,\ldots,A_{i-1}$, và ta hãy chứng minh nó đối với $A_i$. Nếu $A_i$ là một chữ cái, thì $A_i'$ hoặc là cùng một chữ cái hoặc là $T$, và do đó là một số hạng. Nếu $A_i$ có dạng $\neg A_j$, trong đó $A_j$ là một quan hệ đứng trước $A_i$ trong phép dựng, thì $A_i$ đồng nhất với $\neg A_j'$ theo CS5, và ta đã biết rằng $A_j'$ là một quan hệ, do đó $A_i'$ là một quan hệ theo CF2. Chứng minh là tương tự nếu $A_i$ có dạng $\vee A_jA_k$, hoặc $sA_{j_1}\ldots A_{j_m}$. Cuối cùng, nếu $A_i$ có dạng $\tau_z(A_j)$, trong đó $A_j$ là một quan hệ đứng trước $A_i$ trong phép dựng, thì có nhiều trường hợp cần được xét:

(a) $z$ phân biệt với $x$ và với các chữ cái xuất hiện trong $T$. Khi đó $A_i'$ đồng nhất với $\tau_z(A_j')$ theo CS4, và ta đã biết rằng $A_j'$ là một quan hệ; do đó $A_i'$ là một số hạng theo CF3.

(b) $z$ đồng nhất với $x$. Khi đó $A_i$ không chứa $x$, do đó $A_i'$ đồng nhất với $A_i$ và vì thế là một số hạng.

(c) $z$ xuất hiện trong $T$. Khi đó $z$ không xuất hiện trong $A_j$, do đó $A_i'$ đồng nhất với $\tau A_j'$; suy ra $A_i'$ đồng nhất với $\tau A_j'$. Bây giờ, ta đã biết rằng $A_j'$ là một quan hệ, và $\tau A_j'$ đồng nhất với $\tau_u(A_j)$, trong đó $u$ là một chữ cái không xuất hiện trong $A_j$; từ CF3 suy ra rằng $A_i'$ là một số hạng.

Về mặt trực giác, nếu $A$ là một quan hệ trong $\mathscr{T}$, mà ta có thể xem như biểu diễn một tính chất của một đối tượng $x$, thì mệnh đề $(B|x)\,A$ tương đương với việc nói rằng đối tượng $B$ có tính chất này. Nếu $A$ là một số hạng trong $\mathscr{T}$, nó biểu diễn một đối tượng phụ thuộc theo một cách nào đó vào đối tượng được ký hiệu bởi $x$; số hạng $(B|x)\,A$ biểu diễn cái mà đối tượng $A$ trở thành khi ta lấy $x$ là đối tượng $B$.

### Bài tập {#ens-i-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).

[^1]: Ý nghĩa của biểu thức này sẽ trở nên rõ ràng khi chương này tiến triển.
[^2]: Để biết các ý nghĩa trực giác của các dấu này, xem no. 3, Nhận xét.
[^3]: Phù hợp với điều đã nói ở no. 1, cụm từ “$x$ và $y$ là các chữ cái phân biệt” là một lối nói không chuẩn: nó có nghĩa là $x$ và $y$ biểu thị các chữ cái phân biệt trong các dãy ký hiệu đang xét.

[^4]: Như đã nói ở trên, đối với sự phát triển của các lý thuyết toán học hiện nay, có thể hạn chế sự khảo sát của chúng ta vào các ký hiệu cụ thể có trọng số 2, và do đó tránh dùng biểu thức “số tự nhiên $n$” trong định nghĩa của một phép dựng kiến tạo.
