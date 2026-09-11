---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 8
section_title: Scales of sets. Structures
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 383-385
pdf_pages: 0388-0390
extraction: ocr
statements: 0
exercises: 0
content_sha256: 20d5085ecc0a37b24ffbe808aad7588a056e8a30087703855dfefe228333e65f
translated_from: content/en/ens/ER/08_s8_scales_of_sets_structures.md
source_content_sha256: 1729e7f56fb13a5cfb4b19ed30304bcfc4d735d7f99cdf7c9579aa41117e6f82
translation_model: gpt-5-6
translation_run: translate-vi-3b9d2523
glossary_version: 34
glossary_terms_sha256: 8160cda55c1a6988456ec1aed3c05b857c31b01a395101bddbe5505fdcf5efaa
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 8. CÁC THANG TẬP HỢP. CÁC CẤU TRÚC

1. Cho, chẳng hạn, ba tập hợp *phân biệt* E, F, G, ta có thể tạo thành từ chúng các tập hợp khác bằng cách lấy các tập hợp con của chúng, hoặc bằng cách lập tích của một trong chúng với chính nó, hoặc lại bằng cách lập tích của hai trong chúng lấy theo một thứ tự nhất định. Theo cách này ta thu được *mười hai* tập hợp mới. Nếu thêm các tập hợp này vào ba tập hợp ban đầu E, F, G, ta có thể lặp lại các phép toán tương tự trên mười lăm tập hợp này, bỏ qua những phép toán cho ta các tập hợp đã thu được; và cứ tiếp tục như vậy. Nói chung, bất kỳ một tập hợp nào thu được bởi thủ tục này (theo một lược đồ tường minh) được gọi là thuộc *thang tập hợp* trên E, F, G *làm cơ sở*.

Chẳng hạn, cho M, N, P là ba tập hợp của thang này, và cho $R\{x,y,z\}$ là một *quan hệ* giữa các phần tử tổng quát $x$, $y$, $z$ của M, N, P, tương ứng. Khi đó R xác định một tập con của $M \times N \times P$, do đó (qua một sự tương ứng chính tắc) một tập con của $(M \times N) \times P$, nghĩa là một phần tử của $\mathfrak{P}((M \times N) \times P)$. Như vậy, cho một *quan hệ* giữa các phần tử của một số tập hợp trong cùng một thang chính là cho một *phần tử* của một tập hợp khác trong thang. Tương tự, cho một ánh xạ của M vào N, chẳng hạn, tương đương (bằng cách xét đồ thị của ánh xạ này) với việc cho một tập con của $M \times N$, nghĩa là một phần tử của $\mathfrak{P}(M \times N)$, lại là một tập hợp trong thang. Cuối cùng, cho hai phần tử (chẳng hạn) của M tương đương với việc cho một phần tử duy nhất trong tập hợp tích $M \times M$.

Như vậy, việc được cho một số phần tử nhất định của các tập hợp trong một thang, các quan hệ giữa các phần tử tổng quát của các tập hợp này, và các ánh xạ của các tập con của một số tập hợp nhất định này vào các tập hợp khác, xét cho cùng trong phân tích cuối cùng, đều quy về việc được cho một *phần tử duy nhất* của một trong các tập hợp trong thang.

2. Trước đây (§6) ta đã nói rằng một phần tử C của tập hợp $\mathfrak{P}(E \times E)$ xác định một cấu trúc thứ tự trên E nếu nó có các tính chất (a) $C \circ C \subset C$ và (b)

$$C \cap C^{-1} = \Delta.$$

Nói chung, xét một tập hợp M trong một thang tập hợp có cơ sở gồm, chẳng hạn, ba tập hợp E, F, G. Cho trước một số tính chất được phát biểu tường minh của một phần tử tổng quát của M, và gọi T là giao của các tập con của M được xác định bởi các tính chất này. Một phần tử $\sigma$ của T được gọi là xác định một *cấu trúc* thuộc *loài* T trên E, F, G. Do đó các cấu trúc thuộc loài T được đặc trưng bởi lược đồ tạo thành M từ E, F, G, và bởi các tính chất xác định T, được gọi là các *tiên đề* của các cấu trúc này. Ta đặt một tên riêng cho tất cả các cấu trúc cùng một loài. Mọi mệnh đề là một hệ quả của mệnh đề “$\sigma \in T$” (nghĩa là của các tiên đề xác định T) được gọi là thuộc về *lý thuyết* của các cấu trúc thuộc loài T; chẳng hạn, các mệnh đề được phát biểu trong § 6 thuộc về lý thuyết của các cấu trúc của các tập hợp có thứ tự.

