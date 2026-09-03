---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: int-vii-ix
pdf_pages: 0302-0332
extraction: ocr
statements: 0
exercises: 0
content_sha256: 686e455fd1bc761ce7ef4ea6e90431fd7178a3bf36ff3025d0a35ef4e90e4f6c
translated_from: content/en/int/IX/historical_note.md
source_content_sha256: 99a55fef46c115102e6ca090941abc261582890dfee3c615e90b28ab94c2f2b9
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-780f05a6
glossary_version: 34
glossary_terms_sha256: 9451e8a26eeeaa22e19dcd47954b0a317887f14cf88a0f6289410a533f297285
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(N.B. — Các chữ số La Mã chỉ tới thư mục ở cuối ghi chú này.)

Mặc dù việc nghiên cứu các mối liên hệ giữa tôpô và lý thuyết độ đo đã có từ những buổi đầu của lý thuyết hiện đại về các hàm của biến thực, thì chỉ mới rất gần đây việc tích phân trong các không gian tôpô Hausdorff mới được triển khai đầy đủ theo một cách tổng quát. Trước khi trình bày lịch sử của công trình đi trước sự tổng hợp hiện tại, ta điểm qua vài giai đoạn trong sự tiến triển của các ý tưởng về các quan hệ giữa tôpô và độ đo.

Đối với Lebesgue, chỉ là vấn đề tích phân các hàm của một hay nhiều biến thực. Năm 1913, Radon đã định nghĩa các độ đo tổng quát trên $\mathbf{R}^n$ và các tích phân tương ứng; lý thuyết này được trình bày chi tiết trong sách (I) của Ch. de la Vallée Poussin và luôn dựa trên các tính chất tôpô của các không gian Euclid. Ít lâu sau, vào năm 1915, Fréchet đã định nghĩa trong (II, a)) các độ đo 'trừu tượng' trên một tập hợp được trang bị một σ-đại số, và các tích phân đối với các độ đo này; ông nhận thấy rằng theo cách này có thể thiết lập các kết quả chính của lý thuyết Lebesgue mà không cần dùng đến các phương pháp tôpô. Ông biện minh cho công trình của mình bằng những lời sau, trích từ lời mở đầu của (II, b), phần thứ nhất): « Que par exemple dans l’espace à une infinité de coordonnées où diverses applications de l’Analyse avaient conduit à diverses définitions non équivalentes d’une suite convergente, on remplace une de ces définitions par une autre, rien ne sera changé dans les propriétés des familles et fonctions additives d’ensembles dans ces espaces ».(*) Các khảo cứu của Fréchet được Carathéodory hoàn tất, người mà ta owe một định lý quan trọng về việc mở rộng một hàm tập hợp thành một độ đo. Phần mở đầu cuốn sách của Saks (III) trình bày cô đọng quan điểm này.

Sự phát hiện ra độ đo Haar trên các nhóm compact địa phương (xem Ghi chú lịch sử cho Chs. VII và VIII) và những ứng dụng phong phú mà nó ngay lập tức nhận được, rồi các công trình của Weil và Gelfand về Phân tích điều hòa, đã dẫn khoảng năm 1940 đến một sự biến đổi sâu sắc của quan điểm này: trong loại câu hỏi này, thuận tiện nhất là xem một độ đo như một dạng tuyến tính trên một không gian các hàm liên tục. Phương pháp này buộc người ta phải tự hạn chế vào các không gian compact hoặc compact địa phương, nhưng đó không phải là một bất tiện đối với hầu hết các ứng dụng: hơn nữa, việc J. Tate và A. Weil đưa Phân tích điều hòa vào trên các nhóm $p$-adic và các nhóm adèle đã cho phép một sự đổi mới ngoạn mục của Lý thuyết số giải tích.

Chính từ một hướng hoàn toàn khác mà nhu cầu mở rộng quan điểm này bằng cách xét các độ đo trên các không gian tôpô không compact địa phương nảy sinh: dần dần, Lý thuyết xác suất dẫn đến việc nghiên cứu những không gian như vậy và cung cấp nhiều ví dụ không tầm thường. Có lẽ nguyên nhân của ảnh hưởng chậm trễ của những phát triển này đối với lý thuyết độ đo nằm ở sự cô lập tương đối của Lý thuyết xác suất, vốn cho đến gần đây vẫn ở bên lề của các ngành toán học truyền thống.

Độ đo trên các không gian dãy

Một trong những ngành phát triển nhất của Lý thuyết xác suất cổ điển là các định lý giới hạn (luật số lớn, khuynh hướng tiến tới luật Gauss–Laplace, ...); điều này liên quan đến sự đào sâu khái niệm tính quy luật thống kê được biểu lộ bởi các hiện tượng liên quan đến những quần thể rất lớn. Việc phát biểu toán học đúng đắn của các bài toán này đòi hỏi đưa vào các độ đo trên các không gian dãy; những không gian này, vốn là sự tổng quát hóa hiển nhiên nhất của các không gian hữu hạn chiều, đã là đối tượng khảo cứu ưa thích của 'Giải tích tổng quát' do Fréchet, Lévy, Lusin, ... tiến hành vào khoảng năm 1920. Cũng không phải ngẫu nhiên mà Khintchine và Kolmogoroff, những người sáng tạo ra các phương pháp mới của Lý thuyết xác suất, đều là học trò của Lusin, và rằng Lévy rất nhanh chóng hướng sang các bài toán xác suất: chính chúng đã là thước đo của các phương pháp mới.

