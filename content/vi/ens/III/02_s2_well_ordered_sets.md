---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 2
section_title: Well-ordered sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 148-157, 221-229
pdf_pages: 0154-0163, 0227-0235
extraction: ocr
subsections:
    - "no": 1
      title: SEGMENTS OF A WELL-ORDERED SET
      page: 148
      pdf_page: 154
    - "no": 2
      title: THE PRINCIPLE OF TRANSFINITE INDUCTION
      page: 151
      pdf_page: 157
    - "no": 3
      title: ZERMELO'S THEOREM
      page: 152
      pdf_page: 158
    - "no": 4
      title: INDUCTIVE SETS
      page: 154
      pdf_page: 160
    - "no": 5
      title: ISOMORPHISMS OF WELL-ORDERED SETS
      page: 155
      pdf_page: 161
    - "no": 6
      title: LEXICOGRAPHIC PRODUCTS
      page: 157
      pdf_page: 163
statements: 28
exercises: 20
content_sha256: a0534589a0212091e5b7ea8fc158f186a41c2eae85b60e8550c53f2b6308d9e5
translated_from: content/en/ens/III/02_s2_well_ordered_sets.md
source_content_sha256: 65da6eb8d8759db6e65d9e867b0617a631d488f7be094032cffc5bb93cf130d7
translation_model: gpt-5.4, gpt-5.4-mini
translation_run: translate-vi-99f70c1a
glossary_version: 27
glossary_terms_sha256: a95210e50e1988a95cc6dc822ce2dfec733d95512c9724be8d6d0fdf8021758a
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. TẬP ĐƯỢC SẮP THỨ TỰ TỐT

### 1. CÁC ĐOẠN CỦA MỘT TẬP ĐƯỢC SẮP THỨ TỰ TỐT

Một quan hệ $\mathrm{R}\{x, y\}$ được gọi là một *quan hệ sắp thứ tự tốt giữa $x$ và $y$* nếu R là một quan hệ thứ tự giữa $x$ và $y$ và nếu, với mỗi tập hợp không rỗng E mà trên đó $\mathrm{R}\{x, y\}$ cảm sinh một quan hệ thứ tự (nghĩa là, sao cho $x \in \mathrm{E}$ kéo theo $\mathrm{R}\{x, x\}$; xem § 1, no. 1), thì E, được sắp thứ tự bởi quan hệ này, có một *phần tử bé nhất*.

¶ Một tập hợp E được sắp thứ tự bởi một thứ tự $\Gamma$ được gọi là *được sắp tốt* nếu quan hệ $y \in \Gamma\langle x\rangle$ là một quan hệ sắp thứ tự tốt giữa $x$ và $y$; khi đó $\Gamma$ được gọi là một *sắp thứ tự tốt* trên E. Định nghĩa sau là tương đương với định nghĩa này:

#### Định nghĩa 1 {#ens-iii-s2-def-1 .statement tag=03JY}

*Một tập hợp* E *được gọi là được sắp tốt nếu nó có thứ tự và nếu mỗi tập con không rỗng của* E *có một phần tử bé nhất.*

Một tập được sắp thứ tự tốt E được sắp thứ tự toàn phần vì mọi tập con $\{x, y\}$ của E đều có một phần tử bé nhất. Mọi tập con A của E bị chặn trên trong E đều có một cận trên bé nhất trong E.

*Ví dụ*

#### Ví dụ 1 {#ens-iii-s2-n1-exa-1 .statement tag=03SX}

Cho $\mathrm{E} = \{\alpha, \beta\}$ là một tập hợp có các phần tử phân biệt. Dễ dàng kiểm tra rằng tập con $\{(\alpha, \alpha), (\beta, \beta), (\alpha, \beta)\}$ của $\mathrm{E} \times \mathrm{E}$ là đồ thị của một sắp thứ tự tốt trên E.

#### Ví dụ 2 {#ens-iii-s2-n1-exa-2 .statement tag=03SY}

Mọi tập con (đặc biệt là tập con rỗng) của một tập được sắp thứ tự tốt đều được sắp thứ tự tốt theo thứ tự cảm sinh.

#### Ví dụ 3 {#ens-iii-s2-n1-exa-3 .statement tag=03SZ}

Sự tồn tại của các tập được sắp thứ tự toàn phần nhưng không được sắp thứ tự tốt là tương đương với tiên đề vô hạn (§ 4, no. 4, Hệ quả 1 của Mệnh đề 3, và Bài tập 3).

#### Ví dụ 4 {#ens-iii-s2-n1-exa-4 .statement tag=03T0}

Nếu $\Gamma$ là một sắp thứ tự tốt trên E, thì thứ tự đối của $\Gamma$ là một sắp thứ tự tốt trên E chỉ khi E hữu hạn (§ 4, Bài tập 3). \*

#### Ví dụ 5 {#ens-iii-s2-n1-exa-5 .statement tag=03T1}

Cho E là một tập được sắp thứ tự tốt. Tập $\mathrm{E}_1$ thu được bằng cách thêm vào E một phần tử lớn nhất $b$ (§ 1, no. 7) là được sắp thứ tự tốt, vì nếu H là bất kỳ

tập con không rỗng nào của $\mathrm{E}_1$ khác $\{b\}$, thì phần tử nhỏ nhất của $\mathrm{H} \cap \mathrm{E}$ cũng là phần tử nhỏ nhất của H.

#### Chú ý {#ens-iii-s2-n1-rem-1 .statement tag=03JZ}

\* Là hệ quả của tiên đề vô hạn (§ 6, no. 1), tồn tại các tập được sắp thứ tự tốt không có phần tử lớn nhất, chẳng hạn tập $\mathbf{N}$ của các số nguyên tự nhiên. \*

