---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 2
section_title: Functions
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 351-357
pdf_pages: 0356-0362
extraction: ocr
statements: 0
exercises: 0
content_sha256: 5dc426189435aad591d18aa41a0d37e85f43ec180a86a05bca215990e1e9c29d
translated_from: content/en/ens/ER/02_s2_functions.md
source_content_sha256: e080ea464bff6a7c05c7dc505f506fc7d9e94e4178becde6cca23d33e3bb7827
translation_model: gpt-5-6
translation_run: translate-vi-a288c9ba
glossary_version: 34
glossary_terms_sha256: f67ae9538021a82c9d526f21af969ce8b86a9fb21d86da976ec3d4a3b5c262c3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

được ký hiệu bởi $f$, và ta viết $\mathrm{Y} = f(\mathrm{X})$.

Với mọi $f$ và $x$, ta có

$$f(\emptyset) = \emptyset \quad \text{and} \quad f(\{x\}) = \{f(x)\}.$$

Do lạm dụng ngôn ngữ, *giá trị* $f(x)$ của $f$ tại $x$ còn được gọi là *ảnh của* $x$ *qua* $f$.

Nếu $y$ là một phần tử tùy ý của F, tính chất "$y \in f(\mathrm{E})$" có thể được diễn đạt bằng cách nói rằng "$y$ *có dạng* $f(x)$".

Do lạm dụng ngôn ngữ, ảnh $f(\mathrm{E})$ của E qua $f$ đôi khi được gọi là *ảnh của* $f$.

Nếu ta có $f(\mathrm{E}) = \mathrm{F}$, tức là với mọi $y \in$ F tồn tại $x \in$ E sao cho $y = f(x)$, thì $f$ được gọi là một ánh xạ từ E *lên* F, hay một ánh xạ *toàn ánh*, hay một *toàn ánh*.

Cho $x$ là một phần tử tùy ý và X là một tập con bất kỳ của E. Thay vì nói rằng $f(x)$ là giá trị của $f$ tại $x$, và $f(\mathrm{X})$ là ảnh của X qua $f$, đôi khi người ta nói rằng $f$ *biến* (hoặc *ánh xạ*) $x$ thành $f(x)$ và X thành $f(\mathrm{X})$; khi đó $f(x)$ và $f(\mathrm{X})$ lần lượt được gọi là các *ảnh* của $x$ và X qua $f$.

Nếu $f$ là một ánh xạ của E vào chính nó, một tập con X của E được gọi là *ổn định qua* $f$ nếu $f(\mathrm{X}) \subset \mathrm{X}$. Tập con X được gọi là *ổn định* qua một tập hợp các ánh xạ của E vào E nếu X ổn định qua từng ánh xạ trong số đó.

5. Cho $f$ là một ánh xạ của E vào F. Khi đó ta có các mệnh đề sau, trong đó X và Y ký hiệu các tập con tùy ý của E :

(a) Quan hệ $\mathrm{X} \subset \mathrm{Y}$ kéo theo $f(\mathrm{X}) \subset f(\mathrm{Y})$.

(b) Tính chất $\mathrm{X} \neq \emptyset$ tương đương với $f(\mathrm{X}) \neq \emptyset$.

(c) Với mọi X, Y ta có

$$(11) \qquad f(\mathrm{X} \cup \mathrm{Y}) = f(\mathrm{X}) \cup f(\mathrm{Y}),$$

$$(12) \qquad f(\mathrm{X} \cap \mathrm{Y}) \subset f(\mathrm{X}) \cap f(\mathrm{Y}).$$

6. Cho $f$ là một ánh xạ của E vào F, và Y là một tập con tùy ý của F. *Ảnh ngược của* Y *qua* $f$ là tập con X của E gồm tất cả các phần tử $x$ có tính chất $f(x) \in \mathrm{Y}$.

Điều này xác định một quan hệ giữa X và Y có tính phiếm hàm theo X và do đó xác định một ánh xạ của $\mathfrak{P}(F)$ vào $\mathfrak{P}(E)$, được gọi là *mở rộng ngược của f tới các tập hợp các tập con*, và ký hiệu là $\overset{-1}{f}$; do đó ta viết $X = \overset{-1}{f}(Y)$.

