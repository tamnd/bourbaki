---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 2
section_title: Torsion modules over a principal ideal domain
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.6-A VII.14, A VII.54-A VII.59
pdf_pages: 0365-0373, 0413-0418
extraction: ocr
subsections:
    - "no": 1
      title: Modules over a product of rings
      page: 6
      pdf_page: 365
    - "no": 2
      title: Canonical decomposition of a torsion module over a principal ideal domain
      page: 7
      pdf_page: 366
    - "no": 3
      title: 'Applications : I. Canonical decompositions of rational numbers and of rational functions in one indeterminate'
      page: 10
      pdf_page: 369
    - "no": 4
      title: 'Applications : II. The multiplicative group of units of the integers modulo a'
      page: 12
      pdf_page: 371
statements: 22
exercises: 15
content_sha256: 74231c1b9c69bfeed2753efcd52d52c59f4266dcd06eb563885a45a0c5a2b53f
translated_from: content/en/alg/VII/02_s2_torsion_modules_over_a_principal_ideal.md
source_content_sha256: b73a5f55a0428c0bfdc4c56f769d57b1fd5438c4b81624e9f5d24d90a72de89f
translation_model: gpt-5.4-mini
translation_run: translate-vi-a6edd116
glossary_version: 34
glossary_terms_sha256: a077c97848c4feabadcc231f1ee0a5dd5bd0b4232584a3a6b699126bdf0652ab
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC MÔĐUN XOẮN TRÊN MỘT MIỀN IĐÊAN CHÍNH

### 1. Môđun trên một tích các vành

Cho $A$ là một vành và $(b_i)_{i \in I}$ là một phân tích trực tiếp của $A$, nghĩa là (I, p. 110, Định nghĩa 7) một họ hữu hạn các iđêan hai phía của $A$ sao cho đồng cấu tự nhiên từ $A$ vào tích của các $A/b_i$ là song ánh. Theo *loc. cit.*, Mệnh đề 10, tồn tại một họ $(e_i)_{i \in I}$ các idempotent trung tâm của $A$ sao cho $b_i = A(1 - e_i)$, $\sum_{i \in I} e_i = 1$ và $e_i e_j = 0$ với $i \neq j$.

Với mọi $A$-môđun trái $M$, ký hiệu $M_i$ tập hợp các $m \in M$ sao cho $b_i m = 0$; vì $b_i$ là một iđêan hai phía, đây là một môđun con của $M$; hơn nữa, nếu $a, b \in A$ và $a - b \in b_i$, thì các phép vị tự $a_{M_i}$ và $b_{M_i}$ trùng nhau; do đó tồn tại một cấu trúc $(A/b_i)$-môđun duy nhất trên $M_i$ sao cho cấu trúc $A$-môđun của $M_i$ là cảm sinh qua đồng cấu $A \to A/b_i$.

#### Mệnh đề 1 {#alg-vii-s2-prop-1 .statement}

Môđun $A$-môđun $M$ là tổng trực tiếp của các môđun con $M_i$.

Cho $p_i : M \to M$ ký hiệu phép vị tự $m \mapsto e_i m$; ánh xạ $p_i$ là $A$-tuyến tính vì $e_i$ là trung tâm; vì $e_i^2 = e_i$, $\sum_{i \in I} e_i = 1$ và $e_i e_j = 0$ với $i \neq j$, ta có

$$
p_i \circ p_i = p_i , \quad \sum_{i \in I} p_i = 1_M , \quad p_i \circ p_j = 0 \quad \text{với} \quad i \neq j ,
$$

và các $p_i$ tạo thành một họ trực giao các phép chiếu có tổng là đồng nhất (II, p. 209, Định nghĩa 7). Theo *loc. cit.*, Mệnh đề 12, môđun M là tổng trực tiếp của các môđun con $p_i(M) = e_iM$. Ngoài ra $e_iM$ bị triệt tiêu bởi $b_i = A(1 - e_i)$; nếu $i \neq j$ và $m \in M$ thì $(1 - e_i)e_jm = e_jm$, do đó không có phần tử khác không nào của $e_jM$ bị triệt tiêu bởi $1 - e_i$, và vì thế a fortiori bởi $b_i$. Suy ra $e_iM = M_i$, và mệnh đề được chứng minh.

#### Nhận xét 1 {#alg-vii-s2-n1-rem-1 .statement}

Ngược lại, cho $M'_i$ là một $(A/b_i)$-môđun với mỗi i, và xét A-môđun M, là tổng trực tiếp của các A-môđun $M'_i$; khi đó các môđun con $M_i$ được xây dựng ở trên trùng với các $M'_i$ (chỉ cần lưu ý rằng nếu $i \neq j$ thì không có phần tử khác không nào của $M'_j$ bị triệt tiêu bởi $b_i$ vì $b_i + b_j = A$). Do đó, nói một cách đại khái, việc xét một A-môđun M hay một họ $(M_i)$ các môđun trên các vành $A/b_i = A_i$ là cùng một chuyện.

