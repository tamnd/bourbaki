---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: evt-i-v
pdf_pages: 0338-0368
extraction: ocr
statements: 0
exercises: 0
content_sha256: cad20ac89c9e8afb880c90164133d35f9e257df5ef3b452a2029642dd97dfcab
translated_from: content/en/evt/V/historical_note.md
source_content_sha256: 1d568cdf6b7620392b098601685ec9ec289112bf1642f357259f2fe9d3aa3c33
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5.4-mini, gpt-5-mini
translation_run: translate-vi-18a9928e
glossary_version: 34
glossary_terms_sha256: 953ed0114fc1f8e6504a1d39867cb11d50875b0f9a42941010ce5f70b669ab7c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(chương I đến V)

(N.B. — Các chữ cái La Mã chỉ đến thư mục tài liệu tham khảo ở cuối ghi chú này.)
Lý thuyết tổng quát về các không gian vectơ tôpô được xây dựng trong khoảng thời gian từ năm 1920 đến năm 1930. Nhưng cơ sở của nó đã được chuẩn bị từ lâu qua việc nghiên cứu nhiều bài toán của Giải tích phiếm hàm; chúng ta không thể lần lại lịch sử của chủ đề này mà không chỉ ra, ít nhất một cách vắn tắt, cách mà việc nghiên cứu các bài toán này dần dần (đặc biệt kể từ đầu thế kỷ 20) đã dẫn các nhà toán học đến nhận thức về mối quan hệ giữa các vấn đề đang được xét và khả năng phát biểu chúng theo một cách tổng quát hơn nhiều, cũng như áp dụng cho chúng các phương pháp nghiệm thống nhất.

Có thể nói rằng những sự tương tự giữa Đại số và Giải tích, và ý tưởng xem xét các phương trình phiếm hàm (\emph{i.e.} trong đó ẩn là một hàm) như những « trường hợp giới hạn » của các phương trình đại số có nguồn gốc từ Phép tính vi phân vô cùng bé, môn học mà theo một nghĩa nào đó được phát minh để tổng quát hóa « từ hữu hạn đến vô hạn ». Nhưng tổ tiên đại số trực tiếp của Phép tính vi phân vô cùng bé là Phép tính sai phân hữu hạn (\emph{cf.} FVR, Ghi chú lịch sử của các chương I, II, III, p. 54-58) chứ không phải là nghiệm của các hệ tuyến tính tổng quát; chỉ sau giữa thế kỷ 18 những sự tương tự đầu tiên giữa cái sau và các bài toán của Phép tính vi phân mới xuất hiện trong việc nghiên cứu các phương trình của dây rung. Chúng ta sẽ không đi vào chi tiết lịch sử của bài toán này ở đây; nhưng sự tái xuất hiện liên tục của hai ý tưởng cơ bản nổi bật lên, cả hai dường như đều là do D. Bernoulli. Ý tưởng thứ nhất là xem sự dao động của dây như một « trường hợp giới hạn » của sự dao động của một hệ gồm $n$ khối lượng điểm khi $n$ tăng vô hạn; chúng ta biết rằng, về sau, bài toán này, với $n$ hữu hạn, là ví dụ đầu tiên trong việc tìm kiếm các trị riêng của một phép biến đổi tuyến tính (\emph{cf.} A, Các Ghi chú lịch sử của các chương VI-VII); các số này tương ứng trong trường hợp giới hạn với các tần số của các « dao động riêng » của dây, những dao động đã được quan sát bằng thực nghiệm từ lâu trước đó, và sự tồn tại về mặt lý thuyết của chúng đã được thiết lập (đặc biệt bởi Taylor) vào đầu thế kỷ. Sự tương tự hình thức này, mặc dù hầu như không bao giờ được nhắc đến về sau ((I, \emph{b}), p. 390), dường như chưa bao giờ bị mất khỏi tầm nhìn trong suốt thế kỷ 19; nhưng như chúng ta sẽ thấy, nó chỉ đạt được tầm quan trọng đầy đủ của mình vào khoảng những năm 1890-1900.

Ý tưởng khác của D. Bernoulli (có lẽ được gợi ý bởi các sự kiện thực nghiệm) là « nguyên lý chồng chất », theo đó dao động tổng quát nhất của dây phải « phân tích được » bằng sự chồng chất của các « dao động riêng »; nói một cách toán học, điều này có nghĩa là nghiệm tổng quát của phương trình dây rung phải có một khai triển chuỗi dạng $\sum_n c_n \phi_n(x, t)$, trong đó các $\phi_n(x, t)$ biểu diễn các dao động riêng. Chúng ta biết rằng nguyên lý này là điểm khởi đầu của một cuộc tranh luận dài về khả năng khai triển một hàm « tùy ý » thành một chuỗi lượng giác, cuộc tranh luận chỉ được giải quyết bởi các công trình của Fourier và Dirichlet vào phần ba đầu tiên của thế kỷ 19. Nhưng ngay cả trước khi đạt được kết quả này, đã có những ví dụ khác về khai triển chuỗi theo các hàm « trực giao » \* : các hàm cầu, các đa thức Legendre, và cũng các hệ khác nhau dạng $e^{i\lambda_n x}$, trong đó các $\lambda_n$ không còn là các bội của cùng một số; những hệ này đã được đưa vào từ thế kỷ 18 trong các bài toán dao động, cũng như bởi Fourier và Poisson trong quá trình nghiên cứu của họ về lý thuyết nhiệt. Khoảng năm 1830, Sturm (I) và Liouville (II) đã hệ thống hóa tất cả các hiện tượng nhận thấy trong những trường hợp riêng biệt khác nhau này thành một lý thuyết tổng quát về dao động đối với các hàm của một biến; họ xét phương trình vi phân

$$
(1)\quad \frac{d}{dx} \left( p(x) \frac{dy}{dx} \right) + \lambda \rho(x) y = 0 \quad (p(x) > 0,\ \rho(x) > 0)
$$

với các điều kiện biên

$$
(2)\quad
\begin{aligned}
k_1 y'(a) - h_1 y(a) &= 0 \\
k_2 y'(b) + h_2 y(b) &= 0
\end{aligned}
$$
$
(h_1 k_1 \neq 0,\ h_2 k_2 \neq 0,\ a < b)
$

và đã chứng minh các kết quả cơ bản sau đây :
1) bài toán có nghiệm khác không chỉ khi $\lambda$ nhận một trong các giá trị của một dãy $(\lambda_n)$ các số $> 0$, tiến tới $+ \infty$;
2) với mỗi $\lambda_n$, các nghiệm là các bội của cùng một hàm $v_n$, hàm này có thể được giả sử là « chuẩn hóa » bởi điều kiện $\int_a^b \rho v_n^2 dx = 1$, và với $m \neq n$ ta có
$$
\int_a^b \rho v_m v_n dx = 0 ;
$$
3) mọi hàm khả vi hai lần $f$ trên $[a, b]$ thỏa mãn các điều kiện biên (2), có thể được khai triển thành một chuỗi hội tụ đều dạng $f(x) = \sum_n c_n v_n(x)$,
trong đó $c_n = \int_a^b \rho f v_n dx ;$
4) đẳng thức $\int_a^b \rho f^2 dx = \sum_n c_n^2$ đúng (đẳng thức này đã được Parseval chứng minh vào năm 1799, mặc dù theo một cách hoàn toàn hình thức, đối với hệ các hàm lượng giác; và từ đó « bất đẳng thức Bessel » suy ra ngay lập tức; bất đẳng thức sau đã được Bessel công bố (một lần nữa đối với các chuỗi lượng giác) vào năm 1828).

Nửa thế kỷ sau, các tính chất này được hoàn thiện bởi công trình của Gram (III), người, tiếp theo các nghiên cứu của Tchebichef, đã làm sáng tỏ mối quan hệ giữa

\* Tuy nhiên, thuật ngữ này không xuất hiện trước công trình của Hilbert.

sự phát triển thành chuỗi của các hàm trực giao và bài toán « xấp xỉ bậc hai tốt nhất » (một hệ quả trực tiếp của « phương pháp bình phương tối thiểu » của Gauss trong lý thuyết sai số); bài toán sau gồm có điều sau đây : cho một dãy hữu hạn các hàm $(\psi_i)_{1 \leq i \leq n}$, và một hàm $f$, tìm tổ hợp tuyến tính $\sum_i a_i \psi_i$ sao cho tích phân $\int_a^b \rho(f - \sum_i a_i \psi_i)^2 dx$ đạt giá trị nhỏ nhất của nó. Về nguyên tắc, điều này chỉ gợi ra một bài toán đại số tuyến tính tầm thường, nhưng Gram đã giải quyết nó theo một cách nguyên bản, bằng cách áp dụng phương pháp « trực chuẩn hóa » cho các $\psi_i$, như đã mô tả trong chương V, p. 23 (và nói chung được biết dưới tên của Erhard Schmidt). Tiếp theo, trong trường hợp một hệ trực chuẩn vô hạn, nảy sinh câu hỏi tìm xem khi nào « xấp xỉ bậc hai tốt nhất » $\mu_n$ của một hàm $f$, bởi các tổ hợp tuyến tính của $n$ hàm đầu tiên của dãy, tiến tới 0 khi $n$ tăng vô hạn *; do đó Gram đã đi đến định nghĩa khái niệm hệ trực chuẩn đầy đủ, và nhận ra rằng tính chất này tương đương với sự không tồn tại của các hàm khác không trực giao với tất cả các $\phi_n$. Ông thậm chí còn thử làm sáng tỏ khái niệm « hội tụ bậc hai trung bình », nhưng trước khi đưa vào các ý tưởng cơ bản của lý thuyết độ đo, ông hầu như không thể thu được các kết quả tổng quát nào theo hướng này.

Trong nửa sau của thế kỷ 19, nỗ lực chính của các nhà giải tích chủ yếu hướng tới việc mở rộng lý thuyết Sturm-Liouville cho các hàm của nhiều biến. Lý thuyết này được thúc đẩy bởi việc nghiên cứu các phương trình vi phân riêng phần elliptic xuất hiện trong Vật lý Toán học, và các bài toán giá trị biên liên kết tự nhiên với các phương trình này. Mối quan tâm chính trước hết tập trung vào phương trình « màng rung »

$$
L_\lambda(u) \equiv \Delta u + \lambda u = 0
$$

trong đó người ta tìm các nghiệm triệt tiêu trên biên của một miền G đủ chính quy; các phương pháp đã thành công đối với các hàm của một biến không còn thích hợp cho bài toán này nữa, và những khó khăn giải tích đáng kể xuất hiện đã được khắc phục từng bước. Ta nhắc lại các bước chính hướng tới nghiệm : việc đưa vào « hàm Green » của G, sự tồn tại của nó đã được Schwarz chứng minh; chứng minh, cũng do Schwarz, về sự tồn tại của trị riêng nhỏ nhất; và cuối cùng, vào năm 1894, H. Poincaré, trong một hồi ký nổi tiếng (V a) đã thành công trong việc chứng minh sự tồn tại và các tính chất cốt yếu của tất cả các trị riêng. Ông xét nghiệm của phương trình $L_\lambda(u) = f$, với một « vế thứ hai » $f$ đã cho; nghiệm này triệt tiêu trên biên; sau đó bằng một phép tổng quát hóa khéo léo phương pháp của Schwarz, ông chứng minh rằng $u_\lambda$ là một hàm phân hình của biến phức $\lambda$, chỉ có các cực đơn thực $\lambda_n$, và đây chính xác là các trị riêng cần tìm.

\* Cần chỉ ra rằng trong nghiên cứu này, Gram không tự hạn chế chỉ xét các hàm liên tục, mà nhấn mạnh tầm quan trọng của điều kiện $\int_a^b \rho f^2 dx < + \infty$.

Các nghiên cứu này liên quan trực tiếp đến những khởi đầu của lý thuyết các phương trình tích phân tuyến tính, lý thuyết chắc chắn đã góp phần tối đa vào sự ra đời của các ý tưởng hiện đại. Ở đây chúng ta sẽ tự giới hạn ở việc đưa ra một phác thảo ngắn gọn về sự phát triển của lý thuyết này (để biết chi tiết đầy đủ hơn, chúng ta tham khảo các Chú thích lịch sử sẽ theo sau các chương của Luận thuyết này dành cho lý thuyết phổ). Loại phương trình phiếm hàm này, lần đầu tiên xuất hiện một cách khiêm tốn trong nửa đầu thế kỷ 19 (Abel, Liouville), đã có một tầm quan trọng nào đó kể từ khi Beer và C. Neumann đưa nghiệm của « bài toán Dirichlet » cho một miền G đủ chính quy về nghiệm của một « phương trình tích phân loại hai »

$$
u(x) + \int_a^b K(x, y) u(y) \, dy = f(x)
$$

đối với hàm chưa biết $u$; C. Neumann đã giải được phương trình này vào năm 1877 bằng một phương pháp « xấp xỉ liên tiếp ». Được thúc đẩy vừa bởi các tương tự đại số đã nêu ở trên vừa bởi các kết quả ông đã thu được đối với phương trình màng rung, H. Poincaré, vào năm 1896 (V b) đã đưa một tham số biến $\lambda$ vào phía trước tích phân trong phương trình trước đó, và khẳng định rằng, cũng như trong trường hợp phương trình màng rung, nghiệm lại một lần nữa là một hàm phân hình của $\lambda$; nhưng ông không thể chứng minh kết quả này. Điều này đã được thiết lập bảy năm sau bởi I. Fredholm (VI) (đối với một « hạt nhân » liên tục K và một khoảng hữu hạn $[a, b]$). Tác giả được nhắc đến sau cùng này, có lẽ với sự nhận thức rõ hơn các tiền bối của mình, đã để mình được dẫn dắt bởi sự tương tự của (4) với hệ tuyến tính

