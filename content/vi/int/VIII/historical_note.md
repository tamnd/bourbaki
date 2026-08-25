---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: int-vii-ix
pdf_pages: 0175-0182
extraction: ocr
statements: 0
exercises: 0
content_sha256: bf2fca2bd13f8873d97a552a872139447da56c213538d7ab5e435d98f04db9a5
translated_from: content/en/int/VIII/historical_note.md
source_content_sha256: 8310a10c50a658cc062070acbfc343e395a3fba746d5379e0f041cac27733c15
translation_model: gpt-5.4
translation_run: translate-vi-032ee449
glossary_version: 34
glossary_terms_sha256: b9808dd61cb3747c1eedcb2c7c243fd1e3191eef4de88d43f36eb9fe12eb93f5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Chương VII và VIII)

(Xin chú ý. — Các chữ số La Mã quy chiếu đến thư mục ở cuối ghi chú này.)

Các khái niệm độ dài, diện tích và thể tích, ở người Hy Lạp, về cơ bản dựa trên tính bất biến của chúng đối với các phép dời hình: « Những vật trùng nhau (εφαρμόξοντα) thì bằng nhau » (Eucl. El., Quyển I, ‘Khái niệm chung’ 4); và chính bằng một cách sử dụng khéo léo nguyên lý này mà thu được tất cả các công thức cho diện tích hoặc thể tích của các ‘hình’ cổ điển (đa giác, thiết diện cônic, đa diện, mặt cầu, v.v.), đôi khi bằng các phương pháp phân tích hữu hạn, đôi khi bằng phương pháp ‘vét cạn’ (*). Theo ngôn ngữ hiện đại, có thể nói rằng điều các nhà hình học Hy Lạp đã làm là chứng minh sự tồn tại của các ‘hàm tập hợp’, cộng tính và bất biến dưới các phép dời hình, nhưng chỉ được định nghĩa cho các tập hợp thuộc một kiểu rất đặc biệt. Phép tính tích phân có thể được xem là đáp ứng nhu cầu mở rộng miền xác định của các hàm tập hợp này, và từ Cavalieri đến H. Lebesgue, chính mối bận tâm đó đã ở hàng đầu trong nghiên cứu của các nhà giải tích; còn đối với tính chất bất biến dưới các phép dời hình, nó bị đẩy xuống địa vị thứ yếu, vì đã trở thành một hệ quả tầm thường của công thức tổng quát về phép đổi biến trong các tích phân kép hoặc ba và của sự kiện rằng một phép biến đổi trực giao có định thức bằng $\pm 1$. Ngay cả trong các hình học phi Euclid (mặc dù ở đó nhóm các phép dời hình là khác), quan điểm vẫn như thế: một cách tổng quát, Riemann đã định nghĩa vi phân-

