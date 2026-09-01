---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 0
section_title: Pseudomodules
appendix: true
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 378-379, 425
pdf_pages: 0402-0403, 0449-0449
extraction: ocr
subsections:
    - "no": 1
      title: ADJUNCTION OF A UNIT ELEMENT TO A PSEUDO-RING
      page: 378
      pdf_page: 402
    - "no": 2
      title: PSEUDOMODULES
      page: 378
      pdf_page: 402
statements: 0
exercises: 1
content_sha256: a835b314157b2d3992d3bed307ac513304f668992d71606167cb5167ff6da98e
translated_from: content/en/alg/II/A_a_pseudomodules.md
source_content_sha256: db883a717633a15e64137f982b71d8ce6f40a59783e9d1c7d5ac706248c39106
translation_model: gpt-5.4
translation_run: translate-vi-a37710f7
glossary_version: 34
glossary_terms_sha256: 80ca20bb865864ff9c6dc64662f206a849520c54aa505a228f119563e9338ca1
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## PHỤ LỤC

# GIẢ MÔĐUN

### 1. PHÉP NỐI THÊM MỘT PHẦN TỬ ĐƠN VỊ VÀO MỘT GIẢ VÀNH

Cho A là một giả vành (I, § 8, no. 1). Trên tập hợp $A' = \mathbf{Z} \times A$ ta định nghĩa các luật hợp thành sau:

$$
\begin{cases}
(m, a) + (n, b) = (m + n, a + b) \\
(m, a)(n, b) = (mn, mb + na + ab).
\end{cases}
$$

Ngay lập tức kiểm tra được rằng $A'$ với hai luật hợp thành này là một vành trong đó phần tử $(1, 0)$ là phần tử đơn vị. Tập hợp $\{0\} \times A$ là một iđêan hai phía của $A'$ và $i : x \mapsto (0, x)$ là một đẳng cấu của giả vành A lên giả-vành con $\{0\} \times A$, nhờ đó A và $\{0\} \times A$ được đồng nhất. $A'$ được gọi là vành dẫn xuất từ giả vành A bằng cách nối thêm một phần tử đơn vị.

Nếu A đã có một phần tử đơn vị $\varepsilon$, thì phần tử $e = (0, \varepsilon)$ của $A'$ là một phần tử lũy đẳng thuộc tâm của $A'$ và sao cho

$$
A = eA' = A'e.
$$

Khi đó $(eA', (1 - e)A')$ là một phân tích trực tiếp (I, § 8, no. 11) của $A'$ và vành $(1 - e)A'$ đẳng cấu với $\mathbf{Z}$.

### 2. GIẢ MÔĐUN

Cho một giả vành A có hoặc không có phần tử đơn vị, một môđun giả trái trên A là một nhóm giao hoán E (được viết theo lối cộng) có A làm tập hợp toán tử và thỏa mãn các tiên đề $(\mathrm{M}_I), (\mathrm{M}_{II})$ và $(\mathrm{M}_{III})$ của § 1, no. 1, Định nghĩa 1. Các môđun giả phải trên A được định nghĩa tương tự.

Gọi $A'$ là vành thu được bằng cách nối thêm một phần tử đơn vị vào A. Nếu E là một môđun giả trái trên A, thì một cấu trúc $A'$-môđun trái trên E được liên kết với nó bằng cách viết, với mọi $x \in E$ và mọi phần tử $(n, a) \in A'$,

$$
(n, a) . x = nx + ax.
$$

Ngay lập tức kiểm tra được các tiên đề $(\mathrm{M}_I)$ đến $(\mathrm{M}_{IV})$ của § 1, no. 1, Định nghĩa 1;

hơn nữa, khi hạn chế tập hợp toán tử của cấu trúc môđun này vào $\{0\} \times A$ (được đồng nhất với $A$), ta thu được trên $E$ cấu trúc giả môđun đã cho ban đầu.

Để một tập con $M$ của $E$ là một nhóm con với toán tử của giả môđun $E$ (trong trường hợp đó cấu trúc cảm sinh hiển nhiên cũng là một cấu trúc môđun giả trái trên $A$), điều kiện cần và đủ là $M$ là một môđun con của $A'$-môđun liên kết $E$ và môđun con-$A'$ này được liên kết với giả môđun $M$. Hơn nữa, $A'$-môđun thương $E/M$ khi đó được liên kết với nhóm thương với toán tử $E/M$, hiển nhiên là một giả môđun trên $A$.

Nếu $E, F$ là hai giả môđun trên $A$, thì các đồng cấu $E \to F$ của các nhóm có toán tử đồng nhất với các ánh xạ $A'$-tuyến tính $E \to F$ của các $A'$-môđun liên kết tương ứng với các giả môđun $E$ và $F$. Nếu $(E_i)_{i \in I}$ là một họ giả môđun trên $A$, thì các nhóm có toán tử $\prod_{i \in I} E_i$ và $\bigoplus_{i \in I} E_i$ là các giả môđun trên $A$ và các $A'$-môđun liên kết lần lượt là tích và tổng trực tiếp của các $A'$-môđun liên kết $E_i$. Có các kết quả tương tự đối với các giới hạn nghịch và trực tiếp của các giả môđun. Như vậy, lý thuyết các giả môđun trên $A$ có thể được quy toàn bộ về lý thuyết các $A'$-môđun.

### Bài tập {#alg-ii-a0-exercises}

Xem [các bài tập cho Phụ lục 0](exercises/a0/).
