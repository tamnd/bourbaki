---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 5
section_title: Properties of integers
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 171-183, 235-240
pdf_pages: 0177-0189, 0241-0246
extraction: ocr
subsections:
    - "no": 1
      title: OPERATIONS ON INTEGERS AND FINITE SETS
      page: 171
      pdf_page: 177
    - "no": 2
      title: STRICT INEQUALITIES BETWEEN INTEGERS
      page: 173
      pdf_page: 179
    - "no": 3
      title: INTERVALS IN SETS OF INTEGERS
      page: 174
      pdf_page: 180
    - "no": 4
      title: FINITE SEQUENCES
      page: 175
      pdf_page: 181
    - "no": 5
      title: CHARACTERISTIC FUNCTIONS OF SETS
      page: 175
      pdf_page: 181
    - "no": 6
      title: EUCLIDEAN DIVISION
      page: 176
      pdf_page: 182
    - "no": 7
      title: EXPANSION TO BASE $b$
      page: 177
      pdf_page: 183
    - "no": 8
      title: COMBINATORIAL ANALYSIS
      page: 179
      pdf_page: 185
statements: 30
exercises: 18
content_sha256: b51795f6a682e38bc4003611f271f641a1e74c916da18b46672abb47f636a238
translated_from: content/en/ens/III/05_s5_properties_of_integers.md
source_content_sha256: 539828b0c422fed3a1cc49cb93eb6b9243ff661d733b947ed2c4b6d11d68b451
translation_model: gpt-5-6, gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-ebf13ef0
glossary_version: 29
glossary_terms_sha256: b38e6d2ba48454073ae09e72f9c985e28155d8d69c8d1f062ae11edf2f680c66
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 5. CÁC TÍNH CHẤT CỦA SỐ NGUYÊN

### 1. CÁC PHÉP TOÁN TRÊN SỐ NGUYÊN VÀ CÁC TẬP HỢP HỮU HẠN

#### Mệnh đề 1 {#ens-iii-s5-prop-1 .statement tag=03LP}

*Cho $(a_i)_{i \in I}$ là một họ hữu hạn các số nguyên. Khi đó các lực lượng $\sum_{i \in I} a_i$ và $\prod_{i \in I} a_i$ là các số nguyên.*

Trước hết, ta chứng minh rằng nếu $a$ và $b$ là các số nguyên thì $a + b$ cũng là một số nguyên. Ta tiến hành quy nạp theo $b$. Mệnh đề đúng với $b = 0$ vì $a + 0 = a$. Nếu $a + b$ là một số nguyên thì $(a + b) + 1$ cũng là một số nguyên (§ 4, no. 1, Mệnh đề 1). Nhưng $(a + b) + 1 = a + (b + 1)$ (§ 3, no. 3, Hệ quả của Mệnh đề 5); do đó $a + (b + 1)$ là một số nguyên, và do đó $a + b$ là một số nguyên với mọi số nguyên $b$.

Tiếp theo ta chứng minh bằng quy nạp theo $n = \mathrm{Card}\ (\mathrm{I})$ rằng $\sum\limits_{i \in \mathrm{I}} a_i$ là một số nguyên. Điều này hiển nhiên nếu $n = 0$, vì khi đó $\mathrm{I} = \emptyset$ và $\sum\limits_{i \in \mathrm{I}} a_i = 0$. Nếu $\mathrm{Card}\ (\mathrm{I}) = n + 1$, ta có thể viết $\mathrm{I} = \mathrm{J} \cup \{k\}$, trong đó $\mathrm{Card}\ (\mathrm{J}) = n$ và $k \notin \mathrm{J}$. Khi đó

$$\sum_{i \in \mathrm{I}} a_i = a_k + \sum_{i \in \mathrm{J}} a_i$$

($\S\,3$, no. 3, Mệnh đề 5). Giả thiết quy nạp là $\sum\limits_{i \in \mathrm{J}} a_i$ là một số nguyên; do đó $a_k + \sum\limits_{i \in \mathrm{J}} a_i$ cũng là một số nguyên, theo đoạn thứ nhất của chứng minh. Điều đó chứng tỏ rằng $\sum\limits_{i \in \mathrm{I}} a_i$ là một số nguyên với mọi $n$.

Vì tích $ab$ của hai số nguyên $a$ và $b$ là tổng của một họ hữu hạn các số nguyên đều bằng $a$ ($\S\,3$, no. 4, Mệnh đề 6, Hệ quả 2), nên $ab$ là một số nguyên. Ta sẽ chứng minh bằng quy nạp theo $n = \mathrm{Card}\ (\mathrm{I})$ rằng $\prod\limits_{i \in \mathrm{I}} a_i$ là một số nguyên. Điều này đúng với $n = 0$, vì khi đó

$$\prod_{i \in \mathrm{I}} a_i = 1.$$

Nếu $\mathrm{Card}\ (\mathrm{I}) = n + 1$, ta có (với cùng ký hiệu như ở trên)

$$\prod_{i \in \mathrm{I}} a_i = a_k \cdot \prod_{i \in \mathrm{J}} a_i$$

($\S\,3$, no. 3, Mệnh đề 5), và do đó giả thiết quy nạp suy ra rằng $\prod\limits_{i \in \mathrm{I}} a_i$ là một số nguyên. Do đó $\prod\limits_{i \in \mathrm{I}} a_i$ là một số nguyên với mọi $n$.

#### Hệ quả 1 {#ens-iii-s5-prop-1-cor-1 .statement tag=03LQ}

*Hợp* E *của một họ hữu hạn* $(\mathrm{X}_i)_{i \in \mathrm{I}}$ *các tập hợp hữu hạn là một tập hợp hữu hạn.*

