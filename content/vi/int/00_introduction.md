---
book: int
book_title: Integration
chapter: ""
chapter_title: ""
section: 0
section_title: Introduction
kind: introduction
lang: vi
source: int-i-vi
pdf_pages: 0009-0015
extraction: ocr
statements: 0
exercises: 0
content_sha256: 194cc63ebbc06e3e53b862a3749e98119c7755519e60de3fdc58960b687da1a2
translated_from: content/en/int/00_introduction.md
source_content_sha256: b35932fac0c0e6d23a9d819e161f21c556422f54b96079f773b4b400ca4b5789
translation_model: gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-0cd8914b
glossary_version: 34
glossary_terms_sha256: da878c240bfd61747dad98695bed5af70ddc5a959dee2c940abdd043d4f0f68c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## Nhập môn

Khái niệm độ đo của các đại lượng là cơ bản, cả trong đời sống hằng ngày (độ dài, diện tích, thể tích, trọng lượng) cũng như trong khoa học thực nghiệm (điện tích, khối lượng từ, v.v.). Đặc trưng chung của các «độ đo» của những đại lượng đa dạng như vậy nằm ở việc gắn một số với mỗi phần không gian thỏa mãn những điều kiện nhất định, sao cho hợp của hai phần như vậy (giả sử không có điểm chung) tương ứng với tổng của các số được gán cho mỗi phần (tính cộng được của độ đo) (*). Hơn nữa, độ đo thường là một số dương, và điều này kéo theo rằng nó là một hàm tăng của phần không gian được đo (**). Mặt khác, ta nhận thấy rằng trong thực tế, người ta hầu như không bao giờ bận tâm đến việc xác định những phần không gian nào được coi là «đo được»; dĩ nhiên cần phải giải quyết vấn đề này một cách rõ ràng trong mọi lý thuyết toán học về độ đo; ví dụ, đó là điều người ta làm trong hình học sơ cấp khi định nghĩa diện tích của các đa giác hoặc thể tích của các đa diện; trong tất cả các trường hợp này, họ các tập hợp «đo được» dĩ nhiên phải có tính chất là hợp của hai tập hợp bất kỳ trong họ đó không có điểm chung cũng là «đo được».

Trong phần lớn các ví dụ trên, độ đo của một phần không gian tiến tới 0 cùng với đường kính của nó: theo cách hiểu cổ điển, một điểm «không có độ dài», nghĩa là nó được chứa trong các khoảng có độ dài tùy ý nhỏ, do đó ta chỉ có thể gán cho nó độ dài 0; các độ đo của những đại lượng như vậy được gọi là «khuếch tán». Tuy nhiên, sự phát triển của Cơ học và Vật lý đã đưa vào khái niệm các đại lượng mà một vật thể có kích thước không đáng kể vẫn có thể

(*) Không hiển nhiên $a$ priori rằng các loài đại lượng khác nhau có thể được đo bằng cùng những số, và chắc chắn rằng chính bằng cách đào sâu khái niệm độ đo của các đại lượng mà người Hy Lạp đã đạt tới lý thuyết về các tỉ số của các đại lượng, tương đương với lý thuyết về các số thực $> 0$ (cf. GT, Ch. V, §2 và Ghi chú lịch sử của Ch. IV).

(**) Điều này không áp dụng, chẳng hạn, cho điện tích của một vật; tuy nhiên, độ đo của tổng điện tích có thể được xem như hiệu của độ đo các điện tích dương và độ đo các điện tích âm, cả hai đều là các độ đo dương.

có độ đo không đáng kể: các «khối lượng điểm» hấp dẫn hoặc điện, mà nói cho đúng, phần lớn là những hư cấu toán học hơn là những khái niệm thực nghiệm nghiêm ngặt. Vì vậy, trong Toán học, người ta đi đến việc xét các độ đo được định nghĩa như sau: với mỗi điểm $a_i$ ($1 \leq i \leq n$) của một tập hợp hữu hạn F gắn một số $m_i$, «khối lượng» hay «trọng số» của nó, và độ đo của một tập hợp tùy ý A là tổng các khối lượng $m_i$ của những điểm $a_i$ thuộc A.

