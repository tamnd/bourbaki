---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 1
section_title: Structures and isomorphisms
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 259-271, 289
pdf_pages: 0264-0276, 0294-0294
extraction: ocr
subsections:
    - "no": 1
      title: ECHELONS
      page: 259
      pdf_page: 264
    - "no": 2
      title: CANONICAL EXTENSIONS OF MAPPINGS
      page: 260
      pdf_page: 265
    - "no": 3
      title: TRANSPORTABLE RELATIONS
      page: 261
      pdf_page: 266
    - "no": 4
      title: SPECIES OF STRUCTURES
      page: 262
      pdf_page: 267
    - "no": 5
      title: ISOMORPHISMS AND TRANSPORT OF STRUCTURES
      page: 264
      pdf_page: 269
    - "no": 6
      title: DEDUCTION OF STRUCTURES
      page: 266
      pdf_page: 271
    - "no": 7
      title: EQUIVALENT SPECIES OF STRUCTURES
      page: 268
      pdf_page: 273
statements: 16
exercises: 1
content_sha256: 1021f8056c046a70b3bb666792892821fb45a0bb3f0f06882964b88441cd9b9e
translated_from: content/en/ens/IV/01_s1_structures_and_isomorphisms.md
source_content_sha256: 72e7a50a926695c09905a33aa4733b05bfba50ebcbc6f53e8ad15ba1695dd9eb
translation_model: gpt-5.4-mini, gpt-5.4
translation_run: translate-vi-5237b20a
glossary_version: 27
glossary_terms_sha256: 3910c7bbb68aa02e527436420c58cbd3e1dcce3859c29648a967c394b670a86c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. CẤU TRÚC VÀ ĐẲNG CẤU

Mục đích của chương này là trình bày một lần và mãi mãi một số phép dựng và chứng minh kiến tạo (xem Chương I, § 1, số 3 và § 2, số 2) vốn xuất hiện rất thường xuyên trong toán học.

### 1. CÁC TẦNG

Một *lược đồ phép dựng các tầng* là một dãy $c_1$, $c_2$, ..., $c_m$ gồm các cặp có thứ tự của các số nguyên tự nhiên (*)[^1] $c_i = (a_i,\ b_i)$, thỏa mãn các điều kiện sau :

(a)　Nếu $b_i = 0$, thì $1 \leqslant a_i \leqslant i - 1$.
(b)　Nếu $a_i \neq 0$ và $b_i \neq 0$, thì $1 \leqslant a_i \leqslant i - 1$ và $1 \leqslant b_i \leqslant i - 1$.

Các điều kiện này kéo theo $c_1 = (0,\ b_1)$, với $b_1 > 0$. Nếu $n$ là số nguyên lớn nhất trong các số nguyên $b_i$ xuất hiện trong các cặp $(0,\ b_i)$, thì $c_1, c_2, ..., c_m$ được gọi là một lược đồ phép dựng dạng bậc thang *trên $n$ số hạng*.

Cho một lược đồ phép dựng bậc thang $\mathrm{S} = (c_1,\ c_2,\ \ldots,\ c_m)$ trên $n$ hạng, và cho $n$ hạng $\mathrm{E}_1$, $\mathrm{E}_2$, ..., $\mathrm{E}_n$ trong một lý thuyết $\mathscr{T}$ mạnh hơn lý thuyết tập hợp, thì một *phép dựng bậc thang theo lược đồ* $\mathrm{S}$ *trên* $\mathrm{E}_1$, ..., $\mathrm{E}_n$ được gọi là một dãy $\mathrm{A}_1$, $\mathrm{A}_2$, ..., $\mathrm{A}_m$ gồm $m$ hạng trong lý thuyết $\mathscr{T}$, được xác định từng bước bởi các điều kiện sau đây:

(a)　Nếu $c_i = (0,\ b_i)$, thì $\mathrm{A}_i$ là số hạng $\mathrm{E}_{b_i}$.
(b)　Nếu $c_i = (a_i,\ 0)$, thì $\mathrm{A}_i$ là số hạng $\mathfrak{P}(\mathrm{A}_{a_i})$.
(c)　Nếu $c_i = (a_i,\ b_i)$, với $a_i \neq 0$ và $b_i \neq 0$, thì $\mathrm{A}_i$ là số hạng $\mathrm{A}_{a_i} \times \mathrm{A}_{b_i}$.

Số hạng cuối cùng $\mathrm{A}_m$ của phép dựng thang của lược đồ S trên $\mathrm{E}_1$, ..., $\mathrm{E}_n$ được gọi là *thang của lược đồ* S *trên các tập hợp cơ sở* $\mathrm{E}_1$, ..., $\mathrm{E}_n$; trong các lập luận tổng quát tiếp theo, nó sẽ được biểu thị bằng ký hiệu $\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n)$.

#### Ví dụ {#ens-iv-s1-n1-exa-1 .statement tag=03V4}

Cho hai tập hợp E, F, tập hợp $\mathfrak{P}(\mathfrak{P}(\mathrm{E})) \times \mathfrak{P}(\mathrm{F})$ là một thang trên E, F, với lược đồ

$$(0, 1), \quad (0, 2), \quad (1, 0), \quad (3, 0), \quad (2, 0), \quad (4, 5).$$

Nó cũng là thang trên E, F với lược đồ

$$(0, 2), \quad (0, 1), \quad (1, 0), \quad (2, 0), \quad (4, 0), \quad (5, 3).$$

Vậy các lược đồ phân biệt có thể cho cùng một thang trên cùng các số hạng.

### 2. CÁC MỞ RỘNG CHÍNH TẮC CỦA ÁNH XẠ

Cho $\mathrm{S} = (c_1, c_2, \ldots, c_m)$ là một lược đồ phép dựng bậc thang trên $n$ hạng. Cho $\mathrm{E}_1$, ..., $\mathrm{E}_n$, $\mathrm{E}'_1$, ..., $\mathrm{E}'_n$ là các tập hợp (các hạng trong $\mathscr{C}$) và cho $f_1$, ..., $f_n$ là các hạng trong $\mathscr{C}$ sao cho các quan hệ "$f_i$ là một ánh xạ từ $\mathrm{E}_i$ vào $\mathrm{E}'_i$" là các định lý trong $\mathscr{C}$ với $1 \leqslant i \leqslant n$. Cho $\mathrm{A}_1$, ..., $\mathrm{A}_m$ (resp. $\mathrm{A}'_1$, ..., $\mathrm{A}'_m$) là phép dựng bậc thang có lược đồ S trên $\mathrm{E}_1$, ..., $\mathrm{E}_n$ (resp. $\mathrm{E}'_1$, ..., $\mathrm{E}'_n$). Ta định nghĩa từng bước một dãy gồm $m$ hạng $g_1$, ..., $g_m$ sao cho $g_i$ là một *ánh xạ từ* $\mathrm{A}_i$ *vào* $\mathrm{A}'_i$ (với $1 \leqslant i \leqslant m$) theo các điều kiện sau :

(a) Nếu $c_i = (0, b_i)$, do đó $\mathrm{A}_i = \mathrm{E}_{b_i}$ và $\mathrm{A}'_i = \mathrm{E}'_{b_i}$, thì $g_i$ là ánh xạ $f_{b_i}$.

