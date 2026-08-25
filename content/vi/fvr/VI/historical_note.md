---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: fvr-i-vii
pdf_pages: 0314-0318
extraction: ocr
statements: 0
exercises: 0
content_sha256: 07b7287d271ac6ce82bcbdc5aa9fc8cda8cb631a8ccacee2346a0433e9ecebfa
translated_from: content/en/fvr/VI/historical_note.md
source_content_sha256: f46444e85c3eb79a4d7395b05440c907d0dc354d8369c5239ce60b393fc50854
translation_model: gpt-5.4
translation_run: translate-vi-aed4adad
glossary_version: 34
glossary_terms_sha256: ca7cbad99ba801b4a12e4ecf2f34ac6efde80235c05c8fea0143f77dc09f6793
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Chương V và VI)

(Chú ý. Chữ số La Mã chỉ thư mục được đặt ở cuối ghi chú này.)

Sự phân biệt giữa các “vô cùng bé” (hay “vô cùng lớn”) thuộc các cấp khác nhau đã xuất hiện ngầm ẩn trong những trước tác đầu tiên về phép tính vi phân, chẳng hạn trong các trước tác của Fermat; nó được phát biểu đầy đủ với Newton và Leibniz, cùng với lý thuyết về các “hiệu sai cấp cao hơn”; và người ta đã nhanh chóng nhận thấy rằng trong những trường hợp đơn giản nhất, giới hạn (hay “giá trị thực”) của một biểu thức dạng $f(x)/g(x)$ tại một điểm mà $f$ và $g$ đều tiến tới 0 được cho bởi khai triển Taylor của các hàm ấy trên một lân cận của điểm đang xét (“quy tắc l’Hôpital”, có lẽ là của Johann Bernoulli).

Ngoài trường hợp sơ cấp, bài toán chính của việc “đánh giá tiệm cận” đặt ra cho các nhà toán học từ cuối thế kỷ XVII$^{th}$ là việc tính, khớp hoặc gần đúng, các tổng dạng $\sum_{k=1}^n f(k)$ khi $n$ rất lớn; một phép tính như vậy thực sự cần thiết không những cho nội suy và cho việc tính gần đúng bằng số tổng của một chuỗi, mà còn trong phép tính xác suất, nơi các “hàm của những số lớn” như $n!$ hay $\binom{a}{n}$ giữ một vai trò nổi trội. Ngay từ Newton, để thu được các giá trị gần đúng của $\sum_{k=1}^n \frac{1}{a+k}$ khi $n$ lớn, đã chỉ ra một phương pháp mà (trong trường hợp riêng này) quy về việc tính các số hạng đầu tiên trong công thức Euler-Maclaurin (I). Về cuối thế kỷ, Jakob Bernoulli, trong quá trình nghiên cứu của ông về phép tính xác suất, đã tự đặt cho mình việc xác định các tổng $S_k(n) = \sum_{p=1}^{n-1} p^k$, là những đa thức theo $n$ mà ông đã phát hiện ra luật tổng quát để thành lập chúng (không đưa ra chứng minh) $^4$, do đó lần đầu tiên đưa vào, trong biểu thức của các hệ số của các đa thức ấy, những số mang tên ông, và quan hệ quy nạp cho phép tính chúng ((II), p. 97). Năm 1730, Stirling đã thu được một khai triển tiệm cận của $\sum_{k=1}^n \log(x+ka)$, khi $n$ tăng vô hạn, bằng một thủ tục tính các hệ số theo cách đệ quy.

$^4$ Chúng là các nguyên hàm của các “đa thức Bernoulli” $B_k(x)$.

Các công trình có tính chất quyết định của Euler về chuỗi và về các vấn đề liên quan có niên đại từ 1730 đến 1745. Đặt $S(n) = \sum_{k=1}^{n} f(k)$, ông áp dụng công thức Taylor cho hàm $S(n)$, điều này cho ông

$$
f(n) = S(n) - S(n-1) = \frac{dS}{dn} - \frac{1}{2!} \frac{d^2 S}{dn^2} + \frac{1}{3!} \frac{d^3 S}{dn^3} - \cdots,
$$