#### Nhận xét 2 {#alg-vii-s2-n1-rem-2 .statement}

Theo chứng minh trên, các phép chiếu của M lên các thành phần $M_i$ là các phép vị tự.

#### Nhận xét 3 {#alg-vii-s2-n1-rem-3 .statement}

A-môđun M là đơn sinh khi và chỉ khi mỗi $M_i$ là đơn sinh: nếu $M = Am$, thì $M_i = A_i e_i m$; ngược lại nếu $M_i = A_i m_i$ và $m = \sum_{i \in I} m_i$, thì $M = Am$; quả vậy, nếu $n \in M$ chiếu xuống $a_i m_i$ với mỗi i, và nếu $a \in A$ đồng dư với $a_i$ mod $b_i$ với mỗi i, thì am và n có cùng ảnh trong từng $M_i$, nên trùng nhau.

#### Nhận xét 4 {#alg-vii-s2-n1-rem-4 .statement}

Cho M và N là hai A-môđun, với các thành phần $(M_i)$ và $(N_i)$. Cho $u \in \mathrm{Hom}_A(M, N)$ là một ánh xạ A-tuyến tính từ M đến N; khi đó với mọi i và với mọi $m \in M_i$ ta có $u(m) \in N_i$, nên u cảm sinh một ánh xạ $A_i$-tuyến tính $u_i \in \mathrm{Hom}_{A_i}(M_i, N_i)$. Dễ kiểm tra rằng ánh xạ $u \mapsto (u_i)$ là một đẳng cấu của Z-môđun (tương ứng của A-môđun khi A giao hoán)

$$
\mathrm{Hom}_A(M, N) \to \prod_{i \in I} \mathrm{Hom}_{A_i}(M_i, N_i).
$$

### 2. Phân tích chính tắc của một môđun xoắn trên một miền iđêan chính

Cho M là một môđun trên một vành giao hoán A. Với mỗi $a \in A$ hãy ký hiệu $M(\alpha)$ là hạt nhân của tự đồng cấu $x \mapsto \alpha x$ của M. Nếu $a$ và $\beta$ là hai phần tử của A sao cho $\alpha$ chia $\beta$, thì rõ ràng $M(a) \subset M(\beta)$. Đặc biệt, khi n chạy qua tập các số nguyên $\geq 1$, các môđun con $M(\alpha^n)$ tạo thành một dãy tăng; hợp $M$, của các $M(\alpha^n)$ do đó là một môđun con của M, gồm những phần tử của M bị triệt tiêu bởi một lũy thừa nào đó của a. Với mỗi môđun con N của M, rõ ràng $N_1 = N \cap M_a$.

#### Định nghĩa 1 {#alg-vii-s2-def-1 .statement}

Cho $\pi$ là một phần tử bất khả quy của một miền iđêan chính A; một A-môđun M được gọi là rr-nguyên sơ *nếu*, với mọi $x \in M$, tồn tại một số nguyên $n \geq 1$ sao cho $\pi^n x = 0$ (nói cách khác, nếu M bằng với môđun con $M_\pi$).

Rõ ràng mọi môđun đơn sinh có dạng $A/(\pi^s)$ đều là rr-nguyên sơ. Với một A-môđun M tùy ý, môđun con $M_\pi$ là rr-nguyên sơ.

#### Bổ đề 1 {#alg-vii-s2-lem-1 .statement}

Cho M là một môđun trên một miền iđêan chính A; với mọi $a \in A$ sao cho $a \neq 0$, cho $\alpha = \varepsilon \sum_{i=1}^r \pi_i^{n(i)}$ là một phân tích của $\alpha$ thành các nhân tử bất khả quy (VII, p. 4). Môđun con $N = M(a)$ gồm các phần tử của M bị a triệt tiêu là tổng trực tiếp của các môđun con $M(\pi_i^{n(i)})$, và ánh xạ gửi mỗi $x \in M(\alpha)$ tới thành phần của nó trong $M(\pi_i^{n(i)})$ có dạng $x \mapsto \gamma_i x \ (\gamma_i \in A)$. Hơn nữa
$$
M(\pi_i^{n(i)}) = N \cap M_{\pi_i} = N_{\pi_i}
$$
Trước hết chú ý rằng N bị a triệt tiêu, nên có một cấu trúc $A/(\alpha)$-môđun tự nhiên. Theo Mệnh đề 4 của VII, p. 3, đồng cấu chính tắc từ $A/(\alpha)$ vào tích của các vành $A/(\pi_i^{n(i)})$ là một đẳng cấu vành; nay áp dụng Mệnh đề 1 của VII, p. 6, ta suy ra rằng N là tổng trực tiếp của các $M(\pi_i^{n(i)})$; các phép chiếu của phân tích này là các phép nhân vô hướng, theo VII, p. 7, Nhận xét 2. Sự bao hàm $M(\pi_i^{n(i)}) \subset M(\alpha) \cap M_{\pi_i}$ là hiển nhiên; ngược lại, cho $x \in M(\alpha) \cap M_{\pi_i}$. Khi đó tồn tại một lũy thừa $\pi_i^s$ của $\pi_i$ triệt tiêu x; ta có thể giả sử $s \geq n(i)$; theo đẳng thức Bezout, tồn tại $\lambda, \mu \in A$ sao cho $\pi_i^{n(i)} = \lambda \pi_i^s + pa$, do đó $\pi_i^{n(i)} x = 0$ và suy ra cuối cùng $x \in M(\pi_i^{n(i)})$.

