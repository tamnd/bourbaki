---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 6
section_title: Infinite sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 183-190, 241-251
pdf_pages: 0189-0196, 0247-0257
extraction: ocr
subsections:
    - "no": 1
      title: THE SET OF NATURAL INTEGERS
      page: 183
      pdf_page: 189
    - "no": 2
      title: DEFINITION OF MAPPINGS BY INDUCTION
      page: 184
      pdf_page: 190
    - "no": 3
      title: PROPERTIES OF INFINITE CARDINALS
      page: 186
      pdf_page: 192
    - "no": 4
      title: COUNTABLE SETS
      page: 188
      pdf_page: 194
    - "no": 5
      title: STATIONARY SEQUENCES
      page: 189
      pdf_page: 195
statements: 26
exercises: 32
content_sha256: 9cba3c267ad26368dfce8ac2a080224bdaaebd52c1b7e18b9d85140f7963fa6a
translated_from: content/en/ens/III/06_s6_infinite_sets.md
source_content_sha256: 223731a1f4d4b294c9f6780fefb0badacba82554ae1c93ebfea1fbb37a2e871a
translation_model: gpt-5.4, gpt-5.4-mini
translation_run: translate-vi-99f70c1a
glossary_version: 27
glossary_terms_sha256: 91b408418eeb74e0e285be7a733e1a055d0ac6174a65b52078af737c63c3bbdb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 6. TẬP HỢP VÔ HẠN

### 1. TẬP HỢP CÁC SỐ TỰ NHIÊN

#### Định nghĩa 1 {#ens-iii-s6-def-1 .statement tag=03MV}

*Một tập hợp được gọi là vô hạn nếu nó không hữu hạn.*

Đặc biệt, một lực lượng là vô hạn nếu nó không phải là một số nguyên.

Quan hệ "tồn tại một tập hợp vô hạn" kéo theo rằng quan hệ "$x$ là một số nguyên" là *xác định tập* (Chương II, § 1, no. 4); thật vậy, nếu $\mathfrak{a}$ là một lực lượng vô hạn và $n$ là một số nguyên tùy ý, thì không thể có $\mathfrak{a} \leqslant n$ (§ 4, no. 2, Mệnh đề 2). Do đó ta có $n < \mathfrak{a}$ đối với mọi số nguyên $n$, điều này cho thấy rằng tập hợp các số nguyên $< \mathfrak{a}$ (§ 3, no. 2, Nhận xét sau Định lý 1) chứa mọi số nguyên. Ngược lại, nếu quan hệ "$x$ là một số nguyên" là xác định tập, thì tập hợp E các số nguyên là một tập hợp *vô hạn*. Với mỗi số nguyên $n$, khoảng $[0, n]$ là một tập con gồm $n + 1$ phần tử của E (§ 5, no. 3, Mệnh đề 5). Do đó Card (E) $\geqslant n + 1 > n$. Nhưng nói rằng Card(E) $\neq n$ với mọi số nguyên $n$ có nghĩa là E là vô hạn.

¶ Bây giờ ta đưa vào tiên đề sau :

A5 ("Tiên đề vô hạn".) *Tồn tại một tập hợp vô hạn.*

Người ta chưa biết liệu tiên đề này có thể được suy ra hay không từ các tiên đề và các lược đồ tiên đề đã được đưa vào trước đây; mặc dù vấn đề này chưa được giải quyết dứt khoát, có thể giả định rằng tiên đề này độc lập với các tiên đề khác.

Các nhận xét trên khi ấy chứng minh định lý sau :

#### Định lý 1 {#ens-iii-s6-thm-1 .statement tag=03MW}

*Quan hệ "$x$ là một số nguyên" là xác định tập.*

Ta sẽ ký hiệu bởi $\mathbf{N}$ tập hợp các số nguyên (cũng được gọi là "tập hợp các số nguyên tự nhiên" khi cần thiết để tránh sự nhập nhằng). Lực lượng của $\mathbf{N}$ là

được ký hiệu bởi $\aleph_0$. Mỗi khi $\mathbf{N}$ được xét như một tập hợp có thứ tự, thì thứ tự được xét luôn luôn là thứ tự (gọi là thứ tự *thông thường*) được định nghĩa ở § 3, no. 2, trừ khi có phát biểu minh nhiên ngược lại.

#### Định nghĩa 2 {#ens-iii-s6-def-2 .statement tag=03MX}

