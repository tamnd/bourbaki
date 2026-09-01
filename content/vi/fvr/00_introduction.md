---
book: fvr
book_title: Functions of a Real Variable
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: vi
source: fvr-i-vii
book_pages: 1-2
pdf_pages: 0016-0017
extraction: ocr
statements: 0
exercises: 0
content_sha256: 97144552cb93c1b58b5e08f6d0d35eed442d7f3b0ab77524d5d7cd321b514a1c
translated_from: content/en/fvr/00_introduction.md
source_content_sha256: 85e0ba02d9e87d1ef4af523569a61f14e491623624b2c9c740da85ac45ab1be5
translation_model: gpt-5.4
translation_run: translate-vi-38eb09ab
glossary_version: 34
glossary_terms_sha256: 753e833395f34efd12584076c6bbf6a9ae28615fb8f50ae5dcb86603269bee48
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## GIỚI THIỆU

Mục đích của Quyển này là nghiên cứu sơ cấp các tính chất vô cùng bé của một biến thực; việc mở rộng các tính chất ấy cho các hàm của nhiều biến thực, hoặc hơn nữa, cho các hàm xác định trên những không gian tổng quát hơn, sẽ chỉ được xét trong các Quyển sau.

Các kết quả mà chúng tôi sẽ chứng minh trước hết sẽ hữu ích đối với các hàm (hữu hạn) nhận giá trị thực của một biến thực; nhưng phần lớn chúng mở rộng không cần thêm lập luận nào cho các hàm của một biến thực nhận giá trị trong một không gian vectơ tôpô trên $\mathbf{R}$ (xem dưới đây); vì các hàm ấy xuất hiện thường xuyên trong Giải tích nên chúng tôi sẽ phát biểu đối với chúng mọi kết quả không riêng cho các hàm nhận giá trị thực.

Khái niệm không gian vectơ tôpô mà chúng tôi vừa nói đến được định nghĩa và nghiên cứu chi tiết trong Quyển V của Bộ sách này; nhưng trong Quyển này chúng tôi không cần đến bất kỳ kết quả nào của Quyển V; tuy nhiên, một số định nghĩa là cần thiết, và chúng tôi sẽ chép lại chúng dưới đây để tiện cho người đọc.

Chúng tôi sẽ không nhắc lại định nghĩa của một không gian vectơ trên một trường (giao hoán) K (Alg., II, p. 193). $^1$ Một không gian vectơ tôpô E trên một trường tôpô K là một không gian vectơ trên K được trang bị một tôpô sao cho các hàm $x + y$ và $xt$ liên tục tương ứng trên $E \times E$ và $E \times K$; đặc biệt, một tôpô như vậy tương thích với cấu trúc nhóm cộng của E. Mọi không gian vectơ tôpô được xét trong Quyển này đều được ngầm giả thiết là Hausdorff. Khi nhóm tôpô E là đầy đủ, người ta nói rằng không gian vectơ tôpô E là đầy đủ. Mọi không gian vectơ chuẩn trên một trường định giá K (Gen. Top., IX, p. 169) $^2$ đều là một không gian vectơ tôpô trên K.

Cho E là một không gian vectơ (có hoặc không có một tôpô) trên trường thực $\mathbf{R}$; nếu x, y là những điểm tùy ý của E thì tập hợp các điểm $xt + y(1-t)$ khi t chạy qua đoạn đóng

$^1$ Các phần tử (hay vectơ) của một không gian vectơ E trên một trường giao hoán K nói chung sẽ được ký hiệu trong chương này bằng các chữ thường đậm, còn các vô hướng bằng các chữ thường La Mã; thường nhất chúng tôi sẽ đặt vô hướng t ở bên phải trong tích của một vectơ x với t, viết tích đó là $xt$; đôi khi chúng tôi sẽ cho phép mình dùng ký hiệu bên trái $tx$ trong một số trường hợp thuận tiện hơn; ngoài ra, đôi khi chúng tôi sẽ viết tích của vô hướng $1/t$ ($t \neq 0$) với vectơ x dưới dạng $x/t$.

$^2$ Chúng tôi nhắc lại rằng một chuẩn trên E là một hàm thực $\|x\|$ xác định trên E, nhận các giá trị hữu hạn không âm, sao cho quan hệ $\|x\| = 0$ tương đương với $x = 0$ và sao cho

$$
\|x + y\| \leq \|x\| + \|y\| \quad \text{và} \quad \|xt\| = \|x\| \cdot |t|
$$

với mọi $t \in K$ ($|t|$ là giá trị tuyệt đối của $t$ trong K).

đoạn [0, 1] của $\mathbf{R}$ được gọi là *đoạn đóng* có các đầu mút là $x, y$. Người ta nói rằng một tập con $A$ của $E$ là *lồi* nếu với mọi $x, y$ trong $A$ thì đoạn đóng có các đầu mút $x$ và $y$ được chứa trong $A$. Chẳng hạn, một đa tạp tuyến tính afin là lồi; mọi đoạn đóng cũng vậy; trong $\mathbf{R}^n$ mọi hình bình hành tổng quát (*Gen. Top.*, VI, p. 34) đều lồi. Mọi giao của các tập hợp lồi đều lồi.

Chúng tôi nói rằng một không gian vectơ tôpô $E$ trên trường $\mathbf{R}$ là *lồi địa phương* nếu gốc tọa độ (và do đó mọi điểm của $E$) có một hệ cơ bản các lân cận *lồi*. Mọi không gian *chuẩn* đều lồi địa phương; thật vậy, các quả cầu $\|x\| \leq r \ (r > 0)$ tạo thành một hệ cơ bản các lân cận của 0 trong $E$, và mỗi quả cầu như vậy đều lồi, vì các quan hệ $\|x\| \leq r,\ \|y\| \leq r$ suy ra rằng

$$
\|xt + y(1-t)\| \leq \|x\| t + \|y\| (1-t) \leq r
$$

với $0 \leq t \leq 1$.

Sau hết, một *đại số tôpô* $A$ trên một *trường tôpô* (giao hoán) $K$ là một đại số trên $K$ được trang bị một tôpô sao cho các hàm $x + y,\ xy$ và $xt$ liên tục tương ứng trên $A \times A,\ A \times A$ và $A \times K$; khi người ta chỉ trang bị cho $A$ tôpô và cấu trúc không gian vectơ trên $K$ của nó thì $A$ là một không gian vectơ tôpô. Mọi *đại số chuẩn* trên một *trường định giá* $K$ (*Gen. Top.*, IX, p. 175) đều là một đại số tôpô trên $K$.
