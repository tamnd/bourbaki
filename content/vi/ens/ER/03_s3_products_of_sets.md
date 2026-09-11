---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 3
section_title: Products of sets
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 357-362
pdf_pages: 0362-0367
extraction: ocr
statements: 0
exercises: 0
content_sha256: 7bcc3de548f9506f888135256d7c30cca48d168e03caecb58a5f20209706493a
translated_from: content/en/ens/ER/03_s3_products_of_sets.md
source_content_sha256: 911c36b076fa6fa142fe625cbd3bb6de17b251c6493dfaffdaf76058fad82252
translation_model: gpt-5-6
translation_run: translate-vi-85dc4e6a
glossary_version: 34
glossary_terms_sha256: 5fc57d9a55efdad18a831a0c9318a77f62aeb1336cf137ac74cde95412060904
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. TÍCH CÁC TẬP HỢP

1. Cho E, F là hai tập hợp, có thể phân biệt hoặc không. Các *cặp có thứ tự* $(x,y)$, trong đó phần tử thứ nhất $x$ là một phần tử tùy ý của E và phần tử thứ hai $y$ là một phần tử tùy ý của F, là các phần tử của một tập hợp mới, gọi là *tích của E với F*, và ký hiệu là $E\times F$; E và F được gọi là các *thừa số* của $E\times F$. Hai cặp có thứ tự được coi là đồng nhất khi và chỉ khi chúng có cùng phần tử thứ nhất và cùng phần tử thứ hai; nói cách khác, quan hệ “$(x,y)=(x',y')$” tương đương với quan hệ “$x=x'$ và $y=y'$”. Nếu $z$ là một phần tử tùy ý của $E\times F$, quan hệ “$x$ là phần tử thứ nhất của cặp có thứ tự $z$” là một quan hệ phiếm hàm theo $x$; nó xác định một ánh xạ của $E\times F$ lên E, gọi là *hàm tọa độ thứ nhất*, hay *phép chiếu thứ nhất*, và ký hiệu là $\operatorname{pr}_1$. Thay vì nói “$x$ là phần tử thứ nhất của cặp có thứ tự $z$”, ta cũng nói “$x$ là tọa độ thứ nhất (hay phép chiếu thứ nhất) của $z$" hoặc "$x = \mathrm{pr}_1 z$". Tương tự, ta định nghĩa *hàm tọa độ thứ hai*, hay *phép chiếu thứ hai*, là một ánh xạ của $\mathrm{E} \times \mathrm{F}$ *lên* $\mathrm{F}$, ký hiệu là $\mathrm{pr}_2$.

Quan hệ "$x = \mathrm{pr}_1 z$ và $y = \mathrm{pr}_2 z$" tương đương với "$z = (x, y)$".

Mở rộng của hàm $\mathrm{pr}_1$ lên các tập hợp của các tập con được ký hiệu bởi cùng một ký hiệu, theo các quy ước tổng quát, và lại được gọi là *phép chiếu thứ nhất* (ở đây ta không dùng số hạng "tọa độ"); tương tự đối với mở rộng của phép chiếu thứ hai.

2. Một quan hệ R giữa một phần tử tùy ý $x$ của E và một phần tử tùy ý $y$ của F là một tính chất của cặp $(x, y)$, và do đó định nghĩa một tập con của tích $\mathrm{E} \times \mathrm{F}$, gọi là *đồ thị* của R. Ngược lại, mọi tập con A của $\mathrm{E} \times \mathrm{F}$ đều là đồ thị của quan hệ $(x, y) \in \mathrm{A}$ giữa $x$ và $y$.

Cho A là một tập con của E và B là một tập con của F. Ta ký hiệu $\mathrm{A} \times \mathrm{B}$ là tập con của $\mathrm{E} \times \mathrm{F}$ được định nghĩa bởi quan hệ "$x \in \mathrm{A}$ và $y \in \mathrm{B}$" giữa $x$ và $y$.

