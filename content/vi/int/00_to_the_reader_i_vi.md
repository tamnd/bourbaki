---
book: int
book_title: Integration
chapter: ""
chapter_title: ""
section: 0
section_title: TO THE READER
kind: reader
lang: vi
source: int-i-vi
pdf_pages: 0006-0008
extraction: ocr
statements: 0
exercises: 0
content_sha256: 977d8269c528b5452ee43971a27a9cb969c050f1d7b4de4d2f1c8509f03c9215
translated_from: content/en/int/00_to_the_reader_i_vi.md
source_content_sha256: 0b7b4874543c4b1c022753df5b3549321332349ffebf20695d43d3017ad5a5da
translation_model: gpt-5-6-mini
translation_run: translate-vi-57bc4cd2
glossary_version: 34
glossary_terms_sha256: 1311e98de6b1255f8d645b350b899336750b804e29513ae49f4a6c49af3fab13
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## DÀNH CHO ĐỘC GIẢ

1. Bộ Các Yếu tố của Toán học trình bày toán học ngay từ những khởi đầu của nó, và đưa ra các chứng minh đầy đủ. Về nguyên tắc, bộ sách không đòi hỏi người đọc phải có bất kỳ kiến thức đặc biệt nào về toán học, mà chỉ cần một sự quen thuộc nhất định với lập luận toán học và một khả năng nhất định về tư duy trừu tượng. Tuy nhiên, bộ sách đặc biệt hướng tới những người có kiến thức tốt về ít nhất nội dung của một hoặc hai năm đầu của một khóa học toán học đại học.

2. Phương pháp trình bày mà chúng tôi đã lựa chọn là tiên đề, và thông thường tiến hành từ cái tổng quát đến cái cụ thể. Những yêu cầu của việc chứng minh áp đặt một trật tự được xác định chặt chẽ lên nội dung môn học. Do đó, tính hữu ích của một số xem xét nhất định sẽ không hiển nhiên ngay lập tức đối với người đọc, trừ khi người đó đã có một kiến thức toán học khá rộng.

3. Bộ sách được chia thành các Quyển, và mỗi Quyển thành các chương. Các Quyển đã được xuất bản, toàn bộ hoặc một phần, trong ấn bản tiếng Pháp, được liệt kê dưới đây. Khi có bản dịch tiếng Anh, nhan đề tiếng Anh tương ứng được nêu trong dấu ngoặc đơn. Trong toàn bộ tập sách, một tham chiếu chỉ đến ấn bản tiếng Anh khi có sẵn, và nếu không thì đến ấn bản tiếng Pháp.

Lý thuyết tập hợp (Theory of Sets) được ký hiệu bởi E (S)
Đại số (Algebra) — A (A)
Tôpô tổng quát (General Topology) — TG (GT)
Hàm của một biến thực (Functions of a Real Variable) — FVR (FRV)
Không gian vectơ tôpô (Topological Vector Spaces) — EVT (TVS)
Tích phân (Integration) — INT (INT)
Đại số giao hoán (Commutative Algebra) — AC (CA)
Đa tạp vi phân và giải tích — VAR
Nhóm và đại số Lie (Lie Groups and Lie Algebras) — LIE (LIE)
Các lý thuyết phổ — TS

Trong sáu Quyển đầu tiên (theo thứ tự trên), mọi mệnh đề trong văn bản chỉ giả sử đã biết những kết quả đã được thảo luận trong cùng một chương, hoặc trong các chương trước được sắp xếp như sau: S; A, các Chương I đến III; GT, các Chương I đến III; A, từ Chương IV trở đi; GT, từ Chương IV trở đi; FRV; TVS; INT.

Từ Quyển thứ bảy trở đi, độc giả thường sẽ tìm thấy một chỉ dẫn chính xác về quan hệ lôgic của nó với các Quyển khác (sáu Quyển đầu tiên luôn được giả sử là đã biết).

4. Tuy nhiên, đôi khi chúng tôi đã đưa vào văn bản các ví dụ đề cập đến những sự kiện mà người đọc có thể đã biết nhưng chưa được thảo luận trong bộ sách. Những ví dụ như vậy được đặt giữa hai dấu sao: *...*. Hầu hết người đọc chắc chắn sẽ thấy rằng các ví dụ này giúp họ hiểu văn bản. Trong những trường hợp khác, các đoạn nằm giữa *...* đề cập đến những kết quả được thảo luận ở nơi khác trong bộ sách. Chúng tôi hy vọng rằng người đọc sẽ có thể kiểm tra sự không tồn tại của bất kỳ vòng lặp luẩn quẩn nào.

