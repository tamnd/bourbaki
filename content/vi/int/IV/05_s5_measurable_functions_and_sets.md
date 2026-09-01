---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 5
section_title: Measurable functions and sets
lang: vi
source: int-i-vi
book_pages: INT IV.59-INT IV.89, INT IV.127-INT IV.134
pdf_pages: 0166-0196, 0234-0241
extraction: ocr
subsections:
    - "no": 1
      title: Definition of measurable functions and sets
      page: 59
      pdf_page: 166
    - "no": 2
      title: Principle of localization. Locally negligible sets
      page: 61
      pdf_page: 168
    - "no": 3
      title: Elementary properties of measurable functions
      page: 63
      pdf_page: 170
    - "no": 4
      title: Limits of measurable functions
      page: 64
      pdf_page: 171
    - "no": 5
      title: Criteria for measurability
      page: 66
      pdf_page: 173
    - "no": 6
      title: Criteria for integrability
      page: 71
      pdf_page: 178
    - "no": 7
      title: Measure induced on a locally compact subspace
      page: 73
      pdf_page: 180
    - "no": 8
      title: $\mu$-dense families of compact sets
      page: 76
      pdf_page: 183
    - "no": 9
      title: Locally countable partitions
      page: 77
      pdf_page: 184
    - "no": 10
      title: Measurable functions defined on a measurable subset
      page: 78
      pdf_page: 185
    - "no": 11
      title: Convergence in measure
      page: 80
      pdf_page: 187
    - "no": 12
      title: A property of vague convergence
      page: 86
      pdf_page: 193
statements: 77
exercises: 30
content_sha256: 1d23bfbc020705f8bd051cbd553ff783d90ab01957002928e00bbd107eddcc10
translated_from: content/en/int/IV/05_s5_measurable_functions_and_sets.md
source_content_sha256: d2dd442a1870a24021fa0c3140fb4294fafea8355aea1aaaf03d6d89003a2756
translation_model: gpt-5.4
translation_run: translate-vi-67b4b1df
glossary_version: 34
glossary_terms_sha256: 8a1bfb9db69bcdb6ba3a2dd0074891eb139e6b46f9c5d048326e3aef3a744722
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. HÀM VÀ TẬP HỢP ĐO ĐƯỢC

### 1. Định nghĩa các hàm và tập hợp đo được

#### Định nghĩa 1 {#int-iv-s5-def-1 .statement}

*Cho $X$ là một không gian địa phương compact, $\mu$ là một độ đo trên $X$. Một ánh xạ $f$ từ $X$ vào một không gian tôpô $F$ được gọi là đo được đối với độ đo $\mu$ (hoặc là $\mu$-đo được) nếu, với mọi tập con compact $K$ của $X$, tồn tại một tập hợp không đáng kể đối với $\mu$ là $N \subset K$ và một phân hoạch của $K - N$ tạo thành bởi một dãy (hữu hạn hoặc vô hạn) $(K_n)$ các tập hợp compact, sao cho hạn chế của $f$ trên mỗi $K_n$ là liên tục.*

Hiển nhiên mọi ánh xạ liên tục từ $X$ vào $F$ đều đo được.

Chú ý rằng nếu $\mu$ và $\nu$ là hai độ đo trên $X$ sao cho mọi tập hợp không đáng kể đối với $\mu$ đều không đáng kể đối với $\nu$, thì *mọi hàm $\mu$-đo được cũng đều $\nu$-đo được* (xem Ch. V, §5, Nos. 5, 6).

Định nghĩa 1 có thể được chuyển thành tiêu chuẩn sau đây:

#### Mệnh đề 1 {#int-iv-s5-prop-1 .statement}

*Để một ánh xạ $f$ từ $X$ vào $F$ là đo được, điều kiện cần và đủ là, với mọi tập hợp compact $K \subset X$ và mọi số $\varepsilon > 0$, tồn tại một tập hợp compact $K_1 \subset K$ sao cho $|\mu|(K - K_1) \leq \varepsilon$ và hạn chế của $f$ trên $K_1$ là liên tục.*

Nếu điều kiện này được thỏa mãn, ta có thể định nghĩa đệ quy một dãy các tập hợp compact rời nhau từng đôi một $K_n \subset K$ sao cho $|\mu|(K - \bigcup_{i=1}^n K_i) \leq 1/n$ và sao cho hạn chế của $f$ trên mỗi $K_n$ là liên tục ($§ 4$, No. 6, Th. 4); phần bù trong $K$ của hợp các $K_n$ khi đó là không đáng kể ($§ 4$, No. 5, Cor. of Prop. 7), do đó $f$ là đo được. Ngược lại, giả sử tồn tại một tập hợp không đáng kể $N \subset K$ và một phân hoạch $(K_n)$ của $K - N$ tạo thành bởi các tập hợp compact sao cho hạn chế của $f$ trên mỗi $K_n$ là liên tục; với mọi $\varepsilon > 0$ tồn tại một số nguyên $n$ sao cho, nếu $H = \bigcup_{i=1}^n K_i$, thì $|\mu|(K - H) \leq \varepsilon$ (§ 4, No. 5, Cor. of Prop. 7); tập hợp $H$ là compact, các $K_i$ ($1 \leq i \leq n$) tạo thành một phân hoạch hữu hạn của $H$ thành các tập hợp compact, và hạn chế của $f$ trên mỗi $K_i$ là liên tục; do đó hạn chế của $f$ trên $H$ là liên tục.

#### Mệnh đề 2 {#int-iv-s5-prop-2 .statement}

*Cho* $(F_n)$ *là một dãy các không gian tôpô và, với mỗi* $n$, *cho* $f_n$ *là một ánh xạ đo được của* $X$ *vào* $F_n$. *Với mọi tập compact* $K \subset X$ *và mọi* $\varepsilon > 0$, *tồn tại một tập compact* $K_0 \subset K$ *sao cho* $|\mu|(K - K_0) \leq \varepsilon$ *và hạn chế trên* $K_0$ *của mỗi hàm* $f_n$ *là liên tục*.

Với mỗi số nguyên $n \geq 1$ tồn tại một tập compact $K_n \subset K$ sao cho $|\mu|(K - K_n) \leq \varepsilon / 2^n$ và hạn chế của $f_n$ trên $K_n$ là liên tục. Tập hợp $K_0 = \bigcap_{n=1}^\infty K_n$ là compact, các hạn chế trên $K_0$ của tất cả các hàm $f_n$ đều liên tục và, vì $K - K_0$ được chứa trong hợp của các $K - K_n$, ta có $|\mu|(K - K_0) \leq \sum_{n=1}^\infty \varepsilon / 2^n = \varepsilon$.

#### Định nghĩa 2 {#int-iv-s5-def-2 .statement}

*Một tập con* $A$ *của* $X$ *được gọi là đo được nếu hàm đặc số* $\varphi_A$ *của nó là đo được*.

Xét theo Định nghĩa 1, nói rằng một tập đo được $A$ là một tập sao cho, với mọi tập compact $K$, tồn tại một tập không đáng kể $N \subset K$ và một phân hoạch $(K_n)$ của $K - N$ tạo thành bởi một dãy các tập compact mà mỗi tập đều được chứa hoặc trong $K \cap A$ hoặc trong $K \cap \complement A$.

Định nghĩa này cho ngay tiêu chuẩn sau:

#### Mệnh đề 3 {#int-iv-s5-prop-3 .statement}

*Để một tập* $A$ *là đo được, điều kiện cần và đủ là, với mọi tập compact* $K$, $A \cap K$ *là khả tích*.

Điều kiện là cần, vì hợp của một dãy các tập khả tích $A_n$ là khả tích khi $\sum_n |\mu|(A_n)$ là hữu hạn (§ 4, No. 5, Hệ quả của Mệnh đề 8). Điều kiện là đủ vì, với mọi tập khả tích $B$, tồn tại một tập không đáng kể $N \subset B$ và một phân hoạch của $B - N$ thành một dãy các tập compact (§ 4, No. 6, Hệ quả 2 của Định lý 4).

#### Hệ quả 1 {#int-iv-s5-prop-3-cor-1 .statement}

*Các tập mở và các tập đóng là đo được*.

Đặc biệt, toàn bộ không gian $X$ là đo được.

#### Hệ quả 2 {#int-iv-s5-prop-3-cor-2 .statement}

— *Nếu X là khả mêtric, thì mọi tập con Souslin A của X* (GT, IX, §6, No. 2) *đều là μ-đo được đối với mọi độ đo μ trên X*.

Theo Mệnh đề 3, chỉ cần kiểm tra rằng mọi tập Souslin tương đối compact A đều là μ-khả tích. Nhưng một tập như vậy A là capacitable đối với $|\mu|^*$ (GT, IX, §6, No. 9, Định lý 5). Do đó, với mọi $ε > 0$ tồn tại một tập con compact K của A sao cho $|\mu|^*(A) \leq |\mu|^*(K) + ε = |\mu|(K) + ε$. Gọi U là một tập mở tương đối compact trong X chứa A sao cho

$$
|\mu|(U) = |\mu|^*(U) \leq |\mu|^*(A) + ε.
$$

Khi đó $|\mu|^*(U - K) = |\mu|(U) - |\mu|(K) \leq 2ε$, do đó $|\mu|^*(A - K) \leq 2ε$, điều này chứng minh rằng A là μ-khả tích (§4, No. 6, Hệ quả 1 của Định lý 4).

### 2. Nguyên lý địa phương hóa. Các tập địa phương không đáng kể

#### Mệnh đề 4 (Nguyên lý địa phương hóa) {#int-iv-s5-prop-4 .statement}

— *Cho f là một ánh xạ của X vào một không gian tôpô F. Giả sử rằng với mọi $x \in X$, tồn tại một lân cận khả tích $V_x$ của x và một ánh xạ đo được $g_x$ của X vào F sao cho $f(y) = g_x(y)$ hầu khắp trên $V_x$. Khi đó f là đo được.*

Cho K là một tập compact; tồn tại một số hữu hạn các điểm $x_i \in K$ sao cho các $V_{x_i}$ tạo thành một phủ của K. Suy ra ngay (§4, No. 9, Bổ đề) rằng tồn tại một tập không đáng kể $N \subset K$ và một phân hoạch hữu hạn của $K - N$ tạo bởi các tập khả tích $M_j$ sao cho mỗi tập $K \cap V_{x_i}$ là hợp của một tập con của N và của một số các $M_j$, và sao cho trên mỗi $M_j$, $f$ bằng một trong các hàm $g_{x_i}$. Bây giờ, với mỗi $M_j$ tồn tại một tập không đáng kể $N_j \subset M_j$ và một phân hoạch của $M_j - N_j$ tạo bởi một dãy các tập compact $K_{nj}\ (\mathbf{n} \in \mathbf{N})$; mặt khác, với mỗi $K_{nj}$ tồn tại một tập không đáng kể $P_{nj} \subset K_{nj}$ và một phân hoạch của $K_{nj} - P_{nj}$ tạo bởi một dãy các tập compact $K_{mnj}\ (\mathbf{m} \in \mathbf{N})$ sao cho hạn chế của $f$ trên mỗi $K_{mnj}$ là liên tục. Vì hợp của N, các $N_j$ và các $P_{nj}$ là không đáng kể, $f$ là đo được.

Do đó khái niệm hàm đo được là một khái niệm có đặc trưng địa phương.

#### Định nghĩa 3 {#int-iv-s5-def-3 .statement}

— *Một tập hợp $A \subset X$ được gọi là không đáng kể địa phương (đối với độ đo $μ$) nếu, với mọi $x \in X$, tồn tại một lân cận $V$ của $x$ sao cho $V \cap A$ là không đáng kể.*

Theo nguyên lý địa phương hóa, mọi tập không đáng kể địa phương đều *đo được*. Các tính chất của các tập không đáng kể (§2) cho thấy rằng mọi tập con của một tập không đáng kể địa phương đều không đáng kể địa phương, và mọi hợp đếm được của các tập không đáng kể địa phương đều không đáng kể địa phương.

#### Mệnh đề 5 {#int-iv-s5-prop-5 .statement}

— *Để một tập A là không đáng kể địa phương, điều kiện cần và đủ là, với mọi tập compact K, $A \cap K$ là không đáng kể.*

Điều kiện này hiển nhiên là đủ vì mọi điểm của X đều có một lân cận compact. Nó là cần, vì nếu, với mọi $x \in K$, tồn tại một lân cận $V_x$ của $x$ sao cho $A \cap V_x$ là không đáng kể, thì tồn tại một số hữu hạn các điểm $x_i \in K$ sao cho các $V_{x_i}$ tạo thành một phủ của K, và $A \cap K$ được chứa trong hợp của các tập không đáng kể $A \cap V_{x_i}$.

#### Hệ quả 1 {#int-iv-s5-prop-5-cor-1 .statement}

— *Để một tập A là không đáng kể, điều kiện cần và đủ là nó không đáng kể địa phương và có độ đo ngoài hữu hạn.*

Điều kiện này hiển nhiên là cần. Ngược lại, nếu nó được thỏa mãn thì A được chứa trong một tập mở khả tích G, là hợp của một tập không đáng kể N và một dãy $(K_n)$ các tập compact (§ 4, No. 6, Hệ quả 2 của Định lý 4); vì $A \cap N$ và các tập $A \cap K_n$ là không đáng kể, hợp của chúng là A cũng vậy.

#### Hệ quả 2 {#int-iv-s5-prop-5-cor-2 .statement}

— *Mọi tập mở không đáng kể địa phương đều không đáng kể* (và do đó được chứa trong phần bù của giá của $\mu$).

Thật vậy, độ đo ngoài của một tập mở G là cận trên đúng của các độ đo $|\mu|(K)$ của các tập compact $K \subset G$ (§ 4, No. 6, Hệ quả 4 của Định lý 4); nếu G không đáng kể địa phương thì $|\mu|(K) = 0$ với mọi tập compact K được chứa trong G, do đó $|\mu|^*(G) = 0$.

#### Hệ quả 3 {#int-iv-s5-prop-5-cor-3 .statement}

— *Trong một không gian compact địa phương X đếm được ở vô cực, mọi tập không đáng kể địa phương đều không đáng kể.*

Vì X là hợp của một dãy $(K_n)$ các tập compact, mọi tập không đáng kể địa phương A là hợp của các tập không đáng kể $A \cap K_n$, nên là không đáng kể.

Có thể cho các ví dụ về những không gian compact địa phương không đếm được ở vô cực, và về những độ đo trên một không gian như vậy X sao cho tồn tại những tập trong X không đáng kể địa phương nhưng không không đáng kể (§ 1, Exer. 5).

#### Hệ quả 4 {#int-iv-s5-prop-5-cor-4 .statement}

— *Cho f là một ánh xạ từ X vào một không gian tôpô F. Nếu tập N các điểm gián đoạn của f là không đáng kể địa phương, thì f là đo được.*