Gắn bó chặt chẽ với khái niệm độ đo là khái niệm tổng có trọng số. Chẳng hạn, xét trong không gian một số hữu hạn các khối lượng (hấp dẫn hoặc điện) $m_i$ đặt tại các điểm $a_i$ (với các tọa độ $x_i, y_i, z_i$); thành phần theo Oz (chẳng hạn) của lực hút tác dụng lên một điểm b (với khối lượng 1 và các tọa độ $\alpha, \beta, \gamma$) bởi hệ các khối lượng này là (với một hệ đơn vị thích hợp) tổng

$$
\sum_i m_i \frac{(z_i - \gamma)}{r_i^3},
$$

trong đó $r_i^2 = (x_i - \alpha)^2 + (y_i - \beta)^2 + (z_i - \gamma)^2$ là bình phương khoảng cách giữa các điểm $a_i$ và b. Nói cách khác, ta xét giá trị của hàm

$$
f(x, y, z) = \frac{z - \gamma}{\left( (x - \alpha)^2 + (y - \beta)^2 + (z - \gamma)^2 \right)^{3/2}}
$$

tại mỗi điểm $a_i$, nhân nó với «trọng số» của điểm này, và lấy tổng các «giá trị có trọng số» của f thu được như vậy. Người ta biết rằng các tổng như vậy xuất hiện thường xuyên trong Cơ học: các trọng tâm và mômen quán tính là những ví dụ được biết đến nhiều nhất.

Nếu muốn mở rộng khái niệm «tổng có trọng số» từ trường hợp các khối lượng điểm sang trường hợp một độ đo «khuếch tán», trong đó mọi điểm đều có độ đo bằng không, ta gặp phải bài toán, có vẻ ngoài rất nghịch lý, đã làm nảy sinh Phép tính tích phân: làm thế nào gán ý nghĩa cho một «tổng» với vô hạn số hạng mà mỗi số hạng, xét riêng, đều bằng không. Hãy xét lại ví dụ tính lực hút tác dụng lên một điểm, khi các khối lượng hút được «phân bố liên tục» trong toàn bộ một thể tích V. Nếu V được phân chia thành một số hữu hạn các tập con $V_i$ (rời nhau từng đôi một), người ta giả sử rằng thành phần theo Oz của lực hút do V tác dụng lên một điểm b là tổng các thành phần của các lực hút do mỗi $V_i$ tác dụng lên b. Nhưng nếu đường kính của mỗi $V_i$ nhỏ, hàm liên tục $f(x, y, z)$ biến thiên rất ít trong $V_i$, và người ta đi đến việc đồng nhất lực hút do $V_i$ tác dụng với lực hút do một khối lượng điểm bằng khối lượng $m_i$ của $V_i$ và đặt tại một điểm tùy ý $a_i$ của thể tích $V_i$ tác dụng. Vì vậy, người ta đi đến việc lấy, làm giá trị gần đúng của số cần tìm, «tổng Riemann» $\sum_i m_i f(x_i, y_i, z_i)$; để điều này được chứng minh về mặt toán học, dĩ nhiên phải chứng minh rằng các giá trị gần đúng này tiến tới một giới hạn khi đường kính lớn nhất của các $V_i$ tiến tới 0, điều này là hệ quả dễ dàng của tính liên tục đều của hàm $f$ trong $V$ (giả sử $V$ là compact và điểm $b$ không thuộc $V$).

