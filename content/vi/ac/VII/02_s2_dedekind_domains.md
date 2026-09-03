---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 2
section_title: Dedekind domains
lang: vi
source: ac-i-vii
book_pages: 493-502, 556-571
pdf_pages: 0511-0520, 0574-0589
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF DEDEKIND DOMAINS
      page: 493
      pdf_page: 511
    - "no": 2
      title: CHARACTERIZATIONS OF DEDEKIND DOMAINS
      page: 494
      pdf_page: 512
    - "no": 3
      title: DECOMPOSITION OF IDEALS INTO PRODUCTS OF PRIME IDEALS
      page: 496
      pdf_page: 514
    - "no": 4
      title: THE APPROXIMATION THEOREM FOR DEDEKIND DOMAINS
      page: 497
      pdf_page: 515
    - "no": 5
      title: THE KRULL-AKIZUKI THEOREM
      page: 499
      pdf_page: 517
statements: 14
exercises: 27
content_sha256: 33b338ac61226b7bfa7d263cfe8e155aaa36556c97da7b6b5f456fdb75cbc467
translated_from: content/en/ac/VII/02_s2_dedekind_domains.md
source_content_sha256: 16fa7953b099cb50ab812cae794d31718963a0e7a0358d8c489c21f500087f43
translation_model: gpt-5.4
translation_run: translate-vi-026a06a8
glossary_version: 34
glossary_terms_sha256: f2ee899bb8d0114cfe173feac686f459f973a8453466e89c1fab61c3c0eb1e44
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. MIỀN DEDEKIND

### 1. ĐỊNH NGHĨA MIỀN DEDEKIND

Cho $A$ là một miền nguyên. Rõ ràng các điều kiện sau là tương đương:
(a) không có hai iđêan nguyên tố khác không nào của $A$ là so sánh được đối với quan hệ bao hàm;
(b) các iđêan nguyên tố khác không của $A$ là cực đại;
(c) các iđêan nguyên tố khác không của $A$ có chiều cao bằng 1.

#### Định nghĩa 1 {#ac-vii-s2-def-1 .statement}

Một miền Krull mà mọi iđêan nguyên tố khác không đều là cực đại được gọi là một miền Dedekind.

Các ví dụ về miền Dedekind
(1) Mọi miền iđêan chính đều là một miền Dedekind.
(2) Cho K là một mở rộng hữu hạn của $\mathbf{Q}$ và A là bao đóng nguyên của $\mathbf{Z}$ trong K. Vành A là một miền Krull (§ 1, no. 8, Mệnh đề 12). Cho $\mathfrak{p}$ là một iđêan nguyên tố khác không của A. Khi đó $\mathfrak{p} \cap \mathbf{Z}$ là khác không (Chương V, § 2, no. 1, Hệ quả của Mệnh đề 1) và do đó là một iđêan cực đại của $\mathbf{Z}$; do đó $\mathfrak{p}$ là một iđêan cực đại của A (*loc. cit.*, Mệnh đề 1). Vậy A là một miền Dedekind. Nói chung, A không phải là một miền iđêan chính (*Algebra*, Chương VII, § 1, Bài tập 12).
(3) \* Cho V là một đa tạp đại số afin và A là vành các hàm chính quy trên V. Giả sử rằng A không phải là một trường (tức là V không thu về một điểm). Để A là một miền Dedekind, điều kiện cần và đủ là V là một đường cong bất khả quy không có điểm kỳ dị: vì nói rằng A là một miền nguyên tương đương với nói rằng V là bất khả quy; nói rằng mọi iđêan nguyên tố khác không của A đều là cực đại tương đương với nói rằng A là một đường cong; sau cùng, vì A là Noether, nói rằng nó là một miền Krull tương đương với nói rằng nó đóng nguyên, nghĩa là V là một đường cong chuẩn tắc, hay cũng có nghĩa là nó không có điểm kỳ dị. \*
(4) Một vành phân thức $S^{-1}A$ của một miền Dedekind A là một miền Dedekind nếu $0 \notin S$. Thật vậy, $S^{-1}A$ là một miền Krull (§ 1, no. 4, Mệnh đề 6) và mọi iđêan nguyên tố khác không của $S^{-1}A$ đều là cực đại theo Chương II, § 2, no. 5, Mệnh đề 11.

### 2. CÁC ĐẶC TRƯNG CỦA MIỀN DEDEKIND

