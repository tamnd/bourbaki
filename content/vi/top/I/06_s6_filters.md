---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 6
section_title: Filters
lang: vi
source: top-i-iv
pdf_pages: 0063-0074, 0135-0138
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A FILTER
      page: 0
      pdf_page: 63
    - "no": 2
      title: COMPARISON OF FILTERS
      page: 0
      pdf_page: 64
    - "no": 3
      title: BASES OF A FILTER
      page: 0
      pdf_page: 65
    - "no": 4
      title: ULTRAFILTERS
      page: 0
      pdf_page: 66
    - "no": 5
      title: INDUCED FILTER
      page: 0
      pdf_page: 67
    - "no": 6
      title: DIRECT IMAGE AND INVERSE IMAGE OF A FILTER BASE
      page: 0
      pdf_page: 68
    - "no": 7
      title: PRODUCT OF FILTERS
      page: 0
      pdf_page: 69
    - "no": 8
      title: ELEMENTARY FILTERS
      page: 0
      pdf_page: 70
    - "no": 9
      title: GERMS WITH RESPECT TO A FILTER
      page: 0
      pdf_page: 71
    - "no": 10
      title: GERMS AT A POINT
      page: 0
      pdf_page: 74
statements: 30
exercises: 20
content_sha256: 1d0c0d80386725a7710ec3c1a9ceaef14b7c50930bc26348bdd10edaada8bfab
translated_from: content/en/top/I/06_s6_filters.md
source_content_sha256: e428657ce0845aa0620d75cac8c82afb983dbc997f2fca66c06d22631b1480b9
translation_model: gpt-5-6-mini
translation_run: translate-vi-43b6c5e6
glossary_version: 34
glossary_terms_sha256: a27e1f701b347659f9e7e0f1edb4039ee71e6c292ce56b8687874e88903544e8
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 6. BỘ LỌC

### 1. ĐỊNH NGHĨA MỘT BỘ LỌC

#### Định nghĩa 1 {#top-i-s6-def-1 .statement}

*Một bộ lọc trên một tập hợp $X$ là một tập hợp $\mathfrak{F}$ gồm các tập con của $X$ có các tính chất sau:*

$(\mathrm{F}_1)$ *Mọi tập con của $X$ chứa một tập hợp của $\mathfrak{F}$ đều thuộc $\mathfrak{F}$.*
$(\mathrm{F}_\mathrm{II})$ *Mọi giao hữu hạn của các tập hợp của $\mathfrak{F}$ đều thuộc $\mathfrak{F}$.*
$(\mathrm{F}_\mathrm{III})$ *Tập rỗng không thuộc $\mathfrak{F}$.*

Suy ra từ $(\mathrm{F}_\mathrm{II})$ và $(\mathrm{F}_\mathrm{III})$ rằng mọi giao hữu hạn của các tập hợp của $\mathfrak{F}$ đều *không rỗng*.

Một bộ lọc $\mathfrak{F}$ trên $X$ xác định một cấu trúc trên $X$, các tiên đề của nó là $(\mathrm{F}_1)$, $(\mathrm{F}_\mathrm{II})$ và $(\mathrm{F}_\mathrm{III})$; cấu trúc này được gọi là một *cấu trúc của tập hợp được lọc*, và tập hợp $X$ được trang bị cấu trúc này được gọi là một *tập hợp được lọc bởi* $\mathfrak{F}$.

Tiên đề $(\mathrm{F}_\mathrm{II})$ tương đương với phép hội của hai tiên đề sau:
$(\mathrm{F}_{\mathrm{II}\,\mathrm{a}})$ *Giao của hai tập hợp của $\mathfrak{F}$ thuộc $\mathfrak{F}$.*
$(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ *$X$ thuộc $\mathfrak{F}$.*

Các tiên đề $(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ và $(\mathrm{F}_\mathrm{III})$ cho thấy rằng *không có bộ lọc nào trên tập rỗng*.

Để một tập hợp các tập con thỏa mãn $(\mathrm{F}_1)$ cũng thỏa mãn $(\mathrm{F}_{\mathrm{II}\,\mathrm{b}})$ thì điều kiện cần và đủ là nó *không rỗng*. Một tập hợp các tập con thỏa mãn $(\mathrm{F}_1)$ cũng thỏa mãn $(\mathrm{F}_\mathrm{III})$ khi và chỉ khi nó khác $\mathcal{P}(X)$.

*Các ví dụ về bộ lọc.* 1) Nếu $X \neq \varnothing$, tập hợp các tập con gồm riêng $X$ là một bộ lọc trên $X$. Tổng quát hơn, tập hợp tất cả các tập con của $X$ chứa một tập con khác rỗng cho trước $A$ của $X$ là một bộ lọc trên $X$.

2) Trong một không gian tôpô $X$, *tập hợp tất cả các lân cận* của một tập con tùy ý khác rỗng $A$ của $X$ (và đặc biệt là tập hợp tất cả các lân cận của một điểm của $X$) là một bộ lọc, được gọi là *bộ lọc lân cận* của $A$.

3) Nếu $X$ là một *tập hợp vô hạn*, *các phần bù của các tập con hữu hạn* của $X$ là các phần tử của một bộ lọc. Bộ lọc các phần bù của các tập con hữu hạn của tập hợp $\mathbf{N}$ các số nguyên $\geqslant 0$ được gọi là *bộ lọc Fréchet*.

### 2. SO SÁNH CÁC BỘ LỌC

#### Định nghĩa 2 {#top-i-s6-def-2 .statement}

Cho hai lọc $\mathfrak{F}, \mathfrak{F}'$ trên cùng một tập hợp $X$, ta nói $\mathfrak{F}'$ mịn hơn $\mathfrak{F}$, hoặc $\mathfrak{F}$ thô hơn $\mathfrak{F}'$, nếu $\mathfrak{F} \subset \mathfrak{F}$. Nếu còn có $\mathfrak{F} \neq \mathfrak{F}'$, thì ta nói $\mathfrak{F}'$ mịn hơn thực sự $\mathfrak{F}$, hoặc $\mathfrak{F}$ thô hơn thực sự $\mathfrak{F}'$.

Hai lọc được gọi là so sánh được nếu một lọc mịn hơn lọc kia. Tập hợp tất cả các lọc trên $X$ được sắp thứ tự bởi quan hệ " $\mathfrak{F}$ thô hơn $\mathfrak{F}'$"; quan hệ này được cảm sinh bởi quan hệ bao hàm trong $\mathcal{P}(\mathcal{P}(X))$.

Cho $(\mathfrak{F}_i)_{i \in I}$ là một họ không rỗng bất kỳ các lọc trên một tập hợp $X$ (do đó phải là không rỗng); khi đó tập hợp

$$
\mathfrak{F} = \bigcap_{i \in I} \mathfrak{F}_i
$$