một phương trình mà ông đã “đảo” bằng phương pháp hệ số bất định, tìm một nghiệm có dạng

$$
S(n) = \alpha \int f(n)\, dn + \beta\, f(n) + \gamma \frac{df}{dn} + \delta \frac{d^2 f}{dn^2} + \cdots;
$$

do đó ông thu được, từng số hạng một,

$$
S(n) = \int f(n)\, dn + \frac{f(n)}{2} + \frac{1}{12} \frac{df}{dn} - \frac{1}{720} \frac{d^3 f}{dn^3} + \frac{1}{30\,240} \frac{d^5 f}{dn^5} - \cdots
$$

mà lúc đầu chưa thể xác định được luật thành lập của các hệ số (III $a$ và $d$). Nhưng vào khoảng năm 1735, theo phép loại suy với phân tích của một đa thức thành các nhân tử tuyến tính, ông đã không ngần ngại viết công thức

$$
1 - \frac{\sin s}{\sin \alpha} = \left(1 - \frac{s}{\alpha}\right) \left(1 - \frac{s}{\pi - \alpha}\right)
$$
$$
\left(1 - \frac{s}{-\pi - \alpha}\right) \left(1 - \frac{s}{2\pi - \alpha}\right) \left(1 - \frac{s}{-2\pi - \alpha}\right) \cdots
$$

và khi đồng nhất các hệ số trong các khai triển của hai vế thành các chuỗi nguyên ông đặc biệt thu được (với $\alpha = \pi / 2$) các biểu thức nổi tiếng cho chuỗi $\sum_{k=1}^{\infty} \frac{1}{n^{2k}}$

theo lũy thừa của $\pi$ (III $b$) $^5$. Vài năm sau, cuối cùng ông nhận thấy rằng các hệ số của các lũy thừa ấy của $\pi$ được cho bởi các phương trình giống như các phương trình của công thức tổng của ông, và nhận ra mối liên hệ của chúng với các số do Bernoulli đưa vào, cũng như với các hệ số của khai triển chuỗi của $z/(e^z - 1)$ (III $g$).

Một cách độc lập với Euler, Maclaurin đã đi đến cùng công thức tổng ấy vào khoảng cùng thời gian, bằng một con đường ít mạo hiểm hơn đôi chút, gần với con đường mà chúng tôi đã theo trong bản văn; thực vậy ông đã lặp công thức “Taylor” biểu diễn $f(x)$ theo các hiệu $f^{(2k+1)}(x+1) - f^{(2k+1)}(x)$, một công thức mà ông thu được bằng cách “đảo ngược” các khai triển Taylor của các hiệu này bằng phương pháp các

$^5$ Năm 1743 Euler, để đáp lại nhiều nhà phê bình đương thời, đã đưa ra một phép dẫn xuất có phần hợp lý hơn của các “khai triển Euler” của các hàm lượng giác; chẳng hạn, khai triển của $\sin x$ thành một tích vô hạn được dẫn xuất từ biểu thức $\sin x = \frac{1}{2i}(e^{ix} - e^{-ix})$ và sự kiện rằng $e^{ix}$ là giới hạn của đa thức $\left(1 + \frac{ix}{n}\right)^n$ (III $e$).

hệ số bất định (IV); nhưng ông đã không nhận ra luật hình thành của các hệ số, do Euler phát hiện.

Nhưng Maclaurin, cũng như Euler và tất cả các nhà toán học cùng thời ông, đã trình bày tất cả các công thức này dưới dạng khai triển thành chuỗi, mà sự hội tụ của chúng thậm chí còn không được nghiên cứu. Không phải là khái niệm chuỗi hội tụ đã hoàn toàn bị bỏ quên trong thời kỳ này; từ Jakob Bernoulli người ta đã biết rằng chuỗi điều hòa là phân kỳ, và Euler thậm chí còn làm sáng tỏ kết quả này bằng cách tính tổng của $n$ số hạng đầu tiên của chuỗi ấy với sự giúp đỡ của công thức tính tổng của ông (III c and d); cũng chính Euler đã nhận xét rằng tỉ số của hai số Bernoulli liên tiếp tăng vô hạn, và do đó một chuỗi nguyên có các số này làm hệ số thì không thể hội tụ ((III f), p. 357) $^6$. Nhưng khuynh hướng hướng tới phép tính hình thức thì mạnh hơn, và trực giác phi thường của Euler, ngay cả như vậy, cũng không ngăn ông sa vào điều phi lý, chẳng hạn khi ông viết $0 = \sum_{n=-\infty}^{+\infty} x^n$ ((III f), p. 362) $^7$.