#### Định lý 1 {#ac-vii-s2-thm-1 .statement}

Cho A là một miền nguyên và K là trường phân thức của nó. Các điều kiện sau là tương đương:
(a) A là một miền Dedekind;
(b) A là một miền Krull và mọi định giá không suy biến trên K mà dương trên A đều tương đương với một định giá cốt yếu của A;
(c) A là một miền Krull và mọi iđêan phân thức $\mathfrak{J} \neq (0)$ của A đều là chia được;
(d) mọi iđêan phân thức $3 \neq (0)$ của A đều khả nghịch;
(e) A là một miền đóng nguyên Noether và mọi iđêan nguyên tố khác không của A đều là cực đại;
(f) A là Noether và, với mọi iđêan cực đại m của A, $A_m$ hoặc là một trường hoặc là một vành định giá rời rạc;
(g) A là Noether và, với mọi iđêan cực đại m của A, $A_m$ là một miền iđêan chính.

Trước hết ta chứng minh tính tương đương của (a) và (b). Hệ quả 2 của Định lý 3, § 1, no. 6, cho thấy ngay lập tức rằng (a) kéo theo (b). Ngược lại, (b) kéo theo (a), vì, với mọi iđêan nguyên tố $p$ của $A$, tồn tại một vành định giá của $K$ trội hơn $A_p$ (Chương VI, § 1, no. 2, Hệ quả của Định lý 2).

Phần còn lại của chứng minh được tiến hành bằng cách chứng minh các kéo theo sau:

$$
(a) \Rightarrow (c) \Rightarrow (d) \Rightarrow (e) \Rightarrow (f) \Rightarrow (g) \Rightarrow (a).
$$

Nếu $A$ là một miền Dedekind và $b$ là một iđêan phân thức khác không, thì $bA_p = bA_p$ với mọi iđêan cực đại $p$ ($§ 1$, no. 4, Mệnh đề 7) và do đó $b = 6$ (Chương II, $§ 3$, no. 3, Hệ quả 3 của Định lý 1); vì thế (a) kéo theo (c).

Bây giờ ta chứng minh rằng (c) kéo theo (d). Nếu (c) đúng, ánh xạ $a \mapsto \operatorname{div} a$ là một song ánh từ $I(A)$ lên $D(A)$ (xem $§ 1$, no. 1); vì nó là một đồng cấu ($§ 1$, no. 2) và $D(A)$ là một nhóm, mọi phần tử của $I(A)$ đều khả nghịch.

Ta chứng minh rằng (d) kéo theo (e). Nếu (d) đúng, mọi iđêan nguyên $\neq (0)$ của $A$ đều sinh hữu hạn (Chương 11, $§ 5$, no. 6, Định lý 4) và do đó $A$ là Noether; vì $I(A)$ là một nhóm, $D(A)$ là một nhóm và vì thế $A$ hoàn toàn đóng nguyên ($§ 1$, no. 2, Định lý 1). Sau cùng, nếu $p$ là một iđêan nguyên tố khác không của $A$ và $m$ là một iđêan cực đại của $A$ chứa $p$, thì vành $A_{m}$ là một miền iđêan chính (Chương II, $§ 5$, no. 6, Định lý 4); vì $pA_m$ là nguyên tố và khác không, tất yếu $pA_m = mA_m$ (một miền iđêan chính là một miền Dedekind) do đó $p = m$ (Chương 11, $§ 2$, no. 5, Mệnh đề 11) và $p$ là cực đại.

Bây giờ ta chỉ ra rằng (e) suy ra (f). Nếu $m$ là một iđêan cực đại của $A$ và (e) đúng, thì $A_{m}$ là một miền Noether nguyên đóng và iđêan cực đại $mA_m$ của nó hoặc là (0), hoặc là iđêan nguyên tố khác không duy nhất của $A_{m}$; do đó $A_{m}$ là một trường hoặc một vành định giá rời rạc theo Mệnh đề 11 của $§ 1$, no. 7.

Việc (f) suy ra (g) là hiển nhiên.

