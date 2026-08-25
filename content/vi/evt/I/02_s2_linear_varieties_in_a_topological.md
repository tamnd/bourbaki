---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: TOPOLOGICAL VECTOR SPACES OVER A VALUED DIVISION RING
section: 2
section_title: Linear varieties in a topological vector space
lang: vi
source: evt-i-v
book_pages: TVS I.11-TVS I.16, TVS I.25-TVS I.28
pdf_pages: 0019-0024, 0033-0036
extraction: ocr
subsections:
    - "no": 1
      title: The closure of a linear variety
      page: 11
      pdf_page: 19
    - "no": 2
      title: Lines and closed hyperplanes
      page: 12
      pdf_page: 20
    - "no": 3
      title: Vector subspaces of finite dimension
      page: 13
      pdf_page: 21
    - "no": 4
      title: Locally compact topological vector spaces
      page: 15
      pdf_page: 23
statements: 26
exercises: 12
content_sha256: 7b29b5e36f80046d65c74fc796d512c5752476f261e4b3a8404bdb6b0f96a576
translated_from: content/en/evt/I/02_s2_linear_varieties_in_a_topological.md
source_content_sha256: 61cd6dad8d3c88edb55c2b3d99dcd153e54788854713e19386098384030e5241
translation_model: gpt-5.4-mini
translation_run: translate-vi-41cdad82
glossary_version: 34
glossary_terms_sha256: 2ede0ceebec65bcf1af7532ef812dafce547390273ef7bbb6bfa2703b551db76
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. CÁC ĐA TẠP TUYẾN TÍNH TRONG MỘT KHÔNG GIAN VECTƠ TÔPÔ

### 1. Bao đóng của một đa tạp tuyến tính

Nhắc lại (A, II, § 9.3) rằng trong một không gian vectơ $E$ trên một vành chia $K$, một đa tạp tuyến tính afin không rỗng (gọi là « đa tạp tuyến tính » khi điều này không gây nhầm lẫn) là ảnh qua một phép tịnh tiến của một không gian con vectơ của $E$.

#### Mệnh đề 1 {#evt-i-s2-prop-1 .statement}

— *Trong một không gian vectơ tôpô $E$, bao đóng của một đa tạp tuyến tính là một đa tạp tuyến tính.*

Vì mọi phép tịnh tiến đều là một phép đồng phôi của $E$, nên đủ chứng minh mệnh đề cho một không gian con vectơ $M$ của $E$, và trong trường hợp này, mệnh đề đã được chứng minh ở I, p. 4.

#### Hệ quả {#evt-i-s2-n1-cor-1 .statement}

— *Trong một không gian vectơ tôpô $E$, mọi siêu phẳng hoặc là đóng hoặc là trù mật khắp nơi.*

Thật vậy, bao đóng của một siêu phẳng thuần nhất $H$ chỉ có thể là $H$ hoặc toàn bộ không gian $E$, vì nó là một không gian con vectơ chứa $H$ (mệnh đề 1).

Một siêu phẳng $H$ là *đóng* trong $E$ khi, và chỉ khi, $\complement H$ chứa một điểm trong.

Không gian con vectơ $M$ sinh bởi một tập hợp $A$, trong một không gian vectơ tôpô $E$, là tập hợp các tổ hợp tuyến tính của các điểm của $A$ (A, II, § 1.7, mệnh đề 9); bao đóng của $M$ trong $E$ là, theo mệnh đề 1, không gian con vectơ đóng nhỏ nhất chứa $A$; ta nói rằng đó là *không gian con vectơ đóng sinh bởi* $A$.

#### Định nghĩa 1 {#evt-i-s2-def-1 .statement}

— *Một tập hợp $A$, trong một không gian vectơ tôpô $E$, là đầy nếu và chỉ nếu không gian con vectơ đóng sinh bởi $A$ trùng với $E$* (tức là tập các tổ hợp tuyến tính của các phần tử của $A$ là *trù mật khắp nơi*).

#### Ví dụ {#evt-i-s2-n1-exa-1 .statement}

