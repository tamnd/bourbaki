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
pdf_pages: 0016-0017
extraction: ocr
statements: 0
exercises: 0
content_sha256: 84dd9a0e7a4b7592038a8c2fafd00cfe452bd8234dcf7502f1975afa693c2156
translated_from: content/en/fvr/00_introduction.md
source_content_sha256: 85e0ba02d9e87d1ef4af523569a61f14e491623624b2c9c740da85ac45ab1be5
translation_model: laguna-s-2.1-free
translation_run: translate-vi-38eb09ab
glossary_version: 34
glossary_terms_sha256: 753e833395f34efd12584076c6bbf6a9ae28615fb8f50ae5dcb86603269bee48
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

#### GIỚI THIỆU

Mục đích của Quyển sách này là nghiên cứu cơ bản các tính chất vi phân của một biến thực; sự mở rộng những tính chất này sang các hàm nhiều biến thực, hay cả các hàm được định nghĩa trên các không gian tổng quát hơn sẽ chỉ được xử lý trong các Quyển sau.

Các kết quả chúng tôi sẽ chứng minh dưới đây sẽ hữu ích nhất là cho các hàm số hữu hạn giá trị thực của một biến thực; nhưng phần lớn chúng cũng mở rộng mà không cần thêm bất kỳ lập luận nào sang các hàm số của một biến thực nhận giá trị trong một không gian vectơ tôpô trên $\mathbf{R}$ (xem dưới đây); vì những hàm số này thường xuyên xuất hiện trong Giải tích, chúng tôi sẽ nêu ra tất cả các kết quả không đặc thù cho các hàm số giá trị thực cho chúng.

Khái niệm một không gian vectơ tôpô, mà chúng tôi vừa nói đến, được định nghĩa và nghiên cứu chi tiết trong Quyển V của Loạt sách này; tuy nhiên chúng tôi không cần bất kỳ kết quả nào của Quyển V trong Quyển này; tuy nhiên một số định nghĩa là cần thiết, và chúng tôi sẽ sao chép chúng dưới đây để thuận tiện cho người đọc.

Chúng tôi sẽ không lặp lại định nghĩa một không gian vectơ trên một trường (giao hoán) K (Alg., II, p. 193). $^1$ Một không gian vectơ tôpô E trên một trường tôpô K là một không gian vectơ trên K được trang bị một topology sao cho các hàm $x + y$ và $xt$ liên tục trên $E \times E$ và $E \times K$ tương ứng; đặc biệt, một topology như vậy là tương thích với cấu trúc của nhóm cộng của E. Tất cả các không gian vectơ tôpô được xem xét trong Quyển này đều được ngầm coi là Hausdorff. Khi nhóm tôpô E là đầy đủ thì ta nói rằng không gian vectơ tôpô E là đầy đủ. Mỗi không gian vectơ chuẩn trên một trường giá trị K (Gen. Top., IX, p. 169) $^2$ là một không gian vectơ tôpô trên K.

Cho E là một không gian vectơ (với hoặc không có topology) trên trường thực $\mathbf{R}$; nếu x, y là các điểm tùy ý trong E thì tập hợp các điểm $xt + y(1-t)$ khi t chạy qua đoạn thẳng kín [0, 1] của $\mathbf{R}$ được gọi là *đoạn thẳng kín* với các đầu mút là $x, y$. Ta nói rằng một tập con A của E là *lồng tròn* nếu với mọi $x, y$ trong A thì đoạn thẳng kín có các đầu mút là $x$ và $y$ được chứa trong A. Ví dụ, một đa dạng affine tuyến tính là lồng tròn; mọt đoạn thẳng kín cũng là lồng tròn; trong $\mathbf{R}^n$ mọi parallelootope (*Gen. Top.*, VI, p. 34) là lồng tròn. Mỗi giao của các tập lồng tròn đều là lồng tròn.

Ta nói rằng một không gian vectơ tôpô E trên trường $\mathbf{R}$ là *địa phương lồng tròn* nếu nguồn gốc (và do đó là mọi điểm của E) có một hệ thống cơ sở các nghiền lân cận *lồng tròn*. Mỗi không gian *chuẩn* đều là địa phương lồng tròn; thực sự, các quả cầu $\|x\| \leq r \ (r > 0)$ tạo thành một hệ thống cơ sở của các nghiền lân cận của 0 trong E, và mỗi quả cầu này đều là lồng tròn, vì các mối quan hệ $\|x\| \leq r,\ \|y\| \leq r$ ngụ ý rằng

$$
\|xt + y(1-t)\| \leq \|x\| t + \|y\| (1-t) \leq r
$$

với $0 \leq t \leq 1$.

Cuối cùng, một *đại số tôpô* A trên một trường (giao hoán) *tôpô* K là một đại số trên K được trang bị một topology sao cho các hàm $x + y,\ xy$ và $xt$ liên tục trên $A \times A$, $A \times A$ và $A \times K$ tương ứng; khi chúng ta chỉ trang bị A với topology và cấu trúc không gian vectơ của nó trên K thì A là một không gian vectơ tôpô. Mỗi *đại số chuẩn* trên một trường giá trị K (*Gen. Top.*, IX, p. 175) là một đại số tôpô trên K.

$^1$ Các phần tử (hay vectơ) của một không gian vectơ E trên một trường giao hoán K thường được ký hiệu trong chương này bằng các chữ in thường đậm, và các vô hướng bằng các chữ in thường La Mã; thường xuyên chúng tôi sẽ đặt vô hướng t thứ nhất trong tích của một vectơ x và t, viết tích dưới dạng $xt$; vào đôi khi chúng tôi sẽ cho phép bản thân sử dụng ký pháp bên trái $tx$ trong một số trường hợp thuận tiện hơn; cũng có lúc chúng tôi sẽ viết tích của vô hướng $1/t$ ($t \neq 0$) và vectơ x dưới dạng $x/t$.

$^2$ Chúng tôi nhắc lại rằng một chuẩn trên E là một hàm thực $\|x\|$ được định nghĩa trên E, nhận giá trị hữu hạn và không âm, sao cho mối quan hệ $\|x\| = 0$ tương đương với $x = 0$ và sao cho

$$
\|x + y\| \leq \|x\| + \|y\| \quad \text{và} \quad \|xt\| = \|x\| \cdot |t|
$$

với mọi $t \in K$ ($|t|$ là giá trị tuyệt đối của $t$ trong K).