Vì tổng S của họ $(\mathrm{X}_i)$ là hữu hạn; và vì tồn tại một ánh xạ từ S lên E (chương II, $\S\,4$, no. 8), tập hợp E là hữu hạn ($\S\,4$, no. 2, Mệnh đề 2, Hệ quả 3).

#### Hệ quả 2 {#ens-iii-s5-prop-1-cor-2 .statement tag=03LR}

*Tích của một họ hữu hạn các tập hợp hữu hạn là một tập hợp hữu hạn.*

#### Hệ quả 3 {#ens-iii-s5-prop-1-cor-3 .statement tag=03LS}

*Nếu $a$ và $b$ là các số nguyên, $a^b$ là một số nguyên.*

Vì $a^b$ là tích của một họ hữu hạn các số nguyên đều bằng $a$ ($\S\,3$, no. 5, Mệnh đề 10).

#### Hệ quả 4 {#ens-iii-s5-prop-1-cor-4 .statement tag=03LT}

*Tập hợp các tập con của một tập hợp hữu hạn* E *là hữu hạn.*

Vì lực lượng của nó là $2^{\mathrm{Card}\ (\mathrm{E})}$ ($\S\,3$, no. 5, Mệnh đề 12).

### 2. BẤT ĐẲNG THỨC CHẶT GIỮA CÁC SỐ NGUYÊN

#### Mệnh đề 2 {#ens-iii-s5-prop-2 .statement tag=03LU}

*Cho $a$ và $b$ là hai số nguyên. Khi đó $a < b$ nếu và chỉ nếu tồn tại một số nguyên $c > 0$ sao cho $b = a + c$.*

Nếu $a < b$, thì tồn tại một lực lượng $c \leqslant b$ (do đó $c$ là một số nguyên (§ 4, no. 2, Mệnh đề 2)) sao cho $b = a + c$ (§ 3, no. 6, Mệnh đề 13); nếu $a \neq b$, thì tất phải có $c \neq 0$. Ngược lại, nếu $b = a + c$ và $c \neq 0$, thì $c \geqslant 1$ và do đó $a < a + 1 \leqslant a + c = b$.

#### Mệnh đề 3 {#ens-iii-s5-prop-3 .statement tag=03LV}

*Cho $(a_i)_{i \in I}$ và $(b)_{i \in I}$ là hai họ hữu hạn các số nguyên sao cho $a_i \leqslant b_i$ với mọi $i \in I$ và $a_i < b_i$ với ít nhất một chỉ số $i$. Khi đó*

$$\sum_{i \in I} a_i < \sum_{i \in I} b_i.$$

*Nếu thêm nữa $b_i > 0$ với mọi $i \in I$, thì*

$$\prod_{i \in I} a_i < \prod_{i \in I} b_i.$$

Lấy $j$ là một chỉ số sao cho $a_j < b_j$, và đặt $J = I - \{j\}$. Khi đó

$$b_j = a_j + c_j$$

với $c_j > 0$ (Mệnh đề 2), và do đó (§ 3, no. 6, Mệnh đề 14)

$$\sum_{i \in I} b_i = a_j + c_j + \sum_{i \in J} b_i \geqslant c_j + a_j + \sum_{i \in J} a_i = c_j + \sum_{i \in I} a_i.$$

Vì $c_j > 0$, phần thứ nhất của Mệnh đề suy ra từ Mệnh đề 2. Tương tự,

$$\prod_{i \in I} b_i = (a_j + c_j) \prod_{i \in J} b_i = a_j . \prod_{i \in J} b_i + c_j . \prod_{i \in J} b_i \geqslant \prod_{i \in I} a_i + c_j . \prod_{i \in J} b_i.$$

Vì $c_j$ và mọi $b_i$ đều là $\neq 0$, tích $c_j . \prod_{i \in J} b_i$ là $\neq 0$ (§ 3, no. 4, Mệnh đề 7); do đó suy ra phần thứ hai của Mệnh đề.

#### Hệ quả 1 {#ens-iii-s5-prop-3-cor-1 .statement tag=03LW}

*Cho $a$, $a'$, và $b$ là các số nguyên sao cho $a < a'$ và $b > 0$. Khi đó $a^b < a'^b$.*

Chỉ cần biểu diễn $a^b$ và $a'^b$ dưới dạng tích của các họ hữu hạn các số nguyên (§ 3, no. 5, Mệnh đề 10) và áp dụng Mệnh đề 3, nhận thấy rằng quan hệ $a < a'$ kéo theo $a' > 0$.

#### Hệ quả 2 {#ens-iii-s5-prop-3-cor-2 .statement tag=03LX}

*Cho $a$, $b$ và $b'$ là các số nguyên sao cho $a > 1$ và $b < b'$; khi đó $a^b < a^{b'}$.*

Vì tồn tại một số nguyên $c > 0$ sao cho $b' = b + c$ (Mệnh đề 2); do $c \geqslant 1$, ta có $a^c \geqslant a > 1$, do đó $a^{b'} = a^b a^c > a^b$.

#### Hệ quả 3 {#ens-iii-s5-prop-3-cor-3 .statement tag=03LY}

