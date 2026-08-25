---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 2
section_title: Identity element; cancellable elements; invertible elements
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0036-0048, 0150-0153
extraction: ocr
subsections:
    - "no": 1
      title: IDENTITY ELEMENT
      page: 0
      pdf_page: 36
    - "no": 2
      title: CANCELABLE ELEMENTS
      page: 0
      pdf_page: 38
    - "no": 3
      title: INVERTIBLE ELEMENTS
      page: 0
      pdf_page: 39
    - "no": 4
      title: MONOID OF FRACTIONS OF A COMMUTATIVE MONOID
      page: 0
      pdf_page: 41
    - "no": 5
      title: 'APPLICATIONS: I. RATIONAL INTEGERS'
      page: 0
      pdf_page: 44
    - "no": 6
      title: 'APPLICATIONS: II. MULTIPLICATION OF RATIONAL INTEGERS'
      page: 0
      pdf_page: 46
    - "no": 7
      title: 'APPLICATIONS: III. GENERALIZED POWERS'
      page: 0
      pdf_page: 47
    - "no": 8
      title: NOTATION
      page: 0
      pdf_page: 47
statements: 25
exercises: 17
content_sha256: 7e32d708614ec6db0d4c3be0995c9892007f8ecc68cfdbe548d415bf96fe2d5d
translated_from: content/en/alg/I/02_s2_identity_element_cancellable_elements.md
source_content_sha256: cc62dde4f620501b1c1bf68a6fda4a9cfec608416078d5f1a3f2dd2034f84283
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-f1e6c316
glossary_version: 34
glossary_terms_sha256: b3baf1190e05d2f919c30f5fe52bf90d6767f1fc54c98c3a76493569ba7e048c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. PHẦN TỬ ĐƠN VỊ; CÁC PHẦN TỬ GIẢN ƯỚC ĐƯỢC; CÁC PHẦN TỬ KHẢ NGHỊCH

### 1. PHẦN TỬ ĐƠN VỊ

#### Định nghĩa 1 {#alg-i-s2-def-1 .statement}

Đối với một luật hợp thành $\top$ trên một tập hợp $E$ một phần tử $e$ của $E$ được gọi là một phần tử đơn vị nếu, với mọi $x \in E$, $e \top x = x \top e = x$.

Tồn tại nhiều nhất một phần tử đơn vị đối với một luật đã cho $\top$, vì nếu $e$ và $e'$ là các phần tử đơn vị thì $e = e \top e' = e'$. Một phần tử đơn vị giao hoán được với mọi phần tử: nó là một phần tử trung tâm.

#### Định nghĩa 2 {#alg-i-s2-def-2 .statement}

Một magma có một phần tử đơn vị được gọi là một magma có đơn vị. Nếu $E, E'$ là các magma có đơn vị, một đồng cấu của magma $E$ vào magma $E'$ biến phần tử đơn vị của $E$ thành phần tử đơn vị của $E'$ được gọi là một đồng cấu có đơn vị (hoặc cấu xạ) của $E$ vào $E'$. Một magma kết hợp có đơn vị được gọi là một monođ.

Nếu $E, E'$ là các monođ, một cấu xạ có đơn vị của $E$ vào $E'$ được gọi là một đồng cấu monođ hoặc một cấu xạ monođ của $E$ vào $E'$.

#### Ví dụ {#alg-i-s2-n1-exa-1 .statement}

(1) Trong tập hợp $\mathbf{N}$ các số tự nhiên, 0 là một phần tử đơn vị đối với phép cộng và 1 là một phần tử đơn vị đối với phép nhân. Mỗi một trong hai luật này cho $\mathbf{N}$ một cấu trúc monođ giao hoán (Lý thuyết tập hợp, III, § 3, no. 3).

(2) Trong tập hợp các tập con của một tập hợp $E$, $\varnothing$ là một phần tử đơn vị đối với luật $\cup$ và $E$ đối với luật $\cap$. Nói chung, trong một dàn, phần tử nhỏ nhất, nếu tồn tại, là phần tử đơn vị đối với luật sup; ngược lại, nếu tồn tại một phần tử đơn vị đối với luật này thì nó là phần tử nhỏ nhất của tập hợp. Tương tự đối với phần tử lớn nhất và luật inf.

(3) Tập hợp $\mathbf{N}$ không có phần tử đơn vị đối với luật $(x, y) \mapsto x^y$. Đối với luật $(X, Y) \mapsto X \circ Y$ giữa các tập con của $E \times E$ đường chéo $\Delta$ là phần tử đơn vị. Đối với luật $(f, g) \mapsto f \circ g$ giữa các ánh xạ của $E$ vào $E$, ánh xạ đồng nhất của $E$ lên $E$ là phần tử đơn vị.

(4) Cho $E$ là một magma và $R$ là một quan hệ tương đương trên $E$ tương thích với luật trên $E$ (\S 1, no. 6). Nếu $e$ là một phần tử đơn vị của $E$ thì ảnh chính tắc của $e$ trong $E/R$ là một phần tử đơn vị của magma $E/R$.

Phần tử đơn vị của một magma có đơn vị là một đồng cấu có đơn vị; hợp thành của hai đồng cấu có đơn vị cũng là một đồng cấu có đơn vị. Để một ánh xạ là một đẳng cấu magma có đơn vị, điều kiện cần và đủ là nó là một đồng cấu có đơn vị song ánh và khi đó ánh xạ nghịch đảo là một đồng cấu có đơn vị. Cho $E$ và $E'$ là các magma có đơn vị và $e'$ là phần tử đơn vị của $E'$; ánh xạ hằng của $E$ vào $E'$ biến $E$ thành $e'$ là một đồng cấu có đơn vị, được gọi là một đồng cấu tầm thường.

Tích của một họ các magma có đơn vị (tương ứng, monođ) là một magma có đơn vị (tương ứng, monođ).

Mọi magma thương của một magma có đơn vị (tương ứng, monođ) đều là một magma có đơn vị (tương ứng, monođ).

