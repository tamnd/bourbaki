---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 7
section_title: Exterior algebras
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0531-0546, 0657-0661
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE EXTERIOR ALGEBRA OF A MODULE
      page: 0
      pdf_page: 531
    - "no": 2
      title: Functorial properties of the exterior algebra
      page: 0
      pdf_page: 532
    - "no": 3
      title: ANTICOMMUTATIVITY OF THE EXTERIOR ALGEBRA
      page: 0
      pdf_page: 534
    - "no": 4
      title: '*n*-th EXTERIOR POWER OF A MODULE AND ALTERNATING MULTILINEAR MAPPINGS'
      page: 0
      pdf_page: 535
    - "no": 5
      title: EXTENSION OF THE RING OF SCALARS
      page: 0
      pdf_page: 537
    - "no": 6
      title: DIRECT LIMITS OF EXTERIOR ALGEBRAS
      page: 0
      pdf_page: 538
    - "no": 7
      title: EXTERIOR ALGEBRA OF A DIRECT SUM. EXTERIOR ALGEBRA OF A GRADED MODULE
      page: 0
      pdf_page: 539
    - "no": 8
      title: EXTERIOR ALGEBRA OF A FREE MODULE
      page: 0
      pdf_page: 541
    - "no": 9
      title: CRITERIA FOR LINEAR INDEPENDENCE
      page: 0
      pdf_page: 543
statements: 31
exercises: 15
content_sha256: 413c4e77950f8e7b1380f0bbd512ff59bb9f48942d7f589ed00ffe1392087d27
translated_from: content/en/alg/III/07_s7_exterior_algebras.md
source_content_sha256: 76952264b959dbe591e68dd36c4ec6f02ba9ab7f809b7a19e628b038082dd550
translation_model: gpt-5.4-mini, gpt-5-6-mini
translation_run: translate-vi-ad8b440c
glossary_version: 34
glossary_terms_sha256: 9f1e10c30a591b7118cb2afe31617ed956382a0f8f1494a43de7f075949362e5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. ĐẠI SỐ NGOÀI

### 1. ĐỊNH NGHĨA ĐẠI SỐ NGOÀI CỦA MỘT MÔĐUN

#### Định nghĩa 1 {#alg-iii-s7-def-1 .statement}

Cho $A$ là một vành giao hoán và $M$ là một $A$-môđun. Đại số ngoài của $M$, được ký hiệu bởi $\bigwedge(M)$ hoặc $\mathrm{Alt}(M)$ hoặc $\bigwedge_A(M)$, là đại số trên $A$ thu được bằng cách lấy thương của đại số tenxơ $T(M)$ theo iđêan hai phía $\mathfrak{J}''$ (cũng được ký hiệu bởi $\mathfrak{J}_{M}''$) sinh bởi các phần tử $x \otimes x$, với $x$ chạy qua $M$.

Vì iđêan $\mathfrak{J}''$ được sinh bởi các phần tử thuần nhất bậc 2, nên nó là một iđêan phân bậc (II, § 11, no. 3, Mệnh đề 2); ta viết $\mathfrak{J}_n'' = \mathfrak{J}'' \cap T^n(M)$; do đó đại số $\bigwedge(M)$ được phân bậc bởi sự phân bậc (gọi là chính tắc) gồm các $\bigwedge^n(M) = T^n(M)/\mathfrak{J}_n''$. Khi đó $\mathfrak{J}_0'' = \mathfrak{J}_1'' = \{0\}$ và suy ra $\bigwedge^0(M)$ được đồng nhất với $A$ và $\bigwedge^1(M)$ với $T^1(M) = M$; từ đây về sau ta sẽ luôn đồng nhất như vậy và đơn ánh chính tắc $M \to \bigwedge(M)$ sẽ được ký hiệu bởi $\phi''$ hoặc $\phi_M''$.

#### Mệnh đề 1 {#alg-iii-s7-prop-1 .statement}

Cho $E$ là một $A$-đại số và $f : M \to E$ là một ánh xạ tuyến tính $A$ sao cho
$$
(f(x))^2 = 0 \quad \text{với mọi } x \in M.
$$
Có một và chỉ một đồng cấu đại số $g : \bigwedge(M) \to E$ sao cho $f = g \circ \phi''$.

Nói cách khác, $(\bigwedge(M), \phi'')$ là một nghiệm của bài toán ánh xạ phổ quát (Set Theory, IV, § 3, no. 1), trong đó $\Sigma$ là loài của cấu trúc $A$-đại số, còn các $\alpha$-ánh xạ là các ánh xạ tuyến tính từ $A$-môđun $M$ đến một $A$-đại số thỏa mãn (1).

Tính duy nhất của $g$ suy ra từ việc $\phi''(M) = M$ sinh ra $\bigwedge(M)$. Để chứng minh sự tồn tại của $g$, ta nhận thấy rằng theo § 5, no. 1, Mệnh đề 1 tồn tại một đồng cấu đại số $g_1 : T(M) \to E$ sao cho $f = g_1 \circ \phi$; ta cần chứng minh rằng $g_1$ bằng không trên iđêan $\mathfrak{J}''$, vì khi đó nếu
$$
p : T(M) \to \bigwedge(M) = T(M)/\mathfrak{J}''
$$
là đồng cấu chính tắc, ta có thể viết $g_1 = g \circ p$, trong đó $g : \bigwedge(M) \to E$ là một đồng cấu đại số và kết luận sẽ theo từ việc $p \circ \phi = \phi''$. Bây giờ, hạt nhân của $g_1$ là một iđêan hai phía mà, nhờ (1) và quan hệ $g_1 \circ \phi = f$, chứa các phần tử $x \otimes x$ với $x \in M$. Điều này hoàn tất chứng minh.

#### Nhận xét {#alg-iii-s7-n1-rem-1 .statement}

(1) Giả sử rằng $E$ là một A-đại số phân bậc kiểu $\mathbf{Z}$, với phân bậc $(E_n)$, và cũng giả sử rằng ánh xạ tuyến tính $f$ (được giả sử thỏa mãn (1)) sao cho
$$
f(M) \subset E_1.
$$
Khi đó quan hệ $g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p)$ với các $x_i \in M$ cho thấy rằng $g(\bigwedge^p(M)) \subset E_p$ với mọi $p \geq 0$ và do đó $g$ là một đồng cấu đại số phân bậc.

(2) Để tránh nhầm lẫn, tích của hai phần tử $u, v$ của đại số ngoài $\bigwedge(M)$ thường được ký hiệu là $u \wedge v$ và được gọi là *tích ngoài* của $u$ bởi $v$. Các phần tử của $\bigwedge^n(M)$ vì thế là các tổng của các phần tử có dạng $x_1 \wedge x_2 \wedge \cdots \wedge x_n$ với $x_i \in M$ cho $1 \leq i \leq n$ và thường được gọi là *n-vectơ*.

### 2. Tính chất hàm tử của đại số ngoài

#### Mệnh đề 2 {#alg-iii-s7-prop-2 .statement}

*Cho $A$ là một vành giao hoán, $M$ và $N$ là hai $A$-môđun và $u : M \to N$ là một ánh xạ $A$-tuyến tính. Tồn tại một và chỉ một đồng cấu đại số trên $A$*
$$
u'' : \bigwedge(M) \to \bigwedge(N)
$$
*sao cho biểu đồ*

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi_M'' & & \downarrow \phi_N'' \\
\bigwedge(M) & \xrightarrow{u''} & \bigwedge(N)
\end{array}
$$

