---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: top-v-x
pdf_pages: 0353-0372
extraction: ocr
statements: 0
exercises: 0
content_sha256: 068acaca17f888e05264d0323e3938348f9b08e2d2013ecbacc265191861e163
translated_from: content/en/top/X/historical_note.md
source_content_sha256: 40b5235f4ceac5953a07d76a4ff11499284171867bddf1d36dc51ac4536b548e
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-ac1b6c34
glossary_version: 34
glossary_terms_sha256: 4da91808b1dc6f7d8df1f1551ce0ecf19d1fe92ef99f866ed0cb80ed6a72f028
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Các số trong ngoặc vuông tham chiếu đến thư mục ở cuối ghi chú này.)

Khái niệm về một hàm tùy ý hầu như chưa được biết đến vào đầu thế kỷ XIX. *A fortiori*, ý tưởng nghiên cứu các tập hợp hàm nói chung và trang bị cho chúng một cấu trúc tôpô đã không xuất hiện trước thời Riemann (xem Ghi chú lịch sử cho Chương I), và chỉ vào cuối thế kỷ XIX ý tưởng này mới được đưa vào sử dụng một cách có hệ thống.

Tuy nhiên, ý tưởng về sự hội tụ của một *dãy* các hàm nhận giá trị thực đã được sử dụng, một cách ít nhiều có ý thức, từ những buổi đầu của phép tính vô cùng bé. Dĩ nhiên, ở đây khi nói đến sự hội tụ, ta muốn nói đến sự hội tụ *từng điểm*; các kiểu hội tụ khác không thể được mô tả cho đến khi các khái niệm về chuỗi hội tụ và hàm liên tục được Bolzano và Cauchy định nghĩa một cách chính xác. Ban đầu, Cauchy không nhận ra sự khác biệt giữa hội tụ từng điểm và hội tụ đều, và tin rằng ông đã chứng minh rằng tổng của mọi chuỗi hội tụ các hàm liên tục là liên tục ([1], (2), tập 3, p. 120). Sai lầm này được Abel chỉ ra ngay lập tức, đồng thời ông cũng chỉ ra rằng mọi chuỗi lũy thừa đều liên tục bên trong khoảng hội tụ của nó, bằng một lập luận cổ điển mà trong trường hợp riêng này về bản chất đã sử dụng khái niệm hội tụ đều ([2], p. 223-224). Chỉ còn việc phát biểu khái niệm này một cách tổng quát, và điều đó đã được Stokes và Seidel thực hiện độc lập vào năm 1847-1848, và bởi chính Cauchy vào năm 1853 ([1], (1), tập 12, p. 30) (*).

Dưới ảnh hưởng của Weierstrass và Riemann, việc nghiên cứu có hệ thống khái niệm hội tụ đều và các vấn đề liên quan đã được phát triển vào phần ba cuối của thế kỷ XIX bởi trường phái Đức (Hankel, du Bois-Raymond) và trên hết bởi người Ý; Dini và Arzelà đã làm chính xác các điều kiện cần để giới hạn của một dãy các hàm liên tục là liên tục, trong khi Ascoli đưa vào khái niệm cơ bản về liên tục đều và chứng minh định lý đặc trưng các tập hợp compact của các hàm liên tục [3] (một định lý sau này được Montel phổ biến trong lý thuyết của ông về “các họ chuẩn”, là các tập hợp tương đối compact của các hàm giải tích).

(*) Trong một công trình có niên đại 1841 nhưng lần đầu được xuất bản năm 1894 ([4a], p. 67), Weierstrass sử dụng với sự rõ ràng hoàn hảo khái niệm hội tụ đều (mà ông gọi bằng tên này lần đầu tiên) cho các chuỗi lũy thừa theo một hoặc nhiều biến phức.

Mặt khác, chính Weierstrass đã phát hiện [4b] khả năng xấp xỉ đều một hàm liên tục nhận giá trị thực theo một hoặc nhiều biến thực trên một tập hợp bị chặn bằng các đa thức. Kết quả này ngay lập tức thu hút sự quan tâm mạnh mẽ và dẫn đến nhiều nghiên cứu “định lượng” (*).

Đóng góp hiện đại cho các vấn đề này trước hết là trang bị cho chúng tính tổng quát đầy đủ mà chúng có thể đạt được, bằng cách xét các hàm mà miền xác định và miền giá trị không còn bị hạn chế vào $\mathbf{R}$ hoặc các không gian hữu hạn chiều, và do đó đặt chúng vào ngữ cảnh tự nhiên của chúng với sự trợ giúp của các khái niệm tôpô tổng quát. Đặc biệt, định lý Weierstrass, vốn đã chứng tỏ là một công cụ mạnh mẽ trong giải tích cổ điển, trong những năm gần đây đã được M. H. Stone mở rộng sang những tình huống tổng quát hơn nhiều; phát triển một ý tưởng do H. Lebesgue đưa vào (trong một chứng minh định lý Weierstrass), ông đã chỉ ra một cách rõ ràng vai trò quan trọng của các dàn hàm trong lý thuyết xấp xỉ các hàm liên tục nhận giá trị thực (xấp xỉ bằng “các đa thức dàn”, xem § 4, Mệnh đề 2 và Định lý 2), và cũng chỉ ra cách mà định lý Weierstrass tổng quát có các hệ quả ngay lập tức là một loạt các định lý xấp xỉ tương tự, do đó có thể được nhóm lại theo một cách nhất quán hơn nhiều. Chúng tôi ít nhiều đã theo cách trình bày của ông [5].

THƯ MỤC

[1] A.-L. Cauchy, Œuvres, Paris (Gauthier-Villars), 1882-1932.

[2] N. H. Abel, Œuvres, tập 1, tr. 223-224, do Sylow và Lie biên tập (Christiania) 1881.

[3] G. Ascoli, Sulle curve limiti di una varietà data di curve, Mem. Accad. Lincei (3), tập 18 (1883), tr. 521-586.

