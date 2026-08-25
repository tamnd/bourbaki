---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 3
section_title: Graded algebras
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0481-0484, 0650-0650
extraction: ocr
subsections:
    - "no": 1
      title: GRADED ALGEBRAS
      page: 0
      pdf_page: 481
    - "no": 2
      title: GRADED SUBALGEBRAS, GRADED IDEALS OF A GRADED ALGEBRA
      page: 0
      pdf_page: 483
    - "no": 3
      title: DIRECT LIMITS OF GRADED ALGEBRAS
      page: 0
      pdf_page: 484
statements: 4
exercises: 1
content_sha256: d802410ed8c1f057c7a2908c990cb9e332e7bbb99dcee5dbae38a09cefe5ad71
translated_from: content/en/alg/III/03_s3_graded_algebras.md
source_content_sha256: 38b7965ea4ef3a096ea51873d498f423f82feaa31641e8044291d726b3d90f91
translation_model: gpt-5-6-mini
translation_run: translate-vi-470070e5
glossary_version: 34
glossary_terms_sha256: 986f69dcac9ea82deff6c777f68e388622819ea1e625279786cf99864a8acd19
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ĐẠI SỐ PHÂN BẬC

Các phép phân bậc được xét trong đoạn này sẽ có tập các bậc là một *nửa nhóm giao hoán viết theo phép cộng mà phần tử đơn vị được ký hiệu bởi 0*.

### 1. ĐẠI SỐ PHÂN BẬC

#### Định nghĩa 1 {#alg-iii-s3-def-1 .statement}

*Cho $\Delta$ là một nửa nhóm giao hoán, $A$ là một vành phân bậc kiểu $\Delta$* (II, § 11, no. 2), $(A_\lambda)_{\lambda \in \Delta}$ *là phép phân bậc của nó và E là một đại số trên A. Một phép phân bậc* $(E_\lambda)_{\lambda \in \Delta}$ *kiểu $\Delta$ trên nhóm cộng E được gọi là tương thích với cấu trúc đại số trên A của E nếu nó tương thích cả với cấu trúc A-môđun lẫn cấu trúc vành trên E, nói cách khác, nếu, với mọi $\lambda, \mu$ trong $\Delta$,*

(1) $$ A_\lambda E_\mu \subset E_{\lambda + \mu} $$
(2) $$ E_\lambda E_\mu \subset E_{\lambda + \mu}. $$

*Đại số trên A E, với phép phân bậc này, khi đó được gọi là một đại số phân bậc kiểu $\Delta$ trên vành phân bậc A.*

Khi phép phân bậc trên A là *tầm thường* (tức là (II, § 11, no. 1) $A_0 = A, A_\lambda = \{0\}$ với $\lambda \neq 0$), điều kiện (1) có nghĩa là các $E_\lambda$ là các *A-môđun con* của E. Điều này dẫn đến định nghĩa khái niệm đại số phân bậc kiểu $\Delta$ trên một vành giao hoán *không phân bậc* $A$: cho A phép phân bậc tầm thường kiểu $\Delta$ và áp dụng định nghĩa trên.

Khi xét các đại số phân bậc $A$-algebra $E$ có một *phần tử đơn vị* $e$, ta luôn hiểu rằng $e$ *có bậc* 0 (xem Bài tập 1).

Suy ra rằng nếu một phần tử khả nghịch $x \in E$ là *thuần nhất* và có bậc $p$, thì nghịch đảo $x^{-1}$ của nó là *thuần nhất* và có bậc $-p$: chỉ cần phân tích $x^{-1}$ thành tổng các phần tử thuần nhất trong các đẳng thức $x^{-1}x = xx^{-1} = e$.

Cho $E$ và $E'$ là hai đại số phân bậc kiểu $\Delta$ trên một vành phân bậc $A$ kiểu $\Delta$. Một đồng cấu đại số trên $A$ $u : E \to E'$ được gọi là một *đồng cấu đại số phân bậc* nếu $u(E_\lambda) \subset E'_\lambda$ với mọi $\lambda \in \Delta$ (trong đó $(E_\lambda)$ và $(E'_\lambda)$ lần lượt ký hiệu các phép phân bậc của $E$ và $E'$); khi $E$ và $E'$ kết hợp và có đơn vị và $u$ có đơn vị, điều kiện này có nghĩa là $u$ là một đồng cấu vành phân bậc (II, § 11, no. 2).