Sau cùng ta chỉ ra rằng (g) suy ra (a). Vì $A$ là giao của các $A_{m}$, với $m$ chạy qua tập hợp các iđêan cực đại (Chương II, $§ 3$, no. 3, Hệ quả 4 của Định lý 1), (g) suy ra rằng $A$ là nguyên đóng và Noether và do đó $A$ là một miền Krull ($§ 1$, no. 3, Hệ quả của Định lý 2). Mặt khác, có thể chỉ ra rằng mọi iđêan nguyên tố khác không của $A$ đều cực đại như trong chứng minh rằng (d) $\Rightarrow$ (e).

#### Mệnh đề 1 {#ac-vii-s2-prop-1 .statement}

*Một miền Dedekind nửa địa phương là một miền iđêan chính.*

Cho $A$ là một miền Dedekind nửa địa phương, $K$ trường phân thức của nó, $p_1, \ldots, p_n$ các iđêan cực đại của nó và $v_1, \ldots, v$, các định giá cốt yếu tương ứng; đó là các định giá cốt yếu duy nhất của $A$. Cho $a$ là một iđêan nguyên khác không của $A$. Vì nó là một iđêan ước, tồn tại ($§ 1$, no. 4, Mệnh đề 5) các số nguyên $q_1, \ldots, q_n$ sao cho $a$ là tập hợp các $x \in K$ sao cho $v_i(x) \geq q_i$ với $1 \leq i \leq n$. Cho $x_0$ là một phần tử của $K$ sao cho $v_i(x_0) = q_i$ với $1 \leq i \leq n$ (Chương VI, $§ 7$, no. 2, Hệ quả 1 của Định lý 1). Khi đó $a$ là tập hợp các $x \in K$ sao cho $v_i(xx_0^{-1}) \geq 0$ với $1 \leq i \leq n$. Vậy $a = Ax_0$.

Nếu $A$ là một miền Dedekind, trong chứng minh của Định lý 1 đã thấy rằng nhóm D(A) các ước của A được đồng nhất với nhóm I(A) các iđêan phân thức $a \neq (0)$ (vì A là Noether, mọi iđêan phân thức khác không đều sinh hữu hạn). Khi đó nhóm lớp các ước C(A) của A ($§ 1$, no. 2) được đồng nhất với nhóm các lớp iđêan $\neq 0$ của A (được định nghĩa trong Chương II, $§ 5$, no. 7).

### 3. PHÂN TÍCH CÁC IĐÊAN THÀNH TÍCH CÁC IĐÊAN NGUYÊN TỐ

Cho A là một miền Dedekind, I(A) nhóm nhân có thứ tự của các iđêan phân thức khác không của A và D(A) nhóm các ước của A. Đẳng cấu $a \mapsto \operatorname{div} a$ từ I(A) lên D(A) biến các ước cực biên thành các iđêan nguyên tố khác không của A ($§ 1$, no. 6, Định lý 3) và do đó nhóm nhân I(A) nhận tập hợp các iđêan nguyên tố khác không của A làm cơ sở ($§ 1$, no. 3, Định lý 2). Nói cách khác, *mọi iđêan phân thức khác không a của A đều có một phân tích duy nhất dưới dạng*:

$$
a = \prod_p p^{n(p)}
$$

trong đó tích lấy trên các iđêan nguyên tố khác không của A, các số mũ $n(p)$ bằng không trừ ra đối với một số hữu hạn trong chúng. Hơn nữa a là nguyên khi và chỉ khi các $n(p)$ đều dương. Quan hệ (1) được gọi là *phân tích của a thành các nhân tử nguyên tố*. Đặc biệt, nếu a là một iđêan chính $Ax$, thì với mọi $p$, $n(p) = v_p(x)$, trong đó $v_p$ ký hiệu định giá cốt yếu tương ứng với $p$; điều này suy ra từ công thức (4) của $§ 1$, no. 3. Cho

$$
a = \prod_p p^{m(p)}, \quad b = \prod_p p^{n(p)}
$$

là hai iđêan phân thức khác không của A. Khi đó

$$
ab = \prod_p p^{m(p) + n(p)} \tag{2}
$$
$$
a : b = ab^{-1} = \prod_p p^{m(p) - n(p)} \tag{3}
$$
$$
a + b = \prod_p p^{\inf(m(p), n(p))} \tag{4}
$$
$$
a \cap b = \prod_p p^{\sup(m(p), n(p))} \tag{5}
$$

Quan hệ (2) là hiển nhiên; quan hệ (3) suy ra từ đó, đẳng thức $a : b = ab^{-1}$ suy ra từ đẳng thức

