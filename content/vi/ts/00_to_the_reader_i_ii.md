---
book: ts
book_title: Théories spectrales
chapter: ""
chapter_title: ""
section: 0
section_title: MODE D’EMPLOI
kind: reader
lang: vi
source: ts-i-ii-fr
pdf_pages: 0007-0010
extraction: native
statements: 0
exercises: 0
content_sha256: 29f0be9e3181a488ab060a3263c0e3bffe3d6920d1fa401ea4b4ada2b5fcd791
translated_from: content/en-mt/ts/00_to_the_reader_i_ii.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 039d51c6f68f475224d8710792136ef6e796e5f161ec55a7cf2f0a23c93e3849
translation_model: gpt-5-6-mini
translation_run: translate-vi-50755e39
glossary_version: 34
glossary_terms_sha256: cf3aae12009e5e7ba87dd2aa9430639396e2ebbbbd4bf2517ea5d6f17885f631
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

1. Bộ sách trình bày toán học từ những bước đầu và đưa ra các chứng minh đầy đủ. Do đó, về nguyên tắc, việc đọc sách không đòi hỏi một kiến thức toán học đặc biệt nào, mà chỉ cần một sự quen thuộc nhất định với cách suy luận toán học và một khả năng trừu tượng hóa nhất định. Tuy nhiên, bộ sách đặc biệt dành cho những độc giả đã có ít nhất một kiến thức tốt về các môn học được giảng dạy trong một hoặc hai năm đầu ở đại học.

2. Phương pháp trình bày được sử dụng là tiên đề hóa và thường đi từ tổng quát đến cụ thể. Những yêu cầu của việc chứng minh đòi hỏi rằng các chương, về nguyên tắc, phải nối tiếp nhau theo một thứ tự lôgic được xác định chặt chẽ. Vì vậy, ích lợi của một số xem xét chỉ xuất hiện đối với độc giả khi đọc các chương sau, trừ khi họ đã có những kiến thức đủ rộng.

3. Bộ sách được chia thành các Quyển và mỗi Quyển thành các chương. Các Quyển hiện đã xuất bản, toàn bộ hoặc một phần, là các Quyển sau:

Lý thuyết tập hợp ký hiệu bởi E

Đại số — A

Tôpô tổng quát — TG

Hàm của một biến thực — FVR

Không gian vectơ tôpô — EVT

Tích phân — INT

Đại số giao hoán — AC

Đa tạp khả vi và giải tích — VAR

Nhóm Lie và đại số Lie — LIE

Các lý thuyết phổ — TS

Tôpô đại số — TA

vii

Trong sáu Quyển đầu tiên (theo thứ tự đã chỉ ra ở trên), mỗi mệnh đề chỉ sử dụng các định nghĩa và kết quả đã được nêu trước đó trong chương hiện tại hoặc trong các chương trước theo thứ tự sau: E; A, các chương I đến III; TG, các chương I đến III; A, các chương IV và tiếp theo; TG, các chương IV và tiếp theo; FVR; EVT; INT. Bắt đầu từ Quyển thứ bảy, độc giả sẽ tìm thấy, khi thích hợp, ở đầu mỗi Quyển hoặc chương, một chỉ dẫn chính xác về các Quyển hoặc chương khác được sử dụng (sáu Quyển đầu tiên luôn được giả thiết là đã biết).

4. Tuy nhiên, một vài đoạn là ngoại lệ đối với các quy tắc trước đó. Chúng được đặt giữa hai dấu sao$:*$. . . . Trong một số

$$
*
$$

trường hợp, đó chỉ là vấn đề tạo thuận lợi cho việc hiểu văn bản bằng những ví dụ quy chiếu đến các sự kiện mà độc giả có thể đã biết từ các nguồn khác. Đôi khi cũng vậy, không chỉ các kết quả được giả thiết là đã biết trong toàn bộ chương hiện tại được sử dụng, mà cả các kết quả đã được chứng minh ở nơi khác trong bộ sách cũng được sử dụng. Các đoạn này sẽ được sử dụng tự do trong những phần giả thiết đã biết các chương mà chúng được đưa vào và các chương mà chúng quy chiếu đến. Chúng tôi hy vọng độc giả sẽ có thể kiểm tra rằng không có vòng lặp luẩn quẩn nào.

5. Một số Quyển (đã xuất bản hoặc đang chuẩn bị) có kèm theo các tập kết quả. Các tập này chứa những phần cốt yếu của các định nghĩa và kết quả của Quyển, nhưng không có chứng minh nào.

