---
book: alg
book_title: Algebra
chapter: ""
chapter_title: ""
section: 0
section_title: TO THE READER
kind: reader
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0005-0007
extraction: ocr
statements: 0
exercises: 0
content_sha256: 28e13f37e37d08b0bbbdb791969e37bd531e6d75429d6edc75564709bf469c84
translated_from: content/en/alg/00_to_the_reader_i_iii.md
source_content_sha256: e903f839028df378aeb85e47ba7258f296c5fb25cbabdeb48cb8dbf5f24ab59c
translation_model: gpt-5-6
translation_run: translate-vi-3b54821b
glossary_version: 34
glossary_terms_sha256: 3a1e6f307d4198920f0e77be1c07da4c1b81da8655346d06cda0d878288bd023
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## GỬI ĐỘC GIẢ

1. Chuỗi các quyển này, danh sách của chúng được cho ở các trang ix và x, bắt đầu trình bày toán học từ đầu và đưa ra các chứng minh đầy đủ. Về nguyên tắc, nó không đòi hỏi ở độc giả một kiến thức toán học đặc biệt nào, mà chỉ cần một sự quen thuộc nhất định với lập luận toán học và một khả năng nhất định về tư duy trừu tượng. Tuy nhiên, nó đặc biệt hướng đến những người có kiến thức tốt về ít nhất là nội dung của một hoặc hai năm đầu của một khóa học toán học đại học.

2. Phương pháp trình bày mà chúng tôi đã chọn là tiên đề và trừu tượng, và thông thường tiến hành từ cái tổng quát đến cái riêng biệt. Lựa chọn này được quy định bởi mục đích chính của chuyên luận, đó là cung cấp một nền tảng vững chắc cho toàn bộ toán học hiện đại. Để đạt được điều này, điều không thể thiếu là làm quen với một số lượng khá lớn các ý tưởng và nguyên lý rất tổng quát. Hơn nữa, những đòi hỏi của chứng minh áp đặt một cấp bậc được xác định nghiêm ngặt lên đối tượng. Do đó, ích lợi của một số xem xét nhất định sẽ không ngay lập tức hiện ra đối với độc giả, trừ khi người đó đã có một kiến thức toán học khá rộng; nếu không, người đó phải có sự kiên nhẫn để tạm gác phán đoán cho đến khi có dịp thích hợp.

3. Để giảm bớt bất lợi này, chúng tôi thường xuyên đưa vào văn bản các ví dụ liên quan đến những sự kiện mà độc giả có thể đã biết nhưng chưa được thảo luận trong chuỗi này. Các ví dụ như vậy luôn được đặt giữa hai dấu sao: *...*. Phần lớn độc giả chắc chắn sẽ thấy rằng các ví dụ này sẽ giúp họ hiểu văn bản, và sẽ thích không bỏ qua chúng, ngay cả khi đọc lần đầu. Việc bỏ qua chúng dĩ nhiên không gây bất lợi nào, xét thuần túy về mặt lôgic.

4. Chuỗi này được chia thành các quyển (ở đây gọi là “Quyển”). Sáu Quyển đầu được đánh số và nói chung, mọi mệnh đề trong văn bản chỉ giả định đã biết những kết quả đã được thảo luận trong các quyển trước đó. Quy tắc này đúng trong mỗi Quyển, nhưng vì thuận tiện cho việc trình bày, các Quyển này không còn được sắp xếp theo một thứ tự liên tiếp nữa. Ở đầu mỗi Quyển này (hoặc của các chương này), độc giả sẽ tìm thấy một chỉ dẫn chính xác về quan hệ lôgic của nó với các Quyển khác và do đó sẽ có thể tự thỏa mãn rằng không có vòng tròn luẩn quẩn nào.

