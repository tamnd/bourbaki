---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: ts-iii-v-fr
book_pages: TS V.517-TS V.540
pdf_pages: 0530-0553
extraction: native
subsections:
    - "no": 1
      title: Découverte du spectre continu
      page: 517
      pdf_page: 530
    - "no": 2
      title: Opérateurs compacts
      page: 521
      pdf_page: 534
    - "no": 3
      title: Indice de Fredholm et perturbations
      page: 523
      pdf_page: 536
    - "no": 4
      title: Opérateurs partiels et théorème spectral
      page: 526
      pdf_page: 539
    - "no": 5
      title: Jonction entre analyse harmonique et théorie des groupes
      page: 528
      pdf_page: 541
    - "no": 6
      title: Groupes localement compacts commutatifs
      page: 533
      pdf_page: 546
    - "no": 7
      title: Algèbres d’opérateurs
      page: 536
      pdf_page: 549
    - "no": 8
      title: Représentations des groupes localement compacts
      page: 539
      pdf_page: 552
statements: 0
exercises: 0
content_sha256: 306ad7d54c6c88db3297d0a2cb6433cc3f168b4f9f58fb6ce9700a7847758464
translated_from: content/en-mt/ts/V/historical_note.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 1f42e006f997885593b0e632f8b3c56f3053ebc4b3a331465f61e84ffcb3c41b
translation_model: gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-de217e94
glossary_version: 34
glossary_terms_sha256: 6b8320f8d61556e131a9bb06cd22d5de9d9d33ff4bdaafd72c99fd2a1540c5e5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Chương I đến V)

Các khái niệm về trị riêng và chuỗi Fourier đã rất quen thuộc vào năm 1830, thâm nhập vào nhiều lĩnh vực của Giải tích trong suốt thế kỷ xix$^e$ (xem ÉHM, p. 114, 260, 275). Nhưng lý thuyết phổ và giải tích điều hòa, theo nghĩa mà chúng ta hiểu chúng trong cuốn sách này, chỉ bắt đầu có dạng hiện nay vào khoảng một thế kỷ sau — đồng thời với sự nối kết của chúng với việc nghiên cứu các biểu diễn của nhóm vào khoảng năm 1930, và sau đó với việc nghiên cứu các đại số chuẩn vào khoảng năm 1940.

Ở đây chúng ta chỉ giới hạn trong việc vạch ra những đường nét chính của sự phát triển của chúng trong giai đoạn kéo dài từ năm 1906 — thời điểm Hilbert đưa vào khái niệm “phổ liên tục” trong công trình của ông về các phương trình nguyên — đến những năm 1945–1950, khi các lý thuyết được trình bày ở đây về cơ bản đã đạt được dạng mà chúng vẫn giữ cho đến ngày nay.

### 1. Phát hiện phổ liên tục

Trong Chú ý về các không gian vectơ tôpô (xem ÉHM, p. 262–263), chúng tôi đã mô tả cách I. Fredholm, vào khoảng năm 1900 — tiếp tục các công trình của C. Neumann, V. Volterra và H. Poincaré — đã đi đến việc xét phương trình

$$
u(x)-\lambda \int_IK(x, y)u(y)dy=f(x) \tag{1}
$$

với hàm chưa biết $u: I\rightarrow \mathbf{C}$, trong trường hợp khoảng $I\subset \mathbf{R}$ là compact và hạt nhân K liên tục trên $I\times I$. Việc sử dụng khéo léo các “định thức vô hạn”, dựa trên các ý tưởng của Poincaré và H. von Koch, đã cho phép ông thu được các họ nghiệm mà sự phụ thuộc vào biến phức $\lambda$ là phân hình, rồi chứng minh “phương án thay thế” nổi tiếng liên quan đến sự tồn tại của các nghiệm (xem III, p. 81, đl. 5). Nhưng Fredholm ngay lập tức chuyên biệt hóa các kết quả của mình vào trường hợp $\lambda =-1$, mà không khai thác sự kiện rằng phương trình (1) là một bài toán trị riêng[^1].

Khi hạt nhân K đối xứng, chúng ta cũng đã thấy cách Hilbert, trong hồi ký đầu tiên của ông về các phương trình nguyên [**31**], nhận ra mối liên hệ giữa bài toán của Fredholm và việc nghiên cứu các “trục chính” của một dạng toàn phương. Bắt đầu từ sự rút gọn này đối với các “phần” hữu hạn (rời rạc hóa) của hạt nhân K, ông thu được, bằng cách chuyển qua giới hạn, công thức

$$
\int_IK(s, t)x(s)x(t)dt=\sum_{n=1}^{\infty}\frac{1}{\lambda_n}\int_I\varphi_n(s)x(s)ds \tag{2}
$$

trong đó các $\lambda_n$ là các trị riêng của hạt nhân K, các $\varphi_n$ lập thành một hệ trực chuẩn các vectơ riêng liên kết[^2], và trong đó đẳng thức đúng ngay khi $x$ khả tích bình phương trên I (xem ÉHM, p. 264).

Các trở ngại chính xuất hiện đối với Hilbert liên quan đến việc chuyển từ các tổng hữu hạn sang các tích phân trong công thức (2). Ông suy ra từ công thức này sự tồn tại của các trị riêng — tuy nhiên, ông đã đưa ra cho chúng một đặc trưng hóa biến phân độc lập với việc chuyển qua giới hạn, lấy cảm hứng từ phương pháp cổ điển xác định các trị riêng trong số chiều hữu hạn (xem n$^o4$ của IV, p. 153). E. Schmidt sẽ chỉ ra vào năm 1905, lấy cảm hứng từ công trình của H. Schwarz, cách thu được (2) mà không đi qua các “định thức vô hạn” mà trên đó các phương pháp của Fredholm và Hilbert phụ thuộc (xem ÉHM, p. 265).

Nhưng ngay từ năm 1906, Hilbert [**32**] đã chuyển sang bài toán tổng quát hơn về sự rút gọn của một dạng toàn phương

$$
B(x, x) =\sum_{p,q=0}^{\infty}b_{pq}x_px_q,x= (x_p)_{p\in\mathbf{N}}
$$

trên $E =\ell^2_{\mathbf{C}}(\mathbf{N})$. Dĩ nhiên ông vẫn ghi nhớ rằng, bằng cách chuyển qua các hệ số trong một cơ sở trực chuẩn của E, bài toán (1) được rút gọn thành việc tìm các nghiệm của “hệ tuyến tính vô hạn”

$$
x_p+\sum_{q=0}^{\infty}b_{pq}x_q=f_p(p\in \mathbf{N})
$$

Tuy nhiên ông chỉ ra rằng đối với bài toán của Fredholm, các dạng toàn phương được xét là những dạng rất đặc biệt, đối với chúng $B(x_n, x_n)$ tiến tới $B(x, x)$ ngay khi $x_n$ hội tụ yếu đến $x$; ông gọi chúng là “hoàn toàn liên tục” (vollstetig).

Hilbert nhấn mạnh sự khác biệt cốt yếu phân biệt chúng với các dạng toàn phương bị chặn trên E, và quyết định thực hiện sự rút gọn tổng quát hơn của các dạng sau. Một lần nữa, phương pháp của ông là bắt đầu từ sự rút gọn của các “phần hữu hạn”

$$
(x_0, . . . , x_n)\mapsto \sum_{p,q=0}^nb_{pq}x_px_q
$$

của dạng B, rồi cho $n$ tiến tới vô hạn. Đối với sự chuyển qua giới hạn này, ông tận dụng các ý tưởng về tích phân được đưa vào bởi T. Stieltjes trong công trình của ông về phân thức liên tục [**71**]. Ông chứng minh rằng mọi dạng toàn phương bị chặn đều có thể, sau một phép biến đổi trực giao của các biến, được đưa về dạng

$$
\sum_{p\in\mathbf{N}}\frac{1}{\lambda_p}x^2_p+\int_{s\in\mathbf{R}}\frac{1}{s}d\sigma (s, x) \tag{3}
$$

Trong công thức này, các $\lambda_p$ là các trị riêng của B và $x\mapsto \sigma (s, x)$ là (với $s\in \mathbf{R}$ cố định) một dạng toàn phương dương phân ly trên E, trong khi $s\mapsto \sigma (s, x)$ là[^3] (với $x\in E$ cố định) một hàm liên tục tăng tiến tới 0 tại $-\infty$ và tới $\|x\|^2$ tại $+\infty ($xem ÉHM, p. 284, về ký hiệu của Stieltjes).

Gọi S là tập hợp các điểm của $\overline{\mathbf{R}}$ không có lân cận nào trong đó $s\mapsto \sigma (s, x)$ vẫn hằng đối với mọi $x$; khi đó tích phân trong (3) hiển nhiên có thể được lấy trên S. Hilbert gọi tập hợp S là “phổ liên tục” (Streckenspektrum), tập hợp các trị riêng của B là “phổ điểm” (Punktspektrum), và hợp của chúng là “phổ” (Spektrum). Thuật ngữ này, xuất phát từ quang học, đã được W. Wirtinger sử dụng vào năm 1897 [**91**] trong việc nghiên cứu các phương trình vi phân với các hệ số tuần hoàn.

