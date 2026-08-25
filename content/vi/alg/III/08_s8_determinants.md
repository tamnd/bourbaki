---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 8
section_title: Determinants
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0546-0565, 0661-0668
extraction: ocr
subsections:
    - "no": 1
      title: DETERMINANTS OF AN ENDOMORPHISM
      page: 0
      pdf_page: 546
    - "no": 2
      title: CHARACTERIZATION OF AUTOMORPHISMS OF A FINITE-DIMENSIONAL FREE MODULE
      page: 0
      pdf_page: 547
    - "no": 3
      title: DETERMINANT OF A SQUARE MATRIX
      page: 0
      pdf_page: 548
    - "no": 4
      title: CALCULATION OF A DETERMINANT
      page: 0
      pdf_page: 550
    - "no": 5
      title: MINORS OF A MATRIX
      page: 0
      pdf_page: 552
    - "no": 6
      title: EXPANSIONS OF A DETERMINANT
      page: 0
      pdf_page: 554
    - "no": 7
      title: APPLICATION TO LINEAR EQUATIONS
      page: 0
      pdf_page: 558
    - "no": 8
      title: CASE OF A COMMUTATIVE FIELD
      page: 0
      pdf_page: 560
    - "no": 9
      title: THE UNIMODULAR GROUP $ \mathbf{SL}(n, A) $
      page: 0
      pdf_page: 561
    - "no": 10
      title: THE $ \mathbf{A}[X] $-MODULE ASSOCIATED WITH AN $ \mathbf{A} $-MODULE ENDOMORPHISM
      page: 0
      pdf_page: 562
    - "no": 11
      title: CHARACTERISTIC POLYNOMIAL OF AN ENDOMORPHISM
      page: 0
      pdf_page: 564
statements: 36
exercises: 26
content_sha256: 1f6a924bd22499a1851beb85d87cb4f5eae092e20dbd3180164b45bb2af971cd
translated_from: content/en/alg/III/08_s8_determinants.md
source_content_sha256: 61460bcdd2ad78ff72f6c630c7a5c2c7dff603a886863a3d32aebd73ea99c369
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-ea440f38
glossary_version: 34
glossary_terms_sha256: 24200b5d2f70600cc6f090f9191189d180b29f70ebe11c661fb120f34b59de35
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. ĐỊNH THỨC

### 1. ĐỊNH THỨC CỦA MỘT TỰ ĐỒNG CẤU

Cho $ M $ là một $ A $-môđun với một cơ sở hữu hạn gồm $ n $ phần tử và $ u $ là một tự đồng cấu của $ M $. $ A $-môđun $ \bigwedge^n(M) $ là một môđun tự do đơn sinh, tức là đẳng cấu với $ A $ (no. 8, Hệ quả 1 của Định lý 1); $ \bigwedge^n(u) $ là một tự đồng cấu của môđun này và do đó là một phép vị tự $ z \mapsto \lambda z $ với tỉ số $ \lambda \in A $ được xác định duy nhất (II, § 2, no. 3, Mệnh đề 5).

#### Định nghĩa 1 {#alg-iii-s8-def-1 .statement}

*Định thức của một tự đồng cấu $ u $ của một $ A $-môđun tự do $ M $ có số chiều hữu hạn $ n $* (II, § 7, no. 2, Hệ quả của Mệnh đề 3 và Nhận xét 1), *được ký hiệu bởi* $ \det u $, *là vô hướng $ \lambda $ sao cho* $ \bigwedge^n(u) $ *là phép vị tự có tỉ số* $ \lambda $.

Theo công thức (4) của § 7, no. 2, $ \det u $ là vô hướng duy nhất sao cho

(1)
$$
u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n) = (\det u) \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$
với mọi dãy $ (x_i)_{1 \leq i \leq n} $ gồm $ n $ phần tử của $ M $. Nếu $ \det(u) = 1 $, $ u $ được gọi là *đơn môđula*.

#### Mệnh đề 1 {#alg-iii-s8-prop-1 .statement}

(i) *Nếu $ u $ và $ v $ là hai tự đồng cấu của một $ A $-môđun tự do $ M $ có số chiều hữu hạn, thì*

(2)
$$
\det(u \circ v) = (\det u)(\det v).
$$

(ii) $ \det(1_M) = 1 $; *với mọi tự đẳng cấu* $ u $ *của* $ M $, $ \det u $ *là khả nghịch trong* $ A $ *và*

(3)
$$
\det(u^{-1}) = (\det u)^{-1}.
$$

Nếu $ n $ là chiều của $ M $, điều này suy ra ngay lập tức từ quan hệ $ \bigwedge^n(u \circ v) = (\bigwedge^n(u)) \circ (\bigwedge^n(v)) $ § 7, no. 2, công thức (3)).

Cho $ M $ là một $ A $-môđun tự do với một cơ sở hữu hạn $ (e_i)_{1 \leq i \leq n} $; cho một dãy $ (x_i)_{1 \leq i \leq n} $ gồm $ n $ phần tử của $ M $, định thức của dãy này *đối với* cơ sở đã cho $(e_i)$, được ký hiệu bởi $\det(x_1, x_2, \ldots, x_n)$ khi không thể có sự nhầm lẫn về cơ sở, là định thức của tự đồng cấu $u$ của $M$ sao cho $u(e_i) = x_i$ với $1 \leq i \leq n$. Khi đó theo công thức (1)

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = \det(x_1, x_2, \ldots, x_n) \ e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$

và quan hệ này đặc trưng hóa ánh xạ $(x_i) \mapsto \det(x_1, x_2, \ldots, x_n)$ của $M^n$ vào $A$. Nó chỉ ra rằng ánh xạ này là một *dạng tuyến tính n phản xứng*. Vì, theo § 7, no. 4, Mệnh đề 7, $A$-môđun các dạng tuyến tính $n$ phản xứng đẳng cấu chính tắc với đối ngẫu của $\bigwedge^n(M)$ và $\bigwedge^n(M)$ đẳng cấu với $A$, nên thấy rằng *mọi dạng tuyến tính n phản xứng trên $M^n$ đều có thể được viết*

$$(x_1, \ldots, x_n) \mapsto \alpha \det(x_1, x_2, \ldots, x_n)$$

với một $\alpha \in A$ nào đó.

#### Mệnh đề 2 {#alg-iii-s8-prop-2 .statement}

*Cho $M$ là một $A$-môđun tự do với một cơ sở hữu hạn $(e_i)_{1 \leq i \leq n}$ và $v$ là một tự đồng cấu của $M$. Với mọi dãy $(x_i)_{1 \leq i \leq n}$ gồm $n$ phần tử của $M$,*

$$
\det(v(x_1), \ldots, v(x_n)) = (\det v) \det(x_1, \ldots, x_n).
$$

Nếu $u$ là tự đồng cấu của $M$ sao cho $u(e_i) = x_i$ với mọi $i$, thì

$$
v(x_i) = (v \circ u)(e_i)
$$

và (5) do đó suy ra từ (2).

### 2. ĐẶC TRƯNG HÓA CÁC TỰ ĐẲNG CẤU CỦA MỘT MÔĐUN TỰ DO HỮU HẠN CHIỀU

#### Định lý 1 {#alg-iii-s8-thm-1 .statement}

*Cho $M$ là một $A$-môđun tự do hữu hạn chiều và $u$ là một tự đồng cấu của $M$. Các điều kiện sau là tương đương:*
(a) $u$ là song ánh;
(b) $u$ là khả nghịch phải (II, § 1, no. 9, Hệ quả 1 đối với Mệnh đề 15);
(c) $u$ là khả nghịch trái (II, § 1, no. 9, Hệ quả 2 đối với Mệnh đề 15);
(d) $u$ là toàn ánh;
(e) $\det u$ khả nghịch trong $A$.

Cho $(e_i)_{1 \leq i \leq n}$ là một cơ sở của $M$. Nếu $x_i = u(e_i)$ với $1 \leq i \leq n$, thì

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det u) e_1 \wedge e_2 \wedge \cdots \wedge e_n.
$$

Theo § 7, no. 9, Định lý 2, một điều kiện cần và đủ để các $x_i$ lập thành một cơ sở của $M$ là $\det u$ là một phần tử khả nghịch của $A$; điều này chứng minh sự tương đương của (a) và (e). Nhận xét rằng (a) hiển nhiên kéo theo mỗi điều kiện (b), (c) và (d); còn lại cần chứng minh rằng mỗi điều kiện (b), (c) và (d) kéo theo (e). Bây giờ, nếu tồn tại một tự đồng cấu $v$ của $M$ sao cho $v \circ u = 1_M$ hoặc $u \circ v = 1_M$, thì $(\det v)(\det u) = 1$ và do đó $\det u$ khả nghịch trong $A$. Nếu $u$ là toàn ánh, thì $\bigwedge^n(u)$ cũng là toàn ánh (§ 7, no. 2, Mệnh đề 3), nói cách khác phép vị tự có tỉ số det $ u $ trong $ A $ là toàn ánh, điều này ngay lập tức kéo theo rằng det $ u $ là khả nghịch.