6. Khung lôgic của mỗi chương được cấu thành bởi các định nghĩa, các tiên đề và các định lý của chương đó; đây là những điều chủ yếu cần ghi nhớ để phục vụ cho những gì tiếp theo. Các kết quả ít quan trọng hơn, hoặc có thể dễ dàng tìm lại từ các định lý, được đưa dưới tên gọi «mệnh đề», «bổ đề», «hệ quả», «nhận xét»; v.v.; những kết quả có thể bỏ qua khi đọc lần đầu được in bằng chữ nhỏ. Dưới tên gọi «chú giải», đôi khi người ta sẽ tìm thấy một lời bình luận về một định lý đặc biệt quan trọng.

Để tránh những sự lặp lại gây mệt mỏi, đôi khi người ta quy ước đưa vào một số ký hiệu hoặc một số chữ viết tắt chỉ có giá trị trong một chương hoặc một đoạn duy nhất (chẳng hạn, trong một chương mà mọi vành đều giao hoán, có thể quy ước rằng từ “vành” luôn có nghĩa là “vành giao hoán”). Những quy ước như vậy được nêu rõ ở đầu chương hoặc đoạn mà chúng áp dụng.

7. Một số đoạn nhằm đề phòng cho độc giả chống lại những sai lầm nghiêm trọng mà họ có nguy cơ mắc phải; các đoạn này được đánh dấu ở lề bằng ký hiệu («chỗ ngoặt nguy hiểm»).

8. Các bài tập nhằm một mặt cho phép độc giả kiểm tra rằng mình đã lĩnh hội tốt văn bản; mặt khác giúp họ biết đến những kết quả không có chỗ trong văn bản; các bài khó nhất được đánh dấu bằng ký hiệu $\P$.

9. Thuật ngữ được sử dụng trong bộ sách này đã nhận được sự chú ý đặc biệt. Người ta cố gắng không bao giờ rời khỏi thuật ngữ đã được chấp nhận nếu không có những lý do hết sức nghiêm túc.

10. Người ta đã cố gắng sử dụng, không hy sinh sự đơn giản của cách trình bày, một ngôn ngữ hoàn toàn chính xác. Trong phạm vi có thể, những lạm dụng về ngôn ngữ hoặc ký hiệu, nếu không có chúng thì mọi văn bản toán học có nguy cơ trở nên kiểu cách và thậm chí khó đọc, đã được chỉ ra trong quá trình trình bày.

11. Vì văn bản dành cho việc trình bày giáo điều một lý thuyết, người ta chỉ tìm thấy rất ít các tài liệu tham khảo thư mục; đôi khi chúng được nhóm lại trong các Ghi chú lịch sử. Thư mục theo sau mỗi Ghi chú này thường chỉ gồm các sách và hồi ký nguyên bản có tầm quan trọng nhất trong sự phát triển của lý thuyết được xét; nó hoàn toàn không nhằm mục đích đầy đủ.

Đối với các bài tập, nhìn chung người ta không thấy cần thiết phải chỉ ra nguồn gốc của chúng, vì nguồn gốc đó rất đa dạng (các hồi ký nguyên bản, các công trình giáo khoa, các tuyển tập bài tập).

12. Trong ấn bản mới, các tham chiếu đến các định lý, tiên đề, định nghĩa, nhận xét, v.v. về nguyên tắc được đưa ra bằng cách lần lượt chỉ ra Quyển (bằng chữ viết tắt tương ứng với nó trong danh sách đã cho ở số $^o3$), chương và trang nơi chúng xuất hiện. Bên trong cùng một Quyển, việc nhắc đến Quyển đó được bỏ đi; chẳng hạn, trong Quyển Đại số,

E, III, p. 32, cor. 3

chỉ đến hệ quả 3 xuất hiện trong Sách về Lý thuyết tập hợp, chương III, trang 32 của chương này;

II, p. 24, mệnh đề 17

chỉ đến mệnh đề 17 của Sách về Đại số, chương II, trang 24 của chương này.

Các tập kết quả được ký hiệu bằng chữ R; chẳng hạn: EVT, R có nghĩa là "tập kết quả của Sách về Các không gian vectơ tôpô".

Vì một số Sách sẽ được xuất bản sau trong ấn bản mới, các tham chiếu đến các Sách này được thực hiện bằng cách chỉ ra lần lượt Sách, chương, đoạn và số nơi kết quả được xét sẽ xuất hiện; chẳng hạn:

AC, III, § 4, n$^o5$, hệ quả của mệnh đề 6.