Sự xuất hiện ngầm đầu tiên của một độ đo trên một không gian dãy được thấy trong công trình mà E. Borel dành năm 1909 cho các xác suất đếm được (IV). Một ý tưởng rất độc đáo của Borel là áp dụng các kết quả xác suất mà ông vừa thu được vào việc chứng minh các tính chất mà khai triển thập phân của gần như mọi số thực giữa 0 và 1 có. Sự áp dụng này dựa trên nhận xét cơ bản sau: hãy xác định mọi số thực giữa 0 và 1 bởi dãy các chữ số (hay 'digits') trong khai triển của nó theo một cơ số $q$ ($q \geqslant 2$); nếu lần lượt rút ngẫu nhiên các chữ số khác nhau của một số $x$, độc lập với nhau và với xác suất bằng nhau $1/q$ cho $0, 1, \ldots, q - 1$, thì xác suất để $x$ nằm trong một khoảng của $[0, 1[$ bằng độ dài của khoảng ấy.

(*) "Chẳng hạn, trong không gian có vô số tọa độ, nơi các ứng dụng khác nhau của Giải tích đã dẫn đến các định nghĩa khác nhau và không tương đương về một dãy hội tụ, nếu người ta thay một trong các định nghĩa ấy bằng một định nghĩa khác, thì sẽ không có gì thay đổi trong các tính chất của các họ và các hàm cộng tính của các tập hợp trong các không gian ấy."

Năm 1923, Steinhaus (V) đã thiết lập nghiêm ngặt các kết quả này và mô tả mô hình toán học chính xác cho dãy vô hạn các phép rút ngẫu nhiên được Borel xét đến: để đơn giản, ta lấy $q = 2$ và ký hiệu I là tập hợp có hai phần tử $\{0, 1\}$; trang bị cho I độ đo $\mu$ được xác định bởi $\mu(0) = \mu(1) = \frac{1}{2}$; các phần tử của không gian tích $I^{\mathbf{N}}$ là các dãy $\varepsilon = (\varepsilon(n))_{n \in \mathbf{N}}$ gồm các số bằng 0 hoặc 1, và ánh xạ $\varphi : \varepsilon \mapsto \sum_{n \geq 0} \varepsilon(n) \cdot 2^{-n-1}$ là, sai khác trên một tập đếm được, một song ánh của $I^{\mathbf{N}}$ lên khoảng $[0, 1]$; hơn nữa, $\varphi^{-1}$ biến độ đo Lebesgue trên $[0, 1]$ thành độ đo P trên $I^{\mathbf{N}}$, là tích của các độ đo $\mu$ trên mỗi nhân. Thực ra, Steinhaus không có sẵn một phép dựng các độ đo tích; ông đã sử dụng sự tồn tại của ánh xạ gần song ánh $\varphi$ để xây dựng độ đo P trên $I^{\mathbf{N}}$ xuất phát từ độ đo Lebesgue trên $[0, 1]$, rồi đưa ra một đặc trưng hóa tiên đề của P. Đẳng cấu thu được theo cách đó đã làm cho có thể chuyển ngôn ngữ của xác suất sang ngôn ngữ của độ đo và áp dụng các định lý đã biết về tích phân Lebesgue.

Trong cùng công trình, Steinhaus đã xét chuỗi ngẫu nhiên $\sum_{n \geq 0} \sigma_n \cdot a_n$, trong đó các dấu $\sigma_n = \pm 1$ được chọn ngẫu nhiên độc lập với nhau và với xác suất bằng nhau $\frac{1}{2}$; trong khoảng từ năm 1928 đến năm 1935, ông đã nghiên cứu nhiều chuỗi ngẫu nhiên khác. Về phần mình, Paley, Wiener và Zygmund đã xét các chuỗi Fourier ngẫu nhiên$^{(1)}$ có dạng $\sum_{n = -\infty}^{\infty} a_n \exp(2\pi i(nt + \Phi_n))$; các 'biên độ' $a_n$ là cố định, còn các 'pha' $\Phi_n$ là các biến ngẫu nhiên độc lập phân bố đều trên $[0, 1]$. Mặc dù các khó khăn giải tích thay đổi rất lớn từ bài toán này sang bài toán khác, sự chuyển đổi dưới dạng lý thuyết độ đo là như nhau trong mọi trường hợp và biểu thị một mở rộng của trường hợp được Borel và Steinhaus xử lý; vấn đề là xây dựng một độ đo trên $\mathbf{R}^{\mathbf{N}}$ là tích của một họ các độ đo tất cả đều đồng nhất với cùng một độ đo dương $\mu$ trên $\mathbf{R}$ có khối lượng 1; chẳng hạn, các chuỗi Fourier ngẫu nhiên nói trên tương ứng với trường hợp $\mu$ là độ đo Lebesgue trên $[0, 1]$.

Để xây dựng các độ đo tích như vậy, có thể dùng hai phương pháp. Phương pháp thứ nhất là một phương pháp trực tiếp, được Daniell (VI, a)) trình bày chính xác lần đầu tiên vào năm 1918; nó được Jessen (VII) phát hiện lại vào năm 1934, người đã nghiên cứu chi tiết trường hợp $\mu$ là độ đo Lebesgue trên $[0, 1]$. Phương pháp thứ hai là tìm những thủ pháp tương tự như thủ pháp của Steinhaus để rút gọn về độ đo Lebesgue trên $[0, 1]$; cách tiến hành này có ưu điểm là thuận tiện

(1) Về một trình bày các chuỗi Fourier ngẫu nhiên, xem phần trình bày của J. P. KAHANE trong Séminaire Bourbaki (No. 200, năm thứ 12, 1959/60, Benjamin, New York).

chừng nào người ta chưa có một trình bày đầy đủ về lý thuyết độ đo tổng quát, vì nó cho phép sử dụng các định lý của Lebesgue mà không cần những chứng minh mới.(2)

Lý thuyết chuyển động Brown

Lý thuyết này chiếm một vị trí đặc biệt trong sự phát triển khoa học đương đại, do sự trao đổi thường xuyên và phong phú giữa các vấn đề vật lý và toán học ‘thuần túy’ mà nó làm chứng. Việc nghiên cứu chuyển động Brown, được nhà thực vật học Brown phát hiện vào năm 1829, đã được tiến hành tích cực trong thế kỷ 19 bởi nhiều nhà vật lý,(3) nhưng mô hình toán học thỏa đáng đầu tiên chỉ được Einstein xây dựng vào năm 1905. Trong trường hợp đơn giản của một hạt chuyển động dọc theo một đường thẳng, các giả thiết cơ bản của Einstein có thể được phát biểu như sau: nếu $x(t)$ là hoành độ của hạt tại thời điểm $t$, và nếu $t_0 < t_1 < \cdots < t_{n-1} < t_n$, các độ dịch chuyển liên tiếp $x(t_i) - x(t_{i-1})$ (với $1 \leq i \leq n$) là các biến ngẫu nhiên Gauss độc lập. Đây không phải là chỗ để trình bày chi tiết công trình thực nghiệm quan trọng của J. Perrin, công trình đã thúc đẩy lý thuyết của Einstein; đối với mục đích của chúng ta, chỉ cần giữ lại một nhận xét của Perrin, theo đó việc quan sát các quỹ đạo của chuyển động Brown đã gợi ý không thể cưỡng lại cho ông về các “hàm của các nhà toán học không có đạo hàm”. Nhận xét này sẽ là tia lửa ban đầu cho Wiener.

Một dòng tư tưởng hoàn toàn khác có nguồn gốc từ lý thuyết động học chất khí, được phát triển trong khoảng từ năm 1870 đến năm 1900 bởi Boltzmann và Gibbs. Xét một chất khí tạo bởi N phân tử có khối lượng $m$ ở nhiệt độ T (tuyệt đối), và ký hiệu $\mathbf{v}_1, \ldots, \mathbf{v}_N$ là các vận tốc của N phân tử của chất khí; động năng của hệ bằng

$$
\frac{m}{2} (\mathbf{v}_1^2 + \cdots + \mathbf{v}_N^2) = 3NkT,
$$

trong đó $k$ là hằng Boltzmann. Theo các ý tưởng của Gibbs, vô số va chạm giữa các phân tử không cho phép xác định chính xác các vận tốc của các phân tử, và thuận tiện là đưa vào một luật xác suất $P$ trên mặt cầu S của không gian chiều 3N được xác định bởi phương trình (1). Giả thiết ‘vi chính tắc’ bao gồm việc giả sử rằng

(2) Wiener cũng nhiều lần chú ý (xem chẳng hạn (XI), Ch. IX) để chỉ ra rằng độ đo của chuyển động Brown là đẳng cấu với độ đo Lebesgue trên $[0,1]$. Khả năng của những thủ pháp như vậy được giải thích bằng một định lý tổng quát của von Neumann đưa ra một đặc trưng hóa tiên đề của các độ đo đẳng cấu với độ đo Lebesgue trên $[0,1]$.

(3) Một trình bày rất sinh động về lịch sử này có thể tìm thấy trong cuốn sách gần đây của E. Nelson, Dynamical theories of Brownian motion, Mathematical Notes, Princeton, 1967.

rằng P là độ đo trên mặt cầu S có khối lượng 1 bất biến dưới phép quay. Hơn nữa, luật Maxwell về vận tốc phát biểu rằng luật xác suất của một thành phần của vận tốc của một phân tử là một độ đo Gauss với phương sai $2kT/m$ (§ 6, No. 5, *Nhận xét 3*). Borel dường như là người đầu tiên nhận thấy vào năm 1914 rằng luật Maxwell là một hệ quả của các giả thuyết của Gibbs và các tính chất của mặt cầu khi số lượng phân tử rất lớn. Ông xét một mặt cầu S trong một không gian Euclid có chiều lớn và độ đo P có khối lượng 1 trên S bất biến dưới phép quay; sử dụng các phương pháp xấp xỉ cổ điển dựa trên công thức Stirling, ông đã chỉ ra rằng phép chiếu của P trên một trục tọa độ là xấp xỉ Gauss. Các kết quả này đã được Gâteaux và Lévy làm sắc nét hơn một chút sau đó (IX, *a*). Cho một số nguyên $m \geqslant 1$ và một số $r > 0$, ký hiệu $S_{m,r}$ là tập hợp các dãy có dạng $(x_1, \ldots, x_m, 0, 0, \ldots)$ với $x_1^2 + \cdots + x_m^2 = r^2$; đồng thời, ký hiệu $\sigma_{m,r}$ là độ đo có khối lượng 1 trên $S_{m,r}$ bất biến dưới phép quay. Phát biểu bằng ngôn ngữ hiện đại, kết quả của Gâteaux và Lévy như sau: dãy các độ đo $\sigma_{m,1}$ hội tụ chặt đến một khối lượng đơn vị tại gốc tọa độ $(0, 0, \ldots)$, và dãy các độ đo $\sigma_{m, \sqrt{m}}$ hội tụ chặt đến một độ đo $\Gamma$ có dạng

$$
d\Gamma(x_1, x_2, \ldots) = \prod_{n=1}^\infty d\gamma(x_n)
$$

($\gamma$ là độ đo Gauss trên $\mathbf{R}$ với phương sai 1).

Độ đo $\Gamma$ nói trên đóng vai trò của một độ đo Gauss trong các chiều vô hạn. Quả thực, dường như Lévy đã hy vọng một cách mơ hồ định nghĩa một cách nội tại một độ đo Gauss trên mọi không gian Hilbert vô hạn chiều. Thực tế, như Lévy và Wiener đã chỉ ra, độ đo $\Gamma$ là bất biến theo một nghĩa nào đó$^{(4)}$ dưới các tự đẳng cấu của $l^2$; đáng tiếc là tập hợp $l^2$ của các dãy khả tổng bình phương $(x_1, x_2, \ldots, x_n, \ldots)$ có độ đo bằng không đối với $\Gamma$. Ngày nay người ta biết rằng phải bằng lòng với việc có một *tiền độ đo* Gauss trên một không gian Hilbert vô hạn chiều.$^{(5)}$

Ta mang ơn Wiener về tiến bộ cốt yếu: nếu không có một độ đo Gauss hợp lý trên một không gian Hilbert vô hạn chiều, ta có thể


(4) Chính xác hơn, ta có kết quả sau. Cho $U$ là một tự đẳng cấu của không gian Hilbert $l^2$, và $(u_{mn})$ là ma trận của $U$. Gọi E là không gian vectơ của tất cả các dãy thực $(x_n)_{n \geqslant 1}$ và F là không gian con của E tạo bởi các dãy $(x_n)_{n \geqslant 1}$ mà đối với chúng chuỗi $\sum_{n \geqslant 1} u_{mn} x_n$ hội tụ với mọi $m \geqslant 1$. Công thức $(\widetilde{U}x)_m = \sum_{n \geqslant 1} u_{mn} x_n$ định nghĩa một ánh xạ tuyến tính $\widetilde{U}$ từ F vào E, độ đo $\Gamma$ tập trung trên F, và $\widetilde{U}(\Gamma) = \Gamma$.

(5) Khái niệm này được đưa vào dưới tên gọi “phân bố chính tắc yếu” bởi I. E. Segal (*Trans. Amer. Math. Soc.* **88** (1958), 12–42). Ta phải ghi công tác giả này về một nghiên cứu chi tiết các độ đo pro-Gauss, và sự áp dụng của chúng vào một số bài toán trong lý thuyết trường lượng tử.
} xây dựng bằng phép toán nguyên thủy một độ đo $w$ trên một không gian các hàm liên tục bắt đầu từ một độ đo pro-Gauss (xem §6, No. 7, Định lý 1 về các chi tiết). Ta sẽ giải thích ngắn gọn phép dựng ban đầu của Wiener đối với $w$ (X); nó chịu ảnh hưởng trực tiếp bởi quan hệ $\Gamma = \lim_{m \to \infty} \sigma_{m, \sqrt{m}}$ của Gâteaux và Lévy. Với mỗi số nguyên $m \geqslant 1$, ký hiệu $H_m$ là tập hợp các hàm trên $T = ]0, 1]$ không đổi trên mỗi khoảng $\left[ \frac{k-1}{m}, \frac{k}{m} \right]$ (với $k = 1, 2, \ldots, m$), và ký hiệu $\pi_m$ là độ đo khối lượng 1, bất biến qua phép quay, trên mặt cầu Euclid bán kính 1 trong $\mathbf{R}^m$. Gọi $f_m$ là đẳng cấu của $H_m$ lên $\mathbf{R}^m$ gán cho mỗi hàm nhận giá trị $a_k$ trên khoảng $\left[ \frac{k-1}{m}, \frac{k}{m} \right]$ vectơ $(a_1, a_2 - a_1, \ldots, a_m - a_{m-1})$ (do đó có thuật ngữ ‘không gian vi phân’ được Wiener ưa dùng); ký hiệu $w_m$ là độ đo trên $H_m$ là ảnh của $\pi_m$ qua $f_m^{-1}$. Wiener định nghĩa độ đo mong muốn $w$ là giới hạn của các độ đo $w_m$. Chính xác hơn, hãy ký hiệu $H$ là tập hợp các hàm điều hòa từng đoạn trên $T$, với tôpô hội tụ đều (ta có $H_m \subset H$ với mọi số nguyên $m \geqslant 1$); với mọi hàm $F$ bị chặn liên tục đều trên $H$, giới hạn $A\{F\} = \lim_{m \to \infty} \int_{H_m} F(x) \, dw_m(x)$ tồn tại; tiếp theo, Wiener thu được một số chặn trên nhờ một phân tích tinh tế các dao động của trò chơi sấp-ngửa, và tiếp tục các lập luận về tính compact được Daniell nêu bật, ông chỉ ra rằng ta đang ở trong các điều kiện để áp dụng định lý mở rộng Daniell. Ta kết luận sự tồn tại của một độ đo $w$ mang bởi $\mathcal{C}(T)$ và sao cho $A\{F\} = \int_{\mathcal{C}(T)} F(x) \, dw(x)$. Khi đó Wiener có thể chỉ ra rằng độ đo $w$ tương ứng với các giả thuyết của Einstein,(6) và các ước lượng của ông cho phép ông đưa ra ý nghĩa chính xác cho nhận xét của Perrin về các hàm không có đạo hàm: tập hợp các hàm thỏa mãn điều kiện Lipschitz cấp $\frac{1}{2}$ là không đáng kể đối với $w$ (tuy nhiên, với mọi $a$ sao cho $0 < a < \frac{1}{2}$, hầu hết mọi hàm đều thỏa mãn điều kiện Lipschitz cấp $a$).

Ngày nay, đã biết nhiều phép dựng độ đo Wiener. Chẳng hạn, Paley và Wiener dùng các chuỗi Fourier ngẫu nhiên (XI, Ch. IX): với mỗi số thực

(6) Điều này có thể được biểu diễn bằng công thức
$$
\int_{\mathcal{C}(T)} f(x(t_1), \ldots, x(t_n)) \, dw(x) =
(2\pi)^{-n/2} \prod_{i=1}^n (t_i - t_{i-1})^{-1/2} \int \cdots \int f(x_1, \ldots, x_n) \exp \left( -\frac{1}{2} \sum_{i=1}^n \frac{(x_i - x_{i-1})^2}{t_i - t_{i-1}} \right) dx_1 \cdots dx_n,
$$
trong đó $f$ là một hàm liên tục bị chặn tùy ý trên $\mathbf{R}^n$ và trong đó $0 = t_0 < t_1 < \cdots < t_n \leqslant 1$ (ta quy ước $x_0 = 0$). Wiener, được Hardy rèn luyện về tính chặt chẽ giải tích, và hoàn toàn có lý do để nghi ngờ các nền tảng của Lý thuyết Xác suất vào thời đó, đã cẩn thận không sử dụng thuật ngữ hoặc kết quả xác suất. Do đó các hồi ký của ông đầy những công thức đáng sợ mà công thức trên đây là một ví dụ; hoàn cảnh này là một trong những yếu tố làm chậm sự phổ biến các ý tưởng của Wiener.

