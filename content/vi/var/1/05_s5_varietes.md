---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 5
section_title: Variétés
lang: vi
source: var-fr
pdf_pages: 0033-0058
extraction: ocr
subsections:
    - "no": 1
      title: Cartes et atlas. Variétés
      page: 0
      pdf_page: 33
    - "no": 2
      title: Exemples de variétés
      page: 0
      pdf_page: 35
    - "no": 3
      title: Fonctions de classe $C^r$ et morphismes de variétés
      page: 0
      pdf_page: 36
    - "no": 4
      title: Caractérisation des variétés par leurs faisceaux de fonctions
      page: 0
      pdf_page: 38
    - "no": 5
      title: Espaces tangents, applications linéaires tangentes
      page: 0
      pdf_page: 39
    - "no": 6
      title: Produits de variétés
      page: 0
      pdf_page: 42
    - "no": 7
      title: Immersions, morphismes étales
      page: 0
      pdf_page: 43
    - "no": 8
      title: Images inverses de structures de variété, sous-variétés
      page: 0
      pdf_page: 45
    - "no": 9
      title: Submersions et variétés quotients
      page: 0
      pdf_page: 48
    - "no": 10
      title: Subimmersions
      page: 0
      pdf_page: 50
    - "no": 11
      title: Produits fibrés et images réciproques
      page: 0
      pdf_page: 51
    - "no": 12
      title: Variétés de groupes
      page: 0
      pdf_page: 54
    - "no": 13
      title: Affaiblissement de structure
      page: 0
      pdf_page: 56
    - "no": 14
      title: Restriction du corps de base
      page: 0
      pdf_page: 56
statements: 0
exercises: 0
content_sha256: c469f429fb9bcbafd84aec0de53595c8f216eae6cbab806a4086221bd87d5bbb
translated_from: content/en-mt/var/1/05_s5_varietes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: de22b9b5756c12da2b4ad3436a436907dc19032fe6854a0c443ce26f695214a5
translation_model: gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-65020df8
glossary_version: 34
glossary_terms_sha256: da6708055e7d8bd267729f74b0e7809901993f866a05719870129ac73a7dddaa
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. Các đa tạp

### 5.1. Các biểu đồ và atlas. Các đa tạp

5.1.1. Cho X là một tập hợp. Một biểu đồ của X là một bộ ba c = (U, φ, E), trong đó U là một tập con của X, E là một không gian Banach và φ là một song ánh của U lên một tập con mở của E. Ta nói rằng U là miền của biểu đồ c. Nếu E có số chiều hữu hạn n, ta nói rằng c có chiều n. Ngược lại, ta đặt dim c = +∞.

5.1.2. Ta nói rằng hai biểu đồ c = (U, φ, E) và c' = (U', φ', E') của X là tương thích C^r (hoặc đơn giản là tương thích khi không thể có sự nhập nhằng về r) khi các điều kiện sau được thỏa mãn:
(a) φ(U ∩ U') (resp. φ'(U ∩ U')) là mở trong E (resp. E');
(b) ánh xạ φ ∘ φ'^{-1} (resp. φ' ∘ φ^{-1}) của φ'(U ∩ U') lên φ(U ∩ U') (resp. của φ(U ∩ U') lên φ'(U ∩ U')) là thuộc lớp C^r (xem 2.3.1, 3.2.1 và 4.2.1).

5.1.3. Một atlas C^r (hoặc đơn giản là atlas) của một tập hợp X là một tập hợp các biểu đồ của X tương thích C^r từng đôi một có các miền hợp lại thành chính X. Hai atlas A và B của X được gọi là tương đương C^r nếu A ∪ B là một atlas. Quan hệ tương đương C^r giữa các atlas là một quan hệ tương đương.

5.1.4. Cho S là một tập hợp các không gian Banach. Ta nói rằng một atlas A có kiểu S nếu E ∈ S đối với mọi biểu đồ c = (U, φ, E) của A. Theo cách tương tự, ta nói rằng một atlas A có kiểu Hilbert (resp. kiểu Hilbert có số chiều đếm được) nếu E là một không gian Hilbert (resp. một không gian Hilbert kiểu đếm được) đối với mọi biểu đồ (U, φ, E) của A.

5.1.5. Một K-đa tạp lớp C^r (hoặc một đa tạp lớp C^r trên K, hoặc đơn giản là một đa tạp khi không thể có sự nhập nhằng về K và r) là một tập hợp X được trang bị một lớp các atlas tương đương (Ens., chap. II, § 6, No. 9) đối với quan hệ tương đương C^r. Một atlas của lớp này được gọi là một atlas của đa tạp X. Một biểu đồ thuộc một atlas của X được gọi là một biểu đồ của đa tạp X. Một biểu đồ của X có miền chứa một điểm a ∈ X được gọi là một biểu đồ của X tại a. Một biểu đồ tâm tại a là một biểu đồ (U, φ, E) của X tại a sao cho φ(a) = 0.

Nếu X là một tập hợp và A là một atlas của X, tập hợp X được trang bị lớp tương đương của A được gọi là đa tạp xác định bởi A.

Khi r ≠ ω (do đó K = R), một đa tạp lớp C^r đôi khi được gọi là một đa tạp vi phân. Một đa tạp lớp C^ω cũng được gọi là một đa tạp giải tích trên K (hoặc K-đa tạp giải tích).

Khi thêm vào đó $K = \mathbf{R}$ (resp. $\mathbf{C}$, $\mathbf{Q}_p$), ta cũng nói đa tạp giải tích thực (resp. đa tạp giải tích phức, $p$-adic đa tạp giải tích).

5.1.6. Cho $X$ là một đa tạp. Các tập con của $X$ là các hợp của các miền của các biểu đồ của $X$ tạo thành tập hợp các tập con mở đối với một tôpô trên $X$, được gọi là tôpô nằm dưới cấu trúc đa tạp của $X$. Đối với mọi biểu đồ $c = (U, \varphi, E)$ của $X$, ánh xạ $\varphi$ là một đồng phôi từ tập con mở $U$ được trang bị tôpô cảm sinh bởi tôpô của $X$ lên tập con mở $\varphi(U)$ của $E$.

Không gian tôpô nằm dưới $X$ là một không gian Baire. Khi $K$ bằng $\mathbf{R}$ hoặc $\mathbf{C}$, nó là liên thông địa phương.

Cho $X$ là một đa tạp và cho $\mathcal{A}$ là một atlas của $X$. Để không gian tôpô $X$ là tách, điều kiện cần và đủ là điều kiện sau được thỏa mãn: với mọi các biểu đồ $(U, \varphi, E)$ và $(V, \psi, F)$ thuộc atlas $\mathcal{A}$, đồ thị của ánh xạ $\psi \circ \varphi^{-1}$ từ $\varphi(U \cap V)$ vào $\psi(U \cap V)$ là đóng trong $\varphi(U) \times \psi(V)$.

Cho $X$ là một đa tạp; giả sử rằng không gian tôpô $X$ là chính quy. Khi đó đối với mọi điểm $a \in X$, tồn tại một biểu đồ $(U, \varphi, E)$ của $X$ tại $a$ có tính chất sau: để một tập con $Y$ của $U$ là đóng trong $X$, điều kiện cần và đủ là ảnh của nó $\varphi(Y)$ là đóng trong $E$. Nếu không gian $X$ là paracompact, tồn tại trên $X$ một khoảng cách tương thích với tôpô của $X$ và làm cho $X$ là một không gian mêtric đầy đủ.

5.1.7. Cho $\mathfrak{S}$ là một tập hợp các không gian Banach. Ta nói rằng một đa tạp có kiểu $\mathfrak{S}$ (resp. kiểu Hilbert, resp. kiểu Hilbert có số chiều đếm được) nếu nó sở hữu một atlas kiểu $\mathfrak{S}$ (resp. kiểu Hilbert, resp. kiểu Hilbert có số chiều đếm được). Nếu $\mathfrak{S}$ được rút gọn thành một phần tử duy nhất $E$, một đa tạp kiểu $\mathfrak{S}$ cũng được gọi là một đa tạp thuần túy kiểu $E$.

Một đa tạp thuần túy chiều $n$ là một đa tạp thuần túy kiểu $K^n$. Ta nói rằng một đa tạp là địa phương có số chiều hữu hạn nếu nó có kiểu $\mathfrak{S}$ với $\mathfrak{S} = \{ K^n ; n \in \mathbf{N} \}$.

5.1.8. Cho $X$ là một đa tạp và cho $x \in X$. Chiều (hữu hạn hoặc $+\infty$) của một biểu đồ của $X$ tại $x$ chỉ phụ thuộc vào $x$. Nó được gọi là chiều của $X$ tại $x$ và được ký hiệu bởi $\dim_x X$. Chiều của $X$, được ký hiệu bởi $\dim X$, là cận trên đúng của các $\dim_x X$ với $x \in X$.

Ánh xạ $x \mapsto \dim_x X$ là hằng địa phương. Đa tạp $X$ là địa phương hữu hạn chiều (tương ứng thuần túy có chiều $n$) khi và chỉ khi $\dim_x X < +\infty$ (tương ứng $\dim_x X = n$) với mọi $x \in X$.

5.1.9. Giả sử $K$ là compact địa phương. Cho $X$ là một đa tạp tách. Khi đó, để $X$ là địa phương hữu hạn chiều, điều kiện cần và đủ là $X$ compact địa phương.

No. 5.2

5.1.10. Cho X là một đa tạp và cho $\xi^1, \ldots, \xi^n$ là các ánh xạ của một tập con U của X vào K. Ta nói rằng $\xi = (\xi^1, \ldots, \xi^n)$ là một hệ tọa độ của X trong U nếu bộ ba $(U, \xi, K^n)$ là một biểu đồ của X; biểu đồ này cũng được ký hiệu bởi $(U; \xi)$ hoặc $(U; \xi^1, \ldots, \xi^n)$. Nếu $a \in U$, ta cũng nói rằng $\xi$ là một hệ tọa độ của X tại $a$; nếu thêm vào đó $\xi^i(a) = 0$ với $i = 1, 2, \ldots, n$, ta nói rằng hệ tọa độ $\xi$ được tâm hóa tại $a$.

### 5.2. Các ví dụ về đa tạp

5.2.1. Cho X là một tập hợp; trên X tồn tại duy nhất một cấu trúc đa tạp mà không gian tôpô nền là rời rạc; cấu trúc này là một cấu trúc đa tạp thuần túy 0-chiều.

5.2.2. Cho E là một không gian Banach. Bộ ba $c = (E, \mathrm{Id}_E, E)$ là một biểu đồ của E và $\mathcal{A} = {c}$ là một tập bản đồ của E, và do đó xác định một cấu trúc đa tạp thuần túy kiểu E trên E; tôpô nền là tôpô đã cho trên E. Trong những điều sau đây, mỗi khi ta nói về cấu trúc đa tạp trên E, ta sẽ luôn quy chiếu đến cấu trúc trước đó.

Đặc biệt, điều này áp dụng cho mọi không gian vectơ hữu hạn chiều trên K, được trang bị tôpô tách duy nhất tương thích với cấu trúc vectơ của nó (Esp. Vect. Top., chap. I, § 2, No. 3).

5.2.3. Cho X là một đa tạp và U là một tập con mở của X. Trên U tồn tại một cấu trúc đa tạp mà các biểu đồ của nó là các biểu đồ của đa tạp X có miền được chứa trong U. Cấu trúc này được nói là cảm sinh bởi cấu trúc của X (cf. No. 5.3.4); được trang bị cấu trúc này, U được gọi là một đa tạp con mở của X.

Đặc biệt, mọi tập con mở của một không gian Banach E đều được trang bị một cấu trúc đa tạp thuần túy chính tắc kiểu E. Cho X là một đa tạp; để một bộ ba $(U, \varphi, E)$ là một biểu đồ của X, điều kiện cần và đủ là U mở trong X và $\varphi$ là một đẳng cấu từ đa tạp con mở U của X lên một đa tạp con mở của E.