*là giao hoán. Hơn nữa, $u''$ là một đồng cấu đại số phân bậc.*

Sự tồn tại và tính duy nhất của $u'$ suy ra từ mục 1, Mệnh đề 1 áp dụng cho đại số $\bigwedge(N)$ và $f = \phi_N'' \circ u : M \to \bigwedge(N)$; vì $f(M) \subset N$ nên $f$ thỏa mãn điều kiện (1) theo định nghĩa của $\mathfrak{g}_N''$: vì $f(M) \subset \bigwedge^1(N) = N$, việc $u''$ là một đồng cấu đại số phân bậc suy ra từ *Nhận xét* 1 của mục 1.

Đồng cấu $u''$ của Mệnh đề 2 từ nay sẽ được ký hiệu bởi $\bigwedge(u)$. Nếu $P$ là một $A$-môđun và $v : N \to P$ là một ánh xạ $A$-tuyến tính, thì
$$
\bigwedge(v \circ u) = \bigwedge(v) \circ \bigwedge(u)
$$
vì $\bigwedge(v) \circ \bigwedge(u)$ là một đồng cấu đại số làm cho biểu đồ

$$
\begin{array}{ccc}
M & \xrightarrow{v \quad u} & P \\
\downarrow \phi_M' & & \downarrow \phi_P' \\
\bigwedge(M) & \xrightarrow{\bigwedge(v) \circ \bigwedge(u)} & \bigwedge(P)
\end{array}
$$

giao hoán.

Vì $\Lambda(M)$ chứa $M = \Lambda^1(M)$, nên $\Lambda(u)$ đôi khi được gọi là mở rộng chính tắc của $u$ tới $\Lambda(M)$. Hạn chế $\Lambda^n(u): \Lambda^n(M) \to \Lambda^n(N)$ là như sau
$$
\Lambda^n(u)(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n)
$$
với $x_i \in M$, vì $\Lambda(u)$ là một đồng cấu đại số và $\Lambda^1(u) = u$; hạn chế $\Lambda^0(u)$ lên $A$ là ánh xạ đồng nhất. Chú ý rằng $\Lambda^n(u)$ được thu được từ $T^n(u): T^n(M) \to T^n(N)$ bằng cách chuyển qua các thương.

#### Mệnh đề 3 {#alg-iii-s7-prop-3 .statement}

*Nếu $u: M \to N$ là một ánh xạ tuyến tính $A$ toàn ánh, thì đồng cấu $\Lambda(u): \Lambda(M) \to \Lambda(N)$ là toàn ánh và hạt nhân của nó là iđêan hai phía của $\Lambda(M)$ được sinh bởi hạt nhân $P \subset M \subset \Lambda(M)$ của $u$.

Chứng minh được suy ra từ chứng minh của § 6, no. 2, Mệnh đề 4, bằng cách thay thế $S$ bởi $\Lambda$ và $\mathfrak{g}'$ bởi $\mathfrak{g}''$.

Nếu $u: M \to N$ là một ánh xạ tuyến tính đơn ánh, thì không phải lúc nào cũng đúng rằng $\Lambda(u)$ là một ánh xạ đơn ánh (\S 6, Bài tập 3) (xem tuy nhiên bên dưới no. 9, Hệ quả của Mệnh đề 12). Tuy nhiên điều này đúng khi $u$ là một đơn ánh sao cho $u(M)$ là một nhân tử trực tiếp của $N$ và khi đó ảnh của $\Lambda(u)$ (đẳng cấu với $\Lambda(M)$) là một nhân tử trực tiếp của $\Lambda(N)$; chứng minh giống như chứng minh cho các mệnh đề tương tự đối với $T(u)$ (\S 5, no. 2) bằng cách thay thế $T$ bởi $\Lambda$.

#### Mệnh đề 4 {#alg-iii-s7-prop-4 .statement}

*Cho $N$ và $P$ là hai môđun con của một $A$-môđun $M$ sao cho tổng $N + P$ của chúng là một nhân tử trực tiếp trong $M$ và giao $N \cap P$ của chúng là một nhân tử trực tiếp trong $N$ và trong $P$. Khi đó các đồng cấu $\Lambda(N) \to \Lambda(M)$, $\Lambda(P) \to \Lambda(M)$ và $\Lambda(N \cap P) \to \Lambda(M)$, là các phép mở rộng chính tắc của các đơn ánh chính tắc, đều là đơn ánh; nếu $\Lambda(N)$, $\Lambda(P)$ và $\Lambda(N \cap P)$ được đồng nhất với các đại số con của $\Lambda(M)$ nhờ các đồng cấu này, thì*
$$
\Lambda(N \cap P) = \Lambda(N) \cap \Lambda(P).
$$
Chứng minh được suy ra từ chứng minh của § 5, no. 2, Mệnh đề 4 bằng cách thay thế $T$ bởi $\Lambda$ xuyên suốt. Các giả thiết của Mệnh đề 4 luôn được thỏa mãn bởi các môđun con tùy ý $N, P$ của $M$ khi $A$ là một trường.

#### Hệ quả {#alg-iii-s7-n2-cor-1 .statement}

*Cho $K$ là một trường giao hoán và $M$ là một không gian vectơ trên $K$. Với mọi phần tử $z \in \Lambda(M)$, tồn tại một không gian con vectơ nhỏ nhất $N$ của $M$ sao cho $z \in \Lambda(N)$ và $N$ hữu hạn chiều.*

Chứng minh được suy ra từ chứng minh của § 5, no. 2, Hệ quả của Mệnh đề 4 bằng cách thay thế $T$ bởi $\Lambda$ xuyên suốt.

$N$ được gọi là không gian con vectơ của $M$ liên kết với phần tử $z$ của $\Lambda(M)$.

### 3. TÍNH PHẢN GIAO HOÁN CỦA ĐẠI SỐ NGOÀI

#### Mệnh đề 5 {#alg-iii-s7-prop-5 .statement}

(i) Cho $(x_i)_{1 \leq i \leq n}$ là một dãy hữu hạn các phần tử của môđun $M$; với mọi phép hoán vị $\sigma$ trong nhóm đối xứng $S_n$,

$$
x_{\sigma(1)} \wedge x_{\sigma(2)} \wedge \cdots \wedge x_{\sigma(n)} = \varepsilon_\sigma \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

trong đó $\varepsilon_\sigma$ ký hiệu dấu của phép hoán vị $\sigma$.

(ii) Nếu tồn tại hai chỉ số phân biệt $i, j$ sao cho $x_i = x_j$, tích

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

bằng không.

(i) Trước hết, vì $x \wedge x = 0$ với mọi $x \in M$ theo định nghĩa của iđêan $\mathfrak{g}'$, nên, với $x, y$ trong $M$,

$$
x \wedge y + y \wedge x = (x + y) \wedge (x + y) - x \wedge x - y \wedge y = 0.
$$

Điều này thiết lập (6) trong trường hợp $n = 2$. Trường hợp tổng quát suy ra từ § 4, no. 6, Bổ đề 3.

(ii) Theo giả thiết của (ii), tồn tại một phép hoán vị $\sigma \in S_n$ sao cho $\sigma(1) = i$ và $\sigma(2) = j$; khi đó vế trái của (6) bằng không đối với phép hoán vị này và do đó vế phải cũng vậy.

#### Hệ quả 1 {#alg-iii-s7-prop-5-cor-1 .statement}