Với mọi tập compact $K \subset X$, $K \cap N$ là không đáng kể (Mệnh đề 5), do đó, với mọi $\varepsilon > 0$, tồn tại một tập compact $K_1 \subset K - (K \cap N)$ sao cho $|\mu|(K - K_1) \leq \varepsilon$ (§ 4, No. 6, Định lý 4), và theo giả thiết hạn chế của f trên $K_1$ là liên tục, do đó suy ra kết luận.

Nếu $P\{x\}$ là một tính chất, thì theo định nghĩa, tính chất « *P\{x\} địa phương hầu khắp mọi nơi (đối với $\mu$)* » tương đương với tính chất « *tập hợp các x sao cho* (x $\in$ X and not $P\{x\}$) *là địa phương không đáng kể (đối với độ đo* $\mu$) ». Nếu F là một tập hợp bất kỳ, quan hệ «$f(x) = g(x)$ địa phương hầu khắp mọi nơi» là một quan hệ tương đương trong tập hợp các ánh xạ từ X vào F. Đặc biệt, nếu F là một không gian vectơ, một ánh xạ $f$ từ X vào F sao cho f(x) = $0\text{ hầu khắp mọi nơi địa phương được gọi là } \textit{địa phương không đáng kể}$. Chúng tôi để cho người đọc tự thiết lập đối với các khái niệm này phần lớn các tính chất tương ứng với những tính chất đã được liệt kê trong §2, Nos. 4, 5 và 6 đối với các hàm bằng nhau hầu khắp mọi nơi. Chúng tôi sẽ chỉ giới hạn ở việc nhận thấy rằng nếu hai ánh xạ \emph{liên tục} $f, g$ từ X vào một không gian tôpô Hausdorff F bằng nhau \emph{địa phương hầu khắp mọi nơi}, thì chúng bằng nhau \emph{hầu khắp mọi nơi} theo Hệ quả 2 của Mệnh đề 5 (do đó bằng nhau tại mọi điểm thuộc giá của $\mu$ (§ 2, No. 4, Prop. 9)); tuy nhiên, chúng tôi phát biểu tường minh mệnh đề sau đây, là một hệ quả ngay lập tức của nguyên lý địa phương hóa:

#### Mệnh đề 6 {#int-iv-s5-prop-6 .statement}

*Cho $f$ là một ánh xạ đo được từ X vào một không gian tôpô F. Mọi ánh xạ từ X vào F bằng với $f$ địa phương hầu khắp mọi nơi đều đo được.*

### 3. Các tính chất sơ cấp của các hàm đo được

#### Định lý 1 {#int-iv-s5-thm-1 .statement}

*Cho X là một không gian compact địa phương, $\mu$ một độ đo trên X, $(F_n)$ một dãy các không gian tôpô, $F = \prod_n F_n$ là tích của chúng. Với mỗi chỉ số n, cho $f_n$ là một ánh xạ đo được từ X vào $F_n$, và đặt $f(x) = (f_n(x)) \in F$; khi đó, với mọi ánh xạ liên tục u từ $f(X)$ vào một không gian tôpô G, hàm $x \mapsto u(f(x))$ là đo được.*

Với mọi tập con compact K của X và mọi số $\varepsilon > 0$, tồn tại một tập compact $K_1 \subset K$ sao cho $|\mu|(K - K_1) \leq \varepsilon$ và sao cho các hạn chế trên $K_1$ của tất cả các hàm $f_n$ đều liên tục (No. 1, Prop. 2); hiển nhiên là $u \circ f$ liên tục trên $K_1$, do đó suy ra định lý.

#### Nhận xét {#int-iv-s5-n3-rem-1 .statement}

— 1) Định lý không mở rộng được cho một tích \emph{tùy ý} các không gian tôpô (Exer. 1).
2) Nếu $f$ là một ánh xạ liên tục từ X vào chính nó, và $g$ là một ánh xạ đo được từ X vào F, thì $g \circ f$ không nhất thiết đo được (Exer. 2).

#### Hệ quả 1 {#int-iv-s5-thm-1-cor-1 .statement}

*Bao trên và bao dưới của một số hữu hạn các hàm số đo được (hữu hạn hay không) là đo được.*
Thật vậy, $\sup(u, v)$ và $\inf(u, v)$ liên tục trên $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$.

#### Hệ quả 2 {#int-iv-s5-thm-1-cor-2 .statement}

*Để một hàm số $f$ (hữu hạn hay không) là đo được, điều kiện cần và đủ là $f^+$ và $f^-$ đo được.*
Điều kiện là cần theo Hệ quả 1; nó là đủ vì ảnh A của X trong $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ dưới ánh xạ $x \mapsto (f^+(x), f^-(x))$ không chứa các điểm $(+\infty, +\infty)$ và $(-\infty, -\infty)$, do đó ánh xạ $(u, v) \mapsto u - v$ liên tục trên A.

#### Hệ quả 3 {#int-iv-s5-thm-1-cor-3 .statement}

— *Nếu f và g là hai ánh xạ đo được từ X vào một không gian vectơ tôpô F, thì f + g và αf là đo được (α là một vô hướng tùy ý).*

Như vậy tập hợp các ánh xạ đo được từ X vào một không gian vectơ tôpô F là một không gian vectơ.

#### Hệ quả 4 {#int-iv-s5-thm-1-cor-4 .statement}

— *Cho F là một không gian vectơ chiều n trên R và $(e_k)_{1 \leq k \leq n}$ là một cơ sở của F. Để một hàm $f = \sum_{k=1}^{n} e_k f_k$ là đo được, điều kiện cần và đủ là mỗi hàm số $f_k$ đều đo được.*

#### Hệ quả 5 {#int-iv-s5-thm-1-cor-5 .statement}

— *Cho F, G, H là ba không gian vectơ tôpô, và cho (u, v) \to [u \cdot v] là một ánh xạ song tuyến tính liên tục từ F \times G vào H. Nếu f là một ánh xạ đo được từ X vào F, và g là một ánh xạ đo được từ X vào G, thì [f \cdot g] là một ánh xạ đo được từ X vào H.*

Đặc biệt, nếu f là một ánh xạ đo được từ X vào một không gian định chuẩn thực (resp. phức) F, và g là một ánh xạ đo được từ X vào R (resp. C), thì gf là đo được. Nếu F là một *đại số định chuẩn* và f, g là hai ánh xạ đo được từ X vào F, thì fg là đo được.

#### Hệ quả 6 {#int-iv-s5-thm-1-cor-6 .statement}

— *Nếu f là một ánh xạ đo được từ X vào một không gian định chuẩn F, thì hàm số |f| là đo được.*

### 4. Giới hạn của các hàm đo được

#### Định lý 2 (Egoroff) {#int-iv-s5-thm-2 .statement}

— *Cho X là một không gian compact địa phương, μ một độ đo trên X, A một tập hợp đếm được, $\mathfrak{F}$ một bộ lọc trên A có một cơ sở đếm được, và $(f_\alpha)_{\alpha \in A}$ một họ các ánh xạ đo được từ X vào một không gian khả mêtric F. Giả sử rằng $\lim_{\mathfrak{F}} f_\alpha(x) = f(x)$ tồn tại trên phần bù của một tập con địa phương không đáng kể N của X. Trong các điều kiện đó,
1° hàm f (được mở rộng lên N theo một cách bất kỳ) là đo được;
2° với mọi tập con compact K của X và mọi $\varepsilon > 0$, tồn tại một tập compact $K_1 \subset K$ sao cho $|\mu|(K - K_1) \leq \varepsilon$ và sao cho các hạn chế của các $f_\alpha$ trên $K_1$ là liên tục và hội tụ đều đến f trên $K_1$.

Mệnh đề thứ nhất hiển nhiên suy ra từ mệnh đề thứ hai, điều mà ta sẽ chứng minh. Tồn tại một tập compact $K_0 \subset K$ sao cho $|\mu|(K - K_0) \leq \varepsilon/2$ và sao cho các hạn chế lên $K_0$ của mọi hàm $f_\alpha$ đều liên tục (No. 1, Prop. 2). Gọi $(A_n)$ là một cơ sở đếm được giảm của bộ lọc $\mathfrak{F}$; gọi d là một metric trên F tương thích với tôpô. Với mọi cặp số nguyên $n > 0,\ r > 0$, gọi $B_{n,r}$ là tập hợp các điểm $x \in K_0$ sao cho, đối với ít nhất một cặp chỉ số $\alpha, \beta$ thuộc $A_n$, ta có $d(f_\alpha(x), f_\beta(x)) \geq 1/r$; với $\alpha$ và $\beta$ cố định, tập hợp các $x \in K_0$ sao cho $d(f_\alpha(x), f_\beta(x)) \geq 1/r$ là đóng trong $K_0$, nên là compact; do đó, $B_{n,r}$ là một hợp đếm được các tập compact được chứa trong $K_0$, nên khả tích (§ 4, No. 5, Props. 6 and 8). Nếu $r$ cố định, thì giao của dãy giảm các tập hợp $B_{n,r}$ ($n = 1, 2, \ldots$) có độ đo không, vì $f_\alpha(x)$ tiến tới $f(x)$ hầu khắp mọi nơi trong $K_0$ đối với bộ lọc $\mathfrak{F}$; do đó $\lim_{n \to \infty} |\mu|(B_{n,r}) = 0$ (§ 4, No. 5, Cor. of Prop. 7), do đó tồn tại một số nguyên $n_r$ sao cho $|\mu|(B_{n_r,r}) \leq \varepsilon/2^{r+2}$. Gọi $B$ là hợp (với $r = 1, 2, \ldots$) của các tập $B_{n_r,r}$; $B$ khả tích và

$$
|\mu|(B) \leq \sum_{r=1}^\infty |\mu|(B_{n_r,r}) \leq \varepsilon/4
$$

(§ 4, No. 5, Cor. of Prop. 8). Gọi $C$ là phần bù của $B$ trong $K_0$; theo phép dựng, $f_\alpha(x)$ hội tụ đều tới $f(x)$ trên $C$ đối với bộ lọc $\mathfrak{F}$, và vì các hạn chế của các $f_\alpha$ lên $C$ là liên tục, nên hạn chế của $f$ lên $C$ cũng vậy. Khi đó chỉ cần lấy một tập compact $K_1 \subset C$ sao cho $|\mu|(C - K_1) \leq \varepsilon/4$ để thỏa mãn các điều kiện của mệnh đề, vì $|\mu|(K - K_1) = |\mu|(K - K_0) + |\mu|(B) + |\mu|(C - K_1) \leq \varepsilon$.

Các kết luận của Th. 2 không nhất thiết còn đúng nếu $F$ không khả mêtric hóa (Exer. 1). Nếu $F$ khả mêtric hóa, và tập hợp $A$ không đếm được nhưng bộ lọc $\mathfrak{F}$ có một cơ sở đếm được, thì kết luận thứ nhất của Th. 2 lại vẫn đúng; thật vậy, nếu $(A_n)$ là một cơ sở đếm được của $\mathfrak{F}$ và $\alpha_n$ là một phần tử của $A_n$, thì $f$ là giới hạn của dãy $(f_{\alpha_n})$ địa phương hầu khắp mọi nơi, nên là đo được; tuy nhiên, kết luận thứ hai của Th. 2 không còn nhất thiết đúng nữa (x. Exer. 4).

#### Hệ quả 1 {#int-iv-s5-thm-2-cor-1 .statement}

— *Cho* $(f_n)$ *là một dãy các hàm số (hữu hạn hoặc không)*. *Nếu các* $f_n$ *đo được, thì các hàm* $\sup_n f_n$, $\inf_n f_n$, $\limsup_{n \to \infty} f_n$ *và* $\liminf_{n \to \infty} f_n$ *đều đo được*.

Thật vậy, đường thẳng thực mở rộng $\overline{\mathbf{R}}$, do đồng phôi với một khoảng compact của $\mathbf{R}$, là khả mêtric. Hàm $\sup_n f_n$ là giới hạn từng điểm của dãy tăng các hàm $g_n = \sup(f_1, f_2, \ldots, f_n)$, các hàm này đo được (No. 3, Hệ quả 1 của Định lý 1); tương tự, $\limsup_{n \to \infty} f_n$ là giới hạn từng điểm của dãy giảm các hàm $h_n = \sup_{p \geq 0} f_{n+p}$, trong đó mỗi hàm đều đo được theo điều vừa nói trên. Sau cùng, vì $\inf_n f_n = -\sup(-f_n)$ và $\liminf_{n \to \infty} f_n = -\limsup_{n \to \infty} (-f_n)$, các hàm này đo được.

#### Hệ quả 2 {#int-iv-s5-thm-2-cor-2 .statement}

— *Các tập hợp đo được trong* $X$ *lập thành một bộ lạc* (GT, IX, §6, No. 3).

Thật vậy, nếu M và N đo được thì các hàm

$$
\varphi_{M \cup N} = \varphi_M + \varphi_N - \varphi_M \varphi_N \quad \text{và} \quad \varphi_{M \cap C_N} = \varphi_M - \varphi_M \varphi_N
$$

đo được theo No. 3, Hệ quả 3 và 5 của Định lý 1. Nếu $(M_n)$ là một dãy các tập hợp đo được và M là hợp của chúng, thì $\varphi_M = \sup_n \varphi_{M_n}$ đo được theo Hệ quả 1 của Định lý 2, do đó có hệ quả.

Đặc biệt, vì các tập mở là đo được:

#### Hệ quả 3 {#int-iv-s5-thm-2-cor-3 .statement}

*Các tập Borel trong X* (GT, IX, §6, No. 3, Định nghĩa 4) *đều $\mu$-đo được đối với mọi độ đo $\mu$ trên X*.

### 5. Các tiêu chuẩn về tính đo được

Khi F là một không gian vectơ tôpô, mọi hàm thang trên các tập hợp đo được (§4, No. 9, Định nghĩa 4), nhận giá trị trong F, hiển nhiên là đo được (No. 3, Hệ quả 3 của Định lý 1); một hàm như vậy $f$ chỉ nhận một số hữu hạn giá trị, và với mọi $y \in F$, $f^{-1}(y)$ là đo được. Nói chung, cho F là một không gian tôpô bất kỳ, $f$ là một ánh xạ từ X vào F chỉ nhận một số hữu hạn giá trị phân biệt $a_i$ ($1 \leq i \leq m$); nếu các tập hợp $A_i = f^{-1}(a_i)$ đo được, thì hàm $f$ đo được. Thật vậy, với mọi tập compact K và với mỗi tập hợp $A_i \cap K$, tồn tại một tập hợp không đáng kể $N_i \subset A_i \cap K$ và một phân hoạch của $A_i \cap K \cap C N_i$ được tạo thành bởi một dãy $(K_{in})$ các tập compact; vì K là hợp của các tập hợp $A_i \cap K$ và hạn chế của $f$ trên mỗi $K_{in}$ là hằng, do đó liên tục, nên $f$ đo được. Do lạm dụng ngôn ngữ, ta sẽ nói rằng một ánh xạ $f$ từ X vào F là một *hàm thang đo được* nếu nó chỉ nhận một số hữu hạn giá trị và nếu, với mọi $y \in F$, $f^{-1}(y)$ đo được.

