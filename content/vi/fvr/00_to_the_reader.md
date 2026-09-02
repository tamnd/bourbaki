---
book: fvr
book_title: Functions of a Real Variable
chapter: ""
chapter_title: ""
section: 0
section_title: TO THE READER
kind: reader
lang: vi
source: fvr-i-vii
pdf_pages: 0006-0008
extraction: ocr
statements: 0
exercises: 0
content_sha256: 8af9a45f8ae544fa3dfedb5354bfcd4dde385e34ccb1fa8c180b92238208ca77
translated_from: content/en/fvr/00_to_the_reader.md
source_content_sha256: 868eb46c0a2e26838ba29aac207a93969e652bc965912375017101eda1b82550
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-09daac70
glossary_version: 34
glossary_terms_sha256: 6cacaf7bf248a4a0952c183c337f4b540e4b6c61fe9b6f5fd24d2f2e437633d3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## GỬI ĐỘC GIẢ

1. Bộ sách Các Yếu tố của Toán học bắt đầu với toán học từ đầu, và đưa ra các chứng minh đầy đủ. Về nguyên tắc, bộ sách không đòi hỏi độc giả có một kiến thức toán học đặc biệt nào, mà chỉ cần một sự quen thuộc nhất định với lập luận toán học và một khả năng nhất định về tư duy trừu tượng. Tuy nhiên, nó đặc biệt hướng đến những người có một kiến thức tốt về ít nhất nội dung của một hoặc hai năm đầu của một khóa học toán học đại học.

2. Phương pháp trình bày mà chúng tôi đã chọn là tiên đề hóa, và thông thường đi từ tổng quát đến cụ thể. Những yêu cầu của chứng minh áp đặt một thứ tự được xác định nghiêm ngặt lên nội dung. Do đó, ích lợi của một số xem xét có thể không ngay lập tức hiển nhiên đối với độc giả cho đến các chương sau, trừ khi người đó đã có một kiến thức toán học khá rộng.

3. Bộ sách được chia thành các Quyển và mỗi Quyển thành các chương. Các Quyển đã được xuất bản, toàn bộ hoặc một phần, trong ấn bản tiếng Pháp, được liệt kê dưới đây. Khi có một bản dịch tiếng Anh, tên tiếng Anh tương ứng được nêu trong ngoặc đơn. Trong toàn bộ tập sách, một tham chiếu chỉ ra ấn bản tiếng Anh khi có, và nếu không thì chỉ ra ấn bản tiếng Pháp.

Théorie des Ensembles (LÝ THUYẾT TẬP HỢP)                     ký hiệu bởi   E     (Set Theory)
Algèbre (Đại số) [^1]                                                     —   A     (Alg)
Topologie Générale (Tôpô tổng quát)                                      —   TG    (Gen. Top.)
Fonctions d’une Variable Réelle
(Hàm của một biến thực) [^2]                                             —   FVR   (FRV)
Espaces Vectoriels Topologiques
(Không gian vectơ tôpô)                                                   —   EVT   (Top. Vect. Sp.)
Intégration                                                               —   INT
Algèbre Commutative (Đại số giao hoán) [^3]                              —   AC    (Comm. Alg.)
Variétés Différentielles et Analytiques                                  —   VAR
Groupes et Algèbres de Lie
(Nhóm và đại số Lie) [^4]                                                —   LIE   (LIE)
Théories Spectrales                                                       —   TS

Trong sáu Quyển đầu tiên (theo thứ tự trên đây), mọi mệnh đề trong văn bản chỉ giả thiết đã biết những kết quả đã được thảo luận trước đó trong cùng

[^1]: Cho đến nay, chỉ các chương I đến VII đã được dịch.
[^2]: Tập này!
[^3]: Cho đến nay, chỉ các chương I đến VII đã được dịch.
[^4]: Cho đến nay, chỉ các chương I đến III đã được dịch.

chương, hoặc trong các chương trước theo thứ tự sau: E ; A, các chương I đến III ; TG, các chương I đến III ; A, từ chương IV trở đi ; TG, từ chương IV trở đi ; FVR ; EVT ; INT.

Từ Quyển thứ bảy trở đi, độc giả thường sẽ tìm thấy một chỉ dẫn chính xác về quan hệ lôgic của nó với các Quyển khác (sáu Quyển đầu tiên luôn được giả thiết là đã biết).

