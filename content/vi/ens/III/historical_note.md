---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 255-257
pdf_pages: 0261-0263
extraction: ocr
statements: 0
exercises: 0
content_sha256: abd408c359e17994ae74e832bebce933458fbba29d022c0932d3276d445dd858
translated_from: content/en/ens/III/historical_note.md
source_content_sha256: 35c7fafb7fcf59df7cdf3b82fc528a165d03d9d6a7897b9d7068e48d10fcf9a5
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-8c7bd20d
glossary_version: 34
glossary_terms_sha256: 27a7d557a959a9ca8eccab52674a4320dfdbd04aecc4831a65c2e8c55749bc5b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Chương III, § 5)

(Các số trong ngoặc vuông chỉ đến thư mục ở cuối Ghi chú này.)

Sự tiến triển của các ý tưởng liên quan đến các khái niệm số nguyên và số lực lượng không thể tách rời khỏi lịch sử của lý thuyết tập hợp và logic toán học, mà về phần này người đọc được dẫn đến Ghi chú lịch sử sau Chương IV. Mục đích của Ghi chú này là chỉ ra một cách vắn tắt một số sự kiện nổi bật trong lịch sử của phép đếm số và "giải tích tổ hợp".

Lịch sử và khảo cổ học đã cho chúng ta biết một số lượng lớn các "hệ thống ghi số", mục đích chính của chúng là gắn cho mỗi số nguyên riêng biệt (cho đến một giới hạn nào đó tùy thuộc vào các yêu cầu của việc sử dụng thực tế) một tên gọi và một biểu diễn viết, được tạo thành từ một số hạn chế các dấu hiệu theo những quy luật ít nhiều chính quy. Thủ tục thông dụng nhất rất xa là phân tích các số nguyên thành các tổng của các "đơn vị liên tiếp" $b_1$, $b_2$, ..., $b_n$, ..., mỗi đơn vị trong đó là một bội nguyên của đơn vị đứng trước nó; và mặc dù nói chung $b_n/b_{n-1}$ được lấy là một số cố định $b$ ("cơ sở" của hệ thống, thường là 10), có nhiều ngoại lệ đã biết đối với quy tắc này. Ví dụ, trong hệ thống Babylon, $b_n/b_{n-1}$ đôi khi bằng 10 và đôi khi bằng 6 [1], và trong hệ thống niên đại của người Maya $b_n/b_{n-1}$ bằng 20 ngoại trừ trường hợp $n = 2$, và $b_2/b_1 = 18$ [2]. Đối với ký hiệu viết tương ứng, nó phải chỉ ra số lượng các "đơn vị" $b_i$ thuộc mỗi cấp $i$. Trong nhiều hệ thống (chẳng hạn, hệ thống Ai Cập, Hy Lạp và La Mã) các bội liên tiếp $k.b_i$ (trong đó $k$ biến thiên từ 1 đến $(b_{i+1}/b_i) - 1$) được biểu thị bằng các ký hiệu phụ thuộc vào cả $k$ và $i$. Một bước tiến đầu tiên và quan trọng là biểu thị tất cả các số $k.b_i$ (với cùng một giá trị của $k$) bằng cùng một dấu hiệu: đó là nguyên lý của "ghi số theo vị trí", trong đó chỉ số $i$ được chỉ ra bởi thực tế rằng ký hiệu biểu thị $k.b_i$ xuất hiện "ở vị trí thứ $i$". Hệ thống đầu tiên thuộc loại này là của người Babylon, những người, chắc chắn từ sớm nhất là năm 2000 trước Công nguyên, đã dùng cùng một dấu hiệu để biểu thị tất cả các bội $k.60^{\pm i}$ tương ứng với các giá trị khác nhau của số mũ $i$ ([1], pp. 93-109). Sự bất tiện của một hệ thống như vậy dĩ nhiên là tính mơ hồ của nó chừng nào chưa có gì chỉ ra rằng các đơn vị của một cấp nào đó có vắng mặt hay không, tức là chừng nào hệ thống chưa được hoàn thiện bằng việc đưa vào một “không”. Tuy nhiên, người Babylon đã xoay xở không cần một dấu hiệu như vậy trong phần lớn lịch sử của họ, và chỉ sử dụng một “không” trong hai thế kỷ cuối trước Công nguyên, hơn nữa chỉ ở bên trong một số; cho đến thời điểm đó, chỉ có ngữ cảnh mới có thể làm sáng tỏ ý nghĩa của ký hiệu đang được xét. Chỉ có hai hệ thống khác sử dụng một cách có hệ thống một “không”: hệ thống của người Maya (dường như được sử dụng từ đầu Công nguyên [2]) và hệ thống thập phân hiện nay của chúng ta, hệ thống này đến (qua người Ả Rập) từ toán học Ấn Độ, nơi việc sử dụng số không được chứng thực từ những thế kỷ đầu Công nguyên. Hơn nữa, quan niệm về số không như một số (chứ không chỉ như một dấu hiệu phân cách) và việc đưa nó vào các phép tính là những đóng góp nguyên thủy của người Ấn Độ [3]. Dĩ nhiên, một khi nguyên lý "ghi số theo vị trí" đã được tiếp thu, việc mở rộng nó đến một cơ sở tùy ý là dễ dàng. Việc thảo luận các ưu điểm của những "cơ sở" khác nhau được đề xuất từ thế kỷ 17 phụ thuộc vào các kỹ thuật tính toán số, và không thể được đề cập ở đây. Chúng ta chỉ chú ý rằng phép toán nằm ở gốc của các hệ thống này, cái gọi là "phép chia Euclid", đã không xuất hiện trước thời của người Hy Lạp, và chắc chắn bắt nguồn từ những người Pythagore đầu tiên, những người đã biến nó thành công cụ cốt yếu trong số học lý thuyết của họ.

