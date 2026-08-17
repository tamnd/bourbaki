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
content_sha256: 7cdd5ada7ed51277ee7c1dee6c908b7d0241337110e4773a700ef994d75fa48e
translated_from: content/en/ens/I/A_a_characterization_of_terms_and_relations.md
source_content_sha256: df82f63eb14ef58e18c03d3cb3a5081969f0bab7d6da2f050817894fabf24715
translation_model: hy3-free, gpt-5.4-mini, gpt-5-6, laguna-s-2.1-free, gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-99f70c1a
glossary_version: 27
glossary_terms_sha256: 26a06154eb2737870a3589863d80b5e9532fdf7861c48acab26f27bc870afe5d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## Phụ lục

# Đặc trưng hóa các thuật ngữ và quan hệ

Siêu toán học, khi nó vượt quá mức rất sơ cấp của chương hiện tại, sử dụng đáng kể các kết quả của toán học, như chúng tôi đã nói trong Lời giới thiệu. Mục đích của phụ lục này là đưa ra một ví dụ đơn về kiểu lập luận này [^1]. Chúng tôi sẽ bắt đầu bằng việc thiết lập một số kết quả thuộc lý thuyết toán học về *nửa nhóm tự do*; sau đó chúng tôi sẽ dùng các kết quả này trong một " ứng dụng " siêu toán học để có được một đặc trưng hóa các thuật ngữ và quan hệ trong một lý thuyết.

### 1. Các dấu và các từ

* Cho S là một tập hợp không rỗng, các phần tử của nó sẽ được gọi là *ký hiệu* (thuật ngữ này thích hợp với ứng dụng siêu toán học mà ta có trong tâm trí). Cho $\mathrm{L}_0(\mathrm{S})$ là bán nhóm tự do sinh bởi S; các phần tử của $\mathrm{L}_0(\mathrm{S})$ được gọi là *từ* và được đồng nhất với các dãy hữu hạn $A = (s_i)_{0 \leqslant i \leqslant n}$ của các phần tử của S. Luật hợp thành trong $\mathrm{L}_0(\mathrm{S})$ sẽ được viết theo phép nhân, do đó $AB$ là dãy thu được bằng cách ghép $A$ và $B$ lại với nhau. Từ rỗng $\emptyset$ là phần tử đơn vị của $\mathrm{L}_0(\mathrm{S})$. Nhắc lại rằng độ dài $l(A)$ của một từ $A \in \mathrm{L}_0(\mathrm{S})$ là số phần tử trong dãy $A$; do đó $l(AB) = l(A) + l(B)$, và các từ có độ dài 1 là các ký hiệu. Cho $\mathrm{L}(\mathrm{S})$ ký hiệu tập hợp các từ không rỗng trong $\mathrm{L}_0(\mathrm{S})$.
¶ Giả sử, hơn nữa, ta được cho một ánh xạ $s \rightarrow n(s)$ của S vào

tập hợp $\mathbf{N}$ các số nguyên $\geqslant 0$. Với mỗi từ không rỗng $A = (s_i)_{0 \leqslant i \leqslant k}$ của L(S), ta đặt

$$n(A) \;=\; \sum_{i=0}^{k} \, n(s_i)$$