Hilbert sẽ nhanh chóng suy ra từ các phương pháp “phổ” của mình một sự đổi mới sâu sắc đối với một số vấn đề của Giải tích cổ điển, liên quan đến việc nghiên cứu các phương trình vi phân thường (đặc biệt là kiểu Sturm–Liouville), các phương trình vi phân riêng phần hoặc các hàm của một biến phức. Chúng tôi sẽ không trình bày ở đây sự phong phú của các kết quả đã tiếp theo trong phần tư đầu tiên của thế kỷ xx$^e$ và tham chiếu đến sự tổng hợp của E. Hellinger và O. Toeplitz [**29**]. Tuy nhiên, chúng tôi vẫn sẽ đề cập đến một số công trình này về các phương trình nguyên, nơi tìm thấy những mầm mống của các phát triển sau này của lý thuyết trừu tượng.

Đối với Hilbert và các học trò của ông, trung thành với một truyền thống Đức trong Đại số tuyến tính, mô hình vẫn là định lý về các trục chính; do đó vấn đề vẫn là nghiên cứu các phổ của các dạng song tuyến tính hoặc dạng toàn phương, đặc biệt trên không gian “Hilbert” $E =\ell^2_{\mathbf{C}}(\mathbf{N})$. Sự kiện rằng mọi dạng song tuyến tính liên tục B trên E có thể liên hệ với tự đồng cấu liên tục A của E được đặc trưng bởi $\langle Ax, y\rangle = B(x, y)$ đã được trường phái Hilbert biết đến, đặc biệt sau các công trình của E. Schmidt, M. Fréchet và F. Riesz vào năm 1907–1908. Nhưng chính F. Riesz là người đã chỉ ra, trong một cuốn sách đáng ngưỡng mộ [**59**] năm 1913, sự quan trọng của việc đặt các tự đồng cấu lên hàng đầu trong bối cảnh này.

