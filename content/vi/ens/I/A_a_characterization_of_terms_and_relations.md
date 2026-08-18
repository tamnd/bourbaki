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
content_sha256: ada19ded1745a7e4ea2f7bbf0edb698ecd7e5df3f973986c589436fed914ee9d
translated_from: content/en/ens/I/A_a_characterization_of_terms_and_relations.md
source_content_sha256: edb021fd8f3949693679ebb01f91bf25e20ec7a14a764b2755ff6b36f5e23268
translation_model: gpt-5.4
translation_run: translate-vi-f2ab4019
glossary_version: 29
glossary_terms_sha256: 0535f53b0f3056e7867a8c2e210b1395db30f6e677c4d3bef1e76f20d917b730
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# ĐẶC TRƯNG HÓA CÁC THUẬT NGỮ VÀ QUAN HỆ

Siêu toán học, khi vượt quá trình độ rất sơ cấp của chương này, sử dụng rất nhiều các kết quả của toán học, như chúng tôi đã nhận xét trong phần Mở đầu. Mục đích của Phụ lục này là cho một ví dụ đơn giản về kiểu lập luận này [^1]. Trước hết chúng tôi sẽ thiết lập một số kết quả thuộc về lý thuyết toán học của các *nửa nhóm tự do*; sau đó chúng tôi sẽ dùng các kết quả ấy trong một " ứng dụng " siêu toán học để thu được một sự đặc trưng hóa các thuật ngữ và quan hệ trong một lý thuyết.

### 1. CÁC DẤU VÀ CÁC TỪ

* Cho S là một tập hợp khác rỗng, mà các phần tử của nó sẽ được gọi là *dấu* (thuật ngữ này là thích hợp với ứng dụng siêu toán học mà ta có trong ý định). Gọi $\mathrm{L}_0(\mathrm{S})$ là nửa nhóm tự do sinh bởi S; các phần tử của $\mathrm{L}_0(\mathrm{S})$ được gọi là *từ* và được đồng nhất với các dãy hữu hạn $A = (s_i)_{0 \leqslant i \leqslant n}$ gồm các phần tử của S. Luật hợp thành trong $\mathrm{L}_0(\mathrm{S})$ sẽ được viết theo lối nhân, sao cho $AB$ là dãy thu được bằng cách ghép liền $A$ và $B$. Từ rỗng $\emptyset$ là phần tử đơn vị của $\mathrm{L}_0(\mathrm{S})$. Nhắc lại rằng *độ dài* $l(A)$ của một từ $A \in \mathrm{L}_0(\mathrm{S})$ là số các phần tử trong dãy $A$; do đó $l(AB) = l(A) + l(B)$, và các từ có độ dài 1 là các dấu. Ký hiệu $\mathrm{L}(\mathrm{S})$ là tập hợp các từ khác rỗng trong $\mathrm{L}_0(\mathrm{S})$.
¶ Hơn nữa, giả sử rằng ta được cho một ánh xạ $s \rightarrow n(s)$ từ S vào

tập hợp $\mathbf{N}$ các số nguyên $\geqslant 0$. Với mỗi từ không rỗng $A = (s_i)_{0 \leqslant i \leqslant k}$ của L(S), ta đặt

$$n(A) \;=\; \sum_{i=0}^{k} \, n(s_i)$$