$$
\operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b
$$

($§ 1$, no. 2, Hệ quả của Định lý 1); các công thức (4) và (5) suy ra từ Mệnh đề 2, $§ 1$, no. 1.

Các kết quả này áp dụng đặc biệt cho bao đóng nguyên của $\mathbf{Z}$ trong một mở rộng hữu hạn của $\mathbf{Q}$.

Nếu $A$ là một miền iđêan chính, các kết quả trên lại cho các kết quả của Đại số, Chương VII, § 1, no. 3.

### 4. ĐỊNH LÝ XẤP XỈ CHO CÁC MIỀN DEDEKIND

Trong các miền Dedekind có một "định lý xấp xỉ" làm mạnh cả Định lý 1 của Chương VI, § 7, no. 2 lẫn Mệnh đề 9 của § 1, no. 5:

#### Mệnh đề 2 {#ac-vii-s2-prop-2 .statement}

Cho $A$ là một miền Dedekind, $K$ là trường phân thức của nó và $P$ là tập hợp các iđêan nguyên tố khác không của $A$; với $p \in P$ gọi $v_p$ là định giá cốt yếu tương ứng của $A$. Cho $p_1, \ldots, p_q$ là các phần tử phân biệt của $P$ và $n_1, \ldots, n_q$ là các số nguyên hữu tỉ và $x_1, \ldots, x_q$ là các phần tử của $K$. Khi đó tồn tại $x \in K$ sao cho $v_{p_i}(x - x_i) \geq n_i$ với $1 \leq i \leq q$ và $v_p(x) \geq 0$ với mọi $p \in P$ phân biệt với các $p_i$.

Nếu cần, thay thế các $n_i$ bằng những số nguyên lớn hơn, có thể giả sử tất cả chúng đều dương. Trước hết ta xét trường hợp các $x_i$ thuộc $A$; điều đó hiển nhiên quy về việc tìm một $x \in A$ thỏa mãn các đồng dư thức

$$
x \equiv x_i \pmod{p_i^{n_i}}
$$

và sự tồn tại của $x$ khi đó suy ra từ Chương II, § 1, no. 2, Mệnh đề 5.

Bây giờ ta chuyển sang trường hợp tổng quát. Ta có thể viết $x_i = s^{-1} y_i$ trong đó $s, y_i$ thuộc $A$; viết $x = s^{-1} y$, điều đó quy về việc tìm một $y \in A$ sao cho, một mặt, $v_{p_i}(y - y_i) \geq n_i + v_{p_i}(s)$ và, mặt khác, $v_p(y) \geq v_p(s)$ với mọi $p \in P$ phân biệt với các $p_i$; vì $v_p(s) = 0$ trừ ra với một số hữu hạn chỉ số $p$, như vậy bài toán được quy về trường hợp trên; do đó mệnh đề.