Cho $E$ là một đại số phân bậc $A$ kiểu $N$. $E$ được đồng nhất với một đại số phân bậc $A$ kiểu $\mathbf{Z}$ bằng cách đặt $E_n = \{0\}$ với $n < 0$.

#### Nhận xét {#alg-iii-s3-n1-rem-1 .statement}

Định nghĩa 1 cũng có thể được diễn giải bằng cách nói rằng $E$ là một A-môđun phân bậc và ánh xạ tuyến tính $A$-tuyến tính

$$
m : E \otimes_A E \to E
$$

xác định phép nhân trên $E$ (\S 1, no. 3), là *thuần nhất bậc* 0 khi $E \otimes_A E$ được trang bị phép phân bậc kiểu $\Delta$ của nó (II, § 11, no. 5).

Để định nghĩa một cấu trúc đại số phân bậc kiểu $\Delta$ trên vành phân bậc $A$, với $E$ là môđun $A$-phân bậc nền, do đó tương đương với việc định nghĩa, với mỗi cặp có thứ tự $(\lambda, \mu)$ của các phần tử của $\Delta$, một ánh xạ $\mathbf{Z}$-song tuyến tính

$$
m_{\lambda \mu} : E_\lambda \times E_\mu \to E_{\lambda + \mu}
$$

sao cho với mọi bộ ba chỉ số $(\lambda, \mu, \nu)$ và với $\alpha \in A_\lambda,\ x \in E_\mu,\ y \in E_\nu$,

$$
\alpha . m_{\mu \nu}(x, y) = m_{\lambda + \mu, \nu}(\alpha x, y) = m_{\mu, \lambda + \nu}(x, \alpha y).
$$

#### Ví dụ {#alg-iii-s3-n1-exa-1 .statement}

(1) Cho $B$ là một *vành phân bậc* kiểu $\Delta$; nếu $B$ được trang bị cấu trúc đại số $\mathbf{Z}$ chính tắc của nó (\S 1, No. 1, *Ví dụ* 2), $B$ là một đại số $A$-phân bậc ($\mathbf{Z}$ được trang bị phép phân bậc tầm thường).

(2) Cho $A$ là một vành giao hoán phân bậc kiểu $\Delta$ và $M$ là một môđun $A$-phân bậc kiểu $\Delta$. Giả sử rằng mọi phần tử của nửa nhóm $\Delta$ đều *giản ước được*, điều này cho phép ta (II, § 11, No. 6) định nghĩa trên $\mathrm{Homgr}_A(M, M) = \mathrm{Endgr}_A(M)$ một cấu trúc môđun $A$-phân bậc kiểu $\Delta$; vì phép phân bậc này tương thích với cấu trúc vành trên $\mathrm{Endgr}_A(M)$ (II, § 11, No. 6), nó định nghĩa một cấu trúc *đại số $A$-phân bậc có đơn vị* trên đại số $A$ $\mathrm{Endgr}_A(M)$.