*Cho $a$, $b$, $b'$ là các số nguyên* (resp. *các số nguyên sao cho $a > 0$*). *Khi đó $a + b = a + b'$* (resp. *$ab = ab'$*) *khi và chỉ khi $b = b'$.*

#### Hệ quả 4 {#ens-iii-s5-prop-3-cor-4 .statement tag=03LZ}

*Nếu $a$ và $b$ là các số nguyên sao cho $a \leqslant b$, thì tồn tại một số nguyên duy nhất $c$ sao cho $b = a + c$.*

Sự tồn tại của $c$ suy ra từ Mệnh đề 13 của § 3, no. 6, và tính duy nhất của nó suy ra từ Hệ quả 3 ở trên.

¶ Số nguyên $c$ sao cho $b = a + c$ (trong đó $a \leqslant b$) được gọi là *hiệu* của các số nguyên $b$ và $a$, và được viết là $b - a$. Dễ dàng kiểm tra rằng nếu $a$, $b$, $a'$, $b'$ là các số nguyên sao cho $a \leqslant b$ và $a' \leqslant b'$, thì

$$(b - a) + (b' - a') = (b + b') - (a + a').$$

### 3. CÁC KHOẢNG TRONG CÁC TẬP HỢP SỐ NGUYÊN

Mọi tập hợp các số nguyên, vì là một tập hợp các lực lượng, đều được sắp tốt (§ 3, no. 2, Định lý 1). Hơn nữa, với mỗi số nguyên $a$, quan hệ "$x$ là một lực lượng và $x \leqslant a$" là xác định tập theo $x$ (§ 3, no. 2, Chú ý sau Định lý 1), và tập hợp các $x$ thỏa mãn quan hệ này là một tập hợp các số nguyên (§ 4, no. 2, Mệnh đề 2), do đó có thể được ký hiệu là $[0, a]$.

#### Mệnh đề 4 {#ens-iii-s5-prop-4 .statement tag=03M0}

*Cho $a$ và $b$ là các số nguyên. Khi đó ánh xạ $x \rightarrow a + x$ là một đẳng cấu tăng ngặt của khoảng $[0, b]$ lên khoảng $[a, a + b]$, và $y \rightarrow y - a$ là đẳng cấu nghịch đảo.*

Rõ ràng các quan hệ $0 \leqslant x \leqslant b$ suy ra $a \leqslant a + x \leqslant a + b$. Ánh xạ $x \rightarrow a + x$ là tăng ngặt (và do đó đơn ánh) theo Mệnh đề 3 của no. 2. Cuối cùng, các quan hệ $a \leqslant y \leqslant a + b$ suy ra $y = a + x$ với $x \geqslant 0$ và $a + x \leqslant a + b$, do đó $x \leqslant b$ (no. 2, Mệnh đề 3). Điều này hoàn tất chứng minh.

#### Mệnh đề 5 {#ens-iii-s5-prop-5 .statement tag=03M1}

*Nếu $a$ và $b$ là các số nguyên sao cho $a \leqslant b$, thì khoảng $[a, b]$ là một tập hợp hữu hạn có số phần tử bằng $b - a + 1$.*

Theo Mệnh đề 4, ta có thể chỉ xét trường hợp $a = 0$. Chứng minh bằng quy nạp theo $b$. Nếu $b = 0$ thì kết quả là hiển nhiên. Quan hệ $0 \leqslant x \leqslant b + 1$ tương đương với "$0 \leqslant x < b + 1$ hoặc $x = b + 1$", và quan hệ $0 \leqslant x < b + 1$ tương đương với $0 \leqslant x \leqslant b$ (§ 4, no. 2, Mệnh đề 2); nói cách khác, khoảng $[0, b + 1]$ là hợp của $[0, b]$

và $\{b + 1\}$, và hai tập hợp này rời nhau. Theo giả thiết quy nạp, số phần tử của $[0, b + 1]$ bằng $(b + 1) + 1$, và mệnh đề được chứng minh.

#### Mệnh đề 6 {#ens-iii-s5-prop-6 .statement tag=03M2}

*Với mọi tập hợp hữu hạn* E *được sắp thứ tự toàn phần và có n phần tử* $(n \geqslant 1)$, *tồn tại một đẳng cấu duy nhất của* E *lên khoảng* $[1, n]$.

Vì E và $[1, n]$ được sắp tốt (§ 4, no. 4, Mệnh đề 3, Hệ quả 1) và có cùng số phần tử (Mệnh đề 5), kết quả suy ra từ Định lý 3 của § 2, no. 5 và Hệ quả 2 của Mệnh đề 2 của § 4, no. 2.

### 4. DÃY HỮU HẠN

Một *dãy hữu hạn* (resp. *dãy hữu hạn các phần tử của một tập hợp* E) là một họ (resp. một họ các phần tử của E) mà tập chỉ số I của nó là một tập hợp hữu hạn các số nguyên. Số phần tử của I được gọi là *độ dài* của dãy.

Cho $(t_i)_{i \in I}$ là một dãy hữu hạn có độ dài $n$. Theo Mệnh đề 6 của no. 3, tồn tại một đẳng cấu duy nhất $f$ từ khoảng $[1, n]$ lên tập hợp các số nguyên I. Với mỗi $k \in [1, n]$, $t_{f(k)}$ được gọi là *số hạng thứ k của dãy*; $t_{f(1)}$ (resp. $t_{f(n)}$) là *số hạng* *đầu tiên* (resp. *cuối cùng*) của dãy.

Let $\mathrm{P}\{i\}$ là một quan hệ sao cho các phần tử $i$ mà $\mathrm{P}\{i\}$ đúng tạo thành một tập hữu hạn các số nguyên. Khi đó một dãy hữu hạn $(t_i)_{i \in I}$ thường được viết là $(t_i)_{\mathrm{P}\{i\}}$. Chẳng hạn, khi $\mathrm{I} = [a, b]$, ký hiệu $(t_i)_{a \leqslant i \leqslant b}$ thường được sử dụng. Với cùng các điều kiện đó, để chỉ tích của một họ tập hợp $(\mathrm{X}_i)_{i \in I}$, các ký hiệu

$$\prod_{\mathrm{P}\{i\}} \mathrm{X}_i \quad \text{và} \quad \prod_{i=a}^{b} \mathrm{X}_i$$

được sử dụng; và các ký hiệu tương tự cho hợp, giao, tích lực lượng, tổng lực lượng, \* các luật hợp thành trong Đại số $_*$, v.v.

### 5. CÁC HÀM ĐẶC TRƯNG CỦA TẬP HỢP

Cho E là một tập hợp khác rỗng và A là một tập con của E. *Hàm đặc trưng* của tập con A của E là ánh xạ $\varphi_\mathrm{A}$ từ E vào tập hợp $\{0, 1\}$ được định nghĩa bởi

$$\varphi_\mathrm{A}(x) = 1 \quad \text{nếu} \quad x \in \mathrm{A}; \qquad \varphi_\mathrm{A}(x) = 0 \quad \text{nếu} \quad x \in \mathrm{E} - \mathrm{A}.$$

¶ Rõ ràng quan hệ $\varphi_\mathrm{A} = \varphi_\mathrm{B}$ tương đương với $\mathrm{A} = \mathrm{B}$. Ta có $\varphi_\mathrm{E}(x) = 1$ với mọi $x \in \mathrm{E}$ và $\varphi_{\emptyset}(x) = 0$ với mọi $x \in \mathrm{E}$; đây là các hàm đặc trưng hằng duy nhất trên E. Mệnh đề sau là một hệ quả ngay lập tức của các định nghĩa:

#### Mệnh đề 7 {#ens-iii-s5-prop-7 .statement tag=03M3}

*Với mỗi cặp tập con* A, B *của một tập hợp khác rỗng* E, *ta có*

(1) $$\varphi_{\mathrm{E-A}}(x) = 1 - \varphi_{\mathrm{A}}(x),$$

(2) $$\varphi_{\mathrm{A} \cap \mathrm{B}}(x) = \varphi_{\mathrm{A}}(x)\varphi_{\mathrm{B}}(x),$$

(3) $$\varphi_{\mathrm{A} \cup \mathrm{B}}(x) + \varphi_{\mathrm{A} \cap \mathrm{B}}(x) = \varphi_{\mathrm{A}}(x) + \varphi_{\mathrm{B}}(x)$$

*với mọi* $x \in \mathrm{E}$.

### 6. PHÉP CHIA EUCLID

#### Định lý 1 {#ens-iii-s5-thm-1 .statement tag=03M4}

*Cho a và b là các số nguyên sao cho $b > 0$. Khi đó tồn tại các số nguyên q và r sao cho $a = bq + r$ và $r < b$, và các số nguyên q và r được xác định duy nhất bởi các điều kiện này.*

Các điều kiện đối với $q$ và $r$ là tương đương với $bq \leqslant a < b(q + 1)$ và $r = a - bq$ (no. 2, Mệnh đề 2). Vậy ta phải tìm $q$ sao cho $bq \leqslant a < b(q + 1)$; nói cách khác, $q$ phải là số nguyên nhỏ nhất sao cho $a < b(q + 1)$, điều này cho thấy $q$ và $r = a - bq$ được xác định duy nhất. Để chứng minh sự tồn tại của chúng, ta chú ý rằng tồn tại các số nguyên $p$ sao cho $a < bp$, ví dụ $a + 1$ (vì $b > 0$). Gọi $m$ là số nhỏ nhất trong các số nguyên ấy. Ta có $m \neq 0$, và do đó có thể viết $m = q + 1$ với $q \leqslant m$ (§ 4, no. 2, Mệnh đề 2); suy ra $bq \leqslant a < b(q + 1)$.

#### Định nghĩa 1 {#ens-iii-s5-def-1 .statement tag=03M5}

*Với ký hiệu của Định lý 1, r được gọi là số dư của phép chia a cho b. Nếu $r = 0$, ta nói rằng a là bội của b, hoặc a chia được cho b, hoặc b là ước của a, hoặc b chia hết a, hoặc b là nhân tử của a. Khi đó số q được gọi là thương của a cho b và được ký hiệu bởi $\dfrac{a}{b}$ hoặc $a/b$.*

Nếu $a$ không là bội của $b$, số $q$ được gọi là *phần nguyên của thương của a cho b* (xem *Tôpô đại cương*, chương IV, § 8, số 2).

*Trong chương này*, viết $a/b$ hoặc $\dfrac{a}{b}$ sẽ ngụ ý rằng $b$ chia hết $a$.

Các hệ thức $a = bq$ và $q = a/b$ là tương đương (nếu $b > 0$). Mọi bội $a'$ của một bội $a$ của $b$ đều là bội của $b$, và

$$a'/b = (a'/a)\,(a/b) \qquad \text{nếu} \qquad a \neq 0.$$