[4] K. Weierstrass, Mathematische Werke, Berlin (Mayer und Müller), 1894-1903:
    a) Zur Theorie der Potenzreihen, Bd. 1, tr. 67-74;
    b) Über die analytische Darstellbarkeit sogenannter willkürlicher Functionen reeller Argumente, Bd. 3, tr. 1-37.

[5] M. H. Stone, The generalized Weierstrass approximation theorem, Mathematics Magazine, 21 (1948), tr. 167-183 và 237-254.

[6] C. De La Vallée-Poussin, Leçons sur l'approximation des fonctions d'une variable réelle, Paris, (Gauthier-Villars), 1919.

(*) Xem, chẳng hạn, C. De La Vallée Poussin [6].

Các số tham chiếu chỉ chương, tiết diện và tiểu mục hoặc bài tập, theo thứ tự đó.

T : V, 1, 2.
$a^x$ (a là số thực bất kỳ > 0, x là số thực bất kỳ) : V, 4, 1.
$\log_a x$ (a, x là các số thực > 0, $a \neq 1$) : V, 4, 1.
$\mathbf{R}^n$ : VI, 1, 1.
$d(x, y)$ (khoảng cách Euclid) : VI, 2, 1.
$\|x\|$ (chuẩn Euclid) : VI, 2, 1.
$(x|y)$ (tích vô hướng) : VI, 2, 2.
$S_n, B_n, R_n^*$ : VI, 2, 3.
$P_n(\mathbf{R}), P_n$ : VI, 3, 1.
$\tilde{\mathbf{R}}$ : VI, 3, 3.
$\infty$ (điểm của $\tilde{\mathbf{R}}$) : VI, 3, 3.
$P_{n,p}(\mathbf{R}), P_{n,p}$ : VI, 3, 5.
$r(G), d(G)$ (G là nhóm con đóng bất kỳ của $\mathbf{R}^n$) : VII, 1, 2.
$G^*$ (G là nhóm con bất kỳ của $\mathbf{R}^n$) : VII, 1, 3.
$T^n$ : VII, 1, 4.
C, i : VIII, 1, 1.
$\Re(z), \Im(z), \overline{z}, |z|$ (z là một số phức) : VIII, 1, 1.
C*, U : VIII, 1, 3.
H : VIII, 1, 4.
$e(x)$ ($= e^{2\pi ix}$) : VIII, 2, 1.
$(\Delta_1, \Delta_2)$ ($\Delta_1, \Delta_2$ là các tia) : VIII, 2, 2.
$\partial, \omega$ : VIII, 2, 2.
Am (z) (z là một số phức) : VIII, 2, 2.
cos $\theta$, sin $\theta$, tan $\theta$ ($\theta$ là một góc) : VIII, 2, 2.
$\cos_a x, \sin_a x, \tan_a x, \cot_a x$ (x là một số thực) : VIII, 2, 4.
cos $x$, sin $x$, tan $x$, cot $x$ (x là một số thực) : VIII, 2, 4.
$(\widehat{D_1}, \widehat{D_2})$ (D_1, D_2 là các đường thẳng) : VIII, 2, 6.
$\delta_0$ : VIII, 2, 6.
C^n : VIII, 4, 1.
$P_n(C), \tilde{C}$ : VIII, 4, 3.

∞ (điểm của $\tilde{C}$) : VIII, 4, 3.
$P_{n,p}(C)$ : VIII, 4, 4.
$\beta X$ (X là một không gian hoàn toàn chính quy) : IX, 1, Bài tập 7.
$d(A, B), d(x, A)$ [x là một điểm, A, B là các tập con của một không gian mêtric trong đó khoảng cách giữa hai điểm được ký hiệu bởi $d(x, y)$] : IX, 2, 2
$|x|$ (giá trị tuyệt đối trong một vành chia có giá trị) : IX, 3, 2.
$||x||$ (chuẩn trong một không gian định chuẩn) : IX, 3, 3.
D(A) : IX, 5, Bài tập 3.
L(C) (C là một lưới) : IX, 6, 5.
$\prod_{n \in \mathbf{N}} x_n$ : IX, Phụ lục, 1.
$\prod_{n=h}^{\infty} x_n$ : IX, Phụ lục, 3.
$\prod_{n=0}^{\infty} x_n$ : IX, Phụ lục, 3.
$\mathcal{F}(X; Y), H(x)$ [H là một tập con của $\mathcal{F}(X; Y)$], $\Phi(x)$ [$\Phi$ là một lọc trên $\mathcal{F}(X; Y)$], $u|A, H|A$ [A là một tập con của X, $u \in \mathcal{F}(X; Y), H \subset \mathcal{F}(X; Y)$] : X, 1.
W(V) (V là một lân cận của Y) : X, 1, 1.
$\mathcal{F}_u(X; Y)$ : X, 1, 1.
$\mathcal{F}_{\mathcal{G}}(X; Y)$ : X, 1, 2.
W(A, V) (A $\in \mathcal{G}$, V là một lân cận của Y) : X, 1, 2.
$\mathcal{F}_s(X; Y), \mathcal{F}_c(X; Y)$ : X, 1, 3.
$\mathcal{C}(X; Y), \mathcal{C}_{\mathcal{G}}(X; Y), \mathcal{C}_s(X; Y), \mathcal{C}_c(X; Y), \mathcal{C}_u(X; Y)$ : X, 1, 6.
$\mathcal{C}_{\mathcal{G}}(X; Y)$ : X, 1, 6.
$\tilde{x}$ (x là một điểm của X) : X, 2, 1.
$\mathcal{B}_{\mathcal{G}}(X; Y), \mathcal{B}(X; Y)$ (Y là một không gian mêtric) : X, 3, 1.
$||u||$ (u là một ánh xạ bị chặn vào một không gian định chuẩn) : X, 3, 2.
$\mathcal{L}(X_1, \ldots, X_n; Y)$ ($X_1, \ldots, X_n$ và Y là các không gian định chuẩn) : X, 3, 2.
$||u||_i$ (u là một ánh xạ đa tuyến tính từ một tích của các không gian định chuẩn vào một không gian định chuẩn) : X, 3, 2.
T(K, U) (K là một tập con compact của X, U là một tập con mở của Y) : X, 3, 4.
$\mathcal{C}_{\beta}$ : X, 3, 5.
$C^{\infty}(X; \mathbf{R})$ : X, 4, Bài tập 6
$vX$ : X, 4, Bài tập 17.