(*) Có thể chỉ ra rằng nếu hai đa giác phẳng P, P' có cùng diện tích, thì tồn tại hai đa giác R ⊃ P, R' ⊃ P', mỗi đa giác trong số đó có thể được phân tích thành một số hữu hạn các đa giác R_i (tương ứng R'_i) (1 ≤ i ≤ m) không có điểm trong chung, sao cho R_i và R'_i có thể suy ra từ nhau nhờ một phép dời hình (phụ thuộc vào i), và sao cho R (tương ứng R') là hợp của một họ hữu hạn các đa giác S_j (tương ứng S'_j) (0 ≤ j ≤ n), không có điểm trong chung, với S_0 = P, S'_0 = P', và S'_j nhận được từ S_j bằng một phép dời hình với 1 ≤ j ≤ n. Tuy nhiên, M. DEHN đã chứng minh (Ueber den Rauminhalt, Math. Ann., 55 (1902), 465–478) rằng tính chất này không còn đúng đối với thể tích của các đa diện, và do đó các phương pháp vét cạn được sử dụng từ EUDOXUS trở đi là không thể tránh khỏi.

phần vô cùng bé của diện tích hoặc thể tích (hoặc các tương tự của chúng trong số chiều $\geqslant 3$) bắt đầu từ một $ds^2$ bằng các công thức Euclid cổ điển, và vì vậy tính bất biến của chúng dưới các phép biến đổi bảo toàn $ds^2$ hầu như là một điều hiển nhiên.

Chỉ vào khoảng năm 1890 mới xuất hiện những mở rộng khác, ít ngay lập tức hơn, của khái niệm độ đo bất biến dưới một nhóm, với sự phát triển của lý thuyết các *bất biến tích phân*, đặc biệt bởi H. Poincaré và E. Cartan; H. Poincaré chỉ xét các nhóm một tham số tác động trong một miền không gian, trong khi E. Cartan trước hết quan tâm đến các nhóm các phép dời hình, nhưng tác động trên những không gian khác với không gian nơi chúng được định nghĩa. Chẳng hạn, ông đã nhờ đó xác định, trong nhiều điều khác, độ đo bất biến (dưới nhóm các phép dời hình) trên không gian các đường thẳng của $\mathbf{R}^2$ hoặc của $\mathbf{R}^3$ (*); hơn nữa, ông nhận thấy rằng một cách tổng quát các bất biến tích phân đối với một nhóm Lie chẳng qua chỉ là những bất biến vi phân riêng biệt và vì thế có thể xác định tất cả chúng bằng các phương pháp của Lie. Tuy nhiên, dường như trước công trình cơ bản của A. Hurwitz năm 1897 (V), chưa ai nghĩ đến việc xét hoặc sử dụng một độ đo bất biến trên chính nhóm đó. Khi tìm cách lập các đa thức (trên $\mathbf{R}^n$) bất biến dưới nhóm trực giao, Hurwitz bắt đầu từ nhận xét rằng đối với một nhóm hữu hạn các phép biến đổi tuyến tính, bài toán được giải quyết ngay lập tức bằng cách lấy *trung bình* các ảnh $s \cdot \mathrm{P}$ của một đa thức P bất kỳ bởi mọi phần tử $s$ của nhóm, điều này gợi cho ông ý tưởng, đối với nhóm trực giao, thay thế trung bình ấy bằng một tích phân theo một độ đo bất biến; ông đã cho một cách tường minh biểu thức của độ đo này với sự trợ giúp của biểu diễn tham số bằng các góc Euler, nhưng ngay lập tức nhận thấy (độc lập với E. Cartan) rằng các phương pháp của Lie cho sự tồn tại của một độ đo bất biến đối với mọi nhóm Lie. Có lẽ do sự suy tàn của lý thuyết bất biến vào đầu thế kỷ 20, các ý tưởng của Hurwitz hầu như không có tiếng vang ngay lập tức nào, và chỉ được khai thác từ năm 1924 trở đi, với việc I. Schur và H. Weyl mở rộng cho các nhóm compact lý thuyết cổ điển của Frobenius về các biểu diễn tuyến tính của các nhóm hữu hạn. Người thứ nhất chỉ giới hạn ở trường hợp của nhóm trực giao, và chỉ ra cách phương pháp của Hurwitz cho phép mở rộng các hệ thức trực giao cổ điển của các đặc trưng, một ý tưởng mà H. Weyl đã kết hợp với các công trình của E. Cartan về các đại số Lie nửa đơn để thu được các biểu thức tường minh cho các đặc trưng của các biểu diễn bất khả quy của các nhóm Lie compact và định lý về tính phân tích đầy đủ (XI *a*)), rồi, bằng một sự mở rộng táo bạo của khái niệm ‘biểu diễn chính quy’, định lý Peter-Weyl nổi tiếng, một tương tự hoàn hảo của sự phân tích biểu diễn chính quy thành các

(*) Độ đo bất biến trên không gian các đường thẳng của mặt phẳng về cơ bản đã được xác định trước đó trong mối liên hệ với các bài toán về ‘xác suất hình học’, đặc biệt bởi CROFTON, mà các công trình có lẽ E. CARTAN chưa biết vào thời điểm ấy.

thành phần bất khả quy của nó trong lý thuyết các nhóm hữu hạn (XI, b)).