#### Định nghĩa 2 {#ens-iii-s2-def-2 .statement tag=03QN}

*Trong một tập hợp có thứ tự* E, *một tập con của* E *sao cho các quan hệ* $x \in \mathrm{S}$, $y \in \mathrm{E}$, *và* $y \leqslant x$ *suy ra* $y \in \mathrm{S}$ *được gọi là một đoạn của* E.

Rõ ràng, mọi giao và hợp của các đoạn của E đều là một đoạn của E. Nếu S là một đoạn của E, thì mọi đoạn của S cũng là một đoạn của E. Bản thân tập E và tập rỗng đều là các đoạn của E.

#### Mệnh đề 1 {#ens-iii-s2-prop-1 .statement tag=03QO}

*Trong một tập được sắp thứ tự tốt* E, *mọi đoạn đầu của* E *khác* E *chính nó đều là một khoảng* $]\leftarrow, a[$, *trong đó* $a \in \mathrm{E}$.

Cho S là một đoạn đầu của E sao cho $\mathrm{S} \neq \mathrm{E}$. Vì $\mathrm{E} - \mathrm{S}$ không rỗng nên nó có một phần tử bé nhất $a$. Theo Định nghĩa 2, quan hệ $x \geqslant a$ kéo theo $x \notin \mathrm{S}$; nếu không thì ta sẽ có $a \in \mathrm{S}$, điều này vô lý. Do đó $\mathrm{E} - \mathrm{S}$ là khoảng $[a, \rightarrow[$, và S là khoảng $]\leftarrow, a[$.

¶ Với mọi phần tử $x$ trong một tập sắp thứ tự toàn phần E, đoạn đầu $]\leftarrow, x[$ được gọi là *đoạn đầu có đầu mút x*, và được ký hiệu bởi $\mathrm{S}_x$.

Chú ý rằng nếu E được sắp thứ tự tốt và không rỗng, $\mathrm{S}_x$ có phần tử nhỏ nhất $\alpha$ và do đó cũng là khoảng $[\alpha, x[$.

Cho E là một tập sắp thứ tự toàn phần. Hợp A của các $\mathrm{S}_x$, khi $x$ chạy qua E, là E nếu E không có phần tử lớn nhất; và nếu E có một phần tử lớn nhất $b$, thì ta có $\mathrm{A} = \mathrm{E} - \{b\}$.

#### Mệnh đề 2 {#ens-iii-s2-prop-2 .statement tag=03QP}

*Tập* E\* *các đoạn của một tập được sắp thứ tự tốt* E *được sắp thứ tự tốt theo bao hàm. Ánh xạ* $x \rightarrow \mathrm{S}_x$ *là một đẳng cấu của tập được sắp thứ tự tốt* E *lên tập các đoạn của* E *khác với* E *chính nó.*

Rõ ràng là nếu $x \in \mathrm{E}$ và $y \in \mathrm{E}$, thì $x \leqslant y$ kéo theo $\mathrm{S}_x \subset \mathrm{S}_y$, và $x < y$ kéo theo $\mathrm{S}_x \neq \mathrm{S}_y$; do đó ánh xạ $x \rightarrow \mathrm{S}_x$ là một đẳng cấu của E lên tập S(E) các đoạn của E phân biệt với chính E (§ 1, no. 12, Mệnh đề 11), và do đó S(E) được sắp thứ tự tốt. Hơn nữa, E\* đẳng cấu với tập được sắp thứ tự tốt thu được từ S(E) bằng cách thêm vào một phần tử lớn nhất.

#### Mệnh đề 3 {#ens-iii-s2-prop-3 .statement tag=03QQ}

*Cho* $(\mathrm{X}_\iota)_{\iota \in \mathbf{I}}$ *là một họ các tập được sắp thứ tự tốt sao cho với mỗi cặp chỉ số* $(\iota, \varkappa)$ *thì một trong các tập* $\mathrm{X}_\iota$, $\mathrm{X}_\varkappa$ *là một đoạn của tập kia. Khi đó tồn tại một thứ tự duy nhất trên tập* $\mathrm{E} = \bigcup_{\iota \in \mathbf{I}} \mathrm{X}_\iota$ *mà nó cảm sinh thứ tự đã cho trên từng* $\mathrm{X}_\iota$. *Được trang bị thứ tự này,* E *là một tập được sắp thứ tự tốt. Mỗi*

*đoạn của* $\mathrm{X}_\iota$ *đều là một đoạn của* E; *với mỗi* $x \in \mathrm{X}_\iota$, *đoạn có đầu mút* $x$ *trong* $\mathrm{X}_\iota$ *bằng đoạn có đầu mút* $x$ *trong* E; *và mỗi đoạn của* E *hoặc chính là* E *hoặc là một đoạn của một trong các* $\mathrm{X}_\iota$.

Mệnh đề đầu tiên là một hệ quả của bổ đề tổng quát sau :

#### Bổ đề 1 {#ens-iii-s2-lem-1 .statement tag=03QR}

*Cho* $(\mathrm{X}_\alpha)_{\alpha \in \mathrm{A}}$ *là một họ các tập hợp có thứ tự, có hướng đối với quan hệ* $\subset$ (nói cách khác, sao cho với mỗi cặp chỉ số $\alpha$, $\beta$ tồn tại một chỉ số $\gamma$ sao cho $\mathrm{X}_\alpha \subset \mathrm{X}_\gamma$ và $\mathrm{X}_\beta \subset \mathrm{X}_\gamma$). *Giả sử rằng, với mỗi cặp chỉ số* $(\alpha, \beta)$ *sao cho* $\mathrm{X}_\alpha \subset \mathrm{X}_\beta$, *thứ tự cảm sinh trên* $\mathrm{X}_\alpha$ *bởi thứ tự của* $\mathrm{X}_\beta$ *trùng với thứ tự đã cho trên* $\mathrm{X}_\alpha$. *Trong những điều kiện đó tồn tại một thứ tự duy nhất trên tập hợp* $\mathrm{E} = \bigcup_{\alpha \in \mathrm{A}} \mathrm{X}_\alpha$ *mà cảm sinh thứ tự đã cho trên mỗi* $\mathrm{X}_\alpha$.

Cho $\mathrm{G}_\alpha$ là đồ thị của thứ tự đã cho trên $\mathrm{X}_\alpha$. Nếu G là đồ thị của một thứ tự trên E mà trên mỗi $\mathrm{X}_\alpha$ cảm sinh thứ tự có đồ thị là $\mathrm{G}_\alpha$, thì ta phải có $\mathrm{G}_\alpha \subset \mathrm{G}$ với mọi $\alpha \in \mathrm{A}$; do đó G chứa $\bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$. Mặt khác, với mỗi cặp $(x, y)$ gồm các phần tử của E, theo giả thiết tồn tại một chỉ số $\alpha \in \mathrm{A}$ sao cho $x \in \mathrm{X}_\alpha$ và $y \in \mathrm{X}_\alpha$; nếu $(x, y) \in \mathrm{G}$, ta có $(x, y) \in \mathrm{G}_\alpha$, nên $\mathrm{G} \subset \bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$. Vậy nếu thứ tự cần tìm trên E tồn tại, thì đồ thị của nó tất yếu là $\mathrm{G} = \bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$. Còn lại cần chứng minh rằng tập hợp này thỏa mãn các điều kiện của bổ đề. Vì $\mathrm{G}_\beta \cap (\mathrm{X}_\alpha \times \mathrm{X}_\alpha) = \mathrm{G}_\alpha$ nếu $\mathrm{X}_\alpha \subset \mathrm{X}_\beta$, nên ta có $\mathrm{G} \cap (\mathrm{X}_\alpha \times \mathrm{X}_\alpha) = \mathrm{G}_\alpha$ với mọi $\alpha \in \mathrm{A}$; mặt khác, từ giả thiết suy ra rằng ba phần tử bất kỳ $x$, $y$, $z$ của E đều thuộc cùng một $\mathrm{X}_\alpha$. Do đó, $(x, y) \in \mathrm{G}$ là một quan hệ thứ tự trên E, và bổ đề đã được chứng minh.

¶ Bây giờ ta xét chứng minh của Mệnh đề 3. Trước hết ta chỉ ra rằng mỗi $\mathrm{X}_\iota$ là một đoạn của E. Thật vậy, nếu $x \in \mathrm{X}_\iota$, $y \in \mathrm{E}$, và $y \leqslant x$, thì tồn tại một chỉ số $\varkappa$ sao cho $\mathrm{X}_\iota \subset \mathrm{X}_\varkappa$ và $y \in \mathrm{X}_\varkappa$; theo giả thiết, vì $\mathrm{X}_\iota$ là một đoạn của $\mathrm{X}_\varkappa$, nên ta có $y \in \mathrm{X}_\iota$, điều đó chứng minh mệnh đề. Lập luận ấy cũng chứng minh rằng với mỗi $x \in \mathrm{X}_\iota$, đoạn có đầu mút $x$ trong $\mathrm{X}_\iota$ trùng với khoảng $]\leftarrow, x[$ trong E. Tiếp theo, ta chỉ ra rằng E được sắp tốt. Nếu H là một tập con không rỗng của E, thì tồn tại một chỉ số $\iota \in \mathrm{I}$ sao cho $\mathrm{H} \cap \mathrm{X}_\iota \neq \emptyset$; nếu $a$ là phần tử nhỏ nhất của $\mathrm{H} \cap \mathrm{X}_\iota$ trong $\mathrm{X}_\iota$, thì $a$ cũng là phần tử nhỏ nhất của H trong E. Nghĩa là, nếu $x \in \mathrm{H}$, thì tồn tại một chỉ số $\varkappa \in \mathrm{I}$ sao cho $\mathrm{X}_\iota \subset \mathrm{X}_\varkappa$ và $x \in \mathrm{X}_\varkappa$; không thể có $x < a$, vì khoảng $]\leftarrow, a[$ được chứa trong $\mathrm{X}_\iota$, và do đó ta có $x \geqslant a$ vì $\mathrm{X}_\varkappa$ được sắp thứ tự toàn phần.

¶ Cuối cùng, chúng ta phải chỉ ra rằng một đoạn của E, khác với chính E, là một đoạn của một trong các $\mathrm{X}_\iota$; đây là một hệ quả ngay lập tức của các lập luận trước đó, vì một đoạn như thế có dạng $]\leftarrow, x[$ (Mệnh đề 1) và vì $x$ thuộc một $\mathrm{X}_\iota$ nào đó.

### 2. NGUYÊN LÝ QUY NẠP SIÊU HẠN

#### Bổ đề 2 {#ens-iii-s2-lem-2 .statement tag=03K0}

*Cho E là một tập được sắp thứ tự tốt và $\mathscr{S}$ là một tập hợp các đoạn của E có các tính chất sau : (1) mọi hợp của các đoạn thuộc $\mathscr{S}$ đều thuộc $\mathscr{S}$; (2) nếu $S_x\in\mathscr{S}$, thì $S_x\cup\{x\}\in\mathscr{S}$. Khi đó mọi đoạn của E đều thuộc $\mathscr{S}$.*

Giả sử rằng có những đoạn của E không thuộc $\mathscr{S}$, và gọi S là đoạn nhỏ nhất trong số chúng (số 1, Mệnh đề 2). Nếu S không có phần tử lớn nhất, thì S là hợp của các đoạn của S phân biệt với chính nó, và các đoạn này thuộc $\mathscr{S}$ do định nghĩa của S; do đó S $\in\mathscr{S}$, điều này vô lý. Mặt khác, nếu S có một phần tử lớn nhất $a$, thì $S=S_a\cup\{a\}$, và vì $S_a$ là một đoạn của S phân biệt với S, ta có $S_a\in\mathscr{S}$; nhưng khi đó cũng có $S\in\mathscr{S}$, điều này lại vô lý.

¶ Để thuận tiện hơn, ta đặt mình trong một lý thuyết $\mathscr{T}$ trong đó E là một tập hợp *được sắp tốt* bởi một quan hệ được viết là $x\leq y$. Khi đó ta có các tiêu chuẩn sau :

C59. (Nguyên lý quy nạp siêu hạn). *Cho $\mathrm{R}\{x\}$ là một quan hệ trong $\mathscr{T}$ ($x$ không là một hằng số của $\mathscr{T}$) sao cho quan hệ*

$$
(x\in E\ \mathrm{and}\ (\forall y)((y\in E\ \mathrm{and}\ y<x)\Longrightarrow \mathrm{R}\{y\}))\Longrightarrow \mathrm{R}\{x\}
$$

*là một định lý trong $\mathscr{T}$. Trong các điều kiện này, quan hệ $(x\in E)\Longrightarrow \mathrm{R}\{x\}$ là một định lý trong $\mathscr{T}$.*

Gọi $\mathscr{S}$ là tập hợp các đoạn S của E sao cho $(y\in S)\Longrightarrow \mathrm{R}\{y\}$. Rõ ràng mọi hợp của các đoạn thuộc $\mathscr{S}$ cũng thuộc $\mathscr{S}$. Mặt khác, nếu $S_x\in\mathscr{S}$, thì ta có $\mathrm{R}\{x\}$ theo giả thiết; do đó $(y\in S_x\cup\{y\})\Longrightarrow \mathrm{R}\{y\}$ theo phương pháp phân biệt các trường hợp. Vậy nên (Bổ đề 2) $E\in\mathscr{S}$, điều này chứng minh tiêu chuẩn.

¶ Trong các ứng dụng của C59, quan hệ

$$
x\in E\ \mathrm{and}\ (\forall y)((y\in E\ \mathrm{and}\ y<x)\Longrightarrow \mathrm{R}\{y\})
$$

thường được gọi là “giả thiết quy nạp”.

¶ Trong điều sau đây, với mỗi ánh xạ $g$ của một đoạn S của E vào một tập hợp F, và với mỗi $x\in S$ ta sẽ ký hiệu bởi $g^{(x)}$ ánh xạ của đoạn $S_x=]\leftarrow, x[$ của E lên $g(S_x)$, ánh xạ này trùng với $g$ trên $S_x$. Với ký hiệu này ta có

C60. (Định nghĩa một ánh xạ bằng quy nạp siêu hạn.) *Cho $u$ là một chữ cái, $\mathscr{T}\{u\}$ là một số hạng trong lý thuyết $\mathscr{T}$. Tồn tại một tập hợp U và một ánh xạ $f$ của E lên U sao cho với mọi $x\in E$ ta có $f(x)=\mathscr{T}\{f^{(x)}\}$. Hơn nữa, tập hợp U và ánh xạ $f$ được xác định duy nhất bởi các điều kiện này.*

Trước hết, hãy chứng minh tính duy nhất. Giả sử rằng $f'$ và $\mathrm{U}'$ cũng thỏa mãn các điều kiện của tiêu chuẩn. Gọi $\mathfrak{S}$ là tập hợp các đoạn S của E sao cho $f$ và $f'$ trùng nhau trên S. Hiển nhiên là mọi hợp của các đoạn thuộc $\mathfrak{S}$ cũng thuộc $\mathfrak{S}$. Mặt khác, nếu $\mathrm{S}_x \in \mathfrak{S}$, thì $f$ và $f'$ trùng nhau trên $\mathrm{S}_x$ và do đó $f^{(x)} = f'^{(x)}$; do đó

$$f(x) = \mathrm{T}\{f^{(x)}\} = \mathrm{T}\{f'^{(x)}\} = f'(x),$$

điều đó cho thấy rằng $\mathrm{S}_x \cup \{x\} \in \mathfrak{S}$. Suy ra $\mathrm{E} \in \mathfrak{S}$ (Bổ đề 2), do đó $f' = f$ và $\mathrm{U}' = f'(\mathrm{E}) = f(\mathrm{E}) = \mathrm{U}$.

¶ Bây giờ ký hiệu $\mathfrak{S}_1$ là tập hợp các đoạn S của E sao cho tồn tại một tập hợp $\mathrm{U_S}$ và một ánh xạ $f_\mathrm{S}$ từ S *lên* $\mathrm{U_S}$ sao cho với mọi $x \in \mathrm{S}$ ta có $f_\mathrm{S}(x) = \mathrm{T}\{f^{(x)}\}$. Với mỗi $\mathrm{S} \in \mathrm{S}_1$, $f_\mathrm{S}$ và $\mathrm{U_S}$ được xác định duy nhất, theo phần đầu của chứng minh; đặc biệt, nếu $\mathrm{S}'$ và $\mathrm{S}''$ là hai đoạn thuộc $\mathfrak{S}_1$ sao cho $\mathrm{S}' \subset \mathrm{S}''$, thì $f_{\mathrm{S}'}$ là ánh xạ từ $\mathrm{S}'$ lên $f_{\mathrm{S}''}(\mathrm{S}')$ trùng với $f_{\mathrm{S}''}$ trên $\mathrm{S}'$. Từ chú ý này suy ra mọi hợp của các đoạn thuộc $\mathfrak{S}_1$ cũng thuộc $\mathfrak{S}_1$ (Chương II, § 4, no. 6, Mệnh đề 7). Mặt khác, nếu $\mathrm{S}_x \in \mathfrak{S}_1$, ta định nghĩa trên $\mathrm{S} = \mathrm{S}_x \cup \{x\}$ một hàm $f_\mathrm{S}$ mở rộng $f_{\mathrm{S}_x}$ bằng cách đặt

$$f_\mathrm{S}(x) = \mathrm{T}\{f_{\mathrm{S}_x}\}$$

(Chương II, § 4, no. 7, Mệnh đề 8); vì $f_\mathrm{S}^{(x)} = f_{\mathrm{S}_x}$, hiển nhiên là $\mathrm{S}_x \cup \{x\} \in \mathfrak{S}_1$. Do đó (Bổ đề 2) $\mathrm{E} \in \mathfrak{S}_1$, và chứng minh như vậy là đầy đủ.

¶ Thông thường tiêu chuẩn này được áp dụng trong những tình huống mà tồn tại một tập hợp F sao cho *với mọi ánh xạ h của một đoạn của* E *lên một tập con của* F *ta có* $\mathrm{T}\{h\} \in \mathrm{F}$. Khi đó tập hợp U thu được bằng cách áp dụng C60 là một *tập con của* F. Thật vậy, với ký hiệu đã dùng ở trên, gọi $\mathfrak{S}_2$ là tập con của $\mathfrak{S}_1$ gồm các đoạn S của E sao cho $\mathrm{U_S} \subset \mathrm{F}$. Hiển nhiên là mọi hợp của các đoạn thuộc $\mathfrak{S}_2$ cũng thuộc $\mathfrak{S}_2$; mặt khác, giả thiết trên F kéo theo rằng nếu $\mathrm{S}_x \in \mathfrak{S}_2$, thì ta có $\mathrm{S}_x \cup \{x\} \in \mathfrak{S}_2$. Mệnh đề này bây giờ suy ra từ Bổ đề 2.

### 3. ĐỊNH LÝ ZERMELO

#### Bổ đề 3 {#ens-iii-s2-lem-3 .statement tag=03K1}

*Cho* E *là một tập hợp, cho* $\mathfrak{S}$ *là một tập con của* $\mathfrak{P}(\mathrm{E})$, *và cho* $p$ *là một ánh xạ của* $\mathfrak{S}$ *vào* E *sao cho* $p(\mathrm{X}) \notin \mathrm{X}$ *với mọi* $\mathrm{X} \in \mathfrak{S}$. *Khi đó tồn tại một tập con* M *của* E *và một thứ tự tốt* $\Gamma$ *trên* M *sao cho, nếu* $x \leqslant y$ *ký hiệu quan hệ* $y \in \Gamma\langle x \rangle$ *và* $\mathrm{S}_x$ *ký hiệu đoạn* $]\leftarrow, x]$,

(1) *với mọi* $x \in \mathrm{M}$ *ta có* $\mathrm{S}_x \in \mathfrak{S}$ *và* $p(\mathrm{S}_x) = x$;

(2) $\mathrm{M} \notin \mathfrak{S}$.

Cho $\mathfrak{M}$ là tập hợp các tập con G của $\mathrm{E} \times \mathrm{E}$ thỏa mãn các điều kiện sau :

(a) G là đồ thị của một quan hệ thứ tự tốt trên $\mathrm{pr}_1 \mathrm{G} = \mathrm{U}$;

(b) nếu $x \leqslant y$ ký hiệu quan hệ $(x, y) \in \mathrm{G}$ trên U, thì với mỗi $x \in \mathrm{U}$, đoạn đầu $\mathrm{S}_x$ sao cho $\mathrm{S}_x \in \mathfrak{S}$ và $p(\mathrm{S}_x) = x$.

¶ Ta sẽ chỉ ra rằng nếu G và G' là hai phần tử của M và nếu U, U' ký hiệu các hình chiếu thứ nhất của chúng, thì một trong hai tập hợp U, U' được chứa trong tập hợp kia và nếu, chẳng hạn, $\mathrm{U} \subset \mathrm{U}'$, thì $\mathrm{G} = \mathrm{G}' \cap (\mathrm{U} \times \mathrm{U})$ (nói cách khác, quan hệ thứ tự trên U được cảm sinh bởi quan hệ thứ tự trên U') và U là một *đoạn đầu* của U'.

¶ Xét tập hợp V gồm các phần tử $x \in \mathrm{U} \cap \mathrm{U}'$ sao cho các đoạn có đầu mút $x$ là như nhau trong U và U', và sao cho các thứ tự cảm sinh trên đoạn này bởi các thứ tự trên U và U' là trùng nhau. Rõ ràng V là một *đoạn* trong cả U lẫn U' và các thứ tự cảm sinh trên V là như nhau; do đó mệnh đề của chúng ta sẽ được đã chứng minh nếu ta chỉ ra rằng либо $\mathrm{V} = \mathrm{U}$ hoặc $\mathrm{V} = \mathrm{U}'$. Ta lập luận bằng phản chứng và giả sử rằng $\mathrm{V} \neq \mathrm{U}$ và $\mathrm{V} \neq \mathrm{U}'$. Gọi $x$ là phần tử nhỏ nhất của $\mathrm{U} - \mathrm{V}$ trong U và gọi $x'$ là phần tử nhỏ nhất của $\mathrm{U}' - \mathrm{V}$ trong U'; ta có $\mathrm{V} = \mathrm{S}_x$ trong U, và $\mathrm{V} = \mathrm{S}_{x'}$ trong U'. Nhưng theo giả thiết, $\mathrm{V} \in \mathfrak{S}$ và

$$x = p(\mathrm{S}_x), \qquad x' = p(\mathrm{S}_{x'}),$$

so that $x = x'$. Do đó theo định nghĩa $x \in \mathrm{V}$, điều này vô lý.

¶ Vì vậy ta có thể áp dụng Mệnh đề 3 của số 1 cho tập hợp các ảnh chiếu thứ nhất $\mathrm{U} = \mathrm{pr}_1 \mathrm{G}$ (trong đó $\mathrm{G} \in \mathfrak{M}$) và do đó thu được một tập được sắp thứ tự tốt

$$\mathrm{M} = \bigcup_{\mathrm{G} \in \mathfrak{M}} \mathrm{pr}_1 \mathrm{G}.$$

Dễ thấy rằng đồ thị của thứ tự trên M thuộc $\mathfrak{M}$. Nếu ta có $\mathrm{M} \in \mathrm{S}$, thì, đặt $a = p(\mathrm{M})$, ta sẽ có $a \notin \mathrm{M}$. Vì vậy ta có thể thêm vào M phần tử $a$ như là phần tử lớn nhất, và tập $\mathrm{M}' = \mathrm{M} \cup \{a\}$ sẽ được sắp thứ tự tốt. Vì $\mathrm{M} = \mathrm{S}_a$ trong M', ta sẽ có $\mathrm{S}_a \in \mathfrak{S}$ và $p(\mathrm{S}_a) = a$; do đó đồ thị của thứ tự trên M' sẽ thuộc $\mathfrak{M}$, điều này vô lý.

Chú ý rằng nếu $\emptyset \notin \mathfrak{S}$ (và đặc biệt nếu $\mathfrak{S}$ rỗng), thì tập hợp M mà Bổ đề 3 khẳng định sự tồn tại là tập rỗng; điều này suy ra từ điều kiện 1 của Bổ đề 3.

#### Định lý 1 (Zermelo) {#ens-iii-s2-thm-1 .statement tag=03QS}

*Mọi tập hợp* E *đều có thể được sắp tốt.*

Cho $\mathfrak{S} = \mathfrak{P}(\mathrm{E}) - \{\mathrm{E}\}$ là tập hợp tất cả các tập con của E khác với chính E. Với mỗi $\mathrm{X} \in \mathfrak{S}$, đặt $p(\mathrm{X}) = \tau_x \ (x \in \mathrm{E} - \mathrm{X})$; vì quan hệ $\mathrm{X} \in \mathfrak{S}$

suy ra $(\exists x)(x \in \mathrm{E} - \mathrm{X})$, nên ta có $p(\mathrm{X}) \in \mathrm{E} - \mathrm{X}$ (Chương I, § 4, số 1) và do đó $p(\mathrm{X}) \notin \mathrm{X}$. Vậy ta có thể áp dụng Bổ đề 3, và do đó tồn tại một sắp tốt trên một tập con M của E sao cho $\mathrm{M} \notin \mathfrak{S}$; nhưng tập con duy nhất của E không thuộc $\mathfrak{S}$ là chính E, và định lý được chứng minh.

### 4. TẬP HỢP QUY NẠP

#### Định nghĩa 3 {#ens-iii-s2-def-3 .statement tag=03K2}

*Một tập hợp có thứ tự* E *được gọi là quy nạp nếu mọi tập con được sắp thứ tự toàn phần của* E *đều có một cận trên trong* E.

*Các ví dụ*

#### Ví dụ 1 {#ens-iii-s2-n4-exa-1 .statement tag=03T2}

Cho $\mathfrak{F}$ là một tập hợp các tập con của một tập hợp A, được sắp thứ tự bởi quan hệ bao hàm, và sao cho với mọi tập con được sắp thứ tự toàn phần $\mathfrak{G}$ của $\mathfrak{F}$ thì hợp của các tập hợp thuộc $\mathfrak{G}$ thuộc $\mathfrak{F}$. Khi đó $\mathfrak{F}$ là quy nạp đối với quan hệ $\subset$ vì hợp của các tập hợp thuộc $\mathfrak{G}$ là cận trên bé nhất của $\mathfrak{G}$ trong $\mathfrak{P}(\mathrm{A})$.

#### Ví dụ 2 {#ens-iii-s2-n4-exa-2 .statement tag=03T3}

Một ví dụ quan trọng về một tập hợp các tập con là quy nạp đối với quan hệ $\subset$ là tập hợp $\mathfrak{F}$ gồm các đồ thị của các ánh xạ từ các tập con của một tập hợp A vào một tập hợp B. Thật vậy, $\mathfrak{F}$ là một tập con của $\mathfrak{P}(\mathrm{A} \times \mathrm{B})$, và nói rằng một tập con $\mathfrak{G}$ của $\mathfrak{F}$ được sắp thứ tự toàn phần theo quan hệ bao hàm có nghĩa là các phần tử của $\mathfrak{G}$ là các đồ thị của những ánh xạ sao cho, với hai ánh xạ bất kỳ trong số đó, một ánh xạ là một mở rộng của ánh xạ kia. Từ đó ngay lập tức suy ra rằng hợp của các tập hợp thuộc $\mathfrak{G}$ là một phần tử của $\mathfrak{F}$ (Chương II, § 4, no. 6, Mệnh đề 7). Vì thế tập hợp $\Phi(\mathrm{A}, \mathrm{B})$ các ánh xạ từ các tập con của A vào B là quy nạp đối với quan hệ thứ tự "$v$ mở rộng $u$" giữa $u$ và $v$.

#### Ví dụ 3 {#ens-iii-s2-n4-exa-3 .statement tag=03T4}

Từ tiên đề vô hạn (§ 6, no. 1) suy ra rằng tập được sắp thứ tự tốt các số nguyên tự nhiên không là quy nạp đối với quan hệ $\leqslant$. \*

#### Định lý 2 ("bổ đề Zorn") {#ens-iii-s2-thm-2 .statement tag=03QT}

— *Mọi tập hợp có thứ tự quy nạp đều có một phần tử cực đại.*

Định lý này là một trường hợp riêng của kết quả sau :

#### Mệnh đề 4 {#ens-iii-s2-prop-4 .statement tag=03K3}

*Cho* E *là một tập hợp có thứ tự sao cho mọi tập con được sắp tốt của nó đều bị chặn trên; khi đó* E *có một phần tử cực đại.*

Ta sẽ nói rằng một phần tử $v \in \mathrm{E}$ là một *cận trên ngặt* của một tập con X của E nếu $v$ là một cận trên của X và $v \notin \mathrm{X}$. Gọi $\mathfrak{S}$ là tập hợp các tập con của E có một cận trên ngặt trong E, và với mỗi $\mathrm{S} \in \mathfrak{S}$ đặt $p(\mathrm{S}) = \tau_v(v$ là một cận trên ngặt của S$)$; khi đó $p(\mathrm{S})$ là một cận trên ngặt của S. Áp dụng Bổ đề 3 của no. 3 cho $\mathfrak{S}$ và $p$, ta thấy rằng tồn tại một tập con M của E và một thứ tự tốt $\Gamma$ trên M thỏa mãn the

các điều kiện của Bổ đề 3; đặc biệt, M không có cận trên ngặt trong E. Hơn nữa, thứ tự $\Gamma$ trùng với thứ tự cảm sinh trên M bởi thứ tự trên E. Vì trong M, quan hệ “$y\in\Gamma\langle x\rangle$ và $x\ne y$” tương đương với $x\in S_y$; và vì $p(S_y)=y$ là một cận trên của $S_y$ (đối với thứ tự trên E), nên suy ra $x<y$ trong E. Nhưng điều đó có nghĩa là ánh xạ đơn ánh từ M vào E là một ánh xạ tăng ngặt (M được trang bị thứ tự $\Gamma$); và vì M được sắp thứ tự toàn phần, suy ra các quan hệ $y\in\Gamma\langle x\rangle$ và $x\leq y$ tương đương trong M (§ 1, no. 12, Mệnh đề 11). Do đó, theo giả thiết, tồn tại một cận trên $m$ của M trong E; nhưng vì M không có cận trên ngặt, suy ra $m$ là một phần tử cực đại của E.

#### Hệ quả 1 {#ens-iii-s2-prop-4-cor-1 .statement tag=03K4}

*Cho E là một tập hợp có thứ tự quy nạp và cho $a$ là một phần tử của E. Khi đó tồn tại một phần tử cực đại $m$ của E sao cho $m\geq a$.*

Vì theo Định nghĩa 3, tập hợp F gồm các phần tử $x\geq a$ của E là quy nạp, và một phần tử cực đại của F cũng là một phần tử cực đại của E.

#### Hệ quả 2 {#ens-iii-s2-prop-4-cor-2 .statement tag=03K5}

*Cho $\mathscr{F}$ là một tập hợp các tập con của một tập hợp E sao cho, với mọi tập con $\mathscr{G}$ của $\mathscr{F}$ được sắp thứ tự toàn phần bởi quan hệ bao hàm, hợp (tương ứng giao) của các tập hợp thuộc $\mathscr{G}$ đều thuộc $\mathscr{F}$; khi đó $\mathscr{F}$ có một phần tử cực đại (tương ứng cực tiểu).*

### 5. ĐẲNG CẤU CỦA CÁC TẬP HỢP ĐƯỢC SẮP TỐT

#### Định lý 3 {#ens-iii-s2-thm-3 .statement tag=03K6}

*Cho E và F là hai tập hợp được sắp tốt. Khi đó ít nhất một trong hai mệnh đề sau là đúng :*

(1) *tồn tại một đẳng cấu duy nhất của E lên một đoạn của F;*

(2) *tồn tại một đẳng cấu duy nhất của F lên một đoạn của E.*

Cho $\mathscr{F}$ là tập hợp các ánh xạ từ các tập con của E vào F sao cho mỗi ánh xạ được định nghĩa trên một đoạn của E và là một đẳng cấu từ đoạn này lên một đoạn của F. Khi đó tập hợp $\mathscr{F}$, được sắp thứ tự bởi quan hệ “$v$ mở rộng $u$” giữa $u$ và $v$, là *quy nạp*. Thật vậy, nếu $\mathscr{G}$ là một tập con được sắp thứ tự toàn phần của $\mathscr{F}$, thì hợp S của các miền xác định của các ánh xạ $u\in\mathscr{G}$ là một hợp của các đoạn của E và do đó chính nó cũng là một đoạn của E. Nếu $v$ là cận trên bé nhất của $\mathscr{G}$ trong $\Phi(E,F)$ (số 4, Ví dụ 2), thì $v(S)$ là hợp của các ảnh của các ánh xạ $u\in\mathscr{G}$ và do đó là một đoạn của F. Sau cùng, với mỗi cặp phần tử $x$, $y$ của S sao cho $x<y$ thì tồn tại $u\in\mathscr{G}$ mà miền xác định chứa cả $x$ và $y$ (vì $\mathscr{G}$ được sắp thứ tự toàn phần); và vì $v(x)=u(x)<u(y)=v(y)$, nên $v$ là một đẳng cấu từ S lên $v(S)$, và mệnh đề của chúng ta đã được chứng minh.

¶ Bây giờ, cho $u_0$ là một phần tử cực đại của $\mathfrak{S}$ (no. 4, Định lý 2) và $S_0$ là đoạn của E là miền xác định của $u_0$. Nếu ta chứng minh rằng hoặc $S_0=E$ hoặc $u_0(S_0)=F$, thì định lý sẽ được chứng minh. Ta lập luận bằng phản chứng và giả sử rằng $S_0\ne E$ và $u_0(S_0)\ne F$. Khi đó tồn tại một phần tử $a\in E$ và một phần tử $b\in F$ sao cho $S_0=]\leftarrow,a[$ và $u_0(S_0)=]\leftarrow,b[$ (no. 1, Mệnh đề 1). Mở rộng $u_0$ thành một ánh xạ $u_1$ của đoạn $]\leftarrow,a]$ vào F bằng cách đặt $u_1(a)=b$; vì $u_1$ là một đẳng cấu của $]\leftarrow,a]$ lên đoạn $]\leftarrow,b]$, điều này mâu thuẫn với tính cực đại của $u_0$ trong $\mathfrak{S}$.