Các số tham chiếu chỉ chương, tiết và tiểu mục hoặc Bài tập, theo thứ tự đó.

Hoành độ : VI, 1, 4.
Hoành độ, trục : VI, 1, 4.
Giá trị tuyệt đối : IX, 3, 2.
Giá trị tuyệt đối, không đúng : IX, 3, 2.
Giá trị tuyệt đối, $p$-adic : IX, 3, 2.
Các giá trị tuyệt đối, tương đương : IX, 3, 2.
Giá trị tuyệt đối của một số phức : VIII, 1, 1.
Tích vô hạn hội tụ tuyệt đối của các số phức : VIII, 3, 3.
Chuỗi hội tụ tuyệt đối (trong một không gian định chuẩn) : IX, 3, 6.
Chuỗi hội tụ tuyệt đối của các điểm trong $\mathbf{R}^n$ : VII, 3, 2.
Họ cộng được tuyệt đối (trong một không gian định chuẩn) : IX, 3, 6.
Mặt quạt góc nhọn : VIII, 2, 5.
Nhóm cộng của $\mathbf{R}^n$ : VI, 1, 2.
Nhóm cộng của các số thực môđun $a$ : V, 1, 2.
Tính đều cộng của $\mathbf{R}^n$ : VII, 1, 2.
Chấp nhận được : IX, 6, Bài tập 12.
Đại số, định chuẩn : IX, 3, 7.
Chuẩn đại số của một số phức : VIII, 1, 1.
Số đại số : VIII, 1, Bài tập 2.
Ánh xạ gần như mở : IX, 5, Bài tập 24.
Tập gần như mở : IX, 5, Bài tập 6.
Hàm gần tuần hoàn : X, 3, Bài tập 28.
(Giá trị) gần tuần hoàn : X, 3, Bài tập 27.
Biên độ của một số phức : VIII, 2, 2 và VIII, 2, 3.
Góc, phẳng : VIII, 2, 2.
Góc của một cặp tia : VIII, 2, 2 và VIII, 2, 3.
Góc của một mặt quạt góc : VIII, 2, 5.
Góc, vuông dương : VIII, 2, 2.

Mặt quạt góc (nhọn, vuông, tù, phẳng, lồi, tái nhập): VIII, 2, 5.
Xấp xỉ, đều: X, 4, 1.
Archimede (nhóm có thứ tự tuyến tính): V, 3, Bài tập 1.
Tiên đề Archimede: V, 2.
Đối số của một số phức: VIII, 2, 2.
Định lý Ascoli: X, 2, 5.
Nhóm con liên kết của một nhóm con của $\mathbf{R}^n$: VII, 1, 3.
Tiên đề Archimedes: V, 2.
Trục, tọa độ: VI, 1, 4.
Trục, ảo: VIII, 1, 2.
Trục hoành: VI, 1, 4.
Trục tung: VI, 1, 4.
Trục, thực: VIII, 1, 2.

Không gian Baire: IX, 5, 3.
Định lý Baire: IX, 5, 3.
Quả cầu (đóng, mở): IX, 2, 2.
Quả cầu Euclid (mở, đóng): VI, 2, 3.
Quả cầu đơn vị: VI, 2, 3, và IX, 3, 3.
Cơ sở của một hệ đo góc: VIII, 2, 3.
Cơ sở của một hệ lôgarit: V, 4, 1.
Cơ sở, chính tắc (của $\mathbf{R}^n$): VI, 1, 3.
Phân giác của một mặt quạt góc: VIII, 2, 5.
Ánh xạ Borel: IX, 6, Bài tập 16.
Ánh xạ Borel thuộc lớp $\alpha$: IX, 6, Bài tập 16.
Tập Borel: IX, 6, 3.
Tính đều của hội tụ bị chặn: X, 1, 3.
Ánh xạ bị chặn (vào một không gian mêtric): X, 3, 1.
Tập bị chặn (trong một không gian mêtric): IX, 2, 2.
Tập bị chặn trong $\mathbf{R}^n$: VI, 1, 1.
Hộp (đóng, mở): VI, 1, 1.
Đường gấp khúc: VI, 1, Bài tập 6.

Cơ sở chính tắc của $\mathbf{R}^n$: VI, 1, 3.
Tập có khả năng: IX, 6, 9.
Dung lượng: IX, 6, 9.
Phép chiếu trung tâm: VI, 2, 3.
Tâm của một quả cầu: IX, 2, 2.
Tâm của một quả cầu hoặc mặt cầu: VI, 2, 3 và IX 2, 2.
Đường tròn: VI, 2, 3.
Lớp của một ánh xạ Borel: IX, 6, Bài tập 16.
Quả cầu đóng: IX, 2, 2.
Không gian chuẩn tập thể: IX, 4, Bài tập 18.
Tôpô của hội tụ compact: X, 1, 3.