thỏa mãn các tiên đề $(F_I), (F_{II})$ và $(F_{III})$ và do đó là một lọc; $\mathfrak{F}$ được gọi là giao của họ các lọc $(\mathfrak{F}_i)_{i \in I}$ và hiển nhiên là cận dưới lớn nhất của tập hợp các $\mathfrak{F}_i$ trong tập hợp có thứ tự của tất cả các lọc trên $X$.

Lọc được tạo bởi tập hợp duy nhất $X$ là phần tử nhỏ nhất của tập hợp có thứ tự của tất cả các lọc. Ta sẽ thấy ở no. 4 rằng, nếu $X$ có nhiều hơn một phần tử, tập hợp tất cả các lọc trên $X$ không có phần tử lớn nhất.

Cho một tập hợp $\mathcal{G}$ các tập con của một tập hợp $X$, ta hãy xét xem có những lọc nào trên $X$ chứa $\mathcal{G}$ hay không. Nếu tồn tại một lọc như vậy thì theo $(F_{II})$ nó cũng chứa tập hợp $\mathcal{G}'$ gồm các giao hữu hạn của các tập hợp của $\mathcal{G}$ (bao gồm $X$, là giao của tập con rỗng của $\mathcal{G}$); do đó điều kiện cần để một lọc như vậy tồn tại là tập con rỗng của $X$ không thuộc $\mathcal{G}'$. Điều kiện này cũng đủ, vì theo $(F_I)$ mọi lọc chứa $\mathcal{G}'$ cũng chứa tập hợp $\mathcal{G}''$ gồm các tập con của $X$ chứa một tập hợp của $\mathcal{G}'$. Hiện nay $\mathcal{G}''$ rõ ràng thỏa mãn $(F_I)$; nó thỏa mãn $(F_{II})$ do định nghĩa của $\mathcal{G}'$; và cuối cùng nó thỏa mãn $(F_{III})$ vì tập con rỗng của $X$ không thuộc $\mathcal{G}'$. Vậy $\mathcal{G}''$ là lọc thô nhất chứa $\mathcal{G}$, và ta đã chứng minh:

#### Mệnh đề 1 {#top-i-s6-prop-1 .statement}

Một điều kiện cần và đủ để tồn tại một lọc trên $X$ chứa một tập hợp $\mathcal{G}$ các tập con của $X$ là không có tập con hữu hạn nào của $\mathcal{G}$ có giao rỗng.

Bộ lọc $\mathcal{G}''$ được định nghĩa ở trên được nói là được sinh bởi $\mathcal{G}$, và $\mathcal{G}$ được nói là một cơ sở con của $\mathcal{G}''$.

#### Ví dụ {#top-i-s6-n2-exa-1 .statement}

Cho $\mathcal{S}$ là một tập hợp bất kỳ các tập con của một tập hợp $X$, và cho $\mathcal{T}$ là tôpô trên $X$ được sinh bởi $\mathcal{S}$ ($\S$ 2, no. 3, Ví dụ II). Vì tập hợp các giao hữu hạn của các tập hợp của $\mathcal{S}$ là một cơ sở của $\mathcal{T}$, nên suy ra từ chứng minh của Mệnh đề 1 ở trên và từ Mệnh đề 3 của $\S$ 1, no. 3 rằng với mỗi x \in X \text{ bộ lọc lân cận của } x \text{ đối với } \mathcal{T} \text{ được sinh bởi tập hợp } \mathcal{G}(x) \text{ gồm các tập hợp của } \mathcal{S} \text{ chứa } x.

#### Hệ quả 1 {#top-i-s6-prop-1-cor-1 .statement}

Cho $\mathfrak{F}$ là một bộ lọc trên một tập hợp $X$, và $A$ là một tập con của $X$. Khi đó tồn tại một bộ lọc $\mathfrak{F}'$ mịn hơn $\mathfrak{F}$ và sao cho $A \in \mathfrak{F}'$, khi và chỉ khi $A$ giao với mọi tập hợp của $\mathfrak{F}$.

#### Hệ quả 2 {#top-i-s6-prop-1-cor-2 .statement}

Một tập hợp $\Phi$ các bộ lọc trên một tập hợp không rỗng $X$ có một cận trên bé nhất trong tập hợp tất cả các bộ lọc trên $X$ khi và chỉ khi, với mọi dãy hữu hạn $(\mathfrak{F}_i)_{1 \leq i \leq n}$ các phần tử của $\Phi$ và mọi $A_i \in \mathfrak{F}_i$ ($1 \leq i \leq n$), giao $A_1 \cap \cdots \cap A_n$ không rỗng.

Vì điều kiện này biểu thị rằng hợp $\mathcal{G}$ của các bộ lọc $\mathfrak{F} \in \Phi$ thỏa mãn điều kiện của Mệnh đề 1.

#### Hệ quả 3 {#top-i-s6-prop-1-cor-3 .statement}

Tập hợp có thứ tự của tất cả các bộ lọc trên một tập hợp không rỗng $X$ là quy nạp.

Mọi tập hợp có thứ tự tuyến tính $\Phi$ các bộ lọc trên $X$ đều thỏa mãn điều kiện của Hệ quả 2 của Mệnh đề 1, vì các tập hợp $A_i$ đều thuộc cùng một $\mathfrak{F}_j$ theo giả thiết, và ta có thể áp dụng $(\mathrm{F}_{\mathrm{II}})$.

### 3. CƠ SỞ CỦA MỘT BỘ LỌC

Nếu $\mathcal{G}$ là một cơ sở con của một bộ lọc $\mathfrak{F}$ trên $X$ (no. 2), thì $\mathfrak{F}$ nói chung không phải là tập hợp các tập con của $X$ chứa một tập hợp của $\mathcal{G}$; để $\mathcal{G}$ có tính chất này thì điều kiện cần và đủ là mọi giao hữu hạn của các tập hợp của $\mathcal{G}$ đều chứa một tập hợp của $\mathcal{G}$. Do đó có mệnh đề sau:

#### Mệnh đề 2 {#top-i-s6-prop-2 .statement}

Cho $\mathcal{B}$ là một tập hợp các tập con của một tập hợp $X$. Khi đó tập hợp các tập con của $X$ chứa một tập hợp của $\mathcal{B}$ là một bộ lọc khi và chỉ khi $\mathcal{B}$ có hai tính chất sau:
(B_I) Giao của hai tập hợp của $\mathcal{B}$ chứa một tập hợp của $\mathcal{B}$.
(B_{II}) $\mathcal{B}$ không rỗng, và tập con rỗng của $X$ không thuộc $\mathcal{B}$.

#### Định nghĩa 3 {#top-i-s6-def-3 .statement}

Một tập hợp $\mathcal{B}$ các tập con của một tập hợp $X$ thỏa mãn các tiên đề (B_I) và (B_{II}) được gọi là một cơ sở của bộ lọc mà nó sinh ra. Hai cơ sở bộ lọc được nói là tương đương nếu chúng sinh ra cùng một bộ lọc.