#### Mệnh đề 3 {#alg-iii-s8-prop-3 .statement}

*Cho $ M $ là một $ A $-môđun tự do hữu hạn chiều. Đối với mọi tự đồng cấu $ u $ của $ M $, các điều kiện sau là tương đương:*
  (f) $ u $ là đơn ánh;
  (g) det $ u $ không là một ước của không trong $ A $.

Với cùng ký hiệu như trong chứng minh của Định lý 1, để $ u $ là đơn ánh, điều kiện cần và đủ là các $ x_i $ độc lập tuyến tính. Theo § 7, no. 9, Mệnh đề 12, điều kiện cần và đủ cho điều này là quan hệ $ \lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0 $ (với $ \lambda \in A $) kéo theo $ \lambda = 0 $. Nhưng điều này tương đương với $ \lambda (\det u) = 0 $ vì $ e_1 \wedge \cdots \wedge e_n $ là một cơ sở của $ \Lambda^n(M) $; do đó mệnh đề.

#### Nhận xét {#alg-iii-s8-n2-rem-1 .statement}

Khi $ A $ là một trường, điều kiện (e) của Định lý 2 tương đương với điều kiện (g) của Mệnh đề 3, vì cả hai đều có nghĩa là $ \det u \neq 0 $. Do đó trong trường hợp này tất cả các điều kiện của Định lý 1 và Mệnh đề 3 là tương đương (xem II, § 7, no. 4, Hệ quả của Mệnh đề 9).

### 3. ĐỊNH THỨC CỦA MỘT MA TRẬN BÌNH PHƯƠNG

#### Định nghĩa 2 {#alg-iii-s8-def-2 .statement}

*Cho $ I $ là một tập hợp hữu hạn, $ A $ là một vành giao hoán và $ X $ là một ma trận bình phương kiểu $ (I, I) $ trên vành $ A $ (II, § 10, no. 7). Định thức của tự đồng cấu $ u $ của $ A $-môđun $ A^I $, mà ma trận của nó đối với cơ sở chính tắc của $ A^I $ là $ X $, được gọi là định thức của $ X $ và được ký hiệu là $ \det X $.*

Nếu $ X = (\xi_{ij})_{(i,j) \in I \times I} $ và $ (e_i)_{i \in I} $ là cơ sở chính tắc của $ A^I $, thì tự đồng cấu $ u $ được cho bởi
$$
u(e_i) = \sum_{j \in J} \xi_{ji} e_j.
$$

Khi $ I = \{1, n\} \subset \mathbf{N} $, nếu ta viết $ x_i = u(e_i) $ với $ i \in I $, thì định thức của $ X $ được xác định trong quan hệ
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det X) e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$
nói cách khác, $ \det X $ bằng định thức $ \det(x_1, x_2, \ldots, x_n) $ đối với cơ sở chính tắc của $ A^n $. Do đó:

#### Mệnh đề 4 {#alg-iii-s8-prop-4 .statement}

*Đối với $ n $ vectơ $ x_1, \ldots, x_n $ của $ A^n $, gọi $ X(x_1, \ldots, x_n) $ là ma trận bình phương cấp $ n $ mà cột thứ $ i $ của nó là $ x_i $ với $ 1 \leq i \leq n $. Khi đó ánh xạ*
$$
(x_1, \ldots, x_n) \mapsto \det(X(x_1, \ldots, x_n))
$$
*trên $ (A^n)^n $ vào $ A $ là phản xứng và $ n $-tuyến tính.*

Đặc biệt, định thức của một ma trận mà hai cột của nó bằng nhau là không. Nếu một phép hoán vị được thực hiện trên các cột của một ma trận, định thức của ma trận mới bằng định thức của ma trận cũ nhân với $ \varepsilon_{\sigma} $. Nếu thêm vào một cột của một ma trận một bội vô hướng của một cột có chỉ số khác, định thức của ma trận mới bằng định thức của ma trận cũ.

Tổng quát hơn, cho $ M $ là một $ A $-môđun tự do có số chiều hữu hạn $ n $ và cho $ (e_i)_{i \in I} $ là một cơ sở của $ M $; với mọi tự đẳng cấu $ u $ của $ M $, nếu $ X $ là ma trận của $ u $ theo cơ sở $ (e_i) $, thì

$$
\det(u) = \det(X)
$$

như suy ra ngay từ các định nghĩa.

Khi $ I = \{1, n\} $, định thức của $ X $ cũng được ký hiệu bởi

$$
\det(\xi_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}
$$

hoặc đơn giản là $ \det(\xi_{ij}) $ nếu điều đó không gây nhầm lẫn, hoặc cũng

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} & \ldots & \xi_{1n} \\
\xi_{21} & \xi_{22} & \ldots & \xi_{2n} \\
\ldots & \ldots & \ldots & \ldots \\
\xi_{n1} & \xi_{n2} & \ldots & \xi_{nn}
\end{vmatrix}
$$

Khi $ X = 1 $, ma trận $ X $ được gọi là đơn môđula.

#### Ví dụ {#alg-iii-s8-n3-exa-1 .statement}

(1) Định thức của ma trận rỗng bằng 1; định thức của một ma trận vuông cấp 1 bằng phần tử duy nhất của ma trận này. Đối với một ma trận cấp 2

$$
\begin{pmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{pmatrix}
$$

thì, theo ký hiệu trên,

$$
x_1 \wedge x_2 = (\xi_{11} e_1 + \xi_{21} e_2) \wedge (\xi_{12} e_1 + \xi_{22} e_2) = \xi_{11} \xi_{22} e_1' \wedge e_2 + \xi_{21} \xi_{12} e_2 \wedge e_1
$$

do đó

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{vmatrix} = \xi_{11} \xi_{22} - \xi_{12} \xi_{21}.
$$

Ta chuyển sang ngôn ngữ của ma trận một số kết quả của các no. 1 và 2:

#### Mệnh đề 5 {#alg-iii-s8-prop-5 .statement}

*Nếu $ X $ và $ Y $ là hai ma trận vuông trên một vành giao hoán $ A $ với cùng một tập chỉ số hữu hạn, thì*

$$
\det(XY) = (\det X)(\det Y).
$$

Để X khả nghịch, điều kiện cần và đủ là det X là một phần tử khả nghịch của A, và khi đó

(9) $$
\det(X^{-1}) = (\det X)^{-1}.
$$

Điều này suy ra ngay từ số 1, Mệnh đề 1 và no. 2, Định lý 1.

#### Hệ quả {#alg-iii-s8-n3-cor-1 .statement}

*Hai ma trận vuông đồng dạng có các định thức bằng nhau.*

Nếu P là một ma trận vuông khả nghịch, thì $ \det(PXP^{-1}) = \det X $ theo (8) và (9).

#### Mệnh đề 6 {#alg-iii-s8-prop-6 .statement}

*Để các cột của một ma trận vuông X có cấp hữu hạn độc lập tuyến tính, điều kiện cần và đủ là det X không là một ước của không trong A.*

Điều này suy ra từ no. 2, Mệnh đề 3.

### 4. TÍNH ĐỊNH THỨC

#### Bổ đề 1 {#alg-iii-s8-lem-1 .statement}

*Cho A là một vành giao hoán và M là một A-môđun tự do với một cơ sở $(e_j)_{j \in J}$, trong đó tập chỉ số J được sắp thứ tự toàn phần. Với mọi số nguyên $p \leq \mathrm{Card}(J)$, mọi hàm p-tuyến tính phản xứng $f : M^p \to N$ (trong đó N là một A-môđun) và mọi họ gồm p phần tử $x_i = \sum_{j \in J} \xi_{ji} e_j$ của M $(1 \leq i \leq p)$,

$$
f(x_1, x_2, \ldots, x_p)
= \sum_{j_1 < j_2 < \cdots < j_p} \left( \sum_{\sigma \in S_p} \varepsilon_\sigma \cdot \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(p)}, p} \right) f(e_{j_1}, \ldots, e_{j_p})
$$

*trong đó* $(j_k)_{1 \leq k \leq p}$ *chạy qua tập các dãy tăng ngặt gồm p phần tử của J.*

Bây giờ

$$
f(x_1, \ldots, x_p) = \sum_{(j_k)} \xi_{j_1, 1} \xi_{j_2, 2} \cdots \xi_{j_p, p} f(e_{j_1}, e_{j_2}, \ldots, e_{j_p})
$$

trong đó $(j_k)_{1 \leq k \leq p}$ chạy qua *tất cả* các dãy gồm p phần tử của J; khi đó chỉ cần áp dụng Hệ quả 1 cho Mệnh đề 7 của § 7, no. 4 cho f.

Đặc biệt, nếu J hữu hạn và có n phần tử và $x_i = \sum_{j \in J} \xi_{ji} e_j$ $(1 \leq i \leq n)$ là n phần tử của M, thì

(11) $$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
= \left( \sum_{\sigma \in S_n} \varepsilon_\sigma \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n} \right) e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_n}
$$

