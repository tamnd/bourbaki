---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 5
section_title: Decomposable linear Lie algebras
lang: vi
source: lie-vii-ix
book_pages: 34-45, 63-66
pdf_pages: 0044-0055, 0072-0075
extraction: native
subsections:
    - "no": 1
      title: DECOMPOSABLE LINEAR LIE ALGEBRAS
      page: 34
      pdf_page: 44
    - "no": 2
      title: DECOMPOSABLE ENVELOPE
      page: 37
      pdf_page: 47
    - "no": 3
      title: DECOMPOSITIONS OF DECOMPOSABLE ALGEBRAS
      page: 37
      pdf_page: 47
    - "no": 4
      title: LINEAR LIE ALGEBRAS OF NILPOTENT ENDOMORPHISMS
      page: 39
      pdf_page: 49
    - "no": 5
      title: CHARACTERIZATIONS OF DECOMPOSABLE LIE ALGEBRAS
      page: 43
      pdf_page: 53
statements: 29
exercises: 11
content_sha256: dee7e8cb1e1ee6b070aa1127bac339907b57e1cfdc7f90ee3d2b75b36a518dfb
translated_from: content/en/lie/VII/05_s5_decomposable_linear_lie_algebras.md
source_content_sha256: f39f78e5e768eaa875cc9e5c66d099af4d6fb213b7eac794d0dda54d2fbca97d
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-72ce60e8
glossary_version: 34
glossary_terms_sha256: 8e682e197c3b38ee9b700f541de66b2fa33f41bfa523704a11ecd293fa05504d
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. CÁC ĐẠI SỐ LIE TUYẾN TÍNH PHÂN TÍCH ĐƯỢC

Trong đoạn này, $k$ được giả sử có đặc số 0. Ta ký hiệu V là một không gian vectơ hữu hạn chiều.

### 1. CÁC ĐẠI SỐ LIE TUYẾN TÍNH PHÂN TÍCH ĐƯỢC

#### Định nghĩa 1 {#lie-vii-s5-def-1 .statement tag=00WG}

Cho $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$. Khi đó $\mathfrak{g}$ được gọi là phân tích được nếu $\mathfrak{g}$ chứa các thành phần nửa đơn và lũy linh của mỗi phần tử của nó (Đại số, Chương VII, §5, no. 8).

#### Ví dụ 1 {#lie-vii-s5-n1-exa-1 .statement tag=00WH}

Cho $V'$ và $V''$ là các không gian vectơ con của V sao cho $V''\supset V'$. Tập hợp các $x\in \mathfrak{g}\mathfrak{l}(V)$ sao cho $x(V'')\subset V'$ là một đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V)$; thật vậy, với mọi $x\in \mathfrak{g}\mathfrak{l}$(V), các thành phần nửa đơn và lũy linh của $x$ có dạng $P(x)$ và $Q(x)$, trong đó P và Q là các đa thức không có số hạng hằng.

#### Ví dụ 2 {#lie-vii-s5-n1-exa-2 .statement tag=00WI}

Giả sử rằng V có một cấu trúc đại số. Tập hợp các đạo hàm của V là một đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V) ($§1, no. 1, Mệnh đề 4 (ii)).

#### Ví dụ 3 {#lie-vii-s5-n1-exa-3 .statement tag=01KQ}

Nói chung hơn, có thể chứng minh rằng đại số Lie của bất kỳ nhóm con đại số nào của $\mathbf{G}\mathbf{L}(V)$ đều là phân tích được.$_*$

#### Mệnh đề 1 {#lie-vii-s5-prop-1 .statement tag=00WJ}

Cho $\mathfrak{g}$ là một đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V),x\in \mathfrak{g},s$ và $n$ là các thành phần nửa đơn và lũy linh của $x$.

(i) Các thành phần nửa đơn và lũy linh của ad$_{\mathfrak{g}}x$ lần lượt là ad$_{\mathfrak{g}}s$ và ad$_{\mathfrak{g}}n$.

(ii) $x$ là chính quy trong $\mathfrak{g}$ khi và chỉ khi $s$ là chính quy.

(iii) Nếu $\mathfrak{g}'$ là một đại số con của $\mathfrak{g}\mathfrak{l}(V)$ chứa $\mathfrak{g}$, mọi tự đẳng cấu sơ cấp của $\mathfrak{g}$ mở rộng được thành một tự đẳng cấu sơ cấp của $\mathfrak{g}'$.

Đặt $\mathfrak{a}=\mathfrak{g}\mathfrak{l}(V)$. Theo Chương I, §5, no. 4, Bổ đề 2, các thành phần nửa đơn và lũy linh của ad$_{\mathfrak{a}}x$ lần lượt là ad$_{\mathfrak{a}}s$ và ad$_{\mathfrak{a}}n$; mệnh đề (i) suy ra từ điều này. Ta suy ra rằng các đa thức đặc trưng của ad$_{\mathfrak{g}}x$ và ad$_{\mathfrak{g}}s$ là như nhau; do đó có (ii). Nếu ad$_{\mathfrak{g}}x$ là lũy linh, ad$_{\mathfrak{g}}x=$ ad$_{\mathfrak{g}}n$, do đó ad$_{\mathfrak{g}'}n$ mở rộng ad$_{\mathfrak{g}}x$, và $n$ là một phần tử lũy linh của $\mathfrak{g}'$, do đó có (iii).

Cho $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$. Ta biết (Chương I, §6, no. 5, Định lý 4) rằng các điều kiện sau là tương đương:

(i) biểu diễn đồng nhất của $\mathfrak{g}$ là nửa đơn;

(ii) $\mathfrak{g}$ là khả quy và mọi phần tử của tâm của $\mathfrak{g}$ là một tự đồng cấu nửa đơn.

Các điều kiện này thực sự tương đương với các điều kiện sau:

(iii) $\mathfrak{g}$ là một đại số con khả quy trong $\mathfrak{g}\mathfrak{l}(V)$.

Thật vậy, (i) $=\Rightarrow$ (iii) theo Chương I, §6, no. 5, Hệ quả 3 của Định lý 4, và (iii) $=\Rightarrow$ (i) theo Chương I, §6, no. 6, Hệ quả 1 của Mệnh đề 7. Ta sẽ chứng minh rằng nếu $\mathfrak{g}$ thỏa mãn các điều kiện này thì $\mathfrak{g}$ là phân tích được. Tổng quát hơn:

#### Mệnh đề 2 {#lie-vii-s5-prop-2 .statement tag=00WK}

Cho $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$ khả quy trong $\mathfrak{g}\mathfrak{l}(V)$, E là một không gian vectơ hữu hạn chiều và $\pi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(E)$ là một biểu diễn tuyến tính nửa đơn của $\mathfrak{g}$ trên E. Khi đó:

(i) $\mathfrak{g}$ và $\pi (\mathfrak{g})$ đều phân tích được.

(ii) Các phần tử nửa đơn (resp. lũy linh) của $\pi (\mathfrak{g})$ là ảnh qua $\pi$ của các phần tử nửa đơn (resp. lũy linh) của $\mathfrak{g}$.

(iii) Nếu $\mathfrak{h}$ là một đại số con phân tích được của $\mathfrak{g}\mathfrak{l}(V)$ được chứa trong $\mathfrak{g}$, $\pi (\mathfrak{h})$ là một đại số con phân tích được của $\mathfrak{g}\mathfrak{l}(E)$.

(iv) Nếu $\mathfrak{h}'$ là một đại số con phân tích được của $\mathfrak{g}\mathfrak{l}(E)$, $\pi^{-1}(\mathfrak{h}')$ là một đại số con phân tích được của $\mathfrak{g}\mathfrak{l}(V)$.

