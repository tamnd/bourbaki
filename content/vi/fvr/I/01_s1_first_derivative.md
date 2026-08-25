---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 1
section_title: FIRST DERIVATIVE
lang: vi
source: fvr-i-vii
pdf_pages: 0018-0027, 0050-0052
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVE OF A VECTOR FUNCTION
      page: 0
      pdf_page: 18
    - "no": 2
      title: LINEARITY OF DIFFERENTIATION
      page: 0
      pdf_page: 20
    - "no": 3
      title: DERIVATIVE OF A PRODUCT
      page: 0
      pdf_page: 21
    - "no": 4
      title: DERIVATIVE OF THE INVERSE OF A FUNCTION
      page: 0
      pdf_page: 23
    - "no": 5
      title: DERIVATIVE OF A COMPOSITE FUNCTION
      page: 0
      pdf_page: 24
    - "no": 6
      title: DERIVATIVE OF AN INVERSE FUNCTION
      page: 0
      pdf_page: 24
    - "no": 7
      title: DERIVATIVES OF REAL-VALUED FUNCTIONS
      page: 0
      pdf_page: 25
statements: 31
exercises: 9
content_sha256: de796670952022610f2d517314d4917d4072c4a291a4ea4b7d6b463bba78561d
translated_from: content/en/fvr/I/01_s1_first_derivative.md
source_content_sha256: a411ec6338883a3109c8cef83bc1bd84e50d906c78f0da4e98858ad55ca77a45
translation_model: gpt-5.4
translation_run: translate-vi-9093b294
glossary_version: 34
glossary_terms_sha256: 451e1b9e0e1801513f3d6865e2ec5f21e85184235eef81666fff3ce5c1745a90
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. ĐẠO HÀM THỨ NHẤT

Như đã nói trong Lời mở đầu, trong chương này và chương tiếp theo chúng ta sẽ nghiên cứu các tính chất vô cùng bé của những hàm được xác định trên một tập con của trường thực $\mathbf{R}$ và nhận giá trị trong một *không gian vectơ tôpô Hausdorff* E trên trường $\mathbf{R}$; để vắn tắt, ta sẽ nói rằng một hàm như thế là một *hàm vectơ của một biến thực*. Trường hợp quan trọng nhất là trường hợp $E = \mathbf{R}$ (các hàm thực của một biến thực). Khi $E = \mathbf{R}^n$, việc xét một hàm vectơ nhận giá trị trong E quy về việc xét đồng thời $n$ hàm thực hữu hạn.

Nhiều định nghĩa và tính chất được phát biểu trong chương I mở rộng được cho các hàm được xác định trên một tập con của trường $\mathbf{C}$ các số phức và nhận giá trị trong một không gian vectơ tôpô trên $\mathbf{C}$ (các hàm vectơ của một biến phức). Một số trong các định nghĩa và tính chất này còn mở rộng được cả cho các hàm được xác định trên một tập con của một *trường tôpô* giao hoán tùy ý K và nhận giá trị trong một không gian vectơ tôpô trên K.

Chúng tôi sẽ chỉ ra các sự khái quát hóa ấy trong khi trình bày (xem đặc biệt I, p. 10, *Nhận xét 2*), nhấn mạnh trước hết trường hợp các hàm của một biến phức, vốn quan trọng hơn hẳn, cùng với các hàm của một biến thực, và sẽ được nghiên cứu sâu hơn trong một Quyển sau.

### 1. ĐẠO HÀM CỦA MỘT HÀM VECTƠ

#### Định nghĩa 1 {#fvr-i-s1-def-1 .statement}

*Cho $f$ là một hàm vectơ xác định trên một khoảng $I \subset \mathbf{R}$ không rút gọn thành một điểm duy nhất. Ta nói rằng $f$ khả vi tại một điểm $x_0 \in I$ nếu*
$$
\lim_{x \to x_0, x \in I, x \neq x_0} \frac{f(x) - f(x_0)}{x - x_0}
$$
*tồn tại (trong không gian vectơ nơi $f$ nhận các giá trị của nó); giá trị của giới hạn này được gọi là đạo hàm bậc nhất (hoặc đơn giản là đạo hàm) của $f$ tại điểm $x_0$, và được ký hiệu bởi $f'(x_0)$ hoặc $Df(x_0)$.*

Nếu $f$ khả vi tại điểm $x_0$, thì *hạn chế* của $f$ trên mọi khoảng $J \subset I$ không rút gọn thành một điểm duy nhất và sao cho $x_0 \in J$ cũng khả vi; và đạo hàm của hạn chế này bằng $f'(x_0)$. Ngược lại, cho $J$ là một khoảng được chứa trong $I$ và chứa một lân cận của $x_0$ tương đối với $I$; nếu hạn chế của $f$ trên $J$ có đạo hàm tại điểm $x_0$, thì $f$ cũng vậy.

Ta tóm tắt các tính chất này bằng cách nói rằng khái niệm đạo hàm là một khái niệm địa phương.

#### Nhận xét 1 {#fvr-i-s1-n1-rem-1 .statement}

Trong Động học, nếu điểm $\mathbf{f}(t)$ là vị trí của một điểm chuyển động trong không gian $\mathbf{R}^3$ tại thời điểm $t$, thì $\frac{\mathbf{f}(t) - \mathbf{f}(t_0)}{t - t_0}$ được gọi là vận tốc trung bình giữa các thời điểm $t_0$ và $t$, và giới hạn của nó $\mathbf{f}'(t_0)$ là vận tốc tức thời (hay đơn giản là vận tốc) tại thời điểm $t_0$ (khi giới hạn này tồn tại).*
2) Nếu một hàm $\mathbf{f}$, xác định trên $I$, khả vi tại một điểm $x_0 \in I$, thì nó nhất thiết liên tục đối với $I$ tại điểm này.

#### Định nghĩa 2 {#fvr-i-s1-def-2 .statement}