và $n(\emptyset) = 0$. $n(A)$ được gọi là *trọng số* của $A$. Rõ ràng $n(AB) = n(A) + n(B)$. ¶ Nếu $A = A'BA''$, từ $B$ được gọi là một *đoạn* của $A$ (một *thực sự* đoạn nếu cũng $B \neq A$). Nếu $A'$ (resp. $A''$) là rỗng, $B$ được gọi là một *ban đầu* (resp. *cuối*) đoạn của $A$. Nếu $l(A') = k$, thì $B$ được gọi là *bắt đầu tại vị trí thứ $(k+1)$*.

¶ Nếu $A = BCDEF$ (trong đó các từ $B$, $C$, $D$, $E$, $F$ có thể rỗng) thì các đoạn $C$ và $E$ của $A$ được gọi là *rời nhau*.

### 2. CÁC TỪ CÓ NGHĨA

Một *dãy đáng kể* là bất kỳ dãy $(A_j)_{1 \leqslant j \leqslant n}$ nào gồm các từ của $\mathrm{L}_0(\mathrm{S})$ có tính chất sau đây: với mỗi từ $A_i$ của dãy, một trong hai điều kiện sau được thỏa mãn:

(1) $A_i$ là một ký hiệu có trọng số 0.

(2) Tồn tại $p$ từ $A_{i_1}$, $A_{i_2}$, ..., $A_{i_p}$ trong dãy, với các chỉ số nhỏ hơn $i$, và một dấu $f$ có trọng số $p$ sao cho

$$A_i = f\, A_{i_1} A_{i_2} \, \ldots \, A_{i_p}.$$

Các từ xuất hiện trong các dãy đáng kể được gọi là *các từ có nghĩa*. Khi đó ta có:

#### Mệnh đề 1 {#ens-i-a0-prop-1 .statement tag=03P6}

*Nếu $A_1$, $A_2$, ..., $A_p$ là $p$ từ có nghĩa và nếu $f$ là một dấu có trọng số $p$, thì từ $f A_1 A_2 \ldots A_p$ là có nghĩa.*

### 3. ĐẶC TRƯNG CỦA CÁC TỪ CÓ NGHĨA

Một từ $A \in \mathrm{L}_0(\mathrm{S})$ được gọi là *cân bằng* nếu nó có hai tính chất sau:

(1) $l(A) = n(A) + 1$ (suy ra rằng $A$ không rỗng).

(2) Với mọi đoạn đầu thực sự $B$ của $A$, $l(B) \leqslant n(B)$.

#### Mệnh đề 2 {#ens-i-a0-prop-2 .statement tag=03P7}

*Một từ đáng kể khi và chỉ khi nó cân bằng.*

Cho $A$ là một từ đáng kể thuộc một dãy đáng kể

$$A_1, \; A_2, \; \ldots, \; A_n.$$

Ta sẽ chứng minh bằng quy nạp theo $k$ rằng mỗi $A_k$ là cân bằng. Giả sử điều này đã được thiết lập đối với các $A_j$ có chỉ số $j < k$, và ta hãy chứng minh rằng điều đó đúng với $A_k$. Nếu $A_k$ là một dấu có trọng số 0 (đây là khả năng duy nhất khi $k = 1$), thì $A_k$ là cân bằng vì

$$l(A_k) = 1 \qquad \text{và} \qquad n(A_k) = 0.$$

Nếu $A_k$ không phải là một dấu của trọng số 0, thì $A_k = fB_1B_2 \ldots B_p$, trong đó $f$ là một dấu của trọng số $p$, và các $B_j$ có dạng $A_{i_j}$, với $i_j < k$, và vì vậy là các từ cân bằng bởi giả thiết quy nạp. Chúng ta có

$$\begin{aligned} l(A_k) &= 1 + l(B_1) + l(B_2) + \cdots + l(B_p) \\ &= 1 + (n(B_1) + 1) + (n(B_2) + 1) + \cdots + (n(B_p) + 1) \\ &= 1 + p + n(B_1) + n(B_2) + \cdots + n(B_p) \\ &= 1 + n(A_k). \end{aligned}$$

Để $C$ là một đoạn ban đầu thực sự của $A$, và để $q$ là số nguyên lớn nhất trong các số $m < p$ sao cho $B_m$ là một đoạn của $C$, sao cho

$$C = f B_1 B_2 \ldots B_q D,$$

trong đó $D$ là một đoạn đầu thực sự của $B_{q+1}$. Khi đó

$$\begin{aligned} l(C) &= 1 + l(B_1) + l(B_2) + \cdots + l(B_q) + l(D) \\ &\leqslant 1 + (n(B_1) + 1) + (n(B_2) + 1) + \cdots + (n(B_q) + 1) + n(D) \\ &\leqslant p + n(B_1) + \cdots + n(B_q) + n(D) = n(C). \end{aligned}$$

Do đó $A_k$ là cân bằng.

¶ Để chứng minh rằng ngược lại, mọi từ cân bằng đều đáng kể, ta cần hai bổ đề sau:

#### Bổ đề 1 {#ens-i-a0-lem-1 .statement tag=03P8}

*Cho A là một từ cân bằng. Khi đó, với mỗi số nguyên k sao cho $0 \leqslant k < l(A)$, tồn tại duy nhất một đoạn cân bằng S của A bắt đầu tại vị trí thứ $(k + 1)$.*

Tính duy nhất của $S$ là một hệ quả ngay lập tức của nhận xét sau: nếu $T$ là một từ cân bằng, thì theo định nghĩa không có đoạn đầu thực sự nào của $T$ là cân bằng. Ta hãy chứng minh sự tồn tại của $S$. Viết $A = BC$ trong đó $l(B) = k$. Với mỗi $i$ sao cho $0 \leqslant i \leqslant q = l(C)$, gọi $C_i$ là đoạn đầu của $C$ có độ dài $i$. Vì $B$ là một đoạn đầu thực sự của $A$, ta có

$$l(C_q) = l(A) - l(B) \geqslant n(A) + 1 - n(B) = n(C_q) + 1.$$

Mặt khác, ta có $0 = l(C_0) \leqslant n(C_0) = 0$. Gọi $i$ là lớn nhất trong các số nguyên $j < q$ sao cho $l(C_h) \leqslant n(C_h)$ với $0 \leqslant h \leqslant j$; khi đó

ta có $l(C_i)\leq n(C_i)$ và $l(C_{i+1})\geq n(C_{i+1})+1$. Ta chứng minh rằng $C_{i+1}$ là cân bằng: điều kiện liên quan đến các đoạn ban đầu thực sự được thỏa mãn do định nghĩa của $i$; mặt khác, ta có

$$
n(C_{i+1})+1\leq l(C_{i+1})=l(C_i)+1\leq n(C_i)+1\leq n(C_{i+1})+1,
$$

nên $l(C_{i+1})=n(C_{i+1})+1$, và chứng minh của Bổ đề 1 là đầy đủ.

#### Bổ đề 2 {#ens-i-a0-lem-2 .statement tag=03GT}

Mọi từ cân bằng $A$ đều có thể được viết dưới dạng

$$
A=fA_1A_2\ldots A_p,
$$

trong đó các $A_i$ là cân bằng và $n(f)=p$.

Cho $f$ là dấu ban đầu của $A$. Theo Bổ đề 1, $A$ có thể viết thành

$$
fA_1A_2\ldots A_p,
$$

trong đó các $A_i$ là cân bằng: chúng ta chỉ cần định nghĩa $A_i$ bằng quy nạp như là đoạn cân bằng của $A$ bắt đầu tại vị trí thứ $k(i)$, trong đó

$$
k(i)=2+\sum_{j<i}l(A_j).
$$

Hơn nữa, chúng ta có

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

¶ Giờ đây hai bổ đề đã chứng minh, thì thật hiển nhiên bằng quy nạp trên độ dài của $A$ rằng mọi từ cân bằng $A$ đều đáng kể, bởi lý do của Bổ đề 2 và Mệnh đề 1.

#### Hệ quả 1 {#ens-i-a0-lem-2-cor-1 .statement tag=03GU}

Cho $A$ là một từ đáng kể. Với mỗi số nguyên $k$ sao cho $0\leq k<l(A)$ có đúng một đoạn đáng kể của $A$ bắt đầu tại vị trí thứ $(k+1)$.

#### Hệ quả 2 {#ens-i-a0-lem-2-cor-2 .statement tag=03GV}

Mọi từ đáng kể đều có thể được viết theo đúng một cách dưới dạng $fA_1A_2\ldots A_p$, trong đó các $A_i$ là đáng kể và $n(f)=p.$*

### 4. ỨNG DỤNG VÀO CÁC DÃY KÝ HIỆU TRONG MỘT LÝ THUYẾT TOÁN HỌC

Giả sử tập hợp S là tập hợp các dấu của một lý thuyết toán học $\mathscr{T}$. Ta đặt $n(\square)=0$, $n(\tau)=n(\eta)=1$, $n(\vee)=2$, $n(x)=0$ với mọi chữ cái $x$;

Và cuối cùng, với mỗi ký hiệu cụ thể $s$ của $\mathscr{T}$, $n(s)$ là trọng số của $s$, trọng số này được cố định khi $\mathscr{T}$ được cho.

¶ Cho $A$ là một hợp tử trong $\mathscr{T}$. Chúng ta ký hiệu bằng $A^*$ từ thu được bằng cách xóa các liên kết trong $A$, và chúng ta sẽ nói rằng $A$ là *cân bằng* nếu $A^*$ là cân bằng [trong $L_0(S)$]. Một *đoạn* của $A$ là một hợp tử bất kỳ thu được bằng cách thay thế, trong một đoạn $S$ của $A^*$, các liên kết mà, trong $A$, nối các cặp dấu trong $S$.

**Tiêu chuẩn 1.** *Nếu $A$ là một số hạng hoặc một quan hệ trong $\mathscr{T}$, thì $A$ là cân bằng.*

Cho $A_1$, $A_2$, $\ldots$, $A_n$ là một phép dựng kiến tạo trong $\mathscr{T}$, trong đó $A$ xuất hiện. Chúng ta hãy lập luận theo quy nạp và giả sử rằng ta đã chứng minh các $A_j$ có chỉ số $j<i$ là cân bằng; khi đó ta phải chứng minh $A_i$ là cân bằng. Chứng minh tiến hành cũng như trong phần đầu của chứng minh của Mệnh đề 2, ngoại trừ khi $A_i$ có dạng $\tau_x(B)$ với $B=A_j$ và $j<i$. Trong trường hợp này, cho $C$ là hợp tử thu được bằng cách thay thế $x$, ở bất cứ đâu nó xuất hiện trong $B$, bằng $\square$. Từ $A^*$ khi đó đồng nhất với $\tau C^*$; nay $B^*$ là cân bằng, và do đó $C^*$ là cân bằng (bởi vì $n(\square)=n(x)=0$). Do đó $A_i^*$ là cân bằng.

¶ Như vậy, ta đã thu được một điều kiện cần để một dãy ký hiệu trong $\mathscr{T}$ là một số hạng hoặc một quan hệ. Nhưng điều kiện này không đủ, như ta sẽ thấy.

¶ Cho $A$ là một dãy ký hiệu cân bằng trong $\mathscr{T}$. Nếu $A$ bắt đầu bằng một chữ cái hoặc một $\square$, thì $A$ phải chỉ gồm riêng dấu này (Mệnh đề 2, Hệ quả 2). Trong mọi trường hợp khác, ta sẽ định nghĩa ngay các dãy ký hiệu *tiền nhiệm* của $A$.

(1) Nếu $A$ bắt đầu bằng một $\land$, hoặc một $\vee$, hoặc một dấu cụ thể, thì $A^*$ có thể được viết theo đúng một cách dưới dạng $fB_1B_2\ldots B_p$, trong đó $f$ là một dấu có trọng số $p\geq 1$ và các $B_i$ là cân bằng (Mệnh đề 2, Hệ quả 2). Các đoạn $A_1$, $A_2$, $\ldots$, $A_p$ của $A$ tương ứng với các đoạn $B_1$, $B_2$, $\ldots$, $B_p$ của $A^*$ được gọi là các dãy ký hiệu *tiền nhiệm* của $A$. Hơn nữa, ta sẽ nói rằng $A$ là *cân bằng hoàn toàn* nếu $A$ đồng nhất với

$$
fA_1A_2\ldots A_p,
$$

nói cách khác nếu không có liên kết nào trong $A$ nối $f$ với một trong các $B_i$, hoặc nối hai $B_i$ phân biệt.

(2) Nếu $A$ bắt đầu bằng một $\tau$, thì $A^*$ có dạng $\tau B$, trong đó $B$ là cân bằng (Mệnh đề 2, Hệ quả 2). Trong trường hợp này, một dãy ký hiệu tiền thân của $A$ là bất kỳ dãy ký hiệu nào trong các dãy ký hiệu $A_1$ được định nghĩa như sau: thay thế các dấu $\square$ trong $B$ được nối trong $A$ với $\tau$ ban đầu bằng một chữ $x$ phân biệt với các chữ khác xuất hiện trong $B$, và thay thế các liên kết nối hai dấu của $B$ trong $A$. (Nếu thay $x$ bằng một chữ $y$ cũng không xuất hiện trong $B$, ta được một dãy ký hiệu đúng bằng $(y|x)A_1$.) Hơn nữa, ta sẽ nói rằng $A$ là *cân bằng hoàn toàn* nếu $A$ đồng nhất với

$\tau_x(A_1)$, nói cách khác nếu không có liên kết nào nối $\tau$ ban đầu với bất kỳ dấu nào của $B$ ngoài một $\square$.

¶ Bây giờ ta có thể phát biểu tiêu chuẩn sau:

C2. *Cho $A$ là một cấu hình cân bằng trong $\mathscr{T}$.*

¶ *Để $A$ là một số hạng thì cần thiết và đủ rằng một trong các điều kiện sau được thỏa mãn : (1) $A$ gồm một chữ cái duy nhất; (2) $A$ bắt đầu bằng một $\tau$, hoàn toàn cân bằng, và các dãy ký hiệu tiền đề của nó là các quan hệ* (theo CF8, đủ để kiểm tra rằng *một* dãy ký hiệu tiền đề là một quan hệ); *(3) $A$ bắt đầu bằng một dấu tạo chất, hoàn toàn cân bằng, và các dãy ký hiệu tiền đề của nó là các số hạng.*
¶ *Để $A$ là một quan hệ thì cần thiết và đủ rằng một trong các điều kiện sau được thỏa mãn : (1) $A$ bắt đầu bằng một $\vee$ hoặc một $\neg$, hoàn toàn cân bằng, và các dãy ký hiệu tiền đề của nó là các quan hệ; (2) $A$ bắt đầu bằng một dấu quan hệ, hoàn toàn cân bằng, và các dãy ký hiệu tiền đề của nó là các số hạng.*

Các tiêu chuẩn CF1 đến CF4 (§ 1, no. 4) chỉ ra rằng các điều kiện là đủ. Ta hãy chỉ ra rằng chúng là cần thiết. Ta đã thấy (§ 1, no. 3) rằng nếu $A$ là một quan hệ, thì $A$ bắt đầu bằng một $\vee$, hoặc một $\neg$, hoặc một dấu quan hệ. Lập luận là đồng dạng trong mỗi ba trường hợp. Nếu, ví dụ, $A$ bắt đầu bằng một $\vee$, thì $A$ có dạng $\vee BC$, trong đó $B$ và $C$ là các quan hệ, do đó $B$ và $C$ là các dãy ký hiệu đứng trước $A$; vì vậy $A$ hoàn toàn cân bằng. Nếu $A$ là một số hạng, thì có hai trường hợp : nó gồm một chữ cái đơn, hoặc nó bắt đầu bằng một dấu thực chất hoặc một $\tau$. Trong trường hợp thứ hai, ta lập luận như trên. Nếu $A$ bắt đầu bằng một $\tau$, định nghĩa về một phép dựng kiến tạo chỉ ra rằng $A$ có dạng $\tau_x(B)$, trong đó $B$ là một quan hệ và $x$ là một chữ cái, sao cho ta có thể lấy $B$ làm dãy ký hiệu đứng trước $A$, và $A$ hoàn toàn cân bằng.

Khi chúng ta muốn kiểm tra xem một dãy ký hiệu cho trước $A$ (không gồm một chữ cái đơn) có phải là một quan hệ (tương ứng là một số hạng) trong $\mathscr{T}$ hay không, trước tiên chúng ta xác minh rằng $A$ là cân bằng và rằng nó bắt đầu bằng một $\vee$, một $\neg$, hoặc một dấu quan hệ (tương ứng với một $\tau$ hoặc một dấu thực thể). Sau đó chúng ta hình thành dãy ký hiệu tiền đề hoặc các dãy ký hiệu tiền đề, và xác minh (nếu thích hợp) rằng $A$ là hoàn toàn cân bằng. Sau khi làm điều đó, chúng ta còn lại với một bài toán tương tự liên quan đến các dãy ký hiệu ngắn hơn. Như vậy, từng bước một, chúng ta đi xuống đến các dãy ký hiệu mà mỗi cái gồm một dấu đơn, đối với chúng nghiệm là ngay lập tức.

#### Nhận xét {#ens-i-a0-n4-rem-1 .statement tag=03GW}

Ngoại trừ trong một số lý thuyết toán học đặc biệt yếu về tiên đề (xem Bài tập 7), chúng ta không có một thủ tục tổng quát thuộc loại này để cho phép chúng ta kiểm tra xem một quan hệ cho trước $R$ trong một lý thuyết $\mathscr{T}$ có phải là một định lý trong $\mathscr{T}$ hay không.

### Bài tập {#ens-i-a0-exercises}

Xem [các bài tập cho Phụ lục 0](exercises/a0/).

[^1]: (*) Các kết quả được thiết lập trong Phụ lục này sẽ không được sử dụng ở bất kỳ nơi nào khác trong loạt sách này.
