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
content_sha256: facc901c4c5c0a1802d4f4d754e35f59eb05b23e444f869e3164acea9992300d
translated_from: content/en/ens/III/historical_note.md
source_content_sha256: e392386e3fdea6fa40644954a9f6261d3e55aa11cd69be63e10a7679af76d092
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-786fc151
glossary_version: 29
glossary_terms_sha256: a0a2a108608c7038b1b618781507eb92d236290e9578ad7e5a2caee10c323bc6
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Chương III, § 5)

(Các số trong ngoặc chỉ thư mục tài liệu tham khảo
ở cuối Chú ý này.)

Sự phát triển của các ý tưởng liên quan đến các khái niệm số nguyên và số lực lượng gắn liền không thể tách rời với lịch sử của lý thuyết tập hợp và lôgic toán học; về các vấn đề này, xin dẫn người đọc tới Ghi chú lịch sử tiếp sau Chương IV. Mục đích của Chú ý này là chỉ ra vắn tắt một vài sự kiện nổi bật trong lịch sử của phép ghi số và của "giải tích tổ hợp".

Lịch sử và khảo cổ học đã cho chúng ta biết một số lượng lớn các "hệ ghi số", mà mục đích chủ yếu là gắn cho mỗi số nguyên riêng biệt (cho đến một giới hạn nào đó tùy theo những đòi hỏi của việc sử dụng trong thực tế) một tên gọi và một biểu diễn viết, được tạo thành từ một số hạn chế các ký hiệu theo những quy tắc ít nhiều chính quy. Cách thức thông dụng nhất, hơn hẳn các cách khác, là phân tích các số nguyên thành tổng của các "đơn vị liên tiếp" $b_1$, $b_2$, ..., $b_n$, ..., mà mỗi đơn vị là một bội nguyên của đơn vị đứng ngay trước nó; và mặc dù nói chung người ta lấy $b_n/b_{n-1}$ là một số cố định $b$ (là "cơ sở" của hệ, thường là 10), vẫn có nhiều ngoại lệ đã biết đối với quy tắc này. Chẳng hạn, trong hệ Babylon, $b_n/b_{n-1}$ đôi khi là 10 và đôi khi là 6 [1], còn trong hệ niên lịch của người Maya, $b_n/b_{n-1}$ bằng 20 trừ trường hợp $n = 2$, và $b_2/b_1 = 18$ [2]. Về ký hiệu viết tương ứng, nó phải chỉ ra số các "đơn vị" $b_i$ của mỗi thứ tự $i$. Trong nhiều hệ (chẳng hạn hệ Ai Cập, hệ Hy Lạp và hệ La Mã), các bội liên tiếp $k.b_i$ (trong đó $k$ chạy từ 1 đến $(b_{i+1}/b_i) - 1$) được ký hiệu bằng những dấu hiệu phụ thuộc đồng thời vào $k$ và $i$. Một bước tiến đầu tiên và quan trọng là ký hiệu tất cả các số $k.b_i$ (ứng với cùng một giá trị của $k$) bằng cùng một dấu hiệu: đó là nguyên lý của "phép ghi số theo vị trí", trong đó chỉ số $i$ được biểu thị bởi việc ký hiệu biểu diễn $k.b_i$ xuất hiện "ở vị trí thứ $i$". Hệ đầu tiên thuộc loại này là hệ của người Babylon, mà chắc chắn ngay từ năm 2000 trước Công nguyên,