Đặc biệt, nếu $y$ là một phần tử của F, thì $\overset{-1}{f}(\{y\})$ là tập hợp tất cả các $x \in E$ sao cho $f(x) = y$. Các quan hệ "$f(x) = y$" và "$x \in \overset{-1}{f}(\{y\})$" là tương đương. Do lạm dụng ngôn ngữ, ta thường viết $\overset{-1}{f}(y)$ thay cho $\overset{-1}{f}(\{y\})$.

*Dấu vết* $X_A$ của một tập con X của E trên một tập con A đã cho là ảnh ngược của X qua ánh xạ chính tắc của A vào E (no. 3).

7. Cho $f$ là một ánh xạ của E vào F. Khi đó ta có các mệnh đề sau, trong đó X và Y ký hiệu các tập con tùy ý của F :

(a) Quan hệ $X \subset Y$ kéo theo $\overset{-1}{f}(X) \subset \overset{-1}{f}(Y)$.

(b) Với mọi X, Y, ta có

(13) $$\overset{-1}{f}(X \cup Y) = \overset{-1}{f}(X) \cup \overset{-1}{f}(Y),$$

(14) $$\overset{-1}{f}(X \cap Y) = \overset{-1}{f}(X) \cap \overset{-1}{f}(Y),$$

(15) $$\overset{-1}{f}(\complement X) = \complement \overset{-1}{f}(X).$$

Chú ý sự khác biệt giữa các công thức (12) và (14); (14) sẽ không đúng với mọi X và Y nếu ta thay $\overset{-1}{f}$ bằng một ánh xạ tùy ý của F vào E. Một lần nữa, không có điều tương tự như (15) đối với mở rộng của một ánh xạ tùy ý.

Hơn nữa, ta có $\overset{-1}{f}(\emptyset) = \emptyset$; nhưng cũng có thể có $\overset{-1}{f}(X) = \emptyset$ với một tập con X khác rỗng của F. Để $X \neq \emptyset$ kéo theo $\overset{-1}{f}(X) \neq \emptyset$, điều kiện cần và đủ là $f$ phải là một ánh xạ của E *lên* F.

8. Nếu một ánh xạ $f$ của E vào F có tính chất là với mọi $y \in F$ tồn tại *nhiều nhất một* $x \in E$ sao cho $y = f(x)$ (nói cách khác, tập hợp $\overset{-1}{f}(y)$ hoặc là rỗng hoặc gồm một phần tử duy nhất), thì $f$ được gọi là một ánh xạ *một-một* của E vào F, hay một ánh xạ *đơn ánh*, hay một *đơn ánh*. Khi đó, với mọi tập con X, Y của E,

(16) $$f(X \cap Y) = f(X) \cap f(Y).$$

9. Nếu một ánh xạ $f$ của E vào F có tính chất là với mọi $y \in F$ *tồn tại đúng một* $x \in E$ sao cho $y = f(x)$ (nói cách khác, $\overset{-1}{f}(y)$ gồm một phần tử duy nhất), thì $f$ được gọi là một ánh xạ *một-một* của E *lên* F, hay một ánh xạ *song ánh*, hay một *song ánh*. Một ánh xạ như vậy có thể được đặc trưng là vừa là một ánh xạ của E lên F vừa là một ánh xạ *một-một* của E vào F.

Nếu $f$ là một ánh xạ một-một của E lên F, quan hệ $y=f(x)$ không chỉ là phiếm hàm theo $y$, mà còn là *phiếm hàm theo $x$. Với tư cách là một quan hệ phiếm hàm theo $x$, nó xác định một ánh xạ một-một của F lên E, được gọi là *nghịch đảo* của ánh xạ $f$.

Chú ý rằng *mở rộng của nghịch đảo của $f$ chính là nghịch đảo của mở rộng của $f$.

Cho $g$ là nghịch đảo của $f$. Khi đó các quan hệ “$y=f(x)$” và “$x=g(y)$” là *tương đương*. Nghịch đảo của $g$ là $f$. Nếu $f$ là một ánh xạ một-một của E lên F, ta không chỉ có quan hệ (16) mà còn, với mọi tập con X của E,

