---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 0
section_title: Characterization of terms and relations
appendix: true
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 50-55, 60-64
pdf_pages: 0057-0062, 0067-0071
extraction: ocr
subsections:
    - "no": 1
      title: SIGNS AND WORDS
      page: 50
      pdf_page: 57
    - "no": 2
      title: SIGNIFICANT WORDS
      page: 51
      pdf_page: 58
    - "no": 3
      title: CHARACTERIZATION OF SIGNIFICANT WORDS
      page: 51
      pdf_page: 58
    - "no": 4
      title: APPLICATION TO ASSEMBLIES IN A MATHEMATICAL THEORY
      page: 53
      pdf_page: 60
statements: 7
exercises: 8
content_sha256: 80a61228b43b59ad6e44b716b5c6f20e1315b70f2ee869a7f4dca74cc009dda8
translated_from: content/en/ens/I/A_a_characterization_of_terms_and_relations.md
source_content_sha256: 13db39e88a8780043e156517521974c8c14af043efeaa643d5625514ba9d1ea2
translation_model: gpt-5-6, gpt-5-6-mini, copied, gpt-5-mini
translation_run: translate-vi-057020d5
glossary_version: 34
glossary_terms_sha256: 73843910f6f96e463c8550efc75b8743d0fda32fa7e203813bf523f221e24e83
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# ĐẶC TRƯNG HÓA CÁC THUẬT NGỮ VÀ QUAN HỆ

Siêu toán học, khi vượt ra ngoài mức độ hết sức sơ đẳng của chương hiện tại, sử dụng đáng kể các kết quả của toán học, như chúng tôi đã nhận xét trong Phần mở đầu. Mục đích của Phụ lục này là đưa ra một ví dụ đơn giản về kiểu lập luận này [^1]. Trước hết, chúng ta sẽ thiết lập một số kết quả thuộc về lý thuyết toán học của các *nửa nhóm tự do*; sau đó chúng ta sẽ sử dụng các kết quả này trong một "ứng dụng" siêu toán học để thu được một đặc trưng hóa các thuật ngữ và quan hệ trong một lý thuyết.

### 1. CÁC DẤU VÀ CÁC TỪ

\* Cho S là một tập hợp không rỗng, các phần tử của nó sẽ được gọi là *dấu* (thuật ngữ này thích hợp với ứng dụng siêu toán học mà ta đang xét). Cho $\mathrm{L}_0(\mathrm{S})$ là nửa nhóm tự do sinh bởi S; các phần tử của $\mathrm{L}_0(\mathrm{S})$ được gọi là *từ* và được đồng nhất với các dãy hữu hạn $A = (s_i)_{0 \leqslant i \leqslant n}$ gồm các phần tử của S. Luật hợp thành trong $\mathrm{L}_0(\mathrm{S})$ sẽ được viết theo phép nhân, sao cho $AB$ là dãy thu được bằng cách ghép nối $A$ và $B$. Từ rỗng $\emptyset$ là phần tử đơn vị của $\mathrm{L}_0(\mathrm{S})$. Ta nhắc lại rằng *độ dài* $l(A)$ của một từ $A \in \mathrm{L}_0(\mathrm{S})$ là số các phần tử trong dãy $A$; do đó $l(AB) = l(A) + l(B)$, và các từ có độ dài 1 là các dấu. Ký hiệu $\mathrm{L}(\mathrm{S})$ là tập hợp các từ không rỗng trong $\mathrm{L}_0(\mathrm{S})$.
¶ Giả sử thêm rằng ta được cho một ánh xạ $s \rightarrow n(s)$ từ S vào tập hợp $\mathbf{N}$ các số nguyên $\geqslant 0$. Với mỗi từ không rỗng $A = (s_i)_{0 \leqslant i \leqslant k}$ của L(S), ta đặt

$$n(A) \;=\; \sum_{i=0}^{k} \, n(s_i)$$

