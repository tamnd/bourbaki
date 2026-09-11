---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 7
section_title: Powers. Countable sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 380-382
pdf_pages: 0385-0387
extraction: ocr
statements: 0
exercises: 0
content_sha256: 26aba631f000e25656e8062fa0873179a33e89777695f84eaa13705f81dfb27b
translated_from: content/en/ens/ER/07_s7_powers_countable_sets.md
source_content_sha256: 86ddec08acce4507f77a4f26c22ecf7fe435bb7014433e7736350957d8534e86
translation_model: gpt-5-6
translation_run: translate-vi-899df937
glossary_version: 34
glossary_terms_sha256: 99a586d5ab8aa23df673a4fd88665e2c95a28c73dd1c1e42a56bcacce1aa066b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 7. LŨY THỪA. CÁC TẬP ĐẾM ĐƯỢC

1. Hai tập hợp E, F được gọi là *đồng lực* nếu chúng có thể được đặt trong một sự tương ứng một-một.
Hai tập hợp, mỗi tập hợp đồng lực với một tập hợp thứ ba, thì đồng lực với nhau.
Nếu E và F đồng lực, thì $\mathfrak{P}(E)$ và $\mathfrak{P}(F)$ đồng lực.
Nếu E và F, E′ và F′, E″ và F″ tương ứng đồng lực, thì $E\times E'\times E''$ và $F\times F'\times F''$ đồng lực. Mệnh đề này mở rộng cho tích của một số tùy ý các tập hợp.

2. Cho X và Y là hai tập con tùy ý của một tập hợp E. Quan hệ “X và Y đồng lực” là một *quan hệ tương đương* trên $\mathfrak{P}(E)$. Lớp tương đương (đối với quan hệ này) mà X thuộc vào được gọi là *lũy thừa* [^1] của X, và tập hợp các lớp này (nghĩa là thương của $\mathfrak{P}(E)$ bởi quan hệ trên) được gọi là *tập hợp các lũy thừa* của các tập con của E.
Nếu E và F là hai tập hợp phân biệt, quan hệ “X và Y đồng lực” giữa một tập con X của E và một tập con Y của F được diễn đạt bằng cách nói rằng lũy thừa của X và lũy thừa của Y là *tương đương*. Theo cách này ta có một sự tương ứng một-một giữa một tập con của tập hợp các lũy thừa của các tập con của E và một tập con của tập hợp các lũy thừa của các tập con của F.

3. Cho E, F là hai tập hợp bất kỳ, có thể phân biệt hoặc không, và cho $\mathfrak{a}$ (tương ứng $\mathfrak{b}$) là một phần tử của tập hợp các lũy thừa của các tập con của E (tương ứng F). Khi đó $\mathfrak{a}$ được gọi là *nhỏ hơn* $\mathfrak{b}$, hoặc $\mathfrak{b}$ *lớn hơn* $\mathfrak{a}$, nếu tồn tại một ánh xạ một-một của một tập con $X\subset E$ có lũy thừa $\mathfrak{a}$ vào một tập con $Y\subset F$ có lũy thừa $\mathfrak{b}$. Nếu ngoài ra $\mathfrak{a}$ và $\mathfrak{b}$ không phải là các lũy thừa tương đương, thì $\mathfrak{a}$ được gọi là *nhỏ hơn nghiêm ngặt* $\mathfrak{b}$, hoặc $\mathfrak{b}$ *lớn hơn nghiêm ngặt* $\mathfrak{a}$.

Nếu $\mathfrak{a}$ và $\mathfrak{b}$ tương đương, thì $\mathfrak{a}$ vừa lớn hơn vừa nhỏ hơn $\mathfrak{b}$.

Ngược lại, định lý nói rằng *nếu $\mathfrak{a}$ vừa lớn hơn vừa nhỏ hơn $\mathfrak{b}$, thì $\mathfrak{a}$ và $\mathfrak{b}$ tương đương.* Suy ra đặc biệt rằng tập hợp các lũy thừa của các tập con của một tập hợp E là *có thứ tự* bởi quan hệ “$\mathfrak{a}$ nhỏ hơn $\mathfrak{b}$”; mỗi khi ta nói về tập hợp này như một tập hợp có thứ tự, thì luôn luôn ta muốn nói đến thứ tự được xác định bởi quan hệ này.

Hơn nữa, sử dụng bổ đề Zorn (và do đó tiên đề lựa chọn), người ta chứng minh rằng *tập hợp các lũy thừa của các tập con của một tập hợp E được sắp tốt.*