$$
\sum_{q=1}^n (\delta_{pq} + \frac{1}{n} a_{pq}) x_q = b_p \quad (1 \leq p \leq n)
$$

để thu được nghiệm của (4) như thương của hai biểu thức, dựa trên mô hình của các định thức, xuất hiện trong các công thức của Cramer. Tuy nhiên, đây không phải là một ý tưởng mới : từ đầu thế kỷ 19, phương pháp « hệ số bất định » (gồm việc thu được một hàm chưa biết, được giả sử có một khai triển thành chuỗi $\sum_n c_n \phi_n$, trong đó các $\phi_n$ là các hàm đã biết, bằng cách tính các hệ số $c_n$) đã dẫn đến « các hệ tuyến tính với vô hạn ẩn số »

$$
\sum_{j=1}^\infty a_{ij} x_j = b_i \quad (i = 1, 2, ...).
$$

Fourier, người đã gặp phải một hệ như vậy, vẫn giải quyết nó như một nhà toán học thế kỷ XVIII: ông bỏ đi tất cả các số hạng có chỉ số $i$ hoặc $j$ lớn hơn $n$, giải tường minh hệ hữu hạn thu được bằng các công thức Cramer, rồi chuyển qua giới hạn bằng cách cho $n$ tiến tới $+ \infty$ trong nghiệm ! Mãi về sau, khi cách làm này không còn được chấp nhận nữa, người ta lại dùng lý thuyết định thức để tấn công bài toán ; Kể từ năm 1886 (theo công trình của Hill), H. Poincaré, rồi H. von Koch, đã xây dựng một lý thuyết về « định thức vô hạn », cho phép giải một số loại hệ (6) bằng cách theo mô hình cổ điển; và mặc dù các kết quả này không áp dụng trực tiếp được cho bài toán mà Fredholm nghiên cứu, không còn nghi ngờ gì rằng đặc biệt lý thuyết của von Koch đã dùng làm mô hình cho phép dựng các « định thức » của Fredholm.

Chính vào thời điểm này Hilbert xuất hiện và tạo ra một động lực mới cho lý thuyết (VII). Trước hết, ông hoàn thiện công trình của Fredholm bằng cách thực hiện thực sự phép chuyển qua giới hạn, phép này dẫn đến nghiệm của (4) từ nghiệm của (5); nhưng ông ngay lập tức đưa vào phép chuyển qua giới hạn tương ứng trong lý thuyết các dạng toàn phương thực, lý thuyết này nảy sinh một cách tự nhiên từ các phương trình tích phân có hạt nhân đối xứng (*tức là* sao cho $K(y, x) = K(x, y)$). Đây là những phương trình thường gặp nhất trong Vật lý Toán học. Do đó ông đã thu được công thức cơ bản trực tiếp tổng quát hóa phép đưa một dạng toàn phương về các trục của nó

$$
\int_a^b \int_a^b K(s, t) \ x(s) \ x(t) \ dsdt = \sum_{n=1}^\infty \frac{1}{\lambda_n} \left( \int_a^b \phi_n(s) \ x(s) \ ds \right)^2,
$$

trong đó các $\lambda_n$ là các giá trị riêng (nhất thiết thực) của hạt nhân K, các $\phi_n$ lập thành hệ trực chuẩn của các hàm riêng tương ứng, và vế thứ hai của công thức (7) là một chuỗi hội tụ nếu $\int_a^b x^2(s) \ ds \leq 1$. Ông cũng chỉ ra cách mà mọi hàm được « biểu diễn » dưới dạng $f(x) = \int_a^b K(x, y) \ g(y) \ dy$ có một « khai triển » $\sum_{n=1}^\infty \phi_n(x) \int_a^b \phi_n(y) \ f(y) \ dy$, và, theo phép tương tự với lý thuyết cổ điển về các dạng toàn phương, ông chỉ ra một thủ tục xác định các $\lambda_n$ bằng một phương pháp biến phân. Đây chính xác là sự mở rộng của các tính chất cực trị quen thuộc của các trục chính của một mặt bậc hai ((VII), p. 1-38).

Các kết quả sơ bộ này của Hilbert gần như ngay lập tức được E. Schmidt tiếp nhận, dưới một dạng đơn giản hơn và tổng quát hơn, tránh việc đưa vào các « định thức của Fredholm » và cũng tránh việc chuyển từ hữu hạn sang vô hạn. Cách trình bày khi đó đã rất gần với dạng trừu tượng, các tính chất cơ bản của tính tuyến tính và tính dương của phép tích phân rõ ràng là những sự kiện duy nhất được sử dụng trong chứng minh (VII *a*). Nhưng vào thời điểm đó Hilbert đã phát triển các khái niệm tổng quát hơn nhiều. Tất cả các công trình trước đó đã làm nổi bật tầm quan trọng của các hàm bình phương khả tích, và công thức Parseval đã thiết lập một liên hệ trực tiếp giữa các hàm này và các dãy $(c_n)$ sao cho $\sum_n c_n^2 < \infty$. Chắc chắn chính ý tưởng này đã hướng dẫn Hilbert trong các hồi ký năm 1906 của ông ((VII), chap. XI-XIII), trong đó, một lần nữa tiếp nhận phương pháp cũ về « các hệ số bất định », ông đã chỉ ra rằng nghiệm của phương trình tích phân (4) tương đương với nghiệm của một hệ vô hạn các phương trình tuyến tính

$$
x_p + \sum_{q=1}^\infty k_{pq} x_q = b_p \quad (p = 1, 2, ...)
$$

đối với các « hệ số Fourier » $x_p = \int_a^b u(t) \omega_p(t) \, dt$ của hàm chưa biết $u$
theo một hệ trực chuẩn đầy đủ cho trước $(\omega_n)$ (với $b_p = \int_a^b f(t) \omega_p(t) \, dt$)
và $k_{pq} = \int_a^b \int_a^b K(s, t) \omega_p(s) \omega_q(t) \, dsdt$. Hơn nữa, theo quan điểm này, các nghiệm duy nhất của (8) được quan tâm là những nghiệm thỏa mãn $\sum_n x_n^2 < +\infty$; vì vậy Hilbert đã hạn chế một cách có hệ thống vào loại nghiệm này; nhưng mặt khác, ông đã mở rộng các điều kiện áp đặt lên « ma trận vô hạn » $k_{pq}$ (trong (8) nó thỏa mãn $\sum_{p,q} k_{pq}^2 < +\infty$). Từ đó trở đi, rõ ràng rằng « không gian Hilbert » của tất cả các dãy $x = (x_n)$ các số thực sao cho $\sum_n x_n^2 < +\infty$, mặc dù không được đưa vào một cách tường minh, là không gian làm nền tảng cho toàn bộ lý thuyết, và xuất hiện như một « phép chuyển qua giới hạn » từ một không gian Euclid hữu hạn chiều. Ngoài ra, và điều này đặc biệt quan trọng đối với những phát triển sau này, Hilbert đã được dẫn đến việc đưa vào không chỉ một mà hai khái niệm hội tụ phân biệt trong không gian này (tương ứng với điều sau này được gọi là tôpô yếu và tôpô mạnh *), cũng như một « nguyên lý lựa chọn » chính xác là tính chất compact yếu của quả cầu đơn vị. Đại số tuyến tính mới mà ông phát triển liên quan đến việc giải hệ (8) hoàn toàn phụ thuộc vào các ý tưởng tôpô này: các ánh xạ tuyến tính, các dạng tuyến tính và các dạng song tuyến tính (liên kết với các ánh xạ tuyến tính) được phân loại và nghiên cứu theo các tính chất « liên tục » của chúng **. Đặc biệt, Hilbert phát hiện rằng sự thành công của phương pháp Fredholm phụ thuộc vào khái niệm « tính liên tục hoàn toàn », mà ông đã phục hồi bằng cách phát biểu nó cho các dạng song tuyến tính *** và nghiên cứu nó một cách sâu sắc; để biết thêm chi tiết, chúng tôi tham chiếu đến phần của Luận thuyết này nơi khái niệm quan trọng này sẽ được phát triển, và cũng đến các công trình đáng ngưỡng mộ và sâu sắc của Hilbert, nơi ông đã khai sinh lý thuyết phổ của các dạng song tuyến tính đối xứng (bị chặn hoặc không).

Ngôn ngữ của Hilbert vẫn còn mang tính cổ điển, và trong toàn bộ « Grundziige », ông không bao giờ mất đi sự chú ý đối với các ứng dụng của lý thuyết mà ông đã phát triển từ nhiều ví dụ (chiếm gần một nửa của tập sách). Thế hệ tiếp theo đã chấp nhận một quan điểm trừu tượng hơn nhiều. Dưới ảnh hưởng của các ý tưởng của Fréchet và F. Riesz về tôpô tổng quát (xem các Ghi chú lịch sử của GT, chương I), E. Schmidt

\* Phép tính biến phân tất nhiên đã dẫn đến những khái niệm khác nhau về sự hội tụ trên cùng một tập hợp các hàm (tùy theo yêu cầu về sự hội tụ đều của các hàm, hoặc về sự hội tụ đều của các hàm và của một số đạo hàm của chúng); nhưng các kiểu hội tụ được Hilbert định nghĩa hoàn toàn mới vào thời điểm đó.
** Cần chỉ ra rằng cho đến khoảng năm 1935, một hàm « liên tục » thường được hiểu là một ánh xạ biến mọi dãy hội tụ thành một dãy hội tụ.
*** Đối với Hilbert, một dạng song tuyến tính B(x, y) là hoàn toàn liên tục nếu, bất cứ khi nào các dãy $(x_n), (y_n)$ hội tụ yếu lần lượt đến x và y, B$(x_n, y_n)$ hội tụ đến B(x, y).

(VII b) và chính Fréchet, trong các năm 1907-1908, đã cố ý đưa ngôn ngữ của hình học Euclid vào « không gian Hilbert » (thực hoặc phức); chính trong các công trình này chúng ta tìm thấy lần đầu tiên sự đề cập đến chuẩn (với ký hiệu hiện nay $\|x\|$), bất đẳng thức tam giác mà nó thỏa mãn, và sự kiện rằng một không gian Hilbert là « tách được » và đầy đủ; ngoài ra, E. Schmidt đã chứng minh sự tồn tại của phép chiếu trực giao lên một đa tạp tuyến tính đóng, điều này cho phép ông đưa ra một dạng đơn giản hơn và tổng quát hơn cho lý thuyết của Hilbert về các hệ tuyến tính. Cũng vào năm 1907, Fréchet và F. Riesz nhận thấy rằng không gian các hàm khả tích bình phương có một « hình học » tương tự, một sự tương tự đã được giải thích hoàn toàn khi, vài tháng sau, F. Riesz và E. Fischer chứng minh rằng không gian này là đầy đủ và đẳng cấu với một « không gian Hilbert », đồng thời phô bày một cách nổi bật giá trị của công cụ mới được Lebesgue tạo ra. Kể từ thời điểm này, các điểm cốt yếu của lý thuyết các không gian Hilbert có thể được xem là đã đạt được. Trong các phát triển sau này, cần nhắc đến sự trình bày tiên đề của lý thuyết bởi M. H. Stone và J. von Neumann vào khoảng năm 1930, cũng như việc loại bỏ các hạn chế của tính « tách được », là kết quả của các công trình của Rellich, Löwig và F. Riesz (IX e) vào khoảng năm 1934.

Trong khi đó, trong những năm đầu của thế kỷ 20, các dòng ý tưởng khác đã xuất hiện và củng cố xu hướng dẫn đến lý thuyết các không gian chuẩn. Ý tưởng tổng quát về « phiếm hàm » (nghĩa là một hàm số xác định trên một tập hợp mà các phần tử của nó bản thân là các hàm số của một hoặc nhiều biến thực) đã được khôi phục trong những thập niên cuối của thế kỷ 19 liên quan một mặt với phép tính biến phân, mặt khác với lý thuyết các phương trình tích phân. Nhưng chính chủ yếu từ trường phái Ý, xung quanh Pincherle, và trên hết là Volterra, mà ý tưởng tổng quát về « toán tử » đã nảy sinh. Các công trình của trường phái này thường vẫn ở một mức khá hình thức và liên quan đến các bài toán riêng biệt, do thiếu một phân tích đủ sâu về các khái niệm tôpô nền tảng. Năm 1903, Hadamard đã khởi đầu lý thuyết hiện đại về đối ngẫu « tôpô », trong sự tìm kiếm các « phiếm hàm » tuyến tính liên tục tổng quát nhất trên không gian $\mathcal{C}(I)$ của các hàm số liên tục trên một khoảng compact (được trang bị tôpô của sự hội tụ đều), và ông đã đặc trưng các phiếm hàm này như các giới hạn của các dãy tích phân $x \mapsto \int_I k_n(t) \ x(t) \ dt.$

Năm 1907, Fréchet và F. Riesz đã chứng minh tương tự rằng các dạng tuyến tính liên tục trên một không gian Hilbert là các dạng tuyến tính « bị chặn » được Hilbert đưa vào; sau đó vào năm 1909, F. Riesz đã đưa định lý của Hadamard về dạng cuối cùng bằng cách biểu diễn mọi dạng tuyến tính liên tục trên $\mathcal{C}(I)$ như một tích phân Stieltjes, một định lý mà rất lâu sau đã được dùng làm điểm khởi đầu cho lý thuyết hiện đại về phép tích phân (xem các Ghi chú lịch sử của INT, chương II-V).

