---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 2
section_title: Rings and modules of fractions
lang: vi
source: ac-i-vii
book_pages: 55-79, 123-136
pdf_pages: 0075-0099, 0143-0156
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF RINGS OF FRACTIONS
      page: 55
      pdf_page: 75
    - "no": 2
      title: MODULES OF FRACTIONS
      page: 60
      pdf_page: 80
    - "no": 3
      title: CHANGE OF MULTIPLICATIVE SUBSET
      page: 64
      pdf_page: 84
    - "no": 4
      title: PROPERTIES OF MODULES OF FRACTIONS
      page: 67
      pdf_page: 87
    - "no": 5
      title: IDEALS IN A RING OF FRACTIONS
      page: 70
      pdf_page: 90
    - "no": 6
      title: NILRADICAL AND MINIMAL PRIME IDEALS
      page: 73
      pdf_page: 93
    - "no": 7
      title: FRACTIONS OF TENSOR PRODUCTS AND HOMOMORPHISM MODULES
      page: 75
      pdf_page: 95
    - "no": 8
      title: APPLICATION TO ALGEBRAS
      page: 77
      pdf_page: 97
    - "no": 9
      title: MODULES OF FRACTIONS OF GRADED MODULES
      page: 78
      pdf_page: 98
statements: 52
exercises: 23
content_sha256: da9b36a5c15278014539ec6b5bd85b02065c88d9dd427fb0e5572395b42061e8
translated_from: content/en/ac/II/02_s2_rings_and_modules_of_fractions.md
source_content_sha256: 862eb533634e57154a3cf7493419fd43f7b530676770c590cac1d84e03bc8d92
translation_model: gpt-5-6-mini, gpt-5.4, gpt-5.4-mini
translation_run: translate-vi-9a26a26c
glossary_version: 34
glossary_terms_sha256: 9eaa6e3983f0528b490882593cc0f87023c3cb716b4beee922811f1764f941eb
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. VÀNH VÀ MÔĐUN PHÂN THỨC

### 1. ĐỊNH NGHĨA CÁC VÀNH PHÂN THỨC

#### Định nghĩa 1 {#ac-ii-s2-def-1 .statement}

*Cho $A$ là một vành. Một tập con $S$ của $A$ được gọi là có tính nhân nếu mọi tích hữu hạn của các phần tử của $S$ đều thuộc $S$.*

Điều này cũng có nghĩa là $1 \in S$ và tích của hai phần tử của $S$ thuộc $S$.

*Ví dụ*
(1) Với mọi $a \in A$, tập hợp các $a^n$, trong đó $n \in \mathbf{N}$, là một tập con có tính nhân của $A$.
(2) Cho $p$ là một iđêan của $A$. Để $A - p$ là một tập con có tính nhân của $A$, điều kiện cần và đủ là $p$ nguyên tố.
(3) Tập hợp các phần tử của $A$ không là ước của không là một tập con có tính nhân của $A$.

(4) Nếu S và T là các tập con có tính nhân của A, tập hợp ST gồm các tích st, trong đó s ∈ S và t ∈ T, là một tập con có tính nhân.

(5) Cho G là một tập có hướng (đối với quan hệ ⊂ ) gồm các tập con có tính nhân của A. Khi đó T = ⋃_{S ∈ G} S là một tập con có tính nhân của A, vì hai phần tử bất kỳ của T đều thuộc một tập con S ∈ G nào đó, do đó tích của chúng thuộc T.

(6) Mọi giao của các tập con có tính nhân của A đều là một tập con có tính nhân.

Với mọi tập con S của một vành A, tồn tại các tập con có tính nhân của A chứa S, chẳng hạn chính A. Giao của tất cả các tập con này là tập con có tính nhân nhỏ nhất của A chứa S; nó được gọi là được sinh bởi S. Ngay lập tức suy ra rằng nó là tập hợp gồm tất cả các tích hữu hạn của các phần tử của S.

#### Mệnh đề 1 {#ac-ii-s2-prop-1 .statement}

Cho A là một vành và S là một tập con của A. Tồn tại một vành A' và một đồng cấu h từ A vào A' có các tính chất sau:
(1) các phần tử của h(S) là khả nghịch trong A ;
(2) với mọi đồng cấu u từ A vào một vành B sao cho các phần tử của u(S) là khả nghịch trong B, tồn tại một đồng cấu duy nhất u' từ A vào B sao cho u = u' ∘ h.

Nói cách khác, (A', h) là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết Tập hợp, Chương IV, § 3, no. 1) với các điều kiện sau: loài cấu trúc Σ được xét là một vành, các cấu xạ là các đồng cấu vành và các ánh xạ a là các đồng cấu từ A vào một vành sao cho ảnh của S qua đồng cấu đó gồm các phần tử khả nghịch. Nhắc lại (loc. cit.) rằng, nếu (A', h) và (A'_1, h_1) đều là các nghiệm của bài toán này, thì tồn tại một đẳng cấu duy nhất j : A' → A'_1 sao cho h_1 = j ∘ h.

Cho $\overline{S}$ là tập con có tính nhân của A được sinh bởi S. Rõ ràng mọi nghiệm của bài toán ánh xạ phổ quát nói trên cũng là một nghiệm của bài toán ánh xạ phổ quát thu được bằng cách thay thế S bởi $\overline{S}$ và ngược lại.

Xét, trong tập hợp A × S, quan hệ sau đây giữa các phần tử (a, s), (a', s') :

(1) "Tồn tại t ∈ $\overline{S}$ sao cho t (sa' − s'a) = 0".

Quan hệ này là một quan hệ tương đương: rõ ràng nó phản xạ và đối xứng; nó bắc cầu, vì nếu t (sa' − s'a) = 0 và t'(s'a'' − s''a') = 0, thì tt's'(sa' − s'a) = 0 và tt's' ∈ $\overline{S}$. Gọi A' là tập thương của A × $\overline{S}$ theo quan hệ tương đương này; với mọi cặp có thứ tự (a, s) ∈ A × $\overline{S}$, ta ký hiệu a/s là ảnh chính tắc của (a, s) trong A và đặt h(a) = a/1 với mọi a ∈ A. Ta sẽ thấy rằng A' có thể được trang bị một cấu trúc vành sao cho cặp có thứ tự (A', h) là nghiệm của bài toán.

Cho x = a/s và y = b/t là hai phần tử của A'. Các phần tử (ta + sb)/st và $ab/st$ chỉ phụ thuộc vào $x$ và $y$; vì nếu $x = a'/s'$, theo giả thiết tồn tại $r \in \overline{S}$ sao cho $r(s'a - sa') = 0$, do đó

