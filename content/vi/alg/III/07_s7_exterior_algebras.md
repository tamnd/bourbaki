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
book_pages: 507-522, 633-637
pdf_pages: 0531-0546, 0657-0661
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE EXTERIOR ALGEBRA OF A MODULE
      page: 507
      pdf_page: 531
    - "no": 2
      title: Functorial properties of the exterior algebra
      page: 508
      pdf_page: 532
    - "no": 3
      title: ANTICOMMUTATIVITY OF THE EXTERIOR ALGEBRA
      page: 510
      pdf_page: 534
    - "no": 4
      title: '*n*-th EXTERIOR POWER OF A MODULE AND ALTERNATING MULTILINEAR MAPPINGS'
      page: 511
      pdf_page: 535
    - "no": 5
      title: EXTENSION OF THE RING OF SCALARS
      page: 513
      pdf_page: 537
    - "no": 6
      title: DIRECT LIMITS OF EXTERIOR ALGEBRAS
      page: 514
      pdf_page: 538
    - "no": 7
      title: EXTERIOR ALGEBRA OF A DIRECT SUM. EXTERIOR ALGEBRA OF A GRADED MODULE
      page: 515
      pdf_page: 539
    - "no": 8
      title: EXTERIOR ALGEBRA OF A FREE MODULE
      page: 517
      pdf_page: 541
    - "no": 9
      title: CRITERIA FOR LINEAR INDEPENDENCE
      page: 519
      pdf_page: 543
statements: 31
exercises: 15
content_sha256: a85bdaefd42957f8fd00237d59037c1f0ec3ed049a7324d67dac382722b052d2
translated_from: content/en/alg/III/07_s7_exterior_algebras.md
source_content_sha256: c5c58d36fea84ed5e26883e391f20cf1b187d6e1a3de33d7c9e483038c5c4be1
translation_model: gpt-5.4
translation_run: translate-vi-ad8b440c
glossary_version: 34
glossary_terms_sha256: 9f1e10c30a591b7118cb2afe31617ed956382a0f8f1494a43de7f075949362e5
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. ĐẠI SỐ NGOÀI

### 1. ĐỊNH NGHĨA ĐẠI SỐ NGOÀI CỦA MỘT MÔĐUN

#### Định nghĩa 1 {#alg-iii-s7-def-1 .statement}

Cho $A$ là một vành giao hoán và $M$ là một $A$-môđun. Đại số ngoài của $M$, ký hiệu bởi $\bigwedge(M)$ hoặc $\mathrm{Alt}(M)$ hoặc $\bigwedge_A(M)$, là đại số trên $A$ bằng thương của đại số tenxơ $T(M)$ theo iđêan hai phía $\mathfrak{J}''$ (cũng ký hiệu là $\mathfrak{J}_{M}''$) sinh bởi các phần tử $x \otimes x$, trong đó $x$ chạy qua $M$.

Vì iđêan $\mathfrak{J}''$ được sinh bởi các phần tử thuần nhất bậc 2, nó là một iđêan phân bậc (II, § 11, no. 3, Mệnh đề 2); ta viết $\mathfrak{J}_n'' = \mathfrak{J}'' \cap T^n(M)$; do đó đại số $\bigwedge(M)$ được phân bậc bởi phân bậc (gọi là chính tắc) gồm các $\bigwedge^n(M) = T^n(M)/\mathfrak{J}_n''$. Khi đó $\mathfrak{J}_0'' = \mathfrak{J}_1'' = \{0\}$ và vì thế $\bigwedge^0(M)$ được đồng nhất với $A$ và $\bigwedge^1(M)$ với $T^1(M) = M$; trong phần tiếp theo, ta sẽ luôn thực hiện các sự đồng nhất này và đơn ánh chính tắc $M \to \bigwedge(M)$ sẽ được ký hiệu bởi $\phi''$ hoặc $\phi_M''$.

#### Mệnh đề 1 {#alg-iii-s7-prop-1 .statement}

Cho $E$ là một $A$-đại số và $f : M \to E$ là một ánh xạ $A$-tuyến tính sao cho
$$
(f(x))^2 = 0 \quad \text{với mọi } x \in M.
$$
Tồn tại duy nhất một đồng cấu đại số $A$ $g : \bigwedge(M) \to E$ sao cho $f = g \circ \phi''$.

Nói cách khác, $(\bigwedge(M), \phi'')$ là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết tập hợp, IV, § 3, no. 1), trong đó $\Sigma$ là loài các cấu trúc $A$-đại số, còn các ánh xạ $\alpha$ là các ánh xạ tuyến tính từ $A$-môđun $M$ tới một $A$-đại số thỏa mãn (1).

Tính duy nhất của $g$ suy ra từ việc $\phi''(M) = M$ sinh ra $\bigwedge(M)$. Để chứng minh sự tồn tại của $g$, ta nhận thấy rằng theo § 5, no. 1, Mệnh đề 1 tồn tại một đồng cấu đại số $A$ $g_1 : T(M) \to E$ sao cho $f = g_1 \circ \phi$; ta cần chứng minh rằng $g_1$ bằng không trên iđêan $\mathfrak{J}''$, vì khi đó nếu
$$
p : T(M) \to \bigwedge(M) = T(M)/\mathfrak{J}''
$$
là đồng cấu chính tắc, ta có thể viết $g_1 = g \circ p$, trong đó $g : \bigwedge(M) \to E$ là một đồng cấu đại số và kết luận sẽ suy ra từ việc $p \circ \phi = \phi''$. Thật vậy, hạt nhân của $g_1$ là một iđêan hai phía mà, theo (1) và quan hệ $g_1 \circ \phi = f$, chứa các phần tử $x \otimes x$ với $x \in M$. Điều này hoàn tất chứng minh.

#### Nhận xét {#alg-iii-s7-n1-rem-1 .statement}

(1) Giả sử E là một đại số trên A phân bậc kiểu $\mathbf{Z}$, có phân bậc $(E_n)$, và giả sử thêm rằng ánh xạ tuyến tính $f$ (được giả thiết thỏa mãn (1)) sao cho
$$
f(M) \subset E_1.
$$
Khi đó quan hệ $g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p)$ với $x_i \in M$ cho thấy rằng $g(\bigwedge^p(M)) \subset E_p$ với mọi $p \geq 0$ và do đó $g$ là một đồng cấu đại số phân bậc.

(2) Để tránh nhầm lẫn, tích của hai phần tử $u, v$ của đại số ngoài $\bigwedge(M)$ thường được ký hiệu là $u \wedge v$ và được gọi là *tích ngoài* của $u$ với $v$. Do đó các phần tử của $\bigwedge^n(M)$ là những tổng của các phần tử dạng $x_1 \wedge x_2 \wedge \cdots \wedge x_n$ với $x_i \in M$ đối với $1 \leq i \leq n$ và thường được gọi là *n-vectơ*.

### 2. Các tính chất hàm tử của đại số ngoài

#### Mệnh đề 2 {#alg-iii-s7-prop-2 .statement}

*Cho $A$ là một vành giao hoán, $M$ và $N$ là hai $A$-môđun và $u : M \to N$ là một ánh xạ $A$-tuyến tính. Tồn tại một và chỉ một đồng cấu đại số trên $A$*
$$
u'' : \bigwedge(M) \to \bigwedge(N)
$$
*để cho biểu đồ*

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi_M'' & & \downarrow \phi_N'' \\
\bigwedge(M) & \xrightarrow{u''} & \bigwedge(N)
\end{array}
$$

