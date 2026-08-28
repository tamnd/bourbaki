---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 3
section_title: Representations
lang: vi
source: lie-i-iii
pdf_pages: 0043-0056, 0103-0109
extraction: ocr
subsections:
    - "no": 1
      title: REPRESENTATIONS
      page: 0
      pdf_page: 43
    - "no": 2
      title: TENSOR PRODUCT OF REPRESENTATIONS
      page: 0
      pdf_page: 46
    - "no": 3
      title: REPRESENTATIONS ON HOMOMORPHISM MODULES
      page: 0
      pdf_page: 47
    - "no": 4
      title: EXAMPLES
      page: 0
      pdf_page: 49
    - "no": 5
      title: INVARIANT ELEMENTS
      page: 0
      pdf_page: 50
    - "no": 6
      title: INVARIANT BILINEAR FORMS
      page: 0
      pdf_page: 51
    - "no": 7
      title: CASIMIR ELEMENT
      page: 0
      pdf_page: 53
    - "no": 8
      title: EXTENSION OF THE BASE RING
      page: 0
      pdf_page: 54
statements: 24
exercises: 12
content_sha256: d68061b46eaf8aa73f1e61b949377c8fc158212390193dc63d1d1c49bedf6a60
translated_from: content/en/lie/I/03_s3_representations.md
source_content_sha256: 7d8bba5f2b515dc174b1c1ea0359bd8646b26cd6ba716e17900d892c6d4d330a
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-ca1be95b
glossary_version: 34
glossary_terms_sha256: 3c33cba0b88b2808727bcdbda09582f710d12ef5f0413789f52aefa5806ab4f9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. BIỂU DIỄN

### 1. BIỂU DIỄN

#### Định nghĩa 1 {#lie-i-s3-def-1 .statement}

*Cho $g$ là một đại số Lie trên $K$ và $M$ là một $K$-môđun. Một đồng cấu của $g$ vào đại số Lie $gl(M)$ được gọi là một biểu diễn của $g$ trên môđun $M$. Một biểu diễn đơn ánh được gọi là trung thành. Nếu $K$ là một trường, chiều (hữu hạn hoặc vô hạn) của $M$ trên $K$ được gọi là chiều của biểu diễn. Biểu diễn $x \mapsto \operatorname{ad} x$ của $g$ trên $K$-môđun $g$ được gọi là biểu diễn liên hợp của $g$.*

Một biểu diễn của $g$ trên $M$ do đó là một ánh xạ tuyến tính trên $K$ $\rho$ của $g$ vào môđun các tự đồng cấu của $M$ sao cho

$$
\rho([x, y]) \cdot m = \rho(x) \rho(y) \cdot m - \rho(y) \rho(x) \cdot m
$$

với mọi $x \in g, y \in g, m \in M$.

#### Ví dụ {#lie-i-s3-n1-exa-1 .statement}

Cho G là một nhóm Lie thực, g là đại số Lie của nó và θ là một biểu diễn giải tích của G trên một không gian vectơ thực hữu hạn chiều E. Khi đó đồng cấu tương ứng của g vào gl(E) là một biểu diễn của g trên E.*

Cho U là đại số bao quanh của g. Mệnh đề 1 của § 2, no. 1 xác định một sự tương ứng một-một giữa tập hợp các biểu diễn của g trên M và tập hợp các biểu diễn của U trên M. Mặt khác ta biết (Đại số, Chương VIII, § 13, no. 1) rằng có một sự tương đương giữa khái niệm biểu diễn của đại số kết hợp U và khái niệm môđun trái U.

#### Định nghĩa 2 {#lie-i-s3-def-2 .statement}

*Cho g là một đại số Lie trên K và U là đại số bao quanh của nó. Một môđun trái đơn vị trên U được gọi là một môđun trái g, hoặc đơn giản là một g-môđun.*

Nếu M là một g-môđun và x ∈ U, x_M sẽ chỉ phép vị tự của M xác định bởi x (xem Đại số, Chương VIII, § 1, no. 2).

Một môđun phải đơn vị trên U được gọi là một g-môđun phải. Một môđun như vậy được đồng nhất với một U^0-môđun trái, nghĩa là (§ 2, no. 4) với một g^0-môđun trái.

Cho φ là phản tự đồng cấu chính của U. Nếu M là một g-môđun phải, một cấu trúc g-môđun trái được xác định trên M bằng cách viết a.m = m.φ(a) với m ∈ M và a ∈ U.

Các khái niệm và các kết quả của lý thuyết môđun có thể được chuyển sang ngôn ngữ của các biểu diễn:

(1) Hai biểu diễn ρ và ρ' của g trên M và M' được gọi là *tương tự* hoặc *đẳng cấu* nếu các g-môđun M và M' là đẳng cấu. Điều này tương đương với việc tồn tại một đẳng cấu u của K-môđun M lên K-môđun M' sao cho

$$
\rho'(x) = u \circ \rho(x) \circ u^{-1}
$$

với mọi x ∈ g.

(2) Với mọi i ∈ I, cho ρ_i là một biểu diễn của g trên M_i. Cho M là g-môđun là tổng trực tiếp của các g-môđun M_i. Có một biểu diễn tương ứng ρ của g trên M, được gọi là *tổng trực tiếp* của các ρ_i và ký hiệu bởi $\sum_{i \in I} \rho_i$ (hoặc $\rho_1 + \cdots + \rho_n$ trong trường hợp có n biểu diễn $\rho_1, \ldots, \rho_n$). Nếu $m = (m_i)_{i \in I}$ là một phần tử của M và x ∈ g, thì $\rho(x).m = (\rho_i(x).m_i)_{i \in I}$.

(3) Một biểu diễn ρ của g trên M được gọi là *đơn* hoặc *bất khả quy* nếu g-môđun liên kết là đơn. Điều này tương đương với việc nói rằng không tồn tại môđun con-K nào của M (khác với {0} và M) ổn định đối với mọi $\rho(x), x \in g$. Một lớp các g-môđun đơn (Đại số, Chương VIII, § 3, no. 2) xác định một *lớp các biểu diễn đơn của g*.

(4) Một biểu diễn ρ của g trên M được gọi là *nửa đơn* hoặc *hoàn toàn khả quy* nếu g-môđun liên kết là nửa đơn. Điều này tương đương với việc nói rằng ρ tương tự với một tổng trực tiếp của các biểu diễn đơn hoặc rằng mọi môđun con-K của

M ổn định dưới $\rho(x)$ ($x \in g$) đều có một phần bù ổn định dưới $\rho(x)$ ($x \in g$) (xem *Đại số*, Chương VIII, § 3, no. 3).