(b) Nếu $c_i = (a_i, 0)$, do đó $\mathrm{A}_i = \mathfrak{P}(\mathrm{A}_{a_i})$ và $\mathrm{A}'_i = \mathfrak{P}(\mathrm{A}'_{a_i})$, thì $g_i$ là *mở rộng chính tắc* $\hat{g}_{a_i}$ của $g_{a_i}$ lên các tập hợp các tập con (Chương II, § 5, no. 1).

(c) Nếu $c_i = (a_i, b_i)$, trong đó $a_i \neq 0$ và $b_i \neq 0$, do đó

$$\mathrm{A}_i = \mathrm{A}_{a_i} \times \mathrm{A}_{b_i} \qquad \text{và} \qquad \mathrm{A}'_i = \mathrm{A}'_{a_i} \times \mathrm{A}'_{b_i},$$

then $g_i$ là *mở rộng chính tắc* $g_{a_i} \times g_{b_i}$ của $g_{a_i}$ và $g_{b_i}$ tới $\mathrm{A}_{a_i} \times \mathrm{A}_b$ (Chương II, § 3, số 9).

Số hạng cuối cùng $g_m$ của dãy này được gọi là *mở rộng chính tắc, với lược đồ* S, *của các ánh xạ* $f_1$, ..., $f_n$, và sẽ được ký hiệu bởi $\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$.

¶ Các tiêu chuẩn sau có thể được kiểm tra từng bước :

CST1. *Nếu* $f_i$ *là một ánh xạ từ* $\mathrm{E}_i$ *vào* $\mathrm{E}'_i$, *và nếu* $f'_i$ *là một ánh xạ từ* $\mathrm{E}'_i$ *vào* $\mathrm{E}''_i$ *(*$1 \leqslant i \leqslant n$*), thì với mọi sơ đồ dựng bậc thang S trên* $n$ *số hạng ta có*

$$\langle f'_1 \circ f_1, f'_2 \circ f_2, \ldots, f'_n \circ f_n \rangle^{\mathrm{S}} = \langle f'_1, f'_2, \ldots, f'_n \rangle^{\mathrm{S}} \circ \langle f_1, f_2, \ldots, f_n \rangle^{\mathrm{S}}.$$

CST2. *Nếu $f_i$ là đơn ánh* (tương ứng. *toàn ánh*) *đối với* $1 \leqslant i \leqslant n$, *thì* $\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$ *là đơn ánh* (tương ứng. *toàn ánh*).

Tiêu chuẩn này suy ra từ các tính chất tương ứng của phép mở rộng $\hat{g}$ (Chương II, § 5, no. 1, Mệnh đề 1) và phép mở rộng $g \times h$ (Chương II, § 3, no. 9).

CST3. *Nếu $f_i$ là một song ánh từ* $\mathrm{E}_i$ *lên* $\mathrm{E}'_i$, *và nếu $f_i^{-1}$ là song ánh ngược* (\*)[^2], *thì* $\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$ *là một song ánh và* $\langle f_1^{-1}, \ldots, f_n^{-1} \rangle^{\mathrm{S}}$ *là nghịch đảo của nó; nói cách khác*,

$$(\langle f_1, \ldots, f_n \rangle^{\mathrm{S}})^{-1} = \langle f_1^{-1}, \ldots, f_n^{-1} \rangle^{\mathrm{S}}.$$

Điều này suy ra ngay lập tức từ CST1 và CST2.

### 3. QUAN HỆ CHUYỂN ĐƯỢC

Cho $\mathscr{T}$ là một lý thuyết mạnh hơn lý thuyết tập hợp, $x_1, \ldots, x_n$, $s_1, \ldots, s_p$ là các chữ cái phân biệt và phân biệt với các hằng của $\mathscr{T}$, và $\mathrm{A}_1, \ldots, \mathrm{A}_m$ là các hạng trong $\mathscr{T}$ mà không chữ cái nào trong các chữ cái $x_i$ $(1 \leqslant i \leqslant n)$ và $s_j$ $(1 \leqslant j \leqslant p)$ xuất hiện. Cho $\mathrm{S}_1, \ldots, \mathrm{S}_p$ là các lược đồ phép dựng bậc thang trên $n + m$ hạng. Khi đó quan hệ $\mathrm{T}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ :

"$s_1 \in \mathrm{S}_1(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$ và $s_2 \in \mathrm{S}_2(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$ và $\ldots$ và $s_p \in \mathrm{S}_p(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$"

được gọi là một *phép gán kiểu* của các chữ cái $s_1, \ldots, s_p$.

Cho $\mathrm{R}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ là một quan hệ trong $\mathscr{T}$ chứa một số trong các chữ $x_i$, $s_j$ (và có thể cả các chữ khác nữa). Khi đó R được gọi là *khả chuyển* (*trong* $\mathscr{T}$) *đối với kiểu hóa* T, *coi các* $x_i$ $(1 \leqslant i \leqslant n)$ *là các tập cơ sở chính và các* $\mathrm{A}_h$ $(1 \leqslant h \leqslant m)$ *là các tập cơ sở phụ*, nếu điều kiện sau được thỏa mãn: hãy cho $y_1, \ldots, y_n, f_1, \ldots, f_n$ là các chữ cái phân biệt, khác với các $x_i$ $(1 \leqslant i \leqslant n)$, các $s_j$ $(1 \leqslant j \leqslant p)$, các hằng số của $\mathscr{T}$, và mọi chữ cái xuất hiện trong R hoặc trong các hạng $\mathrm{A}_h$ $(1 \leqslant h \leqslant m)$, và hãy cho $\mathrm{Id}_h$ $(1 \leqslant h \leqslant m)$ ký hiệu ánh xạ đồng nhất của $\mathrm{A}_h$ lên chính nó. Khi đó quan hệ

(1)     "$\mathrm{T}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ và ($f_1$ là một song ánh từ $x_1$ lên $y_1$) và $\ldots$ và ($f_n$ là một song ánh từ $x_n$ lên $y_n$)"

*suy ra, trong* $\mathscr{T}$, *quan hệ*

(2)     $\mathrm{R}\{x_1, \ldots, x_n, s_1, \ldots, s_p\} \Leftrightarrow \mathrm{R}\{y_1, \ldots, y_n, s'_1, \ldots, s'_p\}$,

trong đó

$$(3) \qquad s'_j = \langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^s{}_j(s_j) \qquad (1 \leqslant j \leqslant p).$$

Có một định nghĩa tương tự nhưng đơn giản hơn trong trường hợp không có tập hợp phụ trợ.

Ví dụ, nếu $n = p = 2$ và nếu sự điển hình hóa T là "$s_1 \in x_1$ và $s_2 \in x_1$", thì quan hệ $s_1 = s_2$ là khả chuyển. Mặt khác, quan hệ $x_1 = x_2$ thì không khả chuyển.

### 4. LOÀI CẤU TRÚC

Cho $\mathscr{T}$ là một lý thuyết mạnh hơn lý thuyết tập hợp. *Một loài cấu trúc* trong $\mathscr{T}$ là một văn bản $\Sigma$ được tạo thành từ các dãy ký hiệu sau đây :

(1)  một số chữ cái $x_1, \ldots, x_n, s$, phân biệt đôi một và phân biệt với các hằng của $\mathscr{T}$; $x_1, \ldots, x_n$ được gọi là các *tập hợp cơ sở chính* của loài cấu trúc $\Sigma$;

