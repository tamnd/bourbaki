---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 4
section_title: Groups and groups with operators
lang: vi
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 30-52, 132-140
pdf_pages: 0054-0076, 0156-0164
extraction: ocr
subsections:
    - "no": 1
      title: GROUPS
      page: 30
      pdf_page: 54
    - "no": 2
      title: GROUPS WITH OPERATORS
      page: 31
      pdf_page: 55
    - "no": 3
      title: SUBGROUPS
      page: 32
      pdf_page: 56
    - "no": 4
      title: QUOTIENT GROUPS
      page: 34
      pdf_page: 58
    - "no": 5
      title: DECOMPOSITION OF A HOMOMORPHISM
      page: 37
      pdf_page: 61
    - "no": 6
      title: SUBGROUPS OF A QUOTIENT GROUP
      page: 38
      pdf_page: 62
    - "no": 7
      title: THE JORDAN-HÖLDER THEOREM
      page: 41
      pdf_page: 65
    - "no": 8
      title: PRODUCTS AND FIBRE PRODUCTS
      page: 45
      pdf_page: 69
    - "no": 9
      title: RESTRICTED SUMS
      page: 47
      pdf_page: 71
    - "no": 10
      title: MONOGENOUS GROUPS
      page: 48
      pdf_page: 72
statements: 63
exercises: 26
content_sha256: 172998d2110dc8794cc5334e88b77a6972257ba02a31511e489775f8cc5d9fb2
translated_from: content/en/alg/I/04_s4_groups_and_groups_with_operators.md
source_content_sha256: 4e2db9f086cc50fe763891b92a677519247beb4dcab57f7cc8c6398ff2e2e3db
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-8494d73e
glossary_version: 34
glossary_terms_sha256: 9a825f5c62e874cb85898a1e2a6c9ee9516526b52543eb303194249f6b50e9be
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. NHÓM VÀ NHÓM CÓ TOÁN TỬ

### 1. NHÓM

Nhắc lại định nghĩa sau (§ 2, no. 3, Định nghĩa 6).

#### Định nghĩa 1 {#alg-i-s4-def-1 .statement}

*Một tập hợp với một luật hợp thành kết hợp, có phần tử đơn vị và trong đó mọi phần tử đều khả nghịch, được gọi là một nhóm.*

