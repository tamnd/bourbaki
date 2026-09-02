---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ELEMENTS OF THE HISTORY OF MATHEMATICS
section: 18
section_title: Asymptotic Expansions
lang: vi
source: hist
pdf_pages: 0201-0204
extraction: ocr
statements: 0
exercises: 0
content_sha256: 22d1b9da09fafa957fdff8f0c105d6cc22dc0c61299a79988abbf95491305bb4
translated_from: content/en/hist/1/18_s18_asymptotic_expansions.md
source_content_sha256: 9e0ecd11eb4436e4794e19710da53ec78deea64cf184c8d01618eac0fec088a7
translation_model: gpt-5.4
translation_run: translate-vi-97bc3f4f
glossary_version: 34
glossary_terms_sha256: 4b02dedbfa59668957ad1c8662e0f4e9ed15f56f7221a015fc4965b97d0f6685
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 18. KHAI TRIỂN TIỆM CẬN.

Sự phân biệt giữa các đại lượng "vô cùng bé" (hoặc "vô cùng lớn") thuộc các cấp khác nhau xuất hiện một cách hàm ẩn ngay từ những trước tác đầu tiên về phép tính vi phân, chẳng hạn trong các trước tác của Fermat; nó trở nên hoàn toàn có ý thức với Newton và Leibniz, cùng với lý thuyết về các "sai phân cấp cao hơn"; và người ta sớm nhận thấy rằng, trong những trường hợp đơn giản nhất, giới hạn (hay "giá trị thực") của một biểu thức dạng $f(x)/g(x)$ tại một điểm mà $f$ và $g$ đều tiến tới 0, được cho bởi khai triển Taylor của các hàm ấy trong một lân cận của điểm đang xét ("quy tắc l'Hôpital", có lẽ là do Johann Bernoulli).

Ngoài trường hợp sơ cấp này, bài toán chính về "khai triển tiệm cận" đặt ra cho các nhà toán học ngay từ cuối thế kỷ XVII là việc tính toán, chính xác hoặc gần đúng, các tổng dạng $\sum_{k=1}^n f(k)$ khi $n$ rất lớn; thực vậy, một phép tính như thế là cần thiết không chỉ cho phép nội suy và việc tính gần đúng tổng của một chuỗi, mà còn trong phép tính xác suất, ở đó những "hàm của số lớn" như $n!$ hoặc $\binom{a}{n}$ giữ một vai trò trội hẳn. Ngay Newton, để thu được các giá trị gần đúng của $\sum_{k=1}^n \frac{1}{a+k}$ khi $n$ lớn, đã chỉ ra một phương pháp quy về (trong trường hợp riêng này) việc tính các số hạng đầu của công thức Euler-Maclaurin ([262], v. II, pp. 309-310). Về cuối thế kỷ, Jakob Bernoulli, trong quá trình nghiên cứu của ông về phép tính xác suất, đề nghị xác định các tổng $S_k(n) = \sum_{p=1}^n p^k$, là các đa thức$^1$ theo $n$ mà ông khám phá ra luật thành lập tổng quát (mà không đưa ra chứng minh), do đó lần đầu tiên đưa vào, trong biểu thức của các hệ số của các đa thức ấy, những số mang tên ông, cùng với quan hệ truy hồi cho phép tính chúng ([19 b], p. 97). Năm 1730, Stirling thu được một khai triển tiệm cận cho $\sum_{k=1}^n \log(x + ka)$, khi $n$ tăng vô hạn, bằng một thủ tục tính các hệ số bằng phép truy hồi.

Giai đoạn từ 1730 đến 1745 gắn với công trình có tính quyết định của Euler về các chuỗi và những vấn đề liên quan. Đặt $S(n) = \sum_{k=1}^n f(k)$, ông áp dụng công thức Taylor cho hàm $S(n)$, điều này cho ông

$$
f(n) = S(n) - S(n-1) = \frac{dS}{dn} - \frac{1}{2!} \frac{d^2 S}{dn^2} + \frac{1}{3!} \frac{d^3 S}{dn^3} - \ldots,
$$

$^1$ Chúng là các nguyên hàm của các "đa thức Bernoulli" $B_k(x)$.

một phương trình mà ông "nghịch đảo" bằng phương pháp hệ số bất định, trong khi tìm một nghiệm dạng

$$
S(n) = \alpha \int f(n) dn + \beta f(n) + \gamma \frac{df}{dn} + \delta \frac{d^2 f}{dn^2} + \ldots;
$$

do đó ông lần lượt thu được