$$
r(s't(ta + sb) - st(ta' + s'b)) = 0
$$

và $r(s'tab - sta'b) = 0$. Dễ dàng kiểm tra rằng các luật hợp thành $(x, y) \mapsto x + y = (ta + sb)/st$ và $(x, y) \mapsto xy = ab/st$ xác định một cấu trúc vành giao hoán trên $\mathbf{A}'$, trong đó $0/1$ là phần tử đơn vị đối với phép cộng và $1/1$ là phần tử khả nghịch. Hơn nữa, ngay lập tức thấy rằng h là một đồng cấu vành và rằng, với mọi $s \in S$, $s/1$ là khả nghịch trong $\mathbf{A}'$, nghịch đảo của nó là $1/s$. Cuối cùng, cho B là một vành và u : $\mathbf{A} \to B$ là một đồng cấu sao cho các phần tử u(S) là khả nghịch trong B; tồn tại một ánh xạ duy nhất u' : $\mathbf{A}' \to B$ sao cho

(2)
$$
u'(a/s) = u(a)(u(s))^{-1} \quad (a \in \mathbf{A}, s \in \overline{S}).
$$

Nếu a/s = a'/s', tồn tại t ∈ $\overline{S}$ sao cho t(sa' - s'a) = 0, do đó u(t)(u(s)u(a') - u(s')u(a)) = 0 và, vì u(t), u(s) và u(s') đều khả nghịch, u(a)(u(s))^{-1} = u(a')(u(s'))^{-1}. Dễ dàng kiểm tra rằng u' là một đồng cấu đối với phép cộng và phép nhân; cuối cùng, rõ ràng u' \circ h = u và u' là đồng cấu duy nhất thỏa mãn hệ thức này, vì hệ thức đó suy ra

$$
u'(a/s) = u'((a/1)(1/s)) = u'(1/s)u'(a/1) = u'(1/s)u(a)
$$

và $1 = u'(1/1) = u'(s/1)u'(1/s) = u(s)u'(1/s)$, do đó công thức (2).

#### Định nghĩa 2 {#ac-ii-s2-def-2 .statement}

Cho $\mathbf{A}$ là một vành, $S$ là một tập con của $\mathbf{A}$ và $\overline{S}$ là tập con nhân được sinh bởi $S$. Vành các phân thức của $\mathbf{A}$ xác định bởi $S$ và ký hiệu là $\mathbf{A}[S^{-1}]$ là tập thương của $\mathbf{A} \times \overline{S}$ theo quan hệ tương đương (1) với cấu trúc vành được xác định bởi

$$
(a/s) + (b/t) = (ta + sb)/st, \qquad (a/s)(b/t) = (ab)/(st)
$$

với $a, b$ trong $\mathbf{A}$, $s, t$ trong $\overline{S}$. Ánh xạ chính tắc của $\mathbf{A}$ vào $\mathbf{A}[S^{-1}]$ là đồng cấu $a \mapsto a/1$, làm cho $\mathbf{A}[S^{-1}]$ thành một $A$-đại số.

Trong chương này, ta thường ký hiệu ánh xạ chính tắc này bởi $i_A^S$; chứng minh của Mệnh đề 1 chỉ ra rằng cặp có thứ tự $(\mathbf{A}[S^{-1}], i_A^S)$ thỏa mãn các điều kiện trong mệnh đề của Mệnh đề này.

**Nhận xét**

(1) Hiển nhiên $\mathbf{A}[\overline{S}^{-1}] = \mathbf{A}[S^{-1}]$.

(2) Hai phần tử của $\mathbf{A}[S^{-1}]$ luôn có thể được viết dưới dạng $a/s$ và $a'/s$ ($a, a'$ trong $\mathbf{A}$, $s \in \overline{S}$) với cùng một "mẫu số" $s$, vì nếu $b/t$ và $b'/t'$ là hai phần tử của $\mathbf{A}[S^{-1}]$, thì $b/t = bt'/tt'$ và $b'/t' = b't/tt'$.

(3) Hạt nhân của $i_A^S$ là tập hợp các $a \in A$ sao cho tồn tại $s \in \overline{S}$ thỏa mãn $sa = 0$; để $i_A^S$ đơn ánh, điều kiện cần và đủ là $S$ không chứa ước của không trong $A$.

(4) Nếu $S$ chứa một phần tử lũy linh, thì $0 \in \overline{S}$ và vành $A[S^{-1}]$ thu gọn thành 0; điều này suy ra dễ dàng từ Định nghĩa 2.

(5) Để $i_A^S$ là một song ánh, điều kiện cần và đủ là mọi phần tử $s \in S$ đều khả nghịch trong $A$: điều kiện này hiển nhiên là cần, vì $s/1$ khả nghịch trong $A[S^{-1}]$; nó đủ, vì với mọi $t \in \overline{S}$, $t$ do đó khả nghịch trong $A$ và $a/t = at^{-1}/1$ trong $A[S^{-1}]$; do đó $i_A^S$ là toàn ánh và như đã thấy trong Nhận xét 3 nó là đơn ánh. Khi đó $A$ và $A[S^{-1}]$ được đồng nhất thông qua $i_A^S$.

Ví dụ (7). Nếu $R$ là tập hợp các phần tử trong $A$ không là ước của 0, thì vành $A[R^{-1}]$ chính xác là điều mà chúng ta đã gọi là vành các phân thức của $A$ (Đại số, Chương I, §9, no. 4); để tránh mọi nhầm lẫn, chúng ta thường gọi nó là vành phân thức toàn phần của $A$. Đặc biệt, nếu $A$ là một miền nguyên, $A[R^{-1}]$ là trường các phân thức của $A$ (sđd.).

#### Mệnh đề 2 {#ac-ii-s2-prop-2 .statement}

Cho $A, B$ là hai vành, $S$ là một tập con của $A$, $T$ là một tập con của $B$ và $f$ là một đồng cấu từ $A$ đến $B$ sao cho $f(S) \subset T$. Tồn tại một đồng cấu duy nhất $f'$ từ $A[S^{-1}]$ đến $B[T^{-1}]$ sao cho $f'(a/1) = f(a)/1$ với mọi $a \in A$.

Giả sử thêm rằng $T$ được chứa trong tập con nhân của $B$ sinh bởi $f(S)$. Khi đó, nếu $f$ là toàn ánh (tương ứng, đơn ánh) thì $f'$ cũng là toàn ánh (tương ứng, đơn ánh).

Mệnh đề đầu tiên tương đương với việc nói rằng tồn tại một đồng cấu duy nhất $f': A[S^{-1}] \to B[T^{-1}]$ tạo ra một biểu đồ giao hoán:

$$
\begin{array}{ccc}
A & \xrightarrow{f} & B \\
i_A^S \downarrow & & \downarrow i_B^T \\
A[S^{-1}] & \xrightarrow{f'} & B[T^{-1}]
\end{array}
$$

Bây giờ quan hệ $f(S) \subset T$ kéo theo rằng $i_B^T(f(s))$ là khả nghịch trong $B[T^{-1}]$ với mọi $s \in S$ và chỉ cần áp dụng Mệnh đề 1 cho $i_B^T \circ f$. Dễ dàng suy ra từ (2) rằng, với mọi $a \in A$ và $s \in \overline{S}$ (tập con nhân của $A$ sinh bởi $S$),

$$
f'(a/s) = f(a)/f(s).
$$

Giả sử rằng $T$ được chứa trong tập con nhân sinh bởi $f(S)$, mà chính xác là $f(\overline{S})$. Khi đó suy ra từ (3) rằng, nếu $f$ là toàn ánh, thì $f'$ cũng là toàn ánh.

Bây giờ giả sử rằng $f$ là đơn ánh. Cho $a/s$ là một phần tử của hạt nhân của $f'$. Vì tập con nhân sinh bởi $T$ là $f(\overline{S})$, tồn tại một phần tử $s_1 \in \overline{S}$ sao cho $f(s_1)f(a) = 0$, do đó $f(s_1a) = 0$ và $s_1a = 0$ vì $f$ là đơn ánh; khi đó $a/s = 0$, điều này chứng minh rằng $f'$ là đơn ánh.

Nhận xét (6). Nếu các phần tử của $T$ là khả nghịch trong $B$, $B[T^{-1}]$ được đồng nhất với $B$ bằng đẳng cấu $i_B^T$ và khi đó $f'$ trở thành đồng nhất với đồng cấu duy nhất $u'$ của $A[S^{-1}]$ vào $B$ sao cho $u' \circ i_A^S = f$.

#### Hệ quả 1 {#ac-ii-s2-prop-2-cor-1 .statement}

*Cho $A$ là một vành, $S$ là một tập con của $A$ và $u$ là một đơn cấu từ $A$ vào một vành $B$ sao cho các phần tử của $u(S)$ là khả nghịch trong $B$. Đồng cấu duy nhất $u'$ của $A[S^{-1}]$ vào $B$ sao cho $u' \circ i_A^S = u$ khi đó là đơn ánh.*

Đây là một hệ quả ngay lập tức của Mệnh đề 2 và Nhận xét 6.

#### Hệ quả 2 {#ac-ii-s2-prop-2-cor-2 .statement}

*Cho $A$ là một vành và $S$ và $T$ là hai tập con của $A$ sao cho $S \subset T$. Tồn tại một đồng cấu duy nhất $i_A^{T,S}$ từ $A[S^{-1}]$ đến $A[T^{-1}]$ sao cho $i_A^T = i_A^{T,S} \circ i_A^S$.*

Với mọi $a \in A$, $i_A^{T,S}$ khi đó ánh xạ phần tử $a/s$ trong $A[S^{-1}]$ thành phần tử $a/s$ trong $A[T^{-1}]$.

Nhận xét (7). Chú ý rằng, nếu $i_A^T$ là đơn ánh, thì $i_A^{T,S}$ cũng vậy (Hệ quả 1). Điều này xảy ra nếu $T$ là tập hợp $R$ các phần tử của $A$ không phải là các ước của 0; khi đó có thể đồng nhất $A[S^{-1}]$ với vành con của vành phân thức toàn phần $A[R^{-1}]$ sinh bởi $A$ và các phần tử nghịch đảo trong $A[R^{-1}]$ của các phần tử của $S$.

#### Hệ quả 3 {#ac-ii-s2-prop-2-cor-3 .statement}

*Cho $A, B, C$ là ba vành, $S$ (tương ứng $T, U$) là một tập con nhân của $A$ (tương ứng $B, C$), $f : A \to B$, $g : B \to C$ là hai đồng cấu và $h : A \to C$ là đồng cấu hợp thành $g \circ f$; giả sử rằng $f(S) \subset T$, $g(T) \subset U$. Gọi $f' : A[S^{-1}] \to B[T^{-1}]$, $g' : B[T^{-1}] \to C[U^{-1}]$, $h' : A[S^{-1}] \to C[U^{-1}]$ là các đồng cấu tương ứng với $f, g, h$; khi đó $h' = g' \circ f'$.*

Điều này suy ra dễ dàng từ các định nghĩa.

Đặc biệt, nếu $S, T, U$ là ba tập con nhân của $A$ sao cho $S \subset T \subset U$, thì $i_A^{U,S} = i_A^{U,T} \circ i_A^{T,S}$.

#### Hệ quả 4 {#ac-ii-s2-prop-2-cor-4 .statement}

*Cho $S$ là một tập con của một vành $A$, $B$ là một vành con của $A[S^{-1}]$ chứa $i_A^S(A)$ và $S'$ là tập hợp $i_A^S(A)$. Gọi $j$ là đơn ánh chính tắc của $B$ vào $A[S^{-1}]$; đồng cấu duy nhất $g$ từ $B[{S'}^{-1}]$ đến $A[S^{-1}]$ sao cho $g \circ i_A^S = j$ là một đẳng cấu.*

Ánh xạ $g$ là đơn ánh theo Hệ quả 1; vành $g(B[{S'}^{-1}])$ chứa $i_A^S(A)$ và các nghịch đảo của các phần tử của $S'$; do đó nó bằng $A[S^{-1}]$.

Nếu $A$ là một miền nguyên và $0 \notin S$, ký hiệu $A[S^{-1}]$ trùng với ký hiệu trong Đại số, Chương IV, § 2, no. 1; hơn nữa, nếu $S$ là nhân, $A[S^{-1}]$ trong trường hợp này trùng với tập hợp được ký hiệu là $S^{-1}A$ trong Đại số, Chương I, § 1, no. 1.

Như một sự mở rộng của ký hiệu, với mọi tập con nhân $S$ của một vành $A$, từ nay về sau ta ký hiệu $S^{-1}A$ là vành các phân thức $A[S^{-1}]$. Nếu $S$ là phần bù của một iđêan nguyên tố $p$ của $A$, ta viết $A$, thay cho $S^{-1}A$.

Nếu $A$ là một miền nguyên và $0 \notin S$, $S^{-1}A$ luôn được đồng nhất với một vành con của trường phân thức của $A$, chứa $A$ (Nhận xét 7).

### 2. MÔĐUN PHÂN THỨC

Đồng cấu chính tắc $i_A^S : A \to A[S^{-1}]$ được định nghĩa ở No. 1 cho phép ta xem mọi $A[S^{-1}]$-môđun như một $A$-môđun.

#### Mệnh đề 3 {#ac-ii-s2-prop-3 .statement}

Cho $A$ là một vành, $S$ là một tập con của $A$, $M$ là một $A$-môđun, $M'$ là $A$-môđun $M \otimes_A A[S^{-1}]$ và $f$ là đồng cấu $A$ chính tắc $x \mapsto x \otimes 1$ từ $M$ vào $M'$. Khi đó:
(1) Với mọi $s \in S$, phép vị tự $z \mapsto sz$ của $M'$ là song ánh.
(2) Với mọi $A$-môđun $N$ sao cho, với mọi $s \in S$, phép vị tự $y \mapsto sy$ của $N$ là song ánh, và mọi đồng cấu $u$ từ $M$ vào $N$, tồn tại một đồng cấu duy nhất $u'$ từ $M'$ vào $N$ sao cho $u = u' \circ f$.

Nói cách khác, $(M', f)$ là một nghiệm của bài toán ánh xạ phổ quát (Lý thuyết Tập hợp, chương IV, § 3, No. 1) với các điều kiện sau: loài cấu trúc $\Sigma$ là loài của một $A$-môđun trong đó các phép vị tự cảm sinh bởi các phần tử của $S$ là song ánh, các cấu xạ là các đồng cấu $A$-môđun và các ánh xạ-$a$ cũng là các đồng cấu $A$-môđun.

Với mọi $A$-môđun $N$ và mọi $a \in A$, ký hiệu $h_a$ là phép vị tự $y \mapsto ay$ trong $N$; khi đó $a \mapsto h_a$ là một đồng cấu vành từ $A$ vào $\operatorname{End}_A(N)$. Nói rằng $h_a$ là song ánh có nghĩa là $h_a$ là một phần tử khả nghịch của $\operatorname{End}_A(N)$. Giả sử rằng, với mọi $s \in S$, $h_s$ là khả nghịch trong $\operatorname{End}_A(N)$; khi đó các phần tử $h_a$, với $a \in A$, và các nghịch đảo của các phần tử $h_s$, với $s \in S$, sinh trong $\operatorname{End}_A(N)$ một vành con giao hoán $B$, và đồng cấu $a \mapsto h_a$ từ $A$ vào $B$ có tính chất là ảnh của các phần tử của $S$ là khả nghịch. Do đó (no. 1, Mệnh đề 1), tồn tại một đồng cấu duy nhất $h'$ từ $A[S^{-1}]$ vào $B$ sao cho

$$
h'(a/s) = h_a(h_s)^{-1};
$$

Ngược lại, nếu $N$ là một $A[S^{-1}]$-môđun và được xem như một A-môđun nhờ $i_A^S$, thì các phép vị tự $y \mapsto sy$, với $s \in S$, là song ánh, vì $y \mapsto (1/s)y$ là ánh xạ nghịch đảo của $y \mapsto sy$; và cấu trúc $A[S^{-1}]$-môđun trên $N$ dẫn xuất từ cấu trúc A-môđun của nó theo quá trình được mô tả ở trên chính là cấu trúc $A[S^{-1}]$-môđun đã cho ban đầu. Do đó có một sự tương ứng một-một chính tắc giữa các $A[S^{-1}]$-môđun và các A-môđun trong đó các phép vị tự cảm sinh bởi các phần tử của S là song ánh; hơn nữa, nếu $N$, $N'$ là hai A-môđun có tính chất này thì mọi đồng cấu môđun A $u : N \to N'$ cũng là một đồng cấu của các cấu trúc $A[S^{-1}]$-môđun trên $N$ và $N'$, vì, với mọi y $\in N$ và mọi $s \in S$, ta có thể viết $u(y) = u(s.((1/s)y)) = s.u((1/s)y)$, do đó $u((1/s)y) = (1/s)u(y)$; đảo lại là hiển nhiên.

Như vậy, mệnh đề của Mệnh đề 3 chính là đặc trưng hóa môđun thu được từ M bằng cách mở rộng các vô hướng đến $A[S^{-1}]$, có tính đến cách diễn giải ở trên (Đại số, Chương II, § 5, no. 1, Nhận xét 1).

#### Định nghĩa 3 {#ac-ii-s2-def-3 .statement}

Cho A là một vành, S là một tập con của A, $\overline{S}$ là tập con nhân của A sinh bởi S và M là một A-môđun. Khi đó môđun phân thức của M xác định bởi S và ký hiệu là $M[S^{-1}]$ hoặc $\overline{S}^{-1}M$ là $A[S^{-1}]$-môđun $M \otimes_A A[S^{-1}]$.

Trong chương này, thông thường ta sẽ ký hiệu $i_M^S$ là ánh xạ chính tắc $m \mapsto m \otimes 1$ từ M vào

**Nhận xét**
(1) Rõ ràng $M[\overline{S}^{-1}] = M[S^{-1}]$.
(2) Với $m \in M$ và $s \in \overline{S}$ ta cũng viết $m/s$ cho phần tử $m \otimes (1/s)$ của $M[S^{-1}]$. Mọi phần tử của $M[S^{-1}]$ đều có dạng, vì một phần tử như vậy có dạng $\sum_i m_i \otimes (a_i/s)$, trong đó $m_i \in M, a_i \in A, s \in S$ (no. 1, Nhận xét 2), và

$$
m_i \in 3 (a_i/s) = (a_i m_i) \in 3 (1/s),
$$

do đó $\sum_i m_i \otimes (a_i/s) = m \otimes (1/s)$, trong đó $m = \sum_i a_i m_i$. Khi đó

(4)
$$
(m/s) + (m'/s') = (s'm + sm')/ss'
$$
(5)
$$
(a/s)(m/s') = (am)/(ss')
$$

trong đó $m, m' \in M, a \in A$ và $s, s' \in S$.

(3) Nếu S là phần bù của một iđêan nguyên tố p của A, ta viết M_p thay cho S^{-1}M.

(4) Cho M là một A[S^{-1}]-môđun; nếu M được xem một cách chính tắc như một A-môđun, thì i_M^S là một song ánh, vì cặp có thứ tự gồm M và ánh xạ đồng nhất 1 cũng hiển nhiên là một nghiệm của bài toán ánh xạ phổ quát được giải bởi M[S^{-1}] và i_M^S. Khi đó M được đồng nhất với M[S^{-1}].

#### Mệnh đề 4 {#ac-ii-s2-prop-4 .statement}

*Cho S là một tập con nhân tính của A và M là một A-môđun. Để có m|s = 0 (m \in M, s \in S), điều kiện cần và đủ là tồn tại s' \in S sao cho s'm = 0.*

Nếu s' \in S sao cho s'm = 0, thì rõ ràng m|s = (s'm)/(ss') = 0. Ngược lại, giả sử rằng m|s = 0. Vì 1/s khả nghịch trong S^{-1}A, nên m/1 = 0. Với mọi môđun con-A P của S^{-1}A chứa 1, ta ký hiệu bởi \beta(P, m) ảnh của (m, 1) dưới ánh xạ chính tắc từ M \times P đến M \otimes_A P; khi đó \beta(S^{-1}A, m) = 0. Ta biết (*Đại số*, Chương II, § 6, no. 3, Hệ quả 4 của Mệnh đề 7) rằng tồn tại một môđun con *hữu hạn sinh* P của S^{-1}A chứa 1 và sao cho \beta(P, m) = 0. Với mọi t \in S ta ký hiệu bởi A_t tập hợp các a/t, trong đó a \in A; vì P hữu hạn sinh, tồn tại t \in S sao cho P \subset A_t (no. 1, Nhận xét 2), do đó \beta(A_t, m) = 0. Ánh xạ a \mapsto a/t từ A đến A_t là toàn ánh; gọi B là hạt nhân của nó. Nó xác định một ánh xạ toàn ánh h : M \otimes_A A \to M \otimes_A A_t, có hạt nhân là BM (M được đồng nhất với M \otimes A); khi đó \beta(A_t, m) = h(tm) và do đó tm có thể được biểu diễn dưới dạng $\sum_{i=1}^r b_i m_i$, trong đó b_i \in B, m_i \in M (1 \leq i \leq r). Vì b_i/t = 0 với 1 \leq i \leq r, nên tồn tại t' \in S sao cho t'b_i = 0 với 1 \leq i \leq r, do đó t'tm = 0, điều này chứng minh Mệnh đề 4.

#### Hệ quả 1 {#ac-ii-s2-prop-4-cor-1 .statement}

*Để có m|s = m'|s' trong S^{-1}M, điều kiện cần và đủ là tồn tại t \in S sao cho t(s'm - sm') = 0.*

$$(m|s) - (m'|s') = (s'm - sm')/ss'.$$

#### Hệ quả 2 {#ac-ii-s2-prop-4-cor-2 .statement}

*Cho M là một A-môđun hữu hạn sinh. Để có S^{-1}M = 0, điều kiện cần và đủ là tồn tại s \in S sao cho sM = 0.*

Không cần điều kiện nào trên M, rõ ràng quan hệ sM = 0 với một s \in S nào đó kéo theo S^{-1}M = 0. Ngược lại, giả sử rằng S^{-1}M = 0 và cho (m_i)_{1 \leq i \leq n} là một hệ các phần tử sinh của M; các m_i/1 sinh ra S^{-1}A-môđun S^{-1}M, nên nói rằng S^{-1}M = 0 tương đương với nói rằng m_i/1 = 0 với 1 \leq i \leq n; theo mệnh đề 4 tồn tại $s_i \in S$ sao cho $s_i m_i = 0$ và, lấy $s = s_1 s_2 \cdots s_n$, ta có $s m_i = 0$ với mọi $i$ và do đó $sM = 0$.

#### Hệ quả 3 {#ac-ii-s2-prop-4-cor-3 .statement}

*Cho M là một A-môđun hữu hạn sinh. Để một iđêan $a \& A$ thỏa mãn $aM = M$, điều kiện cần và đủ là tồn tại $a \in a$ sao cho $(1 + a)M = 0$.*

Rõ ràng quan hệ $(1 + a)M = 0$ kéo theo $M = aM$. Để chứng minh đảo lại, ta dùng bổ đề sau:

#### Bổ đề 1 {#ac-ii-s2-lem-1 .statement}

*Với mọi iđêan a của A, tập S gồm các phần tử $1 + a$, trong đó $a \in a$, là một tập con nhân tính của A và tập $a'$ gồm các phần tử của $S^{-1}A$ có dạng $a/s$, trong đó $a \in a$ và $s \in S$, là một iđêan được chứa trong căn Jacobson của $S^{-1}A$.*

Mệnh đề thứ nhất là hiển nhiên, cũng như việc $a'$ là một iđêan của $S^{-1}A$. Mặt khác, $(1/1) + (a/s) = (s + a)/s$ và $s + a \in S$ với mọi $s \in S$ và $a \in a$ theo định nghĩa của S; do đó $(1/1) + (a/s)$ khả nghịch trong $S^{-1}A$ với mọi $a/s \in a'$, điều này hoàn tất chứng minh của bổ đề (*Đại số*, Chương VIII, § 6, no. 3, Định lý 1).

Khi đó, nếu đặt $N = S^{-1}M$, thì rõ ràng N là một $S^{-1}A$-môđun hữu hạn sinh; nếu $aM = M$, thì $a'N = N$ và suy ra $N = 0$ theo Bổ đề Nakayama (*Đại số*, Chương VIII, § 6, no. 3, Hệ quả của Mệnh đề 6); hệ quả suy ra từ Hệ quả 2.

#### Mệnh đề 5 {#ac-ii-s2-prop-5 .statement}

*Cho A, B là hai vành, S là một tập con nhân tính của A, T là một tập con nhân tính của B và f là một đồng cấu từ A vào B sao cho $f(S) \subset T$. Cho M là một A-môđun, N là một B-môđun và u là một ánh xạ A-tuyến tính từ M vào N. Khi đó tồn tại duy nhất một ánh xạ $S^{-1}A$-tuyến tính $u'$ từ $S^{-1}M$ đến $T^{-1}N$ sao cho $u'(m/1) = u(m)/1$ với mọi $m \in M$.*

Ánh xạ $i_N^T \circ u$ từ M vào $T^{-1}N$ là A-tuyến tính. Hơn nữa, nếu $s \in S$, thì $f(s) \in T$, do đó phép vị tự cảm sinh bởi s trên $T^{-1}N$ là song ánh. Sự tồn tại và tính duy nhất của $u'$ suy ra từ Mệnh đề 3. Khi đó, với $m \in M$ và $s \in S$,

$$
u'(m/s) = u(m)/f(s).
$$

Với cùng ký hiệu, cho C là một vành thứ ba, U là một tập con nhân của C, g là một đồng cấu từ B vào C sao cho $g(T) \subset U$, P là một C-môđun, v là một ánh xạ B-tuyến tính từ N vào P và $v'$ là ánh xạ $T^{-1}B$-tuyến tính từ B vào $U^{-1}P$ liên kết với v. Khi đó

$$
(v \circ u)' = v' \circ u'
$$

trong đó vế trái là ánh xạ A-tuyến tính $S^{-1}M \to U^{-1}P$ liên kết với $v \circ u$. Tương tự, nếu $u_1$ là một ánh xạ A-tuyến tính thứ hai từ M vào N, thì

$$
(u + u_1)' = u' + u_;
$$

vế trái là ánh xạ A-tuyến tính $S^{-1}M \to T^{-1}N$ liên kết với $u + u_1$.

Nhận xét (5). Nếu, trong Mệnh đề 5, ta lấy $B = A, T = S$ và $f = 1_A$, thì dễ dàng thấy rằng $u'$ chính là ánh xạ $u \otimes 1 : M \otimes S^{-1}A \to N \otimes S^{-1}A$. Từ nay về sau, ta sẽ ký hiệu nó là $S^{-1}u$; nếu S là phần bù của một iđêan nguyên tố $p$ của A, ta viết $u_p$ thay cho $S^{-1}u$.

#### Mệnh đề 6 {#ac-ii-s2-prop-6 .statement}

Cho $f$ là một đồng cấu từ một vành A vào một vành B và S là một tập con nhân của A. Tồn tại một ánh xạ duy nhất j từ $(f(S))^{-1}B$ vào $S^{-1}B$ (trong đó B được xem là một A-môđun nhờ f) sao cho $j(b|f(s)) = b|s$ với mọi $b \in B, s \in S$. Nếu $f' : S^{-1}A \to (f(S))^{-1}B$ là đồng cấu vành liên kết với f (no. 1, Mệnh đề 2), thì $j \circ f' = S^{-1}f$. Ánh xạ j là một đẳng cấu của cấu trúc $S^{-1}A$-môđun trên $(f(S))^{-1}B$ được xác định bởi $f'$ lên cấu trúc đó trên $S^{-1}B$, đồng thời là một đẳng cấu của cấu trúc B-môđun trên $(f(S))^{-1}B$ lên cấu trúc đó trên $S^{-1}B$ (thu được từ định nghĩa $S^{-1}B = (S^{-1}A) \otimes_A B$).

Nếu $b, b'$ thuộc B, $s, s'$ thuộc S, thì các điều kiện $b|s = b'|s'$ và $b|f(s) = b'|f(s')$ là tương đương, như suy ra từ Hệ quả 1 của Mệnh đề 4, mệnh đề này thiết lập sự tồn tại của j và chứng minh rằng j là song ánh; tính duy nhất của j là hiển nhiên. Rõ ràng j là một đẳng cấu nhóm cộng. Nếu $a \in A, b \in B, s \in S, t \in S$, thì

$$
(a|s).(b|f(t)) = f'(a|s)(b|f(t)) = f(a)|f(s)(b|f(t)) = (f(a)b)|f(st),
$$

từ đó suy ra rằng j là $(S^{-1}A)$-tuyến tính. Rõ ràng $j \circ f^1 = S^{-1}f$. Cuối cùng, nếu $b \in B, b' \in B, s \in S$, thì $j(b.(b'|f(s))) = j(bb'|f(s)) = bb'|s = b.(b'|s)$, điều này chứng minh khẳng định cuối cùng.

Ánh xạ j của Mệnh đề 6 được gọi là đẳng cấu chính tắc của $(fS)^{-1}B$ lên $S^{-1}B$. Nói chung, hai tập hợp này được đồng nhất nhờ $f'$; khi đó $f' = S^{-1}f, i_B^S = i_B^{f(S)}$.

### 3. THAY ĐỔI TẬP CON NHÂN

Cho A là một vành, S là một tập con nhân của A và M là một A-môđun. Nếu T là một tập con nhân của A chứa S, thì theo Mệnh đề 5 của no. 2, tồn tại một ánh xạ $S^{-1}A$-tuyến tính duy nhất $i_M^{T,S} : S^{-1}M \to T^{-1}M$ sao cho i_M^T = i_M^{T,S} \circ i_M^S; ánh xạ i_M^{T,S} biến phần tử m/s của $S^{-1}M$ thành phần tử m/s của $T^{-1}M$. Dễ dàng kiểm tra rằng i_M^{T,S} = i_A^{T,S} \otimes 1_M. Nếu U là một tập con nhân thứ ba của A sao cho $T \subset U$, thì i_M^{U,S} = i_M^{U,T} \circ i_M^{T,S}; hơn nữa, nếu $u: M \to N$ là một đồng cấu A-môđun, biểu đồ

$$
\begin{array}{ccc}
S^{-1}M & \xrightarrow{s^{-1}u} & S^{-1}N \\
i_M^{T,S} \downarrow & & \downarrow i_N^{T,S} \\
T^{-1}M & \xrightarrow{T^{-1}u} & T^{-1}N
\end{array}
$$

là giao hoán.

#### Mệnh đề 7 {#ac-ii-s2-prop-7 .statement}

Cho A là một vành và S, T là hai tập con nhân của A. Đặt T' = i(T_A^S).

(i) Tồn tại một đẳng cấu duy nhất j từ vành (ST)^{-1}A lên vành T'^{-1}(S^{-1}A) sao cho biểu đồ

$$
\begin{array}{ccc}
A & \xrightarrow{i_A^S} & S^{-1}A \\
i_M^{ST} \downarrow & & \downarrow i_{S^{-1}A}^{T'-1A} \\
(ST)^{-1}A & \xrightarrow{j} & {T'}^{-1}(S^{-1}A)
\end{array}
$$

là giao hoán.

(ii) Cho M là một A-môđun. Tồn tại một đẳng cấu (ST)^{-1}A duy nhất k từ (ST)^{-1}A-môđun (ST)^{-1}M lên T'^{-1}(S^{-1}A)-môđun T'^{-1}(S^{-1}M) sao cho biểu đồ

$$
\begin{array}{ccc}
M & \xrightarrow{i_M^S} & S^{-1}M \\
i_A^{ST} \downarrow & & \downarrow i_{S^{-1}M}^{T'-1M} \\
(ST)^{-1}M & \xrightarrow{k} & {T'}^{-1}(S^{-1}M)
\end{array}
$$

là giao hoán.

(i) Ta dùng định nghĩa của (ST)^{-1}A như nghiệm của một bài toán ánh xạ phổ quát. Cho B là một vành và f là một đồng cấu từ A đến B sao cho f(ST) gồm các phần tử khả nghịch. Vì f(S) do đó gồm các phần tử khả nghịch, tồn tại một đồng cấu duy nhất f': S^{-1}A \to B sao cho f = f' \circ i_A^S (no. 1, Mệnh đề 1). Với mọi t \in T, f'(i_A^S(t)) = f(t) là khả nghịch trong B theo giả thiết. do đó f'(T') gồm các phần tử khả nghịch; khi đó tồn tại, theo no. 1, Mệnh đề 1, một đồng cấu duy nhất f'' từ T'^{-1}(S^{-1}A) đến B sao cho f'' = f'' \circ i_{S^{-1}A}^{T'}, do đó f = f'' \circ u, đặt u = i_{S^{-1}A}^{T'} \circ i_S^A.

Hơn nữa, nếu $f''_1 : {T'}^{-1}(S^{-1}A) \to B$ là một đồng cấu thứ hai sao cho $f''_1 \circ u = f$, thì $(f''_1 \circ i^{T'}_{S^{-1}A}) \circ i^S_A = (f'' \circ i^{T'}_{S^{-1}A}) \circ i^S_A$, do đó $f''_1 \circ i^{T'}_{S^{-1}A} = f'' \circ i^{T'}_{S^{-1}A}$ và do đó $f''_1 = f''$.

Vì các ảnh theo $u$ của các phần tử của ST trong ${T'}^{-1}(S^{-1}A)$ là khả nghịch, cặp có thứ tự $({T'}^{-1}(S^{-1}A), u)$ là một nghiệm của bài toán ánh xạ phổ quát (đối với A và ST) được xét trong no. 1. Điều này chứng minh sự tồn tại và tính duy nhất của $j$.

(ii) Chứng minh hoàn toàn tương tự với chứng minh của (i), dùng trong trường hợp này no. 2, Mệnh đề 3, và để lại cho người đọc.

#### Mệnh đề 8 {#ac-ii-s2-prop-8 .statement}

Cho A là một vành và S, T là hai tập con nhân của A sao cho $S \subset T$. Các tính chất sau là tương đương:

(a) *Đồng cấu* $i^{T,S}_A : S^{-1}A \to T^{-1}A$ *là song ánh*.
(b) *Với mọi A-môđun M, đồng cấu* $i^{T,S}_A : S^{-1}M \to T^{-1}M$ *là song ánh*.
(c) *Với mọi* $t \in T$, *tồn tại* $a \in A$ *sao cho* $at \in S$ *(nói cách khác, mọi phần tử của T chia hết một phần tử của S)*.
(d) *Mọi iđêan nguyên tố giao với T đều giao với S*.

Ta đã thấy ở trên rằng $i^{T,S}_A = 1_M \otimes i^{T,S}_A$, điều này chứng minh ngay lập tức sự tương đương của (a) và (b). Đặt $T' = i^S_A(T)$; khi đó (Mệnh đề 7) $T^{-1}A$ được đồng nhất với ${T'}^{-1}(S^{-1}A)$ và (a) tương đương với việc nói rằng các phần tử của $T'$ là *khả nghịch* trong $S^{-1}A$ (no. 1, *Nhận xét 5*). Bây giờ, nói rằng $(t/1)(a/s) = 1/1$ ($t \in T$, $a \in A, s \in S$) có nghĩa là tồn tại $s' \in S$ sao cho $tas' = ss'$, điều này chỉ ra sự tương đương của (a) và (c). Ta chứng minh rằng (d) kéo theo (c). Cho $t$ là một phần tử của T và giả sử rằng $t/1$ không khả nghịch trong $S^{-1}A$; khi đó tồn tại một iđêan cực đại $m'$ của $S^{-1}A$ chứa $t/1$ (*Đại số*, Chương I, § 8, no. 7, Định lý 2) và $p = (i^S_A)^{-1}(m')$ là một iđêan nguyên tố của A chứa $t$ và không giao với S (vì ảnh theo $i^S_A$ của một phần tử của S là khả nghịch). Ngược lại, nếu tồn tại một iđêan nguyên tố $p$ giao với T mà không giao với S, thì không có phần tử nào của $p \cap T$ có thể chia hết một phần tử của S; điều này chứng minh rằng (c) kéo theo (d) và hoàn tất chứng minh.

Suy ra từ Mệnh đề 8 rằng, trong số các tập con nhân T của A chứa S và thỏa mãn các điều kiện tương đương của Mệnh đề 8, tồn tại một tập *lớn nhất*, gồm *tất cả* các phần tử của A chia hết một phần tử của S (xem Bài tập 1).

#### Mệnh đề 9 {#ac-ii-s2-prop-9 .statement}

Cho I là một tập có thứ tự trước có hướng phải, $(S_\alpha)_{\alpha \in I}$ là một họ tăng các tập con nhân của một vành A và $S = \bigcup_{\alpha \in I} S_\alpha$. Ta viết $\rho_{\beta \alpha} = i^{S_\beta, S_\alpha}_{A^{S_\beta, S_\alpha}}$ với $\alpha \leq \beta$, $\rho_\alpha = i^{S_\alpha, S_\alpha}$. Khi đó $(S_\alpha^{-1}A, \rho_{\beta \alpha})$ là một hệ trực tiếp của các vành và, nếu, với mọi $\alpha \in I$, $\rho'_\alpha$ là ánh xạ chính tắc của $S_\alpha^{-1}A$ đến $\lim \rightarrow S_\alpha^{-1}A$, tồn tại một đẳng cấu duy nhất $j$ từ $\lim \rightarrow S_\alpha^{-1}A$ đến $S^{-1}A$ sao cho $j \circ \rho'_\alpha = \rho_\alpha$ với mọi $\alpha \in I$.

Với $\alpha \leq \beta \leq \gamma$, $\rho_{\gamma \alpha} = \rho_{\gamma \beta} \circ \rho_{\beta \alpha}$ (no. 1, Hệ quả 3 to Mệnh đề 2), do đó $(S_\alpha^{-1}A, \rho_{\beta \alpha})$ là một hệ trực tiếp. Ký hiệu $A' = \lim \rightarrow S_\alpha^{-1}A$; vì $\rho_\alpha = \rho_\beta \circ \rho_{\beta \alpha}$ với $\alpha \leq \beta$ (no. 1, Hệ quả 3 to Mệnh đề 2), $(\rho_\alpha)$ là một hệ trực tiếp các đồng cấu và $j = \lim \rightarrow \rho_\alpha$ là đồng cấu duy nhất từ $A'$ đến $S^{-1}A$ sao cho $j \circ \rho'_\alpha = \rho_\alpha$ với mọi $a \in I$. Các đồng cấu $\rho'_\alpha \circ i^{S}_{A^\alpha} : A \to A'$ đều bằng nhau, vì $\rho_{\beta \alpha} \circ i^{S}_{A^\alpha} = i^{S}_{A^\beta}$ với $a \leq \beta$; hãy gọi $u$ là giá trị chung của chúng. Rõ ràng các phần tử của $u(S)$ là khả nghịch trong $A'$, điều này cho thấy tồn tại một đồng cấu $h : S^{-1}A \to A'$ sao cho $h \circ i^{S}_{A} = u$ (no. 1, Mệnh đề 1). Khi đó

$$
j \circ h \circ i^{A}_{S} = j \circ u = j \circ \rho'_\alpha \circ i^{A^\alpha}_{S^\alpha} = \rho_\alpha \circ i^{S}_{A^\alpha} = i^{S}_{A}
$$

với mọi $\alpha \in I$ và do đó $j \circ h$ là tự đẳng cấu đồng nhất của $S^{-1}A$. Mặt khác, với mọi $\alpha \in I$,

$$
h \circ j \circ \rho'_\alpha \circ i^{S}_{A^\alpha} = h \circ \rho_\alpha \circ i^{S}_{A^\alpha} = h \circ i^{S}_{A} = u = \rho'_\alpha \circ i^{S}_{A^\alpha},
$$

suy ra $h \circ j \circ \rho'_\alpha = \rho'_\alpha$ với mọi $\alpha \in I$; do đó suy ra $h \circ j$ là tự đẳng cấu đồng nhất của $A'$ và do đó $j$ là một đẳng cấu.

#### Hệ quả {#ac-ii-s2-n3-cor-1 .statement}

*Dưới các giả thiết của Mệnh đề 9, cho M là một A-môđun. Ký hiệu $f_{\beta \alpha} = i^{S_\beta, S_\alpha}_{M}$ với $\alpha \leq \beta, f_\alpha = i^{S, S_\alpha}_{M}$ với mọi $\alpha \in I$ và cho $f'_\alpha$ là ánh xạ chính tắc từ $S_\alpha^{-1}M$ đến $\lim \rightarrow S_\alpha^{-1}M$; khi đó tồn tại một $S^{-1}A$-đẳng cấu $g$ của $S^{-1}M$ lên $\lim \rightarrow S_\alpha^{-1}M$ sao cho $g \circ f_\alpha = f'_\alpha$ với mọi $a \in I$.*

Hệ quả này suy ra ngay từ các định nghĩa $S_\alpha^{-1}M = M \otimes_A S_\alpha^{-1}A$ và $S^{-1}M = M \otimes_A S^{-1}A$ và sự kiện rằng việc lấy giới hạn trực tiếp giao hoán với các tích tenxơ (*Đại số*, Chương 11, § 6, no. 3, Mệnh đề 7).

### 4. CÁC TÍNH CHẤT CỦA CÁC MÔĐUN PHÂN THỨC

*Trong toàn bộ số này, A ký hiệu một vành và S một tập con nhân của A.*

Cho $(M_\alpha, \phi_{\beta \alpha})$ là một hệ trực tiếp các A-môđun; khi đó $(S^{-1}M_\alpha, S^{-1}\phi_{\beta \alpha})$ là một hệ trực tiếp các $S^{-1}A$-môđun và sự kiện rằng việc lấy giới hạn trực tiếp giao hoán với các tích tenxơ (_Đại số_, Chương II, § 6, no. 3, Mệnh đề 7) cho phép ta định nghĩa một đẳng cấu chính tắc

$$
\lim \rightarrow (S^{-1}M_\alpha) \to S^{-1} \lim \rightarrow M_\alpha.
$$

$$
\bigoplus_{i \in I} S^{-1} M_i \to S^{-1} \bigoplus_{i \in I} M_i.
$$

Cuối cùng, ta lưu ý rằng, nếu một $A$-môđun $M$ là tổng của một họ $(N_i)_{i \in I}$ các môđun con, thì $S^{-1}M$ là tổng của họ các $S^{-1}A$-môđun con sinh bởi các $i_M^S(N_i)$. Do đó, nếu $M$ là một $A$-môđun sinh hữu hạn (tương ứng, một $A$-môđun trình bày hữu hạn), thì $S^{-1}M = S^{-1}A \otimes_A M$ là một $S^{-1}A$-môđun sinh hữu hạn (tương ứng, một $S^{-1}A$-môđun trình bày hữu hạn).

#### Định lý 1 {#ac-ii-s2-thm-1 .statement}

*Vành $S^{-1}A$ là một $A$-môđun phẳng* (Chương I, § 2, No. 1, Định nghĩa 2).

Nếu $u : M' \to M$ là một đơn cấu của các $A$-môđun, cần chứng minh rằng $S^{-1}u : S^{-1}M' \to S^{-1}M$ là đơn ánh. Bây giờ, nếu $m'/s$ ($m' \in M'$, $s \in S$) sao cho $u(m')/s = 0$, thì điều này kéo theo sự tồn tại của một $s' \in S$ sao cho $s'u(m') = 0$ (No. 2, Mệnh đề 4) hay $u(s'm') = 0$; vì $u$ là đơn ánh, do đó $s'm' = 0$, suy ra $m'/s = 0$.

Việc $S^{-1}A$ là một $A$-môđun phẳng cho phép ta áp dụng cho nó các kết quả của Chương I, § 2. Đặc biệt:
(1) Nếu $M$ là một $A$-môđun và $N$ là một môđun con của $M$, thì $S^{-1}N$ được đồng nhất một cách chính tắc với một *môđun con* của $S^{-1}M$ sinh bởi $i_M^S(N)$ (Chương I. § 2, No. 3, *Nhận xét 2*); với sự đồng nhất này, $S^{-1}(M/N)$ được đồng nhất với $(S^{-1}M)/(S^{-1}N)$ và, nếu $P$ là một môđun con thứ hai của $M$, thì

$$
S^{-1}(N + P) = S^{-1}N + S^{-1}P, \quad S^{-1}(N \cap P) = S^{-1}N \cap S^{-1}P
$$

(Chương I, § 2, No. 6, Mệnh đề 2).
(2) Nếu $M$ là một $A$-môđun *sinh hữu hạn*, thì

$$
S^{-1} \operatorname{Ann}(M) = \operatorname{Ann}(S^{-1}M)
$$

(Chương I, § 2, No. 10, Hệ quả 2 của Mệnh đề 12).

#### Mệnh đề 10 {#ac-ii-s2-prop-10 .statement}

*Cho $M$ là một $A$-môđun. Với mỗi môđun con $N'$ của $S^{-1}A$-môđun $S^{-1}M$, gọi $\phi(N')$ là ảnh ngược của $N'$ qua $i_M^S$. Khi đó:*
(i) $S\phi(N') = N'$.

(ii) Với mỗi môđun con $N$ của $M$, môđun con $\phi(S^{-1}N)$ của $M$ gồm những $m \in M$ sao cho tồn tại $s \in S$ thỏa mãn $sm \in N$.

(iii) $\phi$ là một đẳng cấu (đối với các thứ tự được xác định bởi quan hệ bao hàm) từ tập hợp các môđun con $S^{-1}A$ của $S^{-1}M$ lên tập hợp các môđun con $Q$ của $M$ thỏa mãn điều kiện sau:

(MS) Nếu $sm \in Q$, trong đó $s \in S$, $m \in M$, thì $m \in Q$.

Hiển nhiên $S^{-1}\phi(N') \subset N'$; ngược lại, nếu $n' = m/s \in N'$, thì $m/1 \in N'$, do đó $m \in \phi(N')$ và do đó $n' \in S^{-1}(\phi(N'))$; do đó (i). Để một phần tử $m \in M$ thỏa mãn $m \in \phi(S^{-1}N)$, điều kiện cần và đủ là $m/1 \in S^{-1}N$, nghĩa là tồn tại $s \in S$ và $n \in N$ sao cho $m/1 = n/s$; điều này có nghĩa là tồn tại $s' \in S$ sao cho $s'sm = sn \in N$, do đó (ii). Cuối cùng, quan hệ $sm \in \phi(N')$ tương đương theo định nghĩa với $sm/1 \in N'$ và vì $s/1$ khả nghịch trong $S^{-1}A$, điều này kéo theo $m/1 \in N'$, hay $m \in \phi(N')$, do đó $\phi(N')$ thỏa mãn điều kiện (MS); mặt khác, từ (ii) suy ra rằng, nếu $N$ thỏa mãn (MS), thì $\phi(S^{-1}N) = N$, điều này hoàn tất chứng minh (iii).

Môđun con $\phi(S^{-1}N)$ được gọi là môđun bão hòa của $N$ trong $M$ đối với $S$, và các môđun con thỏa mãn điều kiện (MS) (và do đó bằng môđun bão hòa của chúng) được gọi là bão hòa đối với $S$. Môđun con $\phi(S^{-1}N)$ là hạt nhân của đồng cấu hợp thành

$$
M \xrightarrow{h} M/N \xrightarrow{i_{M/N}^{S}} S^{-1}M/S^{-1}N
$$

trong đó $h$ là đồng cấu chính tắc, như suy ra từ tính giao hoán của biểu đồ

$$
\begin{array}{ccc}
M & \xrightarrow{h} & M/N \\
i_M^S \downarrow & & i_{M/N}^S \downarrow \\
S^{-1}M & \xrightarrow{s^{-1}h} & S^{-1}M/S^{-1}N
\end{array}
$$

Nếu $S$ là phần bù trong $A$ của một iđêan nguyên tố $p$, $\phi(S^{-1}N)$ cũng được gọi là môđun bão hòa của $N$ trong $M$ đối với $p$.

#### Hệ quả 1 {#ac-ii-s2-prop-10-cor-1 .statement}

Cho $N_1, N_2$ là hai môđun con của một $A$-môđun $M$. Để $S^{-1}N_1 \subset S^{-1}N_2$, điều kiện cần và đủ là môđun bão hòa của $N_1$ đối với $S$ được chứa trong môđun bão hòa của $N_2$.

#### Hệ quả 2 {#ac-ii-s2-prop-10-cor-2 .statement}

*Nếu M là một môđun* Noether *A* (tương ứng, Artin), *S^{-1}M* là một môđun Noether (tương ứng, Artin) trên *S^{-1}A*. *Đặc biệt, nếu vành A là Noether* (tương ứng, Artin), *thì vành S^{-1}A cũng vậy*.

### 5. IĐÊAN TRONG MỘT VÀNH PHÂN THỨC

#### Mệnh đề 11 {#ac-ii-s2-prop-11 .statement}

*Cho A là một vành và S là một tập con nhân của A. Với mọi iđêan b' của S^{-1}A, đặt b = (i_A^S)^{-1}(b') sao cho b' = S^{-1}b.*

(i) *Cho f là đồng cấu chính tắc A \to A/b. Đồng cấu từ S^{-1}A vào (f(S))^{-1}(A/b) liên kết một cách chính tắc với f (no. 1, Mệnh đề 2) là toàn ánh và hạt nhân của nó là b', do đó xác định, bằng cách lấy thương, một đẳng cấu chính tắc của (S^{-1}A)/b' lên (f(S))^{-1}(A/b). Hơn nữa, đồng cấu chính tắc từ A/b vào (f(S))^{-1}(A/b) là đơn ánh.*

(ii) *Ánh xạ b' \mapsto b = (i_M^S)^{-1}(b'), hạn chế trên tập hợp các iđêan cực đại (tương ứng, nguyên tố) của S^{-1}A, là một đẳng cấu (đối với quan hệ bao hàm) của tập hợp này lên tập hợp các iđêan của A cực đại trong số những iđêan không giao với S (tương ứng, tập hợp các iđêan nguyên tố của A không giao với S).*

(iii) *Nếu q' là một iđêan nguyên tố của S^{-1}A và q = (i_A^S)^{-1}(q'), thì tồn tại một đẳng cấu của vành phân thức A, lên vành (S^{-1}A)_{q'}, biến a/b thành (a/1)/(b/1), trong đó a \in A, b \in A - q.*

(i) *(f(S))^{-1}(A/b) có thể được đồng nhất với S^{-1}(A/b) nhờ đẳng cấu chính tắc giữa hai môđun này (no. 2, Mệnh đề 6). Khi đó dãy khớp 0 \to b \to A \to A/b \to 0 cảm sinh một dãy khớp*

$$
0 \to S^{-1}b \to S^{-1}A \to S^{-1}(A/b) \to 0
$$

*(no. 4, Định lý 1), sự tồn tại của dãy này chứng minh mệnh đề đầu tiên của (i), có tính đến sự kiện b' = S^{-1}b. Vì b là bão hòa đối với S, các điều kiện a \in A, s \in S, as \in b kéo theo a \in b; phép vị tự có tỉ số s trên A/b khi đó là đơn ánh, điều này chứng minh mệnh đề thứ hai của (i).*

(ii) Trước hết, ta lưu ý rằng quan hệ b' = S^{-1}A tương đương với quan hệ b \cap S \neq \varnothing, quan hệ sau biểu thị rằng b' chứa các phần tử khả nghịch của S^{-1}A. Theo no. 4, Mệnh đề 10 (iii), suy ra rằng b' \mapsto b = (i_A^S)^{-1}(b') là một đẳng cấu (đối với quan hệ bao hàm) từ tập hợp các iđêan của S^{-1}A phân biệt với S^{-1}A lên tập hợp \mathcal{F} các iđêan của A không gặp S và thỏa mãn điều kiện (MS) của Mệnh đề 10. Nếu b' là cực đại (resp. nguyên tố), thì hiển nhiên b' là cực đại trong \mathcal{F} (resp. nguyên tố) và ngược lại (theo (i)). Mặt khác, nếu r là một iđêan của A rời nhau với S, phần bão hòa r_1 của nó đối với S là một iđêan của A chứa t và rời nhau với S: không có phần tử $a \in S$ nào có thể thỏa mãn $sa \in t$ với một $s \in S$ nào đó, vì khi đó sẽ suy ra $sa \in t \cap S$. Ta kết luận rằng, nếu r là cực đại trong các iđêan của $A$ gặp S, thì nó là cực đại trong \mathcal{F}. Tương tự, nếu r là một iđêan nguyên tố không gặp S, thì theo định nghĩa của các iđêan nguyên tố, nó thỏa mãn điều kiện (MS) của no. 4, Mệnh đề 10 và do đó thuộc \mathcal{F}. Điều này hoàn tất chứng minh (ii).

(iii) Giả sử rằng $q'$ là nguyên tố và $q$ cũng là nguyên tố. Tập hợp $T = A - q$ là một tập con nhân của A chứa S, do đó $ST = T$. Ta viết $T' = i_A^S(T)$; theo no. 3, Mệnh đề 7 (i), tồn tại duy nhất một đẳng cấu $j$ từ $T^{-1}A = A$ lên ${T'}^{-1}(S^{-1}A)$ sao cho

$$
j(a/b) = (a/1)/(b/1),
$$

trong đó $a \in A$ và $b \in T$. Mặt khác, $T'$ hiển nhiên không gặp $q'$; ngược lại, cho $a/s \in S^{-1}A$; vì $1/s$ khả nghịch trong $S^{-1}A$, điều kiện $a/s \notin q'$ tương đương với $i_A^S(a) = a/1 \notin q'$ và do đó tương đương với $a \notin q$; suy ra $S^{-1}A - q' = S^{-1}T'$ và do đó, theo Mệnh đề 8 của no. 3, ${T'}^{-1}(S^{-1}A) = (S^{-1}A)_{q'}$.

Đẳng cấu được xác định trong (iii) được gọi là chính tắc. Nếu $A$ là một miền nguyên, các đẳng cấu chính tắc của $A$, và $(S^{-1}A)_{q'}$ lên các vành con của trường phân thức $K$ của $A$ có cùng ảnh.

#### Nhận xét {#ac-ii-s2-n5-rem-1 .statement}

Đối với một iđêan $a$ của $A$, để thỏa mãn $S^{-1}a = S^{-1}A$ (hay, điều này tương đương với cùng một điều theo no. 4, Định lý I, $S^{-1}(A/a) = 0$), điều kiện cần và đủ là $a \cap S \neq \varnothing$, như suy ra ngay lập tức từ các định nghĩa.

#### Hệ quả 1 {#ac-ii-s2-prop-11-cor-1 .statement}

Cho $A$ là một vành và $S$ là một tập con nhân của $A$. Mọi iđêan $p$ của $A$ cực đại trong số các iđêan không gặp S đều là nguyên tố.

Theo Mệnh đề 11, giả thiết trên $p$ có nghĩa là $p = (i_A^S)^{-1}(m')$, trong đó $m'$ là một iđêan cực đại của $S^{-1}A$; vì $m'$ là nguyên tố, nên p cũng vậy.

#### Hệ quả 2 {#ac-ii-s2-prop-11-cor-2 .statement}

Cho $A$ là một vành và $S$ là một tập con nhân của $A$. Với mọi iđêan $a$ của $A$ không giao với $S$, tồn tại một iđêan nguyên tố chứa $a$ và không giao với $S$.

$S^{-1}a \neq S^{-1}A$ (Nhận xét) và do đó tồn tại một iđêan cực đại của $S^{-1}A$ chứa $S^{-1}a$ (Đại số, Chương I, § 8, no. 7, Định lý 2) và hệ quả suy ra từ Mệnh đề 11 (ii).

#### Hệ quả 3 {#ac-ii-s2-prop-11-cor-3 .statement}

Cho $A, B$ là hai vành, $\rho$ là một đồng cấu từ $A$ đến $B$ và $p$ là một iđêan nguyên tố của $A$. Để tồn tại một iđêan nguyên tố $p'$ của $B$ sao cho $\overline{\rho}^{-1}(p') = p$, điều kiện cần và đủ là $\overline{\rho}^{-1}(B\rho(p)) = p$.

Nếu tồn tại một iđêan $p'$ của $B$ sao cho $\bar{\rho}^{-1}(p') = p$, thì $\rho(p) \subset p'$, do đó $B_{\rho}(p) \subset p'$ và $\bar{\rho}^{-1}(B_{\rho}(p)) \subset \bar{\rho}^{-1}(p') \subset p$; vì bao hàm đảo lại là hiển nhiên, $\bar{\sigma}^{-1}(B_{\rho}(p)) = p$. Đảo lại, giả sử rằng $\bar{\rho}^{-1}(B_{\rho}(p)) = p$ và xét tập con nhân $S = \rho(A - p)$ của $B$; giả thiết chỉ ra rằng
$$
S \cap B_{\rho}(p) = \varnothing;
$$
theo Hệ quả 2 tồn tại một iđêan nguyên tố $p'$ của $B$ chứa $B_{\rho}(p)$ và không giao với $S$; khi đó $\bar{\rho}^{-1}(p')$ chứa $p$ và không thể chứa bất kỳ phần tử nào của $A - p$ và do đó bằng $p$.

#### Hệ quả 4 {#ac-ii-s2-prop-11-cor-4 .statement}

*Mệnh đề $A, B$ là hai vành và $\rho$ là một đồng cấu từ $A$ vào $B$.
(i) Giả sử tồn tại một $B$-môđun $E$ sao cho $\rho_*(E)$ là một môđun $A$ phẳng trung thành. Khi đó, với mọi iđêan nguyên tố $p$ của $A$, tồn tại một iđêan nguyên tố $p'$ của $B$ sao cho $\bar{\rho}^{-1}(p') = p$.
(ii) Ngược lại, giả sử $B$ là một môđun $A$ phẳng. Khi đó, nếu với mọi iđêan nguyên tố $p$ của $A$, tồn tại một iđêan $p'$ của $B$ sao cho $\bar{\rho}^{-1}(p') = p$, thì $B$ là một môđun $A$ phẳng trung thành.*

(i) Giả thiết suy ra rằng, với mọi iđêan $a$ của $A$, $\bar{\rho}^{-1}(B_{\rho}(a)) = a$ (chương I, § 3, no. 5, Mệnh đề 8 (ii)) và chỉ cần áp dụng Hệ quả 3.
(ii) Chỉ cần chứng minh rằng, với mọi iđêan cực đại $m$ của $A$, tồn tại một iđêan cực đại $m'$ của $B$ sao cho $\bar{\rho}^{-1}(m') = m$ (chương I, § 2, no. 5, Mệnh đề 9 (e)). Theo giả thiết, tồn tại một iđêan $q$ của $B$ sao cho $\bar{\rho}^{-1}(q) = m$; vì $q \neq B$, tồn tại một iđêan cực đại $m'$ của $B$ chứa $q$ và do đó $\bar{\rho}^{-1}(m') \supseteq m$; nhưng vì $\bar{\rho}^{-1}(m')$ không thể chứa 1, nên $\bar{\rho}^{-1}(m') = m$.