Mệnh đề 2 có thể được diễn giải như một định lý mật độ. Chính xác hơn, với mọi $p \in P$, ký hiệu $\hat{K}_p$ (resp. $\hat{A}_p$) là phép hoàn bị của $K$ (resp. $A$) đối với định giá rời rạc $v_p$ và xét tích $\prod_{p \in P} \hat{K}_p$; một phần tử $x = (x_p)$ của tích này được gọi là một adèle hạn chế của $A$ nếu $x_p \in \hat{A}_p$ với mọi $p \in P$ trừ ra một số hữu hạn phần tử. Rõ ràng tập hợp $A$ các adèle hạn chế là một vành con của $\prod_{p \in P} \hat{K}_p$, chứa vành tích $A, = \prod_{p \in P} \hat{A}_p$. Xét trên $A$, tôpô tích, đối với tôpô này $A,$ là đầy đủ; tồn tại trên $A$ một tôpô duy nhất $\mathcal{T}$ tương thích với cấu trúc nhóm cộng của nó và đối với đó các lân cận của 0 trong $A$, lập thành một hệ cơ bản $\mathcal{G}$ các lân cận của 0. Tôpô $\mathcal{T}$ tương thích với cấu trúc vành trên $A$; vì rõ ràng tiên đề (AVII) của *General Topology*, Chapter 111, § 6, no. 3, được thỏa mãn, tôpô cảm sinh bởi $\mathcal{T}$ trên $A,$ tương thích với cấu trúc vành trên $A,$. Mặt khác, với mọi $x \in A$ tồn tại một tập con hữu hạn $J$ của $P$ sao cho, nếu viết $J' = P - J, \ K_J \leq \prod_{p \in J} \hat{K}_p, \ A_{J'} = \prod_{p \in J'} \hat{A}_p,$ thì x \in K_J \times A_{J'} và, vì $\hat{A}_p$ là mở trong $\hat{K}_p$ với mọi p, $\mathcal{G}$ là một hệ cơ bản các lân cận của 0 đối với tôpô tích trên $K_J \times A_{J'}$; vì tôpô sau tương thích với cấu trúc vành trên tích này, tiên đề (AV_1) của *General Topology*, Chapter III, *loc. cit.* cũng được thấy là thỏa mãn, điều đó chứng minh mệnh đề của chúng ta. Rõ ràng A, là một vành con *mở* của A và do đó A cũng là một vành *đầy đủ* (*General Topology*, Chapter III, § 3, no. 3, Proposition 4).

Với mọi $x \in K$, ký hiệu $\Delta(x)$ là phần tử $(x_p) \in \prod_{p \in P} \hat{K}_p$ sao cho $x_p = x$ với mọi $p \in P$; vì $x_p \in \hat{A}_p$ trừ ra với một số hữu hạn giá trị của p, ta có $\Delta(x) \in A$; như vậy ta đã xác định được một đồng cấu $A : K \to A$ là *đơn ánh* nếu $P \neq \varnothing$ (nghĩa là nếu A không phải là một trường); các phần tử của $\Delta(K)$ được gọi là các *adèle hạn chế chính* và rõ ràng $\Delta(A) \subset A$.

#### Mệnh đề 3 {#ac-vii-s2-prop-3 .statement}

*Vành A, (resp. A ) được đồng nhất với phép hoàn bị của A (resp. K) đối với tôpô vành mà một hệ cơ bản các lân cận của 0 gồm tất cả các iđêan nguyên $\neq (0)$ của A.*

Ngay lập tức thấy rằng tôpô đang xét trên A (hoặc K) là Hausdorff. Có tính đến no. 3, mệnh đề liên quan đến A, suy ra từ Chương 111, § 2, no. 13, mệnh đề 17. Do đó điều này cho thấy $\Delta(A)$ trù mật trong A,; để thấy tương tự rằng $\Delta(K)$ trù mật trong A, hãy chú ý rằng với mọi $x = (x_i) \in A$ chỉ có hữu hạn $p \in P$ sao cho $v_p(x_p) < 0$; bởi § 1, no. 5, mệnh đề 9, vì thế tồn tại một $s \in K$ sao cho $sx_p \in \hat{A}_p$ với mọi $p \in P$, nói cách khác $\Delta(s)x \in A$, và vì phép nhân bởi $\Delta(s)$ là một đồng cấu từ A vào chính nó, chỉ cần áp dụng sự kiện rằng $\Delta(A)$ trù mật trong A , để suy ra rằng $\Delta(K)$ trù mật trong A.

Dĩ nhiên ta cũng có thể chứng minh rằng $\Delta(K)$ trù mật trong A bằng cách dùng Mệnh đề 2.

Xét bây giờ nhóm nhân $\mathbf{SL}(n, A)$ gồm các ma trận $U \in \mathbf{M}_n(A)$ sao cho $\det(U) = 1$; nếu $\mathbf{M}_n(A) = A^{n^2}$ được trang bị tôpô tích, thì nó cảm sinh trên $\mathbf{SL}(n, A)$ một tôpô *tương thích với cấu trúc nhóm* trên $\mathbf{SL}(n, A)$. Chỉ cần kiểm tra rằng ánh xạ $U \mapsto U^{-1}$ là liên tục trên $\mathbf{SL}(n, A)$; nhưng vì U là đơn môđula, ta biết rằng (*Algebra*, Chương III, § 6, no. 5, công thức (17)) các phần tử của $U^{-1}$ là các *phần bù đại số* của U và do đó là các đa thức theo các phần tử của U, điều này chứng minh mệnh đề của chúng ta. Nếu K được đồng nhất với một vành con của A thông qua A, thì nhóm $\mathbf{SL}(n, K)$ là một nhóm con của $\mathbf{SL}(n, A)$.

#### Mệnh đề 4 {#ac-vii-s2-prop-4 .statement}

*Nhóm $\mathbf{SL}(n, K)$ là trù mật trong $\mathbf{SL}(n, A)$.*

Gọi G là bao đóng của $\mathbf{SL}(n, K)$ trong $\mathbf{SL}(n, A)$; vì K là trù mật trong A (Mệnh đề 3), nên G chứa mọi ma trận có dạng $I + a . E_{ij}$ với $i \neq j$ và $a \in A$. Với mọi $p \in P$ và mọi $\lambda \in \hat{K}_p$, gọi $\lambda(p)$ là adèle hạn chế $x = (x_q)_{q \in P}$ sao cho $x_p = \lambda$ và $x_q = 0$ với $q \neq p$; điều trên cho thấy G chứa các ma trận $I + \lambda(p)E_{ij}$ với $i \neq j$. Nhưng ta biết rằng các ma trận có dạng $I + \lambda E_{ij}$ với $\lambda \in \hat{K}_p$ sinh ra nhóm $\mathbf{SL}(n, \hat{K}_p)$ (*Algebra*, Chương 111). Với mỗi ma trận $U \in \mathbf{SL}(n, A)$, ký hiệu $U_p$ là ảnh chính tắc của $U$ trong $\mathbf{SL}(n, \hat{\mathbf{K}}_p)$; do đó ta thấy rằng, với mọi $p \in P$, G chứa các ma trận $U \in \mathbf{SL}(n, A)$ sao cho $U_q = I$ với mọi $q \# p$. Vì $G$ là một nhóm, nó cũng chứa mọi ma trận $U \in \mathbf{SL}(n, A)$ sao cho $U_p = I$ trừ ra một số *hữu hạn* các $p \in P$; bây giờ, định nghĩa của tôpô trên $A$ cho thấy ngay lập tức rằng tập hợp các ma trận ấy là trù mật trong $\mathbf{SL}(n, A)$.

### 5. ĐỊNH LÝ KRULL-AKIZUKI

#### Bổ đề 1 {#ac-vii-s2-lem-1 .statement}

*Cho $A$ là một miền Noether trong đó mọi iđêan nguyên tố khác không đều là cực đại và $M$ là một $A$-môđun xoắn hữu hạn sinh. Khi đó độ dài $\operatorname{long}_A(M)$ của $M$ là vô hạn.*

Vì $M$ là một môđun xoắn, mọi iđêan nguyên tố liên kết với $M$ đều $\neq (0)$ và do đó đều cực đại. Khi ấy bổ đề suy ra từ Chương IV, § 2, no. 5, Mệnh đề 7.

#### Bổ đề 2 {#ac-vii-s2-lem-2 .statement}

*Cho $A$ là một vành, $T$ một $A$-môđun và $(T_i)$ một họ có hướng phải các môđun con của $T$ với hợp là $T$. Khi đó $\operatorname{long}_A(T) = \sup_i (\operatorname{long}_A(T_i))$.*

$\operatorname{long}_A(T_i) \leq \operatorname{long}_A(T)$ với mọi $i$. Bổ đề là hiển nhiên nếu không có số nguyên nào vượt quá các $\operatorname{long}_A(T_i)$, khi đó cả hai vế đều là vô hạn. Nếu không, gọi $i_0$ là một chỉ số sao cho $\operatorname{long}_A(T_{i_0})$ nhận giá trị lớn nhất của nó; khi đó $T_{i_0} = T$ vì họ $(T_i)$ là có hướng; do đó mệnh đề của chúng ta trong trường hợp này.

#### Nhận xét {#ac-vii-s2-n5-rem-1 .statement}

Chứng minh này không giả thiết rằng $A$ là giao hoán.

#### Bổ đề 3 {#ac-vii-s2-lem-3 .statement}

*Cho $A$ là một miền nguyên Noether sao cho mọi iđêan nguyên tố khác không $\& A$ đều cực đại, $M$ một $A$-môđun không xoắn hạng hữu hạn $r$ và một phần tử khác không của $A$. Khi đó $A/Aa$ là một $A$-môđun có độ dài hữu hạn và:*
$$
\operatorname{long}_A(M/aM) \leq r \cdot \operatorname{long}_A(A/Aa).
$$
Bổ đề 1 cho thấy rằng $\operatorname{long}_A(A/Aa)$ là hữu hạn. Trước hết ta chứng minh (6) trong trường hợp $M$ là *A-môđun hữu hạn sinh*. Vì $M$ không xoắn và có hạng $r$, tồn tại một môđun con $L$ của $M$ đẳng cấu với $A'$ và sao cho $Q = M/L$ là một $A$-môđun xoắn sinh hữu hạn và do đó có độ dài hữu hạn (Bổ đề 1). Với mọi số nguyên $n \geq 1$, hạt nhân của toàn cấu chính tắc $M/a^nM \to Q/a^nQ$ bằng $(L + a^nM)/a^nM$ và đẳng cấu với $L/(a^nM \cap L)$; vì
$$
a^nL \subset a^nM \cap L,
$$
nên
$$
\operatorname{long}_A(M/a^nM) \leq \\
\operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q/a^nQ) \leq \operatorname{long}_A(L/a^nL) + \operatorname{long}_A(Q).
$$
Bây giờ, vì $M$ không xoắn, phép nhân bởi $a$ xác định một đẳng cấu của