Nếu $\mathcal{G}$ là một dưới cơ sở của một lọc $\mathfrak{F}$, thì tập $\mathcal{G}'$ gồm các giao hữu hạn của các tập của $\mathcal{G}$ là một cơ sở của $\mathfrak{F}$ (no. 2).

#### Mệnh đề 3 {#top-i-s6-prop-3 .statement}

Một tập con $\mathcal{B}$ của một lọc $\mathfrak{F}$ trên $X$ là một cơ sở của $\mathfrak{F}$ khi và chỉ khi mọi tập của $\mathfrak{F}$ chứa một tập của $\mathcal{B}$.

Nếu $\mathcal{B}$ là một cơ sở của $\mathfrak{F}$, thì rõ ràng mọi tập của $\mathfrak{F}$ chứa một tập của $\mathcal{B}$; ngược lại, nếu mọi tập của $\mathfrak{F}$ chứa một tập của $\mathcal{B}$, thì tập hợp các tập con của $X$ chứa một tập của $\mathcal{B}$ trùng với $\mathfrak{F}$ theo tính chất của $(\mathrm{F}_1)$.

#### Mệnh đề 4 {#top-i-s6-prop-4 .statement}

Trên một tập $X$, một lọc $\mathcal{F}'$ với cơ sở $\mathcal{B}'$ mịn hơn một lọc $\mathcal{F}$ với cơ sở $\mathcal{B}$ khi và chỉ khi mọi tập của $\mathcal{B}$ chứa một tập của $\mathcal{B}'$.

Đây là một hệ quả ngay lập tức của các Định nghĩa 2 và 3.

#### Hệ quả {#top-i-s6-n3-cor-1 .statement}

Hai cơ sở lọc $\mathcal{B}, \mathcal{B}'$ trên một tập $X$ là tương đương khi và chỉ khi mọi tập của $\mathcal{B}$ chứa một tập của $\mathcal{B}'$ và mọi tập của $\mathcal{B}'$ chứa một tập của $\mathcal{B}$.

Ví dụ về các cơ sở lọc. 1) Cho $X$ là một không gian tôpô. Mệnh đề 3 chỉ ra rằng các cơ sở của lọc lân cận của một điểm $x \in X$ chính xác là các hệ cơ bản các lân cận của $x$ (\$ 1, no. 3, Định nghĩa 5).

2) Cho $X$ là một tập có hướng không rỗng đối với một quan hệ $(\sigma)$ (Lý thuyết tập hợp, Chương III, \$ 1, no. 10). Với mỗi $a \in X$, tập $S(a)$ gồm tất cả các $x \in X$ sao cho $a(\sigma)x$ sẽ được gọi là tiết diện của $X$ tương ứng với phần tử $a$. Khi đó tập $\mathcal{S}$ các tiết diện của $X$ là một cơ sở lọc, vì nó rõ ràng thỏa mãn $(\mathrm{B}_{\mathrm{II}})$, và nếu $a, b$ là hai phần tử bất kỳ của $X$, thì theo giả thiết tồn tại một phần tử $c \in X$ sao cho $a(\sigma)c$ và $b(\sigma)c$, và do đó
$$
S(c) \subset S(a) \cap S(b),
$$
sao cho $(\mathrm{B}_1)$ được thỏa mãn. Lọc sinh bởi $\mathcal{S}$ được gọi là lọc tiết diện của tập có hướng $X$.

Chẳng hạn, lọc Fréchet (no. 1) là lọc tiết diện của tập hợp có thứ tự $\mathbf{N}$, được xem như có hướng bởi quan hệ $\leqslant$.
Cho $\mathcal{F}$ là một lọc trên một tập hợp $Z$. Vì $\mathcal{F}$ có hướng đối với quan hệ $\supset$ [do tiên đề $(\mathrm{F}_{\mathrm{II}})$] ta có thể định nghĩa một lọc tiết diện trên $\mathcal{F}$; ở đây một tiết diện của $\mathcal{F}$ đối với một tập hợp $A \in \mathcal{F}$ là tập hợp $S(A)$ gồm tất cả các $M \in \mathcal{F}$ sao cho $M \subset A$. Lọc này được gọi là lọc tiết diện của lọc $\mathcal{F}$.

### 4. CÁC LỌC SIÊU

#### Định nghĩa 4 {#top-i-s6-def-4 .statement}

Một lọc siêu trên một tập hợp $X$ là một lọc $\mathcal{F}$ sao cho không có lọc nào trên $X$ mịn hơn thực sự $\mathcal{F}$ (nói cách khác, là một phần tử cực đại trong tập hợp có thứ tự của tất cả các lọc trên $X$).

Vì tập hợp có thứ tự của tất cả các lọc trên $X$ là quy nạp (no. 2, Mệnh đề 1, Hệ quả 3), bổ đề Zorn (Lý thuyết tập hợp, R, \$ 6, no. 10) chỉ ra rằng:

#### Định lý 1 {#top-i-s6-thm-1 .statement}

Nếu $\mathcal{F}$ là một lọc bất kỳ trên một tập hợp $X$, thì có một lọc siêu mịn hơn $\mathcal{F}$.

#### Mệnh đề 5 {#top-i-s6-prop-5 .statement}

Cho $\mathcal{F}$ là một lọc siêu trên một tập hợp $X$. Nếu $A$ và $B$ là hai tập con của $X$ sao cho $A \cup B \in \mathcal{F}$, thì hoặc $A \in \mathcal{F}$ hoặc $B \in \mathcal{F}$.

Nếu mệnh đề này sai, tồn tại các tập con $A$ và $B$ của $X$ sao cho $A \notin \mathcal{F}$ và $B \notin \mathcal{F}$ và $A \cup B \in \mathcal{F}$. Cho $\mathcal{G}$ là tập hợp các tập con $M$ của $X$ sao cho $A \cup M \in \mathcal{F}$. Dễ dàng kiểm tra rằng $\mathcal{G}$ là một lọc trên $X$, và $\mathcal{G}$ mịn hơn thực sự $\mathcal{F}$, vì $B \in \mathcal{G}$; nhưng điều này mâu thuẫn với giả thiết rằng $\mathcal{F}$ là một lọc siêu.

#### Hệ quả {#top-i-s6-n4-cor-1 .statement}

*Nếu hợp của một dãy hữu hạn* $(A_i)_{1 \leq i \leq n}$ *các tập con của* $X$ *thuộc một lọc siêu* $\mathcal{F}$, *thì ít nhất một trong các* $A_i$ *thuộc* $\mathcal{F}$.

Chứng minh được thực hiện bằng quy nạp theo $n$.
Đặc biệt, nếu $(A_i)_{1 \leq i \leq n}$ là một *phủ* của $X$, thì ít nhất một trong các $A_i$ thuộc $\mathcal{F}$.
Mệnh đề 5 *đặc trưng* các lọc siêu; tổng quát hơn, ta có:

#### Mệnh đề 6 {#top-i-s6-prop-6 .statement}