*là giao hoán. Hơn nữa, $u''$ là một đồng cấu đại số phân bậc.*

Sự tồn tại và tính duy nhất của $u'$ suy ra từ no. 1, Mệnh đề 1 áp dụng cho đại số $\bigwedge(N)$ và $f = \phi_N'' \circ u : M \to \bigwedge(N)$; thật vậy, $f(M) \subset N$ và do đó $f$ thỏa mãn điều kiện (1) theo định nghĩa của $\mathfrak{g}_N''$: vì $f(M) \subset \bigwedge^1(N) = N$, việc $u''$ là một đồng cấu đại số phân bậc suy ra từ *Nhận xét* 1 của no. 1.

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

là giao hoán.

Vì $\Lambda(M)$ chứa $M = \Lambda^1(M)$, $\Lambda(u)$ đôi khi được gọi là mở rộng chính tắc của $u$ tới $\Lambda(M)$. Hạn chế $\Lambda^n(u): \Lambda^n(M) \to \Lambda^n(N)$ sao cho
$$
\Lambda^n(u)(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n)
$$
với $x_i \in M$, vì $\Lambda(u)$ là một đồng cấu đại số và $\Lambda^1(u) = u$; hạn chế $\Lambda^0(u)$ trên $A$ là ánh xạ đồng nhất. Chú ý rằng $\Lambda^n(u)$ thu được từ $T^n(u): T^n(M) \to T^n(N)$ bằng cách chuyển qua các thương.

#### Mệnh đề 3 {#alg-iii-s7-prop-3 .statement}

*Nếu $u: M \to N$ là một ánh xạ $A$-tuyến tính toàn ánh, thì đồng cấu $\Lambda(u): \Lambda(M) \to \Lambda(N)$ là toàn ánh và hạt nhân của nó là iđêan hai phía của $\Lambda(M)$ sinh bởi hạt nhân $P \subset M \subset \Lambda(M)$ của $u$.

Chứng minh được dẫn xuất từ chứng minh của § 6, no. 2, Mệnh đề 4, thay thế $S$ bằng $\Lambda$ và $\mathfrak{g}'$ bằng $\mathfrak{g}''$.

Nếu $u: M \to N$ là một ánh xạ tuyến tính đơn ánh, thì không phải bao giờ cũng đúng rằng $\Lambda(u)$ là một ánh xạ đơn ánh (§ 6, Bài tập 3) (tuy nhiên xem dưới đây no. 9, Hệ quả của Mệnh đề 12). Tuy nhiên điều đó đúng khi $u$ là một đơn ánh sao cho $u(M)$ là một nhân tử trực tiếp của $N$, và khi đó ảnh của $\Lambda(u)$ (đẳng cấu với $\Lambda(M)$) là một nhân tử trực tiếp của $\Lambda(N)$; chứng minh giống như chứng minh của các khẳng định tương tự đối với $T(u)$ (§ 5, no. 2), thay thế $T$ bằng $\Lambda$.

#### Mệnh đề 4 {#alg-iii-s7-prop-4 .statement}

*Cho $N$ và $P$ là hai môđun con của một $A$-môđun $M$ sao cho tổng của chúng $N + P$ là một nhân tử trực tiếp trong $M$ và giao của chúng $N \cap P$ là một nhân tử trực tiếp trong $N$ và trong $P$. Khi đó các đồng cấu $\Lambda(N) \to \Lambda(M)$, $\Lambda(P) \to \Lambda(M)$ và $\Lambda(N \cap P) \to \Lambda(M)$, là các mở rộng chính tắc của các đơn ánh chính tắc, đều là đơn ánh; nếu $\Lambda(N)$, $\Lambda(P)$ và $\Lambda(N \cap P)$ được đồng nhất với các đại số con của $\Lambda(M)$ bằng các đồng cấu ấy, thì*
$$
\Lambda(N \cap P) = \Lambda(N) \cap \Lambda(P).
$$
Chứng minh được dẫn xuất từ chứng minh của § 5, no. 2, Mệnh đề 4 bằng cách thay thế $T$ bởi $\Lambda$ ở mọi chỗ. Các giả thiết của Mệnh đề 4 luôn được thỏa mãn đối với các môđun con tùy ý $N, P$ của $M$ khi $A$ là một trường.

#### Hệ quả {#alg-iii-s7-n2-cor-1 .statement}

*Cho $K$ là một trường giao hoán và $M$ là một không gian vectơ trên $K$. Với mọi phần tử $z \in \Lambda(M)$, tồn tại một không gian con vectơ nhỏ nhất $N$ của $M$ sao cho $z \in \Lambda(N)$ và $N$ là hữu hạn chiều.*

Chứng minh được suy ra từ chứng minh của § 5, no. 2, Hệ quả của Mệnh đề 4 bằng cách thay thế $T$ bởi $\Lambda$ ở mọi chỗ.

$N$ được gọi là không gian con vectơ của $M$ liên kết với phần tử $z$ của $\Lambda(M)$.

### 3. TÍNH PHẢN GIAO HOÁN CỦA ĐẠI SỐ NGOẠI

#### Mệnh đề 5 {#alg-iii-s7-prop-5 .statement}

(i) Cho $(x_i)_{1 \leq i \leq n}$ là một dãy hữu hạn các phần tử của môđun $M$; với mọi phép hoán vị $\sigma$ trong nhóm đối xứng $S_n$,

$$
x_{\sigma(1)} \wedge x_{\sigma(2)} \wedge \cdots \wedge x_{\sigma(n)} = \varepsilon_\sigma \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

trong đó $\varepsilon_\sigma$ ký hiệu chữ ký của phép hoán vị $\sigma$.

(ii) Nếu tồn tại hai chỉ số phân biệt $i, j$ sao cho $x_i = x_j$, thì tích

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

bằng không.

(i) Trước hết, vì $x \wedge x = 0$ với mọi $x \in M$ theo định nghĩa của iđêan $\mathfrak{g}'$, nên cũng vậy, với $x, y$ trong $M$,

$$
x \wedge y + y \wedge x = (x + y) \wedge (x + y) - x \wedge x - y \wedge y = 0.
$$

Điều này thiết lập (6) trong trường hợp $n = 2$. Trường hợp tổng quát khi đó suy ra từ § 4, no. 6, Bổ đề 3.

(ii) Dưới giả thiết của (ii), tồn tại một phép hoán vị $\sigma \in S_n$ sao cho $\sigma(1) = i$ và $\sigma(2) = j$; khi đó vế trái của (6) bằng không đối với phép hoán vị này và vì thế vế phải cũng vậy.

#### Hệ quả 1 {#alg-iii-s7-prop-5-cor-1 .statement}

Cho $H, K$ là hai tập hợp con bù nhau của khoảng $[1, n]$ của $\mathbf{N}$ và cho $(i_h)_{1 \leq h \leq p}, (j_k)_{1 \leq k \leq n-p}$ là các dãy phần tử của $H$ và $K$ tương ứng, được sắp theo thứ tự tăng; ta viết

$$
x_H = x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}, \quad x_K = x_{j_1} \wedge x_{j_2} \wedge \cdots \wedge x_{j_{n-p}};
$$

khi đó

