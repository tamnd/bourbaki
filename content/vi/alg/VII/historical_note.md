---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 0
section_title: Historical Note
kind: historical
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0432-0460
extraction: ocr
statements: 0
exercises: 0
content_sha256: d84370a7419342d539b368495017af96ae144456f43f89867b19297edaee0999
translated_from: content/en/alg/VII/historical_note.md
source_content_sha256: 0badcac98496c7f98609a5c39885b447949598116e8182f2d00bd1c60192a86d
translation_model: gpt-5.4-mini
translation_run: translate-vi-e22569be
glossary_version: 34
glossary_terms_sha256: 05521e2a7a83e998a82cad6501cf7cc66fb1d3611689501ae0b5165e95d3f721
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

# GHI CHÚ LỊCH SỬ

(Chương VI và VII)

(Chú ý. — Các số La Mã trong ngoặc đơn chỉ đến thư mục ở cuối ghi chú này.)

Các phép toán số học sơ cấp, đặc biệt là các phép toán với phân thức, tất yếu dẫn đến một số quan sát thực nghiệm về tính chia hết giữa các số nguyên. Nhưng dường như cả người Babylon (mặc dù họ là những chuyên gia về đại số), lẫn người Ai Cập (bất chấp kỹ xảo điêu luyện của họ trong việc thao tác với các phân thức) đều không quen với các quy tắc tổng quát chi phối những tính chất này, và sáng kiến theo nghĩa đó thuộc về người Hy Lạp. Công trình số học của họ, mà một trình bày bậc thầy có thể tìm thấy trong Quyển VII và IX của Euclid (I), hoàn toàn không kém gì những phát hiện đẹp nhất của họ ở các ngành khác của Toán học. Sự tồn tại của UCLN của hai số nguyên được chứng minh ngay ở đầu Quyển VII bằng thủ tục được gọi là « thuật toán Euclid » \* ; nó làm cơ sở cho toàn bộ các phát triển tiếp theo (các tính chất của số nguyên tố, sự tồn tại và cách tính BCNN, v.v.), dựa trên những lập luận không khác về bản chất so với những lập luận trong Ch. VI, § 1 ở trên ; và đỉnh cao là hai định lý đáng chú ý chứng minh sự tồn tại vô hạn của các số nguyên tố (Quyển IX, Mệnh đề 20) và đưa ra một phương pháp để xây dựng các số hoàn hảo chẵn (xem VII, p. 53, Bài tập 24 ; trên thực tế phương pháp này cho ra mọi số hoàn hảo chẵn, như Euler sẽ chứng minh). Chỉ có sự tồn tại và tính duy nhất của phân tích thành thừa số nguyên tố là không được chứng minh một cách tổng quát ; tuy nhiên Euclid có chứng minh tường minh rằng mọi số nguyên đều chia hết cho một số nguyên tố (Quyển VII, Mệnh đề 31), cũng như hai mệnh đề sau đây (Quyển IX, Mệnh đề 13 và 14) :

« Nếu bao nhiêu số cũng được xếp thành một cấp số, bắt đầu từ 1, với tỷ số không đổi [tức là cấp số nhân], và nếu số đứng sau 1 là nguyên tố, thì số lớn nhất sẽ không chia hết cho bất kỳ số nào ngoài những số xuất hiện trong cấp số ấy » (nói cách khác, một lũy thừa $p^n$ của một số nguyên tố $p$ chỉ có thể chia hết bởi những lũy thừa của $p$ có số mũ $\leq n$).

« Nếu một số là số nhỏ nhất chia hết cho [các] số nguyên tố [đã cho], thì nó sẽ không chia hết cho bất kỳ số nguyên tố nào khác ngoại trừ những số ban đầu [được cho là] chia hết nó » (nói cách khác, một tích của các số nguyên tố phân biệt $p_1, \ldots, p_k$ không có nhân tử nguyên tố nào khác ngoài $p_1, \ldots, p_k$).

Vì vậy dường như nếu Euclid không phát biểu định lý tổng quát, thì chỉ là vì thiếu một thuật ngữ và ký hiệu thích hợp cho các lũy thừa tùy ý của một số nguyên.*

Mặc dù một khảo cứu cẩn thận khiến người ta có thể nghĩ rằng văn bản của Euclid được cấu thành bởi nhiều lớp kế tiếp nhau, mỗi lớp tương ứng với một giai đoạn trong sự phát triển của Số học **, dường như sự tiến hóa này đã diễn ra hoàn toàn giữa đầu thế kỷ thứ 5 và giữa thế kỷ thứ 4 trước Công nguyên, và người ta phải khâm phục kỹ năng cũng như sự tự tin lôgic mà nó thể hiện: bước tiến tương đương tiếp theo trong Số học sẽ không xảy ra trong hai thiên niên kỷ.

Chính các bài toán gọi là « không xác định » hay « Diophantine » đã là cội nguồn của những phát triển tiếp theo trong Lý thuyết số. Thuật ngữ « phương trình Diophantine », như ngày nay được dùng, xét về mặt lịch sử không hoàn toàn chính xác; nó thường được hiểu là các phương trình đa thức (hoặc hệ phương trình) với hệ số nguyên, mà chỉ tìm các nghiệm nguyên: một bài toán thường là bất khả nếu các phương trình là « xác định », tức là chỉ có hữu hạn nghiệm (thực hoặc phức), nhưng mặt khác thường có nghiệm khi số ẩn nhiều hơn số phương trình. Nay, tuy Diophantus quả thật dường như là người đầu tiên xét các bài toán « không xác định », ông chỉ tìm nghiệm nguyên trong những trường hợp ngoại lệ, và thường chỉ bằng lòng với việc tìm một nghiệm duy nhất trong các số hữu tỉ (II). Đó là một kiểu bài toán mà ông thường có thể giải bằng các phép tính đại số, trong đó

\* Nếu $a_1$ và $a_2$ là hai số nguyên sao cho $a_1 \geq a_2$, ta định nghĩa đệ quy $a_n$ (với $n \geq 3$) là số dư khi chia $a_{n-2}$ cho $a_{n-1}$; nếu $m$ là chỉ số nhỏ nhất sao cho $a_m = 0$, thì $a_1$, $a_2$, là UCLN của $a_1$ và $a_2$. Đây là sự chuyển sang các số nguyên của phương pháp trừ liên tiếp (còn đôi khi được gọi là ἀνθυφαιρεσις) để tìm một ước chung của hai độ dài. Phương pháp sau hẳn có từ người Pythagore, và dường như đã là cơ sở của một lý thuyết về các số vô tỉ trước Eudoxus.

\* Để ủng hộ luận điểm này, cũng có thể nhận thấy rằng chứng minh của định lý về các số hoàn hảo về cơ bản chỉ là một trường hợp riêng khác của định lý phân tích duy nhất thành thừa số nguyên tố. Hơn nữa, mọi bằng chứng đều cho thấy rằng từ thời kỳ này trở đi việc phân tích một số cụ thể thành các số nguyên tố đã được biết rõ và đang được dùng rộng rãi; nhưng không thấy có một chứng minh đầy đủ nào của định lý phân tích trước chứng minh do Gauss đưa ra ở đầu Disquisitiones ((VIII) t. I, p. 15).

** Xem B. L. van der Waerden, Die Arithmetik der Pythagoreer, Math. Ann., vol. CXX (1947-49), p. 127. Một ví dụ về một đoạn còn lại từ một phiên bản trước được cung cấp bởi Mệnh đề 21 đến 34 của Quyển IX, vốn bàn về những tính chất sơ cấp nhất của tính chia hết cho 2, và hẳn là quay về một thời kỳ khi lý thuyết tổng quát về các số nguyên tố chưa được phát triển. Hơn nữa, người ta biết rằng hai phạm trù Chẵn và Lẻ đã đóng một vai trò lớn trong các suy tư siêu hình của những người Pythagore đầu thời, nên tự nhiên có thể muốn gán đoạn này cho họ.

tính chất số học của các ẩn không liên quan *; hơn nữa, lý thuyết về tính chia hết chỉ giữ một vai trò thứ yếu (từ chỉ số nguyên tố chỉ được dùng có một lần ((11), Quyển V, bài toán 9, vol. 1, pp. 334-335), và khái niệm các số nguyên tố cùng nhau chỉ được viện dẫn khi nói đến định lý khẳng định rằng thương của hai số nguyên tố cùng nhau chỉ có thể là một bình phương nếu mỗi số trong chúng là một bình phương) **.

Việc nghiên cứu các nghiệm nguyên của các phương trình vô định chỉ thực sự bắt đầu với các nhà toán học Trung Hoa và Hindu thời trung cổ sơ kỳ. Người Trung Hoa dường như đã bị dẫn đến những suy xét kiểu này bởi các bài toán thực hành về việc lập lịch (trong đó việc xác định các chu kỳ chung của nhiều chu kỳ hiện tượng thiên văn chính xác là một bài toán « Diophantine » tuyến tính); dẫu sao, chính họ (chắc chắn là giữa thế kỷ IV và thế kỷ VII sau Công nguyên) đã đưa ra một quy tắc giải các đồng dư tuyến tính đồng thời (cf. VI, p. 33, Ex. 25). Còn về phía người Hindu, mà Toán học của họ phát triển rực rỡ giữa thế kỷ V và thế kỷ XIII, họ không chỉ biết xử lý một cách có phương pháp (bằng cách áp dụng thuật toán Euclid) các hệ phương trình Diophant tuyến tính trong số ẩn tùy ý nhiều ***. mà họ còn là những người đầu tiên tấn công và giải các bài toán bậc hai, trong đó có một số trường hợp đặc biệt của « phương trình Fermat » Nx^2 + 1 = y^2 ((111), vol. II, pp. 87-307).