*Một dãy* (tương ứng, *một dãy các phần tử của một tập hợp* E) *là một họ* (tương ứng, *một họ các phần tử của* E) *mà tập chỉ số là một tập con của* $\mathbf{N}$. *Dãy được gọi là vô hạn nếu tập chỉ số của nó là một tập con vô hạn của* $\mathbf{N}$.

Cho $\mathrm{P}\{n\}$ là một quan hệ và ký hiệu I là tập hợp các số nguyên $n$ sao cho $\mathrm{P}\{n\}$ đúng. Khi đó I là một tập con của $\mathbf{N}$. Một dãy $(x_n)_{n\in\mathrm{I}}$ khi đó đôi khi được viết $(x_n)_{\mathrm{P}\{n\}}$, và $x_n$ được gọi là *số hạng thứ n* trong dãy. Một dãy có tập chỉ số là tập các số nguyên $n \geqslant k$ thường được viết $(x_n)_{k \leqslant n}$ hoặc $(x_n)_{n \geqslant k}$, hoặc thậm chí chỉ $(x_n)$ nếu $k = 0$ hoặc $k = 1$. Dưới cùng các điều kiện ấy, chẳng hạn, các ký hiệu $\prod_{\mathrm{P}\{n\}} \mathrm{X}_n$ và $\prod_{n=k}^{\infty} \mathrm{X}_n$ được dùng để chỉ tích của một dãy các tập hợp $(\mathrm{X}_n)_{n\in\mathrm{I}}$, và có các ký hiệu tương tự cho các hợp, các giao, các tích lực lượng, và các tổng lực lượng.

Mọi họ con của một dãy là một dãy, gọi là một *dãy con* của dãy đã cho.

Hai dãy $(x_n)_{n\in\mathrm{I}}$, $(y_n)_{n\in\mathrm{I}}$ có cùng tập chỉ số được gọi là *chỉ khác nhau về thứ tự các phần tử của chúng* nếu tồn tại một phép hoán vị $f$ của tập chỉ số I sao cho $x_{f(n)} = y_n$ với mọi $n \in \mathrm{I}$.

Một *dãy bội* là một họ mà tập chỉ số của nó là một tập con của một tích $\mathbf{N}^p$ ($p$ là một số nguyên) ("dãy kép" khi $p = 2$, "dãy ba" khi $p = 3$, và cứ tiếp như vậy).

Let I là một tập đồng lực với $\mathbf{N}$ và cho $f$ là một song ánh từ $\mathbf{N}$ onto I. Với mỗi họ $(x_\iota)_{\iota\in\mathrm{I}}$ được chỉ số hóa bởi tập I, dãy $n \to x_{f(n)}$ được nói là thu được bằng *sắp xếp họ* $(x_\iota)_{\iota\in\mathrm{I}}$ *theo thứ tự được xác định bởi* $f$. Các dãy tương ứng theo cách này với hai song ánh khác nhau của $\mathbf{N}$ onto I chỉ khác nhau ở thứ tự các số hạng của chúng. Đối với một họ hữu hạn được chỉ số hóa bởi một tập I gồm $n$ phần tử, ta cũng có thể định nghĩa một dãy hữu hạn với $[1, n]$ hoặc $[0, n-1]$ làm tập chỉ số, bằng cách sắp xếp họ theo thứ tự được xác định bởi một song ánh của một trong hai khoảng này onto I.

### 2. ĐỊNH NGHĨA CÁC ÁNH XẠ BẰNG QUY NẠP

Vì tập $\mathbf{N}$ được sắp tốt, ta có thể áp dụng tiêu chuẩn C60 (§ 2, no. 2), tiêu chuẩn này lúc này có dạng sau (với cùng ký hiệu) :

