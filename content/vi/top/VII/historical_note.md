---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $ \mathbf{R}^n $
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: top-v-x
pdf_pages: 0103-0105
extraction: ocr
statements: 0
exercises: 0
content_sha256: 35116e92273a84611bcd2fafc7781088526de6da512dbe0e491d7e436efa8b82
translated_from: content/en/top/VII/historical_note.md
source_content_sha256: aa20b9537b63d5570e5f491cf578f62cd8d0694a4e17765b8312533bedaa116c
translation_model: gpt-5-6-mini
translation_run: translate-vi-f5d338fa
glossary_version: 34
glossary_terms_sha256: 35950088ed821f0403455f4471e19636657ed00da07d61a499e4d839b4f9d3be
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Các số trong ngoặc vuông chỉ đến thư mục tài liệu tham khảo ở cuối ghi chú này.)

Những kết quả chính của lý thuyết các nhóm con và các nhóm thương của các nhóm cộng tính $ \mathbf{R}^n $ đã được biết từ cuối thế kỷ trước. Nhiều vấn đề của số học và giải tích đã dẫn các nhà toán học đến việc nghiên cứu cấu trúc của các nhóm con của $ \mathbf{R}^n $ sinh bởi một số hữu hạn điểm. Vì vậy Lagrange, trong khi phát triển lý thuyết "phân thức liên tục", đã chỉ ra khi chuyển qua rằng, với mọi số thực $ \theta $, tồn tại các số nguyên $ m, n $, không đồng thời bằng không, sao cho $ m - n\theta $ tùy ý nhỏ ([1], quyển 7, p. 27). Năm 1835 Jacobi, được thúc đẩy bởi các nghiên cứu của ông về các hàm giải tích tuần hoàn của nhiều biến phức, đã chỉ ra rằng nếu $ x, y, z $ là ba vectơ của $ \mathbf{R}^2 $, thì tồn tại các số nguyên $ m, n, p $, không đồng thời bằng không, làm cho vectơ $ mx + ny + pz $ tùy ý nhỏ ([2], quyển 2, p. 25). Một thời gian ngắn sau đó Dirichlet, trong quá trình công trình của ông về lý thuyết các số đại số, đã phát hiện ra "nguyên lý ngăn kéo" nổi tiếng của mình (Schubfachprinzip) (xem § 1, các Bài tập 10 và 11), nhờ đó ông đã chỉ ra rằng $ p $ dạng $ \alpha_{i1}m_1 + \alpha_{i2}m_2 + \cdots + \alpha_{in}m_n - q_i \quad (1 \leq i \leq p) $, trong đó các $ \alpha_{ij} $ là các số thực tùy ý và các $ m_j $ cùng các $ q_i $ là các số nguyên (không đồng thời bằng không), có thể đồng thời làm cho tùy ý nhỏ ([3], quyển 1, p. 635). Bằng một phương pháp hoàn toàn khác Hermite đã đạt được cùng một kết quả vào năm 1850, đối với các dạng có kiểu riêng $ m\theta_i - q_i \quad (1 \leq i \leq p) $ ([4], quyển 1, p. 105). Cuối cùng, vào năm 1884, Kronecker đã chứng minh kết quả tổng quát được phát biểu trong Mệnh đề 7 của § 1 ([5], quyển 31, p. 47).

Dĩ nhiên các kết quả này độc lập với lý thuyết tổng quát về các nhóm Abel compact địa phương, vốn có nguồn gốc gần đây (xem Ghi chú lịch sử của Chương III); nhưng lý thuyết sau này, đặc biệt là lý thuyết đối ngẫu (*), đã đem lại một ánh sáng mới cho các kết quả cũ này, chủ yếu bằng cách

(*) Xem chẳng hạn A. Weil [8].

làm nổi bật khái niệm cơ bản về các nhóm con liên kết. Phần trình bày trong văn bản dựa trên các ý tưởng này (*).

Quan điểm mà chúng ta đã chọn trong chương này hoàn toàn có tính chất định tính: nghĩa là chúng ta đã thiết lập sự tồn tại của các tổ hợp tuyến tính của $ p $ điểm, với các hệ số nguyên, xấp xỉ tùy ý gần một điểm đã cho (điểm này có thể có thể phải thỏa mãn một số điều kiện nhất định); nhưng người ta cũng có thể hỏi liệu có tồn tại các quan hệ giữa độ chính xác của phép xấp xỉ và độ lớn của các hệ số trong các tổ hợp tuyến tính tạo ra phép xấp xỉ hay không; đây là quan điểm của lý thuyết định lượng về "xấp xỉ Diophantine", và cũng là quan điểm của tất cả các tác giả được trích dẫn trong đoạn đầu tiên. Trong một trăm năm qua, các vấn đề này đã là đối tượng của nhiều nghiên cứu đa dạng, phong phú về các ứng dụng vào lý thuyết số; việc truy tìm sự phát triển của chúng trong bối cảnh này sẽ đưa chúng ta đi quá xa khỏi phạm vi hiện tại, và vì vậy chúng ta sẽ không làm gì hơn ngoài việc dẫn người đọc muốn đi sâu vào các lý thuyết này đến các công trình cơ bản của Minkowski [6] và H. Weyl [7], vốn là nguồn gốc của một nền văn liệu phong phú (**).

(*) Một cách trình bày tương tự đã được Marcel Riesz phác thảo trước đó [9].
(**) Để xem thư mục gần đây về chủ đề này, xem chẳng hạn J. Koksma [10].

[1] J. L. Lagrange, Œuvres, quyển 7, Paris (Gauthier-Villars), 1877.
[2] C. G. J. Jacobi, Gesammelte Werke, quyển 2, Berlin (G. Reimer), 1882.
[2 bis] C. G. J. Jacobi, Über die vierfach periodischen Funktionen zweier Variabeln [Ostwald’s Klassiker, no. 64, Leipzig (Engelmann), 1895].
[3] P. G. Lejeune-Dirichlet, Werke, quyển 1, Berlin (G. Reimer), 1889.
[4] C. Hermite, Œuvres, quyển 1, Paris (Gauthier-Villars), 1905.
[5] L. Kronecker, Werke, quyển 31, Leipzig (Teubner), 1899.
[6] H. Minkowski, Gesammelte Abhandlungen, 2 quyển, Leipzig-Berlin (Teubner), 1911.
[7] H. Weyl, “Über die Gleichverteilung von Zahlen mod. Eins”, Math. Ann., quyển 77 (1916), p. 313 [= Selecta, Basel-Stuttgart (Birkhäuser), 1956, p. 111].
[8] A. Weil, L’intégration dans les groupes topologiques et ses applications. Act. Sci. et Ind., no. 869, Paris (Hermann) 1940, tr. 108-109 [xuất bản lần thứ 2, cùng chỗ, no. 1145 (1953)].
[9] M. Riesz, Modules reciproques [Proc. International Congress of Mathematicians, Oslo (1936), quyển 2, p. 36].
[10] J. Koksma, Diophantische Approximationen, Berlin (Springer), 1936.
