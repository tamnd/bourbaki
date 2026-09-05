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
content_sha256: fdc21d5614ad42c65cec5f02319d8d2c387805d8732e4b4fe712a2ef5af7693a
translated_from: content/en/ac/00_introduction.md
source_content_sha256: 76b5a99586b68b13462663dc0c9b880af0d70ce65bdf4d0e0496ed1cda0fd86b
translation_model: gpt-5-mini, gpt-5-6
translation_run: translate-vi-f92dbaee
glossary_version: 34
glossary_terms_sha256: ea70d1bb9c08e99bca006ea204a49e1d773d96b500cecc0da21c474fa424bd0f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## GIỚI THIỆU

Các câu hỏi được xét trong Quyển này nảy sinh trong quá trình phát triển của lý thuyết số đại số và (sau đó) hình học đại số (xem Ghi chú lịch sử). Từ thế kỷ 19 trở đi, hai lý thuyết này bắt đầu biểu lộ những sự tương tự đáng chú ý; nỗ lực giải quyết các bài toán do chúng đặt ra đã dẫn đến việc tách ra một số ý tưởng tổng quát mà lĩnh vực áp dụng không chỉ giới hạn trong các vành của các số đại số hoặc các hàm đại số; và, như thường lệ, có lợi khi xét chúng dưới dạng tổng quát nhất để thấy được ý nghĩa đích thực của chúng và những ảnh hưởng qua lại của một nghiên cứu đối với một nghiên cứu khác. Các khái niệm được xét trong Quyển này về nguyên tắc có thể áp dụng cho mọi vành giao hoán và các môđun trên những vành như vậy; tuy nhiên cần chỉ ra rằng các kết quả đáng kể thường chỉ thu được dưới một số giả thiết nhất định về *hữu hạn* (những giả thiết này luôn đúng trong các trường hợp cổ điển), chẳng hạn bằng cách giả sử các môđun là sinh hữu hạn hoặc các vành là Noether.

Các khái niệm chủ yếu giữ vai trò trung tâm trong những chương đầu là các khái niệm sau:

**I. Địa phương hóa và toàn cục hóa.** Chẳng hạn, hãy bắt đầu với một hệ phương trình Diophantine :

(*) $$
P_i(x_1, \ldots, x_r) = 0 \quad (1 \leq i \leq n)
$$

trong đó các $P_i$ là các đa thức với hệ số nguyên và ta tìm các nghiệm $(x_i)$ gồm các số *nguyên* hữu tỉ. Có thể bắt đầu tiếp cận bài toán bằng cách tìm các nghiệm gồm các *số hữu tỉ*, điều này tương ứng với việc xét cùng một bài toán với các hệ số của các $P_i$ được xem như các phần tử của *trường phân thức* $\mathbf{Q}$ của $\mathbf{Z}$ và các nghiệm được tìm với các giá trị trong $\mathbf{Q}$. Bước thứ hai là xem xét, với một số nguyên tố $p$ cho trước, có tồn tại hay không các nghiệm hữu tỉ mà mẫu số của chúng không chia hết cho $p$ (các nghiệm *nguyên* rõ ràng thỏa mãn điều kiện này); trong trường hợp này, điều đó tương đương với việc thuộc vành con $\mathbf{Z}_{(p)}$ của $\mathbf{Q}$ gồm các số hữu tỉ có dạng này, được gọi là *vành địa phương* của $\mathbf{Z}$ tương ứng với số nguyên tố $p$. Rõ ràng phép chuyển từ $\mathbf{Z}$ sang $\mathbf{Q}$ và phép chuyển từ $\mathbf{Z}$ sang $\mathbf{Z}_{(p)}$ có cùng dạng: trong cả hai trường hợp, các mẫu số duy nhất được phép không thuộc một *iđêan nguyên tố* nào đó (lần lượt là iđêan $(0)$ và iđêan $(p)$). Cùng một tên gọi "vành địa phương" xuất hiện trong hình học đại số, nơi khái niệm này xuất hiện một cách tự nhiên hơn: chẳng hạn đối với vành $\mathbf{C}[X]$ của các đa thức theo một biến với hệ số phức, vành địa phương tương ứng với iđêan nguyên tố $(X - a)$ là vành các phân thức hữu tỉ "chính quy" tại điểm $a$ (nghĩa là, không có cực tại điểm đó).

Mọi bài toán Diophantine và nói chung mọi bài toán về các A-môđun (A là một vành giao hoán) đều có thể phân tích thành hai bài toán phụ: nghiệm của nó được tìm trong các vành địa phương A, tương ứng với các iđêan nguyên tố khác nhau $\mathfrak{p}$ của A ("địa phương hóa"), sau đó đặt câu hỏi liệu có thể kết luận từ sự tồn tại, với mọi $\mathfrak{p}$, của một nghiệm cho bài toán "đã địa phương hóa" rằng tồn tại một nghiệm cho bài toán được đặt ra ban đầu hay không ("chuyển từ địa phương sang toàn cục"). Chương II dành cho việc nghiên cứu quá trình kép này và cũng thấy rằng "địa phương hóa" không chỉ liên quan đến các iđêan nguyên tố, mà có phạm vi rộng hơn.