4. Lũy thừa của một tập hợp E là *nhỏ hơn nghiêm ngặt* lũy thừa của tập hợp $\mathfrak{P}(E)$.

Nếu $f$ là một ánh xạ từ một tập hợp E vào một tập hợp F, thì lũy thừa của ảnh $f(X)$ của mọi tập con X của E là *nhỏ hơn* lũy thừa của X.

5. Cho $(X_i)_{i\in I}$ là một họ các tập con của một tập hợp E sao cho $X_i\cap X_k=\varnothing$ với mọi $i\ne k$. Cho $(Y_i)_{i\in I}$ là một họ các tập con của một tập hợp F, được đánh chỉ số bởi cùng một tập hợp I và sao cho lũy thừa của $Y_i$ là *nhỏ hơn* lũy thừa của $X_i$, với mọi $i\in I$. Khi đó lũy thừa của hợp $\bigcup_{i\in J}Y_i$ là *nhỏ hơn* lũy thừa của $\bigcup_{i\in J}X_i$ với mọi tập con J của I.

Nếu thêm nữa $Y_i\cap Y_k=\varnothing$ với mọi $i\ne k$, và nếu $X_i$ và $Y_i$ *đồng lực* với mọi $i\in I$, thì $\bigcup_{i\in J}X_i$ *đồng lực* với $\bigcup_{i\in J}Y_i$.

Đặc biệt, nếu F và E là cùng một tập hợp, ta thấy rằng lũy thừa của hợp của một họ các tập con *rời nhau từng đôi một* của E chỉ phụ thuộc vào các lũy thừa của các tập con này; nó được gọi là *tổng* của các lũy thừa này (do đó hàm này được xác định đối với một họ $(\mathfrak{a}_i)$ của các phần tử của tập hợp các lũy thừa chỉ khi tồn tại một họ $(X_i)$ các tập con rời nhau từng đôi một của E sao cho $X_i$ có lũy thừa $\mathfrak{a}_i$ với mỗi chỉ số $i$).

Nếu $(X_i)_{i\in I}$ và $(Y_i)_{i\in I}$ là các họ tập con của E và F, tương ứng, được lập chỉ số bởi cùng một tập hợp I sao cho $X_i$ và $Y_i$ *có cùng lực lượng* với mọi $i$, thì các tích $\prod_i X_i$ và $\prod_i Y_i$ *có cùng lực lượng*.

6. Tập hợp $\mathbf{N}$ các số nguyên tự nhiên có thể được xem như tập hợp các lũy thừa của các tập con *hữu hạn* của một tập *vô hạn*. Quan hệ thứ tự “$x\leq y$” trên $\mathbf{N}$ chính là quan hệ sắp thứ tự tập hợp các lũy thừa này, và *tổng* của hai số nguyên tự nhiên là một hàm đồng nhất với tổng của hai lũy thừa như đã định nghĩa ở trên.

7. Một tập hợp được gọi là *đếm được* nếu nó tương đương với một tập con của tập hợp $\mathbf{N}$ các số nguyên tự nhiên. Do đó, *mọi tập hợp hữu hạn* đều đếm được; nếu nó có $n$ phần tử, thì nó có cùng lực lượng với khoảng $[0,n-1]$ của tập hợp $\mathbf{N}$. Mọi

## TÓM TẮT CÁC KẾT QUẢ

tập hợp *vô hạn đếm được* đều có cùng lực lượng với $\mathbf{N}$; đặc biệt, mọi tập con vô hạn của $\mathbf{N}$ đều có cùng lũy thừa với $\mathbf{N}$.

Nếu $E$ là một tập hợp *vô hạn*, thì tồn tại một *phân hoạch* của $E$ thành các tập hợp *vô hạn đếm được*; đặc biệt, mọi tập hợp vô hạn đều có lũy thừa *lớn hơn* lũy thừa của $\mathbf{N}$.

Nếu $E$ là một tập hợp *vô hạn*, thì các tập hợp $E \times E$ và $E \times \mathbf{N}$ đều *có cùng lực lượng* với $E$, và tập hợp các *tập con hữu hạn* của $E$ *có cùng lực lượng* với $E$. Đặc biệt, $\mathbf{N} \times \mathbf{N}$ là một tập hợp *vô hạn đếm được*.

