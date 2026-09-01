---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ELEMENTS OF THE HISTORY OF MATHEMATICS
section: 11
section_title: Uniform Spaces
lang: vi
source: hist
pdf_pages: 0147-0148
extraction: ocr
statements: 0
exercises: 0
content_sha256: 499f2714cc0e977f9d9d9f1d3766761fed10ad0a447d5b59af4f5a5c3d825294
translated_from: content/en/hist/1/11_s11_uniform_spaces.md
source_content_sha256: 2860052876fd130ce2e248a166f6a973e304ef320bb3054ac1d9d92b237812ff
translation_model: gpt-5-6
translation_run: translate-vi-c4145938
glossary_version: 34
glossary_terms_sha256: 407add2926de65dd90d6c24f21d65889f78c161d027f5ec257f333503c13a0f5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 11. KHÔNG GIAN ĐỀU.

Các khái niệm và mệnh đề chính liên quan đến các không gian đều xuất hiện dần dần từ lý thuyết về các biến thực, và chỉ mới gần đây mới là đối tượng của sự nghiên cứu có hệ thống. Cauchy, khi tìm cách thiết lập một cách chặt chẽ lý thuyết về các chuỗi (xem p. 153), đã lấy làm điểm xuất phát một nguyên lý mà ông dường như xem là hiển nhiên, theo đó một điều kiện cần và đủ để một dãy $(a_n)$ hội tụ là $|a_{n+p} - a_n|$ phải nhỏ tùy ý khi $n$ đủ lớn (xem chẳng hạn ([56 a], (2), t. VII, p. 267)). Cùng với Bolzano [27 c], ông chắc chắn là một trong những người đầu tiên phát biểu tường minh nguyên lý này, và nhận ra tầm quan trọng của nó: do đó có tên “dãy Cauchy” được gán cho các dãy số thực thỏa mãn điều kiện đang xét, và bằng mở rộng cho các dãy $(x_n)$ các điểm trong một không gian metric sao cho khoảng cách giữa $x_{n+p}$ và $x_n$ nhỏ tùy ý khi $n$ đủ lớn; từ đó cuối cùng có tên “lọc Cauchy” được gán cho sự tổng quát hóa của các dãy Cauchy trong các không gian đều.

Khi về sau khái niệm trực giác về số thực không còn thỏa mãn nữa, và người ta tìm cách, để đặt Giải tích trên một nền tảng vững chắc, định nghĩa các số thực bắt đầu từ các số hữu tỉ, thì chính nguyên lý Cauchy đã cung cấp một trong những định nghĩa phong phú nhất trong số các định nghĩa được đề xuất vào nửa sau thế kỷ XIX; đó là định nghĩa của Cantor ([47], tr. 93-96) (cũng được phát triển, trong số những người khác, từ các ý tưởng của Cantor, bởi Heine [154 b], và một cách độc lập, bởi Méray), theo đó người ta cho tương ứng một số thực với mỗi dãy Cauchy (“dãy cơ bản” theo thuật ngữ của Cantor) các số hữu tỉ; cùng một số thực sẽ tương ứng với hai dãy Cauchy các số hữu tỉ $(a_n)$ và $(b_n)$ nếu $|a_n - b_n|$ tiến tới không, và chỉ trong trường hợp này. Ý tưởng cốt yếu ở đây là, theo một quan điểm nào đó, tập hợp $\mathbf{Q}$ các số hữu tỉ là “không đầy đủ”, và tập hợp các số thực là tập hợp “đầy đủ” được suy ra từ $\mathbf{Q}$ bằng cách “hoàn thành” nó.

Mặt khác, Heine, trong các công trình chủ yếu được gợi ý bởi các ý tưởng của Weierstrass và Cantor, là người đầu tiên định nghĩa tính liên tục đều cho các hàm số của một hoặc nhiều biến thực [154 a], và đã chứng minh rằng mọi hàm số, liên tục trên một khoảng đóng bị chặn của $\mathbf{R}$, đều liên tục đều trên đó [154 b]: đó là “định lý Heine”. Kết quả này gắn với tính compact của một khoảng đóng bị chặn trong $\mathbf{R}$ (“định lý Borel-Lebesgue", xem p. 141), và chứng minh mà Heine đưa ra cho định lý của ông cũng có thể được dùng, với một vài sửa đổi, để chứng minh định lý Borel-Lebesgue (điều mà đối với một số tác giả dường như là một lý do đủ để đặt cho định lý này tên “định lý Heine-Borel”).

Sự mở rộng các ý tưởng này đến các không gian tổng quát hơn được thực hiện khi, trước hết một số trường hợp đặc biệt được nghiên cứu, rồi sau đó nói chung, các không gian metric, trong đó một khoảng cách (hàm số của các cặp điểm, thỏa mãn một số tiên đề nhất định) được cho và đồng thời xác định một tôpô và một cấu trúc đều. Fréchet, người đầu tiên phát biểu định nghĩa tổng quát của các không gian này, đã nhận ra tầm quan trọng của nguyên lý Cauchy [115 a], và cũng đưa vào cho mọi không gian metric khái niệm không gian tiền compact (hay “hoàn toàn bị chặn” [115 a và b]). Hausdorff, người trong “Mengenlehre” [152 a và b] đã phát triển nhiều lý thuyết về các không gian metric, đặc biệt nhận ra rằng người ta có thể áp dụng cho các không gian này phép dựng Cantor đã được xét ở trên, và do đó suy ra, đối với mỗi không gian metric không “đầy đủ” (nghĩa là nơi nguyên lý Cauchy không đúng), một không gian metric “đầy đủ”.

Các không gian metric là các “không gian đều” thuộc một loại đặc biệt; các không gian đều chỉ mới được định nghĩa một cách tổng quát gần đây, bởi A. Weil [330 b]. Trước đó người ta chỉ biết cách sử dụng các khái niệm và kết quả liên quan đến “cấu trúc đều” khi xét các không gian metric: điều này giải thích vai trò quan trọng được đóng trong nhiều công trình hiện đại về tôpô bởi các không gian metric hoặc mêtric hóa được (và đặc biệt bởi các không gian compact mêtric hóa được) trong những vấn đề mà khoảng cách không có ích lợi thực sự nào. Một khi định nghĩa về các không gian đều được phát biểu, không có khó khăn gì (đặc biệt khi khái niệm lọc cũng có sẵn) trong việc mở rộng đến các không gian này gần như toàn bộ lý thuyết về các không gian metric, như chẳng hạn được trình bày bởi Hausdorff (và mở rộng theo cùng cách, chẳng hạn, đến mọi không gian compact, các kết quả được trình bày cho các không gian metric compact trong Tôpô của Alexandroff-Hopf [4]). Đặc biệt, định lý hoàn thành cho các không gian đều không gì khác hơn là sự chuyển đổi, không có bất kỳ sửa đổi cốt yếu nào, của phép dựng Cantor đối với các số thực.