#### Định lý 3 {#int-iv-s5-thm-3 .statement}

*Để một ánh xạ $f$ từ X vào một không gian khả mêtric F là đo được, điều kiện cần và đủ là, với mọi tập compact $K \subset X$, tồn tại một dãy $(g_n)$ các hàm thang đo được, nhận giá trị trong F, sao cho $g_n(x)$ tiến tới $f(x)$ với hầu khắp mọi $x \in K$*.

Điều kiện là đủ theo định lý Egoroff và nguyên lý địa phương hóa. Hãy chứng minh rằng nó là cần thiết: theo giả thiết, tồn tại một tập không đáng kể $N \subset K$ và một phân hoạch $(K_m)$ của $K - N$ gồm các tập compact sao cho hạn chế của $f$ trên mỗi $K_m$ là liên tục. Để định nghĩa dãy $(g_n)$, chỉ cần tiến hành theo cách sau: lấy $d$ là một metric tương thích với tôpô của F; với mỗi $K_i$ có chỉ số $i \leq n$, tồn tại một phân hoạch hữu hạn của $K_i$ thành các tập khả tích $A_{ij}$ ($1 \leq j \leq q_i$) đủ nhỏ để độ dao động của $f$ trên mỗi $A_{ij}$ là $\leq 1/n$ (§ 4, No. 9, Bổ đề); lấy $g_n$ là hằng trên mỗi $A_{ij}$, bằng một trong các giá trị của $f$ trong tập hợp này (với $1 \leq i \leq n,\ 1 \leq j \leq q_i$), và bằng một phần tử cố định $a \in \mathbf{F}$ tại mọi điểm của $X$ không thuộc bất kỳ $A_{ij}$ nào. Rõ ràng dãy $(g_n(x))$ hội tụ về $f(x)$ tại mọi điểm của $K$ không thuộc $N$.

#### Hệ quả 1 {#int-iv-s5-thm-3-cor-1 .statement}

*Cho $f$ là một ánh xạ đo được từ $X$ vào một không gian Banach $F$; với mọi tập compact $K \subset X$, tồn tại một dãy $(g_n)$ các hàm bậc thang đo được, có giá đỡ được chứa trong $K$, sao cho $|g_n(x)| \leq |f(x)|$ với mọi $x \in X$ và sao cho $g_n(x)$ tiến tới $f(x)$ với hầu khắp mọi $x \in K$.*

Với các ký hiệu như trong chứng minh của Định lý 3, và ký hiệu bởi $a_{ij}$ một trong các giá trị của $f$ trong $A_{ij}$, chỉ cần lấy, làm giá trị của $g_n$ trong $A_{ij}$, điểm 0 nếu $|a_{ij}| \leq 1/n$ và điểm $a_{ij}(1 - 1/(n|a_{ij}|))$ trong trường hợp ngược lại; sau cùng, đặt $g_n(x) = 0$ trên phần bù của hợp các $A_{ij}$ ($1 \leq i \leq n,\ 1 \leq j \leq q_i$).

#### Hệ quả 2 {#int-iv-s5-thm-3-cor-2 .statement}

*Cho $X$ là một không gian địa phương compact đếm được ở vô cực. Nếu $f$ là một ánh xạ đo được từ $X$ vào một không gian khả mêtric $F$, thì tồn tại một dãy $(g_n)$ các hàm bậc thang đo được, nhận giá trị trong $F$, sao cho $g_n(x)$ tiến tới $f(x)$ với hầu khắp mọi $x \in X$.*

Nếu $X$ là hợp của một dãy tăng $(A_n)$ các tập compact, thì các tập $A_n - A_{n-1}$ khác rỗng tạo thành một phân hoạch của $X$ thành các tập hợp khả tích; do đó, tồn tại một tập không đáng kể $N \subset X$ và một phân hoạch của $\mathbf{C}N$ gồm một dãy $(K_n)$ các tập compact sao cho hạn chế của $f$ trên mỗi $K_n$ là liên tục; khi đó có thể kết thúc chứng minh như trong Đl. 3 mà không cần sửa đổi.

#### Mệnh đề 7 {#int-iv-s5-prop-7 .statement}

*Cho $f$ là một ánh xạ đo được từ $X$ vào một không gian tôpô $F$; ảnh ngược theo $f$ của mọi tập đóng (tương ứng, mở) trong $F$ đều đo được.*

Chỉ cần thực hiện chứng minh đối với ảnh ngược $^{-1}f(A)$ của một tập đóng $A$ trong $F$. Cho $K$ là một tập con compact của $X$; tồn tại một tập không đáng kể $N \subset K$ và một phân hoạch $(K_n)$ của $K - N$ gồm các tập compact sao cho hạn chế của $f$ trên mỗi $K_n$ là liên tục. Khi đó giao $K_n \cap ^{-1}f(A)$ là ảnh ngược của tập đóng $A$ theo hạn chế của $f$ trên $K_n$; vì vậy nó là một tập đóng trong $K_n$, nên compact. Do đó tập $K \cap ^{-1}f(A)$ là hợp của tập không đáng kể $N \cap ^{-1}f(A)$ và các tập compact $K_n \cap ^{-1}f(A)$, điều này chứng minh rằng $^{-1}f(A)$ là đo được.

#### Định lý 4 {#int-iv-s5-thm-4 .statement}

— Cho F là một không gian khả mêtric hóa và d là một mêtric trên F tương thích với tôpô. Để một ánh xạ f từ X vào F là đo được, điều kiện cần và đủ là nó thỏa mãn hai điều kiện sau:
a) ảnh ngược theo f của mọi quả cầu đóng của F là đo được;
b) với mọi tập compact K ⊂ X, tồn tại một tập con đếm được H của F sao cho $f(x) \in \overline{H}$ với hầu khắp mọi $x \in K$.

Điều kiện a) là cần theo Mệnh đề 7; mặt khác, theo các ký hiệu của Đl. 3, điều kiện b) được thỏa mãn khi lấy H là tập đếm được tạo bởi các giá trị của tất cả các hàm $g_n$.

Bây giờ ta hãy chỉ ra rằng các điều kiện a) và b) là đủ. Cho K là một tập con compact bất kỳ của X; tồn tại một tập con không đáng kể N của K sao cho $f(K - N)$ được chứa trong bao đóng của một tập đếm được các điểm của F, mà ta sắp thành một dãy $(a_n)$. Gọi $A_{n,p}$ là tập hợp các $x \in K - N$ sao cho $d(f(x), a_n) \leq 1/p$. Theo điều kiện a), suy ra $A_{n,p}$ là đo được. Với $p$ cố định, định nghĩa truy hồi một dãy các tập $B_{n,p} \subset K - N$ bằng cách đặt

$$
B_{1,p} = A_{1,p} \quad \text{và} \quad B_{n+1,p} = A_{n+1,p} \cap C \left( \bigcup_{k \leq n} A_{k,p} \right);
$$

các tập $B_{n,p}$ là đo được, và những tập khác rỗng tạo thành một phân hoạch của $K - N$. Gọi $g_{m,p}$ là hàm bằng $a_i$ trên tập $B_{i,p}$ với $1 \leq i \leq m$ và bằng một hằng $b \in F$ trên phần bù của hợp của các tập ấy; $g_{m,p}$ là một hàm bậc thang đo được; khi $m$ tiến ra vô hạn, $g_{m,p}$ hội tụ điểm đến hàm $f_p$ bằng $a_n$ trên $B_{n,p}$ ($n \geq 1$) và bằng $b$ trên $N \cup C K$, do đó (Định lý 2) $f_p$ là đo được. Khi $p$ tiến ra vô hạn, $f_p(x)$ tiến đến $f(x)$ với mọi $x \in K - N$, và đến $b$ với $x \in N \cup C K$; vì thế giới hạn của các $f_p$ là đo được, và nguyên lý địa phương hóa chứng minh rằng bản thân $f$ là đo được.

#### Nhận xét 1 {#int-iv-s5-n5-rem-1 .statement}

Chỉ riêng điều kiện a) không đủ để $f$ đo được (Bài tập 7).
2) Nếu tôpô của F có một cơ sở đếm được thì điều kiện b) của Định lý 4 tự động được thỏa mãn đối với mọi ánh xạ từ X vào F. Hơn nữa, chứng minh cho thấy rằng chỉ cần giả thiết các ảnh ngược qua $f$ của các quả cầu đóng có bán kính hữu tỉ, với tâm thuộc một tập con đếm được trù mật của F, là các tập hợp đo được.
3) Giả thiết a) có thể được thay bằng điều kiện rằng ảnh ngược qua $f$ của mọi quả cầu mở của F đều đo được.

Trường hợp các hàm số (hữu hạn hoặc không) đáng được nói riêng:

#### Mệnh đề 8 {#int-iv-s5-prop-8 .statement}

— Cho D là một tập con đếm được trù mật của $\mathbf{R}$. Để một hàm số $f$ (hữu hạn hoặc không) là đo được, điều kiện đủ (và cần) là với mọi $a \in D$, tập hợp các $x \in X$ sao cho $f(x) \geq a$ là đo được.

Thật vậy, nếu như vậy thì, với mọi $b \in \overline{\mathbf{R}}$, tập hợp các $x$ sao cho $f(x) \geqslant b$ là đo được, vì đó là giao của các tập hợp (tạo thành một họ đếm được) các $x$ sao cho $f(x) \geqslant a$, khi $a$ chạy qua tập hợp các điểm của D mà $\leqslant b$. Tập hợp các $x$ sao cho $f(x) < b$ là đo được, vì đó là phần bù của một tập hợp đo được. Tiếp theo, nếu $b$ là hữu hạn thì tập hợp các $x$ sao cho $f(x) \leqslant b$ là đo được, vì đó là giao của các tập hợp các $x$ sao cho $f(x) < b + 1/n$; và $f(-\infty)^{-1}$ là đo được, vì đó là giao của các tập hợp các $x$ sao cho $f(x) < n$, khi $n$ chạy qua $\mathbf{Z}$. Sau cùng, ảnh ngược qua $f$ của mọi khoảng đóng của $\overline{\mathbf{R}}$ là đo được, vì đó là giao của hai tập hợp đo được, và có thể áp dụng Định lý 4.

Tương tự, người ta có thể chứng minh rằng chỉ cần với mọi $a \in \mathrm{D}$, tập hợp các $x$ sao cho $f(x) > a$ là đo được.

#### Hệ quả {#int-iv-s5-n5-cor-1 .statement}

— *Mọi hàm nửa liên tục dưới* (ứng với *nửa liên tục trên*) *đều đo được*.

Thật vậy, nếu $f$ là nửa liên tục dưới, thì tập hợp các $x \in \mathrm{X}$ sao cho $f(x) \leqslant a$ là đóng với mọi $a \in \overline{\mathbf{R}}$.

Khi F khả mêtric và *compact*, Mệnh đề 7 cho phép làm sắc bén hơn Định lý 3 như sau:

#### Mệnh đề 9 {#int-iv-s5-prop-9 .statement}

— *Nếu F là một không gian compact khả mêtric, thì mọi ánh xạ đo được $f$ từ X vào F đều là giới hạn đều (trên toàn bộ X) của một dãy các hàm bậc thang đo được*.

Gọi $d$ là một metric tương thích với tôpô của F. Với mỗi số nguyên dương $n$ tồn tại một số *hữu hạn* các điểm $a_k \in \mathrm{F}$ sao cho các quả cầu đóng $B_k$ tâm $a_k$ và bán kính $1/n$ tạo thành một phủ của F; do đó các tập hợp $A_k = f^{-1}(B_k)$ là đo được (Mệnh đề 7) và tạo thành một phủ của X. Do đó (§ 4, No. 9, Bổ đề) tồn tại một phân hoạch $(C_i)$ của X thành một số hữu hạn các tập hợp đo được sao cho mỗi $A_k$ là hợp của một số $C_i$ nào đó. Gọi $c_i$ là một điểm của $C_i$ và gọi $g_n$ là hàm bậc thang đo được bằng $f(c_i)$ trên $C_i$ (với mỗi chỉ số $i$). Hiển nhiên là $d(f(x), g_n(x)) \leqslant 2/n$ với mọi $x \in \mathrm{X}$.

#### Mệnh đề 10 {#int-iv-s5-prop-10 .statement}

— *Cho F là một không gian Banach tách được, F' là đối ngẫu của nó, và $(\mathbf{a}'_n)$ là một dãy trù mật yếu trong quả cầu đơn vị của F' (TVS, III, § 3, No. 4, Hệ quả 2 của Mệnh đề 6).*¹ *Để một ánh xạ f từ X vào F là đo được, điều kiện cần và đủ là với mọi n hàm vô hướng $x \mapsto \langle \mathbf{f}(x), \mathbf{a}'_n \rangle$ là đo được*.

Điều kiện này hiển nhiên là cần (No. 3, Định lý 1), hãy chứng minh rằng nó là đủ; chỉ cần kiểm tra điều kiện a) của Định lý 4 và, để làm điều này,

¹ Xem chú thích ở cuối § 2, No. 4.

theo nguyên lý địa phương, chỉ cần chứng minh rằng, với mọi tập compact K của X và mọi quả cầu đóng $B \subset F$, tâm $a$ và bán kính $r$, tập hợp $A = K \cap f^{-1}(B)$ là đo được; mà, với mọi $z \in F$,

$$
|z| = \sup_n |\langle z, a'_n \rangle| / |a'_n|;
$$

do đó $A$ là giao của $K$ và các tập hợp được xác định bởi

$$
|\langle f(x), a'_n \rangle - \langle a, a'_n \rangle| \leq r |a'_n|;
$$

vì các tập hợp này là đo được theo giả thiết, $A$ là đo được.

#### Hệ quả 1 {#int-iv-s5-prop-10-cor-1 .statement}

*Cho F là một không gian Banach. Để một ánh xạ f từ X vào F là đo được, điều kiện cần và đủ là nó thỏa mãn hai điều kiện sau:*

a) *với mọi $a' \in F'$, hàm vô hướng $x \mapsto \langle f(x), a' \rangle$ là đo được;*

b) *với mọi tập compact $K \subset X$, tồn tại một tập con đếm được H của F sao cho $f(x) \in \overline{H}$ với hầu khắp mọi $x \in K$.*

Tính cần thiết của các điều kiện suy ra từ No. 3, Định lý 1, và Định lý 4. Để chứng minh rằng các điều kiện là đủ, ở đây cũng chỉ cần kiểm tra điều kiện a) của Định lý 4. Với các ký hiệu như trong chứng minh của Mệnh đề 10, ta có thể (do b)) giả sử, sau khi sửa đổi $f$ nếu cần trên một tập không đáng kể, rằng $f(K) \subset \overline{H}$, trong đó $H$ là một tập con đếm được của $F$. Nếu $V$ là không gian con tuyến tính đóng của $F$ được sinh bởi tập hợp $H \cup \{a\}$, thì $V$ là một không gian Banach tách được và mọi dạng tuyến tính liên tục trên $V$ đều là hạn chế của một dạng $a' \in F'$; cùng một lập luận như trong Mệnh đề 10 khi đó cho thấy rằng $K \cap f^{-1}(B)$ là đo được.