#### Bổ đề 2 {#alg-vii-s2-lem-2 .statement}

Cho M là một môđun xoắn (II, p. 313) trên một miền nguyên A. Với mọi họ hữu hạn $(x_i)_{1 \leq i \leq n}$ các phần tử của M, tồn tại một phần tử $\gamma \neq 0$ trong A sao cho mọi $x_i$ đều thuộc $M(\gamma)$.
Thật vậy, với mỗi chỉ số i tồn tại một phần tử $\alpha_i \neq 0$ trong A triệt tiêu $x_i$, và phần tử $\gamma = \prod_{i=1}^n \alpha_i$ sẽ thỏa mãn yêu cầu.

#### Định lý 1 {#alg-vii-s2-thm-1 .statement}

Cho M là một môđun xoắn trên một miền iđêan chính A; với mỗi phần tử bất khả quy $\pi$ của A, cho $M_\pi$ là môđun con của M gồm các phần tử bị triệt tiêu bởi một lũy thừa nào đó của $\pi$. Nếu P là một hệ đại diện của các phần tử bất khả quy của A, thì M là tổng trực tiếp của các môđun con $M_\pi$ với $\pi \in P$.
Mọi phần tử $x \in M$ đều thuộc môđun con $M(\alpha)$ với một $a \neq 0$, nên theo Bổ đề 1 là một tổng của hữu hạn phần tử, mỗi phần tử lại thuộc một môđun con $M_\pi$. Mặt khác, nếu $\sum_{\pi \in P} x_\pi = \sum_{\pi \in P} y_\pi$, trong đó $x_\pi, y_\pi \in M_\pi$ với mọi $\pi \in P$, và trong đó tất cả trừ hữu hạn các $x_\pi$ và $y_\pi$ đều bằng không, thì Bổ đề 2 cho thấy tồn tại $\gamma \neq 0$ trong A sao cho tất cả các $x_\pi$ và $y_\pi$ đều thuộc cùng một môđun con $M(\gamma)$; áp dụng Bổ đề 1 cho $M(\gamma)$ cho thấy $x_\pi = y_\pi$ với mọi $\pi \in P$, điều đó hoàn tất chứng minh.

Rõ ràng, nếu $\pi$ và $\pi'$ là hai phần tử bất khả quy liên kết, thì $M_\pi = M_{\pi'}$; do đó, với một môđun M cho trước, môđun con $M_\pi$ chỉ phụ thuộc vào iđêan $(\pi)$ của A; nó được gọi là thành phần rr-nguyên sơ của môđun M, và phân tích của M thành tổng trực tiếp của các $M_\pi$ được gọi là phân tích chính tắc của M thành tổng trực tiếp các thành phần rr-nguyên sơ của nó.

#### Hệ quả 1 {#alg-vii-s2-thm-1-cor-1 .statement}

— *Mọi môđun con N của một môđun xoắn M đều là tổng trực tiếp của các môđun con $N \cap M_\pi$.*
Điều này suy ra từ sự kiện rằng $N \cap M_\pi$ là thành phần π-nguyên sơ $N_\pi$ của N.

#### Hệ quả 2 {#alg-vii-s2-thm-1-cor-2 .statement}

— *Môđun con N của môđun xoắn A-môđun M là một nhân tử trực tiếp khi và chỉ khi $N_\pi$ là một nhân tử trực tiếp của $M_\pi$, với mọi phần tử bất khả quy π của A.*
Thật vậy, nếu N và N' là hai môđun con của M, thì M = N ⊕ N' khi và chỉ khi $M_\pi = N_\pi \oplus N'_\pi$ với mọi phần tử bất khả quy π của $\mathcal{A}$ (Hệ quả 1).

#### Hệ quả 3 {#alg-vii-s2-thm-1-cor-3 .statement}