#### Hệ quả 5 {#ac-ii-s2-prop-11-cor-5 .statement}

*Mệnh đề $A$ là một vành, $S$ là một tập con nhân của $A$ và $B$ là một vành sao cho $i_A^S(A) \subset B \subset S^{-1}A$. Cho $q$ là một iđêan nguyên tố của $B$ sao cho iđêan nguyên tố $p = (i_A^S)^{-1}(q)$ của $A$ không giao với $S$ và cho $p'$ là iđêan nguyên tố $S^{-1}p$ của $S^{-1}A$. Khi đó $p' \cap B = q$.*

Cho $S' = i_A^S(S)$; một đẳng cấu chính tắc đã được xác định từ ${S'}^{-1}B$ đến $S^{-1}A$ (no. 1, Hệ quả 4 của Mệnh đề 2); ta đồng nhất hai vành này bằng đẳng cấu này. Vì $q \cap S' = \varnothing$, $q' = {S'}^{-1}q$ là iđêan nguyên tố duy nhất của $S^{-1}A = {S'}^{-1}B$ sao cho $q' \cap B = (i_A^S)^{-1}(q') = q$ (Mệnh đề 11 (ii)), do đó $(i_A^S)^{-1}(q') = p$; do đó $q' = p'$ (Mệnh đề 11 (ii)).

Theo ký hiệu của Hệ quả 5, có các đẳng cấu chính tắc của $A$, và $B_q$ lên $(S^{-1}A)_q$. (Mệnh đề 11 (iii)) và do đó một *đẳng cấu chính tắc* $A, \to B_q$.

### 6. CĂN LŨY LINH VÀ CÁC IĐÊAN NGUYÊN TỐ CỰC TIỂU

Trong một vành (giao hoán) $A$ tập hợp các phần tử lũy linh là một *iđêan*, vì nếu $x, y$ là các phần tử của $A$ sao cho $x^m = y^n = 0$, thì $(x + y)^{m+n} = 0$ theo định lý nhị thức.

#### Định nghĩa 4 {#ac-ii-s2-def-4 .statement}

*Iđêan các phần tử lũy linh của một vành (giao hoán) $A$ được gọi là căn lũy linh của $A$. Nếu $a$ là một iđêan của $A$, ảnh ngược, qua ánh xạ chính tắc $A \to A/a$, của căn lũy linh của $A/a$ được gọi là căn của $a$.*

Ta thường ký hiệu $r(a)$ căn của một iđêan $a$ của $A$.

Nói rằng một phần tử $x \in A$ thuộc căn của $a$ có nghĩa là do đó tồn tại một số nguyên $n > 0$ sao cho $x^n \in a$. Nếu f là một đồng cấu từ $A$ đến một vành $B$ và $b$ là một iđêan của $B$, căn của f $^{-1} (b)$ là *ảnh ngược* qua f của căn của $b$, vì nói rằng $x^n \in f^{-1} (b)$ có nghĩa là $(f(x))^n \in b$.

Căn lũy linh của một vành $A$ được chứa trong căn Jacobson của nó (*Đại số*, Chương VIII, § 6, no. 3, Hệ quả 3 của Định lý 1) nhưng có thể phân biệt với nó; nó luôn bằng nó nếu $A$ là *Artin* (*Đại số*, Chương VIII, § 6, no. 4, Định lý 3).

Ta nói rằng một iđêan nguyên tố $p$ của một vành $A$ là một *iđêan nguyên tố cực tiểu* nếu nó là cực tiểu trong tập hợp các iđêan nguyên tố của $A$ có thứ tự bởi quan hệ chứa.

#### Mệnh đề 12 {#ac-ii-s2-prop-12 .statement}

*Cho $p$ là một iđêan nguyên tố cực tiểu của một vành $A$. Với mọi $x \in p$, tồn tại $s \in A - p$ và một số nguyên $k > 0$ sao cho $sx^k = 0$.*

Tập hợp $S$ gồm các phần tử có dạng $sx^k$ ($k$ là một số nguyên $> 0$, $s \in A - p$) là một tập con nhân của $A$. Nếu $0 \notin S$, sẽ tồn tại một iđêan nguyên tố $p'$ không gặp $S$ (no. 5, Hệ quả 2 của Mệnh đề 11). Khi đó $p' = p$ và $p' \# p$ vì $x \notin p'$, trái với giả thiết rằng $p$ là cực tiểu.

#### Mệnh đề 13 {#ac-ii-s2-prop-13 .statement}

*Căn lũy linh của một vành $A$ là giao của tất cả các iđêan nguyên tố của $A$ và cũng là giao của các iđêan nguyên tố cực tiểu của $A$.*

Rõ ràng, nếu $x \in A$ là lũy linh, thì nó được chứa trong mọi iđêan nguyên tố của $A$ (§ 1, no. 1, Định nghĩa 1). Ngược lại, cho $x$ là một phần tử không lũy linh của $A$; tập hợp $S$ gồm các $x^k$ ($k$ là một số nguyên $\geqslant 0$) khi đó là một tập con nhân của $A$ không chứa 0 và do đó tồn tại một iđêan nguyên tố $p$ của $A$ không gặp $S$ (no. 5, Hệ quả 2 của Mệnh đề 11) và *a fortiori* $x \notin p$; điều này thiết lập mệnh đề thứ nhất. Để chứng minh mệnh đề thứ hai, chỉ cần chứng minh

#### Bổ đề 2 {#ac-ii-s2-lem-2 .statement}

*Mọi iđêan nguyên tố của một vành $A$ đều chứa một iđêan nguyên tố cực tiểu của $A$.*

Theo Bổ đề Zorn, chỉ cần chỉ ra rằng tập hợp P các iđêan nguyên tố, được sắp thứ tự bởi quan hệ $\supseteq$, là *quy nạp*. Bây giờ, nếu $G$ là một tập con sắp thứ tự toàn phần không rỗng của P, giao $p_0$ của các iđêan $p \in G$ cũng là một iđêan nguyên tố: thật vậy, nếu $x \notin p_0$ và $y \notin p_0$, tồn tại một iđêan $p \in G$ sao cho $x \notin p$ và $y \notin p$, do đó $xy \notin p$ và *a fortiori* $xy \notin p_0$.

#### Nhận xét {#ac-ii-s2-n6-rem-1 .statement}

Trong § 4, no. 3, Hệ quả 3 của Mệnh đề 14, ta sẽ chỉ ra rằng trong một vành *Noether* tập hợp các iđêan nguyên tố cực tiểu là *hữu hạn*; hơn nữa ta sẽ thấy sau này rằng mọi dãy giảm các iđêan nguyên tố trong một vành Noether đều *dừng*.

#### Hệ quả 1 {#ac-ii-s2-lem-2-cor-1 .statement}

*Căn của một iđêan* $a$ *trong một vành* $A$ *là giao của các iđêan nguyên tố chứa* $a$ *và cũng là giao của các phần tử cực tiểu của tập hợp các iđêan nguyên tố này.*

#### Hệ quả 2 {#ac-ii-s2-lem-2-cor-2 .statement}

*Đối với một iđêan* $a$ *của một vành* $A$ *ta ký hiệu bởi* $r(a)$ *căn của* $a$. *Khi đó, đối với hai iđêan* $a, b$ *của* $A$,
$$
r(a \cap b) = r(ab) = r(a) \cap r(b);
$$
*đặc biệt, nếu* $a \subset b$, *thì* $r(a) \subset r(b)$.

Đối với một iđêan nguyên tố chứa $a \cap b$ (hoặc $ab$), điều kiện cần và đủ là nó chứa một trong các iđêan $a, b$ (§ 1, no. 1, Mệnh đề 1).

#### Mệnh đề 14 {#ac-ii-s2-prop-14 .statement}

*Đối với hai iđêan* $a, b$ *của một vành, để chúng nguyên tố cùng nhau, điều kiện cần và đủ là các căn* $r(a)$ *và* $r(b)$ *của chúng cũng như vậy*.

Tính cần thiết của điều kiện là hiển nhiên vì $a \subset r(a)$ và $b \subset r(b)$; điều kiện là đủ theo § 1, no. 2, Mệnh đề 3.

#### Mệnh đề 15 {#ac-ii-s2-prop-15 .statement}

*Trong một vành* $A$ *cho* $a$ *là một iđêan và* $b$ *là một iđêan sinh hữu hạn được chứa trong căn của* $a$. *Khi đó tồn tại một số nguyên* $k > 0$ *sao cho* $b^k \subset a$.

Cho $(b_i)_{1 \leq i \leq n}$ là một hệ sinh của $b$. Theo giả thiết, tồn tại một số nguyên $h$ sao cho $b_i^h \in a$ với $1 \leq i \leq n$. Nếu khai triển một tích của $nh$ phần tử, mà mỗi phần tử là một tổ hợp tuyến tính của các $b_i$ với hệ số trong $A$, thì mỗi số hạng là một bội của một tích gồm $nh$ thừa số, mỗi thừa số bằng một $b_i$; trong các thừa số ấy, có ít nhất $h$ thừa số có cùng chỉ số $i$ đối với một $i$ nào đó; do đó tích thuộc $a$ và $nh$ là số nguyên $k$ cần tìm.

#### Hệ quả {#ac-ii-s2-n6-cor-1 .statement}

*Trong một vành Noether, căn lũy linh là một iđêan lũy linh*.

#### Mệnh đề 16 {#ac-ii-s2-prop-16 .statement}

*Cho* $B$ *là một vành và* $A$ *là một vành con của* $B$. *Với mọi iđêan nguyên tố cực tiểu* $p$ *của* $A$ *tồn tại một iđêan nguyên tố cực tiểu* $q$ *của* $B$ *sao cho* $q \cap A = p$.

Đặt $S = A - p$; khi đó vành $A_+ = S^{-1}A$ được đồng nhất với một vành con của $S^{-1}B$ (no. 1, Mệnh đề 2) và mặt khác $A_+$ chỉ có một iđêan nguyên tố duy nhất $p'$ vì $p$ là cực tiểu (no. 5, Mệnh đề 11). Vì $S^{-1}B$ không bằng 0 (do nó chứa $A_+$), nó có ít nhất một iđêan nguyên tố $r'$ và do đó $r' \cap A_+ = p'$; nếu $j = i_B^S$ và đặt $r = j'(t')$, thì
$$
i_A^S(r \cap A) \subset r' \cap A_+ = p'
$$
do đó $r \cap A \subset p$ và, vì $p$ là cực tiểu, $t \cap A = p$; hơn nữa, $r$ là nguyên tố trong $B$; nếu $q$ là một iđêan nguyên tố cực tiểu của $B$ được chứa trong $r$ (Bổ đề 1), thì a fortiori $q \cap A = p$ vì $p$ là cực tiểu.