và $n(\emptyset) = 0$. $n(A)$ được gọi là *trọng số* của $A$. Rõ ràng $n(AB) = n(A) + n(B)$. ¶ Nếu $A = A'BA''$, từ $B$ được gọi là một *đoạn* của $A$ (một đoạn *thực sự* nếu đồng thời $B \neq A$). Nếu $A'$ (tương ứng $A''$) rỗng, thì $B$ được gọi là một đoạn *ban đầu* (tương ứng *cuối*) của $A$. Nếu $l(A') = k$, thì người ta nói rằng $B$ *bắt đầu ở vị trí thứ $(k+1)$*.

¶ Nếu $A = BCDEF$ (trong đó các từ $B$, $C$, $D$, $E$, $F$ có thể rỗng) thì các đoạn $C$ và $E$ của $A$ được gọi là *rời nhau*.

### 2. CÁC TỪ CÓ NGHĨA

Một *dãy đáng kể* là mọi dãy $(A_j)_{1 \leqslant j \leqslant n}$ các từ của $\mathrm{L}_0(\mathrm{S})$ có tính chất sau : với mỗi từ $A_i$ của dãy, một trong hai điều kiện sau được thỏa mãn :

(1) $A_i$ là một dấu có trọng số 0.

(2) Tồn tại $p$ từ $A_{i_1}$, $A_{i_2}$, ..., $A_{i_p}$ trong dãy, với các chỉ số nhỏ hơn $i$, và một ký hiệu $f$ có trọng số $p$ sao cho

$$A_i = f\, A_{i_1} A_{i_2} \, \ldots \, A_{i_p}.$$

Các từ xuất hiện trong các dãy đáng kể được gọi là *các từ có nghĩa*. Khi đó ta có :

#### Mệnh đề 1 {#ens-i-a0-prop-1 .statement tag=03P6}

*Nếu $A_1$, $A_2$, ..., $A_p$ là $p$ từ có nghĩa và nếu $f$ là một ký hiệu có trọng số $p$, thì từ $f A_1 A_2 \ldots A_p$ là có nghĩa.*

### 3. ĐẶC TRƯNG HÓA CÁC TỪ CÓ NGHĨA

Một từ $A \in \mathrm{L}_0(\mathrm{S})$ được gọi là *cân bằng* nếu nó có hai tính chất sau :

(1) $l(A) = n(A) + 1$ (điều này kéo theo rằng $A$ không rỗng).

(2) Với mọi đoạn đầu thực sự $B$ của $A$, $l(B) \leqslant n(B)$.

#### Mệnh đề 2 {#ens-i-a0-prop-2 .statement tag=03P7}

*Một từ là đáng kể khi và chỉ khi nó là cân bằng.*

Cho $A$ là một từ đáng kể thuộc một dãy đáng kể

$$A_1, \; A_2, \; \ldots, \; A_n.$$

Chúng tôi sẽ chứng minh bằng quy nạp theo $k$ rằng mỗi $A_k$ đều cân bằng. Giả sử điều này đã được thiết lập cho các $A_j$ có chỉ số $j < k$, và hãy chứng minh rằng nó đúng với $A_k$. Nếu $A_k$ là một dấu có trọng số 0 (đó là khả năng duy nhất khi $k = 1$), thì $A_k$ là cân bằng vì

$$l(A_k) = 1 \qquad \text{và} \qquad n(A_k) = 0.$$

Nếu $A_k$ không phải là một ký hiệu có trọng số 0, thì $A_k = fB_1B_2 \ldots B_p$, trong đó $f$ là một ký hiệu có trọng số $p$, và các $B_j$ có dạng $A_{i_j}$, với $i_j < k$, và do đó là các từ cân bằng theo giả thiết quy nạp. Ta có

$$\begin{aligned} l(A_k) &= 1 + l(B_1) + l(B_2) + \cdots + l(B_p) \\ &= 1 + (n(B_1) + 1) + (n(B_2) + 1) + \cdots + (n(B_p) + 1) \\ &= 1 + p + n(B_1) + n(B_2) + \cdots + n(B_p) \\ &= 1 + n(A_k). \end{aligned}$$

Cho $C$ là một đoạn đầu ban đầu thực sự của $A$, và gọi $q$ là số nguyên lớn nhất trong các số nguyên $m < p$ sao cho $B_m$ là một đoạn của $C$, sao cho

$$C = f B_1 B_2 \ldots B_q D,$$

trong đó $D$ là một đoạn ban đầu thực sự của $B_{q+1}$. Khi đó

$$\begin{aligned} l(C) &= 1 + l(B_1) + l(B_2) + \cdots + l(B_q) + l(D) \\ &\leqslant 1 + (n(B_1) + 1) + (n(B_2) + 1) + \cdots + (n(B_q) + 1) + n(D) \\ &\leqslant p + n(B_1) + \cdots + n(B_q) + n(D) = n(C). \end{aligned}$$

Do đó $A_k$ là cân bằng.

¶ Để chứng minh rằng, ngược lại, mọi từ cân bằng đều đáng kể, ta cần hai bổ đề sau :

#### Bổ đề 1 {#ens-i-a0-lem-1 .statement tag=03P8}

*Cho A là một từ cân bằng. Khi đó, với mỗi số nguyên k sao cho $0 \leqslant k < l(A)$, tồn tại đúng một đoạn cân bằng S của A bắt đầu ở vị trí thứ $(k + 1)$.*

Tính duy nhất của $S$ là một hệ quả ngay lập tức của chú ý sau đây: nếu $T$ là một từ cân bằng, thì theo định nghĩa không có đoạn đầu thực sự nào của $T$ là cân bằng. Hãy chứng minh sự tồn tại của $S$. Viết $A = BC$ với $l(B) = k$. Với mỗi $i$ sao cho $0 \leqslant i \leqslant q = l(C)$, ký hiệu $C_i$ là đoạn đầu của $C$ có độ dài $i$. Vì $B$ là một đoạn đầu thực sự của $A$, ta có

$$l(C_q) = l(A) - l(B) \geqslant n(A) + 1 - n(B) = n(C_q) + 1.$$

Mặt khác, ta có $0 = l(C_0) \leqslant n(C_0) = 0$. Gọi $i$ là số nguyên lớn nhất trong các số nguyên $j < q$ sao cho $l(C_h) \leqslant n(C_h)$ với $0 \leqslant h \leqslant j$; khi đó

ta có $l(C_i)\leq n(C_i)$ và $l(C_{i+1})\geq n(C_{i+1})+1$. Ta chứng minh rằng $C_{i+1}$ là cân bằng: điều kiện liên hệ với các đoạn ban đầu thực sự được thỏa mãn do lý do là định nghĩa của $i$; mặt khác, ta có

$$
n(C_{i+1})+1\leq l(C_{i+1})=l(C_i)+1\leq n(C_i)+1\leq n(C_{i+1})+1,
$$

do đó $l(C_{i+1})=n(C_{i+1})+1$, và chứng minh của Bổ đề 1 là đầy đủ.

#### Bổ đề 2 {#ens-i-a0-lem-2 .statement tag=03GT}

Mọi từ cân bằng $A$ đều có thể được đặt dưới dạng

$$
A=fA_1A_2\ldots A_p,
$$

trong đó các $A_i$ là cân bằng và $n(f)=p$.

Cho $f$ là dấu ban đầu của $A$. Theo Bổ đề 1, $A$ có thể được viết thành

$$
fA_1A_2\ldots A_p,
$$

trong đó các $A_i$ là cân bằng: chỉ cần định nghĩa $A_i$ bằng quy nạp là đoạn cân bằng của $A$ bắt đầu ở vị trí thứ $k(i)$, trong đó

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

từ đó suy ra $n(f)=p$.

¶ Bây giờ hai bổ đề đã được chứng minh, theo quy nạp trên độ dài của $A$ thì hiển nhiên mọi từ cân bằng $A$ đều đáng kể, do Bổ đề 2 và Mệnh đề 1.

#### Hệ quả 1 {#ens-i-a0-lem-2-cor-1 .statement tag=03GU}

Cho $A$ là một từ đáng kể. Với mỗi số nguyên $k$ sao cho $0\leq k<l(A)$, có đúng một đoạn đáng kể của $A$ bắt đầu ở vị trí thứ $(k+1)$.

#### Hệ quả 2 {#ens-i-a0-lem-2-cor-2 .statement tag=03GV}

Mọi từ đáng kể đều có thể được viết theo đúng một cách dưới dạng $fA_1A_2\ldots A_p$, trong đó các $A_i$ là đáng kể và $n(f)=p.$*

### 4. ÁP DỤNG CHO CÁC DÃY KÝ HIỆU TRONG MỘT LÝ THUYẾT TOÁN HỌC

Giả sử rằng tập hợp S là tập hợp các ký hiệu của một lý thuyết toán học $\mathscr{T}$. Ta đặt $n(\square)=0$, $n(\tau)=n(\eta)=1$, $n(\vee)=2$, $n(x)=0$ với mọi chữ cái $x$;

và cuối cùng, với mọi dấu riêng biệt $s$ của $\mathscr{T}$, $n(s)$ là trọng số của $s$, được cố định khi đã cho $\mathscr{T}$.

¶ Cho $A$ là một assembly trong $\mathscr{T}$. Ta ký hiệu bởi $A^*$ từ thu được bằng cách xóa các liên kết trong $A$, và ta sẽ nói rằng $A$ là *cân bằng* nếu $A^*$ là cân bằng [trong $L_0(S)$]. Một *đoạn* của $A$ là bất kỳ assembly nào thu được bằng cách thay thế, trong một đoạn $S$ của $A^*$, các liên kết mà, trong $A$, nối các cặp ký hiệu trong $S$.

**TIÊU CHUẨN 1.** *Nếu $A$ là một số hạng hoặc một quan hệ trong $\mathscr{T}$, thì $A$ là cân bằng.*

Cho $A_1$, $A_2$, $\ldots$, $A_n$ tạo thành một phép dựng kiến tạo trong $\mathscr{T}$, trong đó $A$ xuất hiện. Lập luận bằng quy nạp và giả sử rằng ta đã chứng minh các $A_j$ có chỉ số $j<i$ là cân bằng; khi đó ta phải chứng minh rằng $A_i$ là cân bằng. Chứng minh diễn ra đúng như trong phần thứ nhất của chứng minh của Mệnh đề 2, trừ trường hợp $A_i$ có dạng $\tau_x(B)$ với $B=A_j$ và $j<i$. Trong trường hợp này, gọi $C$ là biểu thức thu được bằng cách thay thế $x$, ở mọi chỗ nó xuất hiện trong $B$, bởi $\square$. Khi đó từ $A^*$ đồng nhất với $\tau C^*$; mà $B^*$ là cân bằng, nên $C^*$ cũng cân bằng (vì $n(\square)=n(x)=0$). Do đó $A_i^*$ là cân bằng.

¶ Như vậy ta đã thu được một điều kiện cần thiết để một dãy ký hiệu trong $\mathscr{T}$ là một số hạng hoặc một quan hệ. Nhưng điều kiện này không đủ, như ta sẽ thấy.

¶ Cho $A$ là một dãy ký hiệu cân bằng trong $\mathscr{T}$. Nếu $A$ bắt đầu bằng một chữ cái hoặc một $\square$, thì $A$ phải chỉ gồm riêng ký hiệu này mà thôi (Mệnh đề 2, Hệ quả 2). Trong mọi trường hợp khác, bây giờ ta sẽ định nghĩa dãy ký hiệu hoặc các dãy ký hiệu *tiền thân* của $A$.

(1) Nếu $A$ bắt đầu bằng một $\land$, hoặc một $\vee$, hoặc một dấu riêng, thì $A^*$ có thể được viết theo đúng một cách dưới dạng $fB_1B_2\ldots B_p$, trong đó $f$ là một dấu có trọng số $p\geq 1$ và các $B_i$ đều cân bằng (Mệnh đề 2, Hệ quả 2). Các đoạn $A_1$, $A_2$, $\ldots$, $A_p$ của $A$ tương ứng với các đoạn $B_1$, $B_2$, $\ldots$, $B_p$ của $A^*$ được gọi là các dãy ký hiệu *tiền đề* của $A$. Hơn nữa, ta sẽ nói rằng $A$ là *cân bằng hoàn toàn* nếu $A$ đồng nhất với

$$
fA_1A_2\ldots A_p,
$$

nói cách khác nếu không có cạnh nào trong $A$ nối $f$ với một trong các $B_i$, hoặc nối hai $B_i$ phân biệt.

(2) Nếu $A$ bắt đầu bằng một $\tau$, thì $A^*$ có dạng $\tau B$, trong đó $B$ là cân bằng (Mệnh đề 2, Hệ quả 2). Trong trường hợp này, một dãy ký hiệu đứng trước $A$ là bất kỳ dãy ký hiệu nào trong các dãy ký hiệu $A_1$ được định nghĩa như sau : thay thế các dấu $\square$ trong $B$ mà trong $A$ được nối với $\tau$ ban đầu bằng một chữ cái $x$ phân biệt với các chữ cái khác xuất hiện trong $B$, và thay thế các liên kết nối hai dấu của $B$ trong $A$. (Nếu, thay cho $x$, ta thay vào một chữ cái $y$ cũng không xuất hiện trong $B$, thì ta thu được một dãy ký hiệu đơn giản là $(y|x)A_1$.) Hơn nữa, ta sẽ nói rằng $A$ là *cân bằng hoàn toàn* nếu $A$ đồng nhất với

$\tau_x(A_1)$, nói cách khác nếu không có liên kết nào nối $\tau$ ban đầu với một ký hiệu nào của $B$ khác ngoài một $\square$.

¶ Bây giờ ta có thể phát biểu tiêu chuẩn sau :

C2. *Cho $A$ là một cấu hình cân bằng trong $\mathscr{T}$.*

¶ *Điều kiện cần và đủ để $A$ là một số hạng là một trong các điều kiện sau được thỏa mãn : (1) $A$ gồm một chữ cái duy nhất; (2) $A$ bắt đầu bằng một $\tau$, cân bằng hoàn toàn, và các dãy ký hiệu đi trước nó là các quan hệ* (theo CF8, chỉ cần kiểm tra rằng *một* dãy ký hiệu đi trước nó là một quan hệ); *(3) $A$ bắt đầu bằng một dấu substantific, cân bằng hoàn toàn, và các dãy ký hiệu đi trước nó là các số hạng.* ¶ *Điều kiện cần và đủ để $A$ là một quan hệ là một trong các điều kiện sau được thỏa mãn : (1) $A$ bắt đầu bằng một $\vee$ hoặc một $\neg$, cân bằng hoàn toàn, và các dãy ký hiệu đi trước nó là các quan hệ; (2) $A$ bắt đầu bằng một dấu quan hệ, cân bằng hoàn toàn, và các dãy ký hiệu đi trước nó là các số hạng.*

Các tiêu chuẩn CF1 đến CF4 (§ 1, no. 4) cho thấy rằng các điều kiện là đủ. Ta sẽ chỉ ra rằng chúng là cần thiết. Ta đã thấy rồi (§ 1, no. 3) rằng nếu $A$ là một quan hệ, thì $A$ bắt đầu bằng một $\vee$, hoặc một $\neg$, hoặc một dấu quan hệ. Lập luận là đồng dạng trong mỗi một trong ba trường hợp. Chẳng hạn, nếu $A$ bắt đầu bằng một $\vee$, thì $A$ có dạng $\vee BC$, trong đó $B$ và $C$ là các quan hệ, nên $B$ và $C$ là các dãy ký hiệu tiền đề của $A$; do đó $A$ là cân bằng hoàn toàn. Nếu $A$ là một số hạng, thì có hai trường hợp: hoặc nó chỉ gồm một chữ cái duy nhất, hoặc nó bắt đầu bằng một dấu substantific hoặc một $\tau$. Trong trường hợp thứ hai, ta lập luận như trên. Nếu $A$ bắt đầu bằng một $\tau$, thì định nghĩa của một phép dựng kiến tạo cho thấy rằng $A$ có dạng $\tau_x(B)$, trong đó $B$ là một quan hệ và $x$ là một chữ cái, nên ta có thể lấy $B$ làm dãy ký hiệu tiền đề của $A$, và $A$ là cân bằng hoàn toàn.

Khi ta muốn kiểm tra xem một dãy ký hiệu đã cho $A$ (không gồm một chữ
cái duy nhất) có phải là một quan hệ (tương ứng, một số hạng) trong
$\mathscr{T}$ hay không, trước hết ta kiểm tra rằng $A$ là cân bằng và
nó bắt đầu bằng một $\vee$, một $\neg$, hoặc một dấu quan hệ (tương ứng,
bằng một $\tau$ hoặc một dấu thực thể). Sau đó ta lập dãy ký hiệu hoặc các
dãy ký hiệu đứng trước, và kiểm tra (nếu thích hợp) rằng $A$ là cân bằng
hoàn toàn. Làm xong điều này, ta còn lại một bài toán tương tự đối với các
dãy ký hiệu ngắn hơn. Như vậy, từng bước một, ta quy về các dãy ký hiệu mà
mỗi dãy chỉ gồm một dấu duy nhất, và đối với chúng nghiệm là ngay lập tức.

#### Nhận xét {#ens-i-a0-n4-rem-1 .statement tag=03GW}

Trừ trong một số lý thuyết toán học đặc biệt ít tiên đề (xem Bài tập 7),
ta không có một thủ tục tổng quát kiểu này để cho phép kiểm tra xem một
quan hệ đã cho $R$ trong một lý thuyết $\mathscr{T}$ có phải là một định lý
trong $\mathscr{T}$ hay không.

### Bài tập {#ens-i-a0-exercises}

Xem [bài tập cho Phụ lục 0](exercises/a0/).

[^1]: Các kết quả được thiết lập trong Phụ lục này sẽ không được dùng ở bất kỳ chỗ nào khác trong bộ sách này.