(2)  một số hạng $\mathrm{A}_1, \ldots, \mathrm{A}_m$ trong $\mathscr{T}$ mà trong đó không chữ cái nào trong các chữ cái $x_1, \ldots, x_n, s$ xuất hiện, và được gọi là các *tập hợp cơ sở phụ trợ* của $\Sigma$; có thể $\Sigma$ không chứa tập hợp cơ sở phụ trợ nào (nhưng nó phải chứa ít nhất một tập hợp cơ sở chính);

(3)  một sự điển hình hóa $\mathrm{T}\{x_1, \ldots, x_n, s\}$ :

$$s \in \mathrm{S}(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m),$$

trong đó S là một lược đồ phép dựng tầng trên $n + m$ hạng (số 1); $\mathrm{T}\{x_1, \ldots, x_n, s\}$ được gọi là *đặc trưng hóa điển hình* của loài cấu trúc $\Sigma$;

(4)  một quan hệ $\mathrm{R}\{x_1, \ldots, x_n, s\}$ *khả chuyển* (trong $\mathscr{T}$) đối với sự điển hình hóa T, trong đó các $x_i$ là các tập hợp cơ sở chính còn các $\mathrm{A}_h$ là các tập hợp cơ sở phụ trợ (số 3); R được gọi là *tiên đề* của loài cấu trúc $\Sigma$.

Lý thuyết $\mathscr{T}_\Sigma$ có cùng các lược đồ tiên đề như $\mathscr{T}$ và có các tiên đề minh thị là các tiên đề của $\mathscr{T}$, cùng với tiên đề "T và R", được gọi là *lý thuyết của loài cấu trúc* $\Sigma$. Do đó, các hằng của $\mathscr{T}_\Sigma$ là các hằng của $\mathscr{T}$ và các chữ xuất hiện trong T hoặc trong R.

¶ Cho $\mathscr{T}'$ là một lý thuyết mạnh hơn $\mathscr{T}$, và cho $\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}$ là các hạng thức trong $\mathscr{T}'$. Trong lý thuyết $\mathscr{T}'$, U được gọi là một *cấu trúc thuộc loài* $\Sigma$ *trên các tập hợp cơ sở chính* $\mathrm{E}_1, \ldots, \mathrm{E}_n$, *với* $\mathrm{A}_1, \ldots, \mathrm{A}_m$ *làm các tập hợp cơ sở phụ*, nếu quan hệ

$$\text{"}\mathrm{T}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\} \text{ và } \mathrm{R}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\}\text{"}$$

là một *định lý trong* $\mathscr{T}'$. Khi đó, với mỗi định lý $\mathrm{B}\{x_1, \ldots, x_n, s\}$ trong lý thuyết $\mathscr{T}_\Sigma$ thì quan hệ $\mathrm{B}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\}$ là một *định lý trong* $\mathscr{T}'$ (Chương I, § 2, no. 3). Trong $\mathscr{T}_\Sigma$, hằng số $s$ được gọi là *cấu trúc tổng quát của loài* $\Sigma$.

¶ Trong lý thuyết $\mathscr{T}'$, các tập hợp cơ sở chính $\mathrm{E}_1, \ldots, \mathrm{E}_n$ được gọi là *được trang bị cấu trúc* $\mathrm{U}$. Rõ ràng, $\mathrm{U}$ là một phần tử của tập hợp

$$\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{A}_1, \ldots, \mathrm{A}_m).$$

Tập hợp các phần tử $\mathrm{V}$ của $\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$ thỏa mãn quan hệ $\mathrm{R}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{V}\}$ do đó là *tập hợp các cấu trúc của loài* $\Sigma$ *trên* $\mathrm{E}_1, \ldots, \mathrm{E}_n$ (và nó có thể rỗng).

*Ví dụ*

#### Ví dụ 1 {#ens-iv-s1-n4-exa-1 .statement tag=03V5}

Lấy $\mathscr{T}$ là lý thuyết tập hợp, và xét loài cấu trúc không có tập hợp cơ sở phụ trợ nào, có một tập hợp cơ sở chính $\mathrm{A}$, đặc trưng hóa điển hình $s \in \mathfrak{P}(\mathrm{A} \times \mathrm{A})$, và tiên đề

$$s \circ s = s \quad \text{và} \quad s \cap \overset{-1}{s} = \Delta_{\mathbf{A}}$$

(trong đó $\Delta_{\mathbf{A}}$ là đường chéo của $\mathrm{A} \times \mathrm{A}$), là một quan hệ khả chuyển đối với sự điển hình hóa $s \in \mathfrak{P}(\mathrm{A} \times \mathrm{A})$, như dễ dàng kiểm tra được. Rõ ràng lý thuyết của loài cấu trúc này chính là lý thuyết về *tập hợp có thứ tự* (Chương III, §1, no. 3); và do đó loài cấu trúc được định nghĩa như thế cũng được gọi là *loài các cấu trúc thứ tự* trên $\mathrm{A}$. Trong Chương III, chúng ta đã thấy nhiều ví dụ về các tập hợp được trang bị những cấu trúc thuộc loài này.

#### Ví dụ 2 {#ens-iv-s1-n4-exa-2 .statement tag=03V6}

Lấy $\mathscr{T}$ là lý thuyết tập hợp, và xét loài cấu trúc không có tập hợp cơ sở phụ, có một tập hợp cơ sở chính $\mathrm{A}$, đặc trưng hóa điển hình $\mathrm{F} \in \mathfrak{P}((\mathrm{A} \times \mathrm{A}) \times \mathrm{A})$, và lấy làm tiên đề quan hệ khả chuyển "F là một đồ thị phiếm hàm có miền là $\mathrm{A} \times \mathrm{A}$". Các cấu trúc của loài này là những trường hợp riêng của các *cấu trúc đại số*, và hàm có đồ thị là $\mathrm{F}$ (một ánh xạ từ $\mathrm{A} \times \mathrm{A}$ vào $\mathrm{A}$) được gọi là *luật* (*được xác định khắp nơi*) *hợp thành trong* của một cấu trúc như vậy.

#### Ví dụ 3 {#ens-iv-s1-n4-exa-3 .statement tag=03V7}

Như trước, cho $\mathscr{T}$ là lý thuyết tập hợp, và xét loài cấu trúc không có tập hợp cơ sở phụ, có một tập hợp cơ sở chính $\mathrm{A}$, đặc trưng hóa điển hình $\mathrm{V} \in \mathfrak{P}(\mathfrak{P}(\mathrm{A}))$, và lấy làm tiên đề quan hệ khả chuyển

$$(\forall \mathrm{V}) \, ((\mathrm{V}' \subset \mathrm{V}) \Rightarrow ((\bigcup_{\mathrm{X} \in \mathrm{V}'} \mathrm{X}) \in \mathrm{V}))$$
$$\text{và} \quad (\forall \mathrm{X})(\forall \mathrm{Y})((\mathrm{X} \in \mathrm{V} \text{ và } \mathrm{Y} \in \mathrm{V}) \Rightarrow ((\mathrm{X} \cap \mathrm{Y}) \in \mathrm{V})).$$

Loài cấu trúc này được gọi là *loài cấu trúc tôpô*. Một cấu trúc của loài này cũng được gọi là một *tôpô*, và quan hệ $\mathrm{X} \in \mathrm{V}$ được diễn đạt bằng cách nói rằng $\mathrm{X}$ là một *tập mở* trong tôpô $\mathrm{V}$ (*Tôpô đại cương*, Chương I, § 1).

#### Ví dụ 4 {#ens-iv-s1-n4-exa-4 .statement tag=03V8}

