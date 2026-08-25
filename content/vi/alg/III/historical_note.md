---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0679-0734
extraction: ocr
statements: 0
exercises: 0
content_sha256: 3c14dd05a7d164b088e57d9e2055bd53ac660021c557486fef9e72977b5ade91
translated_from: content/en/alg/III/historical_note.md
source_content_sha256: 5af65f5b13b8975b7fe850a1f1e5ddf05b39234af5824438937534fd1b3b408e
translation_model: gpt-5-6-mini
translation_run: translate-vi-d3878555
glossary_version: 34
glossary_terms_sha256: c395893c8cb57c4303a8ba34a4745710b14f7e4583f0b82a0ed4be88a309731f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Chương II và III)

(Chú thích. Các số trong ngoặc vuông chỉ các tài liệu tham khảo ở cuối Ghi chú này.)

Đại số tuyến tính vừa là một trong những ngành toán học cổ xưa nhất, vừa là một trong những ngành mới nhất. Mặt khác, ở nguồn gốc của toán học là các bài toán được giải bằng một phép nhân hoặc phép chia duy nhất, tức là bằng cách tính một giá trị của một hàm $f(x) = ax$, hoặc bằng cách giải một phương trình $ax = b$: đây là những bài toán điển hình của đại số tuyến tính và không thể xử lý chúng, thậm chí không thể đặt chúng một cách đúng đắn, nếu không "suy nghĩ tuyến tính".

Mặt khác, không chỉ những câu hỏi này mà hầu như mọi thứ liên quan đến các phương trình bậc nhất đều đã từ lâu bị xếp vào việc giảng dạy sơ cấp, khi sự phát triển hiện đại của các khái niệm trường, vành, không gian vectơ tôpô, v.v. đã tách ra và nhấn mạnh các khái niệm cốt yếu của đại số tuyến tính (chẳng hạn tính đối ngẫu); khi đó người ta nhận thấy đặc trưng tuyến tính cốt yếu của gần như toàn bộ toán học hiện đại, mà "tuyến tính hóa" tự nó là một trong những nét phân biệt, và đại số tuyến tính đã được dành cho vị trí xứng đáng của nó. Vì vậy, để trình bày lịch sử của nó, từ quan điểm hiện nay của chúng ta, sẽ là một công việc khó khăn cũng như quan trọng; và do đó chúng ta phải bằng lòng với việc đưa ra một bản tóm tắt ngắn gọn.

Từ những điều trên có thể thấy rằng đại số tuyến tính chắc chắn đã ra đời để đáp ứng những nhu cầu của các nhà tính toán thực hành; do đó ta thấy quy tắc tam suất† và quy tắc vị trí sai, được phát biểu ít nhiều rõ ràng, đóng một vai trò quan trọng trong tất cả các sách hướng dẫn về số học thực hành, từ giấy cói Rhind của người Ai Cập đến những sách được sử dụng trong các trường tiểu học của chúng ta, qua Āryabhaṭa, người Ả Rập, Leonard ở

† Xem J. Tropfke, Geschichte der Elementar-Mathematik, 1. Band, 2te Ausgabe, Berlin-Leipzig (W. de Gruyter), 1921, tr. 150–155.

Pisa và vô số "sách tính toán" của thời Trung cổ và thời Phục hưng; nhưng chúng chưa bao giờ tạo thành nhiều hơn một phần nhỏ, dành cho việc sử dụng của những người thực hành, trong các lý thuyết khoa học tiên tiến nhất.

Còn đối với các nhà toán học thực sự, bản chất nghiên cứu của họ về đại số tuyến tính phụ thuộc vào cấu trúc chung của khoa học của họ. Toán học Hy Lạp cổ đại, như được trình bày trong *Cơ sở* của Euclid, đã phát triển hai lý thuyết trừu tượng có tính chất tuyến tính, một mặt là lý thuyết về đại lượng ([2], Quyển V; xem Ghi chú lịch sử về *Tôpô đại cương*, IV) và mặt khác là lý thuyết về số nguyên ([2], Quyển VII). Với người Babylon, ta tìm thấy những phương pháp gần với đại số sơ cấp của chúng ta hơn nhiều; họ biết cách giải, và rất đẹp ([1], tr. 181–183), các hệ phương trình bậc nhất. Tuy nhiên, trong một thời gian rất dài, sự tiến bộ của đại số tuyến tính chủ yếu bị giới hạn trong sự tiến bộ của các phép tính đại số và chúng phải được xem xét từ quan điểm này, vốn nằm ngoài Ghi chú này; để rút gọn một hệ tuyến tính về một phương trình kiểu $ax = b$, chỉ cần, trong trường hợp có một ẩn số, biết các quy tắc (về bản chất đã được Diophantus phát biểu) để chuyển các số hạng từ vế này sang vế kia và kết hợp các số hạng đồng dạng; và, trong trường hợp có nhiều ẩn số, còn cần biết cách khử chúng lần lượt cho đến khi chỉ còn lại một ẩn số. Vì vậy, các Luận thuyết về đại số, cho đến thế kỷ XVIII, cho rằng mọi thứ đã hoàn tất đối với bậc nhất khi họ đã trình bày các quy tắc này; còn đối với một hệ có số phương trình bằng số ẩn số (họ không xét các hệ khác) mà các vế trái không phải là các dạng độc lập tuyến tính, họ chỉ bằng lòng nhận xét chuyển qua rằng điều này chỉ ra một bài toán được đặt không đúng. Trong các luận thuyết của thế kỷ XIX và thậm chí trong một số công trình gần đây hơn, quan điểm này chỉ được thay đổi bởi sự tiến bộ của ký hiệu, cho phép viết các hệ $n$ phương trình với $n$ ẩn số, và bởi việc đưa vào các định thức cho phép đưa ra các công thức của một nghiệm tường minh trong "trường hợp tổng quát"; sự tiến bộ này, công lao đáng lẽ thuộc về Leibniz ([7], p. 239) nếu ông đã phát triển và công bố các ý tưởng của mình về chủ đề này, chủ yếu là nhờ các nhà toán học của thế kỷ XVIII và đầu thế kỷ XIX.

Nhưng trước hết chúng ta phải nghiên cứu các dòng tư tưởng khác nhau mà, nhiều hơn nhiều so với việc nghiên cứu các phương trình tuyến tính, đã góp phần vào sự phát triển của đại số tuyến tính theo nghĩa mà chúng ta hiểu. Lấy cảm hứng từ việc nghiên cứu Apollonius, Fermat [4(a)], sau khi đã hình thành, thậm chí trước Descartes [5], nguyên lý của hình học giải tích, có ý tưởng phân loại các đường cong phẳng theo bậc của chúng (điều mà, sau khi dần dần trở nên quen thuộc với mọi nhà toán học, có thể được xem là đã được nắm bắt hoàn toàn vào cuối thế kỷ XVII) và phát biểu nguyên lý cơ bản rằng một phương trình bậc nhất, trong mặt phẳng, biểu diễn một đường thẳng và một phương trình bậc hai biểu diễn một đường conic: một nguyên lý mà từ đó ông suy ra ngay lập tức một số hệ quả "rất đẹp" liên quan đến các quỹ tích hình học. Đồng thời, ông phát biểu [4(b)] sự phân loại các bài toán thành các bài toán có một nghiệm duy nhất, các bài toán rút gọn về một phương trình với hai ẩn số, một phương trình với ba ẩn số, v.v.; và ông thêm rằng: loại thứ nhất bao gồm việc xác định một điểm, loại thứ hai một quỹ tích đường thẳng hoặc mặt phẳng, các loại khác một mặt, v.v. ("... một bài toán như vậy không chỉ tìm kiếm một điểm hay một đường thẳng, mà là toàn bộ một mặt thích hợp với câu hỏi; ở đây các mặt như các quỹ tích có nguồn gốc của chúng và tương tự đối với phần còn lại", loc. cit., p. 186; ở đây đã có mầm mống của hình học $n$-chiều). Bài viết này, bằng việc phát biểu nguyên lý chiều trong đại số và hình học đại số, chỉ ra sự hợp nhất của đại số và hình học hoàn toàn phù hợp với các ý tưởng hiện đại, nhưng như đã thấy, đã mất hơn hai thế kỷ để thâm nhập vào tư tưởng của con người.

Ít nhất những ý tưởng này nhanh chóng dẫn đến sự khai triển của hình học giải tích, đạt đến sự hoàn thiện của nó vào thế kỷ XVIII với Clairaut, Euler, Cramer, Lagrange và nhiều người khác. Tính chất tuyến tính của các công thức về phép biến đổi tọa độ trong mặt phẳng và trong không gian, điều mà Fermat hẳn đã nhận thấy từ trước, được làm nổi bật chẳng hạn bởi Euler ([8(a)], Các chương II–III và Phụ lục của Chương IV), người ở đây đặt nền móng cho sự phân loại các đường cong phẳng và các mặt theo bậc của chúng (bất biến chính xác vì tính tuyến tính của các công thức này); cũng chính ông (loc. cit., Chương XVIII) đưa vào từ "affinity" để mô tả quan hệ giữa các đường cong có thể suy ra từ nhau bằng một phép biến đổi $x' = ax, y' = by$ (nhưng không nhận thấy bất kỳ điều gì bất biến về mặt hình học trong định nghĩa này, vốn vẫn gắn với một lựa chọn cụ thể của các trục). Ít lâu sau đó, ta thấy Lagrange [9(a)] dành trọn một hồi ký, vốn trong một thời gian dài vẫn nổi tiếng một cách xứng đáng, cho các bài toán điển hình tuyến tính và đa tuyến tính của hình học giải tích trong không gian ba chiều. Vào khoảng thời gian này, liên quan đến bài toán tuyến tính được tạo thành bởi việc tìm một đường cong phẳng đi qua các điểm đã cho, khái niệm định thức hình thành, trước hết theo một cách hơi thực nghiệm, với Cramer [10] và Bezout [11]; khái niệm này sau đó được phát triển bởi nhiều tác giả và các tính chất cốt yếu của nó được xác lập một cách dứt khoát bởi Cauchy [13] và Jacobi [16(a)].