Năm sau, F. Riesz (IX a) lại đạt được những tiến bộ mới và quan trọng trong lý thuyết bằng cách đưa vào và nghiên cứu (mô phỏng theo lý thuyết không gian Hilbert) không gian $L^p(I)$ của các hàm trên một khoảng I mà lũy thừa $p$ của chúng là khả tích (với một số mũ $p$ sao cho $1 < p < + \infty$); ba năm sau, nghiên cứu này được tiếp nối bằng các công trình tương tự về các không gian dãy $\ell^p(\mathbf{N})$ (IX c). Những nghiên cứu này, như chúng ta sẽ thấy sau này, đã đóng góp rất nhiều vào việc phân loại các ý tưởng về đối ngẫu, theo nghĩa rằng lần đầu tiên chúng ta gặp hai không gian đối ngẫu không đẳng cấu tự nhiên với nhau *.

Từ đó trở đi, F. Riesz đã nghĩ đến một nghiên cứu tiên đề có thể bao quát tất cả các kết quả này ((IX a), p. 452), và dường như chỉ những sự dè dặt của một nhà giải tích lo lắng không muốn rời xa toán học cổ điển đã ngăn cản ông viết bản hồi ký nổi tiếng năm 1918 của mình về lý thuyết Fredholm (IX d) dưới dạng này. Ở đó ông chủ yếu xét không gian $\mathcal{C}(I)$ của các hàm liên tục trên một khoảng compact; nhưng sau khi định nghĩa chuẩn của không gian này, và nhận thấy rằng $\mathcal{C}(I)$ được trang bị chuẩn này là đầy đủ, ông đã không sử dụng gì khác ngoài các tiên đề của các không gian chuẩn đầy đủ trong các lập luận của mình **. Không đi vào việc khảo sát chi tiết công trình này, chúng ta đề cập rằng khái niệm về một ánh xạ hoàn toàn liên tục đã được định nghĩa (bởi tính chất biến một lân cận thành một tập compact tương đối) một cách tổng quát lần đầu tiên trong công trình này ***; bằng một kiệt tác của giải tích tiên đề, toàn bộ lý thuyết Fredholm (xét về phương diện định tính của nó) đã được quy về một định lý cơ bản duy nhất, rằng mọi không gian chuẩn compact địa phương đều có chiều hữu hạn.

Định nghĩa tổng quát về các không gian định chuẩn đã được đưa ra vào các năm 1920-1922 bởi S. Banach, H. Hahn và E. Helly (người sau chỉ xét các không gian dãy của các số thực hoặc phức). Trong mười năm tiếp theo, lý thuyết về các không gian này phát triển chủ yếu xoay quanh hai vấn đề có tầm quan trọng cơ bản đối với các ứng dụng: lý thuyết đối ngẫu và các định lý gắn với khái niệm «phạm trù» Baire.

Chúng ta đã thấy rằng ý tưởng về đối ngẫu (theo nghĩa tôpô) bắt nguồn từ đầu thế kỷ 20; đó là khái niệm nền tảng trong lý thuyết của Hilbert và chiếm một vị trí trung tâm trong công trình của F. Riesz. Chẳng hạn, người sau đã nhận thấy vào năm 1911 ((IX b), p. 41-42) rằng quan hệ $|f(x)| \leq M \|x\|$ (được lấy làm định nghĩa của các phiếm hàm tuyến tính «bị chặn» trong một không gian Hilbert) là tương đương với tính liên tục của $f$ trong trường hợp của không gian $\mathcal{C}(I)$, và điều này đã được chứng minh bằng các lập luận khá tổng quát. Về đặc trưng hóa các phiếm hàm tuyến tính liên tục trên $\mathcal{C}(I)$, ông còn nhận thấy rằng điều kiện để một tập hợp A là toàn phần trong $\mathcal{C}(I)$ là không tồn tại độ đo Stieltjes $\mu \neq 0$ trên I «trực giao» với tất cả các hàm trong A (do đó tổng quát hóa điều kiện của Gram đối với các hệ trực chuẩn đầy đủ); cuối cùng, trong cùng

\* Mặc dù thực tế rằng đối ngẫu giữa $L^1$ và $L^\infty$ đã tiềm ẩn trong phần lớn các công trình của thời kỳ này về tích phân Lebesgue, chỉ đến năm 1918 H. Steinhaus mới chứng minh rằng mọi dạng tuyến tính liên tục trên $L^1(I)$ (I là một khoảng hữu hạn) đều có dạng $x \mapsto \int_I f(t) \ x(t) \ dt$, trong đó $f \in L^\infty(I)$.

** F. Riesz tuy nhiên đã nhận xét một cách tường minh rằng các ứng dụng các định lý của ông vào các hàm liên tục chỉ là một «phép thử» của những khái niệm tổng quát hơn nhiều ((IX d), p. 71).

*** Trong công trình của mình về các không gian $L^p$, F. Riesz đã định nghĩa các ánh xạ hoàn toàn liên tục là những ánh xạ biến mọi dãy hội tụ yếu thành một dãy hội tụ mạnh; điều này (do tính compact yếu của quả cầu đơn vị trong $L^p$ với $1 < p < + \infty$) là tương đương với định nghĩa trên trong trường hợp này; ngoài ra, F. Riesz chỉ ra rằng đối với các không gian $L^2$, định nghĩa của ông tương đương với định nghĩa của Hilbert (bằng cách chuyển từ ngôn ngữ của các ánh xạ tuyến tính sang ngôn ngữ của các dạng song tuyến tính ((IX, a), p. 487)).

công trình đó, ông đã thiết lập rằng đối ngẫu của không gian $L^\infty$ «lớn hơn» không gian các độ đo Stieltjes ((IX b), p. 62).

Mặt khác, F. Riesz, trong công trình của mình về các không gian $L^p(I)$ và $\ell^p(\mathbf{N})$ đã thành công trong việc sửa đổi phương pháp giải các hệ tuyến tính trong một không gian Hilbert, do E. Schmidt đưa ra (VIII b), để có thể áp dụng trong các trường hợp tổng quát hơn. Ý tưởng của E. Schmidt bao gồm việc xác định một nghiệm «cực trị» của (6) bằng cách tìm một điểm trong đa tạp tuyến tính đóng được biểu diễn bởi các phương trình (6), có khoảng cách đến gốc là nhỏ nhất. Sử dụng cùng ý tưởng đó, F. Riesz đã chỉ ra rằng điều kiện cần và đủ để tồn tại một hàm $x \in L^p(a, b)$ thỏa mãn các phương trình

$$
\int_a^b \alpha_i(t)\, x(t)\, dt = b_i \quad (i = 1, 2, ...)
$$

(trong đó $\alpha_i$ thuộc $L^q$ (với $\frac{1}{p} + \frac{1}{q} = 1$), và ngoài ra $\int_a^b |x(t)|^p dt \leq M^p$, là, đối với mọi dãy hữu hạn $(\lambda_i)_{1 \leq i \leq n}$ của các số thực, ta có

$$
|\sum_{i=1}^n \lambda_i b_i| \leq M \left( \int_a^b |\sum_{i=1}^n \lambda_i \alpha_i(t)|^q dt \right)^{1/q}.
$$

Năm 1911 (IX b), ông đã xử lý, theo một cách tương tự, «bài toán mômen tổng quát», bao gồm việc giải hệ

$$
\int_a^b \alpha_i(t)\, d\xi(t) = b_i \quad (i = 1, 2, ...)
$$

trong đó $\alpha_i$ là các hàm liên tục và ẩn là một độ đo Stieltjes $\xi$; trong trường hợp này rõ ràng rằng bài toán có thể được phát biểu lại bằng cách nói rằng nó bao gồm việc xác định một phiếm hàm tuyến tính liên tục trên $\mathcal{C}(I)$ từ các giá trị của nó trên một dãy điểm cho trước trong không gian này. Chính dưới dạng này mà Helly đã xử lý bài toán vào năm 1912 — thu được các điều kiện của F. Riesz bằng một phương pháp khá khác biệt có phạm vi rộng hơn nhiều \* — và ông lại xét đến nó vào năm 1921, với các điều kiện tổng quát hơn nhiều. Đưa vào khái niệm chuẩn (trên các không gian dãy), như chúng ta đã thấy ở trên, ông nhận thấy

\* «Bài toán mômen» cổ điển tương ứng với trường hợp khoảng ]$a, b$ là ]$0, + \infty$ hoặc ]$- \infty, + \infty$, và $\alpha_i(t) = t^i$; hơn nữa, người ta giả sử rằng độ đo $\xi$ là dương (trong hồi ký năm 1911 của mình, F. Riesz đã chỉ ra cách các điều kiện tổng quát của ông phải được sửa đổi khi tìm kiếm các nghiệm có bản chất này). Trong số các phương pháp khác nhau để giải bài toán mômen cổ điển, chúng tôi đặc biệt nhắc đến phương pháp của F. Riesz, người đã kết hợp rất thanh nhã các ý tưởng tổng quát của phép tính hàm và lý thuyết các hàm của một biến phức để thu được các điều kiện tường minh trên các $b_i$. (Sur le problème des moments, 3, Ark. för Math., t. XVII (1922-1923), n° 16, 52 p.)

rằng khái niệm này khái quát hóa khái niệm « gauge » của một thân lồi trong một không gian $n$-chiều, như Minkowski đã dùng trong công trình nổi tiếng của ông về « hình học của các số » (IV). Trong quá trình nghiên cứu của mình, Minkowski cũng đã định nghĩa (trong $\mathbf{R}^n$) các khái niệm về một siêu phẳng đỡ và về một « hàm đỡ » (IV $b$), và đã chứng minh sự tồn tại của một siêu phẳng đỡ tại mọi điểm trên biên của một thân lồi ((IV $a$), p. 33-35). Helly đã mở rộng các khái niệm này sang một không gian các dãy E, được trang bị một chuẩn tùy ý ; ông đã thiết lập một đối ngẫu giữa E và không gian E' của các dãy $u = (u_n)$ sao cho với mọi $x = (x_n) \in E$, chuỗi $(u_n x_n)$ hội tụ ; ký hiệu $\langle u, x \rangle$ là tổng của chuỗi này, ông đã định nghĩa một chuẩn trên E' bởi công thức $\sup_{x \neq 0} |\langle u, x \rangle| / \|x\|$, công thức này cho hàm đỡ trong các không gian hữu hạn chiều **. Rồi Helly chứng minh rằng nghiệm của một hệ (6) trong E, trong đó mỗi dãy $u_i = (a_{ij})_{j \geq 1}$ được giả thiết thuộc E', quy về việc giải lần lượt hai bài toán sau đây :
1. tìm một dạng tuyến tính liên tục L trên không gian có chuẩn E', sao cho $L(u_i) = b_i$ với mọi chỉ số $i$ ; điều này, như ông đã chỉ ra, dẫn tới các điều kiện kiểu (10) ; 2. xem liệu một dạng tuyến tính như vậy có thể được viết dưới dạng $u \mapsto \langle u, x \rangle$ với một $x \in E$ nào đó hay không. Bài toán sau, ông nhận thấy, không nhất thiết có nghiệm ngay cả khi L tồn tại, và ông đã đưa ra một số điều kiện đủ suy ra sự tồn tại của nghiệm $x \in E$ trong một vài trường hợp riêng biệt (X).

Năm 1927, các ý tưởng ấy đã được trình bày dưới hình thức dứt khoát của chúng trong một luận văn nền tảng của H. Hahn (XI), mà các kết quả của nó đã được S. Banach tái phát hiện (một cách độc lập) hai năm sau (XII $b$). Hahn đã áp dụng các phương pháp của Minkowski-Helly cho một không gian có chuẩn tùy ý, và do đó đã xác định cấu trúc của một không gian có chuẩn (đầy đủ) trên không gian đối ngẫu; điều này ngay lập tức cho phép Hahn xét các đối ngẫu kế tiếp của một không gian có chuẩn, và đặt bài toán về các không gian phản xạ một cách tổng quát, như Helly đã tiên liệu. Nhưng trên hết, bài toán chủ yếu về việc mở rộng một phiếm hàm tuyến tính liên tục mà không làm tăng chuẩn của nó đã được Hahn giải quyết dứt khoát trong trường hợp tổng quát, bằng một lập luận quy nạp siêu hạn theo chiều — qua đó cho một trong những ví dụ đầu tiên về một ứng dụng quan trọng của tiên đề lựa chọn vào giải tích hàm ***. Đối với các kết quả này, Banach đã bổ sung một nghiên cứu chi tiết về các quan hệ giữa một ánh xạ tuyến tính liên tục và chuyển vị của nó, mở rộng sang các không gian có chuẩn tổng quát những kết quả trước đó chỉ biết trong trường hợp các không gian $L^p$ (IX $a$), bằng một định lý sâu sắc về các tập con đóng yếu của đối ngẫu ($cf.$ IV, p. 25, cor. 2); các kết quả này có thể được diễn đạt theo một cách nổi bật hơn bằng cách dùng khái niệm không gian thương của một không gian có chuẩn, khái niệm này được Hausdorff và chính Banach đưa vào vài năm sau đó. Cuối cùng, cũng chính Banach đã phát hiện mối quan hệ giữa tính compact yếu của quả cầu đơn vị (đã được nhận thấy trong một số trường hợp riêng, như đã nói ở trên) và tính phản xạ, ít nhất đối với các không gian thỏa mãn tiên đề đếm được thứ nhất. Từ đó, các nét đại cương của lý thuyết đối ngẫu của các không gian có chuẩn có thể được xem là đã được xác lập.

