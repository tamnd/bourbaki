---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: top-i-iv
pdf_pages: 0222-0224
extraction: ocr
statements: 0
exercises: 0
content_sha256: 9836b25f890b6d8c95fa9adad563e6cd492265d3291e4dbd7950bc5c309a779d
translated_from: content/en/top/II/historical_note.md
source_content_sha256: 8c3ca4dab2add2fccabc8970597fa4bc448dcf3aa1dc62d5707962e40af3d092
translation_model: gpt-5.4
translation_run: translate-vi-6d97da9b
glossary_version: 34
glossary_terms_sha256: 5351cbae9d3d26b96357853cab670d676301b5ef7c0808c58ac287960e5f0dfe
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Các số trong ngoặc vuông dẫn đến thư mục tài liệu ở cuối chú giải này.)

Các khái niệm và kết quả chính về không gian đều đã xuất hiện dần dần từ lý thuyết các biến số thực, và chỉ trong những năm gần đây chúng mới được nghiên cứu một cách có hệ thống. Cauchy, trong cố gắng đặt lý thuyết chuỗi trên một cơ sở chặt chẽ (xem các Ghi chú lịch sử của các Chương I và IV) đã lấy làm điểm xuất phát một nguyên lý mà dường như ông cho là hiển nhiên, cụ thể là một điều kiện cần và đủ để một dãy $(a_n)$ hội tụ là $|a_{n+p} - a_n|$ nhỏ tùy ý miễn là $n$ đủ lớn (xem chẳng hạn [2]). Cùng với Bolzano [1], chắc chắn ông là một trong những người đầu tiên phát biểu nguyên lý này một cách tường minh và nhận ra tầm quan trọng của nó; do đó có tên gọi "dãy Cauchy" dành cho các dãy số thực thỏa mãn điều kiện đang xét, và theo phép mở rộng dành cho các dãy $(x_n)$ các điểm trong một không gian mêtric (Chương IX) sao cho khoảng cách từ $x_{n+p}$ đến $x_n$ nhỏ tùy ý miễn là $n$ đủ lớn; và cuối cùng do đó có tên gọi "bộ lọc Cauchy" dành cho phép tổng quát hóa của các dãy Cauchy đã được nghiên cứu trong chương này.