Cho $E$ là một magma có đơn vị và $e$ là phần tử đơn vị của nó. Một magma con $A$ của $E$ sao cho $e \in A$ được gọi là một magma con có đơn vị của $E$. Rõ ràng $e$ là phần tử đơn vị của magma $A$. Mọi giao của các magma con có đơn vị của $E$ đều là một magma con có đơn vị của $E$. Nếu $X$ là một tập con của $E$ thì tồn tại một magma con có đơn vị nhỏ nhất của $E$ chứa $X$; nó được gọi là magma con có đơn vị của $E$ sinh bởi $X$; nó bằng $\{e\}$ nếu $X$ là rỗng. Nếu $E$ là một monoid, một magma con có đơn vị của $E$ được gọi là một monoid con của $E$.

Nếu $F$ là một magma không có phần tử đơn vị thì một magma con của $F$ có thể có một phần tử đơn vị. Ví dụ, nếu $F$ là kết hợp và $h$ là một phần tử lũy đẳng của $F$ (I, § 1, no. 4), tập hợp $h \uparrow x \uparrow h$, trong đó $x$ chạy qua $F$, là một magma con của $F$ với $h$ là phần tử đơn vị.

Nếu $E$ là một magma có phần tử đơn vị $e$, một magma con $A$ của $E$ sao cho $e \notin A$ vẫn có thể có một phần tử đơn vị.

#### Định nghĩa 3 {#alg-i-s2-def-3 .statement}

Cho $E$ là một magma có đơn vị. Phần tử đơn vị của $E$ được gọi là hợp thành của họ rỗng các phần tử của $E$.

Nếu $(x_\alpha)_{\alpha \in \varnothing}$ là họ rỗng các phần tử của E thì hợp thành của nó $e$ còn được ký hiệu bởi $\prod_{\alpha \in \varnothing} x_\alpha$. Ví dụ, ta viết
$$
\prod_{q \leq i \leq p} x_i = e
$$
khi $p < q$ ($p, q \in \mathbf{N}$). Tương tự ta viết $\prod^0 x = e$ với $x$ tùy ý. *Với các định nghĩa này, các Định lý 1 và 3 của § 1 vẫn đúng nếu bỏ giả thiết rằng các tập hợp A và B_i là không rỗng.* Tương tự, các công thức $\prod^{m+n} x = \left( \prod^m x \right) \prod^n \left( \prod^n x \right)$ và $\prod^{mn} x = \prod^m \left( \prod^n x \right)$ khi đó đúng với $m \geq 0, n \geq 0$.

Cho E là một magma có đơn vị mà luật của nó được ký hiệu bởi $\top$ và $e$ là phần tử đơn vị của nó. *Giá* của một họ $(x_i)_{i \in I}$ các phần tử của E là tập hợp các chỉ số $i \in I$ sao cho $x_i \neq e$. Cho $(x_i)_{i \in I}$ là một họ các phần tử của E *có giá hữu hạn*. Ta sẽ định nghĩa hợp thành $\prod_{i \in I} x_i$ trong hai trường hợp sau:

(a) tập hợp I được sắp thứ tự toàn phần;
(b) E là kết hợp và các $x_i$ từng đôi một giao hoán.

Trong hai trường hợp này, gọi S là giá của họ $(x_i)$. Nếu J là một tập con hữu hạn của I chứa S, thì $\prod_{i \in J} x_i = \prod_{i \in S} x_i$, như được thấy bằng quy nạp theo số các phần tử của J, áp dụng Định lý 1 của § 1 trong trường hợp (a) và Định lý 3 của § 1 trong trường hợp (b). Ký hiệu $\prod_{i \in I} x_i$ là giá trị chung của các hợp thành $\prod_{i \in J} x_i$ đối với mọi tập con hữu hạn của I chứa S. Khi I là khoảng $[p, \to]$ của $\mathbf{N}$, ta cũng viết $\prod_{i = p}^\infty x_i$.

Với các định nghĩa và ký hiệu này, các Định lý 1 và 3 của § 1 và các nhận xét theo sau Định lý 3 mở rộng cho các họ có giá hữu hạn.

Phần tử đơn vị của một luật được viết *cộng tính* thường được ký hiệu bởi 0 và gọi là *không* hoặc *phần tử không* (hoặc đôi khi là *gốc*). Đối với một luật được viết *nhân tính*, nó thường được ký hiệu bởi 1 và gọi là *phần tử đơn vị* (hoặc *đơn vị*).

### 2. CÁC PHẦN TỬ GIẢN ƯỚC ĐƯỢC

#### Định nghĩa 4 {#alg-i-s2-def-4 .statement}

*Cho một luật hợp thành $\top$ trên một tập hợp E, ánh xạ $x \mapsto a \top x$ (tương ứng $x \mapsto x \top a$) từ E vào chính nó được gọi là phép chuyển trái (tương ứng phép chuyển phải) bởi một phần tử $a \in E$.*

Khi chuyển qua luật đối, các phép chuyển trái trở thành các phép chuyển phải và ngược lại.

Gọi $\gamma_a, \delta_a$ (hoặc $\gamma(a), \delta(a)$) là các phép chuyển trái và phải bởi $a \in E$; khi đó
$$
\gamma_a(x) = a \top x, \qquad \delta_a(x) = x \top a.
$$

#### Mệnh đề 1 {#alg-i-s2-prop-1 .statement}

*Nếu luật* $\mathsf{T}$ *là kết hợp, thì với mọi* $x \in E$ *và* $y \in E$

$$
\gamma_{x \mathsf{T} y} = \gamma_x \circ \gamma_y, \qquad \delta_{x \mathsf{T} y} = \delta_y \circ \delta_x.
$$

Với mọi $z \in E$:

$$
\gamma_{x \mathsf{T} y}(z) = (x \mathsf{T} y) \mathsf{T} z = x \mathsf{T} (y \mathsf{T} z) = \gamma_x(\gamma_y(z))
$$
$$
\delta_{x \mathsf{T} y}(z) = z \mathsf{T} (x \mathsf{T} y) = (z \mathsf{T} x) \mathsf{T} y = \delta_y(\delta_x(z))
$$

Nói cách khác, ánh xạ $x \mapsto \gamma_x$ là một đồng cấu từ magma $E$ vào tập hợp $E^E$ các ánh xạ của $E$ vào chính nó với luật $(f, g) \mapsto f \circ g$; ánh xạ $x \mapsto \delta_x$ là một đồng cấu của $E$ vào tập hợp $E^E$ với luật đối. Nếu $E$ là một monoid, các đồng cấu này có đơn vị.

#### Định nghĩa 5 {#alg-i-s2-def-5 .statement}