M/aM lên aA/a^2M; tương tự đối với L; do đó, bằng quy nạp theo n, các công thức:

$$
\text{long}_A(M/a^nM) = n \cdot \text{long}_A(M/aM).
$$
$$
\text{long}_A(L/a^nL) = n \cdot \text{long}_A(L/aL).
$$

Tính đến (7) ta suy ra:

$$
\text{long}_A(M/aM) \leq \text{long}_A(L/aL) + n^{-1}\text{long}_A(Q)
$$

với mọi $n > 0$; vì L đẳng cấu với A', $\text{long}_A(L/aL) = r \text{long}_A(A/Aa)$; do đó được (6) bằng cách cho $n$ tiến tới vô hạn trong (9).

Bây giờ ta chuyển sang trường hợp tổng quát. Gọi $(M_i)$ là họ các môđun con sinh hữu hạn của M. Môđun $T = M/aM$ là hợp của các môđun con $T_i = (M_i + aM)/aM = M_i/(M_i \cap aM)$. Khi đó, T, đẳng cấu với một môđun thương của $M_i/aM_i$ và do đó

$$
\text{long}_A(T_i) \leq r \text{long}_A(A/Aa)
$$

theo điều ta vừa chứng minh. Do đó

$$
\text{long}_A(T) \leq r \text{long}_A(A/Aa)
$$