Người ta biết rằng 'phương pháp vét cạn' của người Hy Lạp và 'nguyên lý Cavalieri' để tính một cách hệ thống các diện tích phẳng và thể tích dựa trên một thủ tục tương tự, bằng cách phân tích các diện tích và thể tích được xét thành các 'lát'; các 'tổng có trọng số' thu được như vậy không gì khác hơn là các tích phân $\int_a^b f(x)\, dx$ (xem Ghi chú lịch sử cho các Ch. I–III của Quyển IV). Ở đây cũng vậy, chính tính liên tục đều của $f$ kéo theo sự tồn tại của giới hạn của các 'tổng Riemann'; nói chung hơn, nó kéo theo sự tồn tại của một giới hạn cho các tổng tương tự $\sum_i f(\xi_i)(g(x_{i+1}) - g(x_i))$ ($x_i \leq \xi_i \leq x_{i+1}$), trong đó chỉ giả thiết rằng $g$ là một hàm bị chặn *tăng* trên $[a, b]$. Giới hạn này, được ký hiệu là $\int_a^b f(x)\, dg(x)$ và được gọi là *tích phân Stieltjes* của $f$ đối với $g$, có thể được xem như 'tổng có trọng số' của hàm $f$ đối với độ đo $\mu$ được định nghĩa trên tập hợp các khoảng nửa mở $]\alpha, \beta]$ bởi công thức $\mu([\alpha, \beta]) = g(\beta+) - g(\alpha+)$; nó không còn gắn bó với Phép tính vi phân chặt chẽ như khái niệm tích phân thông thường (*).

Điều tương tự cũng đúng đối với các tích phân 'kép' và 'bội ba' cổ điển, tương ứng liên kết với việc đo các diện tích phẳng và thể tích. Tuy nhiên, tất cả các khái niệm tích phân này liên quan với nhau không chỉ bởi định nghĩa của chúng, mà còn bởi các đặc trưng sau đây: 'tích phân' $\mu(f)$ của một hàm số liên tục $f$ trên một tập con compact $K$ nào đó của đường thẳng, mặt phẳng, hoặc không gian 3 chiều, là một số liên kết với phần tử $f$ của không gian $\mathcal{C}(K)$ gồm các hàm liên tục trên $K$; $f \mapsto \mu(f)$ do đó là một ánh xạ từ $\mathcal{C}(K)$ vào $\mathbf{R}$ (đôi khi được gọi là một 'phiếm hàm') có tính chất: 1° *tuyến tính* (nghĩa là, $\mu(\alpha f + \beta g) = \alpha \mu(f) + \beta \mu(g)$ đối với mọi vô hướng $\alpha, \beta$ và các hàm liên tục $f, g$); 2° *dương* (nghĩa là, $\mu(f) \geq 0$ đối với mọi hàm liên tục $f \geq 0$).

Điều đáng chú ý là, ngược lại, hai tính chất này đủ để đặc trưng các tích phân Stieltjes trên một khoảng $[a, b]$ (định lý F. Riesz). Sở dĩ như vậy là vì, bắt đầu từ các giá trị của tích phân của các hàm liên tục, ta có thể *tái tạo* độ đo đã sinh ra nó. Điều này tương đương (nếu ta nghĩ đến cách giải thích $\int_a^b f(x)\, dx$ như một diện tích phẳng) với việc tính tích phân của một *hàm đặc trưng của một khoảng*, giả sử rằng nó đã được biết đối với các hàm liên tục. Nói cách khác, đây là vấn đề *mở rộng* một cách thích hợp phiếm hàm $\mu(f)$ đến một tập hợp các hàm ch-

(*) Nếu, đặc biệt, ta lấy $g$ là một *hàm bậc thang* tăng và liên tục phải, thì tích phân Stieltjes tương ứng không gì khác hơn là tổng có trọng số của $f$ đối với các khối lượng điểm $m_i = g(a_i+) - g(a_i-)$ đặt tại các điểm gián đoạn $a_i$ của $g$.

ứa $\mathcal{C}(K)$ và đủ lớn để cũng chứa các hàm đặc trưng của các khoảng.