Lấy $\mathscr{T}$ là lý thuyết của loài các cấu trúc vành chia, có (trong số những thứ khác) một hằng số K làm tập cơ sở duy nhất (chính). Loài cấu trúc của một *không gian vectơ trái trên* K có K làm tập cơ sở phụ, một tập cơ sở chính E, và có làm đặc trưng hóa điển hình quan hệ

$$V \in \mathfrak{P}((E \times E) \times E) \times \mathfrak{P}((K \times E) \times E)$$

(pr$_1$V là đồ thị của phép cộng trong E, và pr$_2$V là đồ thị của phép nhân vô hướng); ở đây chúng tôi sẽ không phát biểu tiên đề của loài cấu trúc này.

#### Ví dụ 5 {#ens-iv-s1-n4-exa-5 .statement tag=03V9}

Lại lấy $\mathscr{T}$ là lý thuyết tập hợp; trong lý thuyết này, trường số phức $\mathbf{C}$ là một số hạng không chứa chữ cái nào. Loài cấu trúc của một *đa tạp giải tích phức chiều n* có $\mathbf{C}$ làm tập cơ sở phụ, và một tập cơ sở chính V. Ở đây chúng tôi sẽ không chỉ ra đặc trưng hóa điển hình cũng như tiên đề của loài cấu trúc này. *

*Chú ý*

#### Nhận xét 1 {#ens-iv-s1-n4-rem-1 .statement tag=03VA}

Trong các ứng dụng, thường xảy ra trường hợp (như trong Ví dụ 4 ở trên) tầng $S(E_1, \ldots, E_n, A_1, \ldots, A_m)$ là một tích của các tầng

$$S_1(E_1, \ldots, A_m) \times \cdots \times S_p(E_1, \ldots, A_m).$$

Nếu vậy, chữ cái $s$ trong định nghĩa của $\Sigma$ thường được thay bằng một "$p$-bộ" $(s_1, \ldots, s_p)$ (x. Chương II, § 2, no. 1).

Hơn nữa, tiên đề của một loài cấu trúc $\Sigma$ thường được viết như một phép hội của nhiều quan hệ chuyển được (như trong Ví dụ 3 ở trên). Các quan hệ này được gọi là *các tiên đề* của loài $\Sigma$.

#### Nhận xét 2 {#ens-iv-s1-n4-rem-2 .statement tag=03VB}

Người ta đặt tên cho các loài cấu trúc được dùng thường xuyên nhất trong toán học, và cho các tập hợp được trang bị các cấu trúc thuộc những loài ấy. Như vậy, một *tập hợp có thứ tự* (Chương III, § 1) là một tập hợp được trang bị một cấu trúc thứ tự (Ví dụ 1); * trong các Quyển sau của bộ sách này, chúng tôi sẽ định nghĩa các khái niệm *nhóm, trường, không gian tôpô, đa tạp khả vi*, v.v., mà tất cả đều chỉ các tập hợp được trang bị những cấu trúc nhất định. *

#### Nhận xét 3 {#ens-iv-s1-n4-rem-3 .statement tag=03VC}

Lạm dụng ngôn ngữ, trong lý thuyết tập hợp $\mathscr{T}$, việc cho $n$ chữ cái phân biệt $x_1, \ldots, x_n$ (không có đặc trưng điển hình và không có tiên đề) được coi là một loài cấu trúc $\Sigma_0$, gọi là *cấu trúc của một tập hợp* trên $n$ tập cơ sở chính $x_1, \ldots, x_n$.

### 5. ĐẲNG CẤU VÀ PHÉP CHUYỂN CẤU TRÚC