$$
x_H \wedge x_K = (-1)^{\nu} x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

trong đó $\nu$ là số các cặp có thứ tự $(i, j) \in H \times K$ sao cho $i > j$.

Theo Mệnh đề 5, việc này quy về chứng minh

#### Bổ đề 1 {#alg-iii-s7-lem-1 .statement}

Nếu $\sigma \in S_n$ là phép hoán vị sao cho $\sigma(h) = i_h$ với $1 \leq h \leq p$, $\sigma(h) = j_{n-p}$ với $p + 1 \leq h \leq n$, thì $\varepsilon_\sigma = (-1)^\nu$.

Với $1 \leq h < h' \leq p$ hoặc $p + 1 \leq h < h' \leq n$, ta có $\sigma(h') > \sigma(h)$ và số các cặp có thứ tự $(h, h')$ sao cho $1 \leq h \leq p < h' \leq n$ và $\sigma(h) > \sigma(h')$ bằng $\nu$.

#### Hệ quả 2 {#alg-iii-s7-lem-1-cor-2 .statement}

Đại số phân bậc $\bigwedge(M)$ là phản xứng ($§ 4$, no. 9).

Chỉ cần áp dụng Mệnh đề 13 của $§ 4$, no. 9 cho $\bigwedge(M)$, lấy làm hệ sinh tập hợp $M$ và dùng Mệnh đề 5.

#### Mệnh đề 6 {#alg-iii-s7-prop-6 .statement}

*Nếu M là một A-môđun hữu hạn sinh, thì $\bigwedge(M)$ là một A-môđun hữu hạn sinh; hơn nữa, nếu M thừa nhận một hệ sinh gồm n phần tử, thì $\bigwedge^p(M) = \{0\}$ với $p > n$.*

Cho $(x_i)_{1 \leq i \leq n}$ là một hệ sinh của M. Mọi phần tử của $\bigwedge^p(M)$ là một tổ hợp tuyến tính của các phần tử có dạng
$$
x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}
$$
trong đó các chỉ số $i_k$ thuộc $\{1, n\}$; theo Mệnh đề 5, có thể giả sử các chỉ số này phân biệt (nếu không thì phần tử tương ứng bằng không). Nếu $p > n$, thì không có dãy chỉ số như vậy và do đó $\bigwedge^p(M) = \{0\}$. Nếu $p \leq n$, thì các dãy này hữu hạn về số lượng, điều đó hoàn tất chứng minh.

### 4. LŨY THỪA NGOÀI BẬC *n* CỦA MỘT MÔĐUN VÀ CÁC ÁNH XẠ ĐA TUYẾN TÍNH PHẢN XỨNG

Cho hai môđun M, N trên một vành giao hoán A, một ánh xạ *n-tuyến tính phản xứng* của $M^n$ vào N là bất kỳ ánh xạ *n*-tuyến tính nào $f : M^n \to N$ sao cho, với mọi $p \leq n - 2$,
$$
f(u_1, \ldots, u_p, x, x, v_1, \ldots, v_{n-p-2}) = 0
$$
với mọi x, các $u_i$ ($1 \leq i \leq p$) và các $v_j$ ($1 \leq j \leq n - p - 2$) trong M.

#### Mệnh đề 7 {#alg-iii-s7-prop-7 .statement}

*Cho A là một vành giao hoán và M và N là hai A-môđun. Nếu với mỗi ánh xạ A-tuyến tính* $g : \bigwedge^n(M) \to N$ ($n \geq 2$) *ta liên kết ánh xạ n-tuyến tính*
$$
(x_1, x_2, \ldots, x_n) \mapsto g(x_1 \wedge x_2 \wedge \cdots \wedge x_n)
$$
*thì thu được một ánh xạ A-tuyến tính song ánh của A-môđun $\operatorname{Hom}_A(\bigwedge^n(M), N)$ lên A-môđun các ánh xạ n-tuyến tính phản xứng của $M^n$ vào N.*

Ta xét song ánh chính tắc của A-môđun $\operatorname{Hom}_A(T^n(M), N)$ lên A-môđun $\mathcal{L}_n(M, \ldots, M; N)$ gồm *mọi* ánh xạ n-tuyến tính của $M^n$ vào N, thu được bằng cách liên kết với mỗi ánh xạ A-tuyến tính $f : T^n(M) \to N$ ánh xạ n-tuyến tính
$$
\tilde{f} : (x_1, \ldots, x_n) \mapsto f(x_1 \otimes x_2 \otimes \cdots \otimes x_n)
$$
(II, § 3, no. 9). Mặt khác, các ánh xạ A-tuyến tính $g : \bigwedge^n(M) \to N$ tương ứng một-một với các ánh xạ A-tuyến tính $f : T^n(M) \to N$ sao cho *f bằng không trên $\mathfrak{g}_n''$*, bằng cách liên kết với g ánh xạ $f = g \circ p_n$, trong đó
$$
p_n : T^n(M) \to \bigwedge^n(M) = T^n(M)/\mathfrak{g}_n''
$$

là đồng cấu chính tắc (II, § 2, no. 1, Định lý 1). Nhưng vì $\mathfrak{J}_n''$ là một tổ hợp tuyến tính của các phần tử có dạng
$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_p) \otimes (x \otimes x) \otimes (v_1 \otimes \cdots \otimes v_{n-p-2})
$$
$(x, u_i, v_j$ trong $M$), nên việc nói rằng $f$ có dạng $g \circ p_n$ có nghĩa là hàm $n$-tuyến tính tương ứng $\bar{f}$ thỏa mãn (8), nói cách khác, nó là *phản xứng*.

A-môđun $\bigwedge^n(M)$ được gọi là *lũy thừa ngoài bậc n* của M. Với mọi đồng cấu A-môđun $u : M \to N$, ánh xạ
$$
\bigwedge^n(u) : \bigwedge^n(M) \to \bigwedge^n(N)
$$
trùng với $\bigwedge(u)$ trên $\bigwedge^n(M)$ được gọi là *lũy thừa ngoài bậc n của u*.

#### Hệ quả 1 {#alg-iii-s7-prop-7-cor-1 .statement}

*Với mọi ánh xạ n-tuyến tính phản xứng* $g : M^n \to N$, *với mọi phép hoán vị* $\sigma \in \mathfrak{S}_n$,
$$
g(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(n)}) = \varepsilon_\sigma \cdot g(x_1, x_2, \ldots, x_n)
$$
*với mọi* $x_i \in M$; *hơn nữa nếu* $x_i = x_j$ *với hai chỉ số phân biệt* $i, j$, *thì*
$$
g(x_1, x_2, \ldots, x_n) = 0.
$$
Đây là một hệ quả hiển nhiên của Mệnh đề 7 và no. 3, Mệnh đề 5.

#### Hệ quả 2 {#alg-iii-s7-prop-7-cor-2 .statement}

*Cho* $(x_i)_{1 \leq i \leq n}$ *là một dãy gồm n phần tử của M sao cho*
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0;
$$
*khi đó, với mọi ánh xạ n-tuyến tính phản xứng* $g : M^n \to N$, $g(x_1, \ldots, x_n) = 0$.

#### Hệ quả 3 {#alg-iii-s7-prop-7-cor-3 .statement}