*Cho $\mathbf{f}$ là một hàm vectơ xác định trên một khoảng $I \subset \mathbf{R}$, và cho $x_0$ là một điểm của $I$ sao cho khoảng $I \cap [x_0, +\infty[$ (tương ứng, $I \cap ]-\infty, x_0]$) không rút gọn thành một điểm duy nhất. Ta nói rằng $\mathbf{f}$ khả vi bên phải (tương ứng, bên trái) tại điểm $x_0$ nếu hạn chế của $\mathbf{f}$ trên khoảng $I \cap [x_0, +\infty[$ (tương ứng, $I \cap ]-\infty, x_0]$) khả vi tại điểm $x_0$; giá trị của đạo hàm của hạn chế này tại điểm $x_0$ được gọi là đạo hàm phải (tương ứng, trái) của $\mathbf{f}$ tại điểm $x_0$ và được ký hiệu bởi $\mathbf{f}'_d(x_0)$ (tương ứng, $\mathbf{f}'_g(x_0)$).*

Cho $\mathbf{f}$ là một hàm vectơ xác định trên $I$, và $x_0$ là một điểm trong của $I$ sao cho $\mathbf{f}$ liên tục tại điểm này; suy ra từ định nghĩa 1 và 2 rằng để $\mathbf{f}$ khả vi tại $x_0$ thì điều kiện cần và đủ là $\mathbf{f}$ có cả đạo hàm phải và đạo hàm trái tại điểm này, và các đạo hàm ấy bằng nhau; và khi đó

$$
\mathbf{f}'(x_0) = \mathbf{f}'_d(x_0) = \mathbf{f}'_g(x_0).
$$

#### Ví dụ 1 {#fvr-i-s1-n1-exa-1 .statement}

Một hàm hằng có đạo hàm không tại mọi điểm.
2) Một hàm tuyến tính afin $x \mapsto ax + b$ có đạo hàm bằng $a$ tại mọi điểm.
3) Hàm thực $1/x$ (được xác định với $x \neq 0$) khả vi tại mỗi điểm $x_0 \neq 0$, vì ta có $\left( \frac{1}{x} - \frac{1}{x_0} \right) / (x - x_0) = -\frac{1}{x x_0}$, và, do $1/x$ liên tục tại $x_0$, giới hạn của biểu thức đứng trước là $-1/x_0^2$.
4) Hàm vô hướng $|x|$, được xác định trên $\mathbf{R}$, có đạo hàm phải $+1$ và đạo hàm trái $-1$ tại $x = 0$; nó không khả vi tại điểm này.
*5) Hàm thực bằng 0 với $x = 0$, và bằng $x \sin 1/x$ với $x \neq 0$, được xác định và liên tục trên $\mathbf{R}$, nhưng không có cả đạo hàm phải lẫn đạo hàm trái tại điểm $x \neq 0$.* Có thể cho những ví dụ về các hàm liên tục trên một khoảng và không có đạo hàm tại mọi điểm của khoảng ấy (I, p. 35, exerc. 2 and 3).

#### Định nghĩa 3 {#fvr-i-s1-def-3 .statement}

*Ta nói rằng một hàm vectơ $\mathbf{f}$ xác định trên một khoảng $I \subset \mathbf{R}$ là khả vi (tương ứng, khả vi phải, khả vi trái) trên $I$ nếu nó khả vi (tương ứng, khả vi phải, khả vi trái) tại mỗi điểm của $I$; hàm $x \mapsto \mathbf{f}'(x)$ (tương ứng, $x \mapsto \mathbf{f}'_d(x)$, $x \mapsto \mathbf{f}'_g(x)$) xác định trên $I$ được gọi là hàm dẫn xuất, hoặc (do lạm dụng ngôn ngữ) là đạo hàm (tương ứng, đạo hàm phải, đạo hàm trái) của $\mathbf{f}$, và được ký hiệu bởi $\mathbf{f}'$ hoặc $\mathrm{Df}$ hoặc $d\mathbf{f}/dx$ (tương ứng, $\mathbf{f}'_d, \mathbf{f}'_g$).*

#### Nhận xét {#fvr-i-s1-n1-rem-2 .statement}

Một hàm có thể khả vi trên một khoảng mà đạo hàm của nó không liên tục tại mọi điểm của khoảng ấy (*xem.* I, p. 36, exerc. 5); *điều này được chỉ ra bởi ví dụ về hàm bằng 0 khi $x = 0$ và bằng $x^2 \sin 1/x$ khi $x \neq 0$; nó có đạo hàm tại mọi nơi, nhưng đạo hàm này gián đoạn tại điểm $x = 0$.

### 2. TÍNH TUYẾN TÍNH CỦA PHÉP VI PHÂN

#### Mệnh đề 1 {#fvr-i-s1-prop-1 .statement}

*Tập hợp các hàm vectơ xác định trên một khoảng $I \subset \mathbf{R}$, nhận giá trị trong một không gian vectơ tôpô $E$ đã cho, và khả vi tại điểm $x_0$, là một không gian vectơ trên $\mathbf{R}$, và ánh xạ $f \mapsto Df(x_0)$ là một ánh xạ tuyến tính từ không gian này vào $E$.*

Nói cách khác, nếu $f$ và $g$ được xác định trên $I$ và khả vi tại điểm $x_0$, thì $f + g$ và $fa$ ($a$ là một vô hướng tùy ý) khả vi tại $x_0$ và các đạo hàm của chúng tại đó lần lượt là $f'(x_0) + g'(x_0)$ và $f'(x_0)a$. Điều này suy ra ngay lập tức từ tính liên tục của $x + y$ và của $xa$ lần lượt trên $E \times E$ và $E$.

#### Hệ quả {#fvr-i-s1-n2-cor-1 .statement}

*Tập hợp các hàm vectơ xác định trên một khoảng $I$, nhận giá trị trong một không gian vectơ tôpô $E$ đã cho, và khả vi trên $I$, là một không gian vectơ trên $\mathbf{R}$, và ánh xạ $f \mapsto Df$ là một ánh xạ tuyến tính từ không gian này vào không gian vectơ các ánh xạ từ $I$ vào $E$.*