theo Bổ đề 2.

Mệnh đề 5 (Krull-Akizuki). *Cho A là một miền nguyên Noether mà mọi iđêan nguyên tố khác không của nó đều cực đại, K là trường phân thức của nó, L là một mở rộng hữu hạn của K và B là một vành con của L chứa A. Khi đó B là Noether và mọi iđêan nguyên tố khác không của B đều cực đại. Hơn nữa, với mọi iđêan $b \neq (0)$ của B, B/b là một A-môđun hữu hạn sinh.*

Gọi b là một iđêan khác không của B. Ta sẽ chứng minh rằng B/b là một A-môđun có độ dài hữu hạn (do đó, *a fortiori*, là một B-môđun có độ dài hữu hạn) và rằng b là một B-môđun hữu hạn sinh.

Một phần tử khác không y của b thỏa mãn một phương trình dạng:

$$
a_r y^r + a_{r-1} y^{r-1} + \cdots + a_1 = 0 \quad (a_i \in A, a_1 \neq 0).
$$

Phương trình này cho thấy rằng $a_1 \in By \subset b$. Áp dụng Bổ đề 3 cho $M = B$, ta thấy rằng $B/a_0B$ là một A-môđun có độ dài hữu hạn; do đó B/b cũng vậy vì nó là một môđun thương của môđun ấy. Hơn nữa B-môđun b chứa, như một môđun con, $a_0B$ là môđun hữu hạn sinh; vì $b/a_0B$ có độ dài hữu hạn (với tư cách là một môđun con của $B/a_0B$) và do đó sinh hữu hạn, b chắc chắn là một B-môđun hữu hạn sinh.

Điều trên trước hết cho thấy rằng B là Noether. Mặt khác, nếu $p$ là một iđêan nguyên tố khác không của B, vành $B/p$ là một miền nguyên và có độ dài hữu hạn, do đó là một trường (*Đại số*, Chương VIII, § 6, no. 4, Mệnh đề 9), suy ra $p$ là cực đại.

#### Hệ quả 1 {#ac-vii-s2-lem-3-cor-1 .statement}