C62. *Cho $u$ là một chữ và cho* $\mathrm{T}\{u\}$ *là một số hạng. Khi đó tồn tại một tập hợp* U *và một ánh xạ $f$ từ* $\mathbf{N}$ *lên* U *sao cho với mỗi số nguyên $n$ ta có* $f(n) = \mathrm{T}\{f^{(n)}\}$, *trong đó $f^{(n)}$ ký hiệu ánh xạ từ* $[0, n[$ *lên* $f([0, n[)$ *trùng với $f$ trên* $[0, n[$. *Hơn nữa, tập hợp* U *và ánh xạ $f$ được xác định duy nhất bởi điều kiện này.*

Từ đây ta sẽ suy ra tiêu chuẩn sau :

C63. *Cho* $S\{v\}$ *và* $a$ *là hai hạng. Khi đó tồn tại một tập hợp* $V$ *và một ánh xạ* $f$ *từ* $\mathbf{N}$ *lên* $V$ *sao cho* $f(0) = a$ *và* $f(n) = S\{f(n-1)\}$ *với mỗi số nguyên* $n \geqslant 1$. *Hơn nữa, tập hợp* $V$ *và ánh xạ* $f$ *được xác định duy nhất bởi các điều kiện này.*

*Để suy ra C63 từ C62 [^1], đặt*

$$D(u) = \mathcal{E}_x(x \in \mathbf{N} \ \text{và} \ (\exists y)((x, y) \in \mathrm{pr}_1(\mathrm{pr}_1(u))))$$

Với mỗi chữ $u$. Nếu $u$ là một ánh xạ của một tập con của $\mathbf{N}$ vào một tập hợp, thì $D(u)$ chính là miền xác định của $u$ (Chương II, § 3, số 1). Gọi $M(u)$ là cận trên bé nhất của $D(u)$ trong $\mathbf{N}$ [^2]. Gọi $\varphi$ là ánh xạ rỗng, với $\emptyset$ làm nguồn và đích, tức là (Chương II, § 3, các số 1 và 4), bộ ba $(\emptyset, \emptyset, \emptyset))$ và xét quan hệ

$$(u = \varphi \ \text{và} \ y = a) \ \text{hoặc} \ (u \neq \varphi \ \text{và} \ y = S\{u(M(u))\})$$

mà ta ký hiệu là $R\{y, u\}$ ; cuối cùng, đặt $T\{u\}$ là số hạng $\tau_y(R\{y, u\})$. Áp dụng C62 cho số hạng $T\{u\}$. Vì $f^{(0)}$ bằng $\varphi$, ta có $T\{f^{(0)}\} = a$; do đó $f(0) = a$. Mặt khác, nếu $n > 0$, ta có $D(f^{(n)}) = [0, n-1]$ và $M(f^{(n)}) = n-1$, do đó

$$T\{f^{(n)}\} = S\{f^{(n)}(n-1)\} = S\{f(n-1)\}.$$

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s6-n2-exa-1 .statement tag=03TC}

Giả sử $a$ là một phần tử của một tập hợp $E$ và $S\{u\}$ là số hạng $g(u)$, trong đó $g$ là một ánh xạ từ $E$ vào chính nó [^3]. Khi đó, bằng quy nạp theo $n$, người ta thấy ngay lập tức rằng với mọi $n \in \mathbf{N}$ ta có $f(n) \in E$; do đó $f$ là một ánh xạ từ $\mathbf{N}$ vào $E$ sao cho $f(0) = a$ và $f(n+1) = g(f(n))$ với mọi số nguyên $n$.

Tương tự, cho $h$ là một ánh xạ của $\mathbf{N} \times E$ vào $E$, và gọi $\psi$ là ánh xạ của $\mathbf{N} \times E$ vào chính nó được định nghĩa bởi $\psi(n, x) = (n+1, h(n, x))$. Theo thảo luận trước đó, tồn tại một ánh xạ duy nhất $g = (\theta, f)$ của $\mathbf{N}$ vào $\mathbf{N} \times E$ sao cho $g(0) = (0, a)$ và $g(n+1) = \psi(g(n))$ với mọi $n$, từ đó suy ra sự tồn tại và tính duy nhất của một ánh xạ $f$

của $\mathbf{N}$ vào E sao cho $f(0) = a$ và $f(n + 1) = h(n, f(n))$ với mọi số nguyên $n$.

#### Ví dụ 2 {#ens-iii-s6-n2-exa-2 .statement tag=03TD}

Cho X là một tập hợp và E là tập hợp các ánh xạ từ X vào chính nó. Ký hiệu $e$ là ánh xạ đồng nhất của X vào chính nó, và cho $f$ là một phần tử bất kỳ của E. Lấy $S\{u\}$ là số hạng $f \circ u$ (*)[^4]. Áp dụng C63, ta thấy rằng tồn tại một ánh xạ duy nhất của $\mathbf{N}$ vào E, được ký hiệu bởi $n \to f^n$, sao cho $f^0 = e$ và $f^{n+1} = f \circ f^n$. Ánh xạ $f^n$ được gọi là *lần lặp thứ n* của ánh xạ $f$.

#### Ví dụ 3 {#ens-iii-s6-n2-exa-3 .statement tag=03TE}

Nếu ta lấy $S\{u\}$ là số hạng $\mathfrak{P}(u)$, và $a$ là một tập hợp E, thì suy ra tương tự rằng tồn tại một ánh xạ, được ký hiệu bởi $n \to \mathfrak{P}^n(\mathrm{E})$, từ $\mathbf{N}$ vào một tập hợp V(E) sao cho $\mathfrak{P}^0(\mathrm{E}) = \mathrm{E}$, $\mathfrak{P}^1(\mathrm{E}) = \mathfrak{P}(\mathrm{E})$, và $\mathfrak{P}^{n+1}(\mathrm{E}) = \mathfrak{P}(\mathfrak{P}^n(\mathrm{E}))$ với mọi số nguyên $n$.

#### Nhận xét {#ens-iii-s6-n2-rem-1 .statement tag=03MY}

Cho E là một tập hợp, cho A là một tập con của E, cho $g$ là một ánh xạ từ A vào E, và cho $a$ là một phần tử của A. Lấy $S\{u\}$ là số hạng $g(u)$. Tiêu chuẩn C63 áp dụng được và chứng minh sự tồn tại của một ánh xạ $f$ của $\mathbf{N}$ lên một tập hợp V sao cho $f(0) = a$ và $f(n + 1) = g(f(n))$ với mọi số nguyên $n$. Có thể xảy ra rằng $\mathrm{V} \subset \mathrm{A}$; nếu không, cho $p$ là số nguyên lớn nhất sao cho $f([0, p]) \subset \mathrm{A}$. Khi đó $f(p + 1) = g(p) \notin \mathrm{A}$, và $g(g(p))$ là một số hạng về đó không có gì có thể nói được. Do đó trong trường hợp này $f$ được xem là chỉ được định nghĩa trên khoảng $[0, p + 1]$ ("quy nạp hạn chế").

### 3. TÍNH CHẤT CỦA CÁC BẢN SỐ VÔ HẠN

#### Định lý 2 {#ens-iii-s6-thm-2 .statement tag=03MZ}

*Với mọi bản số vô hạn $\mathfrak{a}$ ta có $\mathfrak{a}^2 = \mathfrak{a}$.*

Ta sẽ dùng hai bổ đề sau :

#### Bổ đề 1 {#ens-iii-s6-lem-1 .statement tag=03N0}

*Mọi tập vô hạn E đều chứa một tập đẳng lực với $\mathbf{N}$.*

Tồn tại một quan hệ sắp tốt trên E (§ 2, no. 3, Định lý 1), mà ta sẽ ký hiệu bởi $x \leqslant y$. Giả thiết kéo theo rằng tập được sắp thứ tự tốt E không thể đẳng cấu với một đoạn của $\mathbf{N}$ phân biệt với $\mathbf{N}$, vì một đoạn như thế có dạng $[0, n]$ (§ 2, no. 1, Mệnh đề 1) và do đó là hữu hạn. Suy ra $\mathbf{N}$ đẳng cấu với một đoạn của E (§ 2, no. 3, Định lý 3), do đó có kết quả phải chứng minh.

#### Bổ đề 2 {#ens-iii-s6-lem-2 .statement tag=03N1}

*Tập $\mathbf{N} \times \mathbf{N}$ đẳng lực với $\mathbf{N}$.*

Vì $\mathbf{N} \times \mathbf{N}$ chứa tập hợp $\{0\} \times \mathbf{N}$, là đẳng lực với $\mathbf{N}$, nên ta có $\mathrm{Card}(\mathbf{N}) \leqslant \mathrm{Card}(\mathbf{N} \times \mathbf{N})$. Để hoàn tất chứng minh, chỉ cần định nghĩa một đơn ánh $f$ của $\mathbf{N} \times \mathbf{N}$ vào $\mathbf{N}$. Vì mục đích này, ta chú ý rằng

tồn tại một đơn ánh $\varphi$ từ $\mathbf{N}$ vào tập hợp các ánh xạ từ $\mathbf{N}$ vào $\mathrm{I} = \{0, 1\}$, được cho như sau : nếu $r$ là số nguyên nhỏ nhất sao cho $n > 2^r$, và nếu $\sum_{k=0}^{r-1} \varepsilon_k 2^{r-k-1}$ là khai triển nhị phân của $n$ (§ 5, no. 7), thì $\varphi(n)$ được định nghĩa là dãy $(u_m)_{m \in \mathbf{N}}$ sao cho $u_m = \varepsilon_{r-m-1}$ với $m < r$ và $u_m = 0$ với $m \geqslant r$. Mệnh đề 8 của § 5, no. 7 cho thấy rằng $\varphi$ là đơn ánh. Với mỗi cặp $(n, n') \in \mathbf{N} \times \mathbf{N}$ ta định nghĩa $f(n, n')$ như sau : nếu $\varphi(n) = (u_m)$ và $\varphi(n') = (v_m)$, thì đặt $f(n, \; n')$ là số nguyên $s$ sao cho $\varphi(s) = w_m$, trong đó $w_{2m} = u_m$ và $w_{2m+1} = v_m$ với mọi $m \in \mathbf{N}$. Rõ ràng quan hệ $f(n, \; n') = f(n_1, \; n_1')$ kéo theo $\varphi(n) = \varphi(n_1)$ và $\varphi(n') = \varphi(n_1')$; do đó $(n, n') = (n_1, n_1')$, và vì vậy $f$ là đơn ánh.

¶ Bây giờ ta chuyển sang chứng minh Định lý 2. Cho E là một tập hợp sao cho $\mathrm{Card}(\mathrm{E}) = \mathfrak{a}$. Lấy D là một tập con của E có cùng lực lượng với $\mathbf{N}$ (Bổ đề 1). Khi đó tồn tại một song ánh $\psi_0$ từ D lên $\mathrm{D} \times \mathrm{D}$ (Bổ đề 2). Gọi $\mathfrak{M}$ là tập hợp các cặp $(\mathrm{X}, \psi)$, trong đó X là một tập con của E chứa D và $\psi$ là một song ánh từ X lên $\mathrm{X} \times \mathrm{X}$ mở rộng $\psi_0$. Sắp thứ tự tập hợp $\mathfrak{M}$ bằng quan hệ

$$\text{``} \mathrm{X} \subset \mathrm{X}' \text{ và } \psi' \text{ là một mở rộng của } \psi \text{''}$$

giữa $(\mathrm{X}, \psi)$ và $(\mathrm{X}', \psi')$. Khi đó thấy ngay rằng $\mathfrak{M}$ là *quy nạp* (xem § 2, no. 4, Ví dụ 2). Vì thế, theo Bổ đề Zorn (§ 2, no. 4, Định lý 2), $\mathfrak{M}$ có một phần tử cực đại $(\mathrm{F}, f)$. Ta sẽ chứng minh rằng $\mathrm{Card}\,(\mathrm{F}) = \mathfrak{a}$, điều này sẽ đủ để chứng minh định lý. Nếu $\mathrm{Card}\,(\mathrm{F})$ không bằng $\mathfrak{a}$, thì đặt $\mathrm{Card}\,(\mathrm{F}) = \mathfrak{b} < \mathfrak{a}$. Khi đó $\mathfrak{b} = \mathfrak{b}^2$ và $\mathfrak{b}$ vô hạn, và $\mathfrak{b} \leqslant 2\mathfrak{b} \leqslant 3\mathfrak{b} \leqslant \mathfrak{b}^2 = \mathfrak{b}$ (§ 3, no. 6, Mệnh đề 14); do đó $2\mathfrak{b} = \mathfrak{b}$ và $3\mathfrak{b} = \mathfrak{b}$. Từ giả thiết $\mathfrak{b} < \mathfrak{a}$ suy ra $\mathrm{Card}\,(\mathrm{E} - \mathrm{F}) > \mathfrak{b}$, vì nếu không ta sẽ có $\mathrm{Card}\,(\mathrm{E}) \leqslant 2\mathfrak{b} = \mathfrak{b}$, và ta đã giả thiết rằng $\mathfrak{b} < \mathrm{Card}\,(\mathrm{E})$. Do đó tồn tại một tập con $\mathrm{Y} \subset \mathrm{E} - \mathrm{F}$ đẳng lực với F. Đặt $\mathrm{Z} = \mathrm{F} \cup \mathrm{Y}$; ta sẽ chứng minh rằng tồn tại một song ánh $g$ của Z lên $\mathrm{Z} \times \mathrm{Z}$ mở rộng $f$. Ta có

$$\mathrm{Z} \times \mathrm{Z} = (\mathrm{F} \times \mathrm{F}) \cup (\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y}),$$

và bốn tích ở vế phải đôi một rời nhau. Vì F và Y có cùng lực lượng, ta có

$$\mathrm{Card}(\mathrm{F} \times \mathrm{Y}) = \mathrm{Card}(\mathrm{Y} \times \mathrm{F}) = \mathrm{Card}(\mathrm{Y} \times \mathrm{Y}) = \mathfrak{b}^2 = \mathfrak{b},$$

do đó

$$\mathrm{Card}((\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y})) = 3\mathfrak{b} = \mathfrak{b}.$$

Vì thế tồn tại một song ánh $f_1$ từ Y lên tập hợp

$$(\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y});$$

ánh xạ $g$ của Z vào Z $\times$ Z, bằng $f$ trên F và bằng $f_1$ trên Y, do đó là một song ánh mở rộng $f$, trái với định nghĩa của $f$. Suy ra $\mathrm{Card}(\mathrm{F}) = \mathfrak{a}$, và chứng minh hoàn tất.

#### Hệ quả 1 {#ens-iii-s6-thm-2-cor-1 .statement tag=03N2}

*Nếu $\mathfrak{a}$ là một lực lượng vô hạn, thì $\mathfrak{a}^n = \mathfrak{a}$ với mọi số nguyên $n \geqslant 1$.*

Bằng quy nạp theo $n$.

#### Hệ quả 2 {#ens-iii-s6-thm-2-cor-2 .statement tag=03N3}

*Tích của một họ hữu hạn các lực lượng khác không $(\mathfrak{a}_i)_{i \in \mathrm{I}}$, trong đó lực lượng lớn nhất là một bản số vô hạn $\mathfrak{a}$, bằng $\mathfrak{a}$.*

Ký hiệu $\mathfrak{b}$ là tích ấy và gọi $n$ là số phần tử của I. Khi đó $\mathfrak{b} \leqslant \mathfrak{a}^n = \mathfrak{a}$ (§ 3, no. 6, Mệnh đề 14). Mặt khác, vì $\mathfrak{a}_i \geqslant 1$ với mọi $i \in \mathrm{I}$, nên ta có $\mathfrak{b} \geqslant \mathfrak{a}$ (§ 3, no. 6, Mệnh đề 14).

#### Hệ quả 3 {#ens-iii-s6-thm-2-cor-3 .statement tag=03N4}

*Cho $\mathfrak{a}$ là một lực lượng vô hạn và cho $(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ là một họ các lực lượng $\leqslant \mathfrak{a}$ có tập chỉ số I mang một lực lượng $\leqslant \mathfrak{a}$. Khi đó $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \leqslant \mathfrak{a}$; và nếu $\mathfrak{a}_\iota = \mathfrak{a}$ đối với ít nhất một chỉ số $\iota \in \mathrm{I}$, thì $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \mathfrak{a}$.*

Cho $\mathfrak{b}$ là lực lượng của I; khi đó ta có $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \leqslant \mathfrak{a}\mathfrak{b} \leqslant \mathfrak{a}^2 = \mathfrak{a}$ (§ 3, số 6, Mệnh đề 14), và $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \geqslant \mathfrak{a}_\varkappa$ với mọi $\varkappa \in \mathrm{I}$.

#### Hệ quả 4 {#ens-iii-s6-thm-2-cor-4 .statement tag=03N5}

*Nếu $\mathfrak{a}$ và $\mathfrak{b}$ là hai lực lượng khác không, trong đó một lực lượng là vô hạn, thì ta có $\mathfrak{a}\mathfrak{b} = \mathfrak{a} + \mathfrak{b} = \sup\,(\mathfrak{a},\,\mathfrak{b})$.*

Điều này suy ra trực tiếp từ các Hệ quả 2 và 3.

### 4. CÁC TẬP ĐẾM ĐƯỢC

#### Định nghĩa 3 {#ens-iii-s6-def-3 .statement tag=03N6}

*Một tập hợp được gọi là đếm được nếu nó đẳng lực với một tập con của tập* $\mathbf{N}$ *các số nguyên.*

#### Mệnh đề 1 {#ens-iii-s6-prop-1 .statement tag=03N7}

*Mọi tập con của một tập đếm được đều đếm được. Tích của một họ hữu hạn các tập đếm được là đếm được. Hợp của một dãy các tập đếm được là đếm được.*

Mệnh đề thứ nhất là hiển nhiên. Các mệnh đề kia suy ra từ các Hệ quả của Định lý 2, số 3.

¶ Chúng ta đã chứng minh (số 3, Bổ đề 1) rằng nếu $\mathfrak{a}$ là một bản số vô hạn bất kỳ, thì $\mathrm{Card}(\mathbf{N}) \leqslant \mathfrak{a}$. Điều này có các hệ quả sau:

#### Mệnh đề 2 {#ens-iii-s6-prop-2 .statement tag=03N8}

*Mọi tập vô hạn đếm được E đều đẳng lực với* $\mathbf{N}$.

Vì $\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathbf{N})$ theo định nghĩa; và $\mathrm{Card}(\mathbf{N}) \leqslant \mathrm{Card}(\mathrm{E})$ vì E là vô hạn.

#### Mệnh đề 3 {#ens-iii-s6-prop-3 .statement tag=03N9}

*Mọi tập vô hạn đều có một phân hoạch* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *gồm các tập vô hạn đếm được* $\mathrm{X}_\iota$, *tập chỉ số* I *đẳng lực với* E.

Vì $\mathrm{Card}(\mathrm{E}) = \mathrm{Card}(\mathrm{E})\ \mathrm{Card}(\mathbf{N})$ (số 3, Định lý 2, Hệ quả 4).

#### Mệnh đề 4 {#ens-iii-s6-prop-4 .statement tag=03NA}

*Cho* $f$ *là một ánh xạ từ một tập* E *lên một tập vô hạn* F *sao cho, với mỗi* $y \in \mathrm{F}$, $\overset{-1}{f}(y)$ *là đếm được. Khi đó* F *đẳng lực với* E.

Vì các tập $\overset{-1}{f}(y)$ $(y \in \mathrm{F})$ lập thành một phân hoạch của E; do đó

$$\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathrm{F})\mathrm{Card}(\mathbf{N}) = \mathrm{Card}(\mathrm{F}),$$

