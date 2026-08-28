---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 5
section_title: Tensor algebra. Tensors
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0508-0521, 0651-0656
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE TENSOR ALGEBRA OF A MODULE
      page: 0
      pdf_page: 508
    - "no": 2
      title: FUNCTORIAL PROPERTIES OF THE TENSOR ALGEBRA
      page: 0
      pdf_page: 509
    - "no": 3
      title: EXTENSION OF THE RING OF SCALARS
      page: 0
      pdf_page: 513
    - "no": 4
      title: DIRECT LIMIT OF TENSOR ALGEBRAS
      page: 0
      pdf_page: 514
    - "no": 5
      title: TENSOR ALGEBRA OF A DIRECT SUM. TENSOR ALGEBRA OF A FREE MODULE. TENSOR ALGEBRA OF A GRADED MODULE
      page: 0
      pdf_page: 515
    - "no": 6
      title: TENSORS AND TENSOR NOTATION
      page: 0
      pdf_page: 516
statements: 15
exercises: 10
content_sha256: 9de4ee0dff93501fd053dfe01f312de17bfa63fd353f5393edce6a200b04c800
translated_from: content/en/alg/III/05_s5_tensor_algebra_tensors.md
source_content_sha256: 5e694bf63163c343522e25ec2e20029f6421afbfdb882680198af253edaeb7bc
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-1c09c3b9
glossary_version: 34
glossary_terms_sha256: e1d6704ad08196cbb47a913141f40b0c975675603c4a6c125b73ee5de00eec96
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. ĐẠI SỐ TENXƠ, TENXƠ

### 1. ĐỊNH NGHĨA ĐẠI SỐ TENXƠ CỦA MỘT MÔĐUN

Cho A là một vành giao hoán và M là một A-môđun. Với mỗi số nguyên $n \geqslant 0$, A-môđun là tích tenxơ của $n$ môđun bằng M (còn gọi là *lũy thừa tenxơ thứ $n$* của M) được ký hiệu là $\bigotimes^n M$, hoặc $M^{\otimes n}$, hoặc $T^n(M)$, hoặc $T^n_A(M)$, hoặc $\mathrm{Tens}^n(M)$; khi đó $T^1(M) = M$; ngoài ra ta viết $T^0(M) = A$. A-môđun là *tổng trực tiếp* $\bigoplus_{n \geqslant 0} T^n(M)$ được ký hiệu là $T(M)$ hoặc $\mathrm{Tens}(M)$. Ta sẽ định nghĩa trên $T(M)$ một cấu trúc đại số A phân bậc kiểu $\mathbf{N}$, bằng cách định nghĩa, với mỗi cặp có thứ tự gồm các số nguyên $p \geqslant 0$, $q \geqslant 0$, một ánh xạ A-tuyến tính
$$
m_{pq} : T^p(M) \otimes_A T^q(M) \to T^{p+q}(M)
$$
($\S 3$, no. 1, *Nhận xét*). Với $p > 0$ và $q > 0$, $m_{pq}$ là đẳng cấu tính kết hợp (II, $\S 3$, no. 9) và, khi $p = 0$ (tương ứng $q = 0$), $m_{0,q}$ là đẳng cấu chính tắc của $A \otimes_A T^q(M)$ lên $T^q(M)$ (tương ứng $m_{p,0}$ là đẳng cấu chính tắc của $T^p(M) \otimes_A A$ lên $T^p(M)$ (II, $\S 3$, no. 4, Mệnh đề 4)). Khi đó, với $x_i \in M$, $\alpha \in A$,
$$
\begin{align}
(x_1 \otimes \cdots \otimes x_p) \cdot (x_{p+1} \otimes \cdots \otimes x_{p+q}) &= x_1 \otimes \cdots \otimes x_p \otimes x_{p+1} \otimes \cdots \otimes x_{p+q} \\
\alpha \cdot (x_1 \otimes \cdots \otimes x_p) &= \alpha(x_1 \otimes \cdots \otimes x_p).
\end{align}
$$
Ngay lập tức thấy rằng phép nhân được định nghĩa như vậy trên $T(M)$ là *kết hợp* và có phần tử đơn vị là phần tử đơn vị 1 của $A = T^0(M)$.

#### Định nghĩa 1 {#alg-iii-s5-def-1 .statement}

Với mọi môđun $M$ trên một vành giao hoán $A$, đại số tenxơ của $M$, ký hiệu là $T(M)$, hoặc $\mathrm{Tens}(M)$, hoặc $T_A(M)$, là đại số $\bigoplus_{n \geq 0} T^n(M)$ với phép nhân được định nghĩa trong (1). Đơn ánh chính tắc $\phi : T^1(M) \to T(M)$ (II, § 1, no. 12) (cũng được ký hiệu là $\phi_M$) được gọi là đơn ánh chính tắc của $M$ vào $T(M)$.

#### Mệnh đề 1 {#alg-iii-s5-prop-1 .statement}

Cho $E$ là một đại số $A$ (có đơn vị) và $f : M \to E$ là một ánh xạ A-tuyến tính. Tồn tại duy nhất một đồng cấu đại số A $g : T(M) \to E$ sao cho $f = g \circ \phi$.

Nói cách khác, $(T(M), \phi)$ là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1), trong đó $\Sigma$ là loài của cấu trúc $A$-đại số, các ánh xạ $\alpha$ là các ánh xạ $A$-tuyến tính từ môđun $M$ vào một $A$-đại số. Chú ý rằng ở đây không có vấn đề về một phép phân bậc trên $T(M)$.