8. Một *dãy các phần tử* của một tập hợp $E$ theo định nghĩa là một họ các phần tử của $E$, được lập chỉ số bởi tập hợp $\mathbf{N}$ hoặc một tập con của $\mathbf{N}$. Do đó, một dãy có tập chỉ số là $\mathbf{N}$ được viết $(x_n)_{n\in\mathbf{N}}$, hoặc đơn giản hơn là $(x_n)$ khi không có khả năng nhầm lẫn. Nếu $n$ ký hiệu một số nguyên bất kỳ, thì $x_n$ được gọi là *số hạng tổng quát* của dãy, hoặc *số hạng thứ n*. Thuật ngữ sau cũng được dùng khi $n$ được thay bởi một số nguyên cụ thể. Tập hợp các phần tử của một dãy là đếm được.

Một dãy được gọi là *vô hạn* hoặc *hữu hạn* tùy theo tập chỉ số là một tập con vô hạn hoặc hữu hạn của $\mathbf{N}$. Tập hợp các phần tử của một dãy hữu hạn là hữu hạn.

Mọi họ con của một dãy lại là một dãy, gọi là *dãy con* của dãy đã cho. Mọi dãy con của một dãy hữu hạn đều là một dãy hữu hạn.

Một họ các phần tử có tập chỉ số là $\mathbf{N} \times \mathbf{N}$, hoặc một tập con của $\mathbf{N} \times \mathbf{N}$, được gọi là một *dãy kép*. Một dãy kép được lập chỉ số bởi $\mathbf{N} \times \mathbf{N}$ được viết $(x_{m,n})$, hoặc đơn giản hơn $(x_{mn})$ nếu không có nguy cơ nhầm lẫn. Tương tự đối với các dãy có nhiều hơn hai chỉ số.

Hai dãy $(x_n)$, $(y_n)$ được gọi là *chỉ khác nhau về thứ tự các số hạng* nếu tồn tại một phép hoán vị $f$ của tập chỉ số sao cho $y_n=x_{f(n)}$ với mọi $n$.

Với mỗi họ các phần tử $(x_\iota)_{\iota\in I}$ có tập chỉ số $I$ là vô hạn đếm được, ta có thể gắn với nó một dãy vô hạn như sau: tồn tại một song ánh $n\to f(n)$ từ $\mathbf{N}$ lên I; đặt $y_n=x_{f(n)}$, dãy $(y_n)$ được gọi là thu được bằng cách *xếp họ* $(x_\iota)$ theo *thứ tự xác định bởi f*. Do đó, các dãy tương ứng với hai song ánh phân biệt từ $\mathbf{N}$ lên I chỉ khác nhau về thứ tự các số hạng.

Thực hiện tương tự khi $I$ là *hữu hạn*, ta thu được một *dãy hữu hạn* liên kết với họ $(x_\iota)$.

9. Hợp, giao và tích của một họ $(X_\iota)_{\iota\in I}$ các tập con của một tập hợp $E$ được gọi là *đếm được* nếu $I$ là một tập hợp *đếm được*, *hữu hạn* nếu $I$ hữu hạn.

Nếu $I$ là *đếm được*, và nếu lũy thừa của $X_\iota$ *nhỏ hơn* một lực lượng vô hạn $\alpha$ đã cho với mọi $\iota\in I$, thì lũy thừa của hợp $\bigcup_\iota X_\iota$ *nhỏ hơn* $\alpha$. Nếu hơn nữa ít nhất một trong các $X_\iota$ có lũy thừa $\alpha$, thì $\bigcup_\iota X_\iota$ có lũy thừa $\alpha$. Đặc biệt, mọi hợp đếm được của các tập hợp có lũy thừa $\alpha$ cũng có lũy thừa $\alpha$; mọi hợp đếm được của các tập hợp đếm được đều là một tập hợp đếm được.

[^1]: Trong lý thuyết tập hợp hình thức hóa (xem Chương III, § 3), ta định nghĩa khái niệm *lực lượng* của một tập hợp, mà ta cũng gọi (do lạm dụng ngôn ngữ) là *lũy thừa* của tập hợp. Tuy nhiên, sự lạm dụng ngôn ngữ này không gây ra bất kỳ sự nhầm lẫn nào, vì hai tập con của một tập hợp có cùng lũy thừa (theo nghĩa đã định nghĩa ở trên) khi và chỉ khi chúng có cùng lực lượng; tương tự, lũy thừa của một tập con A của một tập hợp E nhỏ hơn lũy thừa của một tập con B của một tập hợp F (no. 3) khi và chỉ khi lực lượng của A nhỏ hơn lực lượng của B; và cuối cùng, nếu lũy thừa của A là tổng (no. 5) của các lũy thừa của một họ $(A_\iota)$ các tập con của E, thì lực lượng của A là tổng các lực lượng của các $A_\iota$.