Hơn nữa, nếu $c$ và $d$ là các bội của $b$, thì $c+d$ và $c-d$ (nếu $d\leq c$) là các bội của $b$, và ta có

$$\frac{c+d}{b}=\frac{c}{b}+\frac{d}{b},\qquad \frac{c-d}{b}=\frac{c}{b}-\frac{d}{b}.$$

Các số nguyên là bội của 2 được gọi là *chẵn*, còn các số nguyên khác là *lẻ*. Theo Định lý 1, các số nguyên lẻ có dạng $2n+1$.

### 7. KHAI TRIỂN THEO CƠ SỞ $b$

#### Mệnh đề 8 {#ens-iii-s5-prop-8 .statement tag=03M6}

*Cho $b$ là một số nguyên $>1$. Với mỗi số nguyên $k>0$, cho $E_k$ là tích từ điển (§ 2, no. 6) của họ $(J_h)_{0\leq h\leq k-1}$ gồm các khoảng đều đồng nhất với $[0,b-1]$. Với mỗi $r=(r_0,r_1,\ldots,r_{k-1})\in E_k$, cho*

$$f_k(r)=\sum_{h=0}^{k-1}r_hb^{k-h-1};$$

*khi đó ánh xạ $f_k$ là một đẳng cấu của tập hợp có thứ tự $E_k$ lên khoảng $[0,b^k-1]$.*