Đặt $\mathfrak{s}= [\mathfrak{g},\mathfrak{g}]$ và gọi $\mathfrak{c}$ là tâm của $\mathfrak{g}$. Khi đó $\mathfrak{g}=\mathfrak{s}\times \mathfrak{c}$, và $\pi (\mathfrak{g}) =$ $\pi (\mathfrak{s})\times \pi (\mathfrak{c})$ theo Chương I, §6, no. 4, Hệ quả của Mệnh đề 5. Cho $y\in \mathfrak{s}, z\in \mathfrak{c}, y_s$ và $y_n$ là các thành phần nửa đơn và lũy linh của $y$. Khi đó $y_s, y_n\in \mathfrak{s}$ (Chương I, §6, no. 3, Mệnh đề $3$)$,y_s+z$ là nửa đơn (Đại số, Chương VII, §5, no. 7, Hệ quả của Mệnh đề 16), và $y_n$ giao hoán với $y_s+z$. Suy ra, các thành phần nửa đơn và lũy linh của $y+z$ là $y_s+z$ và $y_n$. Do đó, $\mathfrak{g}$ phân tích được. Vì $\pi (\mathfrak{g})$ khả quy trong $\mathfrak{g}\mathfrak{l}$(E), lập luận tương tự áp dụng cho $\pi (\mathfrak{g})$ và cho thấy rằng $\pi (\mathfrak{g})$ phân tích được. Hơn nữa, các phần tử lũy linh của $\mathfrak{g}$ (resp. $\pi (\mathfrak{g})$) là các phần tử lũy linh của $\mathfrak{s}$ (resp. $\pi (\mathfrak{s})$). Suy ra các phần tử lũy linh của $\pi (\mathfrak{g})$ là ảnh qua $\pi$ của các phần tử lũy linh của $\mathfrak{g}$ (Chương I, §6, no. 3, Mệnh đề 4). Các phần tử nửa đơn của $\mathfrak{g}$ (resp. $\pi (\mathfrak{g})$) là tổng của các phần tử nửa đơn của $\mathfrak{s}$ (resp. $\pi (\mathfrak{s})$) và các phần tử của $\mathfrak{c}$ (resp. $\pi (\mathfrak{c})$). Do đó các phần tử nửa đơn của $\pi (\mathfrak{g})$ là ảnh qua $\pi$ của các phần tử nửa đơn của $\mathfrak{g}$ (Chương I, loc. cit.). Suy ra (ii).

Các khẳng định (iii) và (iv) suy ra ngay lập tức từ (i) và (ii).

#### Nhận xét 1 {#lie-vii-s5-n1-rem-1 .statement tag=00WL}

Giả thiết về tính nửa đơn của $\pi$ tương đương với việc nói rằng $\pi (x)$ là nửa đơn với mọi $x\in \mathfrak{c}$. Lưu ý rằng giả thiết này được thỏa mãn khi $\pi$ được thu được từ biểu diễn đồng nhất $\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ bằng cách áp dụng liên tiếp các phép toán sau: tích tenxơ, chuyển sang đối ngẫu, sang một biểu diễn con, sang một thương, sang một tổng trực tiếp.

#### Nhận xét 2 {#lie-vii-s5-n1-rem-2 .statement tag=00WM}

Cho $\mathfrak{g}\subset \mathfrak{g}\mathfrak{l}$(V), $\mathfrak{g}'\subset \mathfrak{g}\mathfrak{l}(V')$ là các đại số Lie phân tích được, $\varphi$ là một đẳng cấu từ $\mathfrak{g}$ đến $\mathfrak{g}'$. Chú ý rằng $\varphi$ không nhất thiết biến các phần tử nửa đơn (tương ứng lũy linh) của $\mathfrak{g}$ thành các phần tử nửa đơn (tương ứng lũy linh) của $\mathfrak{g}'$ (Bài tập 2). Tuy nhiên, điều này đúng nếu $\mathfrak{g}$ là nửa đơn (Ch. I, §6, no. 3, Định lý 3).

#### Mệnh đề 3 {#lie-vii-s5-prop-3 .statement tag=00WN}

Cho $\mathfrak{a}$ là một đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V)$ và cho $\mathfrak{b}$ và $\mathfrak{c}$ là các không gian con vectơ của $\mathfrak{g}\mathfrak{l}(V)$ sao cho $\mathfrak{b}\subset \mathfrak{c}$. Gọi $\mathfrak{a}'$ là tập hợp các $x\in \mathfrak{a}$ sao cho $[x,\mathfrak{c}]\subset \mathfrak{b}$. Khi đó $\mathfrak{a}'$ là phân tích được.

Đặt $\mathfrak{g}=\mathfrak{g}\mathfrak{l}(V)$; đại số con $\mathfrak{h}'$ của $\mathfrak{g}\mathfrak{l}(\mathfrak{g})$ gồm các $z\in \mathfrak{g}\mathfrak{l}(\mathfrak{g})$ sao cho $z(\mathfrak{c})\subset \mathfrak{b}$ là phân tích được (Ví dụ 1). Gọi $\pi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(\mathfrak{g})$ là biểu diễn phụ hợp của $\mathfrak{g}$. Mệnh đề 2 (iv), áp dụng cho $\pi$, cho thấy rằng $\pi^{-1}(\mathfrak{h}')$ là phân tích được. Do đó $\mathfrak{a}'=\mathfrak{a}\cap \pi^{-1}(\mathfrak{h}')$ cũng vậy.

#### Hệ quả 1 {#lie-vii-s5-prop-3-cor-1 .statement tag=00WO}

Nếu $\mathfrak{a}$ là một đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V)$, và $\mathfrak{n}$ là một đại số con Lie của $\mathfrak{a}$, thì chuẩn hóa tử (tương ứng tâm hóa tử) của $\mathfrak{n}$ trong $\mathfrak{a}$ là phân tích được.

Điều này suy ra từ Mệnh đề 3 bằng cách lấy $\mathfrak{c}=\mathfrak{n},\mathfrak{b}=\mathfrak{n}$ (tương ứng $\mathfrak{c}=\mathfrak{n},\mathfrak{b}=\{0\}$).

#### Hệ quả 2 {#lie-vii-s5-prop-3-cor-2 .statement tag=00WP}

Các đại số con Cartan của một đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V)$ là phân tích được.

Điều này suy ra từ Hệ quả 1.

#### Nhận xét {#lie-vii-s5-n1-rem-3 .statement tag=00WQ}

Sau này chúng ta sẽ chứng minh (no. 5, Định lý 2) một đảo lại của Hệ quả 2.

### 2. BAO PHÂN TÍCH ĐƯỢC

Giao của một họ các đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V)$ rõ ràng là phân tích được. Do đó, nếu $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}$(V), tập hợp các đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V)$ chứa $\mathfrak{g}$ có một phần tử nhỏ nhất, được gọi là bao phân tích được của $\mathfrak{g}$; trong đoạn này, bao này sẽ được ký hiệu là $e(\mathfrak{g})$.

#### Mệnh đề 4 {#lie-vii-s5-prop-4 .statement tag=00WR}

Cho $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$ và $\mathfrak{n}$ là một iđêan của $\mathfrak{g}$. Khi đó $\mathfrak{n}$ và $e(\mathfrak{n})$ là các iđêan của $e(\mathfrak{g})$, và $[e(\mathfrak{g}), e(\mathfrak{n})] = [\mathfrak{g},\mathfrak{n}]$.