Cho $H, K$ là hai tập hợp con bù nhau của khoảng $[1, n]$ của $\mathbf{N}$ và cho $(i_h)_{1 \leq h \leq p}, (j_k)_{1 \leq k \leq n-p}$ là các dãy các phần tử của $H$ và $K$ tương ứng, được sắp xếp theo thứ tự tăng; ta viết

$$
x_H = x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}, \quad x_K = x_{j_1} \wedge x_{j_2} \wedge \cdots \wedge x_{j_{n-p}};
$$

khi đó

$$
x_H \wedge x_K = (-1)^{\nu} x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

trong đó $\nu$ là số các cặp có thứ tự $(i, j) \in H \times K$ sao cho $i > j$.

Theo Mệnh đề 5, điều này quy về việc chứng minh

#### Bổ đề 1 {#alg-iii-s7-lem-1 .statement}

Nếu $\sigma \in S_n$ là phép hoán vị sao cho $\sigma(h) = i_h$ với $1 \leq h \leq p$, $\sigma(h) = j_{n-p}$ với $p + 1 \leq h \leq n$, thì $\varepsilon_\sigma = (-1)^\nu$.

Với $1 \leq h < h' \leq p$ hoặc $p + 1 \leq h < h' \leq n$, $\sigma(h') > \sigma(h)$ và số các cặp có thứ tự $(h, h')$ sao cho $1 \leq h \leq p < h' \leq n$ và $\sigma(h) > \sigma(h')$ bằng $\nu$.

#### Hệ quả 2 {#alg-iii-s7-lem-1-cor-2 .statement}

Đại số phân bậc $\bigwedge(M)$ là phản xứng ($\S 4$, no. 9).

Chỉ cần áp dụng Mệnh đề 13 của $\S 4$, no. 9 cho $\bigwedge(M)$, lấy tập hợp $M$ làm hệ sinh và sử dụng Mệnh đề 5.

#### Mệnh đề 6 {#alg-iii-s7-prop-6 .statement}

*Nếu M là một A-môđun sinh hữu hạn, $\bigwedge(M)$ là một A-môđun sinh hữu hạn; ngoài ra, nếu M thừa nhận một hệ sinh gồm n phần tử, thì $\bigwedge^p(M) = \{0\}$ với $p > n$.*

Cho $(x_i)_{1 \leq i \leq n}$ là một hệ sinh của M. Mọi phần tử của $\bigwedge^p(M)$ là một tổ hợp tuyến tính của các phần tử có dạng
$$
x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}
$$
trong đó các chỉ số $i_k$ thuộc $\{1, n\}$; theo Mệnh đề 5, có thể giả sử các chỉ số này phân biệt (nếu không phần tử tương ứng bằng không). Nếu $p > n$, không có dãy chỉ số nào như vậy và do đó $\bigwedge^p(M) = \{0\}$. Nếu $p \leq n$, các dãy này có số lượng hữu hạn, điều này hoàn tất chứng minh.

### 4. LŨY THỪA NGOÀI THỨ *n* CỦA MỘT MÔĐUN VÀ CÁC ÁNH XẠ ĐA TUYẾN TÍNH PHẢN XỨNG

Cho hai A-môđun M, N trên một vành giao hoán A, một *ánh xạ n-tuyến tính phản xứng* từ $M^n$ vào N là bất kỳ ánh xạ *n*-tuyến tính $f : M^n \to N$ sao cho, với mọi $p \leq n - 2$,
$$
f(u_1, \ldots, u_p, x, x, v_1, \ldots, v_{n-p-2}) = 0
$$
với mọi x, các $u_i$ ($1 \leq i \leq p$) và các $v_j$ ($1 \leq j \leq n - p - 2$) trong M.

#### Mệnh đề 7 {#alg-iii-s7-prop-7 .statement}

*Cho A là một vành giao hoán và M và N là hai A-môđun. Nếu với mỗi ánh xạ A-tuyến tính $g : \bigwedge^n(M) \to N$ ($n \geq 2$) ta gán ánh xạ n-tuyến tính*
$$
(x_1, x_2, \ldots, x_n) \mapsto g(x_1 \wedge x_2 \wedge \cdots \wedge x_n)
$$
*thì thu được một ánh xạ A-tuyến tính song ánh của A-môđun $\operatorname{Hom}_A(\bigwedge^n(M), N)$ lên A-môđun các ánh xạ n-tuyến tính phản xứng của $M^n$ vào N.*

Ta xét song ánh chính tắc của A-môđun $\operatorname{Hom}_A(T^n(M), N)$ lên A-môđun $\mathcal{L}_n(M, \ldots, M; N)$ gồm tất cả các ánh xạ n-tuyến tính của $M^n$ vào N, thu được bằng cách gán cho mỗi ánh xạ A-tuyến tính $f : T^n(M) \to N$ ánh xạ n-tuyến tính
$$
\tilde{f} : (x_1, \ldots, x_n) \mapsto f(x_1 \otimes x_2 \otimes \cdots \otimes x_n)
$$
(II, § 3, no. 9). Mặt khác, các ánh xạ A-tuyến tính $g : \bigwedge^n(M) \to N$ tương ứng một-một với các ánh xạ A-tuyến tính $f : T^n(M) \to N$ sao cho *f bằng zero trên $\mathfrak{g}_n''$*, bằng cách gán cho g ánh xạ $f = g \circ p_n$, trong đó
$$
p_n : T^n(M) \to \bigwedge^n(M) = T^n(M)/\mathfrak{g}_n''
$$

là đồng cấu chính tắc (II, § 2, no. 1, Định lý 1). Nhưng vì $\mathfrak{J}_n''$ là một tổ hợp tuyến tính của các phần tử có dạng
$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_p) \otimes (x \otimes x) \otimes (v_1 \otimes \cdots \otimes v_{n-p-2})
$$
$(x, u_i, v_j$ trong $M$), nói rằng $f$ có dạng $g \circ p_n$ có nghĩa là hàm n-tuyến tính tương ứng $\bar{f}$ thỏa mãn (8), nói cách khác nó là *phản xứng*.

A-môđun $\bigwedge^n(M)$ được gọi là *lũy thừa ngoài thứ n* của M. Với mọi đồng cấu A-môđun $u : M \to N$, ánh xạ
$$
\bigwedge^n(u) : \bigwedge^n(M) \to \bigwedge^n(N)
$$
trùng với $\bigwedge(u)$ trên $\bigwedge^n(M)$ được gọi là *lũy thừa ngoài thứ n của u*.

#### Hệ quả 1 {#alg-iii-s7-prop-7-cor-1 .statement}

*Với mọi ánh xạ n-tuyến tính phản xứng* $g : M^n \to N$, *với mọi phép hoán vị* $\sigma \in \mathfrak{S}_n$,
$$
g(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(n)}) = \varepsilon_\sigma \cdot g(x_1, x_2, \ldots, x_n)
$$
*đối với mọi* $x_i \in M$; *hơn nữa nếu* $x_i = x_j$ *đối với hai chỉ số phân biệt* $i, j$, *thì*
$$
g(x_1, x_2, \ldots, x_n) = 0.
$$
Đây là một hệ quả hiển nhiên của Mệnh đề 7 và no. 3, Mệnh đề 5.

#### Hệ quả 2 {#alg-iii-s7-prop-7-cor-2 .statement}

