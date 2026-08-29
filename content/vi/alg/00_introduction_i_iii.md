---
book: alg
book_title: Algebra
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0021-0023
extraction: ocr
statements: 0
exercises: 0
content_sha256: 070b54d17f995967b83ae009c2f4b649438d1dda1b55a62a1f9f5b6fab8aa1a5
translated_from: content/en/alg/00_introduction_i_iii.md
source_content_sha256: 95936eb99f28c9abcab27ec59169aeb970a237913763d70013fdd74c7e6811c6
translation_model: gpt-5.4
translation_run: translate-vi-0ed643d2
glossary_version: 34
glossary_terms_sha256: 91f34fa3eadf7dcbd90ef24c62547dd656c1ac14d5d40859a6bea796ace1ccbc
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## GIỚI THIỆU

Đại số về bản chất liên quan đến việc tính toán, nghĩa là thực hiện, trên các phần tử của một tập hợp, các "phép toán đại số", mà ví dụ quen thuộc nhất là "bốn phép tính" của số học sơ cấp.

Ở đây không phải chỗ để lần lại quá trình chậm chạp của phép trừu tượng hóa tiến triển, qua đó khái niệm phép toán đại số, lúc đầu bị hạn chế vào các số tự nhiên và các đại lượng đo được, từng chút một mở rộng miền của nó, trong khi khái niệm "số" nhận một phép tổng quát hóa song song, cho đến khi, chuyển qua khỏi khái niệm sau, nó được áp dụng cho những phần tử không có tính chất "số" nào, chẳng hạn các hoán vị của một tập hợp (xem ghi chú lịch sử ở Chương I). Không còn nghi ngờ gì rằng chính khả năng của những sự mở rộng kế tiếp này, trong đó dạng của các phép tính vẫn giữ nguyên, còn bản tính của các thực thể toán học chịu những phép tính ấy thì biến đổi rất nhiều, đã dẫn tới việc dần dần tách ra nguyên lý chỉ đạo của Toán học hiện đại, tức là các thực thể toán học tự thân chúng ít có tầm quan trọng; điều quan trọng là các quan hệ của chúng (xem Tập I). Dù sao đi nữa, chắc chắn là Đại số đã đạt tới mức độ trừu tượng này sớm hơn hẳn các ngành khác của Toán học, và từ lâu đã quen được xem như sự nghiên cứu các phép toán đại số, độc lập với các thực thể toán học mà chúng có thể được áp dụng vào.

Bị tước bỏ mọi đặc trưng riêng biệt, khái niệm chung nằm dưới các phép toán đại số thông thường là rất đơn giản: thực hiện một phép toán đại số trên hai phần tử $a, b$ của cùng một tập hợp E, nghĩa là gắn với cặp có thứ tự $(a, b)$ một phần tử thứ ba xác định rõ $c$ của tập hợp E. Nói cách khác, trong khái niệm này không có gì hơn ngoài khái niệm hàm: cho một phép toán đại số tức là cho một hàm xác định trên $E \times E$ và nhận giá trị trong E; nét đặc biệt duy nhất nằm ở chỗ tập xác định của hàm là tích của hai tập hợp đồng nhất với tập hợp mà hàm nhận giá trị; ta đặt cho một hàm như vậy tên là luật hợp thành.

Bên cạnh những "luật trong" này, các nhà toán học đã đi đến chỗ xem xét (chủ yếu dưới ảnh hưởng của Hình học) một kiểu "luật hợp thành" khác; đó là các "luật tác động", trong đó, ngoài tập hợp E (vẫn như ở tiền cảnh), còn xuất hiện một tập hợp phụ $\Omega$, mà các phần tử của nó được gọi là các toán tử: lần này luật gắn với một cặp có thứ tự $(\alpha, a)$ gồm một toán tử $\alpha \in \Omega$ và một phần tử $a \in E$ một phần tử thứ hai $b$ của E. Chẳng hạn một phép vị tự tâm cho trước trên không gian Euclid E gắn với một số thực $k$ ("tỷ số vị tự", ở đây là toán tử) và một điểm A của E một điểm khác A' của E: đó là một luật tác động trên E.

Phù hợp với các định nghĩa tổng quát (Lý thuyết tập hợp, IV, § 1, no. 4), việc cho trên một tập hợp E một hay nhiều luật hợp thành hoặc luật tác động xác định một cấu trúc trên E; đối với các cấu trúc được xác định theo cách ấy, chúng tôi dành chính xác tên gọi cấu trúc đại số, và việc nghiên cứu chúng tạo thành Đại số.