và $n(\emptyset) = 0$. $n(A)$ được gọi là *trọng số* của $A$. Rõ ràng $n(AB) = n(A) + n(B)$. ¶ Nếu $A = A'BA''$, từ $B$ được gọi là một *đoạn* của $A$ (một đoạn *thực sự* nếu thêm nữa $B \neq A$). Nếu $A'$ (resp. $A''$) rỗng, $B$ được gọi là một đoạn *ban đầu* (resp. *cuối cùng*) của $A$. Nếu $l(A') = k$, thì $B$ được gọi là *bắt đầu tại vị trí thứ $(k+1)$*.

¶ Nếu $A = BCDEF$ (trong đó các từ $B$, $C$, $D$, $E$, $F$ có thể rỗng) thì các đoạn $C$ và $E$ của $A$ được gọi là *rời nhau*.

### 2. CÁC TỪ CÓ Ý NGHĨA

Một *dãy có nghĩa* là một dãy bất kỳ $(A_j)_{1 \leqslant j \leqslant n}$ các từ của $\mathrm{L}_0(\mathrm{S})$ có tính chất sau đây: với mỗi từ $A_i$ của dãy, một trong hai điều kiện sau được thỏa mãn:

(1) $A_i$ là một dấu có trọng số 0.

(2) Có $p$ từ $A_{i_1}$, $A_{i_2}$, ..., $A_{i_p}$ trong dãy, với các chỉ số nhỏ hơn $i$, và một dấu $f$ có trọng số $p$ sao cho

$$A_i = f\, A_{i_1} A_{i_2} \, \ldots \, A_{i_p}.$$

Các từ xuất hiện trong các dãy có nghĩa được gọi là *các từ có nghĩa*. Khi đó ta có:

#### Mệnh đề 1 {#ens-i-a0-prop-1 .statement tag=03P6}

*Nếu $A_1$, $A_2$, ..., $A_p$ là $p$ từ có nghĩa và $f$ là một dấu có trọng số $p$, thì từ $f A_1 A_2 \ldots A_p$ là có nghĩa.*

### 3. ĐẶC TRƯNG HÓA CÁC TỪ CÓ NGHĨA

Một từ $A \in \mathrm{L}_0(\mathrm{S})$ được gọi là *cân bằng* nếu nó có hai tính chất sau:

(1) $l(A) = n(A) + 1$ (điều này suy ra rằng $A$ không rỗng).

(2) Với mọi đoạn đầu thực sự $B$ của $A$, $l(B) \leqslant n(B)$.

#### Mệnh đề 2 {#ens-i-a0-prop-2 .statement tag=03P7}

*Một từ là có ý nghĩa khi và chỉ khi nó cân bằng.*

Cho $A$ là một từ có ý nghĩa thuộc một dãy có ý nghĩa

$$A_1, \; A_2, \; \ldots, \; A_n.$$

Chúng ta sẽ chứng minh bằng quy nạp theo $k$ rằng mỗi $A_k$ đều cân bằng. Giả sử điều này đã được thiết lập đối với các $A_j$ với chỉ số $j < k$, và hãy chứng minh rằng điều đó đúng với $A_k$. Nếu $A_k$ là một dấu có trọng số 0 (điều này là khả năng duy nhất khi $k = 1$), thì $A_k$ cân bằng vì

$$l(A_k) = 1 \qquad \text{và} \qquad n(A_k) = 0.$$

Nếu $A_k$ không phải là một dấu có trọng số 0, thì $A_k = fB_1B_2 \ldots B_p$, trong đó $f$ là một dấu có trọng số $p$, và các $B_j$ có dạng $A_{i_j}$, với $i_j < k$, do đó là các từ cân bằng theo giả thiết quy nạp. Ta có

$$\begin{aligned} l(A_k) &= 1 + l(B_1) + l(B_2) + \cdots + l(B_p) \\ &= 1 + (n(B_1) + 1) + (n(B_2) + 1) + \cdots + (n(B_p) + 1) \\ &= 1 + p + n(B_1) + n(B_2) + \cdots + n(B_p) \\ &= 1 + n(A_k). \end{aligned}$$

Cho $C$ là một đoạn đầu thực sự của $A$, và cho $q$ là lớn nhất trong các số nguyên $m < p$ sao cho $B_m$ là một đoạn của $C$, sao cho

$$C = f B_1 B_2 \ldots B_q D,$$

trong đó $D$ là một đoạn đầu thực sự của $B_{q+1}$. Khi đó

$$\begin{aligned} l(C) &= 1 + l(B_1) + l(B_2) + \cdots + l(B_q) + l(D) \\ &\leqslant 1 + (n(B_1) + 1) + (n(B_2) + 1) + \cdots + (n(B_q) + 1) + n(D) \\ &\leqslant p + n(B_1) + \cdots + n(B_q) + n(D) = n(C). \end{aligned}$$

Suy ra $A_k$ là cân bằng.

¶ Để chứng minh rằng, ngược lại, mọi từ cân bằng đều có ý nghĩa, ta cần hai bổ đề sau :

#### Bổ đề 1 {#ens-i-a0-lem-1 .statement tag=03P8}

*Một từ A là cân bằng. Khi đó với mỗi số nguyên k sao cho $0 \leqslant k < l(A)$ tồn tại duy nhất một đoạn cân bằng S của A bắt đầu tại vị trí thứ $(k + 1)$.*

Tính duy nhất của $S$ là một hệ quả ngay lập tức của nhận xét sau: nếu $T$ là một từ cân bằng, thì theo định nghĩa không có đoạn đầu thực sự nào của $T$ là cân bằng. Hãy chứng minh sự tồn tại của $S$. Viết $A = BC$ trong đó $l(B) = k$. Với mỗi $i$ sao cho $0 \leqslant i \leqslant q = l(C)$, gọi $C_i$ là đoạn đầu của $C$ có độ dài $i$. Vì $B$ là một đoạn đầu thực sự của $A$, ta có

$$l(C_q) = l(A) - l(B) \geqslant n(A) + 1 - n(B) = n(C_q) + 1.$$

Mặt khác, ta có $0 = l(C_0) \leqslant n(C_0) = 0$. Gọi $i$ là số lớn nhất trong các số nguyên $j < q$ sao cho $l(C_h) \leqslant n(C_h)$ với $0 \leqslant h \leqslant j$; khi đó ta có $l(C_i)\leq n(C_i)$ và $l(C_{i+1})\geq n(C_{i+1})+1$. Ta chứng minh rằng $C_{i+1}$ là cân bằng: điều kiện liên quan đến các đoạn ban đầu thực sự được thỏa mãn do định nghĩa của $i$; mặt khác, ta có

$$
n(C_{i+1})+1\leq l(C_{i+1})=l(C_i)+1\leq n(C_i)+1\leq n(C_{i+1})+1,
$$

suy ra $l(C_{i+1})=n(C_{i+1})+1$, và chứng minh của Bổ đề 1 hoàn tất.

#### Bổ đề 2 {#ens-i-a0-lem-2 .statement tag=03GT}

Mọi từ cân bằng $A$ có thể được viết dưới dạng

$$
A=fA_1A_2\ldots A_p,
$$

trong đó các $A_i$ là cân bằng và $n(f)=p$.

Cho $f$ là dấu ban đầu của $A$. Theo Bổ đề 1, $A$ có thể được viết thành

$$
fA_1A_2\ldots A_p,
$$

trong đó các $A_i$ là cân bằng : ta chỉ cần định nghĩa $A_i$ bằng quy nạp là đoạn cân bằng của $A$ bắt đầu tại vị trí thứ $k(i)$, trong đó

$$
k(i)=2+\sum_{j<i}l(A_j).
$$

Hơn nữa, ta có

$$
1+l(A_1)+\ldots+l(A_p)=l(A)=n(A)+1
$$
$$
=n(f)+n(A_1)+\ldots+n(A_p)+1
$$
$$
=n(f)+(l(A_1)-1)+\ldots+(l(A_p)-1)+1,
$$

từ đó suy ra rằng $n(f)=p$.

¶ Bây giờ hai bổ đề đã được chứng minh, hiển nhiên bằng quy nạp theo độ dài của $A$ rằng mọi từ cân bằng $A$ đều có ý nghĩa, nhờ Bổ đề 2 và Mệnh đề 1.

#### Hệ quả 1 {#ens-i-a0-lem-2-cor-1 .statement tag=03GU}

Cho $A$ là một từ có ý nghĩa. Với mỗi số nguyên $k$ sao cho $0\leq k<l(A)$ có đúng một đoạn có ý nghĩa của $A$ bắt đầu ở vị trí thứ $(k+1)$.

#### Hệ quả 2 {#ens-i-a0-lem-2-cor-2 .statement tag=03GV}

Mọi từ có ý nghĩa đều có thể được viết theo đúng một cách dưới dạng $fA_1A_2\ldots A_p$, trong đó các $A_i$ là có ý nghĩa và $n(f)=p.$*

### 4. ỨNG DỤNG VÀO CÁC DÃY KÝ HIỆU TRONG MỘT LÝ THUYẾT TOÁN HỌC

Giả sử rằng tập hợp S là tập hợp các dấu của một lý thuyết toán học $\mathscr{T}$. Ta đặt $n(\square)=0$, $n(\tau)=n(\eta)=1$, $n(\vee)=2$, $n(x)=0$ với mọi chữ cái $x$;

và cuối cùng, đối với mỗi ký hiệu cụ thể $s$ của $\mathscr{T}$, $n(s)$ là trọng số của $s$, được cố định khi $\mathscr{T}$ được cho.

¶ Cho $A$ là một cấu tạo trong $\mathscr{T}$. Ta ký hiệu $A^*$ là từ thu được bằng cách xóa các liên kết trong $A$, và ta sẽ nói rằng $A$ là *cân bằng* nếu $A^*$ là cân bằng [trong $L_0(S)$]. Một *đoạn* của $A$ là mọi cấu tạo thu được bằng cách thay thế, trong một đoạn $S$ của $A^*$, các liên kết mà, trong $A$, nối các cặp dấu của $S$.

**TIÊU CHÍ 1.** *Nếu $A$ là một số hạng hoặc một quan hệ trong $\mathscr{T}$, thì $A$ là cân bằng.*

Cho $A_1$, $A_2$, $\ldots$, $A_n$ là một phép dựng kiến tạo trong $\mathscr{T}$, trong đó $A$ xuất hiện. Ta lập luận bằng quy nạp và giả sử rằng đã chứng minh được các $A_j$ có chỉ số $j<i$ là cân bằng; khi đó ta phải chứng minh rằng $A_i$ là cân bằng. Chứng minh tiến hành đúng như trong phần đầu của chứng minh Mệnh đề 2, ngoại trừ khi $A_i$ có dạng $\tau_x(B)$ với $B=A_j$ và $j<i$. Trong trường hợp này, gọi $C$ là tập hợp thu được bằng cách thay thế $x$, tại mọi nơi nó xuất hiện trong $B$, bởi $\square$. Khi đó từ $A^*$ đồng nhất với $\tau C^*$; bây giờ $B^*$ là cân bằng, và do đó $C^*$ là cân bằng (vì $n(\square)=n(x)=0$). Do đó $A_i^*$ là cân bằng.

¶ Như vậy ta đã thu được một điều kiện cần để một dãy ký hiệu trong $\mathscr{T}$ là một số hạng hoặc một quan hệ. Nhưng điều kiện này không đủ, như ta sẽ thấy.

¶ Cho $A$ là một dãy ký hiệu cân bằng trong $\mathscr{T}$. Nếu $A$ bắt đầu bằng một chữ cái hoặc một $\square$, thì $A$ phải chỉ gồm riêng ký hiệu này (Mệnh đề 2, Hệ quả 2). Trong tất cả các trường hợp khác, ta sẽ định nghĩa dãy ký hiệu hoặc các dãy ký hiệu *đứng trước* $A$.

(1) Nếu $A$ bắt đầu bằng một $\land$, hoặc một $\vee$, hoặc một dấu hiệu cụ thể, thì $A^*$ có thể được viết theo đúng một cách dưới dạng $fB_1B_2\ldots B_p$, trong đó $f$ là một dấu hiệu có trọng số $p\geq 1$ và các $B_i$ là cân bằng (Mệnh đề 2, Hệ quả 2). Các đoạn $A_1$, $A_2$, $\ldots$, $A_p$ của $A$ tương ứng với các đoạn $B_1$, $B_2$, $\ldots$, $B_p$ của $A^*$ được gọi là các dãy ký hiệu *tiên nghiệm* đối với $A$. Hơn nữa, ta sẽ nói rằng $A$ là *cân bằng hoàn toàn* nếu $A$ đồng nhất với

$$
fA_1A_2\ldots A_p,
$$

nói cách khác nếu không có một liên kết nào trong $A$ nối $f$ với một trong các $B_i$, hoặc nối hai $B_i$ phân biệt.

(2) Nếu $A$ bắt đầu bằng một $\tau$, thì $A^*$ có dạng $\tau B$, trong đó $B$ là cân bằng (Mệnh đề 2, Hệ quả 2). Trong trường hợp này, một dãy ký hiệu tiền thân của $A$ là bất kỳ dãy ký hiệu nào trong các dãy ký hiệu $A_1$ được xác định như sau : thay thế các dấu $\square$ trong $B$ mà trong $A$ được nối với $\tau$ ban đầu bằng một chữ cái $x$ phân biệt với các chữ cái khác xuất hiện trong $B$, và thay thế các liên kết nối hai dấu của $B$ trong $A$. (Nếu, thay vì $x$, ta thay bằng một chữ cái $y$ cũng không xuất hiện trong $B$, ta thu được một dãy ký hiệu đúng bằng $(y|x)A_1$.) Hơn nữa, ta sẽ nói rằng $A$ là *cân bằng hoàn toàn* nếu $A$ đồng nhất với $\tau_x(A_1)$, nói cách khác nếu không có liên kết nào nối $\tau$ ban đầu với một dấu nào của $B$ khác với một $\square$.

¶ Ta có thể phát biểu tiêu chuẩn sau đây :

C2. *Cho $A$ là một dãy ký hiệu cân bằng trong $\mathscr{T}$.*

¶ *Để $A$ là một số hạng, điều kiện cần và đủ là một trong các điều kiện sau được thỏa mãn : (1) $A$ gồm một chữ cái duy nhất; (2) $A$ bắt đầu bằng một $\tau$, cân bằng hoàn toàn, và các dãy ký hiệu đứng trước của nó là các quan hệ* (theo CF8, chỉ cần kiểm tra rằng *một* dãy ký hiệu đứng trước là một quan hệ); *(3) $A$ bắt đầu bằng một dấu thực thể hóa, cân bằng hoàn toàn, và các dãy ký hiệu đứng trước của nó là các số hạng.* ¶ *Để $A$ là một quan hệ, điều kiện cần và đủ là một trong các điều kiện sau được thỏa mãn : (1) $A$ bắt đầu bằng một $\vee$ hoặc một $\neg$, cân bằng hoàn toàn, và các dãy ký hiệu đứng trước của nó là các quan hệ; (2) $A$ bắt đầu bằng một dấu quan hệ, cân bằng hoàn toàn, và các dãy ký hiệu đứng trước của nó là các số hạng.*

Các tiêu chuẩn CF1 đến CF4 (§ 1, no. 4) cho thấy các điều kiện là đủ. Ta hãy chứng minh rằng chúng là cần. Ta đã thấy (§ 1, no. 3) rằng nếu $A$ là một quan hệ, thì $A$ bắt đầu bằng một $\vee$, hoặc một $\neg$, hoặc một dấu quan hệ. Lập luận là tương tự trong cả ba trường hợp. Chẳng hạn, nếu $A$ bắt đầu bằng một $\vee$, thì $A$ có dạng $\vee BC$, trong đó $B$ và $C$ là các quan hệ, do đó $B$ và $C$ là các dãy ký hiệu tiền nhiệm của $A$; vậy $A$ hoàn toàn cân bằng. Nếu $A$ là một số hạng, thì có hai trường hợp: nó gồm một chữ cái duy nhất, hoặc nó bắt đầu bằng một dấu định chất hoặc một $\tau$. Trong trường hợp thứ hai, ta lập luận như trên. Nếu $A$ bắt đầu bằng một $\tau$, định nghĩa của một phép dựng kiến tạo cho thấy rằng $A$ có dạng $\tau_x(B)$, trong đó $B$ là một quan hệ và $x$ là một chữ cái, do đó ta có thể lấy $B$ làm dãy ký hiệu tiền nhiệm của $A$, và $A$ hoàn toàn cân bằng.

Khi muốn kiểm tra xem một dãy ký hiệu $A$ (không gồm một chữ cái duy nhất) có phải là một quan hệ (resp. một số hạng) trong $\mathscr{T}$ hay không, trước hết ta kiểm tra rằng $A$ là cân bằng và bắt đầu bằng một $\vee$, một $\neg$, hoặc một dấu quan hệ (resp. bằng một $\tau$ hoặc một dấu chỉ định bản thể). Sau đó ta lập dãy ký hiệu tiền đề hoặc các dãy ký hiệu tiền đề, và kiểm tra (nếu thích hợp) rằng $A$ hoàn toàn cân bằng. Làm xong việc này, ta còn lại một bài toán tương tự liên quan đến các dãy ký hiệu ngắn hơn. Như vậy, từng bước một, ta đi xuống đến các dãy ký hiệu mà mỗi dãy đều gồm một dấu duy nhất, và đối với chúng thì nghiệm là ngay lập tức.

#### Nhận xét {#ens-i-a0-n4-rem-1 .statement tag=03GW}

Ngoại trừ trong một số lý thuyết toán học đặc biệt yếu về các tiên đề (xem Bài tập 7), ta không có một thủ tục tổng quát nào thuộc loại này cho phép kiểm tra xem một quan hệ $R$ đã cho trong một lý thuyết $\mathscr{T}$ có phải là một định lý trong $\mathscr{T}$ hay không.

### Bài tập {#ens-i-a0-exercises}

Xem [các bài tập cho Phụ lục 0](exercises/a0/).

[^1]: Các kết quả được thiết lập trong Phụ lục này sẽ không được sử dụng ở bất kỳ nơi nào khác trong chuỗi này.