Có nhiều phương pháp để thực hiện sự mở rộng này; một trong những phương pháp thú vị nhất dựa vào khái niệm không gian hàm. Người ta biết rằng, trên không gian $\mathbf{R}^n$, các chuẩn $\|x\|_\infty = \sup_{1 \leq i \leq n} |x_i|$ và $\|x\|_1 = \sum_{i=1}^n |x_i|$ định nghĩa cùng một tôpô. Bằng cách 'chuyển từ hữu hạn sang vô hạn', người ta được dẫn đến việc xét, trên không gian $\mathcal{C}(K)$ gồm các hàm liên tục trên một khoảng compact $K = [a, b]$ của $\mathbf{R}$, các chuẩn $\|f\|_\infty = \sup_{x \in K} |f(x)|$ và $\|f\|_1 = \int_a^b |f(x)| dx$ (hoặc $\int_a^b |f| dg$ trong trường hợp một tích phân Stieltjes). Nhưng ở đây, các tôpô được định nghĩa bởi hai chuẩn này là khác nhau, và không gian $\mathcal{C}(K)$, vốn đầy đủ đối với chuẩn thứ nhất (GT, X, §1, No. 6, Hệ quả 1 của Định lý 2), không còn như vậy đối với chuẩn thứ hai. Chính xác hơn, ta có thể đồng nhất các phần tử của sự hoàn thành của $\mathcal{C}(K)$ đối với chuẩn $\|f\|_1$ với các lớp gồm các hàm không nhất thiết liên tục, và khi đó sự mở rộng của tích phân được thực hiện đơn giản bằng cách mở rộng *bởi tính liên tục* phiếm hàm $\mu(f)$ được định nghĩa trên $\mathcal{C}(K)$ đến sự hoàn thành của không gian này (các chi tiết kỹ thuật của thủ tục này được trình bày trong Ch. IV). Dĩ nhiên, ta đã giả thiết rằng tích phân của các hàm liên tục được định nghĩa bắt đầu từ một độ đo (bằng thủ tục 'các tổng Riemann' được xét lại ở trên); để thu được định lý F. Riesz, cần tiến hành theo cùng cách, nhưng bằng cách định nghĩa chuẩn là $\mu(|f|)$, trong đó $\mu(f)$ là phiếm hàm tuyến tính dương được định nghĩa trên $\mathcal{C}(K)$.

Phương pháp mở rộng mà ta vừa phác thảo không chỉ dẫn đến định lý Riesz, mà ngoài ra còn cho phép định nghĩa tích phân cho các lớp hàm 'gián đoạn hơn nhiều' so với các hàm đặc trưng của các khoảng; khi xét các hàm đặc trưng của các tập hợp là các hàm 'khả tích', nó cho phép đồng thời mở rộng đến các tập hợp tương ứng độ đo ban đầu chỉ được cho trên các khoảng, bằng cách đặt $\mu(A) = \mu(\varphi_A)$; sự mở rộng này dĩ nhiên bảo toàn các tính chất cơ bản của tính cộng và tính dương của độ đo.

Điều trình bày trên đây liên quan đến tích phân Stieltjes trên đường thẳng, nhưng phương pháp mở rộng được chuyển ngay sang các độ đo được định nghĩa trong mặt phẳng hoặc trong không gian, hoặc trên các đường cong hay mặt. Nói chung hơn, khi phân tích các chứng minh, người ta nhận thấy rằng chúng thực sự đúng đối với mọi phiếm hàm tuyến tính dương được định nghĩa trên không gian $\mathcal{K}(X)$ gồm các hàm liên tục trên một *không gian compact địa phương* tùy ý $X$, mỗi hàm trong đó bằng không bên ngoài một tập con compact (phụ thuộc vào hàm cụ thể).

Loại không gian này, mà lý thuyết tích phân do đó áp dụng được cho, tự nhiên bao gồm các không gian số $\mathbf{R}^n$ cũng như các đa tạp; nó cũng bao gồm các không gian rời rạc (nơi lý thuyết tích phân hòa nhập với lý thuyết về các họ số thực khả tổng (GT, IV, §7)), cũng như các tích (hữu hạn hoặc vô hạn) của các không gian compact đồng nhất với một khoảng của $\mathbf{R}$ hoặc với một tập hữu hạn; về sau ta sẽ thấy rằng lý thuyết độ đo trên các tích như vậy đóng một vai trò quan trọng trong Phép tính Xác suất.