$$f(\mathrm{C}X)=\mathrm{C}f(X).$$

Hơn nữa, mở rộng của $f$ là một ánh xạ một-một của $\wp(E)$ lên $\wp(F)$.

Một ánh xạ một-một của E lên F, cùng với ánh xạ nghịch đảo của nó, được nói là *thực hiện một sự tương ứng một-một giữa E và F*; một cách tương đương, ta nói rằng E và F *được đặt vào sự tương ứng một-một bởi các ánh xạ này*.

Một ánh xạ một-một của một tập hợp E lên chính nó được gọi là một *phép hoán vị* của E. Ánh xạ đồng nhất là một phép hoán vị. Nếu một phép hoán vị trùng với nghịch đảo của nó, nó được gọi là *involutory*; chẳng hạn, ánh xạ $X\rightarrow \mathrm{C}X$ của $\wp(E)$ lên chính nó là involutory.

10. Trong các mệnh đề sau đây, X ký hiệu một tập con tùy ý của E, và Y một tập con tùy ý của F:

(a) Nếu $f$ là một ánh xạ của E *vào* F, ta có

(17)
$$f^{-1}(Y)=f^{-1}(Y\cap f(E)),$$

(18)
$$X\subset f^{-1}(f(X)),$$

(19)
$$f(f^{-1}(Y))\subset Y.$$

(b) Các tính chất “với mọi Y, $f(f^{-1}(Y))=Y$” và “$f$ là một ánh xạ của E lên F” là *tương đương*.

(c) Các tính chất “với mọi X, $f^{-1}(f(X))=X$” và “$f$ là một ánh xạ *một-một* của E vào F” là *tương đương*.

(d) Các tính chất “với mọi X và Y,

$$f^{-1}(f(X))=X\qquad\text{và}\qquad f(f^{-1}(Y))=Y$$

và “$f$ là một ánh xạ *một-một* của E lên F” là *tương đương*.

11. Cho E, F, G là ba tập hợp, có thể phân biệt hoặc không phân biệt. Cho $f$ là một ánh xạ từ E vào F, và $g$ là một ánh xạ từ F vào G. Ánh xạ từ E vào G mà giá trị tại mỗi phần tử $x$ của E là $g(f(x))$ được gọi là *hợp thành* của $g$ và $f$, và được ký hiệu bởi $g \circ f$, hoặc đơn giản là $gf$ nếu không có nguy cơ gây nhầm lẫn.

Đẳng thức $h = g \circ f$ được gọi là một *phân tích* của $h$.

Chú ý rằng, nếu G phân biệt với E, thì ta không thể nói đến hợp thành của $f$ và $g$ (theo thứ tự đó), và ký hiệu $f \circ g$ không có nghĩa. Nếu G đồng nhất với E, thì $f \circ g$ và $g \circ f$ không phải là các phần tử của cùng một tập hợp trừ khi F cũng đồng nhất với E; và ngay cả khi điều này xảy ra, thông thường ta có $f \circ g \neq g \circ f$. Do đó, *thứ tự* hợp thành của $f$ và $g$ là cốt yếu.

Cho $\varphi$ là hợp thành của $g$ và $f$, cho X là một tập con bất kỳ của E, và cho Z là một tập con bất kỳ của G. Khi đó ta có

(20) $$\varphi(\mathrm{X}) = g(f(\mathrm{X})),$$
(21) $$\overset{-1}{\varphi}(\mathrm{Z}) = \overset{-1}{f}(\overset{-1}{g}(\mathrm{Z})).$$

Nếu $f$ là một ánh xạ *một-một* từ E *lên* F, và nếu $g$ là một ánh xạ *một-một* từ F *lên* G, thì $g \circ f$ là một ánh xạ *một-một* từ E *lên* G.

Cho $h$ là một ánh xạ từ G vào một tập hợp H. Khi đó ta có

$$h \circ (g \circ f) = (h \circ g) \circ f;$$

ánh xạ này từ E vào H được viết là $h \circ g \circ f$, và được gọi là *hợp thành* của ba ánh xạ $h$, $g$, $f$ theo thứ tự này. Hợp thành của nhiều hơn ba ánh xạ được định nghĩa tương tự.