Cho $\mathfrak{g}_1$ là tập hợp các $x\in \mathfrak{g}\mathfrak{l}(V)$ sao cho $[x,\mathfrak{n}]\subset [\mathfrak{g},\mathfrak{n}]$. Đây là một đại số con Lie phân rã được của $\mathfrak{g}\mathfrak{l}$(V), chứa $\mathfrak{g}$ và do đó chứa $e(\mathfrak{g})$, cf. no. 1, Mệnh đề 3; nói cách khác, $[e(\mathfrak{g}),\mathfrak{n}]\subset [\mathfrak{g},\mathfrak{n}]$. Gọi $\mathfrak{n}_1$ là tập hợp các $y\in \mathfrak{g}\mathfrak{l}(V)$ sao cho

$$
[e(\mathfrak{g}), y]\subset [\mathfrak{g},\mathfrak{n}]
$$

Đây là một đại số con Lie phân rã được của $\mathfrak{g}\mathfrak{l}(V)$ chứa $\mathfrak{n}$ theo điều trên, và do đó chứa $e(\mathfrak{n})$; nói cách khác $[e(\mathfrak{g}), e(\mathfrak{n})]\subset [\mathfrak{g},\mathfrak{n}]$, vậy

$$
[e(\mathfrak{g}), e(\mathfrak{n})] = [\mathfrak{g},\mathfrak{n}]
$$

Suy ra rằng $[e(\mathfrak{g}),\mathfrak{n}]\subset [e(\mathfrak{g}), e(\mathfrak{n})]\subset \mathfrak{n}$, do đó $\mathfrak{n}$ và $e(\mathfrak{n})$ là các iđêan của $e(\mathfrak{g})$.

#### Hệ quả 1 {#lie-vii-s5-prop-4-cor-1 .statement tag=00WS}

(i) $\mathscr{D}^i\mathfrak{g}=\mathscr{D}^ie(\mathfrak{g})$ for $i\geq 1$, và $\mathscr{C}^i\mathfrak{g}=\mathscr{C}^ie(\mathfrak{g})$ for $i\geq 2$.

(ii) Nếu $\mathfrak{g}$ là giao hoán (tương ứng, lũy linh, tương ứng, giải được), thì $e(\mathfrak{g})$ là giao hoán (tương ứng, lũy linh, tương ứng, giải được).

Khẳng định (i) suy ra từ Mệnh đề 4 bằng quy nạp theo $i$ và (ii) suy ra từ (i).

#### Hệ quả 2 {#lie-vii-s5-prop-4-cor-2 .statement tag=00WT}

Gọi $\mathfrak{r}$ là căn của $\mathfrak{g}$. Nếu $\mathfrak{g}$ phân rã được, $\mathfrak{r}$ phân rã được.

Thật vậy, $e(\mathfrak{r})$ là một iđêan giải được của $\mathfrak{g}$ theo Mệnh đề 4 và Hệ quả 1, do đó $e(\mathfrak{r}) =\mathfrak{r}$.

### 3. PHÂN TÍCH CỦA CÁC ĐẠI SỐ PHÂN RÃ ĐƯỢC

Nếu $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$ với căn $\mathfrak{r}$, tập hợp các phần tử lũy linh của $\mathfrak{r}$ là một iđêan lũy linh của $\mathfrak{g}$, iđêan lũy linh lớn nhất của biểu diễn đồng nhất của $\mathfrak{g}$ (Chương I, §5, no. 3, Hệ quả 6 của Định lý 1). Trong đoạn này, ta sẽ ký hiệu iđêan này bởi $\mathfrak{n}_V(\mathfrak{g})$. Nó chứa căn lũy linh $[\mathfrak{g},\mathfrak{g}]\cap \mathfrak{r}$ của $\mathfrak{g}$ (Chương I, §5, no. 3, Định lý 1).

#### Mệnh đề 5 {#lie-vii-s5-prop-5 .statement tag=00WU}

Cho $\mathfrak{g}$ là một đại số con Lie lũy linh phân rã được của $\mathfrak{g}\mathfrak{l}(V)$. Gọi $\mathfrak{t}$ là tập hợp các phần tử nửa đơn của $\mathfrak{g}$. Khi đó $\mathfrak{t}$ là một đại số con trung tâm của $\mathfrak{g}$, và $\mathfrak{g}$ là tích của $\mathfrak{t}$ và $\mathfrak{n}_V(\mathfrak{g})$ như các đại số Lie.

Nếu $x\in \mathfrak{t}$, ad$_{\mathfrak{g}}x$ là nửa đơn và lũy linh, do đó bằng không, nên $x$ là trung tâm trong $\mathfrak{g}$. Do đó, $\mathfrak{t}$ là một iđêan của $\mathfrak{g}$, và $\mathfrak{t}\cap \mathfrak{n}_V(\mathfrak{g}) = 0$. Vì $\mathfrak{g}$ phân rã được, $\mathfrak{g}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$, do đó có mệnh đề.

#### Mệnh đề 6 {#lie-vii-s5-prop-6 .statement tag=00WV}

Cho $\mathfrak{g}$ là một đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V)$. Cho $\mathscr{T}$ là tập hợp các đại số con giao hoán của $\mathfrak{g}$ gồm các phần tử nửa đơn, và $\mathscr{T}_1$ là tập hợp các phần tử cực đại của $\mathscr{T}$. Cho $\mathscr{H}$ là tập hợp các đại số con Cartan của $\mathfrak{g}$.

(i) Với $\mathfrak{h}\in \mathscr{H}$, đặt $\varphi (\mathfrak{h})$ là tập hợp các phần tử nửa đơn của $\mathfrak{h}$. Khi đó $\varphi (\mathfrak{h})\in \mathscr{T}_1$.

(ii) Với $\mathfrak{t}\in \mathscr{T}_1$, đặt $\psi (\mathfrak{t})$ là hoán tập của $\mathfrak{t}$ trong $\mathfrak{g}$. Khi đó $\psi (\mathfrak{t})\in \mathscr{H}$.

(iii) Các ánh xạ $\varphi$ và $\psi$ là các song ánh nghịch đảo từ $\mathscr{H}$ đến $\mathscr{T}_1$ và từ $\mathscr{T}_1$ đến $\mathscr{H}$.

(iv) Nếu $k$ đóng đại số, Aut$_e(\mathfrak{g})$ tác động bắc cầu trên $\mathscr{T}_1$.

Cho $\mathfrak{h}\in \mathscr{H}$, và đặt $\mathfrak{t}=\varphi (\mathfrak{h})$. Theo Mệnh đề 5 và Hệ quả 2 của Mệnh đề $3,\mathfrak{t}\in \mathscr{T}$ và $\mathfrak{h}=\mathfrak{t}\times \mathfrak{n}_V(\mathfrak{h})$. Với mọi đại số con $\mathfrak{u}$ của $\mathfrak{g}$, ta ký hiệu $\psi (\mathfrak{u})$ là hoán tập của $\mathfrak{u}$ trong $\mathfrak{g}$. Khi đó $\mathfrak{h}\subset \psi (\mathfrak{t})$, và $\psi (\mathfrak{t})\subset \mathfrak{g}^0(\mathfrak{h})$ vì các phần tử của $\mathfrak{n}_V(\mathfrak{h})$ là lũy linh, nên $\mathfrak{h}=\psi (\mathfrak{t})$. Nếu $\mathfrak{t}'\in \mathscr{T}$ và $\mathfrak{t}\subset \mathfrak{t}'$, ta có $\mathfrak{t}'\subset \psi (\mathfrak{t}) =\mathfrak{h}$ nên $\mathfrak{t}'=\mathfrak{t}$, và do đó $\mathfrak{t}\in \mathscr{T}_1$.