— 1) Trong không gian định chuẩn $\mathscr{C}(I; \mathbf{C})$ (trên trường $\mathbf{C}$) của các hàm, liên tục trên $I = \{0, 1\}$, nhận giá trị trong $\mathbf{C}$, các phép hạn chế lên $I$ của các hàm $x^n \ (n \in \mathbf{N})$ tạo thành một tập đầy, theo định lý Weierstrass-Stone (GT, X, § 4.2, th. 3). Tương tự, các phép hạn chế lên $I$ của các hàm $e^{2n\pi ix} \ (n \in \mathbf{Z})$ tạo thành một tập đầy (GT, X, § 4.4, mệnh đề 8), trong không gian con $P$ của $\mathscr{C}(I, \mathbf{C})$ gồm các hàm sao cho $f(0) = f(1)$.

2) Mọi tập hấp thụ trong một không gian vectơ tôpô $E$ trên một vành chia có định giá không rời rạc (và đặc biệt mọi lân cận của 0 trong $E$) đều là một tập đầy vì nó sinh ra $E$ (I, p. 7). Do đó một đa tạp tuyến tính không trù mật trong $E$ tất yếu là một tập không trù mật ở đâu cả trong $E$ (GT, IX, § 5.1) vì bao đóng của nó không thể chứa một điểm trong.

#### Định nghĩa 2 {#evt-i-s2-def-2 .statement}

— *Một họ $(a_i)_{i \in I}$ các điểm của một không gian vectơ tôpô $E$ được gọi là độc lập tôpô nếu với mọi $\kappa \in I$, không gian con vectơ đóng sinh bởi các $a_i$, với $i \neq \kappa$, không chứa $a_\kappa$.*

#### Ví dụ 3 {#evt-i-s2-n1-exa-3 .statement}

Trong không gian chuẩn $\mathcal{C}(I; \mathbf{C})$ của các hàm liên tục được xác định trên $I = \{0, 1\}$, các hạn chế lên I của các hàm $e^{2n\pi i x}$ ($n \in \mathbf{Z}$) lập thành một họ độc lập tôpô. Nếu $f(x)$ là tổ hợp tuyến tính $\sum_{k \neq n} c_k e^{2k\pi i x}$ (trong đó chỉ hữu hạn nhiều $c_k$ khác 0) thì
$$
\int_0^1 |e^{2n\pi i x} - f(x)|^2 \, dx = 1 + \sum_{k \neq n} |c_k|^2 \geq 1
$$
và, *a fortiori*, theo định lý giá trị trung bình
$$
\sup_{x \in I} |e^{2n\pi i x} - f(x)| \geq 1
$$
điều đó cho thấy rằng $e^{2\pi i n x}$ không thuộc không gian con vectơ đóng của $\mathcal{C}(I; \mathbf{C})$ sinh bởi $e^{2k\pi i x}, \ k \neq n$.

Tập các phần tử của một họ độc lập tôpô được gọi là một *tập độc lập tôpô* của E. Mọi tập con của một tập con độc lập tôpô đều độc lập tôpô; mọi tập con gồm một điểm $x \neq 0$ đều độc lập tôpô nếu E là một không gian Hausdorff.

Một họ độc lập tôpô là độc lập (theo nghĩa đại số; *cf.* A, II, § 7.1, *Nhận xét*), nhưng đảo lại thì không đúng.

#### Ví dụ 4 {#evt-i-s2-n1-exa-4 .statement}

Trong không gian chuẩn $\mathcal{C}(I; \mathbf{C})$ của các hàm liên tục trên $I = \{0, 1\}$, các hạn chế lên I của các hàm $x^n$ ($n \in \mathbf{N}$) lập thành một họ độc lập theo nghĩa đại số. Nhưng tồn tại một dãy đa thức $(p_n)$ sao cho $p_n(x^2)$ hội tụ đều đến $x$ trên I (GT, X, § 4.2, bổ đề 2) điều đó cho thấy rằng $x$ thuộc không gian con vectơ đóng của $\mathcal{C}(I; \mathbf{C})$ sinh bởi các hàm $x^{2n}$ ($n \in \mathbf{N}$).

#### Nhận xét 1 {#evt-i-s2-n1-rem-1 .statement}

Họ các tập độc lập tôpô của một không gian vectơ tôpô *không nhất thiết quy nạp* đối với quan hệ bao hàm (I, p. 25, exerc. 2); do đó tình huống này khác với trường hợp của các tập độc lập theo nghĩa đại số. Hơn nữa, trong E không nhất thiết tồn tại một tập con độc lập tôpô cực đại (I, p. 25, exerc. 4), vì vậy không nhất thiết tồn tại một tập con vừa *toàn* vừa độc lập tôpô.