¶ Tính duy nhất được khẳng định trong Định lý 3 là hệ quả của Bổ đề sau :

#### Bổ đề 4 {#ens-iii-s2-lem-4 .statement tag=03K7}

*Cho E, F là hai tập hợp được sắp tốt và $f$, $g$ là hai ánh xạ tăng từ E vào F sao cho $f(E)$ là một đoạn của F và $g$ tăng ngặt; khi đó $f(x)\leq g(x)$ với mọi $x\in E$.*

Giả sử ngược lại rằng tập các phần tử $y\in E$ sao cho $f(y)>g(y)$ không rỗng; khi đó tập này có một phần tử nhỏ nhất $a$. Nếu $x<a$, thì ta có $f(x)\leq g(x)<g(a)<f(a)$ vì $g$ tăng ngặt. Vì $f(E)$ là một đoạn của F, tồn tại $z\in E$ sao cho $g(a)=f(z)$; $f$ tăng, nên $f(z)<f(a)$ suy ra $z<a$. Do đó

$$
f(z)\leq g(z)<g(a)=f(z),
$$

điều này là vô lý.

#### Hệ quả 1 {#ens-iii-s2-lem-4-cor-1 .statement tag=03K8}

*Đẳng cấu duy nhất từ một tập được sắp thứ tự tốt E lên một đoạn của E là ánh xạ đồng nhất của E lên chính nó.*

