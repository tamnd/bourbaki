---
book: evt
book_title: Topological Vector Spaces
chapter: ""
chapter_title: ""
section: 0
section_title: TO THE READER
kind: reader
lang: vi
source: evt-i-v
pdf_pages: 0006-0008
extraction: ocr
statements: 0
exercises: 0
content_sha256: a57a4a9de0fb419b8842de363750e842d7c6b63702aa21ce62fa28188653ba3f
translated_from: content/en/evt/00_to_the_reader.md
source_content_sha256: 6cbc12e12abec8063cd6f21644b2bf89da7f708d54fa1d3ee86bbc47401085c9
translation_model: gpt-5-6-mini
translation_run: translate-vi-c2dead2e
glossary_version: 34
glossary_terms_sha256: 82e1fe5ae2443e8ee1c39dbf10cf1211defb9997d9a23c22bfac40a1cc4bbfdc
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## ĐỐI VỚI NGƯỜI ĐỌC

1. Bộ sách Các Nguyên lý của Toán học tiếp cận toán học ngay từ đầu và đưa ra các chứng minh đầy đủ. Về nguyên tắc, bộ sách không đòi hỏi người đọc phải có kiến thức toán học đặc biệt nào, mà chỉ cần một sự quen thuộc nhất định với lập luận toán học và một năng lực nhất định về tư duy trừu tượng. Tuy nhiên, bộ sách đặc biệt hướng tới những người có kiến thức tốt về ít nhất nội dung của một hoặc hai năm đầu của một khóa học toán học đại học.

2. Phương pháp trình bày mà chúng tôi lựa chọn là tiên đề hóa, và thông thường tiến hành từ cái tổng quát đến cái cụ thể. Những yêu cầu của việc chứng minh áp đặt lên nội dung môn học một trật tự được xác định chặt chẽ. Do đó, ích lợi của một số xem xét nhất định sẽ không hiện ra ngay đối với người đọc nếu người đó chưa có một kiến thức toán học tương đối rộng.

3. Bộ sách được chia thành các Quyển và mỗi Quyển thành các chương. Các Quyển đã được xuất bản, toàn bộ hoặc một phần, trong bản tiếng Pháp được liệt kê dưới đây. Khi có bản dịch tiếng Anh, nhan đề tiếng Anh tương ứng được nêu trong dấu ngoặc đơn. Trong toàn bộ tập sách, một tham chiếu chỉ bản tiếng Anh khi có sẵn, và bản tiếng Pháp trong các trường hợp khác.

LÝ THUYẾT TẬP HỢP (Theory of Sets)    được ký hiệu bởi E    (S)
Đại số (Algebra$^{(1)}$)                —                A    (A)
Tôpô Tổng quát (General Topology)      —                TG   (GT)
Hàm của một Biến thực                  —                FVR
Các Không gian Vectơ Tôpô (Topological Vector Spaces) —                EVT   (TVS)
Tích phân                                —                INT
Đại số Giao hoán (Commutative Algebra$^{(2)}$) —        AC    (CA)
Các Đa tạp Vi phân và Giải tích          —                VAR
Các Nhóm và Đại số Lie (Lie Groups and Lie Algebras$^{(3)}$) —        LIE   (LIE)
Các Lý thuyết Phổ                        —                TS

(1) Cho đến nay, chỉ các chương I đến III đã được dịch.
(2) Cho đến nay, chỉ các chương I đến VII đã được dịch.
(3) Cho đến nay, chỉ các chương I đến III đã được dịch.

Trong sáu quyển đầu tiên (theo thứ tự trên), mọi mệnh đề trong văn bản chỉ giả thiết là đã biết những kết quả đã được thảo luận trong cùng chương, hoặc trong các chương trước được sắp xếp như sau : S ; A, các chương I đến III ; GT, các chương I đến III ; A, từ chương IV trở đi ; GT, từ chương IV trở đi ; FVR ; EVT ; INT.

Từ Quyển thứ bảy trở đi, người đọc thường sẽ tìm thấy một chỉ dẫn chính xác về quan hệ lôgic của nó với các Quyển khác (sáu Quyển đầu tiên luôn được giả thiết là đã biết).