Ở đây không phải chỗ để chúng tôi khảo sát lịch sử của lý thuyết các phương trình Diophant bậc > 1, lý thuyết này, qua các công trình của Fermat, Euler, Lagrange và Gauss, đã dẫn tới lý thuyết các số nguyên đại số vào thế kỷ XIX. Như chúng tôi đã ghi nhận (cf. Ghi chú lịch sử cho Chương II và 111), việc nghiên cứu các hệ tuyến tính, vốn dường như không còn nêu ra những bài toán đáng quan tâm nữa, đã bị sao nhãng khá nhiều trong thời kỳ này: đặc biệt không hề có sự tìm kiếm các điều kiện tồn tại tổng quát cho một hệ tùy ý, cũng như không có một mô tả về tập hợp các nghiệm. Tuy nhiên Hermite, trong các nghiên cứu số học của ông vào thế kỷ XIX

\* Trong khi công trình của Diophantus về các bài toán vô định luôn được quy về các bài toán với một ẩn duy nhất, nhờ chọn số các ẩn còn lại sao cho có thể làm cho nghiệm của phương trình cuối cùng của ông trở nên khả dĩ, thì dường như lý do chủ yếu khiến ông dùng phương pháp này là ký hiệu của ông, vốn không cho phép ông tính với nhiều ẩn cùng một lúc; dù sao đi nữa, ông theo dõi các phép thế số mà ông đã thực hiện trong suốt phép tính, và sau đó nếu cần thì sửa đổi chúng bằng cách viết ra một điều kiện tương thích cho các biến đã thế, rồi giải bài toán phụ này trước. Nói cách khác, ông xử lý các giá trị số đã thế ấy giống như chúng ta xử lý các tham số, đến mức mà điều ông thực sự làm rốt cuộc là tìm một biểu diễn tham số hữu tỉ của một đa tạp đại số cho trước, hoặc của một đa tạp con của nó (cf. (II bis)).

** Tuy nhiên, nhiều dấu hiệu cho thấy Diophantus có kiến thức số học cao hơn: chẳng hạn ông biết rằng phương trình x^2 - y^2 = n không có nghiệm hữu tỉ nếu n là một số nguyên có dạng 4k + 3 (Quyển V, bài toán 9 và Quyển VI, bài toán 14 ((II), vol. 1, pp. 332-335 and p. 425; cf. also (II bis), pp. 105-110)).

*** Các bài toán thiên văn cũng là một trong những bài toán đã dẫn người Hindu đến việc xét loại phương trình này (cf. (III), vol. II, pp. 100, 117 and 135).

thế kỷ, đã bị dẫn tới việc sử dụng một số Bổ đề về các phương trình Diophant tuyến tính, đặc biệt là một « dạng rút gọn » cho một phép biến đổi tuyến tính với các hệ số nguyên ((XIII), pp. 164 and 265); cuối cùng, sau khi Heger vào năm 1858 đã đưa ra điều kiện tồn tại cho một hệ mà hạng của nó bằng số phương trình, H. J. Smith năm 1861 đã định nghĩa các thừa số bất biến của một ma trận nguyên, và thu được định lý tổng quát rằng một ma trận như vậy đưa về « dạng chuẩn » mà chúng tôi đã nêu ở VII, p. 22, Hệ quả 1 (XVII).

Nhưng trong cùng thời kỳ ấy, sau khi được Gauss đưa vào (xem Ghi chú lịch sử cho Chương I, II và III), và do vai trò quan trọng mà nó đã đóng trong sự phát triển tiếp theo của lý thuyết số, khái niệm về một nhóm Abel dần dần được xác định chính xác. Trong công trình nghiên cứu đặc biệt sâu sắc của ông, trình bày trong Disquisitiones, về nhóm Abel hữu hạn các lớp của các dạng toàn phương có cùng biệt thức cho trước, Gauss sớm nhận ra rằng một số nhóm này không tuần hoàn: « trong trường hợp này, » ông nói, « một cơ sở [tức là, một phần tử sinh] không đủ, cần phải lấy hai hoặc nhiều hơn những phần tử nào đó, nhờ phép nhân và hợp thành*, có thể sinh ra tất cả các lớp » ((VIII), vol. I, pp. 374-375). Không chắc rằng Gauss có định dùng những lời này để mô tả sự phân tích của nhóm thành một tích trực tiếp của các nhóm tuần hoàn; tuy nhiên, trong cùng bài viết của Disquisitiones, ông chứng minh rằng tồn tại một phần tử trong nhóm mà cấp của nó là lcm của cấp của tất cả các phần tử khác - nói cách khác, ông thu được sự tồn tại của nhân tử bất biến lớn nhất của nhóm ((VIII), vol. 1, p. 373); và mặt khác, khái niệm tích trực tiếp đã quen thuộc với ông, vì trong một bản thảo có niên đại 1801, nhưng không được công bố khi ông còn sống, ông phác thảo một chứng minh tổng quát về sự phân tích một nhóm Abel hữu hạn thành một tích trực tiếp của các p-nhóm** ((VIII), vol. II, p. 226). Dù sao, năm 1868 Schering, người biên tập các tác phẩm tuyển tập của Gauss, được gợi hứng bởi các kết quả này (đặc biệt bởi bản thảo mà ông vừa tìm thấy), đã chứng minh (vẫn cho nhóm các lớp của các dạng toàn phương) định lý phân tích tổng quát (XVIII) bằng một phương pháp mà, như được Kronecker (XX) nhắc lại bằng thuật ngữ trừu tượng hai năm sau, về thực chất chính là phương pháp mà chúng ta đã dùng ở trên (VII, p. 18, Định lý 1). Còn đối với các nhóm Abel không xoắn, chúng ta đã nói (xem Ghi chú lịch sử cho Chương II và III) về cách lý thuyết các hàm elliptic và các tích phân Abel, được Gauss, Abel và Jacobi phát triển, dần dần dẫn đến việc người ta chú ý đến cấu trúc của chúng; ví dụ đầu tiên và nổi tiếng nhất về một phân tích một nhóm vô hạn thành một tổng trực tiếp của các nhóm tuần hoàn đã được Dirichlet đưa ra năm 1846 trong bài báo của ông về các đơn vị của một trường số đại số (XI). Nhưng phải đến năm 1879 mối liên hệ giữa lý thuyết các nhóm Abel sinh hữu hạn và định lý của Smith mới được Frobenius và Stickelberger nhận ra và sử dụng một cách tường minh ((XXIII), § 10).

\* Gauss dùng ký hiệu cộng cho luật hợp thành của các lớp, vì thế bằng « phép nhân » ông muốn nói tích của một lớp với một số nguyên.
** Abel cũng đã chứng minh tính chất này nhân tiện trong ghi chú của ông về các phương trình Abel ((IX), vol. I, pp. 494-497).

Cũng vào cùng thời kỳ ấy, lý thuyết về tính tương tự của các ma trận (với các phần tử thực hoặc phức) cũng đang đi tới chỗ hoàn chỉnh. Khái niệm trị riêng của một phép biến đổi tuyến tính xuất hiện một cách tường minh trong lý thuyết các hệ phương trình vi phân tuyến tính với hệ số hằng, được Lagrange (VIa) áp dụng cho lý thuyết các dao động nhỏ và được Lagrange (VIb) cùng Laplace (VIIa) áp dụng cho các nhiễu loạn lâu dài của các hành tinh. Nó ẩn tàng trong nhiều bài toán khác cũng được nghiên cứu vào khoảng giữa thế kỷ 18, chẳng hạn bài toán tìm các trục của một đường cônic hoặc một mặt bậc hai (được Euler (Va) giải lần đầu), hoặc việc khảo sát (cũng do Euler (Vb) phát triển) các trục quán tính chính của một vật rắn (được De Segner phát hiện năm 1755); nay ta biết rằng nó cũng hiện diện (ở một dạng ngụy trang hơn) trong những bước đầu của lý thuyết các phương trình vi phân riêng phần, đặc biệt là phương trình của một dây rung. Nhưng (gác trường hợp cuối cùng này sang một bên) mối liên hệ giữa các bài toán khác nhau ấy hầu như chưa được nhận ra trước Cauchy (X). Hơn nữa, vì phần lớn chúng đều liên quan đến việc sử dụng các ma trận đối xứng, nên chính chủ yếu vì các ma trận này mà các trị riêng lúc đầu được nghiên cứu; chúng tôi sẽ trở lại điểm này chi tiết hơn trong các Ghi chú lịch sử theo sau những chương của chuyên luận này dành cho các toán tử Hermit; ở đây chỉ cần lưu ý rằng, ngay từ năm 1826, Cauchy đã chứng minh tính bất biến của các trị riêng của những ma trận như vậy dưới phép tương tự, và chứng minh rằng chúng là thực đối với một ma trận đối xứng $3 \times 3$ (Xa), một kết quả mà ông đã khái quát hóa ba năm sau (Xb) cho các ma trận đối xứng thực tùy ý.* Khái niệm tổng quát về một phép chiếu, do Mobius đưa vào năm 1827, nhanh chóng dẫn đến bài toán phân loại các phép biến đổi như vậy (trước hết trong 2 và 3 chiều), tức là không gì khác hơn bài toán phân loại các ma trận tương ứng theo tương tự; nhưng trong một thời gian dài, bài toán này chỉ được xử lý bằng các phương pháp « tổng hợp » đang thịnh hành vào giữa thế kỷ 19, và sự tiến triển của nó (dù sao cũng khá chậm) dường như không hề ảnh hưởng đến lý thuyết trị riêng. Điều đó không đúng đối với một bài toán hình học khác, việc phân loại các « chùm » các đường cônic hay các mặt bậc hai, mà từ quan điểm hiện đại rút xuống việc nghiên cứu các ước số sơ cấp của ma trận $U + \lambda V$, trong đó $U$ và $V$ là hai ma trận đối xứng; hẳn chính trong tinh thần ấy mà Sylvester đã tấn công bài toán này năm 1851, khi khảo sát cẩn thận (để tìm các « dạng chính tắc » cho chùm đang xét) điều gì xảy ra với các định thức con của ma trận $U + \lambda V$ khi thay vào một giá trị của $\lambda$ làm cho định thức triệt tiêu (XIV). Khía cạnh thuần túy đại số của lý thuyết trị riêng cũng đang tiến triển đồng thời; vì thế mà một số tác giả (kể cả chính Sylvester) đã chứng minh vào khoảng năm 1850 rằng các trị riêng của $U^n$ là các lũy thừa bậc n của các trị riêng của $U$, còn Cayley