11. *Đầy đủ hóa & vành địa phương*. Một vành địa phương A có chung với các trường tính chất chỉ có *một* iđêan cực đại m. Sự kiện này được dùng để biến đổi, ở một mức độ nào đó, một bài toán về các A-môđun thành một bài toán tương tự về các *không gian vectơ* bằng cách chuyển qua vành thương $A/m$, vì vành sau này là một trường. Nếu quay trở lại chẳng hạn với hệ Diophantine (*) thì ý tưởng này không gì khác ngoài nguyên lý "giảm modulo K", biến đổi các phương trình thành các đồng dư thức mod. $p$, điều đã xuất hiện một cách tự nhiên ngay từ những công trình đầu tiên trong lý thuyết số.

Như vậy, rõ ràng chúng ta không thể hy vọng theo cách này thu được các kết quả đầy đủ cho bài toán ban đầu và người ta nhanh chóng nhận ra rằng để có được những thông tin chính xác hơn, cần phải xét không chỉ các đồng dư thức modulo m, mà còn cả các đồng dư thức "cao hơn" modulo $m^n$, với các số nguyên tùy ý $n > 0$. Do đó người ta thấy rằng, $n$ càng lớn thì theo một cách nào đó bài toán ban đầu càng được "tiếp cận" gần hơn (trong trường hợp $A = \mathbf{Z}$ chẳng hạn, lý do là một số nguyên $\neq 0$ không thể chia hết cho *tất cả* các lũy thừa $p^n$ của một số nguyên tố $p$ đã cho; do đó số này sẽ biểu lộ sự hiện diện của nó trong phép giảm mod. $p^n$ miễn là lấy $n$ đủ lớn). Sự diễn đạt toán học của ý tưởng này là xét trên A một tôpô vành (xem *Tôpô đại cương*, Chương III, § 6) trong đó các $m^n$ tạo thành một hệ lân cận cơ sở của 0. Nhưng khi chẳng hạn chúng ta đã giải được hệ đồng dư thức

$$
\text{P}_i(x_1, \ldots, x_m) \equiv 0 \ (\text{mod. } p^k) \qquad (1 \leq i \leq n)
$$

với *mọi số nguyên* $k > 0$, thì vẫn không suy ra rằng hệ (*) có một nghiệm trong vành địa phương $\mathbf{Z}_{(p)}$; giả thiết trên có thể được hiểu là nói rằng (*) nhận một nghiệm trong *bao đầy đủ* $\hat{\mathbf{Z}}_{(p)}$ của vành tôpô $\mathbf{Z}_{(p)}$.

Bài toán ban đầu, được làm yếu đi như vậy, cuối cùng được biến đổi thành bài toán tương tự đối với các vành địa phương kiểu $A/m^n$, những vành này cũng gần các trường hơn các vành tổng quát, vì chúng có một căn lũy linh; trong hình học đại số cổ điển điều này tương ứng với một nghiên cứu "vi phân" của bài toán trong lân cận của một điểm đã cho.

Chương III trình bày một cách tổng quát các áp dụng này của những khái niệm tôpô vào lý thuyết các vành địa phương. Trong Chương VI, một khía cạnh đặc biệt của vấn đề này được nghiên cứu, được thích nghi một mặt cho những nghiên cứu chi tiết hơn về hình học đại số, và trên hết cho số học của các trường số đại số, nơi các vành địa phương gặp phải (chẳng hạn $\mathbf{Z}_{(p)}$) thuộc một lớp đặc biệt đơn giản, đó là lớp các "vành định giá", trong đó tính chia hết là một thứ tự toàn phần (xem Đại số, Chương VI, § 1) của tập hợp các iđêan chính.

Việc nghiên cứu phép chuyển từ một vành A sang một vành địa phương A, hoặc sang một hoàn thành $\hat{A}$ làm nổi bật một đặc điểm chung cho hai phép toán này, đó là tính chất phẳng của các A-môđun A, và $\hat{A}$, cho phép, trong số những điều khác, việc sử dụng các tích tenxơ của những A-môđun như vậy với các A-môđun tùy ý theo một cách hơi giống với các tích tenxơ của các không gian vectơ, nghĩa là không có tất cả những sự thận trọng bao quanh việc sử dụng chúng trong trường hợp tổng quát. Các tính chất liên kết với khái niệm này, vốn cũng áp dụng được cho các môđun trên các vành không giao hoán, là đối tượng nghiên cứu của Chương I.