Cho $\Sigma$ là một loài cấu trúc trong một lý thuyết $\mathscr{T}$, trên $n$ tập cơ sở chính $x_1, \ldots, x_n$, với $m$ tập cơ sở phụ $A_1, \ldots, A_m$. Cho S là sơ đồ phép dựng bậc thang trên $n + m$ chữ cái xuất hiện trong đặc trưng hóa điển hình của $\Sigma$, và cho R là tiên đề của $\Sigma$. Trong một lý thuyết $\mathscr{T}'$ mạnh hơn $\mathscr{T}$, cho U là một cấu trúc thuộc loài $\Sigma$ trên các tập $E_1, \ldots, E_n$ (làm các tập cơ sở chính) và cho U$'$ là một cấu trúc *thuộc cùng loài* trên các tập $E'_1, \ldots, E'_n$. Cuối cùng, cho $f_i$ (trong $\mathscr{T}'$) là một *song ánh* của $E_i$

lên $\mathrm{E}'_i$ $(1 \leqslant i \leqslant n)$. Khi đó, $(f_1, \ldots, f_n)$ được gọi là một *đẳng cấu* của các tập hợp $\mathrm{E}_1, \ldots, \mathrm{E}_n$, được trang bị cấu trúc U, lên các tập hợp $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$, được trang bị cấu trúc $\mathrm{U}'$, nếu ta có (trong $\mathscr{C}'$)

(4) $$\langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(\mathrm{U}) = \mathrm{U}'$$

trong đó $\mathrm{Id}_h$ ký hiệu ánh xạ đồng nhất của $\mathrm{A}_h$ lên chính nó $(1 \leqslant h \leqslant m)$.

¶ Gọi $f'_i$ là nghịch đảo của song ánh $f_i$ $(1 \leqslant i \leqslant n)$. Từ (4) và tiêu chuẩn CST3 (no. 2) suy ra ngay lập tức rằng ta có

$$\langle f'_1, \ldots, f'_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(\mathrm{U}') = \mathrm{U}$$

và do đó $(f'_1, \ldots, f'_n)$ là một *đẳng cấu* của $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$, được trang bị $\mathrm{U}'$, lên $\mathrm{E}_1, \ldots, \mathrm{E}_n$, được trang bị U. Các đẳng cấu $(f_1, \ldots, f_n)$ và $(f'_1, \ldots, f'_n)$ được gọi là *nghịch đảo* của nhau.

$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$, được trang bị $\mathrm{U}'$, được gọi là *đẳng cấu* với $\mathrm{E}_1, \ldots, \mathrm{E}_n$, được trang bị U, nếu tồn tại một đẳng cấu của $\mathrm{E}_1, \ldots, \mathrm{E}_n$ lên $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$; trong trường hợp này các cấu trúc U và $\mathrm{U}'$ được gọi là *đẳng cấu*.

¶ Các định nghĩa trên, cùng với CST1, kéo theo tiêu chuẩn sau:

CST4. *Cho* U, $\mathrm{U}'$, $\mathrm{U}''$ *là ba cấu trúc cùng loài* $\Sigma$ *trên các tập hợp cơ sở chính* $\mathrm{E}_1, \ldots, \mathrm{E}_n$, $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$, $\mathrm{E}''_1, \ldots, \mathrm{E}''_n$, *tương ứng. Cho* $f_i$ *là một song ánh từ* $\mathrm{E}_i$ *lên* $\mathrm{E}'_i$, *và cho* $g_i$ *là một song ánh từ* $\mathrm{E}'_i$ *lên* $\mathrm{E}''_i$ $(1 \leqslant i \leqslant n)$. *Nếu* $(f_1, \ldots, f_n)$ *và* $(g_1, \ldots, g_n)$ *là các đẳng cấu, thì* $(g_1 \circ f_1, \ldots, g_n \circ f_n)$ *cũng vậy*.

Một đẳng cấu của $\mathrm{E}_1, \ldots, \mathrm{E}_n$ onto $\mathrm{E}_1, \ldots, \mathrm{E}_n$ (với cùng một cấu trúc) được gọi là một *tự đẳng cấu* của $\mathrm{E}_1, \ldots, \mathrm{E}_n$. Hợp thành của hai tự đẳng cấu của $\mathrm{E}_1, \ldots, \mathrm{E}_n$ là một tự đẳng cấu, và nghịch đảo của một tự đẳng cấu cũng vậy, \* nên các tự đẳng cấu của $\mathrm{E}_1, \ldots, \mathrm{E}_n$ lập thành một *nhóm*. \*

#### Nhận xét {#ens-iv-s1-n5-rem-1 .statement tag=03VD}

Do dùng từ theo nghĩa rộng, nếu $f_i$ là bất kỳ song ánh nào của $\mathrm{E}_i$ onto $\mathrm{E}'_i$ $(1 \leqslant i \leqslant n)$, thì $(f_1, \ldots, f_n)$ được gọi là một đẳng cấu của $\mathrm{E}_1, \ldots, \mathrm{E}_n$ onto $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ đối với loài cấu trúc của một tập hợp (số 4, Chú ý 3).

CST5. *Trong một lý thuyết* $\mathscr{C}'$ *mạnh hơn* $\mathscr{C}$, *cho* U *là một cấu trúc thuộc loài* $\Sigma$ *trên* $\mathrm{E}_1, \ldots, \mathrm{E}_n$, *và cho* $f_i$ *là một song ánh của* $\mathrm{E}_i$ *lên một tập hợp* $\mathrm{E}'_i$ $(1 \leqslant i \leqslant n)$. *Khi đó tồn tại một cấu trúc duy nhất thuộc loài* $\Sigma$ *trên* $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ *sao cho* $(f_1, \ldots, f_n)$ *là một đẳng cấu của* $\mathrm{E}_1, \ldots, \mathrm{E}_n$ *lên* $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$।

Với cấu trúc này, nếu nó tồn tại, chỉ có thể là số hạng $\mathrm{U}'$ được định nghĩa bởi quan hệ (4); còn phải kiểm tra rằng số hạng này thực sự là một cấu trúc thuộc loài $\Sigma$, nghĩa là quan hệ $\mathrm{R}\{\mathrm{E}'_1, \ldots, \mathrm{E}'_n, \mathrm{U}'\}$ là đúng trong $\mathscr{C}'$. Nhưng điều này suy ra từ việc $\mathrm{R}\{x_1, \ldots, x_n, s\}$ là *khả chuyển*, vì

$R\{E'_1, \ldots, E'_n, U'\}$ tương đương trong $\mathscr{T}'$ với quan hệ $R\{E_1, \ldots, E_n, U\}$ (no. 3), quan hệ này đúng trong $\mathscr{T}'$ theo giả thiết.

¶ Cấu trúc $U'$ được gọi là thu được bằng cách *chuyển cấu trúc* $U$ *sang các tập hợp* $E'_1, \ldots, E'_n$ *nhờ các ánh xạ song ánh* $f_1, \ldots, f_n$. Như vậy hai cấu trúc cùng một loài là đẳng cấu khi và chỉ khi mỗi cấu trúc thu được từ cấu trúc kia bằng phép chuyển cấu trúc.

Có thể xảy ra rằng *bất kỳ* hai cấu trúc của loài $\Sigma$ đều *tất yếu đẳng cấu*; khi đó loài cấu trúc $\Sigma$ được gọi là *đơn trị*. \* Điều này đúng với cấu trúc của một nhóm cyclic vô hạn (đẳng cấu với $\mathbf{Z}$), cấu trúc của một trường nguyên tố có đặc số không (đẳng cấu với $\mathbf{Q}$), cấu trúc của một trường có thứ tự Acsimét đầy đủ (đẳng cấu với $\mathbf{R}$), cấu trúc của một trường tôpô đóng đại số, liên thông, địa phương compact (đẳng cấu với $\mathbf{C}$), và cấu trúc của một vành chia tôpô không giao hoán, liên thông, địa phương compact (đẳng cấu với $\mathbf{H}$, vành chia của các quaternion). Đối với một số loài cấu trúc ấy, chẳng hạn như loài của một trường nguyên tố có đặc số không, hoặc loài của một trường có thứ tự Acsimét đầy đủ, thậm chí không có tự đẳng cấu nào khác ngoài ánh xạ đồng nhất; nhưng ở các ví dụ khác nêu trên thì vẫn có những tự đẳng cấu như vậy (chẳng hạn, phép đối xứng $x \rightarrow -x$ trong $\mathbf{Z}$). \*

Có thể nhận thấy rằng các loài cấu trúc trên về cơ bản chính là những cấu trúc làm nền tảng cho toán học cổ điển. Mặt khác, \* loài cấu trúc nhóm, loài cấu trúc của một tập hợp có thứ tự, và loài cấu trúc tôpô, đều không đơn trị. \*

### 6. SUY DIỄN CÁC CẤU TRÚC

Cho $\Sigma$ là một loài cấu trúc trong một lý thuyết $\mathscr{T}$, trên $n$ tập hợp cơ sở chính $x_1, \ldots, x_n$, với $m$ tập hợp cơ sở phụ $A_1, \ldots, A_m$. Gọi $s$ là cấu trúc tổng quát của $\Sigma$, và gọi $T$ là một lược đồ phép dựng theo bậc trên $n + m$ số hạng. Một số hạng $V\{x_1, \ldots, x_n, s\}$ không chứa chữ cái nào khác ngoài các hằng của $\mathscr{T}_\Sigma$ được gọi là *nội tại* đối với $s$, thuộc kiểu $T(x_1, \ldots, x_n, A_1, \ldots, A_m)$, nếu nó thỏa mãn các điều kiện sau :

(1) quan hệ $V\{x_1, \ldots, x_n, s\} \in T(x_1, \ldots, x_n, A_1, \ldots, A_m)$ là một định lý trong $\mathscr{T}_\Sigma$;

(2) gọi $\mathscr{T}'_\Sigma$ là lý thuyết thu được bằng cách bổ sung vào các tiên đề của $\mathscr{T}_\Sigma$ các tiên đề "$f_i$ là một song ánh từ $x_i$ lên $y_i$" $(1 \leqslant i \leqslant n)$ (trong đó các chữ $y_i$ và $f_i$ phân biệt với nhau và phân biệt với các hằng của $\mathscr{T}_\Sigma$, với $1 \leqslant i \leqslant n$); nếu $s'$ là cấu trúc thu được bằng cách chuyển $s$ theo $(f_1, \ldots, f_n)$ (no. 5), thì

$$V\{y_1, \ldots, y_n, s'\} = \langle f_1, \ldots, f_n. \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{T}}(V\{x_1, \ldots, x_n, s\})$$

là một định lý trong $\mathscr{T}'_\Sigma$.

Phần lớn các thuật ngữ mà người ta được dẫn tới việc định nghĩa trong lý thuyết của một loài cấu trúc đều là những thuật ngữ nội tại.

Cho $\Theta$ là một loài cấu trúc khác trong lý thuyết $\mathscr{T}$, trên $r$ tập hợp cơ sở chính $u_1$, ..., $u_r$, với $p$ tập hợp cơ sở phụ $\mathrm{B}_1$, ..., $\mathrm{B}_p$, và cho $t \in \mathrm{T}(u_1, \ldots, u_r, \mathrm{B}_1, \ldots, \mathrm{B}_p)$ là đặc trưng hóa điển hình của $\Theta$ (số 4). Khi đó, một hệ gồm $r + 1$ số hạng $\mathrm{P}, \mathrm{U}_1, \ldots, \mathrm{U}_r$, *nội tại đối với* $s$, và sao cho $\mathrm{P}$ là một cấu trúc thuộc loài $\Theta$ trên $\mathrm{U}_1$, ..., $\mathrm{U}_r$, *trong lý thuyết* $\mathscr{T}_\Sigma$, được gọi là một *thủ tục suy diễn một cấu trúc thuộc loài* $\Theta$ *từ một cấu trúc thuộc loài* $\Sigma$. Do dùng theo lối nói rộng, riêng số hạng $\mathrm{P}$ thường cũng được gọi là một thủ tục suy diễn.

¶ Cho $\mathscr{T}'$ là một lý thuyết mạnh hơn $\mathscr{T}$. Nếu $\mathscr{S}$ là một cấu trúc trong $\mathscr{T}'$ thuộc loài $\Sigma$ trên $\mathrm{E}_1, \ldots, \mathrm{E}_n$, thì $\mathrm{P}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathscr{S}\}$ là một cấu trúc thuộc loài $\Theta$ trên $r$ tập hợp $\mathrm{F}_j = \mathrm{U}_j\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathscr{S}\}\,(1 \leqslant j \leqslant r)$, được gọi là *suy ra từ* $\mathscr{S}$ *bởi thủ tục* $\mathrm{P}$, *hoặc phụ thuộc vào* $\mathscr{S}$. Giả thiết rằng các hạng $\mathrm{P}, \mathrm{U}_1, \ldots, \mathrm{U}_r$ là nội tại đối với $s$ còn kéo theo tiêu chuẩn sau :

CST6. *Cho* $(g_1, \ldots, g_n)$ *là một đẳng cấu của* $\mathrm{E}_1$, ..., $\mathrm{E}_n$, *được trang bị một cấu trúc* $\mathscr{S}$ *thuộc loài* $\Sigma$, *lên* $\mathrm{E}'_1$, ..., $\mathrm{E}'_n$, *được trang bị một cấu trúc* $\mathscr{S}'$ *thuộc cùng loài. Nếu* $\mathrm{U}_j$ *thuộc kiểu* $\mathfrak{P}(\mathrm{T}_j)$, *đặt*

$$h_j = \langle g_1, \ldots, g_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{T}_j} \ (1 \leqslant j \leqslant r),$$

*và đặt* $\mathrm{F}'_j = \mathrm{U}_j\{\mathrm{E}'_1, \ldots, \mathrm{E}'_n, \mathscr{S}'\}\,(1 \leqslant j \leqslant r)$. *Khi đó* $(h_1, \ldots, h_r)$ *là một đẳng cấu từ* $\mathrm{F}_1$, ..., $\mathrm{F}_r$ *lên* $\mathrm{F}'_1$, ..., $\mathrm{F}'_r$ *khi các hệ tập hợp này được trang bị các cấu trúc thuộc loài* $\Theta$ *suy ra từ* $\mathscr{S}$ *và* $\mathscr{S}'$ *theo thứ tự bằng thủ tục* $\mathrm{P}$.