\* Cũng như F. Riesz ((IX $b$), p. 49-50), Helly đã dùng một « nguyên lý lựa chọn » trong chứng minh của mình, mà chính là tính compact yếu của quả cầu đơn vị trong không gian các độ đo Stieltjes ; F. Riesz cũng đã dùng tính chất tương tự trong các không gian $L^p$ ($1 < p < + \infty$).

** Để thu được một chuẩn theo cách này, ta phải giả sử rằng quan hệ $\langle u, x \rangle = 0$ với mọi $x \in E$ suy ra $u = 0$, như Helly đã nhận xét tường minh.

*** Banach đã từng đưa ra một lập luận tương tự từ năm 1923 để định nghĩa một độ đo bất biến trong mặt phẳng (được định nghĩa cho *mọi* tập con bị chặn) (XII $a$).

Cùng trong thời kỳ ấy, một số định lý có vẻ nghịch lý, mà những ví dụ đầu tiên của chúng xuất hiện vào những năm quanh 1910, đã được làm sáng tỏ. Trong năm đó, Hellinger và Toeplitz về cơ bản đã chứng minh rằng một dãy các dạng song tuyến tính bị chặn $B_n(x, y)$ trên một không gian Hilbert, mà các giá trị $B_n(a, b)$ của nó với mọi cặp $(a, b)$ đều bị chặn (bởi một số phụ thuộc $a$ priori vào $a$ và $b$) thì thật ra bị chặn đều trên mọi quả cầu. Chứng minh của họ dựa trên một lập luận phản chứng, bằng cách dựng lên quy nạp một cặp $(a, b)$ đặc biệt vi phạm giả thiết; phương pháp này từ đó được gọi là « gliding bump », và vẫn hữu ích trong nhiều bài toán tương tự ($cf.$ IV, p. 54, exerc. 15). Năm 1905, Lebesgue đã dùng một phương pháp tương tự để chứng minh sự tồn tại của các hàm liên tục mà chuỗi Fourier của chúng phân kỳ tại một số điểm; và trong cùng năm với Hellinger và Toeplitz ông lại dùng phương pháp ấy, để chứng minh rằng một dãy hội tụ yếu trong $L^1$ bị chặn về chuẩn *. Những ví dụ này xuất hiện ngày càng nhiều trong những năm sau, nhưng không có thêm ý tưởng mới nào cho đến năm 1927, khi Banach và Steinhaus (với sự cộng tác một phần của Saks) liên hệ các hiện tượng này với khái niệm của một tập mỏng và với định lý Baire trong các không gian mêtric đầy đủ, qua đó thu được một mệnh đề tổng quát bao trùm tất cả các trường hợp riêng trước đó (XIII). Cùng trong thời kỳ ấy, việc nghiên cứu các câu hỏi về « loại » trong các không gian có chuẩn đầy đủ đã dẫn Banach tới một số kết quả khác về các ánh xạ tuyến tính liên tục; đáng chú ý nhất và chắc chắn là sâu sắc nhất là định lý « đồ thị đóng » mà, như định lý Banach-Steinhaus, đã trở thành một công cụ thiết yếu trong giải tích hàm hiện đại (XII b).

Việc xuất bản chuyên luận « Các toán tử tuyến tính » của Banach (XII c) đánh dấu sự trưởng thành của lý thuyết các không gian định chuẩn. Tất cả các kết quả đã nêu ở trên và nhiều kết quả khác có thể được tìm thấy trong tập này, mặc dù theo một cách hơi thiếu hệ thống, nhưng với nhiều ví dụ nổi bật rút ra từ những lĩnh vực khác nhau của Giải tích, và dường như báo trước một tương lai rực rỡ cho lý thuyết này. Công trình đã đạt được thành công đáng kể, và một trong những tác động ngay lập tức là sự chấp nhận gần như phổ quát ngôn ngữ và các ký hiệu được Banach sử dụng. Nhưng bất chấp số lượng lớn các nghiên cứu được tiến hành trong 40 năm qua về các không gian Banach (XVII), nếu loại trừ lý thuyết các đại số Banach và những ứng dụng của nó vào giải tích điều hòa giao hoán và không giao hoán, thì sự gần như hoàn toàn thiếu vắng những ứng dụng mới của lý thuyết này vào những bài toán lớn của Giải tích cổ điển phần nào làm suy yếu những hy vọng dựa trên nó.

Chính theo hướng mở rộng và phân tích tiên đề sâu sắc hơn liên quan đến các khái niệm về không gian định chuẩn mà những phát triển phong phú nhất đã diễn ra.

\* Cũng cần nhận thấy định lý tương tự (dễ hơn) do Landau chứng minh năm 1907 và đã làm điểm khởi đầu cho F. Riesz trong lý thuyết các không gian $L^p$ của ông: nếu chuỗi với số hạng tổng quát $u_n x_n$ hội tụ với mọi dãy $(x_n) \in \ell^p(\mathbf{N})$, thì dãy $(u_n)$ thuộc $\ell^q(\mathbf{N})$ (với $\frac{1}{p} + \frac{1}{q} = 1$).

Mặc dù các không gian phiếm hàm gặp phải từ đầu thế kỷ XX nói chung dường như được trang bị một chuẩn « tự nhiên », vẫn có một số ngoại lệ. Khoảng năm 1910, E. H. Moore đã đề xuất một phép tổng quát hóa khái niệm hội tụ đều bằng cách thay thế nó bằng một khái niệm « hội tụ đều tương đối », trong đó một lân cận của 0 bao gồm các hàm $f$ thỏa mãn một quan hệ $|f(t)| \leq \varepsilon g(t)$, trong đó $g$ là một hàm ở mọi nơi $> 0$ và có thể thay đổi theo lân cận. Mặt khác, trước năm 1930, người ta nhận thấy rằng những khái niệm như hội tụ đơn giản, hội tụ theo độ đo đối với các hàm đo được, hoặc hội tụ compact đối với các hàm nguyên, không thể được định nghĩa bằng một chuẩn; và năm 1926, Fréchet nhận thấy rằng các không gian vectơ thuộc loại này có thể mêtric hóa được và đầy đủ. Nhưng lý thuyết về những không gian tổng quát hơn này chỉ có thể được phát triển có hiệu quả khi gắn với ý tưởng về tính lồi. Khái niệm sau (đã xuất hiện trong công trình của Helly) là đối tượng của những nghiên cứu do Banach và các học trò của ông thực hiện, những người đã nhận ra khả năng giải thích hình học một số kết quả của lý thuyết các không gian định chuẩn, do đó chuẩn bị con đường cho một định nghĩa tổng quát về các không gian lồi địa phương, được Kolmogoroff và J. von Neumann đưa ra năm 1935. Lý thuyết về những không gian này và đặc biệt là các vấn đề liên quan đến đối ngẫu, phần lớn được phát triển trong những năm 1950, và trong Sách này chúng tôi đã trình bày các kết quả cốt yếu của nghiên cứu này. Về điểm này, cần chỉ ra, một mặt, sự tiến bộ về tính đơn giản và tính tổng quát, có được nhờ việc tập trung vào những khái niệm cơ bản của Tôpô tổng quát được phát triển trong khoảng 1930 đến 1940; và mặt khác, tầm quan trọng của khái niệm tập bị chặn, được Kolmogoroff và von Neumann đưa vào năm 1935, mà vai trò cơ bản trong lý thuyết đối ngẫu đã được làm sáng tỏ qua các công trình của Mackey (XIV) và Grothendieck (XVIII). Cuối cùng, chắc chắn rằng động lực chính thúc đẩy những nghiên cứu này đến từ những khả năng ứng dụng mới vào Giải tích trong các lĩnh vực mà lý thuyết của Banach không hoạt động: về điểm này, chúng tôi nhắc đến lý thuyết các không gian dãy được phát triển từ năm 1934 bởi Köthe, Toeplitz và các học trò của họ trong một loạt hồi ký (XV), việc tập trung vào lý thuyết « các phiếm hàm giải tích » của Fantappié, và trên hết là lý thuyết các phân bố của L. Schwartz (XVI), trong đó lý thuyết hiện đại về các không gian lồi địa phương đã tìm thấy một lĩnh vực ứng dụng chắc chắn còn lâu mới cạn kiệt.

Thư mục

(I) C. Sturm : a) Về các phương trình vi phân tuyến tính cấp hai, Journ. de Math. (1), t. I (1836), p. 106-186 ; b) Về một lớp các phép toán sai phân riêng phần, ibid., p. 373-444.
(II) J. Liouville : a) Về sự khai triển các hàm hoặc các phần của hàm thành các chuỗi mà các số hạng khác nhau của chúng bị buộc phải thỏa mãn cùng một phương trình vi phân cấp hai chứa một tham số biến thiên, Journ. de Math. (1), t. I (1836), p. 253-265, t. II (1837), p. 16-35 và 418-436 ; b) Về một định lý của ông Sturm và liên quan đến một lớp các hàm siêu việt, ibid., t. I (1836), p. 269-277.
(III) J. P. Gram. Ueber die Entwickelung reeller Functionen in Reihen mittelst der Methode der kleinsten Quadrate, J. de Crelle, t. XCIV (1883), p. 41-73.
(IV) H. Minkowski : a) Geometrie der Zahlen, 1re éd., Leipzig (Teubner), 1896 ; b) Theorie der konvexen Körper, Gesammelte Abhandlungen, t. II, p. 131-229, Leipzig-Berlin (Teubner), 1911. (Tái bản, New York (Chelsea), 1967.)
(V) H. Poincaré : a) Về các phương trình của Vật lý toán học, Rend. Palermo, t. VIII (1894), p. 57-156 (= Œuvres, t. IX, p. 123-196, Paris (Gauthier-Villars), 1954) ; b) Phương pháp Neumann và bài toán Dirichlet, Acta Mathematica, t. XX (1896), p. 59-142 (= Œuvres, t. IX, p. 202-272, Paris (Gauthier-Villars), 1954).
(VI) I. Fredholm, Về một lớp các phương trình hàm, Acta Mathematica, t. XXVII (1903), p. 365-390.
(VII) D. Hilbert, Grundzüge einer allgemeinen Theorie der linearen Integralgleichungen, New York (Chelsea), 1953 (= Gött. Nachr., 1904, 1905, 1906, 1910).
(VIII) E. Schmidt : a) Zur Theorie der linearen und nichtlinearen Integralgleichungen. I. Teil : Entwicklung willkürlicher Funktionen nach Systemen vorgeschriebener, Math. Ann., t. LXIII (1907), p. 433-476 ; b) Ueber die Auflösung linearer Gleichungen mit unendlich vielen Unbekannten, Rend. Palermo, t. XXV (1908), p. 53-77.
(IX) F. Riesz : a) Untersuchungen über Systeme integrierbarer Funktionen, Math. Ann., t. LXIX (1910), p. 449-497 ; b) Về một số hệ phương trình tích phân kỳ dị, Ann. Ec. Norm. Sup. (3), t. XXVIII (1911), p. 33-62 ; c) Các hệ phương trình tuyến tính với vô hạn ẩn, Paris (Gauthier-Villars), 1913 ; d) Ueber lineare Funktionalgleichungen, Acta Mathematica, t. XLI (1918), p. 71-98 ; e) Zur Theorie des Hilbertschen Raumes, Acta litt. ac scient. (Szeged), t. VII (1934-35), p. 34-38.
(X) E. Helly, Ueber Systeme linearer Gleichungen mit unendlich vielen Unbekannten, Monatshefte für Math. und Phys., t. XXXI (1921), p. 60-91.
(XI) H. Hahn, Ueber lineare Gleichungssysteme in linearen Räumen, J. de Crelle, t. CLVII (1927), p. 214-229.
(XII) S. Banach : a) Về bài toán đo, Fund. Math., t. IV (1923), p. 7-33 ; b) Về các phiếm hàm tuyến tính, Studia Math., t. I (1929), p. 211-216 và 223-239 ; c) Lý thuyết các phép toán tuyến tính, Warszawa, 1932. (Tái bản, New York (Chelsea), 1963.)
(XIII) S. Banach và H. Steinhaus, Về nguyên lý ngưng tụ các kỳ dị, Fund. Math., t. IX (1927), p. 50-61.
(XIV) G. W. Mackey : a) On infinite-dimensional linear spaces, Trans. Amer. Math. Soc., t. LVII (1945), p. 155-207 ; b) On convex topological spaces, Trans. Amer. Math. Soc., t. LX (1946), p. 519-537.
(XV) G. Köthe, Neubegründung der Theorie der vollkommenen Räume, Math. Nachr., t. IV (1951), p. 70-80.
(XVI) L. Schwartz, Théorie des distributions, 2e édition, Paris (Hermann), 1966.
(XVII) J. Lindenstrauss và L. Tzafriri, Classical Banach spaces, t. I, Berlin-Heidelberg-New York (Springer), 1977.
(XVIII) A. Grothendieck : a) Produits tensoriels topologiques et espaces nucléaires, Mem. Amer. Math. Soc., n° 16 (1955) ; b) Espaces vectoriels topologiques, 3e éd., São Paulo (Publ. Soc. Mat. São Paulo), 1964.

Chỉ mục ký hiệu

Các số tham chiếu chỉ chương và trang (và đôi khi, bài tập).