Về sau, khi khái niệm trực giác về số thực không còn được xem là đầy đủ nữa, và người ta tìm cách định nghĩa các số thực bằng các số hữu tỉ để cung cấp một cơ sở vững chắc cho Giải tích, thì chính nguyên lý của Cauchy đã đem lại định nghĩa màu mỡ nhất trong các định nghĩa được đề xuất vào nửa sau thế kỷ XIX. Định nghĩa này, do Cantor [3] đưa ra (và được phát triển theo các ý tưởng của Cantor bởi Heine [5] và một cách độc lập bởi M\'eray, cùng với những người khác) gồm ở chỗ làm cho mỗi dãy Cauchy các số hữu tỉ tương ứng với một số thực ("dãy cơ bản" theo thuật ngữ của Cantor); cùng một số thực tương ứng với hai dãy Cauchy $(a_n)$ và $(b_n)$ các số hữu tỉ khi và chỉ khi $|a_n - b_n|$ tiến đến không. Ý tưởng cốt yếu ở đây là, từ một quan điểm nào đó (thực ra là quan điểm của "cấu trúc đều" được định nghĩa trong chương này, § 1, no. 1, Ví dụ 1), tập hợp $ \mathbf{Q} $ các số hữu tỉ là "không đầy đủ", và tập hợp các số thực là tập hợp "đầy đủ" mà người ta thu được từ $ \mathbf{Q} $ bằng "phép hoàn thiện".

Mặt khác, Heine là người đầu tiên định nghĩa tính liên tục đều đối với các hàm số thực của một hay nhiều biến thực, trong công trình phần lớn được gợi hứng bởi các ý tưởng của Weierstrass và Cantor [4], và ông đã chứng minh rằng mọi hàm số thực liên tục trên một khoảng đóng bị chặn của $ \mathbf{R} $ đều liên tục đều trên khoảng này: đó là "định lý Heine". Theo Định lý 2 của § 4, kết quả này liên quan đến tính compắc của một khoảng đóng bị chặn của $ \mathbf{R} $ ("định lý Borel-Lebesgue", Chương IV, § 2, Định lý 2; xem các Ghi chú lịch sử của các Chương I và IV), và chứng minh của Heine cho định lý của ông cũng có thể dùng, với một vài sửa đổi, để chứng minh định lý Borel-Lebesgue (và điều này đã xuất hiện như lý do đủ đối với một số tác giả để gọi định lý sau là "định lý Heine-Borel").

Những ý tưởng này đã được mở rộng sang các không gian tổng quát hơn khi các không gian mêtric bắt đầu được nghiên cứu, trước hết trong các trường hợp riêng rồi sau đó trong trường hợp tổng quát (xem Chương IX); trong một không gian mêtric, một khoảng cách được cho (tức là một hàm số thực của các cặp điểm, thỏa mãn những tiên đề nhất định) xác định đồng thời một tôpô và một cấu trúc đều. Fréchet, người đầu tiên đưa ra một định nghĩa tổng quát về các không gian này, đã nhận ra tầm quan trọng của nguyên lý Cauchy [6] và cũng đã chứng minh cho các không gian mêtric một định lý tương đương với Định lý 3 của § 4 ([6] và [7]). Hausdorff đã phát triển đáng kể lý thuyết các không gian mêtric trong tác phẩm "Mengenlehre" của ông ([8]; xem thêm [8 a]) và đặc biệt nhận ra rằng có thể áp dụng phép dựng của Cantor, đã mô tả ở trên, cho các không gian này và do đó thu được một không gian mêtric "đầy đủ" từ một không gian mêtric "không đầy đủ" (tức là một không gian trong đó nguyên lý Cauchy không đúng).

Các không gian mêtric là một kiểu riêng của "không gian đều"; các không gian sau đã được A. Weil định nghĩa trong toàn bộ tính tổng quát của chúng vào một thời điểm khá gần đây [9]. Trước đó, các khái niệm và kết quả về "cấu trúc đều" chỉ có thể được dùng trong liên hệ với các không gian mêtric, và sự kiện này giải thích vai trò quan trọng của các không gian mêtric và các không gian khả mêtric hóa (và đặc biệt của các không gian compắc khả mêtric hóa) trong nhiều công trình tôpô hiện đại, trong những vấn đề mà khoảng cách không có ích lợi thực sự nào. Một khi đã có định nghĩa của một không gian đều, thì không có khó khăn gì (đặc biệt nếu người ta cũng có sẵn khái niệm bộ lọc) trong việc mở rộng sang các không gian này gần như toàn bộ lý thuyết các không gian mêtric như được trình bày chẳng hạn bởi Hausdorff (và tương tự như vậy trong việc mở rộng, chẳng hạn, sang các không gian compắc tùy ý các kết quả về các không gian compắc mêtric được cho trong Topologie của Alexandroff-Hopf [10]). Đó là điều chúng tôi đã làm trong chương này; đặc biệt, định lý về sự hoàn thiện các không gian đều (§ 3, Định lý 3) không hơn gì một sự chuyển dịch, không có bất kỳ sửa đổi cốt yếu nào, của phép dựng các số thực của Cantor.

[1] B. Bolzano, Rein analytischer Beweis des Lehrsatzes, dass zwischen je zwei Werthen, die ein entgegengesetztes Resultat gewähren, wenigstens eine reelle Wurzel liegt, Ostwald’s Klassiker, no. 153, Leipzig, 1905.

[2] A.-L. Cauchy, Sur la convergence des séries [Exercices d’Analyse, năm thứ 2, Paris, 1827, p. 221 = Oeuvres (II), tập 7, Paris (Gauthier-Villars) 1889, p. 267].

[3] G. Cantor, Gesammelte Abhandlungen, Berlin (Springer), 1932.

[4] E. Heine, Über trigonometrische Reihen, Crelle’s Journal, 71 (1870), tr. 353-365.

[5] E. Heine, Die Elemente der Functionenlehre, Crelle’s Journal, 74 (1872), tr. 172-188.

[6] M. Fréchet, Sur quelques points du calcul fonctionnel, Rend. Palermo, 22 (1906), tr. 1-74.

[7] M. Fréchet, Les ensembles abstraits et le calcul fonctionnel, Rend. Palermo, 30 (1910), tr. 1-26.

[8] F. Hausdorff, Những nét cơ bản của lý thuyết tập hợp, Leipzig (Veit), 1914.

[8 a] F. Hausdorff, Lý thuyết tập hợp, Berlin (de Gruyter), 1927.

[9] A. Weil, Về các không gian có cấu trúc đều và về tôpô đại cương, Act. Scient. et Ind., no. 551, Paris (Hermann), 1937.

[10] P. Alexandroff and H. Hopf, Tôpô học I, Berlin (Springer), 1935.