*Một phần tử* $a$ *của một magma* $E$ *được gọi là giản ước được trái (tương ứng phải) (hoặc chính quy) nếu phép chuyển trái (tương ứng phải) bởi* $a$ *là đơn ánh. Một phần tử giản ước được trái và phải được gọi là một phần tử giản ước được (hoặc chính quy).*

Nói cách khác, để $a$ giản ước được theo luật $\mathsf{T}$, điều kiện cần và đủ là mỗi quan hệ $a \mathsf{T} x = a \mathsf{T} y, x \mathsf{T} a = y \mathsf{T} a$ kéo theo $x = y$ (người ta nói rằng "a có thể được giản ước" khỏi mỗi đẳng thức này). Nếu tồn tại một phần tử đơn vị $e$ theo luật $\mathsf{T}$, thì nó giản ước được theo luật này: khi đó các phép chuyển $\gamma_e$ và $\delta_e$ là ánh xạ đồng nhất của $E$ lên chính nó.

#### Ví dụ {#alg-i-s2-n2-exa-1 .statement}

(1) Mọi số tự nhiên đều giản ước được theo phép cộng; mọi số tự nhiên $\neq 0$ đều giản ước được theo phép nhân.

(2) Trong một dàn không thể có phần tử giản ước được nào theo luật sup ngoài phần tử đơn vị (phần tử nhỏ nhất) nếu nó tồn tại; tương tự đối với inf. Đặc biệt, trong tập hợp các tập con của một tập hợp $E$, $\varnothing$ là phần tử giản ước được duy nhất theo luật $\cup$ và $E$ là phần tử giản ước được duy nhất theo luật $\cap$.

#### Mệnh đề 2 {#alg-i-s2-prop-2 .statement}

*Tập hợp các phần tử giản ước được (tương ứng trái giản ước được, tương ứng phải giản ước được) của một magma kết hợp là một magma con.*

Nếu $\gamma_x$ và $\gamma_y$ là đơn ánh thì $\gamma_{x \mathsf{T} y} = \gamma_x \circ \gamma_y$ cũng là đơn ánh (Mệnh đề 1). Tương tự đối với $\delta_{x \mathsf{T} y}$.

### 3. CÁC PHẦN TỬ KHẢ NGHỊCH

#### Định nghĩa 6 {#alg-i-s2-def-6 .statement}

*Cho* $E$ *là một magma có đơn vị, $\mathsf{T}$ là luật hợp thành của nó, e là phần tử đơn vị của nó và* $x$ *và* $x'$ *là hai phần tử của* $E$. $x'$ *được gọi là một nghịch đảo trái (tương ứng nghịch đảo phải, tương ứng nghịch đảo) của* $x$ *nếu* $x' \mathsf{T} x = e$ *(tương ứng $x \mathsf{T} x' = e$, tương ứng $x' \mathsf{T} x = x \mathsf{T} x' = e$).*

*Một phần tử* $x$ *của* $E$ *được gọi là khả nghịch trái (tương ứng khả nghịch phải, tương ứng khả nghịch) nếu nó có một nghịch đảo trái (tương ứng nghịch đảo phải, tương ứng nghịch đảo).*

*Một monoid mà mọi phần tử đều khả nghịch được gọi là một nhóm.*

Đối xứng và đối xứng hóa đôi khi được dùng thay cho nghịch đảo và khả nghịch. Khi luật trên E được viết cộng tính, nói chung ta nói là âm thay cho nghịch đảo.

#### Ví dụ {#alg-i-s2-n3-exa-1 .statement}

(1) Một phần tử đơn vị là nghịch đảo của chính nó.

(2) Trong tập hợp các ánh xạ từ E vào E, một phần tử f là khả nghịch trái (tương ứng khả nghịch phải) nếu f là một toàn ánh (tương ứng đơn ánh). Khi đó các nghịch đảo trái (tương ứng nghịch đảo phải) là các phép rút (tương ứng các thiết diện) liên kết với f (Lý thuyết tập hợp, II, § 3, no. 8, Định nghĩa 11). Để f khả nghịch, điều kiện cần và đủ là f là một song ánh. Khi đó nghịch đảo duy nhất của nó là song ánh ngược của f.

Cho E và F là hai magma có đơn vị và f là một đồng cấu có đơn vị từ E vào F. Nếu x' là nghịch đảo của x trong E, thì f(x') là nghịch đảo của f(x) trong F. Do đó, nếu x là một phần tử khả nghịch của E, thì f(x) là một phần tử khả nghịch của F.

Đặc biệt, nếu R là một quan hệ tương đương tương thích với luật trên một magma có đơn vị E, thì ảnh chính tắc của một phần tử khả nghịch của E là khả nghịch trong E/R.

#### Mệnh đề 3 {#alg-i-s2-prop-3 .statement}

Cho E là một monoid và x là một phần tử của E.

(i) Để x khả nghịch trái (tương ứng phải), điều kiện cần và đủ là phép tịnh tiến phải (tương ứng trái) bởi x là toàn ánh.

(ii) Để x khả nghịch, điều kiện cần và đủ là nó khả nghịch trái và phải. Trong trường hợp đó x có một nghịch đảo duy nhất, cũng là nghịch đảo trái (tương ứng phải) duy nhất của nó.

Nếu x' là một nghịch đảo trái của x thì (Mệnh đề 1)

$$
\delta_x \circ \delta_{x'} = \delta_{x' \top x} = \delta_e = \mathrm{Id}_E
$$

và $\delta_x$ là toàn ánh. Ngược lại, nếu $\delta_x$ là toàn ánh, tồn tại một phần tử $x'$ của E sao cho $\delta_x(x') = e$ và $x'$ là nghịch đảo trái của $x$. Các khẳng định khác của (i) được suy ra tương tự.

Nếu $x'$ (tương ứng $x''$) là một nghịch đảo trái (tương ứng phải) của $x$, thì

$$
x' = x' \top e = x' \top (x \top x'') = (x' \top x) \top x'' = e \top x'' = x'',
$$

do đó (ii).

#### Nhận xét {#alg-i-s2-n3-rem-1 .statement}

Cho E là một monoid và x là một phần tử của E. Nếu x khả nghịch trái thì nó giản ước trái được; vì, nếu $x'$ là một nghịch đảo trái của $x$, thì