*Cho* $\mathcal{G}$ *là một cơ sở phụ của một bộ lọc trên một tập hợp* $X$. *Nếu với mỗi tập con* $Y$ *của* $X$ *ta có hoặc là* $Y \in \mathcal{G}$ *hoặc là* $\complement Y \in \mathcal{G}$, *thì* $\mathcal{G}$ *là một siêu lọc trên* $X$.

Cho $\mathcal{F}$ là một bộ lọc chứa $\mathcal{G}$ (có một bộ lọc như vậy, theo giả thiết); khi đó $\mathcal{F}$ trùng với $\mathcal{G}$; vì nếu $Y \in \mathcal{F}$ thì $\complement Y \notin \mathcal{F}$; do đó $\complement Y \notin \mathcal{G}$ và suy ra $Y \in \mathcal{G}$.

*Ví dụ về một siêu lọc.* Tập hợp tất cả các tập con của một tập hợp không rỗng $X$ chứa một phần tử cho trước $a \in X$ là một siêu lọc; vì nó là một bộ lọc, và nếu $Y$ là một tập con bất kỳ của $X$ thì hoặc là $a \in Y$ hoặc là $a \in \complement Y$. Những siêu lọc như vậy được gọi là *tầm thường*.

Ngoài ví dụ này, ta sẽ không bao giờ chứng minh sự tồn tại của một siêu lọc (ngay cả trên một tập vô hạn đếm được) trừ khi sử dụng Định lý 1 (và do đó tiên đề lựa chọn).

#### Nhận xét {#top-i-s6-n4-rem-1 .statement}

Nếu $X$ chứa ít nhất hai phần tử, thì có ít nhất hai siêu lọc phân biệt trên $X$, và do đó tập hợp có thứ tự của các bộ lọc trên $X$ không có phần tử lớn nhất.

#### Mệnh đề 7 {#top-i-s6-prop-7 .statement}

*Mọi bộ lọc* $\mathcal{F}$ *trên một tập hợp* $X$ *là giao của các siêu lọc mịn hơn* $\mathcal{F}$.

Rõ ràng giao này chứa $\mathcal{F}$. Ngược lại, cho $A$ là một tập con của $X$ không thuộc $\mathcal{F}$, và ký hiệu $A'$ là $\complement A$; $A$ không chứa tập hợp nào của $\mathcal{F}$; do đó mọi $M \in \mathcal{F}$ đều giao với $A'$ và vì vậy (no. 2, Mệnh đề 1, Hệ quả 1) có một bộ lọc $\mathcal{F}'$ mịn hơn $\mathcal{F}$ và chứa $A'$. Nếu $\mathcal{U}$ là một siêu lọc mịn hơn $\mathcal{F}'$ (Định lý 1) thì suy ra $A \notin \mathcal{U}$. Điều này hoàn thành chứng minh.

### 5. BỘ LỌC CẢM SINH

#### Mệnh đề 8 {#top-i-s6-prop-8 .statement}

*Cho* $\mathcal{F}$ *là một bộ lọc trên một tập hợp* $X$ *và* $A$ *là một tập con của* $X$. *Khi đó vết* $\mathcal{F}_A$ *của* $\mathcal{F}$ *trên* $A$ *là một bộ lọc khi và chỉ khi mỗi tập hợp của* $\mathcal{F}$ *giao với* $A$.

Vì $(M \cap N) \cap A = (M \cap A) \cap (N \cap A)$ ta thấy rằng $\mathfrak{F}_A$ thỏa mãn $(\mathrm{F}_{\mathrm{II}})$; một lần nữa, nếu $M \cap A \subset P \subset A$ thì $P = (M \cup P) \cap A$, do đó $\mathfrak{F}_A$ thỏa mãn $(\mathrm{F}_1)$. Suy ra $\mathfrak{F}_A$ là một lọc khi và chỉ khi nó thỏa mãn $(\mathrm{F}_{\mathrm{III}})$, nghĩa là khi và chỉ khi mỗi tập hợp của $\mathfrak{F}$ giao với $A$.

Đặc biệt, nếu $A \in \mathfrak{F}$ thì $\mathfrak{F}_A$ là một lọc trên $A$, theo $(\mathrm{F}_{\mathrm{II}})$ và $(\mathrm{F}_{\mathrm{III}})$.

#### Định nghĩa 5 {#top-i-s6-def-5 .statement}

*Cho $A$ là một tập con của một tập hợp $X$ và $\mathfrak{F}$ là một lọc trên $X$. Nếu vết của $\mathfrak{F}$ trên $A$ là một lọc trên $A$, thì lọc này được gọi là cảm sinh bởi $\mathfrak{F}$ trên $A$.*

Nếu một lọc $\mathfrak{F}$ trên $X$ cảm sinh một lọc trên $A \subset X$, thì vết trên $A$ của một cơ sở của $\mathfrak{F}$ là một cơ sở của $\mathfrak{F}_A$, do Mệnh đề 3 của no. 3.

#### Ví dụ {#top-i-s6-n5-exa-1 .statement}

Cho $X$ là một không gian tôpô, $A$ một tập con của $X$, $x$ một điểm của $X$. Để vết trên $A$ của *lọc lân cận* $\mathcal{B}$ của $x$ là một lọc trên $A$, điều kiện cần và đủ là mọi lân cận của $x$ đều giao với $A$, nghĩa là $x$ nằm trong *bao đóng* của $A$ (\$ 1, no. 6, Định nghĩa 10).

Ví dụ này về một lọc cảm sinh có ý nghĩa vì hai lý do: trước hết vì nó đóng một vai trò quan trọng trong lý thuyết về giới hạn (\$ 7, no. 5) và thứ hai vì *mọi lọc đều có thể được định nghĩa theo cách này*. Thật vậy, cho $\mathfrak{F}$ là một lọc trên một tập hợp $X$ và cho $X'$ là tập hợp nhận được bằng cách *ghép thêm* một phần tử mới $\omega$ vào $X$, $X$ được đồng nhất với phần bù của $\{ \omega \}$ trong $X'$ (*Lý thuyết tập hợp*, R, \$ 4, no. 5); cho $\mathfrak{F}'$ là lọc trên $X'$ gồm các tập hợp $M \cup \{ \omega \}$ trong đó $M$ chạy qua $\mathfrak{F}$. Với mỗi điểm $x \neq \omega$ của $X'$, cho $\mathcal{B}(x)$ là tập hợp tất cả các tập con của $X'$ chứa $x$, và cho $\mathcal{B}(\omega)$ là $\mathfrak{F}'$; khi đó các $\mathcal{B}(x)$ với $x \in X'$ hiển nhiên thỏa mãn các tiên đề $(\mathrm{V}_1), (\mathrm{V}_{\mathrm{II}}), (\mathrm{V}_{\mathrm{III}})$ và $(\mathrm{V}_{\mathrm{IV}})$ và do đó định nghĩa một tôpô trên $X'$ mà đối với nó chúng là các lọc lân cận của các điểm. Cuối cùng $\omega$ nằm trong *bao đóng* của $X$ trong tôpô này, và $\mathfrak{F}$ được cảm sinh bởi $\mathfrak{F}' = \mathcal{B}(\omega)$ trên $X$. Tôpô được định nghĩa như vậy trên $X'$ (tương ứng tập hợp $X'$ với tôpô này) được gọi là *tôpô* (tương ứng *không gian tôpô*) *liên kết với* $\mathfrak{F}$.