3. Trong các mệnh đề sau, X và X$'$ ký hiệu các tập con tùy ý của E, Y và Y$'$ các tập con tùy ý của F, và Z một tập con tùy ý của $\mathrm{E} \times \mathrm{F}$.

(a) Quan hệ "$\mathrm{X} \times \mathrm{Y} = \emptyset$" *tương đương* với "$\mathrm{X} = \emptyset$ hoặc $\mathrm{Y} = \emptyset$".

(b) Nếu $\mathrm{X} \times \mathrm{Y} \neq \emptyset$, quan hệ "$\mathrm{X} \times \mathrm{Y} \subset \mathrm{X}' \times \mathrm{Y}'$" *tương đương* với "$\mathrm{X} \subset \mathrm{X}'$ và $\mathrm{Y} \subset \mathrm{Y}'$".

(c) Với mọi X, X$'$, Y ta có

$$(\mathrm{X} \times \mathrm{Y}) \cup (\mathrm{X}' \times \mathrm{Y}) = (\mathrm{X} \cup \mathrm{X}') \times \mathrm{Y}. \tag{22}$$

(d) Với mọi X, X$'$, Y, Y$'$ ta có

$$(\mathrm{X} \times \mathrm{Y}) \cap (\mathrm{X}' \times \mathrm{Y}') = (\mathrm{X} \cap \mathrm{X}') \times (\mathrm{Y} \cap \mathrm{Y}'). \tag{23}$$

(e) Với mọi X, Y ta có

$$\overset{-1}{\mathrm{pr}_1}(\mathrm{X}) = \mathrm{X} \times \mathrm{F}, \qquad \overset{-1}{\mathrm{pr}_2}(\mathrm{Y}) = \mathrm{E} \times \mathrm{Y}. \tag{24}$$

(f) Nếu $\mathrm{Y} \neq \emptyset$, thì với mọi X ta có

$$\mathrm{pr}_1(\mathrm{X} \times \mathrm{Y}) = \mathrm{X}. \tag{25}$$

(g) Với mọi Z ta có

$$\mathrm{Z} \subset \mathrm{pr}_1(\mathrm{Z}) \times \mathrm{pr}_2(\mathrm{Z}). \tag{26}$$

(h) Cho $a$ là một phần tử của E. Khi đó ánh xạ $(a, y) \rightarrow y$ của tập hợp $\{a\} \times \mathrm{F}$ *lên* F (nghĩa là, hạn chế của $\mathrm{pr}_2$ lên tập con $\{a\} \times \mathrm{F}$) là *một-một*.

4. Ánh xạ

(27) $$(x, y) \to (y, x)$$

là một ánh xạ *một-một* của $\mathrm{E} \times \mathrm{F}$ *lên* $\mathrm{F} \times \mathrm{E}$, và được gọi là *chính tắc*. Khi E và F là cùng một tập hợp, ánh xạ (27) được gọi là *đối xứng chính tắc*; khi đó nó là *involutory*. Các phần tử $(x, y)$ của $\mathrm{E} \times \mathrm{E}$ được giữ cố định bởi đối xứng này là những phần tử có tính chất $x = y$; tập hợp $\Delta$ gồm các phần tử này được gọi là *đường chéo* của $\mathrm{E} \times \mathrm{E}$. Ánh xạ $x \to (x, x)$ là một *song ánh* của E lên $\Delta$, được gọi là *ánh xạ đường chéo* của E vào $\mathrm{E} \times \mathrm{E}$.

Nếu Z là một tập con bất kỳ của $\mathrm{E} \times \mathrm{F}$, ảnh của Z qua ánh xạ chính tắc của $\mathrm{E} \times \mathrm{F}$ lên $\mathrm{F} \times \mathrm{E}$ được ký hiệu bởi $\overset{-1}{\mathrm{Z}}$. Nếu X là một tập con bất kỳ của E và Y là một tập con bất kỳ của F, thì

$$\overset{-1}{\overgroup{\mathrm{X} \times \mathrm{Y}}} = \mathrm{Y} \times \mathrm{X}.$$