4. Tuy nhiên, đôi khi chúng tôi đã đưa vào văn bản các ví dụ tham chiếu đến những sự kiện mà độc giả có thể đã biết nhưng chưa được thảo luận trong bộ sách. Những ví dụ như vậy được đặt giữa hai dấu sao : \* . . . \* Hầu hết độc giả chắc chắn sẽ thấy rằng những ví dụ này sẽ giúp họ hiểu văn bản. Trong các trường hợp khác, những đoạn nằm giữa \* . . . \* tham chiếu đến các kết quả được thảo luận ở nơi khác trong bộ sách. Chúng tôi hy vọng độc giả sẽ có thể kiểm chứng sự vắng mặt của mọi vòng tròn luẩn quẩn.

5. Khung lôgic của mỗi chương bao gồm các định nghĩa, các tiên đề và các định lý của chương đó. Đây là những phần chủ yếu cần được ghi nhớ để sử dụng về sau. Những kết quả ít quan trọng hơn và những kết quả có thể dễ dàng suy ra từ các định lý được gọi là “mệnh đề”, “bổ đề”, “hệ quả”, “nhận xét”, v.v. Những kết quả có thể bỏ qua khi đọc lần đầu được in bằng kiểu chữ nhỏ. Một chú giải về một định lý đặc biệt quan trọng đôi khi xuất hiện dưới tên “chú giải”.

Để tránh những sự lặp lại tẻ nhạt, đôi khi thuận tiện khi đưa vào các ký hiệu hoặc các viết tắt chỉ có hiệu lực trong một chương nhất định hoặc một tiết diện nhất định của một chương (chẳng hạn, trong một chương chỉ xét các vành giao hoán, từ “vành” sẽ luôn có nghĩa là “vành giao hoán”). Những quy ước như vậy luôn được nêu một cách tường minh, nói chung là ở đầu chương nơi chúng xuất hiện.

6. Một số đoạn được thiết kế để cảnh báo trước cho độc giả về những sai lầm nghiêm trọng.

☡

Những đoạn này được đánh dấu ở lề bằng ký hiệu (“khúc quanh nguy hiểm”).

7. Các Bài tập được thiết kế vừa để giúp độc giả tự thỏa mãn rằng mình đã lĩnh hội văn bản, vừa để đưa đến sự chú ý của độc giả những kết quả không có chỗ trong văn bản nhưng vẫn có ích. Những bài tập khó nhất mang dấu ¶.

8. Nói chung chúng tôi đã tuân theo thuật ngữ được chấp nhận rộng rãi, ngoại trừ những trường hợp có những lý do chính đáng để đi lệch khỏi nó.

9. Chúng tôi đã đặc biệt cố gắng luôn sử dụng ngôn ngữ đúng đắn một cách nghiêm ngặt, mà không hy sinh sự đơn giản. Trong chừng mực có thể, chúng tôi đã lưu ý trong văn bản đến những sự lạm dụng ngôn ngữ, vì nếu không có chúng thì mọi văn bản toán học đều có nguy cơ trở nên kiểu cách, chưa kể đến không thể đọc được.

10. Vì về nguyên tắc văn bản bao gồm một sự trình bày giáo điều của một lý thuyết, nói chung nó không chứa các tham chiếu đến tài liệu. Các tài liệu thư mục được tập hợp trong các Ghi chú lịch sử. Tài liệu thư mục đi sau mỗi ghi chú lịch sử nói chung chỉ chứa những sách và hồi ký nguyên bản có tầm quan trọng lớn nhất trong sự phát triển của lý thuyết đang được xét. Nó không hề giả định là đầy đủ.

Đối với các bài tập, nói chung chúng tôi không cho rằng đáng để chỉ ra nguồn gốc của chúng, vì chúng được lấy từ nhiều nguồn khác nhau (các bài báo nguyên gốc, sách giáo khoa, các tuyển tập bài tập).

11. Trong Quyển hiện tại, các tham chiếu đến các định lý, tiên đề, định nghĩa, . . . được đưa ra bằng cách lần lượt trích dẫn:
– Quyển (dùng chữ viết tắt được liệt kê trong Tiết 3), chương và trang, nơi có thể tìm thấy chúng;
– chỉ chương và trang khi tham chiếu đến Quyển hiện tại.
    Các Bản tóm tắt các kết quả được trích dẫn bằng chữ R; do đó Set Theory, R có nghĩa là "Bản tóm tắt các kết quả của lý thuyết tập hợp".
