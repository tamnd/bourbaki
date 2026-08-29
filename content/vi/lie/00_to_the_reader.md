---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: ""
chapter_title: ""
section: 0
section_title: TO THE READER
kind: reader
lang: vi
source: lie-i-iii
pdf_pages: 0005-0007
extraction: ocr
statements: 0
exercises: 0
content_sha256: 8d41d13dbf3478b04d7f25dd3b6b6f6ca739401bc8b21f88a5bbc0dc2e6a70b0
translated_from: content/en/lie/00_to_the_reader.md
source_content_sha256: 882ada8dae42b2f3f9dd77120386c8bef6ec91cad68747363da14d5f7e825848
translation_model: gpt-5-mini
translation_run: translate-vi-62faf8a7
glossary_version: 34
glossary_terms_sha256: 893df20e60de9859bd2b904985f455099f3bd5b03506b069757e7a5b3267bf11
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## GỬI BẠN ĐỌC

1. Chuỗi các tập này, danh sách của chúng được cho ở các trang ix và x, trình bày toán học ngay từ đầu và đưa ra các chứng minh đầy đủ. Về nguyên tắc, nó không đòi hỏi ở người đọc một kiến thức toán học đặc biệt nào, mà chỉ cần một sự quen thuộc nhất định với lập luận toán học và một khả năng nhất định về tư duy trừu tượng. Tuy nhiên, nó đặc biệt hướng đến những người có kiến thức tốt về ít nhất là nội dung của một hoặc hai năm đầu của một khóa học toán đại học.

2. Phương pháp trình bày mà chúng tôi đã lựa chọn là tiên đề và trừu tượng, và thông thường đi từ tổng quát đến cụ thể. Lựa chọn này được quyết định bởi mục đích chính của chuyên luận, đó là cung cấp một nền tảng vững chắc cho toàn bộ toán học hiện đại. Vì mục đích này, điều không thể thiếu là làm quen với một số lượng khá lớn các ý tưởng và nguyên lý rất tổng quát. Hơn nữa, các yêu cầu của chứng minh áp đặt một cấp bậc được xác định nghiêm ngặt lên đối tượng. Do đó, ích lợi của một số xem xét nhất định sẽ không ngay lập tức hiện rõ đối với người đọc, trừ khi người đó đã có một kiến thức toán học khá rộng; nếu không, người đó phải có sự kiên nhẫn để tạm gác sự phán xét cho đến khi có dịp thích hợp.

3. Để giảm bớt bất lợi này, chúng tôi thường xuyên đưa vào văn bản các ví dụ liên quan đến những sự kiện mà người đọc có thể đã biết nhưng chưa được thảo luận trong chuỗi này. Những ví dụ như vậy luôn được đặt giữa hai dấu sao: \* . . . *. Hầu hết độc giả chắc chắn sẽ thấy rằng các ví dụ này giúp họ hiểu văn bản, và sẽ thích không bỏ qua chúng, ngay cả khi đọc lần đầu. Việc bỏ qua chúng dĩ nhiên không gây bất lợi nào, xét trên quan điểm lôgic thuần túy.

4. Chuỗi này được chia thành các tập (ở đây gọi là “Sách”). Sáu Sách đầu tiên được đánh số và, nói chung, mọi mệnh đề trong văn bản chỉ giả định đã biết những kết quả đã được thảo luận trong các tập trước đó. Quy tắc này được áp dụng trong mỗi Sách, nhưng để thuận tiện cho việc trình bày, các Sách này không còn được sắp xếp theo một thứ tự liên tiếp nữa. Ở đầu mỗi Sách này (hoặc mỗi chương này), người đọc sẽ tìm thấy một chỉ dẫn chính xác về quan hệ lôgic của nó với các Sách khác và do đó có thể tự thỏa mãn rằng không có vòng tròn luẩn quẩn nào.