*Với mọi iđêan nguyên tố p của A, tập hợp các iđêan nguyên tố của B nằm trên p là hữu hạn.*

Giả sử trước hết $p = (0)$; khi đó iđêan nguyên tố duy nhất $q$ của $B$ sao cho $q \cap A = (0)$ là $(0)$; nếu không, đặt $S = A - \{0\}$, thì $S^{-1}q$ sẽ là một iđêan nguyên tố khác không của $S^{-1}B$ (Chương 11, § 2, no. 5, Mệnh đề 11) và $S^{-1}B$ chính là trường phân thức của $B$, vì nó là một vành con của $L$ chứa $K$ (\emph{Algebra}, Chương V, § 3, no. 2, Mệnh đề 3); do đó đi đến một kết luận phi lý. Nếu bây giờ $p \neq (0)$, thì từ Mệnh đề 5 suy ra rằng $B/pB$ là một không gian vectơ hữu hạn chiều trên trường $A/p$, nên là một vành \emph{Artin} và vì vậy chỉ có một số hữu hạn iđêan nguyên tố (Chương IV, § 2, no. 5, Mệnh đề 9), điều này chứng minh rằng chỉ có một số hữu hạn iđêan nguyên tố của $B$ chứa $p$.

#### Hệ quả 2 {#ac-vii-s2-lem-3-cor-2 .statement}

*Bao đóng nguyên của $A$ trong $L$ là một miền Dedekind.*

Bao đóng nguyên này là một miền Noether đóng nguyên mà mọi iđêan nguyên tố khác không của nó đều cực đại; do đó chỉ cần áp dụng Định lý 1 của no. 2.

Đặc biệt:

#### Hệ quả 3 {#ac-vii-s2-lem-3-cor-3 .statement}

*Bao đóng nguyên của một miền Dedekind trong một mở rộng hữu hạn của trường phân thức của nó là một miền Dedekind.*

#### Mệnh đề 6 {#ac-vii-s2-prop-6 .statement}

*Cho $A$ là một miền Dedekind, $K$ trường phân thức của nó, $L$ một mở rộng hữu hạn của $K$ và $B$ bao đóng nguyên của $A$ trong $L$. Cho $p$ là một iđêan nguyên tố khác không của $A$, $v$ định giá cốt yếu tương ứng của $K$ và*

$$
Bp = \prod_i p_i^{e(i)}
$$

*phân tích của iđêan $Bp$ thành tích các iđêan nguyên tố. Khi đó:*
(a) *các iđêan nguyên tố của $B$ nằm trên $p$ là các $p_i$ sao cho $e(i) > 0$;*
(b) *các định giá $v_i$ trên $L$ tương ứng với các iđêan $p_i$ này, xét đến tương đương, là các định giá trên $L$ mở rộng $v$;*
(c) $[B/p_i : A/p] = f(v_i/v);$
(d) $e_i = e(v_i/v)$ (xem Chương VI, § 8, no. 1, Định nghĩa 1 và 2).

(a) Nói rằng một iđêan nguyên tố $q$ của $B$ nằm trên $p$ có nghĩa là $q \supseteq p$, nên $q \supseteq Bp$ và $q$ chứa một trong các $p_i$ sao cho $e(i) > 0$ (Chương 11, § 1, no. 1, Mệnh đề 1).
(b) Điều này suy ra, có tính đến (a), từ § 1, no. 8, Hệ quả của Mệnh đề 12.
(c) Trường thặng dư của $v$ được đồng nhất với $A/p$ và trường thặng dư của $v_i$ với $B/p_i$ (§ 1, no. 4, Hệ quả 1 của Mệnh đề 6).

(d) Cho $a$ (tương ứng $a_i$) là một phần tử chuẩn hoá của $v$ (tương ứng $v_i$). Khi đó
$$
a B_{p_i} = a A_p B_{p_i} = p A_p B_{p_i} = p B . B_{p_i} = \left( \prod_j p_j^{e(j)} \right) B_{p_i} = \prod_j (p_j B_{p_i})^{e(j)} \\
= (p_i B_{p_i})^{e(i)} = a_i^{e(i)} B_{p_i}
$$
vì $p_j B_{p_i} = B_j$ với $j \neq i$; do đó suy ra (d), vì $e(v_i/v) = v_i(a)$.

### Bài tập {#ac-vii-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