Nếu một quan hệ R giữa $x$ và $y$, được xét như một tính chất của cặp có thứ tự $(x, y)$, xác định một tập con A của $\mathrm{E} \times \mathrm{F}$, thì cùng quan hệ đó, được xét như một tính chất của cặp $(y, x)$, xác định tập con $\overset{-1}{\mathrm{A}}$ của $\mathrm{F} \times \mathrm{E}$. R tương đương với mỗi quan hệ $(x, y) \in \mathrm{A}$, $(y, x) \in \overset{-1}{\mathrm{A}}$. Nếu E và F là cùng một tập hợp, quan hệ R và tập con tương ứng A được gọi là *đối xứng* khi $\mathrm{A} = \overset{-1}{\mathrm{A}}$. Đường chéo $\Delta$ (được xác định bởi quan hệ đẳng thức) là đối xứng. Nếu Z là một tập con bất kỳ của $\mathrm{E} \times \mathrm{E}$, thì $\mathrm{Z} \cup \overset{-1}{\mathrm{Z}}$ và $\mathrm{Z} \cap \overset{-1}{\mathrm{Z}}$ là đối xứng.

5. Cho A là một tập con của một tập hợp E, và cho $f$ là một ánh xạ của A vào một tập hợp F. Quan hệ "$x \in \mathrm{A}$ and $y = f(x)$" giữa một phần tử bất kỳ $x$ của E và một phần tử bất kỳ $y$ của F xác định một tập con của $\mathrm{E} \times \mathrm{F}$ được gọi là *đồ thị* của hàm $f$. Nếu B là một tập con của E chứa A, và nếu $g$ là một *mở rộng* (§ 2, no. 13) của $f$ lên B, thì đồ thị của $f$ được *chứa* trong đồ thị của $g$.

Ngược lại, cho C là một tập con của $\mathrm{E} \times \mathrm{F}$ sao cho, với mỗi $x \in \mathrm{E}$, tồn tại nhiều nhất một $y \in \mathrm{F}$ sao cho $(x, y) \in \mathrm{C}$. Khi đó quan hệ $(x, y) \in \mathrm{C}$ giữa một phần tử bất kỳ $x$ *của tập hợp* $\mathrm{pr}_1(\mathrm{C})$ và một phần tử bất kỳ $y$ của F là một quan hệ phiếm hàm theo y và xác định một ánh xạ của $\mathrm{pr}_1(\mathrm{C})$ vào F mà đồ thị là C.

Tập hợp các tập con C của $\mathrm{E} \times \mathrm{F}$ có tính chất "với mọi $x \in \mathrm{E}$ có nhiều nhất một $y \in \mathrm{F}$ sao cho $(x, y) \in \mathrm{C}$" (một tập hợp là tập con của $\mathfrak{P}(\mathrm{E} \times \mathrm{F})$) do đó có thể được đặt vào một sự tương ứng song ánh với *tập hợp các ánh xạ từ các tập con của* E *vào* F.

Cho $f$ là một ánh xạ đơn ánh từ E vào F, và cho $g$ là ánh xạ nghịch đảo của $f$ được xét như một song ánh từ E lên $f(\mathrm{E})$. Nếu C là đồ thị của $f$, thì đồ thị của $g$ là $\overset{-1}{\mathrm{C}}$.

6. Nếu $f$ là một ánh xạ từ E vào F, và C là đồ thị của nó trong E $\times$ F, quan hệ "$y = f(x)$" tương đương với "$(x, y) \in \mathrm{C}$". Quan hệ "$y \in f(\mathrm{X})$" tương đương với "tồn tại $x$ sao cho $x \in \mathrm{X}$ và $(x,\ y) \in \mathrm{C}$".

