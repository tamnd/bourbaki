---
book: ac
book_title: Commutative Algebra
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: vi
source: ac-i-vii
pdf_pages: 0017-0020
extraction: ocr
statements: 0
exercises: 0
content_sha256: d8938ce568a339ff49662254f7d57d33db759133b867e0e8d587b1c05313af17
translated_from: content/en/ac/00_introduction.md
source_content_sha256: 76b5a99586b68b13462663dc0c9b880af0d70ce65bdf4d0e0496ed1cda0fd86b
translation_model: gpt-5.4
translation_run: translate-vi-f92dbaee
glossary_version: 34
glossary_terms_sha256: ea70d1bb9c08e99bca006ea204a49e1d773d96b500cecc0da21c474fa424bd0f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## DẪN NHẬP

Các bài toán được khảo sát trong Quyển này đã nảy sinh trong quá trình phát triển của lý thuyết số đại số và (về sau) hình học đại số (x. Ghi chú lịch sử). Từ thế kỷ 19 trở đi, hai lý thuyết này bắt đầu bộc lộ những phép tương tự đáng chú ý; nỗ lực giải các bài toán do chúng đặt ra đã dẫn đến việc tách ra một số ý tưởng tổng quát mà phạm vi áp dụng không bị giới hạn vào các vành số đại số hay các vành hàm đại số; và, như mọi khi, sẽ có lợi nếu xét chúng dưới dạng tổng quát nhất để thấy được ý nghĩa thực sự của chúng và ảnh hưởng qua lại của việc nghiên cứu lĩnh vực này đối với lĩnh vực kia. Về nguyên tắc, các khái niệm được khảo sát trong Quyển này có thể được áp dụng cho mọi vành giao hoán và các môđun trên những vành như vậy; tuy nhiên phải chỉ ra rằng các kết quả thực chất thường chỉ thu được dưới một số giả thiết về *hữu hạn* (những giả thiết này luôn đúng trong các trường hợp cổ điển), chẳng hạn khi giả sử các môđun là sinh hữu hạn hoặc các vành là Noether.

Các khái niệm chủ yếu, giữ vai trò trung tâm trong những chương đầu, là như sau:

**I. Địa phương hóa và toàn cục hóa.** Chẳng hạn, hãy bắt đầu với một hệ phương trình Diophantine:

(*) $$
P_i(x_1, \ldots, x_r) = 0 \quad (1 \leq i \leq n)
$$

trong đó các $P_i$ là những đa thức với hệ số nguyên và ta tìm các nghiệm $(x_i)$ gồm các *số nguyên* hữu tỉ. Có thể bắt đầu tiếp cận bài toán bằng cách tìm các nghiệm gồm các *số hữu tỉ*, điều này dẫn đến việc xét cùng bài toán ấy khi các hệ số của các $P_i$ được coi là những phần tử của *trường phân thức* $\mathbf{Q}$ của $\mathbf{Z}$ và các nghiệm cần tìm nhận giá trị trong $\mathbf{Q}$. Bước thứ hai là xem, với một số nguyên tố $p$ cho trước, có tồn tại các nghiệm hữu tỉ mà mẫu số không chia hết cho $p$ hay không (các nghiệm *nguyên* hiển nhiên thỏa mãn điều kiện này); trong trường hợp này, điều đó có nghĩa là các nghiệm nằm trong vành con $\mathbf{Z}_{(p)}$ của $\mathbf{Q}$ gồm các số hữu tỉ có dạng như vậy, được gọi là *vành địa phương* của $\mathbf{Z}$ tương ứng với số nguyên tố $p$. Rõ ràng việc chuyển từ $\mathbf{Z}$ sang $\mathbf{Q}$ và việc chuyển từ $\mathbf{Z}$ sang $\mathbf{Z}_{(p)}$ có cùng một dạng: trong cả hai trường hợp, các mẫu số duy nhất được phép đều không thuộc về một *iđêan nguyên tố* nào đó (lần lượt là iđêan $(0)$ và iđêan $(p)$). Cùng tên gọi "vành địa phương" cũng xuất hiện trong hình học đại số, ở đó khái niệm này xuất hiện một cách tự nhiên hơn: chẳng hạn với vành $\mathbf{C}[X]$ các đa thức theo một biến với hệ số phức, vành địa phương tương ứng với iđêan nguyên tố $(X - a)$ là vành các phân thức hữu tỉ "chính quy" tại điểm $a$ (nghĩa là không có cực tại điểm đó).