Cho $\mathfrak{t}\in \mathscr{T}_1$, và đặt $\mathfrak{c}=\psi (\mathfrak{t})$. Cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{c}$. Theo §2, no. 3, Mệnh đề $10,\mathfrak{h}\in \mathscr{H}$ và $\mathfrak{t}\subset \mathfrak{h}$. Đặt $\mathfrak{t}_1=\varphi (\mathfrak{h})\in \mathscr{T}$. Khi đó $\mathfrak{t}\subset \mathfrak{t}_1$ nên $\mathfrak{t}=\mathfrak{t}_1$, và $\mathfrak{h}=\psi (\mathfrak{t}_1) =\psi (\mathfrak{t}) =\mathfrak{c}$ theo điều trên. Do đó, $\psi (\mathfrak{t})\in \mathscr{H}$, và $\varphi (\psi (\mathfrak{t})) =\mathfrak{t}$.

Ta đã chứng minh được (i), (ii) và (iii). Giả sử rằng $k$ đóng đại số. Vì Aut$_e(\mathfrak{g})$ tác động bắc cầu trên $\mathscr{H}($§3, no. 2, Định lý 1), Aut$_e(\mathfrak{g})$ tác động bắc cầu trên $\mathscr{T}_1$.

#### Hệ quả 1 {#lie-vii-s5-prop-6-cor-1 .statement tag=00WW}

Các đại số con Cartan của $\mathfrak{g}$ là các tâm hóa tử của các phần tử nửa đơn chính quy của $\mathfrak{g}$.

Nếu $x\in \mathfrak{g}$ là chính quy, $\mathfrak{g}^0(x)$ là một đại số con Cartan của $\mathfrak{g}($§2, no. 3, Định lý 1 (i)); hơn nữa, nếu $x$ là nửa đơn thì $\mathfrak{g}^0(x)$ là tâm hóa tử của $x$ trong $\mathfrak{g}$. Ngược lại, cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{g}$. Tồn tại $\mathfrak{t}\in \mathscr{T}_1$ sao cho $\mathfrak{h}=\psi (\mathfrak{t})$. Theo §1, no. 2, Mệnh đề 7, tồn tại $x\in \mathfrak{t}$ sao cho $\mathfrak{h}=\mathfrak{g}^0(x)$; vì $x\in \mathfrak{t}$, $\mathfrak{g}^0(x) =\mathfrak{g}_0(x)$. Theo §3, no. 3, Định lý 2 (ii), $x$ là chính quy.

#### Hệ quả 2 {#lie-vii-s5-prop-6-cor-2 .statement tag=00WX}

Giả sử thêm rằng $\mathfrak{g}$ là giải được. Khi đó:

(i) Nhóm con của Aut($\mathfrak{g}$) gồm các $e^{adx}, x\in \mathscr{C}^{\infty}\mathfrak{g}$ (xem §3, no. 4), tác động bắc cầu trên $\mathscr{T}_1$.

(ii) Nếu $\mathfrak{t}\in \mathscr{T}_1,\mathfrak{g}$ là tích nửa trực tiếp của $\mathfrak{t}$ và $\mathfrak{n}_V(\mathfrak{g})$.

Mệnh đề (i) suy ra từ sự kiện rằng nhóm của các $e^{adx},x\in \mathscr{C}^{\infty}\mathfrak{g}$, tác động bắc cầu trên $\mathscr{H}($§3, no. 4, Định lý 3).

Ta chứng minh (ii). Cho $\mathfrak{t}\in \mathscr{T}_1$, và đặt $\mathfrak{h}=\psi (\mathfrak{t})$ là đại số con Cartan tương ứng của $\mathfrak{g}$. Theo Mệnh đề $5,\mathfrak{h}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{h})\subset \mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$. Mặt khác, $\mathfrak{g}=\mathfrak{h}+ [\mathfrak{g},\mathfrak{g}] ($§2, no. 1, Hệ quả 3 của Mệnh đề 4) và $[\mathfrak{g},\mathfrak{g}]\subset \mathfrak{n}_V(\mathfrak{g})$, do đó $\mathfrak{g}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$. Nhưng rõ ràng rằng $\mathfrak{t}\cap \mathfrak{n}_V(\mathfrak{g}) =\{0\}$. Đại số $\mathfrak{g}$ do đó là tích nửa trực tiếp của $\mathfrak{t}$ và iđêan $\mathfrak{n}_V(\mathfrak{g})$.

#### Mệnh đề 7 {#lie-vii-s5-prop-7 .statement tag=00WY}

Cho $\mathfrak{g}$ là một đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V)$.

(i) Tồn tại một đại số con Lie $\mathfrak{m}$ của $\mathfrak{g}$, khả quy trong $\mathfrak{g}\mathfrak{l}(V)$, sao cho $\mathfrak{g}$ là tích nửa trực tiếp của $\mathfrak{m}$ và $\mathfrak{n}_V(\mathfrak{g})$.

(ii) Hai đại số con Lie bất kỳ của $\mathfrak{g}$ có các tính chất trong (i) là liên hợp dưới tác động của Aut$_e(\mathfrak{g})$.

The radical $\mathfrak{r}$ of $\mathfrak{g}$ là phân tích được (no. 2, Hệ quả 2 của Mệnh đề 4). Theo Hệ quả 2 của Mệnh đề 6, tồn tại một đại số con giao hoán $\mathfrak{t}$ của $\mathfrak{r}$, gồm các phần tử nửa đơn, sao cho $\mathfrak{r}=\mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{r})$. Vì ad$_{\mathfrak{g}}\mathfrak{t}$ gồm các phần tử nửa đơn, $\mathfrak{g}$ là tổng trực tiếp của $[\mathfrak{t},\mathfrak{g}]$ và tâm hóa $\mathfrak{z}$ của $\mathfrak{t}$ (Chương I, §3, no. 5, Mệnh đề 6). Vì $[\mathfrak{t},\mathfrak{g}]\subset \mathfrak{r},\mathfrak{g}=\mathfrak{z}+\mathfrak{r}$. Do đó, nếu $\mathfrak{s}$ là một đại số con Levi của $\mathfrak{z}$ (Chương I, §6, số $8$)$,\mathfrak{g}=\mathfrak{s}+\mathfrak{r}$, nên $\mathfrak{s}$ là một đại số con Levi của $\mathfrak{g}$. Đặt $\mathfrak{m}=\mathfrak{s}\oplus \mathfrak{t}$. Vì $[\mathfrak{s},\mathfrak{t}] =\{0\},\mathfrak{m}$ là một đại số Lie con của $\mathfrak{g}$, khả quy trong $\mathfrak{g}\mathfrak{l}(V)$ theo Chương I, §6, no. 5, Định lý 4. Hơn nữa,

$$
\mathfrak{g}=\mathfrak{s}\oplus \mathfrak{r}=\mathfrak{s}\oplus \mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{r}) =\mathfrak{s}\oplus \mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{g}) =\mathfrak{m}\oplus \mathfrak{n}_V(\mathfrak{g})
$$

vì $\mathfrak{n}_V(\mathfrak{g}) =\mathfrak{n}_V(\mathfrak{r})$. Do đó (i).