III. Số nguyên và phân tích các iđêan. Việc nghiên cứu tính chia hết trong các trường số đại số ngay từ đầu đã đòi hỏi phải đưa vào khái niệm số nguyên trong một trường K như vậy, mở rộng khái niệm số nguyên hữu tỉ trong trường $\mathbf{Q}$. Lý thuyết tổng quát về khái niệm "số nguyên đại số" này, như sẽ thấy, liên kết với những điều kiện hữu hạn rất ngặt, được phát triển trong Chương V; nó có thể được áp dụng cho mọi vành giao hoán và có tầm quan trọng lớn không chỉ trong số học, mà còn trong hình học đại số và thậm chí trong lý thuyết hiện đại về các "không gian giải tích" trên trường $\mathbf{C}$.

Một trong những trở ngại lớn đối với việc mở rộng số học cổ điển sang các vành số nguyên đại số từ lâu đã là việc phân tích cổ điển một số nguyên hữu tỉ thành các thừa số nguyên tố nói chung không mở rộng được sang các vành này. Việc xây dựng lý thuyết các iđêan là cần thiết để vượt qua khó khăn này: các phân tích duy nhất khi đó được thiết lập cho các iđêan, khái niệm iđêan nguyên tố được thay thế cho khái niệm số nguyên tố. Hơn nữa, kết quả này có thể được xem như một trường hợp điển hình trong đó "phép chuyển từ địa phương sang toàn cục" được thực hiện thỏa đáng: sự hiểu biết, đối với $x \in K$, về các giá trị tại x của tất cả các "định giá" trên K xác định x sai khác một phép nhân bởi một số nguyên khả nghịch.

Trong các vành ít đơn giản hơn các vành số nguyên đại số (và thậm chí chẳng hạn trong các vành đa thức với nhiều bất định) kết quả này không còn đúng nữa. Tuy nhiên có thể liên kết theo một cách chính tắc với mỗi iđêan một tập hợp được xác định rõ các iđêan nguyên tố: trong hình học đại số, nếu ta xét chẳng hạn trong $K^n$ (K là một trường giao hoán tùy ý) một đa tạp con được xác định bởi một hệ các phương trình đa thức $P_\alpha = 0$, thì các thành phần bất khả quy của đa tạp con này tương ứng song ánh với các phần tử cực tiểu của tập hợp các iđêan nguyên tố được liên kết như vậy với iđêan sinh bởi các $P_\alpha$. Ngoài ra còn có thể (nếu ta hạn chế vào các vành Noether) cho mỗi iđêan một "phân tích" kém chính xác hơn một phân tích thành tích của các iđêan nguyên tố: ở đây tích thực ra được thay thế bởi giao và các lũy thừa của các iđêan nguyên tố bởi các iđêan "nguyên sơ" liên kết với các iđêan nguyên tố liên kết với iđêan đang xét (nhưng chúng không phải là những mở rộng trực tiếp của các lũy thừa của các iđêan nguyên tố). Việc đưa vào các iđêan nguyên tố liên kết với một iđêan và việc nghiên cứu các tính chất của chúng là chủ đề của Chương IV; ở đây cũng vậy, sự tồn tại và một số tính chất duy nhất của các "phân tích nguyên sơ" mà ta vừa đề cập được chứng minh; nhưng hiện nay dường như các phân tích này thường chỉ đóng một vai trò phụ trong các áp dụng, khái niệm cốt yếu là khái niệm iđêan nguyên tố liên kết với một iđêan.

Trong Chương VII, chúng tôi xét chi tiết hơn các vành mà các tính chất của chúng gần nhất với các tính chất của các vành số nguyên đại số xét về phân tích thành tích các iđêan nguyên tố; trong số những điều khác, có thể đưa vào các vành này khái niệm "ước", đó là khía cạnh hình học của sự phân tích này và đóng một vai trò quan trọng trong hình học đại số.

Cuối cùng, các Chương VIII và tiếp theo sẽ xét các khái niệm có nhiều quan tâm hơn trong hình học đại số so với trong số học (nơi chúng trở nên tầm thường) và đặc biệt là khái niệm chiều.

Với các khái niệm này, ta đi đến biên giới của hình học đại số thực sự, một biên giới luôn chuyển động và khó vạch ra. Bởi vì, nếu đại số giao hoán là một công cụ cốt yếu cho sự phát triển của hình học đại số trong toàn bộ tính tổng quát của nó, thì ngược lại (như đã thấy ở trên) ngôn ngữ hình học tỏ ra rất thuận tiện để biểu đạt các định lý của đại số giao hoán và gợi lên một trực giác vốn dĩ vắng mặt một cách tự nhiên trong đại số trừu tượng; với xu hướng ngày càng mở rộng các giới hạn của hình học đại số, ngôn ngữ đại số và hình học có xu hướng hòa nhập với nhau hơn bao giờ hết.