$$
S(n) = \int f(n) dn + \frac{f(n)}{2} + \frac{1}{12} \frac{df}{dn} - \frac{1}{720} \frac{d^3 f}{dn^3} + \frac{1}{30,240} \frac{d^5 f}{dn^5} - \cdots
$$

mà lúc đầu chưa thể xác định được luật thành lập của các hệ số ([108 a], (1), v. XIV, pp. 42-72 and 108-123). Nhưng vào khoảng năm 1735, bằng phép tương tự với việc phân tích một đa thức thành các nhân tử bậc một, ông không ngần ngại viết công thức

$$
1 - \frac{\sin s}{\sin \alpha} =
\left(1 - \frac{s}{\alpha}\right) \left(1 - \frac{s}{\pi - \alpha}\right) \left(1 - \frac{s}{-\pi - \alpha}\right) \left(1 - \frac{s}{2\pi + \alpha}\right) \left(1 - \frac{s}{-2\pi + \alpha}\right) \cdots
$$

và khi đặt các hệ số của các khai triển của hai vế của toàn chuỗi bằng nhau, ông đặc biệt thu được (với $\alpha = \frac{\pi}{2}$) những biểu thức nổi tiếng cho chuỗi $\sum_{n=1}^{\infty} \frac{1}{n^{2k}}$ nhờ các lũy thừa$^2$ của $\pi$ (loc. cit., pp. 73-86). Vài năm sau, cuối cùng ông nhận ra rằng các hệ số của những lũy thừa ấy của $\pi$ được cho bởi cùng những phương trình như các hệ số trong công thức tổng của ông, và nhận ra mối liên hệ của chúng với các số do Bernoulli đưa vào, cũng như với các hệ số của khai triển thành chuỗi của $z/(e^z - 1)$ (loc. cit., pp. 407-462).

Độc lập với Euler, Maclaurin cũng đã đi tới vào khoảng cùng thời gian ấy cùng một công thức lấy tổng, bằng một con đường có phần bớt mạo hiểm hơn, gần với con đường ngày nay: thực vậy, ông lặp lại công thức "kiểu Taylor" biểu diễn $f(x)$ nhờ các sai phân $f^{(2k+1)}(x+1) - f^{(2k+1)}(x)$, một công thức mà ông thu được bằng cách "nghịch đảo" các khai triển Taylor của những sai phân ấy bằng phương pháp hệ số bất định ([214], v. II, pp. 672-675); ngoài ra, ông không nhận thấy luật thành lập của các hệ số, do Euler phát hiện.

Nhưng Maclaurin, cũng như Euler và tất cả các nhà toán học cùng thời với họ, trình bày mọi công thức của mình như những khai triển thành *chuỗi*, mà sự hội tụ thậm chí còn không được nghiên cứu. Không phải là khái niệm chuỗi hội tụ hoàn toàn bị bỏ qua vào thời ấy: người ta biết từ Jakob Bernoulli rằng chuỗi điều hòa là phân kỳ, và chính Euler cũng đã ghi nhận kết quả này khi tính tổng của $n$ số hạng đầu của chuỗi ấy bằng công thức lấy tổng của ông ([108 a], (1), v. XIV,

$^2$ Năm 1743, Euler, để trả lời những lời chỉ trích khác nhau của các người cùng thời, đã đưa ra một suy dẫn có phần khả dĩ hơn của các "khai triển kiểu Euler" của các hàm lượng giác; chẳng hạn, khai triển thành một tích vô hạn của $\sin x$ được rút ra từ biểu thức $\sin x = \frac{1}{2i}(e^{ix} - e^{-ix})$, và từ sự kiện rằng $e^{ix}$ là giới hạn của đa thức $(1 + \frac{ix}{n})^n$ (loc. cit., pp. 138-155).

pp. 87-100 and 108-123); cũng chính Euler nhận thấy rằng tỉ số của hai số Bernoulli liên tiếp tăng vô hạn, và do đó suy ra một chuỗi nguyên có các số ấy làm hệ số thì không thể hội tụ (*loc. cit.*, p. 357).$^3$ Nhưng xu hướng tính toán hình thức mạnh hơn, và trực giác phi thường của chính Euler cũng không ngăn ông đôi khi rơi vào điều vô lý, khi ông chẳng hạn viết $0 = \sum_{n=-\infty}^{+\infty} x^n$ (*loc. cit.*, p. 362).$^4$