và $\mathrm{Card}(\mathrm{F}) \leqslant \mathrm{Card}(\mathrm{E})$ theo Mệnh đề 3 của § 3, no. 2.

#### Mệnh đề 5 {#ens-iii-s6-prop-5 .statement tag=03NB}

*Tập hợp* $\mathfrak{F}(\mathrm{E})$ *các tập con hữu hạn của một tập vô hạn* E *có cùng lực lượng với* E.

Với mỗi số nguyên $n$, ký hiệu $\mathfrak{F}_n$ là tập hợp các tập con của E có $n$ phần tử. Với mỗi $\mathrm{X} \in \mathfrak{F}_n$ tồn tại một song ánh từ $[1, n]$ lên X. Do đó lực lượng của $\mathfrak{F}_n$ nhiều nhất bằng lực lượng của tập hợp các ánh xạ từ $[1, n]$ vào E, tức là bằng $\mathrm{Card}(\mathrm{E}^n) = \mathrm{Card}(\mathrm{E})$ (no. 3, Định lý 2, Hệ quả 1). Vì vậy

$$\mathrm{Card}(\mathfrak{F}(\mathrm{E})) = \sum_{n \in \mathbf{N}} \mathrm{Card}(\mathfrak{F}_n) \leqslant \mathrm{Card}(\mathrm{E})\mathrm{Card}(\mathbf{N}) = \mathrm{Card}(\mathrm{E}).$$