Riesz đưa ra định nghĩa hiện đại của phổ của một phần tử A của $\mathscr{L}(E)$[**59**, p. 139], nhận xét rằng nó là một tập hợp đóng, bị chặn, và chỉ ra rằng giải thức $\lambda \mapsto (\lambda 1_E-A)^{-1}$ là hàm chỉnh hình trên phần bù của phổ của A. Trên hết, ông dành một vai trò trung tâm cho cấu trúc đại số của $\mathscr{L}(E) :$ lấy cảm hứng từ công trình của Volterra, ông phát triển một phiên bản đầu tiên của phép tính phiếm hàm cho các tự đồng cấu đối xứng, cho phép ông khôi phục một cách đơn giản các kết quả rút gọn của Hilbert và Schmidt. Nếu A là một phần tử đối xứng của $\mathscr{L}$ (E), Riesz chỉ ra cách định nghĩa $f(A)$ đối với mọi hàm $f$ nửa liên tục (dưới hoặc trên) từ $\mathbf{R}$ đến $\mathbf{R}$, và nhận xét rằng $f\mapsto f(A)$ là cái mà ngày nay chúng ta gọi là một cấu xạ đại số [**59**, p. 129–130]. Áp dụng ý tưởng này cho hàm đặc trưng của một khoảng $[\xi ,+\infty [$, ta thu được với mọi $\xi$ một tự đồng cấu đối xứng $A_{\xi}$ của E; sử dụng tích phân Stieltjes, Riesz sau đó chỉ ra một phiên bản của quan hệ (3) của Hilbert:

$$
\langle Ax, y\rangle =\int_{\mathbf{R}}\xi  d\langle A_{\xi}x, y\rangle
$$

với $x, y\in E$, một đẳng thức mà ông thậm chí còn viết

$$
A =\int_{\mathbf{R}}\xi  dA_{\xi}
$$

Khi đó phổ của A là tập hợp các giá trị $\xi_0$ sao cho $A_{\xi}$ không giữ nguyên là hằng trong bất kỳ lân cận nào của $\xi_0$, và phổ điểm là tập hợp các điểm gián đoạn của $\xi \mapsto A_{\xi}$.

Ngay trước khi kết thúc với các áp dụng của lý thuyết, Riesz nhận xét [**59**, p. 146] rằng các kết quả của ông có dạng đặc biệt đơn giản khi tự đồng cấu A xuất phát từ một trong các dạng song tuyến tính “liên tục hoàn toàn” của Hilbert: phổ thu gọn thành tập hợp các trị riêng (có thể phải thêm vào 0), các trị riêng được sắp xếp thành một dãy tiến tới 0, và mỗi trị riêng khác không có bội số hữu hạn (III, p. 90, prop. 5).

### 2. Các toán tử compact

Riesz mở rộng đáng kể các nhận xét này chưa đầy ba năm sau, trong hồi ký của ông về các phương trình phiếm hàm [**60**], công trình phát triển, với một sự sáng rõ còn nguyên vẹn sau hơn một thế kỷ, phần cốt yếu của lý thuyết phổ của các toán tử compact trên các không gian Banach. Mục tiêu được nêu của văn bản này là phát biểu lại lý thuyết Fredholm cho phương trình (1) trên một khoảng compact I, bằng cách xét không gian $E =\mathscr{C}(I)$ được trang bị tôpô của sự hội tụ đều. Nhưng như chúng tôi đã chỉ ra trong một chú ý trước đó (ÉHM, p. 268), Riesz rõ ràng ý thức rằng các kết quả của ông áp dụng cho mọi không gian Banach — khái niệm chỉ được đưa vào trong thập kỷ tiếp theo.

Lấy cảm hứng từ các ý tưởng của Fréchet về tôpô tổng quát, Riesz giờ đây xét các tự đồng cấu của E biến mọi dãy bị chặn thành một dãy tương đối compact. Giống như Hilbert, ông vẫn gọi chúng là “liên tục hoàn toàn” và nhận xét rằng khái niệm mới này là tương đương, trong trường hợp của E = $\ell^2_{\mathbf{C}}(\mathbf{N})$, với khái niệm tính liên tục hoàn toàn mà ông đã sử dụng trong cuốn sách năm 1913 của mình[^4].

Riesz nghiên cứu các tự đồng cấu có dạng $B = 1_E-A$ trong đó A là một tự đồng cấu liên tục hoàn toàn của E, và suy ra tất cả các tính chất phổ của chúng từ sự kiện rằng một không gian vectơ định chuẩn compact địa phương phải có số chiều hữu hạn — một sự kiện dường như được phát hiện nhân dịp này. Ông dễ dàng chứng minh rằng hạt nhân của B có số chiều hữu hạn và ảnh của nó là đóng và có đối chiều hữu hạn. Như E. Weyr [**87**] đã làm trong số chiều hữu hạn, sau đó ông xét các lũy thừa lặp $B^k$. Ông chỉ ra rằng dãy các hạt nhân của chúng và dãy các ảnh của chúng là dừng, rồi đưa vào cái mà ngày nay chúng ta gọi là không gian không lũy linh và không gian đối không lũy linh của B, chỉ ra một cách hiệu quả rằng E là tổng trực tiếp tôpô của chúng. Áp dụng nhận xét này cho các tự đồng cấu $B_{\lambda}= 1_E-\lambda A$ với $\lambda \in \mathbf{C}$, ông suy ra không khó khăn các tính chất phổ của các tự đồng cấu liên tục hoàn toàn của một không gian Banach, và điều này dưới một dạng gần như hoàn chỉnh.

Trong số các kết quả chính về phổ của các toán tử này, dường như chỉ những kết quả đòi hỏi một cái nhìn chín chắn hơn về khái niệm không gian phiếm hàm, đặc biệt là về đối ngẫu, mới vượt ra ngoài Riesz. Chẳng hạn, vào cuối những năm 1920, T. Hildebrandt [**33**] và J. Schauder [**63**] sẽ chỉ ra (trong đặt bối cảnh hiện đã được xác lập của các không gian Banach) rằng tự đồng cấu đối ngẫu của một tự đồng cấu liên tục hoàn toàn là liên tục hoàn toàn.

Hơn nữa, khái niệm liên tục hoàn toàn của Riesz vẫn phụ thuộc vào việc sử dụng các dãy; Banach [**4**] đã giải phóng mình khỏi điều này trong cuốn sách năm 1932 của ông để xét các ánh xạ biến đổi mọi tập con bị chặn thành một tập con compact tương đối. Thuật ngữ ánh xạ tuyến tính « compact » chỉ dần dần được thiết lập trong nửa sau của thế kỷ xx$^e$, có lẽ theo sau cuốn sách của E. Hille [**34**] về các nửa nhóm toán tử.

Một số câu hỏi được đặt ra trong những năm 1930 sẽ còn để ngỏ trong một thời gian dài. Theo hướng này, hãy nhắc đến việc giải quyết [**18**] vào năm 1973 của « bài toán xấp xỉ » được Banach và S. Mazur làm nổi tiếng vào các năm 1932 và 1938 (xem Nhận xét 6 của III, p. 16 và Bài tập 25 của III, p. 112).

Cùng lúc đó, Lomonosov [**40**] đã chứng minh sự tồn tại của các không gian con đóng không tầm thường bất biến dưới một tự đồng cấu giao hoán với một tự đồng cấu compact khác không trong một không gian lồi địa phương (hệ quả 2 của III, p. 13). Kết quả này là một trong những tiến bộ đáng kể nhất về bài toán tồn tại một không gian con như vậy đối với một tự đồng cấu liên tục tùy ý (« bài toán không gian con bất biến »). Bài toán này hiện vẫn còn để ngỏ, tại thời điểm hiện tại, trong trường hợp các tự đồng cấu liên tục của các không gian Hilbert kiểu đếm được; P. Enflo [**19**] đã xây dựng vào năm 1987 ví dụ đầu tiên về một tự đồng cấu của một không gian Banach không có không gian con bất biến đóng không tầm thường.

### 3. Chỉ số Fredholm và các nhiễu loạn

Khái niệm chỉ số xuất hiện vào năm 1920 trong một công trình của Fritz Noether về các phương trình nguyên. Trong bài diễn văn của ông tại Đại hội Quốc tế năm 1904, Hilbert đã xét một bài toán do Riemann đặt ra trong lý thuyết thế: nếu cho một miền mở bị chặn Ω của mặt phẳng mà biên là một đường cong đóng trơn đơn Γ, cũng như ba hàm $a,b,f$ trên Γ, bài toán là tìm một hàm $z: \Omega \rightarrow \mathbf{C}$, chỉnh hình trên Ω và liên tục trên Ω, thỏa mãn

$a\mathscr{R}(z) +b\mathscr{I}(z) =f$ sur $\Gamma$.

Tham số hóa Γ bởi một $s\in [0,2\pi ]$ thực, Hilbert chỉ ra rằng bài toán quy về việc giải một phương trình tích phân « hạt nhân kỳ dị » đối với $\varphi =\mathscr{R}(z)$, cụ thể là

$$
a(s)\varphi (s) +\int_0^{2\pi}K(s, t)\varphi (t)dt=f(s) \tag{4}
$$

Ở đây hạt nhân $K(s, t)$ có dạng $b(s)$ cot($\frac{t-s}{2}$) $+ A(s, t)$ đối với một hàm liên tục A. Do đó nó là kỳ dị dọc theo đường chéo, và tích phân trên phải được lấy theo nghĩa giá trị chính Cauchy.

Noether [**53**] nhận xét rằng trái với các phương trình tích phân thỏa mãn thay thế Fredholm, trong trường hợp một hạt nhân K như trên và một vế thứ hai khác không $f$, có thể xảy ra rằng (4) thừa nhận các họ nghiệm không tầm thường. Ông chỉ ra rằng không gian các nghiệm được chi phối bởi số nguyên

(5) $n=\frac{1}{2\pi}\int_{\Gamma}d$ (log($a-ib$)).

Nếu $n <0$, không có nghiệm không tầm thường, và nếu $n\geqslant 0$, phương trình (4) thừa nhận một họ với $2n$ tham số nghiệm. Noether dùng thuật ngữ « chỉ số » (Index) cho số nguyên $n$ và nhận ra trong đó một số vòng quay, một khái niệm cổ điển từ cuối thế kỷ xix$^e$ trong nghiên cứu các hàm của một biến phức.

Các công trình khác sau đó sẽ nghiên cứu các ví dụ về các phương trình đòi hỏi một sự mở rộng của lý thuyết Fredholm. Nhưng cần phải chờ hơn hai mươi năm trước khi khái niệm ánh xạ Fredholm được phát triển một cách hệ thống, đồng thời với việc nghiên cứu các nhiễu loạn bởi các toán tử compact đạt đến độ chín muồi.

Năm 1909, H. Weyl [**81**] đã chỉ ra rằng nếu hai dạng toàn phương bị chặn trên $\ell^2_{\mathbf{C}}(\mathbf{N})$ có một hiệu liên tục hoàn toàn, thì các phổ cốt yếu của chúng trùng nhau (xem III, p. 89, định lý 2). Hơn nữa, trong hồi ký năm 1916 của mình, Riesz đã nhận xét, dĩ nhiên không dùng ngôn ngữ hiện đại, rằng các toán tử compact trên một không gian Banach E tạo thành một iđêan hai phía của $\mathscr{L}(E)$. Tuy nhiên, dường như con đường được chỉ ra bởi hai nhận xét này chỉ được khai thác từ những năm 1940 trở đi. Năm 1941, J. Calkin, được thúc đẩy bởi các công trình của J. von Neumann về các đại số toán tử (mà chúng ta sẽ phải thảo luận sớm, xem p. 537), chỉ ra sự quan tâm của việc nghiên cứu các đồng dư modulo iđêan này trong đặt của các không gian Hilbert [**10**]. Ông chỉ ra cấu trúc của đại số hiện mang tên ông (xem III, p. 75) cho phép khôi phục kết quả của Weyl một cách đơn giản.

Cùng lúc đó, khoảng năm 1942, J. Dieudonné [**15**] đã có ý tưởng nghiên cứu các nhiễu loạn của một ánh xạ tuyến tính liên tục $u$ giữa các không gian định chuẩn, trong trường hợp nhiễu loạn là « nhỏ » theo nghĩa của chuẩn toán tử. Ông tự hạn chế vào trường hợp $u$ là một cấu xạ ngặt mà hạt nhân có chiều hữu hạn hoặc đối chiều hữu hạn, chứng minh rằng điều tương tự cũng đúng đối với mọi « nhiễu loạn nhỏ » của $u$, và chỉ ra rằng trong trường hợp các ánh xạ Fredholm (xem n$^o2$ của III, p. 40), chỉ số là hằng địa phương (định lý 1 của III, p. 58), cũng như một số kết quả được trình bày trong § 4 của III, p. 55.

Hai ý tưởng này hội tụ vào khoảng năm 1950, khi F. Atkinson [**3**], I. Gohberg [**26**], S. Mikhlin [**46**] và B. Yood [**93**] nghiên cứu các nhiễu loạn bởi các toán tử compact. Họ tường minh tạo ra mối liên hệ với chỉ số Noether và đưa ra các khái niệm ánh xạ Fredholm [**3**, p. 8] và ánh xạ Riesz [**93**, §5]. Các ánh xạ sau là đối tượng của nghiên cứu hệ thống trong thập niên tiếp theo, trong đó các kết quả được trình bày trong Chương III có dạng gần như hiện nay.

Đặt thông thường của các lý thuyết này là các không gian Banach; tuy nhiên, nhiều ứng dụng khác nhau thúc đẩy phép tổng quát hóa chúng đến các lớp rộng hơn của các không gian vectơ tôpô. Vì vậy, trường hợp các không gian Fréchet xuất hiện một cách tự nhiên vào năm 1954 trong công trình của H. Cartan và J-P. Serre [**13**], những người chứng minh tính hữu hạn của đối đồng điều của một đa tạp giải tích phức compact với các hệ số trong một bó kết dính, chứng minh sử dụng các kết quả biến dạng được chứng minh bởi L. Schwartz [**66**] (xem định lý 2 của III, p. 73).

Tính bất biến của chỉ số dưới phép biến dạng là hoàn toàn rõ ràng, trong trường hợp của công thức (5), nếu nhận xét rằng vế phải (số vòng quay) là bất biến dưới phép đồng luân. Những biểu thức tôpô như vậy đối với chỉ số sẽ sớm trở nên nổi tiếng cho các ánh xạ Fredholm phát sinh từ hình học vi phân. Nếu D là một toán tử vi phân trên một đa tạp compact X thuộc lớp $C^{\infty}($cf. VAR, §14), và nếu D là “elliptic” (cf. [**2**, §1]), thì một mở rộng của D lên các không gian Sobolev thích hợp xác định một ánh xạ Fredholm. Việc tìm kiếm một công thức cho một biểu thức tôpô của chỉ số của nó bằng các “lớp đặc trưng” của X, được gợi ý, trong số những công trình khác, bởi công trình của I. Gelfand vào khoảng năm 1960 [**23**, vol. I, p. 65], đã dẫn đến “định lý chỉ số” của M. Atiyah và I. Singer vào năm 1963 [**2**]. Định lý sau đã làm nảy sinh những phát triển phi thường tại giao điểm của giải tích, tôpô và hình học vi phân. Chúng ta không thể mô tả ở đây những lĩnh vực rộng lớn mà chúng đã mở ra và những lĩnh vực này, vẫn rất phong phú cho đến ngày nay, không ngừng nhận được nguồn nuôi dưỡng từ lý thuyết Fredholm.

### 4. Các toán tử bộ phận và định lý phổ

Lý thuyết phổ Hilbert tổng quát được xây dựng phần lớn nhằm trả lời bài toán về các nền tảng toán học của Cơ học lượng tử, đặc biệt dưới sự thúc đẩy của von Neumann.

Chúng tôi dẫn chiếu đến công trình của M. Jammer [**35**] để có một mô tả chi tiết về sự phát triển của lý thuyết Lượng tử cho đến bài báo nền tảng của W. Heisenberg, bài báo đã đưa Cơ học lượng tử vào [**28**]. Chưa đầy năm năm đã trôi qua giữa việc công bố nó vào mùa hè năm 1924 và việc công bố bài báo [**50**], vào năm 1929, trong đó von Neumann trình bày, một cách hoàn toàn sáng sủa và chặt chẽ, tất cả các kết quả nền tảng của lý thuyết các toán tử bộ phận Hermit (thường được gọi là “không bị chặn”) trên các không gian Hilbert.

Bằng việc đưa ra trình bày tiên đề đầu tiên về các không gian Hilbert [**49**], von Neumann hoàn thiện một ý tưởng đã được hình thành từ lâu (cf. ÉHM, p. 267), và làm sáng tỏ nhiều đẳng cấu giữa các không gian dãy hoặc hàm vốn đã được Schmidt, Fréchet, Fischer và Riesz biết đến trước năm 1910. Sự gia tăng tính trừu tượng này cho phép von Neumann thực hiện những tiến bộ khái niệm đáng kể.

Đó là ý tưởng về một toán tử bộ phận, dường như vẫn còn lơ lửng, chưa có hình thức, trên một số công trình nghiên cứu tiếp tục lại, sau Hilbert, các phương trình Fredholm (xem ở trên, n$^o1$). Hilbert đã nhận thấy rằng nhiều phương trình vi phân kiểu Sturm–Liouville, đặc biệt trong trường hợp một khoảng không bị chặn, có thể quy về các phương trình Fredholm; nhưng để áp dụng các phương pháp tích phân, cần phải làm yếu các điều kiện đặt lên hạt nhân và rời khỏi môi trường trong đó các kết quả của Fredholm, Hilbert và Schmidt có thể được áp dụng. Qua nhiều năm, các hạt nhân ngày càng kỳ dị hơn được nghiên cứu, cho đến khi xét các phương trình mà vế trái chỉ có nghĩa nếu ẩn thuộc một không gian con của $L^2(I)$. Theo hướng này, cần phải nhắc đến công trình của E. Hilb [**30**] năm 1908, của H. Weyl về lý thuyết Sturm–Liouville [**82**] năm 1910, và trên hết là của T. Carleman [**11**] năm 1923, trong một cách đặt rất tổng quát.

Bằng cách thống nhất các bài toán này, von Neumann đem lại một ánh sáng hoàn toàn mới cho các công trình cổ điển này. Ông đặc biệt nhấn mạnh sự phân biệt nền tảng giữa toán tử đối xứng và toán tử tự liên hợp, và diễn giải các mở rộng tự liên hợp của một toán tử đối xứng theo các “điều kiện biên” trừu tượng, tổng quát hóa các điều kiện biên quen thuộc đã xuất hiện, chẳng hạn, trong các bài toán Dirichlet và Neumann đối với toán tử Laplace trên một tập con mở bị chặn của $\mathbf{R}^n$.

Đồng thời, von Neumann [**51**] làm nổi bật khái niệm toán tử chuẩn[^5] như một cách đặt tự nhiên cho lý thuyết phổ, nhấn mạnh vai trò của đại số giao hoán sinh bởi toán tử và toán tử liên hợp của nó.

Dựa trên hình thức toán học chính xác này, vốn cũng làm sáng tỏ sự tương đương giữa các quan điểm của Heisenberg và Schrödinger, và dựa trên cách diễn giải Copenhagen về các thủ tục và kết quả thực nghiệm, Cơ học lượng tử không tương đối tính do đó đã đạt đến một trạng thái hoàn thiện hầu như không thay đổi kể từ đó; tính đúng đắn của lý thuyết vật lý này, bất chấp những hệ quả đáng ngạc nhiên, thậm chí có vẻ nghịch lý, kể từ đó luôn luôn được thực nghiệm xác nhận, và với độ chính xác đáng kể.

Từ quan điểm hình thức, các nền tảng của lý thuyết phổ đã được thiết lập bởi von Neumann. Đồng thời, sau khi trình bày những ý tưởng đầu tiên của ông, M. Stone đã tiếp tục những nghiên cứu tương tự trong khoảng thời gian từ 1928 đến 1930 và thu được các kết quả liên quan. Sự trình bày rõ ràng và đầy đủ các kết quả đã biết mà Stone công bố năm 1932 [**72**] đã có một ảnh hưởng quan trọng đến sự phổ biến của lý thuyết phổ Hilbert.

Tuy nhiên, những cải tiến khác trong cách trình bày cũng quan trọng đối với sự phổ biến của các kết quả này. Thật vậy, định lý phổ (cf. Theorem 1 of IV, p. 266), như được trình bày bởi von Neumann, trong một thời gian dài đã được xem là rất khó, phần lớn vì nó được phát biểu trong cách đặt của các độ đo nhận giá trị vectơ.

Về sau, P. Halmos [**27**], bằng cách nhấn mạnh cách diễn giải định lý phổ thông qua các toán tử phép nhân trên các không gian $L^2$, đã làm lộ ra khía cạnh về bản chất là sơ cấp của nó trong trường hợp các toán tử bị chặn. Gần đây, S. Woronowicz (trong cách đặt hơi khác của các toán tử chính quy của các môđun Hilbert trên các đại số sao [**92**]) đã đưa vào một sự đơn giản hóa bằng cách đưa vào “sự sinh chuẩn” (cf. No.$^o2$ of IV, p. 265), điều này làm cho có thể xử lý các toán tử bộ phận chuẩn một cách đơn giản như các toán tử tự liên hợp.

Hơn nữa, nếu D là một toán tử vi phân vô hướng đối xứng hình thức trên một tập mở U của $\mathbf{R}^n$, việc nghiên cứu các mở rộng tự liên hợp của D lên $L^2(U)$ được liên kết một cách tự nhiên với việc nghiên cứu các phân bố trên U (trong trường hợp của toán tử Laplace, xem No.$^o6$ của IV, p. 242). Chúng tôi dẫn công trình của J. Dieudonné [**16**, ch. vii] về lịch sử của vấn đề sau — một lịch sử quanh co được tháo gỡ ngay sau thời kỳ vừa được nhắc đến, với những đóng góp quyết định của S. Sobolev [**69**] năm 1936, và của L. Schwartz [**65**] mười năm sau.

Từ quan điểm thuần túy toán học, lý thuyết phổ tương tác theo một cách đặc biệt phong phú với Hình học Riemann. Như vậy, tiếp tục một câu hỏi của S. Bochner, M. Kac đưa ra năm 1966 một trình bày đặc sắc khác thường [**36**] về bài toán xác định các tính chất hình học của một đa tạp Riemann có thể được suy ra từ các tính chất phổ của toán tử Laplace. Câu hỏi này đã được nhà vật lý A. Schuster [**64**] dự liệu vào năm 1882: Việc tìm ra các âm điệu khác nhau phát ra bởi một hệ dao động là một bài toán có thể hoặc không thể giải được trong một số trường hợp đặc biệt, nhưng nó sẽ làm bối rối nhà toán học tài giỏi nhất nếu phải giải bài toán nghịch đảo và tìm ra hình dạng của một cái chuông bằng các âm thanh mà nó có khả năng phát ra. (“Xác định các họa âm phát ra bởi một hệ dao động là một bài toán có thể hoặc không thể giải được trong một số trường hợp riêng biệt, nhưng nhà toán học tài giỏi nhất cũng sẽ lúng túng nếu phải giải bài toán nghịch đảo và xác định hình dạng của một cái chuông từ các âm thanh mà nó có thể phát ra”).

### 5. Sự nối tiếp giữa giải tích điều hòa và lý thuyết nhóm

Chúng tôi đã mô tả, trong các chú ý lịch sử của Sách Tích phân (xem ÉHM, p. 275), cách mà các câu hỏi liên quan đến phương trình nhiệt đã dẫn Fourier đến quan niệm mang tính cách mạng về biểu diễn một hàm tùy ý như một tổng các hàm lượng giác.

Chúng tôi không thể truy lại ở đây sự phát triển của lý thuyết chuỗi Fourier và tích phân Fourier trong suốt thế kỷ xix$^e$, cũng như ảnh hưởng sâu sắc mà các câu hỏi do lý thuyết này đặt ra đã có đối với sự tiến hóa của Giải tích — đến mức làm đảo lộn quan niệm về các số thực, góp phần vào sự ra đời của lý thuyết tập hợp (xem ÉHM, p. 42). Nhưng để hiểu dạng thức của các ý tưởng được trình bày trong Sách này, thích hợp là mô tả cách mà giải tích điều hòa đã được liên kết sau năm 1925 với lý thuyết nhóm và với lý thuyết phổ Hilbert.

Việc nhận ra mối liên hệ giữa các ý tưởng của Fourier và các cấu trúc nhóm của $\mathbf{R}/\mathbf{Z}$ và $\mathbf{R}$, cũng như phép tổng quát hóa các ý tưởng này cho các nhóm khác, đã diễn ra khá muộn.

Một cách tự nhiên, trong những bước đầu của lý thuyết các nhóm hữu hạn và các đặc trưng của chúng, người ta có thể đồng nhất các kết quả mà ngày nay dường như chứa đựng những mầm mống của giải tích Fourier hữu hạn. Chẳng hạn, nhóm đối ngẫu của nhóm các phần tử khả nghịch của $\mathbf{Z}/q\mathbf{Z}$, cũng như quan hệ trực giao biểu diễn hàm đặc trưng của một phần tử như một tổ hợp tuyến tính của các đặc trưng, xuất hiện một cách ngầm ẩn vào năm 1837 trong bài báo của Dirichlet [**17**] chứng minh rằng tồn tại vô hạn số nguyên tố $p\equiv a$ mod$. q$ nếu $a$ nguyên tố cùng nhau với $q$. Nó dựa trên các ý tưởng của Gauss, người đã đưa vào số hạng “đặc trưng” (character) trong nghiên cứu của ông về các dạng toàn phương nhị phân với các hệ số nguyên và biệt thức cố định (xem [**22**, § 230]).

Nhưng cả Gauss lẫn Dirichlet đều không sử dụng ngôn ngữ của các nhóm. Chính Dedekind, khi trình bày các công trình này vào năm 1879, đã nhận ra vai trò tiềm ẩn của chúng và định nghĩa khái niệm đặc trưng cho các nhóm giao hoán. Các nhận xét của Dedekind được H. Weber khuếch đại đáng kể, trước hết vào năm 1882 [**77**], sau đó vào năm 1886 [**78**, p. 112], nơi ông đưa vào nhóm đối ngẫu của một nhóm giao hoán hữu hạn A và nhận xét rằng nó đẳng cấu với A. Mục đích của ông khi đó là xây dựng các mở rộng Abel của trường $\mathbf{Q}$ với nhóm Galois cho trước, và ông không xét bài toán giải tích điều hòa trên một nhóm như vậy.

Trong trường hợp các nhóm không giao hoán, nền tảng của lý thuyết biểu diễn của các nhóm hữu hạn đã được thiết lập vững chắc vào khoảng thời điểm chuyển sang thế kỷ xx$^e$, tiếp theo các công trình của G. Frobenius, W. Burnside và I. Schur (xem ÉHM, p. 154). Sau năm 1905, người ta đã rõ rằng các quan hệ trực giao của các đặc trưng đóng một vai trò cốt yếu trong việc tổ chức lý thuyết. Nhưng mối quan hệ gần gũi của chúng với giải tích điều hòa vẫn còn ẩn giấu.

Chính Hermann Weyl là người đã nối các lĩnh vực này, khi ông hình thành ý tưởng về một lý thuyết tổng quát của các biểu diễn cho các nhóm compact. Trong một số văn bản lớn được xuất bản từ năm 1925 đến năm 1927, ông đã nhận ra các mối liên hệ sẽ hợp nhất một lý thuyết như vậy với giải tích Fourier và lý thuyết phổ Hilbert, và ông đã đặt nền móng cho nhiều khám phá tiếp theo.

Chính một bức thư của Schur đã đưa Weyl đi theo con đường này, nhờ mối quan tâm chung của họ đối với lý thuyết bất biến. Chúng tôi đã mô tả, trong chú ý về độ đo Haar (ÉHM, p. 289–291), cách mà A. Hurwitz đã hình thành ngay từ năm 1897 ý tưởng sử dụng một “tích phân bất biến” để xác định các đa thức trên $\mathbf{R}^n$ bất biến dưới nhóm trực giao. Dường như Schur không biết các kết quả của Hurwitz trước năm 1924, khi ông đột nhiên hiểu rằng tích phân bất biến cho phép mở rộng sang nhóm $\mathbf{O}(n)$ lý thuyết các đặc trưng và các quan hệ trực giao mà ông đã thiết lập cho các nhóm hữu hạn. Weyl ngay lập tức thấy rằng các phương pháp của Schur, kết hợp với công trình của Élie Cartan, cho phép xây dựng các biểu diễn bất khả quy của các nhóm Lie compact nửa đơn. Chuỗi ba hồi ký trong đó Weyl kết hợp các ý tưởng của Cartan và Schur, được xuất bản năm 1925 [**83**], đã chứa phần cốt yếu của các kết quả của LIE, IX, §6-7; xem ÉHM, p. 328–330.

Nhưng chính vào năm sau, trong một văn bản cũng không kém phần nổi tiếng được viết cùng học trò của mình F. Peter [**54**], Weyl đã làm sáng tỏ các mối liên hệ giữa lý thuyết các biểu diễn của các nhóm compact, giải tích Fourier và lý thuyết phổ Hilbert. Văn bản này chưa đầy hai mươi trang nhưng chứa đựng trong mầm mống rất nhiều phát triển tương lai.

Peter và Weyl tự giải phóng khỏi mọi giả thiết đại số về cấu trúc của nhóm được nghiên cứu, chỉ giả sử rằng G là một nhóm tôpô compact được trang bị một độ đo bất biến. Sự tồn tại của một độ đo như vậy là hiển nhiên đối với các nhóm Lie liên thông; chẳng bao lâu sau A. Haar sẽ thiết lập nó trong trường hợp tổng quát, một phần được thúc đẩy bởi các kết quả được trình bày ở đây (cf. ÉHM, p. 291).

Điểm khởi đầu của nghiên cứu của họ là tính trực giao của các hệ số ma trận. Schur đã nhận xét rằng bằng cách chọn một đại diện $\pi \in \widehat{G}$ cho mỗi lớp tương đương của các biểu diễn bất khả quy, một tích vô hướng bất biến bởi G trên không gian E của $\pi$, và một cơ sở trực chuẩn của E, ta thu được một họ các hệ số ma trận trực chuẩn trong $L^2(G)$. Peter và Weyl muốn chứng minh rằng một họ như vậy là toàn phần.

Trong trường hợp các nhóm hữu hạn, kết quả tương tự đã được Frobenius chứng minh bằng cách nghiên cứu đại số nhóm $\mathbf{C}[G]$. Khi đó Peter và Weyl xét không gian $\mathscr{C}(G)$ các hàm liên tục trên G và trang bị cho nó tích chập. Dường như đây là lần đầu tiên tích chập được sử dụng như một phép toán trừu tượng trong mối liên hệ tường minh với cấu trúc nhóm (cf. ÉHM, p. 295). Peter và Weyl hơn nữa gọi Gruppenzahl (“số nhóm”) là một phần tử của đại số $\mathscr{C}$(G), và ký hiệu $xy$ là tích (chập) của hai Gruppenzahlen. Họ cũng trang bị cho $\mathscr{C}(G)$ phép đối hợp $f\mapsto \widetilde{f}$, trong đó $\widetilde{f}(g) =f(g^{-1})$ với $g\in G$.

Sau khi đã đưa vào đại số đối hợp $\mathscr{C}$(G) như vậy, nhận xét đầu tiên của Peter và Weyl là mọi biểu diễn unita $\pi$ của G đều sinh ra một biểu diễn $f\mapsto \pi (f)$ của $\mathscr{C}(G) ($cf. V, p. 400). Khái niệm phần tử Hermit của $\mathscr{C}(G)$ được định nghĩa một cách tường minh, và tương tự (một cách ngầm định) là khái niệm phần tử dương, mở ra con đường cho việc áp dụng các kỹ thuật Hilbert.

Peter và Weyl không còn do dự khi gọi toán tử $\pi (f)$ là “hệ số Fourier” của $f$, và họ tiếp tục sự song song với lý thuyết Fourier bằng cách nhận xét rằng các hệ thức trực giao của Schur kéo theo bất đẳng thức Bessel

(6) $\sum_{\pi\in\widehat{G}}$ dim($\pi$ ) Tr($\pi (f)\pi (f)^*$)$\leqslant (f*\widetilde{f})(e) =\|f\|^2_2$.

Lý thuyết phổ Hilbert–Schmidt sau đó cho phép họ chứng minh rằng đây là một đẳng thức (“công thức Plancherel”). Với mỗi phần tử $\varphi$ của $\mathscr{C}$ (G), Peter và Weyl liên kết với nó hạt nhân liên tục $K_{\varphi}: G\times G\rightarrow \mathbf{C}$ được xác định bởi $K_{\varphi}(x, y) =\varphi (xy^{-1})$. Khi đó họ nhận xét rằng nếu $\varphi$ có dạng $f*\widetilde{f}$ với $f\in \mathscr{C}(G)$,[^6] thì $K_{\varphi}$ là một hạt nhân Hermit dương theo nghĩa của lý thuyết Hilbert–Schmidt. Một biến thể của thuật toán Schmidt[^7] sau đó cho phép họ xây dựng một cơ sở trực chuẩn của các hàm riêng của hạt nhân $K_{\varphi}$, rồi rút gọn chứng minh của đẳng thức trong (6) về sự kiện rằng vết của toán tử xác định bởi $K_{\varphi}$ bằng tổng các giá trị riêng của nó.

Hiển nhiên, chỉ các biểu diễn $\pi$ thỏa mãn $\pi (f)\not = 0$ mới có thể xuất hiện trong (6); lý thuyết phổ đối với $K_{\varphi}$ chỉ ra sự tồn tại của một biểu diễn như vậy nếu $f$ không đồng nhất bằng không. Peter và Weyl dễ dàng suy ra từ đó rằng các biểu diễn bất khả quy phân ly các điểm của G — một trường hợp riêng của định lý Gelfand–Raikov, sẽ được thảo luận sau.

Trong công trình nổi tiếng của Frobenius, một đẳng thức tương tự như (6) đã cho phép chứng minh rằng biểu diễn chính quy của G chứa tất cả các biểu diễn bất khả quy. Nhưng vấn đề là áp dụng đẳng thức này bằng cách lấy $f$ là phần tử đơn vị của $\mathbf{C}[G]$; khi đó hiển nhiên ta có $\pi (f)\not = 0$ đối với mọi $\pi$. Theo Peter và Weyl, sự thiếu vắng một phần tử đơn vị đối với phép chập giải thích nhiều khó khăn trong chứng minh của họ; tuy vậy họ nhận xét, mượn từ lý thuyết chuỗi Fourier một ý tưởng được định sẵn có một tương lai lớn, rằng người ta có thể suy ra kết quả tương tự của Frobenius bằng cách áp dụng (6) cho một dãy các hàm tạo thành một phần tử đơn vị xấp xỉ đối với phép chập (cf. No.$^o10$ of I, p. 120).

Tương tự, bắt đầu từ đẳng thức thu được từ (6), dạng phân cực

(7) $\sum_{\pi\in\widehat{G}}$ dim($\pi$ ) Tr($\pi (x)\pi (y)$) $= (x*y)(e)$

cho phép thu được, bằng cách lấy $y$ là một phần tử đơn vị xấp xỉ đối với phép chập, một sự xấp xỉ đều của mọi phần tử của $\mathscr{C}(G)$ bởi các tổ hợp tuyến tính của các hệ số ma trận của các biểu diễn bất khả quy. Các phương pháp này đã cho phép Weyl đưa ra một chứng minh mới [**84**] cho kết quả cơ bản của lý thuyết “các hàm gần tuần hoàn” của H. Bohr, mà ta sẽ trở lại trong chốc lát. Peter và Weyl chỉ ra rằng ở đó có thể đọc thấy ứng dụng giải tích đầu tiên của lý thuyết các biểu diễn của một nhóm không compact, ở đây là nhóm các phép tịnh tiến của $\mathbf{R}$.

Lý thuyết lượng tử non trẻ rất nhanh chóng đem lại cho Weyl cơ hội trở lại với các biểu diễn của $\mathbf{R}$. Vào cuối năm 1927, ông đã chỉ ra sự quan tâm của các nhóm (hữu hạn hoặc không) và các biểu diễn đối với việc làm sáng tỏ các nền tảng của lý thuyết này [**85**]. Ông trở lại vấn đề này vào năm sau, trong một cuốn sách nổi tiếng [**86**].

Trong bài báo năm 1927 của mình, Weyl nhận xét rằng nếu $u$ là một toán tử tự liên hợp liên tục trên một không gian Hilbert, thì $t\mapsto e^{itu}$ là một biểu diễn unita của $\mathbf{R}$. Nhưng tồn tại các biểu diễn unita của $\mathbf{R}$ không có dạng này; tiếp nhận ý tưởng của von Neumann về vai trò của các toán tử đối xứng từng phần trong việc biểu diễn các đại lượng vật lý quan sát được, Weyl cho rằng mọi biểu diễn unita của $\mathbf{R}$ đều có dạng $t\mapsto e^{itu}$, trong đó $u$ là một toán tử từng phần tự liên hợp trên một không gian Hilbert. Quan điểm này cho phép ông rút gọn việc giải tích các “quan hệ chính tắc” của Heisenberg và Schrödinger, vốn đã được von Neumann nghiên cứu chi tiết, về việc nghiên cứu các liên hệ giữa hai biểu diễn unita của $\mathbf{R}$ trên cùng một không gian Hilbert. Stone [**73**] chứng minh năm 1932 kết quả mà Weyl mong đợi (V, p. 428, Định lý 1), tiếp nối từ nghiên cứu của ông về các tính chất phổ của các toán tử tự liên hợp.

### 6. Các nhóm giao hoán compact địa phương

Sự tương tác giữa giải tích điều hòa và các biểu diễn nhóm do đó đã được thiết lập vững chắc vào đầu những năm 1930. Nó được củng cố mạnh mẽ trong thập niên tiếp theo, mỗi một trong hai chủ đề đều đem lại những tiến bộ nhanh chóng cho chủ đề kia.

Một trường rất màu mỡ cho sự tương tác này là việc nghiên cứu các hàm gần tuần hoàn, được H. Bohr đưa vào năm 1924 trong trường hợp các hàm của một biến thực [**9**]. Theo một trong các định lý cơ bản của ông, đây là các hàm liên tục bị chặn là các giới hạn đều trên $\mathbf{R}$ của các tổ hợp tuyến tính của các hàm $x\mapsto e^{i\lambda x},\lambda \in \mathbf{R}($cf. II, p. 292, bài tập 54). Bochner [**6**] đã chứng minh năm 1926 rằng một hàm $f\in \mathscr{C}_b(\mathbf{R})$ là gần tuần hoàn khi và chỉ khi các phép tịnh tiến của nó $x\mapsto f(x-a)$, với $a\in \mathbf{R}$, tạo thành một tập con tương đối compact của $\mathscr{C}_b(\mathbf{R})$ đối với tôpô hội tụ đều. Bochner và von Neumann nhận xét rằng nếu G là một nhóm tôpô, thì đặc trưng hóa này hiển nhiên cung cấp một khái niệm về hàm gần tuần hoàn (bên phải hoặc bên trái) trên G. Vào đầu những năm 1930, lý thuyết này hứa hẹn sẽ phát triển nhanh chóng, đặc biệt dưới sự thúc đẩy của von Neumann [**52**] và các phương pháp của Peter và Weyl.

Một trường ưu tiên khác xuất hiện bên lề công trình của N. Wiener. Ông đưa vào, trong một bài báo nổi tiếng [**88**] năm 1932, các phương pháp có bản chất đại số trong việc nghiên cứu các bài toán Tauber — tức là, trong việc nghiên cứu hành vi tiệm cận của một hàm (hoặc một dãy) theo một bộ lọc, với thông tin cho trước về hành vi của một số trung bình có trọng số. Cách tiếp cận của ông được thúc đẩy bởi một ý tưởng của R. Schmidt.

Một trong các kết quả phụ trợ của công trình của Wiener ([**88**, Bổ đề IIe]) đặc biệt gây ấn tượng và đã truyền cảm hứng cho nhiều phát triển: nếu $f$ là một hàm tuần hoàn mà chuỗi Fourier của nó hội tụ tuyệt đối, và nếu $f$ không triệt tiêu, thì chuỗi Fourier của $1/f$ hội tụ tuyệt đối (cf. I, p. 38, ví dụ). Ngay từ năm 1932, R. Paley và N. Wiener [**89**] đã phác thảo mối liên hệ giữa kết quả hội tụ này, khái niệm nhóm đối ngẫu đối với một nhóm giao hoán rời rạc, và lý thuyết các hàm gần tuần hoàn.

Trên nền tảng giải tích này, chính tôpô đại số đã dẫn L. Pontryagin đưa ra động lực quyết định cho việc nghiên cứu các đặc trưng của các nhóm Abel compact địa phương. Ông công bố ngay từ năm 1932 [**55**] sự quan tâm của khái niệm nhóm đặc trưng trong việc đặt đối ngẫu các nhóm đồng điều của một tập con compact của không gian Euclid và các nhóm của phần bù của nó. Trong một bài báo [**58**] xuất bản năm 1934, ông chỉ ra rằng nhóm đặc trưng của một nhóm rời rạc là compact, sau đó thiết lập các định lý đối ngẫu trong bối cảnh này. Mặc dù Pontryagin sử dụng các kết quả của Peter và Weyl, cũng như độ đo Haar mà sự tồn tại của nó vừa được thiết lập một cách tổng quát, ông chủ yếu hướng tới các ứng dụng vào tôpô [**57**] và không quan tâm một cách tường minh đến giải tích điều hòa[^8]: các định lý đối ngẫu được chứng minh bằng một nghiên cứu tinh tế về cấu trúc của các nhóm Abel compact.

Công trình của Pontryagin ngay lập tức thu hút sự quan tâm lớn. Theo đề nghị của von Neumann, E. van Kampen mở rộng đối ngẫu vào năm sau cho mọi nhóm giao hoán compact địa phương [**37**]. Ngay sau đó, ông đưa ra một ứng dụng gây ấn tượng của giải tích bất biến mới vào việc nghiên cứu các hàm gần tuần hoàn [**38**], được A. Weil phát hiện độc lập trong cùng thời kỳ [**79**]: nếu G là một nhóm giao hoán compact địa phương, ta thu được một nhóm compact $\widetilde{G}$ bằng cách trước hết trang bị cho nhóm đối ngẫu $\widehat{G}$ tôpô rời rạc, sau đó xác định $\widetilde{G}$ là nhóm đối ngẫu compact của nhóm rời rạc thu được như vậy. Khi đó nhóm G nhúng một cách chính tắc vào $\widetilde{G} ($cf. II, p. 292, bài tập 54) và một ứng dụng đơn giản của lý thuyết Peter–Weyl cho các hàm liên tục trên $\widetilde{G}$ cung cấp tất cả các kết quả đã biết vào thời điểm đó về các hàm gần tuần hoàn trên G.

Đồng thời, các hàm xác định dương, vốn đã được biết rõ trong giải tích cổ điển, xuất hiện trong giai đoạn này trong việc nghiên cứu các biểu diễn đơn vị của $\mathbf{R}$. Khái niệm hạt nhân dương phổ quát đã được J. Mercer [**45**] nghiên cứu ngay trước năm 1910, liên quan đến lý thuyết các phương trình tích phân, trong khi dạng tương tự của nó đối với các dãy đã làm nảy sinh khá nhiều công trình trong cùng thời kỳ, liên quan đặc biệt đến bài toán mômen (xem IV, p. 359, exerc. 21). Trong khi đó, các hàm xác định dương trên $\mathbf{R}$, đã được M. Mathias [**43**] nghiên cứu một cách hệ thống từ năm 1923, đã trở thành trong tay Bochner một trong những công cụ cơ bản của giải tích Fourier và lý thuyết xác suất [**7**]. Năm 1933, Bochner [**8**] và Riesz [**61**] độc lập nhận thấy rằng mọi hệ số ma trận đường chéo của một biểu diễn đơn vị của $\mathbf{R}$ đều là một hàm xác định dương trên $\mathbf{R}$. Nhận xét này cho phép họ đưa ra một chứng minh đơn giản hơn cho định lý Stone, và sẽ có ảnh hưởng quyết định đến sự phát triển của lý thuyết tổng quát (xem n$^o7$).

Các kết quả của thời kỳ này được A. Weil sắp xếp lại, trong một cuốn sách hoàn thành trước năm 1937 và xuất bản năm 1940 [**80**]. Ông trình bày ở đó một cách chi tiết các kết quả của Peter–Weyl, Pontryagin và van Kampen. Nhưng trong trường hợp các nhóm giao hoán, trong khi Pontryagin và van Kampen nhấn mạnh cấu trúc của các nhóm và các định lý đối ngẫu, Weil phát triển một cách có hệ thống giải tích điều hòa, đưa vào biến đổi Fourier và chứng minh công thức Plancherel cùng định lý Bochner (V, p. 455, th. 5). Đặc biệt, ông nhấn mạnh vai trò của tích chập (dưới tên gọi “tích hợp thành”) và vai trò của các hàm xác định dương, từ đó về sau được định nghĩa trên một nhóm tùy ý và liên quan đến các hệ số ma trận đường chéo của các biểu diễn, ít nhất trong trường hợp các biểu diễn hữu hạn chiều.

Tính tổng quát đạt được như vậy trong trường hợp giao hoán sẽ mở ra một thời gian ngắn sau những chân trời mới trong lý thuyết số. Ngay từ năm 1936, nhằm đưa các phương pháp đại số vào lý thuyết trường lớp, C. Chevalley [**14**] đưa vào nhóm các idèle của một trường số, nhóm này về sau sẽ xuất hiện như nhóm các phần tử khả nghịch của vành các adèle (xem AC, VII, p. 221–222, và ÉHM, p. 143). Năm 1950, J. Tate [**75**] sẽ chỉ ra rằng giải tích điều hòa đối với các nhóm adèle và idèle cho phép dễ dàng thu được các phương trình hàm của các hàm L của Hecke, báo trước những phát triển phi thường liên kết giải tích điều hòa trên các nhóm adelic và việc nghiên cứu các dạng tự đẳng cấu.

Nhưng có thể nói rằng vào cuối những năm 1930, các kết quả chính của giải tích điều hòa bất biến đã thu được đối với các nhóm compact và đối với các nhóm giao hoán compact địa phương. Trong trường hợp giao hoán, các chứng minh của Weil vẫn phụ thuộc (cũng như các chứng minh của Pontryagin và van Kampen) vào sự hiểu biết tinh tế về cấu trúc của nhóm, nghĩa là, nói một cách gần đúng, vào các kết quả phân loại của § 2 của II, p. 244. Thập niên tiếp theo sẽ cho thấy cách thoát khỏi điều này, nhờ các phương pháp mới của trường phái Gelfand (xem H. Cartan và R. Godement [**12**]).

### 7. Đại số toán tử

Ta đã thấy vai trò mà Riesz, khi trình bày vào năm 1913 các công trình của trường phái Hilbert, gán cho đại số $\mathscr{L}(E)$ của các tự đồng cấu của một không gian Hilbert, cũng như cho phép tính phiếm hàm chỉnh hình và cho khái niệm trừu tượng về phổ. Trong hồi ký năm 1916 của mình, ông dường như đã báo trước các đại số chuẩn như một cách đặt tự nhiên cho lý thuyết phổ; sau các công trình của Banach và trường phái của ông trong những năm 1920, không có gì đáng ngạc nhiên khi ý tưởng này chiếm một vị trí trung tâm. Khái niệm đại số Banach được M. Nagumo [**48**] đưa vào năm 1936, trong khi S. Mazur [**44**], năm 1938, chứng minh rằng đại số có chuẩn duy nhất trên $\mathbf{C}$ đồng thời là một trường chính là $\mathbf{C}$ (I, p. 26, cor. 2).

Vào khoảng giữa những năm 1930, liên quan đến lý thuyết phổ, những dịp xem xét một cách trừu tượng các đại số của các toán tử trên các không gian Hilbert trở nên ngày càng thường xuyên hơn. F. Murray và J. von Neumann, trong một loạt các công trình sâu sắc và có ảnh hưởng [**47**], nghiên cứu một cách hệ thống các đại số con có phép đối hợp của $\mathscr{L}(E)$ bằng với đối giao hoán tử kép của chúng (“các đại số von Neumann”). Mặt khác, năm 1936, S. Steen đề xuất đưa vào một khái niệm tiên đề về “đại số toán tử” và nghiên cứu sâu các cấu trúc liên kết tương ứng [**70**]. Ngoài ra, Stone [**74**], được thúc đẩy bởi việc nghiên cứu các phép chiếu phổ, nghiên cứu năm 1937 các đại số có đơn vị mà mọi phần tử của chúng đều lũy đẳng (“các đại số Boolean”: xem ÉHM, p. 146). Ông nhận xét rằng nếu X là một không gian tôpô compact địa phương, các hàm đặc trưng của các tập mở và các hàm đặc trưng của phần bù của các tập trù mật khắp nơi sinh ra, trong $\mathscr{C}$ (X), một đại số Boolean A. Sau đó ông chứng minh rằng các iđêan của A tương ứng một cách tự nhiên với các tập đóng của không gian X, qua đó đưa vào một ý tưởng sẽ tỏ ra đặc biệt phong phú.

Từ năm 1939 trở đi, quan điểm của Gelfand mở ra những viễn cảnh mới về các kết quả tương đối rời rạc này. Công trình của ông dường như được thúc đẩy một phần bởi các ý tưởng của Wiener, đặc biệt bởi định lý của ông liên quan đến các chuỗi Fourier hội tụ tuyệt đối, cũng như bởi các phương pháp của Peter và Weyl. Giữa năm 1939 và 1946, trong sự hợp tác với M. Naimark, D. Raikov và G. Shilov, Gelfand xây dựng những nền tảng của lý thuyết các đại số Banach giao hoán và của lý thuyết các đại số sao (xem [**23**], vol. I, p. 169–400). Đặc biệt, ông đưa ra chứng minh cổ điển của định lý Wiener — được P. Lévy [**39**] tổng quát hóa — được trình bày trong cuốn sách này (I, p. 38, ví dụ).

Trong cách tiếp cận của Gelfand, đối tượng cốt yếu mà một đại số Banach giao hoán $A$ liên hệ tới là không gian $X$ của các iđêan cực đại của $A$. Thật vậy, bằng định lý Gelfand–Mazur (I, p. 26, cor. 2), mọi phần tử của $A$ xác định một hàm trên $X$. Tầm quan trọng to lớn mà quan điểm này sẽ có trong sự phát triển tiếp theo của hình học đại số đã được biết rõ (cf. ÉHM, p. 146–148). Bản thân cách tiếp cận này được thúc đẩy bởi công trình của Stone về các đại số Boolean đã được đề cập ở trên.

Dường như chính L. Loomis, trong một giáo trình xuất bản năm 1953 [**41**, p. 53], là người đầu tiên trình bày lý thuyết của Gelfand bằng cách nhấn mạnh không gian các ký tự của $A$, định nghĩa biến đổi Gelfand theo nghĩa mà chúng ta hiểu trong cuốn sách này. Ưu điểm rõ ràng nhất của quan điểm này chắc chắn là các tính chất tôpô của không gian các ký tự suy ra ngay lập tức từ tính compact của quả cầu đơn vị của đối ngẫu của một không gian Banach đối với tôpô yếu.

Ngay từ các công trình đầu tiên của mình, Gelfand đã xây dựng phép tính phiếm hàm chỉnh hình ánh xạ trong một biến trong một đại số Banach, bằng tích phân của Cauchy, và đã suy ra từ đó rằng một đại số Banach đối hợp có một phân tích không tầm thường thành một tích các vành khi không gian các iđêan cực đại của nó không liên thông. Trường hợp của một đại số Banach tùy ý chỉ được xét đến năm 1953, khi Shilov phát triển một dạng của phép tính phiếm hàm trong nhiều biến [**68**].

Đối với các đại số sao, mà Gelfand và Naimark đã chỉ ra ngay từ năm 1942 rằng có thể được thực hiện như các đại số của các toán tử trên một không gian Hilbert (cf. V, p. 442, th. 2), chúng nhanh chóng trở thành đối tượng của những nghiên cứu phong phú và sâu sắc, được thúc đẩy bởi các ứng dụng vào các biểu diễn nhóm, bởi công trình của Murray và von Neumann, và bởi sự hình thức hóa toán học của Cơ học lượng tử. Đặc biệt, hãy nhắc đến các đóng góp của I. Segal, người là một trong những người tiên phong trong việc nghiên cứu có hệ thống các biểu diễn của các đại số sao, liên quan đến việc nghiên cứu đối ngẫu đơn vị của các nhóm compact địa phương mà chúng ta sẽ bàn đến trong vài dòng nữa.

Mặc dù Gelfand, Naimark, Raikov và Shilov đã thiết lập các nền tảng cốt yếu của lý thuyết các đại số sao trước năm 1946, một số điểm kỹ thuật đã được cải tiến sau đó. Chẳng hạn, R. Arens [**1**] đã chỉ ra cách tránh việc viện dẫn sự tồn tại của “biên Shilov” (cf. I, p. 171, exerc. 26) để chứng minh rằng biến đổi Gelfand là một cấu xạ đối hợp. Hơn nữa, lý thuyết của Gelfand và Naimark cho các đại số sao có đơn vị ban đầu thêm vào như một tiên đề sự kiện rằng $1 +x^*x$ khả nghịch với mọi $x$. Tuy vậy họ vẫn phỏng đoán rằng tiên đề này là không cần thiết; chứng minh của mệnh đề này, sơ cấp nhưng tinh tế, chỉ được đưa ra vào khoảng năm 1952, theo sau công trình của M. Fukamiya [**21**] được I. Kaplansky [**62**] tiếp tục.

### 8. Các biểu diễn của các nhóm compact địa phương

Cho đến năm 1939, việc nghiên cứu các biểu diễn của các nhóm tôpô bị giới hạn vào trường hợp compact và trường hợp giao hoán. Về phần mình, các nhà vật lý đã tìm thấy trong Cơ học lượng tử nhiều lý do để nghiên cứu các biểu diễn đơn vị bất khả quy nhằm tìm kiếm các không gian Hilbert có khả năng mô hình hóa các trạng thái của các hạt cơ bản. P. Dirac, dựa trên công trình của E. Majorana, đã chỉ ra khoảng năm 1936 sự quan trọng, từ quan điểm này, của nhóm Lorentz $\mathbf{S}\mathbf{O}(3,1)$ và nhóm Poincaré $\mathbf{S}\mathbf{O}(3,1)\ltimes \mathbf{R}^4$. Các phương pháp của họ vẫn còn rất xa với các phương pháp của các nhà toán học đương thời. Nhưng năm 1939, E. Wigner đã mở ra một hướng mới [**90**] khi ông phân loại các biểu diễn đơn vị bất khả quy của nhóm Poincaré bằng cách dựa vào công trình của Murray và von Neumann.

Dường như chính Gelfand là người ta ghi nhận đã nhận thấy một con đường tổng quát hướng tới việc nghiên cứu các biểu diễn của các nhóm compact địa phương. Trong một hồi ký viết năm 1942 (cf. [**23**], vol. II, p. 3–17), ông chỉ ra cùng với Raikov rằng một lý thuyết như vậy có thể thực hiện được nhờ mối liên hệ giữa các biểu diễn đơn vị và các hàm kiểu dương. Họ chứng minh sự tồn tại của một thực hiện Hilbert cho mọi hàm kiểu dương (V, p. 432, th 1) và suy ra từ đó rằng các biểu diễn đơn vị bất khả quy tách các điểm của G (V, p. 454, th. 4). Các dạng tuyến tính dương trên đại số đối hợp $L^1(G)$ đóng một vai trò cốt yếu: Gelfand và Raikov chỉ ra mối liên hệ nối chúng với các hàm kiểu dương (cf. V, p. 448, prop. 13). Đại số sao bao quanh của một đại số đối hợp được trình bày (không có tên) trong [**24**, § 48], mặc dù khi đó chưa có vấn đề trực tiếp về việc liên kết với G đại số Stell(G) (cf. 9, déf. de I, p. 125).

Sau năm 1945, việc nghiên cứu các biểu diễn đơn vị phát triển với những bước tiến lớn. Sự tương tác với các đại số sao, cũng như với việc phân tích các nền tảng của lý thuyết lượng tử, nhanh chóng cung cấp những kết quả tổng quát có giá trị: khoảng năm 1947, Segal liên kết nhiều[^9] đại số sao với một nhóm compact địa phương [**67**], và dệt nên mối liên hệ giữa các biểu diễn của chúng và các biểu diễn của nhóm được xét. Không lâu sau đó, G. Mackey đưa ra khái niệm biểu diễn cảm sinh [**42**], khái niệm này sẽ hiện diện khắp nơi trong các kết quả cụ thể về các biểu diễn đơn vị.

Đồng thời, lý thuyết này đã được thúc đẩy đáng kể bởi việc nghiên cứu các ví dụ làm bộc lộ tính đa dạng và chiều sâu của nó. Gelfand và Naimark, nghiên cứu ví dụ $\mathbf{S}\mathbf{L}(2,\mathbf{C})$, đã đưa ra vào năm 1947 một trường hợp riêng của khái niệm biểu diễn cảm sinh, sau đó chỉ ra rằng nó là chìa khóa cho việc nghiên cứu các biểu diễn của nhóm này [**23**, vol. II, p. 41– 124]. Cũng trong năm đó, V. Bargmann đã nghiên cứu [**5**] nhóm $\mathbf{S}\mathbf{L}(2,\mathbf{R})$ và phát hiện sự tồn tại của một họ đếm được các biểu diễn khả tích bình phương, được gọi là “chuỗi rời rạc” (discrete series), cũng như các quan hệ trực giao giữa các hệ số ma trận của chúng (xem mđ. 8 của V, p. 424). Như Godement đã ngay lập tức nhận ra [**25**], các quan hệ trực giao của Bargmann được thỏa mãn bởi mọi biểu diễn khả tích bình phương của các nhóm compact địa phương.

Chẳng bao lâu sau, việc nghiên cứu các lớp riêng của các nhóm lại sẽ được ưu tiên hơn lý thuyết trừu tượng, và điều này kéo dài trong một thời gian dài. Đặc biệt, Harish-Chandra sẽ bắt đầu nghiên cứu tổng quát các biểu diễn của các nhóm Lie khả quy — một nhiệm vụ đồ sộ mà chúng ta không thể mô tả ở đây, cũng như không thể mô tả những hệ quả phi thường mà Langlands sẽ tiên liệu đối với lý thuyết số.

[^1]: Hãy nhắc lại rằng chính Poincaré, được dẫn dắt bởi bài toán về “các màng rung động” trong đó khái niệm trị riêng đóng vai trò cốt yếu, đã đưa vào một tham số $\lambda$ trong (1) và đề nghị nghiên cứu sự phụ thuộc vào $\lambda$ của các nghiệm (xem ÉHM, p. 262).
[^2]: Đối với Hilbert, quan hệ xác định các giá trị và vectơ riêng là đẳng thức $\varphi_n(t) =\lambda_n\int_IK(s, t)\varphi_n(s)ds$; do đó các “trị riêng” mà ông nhắc đến là các nghịch đảo của những trị được thuật ngữ hiện đại công nhận, và có thể là vô hạn. Như ta sẽ thấy, sự thay đổi này đã được F. Riesz đề xuất vào năm 1913.
[^3]: Như Hilbert nhận xét, ta có thể đặc trưng $\sigma (s, x) =\sum_{p,q=0}^{\infty}\sigma_{pq}(s)x_px_q$ bởi tính chất nó thỏa mãn $\int_{\mathbf{R}}d\sigma (s, x) =\|x\|^2$ và rằng đối với mọi hàm liên tục $u$ trên $\mathbf{R}$, ta có $\sum_{r=0}^{\infty}\int_{\mathbf{R}}u(s)d\sigma_{pr}(s)\int_{\mathbf{R}}u(s)d\sigma_{rq}(s) =\int_{\mathbf{R}}u(s)^2d\sigma_{pq}(s)$.
[^4]: Sự tương đương này vẫn đúng trong trường hợp không gian Banach phản xạ, nhưng nói chung hai khái niệm này khác nhau: xem III, p. 7, mđ. 8.
[^5]: Khái niệm này đã được các nhà đại số học biết đến vào cuối thế kỷ xix$^e$ và được Toeplitz [**76**] sử dụng trong một đặt giải tích vào năm 1918.
[^6]: Đây là dạng tổng quát của một phần tử dương của $\mathscr{C}$(G), xem n$^o2$ của I, p. 118.
[^7]: Đây là thuật toán cho phép Schmidt, lấy cảm hứng từ công trình của Schwarz và xét các “lặp” của hạt nhân $K_{\varphi}$, đơn giản hóa các kết quả của Fredholm và Hilbert trong luận án của ông năm 1905.
[^8]: Điều này không có nghĩa là Pontryagin đã xem nhẹ Giải tích: trong một chú ý ngắn [**56**] năm 1933, đính kèm với một đóng góp của Stepanoff và Tychonoff liên quan đến các hàm gần tuần hoàn trên $\mathbf{R}$, ông đã viết lại kết quả của họ bằng hai nhóm Abel đối ngẫu.
[^9]: Ngay từ năm 1941, Segal đã đề nghị liên kết một đại số Banach với một nhóm G như vậy để nghiên cứu các biểu diễn; nhưng vào thời điểm đó ông thực ra nghĩ đến đại số thu được từ $L^1(G)$ bằng phép nối một phần tử đơn vị. Năm 1947, trong một bài báo có ảnh hưởng, ông đã liên kết một đại số sao với G nhằm mục đích phân tích biểu diễn chính quy; cái mà ông đưa vào khi đó thực ra là đại số sao “thu gọn”, thương của Stell(G) bởi hạt nhân của biểu diễn chính quy, chứ không phải bản thân đại số sao phổ quát. Đại số sau dường như xuất hiện dưới dạng hiện đại của nó vào năm 1960 trong một văn bản của J. Fell [**20**].