Một năm trước đó, O. Schreier đã sáng lập lý thuyết tổng quát về các nhóm tôpô, và từ đó trở đi hiển nhiên là các lập luận trong hồi ký của Peter–Weyl sẽ vẫn còn đúng nguyên vẹn đối với mọi nhóm tôpô mà trên đó có thể định nghĩa một 'độ đo bất biến'. Thực ra, vào thời đó các khái niệm tổng quát về tôpô và độ đo vẫn còn đang phát triển rất nhanh, và cả phạm trù các nhóm tôpô mà người ta có thể hy vọng định nghĩa một độ đo bất biến trên đó, lẫn các tập hợp mà 'độ đo' này phải được định nghĩa, đều chưa có vẻ được phân định rõ ràng. Điểm hiển nhiên duy nhất là người ta không thể hy vọng mở rộng sang trường hợp tổng quát các phương pháp vô cùng bé chứng minh sự tồn tại của một độ đo bất biến trên một nhóm Lie. Nhưng rồi, một dòng tư tưởng khác, nảy sinh từ các công trình về độ đo Lebesgue, đã dẫn chính xác đến những phương pháp tấn công trực tiếp hơn. Hausdorff đã chứng minh, vào năm 1914, rằng không tồn tại một hàm tập hợp cộng tính, không đồng nhất bằng không, được định nghĩa trên $\textbf{mọi}$ tập con của $\mathbf{R}^3$ và bất biến qua các phép dời hình, và điều tự nhiên là khảo sát xem kết quả này còn đúng cho $\mathbf{R}$ và $\mathbf{R}^2$ hay không: một bài toán đã được S. Banach giải vào năm 1923 theo một cách đáng ngạc nhiên, khi chỉ ra rằng ngược lại, một 'độ đo' như vậy quả thật có tồn tại (I); phương pháp của ông, hết sức khéo léo, đã dựa trên một phép dựng bằng quy nạp siêu hạn và trên việc xét các 'trung bình' $\frac{1}{n} \sum_{k=1}^n f(x + \alpha_k)$ của các phép tịnh tiến của một hàm bởi các phần tử của nhóm (*). Chính những ý tưởng tương tự đã cho phép A. Haar, vào năm 1933 (IV), thực hiện bước quyết định, khi chứng minh sự tồn tại của một độ đo bất biến đối với các nhóm địa phương compact có một cơ sở đếm được của các tập hợp mở: được dẫn dắt bởi phương pháp xấp xỉ một thể tích, trong phép tính tích phân cổ điển, bằng cách ghép cạnh nhau những khối lập phương bằng nhau nhỏ tùy ý, ông đã thu được, với sự trợ giúp của phương pháp đường chéo, độ đo bất biến như giới hạn của một dãy các 'độ đo xấp xỉ', một thủ tục về bản chất chính là thủ tục mà chúng tôi đã dùng trong Ch. VII, §1. Khám phá này đã có một ảnh hưởng rất lớn, đặc biệt vì nó ngay lập tức cho phép J. von Neumann giải, đối với các nhóm compact, "bài toán thứ 5" nổi tiếng của Hilbert về đặc trưng hóa các nhóm Lie bằng các tính chất tôpô thuần túy (loại trừ mọi cấu trúc vi phân được cho trước). Tuy nhiên, người ta cũng nhận thấy ngay lập tức rằng để sử dụng hữu hiệu độ đo bất biến, cần phải biết không chỉ sự tồn tại của nó, mà còn phải biết rằng nó là duy nhất sai khác bởi một nhân tử hằng; điểm này trước hết đã được J. von Neumann chứng minh cho các nhóm compact, bằng cách dùng một phương pháp định nghĩa độ đo Haar qua các 'trung bình' của các hàm liên tục, tương tự với các trung bình của Banach (VII a)); rồi J. von Neumann

(*) J. von NEUMANN đã chỉ ra, vào năm 1929, rằng nguyên nhân sâu xa của sự khác biệt trong cách ứng xử giữa $\mathbf{R}$ và $\mathbf{R}^2$ một mặt, và các $\mathbf{R}^n$ với $n \geq 3$ mặt khác, nằm ở tính giao hoán của nhóm các phép quay của không gian $\mathbf{R}^2$.