trong đó $(j_k)_{1 \leq k \leq n}$ là dãy duy nhất gồm n phần tử của J được sắp theo thứ tự tăng, do đó

(12) $$
\det(x_1, x_2, \ldots, x_n) = \sum_{\sigma \in S} \varepsilon_\sigma \cdot \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n}.
$$

Với ký hiệu của Bổ đề 1, so sánh các công thức (10) và (12) cho

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathcal{F}_p(J)} \det(x_{H,1}, x_{H,2}, \ldots, x_{H,p}) e_H
$$

trong đó $ \mathcal{F}_p(J) $ là tập các tập con của $ J $ có $ p $ phần tử và, với mọi tập con $ H \in \mathcal{F}_p(J) $, ta viết $ x_{H,i} = \sum_{j \in H} \xi_{ji} e_j $ và $ e_H = e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_p} $, $ (j_k)_{1 \leq k \leq p} $ là dãy các phần tử của $ H $ được sắp theo thứ tự tăng, với hiểu ngầm rằng $ \det(x_{H,1}, \ldots, x_{H,p}) $ được lấy theo cơ sở $ (e_{jk})_{1 \leq k \leq p} $.

#### Mệnh đề 7 {#alg-iii-s8-prop-7 .statement}

*Cho $ I $ là một tập hữu hạn và $ X = (\xi_{ji})_{(j, i) \in I \times I} $ là một ma trận vuông kiểu (I, I) trên một vành giao hoán $ A $. Khi đó*

$$
\det X = \sum_{\sigma \in S_I} \varepsilon_\sigma \left( \prod_{i \in I} \xi_{\sigma(i), i} \right)
$$

*trong đó $ \sigma $ chạy qua nhóm $ S_I $ của các hoán vị của $ I $ và $ \varepsilon_\sigma $ là dấu của $ \sigma $* (I, § 5, no. 7).

Chú ý có thể chỉ xét trường hợp $ I = \{1, n\} \subset \mathbf{N} $ và khi đó chỉ cần áp dụng công thức (12), trong đó $ (e_i)_{1 \leq i \leq n} $ là cơ sở chính tắc của $ A^n $ và các $ x_i $ là các cột của $ X $ (cf. no. 3, công thức (6)).

Đặc biệt, với định thức của một ma trận cấp 3

$$
X = \begin{pmatrix}
\xi_{11} & \xi_{12} & \xi_{13} \\
\xi_{21} & \xi_{22} & \xi_{23} \\
\xi_{31} & \xi_{32} & \xi_{33}
\end{pmatrix}
$$

ta có

$$
\det(X) = \xi_{11} \xi_{22} \xi_{33} + \xi_{12} \xi_{23} \xi_{31} + \xi_{21} \xi_{32} \xi_{13} - \xi_{13} \xi_{22} \xi_{31} - \xi_{12} \xi_{21} \xi_{33} - \xi_{11} \xi_{23} \xi_{32}.
$$

#### Mệnh đề 8 {#alg-iii-s8-prop-8 .statement}

*Với mọi ma trận vuông $ X $ trên một vành giao hoán, định thức của ma trận chuyển vị $ {}^t X $ bằng định thức của $ X $.*

Giả sử rằng $ X $ có kiểu (I, I). Với mọi cặp có thứ tự các hoán vị $ \sigma, \tau $ của $ S_I $, (vì phép nhân giao hoán)

$$
\prod_{i \in I} \xi_{\sigma(i), i} = \prod_{j \in I} \xi_{\sigma(\tau(j)), \tau(j)}.
$$

Đặc biệt lấy $ \tau = \sigma^{-1} $; dùng thực tế rằng $ \varepsilon_{\sigma^{-1}} = \varepsilon_\sigma $, ta thấy rằng

$$
\det X = \sum_{\sigma \in S_I} \varepsilon_\sigma \left( \prod_{i \in I, i} \xi_{i, \sigma(i)} \right),
$$

điều này chứng minh mệnh đề.

#### Hệ quả 1 {#alg-iii-s8-prop-8-cor-1 .statement}

Với n vectơ $ x_1, \ldots, x_n $ của $ \mathbf{A}^n $, ký hiệu $ Y(x_1, \ldots, x_n) $ là ma trận vuông cấp n có hàng thứ i là $ x_i $, với $ 1 \leq i \leq n $. Khi đó ánh xạ
$$
(x_1, \ldots, x_n) \mapsto \det(Y(x_1, \ldots, x_n))
$$
từ $ (\mathbf{A}^n)^n $ đến $ \mathbf{A} $ là phản xứng và n-tuyến tính.

#### Hệ quả 2 {#alg-iii-s8-prop-8-cor-2 .statement}

Với một ma trận vuông $ X $ có cấp hữu hạn trên một vành giao hoán $ \mathbf{A} $ các điều kiện sau là tương đương:
(i) các hàng của $ X $ độc lập tuyến tính;
(ii) các cột của $ X $ độc lập tuyến tính;
(iii) $ \det X $ không là ước của không trong $ \mathbf{A} $.

Điều này suy ra ngay lập tức từ no. 3, Mệnh đề 6 và Mệnh đề 8 ở trên.

#### Hệ quả 3 {#alg-iii-s8-prop-8-cor-3 .statement}

Cho $ u $ là một tự đồng cấu của một môđun tự do hữu hạn chiều $ M $ và $ ^t u $ là tự đồng cấu chuyển vị của môđun đối ngẫu $ M^* $ (II, § 2, no. 5, Định nghĩa 5); khi đó
$$
\det(^t u) = \det(u).
$$
Nếu $ X $ là ma trận của $ u $ đối với một cơ sở của $ M $, $ ^t X $ là ma trận của $ ^t u $ đối với cơ sở đối ngẫu (II, § 10, no. 4, Mệnh đề 3); vì $ \det(u) = \det(X) $ và $ \det(^t u) = \det(^t X) $, kết luận suy ra từ Mệnh đề 8.

### 5. CÁC ĐỊNH THỨC CON CỦA MỘT MA TRẬN

Let $ X $ be a rectangular matrix $ (\xi_{ij})_{(i,j) \in I \times J} $ of type (I, J) whose indexing sets I and J are totally ordered. If $ H \subset I $ and $ K \subset J $ are finite subsets with the same number $ p $ of elements, there exists a unique increasing bijection $ \phi : H \to K $ (Set Theory, III, § 5, no. 3, Proposition 6); we shall denote by $ X_{H,K} $ the square matrix of type (H, H) equal to $ (\xi_{i,\phi(j)})_{(i,j) \in H \times H} $. If the elements of $ X $ belong to a commutative ring $ \mathbf{A} $, the determinant $ \det(X_{H,K}) $ is called the minor of the matrix $ X $ of indices H, K; these determinants (for all ordered pairs (H, K) of subsets of I and J respectively with $ p $ elements) are also called the minors of $ X $ of order $ p $. With this notation:

#### Mệnh đề 9 {#alg-iii-s8-prop-9 .statement}

Let $ M $ be an $ \mathbf{A} $-module with a basis $ (e_i)_{i \in J} $ (finite or otherwise) whose indexing set $ J $ is totally ordered. For every integer $ p > 0 $, let $ (e_H)_{H \in \mathfrak{S}_p(J)} $ be the corresponding basis of $ \wedge^p(M) $ (§ 7, no. 8). Let $ (x_i)_{1 \leq i \leq p} $ be a sequence of $ p $ elements of $ M $; let
$$
x_i = \sum_{j \in J} \xi_{ji} e_j \quad \text{cho } i \in I = \{1, p\}
$$

and let $ X $ denote the matrix $ (\xi_{ji}) $ of type $ (J, I) $. Then

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathfrak{F}_p(J)} (\det X_{H,I}) e_H.
$$

where $ H $ runs through the set $ \mathfrak{F}_p(J) $ of subsets of $ J $ with $ p $ elements.

Điều này suy ra ngay lập tức từ công thức (12) của no. 4 và công thức (6) của no. 3.

#### Mệnh đề 10 {#alg-iii-s8-prop-10 .statement}

Let $ M $ and $ N $ be two free $ A $-modules of respective dimensions $ m $ and $ n $, $ u : M \to N $ a linear mapping and $ X $ the matrix of $ u $ with respect to a basis $ (e_i)_{1 \leq i \leq m} $ of $ M $ and a basis $ (f_j)_{1 \leq j \leq n} $ of $ N $. Then, for every integer $ p \leq \inf(m, n) $, the matrix of $ \wedge^p(u) $ with respect to the basis $ (e_K)_{K \in \mathfrak{F}_p(I)} $ of $ \wedge^p(M) $ and the basis $ (f_H)_{H \in \mathfrak{F}_p(J)} $ of $ \wedge^p(N) $ (where we have written $ I = \{1, m\} $ and $ J = \{1, n\} $) is the matrix $ (\det(X_{H,K})) $ of type $ (\mathfrak{F}_p(J), \mathfrak{F}_p(I)) $ (and hence with $ \binom{n}{p} $ rows and $ \binom{m}{p} $ columns).