Mặt khác, vì $x \to \{x\}$ là một ánh xạ đơn ánh từ E vào $\mathfrak{F}(\mathrm{E})$, nên ta có $\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathfrak{F}(\mathrm{E}))$.

#### Định nghĩa 4 {#ens-iii-s6-def-4 .statement tag=03NC}

*Một tập hợp được gọi là có lũy thừa của liên tục nếu nó có cùng lực lượng với tập hợp tất cả các tập con của* $\mathbf{N}$.

Một tập hợp có lũy thừa của liên tục thì không đếm được (§ 3, no. 6, Định lý 2).

\* Tên gọi "lực lượng của liên tục" xuất phát từ तथ्य rằng tập hợp các số thực đẳng lực với $\mathfrak{P}(\mathbf{N})$ (*Tôpô tổng quát*, Chương IV, § 8). ⁎ *Giả thuyết liên tục* là mệnh đề rằng mọi tập hợp không đếm được đều chứa một tập con có lực lượng của liên tục; *giả thuyết liên tục tổng quát* là mệnh đề rằng, với mọi lực lượng vô hạn $\mathfrak{a}$, mọi lực lượng $> \mathfrak{a}$ đều là $\geqslant 2^{\mathfrak{a}}$.

### 5. CÁC DÃY DỪNG