dãy $\mathbf{a} = (a_n)_{n \geq 1}$ và mỗi số nguyên $m \geq 0$, ta định nghĩa hàm $f_{m,\mathbf{a}}$ trên $]0,1]$ bởi

$$
f_{m,\mathbf{a}}(t) = a_1 t + 2 \sum_{k=2}^{2^{m+1}} \frac{1}{\pi k} a_{k-1} \sin \pi kt;
$$

ta có thể chỉ ra rằng với $\Gamma$-hầu hết mọi dãy $\mathbf{a}$, dãy các hàm $f_{m,\mathbf{a}}$ hội tụ đến một hàm liên tục $f_\mathbf{a}$, và rằng $w$ là ảnh của $\Gamma$ qua ánh xạ (được định nghĩa hầu khắp nơi) $\mathbf{a} \mapsto f_\mathbf{a}$. Về sau, Lévy đã đưa ra trong (IX, b), c)) một phép dựng rất gần với phép mà chúng ta đã trình bày trong §6, No. 7. Cuối cùng, Kac, Donsker và Erdös đã chỉ ra vào khoảng năm 1950 cách thay thế các độ đo cầu $\pi_m$ trên $\mathbf{R}^m$ trong phép dựng ban đầu của Wiener bằng các độ đo tổng quát hơn. Các kết quả của họ thiết lập một mối liên hệ vững chắc giữa độ đo Wiener và các định lý giới hạn của Lý thuyết Xác suất; chúng được Prokhorov (XIII) hoàn thiện và hệ thống hóa trong một công trình mà sau này chúng ta sẽ quay lại.

Đây không phải là nơi để phân tích vô số công trình xác suất quan trọng do phát hiện của Wiener mang lại; ngày nay, chuyển động Brown chỉ xuất hiện như một trong những ví dụ quan trọng nhất của quá trình Markoff. Ta chỉ sẽ nhắc đến sự áp dụng độ đo Wiener của Kac vào việc giải một số phương trình đạo hàm riêng parabol; đây là vấn đề thích nghi các ý tưởng của Feynmann trong lý thuyết trường lượng tử—lại là một ví dụ khác về ảnh hưởng qua lại giữa toán học và các vấn đề vật lý.

Giới hạn ngược của các độ đo

Đây là một lý thuyết đã phát triển chủ yếu để đáp ứng các nhu cầu của Lý thuyết xác suất. Các bài toán liên quan đến một dãy hữu hạn các biến ngẫu nhiên $X_1, \ldots, X_n$ về nguyên tắc được giải quyết khi biết luật $P_X$ của dãy: đó là một độ đo dương trên $\mathbf{R}^n$ có khối lượng 1 sao cho xác suất thu được đồng thời các bất đẳng thức $a_1 \leq X_1 \leq b_1, \ldots, a_n \leq X_n \leq b_n$ bằng $P_X(C)$, trong đó $C$ là hộp đóng $[a_1, b_1] \times \cdots \times [a_n, b_n]$ trong $\mathbf{R}^n$. Trong thực hành, độ đo $P_X$ hoặc có giá đỡ rời rạc hoặc thừa nhận một mật độ đối với độ đo Lebesgue. Khi làm việc với một dãy vô hạn $(X_n)_{n \geq 1}$ các biến ngẫu nhiên, người ta nói chung biết luật $P_n$ của dãy bộ phận $(X_1, \ldots, X_n)$ với mọi số nguyên $n \geq 1$; những dữ liệu này thỏa mãn một điều kiện tương hợp, diễn đạt rằng dãy $(P_n)_{n \geq 1}$ là một hệ ngược (hay ‘hệ xạ ảnh’) các độ đo. Cho đến khoảng năm 1920, các xác suất của những biến cố liên quan đến dãy vô hạn được định nghĩa theo cách thức nhiều hay ít là ngầm ẩn bằng những phép chuyển “tự nhiên” sang giới hạn từ các xác suất của trường hợp hữu hạn; do đó người ta giả thiết rằng xác suất để một trò chơi kết thúc là giới hạn, khi $n$ tiến tới vô cùng, của xác suất rằng nó kết thúc trong nhiều nhất $n$ bước. Dĩ nhiên, một lý thuyết như vậy không thật nhất quán, và không có gì loại trừ sự hiện diện của những 'nghịch lý', khi cùng một xác suất nhận hai ước lượng khác nhau tùy theo việc đánh giá bằng một hay bằng phương pháp kia trong hai phương pháp, mà mỗi phương pháp đều 'tự nhiên' như phương pháp còn lại.

Steinhaus (V) dường như là người đầu tiên cảm thấy cần phải xét (đối với trò tung đồng xu) không chỉ hệ ngược $(P_n)_{n \geq 1}$ mà cả giới hạn của nó nữa. Hơi sớm hơn một chút, năm 1919, Daniell (VI, $b$) đã chứng minh một cách tổng quát sự tồn tại của những giới hạn ngược như thế,$^{(7)}$ nhưng kết quả này dường như đã không được biết đến ở châu Âu. Nó được Kolmogoroff phát hiện lại vào năm 1933 trong công trình (XII), nơi tác giả trình bày quan niệm tiên đề của Lý thuyết xác suất. Các chứng minh của Daniell và Kolmogoroff dùng một lập luận về tính compact, về thực chất cũng giống như lập luận mà chúng tôi đã dùng trong ĐL. 2 của §4, No. 3 và dựa trên định lý của Dini.

Định lý Daniell–Kolmogoroff quả thật không để lại điều gì phải mong đợi trong trường hợp các dãy ngẫu nhiên $(X_n)_{n \geq 1}$, nhưng việc nghiên cứu các hàm ngẫu nhiên do Kolmogoroff, Feller và Doob tiến hành từ năm 1935 lại chứa đựng những khó khăn thuộc một bậc hoàn toàn khác. Xét chẳng hạn một khoảng $T$ của $\mathbf{R}$, biểu thị tập hợp các thời điểm quan sát của một 'quá trình ngẫu nhiên'; tập hợp các quỹ đạo có thể là không gian tích $\mathbf{R}^T$, được xem như giới hạn ngược của các tích từng phần $\mathbf{R}^H$, trong đó $H$ chạy qua tập hợp các tập con hữu hạn của $T$; nói chung người ta giả thiết đã cho một hệ ngược các độ đo $(\mu_H)$ (xem §4, No. 2). Định lý của Kolmogoroff quả thật cho một độ đo trên $\mathbf{R}^T$, nhưng nó chỉ được xác định trên một σ-đại số nhỏ hơn đáng kể so với σ-đại số Borel.$^{(8)}$ Một biến thể của phép dựng của Kolmogoroff, cho ra một độ đo trên một không gian tôpô, là do Kakutani (*Proc. Imp. Acad. Tokyo* 19 (1943), 184–188), và từ đó đã nhiều lần được phát hiện lại: người ta xem $\mu_H$ như một độ đo trên $\overline{\mathbf{R}}^H$ mang bởi $\mathbf{R}^H$;$^{(9)}$ không gian compact $E = \overline{\mathbf{R}}^T$ là giới hạn ngược của các tích hữu hạn $\overline{\mathbf{R}}^H$ và có thể định nghĩa một độ đo $\mu$ trên $E$ như là giới hạn ngược của các $\mu_H$ (xem Ch. III, §4, No. 5). Tuy nhiên, phương pháp này có một bất tiện nghiêm trọng; các phần tử của $\overline{\mathbf{R}}^T$ không có tính chất chính quy nào cho phép tiến hành việc nghiên cứu xác suất của quá trình - hay thậm chí chỉ đơn giản xóa bỏ các giá trị ký sinh $\pm \infty$ do phép compact hóa $\overline{\mathbf{R}}$ của $\mathbf{R}$ đưa vào. Điều này có thể khắc phục bằng cách cảm sinh độ đo $\mu$ của $\overline{\mathbf{R}}^T$ trên một không gian con cụ thể (chẳng hạn $\mathcal{C}(T)$ trong trường hợp chuyển động Brown); khó khăn cơ bản phát sinh từ thực tế rằng một không gian hàm, ngay cả một không gian thuộc kiểu thường gặp, không nhất thiết là $\mu$-đo được trong $\overline{\mathbf{R}}^T$, và ngay cả việc lựa chọn không gian hàm cũng có thể gây nghi vấn.$^{(10)}$


(7) Daniell đã xét trường hợp các độ đo trên một tích $\prod_{n \geq 1} I_n$ của các khoảng compact của $\mathbf{R}$, nhưng phương pháp của ông mở rộng ngay lập tức sang trường hợp một tích tùy ý của các không gian compact; về thực chất đó là phương pháp chúng tôi đã dùng trong Ch. III, §4, No. 5.

(8) Độ đo của Kolmogoroff chỉ được xác định cho các tập Borel trong $\mathbf{R}^T$ có dạng $A \times \mathbf{R}^{T-D}$, trong đó $D$ là một tập con đếm được của $T$, và $A$ là một tập con Borel của $\mathbf{R}^D$; vì lý do đó, định lý của Kolmogoroff cho một tích tùy ý $\mathbf{R}^T$ là một hệ quả ngay lập tức của trường hợp các tích đếm được.

(9) Có thể thay thế $\overline{\mathbf{R}}$ bằng bất kỳ không gian compact nào chứa $\mathbf{R}$ như một không gian con trù mật.

Một bước quyết định đã được Prokhorov thực hiện vào năm 1956 trong một công trình (XIII) đã có ảnh hưởng mang tính quyết định đối với lý thuyết các quá trình ngẫu nhiên. Bằng cách đưa vào một dạng tiên đề thích hợp các phương pháp được Wiener dùng trong bài báo đã phân tích ở trên, ông đã thiết lập một định lý tồn tại tổng quát cho các giới hạn ngược của các độ đo trên các không gian hàm, là một trường hợp riêng của ĐL. 1 của §4, No. 2 tương ứng với các không gian Polish.

Một lớp các hệ ngược hạn chế hơn đã được Bochner (XIV) đưa vào năm 1947; đó là các hệ ngược được tạo thành bởi các không gian vectơ thực hữu hạn chiều và các ánh xạ tuyến tính toàn ánh. Giới hạn ngược của một hệ như vậy có thể được đồng nhất một cách tự nhiên với đối ngẫu đại số $E^*$ của một không gian vectơ thực $E$, được trang bị tôpô yếu $\sigma(E^*, E)$; một hệ ngược tương ứng của các độ đo có một giới hạn là một độ đo $\mu$ xác định trên một tộc đáng kể nhỏ hơn tộc Borel của $E^*$. Bochner đã đặc trưng hoàn toàn các 'độ đo pro' như vậy bằng biến đổi Fourier của chúng, là một hàm trên $E$. Nhưng kết quả này hầu như không thể sử dụng được khi không có một tôpô trên $E$, trong trường hợp đó người ta phải xét khả năng xem $\mu$ như một độ đo trên đối ngẫu tôpô $E'$ của $E$. Một cách độc lập, R. Fortet và E. Mourier, trong khi tìm cách mở rộng cho các biến ngẫu nhiên nhận giá trị trong một không gian Banach một số kết quả cổ điển của Lý thuyết Xác suất (luật số lớn, định lý giới hạn trung tâm), cũng đã làm nổi bật vai trò cơ bản do biến đổi Fourier đóng trong các vấn đề như vậy. Nhưng tiến bộ đáng kể chỉ đạt được vào năm 1956 khi Gelfand (XV, b)) đề xuất rằng đặt tự nhiên cho biến đổi Fourier không phải là các không gian Banach hay các không gian Hilbert, mà là các không gian Fréchet hạt nhân. Ông phỏng đoán rằng mọi hàm liên tục kiểu dương trên một không gian như vậy đều là biến đổi Fourier của một độ đo trên đối ngẫu của nó, một kết quả được Minlos (XVI) thiết lập ngay sau đó. Tầm quan trọng của nó trước hết bắt nguồn từ việc nó áp dụng được cho các không gian phân phối, và rằng gần như toàn bộ các không gian hàm là các tập hợp Borel của không gian các phân phối (do đó tạo thành một vật chứa tốt hơn nhiều so với $\mathbf{R}^T$).$^{(11)}$ Lý thuyết các phân phối ngẫu nhiên là một lĩnh vực đang mở rộng đầy đủ, và chúng tôi sẽ chỉ bằng lòng với việc dẫn độc giả tới cuốn sách của Gelfand và Vilenkin (XVII).