$|\xi|,\ \|x\| :$ I, p. 3.
$\mathcal{B}(I;\ K),\ \mathcal{B}_K(I),\ \ell^\infty_K(I),\ \ell^1_K(I),\ \mathcal{B}(I),\ \ell^1(I) :$ I, p. 4.
$E_A$ (A là một tập hợp lồi đối xứng trong một không gian vectơ thực E) : II, p. 26.
$\langle x,\ y \rangle :$ II, p. 42.
$\sigma(F,\ G) :$ II, p. 42.
$M^\circ,\ M^{\circ\circ} :$ II, p. 44.
$^t u$ (u là một ánh xạ tuyến tính) : II, p. 46.
$\mathcal{R}(X) :$ III, p. 9.
$\mathcal{C}^\infty(U) :$ III, p. 9.
$\mathcal{C}_H^\infty(U),\ \mathcal{C}_0^\infty(U) :$ III, p. 9.
$\mathcal{G}_{s,M}(I),\ \mathcal{G}_s(I),\ \mathcal{C}(I) :$ III, p. 10.
$\mathcal{H}(U),\ \mathcal{H}(L)$ (U là một tập con mở của $\mathbf{C}^n$, L là một tập con compact của $\mathbf{C}^n$) : III, p. 10.
$\mathcal{L}(E;\ F) :$ III, p. 13.
$\mathcal{L}_\varepsilon(E;\ F) :$ III, p. 13.
$\mathcal{L}_s(E;\ F),\ \mathcal{L}_c(E;\ F),\ \mathcal{L}_{pc}(E;\ F),\ \mathcal{L}_{cc}(E;\ F),\ \mathcal{L}_b(E;\ F) :$ III, p. 14.
$E',\ E'_\varepsilon,\ E'_s,\ E'_c,\ E'_{pc},\ E'_{cc},\ E'_b :$ III, p. 14.
$\mathcal{L}(E),\ \mathcal{L}_\varepsilon(E),\ \mathcal{L}_s(E),\ \mathcal{L}_c(E),\ \mathcal{L}_{pc}(E),\ \mathcal{L}_{cc}(E),\ \mathcal{L}_b(E) :$ III, p. 14.
$p_M$ (p là một bán chuẩn, M là một tập con bị chặn) : III, p. 14.
$\mathcal{C}_0(\mathbf{R}) :$ III, p. 18.
$\tau(E,\ F) :$ IV, p. 2.
$\beta(E,\ F) :$ IV, p. 4.
$c_E :$ IV, p. 14.
$\ell^\infty(\mathbf{N}) :$ IV, p. 17
$c_0(\mathbf{N}),\ \ell^1(\mathbf{N}) :$ IV, p. 18.
$S(E) :$ IV, p. 26.
$H_p :$ IV, p. 26.
$E_\sigma :$ IV, p. 32.
$\mathcal{C}_s(X) :$ IV, p. 33.
$\mathcal{C}^b(X),\ \mathcal{C}(X) :$ IV, p. 36.
$\mathcal{B}(X;\ \mathbf{R}) :$ IV, p. 40.
$\mathrm{Ind}(u)$ (u là một toán tử Fredholm) : IV, p. 66, Bài tập 21.
$\xi :$ V, p. 1.
$\ell^2,\ \ell^2(\mathbf{N}) :$ V, p. 4.
$E_{(c)} :$ V, p. 4.
$\langle x|y \rangle,\ \|x\| = \langle x|x \rangle^{1/2},\ (x|y) = \langle y|x \rangle :$ V, p. 5.
$E$ (E là một không gian tiền Hilbert phức) : V, p. 6.
$\mathcal{H}^s$ (không gian Sobolev) : V, p. 6.
$H^2(D) :$ V, p. 7.
$\mathcal{C}_0^1(U) :$ V, p. 8.
$p_H$ (H là một tập hợp lồi tách được và đầy đủ trong một không gian tiền Hilbert) : V, p. 10.
$x^*$ (x là một vectơ của một không gian Hilbert) : V, p. 15 và p. 40.
$\bigoplus_{i \in I} E_i :$ V, p. 18.
$E_1 \oplus E_2 \oplus \cdots \oplus E_n$ (E_i là các không gian Hilbert) : V, p. 18.
$\ell^2_E(I),\ \ell^2(\hat{I})$ (E là một không gian Hilbert) : V, p. 18.

$E_1 \otimes_2 E_2, \|z\|_2 (z \in E_1 \otimes_2 E_2) :$ V, p. 26.
$E_1 \otimes_2 E_2 \otimes_2 \cdots \otimes_2 E_n, \bigotimes_{i=1}^n E_i, \|z\|_2 \left( z \in \bigotimes_{i=1}^n E_i \right) :$ V, p. 27.
$E_1 \hat{\otimes}_2 E_2 \hat{\otimes}_2 \cdots \hat{\otimes}_2 E_n, \bigotimes_{1 \leq i \leq n} E_i :$ V, p. 28
$u_1 \hat{\otimes}_2 u_2 \hat{\otimes}_2 \cdots \hat{\otimes}_2 u_n$ (u_i là các ánh xạ tuyến tính) : V, p. 28.
$\hat{T}^n(E), E^{\hat{\otimes}_n} :$ V, p. 29.
$\hat{S}^n(E), \hat{S}(E) :$ V, p. 30.
$\hat{T}^n(u), \hat{S}^n(u)$ (u là một ánh xạ tuyến tính) : V, p. 31 and p. 32.
$\hat{\Lambda}^n(E), \hat{\Lambda}(E) :$ V, p. 33.
$\hat{\Lambda}^n(u)$ (u là một ánh xạ tuyến tính) : V, p. 34.
$v.u, vu$ (u, v là các ánh xạ tuyến tính) : V, p. 37.
$u^*$ (u là một ánh xạ tuyến tính) : V, p. 38.
$\mathcal{H}(E)$ (E là một không gian Hilbert) : V, p. 44.
$u \geq 0$ (u là một tự đồng cấu của một không gian Hilbert) : V, p. 45.
$\mathcal{L}_+(E) :$ V, p. 45.
$u \geq v$ (u, v trong $\mathcal{L}(E)$, E là một không gian Hilbert) : V, p. 45.
$\tau(u)$ (u là một tự đồng cấu hạng hữu hạn) : V, p. 48.
$\mathrm{Tr}(u)$ ($u \geq 0$ trong $\mathcal{L}(E)$) : V, p. 49.
$\mathcal{L}^1(E)$ (E là một không gian Hilbert) : V, p. 51.
$\mathcal{L}^2(E; F), \mathcal{L}^2(E)$ (E, F là các không gian Hilbert) : V, p. 52.
$\|u\|_2$ ($u \in \mathcal{L}(E; F)$, E, F là các không gian Hilbert) : V, p. 52.
$\mathrm{Tr}(\mathbf{Q}/H)$ (Q, H là các dạng toàn phương dương) : V, p. 57.

Chỉ mục thuật ngữ

Tập hấp thụ, sự hấp thụ của một tập hợp bởi một tập hợp khác : I, p. 7.
Bornôlôgi thích nghi : III, p. 3.
Liên hợp : V, p. 38.
Phép biến đổi afin : IV, p. 39.
Liên kết (không gian vectơ Hausdorff) với một không gian vectơ tôpô : I, p. 4.

Bao cân bằng lồi đóng của một tập hợp : II, p. 13 and p. 62.
Lõi cân bằng của một tập hợp : I, p. 7.
Bao cân bằng của một tập hợp : I, p. 7.
Tập cân bằng : I, p. 6.
Định lý Banach-Dieudonné : IV, p. 24.
Định lý Banach-Saks-Kakutani : V, p. 68, exerc. 33.
Không gian Banach : I, p. 5.
Định lý Banach-Steinhaus : III, p. 25.
Định lý Banach : I, p. 17.
Thùng : III, p. 24.
Không gian đẫy : III, p. 24.
Cơ sở của một bornôlôgi : III, p. 1.
Cơ sở (đại số) của một không gian Hilbert : V, p. 22.
Cơ sở (Banach) : IV, p. 69, exerc. 14.
Cơ sở (Banach đầy đủ, Banach co) : IV, p. 70, exerc. 15.
Cơ sở (trực chuẩn) : V, p. 22.
Cơ sở (Banach không điều kiện) : IV, p. 71, exerc. 16.
Bất đẳng thức Bessel : V, p. 21.
Đối ngẫu kép : IV, p. 14.
Định lý lưỡng cực : II, p. 44.
Định lý Birkhoff-Alaoglu : V, p. 78, exerc. 13.
Định lý Bishop-Phelps : II, p. 77, exerc. 4.
Không gian lồi địa phương bornôlôgi : III, p. 12.
Bornôlôgi : III, p. 1.
Bornôlôgi (thích nghi) : III, p. 3.
Bornôlôgi (chính tắc) : III, p. 3.
Bornôlôgi (lồi) : III, p. 2.
Bornôlôgi sinh bởi một họ tập hợp : III, p. 1.
Bornôlôgi (tích) : III, p. 2.
Tập hấp thụ bornôlôgi : III, p. 39, exerc. 11.
Tập bị chặn : III, p. 2 and p. 37, exerc. 1.

Bornôlôgi chính tắc : III, p. 3.
Ánh xạ chính tắc của $\bigoplus_{i \in I} E_i'$ vào $\left( \prod_{i \in I} E_i \right)'$ : IV, p. 13.
Ánh xạ chính tắc của E vào $E''$ : IV, p. 14.
Ánh xạ chính tắc của E lên $E'$ (E là một không gian Hilbert) : V, p. 15.
Tôpô chính tắc trên một không gian vectơ hữu hạn chiều : I, p. 2.
Nắp : II, p. 57.
Bất đẳng thức Cauchy-Schwarz : V, p. 3.
Định lý đồ thị đóng : I, p. 19.
Các nửa không gian đóng được xác định bởi một siêu phẳng đóng : II, p. 15.
Đồng biên : IV, p. 72, exerc. 3.
1-đồng chu trình (liên tục) : IV, p. 72, exerc. 3.

Ánh xạ tuyến tính compact : III, p. 6.
Tôpô và cấu trúc tương thích của một không gian vectơ có thứ tự : II, p. 15.
Cấu trúc không gian vectơ và tiền thứ tự tương thích : II, p. 12.
Cấu trúc không gian vectơ và tôpô tương thích : III, p. 1.
Tương thích với đối ngẫu (tôpô lồi địa phương) : IV, p. 1.
Phần bù (trực giao) : V, p. 13.
Không gian vectơ tôpô đầy đủ : I, p. 5.
Sự hoàn thành của một không gian tiền Hilbert Hausdorff : V, p. 8.
Sự hoàn thành của một không gian vectơ tôpô Hausdorff : I, p. 6.
Dạng tuyến tính phức : II, p. 61.
Không gian con afin phức : II, p. 61.
Không gian lồi địa phương phức : II, p. 62.
Phức hóa (không gian tiền Hilbert) : V, p. 5.
Không gian vectơ tôpô đã phức hóa : II, p. 62.
Hàm lõm : II, p. 17.
Nón (tiệm cận) : II, p. 67.
Nón (lồi) sinh bởi một tập hợp : II, p. 11.
Nón (nhọn và không nhọn) : II, p. 10.
Nón (đa diện) : II, p. 91.
Nón (lồi chính nhọn) : II, p. 11.
Không gian liên hợp của một không gian tiền Hilbert phức : V, p. 6.
Bao lồi cân bằng của một tập hợp : II, p. 10 and p. 62.
Bornôlôgi lồi : III, p. 2.
Bao lồi đóng của một tập hợp : II, p. 13.
Hàm lồi : II, p. 17.
Tập lồi : II, p. 7 and p. 62.
Bao lồi (đối xứng) của một tập hợp : II, p. 10.
Tọa độ theo một cơ sở trực chuẩn : V, p. 22.
Lõi (cân bằng) của một tập hợp : I, p. 7.

Mật độ cấp : V, p. 7.
Chiều (Hilbert) : V, p. 24.
Chiều của một tập lồi : II, p. 10.
Không gian Dirichlet : V, p. 8.
Tập xa : IV, p. 72, exerc. 1.
Không gian đặc biệt : IV, p. 52, exerc. 4.
Đối ngẫu (đại số) của một không gian vectơ tôpô thực : II, p. 42.
Đối ngẫu của một không gian lồi địa phương (thực hoặc phức) : III, p. 14.
Đối ngẫu của một không gian vectơ tôpô thực : II, p. 42.
Đối ngẫu (yếu, mạnh) : III, p. 14.
Đối ngẫu tách trong F, đối ngẫu tách : II, p. 41.
Đối ngẫu (giữa các không gian vectơ) : II, p. 40.
Định lý Dvoretzky-Rogers : V, p. 63, exerc. 14.

Định lý Eberlein : IV, p. 35.
Định lý D. Edwards : II, p. 94, exerc. 41.
Tự đồng cấu (Hermit) : V, p. 44.
Tự đồng cấu (chuẩn) : V, p. 43.
Tự đồng cấu (dương) : V, p. 45.
Bao của một tập hợp (cân bằng) : I, p. 7.
Bao của một tập hợp (cân bằng lồi) : II, p. 10.
Bao của một tập hợp (cân bằng lồi đóng) : II, p. 13 and p. 62.
Bao của một tập hợp (đóng lồi) : II, p. 13.
Bao của một tập hợp (lồi) : II, p. 9.
Bao của một tập hợp (đối xứng lồi) : II, p. 10.
Bao của một tập hợp (đối xứng lồi đóng) : II, p. 13.
Tập \mathcal{S}-đẳng hạ liên tục, \mathfrak{T}-đẳng hạ liên tục, (\mathcal{S}, \mathfrak{T})-đẳng hạ liên tục : III, p. 47, exerc. 7.