Ta đã thấy rồi (Ghi chú lịch sử cho chap. IV) các nhà toán học vào đầu thế kỷ XIX$^{th}$, mệt mỏi vì chủ nghĩa hình thức không kiềm chế và không có cơ sở này, đã đưa Giải tích trở lại con đường nghiêm ngặt như thế nào. Một khi khái niệm chuỗi hội tụ đã được làm cho chính xác, nhu cầu về các tiêu chuẩn đơn giản để chứng minh sự hội tụ của các tích phân và các chuỗi bằng cách so sánh với những tích phân hay chuỗi đã biết đã xuất hiện; Cauchy đã đưa ra một số tiêu chuẩn như thế trong Analyse algébrique của ông (Va), còn Abel, trong một hồi ký được xuất bản sau khi mất (VI), đã thu được các tiêu chuẩn hội tụ lôgarit. Mặt khác, Cauchy (V b) đã làm sáng tỏ nghịch lý của những chuỗi như chuỗi Stirling, thu được bằng cách áp dụng công thức Euler-Maclaurin (và thường được gọi là “chuỗi nửa hội tụ”): ông đã chỉ ra rằng nếu (theo nhận xét của Euler về các số Bernoulli) số hạng tổng quát $u_k(n)$ của một chuỗi như thế, với một giá trị cố định của $n$, tăng vô hạn theo $k$, thì tuy vậy với một giá trị cố định của $k$ tổng riêng $s_k(n) = \sum_{h=1}^k u_h(n)$ vẫn cho một khai triển tiệm cận (khi $n$ tiến tới $+\infty$) của hàm được chuỗi “biểu diễn”, càng chính xác hơn tương ứng khi $k$ lớn hơn.

Trong phần lớn các phép tính của Giải tích Cổ điển, có thể thu được một luật hình thành tổng quát cho các khai triển tiệm cận của một hàm có một số số hạng lớn tùy ý; sự kiện này đã góp phần tạo ra một sự lẫn lộn kéo dài (ít nhất là trong ngôn ngữ) giữa chuỗi và khai triển tiệm cận; đến mức H. Poincaré, khi ông bỏ công, vào năm 1886 (VIII), hệ thống hóa các quy tắc sơ cấp của các khai triển tiệm cận (theo các lũy thừa số nguyên của $1/x$ trên một lân cận của $+\infty$), vẫn còn dùng từ vựng của lý thuyết chuỗi. Chỉ đến khi xuất hiện các khai triển tiệm cận phát sinh từ lý thuyết số giải tích thì một

$^6$ Vì chuỗi mà Euler xét ở đây được đưa vào nhằm phục vụ việc tính toán số, ông chỉ lấy tổng của các số hạng bắt đầu giảm và, từ chỉ số mà tại đó các số hạng bắt đầu tăng, ông thay chúng bằng một số dư mà ông không chỉ ra nguồn gốc (số dư trong công thức Euler-Maclaurin ở dạng tổng quát của nó mãi đến Cauchy mới xuất hiện).
$^7$ Thật trớ trêu là công thức này lại theo sau, chỉ một trang sau, một đoạn văn trong đó Euler đã cảnh báo chống lại việc sử dụng không suy xét các chuỗi phân kỳ!

Sự phân biệt giữa khái niệm khai triển tiệm cận và chuỗi đã được xác lập, do thực tế rằng, trong phần lớn các bài toán mà lý thuyết xét tới, người ta không thể thu được một cách tường minh nhiều hơn một số rất ít số hạng (thường chỉ một) của khai triển cần tìm.