#### Hệ quả 2 {#int-iv-s5-prop-10-cor-2 .statement}

*Cho F là một không gian lồi địa phương vừa khả mêtric vừa tách được, và gọi $F'$ là đối ngẫu của nó. Để một ánh xạ f từ X vào F là đo được, điều kiện cần và đủ là với mọi $a' \in F'$, hàm vô hướng $x \mapsto \langle f(x), a' \rangle$ là đo được.*

Ta có thể xem F như một không gian con của một tích đếm được $\prod_n E_n$ của các không gian Banach (TVS, II, §4, No. 3), và ta có thể giả sử rằng $\operatorname{pr}_n(F)$ là trù mật trong $E_n$, do đó $E_n$ là tách được. Với mọi $n$, ánh xạ $\operatorname{pr}_n \circ f$ khi đó là đo được theo Mệnh đề 10, do đó $f$ là đo được theo No. 3, Định lý 1.

#### Mệnh đề 11 {#int-iv-s5-prop-11 .statement}

*Cho F là một không gian lồi địa phương là giới hạn trực tiếp của một dãy các không gian lồi địa phương khả mêtric tách được $F_n$, F là hợp của các $F_n$. Cho $F'$ là đối ngẫu của F, được trang bị tôpô yếu $\sigma(F', F)$. Để một ánh xạ f từ X vào $F'$ là đo được, điều kiện cần và đủ là, với mọi $a \in F$, hàm vô hướng $x \mapsto \langle a, f(x) \rangle$ là đo được.*

Điều kiện là cần theo No. 3, Th. 1; hãy chứng minh rằng nó là đủ. Trước hết giả sử rằng F là mêtric và tách được, và cho D là một tập hợp trù mật đếm được trong F. Cho $(V_n)$ là một dãy cơ bản giảm các lân cận mở lồi cân bằng của 0 trong F; các tập cực $V_n^\circ$ là đồng liên tục và hợp của chúng là toàn bộ $F'$. Đặt $X_n = f^{-1}(V_n^\circ)$; dãy $(X_n)$ là tăng và $X = \bigcup_n X_n$; hãy chỉ ra rằng mỗi $X_n$ là $\mu$-đo được. Thật vậy, $D \cap V_n$ trù mật trong $V_n$; với mọi $y \in D \cap V_n$ đặt $S_y$ là tập hợp các $x \in X$ sao cho $|\langle y, f(x) \rangle| \leq 1$; giả thiết kéo theo rằng mỗi $S_y$ đều đo được, và $X_n$ là giao của họ đếm được các $S_y$ với $y \in D \cap V_n$. Một khi điều đó đã được thiết lập, với mọi tập con compact K của X và mọi $\varepsilon > 0$, tồn tại một số nguyên n sao cho $|\mu|(K - (K \cap X_n)) \leq \varepsilon/4$, rồi một tập con compact $K_1$ của $K \cap X_n$ sao cho $|\mu|((K \cap X_n) - K_1) \leq \varepsilon/4$; cuối cùng, tồn tại một tập con compact $K_2$ của $K_1$ sao cho $|\mu|(K_1 - K_2) \leq \varepsilon/2$ và sao cho các hạn chế lên $K_2$ của tất cả các hàm $\langle y, f \rangle$, với $y \in D$, là liên tục (No. 1, Prop. 2). Vì tập hợp $f(K_2) \subset f(X_n) \subset V_n^\circ$ là đồng liên tục, tôpô cảm sinh bởi $\sigma(F', F)$ trên $f(K_2)$ đồng nhất với tôpô hội tụ điểm trên D (GT, X, §2, No. 4, Th. 1); do đó hạn chế của f lên $K_2$ là liên tục, do đó mệnh đề của ta trong trường hợp thứ nhất này.

Hãy chuyển sang trường hợp tổng quát. Nếu $z'$ là một dạng tuyến tính liên tục trên F, thì hạn chế $z'_n$ của nó lên $F_n$ là liên tục; vì $F = \bigcup_n F_n$, đối ngẫu $F'$ của F có thể được đồng nhất (về mặt đại số) với một không gian con tuyến tính của tích $\prod_n F'_n$, và khi đó $\operatorname{pr}_n(z') = z'_n$. Hơn nữa, vì mọi tập con hữu hạn của F đều được chứa trong một trong các $F_n$, tôpô $\sigma(F', F)$ không là gì khác ngoài tôpô cảm sinh bởi tôpô tích của các tôpô $\sigma(F'_n, F_n)$. Một khi điều đó đã được thiết lập, nếu $\langle a, f \rangle$ đo được với mọi $a \in F$, thì $\langle a_n, \operatorname{pr}_n \circ f \rangle$ cũng vậy với mọi n và mọi $a_n \in F_n$, vì $\langle a_n, \operatorname{pr}_n \circ f \rangle = \langle a_n, f \rangle$; phần đầu của chứng minh khi đó chỉ ra rằng $\operatorname{pr}_n \circ f$ đo được với mọi n, do đó f cũng đo được (No. 3, Th. 1).

### 6. Các tiêu chuẩn về tính khả tích

#### Định lý 5 {#int-iv-s5-thm-5 .statement}

— Để một ánh xạ f từ X vào một không gian Banach F là khả tích lũy thừa bậc p ($1 \leq p < +\infty$), điều kiện cần và đủ là f đo được và $N_p(f)$ là hữu hạn.

Điều kiện là cần thiết: vì, nếu $f \in \mathcal{L}_F^p$ thì tồn tại một dãy $(g_n)$ các hàm liên tục có giá compact hội tụ hầu khắp nơi đến f ($§ 3$, No. 4, Hệ quả 2 của Định lý 3); theo Định lý 2 của No. 4, f là đo được.

Để chứng minh rằng các điều kiện là đủ, trước hết ta thiết lập một bổ đề:

#### Bổ đề 1 {#int-iv-s5-lem-1 .statement}

*Cho g là một hàm nhận giá trị trong F, sao cho N_p(g) < +\infty* (nói cách khác, một hàm trong $\mathcal{F}_F^p$). *Tập hợp A các điểm x \in X sao cho g(x) \neq 0 được chứa trong hợp của một tập không đáng kể và một dãy các tập compact.*

Gọi $A_n$ là tập hợp các điểm $x \in X$ sao cho $|g(x)| \geq 1/n$; A là hợp của các $A_n$, và $\varphi_{A_n} \leq n|g|$, do đó $|\mu|^*(A_n) \leq (n N_p(g))^p$; suy ra $A_n$ được chứa trong hợp của một tập không đáng kể và một dãy các tập compact (§ 4, No. 6, Hệ quả 3 của Định lý 4), bởi vậy A cũng vậy.

Bổ đề đã được chứng minh, trước hết xét trường hợp f có giá *compact* K. Theo Hệ quả 1 của Định lý 3 của No. 5, tồn tại một dãy $(g_n)$ các hàm bậc thang đo được sao cho $|g_n(x)| \leq |f(x)|$ tại mọi điểm $x \in X$ và sao cho $g_n(x)$ tiến tới $f(x)$ hầu khắp nơi. Khi đó, $g_n$ là một tổ hợp tuyến tính của các hàm đặc trưng của các tập hợp đo được được chứa trong K; vì các tập hợp này khả tích theo Mệnh đề 3 của No. 1, nên $g_n$ thuộc $\mathcal{L}_F^p$. Vì $N_p(f) < +\infty$, định lý của Lebesgue (§ 3, No. 7, Định lý 6) cho thấy f thuộc $\mathcal{L}_F^p$.

Trong trường hợp tổng quát, từ Bổ đề 1 suy ra rằng tồn tại một dãy tăng $(K_n)$ các tập compact sao cho $f(x)$ bằng không hầu khắp nơi trong phần bù của hợp các $K_n$. Gọi $f_n$ là hàm bằng $f(x)$ trên $K_n$ và bằng 0 ở nơi khác; $f_n$ là đo được theo No. 3, Hệ quả 5 của Định lý 1; vì $|f_n| \leq |f|$, nên $f_n$ thuộc $\mathcal{L}_F^p$ theo phần đầu của lập luận. Vì $f(x)$ bằng hầu khắp nơi với giới hạn của dãy $f_n(x)$, định lý của Lebesgue lại chứng minh rằng $f \in \mathcal{L}_F^p$, điều này hoàn tất chứng minh.

Cần chú ý rằng một hàm *địa phương không đáng kể nhưng không không đáng kể* thì không khả tích; do đó, một hàm bằng *địa phương hầu khắp nơi* với một hàm khả tích không nhất thiết là khả tích.

#### Hệ quả 1 {#int-iv-s5-lem-1-cor-1 .statement}

*Để một tập hợp là khả tích, điều kiện cần và đủ là nó đo được và có độ đo ngoài hữu hạn.*

#### Hệ quả 2 {#int-iv-s5-lem-1-cor-2 .statement}

*Cho $(F_n)$ là một dãy các không gian tôpô; với mọi chỉ số n, gọi $f_n$ là một ánh xạ đo được từ X vào $F_n$ và đặt $f(x) = (f_n(x)) \in F = \prod_n F_n$; sau cùng, gọi u là một ánh xạ liên tục từ $f(X)$ vào một không gian Banach G. Để hàm $g(x) = u(f(x))$ khả tích, điều kiện cần và đủ là $N_1(g) < +\infty$.*

Thật vậy, g là đo được (No. 3, Định lý 1).

#### Hệ quả 3 {#int-iv-s5-lem-1-cor-3 .statement}

*Với mọi hàm khả tích f và mọi tập hợp đo được A, hàm $f \varphi_A$ là khả tích.*

Thật vậy, từ Định lý 5 và No. 3, Hệ quả 5 của Định lý 1 suy ra rằng $f \varphi_A$ là đo được, và $N_1(f \varphi_A) \leq N_1(f)$.

Ta viết $\int_A f d\mu = \int f \varphi_A d\mu$ (hoặc $\int_A f \mu$) với mọi hàm khả tích $f$ và mọi tập hợp đo được $A$. Ta cũng viết $\int^* f d|\mu|$ (hoặc $\int^*_A f |\mu|$) thay cho $\int^* f \varphi_A d|\mu|$ với mọi hàm số (hữu hạn hoặc không) $f \geqslant 0$ (đặt $f(x)\varphi_A(x) = 0$ nếu $f(x) = +\infty$ và $\varphi_A(x) = 0$).

#### Hệ quả 4 {#int-iv-s5-lem-1-cor-4 .statement}

*Với mọi dãy* $(f_n)$ *các hàm đo được* $\geqslant 0$ *trên* $X$,

$$
\int^*\left( \sum_n f_n \right) d|\mu| = \sum_n \int^* f_n d|\mu|.
$$

Xét theo §1, No. 3, Th. 3, ta quy về việc chứng minh rằng với mọi hai hàm đo được $f \geqslant 0, g \geqslant 0$ trên $X$,

$$
\int^*(f + g) d|\mu| = \int^* f d|\mu| + \int^* g d|\mu|.
$$

Điều này chỉ là tính cộng của tích phân khi $f$ và $g$ khả tích. Trong trường hợp ngược lại, nếu chẳng hạn $f$ không khả tích, thì $\int^* f d|\mu| = +\infty$ theo Th. 5; *a fortiori*, $\int^*(f + g) d|\mu| = +\infty$.

#### Hệ quả 5 {#int-iv-s5-lem-1-cor-5 .statement}

*Với mọi dãy* $(A_n)$ *gồm các tập hợp đo được rời nhau từng đôi một*,

$$
|\mu|^*\left( \bigcup_n A_n \right) = \sum_n |\mu|^*(A_n).
$$

Điều này suy ra từ Hệ quả 4 áp dụng cho các $\varphi_{A_n}$.

### 7. Độ đo cảm sinh trên một không gian con compact địa phương

Cho $X$ là một không gian compact địa phương, $\mu$ một độ đo trên $X$, và $Y$ là một *không gian con compact địa phương* của $X$. Vì $Y$ là giao của một tập hợp mở và một tập hợp đóng trong $X$ (GT, I, §9, No. 7, Mệnh đề 12), nên nó là $\mu$-đo được (No. 1, Hệ quả của Mệnh đề 3). Với mọi hàm $g \in \mathcal{H}(Y; \mathbf{C})$, gọi $g'$ là hàm, xác định trên toàn bộ $X$, bằng $g$ trên $Y$ và bằng 0 trên $X - Y$; ta sẽ chỉ ra rằng $g'$ là $\mu$-*khả tích*. Ta có thể hạn chế vào trường hợp $g$ là hàm thực và $\geqslant 0$ (viết $g$ như một tổ hợp tuyến tính của các hàm như vậy); vì $g'$ bị chặn và có giá compact, chỉ cần chỉ ra rằng $g'$ là $\mu$-đo được (No. 6, Th. 5); nhưng điều này suy ra từ việc $g'$ là nửa liên tục trên trên $X$ (No. 5, Hệ quả của Mệnh đề 8). Do đó ta có thể đưa ra định nghĩa sau đây:

#### Định nghĩa 4 {#int-iv-s5-def-4 .statement}

— *Cho Y là một không gian con compact địa phương của một không gian compact địa phương X, ta gọi độ đo cảm sinh trên Y bởi một độ đo $\mu$ trên X, và ký hiệu là $\mu_Y$ hoặc $\mu|Y$, là độ đo được xác định bởi công thức*

$$
\int g \, d\mu_Y = \int g' \, d\mu
$$

*đối với mọi hàm $g \in \mathcal{K}(Y; \mathbf{C})$, trong đó $g'$ ký hiệu hàm bằng $g$ trên $Y$ và bằng 0 trên $X - Y$.*

#### Ví dụ {#int-iv-s5-n7-exa-1 .statement}

— Cho $\mu$ là độ đo Lebesgue trên $\mathbf{R}$, I là *bất kỳ* khoảng nào trong $\mathbf{R}$; I là một không gian con compact địa phương của $\mathbf{R}$, và độ đo cảm sinh bởi $\mu$ trên I là dạng tuyến tính

$$
g \mapsto \int_a^b g(x) \, dx
$$

trên $\mathcal{K}(I; \mathbf{C})$, trong đó $a$ và $b$ là các đầu mút (hữu hạn hoặc không) của I (xem § 4, No. 4, *Ví dụ*), nói cách khác, chính là cái mà ta đã gọi là *độ đo Lebesgue trên I*.

Khi Y là một không gian con *mở* của X, Định nghĩa 4 trùng với định nghĩa của độ đo cảm sinh bởi $\mu$ trên Y (hay hạn chế của $\mu$ trên Y) đã cho trong Ch. III, §2, No. 1: thật vậy, với mọi hàm $g \in \mathcal{K}(Y; \mathbf{C})$ thì khi đó hàm $g'$ liên tục trên X.

Ta sẽ nghiên cứu chi tiết phép tích phân đối với một độ đo cảm sinh trong Ch. V, §7, và cho đến lúc đó ta sẽ chỉ cần những kết quả sau đây:

#### Bổ đề 2 {#int-iv-s5-lem-2 .statement}

— *Cho $\mu$ là một độ đo dương trên X, và cho K là một tập con compact của X.*

(i) *Với mọi tập con compact (resp. mở) H của K*, $\mu_K(H) = \mu(H)$.

(ii) *Để một tập con N của K là $\mu_K$-không đáng kể, điều kiện cần và đủ là nó $\mu$-không đáng kể*.

(iii) *Nếu S là giá của $\mu_K$, thì* $\mathrm{Supp}(\mu_S) = S$.

(i) Ta có thể hạn chế vào trường hợp H là compact. Ký hiệu bởi $f$ hàm đặc trưng của H trong không gian K; $f$ là nửa liên tục trên, do đó là bao dưới của một họ có hướng giảm $(g_\alpha)$ các hàm trong $\mathcal{K}_+(K)$; ta có $\mu_K(H) = \inf_\alpha \int g_\alpha \, d\mu_K$ (§ 4, No. 4, Hệ quả 2 của Mệnh đề 5). Nếu $g'_\alpha$ là hàm bằng $g_\alpha$ trên K và bằng 0 trên $X - K$, thì $g'_\alpha$ là nửa liên tục trên, và bao dưới của họ có hướng giảm $(g'_\alpha)$ là hàm đặc trưng $\varphi_H$ của H trong không gian X; do đó

$$
\mu(H) = \inf_\alpha \int g'_\alpha \, d\mu = \inf_\alpha \int g_\alpha \, d\mu_K = \mu_K(H)
$$

theo (1).

(ii) Nếu N là $\mu$-không đáng kể thì, với mọi $\varepsilon > 0$, tồn tại một lân cận mở tương đối compact U của N trong X sao cho $\mu(U) \leq \varepsilon$; vì $K - (U \cap K)$ là compact, từ (i) suy ra $\mu_K(U \cap K) \leq \mu(U) \leq \varepsilon$, vậy N là $\mu_K$-không đáng kể. Ngược lại, nếu N là $\mu_K$-không đáng kể thì tồn tại một lân cận mở V của N trong X sao cho $\mu_K(V \cap K) \leq \varepsilon$; theo (i), ta có $\mu(V \cap K) = \mu_K(V \cap K)$, do đó $\mu(N) = 0$ vì $\varepsilon$ là tùy ý.

(iii) Với mọi tập mở U trong K cắt S, theo giả thiết $\mu_K(U \cap S) \neq 0$, do đó $\mu(U \cap S) \neq 0$ theo (i), và vì $U \cap S$ là mở trong S, nên $\mu_S(U \cap S) \neq 0$ theo (i); vì mọi tập mở khác rỗng trong S đều có dạng $U \cap S$, trong đó U là mở trong K, điều này chứng tỏ rằng $\operatorname{Supp}(\mu_S) = S$.

#### Bổ đề 3 {#int-iv-s5-lem-3 .statement}

*Cho Y là một không gian con địa phương compact của X; với mọi độ đo $\mu$ trên X, $|\mu_Y| = |\mu|_Y$.*

Cho f là một hàm trong $\mathcal{K}_+(Y)$ và $\varepsilon$ là một số tùy ý $> 0$; theo định nghĩa, tồn tại một hàm $g \in \mathcal{K}(Y; \mathbf{C})$ sao cho $|g| \leq f$ và $|\mu_Y|(f) \leq |\mu_Y(g)| + \varepsilon$. Ký hiệu bởi $f'$ và $g'$ các hàm thu được bằng cách mở rộng tương ứng f và g thành 0 trên $X - Y$, ta có $\mu_Y(g) = \mu(g')$ và, vì $|g'| \leq f'$,

$$
|\mu(g')| \leq |\mu|(|g'|) \leq |\mu|(f') = |\mu|_Y(f),
$$

do đó $|\mu_Y|(f) \leq |\mu|_Y(f) + \varepsilon$ và, vì $\varepsilon$ là tùy ý,

$$
|\mu_Y|(f) \leq |\mu|_Y(f).
$$

Mặt khác, cho K là giá của f và cho U là một lân cận compact của K trong X sao cho $|\mu|(U - K) \leq \varepsilon$; theo định lý Urysohn, tồn tại một hàm $f_1 \in \mathcal{K}_+(X)$ mở rộng f, có giá được chứa trong U và sao cho $\|f_1\| = \|f\|$. Tồn tại một hàm $h_1 \in \mathcal{K}(X; \mathbf{C})$ sao cho $|h_1| \leq f_1$ và $|\mu|(f_1) \leq |\mu(h_1)| + \varepsilon$. Nếu h là hạn chế của $h_1$ lên Y, thì $h \in \mathcal{K}(Y; \mathbf{C})$, $|h| \leq f$ và $\mu(h_1) - \mu_Y(h) = \mu(h_1 \varphi_{U-K})$, do đó

$$
|\mu(h_1) - \mu_Y(h)| \leq \|f\| \cdot |\mu|(U - K) \leq \varepsilon \|f\|;
$$

hơn nữa, tương tự ta có

$$
|\mu|(f_1) - |\mu|_Y(f) = |\mu|(f_1 \varphi_{U-K}) \quad \text{và} \quad ||\mu|(f_1) - |\mu|_Y(f)|| \leq \varepsilon \|f\|.
$$

Từ đó ta suy ra rằng

$$
|\mu|_Y(f) \leq |\mu_Y(h)| + \varepsilon(1 + 2\|f\|) \leq |\mu_Y|(f) + \varepsilon(1 + 2\|f\|)
$$

và vì $\varepsilon$ là tùy ý, $|\mu|_Y(f) \leq |\mu_Y|(f)$, điều này hoàn tất chứng minh.

### 8. Các họ các tập compact $\mu$-trù mật

#### Mệnh đề 12 {#int-iv-s5-prop-12 .statement}

— Cho $\mu$ là một độ đo trên một không gian compact địa phương $X$, $A$ là một tập con $\mu$-đo được của $X$, và $\mathcal{K}$ là một tập hợp các tập con compact của $A$ thỏa mãn các điều kiện sau:
(PLI) Mọi tập con đóng (do đó compact) của một tập hợp thuộc $\mathcal{K}$ đều thuộc $\mathcal{K}$.
(PLII) Mọi hợp hữu hạn của các tập hợp thuộc $\mathcal{K}$ đều thuộc $\mathcal{K}$.
Khi đó bốn tính chất sau là tương đương:
a) Để một tập con $B$ của $A$ là địa phương $\mu$-không đáng kể, điều kiện cần và đủ là $|\mu|^*(B \cap K) = 0$ với mọi $K \in \mathcal{K}$.
b) Với mọi tập con compact $K_0$ của $A$ và mọi $\varepsilon > 0$, tồn tại một tập hợp $K \in \mathcal{K}$, được chứa trong $K_0$ và sao cho $|\mu|(K_0 - K) \leq \varepsilon$.
c) Với mọi tập con compact $B$ của $A$, tồn tại một phân hoạch của $B$ gồm một tập $\mu$-không đáng kể $N$ và một dãy $(H_n)$ các tập compact thuộc $\mathcal{K}$.
d) Với mọi tập con compact $B$ của $A$, tồn tại một dãy tăng $(K_n)$ các tập compact thuộc $\mathcal{K}$, được chứa trong $B$ và sao cho tập hợp $N = B - \bigcup_n K_n$ là $\mu$-không đáng kể.