Sự vét cạn của một không gian lồi địa phương Hausdorff, không gian có thể vét cạn : III, p. 49, bài tập 1.
Phần tử sinh cực biên của một nón lồi : II, p. 57.
Điểm cực biên của một tập lồi : II, p. 54.

Mặt (facet) : II, p. 87, bài tập 3.
Mặt (đối ngẫu) : II, p. 87, bài tập 6.
Họ (trực chuẩn) : V, p. 21.
Họ (độc lập tôpô) : I, p. 11.
Tập lọc các nửa chuẩn : II, p. 3.
Tôpô lồi địa phương cuối : II, p. 27.
Không gian con cuối : V, p. 41.
Các không gian Fock : V, p. 32 và p. 34.
Dạng (song tuyến tính) đặt hai không gian trong đối ngẫu : II, p. 40.
Dạng (tuyến tính phức, tuyến tính thực) : II, p. 61.
Dạng (Hermit) : V, p. 1.
Dạng (Hermit dương) : V, p. 2.
Dạng (tuyến tính dương) : II, p. 13.
Dạng (Hermit tách) liên kết với một dạng Hermit : V, p. 2.
Không gian Fréchet : II, p. 24 và p. 63.
Hàm (lõm, lồi, lõm ngặt, lồi ngặt) : II, p. 16-17.
Hàm (xác định dương) : V, p. 8.
Hàm (thuần nhất dương), hàm dưới tuyến tính : II, p. 19-20.
Hệ cơ bản các nửa chuẩn : II, p. 3.

Gauge của một tập lồi : II, p. 20.
Không gian Gaussian : V, p. 32.
Được sinh (bornology) bởi một họ các tập hợp : III, p. 1.
Phần tử sinh (cực biên) của một nón lồi : II, p. 57.
Các không gian Gevrey : III, p. 10.
Định thức Gram : V, p. 71, bài tập 7.
Định lý Grothendieck : III, p. 20.
Nhóm trên đó một trung bình có thể được xác định : IV, p. 72, bài tập 4.

Định lý Haar : II, p. 83, bài tập 8.
Các bất đẳng thức Hadamard : V, p. 37.
Định lý Hahn-Banach : II, p. 22, p. 36 và p. 63.
Các nửa không gian (đóng, mở) được xác định bởi một siêu phẳng đóng : II, p. 15.
Không gian Hardy : V, p. 7.
Phép hoàn thành Hausdorff của một không gian vectơ tôpô : I, p. 6.
Không gian vectơ Hausdorff liên kết với một không gian vectơ tôpô : I, p. 4.
Định lý Helly : II, p. 68, bài tập 21.
Tự đồng cấu Hermit : V, p. 44.
Ánh xạ Hilbert-Schmidt : V, p. 52.
Không gian Hilbert, không gian Hilbert : V, p. 6.
Siêu phẳng (đỡ) của một tập hợp : II, p. 37.
\mathcal{S}-bán liên tục, \mathcal{T}-bán liên tục, ánh xạ song tuyến tính (\mathcal{S}, \mathcal{T})-bán liên tục : III, p. 30.

Chỉ số của một toán tử Fredholm : IV, p. 66, bài tập 21.
Cấu trúc tiền Hilbert cảm sinh trên một không gian con vectơ : V, p. 6.
Giới hạn quy nạp của các không gian lồi địa phương hoặc các tôpô : II, p. 29.
Các bất đẳng thức (của Hadamard) : V, p. 37.
Bất đẳng thức (của Bessel) : V, p. 21.
Bất đẳng thức (Cauchy-Schwarz) : V, p. 3.
Không gian hạ-barrel : III, p. 44, bài tập 7.
Không gian con ban đầu : V, p. 41.
Tôpô ban đầu : IV, p. 4.
Điểm trong của một tập lồi : II, p. 26.

Định lý James-Klee : IV, p. 57, bài tập 25.
Không gian của R. C. James : IV, p. 71, bài tập 18.

Định lý Krein-Milman : II, p. 55.
Định lý Krein : IV, p. 37.

Đa thức Legendre : V, p. 24.
Không gian phức lồi địa phương : II, p. 62.
Không gian thực lồi địa phương : II, p. 23.
Tôpô lồi địa phương : II, p. 23 và p. 62.

Định lý Mackey : IV, p. 2.
Tôpô Mackey : IV, p. 2.
Ánh xạ (Hilbert-Schmidt) : V, p. 52.
Định lý Markoff-Kakutani : IV, p. 39.
Ma trận (của Hilbert) : V, p. 75, bài tập 3.
Ma trận đối với các cơ sở trực chuẩn : V, p. 22.
Trung bình : IV, p. 40.
Không gian vectơ tôpô đo được : I, p. 16.
Kiểu cực tiểu (của không gian) : II, p. 85, bài tập 13.
Không gian Montel : IV, p. 18.

Tự đồng cấu chuẩn tắc : V, p. 43.

Các nửa không gian mở được xác định bởi một siêu phẳng đóng : II, p. 15.
Toán tử (Fredholm) : IV, p. 66, bài tập 21.
Toán tử (unitary) : V, p. 41.
Không gian vectơ có thứ tự : II, p. 12.
Phần trực giao của một không gian con đối với các không gian trong đối ngẫu : II, p. 44.
Phép chiếu trực giao, phép chiếu trực giao : V, p. 13.
Các tập hợp trực giao trong một không gian tiền Hilbert : V, p. 13.
Các tập hợp trực giao trong các không gian trong đối ngẫu : II, p. 41.
Trực giao với một tập con trong một không gian tiền Hilbert : V, p. 13.
Các vectơ trực giao đối với một đối ngẫu : II, p. 41.
Các vectơ trực giao trong một không gian tiền Hilbert : V, p. 5.
Cơ sở trực chuẩn : V, p. 22.
Tập hợp, họ trực chuẩn : V, p. 21.
Sự trực chuẩn hóa : V, p. 24.
Phép chiếu trực giao (ban đầu, cuối) : V, p. 41.

Tập lồi parabol : II, p. 67, bài tập 17.
Quan hệ Parseval : V, p. 22.
Ánh xạ đẳng cự từng phần : V, p. 42.
Nón nhọn : II, p. 10.
Các điểm (lộ ra, của tính lồi ngặt) : II, p. 88, bài tập 6.
Các điểm ở cùng phía, ở cùng phía một cách ngặt, của một siêu phẳng : II, p. 9.
Phân tích cực của một tự đồng cấu Hilbert-Schmidt : V, p. 79, bài tập 14.
Đối cực của một tập hợp : II, p. 44 và 64.
Các công thức phân cực : V, p. 2.
Đa diện : II, p. 90, bài tập 24.
Tự đồng cấu dương : V, p. 45.
Dạng Hermit dương : V, p. 2.
Hàm thuần nhất dương : II, p. 19.
Tiền đối ngẫu : IV, p. 56, bài tập 23.
Nửa chuẩn tiền Hilbert : V, p. 4.
Không gian tiền Hilbert : V, p. 4.
Không gian vectơ tiền thứ tự : II, p. 12.
Nguyên lý ngưng tụ các điểm kỳ dị : III, p. 42, bài tập 10.

Bornology tích : III, p. 2.
Phép chiếu lên một tập lồi : V, p. 11.
Phép chiếu (trực giao) : V, p. 13.
Nón lồi nhọn thực sự : II, p. 11.
Định lý Pythagoras : V, p. 12.

Không gian gần đầy đủ : III, p. 8.

Dạng tuyến tính thực, đa tạp tuyến tính thực : II, p. 61.
Không gian thực lồi địa phương : II, p. 23.
Không gian phản xạ : IV, p. 16.
Không gian bị chặn tương đối : III, p. 43, bài tập 6.
Biểu diễn (unitary) : IV, p. 44.
Định lý Ryll-Nardzewski : IV, p. 43.

Tích vô hướng : V, p. 5.
Bình phương vô hướng : V, p. 5.
Đoạn (đóng, mở, mở tại x và đóng tại y) : II, p. 7.
Nửa tự đẳng cấu của các không gian tiền Hilbert : V, p. 6.
Không gian nửa thùng : IV, p. 21.
Không gian nửa đầy đủ : III, p. 7.
Nửa chuẩn : II, p. 1.
Không gian nửa chuẩn : II, p. 2.
Nửa chuẩn (tiền Hilbert) : V, p. 4.
Không gian nửa phản xạ : IV, p. 15.
Hoàn thiện tách biệt của một không gian tiền Hilbert : V, p. 8.
Hoàn thiện tách biệt của một không gian vectơ tôpô : I, p. 6.
Được phân cách (các tập hợp) bởi một siêu phẳng đóng : II, p. 37.
Ánh xạ song tuyến tính liên tục riêng rẽ : III, p. 28.
Riêng rẽ đều liên tục : III, p. 47.
Đối ngẫu phân tách : II, p. 41.
Phía của một siêu phẳng (các điểm cùng phía, hoàn toàn cùng phía) : II, p. 8.
Đơn hình : II, p. 71, bài tập 41.
Định lý Šmulian : IV, p. 36.
Không gian Sobolev : V, p. 6.
Đáy của một nón : II, p. 60.
Không gian (DF) : IV, p. 57, bài tập 2.
Không gian (vectơ tôpô) : I, p. 1.
Không gian (yếu) : II, p. 42.
Bình phương (vô hướng) : V, p. 5.
Tập hợp sao : II, p. 65, bài tập 1.
Giới hạn quy nạp ngặt của một dãy các không gian lồi địa phương, các tôpô : II, p. 33.
Hàm lõm ngặt, hàm lồi ngặt : II, p. 16-17.
Được phân cách ngặt (các tập hợp) bởi một siêu phẳng đóng : II, p. 37.
Đối ngẫu mạnh : III, p. 14.
Tập con bị chặn mạnh của E′ : III, p. 14.
Hàm dưới tuyến tính : II, p. 20.
Không gian con (đích, ban đầu) của một ánh xạ tuyến tính liên tục : V, p. 41.
Không gian con (tiền Hilbert) : V, p. 6.
Tổng ngoại Hilbert của các không gian Hilbert : V, p. 18.
Tổng Hilbert của các không gian con vectơ : V, p. 18.
Tổng trực tiếp tôpô của các không gian lồi địa phương hoặc các tôpô : II, p. 30.
Đa tạp đỡ : II, p. 87, bài tập 3.
Bao lồi đóng đối xứng của một tập hợp : II, p. 13.

Định lý Tchebycheff : II, p. 84, bài tập 8.
Tích tenxơ Hilbert : V, p. 28.
Tích tenxơ của các không gian tiền Hilbert : V, p. 26-27.

Tập hợp, họ độc lập tôpô : I, p. 12 và p. 11.
$\mathcal{S}$-tôpô : III, p. 13 và IV, p. 2.
Tôpô tương thích với một cấu trúc không gian vectơ có thứ tự : II, p. 15.
Tôpô tương thích với một cấu trúc không gian vectơ : I, p. 1.
Tôpô được xác định bởi một nửa chuẩn, bởi một tập các nửa chuẩn : II, p. 2-3.
Tôpô (ban đầu) : IV, p. 4.
Tôpô (lồi địa phương) : II, p. 23 và p. 62.
Tôpô (Mackey) : IV, p. 2.
Tôpô của hội tụ đơn, compact, tiền compact, compact lồi, bị chặn : III, p. 14.
Tôpô (yếu) : II, p. 42.
Tôpô (suy yếu) : IV, p. 4.
Tập hợp toàn phần : I, p. 11.
Vết của một tự đồng cấu dương liên tục : V, p. 49.
Vết của một dạng toàn phương dương đối với một dạng khác : V, p. 57.
Phép biến đổi afin : IV, p. 39.
Chuyển vị của một ánh xạ tuyến tính liên tục : II, p. 46 và IV, p. 6.

Không gian siêu bornơ : III, p. 45, bài tập 19.
Siêu chuẩn : I, p. 26, bài tập 12.
Siêu nửa chuẩn : II, p. 2.
Toán tử đơn nhất : V, p. 41.
Biểu diễn đơn nhất : IV, p. 44.
Nón không điểm : II, p. 10.

Đa tạp (tuyến tính phức, tuyến tính thực) : II, p. 61.
Đa tạp (đỡ) : II, p. 87, bài tập 3.

Đối ngẫu yếu : III, p. 14.
Tôpô yếu, không gian yếu : II, p. 42.
Tôpô suy yếu : IV, p. 4.
Bị chặn yếu : III, p. 14.

Tóm tắt một số tính chất quan trọng của các không gian Banach

Để tiện cho người đọc, các kết quả chính về các không gian chuẩn và, đặc biệt hơn, về các không gian Banach được tập hợp ở đây. Trường vô hướng K hoặc là $\mathbf{R}$ hoặc là $\mathbf{C}$.

**Không gian ánh xạ tuyến tính ; đối ngẫu**

1) Cho E và F là hai không gian chuẩn. Một ánh xạ tuyến tính $u$ từ E vào F là liên tục khi và chỉ khi

$$
\|u\| = \sup_{\|x\| \leq 1} \|u(x)\|
$$

là hữu hạn. Ánh xạ $u \mapsto \|u\|$ là một chuẩn trên không gian vectơ $\mathcal{L}(E; F)$ của các ánh xạ tuyến tính liên tục từ E vào F.

Cho F là một không gian Banach. Khi đó $\mathcal{L}(E; F)$ cũng là một không gian Banach. Hoàn thiện $\hat{E}$ của E là một không gian Banach và ánh xạ $u \mapsto u|E$ là một đẳng cự song ánh từ $\mathcal{L}(\hat{E}; F)$ lên $\mathcal{L}(E; F)$.