Sự hội tụ compact, tính đều của : X, 1, 3.
Tôpô compact-mở : X, 3, 4.
Phép compact hóa, Stone-Čech : IX, 1, Bài tập 7.
Tương thích (mêtric và tôpô) : IX, 2, 5.
Tương thích (mêtric và tính đều) : IX, 2, 4.
Tương thích (chuẩn và cấu trúc đại số) : IX, 3, 7.
Không gian chuẩn hoàn toàn : IX, 4, Bài tập 3.
Lọc chính quy hoàn toàn : IX, 1, Bài tập 8.
Không gian chính quy hoàn toàn : IX, 1, 5.
Không gian chính quy hoàn toàn liên kết với một không gian khả năng đều hóa : IX, 1, Bài tập 4.
Phân tách hoàn toàn (các tập đóng trong một không gian chính quy hoàn toàn) : IX, 1, Bài tập 11.
Siêu phẳng phức trong C^n : VIII, 4, 1.
Đa tạp tuyến tính phức trong C^n : VIII, 4, 1.
Các đường phức trong C^n : VIII, 4, 1.
Số phức : VIII, 1, 1.
Không gian số phức chiều n : VIII, 4, 1.
Các mặt phẳng phức trong C^n : VIII, 4, 1.
Đường xạ ảnh phức : VIII, 4, 3.
Mặt phẳng xạ ảnh phức : VIII, 4, 3.
Không gian xạ ảnh phức chiều n : VIII, 4, 3.
Liên hợp của một số phức : VIII, 1, 1.
Phân hoạch đơn vị liên tục : IX, 4, 3.
Tích vô hạn hội tụ (trong một đại số chuẩn hóa) : IX, Phụ lục, 3.
Hội tụ, thông thường : X, 3, 2.
Hội tụ, điểm : X, 1, 3.
Hội tụ, đều : X, 1, 1.
Trục tọa độ : VI, 1, 4.
Đa tạp tọa độ : VI, 1, 4.
Côsin của một góc : VIII, 2, 2.
Côsin của một số : VIII, 2, 4.
Côtang của một góc : VIII, 2, 2.
Côtang của một số : VIII, 2, 4.
Kiểu đếm được (không gian mêtric hóa được) : IX, 2, 8.
Không gian compact đếm được : IX, 2, Bài tập 14.
Bao phủ chia được : IX, 4, Bài tập 16.
Bao phủ chẵn : IX, 4, Bài tập 16.
Bao phủ điểm-hữu hạn : IX, 4, 3.
Chéo của một cặp đường : VIII, 2, 6.
Chéo phải : VIII, 2, 6.
Hình lập phương : IX, 1, 5.
Hình lập phương (mở, đóng) : VI, 1, 1.
Đường cong, Peano : VI, 1, Bài tập 2.

Bậc (đơn vị đo góc) : VIII, 2, 3.
Đường kính : IX, 2, 2.
Siêu phẳng đường kính : VI, 2, 4.
Các điểm đối nhau qua tâm của $S_n$ : VI, 3, 1.
Chiều của một nhóm con đóng của $\mathbf{R}^n$ : VII, 1, 2.
Định lý Dini : X, 4, 1.
Tỉ số hướng của một đường hoặc tia : VI, 1, 4.
Vectơ hướng của một đường hoặc tia : VI, 1, 4.
Đĩa (mở, đóng) : VI, 2, 3.
Họ rời rạc của các tập con : IX, 4, Bài tập 18.
Dịch chuyển Euclid : VI, 2, 2.
Khoảng cách giữa hai tập hợp : IX, 2, 2.
Khoảng cách Euclid : VI, 2, 1.
Khoảng cách từ một điểm đến một tập hợp : IX, 2, 2.
Bao phủ chia được : IX, 4, Bài tập 16.
Vành chia của các quaternion : VIII, 1, 4.
Vành chia định giá : IX, 3, 2.

$\varepsilon$-chu kỳ (của một hàm) : X, 3, Bài tập 28.
Tập hợp các ánh xạ liên tục đều : X, 2, 1.
Liên tục đều tại một điểm : X, 2, 1.
Liên tục đều, một cách đều : X, 2, 1.
Phân hoạch đều mod 1 : VII, 1, Bài tập 14.
Các giá trị tuyệt đối tương đương : IX, 3, 2.
Các họ giả mêtric tương đương : IX, 1, 2.
Các chuẩn tương đương : IX, 3, 3.
Các giả mêtric tương đương : IX, 1, 2.
Các giá trị bán tuyệt đối tương đương : IX, 3, Bài tập 10.
Ánh xạ cốt yếu vào $P_n$ : VI, 3, Bài tập 2.
Ánh xạ cốt yếu vào $S_1$ : VI, 2, Bài tập 6.
Quả cầu Euclid (đóng, mở) : VI, 2, 3.
Dịch chuyển Euclid : VI, 2, 2.
Khoảng cách Euclid : VI, 2, 1.
Chuẩn Euclid trong $\mathbf{R}^n$ : VI, 2, 1.
Mặt cầu Euclid : VI, 2, 3.
Bao phủ chẵn : IX, 4, Bài tập 16.
Hàm mũ : V, 4, 1.

Các thừa số của một tích (trong một đại số chuẩn hóa) : IX, Phụ lục, 1.
Họ, tổng tuyệt đối được : IX, 3, 6.
Họ các hàm phụ thuộc vào một họ các tập con : IX, 4, 3.
Chuỗi Farey : VII, 1, Bài tập 13.
Trường các số phức : VIII, 1, 1.
Lọc, chính quy hoàn toàn : IX, 1, Bài tập 8.

Lọc, cực đại chính quy hoàn toàn : IX, 1, Bài tập 8.
Tính đều của các bao phủ mở hữu hạn : IX, 4, Bài tập 17.
Góc phẳng : VIII, 2, 2.
Miền góc phẳng : VIII, 2, 5.
Hàm, gần tuần hoàn : IX, 3, Bài tập 28.
Hàm, mũ : V, 4, 1.
Hàm, tuần hoàn (được xác định trên $\mathbf{R}^n$) : VII, 1, 6.
Hàm, tuần hoàn $q$-lần : VII, 1, 6.

Sinh bởi một tập hợp các tập con ($\sigma$-đại số) : IX, 6, 3.
Grad (đơn vị đo góc) : VIII, 2, 3.
Nhóm, cộng tính (của $\mathbf{R}^n$) : VI, 1, 2.
Nhóm, cộng tính (của các số thực mod $a$) : V, 1, 2.
Nhóm, mêtric hóa được : IX, 3, 1.
Nhóm các phép dịch chuyển Euclid : VI, 2, 2.
Nhóm, một tham số : V, 3.
Nhóm, trực giao : VI, 2, 2.