#### Nhận xét {#fvr-i-s1-n2-rem-1 .statement}

Nếu trang bị cho không gian vectơ các ánh xạ từ $I$ vào $E$ và không gian con của nó gồm các ánh xạ khả vi (*x. Gen. Top.*, X, p. 277) tôpô hội tụ đơn (hoặc tôpô hội tụ đều), thì ánh xạ tuyến tính $f \mapsto Df$ *không liên tục* (nói chung); *chẳng hạn, dãy các hàm* $f_n(x) = \sin n^2 x / n$ *hội tụ đều tới* 0 *trên* $\mathbf{R}$, *nhưng dãy các đạo hàm* $f'_n(x) = n \cos n^2 x$ *thậm chí không hội tụ đơn tới* 0.

#### Mệnh đề 2 {#fvr-i-s1-prop-2 .statement}

*Cho $E$ và $F$ là hai không gian vectơ tôpô trên $\mathbf{R}$, và $u$ là một ánh xạ tuyến tính liên tục từ $E$ vào $F$. Nếu $f$ là một hàm vectơ xác định trên một khoảng $I \subset \mathbf{R}$, nhận giá trị trong $E$, và khả vi tại điểm $x_0 \in I$, thì hàm hợp $u \circ f$ có đạo hàm bằng $u(f'(x_0))$ tại $x_0$.*

Thật vậy, vì $\frac{u(f(x)) - u(f(x_0))}{x - x_0} = u \left( \frac{f(x) - f(x_0)}{x - x_0} \right)$, điều này suy ra từ tính liên tục của $u$.

#### Hệ quả {#fvr-i-s1-n2-cor-2 .statement}

*Nếu $\varphi$ là một dạng tuyến tính liên tục trên $E$, thì hàm thực $\varphi \circ f$ có đạo hàm bằng $\varphi(f'(x_0))$ tại điểm $x_0$.*

#### Ví dụ 1 {#fvr-i-s1-n2-exa-1 .statement}

Cho $f = (f_i)_{1 \leq i \leq n}$ là một hàm nhận giá trị trong $\mathbf{R}^n$, xác định trên một khoảng $I \subset \mathbf{R}$; mỗi hàm thực $f_i$ không gì khác hơn là hàm hợp $\mathrm{pr}_i \circ f$, nên khả vi tại điểm $x_0$ nếu $f$ khả vi tại đó, và khi đó $f'(x_0) = (f'_i(x_0))_{1 \leq i \leq n}$.

#### Ví dụ 2 {#fvr-i-s1-n2-exa-2 .statement}

Trong Động học, nếu $f(t)$ là vị trí của một điểm chuyển động $M$ tại thời điểm $t$, nếu $g(t)$ là vị trí ở cùng thời điểm của hình chiếu $M'$ của $M$ lên một mặt phẳng $P$ (tương ứng, một đường thẳng $D$) với hạt nhân là một đường thẳng (tương ứng, một mặt phẳng) không song song với $P$ (tương ứng, $D$), thì $g$ là hợp thành của phép chiếu $u$ của $\mathbf{R}^3$ lên $P$ (tương ứng, $D$) và của $f$; vì $u$ là một ánh xạ tuyến tính (liên tục), nên ta thấy rằng hình chiếu của vận tốc của một điểm chuyển động lên một mặt phẳng (tương ứng, một đường thẳng) bằng vận tốc của hình chiếu của điểm chuyển động lên mặt phẳng (tương ứng, đường thẳng).*

#### Ví dụ 3 {#fvr-i-s1-n2-exa-3 .statement}

Cho $f$ là một hàm nhận giá trị phức xác định trên một khoảng $I \subset \mathbf{R}$, và cho $a$ là một số phức tùy ý; mệnh đề 2 cho thấy rằng nếu $f$ khả vi tại một điểm $x_0$ thì $af$ cũng vậy, và đạo hàm của hàm này tại $x_0$ bằng $af'(x_0)$.

### 3. ĐẠO HÀM CỦA MỘT TÍCH

Bây giờ ta xét $p$ không gian vectơ tôpô $E_i$ ($1 \leq i \leq p$) trên $\mathbf{R}$, và một ánh xạ đa tuyến tính liên tục $^1$ (mà ta sẽ ký hiệu bởi

$$
(x_1, x_2, \ldots, x_p) \mapsto [x_1.x_2 \ldots x_p])
$$

của $E_1 \times E_2 \times \cdots \times E_p$ vào một không gian vectơ tôpô F trên $\mathbf{R}$.

MỆNH ĐỀ 3 . *Với mỗi chỉ số $i$ ($1 \leq i \leq p$), cho $f_i$ là một hàm xác định trên một khoảng $I \subset \mathbf{R}$, nhận giá trị trong $E_i$, và khả vi tại điểm $x_0 \in I$. Khi đó hàm

$$
x \mapsto [f_1(x).f_2(x) \ldots f_p(x)]
$$

xác định trên $I$ với giá trị trong $F$ có đạo hàm bằng

$$
\sum_{i=1}^p [f_1(x_0) \ldots f_{i-1}(x_0).f'_i(x_0).f_{i+1}(x_0) \ldots f_p(x_0)]
$$

tại $x_0$.

Đặt $h(x) = [f_1(x).f_2(x) \ldots f_p(x)]$; khi đó, nhờ đồng nhất thức

$$
[b_1.b_2 \ldots b_p] - [a_1.a_2 \ldots a_p] = \sum_{i=1}^p [b_1 \ldots b_{i-1}.(b_i - a_i).a_{i+1} \ldots a_p],
$$

ta có thể viết

$$
h(x) - h(x_0) = \sum_{i=1}^p [f_1(x) \ldots f_{i-1}(x).(f_i(x) - f_i(x_0)).f_{i+1}(x_0) \ldots f_p(x_0)].
$$

Nhân cả hai vế với $\frac{1}{x - x_0}$ rồi cho $x$ tiến tới $x_0$ trong $I$, ta thu được biểu thức (1), vì cả ánh xạ

$$
(x_1, x_2, \ldots, x_p) \mapsto [x_1.x_2 \ldots x_p]
$$

lẫn phép cộng trong F đều liên tục.

$^1$ Nhắc lại (Alg., II, p. 265) rằng một ánh xạ $f$ từ $E_1 \times E_2 \times \cdots \times E_p$ vào F được gọi là *đa tuyến tính* nếu mỗi ánh xạ riêng phần

$$
x_i \mapsto f(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_p)
$$

từ $E_i$ vào F ($1 \leq i \leq p$) là một ánh xạ *tuyến tính*, các $a_j$ với chỉ số $j \neq i$ là tùy ý trong $E_j$. Ta chú ý rằng nếu các $E_i$ là hữu hạn chiều trên $\mathbf{R}$ thì mọi ánh xạ đa tuyến tính từ $E_1 \times E_2 \times \cdots \times E_p$ vào F tất yếu là *liên tục*; điều này không nhất thiết còn đúng nếu một vài trong các không gian ấy là các không gian vectơ tôpô chiều vô hạn.

Khi một vài trong các hàm $f_i$ là hằng, thì các số hạng trong biểu thức (1) chứa các đạo hàm của chúng $f'_i(x_0)$ đều bằng không.

Xét chi tiết trường hợp riêng $p = 2$, trường hợp quan trọng nhất trong các ứng dụng: nếu $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}.\mathbf{y}]$ là một ánh xạ song tuyến tính liên tục từ $E \times F$ vào $G$, (E, F, G là các không gian vectơ tôpô trên $\mathbf{R}$), và $\mathbf{f}$ và $\mathbf{g}$ là hai hàm vectơ, khả vi tại $x_0$, nhận giá trị lần lượt trong E và F, thì hàm vectơ $x \mapsto [\mathbf{f}(x).\mathbf{g}(x)]$ (mà ta ký hiệu là $[\mathbf{f}.\mathbf{g}]$) có đạo hàm bằng $[\mathbf{f}'(x_0).\mathbf{g}(x_0)] + [\mathbf{f}(x_0).\mathbf{g}'(x_0)]$ tại $x_0$. Đặc biệt, nếu $\mathbf{a}$ là một vectơ hằng, thì $[\mathbf{a}.\mathbf{f}]$ (resp. $[\mathbf{f}.\mathbf{a}]$) có đạo hàm bằng $[\mathbf{a}.\mathbf{f}'(x_0)]$ (resp. $[\mathbf{f}'(x_0).\mathbf{a}]$) tại $x_0$.