Nói cách khác, một nhóm là một *monoid* (§ 2, no. 1, Định nghĩa 1) trong đó mọi phần tử đều khả nghịch. Một luật hợp thành trên một tập hợp xác định trên đó một cấu trúc nhóm được gọi là một *luật nhóm*. Nếu G và H là hai nhóm, một đồng cấu magma từ G vào H cũng được gọi là một *đồng cấu nhóm*. Một đồng cấu như vậy $f$ ánh xạ phần tử đơn vị thành phần tử đơn vị; thật vậy, gọi $e$ (tương ứng $e'$) là phần tử đơn vị của G (tương ứng H); viết các luật nhóm của G và H theo lối nhân, ta có $e \cdot e = e$, do đó $f(e) \cdot f(e) = f(e)$ và, nhân với $f(e)^{-1}, f(e) = e'$. Vậy $f$ là có đơn vị. Từ đó, theo no. 3 của § 2, suy ra rằng $f(x^{-1}) = f(x)^{-1}$ với mọi $x \in G$.

#### Ví dụ {#alg-i-s4-n1-exa-1 .statement}

Trong mọi monoid E, tập hợp các phần tử khả nghịch với cấu trúc cảm sinh từ cấu trúc trên E là một nhóm. Đặc biệt, tập hợp các ánh xạ song ánh của một tập hợp F lên chính nó (hay tập các *hoán vị* của F) là một nhóm đối với luật $(f, g) \mapsto f \circ g$, được gọi là *nhóm đối xứng của tập hợp* F và ký hiệu bởi $\mathfrak{S}_F$.

Trong mục này, trừ khi có chỉ dẫn ngược lại, luật hợp thành của một nhóm sẽ luôn luôn được viết theo lối *nhân* và $e$ sẽ ký hiệu phần tử đơn vị của một luật nhóm như vậy.

Một nhóm G được gọi là *hữu hạn* nếu tập hợp nền của G là hữu hạn; nếu không thì nó được gọi là *vô hạn*; lực lượng của một nhóm được gọi là *cấp* của nhóm.

Nếu một luật hợp thành trên G xác định một cấu trúc nhóm trên G, thì luật đối cũng xác định một cấu trúc nhóm trên G. Ánh xạ từ một nhóm G lên chính nó gắn với mỗi $x \in G$ phần tử nghịch đảo của $x$ là một *đẳng cấu* từ G lên nhóm đối (§ 2, no. 3, Mệnh đề 4).

Theo những quy ước tổng quát của chúng tôi (*Tập hợp*, II, § 3, no. 1), chúng tôi sẽ ký hiệu bởi $A^{-1}$ ảnh của một tập con A của G qua ánh xạ $x \mapsto x^{-1}$. Nhưng điều quan trọng là phải chú ý rằng, mặc dù có sự tương tự về ký hiệu, $A^{-1}$ tuyệt nhiên không phải là phần tử nghịch đảo của A đối với luật hợp thành $(X, Y) \mapsto XY$ giữa các tập con của G (nhớ rằng XY là tập hợp các $xy$ với $x \in X, y \in Y$): phần tử đơn vị đối với luật này là $\{e\}$ và các phần tử khả nghịch duy nhất của $\mathcal{P}(G)$ đối với luật này là các tập A chỉ gồm một phần tử (hơn nữa, một A như vậy dĩ nhiên có nghịch đảo là $A^{-1}$). Đồng nhất thức

$(AB)^{-1}=B^{-1}A^{-1}$ đúng với $A\subset G$, $B\subset G$. $A$ được gọi là một tập con đối xứng của $G$ nếu $A=A^{-1}$. Với mọi $A\subset G$, $A\cup A^{-1}$, $A\cap A^{-1}$ và $AA^{-1}$ là đối xứng.

### 2. NHÓM CÓ TOÁN TỬ

#### Định nghĩa 2 {#alg-i-s4-def-2 .statement}

Cho $\Omega$ là một tập hợp. Một nhóm $G$ cùng với một tác động của $\Omega$ trên $G$ có tính phân phối đối với luật nhóm, được gọi là một nhóm có toán tử trong $\Omega$.

Trong phần sau, $x^\alpha$ sẽ ký hiệu hợp thành của $\alpha\in\Omega$ và $x\in G$. Khi đó tính phân phối được biểu thị bởi đồng nhất thức $(xy)^\alpha=x^\alpha y^\alpha$.

Trong một nhóm có toán tử $G$, mỗi toán tử xác định một *tự đồng cấu* của *cấu trúc nhóm* nền; các tự đồng cấu này đôi khi sẽ được gọi là các *phép vị tự* của nhóm có toán tử $G$.

Một nhóm có toán tử $G$ được gọi là *giao hoán* (hay *Abel*) nếu luật nhóm của nó là giao hoán.

Trong phần sau, một nhóm $G$ sẽ được đồng nhất với nhóm có toán tử trong $\varnothing$ thu được bằng cách cho $G$ tác động duy nhất của $\varnothing$ trên $G$. Điều này cho phép chúng ta xem các nhóm như những trường hợp riêng của các nhóm có toán tử và áp dụng cho chúng các định nghĩa và kết quả liên quan đến các nhóm sau mà chúng tôi sẽ phát biểu.

#### Ví dụ {#alg-i-s4-n2-exa-1 .statement}

Trong một nhóm giao hoán $G$, viết theo lối nhân, ta có $(xy)^n=x^ny^n$ với mọi $n\in\mathbf{Z}$ (§ 2, no. 8, equation (1)); do đó tác động $n\mapsto(x\mapsto x^n)$ của $\mathbf{Z}$ trên $G$ xác định, cùng với luật nhóm, cấu trúc của một nhóm có toán tử trên $G$.

#### Định nghĩa 3 {#alg-i-s4-def-3 .statement}

Cho $G$ và $G'$ là các nhóm có toán tử trong $\Omega$. Một đồng cấu của các nhóm có toán tử từ $G$ vào $G'$ là một *đồng cấu của nhóm* $G$ vào *nhóm* $G'$ sao cho

$$
f(x^\alpha)=(f(x))^\alpha
$$

với mọi $\alpha\in\Omega$ và mọi $x\in G$.

Một *tự đồng cấu* của nhóm có toán tử $G$ là một tự đồng cấu của nhóm $G$ mà *giao hoán* với mọi *phép vị tự* của $G$.

Vì hai phép vị tự của một nhóm có toán tử $G$ không nhất thiết giao hoán, nên *một phép vị tự của $G$ nói chung không phải là một tự đồng cấu của nhóm có toán tử $G$.*

Ánh xạ đồng nhất của một nhóm có toán tử là một đồng cấu của các nhóm có toán tử; hợp thành của hai đồng cấu của các nhóm có toán tử cũng vậy. Để một ánh xạ là một đẳng cấu của các nhóm có toán tử, điều kiện cần và đủ là nó là một đồng cấu song ánh của các nhóm có toán tử, và khi đó ánh xạ nghịch đảo là một đẳng cấu của các nhóm có toán tử.

Nói chung hơn, cho G (tương ứng G') là một nhóm có toán tử trong $\Omega$ (tương ứng $\Omega'$). Cho $\phi$ là một ánh xạ từ $\Omega$ vào $\Omega'$. Một $\phi$-đồng cấu từ G vào G' là một đồng cấu của nhóm G vào nhóm G' sao cho

$$
f(x^\alpha) = (f(x))^{(\phi(\alpha))}
$$

với mọi $\alpha \in \Omega$ và mọi $x \in G$.

Trong phần còn lại của đoạn này, ta cho trước một tập hợp $\Omega$. Trừ khi có nói khác, các nhóm có toán tử được xét sẽ nhận $\Omega$ làm tập hợp các toán tử.

### 3. NHÓM CON

#### Định nghĩa 4 {#alg-i-s4-def-4 .statement}

*Cho G là một nhóm có toán tử. Một nhóm con ổn định của G là một tập con H của G có các tính chất sau*:

(i) $e \in H$;
(ii) $x, y \in H \implies xy \in H$;
(iii) $x \in H \implies x^{-1} \in H$;
(iv) $x \in H$ và $\alpha \in \Omega$ kéo theo $x^\alpha \in H$.

Nếu H là một nhóm con ổn định của G, thì cấu trúc cảm sinh trên H bởi cấu trúc nhóm có toán tử trên G là một cấu trúc nhóm có toán tử, và đơn ánh chính tắc từ H vào G là một đồng cấu của các nhóm có toán tử.

Cho G là một nhóm. Một nhóm con ổn định của G với tác động của $\varnothing$ (no. 2), tức là một tập con của G thỏa mãn các điều kiện (i), (ii), (iii) của Định nghĩa 4, được gọi là một *nhóm con* của G. Khi nói về một nhóm con của một nhóm có toán tử, ta sẽ luôn luôn hiểu đó là một nhóm con của nhóm nền tảng của G. Một nhóm con của một nhóm có toán tử G không nhất thiết là một nhóm con ổn định của G.

*Ví dụ* (1). Cho $\Sigma$ là một loài cấu trúc (*Set Theory*, IV, § 1, no. 4) và S là một cấu trúc thuộc loài $\Sigma$ trên một tập hợp E (*loc. cit.*). Tập hợp các *tự đẳng cấu* của S là một nhóm con của $\mathcal{G}_E$.

#### Mệnh đề 1 {#alg-i-s4-prop-1 .statement}

*Cho G là một nhóm có toán tử và H là một tập con của G ổn định đối với các phép vị tự của G. Các điều kiện sau là tương đương*:

(a) *H là một nhóm con ổn định của G*.
(b) *H là khác rỗng và các quan hệ* $x \in H, y \in H \implies xy \in H$ *và* $x^{-1} \in H$.
(c) *H là khác rỗng và các quan hệ* $x \in H, y \in H \implies xy^{-1} \in H$.
(d) *H ổn định đối với luật trên G và luật hợp thành cảm sinh trên H bởi luật hợp thành trên G là một luật nhóm*.

Rõ ràng (a) kéo theo (b). Ta chứng minh rằng (b) kéo theo (a). Chỉ cần chứng minh rằng H chứa phần tử đơn vị của G. Vì tập con H là khác rỗng, lấy $x \in H$. Khi đó $x^{-1} \in H$ và $e = xx^{-1} \in H$. Rõ ràng (b) kéo theo (c). Ta chứng minh rằng (c) kéo theo (b). Trước hết, vì H là khác rỗng nên nó chứa một phần tử x. Do đó xx^{-1} = e là một phần tử của H. Với mọi phần tử x của H, $x^{-1} = ex^{-1}$ thuộc H; do đó các quan hệ $x \in H, y \in H$ kéo theo $x(y^{-1})^{-1} = xy \in H$. Rõ ràng (a) kéo theo (d). Ta chứng minh rằng (d) kéo theo (a): đơn ánh chính tắc từ H vào G là một đồng cấu nhóm; do đó $e \in H$ và quan hệ $x \in H$ kéo theo $x^{-1} \in H$ (no. 1).

#### Nhận xét {#alg-i-s4-n3-rem-1 .statement}

(1) Tương tự cũng có thể chứng minh rằng điều kiện (b) là tương đương với điều kiện
(c') $H \neq \varnothing$ và các quan hệ $x \in H$ và $y \in H$ kéo theo $y^{-1}x \in H$.
(2) Với mọi nhóm con H của G có các quan hệ sau
$$(1)$$
$$H.H = H \quad \text{và} \quad H^{-1} = H.$$
Ta có $H.H \subset H$ và $H^{-1} \subset H$ theo (b). Vì $e \in H, H.H \supset e.H = H$ và lấy nghịch đảo biến bao hàm $H^{-1} \subset H$ thành $H \subset H^{-1}$, do đó có các công thức (1).

Nếu H là một nhóm con ổn định của G và K là một nhóm con ổn định của H, thì rõ ràng K là một nhóm con ổn định của G.

Tập hợp $\{e\}$ là nhóm con ổn định nhỏ nhất của G. Giao của một họ các nhóm con ổn định của G là một nhóm con ổn định. Do đó tồn tại một nhóm con ổn định nhỏ nhất H của G chứa một tập con X đã cho của G; nó được gọi là *nhóm con ổn định sinh bởi* X và X được gọi là một *hệ sinh* (hoặc *tập sinh*) của H.

#### Mệnh đề 2 {#alg-i-s4-prop-2 .statement}

*Cho X là một tập con khác rỗng của một nhóm với các toán tử G và $\hat{X}$ là tập con ổn định đối với tác động của $\Omega$ trên G sinh bởi X. Nhóm con ổn định sinh bởi X là tập con ổn định đối với luật trên G sinh bởi tập $Y = \hat{X} \cup \hat{X}^{-1}$.*

Tập con sau cùng Z là tập hợp các hợp thành của các dãy hữu hạn mà mọi hạng của chúng đều là phần tử của $\hat{X}$ hoặc là nghịch đảo của các phần tử của $\hat{X}$: nghịch đảo của một hợp thành như vậy là một hợp thành cùng dạng (§ 2, no. 3, Hệ quả 1 của Mệnh đề 5) và Z ổn định đối với tác động của $\Omega$, như thấy được bằng cách áp dụng § 3, no. 4, Mệnh đề 1 cho các phép vị tự của G, do đó (Mệnh đề 1) Z là một *nhóm con ổn định* của G. Ngược lại, mọi nhóm con ổn định chứa X hiển nhiên chứa Y và do đó chứa Z.

#### Hệ quả 1 {#alg-i-s4-prop-2-cor-1 .statement}

*Cho G là một nhóm với các toán tử và X là một tập con của G ổn định đối với tác động của $\Omega$. Nhóm con sinh bởi X và nhóm con ổn định sinh bởi X là trùng nhau.*

#### Hệ quả 2 {#alg-i-s4-prop-2-cor-2 .statement}

*Cho G là một nhóm và X là một tập con của G gồm các phần tử từng đôi một giao hoán được. Nhóm con của G sinh bởi X là giao hoán.*

Tập $Y = X \cup X^{-1}$ gồm các phần tử từng đôi một giao hoán được (§ 2, no. 3, Mệnh đề 5) và luật cảm sinh trên tập con ổn định sinh bởi Y là giao hoán (§ 1, no. 5, Hệ quả 2).

Nếu G là một nhóm với các toán tử, thì nhóm con ổn định sinh bởi một tập con của G gồm các phần tử từng đôi một giao hoán được không nhất thiết là giao hoán.

#### Hệ quả 3 {#alg-i-s4-prop-2-cor-3 .statement}

Cho $f : G \to G'$ là một đồng cấu của các nhóm với các toán tử và X là một tập con của G. Ảnh qua f của nhóm con ổn định của G sinh bởi X là nhóm con ổn định của G' sinh bởi $f(X)$.

Đặt $X' = f(X)$. Khi đó $\hat{X}' = f(\hat{X})$ và ${X'}^{-1} = f(X^{-1})$. Do đó
$$
f(\hat{X} \cup \hat{X}^{-1}) = \hat{X}' \cup \hat{{X}'}^{-1}.
$$
Hệ quả suy ra từ § 1, no. 4, Mệnh đề 1.

Ví dụ (2). Cho G là một nhóm và x là một phần tử của G. Nhóm con sinh bởi $\{x\}$ (gọi đơn giản hơn là nhóm con sinh bởi x) là tập hợp các $x^n, n \in \mathbf{Z}$. Tập con ổn định (đối với luật trên G) sinh bởi $\{x\}$ là tập hợp các $x^n$ với $n \in \mathbf{N}^*$. Nói chung hai tập hợp này là phân biệt.

Do đó, trong nhóm cộng $\mathbf{Z}$, nhóm con sinh bởi một phần tử x là tập $x.\mathbf{Z}$ gồm các $xn, n \in \mathbf{Z}$, và tập con ổn định sinh bởi x là tập hợp các $xn, n \in \mathbf{N}^*$. Hai tập hợp này luôn luôn phân biệt nếu $x \neq 0$.

Hiển nhiên hợp của một họ có hướng phải các nhóm con ổn định của G là một nhóm con ổn định. Suy ra rằng, nếu P là một tập con của G và H là một nhóm con ổn định của G không giao với P, thì tập hợp các nhóm con ổn định của G chứa H và không giao với P, được sắp thứ tự bởi quan hệ bao hàm, là quy nạp (Lý thuyết tập hợp, III, § 2, no. 4). Áp dụng Bổ đề Zorn (Lý thuyết tập hợp, III, § 2, no. 4), ta thu được kết quả sau:

#### Mệnh đề 3 {#alg-i-s4-prop-3 .statement}

Cho G là một nhóm với các toán tử, P là một tập con của G và H là một nhóm con ổn định của G không giao với P. Tập hợp các nhóm con ổn định của G chứa H và không giao với P có một phần tử cực đại.

### 4. NHÓM THƯƠNG

#### Định lý 1 {#alg-i-s4-thm-1 .statement}

Cho R là một quan hệ tương đương trên một nhóm với các toán tử G; nếu R tương thích trái (resp. phải) (§ 3, no. 3) với luật nhóm trên G và tương thích với tác động của $\Omega$, thì lớp tương đương của e là một nhóm con ổn định H của G và quan hệ R tương đương với $x^{-1}y \in H$ (resp. $yx^{-1} \in H$). Ngược lại, nếu H là một nhóm con ổn định của G, thì quan hệ $x^{-1}y \in H$ (resp. $yx^{-1} \in H$) là một quan hệ tương đương tương thích trái (resp. phải) với luật nhóm trên G và tương thích với tác động của $\Omega$, và theo quan hệ ấy H là lớp tương đương của e.

Ta chỉ xét trường hợp quan hệ R tương thích trái với luật trên G (trường hợp của một quan hệ tương thích phải thu được bằng cách thay thế luật trên G bởi luật đối). Quan hệ $y \equiv x \pmod{R}$ tương đương với $x^{-1}y \equiv e \pmod{R}$, vì $y \equiv x$ kéo theo $x^{-1}y \equiv x^{-1}x = e$ và ngược lại $x^{-1}y \equiv e$ kéo theo $y = x(x^{-1}y) \equiv x$. Nếu H ký hiệu lớp tương đương của e, thì quan hệ R khi đó tương đương với $x^{-1}y \in H$. Ta chứng minh rằng H là một nhóm con ổn định của G. Với mọi toán tử $\alpha$, quan hệ $x \equiv e$ kéo theo $x^\alpha \equiv e^\alpha = e$, do đó $H^\alpha \subset H$ và H ổn định đối với tác động của $\Omega$. Chỉ còn phải thiết lập (Mệnh đề 1) rằng $x \in H$ và $y \in H$ kéo theo $x^{-1}y \in H$, nghĩa là $x \equiv e$ và $y \equiv e$ kéo theo $x \equiv y$, điều này là hệ quả của tính bắc cầu của R.

Ngược lại, cho H là một nhóm con ổn định của G; quan hệ $x^{-1}y \in H$ có tính phản xạ vì $x^{-1}x = e \in H$; nó có tính đối xứng vì $x^{-1}y \in H$ kéo theo $y^{-1}x = (x^{-1}y)^{-1} \in H$; nó có tính bắc cầu, vì $x^{-1}y \in H$ và $y^{-1}z \in H$ kéo theo $x^{-1}z = (x^{-1}y)(y^{-1}z) \in H$; nó tương thích trái với luật hợp thành trên G, vì $x^{-1}y = (zx)^{-1}(zy)$ với mọi $z \in G$; cuối cùng, với mọi tác tử $\alpha$, quan hệ $y \in xH$ kéo theo $y^\alpha \in x^\alpha H^\alpha \subset x^\alpha H$ và do đó quan hệ tương đương $x^{-1}y \in H$ tương thích với tác động của $\Omega$ trên G.

Cho G là một nhóm và H là một nhóm con của G; quan hệ $x^{-1}y \in H$ (resp. $yx^{-1} \in H$) cũng được viết dưới dạng tương đương $y \in xH$ (resp. $y \in Hx$). Như vậy, mỗi nhóm con H của G xác định hai quan hệ tương đương trên G, cụ thể là $y \in xH$ và $y \in Hx$: các lớp tương đương theo các quan hệ này lần lượt là các tập hợp $xH$, được gọi là các *lớp ghép trái của H* (hoặc *modulo H*), và các tập hợp $Hx$, được gọi là các *lớp ghép phải của H* (hoặc *modulo H*). Bằng cách *làm bão hòa* một tập con $A \subset G$ đối với các quan hệ này (*Tập hợp*, II, § 6, no. 4), ta lần lượt thu được các tập hợp AH và HA. Ánh xạ $x \mapsto x^{-1}$ biến các lớp ghép trái modulo H thành các lớp ghép phải modulo H và ngược lại.

Lực lượng của tập hợp các lớp ghép trái (mod. H) được gọi là *chỉ số* của nhóm con H đối với G và được ký hiệu bởi $(G:H)$; nó cũng bằng lực lượng của tập hợp các lớp ghép phải.

Nếu một nhóm con K của G chứa H, thì nó là một hợp của các lớp ghép trái (hoặc phải) của H. Vì một lớp ghép trái của K thu được từ K bằng phép tịnh tiến trái, tập hợp các lớp ghép trái của H được chứa trong một lớp ghép trái của K có lực lượng độc lập với lớp ghép trái đó. Do đó (*Tập hợp*, III, § 5, no. 8, Mệnh đề 9):

#### Mệnh đề 4 {#alg-i-s4-prop-4 .statement}

*Cho H và K là hai nhóm con của một nhóm G sao cho H $\subset$ K. Khi đó*
$$
(G:H) = (G:K)(K:H).
$$

#### Hệ quả {#alg-i-s4-n4-cor-1 .statement}

*Nếu G là một nhóm hữu hạn có cấp g và H là một nhóm con của G có cấp h, thì*
$$
h \cdot (G:H) = g
$$
(đặc biệt, cấp và chỉ số của H là *các ước* của cấp của G).

Định lý 1 cho phép ta xác định các quan hệ tương đương tương thích với các luật trên một nhóm có tác tử G: nếu R là một quan hệ như vậy, thì nó vừa tương thích trái vừa tương thích phải với luật nhóm trên G và với tác động của $\Omega$. Do đó, nếu H là lớp của $e$ (mod. R), thì H là một nhóm con ổn định sao cho các quan hệ $y \in xH$ và $y \in Hx$ là tương đương (vì cả hai đều tương đương với R); do đó $xH = Hx$ với mọi $x \in G$. Ngược lại, nếu điều này đúng, một trong hai quan hệ tương đương $y \in xH, y \in Hx$ tương thích với luật nhóm, vì nó vừa tương thích trái vừa tương thích phải với luật này ($\S$ 3, no. 4) và tương thích với tác động của $\Omega$. Vì phương trình $xH = Hx$ tương đương với $xHx^{-1} = H$, ta đưa ra định nghĩa sau:

#### Định nghĩa 5 {#alg-i-s4-def-5 .statement}

*Một nhóm G có tác tử. Một nhóm con ổn định H của G được gọi là một nhóm con ổn định chuẩn (hoặc bất biến) của G nếu $xHx^{-1} = H$ với mọi $x \in G$.*

Nếu $\Omega = \varnothing$, một nhóm con ổn định chuẩn của G được gọi là một *nhóm con chuẩn* (hoặc *bất biến*) của G. Trong một nhóm giao hoán, mọi nhóm con đều là chuẩn.

Để kiểm tra rằng một nhóm con ổn định H là chuẩn, chỉ cần chứng minh rằng $xHx^{-1} \subset H$ với mọi $x \in G$; vì nếu vậy thì $x^{-1}Hx \subset H$ với mọi $x \in G$, tức là $H \subset xHx^{-1}$, và do đó $H = xHx^{-1}$.

Cho H là một nhóm con ổn định chuẩn của G và R là quan hệ tương đương $y \in xH$ được xác định bởi H; trên tập thương $G/R$, luật nội, tức thương theo R của luật nhóm của G, có tính kết hợp; lớp của e là phần tử đơn vị của luật thương này; các lớp của hai phần tử nghịch đảo trong G là các phần tử nghịch đảo theo luật thương và tác động của $\Omega$, tức thương theo R của tác động của $\Omega$ trên G, phân phối đối với luật nội trên $G/R$ ($\S$ 3, no. 5). Do đó, tóm tắt các kết quả đã thu được:

#### Định lý 2 {#alg-i-s4-thm-2 .statement}

*Cho G là một nhóm có toán tử. Để một quan hệ tương đương R trên G tương thích với luật nhóm và tác động của $\Omega$, điều kiện cần và đủ là nó có dạng $x^{-1}y \in H$, trong đó H là một nhóm con chuẩn ổn định của G (hơn nữa quan hệ $x^{-1}y \in H$ là tương đương với $yx^{-1} \in H$ đối với một nhóm con như vậy). Luật hợp thành trên $G/R$ là thương của luật hợp thành trên G và tác động của $\Omega$ trên $G/R$ là thương của tác động của $\Omega$ trên G theo một quan hệ như vậy R đem lại cho $G/R$ cấu trúc của một nhóm có toán tử, được gọi là cấu trúc thương, và ánh xạ chính tắc chuyển sang thương là một đồng cấu của các nhóm có toán tử.*

#### Định nghĩa 6 {#alg-i-s4-def-6 .statement}

*Thương của một nhóm có toán tử G theo quan hệ tương đương được xác định bởi một nhóm con chuẩn của G, với cấu trúc thương, được gọi là nhóm thương có toán tử của G theo H và được ký hiệu là $G/H$. Ánh xạ chính tắc $G \to G/H$ được gọi là một đồng cấu chính tắc*

Cho G là một nhóm và H là một nhóm con chuẩn của G. Thương $G/H$, với cấu trúc nhóm của nó, được gọi là *nhóm thương* của G theo H. Để một ánh xạ từ $G/H$ vào một nhóm có toán tử là một đồng cấu của các nhóm có toán tử, điều kiện cần và đủ là hợp thành của nó với ánh xạ chính tắc từ G lên $G/H$ là một đồng cấu như vậy: điều này biện minh cho tên gọi "nhóm thương" (*Lý thuyết tập hợp*, IV, $\S$ 2, no. 6).

Quan hệ tương đương được xác định bởi một nhóm con chuẩn ổn định của G được ký hiệu bởi $x \equiv y \pmod{H}$ hoặc $x \equiv y(H)$.

#### Mệnh đề 5 {#alg-i-s4-prop-5 .statement}

Cho $f : G \to G'$ là một đồng cấu của các nhóm có toán tử, và $H$ và $H'$ là các nhóm con chuẩn ổn định của $G$ và $G'$ tương ứng sao cho $f(H) \subset H'$. Ánh xạ $f$ tương thích với các quan hệ tương đương được xác định bởi $H$ và $H'$. Cho $\pi : G \to G/H$ và $\pi' : G' \to G'/H'$ là các đồng cấu chính tắc. Ánh xạ $\bar{f} : G/H \to G'/H'$ dẫn xuất từ $f$ bằng cách chuyển qua các thương là một đồng cấu.

Nếu $x \equiv y \pmod{H}$, thì $x^{-1}y \in H$, do đó
$$
f(x)^{-1}f(y) = f(x^{-1})f(y) = f(x^{-1}y) \in f(H) \subset H'
$$
và vì thế $f(x) \equiv f(y) \pmod{H'}$. Mệnh đề thứ hai suy ra từ tính chất phổ quát của các luật thương ($§ 1$, no. 6).

#### Nhận xét {#alg-i-s4-n4-rem-1 .statement}

(1) Nếu $A$ là một tập con bất kỳ của một nhóm $G$ và $H$ là một nhóm con chuẩn của $G$, thì $AH = HA$; tập hợp này thu được bằng cách bão hòa $A$ đối với quan hệ $x \equiv y \pmod{H}$.

(2) Nếu $H$ là một nhóm con chuẩn của $G$ có chỉ số hữu hạn, thì nhóm thương $G/H$ là một nhóm hữu hạn có cấp $(G:H)$.

Chú ý rằng nếu $H$ là một nhóm con chuẩn của một nhóm $G$ và $K$ là một nhóm con chuẩn của $H$, thì $K$ không nhất thiết là một nhóm con chuẩn của $G$ (I, $§ 5$, Bài tập 10).

Cho $G$ là một nhóm có toán tử. Giao của mọi họ các nhóm con chuẩn ổn định của $G$ là một nhóm con chuẩn ổn định. Do đó, với mọi tập con $X$ của $G$, tồn tại một nhóm con chuẩn ổn định nhỏ nhất chứa $X$, được gọi là nhóm con chuẩn ổn định *sinh bởi* $X$.

Trong một nhóm với các toán tử $G$, các nhóm con ổn định $G$ và $\{e\}$ là chuẩn tắc.

#### Định nghĩa 7 {#alg-i-s4-def-7 .statement}

*Một nhóm với các toán tử* $G$ *được gọi là đơn nếu* $G \neq \{e\}$ *và không tồn tại nhóm con ổn định chuẩn tắc nào của* $G$ *ngoài* $G$ *và* $\{e\}$.

### 5. PHÂN TÍCH CỦA MỘT ĐỒNG CẤU

#### Mệnh đề 6 {#alg-i-s4-prop-6 .statement}

*Cho* $G$ *là một nhóm với các toán tử và* $G'$ *là một magma có một tác động bởi* $\Omega$, *được viết theo lũy thừa*. *Cho* $f : G \to G'$ *là một đồng cấu từ magma* $G$ *vào magma* $G'$ *sao cho, với mọi* $\alpha \in \Omega$ *và mọi* $x \in G$, $f(x^\alpha) = f(x)^\alpha$. *Khi đó* $f(G)$ *là một tập con ổn định của* $G'$ *đối với luật trên* $G'$ *và tác động của* $\Omega$; *tập* $f(G)$ *với các luật cảm sinh là một nhóm với các toán tử và ánh xạ* $x \mapsto f(x)$ *từ* $G$ *vào* $f(G)$ *là một đồng cấu của các nhóm với các toán tử*.

Theo $§ 1$, no. 4, Mệnh đề 1, $f(G)$ là một tập con ổn định của $G'$ đối với luật trong trên $G'$. Với mọi phần tử $x \in G$ và với mọi toán tử $\alpha$,
$f(x)^\alpha = f(x^\alpha) \in f(G)$ và do đó $f(G)$ ổn định dưới tác động của $\Omega$ trên $G'$. Viết luật trong của $G'$ theo lối nhân,
$$
(f(x)f(y))f(z) = f(xy)f(z) = f((xy)z) = f(x(yz)) = f(x)f(yz)
= f(x)(f(y)f(z))
$$
với mọi phần tử $x, y, z$ trong $G$; do đó luật cảm sinh trên $f(G)$ là kết hợp.

Gọi $e$ là phần tử đơn vị của $G$. Ảnh của nó $f(e)$ là một phần tử đơn vị của $f(G)$ ($§ 2$, no. 1). Mọi phần tử của $f(G)$ đều khả nghịch trong $f(G)$ ($§ 2$, no. 3). Do đó luật được cảm sinh trên $f(G)$ bởi luật trong trên $G'$ là một luật nhóm. Với mọi phần tử $x$ và $y$ trong $G$ và mọi toán tử $\alpha$,

$$
(f(x)f(y))^\alpha = (f(xy))^\alpha = f((xy)^\alpha) = f(x^\alpha y^\alpha) = f(x^\alpha)f(y^\alpha) = (f(x))^\alpha(f(y))^\alpha
$$

điều đó cho thấy tác động của $\Omega$ là phân phối đối với luật nhóm trên $f(G)$. Vậy $f(G)$ với các luật cảm sinh là một nhóm với các toán tử và rõ ràng ánh xạ $x \mapsto f(x)$ là một đồng cấu của các nhóm với các toán tử.

#### Định nghĩa 8 {#alg-i-s4-def-8 .statement}

*Cho $f : G \to G'$ là một đồng cấu của các nhóm có toán tử. Ảnh ngược của phần tử đơn vị của $G'$ được gọi là hạt nhân của $f$.*

Hạt nhân của $f$ thường được ký hiệu bởi $\mathrm{Ker}(f)$ và ảnh $f(G)$ của $f$ đôi khi được ký hiệu bởi $\mathrm{Im}(f)$.

#### Định lý 3 {#alg-i-s4-thm-3 .statement}

*Cho $f : G \to G'$ là một đồng cấu của các nhóm có toán tử.*
(a) *$\mathrm{Ker}(f)$ là một nhóm con chuẩn ổn định của $G$;*
(b) *$\mathrm{Im}(f)$ là một nhóm con ổn định của $G'$;*
(c) *ánh xạ $f$ tương thích với quan hệ tương đương xác định trên $G$ bởi $\mathrm{Ker}(f)$;*
(d) *ánh xạ $\tilde{f} : G/\mathrm{Ker}(f) \to \mathrm{Im}(f)$ dẫn xuất từ $f$ bằng cách chuyển qua thương là một đẳng cấu của các nhóm có toán tử;*
(e) *$f = i \circ \tilde{f} \circ \pi$, trong đó $i$ là đơn ánh chính tắc của $\mathrm{Im}(f)$ vào $G'$ và $\pi$ là đồng cấu chính tắc của $G$ lên $G/\mathrm{Ker}(f)$.*

Mệnh đề (b) suy ra từ Mệnh đề 6. Quan hệ tương đương $f(x) = f(y)$ trên $G$ tương thích với cấu trúc nhóm có toán tử trên $G$. Theo Định lý 2 (no. 4), do đó nó có dạng $y \in xH$, trong đó $H$ là một nhóm con chuẩn ổn định của $G$ và $H$ là lớp của phần tử đơn vị, do đó $H = \mathrm{Ker}(f)$. Các mệnh đề (a), (c) và (d) khi đó suy ra. Mệnh đề (e) là hiển nhiên (*Lý thuyết tập hợp*, II, § 6, no. 5).

### 6. CÁC NHÓM CON CỦA MỘT NHÓM THƯƠNG

#### Mệnh đề 7 {#alg-i-s4-prop-7 .statement}

*Cho $G$ và $H$ là hai nhóm có toán tử, $f$ là một đồng cấu của $G$ vào $H$ và $N$ là hạt nhân của $f$.*
(a) *Cho $H'$ là một nhóm con ổn định của $H$. Ảnh ngược $G' = f^{-1}(H')$ là một nhóm con ổn định của $G$ và $G'$ là chuẩn tắc trong $G$ nếu $H'$ là chuẩn tắc trong $H$. Hơn nữa, $N$ là một nhóm con chuẩn tắc của $G'$. Nếu $f$ là toàn ánh, thì $H' = f(G')$ và $f$ xác định một đẳng cấu của $G'/N$ lên $H'$ khi chuyển qua thương.*
(b) *Cho $G'$ là một nhóm con ổn định của $G$. Ảnh $H' = f(G')$ là một nhóm con ổn định của $H$ và $f^{-1}(H') = G'N = NG'$. Đặc biệt, $f^{-1}(H') = G'$ khi và chỉ khi $N \subset G'$. Nếu $f$ là toàn ánh và $G'$ là chuẩn tắc trong $G$, thì $H'$ là chuẩn tắc trong $H$.*

(a) Cho $x$ và $y$ thuộc $G'$ và $\alpha \in \Omega$; khi đó $f(x) \in H'$ và $f(y) \in H'$, do đó $f(xy^{-1}) = f(x)f(y)^{-1} \in H'$, nghĩa là $xy^{-1} \in G'$; suy ra $G'$ là một nhóm con của $G$. Bây giờ $f(x^\alpha) = f(x)^\alpha \in H'$, do đó $x^\alpha \in G'$ và vì vậy $G'$ là ổn định. Giả sử $H'$ là chuẩn tắc trong $H$ và cho $x \in G', y \in G$; khi đó $f(x) \in H'$ và
$$
f(yxy^{-1}) = f(y)f(x)f(y)^{-1} \in H'
$$
do đó $yxy^{-1} \in G'$; suy ra $G'$ là chuẩn tắc trong $G$. Với mọi $n \in N, f(n) = e \in H'$, do đó $N \subset G'$; vì $N$ là chuẩn tắc trong $G$, nó là chuẩn tắc trong $G'$. Cuối cùng, nếu $f$ là toàn ánh,
$$
f(f^{-1}(A)) = A \text{ với mọi tập con } A \text{ của } H,
$$
do đó $H' = f(G')$; hạn chế của $f$ trên $G'$ là một đồng cấu $f'$ từ $G'$ lên $H'$ có hạt nhân $N$, do đó $f'$ xác định qua chuyển qua thương một đẳng cấu của $G'/N$ lên $H'$.

(b) Cho $a$ và $b$ thuộc $H'$ và $\alpha$ thuộc $\Omega$; tồn tại $x, y$ thuộc $G'$ sao cho $a = f(x)$ và $b = f(y)$, do đó $ab^{-1} = f(xy^{-1}) \in H'$, suy ra $H'$ là một nhóm con của $H$ ổn định, vì $a^\alpha = f(x^\alpha) \in H'$. Cho $x \in G$; khi đó $x \in f^{-1}(H')$ khi và chỉ khi $f(x) \in H' = f(G')$, nghĩa là khi và chỉ khi tồn tại $y$ thuộc $G'$ sao cho $f(x) = f(y)$; quan hệ $f(x) = f(y)$ tương đương với sự tồn tại của $n \in N$ sao cho $x = yn$; cuối cùng, $x \in f^{-1}(H')$ tương đương với $x \in G'N = NG'$. Rõ ràng quan hệ $G' = G'N$ tương đương với $G' \supset N$. Cuối cùng giả sử rằng $f$ là toàn ánh và $G'$ là chuẩn trong $G$; cho $a \in H'$ và $b \in H$; tồn tại $x \in G'$ và $y \in G$ sao cho $a = f(x)$ và $b = f(y)$, do đó $bab^{-1} = f(yxy^{-1}) \in f(G') = H'$. Suy ra $H'$ là chuẩn trong $H$.

#### Hệ quả 1 {#alg-i-s4-prop-7-cor-1 .statement}

*Giả sử rằng $f$ là toàn ánh. Gọi $\mathcal{G}$ (tương ứng $\mathcal{G}'$) là tập hợp các nhóm con ổn định (tương ứng ổn định chuẩn) của $G$ chứa $N$ và $\mathfrak{H}$ (tương ứng $\mathfrak{H}'$) là tập hợp các nhóm con ổn định (tương ứng ổn định chuẩn) của $H$, các tập hợp này được có thứ tự bởi quan hệ bao hàm. Ánh xạ $G' \mapsto f(G')$ là một đẳng cấu tập hợp có thứ tự $\Phi : \mathcal{G} \to \mathfrak{H}$; đẳng cấu nghịch đảo $\Psi : \mathfrak{H} \to \mathcal{G}$ là ánh xạ $H' \mapsto f^{-1}(H')$. Hơn nữa $\Phi$ và $\Psi$ cảm sinh các đẳng cấu $\Phi' : \mathcal{G}' \to \mathfrak{H}'$ và $\Psi' : \mathfrak{H}' \to \mathcal{G}'$.