*Cho* $(x_i)_{1 \leq i \leq n}$ *là một dãy gồm n phần tử của M sao cho*
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0;
$$
*thì, với mọi ánh xạ n-tuyến tính phản xứng* $g : M^n \to N$, $g(x_1, \ldots, x_n) = 0$.

#### Hệ quả 3 {#alg-iii-s7-prop-7-cor-3 .statement}

*Cho* $f : M^{n-1} \to A$ *là một dạng* $(n-1)$*-tuyến tính phản xứng*. *Nếu* $(x_i)_{1 \leq i \leq n}$ *là một dãy gồm n phần tử của M sao cho* $x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0$, *thì*
$$
\sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i = 0
$$
*(trong đó ta viết* $f(x_1, \ldots, \hat{x}_i, \ldots, x_n) = f(x_1, \ldots, x_{i-1}, x_{i+1}, \ldots, x_n)$ *cho* $1 \leq i \leq n$.

Đủ để chứng minh rằng ánh xạ $n$-tuyến tính
$$
(x_1, \ldots, x_n) \mapsto \sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i
$$
từ $M^n$ vào $M$ là *phản xứng*. Bây giờ, nếu $x_i = x_{i+1}$, thì mọi hạng trong tổng ở vế phải đều có hệ số bằng không, trừ $x_i$ và $x_{i+1}$, vì $f$ là phản xứng; mặt khác, hệ số của $x_i$ là
$$
(-1)^i f(x_1, \ldots, x_{i-1}, x_{i+1}, x_{i+2}, \ldots, x_n)
$$

và hệ số của $x_{i+1}$ là $(-1)^{i+1} f(x_1, \ldots, x_i, x_{i+2}, \ldots, x_n)$ và chúng là nghịch đảo theo giả thiết.

#### Nhận xét {#alg-iii-s7-n4-rem-1 .statement}

Một phần tử $z$ của $T^n(M)$ được gọi là một (phản biến) *tenxơ phản xứng cấp* $n$ nếu $\sigma.z = \varepsilon_\sigma z$ với mọi phép hoán vị $\sigma \in S_n$ (xem § 6, no. 3, Nhận xét); các phần tử này tạo thành một A-môđun con $A'_n(M)$ của $T^n(M)$. Với mọi $z \in T^n(M)$, ta viết $a.z = \sum_{\sigma \in S_n} \varepsilon_\sigma(\sigma.z)$ và gọi $a.z$ là *phản xứng hóa* của $z$; vì $\varepsilon_{\sigma\tau} = \varepsilon_\sigma \varepsilon_\tau$, ta thấy ngay rằng $a.z$ là một tenxơ phản xứng và do đó $z \mapsto a.z$ là một tự đồng cấu của $T^n(M)$ có ảnh $A''_n(M)$ được chứa trong $A'_n(M)$; nói chung $A''_n(M) \neq A'_n(M)$ (Bài tập 8). Nếu $z$ là một tenxơ phản xứng, thì $a.z = n!z$; do đó, *khi* $n!$ *khả nghịch trong* $A$, tự đồng cấu $z \mapsto (n!)^{-1}a.z$ là một *phép chiếu* của $T^n(M)$ có ảnh là

$$
A'_n(M) = A''_n(M).
$$

Hơn nữa, *hạt nhân* của phép chiếu này chỉ là $\mathfrak{J}_n''$; vì hiển nhiên chỉ có thể xét trường hợp $n \geqslant 2$, nên 2 (một ước của $n!$) khả nghịch trong $A$ và $x \otimes x = 2^{-1}(x \otimes x + x \otimes x)$; do đó $\mathfrak{J}_n''$ được sinh bởi các phần tử $z + \rho.z$, trong đó $\rho$ là một phép hoán vị đổi chỗ hai số liên tiếp trong $\{1, n\}$; hơn nữa, với hai phép hoán vị $\sigma, \tau$ trong $S_n$, ta có thể viết

$$
z - \varepsilon_{\sigma\tau}((\sigma\tau).z) = z - \varepsilon_\tau(\tau.z) + \varepsilon_\tau(\tau.z - \varepsilon_\sigma \sigma.(\tau.z))
$$

do đó suy ra rằng $z - \varepsilon_\sigma(\sigma.z) \in \mathfrak{J}_n''$ với mọi $z \in T^n(M)$ và $\sigma \in S_n$. Vì thế (luôn giả sử $n!$ khả nghịch trong $A$), ta thấy rằng

$$
z - (n!)^{-1}a.z = \sum_{\sigma \in S_n} (n!)^{-1}(z - \varepsilon_\sigma(\sigma.z)) \in \mathfrak{J}_n''
$$

với mọi $z \in T^n(M)$, điều đó chứng minh mệnh đề của chúng ta.

Khi $n!$ khả nghịch trong $A$, các môđun con $A'_n(M)$ và $\mathfrak{J}_n''$ của $T^n(M)$ do đó là *bổ sung* nhau, và sự hạn chế lên $A'_n(M)$ của đồng cấu chính tắc $T^n(M) \to \bigwedge^n(M) = T^n(M)/\mathfrak{J}_n''$ là một *đẳng cấu* A-môđun, điều này cho phép ta trong trường hợp đang xét đồng nhất tensor phản đối xứng cấp $n$ với các phần tử của lũy thừa ngoài thứ $n$ của $M$. Ở đây cũng lưu ý rằng sự đồng nhất này không tương thích với phép nhân, vì tích trong $T(M)$ của hai tensor phản đối xứng nói chung không còn phản đối xứng.

### 5. MỞ RỘNG VÀNH HỆ SỐ

Cho $A, A'$ là hai vành giao hoán, $\rho : A \to A'$ là một đồng cấu vành, $M$ là một $A$-môđun, $M'$ là một $A'$-môđun và $f : M \to M'$ là một *A-đồng cấu* (tương ứng với $\rho$) từ $M$ vào $M'$. Ánh xạ hợp thành $M \xrightarrow{f} M' \xrightarrow{\phi_{M'}} \bigwedge_{A'}(M')$ là một ánh xạ A-tuyến tính từ $M$ vào đại số trên A $\bigwedge_{A'}(M')$ và, vì các phần tử của f(M) ⊂ M' có bình phương bằng không trong $\bigwedge_{A'}(M')$, tồn tại (no. 1, Mệnh đề 1) duy nhất một đồng cấu đại số trên A $f'' : \bigwedge_A(M) \to \bigwedge_{A'}(M')$ làm cho biểu đồ sau giao hoán

$$
\begin{array}{ccc}
M & \xrightarrow{f} & M' \\
\downarrow \phi_M'' & & \downarrow \phi_{M'}'' \\
\bigwedge_A(M) & \xrightarrow{f''} & \bigwedge_{A'}(M')
\end{array}
$$

và $f''$ là một đồng cấu đại số phân bậc. Suy ra ngay rằng nếu $\sigma : A' \to A''$ là một đồng cấu vành khác, $M''$ là một $A''$-môđun, $g : M' \to M''$ là một $A'$-đồng cấu (tương ứng với $\sigma$) và $g'' : \bigwedge_{A'}(M') \to \bigwedge_{A''}(M'')$ là đồng cấu đại số trên $A''$ tương ứng, thì đồng cấu đại số trên A hợp thành

$$
\bigwedge_A(M) \xrightarrow{f''} \bigwedge_{A'}(M') \xrightarrow{g''} \bigwedge_{A''}(M'')
$$

tương ứng với đồng cấu trên A hợp thành $g \circ f : M \to M''$ (tương ứng với $\sigma \circ \rho$).

#### Mệnh đề 8 {#alg-iii-s7-prop-8 .statement}

*Cho $A, B$ là hai vành giao hoán, $\rho : A \to B$ là một đồng cấu vành và $M$ là một $A$-môđun. Sự mở rộng chính tắc*

$$
\psi : \bigwedge_B(B \otimes_A M) \to B \otimes_A \bigwedge_A(M)
$$

*của ánh xạ B-tuyến tính* $1_B \otimes \phi_M'' : B \otimes_A M \to B \otimes_A \bigwedge_A(M)$ *là một đẳng cấu đại số trên B phân bậc.*

Chứng minh được suy ra từ chứng minh của § 5, no. 4, Mệnh đề 5, bằng cách thay $T$ bởi $\bigwedge$ và $\phi_M$ bởi $\phi_M''$.

### 6. GIỚI HẠN TRỰC TIẾP CỦA CÁC ĐẠI SỐ NGOÀI

Cho $(A_\alpha, \phi_{\beta \alpha})$ là một hệ trực tiếp có hướng của các vành giao hoán, $(M_\alpha, f_{\beta \alpha})$ là một hệ trực tiếp của các $A_\alpha$-môđun, $A = \lim \to A_\alpha$ và $M = \lim \to M_\alpha$. Với $\alpha \leq \beta$, từ đồng cấu $A_\alpha$-môđun $f_{\beta \alpha} : M_\alpha \to M_\beta$ ta suy ra một cách chính tắc một đồng cấu $A_\alpha$-đại số (no. 5, công thức (12)) $f_{\beta \alpha}' : \bigwedge_{A_\alpha}(M_\alpha) \to \bigwedge_{A_\beta}(M_\beta)$ và từ (13) suy ra rằng $(\bigwedge_{A_\alpha}(M_\alpha), f_{\beta \alpha}')$ là một *hệ trực tiếp các môđun phân bậc* $A_\alpha$*.* Mặt khác, cho $f_\alpha : M_\alpha \to M$ là đồng cấu $A_\alpha$-môđun chính tắc; ta suy ra (no. 5, công thức (12)) một đồng cấu đại số phân bậc $A_\alpha$ $f_\alpha'' : \bigwedge_{A_\alpha}(M_\alpha) \to \bigwedge_A(M)$ và cũng suy ra từ (13) rằng các $f_\alpha''$ lập thành một hệ trực tiếp các đồng cấu $A_\alpha$-môđun.

#### Mệnh đề 9 {#alg-iii-s7-prop-9 .statement}

*Đồng cấu A* $f'' = \varprojlim f''_\alpha : \varprojlim \Lambda_{A_\alpha}(M_\alpha) \to \Lambda_A(M)$ *là một đẳng cấu đại số phân bậc*.

Chứng minh giống như của § 5, no. 4, Mệnh đề 6, thay T bằng $\Lambda$ và $\phi$ bằng $\phi''$ ở mọi chỗ và xét đến sự kiện rằng giới hạn trực tiếp của các đại số phản xứng là phản xứng.

### 7. ĐẠI SỐ NGOÀI CỦA MỘT TỔNG TRỰC TIẾP. ĐẠI SỐ NGOÀI CỦA MỘT MÔĐUN PHÂN BẬC

Cho A là một vành giao hoán, $M = \bigoplus_{\lambda \in L} M_\lambda$ là tổng trực tiếp của một họ các A-môđun và $j_\lambda : M_\lambda \to M$ là đơn ánh chính tắc; suy ra một đồng cấu $A$-đại số phân bậc $\Lambda(j_\lambda) : \Lambda(M_\lambda) \to \Lambda(M)$. Vì $\Lambda(M)$ là phản giao hoán, có thể áp dụng Mệnh đề 10 của § 4, no. 7 (hoặc nếu cần thì tổng quát hóa sang trường hợp L vô hạn, xem § 4, no. 8, *Nhận xét* 1) cho các đồng cấu $\Lambda(j_\lambda)$; khi đó tồn tại một đồng cấu đại số duy nhất

$$
g : \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda) \to \Lambda(M)
$$