Bây giờ cho K là *một* tập con bất kỳ của E $\times$ F, và cho X là một tập con bất kỳ của E. K(X) ký hiệu tập con của F gồm tất cả các phần tử $y$ thỏa mãn quan hệ "tồn tại $x$ sao cho $x \in \mathrm{X}$ và $(x, y) \in \mathrm{K}$"; do đó quan hệ này tương đương với "$y \in \mathrm{K}(\mathrm{X})$". Ánh xạ $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ của $\mathfrak{P}(\mathrm{E})$ vào $\mathfrak{P}(\mathrm{F})$ được gọi là *được xác định bởi tập con* K của E $\times$ F. Chú ý rằng K(X) là phép chiếu thứ hai của tập hợp $\mathrm{K} \cap (\mathrm{X} \times \mathrm{F})$. Nếu K là đồ thị của một ánh xạ $f$ từ E vào F, thì ánh xạ $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ là mở rộng chính tắc của $f$ lên các tập hợp các tập con.

7. Nếu $x$ là một phần tử tổng quát của E, thì $x \rightarrow \mathrm{K}(\{x\})$ là một ánh xạ từ E vào $\mathfrak{P}(\mathrm{F})$ mà giá trị $\mathrm{K}(\{x\})$ (cũng được ký hiệu bởi $\mathrm{K}(x)$, do lạm dụng ngôn ngữ) được gọi là *tiết diện của* K *tại* $x$. Quan hệ $(x,\ y) \in \mathrm{K}$ tương đương với $y \in \mathrm{K}(x)$.

Ngược lại, *mọi* ánh xạ $x \rightarrow \Phi(x)$ từ E vào $\mathfrak{P}(\mathrm{F})$ đều có thể thu được theo cách này; vì quan hệ $y \in \Phi(x)$ xác định một tập con K của E $\times$ F, và $\Phi(x)$ chính xác là tiết diện của K tại $x$. Tập hợp $\mathfrak{P}(\mathrm{E} \times \mathrm{F})$ và tập hợp các ánh xạ từ E vào $\mathfrak{P}(\mathrm{F})$ do đó có một sự tương ứng song ánh.

8. Mọi ánh xạ $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ được xác định bởi một tập con K của E $\times$ F đều có các tính chất sau, tổng quát hóa các tính chất của mở rộng chính tắc của một ánh xạ từ E vào F (§2, nos. 4 và 5) :
(a)  $\mathrm{K}(\emptyset) = \emptyset$.
(b)  "$\mathrm{X} \subset \mathrm{Y}$" kéo theo "$\mathrm{K}(\mathrm{X}) \subset \mathrm{K}(\mathrm{Y})$".
(c)  Với mọi X, Y, ta có

(28) $$\mathrm{K}(\mathrm{X} \cup \mathrm{Y}) = \mathrm{K}(\mathrm{X}) \cup \mathrm{K}(\mathrm{Y}),$$
(29) $$\mathrm{K}(\mathrm{X} \cap \mathrm{Y}) \subset \mathrm{K}(\mathrm{X}) \cap \mathrm{K}(\mathrm{Y}).$$

Nếu K và K$'$ là hai tập con của E $\times$ F sao cho $\mathrm{K} \subset \mathrm{K}'$, thì ta có $\mathrm{K}(\mathrm{X}) \subset \mathrm{K}'(\mathrm{X})$ với mọi $\mathrm{X} \subset \mathrm{E}$; đặc biệt, $\mathrm{K}(x) \subset \mathrm{K}'(x)$ với mọi $x \in \mathrm{E}$. Ngược lại, nếu $\mathrm{K}(x) \subset \mathrm{K}'(x)$ với mọi $x \in \mathrm{E}$, thì $\mathrm{K} \subset \mathrm{K}'$.

9. Một quan hệ giữa một phần tử tổng quát của E và một phần tử tổng quát của F xác định một tập con K của E $\times$ F và một tập con $\overset{-1}{\mathrm{K}}$ của F $\times$ E, và do đó một ánh xạ $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ của $\mathfrak{P}(\mathrm{E})$ vào $\mathfrak{P}(\mathrm{F})$ và một ánh xạ $\mathrm{Y} \rightarrow \overset{-1}{\mathrm{K}}(\mathrm{Y})$ của $\mathfrak{P}(\mathrm{F})$ vào $\mathfrak{P}(\mathrm{E})$.