Nửa đường thẳng : VI, 1, 4.
Các nửa không gian (mở, đóng) được xác định bởi một siêu phẳng : VI, 1, 4.
Giá trị bán tuyệt đối Hausdorff : IX, 3, Bài tập 9.
Giá trị bán tuyệt đối Hausdorff liên kết với một giá trị bán tuyệt đối : IX, 3, Bài tập 9.
Bán cầu (mở, đóng) : VI, 2, 4.
Hàm đồng dạng : VI, 3, 5.
Iđêan cực đại siêu thực : X, 4, Bài tập 16.
Siêu phẳng ở vô cực : VI, 3, 3.
Siêu phẳng, phức (trong $\mathbf{C}^n$) : VIII, 4, 1.
Siêu phẳng, đường kính : VI, 2, 4.
Siêu phẳng chiếu (trong một phép chiếu lập thể) : VI, 2, 4.

Trục ảo : VIII, 1, 2.
Phần ảo của một số phức : VIII, 1, 1.
Ảo, thuần túy : VIII, 1, 1.
Giá trị tuyệt đối không chính quy : IX, 3, 2.
Bất đẳng thức tam giác : VI, 2, 1, và IX, 1, 1.
Ánh xạ không cốt yếu vào $\mathbf{P}_n$ : VI, 3, Bài tập 2.
Ánh xạ không cốt yếu vào $S_1$ : VI, 2, Bài tập. 6.
Tích vô hạn : IX, Phụ lục, 3.
Mêtric bất biến : IX, 3, 1.
Ánh xạ đẳng cự : IX, 2, 2.
Phép đẳng cự : IX, 2, 2.

Dàn trong $\mathbf{R}^n$ : VII, 1, 1.
Mêtric bất biến trái : IX, 3, 1.
Giả mêtric bất biến trái : IX, 3, Bài tập 1.
Độ dài của một đoạn trong $\mathbf{R}^n$ : VI, 2, 1.
Đường, gấp khúc : VI, 1, Bài tập 6.
Đường, gấp khúc đơn : VI, 1, Bài tập 9.
Đường, xạ ảnh phức : VIII, 4, 3.
Đường, xạ ảnh thực : VI, 3, 1.
Tổ hợp tuyến tính của các hàm với các hệ số trong một không gian chuẩn : X, 4, 4.
Đa tạp tuyến tính, phức (trong $\mathbf{C}^n$) : VIII, 4, 1.
Khả năng tiếp cận tuyến tính : IX, 6, Bài tập 11.
Các đường, phức (trong $\mathbf{C}^n$) : VIII, 4, 1.
Không gian paracompact địa phương : IX, 4, Bài tập 27.
Lôgarit cơ số $a$ : V, 4, 1.
Xoắn ốc lôgarit : VIII, 3, Bài tập 5.
Không gian Lusin : IX, 6, 4.

Ánh xạ gần mở : IX, 5, Bài tập 24.
Ánh xạ Borel : IX, 6, Bài tập 16.
Ánh xạ cảm sinh bởi một sàng lọc : IX, 6, 5.
Ánh xạ vào $P_n$, cốt yếu hoặc không cốt yếu : VI, 3, Bài tập 2.
Ánh xạ vào $S_1$, cốt yếu hoặc không cốt yếu : VI, 2, Bài tập 6.
Ánh xạ đẳng cự : IX, 2, 2.
Ánh xạ tuyến tính từng phần : VI, 1, Bài tập 6.
Lọc cực đại hoàn toàn chính quy : X, 1, Bài tập 8.
Tập hợp không lớn : IX, 5, 2.
Đo của một góc : VIII, 2, 3.
Đo của một chéo : VIII, 2, 6.
Đo chính (của một góc) : VIII, 2, 3.
Đo chính (của một chéo) : VIII, 2, 6.
Không gian siêu compact : IX, 4, Bài tập 25.
Metric : IX, 2, 1.
Metric liên kết với một giả metric : IX, 2, 1.
Metric tương thích với một tôpô : IX, 2, 5.
Metric tương thích với một cấu trúc đồng nhất : IX, 2, 4.
Metric bất biến trái (phải) : IX, 3, 1.
Không gian metric : IX, 2, 1.
Nhóm tôpô mêtric hóa được : IX, 3, 1.
Không gian tôpô mêtric hóa được : IX, 2, 5.
Không gian tôpô mêtric hóa được kiểu đếm được : IX, 2, 8.
Không gian đồng nhất mêtric hóa được : IX, 2, 4.
Cấu trúc đồng nhất mêtric hóa được : IX, 2, 4.
Dãy nhân được (trong một đại số có chuẩn) : IX, Phụ lục, 1.

Định lý Nagata-Smirnov : IX, 4, Bài tập 22.
Nửa trục thực âm : VIII, 1, 2.
Không gian không lớn : IX, 5, Bài tập 7.
Chuẩn (trên một không gian vectơ) : IX, 3, 3.
Chuẩn đại số (của một số phức) : VIII, 1, 1.
Chuẩn tương thích với một cấu trúc đại số : IX, 3, 7.
Chuẩn Euclid (trong $\mathbf{R}^n$) : VI, 2, 1.
Không gian chuẩn : IX, 4, 1.
Chuỗi hội tụ thông thường : X, 3, 2.
Đại số có chuẩn : IX, 3, 7.
Không gian có chuẩn : IX, 3, 3.
Các chuẩn tương đương : IX, 3, 3.
Tập hợp không trù mật ở đâu cả : IX, 5, 1.
Số, đại số : VIII, 1. Bài tập 2.
Số phức : VIII, 1, 1.
Không gian số chiều $n$, phức : VIII, 4, 1.
Không gian số chiều $n$, thực : VI, 1, 1.