Nếu $\mathbf{f}$ và $\mathbf{g}$ đều khả vi trên I thì $[\mathbf{f}.\mathbf{g}]$ cũng vậy, và ta có

$$
[\mathbf{f}.\mathbf{g}]' = [\mathbf{f}'.\mathbf{g}] + [\mathbf{f}.\mathbf{g}'].
$$

(2)

#### Ví dụ 1 {#fvr-i-s1-n3-exa-1 .statement}

Cho $f$ là một hàm thực, $\mathbf{g}$ là một hàm vectơ, cả hai đều khả vi tại một điểm $x_0$; hàm $\mathbf{g}f$ có đạo hàm bằng $\mathbf{g}'(x_0)f(x_0) + \mathbf{g}(x_0)f'(x_0)$ tại $x_0$. Đặc biệt, nếu $\mathbf{a}$ là hằng, thì $\mathbf{a}f$ có đạo hàm $\mathbf{a}f'(x_0)$. Nhận xét cuối cùng này, phối hợp với ví dụ 1 của I, p. 5, chứng minh rằng nếu $\mathbf{f} = (f_i)_{1 \leq i \leq n}$ là một hàm vectơ nhận giá trị trong $\mathbf{R}^n$, thì điều kiện cần và đủ để $\mathbf{f}$ khả vi tại điểm $x_0$ là mỗi hàm thực $f_i$ ($1 \leq i \leq n$) đều khả vi tại đó: thật vậy, nếu $(\mathbf{e}_i)_{1 \leq i \leq n}$ là cơ sở chính tắc của $\mathbf{R}^n$, thì ta có thể viết $\mathbf{f} = \sum_{i=1}^n \mathbf{e}_i f_i$.

#### Ví dụ 2 {#fvr-i-s1-n3-exa-2 .statement}

Hàm thực $x^n$ phát sinh từ hàm đa tuyến tính

$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n
$$

được xác định trên $\mathbf{R}^n$, bằng cách thay $x$ vào mỗi $x_i$; vậy mệnh đề 3 cho thấy rằng $x^n$ khả vi trên $\mathbf{R}$ và có đạo hàm là $nx^{n-1}$. Do đó hàm đa thức $\mathbf{a}_0 x^n + \mathbf{a}_1 x^{n-1} + \cdots + \mathbf{a}_{n-1} x + \mathbf{a}_n$ (trong đó các $\mathbf{a}_i$ là các vectơ hằng) có đạo hàm là

$$
n \mathbf{a}_0 x^{n-1} + (n-1) \mathbf{a}_1 x^{n-2} + \cdots + \mathbf{a}_{n-1};
$$

khi các $\mathbf{a}_i$ là các số thực thì hàm này trùng với đạo hàm của một hàm đa thức như được định nghĩa trong Đại số (A, IV).

#### Ví dụ 3 {#fvr-i-s1-n3-exa-3 .statement}

Tích vô hướng Euclid $(\mathbf{x}| \mathbf{y})$ (Gen. Top , VI, p. 40) là một ánh xạ song tuyến tính (tất yếu liên tục) từ $\mathbf{R}^n \times \mathbf{R}^n$ vào $\mathbf{R}$. Nếu $\mathbf{f}$ và $\mathbf{g}$ là hai hàm vectơ nhận giá trị trong $\mathbf{R}^n$, và khả vi tại điểm $x_0$, thì hàm thực $x \mapsto (\mathbf{f}(x)|\mathbf{g}(x))$ có đạo hàm bằng $(\mathbf{f}'(x_0)|\mathbf{g}(x_0)) + (\mathbf{f}(x_0)|\mathbf{g}'(x_0))$ tại điểm $x_0$. Có một kết quả tương tự đối với tích vô hướng Hermit trên $\mathbf{C}^n$, khi không gian này được xét như một không gian vectơ trên $\mathbf{R}$.

Hãy xét riêng trường hợp chuẩn Euclid $\| \mathbf{f}(x) \|$ là hằng, do đó $(\mathbf{f}(x)|\mathbf{f}(x)) = \| \mathbf{f}(x) \|^2$ cũng là hằng; khi viết rằng đạo hàm của $(\mathbf{f}(x)|\mathbf{f}(x))$ triệt tiêu tại $x_0$ ta được $(\mathbf{f}(x_0)|\mathbf{f}'(x_0)) = 0$; nói cách khác, $\mathbf{f}'(x_0)$ trực giao với $\mathbf{f}(x_0)$.

#### Ví dụ 4 {#fvr-i-s1-n3-exa-4 .statement}

Nếu $E$ là một đại số tôpô trên $\mathbf{R}$ (xem Introduction), thì tích $xy$ của hai phần tử của $E$ là một hàm song tuyến tính liên tục của $(x, y)$; nếu $\mathbf{f}$ và $\mathbf{g}$ nhận giá trị trong $E$ và khả vi tại điểm $x_0$, thì hàm $x \mapsto \mathbf{f}(x)\mathbf{g}(x)$ có đạo hàm bằng $\mathbf{f}'(x_0)\mathbf{g}(x_0) + \mathbf{f}(x_0)\mathbf{g}'(x_0)$ tại $x_0$. Đặc biệt, nếu $U(x) = (\alpha_{ij}(x))$ và $V(x) = (\beta_{ij}(x))$ là hai ma trận vuông cấp $n$, khả vi tại $x_0$, thì tích của chúng $UV$ có đạo hàm bằng $U'(x_0)V(x_0) + U(x_0)V'(x_0)$ tại $x_0$ (trong đó $U'(x) = (\alpha'_{ij}(x))$ và $V'(x) = (\beta'_{ij}(x))$).