$$
\gamma_{x'} \circ \gamma_x = \gamma_{x' \top x} = \gamma_e = \mathrm{Id}_E
$$

và $\gamma_x$ là đơn ánh. Đặc biệt, nếu x khả nghịch trái, các phép tịnh tiến trái và phải bởi x là các song ánh. Ngược lại, giả sử rằng $\gamma_x$ là song ánh; tồn tại $x' \in E$ sao cho $xx' = \gamma_x(x') = e$; khi đó $\gamma_x(x'x) = (xx')x = x = \gamma_x(e)$ và do đó $x'x = e$, vậy x là khả nghịch. Tương tự ta thấy rằng nếu $\delta_x$ là song ánh thì x là khả nghịch.

#### Mệnh đề 4 {#alg-i-s2-prop-4 .statement}

Cho E là một monoid và x và y là các phần tử khả nghịch của E với các nghịch đảo lần lượt là x' và y'. Khi đó y' $\top$ x' là nghịch đảo của x $\top$ y.

Điều này suy ra từ quan hệ
$$
(y' \top x') \top (x \top y) = y' \top (x' \top x) \top y = y' \top y = e
$$
và các tính toán tương tự đối với (x $\top$ y) $\top$ (y' $\top$ x').

#### Hệ quả 1 {#alg-i-s2-prop-4-cor-1 .statement}

Cho E là một monoid; nếu mỗi phần tử $x_\alpha$ của một dãy có thứ tự $(x_\alpha)_{\alpha \in A}$ gồm các phần tử của E có một nghịch đảo $x'_\alpha$, thì hợp thành $\prod_{\alpha \in A} x_\alpha$ có nghịch đảo $\prod_{\alpha \in A'} x'_\alpha$, trong đó A' là tập sắp thứ tự toàn phần dẫn xuất từ A bằng cách thay thế thứ tự trên A bởi thứ tự đối.

Hệ quả này suy ra từ Mệnh đề 4 bằng quy nạp theo số phần tử của A.

Đặc biệt, nếu x và x' là các nghịch đảo, $\prod^n x$ và $\prod^n x'$ là các nghịch đảo với mọi số nguyên $n \geq 0$.

#### Hệ quả 2 {#alg-i-s2-prop-4-cor-2 .statement}

Trong một monoid, tập hợp các phần tử khả nghịch là ổn định.

#### Mệnh đề 5 {#alg-i-s2-prop-5 .statement}

Nếu trong một monoid x và x' là các nghịch đảo và x giao hoán với y, thì x' cũng vậy.

Từ $x \top y = y \top x$, ta suy ra $x' \top (x \top y) \top x' = x' \top (y \top x) \top x'$ và do đó $(x' \top x) \top (y \top x') = (x' \top y) \top (x \top x')$, nghĩa là $y \top x' = x' \top y$.

#### Hệ quả 1 {#alg-i-s2-prop-5-cor-1 .statement}

Cho E là một monoid, X là một tập con của E và X' là bộ giao hoán hóa của X. Nghịch đảo của mọi phần tử khả nghịch của X' thuộc X'.

#### Hệ quả 2 {#alg-i-s2-prop-5-cor-2 .statement}

Trong một monoid, nghịch đảo của một phần tử khả nghịch trung tâm là một phần tử trung tâm.

### 4. MONOID PHÂN THỨC CỦA MỘT MONOID GIAO HOÁN

Trong số này, e sẽ ký hiệu phần tử đơn vị của một monoid và x* là nghịch đảo của một phần tử khả nghịch x của E.

Cho E là một monoid giao hoán, S là một tập con của E và S' là monoid con của E sinh bởi S.

#### Bổ đề 1 {#alg-i-s2-lem-1 .statement}

Trong E $\times$ S', quan hệ R$\mathcal{R}$x, y$\mathcal{R}$ được xác định bởi:

"tồn tại $a, b \in E$ và $p, q, s \in S'$ sao cho $x = (a, p), y = (b, q)$ và $aqs = bps$"

là một quan hệ tương đương tương thích với luật trên monoid tích E $\times$ S'.

Hiển nhiên là R có tính phản xạ và đối xứng. Cho $x = (a, p), y = (b, q)$ và $z = (c, r)$ là các phần tử của E $\times$ S' sao cho R$\mathcal{R}$x, y$\mathcal{R}$ và R$\mathcal{R}$y, z$\mathcal{R}$ đúng. Khi đó tồn tại hai phần tử s và t của S' sao cho
$$
aq s = bps, \quad br t = cqt,
$$
do đó suy ra
$$
ar(stq) = bpsrt = cp(stq)
$$

và do đó $R \{ x, z \}$ đúng, vì $stq$ thuộc $S'$. Quan hệ $R$ vì vậy là bắc cầu.

Hơn nữa, cho $x = (a, p), y = (b, q), x' = (a', p'),$ và $y' = (b', q')$ là các phần tử của $E \times S'$ sao cho $R \{ x, y \}$ và $R \{ x', y' \}$ đúng. Tồn tại $s$ và $s'$ trong $S'$ sao cho
$$
aqs = bps, \qquad a'q's' = b'p's',
$$
do đó suy ra $(aa')(qq')(ss') = (bb')(pp')(ss')$ và do đó $R \{ xx', yy' \}$ vì $ss' \in S'$. Quan hệ tương đương $R$ vì vậy tương thích với luật hợp thành trên $E \times S'$.

Magm thương $(E \times S')/R$ là một monoid giao hoán.

#### Định nghĩa 7 {#alg-i-s2-def-7 .statement}

*Cho $E$ là một monoid giao hoán, $S$ là một tập con của $E$ và $S'$ là monoid con của $E$ sinh bởi $S$. Monoid thương $(E \times S')/R$, trong đó quan hệ tương đương $R$ được mô tả như trong Bổ đề 1, được ký hiệu là $E_S$ và được gọi là monoid phân thức† của $E$ liên kết với $S$ (hay với các mẫu số trong $S$).*