Chứng minh được tiến hành bằng quy nạp theo $k$. Với $k=1$, đó là một hệ quả ngay lập tức của các định nghĩa. Với mỗi $r=(r_0,\ldots,r_{k-1},r_k)\in E_{k+1}$, đặt

$$\varphi(r)=(r_0,\ldots,r_{k-1})\in E_k.$$

Khi đó ánh xạ $r\mapsto(\varphi(r),r_k)$ là một đẳng cấu từ $E_{k+1}$ lên tích theo thứ tự từ điển của $E_k$ và $J=[0,b-1]$; điều này suy ra ngay lập tức từ các định nghĩa. Ta có thể viết

$$f_{k+1}(r)=b\cdot f_k(\varphi(r))+r_k;$$

cho ta thấy rằng quan hệ $r<r'$ trong $E_{k+1}$ kéo theo $f_{k+1}(r)<f_{k+1}(r')$. Thật vậy, hoặc $\varphi(r)<\varphi(r')$, hoặc $\varphi(r)=\varphi(r')$ và $r_k<r'_k$. Trong trường hợp thứ nhất, giả thiết quy nạp suy ra $f_k(\varphi(r))<f_k(\varphi(r'))$, và do đó (§ 4, no. 2, Mệnh đề 2) $f_k(q(r'))\geq f_k(\varphi(r))+1$; do đó

$$f_{k-1}(r')\geq b\cdot f_k(\varphi(r))+b>f_{k+1}(r),$$

vì $r_k\leq b-1$ (no. 2, Mệnh đề 3). Mặt khác, nếu $\varphi(r)=\varphi(r')$ và $r_k<r'_k$, thì hiển nhiên $f_{k+1}(r)<f_{k+1}(r')$. Khi đó, giả thiết quy nạp cho thấy $f_k(\varphi(r))\leq b^k-1$, do đó

$$f_{k+1}(r)\leq b(b^k-1)+b-1=b^{k+1}-1.$$

Suy ra rằng $f_{k+1}$ là một đẳng cấu của $E_{k+1}$ lên một tập con của khoảng $[0,b^{k+1}-1]$; nhưng khoảng này và $E_{k+1}$ có cùng số

các phần tử, tức là $b^{k+1}$ (no. 3, Mệnh đề 5); do đó $f_{k+1}$ là một song ánh (§ 4, no. 2, Mệnh đề 2, Hệ quả 4), và chứng minh đã đầy đủ.
¶ Bây giờ ta chú ý rằng với mọi số nguyên $a$ ta có $a < b^a$. Điều này được chứng minh bằng quy nạp theo $a$; kết quả là hiển nhiên đối với $a = 0$, và giả thiết $a < b^a$ kéo theo $a + 1 \leqslant b^a < b \cdot b^a = b^{a+1}$ (no. 2, Mệnh đề 3 và § 4, no. 2, Mệnh đề 2). Vì vậy tồn tại số nguyên nhỏ nhất $k$ sao cho $a < b^k$, và khi đó Mệnh đề 8 cho thấy rằng tồn tại một dãy hữu hạn duy nhất $(r_h)_{0 \leqslant h \leqslant k-1}$ sao cho $0 \leqslant r_h \leqslant b - 1$ với $0 \leqslant h \leqslant k - 1$ và
$$a = \sum_{h=0}^{k-1} r_h b^{k-h-1}.$$
Hơn nữa, ta phải có $r_0 > 0$, vì nếu không thì $a < b^{k-1}$ theo Mệnh đề 8. Biểu thức
$$\sum_{h=0}^{k-1} r_h b^{k-h-1}$$
được gọi là *khai triển theo cơ sở $b$* của số nguyên $a$.

\* Trong mọi phần của toán học không liên quan đến các phép tính số, Mệnh đề 8 chủ yếu hữu ích khi được áp dụng cho một số *nguyên tố* $b$. \*

Khi số nguyên $b$ đủ nhỏ để việc này là khả hành, ta có thể biểu diễn mỗi số nguyên $< b$ bằng một ký hiệu riêng biệt gọi là một *chữ số*. Các chữ số biểu diễn 0 và 1 thường là 0 và 1. Cho $a$ là một số nguyên và cho $\sum_{h=0}^{k-1} r_h b^{k-h-1}$ là khai triển của nó theo cơ sở $b$. Nếu số nguyên $k$ xuất hiện trong khai triển này đủ nhỏ để việc này là khả hành, thì thông thường ta liên kết với số nguyên $a$ dãy ký hiệu thu được bằng cách viết $r_0 r_1 \ldots r_{k-2} r_{k-1}$ từ trái sang phải rồi thay thế mỗi số nguyên $r_i$ bằng chữ số biểu diễn nó; ký hiệu thu được như vậy được gọi là *ký hiệu số* liên kết với $a$. Khi đó người ta thường thay thế $a$ bằng ký hiệu số của nó trong các thuật ngữ và quan hệ mà nó xuất hiện.

Ví dụ, nếu C, Q, F, D là các chữ số, thì các ký hiệu số CQ, CQF, CQFD lần lượt được liên kết với $\mathrm{C}b + \mathrm{Q}$, $\mathrm{C}b^2 + \mathrm{Q}b + \mathrm{F}$, $\mathrm{C}b^3 + \mathrm{Q}b^2 + \mathrm{F}b + \mathrm{D}$.

Suy ra từ Mệnh đề 8 rằng ký hiệu số liên kết với một số nguyên $a$ là duy nhất, và rằng nếu $a < b^k$ thì nó chứa nhiều nhất $k$ chữ số. Chú ý rằng ký hiệu số liên kết với số nguyên $b^k$ gồm chữ số 1 theo sau bởi $k$ chữ số 0.

Hệ biểu diễn các số nguyên bằng các ký hiệu số này được gọi là *hệ ghi số theo cơ sở $b$*. Trong các phép tính số thực hành, các hệ sau đây được dùng: (*a*) hệ cơ sở 2, hay *hệ nhị phân*, trong đó các chữ số là 0 và 1; (*b*) *hệ thập phân*, trong đó các

các chữ số là $0$, $1$, $2$, $3$, $4$, $5 = 4 + 1$, $6 = 5 + 1$, $7 = 6 + 1$, $8 = 7 + 1$, $9 = 8 + 1$, và trong đó $b$ là số nguyên $9 + 1$ (do đó ký hiệu số của nó trong hệ này là 10).

Kể từ thời Trung cổ, hệ thập phân theo truyền thống đã được dùng trong các phép tính số, và chúng tôi sẽ dùng nó trong bộ sách này mỗi khi cần viết tường minh một số nguyên. Chúng tôi dẫn người đọc tới phần của bộ sách này dành cho phép tính số để trình bày các phương pháp thu được các ký hiệu số liên kết với tổng, hiệu, tích và phần nguyên của thương của hai số nguyên khi biết các ký hiệu số của chúng.

### 8. GIẢI TÍCH TỔ HỢP

#### Mệnh đề 9 {#ens-iii-s5-prop-9 .statement tag=03M7}

*Cho* $\mathrm{E}$ *và* $\mathrm{F}$ *là hai tập hợp,* $\mathfrak{a}$ *và* $\mathfrak{b}$ *là các lực lượng của chúng,* $f$ *là một toàn ánh từ* $\mathrm{E}$ *lên* $\mathrm{F}$ *sao cho các tập hợp* $\overset{-1}{f}(y)$, *với* $y \in \mathrm{F}$, *đều có cùng lực lượng* $\mathfrak{c}$. *Khi đó* $\mathfrak{a} = \mathfrak{b}\mathfrak{c}$.

Thật vậy, họ $(\overset{-1}{f}(y))_{y \in \mathrm{F}}$ là một phân hoạch của $\mathrm{E}$, mà mỗi phần tử của phân hoạch đó là một tập hợp có lực lượng $\mathfrak{c}$; do đó suy ra kết quả (§ 3, no. 4, Mệnh đề 6, Hệ quả 2).

#### Định nghĩa 2 {#ens-iii-s5-def-2 .statement tag=03M8}

*Cho* $n$ *là một số nguyên.* *Tích* $\prod_{i < n} (i + 1)$ *được ký hiệu bởi* $n!$ (đọc là "giai thừa $n$").

Ta có $0! = 1$ (Chương II, § 5, no. 3) và $1! = 1$. Với mỗi số nguyên $n$ ta có $(n + 1)! = n!\,(n + 1)$. Quan hệ này, cùng với quan hệ $0! = 1$, đặc trưng số hạng $n!$, như dễ thấy bằng quy nạp theo $n$.

#### Mệnh đề 10 {#ens-iii-s5-prop-10 .statement tag=03M9}

*Cho* $m$ *và* $n$ *là các số nguyên sao cho* $m \leqslant n$. *Khi đó* $n!/(n - m)!$ *là số các ánh xạ đơn ánh từ một tập hợp* $\mathrm{A}$ *có* $m$ *phần tử vào một tập hợp* $\mathrm{B}$ *có* $n$ *phần tử.*

Phép chứng minh được thực hiện bằng quy nạp theo số $m \leqslant n$ các phần tử của $\mathrm{A}$. Nếu $m = 0$, kết quả là hiển nhiên. Giả sử rằng $m + 1 \leqslant n$. Cho $\mathrm{A}$ là một tập hợp có $m + 1$ phần tử, $\mathrm{A}'$ là một tập con của $\mathrm{A}$ có $m$ phần tử, và $\{a\} = \mathrm{A} - \mathrm{A}'$. Cho $\mathrm{F}$, $\mathrm{F}'$ lần lượt là các tập hợp các ánh xạ đơn ánh của $\mathrm{A}$, $\mathrm{A}'$ vào $\mathrm{B}$, và cho $\varphi$ là ánh xạ $f \to f\,|\mathrm{A}'$ biến mỗi hàm $f \in \mathrm{F}$ thành hạn chế của nó lên $\mathrm{A}'$. Với mỗi $f' \in \mathrm{F}'$, một phần tử $f$ của $\overset{-1}{\varphi}(f')$ được xác định duy nhất bởi giá trị $f(a)$ của nó; vì $f$ là đơn ánh, ta phải có $f(a) \in \mathrm{B} - f'(\mathrm{A}')$. Suy ra $\overset{-1}{\varphi}(f')$ có cùng số $n - m$ phần tử như $\mathrm{B} - f'(\mathrm{A}')$. Do đó, theo Mệnh đề 9, $\mathrm{F}$ có

$$(n - m)\,\frac{n!}{(n - m)!} = \frac{n!}{(n - m - 1)!}$$

phần tử theo giả thiết quy nạp. Điều này hoàn tất chứng minh.

#### Hệ quả {#ens-iii-s5-n8-cor-1 .statement tag=03MA}

*Số các hoán vị của một tập hợp hữu hạn có n phần tử bằng n!.*

Vì số này bằng số các đơn ánh của tập hợp vào chính nó (§ 4, no. 2, Mệnh đề 2, Hệ quả 4).

#### Mệnh đề 11 {#ens-iii-s5-prop-11 .statement tag=03MB}

*Cho* E *là một tập hợp hữu hạn có n phần tử, và cho* $(p_i)_{1 \leqslant i \leqslant h}$ *là một dãy hữu hạn các số nguyên sao cho* $\sum_{i=1}^{h} p_i = n$. *Khi đó số các phủ* $(X_i)_{1 \leqslant i \leqslant h}$ *của* E *bởi các tập hợp đôi một rời nhau* $X_i$ *sao cho* $\mathrm{Card}\,(X_i) = p_i$ *với* $1 \leqslant i \leqslant h$ *bằng*

$$n! \Big/ \prod_{i=1}^{h} p_i!.$$

Cho G là tập hợp các phép hoán vị của E và gọi P là tập hợp các phủ $(X_i)_{1 \leqslant i \leqslant h}$ thỏa mãn các điều kiện của Mệnh đề. Vì $\sum_{i=1}^{h} p_i = n$, P không rỗng. Lấy một phần tử $(A_i)_{1 \leqslant i \leqslant h}$ của P. Với mỗi phép hoán vị $f \in G$, họ $(f(A_i))_{1 \leqslant i \leqslant h}$ cũng lại thuộc P; ta ký hiệu nó bởi $\varphi(f)$. Với mỗi phần tử $(X_i)_{1 \leqslant i \leqslant h}$, hãy tính số các phép hoán vị $f \in G$ sao cho $\varphi(f) = (X_i)$. Ta có $\varphi(f) = (X_i)$ khi và chỉ khi với mỗi chỉ số $i$ ta có $f(A_i) = X_i$. Do đó tập hợp các phép hoán vị $f$ đang xét có cùng lực lượng với tích của các tập hợp các song ánh từ $A_i$ lên $X_i$ (Chương II, § 4, số 7, Mệnh đề 8); do đó tập hợp $\overset{-1}{\varphi}((X_i)_{1 \leqslant i \leqslant h})$ có $\prod_{i=1}^{h} p_i!$ phần tử (Hệ quả của Mệnh đề 10). Vì G có $n!$ phần tử, kết quả bây giờ suy ra từ Mệnh đề 9.

#### Hệ quả 1 {#ens-iii-s5-prop-11-cor-1 .statement tag=03MC}

*Cho* A *là một tập hợp có n phần tử và cho p là một số nguyên* $\leqslant n$. *Khi đó số các tập con của* A *có p phần tử là* $\dfrac{n!}{p!(n-p)!}$.

Đặt $h = 2$, $p_1 = p$, $p_2 = n - p$ trong Mệnh đề 11.

¶ Số các tập con chứa $p$ phần tử trong một tập hợp có $n$ phần tử (với $p \leqslant n$) được ký hiệu là $\begin{pmatrix} n \\ p \end{pmatrix}$ và được gọi là *hệ số nhị thức với các chỉ số n và p*. Từ quan hệ $\begin{pmatrix} n \\ p \end{pmatrix} = \dfrac{n!}{p!(n-p)!}$ suy ra ngay lập tức rằng $\begin{pmatrix} n \\ p \end{pmatrix} = \begin{pmatrix} n \\ n-p \end{pmatrix}$.

Điều này cũng là một hệ quả của sự kiện rằng, nếu E là một tập hợp có $n$ phần tử, $X \to E - X$ là một song ánh của tập hợp các tập con của E gồm $p$ phần tử lên tập hợp các tập con có $n - p$ phần tử.

Ta đặt $\binom{n}{p} = 0$ đối với mỗi cặp số nguyên tự nhiên sao cho $p > n$. Với quy ước này, số tập con gồm $p$ phần tử trong một tập hợp gồm $n$ phần tử là $\binom{n}{p}$ với *mọi* số nguyên tự nhiên $p$.

#### Hệ quả 2 {#ens-iii-s5-prop-11-cor-2 .statement tag=03RG}

*Cho* E *và* F *là các tập hợp hữu hạn được sắp thứ tự toàn phần có lần lượt* $p$ *và* $n$ *phần tử. Khi đó số các ánh xạ tăng ngặt từ* E *vào* F *là* $\binom{n}{p}$.

Thật vậy, một ánh xạ như thế là một đơn ánh từ E vào F (§ 1, số 12, Mệnh đề 11), và vì E và F được sắp tốt (§ 4, số 4, Hệ quả 1 của Mệnh đề 3), nên với mỗi tập con X gồm $p$ phần tử của F có đúng một ánh xạ tăng ngặt từ E lên X (§ 2, số 5, Định lý 3).

#### Mệnh đề 12 {#ens-iii-s5-prop-12 .statement tag=03RH}

*Với mỗi số nguyên* $n$, *ta có*

$$\sum_p \binom{n}{p} = 2^n.$$

Thật vậy, nếu E là một tập hợp gồm $n$ phần tử, thì vế trái của đẳng thức là số các tập con của E. Bây giờ áp dụng Mệnh đề 12 của § 3, số 5.

#### Mệnh đề 13 {#ens-iii-s5-prop-13 .statement tag=03RI}

*Nếu* $n$ *và* $p$ *là các số nguyên, thì*

$$\binom{n+1}{p+1} = \binom{n}{p+1} + \binom{n}{p}.$$

Cho E là một tập hợp có $n + 1$ phần tử, cho P là tập hợp tất cả các tập con của E chứa $p + 1$ phần tử, cho $a$ là một phần tử của E, và đặt

$$\mathrm{E}' = \mathrm{E} - \{a\}.$$

Gọi P′ (resp. P″) là tập hợp các tập con có $p + 1$ phần tử của E chứa $a$ (resp. không chứa $a$). Tập hợp P″ là tập hợp các tập con có $p + 1$ phần tử của E′ và do đó có $\binom{n}{p+1}$ phần tử. Ánh xạ $\mathrm{X} \to \mathrm{X} \cap \mathrm{E}'$ là một song ánh từ P′ lên tập hợp các tập con có $p$ phần tử của E′, và do đó P′ có $\binom{n}{p}$ phần tử. Kết quả nay suy ra từ việc P là hợp của hai tập hợp rời nhau P′ và P″.

Mệnh đề 13 cũng có thể được chứng minh bằng một phép tính đơn giản từ công thức $\binom{n}{p} = \dfrac{n!}{p!(n-p)!}$ với $p \leqslant n$.

#### Mệnh đề 14 {#ens-iii-s5-prop-14 .statement tag=03RJ}

*Cho* $n$ *là một số nguyên* $> 0$. *Khi đó số* $a_n$ (tương ứng $b_n$) *của các cặp có thứ tự* $(i, j)$ *gồm các số nguyên sao cho* $1 \leqslant i \leqslant j \leqslant n$ (tương ứng $1 \leqslant i < j \leqslant n$) *là* $\frac{1}{2}n(n+1)$ ((tương ứng $\frac{1}{2}n(n-1)$)).

Thật vậy, $b_n$ là số các tập con có 2 phần tử của $[1, n]$; do đó

$$b_n = \frac{n!}{2!(n-2)!} = \frac{1}{2} n(n-1).$$

Giá trị của $a_n$ được suy ra từ điều này bằng cách nhận thấy rằng tập hợp các cặp có thứ tự $(i, j)$ sao cho $1 \leqslant i \leqslant j \leqslant n$ là hợp của tập hợp các cặp có thứ tự $(i, j)$ sao cho $1 \leqslant i \leqslant j < n$ và tập hợp các cặp $(i, i)$ với $1 \leqslant i \leqslant n$. Do đó $a_n = n + b_n = \frac{1}{2} n(n+1)$.

#### Hệ quả {#ens-iii-s5-n8-cor-2 .statement tag=03RK}

*Với mỗi số nguyên $n > 0$, ta có*

$$\sum_{i=1}^{n} i = \frac{1}{2} n(n+1).$$

Trong tập hợp A gồm các cặp có thứ tự của các số nguyên $(i, j)$ sao cho $1 \leqslant i \leqslant j \leqslant n$, ký hiệu $A_k$ là tập con các cặp $(i, k)$, trong đó $1 \leqslant i \leqslant k$ (với một số nguyên tùy ý $k \leqslant n$). Khi đó $A_k$ có $k$ phần tử. Nhưng $(A_k)_{1 \leqslant k \leqslant n}$ là một phân hoạch của A; do đó có kết quả.

#### Mệnh đề 15 {#ens-iii-s5-prop-15 .statement tag=03RL}

*Cho $n$ và $h$ là các số nguyên và cho* E *là một tập hợp có $h$ phần tử. Khi đó số các ánh xạ $u$ từ* E *vào* $[0, n]$ *sao cho* $\sum_{x \in E} u(x) \leqslant n$ *(tương ứng,* $\sum_{x \in E} u(x) = n$, *với $h > 0$) là*

$$\binom{n+h}{h} \left( \text{resp.} \ \binom{n+h-1}{h-1} \right).$$

Ký hiệu $A(h, n)$ (tương ứng, $B(h, n)$) là số ánh xạ $u$ từ E vào $[0, n]$ sao cho $\sum_{x \in E} u(x) \leqslant n$ (tương ứng, $\sum_{x \in E} u(x) = n$ đối với $h > 0$). Trước hết ta chỉ ra rằng $A(h-1, n) = B(h, n)$. Để làm điều đó, lấy E′ là một tập con của E có $h - 1$ phần tử, và đặt $\{a\} = E - E'$. Nếu $u$ là một ánh xạ từ E vào $[0, n]$ sao cho $\sum_{x \in E} u(x) = n$, thì hạn chế $u'$ của nó trên E′ thỏa $\sum_{x \in E'} u'(x) \leqslant n$, và hơn nữa $u(a) = n - \sum_{x \in E'} u'(x)$. Ngược lại, mọi ánh xạ $u'$ từ E′ vào $[0, n]$ thỏa $\sum_{x \in E'} u'(x) \leqslant n$ xác định một ánh xạ duy nhất $u$ từ E vào $[0, n]$, mà $u'$ là hạn chế, và sao cho $\sum_{x \ni E} u(x) = n$.

Tiếp theo, ta chú ý rằng nếu $\sum_{x \in E} u(x) \leqslant n$, thì hoặc $\sum_{x \in E} u(x) = n$, hoặc $\sum_{x \in E} u(x) \leqslant n-1$, và hai khả năng này loại trừ lẫn nhau. Do đó

$$A(h, n) = A(h, n-1) + B(h, n) = A(h, n-1) + A(h-1, n).$$

Vì $A(0, 0) = 1 = \binom{0}{0}$, công thức $A(h, n) = \binom{n+h}{h}$ suy ra từ trên và từ Mệnh đề 13, bằng quy nạp theo $n + h$.

\* Số các đơn thức $X_1^{\alpha_1} X_2^{\alpha_2} \ldots X_h^{\alpha_n}$ theo $h$ biến bất định có bậc tổng $\leqslant n$ hiển nhiên bằng số các ánh xạ $i \rightarrow \alpha_i$ của $[1, h]$ vào $[0, n]$ sao cho $\sum_{i=0}^{h} \alpha_i \leqslant n$, và do đó bằng $\binom{n+h}{h}$ theo Mệnh đề 15; số này cũng là số các đơn thức theo $h + 1$ biến bất định có bậc tổng $n$. \*

### Bài tập {#ens-iii-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