#### Định nghĩa 5 {#ens-iii-s6-def-5 .statement tag=03ND}

*Một dãy* $(x_n)_{n \in \mathbf{N}}$ *gồm các phần tử của một tập hợp* E *được gọi là dừng nếu tồn tại một số nguyên* $m$ *sao cho* $x_n = x_m$ *đối với mọi số nguyên* $n \geqslant m$.

#### Mệnh đề 6 {#ens-iii-s6-prop-6 .statement tag=03NE}

*Cho* E *là một tập hợp có thứ tự. Khi đó các mệnh đề sau tương đương :*

(a) *Mọi tập con không rỗng của* E *đều có một phần tử cực đại.*
(b) *Mọi dãy tăng* $(x_n)$ *gồm các phần tử của* E *đều dừng.*

Trước hết ta chứng minh rằng (a) suy ra (b). Gọi X là tập hợp các phần tử của dãy $(x_n)$, và gọi $x_m$ là một phần tử cực đại của X. Nếu $n \geqslant m$, thì theo giả thiết ta có $x_n \geqslant x_m$, và do đó $x_n = x_m$ theo tính cực đại của $x_m$. Ngược lại, giả sử tồn tại một tập con không rỗng A của E không có phần tử cực đại. Với mỗi $x \in A$, gọi $T_x$ là tập hợp всех $y \in A$ sao cho $y > x$. Theo giả thiết, $T_x \neq \emptyset$ với mọi $x \in A$; do đó tồn tại một ánh xạ $f$ từ A vào A sao cho $f(x) > x$ với mọi $x \in A$ (Chương II, § 5, no. 4, Mệnh đề 6). Nếu $a \in A$, thì dãy $(x_n)_{n \in \mathbf{N}}$ được định nghĩa bằng quy nạp bởi các điều kiện $x_0 = a$, $x_{n+1} = f(x_n)$ hiển nhiên là tăng và không dừng.