5. Khuôn khổ logic của mỗi chương bao gồm các định nghĩa, các tiên đề và các định lý của chương. Đây là những phần chủ yếu cần được ghi nhớ để sử dụng về sau. Các kết quả ít quan trọng hơn và những kết quả có thể dễ dàng suy ra từ các định lý được gắn nhãn là "mệnh đề", "bổ đề", "hệ quả", "nhận xét", v.v. Những kết quả có thể được bỏ qua trong lần đọc đầu tiên được in bằng cỡ chữ nhỏ. Một lời bình luận về một định lý đặc biệt quan trọng đôi khi xuất hiện dưới tên "scholium".

Để tránh những sự lặp lại tẻ nhạt, đôi khi thuận tiện đưa vào các ký hiệu hoặc các chữ viết tắt chỉ có hiệu lực trong một chương nhất định hoặc một tiết diện nhất định của một chương (chẳng hạn, trong một chương chỉ xét các vành giao hoán, từ "vành" sẽ luôn có nghĩa là "vành giao hoán"). Các quy ước như vậy luôn được nêu rõ tường minh, nói chung ở đầu chương mà chúng xuất hiện.

6. Một số đoạn trong văn bản được thiết kế để cảnh báo trước cho người đọc về những sai lầm nghiêm trọng. Các đoạn này được đánh dấu ở lề bằng ký hiệu ("khúc cua nguy hiểm").

7. Các Bài tập được thiết kế vừa để giúp người đọc tự kiểm tra rằng mình đã lĩnh hội văn bản, vừa để đưa đến sự chú ý của họ những kết quả không có chỗ trong văn bản nhưng vẫn đáng quan tâm. Những bài tập khó nhất mang ký hiệu ¶.

8. Nhìn chung, chúng tôi đã tuân theo thuật ngữ được chấp nhận rộng rãi, ngoại trừ những trường hợp có những lý do chính đáng để đi lệch khỏi nó.

9. Chúng tôi đã đặc biệt cố gắng luôn sử dụng ngôn ngữ chính xác một cách nghiêm ngặt, mà không hy sinh tính đơn giản. Trong chừng mực có thể, chúng tôi đã chỉ ra trong văn bản những sự lạm dụng ngôn ngữ, bởi nếu thiếu chúng thì bất kỳ văn bản toán học nào cũng có nguy cơ trở nên kiểu cách, nếu không muốn nói là không thể đọc được.

10. Vì về nguyên tắc văn bản bao gồm sự trình bày giáo điều của một lý thuyết, nên nhìn chung nó không chứa các tham chiếu đến tài liệu. Các tham chiếu thư mục được tập hợp trong các Ghi chú Lịch sử. Thư mục theo sau mỗi ghi chú lịch sử nhìn chung chỉ chứa những cuốn sách và hồi ký nguyên bản có tầm quan trọng lớn nhất trong sự phát triển của lý thuyết đang được thảo luận. Nó không hề có ý định đạt đến tính đầy đủ dưới bất kỳ hình thức nào.

Đối với các bài tập, nói chung chúng tôi không cho rằng đáng để chỉ ra nguồn gốc của chúng, vì chúng được lấy từ nhiều nguồn khác nhau (các bài báo gốc, sách giáo khoa, các tập bài tập).

11. Các tham chiếu đến một phần của bộ sách này được đưa ra như sau: a) Nếu tham chiếu đến các định lý, tiên đề hoặc định nghĩa được trình bày trong cùng một mục (\S), chúng được dẫn bằng số của chúng. b) Nếu chúng xuất hiện trong một mục khác của cùng một chương, mục này cũng được nêu trong tham chiếu. c) Nếu chúng xuất hiện trong một chương khác của cùng một Quyển, chương và mục được nêu. d) Nếu chúng xuất hiện trong một Quyển khác, Quyển đó được nêu trước tiên, bằng chữ viết tắt của nhan đề của nó.

Các Bản tóm tắt các kết quả được trích dẫn bởi chữ cái R; do đó S, R có nghĩa là "Bản tóm tắt các kết quả của Lý thuyết tập hợp".
