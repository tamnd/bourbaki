---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 1
section_title: Notion of an integral element
lang: vi
source: ac-i-vii
book_pages: 303-324, 355-362
pdf_pages: 0322-0343, 0374-0381
extraction: ocr
subsections:
    - "no": 1
      title: INTEGRAL ELEMENTS OVER A RING
      page: 303
      pdf_page: 322
    - "no": 2
      title: THE INTEGRAL CLOSURE OF A RING. INTEGRALLY CLOSED DOMAINS
      page: 308
      pdf_page: 327
    - "no": 3
      title: EXAMPLES OF INTEGRALLY CLOSED DOMAINS
      page: 309
      pdf_page: 328
    - "no": 4
      title: COMPLETELY INTEGRALLY CLOSED DOMAINS
      page: 312
      pdf_page: 331
    - "no": 5
      title: THE INTEGRAL CLOSURE OF A RING OF FRACTIONS
      page: 314
      pdf_page: 333
    - "no": 6
      title: NORMS AND TRACES OF INTEGERS
      page: 316
      pdf_page: 335
    - "no": 7
      title: EXTENSION OF SCALARS IN AN INTEGRALLY CLOSED ALGEBRA
      page: 318
      pdf_page: 337
    - "no": 8
      title: INTEGERS OVER A GRADED RING
      page: 320
      pdf_page: 339
    - "no": 9
      title: 'APPLICATION: INVARIANTS OF A GROUP OF AUTOMORPHISMS OF AN ALGEBRA'
      page: 323
      pdf_page: 342
statements: 69
exercises: 29
content_sha256: c9fe750c6079f11c6c7838202df8d0d10209a7b299de7dca04ce287045928b32
translated_from: content/en/ac/V/01_s1_notion_of_an_integral_element.md
source_content_sha256: 2f79a65f77c0aff7fecf7b74bea588fece9fce74137af610f9bfb9d0274e5dc9
translation_model: gpt-5-6-mini, gpt-5.4-mini, gpt-5-mini
translation_run: translate-vi-341390b7
glossary_version: 34
glossary_terms_sha256: 097f3b5095c4af56d39d6edaafe8fb61200e5deb6a63873ad6ac093e6200c808
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. KHÁI NIỆM VỀ PHẦN TỬ NGUYÊN

### 1. CÁC PHẦN TỬ NGUYÊN TRÊN MỘT VÀNH

#### Định lý 1 {#ac-v-s1-thm-1 .statement}

Cho $\mathbf{A}$ là một vành (giao hoán), $\mathbf{R}$ là một đại số trên $\mathbf{A}$ (không nhất thiết giao hoán) và $x$ là một phần tử của $\mathbf{R}$. Các tính chất sau là tương đương:

(E₁) $x$ là một nghiệm của một đa thức đơn khởi trong vành đa thức $\mathbf{A}[X]$.
(E₂) Đại số con $\mathbf{A}[x]$ của $\mathbf{R}$ là một $\mathbf{A}$-môđun sinh hữu hạn.
(E₃) Tồn tại một môđun trung thành trên vành $\mathbf{A}[x]$ là một $\mathbf{A}$-môđun sinh hữu hạn.

Trước hết ta chứng minh rằng (E₁) kéo theo (E₂). Cho
$$
X^n + a_1 X^{n-1} + \ldots + a_n
$$
là một đa thức đơn khởi trong $\mathbf{A}[X]$ có $x$ là một nghiệm; với mỗi số nguyên $q \geq 0$ cho $M_q$ là môđun con-$\mathbf{A}$ của $\mathbf{R}$ sinh bởi $1, x, \ldots, x^n + q$. Khi đó
$$
x^{n+q} = -a_{n+q-1} x^{n+q-1} - \ldots - a_n x^q \in M_{-1}
$$
với mọi $q \geq 1$, do đó, bằng quy nạp theo $q$,
$$
M_q = M_{q-1} = \cdots = M_0.
$$

(*) Các kết quả của chương này và chương tiếp theo không phụ thuộc vào Sách nào khác ngoài các Sách I đến VI, cũng không phụ thuộc vào Chương I, § 4, cũng không phụ thuộc vào Chương 111, § 5.

Ta kết luận rằng $A[x]$ bằng $M_0$ và do đó là một $A$-môđun sinh hữu hạn.

Vì vành giao hoán $A[x]$ là một môđun trung thành trên chính nó, ($E_{II}$) kéo theo ($E_{III}$).

Cuối cùng, sự kiện ($E_{III}$) kéo theo ($E_1$) sẽ suy ra từ bổ đề chính xác hơn sau đây:

#### Bổ đề 1 {#ac-v-s1-lem-1 .statement}

*Cho $A$ là một vành, $R$ là một đại số (không nhất thiết giao hoán) trên $A$ và $x$ là một phần tử của $R$. Cho $M$ là một môđun trung thành trên $A[x]$ là một $A$-môđun sinh hữu hạn. Nếu $q$ là một iđêan của $A$ sao cho $xM \subset qM$, thì $x$ là một nghiệm của một đa thức đơn khởi với các hệ số trong $A$ tất cả $\notin$ mà các hệ số của nó khác hệ số trội đều thuộc $q$.*

Cho $(u_i)_{1 \leq i \leq n}$ là một họ hữu hạn các phần tử của $M$ sao cho $M = \sum_{i=1}^n Au_i$. Với mọi $i$, theo giả thiết tồn tại một họ hữu hạn $(q_{ij})_{1 \leq j \leq n}$ các phần tử của $q$ sao cho

$$
xu_i = \sum_{j=1}^n q_{ij}u_j \quad \text{cho} \quad 1 \leq i \leq n.
$$

Do đó (*Đại số*, Chương III, § 8), nếu $d$ là định thức của ma trận $(q_{ij} - \delta_{ij}x)$ với các phần tử trong $A[x]$ ($\delta_{ij}$ biểu thị chỉ số Kronecker), thì $du_i = 0$ với mọi $i$ và do đó $dM = 0$; vì $M$ được giả thiết là một $A[x]$-môđun trung thành, nhất thiết $d = 0$. Điều này có nghĩa là $x$ là một nghiệm của đa thức $\det(q_{ij} - \delta_{ij}X)$ trong $A[X]$, đa thức này, sai khác một dấu, là một đa thức đơn khởi mà các hệ số khác hệ số đầu thuộc về $q$.

#### Định nghĩa 1 {#ac-v-s1-def-1 .statement}

*Cho $A$ là một vành và $R$ là một $A$-đại số (không nhất thiết giao hoán). Một phần tử $x \in R$ được gọi là nguyên trên $A$ nếu nó thỏa mãn các tính chất tương đương ($E_1$), ($E_{II}$), ($E_{III}$) của Định lý 1.*

Một quan hệ có dạng $P(x) = 0$, trong đó $P$ là một đa thức *đơn khởi* trong $A[X]$, cũng được gọi là một *phương trình phụ thuộc nguyên* với các hệ số trong $A$.

*Ví dụ*

#### Ví dụ 1 {#ac-v-s1-n1-exa-1 .statement}

Cho $K$ là một trường (giao hoán) và $R$ là một $K$-đại số; nói rằng một phần tử $x \in R$ là nguyên trên $K$ tương đương với nói rằng $x$ là một nghiệm của một đa thức *không hằng* trong vành $K[X]$; tổng quát hóa thuật ngữ được đưa vào khi $R$ là một *mở rộng* của $K$ (*Đại số*, Chương V, § 3, no. 3), các phần tử $x \in R$ nguyên trên $K$ còn được gọi là các phần tử *đại số* của $R$ trên $K$.