#### Nhận xét 2 {#evt-i-s2-n1-rem-2 .statement}

Cho M là một không gian con vectơ đóng của E và $(\dot{a}_i)_{i \in I}$ là một họ độc lập tôpô trong không gian thương E/M. Nếu $a_i$ là bất kỳ phần tử nào của lớp $\dot{a}_i$, thì từ định nghĩa 2, và thực tế rằng ánh xạ chính tắc của E lên E/M là liên tục, suy ra họ $(a_i)_{i \in I}$ là độc lập tôpô. Nhưng chú ý rằng nếu N là không gian con vectơ *đóng* sinh bởi các $a_i$ thì có thể xảy ra $M \cap N \neq \{0\}$ (I, p. 25, exerc. 2), và do đó tổng $M + N$ không nhất thiết là trực tiếp theo nghĩa đại số (cũng không *a fortiori* theo nghĩa tôpô).

### 2. Đường thẳng và các siêu phẳng đóng

#### Mệnh đề 2 {#evt-i-s2-prop-2 .statement}

*Mọi không gian vectơ tôpô Hausdorff* E *có chiều* 1 *trên một vành chia có định giá không rời rạc* K *đều đẳng cấu với* $K_s$; *thực vậy, với mọi* $a \neq 0$ *trong* E, *ánh xạ* $\xi \mapsto \xi a$ *của* $K_s$ *lên* E *là một đẳng cấu* (nói cách khác mọi ánh xạ tuyến tính của* $K_s$ *lên* E *đều là một đẳng cấu*).

Vì ánh xạ $\xi \mapsto \xi a$ của $K_s$ lên E là song ánh và liên tục (I, p. 1, định nghĩa 1), chỉ cần chứng minh rằng nó song liên tục. Cho $\alpha$ là một số thực $> 0$, ta chứng minh rằng tồn tại một lân cận V của 0 trong E sao cho nếu $\xi a \in V$ thì $|\xi| < \alpha$. Vì K không rời rạc, tồn tại một phần tử $\xi_0 \in K$ sao cho $0 < |\xi_0| < \alpha$; nhưng, vì E là Hausdorff, có một lân cận V của 0 sao cho $\xi_0 a$ không thuộc V. Ta có thể giả sử V là cân bằng (I, p. 7, mệnh đề 4). Khi đó nếu $\xi a \in V$ và $|\xi| \geq |\xi_0|$ thì ta có $|\xi_0 \xi^{-1}| \leq 1$, và $\xi_0 a = (\xi_0 \xi^{-1}) (\xi a) \in V$; vì mệnh đề cuối cùng này là sai nên ta thấy rằng $\xi a \in V$ suy ra $|\xi| < |\xi_0| < \alpha$. Điều này kết thúc chứng minh.

#### Hệ quả 1 {#evt-i-s2-prop-2-cor-1 .statement}

*Trong một không gian vectơ tôpô Hausdorff E, trên một vành chia có định giá không rời rạc K, mọi không gian con vectơ D có chiều 1 đều đẳng cấu với $K_s$.*

#### Hệ quả 2 {#evt-i-s2-prop-2-cor-2 .statement}

*Cho E là một không gian vectơ tôpô trên một vành chia có định giá không rời rạc. Mọi không gian con vectơ D (có chiều 1) là bổ sung đại số của một siêu phẳng thuần nhất đóng H cũng là bổ sung tôpô của H.*

Trong D, tập $\{0\}$ là đóng, vì nó là giao của D và tập đóng H; do đó D là Hausdorff. Nhưng vì E/H cũng là Hausdorff, ánh xạ chính tắc của D lên E/H, là tuyến tính, cũng là một đẳng cấu theo mệnh đề 2, từ đó suy ra kết luận (GT, III, § 6.2).

#### Định lý 1 {#evt-i-s2-thm-1 .statement}

*Cho E là một không gian vectơ tôpô trên một vành chia có định giá không rời rạc. Cho H là một siêu phẳng trong E được xác định bởi phương trình $f(x) = \alpha$ trong đó f là một dạng tuyến tính không đồng nhất bằng 0. Khi đó H đóng trong E nếu và chỉ nếu f liên tục.*