5. Khung lôgic của mỗi chương gồm các *định nghĩa*, các *tiên đề*, và các *định lý* của chương. Đây là những phần chủ yếu cần được ghi nhớ để sử dụng về sau. Những kết quả ít quan trọng hơn và những kết quả có thể dễ dàng suy ra từ các định lý được gọi là “mệnh đề”, “bổ đề”, “hệ quả”, “nhận xét”, v.v. Những phần có thể bỏ qua trong lần đọc đầu tiên được in bằng kiểu chữ nhỏ. Một chú giải về một định lý đặc biệt quan trọng đôi khi xuất hiện dưới tên “chú giải”.

Để tránh những sự lặp lại nhàm chán, đôi khi thuận tiện khi đưa vào các ký hiệu hoặc các chữ viết tắt chỉ có hiệu lực trong một chương nhất định hoặc một tiết diện nhất định của một chương (ví dụ, trong một chương chỉ xét các vành giao hoán, từ “vành” luôn có nghĩa là “vành giao hoán”). Những quy ước như vậy luôn được nêu rõ, nói chung là ở đầu chương mà chúng xuất hiện.

6. Một số đoạn trong văn bản được thiết kế để cảnh báo trước cho người đọc về những sai lầm nghiêm trọng. Những đoạn này được đánh dấu ở lề bằng dấu

☡

(“chỗ ngoặt nguy hiểm”).

7. Các Bài tập được thiết kế vừa để giúp người đọc tự thỏa mãn rằng mình đã lĩnh hội văn bản, vừa để đưa ra trước mắt người đọc những kết quả không có chỗ trong văn bản nhưng vẫn đáng quan tâm. Những bài tập khó nhất mang dấu ¶.

8. Nói chung, chúng tôi đã tuân theo thuật ngữ được chấp nhận rộng rãi, trừ khi có những lý do chính đáng để đi lệch khỏi nó.

9. Chúng tôi đã đặc biệt cố gắng luôn sử dụng ngôn ngữ đúng đắn một cách nghiêm ngặt, mà không hy sinh tính đơn giản. Trong khả năng có thể, chúng tôi đã lưu ý trong văn bản đến *sự lạm dụng ngôn ngữ*, bởi nếu thiếu điều đó, bất kỳ văn bản toán học nào cũng có nguy cơ trở nên kiểu cách, thậm chí khó đọc.

10. Vì về nguyên tắc văn bản gồm sự trình bày giáo điều của một lý thuyết, nên nói chung nó không chứa các tham chiếu đến tài liệu. Các tham chiếu thư mục được tập hợp trong *Các ghi chú lịch sử*, thường ở cuối mỗi chương. Các ghi chú này cũng chứa, khi thích hợp, các chỉ dẫn về những vấn đề chưa được giải quyết của lý thuyết.

Thư mục theo sau mỗi ghi chú lịch sử nói chung chỉ chứa những sách và hồi ký nguyên bản có tầm quan trọng lớn nhất trong sự phát triển của lý thuyết đang được xét. Nó không hề tuyên bố về tính đầy đủ; đặc biệt, các tham chiếu chỉ nhằm xác định các vấn đề về quyền ưu tiên hầu như luôn bị bỏ qua.

Đối với các bài tập, nói chung chúng tôi không cho rằng cần thiết phải chỉ ra nguồn gốc của chúng, vì chúng được lấy từ nhiều nguồn khác nhau (các bài báo gốc, sách giáo khoa, các tuyển tập bài tập).

11. Các tham chiếu đến một phần của chuỗi này được đưa ra như sau:
a) Nếu tham chiếu đến các định lý, tiên đề, hoặc định nghĩa được trình bày trong cùng một tiết diện, chúng được trích dẫn bằng số của chúng.
b) Nếu chúng xuất hiện trong một tiết diện khác của cùng một chương, tiết diện này cũng được trích dẫn trong tham chiếu.
c) Nếu chúng xuất hiện trong một chương khác của cùng một Sách, chương và tiết diện được trích dẫn.
d) Nếu chúng xuất hiện trong một Sách khác, Sách này trước hết được trích dẫn bằng nhan đề của nó.

Các Bảng tóm tắt kết quả được trích dẫn bằng chữ R; do đó, Lý thuyết tập hợp, R có nghĩa là “Bảng tóm tắt kết quả của Lý thuyết tập hợp”.