Nếu K là đồ thị của một ánh xạ $f$ của E vào F, thì ánh xạ $\mathrm{Y} \rightarrow \overset{-1}{\mathrm{K}}(\mathrm{Y})$ là mở rộng nghịch đảo của $f$.

Cần lưu ý rằng các quan hệ (18) và (19) không tổng quát hóa thành các ánh xạ $X \to K(X)$ và $Y \to \overset{-1}{K}(Y)$, khi $K$ là một tập con tùy ý của $E \times F$.

10. Cho E, F, G là ba tập hợp, có thể phân biệt hoặc không, cho A là một tập con của $E \times F$ và cho B là một tập con của $F \times G$. Khi đó các phần tử $(x, z)$ của $E \times G$ có tính chất "tồn tại $y \in F$ sao cho $(x, y) \in A$ và $(y, z) \in B$" tạo thành một tập con của $E \times G$, được gọi là *hợp thành của* B *và* A, và được ký hiệu bởi $B \circ A$, hoặc đơn giản là BA khi không có nguy cơ nhầm lẫn. Ở đây một lần nữa, thứ tự của hợp thành là cốt yếu.

¶ Ánh xạ $X \to BA(X)$ của $\mathfrak{P}(E)$ vào $\mathfrak{P}(G)$ là hợp thành của $Y \to B(Y)$ và $X \to A(X)$; nói cách khác, với mọi $X \subset E$ ta có

$$(30) \qquad BA(X) = B(A(X)).$$

Cho H là một tập hợp khác, không nhất thiết phân biệt với E, F, G, và cho C là một tập con của $G \times H$. Khi đó ta có $C \circ (B \circ A) = (C \circ B) \circ A$; tập hợp này cũng được ký hiệu bởi $C \circ B \circ A$ (hoặc đơn giản là CBA) và được gọi là *hợp thành* của C, B, A lấy theo thứ tự này.

Cho $f$ là một ánh xạ của E vào F, và cho $g$ là một ánh xạ của F vào G. Nếu A (tương ứng B) là đồ thị của $f$ (tương ứng $g$), thì hợp thành BA là đồ thị của ánh xạ hợp thành $g \circ f$.

11. Ta có

$$(31) \qquad \overset{-1}{\overbrace{B \circ A}} = \overset{-1}{A} \circ \overset{-1}{B}.$$

Cho A, A′ là hai tập con của $E \times F$, và cho B, B′ là hai tập con của $F \times G$. Khi đó quan hệ

$$\text{“}A \subset A' \text{ và } B \subset B'\text{”} \qquad \text{suy ra} \qquad \text{“}B \circ A \subset B' \circ A'\text{”}.$$

Cho A là một tập con của $E \times F$, $\Delta$ là đường chéo của $E \times E$, và $\Delta'$ là đường chéo của $F \times F$. Khi đó ta có

$$(32) \qquad A \circ \Delta = \Delta' \circ A = A.$$

12. Cho E, F, G là ba tập hợp, có thể phân biệt hoặc không phân biệt. *Tích* của chúng $E \times F \times G$ là tập hợp các *bộ ba có thứ tự* $(x, y, z)$, trong đó $x \in E$, $y \in F$, và $z \in G$, quan hệ "$(x, y, z) = (x', y', z')$" là tương đương với "$x = x'$ và $y = y'$ và $z = z'$". Ba ánh xạ $(x, y, z) \to x$, $(x, y, z) \to y$, $(x, y, z) \to z$ của $E \times F \times G$ lên E, F, G tương ứng được gọi là các *hàm tọa độ thứ nhất, thứ hai,* và *thứ ba* (hay các *phép chiếu*); tương tự, chẳng hạn, *phép chiếu với các chỉ số* 1, 2 là ánh xạ

$$
(x, y, z) \mapsto (x, y)
$$

của $E \times F \times G$ lên $E \times F$, và được ký hiệu bởi $\mathrm{pr}_{1,2}$.