#### Hệ quả 2 {#alg-i-s4-prop-7-cor-2 .statement}

*Cho $f : G \to H$ là một đồng cấu của các nhóm có toán tử, $N$ là hạt nhân của $f$, $G'$ là một nhóm con ổn định của $G$ và $L$ là một nhóm con ổn định chuẩn của $G'$. Khi đó $LN, L.(G' \cap N)$ và $f(L)$ lần lượt là các nhóm con ổn định chuẩn của $G'N, G'$ và $f(G')$ và ba nhóm thương có toán tử $G'N/LN, G'/L.(G' \cap N)$ và $f(G')/f(L)$ là đẳng cấu.

Cho $H' = f(G')$ và ký hiệu $f'$ là đồng cấu của $G'$ lên $H'$ trùng với $f$ trên $G'$; hạt nhân của $f'$ là $G \cap N$ và $f'(L) = f(L)$; theo Mệnh đề 7, $f'(L)$ là một nhóm con ổn định chuẩn của $H'$ và
$$
{f'}^{-1}(f'(L)) = L.(G' \cap N)
$$
là một nhóm con ổn định chuẩn của $G'$. Gọi $\lambda$ là đồng cấu chính tắc của $H'$ lên $H'/f'(L) = f(G')/f(L)$: vì $\lambda \circ f'$ là toàn ánh với hạt nhân
$$
{f'}^{-1}(f'(L)) = L.(G' \cap N),
$$

nó xác định một đẳng cấu của $G'/L\cdot(G'\cap N)$ lên $f(G')/f(L)$. Theo Mệnh đề 7, (b), $f^{-1}(H')=G'N$; nếu $f''$ là đồng cấu của $G'N$ lên $H'$ trùng với $f$ trên $G'N$, thì đồng cấu $\lambda\circ f''$ của $G'N$ lên $f(G')/f(L)$ là toàn ánh với hạt nhân $f^{-1}(f(L))=LN$; điều này chứng minh rằng $LN$ là một nhóm con ổn định chuẩn của $G'N$ và rằng $\lambda\circ f''$ xác định một đẳng cấu của $G'N/LN$ lên $f(G')/f(L)$.

#### Hệ quả 3 {#alg-i-s4-prop-7-cor-3 .statement}

Cho $f:G\to H$ là một đồng cấu của các nhóm có toán tử, $N$ là hạt nhân của nó, $X$ là một tập con của $G$ sao cho $f(X)$ sinh ra $H$ và $Y$ là một tập con của $N$ sinh ra $N$. Khi đó $X\cup Y$ sinh ra $N$.

Cho $G'$ là nhóm con ổn định của $G$ sinh bởi $X\cup Y$. Vì $Y\subset G'$, $N\subset G'$.

Vì $f(X)\subset f(G')$, $f(G')=H$, do đó $G'=f^{-1}(H)=G$.

#### Nhận xét {#alg-i-s4-n6-rem-1 .statement}

Theo ký hiệu của Mệnh đề 7, sự kiện rằng ảnh ngược của một nhóm con của $H$ là một nhóm con của $G$ suy ra từ sự kiện tổng quát hơn sau đây.

Nếu $A$ và $B$ là các tập con của $H$ và $f$ là toàn ánh, thì

$$
f^{-1}(A\cdot B)=f^{-1}(A)\cdot f^{-1}(B),\qquad
f^{-1}(A^{-1})=f^{-1}(A)^{-1}.
$$

Hiển nhiên $f^{-1}(A)\cdot f^{-1}(B)\subset f^{-1}(A\cdot B)$; mặt khác, nếu $z\in f^{-1}(A\cdot B)$, tồn tại $a\in A$ và $b\in B$ sao cho $f(z)=ab$; vì $f$ là toàn ánh, tồn tại $x\in G$ sao cho $f(x)=a$; viết $y=x^{-1}z$, ta có $f(y)=a^{-1}f(z)=b$ và $z=xy$, do đó $z\in f^{-1}(A)\cdot f^{-1}(B)$. Quan hệ $x\in f^{-1}(A^{-1})$ là tương đương với $f(x)\in A^{-1}$, do đó tương đương với $f(x^{-1})\in A$, nghĩa là $x^{-1}\in f^{-1}(A)$ và cuối cùng là $x\in f^{-1}(A)^{-1}$.

#### Mệnh đề 8 {#alg-i-s4-prop-8 .statement}

Cho $G$ là một nhóm với các toán tử và $A$ và $B$ là hai nhóm con ổn định của $G$. Giả sử rằng các quan hệ $a\in A$ và $b\in B$ kéo theo $aba^{-1}\in B^{*}$ (nói cách khác, $A$ chuẩn hóa $B$)$^{*}$. Khi đó $AB=BA$ là một nhóm con ổn định của $G$, $A\cap B$ là một nhóm con ổn định chuẩn tắc của $A$ và $B$ là một nhóm con ổn định chuẩn tắc của $AB$. Đơn ánh chính tắc của $A$ vào $AB$ xác định, khi chuyển qua thương, một đẳng cấu của $A/(A\cap B)$ lên $AB/B$.

Các công thức

$$
(ab)(a'b')=aa'({a'}^{-1}ba'\cdot b')
$$