#### Mệnh đề 9 {#top-i-s6-prop-9 .statement}

*Một lọc cực đại $U$ trên một tập hợp $X$ cảm sinh một lọc trên một tập con $A$ của $X$ khi và chỉ khi $A \in U$; và nếu điều kiện này được thỏa mãn thì $U_A$ là một lọc cực đại trên $A$.*

Đây là một hệ quả ngay lập tức của các Mệnh đề 5 và 6 của no. 4.

### 6. ẢNH TRỰC TIẾP VÀ ẢNH NGƯỢC CỦA CƠ SỞ LỌC

Cho $\mathcal{B}$ là một cơ sở lọc trên một tập hợp $X$, và cho $f$ là một ánh xạ từ $X$ vào một tập hợp $X'$; khi đó $f(\mathcal{B})$ là một *cơ sở lọc* trên $X'$, vì quan hệ $M \neq \emptyset$ kéo theo $f(M) \neq \emptyset$, và ta có $f(M \cap N) \subset f(M) \cap f(N)$. Nếu $\mathcal{B}_1$ là một cơ sở của một lọc *mịn hơn* lọc có cơ sở $\mathcal{B}$, thì $f(\mathcal{B}_1)$ là một cơ sở của một lọc *mịn hơn* lọc có cơ sở $f(\mathcal{B})$ (no. 3, Mệnh đề 4).

#### Mệnh đề 10 {#top-i-s6-prop-10 .statement}

*Nếu $\mathcal{B}$ là một cơ sở lọc siêu lọc trên một tập hợp $X$ và nếu $f$ là một ánh xạ của $X$ vào một tập hợp $X'$, thì $f(\mathcal{B})$ là một cơ sở lọc siêu lọc trên $X'$.*

Cho $M'$ là một tập con của $X'$. Nếu $\overline{f}^{-1}(M')$ chứa một tập hợp $M$ của $\mathcal{B}$, thì $M'$ chứa $f(M)$; nếu không, thì $\mathcal{C}_{\overline{f}}^{-1}(M') = \overline{f}^{-1}\mathcal{C}(M')$ chứa một tập hợp $N$ của $\mathcal{B}$ (no. 4, Mệnh đề 5) và do đó $\mathcal{C}M'$ chứa $f(N)$. Suy ra kết quả từ Mệnh đề 6 của no. 4.

Xét riêng trường hợp $f$ là đơn ánh chính tắc $A \to X$ của một tập con $A$ của một tập hợp $X$. Nếu $\mathcal{B}$ là một cơ sở lọc trên $A$ thì $f(\mathcal{B})$ là một cơ sở lọc trên $X$. Lọc $\mathfrak{F}$ trên $X$ sinh bởi $f(\mathcal{B})$ được gọi là *lọc sinh bởi $\mathcal{B}$ khi $\mathcal{B}$ được xem như một cơ sở lọc trên $X$*. Nếu $\mathcal{B}$ là một *cơ sở lọc siêu lọc* trên $A$ thì nó cũng là một *cơ sở lọc siêu lọc* trên $X$ theo Mệnh đề 10.

Tiếp theo hãy xét xem *ảnh ngược* của một cơ sở lọc có phải là một cơ sở lọc hay không. Cho $\mathcal{B}'$ là một cơ sở lọc trên một tập hợp $X'$, và cho $f$ là một ánh xạ của một tập hợp $X$ vào $X'$; khi đó $\overline{f}^{-1}(\mathcal{B}')$ là một cơ sở lọc trên $X$ *khi và chỉ khi* $\overline{f}^{-1}(M') \neq \varnothing$ *với mỗi* $M' \in \mathcal{B}'$. Đây là một hệ quả ngay lập tức của quan hệ $\overline{f}^{-1}(M' \cap N') = \overline{f}^{-1}(M') \cap \overline{f}^{-1}(N')$ và của Định nghĩa 3 của no. 3. Điều kiện này cũng có thể được biểu diễn bằng cách nói rằng *mọi tập hợp của $\mathcal{B}'$ đều gặp $f(X)$* [hoặc rằng vết của $\mathcal{B}'$ trên $f(X)$ là một cơ sở lọc]. Nếu điều kiện này được thỏa mãn, thì $f(\overline{f}^{-1}(\mathcal{B}'))$ là một cơ sở của một lọc *mịn hơn* lọc có cơ sở $\mathcal{B}$.

Nếu $\mathcal{B}$ là một cơ sở lọc trên $X$ thì rõ ràng điều kiện trên được thỏa mãn bởi $\mathcal{B}' = f(\mathcal{B}); \; \overline{f}^{-1}(f(\mathcal{B}))$ khi đó là một cơ sở của một lọc *thô hơn* lọc có cơ sở $\mathcal{B}$.

Cho $A$ là một tập con của một tập hợp $X$, $\varphi$ là đơn ánh chính tắc $A \to X$; nếu $\mathcal{B}$ là một cơ sở lọc trên $X$ thì $\overline{\varphi}^{-1}(\mathcal{B})$ trùng với $\mathcal{B}_A$. Nếu biểu diễn điều này như một cơ sở lọc của $A$ bằng điều kiện trên, ta thu được một phần của Mệnh đề 8 của no. 5.

### 7. TÍCH CỦA CÁC CƠ SỞ LỌC

Cho $(X_i)_{i \in I}$ là một họ các tập hợp, và với mỗi $i \in I$ cho $\mathcal{B}_i$ là một *cơ sở lọc* trên $X_i$. Cho $\mathcal{B}$ là tập hợp các tập con của tập tích $X = \prod_{i \in I} X_i$ có dạng $\prod_{i \in I} M_i$, trong đó $M_i = X_i$ ngoại trừ một số hữu hạn các chỉ số và $M_i \in \mathcal{B}_i$ với mỗi $i$ sao cho $M_i \neq X_i$. Công thức $\left( \prod_{i \in I} M_i \right) \cap \left( \prod_{i \in I} N_i \right) = \prod_{i \in I} (M_i \cap N_i)$ chỉ ra rằng $\mathcal{B}$ là một *cơ sở lọc* trên $X$. Chú ý rằng lọc có cơ sở $\mathcal{B}$ cũng được sinh bởi các

tập hợp $\overline{\mathrm{pr}}_x^{-1}(M_x)$, trong đó $M_x \in \mathcal{B}_x$ và $x$ chạy qua $I$, vì
$$
\overline{\mathrm{pr}}_x^{-1}(M_x) = M_x \times \prod_{i \neq x} X_i.
$$