Mọi bài toán Diophantine và, nói chung hơn, mọi bài toán về các A-môđun (A là một vành giao hoán) đều có thể được phân tích thành hai bài toán phụ: ta tìm nghiệm của nó trong các vành địa phương $A_{\mathfrak{p}}$ tương ứng với các iđêan nguyên tố khác nhau $\mathfrak{p}$ của A ("địa phương hóa"), rồi đặt câu hỏi liệu có thể kết luận từ sự tồn tại, với mọi $\mathfrak{p}$, của một nghiệm của bài toán "đã địa phương hóa" rằng tồn tại một nghiệm của bài toán được đặt ra ban đầu hay không ("chuyển từ địa phương sang toàn cục"). Chương II được dành cho việc nghiên cứu quá trình kép này, và ở đó cũng thấy rằng "địa phương hóa" không chỉ liên quan đến các iđêan nguyên tố mà còn có phạm vi rộng hơn.

11. *Completion & local rings*. A local ring A shares with fields the property of having only *one* maximal ideal m. This fact is used to transform, to a certain extent, a problem on A-modules into an analogous problem on *vector spaces* by passing to the quotient ring $A/m$, as this latter is a field. If we return for example to the Diophantine system (*) this idea is none other than the principle of "reduction modulo K", transforming the equations into congruences mod. $p$, which occurred naturally beginning with the very first works in the theory of numbers.

Như vậy, rõ ràng ta không thể hy vọng bằng cách này mà thu được các kết quả đầy đủ cho bài toán ban đầu, và người ta đã sớm nhận ra rằng để thu được thông tin chính xác hơn thì cần phải xét, không chỉ các đồng dư môđun $m$, mà cả các đồng dư "bậc cao hơn" môđun $m^n$, với các số nguyên tùy ý $n > 0$. Do đó, ta thấy rằng $n$ càng lớn thì theo một nghĩa nào đó bài toán ban đầu càng được "xấp xỉ" gần hơn (chẳng hạn trong trường hợp $A = \mathbf{Z}$, lý do là một số nguyên $\neq 0$ không thể chia hết cho *mọi* lũy thừa $p^n$ của một số nguyên tố cho trước $p$; vì thế số này sẽ bộc lộ sự hiện diện của nó trong phép thu gọn mod. $p^n$ miễn là lấy $n$ đủ lớn). Bản dịch toán học của ý tưởng này là xét trên A một *tôpô* vành (x. *Tôpô đại cương*, Chương III, § 6) trong đó các $m^n$ tạo thành một hệ cơ bản các lân cận của 0. Nhưng khi chẳng hạn ta đã giải được hệ đồng dư

$$
\text{P}_i(x_1, \ldots, x_m) \equiv 0 \ (\text{mod. } p^k) \qquad (1 \leq i \leq n)
$$

với *mọi số nguyên* $k > 0$, thì vẫn chưa suy ra được rằng hệ (*) có một nghiệm trong vành địa phương $\mathbf{Z}_{(p)}$; giả thiết trên có thể được hiểu là (*) thừa nhận một nghiệm trong *hoàn thành* $\hat{\mathbf{Z}}_{(p)}$ của vành tôpô $\mathbf{Z}_{(p)}$.

Bài toán ban đầu, do đó đã được làm yếu đi, cuối cùng được chuyển thành bài toán tương tự đối với các vành địa phương kiểu $A/m^n$, những vành này cũng gần với các trường hơn các vành tổng quát, vì chúng có căn lũy linh; trong hình học đại số cổ điển, điều này tương ứng với một khảo sát "vi phân" của bài toán trong lân cận của một điểm đã cho.

Chương III khảo sát một cách tổng quát các áp dụng này của các khái niệm tôpô vào lý thuyết các vành địa phương. Trong Chương VI, một phương diện đặc biệt của vấn đề này được nghiên cứu, một mặt thích nghi với các nghiên cứu chi tiết hơn của hình học đại số, và trên hết với số học của các trường số đại số, trong đó các vành địa phương gặp phải (chẳng hạn $\mathbf{Z}_{(p)}$) thuộc về một lớp đặc biệt đơn giản, lớp các "vành định giá", nơi tính chia hết là một thứ tự toàn phần (xem Đại số, Chương VI, § 1) trên tập hợp các iđêan chính.

Việc nghiên cứu sự chuyển từ một vành A sang một vành địa phương A, hoặc sang một hoàn chỉnh hóa $\hat{A}$, làm sáng tỏ một đặc điểm chung của hai phép toán này, tính chất phẳng của các A-môđun A và $\hat{A}$, điều cho phép, trong số những điều khác, dùng các tích tenxơ của các A-môđun như vậy với các A-môđun tùy ý theo cách phần nào tương tự như đối với các tích tenxơ của các không gian vectơ, nghĩa là không cần mọi sự thận trọng vốn đi kèm với việc sử dụng chúng trong trường hợp tổng quát. Các tính chất liên kết với khái niệm này, cũng áp dụng được cho các môđun trên các vành không giao hoán, là đối tượng nghiên cứu của Chương I.