For a subset $ K \subset J $ with $ p $ elements, let $ (j_k)_{1 \leq k \leq p} $ be the sequence of elements of $ K $ arranged in increasing order; theo định nghĩa của $ \wedge^p(u) $, theo § 7, no. 2, công thức (4)

$$
\wedge^p(u)(e_K) = u(e_{j_1}) \wedge u(e_{j_2}) \wedge \cdots \wedge u(e_{j_p}).
$$

Do đó phần tử của ma trận của $ \wedge^p(u) $ nằm ở hàng chỉ số $ H $ và cột chỉ số $ K $ là thành phần chỉ số $ H $ của phần tử $ u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}) $; vì vậy nó bằng $ \det(X_{H,K}) $ theo Mệnh đề 9.

Ma trận $ (\det(X_{H,K})) $ được gọi là lũy thừa ngoại thứ $ p $ của ma trận $ X $ và được ký hiệu bởi $ \wedge^p(X) $. Khi $ p = m = n $, $ \wedge^n(X) $ là ma trận chỉ có phần tử duy nhất $ \det(X) $.

#### Mệnh đề 11 {#alg-iii-s8-prop-11 .statement}

Cho $ M $ là một A-môđun tự do có số chiều hữu hạn $ n $; với mọi tự đồng cấu $ u $ của $ M $ và mọi cặp có thứ tự các phần tử $ \xi, \eta $ của $ A $,

$$
\det(\xi 1_M + \eta u) = \sum_{k \geq 0} \operatorname{Tr}(\wedge^k(u)) \xi^{n-k} \eta^k.
$$

Cho $ (e_i)_{1 \leq i \leq n} $ là một cơ sở của $ M $ và đặt $ I = \{1, n\} $; để tính vế trái của (18), ta phải lập tích

$$
(\xi e_1 + \eta u(e_1)) \wedge (\xi e_2 + \eta u(e_2)) \wedge \cdots \wedge (\xi e_n + \eta u(e_n))
$$

điều này bằng tổng các hạng $ \xi^{n-p} \eta^p z_K $, trong đó

$$
z_K = x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

với $ x_i = u(e_i) $ nếu $ i \in K $, $ x_i = e_i $ nếu $ i \in H = I - K $, trong đó số nguyên $ p $ chạy qua khoảng $ [0, n] $ và, với mỗi $ p $, $ K $ chạy qua tập các tập con của I có $ p $ phần tử. Nếu $ i_1 < i_2 < \cdots < i_{n-p} $ (resp. $ j_1 < j_2 < \cdots < j_p $) là các phần tử của H (resp. K) được sắp theo thứ tự tăng dần, ta có thể viết ($ \S 7 $, no. 8, Hệ quả 1 của Định lý 1 và công thức (19))

$$
z_K = \rho_{H, K} e_{i_1} \wedge e_{i_2} \wedge \cdots \wedge e_{i_{n-p}} \wedge u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}).
$$

Nhưng nếu $ X $ là ma trận của $ u $ đối với cơ sở $ (e_i) $, thì theo Mệnh đề 10

$$
u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}) = \sum_{L \in \mathfrak{F}_p(I)} (\det X_{L, K}) e_L
$$

và do đó

$$
z_K = \rho_{H, K} \sum_{L \in \mathfrak{F}_p(I)} (\det X_{L, K}) e_H \wedge e_L.
$$

Bây giờ $ H \cap L \neq \varnothing $ trừ trường hợp $ L = K $; do đó từ $ \S 7 $, no. 8, công thức (20) suy ra $ z_K = (\det X_{K, K}) e_1 \wedge e_2 \wedge \cdots \wedge e_n $ và công thức (18) rồi suy ra từ Mệnh đề 10 và định nghĩa của vết của một ma trận (II, $ \S 10 $, no. 11, các công thức (49) và (50)).

#### Hệ quả {#alg-iii-s8-n5-cor-1 .statement}

*Với các giả thiết như trong Mệnh đề 11, đối với tự đồng cấu $ \bigwedge(u) $ của A-môđun $ \bigwedge(M) $*

$$(19)$$
$$
\operatorname{Tr}(\bigwedge(u)) = \det(1_M + u).
$$

Chỉ cần thay $ \xi $ và $ \eta $ bởi 1 trong (18) và nhận thấy rằng ma trận của $ \bigwedge(u) $ đối với cơ sở của các $ e_H $ ($ H \in \mathfrak{F}(I) $) là ma trận đường chéo của các ma trận của $ \bigwedge^k(u) $ với $ \geq k $ 0 (II, $ \S 10 $, no. 7, *Ví dụ* IV).

### 6. KHAI TRIỂN CỦA MỘT ĐỊNH THỨC

Cho I là một tập chỉ số hữu hạn được sắp thứ tự toàn phần. Với mọi tập con H của I, ký hiệu H' là phần bù I - H. Cho $ X = (\xi_{ij}) $ là một ma trận vuông kiểu (I, I), có thể xem như ma trận của một tự đồng cấu $ u $ của $ M = A^I $ đối với cơ sở chính tắc $ (e_i)_{i \in I} $ của M. Đặt $ n = \operatorname{Card}(I) $ và cho H là một tập con của I có $ q \leq n $ phần tử và K là một tập con của I có $ n - q $ phần tử; khi đó ta có thể viết (no. 5, Mệnh đề 10)

$$
(\bigwedge^q(u))(e_H) = \sum_R \det(X_{R, H}) e_R
$$
$$
(\bigwedge^{n-q}(u))(e_K) = \sum_S \det(X_{S, K}) e_S
$$

trong đó R (tương ứng S) chạy qua tập các tập con của I có $ q $ (tương ứng $ n - q $) phần tử. Từ $ \S 7 $, no. 8, các công thức (19) và (20) suy ra rằng

$$
e_R \wedge e_S = 0
$$

trừ trường hợp $ S = R' $, do đó có công thức

$$
(20) \quad (\wedge^q(u)(e_H)) \wedge (\wedge^{n-q}(u)(e_K)) = \sum_R \rho_{R, R'} \det(X_{R, H}) \det(X_{R', K}) e_I
$$

trong đó $ R $ chạy qua tập $ \mathcal{F}_q(I) $ các tập con của $ I $ có $ q $ phần tử.

Nếu ta lấy $ K = H' $, thì từ định nghĩa của $ \wedge^n(u) $ (\S 7, no. 2, công thức (4)) và \S 7, no. 3, Hệ quả 1 của Mệnh đề 5 suy ra rằng vế phải của (20) là $ \rho_{H, H'} \wedge^n(u)(e_I) $. Do đó (no. 1, công thức (1) và \S 7, no. 2, công thức (4))

$$
(21) \quad \det(X) = \rho_{H, H'} \sum_{R \in \mathcal{F}_q; R' \neq R} \rho_{R, R'} \det(X_{R, H}) \det(X_{R', H'}).
$$

Mặt khác, nếu $ K \neq H' $, thì $ H \cap K \neq \varnothing $; vì vế trái của (20) là $ \pm \wedge^n(u)(e_H \wedge e_K) $, nên nó bằng không, do đó

$$
(22) \quad \sum_R \rho_{R, R'} \det(X_{R, H}) \det(X_{R', K}) = 0 \quad \text{với } K \neq H'.
$$

Vế phải của (21) được gọi là *khai triển Laplace* của định thức của ma trận $ X $ *theo q cột có chỉ số thuộc H và n - q cột có chỉ số thuộc phần bù H' của H*. Các định thức con $ \det(X_{R, H}) $ và $ \det(X_{R', H'}) $ đôi khi được gọi là *bổ sung*.

Một trường hợp đơn giản quan trọng của khai triển Laplace là trường hợp $ I = \{1, n\} $ và $ q = 1 $, do đó $ H = \{i\} $; với mọi tập con $ R = \{j\} $ của I gồm một phần tử thì $ \det X_{R, H} = \xi_{ji} $. Định thức con $ \det X_{R', H'} $ là định thức của ma trận vuông được suy ra một cách chính tắc (no. 5) từ ma trận nhận được khi bỏ khỏi $ X $ hàng có chỉ số $ j $ và cột có chỉ số $ i $. Ký hiệu ma trận vuông đó là $ X^{ji} $. Hiển nhiên $ \rho_{H, H'} = (-1)^{i-1} $ và $ \rho_{R, R'} = (-1)^{j-1} $; do đó (21) trở thành trong trường hợp này

$$
(23) \quad \det X = \sum_{j=1}^n (-1)^{i+j} \xi_{ji} \det(X^{ji})
$$

và ta cũng thu được tương tự từ (22)

$$
(24) \quad \sum_{j=1}^n (-1)^{ji} \xi_{ji} \det(X^{jk}) = 0 \quad \text{với } k \neq i.
$$

Công thức (23) được gọi là *khai triển định thức của X theo cột có chỉ số i*. Vô hướng $ (-1)^{i+j} \det(X^{ji}) $ được gọi là *phần bù đại số* của các chỉ số $ j $ và $ i $ (hoặc, nói không chính xác, phần bù đại số của $ \xi^{ji} $) trong $ X $.