Với $a \in E$ và $p \in S'$, lớp của $(a, p)$ modulo $R$ nói chung được ký hiệu là $a/p$ và được gọi là phân thức có tử số $a$ và mẫu số $p$. Khi đó theo định nghĩa $(a/p).(a'/|p') = aa'/|pp'$. Các phân thức $a/p$ và $a'/|p'$ bằng nhau khi và chỉ khi tồn tại $s$ trong $S'$ sao cho $spa' = sp'a$; nếu vậy, tồn tại $\sigma$ và $\sigma'$ trong $S'$ sao cho $a\sigma = a'\sigma'$ và $p\sigma = p'\sigma'$. Đặc biệt, $a/p = sa/sp$ với $a \in E$ và $s, p$ trong $S'$. Phần tử đơn vị của $E_S$ là phân thức $e/e$.

Cho $a/e = \varepsilon(a)$ với mọi $a \in E$. Điều trên cho thấy rằng $\varepsilon$ là một đồng cấu từ $E$ vào $E_S$, được gọi là chính tắc. Với mọi $p \in S'$, $(p/e).(e/p) = e/e$ và do đó $e/p$ là nghịch đảo của $\varepsilon(p) = p/e$; mọi phần tử của $\varepsilon(S')$ vì vậy đều khả nghịch. Khi đó $a/p = (a/e).(e/p)$, do đó
$$
a/p = \varepsilon(a)\varepsilon(p)^*
$$
với $a \in E$ và $p \in S'$, monoid $E_S$ vì vậy được sinh bởi $\varepsilon(E) \cup \varepsilon(S)^*$.

#### Mệnh đề 6 {#alg-i-s2-prop-6 .statement}

*Ký hiệu là ký hiệu của Định nghĩa 7 và $\varepsilon$ biểu thị đồng cấu chính tắc của $E$ vào $E_S$.
(i) Cho $a$ và $b$ thuộc $E$; để có $\varepsilon(a) = \varepsilon(b)$, điều kiện cần và đủ là tồn tại $s \in S'$ sao cho $sa = sb$.
(ii) Để $\varepsilon$ đơn ánh, điều kiện cần và đủ là mọi phần tử của $S$ đều giản ước được.
(iii) Để $\varepsilon$ song ánh, điều kiện cần và đủ là mọi phần tử của $S$ đều khả nghịch.*

Mệnh đề (i) là hiển nhiên và cho thấy rằng $\varepsilon$ đơn ánh khi và chỉ khi mọi phần tử của $S'$ đều giản ước được; nhưng vì tập hợp các phần tử giản ước được của $E$ là một monoid con của $E$ (no. 2, Mệnh đề 2), điều đó cũng tương đương với việc nói rằng mọi phần tử của $S$ đều giản ước được.

† Nó cũng được gọi là *monoid hiệu* nếu luật trên $E$ được viết theo phép cộng.

Nếu $\varepsilon$ là song ánh thì mọi phần tử của S đều khả nghịch, vì $\varepsilon(S)$ được tạo thành bởi các phần tử khả nghịch của $E_S$. Ngược lại, giả sử mọi phần tử của S đều khả nghịch; khi đó mọi phần tử của $S'$ đều khả nghịch (no. 3, Hệ quả 2 của Mệnh đề 4) và do đó giản ước được. Khi đó $\varepsilon$ là đơn ánh theo (ii) và $a/p = \varepsilon(a.p^*)$ theo (1), do đó $\varepsilon$ là toàn ánh.

#### Định lý 1 {#alg-i-s2-thm-1 .statement}

*Cho E là một nửa nhóm giao hoán, S là một tập con của E, $E_S$ là nửa nhóm các phân thức liên kết với S và $\varepsilon : E \to E_S$ là đồng cấu chính tắc. Ngoài ra, cho f là một đồng cấu từ E vào một nửa nhóm F (không nhất thiết giao hoán) sao cho mọi phần tử của $f(S)$ đều khả nghịch trong F. Tồn tại duy nhất một đồng cấu $\bar{f}$ từ $E_S$ vào F sao cho $f = \bar{f} \circ \varepsilon$.*

Nếu $\bar{f}$ là một đồng cấu từ $E_S$ vào F sao cho $f = \bar{f} \circ \varepsilon$, thì
$$
\bar{f}(a/p) = \bar{f}(\varepsilon(a)\varepsilon(p)^*) = \bar{f}(\varepsilon(a))\bar{f}(\varepsilon(p))^* = f(a)f(p)^*
$$
với $a \in E$ và $p \in S'$, do đó tính duy nhất của $\bar{f}$.