Điều kiện này hiển nhiên là đủ (GT, I, § 2.1, th. 1); ta chứng minh rằng nó là cần. Ta có thể giả sử H là một siêu phẳng thuần nhất đóng với phương trình $f(x) = 0$. Khi đó không gian thương E/H là một không gian vectơ tôpô Hausdorff có chiều 1 trên K. Ta có thể viết $f = g \circ \phi$, trong đó $\phi$ là ánh xạ chính tắc của E lên E/H và g là một ánh xạ tuyến tính của E/H lên $K_s$; theo mệnh đề 2, g liên tục, do đó f cũng liên tục.

#### Hệ quả {#evt-i-s2-n2-cor-1 .statement}

*Mọi dạng tuyến tính liên tục trên E không đồng nhất bằng 0 đều là một cấu xạ ngặt của E lên $K_s$.*
#### Nhận xét {#evt-i-s2-n2-rem-1 .statement}

— Có những ví dụ về các không gian vectơ tôpô chuẩn tắc trên một vành chia có giá trị đầy đủ, không rời rạc, trong đó mọi dạng tuyến tính liên tục đều đồng nhất bằng không (I, p. 25, Bài tập 4); trong một không gian như vậy, do đó, mọi siêu phẳng đều trù mật khắp nơi (I, p. 11, hệ quả).

### 3. Không gian con vectơ có số chiều hữu hạn

#### Định lý 2 {#evt-i-s2-thm-2 .statement}

*Mỗi không gian vectơ tôpô Hausdorff E, có số chiều hữu hạn n, trên một vành chia có giá trị đầy đủ, không rời rạc K, đều đẳng cấu với $K_s^n$; thật vậy, với mỗi cơ sở $(e_i)_{1 \leq i \leq n}$ của E trên K, ánh xạ tuyến tính $(\xi_i) \mapsto \sum_{i=1}^n \xi_i e_i$ là một đẳng cấu của $K_s^n$ lên E.*

Mệnh đề 2 của I, p. 12, suy ra rằng định lý 2 đúng với $n = 1$; ta chứng minh bằng quy nạp theo $n$. Gọi $H$ là không gian con vectơ của $E$ sinh bởi $e_1, e_2, ..., e_{n-1}$; giả thiết quy nạp là ánh xạ $(\xi_i)_{1 \leq i \leq n-1} \mapsto \sum_{i=1}^{n-1} \xi_i e_i$ là một đẳng cấu của $K_s^{n-1}$ lên $H$. Không gian con $H$, vì đẳng cấu với một tích các không gian đầy đủ, nên đầy đủ (GT, II, § 3.5, mệnh đề 10); do đó nó là *đóng* trong $E$ (GT, II, § 3.4, mệnh đề 8). Gọi $D$ là không gian con $Ke_n$ bù với $H$ trong $E$; $E$ là tổng trực tiếp tôpô của $H$ và $D$ (I, p. 13, hệ quả 2), do đó ánh xạ

$$
(\xi_i)_{1 \leq i \leq n} \mapsto \sum_{i=1}^n \xi_i e_i
$$

của $K_s^{n-1} \times K_s$ lên $E$ là một đẳng cấu.

Khi $n > 1$ thì giả thiết rằng $K$ là *đầy đủ* là thiết yếu cho tính đúng đắn của định lý 2. Thật vậy, cho $K$ là một vành chia có giá trị không đầy đủ, và cho $\hat{K}$ là sự hoàn thành của nó : với mỗi $a \neq 0$ của $\hat{K}$ tập $K.a$ trù mật khắp nơi trong $\hat{K}$, vì $x \mapsto xa$ là một đồng phôi của $\hat{K}$ lên chính nó. Nếu $a \notin K$, không gian con $K + Ka$ của không gian vectơ tôpô $\hat{K}$ trên $K$ có số chiều 2 trên $K$, nhưng nó không đẳng cấu với $K_s^2$ vì mọi không gian con có số chiều 1 trong $K + Ka$ đều trù mật trong $K + Ka$.

#### Hệ quả 1 {#evt-i-s2-thm-2-cor-1 .statement}

*Trong một không gian vectơ tôpô Hausdorff $E$ trên một vành chia có giá trị đầy đủ, không rời rạc $K$, mọi không gian con vectơ $F$ có số chiều hữu hạn đều đóng trong $E$.* Thật vậy, nếu $F$ có số chiều $n$ thì nó đẳng cấu với $K_s^n$; do đó nó đầy đủ và suy ra đóng trong $E$ (GT, II, § 3.4, mệnh đề 8).