\* Một cố gắng chứng minh kết quả này trong trường hợp riêng của các nhiễu loạn « thế kỷ » của các hành tinh trước đó đã được Laplace (VIIb) thực hiện vào năm 1784. Còn đối với phương trình bậc ba cho các trục của một mặt bậc hai thực, Euler đã phát biểu mà không chứng minh rằng nó có các nghiệm thực, và một chứng minh thử của Lagrange năm 1773 (VIe) đã không đầy đủ; điểm này lần đầu tiên được Hachette và Poisson chứng minh một cách chặt chẽ vào năm 1801 (Journal de l'École Polytechnique, tập 11 (năm X), pp. 170-172).

được công bố năm 1858, trong bài báo mà ở đó ông đã đưa vào số học ma trận (XVI), « Định lý Cayley-Hamilton » cho một ma trận vuông tùy ý *, mặc dù ông chỉ bằng lòng với một chứng minh trực tiếp cho các ma trận 2 x 2 và 3 x 3. Cuối cùng Weierstrass vào năm 1868, dùng các phương pháp của Sylvester, đã thu được các « dạng chính tắc » cho một « pencil » $U + XV$ trong đó lần này $U$ và V là các ma trận vuông, không nhất thiết đối xứng, chỉ với điều kiện là $\det(U + XV)$ không đồng nhất bằng không; từ đó ông suy ra định nghĩa các ước số sơ cấp của một ma trận vuông (phức) tùy ý, và chứng minh rằng chúng đặc trưng nó tới đồng dạng (XIX); nhân tiện, những kết quả này đã được Jordan tìm lại một phần (và dường như một cách độc lập) hai năm sau ** (XXI). Lại một lần nữa chính Frobenius đã chỉ ra vào năm 1879 rằng định lý của Weierstrass có thể dễ dàng suy ra từ định lý của Smith mở rộng cho đa thức ((XXII), § 13); phương pháp của ông là cơ sở cho chứng minh của định lý này mà chúng tôi đã trình bày ở trên (VII, p. 35).

Chúng ta vừa nhắc đến lý thuyết chia hết cho đa thức một biến; vấn đề chia đa thức hẳn nhiên phải nảy sinh từ buổi đầu của đại số, như phép toán ngược của phép nhân (phép nhân này thậm chí đã được Diophantus biết đến, ít nhất là đối với các đa thức bậc thấp); nhưng có thể hình dung rằng khó mà tấn công bài toán này theo một cách tổng quát trước khi đã thiết lập được một ký hiệu nhất quán cho các lũy thừa khác nhau của biến. Thực vậy, trước giữa thế kỷ 16 *** ta tìm thấy rất ít ví dụ về phép chia « Euclid » cho đa thức, như ta biết ngày nay; và S. Stevin (về thực chất, dùng ký hiệu số mũ) dường như là người đầu tiên nghĩ đến việc suy ra sự mở rộng của « thuật toán Euclid » để tìm ước chung lớn nhất của hai đa thức ((IV, vol. I, pp. 54-56). Ngoài ra, lý thuyết chia hết đã chỉ được hạn chế trong các số nguyên hữu tỉ cho đến giữa thế kỷ 18. Chính Euler vào năm 1770 đã mở ra một chương mới trong Số học bằng cách khá táo bạo mở rộng khái niệm chia hết sang các số nguyên của một mở rộng bậc hai: nhằm xác định các ước của một số có dạng $x^2 + cy^2$ (x, y và c là các số nguyên), ông đặt

$$
x - y \sqrt{-c} = (p + q \sqrt{-c})(r + s \sqrt{-c}) \quad (p, q, r, s \text{ các số nguyên})
$$

và, lấy chuẩn của mỗi vế, ông không ngần ngại khẳng định rằng mọi ước của $x^2 + cy^2$ đều thu được theo cách này dưới dạng $p^2 + cq^2$ (Vc). Nói cách khác,

\* Hamilton, nhân tiện, đã chứng minh định lý này cho các ma trận 3 x 3 vài năm trước đó ((XV), pp. 566-567).

** Jordan không nhắc đến tính bất biến của dạng chuẩn mà ông thu được. Cũng nên ghi nhận nhân tiện rằng ông đã xét bài toán này không phải cho các ma trận phức, mà cho các ma trận trên một trường hữu hạn. Mặt khác, cần lưu ý rằng Grassmann đã đưa ra một phương pháp đưa một ma trận (phức) về dạng tam giác ngay từ năm 1862, và đã nêu tường minh mối liên hệ giữa phép đưa về này với sự phân loại các phép chiếu (Ges. Math. Werke, vol. I2, Leipzig (Teubner), 1896, pp. 249-254).

*** Xem chẳng hạn H. Bosmans, Sur le « libro del Algebra » de Pedro Nuñez, Bibl. Math. (3), vol. VIII (1907-1908), pp. 154-169.

Euler lập luận như thể vành $\mathbf{Z}[\sqrt{-c}]$ là một miền iđêan chính; không lâu sau ông dùng một lập luận tương tự để áp dụng phương pháp « giáng vô hạn » cho phương trình $x^3 + y^3 = z^3$ (ông quy bài toán về việc tìm một căn bậc ba của $p^2 + 3q^2$, điều mà ông làm bằng cách đặt $p + q \sqrt{-3} = (r + s \sqrt{-3})^3$). Nhưng Lagrange đã chứng minh từ năm 1773 (VIc) rằng các ước của những số có dạng $x^2 + cy^2$ không phải tất cả đều có dạng này, đó là ví dụ đầu tiên của khó khăn cơ bản sẽ xuất hiện rõ ràng hơn nhiều trong các nghiên cứu của Gauss và các môn đồ của ông về tính chia hết trong các trường cyclotomic *; nói chung, không thể mở rộng trực tiếp các tính chất cốt yếu của tính chia hết của các số nguyên hữu tỉ, như sự tồn tại của các ước chung lớn nhất và tính duy nhất của phân tích thành thừa số nguyên tố, sang các trường này. Ở đây không phải chỗ để mô tả Kummer, đối với các trường cyclotomic (XII)**, rồi Dedekind và Kronecker đối với các trường số đại số tùy ý, đã vượt qua trở ngại ghê gớm này như thế nào bằng việc sáng tạo ra lý thuyết iđêan, một trong những tiến bộ quyết định nhất của đại số hiện đại. Nhưng Dedekind, vốn luôn tò mò về nền tảng của các lý thuyết Toán học khác nhau, không bằng lòng với thành công này; và bằng cách phân tích cơ chế của các quan hệ chia hết, ông đã đặt nền móng cho lý thuyết các nhóm có thứ tự dàn, trong một bài báo (không được những người đương thời biết đến, và bị chìm trong quên lãng suốt 30 năm) mà chắc chắn là một trong những công trình sớm nhất của Đại số tiên đề (XXIV); nếu bỏ qua ký hiệu, công trình của ông rất gần với dạng hiện đại của lý thuyết này, như chúng tôi đã trình bày ở Chương VI, 91.

\* Gauss dường như đã từng hy vọng rằng vành các số nguyên trong trường các căn bậc n của đơn vị sẽ là một miền iđêan chính; trong một bản thảo không được công bố khi ông còn sống ((VIII), tập II, tr. 387-397), ông chứng minh sự tồn tại của một quá trình chia Euclid trong trường các căn bậc ba của đơn vị, và đưa ra một vài chỉ dẫn về một quá trình tương tự trong trường các căn bậc năm của đơn vị; ông dùng các kết quả này để chứng minh bằng một lập luận « đi xuống vô hạn » chặt chẽ hơn của Euler rằng phương trình $x^3 + y^3 = z'$ không có nghiệm trong trường các căn bậc ba của đơn vị, chỉ ra rằng có thể mở rộng phương pháp sang phương trình $x^5 + y^5 = z^5$, nhưng dừng lại trước phương trình $x^7 + y^7 = z^7$, nói rằng ở đây không thể bác bỏ tiên nghiệm trường hợp x, y và z không chia hết cho 7.

** Trong công trình sớm nhất của mình về « số iđêan », Kummer đã chỉ ra tường minh khả năng áp dụng phương pháp của mình, không những cho các trường cyclotomic, mà còn cho các trường bậc hai, và do đó khôi phục các kết quả của Gauss về các dạng toàn phương nhị phân ((XII), tr. 324-325).

(Vd): với mọi đa thức $f$ có các hệ số thực, ông đã tìm cách chứng minh sự tồn tại của một phân tích $f = f_1 f_2$ thành hai đa thức (không hằng) có các hệ số *thực*, điều này sẽ cho ông một chứng minh của « định lý cơ bản » bằng quy nạp theo bậc của f. Thậm chí, như ông nhận thấy, chỉ cần dừng lại ở nhân tử có bậc lẻ đầu tiên, và do đó mọi khó khăn được quy về xét trường hợp bậc $n$ của f là chẵn. Euler sau đó tự hạn chế mình vào trường hợp các nhân tử cần tìm đều có bậc $n/2$, và ông chỉ ra rằng bằng một quá trình khử thích hợp có thể biểu diễn các hệ số chưa biết của $f_1$ và $f_2$ dưới dạng các hàm hữu tỉ của một nghiệm của một phương trình với các hệ số thực, mà các hạng đầu và cuối có *dấu trái nhau* và do đó có ít nhất một nghiệm thực. Nhưng chứng minh của Euler chỉ là một phác thảo, và bỏ qua một số điểm cốt yếu; phải đến *1772* Lagrange mới giải quyết được các khó khăn do chứng minh này đặt ra (*VIId*) bằng một phân tích cực kỳ dài và tỉ mỉ, trong đó ông thể hiện một sự điêu luyện đáng chú ý khi sử dụng « các phương pháp Galois » mà ông mới tạo ra gần đây (xem Ghi chú lịch sử về Chương IV và V).

Dẫu vậy, Lagrange, cũng như Euler và tất cả những người cùng thời của ông, không ngần ngại lập luận hình thức trong một « trường nghiệm » của một đa thức (tức là, theo ngôn ngữ của ông, xét các « nghiệm ảo » của đa thức này); Toán học thời đó không hề biện minh cho kiểu lập luận này. Gauss, người ngay từ đầu đã kiên quyết chống lại chủ nghĩa hình thức không bị ràng buộc của thế kỷ 18, đã kịch liệt phản đối sự lạm dụng này trong luận án của ông ((VIII), tập *III*, p. 3). Nhưng hẳn không hợp với ông nếu không nhận ra rằng đây là một cách trình bày bề ngoài có lỗi của một lập luận vốn đúng về bản chất. Vài năm sau đó chúng ta cũng thấy ông ((VIII), tập *III*, p. 33; xem thêm *(VIIIbis)*), tiếp nhận một dạng đơn giản hơn của lập luận của Euler, vốn đã được Foncenex gợi ý vào *1759* (tuy nhiên, ông này không thể khai thác nó vào việc gì), để thu được một chứng minh mới của « định lý cơ bản » trong đó ông cẩn thận tránh mọi nhắc đến các nghiệm « ảo »: những nghiệm này được thay bằng phép nối khéo léo và chuyên biệt hóa các ẩn. Về thực chất, chính là chứng minh này của Gauss mà chúng tôi đã trình bày trong văn bản (VI, p. 26, Định lý 3), với các đơn giản hóa có được nhờ việc sử dụng các mở rộng đại số.

Vai trò của Tôpô trong « định lý cơ bản » vì thế đã được rút xuống thành định lý duy nhất rằng một đa thức với hệ số thực không thể đổi dấu trên một khoảng mà không có một nghiệm (Định lý Bolzano cho đa thức). Định lý này cũng nằm ở gốc của mọi tiêu chuẩn phân tách các nghiệm thực của một đa thức (với các hệ số thực), vốn là một trong những chủ đề đại số được ưa thích nhất trong thế kỷ 19 *. Trong quá trình nghiên cứu này, người ta thấy rõ rằng chính cấu trúc thứ tự của $\mathbf{R}$, chứ không phải tôpô của nó, mới đóng vai trò cốt yếu *; chẳng hạn Định lý Bolzano cho đa thức vẫn đúng trong trường của tất cả các số đại số thực. Chuỗi ý tưởng này đã dẫn tới lý thuyết trừu tượng về các trường có thứ tự, do E. Artin và O. Schreier tạo ra (XXV); một trong những kết quả đáng chú ý nhất của nó hẳn là phát hiện rằng sự tồn tại của một quan hệ thứ tự trên một trường liên quan đến các tính chất thuần túy đại số của trường đó. Đó là lý thuyết được trình bày ở § 2 của Chương VI.

\* Khuynh hướng gán tầm quan trọng quá mức cho cấu trúc thứ tự của các số thực cũng có thể thấy trong định nghĩa của chúng bằng các « lát cắt » của Dedekind, về cơ bản là một quá trình có thể áp dụng cho mọi tập hợp có thứ tự (xem VI, p. 35, Bài tập 30 trở đi).

Thư mục

(I) Euclidis Elementa, 5 vol., ed. J. L. Heiberg, Lipsiae (Teubner), 1883-88.
(I bis) T. L. Heath, The thirteen books of Euclid's Elements..., 3 vol., Cambridge, 1908.
(II) Diophanti Alexandrini Opera Omnia..., 2 vol., ed. P. Tannery, Lipsiae (Teubner), 1893-95.
(II bis) T. L. Heath, Diophantus of Alexandria, 2nd ed., Cambridge, 1910.
(III) B. Datta and A. N. Singh, History of Hindu Mathematics, 2 vol., Lahore (Motilal Banarsí Das), 1935-38.
(IV) S. Stevin, Les œuvres mathématiques..., ed. A. Girard, Leyde (Elsevier), 1634, vol. I.
(V) L. Euler : a) Introductio in Analysin Infinitorum (Opera Omnia, (1), t. IX, Zürich-Leipzig-Berlin (O. Füssli and B. G. Teubner), 1945, p. 384); b) Theoria motus corporum solidorum seu rigidorum (Opera Omnia (2), t. III, Zurich-Leipzig-Berlin (B. G. Teubner), 1948, p. 200-201); c) Vollständige Anleitung zur Algebra (Opera Omnia (1), t. I, Leipzig-Berlin (Teubner), 1911, p. 422); d) Recherches sur les racines imaginaires des équations (Opera Omnia (1), t. VI, Leipzig-Berlin (Teubner), 1921, p. 78).
(VI) J.-L. Lagrange, Œuvres, Paris (Gauthier-Villars), 1867-1892 : a) Solutions de divers problemes de Calcul integral, t. I, p. 520; b) Recherches sur les équations séculaires du mouvement des nœuds, t. VI, p. 655-666; c) Recherches d'arithmétique, t. III, p. 695-795; d) Sur la forme des racines imaginaires des équations, t. III, p. 479; e) Nouvelle solution du probleme de rotation d'un corps quelconque qui n'est animé par aucune force accélératrice, t. III, p. 579-616.
(VII) P. S. Laplace : a) Mémoire sur les solutions particulières des equations différentielles et sur les inegalites seculaires des planetes (Œuvres, t. VIII, Paris (Gauthier-Villars), 1891, p. 325-366); b) Mémoire sur les inégalités seculaires des planetes et des satellites (Œuvres, t. XI, Paris (Gauthier-Villars), 1895, p. 49-92).
(VIII) C. F. Gauss, Werke, t. I (Gottingen, 1870), t. II (ibid., 1876) et t. III (ibid., 1876).
(VIII bis) Die vier Gauss'schen Beweise für die Zerlegung ganzer algebraischer Functionen in reelle Factoren ersten oder zweiten Grades (Ostwald's Klassiker, n° 14, Leipzig (Teubner), 1904).
(IX) N. H. Abel, Œuvres, t. I, ed. Sylow and Lie, Christiania, 1881.
(X) A. L. Cauchy : a) Leçons sur les applications du Calcul infinitésimal a la Géométrie (Œuvres complètes (2), t. V, Paris (Gauthier-Villars), 1903, p. 248); b) Sur l'équation a l'aide de laquelle on determine les inégalités séculaires des planetes (Œuvres complètes (2), t. IX, Paris (Gauthier-Villars), 1891, p. 174).
(XI) P. G. Lejeune-Dirichlet, Werke, t. I, Berlin (G. Reimer), 1889, p. 619-644.
(XII) E. Kummer, Zur Theorie der complexen Zahlen, J. de Crelle, t. XLIII (1847), p. 319 (Collected papers, vol. I, Heidelberg (Springer V.), 1975, p. 203).
(XIII) Ch. Hermite, Œuvres, t. I, Paris (Gauthier-Villars), 1905.
(XIV) J. J. Sylvester, Collected Mathematical Papers, vol. I, Cambridge, 1904 : An enumeration of the contacts of lines and surfaces of the second order, p. 219 (= Phil. Mag., 1851).
(XV) W. R. Hamilton, Lectures on Quaternions, Dublin, 1853.
(XVI) A. Cayley, Collected Mathematical Papers, Cambridge, 1889-1898 : A memoir on the theory of matrices, t. II. p. 475-496 (= Phil. Trans., 1858).