Cho g là ánh xạ từ $E \times S'$ vào F được xác định bởi $g(a,p) = f(a)f(p)^*$. Ta chứng minh rằng g là một đồng cấu từ $E \times S'$ vào F. Trước hết,
$$
g(e,e) = f(e)f(e)^* = e.
$$
Cho $(a,p)$ và $(a',p')$ là hai phần tử của $E \times S'$; vì $a'$ và $p$ giao hoán trong E, nên $f(a')$ và $f(p)$ giao hoán trong F, do đó $f(a')f(p)^* = f(p)^*f(a')$ theo no. 3, Mệnh đề 5. Hơn nữa $f(pp')^* = f(p'p)^* = (f(p')f(p))^* = f(p)^*f(p')^*$ theo no. 3, Mệnh đề 4, do đó
$$
g(aa',pp') = f(aa')f(pp')^* = f(a)f(a')f(p)^*f(p')^* = f(a)f(p)^*f(a')f(p')^*
= g(a,p)g(a',p').
$$
Ta chứng minh rằng g tương thích với quan hệ tương đương R trên $E \times S'$: nếu $(a,p)$ và $(a',p')$ đồng dư mod. R, thì tồn tại $s \in S'$ sao cho $spa' = sap'$, do đó $f(s)f(p)f(a') = f(s)f(a)f(p')$. Vì $f(s)$ khả nghịch, suy ra $f(p)f(a') = f(a)f(p')$ và khi đó bằng phép nhân bên trái với $f(p)^*$ và phép nhân bên phải với $f(p')^*$
$$
g(a',p') = f(a')f(p')^* = f(p)^*f(a) = f(a)f(p)^* = g(a,p).
$$
Do đó tồn tại một đồng cấu $\bar{f}$ từ $E_S$ vào F sao cho $\bar{f}(a/p) = g(a,p)$, do đó $\bar{f}(\varepsilon(a)) = \bar{f}(a/e) = f(a)f(e)^* = f(a)$. Suy ra $\bar{f} \circ \varepsilon = f$.

#### Hệ quả {#alg-i-s2-n4-cor-1 .statement}

*Cho E và F là hai nửa nhóm giao hoán, S và T lần lượt là các tập con của E và F, f là một đồng cấu từ E vào F sao cho $f(S) \subset T$ và $\varepsilon : E \to E_S, \eta : F \to F_T$ là các đồng cấu chính tắc. Tồn tại duy nhất một đồng cấu $g : E_S \to F_T$ sao cho $g \circ \varepsilon = \eta \circ f$.*

Đồng cấu $\eta \circ f$ từ E vào $F_T$ ánh xạ mọi phần tử của S thành một phần tử khả nghịch của $F_T$.

(2) Để tồn tại nghiệm của bài toán ánh xạ phổ quát trên, không cần thiết phải giả sử nửa nhóm E là giao hoán, như suy ra từ *Lý thuyết tập hợp*, IV, § 3, no. 2 (cf. Bài tập 17).

Ta nêu hai trường hợp đặc biệt quan trọng của các nửa nhóm phân thức.

(a) Cho $\overline{E} = E_E$. Vì monoid $\overline{E}$ được sinh bởi tập hợp $\varepsilon(E) \cup \varepsilon(E)^*$, vốn gồm các phần tử khả nghịch, nên mọi phần tử của $\overline{E}$ đều khả nghịch (no. 3, Hệ quả 2 của Mệnh đề 4). Nói cách khác, $\overline{E}$ là một nhóm giao hoán. Hơn nữa, theo Định lý 1, mọi đồng cấu $f$ của E vào một nhóm G đều được phân tích duy nhất dưới dạng $f = \bar{f} \circ \varepsilon$, trong đó $\bar{f}: \overline{E} \to G$ là một đồng cấu. $\overline{E}$ được gọi là *nhóm các phân thức của* E (hay *nhóm các hiệu của* E trong trường hợp dùng ký hiệu cộng).

(b) Đặt $\Phi = E_{\Sigma}$, trong đó $\Sigma$ gồm các phần tử giản ước được của E. Theo Mệnh đề 6, (ii), đồng cấu chính tắc của E vào $\Phi$ là đơn ánh; ta sẽ đồng nhất E với ảnh của nó trong $\Phi$. Do đó E là một monoid con của $\Phi$, mọi phần tử giản ước được của E đều có một phần tử nghịch đảo trong $\Phi$ và mọi phần tử của $\Phi$ đều có dạng $a/p = a.p^*$ với $a \in E$ và $p \in \Sigma$; khi đó $a/p = a'/p'$ khi và chỉ khi $ap' = pa'$. Dễ thấy các phần tử khả nghịch của $\Phi$ là các phân thức $a/p$, trong đó $a$ và $p$ đều giản ước được, và $p/a$ là nghịch đảo của $a/p$.

Bây giờ cho S là một tập hợp các phần tử giản ước được của E và $S'$ là monoid con của E được sinh bởi S. Nếu $a/p$ và $a'/p'$ là hai phần tử của $E_S$, thì $a/p = a'/p'$ khi và chỉ khi $ap' = pa'$ (vì $sap' = spa'$ suy ra $ap' = pa'$ với mọi $s \in S'$). Do đó $E_S$ có thể được đồng nhất với monoid con của $\Phi$ được sinh bởi $E \cup S^*$.

Nếu mọi phần tử của E đều giản ước được, thì $\Phi = \overline{E}$ và E là một monoid con của nhóm giao hoán $\Phi$. Ngược lại, nếu E đẳng cấu với một monoid con của một nhóm, thì mọi phần tử của E đều giản ước được.

### 5. ỨNG DỤNG: I. CÁC SỐ NGUYÊN HỮU TỈ

Xét monoid giao hoán $\mathbf{N}$ của các số tự nhiên với luật hợp thành là phép cộng; mọi phần tử của $\mathbf{N}$ đều giản ước được theo luật này (*Lý thuyết tập hợp*, III, § 5, no. 2, Hệ quả 3). Nhóm hiệu của $\mathbf{N}$ được ký hiệu bởi $\mathbf{Z}$; các phần tử của nó được gọi là *các số nguyên hữu tỉ*; luật của nó được gọi là *phép cộng các số nguyên hữu tỉ* và cũng được ký hiệu bởi +. Đồng cấu chính tắc từ $\mathbf{N}$ vào $\mathbf{Z}$ là đơn ánh và ta sẽ đồng nhất mỗi phần tử của $\mathbf{N}$ với ảnh của nó trong $\mathbf{Z}$. Theo định nghĩa, các phần tử của $\mathbf{Z}$ là các lớp tương đương được xác định trong $\mathbf{N} \times \mathbf{N}$ bởi quan hệ giữa $(m_1, n_1)$ và $(m_2, n_2)$ được viết là $m_1 + n_2 = m_2 + n_1$; một phần tử $m$ của $\mathbf{N}$ được đồng nhất với lớp gồm các phần tử $(m + n, n)$, trong đó $n \in \mathbf{N}$; nó có trong $\mathbf{Z}$ phần tử đối là lớp gồm các phần tử $(n, m + n)$. Mọi phần tử $(p, q)$ của $\mathbf{N} \times \mathbf{N}$ đều có thể viết dưới dạng $(m + n, n)$ nếu $p \geq q$ hoặc dưới dạng $(n, m + n)$ nếu $p \leq q$; suy ra rằng $\mathbf{Z}$ là *hợp của $\mathbf{N}$ và tập hợp các phần tử đối của các phần tử của $\mathbf{N}$*. Phần tử đơn vị 0 là phần tử duy nhất của $\mathbf{N}$ mà phần tử đối của nó thuộc $\mathbf{N}$.

Với mọi số tự nhiên $m$, $-m$ ký hiệu số nguyên hữu tỉ đối của $m$ và $-\mathbf{N}$ ký hiệu tập hợp các phần tử $-m$ với $m \in \mathbf{N}$. Khi đó

$$
\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N}) \quad \text{và} \quad \mathbf{N} \cap (-\mathbf{N}) = \{0\}.
$$

với $m \in \mathbf{N}$, $m = -m$ khi và chỉ khi $m = 0$.

Cho $m$ và $n$ là hai số tự nhiên;