*Ma trận các phần bù đại số* của $ X $ là ma trận

$$
(25) \quad Y = ((-1)^{i+j} \det(X^{ji}))
$$

mà phần tử ở hàng thứ $ j $ và cột thứ $ i $ là phần bù đại số của các chỉ số $ j $ và $ i $. Các công thức (23) và (24) tương đương với công thức

$$(26)$$
$$
{}^tY . X = (\det X) I_n.
$$

Do đó:

#### Mệnh đề 12 {#alg-iii-s8-prop-12 .statement}

*Với mọi ma trận vuông khả nghịch $ X $ kiểu $(n, n)$, nghịch đảo của $ X $ được cho bởi công thức*

$$(27)$$
$$
X^{-1} = (\det X)^{-1} {}^t Y
$$

*trong đó $ Y $ là ma trận phần bù đại số của $ X $.*

Bằng cách xét *chuyển vị* của $ X $ và dùng Mệnh đề 8 của no. 5, các khai triển Laplace có thể được thu được tương ứng với hai tập hợp các hàng bù nhau và, nói riêng, khai triển của $ \det X $ theo một hàng, do đó có các công thức tương đương với

$$(28)$$
$$
X . {}^t Y = (\det X) I_n,
$$

theo ký hiệu trên.

Dễ dàng kiểm tra rằng nếu $ X $ là ma trận của một tự đồng cấu $ u $ của một $ \mathbf{A} $-môđun tự do $ M $ có chiều $ n $ đối với một cơ sở $ (e_i)_{1 \leq i \leq n} $, thì $ {}^t Y $ là ma trận của tự đồng cấu $ \tilde{u} $ của $ M $ được xác định bởi điều kiện sau: với mọi tập hợp gồm $ n $ phần tử $ x, y_2, \ldots, y_n $ của $ M $,

$$
\tilde{u}(x) \wedge y_2 \wedge \cdots \wedge y_n = x \wedge u(y_2) \wedge \cdots \wedge u(y_n).
$$

$ \tilde{u} $ được gọi là *chuyển vị kép* của $ u $ (xem § 11, no. 11, Hệ quả của Mệnh đề 13).

#### Ví dụ {#alg-iii-s8-n6-exa-1 .statement}

(1) *Định thức Vandermonde.* Cho một dãy $ (\zeta_i)_{1 \leq i \leq n} $ gồm $ n $ phần tử của $ \mathbf{A} $, định thức *Vandermonde* của dãy này là định thức

$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \ldots & 1 \\
\zeta_1 & \zeta_2 & \ldots & \zeta_n \\
\zeta_1^2 & \zeta_2^2 & \ldots & \zeta_n^2 \\
\vdots & \vdots & \ddots & \vdots \\
\zeta_1^{n-1} & \zeta_2^{n-1} & \ldots & \zeta_n^{n-1}
\end{vmatrix}
$$

Ta sẽ chứng minh rằng

$$(29)$$
$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \prod_{i < j} (\zeta_j - \zeta_i).
$$

Vì mệnh đề là hiển nhiên khi $ n = 1 $, ta chứng minh bằng quy nạp theo $ n $.

Với mỗi chỉ số $ k \geq 2 $, ta trừ khỏi hàng có chỉ số $ k $ hàng có chỉ số $ k - 1 $ nhân với $ \zeta_1 $; giá trị của định thức không đổi và do đó

$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \cdots & 1 \\
0 & \zeta_2 - \zeta_1 & \cdots & \zeta_n - \zeta_1 \\
0 & \zeta_2(\zeta_2 - \zeta_1) & \cdots & \zeta_n(\zeta_n - \zeta_1) \\
\cdots & \cdots & \cdots & \cdots \\
0 & \zeta_2^{n-2}(\zeta_2 - \zeta_1) & \cdots & \zeta_n^{n-2}(\zeta_n - \zeta_1)
\end{vmatrix}
$$

do đó, khai triển theo cột thứ nhất rồi lấy nhân tử $ \zeta_k - \zeta_1 $ ra khỏi cột có chỉ số $ k - 1 $ của định thức con thu được ($ 2 \leq k \leq n $)

$$
V(\zeta_1, \ldots, \zeta_n) = (\zeta_2 - \zeta_1)(\zeta_3 - \zeta_1) \cdots (\zeta_n - \zeta_1) V(\zeta_2, \ldots, \zeta_n)
$$

điều này chứng minh (29) bằng quy nạp.

(2) Xét một ma trận vuông cấp $ n $ được viết dưới dạng một "ma trận tam giác trên của các ma trận" (II, § 10, no. 7, Ví dụ IV)

$$
X = \begin{pmatrix} Y & T \\ 0 & Z \end{pmatrix}
$$

Ta chứng minh rằng

$$
\det X = (\det Y)(\det Z).
$$

Cho $ n $ là cấp của ma trận $ X $, $ h $ là cấp của $ Y $, $ (e_i)_{1 \leq i \leq n} $ là cơ sở chính tắc của $ \mathbf{A}^n $ và $ x_i $ ($ 1 \leq i \leq n $) là các cột của $ X $; giả thiết suy ra rằng các cột $ x_1, \ldots, x_h $ thuộc môđun con của $ \mathbf{A}^n $ có cơ sở $ e_1, \ldots, e_h $ và khi đó theo định nghĩa (no. 3, formula (6))

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det Y)e_1 \wedge e_2 \wedge \cdots \wedge e_h.
$$

Mặt khác, với mọi chỉ số $ i > h $, ta có thể viết $ x_i = y_i + z_i $, trong đó $ y_i $ là một tổ hợp tuyến tính của $ e_1, e_2, \ldots, e_h $ và $ z_i $ là một tổ hợp tuyến tính của $ e_{h+1}, \ldots, e_n $. Theo (30), $ x_1 \wedge x_2 \wedge \cdots \wedge x_n \wedge y_i = 0 $ với mọi $ i > h $, do đó

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det Y)e_1 \wedge e_2 \wedge \cdots \wedge e_h \wedge z_{h+1} \wedge \cdots \wedge z_n.
$$

Nhưng theo định nghĩa

$$
z_{h+1} \wedge z_{h+2} \wedge \cdots \wedge z_n = (\det Z)e_{h+1} \wedge e_{h+2} \wedge \cdots \wedge e_n
$$

do đó công thức (30).

Bằng quy nạp theo $ p $, suy ra rằng nếu $ X $ có dạng một ma trận tam giác trên của các ma trận:

$$
X = \begin{pmatrix}
X_{11} & X_{12} & \cdots & X_{1p} \\
0 & X_{22} & \cdots & X_{2p} \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & X_{pp}
\end{pmatrix}
$$

(31) $$
\det X = (\det X_{11})(\det X_{22}) \ldots (\det X_{pp}).
$$

Điều này có thể được áp dụng đặc biệt cho một ma trận tam giác (trong đó mọi $ X_{ii} $ đều có cấp 1) và đặc biệt hơn nữa cho một ma trận đường chéo:

(32) $$
\det(\operatorname{diag}(\alpha_1, \alpha_2, \ldots, \alpha_n)) = \alpha_1 \alpha_2 \ldots \alpha_n.
$$

(3) Cho $ M, M' $ là hai $ A $-môđun tự do có các số chiều tương ứng $ n, n' $, $ u $ là một tự đồng cấu của $ M $ và $ u' $ là một tự đồng cấu của $ M' $. Khi đó