(còn được ký hiệu bởi $g_M$) sao cho $\Lambda(j_\lambda) = g \circ f_\lambda$, với

$$
f_\lambda : \Lambda(M_\lambda) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)
$$

ký hiệu đồng cấu chính tắc.

#### Mệnh đề 10 {#alg-iii-s7-prop-10 .statement}

*Đồng cấu chính tắc* g (*công thức (14)*) *là một đẳng cấu đại số phân bậc*.

Để chứng minh rằng g song ánh, ta định nghĩa một đồng cấu đại số phân bậc

$$
h : \Lambda(M) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)
$$

sao cho $g \circ h$ và $h \circ g$ lần lượt là các ánh xạ đồng nhất trên $\Lambda(M)$ và $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$. Với mỗi $\lambda \in L$, xét ánh xạ tuyến tính hợp thành

$$
u_\lambda : M_\lambda \xrightarrow{\phi''_{M_\lambda}} \Lambda(M_\lambda) \xrightarrow{f_\lambda} \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda).
$$

Có một và chỉ một ánh xạ A-tuyến tính $u : M \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$ sao cho $u \circ j_\lambda = u_\lambda$ với mọi $\lambda \in L$. Tích tenxơ phản xứng $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$ là một *đại số phản xứng*: vì, với L hữu hạn, điều này suy ra từ § 4, no. 9, Mệnh đề 14 và, với L tùy ý, điều này suy ra từ định nghĩa của tích này cho trong § 4, no. 8, *Nhận xét* 1 và từ sự kiện rằng giới hạn trực tiếp của các đại số phân bậc phản xứng là phản xứng. Vì $u(M)$ cũng được chứa trong môđun con các phần tử bậc 1 trong đại số phân bậc $\bigotimes_{\lambda \in L} \Lambda(M_\lambda)$, nên từ no. 1, Mệnh đề 1 và *Nhận xét* 1 suy ra rằng tồn tại một đồng cấu đại số phân bậc duy nhất.

$$
h : \Lambda(M) \to \bigotimes_{\lambda \in L} \Lambda(M_\lambda)
$$

sao cho $h \circ \phi''_M = u$. Việc kiểm tra rằng $g \circ h$ và $h \circ g$ là các ánh xạ đồng nhất được tiến hành như ở § 6, no. 6, Mệnh đề 9, thay $S$ bằng $\Lambda$ và $\phi'$ bằng $\phi''$.

#### Nhận xét {#alg-iii-s7-n7-rem-1 .statement}

Cho $N = \bigoplus_{\lambda \in L} N_\lambda$ là tổng trực tiếp của một họ khác các $A$-môđun với $L$ làm tập chỉ số và, với mọi $\lambda \in L$, cho $v_\lambda : M_\lambda \to N_\lambda$ là một ánh xạ A-tuyến tính, do đó có một ánh xạ A-tuyến tính $v = \bigoplus_\lambda v_\lambda : M \to N$ (II, § 1, no. 6, Mệnh đề 7). Khi đó biểu đồ

==========

$$
\begin{array}{ccc}
\bigotimes_{\lambda \in L} \Lambda(M_\lambda) & \xrightarrow{g_M} & \Lambda(M) \\
\downarrow & & \downarrow \\
\bigotimes_{\lambda \in L} \Lambda(v_\lambda) & & \Lambda(v) \\
\downarrow & & \downarrow \\
\bigotimes_{\lambda \in L} \Lambda(N_\lambda) & \xrightarrow{g_N} & \Lambda(N)
\end{array}
$$