Đối với mọi họ hữu hạn $(x_i)_{1 \leq i \leq n}$ gồm $n$ phần tử của $M$, theo định nghĩa của tích trong $T(M)$, $x_1 \otimes x_2 \otimes \cdots \otimes x_n = \phi(x_1)\phi(x_2)\ldots\phi(x_n)$; khi đó tất yếu $g(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = f(x_1)f(x_2)\ldots f(x_n)$ với $n \geq 1$ và $g(\alpha) = \alpha e$ (nếu $e$ là phần tử đơn vị của $E$) với $\alpha \in A$, điều này chứng minh tính duy nhất của $g$. Ngược lại, chú ý rằng, với mọi $n > 0$, ánh xạ
$$
(x_1, \ldots, x_n) \mapsto f(x_1)f(x_2)\ldots f(x_n)
$$
từ $M^n$ vào $E$ là $A$-đa tuyến tính; do đó tương ứng với nó là một ánh xạ $A$-tuyến tính $g_n : T^n(M) \to E$ sao cho
$$
g(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = f(x_1)f(x_2)\ldots f(x_n).
$$
Ta cũng định nghĩa ánh xạ $g_0 : T^0(M) \to E$ bằng $\eta_E$ ($\S 1$, no. 3), nói cách khác $g_0(\alpha) = \alpha e$ với $\alpha \in A$. Gọi $g$ là ánh xạ $A$-tuyến tính duy nhất từ $T(M)$ vào $E$ mà hạn chế của nó lên $T^n(M)$ là $g_n$ ($n \geq 0$); ngay lập tức ta có $g \circ \phi = g_1 = f$ và còn phải kiểm tra rằng $g$ là một đồng cấu $A$-đại số. Theo phép dựng $g(1) = e$ và chỉ cần, nhờ tính tuyến tính, chứng minh rằng $g(uv) = g(u)g(v)$ với $u \in T^p(M)$ và $v \in T^q(M)$ ($p > 0, q > 0$); bây giờ từ các công thức (1) và (2) suy ra rằng quan hệ này đúng khi $u = x_1 \otimes x_2 \otimes \cdots \otimes x_p$ và $v \in x_{p+1} \otimes \cdots \otimes x_{p+q}$ (trong đó các $x_i$ thuộc $E$). Do đó nó đúng với $u \in T^p(M)$ và $v \in T^q(M)$ nhờ tính tuyến tính.

#### Nhận xét {#alg-iii-s5-n1-rem-1 .statement}

Giả sử $E$ là một đại số trên $A$ phân bậc kiểu $\mathbf{Z}$, với phép phân bậc $(E_n)$, và cũng giả sử rằng
$$
f(M) \subset E_1.
$$
Khi đó từ (2) suy ra $g(T^p(M)) \subset E_p$ với mọi $p \geq 0$ và do đó $g$ là một đồng cấu đại số phân bậc.

### 2. CÁC TÍNH CHẤT HÀM TỬ CỦA ĐẠI SỐ TENXƠ

#### Mệnh đề 2 {#alg-iii-s5-prop-2 .statement}

Cho $A$ là một vành giao hoán, $M$ và $N$ là hai A-môđun và
$$
u : M \to N
$$

là một ánh xạ A-tuyến tính. Tồn tại một và chỉ một đồng cấu đại số trên A

$$
u': \mathbf{T}(M) \to \mathbf{T}(N)
$$

sao cho biểu đồ

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi_M & & \downarrow \phi_N \\
\mathbf{T}(M) & \xrightarrow{u'} & \mathbf{T}(N)
\end{array}
$$

giao hoán. Hơn nữa, $u'$ là một đồng cấu đại số phân bậc.

Sự tồn tại và tính duy nhất của $u'$ suy ra từ no. 1, Mệnh đề 1, áp dụng cho đại số $\mathbf{T}(N)$ và ánh xạ tuyến tính $\phi_N \circ u : M \to \mathbf{T}(N)$; vì

$$
u(M) \subset \mathbf{T}^1(N) = N,
$$

nên việc $u'$ là một đồng cấu đại số phân bậc suy ra từ Nhận xét của no. 1.

Đồng cấu $u'$ của Mệnh đề 2 từ nay về sau được ký hiệu là $\mathbf{T}(u)$. Nếu P là một A-môđun và $v : N \to P$ là một ánh xạ A-tuyến tính, thì

$$
\mathbf{T}(v \circ u) = \mathbf{T}(v) \circ \mathbf{T}(u)
$$

vì $\mathbf{T}(v) \circ \mathbf{T}(u)$ là một đồng cấu đại số làm cho biểu đồ

$$
\begin{array}{ccc}
M & \xrightarrow{v \circ u} & P \\
\downarrow \phi_M & & \downarrow \phi_P \\
\mathbf{T}(M) & \xrightarrow{\mathbf{T}(v) \circ \mathbf{T}(u)} & \mathbf{T}(P)
\end{array}
$$

giao hoán.

$\mathbf{T}(u)$ đôi khi được gọi là mở rộng chính tắc của $u$ lên $\mathbf{T}(M)$ (chứa $M = \mathbf{T}^1(M)$). Chú ý rằng hạn chế $\mathbf{T}^n(u) : \mathbf{T}^n(M) \to \mathbf{T}^n(N)$ chỉ là ánh xạ tuyến tính $u^{\otimes n} = u \otimes u \otimes \cdots \otimes u$ (n lần), vì

$$
\mathbf{T}^n(u)(x_1 \otimes \cdots \otimes x_n) = u(x_1) \otimes \cdots \otimes u(x_n)
$$

do $\mathbf{T}(u)$ là một đồng cấu đại số và $\mathbf{T}^1(u) = u$; hạn chế $\mathbf{T}^0(u)$ lên A là ánh xạ đồng nhất. $\mathbf{T}^n(u)$ được gọi là lũy thừa tenxơ thứ $n$ của $u$.

#### Mệnh đề 3 {#alg-iii-s5-prop-3 .statement}

*Nếu $u : M \to N$ là một ánh xạ A-tuyến tính toàn ánh, đồng cấu $\mathbf{T}(u) : \mathbf{T}(M) \to \mathbf{T}(N)$ là toàn ánh và hạt nhân của nó là iđêan hai phía của $\mathbf{T}(M)$ sinh bởi hạt nhân $P \subset M \subset \mathbf{T}(M)$ của $u$.*

$\mathbf{T}^0(u) : \mathbf{T}^0(M) \to \mathbf{T}^0(N)$ là song ánh và với mọi số nguyên $n > 0$,

$$
\mathbf{T}^n(u) : \mathbf{T}^n(M) \to \mathbf{T}^n(N)
$$

là toàn ánh, như thấy được bằng quy nạp theo $n$ sử dụng II, § 3, no. 6, Mệnh đề 6; mệnh đề sau cũng cho thấy, bằng quy nạp theo $n$, rằng hạt nhân $\mathfrak{I}_n$ của $T^n(u)$ là môđun con của $T^n(M)$ sinh bởi các tích
$$
x_1 \otimes x_2 \otimes \cdots \otimes x_n
$$
trong đó ít nhất một trong các $x_i$ thuộc $P$. Điều này cho thấy hạt nhân $\mathfrak{I} = \bigoplus_{n \geq 1} \mathfrak{I}_n$ của $T(u)$ là iđêan hai phía sinh bởi $P$ trong $T(M)$.

Nếu $u : M \to N$ là một ánh xạ tuyến tính *đơn ánh*, thì không phải lúc nào cũng đúng rằng $T(u)$ là một ánh xạ đơn ánh (Bài tập 1). Tuy nhiên, điều này đúng khi $u$ là một đơn ánh sao cho $u(M)$ là một *nhân tử trực tiếp* của $N$, vì khi đó tồn tại một ánh xạ tuyến tính $v : N \to M$ sao cho $v \circ u$ là ánh xạ đồng nhất trên $M$ và do đó
$$
T(v \circ u) = T(v) \circ T(u)
$$
là ánh xạ đồng nhất trên $T(M)$, suy ra $T(u)$ là đơn ánh và ảnh của nó (đẳng cấu với $T(M)$) là một *nhân tử trực tiếp* của $T(N)$ (II, § 1, no. 9, Mệnh đề 15). Chính xác hơn:

#### Mệnh đề 4 {#alg-iii-s5-prop-4 .statement}

*Cho $N$ và $P$ là hai môđun con của một môđun $A$-môđun $M$ sao cho tổng của chúng $N + P$ là một nhân tử trực tiếp trong $M$ và giao của chúng $N \cap P$ là một nhân tử trực tiếp trong $N$ và trong $P$. Khi đó các đồng cấu $T(N) \to T(M)$, $T(P) \to T(M)$ và*
$$
T(N \cap P) \to T(M),
$$
*là các mở rộng chính tắc của các đơn ánh chính tắc, đều là đơn ánh; nếu $T(N)$, $T(P)$ và $T(N \cap P)$ được đồng nhất với các đại số con của $T(M)$ bằng các đồng cấu này, thì*
(5)
$$
T(N \cap P) = T(N) \cap T(P).
$$

Theo giả thiết, tồn tại các môđun con $N' \subset N$ và $P' \subset P$ sao cho $N = N' \oplus (N \cap P)$, $P = P' \oplus (N \cap P)$; khi đó
$$
N + P = N' \oplus P' \oplus (N \cap P)
$$
và theo giả thiết tồn tại một môđun con $M'$ của $M$ sao cho
$$
M = M' \oplus (N + P) = M' \oplus N' \oplus P' \oplus (N \cap P) \\
= M' \oplus P' \oplus N = M' \oplus N' \oplus P.
$$

Đặc biệt, $N + P$, $N$, $P$ và $N \cap P$ là các nhân tử trực tiếp trong $M$, điều này kéo theo, như đã thấy ở trên, rằng các đồng cấu chính tắc
$$
T(N + P) \to T(M), \quad T(N) \to T(M),
$$
$$
T(P) \to T(M), \quad T(N \cap P) \to T(M)
$$
là đơn ánh. Ba đại số $T(N)$, $T(P)$ và $T(N \cap P)$ do đó được đồng nhất với các đại số con của $T(N + P)$ và đại số sau lại được đồng nhất với một đại số con của $T(M)$;

viết $Q = N \cap P$, còn phải chứng minh rằng, nếu $T(Q)$, $T(N' \oplus Q)$ và $T(P' \oplus Q)$ được đồng nhất với các đại số con của $T(N' \oplus P' \oplus Q)$, thì

$$
T(N' \oplus Q) \cap T(P' \oplus Q) = T(Q).
$$

Bây giờ, xét biểu đồ giao hoán

$$
\begin{array}{ccc}
N' \oplus Q & \longrightarrow & N' \oplus P' \oplus Q \\
\downarrow & & \downarrow \\
Q & \longrightarrow & P' \oplus Q
\end{array}
$$

trong đó các mũi tên ngang là các đơn ánh chính tắc và các mũi tên đứng là các phép chiếu chính tắc. Ta suy ra một biểu đồ giao hoán

$$
\begin{array}{ccc}
T(N' \oplus Q) & \overset{u}{\longrightarrow} & T(N' \oplus P' \oplus Q) \\
\downarrow r & & \downarrow s \\
T(Q) & \overset{v}{\longrightarrow} & T(P' \oplus Q)
\end{array}
$$

trong đó $r$ và $s$ là các đồng cấu toàn ánh (Mệnh đề 3) và $u$ và $v$ là các đồng cấu đơn ánh. Do đó, để chứng minh (6), chú ý rằng vế phải hiển nhiên được chứa trong vế trái; vì vậy chỉ cần kiểm tra rằng nếu

$$
x \in T(N' \oplus Q) \cap T(P' \oplus Q),
$$

thì $x \in T(Q)$. Bây giờ định nghĩa của đồng cấu $s$ cho thấy rằng hạn chế của nó lên $T(P' \oplus Q)$ (được đồng nhất với một đại số con của $T(N' \oplus P' \oplus Q)$) là ánh xạ đồng nhất; giả thiết về $x$ do đó suy ra rằng $s(u(x)) = x$. Nhưng khi đó cũng có $v(r(x)) = x$, nói cách khác $x$ thuộc ảnh của $T(Q)$ trong $T(P' \oplus Q)$, điều cần phải chứng minh.

#### Nhận xét {#alg-iii-s5-n2-rem-1 .statement}

Đặc biệt lưu ý rằng các giả thiết của Mệnh đề 4 luôn đúng đối với các môđun con tùy ý $N, P$ của $M$ khi $A$ là một trường (II, § 7, no. 3, Mệnh đề 4). Hơn nữa, nếu $N \subset P$ và $N \neq P$, thì $T^n(N) \neq T^n(P)$ với mọi $n \geq 1$, vì nếu $R$ là một phần bù của $P$ trong $N$, thì $T^n(P) \cap T^n(R) = \{0\}$ theo (4) và $T^n(R) \neq \{0\}$.

#### Hệ quả {#alg-iii-s5-n2-cor-1 .statement}

*Cho $K$ là một trường giao hoán và $M$ là một không gian vectơ trên $K$. Với mọi phần tử $z \in T(M)$, tồn tại một không gian vectơ $N$ nhỏ nhất của $M$ sao cho $z \in T(N)$ và $N$ có hạng hữu hạn trên $K$.*

Trong mệnh đề này, ta hiểu rằng đối với mọi không gian con vectơ $P$ của $M$, $T(P)$ được đồng nhất một cách chính tắc với một đại số con của $T(M)$. Cho $z \in T(M)$; $z$ có thể được biểu diễn thành một tổ hợp tuyến tính của các phần tử mà mỗi phần tử trong đó là một tích hữu hạn của các phần tử của $M = T^1(M)$; tất cả các phần tử của $M$ xuất hiện trong các tích này sinh ra một không gian con vectơ $Q$ có hạng hữu hạn và $z \in T(Q)$.

Gọi $\mathcal{F}$ là tập hợp (không rỗng) các không gian con vectơ $P$ có hạng hữu hạn sao cho $z \in T(P)$. Mọi dãy giảm các phần tử của $\mathcal{F}$ đều dừng, vì chúng là các không gian vectơ có hạng hữu hạn. Do đó $\mathcal{F}$ có một phần tử cực tiểu $N$ (Lý thuyết tập hợp, III, § 6, no. 5). Còn lại là kiểm tra rằng mọi $P \in \mathcal{F}$ đều chứa $N$; bây giờ, $z \in T(P) \cap T(N) = T(P \cap N)$ (Mệnh đề 4); theo định nghĩa của $N$, điều này suy ra $N \cap P = N$, nghĩa là $P \supset N$.

Không gian con $N$ của $M$ được gọi là *liên kết* với $z$.

### 3. MỞ RỘNG VÀNH CÁC VÔ HƯỚNG

Cho $A, A'$ là hai vành giao hoán và $\rho : A \to A'$ là một đồng cấu vành. Cho $M$ là một $A$-môđun, $M'$ là một $A'$-môđun và $u : M \to M'$ là một $A$-đồng cấu; vì đơn ánh chính tắc $\phi_{M'} : M' \to T_{A'}(M')$ cũng là một $A$-đồng cấu (bằng hạn chế các vô hướng), nên hợp thành $M \xrightarrow{u} M' \xrightarrow{\phi_{M'}} T_{A'}(M')$ cũng vậy. Một đồng cấu đại số trên A $T_A(M) \to \rho^*(T_{A'}(M'))$ được dẫn xuất (no. 2), còn được ký hiệu là $T(u) : T_A(M) \to T_{A'}(M')$, đó là $A$-đồng cấu duy nhất làm cho biểu đồ sau giao hoán

$$
\begin{array}{ccc}
M & \xrightarrow{u} & M' \\
\downarrow \phi_M & & \downarrow \phi_{M'} \\
T_A(M) & \xrightarrow{T(u)} & T_{A'}(M')
\end{array}
$$

Nếu $\sigma : A' \to A''$ là một đồng cấu vành giao hoán, $M''$ là một $A''$-môđun và $v : M' \to M''$ là một $A'$-đồng cấu, tính chất duy nhất ở trên cho thấy rằng

$$
T(v \circ u) = T(v) \circ T(u).
$$

#### Mệnh đề 5 {#alg-iii-s5-prop-5 .statement}

*Cho $A, B$ là hai vành giao hoán, $\rho : A \to B$ là một đồng cấu vành và $M$ là một $A$-môđun. Phần mở rộng chính tắc*

$$
\psi : T_B(B \otimes_A M) \to B \otimes_A T_A(M)
$$

*của ánh xạ B-tuyến tính* $l_B \otimes \phi_M : B \otimes_A M \to B \otimes_A T_A(M)$ *là một đẳng cấu của các đại số B phân bậc*.

Xét hai đồng cấu đại số trên A: đơn ánh chính tắc $j : B = T^0(B \otimes_A M) \to T(B \otimes_A M)$ và đồng cấu

$$
h = T(i) : T(M) \to T(B \otimes_A M)
$$

được dẫn xuất (xem công thức (8)) từ ánh xạ A-tuyến tính chính tắc

$$
i : M \to B \otimes_A M.
$$

Vì $T^0(B \otimes_A M)$ được chứa trong tâm của $T(B \otimes_A M)$, Mệnh đề 5 của § 4, no. 2 có thể được áp dụng và một đồng cấu đại số trên A

$$
\psi': B \otimes_A T(M) \to T(B \otimes_A M)
$$

được thu được sao cho, với $\beta \in B, x_i \in M$ cho $1 \leq i \leq n$,

$$
\psi'(\beta \otimes (x_1 \otimes x_2 \otimes \cdots \otimes x_n)) = \beta((1 \otimes x_1) \otimes (1 \otimes x_2) \otimes \cdots \otimes (1 \otimes x_n)),
$$

điều này cho thấy ngay lập tức rằng $\psi'$ cũng là một đồng cấu đại số trên B. Chỉ cần chứng minh rằng $\psi \circ \psi'$ và $\psi' \circ \psi$ lần lượt là các ánh xạ đồng nhất trên $B \otimes_A T(M)$ và $T(B \otimes_A M)$. Bây giờ, hai đại số này được sinh bởi $B \otimes_A M$ và rõ ràng $\psi \circ \psi'$ và $\psi' \circ \psi$ trùng với ánh xạ đồng nhất trên $B \otimes_A M$, do đó kết luận.

### 4. GIỚI HẠN TRỰC TIẾP CỦA CÁC ĐẠI SỐ TENXƠ

Cho $(A_\alpha, \phi_{\beta \alpha})$ là một hệ trực tiếp có hướng của các vành giao hoán và $(M_\alpha, f_{\beta \alpha})$ là một hệ trực tiếp của các $A_\alpha$-môđun (II, § 6, no. 2); đặt $A = \lim \rightarrow A_\alpha$ và $M = \lim \rightarrow M_\alpha$, là một $A$-môđun. Với $\alpha \leq \beta$, một đồng cấu đại số $A_\alpha$ (no. 3, công thức (8)) $f'_{\beta \alpha} = T(f_{\beta \alpha}): T_{A\alpha}(M_\alpha) \to T_{A\beta}(M_\beta)$ được dẫn xuất một cách chính tắc từ đồng cấu $A_\alpha$ $f_{\beta \alpha}: M_\alpha \to M_\beta$ và từ (9) (no. 3) suy ra rằng $(T_{A\alpha}(M_\alpha), f'_{\beta \alpha})$ là một *hệ trực tiếp của các đại số $A_\alpha$*. Mặt khác, đặt $f'_\alpha: M_\alpha \to M$ là đồng cấu $A_\alpha$ chính tắc; một đồng cấu đại số $A_\alpha$ $f'_\alpha: T_{A\alpha}(M_\alpha) \to T_A(M)$ được dẫn xuất (no. 3, công thức (8)) và cũng từ (9) (no. 3) suy ra rằng các $f'_\alpha$ tạo thành một hệ trực tiếp của các đồng cấu $A_\alpha$.

#### Mệnh đề 6 {#alg-iii-s5-prop-6 .statement}

*Đồng cấu $A$* $f' = \lim \rightarrow f'_\alpha : \lim \rightarrow T_{A\alpha}(M_\alpha) \to T_A(M)$ *là một đẳng cấu đại số phân bậc*.

Để đơn giản, ta viết $E = T_A(M)$ và $E' = \lim \rightarrow T_{A\alpha}(M_\alpha)$ và gọi

$$
g_\alpha: T_{A\alpha}(M_\alpha) \to E'
$$

là đồng cấu $A_\alpha$ chính tắc. Rõ ràng các ánh xạ tuyến tính $A_\alpha$ hợp thành $M_\alpha \xrightarrow{\phi_{M_\alpha}} T_{A\alpha}(M_\alpha) \xrightarrow{g_\alpha} E'$ tạo thành một hệ trực tiếp và do đó tồn tại duy nhất một ánh xạ $A$ tuyến tính $u = \lim \rightarrow (g_\alpha \circ \phi_{M_\alpha}): M \to E'$ sao cho

$$
u \circ f_\alpha = g_\alpha \circ \phi_{M_\alpha}
$$

với mọi $\alpha$. Ánh xạ này tự nó phân tích duy nhất (no. 1, Mệnh đề 1) thành $M \xrightarrow{\phi_M} E \to E'$, trong đó $h$ là một đồng cấu đại số $A$. Chỉ cần chứng minh rằng $h \circ f' = 1_{E'}$ và $f' \circ h = 1_E$.

Vì mục đích này, chú ý rằng, với mọi chỉ số $\alpha$, (no. 3, công thức (8))

$$
h \circ f'_\alpha \circ \phi_{M_\alpha} = h \circ \phi_M \circ f_\alpha = u \circ f_\alpha = g_\alpha \circ \phi_{M_\alpha}
$$

do đó, theo tính duy nhất của mệnh đề trong no. 1, Mệnh đề 1,

$$
h \circ f'_\alpha = g_\alpha
$$

với mọi $\alpha$; suy ra $(h \circ f') \circ g_\alpha = g_\alpha$ với mọi $\alpha$ và do đó $h \circ f' = 1_{E'}$ theo định nghĩa của giới hạn trực tiếp.

Mặt khác, theo no. 3, công thức (8),

$$
f' \circ u \circ f_\alpha = f' \circ g_\alpha \circ \phi_{M_\alpha} = f'_\alpha \circ \phi_{M_\alpha} = \phi_M \circ f_\alpha,
$$

do đó lại theo định nghĩa của giới hạn trực tiếp, $f' \circ u = \phi_M$; ta kết luận rằng $f' \circ h \circ \phi_M = \phi_M$ và tính duy nhất của no. 1, Mệnh đề 1 cho $f' \circ h = 1_E$.

Mệnh đề 6 cũng có thể được chứng minh bằng cách nhận thấy rằng, với mọi số nguyên $n \geq 1$, tồn tại một đẳng cấu $A$-môđun chính tắc $\lim \rightarrow T^n_{A_\alpha}(M_\alpha) \to T^n_A(M)$, suy ra bằng quy nạp theo $n$ từ II, § 6, no. 3, Mệnh đề 7. Ngay lập tức kiểm tra được rằng các đẳng cấu này là các hạn chế của $f'$.

### 5. ĐẠI SỐ TENXƠ CỦA MỘT TỔNG TRỰC TIẾP. ĐẠI SỐ TENXƠ CỦA MỘT MÔĐUN TỰ DO. ĐẠI SỐ TENXƠ CỦA MỘT MÔĐUN PHÂN BẬC

Cho $A$ là một vành giao hoán và $M = \bigoplus_{\lambda \in L} M_\lambda$ là tổng trực tiếp của một họ các $A$-môđun. Từ II, § 3, no. 7, Mệnh đề 7, bằng quy nạp theo $n$, suy ra rằng $T^n(M)$ là tổng trực tiếp của các môđun là ảnh của các đơn ánh chính tắc

$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n} \to T^n(M) = M^{\otimes n}
$$

ứng với *tất cả* các dãy $(\lambda_i) \in L^n$. Đồng nhất $M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n}$ với ảnh này, ta thấy rằng $T(M)$ là *tổng trực tiếp của tất cả các môđun*

$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n}
$$

trong đó $n$ chạy qua $\mathbf{N}$ và, với mỗi $n$, $(\lambda_i)$ chạy qua $L^n$.

Trước hết ta suy ra hệ quả sau:

#### Định lý 1 {#alg-iii-s5-thm-1 .statement}

*Cho $A$ là một vành giao hoán, $M$ là một môđun $A$ tự do và $(e_\lambda)_{\lambda \in L}$ là một cơ sở của $M$. Khi đó các phần tử $e_s = e_{\lambda_1} \otimes e_{\lambda_2} \otimes \cdots \otimes e_{\lambda_n}$, trong đó $s = (\lambda_1, \ldots, \lambda_n)$ chạy qua tập hợp tất cả các dãy hữu hạn các phần tử của $L$ và $e_\varnothing$ được dùng để chỉ phần tử đơn vị của $T(M)$, tạo thành một cơ sở của môđun $A$ $T(M)$.*

Các phần tử của cơ sở này hiển nhiên là thuần nhất và bảng phép nhân được cho bởi

$$
e_s e_t = e_{st}
$$

trong đó $st$ chỉ dãy các phần tử của $L$ nhận được bằng cách *ghép liền* các dãy $s$ và $t$ (I, § 7, no. 2).

Ta thấy rằng cơ sở $(e_s)$ của $T(M)$, với luật nhân (10), đẳng cấu một cách chính tắc với *nửa đơn tự do* của tập hợp $L$ (I, § 7, no. 2), đẳng cấu này được thu được bằng cách ánh xạ mỗi từ $s$ của nửa đơn này vào phần tử $e_s$. Suy ra (\S 2, no. 7) rằng *đại số tenxơ $T(M)$ của một môđun tự do $M$, với một cơ sở có tập hợp chỉ số $L$, đẳng cấu một cách chính tắc với đại số kết hợp tự do của $L$ trên $A$*. Đặc biệt (\S 2, no. 7, Mệnh đề 7), với mọi ánh xạ $f : L \to E$ từ $L$ vào một đại số $A$ $E$, tồn tại duy nhất một đồng cấu đại số $A$ $\bar{f} : T(M) \to E$ sao cho $\bar{f}(e_\lambda) = f(\lambda)$.

#### Nhận xét {#alg-iii-s5-n5-rem-1 .statement}

Các kết quả trên cũng có thể thu được như một hệ quả của các tính chất phổ quát của đại số kết hợp tự do của đại số tenxơ, bằng cách sử dụng II, § 3, no. 7, Hệ quả 2 của Mệnh đề 7.

#### Hệ quả {#alg-iii-s5-n5-cor-1 .statement}

*Nếu $M$ là một môđun $A$ xạ ảnh, thì $T(M)$ là một môđun $A$ xạ ảnh.*

$M$ là một nhân tử trực tiếp của một môđun $A$ tự do $N$ (II, § 2, no. 2, Mệnh đề 4) và do đó $T(M)$ là một nhân tử trực tiếp của $T(N)$ (no. 2); vì $T(N)$ là tự do (Định lý 1), điều này cho thấy rằng $T(M)$ là xạ ảnh (II, § 2, no. 2).

#### Mệnh đề 7 {#alg-iii-s5-prop-7 .statement}

*Cho $\Delta$ là một nửa nhóm giao hoán, $M$ là một $A$-môđun phân bậc kiểu $\Delta$ và $(M_\alpha)_{\alpha \in \Delta}$ là sự phân bậc của nó. Với mọi cặp có thứ tự $(\alpha, n) \in \Delta \times \mathbf{N}$, đặt $T^{\alpha, n}(M)$ là tổng (trực tiếp) của các môđun con $M_{\alpha_1} \otimes M_{\alpha_2} \otimes \cdots \otimes M_{\alpha_n}$ của $T^n(M)$ sao cho $\sum_{i=1}^n \alpha_i = \alpha$; khi đó $(T^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$ là sự phân bậc duy nhất kiểu $\Delta \times \mathbf{N}$ tương thích với cấu trúc đại số trên $T(M)$ và cảm sinh trên $M = T^1(M)$ sự phân bậc đã cho.*

Ở đầu số này đã thấy rằng $T(M)$ là tổng trực tiếp của các $T^{\alpha, n}(M)$ và ngay lập tức từ các định nghĩa suy ra rằng đây là một sự phân bậc tương thích với cấu trúc đại số. Nếu $({T'}^{\alpha, n})$ là một sự phân bậc khác kiểu $\Delta \times \mathbf{N}$ trên $T(M)$ tương thích với cấu trúc đại số và sao cho ${T'}^{\alpha, 1}(M) = {T'}^{\alpha, 1}$ với $\alpha \in \Delta$, thì ngay lập tức từ các định nghĩa suy ra rằng, với mọi $n \geq 1$ và mọi $\alpha \in \Delta$, $T^{\alpha, n}(M) \subset {T'}^{\alpha, n}$; nhưng vì $T(M)$ cũng là tổng trực tiếp của các $T^{\alpha, n}(M)$, điều này suy ra rằng ${T'}^{\alpha, n} = T^{\alpha, n}(M)$ (II, § 1, no. 8, *Nhận xét*).

### 6. TENXƠ VÀ KÝ HIỆU TENXƠ

Cho $A$ là một vành giao hoán, $M$ một $A$-môđun, $M^*$ là *đối ngẫu* của $M$ (II, § 2, no. 3) và $I$ và $J$ là hai tập hợp *rời nhau hữu hạn*; $A$-môđun $\bigotimes_{i \in I \cup J} E_i$, trong đó $E_i = M$ nếu $i \in I$, $E_i = M^*$ nếu $i \in J$, được ký hiệu là $T^I_J(M)$; các phần tử của $T^I_J(M)$ được gọi là *tenxơ kiểu* $(I, J)$ trên $M$. Chúng được gọi là *phản biến* nếu $J = \varnothing$, *đồng biến* nếu $I = \varnothing$ và *hỗn hợp* trong trường hợp còn lại.

Cho $I', I''$ là hai tập con của $I$ và $J', J''$ là hai tập con của $J$ sao cho $I' \cup I'' = I$,

$I' \cap I'' = \varnothing,\ J' \cup J'' = J,\ J' \cap J'' = \varnothing$; khi đó có một đẳng cấu kết hợp chính tắc (II, § 3, no. 9)

$$
T_J^I(M) \to T_{J'}^{I'}(M) \otimes_A T_{J''}^{I''}(M).
$$

Xét đại số tenxơ $T(M \oplus M^*)$, từ no. 5 suy ra rằng $T^n(M \oplus M^*)$ được đồng nhất một cách chính tắc với tổng trực tiếp của các $T_J^I(M)$ trong đó I chạy qua tập hợp các tập con của khoảng $\{1, n\}$ của $\mathbf{N}$ và $J$ là phần bù của I trong $\{1, n\}$.

Khi $I = \{1, p\}$ và $J = \{p + 1, p + q\}$ với các số nguyên $p \geq 0,\ q \geq 0$ (trong đó ta thay I (tương ứng J) bằng $\varnothing$ khi $p = 0$ (tương ứng $q = 0$)), A-môđun $T_J^I(M)$ cũng được ký hiệu là $T_q^p(M)$; do đó, theo định nghĩa, các A-môđun $T_0^n(M)$ và $T_n^0(M)$ lần lượt là các A-môđun $T^n(M)$ và $T^n(M^*)$. Khi I và J là các tập hữu hạn tùy ý có số phần tử lần lượt là $p = \mathrm{Card}(I)$ và $q = \mathrm{Card}(J)$, ta đặt trên mỗi tập một thứ tự toàn phần; khi đó tồn tại một song ánh tăng từ I (tương ứng J) lên $\{1, p\}$ (tương ứng $\{p + 1, p + q\}$) và do đó các song ánh này xác định một đẳng cấu

$$
T_J^I(M) \to T_q^p(M).
$$

Khi M là một A-môđun *xạ ảnh sinh hữu hạn*, theo II, § 2, no. 7, Hệ quả 4 của Mệnh đề 13 và II, § 4, no. 4, Hệ quả 1 của Mệnh đề 4, tồn tại một đẳng cấu chính tắc

$$
(T_J^I(M))^* \to T_I^J(M).
$$

Bây giờ giả sử M là một A-môđun *tự do sinh hữu hạn* và $(e_\lambda)_{\lambda \in L}$ là một cơ sở của M (do đó L là một tập *hữu hạn*). Cơ sở của $M^*$ *đối ngẫu* với $(e_\lambda)$ (II, § 2, no. 6) được ký hiệu là $(e^\lambda)_{\lambda \in L}$. Các cơ sở $(e_\lambda)$ và $(e^\lambda)$ của M và $M^*$ tương ứng xác định (no. 5) một cơ sở của $T_J^I(M)$, mà ta mô tả *tường minh* như sau: cho hai ánh xạ $f : I \to L$ và $g : J \to L$, đặt $e_f^g$ là phần tử $\bigotimes_{i \in I \cup J} x_i$ của $T_J^I(M)$ được xác định bởi

$$
x_i = e_{f(i)} \quad \text{nếu } i \in I, \qquad x_i = e_{g(i)} \quad \text{nếu } i \in J.
$$

Khi $(f, g)$ chạy qua tập hợp các cặp ánh xạ có thứ tự $f : I \to L$ và $g : J \to L$, các $e_f^g$ lập thành một *cơ sở* của A-môđun $T_J^I(M)$, được gọi là *liên kết* với cơ sở $(e_\lambda)$ đã cho của M. Do đó, với $z \in T_J^I(M)$, ta có thể viết

$$
z = \sum_{(f, g)} \alpha_g^f(z) \cdot e_f^g
$$

trong đó $\alpha_g^f$ là các dạng tọa độ tương đối với cơ sở $(e_f^g)$; do lạm dụng ngôn ngữ, các $\alpha_g^f(z)$ được gọi là các tọa độ của tenxơ $z$ *đối với cơ sở* $(e_\lambda)$ của môđun M. Các $\alpha_g^f$ tạo thành cơ sở đối ngẫu của $(e_f^g)$, nói cách khác chúng được đồng nhất với các phần tử của cơ sở của $T_I^J(M)$, *liên kết* với $(e_\lambda)$. Khi I và J là các tập con bù nhau của một khoảng $\{1, n\}$ của $\mathbf{N}$, $\alpha_g^f$ (hoặc $\alpha_g^f(z)$) được ký hiệu như sau: mỗi phần tử $f(i)$ với $i \in I$ được viết như một chỉ số trên ở vị trí thứ i với một dấu chấm ở vị trí thứ i đối với $i \in J$; tương tự, $g(i)$ với $i \in J$ được viết như một chỉ số dưới ở vị trí thứ i với một dấu chấm ở vị trí thứ i đối với $i \in I$. Ví dụ, với $I = \{1, 4\}, J = \{2, 3\}$, ta viết $\alpha_{v\rho}^{\lambda\cdot\cdot\mu}$: nếu $f(1) = \lambda, f(4) = \mu, g(2) = \nu, g(3) = \rho$.

Cho $(\tilde{e}_{\lambda})_{\lambda \in L}$ là một cơ sở khác của M và P là ma trận của phép chuyển từ $(e_{\lambda})$ sang $(\tilde{e}_{\lambda})$ (II, § 10, no. 8). Khi đó ma trận của phép chuyển từ $(e^{\lambda})$ sang $(\tilde{e}^{\lambda})$ (cơ sở đối ngẫu của $(\tilde{e}_{\lambda})$) là ma trận đối nghịch $^tP^{-1}$ của P (II, § 10, no. 8, Mệnh đề 5). Suy ra (II, § 10, no. 10) rằng ma trận của phép chuyển từ cơ sở $(e^{g}_{f})$ của $T^{I}_{J}(M)$ sang cơ sở $(\tilde{e}^{g}_{f})$ (trong đó $f$ (tương ứng $g$) chạy qua tập hợp các ánh xạ của I vào L (tương ứng của J vào L)) là ma trận

$$
\bigotimes_{i \in I \cup J} Q_{i}, \quad \text{trong đó } Q_{i} = P \text{ nếu } i \in I, Q_{i} = {}^{t}P^{-1} \text{ nếu } i \in J.
$$

Ma trận chuyển vị của ma trận này do đó được đồng nhất với

$$
\bigotimes_{i \in I \cup J} R_{i}, \quad \text{trong đó } R_{i} = {}^{t}P^{-1} \text{ nếu } i \in I, R_{i} = P \text{ nếu } i \in J.
$$

Bây giờ giả sử M là một môđun tùy ý. Cho $i \in I, j \in J$ và đặt $I' = I - \{i\}, J' = J - \{j\}$; ta sẽ định nghĩa một ánh xạ A-tuyến tính chính tắc

$$
c^{i}_{j}: T^{I}_{J}(M) \to T^{I'}_{J'}(M),
$$

được gọi là phép co của chỉ số i và chỉ số j. Để làm điều này, chú ý rằng ánh xạ của $M^{I} \times (M^{*})^{J}$, ánh xạ này liên kết với mỗi họ $(x_{i})_{i \in I \cup J}$, trong đó $x_{i} \in M$ nếu $i \in I$ và $x_{i} \in M^{*}$ nếu $i \in J$, phần tử

$$
\langle x_{i}, x_{j} \rangle_{k \in (I \cup J) - \{i, j\}} x_{k}
$$

của $T^{I'}_{J'}(M)$, là A-đa tuyến tính; $c^{i}_{j}$ là ánh xạ A-tuyến tính tương ứng.

Bây giờ giả sử M là tự do và sinh hữu hạn và cho $(e_{\lambda})_{\lambda \in L}$ là một cơ sở của M. Với hai ánh xạ $f: I \to L, g: J \to L$, gọi $f_{i}$ là hạn chế của $f$ lên $I' = I - \{i\}$ và $g_{j}$ là hạn chế của $g$ lên $J' = J - \{j\}$; khi đó theo (12)

$$
c^{i}_{j}(e^{g}_{f}) = \begin{cases} 0 & \text{nếu } f(i) \neq g(j) \\ e^{g_{j}}_{f_{i}} & \text{nếu } f(i) = g(j) \end{cases}
$$

Đạt được biểu thức của các tọa độ của $c^{i}_{j}(z)$ theo các tọa độ của z; với mỗi ánh xạ $f'$ (tương ứng $g'$) của I' vào L (tương ứng của J' vào L) và mỗi $\lambda \in L$, ký hiệu $(f', \lambda)$ (tương ứng $(g', \lambda)$) là ánh xạ của I vào L (tương ứng của J vào L) mà hạn chế trên I' (tương ứng J') là $f'$ (tương ứng $g'$) và nhận giá trị $\lambda$ tại phần tử i (tương ứng j). Khi đó, nếu các dạng tọa độ đối với cơ sở $(e^{g'}_{f'})$ của $T^{I'}_{J'}(M)$ được ký hiệu là $\beta^{f'}_{g'}$,

$$
\beta^{f'}_{g'}(c^{i}_{j}(z)) = \sum_{\lambda \in L} \alpha^{(f'; \lambda)}_{(g'; \lambda)}(z).
$$

Các ví dụ về tenxơ. (1) Cho M là một A-môđun xạ ảnh sinh hữu hạn. Ta biết (II, § 4, no. 2, Hệ quả của Mệnh đề 2) rằng có một đẳng cấu A-môđun chính tắc

$$
\theta_M : M^* \otimes_A M \to \operatorname{End}_A(M)
$$

sao cho $\theta_M(x^* \otimes x)$ (với $x \in M, x^* \in M^*$) là tự đồng cấu

$$
y \mapsto \langle y, x^*\rangle x.
$$

Do đó, nhờ $\theta_M$, $T^{(2)}_{\{1\}}(M)$ (đẳng cấu với $T^1_1(M)$) có thể được đồng nhất với A-môđun $\operatorname{End}_A(M)$. Giả sử M là một môđun tự do và $(e_\lambda)_{\lambda \in L}$ là một cơ sở của M; khi đó các tọa độ của một tenxơ $z \in M^* \otimes M$ đối với cơ sở $(e^\mu \otimes e_\lambda)$ của môđun này được ký hiệu là $\zeta_{\mu \cdot \lambda}$. Vì $\theta_M(e^\mu \otimes e_\lambda)$ là tự đồng cấu $y \mapsto \langle y, e^\mu\rangle e_\lambda$, tự đồng cấu $u = \theta_M(z) = \theta_M\left( \sum_{\lambda, \mu} \zeta_{\mu \cdot \lambda} e^\mu \otimes e_\lambda \right)$ biến y thành $\sum_{\lambda, \mu} \zeta_{\mu \cdot \lambda} \langle y, e^\mu\rangle e_\lambda$; viết $y = e_\lambda$, ta thu được quan hệ

$$
u(e_\lambda) = \sum_{\mu \in L} \zeta_{\lambda \cdot \mu} e_\mu
$$

nói cách khác, *ma trận của ánh xạ tuyến tính* $u = \theta_M(z)$ *là ma trận mà phần tử ở hàng có chỉ số* $\mu$ *và cột có chỉ số* $\lambda$ *là* $\zeta_{\lambda \cdot \mu}$.

Định nghĩa của *vết* của u (II, § 4, no. 3) cho thấy ngay lập tức rằng

$$
\operatorname{Tr}(\theta_M(z)) = c_1^2(z).
$$

Do đó phần tử $z_0 = \sum_{\lambda \in L} e^\lambda \otimes e_\lambda$ (có các tọa độ $\zeta_{\mu \cdot \lambda}$ bằng không với $\lambda \neq \mu$ và bằng 1 với $\lambda = \mu$), sao cho $\theta_M(z_0) = 1_M$, là ảnh của phần tử $1 \in A = T^0_0(M)$ qua ánh xạ là *chuyển vị của phép co*

$$
c_1^2 : T^{(2)}_{\{1\}}(M) \to A.
$$

(2) Luôn giả sử rằng M là một A-môđun xạ ảnh sinh hữu hạn; có một đẳng cấu A-môđun chính tắc

$$
\mu : M^* \otimes_A M^* \to (M \otimes_A M)^*
$$

(II, § 4, no. 4, Hệ quả 1 của Mệnh đề 2) và một đẳng cấu chính tắc

$$
\theta : (M \otimes_A M)^* \otimes_A M \to \operatorname{Hom}_A(M \otimes_A M, M)
$$

(II, § 4, no. 2, Hệ quả của Mệnh đề 2); ngoài ra $\operatorname{Hom}_A(M \otimes_A M, M)$ đẳng cấu một cách chính tắc với A-môđun $\mathcal{L}_2(M, M; M)$ gồm các ánh xạ A-*song tuyến tính* của $M \times M$ vào M (II, § 3, no. 9). Hợp thành các đẳng cấu này cho ta một đẳng cấu chính tắc

$$
\chi_M : T^{(3)}_{\{1, 2\}}(M) = M^* \otimes M^* \otimes M \to \mathcal{L}_2(M, M; M)
$$

sao cho, với $x^*, y^*$ trong $M^*$, $z \in M$, $\chi_M(x^* \otimes y^* \otimes z)$ là ánh xạ song tuyến tính
$$
(u, v) \mapsto \langle u, x^*\rangle \langle v, y^*\rangle z.
$$
Do đó, thông qua $\chi_M$, $T_{\{1, 2\}}^{(3)}(M)$ (đẳng cấu với $T_2^1(M)$) có thể được đồng nhất với A-môđun $\mathcal{L}_2(M, M; M)$. Giả sử M là một A-môđun tự do và $(e_\lambda)_{\lambda \in L}$ là một cơ sở của M; khi đó các tọa độ của một tenxơ $z \in M^* \otimes M^* \otimes M$ đối với cơ sở $(e^\lambda \otimes e^\mu \otimes e_\nu)$ của môđun này được ký hiệu là $\zeta_{\lambda \mu \nu}$. Ánh xạ song tuyến tính $\chi_M(z)$ ánh xạ cặp có thứ tự $(e_\lambda, e_\mu)$ vào
$$
\sum_{\nu \in L} \zeta_{\lambda \mu \nu} e_\nu
$$
và do đó các $\zeta_{\lambda \mu \nu}$ chính là các *hằng số cấu trúc* của đại số (nói chung không kết hợp) xác định trên M bởi ánh xạ song tuyến tính $\chi_M(z)$, đối với cơ sở $(e_\lambda)$ (\S 1, no. 7).

#### Nhận xét 2 {#alg-iii-s5-n6-rem-2 .statement}

Cho $(e_\lambda)_{\lambda \in L}$, $(\bar{e}_\lambda)_{\lambda \in L}$ là hai cơ sở của M và P là ma trận chuyển từ $(e_\lambda)$ sang $(\bar{e}_\lambda)$. Theo những gì đã thấy trong *Ví dụ 1*, phần tử của P xuất hiện trong hàng có chỉ số $\lambda$ và cột có chỉ số $\mu$ được ký hiệu là $\alpha_\mu^\lambda$ và phần tử của ma trận đối liên hợp ${}^tP^{-1}$ xuất hiện trong hàng có chỉ số $\lambda$ và cột có chỉ số $\mu$ được ký hiệu là $\beta_\lambda^\mu$. Khi đó (theo ký hiệu đã đưa vào ở trên)
$$
\begin{cases}
\bar{e}_\mu = \sum_\lambda \alpha_\mu^\lambda e_\lambda \\
\bar{e}^\mu = \sum_\lambda \beta_\lambda^\mu e_\lambda
\end{cases}
$$
$$
\bar{e}_{f'}^{g'} = \sum_{(f', g)} \left( \prod_{i \in I} \alpha_{f'(i)}^{f(i)} \right) \left( \prod_{j \in J} \beta_{g(j)}^{g'(j)} \right) e_f^g
$$
với mọi ánh xạ $f': I \to L$ và $g': J \to L$. Do đó, các tọa độ $\zeta_g^f$ của tenxơ $z \in T_J^I(M)$ đối với cơ sở $(e_\lambda)$ có thể được biểu diễn theo các tọa độ $\bar{\zeta}_{g'}^{f'}$ của z đối với cơ sở $(\bar{e}_\lambda)$ bằng các công thức
$$
\zeta_g^f = \sum_{(f', g')} \left( \prod_{i \in I} \alpha_{g'(i)}^{g(i)} \right) \left( \prod_{j \in J} \beta_{f'(j)}^{f(j)} \right) \bar{\zeta}_{g'}^{f'}
$$
Ma trận $P^{-1}$ chuyển từ cơ sở $(\bar{e}_\lambda)$ sang cơ sở $(e_\lambda)$ là chuyển vị của ${}^tP^{-1}$, do đó $\beta_\lambda^\mu$ là phần tử xuất hiện trong cột có chỉ số $\lambda$ và hàng có chỉ số $\mu$ của $P^{-1}$. Vì vậy, phép tính $e_f^g$ theo các $\bar{e}_{f'}^{g'}$ và phép tính các $\bar{\zeta}_{g'}^{f'}$ theo các $\zeta_g^f$ được thực hiện bằng cách thay $\alpha_\mu^\lambda$ bởi $\beta_\lambda^\mu$ và $\beta_\lambda^\mu$ bởi $\alpha_\mu^\lambda$ trong các phép tính trên và đổi vai trò của $f$ và $f'$ cũng như của $g$ và $g'$. Khi đó
$$
e_f^g = \sum_{(f', g')} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f'(i)}^{f(i)} \right) \bar{e}_{f'}^{g'}
$$

(23)
$$
\bar{\zeta}_{g'}^{f'} = \sum_{(f,g)} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f(i)}^{f'(i)} \right) \zeta_g^f.
$$

Các công thức trên được lập sao cho phép tổng lấy trên các chỉ số xuất hiện một lần ở vị trí chỉ số dưới và một lần ở vị trí chỉ số trên. Một số tác giả, vì lý do này, cho phép mình bỏ các dấu tổng.
### Bài tập {#alg-iii-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