*Cho* $f : M^{n-1} \to A$ *là một dạng* $(n-1)$*-tuyến tính phản xứng*. *Nếu* $(x_i)_{1 \leq i \leq n}$ *là một dãy gồm n phần tử của M sao cho* $x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0$, *thì*
$$
\sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i = 0
$$
*(trong đó ta viết* $f(x_1, \ldots, \hat{x}_i, \ldots, x_n) = f(x_1, \ldots, x_{i-1}, x_{i+1}, \ldots, x_n)$ *với* $1 \leq i \leq n$.

Chỉ cần chứng minh rằng ánh xạ $n$-tuyến tính
$$
(x_1, \ldots, x_n) \mapsto \sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i
$$
từ $M^n$ vào $M$ là *phản xứng*. Thật vậy, nếu $x_i = x_{i+1}$, thì mọi hạng trong tổng ở vế phải đều có hệ số bằng không, trừ $x_i$ và $x_{i+1}$, vì $f$ là phản xứng; mặt khác, hệ số của $x_i$ là
$$
(-1)^i f(x_1, \ldots, x_{i-1}, x_{i+1}, x_{i+2}, \ldots, x_n)
$$

và hệ số của $x_{i+1}$ là $(-1)^{i+1} f(x_1, \ldots, x_i, x_{i+2}, \ldots, x_n)$, và theo giả thiết chúng đối nhau.

#### Nhận xét {#alg-iii-s7-n4-rem-1 .statement}

Một phần tử $z$ của $T^n(M)$ được gọi là một tenxơ *phản đối xứng bậc* $n$ (phản biến) nếu $\sigma.z = \varepsilon_\sigma z$ với mọi phép hoán vị $\sigma \in S_n$ (x. § 6, no. 3, Nhận xét); các phần tử ấy tạo thành một A-môđun con $A'_n(M)$ của $T^n(M)$. Với mọi $z \in T^n(M)$, ta đặt $a.z = \sum_{\sigma \in S_n} \varepsilon_\sigma(\sigma.z)$ và gọi $a.z$ là *phản đối xứng hóa* của $z$; do $\varepsilon_{\sigma\tau} = \varepsilon_\sigma \varepsilon_\tau$, thấy ngay lập tức rằng $a.z$ là một tenxơ phản đối xứng và vì vậy $z \mapsto a.z$ là một tự đồng cấu của $T^n(M)$ mà ảnh $A''_n(M)$ của nó được chứa trong $A'_n(M)$; nói chung $A''_n(M) \neq A'_n(M)$ (Bài tập 8). Nếu $z$ là một tenxơ phản đối xứng, thì $a.z = n!z$; do đó, *khi* $n!$ *khả nghịch trong* $A$, tự đồng cấu $z \mapsto (n!)^{-1}a.z$ là một *phép chiếu* của $T^n(M)$ mà ảnh là

$$
A'_n(M) = A''_n(M).
$$

Hơn nữa, *hạt nhân* của phép chiếu này chính là $\mathfrak{J}_n''$; vì hiển nhiên có thể chỉ cần xét trường hợp $n \geqslant 2$, nên 2 (một ước của $n!$) khả nghịch trong $A$ và $x \otimes x = 2^{-1}(x \otimes x + x \otimes x)$; do đó $\mathfrak{J}_n''$ được sinh bởi các phần tử $z + \rho.z$, trong đó $\rho$ là một phép đổi chỗ hoán đổi hai số liên tiếp trong $\{1, n\}$; hơn nữa, với hai phép hoán vị $\sigma, \tau$ trong $S_n$, ta có thể viết

$$
z - \varepsilon_{\sigma\tau}((\sigma\tau).z) = z - \varepsilon_\tau(\tau.z) + \varepsilon_\tau(\tau.z - \varepsilon_\sigma \sigma.(\tau.z))
$$

do đó suy ra rằng $z - \varepsilon_\sigma(\sigma.z) \in \mathfrak{J}_n''$ với mọi $z \in T^n(M)$ và $\sigma \in S_n$. Vì vậy (vẫn giả sử rằng $n!$ khả nghịch trong $A$), ta thấy rằng

$$
z - (n!)^{-1}a.z = \sum_{\sigma \in S_n} (n!)^{-1}(z - \varepsilon_\sigma(\sigma.z)) \in \mathfrak{J}_n''
$$

với mọi $z \in T^n(M)$, điều này chứng minh mệnh đề đã nêu.

Khi $n!$ khả nghịch trong $A$, các môđun con $A'_n(M)$ và $\mathfrak{J}_n''$ của $T^n(M)$ do đó là *bù nhau* và hạn chế trên $A'_n(M)$ của đồng cấu chính tắc $T^n(M) \to \bigwedge^n(M) = T^n(M)/\mathfrak{J}_n''$ là một A-môđun *đẳng cấu*, điều này cho phép ta trong trường hợp đang xét đồng nhất các tenxơ phản đối xứng cấp $n$ với các phần tử của lũy thừa ngoài thứ $n$ của $M$. Ở đây cũng chú ý rằng sự đồng nhất này không tương thích với phép nhân, vì tích trong $T(M)$ của hai tenxơ phản đối xứng nói chung không phản đối xứng.

### 5. MỞ RỘNG VÀNH VÔ HƯỚNG

Cho $A, A'$ là hai vành giao hoán, $\rho : A \to A'$ là một đồng cấu vành, $M$ là một $A$-môđun, $M'$ là một $A'$-môđun và $f : M \to M'$ là một *A-đồng cấu* (đối với $\rho$) của $M$ vào $M'$. Ánh xạ hợp thành $M \xrightarrow{f} M' \xrightarrow{\phi_{M'}} \bigwedge_{A'}(M')$ là một ánh xạ A-tuyến tính của $M$ vào đại số trên A $\bigwedge_{A'}(M')$ và, vì các phần tử của f(M) ⊂ M' có bình phương bằng không trong $\bigwedge_{A'}(M')$, tồn tại (no. 1, Mệnh đề 1) một và chỉ một $A$-đồng cấu đại số $f'' : \bigwedge_A(M) \to \bigwedge_{A'}(M')$ làm cho biểu đồ

$$
\begin{array}{ccc}
M & \xrightarrow{f} & M' \\
\downarrow \phi_M'' & & \downarrow \phi_{M'}'' \\
\bigwedge_A(M) & \xrightarrow{f''} & \bigwedge_{A'}(M')
\end{array}
$$

giao hoán, và $f''$ là một đồng cấu đại số phân bậc. Ngay lập tức suy ra rằng nếu $\sigma : A' \to A''$ là một đồng cấu vành khác, $M''$ là một $A''$-môđun, $g : M' \to M''$ là một $A'$-đồng cấu (đối với $\sigma$) và $g'' : \bigwedge_{A'}(M') \to \bigwedge_{A''}(M'')$ là đồng cấu đại số $A''$ tương ứng, thì $A$-đồng cấu đại số hợp thành

$$
\bigwedge_A(M) \xrightarrow{f''} \bigwedge_{A'}(M') \xrightarrow{g''} \bigwedge_{A''}(M'')
$$

tương ứng với $A$-đồng cấu hợp thành $g \circ f : M \to M''$ (đối với $\sigma \circ \rho$).

#### Mệnh đề 8 {#alg-iii-s7-prop-8 .statement}

*Cho $A, B$ là hai vành giao hoán, $\rho : A \to B$ là một đồng cấu vành và $M$ là một $A$-môđun. Mở rộng chính tắc*

$$
\psi : \bigwedge_B(B \otimes_A M) \to B \otimes_A \bigwedge_A(M)
$$

*của ánh xạ* $B$-*tuyến tính* $1_B \otimes \phi_M'' : B \otimes_A M \to B \otimes_A \bigwedge_A(M)$ *là một đẳng cấu đại số* $B$-*phân bậc.*

Chứng minh được dẫn xuất từ chứng minh của § 5, no. 4, Mệnh đề 5 khi thay thế $T$ bởi $\bigwedge$ và $\phi_M$ bởi $\phi_M''$.

### 6. GIỚI HẠN TRỰC TIẾP CỦA CÁC ĐẠI SỐ NGOÀI

Cho $(A_\alpha, \phi_{\beta \alpha})$ là một hệ trực tiếp có hướng các vành giao hoán, $(M_\alpha, f_{\beta \alpha})$ là một hệ trực tiếp các $A_\alpha$-môđun, $A = \lim \to A_\alpha$ và $M = \lim \to M_\alpha$. Với $\alpha \leq \beta$, từ đồng cấu $A_\alpha$-môđun $f_{\beta \alpha} : M_\alpha \to M_\beta$ ta suy ra một cách chính tắc một đồng cấu đại số $A_\alpha$ (no. 5, công thức (12)) $f_{\beta \alpha}' : \bigwedge_{A_\alpha}(M_\alpha) \to \bigwedge_{A_\beta}(M_\beta)$ và từ (13) suy ra rằng $(\bigwedge_{A_\alpha}(M_\alpha), f_{\beta \alpha}')$ là một *hệ trực tiếp các* $A_\alpha$*-môđun phân bậc*. Mặt khác, cho $f_\alpha : M_\alpha \to M$ là đồng cấu chính tắc $A_\alpha$; ta suy ra (no. 5, công thức (12)) một đồng cấu đại số phân bậc $A_\alpha$ $f_\alpha'' : \bigwedge_{A_\alpha}(M_\alpha) \to \bigwedge_A(M)$ và từ (13) cũng suy ra rằng các $f_\alpha''$ cấu thành một hệ trực tiếp các đồng cấu $A_\alpha$.

#### Mệnh đề 9 {#alg-iii-s7-prop-9 .statement}

*Đồng cấu A* $f'' = \varprojlim f''_\alpha : \varprojlim \Lambda_{A_\alpha}(M_\alpha) \to \Lambda_A(M)$ *là một đẳng cấu đại số phân bậc*.

Chứng minh giống như chứng minh của § 5, no. 4, Mệnh đề 6, thay khắp nơi T bằng $\Lambda$ và $\phi$ bằng $\phi''$, đồng thời lưu ý rằng giới hạn trực tiếp của các đại số phản xứng là phản xứng.

### 7. ĐẠI SỐ NGOẠI CỦA MỘT TỔNG TRỰC TIẾP. ĐẠI SỐ NGOẠI CỦA MỘT MÔĐUN PHÂN BẬC

Cho A là một vành giao hoán, $M = \bigoplus_{\lambda \in L} M_\lambda$ là tổng trực tiếp của một họ các A-môđun và $j_\lambda : M_\lambda \to M$ là đơn ánh chính tắc; ta suy ra một đồng cấu A của các đại số phân bậc $\Lambda(j_\lambda) : \Lambda(M_\lambda) \to \Lambda(M)$. Vì $\Lambda(M)$ là phản giao hoán, nên có thể áp dụng Mệnh đề 10 của § 4, no. 7 (hoặc nếu cần thì tổng quát hóa cho trường hợp L là vô hạn, cf. § 4, no. 8, *Nhận xét* 1) cho các đồng cấu $\Lambda(j_\lambda)$; khi đó tồn tại một và chỉ một đồng cấu đại số

$$
g : \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda) \to \Lambda(M)
$$