#### Hệ quả 2 {#evt-i-s2-thm-2-cor-2 .statement}

*Cho $K$ là một vành chia có giá trị đầy đủ, không rời rạc, và $E$ là một không gian vectơ tôpô Hausdorff có số chiều hữu hạn trên $K$. Nếu $F$ là bất kỳ không gian vectơ tôpô nào trên $K$, thì mọi ánh xạ tuyến tính của $E$ vào $F$ đều liên tục.*

#### Hệ quả 3 {#evt-i-s2-thm-2-cor-3 .statement}

*Trong một không gian vectơ tôpô Hausdorff $E$, trên một vành chia có giá trị đầy đủ, không rời rạc, mọi tập độc lập hữu hạn đều độc lập về tôpô.*

#### Hệ quả 4 {#evt-i-s2-thm-2-cor-4 .statement}

==========

*Cho $E$ là một không gian vectơ tôpô trên một vành chia có giá trị đầy đủ không rời rạc. Nếu $M$ là một không gian con vectơ đóng của $E$ và $F$ là một không gian con vectơ của $E$ có số chiều hữu hạn, thì không gian con $M + F$ là đóng trong $E$.*
Viết $\phi$ là đồng cấu chính tắc của $E$ lên không gian thương $E/M$ (tất nhiên là Hausdorff). Khi đó không gian con $M + F$ trùng với $\overline{\phi}^{-1}(\phi(F))$. Bây giờ $\phi(F)$ có số chiều hữu hạn trong $E/M$, do đó (hệ quả 1) $\phi(F)$ đóng trong $E/M$, và suy ra $\overline{\phi}^{-1}(\phi(F))$ đóng trong $E$.

Chú ý rằng, nếu $M$ và $N$ là *bất kỳ* hai không gian con vectơ đóng nào trong một không gian vectơ tôpô Hausdorff $E$, thì $M + N$ không nhất thiết đóng trong $E$, *ngay cả khi $E$ là một không gian Hilbert* (xem IV, p. 64, bài tập 13, d)).

#### Mệnh đề 3 {#evt-i-s2-prop-3 .statement}

*Cho $E$ là một không gian vectơ tôpô trên một vành chia có giá trị đầy đủ, không rời rạc* $K$. Cho $M$ là một không gian con vectơ đóng có đối chiều hữu hạn $n$ trong $E$. Khi đó mọi không gian con $N$ là một bổ trực đại số của $M$ trong $E$ cũng là một bổ trực tôpô.

Trong $N$, tập hợp $\{0\}$ là đóng, vì nó là giao của $N$ và tập hợp $M$ là đóng trong $E$; do đó $N$ là Hausdorff. Vì $E/M$ cũng Hausdorff, ánh xạ chính tắc của $N$ lên $E/M$, là tuyến tính và song ánh, là song tục (I, p. 14, hệ quả 2), từ đó suy ra mệnh đề.

#### Hệ quả {#evt-i-s2-n3-cor-1 .statement}

*Cho $E$ và $F$ là hai không gian vectơ tôpô trên một vành chia có giá trị đầy đủ không rời rạc. Nếu $F$ là Hausdorff và có số chiều hữu hạn, thì mọi ánh xạ tuyến tính liên tục của $E$ lên $F$ đều là một cấu xạ ngặt.*

#### Nhận xét {#evt-i-s2-n3-rem-1 .statement}

— Các kết quả của các số 2, 3 không còn đúng khi $K$ là *rời rạc*. Chẳng hạn, cho $K_1$ là một vành chia có giá trị không rời rạc và cho $K$ là vành chia rời rạc thu được bằng cách trang bị cho $K_1$ giá trị tuyệt đối tầm thường trên $K_1$. Khi đó $K_1$ là một không gian vectơ tôpô có chiều 1 trên $K$, nhưng nó không đẳng cấu với $K_s$. Tuy nhiên, ta có thể chứng minh rằng các kết quả của các số 2, 3 vẫn đúng ngay cả khi $K$ là rời rạc, với điều kiện ta áp đặt lên các không gian vectơ tôpô được xét tính chất có một hệ lân cận cơ bản gồm các lân cận *cân bằng* của 0 (tức là các lân cận $V$ sao cho $K.V = V$) (I, p. 27, bài tập 14); điều kiện này (luôn được thỏa mãn khi $K$ là một vành chia có giá trị không rời rạc *xem* I, p. 7, mệnh đề 4) không đúng đối với mọi không gian vectơ tôpô trên $K$ như ví dụ trên cho thấy.