— *Cho N là một môđun con của môđun xoắn A-môđun M. Nếu, với mọi phần tử bất khả quy π của A, hoặc $N_\pi = 0$ hoặc $(M/N)_\pi = 0$, thì N là một nhân tử trực tiếp của M*.

Thật vậy, điều kiện $(M/N)_\pi = 0$ suy ra $N_\pi = M_\pi$, và Hệ quả 2 áp dụng.

Một A-môđun M được gọi là *nửa đơn* nếu mọi môđun con của M đều là một nhân tử trực tiếp (cf. A, VIII, § 3).

#### Hệ quả 4 {#alg-vii-s2-thm-1-cor-4 .statement}

— *Cho A là một miền iđêan chính không phải là một trường, và cho M là một A-môđun. Khi đó M là nửa đơn khi và chỉ khi M là một môđun xoắn và $M_\pi = M(\pi)$ với mọi phần tử bất khả quy π của A*.

Trước hết giả sử rằng M là nửa đơn; let x ∈ M và let π là một phần tử bất khả quy của $\mathcal{A}$. Nếu N là một phần bù của $Annx$ trong M, thì ta có thể viết $x = \alpha \pi x + y$, với $\alpha \in \mathcal{A}$ và $y \in N$; nhưng điều đó suy ra $y = (1 - \alpha n)x$, do đó $$
\pi(1 - \alpha \pi)x \in A\pi x \cap N = 0 .
$$ Trước hết suy ra rằng M là một môđun xoắn; nếu hơn nữa $x \in M_π$, thì $\pi(1 - \alpha \pi)x = 0$, do đó $\pi x = \alpha \pi^2 x = \alpha^2 \pi^3 x = \cdots = \alpha^n \pi^{n+1} x$ bằng không và $M_π = M(\pi)$.

Ngược lại, theo Hệ quả 2 là đủ để chứng minh rằng một A-môđun M bị triệt tiêu bởi một phần tử bất khả quy π là nửa đơn; nhưng điều đó hiển nhiên, vì khi đó M có một cấu trúc tự nhiên của một không gian vectơ trên trường $\mathcal{A}/(\pi)$, và các môđun con của M chính xác là các không gian vectơ con theo cấu trúc này.

#### Nhận xét 1 {#alg-vii-s2-n2-rem-1 .statement}

— Rõ ràng linh hóa tử của mọi phần tử khác 0 của một môđun nguyên sơ τ có dạng $A\pi^k$ ($k > 0$ là một số nguyên), vì nó là một iđêan chính chứa một lũy thừa của τ. Cho x là một phần tử của M; với mỗi $\pi \in P$, đặt $x_\pi$ là thành phần của x trong $M_π$; linh hóa tử của x là BCNN của các linh hóa tử của những $x_\pi$ khác không, nhưng theo trên thì trong trường hợp này nó bằng *tích* của các linh hóa tử của những $x_\pi$ khác không (VI, p. 16, Mệnh đề 12 (DIV)).

#### Mệnh đề 2 {#alg-vii-s2-prop-2 .statement}

— *Nếu M là một môđun xoắn sinh hữu hạn trên một miền iđêan chính A, thì các thành phần nguyên sơ n của M bằng không, trừ ra một số hữu hạn, và các phép chiếu của M lên các thành phần này $M_\pi$ là các phép vị tự*.

Điều này suy ra ngay lập tức từ Bổ đề 1, vì theo Bổ đề 2 tồn tại $\alpha \neq 0$ trong $\mathcal{A}$ sao cho $M = M(\alpha)$.

#### Nhận xét 2 {#alg-vii-s2-n2-rem-2 .statement}

— Theo VII, p. 7, Nhận xét 3, một A-môđun xoắn sinh hữu hạn là cyclic khi và chỉ khi mỗi thành phần nguyên sơ π của nó là cyclic.

Một trường hợp riêng quan trọng mà Định lý 1 và Mệnh đề 2 áp dụng là khi $A = \mathbf{Z}$; một $\mathbf{Z}$-môđun chỉ là một *nhóm Abel*. Một nhóm Abel được gọi là một *nhóm xoắn* nếu nó là một $\mathbf{Z}$-môđun xoắn, tức là nếu mọi phần tử của nó đều có *cấp hữu hạn*. Khi đó $P$ được lấy là tập hợp các số nguyên tố $> 0$; với mỗi số nguyên tố $p > 0$, một nhóm (Abel) được gọi là $p$-xoắn nếu mọi phần tử của nó đều có các cấp là những lũy thừa của $p$. Theo thuật ngữ này, Định lý 1 cho thấy rằng *mọi nhóm Abel xoắn đều là một tổng trực tiếp của các nhóm p-xoắn*. Trong trường hợp các nhóm hữu hạn, điều này cũng suy ra từ I, p. 80, Định lý 4.