Bây giờ cho $\mathfrak{m}'$ là một đại số Lie con của $\mathfrak{g}$ bổ sung với $\mathfrak{n}_V(\mathfrak{g})$ và khả quy trong $\mathfrak{g}\mathfrak{l}(V)$. Ta chứng minh rằng $\mathfrak{m}'$ liên hợp với $\mathfrak{m}$ dưới Aut$_e(\mathfrak{g})$. Ta có $\mathfrak{m}'=\mathfrak{s}'\oplus \mathfrak{t}'$, trong đó $\mathfrak{s}'= [\mathfrak{m}',\mathfrak{m}']$ là nửa đơn và tâm $\mathfrak{t}'$ của $\mathfrak{m}'$ gồm các phần tử nửa đơn. Khi đó $\mathfrak{r}=\mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{g}) =\mathfrak{t}'\oplus \mathfrak{n}_V(\mathfrak{g})$. Theo Hệ quả 2 của Mệnh đề 6, ta quy về trường hợp $\mathfrak{t}=\mathfrak{t}'$. Khi đó $\mathfrak{s}'\subset \mathfrak{z}$; vì dim$\mathfrak{s}'=$ dim$\mathfrak{s}$, $\mathfrak{s}'$ là một đại số con Levi của $\mathfrak{z}$. Theo Chương I, §6, no. 8, Định lý 5, tồn tại $x\in \mathfrak{n}_V(\mathfrak{z})$ sao cho $e^{adx}(\mathfrak{s}) =\mathfrak{s}'$; vì $x$ giao hoán với $\mathfrak{t}$, ta cũng có $e^{adx}(\mathfrak{t}) =\mathfrak{t}$.

### 4. CÁC ĐẠI SỐ LIE TUYẾN TÍNH CỦA CÁC TỰ ĐỒNG CẤU LŨY LINH

#### Bổ đề 1 {#lie-vii-s5-lem-1 .statement tag=00WZ}

Cho $\mathfrak{n}$ là một đại số Lie con của $\mathfrak{g}\mathfrak{l}(V)$ gồm các tự đồng cấu lũy linh, và N là nhóm con exp$\mathfrak{n}$ của $\mathbf{G}\mathbf{L}(V)$ ($§3, no. 1, Bổ đề 1).

(i) Cho $\rho$ là một biểu diễn tuyến tính hữu hạn chiều của $\mathfrak{n}$ trên W, sao cho các phần tử của $\rho (\mathfrak{n})$ là lũy linh, $W'$ là một không gian con vectơ của W ổn định dưới $\rho ,\rho_1$ và $\rho_2$ là biểu diễn con và biểu diễn thương của $\rho$ được xác định bởi $W',\pi , \pi_1, \pi_2$ là các biểu diễn của N tương thích với $\rho , \rho_1, \rho_2($§3, no. 1). Khi đó $\pi_1, \pi_2$ là biểu diễn con và biểu diễn thương của $\pi$ được xác định bởi $W'$.

(ii) Cho $\rho_1, \rho_2$ là các biểu diễn tuyến tính hữu hạn chiều của $\mathfrak{n}$ sao cho các phần tử của $\rho_1(\mathfrak{n})$ và $\rho_2(\mathfrak{n})$ là lũy linh, và $\pi_1, \pi_2$ là các biểu diễn của N tương thích với $\rho_1, \rho_2$. Khi đó $\pi_1\otimes \pi_2$ là biểu diễn của N tương thích với $\rho_1\otimes \rho_2$.

(iii) Cho $\rho_1, \rho_2$ là các biểu diễn tuyến tính hữu hạn chiều của $\mathfrak{n}$ trên các không gian vectơ $V_1,V_2$, sao cho các phần tử của $\rho_1(\mathfrak{n})$ và $\rho_2(\mathfrak{n})$ là lũy linh, $\rho$ là biểu diễn của $\mathfrak{n}$ trên Hom(V$_1,V_2$) được xác định bởi $\rho_1, \rho_2$. Cho $\pi_1, \pi_2$ là các biểu diễn của N tương thích với $\rho_1, \rho_2$, và $\pi$ là biểu diễn của N trên Hom(V$_1,V_2$) được xác định bởi $\pi_1, \pi_2$. Khi đó $\pi$ là biểu diễn của N tương thích với $\rho$.

Mệnh đề (i) hiển nhiên. Cho $\rho_1, \rho_2, \pi_1, \pi_2$ như trong (ii). Nếu $x\in \mathfrak{n}$, ta có, vì $\rho_1(x)\otimes 1$ và $1\otimes \rho_2(x)$ giao hoán,

exp($\rho_1(x)\otimes 1 + 1\otimes \rho_2(x)$) $=$ exp($\rho_1(x)\otimes 1$). exp(1 $\otimes \rho_2(x)$)

= (exp $\rho_1(x)$)$\otimes 1.1\otimes$ (exp$\rho_2(x)$)

= (exp $\rho_1(x)$)$\otimes$ (exp$\rho_2(x)$)

$=\pi_1$(exp $x$)$\otimes \pi_2$(exp $x$)

$= (\pi_1\otimes \pi_2$)(exp $x$),

do đó (ii). Nếu $v_1\in$ EndV$_1$ và $v_2\in$ EndV$_2$, ký hiệu bởi $R_{v_1}$ và $L_{v_2}$ các ánh xạ $u \rightarrow uv_1$ và $u \rightarrow v_2u$ từ Hom(V$_1$,V$_2$) vào chính nó; các ánh xạ này giao hoán và $\rho (x)u= (L_{\rho_2(x)}-R_{\rho_1(x)})u$, nên

exp$\rho (x).u=$ exp $L_{\rho_2(x)}$. exp $R_{-\rho_1(x)}.u$

$$
= L_{exp\rho_2(x)}.R_{exp(-\rho_1(x))}.u
$$

$$
= L_{\pi_2(expx)}.R_{\pi_1(exp(-x))}.u
$$

$=\pi$(exp $x$)$.u$,

do đó (iii).

#### Bổ đề 2 {#lie-vii-s5-lem-2 .statement tag=01JS}

$^2$ (i) Cho W là một không gian con của V có chiều $d$, D là đường thẳng $\bigwedge^dW\subset \bigwedge^dV,\theta$ là biểu diễn chính tắc của $\mathfrak{g}\mathfrak{l}(V)$ trên $\bigwedge V$ (Ch. III, Phụ lục). Cho $x\in \mathfrak{g}\mathfrak{l}(V)$. Khi đó $x(W)\subset W$ khi và chỉ khi $\theta (x)(D)\subset D$.

(ii) Cho $(e_1, . . . , e_n)$ là cơ sở chính tắc của $k^n,\theta$ là biểu diễn chính tắc của $\mathfrak{g}\mathfrak{l}(n, k)$ trên $\bigwedge(k^n)$, và $x\in \mathfrak{g}\mathfrak{l}(n, k)$. Khi đó $x\in \mathfrak{n}(n, k)$ khi và chỉ khi

$$
\theta (x)(e_{n-d+1}\wedge  \cdots  \wedge e_n) = 0
$$

với $1\leq d\leq n$.

(i) Nếu $x(W)\subset W$, thì rõ ràng $\theta (x)D\subset D$. Ngược lại, giả sử $\theta (x)D\subset D$. Cho $u$ là một phần tử khác không của D và cho $y\in W$. Khi đó $y\wedge u= 0$. Vì $\theta (x)$ là một đạo hàm của $\bigwedge V$, điều này suy ra

$$
\theta (x)y\wedge u+y\wedge \theta (x)u= 0
$$