5.2.4. Cho X là một tập hợp, và $(X_i)_{i \in I}$ là một phủ của X. Giả sử rằng mỗi $X_i$ được trang bị một cấu trúc đa tạp sao cho điều kiện sau được thỏa mãn:

Với mọi $i$ và $j$ trong I, tập hợp $X_i \cap X_j$ là mở trong $X_i$ và $X_j$ và các cấu trúc đa tạp cảm sinh trên $X_i \cap X_j$ bởi các cấu trúc của $X_i$ và $X_j$ trùng nhau.

Khi đó trên X tồn tại duy nhất một cấu trúc đa tạp sao cho $X_i$ là một đa tạp con mở của X với mọi $i$ trong I. Ta nói rằng đa tạp X thu được bằng cách dán các đa tạp $X_i$.

5.2.5. Cho X là một đa tạp. Tập hợp $X_n$ gồm các điểm $x$ của X sao cho dim_x X = n (n số nguyên $\geq 0$) là một đa tạp con mở của X, thuần túy có chiều n.

5.2.6. Cho E là một không gian Banach. Tập hợp G(E) các không gian con vectơ của E thừa nhận một phần bù tôpô có thể được trang bị một cấu trúc đa tạp giải tích theo cách sau: với mọi cặp (F_0, G_0) $\in G(E) \times G(E)$ sao cho E = F_0 $\oplus$ G_0, ký hiệu U_{G_0} là tập hợp các F $\in G(E)$ thừa nhận G_0 làm phần bù, và định nghĩa một song ánh $\varphi_{F_0, G_0}$ của U_{G_0} lên không gian Banach $\mathcal{L}(F_0; G_0)$ bằng cách gán cho mỗi F $\in U_{G_0}$ ánh xạ từ F_0 vào G_0 có đồ thị là không gian con F của E = F_0 $\times$ G_0. Các bản đồ địa phương (U_{G_0}, $\varphi_{F_0, G_0}$, $\mathcal{L}(F_0; G_0)$) tạo thành một atlas của G(E). Được trang bị cấu trúc đa tạp được định nghĩa bởi atlas này, G(E) được gọi là đa tạp Grassmann của E.

Không gian tôpô G(E) là mêtric hóa được. Nếu K là compact địa phương và E hữu hạn chiều, G(E) là compact.

Với mọi số nguyên $n \geq 0$, tập hợp G_n(E) (tương ứng G^n(E)) của các F $\in G(E)$ có chiều (tương ứng đối chiều) n là mở và đóng trong G(E) và là một đa tạp con mở thuần túy của G(E). Nếu K = R hoặc C, G_n(E) liên thông với mọi n.

Ánh xạ gán cho F $\in G(E)$ phần trực giao của nó trong không gian đối ngẫu E’ của E là một cấu xạ từ G(E) vào G(E’) cảm sinh một đẳng cấu của G^n(E) lên G_n(E’) với mọi số nguyên n.

Nếu K = R hoặc C, hoặc nếu E hữu hạn chiều, G_1(E) không gì khác ngoài không gian xạ ảnh suy ra từ E, do đó được trang bị một cấu trúc đa tạp giải tích.

### 5.3. Các hàm thuộc lớp $C^r$ và các cấu xạ của các đa tạp

5.3.1. Cho X là một đa tạp thuộc lớp C', F là một không gian đa chuẩn phân ly và f là một ánh xạ từ X vào F. Ta nói rằng f thuộc lớp C' nếu với mọi bản đồ địa phương (V, $\varphi$, E) của X, ánh xạ $f \circ \varphi^{-1}$ từ $\varphi(V)$ vào F thuộc lớp C'. Đối với điều này, chỉ cần điều kiện này được thỏa mãn đối với các bản đồ địa phương của một atlas của X. Tập hợp các ánh xạ thuộc lớp C' từ X vào F tạo thành một không gian con vectơ của không gian tất cả các ánh xạ từ X vào F. Nó được ký hiệu bởi $\mathcal{C}'(X; F)$.

Khi F = K, ta đặt $\mathcal{C}'(X; K) = \mathcal{C}'(X)$; đây là một đại số con trên K của đại số các ánh xạ từ X vào K. Các phần tử của $\mathcal{C}'(X)$ cũng được gọi là các hàm cấu xạ.

Khi X là một tập con mở của một không gian Banach, thuật ngữ này phù hợp với thuật ngữ của No. 2.3.1, 3.2.1 và 4.2.1.