Hiển nhiên là các hạng $x_1, \ldots, x_n$ là nội tại đối với $s$. Trong nhiều trường hợp, các hạng $\mathrm{U}_1, \ldots, \mathrm{U}_r$ là một số trong các chữ $x_1, \ldots, x_n$; khi đó cấu trúc thuộc loài $\Theta$ suy ra từ $s$ bởi thủ tục $\mathrm{P}$ được gọi là một cấu trúc *nền* của $s$.

*Ví dụ*

#### Ví dụ 1 {#ens-iv-s1-n6-exa-1 .statement tag=03VE}

Loài các cấu trúc *nhóm tôpô* có một tập hợp cơ sở chính duy nhất A, không có tập hợp cơ sở phụ trợ nào, và cấu trúc tổng quát tương ứng là một cặp $(s_1, s_2)$ ($s_1$ là đồ thị của luật hợp thành trên A, còn $s_2$ là tập hợp các tập hợp mở trong tôpô của A; xem *Tôpô đại cương*, Chương III, § 1). Mỗi hạng trong hai hạng $s_1$, $s_2$ là một thủ tục suy diễn và lần lượt cho cấu trúc *nhóm* và *tôpô* nền của cấu trúc nhóm tôpô $(s_1, s_2)$.

Tương tự, từ một cấu trúc không gian vectơ có thể suy ra một cấu trúc nhóm giao hoán nền. Từ một cấu trúc vành có thể suy ra một cấu trúc nhóm giao hoán nền và một cấu trúc nửa nhóm (nhân)

nền. Từ cấu trúc của một đa tạp khả vi có thể suy ra một tôpô nền, v.v.

#### Ví dụ 2 {#ens-iv-s1-n6-exa-2 .statement tag=03VF}

Loài các cấu trúc không gian vectơ trên $\mathbf{C}$ (resp. $\mathbf{R}$) có một tập hợp cơ sở chính E, một tập hợp cơ sở phụ bằng $\mathbf{C}$ (resp. $\mathbf{R}$), và đặc trưng hóa điển hình

$$s_1 \in \mathfrak{P}((\mathrm{E} \times \mathrm{E}) \times \mathrm{E}) \quad \text{và} \quad s_2 \in \mathfrak{P}((\mathbf{C} \times \mathrm{E}) \times \mathrm{E})$$

(resp. $\quad s_1 \in \mathfrak{P}((\mathrm{E} \times \mathrm{E}) \times \mathrm{E}) \quad \text{và} \quad s_2 \in \mathfrak{P}((\mathbf{R} \times \mathrm{E}) \times \mathrm{E}))$.

Cặp $(s_1, s_2 \cap ((\mathbf{R} \times \mathrm{E}) \times \mathrm{E}))$ là một thủ tục suy diễn một cấu trúc không gian vectơ trên $\mathbf{R}$ từ một cấu trúc không gian vectơ trên $\mathbf{C}$ ("hạn chế của trường vô hướng xuống $\mathbf{R}$"). ∗

#### Ví dụ 3 {#ens-iv-s1-n6-exa-3 .statement tag=03VG}

Giả sử rằng $\Theta$ có *cùng* các tập hợp cơ sở (chính và phụ trợ) như $\Sigma$, và *cùng* đặc trưng hóa điển hình. Hơn nữa, nếu tiên đề của $\Sigma$ *hàm ý* (trong $\mathscr{T}$) tiên đề của $\Theta$, thì rõ ràng số hạng $s$ là một thủ tục suy diễn một cấu trúc thuộc loài $\Theta$ từ một cấu trúc thuộc loài $\Sigma$. Khi đó người ta nói rằng $\Theta$ *nghèo hơn* $\Sigma$, và $\Sigma$ *giàu hơn* $\Theta$. Khi ấy, mọi cấu trúc thuộc loài $\Sigma$, trong một lý thuyết $\mathscr{T}'$ mạnh hơn $\mathscr{T}$, cũng là một cấu trúc thuộc loài $\Theta$. Chẳng hạn, loài cấu trúc của các tập hợp *được sắp thứ tự toàn phần* (thu được bằng cách lấy làm tiên đề phép hội của tiên đề về các cấu trúc thứ tự (no. 4, Ví dụ 1) và quan hệ $s \cup \overset{-1}{s} = \mathrm{A} \times \mathrm{A}$) giàu hơn loài cấu trúc thứ tự. ∗Loài cấu trúc nhóm giao hoán giàu hơn loài cấu trúc nhóm. Loài cấu trúc không gian tôpô compact giàu hơn loài cấu trúc tôpô, v.v. ∗