#### Ví dụ 5 {#fvr-i-s1-n3-exa-5 .statement}

Định thức $\det(\mathbf{x}_1, \mathbf{x}_2, \ldots, \mathbf{x}_n)$ của $n$ vectơ $\mathbf{x}_i = (x_{ij})_{1 \leq i \leq n}$ của không gian $\mathbf{R}^n$ (Alg., III, p. 522) là một hàm đa tuyến tính (liên tục) theo các $\mathbf{x}_i$, nên ta thấy rằng nếu $n^2$ hàm thực $f_{ij}$ khả vi tại $x_0$, thì định thức của chúng $g(x) = \det(f_{ij}(x))$ có đạo hàm bằng
$$
\sum_{i=1}^n \left[ \mathbf{f}_1(x_0), \ldots, \mathbf{f}_{i-1}(x_0), \mathbf{f}_i'(x_0), \mathbf{f}_{i+1}(x_0), \ldots, \mathbf{f}_n(x_0) \right]
$$
tại $x_0$, trong đó $\mathbf{f}_i(x) = (f_{ij}(x))_{1 \leq j \leq n}$; nói cách khác, ta thu được đạo hàm của một định thức cấp $n$ bằng cách lấy tổng của $n$ định thức được tạo thành bằng cách thay thế, với mỗi $i$, các phần tử của cột thứ $i^{th}$ bởi các đạo hàm của chúng.

#### Nhận xét {#fvr-i-s1-n3-rem-1 .statement}

Nếu $U(x)$ là một ma trận bình phương khả vi và khả nghịch tại điểm $x_0$, thì đạo hàm của định thức của nó $\Delta(x) = \det(U(x))$ có thể được biểu diễn theo đạo hàm của $U(x)$ bởi công thức
$$
\Delta'(x_0) = \Delta(x_0) \cdot \operatorname{Tr}(U'(x_0) U^{-1}(x_0)).
$$
Thật vậy, đặt $U(x_0 + h) = U(x_0) + h V$; khi đó, theo định nghĩa, $V$ tiến tới $U'(x_0)$ khi $h$ tiến tới 0. Ta có thể viết
$$
\Delta(x_0 + h) = \Delta(x_0) \cdot \det(I + h V U^{-1}(x_0)).
$$
Bây giờ $\det(I + h X) = 1 + h \operatorname{Tr}(X) + \sum_{k=2}^n \lambda_k h^k$, trong đó các $\lambda_k$ ($k \geq 2$) là các đa thức theo các phần tử của ma trận $X$; vì các phần tử của $V U^{-1}(x_0)$ có giới hạn khi $h$ tiến tới 0, nên quả thật ta thu được công thức (3).

### 4. ĐẠO HÀM CỦA NGHỊCH ĐẢO CỦA MỘT HÀM

#### Mệnh đề 4 {#fvr-i-s1-prop-4 .statement}

*Cho E là một đại số chuẩn đầy đủ với một phần tử đơn vị trên $\mathbf{R}$ và cho $\mathbf{f}$ là một hàm xác định trên một khoảng $I \subset \mathbf{R}$, nhận giá trị trong E, và khả vi tại điểm $x_0 \in I$. Nếu $y_0 = \mathbf{f}(x_0)$ khả nghịch $^2$ trong E, thì hàm $x \mapsto (\mathbf{f}(x))^{-1}$ được xác định trên một lân cận của $x_0$ (đối với I), và có đạo hàm bằng $-(\mathbf{f}(x_0))^{-1} \mathbf{f}'(x_0) (\mathbf{f}(x_0))^{-1}$ tại $x_0$.*