Sự mở rộng khái niệm độ đo sang các không gian compact địa phương tổng quát đã tỏ ra đặc biệt phong phú trong lý thuyết về các *nhóm compact địa phương*; nói chung, khái niệm tích phân dường như là công cụ thích hợp khi, trong Đại số Tôpô, người ta muốn "chuyển từ hữu hạn sang vô hạn", nghĩa là tổng quát hóa các thủ tục của đại số thuần túy trong đó xuất hiện các tổng *hữu hạn*, sang trường hợp phép "tổng" phải xử lý một số vô hạn các số hạng. Chẳng hạn, ta biết (A, III, §2) rằng các phần tử của *đại số của một nhóm hữu hạn* $G$ (trên trường $\mathbf{R}$) là các ánh xạ $s \mapsto \alpha(s)$ của $G$ vào $\mathbf{R}$, với luật nhân $\alpha * \beta = \gamma$, trong đó $\gamma$ là hàm được xác định bởi

$$
\gamma(s) = \sum_{t \in G} \alpha(t) \beta(t^{-1} s) .
$$

Điều có vẻ là một phép tổng quát hóa tự nhiên của đại số này, đối với một nhóm compact địa phương tùy ý $G$, là tập hợp các ánh xạ của $G$ vào $\mathbf{R}$ khả tích đối với một độ đo đặc biệt nào đó $\mu$ trên $G$ (độ đo Haar), phép nhân trong đại số được cho bởi

$$
(f * g)(s) = \int f(t) g(t^{-1} s) \, d\mu(t) .
$$

Hơn nữa, một khi đã đi theo con đường này, người ta nhanh chóng cảm thấy khó chịu bởi nghĩa vụ chỉ "tổng" các hàm có giá trị thực; trong nhiều trường hợp, điều hữu ích là biết cách định nghĩa tích phân của các hàm được xác định trên $X$ và nhận các giá trị trong một *không gian vectơ tôpô* trên $\mathbf{R}$, chẳng hạn một không gian Banach hoặc một không gian các toán tử trên một không gian Banach. Người ta nhận thấy rằng sự mở rộng này có thể thực hiện dễ dàng mà không cần bất kỳ sự sửa đổi sâu sắc nào của lý thuyết tích phân.

Trong phác thảo trên đây, vai trò chủ yếu đã được dành cho các hàm *liên tục*; thật tự nhiên khi hỏi liệu khái niệm độ đo trên thực tế có gắn một cách cốt yếu với sự tồn tại của một tôpô trên tập $X$ nơi nó được xác định hay không. Việc xem xét kỹ lý thuyết cho thấy rằng hoàn toàn không phải như vậy, và rằng các phương pháp mở rộng cũng áp dụng cho một phiếm hàm tuyến tính dương $\mu(f)$ được xác định trên một không gian vectơ $\mathcal{V}$ gồm các hàm số được xác định trên một tập *tùy ý* $X$, bằng cách dùng một số điều kiện bổ sung đặt ra trên $\mathcal{V}$ và trên $\mu(f)$; các điều kiện này được *tự động* thỏa mãn khi $\mathcal{V}$ là một không gian $\mathcal{K}(X)$ của các hàm liên tục có giá compact, nhưng chúng cũng được thỏa mãn trong các trường hợp tổng quát hơn. Tuy nhiên, tính tổng quát lớn hơn này trên một số phương diện chỉ là ảo tưởng: thật vậy, có thể chứng minh rằng mọi "độ đo trừu tượng" theo một nghĩa nào đó là "đẳng cấu" với một độ đo được xác định (bắt đầu từ các hàm liên tục) trên một không gian compact địa phương thích hợp; mặt khác, phần lớn các ứng dụng liên quan đến các tập X được trang bị một tôpô can thiệp một cách tự nhiên vào vấn đề; do đó, cho đến Chương IX, ta sẽ chỉ nghiên cứu các độ đo được xác định trên các *không gian compact địa phương*.

Hai chương đầu là những phần chuẩn bị cho lý thuyết: chúng dành cho việc chứng minh các bất đẳng thức cơ bản đối với sự mở rộng, và cho việc nghiên cứu một số không gian vectơ có thứ tự, các *không gian Riesz*, đóng một vai trò quan trọng trong một số vấn đề về sau.