#### Định nghĩa 6 {#top-i-s6-def-6 .statement}

*Một lọc $\mathfrak{F}_i$ trên mỗi tập hợp $X_i$ của một họ các tập hợp $(X_i)_{i \in I}$ được cho, tích của các lọc $\mathfrak{F}_i$ là lọc trên $X = \prod_{i \in I} X_i$ có một cơ sở là tập hợp các tập con của $X$ có dạng $\prod_{i \in I} M_i$, trong đó $M_i \in \mathfrak{F}_i$ với mỗi $i \in I$ và $M_i = X_i$ với mọi chỉ số trừ một số hữu hạn. Lọc tích được ký hiệu bởi $\prod_{i \in I} \mathfrak{F}_i$.*

Người đọc có thể dễ dàng kiểm tra rằng tích của các lọc $\mathfrak{F}_i$ cũng có thể được định nghĩa như lọc *thô nhất* $\mathfrak{G}$ trên $X$ sao cho $\mathrm{pr}_i(\mathfrak{G}) = \mathfrak{F}_i$ với mỗi $i \in I$.

Các nhận xét trước đó chỉ ra rằng nếu $\mathcal{B}_i$ là một cơ sở của $\mathfrak{F}_i$ với mỗi $i \in I$, thì $\mathcal{B}$ là một *cơ sở* của lọc tích $\prod_{i \in I} \mathfrak{F}_i$ (no. 3, Mệnh đề 3).

Trên một tích $X = \prod_{i \in I} X_i$ của các không gian tôpô, lọc lân cận của mọi điểm $x = (x_i)$ là *tích* của các lọc lân cận của các $x_i$ (\S 4, no. 1).

Phép dựng của một tích bộ lọc $\mathfrak{F} = \prod_{i \in I} \mathfrak{F}_i$ đơn giản hơn khi tập hợp chỉ số $I$ là *hữu hạn*: một cơ sở của $\mathfrak{F}$ khi đó được tạo bởi *tất cả* các tích $\prod_{i \in I} M_i$, trong đó $M_i \in \mathfrak{F}_i$ với mỗi $i \in I$. Nếu $I = \{ 1, 2, \ldots, n \}$ ta viết
$$
\mathfrak{F}_1 \times \mathfrak{F}_2 \times \cdots \times \mathfrak{F}_n
$$
thay cho $\prod_{i \in I} \mathfrak{F}_i$.

### 8. CÁC BỘ LỌC SƠ CẤP

#### Định nghĩa 7 {#top-i-s6-def-7 .statement}

*Cho $(x_n)_{n \in \mathbf{N}}$ là một dãy vô hạn các phần tử của một tập hợp $X$. Bộ lọc sơ cấp liên kết với dãy $(x_n)$ là bộ lọc sinh bởi ảnh của bộ lọc Fréchet (no. 1) qua ánh xạ $n \to x_n$ từ $\mathbf{N}$ vào $X$.*

Điều này cũng tương tự như nói rằng bộ lọc sơ cấp liên kết với $(x_n)$ là tập hợp các tập con $M$ của $X$ sao cho $x_n \in M$ ngoại trừ một số *hữu hạn* giá trị của $n$. Nếu $S_n$ chỉ tập hợp tất cả các $x_p$ sao cho $p \geq n$, thì các tập hợp $S_n$ tạo thành một *cơ sở* của bộ lọc sơ cấp liên kết với dãy $(x_n)$.

Bộ lọc sơ cấp liên kết với một *dãy con* vô hạn của một dãy $(x_n)$ là *mịn hơn* bộ lọc sơ cấp liên kết với $(x_n)$ (xem Bài tập 15).

Theo định nghĩa, mọi bộ lọc sơ cấp đều có một cơ sở đếm được. Ngược lại:

#### Mệnh đề 11 {#top-i-s6-prop-11 .statement}

*Nếu một bộ lọc $\mathfrak{F}$ có một cơ sở đếm được, thì nó là giao của các bộ lọc sơ cấp mịn hơn $\mathfrak{F}$.*

Hãy sắp xếp cơ sở đếm được của $\mathfrak{F}$ thành một dãy $(A_n)_{n \in \mathbf{N}}$; nếu ta đặt

$$
B_n = \bigcap_{p=0}^n A_p,
$$

thì các $B_n$ lại tạo thành một cơ sở của $\mathfrak{F}$ (no. 3, Mệnh đề 3) và ta có $B_{n+1} \subset B_n$ với mỗi $n$. Cho $a_n$ là một phần tử bất kỳ của $B_n$ với mỗi $n \in \mathbf{N}$; khi đó rõ ràng rằng $\mathfrak{F}$ thô hơn bộ lọc sơ cấp liên kết với $(a_n)$. Do đó giao $\mathfrak{J}$ của các bộ lọc sơ cấp mịn hơn $\mathfrak{F}$ tồn tại và mịn hơn $\mathfrak{F}$; nếu $\mathfrak{J}$ *thực sự mịn hơn* $\mathfrak{F}$ thì tồn tại một tập hợp $M \in \mathfrak{J}$ sao cho $B_n \cap \complement M \neq \varnothing$ với mỗi $n$; nếu $b_n \in B_n \cap \complement M$, thì bộ lọc sơ cấp liên kết với dãy $(b_n)$ mịn hơn $\mathfrak{F}$ và không chứa $M$. Điều này mâu thuẫn với định nghĩa của $\mathfrak{J}$.

#### Nhận xét {#top-i-s6-n8-rem-1 .statement}

Một bộ lọc *thô hơn* một bộ lọc có một cơ sở đếm được không nhất thiết phải có một cơ sở đếm được; ví dụ, nếu $X$ là một tập hợp vô hạn không đếm được, thì bộ lọc gồm các phần bù của các tập con hữu hạn của $X$ không có cơ sở đếm được (nếu không thì tập hợp các tập con hữu hạn của $X$ sẽ là đếm được, trái với giả thiết); tuy nhiên bộ lọc này thô hơn mọi bộ lọc sơ cấp liên kết với một dãy vô hạn các phần tử phân biệt của $X$.

### 9. MẦM ĐỐI VỚI MỘT BỘ LỌC

Cho $\mathfrak{F}$ là một lọc trên một tập hợp $X$. Trên tập hợp $\mathfrak{P}(X)$ gồm mọi tập con của $X$, quan hệ

"tồn tại $V \in \mathfrak{F}$ sao cho $M \cap V = N \cap V$"