#### Định nghĩa 5 {#ac-ii-s2-def-5 .statement}

Một vành $A$ được gọi là rút gọn nếu căn lũy linh của nó bằng 0, nói cách khác nếu không có phần tử nào $\neq 0$ của $A$ là lũy linh.

Nếu $\mathfrak{N}$ là căn lũy linh của một vành $A$, thì $A/\mathfrak{N}$ là vành khử, vì nếu lớp mod. $\mathfrak{N}$ của một phần tử $x \in A$ là lũy linh trong $A/\mathfrak{N}$, điều này có nghĩa là $x^h \in \mathfrak{N}$ với một số số nguyên $h$, do đó $x^{hk} = 0$ với một số số nguyên $k$ và $x \in \mathfrak{N}$.

#### Mệnh đề 17 {#ac-ii-s2-prop-17 .statement}

Cho $A$ là một vành và $\mathfrak{N}$ là căn lũy linh của nó. Với mọi tập con nhân $S$ của $A$, $S^{-1}\mathfrak{N}$ là căn lũy linh của $S^{-1}A$. Đặc biệt, nếu $A$ là vành khử, thì $S^{-1}A$ là vành khử.

Nếu $x \in A$, $s \in S$ thỏa mãn $(x/s)^n = x^n/s^n = 0$, thì tồn tại $s' \in S$ sao cho $s'x^n = 0$ (no. 1, Nhận xét 3) và a fortiori $(s'x)^n = 0$, do đó $s'x \in \mathfrak{N}$ và $x/s = s'x/s's \in S^{-1}\mathfrak{N}$; đảo lại là ngay lập tức.

### 7. PHÂN THỨC CỦA CÁC TÍCH TENXƠ VÀ CÁC MÔĐUN ĐỒNG CẤU

#### Mệnh đề 18 {#ac-ii-s2-prop-18 .statement}

Cho $A$ là một vành và $S$ là một tập con nhân của $A$.

(i) Nếu $M$ và $N$ là hai $A$-môđun, thì các $S^{-1}A$-môđun $(S^{-1}M) \otimes_A N, M \otimes_A (S^{-1}N)$, $(S^{-1}M) \otimes_{S^{-1}A} (S^{-1}N)$ và $S^{-1}(M \otimes_A N)$ là đẳng cấu chính tắc.

(ii) Nếu $M$ và $N'$ là hai $S^{-1}A$-môđun, thì đồng cấu chính tắc
$$
M' \otimes_A N' \to M' \otimes_{S^{-1}A} N'
$$
dẫn xuất từ ánh xạ $A$-song tuyến tính $(x', y') \mapsto x' \otimes y'$ từ $M' \times N'$ vào $M' \otimes_{S^{-1}A} N'$
là song ánh.

Mệnh đề (i) là một hệ quả ngay lập tức của định nghĩa $S^{-1}M =$

$M \otimes_A S^{-1}A$ và tính kết hợp của các tích tenxơ, cho đến các đẳng cấu chính tắc, cho

$$
(S^{-1}M \otimes_{S^{-1}A} (S^{-1}N)) = (S^{-1}M) \otimes_{S^{-1}A} (S^{-1}A \otimes N) = (S^{-1}M) \otimes_A N \\
= (S^{-1}A) \otimes_A M \otimes_A N = S^{-1}(M \otimes_A N).
$$

Để chứng minh (ii), trước hết ta nhận thấy rằng trong $M'$ và $N'$, được xem như các $A$-môđun, các phép đồng nhất tâm cảm sinh bởi các phần tử $s \in S$ là song ánh, do đó $M' = S^{-1}M'$ và $N' = S^{-1}N'$ (no. 2, Nhận xét 4) và tương tự $S^{-1}(M' \otimes_A N') = M' \otimes_A N'$; (ii) khi đó là một trường hợp riêng của (i).

#### Hệ quả {#ac-ii-s2-n7-cor-1 .statement}

Cho $M$ là một $A$-môđun và $a$ là một iđêan của $A$. Các $S^{-1}A$-môđun con $(S^{-1}a)(S^{-1}M)$, $a(S^{-1}M)$, $(S^{-1}a)j(M)$ (trong đó $j : M \to S^{-1}M$ là ánh xạ chính tắc) và $S^{-1}(aM)$ của $S^{-1}M$ là đồng nhất. Đặc biệt, nếu $a$ và $b$ là hai iđêan của $A$, thì

$$
(S^{-1}a)(S^{-1}b) = a(S^{-1}b) = (S^{-1}a)b = S^{-1}(ab).
$$

#### Nhận xét {#ac-ii-s2-n7-rem-1 .statement}

Cho $M, N, P$ là ba $A$-môđun, $f : M \times N \to P$ là một ánh xạ $A$-song tuyến tính và $S^{-1}f : (S^{-1}M) \times (S^{-1}N) \to (S^{-1}P)$ là ánh xạ $S^{-1}A$-song tuyến tính nhận được từ $f$ bằng cách mở rộng vành vô hướng tới $S^{-1}A$ (Đại số, Chương IX, § 1, no. 4, Mệnh đề 1). Cho $i : M \to S^{-1}M, j : N \to S^{-1}N$ là các đồng cấu chính tắc; suy ra ngay lập tức rằng, nếu $Q$ là $A$-môđun con của $P$ sinh bởi $f(M \times N)$, thì $S^{-1}Q$ là $S^{-1}A$-môđun con của $S^{-1}P$ sinh bởi $(S^{-1}f)(i(M) \times j(N))$.

#### Mệnh đề 19 {#ac-ii-s2-prop-19 .statement}

Cho $A$ là một vành và $S$ là một tập con nhân của $A$.
(i) Nếu $M$ và $N$ là hai $A$-môđun và $M$ là sinh hữu hạn (tương ứng, trình bày hữu hạn), thì đồng cấu chính tắc (Chương I, §2, no. 10, công thức (10))

$$
S^{-1}\operatorname{Hom}_A(M, N) \to \operatorname{Hom}_{S^{-1}A}(S^{-1}M, S^{-1}N)
$$

là đơn ánh (tương ứng, song ánh).
(ii) Nếu $M', N'$ là hai $S^{-1}A$-môđun, thì song ánh chính tắc

$$
\operatorname{Hom}_{S^{-1}A}(M', N') \to \operatorname{Hom}_A(M', N')
$$

là song ánh.

Vì $S^{-1}A$ là một $A$-môđun phẳng, (i) là một trường hợp riêng của Chương I, §2, no. 10, Mệnh đề 11. Mặt khác, ta đã nhận xét rằng mọi $A$-đồng cấu của các $S^{-1}A$-môđun nhất thiết là một $S^{-1}A$-đồng cấu, trong quá trình chứng minh Mệnh đề 3 của no. 2; do đó (ii).

#### Mệnh đề 20 {#ac-ii-s2-prop-20 .statement}

Cho $A, A'$ là hai vành, $p : A \to A'$ là một đồng cấu, $S$ là một tập con nhân của $A$, $S' = \rho(S)$ và $\rho' : S^{-1}A \to {S'}^{-1}A'$ là đồng cấu tương ứng với $p$ (no. 1, Mệnh đề 2).

(i) *Với mọi* $A'$-môđun $M'$ tồn tại một đẳng cấu $S^{-1}A$-duy nhất
$$
j : S^{-1}\rho_*(M') \to \rho'_*({S'}^{-1}M')
$$
*thỏa mãn* $j(m'/s) = m'/\rho(s)$ *với mọi* $m' \in M', s \in S$.

(ii) *Với mọi* $A$-môđun $M$, tồn tại một đẳng cấu duy nhất
$$
j' : (S^{-1}M) \otimes_{S^{-1}A} ({S'}^{-1}A') \to {S'}^{-1}(M \otimes_A A')
$$
*giữa các* ${S'}^{-1}A'$*-môđun* *thỏa mãn* $j'((m/s) \otimes (a'/s')) = (m \otimes a')/(\rho(s)s')$.

(i) Nếu ta xem ${S'}^{-1}M'$ như một $A$-môđun thông qua đồng cấu hợp thành $i^{S'}_{M'} \circ p$, các phép vị tự cảm sinh bởi các phần tử của $S$ đều song ánh, do đó tồn tại một đồng cấu $j$ duy nhất thỏa mãn tính chất đã nêu (No. 2, Mệnh đề 3). Vì $\rho(S) = S'$, $j$ là toàn ánh; hơn nữa, nếu $m' \in M'$, $s \in S$, $m'/\rho(s) = 0$, thì tồn tại $t' \in S'$ sao cho $t'm' = 0$; vì tồn tại $t \in S$ sao cho $\rho(t) = t', t'.m' = 0$ trong $\rho_*(M')$, suy ra $m'/s = 0$ trong $S^{-1}\rho_*(M')$.

(ii) Vì $(S^{-1}M) \otimes_{S^{-1}A} ({S'}^{-1}A') = (M \otimes_A S^{-1}A) \otimes_{S^{-1}A} ({S'}^{-1}A')$ và
$$
{S'}^{-1}(M \otimes_A A') = (M \otimes_A A') \otimes_{A'} ({S'}^{-1}A'),
$$
sự tồn tại của $j'$ suy ra từ tính kết hợp của các tích tenxơ.

### 8. ÁP DỤNG VÀO CÁC ĐẠI SỐ

Cho $A$ là một vành, $B$ là một $A$-đại số (không nhất thiết kết hợp hoặc giao hoán và không nhất thiết có phần tử đơn vị) và $S$ là một tập con nhân của $A$. Ta biết rằng có thể định nghĩa trên $S^{-1}A$-môđun $S^{-1}B = B \otimes_A S^{-1}A$ một cấu trúc $S^{-1}A$-*đại số* chính tắc, được gọi là thu được bằng mở rộng vành vô hướng đến $S^{-1}A$ (Đại số, chương III, § 3), và theo cấu trúc đó tích $(x/s)(y/t)$ bằng $(xy)/(st)$. Nếu $e$ là phần tử đơn vị của $B$, $e/1$ là phần tử đơn vị của $S^{-1}B$ và nếu $B$ kết hợp (tương ứng, giao hoán), *thì* $S^{-1}B$ cũng vậy.

Cho $A$ là một vành và $M$ là một $A$-môđun; ta ký hiệu $T(M)$ (tương ứng $\Lambda(M)$, $S(M)$) là đại số *tenxơ* (tương ứng đại số ngoài, đại số đối xứng) của $M$ (Đại số, Chương 111). Ta biết rằng với mọi đại số $A$-giao hoán $C$ tồn tại một đẳng cấu duy nhất $j$ từ $T(M) \otimes_A C$ lên $T(M \otimes_A C)$ (tương ứng từ $\Lambda(M) \oplus_A C$ lên $\Lambda(M \otimes_A C)$, từ $S(M) \otimes_A C$ lên $S(M \otimes_A C)$) sao cho $$
i(x \otimes 1) = x \otimes 1
$$ với mọi $x \in M$, trong đó $M$ được đồng nhất một cách chính tắc với một môđun con của $T(M)$ (tương ứng $\Lambda(M), S(M)$) (*loc. cit.*). Khi đó, đặc biệt, ta thấy rằng với mọi tập con nhân $R$ của $A$ có các *đẳng cấu chính tắc* $$
R^{-1}T(M) \to T(R^{-1}M), \qquad R^{-1}\Lambda(M) \to \Lambda(R^{-1}M), \qquad R^{-1}S(M) \to S(R^{-1}M)
$$ là đồng nhất trên $R^{-1}M$.

### 9. MÔĐUN PHÂN THỨC CỦA CÁC MÔĐUN PHÂN BẬC

Cho $A$ là một vành phân bậc, $M$ là một $A$-môđun phân bậc và $A$ là monoid bậc; trong số này ta giả sử rằng $A$ là một *nhóm*. Nhắc lại (*Đại số*, Chương II, § 11) rằng $A$ và $M$ lần lượt là các tổng trực tiếp của các nhóm cộng tính $$
A = \bigoplus_{i \in \Delta} A_i, \qquad M = \bigoplus_{i \in \Delta} M_i
$$ với $A_i A_j \subset A_{i+j}$ và $A_i M_j \subset M_{i+j}$ với mọi $i, j \in A$. Cho $S$ là một tập con nhân của $A$ *mà mọi phần tử của nó đều thuần nhất*. Với mọi $i \in A$, ta đặt $S_i = S \cap A_i$ và ký hiệu $(S^{-1}M)_i$ là tập hợp các phần tử $m'$ của $S^{-1}M$ sao cho tồn tại các phần tử $j, k$ của $A$, một phần tử $m \in M_j$ và một phần tử $s \in S_k$ sao cho $j - k = i$ và $m' = m/s$. Nếu $(m'_q)_{1 \leq q \leq r}$ là một họ hữu hạn các phần tử của $S^{-1}M$ sao cho $$
m'_q \in (S^{-1}M)_{j(q)},
$$ thì tồn tại các phần tử $j(q) \in A$ và $k \in A$, các phần tử $m_q \in M_{j(q)}$ ($1 \leq q \leq r$) và $s \in S_k$ sao cho $m'_q = m_q/s$ với $1 \leq q \leq r$ (no. 1, *Nhận xét 2*).

#### Mệnh đề 21 {#ac-ii-s2-prop-21 .statement}

*Vành $S^{-1}A$ với họ $((S^{-1}A)_i)$ là một vành phân bậc và $S^{-1}M$ với họ $((S^{-1}M)_i)$ là một môđun phân bậc trên vành phân bậc $S^{-1}A$. Các ánh xạ chính tắc $i^S_A$ và $i^S_M$ là thuần nhất bậc 0.*

Cho $m \in M$, $s \in S_k$, $m' \in M_{j'}$, $s' \in S_{k'}$ và giả sử rằng $j - k = j' - k' = i$; khi đó $(m/s) - (m'/s') = (s'm - sm')/ss'$ và $s'm - sm' \in M_{j'+k'} = M_{j'+k'}$ và $ss' \in S_{k+k'}$, do đó $(m/s) - (m'/s') \in (S^{-1}M)_i$ theo định nghĩa; điều này chỉ ra rằng các $(S^{-1}M)_i$ là các nhóm con cộng tính của $S^{-1}M$. Tổng của các nhóm này là toàn bộ $S^{-1}M$: với mọi $x \in S^{-1}M$ có thể viết được dưới dạng $m/s$ trong đó $m \in M, s \in S; s$ là thuần nhất theo giả thiết và $m$ là tổng của các phần tử thuần nhất $m_j$; do đó $x$ là tổng của các $m_j/s$, mỗi phần tử trong đó thuộc một nhóm con $(S^{-1}M)_i$. Cuối cùng tổng của các $(S^{-1}M)_i$ là trực tiếp; thật vậy, xét một họ hữu hạn các phần tử $x_q$ ($1 \leq q \leq n$) sao cho $x_q \in (S^{-1}M)_{i(q)}$, trong đó các chỉ số $i(q)$ là phân biệt, và giả sử rằng $\sum_{q=1}^n x_q = 0$. Mỗi $x_q$ có thể viết dưới dạng $x_q = m_q/s$ trong đó $s \in S_k$ và $m_q \in M_{i(q)+k}$; giả thiết kéo theo rằng tồn tại $s' \in S$ sao cho $s'\left( \sum_{q=1}^n m_q \right) = 0$; nếu các $s'm_q$ không phải tất cả đều bằng không, ta sẽ có một mâu thuẫn vì, nếu $s' \in S_d$, thì $s'm, \in M_{i(q)+d}$ và các $i(q) + d$ đều phân biệt. Suy ra rằng $x_q = 0$ với mọi chỉ số $q$.

Ta kiểm tra ngay lập tức rằng, nếu $a \in (S^{-1}A)_i$ và $x \in (S^{-1}M)_j$, thì $ax \in (S^{-1}M)_{i+j}$. Áp dụng kết quả này cho trường hợp $M = A$, trước hết ta thấy rằng $S^{-1}A$ là một vành được phân bậc bởi các $(S^{-1}A)_i$; sau đó ta thấy rằng $S^{-1}M$ là môđun phân bậc trên $S^{-1}A$. Cuối cùng, vì $1 \in A_0$, $i_A^S$ và $i_M^S$ là thuần nhất bậc 0.

#### Mệnh đề 22 {#ac-ii-s2-prop-22 .statement}

Cho A (tương ứng B) là một vành phân bậc kiểu A, M (tương ứng N) là một môđun phân bậc trên vành phân bậc A (tương ứng B), S (tương ứng T) là một tập con nhân tính của A (tương ứng B) mà mọi phần tử đều thuần nhất, $f : A \to B$ là một đồng cấu thuần nhất bậc 0 sao cho $f(S) \subset T$ và $u : M \to N$ là một ánh xạ A-tuyến tính thuần nhất bậc k. Khi đó đồng cấu $f' : S^{-1}A \to T^{-1}B$ dẫn xuất từ f (no. 1, Mệnh đề 2) là thuần nhất bậc 0 và ánh xạ $(S^{-1}A)$-tuyến tính

$$
u' : S^{-1}M \to T^{-1}N
$$

dẫn xuất từ f và $u$ (no. 2, Mệnh đề 5) là thuần nhất bậc k.

Điều này suy ra ngay lập tức từ các đẳng thức $f'(a/s) = f(a)/f(s)$ và $u'(m/s) = u(m)/f(s)$.

Cuối cùng chú ý rằng, nếu E là một đại số trên A phân bậc và S là một tập con nhân tính của A gồm các phần tử thuần nhất, thì $S^{-1}E$, với cấu trúc đại số trên $(S^{-1}A)$ của nó (no. 8) và phân bậc $(S^{-1}E)_i$, là một đại số trên $S^{-1}A$ phân bậc, như suy ra ngay lập tức từ các định nghĩa.

### Bài tập {#ac-ii-s2-exercises}

Xem [bài tập của § 2](exercises/s2/).