*(2)* Các phần tử *của* $\mathbf{Q}(i)$ nguyên trên $\mathbf{Z}$ là các phần tử có dạng $a + ib$ trong đó $a \in \mathbf{Z}$ và $b \in \mathbf{Z}$ ("*các số nguyên Gaussian*"'); các phần tử của $\mathbf{Q}(\sqrt{5})$ nguyên trên $\mathbf{Z}$ là các phần tử *có* dạng $(a + b\sqrt{5})/2$ trong đó $a$ và $b$ thuộc $\mathbf{Z}$ và cả hai đều chẵn hoặc cả hai đều lẻ (đối với hai ví dụ này xem Bài tập 1).

(3) Các số phức nguyên trên $\mathbf{Z}$ còn được gọi là các số nguyên đại số.

Nhận xét

(1) Cho $A'$ là vành con của $R$ (được chứa trong tâm của $R$) là ảnh của $A$ qua đồng cấu vành $A \to R$ xác định cấu trúc đại số trên $A$ của $R$. Rõ ràng là tương đương khi nói rằng một phần tử của $R$ là nguyên trên $A$ hoặc là nguyên trên $A'$.

#### Ví dụ 2 {#ac-v-s1-n1-exa-2 .statement}

Cho $R'$ là một đại số con trên $A$ của $R$; các phần tử của $R'$ nguyên trên $A$ chính là các phần tử của $R$ nguyên trên $A$ và thuộc $R'$; điều này thường cho phép ta không cần chỉ rõ đại số mà một phần tử nguyên trên $A$ thuộc về, khi không thể có sự nhầm lẫn.

#### Mệnh đề 1 {#ac-v-s1-prop-1 .statement}

*Cho $A$ là một vành, $R$ là một đại số trên $A$ (không nhất thiết giao hoán) và $x$ là một phần tử của $R$. Để $x$ nguyên trên $A$, cần và đủ rằng $A[x]$ được chứa trong một đại số con $R'$ của $R$ là một A-môđun sinh hữu hạn.*

Điều kiện này hiển nhiên là cần do tính chất (E_{II}); nó cũng đủ do (E_{III}), vì $R'$ là một $A[x]$-môđun trung thành (vì nó chứa phần tử đơn vị của $R$).

#### Hệ quả {#ac-v-s1-n1-cor-1 .statement}

*Cho $A$ là một vành Noether, $R$ là một $A$-đại số (không nhất thiết giao hoán) và $x$ là một phần tử của $R$. Để $x$ nguyên trên $A$, cần và đủ rằng tồn tại một A-môđun con sinh hữu hạn của $R$ chứa $A[x]$.*

Điều kiện này là cần do (E_{II}); nó đủ, vì nếu $A[x]$ là một A-môđun con của một A-môđun sinh hữu hạn, thì chính nó là một A-môđun sinh hữu hạn (*Đại số*, Chương VIII, § 2, no. 3, Mệnh đề 7).

Giả thiết rằng $A$ là Noether không thể bỏ khỏi mệnh đề (Bài tập 2).

#### Định nghĩa 2 {#ac-v-s1-def-2 .statement}

*Cho $A$ là một vành. Một đại số trên $A$ $R$ (không nhất thiết giao hoán) được gọi là nguyên trên $A$ nếu mọi phần tử của $R$ đều nguyên trên $A$. $R$ được gọi là hữu hạn trên $A$ nếu $R$ là một A-môđun sinh hữu hạn.*

Từ Mệnh đề 1 suy ra rằng mọi đại số trên $A$ hữu hạn đều là nguyên; nếu $R$ giao hoán và là một đại số trên $A$ hữu hạn, thì hiển nhiên $R$ là một đại số trên $A$ sinh hữu hạn; điều đảo lại là sai.

*Ví dụ (4)* Nếu $M$ là một $A$-môđun sinh hữu hạn, thì đại số $\mathrm{End}_A(M)$ của các tự đồng cấu của $M$ là nguyên trên $A$ nhờ (E_{III}); đặc biệt, với mọi số nguyên $n$, đại số ma trận $M_n(A) = \mathrm{End}_A(A^n)$ là nguyên (và thậm chí hữu hạn) trên $A$.

#### Mệnh đề 2 {#ac-v-s1-prop-2 .statement}

*Cho $A, A'$ là hai vành, $R$ là một $A$-đại số, $R$ là một $A'$-đại số (không nhất thiết giao hoán) và $f : A \to A'$ cùng $g : R \to R'$ là hai đồng cấu vành sao cho biểu đồ

$$
\begin{array}{ccc}
A & \xrightarrow{f} & A' \\
| & & | \\
\mathbf{R} & \xrightarrow{g} & \mathbf{R}'
\end{array}
$$

là giao hoán. Nếu một phần tử $x \in R$ nguyên trên $A$ thì $g(x)$ nguyên trên $A'$.

Nếu $x^n + a_1 x^{n-1} + \cdots + a_n = 0$ trong đó $a_i \in A$ với $1 \leq i \leq n$, ta suy ra rằng

$$
(g(x))^n + f(a_1)(g(x))^{n-1} + \cdots + f(a_n) = 0.
$$*

#### Hệ quả 1 {#ac-v-s1-prop-2-cor-1 .statement}

*Cho $A$ là một vành, $B$ là một $A$-đại số (giao hoán) và $C$ là một $B$-đại số (không nhất thiết giao hoán). Khi đó mọi phần tử $x \in C$ nguyên trên $A$ đều nguyên trên $B$.*

#### Hệ quả 2 {#ac-v-s1-prop-2-cor-2 .statement}

*Cho $K$ là một trường, $L$ là một mở rộng của $K$ và $x, x'$ là hai phần tử của $L$ liên hợp trên $K$ (Đại số, Chương V, § 6, no. 2). Nếu $A$ là một vành con của $K$ và $x$ nguyên trên $A$, thì $x'$ cũng nguyên trên $A$.*

Tồn tại một $K$-đẳng cấu $f$ của $K(x)$ lên $K(x')$ sao cho $f(x) = x'$ và các phần tử của $A$ bất biến dưới $f$.

#### Hệ quả 3 {#ac-v-s1-prop-2-cor-3 .statement}

*Cho $A$ là một vành, $B$ là một $A$-đại số (giao hoán) và $C$ là một $B$-đại số (không nhất thiết giao hoán). Nếu $C$ nguyên trên $A$, thì $C$ nguyên trên $B$.*

#### Mệnh đề 3 {#ac-v-s1-prop-3 .statement}

*Cho $(R_i)_{1 \leq i \leq n}$ là một họ hữu hạn các đại số trên $A$ (không nhất thiết giao hoán) và cho $R = \prod_{i=1}^n R_i$ là tích của chúng. Để một phần tử $x = (x_i)_{1 \leq i \leq n}$ của $R$ nguyên trên $A$, điều kiện cần và đủ là mỗi $x_i$ đều nguyên trên $A$. Để $R$ nguyên trên $A$, điều kiện cần và đủ là mỗi $R_i$ đều nguyên trên $A$.*

Hiển nhiên chỉ cần chứng minh mệnh đề thứ nhất. Điều kiện này là cần theo Mệnh đề 2. Ngược lại, nếu mỗi $x_i$ đều nguyên trên $A$, thì đại số con $A[x_i]$ của $R_i$ là một $A$-môđun hữu hạn sinh và do đó đại số con $\prod_{i=1}^n A[x_i]$ của $R$ cũng vậy; vì $A[x]$ được chứa trong đại số con này, nên $x$ nguyên trên $A$ theo Mệnh đề 1.

#### Mệnh đề 4 {#ac-v-s1-prop-4 .statement}

*Cho $A$ là một vành, $R$ là một đại số trên $A$ (không nhất thiết giao hoán) và $(x_i)_{1 \leq i \leq n}$ là một họ hữu hạn các phần tử của $R$ từng đôi một giao hoán. Nếu, với mọi $i$, $x_i$ nguyên trên $A[x_1, \ldots, x_{i-1}]$ (và đặc biệt nếu mọi $x_i$ đều nguyên trên $A$), thì đại số con $A[x_1, \ldots, x_n]$ của $R$ là một $A$-môđun hữu hạn sinh.*

Ta chứng minh bằng quy nạp theo $n$, mệnh đề này chỉ là (E_{II}) khi $n = 1$. Giả thiết quy nạp suy ra rằng $B = A[x_1, \ldots, x_{n-1}]$ là một A-môđun hữu hạn sinh; vì $x_n$ nguyên trên $B$, nên $B[x_n] = A[x_1, \ldots, x_n]$ là một B-môđun hữu hạn sinh và do đó cũng là một A-môđun hữu hạn sinh (Đại số, Chương II, § 1, no. 13, Mệnh đề 25).

#### Hệ quả 1 {#ac-v-s1-prop-4-cor-1 .statement}

Cho $A$ là một vành và $R$ là một A-đại số (giao hoán). Tập hợp các phần tử $\& R$ nguyên trên $A$ là một đại số con của $R$.

Thật vậy, nếu $x, y$ là hai phần tử của $R$ nguyên trên $A$, thì từ Mệnh đề 4 suy ra $A[x, y]$ là một A-môđun hữu hạn sinh; vì nó chứa $x + y$ và $xy$, hệ quả suy ra từ Mệnh đề 1.

Trong một đại số không giao hoán, tổng và tích của hai phần tử nguyên trên $A$ không nhất thiết nguyên trên $A$ (Bài tập 4).

#### Hệ quả 2 {#ac-v-s1-prop-4-cor-2 .statement}

Cho $A$ là một vành, $R$ là một đại số trên A (không nhất thiết giao hoán) và $E$ là một tập hợp $\&$ phần tử $\& R$ từng đôi một giao hoán với nhau và nguyên trên $A$. Khi đó đại số con trên A $B \& R$ sinh bởi $E$ là nguyên trên $A$.

Mọi phần tử của $B$ đều thuộc một đại số con trên A của $B$ được sinh bởi một tập con hữu hạn của $E$.

Nhận xét (3) Suy ra từ Mệnh đề 4 rằng mọi đại số giao hoán trên A nguyên trên $A$ là hợp của một họ có hướng phải của các đại số con hữu hạn trên $A$.

#### Mệnh đề 5 {#ac-v-s1-prop-5 .statement}

Cho $A$ là một vành và $A$ và $R$ là hai đại số trên A (giao hoán). Nếu $R$ là nguyên trên $A$, thì $R \otimes_A A'$ là nguyên trên $A'$.

Xét một phần tử bất kỳ $x' = \sum_{i=1}^n x_i \otimes a'_i$ của $R \otimes_A A'$, trong đó các $x_i$ thuộc $R$ và các $a'_i$ thuộc $A'$; vì $x_i \otimes a'_i = (x_i \otimes 1)a'_i$ và các $x_i \otimes 1$ là nguyên trên $A'$ (Mệnh đề 2), nên $x$ cũng vậy.

#### Hệ quả {#ac-v-s1-n1-cor-2 .statement}

Cho $R$ là một vành và $A, B, C$ là các vành con $\& R$ sao cho $A \subset B$. Nếu $B$ là nguyên trên $A$, thì $C[B]$ là nguyên trên $C[A]$.

$B \otimes_A C[A]$ là nguyên trên $C[A]$ theo Mệnh đề 5 và do đó ảnh chính tắc $C[B]$ của $B \otimes_A C[A]$ trong $R$ (được xem như một đại số trên A) cũng vậy theo Mệnh đề 2.

#### Mệnh đề 6 {#ac-v-s1-prop-6 .statement}

Cho $A$ là một vành, $B$ là một đại số trên A (giao hoán) và $C$ là một đại số trên B (không nhất thiết giao hoán). Nếu $B$ là nguyên trên $A$ và $C$ là nguyên trên $B$, thì $C$ là nguyên trên $A$.

Ta chỉ cần kiểm tra rằng mọi $x \in C$ đều nguyên trên $A$. Theo giả thiết tồn tại một đa thức đơn khởi $X^n + b_1 X^{n-1} + \cdots + b$, với các hệ số trong $B$ nhận $x$ làm nghiệm; khi đó $x$ là nguyên trên $B' = A[b_1, \ldots, b_n]$ và $B'[x]$ do đó là một B-môđun sinh hữu hạn. Nhưng vì $B$ nguyên trên $A$, $B'$ là một A-môđun sinh hữu hạn (Mệnh đề 4); ta kết luận rằng B'[x] cũng là một A-môđun sinh hữu hạn (Đại số, Chương 11, § 1, no. 13, Mệnh đề 25) và do đó x là nguyên trên A.

#### Hệ quả {#ac-v-s1-n1-cor-3 .statement}

*Cho A là một vành và R, R' là hai đại số trên A (giao hoán) nguyên trên A. Khi đó R $\otimes_A$ R' là nguyên trên A.*

$R \otimes_A R$ là nguyên trên R (Mệnh đề 5) và do đó hệ quả suy ra từ Mệnh đề 6.

### 2. BAO ĐÓNG NGUYÊN CỦA MỘT VÀNH. CÁC MIỀN NGUYÊN ĐÓNG

#### Định nghĩa 3 {#ac-v-s1-def-3 .statement}

*Cho A là một vành và R là một đại số trên A (giao hoán). Đại số con-A A' của R gồm các phần tử của R nguyên trên A (no. 1, Hệ quả 1 của Mệnh đề 4) được gọi là bao đóng nguyên của A trong R. Nếu A' bằng ảnh chính tắc của A trong R, thì A được gọi là đóng nguyên trong R.*

Nhận xét

(1) Nếu $h : A \to R$ là đồng cấu vành xác định cấu trúc đại số trên A của R, thì bao đóng nguyên của A trong R cũng là bao đóng nguyên của $h(A)$ trong R. Mặt khác, nếu R' là một đại số con của R, thì bao đóng nguyên của A trong R' là $A' \cap R'$.

(2) Nếu A là một trường, bao đóng nguyên $A'$ của A trong R gồm các phần tử của R đại số trên A (no. 1, Ví dụ 1); tổng quát hóa thuật ngữ được dùng cho các mở rộng trường (Đại số, Chương V, § 3, no. 3), khi đó A' còn được gọi là bao đóng đại số của trường A trong đại số R và A được gọi là đóng đại số trong R nếu $A' = A$.

#### Định nghĩa 4 {#ac-v-s1-def-4 .statement}

*Nếu A là một miền nguyên, bao đóng nguyên của A trong trường phân thức của nó được gọi là bao đóng nguyên của A. Một miền nguyên được gọi là đóng nguyên nếu nó bằng bao đóng nguyên của nó.*

Chú ý rằng một miền nguyên đóng nguyên không nhất thiết đóng trong mọi vành chứa nó, như ví dụ về một trường không đóng đại số chỉ ra.

#### Mệnh đề 7 {#ac-v-s1-prop-7 .statement}

*Cho A là một vành và R là một đại số trên A. Bao đóng nguyên A' của A trong R là một vành con đóng nguyên trong R.*

Bao đóng nguyên của A' trong R là nguyên trên A theo no. 1, Mệnh đề 6; do đó nó bằng A'.

#### Hệ quả {#ac-v-s1-n2-cor-1 .statement}

*Bao đóng nguyên của một miền nguyên A là một miền nguyên đóng nguyên.*

Gọi K là trường phân thức của A và B là bao đóng nguyên của A. Rõ ràng

K là trường phân thức của B và chỉ cần áp dụng Mệnh đề 7 cho $R = K$.

#### Mệnh đề 8 {#ac-v-s1-prop-8 .statement}

*Cho $R$ là một vành, $(B_\lambda)_{\lambda \in L}$ là một họ các vành con của $R$ và với mỗi $\lambda \in L$ cho $A_\lambda$ là một vành con của $B_\lambda$. Nếu mỗi $A_\lambda$ đóng nguyên trong $B_\lambda$, thì $A = \bigcap_{\lambda \in L} A_\lambda$ đóng nguyên trong $B = \bigcap_{\lambda \in L} B_\lambda$.*

Điều này suy ra ngay lập tức từ Định nghĩa 3 và no. 1, Hệ quả 1 của Mệnh đề 2.

#### Hệ quả {#ac-v-s1-n2-cor-2 .statement}

*Mọi giao của một họ không rỗng các miền con đóng nguyên của một miền nguyên $A$ là một miền nguyên đóng nguyên.*

Chỉ cần áp dụng Mệnh đề 8 bằng cách lấy $R$ và các $B_\lambda$ bằng trường phân thức $K$ của $A$ và nhận xét rằng một vành con của $K$ đóng nguyên trong $K$ là *a fortiori* một miền nguyên đóng nguyên vì trường phân thức của nó được chứa trong $K$.

#### Mệnh đề 9 {#ac-v-s1-prop-9 .statement}

*Cho $A$ là một vành, $(R_i)_{1 \leq i \leq n}$ là một họ hữu hạn các đại số trên $A$ và $A'_i$ là bao đóng nguyên của $A$ trong $R_i$, $(1 \leq i \leq n)$. Khi đó bao đóng nguyên của $A$ trong $R = \prod_{i=1}^n R_i$, bằng $\prod_{i=1}^n A'_i$.*

Đây là một hệ quả ngay lập tức của no. 1, Mệnh đề 3.

#### Hệ quả 1 {#ac-v-s1-prop-9-cor-1 .statement}

*Cho $A$ là một vành Noether rút gọn, $p_i$ $(1 \leq i \leq n)$ là các iđêan nguyên tố tối tiểu phân biệt của nó, $K$, trường phân thức của miền nguyên $A/p_i$ (đẳng cấu chính tắc với vành địa phương $A_{p_i}$ (Chương IV, § 2, no. 5, Mệnh đề 10)) và $A'_i$ là bao đóng nguyên của $A$ trong $K$, $(1 \leq i \leq n)$. Khi đó đẳng cấu chính tắc của vành phân thức tổng $B$ của $A$ lên $\prod_{i=1}^n K_i$ (loc. cit.) gửi bao đóng nguyên của $A$ trong $B$ lên vành tích $\prod_{i=1}^n A'_i$.*

#### Hệ quả 2 {#ac-v-s1-prop-9-cor-2 .statement}

*Một vành Noether rút gọn là đóng nguyên trong vành phân thức của nó khi và chỉ khi nó là một hợp thành trực tiếp của các miền (Noether) đóng nguyên.*

### 3. CÁC VÍ DỤ VỀ MIỀN ĐÓNG NGUYÊN

#### Mệnh đề 10 {#ac-v-s1-prop-10 .statement}

*Mọi miền iđêan chính đều đóng nguyên.*

Cho $A$ là một miền iđêan chính, $K$ là trường phân thức của nó và $x$ là một phần tử của $K$. Tồn tại hai phần tử nguyên tố cùng nhau $a, b$ của $A$ sao cho $x = ab^{-1}$ (*Đại số*, Chương VII, § 1, no. 2, Mệnh đề 1 và Chương VI, § 1, no. 11, Mệnh đề 9 (DIV)). Nếu $x$ nguyên trên $A$, thì nó là một nghiệm của một đa thức

X^n + c_1 X^{n-1} + \ldots + c_n \text{ của } A[X]. Khi đó $a^n = b(-c_1 a^{n-1} - \ldots - c_n b^{n-1})$, điều đó chứng tỏ rằng $b$ chia $a''$. Vì $a$ và $b$ nguyên tố cùng nhau, suy ra $b$ khả nghịch trong $A$ (*Đại số*, Chương VI, § 1, no. 12, Hệ quả 1 của Mệnh đề 11 (DIV)); do đó $x \in A$.

#### Bổ đề 2 {#ac-v-s1-lem-2 .statement}

*Cho R là một vành và P là một đa thức đơn khởi trong R[X]. Tồn tại một vành R' chứa R sao cho trong vành đa thức R'[X], đa thức P là một tích của các đa thức đơn khởi bậc 1.*

Ta chứng minh bằng quy nạp theo bậc $n$ của P, bổ đề là hiển nhiên với $n = 0$ và $n = 1$. Vì thế giả sử $n > 1$. Cho $a$ là iđêan của $R[X]$ được sinh bởi P và cho $f$ là đồng cấu chính tắc của $R[X]$ lên $B = R[X]/a$. Vì P là đơn khởi, với mọi đa thức $Q \in R[X]$, $\deg(PQ) = \deg(P) + \deg(Q)$, do đó $a \cap R = 0$; vì thế hạn chế của $f$ lên R là đơn ánh. Đồng nhất R với vành con $f(R)$ của B qua $f$ và viết $b = f(X)$, ta thấy rằng $b$ là một nghiệm của P trong B, P được xét như một đa thức trong $B[X]$. Khi đó tồn tại một đa thức đơn khởi Q trong $B[X]$ bậc $n - 1$ sao cho $P(X) = (X - b)Q(X)$ (*Đại số*, Chương IV, § 1, no. 4, Mệnh đề 5). Theo giả thiết quy nạp tồn tại một vành $R' \supseteq B$ sao cho trong $R'[X]$ đa thức Q là một tích của các đa thức đơn khởi bậc 1; hiển nhiên trong $R'[X]$ khi đó P là một tích của các đa thức đơn khởi bậc 1.

#### Mệnh đề 11 {#ac-v-s1-prop-11 .statement}

*Cho A là một vành, R là một A-đại số và P và Q là các đa thức đơn khởi trong R[X]. Nếu các hệ số của PQ nguyên trên A, thì các hệ số của P và Q nguyên trên A.*

Bằng cách áp dụng kép Bổ đề 2, ta thấy rằng tồn tại một vành R' chứa R và các họ phần tử $(a_i)_{1 \leq i \leq m}, (b_j)_{1 \leq j \leq n}$ của R' sao cho trong $R'[X]$
$$
P(X) = \prod_{i=1}^\infty (X - a_i), \quad Q(X) = \prod_{j=1}^n (X - b_j);
$$
các hệ số của P Q thuộc bao đóng nguyên $A'$ của A trong R' và do đó (no. 2, Mệnh đề 7) các phần tử $a, (1 \leq i \leq m)$ và $b, (1 \leq j \leq n)$ thuộc A. Suy ra rằng các hệ số của P và Q là nguyên trên A (no. 1, Hệ quả 1 của Mệnh đề 4).

Cho A là một miền nguyên, K là trường các phân thức của nó và K' là một đại số trên K (không nhất thiết giao hoán). Cho một phần tử $x \in K'$ đại số trên K, các đa thức $P \in K[X]$ sao cho $P(x) = 0$ tạo thành một iđêan $a \neq 0$ của $K[X]$, nhất thiết chính (Đại số, Chương IV, § 1, no. 5, Mệnh đề 7). Tồn tại một đa thức đơn khởi duy nhất sinh ra a; bằng cách mở rộng thuật ngữ đã đưa vào trong Đại số, Chương V, § 3, no. 1, Định nghĩa 3, đa thức đơn khởi này sẽ được gọi là đa thức tối tiểu của x trên K.

#### Hệ quả {#ac-v-s1-n3-cor-1 .statement}

*Cho A là một miền nguyên, K là trường các phân thức của nó và x là một phần tử của một đại số trên K K* (không nhất thiết giao hoán). *Nếu x là nguyên trên A, các hệ số của đa thức tối tiểu $P$ của $x$ trên $K$ là nguyên trên $A$ (và do đó chúng thuộc $A$ nếu $A$ đóng nguyên).

Theo giả thiết (no. 1, Định lý 1), tồn tại một đa thức đơn khởi $Q \in A[X]$ sao cho $Q(x) = 0$. Vì $P$ chia $Q$ trong $K[X]$, suy ra từ Mệnh đề 11 rằng các hệ số của $P$ là nguyên trên $A$.

Cho $A$ là một vành và $R$ là một đại số trên $A$ (giao hoán); đồng cấu $\phi : A \to R$ xác định cấu trúc đại số trên $A$ của $R$ có thể được mở rộng duy nhất thành một đồng cấu $A[X] \to R[X]$ của các vành đa thức trên $A$ và $R$, giữ $X$ bất biến và do đó $R[X]$ được trang bị một cấu trúc đại số trên $A[X]$ chính tắc.

#### Mệnh đề 12 {#ac-v-s1-prop-12 .statement}

Cho $A$ là một vành, $R$ là một đại số trên $A$ và $P$ là một đa thức trong $R[X_1, \ldots, X_n]$. Để $P$ là nguyên trên $A[X_1, \ldots, X_n]$, điều kiện cần và đủ là các hệ số của $P$ là nguyên trên $A$.

Bằng cách xem các đa thức của $R[X_1, \ldots, X_n]$ như các đa thức theo $X$, với các hệ số trong $R[X_1, \ldots, X_{n-1}]$, ta thấy ngay lập tức rằng quy về việc chứng minh mệnh đề cho $n = 1$. Khi đó cho $P$ là một đa thức trong $R[X]$; suy ra ngay lập tức từ no. 1, Mệnh đề 5 rằng, nếu các hệ số của $P$ thuộc bao đóng nguyên $B$ của $A$ trong $R$, phần tử $P$, thuộc $B[X] = B \otimes_A A[X]$, là nguyên trên $A[X]$. Ngược lại, giả sử rằng $P$ là nguyên trên $A[X]$ và cho

$$
Q(Y) = Y^m + F_1 Y^{m-1} + \cdots + F,
$$

là một đa thức đơn khởi với các hệ số $F_i \in A[X]$ có $P$ làm nghiệm. Cho $r$ là một số nguyên lớn hơn nghiêm ngặt tất cả các bậc của các đa thức $P$ và $F_i$ ($1 \leq i \leq m$) và ta viết

$$
P_1(X) = P(X) - X^r.
$$

Khi đó $P_1$ là nghiệm của đa thức

$$
Q_1(Y) = Q(Y + X') = Y^m + G_1 Y^{m-1} + \cdots + G,
$$

với các hệ số trong $A[X]$; do đó ta có thể viết

$$
-P_1(P_1^{m-1} + G_1 P_1^{m-2} + \cdots + G_{m-1}) = G_r
$$

Bây giờ lựa chọn $r$ kéo theo rằng $-P_1$ là một đa thức đơn khởi của $R[X]$ và $G_m(X) = Q(X^r)$ cũng vậy, các bậc của các đa thức $F_k(X) X^{r(m-k)}$ đều $< rm$ với $k \geq 1$. Trước hết ta kết luận rằng đa thức

$$
P_1^{m-1} + G_1 P_1^{m-2} + \cdots + G_{m-1}
$$

của $R[X]$ cũng là đơn khởi; hơn nữa, vì các hệ số của $G_i$ thuộc về $A$, Mệnh đề 11 chỉ ra rằng $P_1$ có các hệ số nguyên trên $A$ và các hệ số của $P$ do đó chắc chắn là nguyên trên $A$.

#### Mệnh đề 13 {#ac-v-s1-prop-13 .statement}

Cho $A$ là một vành, $\mathbf{R}$ là một $A$-đại số và $A'$ là bao đóng nguyên của $A$ trong $\mathbf{R}$. Khi đó bao đóng nguyên của $A[X_1, \ldots, X_n]$ trong $\mathbf{R}[X_1, \ldots, X_n]$ bằng $A'[X_1, \ldots, X_n]$.

Điều này suy ra từ Mệnh đề 12 và Định nghĩa 3 của no. 2.

#### Hệ quả 1 {#ac-v-s1-prop-13-cor-1 .statement}

Cho $A$ là một miền nguyên và $A'$ là bao đóng nguyên của nó. Khi đó bao đóng nguyên của vành đa thức $A[X_1, \ldots, X_n]$ là $A'[X_1, \ldots, X_n]$.

Lập luận bằng quy nạp theo $n$, bài toán được rút gọn ngay lập tức về trường hợp $n = 1$. Cho $K$ là trường các phân thức của $A$, cũng là trường các phân thức của $A'$; nếu một phần tử $P$ của trường các phân thức $K(X)$ của $A[X]$ là nguyên trên $A[X]$, nó thuộc về vành đa thức $K[X]$, vì vành sau là một miền iđêan chính (Đại số, Chương IV, § 1, no. 5, Mệnh đề 7) và do đó đóng nguyên (Mệnh đề 10); hệ quả khi đó suy ra từ Mệnh đề 13 áp dụng cho $\mathbf{R} = K$.

#### Hệ quả 2 {#ac-v-s1-prop-13-cor-2 .statement}

Cho $A$ là một miền nguyên. Để vành đa thức $A[X_1, \ldots, X_n]$ đóng nguyên, điều kiện cần và đủ là $A$ đóng nguyên.

#### Hệ quả 3 {#ac-v-s1-prop-13-cor-3 .statement}

Nếu $K$ là một trường, mọi đại số đa thức $K[X_1, \ldots, X_n]$ đều là một miền đóng nguyên.

### 4. CÁC MIỀN NGUYÊN ĐÓNG HOÀN TOÀN

#### Định nghĩa 5 {#ac-v-s1-def-5 .statement}

Một miền nguyên $A$ được gọi là đóng nguyên hoàn toàn nếu điều kiện sau được thỏa mãn: mọi phần tử $x$ của trường phân thức $K$ của $A$ sao cho tất cả các lũy thừa $x^n$ ($n \geqslant 0$) được chứa trong một A-môđun con sinh hữu hạn của $K$, đều thuộc về $A$.

Chú ý rằng giả thiết các $x^n$ được chứa trong một A-môđun con sinh hữu hạn của $K$ cũng có thể được biểu diễn bằng cách nói rằng tồn tại một phần tử khác không $d \in A$ sao cho $dx^n \in A$ với mọi $n \geqslant 0$; vì điều kiện sau có nghĩa là $x^n \in Ad^{-1}$; và ngược lại, nếu $(b_i)_{1 \leqslant i \leqslant m}$ là một dãy hữu hạn các phần tử của $K$, thì tồn tại $d \in A$ sao cho $db_i \in A$ với $1 \leqslant i \leqslant m$, do đó $dM \subset A$ đối với A-môđun con $M$ của $K$ sinh bởi các $b_i$.

Rõ ràng một miền đóng nguyên hoàn toàn là đóng nguyên; ngược lại, Hệ quả của Mệnh đề 1 của no. 1 chỉ ra rằng một miền Noether đóng nguyên là đóng nguyên hoàn toàn. \* Mặt khác, vành của một định giá có chiều cao $\geqslant 2$ (Chương VI, § 4, no. 4) là đóng nguyên nhưng không đóng nguyên hoàn toàn. \* Nếu $(A_i)$ là một họ các miền đóng nguyên hoàn toàn có cùng trường phân thức $K$, thì $A = \bigcap_i A_i$ là đóng nguyên hoàn toàn. Thật vậy, nếu $x \in K$ là sao cho với một $d$ khác không nào đó trong $A$, $dx^n$ thuộc về $A$ với mọi $n > 0$, thì giả thiết suy ra rằng $x \in A$, với mọi $i$ và do đó $x \in A$.

#### Mệnh đề 14 {#ac-v-s1-prop-14 .statement}

*Cho $A$ là một miền nguyên đóng nguyên hoàn toàn. Khi đó mọi vành đa thức $A[X_1, \ldots, X_n]$ (tương ứng mọi vành chuỗi lũy thừa hình thức $A[[X_1, \ldots, X_n]]$) đều đóng nguyên hoàn toàn.*

Bằng quy nạp theo $n$, chỉ cần chứng minh rằng $A[X]$ (tương ứng $A[[X]]$) là đóng nguyên hoàn toàn. Khi đó cho $P$ là một phần tử của trường phân thức của $A[X]$ (tương ứng $A[[X]]$) và giả sử rằng tồn tại một phần tử khác không $Q \in A[X]$ (tương ứng $Q \in A[[X]]$) sao cho $Q P^m \in A[X]$ (tương ứng $Q P'' \in A[[X]]$) với mọi số nguyên $m \geq 0$. Nếu $K$ là trường phân thức của $A$, $A[X]$ (tương ứng $A[[X]]$) là một vành con của $K[X]$ (tương ứng $K[[X]]$) và $K[X]$ (tương ứng $K[[X]]$) là một miền iđêan chính (*Algebra*, Chương VII, § 1, no. 1) và do đó đóng nguyên (no. 4, Mệnh đề 10) và Noether (*Algebra*, Chương VIII, § 2, no. 3) và vì vậy đóng nguyên hoàn toàn; khi đó ta đã thấy rằng

$P \in K[X]$ (tương ứng $P \in K[[X]]$). Cho $P = \sum_{k=0}^{\infty} a_k X^k$ ($a_k \in K$) và $Q = \sum_{k=0}^{\infty} b_k X^k$ ($b_k \in A$) và ta lập luận bằng *phản chứng* bằng cách giả sử rằng các $a_i$ không phải tất cả đều thuộc $A$; khi đó tồn tại một chỉ số nhỏ nhất $i$ sao cho $a_i \notin A$; nếu ta viết

$$
P_1 = \sum_{k=0}^{i-1} a_k X^k \in A[X],
$$

thì suy ra ngay lập tức từ giả thiết rằng cũng có $Q(P - P_1)^m \in A[X]$ (tương ứng $Q(P - P_1)^m \in A[[X]]$) với mọi $m \geq 0$. Gọi $j$ là số nguyên nhỏ nhất sao cho $b_j \neq 0$; rõ ràng trong $Q(P - P_1)^m$, số hạng có bậc nhỏ nhất với hệ số $\neq 0$ là $b_j a_i^m X^{j + mi}$ và do đó $b_j a_i^m \in A$ với mọi $m \geq 0$; nhưng vì $A$ là đóng nguyên hoàn toàn, điều này kéo theo $a_i \in A$, trái với giả thiết.

#### Mệnh đề 15 {#ac-v-s1-prop-15 .statement}

*Cho $A$ là một vành lọc có lọc là đầy đủ và sao cho mọi iđêan chính của $A$ đều đóng đối với tôpô được xác định bởi lọc. Nếu vành phân bậc liên kết $\mathrm{gr}(A)$ (Chương III, § 2, no. 3) là một miền nguyên đóng nguyên hoàn toàn, thì $A$ là một miền nguyên đóng nguyên hoàn toàn.*

Cho $(A_n)_{n \in \mathbf{Z}}$ là lọc được xác định trên $A$; vì $\bigcap_{n \in \mathbf{Z}} A_n$, là bao đóng của iđêan (0) (Chương III, § 2, no. 5), giả thiết trước hết kéo theo rằng lọc $(A,,)$ là tách được và, vì $\mathrm{gr}(A)$ là một miền nguyên, nên $A$ cũng vậy (Chương III, § 2, no. 3, Hệ quả của Mệnh đề 1). Cho $x = b/a$ là một phần tử của trường các phân thức $K$ của $A$ ($a \in A, b \in A$) sao cho tồn tại một phần tử $d \neq 0$ của $A$ thỏa mãn $dx^n \in A$ với mọi $n \geq 0$. Ta phải chứng minh rằng $b \in A a$ và, vì theo giả thiết iđêan $A a$ là đóng, chỉ cần chỉ ra rằng, với mọi $n \in \mathbf{Z}, b \in A a + A$. Vì lọc của $A$ là đầy đủ, tồn tại một số nguyên $q \in \mathbf{Z}$ sao cho $b \in A a + A_q$. Do đó chỉ cần chứng minh rằng quan hệ $b \in A a + A_q$ kéo theo $b \in A a + A_{q+1}$.

Giả sử khi đó rằng $b = a y + z$ trong đó $y \in A, z \in A_{q+1}$. Khi đó theo giả thiết $dx^n \in A$ với mọi $n \geq 0$, do đó ta thu được ngay lập tức $d(x - y)^n \in A$ với mọi $n \geq 0$; nói cách khác, $dz^n = a^n t_n$ trong đó $t_n \in A$ với mọi $n \geq 0$. Ta hiển nhiên có thể giới hạn sự chú ý của mình vào trường hợp $z \neq 0$. Gọi $v$ là hàm cấp trên $A$ (chương III, § 1, no. 2) và viết $v(d) = n_1,\ v(z) = n_2 \geq m,\ v(a) = n_3$; gọi $d', z', a'$ là các ảnh tương ứng của $d, z, a$ trong $A_{n_1}/A_{n_1+1},\ A_{n_2}/A_{n_2+1},\ A_{n_3}/A_{n_3+1}$. Với mọi $n \geq 0,\ v(dz^n) = n_1 + nn_2$ (chương III, § 2, no. 3, Mệnh đề 1) và do đó ảnh chính tắc trong $\mathrm{gr}(A)$ của $dz^n$ là $d'{z'}^n$; tương tự, người ta thấy rằng ảnh chính tắc trong $\mathrm{gr}(A)$ của $a^n t_n$ có dạng ${d'}^n t'_n$ trong đó $t'_n \in \mathrm{gr}(A)$ và, vì $a' \neq 0$ ta suy ra rằng, với mọi $n \geq 0,\ d'(z'/a')^n \in \mathrm{gr}(A)$. Giả thiết rằng $\mathrm{gr}(A)$ là hoàn toàn nguyên đóng do đó kéo theo sự tồn tại của một $s' \in \mathrm{gr}(A)$ sao cho $z' = a's'$; phân tích $s'$ thành một tổng các phần tử thuần nhất, người ta còn thấy (vì $z'$ và $a'$ là thuần nhất) rằng có thể giả sử $s'$ là thuần nhất, nghĩa là ảnh của một phần tử $s \in A$; khi đó $v(as) = v(z) = n_2$ và $z \equiv as \pmod{A_{n_2+1}}$; vì $n_2 \geq m, a fortiori$ $z \equiv as \pmod{A_{m+1}}$, do đó $b \equiv a(y+s) \pmod{A,,+,}$.

### 5. ĐÓNG NGUYÊN CỦA MỘT VÀNH PHÂN THỨC

Cho $A$ là một vành, $R$ là một $A$-đại số và $S$ là một tập con nhân của $A$. Nhắc lại (chương II, § 2, no. 8) rằng $S^{-1}R$ có một cấu trúc $S^{-1}A$-đại số chính tắc.

#### Mệnh đề 16 {#ac-v-s1-prop-16 .statement}

*Cho $A$ là một vành, $R$ là một $A$-đại số, $A'$ là đóng nguyên của $A$ trong $R$ và $S$ là một tập con nhân của $A$. Khi đó đóng nguyên của $S^{-1}A$ trong $S^{-1}R$ là $S^{-1}A'$.*

Cho $b/s$ là một phần tử của $S^{-1}A'$ ($s \in S,\ b \in A'$). Vì biểu đồ

$$
\begin{array}{ccc}
A & \xrightarrow{i_A^S} & S^{-1}A \\
\downarrow h & & \downarrow S^{-1}h \\
R & \xrightarrow{i_R^S} & S^{-1}R
\end{array}
$$

là giao hoán, $b/1$ là nguyên trên $S^{-1}A$ (no. 1, Mệnh đề 2). Vì $1/s \in S^{-1}A$, $b/s = (b/1)(1/s)$ là nguyên trên $S^{-1}A$.

Ngược lại, cho $r/t \ (r \in R,\ t \in S)$ là một phần tử của $S^{-1}R$ nguyên trên $S^{-1}A$; khi đó $r/1 = (t/1)(r/t)$ là nguyên trên $S^{-1}A$. Khi đó tồn tại một quan hệ dạng

$$
(r/1)^n + (a_1/s)(r/1)^{n-1} + \cdots + (a_n/s) = 0,
$$

trong đó $a_i \in A \ (1 \leq i \leq n)$ và $s \in S$. Quan hệ này cũng có thể được viết

$$
(sr^n + a_1 r^{n-1} + \ldots + a_n)/s = 0
$$

và do đó tồn tại $s' \in S$ sao cho ${s'}^n(sr^n + a_1 r^{n-1} + \ldots + a_n) = 0$; ta suy ra rằng $(s'sr)^n + s'a_1(s'sr)^{n-1} + \ldots + {s'}^ns^{n-1}a_n = 0$. Theo định nghĩa, do đó $s'sr \in A'$, do đó $r/1 \in S^{-1}A'$ và $r/t \in S^{-1}A'$.

#### Hệ quả 1 {#ac-v-s1-prop-16-cor-1 .statement}

Cho $A$ là một miền nguyên, $A'$ là bao đóng nguyên của nó và $S$ là một tập con nhân của $A$ sao cho $0 \notin S$. Khi đó bao đóng nguyên của $S^{-1}A$ là $S^{-1}A'$.

Trường phân thức $R$ của $A$ cũng là trường phân thức của $S^{-1}A$ vì $0 \notin S$ (Chương II, § 1, no. 1, Nhận xét 7); khi đó Mệnh đề 16 được áp dụng cho $R$.

#### Hệ quả 2 {#ac-v-s1-prop-16-cor-2 .statement}

Cho $A$ là một miền nguyên, $K$ là trường phân thức của nó, $R$ là một đại số trên $K$ và $B$ là bao đóng nguyên của $A$ trong $R$. Các phần tử của $R$ đại số trên $K$ (no. 1, Ví dụ 1) là các phần tử có dạng $a^{-1} b$ trong đó $b \in B$ và $a \in A, a \neq 0$; nếu $L$ là bao đóng đại số của $K$ trong $R$, thì tồn tại một cơ sở của $L$ trên $K$ được chứa trong $B$.

Khẳng định đầu tiên suy ra từ Mệnh đề 16 áp dụng trong trường hợp $S = A - \{0\}$. Nếu $(x_i)_{i \in I}$ là một cơ sở của $L$ trên $K$, thì với mọi $i \in I$ tồn tại một phần tử $a_i \neq 0$ của $A$ sao cho $a_i x_i \in B$; khi đó $(a_i x_i)_{i \in I}$ cũng là một cơ sở của $L$ trên $K$.

#### Hệ quả 3 {#ac-v-s1-prop-16-cor-3 .statement}

Cho $A$ là một miền nguyên và $\Omega$ là tập hợp các iđêan cực đại của $A$. Để $A$ đóng nguyên, điều kiện cần và đủ là, với mọi $m \in \Omega$, $A_m$ đóng nguyên.

Điều kiện cần suy ra từ Hệ quả 1. Điều kiện đủ, vì $A = \bigcap_{m \in \Omega} A_m$ (Chương II, § 3, no. 3, công thức (2)) và chỉ cần áp dụng Hệ quả cho Mệnh đề 8 của no. 2.

#### Hệ quả 4 {#ac-v-s1-prop-16-cor-4 .statement}

Cho $A$ là một miền nguyên, $K$ là trường phân thức của nó và $S$ là một tập con nhân của $A$ sao cho $0 \notin S$.

(i) Cho $B$ là một vành con của $K$ nguyên trên $A$ và cho $\mathfrak{f}$ là linh hóa tử của $A$-môđun $B/A$. Khi đó $S^{-1}\mathfrak{f}$ được chứa trong linh hóa tử của $(S^{-1}A)$-môđun $S^{-1}B/S^{-1}A$ và bằng linh hóa tử này nếu $B$ là một $A$-môđun sinh hữu hạn.

(ii) Cho $A'$ là đóng nguyên của $A$. Để $S^{-1}A$ đóng nguyên, điều kiện đủ là linh hóa tử $\mathfrak{f}$ của $A$-môđun $A'/A$ gặp $S$. Điều kiện này cũng là cần nếu $A'$ là một $A$-môđun sinh hữu hạn.

(i) Vì $\mathfrak{f}B \subset A$, $(S^{-1}\mathfrak{f})(S^{-1}B) \subset S^{-1}A$ và do đó $S^{-1}\mathfrak{f}$ được chứa trong $\operatorname{Ann}(S^{-1}B/S^{-1}A)$. Nếu $B$ là một $A$-môđun sinh hữu hạn, đẳng thức $S^{-1}\mathfrak{f} = \operatorname{Ann}(S^{-1}B/S^{-1}A)$ là một trường hợp đặc biệt của công thức (9) của Chương II, § 2, no. 4, $S^{-1}B/S^{-1}A$ được đồng nhất một cách chính tắc với $S^{-1}(B/A)$.

(ii) Theo Hệ quả 1 $S^{-1}A'$ là đóng nguyên của $S^{-1}A$. Vì các quan hệ $\mathfrak{f} \cap S \neq \varnothing$ và $S^{-1}\mathfrak{f} = S^{-1}A$ là tương đương (Chương II, § 2, no. 5, Nhận xét), (ii) là một hệ quả ngay lập tức của (i).

Nếu $B$ là một vành con của $K$ nguyên trên $A$, linh hóa tử $f$ của $B/A$ (bằng theo định nghĩa với vành vận chuyển $A : B$ (Chương I, § 2, no. 10)) đôi khi được gọi là *vật dẫn* của $B$ trong $A$.

#### Hệ quả 5 {#ac-v-s1-prop-16-cor-5 .statement}

*Cho $A$ là một miền nguyên, $A'$ là bao đóng nguyên của nó và $f$ là linh hóa tử của $A$-môđun $A'/A$. Giả sử rằng $A'$ là một $A$-môđun sinh hữu hạn. Các iđêan nguyên tố $p \in A$ sao cho $A_p$ không đóng nguyên là những iđêan chứa $f$.*

Điều này suy ra ngay lập tức từ Hệ quả **4 (ii)** áp dụng cho $S = A - p$.

Chú ý rằng dưới các giả thiết của Hệ quả 5 $f \neq 0$ vì $A'$ là một $A$-môđun sinh hữu hạn và mọi phần tử của $K/A$ ($K$ là trường phân thức của $A$) có một linh hóa tử $\neq 0$.

*Trong hình học đại số, Hệ quả 5 và nhận xét trên chỉ ra rằng các điểm mà tại đó một đa tạp afin $V$ không chuẩn tạo thành một tập hợp đóng phân biệt với $V$.* \*

### 6. CHUẨN VÀ VẾT CỦA CÁC PHẦN TỬ NGUYÊN

#### Mệnh đề 17 {#ac-v-s1-prop-17 .statement}

*Cho $A$ là một vành, $B$ là một $A$-đại số (giao hoán) và $X$ là một ma trận vuông cấp $n$ trên $B$; các tính chất sau là tương đương:

(a) $X$ là nguyên trên $A$.

(b) Tồn tại một $A$-môđun con sinh hữu hạn $M$ của $B^n$ sao cho $X.x \in M$ với mọi $x \in M$ và $M$ là một hệ các phần tử sinh của $B$-môđun $B^n$.

(c) Các hệ số của đa thức đặc trưng của $X$ là nguyên trên $A$.*

Nếu $\chi(T) = \det(T.1 - X)$ là đa thức đặc trưng của $X$, Định lý Cayley-Hamilton chỉ ra rằng $\chi(X) = 0$ (*Đại số*, Chương VII, § 5, no. 4, *Nhận xét* 1) và, vì $\chi$ là một đa thức đơn khởi, (c) kéo theo (a) theo no. 1, Mệnh đề 6.

Trong trường hợp thứ hai, giả sử (a) đúng. Nếu $(e_i)_{1 \leq i \leq n}$ là cơ sở chính tắc của $B^n$, thì môđun con trên $A$ $M$ của $B$ được sinh bởi các $X^k.e_i$ ($1 \leq i \leq n, k \geq 0$) là một $A$-môđun sinh hữu hạn, vì $A$-đại số $A[X]$ là một $A$-môđun sinh hữu hạn (no. 1, Định lý 1); vì $M$ chứa các $e_i$, thấy rằng (a) suy ra (b); đảo lại là hệ quả của no. 1, Định lý 1, điều kiện (E_{III}).

Cuối cùng, ta chứng minh rằng (a) suy ra (c); vì $X$ nguyên trên $A$ và *a fortiori* trên vành đa thức $A[T]$, nên $T.1 - X$ cũng nguyên trên $A[T]$ và theo no. 3, Mệnh đề 12, bài toán được thấy là quy về (bằng cách thay $X$ bởi $T.1 - X$ và $A$ bởi $A[T]$) chứng minh rằng, nếu $X$ nguyên trên $A$, thì $d = \det(X)$ là một phần tử của $B$ nguyên trên $A$. Bây giờ, ta đã thấy ở trên rằng tự đồng cấu $u$ của $B^n$ do $X$ xác định giữ ổn định một môđun con trên $A$ sinh hữu hạn $M$ chứa các $e_i$; do đó các $n$-vectơ $x_1 \wedge x_2 \wedge \ldots \wedge x_n$, với $x_i \in M$ cho $1 \leq i \leq n$, sinh ra trong $\bigwedge^n(B^n)$ một môđun con trên $A$ sinh hữu hạn chứa $e_1 \wedge e_2 \wedge \ldots \wedge e,$ và ổn định dưới $\bigwedge^n u$, nói cách khác dưới phép vị tự có tỉ số $d$; vì linh hóa tử của

$$
e_1 \wedge e_2 \wedge \ldots \wedge e,
$$

trong $B$ giảm xuống 0, điều kiện (E_{III}) của no. 1, Định lý 1 chứng minh rằng $d$ nguyên trên $A$.

#### Hệ quả 1 {#ac-v-s1-prop-17-cor-1 .statement}

Cho $A$ là một miền nguyên, $K$ là trường phân thức của nó và $K'$ là một đại số $K$ hữu hạn chiều (không nhất thiết giao hoán). Nếu $x \in K'$ nguyên trên $A$, thì các hệ số của đa thức đặc trưng $Pc_{K'/K}(x; X)$ (Đại số, Chương VIII, § 12, no. 2) đều nguyên trên $A$.

Nếu $z \mapsto M(z)$ là biểu diễn chính quy của đại số $K'$ (xét như một biểu diễn ma trận; xem Đại số, Chương VIII, § 13) thì $Pc_{K'/K}(x; X)$ theo định nghĩa là đa thức đặc trưng của ma trận $M(x)$; nếu $x$ nguyên trên $A$, thì ma trận $M(x)$ nguyên trên $A$ (no. 1, Mệnh đề 2) và chỉ cần áp dụng Mệnh đề 17.

#### Hệ quả 2 {#ac-v-s1-prop-17-cor-2 .statement}

Với cùng các giả thiết và ký hiệu như trong Hệ quả 1, $Tr_{K'/K}(x)$ và $N_{K'/K}(x)$ đều nguyên trên $A$.

$Tr_{K'/K}(x)$ và $N_{K'/K}(x)$, tới một dấu, là các hệ số của $Pc_{K'/K}(x; X)$ (Đại số, Chương VIII, § 12, no. 1, các phương trình (4)) và do đó đều nguyên.

Nhận xét (1) Nếu $K'$ là một đại số trung tâm đơn trên $K$ và $x \in K'$ nguyên trên $A$, thì các hệ số của đa thức đặc trưng rút gọn của $x$ (Đại số, Chương VIII, § 12, no. 3) đều nguyên trên $A$. Thật vậy, có một lũy thừa của đa thức này bằng $Pc_{K'/K}(x; X)$ (loc. cit., Mệnh đề 8) và chỉ cần áp dụng Mệnh đề 17 và no. 3, Mệnh đề 11.

#### Mệnh đề 18 {#ac-v-s1-prop-18 .statement}

Cho $A$ là một miền nguyên đóng, $K$ là trường phân thức của nó, $K'$ là một đại số $K$ tách được hữu hạn chiều (Đại số, Chương VIII, § 7, no. 5) và $A'$ là bao đóng nguyên của $A$ trong $K'$. Khi đó $A'$ được chứa trong một $A$-môđun sinh hữu hạn.

Mệnh đề sẽ suy ra từ bổ đề chính xác hơn sau đây:

#### Bổ đề 3 {#ac-v-s1-lem-3 .statement}

Dưới các giả thiết của Mệnh đề 18, cho $(w_1, ..., w_n)$ là một cơ sở của $K'$ trên $K$ nằm trong $A'$ (no. 5, Hệ quả 2 của Mệnh đề 16); khi đó tồn tại duy nhất một cơ sở $(w_1^*, ..., w_n^*)$ của $K'$ trên $K$ sao cho $Tr_{K'/K}(w_i w_j^*) = \delta_{ij}$ (chỉ số Kronecker); nếu $d = D_{K'/K}(w_1, ..., w_n)$ là biệt thức của cơ sở $(w_1, ..., w_n)$ (Đại số, Chương IX, § 2), thì $d \neq 0$ và

$$
\sum_{i=1}^n Aw_i \subset A' \subset \sum_{i=1}^n Aw_i^* < d^{-1} \left( \sum_{i=1}^n Aw_i \right).
$$

Đặc biệt, nếu $d$ là một phần tử khả nghịch của A, thì $A'$ là một A-môđun tự do với cơ sở $(w_1, ..., w_n)$.

Vì $K'$ là một đại số $K$ tách được, nên $d \neq 0$ (Đại số, Chương IX, § 2, Mệnh đề 5) và dạng song tuyến tính trên K

$$
(x, y) \mapsto \operatorname{Tr}_{K'/K}(xy)
$$

trên K' do đó không suy biến (*loc. cit.*, Mệnh đề 4); điều này cho thấy sự tồn tại và tính duy nhất của cơ sở $(w_i^*)_{1 \leq i \leq n}$ (*Algebra*, Chương IX, § 1, no. 6, Hệ quả của Mệnh đề 6). Như vậy, bao hàm thức thứ nhất của (2) là hiển nhiên. Cho $x$ là một phần tử của $A'$; ta viết $x = \sum_{i=1}^n \xi_i w_i^*$ với $\xi_i \in K$; với mọi $i$, $\xi_i = \mathrm{Tr}_{K'/K}(xw_i)$, do đó $\xi_i$ là nguyên trên $A$ (Hệ quả 2 của Mệnh đề 17) và, vì $A$ là đóng nguyên, $\xi_i \in A$ với $1 \leq i \leq n$; điều này cho thấy bao hàm thức thứ hai (2). Cuối cùng, ta viết $w_j^* = \sum_{i=1}^n \alpha_{ji} w_i$ với $\alpha_{ji} \in K$; khi đó $$\sum_{i=1}^n \alpha_{ji} \mathrm{Tr}_{K'/K}(w_i w_k) = \delta_{jk}$$ với mọi $j$ và $k$; các công thức của Cramer cho thấy rằng các $\alpha_{ji}$ thuộc $d^{-1}A$, do đó bao hàm thức thứ ba (2). Khẳng định cuối cùng suy ra ngay lập tức từ (2), mà trong trường hợp này cho $A' = \sum_{i=1}^n Aw_i$.

Trong hai hệ quả sau đây, các giả thiết và ký hiệu là của Mệnh đề 18.

#### Hệ quả 1 {#ac-v-s1-lem-3-cor-1 .statement}

*Nếu $A$ là một vành Noether, $A$-môđun $A'$ là sinh hữu hạn và đặc biệt vành $A'$ là Noether.*

$A'$ là một môđun con của một $A$-môđun sinh hữu hạn.

#### Hệ quả 2 {#ac-v-s1-lem-3-cor-2 .statement}

*Nếu $A$ là một miền iđêan chính, $A'$ là một $A$-môđun tự do hạng $n$.* Khi đó, mọi môđun con của một $A$-môđun tự do đều tự do (*Algebra*, Chương VII, § 3, Định lý 1).

#### Hệ quả 3 {#ac-v-s1-lem-3-cor-3 .statement}

*Cho $E$ là một mở rộng bậc $n$ của trường $Q$ các số hữu tỉ. Nhóm cộng của bao đóng nguyên trong $E$ của vành $Z$ các số nguyên là một nhóm giao hoán tự do hạng $n$.*

$Z$ là đóng nguyên (no. 3, Mệnh đề 10) và $E$ là tách được vì $Q$ có đặc số 0. Do đó có thể áp dụng Hệ quả 2 cho trường hợp $A = Z$, $K = Q$ và $K' = E$.

*Nhận xét (2).* Các kết luận của Hệ quả 1 không nhất thiết đúng nếu không giả thiết $K'$ tách được trên $K$, ngay cả khi $K'$ là một trường mở rộng của $K$ (Bài tập 20). Mặt khác, nếu $A$ là một *đại số nguyên sinh hữu hạn trên $K_0$*, trong đó $K_0$ là một *trường*, thì bao đóng nguyên của $A$ trong *bất kỳ* mở rộng nào có bậc hữu hạn của trường phân thức của $A$ là một $A$-môđun sinh hữu hạn và một vành Noether, như ta sẽ thấy ở § 3, no. 2, Định lý 2.

### 7. MỞ RỘNG VÔ HƯỚNG TRONG MỘT ĐẠI SỐ ĐÓNG NGUYÊN

#### Mệnh đề 19 {#ac-v-s1-prop-19 .statement}

*Cho $k$ là một trường, $L$ là một mở rộng tách được của $k$ và $R$ là một $k$-đại số đóng nguyên. Nếu vành $L \otimes_k R$ là một miền nguyên, nó là đóng nguyên.*

Cho K là trường phân thức của R; vì k là một trường, L $\otimes_k$ R được đồng nhất một cách chính tắc với một k-đại số con của L $\otimes_k$ K và L và R với các k-đại số con của L $\otimes_k$ R. Hơn nữa, vì một phần tử s $\# 0$ của R không phải là ước của 0 trong R, nên 1 $\otimes s$ không phải là ước của 0 trong L $\otimes_k$ R vì L phẳng trên k (Chương I, § 2, no. 3); đồng nhất s với 1 $\otimes s$, do đó suy ra rằng, nếu S = R - {0}, L $\otimes_k$ K được đồng nhất với S$^{-1}$(L $\otimes_k$ K); vì giả thiết L $\otimes_k$ R là một miền nguyên, nên L $\otimes_k$ K vì thế được đồng nhất với một vành con của trường phân thức $\Omega$ của L $\otimes_k$ R.

(1) Giả sử L là một mở rộng hữu hạn của k; khi đó L $\otimes_k$ K là một đại số có hạng hữu hạn trên K và theo giả thiết không có ước của 0; do đó nó là một trường (Đại số, Chương V, § 2, no. 1, Mệnh đề 1) và vì thế trong trường hợp này nó chính là trường phân thức $\Omega$ của L $\otimes_k$ R. Cho ($w_1, \ldots, w_r$) là một cơ sở của L trên k, nên cũng là một cơ sở của L $\otimes_k$ K trên K. Tồn tại một cơ sở ($w_1^*, \ldots, w_n^*$) của L sao cho $\mathrm{Tr}_{L/k}(w_i w_j^*) = \delta_{ij}$ (no. 6, Bổ đề 3); mọi $z \in L \otimes_k K$ đều viết duy nhất $z = \sum_{i=1}^u a_i w_i$ trong đó $a_i \in K$; khi đó

$$
\mathrm{Tr}_{(L \otimes K)/K}(z w_j^*) = \sum_{i=1}^n a_i \mathrm{Tr}_{(L \otimes K)/K}(w_i w_j^*)
$$

và như trong L, các vết $\mathrm{Tr}_{(L \otimes K)/K}$ và $\mathrm{Tr}_{L/K}$ trùng nhau (Đại số, Chương VIII, § 12, no. 2, công thức (13)) suy ra cuối cùng $\mathrm{Tr}_{(L \otimes K)/K}(z w_j^*) = a_j$, với $1 \leq j \leq n$. Mặt khác, lưu ý rằng các phần tử của L là nguyên trên k và do đó cũng nguyên trên R (no. 1, Hệ quả 1 của Mệnh đề 2); vì thế (no. 1, Mệnh đề 5) L $\otimes_k$ R là nguyên trên R. Trong tình huống đó, giả sử rằng $z \in L \otimes_k K$ là nguyên trên L $\otimes_k$ R; khi đó z cũng nguyên trên R (no. 1, Mệnh đề 6), do đó $z w_j^*$ cũng vậy và vì thế $a_j = \mathrm{Tr}_{(L \otimes K)/K}(z w_j^*)$ cũng nguyên trên R với mọi $1 \leq j \leq n$ (no. 6, Hệ quả 2 của Mệnh đề 17). Vì R là đóng nguyên, $a_j \in R$ với mọi j và do đó $z \in L \otimes_k R$, điều này chứng minh mệnh đề trong trường hợp này.

(2) Bây giờ giả sử L là một mở rộng tách được sinh hữu hạn của K; khi đó tồn tại một cơ sở siêu việt tách được ($x_1, \ldots, x_d$) của L trên k (Đại số, Chương V, § 9, no. 3, Định lý 2); vì L và K rời nhau đại số trên k trong trường $\Omega$ (Đại số, Chương V, § 5, no. 4), nên các $x_i$ độc lập đại số trên K; do đó $R[x_1, \ldots, x_d]$ là đóng nguyên (no. 3, Hệ quả 2 của Mệnh đề 13). Cho T là tập hợp các phần tử $\neq 0$ của vành $A = k[x_1, \ldots, x_d] \subset L$, sao cho trường $k_1 = k(x_1, \ldots, x_d) \subset L$ bằng $T^{-1}k[x_1, \ldots, x_d]$; khi đó

$$
k_1 \otimes_k R = (T^{-1}A) \otimes_k R = T^{-1}A \otimes_A (A \otimes_k R) = T^{-1}(A \otimes_k R)
= T^{-1}R[x_1, \ldots, x_d]
$$

theo tính kết hợp của tích tenxơ, nên miền này là đóng nguyên (no. 5, Hệ quả 1 của Mệnh đề 16). Nhưng $L \otimes_k R$ được đồng nhất với

$$
L \otimes_{k_1} (k_1 \otimes_k R)
$$

và theo định nghĩa L là một mở rộng tách được hữu hạn của $k_1$; do đó suy ra từ (1) rằng $L \otimes_k R$ là đóng nguyên.

(3) *Trường hợp tổng quát.* Nếu $z$ là một phần tử của $\Omega$ nguyên trên $L \otimes_k R$, nó thỏa mãn một quan hệ có dạng $z^m + b_1 z^{m-1} + \ldots + b_m = 0$, trong đó các $b_i$ thuộc $L \otimes_k R$; khi đó tồn tại một mở rộng con sinh hữu hạn $L'$ của L trên $k$ sao cho các $b_i$ thuộc $L' \otimes_k R$ với $1 \leq i \leq m$ và $z$ thuộc $L' \otimes_k K$. Khi đó suy ra từ (2) rằng $z \in L' \otimes_k R$ và do đó $L \otimes_k R$ là đóng nguyên.

\* Cho V là một đa tạp đại số afin bất khả quy, $k$ là một trường định nghĩa của V và $R$ là vành các hàm chính quy trên V được xác định trên $k$; nếu R đóng nguyên, V được gọi là *chính quy trên $k$*; Mệnh đề 19 chỉ ra rằng, nếu V chính quy trên $k$, thì nó vẫn chính quy trên mọi mở rộng tách được L của $k$. \*

#### Hệ quả {#ac-v-s1-n7-cor-1 .statement}

*Cho k là một trường và R và S là hai đại số trên k đóng nguyên. Giả sử rằng vành $R \otimes_k S$ là một miền nguyên và các trường phân thức K và L của R và S tương ứng là tách được trên k. Khi đó vành $R \otimes_k S$ là một miền đóng nguyên.*

Vì R và S được đồng nhất với các đại số con của $R \otimes_k S$, K và L được đồng nhất với các trường con của trường phân thức $\Omega$ của $R \otimes_k S$ là rời nhau tuyến tính trên $k$ (*Algebra*, Chương V, § 2, no. 3, Mệnh đề 5). Khi đó suy ra từ Mệnh đề 19 rằng $R \otimes_k L$ và $K \otimes_k S$ là các miền đóng nguyên; vì giao của chúng là $R \otimes_k S$ (Chương I, § 2, no. 6, Mệnh đề 7), nên $R \otimes_k S$ là một miền đóng nguyên (no. 2, Hệ quả của Mệnh đề 8).

\* Cho hai đa tạp afin bất khả quy V, W xác định trên $k$, tích của chúng $V \times W$ là một đa tạp afin và vành các hàm chính quy trên $V \times W$ được đồng nhất với tích tenxơ trên $k$ của vành các hàm chính quy trên V và vành các hàm chính quy trên W. Hệ quả của Mệnh đề 19 chỉ ra rằng, nếu V và W chính quy trên $k$, thì $V \times W$ chính quy trên $k$. \*

### 8. CÁC PHẦN TỬ NGUYÊN TRÊN MỘT VÀNH PHÂN BẬC

*Mọi phép phân bậc được xét trong no. này đều thuộc kiểu $\mathbf{Z}$; nếu A là một vành phân bậc và $i \in \mathbf{Z}$, $A_i$ ký hiệu tập hợp các phần tử thuần nhất có bậc $i$ của vành A.*

Cho A là một vành phân bậc và B là một đại số phân bậc trên A. Cho x là một phần tử *thuần nhất* của B nguyên trên A ; khi đó tồn tại một quan hệ

$$
x^n + a_1 x^{n-1} + \ldots + a_n = 0 \quad \text{với } a_i \in A \quad \text{với } 1 \leq i \leq n.
$$

Đặt $m = \deg(x)$ và cho $a'_i$ là thành phần thuần nhất có bậc $mi$ của $a_i$ ($1 \leq i \leq n$); khi đó hiển nhiên

$$
x^n + a'_1 x^{n-1} + \ldots + a'_n = 0
$$

nói cách khác x thỏa mãn một phương trình phụ thuộc nguyên với các hệ số *thuần nhất*.

Cho $\mathbf{A}[X, X^{-1}]$ là vành phân thức $S^{-1}\mathbf{A}[X]$ của vành đa thức $\mathbf{A}[X]$ theo một bất định, $S$ là tập con nhân của $\mathbf{A}[X]$ gồm các lũy thừa $X^n$ của $X$ ($n \geq 0$); vì $X$ không là ước của 0 trong $\mathbf{A}[X]$ nên ngay lập tức suy ra rằng các $X^i$ ($i \in \mathbf{Z}$) tạo thành một cơ sở trên $\mathbf{A}$ của $\mathbf{A}$-môđun $\mathbf{A}[X, X^{-1}]$. Với mọi phần tử $a \in \mathbf{A}$ có các thành phần thuần nhất $a_i$ ($i \in \mathbf{Z}$), ta viết

$$
j_{\mathbf{A}}(a) = \sum_{i \in \mathbf{Z}} a_i X^i \in \mathbf{A}[X, X^{-1}]
$$

ngay lập tức suy ra rằng $j_{\mathbf{A}} : \mathbf{A} \to \mathbf{A}[X, X^{-1}]$ là một đồng cấu vành đơn ánh.

#### Mệnh đề 20 {#ac-v-s1-prop-20 .statement}

*Cho $\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} A_i$, là một vành phân bậc và $\mathbf{B}$ là một đại số con (giao hoán) phân bậc của $\mathbf{A}$. Tập hợp $\mathbf{A}'$ các phần tử của $\mathbf{B}$ nguyên trên $\mathbf{A}$ là một đại số con phân bậc của $\mathbf{B}$.

Nếu $A_i = 0$ với $i < 0$ và $\mathbf{B}$ là một vành thu gọn, thì $A'_i = 0$ với $i < 0$.*

Biểu đồ

$$
\begin{array}{ccc}
\mathbf{B} & & \mathbf{A} \\
& \rho & \\
& & \\
& & \\
\mathbf{A}[X, X^{-1}] \xrightarrow{\phi'} \mathbf{B}[X, X^{-1}] \\
\end{array}
$$

(trong đó $\rho$ là đồng cấu xác định cấu trúc $\mathbf{A}$-đại số trên $\mathbf{B}$ và $\rho'$ là đồng cấu một cách chính tắc dẫn xuất từ nó) là giao hoán, như được kiểm tra ngay lập tức từ định nghĩa (5). Cho $x$ là một phần tử của $\mathbf{B}$ nguyên trên $\mathbf{A}$; khi đó $j_{\mathbf{B}}(x)$ là nguyên trên $\mathbf{A}[X, X^{-1}]$ (no. 1, Mệnh đề 2) và do đó suy ra từ no. 5, Mệnh đề 16 rằng tồn tại một số nguyên $m > 0$ sao cho $X^m j_{\mathbf{B}}(x)$ là một phần tử của $\mathbf{B}[X]$ nguyên trên $\mathbf{A}[X]$. Khi đó ta suy ra từ no. 3, Mệnh đề 12 rằng các hệ số của đa thức $X^m j_{\mathbf{B}}(x)$ là nguyên trên $\mathbf{A}$; vì các hệ số này theo định nghĩa là các thành phần thuần nhất của $x$, ta thấy rằng chúng là nguyên trên $\mathbf{A}$, điều này chứng minh rằng $\mathbf{A}'$ là một đại số con phân bậc của $\mathbf{B}$.

Giả sử bây giờ $x \in A'_i$ với $i < 0$; nhận xét ở đầu mục này cho thấy rằng $x$ thỏa mãn một phương trình có dạng (4) trong đó $a_k' \in A_{kt}$ với $1 \leq k \leq n$. Nếu $A_j = 0$ với $j < 0$, thì $x^n = 0$ và nếu $\mathbf{B}$ là một vành giảm thì ta suy ra rằng $x = 0$ và do đó $A'_i = 0$ với mọi $i < 0$ trong trường hợp này.

Nhắc lại (Chương II, § 2, no. 9) rằng, nếu $\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$ là một vành phân bậc và $S$ là một tập con nhân của $\mathbf{A}$ gồm các phần tử *thuần nhất*, thì một cấu trúc vành phân bậc được xác định trên $S^{-1}\mathbf{A}$ bằng cách lấy tập $(S^{-1}\mathbf{A})_i$ các phần tử thuần nhất bậc $i$ làm tập các phần tử có dạng $a/s$, trong đó $a \in \mathbf{A}$ và $s \in S$ là thuần nhất và sao cho $\deg(a) - \deg(s) = i$

#### Bổ đề 4 {#ac-v-s1-lem-4 .statement}

Cho $\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$ là một miền nguyên phân bậc và $S$ là tập các phần tử thuần nhất khác $0$ của $\mathbf{A}$.

(i) Mọi phần tử thuần nhất khác $0$ của $S^{-1}\mathbf{A}$ đều khả nghịch, và vành $K_0 = (S^{-1}\mathbf{A})_0$ là một trường và tập các $i \in \mathbf{Z}$ sao cho $(S^{-1}\mathbf{A})_i \neq 0$ là một nhóm con $q\mathbf{Z}$ của $\mathbf{Z}$ (với $q \geqslant 0$).

(ii) Giả sử $q \geqslant 1$ và lấy $t$ là một phần tử khác $0$ của $(S^{-1}\mathbf{A})_q$. Khi đó đồng cấu trên $K_0$ $f$ của vành đa thức $K_0[X]$ vào $S^{-1}\mathbf{A}$, gửi $X$ tới $t$, kéo dài thành một đẳng cấu của $K_0[X, X^{-1}]$ lên $S^{-1}\mathbf{A}$ và $S^{-1}\mathbf{A}$ là một vành đóng nguyên.

Các mệnh đề trong (i) suy ra ngay lập tức từ các định nghĩa và giả thiết rằng $\mathbf{A}$ là một miền nguyên, vì nếu $a/s$ và $a'/s'$ là hai phần tử thuần nhất $\neq 0$ của $S^{-1}\mathbf{A}$ có bậc $i$ và $i'$, thì $aa'/ss'$ là một phần tử thuần nhất $\neq 0$ và có bậc $i + i'$. Để chứng minh (ii), ta nhận thấy rằng vì $t$ khả nghịch trong $S^{-1}\mathbf{A}$ nên đồng cấu $f$ kéo dài một cách duy nhất thành một đồng cấu $\tilde{f}: K_0[X, X^{-1}] \to S^{-1}\mathbf{A}$ và tất yếu $\tilde{f}(X^{-1}) = t^{-1}$. Mặt khác, theo định nghĩa của $q$, mọi phần tử thuần nhất $\neq 0$ của $S^{-1}\mathbf{A}$ đều có bậc $qn \ (n \in \mathbf{Z})$ và do đó có thể viết duy nhất dưới dạng $\lambda t^n$ với $\lambda \in K_0$ (vì $S^{-1}\mathbf{A}$ là một miền nguyên); suy ra $\tilde{f}$ là song ánh. Cuối cùng, ta biết rằng $K_0[X]$ đóng nguyên (no. 3, Mệnh đề 10) và do đó $K_0[X, X^{-1}]$ cũng vậy (no. 5, Hệ quả 1 của Mệnh đề 16), điều này hoàn tất chứng minh của Bổ đề.

#### Mệnh đề 21 {#ac-v-s1-prop-21 .statement}

Cho $\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$ là một miền nguyên phân bậc và $S$ là tập hợp các phần tử thuần nhất $\neq 0$ của $\mathbf{A}$. Khi đó bao đóng nguyên $\mathbf{A}'$ của $\mathbf{A}$ là một vành con phân bậc của $S^{-1}\mathbf{A}$. Nếu thêm nữa $\mathbf{A}_i = 0$ với $i < 0$, thì $\mathbf{A}'_i = 0$ với $i < 0$.

Nếu $\mathbf{A} = \mathbf{A}_0$, thì mệnh đề là tầm thường. Ngược lại ta có thể áp dụng Bổ đề 4; vành $S^{-1}\mathbf{A}$ là một miền đóng nguyên và do đó $\mathbf{A} \subset S^{-1}\mathbf{A}$; vì $S^{-1}\mathbf{A}$ là phân bậc, nên $\mathbf{A}'$ cũng phân bậc theo Mệnh đề 20; mệnh đề sau cũng suy ra từ Mệnh đề 20.

#### Hệ quả 1 {#ac-v-s1-prop-21-cor-1 .statement}

Với các giả thiết và ký hiệu của Mệnh đề 21, nếu mọi phần tử thuần nhất của $S^{-1}\mathbf{A}$ nguyên trên $\mathbf{A}$ đều thuộc $\mathbf{A}$, thì $\mathbf{A}$ là đóng nguyên.

Khi đó $\mathbf{A}'_i \subset \mathbf{A}$ với mọi $i \in \mathbf{Z}$ và suy ra $\mathbf{A}' = \mathbf{A}$.

#### Hệ quả 2 {#ac-v-s1-prop-21-cor-2 .statement}

Nếu $\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$ là một miền phân bậc đóng nguyên, thì miền $\mathbf{A}_0$ đóng nguyên.

Trường phân thức $K_0$ của $\mathbf{A}$ được đồng nhất (theo ký hiệu của Mệnh đề 21) với một vành con của vành các phần tử thuần nhất bậc 0 của $S^{-1}A$; do đó mọi phần tử của $K_0$ nguyên trên $A$ (và *a fortiori* trên $A$) theo giả thiết đều thuộc $A$.

#### Hệ quả 3 {#ac-v-s1-prop-21-cor-3 .statement}

*Cho $A = \bigoplus_{i \in \mathbf{Z}} A_i$ là một miền nguyên phân bậc đóng nguyên. Khi đó, với mọi số nguyên $d > 0$, vành $A^{(d)}$ (Chương III, § 1, no. 3) là một miền nguyên đóng nguyên.*

Cho $U$ là tập hợp các phần tử thuần nhất $\neq 0$ của $A^{(d)}$ và cho $x$ là một phần tử thuần nhất của $U^{-1}A^{(d)}$ nguyên trên $A^{(d)}$ và do đó trên $A$; vì $x \in S^{-1}A$, nên $x$ thuộc $A$ theo giả thiết; vì bậc của nó chia hết cho $d$, nó thuộc $A^{(d)}$ và khi đó suy ra từ Hệ quả 1 rằng $A^{(d)}$ là đóng nguyên.

### 9. ỨNG DỤNG: BẤT BIẾN CỦA MỘT NHÓM TỰ ĐẲNG CẤU CỦA MỘT ĐẠI SỐ

Cho một vành $K$, một $K$-đại số $A$ và một nhóm $G$, ta sẽ nói rằng $G$ tác động lên $A$ nếu: (1) tập hợp $A$ có nhóm toán tử $G$ (*Đại số*, Chương I, § 7, no. 2); (2) với mọi $\sigma \in G$, ánh xạ $x \mapsto \sigma.x$ là một *tự đồng cấu* của $K$-đại số $A$ (và do đó là một *tự đẳng cấu* vì nó là song ánh (*loc. cit.*)). Ta ký hiệu $A^G$ là tập hợp các phần tử của $A$ là *bất biến* dưới $G$; rõ ràng nó là một *đại số con trên K* của $A$.

Ta sẽ nói rằng $G$ là một nhóm toán tử *hữu hạn địa phương* trên $A$ nếu mọi *quỹ đạo* của $G$ trong $A$ (*Đại số*, Chương I, Sửa chữa *Fascicule* IV) đều *hữu hạn*.

#### Mệnh đề 22 {#ac-v-s1-prop-22 .statement}

*Cho $A$ là một $K$-đại số (giao hoán) và $G$ là một nhóm toán tử hữu hạn địa phương trên $A$. Khi đó $A$ là nguyên trên đại số con $A^G$.*

Với mọi $x \in A$, cho $x_i$ ($1 \leq i \leq n$) là các phần tử phân biệt của quỹ đạo của $x$ dưới tác động của $G$; với mọi $\sigma \in G$, tồn tại một phép hoán vị $\pi_\sigma$ của tập hợp $\{1, 2, \ldots, n\}$ sao cho $\sigma.x_i = x_{\pi_\sigma(i)}$ với $1 \leq i \leq n$; do đó các hàm đối xứng sơ cấp của các $x_i$ là những phần tử của $A$ bất biến dưới $G$, nói cách khác là những phần tử của $A^G$. Vì $x$ là một nghiệm của đa thức đơn khởi $\prod_{i=1}^n (X - x_i)$ và các hệ số của đa thức này thuộc $A^G$, nên $x$ là nguyên trên $A^G$.

#### Định lý 2 {#ac-v-s1-thm-2 .statement}

*Cho $A$ là một đại số trên $K$ sinh hữu hạn và $G$ là một nhóm hữu hạn địa phương các phép tác động trên $A$. Khi đó $A$ là một A-môđun sinh hữu hạn; nếu thêm $K$ là Noether, $A^G$ là một đại số trên $K$ sinh hữu hạn.*

Gọi $(a_j)_{1 \leq j \leq m}$ là một hệ sinh của đại số trên $K$ $A$; do *a fortiori* $A = A^G[a_1, \ldots, a_l]$ và các $a_j$ là nguyên trên $A^G$ theo Mệnh đề 22, mệnh đề thứ nhất suy ra từ no. 1, Mệnh đề 4. Mệnh đề thứ hai là hệ quả của bổ đề sau:

#### Bổ đề 5 {#ac-v-s1-lem-5 .statement}

*Cho $K$ là một vành Noether, $B$ là một đại số trên $K$ sinh hữu hạn và $C$ là một đại số con trên $K$ của B sao cho B nguyên trên C. Khi đó C là một đại số trên A sinh hữu hạn.*

Cho $(x_i)_{1 \leq i \leq n}$ là một hệ sinh hữu hạn của đại số trên $K$ B. Với mọi i, theo giả thiết tồn tại một đa thức đơn khởi $P_i \in C[X]$ sao cho $P_i(x_i) = 0$. Gọi C' là đại số con trên K của C sinh bởi các hệ số của các $P_i$ ($1 \leq i \leq n$); hiển nhiên các $x_i$ là nguyên trên C' và $B = C'[x_1, \ldots, x_n]$; do đó B là một môđun $C'$ sinh hữu hạn (no. 1, Mệnh đề 4). Mặt khác $C'$ là một vành Noether (Chương III, § 2, no. 10, Hệ quả 3 của Định lý 2); do đó C là một môđun $C'$ sinh hữu hạn, điều này chứng minh rằng C là một đại số trên K sinh hữu hạn.

#### Nhận xét {#ac-v-s1-n9-rem-1 .statement}

Tập các $\sigma \in G$ sao cho $\sigma a_j = a_j$ với $1 \leq j \leq m$ hiển nhiên giữ bất biến mọi phần tử của A. Nhóm con chuẩn tắc $\mathcal{H}$ của $G$ giữ bất biến mọi phần tử của A do đó có chỉ số hữu hạn trong $G$ và có thể xem A như có một nhóm hữu hạn các phép tác động $G/\mathcal{H}$; hiển nhiên $A^{G/\mathcal{H}} = A^G$.

Cho S là một tập con nhân của một vành A và G là một nhóm tác động lên A và sao cho S ổn định; khi đó, với mọi $\sigma \in G$, tồn tại duy nhất một tự đồng cấu $z \mapsto q_z$ của vành $S^{-1}A$ sao cho $q_z(a/1) = (a.a)/1$ với mọi $a \in A$; nó được cho bởi công thức $\sigma.(a/s) = (\sigma.a)/(\sigma.s)$ với $a \in A$ và $s \in S$ (Chương II, § 2, no. 1, Hệ quả 2 của Mệnh đề 2); nếu $\tau$ là một phần tử khác của G, rõ ràng $q_z(\tau.z) = (\sigma\tau).z$ với mọi $z \in S^{-1}A$ và do đó nhóm G tác động lên vành $S^{-1}A$.

#### Mệnh đề 23 {#ac-v-s1-prop-23 .statement}

Cho A là một đại số trên K, $G$ là một nhóm hữu hạn địa phương các phép tác động trên A, S là một tập con nhân của A ổn định dưới $G$ và $S^G$ là tập $S \cap A''$. Khi đó ánh xạ chính tắc từ $(S^G)^{-1}A$ đến $S^{-1}A$ (Chương II, § 2, no. 1, Hệ quả 2 của Mệnh đề 2) là một đẳng cấu đưa $(S^G)^{-1}A^G$ tới $(S^{-1}A)^G$.

Với mọi $s \in S$, cho $s, s_1, \ldots, s_q$ là các phần tử phân biệt của quỹ đạo của s dưới tác động của $G$; vì $ss_1 \ldots s_q \in S^G$, mệnh đề đầu tiên suy ra từ Chương 11, § 2, no. 3, Mệnh đề 8. Đồng nhất một cách chính tắc $(S^G)^{-1}A$ với $S^{-1}A$, rõ ràng mọi phần tử của $(S^G)^{-1}A^G$ đều bất biến dưới $G$. Ngược lại, cho $a/t$ là một phần tử của $(S^G)^{-1}A$ bất biến dưới $G$ ($a \in A, t \in S^G$); nếu $a, (1 \leq j \leq m)$ là các phần tử phân biệt của quỹ đạo của $a$ dưới tác động của $G$, thì $a_j/t = a/t$ với $1 \leq j \leq m$ và do đó tồn tại $s \in S^G$ sao cho $s(a_j - a) = 0$ với $1 \leq j \leq m$; nói cách khác, sa là bất biến dưới $G$ và, vì $a/t = (sa)/(st)$, chắc chắn $a/t \in (S^G)^{-1}A^G$.

#### Hệ quả {#ac-v-s1-n9-cor-1 .statement}

Cho A là một miền nguyên, K là trường các phân thức của nó và $G$ là một nhóm hữu hạn địa phương các toán tử trên A. Khi đó $G$ tác động trên K và $K^G$ là trường các phân thức của $A^G$.

A $- \{0\}$ là ổn định dưới $G$.

### Bài tập {#ac-v-s1-exercises}

Xem các [bài tập cho § 1](exercises/s1/).