Các bài toán tổng quát về phép đếm, được tập hợp dưới tên gọi “giải tích tổ hợp”, dường như chưa từng được xét đến trước những thế kỷ cuối của thời cổ đại cổ điển; chỉ có công thức $\binom{n}{2}=\frac{1}{2}n(n-1)$ được ghi nhận, vào thế kỷ thứ ba sau Công nguyên. Nhà toán học Hindu Bhaskara (thế kỷ 12) đã biết công thức tổng quát của $\binom{n}{p}$. Một nghiên cứu có hệ thống hơn được tìm thấy trong một bản thảo của Levi ben Gerson (đầu thế kỷ 13): ông đã thu được công thức quy nạp cho số $V_n^p$ các cách sắp xếp $n$ đối tượng $p$ một lần, và đặc biệt cho số các hoán vị của $n$ đối tượng, đồng thời ông đã nêu ra các quy tắc tương đương với các quan hệ $\binom{n}{p}=V_n^p/p!$ và $\binom{n}{p}=\binom{n}{n-p}$ ([4], tr. 64-65). Nhưng bản thảo này dường như vẫn không được những người đương thời của ông biết đến, và các kết quả chỉ dần dần được các nhà toán học trong những thế kỷ tiếp theo khám phá lại. Về những tiến bộ sau này, hãy ghi nhận rằng Cardan đã chứng minh rằng số các tập con không rỗng của một tập hợp gồm $n$ phần tử là $2^n-1$. Pascal và Fermat, khi xây dựng phép tính xác suất, đã khám phá lại biểu thức của $\binom{n}{p}$, và Pascal là người đầu tiên nhận thấy quan hệ giữa các số này và định lý nhị thức, định lý dường như đã được người Ả Rập biết đến từ thế kỷ 13, người Trung Hoa biết đến vào thế kỷ 14, và đã được khám phá lại ở phương Tây vào đầu thế kỷ 16, cùng với phương pháp quy nạp tính toán các hệ số được gọi là "tam giác Pascal" ([4], tr. 35-38). Cuối cùng, vào khoảng năm 1676, Leibniz đã thu được (nhưng không công bố) công thức tổng quát cho "các hệ số đa thức", công thức này đã được de Moivre độc lập khám phá lại và công bố 20 năm sau.

# THƯ MỤC TÀI LIỆU

1. O. NEUGEBAUER, *Vorlesungen über die Geschichte der antiken Mathematik*, Bd. I : Vorgriechische Mathematik, Berlin (Springer), 1934.
2. S. G. MORLEY, *The Ancient Maya*, Stanford University Press, 1946.
3. B. DATTA and A. N. SINGH, *History of Hindu Mathematics*, vol. I, Lahore (Motilal Banarsi Das), 1935.
4. J. TROPFKE, *Geschichte der Elementar-Mathematik*, vol. VI : Analysis, Analytische Geometrie, Berlin-Leipzig (de Gruyter), 1924.