(33) $$
\det(u \otimes u') = (\det u)^{n'} (\det u')^n.
$$

Thật vậy, ta có thể viết $ u \otimes u' = (u \otimes 1_{M'}) \circ (1_M \otimes u') $ và do đó được đưa về trường hợp một trong hai tự đồng cấu $ u, u' $ là đồng nhất. Chẳng hạn nếu $ u' = 1_{M'} $ và $ X $ là ma trận của $ u $ đối với một cơ sở $ (e_i) $ của $ M $, thì ma trận của $ u \otimes 1_{M'} $ đối với tích tenxơ của $ (e_i) $ và một cơ sở của $ M' $ có thể được viết như một ma trận (với $ n' $ hàng và $ n' $ cột) của các ma trận với $ n $ hàng và $ n $ cột

$$
\begin{pmatrix}
X & 0 & \ldots & 0 \\
0 & X & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X
\end{pmatrix}
$$

do đó, theo *Ví dụ 2*,

$$
\det(u \otimes 1_{M'}) = (\det X)^{n'} = (\det u)^{n'}
$$

điều này suy ra ngay công thức (33).

### 7. ỨNG DỤNG VÀO CÁC PHƯƠNG TRÌNH TUYẾN TÍNH

Xét một hệ gồm $ n $ phương trình tuyến tính vô hướng trong $ n $ ẩn trên một vành (*giao hoán*) $ A $ (II, § 2, no. 8):

(34) $$
\sum_{j=1}^n \lambda_{ij} x_j = \eta_i \quad (1 \leq i \leq n).
$$

Cho $ L $ là ma trận vuông $(\lambda_{ij})$ cấp $ n $; bằng cách đồng nhất như thường lệ ma trận với một cột gồm các $ \xi_i $ (resp. các $ \eta_i $) với một phần tử $ x = (\xi_i) $ của $ \mathbf{A}^n $ (resp. phần tử $ y = (\eta_i) $ của $ \mathbf{A}^n $), hệ (34) cũng có thể được viết (II, § 10, no. 3, Mệnh đề 2)

(35)
$$
L.x = y.
$$

Cho $ u $ là tự đồng cấu $ x \mapsto L.x $ của $ \mathbf{A}^n $, với $ L $ làm ma trận theo cơ sở chính tắc; nói rằng phương trình (35) có (ít nhất) một nghiệm với mọi $ y \in \mathbf{A}^n $ nghĩa là $ u $ là toàn ánh; Định lý 1 của no. 2 khi đó suy ra mệnh đề sau:

#### Mệnh đề 13 {#alg-iii-s8-prop-13 .statement}

*Để một hệ gồm $ n $ phương trình tuyến tính trong $ n $ ẩn trên một vành giao hoán có ít nhất một nghiệm, bất kể các vế phải, thì cần và đủ rằng định thức của ma trận của hệ khả nghịch; trong trường hợp này hệ có một nghiệm duy nhất.*

Nếu $ \det L $ không là ước của không trong $ \mathbf{A} $, phương trình (34) tương đương với phương trình
$$
(\det L)L.x = (\det L)y.
$$
Nếu $ M $ là ma trận các phần bù đại số của $ L $, từ (34) và công thức (26) của no. 6 ta suy ra quan hệ
(36)
$$
(\det L)x = {}^tM.y
$$
có thể cũng viết
(37)
$$
(\det L)\xi_i = \sum_{j=1}^n (-1)^{i+j}(\det L^{ij})\eta_j = \det L_i \quad (1 \leq i \leq n)
$$
trong đó $ L_i $ ký hiệu ma trận thu được bằng cách thay cột của $ L $ có chỉ số $ i $ bởi $ y $. Các công thức (37) được gọi là *các công thức Cramer* cho hệ (34); mọi nghiệm của (34) cũng là một nghiệm của (37). Ngược lại, từ (36), xét đến công thức (28) của no. 6, ta suy ra
(38)
$$
(\det L)(L.x - y) = 0
$$
và do đó, nếu $ \det L $ không là ước của không trong $ \mathbf{A} $, thì các hệ (34) và (37) là *tương đương*; nếu $ \det L $ khả nghịch, nghiệm duy nhất của (34) được cho bởi
(39)
$$
\xi_i = (\det L)^{-1}(\det L_i) \quad (1 \leq i \leq n).
$$
Một hệ (34) sao cho $ \det L $ khả nghịch cũng còn được gọi là một *hệ Cramer*.

Đặc biệt, cho $ y = 0 $; khi đó theo Hệ quả 3 của no. 2 suy ra:

#### Mệnh đề 14 {#alg-iii-s8-prop-14 .statement}

*Để một hệ tuyến tính thuần nhất gồm $ n $ phương trình trong $ n $ ẩn trên một vành giao hoán có một nghiệm khác không, thì cần và đủ rằng định thức của ma trận của nó là một ước của không.*

### 8. TRƯỜNG GIAO HOÁN

Tất cả những điều trên đều áp dụng khi vành $ \mathbf{A} $ là một trường giao hoán; nhưng có những giản lược và các kết quả bổ sung.

Do đó Mệnh đề 12 của § 7, no. 9 có thể được phát biểu trong trường hợp này như sau:

#### Mệnh đề 15 {#alg-iii-s8-prop-15 .statement}

Cho $ \mathbf{E} $ là một không gian vectơ trên một trường giao hoán; để $ p $ vectơ $ x_i \in \mathbf{E} $ ($ 1 \leq i \leq p $) độc lập tuyến tính, cần và đủ rằng $ x_1 \wedge x_2 \wedge \cdots \wedge x_p \neq 0 $.

#### Hệ quả {#alg-iii-s8-n8-cor-1 .statement}

Cho $ X $ là một ma trận kiểu $(m, n)$ trên một trường giao hoán. Hạng của $ X $ bằng số nguyên lớn nhất $ p $ sao cho tồn tại ít nhất một định thức con của $ X $ cấp $ p $ khác $0$.

Hạng của $ X $ là số lượng lớn nhất các cột độc lập tuyến tính của $ X $ (II, § 10, no. 12, Định nghĩa 7). Hệ quả đó khi ấy suy ra từ Mệnh đề 15 và công thức (17) của no. 5.

Xét bây giờ trường hợp một hệ gồm $ m $ phương trình tuyến tính trong $ n $ ẩn trên một trường giao hoán $ \mathbf{K} $:

$$
\sum_{j=1}^n \lambda_{ij} \xi_j = \eta_i \quad (1 \leq i \leq m).
$$

(41)

#### Mệnh đề 16 {#alg-iii-s8-prop-16 .statement}

Cho $ L = (\lambda_{ij}) $ là ma trận (kiểu $(m, n)$) của hệ (41). Cho $ M $ là ma trận kiểu $(m, n+1)$ thu được bằng cách thêm vào $ L $ cột thứ $(n+1)$ $(\eta_i)$ (II, § 10, no. 1). Cho $ p $ là hạng của $ L $ (tính bằng cách áp dụng Hệ quả của Mệnh đề 15). Giả sử rằng định thức con $ \Delta $ của $ L $, tức là định thức của ma trận thu được bằng cách bỏ các hàng và các cột có chỉ số $ \geq p + 1 $ trong $ L $, là $ \neq 0 $ (điều này luôn có thể làm được nhờ một phép hoán vị thích hợp trên các hàng của $ L $ và một phép hoán vị thích hợp trên các cột của $ L $). Khi đó, để hệ (41) có ít nhất một nghiệm, điều kiện cần và đủ là tất cả các định thức con cấp $ p + 1 $ của $ M $, tức là các định thức của các ma trận con cấp $ p + 1 $ của $ M $ có các cột mang chỉ số $ 1, 2, \ldots, p $ và $ n+1 $, đều bằng không. Nếu vậy, các nghiệm của hệ (41) là các nghiệm của hệ gồm $ p $ phương trình đầu tiên; nếu viết chúng dưới dạng

$$
\sum_{j=1}^p \lambda_{ij} \xi_j = \eta_i - \sum_{k=p+1}^n \lambda_{ik} \xi_k \quad (1 \leq i \leq p)
$$

mọi nghiệm của hệ này thu được bằng cách gán cho các $ \xi_k $ có chỉ số $ k > p $ những giá trị tùy ý và áp dụng các công thức Cramer (no. 7, các công thức (37)) để tính các $ \xi_j $ có chỉ số $ j \leq p $.

Ta biết (II, § 10, no. 12, Mệnh đề 12) rằng để hệ (41) có ít nhất một nghiệm, điều kiện cần và đủ là các ma trận $ L $ và $ M $ có cùng hạng. Sau khi hoán vị các hàng và các cột của $ L $ để thỏa mãn điều kiện của mệnh đề, hãy ký hiệu $ a_i $ ($ 1 \leq i \leq p $) là $ p $ cột đầu tiên của $ L $ và $ y = (\eta_i) $ là cột thứ $(n+1)$ của $ M $; vì theo giả thiết mọi cột của $ L $ đều là tổ hợp tuyến tính của các $ a_i $, nói rằng $ M $ có cùng hạng $ p $ như $ L $ có nghĩa là $ y $ là một tổ hợp tuyến tính của các $ a_i $, hay cũng vậy (Mệnh đề 15) là $ a_1 \wedge \cdots \wedge a_p \wedge y = 0 $. Điều kiện khả năng trong mệnh đề là bản dịch của quan hệ sau, xét đến công thức (17) của no. 5. Hơn nữa, vì $ p $ hàng đầu tiên của $ M $ độc lập tuyến tính, nên các hàng có chỉ số $ > p $ là các tổ hợp tuyến tính của chúng, do đó mọi nghiệm của (42) cũng là nghiệm của (41). Khẳng định cuối cùng khi đó là một hệ quả ngay lập tức của Mệnh đề 13 của no. 7.

### 9. NHÓM ĐƠN MÔĐULA $ \mathbf{SL}(n, A) $

Xét $ \mathbf{M}_n(A) $ là vành các ma trận vuông cấp $ n $ trên $ A $. Xét ánh xạ $ \det : \mathbf{M}_n(A) \to A $. Nhóm $ \mathbf{GL}(n, A) $ gồm các phần tử khả nghịch của $ \mathbf{M}_n(A) $ (đẳng cấu với nhóm các tự đẳng cấu của $ A $-môđun $ A^n $ (II, § 10, no. 7)) chính là ảnh ngược qua ánh xạ này của nhóm nhân $ A^* $ gồm các phần tử khả nghịch của $ A $ (no. 3, Mệnh đề 5). Mặt khác, lưu ý rằng ánh xạ $ \det : \mathbf{GL}(n, A) \to A^* $ là một đồng cấu nhóm (no. 3, Mệnh đề 5).

Ánh xạ $ \det : \mathbf{M}_n(A) \to A $ hơn nữa là *toàn ánh* (và do đó đồng cấu $ \det : \mathbf{GL}(n, A) \to A^* $ cũng toàn ánh); vì, với mọi $ \lambda \in A $,

$$
\det(\operatorname{diag}(\lambda, 1, \ldots, 1)) = \lambda
$$

nhờ công thức (32) của no. 6.

*Hạt nhân* của đồng cấu toàn ánh $ \det : \mathbf{GL}(n, A) \to A^* $ là một nhóm con chuẩn tắc của $ \mathbf{GL}(n, A) $, được cấu thành bởi các ma trận *đơn môđula*; nó được ký hiệu bởi $ \mathbf{SL}_n(A) $ hoặc $ \mathbf{SL}(n, A) $ và thường được gọi là *nhóm đơn môđula* hay *nhóm tuyến tính đặc biệt* của các ma trận vuông cấp $ n $ trên $ A $.

Trong no. này ta sẽ xét trường hợp $ A $ là một *trường*. Nhắc lại rằng với $ 1 \leq i \leq n, 1 \leq j \leq n $, $ E_{ij} $ ký hiệu ma trận vuông cấp $ n $ có mọi phần tử đều bằng không trừ phần tử ở hàng chỉ số $ i $ và cột chỉ số $ j $, là phần tử bằng 1; với $ I_n $ ký hiệu ma trận đơn vị cấp $ n $, ta viết $ B_{ij}(\lambda) = I_n + \lambda E_{ij} $ cho mọi cặp có thứ tự của các chỉ số *phân biệt* $ i, j $ và mọi $ \lambda \in A $ (II, § 10, no. 13).

#### Mệnh đề 17 {#alg-iii-s8-prop-17 .statement}

*Cho $ K $ là một trường giao hoán. Nhóm đơn môđula $ \mathbf{SL}(n, K) $ được sinh bởi các ma trận $ B_{ij}(\lambda) $ với $ i \neq j $ và $ \lambda \in K $. *

Theo II, § 10, no. 13, Mệnh đề 14, ta biết rằng mọi ma trận trong $ \mathbf{GL}(n, K) $ đều là một tích của các ma trận có dạng $ B_{ij}(\lambda) $ và một ma trận có dạng $ \operatorname{diag}(1, 1, \ldots, 1, \alpha) $ với $ \alpha \in K^* $. Bây giờ là ngay lập tức rằng $ \det(B_{ij}(\lambda)) = 1 $ và $ \det(\operatorname{diag}(1, \ldots, 1, \alpha)) = \alpha $ (no. 6, *Ví dụ 2*); do đó có mệnh đề.

#### Hệ quả {#alg-iii-s8-n9-cor-1 .statement}

*Nhóm* $ \mathbf{SL}(n, K) $ *là nhóm giao hoán tử của* $ \mathbf{GL}(n, K) $, *trừ trường hợp* $ n = 2 $ *và* $ K $ *là một trường có 2 phần tử*.

As $ \mathbf{SL}(n, K) $ là hạt nhân của đồng cấu det từ $ \mathbf{GL}(n, K) $ đến một nhóm giao hoán $ K^* $, nên $ \mathbf{SL}(n, K) $ chứa nhóm giao hoán tử $ \Gamma $ của $ \mathbf{GL}(n, K) $ (I, § 6, no. 2). Để chứng minh rằng $ \mathbf{SL}(n, K) = \Gamma $, theo Mệnh đề 17, chỉ cần chỉ ra rằng, với mọi $ \lambda \in K^* $, $ B_{ij}(\lambda) $ thuộc $ \Gamma $. Bây giờ, $ B_{ij}(\lambda) $ là một tự đẳng cấu liên hợp của $ B_{ij}(1) $ trong $ \mathbf{GL}(n, K) $ vì $ B_{ij}(\lambda) = Q . B_{ij}(1) . Q^{-1} $, trong đó $ Q $ ký hiệu ma trận của tự đẳng cấu $ v $ của $ K^n $ đối với cơ sở chính tắc $ (e_i) $ sao cho $ v(e_i) = \lambda e_i, v(e_k) = e_k $ với $ k \neq i $. Mặt khác, gọi $ u_{ij} $ (với $ i \neq j $) là tự đẳng cấu của $ K^n $ sao cho $ u_{ij}(e_i) = -e_j, \ u_{ij}(e_j) = e_i, \ u_{ij}(e_k) = e_k $ với $ k \notin \{i, j\} $, khi đó nó thuộc $ \mathbf{SL}(n, K) $; rồi $ B_{ji}(\lambda) = U_{ij} B_{ij}(-\lambda) U_{ij}^{-1} $, trong đó $ U_{ij} $ là ma trận của $ u_{ij} $ đối với cơ sở chính tắc. Tương tự, nếu $ 1 < i < j $, thì $ B_{1j}(\lambda) = U_{1i} B_{ij}(\lambda) U_{1i}^{-1} $ và cuối cùng, với $ 2 < j $, $ B_{12}(\lambda) = U_{2j} B_{1j}(\lambda) U_{2j}^{-1} $. Điều này chứng minh rằng mọi $ B_{ij}(\lambda) $ đều có cùng ảnh $ s $ trong $ \mathbf{GL}(n, K)/\Gamma $ và còn lại phải chỉ ra rằng $ s $ là phần tử đơn vị.

Trước hết, giả sử $ K $ chứa một phần tử $ \lambda $ khác 0 và 1; khi đó $ 1 = \lambda + (1 - \lambda) $, hai số hạng ở vế phải đều khác 0; hệ thức $ B_{12}(1) = B_{12}(\lambda) B_{12}(1 - \lambda) $ cho thấy $ s^2 = s $ và do đó $ s $ là phần tử đơn vị.

Giả sử bây giờ rằng $ n \geq 3 $. Tích $ B_{21}(1) B_{31}(1) $ là ma trận của một tự đẳng cấu $ u $ của $ K^n $ sao cho $ u(e_1) = e_1 + e_2 + e_3, u(e_i) = e_i $ với $ i \neq 1 $. Nếu $ S $ là ma trận của tự đẳng cấu $ u' $ của $ K^n $ sao cho $ u'(e_2) = e_2 + e_3, u'(e_i) = e_i $ với $ i \neq 2 $, thì $ S . B_{21}(1) B_{31}(1) . S^{-1} = B_{21}(1) $; cũng suy ra rằng $ s^2 = s $, điều này hoàn tất chứng minh.

#### Nhận xét {#alg-iii-s8-n9-rem-1 .statement}

(1) $ \mathbf{GL}(2, \mathbf{F}_2) = \mathbf{SL}(2, \mathbf{F}_2) $; đây là một nhóm giải được có cấp 6, mà nhóm giao hoán tử của nó có chỉ số 2 (II, § 10, Bài tập 14).

(2) Với cùng ký hiệu như trên, có thể chứng minh như trong I, § 5, no. 7, Mệnh đề 9 rằng, với $ i < j, j - i > 1 $, $ u_{ij} = u_{j-1, j} u_i, _{j-1} u_{j-1, j}^{-1} $; do đó *nhóm* $ \mathbf{SL}(n, K) $ *được sinh bởi các ma trận* $ B_{12}(\lambda) $ *và* $ U_{i, i+1} $ *với* $ 1 \leq i \leq n - 1 $.

### 10. MÔĐUN $ \mathbf{A}[X] $ GẮN VỚI MỘT TỰ ĐỒNG CẤU CỦA MỘT $ \mathbf{A} $-MÔĐUN

Cho $ M $ là một $ \mathbf{A} $-môđun và $ u $ là một tự đồng cấu của $ M $. Xét vành đa thức $ \mathbf{A}[X] $ trong một biến bất định $ X $ trên $ \mathbf{A} $. Với mọi đa thức $ p \in \mathbf{A}[X] $ và mọi $ x \in M $, ta viết

$$
p . x = p(u)(x).
$$

Vì $ (pq)(u) = p(y) \circ q(u) $ với hai đa thức $ p, q $ của $ \mathbf{A}[X] $, nên cấu trúc môđun $ \mathbf{A}[X] $ được xác định trên $ M $; tập hợp $ M $, với cấu trúc này, sẽ được ký hiệu là $ M_u $; cấu trúc $ \mathbf{A} $-môđun trên $ M $ thu được bằng cách hạn chế vành các toán tử của $ M_u $ xuống $ \mathbf{A} $. Chú ý rằng các môđun con của $ M_u $ chỉ là các môđun con của $ M $ mà *ổn định* đối với $ u $.

Vì ánh xạ $(p, x) \mapsto p.x$ của $A[X] \times M$ vào $M$ là $A$-song tuyến tính, nên nó xác định một cách chính tắc một ánh xạ tuyến tính $\phi : A[X] \otimes_A M \to M$ sao cho
$$
\phi(p \otimes x) = p.x = p(u)(x).
$$
Mặt khác, $A[X] \otimes_A M$ có một cấu trúc môđun $A[X]$ một cách chính tắc (II, § 5, no. 1); ta sẽ ký hiệu môđun $A[X]$ này bởi $M[X]$; ánh xạ $\phi : M[X] \to M_u$ là tuyến tính $A[X]$ vì, với $p, q$ trong $A[X]$ và $x \in M$,
$$
\phi(q(p \otimes x)) = \phi((qp) \otimes x) = (qp).x = q(u)(p(u)(x)) = q.\phi(p \otimes x).
$$
Hơn nữa, $u$ là một tự đồng cấu $A[X]$ của $M_u$, vì
$$
u(p.x) = u(p(u)(x)) = (up(x))(x) = p.u(x).
$$
Cuối cùng, một tự đồng cấu $A[X]$ $\bar{u}$ của $M[X]$ được xác định bằng cách viết (II, § 5, no. 1)
$$
\bar{u}(p \otimes x) = p \otimes u(x).
$$
Hơn nữa suy ra từ các công thức (44) và (45) rằng các ánh xạ tuyến tính $A[X]$ $u, \bar{u}$ và $\phi$ liên quan với nhau bởi quan hệ
$$
\phi \circ \bar{u} = u \circ \phi.
$$
Ký hiệu $\psi$ là tự đồng cấu $A[X]$ $X - \bar{u}$ của $M[X]$, do đó $\psi(p \otimes x) = (Xp) \otimes x - p \otimes u(x)$. Ta có mệnh đề sau:

#### Mệnh đề 18 {#alg-iii-s8-prop-18 .statement}

*Dãy các đồng cấu $A[X]$*
$$
M[X] \xrightarrow{\psi} M[X] \xrightarrow{\phi} M_u \longrightarrow 0
$$
là khớp.

Vì $\phi(1 \otimes x) = x$ với mọi $x \in M$, rõ ràng $\phi$ là toàn ánh; mặt khác,
$$
\phi(X(p \otimes x)) = X.\phi(p \otimes x) = u(\phi(p \otimes x)),
$$
nói cách khác, theo (46), $\phi \circ X = u \circ \phi = \phi \circ \bar{u}$; điều này chứng tỏ rằng $\phi \circ \psi = 0$. Còn phải kiểm tra rằng $\operatorname{Ker} \phi \subset \operatorname{Im} \psi$. Với điều này, chú ý rằng, vì các đơn thức $X^k$ ($k \geq 0$) tạo thành một cơ sở của $A$-môđun $A[X]$, mọi phần tử $z \in M[X]$ đều có thể được viết duy nhất dưới dạng $z = \sum_k X^k \otimes x_k$, trong đó $(x_k)$ là một họ các phần tử của $M$, có giá hữu hạn. Nếu $z \in \operatorname{Ker} \phi$, thì $\phi(z) = \sum_k u^k(x_k) = 0$ và ta có thể viết
$$
z = \sum_k (X^k \otimes x_k - 1 \otimes u^k(x_k)) = \sum_k (X^k - \bar{u}^k)(1 \otimes x_k).
$$
Nhưng vì các tự đồng cấu $A[X]$ $X$ và $\bar{u}$ của $M[X]$ giao hoán với nhau, nên

X^k - \bar{u}^k = (X - \bar{u}) \circ \left( \sum_{j=0}^{k-1} X^j \bar{u}^{k-j-1} \right) điều này chứng tỏ rằng tồn tại một $ y \in M[X] $ sao cho $ z = \psi(y) $.

Bây giờ cho $ M' $ là một $ A $-môđun khác và $ u' $ là một tự đồng cấu của $ M' $; cho $ M'_{u'} $, $ \phi' $, $ \bar{u}' $, $ \psi' $ là môđun và ánh xạ nhận được từ $ M' $ và $ u' $ như $ M_u $, $ \phi $, $ \bar{u} $, $ \psi $ được nhận được từ $ M $ và $ u $. Khi đó:

#### Mệnh đề 19 {#alg-iii-s8-prop-19 .statement}

*Để một ánh xạ g từ M vào M' là một A[X]-đồng cấu từ M_u vào M'_u, thì cần và đủ rằng g là một A-đồng cấu từ M vào M' sao cho $ g \circ u = u' \circ g $. Khi đó, nếu $ \bar{g} $ là A[X]-đồng cấu của M[X] vào M'[X] bằng $ 1_{A[x]} \otimes g $ (II, § 5, no. 1), thì biểu đồ*

$$
\begin{array}{cccccc}
M[X] & \xrightarrow{\psi} & M[X] & \xrightarrow{\phi} & M_u & \longrightarrow 0 \\
\downarrow \bar{g} & & \downarrow \bar{g} & & \downarrow g & \\
M'[X] & \xrightarrow{\psi'} & M'[X] & \xrightarrow{\phi'} & M'_{u'} & \longrightarrow 0
\end{array}
$$

là *giao hoán*.

Điều kiện $ g \circ u = u' \circ g $ là hiển nhiên cần thiết theo (43) để $ g $ là một A[X]-đồng cấu; nó đủ, vì nó suy ra bằng quy nạp rằng $ g \circ u^n = {u'}^n \circ g $ với mọi số nguyên $ n > 0 $. Mặt khác, với mọi $ x \in M $ và mọi $ p \in A[X] $,