Có nhiều loài (Lý thuyết tập hợp, IV, § 1, no. 4) cấu trúc đại số, được đặc trưng một mặt bởi các luật hợp thành hoặc luật tác động xác định chúng và mặt khác bởi các tiên đề mà các luật ấy phải tuân theo. Dĩ nhiên, các tiên đề này không được chọn một cách tùy ý, mà đơn giản là các tính chất của phần lớn các luật xuất hiện trong áp dụng, như tính kết hợp, tính giao hoán, v.v. Chương I về bản chất được dành cho việc trình bày các tiên đề ấy và các hệ quả tổng quát suy ra từ chúng; đồng thời còn có một nghiên cứu chi tiết hơn về hai loài cấu trúc đại số quan trọng nhất, đó là cấu trúc nhóm (trong đó chỉ có một luật hợp thành xuất hiện) và cấu trúc vành (với hai luật hợp thành), mà cấu trúc trường là một trường hợp riêng.

Trong Chương I cũng có các định nghĩa của nhóm với toán tử và vành với toán tử, trong đó, ngoài các luật hợp thành, còn xuất hiện một hay nhiều luật tác động. Các nhóm với toán tử quan trọng nhất là các môđun, mà các không gian vectơ là một ví dụ riêng, chúng đóng một vai trò quan trọng cả trong Hình học cổ điển lẫn trong Giải tích hiện đại. Việc nghiên cứu các cấu trúc môđun bắt nguồn từ việc nghiên cứu các phương trình tuyến tính, do đó có tên là Đại số tuyến tính; các kết quả về vấn đề này được trình bày trong Chương II.

Tương tự như vậy, các vành với toán tử thường gặp nhất được gọi là các đại số (hay các hệ siêu phức). Trong các Chương III và IV, người ta nghiên cứu chi tiết hai kiểu riêng của đại số: các đại số ngoài, cùng với lý thuyết định thức được dẫn xuất từ chúng, là một công cụ quý giá của Đại số tuyến tính; và các đại số đa thức, là nền tảng đối với lý thuyết các phương trình đại số.

Trong Chương V có sự trình bày lý thuyết tổng quát của các trường giao hoán và sự phân loại chúng. Nguồn gốc của lý thuyết này là sự nghiên cứu các phương trình đại số một ẩn; những vấn đề đã sinh ra lý thuyết ấy ngày nay hầu như không còn hơn một mối quan tâm lịch sử, nhưng lý thuyết các trường giao hoán vẫn là nền tảng đối với Đại số, vì nó là cơ sở của lý thuyết các số đại số một mặt và của Hình học đại số mặt khác.

Vì tập hợp các số tự nhiên có hai phép hợp thành, phép cộng và phép nhân, nên Số học cổ điển (hay Lý thuyết số), là ngành nghiên cứu các số tự nhiên, lệ thuộc vào Đại số. Tuy nhiên, liên quan với cấu trúc đại số được xác định bởi hai phép ấy còn có cấu trúc được xác định bởi quan hệ thứ tự "a chia hết b"; và nét đặc trưng của Số học cổ điển chính xác là việc nghiên cứu các quan hệ giữa hai cấu trúc liên kết ấy. Đây không phải là ví dụ duy nhất trong đó một cấu trúc thứ tự được liên kết như vậy với một cấu trúc đại số bởi một quan hệ "chia hết": quan hệ này cũng giữ một vai trò quan trọng không kém trong các vành đa thức. Vì vậy, một nghiên cứu tổng quát về vấn đề này sẽ được trình bày trong Chương VI; nghiên cứu ấy sẽ được áp dụng trong Chương VII để xác định cấu trúc của các môđun trên một số vành đặc biệt đơn giản và đặc biệt là đối với lý thuyết các "ước sơ cấp".

Các Chương VIII và IX dành cho những lý thuyết chuyên biệt hơn, nhưng có nhiều áp dụng trong Giải tích: một mặt là lý thuyết các môđun và vành nửa đơn, liên quan chặt chẽ với lý thuyết các biểu diễn tuyến tính của nhóm; mặt khác là lý thuyết các dạng toàn phương và các dạng Hermit, cùng với việc nghiên cứu các nhóm liên kết với chúng. Sau hết, các hình học sơ cấp (afin, xạ ảnh, Euclid, v.v.) được nghiên cứu trong các Chương II, VI và IX từ một quan điểm thuần túy đại số: ở đây hầu như không có gì hơn ngoài một ngôn ngữ mới để biểu đạt những kết quả Đại số đã thu được ở nơi khác, nhưng đó là một ngôn ngữ đặc biệt thích nghi với những phát triển về sau của Hình học đại số và Hình học vi phân, mà chương này dùng làm phần nhập môn.