(XVII) H. J. SMITH, Collected Mathematical Papers, vol. I, Oxford, 1894 ; On systems of linear indeterminate equations and congruences, p. 367 (Phil. Trans., 1861).
(XVIII) E. SCHERING, Die fundamental Classen der zusammensetzbaren arithmetischen Formen, Abh. Ges. Göttingen, t. XIV (1868-69), p. 13.
(XIX) K. WEIERSTRASS, Mathematische Werke, Bd. II, Berlin (Mayer und Müller), 1895 : Zur Theorie der bilinearen und quadratischen Formen, p. 19.
(XX) L. KRONECKER, Auseinandersetzungen einiger Eigenschaften der Klassenanzahl idealer complexer Zahlen, Monats. Abhandl. Berlin (1870), p. 881 (= Werke, t. I, Leipzig (Teubner), 1895, p. 273).
(XXI) C. JORDAN, Traité des substitutions et des équations algébriques. Paris (Gauthier-Villars), 1870, p. 114-125.
(XXII) G. FROBENIUS, Theorie der linearen Formen mit ganzen Coefficienten, Gesammelte Abhandlungen, vol. I, Heidelberg (Springer V.), 1968, p. 482 (= J. de Crelle, 1879).
(XXIII) G. FROBENIUS und L. STICKELBERGER, Ueber Gruppen von vertauschbaren Elementen, J. de Crelle, t. LXXXVI (1879), p. 217 (= Frobenius, Ges. Abh., vol. I, p. 545).
(XXIV) R. DEDEKIND, Gesammelte mathematische Werke, t. II, Braunschweig (Vieweg), 1932 : Ueber Zerlegungen von Zahlen durch ihre grössten gemeinsamen Teiler, p. 103.
(XXV) a) E. ARTIN und O. SCHREIER, Algebraische Konstruktion reeler Korper, Abh. Math. Sem. Univ. Hamburg, t. V (1927), p. 83 ; b) E. ARTIN, Ueber die Zerlegung definiter Funktionen in Quadrate (ibid., p. 100) ; c) E. ARTIN und O. SCHREIER, Eine Kennzeichnung der reell abgeschlossenen Korper (ibid., p. 225).