III. Số nguyên và phân tích iđêan. Việc nghiên cứu tính chia hết trong các trường số đại số ngay từ đầu đã đòi hỏi phải đưa vào khái niệm số nguyên trong một trường như vậy K, tổng quát hóa khái niệm số nguyên hữu tỉ trong trường $\mathbf{Q}$. Lý thuyết tổng quát của khái niệm "số nguyên đại số" này, gắn với, như sẽ thấy, những điều kiện hữu hạn rất ngặt, được phát triển trong Chương V; nó có thể được áp dụng cho mọi vành giao hoán và có tầm quan trọng lớn không những trong số học, mà còn trong hình học đại số và ngay cả trong lý thuyết hiện đại về các "không gian giải tích" trên trường $\mathbf{C}$.

Một trong những trở ngại chủ yếu đối với việc mở rộng số học cổ điển sang các vành số nguyên đại số từ lâu là sự phân tích cổ điển của một số nguyên hữu tỉ thành các thừa số nguyên tố nói chung không mở rộng được sang các vành này. Việc xây dựng lý thuyết iđêan là cần thiết để vượt qua khó khăn này: khi đó sự phân tích duy nhất được tìm kiếm được thiết lập cho các iđêan, khái niệm iđêan nguyên tố thay thế cho khái niệm số nguyên tố. Hơn nữa, kết quả này có thể được xem như một trường hợp điển hình trong đó "sự chuyển từ địa phương sang toàn cục" được thực hiện một cách thỏa đáng: việc biết, với $x \in K$, các giá trị tại $x$ của mọi "định giá" trên K xác định $x$ sai khác đến một phép nhân với một số nguyên khả nghịch.

Trong những vành kém đơn giản hơn các vành số nguyên đại số (và chẳng hạn ngay cả đối với các vành đa thức theo nhiều ẩn) kết quả này không còn đúng nữa. Tuy nhiên, có thể liên kết một cách chính tắc với mọi iđêan một tập hợp các iđêan nguyên tố được xác định rõ: trong hình học đại số, nếu chẳng hạn ta xét trong $K^n$ (K là một trường giao hoán tùy ý) một đa tạp con được xác định bởi một hệ phương trình đa thức $P_\alpha = 0$, thì các thành phần bất khả quy của đa tạp con này tương ứng song ánh với các phần tử cực tiểu của tập hợp các iđêan nguyên tố được liên kết như vậy với iđêan sinh bởi các $P_\alpha$. Hơn nữa, cũng có thể (nếu ta chỉ giới hạn ở các vành Noether) cho với mọi iđêan một "phân tích" kém chính xác hơn một phân tích thành tích các iđêan nguyên tố: ở đây tích thực ra được thay bằng giao và các lũy thừa của các iđêan nguyên tố được thay bằng các iđêan "nguyên sơ" liên thông với các iđêan nguyên tố liên kết với iđêan đang xét (nhưng không phải là các tổng quát hóa trực tiếp của các lũy thừa của iđêan nguyên tố). Việc đưa vào các iđêan nguyên tố liên kết với một iđêan và việc nghiên cứu các tính chất của chúng là đối tượng của Chương IV; ở đây cũng chứng minh sự tồn tại và một số tính chất duy nhất của các "phân tích nguyên sơ" mà ta vừa nói tới; nhưng hiện nay có vẻ như các phân tích này nói chung chỉ đóng một vai trò phụ trong các áp dụng, còn khái niệm cốt yếu là khái niệm iđêan nguyên tố liên kết với một iđêan.

Trong Chương VII, chúng tôi khảo sát chi tiết hơn các vành mà các tính chất của chúng gần nhất với các tính chất của các vành số nguyên đại số về mặt phân tích thành tích các iđêan nguyên tố; trong số những điều khác, có thể đưa vào các vành này khái niệm "ước", là phương diện hình học của sự phân tích này và giữ một vai trò quan trọng trong hình học đại số.

Sau cùng, từ Chương VIII trở đi sẽ khảo sát các khái niệm được quan tâm nhiều hơn trong hình học đại số hơn là trong số học (nơi chúng trở nên tầm thường), đặc biệt là khái niệm chiều.

Với các khái niệm này, chúng ta đi tới biên giới của bản thân hình học đại số, một biên giới luôn luôn dịch chuyển và khó vạch ra. Vì, nếu đại số giao hoán là một công cụ cốt yếu cho sự phát triển của hình học đại số trong toàn bộ tính tổng quát của nó, thì ngược lại (như đã thấy ở trên) ngôn ngữ hình học tỏ ra rất thuận tiện để phát biểu các định lý của đại số giao hoán và gợi ra một trực giác nào đó vốn dĩ vắng mặt một cách tự nhiên trong đại số trừu tượng; cùng với xu hướng ngày càng mở rộng các giới hạn của hình học đại số, ngôn ngữ đại số và ngôn ngữ hình học hơn bao giờ hết có xu hướng hòa lẫn vào nhau.