(VII b)) và A. Weil (X), bằng những phương pháp khác nhau, đã đồng thời thu được tính duy nhất trong trường hợp các nhóm địa phương compact, đồng thời A. Weil cũng chỉ ra cách phương pháp của Haar có thể được mở rộng cho các nhóm địa phương compact tổng quát. Cũng chính A. Weil (loc. cit.) là người đã thu được điều kiện để tồn tại một độ đo tương đối bất biến trên một không gian thuần nhất, và cuối cùng đã chỉ ra rằng sự tồn tại của một ‘độ đo’ (được trang bị những tính chất hợp lý) trên một nhóm tôpô Hausdorff kéo theo ipso facto rằng nhóm đó là địa phương tiền compact. Công trình này về cơ bản đã hoàn thành lý thuyết tổng quát về độ đo Haar; điểm bổ sung gần đây duy nhất cần nhắc tới là khái niệm độ đo giả bất biến, hầu như chưa được đồng nhất trước khoảng năm 1950, trong mối liên hệ với lý thuyết biểu diễn của các nhóm địa phương compact trong các không gian Hilbert.

Lịch sử của tích chập thì phức tạp hơn. Ngay từ đầu thế kỷ 19, người ta đã nhận thấy rằng nếu, chẳng hạn, F(x, t) là một nghiệm của một phương trình đạo hàm riêng theo x và t, tuyến tính và có các hệ số hằng, thì

$$
\int_{-\infty}^{+\infty} F(x - s, t) f(s) \, ds
$$

cũng là một nghiệm của cùng phương trình đó; từ trước năm 1820, Poisson, cùng với những người khác, đã dùng ý tưởng này để viết các nghiệm của phương trình nhiệt dưới dạng

(1)
$$
\int_{-\infty}^{+\infty} \exp \left( - \frac{(x - s)^2}{4t} \right) f(s) \, ds.
$$

Ít lâu sau, biểu thức

(2)
$$
\frac{1}{2\pi} \int_{-\pi}^{+\pi} \frac{\sin \frac{2n+1}{2}(x-t)}{\sin \frac{x-t}{2}} f(t) \, dt
$$

đối với tổng riêng của một chuỗi Fourier, và việc Dirichlet nghiên cứu giới hạn của tích phân này khi n tiến tới $+\infty$, đã cung cấp ví dụ đầu tiên về một phép ‘chính quy hóa’ $f \mapsto \rho_n * f$ trên xuyến $\mathbf{T}$ (thực ra bằng một dãy các ‘hạt nhân’ không dương, điều này làm cho việc nghiên cứu phức tạp hơn nhiều); dưới tên gọi ‘tích phân kỳ dị’, các biểu thức tích phân tương tự đã là một đối tượng được các nhà giải tích đặc biệt lựa chọn vào cuối thế kỷ 19 và đầu thế kỷ 20, từ P. du Bois-Reymond đến H. Lebesgue. Trên $\mathbf{R}$, Weierstrass đã sử dụng tích phân (1) trong chứng minh định lý của ông về xấp xỉ bằng đa thức, và trong liên hệ này đã nêu ra nguyên lý tổng quát của sự chính quy hóa bằng một dãy các ‘hạt nhân’ dương $\rho_n$ có dạng $x \mapsto c_n \rho(x/n)$. Trên $\mathbf{T}$, ví dụ nổi tiếng nhất về sự chính quy hóa bằng các hạt nhân dương được Fejér đưa ra ít lâu sau đó, và kể từ lúc ấy, đó là thủ tục chuẩn sẽ trở thành cơ sở của phần lớn các 'phương pháp tổng' cho các chuỗi hàm.

Tuy nhiên, do tính bất đối xứng của các vai trò do ‘hạt nhân’ và hàm được chính quy hóa đảm nhiệm, các công trình này hầu như không làm lộ rõ các tính chất đại số của tích chập. Trên hết, chúng ta mắc nợ Volterra vì đã nhấn mạnh điểm này. Ông đã nghiên cứu một cách tổng quát ‘hợp thành’ $F * G$ của hai hàm hai biến

$$
(F * G)(x, y) = \int_x^y F(x, t)G(t, y)\, dt,
$$