giữa $M$ và $N$ là một *quan hệ tương đương* $R$, vì $R$ hiển nhiên phản xạ và đối xứng, và nếu $M, N, P$ là ba tập con của $X$ sao cho $M \cap V = N \cap V$ và $N \cap W = P \cap W$, trong đó $V$ và $W$ thuộc $\mathfrak{F}$, thì suy ra $M \cap (V \cap W) = N \cap (V \cap W) = P \cap (V \cap W)$ và $V \cap W \in \mathfrak{F}$, do đó $R$ là bắc cầu. Lớp tương đương mod $R$ của một tập con $M$ của $X$ được gọi là *mầm của $M$ đối với $\mathfrak{F}$*; tập thương $\mathfrak{P}(X)/R$ được gọi là *tập hợp các mầm của các tập con của $X$ (đối với $\mathfrak{F}$)*. Các ánh xạ $(M, N) \to M \cap N$ và $(M, N) \to M \cup N$ từ

$$
\mathfrak{P}(X) \times \mathfrak{P}(X)
$$

vào $\mathfrak{P}(X)$ là tương thích với các quan hệ tương đương $R \times R$ và $R$

$$
M \cap V = M' \cap V \quad \text{và} \quad N \cap W = N' \cap W,
$$
sao cho
$$
(M \cap N) \cap (V \cap W) = (M' \cap N') \cap (V \cap W)
$$
và
$$
\begin{align*}
(M \cup N) \cap (V \cap W) &= (M \cap (V \cap W)) \cup (N \cap (V \cap W)) \\
&= (M' \cap (V \cap W)) \cup (N' \cap (V \cap W)) \\
&= (M' \cup N') \cap (V \cap W).
\end{align*}
$$

Chuyển qua các tập thương, các ánh xạ này cảm sinh hai ánh xạ từ $(\mathfrak{P}(X)/R) \times (\mathfrak{P}(X)/R)$ vào $\mathfrak{P}(X)/R$, mà ta ký hiệu (do lạm dụng ngôn ngữ) lần lượt là $(\xi, \eta) \to \xi \cap \eta$ và $(\xi, \eta) \to \xi \cup \eta$. Đây là một bài tập đơn giản để kiểm tra rằng đối với các luật hợp thành này [được xác định trên toàn bộ $\mathfrak{P}(X)/R$] mọi phần tử đều lũy đẳng, và mỗi luật đều giao hoán và kết hợp và phân phối đối với luật kia. Hơn nữa, các quan hệ $\xi = \xi \cap \eta$ và $\eta = \xi \cup \eta$ là tương đương; nếu ta ký hiệu chúng (do lạm dụng ngôn ngữ) là $\xi \subset \eta$, thì dễ dàng kiểm tra rằng quan hệ này là một thứ tự trên $\mathfrak{P}(X)/R$, theo đó $\mathfrak{P}(X)/R$ là một dàn có phần tử nhỏ nhất là mầm của $\varnothing$ và phần tử lớn nhất là mầm của $X$. Chú ý rằng quan hệ $\xi \subset \eta$ có nghĩa là tồn tại $M \in \xi$, $N \in \eta$ và $V \in \mathfrak{F}$ sao cho $M \cap V \subset N \cap V$.

Bây giờ cho $X'$ là một tập hợp khác, và cho $\Phi$ là tập hợp tất cả các ánh xạ của một tập hợp thuộc $\mathfrak{F}$ vào $X'$. Quan hệ trên $\Phi$

"tồn tại $V \in \mathfrak{F}$ sao cho $f$ và $g$ được xác định và trùng nhau trên $V$"

giữa $f$ và $g$ là một quan hệ tương đương $S$; hiển nhiên rằng $S$ là phản xạ và đối xứng, và nếu $f, g, h$ là ba phần tử của $\Phi$ sao cho $f$ và $g$ được xác định trên $V \in \mathfrak{F}$, còn $g$ và $h$ được xác định và trùng nhau trên $W \in \mathfrak{F}$, thì $f$ và $h$ được xác định và trùng nhau trên $V \cap W \in \mathfrak{F}$, do đó $S$ là bắc cầu. Lớp tương đương mod $S$ của một ánh xạ $f$ của một tập hợp $V \in \mathfrak{F}$ vào $X'$ được gọi là mầm của $f$ (đối với $\mathfrak{F}$), và tập thương $\tilde{\Phi} = \Phi/S$ được gọi là tập hợp các mầm của các ánh xạ từ $X$ vào $X'$ (đối với $\mathfrak{F}$).

#### Nhận xét 1 {#top-i-s6-n9-rem-1 .statement}

Mọi ánh xạ $f$ của một tập con $M$ của $X$ vào $X'$, trong đó $M$ thuộc về $\mathfrak{F}$, đều tương đương mod $S$ với một ánh xạ $f_1$ của $X$ vào $X'$ (điều này biện minh cho thuật ngữ trên đây): chỉ cần mở rộng $f$ lên $X$, chẳng hạn bằng cách gán cho nó một giá trị hằng trên $X - M$.

#### Nhận xét 2 {#top-i-s6-n9-rem-2 .statement}

Các hàm đặc trưng $\varphi_M$ và $\varphi_N$ của hai tập con $M$ và $N$ của $X$ có cùng một mầm đối với $\mathfrak{F}$ khi và chỉ khi $M$ và $N$ có cùng một mầm đối với $\mathfrak{F}$.

Cho $X''$ là một tập hợp thứ ba, $\varphi$ là một ánh xạ của $X'$ vào $X''$, $\Phi'$ là tập hợp tất cả các ánh xạ của một tập hợp của $\mathfrak{F}$ vào $X''$. Với mỗi $f \in \Phi$, $\varphi \circ f$ thuộc về $\Phi'$; hơn nữa, ta thấy ngay rằng nếu $g \in \Phi$ có cùng mầm với $f$ đối với $\mathfrak{F}$, thì $\varphi \circ f$ và $\varphi \circ g$ có cùng mầm đối với $\mathfrak{F}$.

Do đó mầm này chỉ phụ thuộc vào mầm $\tilde{f}$ của $f$ đối với $\mathfrak{F}$ và được ký hiệu là $\varphi(\tilde{f})$. Như vậy ta định nghĩa một ánh xạ (được ký hiệu là $\varphi$, do lạm dụng ngôn ngữ) từ tập hợp $\tilde{\Phi}$ các mầm của các ánh xạ từ $X$ vào $X'$, vào tập hợp $\tilde{\Phi}'$ các mầm của các ánh xạ từ $X$ vào $X''$.