(10) Để có một thảo luận chi tiết về bài toán dựng các độ đo trên các không gian hàm, và các phương pháp được sử dụng trước Prokhorov, xem J. L. DOOB, Bull. Amer. Math. Soc. 53 (1947), 15–30.
(11) Có thể tham khảo phần trình bày của X. FERNIQUE, Ann. Inst. Fourier 17 (1967), 1–92, cũng chứa nhiều kết quả về hội tụ chặt.

Các kết quả về các giới hạn ngược vừa được nhắc đến sử dụng sự tồn tại của các tôpô trên các không gian cơ sở. Người ta có thể hỏi liệu có tồn tại một lý thuyết tương tự trong trường hợp các độ đo 'trừu tượng' hay không. Von Neumann đã chứng minh vào năm 1935 sự tồn tại của các độ đo tích trong mọi trường hợp, nhưng việc phát hiện một ví dụ ngược bởi Jessen và Andersen (XVIII) đã dập tắt hy vọng rằng mọi hệ ngược của các độ đo đều có một giới hạn. Hai biện pháp xoa dịu đã được phát hiện: vào năm 1949, C. Ionescu-Tulcea đã thiết lập sự tồn tại của các giới hạn ngược đếm được, nhờ sự tồn tại của các phép phân rã thích hợp,(12) một kết quả rất đáng quan tâm đối với việc nghiên cứu các quá trình Markoff; hơn nữa, người ta đã nhận thấy rằng tôpô của các không gian chỉ can thiệp thông qua trung gian là tập hợp các tập compact. Vì vậy, tự nhiên là thử tiên đề hóa tình huống này trong phạm vi lý thuyết trừu tượng, bằng khái niệm lớp compact của các tập con của một tập hợp. Công việc này được thực hiện vào năm 1953 bởi Marczewski (người đã thiết lập một định lý giới hạn ngược trừu tượng bằng các phương tiện như vậy) và Ryll-Nardzewski (người đã xử lý sự phân rã của các độ đo).(13)

(12) Dường như chính sự thiếu vắng một lý thuyết thỏa đáng về phân rã là điều đánh dấu giới hạn của lý thuyết các độ đo 'trừu tượng'. Khó khăn này xuất hiện trở lại một cách dai dẳng trong Lý thuyết Xác suất liên quan đến các xác suất có điều kiện.
(13) Để có một trình bày về lý thuyết này, có thể tham khảo J. PFANZAGL và W. PIERLO, Lecture Notes in Mathematics (Springer–Verlag), Vol. 16 (1966).

Các độ đo trên các không gian tôpô tổng quát và hội tụ chặt

Việc nghiên cứu các mối liên hệ giữa tôpô và lý thuyết độ đo trước hết đã được quan niệm như việc nghiên cứu các tính chất chính quy của các độ đo, và đặc biệt là tính chính quy 'ngoài' và tính chính quy 'trong';(14) tính chính quy trong tương đương với tính chính quy ngoài trên một không gian compact địa phương đếm được tại vô hạn. Phép dựng mà Lebesgue đưa ra cho độ đo của các tập con của đường thẳng làm nổi bật hai loại tính chính quy này, và tính chất chính quy ngoài của các độ đo trên một không gian Polish dường như đã có tiếng tăm công khai vào khoảng năm 1935. Nhưng mãi đến năm 1940, trong một bài báo mà sự phổ biến bị trì hoãn bởi chiến tranh, A. D. Alexandroff (XIX) mới làm nổi bật vai trò của tính chính quy trong và chỉ ra rằng nó được các độ đo trên một không gian Polish sở hữu; kết quả này sau đó được Prokhorov (XIII) phát hiện lại và thường bị quy nhầm cho tác giả này. Mãi đến rất gần đây người ta mới nhận thấy rằng tính chất này mở rộng đến các không gian Souslin; vì điều này,

(14) Một độ đo 'trừu tượng' $\mu$ trên tộc Borel của một không gian tôpô Hausdorff được gọi là chính quy ngoài nếu độ đo của mọi tập Borel là cận dưới lớn nhất của các độ đo của các tập mở chứa nó; độ đo $\mu$ được gọi là chính quy trong nếu độ đo của mọi tập Borel là cận trên nhỏ nhất của các độ đo của các tập compact của nó.

tầm quan trọng của các không gian này đã tăng lên rất nhiều, thậm chí còn hơn nữa khi người ta nhận ra rằng lý thuyết của chúng có thể được xây dựng mà không cần giả thiết mêtric hóa, và rằng gần như toàn bộ các không gian hàm đều là Souslin (thường hơn nữa, là Lusin).(15) Đây là những lý do khiến chúng tôi đặt trọng tâm vào các độ đo chính quy trong trong chương này.

Việc định nghĩa một mode hội tụ (mơ hồ hay chặt) cho các độ đo được làm thuận tiện nhất bằng cách đặt không gian các độ đo vào thế đối ngẫu với một không gian các hàm liên tục. Khái quát hóa một kết quả cũ của F. Riesz, A. A. Markoff đã thiết lập năm 1938 một sự tương ứng một-một giữa các phiếm hàm dương trên $\mathcal{C}(X)$ và các độ đo chính quy trên một không gian compact X. Trong công trình (XIX) đã được dẫn ở trên, A. D. Alexandroff mở rộng các kết quả này sang trường hợp một không gian hoàn toàn chính quy: ông đưa vào một thứ bậc trong tập hợp các dạng tuyến tính dương trên không gian $\mathcal{C}^b(X)$ của các hàm liên tục bị chặn trên một không gian hoàn toàn chính quy X,(16) ông định nghĩa sự hội tụ chặt của các độ đo bị chặn và chứng minh trong số đó, ngoài ra, hai định lý sau:

a) nếu X là Polish, tập hợp các dạng tuyến tính trên $\mathcal{C}^b(X)$ tương ứng với các độ đo là đóng đối với sự hội tụ yếu của các dãy;
b) nếu một dãy các độ đo bị chặn có một giới hạn chặt, thì 'không có khối lượng nào thoát ra ở vô cực' (đây là một dạng yếu của mệnh đề đảo của định lý Prokhorov về hội tụ chặt).

Từ sự phong phú của các khái niệm và định lý này, Prokhorov đã có thể rút ra những kết quả quan trọng cho lý thuyết các quá trình ngẫu nhiên, và trình bày chúng dưới một dạng đơn giản và nổi bật. Trong công trình lớn năm 1956 đã được dẫn ở trên (XIII), một phần lớn dành cho các độ đo dương bị chặn trên một không gian Polish; khái quát hóa một phép dựng của Lévy, ông định nghĩa một mêtric trên tập hợp các độ đo dương có khối lượng 1 làm cho nó trở thành một không gian Polish, rồi thiết lập một tiêu chuẩn compact quan trọng cho sự hội tụ chặt (xem §5, No. 5, Th. 1). Độc lập với Prokhorov, Le Cam (XX) đã thu được một số kết quả compact cho sự hội tụ chặt của các độ đo; ông không đặt ra giả thiết khả metr hóa nào trên các không gian mà ông xét, và các kết quả của ông rút gọn về các định lý trước đó của Dieudonné trong trường hợp compact địa phương.

(15) Để cố gắng giải quyết một số khó khăn xác suất (cụ thể là các quan hệ giữa những khái niệm khác nhau về độc lập hay phụ thuộc ngẫu nhiên), một số tác giả đã đưa vào các lớp hạn chế của các độ đo 'abstract': các không gian 'hoàn hảo' của Kolmogoroff-Gnedenko, các không gian 'Lusin' của Blackwell, các không gian 'Lebesgue' của Rokhlin. Thực ra (ít nhất giả sử một giả thiết đếm được khá yếu), tất cả các định nghĩa này đều cho những đặc trưng của các độ đo 'abstract' đẳng cấu với một độ đo dương bị chặn trên một không gian Souslin. Về chủ đề này, có thể xem công trình được dẫn ở chú thích (13).

(16) Ông phân biệt, theo thứ tự giảm dần về tính tổng quát, giữa các $\sigma$-độ đo (các độ đo 'abstract' trên bộ tộc Borel của X ), các $\tau$-độ đo (các độ đo chính quy ngoài) và các độ đo taut (các độ đo chính quy trong). Khi X là Polish, ba khái niệm này trùng nhau. Chính thuật ngữ này là do McShane và Le Cam (XX) đưa ra. Có thể tìm một bản tường thuật về các công trình mà sự phân loại này đã dẫn tới trong V. S. VARADARAJAN (Amer. Math. Soc. Transl. (2), 48, 161–228).

(I) Ch. de la Vallée Poussin, Intégrales de Lebesgue, Fonctions d’ensembles, Classes de Baire, Paris (Gauthier–Villars), ấn bản thứ nhất, 1916; ấn bản thứ hai, 1936.

(II) M. Fréchet: a) Sur l’intégrale d’une fonctionnelle étendue à un ensemble abstrait, Bull. Soc. Math. France, 43 (1915), pp. 248–265; b) Les familles et fonctions additives d’ensembles abstraits, Fund. Math., 4 (1923), pp. 329–365; ibid. 5 (1924), pp. 206–251.

(III) S. Saks, Theory of the Integral, ấn bản thứ hai, New York (Stechert), 1937.

(IV) E. Borel, Les probabilités dénombrables et leurs applications arithmétiques, Rend. Circ. Math. Palermo, 27 (1909), pp. 247–271.

(V) H. Steinhaus, Les probabilités dénombrables et leur rapport à la théorie de la mesure, Fund. Math., 4 (1923), pp. 286–310.

(VI) P. J. Daniell: a) Integrals in an infinite number of dimensions, Ann. of Math., 20 (1918–19), pp. 281–288; b) Functions of limited variation in an infinite number of dimensions, ibid. 21 (1919–20), pp. 30–38.

(VII) B. Jessen, The theory of integration in a space of an infinite number of dimensions, Acta Math., 63 (1934), pp. 249–323.

(VIII) A. Einstein, Investigations on the Theory of the Brownian Movement, New York (Dover), 1956.

(IX) P. LÉVY: a) Leçons d’Analyse Fonctionnelle, Paris (Gauthier–Villars), 1922 (ấn bản thứ hai xuất hiện năm 1951 cùng nhà xuất bản, dưới nhan đề Problèmes concrets d’Analyse Fonctionnelle); b) Processus stochastiques et mouvement brownien, Paris (Gauthier–Villars), 1948; c) Le mouvement brownien, Mémor. Sci. Math., 126 (1954).

(X) N. WIENER, Differential space, J. Math. Phys. MIT, 2 (1923), pp. 131–174 (= Selecta, pp. 55–98, Cambridge (MIT Press), 1964).