mà ông xem như một phép tổng quát hóa, ‘bằng sự chuyển từ hữu hạn sang vô hạn’, của tích của hai ma trận (IX). Rất sớm ông đã tách riêng trường hợp (được gọi là ‘chu trình đóng’ vì cách diễn giải của nó trong lý thuyết di truyền) trong đó F và G chỉ phụ thuộc vào $y - x$; khi đó điều tương tự cũng đúng với $H = F * G$, và nếu đặt $F(x, y) = f(y - x)$, $G(x, y) = g(y - x)$, thì

$$
H(x, y) = h(y - x),
$$

trong đó

$$
h(t) = \int_0^t f(t - s)g(s)\, ds,
$$

sao cho, với $t \geq 0$, $h$ trùng với tích chập của các hàm $f_1, g_1$ lần lượt bằng $f$ và $g$ khi $t \geq 0$, và bằng 0 khi $t < 0$.

Tuy nhiên, hình thức luận đại số do Volterra phát triển đã không làm lộ ra các liên hệ với cấu trúc nhóm của $\mathbf{R}$ và phép biến đổi Fourier. Đây không phải chỗ để thuật lại lịch sử của phép biến đổi sau; nhưng thích hợp để chú ý rằng từ Cauchy trở đi, các nhà giải tích nghiên cứu tích phân Fourier trước hết đã chuyên tâm tìm những điều kiện ngày càng rộng hơn cho tính đúng của nhiều công thức “nghịch đảo” khác nhau, và phần nào đã xem nhẹ các tính chất đại số của nó. Chắc chắn không thể nói như vậy về các công trình của chính Fourier (hoặc của Laplace về tích phân tương tự $\int_0^{+\infty} e^{-st} f(t)\, dt$); nhưng các phép biến đổi này về căn bản đã được đưa vào gắn với các bài toán tuyến tính, và vì thế cũng không có gì đáng ngạc nhiên lắm khi phải khá lâu người ta mới nghĩ đến việc xét tích của hai biến đổi Fourier (trừ trường hợp các tích của các chuỗi lượng giác hoặc của các chuỗi lũy thừa, nhưng liên hệ với tích chập của các độ đo rời rạc hiển nhiên không thể được nhận thấy trong thế kỷ 19). Sự nhắc đến đầu tiên về tích này và về tích chập trên $\mathbf{R}$ có lẽ gặp trong một hồi ký của Tchebychef (VIII), gắn với các vấn đề của lý thuyết xác suất. Thật vậy, trong lý thuyết này, tích chập $\mu * \nu$ của hai “luật xác suất” trên $\mathbf{R}$ (các độ đo dương có tổng khối lượng bằng 1 ) không là gì khác ngoài luật xác suất “hợp thành” của $\mu$ và $\nu$ (đối với phép cộng của các “biến ngẫu nhiên” tương ứng). Dĩ nhiên, đối với Tchebychef, vẫn chỉ là vấn đề tích chập của các luật xác suất có mật độ (đối với độ đo Lebesgue), do đó là tích chập của các hàm; hơn nữa, trong công trình của ông nó chỉ xuất hiện một cách giai thoại, và tình hình cũng như vậy trong một vài công trình hiếm hoi trong đó nó xuất hiện trước giai đoạn 1920–1930. Năm 1920, P. J. Daniell, trong một ghi chú (III) ít được chú ý vào thời đó, đã định nghĩa tích chập của hai độ đo tùy ý trên $\mathbf{R}$ và phép biến đổi Fourier của một độ đo như vậy, và đã nhận thấy tường minh rằng phép biến đổi Fourier chuyển tích chập thành một tích thông thường — một hình thức luận mà từ năm 1925 trở đi đã được các nhà xác suất sử dụng một cách mạnh mẽ, đặc biệt theo sau P. Lévy. Nhưng tầm quan trọng cơ bản của tích chập trong lý thuyết nhóm chỉ được H. Weyl hoàn toàn nhận ra vào năm 1927; ông nhận thấy rằng đối với một nhóm compact, tích chập của các hàm giữ vai trò của phép nhân trong đại số của một nhóm hữu hạn, cho phép ông sau đó định nghĩa “biểu diễn chính quy”; đồng thời, ông đã tìm thấy trong sự chính quy hóa cái tương đương với phần tử đơn vị của đại số của một nhóm hữu hạn. Còn lại là phải thực hiện sự tổng hợp của tất cả các quan điểm ấy; điều này đã được hoàn thành trong cuốn sách của A. Weil (X), mở đường cho các khái quát hóa về sau, những khái quát hóa sẽ cấu thành, một mặt, lý thuyết các đại số định chuẩn của I. Gelfand, và mặt khác, tích chập các phân phối.