Bây giờ $\theta (x)u\in ku$, nên $y\wedge \theta (x)u= 0$ và do đó $\theta (x)y\wedge u= 0$. Theo Đại số, Ch. III, §7, no. 9, Mệnh đề 13, điều này suy ra $\theta (x)y\in W$, tức là $x(y)\in W$, điều đó chứng tỏ rằng $x(W)\subset W$.

(ii) Điều kiện nêu trong (ii) hiển nhiên là cần thiết để $x\in \mathfrak{n}(n, k)$. Giả sử điều đó được thỏa mãn. Theo (i), $x$ giữ ổn định

$^2$ Trong bổ đề này, $k$ có thể là một trường giao hoán tùy ý.

$$
ke_{n-d+1}+\cdots +ke_n
$$

và vì điều này đúng với $d= 1, . . . , n,x$ là tam giác dưới. Đặt

$$
x= (x_{ij})_{1\leq i,j\leq n}
$$

Ta có $0 =x(e_n) =x_{nn}e_n$, do đó $x_{nn}= 0$. Cho $i < n$, và giả sử rằng ta đã chứng minh $x_{jj}= 0$ với $j > i$. Khi đó

$$
0 =\theta (x)(e_i\wedge e_{i+1}\wedge  \cdots  \wedge e_n) =x_{ii}(e_i\wedge e_{i+1}\wedge  \cdots  \wedge e_n)
$$

nên $x_{ii}= 0$. Vậy $x\in \mathfrak{n}(n, k)$.

#### Mệnh đề 8 {#lie-vii-s5-prop-8 .statement tag=00X0}

Cho $\mathfrak{n}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$ gồm các phần tử lũy linh, $\mathfrak{q}$ là bộ chuẩn hóa của $\mathfrak{n}$ trong $\mathfrak{g}\mathfrak{l}(V)$. Tồn tại một không gian vectơ hữu hạn chiều E, một biểu diễn $\rho$ của $\mathfrak{g}\mathfrak{l}(V)$ trên E, và một không gian con vectơ F của E, thỏa mãn các điều kiện sau:

(i) ảnh qua $\rho$ của một phép vị tự của V là chéo hóa được;

(ii) F ổn định dưới $\rho (\mathfrak{q})$;

(iii) $\mathfrak{n}$ là tập hợp các $x\in \mathfrak{g}\mathfrak{l}(V)$ sao cho $\rho (x)(F) = 0$.

Đặt $n=$ dim V. Theo định lý Engel, V có thể được đồng nhất với $k^n$ sao cho $\mathfrak{n}\subset \mathfrak{n}(n, k)$. Ký hiệu P là đại số các hàm đa thức trên $\mathfrak{g}\mathfrak{l}(n, k)$. Với $i= 0,1, . .$., ký hiệu $P_i$ là tập hợp các phần tử của P thuần nhất bậc $i$. Đặt N = exp $\mathfrak{n}$, là một nhóm con của nhóm tam giác dưới nghiêm ngặt T. Gọi J là tập hợp các phần tử của P bằng không trên N; đó là một iđêan trong P. Ký hiệu $N_J$ là tập hợp các $x\in \mathfrak{g}\mathfrak{l}(n, k)$ sao cho $p(x) = 0$ với mọi $p\in J$. Khi đó $N\subset N_J$. Ngược lại, lấy $x\in N_J$. Ký hiệu bởi $p_{ij}$ các hàm đa thức cho các phần tử của một phần tử của $\mathfrak{g}\mathfrak{l}(n, k)$. Iđêan J chứa các $p_{ij}$ (với $i < j$) và các $p_{ii}-1$; do đó $x\in T$. Mặt khác, nếu $u$ là một dạng tuyến tính trên $\mathfrak{g}\mathfrak{l}(n, k)$ bằng không trên $\mathfrak{n}$, thì tồn tại $p_u\in P$ sao cho $p_u(z) =u$(log $z$) với mọi $z\in T ($§3, no. 1, Bổ đề 1 (i)); ta có $p_u\in J$, nên $u$(log $x$) $= 0$. Suy ra log $x$ thuộc $\mathfrak{n}$, nên $x\in N$, chứng minh rằng $N = N_J$.

Với mọi $p\in P$ và $g\in \mathbf{G}\mathbf{L}_n(k)$, gọi $\lambda (g)p$ là hàm $x \rightarrow p(g^{-1}x)$ trên $\mathfrak{g}\mathfrak{l}(n, k)$; khi đó $\lambda (g)p\in P,\lambda (g)$ là một tự đẳng cấu của đại số P, và $\lambda$ là một biểu diễn của $\mathbf{G}\mathbf{L}_n(k)$ trên P, làm cho mỗi $P_i$ ổn định. Ta chứng minh rằng

$$
N =\{x\in \mathbf{G}\mathbf{L}_n(k)|\lambda (x)J = J\} \tag{1}
$$

Nếu $x\in N, p\in J, y\in N$, thì $(\lambda (x)p)(y) =p(x^{-1}y) = 0$ vì $x^{-1}y\in N$; do đó $\lambda (x)p\in J$, suy ra $\lambda (x)J = J$. Giả sử $x\in \mathbf{G}\mathbf{L}_n(k)$ sao cho $\lambda (x)J = J$; lấy $p\in J$; khi đó $p(x^{-1}) = (\lambda (x)p)(e) = 0$, nên $x^{-1}\in N_J= N$ và $x\in N$. Điều này chứng minh (i).

Iđêan J là hữu hạn sinh (Commutative Algebra, Chap. III, §2, no. 10, Cor. 2 of Th. 2). Do đó, tồn tại một số nguyên $q$ sao cho, nếu $W = P_0+ P_1+\cdots + P_q$, thì $J\cap W$ sinh ra J như một iđêan. Ký hiệu bởi $\lambda_j$ (resp. $\lambda '$) biểu diễn con của $\lambda$ được xác định bởi $P_J$ (resp. bởi W). Theo (1),

$$
N =\{x\in \mathbf{G}\mathbf{L}_n(k)|\lambda '(x)(J\cap W) = J\cap W\} \tag{2}
$$

Ta chứng minh rằng, với mọi $j$, tồn tại một biểu diễn $\sigma_j$ của đại số Lie $\mathfrak{g}\mathfrak{l}(n, k)$ trên $P_j$ sao cho:

$\sigma_j|\mathfrak{n}(n, k)$ là tương thích (§$3$, no$.1$) với $\lambda_j|T$. (3)

Với mọi $x\in k.1_n$, $\sigma_j(x)$ là một phép vị tự. (4)

Vì $\lambda_j$ là lũy thừa đối xứng thứ $j$ của $\lambda_1$, đủ chứng minh sự tồn tại của $\sigma_1$, xem Bổ đề 1. Bây giờ $\lambda_1$ là biểu diễn đối ngẫu của biểu diễn $\gamma$ của $\mathbf{G}\mathbf{L}_n(k)$ trên $\mathfrak{g}\mathfrak{l}(n, k)$ cho bởi

$$
\gamma (x)y=xy, x\in \mathbf{G}\mathbf{L}_n(k), y\in \mathfrak{g}\mathfrak{l}(n, k)
$$

Cho $c$ là biểu diễn của đại số Lie $\mathfrak{g}\mathfrak{l}(n, k)$ trên $\mathfrak{g}\mathfrak{l}(n, k)$ cho bởi

$$
c(x)y=xy, x, y\in \mathfrak{g}\mathfrak{l}(n, k)
$$

Rõ ràng là $c|\mathfrak{n}(n, k)$ và $\gamma |T$ là tương thích, và rằng $c(x)$ là một phép vị tự với mọi $x\in k.1_n$. Vì thế, đủ lấy $\sigma_1$ là biểu diễn đối ngẫu của $c$ (Chap. I, §3, no. 3).

Bây giờ xét $\sigma '$ là biểu diễn của đại số Lie $\mathfrak{g}\mathfrak{l}(n, k)$ trên W được cho bởi tổng trực tiếp của các $\sigma_j, 0\leq j\leq q$. Xét theo (2) và các quan hệ

$\lambda '$(exp($x$)) $=$ exp($\sigma '(x)$) và $\sigma '$(log($y$)) $=$ log($\lambda '(y)$)$, x\in \mathfrak{n}(n, k), y\in T$,