Ngay lập tức (No. 2, Mệnh đề 5) ta có d) kéo theo $a); c)$ kéo theo d) khi lấy $K_n$ là hợp của các $H_p$ với $p \leq n$ và viện dẫn (PLII). Để chứng minh rằng b) kéo theo c), người ta xác định bằng quy nạp một dãy $(H_p)$ các tập hợp thuộc $\mathcal{K}$ sao cho $H_{n+1} \subset B - \bigcup_{p \leq n} H_p$ và $|\mu|(B - \bigcup_{p \leq n} H_p) \leq 1/n$ (§ 4, No. 6, Định lý 4).

Còn phải chứng minh rằng a) kéo theo b). Ta sẽ lập luận bằng phản chứng, và giả sử rằng cận trên $\alpha$ của các số $|\mu|(K)$, khi $K$ chạy qua tập hợp các tập con của $K_0$ thuộc $\mathcal{K}$, là $< |\mu|(K_0)$. Theo (PLII), tồn tại một dãy tăng $(L_n)$ các tập con compac của $K_0$, thuộc $\mathcal{K}$ và sao cho $\sup_n |\mu|(L_n) = \alpha$. Đặt $B = \bigcup_n L_n$; $B$ khả tích và $|\mu|(B) = \alpha$, do đó $|\mu|(K_0 - B) = |\mu|(K_0) - \alpha > 0$. Mặt khác, ta sẽ thấy rằng với mọi tập hợp $K \in \mathcal{K}$, ta có $|\mu|(K \cap (K_0 - B)) = 0$, điều này, chiếu theo a), sẽ dẫn đến mâu thuẫn. Thật vậy, nếu tồn tại một tập hợp $K \in \mathcal{K}$ sao cho $|\mu|(K \cap (K_0 - B)) > 0$, thì sẽ tồn tại một tập con compac $H$ của $K \cap (K_0 - B)$ sao cho $|\mu|(H) > 0$. Theo (PLI), ta sẽ có $H \in \mathcal{K}$, và, với $n$ đủ lớn,

$$
|\mu|(L_n \cup H) = |\mu|(L_n) + |\mu|(H) > \alpha .
$$

Nhưng $L_n \cup H$ thuộc $\mathcal{K}$ theo (PLII), và điều này mâu thuẫn với định nghĩa của $\alpha$.

#### Định nghĩa 6 {#int-iv-s5-def-6 .statement}

— Cho $A$ là một tập con $\mu$-đo được của $X$. Một tập hợp $\mathcal{K}$ các tập con compac của $A$ được gọi là $\mu$-trù mật trong $A$ nếu nó thỏa mãn các điều kiện (PLI), (PLII), $a), b), c), d)$ của Mệnh đề 12.

Tập hợp các tập con compac của $A$ là $\mu$-trù mật trong $A$.

Khi $A = X$, ta sẽ nói đơn giản ' tập hợp $\mu$-trù mật' thay cho 'tập hợp $\mu$-trù mật trong $X$'. Nếu $X - A$ địa phương $\mu$-không đáng kể, thì mọi tập hợp các tập con compac của $A$ mà $\mu$-trù mật trong $A$ cũng đều $\mu$-trù mật trong $X$.

#### Nhận xét {#int-iv-s5-n8-rem-1 .statement}

— Giả sử rằng $A$ là hợp của một dãy $(L_n)$ các tập compact và một tập hợp $\mu$-không đáng kể (resp. địa phương $\mu$-không đáng kể), và gọi $\mathcal{K}$ là một tập hợp các tập con compact $\mu$-trù mật trong $A$. Áp dụng cho mỗi $L_n$ tính chất *c*) của mệnh đề của Mệnh đề 12, ta thấy rằng $A$ là hợp của một dãy các tập compact *thuộc* $\mathcal{K}$ và một tập hợp $\mu$-không đáng kể (resp. địa phương $\mu$-không đáng kể).

Nếu $K$ là một tập con compact của $X$, thì nói rằng một tập hợp các tập con compact của $K$ là $\mu$-trù mật trong $K$ hay là nó $\mu_K$-*trù mật* trong $K$ cũng như nhau; điều này suy ra từ các Bổ đề 2 và 3 của No. 7 và điều kiện *b*) của Mệnh đề 12.

#### Mệnh đề 13 {#int-iv-s5-prop-13 .statement}

*Cho $A$ là một tập con $\mu$-đo được của $X$, $\mathcal{K}$ là một tập hợp các tập con compact $\mu$-trù mật trong $A$. Gọi $\mathfrak{H}$ là một tập hợp các tập con compact của $A$ thỏa mãn (PL$_I$) và (PL$_{II}$) và sao cho, với mọi $K \in \mathcal{K}$, tập hợp các $H \in \mathfrak{H}$ sao cho $H \subset K$ là $\mu_K$-*trù mật* (hay, điều này cũng tương đương, $\mu$-*trù mật*) trong $K$. Khi đó $\mathfrak{H}$ là $\mu$-trù mật trong $A$.*

Thật vậy, cho $L$ là một tập con compact của $A$. Với mọi $\varepsilon > 0$ tồn tại một $K \in \mathcal{K}$ sao cho $K \subset L$ và $|\mu|(L - K) \leq \varepsilon/2$, rồi tồn tại một $H \in \mathfrak{H}$ sao cho $H \subset K$ và $|\mu|(K - H) \leq \varepsilon/2$; suy ra $|\mu|(L - H) \leq \varepsilon$, do đó có mệnh đề.

### 9. Các phân hoạch đếm được địa phương

#### Định nghĩa 7 {#int-iv-s5-def-7 .statement}

*Một tập hợp $\mathfrak{A}$ các tập con của một không gian tôpô $T$ được gọi là *đếm được địa phương* nếu, với mọi $t \in T$, tồn tại một lân cận $V$ của $t$ sao cho tập hợp các $A \in \mathfrak{A}$ cắt $V$ là đếm được.*

Nếu tập hợp $\mathfrak{A}$ các tập con của $T$ là đếm được địa phương thì, với mọi tập con compact $K$ của $T$, tập hợp các $A \in \mathfrak{A}$ cắt $K$ là đếm được, vì $K$ có thể được phủ bởi một số hữu hạn lân cận mở của các điểm của $K$, mỗi lân cận trong số đó chỉ cắt một tập đếm được các tập con thuộc $\mathfrak{A}$.

Định nghĩa 7 cho thấy *hợp* của một tập đếm được địa phương các tập con $\mu$-đo được (tương ứng, địa phương $\mu$-không đáng kể) của một không gian compact địa phương là $\mu$-đo được (tương ứng, địa phương $\mu$-không đáng kể) (No. 1, Mệnh đề 3 và No. 2, Mệnh đề 5).

#### Mệnh đề 14 {#int-iv-s5-prop-14 .statement}

*Cho $X$ là một không gian compact địa phương, $\mu$ là một độ đo trên $X$, $A$ là một tập con $\mu$-đo được của $X$, và $\mathcal{K}$ là một tập hợp các tập con compact của $A$ mà $\mu$-trù mật trong $A$. Tồn tại một tập đếm được địa phương $\mathfrak{H} \subset \mathcal{K}$, gồm các tập đôi một rời nhau, sao cho $A - \bigcup_{K \in \mathfrak{H}} K$ là địa phương $\mu$-không đáng kể và sao cho, với mọi $K \in \mathfrak{H}$, giá của $\mu_K$ là toàn bộ $K$.*