4. Tuy nhiên, đôi khi chúng tôi đã đưa vào văn bản những ví dụ liên quan đến các sự kiện mà người đọc có thể đã biết nhưng chưa được thảo luận trong bộ sách. Những ví dụ như vậy được đặt giữa hai dấu sao : *...*. Phần lớn độc giả chắc chắn sẽ nhận thấy rằng những ví dụ này sẽ giúp họ hiểu văn bản. Trong những trường hợp khác, các đoạn nằm giữa *...* đề cập đến những kết quả được thảo luận ở nơi khác trong Bộ sách. Chúng tôi hy vọng người đọc sẽ có thể kiểm tra rằng không có vòng luẩn quẩn nào xuất hiện.

5. Khuôn khổ lôgic của mỗi chương bao gồm các định nghĩa, các tiên đề và các định lý của chương đó. Đây là những phần chủ yếu cần được ghi nhớ để sử dụng về sau. Những kết quả ít quan trọng hơn và những kết quả có thể dễ dàng suy ra từ các định lý được gọi là « mệnh đề », « bổ đề », « hệ quả », « nhận xét », v.v. Những phần có thể bỏ qua trong lần đọc đầu tiên được in bằng cỡ chữ nhỏ. Một lời bình luận về một định lý đặc biệt quan trọng đôi khi xuất hiện dưới tên gọi « chú giải ».

Để tránh những sự lặp lại tẻ nhạt, đôi khi thuận tiện khi đưa vào các ký hiệu hoặc các từ viết tắt chỉ có hiệu lực trong một chương nhất định hoặc một tiết diện nhất định của một chương (chẳng hạn, trong một chương chỉ nghiên cứu các vành giao hoán, từ « vành » sẽ luôn có nghĩa là « vành giao hoán »). Các quy ước như vậy luôn được nêu rõ một cách tường minh, nói chung là ở đầu chương mà chúng xuất hiện.

6. Một số đoạn trong văn bản được thiết kế nhằm cảnh báo trước cho người đọc về những sai lầm nghiêm trọng. Những đoạn này được đánh dấu ở lề bằng ký hiệu ☡ (« khúc quanh nguy hiểm »).

7. Các Bài tập được thiết kế vừa để giúp người đọc tự kiểm tra rằng mình đã lĩnh hội văn bản, vừa để lưu ý họ đến những kết quả không có chỗ trong văn bản nhưng vẫn đáng quan tâm. Những bài tập khó nhất mang ký hiệu ¶.

8. Nhìn chung, chúng tôi đã tuân theo thuật ngữ được chấp nhận rộng rãi, ngoại trừ những trường hợp có những lý do xác đáng để đi lệch khỏi nó.

9. Chúng tôi đã đặc biệt cố gắng luôn sử dụng ngôn ngữ chính xác một cách chặt chẽ, mà không hy sinh tính đơn giản. Trong phạm vi có thể, chúng tôi đã chỉ ra trong văn bản những sự lạm dụng ngôn ngữ, bởi nếu không có chúng thì mọi văn bản toán học đều có nguy cơ trở nên câu nệ, thậm chí khó đọc.

10. Vì về nguyên tắc văn bản bao gồm sự trình bày giáo điều của một lý thuyết, nên nhìn chung nó không chứa các tham chiếu đến tài liệu. Các tài liệu tham khảo thư mục được tập hợp trong các Ghi chú Lịch sử. Thư mục theo sau mỗi ghi chú lịch sử nhìn chung chỉ chứa những cuốn sách và hồi ký nguyên bản có tầm quan trọng lớn nhất trong sự phát triển của lý thuyết đang được bàn luận. Nó không hề có ý định đầy đủ.

Đối với các bài tập, nói chung chúng tôi không thấy đáng để chỉ ra nguồn gốc của chúng, vì chúng được lấy từ nhiều nguồn khác nhau (các bài báo gốc, sách giáo khoa, các tuyển tập bài tập).

11. Trong Quyển hiện tại, các tham chiếu đến các định lý, tiên đề, định nghĩa, ... được đưa ra bằng cách trích dẫn lần lượt :

— Quyển sách (sử dụng chữ viết tắt được liệt kê trong Mục 3), chương và trang, nơi có thể tìm thấy chúng, khi tham chiếu đến ấn bản tiếng Pháp ;
— chỉ chương và trang khi tham chiếu đến Quyển sách hiện tại ;
— chương, đoạn và tiết diện khi tham chiếu đến ấn bản tiếng Anh.

Các Tóm tắt các Kết quả được trích dẫn bằng chữ cái R ; do đó Lý thuyết tập hợp, R có nghĩa là « Tóm tắt các Kết quả của lý thuyết tập hợp ».