(XI) R. E. A. C. PALEY and N. WIENER, Fourier transforms in the complex domain, Amer. Math. Soc. Colloq. Publ. No. 19, New York, 1934.

(XII) A. N. KOLMOGOROFF, Grundbegriffe der Wahrscheinlichkeitsrechnung, Berlin (Springer), 1933.

(XIII) Ju. V. PROKHOROV, Convergence of random processes and limit theorems in probability theory, Theor. Probability Appl., 1 (1956), pp. 156–214.

(XIV) S. BOCHNER, Harmonic Analysis and the Theory of Probability, Berkeley (University of California Press), 1960.

(XV) I. M. GELFAND: a) Generalized stochastic processes (in Russian), Dokl. Akad. Nauk SSSR, 100 (1955), pp. 853–856; b) Some problems of functional analysis (in Russian), Uspehi Mat. Nauk, 11 (1956), pp. 3–12 (= Amer. Math. Soc. Transl. (2), 16 (1960), pp. 315–324).

(XVI) R. A. MINLOS, Generalized random processes and their extension to a measure (in Russian), Trudy Moskov. Math. Obšč., 8 (1959), pp. 497–518 (= Selected translations in mathematical statistics and probability, III (19), pp. 291–313).

(XVII) I. M. GELFAND and N. Ya. VILENKIN, Generalized Functions, Vol. IV, New York (Academic Press), 1964 (English translation).

(XVIII) E. SPARRE-ANDERSSON and B. JESSEN, Về việc đưa độ đo vào các tập tích vô hạn, Dansk. Vid. Selbskab. Mat. Fys. Medd., 25 (1948), No. 4, pp. 1–7.

(XIX) A. D. ALEXANDROFF, Các hàm tập hợp cộng tính trong các không gian trừu tượng. I (Ch. 1), Mat. Sbornik, 8 (1940), pp. 307–348; II (Chs. 2 and 3), ibid., 9 (1941), pp. 563–628; III (Chs. 4 to 6), ibid., 13 (1943), pp. 169–238.

(XX) L. LE CAM, Sự hội tụ theo phân phối của các quá trình ngẫu nhiên, Univ. Cal. Publ. Statistics, No. 11 (1957), pp. 207–236.

Chỉ mục ký hiệu

Các số tham chiếu chỉ, theo thứ tự, chương, tiết diện và tiểu mục.

Chương VII:

$\gamma_X(s) ,\ \gamma(s)$: VII, 1, 1.
$\gamma(s)f ,\ \gamma(s)\mu$ ($f$ là một hàm, $\mu$ là một độ đo): VII, 1, 1.
$d\mu(s^{-1}x)$: VII, 1, 1.
$\delta_X(s) ,\ \delta(s) ,\ \delta(s)f ,\ \delta(s)\mu,\ d\mu(xs)$: VII, 1, 1.
$\check{f} ,\ \check{\mu} ,\ d\mu(x^{-1})$ ($f$ là một hàm, $\mu$ là một độ đo): VII, 1, 1.
$\Delta_G ,\ \Delta$: VII, 1, 3.
$\mathrm{mod}_G \varphi ,\ \mathrm{mod}\varphi$ ($\varphi$ là một tự đẳng cấu): VII, 1, 4.
$\mathbf{Z}_p$ ($p$ là một số nguyên tố): VII, 1, 6.
$K^+$ ($K$ là một trường): VII, 1, 10.
$\mathrm{mod}_K a ,\ \mathrm{mod}\ a$ ($a$ là một phần tử của một trường địa phương compact $K$): VII, 1, 10.
$\mathcal{H}^\chi(X) ,\ \mathcal{H}_+^\chi(X) ,\ \mathcal{H}^1(X) ,\ f^\chi ,\ f^1$ ($X$ là một không gian địa phương compact trong đó một nhóm địa phương compact $H$ tác động, $\chi$ là một biểu diễn liên tục của $H$ trong $\mathbf{R}_+^*$): VII, 2, 1.
$f^b$: VII, 2, 2.
$\lambda^{\#} ,\ \frac{\mu}{\beta} ,\ \mu/\beta$: VII, 2, 2.
$m^{\#}$ ($m$ là một độ đo vectơ): VII, 2, 2.
$T_J ,\ T_1(n,K) ,\ T(n,K) ,\ T(n,K)^*$: VII, 3, 3.

Chương VIII:

$*_{i=1}^n \mu_i ,\ *\varphi(\mu_i)_{1 \leq i \leq n} ,\ \mu_1 * \mu_2 * \cdots * \mu_n$: VIII, 1, 1.
$\gamma_\chi$: VIII, 2, 3 and VIII, 2, 4.
$\gamma_{\chi,p}$: VIII, 2, 5.
$U(\mu)$ ($U$ là một biểu diễn của một nhóm địa phương compact $G$, $\mu$ là một độ đo trên $G$): VIII, 2, 6.
$\mathcal{M}^\rho(G)$ ($G$ là một nhóm địa phương compact): VIII, 3, 1.
$\mu *^\beta f ,\ \mu * f$ ($\mu$ là một độ đo, $f$ là một hàm): VIII, 4, 1.
$\mathcal{L}(G)$ ($G$ là một nhóm địa phương compact): VIII, 4, 5.
$\mathcal{U}_s^\infty(G)$ ($G$ là một nhóm địa phương compact): VIII, 4, Exer. 21.

Chương IX:

\mathcal{F}_+(T), \mathcal{F}_+, f_A, f^0: các quy ước sơ bộ.
\pi(p), p_A \text{ or } p|A: IX, 1, 1.
$\mathcal{P}(T; \mathbf{C}), \mathcal{P}(T; \mathbf{R}), \mathcal{P}(T), \mathcal{P}_+(T)$ : IX, 1, 2.
w^\bullet(f), \int^\bullet f dw, \int^\bullet f(t) dw(t): IX, 1, 2.
$w^\bullet, w_K^\bullet$ : IX, 1, 2.
$w^+, w^-, |w|$ : IX, 1, 2.
\mu(f), \mu(A): IX, 1, 5.
\operatorname{Supp}(\mu): IX, 1, 6.
$\sum_{i \in I} \mu_i$ : IX, 1, 7.
\mu^*(f), \mu^*(A), \int^* f d\mu, \int^* f(t) d\mu(t): IX, 1, 9.
$\mu^*$ : IX, 1, 9.
\overline{\mathcal{L}}^p(T, \mu), \overline{\mathcal{L}}_F^p(T, \mu), \mathcal{L}^p(T, \mu), \mathcal{L}_F^p(T, \mu) \text{ (cho } 1 \leq p \leq +\infty): IX, 1, 10.
$\overline{\mathcal{L}}_F^p(\mu), \overline{\mathcal{L}}_F^p, \overline{\mathcal{L}}^p, \overline{\mathcal{L}}^p(\mu), \mathcal{L}^p(\mu), \mathcal{L}^p$ : IX, 1, 10.
$\overline{N}_p(f), N_p(f), \overline{\mathcal{N}}_F, \mathcal{N}_F$ : IX, 1, 10.
$L_F^p(\mu), L_F^p$ : IX, 1, 10.
$\int f d\mu, \mu(f), \int f(t) d\mu(t)$ : IX, 1, 10.
$\mu_X^\bullet, \mu_X, \mu|X$ : IX, 2, 1.
$f \cdot \mu$ : IX, 2, 2.
\pi(\mu): IX, 2, 3.
$\lambda \otimes \mu$ : IX, 2, 5.
\mathcal{K}(T), \mathcal{B}(T): các quy ước của §3.
\mathcal{C}^b(T; F), \mathcal{C}^b(T), \mathcal{C}^b, \mathcal{C}_+^b(T), \mathcal{C}_+^b: các quy ước của §5.
\mathcal{M}^b(T; \mathbf{C}), \mathcal{M}^b(T), \mathcal{M}^b, \mathcal{M}_+^b(T), \mathcal{M}_+^b: các quy ước của §5.
$\mathcal{L}\mu$ : IX, 5, 7.
$\mathcal{F}(E)$ : IX, 6, 1.
p_V, p_{VW}: IX, 6, 1.
$\mathcal{Q}(E)$ : IX, 6, 1.
$\tilde{\lambda}$ : IX, 6, 1.
u(\mu) ($\mu$ là một tiền độ đo): IX, 6, 2.
\mathcal{F}\mu ($\mu$ là một tiền độ đo hoặc một độ đo): IX, 6, 3.
\Gamma_Q, \gamma_a: IX, 6, 5.
\gamma_C: IX, 6, 6.
\operatorname{Tr}(Q/H): IX, Annex, 1.
u^*: IX, Annex, 2.

Chỉ mục thuật ngữ

Các số tham chiếu chỉ, theo thứ tự, chương, tiết diện và tiểu mục (hoặc, một cách đặc biệt, bài tập).

Độ đo trừu tượng, tích phân: IX, 3, Exer. 4.
Hàm tập hợp cộng tính: IX, 3, 2.
Cộng tính, đếm được (hàm tập hợp): IX, 3, 2.
Ánh xạ liên hợp của một ánh xạ tuyến tính: IX, Annex, 2.
Đại số tam giác (trên, dưới): VII, 3, 3.
Hầu khắp nơi: IX, 1, 9.
Tiền độ đo liên kết với một độ đo: IX, 6, 1.
Gauge nguyên tử: IX, 3, Exer. 9.
Cơ sở $\mu$, độ đo có: IX, 2, 2.
Định lý Bochner: IX, 6, 12.
Bao trùm bị chặn: IX, 1, 1.
Độ đo bị chặn: IX, 1, 2.
Hàm tập hợp bị chặn: IX, 3, 2.
Bất đẳng thức Brunn–Minkowski: VII, 1, Exer. 25.
Lực lượng siêu không tới được: IX, 3, Exer. 13, footnote.
Lực lượng Ulam: IX, 3, Exer. 11.
Đặc trưng của một nửa nhóm đơn vị: IX, 5, 7.
Tập trung trên một tập con (bao trùm): IX, 1, 1.
Tập trung trên một tập con (độ đo): IX, 1, 4.
Biểu diễn tuyến tính liên tục: VIII, 2, 1.
Biểu diễn tuyến tính đối ngẫu: VIII, 2, 2.
Tích chập của một dãy hữu hạn các độ đo: VIII, 1, 1.
Tích chập của các hàm: VIII, 4, 5.
Các hàm có thể tích chập: VIII, 4, 5.
Độ đo và hàm có thể tích chập: VIII, 4, 1.
Có thể tích chập, $\varphi$-có thể tích chập (dãy hữu hạn các độ đo): VIII, 1, 1.
Hàm tập hợp cộng tính đếm được: IX, 3, 2.
Ma trận hiệp phương sai của một độ đo Gauss: IX, 6, 6.
Hiệp phương sai của một tiền độ đo Gauss trên $\mathbf{R}^T$: IX, 6, 6.
Tập hẹp các độ đo bị chặn: VIII, 3, Exer. 10.

Nén: IX, 1, 8.
Phân tích Iwasawa của $\mathbf{GL}(n, K)$: VII, 3, 3.
Mật độ của một độ đo đối với một độ đo khác: IX, 2, 2.
Thước đo phân tán: IX, 3, Bài tập 9.
Phân rã của một độ đo: IX, 2, 7.
Miền cơ bản: VII, 2, 10.
Tải: IX, 1, 1.
Tải, bị chặn: IX, 1, 1.
Tải, tập trung trên một tập con: IX, 1, 1.
Tải, ảnh: IX, 1, 1.
Tải, cảm sinh: IX, 1, 1.
Tải, địa phương bị chặn: IX, 1, 1.
Biểu diễn tuyến tính đều liên tục: VIII, 2, 1.
Nguyên trên cốt yếu: IX, 1, 2.
Hàm bị chặn cốt yếu: IX, 1, 10.
Hàm khả tích cốt yếu: IX, 1, 10.
Dãy hữu hạn $\varphi$-khả tích chập của các độ đo: VIII, 1, 1.
Dạng bậc hai hạt nhân: IX, Phụ lục, 1.
Monoid con đầy đủ: IX, 5, 7.
Hàm kiểu dương: IX, 6, 12.
Hàm bị chặn cốt yếu: IX, 1, 10.
Hàm khả tích cốt yếu: IX, 1, 10.
Hàm sinh (của một dãy): IX, 5, 7.
Hàm khả tích: IX, 1, 10.
Hàm khả tích địa phương: IX, 2, 2.
Hàm không đáng kể địa phương: IX, 1, 4.
Hàm đo được: IX, 1, 5.
Hàm điều độ: IX, 1, 9.
Hàm môđun (của một nhóm địa phương compact): VII, 1, 3.
Hàm không đáng kể: IX, 1, 9.
Hàm đo được phổ quát: IX, 2, 7.
Miền cơ bản: VII, 2, 10.
G-bao phủ: VII, 1, Bài tập 27.
G-lấp đầy: VII, 1, Bài tập 27.
G-lát: VII, 1, Bài tập 27.
Thước đo trên một tập hợp X: IX, 3, Bài tập 9.
Độ đo Gaussian, tiền độ đo: IX, 6, 5.
Độ đo Gaussian với ma trận hiệp phương sai $C$: IX, 6, 6.
Tiền độ đo Gaussian với hiệp phương sai $K$: IX, 6, 6.

Tiền độ đo Gaussian, chính tắc, trên một không gian Hilbert thực: IX, 6, 6. Nhóm tuyến tính tổng quát: VII, 3, 3. Hàm sinh của một dãy: IX, 5, 7. Nhóm tam giác lớn (trên, dưới): VII, 3, 3. Nhóm tam giác đặc biệt (trên, dưới): VII, 3, 3. Nhóm tam giác ngặt (trên, dưới): VII, 3, 3. Nhóm đơn môđula: VII, 1, 3. Độ đo Haar (trái, phải): VII, 1, 2. Ánh xạ Hilbert–Schmidt: IX, Phụ lục, 2. Ảnh của một độ đo: IX, 2, 3. Ảnh của một tiền độ đo: IX, 6. 2. Ảnh của một tải: IX, 1, 1. Tải cảm sinh: IX, 1, 1. Độ đo cảm sinh: IX, 2, 1. Bất đẳng thức Brunn–Minkowski: VII, 1, Bài tập 25. Hàm tập hợp nội chính quy: IX, 3, 2. Các số nguyên $p$-adic: VII, 1, 6. Hàm khả tích: IX, 1, 10. Tập hợp khả tích: IX, 1, 9. Nguyên trừu tượng: IX, 3, Bài tập 4. Nguyên trên cốt yếu: IX, 1, 2. Nguyên trên: IX, 1, 9. Nguyên của một hàm: IX, 1, 10. Độ đo bất biến (trái, phải) trên một nhóm: VII, 1, 1. Độ đo bất biến, dưới tác dụng của một nhóm các toán tử: VII, 1, 1. Giới hạn nghịch (hoặc xạ ảnh) của các độ đo trên một giới hạn nghịch (hoặc xạ ảnh) của các nhóm địa phương compact: VII, 1, 6. Giới hạn nghịch (hoặc xạ ảnh) của các độ đo: IX, 4, 2. Hệ nghịch (hoặc xạ ảnh) của các độ đo: IX, 4, 2. Biểu diễn tuyến tính đẳng cự: VIII, 2, 1. Phân tích Iwasawa của $\mathbf{GL}(n, K)$: VII, 3, 3. Hạt nhân kiểu dương: IX, 6, 6. Định lý Lagrange: VII, 1, Bài tập 29. Phép biến đổi Laplace: IX, 5, 7. Nhóm tam giác lớn (trên, dưới): VII, 3, 3. Độ đo Haar trái: VII, 1, 2. Nhân tử trái của một độ đo tương đối bất biến trên một nhóm địa phương compact: VII, 1, 8. Độ đo bất biến trái trên một nhóm: VII, 1, 1. ng compact: VII, 1, 8. Độ đo bất biến trái trên một nhóm: VII, 1, 1.

Định lý của P. Levy: IX, 5, Bài tập 13. Phép nâng các độ đo: IX, 2, 4. Giới hạn nghịch (hoặc xạ ảnh) của các độ đo trên một giới hạn nghịch (hoặc xạ ảnh) của các nhóm địa phương compact: VII, 1, 6. Giới hạn nghịch (hoặc xạ ảnh) của các độ đo: IX, 4, 2. Biểu diễn tuyến tính chuyển vị, đối ngẫu của một biểu diễn tuyến tính: VIII, 2, 2. Địa phương hầu như khắp nơi: IX, 1, 4. Tải địa phương bị chặn: IX, 1, 1. Hàm tập hợp địa phương bị chặn: IX, 3, 2. Hàm khả tích địa phương: IX, 2, 2. Hàm không đáng kể địa phương: IX, 1, 4. Tập hợp không đáng kể địa phương: IX, 1, 4. Ánh xạ Hilbert–Schmidt: IX, Phụ lục, 2. Ánh xạ $\mu$-thực sự: IX, 2, 3. Các biên của một độ đo trên một không gian hàm: IX, 4, 3. Khối lượng toàn phần (của một tiền độ đo): IX, 6, 1. Trung bình quỹ đạo: VII, 2, 2. Hàm đo được: IX, 1, 5. Tập hợp đo được: IX, 1, 5. Độ đo: IX, 1, 2. Độ đo trừu tượng: IX, 3, Bài tập 4. Độ đo trên $\mathbf{Q}_p$, Haar chuẩn hoá: VII, 1, 6. Độ đo bị chặn: IX, 1, 2. Độ đo Gaussian với ma trận hiệp phương sai $C$: IX, 6, 6. Độ đo Gaussian với phương sai $Q$: IX, 6, 5. Độ đo Haar (trái, phải), trên một nhóm địa phương compact: VII, 1, 2. Ảnh của một độ đo: IX, 2, 3. Độ đo cảm sinh: IX, 2, 1. Độ đo bất biến (tương đối bất biến, gần bất biến) dưới tác dụng của một nhóm các toán tử: VII, 1, 1. Độ đo bất biến trái (phải), trên một nhóm địa phương compact: VII, 1, 1. Phép nâng các độ đo: IX, 2, 4. Độ đo điều độ: IX, 1, 9. Độ đo Haar chuẩn hoá, trên một nhóm compact, trên một nhóm rời rạc: VII, 1, 3. Độ đo ngoài (của một tập hợp): IX, 1, 9. Độ đo tích: IX, 2, 5. Độ đo gần bất biến, trên một nhóm địa phương compact: VII, 1, 9. Độ đo tương đối bất biến, trên một nhóm địa phương compact: VII, 1, 8.

Độ đo Wiener: IX, 6, 7.
Độ đo, với cơ sở $\mu$: IX, 2, 2.
Độ đo, với mật độ $f$ đối với một độ đo $\mu$: IX, 2, 2.
Không gian có độ đo: IX, 6, 7, Chú thích (2).
Định lý Minkowski: VII, 1, Bài tập 27.
Định lý Minlos: IX, 6, 10.
Hàm điều độ: IX, 1, 9.
Độ đo điều độ: IX, 1, 9.
Tập hợp điều độ: IX, 1, 9.
Hàm môđun của một nhóm compact địa phương: VII, 1, 3.
Môđun của một nhóm compact địa phương: VII, 1, 3.
Môđun của một tự đẳng cấu: VII, 1, 4.
Nhân tử (trái, phải) của một độ đo bất biến tương đối trên một nhóm compact địa phương: VII, 1, 8.
Nhân tử trên một tích $G \times X$ của một nhóm $G$ và một tập hợp $X$ mà $G$ tác động lên: VIII, 2, 3.
Nhân tử của một độ đo bất biến tương đối dưới một nhóm toán tử: VII, 1, 1.
Hàm bỏ qua được: IX, 1, 9.
Tập hợp bỏ qua được: IX, 1, 9.
Độ đo Haar chuẩn hóa trên một nhóm compact, trên một nhóm rời rạc: VII, 1, 3.
Độ đo Haar chuẩn hóa trên $Q_p$: VII, 1, 6.
Dạng toàn phương hạt nhân: IX, Annex, 1.
Không gian hạt nhân: IX, 6, 10.
Trung bình quỹ đạo: VII, 2, 2.
Độ đo ngoài: IX, 1, 9.
Các số nguyên $p$-adic: VII, 1, 6.
Tiền độ đo dương, độ đo: IX, 1, 2.
Hàm loại dương: IX, 6, 12.
Hạt nhân loại dương: IX, 6, 6.
Tiền độ đo: IX, 1, 2.
Tiền độ đo dương: IX, 1, 2.
Tiền độ đo thực: IX, 1, 2.
Tích của một họ các độ đo: IX, 4, 3.
Tích của hai độ đo: IX, 2, 5.
Tích chập (của một độ đo và một hàm): VIII, 4, 1.
Tích chập (của các hàm): VIII, 4, 5.
Tích chập (của các độ đo), theo một ánh xạ: VIII, 1, 1.
Giới hạn xạ ảnh (hay nghịch đảo) của các độ đo: IX, 4, 2.

Hệ xạ ảnh (hay nghịch đảo) của các độ đo: IX, 4, 2.
Các điều kiện của Prokhorov: IX, 4, 2 và IX, 5, 5.
Độ đo sơ khởi: IX, 6, 1.
Độ đo sơ khởi liên kết với một độ đo: IX, 6, 1.
Độ đo sơ khởi Gauss chính tắc, trên một không gian Hilbert thực: IX, 6, 6.
Biến đổi Fourier của độ đo sơ khởi: IX, 6, 3.
Độ đo sơ khởi Gauss với hiệp phương sai $K$, trên $\mathbf{R}^T$: IX, 6, 6.
Độ đo sơ khởi Gauss với phương sai $Q$: IX, 6, 5.
Ảnh của độ đo sơ khởi: IX, 6, 2.
Tổng khối lượng của một độ đo sơ khởi: IX, 6, 1.
Ánh xạ $\mu$-thực sự: IX, 2, 3.
Dạng toàn phương hạt nhân: IX, Annex, 1.
Độ đo gần bất biến trên một nhóm compact địa phương: VII, 1, 9.
Độ đo gần bất biến, dưới một nhóm toán tử: VII, 1, 1.
Thương của một độ đo trên một không gian compact địa phương $X$ theo một độ đo Haar của một nhóm tác động trên $X$: VII, 2, 2.
Không gian Radon: IX, 3, 3.
Độ đo thực, tiền độ đo: IX, 1, 2.
Biểu diễn chính quy (trái, phải): VIII, 2, 5.
Sự chính quy hóa: VIII, 4, 7.
Độ đo bất biến tương đối, trên một nhóm compact địa phương: VII, 1, 8.
Độ đo bất biến tương đối, dưới một nhóm toán tử: VII, 1, 1.
Biểu diễn, liên tục (liên tục riêng rẽ, đều liên tục, đẳng cự): VIII, 2, 1.
Biểu diễn, chính quy (trái, phải): VIII, 2, 5.
Biểu diễn đơn vị: VIII, 2, Bài tập 4.
Độ đo Haar phải: VII, 1, 2.
Nhân tử phải của một độ đo bất biến tương đối trên một nhóm compact địa phương: VII, 1, 8.
Độ đo bất biến phải trên một nhóm: VII, 1, 1.
Tôpô Sazonov: IX, 6, 10.
Liên tục riêng rẽ (biểu diễn tuyến tính): VIII, 2, 1.
Hàm tập hợp cộng tính: IX, 3, 2.
Hàm tập hợp bị chặn: IX, 3, 2.
Hàm tập hợp đếm được cộng tính: IX, 3, 2.
Hàm tập hợp chính quy trong: IX, 3, 2.
Hàm tập hợp bị chặn địa phương: IX, 3, 2.
Không gian hạt nhân: IX, 6, 10.
Không gian Radon: IX, 3, 3.

Không gian Radon mạnh: IX, 3, 3.
Nhóm tam giác đặc biệt (trên, dưới): VII, 3, 3.
Nhóm tam giác ngặt (trên, dưới): VII, 3, 3.
Lực lượng siêu khả cận mạnh: IX, 3, Bài tập 13, chú thích.
Không gian Radon mạnh: IX, 3, 3.
Hệ con nghịch đảo (hay xạ ảnh con) của các độ đo: IX, 4, 2.
Monoid con đầy đủ: IX, 5, 7.
Tổng của một họ các độ đo: IX, 1, 7.
Họ các độ đo khả tổng: IX, 1, 7.
Giá của một độ đo: IX, 1, 6.
Hệ nghịch đảo (hay xạ ảnh) của các độ đo: IX, 4, 2.
Hệ con nghịch đảo (hay xạ ảnh con) của các độ đo: IX, 4, 2.
Định lý Bochner: IX, 6, 12.
Định lý Lagrange: VII, 1, Bài tập 29.
Định lý Minkowski: VII, 1, Bài tập 27.
Định lý Minlos: IX, 6, 10.
Định lý P. Lévy: IX, 5, Bài tập 13.
Định lý Thue: VII, 1, Bài tập 28.
Định lý Thue: VII, 1, Bài tập 28.
Tôpô của sự hội tụ chặt: IX, 5, 3.
Tôpô chặt: IX, 5, 3.
Tôpô Sazonov: IX, 6, 10.
Tôpô chặt: IX, 5, 3.
Tổng khối lượng của một độ đo sơ khởi: IX, 6, 1.
Vết của một dạng toàn phương đối với một dạng khác: IX, Annex, 1.
Biến đổi Fourier (của một độ đo, của một độ đo sơ khởi): IX, 6, 3.
Biến đổi Laplace (của một độ đo): IX, 5, 7.
Biểu diễn tuyến tính chuyển vị: VIII, 2, 2.
Đại số tam giác: VII, 3, 3.
Nhóm tam giác (lớn, ngặt, đặc biệt): VII, 3, 3.
Lực lượng Ulam: IX, 3, Bài tập 11.
Siêu lọc Ulam: IX, 3, Bài tập 11.
Nhóm đơn môđula: VII, 1, 3.
Biểu diễn đơn vị: VIII, 2, Bài tập 4.
Hàm đo được phổ quát: IX, 2, 7.
Tập hợp đo được phổ quát: IX, 3, 3.
Tích phân trên: IX, 1, 9.
Phương sai của một độ đo: IX, 6, 5.
Độ đo Wiener: IX, 6, 7.

Các công thức liên quan đến $\gamma(s)$ và $\delta(s)$

Cho $G$ là một nhóm tôpô tác động liên tục bên trái trên một không gian compact địa phương $X$ bởi $(s, x) \mapsto sx$.

$$
\begin{align*}
\gamma(s)x &= sx & (s \in G, x \in X) \\
\gamma(st) &= \gamma(s)\gamma(t) & (s, t \text{ trong } G) \\
(\gamma(s)f)(x) &= f(s^{-1}x) & (f \text{ là một hàm trên } X) \\
\langle f, \gamma(s)\mu \rangle &= \langle \gamma(s^{-1})f, \mu \rangle & (\mu \text{ là một độ đo trên } X) \\
d(\gamma(s)\mu)(x) &= d\mu(s^{-1}x) \\
(\gamma(s)\mu)(A) &= \mu(s^{-1}A) & (\text{A là một } \gamma(s)\mu\text{-tập hợp khả tích})
\end{align*}
$$

Nếu $\mu$ là bất biến tương đối với nhân tử $\chi$,

$$
\begin{align*}
\gamma(s)\mu &= \chi(s)^{-1}\mu \\
d\mu(sx) &= \chi(s)\,d\mu(x).
\end{align*}
$$

Cho $G$ là một nhóm tôpô tác động liên tục bên phải trên một không gian compact địa phương $X$ bởi $(s, x) \mapsto xs$.

$$
\begin{align*}
\delta(s)x &= xs^{-1} \\
\delta(st) &= \delta(s)\delta(t) \\
(\delta(s)f)(x) &= f(xs) \\
\langle f, \delta(s)\mu \rangle &= \langle \delta(s^{-1})f, \mu \rangle \\
d(\delta(s)\mu)(x) &= d\mu(xs) \\
(\delta(s)\mu)(A) &= \mu(As).
\end{align*}
$$

Nếu $\mu$ là tương đối bất biến với nhân tử $\chi'$,

$$
\begin{align*}
\delta(s)\mu &= \chi'(s)\mu \\
d\mu(xs) &= \chi'(s)\,d\mu(x).
\end{align*}
$$

Các công thức liên quan đến độ đo Haar

Cho G là một nhóm compact địa phương, $\Delta$ là môđun của nó, $\mu$ là một độ đo Haar trái, $\nu$ là một độ đo Haar phải.

1) Ta có
$$
\begin{align*}
\gamma(s)\mu &= \mu \\
d\mu(sx) &= d\mu(x)
\end{align*}
$$
$$
\begin{align*}
\delta(s)\mu &= \Delta(s)\mu \\
d\mu(xs) &= \Delta(s)\, d\mu(x)
\end{align*}
$$
$$
\begin{align*}
\dot{\mu} &= \Delta^{-1} \cdot \mu \\
d\mu(x^{-1}) &= \Delta(x)^{-1}\, d\mu(x).
\end{align*}
$$

Nếu $f$ là $\mu$-khả tích,
$$
\int f(sx)\, d\mu(x) = \int f(x)\, d\mu(x)
$$
$$
\int f(xs)\, d\mu(x) = \Delta(s)^{-1} \int f(x)\, d\mu(x)
$$
$$
\int f(x^{-1})\Delta(x)^{-1}\, d\mu(x) = \int f(x)\, d\mu(x).
$$

Nếu $A \subset G$ là $\mu$-khả tích,
$$
\mu(sA) = \mu(A) \qquad \mu(As) = \Delta(s)\mu(A).
$$

2) Ta có
$$
\begin{align*}
\delta(s)\nu &= \nu \\
d\nu(xs) &= d\nu(x)
\end{align*}
$$
$$
\begin{align*}
\gamma(s)\nu &= \Delta(s)\nu \\
d\nu(s^{-1}x) &= \Delta(s)\, d\nu(x)
\end{align*}
$$
$$
\begin{align*}
\dot{\nu} &= \Delta \cdot \nu \\
d\nu(x^{-1}) &= \Delta(x)\, d\nu(x).
\end{align*}
$$