### 3. Ứng dụng : I. Các phân rã chính tắc của các số hữu tỉ và của các hàm hữu tỉ theo một ẩn

#### Định lý 2 {#alg-vii-s2-thm-2 .statement}

*Cho $A$ là một miền iđêan chính, cho $K$ là trường các phân số của nó và cho $P$ là một hệ đại diện của các phần tử bất khả quy của $A$. Với một phần tử $x \in K$, tồn tại một tập con hữu hạn $H$ của $P$, các phần tử $a_0 \in A$ và $a_p \in A$ không chia hết cho $p$ trong $A$ ($p \in H$), và các số nguyên $s(p) > 0$ ($p \in H$) sao cho*

$$
x = a_0 + \sum_{p \in H} a_p p^{-s(p)},
$$

*trong đó $H$ và các $s(p)$ được xác định duy nhất bởi các điều kiện này.*

*Hơn nữa, nếu $R_p$ ký hiệu một tập con của $A$ chứa chính xác một phần tử của mỗi lớp thặng dư mod $p$ trong $A$ ($p \in P$), thì mỗi $x \in K$ có thể được biểu diễn duy nhất dưới dạng*

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} r_{ph} p^{-h} \right)
$$

*trong đó $a \in A$ và $r_{ph} \in R_p$ với mọi $h$ và $p$, và tất cả trừ hữu hạn nhiều trong số các $r_{ph}$ đều bằng không.*

Xét $K$ như một $A$-môđun; khi đó $A$ là môđun con sinh bởi 1. Môđun thương $K/A$ là thương của $K$ bởi quan hệ tương đương $x' - x \in A$, cũng được viết, theo ký hiệu ở VI, p. 6, là $x \equiv x'$ (mod 1); ký hiệu $f$ là đồng cấu tự nhiên từ $K$ lên $M = K/A$.

Môđun thương $M$ là một *môđun xoắn*, vì mỗi phần tử của $M$ có dạng $f(a/b)$ ($a \in A, b \in A, b \neq 0$), do đó $b f(a/b) = f(a) = 0$. Do đó Định lý 1 của VII, p. 8 áp dụng. Cho $M_p$ ($p \in P$) là môđun con gồm các phần tử của $M$ bị triệt tiêu bởi các lũy thừa của $p$; khi đó $f^{-1}(M_p)$ là vành con $A_p$ gồm các phần tử của $K$ có dạng $a p^{-n}$ với $a \in A$ và $n \geq 0$ là một số nguyên. Môđun $M$ là tổng trực tiếp của các $M_p$, nên mọi $x \in K$ đều đồng dư mod 1 với một phần tử trong tổng của các $A_p$; nói cách khác, công thức (1) đúng, với các số nguyên $s(p)$ $> 0$, và các $a$, là một số hữu hạn phần tử của $A$ sao cho $a$, không là bội của $p$.

Ta sẽ chỉ ra rằng các điều kiện này trên các $s(p)$ và các $a$, xác định hoàn toàn $H$ và các $s(p)$. Thật vậy $H$ khi đó là tập hợp các $p \in P$ sao cho thành phần của $f(x)$ trong $M_p$ là $\neq 0$. Mặt khác, nếu $s$ và $s'$ là hai số nguyên $> 0$ sao cho $s \geq s'$ và nếu $a$ và $a'$ là các phần tử của $A$ không chia hết cho $p$ sao cho $ap^{-s} \equiv a'p^{-s'} \pmod{1}$, thì suy ra rằng $a \equiv a'p^{s-s'} \pmod{p^s}$; nếu $s > s'$ thì $a \equiv 0 \pmod{p}$, mâu thuẫn với các giả thiết. Lập luận này cũng cho thấy rằng mỗi $a_i$ được xác định mod $p^{s(p)}$.

Để hoàn thành chứng minh, trước hết ta nhận thấy rằng trong mỗi lớp thặng dư mod $p^i$ của $A$ tồn tại một phần tử duy nhất có dạng $\sum_{h=0}^{s-1} r_h p^h$ với $r_h \in R_p$ cho $0 \leq h \leq s-1$. Thật vậy, ta tiến hành bằng quy nạp theo $s$ (tính chất suy ra từ định nghĩa của $R_p$ khi $s = 1$) : cho $x \in A$; theo giả thiết, tồn tại một phần tử duy nhất có dạng $\sum_{h=0}^{s-2} r_h p^h$ ($r_h \in R_p$) trong lớp thặng dư của $x$ mod $p^{s-1}$; khi đó $x - \sum_{h=0}^{s-2} r_h p^h$ là một bội $ap^{s-1}$ của $p^{s-1}$; nay tồn tại một phần tử duy nhất $r_s$, của $R_p$, sao cho $a \equiv r_s \pmod{p}$; do đó $x \equiv \sum_{h=0}^{s-1} r_h p^h \pmod{p^s}$. Để thu được công thức (2) bây giờ chỉ cần áp dụng nhận xét này cho từng $a_p$ trong công thức (1). Tính duy nhất là hiển nhiên theo trên.

Sau đây là những áp dụng quan trọng nhất của ĐL 2 :

I. *Vành A là vành Z của các số nguyên hữu tỉ, và K = Q*. Cho P là tập hợp các số nguyên tố > 0, và với mỗi $p \in P$ hãy lấy $R_p$ là khoảng $(0, p-1)$ trong $\mathbf{Z}$. Như vậy ta có sự phân tích chính tắc

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} e_{ph} p^{-h} \right)
$$