(cũng được ký hiệu bởi $g_M$) sao cho $\Lambda(j_\lambda) = g \circ f_\lambda$, trong đó

$$
f_\lambda : \Lambda(M_\lambda) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)
$$

ký hiệu đồng cấu chính tắc.

#### Mệnh đề 10 {#alg-iii-s7-prop-10 .statement}

*Đồng cấu chính tắc* g (*công thức (14)*) *là một đẳng cấu đại số phân bậc*.

Để chứng minh rằng g là song ánh, ta định nghĩa một đồng cấu đại số phân bậc

$$
h : \Lambda(M) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)
$$

sao cho $g \circ h$ và $h \circ g$ lần lượt là các ánh xạ đồng nhất trên $\Lambda(M)$ và $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$. Với mỗi $\lambda \in L$, xét ánh xạ tuyến tính hợp thành

$$
u_\lambda : M_\lambda \xrightarrow{\phi''_{M_\lambda}} \Lambda(M_\lambda) \xrightarrow{f_\lambda} \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda).
$$

Tồn tại một và chỉ một ánh xạ A-tuyến tính $u : M \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$ sao cho $u \circ j_\lambda = u_\lambda$ với mọi $\lambda \in L$. Tích tenxơ lệch $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \Lambda(M_\lambda)$ là một đại số *phản xứng*: thật vậy, khi L hữu hạn, điều này suy ra từ § 4, no. 9, Mệnh đề 14, và khi L tùy ý, điều này suy ra từ định nghĩa của tích này đã cho trong § 4, no. 8, *Nhận xét* 1 và từ sự kiện rằng giới hạn trực tiếp của các đại số phân bậc phản xứng là phản xứng. Vì $u(M)$ cũng được chứa trong môđun con các phần tử bậc 1 của đại số phân bậc $\bigotimes_{\lambda \in L} \Lambda(M_\lambda)$, nên từ no. 1, Mệnh đề 1 và *Nhận xét* 1 suy ra rằng tồn tại một đồng cấu đại số phân bậc duy nhất

$$
h : \Lambda(M) \to \bigotimes_{\lambda \in L} \Lambda(M_\lambda)
$$

sao cho $h \circ \phi''_M = u$. Việc kiểm tra rằng $g \circ h$ và $h \circ g$ là các ánh xạ đồng nhất khi đó được thực hiện như trong § 6, no. 6, Mệnh đề 9, thay $S$ bằng $\Lambda$ và $\phi'$ bằng $\phi''$.

#### Nhận xét {#alg-iii-s7-n7-rem-1 .statement}

Cho $N = \bigoplus_{\lambda \in L} N_\lambda$ là tổng trực tiếp của một họ khác các $A$-môđun với L làm tập hợp chỉ số và, với mọi $\lambda \in L$, cho $v_\lambda : M_\lambda \to N_\lambda$ là một ánh xạ $A$-tuyến tính, do đó có một ánh xạ $A$-tuyến tính $v = \bigoplus_\lambda v_\lambda : M \to N$ (II, § 1, no. 6, Mệnh đề 7). Khi đó biểu đồ

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