Độ đo Haar và tích chập đã nhanh chóng trở thành những công cụ cốt yếu trong xu hướng đại số hóa vốn đánh dấu rất mạnh Giải tích hiện đại; chúng ta sẽ có dịp phát triển nhiều ứng dụng của chúng trong các Quyển sau. Ứng dụng duy nhất mà chúng ta đã xét trong các chương này liên quan đến “sự biến thiên” của các nhóm con đóng (và đặc biệt của các nhóm con rời rạc) của một nhóm compact địa phương. Lý thuyết này, khởi đi từ một kết quả của K. Mahler trong Hình học các số, đã được C. Chabauty khai mở vào năm 1950, và vừa mới được Macbeath và Swierczkowski (VII) phát triển và đào sâu đáng kể, những kết quả chính của họ chúng ta đã chép lại ở đây.

(I) S. Banach, Về bài toán độ đo, Fund. Math., 4 (1923), tr. 7–33.

(II) E. Cartan, Nguyên lý đối ngẫu và một số tích phân bội của không gian tiếp xúc và của không gian được kẻ, Bull. Soc. Math. France, 24 (1896), tr. 140–177 (= Œuvres complètes, v. II₁, tr. 265–302).

(III) P. J. Daniell, Các tích Stieltjes–Volterra, Congr. Intern. des Math., Strasbourg, 1920, tr. 130–136.

(IV) A. Haar, Khái niệm độ đo trong lý thuyết các nhóm liên tục, Ann. of Math., (2), 34 (1933), tr. 147–169 (= Gesammelte Arbeiten, tr. 600–622).

(V) A. Hurwitz, Về sự sinh các bất biến bằng phép lấy tích phân, Gött. Nachr., 1897, tr. 71–90 (= Math. Werke, v. II, tr. 546–564).

(VI) A. M. Macbeath, S. Swierczkowski, Giới hạn của các mạng trong một nhóm sinh compact, Canad. J. Math., 12 (1960), tr. 427–437.

(VII) J. von Neumann, a) Về độ đo Haar trong các nhóm tôpô, Comp. Math., 1 (1934), tr. 106–114 (= Collected Works, v. II, n° 22); b) Tính duy nhất của độ đo Haar, Mat. Sbornik, 1 (43) (1936), tr. 721–734 (= Collected Works, v. IV, n° 6).

(VIII) P. Tchebychef, Về hai định lý liên quan đến xác suất, Acta. Math., 14 (1890), tr. 305–315) (= Œuvres, v. II, tr. 481–491).

(IX) V. Volterra, Bài giảng về các hàm đường, Paris (Gauthier-Villars), 1913.

(X) A. Weil, Phép lấy tích phân trong các nhóm tôpô và các ứng dụng của nó, Actual. Scient. et Ind., n° 869, Paris, Hermann, 1940 (ấn bản thứ 2, ibid., n° 869-1145, Paris, Hermann, 1953).

(XI) H. Weyl, a) Lý thuyết biểu diễn các nhóm nửa đơn liên tục bằng các phép biến đổi tuyến tính, Math. Zeit., 23 (1925), tr. 271–309, 24 (1926), tr. 328–395 và 789–791 (= Selecta, Basel–Stuttgart (Birkhäuser), 1956, tr. 262–366); b) (với F. Peter) Tính đầy đủ của các biểu diễn nguyên thủy của một nhóm liên tục đóng, Math. Ann., 97 (1927), tr. 737–755 (= Selecta, tr. 387–404).