∗ (4) Khi mỗi $\Sigma$ và $\Theta$ là loài các cấu trúc nhóm (tương ứng các cấu trúc vành), trong đại số có định nghĩa một thủ tục suy diễn gắn với mỗi cấu trúc nhóm (tương ứng cấu trúc vành) cấu trúc nhóm (tương ứng cấu trúc vành) trên *tâm* của nó. Khi $\Sigma$ là loài các cấu trúc không gian vectơ trên một trường K, và khi $\Theta$ là loài các cấu trúc đại số trên K, có những thủ tục suy diễn gắn với mỗi không gian vectơ trên K *đại số tenxơ* hoặc *đại số ngoài* của nó. Về sau trong chuỗi này chúng ta sẽ gặp nhiều ví dụ khác nữa. ∗

#### Nhận xét {#ens-iv-s1-n6-rem-1 .statement tag=03VH}

Khi P là một "$q$-bộ" $(\mathrm{P}_1, \ldots, \mathrm{P}_q)$, người ta cũng nói rằng các hạng $\mathrm{P}_1, \ldots, \mathrm{P}_q$ tạo thành một thủ tục suy diễn của một cấu trúc thuộc loài $\Theta$ từ một cấu trúc thuộc loài $\Sigma$.

### 7. CÁC LOẠI CẤU TRÚC TƯƠNG ĐƯƠNG

Cho $\Sigma$ và $\Theta$ là hai loài cấu trúc, trong cùng một lý thuyết $\mathscr{T}$, có *cùng* các tập cơ sở chính $x_1, \ldots, x_n$. Gọi $s, t$ là các cấu trúc điển hình của các loài $\Sigma$, $\Theta$ tương ứng. Giả sử rằng các điều kiện sau được thỏa mãn :

(1) Ta có một thủ tục suy diễn $\mathrm{P}\{x_1, \ldots, x_n, s\}$ của một cấu trúc thuộc loài $\Theta$ trên $x_1, \ldots, x_n$ từ một cấu trúc thuộc loài $\Sigma$ trên $x_1, \ldots, x_n$.

(2) Ta có một thủ tục suy diễn $Q\,\{x_1, \ldots, x_n, t\}$ của một cấu trúc thuộc loài $\Sigma$ trên $x_1, \ldots, x_n$ từ một cấu trúc thuộc loài $\Theta$ trên $x_1, \ldots, x_n$.

(3) Quan hệ $Q\,\{x_1, \ldots, x_n, P\{x_1, \ldots, x_n, s\}\} = s$ là một định lý trong $\mathscr{T}_\Sigma$, và quan hệ $P\{x_1, \ldots, x_n, Q\,\{x_1, \ldots, x_n, t\}\} = t$ là một định lý trong $\mathscr{T}_\Theta$.

Loài cấu trúc $\Sigma$ và $\Theta$ khi đó được gọi là *tương đương nhờ các thủ tục suy diễn* P và Q. Trong trường hợp này, với mọi định lý $B\{x_1, \ldots, x_n, s\}$ trong lý thuyết $\mathscr{T}_\Sigma$, quan hệ $B\{x_1, \ldots, x_n, Q\}$ là một định lý trong $\mathscr{T}_\Theta$; và ngược lại, với mọi định lý $C\{x_1, \ldots, x_n, t\}$ trong lý thuyết $\mathscr{T}_\Theta$, quan hệ $C\{x_1, \ldots, x_n, P\}$ là một định lý trong $\mathscr{T}_\Sigma$.

Nếu U là một cấu trúc thuộc loài $\Sigma$, thì cấu trúc suy ra từ U bằng thủ tục P được gọi là *tương đương* với U. Tiêu chuẩn CST6 suy ra điều sau đây :

CST7. *Cho $\mathscr{S}$, $\mathscr{S}'$ là hai cấu trúc thuộc loài $\Sigma$ trên các tập hợp cơ sở chính $(\mathrm{E}_1, \ldots, \mathrm{E}_n)$, $(\mathrm{E}'_1, \ldots, \mathrm{E}'_n)$, tương ứng. Cho $\mathscr{S}_0$, $\mathscr{S}'_0$ là các cấu trúc thuộc loài $\Theta$ tương ứng tương đương với $\mathscr{S}$ và $\mathscr{S}'$. Điều kiện cần thiết và đủ để $(g_1, \ldots, g_n)$ là một đẳng cấu đối với các cấu trúc $\mathscr{S}_0$ và $\mathscr{S}'_0$ là $(g_1, \ldots, g_n)$ là một đẳng cấu đối với các cấu trúc $\mathscr{S}$ và $\mathscr{S}'$.*

Trong thực hành, chúng tôi không phân biệt giữa các lý thuyết $\mathscr{T}_\Sigma$ và $\mathscr{T}_\Theta$ của hai loài cấu trúc tương đương.

*Ví dụ*

#### Ví dụ 1 {#ens-iv-s1-n7-exa-1 .statement tag=03VI}

Cho $\Sigma$ là loài các cấu trúc nhóm giao hoán; $\Sigma$ có một tập hợp cơ sở (chính) duy nhất A, và cấu trúc tổng quát của nó gồm một chữ duy nhất F; đặc trưng hóa điển hình của $\Sigma$ là $F \in \mathfrak{P}((A \times A) \times A)$, và ta ký hiệu tiên đề của $\Sigma$ bởi $R\,\{A, F\}$. Tiên đề này kéo theo đặc biệt rằng F là đồ thị của một hàm (luật hợp thành của nhóm; xem số 4, Ví dụ 2). Trong lý thuyết $\mathscr{T}_\Sigma$ (trong đó $\mathscr{T}$ ký hiệu lý thuyết tập hợp) ta định nghĩa một số hạng $M\{A, F\}$ là một đồ thị phiếm hàm trong $\mathfrak{P}((\mathbf{Z} \times A) \times A)$ và thỏa mãn quan hệ sau đây $B\{M, A, F\}$ :

$$(\forall x)(\forall y)(\forall n)((x \in A \text{ và } y \in A \text{ và } n \in \mathbf{Z})$$
$$\Rightarrow (M(n,\ F(x,\ y)) = F(M(n,\ x),\ M(n,\ y))))$$
$$\text{và} \quad (\forall x)(\forall m)(\forall n)((x \in A \text{ và } m \in \mathbf{Z} \text{ và } n \in \mathbf{Z})$$
$$\Rightarrow (M(m + n,\ x) = F(M(m,\ x),\ M(n,\ x))))$$
$$\text{và} \quad (\forall x)(\forall m)(\forall n)((x \in A \text{ và } m \in \mathbf{Z} \text{ và } n \in \mathbf{Z})$$
$$\Rightarrow (M(m,\ M(n,\ x)) = M(mn,\ x)))$$
$$\text{và} \qquad (\forall x)((x \in A) \Rightarrow (M(1,\ x) = x)).$$

("phép nhân của một phần tử của A với một số nguyên").

Xét loài $\Theta$ của các cấu trúc $\mathbf{Z}$-*môđun*, loài này có một tập hợp cơ sở chính duy nhất A, với $\mathbf{Z}$ làm tập hợp phụ trợ, và cấu-