với $a \in \mathbf{Z}$, $e_{ph} \in \mathbf{Z}$ và $0 \leq e_{ph} \leq p-1$.

II. *Vành A là vành E[X] của các đa thức theo một ẩn trên một trường giao hoán E, và K = E(X)*. Cho P là tập hợp các đa thức bất khả quy đơn thức trong $E[X]$ (VII, p. 5). Với $p \in P$ ta có thể, nhờ phép chia Euclid của đa thức (IV, p. 10), lấy $R_p$ là tập hợp các đa thức có bậc nhỏ hơn hẳn bậc của $p$. Như vậy ta có sự phân tích (gọi là chính tắc) của một hàm hữu tỉ $r(X) \in E(X)$:

$$
r(X) = a(X) + \sum_{p \in P} \left( \sum_{h=1}^{\infty} v_{ph}(X) \cdot p(X)^{-h} \right)
$$

trong đó $a(X)$ là một đa thức và $v_{ph}(X)$ là một đa thức có bậc nhỏ hơn hẳn bậc của $p(X)$, với mọi $p$ và $h$. Đặc biệt, nếu trường E là *đóng đại số*, thì các $p(X)$ có dạng $X - a$ với $a \in E$, và do đó các $v_{ph}(X)$ là các hằng số.

Vì thế ta có thể nói rằng không gian vectơ $E(X)$ trên trường E có một cơ sở gồm các đơn thức $X^n$ ($n \geq 0$ là một số nguyên) và các hàm hữu tỉ có dạng $X^m / (p(X))^h$, trong đó $p \in P$ và $h$ và $m$ là các số nguyên với $h \geq 1$ và $0 \leq rn < \deg(p)$.

### 4. Ứng dụng : II. Nhóm nhân của các đơn vị của các số nguyên theo môđun a