(5) Cho $\delta$ là một lớp các biểu diễn đơn của $g$ tương ứng với một lớp C các g-môđun đơn. Mặt khác cho $\rho$ là một biểu diễn của g trên M. Thành phần đẳng kiểu $M_C$ thuộc loài C của g-môđun M (*Đại số*, Chương VIII, § 3, no. 4) cũng được gọi là *thành phần đẳng kiểu của M thuộc loài* $\delta$. Thành phần này là tổng của các môđun con-K của M ổn định dưới $\rho(x)$ và trên đó $\rho(x)$ cảm sinh một biểu diễn thuộc lớp $\delta$; nó là tổng trực tiếp của một số môđun con trong các môđun này; nếu $M_C$ có độ dài $n$, thì ρ được nói là *chứa* $\delta$ *n lần*. Tổng của các $M_C$ khác nhau là trực tiếp; nó bằng M khi và chỉ khi ρ là nửa đơn.

(6) Cho $\rho, \rho'$ là hai biểu diễn của $g$. $\rho'$ được gọi là một *biểu diễn con* (tương ứng *biểu diễn thương*) của $\rho$ nếu môđun của $\rho'$ là một môđun con (tương ứng môđun thương) của môđun của $\rho$.

Cho M là một K-môđun. Biểu diễn không của $g$ trên M xác định trên M một cấu trúc $g$-môđun. Với cấu trúc này M được gọi là một $g$-môđun *tầm thường*.

Cho M là một $g$-môđun. Các $g$-môđun thương của các môđun con-$g$ của M cũng là các môđun con-$g$ của các môđun thương của M: chúng thu được bằng cách xét hai môđun con-$g$ U, $U'$ của M sao cho $U \supset U'$ và lập $g$-môđun $U/U'$. Khi đó nếu mọi môđun đơn thuộc kiểu trên đều đẳng cấu với một $g$-môđun đơn N đã cho, M được gọi là một $g$-môđun *thuần* *loài* N. Nếu $\rho$ và $\sigma$ là các biểu diễn của $g$ tương ứng với M và N, ta cũng nói rằng $\rho$ là *thuần loài* $\sigma$.