Khái niệm độ đo trên một không gian compact địa phương được định nghĩa trong Chương III; ta lấy làm điểm xuất phát định lý Riesz, định lý này do đó trở thành một định nghĩa: tích phân của các hàm liên tục vì vậy được định nghĩa *trước* độ đo của các tập hợp, như một phiếm hàm tuyến tính dương trên $\mathcal{K}(X)$. Cách trình bày này có những ưu điểm kỹ thuật nhất định (đặc biệt do thực tế rằng các hàm liên tục tạo thành một không gian vectơ, trong khi điều này không đúng đối với các hàm đặc trưng của các tập hợp); hơn nữa, chính dưới dạng một phiếm hàm trên $\mathcal{K}(X)$ mà tích phân xuất hiện một cách tự nhiên trong nhiều vấn đề. Cuối cùng, hiệu của hai phiếm hàm tuyến tính dương trên $\mathcal{K}(X)$ (mà ta lại gọi là các *độ đo* trên X) có thể được đặc trưng như các dạng tuyến tính trên $\mathcal{K}(X)$ thỏa mãn một số điều kiện *liên tục*; do đó lý thuyết tích phân có liên quan, một mặt với lý thuyết tổng quát về đối ngẫu trong các không gian vectơ tôpô (xem Quyển V) và mặt khác với lý thuyết về *phân phối*, lý thuyết này tổng quát hóa một số khía cạnh của khái niệm độ đo và sẽ được trình bày trong một Quyển sau.

Chương IV dành cho sự *mở rộng* của tích phân; ở đó các hàm khả tích và độ đo của các tập hợp đều được định nghĩa, cũng như các không gian hàm $L^p$, mà tầm quan trọng của chúng trong các ứng dụng là đáng kể; ở đó cũng chỉ ra cách việc đưa vào khái niệm *hàm đo được* dẫn đến các tiêu chuẩn thuận tiện về tính khả tích.

Trong hai chương tiếp theo, ta sẽ thấy các hàm đo được cũng xuất hiện như những "mật độ", cho phép định nghĩa các độ đo mới trên một không gian X bắt đầu từ một độ đo đã cho. Nghiên cứu này, dẫn đến đặc biệt các kết quả quan trọng trong lý thuyết đối ngẫu của các không gian $L^p$, cũng gắn với khái niệm *độ đo vectơ*, khái niệm này, trong những trường hợp thuận lợi nhất, có thể đưa về lý thuyết tích phân (đối với một độ đo dương) của các hàm có giá trị vectơ.

Chúng ta cũng sẽ phát triển điều có thể được xem là sự hoàn thiện hiện đại của ý tưởng về “phân tích thành các lát” của các miền phẳng và các thể tích, được đưa vào bởi những người sáng lập Phép tính tích phân: dưới những điều kiện nhất định, một độ đo trên một không gian X có thể được phân tích thành một “tổng” các độ đo mà mỗi độ đo trong đó được mang bởi một “lát” của không gian X (nghĩa là, bởi một lớp tương đương đối với một quan hệ R nào đó); hơn nữa, một phân tích như vậy cho phép tính tích phân của một hàm, đối với độ đo ban đầu, bằng cách trước hết lấy tích phân “trên mỗi lát”, rồi lấy tích phân (đối với một độ đo thích hợp) của hàm thu được trên không gian thương X/R (một phép tổng quát hóa của “phép cộng kép” đối với tổng của một họ trong đó các chỉ số chạy trên một tập hợp tích).

Chương VII dành cho việc nghiên cứu độ đo Haar trên một nhóm compact địa phương, được đặc trưng, sai khác một bội vô hướng, bởi tính chất bất biến dưới mọi phép tịnh tiến trái của nhóm.

Trong Chương VIII phép xoắn của các độ đo được trình bày, một khái niệm giữ một vai trò cấp một trong Giải tích phiếm hàm hiện đại.

Chương IX dành cho phép lấy tích phân trong các không gian tôpô Hausdorff không nhất thiết compact địa phương, và đặc biệt trong các không gian vectơ lồi địa phương; điều này cho phép, đáng chú ý, mở rộng lý thuyết về phép biến đổi Fourier đến các không gian sau. Cách trình bày được chọn trong các mục đầu tiên bao gồm việc, trong chừng mực có thể, quy về trường hợp các không gian compact được xét trong các chương trước.