Nếu $f$ là một ánh xạ từ E vào chính E, thì các *lần lặp* của $f$ được định nghĩa là các ánh xạ $f^n$ ($n$ là một số nguyên $\geqslant 1$) từ E vào chính E, được định nghĩa bằng quy nạp theo $n$ nhờ các hệ thức $f^1 = f$, $f^n = f^{n-1} \circ f$; $f^n$ được gọi là *lần lặp thứ n* của $f$. Ta có $f^{m+n} = f^m \circ f^n$.

12. Nói chung, hợp thành $\overset{-1}{f} \circ f$ của mở rộng nghịch đảo và mở rộng của một ánh xạ $f$ không phải là ánh xạ đồng nhất của $\mathfrak{P}(\mathrm{E})$ lên chính nó. Tương tự, $f \circ \overset{-1}{f}$ thường không phải là ánh xạ đồng nhất của $\mathfrak{P}(\mathrm{E})$ lên chính nó. Hai điều kiện này đồng thời được thỏa mãn chỉ khi $f$ là một *song ánh* từ E lên F.

Nếu $f$ là một song ánh từ E lên F, và nếu $g$ ký hiệu ánh xạ nghịch đảo của $f$, thì các hợp thành $g \circ f$ và $f \circ g$ lần lượt là ánh xạ đồng nhất của E lên E và ánh xạ đồng nhất của F lên F.

Ngược lại, nếu $f$ là một ánh xạ từ E vào F, và $g$ là một ánh xạ từ F vào E, sao cho $g \circ f$ là một phép hoán vị của E và $f \circ g$ là một phép hoán vị của F, thì $f$ là một song ánh từ E lên F và $g$ là một song ánh từ F lên E.

Hơn nữa, nếu $g\circ f$ là ánh xạ đồng nhất của E lên chính nó, thì $g$ là ánh xạ nghịch đảo của $f$.

13. Cho $f$ là một ánh xạ từ E vào F, và cho A là một tập con bất kỳ của E. Ánh xạ $f_A$ từ A vào F mà giá trị tại mọi phần tử $x$ của A là $f(x)$ được gọi là *hạn chế của $f$ lên tập con A*; nó chính là hợp thành của $f$ và ánh xạ chính tắc từ A vào E. Nếu hai ánh xạ $f$, $g$ từ E vào F có cùng hạn chế lên A, thì chúng được nói là *trùng nhau (hay coincide)* trên A. Ngược lại, $f$ được gọi là một *mở rộng* của $f_A$ lên E.

14. Một ánh xạ của một tập hợp E *lên* một tập hợp F còn được gọi là một *biểu diễn tham số* của F *bằng* E; khi đó E được gọi là *tập hợp tham số* của biểu diễn này, và các phần tử của E được gọi là *các tham số*.

Một *họ các phần tử* của một tập hợp F theo định nghĩa là một tập con của F được trang bị một biểu diễn tham số; nói cách khác, cho một họ các phần tử của F tương đương với cho một ánh xạ từ một tập hợp nào đó E vào F. Ảnh của E qua ánh xạ này được gọi là *tập hợp các phần tử của họ*. Chú ý rằng hai họ các phần tử phân biệt của F có thể có cùng một tập con của F làm tập hợp các phần tử của chúng.

Với mỗi tập con A của một tập hợp F, ta luôn có thể liên kết một họ các phần tử có tập hợp các phần tử là A. Chỉ cần xét họ được xác định bởi *ánh xạ chính tắc* từ A vào F.

Một họ các phần tử của F, được xác định bởi một ánh xạ $\iota\mapsto x_\iota$ từ một tập hợp I vào F, được ký hiệu là $(x_\iota)_{\iota\in I}$, hoặc đơn giản là $(x_\iota)$ nếu không thể có sự nhầm lẫn nào về tập hợp chỉ số.

Nếu J là một tập con của I, họ $(x_\iota)_{\iota\in J}$ được gọi là *họ con* tương ứng với J của họ $(x_\iota)_{\iota\in I}$; nó được xác định bởi hạn chế trên J của ánh xạ $\iota\mapsto x_\iota$.

Hạn chế trên J của ánh xạ $\iota\mapsto x_\iota$.