5. Khuôn khổ lôgic của mỗi chương gồm các định nghĩa, các tiên đề và các định lý của chương đó. Đây là những phần chủ yếu cần ghi nhớ để sử dụng về sau. Những kết quả ít quan trọng hơn và những kết quả có thể dễ dàng suy ra từ các định lý được gắn nhãn là “mệnh đề”, “bổ đề”, “hệ quả”, “nhận xét”, v.v. Những phần có thể bỏ qua khi đọc lần đầu được in bằng kiểu chữ nhỏ. Một lời bình luận về một định lý đặc biệt quan trọng đôi khi xuất hiện dưới tên “chú giải”.

Để tránh những sự lặp lại tẻ nhạt, đôi khi thuận tiện khi đưa vào các ký hiệu hoặc các chữ viết tắt chỉ có hiệu lực trong một chương nhất định hoặc một tiết diện nhất định của một chương (chẳng hạn, trong một chương chỉ xét các vành giao hoán, từ “vành” luôn có nghĩa là “vành giao hoán”). Những quy ước như vậy luôn được nêu tường minh, nói chung là ở đầu chương nơi chúng xuất hiện.

6. Một số đoạn trong văn bản được thiết kế để cảnh báo trước cho độc giả về những sai lầm nghiêm trọng. Các đoạn này được đánh dấu ở lề bằng ký hiệu ☡ (“khúc quanh nguy hiểm”).

7. Các Bài tập được thiết kế vừa để giúp độc giả tự kiểm tra rằng mình đã lĩnh hội văn bản, vừa để đưa ra sự chú ý của độc giả những kết quả không có chỗ trong văn bản nhưng vẫn đáng quan tâm. Các bài tập khó nhất mang ký hiệu ¶.

8. Nói chung, chúng tôi đã tuân theo thuật ngữ được chấp nhận rộng rãi, trừ khi có những lý do chính đáng để đi chệch khỏi nó.

9. Chúng tôi đã đặc biệt cố gắng luôn sử dụng ngôn ngữ chính xác một cách nghiêm ngặt, mà không hy sinh tính đơn giản. Trong chừng mực có thể, chúng tôi đã chỉ ra trong văn bản những sự lạm dụng ngôn ngữ, nếu thiếu chúng thì bất kỳ văn bản toán học nào cũng có nguy cơ trở nên kiểu cách, chưa nói đến không thể đọc được.

10. Vì về nguyên tắc văn bản gồm sự trình bày giáo điều của một lý thuyết, nên nói chung nó không chứa các tham chiếu đến tài liệu. Các tham chiếu thư mục được tập hợp trong các Ghi chú lịch sử, thường ở cuối mỗi chương. Các ghi chú này cũng chứa những chỉ dẫn, khi thích hợp, về các vấn đề chưa được giải quyết của lý thuyết.

Thư mục theo sau mỗi ghi chú lịch sử nói chung chỉ chứa những sách và hồi ký nguyên thủy có tầm quan trọng lớn nhất trong sự phát triển của lý thuyết đang được bàn luận. Nó không hề có ý định đầy đủ; đặc biệt, các tham chiếu chỉ nhằm xác định những vấn đề về quyền ưu tiên hầu như luôn được bỏ qua.

Đối với các bài tập, nói chung chúng tôi không thấy cần thiết phải chỉ ra nguồn gốc của chúng, vì chúng được lấy từ nhiều nguồn khác nhau (các bài báo nguyên thủy, giáo trình, các tuyển tập bài tập).

11. Các tham chiếu đến một phần của chuỗi này được đưa ra như sau:

a) Nếu tham chiếu đến các định lý, tiên đề hoặc định nghĩa được trình bày trong cùng một tiết diện, chúng được trích dẫn bằng số của chúng.
b) Nếu chúng xuất hiện trong một tiết diện khác của cùng một chương, tiết diện này cũng được trích dẫn trong tham chiếu.
c) Nếu chúng xuất hiện trong một chương khác của cùng một Quyển, chương và tiết diện được trích dẫn.
d) Nếu chúng xuất hiện trong một Quyển khác, trước hết Quyển này được trích dẫn bằng nhan đề của nó.
Các Bản tóm tắt kết quả được trích dẫn bằng chữ R; như vậy, Lý thuyết tập hợp, R có nghĩa là “Bản tóm tắt kết quả của Lý thuyết tập hợp”.