Mặt quạt góc tù : VI, 2, 5.
Các nhóm một tham số : V, 3.
Quả cầu mở : IX, 2, 2.
Các tia đối : VI, 1, 4.
Phân hoạch có thứ tự : IX, Phụ lục, Bài tập 2.
Tung độ : VI, 1, 4.
Trục của các tung độ : VI, 1, 4.
Gốc của một tia : VI, 1, 4.
Các đa tạp affine tuyến tính trực giao : VI, 2, 2.
Nhóm trực giao : VI, 2, 2.
Biến đổi trực giao : VI, 2, 2.
Các vectơ trực giao, các không gian con vectơ : VI, 2, 2.
Dao động của một hàm tại một điểm : IX, 2, 3.
Dao động của một hàm trong một tập hợp : IX, 2, 3.

Giá trị tuyệt đối $p$-adic : IX, 3, 7.
Hình hộp song song (mở, đóng) : VI, 1, 3.
Phân hoạch đơn vị, liên tục : IX, 4, 3.
Phân hoạch, có thứ tự : IX, Phụ lục, Bài tập 2.
Đường cong Peano : VI, 1, Bài tập 2.
Không gian hoàn toàn chuẩn : IX, 4, Bài tập 7.
Hàm tuần hoàn, xác định trên $\mathbf{R}^n$ : VII, 1, 6.
Các chu kỳ của một hàm tuần hoàn : VII, 1, 6.
Ánh xạ tuyến tính từng phần : VI, 1, Bài tập 6.
Nguyên lý ngăn kéo : VII, 1, Bài tập 11.
Mặt phẳng xạ ảnh phức : VIII, 4, 3.

Mặt phẳng xạ ảnh thực : VI, 3, 1.
Các mặt phẳng, phức (trong $\mathbf{C}^n$) : VIII, 4, 1.
Điểm ở vô cực : VI, 3, 3.
Phủ điểm-hữu hạn : IX, 4, 3.
Điểm hội tụ đều : X, 1, Bài tập 9.
Sự hội tụ từng điểm trong một tập con của $X$ : X, 1, 3.
Sự hội tụ từng điểm, tôpô của : X, 1, 3 và 3, 4.
Sự hội tụ từng điểm, cấu trúc đồng nhất của : X, 1, 3.
Hội tụ từng điểm (lọc) : X, 1, 3.
Không gian Polish : IX, 6, 1.
Đa thức theo các hàm thuộc một tập hợp đã cho : X, 4, 2 và 4, 4.
Đa thức lượng giác : X, 4, 4.
Nửa trục thực dương : VIII, 1, 2.
Hội tụ tiền compact, cấu trúc đồng nhất của : X, 1, 3.
Đo chính của một góc : VIII, 2, 3.
Đo chính của một chéo : VIII, 2, 6.
Hệ chính các chu kỳ của một hàm tuần hoàn $q$-bội : VII, 1, 6.
Tích, hội tụ tuyệt đối (của các số phức) : VIII, 3, 3.
Tích vô hạn : IX, Phụ lục, 3.
Tích của một dãy nhân được trong một đại số có chuẩn : IX, Phụ lục, 1.
Tích vô hướng : VI, 2, 2.
Phép chiếu trung tâm : VI, 2, 3.
Siêu phẳng của phép chiếu : VI, 2, 4.
Phép chiếu lập thể : VI, 2, 4.
Đỉnh của phép chiếu : VI, 2, 4.
Không gian xạ ảnh chiều $n$, phức : VIII, 4, 3.
Không gian xạ ảnh chiều $n$, thực : VI, 3, 1.
Thực sự tại một điểm (nhóm các toán tử) : X, 2, Bài tập 18.
Không gian giả compact : IX, 1, Bài tập 22.
Giả metric : IX, 1, 1.
Giả metric bất biến : IX, 3, Bài tập 1.
Các giả metric tương đương : IX, 1, 2.
Thuần ảo (số phức) : VIII, 1, 1.

Hàm tuần hoàn $q$-bội trên $\mathbf{R}^n$ : VII, 1, 6.
Mặt bậc hai (trong $\mathbf{P}_n$) : VI, 3, Bài tập 10.
Mặt bậc hai (trong $\mathbf{R}^n$) : VI, 2, Bài tập 10.
Nón bậc hai (trong $\mathbf{P}_n$) : VI, 3, Bài tập 11.
Nón bậc hai (trong $\mathbf{R}^n$) : VI, 2, Bài tập 11.
Quaternion : VIII, 1, 4.

Radian, độ đo : VIII, 2, 3.
Bán kính của một quả cầu : IX, 2, 2.
Bán kính của một quả cầu hoặc mặt cầu : VI, 2, 3 và IX, 2, 2.

Hạng hữu tỉ của một nhóm con của $\mathbf{R}^n$ : VII, 1.
Tỉ số, hướng : VI, 1, 4.
Tia (đóng, mở) : VI, 1, 4.
Các tia, đối : VI, 1, 4.
Trục thực : VIII, 1, 2.
Không gian thực compact : X, 4, Bài tập 17.
Compact hóa thực của một không gian : X, 4, Bài tập 17.
Đa tạp tuyến tính thực (trong $\mathbf{C}^n$) : VIII, 4, 1.
Iđêan cực đại thực : X, 4, Bài tập 16.
Không gian số thực có $n$ chiều : VI, 1, 1.
Phần thực của một số phức : VIII, 1, 1.
Đường xạ ảnh thực : VI, 3, 1.
Mặt phẳng xạ ảnh thực : VI, 3, 1.
Không gian xạ ảnh thực có $n$ chiều : VI, 3, 1.
Định giá thực của một vành chia : IX, 3, 2.
Hình chữ nhật (mở, đóng) : VI, 1, 1.
Mặt quạt góc lõm : VIII, 2, 5.
Góc vuông, dương : VIII, 2, 2.
Mặt quạt góc vuông : VIII, 2, 5.
Chéo vuông : VIII, 2, 6.
Metric bất biến phải : IX, 3, 1.
Giả metric bất biến phải : IX, 3, Bài tập 1.