Cho a là một số nguyên > 1, và cho $(\mathbf{Z}/a\mathbf{Z})^*$ là nhóm nhân của các phần tử khả nghịch của vành $\mathbf{Z}/a\mathbf{Z}$. Nếu $a = \prod p_i^{n(i)}$ là phân tích của a thành các thừa số nguyên tố, thì vành $\mathbf{Z}/a\mathbf{Z}$ đẳng cấu với tích của các vành $\mathbf{Z}/p_i^{n(i)}\mathbf{Z}$ (VII, p. 3, Mệnh đề 4) và nhóm $(\mathbf{Z}/a\mathbf{Z})^*$ đẳng cấu với tích của các nhóm $(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$. Do đó ta quy về việc nghiên cứu các nhóm $(\mathbf{Z}/p^n\mathbf{Z})^*$, trong đó p là một số nguyên tố; nhắc lại rằng (V, p. 80) cấp $\varphi(p^n)$ của $(\mathbf{Z}/p^n\mathbf{Z})^*$ là $p^n - p^{n-1} = p^{n-1}(p-1)$.

Trước hết, giả sử $p > 2$; đồng cấu tự nhiên $\mathbf{Z}/p^n\mathbf{Z} \to \mathbf{Z}/p\mathbf{Z}$ hạn chế thành một đồng cấu nhóm từ $(\mathbf{Z}/p^n\mathbf{Z})^*$ lên $(\mathbf{Z}/p\mathbf{Z})^*$, có hạt nhân ta ký hiệu là U$(p^n)$; theo VII, p. 3, Mệnh đề 3, lớp thặng dư modulo $p^n$ của một số nguyên m là khả nghịch khi và chỉ khi m nguyên tố cùng nhau với p, tức là khi và chỉ khi lớp thặng dư của $m$ modulo p là khả nghịch. Suy ra rằng U$(p^n)$ gồm tất cả các lớp thặng dư modulo $p^n$ của các số nguyên đồng dư với 1 modulo p, nên có $p^{n-1}$ phần tử, và có một dãy khớp

(3)
$$
\{1\} \to \mathrm{U}(p^n) \to (\mathbf{Z}/p^n\mathbf{Z})^* \to (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}.
$$

Tương tự, với $n \geq 2$ hãy ký hiệu U$(2^n)$ là hạt nhân của đồng cấu tự nhiên từ $(\mathbf{Z}/2^n\mathbf{Z})^*$ đến $(\mathbf{Z}/4\mathbf{Z})^*$; đây là một nhóm có cấp $2^{n-2}$, gồm tất cả các lớp thặng dư modulo $2^n$ của các số nguyên đồng dư với 1 modulo 4, và có một dãy khớp

(4)
$$
\{1\} \to \mathrm{U}(2^n) \to (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

#### Bổ đề 3 {#alg-vii-s2-lem-3 .statement}

Cho x, y, k là các số nguyên với $k \geq 0$, và cho $p > 2$ là một số nguyên tố. Nếu $x \equiv 1 + py \mod p^2$ thì $x^{p^k} \equiv 1 + p^{k+1}y \mod p^{k+2}$. *Nếu* $x \equiv 1 + 4y \mod 8$ thì $x^{2^k} \equiv 1 + 2^{k+2}y \mod 2^{k+3}$.

Để chứng minh mệnh đề thứ nhất, chỉ cần chỉ ra rằng, nếu $k \geq 1$ và $x \equiv 1 + p^ky \mod p^{k+1}$, thì $x^p \equiv 1 + p^{k+1}y \mod p^{k+2}$, rồi lập luận theo quy nạp theo số nguyên k. Với mọi $a \in \mathbf{Z}$ và $k \geq 1$, hiển nhiên là
$$
(1 + p^ka)^p \equiv 1 + p^{k+1}a \mod p^{k+2},
$$
do đó
$$
(1 + p^ky + p^{k+1}z)^p = (1 + p^k(y + pz))^p \equiv \\
= 1 + p^{k+1}(y + pz) \equiv 1 + p^{k+1}y \mod p^{k+2}.
$$
Tương tự, với $k \geq 1$ ta có
$$
(1 + 2^{k+1}a)^2 \equiv 1 + 2^{k+2}a \mod 2^{k+3},
$$
suy ra
$$
(1 + 2^{k+1}y + 2^{k+2}z)^2 \equiv 1 + 2^{k+2}y \mod 2^{k+3},
$$
do đó mệnh đề thứ hai theo quy nạp theo k.

#### Mệnh đề 3 {#alg-vii-s2-prop-3 .statement}

Cho $p > 2$ là một số nguyên tố và cho $n > 0$ là một số nguyên; khi đó nhóm $U(p^n)$ là cyclic cấp $p^{n-1}$; nếu $n \geq 2$ thì lớp thặng dư mod $p^n$ của một số nguyên $x$ đồng dư với 1 mod $p$ là một phần tử sinh của $U(p^n)$ khi và chỉ khi $x$ không đồng dư với 1 mod $p^2$. Cho $m > 1$ là một số nguyên; khi đó nhóm $U(2^m)$ là cyclic cấp $2^{m-2}$; nếu $m \geq 3$ thì lớp thặng dư mod $2^m$ của một số nguyên $x$ đồng dư với 1 mod 4 là một phần tử sinh của $U(2^m)$ khi và chỉ khi $x$ không đồng dư với 1 mod 8.

Vì $U(p^n)$ có cấp $p^{n-1}$, cấp của mọi phần tử $u$ của $U(p^n)$ là một lũy thừa của $p$, và $u$ là một phần tử sinh của $U(p^n)$ khi và chỉ khi $u^{p^{n-2}} \neq 1$. Khi đó, nếu $u$ là lớp của $x = 1 + py$, thì $u^{p^{n-2}}$ là lớp của $1 + p^{n-1}y$, theo Bổ đề 3, do đó $u$ sinh ra $U(p^n)$ khi và chỉ khi $y \not\equiv 0 \mod p$, nói cách khác $x \not\equiv 1 \mod p^2$. Chẳng hạn, lớp $1 + p$ sinh ra $U(p^n)$. Tương tự, lớp $u$ của $x$ mod $2^n$ sinh ra $U(2^n)$ khi và chỉ khi $u^{2^{n-3}} \neq 1$, tức là $x$ không đồng dư với 1 mod 8, theo Bổ đề 3; điều này được thỏa bởi $x = 5$.

#### Bổ đề 4 {#alg-vii-s2-lem-4 .statement}

Cho $A$ là một miền iđêan chính và cho $0 \to N \to M \to P \to 0$ là một dãy khớp các $A$-môđun. Giả sử tồn tại các phần tử nguyên tố cùng nhau $a, b \in A$ sao cho $aN = 0$ và $bP = 0$. Khi đó dãy khớp tách ra. Nếu thêm vào đó $N$ và $P$ đều là môđun cyclic, thì $M$ cũng là môđun cyclic.

==========

Môđun $M$ là xoắn, vì $abM = 0$. Khẳng định đầu tiên suy ra từ Hệ quả 3 của VII, p. 9. Nếu $N$ và $P$ là cyclic, thì chúng sinh hữu hạn, và do đó $M$ cũng sinh hữu hạn (II, p. 17, Hệ quả 5); vì mỗi thành phần $p$-nguyên sơ của $M$ đẳng cấu với một thành phần $p$-nguyên sơ hoặc của $N$ hoặc của $P$, suy ra từ Nhận xét 2 của VII, p. 10 rằng $M$ là cyclic.

#### Định lý 3 {#alg-vii-s2-thm-3 .statement}

Nếu $a = \prod p_i^{n(i)}$ là phân tích thành thừa số nguyên tố của số nguyên $a > 1$, thì nhóm $(\mathbf{Z}/a\mathbf{Z})^*$ gồm các phần tử khả nghịch của vành $\mathbf{Z}/a\mathbf{Z}$ đẳng cấu với tích của các nhóm $(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$. Nếu $p > 2$ là một số nguyên tố và $n \geq 1$ là một số nguyên, thì nhóm $(\mathbf{Z}/p^n\mathbf{Z})^*$ là cyclic cấp $p^n \ ^1(p - 1)$. Nhóm $(\mathbf{Z}/2\mathbf{Z})^*$ là tầm thường; với $n \geq 2$ nhóm $(\mathbf{Z}/2^n\mathbf{Z})^*$ là tích trực tiếp của nhóm cyclic cấp $2^n \ ^2$ sinh bởi lớp thặng dư của 5 mod $2^n$ và nhóm cyclic cấp 2 gồm các lớp thặng dư của 1 và $-1$ mod $2^n$.

Các cấp $p^n \ ^1$ của $U(p^n)$ và $p - 1$ của $(\mathbf{Z}/p\mathbf{Z})^*$ nguyên tố cùng nhau; vì $U(p^n)$ và $(\mathbf{Z}/p\mathbf{Z})^*$ là cyclic (Mệnh đề 3 và V, p. 78, Bổ đề 1), nhóm $(\mathbf{Z}/p^n\mathbf{Z})^*$ là cyclic (áp dụng Bổ đề 4 cho dãy khớp (3)). Nếu $n \geq 2$ thì hạn chế của đồng cấu $v : (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^*$ lên nhóm con $(1, -1)$ là song ánh; do đó nhóm $(\mathbf{Z}/2^n\mathbf{Z})^*$ là tích trực tiếp của nhóm con này và hạt nhân $U(2^n)$ của $v$; kết quả suy ra từ Mệnh đề 3.

#### Nhận xét {#alg-vii-s2-n4-rem-1 .statement}

Cho $p > 2$ là một số nguyên tố và cho $x$ là một số nguyên đồng dư với 1 mod $p$ và không đồng dư với 1 mod $p^2$; có một dãy khớp

$$
\{0\} \to \mathbf{Z}/p^n \ ^1\mathbf{Z} \xrightarrow{u} (\mathbf{Z}/p^n\mathbf{Z})^* \xrightarrow{\nu} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

của các nhóm, trong đó $v$ là phép chiếu tự nhiên và trong đó $u$ được cảm sinh trên các thương bởi ánh xạ $r \mapsto x^r$. Cho $\mathbf{Z}_p$ là vành các số nguyên $p$-adic ($V$, p. 96), và cho $x$ là một phần tử của $\mathbf{Z}_p$ sao cho $x - 1 \in p\mathbf{Z}_p$ và $x - 1 \notin p^2\mathbf{Z}_p$; khi chuyển qua giới hạn ngược, các dãy khớp (5) cảm sinh một dãy khớp

$$
\{0\} \to \mathbf{Z}_p \xrightarrow{u} \mathbf{Z}_p^* \xrightarrow{v} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

trong đó $v$ là ánh xạ tự nhiên, và ánh xạ liên tục $u$ mở rộng ánh xạ $n \mapsto x^n$ ($n \in \mathbf{Z}$). Ta thường đặt $x^n = u(x)$ với $n \in \mathbf{Z}_p$.

Tương tự, nếu $x \in \mathbf{Z}_2$ với $x - 1 \in 4\mathbf{Z}$, và $x - 1 \notin 8\mathbf{Z}_2$, thì có một dãy khớp tách

$$
\{0\} \to \mathbf{Z}_2 \xrightarrow{u} \mathbf{Z}_2^* \xrightarrow{v} (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

trong đó $u$ là một mở rộng liên tục của ánh xạ $n \mapsto x^n$

### Bài tập {#alg-vii-s2-exercises}

Xem các [bài tập cho § 2](exercises/s2/).