Xét các tập hợp $\mathcal{L} \subset \mathfrak{K}$ gồm các tập đôi một rời nhau sao cho, với mọi $L \in \mathcal{L}$, $\operatorname{Supp}(\mu_L) = L$. Các tập hợp $\mathcal{L}$ tạo thành một tập con $\mathcal{H}$ của $\mathcal{P}(\mathfrak{K})$ khác rỗng (vì nó chứa phần tử $\varnothing$) và ta sẽ sắp thứ tự nó bởi quan hệ bao hàm trong $\mathcal{P}(\mathfrak{K})$. Ngay lập tức thấy rằng $\mathcal{H}$ là *quy nạp*; gọi $\mathfrak{H}$ là một phần tử cực đại của $\mathcal{H}$ (S, R, §6, No. 10). Trước hết, hãy chứng minh rằng $\mathfrak{H}$ là *đếm được địa phương*. Thật vậy, với mọi $x \in X$, gọi $V$ là một lân cận mở tương đối compact của $x$; nếu $(K_i)_{1 \leq i \leq n}$ là một họ hữu hạn các tập phân biệt của $\mathfrak{H}$ cắt $V$, thì

$$
\sum_{i=1}^n |\mu|(K_i \cap V) = |\mu|\left(V \cap \left( \bigcup_{i=1}^n K_i \right)\right)
$$

vì các $K_i$ đôi một rời nhau, do đó $\sum_{i=1}^n |\mu|(K_i \cap V) \leq |\mu|(V)$. Suy ra rằng nếu $\mathfrak{H}_V$ là tập hợp các $K \in \mathfrak{H}$ cắt $V$, thì

$$
\sum_{K \in \mathfrak{H}_V} |\mu|(K \cap V) < +\infty,
$$

và vì $|\mu|(K \cap V) > 0$ đối với mọi $K \in \mathfrak{H}_V$, nên $\mathfrak{H}_V$ tất yếu là đếm được. Tiếp theo, ta hãy chứng minh rằng $N = A - \bigcup_{K \in \mathfrak{H}} K$ là địa phương $\mu$-không đáng kể. Ta đã thấy ở trên rằng $N$ là $\mu$-đo được. Nếu $N$ không địa phương không đáng kể, thì nó sẽ chứa một tập compact không đáng kể $L_0$, do đó (No. 8, Mệnh đề 12) một tập compact không đáng kể $L \subset L_0$ thuộc $\mathfrak{K}$. Vì $|\mu_L|(L) = |\mu|(L) > 0$ (No. 7, Bổ đề 2 và 3), độ đo $\mu_L$ cảm sinh trên $L$ bởi $\mu$ là khác không; do đó giá của nó là một tập compact khác rỗng $S$ thuộc $\mathfrak{K}$ theo (PL₁), và $\operatorname{Supp}(\mu_S) = S$ (No. 7, Bổ đề 2, (iii)). Suy ra tập hợp $\mathfrak{H} \cup \{S\}$ thuộc $\mathcal{H}$, điều này mâu thuẫn với định nghĩa của $\mathfrak{H}$; do đó tập $N$ là địa phương không đáng kể, điều này hoàn tất chứng minh.

### 10. Các ánh xạ đo được xác định trên một tập con đo được

#### Mệnh đề 15 {#int-iv-s5-prop-15 .statement}

*Cho $X$ là một không gian compact địa phương, $\mu$ một độ đo trên $X$, $A$ một tập con $\mu$-đo được của $X$, và $f$ một ánh xạ từ $A$ vào một không gian tôpô $F$. Các điều kiện sau là tương đương:

a) Tập $\mathfrak{H}$ các tập compact $K$ của $A$ sao cho hạn chế của $f$ trên $K$ là liên tục, là $\mu$-trù mật trong $A$.

b) Tồn tại một tập hợp $\mathfrak{K}$ các tập compact của $A$, $\mu$-trù mật trong $A$, sao cho hạn chế của $f$ trên mọi $K \in \mathfrak{K}$ là $\mu_K$-đo được.

c) Tồn tại một đồng phôi $j$ của $F$ lên một không gian con của một không gian tôpô $G$ và một ánh xạ $\mu$-đo được $g$ từ $X$ vào $G$, sao cho $g|A = j \circ f$.*

d) Mọi mở rộng của $f$ thành một ánh xạ từ $X$ vào $F$, hằng trên $X - A$, đều là $\mu$-đo được.

Hiển nhiên rằng a) suy ra b) và d) suy ra c). Việc c) suy ra a) là hệ quả của điều kiện c) của Mệnh đề 12 ở No. 8. Mặt khác, b) suy ra a): thật vậy, Định nghĩa 1 cho thấy rằng, với mỗi $K \in \mathcal{K}$, tập hợp các tập con $H \in \mathcal{H}$ được chứa trong $K$ là $\mu_K$-trù mật trong $K$ (No. 8, Mệnh đề 12, c)), và Mệnh đề 13 của No. 8 cho thấy rằng $\mathcal{H}$ là $\mu$-trù mật trong $A$. Còn lại phải thấy rằng a) suy ra d). Gọi $g$ là một mở rộng của $f$ lên $X$, hằng trên $X - A$. Với mọi tập con compact $L$ của $X$, $L \cap A$ và $L \cap (X - A)$ là $\mu$-khả tích; do đó, với mọi $\varepsilon > 0$, tồn tại một tập con compact $P \subset L \cap A$ và một tập con compact $Q \subset L \cap (X - A)$ sao cho

$$
|\mu|((L \cap A) - P) \leq \varepsilon/4 \quad \text{và} \quad |\mu|\left((L \cap (X - A)) - Q\right) \leq \varepsilon/4.
$$

Mặt khác, tồn tại một tập hợp $H \in \mathcal{H}$ được chứa trong $P$ sao cho $|\mu|(P - H) \leq \varepsilon/2$; khi đó hạn chế của $g$ lên tập compact $K = H \cup Q$ là liên tục ($g$ hằng trên $Q$) và $|\mu|(L - K) \leq \varepsilon$, điều này hoàn tất chứng minh.

#### Định nghĩa 8 {#int-iv-s5-def-8 .statement}

*Cho $X$ là một không gian compact địa phương, $\mu$ là một độ đo trên $X$, và $A$ là một tập con $\mu$-đo được của $X$. Một ánh xạ $f$ từ $A$ vào một không gian tôpô $F$ được gọi là $\mu$-đo được nếu nó thỏa mãn các điều kiện tương đương của Mệnh đề 15.*

Nếu $A$ là địa phương $\mu$-không đáng kể, thì *mọi* ánh xạ từ $A$ vào $F$ do đó đều là $\mu$-đo được.

#### Hệ quả 1 {#int-iv-s5-def-8-cor-1 .statement}

*Cho $X$ là một không gian compact địa phương, $\mu$ là một độ đo trên $X$, $A$ là một tập con $\mu$-đo được của $X$, và $f$ là một ánh xạ $\mu$-đo được từ $A$ vào một không gian tôpô $F$. Cho $\mathcal{K}$ là một tập hợp các tập con compact của $X$, $\mu$-trù mật trong $X$. Khi đó, tồn tại một phân hoạch của $A$ gồm một tập địa phương không đáng kể $N$ và một họ đếm được địa phương $(K_\lambda)_{\lambda \in L}$ các tập hợp $K_\lambda \in \mathcal{K}$, sao cho $f|K_\lambda$ liên tục với mọi $\lambda \in L$.

Theo No. 9, Mệnh đề 14, chỉ cần chứng minh rằng tập hợp $\mathcal{H} \subset \mathcal{K}$ các tập con $K \in \mathcal{K}$ sao cho $K \subset A$ và $f|K$ liên tục, là $\mu$-trù mật trong $A$. Bây giờ, suy ra ngay từ Mệnh đề 1 của No. 1 và điều kiện d) của Mệnh đề 15 rằng, với mọi tập con compact $K_0$ của $A$ và mọi $\varepsilon > 0$, tồn tại một tập con $K \subset K_0$ thuộc $\mathcal{K}$ sao cho $|\mu|(K_0 - K) \leq \varepsilon$ và $f|K$ liên tục; do đó kết luận suy ra từ Mệnh đề 12 của No. 8.

#### Hệ quả 2 {#int-iv-s5-def-8-cor-2 .statement}

*Cho $K$ là một không gian con compact của $X$; để một ánh xạ $f$ từ $K$ vào một không gian tôpô $F$ là $\mu$-đo được, điều cần và đủ là nó $\mu_K$-đo được.*

Theo Bổ đề 2 của No. 7, điều này suy ra ngay từ Mệnh đề 1 của No. 1 và điều kiện a) của Mệnh đề 15.

#### Mệnh đề 16 {#int-iv-s5-prop-16 .statement}

*Cho $\mathfrak{A}$ là một tập hợp đếm được địa phương các tập con $\mu$-đo được của $X$ và đặt $B = \bigcup_{A \in \mathfrak{A}} A$. Để một ánh xạ $f$ từ $B$ vào một không gian tôpô $F$ là $\mu$-đo được, điều cần và đủ là hạn chế của $f$ trên mọi $A \in \mathfrak{A}$ là $\mu$-đo được.*

Ta đã nhận thấy (No. 9) rằng $B$ là $\mu$-đo được. Điều kiện này hiển nhiên là cần thiết; ta hãy chứng minh rằng nó là đủ. Vậy, cho $K$ là một tập con compắc của $B$. Theo giả thiết, tồn tại một dãy $(A_n)$ các tập hợp thuộc $\mathfrak{A}$ sao cho các $K \cap A_n$ tạo thành một phủ của $K$. Đặt $C_0 = K \cap A_0$ và
$$
C_n = K \cap A_n \cap \mathbf{C}\left( \bigcup_{i < n} C_i \right)
$$
với $n > 0$, sao cho các $C_n$ khác rỗng tạo thành một phân hoạch của $K$ thành các tập hợp $\mu$-khả tích. Vì hạn chế của $f$ lên $C_n$ là $\mu$-đo được, tồn tại một phân hoạch của $C_n$ gồm một tập hợp $\mu$-không đáng kể $N_n$ và một dãy $(L_{mn})_{m \geq 0}$ các tập hợp compắc sao cho $f|L_{mn}$ liên tục. Vì $N = \bigcup_n N_n$ là $\mu$-không đáng kể, ta thấy rằng điều kiện a) của Mệnh đề 15 được thỏa mãn, do đó mệnh đề được chứng minh.

Tính chất d) của Mệnh đề 15 cho phép tổng quát hóa ngay lập tức các tính chất của các hàm đo được xác định trên toàn bộ $X$, đã được nhận thấy trong Nos. 2 đến 5, cho các hàm đo được xác định trên một tập con đo được $A$ của $X$; các tổng quát hóa này được để lại cho người đọc. Ta chỉ chỉ ra tường minh rằng nguyên lý địa phương hóa (No. 2, Mệnh đề 4) vẫn còn đúng khi giả sử rằng mỗi hàm $g_x$ chỉ được xác định trong $V_x$ (hoặc hầu khắp nơi trong $V_x$) và là đo được.

### 11. Hội tụ theo độ đo

Cho $X$ là một không gian địa phương compact, $\mu$ là một độ đo trên $X$, $A$ là một tập con $\mu$-đo được của $X$, và $F$ là một *không gian đều*; ta sẽ ký hiệu bởi $\mathcal{S}(A, \mu; F)$, hoặc $\mathcal{S}_F(A, \mu)$ (hoặc đơn giản là $\mathcal{S}_F(\mu)$, hoặc thậm chí $\mathcal{S}_F$, khi $A = X$) tập hợp các *ánh xạ $\mu$-đo được từ $A$ vào $F$* (No. 10, Def. 8). Với mọi lân cận đều $V$ của cấu trúc đều của $F$, mọi tập hợp $\mu$-khả tích $B \subset A$ và mọi số $\delta > 0$, ta sẽ ký hiệu bởi $W(V, B, \delta)$ tập hợp các cặp $(f, g)$ gồm các hàm trong $\mathcal{S}(A, \mu; F)$ có tính chất sau: tập hợp $M$ của mọi $x \in B$ sao cho $(f(x), g(x)) \notin V$ là sao cho $|\mu|^*(M) \leq \delta$. Hãy chứng minh rằng các tập hợp $W(V, B, \delta)$ tạo thành một *hệ cơ bản các lân cận đều* của một cấu trúc đều trên $\mathcal{S}(A, \mu; F)$: hiển nhiên là $W(V, B, \delta)$ là đối xứng nếu $V$ đối xứng, và nếu $V' \subset V,\ B' \supset B$ và $\delta' \leq \delta$, thì