Thật vậy, tập hợp các phần tử khả nghịch trong E là một tập hợp mở mà trên đó hàm $y \mapsto y^{-1}$ là liên tục (*Gen. Top.*, IX, p. 178); vì $\mathbf{f}$ liên tục (tương đối với I) tại $x_0$, nên $(\mathbf{f}(x))^{-1}$ được xác định trên một lân cận của $x_0$, và ta có
$$
(\mathbf{f}(x))^{-1} - (\mathbf{f}(x_0))^{-1} = (\mathbf{f}(x))^{-1} \left( \mathbf{f}(x_0) - \mathbf{f}(x) \right) (\mathbf{f}(x_0))^{-1}.
$$
Do đó mệnh đề suy ra từ tính liên tục của $y^{-1}$ trên một lân cận của $y_0$ và tính liên tục của $xy$ trên $E \times E$.

$^2$ Nhắc lại từ (*Alg.*, I, p. 15) rằng một phần tử $z \in E$ được gọi là *khả nghịch* nếu tồn tại một phần tử của $E$, ký hiệu là $z^{-1}$, sao cho $zz^{-1} = z^{-1}z = e$ (ở đây e là phần tử đơn vị của $E$).

#### Ví dụ 1 {#fvr-i-s1-n4-exa-1 .statement}

Trường hợp riêng quan trọng nhất là trường hợp E là một trong các trường $\mathbf{R}$ hoặc $\mathbf{C}$: nếu $f$ là một hàm nhận giá trị thực hoặc phức, khả vi tại điểm $x_0$, và sao cho $f(x_0) \neq 0$, thì $1/f$ có đạo hàm bằng $-f'(x_0)/(f(x_0))^2$ tại $x_0$.

#### Ví dụ 2 {#fvr-i-s1-n4-exa-2 .statement}

Nếu $U = (\alpha_{ij}(x))$ là một ma trận bình phương cấp $n$, khả vi tại $x_0$ và khả nghịch tại điểm này, thì $U^{-1}$ có đạo hàm bằng $-U^{-1} U' U^{-1}$ tại $x_0$.

### 5. ĐẠO HÀM CỦA MỘT HÀM HỢP

#### Mệnh đề 5 {#fvr-i-s1-prop-5 .statement}

*Cho $f$ là một hàm thực xác định trên một khoảng $I \subset \mathbf{R}$, và $g$ là một hàm vectơ xác định trên một khoảng của $\mathbf{R}$ chứa $f(I)$. Nếu $f$ khả vi tại điểm $x_0$ và $g$ khả vi tại điểm $f(x_0)$ thì hàm hợp $g \circ f$ có đạo hàm bằng $g'(f(x_0)) f'(x_0)$ tại $x_0$.*

Đặt $h = g \circ f$; với $x \neq x_0$ ta có thể viết
$$
\frac{h(x) - h(x_0)}{x - x_0} = u(x) \frac{f(x) - f(x_0)}{x - x_0}
$$
trong đó ta đặt $u(x) = \frac{g(f(x)) - g(f(x_0))}{f(x) - f(x_0)}$ nếu $f(x) \neq f(x_0)$, và $u(x) = g'(f(x_0))$ trong trường hợp ngược lại. Bây giờ $f(x)$ có giới hạn $f(x_0)$ khi $x$ tiến tới $x_0$, nên $u(x)$ có giới hạn $g'(f(x_0))$, từ đó suy ra mệnh đề do tính liên tục của hàm $yx$ trên $E \times \mathbf{R}$.

### 6. ĐẠO HÀM CỦA MỘT HÀM NGHỊCH ĐẢO

#### Mệnh đề 6 {#fvr-i-s1-prop-6 .statement}

*Cho $f$ là một đồng phôi của một khoảng $I \subset \mathbf{R}$ lên một khoảng $J = f(I) \subset \mathbf{R}$, và cho $g$ là đồng phôi nghịch đảo$^3$. Nếu $f$ khả vi tại điểm $x_0 \in I$, và nếu $f'(x_0) \neq 0$, thì $g$ có đạo hàm bằng $1/f'(x_0)$ tại $y_0 = f(x_0)$.*

Với mỗi $y \in J$ ta có $g(y) \in I$ và $u = f(g(y))$; do đó ta có thể viết
$$
\frac{g(y) - g(y_0)}{y - y_0} = \frac{g(y) - x_0}{f(g(y)) - f(x_0)}
$$
với $y \neq y_0$. Khi $y$ tiến tới $y_0$ trong khi vẫn thuộc $J$ và $\neq y_0$, thì $g(y)$ tiến tới $x_0$ trong khi vẫn thuộc $I$ và $\neq x_0$, và vì thế vế phải của công thức trên có giới hạn là $1/f'(x_0)$, vì theo giả thiết $f'(x_0) \neq 0$.

#### Hệ quả {#fvr-i-s1-n6-cor-1 .statement}

*Nếu $f$ khả vi trên $I$ và nếu $f'(x) \neq 0$ trên $I$, thì $g$ khả vi trên $J$ và đạo hàm của nó tại mỗi điểm $y \in J$ là $1/f'(g(y))$.*

Ví dụ, với mỗi số nguyên $n > 0$, hàm $x^{1/n}$ là một đồng phôi của $\mathbf{R}_+$ lên chính nó, là hàm nghịch đảo của $x^n$, và có đạo hàm $\frac{1}{n} x^{\frac{1}{n} - 1}$ tại mỗi $x > 0$.

Từ mệnh đề 5, người ta dễ dàng suy ra rằng với mọi số hữu tỉ $r = p/q > 0$ thì hàm $x^r = (x^{1/q})^p$ có đạo hàm $rx'^{-1}$ tại mọi $x > 0$.

$^3$ Để $f$ là một đồng phôi từ $I$ lên một tập con của $\mathbf{R}$ thì điều kiện cần và đủ là $f$ liên tục và đơn điệu nghiêm ngặt trên $I$ (*Gen. Top.*, IV, p. 338, định lý 5).