Chúng tôi đã nói ở nơi khác (xem p. 153) các nhà toán học vào đầu thế kỷ XIX, mệt mỏi vì lối hình thức chủ nghĩa không kiềm chế và không có cơ sở này, đã đưa Giải tích trở lại con đường của tính chặt chẽ như thế nào. Một khi khái niệm chuỗi hội tụ được làm chính xác, sự cần thiết của những tiêu chuẩn đơn cung cấp một chứng minh về sự hội tụ của các tích phân và các chuỗi bằng cách so sánh với những tích phân hoặc chuỗi đã biết đã xuất hiện; Cauchy đưa ra một số tiêu chuẩn như vậy trong *Analyse algébrique* của ông ([56 a], (2), v. III), trong khi Abel, trong một hồi ký di cảo ([1], v. II, pp. 197-205), thu được các tiêu chuẩn lôgarit về hội tụ. Mặt khác, Cauchy ([56 a], (1), v. VIII, pp. 18-25) làm sáng tỏ nghịch lý của những chuỗi như chuỗi Stirling, thu được bằng cách áp dụng công thức Euler-Maclaurin (và thường được gọi là "chuỗi nửa hội tụ"): ông chỉ ra rằng nếu (do nhận xét của Euler về các số Bernoulli) số hạng tổng quát $u_k(n)$ của một chuỗi như vậy, với một giá trị *cố định* của $n$, tăng vô hạn theo $k$, thì tuy vậy vẫn đúng là, với một giá trị *cố định* của $k$, tổng riêng $s_k(n) = \sum_{h=1}^k u_h(n)$ cho một khai triển tiệm cận (khi $n$ tiến tới $+\infty$) của hàm được chuỗi "biểu diễn", và độ chính xác càng cao khi $k$ càng lớn.

Trong đại đa số các phép tính của Giải tích cổ điển, có thể thu được một luật hình thành tổng quát cho các khai triển tiệm cận của một hàm, có một số hạng *lớn tùy ý*; sự kiện này đã góp phần tạo ra một sự lẫn lộn lâu dài (ít nhất là trong ngôn ngữ) giữa chuỗi và khai triển tiệm cận; đến mức H. Poincaré, khi ông bỏ công, vào năm 1886 ([251 a], v. I, pp. 290-296), hệ thống hóa các quy tắc sơ cấp của các khai triển tiệm cận (theo các lũy thừa nguyên của $1/x$ trong lân cận của $+\infty$), vẫn còn dùng từ vựng của lý thuyết chuỗi. Chỉ đến khi xuất hiện các khai triển tiệm cận bắt nguồn từ lý thuyết giải tích các số thì mới có một sự phân biệt rõ ràng giữa khái niệm khai triển tiệm cận và khái niệm chuỗi, do sự kiện là, trong đại đa số các bài toán mà lý thuyết này xét đến, chỉ có thể thu được tường minh một số rất nhỏ số hạng (thường chỉ một) trong khai triển cần tìm.

$^3$ Vì chuỗi mà Euler xét ở chỗ này được đưa vào liên hệ với việc tính toán số, ông chỉ lấy tổng các số hạng giảm, và bắt đầu từ chỉ số mà tại đó các số hạng bắt đầu tăng, ông thay chúng bằng một số dư mà ông không chỉ ra nguồn gốc (số dư của công thức Euler-Maclaurin trong dạng tổng quát của nó không xuất hiện trước Cauchy).

$^4$ Thật mỉa mai là công thức này lại xuất hiện, chỉ cách đó một trang, sau một đoạn mà Euler cảnh báo chống lại việc sử dụng không cân nhắc các chuỗi phân kỳ!

Những bài toán này cũng làm cho các nhà toán học quen thuộc với việc dùng các thang so sánh khác với các thang lũy thừa của biến (thực hoặc nguyên). Sự mở rộng này bắt nguồn từ công trình của P. du Bois-Reymond [94 a and b], người đầu tiên đã tấn công một cách có hệ thống các bài toán so sánh các hàm trong lân cận của một điểm, và, trong những công trình rất độc đáo, đã nhận ra tính chất "phi-Archimede" của các thang so sánh, đồng thời nghiên cứu một cách tổng quát việc lấy tích phân và vi phân các quan hệ so sánh, và từ đó rút ra một số lớn hệ quả thú vị [94 b]. Tuy nhiên, các chứng minh của ông thiếu sáng sủa và chặt chẽ, và chính G. H. Hardy [147] là người đã đưa ra cách trình bày đúng đắn các kết quả của du Bois-Reymond: đóng góp chủ yếu của ông là nhận ra và chứng minh sự tồn tại của một tập hợp các "hàm sơ cấp", các hàm $(H)$, trên đó các phép toán thường dùng của Giải tích (đặc biệt là phép vi phân) áp dụng được cho các quan hệ so sánh.