A-môđun con của $\bigotimes_{\lambda \in L} \Lambda(M_\lambda)$ mà với nó $\Lambda^n(M)$ được đồng nhất nhờ đẳng cấu $g$ có thể được mô tả chính xác hơn. Với mọi tập con hữu hạn $J$ của $L$, ta viết $E_J = \bigotimes_{\lambda \in J} \Lambda(M_\lambda)$, sao cho $\bigotimes_{\lambda \in L} \Lambda(M_\lambda) = \lim \to E_J$ đối với tập có hướng $\mathcal{F}(L)$ các tập con hữu hạn của $L$, theo định nghĩa ($§ 4$, no. 8, *Nhận xét* 1). Với mọi họ $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$ (do đó có giá *hữu hạn* khác không) sao cho $\sum_{\lambda \in L} n_\lambda = n$ và mọi tập con hữu hạn $J$ của $L$ chứa giá của họ $\nu$, ta viết

$$
\Lambda^{J,\nu}(M) = \bigotimes_{\lambda \in J} \Lambda^{n_\lambda}(M_\lambda)
$$

sao cho môđun con $E_{J,n}$ gồm các phần tử bậc $n$ trong $E_J$ là *tổng trực tiếp* của các $\Lambda^{J,\nu}(M)$ với mọi họ $\nu$ có giá được chứa trong $J$ và sao cho

$$
\sum_{\lambda \in L} n_\lambda = n
$$

($§ 4$, no. 7, Mệnh đề 10 và no. 8). Theo quy ước ta viết $\Lambda^{J,\nu}(M) = \{0\}$ đối với các họ $\nu$ mà giá của chúng không được chứa trong $J$; khi đó

E_{J,n} cũng có thể được gọi là tổng trực tiếp của tất cả các $\bigwedge^{J,\nu}(M)$, trong đó $\nu$ chạy qua tập hợp $H_n$ của mọi họ $\nu = (n_\lambda)_{\lambda \in L}$ sao cho $\sum_{\lambda \in L} n_\lambda = n$. Vì $\bigwedge^0(M_\lambda)$ được đồng nhất với $A$, nên rõ ràng cũng vậy, với hai tập con hữu hạn $J \subset J'$ của $L$ và một họ $\nu$ có giá được chứa trong $J$, ánh xạ chính tắc $\bigwedge^{J,\nu}(M) \to \bigwedge^{J',\nu}(M)$ (hạn chế của ánh xạ chính tắc $E_J \to E_{J'}$ lên $\bigwedge^{J,\nu}(M)$) là song ánh. Nếu ta viết, với mọi $\nu \in H_n$,

$$
\bigwedge^\nu(M) = \lim_{\longrightarrow} \bigwedge^{J,\nu}(M)
$$

thì thấy rằng, có lưu ý đến II, § 6, no. 2, Mệnh đề 5, ta có:

#### Hệ quả {#alg-iii-s7-n7-cor-1 .statement}

*A-môđun* $\bigwedge^n(M)$ *là ảnh qua đẳng cấu (14) của môđun con của* $\bigotimes_{\lambda \in L} \bigwedge(M_\lambda)$* là tổng trực tiếp của các môđun con* $\bigwedge^\nu(M)$* với mọi họ* $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$* sao cho* $\sum_{\lambda \in L} n_\lambda = n$; *nếu* $J$* là giá của* $\nu$, $\bigwedge^\nu(M)$* đẳng cấu chính tắc với* $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_\lambda)$.

Nói chung $\bigwedge^\nu(M)$, $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_\lambda)$ và ảnh của chúng trong $\bigwedge^n(M)$ được đồng nhất. Với quy ước này:

#### Mệnh đề 11 {#alg-iii-s7-prop-11 .statement}