#### Hệ quả 1 {#ens-iii-s6-prop-6-cor-1 .statement tag=03NF}

*Một tập sắp thứ tự toàn phần* E *được sắp tốt nếu và chỉ nếu mọi dãy giảm các phần tử của* E *đều dừng.*

Thật vậy, nói rằng E được sắp tốt tương đương với nói rằng mọi tập con không rỗng của E đều có một phần tử cực tiểu (§ 1, no. 10, Mệnh đề 10), và do đó mệnh đề này suy ra từ Mệnh đề 6.

#### Hệ quả 2 {#ens-iii-s6-prop-6-cor-2 .statement tag=03NG}

*Mọi dãy tăng các phần tử của một tập có thứ tự hữu hạn đều dừng.*

Thật vậy, mọi tập có thứ tự hữu hạn đều có một phần tử cực đại (§ 4, no. 4, Mệnh đề 3, Hệ quả 2).

¶ Một tập có thứ tự E thỏa mãn các điều kiện tương đương của Mệnh đề 6 đôi khi được gọi là *Noether*.

#### Mệnh đề 7 ("Nguyên lý quy nạp Noether") {#ens-iii-s6-prop-7 .statement tag=03RM}

— *Cho* E *là một tập Noether, và cho* F *là một tập con của* E *có tính chất sau: nếu* $a \in E$ *sao cho quan hệ* $x > a$ *suy ra* $x \in F$, *thì* $a \in F$. *Trong các điều kiện đó,* F $=$ E.