Mặt khác, trong khi các nhà toán học có khuynh hướng hơi coi thường các phương trình bậc nhất, việc giải các phương trình vi phân lại được xem là một bài toán quan trọng; thật tự nhiên rằng, trong số các phương trình này, các phương trình tuyến tính, với hệ số hằng hoặc không, đã sớm được phân biệt và việc nghiên cứu chúng góp phần nhấn mạnh tính tuyến tính và các tính chất liên quan. Điều này chắc chắn thấy được trong công trình của Lagrange [9(b)] và Euler [8(b)], ít nhất là đối với các phương trình thuần nhất; vì các tác giả này không thấy có ý nghĩa gì trong việc nói rằng nghiệm tổng quát của phương trình không thuần nhất là tổng của một nghiệm riêng và nghiệm tổng quát của phương trình thuần nhất tương ứng, và họ không sử dụng nguyên lý này (tuy nhiên đã được d'Alembert biết đến); ở đây ta cũng chú ý rằng, khi họ phát biểu rằng nghiệm tổng quát của phương trình tuyến tính thuần nhất cấp $n$ là một tổ hợp tuyến tính của $n$ nghiệm riêng, họ không nói thêm rằng các nghiệm này phải độc lập tuyến tính và không cố gắng làm rõ tường minh khái niệm sau; có vẻ như chỉ việc giảng dạy của Cauchy tại École Polytechnique mới làm sáng tỏ ([14], pp. 573–574) các điểm này cũng như nhiều điểm khác. Nhưng ngay từ trước đó Lagrange (*loc. cit.*) cũng đưa vào (thật vậy, chỉ bằng tính toán thuần túy và không đặt tên cho nó) phương trình liên hợp $L^*(y) = 0$ của một phương trình vi phân tuyến tính $L(y) = 0$, một ví dụ điển hình của đối ngẫu nhờ quan hệ

$$
\int z L(y)\, dx = \int L^*(z) y\, dx,
$$

đúng với $y$ và $z$ bằng không tại các đầu mút của khoảng lấy tích phân; chính xác hơn, và 30 năm trước khi Gauss định nghĩa tường minh phép chuyển vị của một phép thế tuyến tính trong 3 biến, ở đây ta thấy không nghi ngờ gì ví dụ đầu tiên của một "toán tử phiếm hàm" $L^*$ là chuyển vị hay "liên hợp" của một toán tử $L$ được cho bằng một hàm song tuyến tính (ở đây là tích phân $\int yz\, dx$).

Đồng thời và một lần nữa với Lagrange [9(c)], các phép thế tuyến tính, lúc đầu trong 2 và 3 biến, đang trong quá trình chinh phục số học. Rõ ràng tập hợp các giá trị của một hàm $F(x, y)$, khi $x$ và $y$ nhận mọi giá trị nguyên, không thay đổi khi thực hiện một phép thế tuyến tính với các hệ số nguyên, có định thức 1, trên $x$ và $y$; dựa trên nhận xét cơ bản này Lagrange xây dựng lý thuyết biểu diễn số bằng các dạng và lý thuyết rút gọn các dạng; còn Gauss, bằng một bước mà sự táo bạo của nó ngày nay đã trở nên khó để chúng ta đánh giá đúng, cô lập khái niệm tương đương và khái niệm lớp của các dạng (xem Ghi chú lịch sử cho I); về chủ đề này, ông nhận ra sự cần thiết của một số nguyên lý sơ cấp liên quan đến các phép thế tuyến tính và đưa vào đặc biệt khái niệm chuyển vị hay liên hợp ([12(a)], p. 304). Từ thời điểm này trở đi, việc nghiên cứu số học và việc nghiên cứu đại số của các dạng toàn phương, trong 2, 3 và sau đó $n$ biến, việc nghiên cứu các dạng song tuyến tính liên quan chặt chẽ đến chúng và gần đây hơn là phép tổng quát hóa các khái niệm này đến vô hạn biến, cho đến hiện nay, đã tạo thành một trong những nguồn tiến bộ phong phú nhất của đại số tuyến tính (xem Ghi chú lịch sử cho IX).

Nhưng một tiến bộ có lẽ còn quyết định hơn là việc Gauss tạo ra, trong cùng *Disquisitiones* (xem Ghi chú lịch sử cho I), lý thuyết về các nhóm giao hoán hữu hạn, xuất hiện ở đó theo bốn cách khác nhau, trong nhóm cộng của các số nguyên modulo $m$ (với $m$ là một số nguyên), trong nhóm nhân của các số nguyên nguyên tố cùng nhau với $m$ modulo $m$, trong nhóm các lớp của các dạng toàn phương nhị thức và cuối cùng trong nhóm nhân của các căn bậc $m$ của đơn vị; và, như chúng ta đã ghi nhận, rõ ràng là với tư cách các nhóm giao hoán, hay đúng hơn là các môđun trên $\mathbf{Z}$, Gauss xử lý tất cả các nhóm này và nghiên cứu cấu trúc, các quan hệ đẳng cấu của chúng, v.v. Trong môđun của các "số nguyên phức" $a + bi$, về sau ta thấy ông nghiên cứu một môđun vô hạn trên $\mathbf{Z}$, mà sự đẳng cấu của nó chắc chắn ông đã nhận thấy với môđun các chu kỳ (do ông phát hiện trong miền phức) của các hàm elliptic; trong mọi trường hợp ý tưởng này đã xuất hiện rõ ràng trong công trình của Jacobi, chẳng hạn trong chứng minh nổi tiếng của ông về tính bất khả của một hàm có 3 chu kỳ và các quan điểm của ông về bài toán đảo của các tích phân Abel [16(b)], để nhanh chóng dẫn đến các định lý của Kronecker (xem Ghi chú lịch sử cho Tôpô đại cương, VII).

Ở đây, một dòng chảy khác hợp lưu với những dòng chảy mà chúng ta đã cố gắng lần theo quá trình và những chỗ quanh co đôi khi của chúng, và dòng chảy này từ lâu vẫn nằm dưới lòng đất. Như sau này sẽ được trình bày chi tiết hơn (Ghi chú lịch sử cho IX), hình học “thuần túy” theo nghĩa được hiểu vào thế kỷ trước, tức về cơ bản là hình học xạ ảnh của mặt phẳng và không gian mà không sử dụng tọa độ, đã được Desargues [6] sáng tạo vào thế kỷ XVII; những ý tưởng của ông, được một Fermat đánh giá đúng giá trị và được một Pascal đưa vào thực hành, sau đó đã bị chôn vùi trong quên lãng, bị lu mờ bởi những tiến bộ rực rỡ của hình học giải tích; nó được phục hồi vào cuối thế kỷ XVIII, với Monge, rồi Poncelet và những đối thủ của ông là Brianchon và Chasles, đôi khi hoàn toàn và có chủ ý tách khỏi các phương pháp giải tích, đôi khi (đặc biệt ở Đức) đan xen chặt chẽ với chúng. Giờ đây, các phép biến đổi xạ ảnh, xét từ bất kỳ quan điểm nào (tổng hợp hay giải tích), dĩ nhiên chỉ là các phép thế tuyến tính trên các tọa độ xạ ảnh hay “trọng tâm”; lý thuyết các đường conic (vào thế kỷ XVII) và sau đó là lý thuyết các quadric, mà các tính chất xạ ảnh của chúng là mối quan tâm chủ yếu của trường phái này trong một thời gian dài, chỉ là lý thuyết các dạng toàn phương, mà mối liên hệ chặt chẽ của chúng với đại số tuyến tính chúng ta đã chỉ ra trước đây. Thêm vào các khái niệm này là khái niệm đối cực: cũng do Desargues sáng tạo, lý thuyết các cực và đối cực, trong tay Monge và những người kế tục ông và chẳng bao lâu dưới tên gọi nguyên lý đối ngẫu, trở thành một công cụ mạnh để biến đổi các định lý hình học; nếu không thể khẳng định rằng mối quan hệ của nó với các phương trình vi phân liên hợp đã được nhận thấy trong thời kỳ đó (chúng được Pincherle chỉ ra vào cuối thế kỷ), thì ít nhất Chasles cũng không quên [17] nhận thấy mối quan hệ của nó với khái niệm các tam giác cầu đối ngẫu, được đưa vào lượng giác cầu bởi Viète ([3], p. 428) và Snellius ngay từ thế kỷ XVI. Nhưng tính đối ngẫu trong hình học xạ ảnh chỉ là một phương diện của tính đối ngẫu của các không gian vectơ, có tính đến những biến đổi do việc chuyển từ không gian afin sang không gian xạ ảnh áp đặt (là một không gian thương của nó, theo quan hệ “phép nhân vô hướng”).

Thế kỷ XIX, hơn bất kỳ thời kỳ nào trong lịch sử của chúng ta, rất phong phú về các nhà toán học bậc nhất; và thật khó, trong vài trang, ngay cả khi chỉ giới hạn ở những nét nổi bật nhất, mô tả tất cả những gì được tạo ra trong tay họ do sự hội tụ của những dòng tư tưởng này. Giữa một bên là các phương pháp tổng hợp thuần túy, một kiểu giường Procrustes nơi những người theo chính thống của chúng tự đặt mình vào tình thế khổ sở, và bên kia là các phương pháp giải tích gắn với một hệ tọa độ được áp đặt tùy ý lên không gian, nhu cầu về một phép tính hình học sớm được cảm nhận, được Leibniz mơ tới nhưng không sáng tạo ra và được Carnot phác thảo một cách không hoàn chỉnh: trước hết xuất hiện phép cộng các vectơ, tiềm ẩn trong công trình của Gauss về biểu diễn hình học của các số phức và những ứng dụng ông thực hiện đối với hình học sơ cấp (xem Ghi chú lịch sử về Tôpô đại cương, VIII), được Bellavitis phát triển dưới tên gọi “phương pháp các đoạn tương đẳng” và mang hình thức cuối cùng với Grassmann, Möbius và Hamilton; đồng thời, dưới tên gọi “phép tính trọng tâm”, Möbius đưa ra một phiên bản của nó thích hợp với các nhu cầu của hình học xạ ảnh [18].

Cũng trong thời kỳ ấy, và bởi chính những người đó, bước chuyển, tự nhiên đến vậy (một khi đã đi theo con đường này), từ mặt phẳng và không gian “thông thường” sang không gian $n$-chiều được thực hiện; thực vậy, đó là một bước chuyển không thể tránh khỏi, vì các hiện tượng đại số mà trong hai hoặc ba biến có thể được giải thích bằng hình học vẫn còn đúng với một số tùy ý các biến; do đó, việc áp đặt, khi sử dụng ngôn ngữ hình học, sự hạn chế vào 2 hoặc 3 chiều, đối với nhà toán học hiện đại cũng là một ách khó chịu chẳng khác gì ách luôn ngăn cản người Hy Lạp mở rộng khái niệm số tới các tỉ số của những đại lượng không thông ước. Vì thế, ngôn ngữ và các ý tưởng liên quan đến không gian $n$-chiều xuất hiện gần như đồng thời ở mọi nơi, một cách mơ hồ trong công trình của Gauss, một cách rõ ràng trong công trình của các nhà toán học thuộc thế hệ kế tiếp; và mức độ tự tin nhiều hay ít của họ khi sử dụng chúng có lẽ ít phụ thuộc vào khuynh hướng toán học của họ hơn là vào cách nhìn triết học hoặc thậm chí thuần túy thực tiễn của họ. Trong mọi trường hợp, Cayley và Grassmann, vào khoảng năm 1846, xử lý các khái niệm này hết sức dễ dàng (và điều này, Cayley nói, hoàn toàn trái với Grassmann ([22(a)], p. 321), “không cần viện đến bất kỳ khái niệm siêu hình nào”); Cayley không bao giờ xa rời cách giải thích giải tích và tọa độ, trong khi ngay từ đầu, trong công trình của Grassmann, phép cộng các vectơ trong không gian $n$-chiều và phương diện hình học chiếm ưu thế, dẫn đến những phát triển mà chúng ta sẽ nói đến ngay sau đây.

Trong khi đó, động lực do Gauss tạo ra đã thúc đẩy các nhà toán học, theo hai hướng khác nhau, tiến tới nghiên cứu các đại số hay “hệ siêu phức”. Một mặt, việc cố gắng mở rộng miền các số thực theo một cách khác với việc đưa vào “đơn vị ảo” $i = \sqrt{-1}$ và nhờ đó có lẽ mở ra những miền rộng lớn hơn, cũng phong phú như miền các số phức, là điều không thể tránh khỏi. Bản thân Gauss tin ([12(b)], p. 178) rằng không thể có một mở rộng như vậy, chừng nào người ta còn muốn giữ lại các tính chất chính của các số phức, tức là, theo ngôn ngữ hiện đại, những tính chất làm cho nó trở thành một trường giao hoán; và, hoặc dưới ảnh hưởng của ông hoặc một cách độc lập, những người cùng thời với ông dường như cũng chia sẻ niềm tin này, mà mãi về sau Weierstrass [23] mới chứng minh được bằng một định lý chính xác. Nhưng một khi phép nhân các số phức được diễn giải bằng các phép quay trong mặt phẳng, thì nếu đề xuất mở rộng ý tưởng này lên không gian ba chiều (vì các phép quay trong không gian tạo thành một nhóm không Abel), phải xét đến các phép nhân không giao hoán; đây là một trong những ý tưởng dẫn đường của Hamilton† trong việc phát hiện ra các quaternion [20], ví dụ đầu tiên về một trường không giao hoán. Tính chất đặc biệt của ví dụ này (ví dụ duy nhất, như Frobenius về sau đã chỉ ra, có thể xây dựng trên

† Xem lời tựa thú vị của Lectures on quaternions [20], trong đó ông thuật lại toàn bộ lịch sử phát hiện của mình.

trường các số thực) phần nào hạn chế tầm quan trọng của nó, mặc dù, hay có lẽ chính vì, sự hình thành một trường phái những “nhà quaternion” cuồng tín: một hiện tượng kỳ lạ, về sau lại tái diễn quanh công trình của Grassmann, rồi quanh những nhà phổ biến hóa đã rút ra từ Hamilton và Grassmann cái được gọi là “phép tính vectơ”. Việc từ bỏ tính kết hợp ít lâu sau đó, bởi Graves và Cayley, những người xây dựng nên các “số Cayley”, không mở ra một con đường nào thật thú vị. Nhưng sau khi Sylvester đã đưa vào các ma trận và (mà không đặt tên cho nó) đã xác định rõ ràng hạng của chúng [21], thì lại chính Cayley [22(b)] đã xây dựng phép tính ma trận, không phải không nhận thấy (một sự kiện cốt yếu thường bị bỏ qua về sau) rằng một ma trận chỉ là một ký hiệu rút gọn cho một phép thế tuyến tính, cũng như Gauss đã ký hiệu dạng $aX^2 + 2bXY + cY^2$ bằng $(a, b, c)$. Đây dĩ nhiên chỉ là một khía cạnh, đối với chúng ta là khía cạnh thú vị nhất, của sản lượng phong phú của Sylvester và Cayley về các định thức và mọi thứ liên quan đến chúng, một sản lượng đầy những đồng nhất thức tài tình và những phép tính ấn tượng.

Ngoài ra (trong số những công trình khác), Grassmann phát hiện một đại số trên trường số thực, đại số ngoài vẫn mang tên ông. Công trình của ông, thậm chí còn sớm hơn công trình của Hamilton [19(a)], được tạo ra trong một sự cô độc tinh thần gần như hoàn toàn, trong một thời gian dài vẫn ít được biết đến, không nghi ngờ gì nữa vì tính độc đáo của nó, và cũng vì những màn sương triết học mà ngay từ đầu nó đã tự bao phủ lấy mình, đến mức chẳng hạn lúc đầu đã khiến Möbius e ngại. Được thúc đẩy bởi những mối quan tâm tương tự như Hamilton nhưng có tầm quan trọng lớn hơn (và điều mà ông sớm nhận thấy chính là những mối quan tâm của Leibniz), Grassmann xây dựng một công trình đại số-hình học đồ sộ, dựa trên một quan niệm hình học hay “nội tại” (đã được tiên đề hóa ít nhiều) về không gian vectơ $n$-chiều; trong số những kết quả sơ cấp hơn mà ông đạt được, chúng ta nêu chẳng hạn định nghĩa về sự độc lập tuyến tính của các vectơ, định nghĩa về chiều và hệ thức cơ bản

$$
\dim V + \dim W = \dim(V + W) + \dim(V \cap W)
$$

(loc. cit., p. 209; cf. [19(b)], p. 21). Nhưng đặc biệt là phép nhân ngoài, rồi phép nhân nội, của các đa vectơ đã cung cấp cho ông những công cụ mà nhờ đó ông dễ dàng xử lý trước hết các bài toán của đại số tuyến tính theo đúng nghĩa, rồi đến những bài toán liên quan đến cấu trúc Euclid, tức là tính trực giao của các vectơ (nơi ông tìm thấy tương đương của đối ngẫu, cái mà ông không có).

Con đường khác mà Gauss đã mở ra trong việc nghiên cứu các hệ siêu phức là con đường xuất phát từ các số nguyên phức $a + bi$; tiếp theo đó một cách khá tự nhiên là các đại số hoặc tổng quát hơn, các hệ siêu phức, trên vành $\mathbf{Z}$ các số nguyên và trên trường $\mathbf{Q}$ các số hữu tỉ, trước hết là những hệ đã được Gauss hình dung, được sinh bởi các căn của đơn vị, rồi đến các trường số đại số và các môđun các số nguyên đại số: các trường này là chủ đề chính trong công trình của Kummer, còn việc nghiên cứu các môđun sau được Dirichlet, Hermite, Kronecker và Dedekind bắt đầu. Ở đây, trái với điều xảy ra với các đại số trên trường thực, không cần từ bỏ bất kỳ tính chất đặc trưng nào của các trường giao hoán, và sự chú ý trong suốt thế kỷ XIX chỉ tập trung vào các trường này. Nhưng các tính chất tuyến tính và chẳng hạn việc tìm cơ sở của các số nguyên của trường (không thể thiếu đối với một định nghĩa tổng quát của biệt thức) đóng vai trò cốt yếu tại nhiều chỗ; và ít nhất là với Dedekind, các phương pháp đã định hướng trở thành điển hình "siêu phức"; hơn nữa, bản thân Dedekind, không đặt cho mình bài toán về các đại số nói chung, ý thức được tính chất này trong các công trình của mình và điều liên hệ chúng, chẳng hạn, với các kết quả của Weierstrass về các hệ siêu phức trên trường thực ([24], đặc biệt tập 2, p. 1). Đồng thời, việc xác định cấu trúc của nhóm nhân các phần tử khả nghịch trong một trường số đại số, do Dirichlet thực hiện trong một số ghi chú nổi tiếng [15] và gần như đồng thời bởi Hermite, có tầm quan trọng sống còn trong việc làm sáng tỏ các ý niệm về các môđun trên $\mathbf{Z}$, các hệ sinh của chúng và các cơ sở của chúng (khi chúng tồn tại). Sau đó, khái niệm iđêan, được Dedekind định nghĩa trong các trường số đại số (như một môđun trên vành các số nguyên của trường), trong khi Kronecker đưa vào các vành đa thức (dưới tên gọi "các hệ môđun") một khái niệm tương đương, cho những ví dụ đầu tiên về các môđun trên những vành tổng quát hơn $\mathbf{Z}$; và trong công trình của chính các tác giả ấy, rồi của Hilbert, trong những trường hợp đặc biệt khái niệm nhóm với các toán tử dần dần được tách riêng, cùng với khả năng luôn luôn dựng từ một nhóm như vậy một môđun trên một vành được xác định thích hợp.

Đồng thời, việc nghiên cứu số học-đại số các dạng song tuyến tính toàn phương và phép "rút gọn" của chúng (hay, điều tương đương, của các ma trận và các "bất biến" của chúng) dẫn đến việc phát hiện ra các nguyên lý tổng quát về nghiệm của các hệ phương trình tuyến tính, những nguyên lý mà do thiếu khái niệm hạng đã thoát khỏi Jacobi.\footnote{Về việc phân loại các hệ gồm $n$ phương trình với $n$ ẩn khi định thức bằng không, ông nói ([16(a)], p. 370): "paullo prolixum videtur negotium" (không thể làm sáng tỏ một cách ngắn gọn).} Bài toán tìm nghiệm nguyên của các hệ phương trình tuyến tính với các hệ số nguyên được Hermite tấn công và giải quyết, trước hết trong một trường hợp đặc biệt, rồi trong toàn bộ tính tổng quát bởi H. J. Smith [25]; các kết quả của người sau chỉ đến năm 1878 mới được Frobenius tìm lại, trong khuôn khổ một chương trình nghiên cứu rộng lớn do Kronecker đề xướng và trong đó Weierstrass cũng tham gia; nhân tiện, trong quá trình tiến hành những công trình này, Kronecker đã đưa các định lý về các hệ tuyến tính với các hệ số thực (hoặc phức) đến dạng hoàn chỉnh, những định lý này cũng được, trong một cuốn sách giáo khoa tối nghĩa, trình bày với sự cẩn trọng tỉ mỉ đặc trưng của ông, bởi tác giả nổi tiếng của *Alice in Wonderland*; còn về Kronecker, ông khinh thường việc công bố các kết quả này và để chúng lại cho các đồng nghiệp và môn đệ của mình; bản thân từ "hạng" chỉ được Frobenius đưa vào. Cũng trong quá trình giảng dạy tại Đại học Berlin, Kronecker [26] và Weierstrass đưa vào định nghĩa "tiên đề" của định thức (như một hàm đa tuyến tính phản xứng của $n$ vectơ trong không gian $n$-chiều, được chuẩn hóa sao cho nó nhận giá trị 1 tại ma trận đơn vị), một định nghĩa tương đương với định nghĩa dẫn xuất từ phép tính của Grassmann và với định nghĩa được chấp nhận trong Chuyên luận này; cũng trong các khóa giảng của mình, Kronecker, không cảm thấy cần phải đặt tên cho nó và vẫn ở một dạng chưa nội tại, đưa vào tích tenxơ của các không gian và tích "Kronecker" của các ma trận (phép thế tuyến tính cảm sinh trên một tích tenxơ bởi các phép thế tuyến tính đã cho được áp dụng lên các thừa số).

Nghiên cứu này không thể tách rời khỏi lý thuyết về các bất biến do Cayley, Hermite và Sylvester sáng tạo (bộ ba “bất biến” mà về sau Hermite nói đến trong các bức thư của mình), và từ quan điểm hiện đại, trên hết là một lý thuyết về các biểu diễn của nhóm tuyến tính. Ở đây, với tư cách tương đương đại số của tính đối ngẫu trong hình học xạ ảnh, xuất hiện sự phân biệt giữa các chuỗi biến cogredient và contragredient, tức là các vectơ trong một không gian và các vectơ trong không gian đối ngẫu; và, sau khi trước hết xét đến các dạng bậc thấp rồi đến bậc tùy ý, trong 2 và 3 biến, hầu như ngay lập tức các dạng song tuyến tính, rồi các dạng đa tuyến tính, được khảo sát trong một số chuỗi biến “cogredient” hoặc “contragredient”, điều này tương đương với việc đưa vào các tenxơ; khái niệm sau trở nên tường minh và được phổ biến khi, dưới sự gợi ý của lý thuyết về các bất biến, Ricci và Levi-Civitá, vào năm 1900, đưa “phép tính tenxơ” vào hình học vi phân [28], mà về sau trở nên rất thịnh hành nhờ được các nhà vật lý “tương đối luận” sử dụng. Một lần nữa, sự đan xen ngày càng tăng của lý thuyết về các bất biến, hình học vi phân và lý thuyết các phương trình đạo hàm riêng (đặc biệt là bài toán gọi là bài toán Pfaff và các tổng quát hóa của nó) dần dần dẫn các nhà hình học đến việc xét các dạng song tuyến tính phản xứng của các vi phân, đặc biệt là “đối bất biến song tuyến tính” của một dạng bậc 1 (được Lipschitz đưa vào năm 1870 và sau đó được Frobenius nghiên cứu), để dẫn đến việc E. Cartan [29] và Poincaré [30] sáng tạo ra phép tính các dạng vi phân ngoài. Poincaré đưa các dạng này vào, nhằm tạo nên các bất biến nguyên của mình, dưới dạng những biểu thức xuất hiện trong các tích phân bội, trong khi Cartan, không nghi ngờ gì, được định hướng bởi các nghiên cứu của ông về các đại số, đưa chúng vào theo một cách hình thức hơn, nhưng không quên nhận thấy rằng phần đại số của phép tính của chúng đồng nhất với phép nhân ngoài của Grassmann (do đó có tên gọi mà ông chọn), qua đó dứt khoát trả lại cho công trình của người này vị trí thích đáng của nó. Việc chuyển các dạng vi phân ngoài sang ký hiệu của phép tính tenxơ, hơn nữa, cho thấy ngay lập tức mối liên hệ của chúng với các tenxơ phản đối xứng, điều này, một khi chấp nhận quan điểm thuần túy đại số, cho thấy rằng chúng đối với các dạng đa tuyến tính phản xứng cũng như các tenxơ hiệp biến đối với các dạng đa tuyến tính tùy ý; khía cạnh này được làm sáng tỏ thêm với lý thuyết hiện đại về các biểu diễn của nhóm tuyến tính; và do đó, chẳng hạn, tính đồng nhất cơ bản giữa định nghĩa các định thức do Weierstrass và Kronecker đưa ra với định nghĩa thu được từ phép tính của Grassmann được nhận ra.

Do đó, chúng ta đi đến thời kỳ hiện đại, trong đó phương pháp tiên đề và khái niệm cấu trúc (ban đầu được nhận thức một cách mơ hồ, và chỉ mới đây được định nghĩa) cho phép chúng ta tách những khái niệm vốn cho đến lúc đó đã bị trộn lẫn không thể gỡ ra, phát biểu những gì còn mơ hồ hoặc được để cho trực giác, và chứng minh với tính tổng quát thực sự các định lý vốn chỉ được biết trong những trường hợp đặc biệt. Peano, một trong những người sáng tạo ra phương pháp tiên đề và cũng là một trong những nhà toán học đầu tiên đánh giá đầy đủ công trình của Grassmann, đã đưa ra ngay từ năm 1888 ([27], Chương IX) định nghĩa tiên đề của các không gian vectơ (hữu hạn chiều hoặc không) trên trường các số thực và, với một ký hiệu hoàn toàn hiện đại, của các ánh xạ tuyến tính từ một không gian như vậy vào một không gian khác; một thời gian sau, Pincherle tìm cách phát triển các áp dụng của đại số tuyến tính, được quan niệm như vậy, vào lý thuyết hàm, theo một hướng, quả thực, không mấy hiệu quả; ít nhất quan điểm của ông cho phép ông nhận ra “liên hợp Lagrange” như một trường hợp đặc biệt của phép chuyển vị các ánh xạ tuyến tính: điều này sớm xuất hiện, còn rõ ràng hơn nữa, và đối với các phương trình đạo hàm riêng cũng như các phương trình vi phân, trong quá trình các công trình đáng ghi nhớ của Hilbert và trường phái của ông về không gian Hilbert và các áp dụng của nó vào giải tích. Chính trong dịp đó Toeplitz [31], cũng đưa vào (nhưng bằng các tọa độ) không gian vectơ tổng quát nhất trên các số thực, đã đưa ra nhận xét cơ bản rằng lý thuyết về các định thức không cần thiết để chứng minh các định lý chính của đại số tuyến tính, điều này cho phép mở rộng chúng không khó khăn đến các không gian vô hạn chiều; và ông cũng chỉ ra rằng đại số tuyến tính được hiểu theo cách này dĩ nhiên có thể áp dụng cho một trường cơ sở giao hoán tùy ý.

Mặt khác, với việc Banach đưa vào năm 1922 các không gian mang tên ông, người ta gặp những không gian không đẳng cấu với đối ngẫu của chúng,\footnote{Đó là những không gian vectơ chuẩn đầy đủ trên trường số thực hoặc trường số phức.} mặc dù trong một bài toán vừa mang tính tôpô vừa mang tính đại số. Ngay giữa một không gian vectơ hữu hạn chiều và đối ngẫu của nó cũng không có một đẳng cấu “chính tắc”, tức là được xác định bởi cấu trúc của nó, điều đã từ lâu được phản ánh trong sự phân biệt giữa đồng biến và phản biến. Tuy nhiên, dường như không còn nghi ngờ gì rằng sự phân biệt giữa một không gian và đối ngẫu của nó chỉ được xác lập một cách dứt khoát sau công trình của Banach và trường phái của ông; cũng trong các công trình này, tầm quan trọng của khái niệm đối chiều được làm sáng tỏ. Về phép đối ngẫu hay “trực giao” giữa các không gian con vectơ của một không gian và các không gian con vectơ của đối ngẫu của nó, cách thức nó được phát biểu ngày nay không chỉ có một sự tương tự bề ngoài với cách phát biểu hiện đại của định lý chính của lý thuyết Galois (cf. *Algebra*, V) và với cái gọi là đối ngẫu Pontrjagin trong các nhóm Abel địa phương compact; cái sau bắt nguồn từ Weber, người, trong quá trình nghiên cứu số học, đã đặt nền móng cho nó vào năm 1886 đối với các nhóm hữu hạn; trong lý thuyết Galois, “đối ngẫu” giữa các nhóm con và các trường con thành hình trong các công trình của Dedekind và Hilbert; còn tính trực giao giữa các không gian con vectơ bắt nguồn một cách hiển nhiên, trước hết từ đối ngẫu giữa các đa tạp tuyến tính trong hình học xạ ảnh và cũng từ khái niệm và các tính chất của các đa tạp hoàn toàn trực giao trong một không gian Euclid hoặc một không gian Hilbert (do đó có tên gọi của nó). Tất cả những mạch này được tập hợp lại trong thời kỳ đương đại, dưới bàn tay của các nhà đại số như

E. Noether, Artin và Hasse và các nhà tôpô học như Pontrjagin và Whitney (không phải là không có ảnh hưởng lẫn nhau) để đi tới, trong mỗi lĩnh vực này, trình độ hiểu biết mà các kết quả được trình bày trong Chuyên khảo này.

Đồng thời, một sự xem xét có tính phê phán được tiến hành, nhằm loại bỏ, trên từng điểm, những giả thiết không hoàn toàn thiết yếu, và đặc biệt là những giả thiết có thể cản trở con đường dẫn tới một số áp dụng. Do đó, người ta nhận thấy khả năng thay thế các trường bằng các vành trong khái niệm không gian vectơ và, bằng cách tạo ra khái niệm tổng quát về môđun, đồng thời xử lý các không gian này, các nhóm Abel, các môđun đặc biệt đã được Kronecker, Weierstrass, Dedekind và Steinitz nghiên cứu trước đó, và thậm chí cả các nhóm có toán tử và chẳng hạn áp dụng định lý Jordan-Hölder cho chúng; đồng thời, với sự phân biệt giữa môđun phải và môđun trái, chúng ta chuyển sang trường hợp không giao hoán, nảy sinh từ sự phát triển hiện đại của lý thuyết các đại số bởi trường phái Mỹ (Wedderburn, Dickson) và đặc biệt là trường phái Đức (E. Noether, E. Artin).

TÀI LIỆU THAM KHẢO

1. O. Neugebauer, Vorlesungen über Geschichte der antiken Mathematik, Vol. I: Vorgriechische Mathematik, Berlin (Springer), 1934.
2. Euclidis Elementa, 5 vols., ed. J. L. Heiberg, Lipsiae (Teubner), 1883–88.
2 bis. T. L. Heath, The thirteen books of Euclid’s Elements ..., 3 vols., Cambridge, 1908.
3. Francisci Vietae, Opera mathematica ..., Lugduni Batavorum (Elzevir), 1646.
4. P. Fermat, Oeuvres, vol. I, Paris (Gauthier-Villars), 1891: (a) Ad locos planos et solidos Isagoge (pp. 91–110; French transl. ibid., vol. III, p. 85); (b) Appendix ad methodum ... (pp. 184–188; French transl., ibid., vol. III, p. 159).
5. R. Descartes, La géométrie, Leyde (Jan Maire), 1637 (=Oeuvres, ed. Ch. Adam and P. Tannery, vol. VI, Paris (L. Cerf), 1902).
6. G. Desargues, Oeuvres ..., vol. I, Paris (Leiber), 1864: Brouillon proiect d’une atteinte aux éuénemens des rencontres d’un cône auec un plan (pp. 103–230).
7. G. W. Leibniz, Mathematische Schriften, ed. C. I. Gerhardt, vol. I, Berlin (Asher), 1849.
8. L. Euler: (a) Introductio in Analysin Infinitorum, vol. 2, Lausannae, 1748 (=Opera Omnia (1), vol. IX, Zürich-Leipzig-Berlin (O. Füssli and B. G. Teubner), 1945); (b) Institutionum Calculi Integralis, vol. 2, Petropoli, 1769 (=Opera Omnia (1), vol. XII, Leipzig-Berlin (B. G. Teubner), 1914).
9. J.-L. Lagrange, Oeuvres, Paris (Gauthier-Villars), 1867–1892: (a) Solutions analytiques de quelques problèmes sur les pyramides triangulaires, vol. III, pp. 661–692; (b) Solution de différents problèmes de calcul intégral, vol. I, p. 471; (c) Recherches d’arithmétique, vol. III, pp. 695–795.

10. G. Cramer, Introduction à l’analyse des lignes courbes, Geneva (Cramer and Philibert), 1750.

11. E. Bezout, Théorie générale des équations algébriques, Paris, 1779.

12. C. F. Gauss, Werke, Göttingen, 1870–1927: (a) Disquisitiones arithmeticae, vol. I; (b) Selbstanzeige zur Theoria residuorum biquadraticorum, Commentatio secunda, vol. II, pp. 169–178.

13. A.-L. Cauchy, Mémoire sur les fonctions qui ne peuvent obtenir que deux valeurs égales et de signes contraires par suite des transpositions opérées entre les variables qu’elles renferment, J. Ec. Polytech., cahier 17 (volume X), 1815, pp. 29–112 (=Oeuvres complètes (2), vol. I, Paris (Gauthier-Villars), 1905, pp. 91–169).

14. A.-L. Cauchy, in Leçons de calcul différentiel et de calcul intégral, rédigées principalement d’après les méthodes de M. A.-L. Cauchy by Abbé Moigno, vol. II, Paris, 1844.

15. P. G. Lejeune-Dirichlet, Werke, vol. I, Berlin (G. Reimer), 1889, pp. 619–644.

16. C. G. J. Jacobi, Gesammelte Werke, Berlin (G. Reimer), 1881–1891: (a) De formatione et proprietatibus determinantium, vol. III, pp. 355–392; (b) De functionibus duarum variabilium . . ., vol. II, pp. 25–50.

17. M. Chasles, Aperçu historique sur l’origine et le développement des méthodes en géométrie . . ., Bruxelles, 1837.

18. A. F. Möbius, Der baryzentrische Calcul . . ., Leipzig, 1827 (=Gesammelte Werke, vol. I, Leipzig (Hirzel), 1885).

19. H. Grassmann: (a) Die lineale Ausdehnungslehre, ein neuer Zweig der Mathematik, dargestellt und durch Anwendungen auf die übrigen Zweige der Mathematik, wie auch auf die Statik, Mechanik, die Lehre vom Magnetismus und die Kristallonomie erläutert, Leipzig (Wigand), 1844 (=Gesammelte Werke, vol. I, 1st Part, Leipzig (Teubner), 1894); (b) Die Ausdehnungslehre, vollständig und in strenger Form bearbeitet, Berlin, 1862 (=Gesammelte Werke, vol. I, 2nd Part, Leipzig (Teubner), 1896).

20. W. R. Hamilton, Lectures on quaternions, Dublin, 1853.

21. J. J. Sylvester, Collected Mathematical Papers, vol. I, Cambridge, 1904: No. 25, Addition to the articles . . ., pp. 145–151 (=Phil. Mag., 1850).

22. A. Cayley, Collected Mathematical Papers, Cambridge, 1889–1898: (a) Sur quelques théorèmes de la géométrie de position, vol. I, pp. 317–328 (=Crelle’s J., vol. XXXI (1846), pp. 213–227); (b) A memoir on the theory of matrices, vol. II, pp. 475–496 (=Phil. Trans., 1858).

23. K. Weierstrass, Mathematische Werke, vol. II, Berlin, (Mayer und Müller),

1895: Về lý thuyết các đại lượng phức được tạo thành từ $n$ đơn vị chính, tr. 311–332.
24. R. Dedekind, Các công trình toán học tuyển tập, 3 tập, Braunschweig (Vieweg), 1930–32.
25. H. J. Smith, Các bài báo toán học tuyển tập, tập I, Oxford, 1894: Về các hệ phương trình tuyến tính bất định và các đồng dư, p. 367 (=Phil. Trans., 1861).
26. L. Kronecker, Bài giảng về lý thuyết các định thức . . ., Leipzig (Teubner), 1903.
27. G. Peano, Tính toán hình học theo lý thuyết Ausdehnung của Grassmann, được mở đầu bằng các phép toán của lôgic suy diễn, Torino, 1888.
28. G. Ricci và T. Levi-Civita, Các phương pháp tính vi phân tuyệt đối và các ứng dụng của chúng, Math. Ann., tập LIV (1901), p. 125.
29. E. Cartan, Về một số biểu thức vi phân và bài toán Pfaff, Ann. E.N.S. (3), tập XVI (1899), tr. 239–332 (=Oeuvres complètes, tập II_1, Paris (Gauthier-Villars), 1953, tr. 303–396).
30. H. Poincaré, Các phương pháp mới của cơ học thiên thể, tập III, Paris (Gauthier-Villars), 1899, Chương XXII.
31. O. Toeplitz, Về việc giải vô hạn các phương trình tuyến tính với vô hạn ẩn, Rend. Circ. Mat. Pal., tập XXVIII (1909), tr. 88–96.

$x + y, x \cdot y, xy, x \top y, x \perp y$: I, § 1, no. 1.
$X \top Y, X + Y, XY$ (X, Y là các tập con): I, § 1, no. 1.
$X \top a, a \top X$ (X là một tập con, a là một phần tử): I, § 1, no. 1.

$$
\prod_{\alpha \in A} x_\alpha, \bigwedge_{\alpha} x_\alpha, \bigwedge x_\alpha, \bigwedge_{\alpha \in A} x, \bigwedge_{\alpha} x_\alpha, \bigwedge x_\alpha, \sum_{\alpha \in A} x_\alpha, \sum x_\alpha, \sum_{\alpha} x_\alpha, \prod_{\alpha \in A} x_\alpha, \prod x_\alpha,
$$

$$
\prod_{\alpha \in A} x_\alpha : \text{I, § 1, no. 2}.
$$

$$
\prod_{p \leq i \leq q} x_i, \prod_{i=p}^q x_i : \text{I, § 1, no. 2}.
$$

$x_p \top x_{p+1} \top \cdots \top x_q : \text{I, § 1, no. 3}$.

$$
\prod^n x, \perp x^n, nx \quad (n \in \mathbf{N}) : \text{I, § 1, no. 3}.
$$

$$
\prod_{0 \leq i < j \leq n} x_{ij}, \prod_{i < j} x_{ij} : \text{I, § 1, no. 5}.
$$

$$
\sum_{i=p}^q \sum_{j=r}^s x_{ij}, \sum_{j=r}^s \sum_{i=p}^q x_{ij} : \text{I, § 1, no. 5}.
$$

$$
\prod_{0 \leq i_1 < i_2 < \cdots < i_p \leq n} x_{i_1 i_2 \cdots i_p}, \prod_{i_1 < i_2 < \cdots < i_p} x_{i_1 i_2 \cdots i_p} : \text{I, § 1, no. 5}.
$$

$0, 1 : \text{I, § 2, no. 1}$.

$\gamma_a, \delta_a, \gamma(a), \delta(a) : \text{I, § 2, no. 2}$.

$E_S$ (S là một tập con của một nửa nhóm giao hoán E): I, § 2, no. 4.

$\mathbf{Z}, +$ (phép cộng trong $\mathbf{Z}$): I, § 2, no. 5.

$\leq$ (quan hệ thứ tự trên $\mathbf{Z}$): I, § 2, no. 5.

$\mathbf{N}^* : \text{I, § 2, no. 5}$.

$\prod^n$ (đối với $n \in \mathbf{Z}$): I, § 2, no. 7.

$
-x, x - y, x + y - z, x - y - z, x - y + z - t : \text{I, § 2, no. 8}.
$

$nx$ ($n \in \mathbf{Z}$): I, § 2, no. 8.

$x^n$ ($n \in \mathbf{Z}$): I, § 2, no. 8.

$
\frac{1}{x}, \frac{x}{y}, x/y : \text{I, § 2, no. 8}.
$ $\alpha.x, x.\alpha, x^\alpha$ ($\alpha$ một toán tử): I, § 3, no. 1.
$\alpha \perp x, \alpha \perp X, \Xi \perp X$ ($\alpha$ một toán tử, $\Xi$ một tập hợp các toán tử): I, § 3, no. 1.
$\mathfrak{S}_F$: I, § 4, no. 1.
$(G:H), G/H$ ($H$ một nhóm con của G): I, § 4, no. 4.
$x \equiv y$ (mod. H), $x \equiv y$ (H) (H một nhóm con chuẩn tắc): I, § 4, no. 4.
Ker $f$, Im $f$ ($f$ một đồng cấu nhóm): I, § 4, no. 5.
$$
\prod_{i \in I} G_i \quad (G_i \text{ các nhóm}): \text{I, } \S 4, \text{ no. 8}.
$$
$G_1 \times_H G_2$: I, § 4, no. 8.
$$
\prod_{i \in I} G_i \quad (G_i \text{ các nhóm}): \text{I, } \S 4, \text{ no. 9}.
$$
$x \equiv y$ (mod. $a$), $x \equiv y$ ($a$) ($a, x, y$ các số nguyên hữu tỉ): I, § 4, no. 10.
$v_p(a)$ ($p$ một số nguyên tố, $a$ một số nguyên hữu tỉ): I, § 4, no. 10.
Aut(G), Int(G), Int(x) (G một nhóm, $x \in G$): I, § 5, no. 3.
$N_G(A), N(A)$ (G một nhóm, $A \subset G$): I, § 5, no. 3.
$C_G(A), C(A)$ (G một nhóm, $A \subset G$): I, § 5, no. 3.
E/G, G|E (G một nhóm tác động trên E): I, § 5, no. 4.
G|E/H (G, H các nhóm tác động trên E bằng các tác động giao hoán): I, § 5, no. 4.
$\mathfrak{S}_n$: I, § 5, no. 7.
$\tau_{x,y}$ (phép hoán vị chuyển trí có giá $\{x, y\}$): I, § 5, no. 7.
$\varepsilon(\sigma), \varepsilon_\sigma$ ($\sigma$ một phép hoán vị): I, § 5, no. 7.
$\mathcal{U}_E, \mathcal{U}_n$: I, § 5, no. 7.
$F \xrightarrow{i} E \xrightarrow{\rho} G$ (E, F, G các nhóm): I, § 6, no. 1.
$F \times_\tau G, \mathcal{E}_\tau$ ($\tau$ một đồng cấu của G vào Aut(F)): I, § 6, no. 1.
$gf$ ($f \in F, g \in G$): I, § 6, no. 1.
$(f, g) \cdot_\tau (f', g')$ ($f, f'$ trong F, $g, g'$ trong G): I, § 6, no. 1.
$(x, y), (A, B)$ ($x, y$ các phần tử, A, B các tập con của một nhóm G): I, § 6, no. 2.
D(G): I, § 6, no. 2.
$C^n(G)$: I, § 6, no. 3.
$D^n(G)$: I, § 6, no. 4.
$E^G$ (G một nhóm tác động trên E): I, § 6, no. 5.
$M_n(X), M(X)$ (X một tập hợp): I, § 7, no. 1.
$l(w)$ ($w$ một phần tử của M(X)): I, § 7, no. 1.
$ww', w.w'$ ($w, w'$ các phần tử của M(X)): I, § 7, no. 1.
$l(w)$ ($w$ một từ trên X): I, § 7, no. 2.
$ww', w.w'$ ($w, w'$ các từ trên X): I, § 7, no. 2.
Mo(X) (X một tập hợp): I, § 7, no. 2.
$l(\sigma)$ ($\sigma$ một phân tích): I, § 7, no. 3.
$*G_i, G_1 * G_2$ ($G_1, G_2, G_i$ các nhóm): I, § 7, no. 3.
$\langle \tau_1, \ldots, \tau_n; r_1, \ldots, r_m \rangle$ ($\tau_j$ các phần tử sinh, $r_i$ các quan hệ): I, § 7, no. 6.
$\langle \tau_1, \ldots, \tau_n; u_1 = v_1, \ldots, u_m = v_m \rangle$ ($\tau_j$ các phần tử sinh, $u_i, v_i$ các phần tử của một nhóm tự do): I, § 7, no. 6.
$\mathbf{Z}^{(X)}, \mathbf{N}^{(X)}$ (X một tập hợp): I, § 7, no. 7.

0, 1 (các phần tử của một vành): I, § 8, no. 1.
A^0 (A một vành): I, § 8, no. 3.
(a) (a một phần tử của A): I, § 8, no. 6.
$\sum_{\lambda} a_\lambda$ (a_\lambda các iđêan): I, § 8, no. 6.
$x \equiv y \pmod{a}$, $x \equiv y$ (a) (a một iđêan): I, § 8, no. 7.
A/a (a một iđêan hai phía): I, § 8, no. 7.
ab (a, b các iđêan hai phía): I, § 8, no. 9.
A[S^{-1}] (S một tập con của một vành A): I, § 8, no. 12.
$F_p$ (p một số nguyên tố): I, § 9, no. 1.
$\mathbf{Q}$: I, § 9, no. 4.
$\mathbf{Q}_+$: I, § 9, no. 4.
|x|, sgn x (x một số hữu tỉ): I, § 9, no. 4.
in(G): I, § 4, Bài tập 13.
D_n: I, § 6, Bài tập 4.
Q: I, § 6, Bài tập 4.
A \approx B: I, § 6, Bài tập 39.
e(G): I, § 7, Bài tập 39.
d_n(X): I, § 7, Bài tập 39.
A_s, A_d (A một vành): II, § 1, no. 1.
$\sum_{i \in I} x_i ((x_i)_{i \in I})$ một họ các phần tử của một môđun có giá hữu hạn: II, § 1, no. 1.
Hom_A(E, F), Hom(E, F), (E, F, A-môđun): II, § 1, no. 2.
End_A(E), End(E), Aut(E), GL(E) (E một A-môđun): II, § 1, no. 2.
Hom_A(u, v), Hom(u, v) (u, v các ánh xạ tuyến tính): II, § 1, no. 2.
1_E (E một môđun): II, § 1, no. 2.
0 (môđun không): II, § 1, no. 3.
Ker u, Im u, Coim u, Coker u (u một ánh xạ tuyến tính): II, § 1, no. 3.
$\prod_i f_i$ (f_i: E_i \to F_i các ánh xạ tuyến tính): II, § 1, no. 5.
$\bigoplus_{i \in I} E_i, E_p \oplus E_{p+1} \oplus \cdots \oplus E_q ((E_i)_{i \in I}$ một họ các A-môđun): II, § 1, no. 6.
$\sum_{i \in I} f_i$ (f_i: E_i \to F_i các ánh xạ tuyến tính): II, § 1, no. 6.
$\bigoplus_{i \in I} f_i, f_p \oplus f_{p+1} \oplus \cdots \oplus f_q$ (f_i: E_i \to F_i các ánh xạ tuyến tính): II, § 1, no. 6.
E^{(1)} (E một môđun): II, § 1, no. 6.
$\bigoplus_{i \in I} M_i$ ((M_i)_{i \in I} một họ các môđun con): II, § 1, no 7.
long_A(M), long(M) (M một A-môđun có độ dài hữu hạn): II, § 1, no. 10.
$\delta_{st}$ (ký hiệu Kronecker): II, § 1, no. 11.
$\sum_{t \in T} \xi_t \cdot t$ (T một tập hợp, $\xi_t$ các phần tử của một vành): II, § 1, no. 11.

Ann(S), Ann(x) (S một tập con của một môđun, x một phần tử của một môđun): II, § 1, no. 12.
$\rho_*(E), E_{[B]}$ (E một A-môđun, $\rho : B \to A$ một đồng cấu vành): II, § 1, no. 13.
$\rho_*(u)$ ($\rho : B \to A$ một đồng cấu vành, u một ánh xạ A-tuyến tính): II, § 1, no. 13.
E* (E một môđun): II, § 2, no. 3.
$\langle x, x^* \rangle$ (x một phần tử của một môđun trái E, $x^*$ một phần tử của môđun đối ngẫu E* của nó): II, § 2, no. 3.
$\langle x^*, x \rangle$ (x một phần tử của một môđun phải E, $x^*$ một phần tử của môđun đối ngẫu E* của nó): II, § 2, no. 3.
$t_u$ (u một ánh xạ tuyến tính hoặc nửa tuyến tính): II, § 2, no. 5.
$\tilde{u}$ (u một đẳng cấu): II, § 2, no. 5.
$E \otimes_A F, E \otimes_A F$ (E một A-môđun phải, F một A-môđun trái): II, § 3, no. 1.
$x \otimes y$ (x $\in$ E (một môđun phải), y $\in$ F (một môđun trái)): II, § 3, no. 1.
$u \otimes v$ (u, v các ánh xạ tuyến tính): II, § 3, no. 2.
$u \otimes v$ (u, v các ánh xạ nửa tuyến tính): II, § 3, no. 3.
$s_{A_d}$ (A một vành): II, § 3, no. 4.
$\mathcal{L}_2(E, F; G)$ (E, F, G các môđun trên một vành giao hoán): II, § 3, no. 5.
$\bigotimes_{\lambda \in L} G_\lambda, \bigotimes_{\lambda \in L} x_\lambda$ (($G_\lambda$) một họ các môđun $\mathbf{Z}$, $x_\lambda \in G_\lambda$ với mọi $\lambda$): II, § 3, no. 9.
$\bigotimes_{\lambda \in L} v_\lambda$ ($v_\lambda : G_\lambda \to G'_\lambda$ $\mathbf{Z}$-các ánh xạ tuyến tính): II, § 3, no. 9.
$\bigotimes_{(c,p,q)} G_\lambda, \bigotimes_{(c,p,q)} x_\lambda, \bigotimes_{(c)} x_\lambda$: II, § 3, no. 9.
$\bigotimes_{(c)} v_\lambda$ ($v_\lambda$ $\mathbf{Z}$-các ánh xạ tuyến tính): II, § 3, no. 9.
$E_1 \otimes_{A_1} E_2 \otimes_{A_2} E_3 \otimes \cdots \otimes_{A_{n-2}} E_{n-1} \otimes_{A_{n-1}} E_n$: II, § 3, no. 9.
$x_1 \otimes x_2 \otimes \cdots \otimes x_n$: II, § 3, no. 9.
$u_1 \otimes u_2 \otimes \cdots \otimes u_n$ ($u_i$ các ánh xạ tuyến tính): II, § 3, no. 9.
$\mathcal{L}_n(E_1, \ldots, E_n; G)$ ($E_1, \ldots, E_n, G$ các môđun trên một vành giao hoán): II, § 3, no. 9.
Tr(u) (u một tự đồng cấu của một môđun trên một vành giao hoán): II, § 4, no. 3.
$\rho^*(E), E_{(B)}$ (E một A-môđun, $\rho : A \to B$ một đồng cấu vành): II, § 5, no. 1.
$\rho^*(u), u_{(B)}$ ($\rho : A \to B$ một đồng cấu vành, u một đồng cấu A-môđun): II, § 5, no. 1.
dim_K E, dim E, [E : K] (E một không gian vectơ K): II, § 7, no. 2.
dim_A E, dim E (E một A-môđun mà mọi hai cơ sở đều có cùng lực lượng): II, § 7, no. 2.
codim_E F, codim F (F một không gian con vectơ của một không gian vectơ E): II, § 7, no. 3.
rg(u) (u một ánh xạ tuyến tính của các không gian vectơ): II, § 7, no. 4.
rg(u) (u một phần tử của một tích tenxơ của các không gian vectơ): II, § 7, no. 8.
dim_K E, dim E (E một không gian affine trên một trường K): II, § 9, no. 1.
$a + t, t + a$ (a một điểm, t một phép tịnh tiến của một không gian affine): II, § 9, no. 1.

$b - a$ ($a, b$ các điểm của một không gian affine): II, § 9, no. 1.

$\sum_{c \in I} \lambda_i x_i$ (($x_i$)$_{i \in I}$ một họ các điểm của một không gian affine, $(\lambda_i)_{i \in I}$ một họ các vô hướng, có giá hữu hạn, sao cho $\sum_i \lambda_i = 1$ hoặc $\sum_i \lambda_i = 0$): II, § 9, no. 1.

$\mathbf{P}(V), \Delta(V)$ (V một không gian vectơ): II, § 9, no. 5.
$\mathbf{P}_n(K), \Delta_n(K)$ (K một trường): II, § 9, no. 5.
$\dim_K \mathbf{P}(V), \dim \mathbf{P}(V)$ (V một không gian K-vectơ): II, § 9, no. 5.
$\tilde{K}, \infty$ (K một trường): II, § 9, no. 9.
$\mathbf{PGL}(V), \mathbf{PGL}_n(K), \mathbf{PGL}(n, K)$ (K một trường, V một không gian vectơ): II, § 9, no. 10.
$^tM$ ($M$ một ma trận): II, § 10, no. 1.
$M' + M''$ ($M', M''$ các ma trận trên một nhóm giao hoán): II, § 10, no. 2.
$f(M', M''), M'M''$ ($M', M''$ các ma trận): II, § 10, no. 2.
$E_{ij}$ (các đơn vị ma trận): II, § 10, no. 3.
$\sigma(M), M^\sigma$ ($M$ một ma trận, $\sigma$ một đồng cấu vành): II, § 10, no. 3.
$M(x), x$ (x một phần tử của một môđun tự do sinh hữu hạn): II, § 10, no. 4.
$M(u)$ (u một đồng cấu của một môđun tự do vào một môđun tự do): II, § 10, no. 4.
$M(x), M(u)$ (các ma trận đối với các phân tích thành tổng trực tiếp): II, § 10, no. 5.
$M(u)$ (u một ánh xạ nửa tuyến tính): II, § 10, no. 6.
$\mathbf{M}_n(A), I_n, 1_n$ (A một vành): II, § 10, no. 7.
$\mathbf{GL}_n(A), \mathbf{GL}(n, A)$ (A một vành): II, § 10, no. 7.
$^tX^{-1}$ (X một ma trận bình phương khả nghịch): II, § 10, no. 7.
$\operatorname{diag}(a_i)_{i \in I}, \operatorname{diag}(a_1, a_2, \ldots, a_n)$: II, § 10, no. 7.
$X_1 \otimes X_2$ ($X_1, X_2$ các ma trận trên một vành giao hoán): II, § 10, no. 10.
$\operatorname{Tr}(X)$ (X một ma trận bình phương trên một vành giao hoán): II, § 10, no. 11.
$\operatorname{rg}(X)$ (X một ma trận trên một trường): II, § 10, no. 12.
$\deg(x)$ (x một phần tử của một nhóm phân bậc): II, § 11, no. 1.
$M(\lambda_0)$ (M một môđun phân bậc, $\lambda_0$ một phần tử của monoid các bậc): II, § 11, no. 2.
$\operatorname{Homgr}_A(M, N)$ (M, N các môđun phân bậc trên một vành phân bậc A): II, § 11, no. 6.
$\operatorname{Engr}_A(M), M^{*\operatorname{gr}}$ (M một môđun phân bậc): II, § 11, no. 6.
$M:N$ (M, N các môđun): II, § 1, Bài tập 24.

$$
\begin{bmatrix}
a & b \\
d & c
\end{bmatrix}
$$ (a, b, c, d các điểm trên một đường thẳng xạ ảnh): II, § 9, Bài tập 11.

$\mathbf{SL}(E)$ (E một không gian vectơ): II, § 10, Bài tập 12.
$\mathbf{PSL}(E)$ (E một không gian vectơ): II, § 10, Bài tập 14.
$x.y, xy$ (phép nhân trong một đại số): III, § 1, no. 1.
$E^0$ (E một đại số): III, § 1, no. 1.
$\operatorname{Hom}_{A-\operatorname{alg.}}(E, F)$ (E, F các A-đại số): III, § 1, no. 1.
$E/b$ (b một iđêan hai phía của một đại số E): III, § 1, no. 2.
$\hat{E}$ (E một đại số): III, § 1, no. 2.
$\eta_c, \eta_E, \eta$ (E một đại số, c một phần tử khả nghịch): III, § 1, no. 3.

T(u), N(u): III, § 2, no. 3.
\bar{u}: III, § 2, no. 4.
H: III, § 2, no. 5.
Lib_A(I), Libas_A(I), Libasc_A(I): III, § 2, no. 7.
U((x_i)_{i \in I}): III, § 2, no. 8.
A[(x_i)_{i \in I}], A[x_i]_{i \in I}: III, § 2, no. 9.
A[(X_i)_{i \in I}]: III, § 2, no. 9.
A[X_1, \ldots, X_n]: III, § 2, no. 9.
A[X], A[X, Y], A[X, Y, Z]: III, § 2, no. 9.
X^\nu (\nu \text{ một đa chỉ số}): III, § 2, no. 9.

\sum_s \xi_s e_s, \sum_s \xi_s . s (s \text{ các phần tử của một monoid}): III, § 2, no. 10.
A[[X_i]]_{i \in I}: III, § 2, no. 11.
\sum_\nu \alpha_\nu X^\nu: III, § 2, no. 11.
\omega(u), \omega_K(u) (u \text{ một chuỗi lũy thừa hình thức}): III, § 2, no. 11.

\bigotimes_{i \in I} E_i, E_1 \otimes_A E_2 \otimes \cdots \otimes_A E_n, E_1 \otimes E_2 \otimes \cdots \otimes E_n (E_i \text{ các A-đại số}): III, § 4, no. 1.
E^{\otimes n} (E \text{ một đại số}): III, § 4, no. 1.

\bigotimes_{i \in I} E_i (I \text{ một tập vô hạn, } E_i \text{ các đại số}): III, § 4, no. 5.

\bigotimes_{i \in I} u_i, \bigotimes_{i \in I} x_i (u_i \text{ các đồng cấu đại số, } x_i \text{ các phần tử, I vô hạn}): III, § 4, no. 5.

\epsilon \bigotimes_{i \in I} E_i, \epsilon \bigotimes_{i \in I} f_i, \epsilon G^{\otimes n} (E_i, G \text{ các đại số phân bậc, } f_i \text{ các đồng cấu đại số phân bậc, } \epsilon \text{ một hệ các nhân tử giao hoán}): III, § 4, no. 7.

g \bigotimes_{i \in I} E_i, E^g \otimes_A F, gG^{\otimes n}, g \bigotimes_{i \in I} f_i, f_1 \otimes f_2, gf^{\otimes n}: III, § 4, no. 7.

\bigotimes^n M, T^n(M), \mathrm{Tens}^n(M), T^n_A(M), T(M), \mathrm{Tens}(M), T_A(M) (M một A-môđun): III, § 5, no. 1.
T(u), T^n(u) (u \text{ một ánh xạ tuyến tính}): III, § 5, no. 2.
T_J^1(M), T_q^p(M) (M một môđun): III, § 5, no. 6.
\alpha_q^f(z), e_f^g: III, § 5, no. 6.
\alpha_{v_p}^{\lambda \cdots \mu}: III, § 5, no. 6.
c_j^i: III, § 5, no. 6
S(M), S_A(M), \mathrm{Sym}(M): III, § 6, no. 1.
\mathfrak{g}', \mathfrak{g}'_M, \mathfrak{g}'_n: III, § 6, no. 1.
S^n(M), S^n(u), S(u) (M một môđun, u một ánh xạ tuyến tính): III, § 6, nos. 1 and 2.
s.z: III, § 6, no. 3.
e^\alpha (\alpha \text{ một đa chỉ số}): III, § 6, no. 6.
\wedge(M), \wedge_A(M), \mathrm{Alt}(M): III, § 7, no. 1.
\mathfrak{g}'', \mathfrak{g}''_M, \mathfrak{g}''_n: III, § 7, no. 1.

$\wedge^n(M)$: III, § 7, no. 1.
$u \wedge v, x_1 \wedge x_2 \wedge \cdots \wedge x_n$: III, § 7, no. 1.
$\wedge(u), \wedge^n(u)$ ($u$ một ánh xạ tuyến tính): III, § 7, no. 2.
$x_H$ (H là một tập con của $\{1, n\}$): III, § 7, no. 3.
$u(x_1, \ldots, \hat{x}_j, \ldots, x_n)$: III, § 7, no. 4.
$a.z$: III, § 7, no. 4.
$A'_n(M), A''_n(M)$: III, § 7, no. 4.
$e_J$: III, § 7, no. 8.
$\rho_{J, K}$: III, § 7, no. 8.
$\det(u)$ ($u$ một tự đồng cấu): III, § 8, no. 1.
$\det(x_1, x_2, \ldots, x_n)$ ($x_j$ là các vectơ trong một A-môđun tự do $n$-chiều): III, § 8, no. 1.
$\det(X)$ ($X$ là một ma trận): III, § 8, no. 3.
$\det(\xi_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}, \det(\xi_{ij})$: III, § 8, no. 3.

$$
\begin{vmatrix}
\xi_{11} & \cdots & \xi_{1n} \\
\vdots & \ddots & \vdots \\
\xi_{n1} & \cdots & \xi_{nn}
\end{vmatrix}
$$
: III, § 8, no. 3.

$X_{H, K}, X^{H}$ ($X$ một ma trận): III, § 8, no. 5 và 6.
$\mathrm{SL}_n(A), \mathrm{SL}(n, A)$: III, § 8, no. 9.
$p.x$ ($p \in A[X]$, $x$ một phần tử của một A-môđun): III, § 8, no. 10.
$M_u, M[X]$ ($M$ một A-môđun, $u$ một tự đồng cấu): III, § 8, no. 10.
$\chi_u(X)$ ($u$ một tự đồng cấu A-môđun): III, § 8, no. 11.
$\mathrm{Tr}_{M/K}(a), N_{M/K}(a), \mathrm{Pc}_{M/K}(a; X)$ ($A$ một đại số trên K, $M$ một A-môđun, $a \in A$) : III, § 9, no. 1.
$\mathrm{Tr}_{A/K}(a), N_{A/K}(a), \mathrm{Pc}_{A/K}(a; X)$ ($A$ một đại số trên K, $a \in A$) : III, § 9, no. 3.
$D_{A/K}(x_1, \ldots, x_n)$ ($x_j$ các phần tử của một đại số trên K A): III, § 9, no. 5.
$[u, v]_g, [u, v]$ ($u, v$ các phần tử của một đại số phân bậc): III, § 10, no. 4.
$P(D), P(d_1, \ldots, d_n)$ ($P$ một đa thức, $d_j$ các dẫn xuất): III, § 10, no. 4.
$\mathrm{ad}_e(a), \mathrm{ad}(a)$ ($a$ một phần tử thuần nhất của một đại số phân bậc): III, § 10, no. 6.
$D_K(B, F)$ ($B$ một đại số trên K, $F$ một song môđun (B, B)): III, § 10, no. 7.
$D_{A, \rho}(B, F), D_A(B, F)$: III, § 10, no. 7.
$D_s$ ($s$ một tự đồng cấu): III, § 10, no. 9.
$\Omega_K(A), d_{A/K}(x), dx$ ($x$ một phần tử của một đại số trên K A): III, § 10, no. 11.
$D_iP, \partial P/\partial X_i$ ($P$ một đa thức): III, § 10, no. 11.
$\Omega(u), \Omega_0(u)$ ($u$ một đồng cấu vành): III, § 10, no. 12.
$\Omega_u$ ($u$ một đồng cấu đại số trên K): III, § 10, no. 12.
$M^{*gr}$ ($M$ một môđun phân bậc): III, § 11.
$u.v, u._mv$ ($u, v$ các ánh xạ đa tuyến tính đối xứng): III, § 11, no. 2.
$u \wedge v$ ($u, v$ các ánh xạ đa tuyến tính phản xứng): III, § 11, no. 2.
$\theta_T, \theta_S, \theta_\Lambda$: III, § 11, no. 5.

u \perp x, i(x): III, § 11, no. 6.
x \perp u, i'(x): III, § 11, no. 6.
x \perp u, i(u): III, § 11, no. 7.
u \perp x, i'(u): III, § 11, no. 7.
G_p(E), G_{n,p}(K): III, § 11, no. 13.
a(x, y, z): III, Phụ lục, no. 1.
ME: III, § 2, Bài tập 13.
E * F: III, § 5, Bài tập 6.
R[a]: III, § 6, Bài tập 4.
K[X; \sigma, d]: III, § 10, Bài tập 3.
\tilde{X}: III, § 11, Bài tập 9.

Nhóm Abel: I, § 4, no. 2.
Giá trị tuyệt đối của một số hữu tỉ: I, § 9, no. 4.
Tác động của một tập hợp lên một tập hợp khác: I, § 3, no. 1.
Tác động, chính tắc: I, § 3, no. 1.
Tác động, phân phối: I, § 3, no. 4.
Tác động, cảm sinh: I, § 3, no. 2.
Tác động, thương: I, § 3, no. 3.
Tác động phải, trái, dẫn xuất từ một luật hợp thành: I, § 3, no. 1.
Các tác động giao hoán với nhau: I, § 5, no. 4.
Phép cộng: I, § 1, no. 1.
Phép cộng các số nguyên hữu tỉ: I, § 2, no. 5.
Theo phép cộng (luật được viết): I, § 1, no. 1.
Phần tử liên hợp của một ma trận: III, § 11, Bài tập 9.
Phép nối một phần tử đơn vị (đại số được dẫn xuất bởi): III, § 1, no. 2.
Hàm affine: II, § 9, no. 4.
Nhóm affine: II, § 9, no. 4.
Đường thẳng, mặt phẳng, siêu phẳng affine: II, § 9, no. 3.
Ánh xạ affine: II, § 9, no. 4.
Không gian affine: II, § 9, no. 1.
Tập con affine, đa tạp tuyến tính: II, § 9, no. 3.
Họ tự do affine, họ liên quan affine: II, § 9, no. 3.
Các điểm độc lập affine: II, § 9, no. 3.
Đại số, A-đại số: III, § 1, no. 1.
Đại số alternative: III, Phụ lục, no. 1.
Đại số phân bậc phản xứng: III, § 4, no. 9.
Đại số phân bậc phản giao hoán: III, § 4, no. 9.
Đại số kết hợp: III, § 1, no. 1.
Đại số Cayley: III, § 2, no. 4.
Đại số giao hoán: III, § 1, no. 1.

Đại số dẫn xuất từ một đại số bằng phép nối một phần tử đơn vị: III, § 1, no. 2.
Đại số ngoài của một môđun: III, § 7, no. 1.
Đại số tự do: III, § 2, no. 7.
Đại số kết hợp tự do: III, § 2, no. 7.
Đại số kết hợp và giao hoán tự do: III, § 2, no. 7.
Đại số tự do của một môđun: III, § 2, Bài tập 13.
Đại số được sinh bởi các phần tử sinh thỏa mãn các quan hệ: III, § 2, no. 8.
Đại số phân bậc trên một vành phân bậc: III, § 3, no. 1.
Đại số toàn phần của một monoid: III, § 2, no. 10.
Đại số thu được bằng mở rộng các vô hướng: III, § 1, no. 5.
Đại số thu được bằng hạn chế các vô hướng: III, § 1, no. 5.
Đại số của một nhóm, của một magma, của một monoid: III, § 2, no. 6.
Đại số các số đối ngẫu: III, § 2, no. 3.
Đại số các chuỗi lũy thừa hình thức: III, § 2, no. 11.
Đại số các quaternion Hamilton: III, § 2, no. 5.
Đại số các octonion kiểu $(\alpha, \beta, \gamma, \delta)$: III, Phụ lục, no. 3.
Đại số các quaternion: III, § 2, no. 5.
Đại số các quaternion kiểu $(\alpha, \beta, \gamma)$, kiểu $(\alpha, \gamma)$: III, § 2, số 5.
Đại số đối: III, § 1, no. 1.
Đại số tích: III, § 1, no. 4.
Đại số toàn phương: III, § 2, no. 3.
Đại số toàn phương kiểu $(\alpha, \beta)$: III, § 2, no. 3.
Đại số thương: III, § 1, no. 4.
Đại số Rees: III, § 6, Bài tập 4.
Đại số hạn chế của một monoid: III, § 2, no. 10.
Đại số đối xứng của một môđun: III, § 6, no. 1.
Đại số tenxơ của một môđun: III, § 5, no. 1.
Đại số có đơn vị: III, § 1, no. 1.
Đại số phổ quát được xác định bởi một hệ sinh liên quan bởi một họ các quan hệ: III, § 2, no. 8.
Đại số phổ quát được sinh bởi một tập hợp chịu các đồng nhất thức: III, § 2, no. 8.
Đại số phổ quát kết hợp có đơn vị, được xác định bởi một hệ sinh liên quan bởi một họ các quan hệ: III, § 2, no. 8.
Các đại số rời nhau tuyến tính: III, § 4, no. 4.
Đại số phân bậc phản xứng: III, § 4, no. 9.
Nhóm phản xứng: III, § 5, no. 7.
Ánh xạ đa tuyến tính phản xứng: III, § 7, no. 4.
Đại số alternative: III, Phụ lục, no. 1.
Tổng dính: I, § 7, no. 3.
Bị triệt tiêu bởi một vô hướng (phần tử): II, § 1, no. 12.
Linh hóa tử trái, phải: I, § 8, no. 6.
Linh hóa tử của một tập con, của một phần tử của một môđun: II, § 1, no. 12.

Phản tự đẳng cấu: III, § 1, no. 1.
Đối đối giao hoán phân bậc đối đại số: III, § 11, no. 3.
Đối giao hoán phân bậc lệch đối đại số: III, § 11, no. 4.
Đại số phản giao hoán phân bậc: III, § 4, no. 9.
Đại số phản giao hoán phân bậc lệch đối đại số: III, § 11, no. 4.
Đối đạo hàm, K-đối đạo hàm: III, § 10, no. 2.
Phản đồng cấu của một vành: II, § 10, no. 6.
Liên kết (B-môđun) với một A-môđun và một đồng cấu vành B → A:
II, § 1, no. 13.
Liên kết (môđun trung thành) với một môđun: II, § 1, no. 12.
Liên kết (luật tác động) với một tác động: I, § 3, no. 1.
Liên kết (ánh xạ tuyến tính) với một ánh xạ tuyến tính afin: II, § 9, no. 4.
Liên kết (không gian vectơ) với một môđun trên một miền nguyên: II, § 7, no. 10.
Liên kết (không gian con vectơ) với một phần tử thuần nhất của một đại số ngoài: III, § 7, no. 2.
Liên kết (không gian con vectơ) với một phần tử thuần nhất của một đại số đối xứng: III, § 6, no. 2.
Liên kết (không gian con vectơ) với một phần tử thuần nhất của một đại số tenxơ: III, § 5, no. 2.
Đại số kết hợp: III, § 1, no. 1.
Đại số kết hợp, tự do: III, § 2, no. 7.
Đại số kết hợp và giao hoán, tự do: III, § 2, no. 7.
Luật kết hợp: I, § 1, no. 3.
Các quan hệ tính kết hợp trong một bảng phép nhân: III, § 1, no. 7.
Định lý tính kết hợp: I, § 1, no. 3.
Phần tử kết hợp: III, Phụ lục, no. 1.
Gắn (không gian afin) vào một không gian vectơ: II, § 9, no. 3.
Phép tăng: III, § 10, no. 8.
Tự đẳng cấu, nội của một nhóm: I, § 5, no. 3.
Tự đẳng cấu, nội, của một vành: I, § 8, no. 4.
Tự đẳng cấu không có điểm bất động: I, § 6, Bài tập 23.

Trọng tâm của m điểm, trọng tâm của một họ các điểm có trọng số: II, § 9, no. 2.
Tọa độ trọng tâm: II, § 9, no. 3.
Các cơ sở đối ngẫu với nhau: II, § 2, no. 7.
Họ cơ bản trong một nhóm: I, § 7, no. 6.
Cơ sở đối ngẫu của một cơ sở của môđun: II, § 2, no. 6.
Cơ sở Hamel: II, § 7, no. 1.
Cơ sở của một môđun: II, § 1, no. 11.
Cơ sở của một đại số: III, § 1, no. 7.
Cơ sở của $T_I^J(M)$ liên kết với một cơ sở của M: III, § 5, no. 6.

Cơ sở kiểu $(\alpha, \beta)$ của một đại số bậc hai: III, § 2, no. 3.
Cơ sở kiểu $(\alpha, \beta, \gamma)$, kiểu $(\alpha, \gamma)$, của một đại số quaternion: III, § 2, no. 5.
Cơ sở, xạ ảnh: II, § 9, Bài tập 10.
Song cộng, ánh xạ song tuyến tính $\mathbf{Z}$: II, § 3, no. 1.
Đối tâm hóa kép: I, § 1, no. 5.
Đối tâm hóa kép của một đại số con: III, § 1, no. 2.
Nhóm hai chu kỳ: I, § 6, Bài tập 26.
Đối ngẫu kép của một môđun: II, § 2, no. 7.
Đối đại số, phản giao hoán, đối đối giao hoán, phân bậc lệch: III, § 11, no. 4
Đối đại số, đối giao hoán, giao hoán, phân bậc: III, § 11, no. 4.
Đối đại số, đối đại số phân bậc, đối đại số phân bậc lệch, III, § 11, no. 4.
Đối đại số của một nửa nhóm: III, § 11, no. 4.
Nhóm, vành, môđun phân bậc kép: II, § 11, no. 2.
Phân bậc kép: II, § 11, no. 1.
Ánh xạ song tuyến tính: II, § 3, no. 5.
Song môđun, song môđun (A, B): II, § 1, no. 14.
Song môđun trên các đại số: III, § 4, no. 3.
Công thức nhị thức: I, § 8, no. 2.
Tích khối của các ma trận: II, § 10, no. 5.
Vành Boolean: I, § 9, Bài tập 8.
Ma trận viền: II, § 10, no. 1.
Ngoặc, ngoặc $\varepsilon$ của hai đạo hàm: III, § 10, no. 4.

Giản ước được, trái, phải, phần tử giản ước được: I, § 2, no 2.
Định lý Cartan-Brauer-Hua: I, § 9, Bài tập 18.
Đại số Cayley: III, § 2, no. 4.
Mở rộng Cayley của một đại số: III, § 2, no. 5.
Định lý Cayley-Hamilton: III, § 8, no. 11.
Chuẩn, vết Cayley: III, § 2, no. 4.
Các octonion Cayley: III, Phụ lục, no. 3.
Phần tử trung tâm: I, § 1, no. 5.
Mở rộng trung tâm: I, § 6, no. 1.
Phép vị tự trung tâm: II, § 1, no. 2.
Đồng cấu vành trung tâm: II, § 5, no. 3.
Chuỗi trung tâm, dưới: I, § 6, no. 3.
Đại hóa tử: I, § 5, no. 3.
Đại hóa tử của một đại số con của một đại số kết hợp: III, § 1, no. 2.
Đại hóa tử của một tập con: I, § 1, no. 5.
Đại hóa tử của một tập con của một trường: II, § 7, no. 7.
Đại số con đại hóa tử: III, § 1, no. 2.
Phần tử giao hoán hóa trung tâm: I, § 5, no. 3.
Tập con giao hoán hóa trung tâm: I, § 5, no. 3.
Tâm: I, § 1, no. 5.

Tâm của một đại số: III, § 1, no. 2.
Tâm của một ánh xạ tuyến tính xạ ảnh: II, § 9, no. 10.
Thay đổi tọa độ, các công thức của: II, § 10, no. 8.
Đặc số của một trường: I, § 9, Bài tập 4.
Đa thức đặc trưng của một ma trận: III, § 8, no. 11.
Nhóm con đặc trưng: I, § 5, no. 3.
Lớp, liên hợp: I, § 5, no. 4.
Lớp, tính lũy linh, của một nhóm: I, § 6, no. 3.
Lớp, tính giải được, của một nhóm: I, § 6, no. 4.
Đối đại số kết hợp: III, § 11, no. 2.
Đối đại số đối giao hoán: III, § 11, no. 4.
Đối đại số giao hoán: III, § 11, no. 2.
Ánh xạ đường chéo đối: II, § 1, no. 6.
Đối chiều của một đa tạp tuyến tính afin: II, § 9, no. 3.
Đối chiều của một không gian con vectơ: II, § 7, no. 3.
Các hệ số của một chuỗi lũy thừa hình thức: III, § 2, no. 11.
Các hệ số của một tổ hợp tuyến tính: II, § 1, no. 1.
Các hệ số của một đa thức: III, § 2, no. 9.
Các hệ số của một hệ phương trình tuyến tính: II, § 2, no. 8.
Phần bù đại số của một phần tử của một ma trận vuông: III, § 8, no. 6.
Đối đại số, A-đối đại số: III, § 11, no. 1.
Đối đại số, đối đối giao hoán phân bậc: III, § 11, no. 3.
Đối đại số, kết hợp: III, § 11, no. 2.
Đối đại số, đối giao hoán: III, § 11, no. 2.
Đối đại số, có đồng vị: III, § 11, no. 2.
Đối đại số, phân bậc: III, § 11, no. 1.
Đối đại số, đối: III, § 11, no. 1.
Đối ảnh của một ánh xạ tuyến tính: II, § 1, no. 3.
Nhóm trùng hợp: I, § 4, no. 8.
Đối hạt nhân của một ánh xạ tuyến tính: II, § 1, no. 3.
Cột của một ma trận: II, § 10, no. 1.
Tổ hợp, tuyến tính: II, § 2, no. 5.
Các tổ hợp tuyến tính hình thức (môđun của): II, § 1, no. 11.
Nhân tử giao hoán: III, § 10, no. 1.
Đại số giao hoán: III, § 1, no. 1.
Trường giao hoán: I, § 9, no. 1.
Đối đại số phân bậc giao hoán: III, § 11, no. 4.
Nhóm giao hoán tự do trên X: I, § 7, no. 5.
Nhóm giao hoán với các toán tử: I, § 4, no. 2.
Luật giao hoán: I, § 1, no. 5.
Magma giao hoán: I, § 1, no. 5.
Nửa nhóm giao hoán tự do trên X: I, § 7, no. 7.
Vành giao hoán: I, § 8, no. 1.

II, § 10, no. 2.
Đạo hàm riêng: III, § 10, no. 11.
Dẫn xuất (phần tử) từ một phần tử của đại số tự do bằng cách thế các phần tử vào các bất định: III, § 2, no. 8.

Phần tử dẫn xuất từ một phần tử của đại số kết hợp tự do bằng cách thế các phần tử vào các bất định: III, § 2, no. 8.
Nhóm dẫn xuất của một nhóm: I, § 6, no. 2.
Tác động trái, tác động phải dẫn xuất từ một luật hợp thành: I, § 3, no. 1.
Chuỗi dẫn xuất của một nhóm: I, § 6, no. 4.
Định thức, Cauchy: III, § 8, Bài tập 5.
Định thức của một ma trận: III, § 8, no. 3.
Định thức của một tự đồng cấu: III, § 8, no. 1.
Định thức của một dãy các vectơ: III, § 8, no. 1.
Định thức, Vandermonde: III, § 8, no. 6.
Các phần tử đường chéo của một ma trận bình phương: II, § 10, no. 7.
Ma trận đường chéo của các ma trận: II, § 10, no. 7.
Đường chéo của một ma trận bình phương, ma trận đường chéo: II, § 10, no. 7.
Biểu đồ khớp: II, § 1, no. 4.
Nhóm các hiệu: I, § 2, no. 4.
Monoid các hiệu: I, § 2, no. 4.
K-vi phân: III, § 10, no. 11.
Vi phân của một phần tử: III, § 10, no. 11.
Nhóm nhị diện: I, § 6, Bài tập 4.
Phép co giãn: II, § 10, Bài tập 11.
Chiều của một môđun tự do: II, § 7, no. 2.
Chiều của một đa tạp tuyến tính affine: II, § 9, no. 3.
Chiều của một không gian affine: II, § 9, no. 1.
Chiều của một không gian xạ ảnh: II, § 9, no. 5.
Chiều của một không gian vectơ: II, § 7, no. 2.
Đẳng hình: II, § 1, no. 13.
Phân tích trực tiếp của một vành: I, § 8, no. 11.
Nhân tử trực tiếp: I, § 4, no. 9.
Giới hạn trực tiếp: xem Giới hạn, trực tiếp.
Tích trực tiếp: I, § 4, no. 9.
Tích trực tiếp, nội tại: I, § 4, no. 9.
Tổng trực tiếp: I, § 4, no. 9.
Hệ trực tiếp: xem Hệ, trực tiếp.
Phương của một đa tạp tuyến tính affine: II, § 9, no. 3.
Các tham số phương của một đường thẳng affine: II, § 9, no. 3.
Vectơ phương của một đường thẳng affine: II, § 9, no. 3.
Iđêan biệt thức của một đại số: III, § 9, no. 5.
Biệt thức của một dãy hữu hạn trong một đại số: III, § 9, no. 5.
Tác động phân phối: I, § 3, no. 4.
Luật phân phối, phân phối trái, phân phối phải: I, § 3, no. 4.
Ánh xạ phân phối đối với một chỉ số: I, § 3, no. 4.
Tính phân phối của một luật hợp thành đối với một luật khác: I, § 3, no. 5.
Ước trái, phải: I, § 8, no. 1.

Ước của không, trái, phải: I, § 8, no. 1.
Miền nguyên, miền nguyên: I, § 9, no. 2.
Lớp kề kép đối với hai nhóm con: I, § 5, no. 4.
Các cơ sở đối ngẫu: II, § 2, nos. 6 và 7.
Đối ngẫu phân bậc của một môđun phân bậc: II, § 11, no. 6.
Đại số các số đối ngẫu: III, § 2, no. 3.
Đối ngẫu của một môđun: II, § 2, no. 3.

Phần tử, trung tâm: I, § 1, no. 5.
Phần tử giao hoán với một tập con: I, § 5, no. 3.
Phần tử dẫn xuất từ một phần tử của đại số tự do bằng cách thế các phần tử vào các bất định: III, § 2, no. 8.
Phần tử dẫn xuất từ một phần tử của đại số kết hợp tự do bằng cách thế các phần tử vào các bất định: III, § 2, no. 8.
Phần tử, tự do, của một môđun: II, § 1, no. 11.
Phần tử, thuần nhất (thuần nhất bậc $n$), của một nhóm phân bậc: II, § 11, no. 1.
Phần tử, đơn vị: I, § 2, no. 1.
Phần tử bất biến dưới một toán tử: I, § 3, no. 2.
Phần tử, đẳng bậc, của một nhóm phân bậc: II, § 11, no. 1.
Phần tử, giản ước được trái, giản ước được phải, giản ước được: I, § 2, no. 2.
Phần tử, khả nghịch trái, khả nghịch phải, khả nghịch: I, § 2, no. 3.
Phần tử, chính quy trái, chính quy phải, chính quy: I, § 2, no. 2.
Phần tử chuẩn hóa một tập con: i, § 5, no. 3.
Phần tử, $p$-chính quy: I, § 6, Bài tập 28.
Phần tử, $p$-unipotent: I, § 6, Bài tập 28.
Phần tử, nguyên thủy, trong một nhóm tự do: I, § 7, Bài tập 26.
Phần tử, nguyên thủy, của một đại song đại số phân bậc: III, § 11, no. 8.
Phần tử thu được từ việc thế các phần tử vào các bất định trong một nhóm tự do: I, § 7, no. 5.
Phần tử, lân cận-s, I, § 7, Bài tập 18.
Phần tử xoắn của một môđun: II, § 7, no. 10.
Phần tử, đơn vị: I, § 2, no. 1.
Phần tử, đơn vị, của một đại số: III, § 1, no. 1.
Phần tử, không: I, § 2, no. 1.
Các phần tử đồng dư modulo một iđêan: I, § 8, no. 7.
Các phần tử liên hợp, trong một nhóm: I, § 5, no. 4.
Các phần tử liên hợp, dưới phép toán của một nhóm: I, § 5, no. 4.
Các phần tử đường chéo, của một ma trận bình phương: II, § 10, no. 7.
Các phần tử phụ thuộc tuyến tính (độc lập tuyến tính) trong một môđun: II, § 1, no. 11.
Các phần tử trực giao: II, § 2, no. 4.
Các phần tử hoán vị được, các phần tử giao hoán với nhau: I, § 1, no. 5.

Ma trận rỗng: II, § 10, no. 1.
Tự đồng cấu: I, § 1, no. 1.
Tự đồng cấu của một môđun: II, § 1, no. 2.
Tự đồng cấu của một vành: I, § 8, no. 4.
Tự đồng cấu, đơn môđula: III, § 8, no. 1.
Các tự đồng cấu tương đương, đồng dạng: III, § 8, Bài tập 26.
Số đầu mút, số các đầu mút: I, § 7, Bài tập 37.
Bao đơn ánh của một môđun: II, § 2, no. 1.
Phương trình, tuyến tính, phương trình tuyến tính thuần nhất, phương trình tuyến tính thuần nhất liên kết với một phương trình tuyến tính: II, § 2, no. 8.
Phương trình của một siêu phẳng: II, § 7, no. 5.
Phương trình tuyến tính vô hướng: II, § 2, no. 8.
Các phương trình tuyến tính (hệ): II, § 2, no. 8.
Các phương trình (hệ) của một không gian con vectơ: II, § 7, no. 5.
Các chuỗi hợp thành tương đương: I, § 4, no. 7.
Các tự đồng cấu tương đương: III, § 8, Bài tập 26.
Các ma trận tương đương: II, § 10, no. 9.
Phép hoán vị chẵn: I, § 5, no. 7.
Biểu đồ khớp: II, § 1, no. 4.
Dãy khớp: II, § 1, no. 4.
Khai triển theo một cột: III, § 8, no. 6.
Khai triển theo một hàng: III, § 8, no. 6.
Khai triển Laplace: III, § 8, no. 6.
Mở rộng Cayley của một đại số: III, § 2, no. 5.
Mở rộng trung tâm: I, § 6, no. 1.
Mở rộng cốt yếu của một môđun: II, § 2, Bài tập 15.
Mở rộng các luật của phép toán: I, § 5, no. 1.
Mở rộng một nhóm bởi một nhóm khác: I, § 6, no. 1.
Mở rộng một môđun bởi một môđun khác: II, § 1, no. 4.
Mở rộng vô hướng (môđun thu được bởi): II, § 5, no. 1.
Mở rộng vô hướng (đại số thu được bởi): III, § 1, no. 5.
Mở rộng tầm thường: I, § 6, no. 1.
Mở rộng tầm thường của một môđun: II, § 1, no. 9.
Đại số ngoài của một môđun: III, § 7, no. 1.
Lũy thừa ngoài $p$-th của một tự đồng cấu: III, § 7, no. 4.
Lũy thừa ngoài $p$-th của một ma trận: III, § 8, no. 5.
Lũy thừa ngoài $p$-th của một môđun: III, § 7, no. 4.
Tích ngoài của một $p$-vectơ và một $q$-vectơ: III, § 7, no. 1.
Phép toán ngoài của hợp thành: I, § 3, no. 1.

Nhân tử trực tiếp của một nhóm: I, § 4, no. 9.
Nhân tử trực tiếp của một môđun: II, § 1, no. 9.
Nhân tử của một tích: I, § 1, no. 2.

Hệ các nhân tử: III, § 2, Bài tập 11.
Trung thành (môđun vận hành): I, § 5, no. 1.
Môđun trung thành: III, § 1, no. 12.
Họ tự do afin, liên quan afin của các điểm trong một không gian afin: II, § 9, no. 3.
Họ cơ bản, tự do, sinh trong một nhóm: I, § 7, no. 6.
Họ tự do, liên quan của các phần tử của một môđun: II, § 1, no. 11.
Họ sinh của một đại số: III, § 1, no. 2.
Họ trực giao của các phép chiếu: II, § 1, no. 8.
Họ tự do xạ ảnh, liên quan xạ ảnh của các điểm trong một không gian xạ ảnh: II, § 9, no. 7.
Tích sợi: I, § 4, no. 8.
Trường: I, § 9, no. 1.
Trường, giao hoán, trường không giao hoán: I, § 9, no. 1.
Trường phân thức của một miền nguyên: I, § 9, no. 2.
Trường phân thức trái: I, § 9, Bài tập 15.
Trường số hữu tỉ: I, § 9, no. 4.
Trường xạ ảnh: II, § 9, no. 9.
Chuỗi hợp thành mịn hơn: I, § 4, no. 7.
Nhóm hữu hạn: I, § 4, no. 1.
Nhóm sinh hữu hạn: I, § 7, Bài tập 16.
Môđun hữu hạn sinh: II, § 1, no. 7.
Tập phần tử giữ cố định của một tập hợp: I, § 5, no. 2.
Phép giữ cố định một tập con của một tập hợp (toán tử, tập các toán tử): I, § 5, no. 2.
Dạng song tuyến tính chính tắc: II, § 2, no. 3.
Dạng tọa độ: II, § 2, no. 6.
Dạng tuyến tính: II, § 2, no. 3.
Dạng $n$-tuyến tính: II, § 3, no. 9.
$n$-dạng: III, § 11, no. 7.
Công thức nhị thức: I, § 8, no. 2.
Công thức Leibniz: III, § 10, no. 4.
Các công thức Cramer: III, § 8, no. 7.
Các công thức đổi tọa độ: II, § 10, no. 8.
Các công thức về tính bắc cầu của chuẩn và vết: III, § 9, no. 4.
Phân thức (trường của) của một miền nguyên: I, § 9, no. 2.
Nhóm phân thức của một nửa nhóm: I, § 2, no. 4.
Nửa nhóm phân thức, với mẫu thuộc S: I, § 2, no. 4.
Vành phân thức, với mẫu thuộc S: I, § 8, no. 12.
Vành phân thức toàn phần: I, § 8, no. 12.
Đại số tự do, đại số kết hợp, đại số kết hợp và giao hoán: III, § 2, no. 7.
Đại số tự do của một môđun: III, § 2, Bài tập 13.
Nhóm giao hoán tự do: I, § 7, no. 5.

Nửa nhóm giao hoán tự do: I, § 7, no. 7.
Phần tử tự do, họ tự do, môđun tự do, tập con tự do, hệ tự do: II, § 1, no. 11, và (do lạm dụng ngôn ngữ) II, § 9, no. 7.
Họ tự do trong một nhóm: I, § 7, no. 6.
Nhóm tự do: I, § 7, no. 5.
Magma tự do: I, § 7, no. 1.
Nửa nhóm tự do: I, § 7, no. 2.
Tích tự do của các đại số: III, § 5, Bài tập 6.
Tích tự do của các nhóm: I, § 7, no. 3.
Vectơ tự do trong một không gian afin: II, § 9, no. 1.
Một cách tự do, nhóm vận hành: I, § 5, no. 4.
Hàm afin tuyến tính, hàm afin: II, § 9, no. 4.

Được sinh bởi một họ các cặp có thứ tự (quan hệ tương đương): I, § 1, no. 6.
Được sinh bởi một tập con (iđêan): I, § 8, no. 6, và III, § 1, no. 2.
Được sinh bởi một tập con (nhóm con ổn định): I, § 4, no. 3.
Được sinh bởi một tập con (tập con ổn định): I, § 1, no. 4.
Được sinh bởi một tập con (đại số con): III, § 1, no. 2.
Được sinh bởi một tập con (trường con): I, § 9, no. 1.
Được sinh bởi một tập con (magma con): I, § 1, no. 4.
Được sinh bởi một tập con (vành con): I, § 8, no. 5.
Được sinh bởi một tập con (magma con có đơn vị, monoid con): I, § 2, no. 1.
Họ sinh của một nhóm: I, § 7, no. 6.
Họ sinh của một đại số: III, § 1, no. 2.
Tập sinh, hệ sinh, của một trường: I, § 9, no. 1.
Tập sinh, hệ sinh, của một magma: I, § 1, no. 4.
Tập sinh, hệ sinh, của một môđun: II, § 1, no. 7.
Tập sinh, hệ sinh, của một iđêan: I, § 8, no. 6.
Tập sinh, hệ sinh, của một vành: I, § 8, no. 5.
Tập sinh, hệ sinh, của một nhóm con ổn định: I, § 4, no. 3.
Tập sinh, hệ sinh, của một tập con ổn định: I, § 1, no. 4.
Tập sinh, hệ sinh, của một magma con có đơn vị, của một monoid con: I, § 2, no. 1.
Các sinh của một biểu diễn: I, § 7, no. 6.
Đại số phân bậc trên một vành phân bậc: III, § 3, no. 1.
Đại bigebra phân bậc: III, § 11, no. 4.
Đại bigebra phân bậc, xiên: III, § 11, no. 4.
Đồng bigebra phân bậc: III, § 11, no. 1.
Nhóm, môđun, vành phân bậc: II, § 11, nos. 1 and 2.
Đồng cấu phân bậc: II, § 11, no. 2.
Đại số con phân bậc: III, § 3, no. 2.
Vành con, môđun con, iđêan phân bậc: II, § 11, no. 3.
Tích tenxơ phân bậc kiểu $\Delta_0$: III, § 4, no. 8.

Phân bậc tương thích với một đồng tích: III, § 11, no. 1.
Phân bậc tương thích với một cấu trúc đại số: III, § 3, no. 1.
Phân bậc cảm sinh, phân bậc thương: II, § 11, no. 3.
Phân bậc kiểu Δ: II, § 11, no. 1.
Phân bậc, bộ phận, phân bậc toàn phần: II, § 11, nos. 1 and 2.
Phân bậc, tầm thường: II, § 11, no. 1.
Grassmannian: III, § 11, no. 13.
Các quan hệ Grassmann: III, § 11, no. 13.
Ước chung lớn nhất (u.c.l.n.) của hai số nguyên: I, § 8, no. 11.
Nhóm: I, § 2, no. 3.
Nhóm cộng tính của một vành: I, § 8, no. 1.
Nhóm afin: I, § 9, no. 4.
Nhóm phản xứng: I, § 5, no. 7.
Nhóm hai chu kỳ: I, § 6, Bài tập 26.
Nhóm phân bậc kép: II, § 11, no. 2.
Nhóm trùng nhau của hai đồng cấu: I, § 4, no. 8.
Giao hoán tử nhóm: I, § 6, no. 2.
Nhóm chu kỳ: I, § 4, no. 10.
Nhóm xác định bởi các sinh và các quan hệ: I, § 7, no. 6.
Nhóm dẫn xuất: I, § 6, no. 2.
Nhóm diedral: I, § 6, Bài tập 4.
Nhóm hữu hạn, nhóm vô hạn: I, § 4, no. 1.
Nhóm sinh hữu hạn: I, § 7, Bài tập 16.
Nhóm có biểu diễn hữu hạn: I, § 7, Bài tập 16.
Nhóm giao hoán tự do, trên một tập hợp: I, § 7, no. 7 và II, § 1, no. 11.
Nhóm tự do, trên một tập hợp: I, § 7, no. 5.
Nhóm phân bậc: II, § 11, no. 1.
Nhóm tuyến tính: II, § 2, no. 6.
Nhóm đơn cực tiểu: I, § 6, Bài tập 27.
Nhóm đơn sinh: I, § 4, no. 10.
Nhóm nhân của một vành: I, § 8, no. 1.
Nhóm lũy linh, nhóm lũy linh lớp $n$: I, § 6, no. 3.
Nhóm hiệu, nhóm phân thức: I, § 2, no. 4.
Nhóm kiểu mũ: I, § 7, Bài tập 39.
Nhóm tác động trung thành: I, § 5, no. 1.
Nhóm tác động tự do: I, § 5, no. 4.
Nhóm tác động đơn bắc cầu: I, § 5, no. 6.
Nhóm tác động bắc cầu: I, § 5, no. 5.
$p$-nhóm: I, § 6, no. 5.
Nhóm xạ ảnh: II, § 9, no. 10.
Nhóm hữu hạn dư: I, § 5, Bài tập 5.
Nhóm giải được, nhóm giải được lớp $n$: I, § 6, no. 4.
Nhóm tuyến tính đặc biệt: III, § 8, no. 9.

Nhóm siêu giải được: I, § 6, Bài tập 26.
Nhóm đối xứng: I, § 4, no. 1.
Nhóm đơn môđula: III, § 8, no. 9.
Nhóm với các toán tử, Abel, giao hoán: I, § 4, no. 2.
Nhóm với các toán tử: I, § 4, no. 2.
Tích của nhóm với các toán tử: I, § 4, no. 8.
Tích (hoặc tích trong) của nhóm với các toán tử, của một họ các nhóm thương: I, § 4, no. 8.
Nhóm thương với các toán tử: I, § 4, no. 4.
Nhóm đơn với các toán tử: I, § 4, no. 4.
Groupoid: I, § 4, Bài tập 23.

Định lý Hall: I, § 6, Bài tập 10.
Cơ sở Hamel: II, § 7, no. 1.
Các quaternion Hamilton: III, § 2, no. 5.
Phần tử thuần nhất trong một nhóm phân bậc: II, § 11, no. 1.
G-tập thuần nhất: I, § 5, no. 5.
Phương trình tuyến tính thuần nhất, hệ tuyến tính: II, § 2, no. 8.
Tập con thuần nhất bậc $p$ trong một chuỗi lũy thừa hình thức: III, § 2, no. 11.
Tập con thuần nhất bậc $p$ đối với một số bất định trong một chuỗi lũy thừa hình thức: III, § 2, no. 11.
Đồng cấu đại số: III, § 1, no. 1.
Đồng cấu A-môđun, A-đồng cấu: II, § 1, no. 2.
Đồng cấu vành trung tâm: II, § 5, no. 3.
Đồng cấu chéo: I, § 6, Bài tập 7.
Đồng cấu cốt yếu: II, § 2, Bài tập 15.
Đồng cấu đối với hai luật hợp thành: I, § 1, no. 1.
Đồng cấu phân bậc: II, § 11, no. 2.
Đồng cấu đại số phân bậc: II, § 11, no. 2.
Đồng cấu nhóm: I, § 4, no. 1.
Đồng cấu monoid: I, § 2, no. 1.
Đồng cấu M-tập: I, § 5, no. 1.
Đồng cấu đa nút: II, § 1, no. 14.
Đồng cấu của các nhóm với các toán tử: I, § 4, no. 2.
$\phi$-đồng cấu: I, § 3, no. 1.
Đồng cấu phép chiếu: I, § 4, no. 8.
Đồng cấu vành: I, § 8, no. 4.
Đồng cấu tầm thường: I, § 2, no. 1.
Đồng cấu có đơn vị: I, § 2, no. 1.
Đồng cấu đại số có đơn vị: III, § 1, no. 1.
Phép vị tự: I, § 4, no. 2 và II, § 1, no. 1.
Phép vị tự trung tâm: II, § 1, no. 2 và III, § 9, Bài tập 6.
Siêu phẳng afin: II, § 9, no. 3.

Siêu phẳng ở vô tận: II, § 9, no. 8.
Siêu phẳng đi qua 0 trong một không gian vectơ: II, § 7, no. 3.
Siêu phẳng xạ ảnh: II, § 9, no. 7.
Siêu phẳng xạ ảnh, được lấy làm siêu phẳng ở vô tận: II, § 9, no. 10.

Đối, nhóm: I, § 1, no. 1.
Magma, kết hợp: I, § 1, no. 3.
Magma, giao hoán: I, § 1, no. 5.
Magma, xác định bởi các phần tử sinh và các quan hệ: I, § 7, no. 1.
Magma, tự do, trên một tập hợp: I, § 7, no. 1.
Magma của các ánh xạ vào một magma: I, § 1, no. 1.

Magma, đối: I, § 1, no. 1.
Magma, tích: I, § 1, no. 1.
Magma, thương: I, § 1, no. 6.
Magma, có đơn vị: I, § 2, no. 1.
Magma, đẳng cấu: I, § 1, no. 1.
Ánh xạ, affine tuyến tính, affine: II, § 9, no. 4.
Ánh xạ, phản xứng đa tuyến tính: III, § 7, no. 4.
Ánh xạ, bi-cộng tính, $\mathbf{Z}$-song tuyến tính: II, § 3, no. 1.
Ánh xạ, C-song tuyến tính: II, § 3, no. 5.
Ánh xạ tương thích với một tác động: I, § 3, no. 1.
Ánh xạ tương thích với phép toán của một monoid: I, § 5, no. 1.
Ánh xạ phân phối đối với một biến: I, § 3, no. 4.
Ánh xạ, tuyến tính, A-tuyến tính: II, § 1, no. 2.
Ánh xạ, tuyến tính, $A_s(T) \to E$ được xác định bởi một ánh xạ $T \to E$: II, § 1, no. 11.
Ánh xạ, tuyến tính, liên kết với một ánh xạ affine: II, § 9, no. 4.
Ánh xạ, đa cộng tính, $\mathbf{Z}$-đa tuyến tính: II, § 3, no. 9.
Ánh xạ, C-đa tuyến tính: II, § 3, no. 9.
Ánh xạ, quỹ đạo: I, § 5, no. 4.
Ánh xạ, xạ ảnh tuyến tính, xạ ảnh: II, § 9, no. 10.
Ánh xạ, tuyến tính khả nghịch phải, tuyến tính khả nghịch trái: II, § 1, no. 9.
Ánh xạ, nửa tuyến tính: II, § 1, no. 13.
Ánh xạ, đối xứng đa tuyến tính: III, § 6, no. 3.
Các ma trận chỉ khác nhau bởi cấp của các cột, các hàng: II, § 10, no. 9.
Các ma trận, tương đương: II, § 10, no. 9.
Các ma trận, vuông đồng dạng: II, § 10, no. 9.
Ma trận, đối liên hợp, của một ma trận khả nghịch: II, § 10, no. 7.
Ma trận, đường chéo: II, § 10, no. 7.
Ma trận, rỗng: II, § 10, no. 1.
Ma trận, khả nghịch: II, § 10, no. 7.
Ma trận, tam giác dưới, tam giác trên: II, § 10, no. 7.
Ma trận, ma trận kiểu $(p, q)$: II, § 10, no. 1.
Ma trận, đơn thức: II, § 10, no. 7.
Ma trận thu được bằng cách viền một ma trận: II, § 10, no. 1.
Ma trận thu được bằng cách bỏ các cột, các hàng: II, § 10, no. 1.
Ma trận của một ánh xạ tuyến tính đối với hai cơ sở: II, § 10, no. 4.
Ma trận của một hệ tuyến tính: II, § 10, no. 4.
Ma trận của một phần tử đối với một cơ sở: II, § 10, no. 4.
Ma trận của một tự đồng cấu đối với một cơ sở: II, § 10, no. 7.
Ma trận của một phép hoán vị: II, § 10, no. 7.
Ma trận của một ánh xạ nửa tuyến tính đối với hai cơ sở: II, § 10, no. 6.
Ma trận chuyển từ một cơ sở này sang một cơ sở khác: II, § 10, no. 8.
Ma trận, vô hướng: II, § 10, no. 7.

Ma trận, vuông, ma trận vuông cấp $n$: II, § 10, no. 7.
Ma trận, đơn môđula: III, § 8, no. 4.
Các đơn vị ma trận: II, § 10, no. 3.
Ma trận chỉ có các số không bên dưới (bên trên) đường chéo: II, § 10, no. 7.
Ma trận, không: II, § 10, no. 2.
Iđêan cực đại: I, § 8, no. 6.
Trung bình G: I, § 6, Bài tập 8.
Các nhóm con ổn định chuẩn cực tiểu: I, § 4, Bài tập 15.
Nhóm đơn cực tiểu: I, § 6, Bài tập 27.
Minor, minor cấp $p$ của một ma trận: III, § 8, no. 5.
Các minor, bổ sung: III, § 8, no. 6.
Tenxơ hỗn hợp: III, § 5, no. 6.
Môđun, phân bậc hai: II, § 11, no. 2.
Môđun, chia được: II, § 7, Bài tập 33.
Môđun, đối ngẫu: II, § 2, no. 3.
Môđun, trung thành: II, § 1, no. 12.
Môđun, trung thành, liên kết với một môđun: II, § 1, no. 12.
Môđun, tự do: II, § 1, no. 11.
Môđun, tự do phân bậc: II, § 11, no. 2.
Môđun, phân bậc, môđun phân bậc với các bậc dương: II, § 11, no. 2.
Môđun, thương phân bậc: II, § 11, no. 3.
Môđun, không phân tích được: II, § 2, Bài tập 21.
Môđun, đơn ánh: II, § 2, Bài tập 11.
Môđun, trái, môđun phải, A-môđun: II, § 1, no. 1.
Môđun, đơn sinh: II, § 1, no. 12.
Môđun có độ dài hữu hạn: II, § 1, no. 10.
Môđun của các tổ hợp tuyến tính hình thức: II, § 1, no. 11.
Môđun của các quan hệ tuyến tính: II, § 1, no. 11.
Môđun trên một đại số: III, § 4, no. 3.
Môđun, tích: II, § 1, no. 5.
Môđun, xạ ảnh: II, § 2, no. 2.
Môđun, thương: II, § 1, no. 3.
Môđun, phản xạ: II, § 2, no. 7.
Môđun, không xoắn, trên một miền nguyên: II, § 7, no. 10.
Môđun, xoắn, trên một miền nguyên: II, § 7, no. 10.
Nhóm đơn sinh: I, § 4, no. 10.
Môđun đơn sinh: II, § 1, no. 2.
Monoid: I, § 2, no. 1.
Monoid được xác định bởi các phần tử sinh và các quan hệ: I, § 7, no. 2.
Monoid, tự do, trên một tập hợp: I, § 7, no. 2.
Monoid hiệu: I, § 2, no. 4.
Monoid phân thức với các mẫu số trong S: I, § 2, no. 4.
Monoid tác động trung thành trên một tập hợp: I, § 5, no. 1.

Tổng monoid: I, § 7, no. 3.
Đơn thức: III, § 2, no. 9.
Cấu xạ, đại số: III, § 1, no. 1.
Cấu xạ, A-môđun: II, § 1, no. 2.
Cấu xạ, đối đại số: III, § 11, no. 1.
Cấu xạ, đại số song phân bậc, cấu xạ đại số song phân bậc trái: III, § 11, no. 4.
Cấu xạ, đối đại số phân bậc: III, § 11, no. 1.
Cấu xạ, magma: I, § 1, no. 1.
Cấu xạ, monoid: I, § 2, no. 1.
Cấu xạ của các mở rộng: I, § 6, no. 1.
Cấu xạ, vành: I, § 8, no. 4.
Cấu xạ, đại số có đơn vị: III, § 4, no. 5.
Cấu xạ, magma có đơn vị: I, § 2, no. 1.
Cấu xạ-ϕ (ϕ là một đồng cấu của một monoid các toán tử vào một monoid khác):
    I, § 5, no. 1.
Cấu xạ-ϕ (ϕ là một ánh xạ của một tập hợp các toán tử vào một tập hợp khác): I, § 3, no. 1.
Cấu xạ-M (M là một monoid các toán tử): I, § 5, no. 1.
Cấu xạ-Ω (Ω là một tập hợp các toán tử): I, § 3, no. 1.
Đa cộng tính, Z-đa tuyến tính, ánh xạ: II, § 3, no. 9.
Đa bậc trong đại số tự do của một monoid: III, § 2, Bài tập 13.
Đa chỉ số: I, § 7, no. 7.
Dạng đa tuyến tính: II, § 3, no. 9.
Ánh xạ C-đa tuyến tính: II, § 3, no. 9.
Đa môđun: II, § 1, no. 14.
Đa môđun, thương: II, § 1, no. 14.
Bội, trái, phải: I, § 8, no. 1.
Phép nhân: I, § 1, no. 1.
Phép nhân trong một đại số. III, § 1, no. 1.
Bảng phép nhân: III, § 1, no. 7.
Nhóm nhân của một vành: I, § 8, no. 1.

Phần tử đối của một phần tử: I, § 2, no. 3.
Số nguyên hữu tỉ âm: I, § 2, no. 5.
Số hữu tỉ âm: I, § 9, no. 4.
Phần tử lân cận-S: I, § 7, Bài tập 18.
Định lý Nielson-Schreier: I, § 7, Bài tập 20.
Nhóm lũy linh, nhóm lũy linh cấp n: I, § 6, no. 3.
Chuẩn Cayley: III, § 2, no. 4.
Chuẩn trong một đại số bậc hai: III, § 2, no. 3.
Chuẩn của một phần tử trong một K-đại số đối với K: III, § 9, no. 3.
Chuẩn của một vô hướng đối với một môđun: III, § 9, no. 1.
Nhóm con ổn định chuẩn: I, § 4, no. 4.

Nhóm con chuẩn: I, § 4, no. 4.
Chuẩn hóa tử: I, § 5, no. 3.
Chuẩn hóa (phần tử, tập con) một tập con: I, § 5, no. 3.
Phần tử không: I, § 2, no. 1.
Số nguyên tố: I, § 4, no. 10.
Số hữu tỉ: I, § 9, no. 4.
Số (hữu tỉ), âm, dương, âm ngặt, dương ngặt: I, § 9, no. 4.
Tử số: I, § 2, no. 4.

Octonion Cayley: III, Phụ lục, no. 3.
Octonion kiểu ($\alpha, \beta, \gamma, \delta$) (đại số của): III, Phụ lục, no. 3.
Phép hoán vị lẻ: I, § 5, no. 7.
Phép toán bởi trái, phải, tịnh tiến: I, § 5, no. 1.
Phép toán, trái, phải (các luật của): I, § 5, no. 1.
Phép toán, trái, phải, của một monoid: I, § 5, no. 1.
Phép toán, đơn bắc cầu: I, § 5, no. 6.
Phép toán, bắc cầu: I, § 5, no. 5.
Phép toán, tầm thường: I, § 5, no. 2.
Toán tử: I, § 3, no. 1.
Đại số đối: III, § 1, no. 1.
Đối đại số đối: III, § 11, no. 1.
Luật đối: I, § 1, no. 1.
Magma đối: I, § 1, no. 1.
Đối với một M-tập, $M^0$-tập: I, § 5, no. 1.
Vành đối: I, § 8, no. 3.
Quỹ đạo: I, § 5, no. 4.
Ánh xạ quỹ đạo: I, § 5, no. 4.
Cấp, phần tử của vô hạn: I, § 4, no. 10.
Cấp của một chu trình: I, § 5, no. 7.
Cấp của một chuỗi lũy thừa hình thức đối với một số bất định nhất định: III, § 2, no. 11.
Cấp của một nhóm: I, § 4, no. 1.
Cấp của một phần tử trong một nhóm: I, § 4, no. 10.
Cấp của một ma trận vuông: II, § 10, no. 7.
Cấp, cấp toàn phần, của một chuỗi lũy thừa hình thức: III, § 2, no. 11.
Dãy có thứ tự: I, § 1, no. 2.
Các dãy có thứ tự, tương tự: I, § 1, no. 2.
Gốc: I, § 2, no. 1.
Gốc, lựa chọn, trong một không gian affine: II, § 9, no. 1.
Các phần tử trực giao, các tập hợp: II, § 2, no. 3.
Họ các phép chiếu trực giao: II, § 1, no. 8.
Môđun con trực giao với một tập con của E (resp. E$^*$): II, § 2, no. 4.

Các đa tạp tuyến tính song song: II, § 9, no. 3.
Hình bình hành: II, § 9, Bài tập 1.
Các tham số phương, của một đường thẳng affine: II, § 9, no. 3.
Đạo hàm riêng: III, § 10, no. 11.
Phân bậc bộ phận: II, § 11, no. 1.
Ma trận chuyển: II, § 10, no. 8.
Các phần tử giao hoán được: I, § 1, no. 5.
Phép hoán vị chẵn, lẻ: I, § 5, no. 7.
Mặt phẳng, affine: II, § 9, nos. 1 and 3.
Mặt phẳng đi qua 0 trong một không gian vectơ: II, § 7, no. 3.
Mặt phẳng, xạ ảnh: II, § 9, no. 5.
Điểm của một không gian affine: II, § 9, no. 1.
Điểm của một không gian xạ ảnh: II, § 9, no. 5.
Các điểm, độc lập affine: II, § 9, no. 3.
Các điểm ở vô hạn: II, § 9, no. 8.
Đa thức, đặc số, của một phần tử trong một đại số trên K: III, § 9, no. 3.
Đa thức, đặc số, của một tự đồng cấu: III, § 8, no. 11.
Đa thức, đặc số, của một vô hướng đối với một môđun: III, § 9, no. 1.
Đa thức không chứa số hạng theo X^v: III, § 2, no. 9.
Các đồng nhất thức đa thức: III, § 2, no. 9.
Đa thức bậc n: III, § 2, no. 9.
Các quan hệ đa thức: III, § 2, no. 9.
Đa thức không có số hạng hằng: III, § 2, no. 9.
Đa thức đối với một họ các bất định, với các hệ số trong một vành: III, § 2, no. 9.
Số nguyên hữu tỉ dương: I, § 2, no. 5.
Số hữu tỉ dương: I, § 9, no. 4.
Lũy thừa ngoài của một ánh xạ tuyến tính: III, § 7, no. 4.
Lũy thừa ngoài của một ma trận: III, § 8, no. 5.
Lũy thừa ngoài của một môđun: III, § 7, no. 4.
Lũy thừa thứ n, theo một luật kết hợp: I, § 1, no. 3.
Lũy thừa đối xứng của một ánh xạ tuyến tính, của một môđun: III, § 6, no. 3.
Lũy thừa tenxơ của một ánh xạ tuyến tính: III, § 5, no. 2.
Lũy thừa tenxơ của một môđun: III, § 5, no. 1.
Trình bày của một nhóm: I, § 7, no. 6.
Trình bày của một đại số: III, § 2, no. 8.
Được trình bày hữu hạn (nhóm): I, § 7, Bài tập 16.
Bảo toàn khi chuyển qua thương: I, § 1, no. 6.
Iđêan nguyên tố: I, § 9, no. 3.
Số nguyên tố: I, § 4, no. 10.
Nguyên tố cùng nhau (các số nguyên): I, § 8, no. 10.
Phần tử nguyên thủy trong một nhóm tự do: I, § 7, Bài tập 26.

Phần tử nguyên thủy trong một magma tự do sinh bởi một phần tử duy nhất: I, § 7, Bài tập 7.
Phần tử nguyên thủy của một đối đại số hai phía phân bậc: III, § 11, no. 8.
G-tập chính, thuần nhất: I, § 5, no. 6.
Iđêan chính: I, § 8, no. 6.
Chuỗi chính: I, § 4, Bài tập 17.
Tập chính dưới G, thuần nhất: I, § 5, no. 6.
Nguyên lý mở rộng bởi tính tuyến tính: II, § 1, no. 7.
Bài toán, tuyến tính: II, § 2, no. 8.
Đại số tích: III, § 1, no. 4.
Tích, khối, của các ma trận: II, § 10, no. 5.
Tích, chéo: III, § 2, Bài tập 11.
Tích, ngoài, của một $p$-vectơ và một $q$-vectơ: III, § 7, no. 1.
Tích, nửa trực tiếp ngoài, của G bởi F đối với $\tau$: I, § 6, no. 1.
Tích, thớ, của các nhóm có toán tử: I, § 4, no. 8.
Tích, thớ, của các môđun: II, § 1, Bài tập 4.
Tích, tự do, của các đại số: III, § 5, Bài tập 6.
Tích, tự do, của các nhóm: I, § 7, no. 5.
Tích tenxơ phân bậc của hai môđun phân bậc: II, § 11, no. 5.
Tích tenxơ phân bậc của các đại số phân bậc: III, § 4, nos. 7 and 9.
Nhóm tích, nhóm tích nội, của một họ các nhóm thương: I, § 4, no. 8.
Nhóm tích có toán tử: I, § 4, no. 8.
Tích, trực tiếp nội, tích trực tiếp, tích, của các nhóm con: I, § 4, no. 9.
Magma tích: I, § 1, no. 1.
Tích của các K'-cấu trúc: II, § 8, no. 3.
Tích của các luật hợp thành: I, § 1, no. 1.
Tích của các ma trận tính theo một ánh xạ: II, § 10, no. 2.
Tích của các ma trận tính trong một vành: II, § 10, no. 3.
Tích của các môđun: II, § 1, no. 5.
Tích của các đa môđun: II, § 1, no. 14.
Tích của một toán tử và một phần tử: I, § 3, no. 1.
Tích của một dãy có thứ tự: I, § 1, no. 2.
Tích của hai phần tử: I, § 1, no. 1.
Tích của các iđêan hai phía: I, § 8, no. 9.
Tích, (phải, trái) nội: III, § 11, nos. 6 and 7.
Vành tích: I, § 8, no. 10.
Tích, đối xứng, của các ánh xạ đa tuyến tính: III, § 11, no. 2.
Tích, tenxơ, của một họ các $\mathbf{Z}$-môđun đối với một bộ ba $(c, p, q)$: II, § 3, no. 9.
Tích, tenxơ, của các đại số: III, § 4, no. 1.
Tích, tenxơ, của một họ vô hạn các đại số: III, § 4, no. 5.
Tích, tenxơ, của các cơ sở của các đại số: III, § 4, no. 5.

Tích tenxơ, của các đối đại số: III, § 11, no. 1.
Tích tenxơ, của hai cơ sở: II, § 3, no. 7.
Tích tenxơ, của hai phần tử: II, § 3, no. 1.
Tích tenxơ, của hai ánh xạ tuyến tính: II, § 3, no. 2.
Tích tenxơ, của hai ma trận trên một vành giao hoán: II, § 10, no. 10
Tích tenxơ, của hai môđun: II, § 3, no. 1.
Tích tenxơ, của hai đa môđun: II, § 3, no. 4.
Tích tenxơ, của hai ánh xạ nửa tuyến tính: II, § 3, no. 3.
Đồng cấu phép chiếu: I, § 4, no. 8.
Trường xạ ảnh: II, § 9, no. 9.
Nhóm xạ ảnh: II, § 9, no. 10.
Siêu phẳng, phẳng xạ ảnh: II, § 9, no. 7.
Đường thẳng xạ ảnh: II, § 9, no. 5.
Ánh xạ xạ ảnh: II, § 9, no. 10.
Môđun xạ ảnh: II, § 2, no. 2.
Không gian xạ ảnh: II, § 9, các no. 5 và 11.
Tự do xạ ảnh, liên quan xạ ảnh, họ: II, § 9, no. 7.
Phép chiếu: II, § 1, no. 8.
Giả môđun trái, phải: II, Phụ lục, no. 2.
Giả vành: I, § 8, no. 1.
Giả vành có bình phương không: I, § 8, no. 3.
Vectơ $p$-nguyên thủy: III, § 11, no. 13.
Quaternion nguyên thủy: III, § 2, Bài tập 3.

Đại số bậc hai: III, § 2, no. 3.
Nửa nhóm: I, § 3, Bài tập 6.
Quaternion, nguyên thủy: III, § 2, Bài tập 3.
Đại số quaternion: III, § 2, no. 5.
Nhóm quaternion: I, § 6, Bài tập 4.
Đại số thương: III, § 1, no. 2.
Phân bậc thương: II, § 11, no. 3.
Nhóm thương với các toán tử: I, § 4, no. 4.
Luật thương: I, § 1, no. 6.
Magma thương: I, § 1, no. 11.
Môđun thương, không gian vectơ: II, § 1, no. 3.
Đa nút thương: II, § 1, no. 14.
Thương của một tác động: I, § 3, no. 3.
Vành thương: I, § 8, no. 7.
Các thương của một chuỗi hợp thành của một nhóm với các toán tử: I, § 4, no. 7.

Hạng của một nhóm tự do: I, § 7, Bài tập 14.
Hạng của một ánh xạ tuyến tính của các không gian vectơ: II, § 7, no. 4.
Hạng của một hệ tuyến tính trên một trường: II, § 7, no. 6.

Hạng của một ma trận trên một trường: II, § 10, no. 12.
Hạng của một ánh xạ tuyến tính afin: II, § 9, no. 4.
Hạng của một phần tử trong một tích tenxơ của các không gian vectơ: II, § 7, no. 8.
Hạng của một ánh xạ nửa tuyến tính của các không gian vectơ: II, § 7, no. 4.
Hạng của một tập con của một môđun trên một miền nguyên: II, § 7, no. 10.
Hạng của một tập con của một không gian vectơ: II, § 7, no. 2.
Tỉ số của một phép vị tự: II, § 1, no. 1.
Số nguyên hữu tỉ: I, § 2, no. 5.
Số hữu tỉ: I, § 9, no. 4.
Trường các số hữu tỉ: I, § 9, no. 4.
Hữu tỉ trên một trường con (dạng tuyến tính): II, § 8, no. 4.
Hữu tỉ trên một trường con (ánh xạ tuyến tính): II, § 8, no. 3.
Hữu tỉ trên một trường con (không gian con, vectơ): II, § 8, no. 2.
Phân tích rút gọn của một phần tử của một tổng dính: I, § 7, no. 3.
Môđun phản xạ: II, § 2, no. 7.
Chính quy, chính quy trái, chính quy phải, phần tử: I, § 2, no. 2.
Phần tử p-chính quy: I, § 6, Bài tập 28.
Hệ liên quan, tập con: II, § 1, no. 11, và § 9, no. 7.
Quan hệ, tương đương, tương thích với một luật hợp thành: I, § 1, no. 6.
Quan hệ, tương đương, tương thích với một tác động: I, § 3, no. 3.
Quan hệ, tương đương, sinh bởi một họ các cặp có thứ tự: I, § 1, no. 6.
Quan hệ, tương đương, trái, phải, tương thích với một luật hợp thành: I, § 3, no. 3.
Các quan hệ, tính giao hoán, trong một bảng phép nhân: III, § 1, no. 7.
Các quan hệ, Grassmann: III, § 11, no. 13.
Các quan hệ, môđun tuyến tính của: II, § 1, no. 11.
Các số nguyên nguyên tố cùng nhau: I, § 8, no. 11.
Phần tử liên hệ: I, § 7, no. 6 và III, § 2, no. 8.
Phần tử liên hệ, phổ quát: III, § 2, no. 8.
Iđêan của các phần tử liên hệ: III, § 3, no. 8.
Các phần tử liên hệ của một trình bày: I, § 7, no. 6 và III, § 2, no. 8.
Các phần tử liên hệ, đa thức: III, § 2, no. 9.
Thặng dư của một nửa nhóm: I, § 2, Bài tập 11.
Nhóm hữu hạn địa phương: I, § 5, Bài tập 5.
Đại số hạn chế của một nửa nhóm: III, § 2, no. 10.
Tổng hạn chế, nội tại: I, § 4, no. 9.
Tổng hạn chế của các nhóm: I, § 4, no. 9.
Tổng hạn chế của các nhóm đối với các nhóm con: I, § 4, no. 9.
Hạn chế vô hướng (đại số thu được bởi): III, § 1, no. 5.
(Phần tử) thu được từ việc thay các phần tử vào các bất định: I, § 7, no. 5.
Phép rút lại của một mở rộng: I, § 6, no. 1.

Vế phải của một phương trình tuyến tính, các vế phải của một hệ tuyến tính: II, § 2, no. 8.
Vành: I, § 8, no. 1.
Vành Boolean: I, § 9, Bài tập 8.
Vành giao hoán: I, § 8, no. 1.
Vành (phân bậc, phân bậc với các bậc dương, phân bậc kép): II, § 11, no. 2.
Vành thương phân bậc: II, § 11, no. 3.
Vành thu được bởi phép nối một phần tử đơn vị: II, Phụ lục, no. 1.
Vành các tự đồng cấu của một nhóm giao hoán: I, § 8, no. 4.
Vành các phân thức với mẫu thuộc S: I, § 8, no. 12.
Vành các số nguyên modulo n: I, § 8, no. 11.
Vành các đa thức không giao hoán đối với một tự đồng cấu và một đạo hàm: III, § 10, Bài tập 3.
Vành đối: I, § 8, no. 3.
Vành tích: I, § 8, no. 10.
Vành thương: I, § 8, no. 7.
Vành toàn bộ các phân thức: I, § 8, no. 2.
Vành không: I, § 8, no. 3.
Dòng của một ma trận: II, § 10, no. 1.
Luật, dấu: I, § 8, no. 1.

Vô hướng: II, § 1, no. 1.
Phương trình tuyến tính vô hướng: II, § 2, no. 8.
Ma trận vô hướng: II, § 10, no. 7.
Định lý Schreier về các chuỗi hợp thành: I, § 4, no. 7.
Tiết diện của một mở rộng: I, § 6, no. 2.
Tích nửa trực tiếp của các nhóm: I, § 6, no. 1.
Nửa nhóm, trái, phải: I, § 2, Bài tập 11.
Nửa đồng cấu, đại số, đại số ρ-đồng cấu: III, § 1, số 5.
Ánh xạ nửa tuyến tính: II, § 1, no. 13.
Dãy, khớp: II, § 1, no. 4.
Dãy, có thứ tự: I, § 1, no. 2.
Dãy khớp tách: II, § 1, no. 9.
Các dãy có thứ tự tương tự: I, § 1, no. 2.
Chuỗi, đại số lũy thừa hình thức: III, § 2, no. 11.
Chuỗi, hợp thành: I, § 4, no. 6.
Chuỗi, dẫn xuất: I, § 6, no. 4.
Chuỗi, phân tích tương đương: I, § 4, no. 7.
Chuỗi, hợp thành mịn hơn: I, § 4, no. 7.
Chuỗi, lũy thừa hình thức: III, § 2, no. 11.
Chuỗi, Jordan-Hölder: I, § 4, no. 7.
Chuỗi, trung tâm dưới: I, § 6, no. 3.
Chuỗi, chuẩn: I, § 4, Bài tập 17.

Chuỗi, chính: I, § 4, Bài tập 17.
G-tập hợp, thuần nhất (G là một nhóm các toán tử): I, § 5, no. 5.
G-tập hợp, thuần nhất chính, tập hợp thuần nhất chính dưới G: I, § 5, no. 6.
Tập hợp sinh của một nhóm: I, § 4, no. 3.
Tập hợp sinh của một magma: I, § 1, no. 4.
M-tập hợp (M là một đơn vị tử của các toán tử): I, § 5, no. 1.
M^0-tập hợp đối với một M-tập hợp: I, § 5, no. 1.
Tập hợp các bậc của một nhóm phân bậc: II, § 11, no. 1.
Tập hợp các nhóm con thỏa mãn điều kiện cực đại, điều kiện cực tiểu: I, § 4, Bài tập 15.
Các tập hợp trực giao: II, § 2, no. 4.
Các G-tập hợp tương đương yếu: I, § 5, Bài tập 26.
Dịch chuyển, phép dịch chuyển: II, § 11, no. 2.
Dấu của một phép hoán vị: I, § 5, no. 7.
Dấu của một số hữu tỉ: I, § 9, no. 4.
Các tự đồng cấu tương tự: III, § 8, Bài tập 26.
Các ma trận tương tự: II, § 10, no. 9.
Các dãy có thứ tự tương tự: I, § 1, no. 2.
Nhóm đơn: I, § 4, no. 4.
Phép toán bắc cầu đơn: I, § 5, no. 6.
Trường đối: I, § 9, no. 1.
Đại số hai phân bậc đối: III, § 11, no. 4.
Tenxơ đối xứng xiên: III, § 7, no. 4.
Tenxơ phản đối xứng: III, § 7, no. 4.
Tích tenxơ đối của các đại số phân bậc: III, § 4, nos. 7 and 8.
Nghiệm của một phương trình tuyến tính, của một hệ tuyến tính: II, § 2, no. 8.
Nghiệm tầm thường, nghiệm không của một phương trình tuyến tính thuần nhất: II, § 2, no. 8.
Nhóm giải được, nhóm giải được lớp n: I, § 6, no. 4.
Không gian affine, gắn với một không gian vectơ: II, § 9, no. 1.
Không gian xạ ảnh chính tắc, liên kết với một không gian vectơ: II, § 9, no. 8.
Không gian xạ ảnh: II, § 9, nos. 5 and 11.
Không gian xạ ảnh, dẫn xuất từ một không gian vectơ: II, § 9, no. 5.
Không gian vectơ thương, không gian thương: II, § 1, no. 3.
Không gian phải, trái, vectơ, trên một trường: II, § 1, no. 1.
Không gian vectơ, liên kết với một môđun trên một miền nguyên: II, § 7, no. 10.
Không gian vectơ, thu được bằng cách chọn một gốc trong một không gian affine: II, § 9, no. 1.
Không gian vectơ, của các phép tịnh tiến của một không gian affine: II, § 9, no. 1.
Dãy khớp tách: II, § 1, no. 10.
Ổn định (toán tử, tập hợp các toán tử) một tập con: I, § 5, no. 2.
Ổn định ngặt (toán tử, tập hợp các toán tử) một tập con: I, § 5, no. 2.
Nhóm con ổn định của một nhóm với các toán tử: I, § 4, no. 3.

Tập con ổn định: I, § 1, no. 4.
Âm ngặt, dương ngặt, số nguyên hữu tỉ: I, § 2, no. 5.
Âm ngặt, dương ngặt, số hữu tỉ: I, § 9, no. 4.
Nhóm ổn định ngặt: I, § 5, no. 2.
Ổn định ngặt một tập con: I, § 5, no. 2.
Toán tử chuyển ngặt: I, § 5, no. 2.
Tập con kết hợp mạnh: III, Phụ lục, no. 1.
Các cấu trúc môđun (đa môđun), tương thích: II, § 1, no. 14.
Cấu trúc, không gian xạ ảnh: II, § 9, no. 11.
Cấu trúc K', cảm sinh: II, § 8, no. 2.
Cấu trúc K' trên một không gian K-vectơ: II, § 8, no. 1.
Cấu trúc K', tích: II, § 8, no. 3.
Đại số con: III, § 1, no. 2.
Đại số con sinh bởi một tập con: III, § 1, no. 2.
Đại số con, phân bậc: III, § 3, no. 2.
Trường con: I, § 9, no. 1.
Trường con sinh bởi một tập con: I, § 9, no. 1.
Nhóm con, đặc trưng: I, § 5, no. 3.
Nhóm con, ổn định bất biến, nhóm con bất biến: I, § 4, no. 4.
Nhóm con, ổn định chuẩn tắc, nhóm con chuẩn tắc: I, § 4, no. 4.
Nhóm con, ổn định, sinh bởi một tập con: I, § 4, no. 3.
Nhóm con, nhóm con ổn định: I, § 4, no. 3.
Nhóm con Sylow, nhóm con Sylow $p$-nhóm: I, § 6, no. 6.
Magma con: I, § 1, no. 4.
Magma con sinh bởi một tập con: I, § 1, no. 4.
Magma con, có đơn vị: I, § 2, no. 1.
Magma con, có đơn vị, sinh bởi một tập con: I, § 2, no. 1.
Ma trận con: II, § 10, no. 1.
Môđun con: II, § 1, no. 3.
Môđun con, thành phần, của một tổng trực tiếp các môđun: II, § 1, no. 6.
Môđun con sinh bởi một họ: II, § 1, no. 7.
Môđun con, phân bậc: II, § 11, no. 3.
Môđun con, bất khả quy: II, § 2, Bài tập 16.
Môđun con, trực giao (hoặc hoàn toàn trực giao) với một tập con của E (resp. E*) II, § 2, no. 4.
Môđun con, xoắn, của một môđun trên một miền nguyên: II, § 7, no. 10.
Môđun con, không: II, § 1, no. 3.
Các môđun con, bổ sung: II, § 1, no. 9.
Môđun đa con: II, § 1, nos. 14.
Vành con: I, § 8, no. 5.
Vành con sinh bởi một tập con: I, § 8, no. 5.
Vành con, phân bậc: II, § 11, no. 3.
Tập con affine: II, § 9, no. 3.

Tập con giao hoán với một tập con: I, § 5, no. 3.
Tập con, tự do, tập con liên quan: II, § 1, no. 11.
Tập con, thuần nhất, bậc $p$ đối với một số bất định trong một chuỗi lũy thừa hình thức: III, § 2, no. 11.
Tập con chuẩn hóa một tập con: I, § 5, no. 3.
Tập con, ổn định: I, § 1, no. 4 và § 3, no. 2.
Tập con, ổn định, được sinh bởi một tập con: I, § 1, no. 4 và § 3, no. 2.
Tập con, kết hợp mạnh: III, Phụ lục, no. 1.
Tập con, đối xứng: I, § 4, no. 1.
Các tập con, liên hợp: I, § 5, no. 4.
Các không gian con liên kết với một phần tử thuần nhất của đại số ngoài: III, § 7, no. 2.
Không gian con liên kết với một phần tử thuần nhất của đại số đối xứng: III, § 6, no. 2.
Không gian con liên kết với một phần tử thuần nhất của đại số tenxơ: III, § 5, no. 2.
Các không gian con liên kết với một phần tử của một tích tenxơ của các không gian vectơ: II, § 7, no. 8.
Không gian con hữu tỉ trên một trường con: II, § 8, no. 2.
Không gian con, vectơ, không gian con: II, § 1, no. 3.
Tổng, ghép, của các môđun: II, § 1, Bài tập 5.
Tổng, ghép, của các monoid: II, § 7, no. 3.
Tổng, trực tiếp: I, § 4, no. 9.
Tổng, trực tiếp, của một họ các môđun con: II, § 1, no. 8.
Tổng trực tiếp ngoài, của một họ các môđun con: II, § 1, no. 6.
Tổng hạn chế trong, của các nhóm con: I, § 4, no. 9.
Tổng, đơn thức: I, § 7, no. 3.
Tổng của một họ các phần tử có giá hữu hạn: I, § 2, no. 1.
Tổng của một họ các iđêan trái, của các iđêan phải: I, § 8, no. 6.
Tổng của một họ các môđun con: II, § 1, no. 7.
Tổng của một dãy có thứ tự: I, § 1, no. 2.
Tổng của hai phần tử: I, § 1, no. 1.
Tổng của hai ma trận: II, § 10, no. 2.
Tổng hạn chế của các nhóm đối với các nhóm con, tổng hạn chế của các nhóm: I, § 4, no. 9.
Nhóm siêu giải được: I, § 6, Bài tập 26.
Các môđun con bổ sung: II, § 1, no. 9.
Giá của một chu trình: I, § 5, no. 7.
Giá của một họ: I, § 2, no. 1.
Bỏ các cột, các hàng, trong một ma trận: II, § 10, no. 1.
Nhóm con Sylow: I, § 6, no. 6.
Ký hiệu Kronecker: II, § 1, no. 11.
Đại số đối xứng của một môđun: III, § 6, no. 1.

Nhóm đối xứng: I, § 4, no. 1.
Ánh xạ đa tuyến tính đối xứng: III, § 6, no. 3.
Lũy thừa đối xứng của một ánh xạ tuyến tính: III, § 6, no. 3.
Lũy thừa đối xứng của một môđun: III, § 6, no. 3.
Tích đối xứng của hai ánh xạ đa tuyến tính: III, § 11, no. 2.
Tập con đối xứng trong một nhóm: I, § 4, no. 1.
Tenxơ đối xứng: III, § 6, no. 3.
Đối xứng hóa của một tenxơ: III, § 6, no. 3.
Hệ trực tiếp của các đại số phân bậc: III, § 3, no. 3.
Hệ trực tiếp của các magma: I, § 10, no. 3.
Hệ trực tiếp của các môđun: II, § 6, no. 2.
Hệ trực tiếp của các vành (nhóm, trường): I, § 10, no. 3.
Hệ tự do, hệ liên quan: II, § 1, no. 11.
Hệ sinh của một nhóm: I, § 4, no. 3.
Hệ sinh của một magma: I, § 1, no. 4.
Hệ sinh của một môđun: II, § 1, no. 7.
Hệ sinh của một không gian xạ ảnh: II, § 9, no. 8.
Hệ sinh của một magma có đơn vị: I, § 2, no. 1.
Hệ sinh của một đại số: III, § 1, no. 2.
Hệ nghịch đảo của các đại số: III, § 1, no. 6.
Hệ nghịch đảo của các magma: II, § 10, no. 1.
Hệ nghịch đảo của các môđun: II, § 6, no. 1.
Hệ nghịch đảo của các vành (nhóm, trường): I, § 10, no. 1.
Hệ phương trình của một không gian con vectơ: II, § 7, no. 5.
Hệ nhân tử: III, § 2, Bài tập 11.
Hệ tọa độ thuần nhất của một điểm: II, § 9, no. 6.
Hệ phương trình tuyến tính, hệ tuyến tính, hệ tuyến tính thuần nhất: II, § 2, no. 8.
Hệ tầm thường của các nhân tử giao hoán: III, § 4, no. 7.

Bảng, đường chéo, tam giác dưới, tam giác trên, của các ma trận: II, § 10, no. 7.
Bảng nhân của một đại số: III, § 1, no. 7.
Bảng bình phương của các ma trận: II, § 10, no. 5.
Đại số tenxơ của một môđun: III, § 5, no. 1.
Tenxơ đối biến, tenxơ hiệp biến, tenxơ hỗn hợp: III, § 5, no. 6.
Tenxơ kiểu (I, J): III, § 5, no. 6.
Tenxơ phản đối xứng: III, § 7, no. 4.
Tenxơ đối xứng: III, § 6, no. 3.
Lũy thừa tenxơ của một ánh xạ tuyến tính: III, § 5, no. 2.
Lũy thừa tenxơ của một môđun: III, § 5, no. 1.
Số hạng hằng của một chuỗi lũy thừa hình thức: III, § 2, no. 11.
Số hạng hằng của một đa thức: III, § 2, no. 9.
Số hạng trong $X^α$ của một đa thức: III, § 2, no. 9.

Số hạng của một chuỗi lũy thừa hình thức: III, § 2, No. 11.
Số hạng của một đa thức: III, § 2, No. 9.
Số hạng của một tổng: I, § 1, No. 2.
Số hạng bậc $p$ đối với một số bất định trong một chuỗi lũy thừa hình thức: III, § 2, No. 11.
Số hạng có bậc toàn phần $p$ trong một chuỗi lũy thừa hình thức: III, § 2, No. 11.
Định lý về tính kết hợp: I, § 1, No. 3.
Định lý Cayley-Hamilton: III, § 8, No. 11.
Định lý về tính giao hoán: I, § 1, No. 5.
Định lý Desargues: II, § 9, Bài tập 15.
Định lý Erdős-Kaplansky: II, § 7, Bài tập 3.
Định lý cơ bản của hình học xạ ảnh: II, § 9, Bài tập 16.
Định lý Hall: I, § 6, Bài tập 7.
Định lý Jordan-Hölder: I, § 4, No. 7.
Định lý Kaplansky: II, § 2, Bài tập 2.
Định lý Krull: I, § 8, No. 6.
Định lý Nielsen-Schreier: I, § 7, Bài tập 20.
Định lý về tứ giác đầy đủ: II, § 9, Bài tập 13.
Định lý Pappus: II, § 9, Bài tập 14.
Định lý Schreier: I, § 4, No. 7.
Phần tử xoắn, môđun xoắn, môđun con xoắn: II, § 7, No. 10.
Môđun không xoắn: II, § 7, No. 10.
Đại số toàn phần của một nửa nhóm: III, § 2, No. 10.
Phân bậc toàn phần: II, § 11, No. 1.
(Môđun con) trực giao hoàn toàn với một tập con: II, § 2, No. 4.
Vết Cayley: III, § 2, No. 4.
Vết trong một đại số bậc hai: III, § 2, No. 3.
Vết của một ma trận: II, § 10, No. 11.
Vết của một phần tử trong một đại số trên K: III, § 9, No. 3.
Vết của một tự đồng cấu: II, § 4, No. 3.
Vết của một vô hướng đối với một môđun: III, § 9, No. 1.
Phép toán bắc cầu: I, § 5, No. 5.
Các công thức về tính bắc cầu: III, § 9, No. 4.
Phép tịnh tiến trong một không gian affine, không gian các phép tịnh tiến: II, § 9, No. 1.
Phép tịnh tiến trái, phải: I, § 2, No. 2.
Phép tịnh tiến trái, phải (của một nửa nhóm tác động lên chính nó): I, § 5, No. 1.
Toán tử vận chuyển, toán tử vận chuyển ngặt: I, § 5, No. 2.
Chuyển vị của một ánh xạ tuyến tính, của một ánh xạ nửa tuyến tính: II, § 2, No. 5.
Chuyển vị của một ma trận: II, § 10, No. 1.
Phép chuyển vị: I, § 5, No. 7.
Phép xuyên vị: II, § 10, Bài tập 11.
Ma trận tam giác, tam giác dưới, tam giác trên: II, § 10, No. 7.
Mở rộng tầm thường: I, § 6, No. 1.

Phân bậc tầm thường: II, § 11, No. 1.
Đồng cấu tầm thường: I, § 2, No. 1.
Phép toán tầm thường: I, § 5, No. 2.
Nghiệm tầm thường của một phương trình tuyến tính thuần nhất: II, § 2, No. 8.
Hệ tầm thường của các nhân tử giao hoán: III, § 4, No. 7.
Iđêan hai phía: I, § 8, No. 6 và III, § 1, No. 2.
Nhóm kiểu mũ: I, § 7, Bài tập 39.
Phân bậc kiểu Δ: II, § 11, No. 1.

Tự đồng cấu đơn môđula: III, § 8, No. 1.
Nhóm đơn môđula: III, § 8, No. 9.
Ma trận đơn môđula: III, § 8, No. 3.
Phần tử p-unipotent: I, § 6, Bài tập 28.
Phần tử đơn vị của một đại số: III, § 1, No. 1.
Phần tử đơn vị trái, phải trong một groupoid: I, § 4, Bài tập 23.
Phần tử khả nghịch, phần tử đơn vị của một magma: I, § 2, No. 1.
Đại số có đơn vị: III, § 1, No. 1.
Đồng cấu đại số có đơn vị, cấu xạ: III, § 1, No. 1.
Đồng cấu có đơn vị: I, § 2, No. 1.
Magma có đơn vị: I, § 2, No. 1.
Các phần tử khả nghịch của ma trận: II, § 10, No. 3.
Đại số phổ quát xác định bởi một hệ sinh liên hệ với nhau bởi một họ các hệ thức: III, § 2, No. 8.
Đại số phổ quát thỏa mãn các đồng nhất thức: III, § 2, No. 8.
Hệ thức phổ quát: III, § 2, No. 8.
Các ẩn của một hệ tuyến tính: II, § 2, No. 8.

Giá trị tuyệt đối của một số hữu tỉ: I, § 9, No. 4.
Giá trị của một phần tử của một đại số tự do: III, § 2, No. 8.
Định thức Vandermonde: III, § 8, No. 6.
Đa tạp tuyến tính affine, đa tạp tuyến tính affine sinh bởi một họ: II, § 9, No. 3.
Đa tạp tuyến tính: II, § 9, Nos. 3, 7 và 11.
Đa tạp tuyến tính xạ ảnh, đa tạp tuyến tính xạ ảnh sinh bởi một họ: II, § 9, Nos. 7 và 11.
Các đa tạp tuyến tính song song: II, § 9, No. 3.
Vectơ: II, § 1, No. 1.
Vectơ chỉ phương của một đường thẳng affine: II, § 9, No. 3.
Vectơ tự do của một không gian affine: II, § 9, No. 1.
p-vectơ: III, § 7, No. 1.
p-vectơ thuần: III, § 11, No. 13.
Vectơ hữu tỉ trên một trường con: II, § 8, No. 2.
Không gian vectơ: II, § 1, No. 1.

Từ: I, § 7, No. 2.

Trọng số của một phần tử thuần nhất: II, § 11, No. 1.
(Không có điểm bất động) (tự đẳng cấu): I, § 6, Bài tập 23.

Bổ đề Zassenhaus: I, § 4, No. 7.
Không: I, § 2, No. 1.
Ma trận không: II, § 10, No. 22.
Vành không: I, § 8, No. 3.
Nghiệm không của một phương trình tuyến tính: II, § 2, No. 8.
Môđun con không: II, § 1, No. 3.

N. Bourbaki, Các phần tử của Toán học, Đại số, Các chương 1-3

Đây là bản in lại bìa mềm của bản dịch tiếng Anh năm 1974 (được Springer cung cấp từ năm 1989) của 3 chương đầu trong tác phẩm "Algebrec" của Bourbaki. Sách trình bày đầy đủ các cơ sở của đại số tổng quát, đại số tuyến tính và đại số đa tuyến tính. Chương thứ nhất giới thiệu các đối tượng cơ bản: nhóm, tác động, vành, trường. Chương thứ hai nghiên cứu các tính chất của môđun và các ánh xạ tuyến tính, đặc biệt đối với tích tenxơ và các cấu trúc đối ngẫu. Chương thứ ba nghiên cứu các đại số, đặc biệt là các đại số tenxơ. Các định thức, chuẩn, vết và các phép đạo hàm cũng được nghiên cứu.