ta có

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\sigma '(x)(J\cap W)\subset J\cap W\} \tag{5}
$$

Cho $d=$ dim(J $\cap W$), và cho $\tau =\bigwedge^d\sigma '$. Cho $D =\bigwedge^d(J\cap W)$. Theo (5) và Bổ đề 2 (i),

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\tau (x)(D)\subset D\} \tag{6}
$$

Nhưng $\tau (\mathfrak{n}(n, k))$ chỉ gồm các tự đồng cấu lũy linh, nên (6) cũng có thể viết là

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\tau (x)(D) = 0\} \tag{7}
$$

Bây giờ cho $E =\bigwedge^dW\oplus \bigwedge^1V\oplus \bigwedge^2V\oplus  \cdots  \oplus \bigwedge^nV$; cho $\rho$ là tổng trực tiếp của $\tau$ và các biểu diễn chính tắc của $\mathfrak{g}\mathfrak{l}(n, k)$ trên $\bigwedge^1V, . . . ,\bigwedge^nV$. Cho $E_0\subset E$ là tổng của $D =\bigwedge^d(J\cap W)$ và các đường thẳng sinh bởi $e_{n-j+1}\wedge  \cdots  \wedge e_n$ với $j= 1, . . . , n$. Theo (7) và Bổ đề 2 (ii),

$$
\mathfrak{n}=\{x\in \mathfrak{g}\mathfrak{l}(V)|\rho (x)(E_0) = 0\} \tag{8}
$$

Ngay lập tức, nếu $x\in k.1_n,\rho (x)$ là chéo hóa được. Cuối cùng, nếu F là tập hợp các phần tử của E bị triệt tiêu bởi $\rho (\mathfrak{n})$, thì F ổn định dưới $\rho (\mathfrak{q})$ (Chap. I, §3, no. 5, Prop. 5), và theo (8),

$$
\mathfrak{n}=\{x\in \mathfrak{g}\mathfrak{l}(V)|\rho (x)(F) = 0\} \tag{9}
$$

### 5. CÁC ĐẶC TRƯNG CỦA CÁC ĐẠI SỐ LIE PHÂN RÃ ĐƯỢC

Mọi đại số Lie phân rã được đều được sinh như một không gian vectơ (và a fortiori như một đại số Lie) bởi tập hợp các phần tử của nó hoặc là nửa đơn hoặc là lũy linh. Chiều ngược lại:

#### Định lý 1 {#lie-vii-s5-thm-1 .statement tag=00X1}

Cho $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$ và cho X là một tập con của $\mathfrak{g}$ sinh ra $\mathfrak{g}$ như một đại số Lie trên $k$. Nếu mọi phần tử của X đều hoặc là nửa đơn hoặc là lũy linh, thì $\mathfrak{g}$ phân rã được.

a) $\mathfrak{g}$ giao hoán.

Các phần tử nửa đơn (resp. lũy linh) của $\mathfrak{g}$ tạo thành một không gian con $\mathfrak{g}_s$ (resp. $\mathfrak{g}_n$). Giả thiết này tương đương với $\mathfrak{g}=\mathfrak{g}_s\oplus \mathfrak{g}_n$, do đó $\mathfrak{g}$ phân rã được.

b) $\mathfrak{g}$ khả quy.

Then $\mathfrak{g}=\mathfrak{g}'\times \mathfrak{c}$ với $\mathfrak{g}'$ nửa đơn và $\mathfrak{c}$ giao hoán. Theo Mệnh đề $2,\mathfrak{g}'$ là phân tích được. Cho $x=a+b\in \mathfrak{g}$ với $a\in \mathfrak{g}',b\in \mathfrak{c}$. Gọi $a_s, a_n, b_s, b_n$ là các thành phần nửa đơn và lũy linh của $a, b$. Vì $a_s, a_n, b_s, b_n$ giao hoán đôi một, nên các thành phần nửa đơn và lũy linh của $x$ là $a_s+b_s, a_n+b_n$. Nay $a_s, a_n\in \mathfrak{g}'$. Nếu $x$ là nửa đơn, thì $x=a_s+b_s$; vì $a_s\in \mathfrak{g}'$, ta có $b_s\in \mathfrak{g}$, nên $b_s\in \mathfrak{c}$ vì $b_s$ giao hoán với $\mathfrak{g}$; do đó, $a=a_s$ và $b=b_s$. Tương tự, nếu $x$ là lũy linh, thì $a=a_n$ và $b=b_n$. Suy ra rằng các ảnh chiếu lên $\mathfrak{c}$ của các phần tử của X hoặc là nửa đơn hoặc là lũy linh; theo $a)$, điều này kéo theo rằng $\mathfrak{c}$ là phân tích được. Giữ nguyên ký hiệu trước đó, nhưng không còn giả thiết về $x$, ta có $b_s, b_n\in \mathfrak{c}$, nên $a_s+b_s, a_n+b_n\in \mathfrak{g}$, điều này chứng minh định lý trong trường hợp này.

c) Trường hợp chung.

Ta giả sử định lý đã được chứng minh cho các đại số Lie có chiều $<$ dim $\mathfrak{g}$ và chứng minh nó cho $\mathfrak{g}$.

Cho $\mathfrak{n}$ là iđêan lũy linh lớn nhất của biểu diễn đồng nhất của $\mathfrak{g}$. Nếu $\mathfrak{n}= 0,\mathfrak{g}$ có một biểu diễn nửa đơn đơn ánh, nên là khả quy. Giả sử $\mathfrak{n}\not= 0$. Cho $\mathfrak{p}$ là bộ chuẩn hoá của $\mathfrak{n}$ trong $\mathfrak{g}\mathfrak{l}(V)$. Tồn tại $E, \rho ,F$ thỏa mãn các điều kiện của Mệnh đề 8. Vì $\mathfrak{g}\subset \mathfrak{p},\rho (\mathfrak{g})$ giữ F ổn định; cho $\rho_0$ là biểu diễn $u \rightarrow \rho (u)|F$ của $\mathfrak{g}$ trên F; ta có $\mathfrak{n}=$ Ker$\rho_0$. Ảnh qua $\rho$ của mọi phần tử nửa đơn (tương ứng lũy linh) của $\mathfrak{g}\mathfrak{l}(V)$ là nửa đơn (tương ứng lũy linh) (Mệnh đề 2). Do đó đại số $\rho_0(\mathfrak{g})$ được sinh bởi các phần tử nửa đơn và các phần tử lũy linh của nó. Theo giả thiết quy nạp, $\rho_0(\mathfrak{g})$ là phân tích được.