2) Cho E là một không gian chuẩn. Viết $E' = \mathcal{L}(E; K)$, trong đó K mang chuẩn $\lambda \mapsto |\lambda|$. Không gian Banach $E'$ được gọi là *đối ngẫu* của E, và đối ngẫu $E''$ của $E'$ được gọi là *đối ngẫu kép* của E.

Ký hiệu $\sigma(E, E')$ là tôpô thô nhất trên E sao cho mọi phiếm hàm tuyến tính $x' \in E'$ đều liên tục; nó được gọi là tôpô *suy yếu* của E. Ký hiệu $\sigma(E', E)$ là tôpô thô nhất trên $E'$ sao cho các phiếm hàm tuyến tính $x' \mapsto \langle x', x \rangle$ trên $E'$, khi x chạy trong E, đều liên tục; khi đó $\sigma(E', E)$ được gọi là tôpô *yếu* trên $E'$. Tôpô trên $E'$ suy ra từ chuẩn được gọi là tôpô *mạnh*.

3) Cho E là một không gian chuẩn và M là một không gian con vectơ đóng của E. Gọi π là ánh xạ chính tắc của E lên $E/M$. Một chuẩn trên không gian vectơ $E/M$ được xác định bởi

$$
\|\xi\| = \inf_{\pi(x) = \xi} \|x\|.
$$

Khi E là một không gian Banach, thì M và $E/M$ cũng vậy. Với mọi không gian chuẩn F, ánh xạ tuyến tính $u \mapsto u \circ \pi$ từ $\mathcal{L}(E/M; F)$ vào $\mathcal{L}(E; F)$ là đẳng cự.

4) Cho E là một không gian chuẩn. Với mọi $x' \in E'$, theo định nghĩa ta có

$$
\|x'\| = \sup_{\substack{\|x\| \leq 1 \\ x \in E}} |\langle x', x \rangle|.
$$

Hơn nữa (định lý Hahn-Banach), ta có

$$
\|x\| = \sup_{\substack{\|x'\| \leq 1 \\ x' \in E'}} |\langle x', x \rangle|
$$

với mọi $x \in E$. Nói cách khác, ánh xạ chính tắc của $E$ vào đối ngẫu kép $E''$ là đẳng cự.

Đối cực và trực giao

5) Cho $E$ là một không gian chuẩn. Với mọi tập con A của E (tương ứng B của $E'$), đối cực của A (tương ứng B) ký hiệu bởi $A^\circ$ (tương ứng $B^\circ$) là tập hợp các $x' \in E'$ (tương ứng $x \in E$) sao cho

$$
\Re \langle x', x \rangle \geq -1
$$

với mọi $x \in A$ (resp. $x' \in B$). Khi $A$ (resp. $B$) là một không gian con vectơ, quan hệ (5) tương đương với $\langle x', x \rangle = 0$, và khi đó ta nói rằng $A^\circ$ (resp. $B^\circ$) là *trực giao* của $A$ (resp. $B$).

6) (« Định lý lưỡng cực »). Cho $E$ là một không gian chuẩn. Cho $A$ (resp. $B$) là một tập con của $E$ (resp. $E'$) chứa 0. Khi đó lưỡng cực $A^{\circ \circ}$ của $A$ (resp. $B^{\circ \circ}$ của $B$) là bao đóng đối với tôpô $\sigma(E, E')$ (resp. $\sigma(E', E)$) của bao lồi của $A$ (resp. $B$).

7) Cho $A$ là một tập con của một không gian chuẩn $E$. Cho $x$ là một điểm trong bao đóng của $A$ đối với tôpô $\sigma(E, E')$. Khi đó $x$ là giới hạn (theo nghĩa chuẩn) của một dãy các điểm của bao lồi của $A$. Đặc biệt, các tập lồi của $E$ đóng trong không gian chuẩn $E$ cũng chính là các tập đóng đối với $\sigma(E, E')$.

8) Cho $E$ là một không gian chuẩn và $M$ là một không gian con vectơ của $E$. Với mọi dạng tuyến tính $u_0 \in M'$, tồn tại một dạng tuyến tính $u \in E'$ mở rộng $u_0$ và sao cho $\|u\| = \|u_0\|$. Cho $H$ là trực giao của $M$ trong $E'$; khi đó trực giao $H^\circ$ của $H$ là bao đóng của $M$ trong $E$.

Chuyển vị

9) Cho $E$ và $F$ là hai không gian chuẩn và $u \in \mathcal{L}(E; F)$. *Chuyển vị* $^t u \in \mathcal{L}(F'; E')$ của $u$ được xác định bởi quan hệ

$$
\langle u(y'), x \rangle = \langle y', u(x) \rangle \quad \text{với mọi } x \in E, \ y' \in F'.
$$

Ta có $\|^t u\| = \|u\|$. Hạt nhân của $u$ là trực giao trong $E$ của ảnh của $^t u$. Hạt nhân của $^t u$ là trực giao trong $F'$ của ảnh của $u$.

10) Cho $E$ là một không gian định chuẩn, $M$ là một không gian con vectơ đóng của $E$ và $F = E/M$. Cho $i$ là đơn ánh chính tắc của $M$ vào $E$ và cho $\pi$ là toàn cấu chính tắc của $E$ lên $F$. Khi đó $^t i$ có hạt nhân là trực giao $M^\circ$ của $M$ và cảm sinh, khi chuyển qua thương, một đẳng cự của $E'/M^\circ$ lên $M'$. Hơn nữa $^t \pi$ là một đẳng cự của $F'$ lên $M^\circ$.

Các điều kiện về tính liên tục của một ánh xạ tuyến tính

11) Cho $E$ và $F$ là hai không gian Banach và $u$ là một ánh xạ tuyến tính của $E$ vào $F$. Giả sử rằng với mọi dãy $(x_n)_{n \geq 0}$ các điểm của $E$ hội tụ về 0 và sao cho dãy $(u(x_n))_{n \geq 0}$ có một giới hạn $y$ trong $F$, thì $y$ tất yếu là 0. Khi đó $u$ là liên tục.

\* Giả sử rằng với mọi tập con compact K của E, với mọi độ đo dương $\mu$ trên K và với mọi dạng tuyến tính liên tục $y'$ trên F, hạn chế của $y' \circ u$ lên K là $\mu$-đo được. Khi đó $u$ là liên tục.*

12) Cho E và F là hai không gian Banach và $u \in \mathcal{L}(E; F)$. Khi đó hoặc $u(E)$ là thưa, hoặc $u$ là toàn ánh.

Giả sử rằng $u$ là toàn ánh. Khi đó tồn tại một số $C > 0$ sao cho, với mọi $y \in F$, tồn tại $x \in E$ với $u(x) = y$ và $\|x\| \leq C.\|y\|$. Nếu N là hạt nhân của $u$, thì $u$ cảm sinh khi chuyển qua thương một đồng phôi của $E/N$ lên F.

13) Cho E và F là hai không gian Banach. Nếu $u$ là một ánh xạ tuyến tính liên tục của E vào F là song ánh, thì $u^{-1}$ là liên tục.

14) Cho E và F là hai không gian Banach, cho $u \in \mathcal{L}(E; F)$ và $x' \in E'$. Để $x'$ thuộc ảnh của $'u$, điều kiện cần và đủ là tồn tại một số $C > 0$ sao cho

$$
|\langle x', x \rangle| \leq C.\|u(x)\|
$$

với mọi $x \in E$.

(15) Cho E và F là hai không gian Banach và $u \in \mathcal{L}(E; F)$. Để $u$ toàn ánh, điều kiện cần và đủ là tồn tại một số $C > 0$ sao cho $\| 'u(y') \| \geq C.\|y'\|$ với mọi $y' \in F'$.

Định lý Banach-Steinhaus

16) (« Định lý Banach-Steinhaus »). Cho E là một không gian Banach; F là một không gian định chuẩn và cho $(u_i)_{i \in I}$ là một họ các phần tử của $\mathcal{L}(E; F)$. Cho A là tập con của $x \in E$ sao cho $\sup_{i \in I} \|u_i(x)\| < + \infty$. Khi đó hoặc A là một tập mảnh và phần bù của nó trù mật trong E, hoặc ngược lại $\sup_{i \in I} \|u_i\| < + \infty$. Đặc biệt, nếu $A = E$ thì $\sup_{i \in I} \|u_i\| < + \infty$.

17) Cho E và F là hai không gian Banach và cho $(u_n)_{n \geq 0}$ là một dãy các phần tử của $\mathcal{L}(E; F)$. Giả sử giới hạn $u(x) = \lim_{n \to \infty} u_n(x)$ tồn tại với mọi $x \in E$. Khi đó $\sup_n \|u_n\| < + \infty$, $u$ liên tục và dãy $(u_n)$ hội tụ đều tới $u$ trên mọi tập con compact của E.

Các tính chất của tôpô yếu trên một không gian đối ngẫu

18) Cho E là một không gian Banach và B' là một tập con của E'. Các điều kiện sau là tương đương :
(i) B' được chứa trong một quả cầu của E'.
(ii) B' tương đối compact đối với tôpô $\sigma(E', E)$.
(iii) Với mọi $x \in E$, ta có $\sup_{x' \in B'} |\langle x', x \rangle| < + \infty$.

19) Cho E là một không gian Banach và cho B' là quả cầu đơn vị (đóng) của E'. Khi đó B' là compact đối với $\sigma(E', E)$. Giả sử tồn tại một tập con toàn phần đếm được của E ; khi đó B' là mêtric hóa được đối với $\sigma(E', E)$, và tồn tại một tập con đếm được của E' trù mật đối với $\sigma(E', E)$.

20) Cho E là một không gian Banach, $u$ là một dạng tuyến tính trên E' và B' là quả cầu đơn vị của E'. Các điều kiện sau là tương đương :
(i) Tồn tại $x \in E$ sao cho $u(x') = \langle x', x \rangle$ với mọi $x' \in E'$.
(ii) Hạn chế của $u$ lên B' liên tục đối với tôpô $\sigma(E', E)$.
(iii) Với mọi dãy $(x'_n)$ gồm các phần tử của E' mà tiến tới 0 đối với $\sigma(E', E)$, ta có $\lim_{n \to \infty} u(x'_n) = 0$.

21) Cho E là một không gian Banach, B' là quả cầu đơn vị của E' và C là một tập con lồi của E' (đặc biệt là một không gian vectơ con). Để C đóng đối với $\sigma(E', E)$, điều kiện cần và đủ là giao $C \cap rB'$ đóng đối với $\sigma(E', E)$ với mọi số thực $r > 0$.

Các không gian phản xạ