Nếu $f$ là $\nu$-khả tích,
$$
\int f(xs)\, d\nu(x) = \int f(x)\, d\mu(x)
$$
$$
\int f(xs)\, d\nu(x) = \Delta(s) \int f(x)\, d\nu(x)
$$
$$
\int f(x^{-1})\Delta(x)\, d\nu(x) = \int f(x)\, d\nu(x).
$$

Nếu $A \subset G$ là $\nu$-khả tích,
$$
\nu(As) = \nu(A) \qquad \nu(sA) = \Delta(s^{-1})\nu(A).
$$

3) $\nu$ tỉ lệ với $\Delta^{-1} \cdot \mu$, $\mu$ tỉ lệ với $\Delta \cdot \nu$.

CÁC ĐIỀU KIỆN ĐỦ CHO SỰ TỒN TẠI
CỦA TÍCH CHẬP

I. — Trường hợp tích chập $\mu * \nu$ của hai độ đo tồn tại:

(a) \* được xác định bởi một ánh xạ liên tục $\varphi : X \times Y \to Z$:
$\mu, \nu$ bị chặn (khi đó $\mu * \nu$ bị chặn và $\| \mu * \nu \| \leq \| \mu \| \cdot \| \nu \|$).
$\mu, \nu$ có giá đỡ compact (khi đó $\mu * \nu$ có giá đỡ compact và $\mathrm{Supp}(\mu * \nu) \subset \varphi(\mathrm{Supp} \mu \times \mathrm{Supp} \nu)$).

(b) \* được xác định bởi một nhóm tác động liên tục bên trái trên một không gian:
$\mu$ có giá đỡ compact, $\nu$ tùy ý.

(c) \* được xác định bởi phép nhân trong một nhóm $G$:
một trong hai độ đo có giá đỡ compact.
$\mu, \nu$ trong $\mathcal{M}^\rho(G)$ (khi đó $\mu * \nu \in \mathcal{M}^\rho(G)$, và $\| \mu * \nu \|_\rho \leq \| \mu \|_\rho \| \nu \|_\rho$).

II. — Trường hợp tích chập $\mu * f$ của một độ đo và một hàm tồn tại:

(a) \* được định nghĩa bởi một nhóm $G$ tác động liên tục bên trái trên một không gian $X$ được trang bị một độ đo $\beta \geq 0$ sao cho $\gamma(s)\beta = \chi(s^{-1}, \cdot)\beta$, với $\chi$ liên tục:
$\mu$ có giá compact, $f$ khả tích địa phương theo $\beta$ (nếu $f$ liên tục, $\mu * f$ liên tục; nếu $f$ liên tục có giá compact, $\mu * f$ liên tục có giá compact).
$G$ tác động đúng đắn trên $X$, $f \in \mathcal{K}(X)$ ($\mu * f$ liên tục).

(b) các $\chi(s, \cdot)$ bị chặn; đặt $\rho(s) = \sup_{x \in X} \chi(s^{-1}, x)$:
$\mu \in \mathcal{M}^\rho(G)$, $f \in L^\infty(X, \beta)$ (thì $\mu * f \in L^\infty(X, \beta)$; nếu $f \in C^\infty(X)$,
$\mu * f \in C^\infty(X)$; nếu $f \in \mathcal{K}(X)$, $\mu * f \in \mathcal{K}(X)$).
$\mu \in \mathcal{M}^{\rho^{1/q}}(G)$, $f \in L^p(X, \beta)$ với $1/p + 1/q = 1$ (thì $\mu * f \in L^p(X, \beta)$)
và $\| \mu * f \|_p \leq \| \mu \|_{\rho^{1/q}} \| f \|_p$.