Cho $x\in \mathfrak{g}$, và gọi $x_s, x_n$ là các thành phần nửa đơn và lũy linh của nó. Theo Mệnh đề 2, các thành phần nửa đơn và lũy linh của $\rho (x)$ là $\rho (x_s), \rho (x_n)$. Vì $\rho_0(\mathfrak{g})$ là phân tích được, tồn tại $y, z\in \mathfrak{g}$ sao cho

$$
\rho_0(y) =\rho (x_s)|F, \rho_0(z) =\rho (x_n)|F
$$

Khi đó $x_s\in y+\mathfrak{n}, x_n\in z+\mathfrak{n}$, do đó $x_s, x_n\in \mathfrak{g}$. ĐPCM.

#### Hệ quả 1 {#lie-vii-s5-thm-1-cor-1 .statement tag=00X2}

Mọi đại số con của $\mathfrak{g}\mathfrak{l}(V)$ được sinh bởi các đại số con phân tích được của nó đều phân tích được.

Điều này hiển nhiên.

#### Hệ quả 2 {#lie-vii-s5-thm-1-cor-2 .statement tag=00X3}

Cho $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$. Khi đó $[\mathfrak{g},\mathfrak{g}]$ là phân tích được.

Cho $\mathfrak{r}$ là căn của $\mathfrak{g},\mathfrak{s}$ là một đại số con Levi của $\mathfrak{g}$ (Chương I, §6, no. 8). Khi đó

$$
[\mathfrak{g},\mathfrak{g}] = [\mathfrak{s},\mathfrak{s}] + [\mathfrak{s},\mathfrak{r}] + [\mathfrak{r},\mathfrak{r}] =\mathfrak{s}+ [\mathfrak{g},\mathfrak{r}]
$$

Đại số $[\mathfrak{g},\mathfrak{r}]$ là phân tích được vì mọi phần tử của nó đều lũy linh (Chương I, §5, no. 3). Mặt khác, $\mathfrak{s}$ là phân tích được (Mệnh đề 2). Suy ra $[\mathfrak{g},\mathfrak{g}]$ là phân tích được (Hệ quả 1).

#### Hệ quả 3 {#lie-vii-s5-thm-1-cor-3 .statement tag=00X4}

Cho $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$, và cho X là một tập con của $\mathfrak{g}$ sinh ra $\mathfrak{g}($như một đại số Lie trên $k)$.

(i) Bao phân tích được $e(\mathfrak{g})$ của $\mathfrak{g}$ được sinh bởi các thành phần nửa đơn và lũy linh của các phần tử của X.

(ii) Nếu $k'$ là một mở rộng đóng đại số của $k,e(\mathfrak{g}\otimes_kk') =e(\mathfrak{g})\otimes_kk'$; và $\mathfrak{g}$ phân tích được khi và chỉ khi $\mathfrak{g}\otimes_kk'$ phân tích được.

Cho $\widetilde{\mathfrak{g}}$ là đại số con của $\mathfrak{g}\mathfrak{l}(V)$ được sinh bởi các thành phần nửa đơn và lũy linh của các phần tử của X. Khi đó $\mathfrak{g}\subset \widetilde{\mathfrak{g}}\subset e(\mathfrak{g})$; theo Định lý $1, \widetilde{\mathfrak{g}}$ là phân tích được, nên $\widetilde{\mathfrak{g}}=e(\mathfrak{g})$, điều đó chứng minh (i). Mệnh đề (ii) suy ra, vì X sinh ra $k'$-đại số $\mathfrak{g}\otimes_kk'$.

#### Hệ quả 4 {#lie-vii-s5-thm-1-cor-4 .statement tag=00X5}

Cho $\mathfrak{g}$ là một đại số con Lie phân tích được của $\mathfrak{g}\mathfrak{l}(V)$. Cho $\mathscr{T}$ là tập hợp các đại số con giao hoán của $\mathfrak{g}$ gồm các phần tử nửa đơn (xem Mệnh đề 6). Các phần tử cực đại của $\mathscr{T}$ đều có cùng chiều.

Cho $k'$ là một mở rộng đóng đại số của $k$ và $V'= V\otimes_kk',\mathfrak{g}'=$ $\mathfrak{g}\otimes_kk'$. Cho $\mathfrak{t}_1,\mathfrak{t}_2$ là các phần tử cực đại của $\mathscr{T},\mathfrak{t}'_i=\mathfrak{t}_i\otimes_kk',\mathfrak{h}_i$ là hoán tập của $\mathfrak{t}_i$ trong $\mathfrak{g},\mathfrak{h}'_i=\mathfrak{h}_i\otimes_kk'$. Khi đó $\mathfrak{h}_i$ là một đại số con Cartan của $\mathfrak{g}$ (Mệnh đề 6) nên $\mathfrak{h}'_i$ là một đại số con Cartan của $\mathfrak{g}'$. Khi đó $\mathfrak{h}_i=\mathfrak{t}_i\times \mathfrak{n}_V(\mathfrak{h}_i)$, do đó $\mathfrak{h}'_i=\mathfrak{t}'_i\times \mathfrak{n}_{V'}(\mathfrak{h}'_i)$, sao cho $\mathfrak{t}'_i$ là tập hợp các phần tử nửa đơn của $\mathfrak{h}'_i$. Vì $\mathfrak{g}'$ là phân tích được (Hệ quả $3$)$,\mathfrak{t}'_1$ và $\mathfrak{t}'_2$ liên hợp dưới Aut$_e(\mathfrak{g}')$ (Mệnh đề 6), nên dim$\mathfrak{t}_1=$ dim$\mathfrak{t}_2$.

#### Định lý 2 {#lie-vii-s5-thm-2 .statement tag=00X6}

Cho $\mathfrak{g}$ là một đại số con Lie của $\mathfrak{g}\mathfrak{l}(V)$. Các điều kiện sau là tương đương:

(i) $\mathfrak{g}$ là phân tích được;

(ii) mọi đại số con Cartan của $\mathfrak{g}$ đều phân tích được;

(iii) $\mathfrak{g}$ có một đại số con Cartan phân tích được;

(iv) căn của $\mathfrak{g}$ phân tích được.

(i) $=\Rightarrow$ (ii): Điều này suy ra từ Hệ quả 2 của Mệnh đề 3.

(ii) $=\Rightarrow$ (i): Điều này suy ra từ Hệ quả 1 của Định lý 1, vì $\mathfrak{g}$ được sinh bởi các đại số con Cartan của nó (§2, no. 3, Hệ quả 3 của Định lý 1).

(ii) $=\Rightarrow$ (iii): Điều này rõ ràng.

(iii) $=\Rightarrow$ (ii): Theo Hệ quả 3 của Định lý 1, ta có thể giả sử rằng $k$ đóng đại số. Khi đó các đại số con Cartan của $\mathfrak{g}$ liên hợp dưới các tự đẳng cấu sơ cấp của $\mathfrak{g}($§3, no. 2, Định lý 1); do Nhận xét 1 của §3, no. 1, suy ra rằng, nếu một trong số chúng phân tích được thì tất cả đều phân tích được.

(i) $=\Rightarrow$ (iv): Điều này suy ra từ Hệ quả 2 của Mệnh đề 4.

(iv) $=\Rightarrow$ (i): Giả sử rằng căn $\mathfrak{r}$ của $\mathfrak{g}$ phân tích được. Cho $\mathfrak{s}$ là một đại số con Levi của $\mathfrak{g}$; nó phân tích được (Mệnh đề 2). Do đó $\mathfrak{g}=\mathfrak{s}+\mathfrak{r}$ phân tích được (Hệ quả 1 của Định lý 1).

### Bài tập {#lie-vii-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