5.3.2. Cho X và Y là hai đa tạp thuộc lớp C' và cho f là một ánh xạ từ X vào Y. Ta nói rằng f thuộc lớp C' hoặc là một cấu xạ của các đa tạp (thuộc lớp C') nếu nó liên tục và nếu, với mọi bản đồ địa phương (V, $\psi$, F) của Y, ánh xạ $\psi \circ f$ từ đa tạp con mở $f^{-1}(V)$ vào không gian Banach F thuộc lớp $C'$. Đối với điều này, chỉ cần tồn tại một atlas $\mathcal{A}$ của Y sao cho, với mọi bản đồ địa phương $(V, \psi, F) \in \mathcal{A}$, tập hợp $f^{-1}(V)$ là mở trong X và ánh xạ $\psi \circ f$ từ đa tạp con mở $f^{-1}(V)$ của X vào F thuộc lớp $C'$. Tập hợp các cấu xạ từ X vào Y được ký hiệu bởi $\mathcal{C}'(X; Y)$. Khi Y là một không gian Banach được trang bị cấu trúc đa tạp chính tắc của nó, các định nghĩa của 5.3.1. và 5.3.2 là nhất quán. Một ánh xạ thuộc lớp $C^\omega$ cũng được gọi là một *ánh xạ K-giải tích* (hoặc đơn giản là giải tích). Khi $K = \mathbf{C}$, người ta cũng nói là ánh xạ chỉnh hình.

Cho $(U, \varphi, E)$ là một bản đồ địa phương của X và $(V, \psi, F)$ là một bản đồ địa phương của Y sao cho $f(U) \subset V$. Ánh xạ $\psi \circ f \circ \varphi^{-1}$ từ tập hợp mở $\varphi(U)$ của E vào tập hợp mở $\psi(V)$ của F được gọi là *biểu thức của f* trong các bản đồ địa phương đã cho.

5.3.3. Giả sử X và Y hữu hạn chiều; cho $a \in X,\ b \in Y$ và f là một ánh xạ từ X vào Y với $f(a) = b$. Trước hết giả sử rằng f thuộc lớp C' và xét các hệ tọa độ $(U; \xi^1, \ldots, \xi^m)$ của X tại a và $(V; \eta^1, \ldots, \eta^n)$ của Y tại b tương ứng, với $f(U) \subset V$. Gọi $\xi$ là ánh xạ $(\xi^1, \ldots, \xi^m)$ từ U vào $K^m$. Khi đó tồn tại các hàm $u^j$ thuộc lớp C' trên tập hợp mở $\xi(U)$ của $K^m$, với giá trị trong K, sao cho các tọa độ của một điểm $y = f(x)$ của Y, (với x trong U), được cho bởi các công thức:

(1)
$$
\eta^j(y) = u^j(\xi^1(x), \ldots, \xi^m(x)) \quad \text{for } 1 \leq j \leq n
$$
tương đương với:

(2)
$$
\eta^j \circ f = u^j(\xi^1, \ldots, \xi^m) \quad \text{for } 1 \leq j \leq n.
$$
Ta nói rằng các công thức trên tạo thành *biểu thức* của $f$ bằng các hệ tọa độ đã chọn.

*bó các hàm lấy giá trị trong* $Y$ nếu nó thỏa mãn điều kiện sau:

*Cho* $(U_i)_{i \in I}$ *là một họ các tập mở của* $X$, *với hợp là* $U$, *và cho* $f$ *là một ánh xạ từ* $U$ *vào* $Y$; *để* $f$ *thuộc* $\mathcal{L}(U)$, *điều kiện cần và đủ là* $f|U_i$ *thuộc* $\mathcal{L}(U_i)$ *với mọi* $i$ *trong* $I$.

5.4.2. Cho $X$ và $Y$ là hai đa tạp; với mỗi tập mở $U \subset X$, cho $\mathcal{L}(U)$ là tập hợp các cấu xạ từ $U$ vào $Y$; khi đó $\mathcal{L}$ là một bó các ánh xạ có giá trị trong $Y$.

Khi $Y = K$, bó được xác định như vậy được ký hiệu bởi $\mathscr{C}_X^{r'}$.

5.4.3. Cho $X$ là một không gian tôpô và cho $\mathcal{S}$ là một tập hợp các không gian Banach. Với mỗi $E \in \mathcal{S}$, cho $\mathcal{F}_E$ là một bó các ánh xạ trên $X$ có giá trị trong $E$. Giả sử rằng họ các $\mathcal{F}_E$, với $E \in \mathcal{S}$, thỏa mãn điều kiện sau:

Với mỗi $x \in X$, tồn tại một lân cận mở $U$ của $x$, một không gian

$E_0 \in \mathcal{S}$, và một đồng phôi $\varphi$ từ U lên một tập mở của E_0, sao cho, với mỗi tập mở $V \subset U$ và mỗi $E \in \mathcal{S}$, tập hợp $\mathcal{F}_E(V)$ gồm các hàm $g \circ \varphi$, trong đó $g$ chạy qua không gian $\mathcal{C}^r(\varphi(V); E)$.

Khi đó tồn tại trên X một cấu trúc của đa tạp cấp $C^r$ và kiểu $\mathcal{S}$, và chỉ một cấu trúc như vậy, tương thích với tôpô đã cho trên X và sao cho $\mathcal{F}_E$ là bó các hàm cấp $C^r$ trên X có giá trị trong E.

5.4.4. Cho X là một không gian tôpô và cho $\mathcal{F}$ là một bó các hàm có giá trị trong K, thỏa mãn điều kiện sau: với mỗi điểm x của X, tồn tại một số nguyên n, một lân cận mở U của x và một đồng phôi $\varphi$ từ U lên một tập mở của $K^n$, sao cho, với mỗi tập mở V của U, tập hợp $\mathcal{F}(V)$ gồm các hàm $g \circ \varphi$ trong đó $g$ chạy qua tập hợp các hàm cấp $C^r$ có giá trị trong K trên tập mở $\varphi(V)$ của $K^n$.

Khi đó tồn tại trên X một cấu trúc của đa tạp hữu hạn chiều địa phương cấp $C^r$ và chỉ một cấu trúc như vậy sao cho $\mathcal{F} = \mathcal{C}^r_X$.

5.4.5. Cho $X$ và $X'$ là hai đa tạp lớp $C^r$, địa phương có số chiều hữu hạn, và cho $f$ là một ánh xạ liên tục từ X vào X'. Để $f$ là một cấu xạ, điều kiện cần và đủ là với mọi tập mở U' của X' và mọi hàm $g \in \mathcal{C}^r(U'; K)$, hàm $g \circ f$ thuộc $\mathcal{C}^r(U; K)$, trong đó $U = f^{-1}(U')$.

### 5.5. Các không gian tiếp xúc, các ánh xạ tuyến tính tiếp xúc

5.5.1. Cho X là một đa tạp và cho $a \in X$. Xét các cặp $(c, h)$ trong đó $c = (U, \varphi, E)$ là một biểu đồ của đa tạp X tại $a$ và $h$ là một phần tử của E. Hai cặp như vậy $(c, h)$ và $(c', h')$ được gọi là tương đương nếu đạo hàm tại $\varphi(a)$ của ánh xạ $\varphi' \circ \varphi^{-1}$ (được xác định trên một lân cận của $\varphi(a)$) biến đổi $h$ thành $h'$. Do đó ta thu được một quan hệ tương đương giữa các cặp $(c, h)$ và gọi một vectơ tiếp xúc tại $a$ của X là một lớp các cặp tương đương $(c, h)$ (Ens., Chương II, § 6, No. 9).

Các vectơ tiếp xúc tại $a$ của X tạo thành một tập hợp được ký hiệu bởi $T_a(X)$. Nếu $c = (U, \varphi, E)$ là một biểu đồ của đa tạp X tại $a$, ánh xạ $\theta_c$ từ E vào $T_a(X)$ gán cho một phần tử $h$ của E vectơ tiếp xúc được biểu diễn bởi cặp $(c, h)$ là một song ánh. Nếu ta chuyển sang $T_a(X)$, bằng cách sử dụng $\theta_c$, cấu trúc của không gian vectơ tôpô K của E, thì cấu trúc thu được như vậy không phụ thuộc vào lựa chọn của $c$ và biến $T_a(X)$ thành một không gian Banach, được gọi là không gian tiếp xúc của X tại $a$. Chiều (hữu hạn hoặc $+\infty$) của $T_a(X)$ bằng chiều của X tại $a$.

5.5.2. Cho X, Y là hai đa tạp, $f$ là một cấu xạ từ X vào Y và $a$ là một điểm của X. Xét một biểu đồ $c = (U, \varphi, E)$ của X tại $a$ và một biểu đồ $c' = (V, \psi, F)$ của Y tại $b$ với $f(U) \subset V$; ánh xạ $\Phi = \psi \circ f \circ \varphi^{-1}$ từ $\varphi(U)$ vào F là thuộc lớp $C^r$, và đạo hàm của nó $D\Phi(\varphi(a))$ tại điểm $\varphi(a)$ là một ánh xạ tuyến tính liên tục từ E vào F. Ánh xạ tuyến tính liên tục $\theta_{c'} \circ D\Phi(\varphi(a)) \circ \theta_c^{-1}$ từ $T_a(X)$ vào $T_b(Y)$ không phụ thuộc vào các biểu đồ $c$ và $c'$ đã chọn; nó được ký hiệu là $T_a(f)$ và được gọi là ánh xạ tuyến tính tiếp xúc của $f$ tại $a$. Nếu $g$ là một cấu xạ từ $Y$ vào một đa tạp $Z$, ta có:

$$
T_a(g \circ f) = T_{f(a)}(g) \circ T_a(f).
$$

5.5.3. Cho $f : X \to Y$ là một cấu xạ của các đa tạp. Nếu $f$ là hằng địa phương, ta có $T_a(f) = 0$ với mọi $a$ trong $X$. Ngược lại, nếu $T_a(f) = 0$ với mọi $a \in X$ và nếu trường $K$ có đặc số 0, thì $f$ là hằng địa phương.

5.5.4. Cho $U$ là một tập hợp mở của một đa tạp $X$ và $f$ là đơn ánh chính tắc của $U$ vào $X$; với mọi điểm $a$ của $U$, ánh xạ $T_a(f)$ từ $T_a(U)$ vào $T_a(X)$ là một đẳng cấu của các không gian vectơ tôpô, nhờ đó hai không gian này từ nay về sau sẽ được đồng nhất.

5.5.5. Cho $U$ là một tập hợp mở của một không gian Banach $E$; nếu $\iota$ là đơn ánh chính tắc của $U$ vào $E$, bộ ba $c = (U, \iota, E)$ là một biểu đồ của $U$, và atlas $\{c\}$ xác định cấu trúc đa tạp của $U$. Cho một điểm $a$ của $U$, ánh xạ $\theta_c$ là một đẳng cấu của các không gian vectơ tôpô từ $E$ lên $T_a(U)$; đẳng cấu nghịch đảo sẽ được ký hiệu bởi $\zeta_E(a)$.

Cho $f$ là một ánh xạ thuộc lớp $C^r$ từ $U$ vào một tập mở $V$ của một không gian Banach $F$; với mọi điểm $a$ của $U$, ta có:

$$
Df(a) \circ \zeta_E(a) = \zeta_F(f(a)) \circ T_a(f)
$$

trong đó $Df(a)$ là đạo hàm của $f$ tại $a$ (1.2.1). Nói cách khác, biểu đồ:

$$
\begin{array}{ccc}
T_a(U) & \xrightarrow{T_a(f)} & T_{f(a)}(V) \\
\downarrow \zeta_E(a) & & \downarrow \zeta_F(f(a)) \\
E & \xrightarrow{Df(a)} & F
\end{array}
$$

là giao hoán.

5.5.6. Một vectơ đối tiếp xúc của $X$ tại $a$, hay còn gọi là một đối vectơ tiếp xúc hoặc đơn giản là một đối vectơ tại $a$, là một dạng tuyến tính liên tục bất kỳ trên không gian vectơ tôpô $T_a(X)$; do đó các đối vectơ này là các phần tử của đối ngẫu tôpô $T_a(X)'$ của không gian tiếp xúc với $X$ tại $a$. Không gian này sẽ được trang bị tôpô của sự hội tụ đều trên các tập con bị chặn của $T_a(X)$: được trang bị tôpô này, $T_a(X)'$ là một không gian Banach được gọi là không gian đối tiếp xúc của $X$ tại $a$. Nó cũng được ký hiệu bởi $T'_a(X)$.

Cho $f$ là một cấu xạ từ $X$ vào một không gian Banach $E$. Vi phân của $f$ tại $a$, ký hiệu bởi $d_a f$ hoặc $df_a$, là ánh xạ tuyến tính liên tục $\zeta_E(f(a)) \circ T_a(f)$ từ $T_a(X)$ vào $E$. Với $t \in T_a(X)$, đôi khi người ta ký hiệu bởi t(f) hoặc t . f giá trị $d_a f(t)$ của ánh xạ tuyến tính $d_a f$ tại điểm $t$. Ánh xạ $f \mapsto d_a f$ là tuyến tính.

Nếu $E = K$, vi phân $d_a f$ của $f$ tại $a$ là một đối vectơ của $X$ tại $a$.

Cho $E, F, G$ là ba không gian Banach và cho $(u, v) \mapsto u . v$ là một ánh xạ song tuyến tính liên tục từ $F \times G$ vào $E$. Cho $f$ (tương ứng $g$) là một cấu xạ từ $X$ vào $F$ (tương ứng $G$). Khi đó ánh xạ $f . g : x \mapsto f(x) . g(x)$ là một cấu xạ từ $X$ vào $E$ và, với mọi $t \in T_a(X)$, ta có:

$$
d_a(f . g)(t) = f(a) . d_a g(t) + d_a f(t) . g(a).
$$

Xét riêng $G = E$ và $F = K$, ánh xạ song tuyến tính được xét là phép nhân. Khi đó ta có:

$$
d_a(fg) = f(a)d_ag + g(a)\ d_af.
$$

5.5.7. Cho $X$ là một đa tạp hữu hạn chiều địa phương và cho $\xi^1, \ldots, \xi^m$ là các hàm hình thái được xác định trong một lân cận mở $U$ của một điểm $a$ của $X$. Các điều kiện sau là tương đương:

(i) tồn tại một lân cận mở $V$ của $a$ được chứa trong $U$, sao cho các hàm $\xi^i|V$ (với $1 \leq i \leq m$) tạo thành một hệ tọa độ của $X$ trong $V$;

(ii) các vi phân $d_a \xi^i$ với $1 \leq i \leq m$ tạo thành một cơ sở của $T_a(X)'$;

(iii) ánh xạ $\xi = (\xi^1, \ldots, \xi^m)$ của $U$ vào $K^m$ là étale tại $a$ (xem No. 5.7.6).

Để các vi phân $d_a \xi^1, \ldots, d_a \xi^m$ độc lập tuyến tính, điều kiện cần và đủ là tồn tại một lân cận $V$ của $a$, được chứa trong $U$, sao cho các hàm $\xi^i|V$ tạo thành một phần của một hệ tọa độ của $X$ trong $V$.

5.5.8. Cho $X$ là một đa tạp hữu hạn chiều địa phương và cho $\xi = (\xi^1, \ldots, \xi^m)$ là một hệ tọa độ của $X$ trong một tập mở $U$. Cho $a \in U$: ta ký hiệu bởi $(\partial_{1,a}, \ldots, \partial_{m,a})$ cơ sở của không gian tiếp xúc $T_a(X)$ đối ngẫu với cơ sở $(d_a \xi^1, \ldots, d_a \xi^m)$ của $T_a(X)'$. Do đó ta có:

$$
\partial_{i,a}(\xi^j) = \delta_{i,j} \quad \text{(chỉ số Kronecker)}.
$$

Vectơ tiếp xúc $\partial_{i,a}$ còn được ký hiệu bởi $(\partial/\partial \xi^i)_a$.

Cho $f$ là một hàm lớp $C^r$ trên $U$, với các giá trị trong một không gian Banach $E$. Ta ký hiệu bởi $\partial_i f$ hoặc $\partial f/\partial \xi^i$ hàm $a \mapsto \partial_{i,a}(f)$: đây là một hàm lớp $C^{r-1}$ trên $U$ với các giá trị trong $E$ (một hàm liên tục nếu $r = 1$). Giá trị của nó tại một điểm $a$ của $U$ đôi khi được ký hiệu bởi $(\partial f/\partial \xi^i)_a$. Với mọi $t \in T_a(X)$, ta có:

$$
d_a f(t) = \sum_{i=1}^m d_a \xi^i(t) \frac{\partial f}{\partial \xi^i}(a),
$$

cũng có thể được viết:

$$
d_a f = \sum_{i=1}^m \frac{\partial f}{\partial \xi^i}(a) d_a \xi^i.
$$

Các ký hiệu này phù hợp với các ký hiệu của 1.6.3.

5.5.9. Cho $X$ và $Y$ là hai đa tạp và $f$ là một cấu xạ từ $X$ vào $Y$. *Hạng của* $f$ tại một điểm $a$ của $X$, kí hiệu $\mathrm{rg}_a f$, là hạng (hữu hạn hoặc bằng $+\infty$) của ánh xạ tuyến tính $T_a(f)$. Ánh xạ $a \mapsto \mathrm{rg}_a f$ là nửa liên tục dưới.

### 5.6. Tích của các đa tạp

5.6.1. Cho $X$ và $X'$ là hai tập hợp và cho $c = (U, \varphi, E)$ (tương ứng $c' = (U', \varphi, E')$) là một biểu đồ của $X$ (tương ứng $X'$). Bộ ba

$$
(U \times U', \varphi \times \varphi', E \times E')
$$

là một biểu đồ của tập hợp tích $X \times X'$, kí hiệu $c \times c'$.

5.6.2. Cho $X$ và $X'$ là hai đa tạp thuộc lớp $C^r$. Trên tập hợp tích $X \times X'$ tồn tại duy nhất một cấu trúc của một đa tạp thuộc lớp $C^r$ sao cho $c \times c'$ là một biểu đồ của $X \times X'$ đối với mọi biểu đồ $c$ của $X$ và mọi biểu đồ $c'$ của $X'$. Được trang bị cấu trúc này, $X \times X'$ được gọi là *đa tạp tích* của các đa tạp $X$ và $X'$. Ta định nghĩa tương tự tích của mọi số hữu hạn các đa tạp. Tôpô của đa tạp $X \times X'$ là tôpô tích của các tôpô của $X$ và $X'$. Với $a \in X$ và $b \in X'$, ta có:

$$
\dim_{(a,b)}(X \times X') = \dim_a X + \dim_b X'.
$$

5.6.3. Cho $X$ và $X'$ là hai đa tạp, và cho $X \times X'$ là tích của chúng. Cho $a \in X$ và cho $a' \in X'$. Các phép chiếu chính tắc

$$
\mathrm{pr}_1 : X \times X' \to X \quad \text{và} \quad \mathrm{pr}_2 : X \times X' \to X'
$$

là các cấu xạ. Cho $\pi_i \ (i = 1, 2)$ là các ánh xạ tuyến tính tiếp xúc của chúng tại điểm $(a, a')$. Ánh xạ

$$
(\pi_1, \pi_2) : T_{(a,a')}(X \times X') \to T_a(X) \times T_{a'}(X')
$$

là một *đẳng cấu*, điều này cho phép *đồng nhất không gian tiếp xúc của* $X \times X'$ *tại* $(a, a')$ *với tích* $T_a(X) \times T_{a'}(X')$.

Đơn ánh của $T_a(X)$ vào $T_{(a,a')}(X \times X')$ thu được từ sự đồng nhất này là ánh xạ tuyến tính tiếp xúc tại $a$ của cấu xạ $x \mapsto (x, a')$ của $X$ vào $X \times X'$; có một kết quả tương tự đối với đơn ánh của $T_{a'}(X')$ vào $T_{(a,a')}(X \times X')$.

5.6.4. Cho $W, X$ và $X'$ là ba đa tạp, và cho $f : W \to X, f' : W \to X'$ là hai ánh xạ. Đối với ánh xạ

$$
(f, f') : W \to X \times X'
$$

để là một cấu xạ, điều kiện cần và đủ là $f$ và $f'$ là các cấu xạ (điều này biện minh cho việc dùng thuật ngữ « tích », cf. Ens., Chap. IV, § 2, No. 4). Trong trường hợp này, nếu $a$ là một điểm của $W$, ta có:

$$
T_a(f, f') = (T_a(f), T_a(f'))
$$

có tính đến sự đồng nhất đã thực hiện ở trên.

5.6.5. Cho $f : X \to Y$ và $f' : X' \to Y'$ là các cấu xạ của các đa tạp. Khi đó $f \times f' : X \times X' \to Y \times Y'$ là một cấu xạ. Nếu $a \in X$ và $a' \in X'$, ta có:

$$
T_{(a, a')}(f \times f') = T_a(f) \times T_{a'}(f')
$$
$$
\mathrm{rg}_{(a, a')}(f \times f') = \mathrm{rg}_a f + \mathrm{rg}_{a'} f'.
$$

5.6.6. Cho $X_1, X_2$ và $Z$ là ba đa tạp và $f$ là một cấu xạ từ $X_1 \times X_2$ vào $Z$. Cho $a \in X_1$ và $b \in X_2$. Ánh xạ tuyến tính tiếp xúc của ánh xạ riêng phần $x \mapsto f(x, b)$ (tương ứng $y \mapsto f(a, y)$) của $X_1$ (tương ứng $X_2$) vào $Z$ được ký hiệu là $T^1_{(a, b)}(f)$ (tương ứng $T^2_{(a, b)}(f)$). Nếu ta đồng nhất $T_{(a, b)}(X_1 \times X_2)$ với $T_a(X_1) \times T_b(X_2)$, ta có:

$$
T_{(a, b)}(f) \cdot (u, v) = T^1_{(a, b)}(f) \cdot u + T^2_{(a, b)}(f) \cdot v
$$

với mọi $u \in T_a(X_1)$ và mọi $v \in T_b(X_2)$.

5.6.7. (« Định lý về các hàm ẩn »). Với các giả thiết và ký hiệu của số trước, giả sử thêm rằng $T^2_{(a, b)}(f)$ là song ánh. Khi đó tồn tại một lân cận mở $U$ của $a$ trong $X_1$ và một lân cận mở $V$ của $b$ trong $X_2$ có tính chất sau: với mọi $x \in U$, tồn tại một và chỉ một điểm $g(x)$ của $V$ sao cho $f(x, g(x)) = f(a, b)$, và ánh xạ $g$ là một cấu xạ từ $U$ vào $V$. Với mọi $x \in U$, ta có:

$$
T_x(g) = - (T^2_{(x, g(x))}(f))^{-1} \circ T^1_{(x, g(x))}(f).
$$

### 5.7. Các phép nhúng, các cấu xạ étale

5.7.1. Cho $X$ và $Y$ là hai đa tạp, $f$ là một cấu xạ từ $X$ vào $Y$ và $a$ là một điểm của $X$. Đặt $b = f(a)$. Các điều kiện sau là tương đương:
(i) Ánh xạ tuyến tính $T_a(f)$ là đơn ánh và ảnh của nó là một không gian con vectơ đóng của $T_b(Y)$ thừa nhận một phần bù tôpô $^1$;

(ii) Tồn tại một không gian Banach $F$, một không gian con vectơ đóng $E$ của $F$ thừa nhận một phần bù tôpô, và các hệ tọa độ $(U, \varphi, E)$ của $X$ tại $a$ và $(V, \psi, F)$ của $Y$ tại $b$ sao cho $f(U) \subset V$ và $\varphi = \psi \circ (f|U)$.

(iii) Tồn tại một lân cận mở $U$ của $a$, một lân cận mở $V$ của $b$ chứa $f(U)$, một đa tạp $Z$, một điểm $c$ của $Z$, và một đẳng cấu của các đa tạp $g$ từ $U \times Z$ lên $V$ sao cho $f(x) = g(x, c)$ với mọi $x \in U$.

(iv) Tồn tại một lân cận mở $U$ của $a$, một lân cận mở $V$ của $b$ và một cấu xạ $q$ từ $V$ vào $X$ với $f(U) \subset V$, và $q(f(x)) = x$ với mọi $x \in U$.

Khi $X$ và $Y$ là hữu hạn chiều, các điều kiện trên cũng tương đương với điều kiện sau:

(v) Tồn tại một lân cận mở $U$ của $a$, một hệ tọa độ $(\eta^1, \ldots, \eta^n)$ của $Y$ trong một lân cận mở $V$ của $b$ chứa $f(U)$ và một số nguyên $m \leq n$ sao cho $\eta^j \circ f = 0$ với $m < j \leq n$ và các hàm $\eta^1 \circ f, \ldots, \eta^m \circ f$ tạo thành một hệ tọa độ của $X$ trong $U$.

Nếu các tính chất (i) đến (iv) được thỏa mãn, ta nói rằng $f$ là một phép nhúng tại $a$.

Tập hợp các điểm nơi $f$ là một phép nhúng là mở trong $X$; nếu tập mở này là toàn bộ $X$, ta nói rằng $f$ là một phép nhúng.

Để $f$ là một phép nhúng, điều kiện cần và đủ là $X$ có thể được phủ bởi các tập mở $U_i$ sao cho, với mọi $i, f|U_i$ là một đẳng cấu của $U_i$ lên một đa tạp con của $Y$ (xem No. 5.8.3).

5.7.2. Ví dụ:
(a) Nếu $X$ là một tập mở trong một đa tạp $Y$, đơn ánh chính tắc của $X$ vào $Y$ là một phép nhúng.
(b) Cho $E$ và $F$ là hai không gian Banach và cho $u$ là một ánh xạ tuyến tính liên tục của $E$ vào $F$. Khi đó $u$ là một phép nhúng khi và chỉ khi $u$ là một đẳng cấu của $E$ lên một không gian con vectơ đóng của $F$ thừa nhận một phần bù tôpô.

5.7.3. Cho $f : X \to Y$ và $g : Y \to Z$ là hai cấu xạ. Nếu $f$ và $g$ là các phép nhúng, $g \circ f$ là một phép nhúng. Ngược lại, nếu $g \circ f$ là một phép nhúng, thì $f$ là một phép nhúng. Nếu $f : X \to Y$ và $f' : X' \to Y'$ là các phép nhúng, $f \times f'$ là một phép nhúng.

5.7.4 Giả sử rằng $X$ và $Y$ là các đa tạp có số chiều hữu hạn trên một trường $K$ có đặc số 0. Nếu $f : X \to Y$ là một cấu xạ đơn ánh, tập hợp các điểm của $X$ nơi $f$ là một phép nhúng là một tập mở trù mật

$^1$ Mọi không gian con vectơ đóng có đối chiều hữu hạn của một không gian Banach đều thừa nhận một phần bù tôpô; nếu $K = \mathbf{R}$ hoặc $\mathbf{C}$, điều tương tự đúng với mọi không gian con vectơ hữu hạn chiều (nhất thiết đóng).

trong $X$. Nếu K = R hoặc C, kết quả này vẫn đúng nếu chỉ giả sử rằng X có số chiều hữu hạn.

5.7.5. Cho $f : X \to Y$ là một phép nhúng và cho $g$ là một ánh xạ liên tục của một đa tạp Z vào X. Để $g$ là một cấu xạ, điều kiện cần và đủ là $f \circ g$ là một cấu xạ.

5.7.6. Cho $f : X \to Y$ là một cấu xạ, và cho $a$ thuộc X. Hai tính chất sau là tương đương:
(i) $T_a(f)$ là song ánh.
(ii) Tồn tại một lân cận mở U của $a$ và một lân cận mở V của $f(a)$ sao cho $f$ cảm sinh một đẳng cấu của U lên V.
Khi các tính chất này được thỏa mãn, ta nói rằng $f$ là một đẳng cấu địa phương tại $a$, hoặc rằng $f$ là étale tại $a$. Nếu điều này đúng với mọi $a \in X$, ta nói rằng $f$ là étale, hoặc là một étalement, hoặc rằng X là étalé trong Y (bằng $f$). Để một cấu xạ là étale, điều kiện cần và đủ là nó vừa là một phép nhúng (No. 5.7.1) vừa là một phép dưới ngâm (No. 5.9.1.).

5.7.7. Cho $f : X \to Y$ là một phép nhúng; giả sử đa tạp X là thuần túy hữu hạn chiều. Khi đó $f$ là étale trong mỗi một trong hai trường hợp sau:
(i) $\dim Y = \dim X$;
(ii) $f$ là toàn ánh và tôpô của X có một cơ sở đếm được gồm các tập mở.

5.7.8. Để một cấu xạ $f$ là một đẳng cấu lên một đa tạp con mở (tương ứng, một đẳng cấu), điều kiện cần và đủ là $f$ là étale và đơn ánh (tương ứng, étale và song ánh).

### 5.8. Ảnh ngược của các cấu trúc đa tạp, các đa tạp con

5.8.1. Cho X là một không gian tôpô, Y là một đa tạp và $f$ là một ánh xạ từ X vào Y. Xét các điều kiện sau:
(QR) (tương ứng, (R)) Với mọi $a \in X$, tồn tại một lân cận mở U của a trong X và một biểu đồ $(V, \varphi, E)$ của đa tạp Y tại $f(a)$ sao cho $f(U) \subset V$ và $\varphi \circ f$ cảm sinh một đồng phôi của U lên giao của $\varphi(V)$ với một không gian con vectơ đóng (tương ứng, đóng và thừa nhận một phần bù tôpô) F của E.
Nếu điều kiện (QR) được thỏa mãn, tồn tại trên X một và chỉ một cấu trúc đa tạp sao cho các bộ ba $(U, \varphi \circ f, F)$ (với ký hiệu của (QR)) là các biểu đồ của X. Nó được gọi là cấu trúc ảnh ngược của cấu trúc đa tạp của Y bởi $f$. Tôpô của nó là tôpô của X.
Để tồn tại trên X một cấu trúc đa tạp tương thích với tôpô đã cho và sao cho $f$ là một phép nhúng, điều kiện cần và đủ là điều kiện (R) được thỏa mãn. Cấu trúc này khi đó là duy nhất: nó là ảnh ngược bởi $f$ của cấu trúc đa tạp của $Y$.

5.8.2. Điều kiện (R) ở trên đặc biệt được thỏa mãn khi, với mọi $a \in X$, tồn tại một lân cận mở $U$ của $a$ sao cho $f|U$ là một đồng phôi của $U$ lên một tập mở của $Y$. Trong trường hợp này, đa tạp $X$ thu được là étalé trên $Y$ (5.7.6).

5.8.3. Bây giờ giả sử rằng $X$ là một không gian con tôpô của $Y$, $f$ là đơn ánh chính tắc. Nếu $f$ thỏa mãn điều kiện (R) (tương ứng, (QR)) của No. 5.8.1, ta nói rằng X, được trang bị cấu trúc ảnh ngược của cấu trúc đa tạp của $Y$ bởi $f$, là một đa tạp con (tương ứng, đa tạp con tựa) của $Y$. Một đa tạp con là một đa tạp con tựa.

Mọi đa tạp con tựa đều đóng địa phương; mọi tập mở đều là một đa tạp con và cấu trúc của nó là cấu trúc được xác định trong No. 5.2.3.

của $Y$ (Ens., ch. IV, § 2, No. 4).

5.8.6. Nếu $X$ là một đa tạp con (tương ứng, đa tạp con tựa) của $Y$ và nếu $Y$ là một đa tạp con của một đa tạp $Z$, thì X là một đa tạp con (tương ứng, đa tạp con tựa) của $Z$.

5.8.7. Cho $X_i$ (với $i = 1, 2$) là một đa tạp và cho $Y_i$ là một đa tạp con (tương ứng đa tạp con giả) của $X_i$ (với $i = 1, 2$). Khi đó $Y_1 \times Y_2$ là một đa tạp con (tương ứng đa tạp con giả) của $X_1 \times X_2$.

5.8.8. Cho X là một đa tạp con giả của một đa tạp Y; cho x là một điểm của X, và ký hiệu f là đơn ánh chính tắc của X vào Y. Ánh xạ T_x(f) : T_x(X) → T_x(Y) là đơn ánh và cho phép ta đồng nhất không gian T_x(X) với một không gian con vectơ đóng của T_x(Y). Không gian vectơ tôpô thương T_x(Y)/T_x(X) là một không gian Banach, được gọi là không gian ngang của X (trong Y) tại x. Chiều của nó (hữu hạn hoặc +∞) được gọi là đối chiều của X trong Y tại điểm x.

Nếu hơn nữa X là một đa tạp con của Y, thì không gian T_x(X) thừa nhận một phần bù tôpô trong T_x(Y).

5.8.9. Cho f là một ánh xạ từ một đa tạp X vào một đa tạp Y, và cho Γ là đồ thị của nó. Để f là một cấu xạ, điều kiện cần và đủ là hai điều kiện sau được thỏa mãn:
(i) Γ là một đa tạp con của X × Y.
(ii) Với mọi (x, y) ∈ Γ, ta có
$$
T_{(x,y)}(X \times Y) = T_{(x,y)}(\Gamma) \oplus T_y(Y).
$$
Nếu điều này xảy ra, ánh xạ $\mathrm{pr}_1$ cảm sinh một đẳng cấu của $\Gamma$ lên X, và $T_{(x,y)}(\Gamma)$ được đồng nhất với đồ thị của $T_x(f)$.

Đặc biệt, đường chéo của X × X là một đa tạp con của X × X.

5.8.10. Cho Y là một đa tạp, và cho $(f_i)_{i∈I}$ là một họ hữu hạn các hàm cấu xạ trên Y. Cho X là tập hợp các x ∈ Y sao cho f_i(x) = 0 với mọi i. Đặt giả thiết sau:
(J) Với mọi x ∈ X, các vi phân d_x f_i là độc lập tuyến tính trong T'_x(Y).

Khi đó X là một đa tạp con đóng của Y, không gian tiếp xúc T'_x(X) là không gian con của T_x(Y) tạo bởi các α sao cho α . f_i = 0 với mọi i trong I. Hơn nữa, đối chiều của X trong Y bằng Card (I) tại mỗi điểm của nó.

5.8.11. (Các không của đơn giản của một iđêan). Cho a là một iđêan của đại số các đa thức K[X_1, ..., X_n]. Một điểm x = (x_1, ..., x_n) của K^n được gọi là một không của a nếu f(x) = 0 với mọi f ∈ a. Nếu x ∈ K^n, ký hiệu S_x là đại số con của K(X_1, ..., X_n) tạo bởi các phân thức f/g, với f, g ∈ K[X_1, ..., X_n], và g(x) ≠ 0; ký hiệu a_x là iđêan của S_x sinh bởi a trong S_x. Một điểm x được gọi là một không đơn của a nếu nó là một không của a và nếu điều kiện sau được thỏa mãn:
(S) Tồn tại một dãy hữu hạn (f_1, ..., f_m) các phần tử của a sinh iđêan a_x và có các vi phân tại x độc lập tuyến tính. (Điều kiện này tương đương với việc nói rằng vành địa phương S_x/a_x là chính quy (Alg. Comm., sắp xuất hiện).)
Cho Z (tương ứng Z_s) là tập hợp các không (tương ứng các không đơn) của a. Tập hợp Z là đóng trong K^n, Z_s là mở trong Z, và Z_s là một đa tạp con của $K^n$. Nếu $x \in Z_s$, iđêan $K[X_1, \ldots, X_n] \cap a_x$ gồm các đa thức $f$ triệt tiêu trong một lân cận của $x$ trong $Z_s$.

Cho $\bar{a}$ là iđêan các đa thức triệt tiêu trên $Z$. Nếu $K$ là đóng đại số, tập hợp các không đơn của a là trù mật trong Z.

5.8.12. Cho $X$ là một đa tạp và $L$ là tập hợp các cặp $(x, Z)$ trong đó x là một điểm của X và Z là một đa tạp con của X chứa x. Cho hai cặp $\pi = (x, Z)$ và $\pi' = (x', Z')$, ta ký hiệu bởi $R\{\pi, \pi'\}$ quan hệ:

« Nếu $x = x'$ và tồn tại một lân cận $U$ của $x$ sao cho $U \cap Z = U \cap Z'$ ». Khi đó R là một quan hệ tương đương trong L; ta ký hiệu bởi $\gamma_x(Z)$ lớp tương đương của cặp $(x, Z) \in L$. Trên tập hợp $J = L/R$, tồn tại duy nhất một cấu trúc đa tạp thỏa mãn điều kiện sau:
Với mọi đa tạp con Z của X, ánh xạ $x \mapsto \gamma_x(Z)$ từ Z vào J là một đẳng cấu của Z lên một đa tạp con mở của J.
Ta nói rằng J là đa tạp các mầm của các đa tạp con của X (xem Top. Gén., Chương I, ấn bản lần thứ 4, § 6, No. 10).
Ánh xạ $\rho : J \to X$ xác định bởi $\rho(\gamma_x(Z)) = x$ là một phép nhúng; ta gọi nó là phép nhúng chính tắc của J vào X.
Nếu $X$ là một đa tạp giải tích tách được có số chiều hữu hạn, điều tương tự cũng đúng với $J$.

### 5.9. Các phép dìm và các đa tạp thương

5.9.1. Cho $f : X \to Y$ là một cấu xạ của các đa tạp, cho $a$ là một điểm của $X$, và đặt $b = f(a)$. Các điều kiện sau là tương đương:
(i) Ánh xạ tuyến tính $T_a(f)$ là toàn ánh, và hạt nhân của nó có một phần bù tôpô trong $T_a(X)$.
(ii) Tồn tại một biểu đồ $(U, \varphi, E)$ của $X$ tại $a$, một biểu đồ $(V, \psi, F)$ của $Y$ tại $b$, và một ánh xạ tuyến tính liên tục toàn ánh $u$ của $E$ vào $F$ sao cho
$$
f(U) \subset V, \quad \psi \circ f = u \circ \varphi
$$
và sao cho hạt nhân của $u$ có một phần bù tôpô trong $E$.
(iii) Tồn tại một lân cận mở $U$ của $a$, một lân cận mở $V$ của $b$ chứa $f(U)$, và một cấu xạ $g$ của $U$ vào một đa tạp $Z$ sao cho ánh xạ $(f, g)$ của $U$ vào $V \times Z$ là một đẳng cấu.
(iv) Tồn tại một lân cận mở $V$ của $b$ và một cấu xạ $s$ của $V$ vào $X$ sao cho $s(b) = a$ và $f(s(y)) = y$ với mọi $y$ trong $V$ ("tiết diện địa phương").
Khi $X$ và $Y$ là hữu hạn chiều, các điều kiện trước đó tương đương với điều kiện sau:
(v) Tồn tại một lân cận mở $U$ của $a$, một lân cận mở $V$ của $b$ chứa $f(U)$, và một hệ tọa độ $(\eta^1, \ldots, \eta^n)$ trên $V$ sao cho các hàm $\eta^i \circ f$ trên $U$ tạo thành một phần của một hệ tọa độ trên $U$.
Nếu các tính chất (i) đến (iv) được thỏa mãn, ta nói rằng $f$ là một cấu xạ hạ chìm tại $a$. Tập hợp các điểm mà tại đó $f$ là một cấu xạ hạ chìm là mở trong $X$; nếu tập mở này là toàn bộ $X$, ta nói rằng $f$ là một cấu xạ hạ chìm.

5.9.2. Cho $f : X \to Y$ và $g : Y \to Z$ là hai cấu xạ. Nếu $f$ và $g$ là các phép chìm, thì $g \circ f$ cũng là một phép chìm; ngược lại, nếu $g \circ f$ là một phép chìm và $f$ là toàn ánh, thì $g$ là một phép chìm.

5.9.3. Nếu $f : X \to Y$ và $f' : X' \to Y'$ là các phép chìm, thì $f \times f'$ là một phép chìm.

5.9.4. Một phép chìm $f : X \to Y$ là một ánh xạ mở (xem Top. gén., ch. I, 4e éd., § 5, n° 1); đặc biệt, quan hệ tương đương R được xác định bởi $f$ là mở, $f$ xác định qua chuyển qua thương một phép đồng phôi của $X/R$ lên $f(X)$, và $f(X)$ là mở trong $Y$.

5.9.5. Cho $R$ là một quan hệ tương đương trên một đa tạp $X$. Ta nói rằng $R$ là chính quy nếu tồn tại trên không gian thương $X/R$ một cấu trúc của một đa tạp sao cho phép chiếu chính tắc $p : X \to X/R$ là một phép chìm; cấu trúc của đa tạp này khi đó là duy nhất; nó là cấu trúc thương của cấu trúc trên $X$ (Ens., ch. IV, § 2, n° 6): nói cách khác, để một ánh xạ $g$ của $X/R$ vào một đa tạp $Y$ là một cấu xạ, điều kiện cần và đủ là $g \circ p$ là một cấu xạ của $X$ vào $Y$.

Cho $C \subset X \times X$ là đồ thị của $R$. Để $R$ là chính quy, điều kiện cần và đủ là hai điều kiện sau được thỏa mãn:
(i) $C$ là một đa tạp con của $X \times X$.
(ii) Ánh xạ $\mathrm{pr}_1$ của $C$ vào $X$ là một phép chìm.

Điều kiện (ii) cũng có nghĩa là nếu $a$ và $b$ là đồng dư modulo $R$, thì tồn tại một lân cận mở $U$ của $a$ và một cấu xạ $s$ của $U$ vào $X$ sao cho $s(a) = b$ và sao cho $s(x)$ đồng dư với $x$ modulo $R$ với mọi $x \in U$.

Giả sử rằng $R$ là chính quy. Để đa tạp thương $X/R$ là tách được, điều kiện cần và đủ là đồ thị của $R$ đóng trong $X \times X$.

5.9.6. Cho $X$ và $X'$ là hai đa tạp, $R$ và $R'$ là các quan hệ tương đương chính quy trên $X$ và $X'$, và cho $f : X \to X'$ là một cấu xạ tương thích với các quan hệ $R$ và $R'$. Ánh xạ $\tilde{f} : X/R \to X'/R'$ suy ra từ $f$ bằng cách chuyển qua các thương khi đó là một cấu xạ.

5.9.7. (« Tính bắc cầu của các thương ») Cho $R$ và $S$ là hai quan hệ tương đương trên một đa tạp $X$ sao cho $R$ kéo theo $S$, và cho $S/R$ là quan hệ tương đương thương trên $X/R$. Giả sử rằng $R$ là chính quy. Khi đó, để $S$ là chính quy, điều kiện cần và đủ là $S/R$ cũng chính quy; nếu trường hợp này xảy ra, song ánh chính tắc

$$
(X/R)/(S/R) \to X/S
$$

là một đẳng cấu của các đa tạp.

5.9.8. (« Các tích của các thương ») Cho $(X_i)_{i \in I}$ là một họ hữu hạn các đa tạp, mỗi đa tạp được trang bị một quan hệ tương đương chính quy $R_i$. Cho $X = \prod_{i \in I} X_i$, và cho $R$ là quan hệ tương đương trên $X$ là tích của các $R_i$ (cf. Top. Gén., chap. I, 4e éd., § 5, n° 3, cor. de la prop. 8). Khi đó $R$ là chính quy, và song ánh chính tắc của $X/R$ lên $\prod_{i \in I} (X_i/R_i)$ là một đẳng cấu của các đa tạp.

### 5.10. Các nhúng con

5.10.1. Cho $f : X \to Y$ là một cấu xạ của các đa tạp và cho $\Gamma$ là đồ thị của $f$. Ánh xạ $j : x \mapsto (x, f(x))$ là một phép nhúng của $X$ vào $X \times Y$, có ảnh là đa tạp con $\Gamma$, và $f = \mathrm{pr}_2 \circ j$ là hợp thành của phép nhúng $j$ theo sau bởi phép dìm $\mathrm{pr}_2$.

Cho $a \in X$. Ta nói rằng $f$ là một phép dìm con tại $a$ nếu tồn tại một lân cận mở $U$ của $a$, một đa tạp $Z$, một phép dìm $s$ của $U$ vào $Z$ và một phép nhúng $i$ của $Z$ vào $Y$ sao cho $f|U = i \circ s$. Tập hợp các điểm của $X$ tại đó $f$ là một phép dìm con là một tập hợp mở của $X$; nếu tập hợp mở này là toàn bộ $X$, ta nói rằng $f$ là một phép dìm con.

5.10.2. Các phép nhúng và các phép dưới chìm là các phép dưới chìm. Nếu $f : X \to Y$ là một phép dưới chìm, $g : Y \to Z$ là một phép nhúng và $h : W \to X$ là một phép dưới chìm, thì $g \circ f \circ h$ là một phép dưới chìm.

Nếu $f$ và $f'$ là các phép dưới chìm, thì $f \times f'$ là một phép dưới chìm.

5.10.3. Để $f : X \to Y$ là một phép dưới chìm tại một điểm $a$ của $X$, điều kiện cần và đủ là tồn tại một biểu đồ $(U, \varphi, E)$ của $X$ tại $a$, một biểu đồ $(V, \psi, F)$ của $Y$ tại điểm $f(a)$ và một ánh xạ tuyến tính liên tục $g$ từ $E$ vào $F$ sao cho:
(i) $f(U) \subset V,\ g(\varphi(U)) \subset \psi(V)$ và $f|U = \psi^{-1} \circ g \circ \varphi$;
(ii) hạt nhân (tương ứng, ảnh) của $g$ là một không gian con đóng của $E$ (tương ứng $F$) có một phần bù tôpô.

5.10.4. Cho $X$ và $Y$ là hai đa tạp hữu hạn chiều. Để một cấu xạ $f$ từ $X$ vào $Y$ là một phép dưới chìm tại một điểm $a$ của $X$, điều kiện cần và đủ là tồn tại một hệ tọa độ $(\xi^1, \ldots, \xi^m)$ của $X$ tại $a$, một hệ tọa độ $(\eta^1, \ldots, \eta^n)$ của $Y$ tại $f(a)$ và một số nguyên $k \leq \inf(m, n)$ sao cho
$$
\eta^i \circ f = \xi^i \quad \text{cho } 1 \leq i \leq k \\
\eta^i \circ f = 0 \quad \text{cho } k < i \leq n.
$$

5.10.5. Cho $f : X \to Y$ là một phép dưới chìm. Với mọi $b \in Y$, $f^{-1}(b)$ là một đa tạp con của $X$; không gian con của $T_a(X)$ tiếp xúc với đa tạp con $f^{-1}(b)$ tại điểm $a \in f^{-1}(b)$ là hạt nhân của $T_a(f)$.

5.10.6. (“Định lý hạng hằng”) Cho $f : X \to Y$ là một cấu xạ của các đa tạp và cho $a \in X$. Nếu $f$ là một phép dưới nhúng tại $a$, thì $\mathrm{rg}_x f = \mathrm{rg}_a f$ với $x$ trong một lân cận của $a$.

Ngược lại, giả sử trường $K$ có đặc số không. Cho $(U, \varphi, E)$ là một bản đồ của $X$ tại $a$ và cho $(V, \psi, F)$ là một bản đồ của $Y$ tại $f(a)$, với $f(U) \subset V$. Đặt $g = \psi \circ f \circ \varphi^{-1}$. Nếu tồn tại một không gian con vectơ đóng $E_1$ của $E$ và một không gian con vectơ đóng $F_1$ của $F$ sao cho với mọi $x \in U$, không gian con $E_1$ (tương ứng $F_1$) là một phần bù tôpô của hạt nhân (tương ứng của ảnh) của đạo hàm $Dg(\varphi(x))$ của $g$ tại điểm $\varphi(x)$, thì $f$ là một phép chìm con tại $a$.

Nếu $K$ có đặc số không (tương ứng $K = \mathbf{R}$ hoặc $\mathbf{C}$) và nếu $Y$ có chiều hữu hạn (tương ứng $\mathrm{rg}_a f < +\infty$), thì $f$ là một phép chìm con tại $a$ khi và chỉ khi $\mathrm{rg}_x f = \mathrm{rg}_a f$ với mọi $x$ đủ gần $a$.

Nếu $K$ có đặc số không (tương ứng $K = \mathbf{R}$ hoặc $\mathbf{C}$) và $Y$ (tương ứng $X$) có chiều hữu hạn, tập hợp các điểm $x \in X$ tại đó $f$ là một phép chìm con là một tập hợp mở trù mật trong $X$.

5.10.7. ("Phân tích chính tắc của một ánh xạ hạ chìm") Mọi ánh xạ hạ chìm đều là hợp thành của một ánh xạ chìm và một phép nhúng. Chính xác hơn, cho $f : X \to Y$ là một ánh xạ hạ chìm, và cho $J$ là đa tạp các mầm của các đa tạp con của $Y$ (5.8.12). Cho $x$ thuộc $X$ và $y = f(x)$; tồn tại các lân cận mở $U$ của $x$ sao cho $f|U$ là một ánh xạ chìm của $U$ lên một đa tạp con $Z$ của $Y$; phần tử $\gamma_y(Z)$ của $J$ chỉ phụ thuộc vào $x$ chứ không phụ thuộc vào lân cận $U$ được chọn, và, nếu ký hiệu nó là $\lambda(x)$, thì ánh xạ $\lambda$ là một ánh xạ chìm của $X$ vào $J$; nếu $\rho$ ký hiệu phép nhúng chính tắc của $J$ vào $Y$, ta có $f = \rho \circ \lambda$. Nếu $f$ là một phép nhúng, thì cấu xạ $\lambda$ của $X$ vào $J$ là étale.

Nếu $g$ là một ánh xạ chìm toàn ánh của $X$ lên một đa tạp $Z$ và $h$ là một cấu xạ của $Z$ vào $Y$ sao cho $f = h \circ g$, thì tồn tại một ánh xạ chìm duy nhất $\mu$ của $Z$ vào $J$ sao cho $\lambda = \mu \circ g$.

### 5.11. Tích sợi và ảnh ngược

5.11.1. Cho $F$ là một không gian Banach, $(E_i)_{i \in I}$ là một họ hữu hạn các không gian Banach, và $f = (f_i)_{i \in I}$ là một họ các ánh xạ tuyến tính liên tục $f_i$ của $E_i$ vào $F$. Cho $E$ là tích của các $E_i$ và $f$ là ánh xạ tuyến tính liên tục của $E$ vào $F^I$ là tích của các $f_i$. Cuối cùng, cho $D$ là không gian con đóng của $F^I$ gồm các $(y_i)_{i \in I}$ sao cho $y_i$ độc lập với $i$ (“đường chéo” của $F^I$). Ta nói rằng họ $f$ là xuyên ngang nếu ánh xạ tuyến tính liên tục thu được bằng cách hợp thành $f$ với phép chiếu chính tắc của $F^I$ lên không gian thương $F^I/D$ là toàn ánh và nếu hạt nhân của nó $f^{-1}(D)$ thừa nhận một phần bù tôpô.

Nếu các không gian $E_i$ và $F$ đều hữu hạn chiều, họ $f$ là xuyên ngang khi và chỉ khi ta có:

$$
\operatorname{codim} \left( \bigcap_i \operatorname{Im} f_i \right) = \sum_i \operatorname{codim} (\operatorname{Im} f_i)
$$

Nếu $I = \{1, 2\}$, cặp $(f_1, f_2)$ là xuyên ngang khi và chỉ khi ánh xạ

$$
f_1 + f_2 : E_1 \oplus E_2 \to F
$$

là toàn ánh và nếu hạt nhân của nó thừa nhận một phần bù tôpô (nếu $E_1$ và $E_2$ hữu hạn chiều, điều này tương đương với việc nói rằng

$$
\operatorname{Im} f_1 + \operatorname{Im} f_2 = F).
$$

5.11.2. Cho $S$ là một đa tạp, $(X_i)_{i \in I}$ là một họ hữu hạn các đa tạp, và $f = (f_i)_{i \in I}$ là một họ các cấu xạ $f_i$ của $X_i$ vào $S$. Cho $P$ là tập con của tích $X$ của các $X_i$ gồm các điểm $(x_i)_{i \in I}$ sao cho $f_i(x_i)$ độc lập với $i$. Cho $x \in P$ và cho $y = f_i(x_i) \in F$. Ta nói rằng họ $f$ là *xuyên ngang* tại điểm $x$ của $P$ nếu các ánh xạ $T_x(f_i)$ tạo thành một họ xuyên ngang các ánh xạ tuyến tính liên tục có giá trị trong không gian Banach $T_y(S)$. Ta nói rằng $f$ là *xuyên ngang* nếu nó xuyên ngang tại mọi điểm của $P$.

Nếu $f$ là xuyên giao, thì $P$ là một *đa tạp con* của $X$, được gọi là *tích sợi của họ của các $X_i$ trên $S$* (đối với họ $f$), và được ký hiệu bởi $\prod_{i \in I} X_i$ (hoặc đơn giản hơn là $X_1 \times_S X_2$ khi $I = \{1, 2\}$, chẳng hạn). Với mọi điểm $x = (x_i)$ của $P$, không gian tiếp xúc $T_x(\prod_{i \in I} X_i)$ là không gian con của $\prod T_{x_i}(X_i)$ tạo bởi các vectơ tiếp xúc $t = (t_i)$ sao cho $T_{x_i}(f_i) \cdot t_i$ là độc lập với chỉ số $i$.

Nếu $f_1 : X_1 \to Y$ là một *hàm chìm* và $f_2 : X_2 \to Y$ là một cấu xạ, thì cặp $(f_1, f_2)$ là xuyên giao.

5.11.3. (*Tính chất phổ quát của các tích sợi*) Cho $f = (f_i)_{i \in I}$ là một họ xuyên giao các cấu xạ $f_i : X_i \to S$, và cho $P$ là tích sợi của các $X_i$ trên $S$; với mọi $i \in I$, ký hiệu $\pi_i$ là cấu xạ từ $P$ vào $X_i$ thu được bằng hạn chế xuống $P$ của phép chiếu của $X$ lên $X_i$; khi đó $f_i \circ \pi_i$ là một cấu xạ từ $P$ vào $S$ độc lập với $i$. Cho $T$ là một đa tạp, và cho $g_i : T \to X_i$ là các cấu xạ của các đa tạp sao cho $f_i \circ g_i$ là một cấu xạ từ $T$ vào $S$ độc lập với $i \in I$; khi đó tồn tại một và chỉ một cấu xạ $h$ từ $T$ vào $P$ sao cho $g_i = \pi_i \circ h$ với mọi $i \in I$.

5.11.4. (*Tính kết hợp của tích sợi*) Cho $f = (f_i)_{i \in I}$ là một họ hữu hạn các cấu xạ của các đa tạp $f_i : X_i \to S$, và cho $(J_\lambda)_{\lambda \in \Lambda}$ là một phân hoạch của $I$. Giả sử rằng, với mọi $\lambda$ trong $\Lambda$, họ $f_\lambda = (f_i)_{i \in J_\lambda}$ là xuyên giao, và ký hiệu $P_\lambda$ là tích sợi của họ này; với mọi điểm $x = (x_i)_{i \in J_\lambda}$ của $P_\lambda$, phần tử $f_i(x_i)$ của $S$ là độc lập với $i \in J_\lambda$ và sẽ được ký hiệu bởi $u_\lambda(x)$;

khi đó $u_\lambda$ là một cấu xạ từ $P_\lambda$ vào $S$. Để họ $u = (u_\lambda)$ là ngang, điều kiện cần và đủ là họ $f$ cũng như vậy. Song ánh chính tắc của $\prod_{\lambda \in \Lambda} \prod_{i \in J_\lambda} X_i$ lên $\prod_{i \in I} X_i$ khi đó cho bởi hạn chế một đẳng cấu của tích sợi $\prod_{\lambda \in \Lambda} \prod_{s} P_\lambda$ lên tích sợi $\prod_{i \in I} \prod_{s} X_i$.

5.11.5. Cho $S$ là một đa tạp. Một *đa tạp trên* $S$ là một đa tạp $X$ được trang bị một cấu xạ $\lambda : X \to S$. Cho $(X, \lambda)$ là một đa tạp trên $S$ và cho $f : S' \to S$ là một cấu xạ của các đa tạp sao cho cặp $(f, \lambda)$ là ngang. Khi đó ta ký hiệu $f^*(X)$ là đa tạp $S' \times_S X$, được trang bị cấu xạ $f^*(\lambda) : S' \times_S X$ xác định bởi $f^*(\lambda)(s', x) = s'$. Ta nói rằng $f^*(X)$ được suy ra từ $X$ bằng thay đổi cơ sở từ $S$ đến $S'$ theo $f$. Nếu $\lambda$ là một cấu xạ ngập chìm (tương ứng là một cấu xạ nhúng, một cấu xạ dưới-nhúng, một cấu xạ étale), thì điều tương tự cũng đúng với $f^*(\lambda)$.

5.11.6. Cho $f : X \to Y$ là một cấu xạ của các đa tạp và cho $W$ là một đa tạp con của $Y$; cho $i$ là đơn ánh chính tắc của $W$ vào $Y$. Ta nói rằng $f$ là *xuyên ngang với* $W$ *tại một điểm* $x \in f^{-1}(W)$ nếu cặp $(f, i)$ là xuyên ngang tại điểm $(x, f(x))$ của $X \times W$. Để có điều này, điều kiện cần và đủ là các điều kiện sau được thỏa mãn:
(i) không gian tiếp xúc $T_{f(x)}(Y)$ là tổng của $T_{f(x)}(W)$ và ảnh của $T_x(f)$;
(ii) ảnh ngược $T_x(f)^{-1}(T_{f(x)}(W))$ của không gian tiếp xúc với $W$ tại $f(x)$ thừa nhận một phần bù tôpô.
Ta nói rằng $f$ là *xuyên ngang với* $W$ nếu nó xuyên ngang với $W$ tại mọi điểm của $f^{-1}(W)$.
Để một cấu xạ $f$ của $X$ vào $Y$ là một cấu xạ phân chìm, điều kiện đủ là nó xuyên ngang với mọi điểm của $Y$, và điều kiện cần là nó xuyên ngang với mọi đa tạp con của $Y$. Để một họ hữu hạn các cấu xạ $f_i : X_i \to S$ là xuyên ngang, điều kiện cần và đủ là cấu xạ $g$ của $\prod_{i \in I} X_i$ vào $S^I$ được xác định bởi $g((x_i)_{i \in I}) = (f_i(x_i))_{i \in I}$ là xuyên ngang với đường chéo của $S^I$.

5.11.7. Giả sử rằng cấu xạ $f : X \to Y$ là xuyên ngang với đa tạp con $W$ của $Y$. Khi đó $f^{-1}(W)$ là một đa tạp con của $X$, và đối với $x$ trong $f^{-1}(W)$ không gian con của $T_x(X)$ tiếp xúc với $f^{-1}(W)$ là ảnh ngược qua $T_x(f)$ của không gian con $T_{f(x)}(W)$. Qua việc chuyển qua thương, ánh xạ tuyến tính $T_x(f)$ xác định một đẳng cấu của các không gian vectơ tôpô từ không gian xuyên ngang với $f^{-1}(W)$ tại $x$ lên không gian xuyên ngang với $W$ tại $y = f(x)$. Nếu $W$ có đối chiều $d$ tại $y$ trong $Y$, đa tạp con $f^{-1}(W)$ của $X$ có đối chiều $d$ tại mọi điểm của $f^{-1}(W)$. Cuối cùng, ánh xạ $x \mapsto (x, f(x))$ là một đẳng cấu của các đa tạp của $f^{-1}(W)$ lên tích sợi $X \times_Y W$.

5.11.8. Cho $Y_1$ và $Y_2$ là hai đa tạp con của một đa tạp $X$, và cho $\iota_j$ là đơn ánh của $Y_j$ vào $X$. Ta nói rằng $Y_1$ và $Y_2$ là ngang nếu cặp $(\iota_1, \iota_2)$ là ngang; tương đương, chỉ cần giả sử rằng, với mọi điểm $x$ của $Y_1 \cap Y_2$, các không gian con $T_x(Y_1)$ và $T_x(Y_2)$ của $T_x(X)$ có $T_x(X)$ là tổng của chúng, và giao của chúng có một phần bù tôpô trong $T_x(X)$. Dưới các điều kiện này, $Y_1 \cap Y_2$ là một đa tạp con của $X$ và với mọi $x$ trong $Y_1 \cap Y_2$, ta có:

$$
T_x(Y_1 \cap Y_2) = T_x(Y_1) \cap T_x(Y_2);
$$

hơn nữa, nếu $Y_i$ có đối chiều $d_i$ tại $x$, thì $Y_1 \cap Y_2$ có đối chiều $d_1 + d_2$ tại $x$.

5.11.9. Cho $f$ và $g$ là hai cấu xạ của một đa tạp $X$ vào một đa tạp $Y$. Nếu cấu xạ $(f, g) : X \to Y \times Y$ là ngang với đường chéo của $Y \times Y$, tập con $N$ của $X$ tạo bởi các điểm $x$ sao cho $f(x) = g(x)$ là một đa tạp con của $X$; ta gọi nó là *hạt nhân* của mũi tên kép

$$
f, g : X \twoheadrightarrow Y.
$$

### 5.12. Các đa tạp nhóm

5.12.1. Cho $G$ là một nhóm. Một cấu trúc đa tạp trên $G$ được gọi là *tương thích* với cấu trúc nhóm của $G$ nếu ánh xạ $(x, y) \mapsto xy$ của $G \times G$ vào $G$ là một cấu xạ. Khi đó ánh xạ $x \mapsto x^{-1}$ là một cấu xạ của $G$ vào chính nó. Tập hợp $G$, được trang bị cấu trúc nhóm và cấu trúc đa tạp của nó, được gọi là một *đa tạp nhóm* (« thuộc lớp $C^r$ » nếu muốn chính xác), hoặc còn gọi là một *nhóm Lie*. Nếu $r = \omega$, nó còn được gọi là một *nhóm giải tích*. Nếu $K = \mathbf{R}$ (tương ứng. $\mathbf{C}, \mathbf{Q}_p$), nó còn được gọi là một *nhóm Lie thực* (tương ứng. *phức*, *p-adic*). Mọi đa tạp nhóm đều là thuần túy. Ta gọi *đồng cấu của các đa tạp nhóm* (hoặc đơn giản là *đồng cấu*) mọi ánh xạ từ một đa tạp nhóm vào một đa tạp nhóm khác vừa là một đồng cấu nhóm vừa là một *cấu xạ* của các đa tạp.

Nếu $G$ là một đa tạp nhóm, cấu trúc tôpô nền tảng của cấu trúc đa tạp của $G$ làm cho nó trở thành một *nhóm tôpô mêtric và đầy đủ*; nó là compact địa phương nếu $K$ là compact địa phương và $G$ hữu hạn chiều.

5.12.2. *Ví dụ* :
(i) Nếu $V$ là một không gian Banach, cấu trúc đa tạp chính tắc của $V$ tương thích với cấu trúc nhóm giao hoán của nó.
(ii) Cho $A$ là một $K$-đại số định chuẩn đầy đủ, có một phần tử đơn vị, và cho $A^*$ là nhóm các phần tử khả nghịch của $A$. Đây là một không gian con mở của $A$ và cấu trúc đa tạp cảm sinh trên tập mở này bởi cấu trúc đa tạp chính tắc của không gian vectơ $K$ $A$ tương thích với cấu trúc nhóm trong $A^*$. Đặc biệt, lấy $A$ là đại số

L(E) của các đồng cấu liên tục của một không gian Banach E; nhóm $A^*$ gồm các tự đẳng cấu của không gian vectơ tôpô E; ta ký hiệu bởi $\mathrm{GL}(E)$ đa tạp nhóm thu được như vậy. Khi $A = M_n(K)$, ta thu được một cấu trúc đa tạp nhóm trên $\mathrm{GL}(n, K)$.

(iii) Nếu $G_1, \ldots, G_n$ là các đa tạp nhóm, nhóm tích $G = G_1 \times \cdots \times G_n$ là một đa tạp nhóm, khi nó được trang bị cấu trúc đa tạp tích của các cấu trúc của các $G_i$.

5.12.3. Cho $G$ là một đa tạp nhóm, cho $H$ là một nhóm tôpô và cho $f : H \to G$ là một đồng cấu liên tục thỏa mãn điều kiện (QR) của No. 5.8.1. Cấu trúc đa tạp ảnh ngược của cấu trúc của $G$ bởi $f$ khi đó làm cho $H$ trở thành một đa tạp nhóm. Điều này đặc biệt áp dụng khi $H$ là một *nhóm con của $G$ là một đa tạp con* (resp. đa tạp con gần); một nhóm con như vậy được gọi là một *đa tạp con* (resp. đa tạp con gần) *của nhóm* $G$; nó nhất thiết *đóng* trong $G$.

Nếu $H_i (i = 1, \ldots, n)$ là một đa tạp con của nhóm $G_i$, thì $H_1 \times \cdots \times H_n$ là một đa tạp con của nhóm $G_1 \times \cdots \times G_n$.

5.12.4. Cho $G$ là một đa tạp nhóm và cho $H$ là một đa tạp con của nhóm $G$. Quan hệ tương đương $x^{-1} y \in H$ là chính quy, điều này làm cho có thể trang bị cho không gian $G/H$ của các lớp kề trái $xH$ một cấu trúc đa tạp được gọi là *thương* của cấu trúc của $G$. Ánh xạ chính tắc $(g, x) \mapsto g \cdot x$ của $G \times (G/H)$ vào $G/H$ là một cấu xạ. Có các kết quả tương tự cho không gian thuần nhất $H\backslash G$ của các lớp kề phải $Hx$. Nếu $H$ là chuẩn tắc, cấu trúc đa tạp của $G/H$ tương thích với cấu trúc nhóm của nó.

5.12.5. Cho $G$ là một đa tạp nhóm và cho $X$ là một đa tạp. Một *luật tác động trái của nhóm $G$ trên đa tạp $X$* là bất kỳ cấu xạ nào $(s, x) \mapsto sx$ của $G \times X$ vào $X$ sao cho

$$
s(tx) = (st)x \quad \text{nếu} \quad s, t \in G, x \in X \\
ex = x \quad \text{nếu} \quad x \in X \ (\text{$ e $ là phần tử đơn vị của } G).
$$

Đa tạp nhóm $G$ cũng được nói là *tác động bên trái* trên $X$; các luật tác động phải được định nghĩa tương tự.

Cho $x \in X$ và cho $G_x$ là nhóm ổn định của nó trong $G$. Giả sử rằng ánh xạ $g \mapsto g \cdot x$ là một *hạ chìm* (một giả thiết tự động được thỏa mãn nếu đặc số của $K$ là 0 và $X$ là hữu hạn chiều). Khi đó $G_x$ là một đa tạp con nhóm con của $G$ và ánh xạ của $G/G_x$ vào $X$ nhận được bằng cách chuyển qua thương từ $g \mapsto g \cdot x$ là một phép nhúng. Hơn nữa, nếu quỹ đạo $G \cdot x$ của $x$ là đóng địa phương và nếu tôpô của $G$ có một cơ sở đếm được, thì $G \cdot x$ là một đa tạp con của $X$ và ánh xạ $G/G_x \to G \cdot x$ là một đẳng cấu của các đa tạp.

### 5.13. Làm yếu cấu trúc

Trong suốt No. này, các chữ $r, s, r', s'$ ký hiệu hoặc các số nguyên $\geqslant 1$, hoặc một trong các ký hiệu $\infty$ và $\omega$. Ta giả thiết rằng $K = \mathbf{R}$.

5.13.1. Cho $r \leqslant s$, và cho $X$ là một đa tạp thuộc lớp $C^s$. Trên không gian tôpô $X$ tồn tại một cấu trúc của một đa tạp thuộc lớp $C^r$ và chỉ một cấu trúc như vậy sao cho mọi biểu đồ của $X$ đối với cấu trúc đã cho cũng là một biểu đồ của $X$ đối với cấu trúc mới này. Gọi $X_r$ là đa tạp thuộc lớp $C^r$ được xác định như vậy. Ta nói rằng nó nhận được từ $X$ bằng cách làm yếu cấu trúc đa tạp của $X$, hoặc cũng nói rằng cấu trúc đa tạp của nó nằm dưới cấu trúc của $X$. Khái niệm làm yếu là bắc cầu: nếu $r' \leqslant r$, ta có $X_{r'} = (X_r)_{r'}$; nó giao hoán với các tích: nếu $Y$ thuộc lớp $C^s$, ta có $(X \times Y)_r = X_r \times Y_r$; có một kết quả tương tự đối với $X \times_s Y$ dưới các giả thiết của No. 5.11.2.

Cho $a \in X$ và cho $c$ là một biểu đồ của $X$ tại $a$; nó cũng là một biểu đồ của $X_r$ tại $a$. Từ (5.5.1) ta suy ra các đẳng cấu

$$
\theta_c : E \to T_a(X), \quad \theta'_c : E \to T_a(X_r),
$$

do đó có một đẳng cấu $\theta'_c \circ \theta_c^{-1} : T_a(X) \to T_a(X_r)$. Đẳng cấu này độc lập với lựa chọn $c$; nó cho phép ta đồng nhất các không gian tiếp xúc với $X$ và với $X_r$ tại $a$.

5.13.2. Cho $X$ (tương ứng $X'$) là một đa tạp thuộc lớp $C^s$ (tương ứng $C^{s'}$), và cho $r$ là số sao cho $r \leqslant \inf(s, s')$. Một ánh xạ $f : X \to X'$ được gọi là thuộc lớp $C^r$ nếu nó là một cấu xạ từ $X_r$ vào $X'_r$; một ánh xạ như vậy thuộc lớp $C^{r'}$ với mọi $r' \leqslant r$. Hơn nữa, ánh xạ tuyến tính tiếp xúc của $f : X_r \to X'_r$ tại một điểm $a \in X$ trùng với ánh xạ tuyến tính tiếp xúc của $f$ được xét như một cấu xạ từ $X_r$ vào $X'_r$.

Thông thường nhất, cùng một ký hiệu sẽ được dùng để chỉ các đa tạp $X$ và $X_r$; do đó, nếu $X$ thuộc lớp $C^s$, biểu thức "một đa tạp con của $X$ thuộc lớp $C^r$" ($r \leqslant s$) có nghĩa là "một đa tạp con của $X_r$".

### 5.14. Hạn chế trường cơ sở

Trong số này, cho hai trường giao hoán đầy đủ không rời rạc có giá trị $K$ và $L$, cùng với một đẳng cấu $\sigma$ của trường có giá trị $K$ lên một trường con của $L$. Nếu $E$ là một không gian Banach trên $L$, $\sigma_*(E)$ ký hiệu không gian vectơ trên $K$ thu được bằng hạn chế vô hướng (xem Alg., chap. II, ấn bản thứ 3, § 8); tôpô cho trên $E$ tương thích với cấu trúc của không gian vectơ trên $K$, và $\sigma_*(E)$ là một không gian Banach trên $K$.

5.14.1. Cho $X$ là một đa tạp giải tích trên $L$ và cho $c = (U, \varphi, E)$ là một bản đồ của $X$. Ánh xạ $\varphi$ là một song ánh của $U$ lên một tập con mở của $\sigma_*(E)$ và bộ ba $c_\sigma = (U, \varphi, \sigma_*(E))$ là một bản đồ của $X$. Trên $X$ tồn tại một và chỉ một cấu trúc đa tạp giải tích trên $K$ sao cho $c_\sigma$ là một bản đồ đối với mọi bản đồ $c$ của đa tạp giải tích trên $L$ $X$. Đa tạp giải tích trên $K$ thu được như vậy được ký hiệu là $X_\sigma$, và ta nói rằng $X_\sigma$ thu được từ $X$ bằng hạn chế vô hướng (từ $L$ đến $K$ nhờ $\sigma$). Không gian tôpô nền của $X_\sigma$ là cùng một không gian với không gian tôpô nền của $X$.

5.14.2. Ví dụ:
(a) Lấy $K = \mathbf{R},\ L = \mathbf{C},\ \sigma$ là đơn ánh chính tắc của R vào C. Do đó mọi đa tạp giải tích phức đều được trang bị một cách chính tắc một cấu trúc của đa tạp giải tích thực; bản thân cấu trúc giải tích thực này định nghĩa các cấu trúc vi phân lớp $C^r$ với mọi r.
(b) Lấy $K = \mathbf{C},\ L = \mathbf{C},\ \sigma$ là phép liên hợp $x \mapsto \bar{x}$. Do đó với mỗi đa tạp giải tích phức X ta liên kết một đa tạp giải tích phức $\overline{X}$, gọi là đa tạp liên hợp của X. Nếu $f$ là một hàm nhận giá trị phức, được định nghĩa trên một tập mở U của X, thì $f$ là giải tích đối với cấu trúc của $\overline{X}$ khi và chỉ khi hàm liên hợp $\bar{f}$ là giải tích đối với cấu trúc của X. Các đa tạp X và $\overline{X}$ định nghĩa, bằng hạn chế vô hướng, cùng một đa tạp giải tích thực.

5.14.3. Cho X là một đa tạp giải tích trên K, và Y là một đa tạp giải tích trên L. Một ánh xạ $f : X \to Y$ được gọi là $\sigma$-giải tích nếu nó là một cấu xạ từ X vào $Y_\sigma$. Nếu $K \subset L,\ \sigma$ là đơn ánh của K vào L, và X là một đa tạp giải tích trên L, một ánh xạ K-giải tích được gọi là một ánh xạ $\sigma$-giải tích của $X_\sigma$ vào Y.

5.14.4. Cho V là một không gian Banach-L. Ta có $V_\sigma = \sigma_*(V)$: cấu trúc chính tắc của một đa tạp giải tích trên K trên $\sigma_*(V)$ thu được bằng hạn chế vô hướng từ cấu trúc chính tắc của một đa tạp giải tích trên L trên V.

5.14.5. Cho X là một đa tạp giải tích trên L, và cho $a \in X$. Gọi c là một biểu đồ của X tại a; khi đó $c_\sigma$ là một biểu đồ của $X_\sigma$ tại a và ta suy ra từ đó các đẳng cấu
$$
\theta_c : E \to T_a(X), \quad \theta_{c_\sigma} : \sigma_*(E) \to T_a(X_\sigma)
$$
do đó một đẳng cấu $\theta_{c_\sigma} \circ \sigma_*(\theta_c)^{-1}$ của $\sigma_*(T_a(X))$ lên $T_a(X_\sigma)$; đẳng cấu này không phụ thuộc vào lựa chọn c; nó cho phép ta đồng nhất $T_a(X_\sigma)$ với $\sigma_*(T_a(X))$ và thậm chí với $T_a(X)$ bằng sự lạm dụng ký hiệu.
Nếu $f$ là một ánh xạ giải tích trên L từ X vào một đa tạp Y, ánh xạ tuyến tính tiếp xúc của $f$ tại a ($f$ được xem như một cấu xạ của $X_\sigma$ vào $Y_\sigma$) bằng $\sigma_*(T_a(f))$.

5.14.6. Cho X và Y là hai đa tạp giải tích trên L, và cho $f : X_\sigma \to Y$ là một ánh xạ $\sigma$-giải tích. Giả sử rằng đặc số của K là 0. Khi đó, để $f$ là giải tích trên L, điều kiện cần và đủ là, với mọi $a \in X$, ánh xạ $T_a(f)$ là L-tuyến tính.

Khi $K = \mathbf{R},\ L = \mathbf{C}$ (trường hợp (a) của No. 5.14.2), ta có một kết quả chính xác hơn: nếu $X$ và $Y$ là hữu hạn chiều và nếu $f : X \to Y$ là một ánh xạ lớp $C^1$ mà ánh xạ tiếp xúc của nó tại mọi điểm của $x$ là $\mathbf{C}$-tuyến tính, thì $f$ là giải tích phức.

5.14.7. Cho $X$ là một đa tạp *giải tích phức* và g là một ánh xạ của X vào chính nó thỏa mãn các điều kiện:
(i) Ta có $g \circ g = \mathrm{Id}_X$.
(ii) Ánh xạ g là một đẳng cấu của đa tạp giải tích $X$ lên đa tạp liên hợp $\overline{X}$ (5.14.2).

Tập hợp $X_0$ gồm các điểm $x$ của $X$ sao cho $g(x) = x$ là một đa tạp con giải tích đóng của đa tạp giải tích thực nền của $X$. Với $x \in X_0$, ta có $T_x(X) = T_x(X_0) \oplus i T_x(X_0)$.

Cho $U$ là một tập mở *liên thông* của $X$ và cho $f$ và $g$ là hai ánh xạ giải tích phức của $U$ vào một không gian lồi địa phương phức tách được hoặc vào một đa tạp giải tích phức tách được. Nếu $f$ và $g$ trùng nhau trên một tập con khác rỗng của $U \cap X_0$, mở trong $X_0$, thì $f = g$.

Giả sử $X_0$ paracompact. Nếu $f$ là một ánh xạ giải tích thực của $X_0$ vào một không gian lồi địa phương tách được hoặc vào một đa tạp giải tích phức tách được, thì tồn tại một lân cận mở $U$ của $X_0$ trong $X$ và một ánh xạ giải tích phức của $U$ vào không gian giá trị của $f$, mở rộng $f$. Hai mở rộng như vậy trùng nhau trên một lân cận của $X_0$ trong $X$.

Giả sử $X$ hữu hạn chiều. Với mọi điểm $a \in X_0$, tồn tại một hệ tọa độ (phức) $\zeta^1, \ldots, \zeta^n$ trong một lân cận mở $U$ của $a$, sao cho $\zeta^i \circ g = \bar{\zeta}^i$ với $1 \leq i \leq n$; hạn chế $\zeta^i$ của $\zeta^i$ vào $U \cap X_0$ khi đó có giá trị thực và $(\xi^1, \ldots, \xi^n)$ là một hệ tọa độ tại $a$ của đa tạp giải tích thực $X_0$.

5.14.8. Với mọi đa tạp giải tích thực $Y$, *paracompact*, tồn tại một cặp $(X, g)$ gồm một đa tạp giải tích phức $X$ và một ánh xạ $g$ của $X$ vào chính nó thỏa mãn các điều kiện (i) và (ii) của 5.14.7, và một đẳng cấu $f$ của $Y$ lên $X_0$. Ta nói rằng $X$ (được trang bị bởi $f$ và $g$) là một *phức hóa* của $Y$.