$\sigma$-đại số : IX, 6, 3.
Múi góc nổi bật : VIII, 2, 5.
Họ nửa mêtric bão hòa : IX, 1, 2.
Tập bão hòa các tập con : X, 1, Bài tập 5.
Tích vô hướng : VI, 2, 2.
Múi góc, góc : VIII, 2, 5.
Đoạn (đóng, mở, mở tại $x$ và đóng tại $y$) : VI, 1, 4.
Đoạn, độ dài của : VI, 2, 1.
Nửa giá trị tuyệt đối : IX, 3, Bài tập 9.
Nửa giá trị tuyệt đối Hausdorff : IX, 3, Bài tập 9.
Các nửa giá trị tuyệt đối, tương đương : IX, 3, Bài tập 10.
Nửa trục, thực âm : VIII, 1, 2.
Nửa trục, thực dương : VIII, 1, 2.
Nửa đường tròn (mở, đóng) : VI, 2, 4.
Không gian mêtric tách được : IX, 2, 8.
Tập các hàm phân tách : X, 4, 1.
Sự phân tách các điểm của một tập bởi một tập các hàm : X, 4, 1.
Dãy, nhân được : IX, Phụ lục, 1.
Chuỗi hội tụ tuyệt đối (của các điểm của $\mathbf{R}^n$) : VII, 3, 2.
Chuỗi Farey : VII, 1, Bài tập 13.
Tập, gần mở : IX, 5, Bài tập 6.

Tập, Borel : IX, 6, 3.
Tập, bị chặn : IX, 2, 2.
Tập, bị chặn (trong $\mathbf{R}^n$) : VI, 1, 1.
Tập, có thể dung lượng hóa : IX, 6, 9.
Tập, thưa : IX, 5, 2.
Tập, không đâu trù mật : IX, 5, 1.
Tập, Souslin : IX, 6, 2.
Tập, hình sao (trong $\mathbf{R}^n$) : VI, 2, Bài tập 12.
Tập, mỏng : IX, 5, Bài tập 2.
Vỏ của một tập hình sao : VI, 2, Bài tập 12.
Mặt của một hình lập phương : VI, 1, 1.
Các cạnh của một đường gấp khúc : VI, 1, Bài tập 6.
Sàng : IX, 6, 5.
Sự sàng lọc : IX, 6, 5.
Sự sàng lọc, ánh xạ cảm sinh bởi : IX, 6, 5.
Đường gấp khúc đơn : VI, 1, Bài tập 9.
Sin của một góc : VIII, 2, 2.
Sin của một số : VIII, 2, 4.
Lát cắt (trong một tập hợp có thứ tự tuyến tính) : IX, Phụ lục, Bài tập 2.
Hệ số góc của một đường thẳng : VIII, 2, 6.
Tập Souslin : IX, 6, 2.
Không gian Souslin : IX, 6, 2.
Không gian liên kết với một sự sàng lọc : IX, 6, 5.
Không gian Baire : IX, 5, 3.
Không gian chuẩn tập thể : IX, 4, Bài tập 18.
Không gian chuẩn hoàn toàn : IX, 4, Bài tập 3.
Không gian chính quy hoàn toàn : IX, 1, 5.
Không gian số phức : VIII, 4, 1.
Không gian xạ ảnh phức : VIII, 4, 3.
Không gian compact đếm được : IX, 2, Bài tập 14.
Không gian paracompact địa phương : IX, 4, Bài tập 27.
Không gian Lusin : IX, 6, 4.
Không gian metacompact : IX, 4, Bài tập 25.
Không gian mêtric : IX, 2, 1.
Không gian mêtric được kiểu đếm được : IX, 2, 8.
Không gian tôpô mêtric được : IX, 2, 5.
Không gian đều mêtric được : IX, 2, 4.
Không gian không thưa : IX, 5, Bài tập 7.
Không gian chuẩn : IX, 4, 1.
Không gian chuẩn tắc : IX, 3, 3.
Không gian các vòng : X, 3, 4.
Không gian các đường đi : X, 3, 4.
Không gian các đa tạp tuyến tính xạ ảnh chiều $p$ trong không gian xạ ảnh phức chiều $n$ : VIII, 4, 3.

Không gian các đa tạp tuyến tính xạ ảnh chiều $p$ trong không gian xạ ảnh thực chiều $n$: VI, 3, 5.
Không gian chuẩn hoàn hảo : IX, 4, Bài tập 7.
Không gian Polish : IX, 6, 1.
Không gian giả compact : XI, 1, Bài tập 21.
Không gian compact thực : X, 4, Bài tập 17.
Không gian số thực : VI, 1, 1.
Không gian xạ ảnh thực : VI, 3, 1.
Không gian mêtric tách được : IX, 2, 8.
Không gian Souslin : IX, 6, 2.
Không gian không chiều mạnh : IX, 6, Bài tập 1.
Không gian dưới mêtric : IX, 2, Bài tập 23.
Không gian hoàn toàn không thưa : IX, 5, Bài tập 12.
Không gian siêu mêtric : IX, 2, Bài tập 4.
Không gian không chiều : IX, 6, 4.
Mặt cầu : IX, 2, 2, VI, 2, 3.
Đường xoắn ốc, logarit : VIII, 3, Bài tập 5.
Hình vuông (đóng, mở) : VI, 1, 1.
Tập hình sao trong $\mathbf{R}^n$ : VI, 2, Bài tập 12.
Phép chiếu lập thể : VI, 2, 4.
Compact hóa Stone-Čech : IX, 1, Bài tập 7.
Định lý Stone : X, 4, 1.
Định lý Stone-Weierstrass : X, 4, 2.
Sàng lọc ngặt : IX, 6, 5.
Không gian không chiều mạnh : IX, 6, Bài tập 1.
Nhóm con liên kết : VII, 1, 3.
Không gian dưới mêtric : IX, 2, Bài tập 23.
Phụ thuộc vào một họ các tập con (họ các hàm) : IX, 4, 3.
Giá đỡ của một hàm : IX, 4, 3.