(3) *Đại số của một magma.* Cho $S$ là một magma và $\phi : S \to \Delta$ là một đồng cấu. Với mọi $\lambda \in \Delta$, ta viết $S_\lambda = \phi^{-1}(\lambda)$; khi đó $S_\lambda S_\mu \subset S_{\lambda + \mu}$. Cho $A$ là một vành giao hoán phân bậc có kiểu $\Delta$ và $(A_\lambda)_{\lambda \in \Delta}$ là phép phân bậc của nó; ta sẽ định nghĩa một cấu trúc đại số $A$ phân bậc trên đại số $E = A^{(S)}$ của magma $S$ (\S 2, no. 6). Để làm điều này, gọi $E_{\lambda}$ là nhóm con cộng tính của $E$ sinh bởi các phần tử có dạng $\alpha.s$ sao cho $\alpha \in A_{\mu}, s \in S_{\nu}$ và $\mu + \nu = \lambda$. Vì các $S_{\lambda}$ rời nhau từng đôi một, $E$ là tổng trực tiếp của các $A_{\mu}S_{\nu}$ và do đó cũng là tổng trực tiếp của các $E_{\lambda}$ và hiển nhiên rằng các $E_{\lambda}$ thỏa mãn các điều kiện (1) và (2) và vì thế xác định trên $E$ cấu trúc đại số $A$ phân bậc mong muốn. Nếu $S$ có một phần tử đơn vị $e$, thì cũng có thể giả sử rằng $\phi(e) = 0$. Một trường hợp riêng là trường hợp phép phân bậc của vành $A$ là tầm thường; khi đó $E_{\lambda}$ là môđun con-$A$ của $E$ sinh bởi $S_{\lambda}$. Đặc biệt hơn, nếu ta lấy $S = \mathbf{N}^{(1)}, \Delta = \mathbf{N}$ và $\phi$ là ánh xạ sao cho $\phi((n_i)) = \sum_{i \in I} n_i$, vành $A$ có phép phân bậc tầm thường, ta thu được một phép phân bậc trên đại số đa thức $A[X_i]_{i \in I}$, trong đó bậc của một đa thức thuần nhất $\neq 0$ là bậc toàn phần được định nghĩa trong § 2, no. 9 (cf. § 6, no. 6).

Bây giờ ta lấy $S$ là monôit tự do $Mo(B)$ của một tập hợp $B$ (I, § 7, no. 2) và $\phi$ là đồng cấu $Mo(B) \to \mathbf{N}$ gán cho mỗi từ độ dài của nó. Như vậy thu được một cấu trúc đại số $A$ phân bậc trên đại số kết hợp tự do của tập hợp $B$ (§ 2, no. 7; cf. § 5, no. 5).

### 2. ĐẠI SỐ CON PHÂN BẬC, IDEAL PHÂN BẬC CỦA MỘT ĐẠI SỐ PHÂN BẬC

Cho $E$ là một đại số phân bậc có kiểu $\Delta$ trên một vành phân bậc $A$ có kiểu $\Delta$. Nếu $F$ là một đại số con-$A$ của $E$ là một môđun con-$A$ phân bậc, thì phép phân bậc $(F_{\lambda})$ trên $F$ tương thích với cấu trúc đại số $A$ của nó, vì $F_{\lambda} = F \cap E_{\lambda}$; trong trường hợp này $F$ được gọi là một đại số con phân bậc của $E$ và đơn ánh chính tắc $F \to E$ là một đồng cấu đại số phân bậc.

Tương tự, nếu $a$ là một iđêan trái (tương ứng phải) của $E$ là một môđun con $A$ phân bậc, thì $E_{\lambda}a_{\mu} \subset a_{\lambda+\mu}$ (tương ứng $a_{\lambda}E_{\mu} \subset a_{\lambda+\mu}$), vì $a_{\lambda} = a \cap E_{\lambda}$; khi đó $a$ được gọi là một iđêan phân bậc của đại số $E$. Nếu $b$ là một iđêan hai phía phân bậc của $E$ thì phép phân bậc thương trên môđun $E/b$ tương thích với cấu trúc đại số trên $E/b$ và đồng cấu chính tắc $E \to E/b$ là một đồng cấu đại số phân bậc.

Nếu $u : E \to E'$ là một đồng cấu đại số phân bậc, $\operatorname{Im}(u)$ là một đại số con phân bậc của $E'$, $\operatorname{Ker}(u)$ là một iđêan hai phía phân bậc của $E$ và song ánh $E/\operatorname{Ker}(u) \to \operatorname{Im}(u)$ liên kết một cách chính tắc với $u$ là một đẳng cấu đại số phân bậc.

#### Mệnh đề 1 {#alg-iii-s3-prop-1 .statement}