*Cho* $\Delta$ *là một monoïde giao hoán, $M$ là một A-môđun phân bậc kiểu $\Delta$ và* $(M_\alpha)_{\alpha \in \Delta}$* *phân bậc của nó. Với mọi cặp có thứ tự* $(\alpha, n) \in \Delta \times \mathbf{N}$, *đặt* $\bigwedge^{\alpha,n}(M)$* *là môđun con của* $\bigwedge^n(M)$* *bằng tổng trực tiếp của các môđun con* $\bigotimes_{\lambda \in J} \bigwedge^{n_\lambda}(M_{\alpha_\lambda})$, *trong đó* $(n_\lambda)_{\lambda \in L}$* *chạy qua tập các họ số nguyên* $\geq 0$* *sao cho* $\sum_{\lambda \in L} n_\lambda = n$, $J$* *là giá của nó và, với mỗi* $(n_\lambda)$, $(\alpha_\lambda)_{\lambda \in J}$* *chạy qua tập các họ của* $\Delta^J$* *sao cho* $\sum_{\lambda \in J} \alpha_\lambda = \alpha$. *Khi đó* $(\bigwedge^{\alpha,n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$* *là phân bậc duy nhất kiểu* $\Delta \times \mathbf{N}$* *tương thích với cấu trúc đại số trên* $\bigwedge(M)$* *và cảm sinh trên* $M = \bigwedge^1(M)$* *phân bậc đã cho.*

Việc $\bigwedge(M)$ là tổng trực tiếp của các $\bigwedge^{\alpha,n}(M)$ suy ra từ Hệ quả của Mệnh đề 10; phần còn lại của chứng minh giống hệt phần cuối của chứng minh ở § 5, no. 5, Mệnh đề 7.

### 8. ĐẠI SỐ NGOÀI CỦA MỘT MÔĐUN TỰ DO

#### Định lý 1 {#alg-iii-s7-thm-1 .statement}

*Cho* $M$* *là một A-môđun có một cơ sở* $(e_\lambda)_{\lambda \in L}$. *Giả sử* $L$* *được trang bị cấu trúc của một tập sắp thứ tự toàn phần* (Set Theory, III, § 2, no. 3, Theorem 1)* *và với mọi tập con hữu hạn* $J$* *của* $L$* *ta viết*

$$
e_J = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}
$$

trong đó $(\lambda_k)_{1 \leq k \leq n}$ là dãy các phần tử của J được sắp theo thứ tự tăng (Set Theory, III, § 5, no. 3, Proposition 6); ta viết $e_\varnothing = 1$, phần tử đơn vị của A. Khi đó các $e_J$, khi J chạy qua tập $\mathcal{F}(L)$ các tập con hữu hạn của L, tạo thành một cơ sở của đại số ngoài $\bigwedge(M)$.

Vì các $e_\lambda$ sinh A-môđun M, mọi phần tử của $\bigwedge(M)$ là một tổ hợp tuyến tính của một số hữu hạn tích của các phần tử $e_\lambda$ và do đó (có tính đến no. 3, Mệnh đề 5) là một tổ hợp tuyến tính của một số hữu hạn phần tử $e_J$ với $J \in \mathcal{F}(L)$. Vậy chỉ còn phải chứng minh rằng các $e_J$ độc lập tuyến tính trên A. Nếu không, sẽ tồn tại giữa các phần tử ấy một quan hệ tuyến tính với các hệ số không phải tất cả đều bằng không; hợp của các tập con J tương ứng với các $e_J$ mà các hệ số của chúng trong quan hệ này là $\neq 0$ là một tập con hữu hạn K của L (vì chỉ có một số hữu hạn hệ số $\neq 0$). Gọi N là môđun con của M sinh bởi các $e_\lambda$ sao cho $\lambda \in K$; N là một nhân tử trực tiếp của M, do đó (no. 2) $\bigwedge(N)$ được đồng nhất với một đại số con của $\bigwedge(M)$ và, nếu ta chỉ ra rằng các $e_J$ với $J \subset K$ tạo thành một cơ sở của $\bigwedge(N)$, thì ta sẽ thu được mâu thuẫn cần tìm.

Do đó điều này quy về việc đưa ra Định lý 1 khi cơ sở của M là hữu hạn; vì vậy ta có thể giả sử rằng $L = \{1, m\} \subset N$. Với mỗi $i \in L$, gọi $M_i$ là môđun con tự do $Ae_i$ của M; M là tổng trực tiếp của các $M_i$ và $\bigwedge(M_i)$ là tổng trực tiếp của $\bigwedge^0(M_i) = A$ và $\bigwedge^1(M_i) = M_i$ (no. 3, Mệnh đề 6). Đồng nhất một cách chính tắc $\bigwedge(M)$ với A-môđun là tích tenxơ của các $\bigwedge(M_i)$ (no. 7, Mệnh đề 10); môđun sau có cơ sở là tích tenxơ của các cơ sở $(1, e_i)$ của các $\bigwedge(M_i)$ (II, § 3, no. 7, Hệ quả 2 của Mệnh đề 7); do đó ta thu được tất cả các phần tử

$$
u_1 \otimes u_2 \otimes \cdots \otimes u_m
$$

trong đó hoặc $u_i = 1$ hoặc $u_i = e_i$; nếu J là tập hợp các chỉ số i sao cho $u_i = e_i$, thì $u_1 \otimes u_2 \otimes \cdots \otimes u_m$ đồng nhất với $e_J$, điều này hoàn tất chứng minh.

#### Hệ quả 1 {#alg-iii-s7-thm-1-cor-1 .statement}

Giả sử rằng $L = \{1, m\}$; khi đó cơ sở $(e_J)_{J \in \mathcal{P}(L)}$ của $\bigwedge(M)$ có $2^m$ phần tử. Với $p > m$, $\bigwedge^p(M) = \{0\}$; $\bigwedge^m(M)$ có một cơ sở gồm một phần tử duy nhất $e_L$; với $0 \leq p \leq m$ số phần tử trong cơ sở $(e_J)$ của $\bigwedge^p(M)$ gồm các $e_J$ sao cho $\mathrm{Card}(J) = p$ là

$$
\binom{m}{p} = \frac{m!}{p!(m-p)!}
$$

Điều này suy ra từ Lý thuyết tập hợp, III, § 3, no. 5, Mệnh đề 12 và Lý thuyết tập hợp, III, § 5, no. 8, Hệ quả 1 của Mệnh đề 11.

Ta quay lại trường hợp mà tập hợp L trong Định lý 1 là tùy ý và cho tường minh bảng phép nhân (§ 1, no. 7) của cơ sở $(e_J)$. Với hai tập con hữu hạn $J, K$ của tập sắp thứ tự toàn phần $L$, ta viết
$$
\begin{cases}
\rho_{J, K} = 0 & \text{nếu } J \cap K \neq \varnothing \\
\rho_{J, K} = (-1)^v & \text{nếu } J \cap K = \varnothing
\end{cases}
$$
trong đó $v$ ký hiệu số các cặp có thứ tự $(\lambda, \mu) \in J \times K$ sao cho $\lambda > \mu$. Khi đó Hệ quả 1 của Mệnh đề 4 ở no. 2 ngay lập tức suy ra quan hệ
$$
e_J \wedge e_K = \rho_{J, K} e_{J \cup K}.
$$
Chú ý công thức
$$
\rho_{J, K} \rho_{K, J} = (-1)^{jk}
$$
khi $J \cap K = \varnothing, j = \mathrm{Card}(J), k = \mathrm{Card}(K)$ (no. 3, Hệ quả 2 của Mệnh đề 5.)

#### Hệ quả 2 {#alg-iii-s7-thm-1-cor-2 .statement}

*Nếu M là một A-môđun xạ ảnh, $\bigwedge(M)$ là một A-môđun xạ ảnh.*

Chứng minh giống như chứng minh của § 5, no. 5, Hệ quả của Định lý 1 khi thay T bằng $\bigwedge$.

#### Hệ quả 3 {#alg-iii-s7-thm-1-cor-3 .statement}

*Cho M là một A-môđun xạ ảnh và $(x_i)_{1 \leq i \leq n}$ một dãy hữu hạn các phần tử của M. Để tồn tại trên M một dạng phản xứng n-tuyến tính f sao cho*
$$
f(x_1, x_2, \ldots, x_n) \neq 0,
$$
*điều kiện cần và đủ là* $x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0$.

Ta đã biết rồi (không có giả thiết nào trên M) rằng điều kiện đó là cần thiết (no. 4, Mệnh đề 7). Bây giờ giả sử rằng M là xạ ảnh và rằng
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0.
$$
Khi đó $\bigwedge^n(M)$ là xạ ảnh (Hệ quả 2) và vì thế ánh xạ chính tắc
$$
\bigwedge^n(M) \to (\bigwedge^n(M))^{**}
$$
là đơn ánh (II, § 2, no. 7, Hệ quả 4 của Mệnh đề 13); ta kết luận rằng tồn tại một dạng tuyến tính $g : \bigwedge^n(M) \to A$ sao cho $g(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \neq 0$. Nếu $f$ là dạng phản xứng n-tuyến tính tương ứng với $g$ (no. 4, Mệnh đề 7), thì $f(x_1, \ldots, x_n) \neq 0$.

### 9. CÁC TIÊU CHUẨN VỀ TÍNH PHỤ THUỘC TUYẾN TÍNH

#### Mệnh đề 12 {#alg-iii-s7-prop-12 .statement}

*Cho M là một A-môđun xạ ảnh. Để các phần tử $x_1, x_2, \ldots, x_n$ của M phụ thuộc tuyến tính, điều kiện cần và đủ là tồn tại $\lambda \neq 0$ trong A sao cho*
$$
\lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0.
$$

Điều kiện là cần thiết (không có giả thiết nào trên M), vì chẳng hạn nếu $\lambda x_1$ (với $\lambda \neq 0$) là một tổ hợp tuyến tính của $x_2, \ldots, x_n$, thì quan hệ (22) được thỏa mãn (no. 3, Mệnh đề 5). Ta sẽ chỉ ra rằng điều kiện là đủ bằng quy nạp theo $n$; với $n = 1$, đó là một hệ quả tầm thường của định nghĩa. Vậy giả sử rằng $n > 1$ và điều kiện (22) được thỏa mãn với một $\lambda \neq 0$ nào đó. Nếu
$$
\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n = 0,
$$
thì giả thiết quy nạp suy ra rằng $x_2, \ldots, x_n$ phụ thuộc tuyến tính và vì thế *a fortiori* $x_1, x_2, \ldots, x_n$ cũng vậy. Nếu $\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n \neq 0$, thì từ no. 8, Hệ quả 3 của Định lý 1 suy ra tồn tại một dạng phản xứng $(n - 1)$-tuyến tính $f$ sao cho $f(\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n) = \mu \neq 0$. Vì
$$
x_1 \wedge (\lambda x_2) \wedge \cdots \wedge x_n = 0,
$$
nên từ no. 8, Hệ quả 3 của Định lý 1 suy ra rằng $\mu x_1$ là một tổ hợp tuyến tính của $\lambda x_2, x_3, \ldots, x_n$; do đó $x_1, x_2, \ldots, x_n$ phụ thuộc tuyến tính.

#### Hệ quả {#alg-iii-s7-n9-cor-1 .statement}

*Cho M và N là hai A-môđun xạ ảnh và $f : M \to N$ là một ánh xạ A-tuyến tính. Nếu f là đơn ánh, thì $\Lambda(f) : \Lambda(M) \to \Lambda(N)$ cũng là đơn ánh.*

Trước hết ta chứng minh điều này dưới giả thiết rằng M là *tự do*; gọi $(e_\lambda)_{\lambda \in L}$ là một cơ sở của M, sao cho $(e_J)_{J \in \mathfrak{B}(L)}$ (công thức (18)) là một cơ sở của $\Lambda(M)$. Giả sử rằng hạt nhân của $\Lambda(f)$ chứa một phần tử $u = \sum_J \alpha_J e_J \neq 0$. Gọi K là một phần tử cực tiểu trong các tập con hữu hạn J sao cho $\alpha_J \neq 0$ và gọi H là một tập con hữu hạn của L rời nhau với K và sao cho $K \cup H$ chứa mọi J (hữu hạn về số lượng) sao cho $\alpha_J \neq 0$; vậy với mọi $J \neq K$ sao cho $\alpha_J \neq 0$, theo định nghĩa ta có $J \cap H \neq 0$ và do đó (no. 8, công thức (20)).
$$
u \wedge e_H = +\alpha_K e_{K \cup H}
$$
thuộc iđêan hai phía của $\Lambda(M)$, tức là hạt nhân của $\Lambda(f)$. Ta viết $e_{K \cup H} = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}$; khi đó $\alpha_K f(e_{\lambda_1}) \wedge f(e_{\lambda_2}) \wedge \cdots \wedge f(e_{\lambda_n}) = 0$; nhờ Mệnh đề 12, các phần tử $f(e_{\lambda_i})$ ($1 \leq i \leq n$) của N phụ thuộc tuyến tính. Nhưng điều này mâu thuẫn với giả thiết rằng $f$ là đơn ánh (II, § 1, no. 11, Hệ quả 3 của Mệnh đề 17).

Bây giờ ta xét trường hợp tổng quát; gọi $M'$ là một A-môđun sao cho $M \oplus M' = P$ là tự do (II, § 2, no. 2, Mệnh đề 4). Xét ánh xạ tuyến tính $g : M \oplus M' \to N \oplus M \oplus M'$ sao cho $g(x, y) = (f(x), 0, y)$, khi đó có biểu đồ giao hoán
$$
\begin{array}{ccc}
M & \xrightarrow{f} & N \\
j \downarrow & & j' \downarrow \\
P & \xrightarrow{g} & N \oplus P
\end{array}
$$

trong đó các mũi tên thẳng đứng là các đơn cấu chính tắc. Vì $g$ là đơn ánh và $P$ là tự do, nên $\Lambda(g)$ là một đồng cấu đơn cấu như đã thấy ở trên. Mặt khác, $\Lambda(j): \Lambda(M) \to \Lambda(P)$ là một đồng cấu đơn cấu vì $M$ là một nhân tử trực tiếp của $P$ (no. 2). Do đó đồng cấu hợp thành

$$
\Lambda(M) \xrightarrow{\Lambda(j)} \Lambda(P) \xrightarrow{\Lambda(g)} \Lambda(N \oplus P)
$$

là đơn cấu và, vì nó cũng bằng đồng cấu hợp thành

$$
\Lambda(M) \xrightarrow{\Lambda(f)} \Lambda(N) \xrightarrow{\Lambda(g')} \Lambda(N \oplus P)
$$

nên ta kết luận rằng $\Lambda(f)$ là đơn ánh.

#### Mệnh đề 13 {#alg-iii-s7-prop-13 .statement}

*Cho $M$ là một $A$-môđun, $N$ là một môđun con hạng tử trực tiếp của $M$ tự do có chiều $p$ và $\{u\}$ là một cơ sở của $\Lambda^p(N)$. Để một phần tử $x \in M$ thuộc $N$, điều kiện cần và đủ là $u \wedge x = 0$.*

Cho $P$ là một môđun con của $M$ bổ sung với $N$ và cho $y \in N,\ z \in P$ sao cho $x = y + z$. Khi đó $u \wedge x = u \wedge z$. Vì $\Lambda^p(N)$ là tự do chiều 1, ánh xạ $\phi: P \to P \otimes \Lambda^p(N)$ sao cho $\phi(p) = p \otimes u$ là song ánh (II, § 3, no. 4, Mệnh đề 4). Mặt khác (no. 7, Mệnh đề 10), hợp thành của các đồng cấu chính tắc

$$
\psi: P \otimes \Lambda^p(N) \to \Lambda(P) \otimes \Lambda(N) \to \Lambda(M)
$$

là đơn ánh. Do đó ánh xạ $\psi \circ \phi$ là đơn ánh, do đó mệnh đề được chứng minh.

#### Định lý 2 {#alg-iii-s7-thm-2 .statement}

*Cho $M$ là một $A$-môđun có một cơ sở hữu hạn $(e_i)_{1 \leq i \leq n}$. Để một dãy $(x_i)_{1 \leq i \leq n}$ gồm $n$ phần tử của $M$ lập thành một cơ sở của $M$, điều kiện cần và đủ là phần tử $\lambda \in A$ sao cho

$$
x_1 \wedge x_2 \wedge \ldots \wedge x_n = \lambda \cdot e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$

là khả nghịch trong $A$.*

Nhắc lại rằng $e_1 \wedge e_2 \wedge \cdots \wedge e_n$ là phần tử duy nhất của một cơ sở của $\Lambda^n(M)$ (no. 8, Hệ quả 1 to Định lý 1) nên phần tử $\lambda \in A$ thỏa mãn (23) được xác định duy nhất. Nếu $(x_i)_{1 \leq i \leq n}$ là một cơ sở của $M$, thì $x_1 \wedge x_2 \wedge \cdots \wedge x_n$ là phần tử duy nhất trong một cơ sở của $\Lambda^n(M)$ (no. 8), khi đó $\lambda$ là khả nghịch. Ngược lại, giả sử $\lambda$ là khả nghịch; khi đó dạng $n$-tuyến tính phản xứng $f$ tương ứng với ánh xạ tuyến tính $g: \Lambda^n(M) \to A$ sao cho

$$
g(e_1 \wedge e_2 \wedge \cdots \wedge e_n) = \lambda^{-1}
$$

thỏa mãn $f(x_1, x_2, \ldots, x_n) = 1$. Với mọi $x \in M$, hiển nhiên

$$
x \wedge x_1 \wedge \cdots \wedge x_n = 0
$$

(no. 3, Mệnh đề 6); áp dụng no. 8, Hệ quả 3 to Định lý 1, ta được

$$
f(x_1, x_2, \ldots, x_n) \cdot x = \sum_{i=1}^n (-1)^{i-1} f(x, x_1, \ldots, \hat{x}_i, \ldots, x_n) \cdot x_i.
$$

Vì $f(x_1, \ldots, x_n) = 1$, điều này cho thấy mọi $x \in M$ đều là một tổ hợp tuyến tính của $x_1, x_2, \ldots, x_n$ và, vì các phần tử sau độc lập tuyến tính (do

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0),
$$

nên chúng lập thành một cơ sở của $M$.

### Bài tập {#alg-iii-s7-exercises}

Xem [các bài tập của § 7](exercises/s7/).