22) Cho E là một không gian định chuẩn, $E''$ là đối ngẫu kép của nó và i là ánh xạ chính tắc của E vào $E''$. Quả cầu đơn vị của $E''$ là bao đóng đối với $\sigma(E'', E')$ của ảnh qua i của quả cầu đơn vị của E.

Các điều kiện sau là tương đương :
(i) Ánh xạ đẳng cự $i : E \mapsto E''$ là toàn ánh.
(ii) Quả cầu đơn vị trong E là compact đối với $\sigma(E, E')$.
Khi các điều kiện này được thỏa mãn, ta nói rằng E là phản xạ.

Các tôpô tương thích với tính đối ngẫu

23) Cho E là một không gian Banach và $\mathcal{T}$ là một tôpô lồi địa phương trên E. Các điều kiện sau là tương đương :
(i) Tôpô $\mathcal{T}$ mịn hơn $\sigma(E, E')$ và thô hơn tôpô do chuẩn xác định trên E.
(ii) E' là tập hợp các dạng tuyến tính trên E liên tục đối với $\mathcal{T}$.

Giả sử các điều kiện này được thỏa mãn. Cho A là một tập con của E. Khi đó A là tương đối compact đối với $\mathcal{T}$ khi và chỉ khi mọi dãy các điểm của A đều có một điểm tụ đối với $\mathcal{T}$ trong E. Nếu điều này đúng thì bao lồi cân bằng của A là tương đối compact đối với $\mathcal{T}$.

Mục lục

CHƯƠNG I. — KHÔNG GIAN VECTƠ TÔPÔ TRÊN MỘT VÀNH CHIA CÓ GIÁ TRỊ. I. 1

§ 1. Không gian vectơ tôpô ............................................. I. 1
    1. Định nghĩa của một không gian vectơ tôpô ......................... I. 1
    2. Các không gian chuẩn trên một vành chia có giá trị ....................... I. 3
    3. Các không gian con vectơ và các không gian thương của một không gian vectơ tôpô; các tích của các không gian vectơ tôpô; các tổng trực tiếp tôpô của các không gian con ............................................. I. 4
    4. Cấu trúc đều và sự đầy đủ của một không gian vectơ tôpô ................................................................. I. 5
    5. Các lân cận của gốc trong một không gian vectơ tôpô trên một vành chia có giá trị ............................................. I. 6
    6. Các tiêu chuẩn của tính liên tục và tính liên tục đều ....................... I. 8
    7. Các tôpô ban đầu của các không gian vectơ ............................. I. 9

§ 2. Các đa tạp tuyến tính trong một không gian vectơ tôpô .................... I. 11
    1. Bao đóng của một đa tạp tuyến tính ................................. I. 11
    2. Các đường thẳng và các siêu phẳng đóng .................................. I. 12
    3. Các không gian con vectơ có số chiều hữu hạn ........................ I. 13
    4. Các không gian vectơ tôpô compact địa phương .................... I. 15

§ 3. Các không gian vectơ tôpô đo được ..................................... I. 16
    1. Các lân cận của 0 trong một không gian vectơ tôpô đo được. I. 16
    2. Các tính chất của các không gian vectơ đo được ....................... I. 17
    3. Các hàm tuyến tính liên tục trong một không gian vectơ đo được .... I. 17

Các bài tập của § 1 ............................................................. I. 22
Các bài tập của § 2 ............................................................. I. 25
Các bài tập của § 3 ............................................................. I. 28

CHƯƠNG II. — CÁC TẬP LỒI VÀ CÁC KHÔNG GIAN LỒI ĐỊA PHƯƠNG ............... II. 1

§ 1. Bán chuẩn ............................................................ II. 1
    1. Định nghĩa của các bán chuẩn ....................................... II. 1
    2. Các tôpô xác định bởi các bán chuẩn ............................. II. 2
    3. Các bán chuẩn trong các không gian thương và trong các không gian tích .......... II. 4

4. Equicontinuity criteria of multilinear mappings for topologies defined by semi-norms ............................................. II.5

§ 2. Các tập lồi ................................................................. II.7
  1. Định nghĩa của một tập lồi ............................................. II.7
  2. Các giao của các tập lồi. Các tích của các tập lồi .......... II.9
  3. Bao lồi của một tập ............................................. II.9
  4. Các nón lồi .......................................................... II.10
  5. Các không gian vectơ có thứ tự ................................................ II.12
  6. Các nón lồi trong các không gian vectơ tôpô ....................... II.13
  7. Các tôpô trên các không gian vectơ có thứ tự .............................. II.15
  8. Các hàm lồi .................................................... II.16
  9. Các phép toán trên các hàm lồi ..................................... II.18
 10. Các hàm lồi trên một tập lồi mở ....................... II.18
 11. Các bán chuẩn và các tập lồi ....................................... II.19

§ 3. Định lý Hahn-Banach (dạng giải tích) ....................... II.21
  1. Mở rộng các dạng tuyến tính dương ............................... II.21
  2. Định lý Hahn-Banach (dạng giải tích) ....................... II.22

§ 4. Các không gian lồi địa phương ............................................... II.23
  1. Định nghĩa của một không gian lồi địa phương ............................ II.23
  2. Các ví dụ về các không gian lồi địa phương ............................... II.25
  3. Các tôpô ban đầu lồi địa phương ............................... II.26
  4. Các tôpô cuối lồi địa phương ................................. II.27
  5. Tổng trực tiếp tôpô của một họ các không gian lồi địa phương. II.29
  6. Các giới hạn quy nạp của các dãy các không gian lồi địa phương ........ II.31
  7. Các nhận xét về các không gian Fréchet ....................................... II.34

§ 5. Sự tách các tập lồi .......................................... II.36
  1. Định lý Hahn-Banach (dạng hình học) ..................... II.36
  2. Sự tách các tập lồi trong một không gian vectơ tôpô ...... II.37
  3. Sự tách các tập lồi trong một không gian lồi địa phương .......... II.38
  4. Sự xấp xỉ các hàm lồi ............................... II.39

§ 6. Các tôpô yếu .................................................... II.40
  1. Các không gian vectơ đối ngẫu ................................................ II.40
  2. Các tôpô yếu ................................................... II.42
  3. Các tập cực và các không gian con trực giao ............................. II.44
  4. Sự chuyển vị của một ánh xạ tuyến tính liên tục .................. II.46
  5. Các không gian thương và các không gian con của một không gian yếu ................. II.48
  6. Các tích của các tôpô yếu ....................................... II.50
  7. Các không gian đầy đủ yếu ........................................... II.51
  8. Các nón lồi đầy đủ trong các không gian yếu ........................... II.52

§ 7. Các điểm cực biên và các sinh cực biên ............................................. II.54
    1. Các điểm cực biên của các tập lồi compact ............................................. II.54
    2. Các sinh cực biên của các nón lồi ............................................... II.57
    3. Các nón lồi có đáy compact ..................................................... II.59

§ 8. Các không gian lồi địa phương phức ............................................................ II.60
    1. Các không gian vectơ tôpô trên C ..................................................... II.60
    2. Các không gian lồi địa phương phức ......................................................... II.62
    3. Định lý Hahn-Banach và các ứng dụng của nó ................................. II.63
    4. Các tôpô yếu trên các không gian vectơ phức ....................................... II.64

Các bài tập về § 2 ......................................................................................... II.65
Các bài tập về § 3 ......................................................................................... II.72
Các bài tập về § 4 ......................................................................................... II.74
Các bài tập về § 5 ......................................................................................... II.76
Các bài tập về § 6 ......................................................................................... II.81
Các bài tập về § 7 ......................................................................................... II.87
Các bài tập về § 8 ......................................................................................... II.95

Chương III. — Các không gian của các ánh xạ tuyến tính liên tục ............................. III.1

§ 1. Bornology trong một không gian vectơ tôpô ............................................. III.1
    1. Các bornology ......................................................................................... III.1
    2. Các tập hợp bị chặn của một không gian vectơ tôpô ................................. III.2
    3. Ảnh qua một ánh xạ liên tục .................................................. III.4
    4. Các tập hợp bị chặn trong một số giới hạn quy nạp ...................................... III.5
    5. Các không gian E_A (A bị chặn) ............................................................. III.7
    6. Các tập hợp bị chặn đầy đủ và các không gian nửa đầy đủ ....................... III.8
    7. Các ví dụ ............................................................................................ III.9

§ 2. Các không gian bornological ............................................................................. III.11

§ 3. Các không gian của các ánh xạ tuyến tính liên tục ............................................... III.13
    1. Các không gian $\mathcal{L}_\mathfrak{S}(E; F)$ ............................................. III.13
    2. Điều kiện để $\mathcal{L}_\mathfrak{S}(E; F)$ là Hausdorff .................. III.15
    3. Các quan hệ giữa $\mathcal{L}(E; F)$ và $\mathcal{L}(\hat{E}; F)$ ............. III.15
    4. Các tập hợp liên tục đều của $\mathcal{L}(E; F)$ ..................................... III.16
    5. Các tập hợp liên tục đều của $E'$ ....................................................... III.19
    6. Sự hoàn thành của một không gian lồi địa phương ....................................... III.20
    7. Các bornology $\mathfrak{S}$ trên $\mathcal{L}(E; F)$ ..................................... III.21
    8. Các tập hợp đầy đủ của $\mathcal{L}_\mathfrak{S}(E; F)$ ..................................... III.22

§ 4. Định lý Banach-Steinhaus ....................................................... III.23
    1. Các thùng và các không gian thùng ............................................................. III.24

2. The Banach-Steinhaus theorem ............................................. III.25
3. Bounded subsets of $\mathcal{L}(E; F)$ (quasi-complete case) .......... III.27

§ 5. Các ánh xạ song tuyến tính giả liên tục ........................................ III.28
    1. Các ánh xạ song tuyến tính liên tục riêng rẽ ............................... III.28
    2. Các ánh xạ song tuyến tính liên tục riêng rẽ trên một tích của các không gian Fréchet .................................................. III.29
    3. Các ánh xạ song tuyến tính giả liên tục ..................................... III.30
    4. Mở rộng của một ánh xạ song tuyến tính giả liên tục ..................... III.32
    5. Tính giả liên tục của ánh xạ $(u, v) \mapsto v \circ u$ ........ III.32

§ 6. Định lý đồ thị Borel .................................................... III.34
    1. Định lý đồ thị Borel .................................................. III.34
    2. Các không gian Lusin lồi địa phương ........................................... III.34
    3. Các ánh xạ tuyến tính đo được trên một không gian Banach ....................... III.36

Các bài tập về § 1 ............................................................. III.37
Các bài tập về § 2 ............................................................. III.40
Các bài tập về § 3 ............................................................. III.41
Các bài tập về § 4 ............................................................. III.43
Các bài tập về § 5 ............................................................. III.46
Các bài tập về § 6 ............................................................. III.49

CHƯƠNG IV. — Đối ngẫu trong các không gian vectơ tôpô ......................... IV.1

§ 1. Đối ngẫu ................................................................. IV.1
    1. Các tôpô tương thích với một đối ngẫu ................................. IV.1
    2. Tôpô Mackey và tôpô yếu hơn trên một không gian lồi địa phương .................................................. IV.4
    3. Chuyển vị của một ánh xạ tuyến tính liên tục ........................... IV.6
    4. Đối ngẫu của một không gian thương và của một không gian con ......................... IV.8
    5. Đối ngẫu của một tổng trực tiếp và của một tích .............................. IV.11

§ 2. Đối ngẫu kép. Các không gian phản xạ ............................................... IV.14
    1. Đối ngẫu kép ............................................................... IV.14
    2. Các không gian nửa phản xạ ............................................... IV.15
    3. Các không gian phản xạ .................................................. IV.16
    4. Trường hợp các không gian định chuẩn .......................................... IV.17
    5. Các không gian Montel ..................................................... IV.18

§ 3. Đối ngẫu của một không gian Fréchet ............................................. IV.21
    1. Các không gian nửa thùng ............................................... IV.21
    2. Đối ngẫu của một không gian lồi địa phương mêtric hóa được ........................ IV.22
    3. Đối ngẫu kép của một không gian lồi địa phương mêtric hóa được ...................... IV.23
    4. Đối ngẫu của một không gian Fréchet phản xạ ................................ IV.23

5. The topology of compact convergence on the dual of a Fréchet space .................................................. IV.24
6. Separately continuous bilinear mappings ......................... IV.26

§ 4. Các đồng cấu ngặt của các không gian Fréchet ............................. IV.26
    1. Các đặc trưng của các đồng cấu ngặt ......................... IV.27
    2. Các đồng cấu ngặt của các không gian Fréchet ............................ IV.28
    3. Các tiêu chuẩn cho tính toàn ánh ....................................... IV.31

§ 5. Các tiêu chuẩn compact ............................................. IV.32
    1. Các nhận xét chung ............................................... IV.32
    2. Tính compact đơn giản của các tập hợp hàm liên tục .......... IV.33
    3. Các định lý Eberlein và Šmulian ............................ IV.35
    4. Trường hợp các không gian các hàm liên tục bị chặn .......... IV.36
    5. Bao lồi của một tập compact yếu ...................... IV.37

Phụ lục. — Các điểm bất động của các nhóm các phép biến đổi afin ...... IV.39
    1. Trường hợp các nhóm giải được .................................. IV.39
    2. Các trung bình bất biến ............................................... IV.40
    3. Định lý Ryll-Nardzewski ...................................... IV.41
    4. Các ứng dụng .................................................. IV.44

Các bài tập về § 1 ..................................................... IV.47
Các bài tập về § 2 ..................................................... IV.52
Các bài tập về § 3 ..................................................... IV.57
Các bài tập về § 4 ..................................................... IV.62
Các bài tập về § 5 ..................................................... IV.67
Các bài tập về Phụ lục .............................................. IV.72
Bảng I. — Các kiểu chính của các không gian lồi địa phương ............... IV.75
Bảng II. — Các bornôlôg chính trên đối ngẫu của một không gian lồi địa phương .... IV.76

CHƯƠNG V. — Các không gian Hilbert (lý thuyết sơ cấp) ............... V.1

§ 1. Các không gian tiền Hilbert và các không gian Hilbert .................... V.1
    1. Các dạng Hermit ............................................... V.1
    2. Các dạng Hermit dương ...................................... V.2
    3. Các không gian tiền Hilbert ......................................... V.4
    4. Các không gian Hilbert ............................................ V.6
    5. Các tập con lồi của một không gian tiền Hilbert ..................... V.9
    6. Các không gian con vectơ và các phép chiếu trực giao ......................... V.12
    7. Đối ngẫu của một không gian Hilbert .................................. V.15

§ 2. Các họ trực giao trong một không gian Hilbert .................... V.17
    1. Tổng Hilbert ngoài của các không gian Hilbert ............... V.17
    2. Tổng Hilbert của các không gian con trực giao của một không gian Hilbert .. V.18

3. Orthonormal families ............................................. V.21
4. Orthonormalisation ............................................... V.23

§ 3. Tích tenxơ của các không gian Hilbert .......................... V.25
    1. Tích tenxơ của các không gian tiền Hilbert ....................... V.25
    2. Tích tenxơ Hilbert của các không gian Hilbert ............... V.28
    3. Các lũy thừa Hilbert đối xứng .................................. V.29
    4. Các lũy thừa Hilbert ngoài .................................... V.33
    5. Phép nhân ngoài ....................................... V.35

§ 4. Một số lớp toán tử trong các không gian Hilbert ............... V.37
    1. Liên hợp ..................................................... V.38
    2. Các ánh xạ tuyến tính đẳng cự từng phần .......................... V.41
    3. Các tự đồng cấu chuẩn ......................................... V.43
    4. Các tự đồng cấu Hermit ...................................... V.44
    5. Các tự đồng cấu dương ....................................... V.45
    6. Vết của một tự đồng cấu ..................................... V.48
    7. Các ánh xạ Hilbert-Schmidt ..................................... V.52
    8. Chéo hóa các ánh xạ Hilbert-Schmidt ................. V.55
    9. Vết của một dạng toàn phương đối với một dạng khác .......... V.57

Các bài tập của § 1 .................................................. V.60
Các bài tập của § 2 .................................................. V.70
Các bài tập của § 3 .................................................. V.73
Các bài tập của § 4 .................................................. V.74
Các ghi chú lịch sử .................................................. V.80
Tài liệu tham khảo .................................................. V.92
Chỉ số ký hiệu ...................................................... 347
Chỉ số thuật ngữ ................................................... 349
Tóm tắt một số tính chất quan trọng của các không gian Banach .... 355
Mục lục ............................................................. 359