được ký hiệu bằng cùng một dấu tất cả các bội $k.60^{\pm i}$ tương ứng với các giá trị khác nhau của số mũ $i$ ([1], pp. 93-109). Sự bất tiện của một hệ như vậy dĩ nhiên là tính nhập nhằng của nó chừng nào chưa có gì chỉ ra liệu các đơn vị của một cấp nhất định có vắng mặt hay không, nghĩa là chừng nào hệ chưa được hoàn chỉnh bằng việc đưa vào một “không”. Tuy nhiên, người Babylon đã xoay xở không cần một dấu như vậy trong phần lớn lịch sử của họ, và chỉ sử dụng một “không” trong hai thế kỷ cuối trước Công nguyên, rồi cũng chỉ ở bên trong một số; cho đến thời điểm đó, chỉ có ngữ cảnh mới có thể làm rõ ý nghĩa của ký hiệu đang xét. Chỉ có hai hệ khác sử dụng một cách có hệ thống một “không”: hệ của người Maya (dường như được sử dụng từ đầu Công nguyên [2]) và hệ thập phân hiện nay của chúng ta, hệ này đến từ toán học Hindu (qua người Ả Rập), nơi việc sử dụng số không được chứng thực từ những thế kỷ đầu Công nguyên. Hơn nữa, quan niệm về không như một số (chứ không chỉ là một dấu phân cách) và việc đưa nó vào các phép tính là những đóng góp nguyên bản của người Hindu [3]. Dĩ nhiên, một khi nguyên lý “ghi số theo vị trí” đã được tiếp thu, việc mở rộng nó đến một cơ sở tùy ý là dễ dàng. Việc thảo luận những ưu điểm của các “cơ sở” khác nhau được đề xuất từ thế kỷ 17 phụ thuộc vào các kỹ thuật tính toán số, và không thể được đề cập ở đây. Chúng ta chỉ chú ý rằng phép toán nằm ở gốc của các hệ này, cái gọi là “phép chia Euclid”, đã không xuất hiện trước thời kỳ của người Hy Lạp, và chắc chắn bắt nguồn từ những người Pythagore đầu tiên, những người đã biến nó thành công cụ cốt yếu trong số học lý thuyết của họ.

Các vấn đề tổng quát về việc đếm, được gộp lại dưới tên gọi “giải tích tổ hợp”, dường như chưa từng được thử xét trước những thế kỷ cuối của thời cổ đại cổ điển; chỉ có công thức $\binom{n}{2}=\frac{1}{2}n(n-1)$ được chứng thực, vào thế kỷ thứ ba Công nguyên. Nhà toán học Hindu Bhaskara (thế kỷ 12) biết công thức tổng quát cho $\binom{n}{p}$. Một nghiên cứu có hệ thống hơn được tìm thấy trong một bản thảo của Levi ben Gerson (đầu thế kỷ 13): ông đã thu được công thức quy nạp cho số $V_n^p$ các cách sắp xếp $n$ đối tượng lấy $p$ một lần, và đặc biệt cho số các hoán vị của $n$ đối tượng, và ông đã phát biểu các quy tắc tương đương với các quan hệ $\binom{n}{p}=V_n^p/p!$ và $\binom{n}{p}=\binom{n}{n-p}$ ([4], pp. 64-65). Nhưng bản thảo này dường như vẫn không được những người đương thời của ông biết đến, và các kết quả chỉ dần dần được các nhà toán học tái phát hiện trong những thế kỷ tiếp theo. Về những tiến bộ sau này, ta hãy ghi nhận rằng Cardan đã chứng minh rằng số các tập con không rỗng của một tập hợp gồm $n$ phần tử là $2^n-1$. Pascal và Fermat, khi xây dựng phép tính xác suất, đã tái phát hiện biểu thức của $\binom{n}{p}$, và Pascal là người đầu tiên nhận thấy quan hệ giữa các số này và định lý nhị thức, định lý dường như đã được người Ả Rập biết đến từ thế kỷ 13, người Trung Quốc vào thế kỷ 14, và đã được tái phát hiện ở phương Tây vào đầu thế kỷ 16, cùng với phương pháp quy nạp để tính toán

các hệ số được biết đến với tên gọi “tam giác Pascal” ([4], pp. 35-38). Cuối cùng, vào khoảng năm 1676, Leibniz đã thu được (nhưng không công bố) công thức tổng quát cho “các hệ số đa thức”, công thức này đã được de Moivre tái phát hiện một cách độc lập và công bố 20 năm sau.

# TÀI LIỆU THAM KHẢO

1. O. NEUGEBAUER, *Vorlesungen über die Geschichte der antiken Mathematik*, Bd. I : Vorgriechische Mathematik, Berlin (Springer), 1934.
2. S. G. MORLEY, *The Ancient Maya*, Stanford University Press, 1946.
3. B. DATTA and A. N. SINGH, *History of Hindu Mathematics*, vol. I, Lahore (Motilal Banarsi Das), 1935.
4. J. TROPFKE, *Geschichte der Elementar-Mathematik*, vol. VI : Analysis, Analytische Geometrie, Berlin-Leipzig (de Gruyter), 1924.