#### Nhận xét 1 {#fvr-i-s1-n6-rem-1 .statement}

Tất cả các mệnh đề trước đây, được phát biểu cho các hàm khả vi tại một điểm $x_0$, ngay lập tức cho các mệnh đề đối với các hàm khả vi phải (tương ứng, trái) tại $x_0$, khi, thay vì xét chính các hàm ấy, người ta xét các hạn chế của chúng trên giao của các khoảng định nghĩa của chúng với khoảng $[x_0, +\infty[$ (tương ứng, ]$-\infty, x_0$]); chúng tôi để độc giả tự phát biểu chúng.

#### Nhận xét 2 {#fvr-i-s1-n6-rem-2 .statement}

Các định nghĩa và mệnh đề đi trước (trừ những điều liên quan đến các đạo hàm phải và trái) được mở rộng dễ dàng sang trường hợp khi người ta thay thế $\mathbf{R}$ bởi một *trường tôpô giao hoán không rời rạc* tùy ý $K$, và các không gian vectơ tôpô (tương ứng, các đại số tôpô) trên $\mathbf{R}$ bởi các không gian vectơ tôpô (tương ứng, các đại số tôpô) trên $K$. Trong đn. 1 và các mệnh đề 1, 2 và 3, chỉ cần thay thế I bởi một *lân cận* của $x_0$ trong $K$; trong mệnh đề 4, còn phải giả thiết thêm rằng ánh xạ $y \mapsto y'$ được xác định và liên tục trên một lân cận của $f(x_0)$ trong E. Mệnh đề 5 được tổng quát hóa theo cách sau: cho $K'$ là một trường con không rời rạc của trường tôpô $K$, cho E là một không gian vectơ tôpô *trên* $K$; cho $f$ là một hàm được xác định trên một lân cận $V \subset K'$ của $x_0 \in K'$, nhận giá trị trong $K$ (được xét như một không gian vectơ tôpô trên $K'$), khả vi tại $x_0$, và cho g là một hàm được xác định trên một lân cận của $f(x_0) \in K$, nhận giá trị trong E, và khả vi tại điểm $f(x_0)$; khi đó ánh xạ $g \circ f$ khả vi tại $x_0$ và có đạo hàm $g'(f(x_0))f'(x_0)$ tại đó (khi ấy E được xét như một không gian vectơ tôpô *trên* $K'$).

Với cùng ký hiệu, cho $f$ là một hàm được xác định trên một lân cận V của $a \in K$, nhận giá trị trong E, và khả vi tại điểm $a$; nếu $a \in K'$ thì *hạn chế* của $f$ lên $V \cap K'$ khả vi tại $a$, và có đạo hàm $f'(a)$ tại đó. Trong thực hành, những nhận xét này áp dụng trước hết cho trường hợp $K = \mathbf{C}$ và $K' = \mathbf{R}$.

Sau cùng, mệnh đề 6 cũng mở rộng cho trường hợp thay I bằng một lân cận của $x_0 \in K$, và $f$ bằng một đồng phôi từ I lên một lân cận $J = f(I)$ của $y_0 = f(x_0)$ trong $K$.

### 7. ĐẠO HÀM CỦA CÁC HÀM THỰC

Các định nghĩa và mệnh đề trước đây còn có thể được bổ sung trên nhiều phương diện khi ta xét các hàm *thực* của một biến thực.

Trước hết, nếu $f$ là một hàm như vậy, xác định trên một khoảng $I \subset \mathbf{R}$, và liên tục tương đối đối với I tại một điểm $x_0 \in I$, thì có thể xảy ra rằng khi $x$ tiến tới $x_0$ mà vẫn nằm trong I và $\neq x_0$, thì $\frac{f(x) - f(x_0)}{x - x_0}$ có một giới hạn bằng $+\infty$ hoặc bằng $-\infty$; khi đó người ta nói rằng $f$ khả vi tại $x_0$ và có đạo hàm bằng $+\infty$ (tương ứng $-\infty$) tại đó; nếu hàm $f$ có một đạo hàm $f'(x)$ (hữu hạn hoặc vô hạn) tại mọi điểm $x$ của I, thì hàm $f'$ (nhận giá trị trong $\overline{\mathbf{R}}$) lại được gọi là hàm dẫn xuất (hoặc đơn giản là đạo hàm) của $f$. Người ta cũng tổng quát hóa tương tự các định nghĩa về đạo hàm phải và đạo hàm trái.

#### Ví dụ {#fvr-i-s1-n7-exa-1 .statement}

Tại điểm $x = 0$ hàm $x^{1/3}$ (hàm nghịch đảo của $x^3$, một đồng phôi của $\mathbf{R}$ lên chính nó) có đạo hàm, bằng $+\infty$; tại $x = 0$ hàm $|x|^{1/3}$ có đạo hàm phải $+\infty$ và đạo hàm trái $-\infty$.

Các công thức tính đạo hàm của một tổng, của một tích các hàm thực khả vi, và của hàm nghịch đảo của một hàm khả vi (mệnh đề 1, 3 và 4), cũng như công thức tính đạo hàm của một hợp thành (nhận giá trị thực) của các hàm (mệnh đề 5) vẫn còn đúng khi các đạo hàm xuất hiện là vô hạn, miễn là mọi biểu thức xuất hiện trong các công thức ấy đều có nghĩa (*Gen Top.*, IV, p. 345–346). Thật vậy, nếu trong mệnh đề 6 ta giả sử rằng $f$ tăng ngặt (tương ứng giảm nghiêm ngặt) và liên tục trên I, và nếu $f'(x_0) = 0$, thì hàm nghịch đảo $g$ có đạo hàm bằng $+\infty$ (tương ứng $-\infty$) tại điểm $y_0 = f(x_0)$; nếu $f'(x_0) = +\infty$ (tương ứng $-\infty$), thì $g$ có đạo hàm bằng 0. Có những kết quả tương tự đối với các đạo hàm phải và trái, mà chúng tôi để bạn đọc tự xử lý.