Chỉ mục ký hiệu

A[(X_i)_{i \in I}], A[X_1, ..., X_n], X^\nu : IV, tr. 1. $deg u$ : IV, tr. 3. $f \circ g$ : IV, tr. 4. D_i P, D_{x_i} P, \frac{\partial P}{\partial X_i}, P'_{x_i}, D^\nu, DP, \frac{dP}{dX}, P' : IV, tr. 6. $\Delta^\nu$ : IV, tr. 7. K((X_i)_{i \in I}), deg r : IV, tr. 19 và 20. D_i f, D_{x_i} f, \frac{\partial f}{\partial X_i}, f'_{x_i}, Df, \frac{df}{dX}, f' : IV, tr. 23. $A[[X_i)_{i \in I}]], A[[I]]$ : IV, tr. 24. $\omega$ : IV, tr. 25. u(x), u((x_i)_{i \in I}), u(x_1, ..., x_n) : IV, tr. 29. $A", D", D_i$ : IV, tr. 31 và 32. D_i u, D_{x_i} u, \frac{\partial u}{\partial X_i}, u'_{x_i}, Du, \frac{du}{dX} : IV, tr. 32. $A\{I\}, f \circ g$ : IV, tr. 29 và 36. $T_1$ : IV, tr. 36. exp X, e^X, e(X), l(X) : IV, tr. 39 và 40. $exp f, log g$ : IV, tr. 40. M^H, Tr_{H/G} : IV, tr. 41 và 42. TS^n(M), TS(M) : IV, tr. 42. $\mathfrak{S}_{p|q}, \mathfrak{S}_{p,q}, \mathfrak{S}_{p_1|\cdots|p_n}$ : IV, tr. 43. \gamma_k(x), x \in M : IV, tr. 45. $\varphi_M, \psi_M$ : IV, tr. 52. Pol_A^q(M, N), Pol^q(M, N) : IV, tr. 55. Map(M, N), Pol_A(M, N), Pol(M, N) : IV, tr. 57. s_k, s_{k,n}, A[X_1, ..., X_n]^{\text{sym}} : IV, tr. 61. $S(\alpha), M(\alpha)$ : IV, tr. 65 và 66. s_k, A[[X]]^{\text{sym}} : IV, tr. 67 và 68. $\mathcal{B}_k$ : IV, tr. 70. M(f, g, p, q), res_{p,q}(f, g), res(f, g) : IV, tr. 76. dis(f), đa thức monic f : IV, tr. 81. dis_m(f), đa thức f có bậc \leq m : IV, tr. 83. \Gamma(E), \Gamma_p(E), \gamma_p, \Gamma(h) : IV, tr. 92, bt. 2. $Q, F_p$ : V, tr. 1. S^{pf} : V, tr. 4.

$K[S]$ : V, p. 4.
$S^{p^{-f}}, A^{p^{-\infty}}$: V, p. 5 and 6.
[A : K]: V, p. 10.
K(x_i), K(x), K(x_1, ..., x_n): V, p. 10.
h(L), [A : K], $\mathcal{H}(A)$: V, p. 31.
$E_s$ : V, p. 44.
$[E:K]_s, [E:K],$ : V, p. 31 and 46.
$N_{A/K}(x), \mathrm{Tr}_{A/K}(x), D_{A/K}(x_1, ..., x_n)$ : V, p. 47.
$Gal(N/K)$ : V, p. 58.
$k(\Delta), g(E)$ : V, p. 67.
K_{ab}: V, p. 77.
$\mu_m(K), \mu_\infty(K), \mathbf{Z}[1/p]$: V, p. 78.
$\mu_{l^\infty}(K)$: V, p. 79.
$\varphi(n)$: V, p. 79.
R_n(K), \Phi_n, \chi_n: V, p. 81.
K(A^{1/n}), \langle \sigma, a \rangle: V, p. 88.
$\mathfrak{g}, K(\mathfrak{g}^{-1}(A))$, [u, a]: V, p. 91.
F_q(\Omega), F_q: V, p. 95.
Z_l, Z: V, p. 96.
$\sigma_q$: v, p. 97.
$\varphi_n$: V, p. 97.
deg.tr_K E: V, p. 110.
f^A: V, p. 127.

$\chi(f), f$ là một ánh xạ tuyến tính: V, p. 132.