Tang của một góc : VIII, 2, 2.
Tang của một đường chéo : VIII, 2, 6.
Tang của một số : VIII, 2, 4.
Định lý Ascoli : X, 2, 5.
Định lý Baire : IX, 5, 3.
Định lý Dini : X, 4, 1.
Định lý của R. Ellis : X, 3, Bài tập 25.
Định lý Nagata-Smirnov : IX, 4, Bài tập 22.
Định lý Stone : X, 4, 1.
Định lý Stone-Weierstrass : X, 4, 2.
Các định lý Urysohn : IX, 4, 1 và 4, 2.
Tập mỏng : IX, 5, Bài tập 2.
Tôpô compact-mở : X, 3, 4.
Tôpô hội tụ compact : X, 1, 3 và 3, 4.

Tôpô hội tụ điểm : X, 1, 3.
Tôpô hội tụ điểm trong một tập con của X : X, 1, 3.
Tôpô hội tụ S : X, 1, 2.
Tôpô hội tụ đều : X, 1, 1.
Tôpô hội tụ đều trong một tập con của X : X, 1, 3.
Xuyến, một chiều : V, 1, 2.
Xuyến, $n$-chiều : VII, 1, 4.
Xuyến tròn xoay : VII, 1, Bài tập 15.
Không gian hoàn toàn không thưa : IX, 5, Bài tập 12.
Phép biến đổi trực giao : VI, 2, 2.
Bất đẳng thức tam giác : IX, 1, 1.
Bất đẳng thức tam giác : VI, 2, 1.
Dạng lượng giác của một số phức : VIII, 2, 2.
Các đa thức lượng giác theo $m$ biến : X, 4, 4.

Không gian ultrametric : IX, 2, Bài tập 4.
Xấp xỉ đều một hàm thực liên tục bằng các hàm liên tục thuộc một tập hợp đã cho : X, 4, 1.
Hội tụ đều trong một tập con của X : X, 1, 3.
Hội tụ đều trong các tập hợp của S : X, 1, 2.
Điểm hội tụ đều : X, 1, Bài tập 9.
Tôpô của hội tụ đều : X, 1, 1.
Tính đều của hội tụ đều : X, 1, 1.
Tính đều, cộng tính (của R^n) : VI, 1, 2.
Tính đều của hội tụ bị chặn : X, 1, 3.
Tính đều của hội tụ compact : X, 1, 3.
Tính đều xác định bởi một họ giả metric : IX, 1, 2.
Tính đều xác định bởi một giả metric : IX, 1, 2.
Tính đều của các phủ mở hữu hạn : IX, 4, Bài tập 17.
Tính đều của hội tụ từng điểm : X, 1, 3.
Tính đều của hội tụ từng điểm trong một tập con của X : X, 1, 3.
Tính đều của hội tụ tiền compact : X, 1, 3.
Tính đều của hội tụ S : X, 1, 2.
Tính đều của hội tụ đều : X, 1, 1.
Tính đều của hội tụ đều trong một tập con của X : X, 1, 3.
Tính đều của hội tụ đều trong các tập hợp của S : X, 1, 2.
Tính đều, phổ quát : IX, 1, Bài tập 5.
Hội tụ đều (lọc) : X, 1, 1.
Hội tụ đều trong mọi tập hợp của S (họ ánh xạ, lọc, dãy, chuỗi) : X, 1, 2.
Họ ánh xạ liên tục đều : X, 2, 1.
Họ khả tổng đều : X, 1, 2.
Quả cầu đơn vị, mặt cầu : VI, 2, 3 và IX, 3, 3.
Đơn vị đo góc : VIII, 2, 3.

Tính đều phổ quát : IX, 1, Bài tập 5.
Các định lý Urysohn : IX, 4, 1 và 4, 2.

Định giá, thực : IX, 3, 2.
Giá trị, tuyệt đối : IX, 3, 2.
Giá trị, tuyệt đối (của một số phức) : VIII, 1, 1.
Giá trị, bán tuyệt đối : IX, 3, Bài tập 9.
Vành chia có giá trị : IX, 3, 2.
Đa tạp, tọa độ : VI, 1, 4.
Vectơ, hướng (của một đường thẳng hoặc tia) : VI, 1, 4.
Các không gian vectơ con trực giao : VI, 2, 2.
Các vectơ trực giao : VI, 2, 2.
Đỉnh của một phép chiếu lập thể : VI, 2, 4.

Định lý Weierstrass-Stone : X, 4, 2.

Không gian không chiều : IX, 6, 4

In ấn: Mercedesdruck, Berlin
Đóng bìa: Buchbinderei Lüderitz & Bauer, Berlin

THƯ VIỆN ĐẠI HỌC ST. FRANCIS XAVIER
3 1993 02600023 1

N. Bourbaki, Các yếu tố của Toán học,
Tôpô đại cương, Các chương 5-10

Đây là bản tái bản bìa mềm của bản dịch tiếng Anh năm 1966 (có sẵn từ Springer từ năm 1989) của các chương sau của “Topologie générale” của Bourbaki.

Nó hoàn thành việc nghiên cứu tôpô đại cương đã bắt đầu trong Phần I (Các chương 1–4, cũng có bản tiếng Anh bìa mềm).

Sau khi các số thực được đưa vào trong Chương 4, các chương đầu tiên của tập này nghiên cứu các nhóm con và các thương của $\mathbf{R}$ (với các áp dụng vào “phép đo các đại lượng” và các hàm log và exp), rồi các không gian vectơ thực và các không gian xạ ảnh, rồi các nhóm cộng tính $\mathbf{R}^n$ (các nhóm con, các thương, các đồng cấu, các tổng và tích vô hạn). Các tính chất tương tự sau đó được nghiên cứu đối với các số phức, trong Chương 8. Chương 9 minh họa việc sử dụng các số thực trong tôpô đại cương, nghiên cứu các loại không gian tôpô quan trọng khác nhau: các không gian khả đều, metric, chuẩn Baire, Polish, Borel. Chương cuối cùng đề cập đến các tôpô khác nhau của các không gian hàm, kết thúc bằng một tiết diện về xấp xỉ các hàm.