$$
W(V', B', \delta') \subset W(V, B, \delta);
$$

do đó chỉ cần kiểm tra tiên đề $(U'_{III})$ (GT, II, §1, No. 1). Bây giờ, nếu $V'$ là một lân cận đều sao cho ${V'}^2 \subset V$, thì

$$
W(V', B, \delta/2) \circ W(V', B, \delta/2) \subset W(V, B, \delta).
$$

Chú ý rằng khi $K$ chạy qua một hệ $\mu$-trù mật $\mathfrak{K}$ các tập con *compact* của $A$, thì các tập hợp $W(V, K, \delta)$ cũng tạo thành một hệ cơ bản các lân cận đều cho cấu trúc đều nói trên: thật vậy, với mọi tập hợp khả tích $B \subset A$, tồn tại một tập compact $K \in \mathfrak{K}$ được chứa trong $B$ sao cho $|\mu|(B - K) \leq \delta$, và do đó $W(V, K, \delta) \subset W(V, B, 2\delta)$.

#### Định nghĩa 9 {#int-iv-s5-def-9 .statement}

*Cấu trúc đều trên $\mathcal{S}(A, \mu; F)$ mà trong đó các $W(V, B, \delta)$ tạo thành một hệ cơ bản các lân cận đều được gọi là cấu trúc đều của sự hội tụ theo độ đo trong $A$.*.

Tôpô tương ứng được gọi là *tôpô của sự hội tụ theo độ đo trong $A$*, và một bộ lọc (hoặc một dãy) hội tụ theo tôpô này được gọi là *hội tụ theo độ đo trong $A$*; việc nhắc đến $A$ thường được lược bỏ khi $A = X$.

Giả sử $F$ là *Hausdorff*; khi đó, với mọi tập $B \subset A$ là $\mu$-khả tích, giao của các lân cận $W(V, B, \delta)$, trong đó $V$ chạy qua một hệ cơ bản các lân cận của $F$ và $\delta$ chạy qua tập các số $> 0$, là tập các cặp $(f, g)$ sao cho $f(x) = g(x)$ *hầu khắp trên $B$* (*đối với $\mu$*). Thật vậy, tập $M$ gồm các $x \in B$ sao cho $f(x) \neq g(x)$ là $\mu$-khả tích, vì nó là ảnh ngược, qua ánh xạ $\mu$-đo được $x \mapsto (f(x), g(x))$, của phần bù của đường chéo trong $F \times F$, là một tập mở (No. 5, Mệnh đề 7); nếu $|\mu|(M) = \alpha > 0$, tồn tại một tập con compact $K \subset M$ sao cho $|\mu|(M - K) < \alpha/2$ và sao cho các hạn chế của $f$ và $g$ trên $K$ là liên tục; do đó, tồn tại một lân cận $V_0$ của $F$ sao cho $(f(x), g(x)) \notin V_0$ với mọi $x \in K$, do đó $(f, g) \notin W(V_0, B, \alpha/2)$.

Từ đó suy ra rằng nếu $F$ là Hausdorff, thì giao của *mọi* lân cận của $\mathcal{S}(A, \mu; F)$ là tập các cặp $(f, g)$ sao cho $f(x) = g(x)$ *hầu khắp địa phương trên $A$*. Vậy không gian đều Hausdorff liên kết với $\mathcal{S}(A, \mu; F)$, mà ta sẽ ký hiệu là $S(A, \mu; F)$ hoặc $S_F(A, \mu)$ (hoặc cả $S_F(\mu)$ hay $S_F$ khi $A = X$), do đó gồm các *lớp tương đương* đối với quan hệ « $f(x) = g(x)$ hầu khắp địa phương trên $A$ » trong tập $\mathcal{S}(A, \mu; F)$.

#### Mệnh đề 17 {#int-iv-s5-prop-17 .statement}

— Cho $(A_\lambda)_{\lambda \in L}$ là một họ đếm được địa phương các tập con $\mu$-đo được của $A$, rời nhau từng đôi một và sao cho $A - \bigcup_{\lambda \in L} A_\lambda$ là $\mu$-không đáng kể địa phương. Nếu, với mọi lớp $f \in S(A, \mu; F)$ và mọi $\lambda \in L$, $f_\lambda$ ký hiệu lớp của hạn chế trên $A_\lambda$ của một hàm bất kỳ trong lớp $f$, thì ánh xạ $\psi : f \mapsto (f_\lambda)_{\lambda \in L}$ là một đẳng cấu của không gian đều $S(A, \mu; F)$ lên không gian đều tích $\prod_{\lambda \in L} S(A_\lambda, \mu; F)$.

Từ No. 10, Mệnh đề 16 suy ra rằng $\psi$ là song ánh. Xét một lân cận $T$ của $S(A, \mu; F)$ là ảnh chính tắc của một $W(V, B, \delta)$, trong đó $B$ là một tập con compact của $A$; ta biết rằng tập hợp $J$ các $\lambda \in L$ sao cho $B \cap A_\lambda \neq \varnothing$ là đếm được (No. 9), và $|\mu|(B) = \sum_{\lambda \in J} |\mu|(B \cap A_\lambda)$; do đó, tồn tại một tập con hữu hạn $H$ của $J$ sao cho

$$
\sum_{\lambda \in J - H} |\mu|(B \cap A_\lambda) \leq \frac{\delta}{2}.
$$

Ảnh của $T$ dưới $\psi \times \psi$ khi đó được chứa trong ảnh chính tắc của tích $\prod_{\lambda \in H} W(V, B \cap A_\lambda, \delta)$. Mặt khác, nếu $m$ là số phần tử của $H$, thì ảnh của $T$ dưới $\psi \times \psi$ chứa ảnh chính tắc của lân cận $\prod_{\lambda \in H} W(V, A_\lambda, \delta/2m)$, điều này chứng minh mệnh đề.

#### Mệnh đề 18 {#int-iv-s5-prop-18 .statement}

— *Nếu $F$ khả mêtric, và $A$ là hợp của một tập hợp địa phương $\mu$-không đáng kể và một dãy $(A_n)$ các tập hợp $\mu$-khả tích, thì không gian $S(A, \mu; F)$ là khả mêtric.*

Vì mỗi $A_n$ là hợp của một tập hợp không đáng kể và một dãy các tập compact, ta có thể giả sử rằng các $A_n$ đã là *compact* và từng đôi một rời nhau. Khi đó Mệnh đề 17 cho phép ta giả sử rằng $A$ là compact. Nếu $(V_n)$ là một hệ cơ bản đếm được các lân cận của $F$, thì hiển nhiên các $W(V_n, A, 1/n)$ tạo thành một hệ cơ bản các lân cận của $S(A, \mu; F)$ khi $n$ chạy qua $\mathbf{N}$, do đó suy ra mệnh đề.

#### Bổ đề 4 {#int-iv-s5-lem-4 .statement}

— *Cho $F$ là một không gian đều khả mêtric, và cho $B \subset A$ là một hợp đếm được của các tập hợp $\mu$-khả tích. Khi đó, với mọi dãy Cauchy $(f_n)$ trong $S(A, \mu; F)$, tồn tại một dãy con $(f_{n_k})$ của $(f_n)$ sao cho $(f_{n_k}(x))$ là một dãy Cauchy trong $F$ với hầu khắp mọi $x \in B$.*

Trước hết giả sử rằng $B$ là khả tích, và ký hiệu bởi $d$ một mêtric tương thích với cấu trúc đều của $F$. Ta sẽ định nghĩa đệ quy một dãy kép $(f_{mn})$ các hàm trong $S(A, \mu; F)$ sao cho $f_{0n} = f_n$ với mọi $n$, $(f_{mn})_{n \geq 0}$ là một dãy con của $(f_{m-1,n})_{n \geq 0}$ với mọi $m > 0$ và, sau cùng, sao cho với mọi $m > 0$ tập hợp $M_{mn}$ các $x \in B$ mà với chúng $d(f_{mn}(x), f_{m,n+1}(x)) > 1/2^{m+n+1}$ có độ đo $|\mu|(M_{mn}) \leq 1/2^{m+n+1}$;

khả năng thực hiện được định nghĩa như vậy suy ra từ việc $(f_n)$ là một dãy Cauchy trong $\mathcal{S}(A, \mu; F)$. Đặt $M_m = \bigcup_{n \geq 0} M_{mn}$; khi đó

$$
|\mu|(M_m) \leq \sum_{n=0}^{\infty} |\mu|(M_{mn}) \leq 1/2^m
$$

và, với mọi $x \in B - M_m$, ta có $d(f_{mn}(x), f_{m,n+p}(x)) \leq 1/2^{m+n}$ với mọi $n \geq 0$ và mọi $p > 0$; do đó dãy $(f_{mn}(x))_{n \geq 0}$ là một dãy Cauchy trong $F$. Bây giờ đặt $N = \bigcap_{m=0}^{\infty} M_m$; $N$ là không đáng kể. Đặt $g_n = f_{nn}$ với mọi $n \geq 0$; với mọi $m$, dãy $(g_n)_{n \geq m}$ là một dãy con của dãy $(f_{mn})_{n \geq 0}$; nếu $x \in B - N$, tồn tại một chỉ số $m$ sao cho $x \notin M_m$, điều đó chứng tỏ rằng dãy $(g_n(x))$ là một dãy Cauchy trong $F$.

Nếu bây giờ $B$ là hợp của một dãy $(B_m)$ các tập hợp khả tích, ta có thể định nghĩa đệ quy một dãy kép $(g_{mn})$ sao cho $g_{0n} = f_n$, $(g_{mn})_{n \geq 0}$ là một dãy con của $(g_{m-1,n})_{n \geq 0}$ với mọi $m > 0$, và sao cho dãy $(g_{mn}(x))_{n \geq 0}$ là một dãy Cauchy trong $B_m - P_m$, trong đó $P_m$ là không đáng kể. Đặt $h_n = g_{nn}$ với mọi $n \geq 0$, để rồi, với mọi $m$, dãy $(h_n)_{n \geq m}$ là một dãy con của $(g_{mn})_{n \geq 0}$; khi đó dãy $(h_n(x))_{n \geq 0}$ là một dãy Cauchy trong $F$ với mọi $x \in B - P$, trong đó $P = \bigcup_{m=0}^{\infty} P_m$ là không đáng kể.

#### Mệnh đề 19 {#int-iv-s5-prop-19 .statement}

*Nếu không gian đều $F$ là mêtrizable và đầy đủ, thì không gian đều $S(A, \mu; F)$ là đầy đủ.*

Tồn tại một họ địa phương đếm được $(K_{\lambda})_{\lambda \in L}$ các tập con compact của $A$ sao cho các $K_{\lambda}$ rời nhau từng đôi một và $A - \bigcup_{\lambda} K_{\lambda}$ là địa phương không đáng kể (No. 9, Mệnh đề 14). Theo Mệnh đề 17, $S(A, \mu; F)$ đẳng cấu với tích $\prod_{\lambda \in L} S(K_{\lambda}, \mu; F)$; do đó ta được đưa về việc chứng minh mệnh đề khi $A$ là *khả tích*; khi đó $S(A, \mu; F)$ có thể mêtric hóa (Mệnh đề 18) và, theo Bổ đề 4, với mọi dãy Cauchy $(f_n)$ trong $\mathcal{S}(A, \mu; F)$ tồn tại một dãy con $(f_{n_k})$ hội tụ trong $A - N$, ở đây $N$ là không đáng kể; khi đó giới hạn $f$ của $(f_{n_k})$ (được mở rộng theo một cách bất kỳ ra toàn bộ $A$) là $\mu$-đo được, và từ sự mở rộng của định lý Egoroff đã nhắc đến trong No. 10 suy ra rằng dãy $(f_{n_k})$ *hội tụ theo độ đo* tới $f$ trong $A$. Điều đó kéo theo $f$ là một điểm tụ của dãy $(f_n)$ trong $\mathcal{S}(A, \mu; F)$, và vì dãy $(f_n)$ theo giả thiết là một dãy Cauchy, nó hội tụ tới $f$.

Q.E.D.

#### Hệ quả {#int-iv-s5-n11-cor-1 .statement}

— Cho F là một không gian đều có thể mêtric hóa.

(i) Mọi dãy $(f_n)$ các phần tử của $\mathcal{S}(A, \mu; F)$ hội tụ hầu khắp địa phương tới một ánh xạ $f$ (tất yếu là $\mu$-đo được) từ A vào F, đều hội tụ theo độ đo tới $f$ trong A.

(ii) Cho $(f_n)$ là một dãy các phần tử của $\mathcal{S}(A, \mu; F)$ hội tụ theo độ đo tới một ánh xạ $f$ từ A vào F. Với mọi tập hợp $B \subset A$ là một hợp đếm được của các tập khả tích, tồn tại một dãy con $(f_{n_k})$ của $(f_n)$ sao cho dãy $(f_{n_k}(x))$ hội tụ trong F tới $f(x)$ với hầu hết mọi $x \in B$.

(i) Mệnh đề được suy ra ngay từ sự mở rộng của định lý Egoroff đã nhắc đến trong No. 10.

(ii) Theo Bổ đề 4, tồn tại một dãy con $(f_{n_k})$ của $(f_n)$ sao cho $(f_{n_k}(x))$ là một dãy Cauchy trong F với mọi $x \in B - N$, ở đây N là không đáng kể; gọi $f'(x) \in \widehat{F}$ là giới hạn của dãy này với $x \in B - N$. Hiển nhiên $f'$ là một ánh xạ $\mu$-đo được từ $B - N$ vào $\widehat{F}$, và dãy $(f_n)$ hội tụ theo độ đo tới $f'$ trong $B - N$ theo (i); do đó $f'$ bằng $f$ hầu khắp trong B.

#### Mệnh đề 20 {#int-iv-s5-prop-20 .statement}

— Cho F là một không gian Banach, được trang bị cấu trúc đều xác định bởi chuẩn của nó.

(i) Với mọi tập con $\mu$-đo được A của X, tôpô của sự hội tụ theo độ đo tương thích với cấu trúc không gian vectơ của $\mathcal{S}(A, \mu; F)$.

(ii) Không gian $\mathcal{K}(X; F)$ trù mật trong $\mathcal{S}(X, \mu; F)$.

(iii) Với mọi số thực $p \geq 1$, tôpô cảm sinh trên không gian $\mathcal{L}_F^p(X, \mu)$ bởi tôpô hội tụ theo độ đo là thô hơn tôpô hội tụ trung bình cấp $p$.

(i) Với mọi tập con B của A khả tích đối với $\mu$ và mọi $\delta > 0$, ký hiệu bởi $T(B, \delta)$ tập hợp các $f \in \mathcal{S}(A, \mu; F)$ mà đối với chúng tập C các $x \in B$ sao cho $|f(x)| \geq \delta$ thỏa mãn quan hệ $|\mu|(C) \leq \delta$; hiển nhiên rằng nếu $V_\delta$ là lân cận của F gồm các cặp $(y, z)$ sao cho $|y - z| \leq \delta$, thì lân cận $W(V_\delta, B, \delta)$ là tập hợp các cặp $(f, g)$ của các ánh xạ đo được từ A vào F sao cho $f - g \in T(B, \delta)$. Hiển nhiên rằng các tập hợp $T(B, \delta)$ là đối xứng, và rằng $T(B, \delta) + T(B, \delta) \subset T(B, 2\delta)$ và $T(B, |\alpha|\delta) \subset \alpha T(B, \delta)$ với mọi vô hướng khác không $\alpha$ sao cho $|\alpha| \leq 1$; do đó chỉ cần kiểm tra rằng các tập hợp $T(B, \delta)$ là hút được (TVS, I, §1, No. 5, Prop. 4). Bây giờ, nếu $f$ là một ánh xạ $\mu$-đo được từ A vào F, thì hàm số $|f|$ cũng là $\mu$-đo được (No. 3, Cor. 6 of Th. 1). Gọi $C_n$ là tập hợp các $x \in B$ sao cho $|f(x)| \geq n$; các $C_n$ lập thành một dãy giảm các tập hợp khả tích mà giao là rỗng; do đó tồn tại một số nguyên $n$ sao cho $|\mu|(C_n) \leq \delta$ (§ 4, No. 5, Cor. of Prop. 7); hơn nữa ta có thể giả sử rằng $n$ được chọn đủ lớn để $1/n \leq \delta$; khi đó $f/n^2 \in T(B, \delta)$, điều này hoàn tất chứng minh mệnh đề (i).

(iii) Quan hệ $\int |f|^p d|\mu| \leq \delta^{p+1}$ kéo theo rằng nếu $C$ là tập hợp các $x \in X$ sao cho $|f(x)| \geq \delta$, thì

$$
\delta^p |\mu|^*(C) \leq \int |f|^p d|\mu| \leq \delta^{p+1},
$$

do đó $|\mu|^*(C) \leq \delta$, điều này chứng minh (iii).

(ii) Theo (iii), chẳng hạn chỉ cần chỉ ra rằng $\mathcal{L}_F^1$ trù mật trong $\mathcal{S}_F$, vì theo định nghĩa $\mathcal{H}(X; F)$ là trù mật trong $\mathcal{L}_F^1$ đối với tôpô hội tụ trung bình. Bây giờ, gọi $f$ là một phần tử bất kỳ của $\mathcal{S}_F$ và $T(B, \delta)$ là một lân cận của 0 trong không gian này; ta thấy như trong (i) rằng tồn tại một tập con khả tích $C$ của $B$ sao cho $|\mu|(C) \leq \delta$ và sao cho $f$ là *bị chặn* trên $B - C$; khi đó ký hiệu bởi $g$ hàm bằng $f$ trên $B - C$ và bằng 0 trên $X - (B - C)$, suy ra từ No. 6, Th. 5 rằng $g$ là khả tích, và hiển nhiên $f - g \in T(B, \delta)$.

#### Nhận xét {#int-iv-s5-n11-rem-1 .statement}

— 1) Không gian vectơ tôpô $\mathcal{S}(X, \mu; F)$ không nhất thiết lồi địa phương (Bài tập 24).
2) Tôpô cảm sinh trên tập hợp các $f$ sao cho $N_p(f) \leq 1$ bởi tôpô hội tụ theo độ đo có thể thực sự thô hơn tôpô cảm sinh trên tập hợp này bởi tôpô hội tụ trong trung bình cấp $p$ (Bài tập 22). Tuy nhiên, xem Mệnh đề 21 dưới đây.

#### Định nghĩa 10 {#int-iv-s5-def-10 .statement}

*Cho $X$ là một không gian địa phương compact, $\mu$ là một độ đo trên $X$, $F$ là một không gian Banach, và $p \in [1, +\infty[$. Một tập con $H$ của $\mathcal{L}_F^p(X, \mu)$ được gọi là đồng khả tích cấp $p$ (đối với $\mu$) nếu nó thỏa mãn các điều kiện sau:*

(i) *Với mọi $\varepsilon > 0$ tồn tại một $\delta > 0$ sao cho, với mọi tập khả tích $A$ có độ đo $|\mu|(A) \leq \delta$ và mọi $f \in H$,*

$$
\int |f|^p \varphi_A d|\mu| \leq \varepsilon.
$$

(ii) *Với mọi $\varepsilon > 0$ tồn tại một tập con compact $K$ của $X$ sao cho, với mọi $f \in H$,* $\int |f|^p \varphi_{X-K} d|\mu| \leq \varepsilon$.

Khi $p = 1$ ta nói 'đồng khả tích' thay cho 'đồng khả tích cấp 1'.

#### Nhận xét {#int-iv-s5-n11-rem-2 .statement}

— Giả sử $\mu$ bị chặn. Với mọi $a > 0$, tập hợp các ánh xạ đo được từ $X$ vào $F$ sao cho $|f(x)| \leq a$ hầu khắp nơi là đồng khả tích cấp $p$, và điều này đúng với mọi $p \in [1, +\infty[$.

#### Mệnh đề 21 {#int-iv-s5-prop-21 .statement}

*Cho $H$ là một tập con của $\mathcal{L}_F^p(X, \mu)$ đồng khả tích cấp $p$. Trên $H$, cấu trúc đều của hội tụ theo độ đo bằng cấu trúc đều cảm sinh bởi cấu trúc đều của $\mathcal{L}_F^p(X, \mu)$.*

Cho $\varepsilon > 0$. Tồn tại $\delta$ và $K$ có các tính chất (i) và (ii) của Định nghĩa 10. Cho $f, g$ trong $H$ sao cho

$$
|f(x) - g(x)| \leq \left( \frac{\varepsilon}{|\mu|(K)} \right)^{1/p}
$$

với $x \in K$, trừ trên một tập $M$ có độ đo $\leq \delta$. Khi đó

$$
\left( \int_{X-K} |f-g|^p d|\mu| \right)^{1/p} \leq \left( \int_{X-K} |f|^p d|\mu| \right)^{1/p} + \left( \int_{X-K} |g|^p d|\mu| \right)^{1/p}
$$
$$
\leq 2\varepsilon^{1/p}
$$

và tương tự
$$
\left( \int_M |f-g|^p d|\mu| \right)^{1/p} \leq 2\varepsilon^{1/p},
$$
do đó
$$
\int |f-g|^p d|\mu| = \int_{X-K} |f-g|^p d|\mu| + \int_M |f-g|^p d|\mu| + \int_{K-M} |f-g|^p d|\mu|
$$
$$
\leq 2^p \varepsilon + 2^p \varepsilon + \frac{\varepsilon}{|\mu|(K)} |\mu|(K-M) \leq (2^{p+1} + 1)\varepsilon.
$$

Vậy, cấu trúc đều của hội tụ theo độ đo trên $H$ mịn hơn cấu trúc đều cảm sinh bởi cấu trúc đều của $\mathcal{L}_F^p(X, \mu)$. Khi đó chỉ cần áp dụng Mệnh đề 20.

### 12. Một tính chất của hội tụ mơ hồ

#### Bổ đề 5 {#int-iv-s5-lem-5 .statement}

*Cho $X$ là một không gian địa phương compact, $\mu$ là một độ đo dương bị chặn trên $X$, $F$ là một không gian Banach, và $f$ là một hàm bị chặn trên $X$ nhận giá trị trong $F$. Các điều kiện sau là tương đương:*

(i) *Tập hợp các điểm gián đoạn của $f$ là $\mu$-không đáng kể.*

(ii) *Với mọi $\varepsilon > 0$, tồn tại các phần tử $a_1, \ldots, a_n$ của $F$, các hàm $g_1, \ldots, g_n$ thuộc $\mathscr{K}(X)$, và một hàm liên tục bị chặn $h \geq 0$ trên $X$ sao cho $|f - g_1 a_1 - \cdots - g_n a_n| \leq h \leq 2 \sup |f|$ trên $X$, và $\int h d\mu \leq \varepsilon$.*

Ký hiệu $N$ là tập hợp các điểm gián đoạn của $f$, và đặt $M = \sup |f|$.

(i) $\Rightarrow$ (ii). Giả sử điều kiện (i) được thỏa mãn. Cho $\varepsilon > 0$. Hàm $f$ là $\mu$-khả tích (No. 2, Hệ quả 4 của Mệnh đề 5, và No. 6, Định lý 5), do đó tồn tại $a_1, \ldots, a_n$ trong $F$ và $g_1, \ldots, g_n$ trong $\mathscr{K}(X)$ sao cho, khi đặt $k = |f - g_1 a_1 - \cdots - g_n a_n|$, ta có $\int k d\mu \leq \varepsilon/2$ (§ 3, No. 5,

Mệnh đề 10). Nhân $g_1, \ldots, g_n$ với cùng một phần tử thích hợp của $\mathcal{K}(X)$, ta còn có thể giả sử thêm rằng

$$
|g_1 a_1 + \cdots + g_n a_n| \leq M = \sup |f|
$$

trên X, do đó $k \leq 2M$. Tập hợp $N'$ các điểm gián đoạn của $k$ được chứa trong $N$, nên là không đáng kể. Với mọi $x \in X$, đặt $l(x) = \limsup_{y \to x} k(y)$.

Khi đó $2M \geq l \geq k$ trên X, và $l = k$ trên $X - N'$, nghĩa là, hầu khắp nơi đối với $\mu$, do đó $\int l \, d\mu \leq \varepsilon / 2$. Mặt khác, $l$ bị chặn và nửa liên tục trên, nên là bao dưới của tập hợp các hàm liên tục bị chặn $\geq l$. Vậy tồn tại một hàm liên tục bị chặn $h \geq l$ trên X sao cho $h \leq 2M$ và $\int h \, d\mu \leq \int l \, d\mu + \varepsilon / 2$ (§ 4, No. 4, Hệ quả 2 của Mệnh đề 5). Khi đó $\int h \, d\mu \leq \varepsilon$ và $|f - g_1 a_1 - \cdots - g_n a_n| \leq h$.

(ii) $\Rightarrow$ (i). Giả sử rằng điều kiện (ii) được thỏa mãn. Với mọi $x \in X$ gọi $\omega(x)$ là dao động của f tại x (GT, IX, § 2, No. 3). Cho $\varepsilon > 0$. Tồn tại $a_1, \ldots, a_n, g_1, \ldots, g_n, h$ có các tính chất của (ii). Với mọi $x \in X$, $\omega(x)$ là dao động của $f - g_1 a_1 - \cdots - g_n a_n$ tại x, do đó $\omega(x) \leq 2h(x)$. Vì thế $\int \omega \, d\mu \leq 2\varepsilon$. Do đó, tập hợp $A_\varepsilon$ các $x \in X$ sao cho $\omega(x) \geq \sqrt{\varepsilon}$ thỏa mãn $\mu(A_\varepsilon) \leq 2\sqrt{\varepsilon}$. Điều này chứng tỏ rằng $\mu(N) \leq 2\sqrt{\varepsilon}$, do đó $\mu(N) = 0$.

#### Mệnh đề 22 {#int-iv-s5-prop-22 .statement}

— *Cho F là một không gian Banach, X một không gian compact địa phương, $\mathcal{E}$ tập hợp các độ đo dương bị chặn trên X, $\mu$ một phần tử của $\mathcal{E}$, và $\mathcal{B}$ một cơ sở lọc trên $\mathcal{E}$. Giả sử rằng $\mathcal{B}$ hội tụ mơ hồ về $\mu$ và rằng $\| \nu \|$ hội tụ về $\| \mu \|$ đối với $\mathcal{B}$. Cho f là một ánh xạ từ X vào F thỏa mãn các điều kiện sau:

(i) f bị chặn, và khả tích đối với $\mu$ và đối với mọi độ đo thuộc một phần tử nào đó của $\mathcal{B}$;
(ii) tập hợp các điểm gián đoạn của f là $\mu$-không đáng kể.
Khi đó $\int f \, d\nu$ hội tụ về $\int f \, d\mu$ đối với $\mathcal{B}$.

Cho $\varepsilon > 0$. Tồn tại các phần tử $a_1, \ldots, a_n$ của F, các hàm $g_1, \ldots, g_n$ trong $\mathcal{K}(X)$, và một hàm liên tục bị chặn $h \geq 0$ trên X, sao cho

$$
|f - g_1 a_1 - \cdots - g_n a_n| \leq h \leq 2 \sup |f|
$$

trên X và $\int h \, d\mu \leq \varepsilon$ (Bổ đề 5). Đặt $M = \sup |f|$. Tồn tại một tập con compact K của X sao cho $\mu^*(X - K) \leq \varepsilon$ (§ 4, No. 7, Mệnh đề 12 and No. 6, Định lý 4), một lân cận compact $K'$ của K trong X, và một ánh xạ liên tục $h'$ từ X vào $[0, 2M]$ sao cho $h' = h$ trên K, $h' = 2M$ trên $X - K'$; thay thế $h'$ bằng $\sup(h, h')$, ta còn có thể giả sử rằng $h' \geq h$. Khi đó $\int (h' - h) \, d\mu \leq 2M \mu^*(X - K) \leq 2M \varepsilon$. Mặt khác, $h' = h_1 + 2M$, với $h_1 \in \mathcal{K}(X)$. Có tính đến § 4, No. 7, Mệnh đề 12, số

$$
\int h' \, d\nu = \int h_1 \, d\nu + 2M \|\nu\| \text{ hội tụ về } \int h_1 \, d\mu + 2M \|\mu\| = \int h' \, d\mu \text{ đối với } \mathcal{B}. \text{ Khi đó tồn tại một } A \in \mathcal{B} \text{ sao cho, với mọi } \nu \in A,
$$
$$
\left| \int (g_1 a_1 + \cdots + g_n a_n) \, d\nu - \int (g_1 a_1 + \cdots + g_n a_n) \, d\mu \right| \leq \varepsilon,
$$
$$
\int h \, d\nu \leq \int h' \, d\nu \leq \int h' \, d\mu + \varepsilon \leq \int h \, d\mu + 2M \varepsilon + \varepsilon \leq 2(M + 1)\varepsilon.
$$
Các bất đẳng thức này kéo theo
$$
\left| \int f \, d\nu - \int f \, d\mu \right| \leq
$$
$$
\int h \, d\nu + \left| \int (g_1 a_1 + \cdots + g_n a_n) \, d\nu - \int (g_1 a_1 + \cdots + g_n a_n) \, d\mu \right| + \int h \, d\mu
$$
$$
\leq 2(M + 2)\varepsilon,
$$
điều này chứng tỏ mệnh đề.

#### Nhận xét {#int-iv-s5-n12-rem-1 .statement}

Các điều kiện (i) và (ii) của Mệnh đề 22 được thỏa mãn nếu $f$ liên tục và bị chặn.

#### Ví dụ {#int-iv-s5-n12-exa-1 .statement}

Lấy $X$ là không gian compact $\mathbf{U}$ gồm các số phức có giá trị tuyệt đối bằng 1. Đặt $\mu(f) = \int_0^1 f(e^{2i\pi t}) \, dt$ với mọi $f \in \mathcal{H}(\mathbf{U})$, ta định nghĩa được một độ đo dương có khối lượng 1 trên $\mathbf{U}$. Mặt khác, cho $\theta$ là một số thực; với mọi số nguyên $n \geq 0$, gọi $\nu_n$ là khối lượng đơn vị đặt tại điểm $e^{2i\pi n \theta}$ của $\mathbf{U}$, và đặt
$$
\mu_n = \frac{1}{n+1} (\nu_0 + \cdots + \nu_n),
$$
sao cho $\mu_n$ là một độ đo dương có khối lượng 1 trên $\mathbf{U}$. Khi đó, nếu $\theta$ vô tỉ, $\mu_n$ hội tụ mơ hồ đến $\mu$. Thật vậy, vì các tổ hợp tuyến tính của các hàm $z \mapsto z^k$ ($k \in \mathbf{Z}$) là trù mật trong $\mathcal{H}(\mathbf{U})$ (GT, X, §4, No. 4, Prop. 8), chỉ cần chứng minh rằng $\mu_n(z^k)$ hội tụ đến $\mu(z^k)$ với $k \in \mathbf{Z}$. Bây giờ, với $k = 0$, $\mu_n(z^k) = \mu(z^k) = 1$; với $k \neq 0$,
$$
\mu_n(z^k) = \frac{1}{n+1} (1 + e^{2i\pi k \theta} + e^{4i\pi k \theta} + \cdots + e^{2i\pi k n \theta}).
$$
Vì $e^{2i\pi k \theta} \neq 1$ (do $\theta$ vô tỉ), suy ra
$$
|\mu_n(z^k)| = \left| \frac{1}{n+1} \frac{e^{2i\pi k(n+1)\theta} - 1}{e^{2i\pi k \theta} - 1} \right| \leq \frac{1}{n+1} \frac{2}{|e^{2i\pi k \theta} - 1|},
$$

do đó $\mu_n(z^k)$ hội tụ đến $0 = \mu(z^k)$. Trong các điều kiện ấy, có thể áp dụng Mệnh đề 22, và đặc biệt ta thấy rằng nếu $A$ là một tập con của $U$ có biên không đáng kể đối với $\mu$, thì $\mu_n(A)$ hội tụ đến $\mu(A)$. Nói cách khác, nếu $p_n$ ký hiệu số các số nguyên $k \in [0, n]$ sao cho $e^{2i\pi k \theta} \in A$, thì $n^{-1} p_n$ hội tụ đến $\mu(A)$ khi $n$ hội tụ đến $+\infty$.

### Bài tập {#int-iv-s5-exercises}

Xem [các bài tập của § 5](exercises/s5/).