$x|y, x|y$ : VI, p. 5.
$(x)$ : VI, p. 6.
$x \equiv x' (\bmod y)$ : VI, p. 6.
sup_F(x_i) (F là một tập con của một tập có thứ tự E): VI, p. 8.
gcd(x_i), lcm(x_i): VI, p. 8.
x^+, x^-, |x| (x là một phần tử của một nhóm có thứ tự dàn): VI, p. 12.
sgn(x): VI, p. 20.
$\sqrt{a}$ (a là một phần tử $\geq 0$ của một trường có thứ tự) VI, p. 24.
|z| (z là một phần tử của K(i). trong đó K là một trường có thứ tự và i^2 = -1): VI, p. 27.
GL+(E) (E là một không gian vectơ có hướng): VI, p. 29.
M(\alpha), M_\alpha (M là một môđun trên A, \alpha \in A): VII, p. 7.
(Z/nZ)^*: U(p^n): VII, p. 12.
c_L(x), L là một môđun tự do trên một miền iđêan chính A, x \in L: VII, p. 16.
m(0), m(p^n) (p bất khả quy, n là một số nguyên $\geq 1$): VII, p. 24.
D(M) (M là một môđun trên một miền iđêan chính A, N^0: VII, p. 25 to 27.
$c_M: M \to D(D(M))$ : VII, p. 26.
M_u (M là một môđun, u là một tự đồng cấu của M): VII, p. 28.
V_\alpha (V là một không gian vectơ, \alpha \in K): VII, p. 30.
$\chi_u, \chi_v$: VII, p. 30.
$U_{m,\alpha}$ : VII, p. 35.
u_s, u_j (u là một tự đồng cấu): VII, p. 43 and 45.
f_s, f_u (f là một tự đẳng cấu): VII, p. 46.

Chỉ mục thuật ngữ

Bao đóng Abel : V, p. 77.
Mở rộng Abel : V, p. 77.
Tự đồng cấu nửa đơn tuyệt đối : VII, p. 42.
Phép cộng bất đẳng thức : VI, p. 2.
Phép nối (mở rộng thu được bằng) : V, p. 11.
Bao đóng đại số : V, p. 22.
Phần tử đại số trong một đại số : V, p. 16.
Mở rộng đại số : V, p. 17.
Số đại số : V, p. 20.
Trường đóng đại số : V, p. 20.
Họ, tập con phụ thuộc đại số : V, p. 106.
Các mở rộng đại số rời nhau : V, p. 112.
Họ các mở rộng đại số tự do : V, p. 115.
Họ, tập con đại số tự do : IV, p. 4, V, p. 106.
Nhóm có thứ tự Archimede : VI, p. 35, Ex. 31.
Định lý Artin : V, p. 65.
Định lý Artin-Schreier : VI, p. 22.
Lý thuyết Artin-Schreier : V, p. 91.
Các phần tử liên kết : VI, p. 5.

Đẳng thức Bezout : VII, p. 2.
Quy tắc Budan-Fourier : VI, p. 42, Ex. 21.

Số mũ đặc trưng của một trường : V, p. 7.
Đặc số của một vành : V, p. 2.
Môđun con đặc trưng : VII, p. 67, Ex. 16.
Định lý phần dư Trung Hoa : VI, p. 33, Ex. 25.
Đóng (trường, đại số) : V, p. 20.
Đóng (trường, tách được) : V, p. 45.
Nửa đường thẳng đóng : VI, p. 28.
Trường đóng tương đối đại số : V, p. 19.
Bao đóng Abel của một trường : V, p. 77.
Bao đóng đại số của một trường : V, p. 22.
Bao đóng đại số tách được : V, p. 45.
Bao đóng hoàn hảo : V, p. 5.
Bao đóng đại số tương đối : V, p. 19.

Bao đóng tương đối p-căn : V, p. 25.
Bao đóng đại số tách được tương đối : V, p. 43.
Các hệ số của một chuỗi lũy thừa hình thức : IV, p. 24.
Các hệ số của một đa thức : IV, p. 1.
Tương thích (quan hệ thứ tự) với cấu trúc nhóm, cấu trúc monoid : VI, p. 1.
Tương thích (quan hệ thứ tự) với cấu trúc vành : VI, p. 19.
Tương thích (quan hệ tiền thứ tự) với cấu trúc monoid giao hoán : VI, p. 3.
Hướng bổ sung : VI, p. 29.
Mở rộng hợp : V, p. 12.
Phép hợp thành của các chuỗi : IV, p. 97, Ex. 15.
Lớp liên hợp trong $\Omega$ : V, p. 52.
Các phần tử liên hợp : V, p. 52 ;
Các mở rộng liên hợp : V, p. 52.
Đa thức hằng, số hạng : IV, p. 1.
Nội dung : VII, p. 16.
Các phần tử nguyên tố cùng nhau : VI, p. 13.
Đồng tích trong TS(M) : IV, p. 50.
Mở rộng bậc ba : V, p. 10.
Mở rộng cyclic : V, p. 85.
Không gian vectơ cyclic (đối với u) : VII, p. 29.
Mở rộng cyclotomic : V, p. 81.
Đa thức cyclotomic : V, p. 81.

Môđun phân tích được : VII, p. 23.
Đại số phân tích (phổ quát) của một đa thức : IV, p. 73.
Định lý phân tích: VI, p. 11.
Định lý của Dedekind : V, p. 27.
Bậc (bất khả tách) của một mở rộng : V, p. 46.
Bậc của một đại số trên một trường : V, p. 10.
Bậc của một phần tử đại số : V, p. 16.
Bậc (toàn phần) của một đa thức : IV, p. 3.
Bậc (toàn phần) của một phân thức hữu tỉ : IV, p. 20.
Bậc (tách được) của một mở rộng : V, p. 31.
Đạo hàm riêng trong một mở rộng p-căn có độ cao $\leq 1$ : V, p. 103.
Đạo hàm riêng của một chuỗi lũy thừa hình thức : IV, p. 32.
Đạo hàm riêng của một đa thức : IV, p. 6.
Quy tắc Descartes : VI, p. 42, Ex. 21.
Đường chéo, tập các tự đồng cấu chéo hóa được : VII, p. 40.
Chéo hóa được, đại số chéo hóa : V, p. 28.
Cơ sở trực tiếp : VI, p. 29.
Vectơ chỉ phương : VI, p. 28.
Hướng của một nửa đường thẳng : VI, p. 28.
Biệt thức của một đa thức đơn khởi : IV, p. 81.
Biệt thức của một đa thức : IV, p. 83.
Biệt thức của một dãy các phần tử : V, p. 47.
Các mở rộng rời nhau (theo đại số) : V, p. 112.

Các mở rộng rời tuyến tính : V, p. 14.
Lũy thừa chia trong TS(M) : IV, p. 45.
Lũy thừa chia của một chuỗi : IV, p. 96, Ex. 13.
Quan hệ chia hết : VI, p. 5.
Phép chia (Euclid) : IV, p. 10.
Ước (chung lớn nhất) : IV, p. 12, VI, p. 8.
Ước của một phần tử : VI, p. 5.
Các ước sơ cấp của một môđun : VII, p. 24.
Nghiệm kép : IV, p. 15.

Không gian riêng : VII, p. 30.
Trị riêng : VII, p. 30.
Ước sơ cấp của một môđun : VII, p. 24.
Đa thức đối xứng sơ cấp : IV, p. 61.
Đại số étale : V, p. 28.
Bổ đề Euclid : VI, p. 15.
Miền Euclid : VII, p. 49, Ex. 7.
Đẳng thức Euler : VI, p. 8, IV, p. 89, Ex. 6.
Định lý Euler-Lagrange : VI, p. 26.
Khai triển tại gốc của một phân thức hữu tỉ : IV, p. 30, V, p. 39.
Hàm mũ của một chuỗi lũy thừa hình thức : IV, p. 39.
Kiểu mũ (của dãy) : IV, p. 91, Ex. 1.
Mở rộng của một trường : V, p. 9.
Nguyên lý mở rộng các đồng nhất thức đại số : IV, p. 18.

Mở rộng hữu hạn : V, p. 10.
Mở rộng sinh hữu hạn : V, p. 11.
Dạng bậc n : IV, p. 2.
Chuỗi lũy thừa hình thức : IV, p. 24.
Chuỗi lũy thừa hình thức (tổng quát) : IV, p. 38.
Trường phân thức hữu tỉ : IV, p. 19.
Đồng cấu Frobenius : V, p. 4, V, p. 92.

Mở rộng Galois : V, p. 57.
Nhóm Galois của một mở rộng, của một đa thức : V, p. 58.
Lý thuyết Galois : V, p. 67.
Đại số Gamma của một môđun : IV, p. 92, Ex. 2.
Số nguyên Gaussian : VII, p. 1.
Mở rộng sinh : V, p. 11.
Mở rộng Galois sinh : V, p. 57.
Mở rộng quasi-Galois sinh : V, p. 55.
Họ sinh của một mở rộng : V, p. 11.
Ước chung lớn nhất (UCLN) của các phần tử : VI, p. 8.
Ước chung lớn nhất của các đa thức : IV, p. 12.
Ước chung lớn nhất của các iđêan chính : VII, p. 3.

Nửa đường thẳng (đóng, mở) : VI, p. 28.
Các nửa đường thẳng đối nhau : VI, p. 28.
Các định thức Hankel : IV, p. 90, Ex. 1.
Độ cao của một phần tử p-căn : V, p. 24.
Độ cao của một mở rộng p-căn : V, p. 26.
Độ cao của một phần tử của K(T) : V, p. 148, Ex. 11.
Công thức nội suy Hermite : IV, p. 88, Ex. 13.
Dạng rút gọn Hermite : VII, p. 68, Ex. 21.
Thành phần thuần nhất của một chuỗi lũy thừa hình thức : IV, p. 25.

Trường không hoàn hảo : V, p. 7.
Bậc không hoàn hảo : V, p. 170, Ex. 1.
Môđun bất khả phân : VII, p. 23.
Ẩn : IV, p. 1.
Chỉ số của một ánh xạ tuyến tính : V, p. 132.
Chỉ số Euler : V, p. 79.
Phần tử không phân chia được : VII, p. 17.
Đồng cấu lạm phát : V, p. 70.
Bậc bất khả tách : V, p. 46.
Iđêan nguyên : VI, p. 6.
Các nhân tử bất biến của một ánh xạ tuyến tính : VII, p. 22.
Các nhân tử bất biến của một môđun : VII, p. 20.
Các nhân tử bất biến của một môđun con : VII, p. 19.
Các bất biến (tương tự) của một tự đồng cấu : VII, p. 32.
Phần tử bất khả quy : VI, p. 17.
Đa thức bất khả quy : IV, p. 13.
Đa thức đẳng trọng : IV, p. 3.

Phân tích Jordan : VII, p. 43.
Phân tích Jordan (nhân) : VII, p. 46.
Ma trận Jordan : VII, p. 35.

Mở rộng Kummer : V, p. 162, Ex. 7.
Lý thuyết Kummer : V, p. 88.

Công thức nội suy Lagrange : IV, p. 16.
Luật (đa thức) : IV, p. 94, Ex. 9.
Hệ số dẫn đầu : IV, p. 3.
Bội chung nhỏ nhất (BCNN) của các phần tử : VI, p. 8.
Bội chung nhỏ nhất của các iđêan chính : VII, p. 3.
Nguyên lý Lefschetz : V, p. 117.
Tích từ điển của các nhóm có thứ tự : VI, p. 7.
Tôpô tuyến tính : IV, p. 28.
Các mở rộng rời tuyến tính : V, p. 13.
Đại số có tôpô tuyến tính : IV, p. 28.

Logarit của một chuỗi lũy thừa hình thức : IV, p. 40
Đạo hàm logarit : IV, p. 41.
Định lý Liiroth : V, p. 149, Ex. 11.

Tiêu chuẩn Mac Laner : V, p. 43, V, p. 123.
Trường có thứ tự cực đại : VI, p. 25.
Đa thức tối tiểu của một phần tử : V, p. 16.
Đa thức tối tiểu của một tự đồng cấu : VII, p. 29.
Bổ đề Minkowski : VII, p. 50, Ex. 9.
Đa thức đơn khởi : IV, p. 3.
Mở rộng đơn sinh : V, p. 11.
Các đơn thức, IV, p. 1.
Đa thức không có nhân tử bội : IV, p. 14.
Bội của một phần tử : VI, p. 5.
Nghiệm bội : IV, p. 15.
Bội số (hình học) của một trị riêng : VII, p. 30.
Bội số của một nghiệm : IV, p. 15.
Bội số của một ước sơ cấp : VII, p. 24.

Phần tử âm : VI, p. 4.
n-vectơ âm : VI, p. 29.
Cơ sở âm : VI, p. 29.
Đa giác Newton : V, p. 150, Ex. 2.
Các hệ thức Newton : IV, p. 70, IV, p. 75.
Thành phần lũy linh : VII, p. 45.
Cơ sở chuẩn, định lý cơ sở chuẩn : V, p. 73.
Mở rộng chuẩn : V, p. 53.
Chuẩn : V, p. 47.

Nửa đường thẳng mở : VI. p. 28.
Các nửa đường thẳng đối nhau : VI, p. 28.
Cấp của một chuỗi lũy thừa hình thức (tổng quát) : IV, p. 25, IV, p. 38
Cấp của một nghiệm : IV, p. 15.
Trường có thể sắp thứ tự : VI, p. 39, Ex. 8.
Mở rộng có thứ tự : VI, p. 21.
Trường có thứ tự : VI, p. 20.
Nhóm có thứ tự, monoid có thứ tự : VI, p. 1.
Vành có thứ tự : VI, p. 19.
Định hướng của một không gian vectơ : VI, p. 29.
Không gian afin có định hướng, không gian vectơ có định hướng : VI, p. 29.

vành các số nguyên p-adic : V, p. 96
Cơ sở p : V, p. 98.
Cơ sở p (tuyệt đối) : V, p. 98.
Họ p-tự do : V, p. 98.

Mục lục

Chương IV. — Đa thức và phân thức hữu tỉ ............ IV.1

§ 1. Đa thức ..................................................... IV.1
    1. Định nghĩa của đa thức .................................. IV.1
    2. Bậc ..................................................... IV.2
    3. Phép thế .............................................. IV.4
    4. Vi phân và đạo hàm ............................. IV.6
    5. Ước của không trong một vành đa thức .................... IV.9
    6. Phép chia Euclid của đa thức theo một ẩn .... IV.10
    7. Tính chia hết của đa thức theo một ẩn .......... IV.11
    8. Đa thức bất khả quy ................................... IV.13

§ 2. Nghiệm của đa thức ......................................... IV.14
    1. Nghiệm của một đa thức theo một ẩn. Bội số ..................................................... IV.14
    2. Tiêu chuẩn vi phân cho bội số của một nghiệm ..... IV.17
    3. Hàm đa thức trên một miền nguyên vô hạn ...... IV.17

§ 3. Phân thức hữu tỉ ............................................. IV.19
    1. Định nghĩa của phân thức hữu tỉ ........................... IV.19
    2. Bậc ..................................................... IV.20
    3. Phép thế .............................................. IV.21
    4. Vi phân và đạo hàm ............................. IV.23

§ 4. Chuỗi lũy thừa hình thức .......................................... IV.24
    1. Định nghĩa của chuỗi lũy thừa hình thức. Cấp .................. IV.24
    2. Tôpô trên tập hợp các chuỗi lũy thừa hình thức. Các họ khả cộng ..................................................... IV.25
    3. Phép thế .............................................. IV.28
    4. Các chuỗi lũy thừa hình thức khả nghịch ............................ IV.30
    5. Công thức Taylor cho các chuỗi lũy thừa hình thức .................. IV.31
    6. Các phép vi phân trong đại số các chuỗi lũy thừa hình thức ....... IV.32
    7. Nghiệm của các phương trình trong một vành chuỗi lũy thừa hình thức .. IV.35
    8. Chuỗi lũy thừa hình thức trên một miền nguyên .............. IV.38
    9. Trường phân thức của vành chuỗi lũy thừa hình thức theo một ẩn trên một trường ....................... IV.38
   10. Hàm mũ và lôgarit .................................. IV.39

§ 5. Các tensor đối xứng và các ánh xạ đa thức ......................... IV.41
    1. Vết tương đối .................................................. IV.41
    2. Định nghĩa của các tensor đối xứng ................................. IV.42
    3. Tích cho các tensor đối xứng .................................. IV.43
    4. Lũy thừa chia .................................................. IV.45
    5. Các tensor đối xứng trên một môđun tự do .......................... IV.47
    6. Hàm tử TS .................................................. IV.48
    7. Đồng tích cho các tensor đối xứng ................................. IV.50
    8. Quan hệ giữa TS(M) và S(M) .............................. IV.52
    9. Các ánh xạ đa thức thuần nhất ................................. IV.54
   10. Các ánh xạ đa thức ............................................. IV.57
   11. Quan hệ giữa S(M*), TS(M)*gr và Pol(M, A) ......... IV.59

§ 6. Các hàm đối xứng ............................................. IV.61
    1. Các đa thức đối xứng .......................................... IV.61
    2. Các phân thức hữu tỉ đối xứng ................................. IV.67
    3. Các chuỗi lũy thừa hình thức đối xứng ................................. IV.67
    4. Tổng các lũy thừa ................................................ IV.70
    5. Các hàm đối xứng trong các nghiệm của một đa thức .......... IV.72
    6. Hợp thức .................................................. IV.75
    7. Biệt thức ............................................... IV.81

Bài tập về § 1 .................................................... IV.86
Bài tập về § 2 .................................................... IV.87
Bài tập về § 3 .................................................... IV.89
Bài tập về § 4 .................................................... IV.90
Bài tập về § 5 .................................................... IV.91
Bài tập về § 6 .................................................... IV.98
Bảng ............................................................... IV.103

CHƯƠNG V. — CÁC TRƯỜNG GIAO HOÁN .................................. V.1

§ 1. Các trường nguyên tố. Đặc số .................................. V.1
    1. Các trường nguyên tố .................................................. V.1
    2. Đặc số của một vành và của một trường ..................... V.2
    3. Các vành giao hoán có đặc số p ....................... V.3
    4. Các vành hoàn hảo có đặc số $p$ ....................... V.5
    5. Số mũ đặc số của một trường. Các trường hoàn hảo ........ V.7
    6. Đặc trưng hóa các đa thức có vi phân bằng không .. V.7

§ 2. Các mở rộng .................................................... V.9
    1. Cấu trúc của một mở rộng ............................... V.9
    2. Bậc của một mở rộng ...................................... V.10
    3. Phép nối .................................................. V.10
    4. Các mở rộng hợp thành ......................................... V.12
    5. Các mở rộng rời nhau tuyến tính ............................... V.13

§ 3. Các mở rộng đại số ......................................... V.15
    1. Các phần tử đại số của một đại số ........................... V.15

2. Các mở rộng đại số ..................................................... V.17 3. Tính bắc cầu của các mở rộng đại số. Các trường tương đối đóng đại số trong một trường mở rộng ............ V.19

§ 4. Các mở rộng đóng đại số ............................................. V.19
    1. Các trường đóng đại số ............................................. V.19
    2. Các mở rộng tách .................................................. V.21
    3. Bao đóng đại số của một trường .......................................... V.22

§ 5. Các mở rộng p-căn .......................................................... V.24
    1. Các phần tử p-căn ..................................................... V.24
    2. Các mở rộng p-căn .................................................. V.25

§ 6. Đại số etale ................................................................. V.26
    1. Tính độc lập tuyến tính của các đồng cấu ......................... V.26
    2. Tính độc lập đại số của các đồng cấu .................. V.28
    3. Các đại số chéo hóa được và các đại số etale ............... V.28
    4. Các đại số con của một đại số etale ................................. V.30
    5. Bậc tách được của một đại số giao hoán ................. V.31
    6. Đặc trưng hóa vi phân của các đại số etale ........... V.33
    7. Các đại số rút gọn và các đại số etale .......................... V.34

§ 7. Các mở rộng đại số tách được ............................................. V.36
    1. Các mở rộng đại số tách được .................................. V.36
    2. Các đa thức tách được ............................................... V.37
    3. Các phần tử đại số tách được ...................................... V.39
    4. Định lý về phần tử nguyên thủy ......................... V.40
    5. Các tính chất ổn định của các mở rộng đại số tách được ... V.41
    6. Một tiêu chuẩn tách được ........................................... V.42
    7. Bao đóng đại số tách được tương đối .................... V.43
    8. Bao đóng tách được của một trường ................................. V.45
    9. Bậc tách được và bậc không tách được của một mở rộng bậc hữu hạn ..................................................... V.46

§ 8. Chuẩn và vết ............................................................. V.47
    1. Nhắc lại ............................................................................. V.47
    2. Chuẩn và vết trong các đại số etale ............................. V.47
    3. Chuẩn và vết trong các mở rộng bậc hữu hạn .......... V.50

§ 9. Các phần tử liên hợp và các mở rộng quasi-Galois ......................... V.52
    1. Mở rộng các đẳng cấu ......................................... V.52
    2. Các mở rộng liên hợp. Các phần tử liên hợp .................. V.52
    3. Các mở rộng quasi-Galois ............................................. V.53
    4. Mở rộng quasi-Galois sinh bởi một tập hợp ............. V.55

§ 10. Các mở rộng Galois ............................................................ V.56
    1. Định nghĩa về các mở rộng Galois .................................. V.56
    2. Nhóm Galois ..................................................... V.58
    3. Tôpô của nhóm Galois ...................................... V.60

4. Sự hạ xuống Galois .................................................. V.62 5. Đồng điều Galois ............................................. V.64 6. Định lý Artin ............................................... V.65 7. Định lý cơ bản của lý thuyết Galois ............... V.67 8. Thay đổi trường cơ sở ......................................... V.69 9. Định lý cơ sở chuẩn .................................... VII.72 10. Các tập $\Gamma$ hữu hạn và các đại số etale .................. V.75 11. Cấu trúc của các mở rộng giả-Galois ................. V.76

§ 11. Các mở rộng Abel ........................................ V.77
    1. Các mở rộng Abel và bao đóng Abel ............ V.77
    2. Các căn của đơn vị ........................................... V.78
    3. Các căn nguyên thủy của đơn vị ................................ V.79
    4. Các mở rộng cyclotomic .................................... V.81
    5. Tính bất khả quy của các đa thức cyclotomic ............... V.83
    6. Các mở rộng cyclic ......................................... V.85
    7. Tính đối ngẫu của các môđun $\mathbf{Z}/n\mathbf{Z}$ ............ V.86
    8. Lý thuyết Kummer ........................................... V.88
    9. Lý thuyết Artin-Schreier .................................... V.91

§ 12. Các trường hữu hạn .............................................. V.93
    1. Cấu trúc của các trường hữu hạn .......................... V.93
    2. Các mở rộng đại số của một trường hữu hạn .................. V.94
    3. Nhóm Galois của bao đóng đại số của một trường hữu hạn .................................................. V.96
    4. Các đa thức cyclotomic trên một trường hữu hạn ............. V.97

§ 13. Các mở rộng $p$-căn có độ cao $\leq 1$ .......... V.98
    1. Các tập con $p$-tự do và các $p$-cơ sở ..................... V.98
    2. Các vi phân và các $p$-cơ sở .......................... V.100
    3. Sự tương ứng Galois giữa các trường con và các đại số Lie của các phép đạo hàm ................................. V.104

§ 14. Các mở rộng siêu việt ................................ V.106
    1. Các họ đại số tự do. Các mở rộng thuần ............ V.106
    2. Các cơ sở siêu việt ...................................... V.107
    3. Bậc siêu việt của một mở rộng ............... V.110
    4. Mở rộng các đẳng cấu ................................ V.111
    5. Các mở rộng đại số rời nhau ....................... V.112
    6. Các họ mở rộng đại số tự do ............... V.115
    7. Các mở rộng sinh hữu hạn ........................... V.117

§ 15. Các mở rộng tách được ...................................... V.118
    1. Đặc trưng hóa các phần tử lũy linh của một vành ... V.118
    2. Các đại số tách được ....................................... V.119
    3. Các mở rộng tách được ..................................... V.121
    4. Tiêu chuẩn tách được của Mac Lane ....................... V.122
    5. Các mở rộng của một trường hoàn hảo ........................... V.125
    6. Đặc trưng hóa tính tách được bằng các tự đẳng cấu V.125

§ 16. Các tiêu chuẩn vi phân của tính tách được ............................................. V.127
    1. Mở rộng các phép đạo hàm : trường hợp của các vành .................... V.127
    2. Mở rộng các phép đạo hàm : trường hợp của các trường ................. V.128
    3. Các phép đạo hàm trong các trường đặc số không .................. V.130
    4. Các phép đạo hàm trong các mở rộng tách được ............................. V.131
    5. Chỉ số của một ánh xạ tuyến tính ..................................... V.132
    6. Các tính chất vi phân của các mở rộng sinh hữu hạn . V.133
    7. Các cơ sở siêu việt tách được ................................... V.136

§ 17. Mở rộng chính quy ................................................................. V.137
    1. Bổ sung về bao đóng đại số tách được tương đối ..................................................... V.137
    2. Tích tenxơ của các mở rộng ................................. V.139
    3. Các đại số chính quy ............................................................. V.140
    4. Các mở rộng chính quy .......................................................... V.141
    5. Đặc trưng hóa các mở rộng chính quy ......................... V.142
    6. Ứng dụng trong các mở rộng hợp thành .......................... V.143

Bài tập về § 1 ............................................................................. V.145
Bài tập về § 2 ............................................................................. V.146
Bài tập về § 3 ............................................................................. V.147
Bài tập về § 4 ............................................................................. V.150
Bài tập về § 5 ............................................................................. V.150
Bài tập về § 6 ............................................................................. V.151
Bài tập về § 7 ............................................................................. V.151
Bài tập về § 8 ............................................................................. V.153
Bài tập về § 9 ............................................................................. V.153
Bài tập về § 10 ........................................................................... V.154
Bài tập về § 11 .......................................................................... V.160
Bài tập về § 12 .......................................................................... V.166
Bài tập về § 13 .......................................................................... V.170
Bài tập về § 14 .......................................................................... V.171
Bài tập về § 15 .......................................................................... V.175
Bài tập về § 16 .......................................................................... V.177
Bài tập về § 17 .......................................................................... V.180
Ghi chú lịch sử (các chương IV và V) ............................................. V.182
Thư mục .................................................................................. V.197

CHƯƠNG VI. — NHÓM VÀ TRƯỜNG CÓ THỨ TỰ ............................. VI.1

§ 1. Nhóm có thứ tự. Tính chia hết ..................................................... VI.1
    1. Định nghĩa các monoid có thứ tự và các nhóm ....................... VI.1
    2. Các monoid và các nhóm tiền thứ tự ................................. VI.3
    3. Các phần tử dương ............................................................... VI.3
    4. Các nhóm được lọc ................................................................. VI.4
    5. Các quan hệ chia hết trong một trường ..................................... VI.5
    6. Các phép toán sơ cấp trên các nhóm có thứ tự .................. VI.7
    7. Các đồng cấu tăng của các nhóm có thứ tự ............. VI.7

8. Cực thượng và cực hạ trong một nhóm có thứ tự ......................... VI.8 9. Các nhóm có thứ tự mạng ............................................. VI.10 10. Định lý phân rã ....................................... VI.11 11. Các phần dương và âm ...................................... VI.12 12. Các phần tử nguyên tố cùng nhau .................................................. VI.13 13. Các phần tử bất khả quy ............................................... VI.17

§ 2. Trường có thứ tự ............................................................ VI.19
    1. Vành có thứ tự ....................................................... VI.19
    2. Trường có thứ tự ..................................................... VI.20
    3. Các mở rộng của các trường có thứ tự ..................................... VI.21
    4. Các mở rộng đại số của các trường có thứ tự ........................ VI.23
    5. Các trường có thứ tự cực đại ........................................... VI.25
    6. Đặc trưng hóa các trường có thứ tự cực đại. Định lý Euler-Lagrange ..................................................... VI.26
    7. Không gian vectơ trên một trường có thứ tự ............................. VI.28

Bài tập về § 1 ............................................................. VI.30
Bài tập về § 2 ............................................................. VI.37

CHƯƠNG VII. — CÁC MÔĐUN TRÊN CÁC MIỀN IĐÊAN CHÍNH ........ VII.1

§ 1. Các miền iđêan chính ............................................. VII.1
    1. Định nghĩa một miền iđêan chính ......................... VII.1
    2. Tính chia hết trong các miền iđêan chính ....................... VII.1
    3. Phân tích thành các nhân tử bất khả quy trong các miền iđêan chính ..................................................... VII.3
    4. Tính chia hết của các số nguyên hữu tỉ ................................. VII.5
    5. Tính chia hết của các đa thức theo một ẩn trên một trường ..................................................... VII.5

§ 2. Các môđun xoắn trên một miền iđêan chính ................. VII.6
    1. Các môđun trên một tích của các vành ................................. v11.6
    2. Phân tích chính tắc của một môđun xoắn trên một miền iđêan chính ........................................... VII.7
    3. Ứng dụng : I. Các phân tích chính tắc của các số hữu tỉ và của các hàm hữu tỉ theo một ẩn .... VII.10
    4. Ứng dụng : II. Nhóm nhân của các đơn vị của các số nguyên modulo $a$ ........................................... VII.12

§ 3. Các môđun tự do trên một miền iđêan chính .................... VII.14

§ 4. Các môđun sinh hữu hạn trên một miền iđêan chính ... VII.15
    1. Tổng trực tiếp của các môđun cyclic ................................. VII.15
    2. Nội dung của một phần tử của một môđun tự do ............... VII.16
    3. Các nhân tử bất biến của một môđun con ......................... VII.18
    4. Cấu trúc của các môđun sinh hữu hạn ............................... VII.19
    5. Tính toán các nhân tử bất biến ..................................... VII.20

6. Các ánh xạ tuyến tính của các modun tự do. và các ma trận trên một vành iđêan chính .................................................. VII.21 7. Các nhóm abel hữu hạn sinh .................................................. VII.22 8. Các modun không phân rã được. Các ước tử sơ cấp ............ VII.23 9. Đối ngẫu trong các modun độ dài hữu hạn trên một vành iđêan chính ............................................................. VII.25

§ 5. Các tự đồng cấu của không gian vectơ ........................................ VII.28
    1. Môđun liên kết với một tự đồng cấu ............................... VII.28
    2. Các giá trị riêng và các vectơ riêng ................................. VII.30
    3. Các bất biến đồng dạng của một tự đồng cấu ................. VII.31
    4. Tự đồng cấu tam giác hóa được ..................................... VII.34
    5. Các tính chất của đa thức đặc trưng : vết và định thức .................................................. VII.36
    6. Đa thức đặc trưng của tích tenxơ của hai tự đồng cấu .................................................. VII.39
    7. Các tự đồng cấu chéo hóa được .................................. VII.40
    8. Các tự đồng cấu nửa đơn và tuyệt đối nửa đơn .......................................................... VII.41
    9. Phân tích Jordan ............................................... VII.43

Bài tập ở § 1 ............................................................................. VII.48
Bài tập ở § 2 ............................................................................. VII.54
Bài tập ở § 3 ............................................................................. VII.59
Bài tập ở § 4 ............................................................................. VII.62
Bài tập ở § 5 ............................................................................. VII.70
Ghi chú lịch sử (Chương VI và VII) ........................................... VII.73
Tài liệu tham khảo .................................................................................. VII.83
Bảng ký hiệu ........................................................................ 445
Bảng thuật ngữ .................................................................... 447
Mục lục .......................................................................... 455