Trong ví dụ cuối, các tiên đề có thể được phát biểu cho một tập hợp cơ sở E hoàn toàn tùy ý. Do đó ta đặt cùng một tên cho các cấu trúc thỏa mãn các tiên đề này, không phụ thuộc vào tập hợp mà trên đó chúng được định nghĩa; và các mệnh đề suy ra từ các tiên đề này đúng trong mọi tập hợp, bởi vì cách phát biểu của chúng không liên quan đến bất kỳ tính chất đặc biệt nào của tập hợp E. Những nhận xét như vậy được áp dụng bất cứ khi nào các tiên đề có bản chất này [^1].

Thông thường nhất, khi một thang được sử dụng với một cơ sở gồm nhiều tập hợp E, F, G, một trong các tập hợp này, chẳng hạn E, đóng một vai trò chi phối trong các cấu trúc đang xét. Vì vậy, do lạm dụng ngôn ngữ, người ta nói rằng các cấu trúc này được định nghĩa trong tập hợp E, còn F và G được xem là các tập hợp phụ trợ.

Cuối cùng, để đơn giản hóa ngôn ngữ, người ta thường đặt một tên riêng cho một tập hợp đã được trang bị một cấu trúc thuộc một loài xác định. Vì vậy ta nói về một *tập hợp có thứ tự*, và trong các phần sau của chuỗi này ta sẽ định nghĩa các khái niệm *nhóm, vành, trường, không gian tôpô, không gian đồng đều*, v.v., tất cả đều là những từ chỉ các tập hợp được trang bị những cấu trúc nhất định.

3. Xét các cấu trúc cùng một loài T, trong đó T là một tập con của một tập hợp M trong một thang tập hợp. Nếu ta thêm các “tiên đề” mới vào các tiên đề xác định T, hệ các tiên đề thu được như vậy xác định một tập con U của M, được chứa trong T. Các cấu trúc thuộc loài U được gọi là *phong phú hơn* các cấu trúc thuộc loài T. Chẳng hạn, các cấu trúc của các tập hợp *được sắp thứ tự toàn phần* phong phú hơn các cấu trúc của các tập hợp có thứ tự, bởi vì phần tử C của $\mathfrak{P}(E \times E)$ xác định một cấu trúc như vậy phải thỏa mãn tiên đề bổ sung

$$C \cup \overline{C}^{-1} = E \times E.$$

4. Cho M, M′ là hai tập hợp trong cùng một thang, chẳng hạn với E, F, G làm cơ sở. Cho T là một tập con của M và T′ là một tập con của M′, mỗi tập được xác định bởi một số tiên đề được phát biểu tường minh. Bất cứ khi nào ta có thể xác định tường minh một *ánh xạ một-một* của T lên T′, ta xem hai phần tử $\sigma \in T$, $\sigma' \in T'$ tương ứng với nhau qua ánh xạ này, là xác định *cùng một cấu trúc* trên E, F, G; và các hệ tiên đề xác định T và T′ được gọi là *tương đương*.

Các *cấu trúc tôpô* cung cấp một ví dụ về tình huống này; chúng có thể được định nghĩa bằng nhiều hệ tiên đề tương đương, trong đó có hai hệ đặc biệt hữu ích (xem *Tôpô đại cương*, Chương I, § 1).