$$
\phi'(\bar{g}(p \otimes x)) = \phi'(p \otimes g(x)) = p(u')(g(x)) = g(p(u)(x)) = g(\phi(p \otimes x))
$$
và
$$
\bar{u}'(g(p \otimes x)) = \bar{u}'(p \otimes g(x)) = p \otimes u'(g(x)) = p \otimes g(u(x)) = \bar{g}(\bar{u}(p \otimes x))
$$
điều đó chứng minh tính giao hoán của biểu đồ (48).

### 11. ĐA THỨC ĐẶC TRƯNG CỦA MỘT TỰ ĐỒNG CẤU

Cho $ M $ là một $ A $-môđun tự do có chiều $ n $ và $ u $ là một tự đồng cấu của $ M $. Xét vành đa thức trên hai ẩn $ A[X, Y] $ và $ A[X, Y] $-môđun $ M[X, Y] = A[X, Y] \otimes_A M $; cho $ \bar{u} $ là tự đồng cấu của $ A[X, Y] $-môđun $ M[X, Y] $ được dẫn xuất một cách chính tắc từ $ u $ (II, § 5, no. 1). Từ no. 5, Mệnh đề 11 suy ra rằng

$$
\det(X - Y \bar{u}) = \sum_{j=0}^n (-1)^j \mathrm{Tr}(\wedge^j(u)) X^{n-j} Y^j
$$

vì nếu $ U $ là ma trận của $ u $ đối với một cơ sở $ (e_i)_{1 \leq i \leq n} $ của $ M $, $ U $ là ma trận của $ \bar{u} $ đối với cơ sở $ (1 \otimes e_i)_{1 \leq i \leq n} $ của $ M[X, Y] $, do đó

$$
\mathrm{Tr}(\wedge^j(\bar{u})) = \mathrm{Tr}(\wedge^j(u)).
$$

#### Định nghĩa 3 {#alg-iii-s8-def-3 .statement}

Cho $ M $ là một $ A $-môđun tự do hữu hạn chiều và $ u $ là một tự đồng cấu của $ M $. Định thức của tự đồng cấu $ X - \bar{u} $ của $ A[X] $-môđun tự do $ M[X] $ được gọi là đa thức đặc trưng của $ u $ và được ký hiệu là $ \chi_u(X) $.

Nếu $ M $ có hạng $ n $, từ (49) suy ra rằng

$$
\chi_u(X) = \sum_{j=0}^n (-1)^j \operatorname{Tr}(\wedge^j(u)) X^{n-j}
$$

với $ \det(X - Y \bar{u}) = \det(X . I_n + Y U) $ và $ \det(X - \bar{u}) = \det(X . I_n - U) $. Do đó suy ra rằng $ \chi_u(X) $ là một đa thức đơn khởi bậc $ n $, trong đó hệ số của $ X^{n-1} $ là $ -\operatorname{Tr}(u) $ và số hạng tự do là $ (-1)^n \det(u) $.

#### Mệnh đề 20 ("Định lý Cayley–Hamilton") {#alg-iii-s8-prop-20 .statement}

Với mọi tự đồng cấu $ u $ của một A-môđun tự do hữu hạn chiều, $ \chi_u(u) = 0 $.

Theo ký hiệu của Mệnh đề 18 ($ \S 3 $, no. 10), với mọi $ x \in M $, $ \chi_u(u)(x) $ là ảnh qua $ \phi $ của $ \chi_u(X) \otimes x $. Nhưng nếu $ v $ là tự đồng cấu của $ M[X] $, đồng chuyển vị của $ X - \bar{u} $ (no. 6), thì

$$
\chi_u(X) \otimes x = \chi_u(X)(1 \otimes x) = (X - \bar{u})(v(1 \otimes x))
$$

và kết luận suy ra từ Mệnh đề 18 của no. 10.

### Bài tập {#alg-iii-s8-exercises}

Xem [các bài tập cho § 8](exercises/s8/).