*Cho $A$ là một vành giao hoán phân bậc kiểu $\Delta$, $E$ là một đại số $A$ phân bậc kiểu $\Delta$ và $S$ là một tập hợp các phần tử thuần nhất của $E$. Khi đó đại số con $A$ (tương ứng iđêan trái, iđêan phải, iđêan hai phía) sinh bởi $S$ là một đại số con phân bậc (tương ứng iđêan phân bậc).*.

Đại số con của $E$ sinh bởi $S$ là môđun con $A$ sinh bởi các tích hữu hạn của các phần tử của $S$, vốn thuần nhất; tương tự, iđêan trái (tương ứng phải) sinh bởi $S$ là môđun con $A$ sinh bởi các phần tử có dạng $u_1(u_2(\ldots(u_n s))\ldots)$ (tương ứng $(\ldots((s u_n) u_{n-1})\ldots) u_2$ ) $u_1$ ) trong đó s ∈ S và các $u_j \in E$ là thuần nhất (n tùy ý) và các tích này là thuần nhất, do đó trong trường hợp này kết luận được suy ra từ II, § 11, no. 3, Mệnh đề 2); cuối cùng iđêan hai phía sinh bởi S là hợp của dãy $(\mathfrak{I}_n)_{n \geq 1}$, trong đó $\mathfrak{I}_1$ là iđêan trái sinh bởi S và $\mathfrak{I}_{2n}$ (tương ứng $\mathfrak{I}_{2n+1}$) là iđêan phải (tương ứng trái) sinh bởi $\mathfrak{I}_{2n-1}$ (tương ứng $\mathfrak{I}_{2n}$), điều này hoàn tất chứng minh.

### 3. GIỚI HẠN TRỰC TIẾP CỦA CÁC ĐẠI SỐ PHÂN BẬC

Cho $(A_\alpha, \phi_{\beta \alpha})$ là một hệ trực tiếp có hướng của các vành giao hoán phân bậc kiểu $\Delta$ (II, § 11, no. 3, Nhận xét 3) và với mỗi $\alpha$ cho $E_\alpha$ là một đại số $A_\alpha$ phân bậc kiểu $\Delta$; với $\alpha \leq \beta$ cho $f_{\beta \alpha}: E_\alpha \to E_\beta$ là một đồng cấu đại số phân bậc trên $A_\alpha$ và giả sử rằng $f_{\gamma \alpha} = f_{\gamma \beta} \circ f_{\beta \alpha}$ với $\alpha \leq \beta \leq \gamma$; khi đó ta gọi $(E_\alpha, f_{\beta \alpha})$ là một hệ trực tiếp có hướng của các đại số phân bậc kiểu $\Delta$ trên hệ trực tiếp có hướng $(A_\alpha, \phi_{\beta \alpha})$ của các vành giao hoán phân bậc kiểu $\Delta$. Khi đó ta biết (II, § 11, no. 3) rằng $E = \lim \to E_\alpha$ có một cách chính tắc một cấu trúc môđun phân bậc kiểu $\Delta$ trên vành phân bậc $A = \lim \to A_\alpha$ và một phép nhân sao cho $E^\lambda E^\mu \subset E^{\lambda + \mu}$ (trong đó $(E^\lambda)$ ký hiệu phép phân bậc trên E); khi đó phép nhân này và cấu trúc môđun $A$ phân bậc trên E xác định trên E một cấu trúc đại số $A$ phân bậc kiểu $\Delta$; E, với cấu trúc này, được gọi là giới hạn trực tiếp của hệ trực tiếp $(E_\alpha, f_{\beta \alpha})$ của các đại số phân bậc. Các đồng cấu chính tắc $E_\alpha \to E$ được xem là các đồng cấu đại số phân bậc trên $A_\alpha$. Hơn nữa, nếu F là một đại số $A$ phân bậc kiểu $\Delta$ và $(u_\alpha)$ là một hệ trực tiếp của các đồng cấu trên $A_\alpha$ $u_\alpha: E_\alpha \to F$, $u = \lim \to u_\alpha$ là một đồng cấu đại số phân bậc trên A.

### 3. BÀI TẬP {#alg-iii-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