5. Cho E, F, G là ba tập hợp, và giả sử ta được cho các ánh xạ *song ánh* tương ứng của E, F, G lên ba tập hợp khác E′, F′, G′. Vì ta biết cách định nghĩa *các mở rộng chính tắc* của các ánh xạ song ánh lên các tập hợp con (§ 2, no. 9) và lên các tập tích (§ 3, no. 14), nên ta có thể định nghĩa, từng bước một, *mở rộng* của các song ánh đã cho lên hai tập hợp M, M′ lần lượt được xây dựng theo *cùng một lược đồ* trong thang các tập hợp dựa trên E, F, G và trong thang dựa trên E′, F′, G′. Gọi $f$ là song ánh của M lên M′ thu được như vậy. Nếu $\sigma$ là một cấu trúc trên E, F, G, là một phần tử của một tập con T của M, ta nói rằng $f(\sigma)$ là cấu trúc thu được bằng cách *vận chuyển* cấu trúc $\sigma$ lên E′, F′, G′ nhờ các song ánh đã cho của E lên E′, F lên F′, G lên G′. Mọi mệnh đề liên quan đến cấu trúc $\sigma$ trên E, F, G đều dẫn đến (bằng cách sử dụng các mở rộng thích hợp) một mệnh đề liên quan đến cấu trúc $f(\sigma)$ trên E′, F′, G′.

Ngược lại, một cấu trúc $\sigma$ trên E, F, G và một cấu trúc $\sigma'$ trên E′, F′, G′ được gọi là *đẳng cấu* nếu $\sigma'$ có thể thu được bằng cách *vận chuyển* $\sigma$ nhờ các song ánh tương ứng của E, F, G lên E′, F′, G′; khi đó các ánh xạ này được gọi là tạo thành một *đẳng cấu* của $\sigma$ lên $\sigma'$.

Khi ta xét các cấu trúc trên một tập hợp duy nhất E, song ánh của E lên E′ vận chuyển $\sigma$ thành $\sigma'$ cũng được gọi là một *đẳng cấu của tập hợp E, được trang bị cấu trúc $\sigma$, lên tập hợp E′, được trang bị cấu trúc $\sigma'$.*

Ánh xạ này cũng được gọi là một *đẳng cấu* khi F và G là hai tập hợp phụ trợ, và các song ánh đối với hai tập hợp này là các ánh xạ *đồng nhất* của F và G lên chính chúng.

Một *đẳng cấu* của một tập hợp E, được trang bị một cấu trúc $\sigma$, lên chính nó được gọi là một *tự đẳng cấu*.

Khi tồn tại một *đẳng cấu* của một tập hợp E, được trang bị một cấu trúc $\sigma$, lên một tập hợp E′, được trang bị một cấu trúc $\sigma'$, thường thuận tiện khi *đồng nhất* E với E′, tức là gán *cùng một tên* cho một phần tử của một tập hợp M trong thang dựa trên E và cho phần tử là ảnh của nó dưới mở rộng thích hợp của $f$ lên tập hợp M.

6. Cho một hệ các tiên đề định nghĩa một tập con T của một tập hợp M trong một thang các tập hợp, trước khi nói đến các cấu trúc *thỏa mãn* các tiên đề này, ta phải bảo đảm rằng tập hợp T là *không nhất thiết rỗng*; nếu không, các tiên đề sẽ được gọi là *mâu thuẫn* hoặc *không nhất quán*.

7. Có thể xảy ra rằng một hệ các tiên đề định nghĩa một cấu trúc trên một tập hợp có thể được phát biểu đối với một tập hợp tùy ý, nhưng khi xét hai cấu trúc thỏa mãn các tiên đề này và được định nghĩa trên hai tập hợp phân biệt E, F, ta nhận thấy từ các tiên đề rằng các cấu trúc này (nếu tồn tại) nhất thiết *đẳng cấu* (điều này đặc biệt kéo theo rằng E và F *cùng lực lượng*). Khi đó, lý thuyết về các cấu trúc thỏa mãn các tiên đề này được gọi là *đơn trị*; ngược lại, chúng được gọi là *đa trị*.

Lý thuyết về các số nguyên, lý thuyết về các số thực và hình học Euclid cổ điển là các lý thuyết đơn trị; lý thuyết về các tập hợp có thứ tự, lý thuyết nhóm và tôpô là các lý thuyết đa trị. Việc nghiên cứu các lý thuyết đa trị là đặc điểm nổi bật nhất phân biệt toán học hiện đại với toán học cổ điển.

[^1]: Độc giả có thể đã nhận thấy rằng các chỉ dẫn được đưa ra ở đây còn khá mơ hồ; chúng không nhằm mục đích nào khác ngoài tính chất gợi ý, và quả thực dường như khó có thể phát biểu các định nghĩa tổng quát và chính xác cho các cấu trúc nằm ngoài khuôn khổ của toán học hình thức (xem Chương IV).