là giao hoán (xem § 4, no. 5, Hệ quả của Mệnh đề 8).

Môđun con $A$-môđun của $\bigotimes_{\lambda \in L} \Lambda(M_\lambda)$ mà $\Lambda^n(M)$ được đồng nhất với nó nhờ đẳng cấu $g$ có thể được mô tả chính xác hơn. Với mọi tập con hữu hạn $J$ của $L$, ta viết $E_J = \bigotimes_{\lambda \in J} \Lambda(M_\lambda)$, do đó $\bigotimes_{\lambda \in L} \Lambda(M_\lambda) = \lim \to E_J$ tương ứng với tập có hướng $\mathcal{F}(L)$ gồm các tập con hữu hạn của $L$, theo định nghĩa ($\S 4$, no. 8, *Nhận xét* 1). Với mọi họ $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$ (vì vậy có giá đỡ *hữu hạn*) sao cho $\sum_{\lambda \in L} n_\lambda = n$ và mọi tập con hữu hạn $J$ của $L$ chứa giá đỡ của họ $\nu$, ta viết

$$
\Lambda^{J,\nu}(M) = \bigotimes_{\lambda \in J} \Lambda^{n_\lambda}(M_\lambda)
$$

do đó môđun con $E_{J,n}$ gồm các phần tử bậc $n$ trong $E_J$ là *tổng trực tiếp* của các $\Lambda^{J,\nu}(M)$ đối với mọi họ $\nu$ có giá đỡ được chứa trong $J$ và sao cho

$$
\sum_{\lambda \in L} n_\lambda = n
$$

($\S 4$, no. 7, Mệnh đề 10 và no. 8). Theo quy ước ta viết $\Lambda^{J,\nu}(M) = \{0\}$ cho các họ $\nu$ mà giá đỡ của chúng không được chứa trong $J$; khi đó

E_{J,n} cũng có thể được gọi là tổng trực tiếp của tất cả các $\bigwedge^{J,\nu}(M)$, trong đó $\nu$ chạy qua tập $H_n$ gồm tất cả các họ $\nu = (n_\lambda)_{\lambda \in L}$ sao cho $\sum_{\lambda \in L} n_\lambda = n$. Vì $\bigwedge^0(M_\lambda)$ được đồng nhất với $A$, rõ ràng cũng với hai tập con hữu hạn $J \subset J'$ của $L$ và một họ $\nu$ có giá đỡ được chứa trong $J$, ánh xạ chính tắc $\bigwedge^{J,\nu}(M) \to \bigwedge^{J',\nu}(M)$ (hạn chế của ánh xạ chính tắc $E_J \to E_{J'}$ lên $\bigwedge^{J,\nu}(M)$) là song ánh. Nếu ta viết, với mọi $\nu \in H_n$,

$$
\bigwedge^\nu(M) = \lim_{\longrightarrow} \bigwedge^{J,\nu}(M)
$$

thì khi xét đến II, § 6, no. 2, Mệnh đề 5, ta thấy rằng:

#### Hệ quả {#alg-iii-s7-n7-cor-1 .statement}

*Môđun* $A$-*môđun* $\bigwedge^n(M)$ *là ảnh qua đẳng cấu (14) của môđun con của* $\bigotimes_{\lambda \in L} \bigwedge(M_\lambda)$* *là tổng trực tiếp của các môđun con* $\bigwedge^\nu(M)$* *đối với mọi họ* $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$* *sao cho* $\sum_{\lambda \in L} n_\lambda = n$; *nếu* $J$* là giá đỡ của* $\nu$, $\bigwedge^\nu(M)$* *đẳng cấu chính tắc với* $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_\lambda)$.

Nói chung $\bigwedge^\nu(M)$, $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_\lambda)$ và ảnh của chúng trong $\bigwedge^n(M)$ được đồng nhất. Với quy ước này:

#### Mệnh đề 11 {#alg-iii-s7-prop-11 .statement}