### 4. Các không gian vectơ tôpô địa phương compact

#### Định lý 3 {#evt-i-s2-thm-3 .statement}

*Cho $K$ là một vành chia có định giá đầy đủ không rời rạc. Nếu $E$ là một không gian vectơ tôpô Hausdorff trên $K$, sao cho tồn tại một lân cận $V$ của 0 trong $E$ là tiền compact, thì $E$ có số chiều hữu hạn. Nếu $E \neq \{0\}$, thì cả $K$ lẫn $E$ đều địa phương compact.*

Khi chứng minh mệnh đề thứ nhất, ta chỉ cần xét trường hợp $E$ là *đầy đủ*; vì $E$ là một không gian con trù mật khắp nơi của sự đầy đủ hóa $\hat{E}$ của nó, và bao đóng $\overline{V}$ của $V$ trong $\hat{E}$ là compact và là một lân cận của 0 trong $\hat{E}$ (GT, III, § 3.4, mệnh đề 7).

Vậy ta có thể giả sử rằng có một lân cận *compact* $V$ của 0 trong $E$. Lấy $\alpha \in K$ sao cho $0 < |\alpha| < 1$; khi đó có hữu hạn điểm $a_i \in V$ sao cho

$$
V \subset \bigcup_i (a_i + \alpha V).
$$

Lấy $M$ là không gian con hữu hạn chiều của $E$ sinh bởi các $a_i$; nó đóng trong $E$ (I, p. 14, hệ quả 1). Trong không gian vectơ tôpô Hausdorff $E/M$, ảnh chính tắc của $V$ là một lân cận compact $W$ của 0, sao cho $W \subset \alpha W$; do đó $\alpha^{-1} W \subset W$, và, theo quy nạp trên $n$, $\alpha^{-n} W \subset W$ với mọi số nguyên dương $n$. Vì $W$ là hấp thụ, suy ra rằng $W = E/M$; và do đó $E/M$ là *compact*. Để hoàn tất chứng minh mệnh đề thứ nhất trong định lý, vì vậy chỉ cần thiết lập bổ đề sau.

#### Bổ đề 1 {#evt-i-s2-lem-1 .statement}

— *Mọi không gian vectơ tôpô compact $E$ trên một vành chia có định giá không rời rạc chỉ là tập $\{0\}$.*

Vì E đầy đủ nên có thể giả sử K đầy đủ (I, p. 6). Nếu E $\neq \{0\}$ thì E chứa một đường thẳng đóng trong E (I, p. 14, hệ quả 1) và do đó compact. Đường thẳng này đẳng cấu với $K_s$ (I, p. 12, mệnh đề 2) và vì thế K phải compact. Bây giờ ánh xạ $\xi \mapsto |\xi|$ của K vào $\mathbf{R}$ là liên tục và do đó ảnh của K phải bị chặn, mặt khác tồn tại $\gamma \in K$ với $|\gamma| > 1$, và tập $|\gamma^n| = |\gamma|^n, n \in \mathbf{N}$, là không bị chặn. Mâu thuẫn này cho thấy rằng $E = \{0\}$.

Để chứng minh mệnh đề thứ hai trong định lý, nếu $E \neq \{0\}$ thì từ phần thứ nhất của định lý E đẳng cấu với $K_s^n$ với $n > 0$; mà K đầy đủ, nên E cũng đầy đủ, và do đó E là địa phương compact. Nhưng $K_s$ đẳng cấu với một đường thẳng trong E (I, p. 12, mệnh đề 2), mà đường thẳng ấy tất yếu đóng trong E (I, p. 14, hệ quả 1); suy ra K là địa phương compact.

#### Nhận xét {#evt-i-s2-n4-rem-1 .statement}

Kết quả của đl. 3 không còn đúng nếu K là một vành chia rời rạc, như được chỉ ra bởi ví dụ của $\mathbf{R}$ (với tôpô thông thường) xét như một không gian vectơ tôpô trên trường rời rạc $\mathbf{Q}$.

### Bài tập {#evt-i-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