Thật vậy, giả sử E $\neq$ F; khi đó E $-$ F có một phần tử cực đại $b$. Theo định nghĩa ta có $x \in F$ với mọi $x > b$; nhưng điều này suy ra $b \in F$, điều vô lý.

### Bài tập {#ens-iii-s6-exercises}

Xem [các bài tập của § 6](exercises/s6/).

[^1]: (*) Cũng có thể đưa ra một chứng minh trực tiếp cho C63, tương tự như chứng minh của C60 (§ 2, no. 2).
[^2]: (†) Định nghĩa của cận trên bé nhất (§ 1, nos. 7, 8, and 9) có thể được phát biểu theo cách sao cho nó có nghĩa ngay cả đối với một tập hợp không bị chặn trên (nó ký hiệu một số hạng, trong ngôn ngữ hình thức hóa, có dạng $\tau_x(R\{x\})$, mà người đọc sẽ không gặp khó khăn gì để viết ra).
[^3]: (**) Nếu $g = (G, E, E)$, số hạng $g(u)$ là số hạng được ký hiệu bởi $\tau_y((u, y) \in G)$.
[^4]: (*) Ở đây chúng tôi muốn nói số hạng được ký hiệu bởi (T, X, X), trong đó T là số hạng được ký hiệu bởi $\mathfrak{S}_z(z$ là một cặp có thứ tự và $(\exists y)((\mathrm{pr}_1 z, y) \in \mathrm{pr}_1(\mathrm{pr}_1(u))$ và $(y, \mathrm{pr}_2 z) \in \mathrm{pr}_1(\mathrm{pr}_1(f)))$.