$$
(ab)^{-1}=a^{-1}(ab^{-1}a^{-1})
$$

$$
(ab)^\alpha=a^\alpha b^\alpha
$$

với $a,a'\in A$, $b,b'\in B$ và mọi toán tử $\alpha$ trên $G$, hãy chứng tỏ rằng $AB$ là một nhóm con ổn định của $G$. Cho $a\in A$ và $x\in A\cap B$; khi đó $axa^{-1}\in B$ theo các giả thiết đặt trên $A$ và $B$ và rõ ràng $axa^{-1}$ thuộc $A$, do đó $A\cap B$ là chuẩn tắc trong $A$. Cho $a\in A$ và $b,b'$ thuộc $B$; công thức $(ab)b'(ab)^{-1}=a(bb'b^{-1})a^{-1}$ cho thấy rằng $B$ là chuẩn tắc trong $AB$. Gọi $\phi$ là hạn chế lên $A$ của đồng cấu chính tắc của AB lên AB/B; khi đó $\phi(a) = aB$ và do đó hạt nhân của $\phi$ bằng $A \cap B$. Rõ ràng $\phi$ là toàn ánh và vì vậy xác định một đẳng cấu của $A/(A \cap B)$ lên $AB/B$.

#### Định lý 4 {#alg-i-s4-thm-4 .statement}

*Cho G là một nhóm có toán tử và N là một nhóm con ổn định chuẩn tắc của G.*

(a) *Ánh xạ $G' \mapsto G'/N$ là một song ánh từ tập hợp các nhóm con ổn định của G chứa N lên tập hợp các nhóm con ổn định của G/N.*

(b) *Cho $G'$ là một nhóm con ổn định của G chứa N. Để $G'/N$ chuẩn tắc trong $G/N$, điều kiện cần và đủ là $G'$ chuẩn tắc trong G, và khi đó các nhóm $G/G'$ và $(G/N)/(G'/N)$ là đẳng cấu.*

(c) *Cho $G'$ là một nhóm con ổn định của G. Khi đó $G'N$ là một nhóm con ổn định của G và N là chuẩn tắc trong $G'N$. Hơn nữa $G' \cap N$ là chuẩn tắc trong $G'$ và các nhóm $G'/(G' \cap N)$ và $G'N/N$ là đẳng cấu.*

Ký hiệu $f$ là đồng cấu chính tắc của G lên $G/N$. Với mọi $x \in G$, $f(x) \in xN$; do đó, $f(G') = G'/N$ với mọi nhóm con $G'$ của G chứa N. Vì $f$ là toàn ánh, mệnh đề (a) suy ra từ Hệ quả 1 của Mệnh đề 7; tương tự đối với tương đương thức "G' chuẩn tắc" $\Leftrightarrow$ "G'/N chuẩn tắc". Giả sử rằng $G'$ là một nhóm con ổn định chuẩn tắc của G chứa N. Theo no. 4, Mệnh đề 5 áp dụng cho $\mathrm{Id}_G$, tồn tại một đồng cấu $u$ từ $G/N$ vào $G/G'$ được xác định bởi $u(xN) = xG'$ với mọi $x \in G$. Ngay lập tức thấy rằng $u$ là toàn ánh với hạt nhân $G'/N$ do đó có đẳng cấu cần tìm từ $(G/N)/(G'/N)$ lên $G/G'$. Cuối cùng, (c) suy ra ngay lập tức từ Mệnh đề 8.

### 7. ĐỊNH LÝ JORDAN-HÖLDER

#### Định nghĩa 9 {#alg-i-s4-def-9 .statement}

*Một chuỗi hợp thành của một nhóm có toán tử G là một dãy hữu hạn $(G_i)_{0 \leq i \leq n}$ các nhóm con ổn định của G, với $G_0 = G$ và $G_n = \{e\}$, sao cho $G_{i+1}$ là một nhóm con chuẩn tắc của $G_i$ với $0 \leq i \leq n-1$. Các thương $G_i/G_{i+1}$ được gọi là các thương của chuỗi. Một chuỗi hợp thành $\Sigma'$ được gọi là mịn hơn một chuỗi hợp thành $\Sigma$ nếu $\Sigma$ là một chuỗi lấy từ $\Sigma'$.

Nếu $(G_i)_{0 \leq i \leq n}$ và $(H_j)_{0 \leq j \leq m}$ lần lượt là các chuỗi hợp thành của hai nhóm có toán tử G và H, thì chúng được gọi là tương đương nếu $m = n$ và tồn tại một phép hoán vị $\phi$ của khoảng $\{0, n-1\}$ của $\mathbf{N}$ sao cho các nhóm có toán tử $G_i/G_{i+1}$ và $H_{\phi(i)}/H_{\phi(i)+1}$ đẳng cấu với nhau với mọi $i$.

Chú ý rằng nói chung một chuỗi lấy từ một chuỗi hợp thành $(G_i)$ không phải là một chuỗi hợp thành, vì với $j > i + 1$, $G_j$ nói chung không phải là một nhóm con chuẩn tắc của $G_i$.

**Định lý 5 (Schreier).** *Cho hai chuỗi hợp thành $\Sigma_1, \Sigma_2$ của một nhóm có toán tử G. Khi đó tồn tại hai chuỗi hợp thành tương đương $\Sigma'_1, \Sigma'_2$, lần lượt mịn hơn $\Sigma_1$ và $\Sigma_2$.

Cho $\Sigma_1 = (H_i)_{0 \leq i \leq n}$ và $\Sigma_2 = (K_j)_{0 \leq j \leq p}$ là hai chuỗi hợp thành đã cho, lần lượt có $n + 1$ và $p + 1$ số hạng; ta sẽ thấy rằng chuỗi hợp thành $\Sigma'_1$ có thể được tạo thành bằng cách chèn $p - 1$ nhóm con $H'_{i,j}$ (1 \leq j \leq p - 1) vào giữa H_i và H_{i+1} với 0 \leq i \leq n - 1, và chuỗi \Sigma_2' bằng cách chèn n - 1 nhóm con K_{j,i}' (1 \leq i \leq n - 1) vào giữa K_j và K_{j+1} với 0 \leq j \leq p - 1; như vậy thu được hai chuỗi gồm pn + 1 nhóm con ổn định của G; bằng cách chọn thích hợp các nhóm con ổn định được chèn vào, ta sẽ chứng minh rằng các chuỗi này là các chuỗi hợp thành tương đương.

Để làm điều đó, chú ý rằng H_i \cap K_j là một nhóm con ổn định của H_i và của K_j, và do đó (Định lý 4) H_{i+1}.(H_i \cap K_j) là một nhóm con ổn định của H_i chứa H_{i+1}, và K_{j+1}.(H_i \cap K_j) là một nhóm con ổn định của K_j chứa K_{j+1}. Nếu ta viết H_{i,j}' = H_{i+1}.(H_i \cap K_j) và K_{j,i}' = K_{j+1}.(H_i \cap K_j), thì H_{i,j+1}' là một nhóm con ổn định của H_{i,j}' (0 \leq j \leq p - 1) và K_{j,i+1}' là một nhóm con ổn định của K_{j,i}' (0 \leq i \leq n - 1). Hơn nữa H_{i,0}' = H_i, H_{i,p}' = H_{i+1}, K_{j,0}' = K_j và K_{j,p}' = K_{j+1}. Để chứng minh định lý, chỉ cần chứng minh rằng H_{i,j+1}' (tương ứng, K_{j,i+1}') là một nhóm con ổn định chuẩn tắc của H_{i,j}' (tương ứng, K_{j,i}') và rằng các nhóm thương H_{i,j}'/H_{i,j+1}' và K_{j,i}'/K_{j,i+1}' là đẳng cấu (0 \leq i \leq n - 1, 0 \leq j \leq p - 1). Điều này suy ra từ bổ đề sau đây bằng cách lấy H = H_i, H' = H_{i+1}, K = K_j, K' = K_{j+1}.

Bổ đề 1 (Zassenhaus). Cho H và K là hai nhóm con ổn định của một nhóm có toán tử G, và H' và K' lần lượt là các nhóm con ổn định chuẩn tắc của H và K; khi đó H'.(H \cap K') là một nhóm con ổn định chuẩn tắc của H'.(H \cap K), K'.(K \cap H') là một nhóm con ổn định chuẩn tắc của K'.(K \cap H), và các nhóm thương có toán tử (H'.(H \cap K))/(H'.(H \cap K')) và (K'.(K \cap H))/(K'.(K \cap H')) là đẳng cấu.

Theo Định lý 4, H' \cap K = H' \cap (H \cap K) là một nhóm con ổn định chuẩn tắc của H \cap K; tương tự K' \cap H là một nhóm con ổn định chuẩn tắc của K \cap H; do đó (no. 6, Hệ quả 2) (H' \cap K)(K' \cap H) là một nhóm con ổn định chuẩn tắc của H \cap K. Theo Định lý 4 áp dụng cho nhóm H,

$$
H'.(H' \cap K).(K' \cap H) = H'.(H \cap K')
$$

là một nhóm con ổn định chuẩn tắc của H'.(H \cap K), và nhóm thương

$$
(H'.(H \cap K))/(H'.(H \cap K))
$$

là đẳng cấu với

$$
(H \cap K)/((H' \cap K).(K' \cap H)).
$$

Trong thương cuối cùng này, H và H' một mặt, K và K' mặt khác, xuất hiện một cách đối xứng; hoán vị chúng thì thu được kết quả đã nêu.

#### Định nghĩa 10 {#alg-i-s4-def-10 .statement}

Một chuỗi Jordan-Hölder của một nhóm có toán tử G là một chuỗi phân tích giảm nghiêm ngặt \Sigma sao cho không tồn tại chuỗi phân tích giảm nghiêm ngặt nào khác \Sigma và mịn hơn \Sigma.

#### Mệnh đề 9 {#alg-i-s4-prop-9 .statement}

Điều kiện cần và đủ để một chuỗi phân tích của G là một chuỗi Jordan-Hölder là mọi thương của chuỗi đều đơn.

Một chuỗi phân tích giảm nghiêm ngặt khi và chỉ khi không có thương liên tiếp nào của nó rút gọn thành phần tử đơn vị. Nếu một chuỗi hợp thành giảm nghiêm ngặt $\Sigma$ không phải là một chuỗi Jordan-Hölder, thì tồn tại một chuỗi hợp thành giảm nghiêm ngặt $\Sigma'$ mịn hơn $\Sigma$ và phân biệt với $\Sigma$. Do đó có hai số hạng liên tiếp $G_i, G_{i+1}$ của $\Sigma$ không liên tiếp trong $\Sigma'$; gọi $H$ là số hạng đầu tiên đứng sau $G_i$ trong $\Sigma'$; $H$ là một nhóm con ổn định chuẩn của $G_i$, chứa $G_{i+1}$ và phân biệt với nhóm sau; do đó $H/G_{i+1}$ là một nhóm con ổn định chuẩn của $G_i/G_{i+1}$, phân biệt với nhóm sau và với phần tử đơn vị; vậy $G_i/G_{i+1}$ không đơn. Ngược lại, nếu $\Sigma$ là một chuỗi hợp thành giảm nghiêm ngặt mà một trong các thương $G_i/G_{i+1}$ của nó không đơn, thì thương này chứa một nhóm con ổn định chuẩn khác với chính nó và $\{e\}$, có ảnh ngược trong $G_i$ là một nhóm con ổn định chuẩn $H$ của $G_i$, phân biệt với $G_i$ và $G_{i+1}$ (Định lý 4); chỉ cần chèn $H$ vào giữa $G_i$ và $G_{i+1}$ để thu được một chuỗi hợp thành giảm nghiêm ngặt phân biệt với $\Sigma$ và mịn hơn $\Sigma$.

**Định lý 6 (Jordan-Hölder).** *Hai chuỗi Jordan-Hölder của một nhóm có toán tử là tương đương.*

Cho $\Sigma_1, \Sigma_2$ là hai chuỗi Jordan-Hölder của một nhóm có toán tử $G$; bằng cách áp dụng Định lý 5 thu được hai chuỗi hợp thành *tương đương* $\Sigma'_1, \Sigma'_2$ lần lượt mịn hơn $\Sigma_1$ và $\Sigma_2$; vì các chuỗi sau là các chuỗi Jordan-Hölder, $\Sigma'_1$ đồng nhất với $\Sigma_1$ hoặc được dẫn xuất từ nó bằng cách lặp lại một số số hạng nhất định; chuỗi các thương của $\Sigma'_1$ được dẫn xuất từ chuỗi tương ứng của $\Sigma_1$ bằng cách chèn một số số hạng đẳng cấu với nhóm $\{e\}$; vì $\Sigma_1$ giảm nghiêm ngặt, chuỗi các thương của $\Sigma_1$ được dẫn xuất từ chuỗi của $\Sigma'_1$ bằng cách loại bỏ trong chuỗi sau *tất cả* các số hạng đẳng cấu với $\{e\}$. Tương tự đối với $\Sigma_2$ và $\Sigma'_2$. Vì chuỗi các thương của $\Sigma'_1$ và $\Sigma'_2$ chỉ khác nhau (sai khác đẳng cấu) về cấp của các số hạng, điều tương tự cũng đúng đối với $\Sigma_1$ và $\Sigma_2$; định lý được chứng minh.

#### Hệ quả {#alg-i-s4-n7-cor-1 .statement}

*Cho $G$ là một nhóm có toán tử trong đó tồn tại một chuỗi Jordan-Hölder. Nếu $\Sigma$ là một chuỗi hợp thành giảm nghiêm ngặt bất kỳ của $G$, thì tồn tại một chuỗi Jordan-Hölder mịn hơn $\Sigma$.*

Cho $\Sigma_0$ là một chuỗi Jordan-Hölder của $G$; theo Định lý 5, tồn tại hai chuỗi hợp thành tương đương, $\Sigma'$ và $\Sigma'_0$, mịn hơn lần lượt $\Sigma$ và $\Sigma_0$; lập luận của Định lý 6 cho thấy rằng, bằng cách lược bỏ khỏi $\Sigma'$ các sự lặp lại, thu được một dãy $\Sigma''$ tương đương với $\Sigma_0$ và do đó là một chuỗi Jordan-Hölder, vì mọi thương của nó đều đơn (Mệnh đề 9). Vì $\Sigma$ giảm nghiêm ngặt, $\Sigma''$ mịn hơn $\Sigma$, do đó có hệ quả.

#### Nhận xét {#alg-i-s4-n7-rem-1 .statement}

Một nhóm với các toán tử không phải lúc nào cũng có một chuỗi Jordan-Hölder; một ví dụ được cho bởi nhóm cộng $\mathbf{Z}$ của các số nguyên: dãy $(2^n \cdot \mathbf{Z})_{n \geq 0}$ là một dãy vô hạn giảm nghiêm ngặt các nhóm con (chuẩn) của $\mathbf{Z}$; với mọi $p$, $p$ số hạng đầu của dãy này cùng với nhóm $\{0\}$ tạo thành một chuỗi hợp thành giảm nghiêm ngặt; nếu tồn tại một chuỗi Jordan-Hölder của $\mathbf{Z}$, thì nó sẽ có ít nhất $p+1$ số hạng, theo Hệ quả của Định lý 6; điều này vô lý, vì $p$ là tùy ý.

Mặt khác, tồn tại một chuỗi Jordan-Hölder trong mọi nhóm *hữu hạn* với các toán tử G: nếu $G \ne \{e\}$, trong các nhóm con chuẩn ổn định của G khác G, lấy $H_1$ là một nhóm con cực đại; tương tự, định nghĩa $H_{n+1}$ bằng quy nạp là một phần tử cực đại trong tập hợp các nhóm con chuẩn của $H_n$, khác $H_n$, khi $H_n \ne \{e\}$; dãy các cấp của các $H_n$ giảm nghiêm ngặt, do đó tồn tại $n$ sao cho $H_n = \{e\}$ và dãy gồm G và các $H_i$ ($1 \leq i \leq n$) theo cách xây dựng của nó là một chuỗi Jordan-Hölder.

#### Định nghĩa 11 {#alg-i-s4-def-11 .statement}

Cho G là một nhóm với các toán tử; độ dài của G là cận trên của các số nguyên $n$ sao cho tồn tại một chuỗi hợp thành giảm nghiêm ngặt của G $(G_i)_{0\leq i\leq n}$.

Nếu G có một chuỗi Jordan-Hölder, thì độ dài của G là số các thương liên tiếp của chuỗi này, như suy ra từ Hệ quả của Định lý 6. Nếu G không có chuỗi Jordan-Hölder, thì độ dài của nó là vô hạn; theo Mệnh đề 9, với mọi chuỗi giảm nghiêm ngặt của G đều tồn tại một chuỗi giảm nghiêm ngặt mịn hơn nghiêm ngặt. Nhóm gồm phần tử đơn vị là nhóm duy nhất với các toán tử có độ dài không. Một nhóm với các toán tử là đơn khi và chỉ khi nó có độ dài 1.

Cho G là một nhóm với các toán tử, H là một nhóm con chuẩn ổn định của G, K là thương G/H và $\pi:G\to K$ là đồng cấu chính tắc. Cho

$$
\Sigma'=(H_i)_{0\leq i\leq n}
$$

là một chuỗi phân tích của H và

$$
\Sigma''=(K_j)_{0\leq j\leq p}
$$

là một chuỗi hợp thành của K. Viết $G_i=\pi^{-1}(K_i)$ với $0\leq i\leq p$ và $G_i=H_{i-p}$ với $p\leq i\leq n+p$, ta thu được một chuỗi hợp thành

$$
\Sigma=(G_i)_{0\leq i\leq n+p}
$$

của G. Dãy các thương của $\Sigma$ được thu được bằng cách ghép dãy các thương của $\Sigma''$ với dãy các thương của $\Sigma'$. Nếu $\Sigma'$ và $\Sigma''$ là các chuỗi Jordan-Hölder, thì $\Sigma$ là một chuỗi Jordan-Hölder của G, theo Mệnh đề 9. Nếu H hoặc K có các chuỗi hợp thành với độ dài tùy ý, thì G cũng vậy. Ta đã chứng minh:

#### Mệnh đề 10 {#alg-i-s4-prop-10 .statement}

Cho G là một nhóm với các toán tử và H là một nhóm con chuẩn ổn định của G. Độ dài của G là tổng các độ dài của H và G/H.

#### Hệ quả {#alg-i-s4-n7-cor-2 .statement}

Cho G là một nhóm với các toán tử và $(G_i)_{0\leq i\leq n}$ là một chuỗi hợp thành của G. Độ dài của G là tổng các độ dài của các $G_i/G_{i+1}$, $0\leq i\leq n-1$.

Nếu G và $G'$ là các nhóm đẳng cấu với các toán tử và G có một chuỗi Jordan-Hölder, thì $G'$ cũng vậy và các chuỗi Jordan-Hölder của G và $G'$ là tương đương. Tuy nhiên, các nhóm không đẳng cấu có thể có các chuỗi Jordan-Hölder tương đương; điều đó đúng với $\mathbf{Z}/4\mathbf{Z}$ và $(\mathbf{Z}/2\mathbf{Z})\times(\mathbf{Z}/2\mathbf{Z})$, xem no. 10.

### 8. TÍCH VÀ TÍCH THỚ THẲNG

Cho $(G_i)_{i \in I}$ là một họ các nhóm có tác tử. Cho $G$ là monôit tích của các $G_i$. Xét tác động của $\Omega$ trên $G$ được xác định bởi

$$
((x_i)_{i \in I})^\alpha = (x_i^\alpha)_{i \in I} \quad (\alpha \in \Omega, x_i \in G_i).
$$

Với cấu trúc này $G$ là một nhóm có tác tử. Với mọi $i \in I$, phép chiếu $\mathrm{pr}_i : G \to G_i$ là một đồng cấu của các nhóm có tác tử.

#### Định nghĩa 12 {#alg-i-s4-def-12 .statement}

*Nhóm có tác tử* $G = \prod_{i \in I} G_i$ *được xác định ở trên là nhóm tích có tác tử của các* $G_i$. *Các ánh xạ* $\mathrm{pr}_i : G \to G_i$ *được gọi là các* đồng cấu chiếu.

Một trường hợp riêng của tích các nhóm có tác tử là nhóm $G^E$ gồm các ánh xạ của một tập hợp $E$ vào một nhóm có tác tử $G$, các phép toán được xác định bởi:

$$
(fg)(x) = f(x)g(x) \quad (f, g \in G^E, x \in E)
$$
$$
f^\alpha(x) = f(x)^\alpha \quad (f \in G^E, \alpha \in \Omega, x \in E).
$$

Cho $(\phi_i : H \to G_i)_{i \in I}$ là một họ các đồng cấu của các nhóm có tác tử. Ánh xạ $h \mapsto (\phi_i(h))_{i \in I}$ từ $H$ vào $\prod_{i \in I} G_i$ là một đồng cấu của các nhóm có tác tử. Đây là đồng cấu duy nhất $\Phi : H \to \prod_{i \in I} G_i$ thỏa mãn $\mathrm{pr}_i \circ \Phi = \phi_i$ với mọi $i$. Điều này biện minh cho tên gọi "nhóm tích có tác tử" (*Lý thuyết tập hợp*, IV, § 2, no. 4).

Cho $(\phi_i : H_i \to G_i)_{i \in I}$ là một họ các đồng cấu của các nhóm có tác tử. Ánh xạ $\prod_{i \in I} \phi_i : (h_i)_{i \in I} \mapsto (\phi_i(h_i))_{i \in I}$ từ $\prod_{i \in I} H_i$ vào $\prod_{i \in I} G_i$ là một đồng cấu của các nhóm có tác tử.

#### Mệnh đề 11 {#alg-i-s4-prop-11 .statement}

*Cho* $(\phi_i : H_i \to G_i)_{i \in I}$ *là một họ các đồng cấu của các nhóm có tác tử và cho* $\Phi = \prod_{i \in I} \phi_i$. *Khi đó:*

(a) $\mathrm{Ker}(\Phi) = \prod_{i \in I} \mathrm{Ker}(\phi_i)$; *đặc biệt, nếu mọi* $\phi_i$ *đều đơn ánh, thì* $\Phi$ *đơn ánh*.

(b) $\mathrm{Im}(\Phi) = \prod_{i \in I} \mathrm{Im}(\phi_i)$; *đặc biệt, nếu mọi* $\phi_i$ *đều toàn ánh, thì* $\Phi$ *toàn ánh*.

Điều này là ngay lập tức.

Đặc biệt, cho $(G_i)_{i \in I}$ là một họ các nhóm có toán tử và, với mọi $i$, cho $H_i$ là một nhóm con ổn định (tương ứng, nhóm con ổn định chuẩn tắc) của $G_i$. Tích $\prod_{i \in I} H_i$ là một nhóm con ổn định (tương ứng, nhóm con ổn định chuẩn tắc) của $\prod_{i \in I} G_i$ và ánh xạ chính tắc của $\prod_{i \in I} G_i$ lên $\prod_{i \in I} (G_i / H_i)$ xác định khi chuyển qua thương một đẳng cấu từ
$$
\left( \prod_{i \in I} G_i \right) / \left( \prod_{i \in I} H_i \right)
$$
lên $\prod_{i \in I} (G_i / H_i)$. Ví dụ, cho $J$ là một tập con của $I$. Nhóm con $G_J$ của $\prod_{i \in I} G_i$ gồm các $(x_i)_{i \in I}$ sao cho $x_i = e_i$ với $i \notin J$ là một nhóm con ổn định chuẩn tắc. Ánh xạ $\iota_J$ gán cho $x = (x_j)_{j \in J}$ phần tử $y = (y_i)_{i \in I}$ sao cho $y_i = e_i$ với $i \notin J$ và $y_i = x_i$ với $i \in J$, là một đẳng cấu của $\prod_{j \in J} G_j$ lên $G_J$. Ánh xạ $\mathrm{pr}_{I-J}$ xác định khi chuyển qua thương một đẳng cấu $\theta_J$ của nhóm thương $G / G_J$ lên $\prod_{i \in I-J} G_i$. Hợp thành $\mathrm{pr}_J \circ \iota_J$ là ánh xạ đồng nhất của $\prod_{j \in J} G_j$. $G / G_J$ thường được đồng nhất với $\prod_{i \in I-J} G_i$ nhờ $\theta_J$ và $\prod_{i \in J} G_i$ với $G_J$ nhờ $\iota_J$.

Nếu $J_1$ và $J_2$ là các tập con rời nhau của $I$, theo các định nghĩa, mọi phần tử của $G_{J_1}$ giao hoán với mọi phần tử của $G_{J_2}$.

#### Định nghĩa 13 {#alg-i-s4-def-13 .statement}

*Cho $G$ là một nhóm có toán tử và $(H_i)_{i \in I}$ là một họ các nhóm con ổn định chuẩn tắc của $G$. Cho $p_i : G \to G / H_i$ là đồng cấu chính tắc. $G$ được gọi là tích nội tại (hay tích) của họ các nhóm thương $(G / H_i)$ nếu đồng cấu $g \mapsto (p_i(g))_{i \in I}$ là một đẳng cấu của $G$ lên $\prod_{i \in I} G / H_i$.*

Cho $G$ và $H$ là các nhóm có toán tử và $\phi$ và $\psi$ là hai đồng cấu của $G$ vào $H$. Tập hợp các phần tử $x$ của $G$ sao cho $\phi(x) = \psi(x)$ là một nhóm con ổn định của $G$, gọi là *nhóm trùng hợp* của $\phi$ và $\psi$. Đặc biệt, cho $\phi_1 : G_1 \to H$ và $\phi_2 : G_2 \to H$ là các đồng cấu của các nhóm có toán tử; nhóm trùng hợp của các đồng cấu $\phi_1 \circ \mathrm{pr}_1$ và $\phi_2 \circ \mathrm{pr}_2$ của $G_1 \times G_2$ vào $H$ được gọi là *tích thớ* của $G_1$ và $G_2$ trên $H$ đối với $\phi_1$ và $\phi_2$. Nó được ký hiệu bởi $G_1 \times_H G_2$ khi không có sự nhập nhằng về $\phi_1$ và $\phi_2$ và các hạn chế $p_1$ và $p_2$ của $\mathrm{pr}_1$ và $\mathrm{pr}_2$ lên $G_1 \times_H G_2$ cũng được gọi là các đồng cấu phép chiếu. Khi đó $\phi_1 \circ p_1 = \phi_2 \circ p_2$. Các phần tử của $G_1 \times_H G_2$ là các cặp có thứ tự $(g_1, g_2) \in G_1 \times G_2$ sao cho $\phi_1(g_1) = \phi_2(g_2)$. Nếu $f_i$ là một đồng cấu của một nhóm có toán tử $K$ vào $G_i$ ($i = 1, 2$) và $\phi_1 \circ f_1 = \phi_2 \circ f_2$, thì tồn tại một và chỉ một đồng cấu $f$ của $K$ vào $G_1 \times_H G_2$ sao cho $f_i = p_i \circ f$ với $i = 1, 2$.

### 9. CÁC TỔNG HẠN CHẾ

Cho $(G_i)_{i \in I}$ là một họ các nhóm có toán tử và, với $i \in I$, cho $H_i$ là một nhóm con ổn định của $G_i$. Tập con của $\prod_{i \in I} G_i$ gồm các $(x_i)_{i \in I}$ sao cho tập hợp các $i \in I$ với $x_i \notin H_i$ là hữu hạn là một nhóm con ổn định của $\prod_{i \in I} G_i$ bằng $\prod_{i \in I} G_i$ nếu $I$ là hữu hạn. Nó được gọi là *tổng hạn chế của các $G_i$ đối với các $H_i$*. Khi, với mọi $i$ ngoại trừ một số hữu hạn, $H_i$ là một nhóm con ổn định chuẩn của $G_i$, tổng hạn chế là một nhóm con ổn định chuẩn của tích. Khi, với mọi $i$, nhóm con $H_i$ được thu gọn thành phần tử đơn vị của $G_i$, tổng trực tiếp của các $G_i$ đối với các $H_i$ được gọi đơn giản là *tổng hạn chế của các $G_i$* và đôi khi được ký hiệu bởi $\prod_{i \in I} G_i$. Với mọi $i_0 \in I$, ánh xạ $\iota_{i_0}: G_{i_0} \to \prod_{i \in I} G_i$ xác định bởi $\iota_{i_0}(x) = (x_i)_{i \in I}$, trong đó $x_{i_0} = x$ và $x_i = e_i$ nếu $i \neq i_0$, là một đơn cấu các nhóm có toán tử được gọi là *đơn ánh chính tắc*. $G_i$ được đồng nhất với nhóm con ổn định $\operatorname{Im}(\iota_i)$. Các nhóm con $G_i$ là chuẩn. Với $i \neq j$, các phần tử của $G_i$ và $G_j$ giao hoán và $G_i \cap G_j = \{e\}$. Nhóm $\prod_{i \in I} G_i$ được sinh bởi tập hợp $\bigcup_{i \in I} G_i$.

#### Mệnh đề 12 {#alg-i-s4-prop-12 .statement}

*Cho $(\phi_i: G_i \to K)_{i \in I}$ là một họ các đồng cấu của các nhóm có toán tử sao cho, với mọi $i \in I$ và $j \in I$ với $i \neq j$, $x \in G_i$, $y \in G_j$, các phần tử $\phi_i(x)$ và $\phi_j(y)$ của $K$ giao hoán; tồn tại duy nhất một đồng cấu của các nhóm có toán tử $\Phi$ từ $\prod_{i \in I} G_i$ vào $K$ sao cho $\phi_i = \Phi \circ \iota_i$ với mọi $i \in I$. Với mọi phần tử $x = (x_i)_{i \in I}$ của $\prod_{i \in I} G_i$, $\Phi(x) = \prod_{i \in I} \phi_i(x_i)$.*

Nếu $\Phi$ và $\Phi$ là các nghiệm của bài toán, thì chúng trùng nhau trên $\bigcup_{i \in I} G_i$ và do đó trên $\prod_{i \in I} G_i$, suy ra tính duy nhất của $\Phi$. Bây giờ ta chứng minh sự tồn tại của $\Phi$: với mọi phần tử $x = (x_i)_{i \in I}$ của $\prod_{i \in I} G_i$, đặt $\Phi(x) = \prod_{i \in I} \phi_i(x_i)$ (§ 1, no. 5). Rõ ràng $\Phi \circ \iota_i = \phi_i$ với mọi $i$ và $\Phi$ giao hoán với các phép vị tự; công thức $\Phi(xy) = \Phi(x)\Phi(y)$ suy ra từ § 1, no. 5, công thức (9).

#### Định nghĩa 14 {#alg-i-s4-def-14 .statement}

*Cho $G$ là một nhóm với toán tử và $(H_i)_{i \in I}$ là một họ các nhóm con ổn định của $G$. Ta gọi $G$ là tổng hạn chế trong (hoặc tổng hạn chế) của họ các nhóm con $(H_i)$ nếu mọi phần tử của $H_i$ đều hoán vị được với mọi phần tử của $H_j$ khi $j \neq i$ và đồng cấu duy nhất từ $\prod_{i \in I} H_i$ vào $G$ mà hạn chế của nó trên mỗi $H_i$ là đơn ánh chính tắc là một đẳng cấu.*

Khi $I$ là hữu hạn, do lạm dụng ngôn ngữ, ta cũng nói *tích trực tiếp trong* (hoặc *tích trực tiếp*, hoặc *tích*) thay cho tổng hạn chế trong. Mọi nhóm con ổn định H của G mà tồn tại một nhóm con ổn định H' của G sao cho G là tích trực tiếp của H và H' đều được gọi là một *nhân tử trực tiếp* của G.

#### Mệnh đề 13 {#alg-i-s4-prop-13 .statement}

*Cho G là một nhóm với toán tử và $(H_i)_{i \in I}$ là một họ các nhóm con ổn định của G sao cho mọi phần tử của $H_i$ đều hoán vị được với mọi phần tử của $H_j$ khi $j \neq i$. Để G là tổng hạn chế của họ các nhóm con $(H_i)_{i \in I}$, điều kiện cần và đủ là mọi phần tử x của G đều biểu diễn được duy nhất dưới dạng $\prod_{i \in I} y_i$, trong đó $(y_i)_{i \in I}$ là một họ giá hữu hạn các phần tử của G với $y_i \in H_i$ với mọi i.*

Hiển nhiên.

#### Mệnh đề 14 {#alg-i-s4-prop-14 .statement}

*Cho G là một nhóm với toán tử và $(H_i)_{i \in I}$ là một họ hữu hạn các nhóm con ổn định của G. Để G là tổng hạn chế của họ các nhóm con $(H_i)$, điều kiện cần và đủ là mỗi $H_i$ đều là chuẩn tắc và G là tích của các nhóm thương $(G/H^i)$, trong đó $H^i$ là nhóm con sinh bởi các $H_j$ khi $j \neq i$.*

Điều kiện ấy hiển nhiên là cần. Ngược lại, giả sử G là tích của các $K_i = G/H^i$ và đồng nhất G với tích của các $K_i$. Khi đó $H_i$ được đồng nhất với một nhóm con của $K_i$, nên, với $i \neq j$, mọi phần tử của $H_i$ đều hoán vị được với mọi phần tử của $H_j$; mặt khác, $H^i$ được đồng nhất với tích của các $K_j$ khi $j \neq i$, do đó $H_i = K_i$ với mọi $i$ và G là tích trực tiếp của các $H_i$.

#### Mệnh đề 15 {#alg-i-s4-prop-15 .statement}

*Cho G là một nhóm với toán tử và $(H_i)_{1 \leq i \leq n}$ là một dãy các nhóm con chuẩn tắc ổn định của G sao cho*
$$
(H_1 H_2 \ldots H_i) \cap H_{i+1} = \{e\} \quad \text{với } 1 \leq i \leq n-1,
$$
*thì tập hợp $H_1 H_2 \ldots H_n$ là một nhóm con chuẩn tắc ổn định của G, là tổng hạn chế của các $H_i$.*

Bằng quy nạp theo $n$, điều này ngay lập tức được quy về việc chứng minh mệnh đề cho $n = 2$. Trước hết ta chỉ ra rằng, nếu $x \in H_1$ và $y \in H_2$, thì x và y là *hoán vị được*; vì $xyx^{-1}y^{-1} = (xyx^{-1})y^{-1} = x(yx^{-1}y^{-1})$ và do đó (vì $H_1$ và $H_2$ là chuẩn tắc) $xyx^{-1}y^{-1} \in H_1 \cap H_2$, nghĩa là $xyx^{-1}y^{-1} = e$, theo giả thiết. Hơn nữa $H_1 H_2$ là một tập con của G ổn định đối với các phép vị tự của G. Suy ra (theo no. 3, mệnh đề 1) rằng $H_1 H_2$ là một nhóm con ổn định của G và kiểm tra ngay lập tức được rằng nhóm con này là chuẩn tắc. Sau cùng, giả sử rằng $xy = x'y'$, với $x \in H_1, x' \in H_1, y \in H_2, y' \in H_2$; khi đó ${x'}^{-1}x = y'y^{-1}$, do đó ${x'}^{-1}x \in H_1 \cap H_2 = \{e\}$, $x' = x$ và tương tự $y' = y$; vậy $H_1 H_2$ là tích trực tiếp của $H_1$ và $H_2$.

Khi nhóm đang xét là giao hoán, thuật ngữ *tổng trực tiếp* được dùng thay cho tích trực tiếp.

### 10. NHÓM ĐƠN SINH

Cho $a \in \mathbf{Z}$; vì $a\mathbf{Z}$ là một nhóm con của $\mathbf{Z}$, quan hệ giữa các phần tử $x, y$ của $\mathbf{Z}$ phát biểu rằng "tồn tại $z \in \mathbf{Z}$ sao cho $x - y = az$" là một quan hệ tương đương, mà ta quy ước, một lần cho mãi mãi, viết là $x \equiv y \pmod{a}$ hoặc $x \equiv y(a)$ và được gọi là *đồng dư modulo* $a$. Thay thế $a$ bởi $-a$ thì thu được một quan hệ tương đương, do đó có thể giả sử rằng $a \geqslant 0$; với $a = 0$, $x \equiv y(0)$ có nghĩa là $x = y$, do đó chỉ thu được một quan hệ phân biệt với đẳng thức nếu $a \neq 0$: vì vậy trong phần sau ta sẽ giả sử rằng $a > 0$ trừ khi có nói khác.

Với $a > 0$, thương của $\mathbf{Z}$ theo đồng dư $x \equiv y(a)$, tức là nhóm $\mathbf{Z}/a\mathbf{Z}$, được gọi là *nhóm các số nguyên hữu tỉ modulo* $a$.

#### Mệnh đề 16 {#alg-i-s4-prop-16 .statement}

*Cho $a$ là một số nguyên $> 0$. Các số nguyên $r$ sao cho $0 \leqslant r < a$ tạo thành một hệ đại diện của quan hệ tương đương $x \equiv y \pmod{a}$ trên $\mathbf{Z}$.*

Nếu $x$ là một số nguyên $\geqslant 0$, tồn tại các số nguyên $q$ và $r$ (Lý thuyết tập hợp, III, § 5, no. 6) sao cho $x = aq + r$ và $0 \leqslant r < a$ và $x \equiv r \pmod{a}$. Nếu $x$ là một số nguyên $\leqslant 0$, số nguyên $-x$ là $\geqslant 0$ và theo điều trên tồn tại một số nguyên $r$ sao cho $0 \leqslant r < a$ và $-x \equiv r \pmod{a}$. Đặt $r' = 0$ nếu $r = 0$ và $r' = a - r$ nếu $r > 0$, khi đó

$$
x \equiv -r \equiv r' \pmod{a}
$$

và $0 \leqslant r' < a$. Bây giờ ta chứng minh rằng nếu $0 \leqslant r < r' < a$, thì $r \not\equiv r' \pmod{a}$. Ta có $r' - r < na$ với $n \geqslant 1$ và $r' - r > na$ với $n \leqslant 0$, do đó $r' - r \notin a\mathbf{Z}$.

#### Hệ quả {#alg-i-s4-n10-cor-1 .statement}

*Cho $a$ là một số nguyên $> 0$. Nhóm $\mathbf{Z}/a\mathbf{Z}$ của các số nguyên hữu tỉ modulo $a$ là một nhóm có cấp $a$.*

#### Mệnh đề 17 {#alg-i-s4-prop-17 .statement}

*Cho $\mathrm{H}$ là một nhóm con của $\mathbf{Z}$. Tồn tại duy nhất một số nguyên $a \geqslant 0$ sao cho $\mathrm{H} = a\mathbf{Z}$.*

Nếu $\mathrm{H} = \{0\}$, thì $\mathrm{H} = 0\mathbf{Z}$. Giả sử $\mathrm{H} \neq \{0\}$. Nhóm con $\mathrm{H}$ có một phần tử $x \neq 0$. Khi đó $x > 0$ hoặc $-x > 0$, và do đó $\mathrm{H}$ có những phần tử $> 0$. Gọi $a$ là phần tử nhỏ nhất $> 0$ của $\mathrm{H}$. Nhóm con $a\mathbf{Z}$ sinh bởi $a$ được chứa trong $\mathrm{H}$; ta chứng minh rằng $\mathrm{H} \subset a\mathbf{Z}$. Cho $y \in \mathrm{H}$. Theo Mệnh đề 16, tồn tại một số nguyên $r$ sao cho $y \equiv r \pmod{a}$ và $0 \leqslant r < a$. *A fortiori* $y \equiv r \pmod{\mathrm{H}}$, do đó $r \in \mathrm{H}$. Nhưng điều này chỉ có thể xảy ra nếu $r = 0$ và vì thế $y \in a\mathbf{Z}$. Số nguyên $a$ là duy nhất: nếu $\mathrm{H} = \{0\}$, thì tất yếu $a = 0$, và nếu $\mathrm{H} \neq \{0\}$, số nguyên $a$ là cấp của $\mathbf{Z}/\mathrm{H}$.

#### Định nghĩa 15 {#alg-i-s4-def-15 .statement}

*Một nhóm được gọi là đơn sinh nếu nó thừa nhận một hệ các phần tử sinh gồm một phần tử duy nhất. Một nhóm đơn sinh hữu hạn được gọi là cyclic.*

Mọi nhóm đơn sinh đều giao hoán (no. 3, Hệ quả 2 của Mệnh đề 2). Mọi nhóm thương của một nhóm đơn sinh đều đơn sinh (no. 3, Hệ quả 3 của Mệnh đề 2).

Nhóm cộng $\mathbf{Z}$ là đơn sinh: nó được sinh bởi $\{1\}$. Với mọi số nguyên dương $a$, nhóm $\mathbf{Z}/a\mathbf{Z}$ là đơn sinh, vì nó là một nhóm thương của $\mathbf{Z}$.

#### Mệnh đề 18 {#alg-i-s4-prop-18 .statement}

*Một nhóm đơn sinh hữu hạn cấp a đẳng cấu với $\mathbf{Z}/a\mathbf{Z}$. Một nhóm đơn sinh vô hạn đẳng cấu với $\mathbf{Z}$.*

Cho G là một nhóm đơn sinh (viết theo lối nhân) và x là một phần tử sinh của G. Đồng nhất thức $x^m x^n = x^{m+n}$ (§ 1, no. 3, công thức (1)) cho thấy rằng ánh xạ $n \mapsto x^n$ là một đồng cấu từ $\mathbf{Z}$ vào G. Ảnh của nó là một nhóm con của G chứa x và vì thế là G. Theo no. 5, Định lý 3, nhóm G đẳng cấu với thương của $\mathbf{Z}$ bởi một nhóm con, mà tất yếu có dạng $a\mathbf{Z}$ (Mệnh đề 17). Nếu $a > 0$, nhóm G là hữu hạn cấp a và nếu $a = 0$, nhóm G đẳng cấu với $\mathbf{Z}$.

#### Mệnh đề 19 {#alg-i-s4-prop-19 .statement}

*Cho a là một số nguyên > 0. Cho H là một nhóm con của $\mathbf{Z}/a\mathbf{Z}$, b là cấp của H và c là chỉ số của nó trong $\mathbf{Z}/a\mathbf{Z}$. Khi đó $a = bc$, $H = c\mathbf{Z}/a\mathbf{Z}$ và H đẳng cấu với $\mathbf{Z}/b\mathbf{Z}$.

Ngược lại, cho b và c là hai số nguyên > 0 sao cho $a = bc$. Khi đó $a\mathbf{Z} \subset c\mathbf{Z}$ và $c\mathbf{Z}/a\mathbf{Z}$ là một nhóm con của $\mathbf{Z}/a\mathbf{Z}$, có cấp b và chỉ số c.

$a = bc$ theo no. 4, Hệ quả của Mệnh đề 4. Theo no. 7, Định lý 4, H có dạng $H'/a\mathbf{Z}$, trong đó $H'$ là một nhóm con của $\mathbf{Z}$ và $\mathbf{Z}/H'$ đẳng cấu với $(\mathbf{Z}/a\mathbf{Z})/H$ và do đó có cấp c. Theo Mệnh đề 17 và Hệ quả của Mệnh đề 16, $H' = c\mathbf{Z}$ và do đó H là đơn sinh. Sau cùng, H đẳng cấu với $\mathbf{Z}/b\mathbf{Z}$ theo Mệnh đề 18. Ngược lại, nếu $a = bc$, thì $a\mathbf{Z} \subset c\mathbf{Z}$ vì $a \in c\mathbf{Z}$: nhóm thương $(\mathbf{Z}/a\mathbf{Z})/(c\mathbf{Z}/a\mathbf{Z})$ đẳng cấu với $\mathbf{Z}/c\mathbf{Z}$ (no. 7, Định lý 4) và do đó có cấp c (no. 4, Hệ quả của Mệnh đề 4) và chỉ số b (no. 4, Hệ quả của Mệnh đề 4).

#### Hệ quả {#alg-i-s4-n10-cor-2 .statement}

*Mọi nhóm con của một nhóm đơn sinh đều đơn sinh.*

Cho a và b là hai số nguyên $\neq 0$. Quan hệ $b \in a\mathbf{Z}$ cũng được viết là: *b là một bội của a*, và cũng là *a chia b* hoặc *a là một ước của b*.

#### Định nghĩa 16 {#alg-i-s4-def-16 .statement}

*Một số nguyên $p > 0$ được gọi là nguyên tố nếu $p \neq 1$ và nó không nhận ước nào > 1 ngoài p.*

#### Mệnh đề 20 {#alg-i-s4-prop-20 .statement}

*Một số nguyên $p > 0$ là nguyên tố khi và chỉ khi nhóm $\mathbf{Z}/p\mathbf{Z}$ là một nhóm đơn.*

Điều này suy ra từ Mệnh đề 19.

#### Hệ quả {#alg-i-s4-n10-cor-3 .statement}

*Mọi nhóm đơn giao hoán đều là cyclic cấp nguyên tố.*

Cho G là một nhóm như vậy. Khi đó $G \neq \{e\}$; lấy $a \neq e$ là một phần tử của G. Nhóm con sinh bởi a là chuẩn tắc vì G giao hoán, nó không bị quy về $\{e\}$ và do đó bằng G. Vậy nên G là đơn sinh và do đó đẳng cấu với một nhóm có dạng $\mathbf{Z}/p\mathbf{Z}$ với $p > 0$, vì $\mathbf{Z}$ không đơn, và p tất yếu là nguyên tố.

#### Nhận xét {#alg-i-s4-n10-rem-1 .statement}

Một nhóm hữu hạn G có cấp nguyên tố tất yếu là cyclic. G không có nhóm con nào ngoài G và $\{e\}$ và do đó nó được sinh bởi mọi phần tử $\neq e$.

#### Bổ đề 2 {#alg-i-s4-lem-2 .statement}

Cho $a$ là một số nguyên $> 0$. Khi gán cho mỗi chuỗi hợp thành $(\mathbf{H}_i)_{0 \leq i \leq n}$ của nhóm $\mathbf{Z}/a\mathbf{Z}$ dãy $(s_i)_{1 \leq i \leq n}$, trong đó $s_i$ là cấp của $\mathbf{H}_{i-1}/\mathbf{H}_i$, ta thu được một sự tương ứng một-một giữa các chuỗi hợp thành của $\mathbf{Z}/a\mathbf{Z}$ và các dãy hữu hạn $(s_i)$ gồm các số nguyên $> 0$ sao cho $a = s_1 \ldots s_n$. Chuỗi hợp thành $(\mathbf{H}_i)_{0 \leq i \leq n}$ là một chuỗi Jordan-Hölder khi và chỉ khi các $s_i$ là nguyên tố.

Nếu $(\mathbf{H}_i)_{0 \leq i \leq n}$ là một chuỗi hợp thành của $\mathbf{Z}/a\mathbf{Z}$, thì suy ra, bằng quy nạp theo $n$, từ no. 4, Mệnh đề 4, rằng $a = \prod_{i=1}^n (\mathbf{H}_{i-1} : \mathbf{H}_i)$.

Ngược lại, cho $(s_i)_{1 \leq i \leq n}$ là một dãy số nguyên $> 0$ sao cho $a = s_1 \ldots s_n$. Nếu $(\mathbf{H}_i)_{0 \leq i \leq n}$ là một chuỗi hợp thành của $\mathbf{Z}/a\mathbf{Z}$ sao cho $(\mathbf{H}_{i-1} : \mathbf{H}_i) = s_i$ với $1 \leq i \leq n$, thì tất yếu $((\mathbf{Z}/a\mathbf{Z}) : \mathbf{H}_i) = \prod_{1 \leq j \leq i} s_j$ như thấy được bằng quy nạp theo $i$, do đó $\mathbf{H}_i = \left( \prod_{j=1}^i s_j \right) \mathbf{Z}/a\mathbf{Z}$ (Mệnh đề 19), điều này chứng tỏ tính đơn ánh của ánh xạ đang xét. Bây giờ ta sẽ chứng minh tính toàn ánh của nó. Đặt $\mathbf{H}_i = \left( \prod_{j=1}^i s_j \right) \mathbf{Z}/a\mathbf{Z}$ với $0 \leq i \leq n$, ta thu được một chuỗi hợp thành của $\mathbf{Z}/a\mathbf{Z}$ sao cho $(\mathbf{H}_{i-1} : \mathbf{H}_i) = s_i$ (Mệnh đề 19). Mệnh đề thứ hai suy ra từ Mệnh đề 20 và no. 7, Mệnh đề 9.

Ký hiệu $\mathfrak{P}$ là tập hợp các số nguyên tố.

#### Định lý 7 (phân tích thành các thừa số nguyên tố) {#alg-i-s4-thm-7 .statement}

*Cho $a$ là một số nguyên dương ngặt. Tồn tại một và chỉ một họ $(v_p(a))_{p \in \mathfrak{P}}$ các số nguyên $> 0$ sao cho tập hợp các $p \in \mathfrak{P}$ với $v_p(a) \neq 0$ là hữu hạn và*

$$
a = \prod_{p \in \mathfrak{P}} p^{v_p(a)}.
$$

Vì nhóm $\mathbf{Z}/a\mathbf{Z}$ là hữu hạn, nó có một chuỗi Jordan-Hölder. Khi đó Bổ đề 2 suy ra rằng $a$ là một tích các số nguyên tố, do đó có sự tồn tại của họ $(v_p(a))$; hơn nữa, đối với mọi họ $(v_p(a))_{p \in \mathfrak{P}}$ thỏa mãn các điều kiện của Định lý 7, số nguyên $v_p(a)$, với mọi $p \in \mathfrak{P}$, bằng số các thừa số của một chuỗi Jordan-Hölder của $\mathbf{Z}/a\mathbf{Z}$ đẳng cấu với $\mathbf{Z}/p\mathbf{Z}$ (Bổ đề 2). Vì thế tính duy nhất của họ $(v_p(a))$ suy ra từ định lý Jordan-Hölder (no. 7, Định lý 6).

#### Hệ quả {#alg-i-s4-n10-cor-4 .statement}

*Cho $a$ và $b$ là hai số nguyên $> 0$. Khi đó $v_p(ab) = v_p(a) + v_p(b)$. Để $a$ chia hết $b$, điều kiện cần và đủ là $v_p(a) \leq v_p(b)$ với mọi số nguyên tố $p$.*

Trong mọi nhóm $G$, nếu nhóm con (đơn sinh) sinh bởi một phần tử $x \in G$ có cấp hữu hạn $d$, thì $x$ được gọi là một phần tử có *cấp* $d$; do đó số $d$ là số nguyên nhỏ nhất $> 0$ sao cho $x^d = e$; nếu nhóm con sinh bởi $x$ là vô hạn, thì $x$ được gọi là có *cấp vô hạn*. Đặc biệt, các định nghĩa này, cùng với Mệnh đề 4 (no. 4), kéo theo rằng trong một nhóm hữu hạn G, cấp của mọi phần tử của G là một ước của cấp của G.

#### Mệnh đề 21 {#alg-i-s4-prop-21 .statement}

Trong một nhóm hữu hạn G có cấp n, $x^n = e$ với mọi $x \in G$.

Nếu $p$ là cấp của $x$, thì $n = pq$, với $q$ là một số nguyên, và do đó $x^n = (x^p)^q = e$.

### Bài tập {#alg-i-s4-exercises}

Xem [bài tập của § 4](exercises/s4/).