Các định nghĩa và mệnh đề của các số 2, 3, và 4 dễ dàng tổng quát hóa cho tích của ba tập hợp.

Hơn nữa, thay vì xét tích $E \times F \times G$ của ba tập hợp, ta có thể tương đương xét tích $(E \times F) \times G$, thu được bằng một phép áp dụng kép của phép toán tạo thành tích của hai tập hợp. Thật vậy, $(x, y, z) \mapsto ((x, y), z)$ là một ánh xạ một-một của $E \times F \times G$ lên $(E \times F) \times G$, được gọi là *chính tắc*. Tương tự ta định nghĩa các ánh xạ một-một của $E \times F \times G$ lên tập hợp $E \times (F \times G)$, và lên tất cả các tập hợp thu được từ $E \times F \times G$, $(E \times F) \times G$, và $E \times (F \times G)$ bằng cách hoán vị ba chữ cái E, F, G.

Có các định nghĩa và tính chất tương tự đối với tích của nhiều hơn ba tập hợp.

13. Nếu một hàm $f$, lấy các giá trị của nó trong một tập hợp bất kỳ $E'$, được xác định trên một tích của ba tập hợp $E$, $F$, $G$, thì nó được gọi là một hàm của *ba biến*, mỗi biến chạy qua một trong các tập hợp $E$, $F$, $G$. Giá trị của $f$ tại phần tử $(x, y, z)$ của $E \times F \times G$ được ký hiệu bởi $f(x, y, z)$.

Cho $a$ là một phần tử bất kỳ của $E$. Khi đó $(y, z) \mapsto f(a, y, z)$ là một ánh xạ của $F \times G$ vào $E'$, được gọi là một *ánh xạ riêng phần (hay hàm) được xác định bởi $f$ tương ứng với giá trị $a$ của $x$; nó cũng là ánh xạ hợp của $f$ và ánh xạ $(y, z) \mapsto (a, y, z)$ của $F \times G$ vào $E \times F \times G$.

Tương tự, nếu $b$ là một phần tử của $F$, thì $z \mapsto f(a, b, z)$ là một ánh xạ từ $G$ vào $E'$, được gọi là ánh xạ riêng phần được xác định bởi $f$ tương ứng với các giá trị $a$, $b$ của $x$, $y$.

Ngược lại, cho $g$ là một ánh xạ từ $E$ vào $E'$. Khi đó $(x, y, z) \mapsto g(x)$ là một ánh xạ $h$ từ $E \times F \times G$ vào $E'$ sao cho mọi ánh xạ riêng phần từ $E$ vào $E'$ được xác định bởi $h$, tương ứng với bất kỳ giá trị nào của $y$ và $z$, đều đồng nhất với $g$. Sự kiện này thường được diễn đạt bằng cách nói rằng một hàm của đối số $x$ luôn có thể được xem như một hàm của tất cả các đối số cần được xét tại một thời điểm đã cho và tất nhiên sẽ bao gồm $x$.

14. Cho $f$, $g$, $h$ lần lượt là ba ánh xạ từ $E$ vào $E'$, từ $F$ vào $F'$, từ $G$ vào $G'$. Ánh xạ $(x, y, z) \mapsto (f(x), g(y), h(z))$ từ $E \times F \times G$ vào $E' \times F' \times G'$ được ký hiệu là $f \times g \times h$ và được gọi là *mở rộng của $f$, $g$, $h$ lên các tích*. Nếu cả ba ánh xạ $f$, $g$, $h$ đều đơn ánh (resp. toàn ánh, song ánh), thì $f \times g \times h$ là đơn ánh (resp. toàn ánh, song ánh).

Trong tiểu mục này và tiểu mục trước, chúng ta chỉ xét trường hợp *ba* tập hợp nhằm làm rõ ý tưởng; những xét tương tự đúng với bất kỳ số hữu hạn tập hợp nào.

old đối với bất kỳ số hữu hạn tập hợp nào.