Các bài toán ấy cũng đã làm cho các nhà toán học quen thuộc với việc sử dụng những thang so sánh khác với các thang gồm các lũy thừa (thực hoặc nguyên) của biến. Khái niệm này trước hết là do các công trình của P. du Bois-Reymond (VII), người đầu tiên đã xử lý một cách hệ thống việc so sánh các hàm trong một lân cận của một điểm, và, trong một số rất ít công trình, đã nhận ra tính chất “phi-Archimede” của các thang so sánh, đồng thời ông nghiên cứu một cách tổng quát các quan hệ so sánh đối với phép lấy tích phân và phép vi phân, và suy ra hàng loạt hệ quả lý thú (VII b). Các công trình ấy đôi khi thiếu sáng sủa và chặt chẽ, và chính G.H. Hardy (IX) là người đã trình bày các kết quả của du Bois-Reymond: đóng góp chính của ông là ở chỗ nhận ra và chứng minh sự tồn tại của một tập hợp các “hàm sơ cấp”, những hàm mà trên đó các phép toán thông thường của Giải tích (đặc biệt là phép vi phân) áp dụng được cho các quan hệ so sánh $^8$.

———
không thuộc phạm vi của chúng tôi trong các chương này triển khai những phương pháp cho phép thu được các khai triển tiệm cận của các hàm thuộc những loại riêng biệt nào đó, chẳng hạn một số kiểu tích phân phụ thuộc vào một tham số, vốn xuất hiện khá thường xuyên trong giải tích; về điểm này (và đặc biệt về các phương pháp quan trọng của Laplace và Darboux), độc giả có thể tham khảo cuốn sách của Hardy (IX) đã được nhắc đến, cuốn sách này chứa một thư mục rất đầy đủ.

(I) I. NEWTON, trong St. P. RIGAUD, Sự tương ứng của những người làm khoa học, Oxford, 1841, t. II, p. 309-310.
(II) Jakob Bernoulli, Ars conjectandi, Bâle, 1713.
(III) L. EULER, Opera omnia (1), t. XIV; Commentationes analyticae . . . , Leipzig-Berlin (Teubner), 1924: a) Methodus generalis summandi progressiones, p. 42-72 (=Comm. Acad. petrop , t. VI (1732-33)); b) De summis serierum reciprocarum, p. 73-86 (=Comm. Acad. petrop., t. VII (1734-35)); c) De progressionibus harmonicis observationes, p. 87-100 (ibid.); d) Inventio summae cujusque seriei . . . , p. 108-123 (=Comm. Acad. petrop., t. VIII (1736)); e) De summis serierum reciprocarum . . . dissertatio altera . . . , p. 138-155 (=Misc. Berol., t. VII (1743)); f) Consideratio progressionis . . . , p. 350-363 (=Comm. Acad. petrop., t. XI (1739)); g) De seriebus quibusdam considerationes, p. 407-462 (=Comm. Acad. petrop., t. XII (1740)).
(IV) C. MACLAURIN, Một chuyên luận đầy đủ về fluxions, Edinburgh, 1742.
(V) A. L. CAUCHY: a) Cours d’Analyse de l’Ecole Royale Polytechnique, 1re partie, 1821 (=Œuvres, (2), t. III, Paris (Gauthier-Villars), 1897; b) Œuvres, (1), t. VIII, p. 18-25, Paris (Gauthier-Villars), 1893.
(VI) N. H. ABEL, Œuvres, t. II, p. 197-205, éd. Sylow and Lie, Christiania, 1881.
(VII) P. DU BOIS-REYMOND: a) Sur la grandeur relative des infinis des fonctions, Ann. di Mat. (2), t. IV (1871), p. 338-353; b) Ueber asymptotische Werthe, infinitäre Approximationen und infinitäre Auflösung von Gleichungen, Math. Ann., t. VIII (1875), p. 362-414.
(VIII) H. POINCARÉ, Sur les intégrales irrégulières des équations linéaires, Acta Math., t. VIII (1886), p. 295-344.
(IX) G. H. HARDY, Orders of infinity, Cambridge tracts, n° 12, 2nd ed., Cambridge University Press, 1924.