Cho C là đồ thị hay đường biểu diễn của một hàm thực hữu hạn $f$, tập con của mặt phẳng $\mathbf{R}^2$ tạo thành bởi các điểm $(x, f(x))$ khi $x$ chạy qua tập hợp trên đó $f$ được xác định. Nếu hàm $f$ có đạo hàm phải hữu hạn tại một điểm $x_0 \in I$, thì nửa đường thẳng có gốc tại điểm $M_{x_0} = (x_0, f(x_0))$ của C, và có các hệ số chỉ phương $(1, f'_d(x_0))$ được gọi là nửa tiếp tuyến phải của đường cong C tại điểm $M_{x_0}$; khi $f'_d(x_0) = +\infty$ (resp. $f'_d(x_0) = -\infty$) ta cũng dùng thuật ngữ ấy cho nửa đường thẳng có gốc $M_{x_0}$ và có các hệ số chỉ phương $(0, 1)$ (resp. $(0, -1)$). Tương tự, người ta định nghĩa nửa tiếp tuyến trái tại $M_{x_0}$ khi $f'_g(x_0)$ tồn tại. Với các định nghĩa này, có thể kiểm tra nhanh rằng góc mà nửa tiếp tuyến phải (resp. trái) tạo với trục hoành là giới hạn của góc mà trục này tạo với nửa đường thẳng xuất phát từ $M_{x_0}$ và chuyển qua điểm $M_1 = (x, f(x))$ của C, khi $x$ tiến tới $x_0$ nhưng vẫn giữ $> x_0$ (resp. $< x_0$).

Cũng có thể nói rằng nửa tiếp tuyến phải (tương ứng trái) là giới hạn của nửa đường thẳng gốc tại $M_{x_0}$ chuyển qua $M_1$, khi ta trang bị cho tập hợp các nửa đường thẳng có cùng gốc tôpô không gian thương $C^*/\mathbf{R}_+^*$ (Top. Gén., VIII, p. 107).

Nếu hai nửa tiếp tuyến tồn tại tại một điểm $M_{x_0}$ của C, thì chúng chỉ có các hướng đối nhau khi $f$ có đạo hàm (hữu hạn hay không) tại điểm $x_0$ (giả sử là điểm trong của I); chúng chỉ trùng nhau khi $f'_d(x_0)$ và $f'_g(x_0)$ là vô hạn và trái dấu. Trong hai trường hợp ấy, ta nói rằng đường thẳng chứa hai nửa tiếp tuyến đó là tiếp tuyến với C tại điểm $M_{x_0}$.

Khi tiếp tuyến tại $M_{x_0}$ tồn tại, nó là giới hạn của đường thẳng đi qua $M_{x_0}$ và $M_1$ khi $x$ tiến tới $x_0$ mà vẫn $\neq x_0$, tôpô trên tập hợp các đường thẳng đi qua một điểm cố định cho trước là tôpô của không gian thương $C^*/\mathbf{R}^*$ (Gen. Top., VIII, p. 114).

Các khái niệm tiếp tuyến và nửa tiếp tuyến của một đồ thị là những trường hợp riêng của các khái niệm tổng quát sẽ được định nghĩa trong phần của Bộ sách này dành cho các đa tạp khả vi.

#### Định nghĩa 4 {#fvr-i-s1-def-4 .statement}

Ta nói rằng một hàm thực $f$, xác định trên một tập con A của một không gian tôpô E, có một cực đại tương đối (tương ứng, cực đại tương đối ngặt, cực tiểu tương đối, cực tiểu tương đối ngặt) tại một điểm $x_0 \in A$, tương đối với A, nếu tồn tại một lân cận $V$ của $x_0$ trong E sao cho tại mọi điểm $x \in V \cap A$ phân biệt với $x_0$ ta có $f(x) \leq f(x_0)$ (tương ứng, $f(x) < f(x_0)$, $f(x) \geq f(x_0)$, $f(x) > f(x_0)$).

Hiển nhiên là nếu $f$ đạt cận trên bé nhất của nó (tương ứng, cận dưới lớn nhất) trên A tại một điểm của A, thì nó có một cực đại tương đối (tương ứng, cực tiểu tương đối) tương đối với A tại điểm đó; dĩ nhiên mệnh đề đảo lại là sai.

Chú ý rằng nếu $B \subset A$, và nếu $f$ có (chẳng hạn) một cực đại tương đối tại một điểm $x_0 \in B$ tương đối với B, thì $f$ không nhất thiết có một cực đại tương đối tương đối với A tại điểm đó.

#### Mệnh đề 7 {#fvr-i-s1-prop-7 .statement}

Cho $f$ là một hàm thực hữu hạn, xác định trên một khoảng $I \subset \mathbf{R}$. Nếu $f$ đạt cực đại tương đối (tương ứng cực tiểu tương đối) tại một điểm $x_0$ nằm trong I, và có cả đạo hàm phải lẫn đạo hàm trái tại điểm này, thì ta có $f'_d(x_0) \leq 0$ và $f'_g(x_0) \geq 0$ (tương ứng $f'_d(x_0) \geq 0$ và $f'_g(x_0) \leq 0$); đặc biệt, nếu $f$ khả vi tại điểm $x_0$, thì $f'(x_0) = 0$.

Mệnh đề này suy ra một cách hiển nhiên từ các định nghĩa.

Ta còn có thể nói thêm rằng nếu tại một điểm $x_0$ nằm trong I, hàm $f$ khả vi và đạt một cực đại hoặc cực tiểu tương đối, thì tiếp tuyến với đồ thị của nó song song với trục hoành. Đảo lại là sai, như ví dụ hàm $x^3$ cho thấy: hàm này có đạo hàm không tại điểm $x = 0$, nhưng tại điểm đó không có cực đại tương đối cũng không có cực tiểu tương đối.

### Bài tập {#fvr-i-s1-exercises}

Xem [các bài tập cho § 1](exercises/s1/).