Cho $M'$ là một môđun con-$g$ của M. Để M thuần loài N, điều kiện cần và đủ là $M'$ và $M/M'$ thuần loài N. Quả vậy, điều kiện này hiển nhiên là cần. Giả sử nó đúng và cho U, $U'$ là các môđun con-$g$ của M sao cho $U' \subset U$ và $U/U'$ là đơn; gọi $\phi$ là đồng cấu chính tắc từ M lên $M/M'$; nếu $\phi(U) \neq \phi(U')$, $U/U'$ đẳng cấu với $\phi(U)/\phi(U')$ và do đó đẳng cấu với N; nếu $\phi(U) = \phi(U')$, thì $U \subset U' + M'$, do đó $U/U'$ đẳng cấu với một môđun con đơn của $(U' + M')/U'$ và môđun sau cùng này tự nó đẳng cấu với $M'/(U' \cap M')$; do đó $U/U'$ lại đẳng cấu với N, vậy M thuần loài N.

Từ đây về sau, cho M là một $g$-môđun và giả sử rằng tập hợp các môđun con-$g$ của M thuần loài N thừa nhận một phần tử cực đại $M'$. Khi đó mọi môđun con $M''$ của M thuần loài N đều được chứa trong $M'$. Vì $M''/(M' \cap M'')$ và $M'$ đều thuần loài N, nên $M' + M''$ thuần loài N theo điều trên và do đó $M' + M'' \subset M'$.

Giả sử $g$-môđun M thừa nhận một chuỗi Jordan-Hölder $(M_i)_{0 \leq i \leq n}$. Để M thuần loài N, điều kiện cần và đủ là $M_0/M_1, M_1/M_2, \ldots, M_{n-1}/M_n$ đẳng cấu với N; vì điều kiện này hiển nhiên là cần và tính đủ của nó suy ra ngay lập tức bằng quy nạp theo $n$ từ điều đã thấy ở trên.

#### Mệnh đề 1 {#lie-i-s3-prop-1 .statement}

*Cho g là một đại số Lie trên K và a là một iđêan của g. Cho M là một môđun g* và $N$ là một $a$-môđun đơn. Xét $M$ như một $a$-môđun và giả sử rằng tập hợp các môđun con-$a$ của $M$ thuần nhất thuộc loài $N$ thừa nhận một phần tử cực đại $M'$. Khi đó $M'$ là một môđun con-$g$ của $M$.

Cho $y \in g$. Gọi $\phi$ là ánh xạ chính tắc của $M$ lên $M/M'$ và $f$ là ánh xạ $m \mapsto \phi(y_M \cdot m)$ của $M'$ vào $M/M'$. Chỉ cần chứng minh rằng $f(M') = \{0\}$. Cho $x \in a$. Khi đó, với $m \in M$,

$$
x_{M/M'} \cdot f(m) = \phi(x_M y_M \cdot m) = \phi(y_M x_M \cdot m) + \phi([x, y]_M \cdot m).
$$

Bây giờ $[x, y] \in a$, do đó $\phi([x, y]_M \cdot m) = 0$; mặt khác,

$$
\phi(y_M x_M \cdot m) = f(x_M \cdot m).
$$

Suy ra $x_{M/M'} \cdot f(m) = f(x_M \cdot m)$. Từ đó suy ra rằng $f(M')$ là một môđun con-$a$ của $M/M'$ đẳng cấu với một thương của $M'$ và do đó thuần nhất thuộc loài $N$; do đó $f(M') = \{0\}$.

#### Hệ quả {#lie-i-s3-n1-cor-1 .statement}

*Cho $g$ là một đại số Lie trên $K$ và $a$ là một iđêan của $g$. Cho $M$ là một môđun $g$ đơn, có độ dài hữu hạn như một môđun $K$. Tồn tại một $a$-môđun đơn $N$ sao cho $M$ là một $a$-môđun thuần nhất thuộc loài $N$.*

Vì $a$-môđun $M$ có độ dài hữu hạn, tồn tại một phần tử cực tiểu $N$ trong tập hợp các môđun con-$a$ của $M$: nó là một môđun con-$a$ đơn của $M$. Môđun con-$a$ lớn nhất của $M$ thuần nhất thuộc loài $N$ do đó là $\neq \{0\}$ và là một môđun con-$g$ của $M$ (Mệnh đề 1), và vì vậy trùng với $M$.

### 2. TÍCH TENXƠ CỦA CÁC BIỂU DIỄN

Ta đã định nghĩa trong no. 1 tổng trực tiếp của một họ các biểu diễn của $g$. Bây giờ ta sẽ định nghĩa các phép toán khác trên các biểu diễn.

Cho $g_1, g_2$ là hai đại số Lie trên $K$ và $M_i$ là một $g_i$-môđun ($i = 1, 2$). Gọi $U_i$ là đại số bao quanh của $g_i$ và $\sigma_i$ là ánh xạ chính tắc của $g_i$ vào $U_i$. Khi đó $M_i$ là một $U_i$-môđun trái và do đó $M_1 \otimes_K M_2$ có một cấu trúc môđun trái chính tắc trên $(U_1 \otimes_K U_2)$. Bây giờ $U_1 \otimes_K U_2$ là đại số bao quanh của $g_1 \times g_2$ và ánh xạ $(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)$ là ánh xạ chính tắc của $g_1 \times g_2$ vào đại số bao quanh này (§ 2, no. 2). Do đó tồn tại một cấu trúc $(g_1 \times g_2)$-môđun trên $M = M_1 \otimes_K M_2$ sao cho:

$$
\begin{align*}
(1) \quad (x_1, x_2)_M \cdot (m_1 \otimes m_2) &= (\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot (m_1 \otimes m_2) \\
&= ((x_1)_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes ((x_2)_{M_2} \cdot m_2).
\end{align*}
$$

Cấu trúc này xác định một biểu diễn của $g_1 \times g_2$ trên $M$.

Nếu bây giờ $g_1 = g_2 = g$, đồng cấu $x \mapsto (x, x)$ của $g$ vào $g \times g$, hợp với biểu diễn trên, xác định một biểu diễn của $g$ trên $M$ và do đó một cấu trúc $g$-môđun trên $M$ sao cho:

$$
(2) \quad x_M \cdot (m_1 \otimes m_2) = (x_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes (x_{M_2} \cdot m_2).
$$

Bằng một lập luận tương tự ta thấy rằng:

#### Mệnh đề 2 {#lie-i-s3-prop-2 .statement}

Cho $g$ là một đại số Lie trên $K$ và $M_i$ là một $g$-môđun ($1 \leq i \leq n$). Trên tích tenxơ $M_1 \otimes_K M_2 \otimes \cdots \otimes M_n$, tồn tại một và chỉ một cấu trúc $g$-môđun sao cho

$$
x_M \cdot (m_1 \otimes \cdots \otimes m_m) = \sum_{t=1}^n m_1 \otimes \cdots \otimes (x_{M_t} \cdot m_i) \otimes \cdots \otimes m_n
$$

với mọi $x \in g, m_1 \in M_1, \ldots, m_n \in M_n$.

Biểu diễn tương ứng được gọi là *tích tenxơ* của các biểu diễn đã cho của $g$ trên các $M_i$.

Đặc biệt, nếu $M$ là một $g$-môđun, Mệnh đề 2 xác định một cấu trúc $g$-môđun trên mỗi $M_p = \bigotimes^p M$ và do đó trên đại số tenxơ $T$ của $M$.

Công thức (3) chỉ ra rằng, với mọi $x \in g, x_T$ là đạo hàm *duy nhất* của đại số $T$ mở rộng $x_M$. Ta biết (§ 2, no. 8) rằng $x_T$ xác định, khi chuyển qua thương, một đạo hàm của đại số đối xứng $S$ của $M$. Do đó $S$ có thể được xem như một $g$-môđun thương của $T$ và các $x_S$ là các đạo hàm của $S$.

Đặc biệt hơn nữa, xét $g$ như một $g$-môđun bằng cách dùng biểu diễn phụ hợp của $g$. Gọi $U$ là đại số bao quanh của $g$. Theo Mệnh đề 7 của § 2, $x_M$ xác định, bằng cách chuyển qua các thương, một đạo hàm của $U$, chính là đạo hàm nội xác định bởi $\sigma(x)$ ($\sigma$ ký hiệu ánh xạ chính tắc của $g$ vào $U$). Khi đó $U$ có thể được xem như một $g$-môđun thương của $T$. Nếu $K$ là một trường có đặc số 0, đẳng cấu chính tắc của $S$ lên $U$ là một đẳng cấu $g$-môđun (§ 2, no. 8).

### 3. BIỂU DIỄN TRÊN CÁC MÔĐUN ĐỒNG CẤU

Một lần nữa, cho $g_1$ và $g_2$ là hai đại số Lie trên $K$ và $M_i$ là một $g_i$-môđun ($i = 1, 2$). Gọi $U_i$ là đại số bao quanh của $g_i$ và $\sigma_i$ là ánh xạ chính tắc của $g_i$ vào $U_i$. Khi đó $M_i$ là một $U_i$-môđun trái và do đó $\mathcal{L}_K(M_1, M_2)$ có một cấu trúc môđun trái chính tắc $(U_1^0 \otimes U_2)$. Bây giờ $U_1^0 \otimes_K U_2$ là đại số bao quanh của $g_1^0 \times g_2$ và ánh xạ

$$
(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)
$$

là ánh xạ chính tắc của $g_1^0 \times g_2$ vào đại số bao quanh này. Do đó tồn tại một cấu trúc $(g_1^0 \times g_2)$-môđun trên $M = \mathcal{L}_K(M_1, M_2)$ sao cho

$$
((x_1, x_2)_M \cdot u) \cdot m_1 = ((\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot u) \cdot m_1 \\
= u((x_1)_{M_1} \cdot m_1) + (x_2)_{M_2} \cdot u(m_1)
$$

với mọi $u \in \mathcal{L}_K(M_1, M_2), m_1 \in M_1$. Cấu trúc này xác định một biểu diễn của $g_1^0 \times g_2$ trên $M$.

Nếu bây giờ $g_1 = g_2 = g$, đồng cấu $x \mapsto (-x, x)$ của $g$ vào $g^0 \times g$, hợp với biểu diễn trên, xác định một biểu diễn của $g$ trên $M$ và do đó một cấu trúc $g$-môđun trên $M$ sao cho

$$
(x_M \cdot u) \cdot m_1 = x_{M_2} \cdot u(m_1) - u(x_{M_1} \cdot m_1)
$$

hoặc

$$
x_M \cdot u = x_{M_2} u - u x_{M_1}.
$$

Kết hợp các kết quả này với Mệnh đề 2, ta thấy rằng:

#### Mệnh đề 3 {#lie-i-s3-prop-3 .statement}

*Cho $g$ là một đại số Lie trên $K$ và $M_i$ là một $g$-môđun ($1 \leq i \leq n + 1$). Cho $N$ là $K$-môđun $\mathcal{L}_K(M_1, \ldots, M_n; M_{n+1})$ gồm các ánh xạ đa tuyến từ $\prod_{i=1}^n M_i$ vào $M_{n+1}$. Tồn tại duy nhất một cấu trúc $g$-môđun trên $N$ sao cho*

$$
(x_N \cdot u)(m_1, \ldots, m_n) = - \sum_{i=1}^n u(m_1, \ldots, x_{M_i} \cdot m_i, \ldots, m_n)
$$
$$
+ x_{M_{n+1}} \cdot u(m_1, \ldots, m_n)
$$

*đối với mọi* $x \in g, u \in N$ *và* $m_i \in M_i$ ($1 \leq i \leq n$).

Đặc biệt, cho $g$ là một đại số Lie trên $K$ và $M$ là một $g$-môđun, và xét $K$ như một $g$-môđun tầm thường. Mệnh đề 3 xác định một cấu trúc $g$-môđun trên $\mathcal{L}_K(M, K) = M^*$. Biểu diễn tương ứng được gọi là biểu diễn *đối ngẫu* của biểu diễn $x \mapsto x_M$. Ta có:

$$
(x_{M^*} \cdot f)(m) = -f(x_M \cdot m)
$$

đối với mọi $x \in g, f \in M^*, m \in M$. Nói cách khác:

$$
x_{M^*} = -{}^t x_M.
$$

Khi $K$ là một trường và $M$ là hữu hạn chiều, $g$-môđun $M$ là đơn (tương ứng, nửa đơn) khi và chỉ khi $g$-môđun $M^*$ là đơn (tương ứng, nửa đơn).

#### Mệnh đề 4 {#lie-i-s3-prop-4 .statement}

*Cho $M_1, M_2$ là hai $g$-môđun. Các ánh xạ $K$-tuyến tính chính tắc* (Đại số, Chương II, § 4, no. 2, Mệnh đề 2 và no. 1, Mệnh đề 1):

$$
M_1^* \otimes_K M_2 \xrightarrow{\phi} \mathcal{L}_K(M_1, M_2), \quad \mathcal{L}_K(M_1, M_2^*) \xrightarrow{\psi} (M_1 \otimes_K M_2)^*
$$

*(trong đó ánh xạ thứ hai là song ánh)* là các đồng cấu $g$-môđun.

Ta viết

$$
N = M_1^* \otimes M_2, \quad P = \mathcal{L}(M_1, M_2), \quad Q = \mathcal{L}(M_1, M_2^*), \quad R = (M_1 \otimes M_2)^*.
$$

Khi đó, với $x \in g, f \in M_1^*, m_1 \in M_1, m_2 \in M_2$,

$$
((\phi x_N)(f \otimes m_2)) \cdot m_1 = (\phi(x_{M_1^*} f \otimes m_2 + f \otimes x_{M_2} m_2)) \cdot m_1 \\
= \langle x_{M_1^*} f, m_1 \rangle m_2 + \langle f, m_1 \rangle x_{M_2} m_2
$$

$$
((x_P \phi)(f \otimes m_2)) \cdot m_1 = x_{M_2}(\phi(f \otimes m_2) \cdot m_1) - \phi(f \otimes m_2)(x_{M_1} m_1) \\
= \langle f, m_1 \rangle x_{M_2} m_2 - \langle f, x_{M_1} m_1 \rangle m_2
$$

và do đó $\phi x_N = x_P \phi$. Mặt khác, với $x \in g, u \in \mathcal{L}(M_1, M_2^*), m_1 \in M_1, m_2 \in M_2$:

$$
(\psi x_Q u)(m_1 \otimes m_2) = \langle (x_Q u) \cdot m_1, m_2 \rangle = \langle x_{M_2^*} u m_1 - u x_{M_1} m_1, m_2 \rangle \\
(x_R \psi u)(m_1 \otimes m_2) = -\langle \psi u, x_{M_1} m_1 \otimes m_2 + m_1 \otimes x_{M_2} m_2 \rangle \\
= -\langle u x_{M_1} m_1, m_2 \rangle - \langle u m_1, x_{M_2} m_2 \rangle
$$

và do đó $\psi x_Q = x_R \psi$, điều này hoàn thành chứng minh.

Các $g$-môđun $\mathcal{L}(M_1, M_2^*)$ và $(M_1 \otimes M_2)^*$ được đồng nhất dưới đẳng cấu $\psi$. Nếu $M_1$ và $M_2$ có các cơ sở hữu hạn, $\phi$ là một đẳng cấu (Algebra, Chapter II, § 4, no. 2, Proposition 2), điều này cho phép chúng ta đồng nhất các $g$-môđun $M_1^* \otimes M_2$ và $\mathcal{L}(M_1, M_2)$; trong trường hợp đó, do đó chúng ta có thể đồng nhất các $g$-môđun $M_1^* \otimes M_2^*, \mathcal{L}(M_1, M_2^*)$ và $(M_1 \otimes M_2)^*$.

### 4. VÍ DỤ

#### Ví dụ 1 {#lie-i-s3-n4-exa-1 .statement}

Cho $g$ là một đại số Lie trên $K$ và $M$ là một $g$-môđun. Cấu trúc $g$-môđun trên $M$ và cấu trúc $g$-môđun tầm thường trên $K$ xác định một cấu trúc $g$-môđun trên $K$-môđun $N = \mathcal{L}(M, M; K)$ của các dạng song tuyến tính trên $M$. Khi đó

$$
(x_N \cdot \beta)(m, m') = -\beta(x_M \cdot m, m') + \beta(m, x_M \cdot m')
$$

với mọi $x \in g, m, m'$ trong $M, \beta \in N$. Nếu $\beta$ là một phần tử đã cho của $N$, tập hợp các $x \in g$ sao cho $x_N \cdot \beta = 0$ là một đại số con của $g$.

Cho $M$ là một $K$-môđun và $\beta$ là một dạng song tuyến tính trên $M$. Theo trên, tập hợp các $x \in gl(M)$ sao cho

$$
\beta(x \cdot m, m') + \beta(m, x \cdot m') = 0
$$

với mọi $m \in M$ và $m' \in M$ là một đại số con Lie của $gl(M)$. Giả sử rằng $K$ là một trường, $M$ là hữu hạn chiều và $\beta$ không suy biến. Khi đó mọi $x \in gl(M)$ đều có một liên hợp trái $x^*$ (đối với $\beta$) được xác định khắp nơi và đại số con đang xét là tập hợp các $x \in gl(M)$ sao cho $x^* = -x$. Bằng quá trình này chúng ta có thể xây dựng hai ví dụ quan trọng của các đại số Lie:

(a) Lấy $M = K^n$ và

$$
\beta((\xi_1, \ldots, \xi_n), (\eta_1, \ldots, \eta_n)) = \xi_1 \eta_1 + \cdots + \xi_n \eta_n.
$$

Chúng ta đồng nhất một cách chính tắc $gl(K^n)$ với $M_n(K)$. Khi đó đại số Lie thu được là đại số Lie của các ma trận đối xứng lệch. *(Khi $K = \mathbf{R}$, đại số này là đại số Lie của nhóm trực giao $O(n, \mathbf{R})$).*

(b) Lấy $M = K^{2m}$ và
$$
\beta((\xi_1, \ldots, \xi_{2m}), (\eta_1, \ldots, \eta_{2m})) = \xi_1 \eta_{m+1} - \eta_1 \xi_{m+1} + \cdots + \xi_m \eta_{2m} - \eta_m \xi_{2m}.
$$
Ma trận của $\beta$ đối với cơ sở chính tắc của $K^{2m}$ là ma trận
$$
\begin{pmatrix}
0 & I_m \\
-I_m & 0
\end{pmatrix}.
$$
Cho $U = \begin{pmatrix} A & B \\ C & D \end{pmatrix}$ là ma trận đối với cơ sở chính tắc của $K^{2m}$ của một phần tử $u$ của $\mathrm{gl}(M)$ ($A, B, C, D$ nằm trong $\mathbf{M}_m(K)$). Theo công thức (50) của *Đại số*, Chương IX, § 1, no. 10, $u^*$ có đối với cùng cơ sở ma trận
$$
\begin{pmatrix}
0 & -I_m \\
I_m & 0
\end{pmatrix}
\begin{pmatrix}
tA & tC \\
tB & tD
\end{pmatrix}
\begin{pmatrix}
0 & I_m \\
-I_m & 0
\end{pmatrix}
= \begin{pmatrix}
tD & -tB \\
-tC & tA
\end{pmatrix}.
$$
Điều kiện $u^* = -u$ do đó tương đương với các điều kiện
$$
D = -tA \quad B = tB \quad C = tC.
$$
*Khi $K = \mathbf{R}$, đại số Lie thu được là đại số Lie của nhóm symplectic $\mathbf{Sp}(2m, \mathbf{R})$.*

#### Ví dụ 2 {#lie-i-s3-n4-exa-2 .statement}

Ta giữ ký hiệu của *Ví dụ 1*.

Cấu trúc môđun-$g$ trên $M$ xác định trên môđun-$K$ $P = \mathcal{L}_K(M, M)$ của các tự đồng cấu của $M$ một cấu trúc môđun-$g$. Theo (6), với mọi $x \in g$ và $u \in P$:
$$(11)$$
$$
x_P \cdot u = [x_M, u] = (\mathrm{ad}\, x_M) \cdot u
$$
trong đó $\mathrm{ad}\, x_M$ chỉ ảnh của $x_M$ qua biểu diễn phụ hợp của $\mathrm{gl}(M)$. Nói cách khác:
$$(12)$$
$$
x_P = \mathrm{ad}\, x_M
$$
trong $\mathcal{L}(\mathcal{L}(M, M)) = \mathcal{L}(\mathrm{gl}(M))$.

### 5. CÁC PHẦN TỬ BẤT BIẾN

#### Định nghĩa 3 {#lie-i-s3-def-3 .statement}

*Một phần tử $m \in M$ của một đại số Lie $g$ và một môđun-$g$ $M$ được gọi là bất biến (đối với cấu trúc môđun-$g$ trên $M$ hoặc đối với biểu diễn tương ứng của $g$) nếu $x_M \cdot m = 0$ với mọi $x \in g$.*

*Một nhóm Lie thực liên thông $G$, $g$ là đại số Lie của nó, $\theta$ là một biểu diễn giải tích của $G$ trên một không gian vectơ thực hữu hạn chiều $E$ và $\rho$ là biểu diễn tương ứng của $g$ trên $E$. Cho $m \in E$. Phần tử $m$ là bất biến đối với $\rho$ khi và chỉ khi $\theta(g) \cdot m = m$ với mọi $g \in G$. Điều này giải thích việc sử dụng từ "bất biến".*

#### Ví dụ 1 {#lie-i-s3-n5-exa-1 .statement}

Cho $M, N$ là hai $g$-môđun và $P = \mathcal{L}_K(M, N)$. Để một phần tử $f$ của $P$ là bất biến, theo (6), điều kiện cần và đủ là $f$ là một đồng cấu của $g$-môđun $M$ vào $g$-môđun $N$. Đặc biệt, nếu $M = N$ và $x_M = x_N$ với mọi $x \in g$, thì $f$ là bất biến khi và chỉ khi $f$ giao hoán được với các $x_M$.

#### Ví dụ 2 {#lie-i-s3-n5-exa-2 .statement}

Cho M là một K-môđun có một cơ sở hữu hạn. Nếu M có một cấu trúc $g$-môđun, $\mathcal{L}(M, M)$ và $M^* \otimes M$ có các cấu trúc $g$-môđun và ánh xạ chính tắc của $M^* \otimes M$ vào $\mathcal{L}(M, M)$ là một đẳng cấu $g$-môđun (Mệnh đề 4). Vì $1 \in \mathcal{L}(M, M)$ hiển nhiên là một phần tử bất biến (xem Ví dụ 1), nên phần tử $u$ tương ứng của $M^* \otimes M$ là một phần tử bất biến. Nếu $(e_i)_{1 \leq i \leq n}$ là một cơ sở của M và $(e_i^*)_{1 \leq i \leq n}$ là cơ sở đối ngẫu, ta có $u = \sum_{i=1}^n e_i^* \otimes e_i$.

#### Ví dụ 3 {#lie-i-s3-n5-exa-3 .statement}

Cho M là một $g$-môđun. Cho $\beta$ là một dạng song tuyến tính trên M và f là phần tử tương ứng của $\mathcal{L}(M, M^*)$. Để $\beta$ là bất biến, điều kiện cần và đủ là f là một đồng cấu $g$-môđun (Mệnh đề 4 và Ví dụ 1). Giả sử rằng K là một trường và rằng $\dim_K M < +\infty$. Một dạng song tuyến tính bất biến không suy biến $\beta$ trên M xác định một đẳng cấu của $g$-môđun M lên $g$-môđun $M^*$ và do đó một đẳng cấu của $g$-môđun $M \otimes M$ lên $g$-môđun $M^* \otimes M$. Vì vậy, theo Ví dụ 2, việc cho $\beta$ xác định một cách chính tắc một phần tử bất biến c trong $g$-môđun $M \otimes M$, phần tử này có thể được xây dựng như sau: cho $(e_i)_{1 \leq i \leq n}$ là một cơ sở của M và $(e'_i)_{1 \leq i \leq n}$ là cơ sở của M sao cho $\beta(e_i, e'_j) = \delta_{ij}$; khi đó $c = \sum_{i=1}^n e_i \otimes e'_i$.

#### Mệnh đề 5 {#lie-i-s3-prop-5 .statement}

*Cho g là một đại số Lie trên K, h là một iđêan của g, $\rho$ là một biểu diễn của g trên M và $\rho'$ là hạn chế của $\rho$ vào h. Khi đó tập hợp N các phần tử của M bất biến đối với $\rho'$ là ổn định dưới $\rho(g)$.*

Cho $n \in N$ và $y \in g$; với mọi $x \in h, [x, y] \in h$ và do đó
$$
\rho(x)\rho(y)n = \rho([x, y])n + \rho(y)\rho(x)n = 0;
$$
do đó $\rho(y)n \in N$.

#### Mệnh đề 6 {#lie-i-s3-prop-6 .statement}

*Cho M là một $g$-môđun nửa đơn. Khi đó môđun con $M_0$ gồm các phần tử bất biến của M thừa nhận duy nhất một phần bù ổn định dưới các $x_M$, cụ thể là môđun con $M_1$ sinh bởi các $x_M.m$ ($x \in g, m \in M$).*

Cho $M'$ là một môđun con của M ổn định dưới $x_M$ và là một phần bù của $M_0$ trong M. Với mọi $m \in M, m = m_0 + m'$ với $m_0 \in M_0, m' \in M'$, và do đó $x_M m = x_M m' \in M'$. Suy ra $M_1 \subset M'$. Gọi $M_2$ là một môđun con của $M'$ ổn định dưới $x_M$ và bổ sung cho $M_1$ trong $M'$. Với mọi $m \in M_2$,
$$
x_M m \in M_2 \cap M_1 = \{0\}
$$
với mọi $x \in g$, do đó $m \in M_0$ và do đó $m = 0$. Suy ra $M_2 = \{0\}$, điều này chứng minh rằng $M_1 = M'$.

### 6. CÁC DẠNG SONG TUYẾN TÍNH BẤT BIẾN

Cho g là một đại số Lie trên K. Biểu diễn phụ hợp của g trên g và biểu diễn không của g trên K định nghĩa một cấu trúc g-môđun trên K-môđun

$N = \mathcal{L}(g, g; K)$ gồm các dạng song tuyến tính trên $g$. Nói ngắn gọn, ta nói rằng một dạng song tuyến tính $\beta$ trên $g$ là *bất biến* nếu nó bất biến dưới biểu diễn $x \mapsto x_N$. Theo công thức (10), điều kiện cần và đủ để điều này xảy ra là:

$$
\beta([x, y], z) = \beta(x, [y, z])
$$

với mọi $x, y, z$ trong $g$.

Bây giờ gọi $\mathfrak{d}$ là đại số Lie của các phép dẫn xuất của $g$. Biểu diễn đồng nhất của $\mathfrak{d}$ và biểu diễn không của $\mathfrak{d}$ trên K định nghĩa một biểu diễn $D \mapsto D_N$ của $\mathfrak{d}$ trên $N$. Nói ngắn gọn, ta nói rằng một dạng song tuyến tính trên $g$ là *hoàn toàn bất biến* nếu nó bất biến dưới biểu diễn $D \mapsto D_N$. Một dạng song tuyến tính hoàn toàn bất biến là bất biến. Để một dạng song tuyến tính $\beta$ trên $g$ là hoàn toàn bất biến, điều kiện cần và đủ là:

$$
\beta(Dx, y) + \beta(x, Dy) = 0
$$

với mọi $x, y$ trong $g$ và $D \in \mathfrak{d}$.

#### Mệnh đề 7 {#lie-i-s3-prop-7 .statement}

*Cho $g$ là một đại số Lie, $\beta$ là một dạng song tuyến tính đối xứng bất biến trên $g$ và $a$ là một iđêan của $g$.*

(a) *Phần tử trực giao $a'$ của $a$ đối với $\beta$ là một iđêan của $g$.*

(b) *Nếu $a$ là đặc số và $\beta$ là hoàn toàn bất biến, thì $a'$ là đặc số.*

(c) *Nếu $\beta$ không suy biến, thì $a \cap a'$ là giao hoán.*

Cho $D$ là một đạo hàm của $g$. Giả sử rằng $a$ ổn định dưới $D$ và rằng $\beta(Dx, y) + \beta(x, Dy) = 0$ với $x, y$ thuộc $g$. Khi đó $z \in a'$ kéo theo $Dz \in a'$, vì, với mọi $t \in a$, $Dt \in a$ và do đó $\beta(Dz, t) = -\beta(z, Dt) = 0$. Vậy $a'$ ổn định dưới $D$. Điều này thiết lập (a) và (b).

Bây giờ cho $b$ là một iđêan của $g$ và giả sử rằng hạn chế của $\beta$ lên $b$ là không. Với $x, y$ thuộc $b$ và $z \in g$, $\beta([x, y], z) = \beta(x, [y, z]) = 0$, vì $[y, z] \in b$. Do đó $[b, b]$ trực giao với $g$. Nếu $\beta$ không suy biến, thì $b$ do đó là giao hoán. Kết quả này áp dụng cho $a \cap a'$ chứng minh (c).

#### Định nghĩa 4 {#lie-i-s3-def-4 .statement}

*Cho $g$ là một đại số $K$-Lie và $M$ là một $g$-môđun. Giả sử rằng $M$, được xem như một $K$-môđun, thừa nhận một cơ sở hữu hạn. Dạng song tuyến tính liên kết với $g$-môđun $M$ (hoặc với biểu diễn tương ứng) là dạng song tuyến tính đối xứng $(x, y) \mapsto \operatorname{Tr}(x_M y_M)$ trên $g$. Nếu biểu diễn đang xét là biểu diễn phụ hợp, dạng song tuyến tính liên kết được gọi là dạng Killing của $g$.*

#### Mệnh đề 8 {#lie-i-s3-prop-8 .statement}

*Cho $g$ là một đại số Lie và $M$ là một $g$-môđun. Giả sử rằng $M$, được xem như một $K$-môđun, thừa nhận một cơ sở hữu hạn. Dạng song tuyến tính liên kết với $M$ là bất biến.*

Với $x, y, z$ thuộc $g$, ta có:

$$
\begin{align*}
\operatorname{Tr}([x, y]_M z_M) &= \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(y_M x_M z_M) = \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(x_M z_M y_M) \\
&= \operatorname{Tr}(x_M [y, z]_M).
\end{align*}
$$

#### Mệnh đề 9 {#lie-i-s3-prop-9 .statement}

*Giả sử rằng $K$ là một trường và rằng đại số Lie $g$ là hữu hạn chiều* trên $K$. *Cho $a$ là một iđêan của $g$, $\beta$ là dạng Killing của $g$ và $\beta'$ là dạng Killing của $a$. Khi đó $\beta'$ là hạn chế của $\beta$ lên $a$.*

Cho $u$ là một tự đồng cấu của không gian vectơ $g$ giữ ổn định $a$. Cho $v$ là hạn chế của $u$ vào $a$ và $w$ là tự đồng cấu của không gian vectơ $g/a$ dẫn xuất từ $u$ khi chuyển qua thương. Khi đó $\operatorname{Tr} u = \operatorname{Tr} v + \operatorname{Tr} w$ như thấy được bằng cách lấy một cơ sở $(x_1, \ldots, x_n)$ của $g$ mà $p$ phần tử đầu tiên lập thành một cơ sở của $a$. Khi đó cho $x \in a, y \in a$ và áp dụng công thức trên vào trường hợp $u = (\operatorname{ad}_g x)(\operatorname{ad}_g y)$. Khi đó $v = (\operatorname{ad}_a x)(\operatorname{ad}_a y)$ và $w = 0$. Suy ra $\beta(x, y) = \beta'(x, y)$.

#### Mệnh đề 10 {#lie-i-s3-prop-10 .statement}

*Giả sử rằng $K$ là một trường và đại số Lie $g$ là hữu hạn chiều trên $K$. Dạng Killing $\beta$ của $g$ là hoàn toàn bất biến.*

Cho $D$ là một đạo hàm của $g$. Tồn tại một đại số Lie $g'$ chứa $g$ như một iđêan có đối chiều 1 và một phần tử $x_0$ của $g'$ sao cho $Dx = [x_0, x]$ với mọi $x \in g$ (§ 1, no. 8, Ví dụ 1). Cho $\beta'$ là dạng Killing của $g'$. Với $x, y$ trong $g$, $\beta'([x, x_0], y) = \beta'(x, [x_0, y])$, nghĩa là $\beta'(Dx, y) + \beta'(x, Dy) = 0$. Bây giờ hạn chế của $\beta'$ vào $g$ là $\beta$ (Mệnh đề 9). Do đó mệnh đề.

### 7. PHẦN TỬ CASIMIR

#### Mệnh đề 11 {#lie-i-s3-prop-11 .statement}

*Cho $g$ là một đại số Lie trên một trường $K$, $U$ là đại số bao quanh của nó, $h$ là một iđêan hữu hạn chiều của $g$ và $\beta$ là một dạng song tuyến tính bất biến trên $g$, mà hạn chế của nó vào $h$ là không suy biến. Cho $(e_i)_{1 \leq i \leq n}, (e'_j)_{1 \leq j \leq n}$ là hai cơ sở của $h$ sao cho $\beta(e_i, e'_j) = \delta_{ij}$. Khi đó phần tử $c = \sum_{i=1}^n e_i e'_i$ của $U$ thuộc về tâm của $U$ và độc lập với lựa chọn cơ sở $(e_i)$.*

Với $x \in g$, cho $x_h$ là hạn chế xuống $h$ của $\operatorname{ad}_g x$. Khi đó $x \mapsto x_h$ là một biểu diễn của $g$ trên không gian vectơ $h$ và hạn chế $\beta'$ của $\beta$ xuống $h$ là bất biến đối với biểu diễn này. Theo no. 5, *Ví dụ 3*, tenxơ $\sum_{i=1}^n e_i \otimes e'_i$ là độc lập với lựa chọn cơ sở $(e_i)$ và là một phần tử bất biến của đại số tenxơ của $h$. Nó cũng là một phần tử của đại số tenxơ $T$ của $g$, đại số này bất biến đối với biểu diễn dẫn xuất từ biểu diễn phụ hợp của $g$. Ảnh chính tắc của nó trong $U$, tức là $c$, do đó độc lập với lựa chọn cơ sở $(e_i)$ và là một bất biến đối với biểu diễn của $g$ trên $U$ được xét ở cuối no. 2. Do đó phần tử này khả hoán với mọi phần tử của $g$ và vì thế thuộc tâm của $U$.

Khi $\beta$ là dạng song tuyến tính liên kết với một $g$-môđun $M$, phần tử $c$ của Mệnh đề 11 được gọi là *phần tử Casimir* liên kết với $M$ (hoặc với biểu diễn tương ứng). Phần tử này tồn tại nếu hạn chế của $\beta$ xuống $h$ là không suy biến.

#### Mệnh đề 12 {#lie-i-s3-prop-12 .statement}

*Cho $g$ là một đại số Lie trên một trường $K$, $h$ là một iđêan của $g$ có số chiều hữu hạn n và M là một g-môđun có số chiều hữu hạn trên K. Cho c là phần tử Casimir (giả sử tồn tại) liên kết với M và h.

(a) $\operatorname{Tr}(c_M) = n$.
(b) *Nếu M là đơn và n không chia hết cho đặc số của K, $c_M$ là một tự đẳng cấu của M*.

Theo ký hiệu của Mệnh đề 11,

$$
\operatorname{Tr}(c_M) = \sum_{i=1}^n \operatorname{Tr}((e_i)_M(e'_i)_M) = \sum_{i=1}^n \beta(e_i, e'_i) = n.
$$

Do đó, nếu n không chia hết cho đặc số của K, $c_M \neq 0$. Mặt khác, vì c thuộc tâm của U, $c_M$ khả hoán với mọi $x_M, x \in g$. Nếu thêm M là đơn, $c_M$ do đó khả nghịch trong $\mathcal{L}(M)$ (*Đại số*, Chương VIII, § 4, no. 3, Mệnh đề 2).

### 8. MỞ RỘNG VÀNH CƠ SỞ

Cho $K_1$ là một vành giao hoán có phần tử đơn vị và $\phi$ là một đồng cấu của K vào $K_1$ ánh xạ 1 thành 1. Cho g là một đại số Lie trên K, U là đại số bao của nó và M là một g-môđun trái, tức là một U-môđun trái. Khi đó $M_{(K_1)}$ có một cấu trúc môđun trái chính tắc $U_{(K_1)}$ và do đó một cấu trúc g-môđun trái $g_{(K_1)}$. Gọi $\rho$ và $\rho_{(K_1)}$ là các biểu diễn của g và $g_{(K_1)}$ tương ứng với M và $M_{(K_1)}$: $\rho_{(K_1)}$ được nói là dẫn xuất từ $\rho$ bằng cách *mở rộng vành cơ sở* và các kết quả của *Đại số*, Chương VIII, § 13, no. 4 có thể được áp dụng. Nếu $x \in g$, $\rho_{(K_1)}(x)$ chỉ là tự đồng cấu $\rho(x) \otimes 1$ của $M_{(K_1)} = M \otimes_K K_1$.

Giả sử K là một trường, $K_1$ là một mở rộng của K và $\phi$ là đơn ánh chính tắc của K vào $K_1$. Cho V và V' là các không gian con vectơ của M. Gọi a là không gian con vectơ của g gồm các $x \in g$ sao cho $\rho(x)(V) \subset V'$. Gọi $a'$ là không gian con vectơ của $g_{(K_1)}$ gồm các $x' \in g_{(K_1)}$ sao cho $\rho_{(K_1)}(x')(V_{(K_1)}) \subset V'_{(K_1)}$. Khi đó $a' = a_{(K_1)}$. Vì rõ ràng $a_{(K_1)} \subset a'$. Bây giờ cho $x' \in a'$. Ta có thể viết $x' = \sum_{i=1}^n \lambda_i x_i$, trong đó các $x_i$ thuộc g và các $\lambda_i$ là các phần tử của $K_1$ độc lập tuyến tính trên K. Với mọi $u \in V$, $\rho(x') \cdot u \in V'_{(K_1)}$, tức là $\sum_{i=1}^n \lambda_i \rho(x_i) \cdot u \in V'_{(K_1)}$, do đó $\rho(x_i) \cdot u \in V'$, suy ra $x_i \in a$ và $x' \in a_{(K_1)}$. Điều này chứng minh rằng $a' = a_{(K_1)}$. Đặc biệt, *tâm* của $g_{(K_1)}$ được dẫn xuất từ tâm của g bằng cách mở rộng K thành $K_1$: chỉ cần áp dụng điều trên cho biểu diễn liên hợp của g. Suy ra rằng $\mathcal{C}_p(g_{(K_1)}) = (\mathcal{C}_p g)_{(K_1)}$ với mọi $p$. Tương tự, cho h là một đại số con của g và n là *bộ chuẩn hóa* của h trong g. Khi đó bộ chuẩn hóa của $h_{(K_1)}$ trong $g_{(K_1)}$ là $n_{(K_1)}$.

Cho K, $K_1$, g, $\rho$, M như trong đoạn trước. Cho b là một không gian con vectơ của g và W là một không gian con vectơ của M. Gọi V là không gian con vectơ của M gồm các $m \in M$ sao cho $\rho(b) \cdot m \subset W$. Gọi V' là không gian con vectơ của $M_{(K_1)}$ gồm các $m' \in M_{(K_1)}$ sao cho $\rho_{(K_1)}(b_{(K_1)}) \cdot m' \subset W_{(K_1)}$. Như trên ta thấy rằng $V' = V_{(K_1)}$. Đặc biệt, không gian con vectơ các *phần tử bất biến* của $M_{(K_1)}$ được dẫn xuất từ không gian con vectơ các phần tử bất biến của M bằng cách mở rộng trường cơ sở từ $K$ thành $K_1$.

Cho $K, K_1$ và $\phi$ như ở đầu số này. Cho $g$ là một đại số Lie $K$ và M và N là các g-môđun. Nếu M và N là các g-môđun đẳng cấu, thì $M_{(K_1)}$ và $N_{(K_1)}$ là các $g_{(K_1)}$-môđun đẳng cấu. Ngược lại:

#### Mệnh đề 13 {#lie-i-s3-prop-13 .statement}

*Cho $K$ là một trường, $K_1$ là một mở rộng của $K$, $g$ là một đại số Lie trên $K$ và $M, N$ là hai $g$-môđun có số chiều hữu hạn trên $K$. Nếu $M_{(K_1)}$ và $N_{(K_1)}$ là các $g_{(K_1)}$-môđun đẳng cấu, thì $M$ và $N$ là các $g$-môđun đẳng cấu.*

Chứng minh gồm hai bước.

(1) Trước hết giả sử rằng $K_1$ là một mở rộng của $K$ có *bậc hữu hạn* $n$. Gọi $U$ là đại số bao quanh của $g$, sao cho đại số bao quanh của $g_{(K_1)}$ là $U_{(K_1)} = U \otimes_K K_1$ (§ 2, no. 9). Vì $M_{(K_1)}$ và $N_{(K_1)}$ đẳng cấu như các $U_{(K_1)}$-môđun nên chúng *a fortiori* đẳng cấu như các $U$-môđun; nhưng như các $U$-môđun chúng lần lượt đẳng cấu với $M^n$ và $N^n$. Bây giờ $M$ và $N$ là các $U$-môđun có độ dài hữu hạn; do đó $M$ (tương ứng $N$) là tổng trực tiếp của một họ $(P_i^{r_i})_{1 \leq i \leq p}$ (tương ứng $(Q_j^{s_j})_{1 \leq j \leq q}$) các môđun con sao cho các $P_i$ (tương ứng $Q_j$) là không phân tích được và hai $P_i$ (tương ứng $Q_j$) có các chỉ số khác nhau thì không đẳng cấu (*Đại số*, Chương VIII, § 2, no. 2, Định lý 1). Khi đó $M^n$ (tương ứng $N^n$) đẳng cấu với tổng trực tiếp của các $P_i^{n r_i}$ (tương ứng $Q_j^{n s_j}$); suy ra (*loc. cit.*) rằng $p = q$ và rằng sau khi hoán vị các $Q_j$ nếu cần thiết thì $n r_i = n s_i$ và $P_i$ đẳng cấu với $Q_i$ với $1 \leq i \leq p$, do đó $M$ đẳng cấu với $N$.

(2) *Trường hợp tổng quát.* Cho $P$ là $g$-môđun $\mathcal{L}_K(M, N)$ và $Q$ là không gian con các bất biến của $P$, nghĩa là tập hợp các đồng cấu của $g$-môđun $M$ vào $g$-môđun $N$. Trong $g_{(K_1)}$-môđun $\mathcal{L}_{K_1}(M_{(K_1)}, N_{(K_1)}) = (\mathcal{L}_K(M, N))_{(K_1)}$, không gian con các bất biến là $Q_{(K_1)}$. Giả thiết rằng $M_{(K_1)}$ và $N_{(K_1)}$ đẳng cấu suy ra rằng $M$ và $N$ có cùng chiều trên $K$ và rằng tồn tại trong $Q_{(K_1)}$ một phần tử $g$ là một đẳng cấu của $M_{(K_1)}$ lên $N_{(K_1)}$. Cho $(f_1, \ldots, f_d)$ là một cơ sở của $Q$ trên $K$ và chọn các cơ sở của $M$ và $N$ trên $K$. Nếu $\lambda_k \in K_1$ cho $1 \leq k \leq d$, ma trận của $f = \sum_{k=1}^d \lambda_k f_k$ đối với các cơ sở này có định thức là một đa thức $D(\lambda_1, \ldots, \lambda_d)$ với các hệ số *trong* $K$. Khi $f = g$, định thức này khác không và do đó các hệ số của $D$ không phải tất cả đều khác không. Vì vậy, nếu $\Omega$ là bao đóng đại số của $K$, tồn tại (vì $\Omega$ là vô hạn) các phần tử $\mu_k \in \Omega$ $(1 \leq k \leq d)$ sao cho $D(\mu_1, \ldots, \mu_d) \neq 0$ (*Algebra*, Chương IV, § 2, no. 5, Mệnh đề 8). Nếu $K_2$ là mở rộng đại số của $K$ sinh bởi các $\mu_k$ $(1 \leq k \leq d)$, thì suy ra rằng $\sum_{k=1}^d \mu_k f_k$ là một đẳng cấu của $M_{(K_2)}$ lên $N_{(K_2)}$; nhưng $K_2$ có bậc hữu hạn trên $K$ (*Algebra*, Chương V, § 3, no. 2, Mệnh đề 5) và do đó $M$ và $N$ đẳng cấu theo phần thứ nhất của lập luận.

Lại cho $K, K_1$ và $\phi$ như ở đầu số này. Cho $\rho$ là một biểu diễn của $g$ trên một $K$-môđun $M$ với một cơ sở hữu hạn $(x_1, \ldots, x_n)$. Khi đó dạng song tuyến tính trên $g_{(K_1)}$ liên kết với $\rho_{(K_1)}$ được dẫn xuất từ dạng song tuyến tính liên kết với $\rho$ bằng cách mở rộng vành cơ sở đến $K_1$ (vì, nếu $u \in \mathcal{L}_K(M)$, $u$ có cùng ma trận đối với $(x_1, \ldots, x_n)$ như $u \otimes 1$ đối với $(x_1 \otimes 1, \ldots, x_n \otimes 1)$ và do đó $u$ và $u \otimes 1$ có cùng vết). Đặc biệt, nếu $K$-môđun $g$ có một cơ sở hữu hạn, dạng *Killing* của $g_{(K_1)}$ được dẫn xuất từ dạng đó của $g$ bằng cách mở rộng vành cơ sở đến $K_1$.

### Bài tập {#lie-i-s3-exercises}

Xem các [bài tập cho § 3](exercises/s3/).