trúc khái quát của nó chứa hai chữ G, L, với đặc trưng hóa điển hình

$$\mathrm{G} \in \mathfrak{P}((\mathrm{A} \times \mathrm{A}) \times \mathrm{A}) \quad \text{và} \quad \mathrm{L} \in \mathfrak{P}((\mathbf{Z} \times \mathrm{A}) \times \mathrm{A})$$

và tiên đề

"$\mathrm{R}\{\mathrm{A},\ \mathrm{G}\}$ và (L là một đồ thị phiếm hàm) và $\mathrm{B}\{\mathrm{L},\ \mathrm{A},\ \mathrm{G}\}$".

Người ta kiểm tra ngay lập tức rằng các số hạng F, M cấu thành một thủ tục suy diễn một cấu trúc thuộc loài $\Theta$ từ một cấu trúc thuộc loài $\Sigma$, và rằng số hạng G là một thủ tục suy diễn một cấu trúc thuộc loài $\Sigma$ từ một cấu trúc thuộc loài $\Theta$. Hơn nữa, điều kiện (3) ở trên được thỏa mãn một cách hiển nhiên. Do đó ta có thể nói rằng loài các cấu trúc nhóm giao hoán và loài các cấu trúc $\mathbf{Z}$-môđun là tương đương.

#### Ví dụ 2 {#ens-iv-s1-n7-exa-2 .statement tag=03VJ}

Cho $\Sigma$ là loài các cấu trúc tôpô (số 4, Ví dụ 3), cho A là tập hợp cơ sở (chính), và cho V là cấu trúc tổng quát của $\Sigma$. Xét quan hệ

$$x \in \mathrm{A} \text{ và } \mathrm{X} \subset \mathrm{A} \text{ và } (\forall \mathrm{U})((\mathrm{U} \in \mathrm{V} \text{ và } x \in \mathrm{U}) \Rightarrow (\mathrm{X} \cap \mathrm{U} \neq \emptyset)).$$

Quan hệ này có một đồ thị $\mathrm{P} \subset \mathfrak{P}(\mathrm{A}) \times \mathrm{A}$ đối với cặp $(\mathrm{X},\ x)$; $\mathrm{P}\{\mathrm{A},\ \mathrm{V}\}$ là một số hạng được gọi là "tập hợp của mọi cặp $(\mathrm{X},\ x)$ sao cho $x$ thuộc *bao đóng* của X đối với tôpô V". Khi đó có thể chứng minh (xem *Topologie Générale*, Chương I, § 1) rằng các quan hệ sau là các định lý trong $\mathscr{C}_\Sigma$ :

$$\mathrm{P}(\emptyset) = \emptyset,$$
$$(\forall \mathrm{Y})((\mathrm{Y} \subset \mathrm{A}) \Rightarrow (\mathrm{Y} \subset \mathrm{P}(\mathrm{Y}))),$$
$$(\forall \mathrm{Y})((\mathrm{Y} \subset \mathrm{A}) \Rightarrow (\mathrm{P}(\mathrm{P}(\mathrm{Y})) = \mathrm{P}(\mathrm{Y}))),$$
$$(\forall \mathrm{Y})(\forall \mathrm{Z})((\mathrm{Y} \subset \mathrm{A} \text{ và } \mathrm{Z} \subset \mathrm{A}) \Rightarrow (\mathrm{P}(\mathrm{Y} \cup \mathrm{Z}) = \mathrm{P}(\mathrm{Y}) \cup \mathrm{P}(\mathrm{Z}))).$$

Xét loài cấu trúc $\Theta$, có một tập cơ sở (chính) duy nhất A, mà cấu trúc điển hình của nó gồm một chữ W duy nhất, có đặc trưng điển hình $\mathrm{W} \in \mathfrak{P}(\mathfrak{P}(\mathrm{A}) \times \mathrm{A})$ và tiên đề là

$$\mathrm{W}(\emptyset) = \emptyset \quad \text{và} \quad (\forall \mathrm{Y})((\mathrm{Y} \subset \mathrm{A}) \Rightarrow (\mathrm{Y} \subset \mathrm{W}(\mathrm{Y})))$$
và $\qquad (\forall \mathrm{Y})((\mathrm{Y} \subset \mathrm{A}) \Rightarrow (\mathrm{W}(\mathrm{W}(\mathrm{Y})) = \mathrm{W}(\mathrm{Y})))$
và $\quad (\forall \mathrm{Y})(\forall \mathrm{Z})((\mathrm{Y} \subset \mathrm{A} \quad \text{và} \quad \mathrm{Z} \subset \mathrm{A}) \Rightarrow (\mathrm{W}(\mathrm{Y} \cup \mathrm{Z}) = \mathrm{W}(\mathrm{Y}) \cup \mathrm{W}(\mathrm{Z}))).$

Xét thêm quan hệ

$$\mathrm{U} \subset \mathrm{A} \quad \text{và} \quad (\forall x)((x \in \mathrm{U}) \Rightarrow x \notin \mathrm{W}(\mathrm{A} - \mathrm{U})).$$

Tập hợp tất cả $\mathrm{U} \in \mathfrak{P}(\mathrm{A})$ thỏa mãn quan hệ này là một tập con $\mathrm{Q}\{\mathrm{A},\ \mathrm{W}\}$ của $\mathfrak{P}(\mathrm{A})$. Ta có thể chứng minh (*Tôpô tổng quát*, chương I, § 1, bài tập 10) rằng các quan hệ sau là những định lý trong $\mathscr{C}_\Theta$ :

$$\mathrm{A} \in \mathrm{Q},$$
$$(\forall \mathrm{M})((\mathrm{M} \subset \mathrm{Q}) \Rightarrow \left(\left(\bigcup_{\mathrm{X} \in \mathrm{M}} \mathrm{X}\right) \in \mathrm{Q}\right),$$
$$(\forall \mathrm{X})(\forall \mathrm{Y})((\mathrm{X} \in \mathrm{Q} \text{ và } \mathrm{Y} \in \mathrm{Q}) \Rightarrow ((\mathrm{X} \cap \mathrm{Y}) \in \mathrm{Q})).$$

Do đó các hạng $\mathrm{P}\{\mathrm{A}, \mathrm{V}\}$ và $\mathrm{Q}\{\mathrm{A}, \mathrm{W}\}$ thỏa mãn các điều kiện (1) và (2) ở trên, và dễ thấy rằng chúng cũng thỏa mãn điều kiện (3). Vậy các loài cấu trúc $\Sigma$ và $\Theta$ là tương đương, và do đó chúng tôi coi mọi cấu trúc thuộc loài $\Theta$ như một tôpô, tức là tôpô tương ứng với nó theo thủ tục suy diễn $\mathrm{Q}\{\mathrm{A}, \mathrm{W}\}$. ∗

### Bài tập {#ens-iv-s1-exercises}

Xem [bài tập cho § 1](exercises/s1/).

[^1]: (*) Chúng tôi dùng khái niệm số nguyên theo cùng cách như trong Chương I, nghĩa là theo nghĩa siêu toán học, như những dấu được sắp xếp theo một thứ tự nhất định; cách dùng này không có gì liên quan đến lý thuyết toán học về số nguyên đã được phát triển trong Chương III.
[^2]: (\*) Vì những lý do sắp chữ, ở đây chúng tôi viết $f^{-1}$ thay cho $\overset{-1}{f}$.
