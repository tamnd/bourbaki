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
content_sha256: 45714da37952ec6b0b4d56ef856b3d56fad15f6bae7098a4165ea5b300c0524e
translated_from: content/en/alg/III/08_s8_determinants.md
source_content_sha256: 61460bcdd2ad78ff72f6c630c7a5c2c7dff603a886863a3d32aebd73ea99c369
translation_model: gpt-5-6-mini
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