III. — Trường hợp tích chập $f * g$ của hai hàm khả tích địa phương theo $\beta$ tồn tại ($\beta$ là một độ đo tương đối bất biến $\geq 0$ trên một nhóm $G$, với các hệ số nhân trái và phải $\chi$ và $\chi'$):

$f$ hoặc $g$ liên tục, $f$ hoặc $g$ có giá compact (thì $f * g$ liên tục;
nếu $f, g$ thuộc $\mathcal{K}(G)$ thì $f * g \in \mathcal{K}(G)$).

$$
f \chi^{-1/q} \in L^1(G, \beta) \text{ và } g \in L^p(G, \beta), \text{ với } 1/p + 1/q = 1 \text{ (thì } f * g \in L^p(G, \beta) \text{ và } \|f * g\|_p \leq \|f \chi^{-1/q}\|_1 \|g\|_p).
$$
$$
f \in L^p(G, \beta) \text{ và } g {\chi'}^{-1/q} \in L^1(G, \beta) \text{ (thì } f * g \in L^p(G, \beta) \text{ và } \|f * g\|_p \leq \|f\|_p \|g {\chi'}^{-1/q}\|_1 ).
$$
$$
f \chi^{-1} \in L^1(G, \beta) \text{ và } g \in \mathcal{C}^\infty(G) \text{ (resp. } \overline{\mathcal{K}(G)} ) \text{ (thì } f * g \in \mathcal{C}^\infty(G) \text{ (resp. } \mathcal{K}(G) ) ).
$$
$$
f \in \mathcal{C}^\infty(G, \beta) \text{ (resp. } \overline{\mathcal{K}(G)} ) \text{ và } g {\chi'}^{-1} \in L^1(G, \beta) \text{ (thì } f * g \in \mathcal{C}^\infty(G) \text{ (resp. } \mathcal{K}(G) ) ).
$$
$$
f \in L^p(G, \beta), \ g \in L^q(G, \dot{\beta}) \text{ với } 1/p + 1/q = 1, \ 1 < p < +\infty, \ \beta \text{ trái bất biến (thì } f * g \in \overline{\mathcal{K}(G)} \text{ và } \|f * g\|_\infty \leq \|f\|_p \|g\|_q ).
$$

Mục lục

CHƯƠNG VII. — ĐỘ ĐO HAAR ............................................. VII.1

§1. Phép dựng một độ đo Haar ........................................ VII.1
    1. Các định nghĩa và ký hiệu ............................................ VII.1
    2. Định lý tồn tại và duy nhất ............................... VII.6
    3. Môđun ............................................................. VII.10
    4. Môđun của một tự đẳng cấu ...................................... VII.13
    5. Độ đo Haar của một tích ......................................... VII.14
    6. Độ đo Haar của một giới hạn ngược .................................. VII.15
    7. Định nghĩa địa phương của một độ đo Haar ............................... VII.18
    8. Các độ đo tương đối bất biến ..................................... VII.19
    9. Các độ đo bán bất biến .......................................... VII.20
   10. Các trường compact địa phương ............................................ VII.21
   11. Các đại số hữu hạn chiều trên một trường compact địa phương ...... VII.25

§2. Thương của một không gian theo một nhóm; các không gian thuần nhất ............. VII.27
    1. Các kết quả tổng quát .................................................. VII.27
    2. Trường hợp $\chi = 1$ ........................................... VII.29
    3. Một cách hiểu khác của $\lambda^{\#}$ .......................... VII.32
    4. Trường hợp $X/H$ là paracompact ............................... VII.36
    5. Các độ đo bán bất biến trên một không gian thuần nhất ......... VII.38
    6. Các độ đo tương đối bất biến trên một không gian thuần nhất .. VII.43
    7. Độ đo Haar trên một nhóm thương ............................... VII.44
    8. Một tính bắc cầu .......................................... VII.45
    9. Phép dựng độ đo Haar của một nhóm từ
        các độ đo Haar của một số nhóm con ..................... VII.48
   10. Tích phân trên một miền cơ bản ............................. VII.50

§3. Ứng dụng và ví dụ ........................................... VII.53
    1. Các nhóm compact của các ánh xạ tuyến tính ............................... VII.53
    2. Tính tầm thường của các không gian sợi và của các mở rộng nhóm ..... VII.55
    3. Ví dụ: 1. Nhóm tuyến tính tổng quát ............................... VII.60
        2. Nhóm affine .................................................. VII.61
        3. Nhóm tam giác ngặt ..................................... VII.62
        4. Nhóm tam giác lớn ...................................... VII.63
        5. Nhóm tam giác đặc biệt .................................... VII.66

6. Nhóm tuyến tính đặc biệt ......................... VII.67 7. Phân tích Iwasawa của $\mathbf{GL}(n, K)$ ..... VII.69 8. Các không gian của các dạng hermitian .................... VII.72 Phụ lục I ........................................ VII.74 Phụ lục II ......................................... VII.76 Bài tập cho §1 .................................. VII.78 Bài tập cho §2 .................................. VII.87 Bài tập cho §3 .................................. VII.91

CHƯƠNG VIII. — TÍCH CHẬP VÀ BIỂU DIỄN .... VIII.1

§1. Tích chập ..................................... VIII.1
    1. Định nghĩa và ví dụ ..................... VIII.1
    2. Tính kết hợp ............................... VIII.3
    3. Trường hợp các độ đo bị chặn ............... VIII.6
    4. Các tính chất liên quan đến giá ............. VIII.6
    5. Biểu thức vectơ của tích chập ...... VIII.7

§2. Biểu diễn tuyến tính của nhóm ............... VIII.8
    1. Biểu diễn tuyến tính liên tục .......... VIII.8
    2. Biểu diễn phản liên hợp .............. VIII.10
    3. Ví dụ: biểu diễn tuyến tính trong các không gian các hàm liên tục .......................... VIII.11
    4. Ví dụ: biểu diễn tuyến tính trong các không gian độ đo .. VIII.12
    5. Ví dụ: biểu diễn tuyến tính trong các không gian $L^p$ ...... VIII.13
    6. Mở rộng một biểu diễn tuyến tính của G lên các độ đo trên G ............................... VIII.15
    7. Các quan hệ giữa các tự đồng cấu $U(\mu)$ và các tự đồng cấu $U(s)$ .................. VIII.16

§3. Tích chập của các độ đo trên các nhóm ............. VIII.18
    1. Các đại số độ đo ........................ VIII.18
    2. Trường hợp một nhóm tác động trên một không gian ........ VIII.21
    3. Tích chập và biểu diễn tuyến tính ........ VIII.22

§4. Tích chập của các độ đo và các hàm .......... VIII.24
    1. Tích chập của một độ đo và một hàm ........ VIII.24
    2. Các ví dụ về các độ đo và các hàm có thể tích chập ...... VIII.28
    3. Tích chập và chuyển vị ................ VIII.34
    4. Tích chập của một độ đo và một hàm trên một nhóm ... VIII.37
    5. Tích chập của các hàm trên một nhóm ............ VIII.38
    6. Các ứng dụng .................................. VIII.42
    7. Chính quy hóa ............................... VIII.44

§5. Không gian của các nhóm con đóng ........................................ VIII.46

1. Không gian các độ đo Haar trên các nhóm con đóng của G .................................................. VIII.46 2. Tính bán liên tục của thể tích của không gian thuần nhất VIII.48 3. Không gian các nhóm con đóng của C ......................... VIII.51 4. Trường hợp các nhóm không có các nhóm con hữu hạn nhỏ tùy ý ............................................. VIII.53 5. Trường hợp các nhóm abel .................................... VIII.55 6. Một cách giải thích khác về topo của không gian các nhóm con đóng ............................... VIII.56 Bài tập cho §1 .......................................................... VIII.59 Bài tập cho §2 .......................................................... VIII.59 Bài tập cho §3 .......................................................... VIII.61 Bài tập cho §4 .......................................................... VIII.65 Bài tập cho §5 .......................................................... VIII.73 Ghi chú lịch sử (Chs. VII và VIII) ................................. VIII.75

Chương IX. — Độ đo trên các không gian tôpô Hausdorff IX.1

§1. Tiền độ đo và độ đo trên một không gian tôpô ............ IX.1

1. Các trở ngại .................................................. IX.1 2. Các tiền độ đo và các độ đo ...................................... IX.3 3. Các ví dụ về độ đo .......................................... IX.6 4. Các tập hợp và hàm không đáng kể địa phương ....................... IX.8 5. Các tập hợp và hàm đo được ............................... IX.9 6. Các họ có hướng; giá của một độ đo ..................... IX.11 7. Các bao trên và các tổng của các độ đo ....................... IX.12 8. Các phép ép ..................................................... IX.13 9. Tích phân trên ................................................ IX.17 10. Lý thuyết tích phân ............................................. IX.20

§2. Các phép toán trên độ đo ........................................... IX.22

1. Độ đo cảm sinh trên một không gian con đo được ................... IX.22 2. Các độ đo được xác định bởi các mật độ số ..................... IX.24 3. Ảnh của một độ đo ........................................... IX.26 4. Nâng của các độ đo .......................................... IX.29 5. Tích của hai độ đo ...................................... IX.31 6. Tích phân đối với tích của hai độ đo IX.33 7. Một kết quả về sự phân rã của các độ đo ................. IX.37

§3. Độ đo và các hàm tập hợp cộng tính ............................................. IX.41
    1. Độ đo và các hàm tập hợp cộng tính của các tập compact ... IX.41
    2. Các hàm tập hợp chính quy trong ............................................. IX.44
    3. Không gian Radon ............................................................ IX.46

§4. Giới hạn ngược của các độ đo ..................................................... IX.49
    1. Bổ sung trên các không gian compact và giới hạn ngược ....... IX.50
    2. Các hệ ngược của độ đo ......................................... IX.50
    3. Trường hợp các hệ ngược đếm được ....................... IX.54

§5. Độ đo trên các không gian hoàn toàn chính quy ................................. IX.56
    1. Độ đo và các hàm liên tục bị chặn ............... IX.56
    2. Các độ đo bị chặn và các dạng tuyến tính trên $\mathcal{C}^b(T)$ .......... IX.59
    3. Sự hội tụ chặt của các độ đo bị chặn ..................... IX.60
    4. Ứng dụng: các tính chất tôpô của không gian $\mathcal{M}_+^b(T)$ IX.63
    5. Tiêu chuẩn compact cho sự hội tụ chặt ............. IX.64
    6. Sự hội tụ chặt của các độ đo và sự hội tụ compact của các hàm .................................................. IX.67
    7. Ứng dụng: Biến đổi Laplace .................. IX.68

§6. Độ đo trước và độ đo trên một không gian lồi địa phương ............ IX.72
    1. Độ đo trước trên một không gian lồi địa phương ..................... IX.72
    2. Ảnh của một độ đo trước ............................................. IX.74
    3. Biến đổi Fourier của một độ đo trước .......................... IX.75
    4. Tính toán các tích phân Gaussian ............................ IX.77
    5. Độ đo trước Gaussian và độ đo Gaussian .......................... IX.78
    6. Các ví dụ về độ đo trước Gaussian ............................ IX.82
    7. Độ đo Wiener ..................................................... IX.85
    8. Tính liên tục của biến đổi Fourier ....................... IX.92
    9. Bổ đề của Minlos ..................................................... IX.93
    10. Độ đo trên đối ngẫu của một không gian hạch ................. IX.96
    11. Độ đo trên một không gian Hilbert ................................. IX.97
    *12. Quan hệ với các hàm dương tính* ............. IX.99

PHỤ LỤC: Bổ sung về các không gian Hilbert ................................. IX.102
    1. Vết của một dạng toàn phương đối với một dạng khác ...... IX.102
    2. Các ánh xạ Hilbert–Schmidt ....................................... IX.104

Bài tập cho §1 ............................................................. IX.106
Bài tập cho §2 ............................................................. IX.108
Bài tập cho §3 ............................................................. IX.108
Bài tập cho §4 ............................................................. IX.112
Bài tập cho §5 ............................................................. IX.113
Bài tập cho §6 ............................................................. IX.117

Bài tập cho Phụ lục .................................................. IX.118
Ghi chú lịch sử ............................................................. IX.120
Chỉ mục ký hiệu .......................................................... 309
Chỉ mục thuật ngữ ....................................................... 311
Các công thức chính của Chương VII ........................................ 318
Các điều kiện đủ cho sự tồn tại của tích chập . 320