Đặt $F=E$ trong Định lý 3.

#### Hệ quả 2 {#ens-iii-s2-lem-4-cor-2 .statement tag=03K9}

*Cho E, F là hai tập hợp được sắp thứ tự tốt. Nếu tồn tại một đẳng cấu $f$ từ E lên một đoạn đầu T của F và một đẳng cấu $g$ từ F lên một đoạn đầu S của E, thì tất phải có $S=E$, $T=F$, và $g$, $f$ là các ánh xạ ngược của nhau.*

Thật vậy, $g\mathbin{\circ}f$ là một đẳng cấu của E lên đoạn đầu $g(T)\subset S$ của E; theo Hệ quả 1 ta có $g(T)=S=E$, và $g\mathbin{\circ}f$ là ánh xạ đồng nhất của E. Tương tự, $f\mathbin{\circ}g$ là ánh xạ đồng nhất của F, do đó suy ra kết quả.

#### Hệ quả 3 {#ens-iii-s2-lem-4-cor-3 .statement tag=03KA}

*Mọi tập con A của một tập được sắp thứ tự tốt E đều đẳng cấu với một đoạn đầu của E.*

Theo Định lý 3, chỉ cần chứng minh rằng không tồn tại đẳng cấu $g$ từ E lên một đoạn của A có dạng $S_a$. Nếu có, thì $g$ khi đó sẽ là một ánh xạ tăng ngặt từ E vào E sao cho $g(a)\in S_a$, nói cách khác sao cho $g(a)<a$; nhưng bất đẳng thức này mâu thuẫn với Bổ đề 4 (với $f$ là ánh xạ đồng nhất).