(a) nếu $m \geq n$, thì $m + (-n) = p$, trong đó $p$ là phần tử của $\mathbf{N}$ sao cho $m = n + p$;
(b) nếu $m \leq n$, thì $m + (-n) = -p$, trong đó $p$ là phần tử của $\mathbf{N}$ sao cho $m + p = n$;
(c) $(-m) + (-n) = -(m + n)$.

Các tính chất (b) và (c) suy ra từ no. 3, Mệnh đề 4; vì $\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$, phép cộng trong $\mathbf{N}$ và các tính chất (a), (b) và (c) mô tả hoàn toàn phép cộng trong $\mathbf{Z}$.

Tổng quát hơn, $-x$ được dùng để ký hiệu phần tử đối của một số nguyên hữu tỉ tùy ý $x$; hợp thành $x + (-y)$ được viết tắt thành $x - y$ (xem no. 8).

Quan hệ thứ tự $\leq$ giữa các số tự nhiên được đặc trưng bởi tính chất sau: $m \leq n$ khi và chỉ khi tồn tại một số nguyên $p \in \mathbf{N}$ sao cho $m + p = n$ (*Lý thuyết tập hợp*, III, § 3, no. 6, Mệnh đề 13 và § 5, no. 2, Mệnh đề 2). Quan hệ $y - x \in \mathbf{N}$ giữa các số nguyên hữu tỉ $x$ và $y$ là một quan hệ *thứ tự toàn phần* trên $\mathbf{Z}$ mở rộng quan hệ thứ tự $\leq$ trên $\mathbf{N}$. Thật vậy, với mọi $x \in \mathbf{Z}$, $x - x = 0 \in \mathbf{N}$; nếu $y - x \in \mathbf{N}$ và $z - y \in \mathbf{N}$, thì

$$
z - x = (z - y) + (y - x) \in \mathbf{N},
$$

vì $\mathbf{N}$ ổn định đối với phép cộng; nếu $y - x \in \mathbf{N}$ và $x - y \in \mathbf{N}$, thì $y - x = 0$, vì 0 là phần tử duy nhất của $\mathbf{N}$ mà số đối của nó thuộc $\mathbf{N}$; với các số nguyên hữu tỉ tùy ý $x$ và $y$, $y - x \in \mathbf{N}$ hoặc $x - y \in \mathbf{N}$, vì $\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$; cuối cùng, nếu $x$ và $y$ là các số tự nhiên, thì $y - x \in \mathbf{N}$ khi và chỉ khi tồn tại $p \in \mathbf{N}$ sao cho $x + p = y$. Quan hệ thứ tự này cũng được ký hiệu bởi $\leq$.

Từ nay về sau, khi $\mathbf{Z}$ được xét như một tập hợp có thứ tự, nếu không có nói gì khác, nó sẽ luôn được trang bị quan hệ thứ tự vừa định nghĩa, các số tự nhiên được đồng nhất với các số nguyên $\geq 0$; chúng cũng được gọi là các số nguyên *dương*; các số nguyên $\leq 0$, là số đối của các số nguyên dương, được gọi là các số nguyên *âm*; các số nguyên $> 0$ (tương ứng $< 0$) được gọi là các số nguyên *dương ngặt* (tương ứng *âm ngặt*); tập hợp các số nguyên $> 0$ đôi khi được ký hiệu là $\mathbf{N}^*$.

Cho $x$, $y$ và $z$ là ba số nguyên hữu tỉ; khi đó $x \leq y$ khi và chỉ khi x + z \leq y + z. Vì x - y = (x + z) - (y + z). Tính chất này được diễn đạt bằng cách nói rằng quan hệ thứ tự trên $\mathbf{Z}$ là bất biến đối với phép tịnh tiến.

### 6. ỨNG DỤNG: II. PHÉP NHÂN CÁC SỐ NGUYÊN HỮU TỈ

#### Bổ đề 2 {#alg-i-s2-lem-2 .statement}

Cho E là một monoid và x là một phần tử của E.
    (i) Tồn tại một đồng cấu duy nhất f từ $\mathbf{N}$ vào E với $f(1) = x$ và $f(n) = \frac{n}{1} x$ với mọi $n \in \mathbf{N}$.
    (ii) Nếu x khả nghịch, tồn tại một đồng cấu duy nhất g từ $\mathbf{Z}$ vào E sao cho $g(1) = x$ và g trùng với f trên $\mathbf{N}$.

    Viết $f(n) = \frac{n}{1} x$ với mọi $n \in \mathbf{N}$, các công thức
    $$
    \frac{0}{1} x = e \quad \text{và} \quad \left( \frac{m}{1} x \right) \cdot \left( \frac{n}{1} x \right) = \frac{m+n}{1} x
    $$
    (no. 1) diễn đạt rằng f là một đồng cấu từ $\mathbf{N}$ vào E và hiển nhiên $f(1) = x$. Nếu $f'$ là một đồng cấu từ $\mathbf{N}$ vào E sao cho $f'(1) = x$, thì $f = f'$, theo § 1, no. 4, Mệnh đề 1, (iv).

Giả sử bây giờ x khả nghịch. Theo no. 3, Hệ quả 2 của Mệnh đề 4, $f(n) = \frac{n}{1} x$ khả nghịch với mọi số nguyên $n \geq 0$. Theo phép dựng, $\mathbf{Z}$ là nhóm các hiệu của $\mathbf{N}$ và do đó (no. 4, Định lý 1) f mở rộng duy nhất thành một đồng cấu g của $\mathbf{Z}$ vào E. Nếu $g'$ là một đồng cấu của $\mathbf{Z}$ vào E với $g'(1) = x$, hạn chế $f'$ của $g'$ lên $\mathbf{N}$ là một đồng cấu của $\mathbf{N}$ vào E với $f'(1) = x$. Do đó $f' = f$, suy ra $g' = g$.

Chúng ta sẽ áp dụng Bổ đề 2 vào trường hợp monoid E là $\mathbf{Z}$; do đó với mọi số nguyên $m \in \mathbf{Z}$ tồn tại một tự đồng cấu $f_m$ của $\mathbf{Z}$ được đặc trưng bởi $f_m(1) = m$. Nếu m thuộc $\mathbf{N}$, ánh xạ $n \mapsto mn$ của $\mathbf{N}$ vào $\mathbf{N}$ là một tự đồng cấu của magma $\mathbf{N}$ (Lý thuyết tập hợp, III, § 3, no. 3, Hệ quả của Mệnh đề 5); do đó $f_m(n) = mn$ với mọi $m, n$ thuộc $\mathbf{N}$.