Bây giờ cho $X'_i$ ($1 \leq i \leq n$) là các tập hợp và
$$
Y = \prod_{i=1}^n X'_i
$$
là tích của chúng; ký hiệu $\Phi_i$ (tương ứng $\Phi$) là tập hợp tất cả các ánh xạ từ một tập hợp của $\mathfrak{F}$ vào $X'_i$ (tương ứng $Y$). Nếu $f_i \in \Phi_i$ với $1 \leq i \leq n$ và nếu $M_i \in \mathfrak{F}$ là miền xác định của $f_i$, thì ánh xạ $t \to (f_1(t), \ldots, f_n(t))$ được xác định trên
$$
\bigcap_{i=1}^n M_i
$$
và do đó thuộc $\Phi$; ta ký hiệu ánh xạ này (do lạm dụng ngôn ngữ) bởi $(f_1, \ldots, f_n)$. Hơn nữa, nếu $f_i$ và $g_i$ thuộc $\Phi_i$ và có cùng mầm đối với $\mathfrak{F}$ (với $1 \leq i \leq n$), thì ngay lập tức thấy rằng $(f_1, \ldots, f_n)$ và $(g_1, \ldots, g_n)$ có cùng mầm đối với $\mathfrak{F}$; do đó mầm này chỉ phụ thuộc vào các mầm $\tilde{f}_i$ của các $f_i$. Nếu ta ký hiệu nó bởi $\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$ thì $\Gamma$ rõ ràng là một song ánh từ tập hợp tích
$$
\prod_{i=1}^n \tilde{\Phi}_i
$$
lên tập hợp $\tilde{\Phi}$, trong đó $\tilde{\Phi}_i$ (tương ứng $\tilde{\Phi}$) ký hiệu tập hợp các mầm của các ánh xạ từ $X$ vào $X'_i$ (tương ứng $Y$) đối với $\mathfrak{F}$; do đó, do lạm dụng ngôn ngữ, ta sẽ nói chung viết $(\tilde{f}_1, \ldots, \tilde{f}_n)$ thay cho $\Gamma(\tilde{f}_1, \ldots, \tilde{f}_n)$ bất cứ khi nào không có nguy cơ nhầm lẫn.

Từ những điều đã nói, mọi ánh xạ $\psi$ từ $Y$ vào một tập hợp $X''$ xác định một ánh xạ $(\tilde{f}_1, \ldots, \tilde{f}_n) \to \psi(\tilde{f}_1, \ldots, \tilde{f}_n)$ từ
$$
\prod_{i=1}^n \tilde{\Phi}_i
$$
vào tập hợp $\tilde{\Phi}'$ các mầm của các ánh xạ từ $X$ vào $X''$.

Đặc biệt, nếu $n = 2$ và nếu $X'_1, X'_2$ và $X''$ đều bằng cùng một tập hợp $X'$ (sao cho $\psi$ là một luật hợp thành được xác định trên toàn bộ $X'$), thì $\psi$ cảm sinh một luật hợp thành được xác định trên toàn bộ tập hợp $\tilde{\Phi}$ các mầm của các ánh xạ từ $X$ vào $X'$. Dễ dàng kiểm chứng rằng nếu luật được cho trên $X'$ là kết hợp (tương ứng giao hoán) thì luật tương ứng trên $\tilde{\Phi}$ cũng vậy; nếu luật $\psi$ trên $X'$ có một phần tử đơn vị $e'$, thì mầm đối với $\mathfrak{F}$ của ánh xạ hằng $x \to e'$ là một phần tử đơn vị đối với luật tương ứng trên $\tilde{\Phi}$. Cuối cùng, nếu luật trên $X'$ có một phần tử đơn vị $e'$, thì mầm $\tilde{f}$ của $f \in \Phi$ có một nghịch đảo trong $\tilde{\Phi}$ khi và chỉ khi tồn tại $V \in \mathfrak{F}$, được chứa trong miền xác định của $f$, sao cho $f(t)$ là khả nghịch trong $X'$ với mỗi $t \in V$; nếu, với mỗi $t \in V$, $g(t)$ ký hiệu nghịch đảo của $f(t)$ thì mầm $\tilde{g}$ của $g$ là nghịch đảo của $\tilde{f}$ trong $\tilde{\Phi}$. Đặc biệt nếu $X'$ là một nhóm đối với luật $\psi$, thì $\tilde{\Phi}$ là một nhóm đối với luật tương ứng; tương tự, nếu $X'$ là một vành (tương ứng một đại số trên một vành $A$) thì $\tilde{\Phi}$ là một vành (tương ứng một đại số trên $A$) đối với các luật hợp thành tương ứng.

### 10. CÁC MẦM TẠI MỘT ĐIỂM

Một trong những tình huống thường gặp nhất mà các định nghĩa và kết quả của no. 9 được áp dụng là tình huống trong đó $\mathfrak{F}$ là bộ lọc lân cận của một điểm $a$ của một không gian tôpô $X$; thay vì nói "các mầm đối với $\mathfrak{F}$" ta khi đó nói "các mầm tại điểm $a$". Chú ý rằng chỉ có một mầm các lân cận của $a$, đó là mầm của toàn bộ không gian $X$. Các mầm của các tập hợp đóng trùng với các mầm của các tập hợp đóng địa phương tại điểm $a$, vì nếu $L$ đóng địa phương tại $a$, thì các mầm của $L$ và $\overline{\Gamma}$ tại $a$ là bằng nhau (\S 3, no. 1, Proposition 1). Suy ra rằng nếu $\xi, \eta$ là hai mầm của các tập hợp đóng địa phương tại $a$, thì $\xi \cup \eta$ và $\xi \cap \eta$ cũng vậy.

Vì $a$ thuộc mọi $V \in \mathfrak{F}$, $f(a)$ được xác định với mỗi ánh xạ $f$ mà miền xác định thuộc $\mathfrak{F}$; hơn nữa, nếu $f$ và $g$ có cùng mầm tại $a$ thì ta phải có $f(a) = g(a)$, do đó $f(a)$ chỉ phụ thuộc vào mầm $\tilde{f}$ của $f$ tại $a$, và được gọi là giá trị của $\tilde{f}$ tại $a$ và được ký hiệu là $\tilde{f}(a)$. Cần nhấn mạnh rằng quan hệ $\tilde{f}(a) = \tilde{g}(a)$ nói chung không kéo theo $\tilde{f} = \tilde{g}$.

Cho $X', X''$ là hai không gian tôpô; $b$ là một điểm của $X''$; $g, g'$ là hai ánh xạ từ $X'$ vào $X''$ có cùng mầm tại $b$. Nếu $f, f'$ là hai ánh xạ từ $X$ vào $X'$ liên tục tại $a$ và có cùng mầm tại $a$ và thỏa mãn $f(a) = b$, thì $g \circ f$ và $g' \circ f'$ có cùng mầm tại điểm $a$; vì nếu $V'$ là một lân cận của $b$ trong $X'$ sao cho $g(x') = g'(x')$ với mọi $x' \in V'$, thì tồn tại một lân cận $V$ của $a$ sao cho $f(V) \subset V'$, $f'(V) \subset V'$ và $f(x) = f'(x')$ với mọi $x \in V$, và mệnh đề được suy ra. Mầm của $g \circ f$ tại $a$ khi đó được gọi là hợp thành của các mầm $\tilde{g}$ và $\tilde{f}$ của $g$ và $f$ tương ứng và được ký hiệu là $\tilde{g} \circ \tilde{f}$.

### Bài tập {#top-i-s6-exercises}

Xem các [bài tập của § 6](exercises/s6/).