*Cho $\Delta$ là một monoid giao hoán, $M$ là một A-môđun phân bậc kiểu $\Delta$ và* $(M_\alpha)_{\alpha \in \Delta}$* *là sự phân bậc của nó. Với mỗi cặp có thứ tự* $(\alpha, n) \in \Delta \times \mathbf{N}$, *đặt* $\bigwedge^{\alpha,n}(M)$* *là môđun con của* $\bigwedge^n(M)$* *là tổng trực tiếp của các môđun con* $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_{\alpha_\lambda})$, *trong đó* $(n_\lambda)_{\lambda \in L}$* *chạy qua tập các họ số nguyên* $\geq 0$* *sao cho* $\sum_{\lambda \in L} n_\lambda = n$, $J$* *là giá đỡ của nó và, với mỗi* $(n_\lambda)$, $(\alpha_\lambda)_{\lambda \in J}$* *chạy qua tập các họ của* $\Delta^J$* *sao cho* $\sum_{\lambda \in J} \alpha_\lambda = \alpha$. *Khi đó* $(\bigwedge^{\alpha,n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$* *là phân bậc duy nhất kiểu* $\Delta \times \mathbf{N}$* *tương thích với cấu trúc đại số trên* $\bigwedge(M)$* *và cảm sinh trên* $M = \bigwedge^1(M)$* *phân bậc đã cho.*

Việc $\bigwedge(M)$ là tổng trực tiếp của các $\bigwedge^{\alpha,n}(M)$ suy ra từ Hệ quả của Mệnh đề 10; phần còn lại của chứng minh giống hệt với phần cuối của chứng minh ở § 5, no. 5, Mệnh đề 7.

### 8. ĐẠI SỐ NGOÀI CỦA MỘT MÔĐUN TỰ DO

#### Định lý 1 {#alg-iii-s7-thm-1 .statement}

*Cho* $M$* *là một A-môđun có một cơ sở* $(e_\lambda)_{\lambda \in L}$. *Cho* $L$* *được cho cấu trúc của một tập sắp thứ tự toàn phần* (Lý thuyết tập hợp, III, § 2, no. 3, Định lý 1)* *và với mỗi tập con hữu hạn* $J$* *của* $L$* *ta viết*

$$
e_J = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}
$$

trong đó $(\lambda_k)_{1 \leq k \leq n}$ là dãy các phần tử của J được sắp theo thứ tự tăng (Lý thuyết tập hợp, III, § 5, no. 3, Mệnh đề 6); ta viết $e_\varnothing = 1$, phần tử đơn vị của A. Khi đó các $e_J$, khi J chạy qua tập $\mathcal{F}(L)$ các tập con hữu hạn của L, lập thành một cơ sở của đại số ngoài $\bigwedge(M)$.

Vì các $e_\lambda$ sinh ra A-môđun M, mọi phần tử của $\bigwedge(M)$ là một tổ hợp tuyến tính của hữu hạn tích các phần tử $e_\lambda$ và do đó (theo no. 3, Mệnh đề 5) là một tổ hợp tuyến tính của hữu hạn phần tử $e_J$ với $J \in \mathcal{F}(L)$. Điều còn lại là chứng minh rằng các $e_J$ độc lập tuyến tính trên A. Nếu không, sẽ tồn tại giữa các phần tử này một quan hệ tuyến tính với các hệ số không phải đều bằng $0$; hợp của các tập con J tương ứng với những $e_J$ có hệ số trong quan hệ này khác $0$ là một tập con hữu hạn K của L (vì chỉ có hữu hạn hệ số khác $0$). Đặt N là môđun con của M sinh bởi các $e_\lambda$ sao cho $\lambda \in K$; N là một nhân tử trực tiếp trong M, do đó (no. 2) $\bigwedge(N)$ được đồng nhất với một đại số con của $\bigwedge(M)$ và, nếu ta chứng minh rằng các $e_J$ với $J \subset K$ lập thành một cơ sở của $\bigwedge(N)$, thì ta sẽ thu được phản chứng mong muốn.

Do đó chỉ cần chứng minh Định lý 1 khi cơ sở của M là hữu hạn; vì vậy ta có thể giả sử rằng $L = \{1, m\} \subset N$. Với mỗi $i \in L$, đặt $M_i$ là môđun con tự do $Ae_i$ của M; M là tổng trực tiếp của các $M_i$ và $\bigwedge(M_i)$ là tổng trực tiếp của $\bigwedge^0(M_i) = A$ và $\bigwedge^1(M_i) = M_i$ (no. 3, Mệnh đề 6). Hãy đồng nhất một cách chính tắc $\bigwedge(M)$ với A-môđun là tích tenxơ của các $\bigwedge(M_i)$ (no. 7, Mệnh đề 10); môđun sau có cơ sở là tích tenxơ của các cơ sở $(1, e_i)$ của các $\bigwedge(M_i)$ (II, § 3, no. 7, Hệ quả 2 của Mệnh đề 7); do đó ta thu được mọi phần tử

$$
u_1 \otimes u_2 \otimes \cdots \otimes u_m
$$

trong đó hoặc $u_i = 1$ hoặc $u_i = e_i$; nếu J là tập các chỉ số i sao cho $u_i = e_i$, thì $u_1 \otimes u_2 \otimes \cdots \otimes u_m$ đồng nhất với $e_J$, và thế là chứng minh xong.

#### Hệ quả 1 {#alg-iii-s7-thm-1-cor-1 .statement}

Giả sử rằng $L = \{1, m\}$; khi đó cơ sở $(e_J)_{J \in \mathcal{P}(L)}$ của $\bigwedge(M)$ có $2^m$ phần tử. Với $p > m$, $\bigwedge^p(M) = \{0\}$; $\bigwedge^m(M)$ có một cơ sở gồm một phần tử duy nhất $e_L$; với $0 \leq p \leq m$ số phần tử trong cơ sở $(e_J)$ của $\bigwedge^p(M)$ gồm các $e_J$ sao cho $\mathrm{Card}(J) = p$ là

$$
\binom{m}{p} = \frac{m!}{p!(m-p)!}
$$

Điều này suy ra từ Lý thuyết tập hợp, III, § 3, no. 5, Mệnh đề 12 và Lý thuyết tập hợp, III, § 5, no. 8, Hệ quả 1 của Mệnh đề 11.

Ta trở lại trường hợp mà tập L trong Định lý 1 là tùy ý và cho tường minh bảng phép nhân (\S 1, no. 7) của cơ sở $(e_J)$. Cho hai tập con hữu hạn J, K của tập sắp thứ tự toàn phần L, ta viết
$$
\begin{cases}
\rho_{J, K} = 0 & \text{nếu } J \cap K \neq \varnothing \\
\rho_{J, K} = (-1)^v & \text{nếu } J \cap K = \varnothing
\end{cases}
$$
trong đó v chỉ số cặp có thứ tự $(\lambda, \mu) \in J \times K$ sao cho $\lambda > \mu$. Khi đó Hệ quả 1 của Mệnh đề 4 ở no. 2 ngay lập tức suy ra quan hệ
$$
e_J \wedge e_K = \rho_{J, K} e_{J \cup K}.
$$
Lưu ý công thức
$$
\rho_{J, K} \rho_{K, J} = (-1)^{jk}
$$
khi $J \cap K = \varnothing, j = \mathrm{Card}(J), k = \mathrm{Card}(K)$ (no. 3, Hệ quả 2 của Mệnh đề 5.)

#### Hệ quả 2 {#alg-iii-s7-thm-1-cor-2 .statement}

*Nếu M là một A-môđun xạ ảnh, $\bigwedge(M)$ là một A-môđun xạ ảnh.*

Chứng minh giống như của \S 5, no. 5, Hệ quả của Định lý 1, thay T bằng $\bigwedge$.

#### Hệ quả 3 {#alg-iii-s7-thm-1-cor-3 .statement}

*Cho M là một A-môđun xạ ảnh và $(x_i)_{1 \leq i \leq n}$ là một dãy hữu hạn các phần tử của M. Để tồn tại trên M một dạng n-tuyến tính phản xứng f sao cho*
$$
f(x_1, x_2, \ldots, x_n) \neq 0,
$$
*điều kiện cần và đủ là* $x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0$.

Ta đã biết (không có giả thiết nào về M) rằng điều kiện là cần thiết (no. 4, Mệnh đề 7). Giả sử giờ rằng M là xạ ảnh và rằng
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0.
$$
Khi đó $\bigwedge^n(M)$ là xạ ảnh (Hệ quả 2) và do đó ánh xạ chính tắc
$$
\bigwedge^n(M) \to (\bigwedge^n(M))^{**}
$$
là đơn ánh (II, \S 2, no. 7, Hệ quả 4 của Mệnh đề 13); suy ra có một dạng tuyến tính $g : \bigwedge^n(M) \to A$ sao cho $g(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \neq 0$. Nếu f là dạng n-tuyến tính phản xứng tương ứng với g (no. 4, Mệnh đề 7), thì $f(x_1, \ldots, x_n) \neq 0$.

### 9. CÁC TIÊU CHUẨN ĐỘC LẬP TUYẾN TÍNH

#### Mệnh đề 12 {#alg-iii-s7-prop-12 .statement}

*Cho M là một A-môđun xạ ảnh. Để các phần tử $x_1, x_2, \ldots, x_n$ của M phụ thuộc tuyến tính, điều kiện cần và đủ là tồn tại $\lambda \neq 0$ trong A sao cho*
$$
\lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0.
$$

Điều kiện này là cần thiết (không có giả thiết nào về M), vì chẳng hạn nếu $\lambda x_1$ (với $\lambda \neq 0$) là một tổ hợp tuyến tính của $x_2, \ldots, x_n$, thì quan hệ (22) đúng (no. 3, Mệnh đề 5). Ta chứng minh rằng điều kiện này là đủ bằng quy nạp trên $n$; với $n = 1$, đó là một hệ quả tầm thường của định nghĩa. Vậy giả sử rằng $n > 1$ và điều kiện (22) đúng với một $\lambda \neq 0$. Nếu
$$
\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n = 0,
$$
thì giả thiết quy nạp suy ra rằng $x_2, \ldots, x_n$ phụ thuộc tuyến tính và do đó *a fortiori* $x_1, x_2, \ldots, x_n$ cũng vậy. Nếu $\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n \neq 0$, thì từ no. 8, Hệ quả 3 của Định lý 1 suy ra rằng tồn tại một dạng phản xứng $(n - 1)$-tuyến tính $f$ sao cho $f(\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n) = \mu \neq 0$. Vì
$$
x_1 \wedge (\lambda x_2) \wedge \cdots \wedge x_n = 0,
$$
nên từ no. 8, Hệ quả 3 của Định lý 1 suy ra rằng $\mu x_1$ là một tổ hợp tuyến tính của $\lambda x_2, x_3, \ldots, x_n$; do đó $x_1, x_2, \ldots, x_n$ phụ thuộc tuyến tính.

#### Hệ quả {#alg-iii-s7-n9-cor-1 .statement}

*Cho M và N là hai A-môđun xạ ảnh và $f : M \to N$ là một ánh xạ A-tuyến tính. Nếu f là đơn ánh, thì $\Lambda(f) : \Lambda(M) \to \Lambda(N)$ là đơn ánh.*

Ta chứng minh điều này trước hết dưới giả thiết rằng M là *tự do*; cho $(e_\lambda)_{\lambda \in L}$ là một cơ sở của M, khi đó $(e_J)_{J \in \mathfrak{B}(L)}$ (công thức (18)) là một cơ sở của $\Lambda(M)$. Giả sử rằng hạt nhân của $\Lambda(f)$ chứa một phần tử $u = \sum_J \alpha_J e_J \neq 0$. Gọi K là một tập con cực tiểu trong số các tập con hữu hạn J sao cho $\alpha_J \neq 0$ và gọi H là một tập con hữu hạn của L rời nhau với K và sao cho $K \cup H$ chứa tất cả các J (hữu hạn về số lượng) sao cho $\alpha_J \neq 0$; vì vậy, với mọi $J \neq K$ sao cho $\alpha_J \neq 0$, theo định nghĩa ta có $J \cap H \neq 0$ và do đó (no. 8, công thức (20)).
$$
u \wedge e_H = +\alpha_K e_{K \cup H}
$$
thuộc iđêan hai phía của $\Lambda(M)$, tức hạt nhân của $\Lambda(f)$. Ta viết $e_{K \cup H} = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}$; khi đó $\alpha_K f(e_{\lambda_1}) \wedge f(e_{\lambda_2}) \wedge \cdots \wedge f(e_{\lambda_n}) = 0$; nhờ Mệnh đề 12, các phần tử $f(e_{\lambda_i})$ ($1 \leq i \leq n$) của N phụ thuộc tuyến tính. Nhưng điều này mâu thuẫn với giả thiết rằng $f$ là đơn ánh (II, § 1, no. 11, Hệ quả 3 của Mệnh đề 17).

Ta xét trường hợp tổng quát; cho $M'$ là một A-môđun sao cho $M \oplus M' = P$ là tự do (II, § 2, no. 2, Mệnh đề 4). Xét ánh xạ tuyến tính $g : M \oplus M' \to N \oplus M \oplus M'$ sao cho $g(x, y) = (f(x), 0, y)$, khi đó có một biểu đồ giao hoán
$$
\begin{array}{ccc}
M & \xrightarrow{f} & N \\
j \downarrow & & j' \downarrow \\
P & \xrightarrow{g} & N \oplus P
\end{array}
$$

trong đó các mũi tên dọc là các đơn cấu chính tắc. Vì $g$ là đơn ánh và $P$ là tự do, $\Lambda(g)$ là một đồng cấu đơn cấu như đã thấy ở trên. Bây giờ, $\Lambda(j): \Lambda(M) \to \Lambda(P)$ là một đồng cấu đơn cấu vì $M$ là một nhân tử trực tiếp của $P$ (no. 2). Do đó đồng cấu hợp thành

$$
\Lambda(M) \xrightarrow{\Lambda(j)} \Lambda(P) \xrightarrow{\Lambda(g)} \Lambda(N \oplus P)
$$

là đơn ánh và, vì nó cũng bằng đồng cấu hợp thành

$$
\Lambda(M) \xrightarrow{\Lambda(f)} \Lambda(N) \xrightarrow{\Lambda(g')} \Lambda(N \oplus P)
$$

nên ta kết luận rằng $\Lambda(f)$ là đơn ánh.

#### Mệnh đề 13 {#alg-iii-s7-prop-13 .statement}

*Cho $M$ là một $A$-môđun, $N$ là một môđun con hạng tử trực tiếp của $M$ tự do có chiều $p$ và $\{u\}$ là một cơ sở của $\Lambda^p(N)$. Để một phần tử $x \in M$ thuộc $N$, cần và đủ là $u \wedge x = 0$.*

Cho $P$ là một môđun con của $M$ bổ sung cho $N$ và cho $y \in N,\ z \in P$ sao cho $x = y + z$. Khi đó $u \wedge x = u \wedge z$. Vì $\Lambda^p(N)$ là tự do có chiều 1, ánh xạ $\phi: P \to P \otimes \Lambda^p(N)$ sao cho $\phi(p) = p \otimes u$ là song ánh (II, § 3, no. 4, Mệnh đề 4). Mặt khác (no. 7, Mệnh đề 10), hợp thành của các đồng cấu chính tắc

$$
\psi: P \otimes \Lambda^p(N) \to \Lambda(P) \otimes \Lambda(N) \to \Lambda(M)
$$

là đơn ánh. Do đó ánh xạ $\psi \circ \phi$ là đơn ánh, suy ra mệnh đề.

#### Định lý 2 {#alg-iii-s7-thm-2 .statement}

*Cho $M$ là một $A$-môđun có một cơ sở hữu hạn $(e_i)_{1 \leq i \leq n}$. Đối với một dãy $(x_i)_{1 \leq i \leq n}$ gồm $n$ phần tử của $M$ để lập thành một cơ sở của $M$, cần và đủ là phần tử $\lambda \in A$ sao cho

$$
x_1 \wedge x_2 \wedge \ldots \wedge x_n = \lambda \cdot e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$

khả nghịch trong $A$. \*

Nhắc lại rằng $e_1 \wedge e_2 \wedge \cdots \wedge e_n$ là phần tử duy nhất của một cơ sở của $\Lambda^n(M)$ (no. 8, Hệ quả 1 của Định lý 1), do đó phần tử $\lambda \in A$ thỏa mãn (23) được xác định duy nhất. Nếu $(x_i)_{1 \leq i \leq n}$ là một cơ sở của $M$, thì $x_1 \wedge x_2 \wedge \cdots \wedge x_n$ là phần tử duy nhất của một cơ sở của $\Lambda^n(M)$ (no. 8), khi đó $\lambda$ khả nghịch. Ngược lại, giả sử $\lambda$ khả nghịch; khi đó dạng $n$-tuyến tính phản xứng $f$ tương ứng với ánh xạ tuyến tính $g: \Lambda^n(M) \to A$ sao cho

$$
g(e_1 \wedge e_2 \wedge \cdots \wedge e_n) = \lambda^{-1}
$$

thì thỏa mãn $f(x_1, x_2, \ldots, x_n) = 1$. Với mọi $x \in M$, hiển nhiên

$$
x \wedge x_1 \wedge \cdots \wedge x_n = 0
$$

(no. 3, Mệnh đề 6); áp dụng no. 8, Hệ quả 3 của Định lý 1, ta được

$$
f(x_1, x_2, \ldots, x_n) \cdot x = \sum_{i=1}^n (-1)^{i-1} f(x, x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i.
$$

Vì $f(x_1, \ldots, x_n) = 1$, điều này cho thấy mọi $x \in M$ là một tổ hợp tuyến tính của $x_1, x_2, \ldots, x_n$ và, vì các phần tử sau độc lập tuyến tính (do

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0),
$$

chúng lập thành một cơ sở của $M$.

### Bài tập {#alg-iii-s7-exercises}

Xem các [bài tập của § 7](exercises/s7/).