Phép nhân trên $\mathbf{N}$ do đó có thể được mở rộng thành phép nhân trên $\mathbf{Z}$ bằng công thức $mn = f_m(n)$ với $m, n$ thuộc $\mathbf{Z}$. Chúng ta sẽ thiết lập các công thức:

(2) $$ xy = yx $$
(3) $$ (xy)z = x(yz) $$
(4) $$ x(y+z) = xy + xz $$
(5) $$ (x+y)z = xz + yz $$
(6) $$ 0.x = x.0 = 0 $$
(7) $$ 1.x = x.1 = x $$
(8) $$ (-1).x = x.(-1) = -x $$

với $x, y, z$ trong $\mathbf{Z}$. (*Nói cách khác, $\mathbf{Z}$ là một vành giao hoán.*) Các công thức $x(y+z) = xy + xz$ và $x.0 = 0$ biểu thị rằng $f_x$ là một tự đồng cấu của monoid cộng tính $\mathbf{Z}$ và $f_x(1) = x$ có thể được viết là $x.1 = x$. Tự đồng cấu $f_x \circ f_y$ của $\mathbf{Z}$ biến 1 thành $xy$ và do đó bằng $f_{xy}$, do đó (3). Bây giờ $f_x(-y) = -f_x(y)$, nghĩa là $x(-y) = -xy$; tương tự, tự đồng cấu $y \mapsto -xy$ của $\mathbf{Z}$ biến 1 thành $-x$, do đó $(-x).y = -xy$ và vì vậy
$$
(-x)(-y) = -(x(-y)) = -(-xy) = xy.
$$
Với $m, n$ trong $\mathbf{N}$, $mn = nm$ (Lý thuyết Tập hợp, III, § 3, no. 3, Hệ quả của Mệnh đề 5), do đó $(-m).n = n(-m)$ và $(-m)(-n) = (-n)(-m)$; vì $\mathbf{Z} = \mathbf{N} \cup (-\mathbf{N})$, $xy = yx$ với $x, y$ trong $\mathbf{Z}$; và công thức này có nghĩa là (5) suy ra từ (4) và hoàn tất chứng minh công thức (6) đến (8).

### 7. ỨNG DỤNG: III. LŨY THỪA TỔNG QUÁT

Cho E là một monoid có phần tử đơn vị $e$ và luật hợp thành được ký hiệu bởi $\top$. Nếu $x$ khả nghịch trong E, gọi $g_x$ là đồng cấu từ $\mathbf{Z}$ vào E biến 1 thành $x$. Đặt $g_x(n) = \frac{n}{\top} x$ với mọi $n \in \mathbf{Z}$; theo Bổ đề 2, ký hiệu này tương thích với ký hiệu đã đưa vào trước đây đối với $n \in \mathbf{N}$. Khi đó
$$
\begin{align*}
\text{(9)} \quad & \frac{m+n}{\top} x = \left( \frac{m}{\top} x \right) \top \left( \frac{n}{\top} x \right) \\
\text{(10)} \quad & \frac{0}{\top} x = e \\
\text{(11)} \quad & \frac{1}{\top} x = x
\end{align*}
$$
với $x$ khả nghịch trong E và $m, n$ trong $\mathbf{Z}$. Hơn nữa, nếu $y = \frac{m}{\top} x$, ánh xạ $n \mapsto g_x(mn)$ từ $\mathbf{Z}$ vào E là một đồng cấu biến 1 thành $y$, do đó $g_x(mn) = g_y(n)$, nghĩa là
$$
\text{(12)} \quad \frac{mn}{\top} x = \frac{n}{\top} \left( \frac{m}{\top} x \right).
$$
Vì $-1$ là phần tử đối của 1 trong $\mathbf{Z}$, $\frac{-1}{\top} x$ là nghịch đảo của $x = \frac{1}{\top} x$ trong E. Nếu ta viết $n = -m$ trong (9), ta thấy rằng $\frac{-m}{\top} x$ là nghịch đảo của $\frac{m}{\top} x$.

### 8. KÝ HIỆU

(a) Theo quy tắc chung, luật của một monoid giao hoán được viết theo phép cộng. Khi đó, theo quy ước, $-x$ ký hiệu số đối của $x$. Ký hiệu $x + (-y)$ được viết tắt thành $x - y$ và tương tự
$$
x + y - z, \quad x - y - z, \quad x - y + z - t, \quad \text{v.v. . . .}
$$
lần lượt biểu thị
$$
x + y + (-z), \quad x + (-y) + (-z), \quad x + (-y) + z + (-t), \quad \text{v.v. . . .}
$$

Với $n \in \mathbf{Z}$, ký hiệu $\overset{n}{\top} x$ được thay bằng $nx$. Các công thức (9) đến (12) khi đó trở thành

(13) $$
(m + n).x = m.x + n.x
$$
(14) $$
0.x = 0
$$
(15) $$
1.x = x
$$
(16) $$
m.(n.x) = (mn).x
$$

trong đó $m$ và $n$ thuộc $\mathbf{N}$ hoặc thậm chí thuộc $\mathbf{Z}$ nếu $x$ có số đối. Cũng trong trường hợp sau, quan hệ $(-1).x = -x$ đúng. Ta cũng chú ý đến công thức

(17) $$
n.(x + y) = n.x + n.y.
$$

(b) Cho E là một monoid được viết theo phép nhân. Với $n \in \mathbf{Z}$, ký hiệu $\overset{n}{\top} x$ được thay bằng $x^n$. Ta có các quan hệ

$$
x^{m+n} = x^m.x^n \\
x^0 = 1 \\
x^1 = x \\
(x^m)^n = x^{mn}
$$

và cả $(xy)^n = x^ny^n$ nếu $x$ và $y$ giao hoán.

Khi $x$ có nghịch đảo, thì đây chính xác là $x^{-1}$. Ký hiệu $\frac{1}{x}$ cũng được dùng thay cho $x^{-1}$. Cuối cùng, khi monoid E giao hoán, $\frac{x}{y}$ hoặc $x/y$ cũng được dùng để chỉ $xy^{-1}$.

### Bài tập {#alg-i-s2-exercises}

Xem [các bài tập của § 2](exercises/s2/).