### 6. CÁC TÍCH TỪ ĐIỂN

Cho $(E_\ell)_{\ell\in I}$ là một họ các tập hợp có thứ tự, được đánh chỉ số bởi một tập hợp *được sắp tốt* $I$. Xét tập hợp tích $E=\prod_{\ell\in I}E_\ell$, và quan hệ

$$
“x\in E\text{ và }y\in E,\text{ và đối với chỉ số nhỏ nhất }\ell\in I\text{ sao cho }\operatorname{pr}_\ell x\ne\operatorname{pr}_\ell y,\text{ ta có }\operatorname{pr}_\ell x<\operatorname{pr}_\ell y”,
$$

ta sẽ ký hiệu bởi $R\{x,y\}$. Rõ ràng $R\{x,x\}$ tương đương với $x\in E$, $R\{x,y\}$ suy ra $R\{x,x\}$ và $R\{y,y\}$, và $(R\{x,y\}$ và $R\{y,x\})$ suy ra $x=y$. Cũng dễ dàng kiểm tra rằng $(R\{x,y\}$ và $R\{y,z\})$ suy ra $R\{x,z\}$ (xét chỉ số nhỏ nhất $\ell\in I$ sao cho ít nhất hai trong ba phần tử $\operatorname{pr}_\ell x$, $\operatorname{pr}_\ell y$, $\operatorname{pr}_\ell z$ khác nhau); do đó $R\{x,y\}$ là một *quan hệ thứ tự* trên *tập hợp tích* $E$. Quan hệ này và thứ tự mà nó xác định được gọi là *quan hệ thứ tự từ điển* và *thứ tự từ điển* trên $E$ (được cảm sinh bởi các thứ tự đã cho trên $I$ và trên các $E_\ell$); tập hợp $E$ với thứ tự này được gọi là *tích từ điển* của họ các tập hợp có thứ tự $(E_\ell)_{\ell\in I}$. Nếu mỗi $E_\ell$ đều *được sắp thứ tự toàn phần* thì tích từ điển cũng *được sắp thứ tự toàn phần*.

### Bài tập {#ens-iii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
