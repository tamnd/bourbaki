---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 7
section_title: Fibrés vectoriels
lang: vi
source: var-fr
pdf_pages: 0068-0085
extraction: ocr
subsections:
    - "no": 1
      title: Définition des fibrés vectoriels
      page: 0
      pdf_page: 68
    - "no": 2
      title: Morphismes de fibrés vectoriels
      page: 0
      pdf_page: 69
    - "no": 3
      title: Morphismes multilinéaires
      page: 0
      pdf_page: 71
    - "no": 4
      title: Sections
      page: 0
      pdf_page: 72
    - "no": 5
      title: Sous-fibrés vectoriels, fibrés vectoriels quotients, suites exactes
      page: 0
      pdf_page: 74
    - "no": 6
      title: Foncteurs vectoriels
      page: 0
      pdf_page: 76
    - "no": 7
      title: Sommes directes, fibrés d’applications multilinéaires, dual
      page: 0
      pdf_page: 78
    - "no": 8
      title: Fibrés d’applications multilinéaires alternées
      page: 0
      pdf_page: 79
    - "no": 9
      title: Produits tensoriels, espaces tensoriels, algèbre extérieure
      page: 0
      pdf_page: 81
    - "no": 10
      title: Fibrés vectoriels et fibrés principaux
      page: 0
      pdf_page: 83
    - "no": 11
      title: Changement de structure
      page: 0
      pdf_page: 85
statements: 0
exercises: 0
content_sha256: d3575cd12c8f31ef59a3c0febd751509fdfd81f020f1b04db03005c1dadb4d66
translated_from: content/en-mt/var/1/07_s7_fibres_vectoriels.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 3ea89201f780c796ce69c1f3f443fb7823d3576700c6b7dc188afb4fa20c7b4c
translation_model: gpt-5.4
translation_run: translate-vi-0cc2362d
glossary_version: 34
glossary_terms_sha256: 1ec0309119514a1a2ec3b0bb288c5588b520cba6815f8ab2ebdda2795c2a4342
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. Bó vectơ

Trong suốt mục này, chữ B ký hiệu một đa tạp lớp $C^r$ ($r \geqslant 1$) và chữ M ký hiệu một tập hợp được trang bị một ánh xạ $\pi$ từ M vào B. Ta nói B là cơ sở của M và với mọi $b \in B$, ta ký hiệu bởi $M_b$ và gọi là thớ của M tại $b$ tập con $\pi^{-1}(b)$ của M.

### 7.1. Định nghĩa bó vectơ

7.1.1. Một bản đồ vectơ của M là một bộ ba $t = (U, \varphi, F)$, trong đó U là một tập mở của B, F là một không gian Banach và $\varphi$ là một song ánh từ $\pi^{-1}(U)$ lên $U \times F$ sao cho $\pi(\varphi^{-1}(b, h)) = b$ với mọi $b \in B$ và mọi $h \in F$. Ta nói U là miền của bản đồ vectơ t và rằng t là một bản đồ vectơ của M tại $b \in B$ nếu $b \in U$. Với mọi $b \in U$, ta ký hiệu bởi $t_b$ song ánh từ F lên $M_b$ được xác định bởi $t_b(h) = \varphi^{-1}(b, h)$ với $h \in F$.

7.1.2. Ta nói rằng hai bản đồ vectơ $t = (U, \varphi, F)$ và $t' = (U', \varphi', F')$ của M là tương thích-$C^r$ (hoặc đơn giản là tương thích) nếu tồn tại một ánh xạ $\lambda$ lớp $C^r$ từ đa tạp $U \cap U'$ vào không gian Banach $\mathcal{L}(F; F')$ sao cho:

$$
t_b = t'_b \circ \lambda(b) \quad \text{với mọi } b \in U \cap U'.
$$

7.1.3. Ta nói rằng một tập hợp các bản đồ vectơ của M là một átlat vectơ-$C^r$ (hoặc đơn giản là átlat vectơ) của M nếu nó gồm các bản đồ vectơ từng đôi một tương thích-$C^r$ và các miền của chúng có hợp là B. Ta nói rằng hai átlat vectơ $\mathcal{A}$ và $\mathcal{B}$ của M là tương đương-$C^r$ (hoặc tương đương) nếu $\mathcal{A} \cup \mathcal{B}$ lại là một átlat vectơ của M. Quan hệ này là một quan hệ tương đương.

7.1.4. Một cấu trúc bó vectơ lớp $C^r$ (với cơ sở B) trên M là dữ kiện của một lớp tương đương các átlat vectơ (Ens., Chap. II, § 6, No. 9). Một bản đồ vectơ thuộc một átlat vectơ của lớp này được gọi là một bản đồ vectơ của bó vectơ M.

Cho M là một bó vectơ với cơ sở B. Với mọi $b \in B$, tồn tại trên thớ $M_b$ một và chỉ một cấu trúc không gian Banach sao cho, với mọi bản đồ vectơ $t = (U, \varphi, F)$ của bó vectơ M tại $b$, ánh xạ $t_b$ là một đẳng cấu từ F lên $M_b$.

Cho $c = (U, \psi, E)$ là một bản đồ của đa tạp B và cho $t = (U, \varphi, F)$ là một bản đồ vectơ của bó vectơ M, có cùng miền U. Với $x \in \pi^{-1}(U)$, đặt:

$$
\alpha(x) = (\psi(\pi(x)), t_{\pi(x)}^{-1}(x)).
$$

Khi đó bộ ba $(\pi^{-1}(U), \alpha, E \times F)$ là một bản đồ của tập hợp $M$. Tồn tại trên $M$ một và chỉ một cấu trúc đa tạp lớp $C'$ (được gọi là nền tảng của $M$) mà đối với nó mọi bản đồ thu được như vậy đều là các bản đồ của đa tạp $M$. Khi đó bộ ba $(M, B, \pi)$ là một phân thớ (6.1.1).

7.1.5. Cho $F$ là một không gian Banach. Đặt $M = B \times F$, ánh xạ là phép chiếu thứ nhất. Tồn tại trên $M$ một cấu trúc bó vectơ (với cơ sở $B$), và chỉ một, sao cho $(B, \mathrm{Id}_M, F)$ là một bản đồ vectơ. Người ta nói rằng $B \times F$ được trang bị cấu trúc này là bó vectơ tầm thường có cơ sở $B$ và thớ $F$, và đôi khi ký hiệu nó bởi $F_B$. Cấu trúc đa tạp của $F_B$ là cấu trúc đa tạp tích, và với mọi $b \in B$, ánh xạ $h \mapsto (b, h)$ là một đẳng cấu không gian Banach từ $F$ lên thớ của $F_B$ tại điểm $b \in B$. Người ta thường ký hiệu bởi $0$ một bó vectơ tầm thường mà thớ được thu về $0$.

7.1.6. Cho $M$ là một bó vectơ có cơ sở $B$. Với $b \in B$, người ta gọi là hạng của $M$ tại $b$ và ký hiệu bởi $\mathrm{rg}_b(M)$ chiều (hữu hạn hoặc $+\infty$) của không gian Banach $M_b$. Ta có $\dim_x M = \dim_b B + \mathrm{rg}_b M$ với $b = \pi(x)$. Hàm $b \mapsto \mathrm{rg}_b M$ là hằng địa phương. Người ta nói rằng $M$ có hạng hữu hạn nếu $\mathrm{rg}_b M < +\infty$ với mọi $b \in B$.

### 7.2. Cấu xạ của các bó vectơ

7.2.1. Cho $B$ và $B'$ là hai đa tạp và cho $f$ là một cấu xạ từ $B$ vào $B'$. Cho $M$ là một bó vectơ có cơ sở $B$ và $M'$ một bó vectơ có cơ sở $B'$. Người ta nói rằng một ánh xạ $g$ từ $M$ vào $M'$ là một $f$-cấu xạ của các bó vectơ nếu điều kiện sau được thỏa mãn:

Với mọi điểm $b_0 \in B$, tồn tại một biểu đồ vectơ $t = (U, \varphi, F)$ của $M$ tại $b_0$, một biểu đồ vectơ $t' = (U', \varphi', F')$ của $M'$ tại $f(b_0)$ và một ánh xạ $\lambda$ thuộc lớp $C'$ từ $U$ vào $\mathcal{L}(F; F')$ sao cho $f(U) \subset U'$ và $g_b \circ t_b = t'_{f(b)} \circ \lambda(b)$ với mọi $b \in U$, trong đó $g_b$ là hạn chế của $g$ lên $M_b$.

Dưới các giả thiết đó, $g$ là một cấu xạ của các đa tạp và, với mọi $b \in B$, $g$ cảm sinh một ánh xạ tuyến tính liên tục từ $M_b$ vào $M'_{f(b)}$. Hạng vectơ của $g$ tại $b \in B$ được gọi là và được ký hiệu bởi $\mathrm{rg}_b(g)$ hạng (hữu hạn hoặc $+\infty$) của ánh xạ tuyến tính $g_b$.

Ngược lại, nếu $r \geqslant \infty$ hoặc nếu $M$ có hạng hữu hạn, thì một $f$-cấu xạ của các phân thớ của $(M, B, \pi)$ vào $(M', B', \pi')$ mà cảm sinh trên mỗi thớ $M_b$ một ánh xạ tuyến tính từ $M_b$ vào $M'_{f(b)}$ (với mọi $b \in B$), là một $f$-cấu xạ của các bó vectơ.

7.2.2. Giả sử thêm rằng $f'$ là một cấu xạ từ $B'$ vào một đa tạp $B''$. Nếu $g$ là một $f$-cấu xạ của $M$ vào $M'$, và nếu $g'$ là một $f'$-cấu xạ của $M'$ vào một bó vectơ $M''$ có cơ sở là $B''$, thì ánh xạ $g' \circ g$ là một $(f' \circ f)$-cấu xạ của $M$ vào $M''$. Ta có $(g' \circ g)_b = g'_{f(b)} \circ g_b$ với mọi $b$ trong $B$.

7.2.3. Cho M và M' là hai bó vectơ có cùng cơ sở B. Một B-cấu xạ, hay đơn giản là một cấu xạ từ M vào M', được gọi là mọi Id_B-cấu xạ. Hợp thành của hai cấu xạ là một cấu xạ.

Cho g là một cấu xạ bó vectơ từ M vào M'; nếu g là song ánh, thì nó là một đẳng cấu của đa tạp M lên đa tạp M', ánh xạ nghịch đảo $g^{-1}$ là một cấu xạ bó vectơ từ M' vào M và ta có $(g^{-1})_b = g_b^{-1}$ với mọi b trong B. Khi đó ánh xạ g là một đẳng cấu bó vectơ.

7.2.4. Cho f là một cấu xạ của một đa tạp B' vào B và cho M là một bó vectơ có cơ sở B. Đặt $M' = B' \times_B M$ và ký hiệu bởi $\pi'$ (tương ứng g) sự hạn chế lên M' của phép chiếu từ $B' \times M$ lên B' (tương ứng M). Tồn tại trên M' một và chỉ một cấu trúc bó vectơ có cơ sở B' (đối với $\pi'$) sao cho g là một f-cấu xạ. Ta nói M' là bó vectơ có cơ sở B' ảnh ngược của M bởi f và ký hiệu nó bởi $f^*M$; f-cấu xạ g được gọi là f-cấu xạ chính tắc của $f^*M$ vào M.

Cấu trúc đa tạp của $f^*M$ là cấu trúc của tích thớ của các đa tạp B' và M trên B (5.11.2); với mọi $b \in B'$, ánh xạ $x \mapsto (b, x)$ là một đẳng cấu các không gian Banach từ $M_{f(b)}$ lên $(f^*M)_b$.

Việc thành lập các ảnh ngược của các bó vectơ là bắc cầu.

Cho N' là một bó vectơ có cơ sở B' và cho h là một f-cấu xạ từ N' vào M. Tồn tại một và chỉ một B'-cấu xạ $\tilde{h}$ từ N' vào $f^*M$ sao cho $h = g \circ \tilde{h}$.

Cho N là một bó vectơ có cơ sở B và v là một B-cấu xạ từ N vào M. Tồn tại một và chỉ một B'-cấu xạ, ký hiệu bởi $f^*v$, từ $f^*N$ vào $f^*M$ sao cho biểu đồ

$$
\begin{array}{ccc}
f^*N & \xrightarrow{f^*v} & f^*M \\
\downarrow & & \downarrow \\
N & \xrightarrow{v} & M
\end{array}
$$

là giao hoán.

7.2.5. Cho B' là một đa tạp con của B và cho i là đơn ánh chính tắc của B' vào B. Nếu M là một bó vectơ có cơ sở B, ảnh ngược $i^*M$ được gọi là bó vectơ cảm sinh trên B' bởi M và được ký hiệu bởi $M|B'$. Nếu $t = (U, \varphi, F)$ là một thẻ vectơ của M, thì $(U \cap B', \varphi|\pi^{-1}(U \cap B'), F)$ là một thẻ vectơ của $M|B'$. f-cấu xạ chính tắc của $M|B'$ vào M là một đẳng cấu đa tạp từ $M|B'$ lên đa tạp con $\pi^{-1}(B')$ của M.

7.2.6. Cho f là một cấu xạ của một đa tạp B' vào B và cho M (tương ứng M') là một bó vectơ có cơ sở B (tương ứng B'). Một f-đối cấu xạ từ M vào M' được gọi là một B'-cấu xạ từ $f^*M$ vào M'. Khi B = B' và $f = \mathrm{Id}_B$, việc cho một $f$-đối cấu xạ từ $M$ vào $M'$ tương đương với việc cho một $B$-cấu xạ từ $M$ vào $M'$.

Cho $g$ là một $f$-đối cấu xạ từ $M$ vào $M'$. Với mọi $b \in B'$, ánh xạ $g_b : x \mapsto g(b, x)$ từ $M_{f(b)}$ vào $M'_b$ là một ánh xạ tuyến tính liên tục.

Giả sử thêm rằng $f'$ là một cấu xạ của một đa tạp $B''$ vào $B'$ và rằng $h$ là một $f'$-đối cấu xạ từ $M'$ vào một bó vectơ $M''$ có cơ sở $B''$. Khi đó ánh xạ $h \circ f^*g$ từ ${f'}^*(f^*M) = (f \circ f')^*M$ vào $M''$ là một $(f \circ f')$-đối cấu xạ từ $M$ vào $M''$, ký hiệu bởi $h \circ g$. Với $b \in B''$, ta có

$$
(h \circ g)_b = h_b \circ g_{f'(b)}.
$$

### 7.3. Cấu xạ đa tuyến tính

7.3.1. Cho $M_1, \ldots, M_d$ và $N$ là các bó vectơ có cơ sở $B$, và cho $u$ là một ánh xạ từ tập hợp $M_1 \times_B \cdots \times_B M_d$ vào $N$. Ta nói $u$ là một *cấu xạ đa tuyến tính* (hay $d$-tuyến tính) nếu điều kiện sau được thỏa mãn:

*Với mọi $b_0 \in B$, tồn tại một lân cận mở $U$ của $b_0$ trong $B$, các bản đồ địa phương của bó vectơ $t^j = (U, \varphi^j, F^j)$ của $M_j$ (với $1 \leq j \leq d$) và $t = (U, \varphi, F)$ của $N$, và một ánh xạ $\lambda$ thuộc lớp $C^r$ từ $U$ vào không gian Banach $\mathcal{L}(F^1, \ldots, F^d; F)$ gồm các ánh xạ $d$-tuyến tính liên tục từ $F^1 \times \cdots \times F^d$ vào $F$, sao cho*:

$$
(t_b \circ \lambda(b))(x_1, \ldots, x_d) = u(t_b^1(x_1), \ldots, t_b^d(x_d))
$$

*với mọi $b \in U$ và mọi $x_j \in F^j$*.

Mọi cấu xạ đa tuyến tính $u$ đều là một cấu xạ đa tạp từ tích thớ $M_1 \times_B \cdots \times_B M_d$ vào $N$ và cảm sinh, với mỗi $b \in B$, một ánh xạ $d$-tuyến tính liên tục $u_b$ từ $(M_1)_b \times \cdots \times (M_d)_b$ vào $N_b$.

Nếu $f$ là một cấu xạ từ $B$ vào một đa tạp $B'$, thì theo định nghĩa, một cấu xạ đa tuyến tính từ $M_1 \times_B \cdots \times_B M_d$ vào một bó vectơ $M'$ có cơ sở $B'$ là hợp thành của một cấu xạ đa tuyến tính từ $M_1 \times_B \cdots \times_B M_d$ vào $f^*M'$ với cấu xạ $f$ chính tắc từ $f^*M'$ vào $M'$.

Một cấu xạ song tuyến tính cũng được gọi là một *ghép đôi*. Với $d = 1$, một cấu xạ tuyến tính là một cấu xạ theo nghĩa của 7.2.1. Với $d = 0$, một cấu xạ $0$-tuyến tính được đồng nhất với một *tiết diện* của $N$ (7.4).

7.3.2. Một *bó đại số* có cơ sở $B$ được gọi là một bó vectơ $A$ có cơ sở $B$, được trang bị một phép ghép cặp từ $A \times_B A$ vào $A$. Khi đó mỗi thớ $A_b$ được trang bị một cấu trúc đại số trên $K$. Nếu, với mọi $b \in B$, đại số $A_b$ có một phần tử đơn vị, ký hiệu bởi $e_b$, thì ánh xạ $b \mapsto e_b$ là một tiết diện của $A$ (xem 7.4). Một bó đại số $A$ được gọi là *địa phương tầm thường* nếu, với mọi điểm $b_0$ của $B$, tồn tại một phiến đồ vectơ $t = (U, \varphi, E)$ của $A$ tại điểm $b_0$ và một cấu trúc đại số trên $K$ của $E$ sao cho $t_b$ là một đẳng cấu đại số từ $E$ lên $A_b$ với mọi $b \in U$.

7.3.3. Cho $A$ là một bó đại số kết hợp có phần tử đơn vị, có cơ sở $B$. Một *bó A-môđun* có cơ sở $B$ được gọi là một bó vectơ $M$ có cơ sở $B$ được trang bị một phép ghép cặp $m : A \times_B M \to M$ sao cho ánh xạ $m_b : A_b \times M_b \to M_b$ xác định, với mọi $b \in B$, một cấu trúc $A_b$-môđun trên thớ $M_b$.

Cho $M$ và $M'$ là hai bó $A$-môđun. Một *đồng cấu A* từ $M$ vào $M'$ được gọi là mọi cấu xạ $g : M \to M'$ của các bó vectơ có cơ sở $B$ mà với mọi $b$ thuộc $B$ cảm sinh một ánh xạ $A_b$-tuyến tính từ $M_b$ vào $M'_b$.

Giả sử $A$ là địa phương tầm thường. Một phân thớ $M$ các $A$-môđun được gọi là *địa phương tầm thường* nếu, với mọi điểm $b_0$ của $B$, tồn tại một bản đồ vectơ $t = (U, \varphi, E)$ của $A$ tại $b_0$ như trong 7.3.2, một bản đồ vectơ $t' = (U, \varphi', L)$ của $M$ tại $b_0$, và một cấu trúc môđun của $E$ trên $L$ sao cho, với mọi $b \in U$, $t'_b$ là một $t_b$-đẳng cấu của $A_b$-môđun $M_b$ lên $E$-môđun $L$.

7.3.4. Cho $A$ là một đại số Banach trên $K$ (ví dụ một trường được trang bị một cấu trúc $K$-đại số hữu hạn chiều). Khi đó phân thớ tầm thường $A_B$ là một phân thớ các đại số, địa phương tầm thường. Một phân thớ địa phương tầm thường các $A_B$-môđun $M$ cũng được gọi là một phân thớ vectơ trên $A$ (có cơ sở là $B$). Khi đó các thớ $M_b$ là các $A$-môđun tôpô. Một $f$-cấu xạ $u$ của $M$ vào một phân thớ vectơ khác trên $A$ được gọi là $A$-tuyến tính nếu các ánh xạ $u_b$ là $A$-tuyến tính với mọi $b \in B$.

### 7.4. Các tiết diện

7.4.1. Cho $M$ là một phân thớ vectơ có cơ sở $B$. Với mọi tập mở $U$ của $B$, ta ký hiệu bởi $\mathscr{S}_M^r(U)$ tập hợp các tiết diện cấp $C^r$ của $M$ trên $U$, nghĩa là, các cấu xạ cấp $C^r$ từ $U$ vào $M$ sao cho $s(b) \in M_b$ với mọi $b \in U$. Tập hợp này được trang bị một cấu trúc môđun trên vành các hàm cấu xạ $\mathscr{C}^r(U)$ theo các quy tắc:

(1)
$$
(s + s')(b) = s(b) + s'(b)
$$
(2)
$$
(\varphi \cdot s)(b) = \varphi(b) \cdot s(b)
$$
với $s, s'$ trong $\mathscr{S}_M^r(U)$ và $\varphi$ trong $\mathscr{C}^r(U)$. Khi tập mở $U$ biến thiên, ta thu được một bó $\mathscr{S}_M^r$ các ánh xạ từ $B$ vào $M$ (x. No. 5.4.1), gọi là *bó các tiết diện* của $M$.

7.4.2. Cho $M_1, \ldots, M_d$ và $N$ là các bó vectơ có cơ sở $M$ và cho $u$ là một cấu xạ đa tuyến tính từ $M_1 \times_B \ldots \times_B M_d$ vào $N$. Với $1 \leq j \leq d$, giả sử ta cho một tiết diện $s_j$ của $M_j$ trên một tập mở $U$ của $B$; ta định nghĩa một tiết diện $u(s_1, \ldots, s_d)$ của $N$ trên $U$ bởi công thức:
$$
u(s_1, \ldots, s_d)(b) = u_b(s_1(b), \ldots, s_d(b)) \quad \text{với } b \in U.
$$

Ánh xạ $(s_1, \ldots, s_d) \mapsto u(s_1, \ldots, s_d)$ là đa tuyến tính trên $\mathcal{C}^r(U)$. Đôi khi nó được ký hiệu là $\mathscr{S}(u)$.

7.4.3. Cho $f$ là một cấu xạ từ một đa tạp $B'$ vào $B$ và cho $M$ là một bó vectơ có cơ sở $B$. Với mọi tập mở $U$ của $B$ và mọi $s \in \mathscr{S}_M^r(U)$, ánh xạ $x \mapsto (x, s(f(x)))$ là một tiết diện cấp $C^r$ của $f^*M$ trên tập mở $f^{-1}(U)$, được ký hiệu là $f^*s$ và gọi là ảnh ngược của $s$ bởi $f$. Ánh xạ $s \mapsto f^*s$ từ $\mathscr{S}_M^r(U)$ vào $\mathscr{S}_{f^*M}(f^{-1}(U))$ là nửa tuyến tính đối với đồng cấu $g \mapsto g \circ (f|f^{-1}(U))$ từ $\mathcal{C}^r(U)$ vào $\mathcal{C}^r(f^{-1}(U))$.

Nếu hơn nữa $N$ là một bó vectơ có cơ sở $B'$ và $g$ là một $f$-đối cấu xạ từ $M$ vào $N$, đôi khi người ta ký hiệu bởi $\mathscr{S}(g)$ ánh xạ $s \mapsto g \circ f^*s$ từ $\mathscr{S}_M^r(U)$ vào $\mathscr{S}_N^r(f^{-1}(U))$.

7.4.4. Cho $M$ là một bó vectơ với cơ sở $B$, *có hạng hữu hạn*. Một *khung* của $M$ trên một tập mở $U$ của $B$ được gọi là một dãy hữu hạn $(s_1, \ldots, s_n)$ các tiết diện của $M$ trên $U$ sao cho $(s_1(b), \ldots, s_n(b))$ là một *cơ sở* của không gian vectơ $M_b$ với mọi $b \in B$. Khi đó dãy $(s_1, \ldots, s_n)$ là một cơ sở của $\mathcal{C}^r(U)$-môđun $\mathscr{S}_M^r(U)$. Nếu $f$ là một cấu xạ từ một đa tạp $B'$ vào $B$, thì các tiết diện $f^*s_j$ lập thành một khung của $f^*M$ trên $f^{-1}(U)$.

7.4.5. Cho $L$ là một trường, được trang bị một cấu trúc đại số trên $K$ có số chiều hữu hạn và cho $(M, B, \pi)$ là một phân thớ. Giả sử rằng trên mỗi thớ $M_b$ đã cho một cấu trúc không gian vectơ trên $L$, *có số chiều hữu hạn*. Khi đó tồn tại nhiều nhất một cấu trúc bó vectơ trên $L$ với cơ sở $B$ trên $M$, tương thích với ánh xạ $\pi$, cấu trúc đa tạp của $M$ và các cấu trúc không gian vectơ trên $L$ trên các thớ (7.3.4). Để một cấu trúc như vậy tồn tại, điều kiện cần và đủ là điều kiện sau được thỏa mãn:

(FV) *Với mọi $b_0 \in B$, tồn tại một lân cận mở $U$ của $b_0$ trong $B$ và một đẳng cấu đa tạp $\varphi$ từ $\pi^{-1}(U)$ lên tích $U \times F$ của $U$ với một không gian vectơ $F$ trên $L$ có số chiều hữu hạn, sao cho với mọi $b \in U$, song ánh $\varphi_b$ từ $M_b$ lên $F$ cảm sinh bởi $\varphi$ là một đẳng cấu các không gian vectơ trên trường $L$.*

Khi đó các bộ ba $(U, \varphi, F)$ thỏa mãn (FV) là các bản đồ địa phương của bó vectơ của bó vectơ $M$.

Điều kiện (FV) tương đương với:
(FV') *Với mọi $b_0 \in B$, tồn tại một số nguyên $n$ và $n$ tiết diện $s_1, \ldots, s_n$ của $M$ trên một lân cận mở $U$ của $b_0$ sao cho ánh xạ*
$$
(b, a_1, \ldots, a_n) \mapsto a_1 s_1(b) + \cdots + a_n s_n(b)
$$
*là một đẳng cấu của đa tạp $U \times L^n$ lên đa tạp $\pi^{-1}(U)$.*

7.4.6. Cho $M_1, \ldots, M_d$ và $N$ là các bó vectơ có cơ sở $B$, trong đó các $M_j$ có *hạng hữu hạn*. Giả sử rằng với mọi tập mở $U$ của $B$ ta được cho một ánh xạ $\varphi_U$ từ $\mathscr{S}_{M_1}^r(U) \times \cdots \times \mathscr{S}_{M_d}^r(U)$ vào $\mathscr{S}_N^r(U)$, $\mathcal{C}^r(U)$-đa tuyến tính, sao cho với $V \subset U$ ta có:

$$
\varphi_U(s_1, \ldots, s_d)|V = \varphi_V(s_1|V, \ldots, s_d|V).
$$

Khi đó tồn tại một và chỉ một cấu xạ đa tuyến tính $u$ từ $M_1 \times_B \ldots \times_B M_d$ vào $N$ sao cho $\varphi_U(s_1, \ldots, s_d) = u(s_1, \ldots, s_d)$ với mọi tiết diện $s_j$ của $M$ trên tập mở $U$ của $B$.

7.4.7. Cho $f$ là một cấu xạ của một đa tạp $B'$ vào $B$ và cho $M$ (tương ứng $M'$) là một bó vectơ có cơ sở $B$ (tương ứng $B'$) và có hạng hữu hạn. Giả sử rằng với mọi tập mở $U$ của $B$ ta được cho một ánh xạ $\varphi_U$ từ $\mathcal{S}_M^r(U)$ vào $\mathcal{S}_{M'}^{r'}(f^{-1}(U))$, $\mathcal{C}^r(U)$-nửa tuyến tính, sao cho

$$
\varphi_U(s)|f^{-1}(V) = \varphi_V(s|V)
$$

với mọi tập mở $V \subset U$. Khi đó tồn tại một và chỉ một $f$-đối cấu xạ $g$ từ $M$ vào $M'$ sao cho $\varphi_U(s) = \mathcal{S}(g)(s)$ với mọi $s \in \mathcal{S}_M^r(U)$.

*7.4.8. Cho $\mathcal{F}$ là một bó các môđun trên bó các vành $\mathcal{C}_B^r$. Ta nói rằng $\mathcal{F}$ là địa phương tự do nếu với mọi $b \in B$, tồn tại một lân cận mở $U$ của $b$ và một số nguyên $n$ sao cho $\mathcal{F}|U$ đẳng cấu (như một bó các $\mathcal{C}_U^r$-môđun) với bó $(\mathcal{C}_U^r)^n$.

Nếu $M$ là một bó vectơ có cơ sở $B$ và hạng hữu hạn, thì faisceau $\mathcal{S}_M^r$ là tự do địa phương. Ngược lại, với mọi faisceau tự do địa phương $\mathcal{F}$ trên $B$, tồn tại một bó vectơ $M$ và một đẳng cấu của faisceau từ $\mathcal{S}_M^r$ lên $\mathcal{F}$. Nếu $M'$ là một bó vectơ khác có cơ sở $B$ và hạng hữu hạn, thì ánh xạ $g \mapsto \mathcal{S}(g)$ là một song ánh từ tập hợp các $B$-cấu xạ của $M$ vào $M'$ lên tập hợp các cấu xạ của faisceau các $\mathcal{C}^r$-môđun từ $\mathcal{S}_M^r$ vào $\mathcal{S}_{M'}^{r'}$*

### 7.5. Bó vectơ con, bó vectơ thương, dãy khớp

Trong số này, bó vectơ có nghĩa là bó vectơ có cơ sở $B$ và cấu xạ của các bó vectơ có nghĩa là một $\\mathrm{Id}_B$-cấu xạ.

7.5.1. Cho $M$ là một bó vectơ. Một tập con $M'$ của $M$ được gọi là một bó vectơ con của $M$ nếu, với mọi điểm $b \in B$, tồn tại một bản đồ vectơ $t = (U, \varphi, E)$ của $M$ tại $b$ và một không gian con vectơ đóng $F$ của $E$ có một phần bù tôpô, sao cho

$$
\varphi(\pi^{-1}(U) \cap M') = U \times F.
$$

Trong các điều kiện đó, trên $M'$ tồn tại một và chỉ một cấu trúc bó vectơ sao cho đơn ánh chính tắc của $M'$ vào $M$ là một cấu xạ. Với mỗi $b \in B$, thớ $M'_b$ của $M'$ là không gian con vectơ đóng $M' \cap M_b$ của $M_b$; $M'$ là một đa tạp con đóng của $M$ và cấu trúc đa tạp nền của cấu trúc bó vectơ của $M'$ trùng với cấu trúc được cảm sinh bởi cấu trúc đa tạp của $M$.

7.5.2. Cho $M'$ là một bó vectơ con của $M$. Gọi $R\{x, y\}$ là quan hệ sau giữa các điểm $x, y$ của $M$:
« tồn tại một phần tử $b$ của $B$ sao cho $x \in M_b, y \in M_b$ và $x - y \in M'_b$ ». Khi đó $R$ là một quan hệ tương đương chính quy trên $M$ (x. n° 5.9.7). Trên tập hợp $M/R$, tồn tại một và chỉ một cấu trúc bó vectơ sao cho ánh xạ chính tắc từ $M$ lên $M/R$ là một cấu xạ. Ta ký hiệu nó bởi $M/M'$ và gọi bó vectơ được xác định như vậy là thương của $M$ bởi $M'$; với mỗi điểm $b$ của $B$, bó $(M/M')_b$ là không gian vectơ tôpô thương $M_b/M'_b$ và cấu trúc đa tạp trên $M/M'$ là thương của cấu trúc đa tạp trên $M$.

7.5.3. Giữ các giả thiết của 7.5.2. Với mọi điểm $b_0$ của $B$, ta có thể tìm được một lân cận mở $U$ của $b_0$, một không gian Banach $F$, là tổng trực tiếp của hai không gian con đóng $F'$ và $F''$, và một đẳng cấu bó vectơ $\iota$ từ $F_U$ lên $M|U$ với các tính chất sau:
(i) Hạn chế $\iota'$ của $\iota$ lên $U \times F'$ là một đẳng cấu từ $F'_U$ lên $M'|U$.
(ii) Nếu $\rho$ là ánh xạ chính tắc từ $M$ lên $M'' = M/M'$, và nếu $\iota''$ là hạn chế của $\iota$ lên $U \times F''$, thì ánh xạ $\rho \circ \iota''$ là một đẳng cấu từ $F''_U$ lên $M''|U$.

7.5.4. Nếu một cấu xạ của các bó vectơ $g : L \to M$ có ảnh được chứa trong $M'$, thì nó là một cấu xạ của các bó vectơ từ $L$ vào $M'$.
Bây giờ xét một cấu xạ của các bó vectơ $h : M \to N$ và giả sử rằng, với mọi $b$ thuộc $B$, hạn chế của $h_b$ lên $M'_b$ bằng không. Nếu $\rho$ là cấu xạ chính tắc từ $M$ lên $M/M'$, thì tồn tại một và chỉ một cấu xạ $\bar{h}$ từ $M/M'$ vào $N$ sao cho $h = \bar{h} \circ \rho$.

7.5.5. Cho $P$ và $Q$ là hai bó vectơ, và cho $g$ là một cấu xạ từ $P$ vào $Q$; với mọi điểm $b$ của $B$, ký hiệu bởi $N_b$ và $I_b$ tương ứng là hạt nhân và ảnh của ánh xạ tuyến tính $g_b : P_b \to Q_b$. Đặt $N = \bigcup_{b \in B} N_b$ và $I = \bigcup_{b \in B} I_b$. Cấu xạ $g$ được gọi là trực tiếp địa phương nếu $N$ là một bó vectơ con của $P$ và $I$ là một bó vectơ con của $Q$. Khi đó cấu xạ $g$ xác định, bằng cách chuyển qua thương, một đẳng cấu từ $P/N$ lên $I$. Người ta nói rằng $N$ là hạt nhân của $g$ và ký hiệu nó bởi $\mathrm{Ker}\,g$. Tương tự, bó con $I$ được gọi là ảnh của $g$ và được ký hiệu bởi $\mathrm{Im}\,g$.
Nếu $r \geqslant \infty$, cấu xạ $g$ là trực tiếp địa phương khi và chỉ khi $g$ là một phép dưới-ngâm. Nếu $P$ có hạng hữu hạn, cấu xạ $g$ là trực tiếp địa phương khi và chỉ khi hạng vectơ của $g$ là hằng địa phương, hay tương đương, khi và chỉ khi $g$ là một phép dưới-ngâm.

7.5.6. Cho $M \xrightarrow{f} M' \xrightarrow{g} M''$ là hai cấu xạ của các bó vectơ. Ta nói rằng dãy $(f, g)$ là khớp trực tiếp địa phương nếu hai cấu xạ $f$ và $g$ là trực tiếp địa phương và nếu $\operatorname{Im} f = \operatorname{Ker} g$. Nếu $g \circ f = 0$, tập hợp $D$ các điểm $b \in B$ sao cho dãy $M_b \xrightarrow{f_b} M'_b \xrightarrow{g_b} M''_b$ là khớp trực tiếp (nghĩa là $\operatorname{Ker} f_b$ và $\operatorname{Im} g_b$ có các phần bù tôpô và $\operatorname{Im} f_b = \operatorname{Ker} g_b$) là mở, và dãy $M|D \xrightarrow{f} M'|D \xrightarrow{g} M''|D$ là khớp trực tiếp địa phương.

Người ta định nghĩa tương tự các dãy khớp trực tiếp địa phương có độ dài tùy ý. Do lạm dụng ngôn ngữ, đôi khi người ta nói dãy khớp trực tiếp thay cho dãy khớp trực tiếp địa phương.

7.5.7. Cho $0 \to M \xrightarrow{f} M' \xrightarrow{g} M'' \to 0$ là một dãy các cấu xạ của các bó vectơ. Để dãy này là khớp trực tiếp địa phương, điều kiện cần và đủ là $f$ là một đẳng cấu từ $M$ lên một bó vectơ con $f(M)$ của $M'$ và $g$ định nghĩa, bằng cách chuyển qua thương, một đẳng cấu của bó vectơ thương $M'/f(M)$ lên $M''$.

### 7.6. Hàm tử vectơ

Trong số này và trong ba số tiếp theo 7.7 đến 7.9, chữ I chỉ một tập hợp hữu hạn, hợp của hai tập con rời nhau $I_+$ và $I_-$. Ta ký hiệu bởi $\mathcal{V} = (V_i)_{i \in I}$ (và tương tự bởi $\mathcal{V}', \mathcal{V}'', \ldots$) một họ các không gian Banach được đánh chỉ số bởi $I$. Ta ký hiệu bởi $\operatorname{Hom}(\mathcal{V}, \mathcal{V}')$ không gian Banach $\prod_{i \in I_+} \mathcal{L}(V_i; V'_i) \times \prod_{i \in I_-} \mathcal{L}(V'_i; V_i)$ và bởi $f = (f_i)$ một phần tử của $\operatorname{Hom}(\mathcal{V}, \mathcal{V}')$. Ta ký hiệu bởi $\operatorname{Id}_{\mathcal{V}}$ phần tử $(\operatorname{Id}_{V_i})_{i \in I}$ của $\operatorname{Hom}(\mathcal{V}, \mathcal{V})$. Với $f \in \operatorname{Hom}(\mathcal{V}, \mathcal{V}')$ và $f' \in \operatorname{Hom}(\mathcal{V}', \mathcal{V}'')$, ta ký hiệu bởi $f' \circ f$ phần tử của $\operatorname{Hom}(\mathcal{V}, \mathcal{V}'')$ mà các thành phần được cho bởi:

$$
(f' \circ f)_i = f'_i \circ f_i \quad \text{nếu } i \in I_+
$$
$$
(f' \circ f)_i = f_i \circ f'_i \quad \text{nếu } i \in I_-
$$

7.6.1. Một hàm tử vectơ (tương ứng, hàm tử vectơ hữu hạn chiều) kiểu I và lớp $C^r$ là dữ liệu, với mỗi họ $\mathcal{V} = (V_i)_{i \in I}$ các không gian Banach (tương ứng, các không gian vectơ hữu hạn chiều trên $K$), của một không gian Banach $\tau(\mathcal{V})$ và, với mỗi $f \in \operatorname{Hom}(\mathcal{V}, \mathcal{V}')$, của một phần tử $\tau(f) \in \mathcal{L}(\tau(\mathcal{V}); \tau(\mathcal{V}'))$, các dữ liệu này thỏa mãn hai điều kiện sau:
(a) Ta có $\tau(\operatorname{Id}_\mathcal{V}) = \operatorname{Id}_{\tau(\mathcal{V})}$ và $\tau(f' \circ f) = \tau(f') \circ \tau(f)$.
(b) Ánh xạ $\tau : \operatorname{Hom}(\mathcal{V}, \mathcal{V}') \to \mathcal{L}(\tau(\mathcal{V}); \tau(\mathcal{V}'))$ là thuộc lớp $C^r$.

7.6.2. Cho $\mathcal{M} = (M^i)_{i \in I}$ là một họ các bó vectơ có cơ sở $B$. Với $b \in B$, đặt $\mathcal{M}_b = (M^i_b)_{i \in I}$. Cho $\tau$ là một hàm tử vectơ và gọi $\tau(\mathcal{M})$ là tập hợp tổng của các $\tau(\mathcal{M}_b)$ với $b \in B$; *trên $\tau(\mathcal{M})$ tồn tại một và chỉ một cấu trúc bó vectơ* (có cơ sở $B$ đối với ánh xạ $\pi$ từ $\tau(\mathcal{M})$ vào $B$ sao cho, với mọi $b \in B$, ta có $\tau(\mathcal{M}_b) = \{ b \}$) có tính chất sau:

Cho $U$ là một tập mở của $B$ và, với mọi $i$, cho $t^i = (U, \varphi_i, F_i)$ là một bản đồ vectơ của $M^i$, có miền xác định là $U$; đặt $\mathcal{F} = (F_i)_{i \in I}$ và gọi $\psi_b$ là phần tử của $\mathrm{Hom}(\mathcal{M}_b, \mathcal{F})$ được xác định bởi $(\psi_b)_i = (t^i_b)^{-1}$ với $i \in I_+$ và $(\psi_b)_i = t^i_b$ với $i \in I_-$; với $x \in \pi^{-1}(U)$, đặt $\psi(x) = (\pi(x), \tau(\psi_{\pi(x)})(x))$. Khi đó bộ ba $(U, \psi, \tau(\mathcal{F}))$ là một bản đồ vectơ của bó vectơ $\tau(\mathcal{M})$.

Được trang bị cấu trúc này, $\tau(\mathcal{M})$ được gọi là *bó vectơ suy ra từ họ $\mathcal{M}$ bởi hàm tử vectơ $\tau$*.

7.6.3. Cho $f$ là một cấu xạ từ $B$ vào một đa tạp $B'$. Cho $\mathcal{M} = (M^i)$ (tương ứng $\mathcal{M}' = ({M'}^i)$) là một họ được đánh chỉ số bởi $I$ các bó vectơ có cơ sở $B$ (tương ứng $B'$). Với mọi $i \in I_+$, cho $g_i$ là một $f$-cấu xạ từ $M^i$ vào ${M'}^i$ và với mọi $i \in I_-$, cho $g_i$ là một $f$-đối cấu xạ từ ${M'}^i$ vào $M^i$. Đặt $g = (g_i)_{i \in I}$ và với $b \in B$, đặt $g_b = ((g_i)_b)_{i \in I}$ (xem 7.2.1 và 7.2.6). *Tồn tại một và chỉ một $f$-cấu xạ, ký hiệu là $\tau(g)$, từ $\tau(\mathcal{M})$ vào $\tau(\mathcal{M}')$ sao cho $\tau(g)_b = \tau(g_b)$ với mọi $b \in B$*.

Đặc biệt, nếu $M^i = f^*{M'}^i$, các $g_i$ là các cấu xạ hoặc đối cấu xạ chính tắc, thì $B$-cấu xạ từ $\tau(\mathcal{M})$ vào $f^*\tau(\mathcal{M}')$ được xác định bởi $\tau(g)$ (7.2.4) là một đẳng cấu: sự kiện này được diễn đạt bằng cách nói rằng $\tau$ *giao hoán với các ảnh nghịch đảo*.

Đặc biệt, cho $B'$ là một đa tạp con của $B$ và đặt $\mathcal{M}|B' = (M^i|B')_{i \in I}$. Khi đó các bó vectơ $\tau(\mathcal{M})|B'$ và $\tau(\mathcal{M}|B')$ đẳng cấu với nhau trên $B'$ một cách chính tắc.

7.6.4. Cho $\tau, \tau_1, \ldots, \tau_d$ là các hàm tử vectơ (kiểu $I$ và lớp $C'$). Một *cấu xạ $d$-tuyến tính* $\theta$ từ $(\tau_1, \ldots, \tau_d)$ vào $\tau$ là dữ liệu, với mọi họ $\mathcal{V}$ các không gian Banach được đánh chỉ số bởi $I$, của một ánh xạ tuyến tính $d$-tuyến tính liên tục $\theta_{\mathcal{V}}$ từ $\tau_1(\mathcal{V}) \times \cdots \times \tau_d(\mathcal{V})$ vào $\tau(\mathcal{V})$, dữ liệu này thỏa mãn điều kiện sau: với mọi $f \in \mathrm{Hom}(\mathcal{V}', \mathcal{V}'')$ ta có
$$
\tau(f) \circ \theta_{\mathcal{V}} = \theta_{\mathcal{V}''} \circ (\tau_1(f) \times \cdots \times \tau_d(f)).
$$
Với $d = 1$, người ta nói đơn giản là một *cấu xạ* từ $\tau_1$ vào $\tau$.

Cho $\mathcal{M}$ khi đó là một họ được chỉ số hóa bởi $I$ các bó vectơ trên $B$.
*Tồn tại một và chỉ một cấu xạ B-d-tuyến tính $\theta_{\mathcal{M}}$ từ $\tau_1(\mathcal{M}) \times_B \cdots \times_B \tau_d(\mathcal{M})$ vào $\tau(\mathcal{M})$ sao cho $(\theta_{\mathcal{M}})_b = \theta_{\mathcal{M}_b}$ với mọi $b \in B$*.

Với các ký hiệu của 7.6.3., ta có
$$
\tau(g) \circ \theta_{\mathcal{M}} = \theta_{\mathcal{M}'} \circ (\tau_1(g) \times \cdots \times \tau_d(g)).
$$
Nếu $d = 1$, và nếu $\theta$ là một đẳng cấu (nghĩa là $\theta_{\mathcal{V}}$ là một đẳng cấu với mọi họ $\mathcal{V}$), thì $\theta_{\mathcal{M}}$ là một đẳng cấu.

7.6.5. Các định nghĩa và kết quả của các No. 7.6.2 đến 7.6.4 mở rộng cho trường hợp các hàm tử vectơ hữu hạn chiều, với điều kiện giả thiết ở mọi nơi rằng các bó vectơ đã cho đều có hạng hữu hạn.

Chúng cũng mở rộng cho trường hợp sau: cho L là một trường được trang bị một cấu trúc đại số trên K hữu hạn chiều; lấy cho τ một hàm tử vectơ trên L (tức là thỏa mãn các giả thiết của 7.6.1 trong đó K đã được thay bằng L), và chỉ xét các bó vectơ trên L theo nghĩa của 7.3.4.

7.6.6. Ta gọi là một hàm tử vectơ cho các đẳng cấu (tương ứng, hàm tử vectơ hữu hạn chiều cho các đẳng cấu) dữ liệu, với mỗi không gian Banach V (tương ứng, mỗi không gian vectơ hữu hạn chiều trên K), của một không gian Banach τ(V) và, với mỗi đẳng cấu f của V lên một không gian Banach V’, của một đẳng cấu τ(f) của τ(V) lên τ(V’), các dữ liệu này phải thỏa mãn điều kiện (a) của 7.6.1 và điều kiện sau:

(b’) Ánh xạ $f \mapsto \tau(f)$ từ tập con mở của $\mathcal{L}(V; V')$ được tạo thành bởi các đẳng cấu của V lên V’, vào $\mathcal{L}(\tau(V); \tau(V'))$, thuộc lớp $C^r$.

Các định nghĩa và kết quả của các Số trước đó mở rộng cho trường hợp các hàm tử vectơ cho các đẳng cấu (bằng cách lấy $I_+ = \{1\}$ và $I_- = \varnothing$), ngoại trừ các định nghĩa và kết quả của đoạn thứ nhất của Số 7.6.3.

### 7.7. Tổng trực tiếp, các bó của các ánh xạ đa tuyến tính, đối ngẫu

7.7.1. Giả sử rằng $I_- = \varnothing$. Ta định nghĩa một hàm tử vectơ σ gọi là hàm tử tổng trực tiếp bằng cách đặt $\sigma(\mathcal{V}) = \bigoplus_{i \in I} V_i$ và $\sigma(\mathfrak{f}) = \bigoplus_{i \in I} f_i$. Nếu $\mathcal{M} = (M^i)_{i \in I}$ là một họ các bó vectơ trên B, thì bó vectơ $\sigma(\mathcal{M})$ được gọi là tổng trực tiếp của các $M^i$ và được ký hiệu bởi $\bigoplus_{i \in I} M^i$. Với mỗi $b \in B$, thớ tại $b$ của $\bigoplus_{i \in I} M^i$ là tổng trực tiếp của các thớ của các $M^i$ tại $b$.

Cho U là một tập con mở của B và cho $s_i \in \mathscr{F}_{M_i}(U)$ (với $i \in I$). Khi đó ánh xạ $b \mapsto \sum_{i \in I} s_i(b)$ là một tiết diện, ký hiệu là $\sum_i s_i$, thuộc lớp $C^r$ của $M = \bigoplus_{i \in I} M^i$ và ánh xạ $(s_i)_{i \in I} \mapsto \sum_i s_i$ là một đẳng cấu các $\mathscr{C}^r(U)$-môđun từ $\bigoplus_{i \in I} \mathscr{F}_{M_i}(U)$ lên $\mathscr{F}_M(U)$.

Đa tạp nền của $\bigoplus_{i \in I} M^i$ được đồng nhất với tích thớ $\prod_B M^i$.

Ta ký hiệu bởi $\mathrm{pr}_i$ cấu xạ các bó vectơ từ $\bigoplus_{i \in I} M^i$ vào $M^i$ mà trên mỗi thớ $\bigoplus_{i \in I} M^i_b$ là phép chiếu thứ i. Ta định nghĩa tương tự đơn ánh chính tắc $j_i$ của $M^i$ vào $\bigoplus_{i \in I} M^i$.

Cho $f$ là một cấu xạ từ B vào một đa tạp $B'$; cho H là một tập hợp hữu hạn thứ hai và cho $\mathcal{N} = (N^h)_{h \in H}$ là một họ các bó vectơ có cơ sở $B'$. Ánh xạ $u \to \bigoplus_{i \in I} (\mathrm{pr}_h \circ u \circ j_i)_{(h,i) \in H \times I}$ là một song ánh từ tập hợp các $f$-cấu xạ của $\bigoplus_{i \in I} M^i$ vào $\bigoplus_{h \in H} N^h$ lên tập hợp các ma trận $(u_{h,i})_{(h,i) \in H \times I}$, trong đó $u_{h,i}$ là một $f$-cấu xạ từ $M^i$ vào $N^h$.

Nếu $I = \{1,2\}$, dãy
$$
0 \to M^{1} \xrightarrow{j_1} M^1 \oplus M^2 \xrightarrow{\mathrm{pr}_2} M^2 \to 0
$$
là khớp trực tiếp.

Ngược lại, cho $M$ là một bó vectơ có cơ sở $B$ và cho $M'$ là một bó vectơ con của $M$. Giả sử rằng đa tạp $B$ là paracompact và rằng một trong hai điều kiện sau được thỏa mãn:
(i) $K$ khác $\mathbf{R}$ hoặc $\mathbf{C}$;
(ii) $K = \mathbf{R}, r \neq \omega$ và đa tạp $B$ thừa nhận các phân hoạch đơn vị lớp $C^r$ (5.3.6).

Khi đó tồn tại một bó vectơ con $M''$ của $M$ sao cho $M$ được đồng nhất với tổng trực tiếp $M' \oplus M''$.

7.7.2. Giả sử rằng $I_+ = \{0\}$ và rằng $I_- = \{1,2,\ldots,d\}$. Ta định nghĩa một hàm tử vectơ $\eta_d$ kiểu $I$ và lớp $C^r$ bằng cách đặt $\eta_d(\mathcal{V}) = \mathcal{L}(V_1,\ldots,V_d; V_0)$ và $\eta_d(f)(u) = f_0 \circ u \circ (f_1 \times \cdots \times f_d)$ với $u \in \eta_d(\mathcal{V})$. Nếu $\mathcal{M} = (M_i)_{i \in I}$ là một họ các bó vectơ có cơ sở $B$, bó vectơ $\eta_d(\mathcal{M})$ được ký hiệu bởi $\mathcal{L}(M_1,\ldots,M_d; M_0)$.

Cho $u$ là một cấu xạ đa tuyến tính từ $M_1 \times_B \cdots \times_B M_d$ vào $M_0$. Khi đó ánh xạ $\hat{u} : b \mapsto u_b$ là một tiết diện của $\mathcal{L}(M_1,\ldots,M_d; M_0)$ và ánh xạ $u \mapsto \hat{u}$ là song ánh.

7.7.3. Giữ các ký hiệu của 7.7.2 và giả sử thêm rằng $d = 1$. Khi đó bó vectơ $\mathcal{L}(M_1; M_0)$ được gọi là bó các đồng cấu từ $M_1$ vào $M_0$. Các tiết diện của nó tương ứng với các $B$-cấu xạ từ $M_1$ vào $M_0$.

Nếu hơn nữa $M_0$ là bó tầm thường $K_B$, bó vectơ $\mathcal{L}(M_1; K_B)$ được gọi là đối ngẫu của $M = M_1$ và được ký hiệu bởi $M'$: thớ $(M')_b$ là không gian các dạng tuyến tính liên tục trên thớ $M_b$ của $M$ tại điểm $b \in B$.

Nếu $s$ (resp. $t$) là một tiết diện của $M$ (resp. $M'$) trên một tập mở $U$ của $B$, ánh xạ $b \mapsto (b, \langle s(b), t(b) \rangle)$ là một tiết diện, ký hiệu là $\langle s, t \rangle$ của bó tầm thường $K_B$.$^1$

### 7.8. Các bó của các ánh xạ đa tuyến tính phản xứng

Trong các số 7.8.1 đến 7.8.5, giả thiết rằng $K$ có đặc số 0 hoặc các bó vectơ được xét có hạng hữu hạn. Người ta chưa biết liệu định nghĩa của hàm tử vectơ $\alpha_d$ được cho trong 7.8.1 có thể được thực hiện mà không có bất kỳ hạn chế nào hay không.

7.8.1. Cho $I_+ = \{0\}, I_- = \{1\}$ và cho $d$ là một số nguyên $\geqslant 1$. Ta định nghĩa một

$^1$ Khi $M$ có hạng hữu hạn, người ta viết $M^*$ thay cho $M'$.

hàm tử vectơ $\alpha_d$ bằng cách ký hiệu bởi $\alpha_d(\mathcal{V})$ không gian Banach của các ánh xạ $d$-tuyến tính phản xứng liên tục từ $V_1^d$ vào $V_0$ và bằng cách đặt $\alpha_d(f)(u) = f_0 \circ u \circ f_1^d$ đối với $u \in \alpha_d(\mathcal{V})$. Bó vectơ $\alpha_d((M_1, M_0))$ được ký hiệu là $\mathrm{Alt}^d(M_1; M_0)$ và được gọi là bó vectơ của các ánh xạ $d$-tuyến tính phản xứng từ $M_1$ vào $M_0$.

Đơn ánh chính tắc của $\mathrm{Alt}^d(M_1; M_0)$ vào $\mathcal{L}(M_1, \ldots, M_1; M_0)$ là một cấu xạ của các bó vectơ; $\mathrm{Alt}^d(M_1; M_0)$ là một bó vectơ con của $\mathcal{L}(M_1, \ldots, M_1; M_0)$.

Ta có $\mathrm{Alt}^1(M_1; M_0) = \mathcal{L}(M_1; M_0)$. Ta đặt $\mathrm{Alt}^0(M_1; M_0) = M_0$.

Nếu $\omega$ là một tiết diện $^1$ của $\mathrm{Alt}^d(M_1; M_0)$ và nếu $s_1, \ldots, s_d$ là các tiết diện của $M_1$, thì tồn tại một và chỉ một tiết diện của $M_0$, ký hiệu là $\omega(s_1, \ldots, s_d)$, sao cho
$$
\omega(s_1, \ldots, s_d)(b) = \omega(b)(s_1(b), \ldots, s_d(b)) \quad \text{với mọi } b \in B.
$$

7.8.2 Cho $\varphi$ là một ghép cặp của $N \times_B N'$ vào $N''$ (xem No. 7.3.1); với mỗi $b$, ta có một ánh xạ song tuyến tính $\varphi_b$ của $N_b \times N'_b$ vào $N''_b$ mà từ đó định nghĩa (xem A, III, p. 142) một ánh xạ song tuyến tính của
$$
\mathrm{Alt}^d(M; N)_b \times \mathrm{Alt}^e(M; N')_b
$$
vào $\mathrm{Alt}^{d+e}(M; N'')_b$. Họ các ánh xạ song tuyến tính này định nghĩa một ghép cặp $u$ của
$$
\mathrm{Alt}^d(M; N) \times_B \mathrm{Alt}^e(M; N')
$$
vào $\mathrm{Alt}^{d+e}(M; N'')$; nếu $\omega$ và $\omega'$ lần lượt là các tiết diện của $\mathrm{Alt}^d(M; N)$ và $\mathrm{Alt}^e(M; N')$ trên một tập mở $U$, thì tiết diện $u(\omega, \omega')$ của $\mathrm{Alt}^{d+e}(M; N'')$ trên $U$ sẽ được ký hiệu là $\omega \wedge_\varphi \omega'$, và được gọi là tích ngoài của $\omega$ và $\omega'$.
Ta có công thức:
(1) $$
(\omega \wedge_\varphi \omega')(s_1, \ldots, s_{d+e}) = \sum_\sigma \varepsilon_\sigma \varphi(\omega(s_{\sigma(1)}, \ldots, s_{\sigma(d)}), \omega'(s_{\sigma(d+1)}, \ldots, s_{\sigma(d+e)}))
$$
trong đó các $s_i$ là các tiết diện của $M$ trên $U$, và trong đó phép lấy tổng được mở rộng trên các hoán vị $\sigma$ của $\{1, 2, \ldots, d+e\}$ sao cho
$$
\sigma(1) < \cdots < \sigma(d) \quad \text{and} \quad \sigma(d+1) < \cdots < \sigma(d+e).
$$

7.8.3. Cho $M$ là một bó vectơ và $A$ một bó đại số, có cơ sở $B$. Giả sử rằng các sợi $A_b$ của $A$ là các đại số kết hợp và giao hoán, có một phần tử đơn vị, ký hiệu là $e_b$. Với mỗi tập mở $U$ của $B$, ta sẽ ký hiệu bởi $\Omega^d(U)$ môđun $\mathcal{C}^r(U)$ gồm các tiết diện của bó $\mathrm{Alt}^d(M; A)$ và bởi $\Omega^*(U)$ tổng trực tiếp của các $\Omega^d(U)$ với $d \geq 0$. Các phép nhân trên mỗi sợi định nghĩa một ghép cặp của $A \times_B A$ vào $A$, do đó theo (7.8.2) một cấu trúc đại số phân bậc trên $\Omega^*(U)$, cấu trúc này là kết hợp và phản giao hoán. Đại số con $\Omega^0(U)$ là đại số của

¹ Bạn đọc cần chú ý đừng nhầm cách dùng chữ cái $\omega$ này với cách dùng được định nghĩa ở p. 10.

các tiết diện của A. Một phần tử $\omega$ của $\Omega^1(U)$ được đồng nhất với một cấu xạ trên $U$ của $M|U$ vào $A|U$ (7.7.3): nếu $s \in \mathcal{S}'_M(U)$, ta sẽ ký hiệu bởi $\langle \omega, s \rangle$ tiết diện $\omega(s)$ của A (7.4.2). Cho $s_j \in \mathcal{S}'_M(U)$ và $\omega_j \in \Omega^1(U)$ (với $1 \leq j \leq d$); ta có:

(2) $$
\omega(s_1, \ldots, s_d) = \det(\langle \omega_i, s_j \rangle) \quad \text{với } \omega = \omega_1 \wedge \ldots \wedge \omega_d.
$$

7.8.4. Cho $d \geq 1$. Tồn tại một phép ghép cặp $i$ từ $M \times_B \mathrm{Alt}^d(M; A)$ vào $\mathrm{Alt}^{d-1}(M; A)$ mà hạn chế của nó trên mỗi thớ được cho bởi tích trong phải (xem A, III, p. 156). Nếu $s$ là một tiết diện của $M$ trên tập mở $U$ và nếu $\omega \in \Omega^d(U)$, ta ký hiệu bởi $i(s)\omega$ tiết diện $i(s, \omega)$ của $\mathrm{Alt}^{d-1}(M; A)$ trên $U$; ta đặt $i(s)\omega = 0$ đối với $\omega$ trong $\Omega^0(U)$.

Như vậy với mỗi tiết diện $s$ của $M$ trên $U$ ta liên kết một tự đồng cấu của $\mathcal{C}'(U)$-môđun $\Omega^*(U)$. Ta có các công thức sau:

(3) $$(i(s)\omega)(s_1, \ldots, s_{d-1}) = \omega(s, s_1, \ldots, s_{d-1}) \quad \text{với } \omega \in \Omega^d(U), d \geq 1$$
(4) $$i(s) \circ i(s) = 0$$
(5) $$i(s)\omega = \langle \omega, s \rangle \quad \text{với } \omega \in \Omega^1(U)$$
(6) $$i(s) . (\omega \wedge \omega') = i(s)\omega \wedge \omega' + (-1)^d \omega \wedge i(s)\omega' \quad \text{với } \omega \in \Omega^d(U)$$
(7) $$i(s)(\omega_1 \wedge \ldots \wedge \omega_p) = \sum_{i=1}^p (-1)^{i+1} \langle \omega_i, s \rangle \omega_1 \wedge \ldots \wedge \hat{\omega}_i \wedge \ldots \wedge \omega_d.$$

Trong công thức cuối cùng, các $\omega_i$ thuộc $\Omega^1(U)$ và dấu $\hat{}$ chỉ ra rằng ký hiệu mà nó đội lên phải được lược bỏ.

Mọi phép toán mô tả ở trên trên các tiết diện đều là đa tuyến tính trên vành $\mathcal{C}'(U; K)$.

7.8.5. Cho L là một đại số Banach trên K. Các định nghĩa và kết quả của Số 7.7 và 7.8 mở rộng sang trường hợp các bó vectơ trên L: theo cách tương tự người ta định nghĩa các bó của các ánh xạ đa tuyến tính trên L hoặc phản xứng đa tuyến tính trên L.

### 7.9. Tích tenxơ, không gian tenxơ, đại số ngoài

Ta giữ các ký hiệu của 7.6. Hơn nữa, ta ký hiệu bởi L một trường giao hoán được trang bị một cấu trúc đại số trên K hữu hạn chiều và ta gọi bó vectơ là một bó vectơ trên L, với cơ sở B và hạng hữu hạn địa phương.

7.9.1. Giả sử rằng $I_- = \varnothing$. Nếu $\mathcal{V}$ và $\mathcal{V}'$ là hai họ được đánh chỉ số bởi I gồm các không gian vectơ hữu hạn chiều trên L, ta ký hiệu bởi $\tau(\mathcal{V})$ tích tenxơ của các $V_i$ với $i \in I$ (A, II, p. 71) và nếu $f \in \mathrm{Hom}(\mathcal{V}, \mathcal{V}')$, ta đặt $\tau(f) = \otimes f_i$. Như vậy ta định nghĩa một hàm tử vectơ trên L trong số chiều hữu hạn và nếu $\mathcal{M} = (M_i)_{i \in I}$ là một họ các bó vectơ, ta ký hiệu bởi $\bigotimes_{i \in I} M_i$ và gọi là tích tenxơ (trên L) của các $M_i$ bó vectơ $\tau(\mathcal{M})$.

Nếu $s_i$ là một tiết diện của $M_i$ trên tập mở U của B (với $i \in I$), ánh xạ $b \mapsto \bigotimes_{i \in I} s_i(b)$ là một tiết diện của $\bigotimes_{i \in I} M_i$, được ký hiệu bởi $\bigotimes_{i \in I} s_i$. Ánh xạ $(s_i)_{i \in I} \mapsto \bigotimes_{i \in I} s_i$ là đa tuyến tính trên vành $\mathcal{C}^r(U;L)$.

7.9.2. Các đẳng cấu chính tắc được định nghĩa trong Alg., Chap. II cung cấp các đẳng cấu của các hàm tử vectơ. Từ 7.6.4 suy ra rằng có các đẳng cấu của các bó vectơ. Ví dụ, có các đẳng cấu chính tắc:

$$
(M_1 \oplus M_2) \otimes M_3 \longrightarrow (M_1 \otimes M_3) \oplus (M_2 \otimes M_3)
$$
$$
M_1^* \otimes M_2 \longrightarrow \mathcal{L}(M_1; M_2)
$$

v.v.

7.9.3. Cho $M$ là một bó vectơ và $I$ và $J$ là hai tập hợp hữu hạn rời nhau. Bó tenxơ $T^I_J(M)$ được định nghĩa là tích tenxơ $\bigotimes_{\alpha \in I \cup J} M_\alpha$, trong đó $M_\alpha = M$ nếu $\alpha \in I$, và $M_\alpha = M^*$ nếu $\alpha \in J$, ở đây $M^*$ ký hiệu đối ngẫu của $M$ (A, III, p. 63). Thớ $T^I_J(M)_b$ của bó này tại một điểm $b$ bằng không gian tenxơ $T^I_J(M_b)$ được định nghĩa trong Alg., loc. cit. Khi $I = \{1, \ldots, p\}$ và $J = \{p+1, \ldots, p+q\}$, người ta viết $T^p_q(M)$ thay cho $T^I_J(M)$; ta có
$$
T^p_q(M) = (\bigotimes^p M) \otimes (\bigotimes^q M^*).
$$
Việc cho một thứ tự toàn phần trên $I$ và trên $J$ xác định một đẳng cấu chính tắc từ $T^I_J(M)$ lên $T^p_q(M)$.

7.9.4. Nếu $I$ (resp. $J$) là hợp của hai tập con rời nhau $I'$ và $I''$ (resp. $J'$ và $J''$), thì $T^I_J(M)$ được đồng nhất một cách chính tắc với tích tenxơ $T^{I'}_{J'}(M) \otimes T^{I''}_{J''}(M)$. Đặc biệt, nếu $s'$ (resp. $s''$) là một tiết diện của $T^{I'}_{J'}(M)$ (resp. của $T^{I''}_{J''}(M)$), thì tích tenxơ $s' \otimes s''$ được đồng nhất với một tiết diện của $T^I_J(M)$.

7.9.5. Đối ngẫu của $T^I_J(M)$ được đồng nhất với $T^J_I(M)$.

7.9.6. Cho $i \in I$ và $j \in J$. Với mọi $b \in B$, đồng cấu co các chỉ số $i$ và $j$ được định nghĩa (xem Alg., loc. cit.); đó là một đồng cấu $(c^i_j)_b : T^I_J(M_b) \to T^{I-\{i\}}_{J-\{j\}}(M_b)$. Họ các $(c^i_j)_b$ xác định một cấu xạ của các không gian bó vectơ
$$
c^i_j : T^I_J(M) \to T^{I-\{i\}}_{J-\{j\}}(M),
$$

cũng được gọi là phép co các chỉ số $i$ và $j$. Người ta định nghĩa tương tự phép co các chỉ số $i_1, \ldots, i_k$ của $I$ với các chỉ số $j_1, \ldots, j_k$ của $J$.

7.9.7. Cho $d$ là một số nguyên $\geqslant 0$; cho $V$ và $V'$ là hai không gian vectơ có số chiều hữu hạn trên $L$ và $f \in \mathrm{Hom}_L(V, V')$; đặt $\lambda_d(V) = \bigwedge^d(V)$ và $\lambda_d(f) = \bigwedge^d(f)$. Như vậy ta định nghĩa được một hàm tử vectơ trên $L$ trong số chiều hữu hạn và, nếu $M$ là một bó vectơ, ta ký hiệu bởi $\bigwedge^d(M)$ và gọi là lũy thừa ngoài thứ $d$ của $M$ (trên $L$) bó vectơ $\lambda_d(M)$.

Ánh xạ chính tắc của $\bigotimes^d V$ lên $\bigwedge^d(V)$ xác định một cấu xạ của các hàm tử vectơ, do đó một cấu xạ chính tắc của $\bigotimes^d M$ vào $\bigwedge^d(M)$. Cấu xạ này là toàn ánh.

Các đẳng cấu chính tắc của không gian các ánh xạ $d$-tuyến tính phản xứng trên không gian $\bigwedge^d(V^*)$ hoặc trên $(\bigwedge^d(V))^*$ cho ta các đẳng cấu, được gọi là chính tắc, của bó vectơ $\mathrm{Alt}^d(M; L)$ các ánh xạ $d$-tuyến tính phản xứng trên $L$, lên bó vectơ $\bigwedge^d(M^*)$ hoặc lên $(\bigwedge^d(M))^*$.

7.9.8. Bây giờ đặt $\lambda(V) = \bigwedge(V)$ và $\lambda(f) = \bigwedge(f)$; như vậy ta lại định nghĩa được một hàm tử vectơ trên $L$ trong số chiều hữu hạn. Bó vectơ $\lambda(M)$ được ký hiệu bởi $\bigwedge(M)$. Sợi $\bigwedge(M)_b$ của nó tại $b \in B$ là đại số ngoài (trên $L$) của sợi $M_b$. Bó vectơ $\bigwedge(M)$ là một bó vectơ địa phương tầm thường theo các đại số.

Các định nghĩa và tính chất của các tích trong đã cho trong Alg., Chương III, ấn bản thứ 3, § 10 được mở rộng ngay lập tức cho các tiết diện của các bó vectơ $\bigwedge(M)$ và $\bigwedge(M^*)$ (xem thêm các công thức (1) đến (7) của các Số 7.8.2 đến 7.8.4).

7.9.9. Cho $M$ là một bó vectơ. Với mỗi số nguyên $n$, gọi $B_n$ là tập hợp (mở) các điểm $b \in B$ sao cho chiều (trên $L$) của $M_b$ bằng $n$. Với $b \in B_n$, đặt $N_b = \bigwedge^n(M_b)$ và gọi $N$ là tập hợp tổng của các $N_b$ với $b \in B$. Trên $N$ tồn tại một và chỉ một cấu trúc bó vectơ sao cho ánh xạ hiển nhiên của $N|B_n$ vào $\bigwedge^n(M)|B_n$ là một đẳng cấu với mọi $n$. Được trang bị cấu trúc này, bó vectơ $N$ có hạng một tại mỗi điểm được ký hiệu bởi $\det(M)$.

### 7.10. Bó vectơ và bó chính

7.10.1. Cho $F$ là một không gian Banach. Một bó vectơ M có cơ sở $B$ được gọi là thuần kiểu $F$ nếu mọi thớ $M_b$ của M (với $b \in B$) đều đẳng cấu (như các không gian Banach) với $F$.

Cho $M$ là một bó vectơ có cơ sở $B$ thuần kiểu $F$ và gọi $P$ là dưới đa tạp mở của bó vectơ $\mathcal{L}(F_B; M)$ gồm các cặp $(b, u)$ trong đó $b \in B$ và $u$ là một đẳng cấu từ $F_b = F$ lên $M_b$. Nhóm $\mathrm{GL}(F)$ các tự đẳng cấu của $F$ tác động bên phải trên $P$ bằng cách đặt $(b, u) \cdot g = (b, u \circ g)$ với $(b, u) \in P$ và $g \in \mathrm{GL}(F)$. Gọi $\pi_P$ là ánh xạ $(b, u) \mapsto b$ từ P vào B. Bộ tứ $\lambda = (P, GL(F), B, \pi_P)$ (trong đó $GL(F)$ được trang bị cấu trúc chính tắc của một đa tạp nhóm (5.12.2)) là một phân thớ chính (6.2.1): nó được gọi là phân thớ các khung của M. Ánh xạ $((b, u), h) \mapsto u(h)$ từ $P \times F$ vào M trang bị cho M một cấu trúc bó liên kết với $\lambda$, kiểu thớ F (6.5.1).

Khi $F = K^n$, ta có thể đồng nhất một đẳng cấu $u$ từ F lên $M_b$ với cơ sở của $M_b$ là ảnh bởi $u$ của cơ sở chính tắc của $K^n$. Không gian phân thớ các khung của M khi đó được đồng nhất với dưới đa tạp mở của $M \times_B \ldots \times_B M$ tạo thành bởi các cơ sở $(e_1, \ldots, e_n)$ của các thớ khác nhau $M_b$.

Cho U là một tập con mở của B và gọi $t = (U, \varphi, E)$ là một phiến đồ vectơ của M có miền U, với $E = F$. Khi đó ánh xạ $b \mapsto (b, t_b)$ là một tiết diện của P, ký hiệu là $\tilde{t}$, và ánh xạ $t \mapsto \tilde{t}$ là một song ánh từ tập hợp các phiến đồ vectơ của M có dạng $(U, \varphi, F)$ lên tập hợp các tiết diện của P trên U.

7.10.2. Ngược lại, cho $\lambda = (Q, G, B, \pi_Q)$ là một phân thớ chính và cho $\varphi$ là một đồng cấu các đa tạp nhóm của G vào nhóm $GL(F)$ các tự đẳng cấu của một không gian Banach F. Cho G tác động bên trái lên F bằng cách đặt $g . h = \varphi(g)(h)$ ($h \in F, g \in G$). Cho M là một không gian phân thớ liên kết với $\lambda$, kiểu sợi là F, và cho $\rho : Q \times F \to M$ là ánh xạ khung của nó (6.5.1). Cho $\pi$ là ánh xạ từ M vào B được xác định bởi
$$
\pi(\rho(q, h)) = \pi_Q(q) \quad (q \in Q \text{ and } h \in F).
$$
Cho s là một tiết diện của Q trên một tập con mở U của B; khi đó ánh xạ
$$
\tilde{s} : (b, h) \mapsto (s(b), h)
$$
là một song ánh từ $U \times F$ lên $\pi^{-1}(U)$. Tồn tại trên cặp $(M, \pi)$ một và chỉ một cấu trúc bó vectơ với cơ sở B mà đối với nó các bộ ba $t_s = (U, \tilde{s}^{-1}, F)$ là các thẻ vectơ (với mọi tiết diện s của Q). Cấu trúc đa tạp nền của cấu trúc này là cấu trúc của không gian phân thớ liên kết với $\lambda$.

Cho $q \in Q$; đặt $b = \pi_Q(q)$ và cho $u$ là đẳng cấu từ F lên $M_b$ được xác định bởi $u(h) = \rho(q, h)$ (với $h \in F$). Ánh xạ $f : q \mapsto (b, u)$ là một B-cấu xạ của các phân thớ chính, tương thích với $\varphi$, từ $(Q, G, B, \pi_Q)$ vào bó khung $(P, GL(F), B, \pi_P)$ của bó vectơ M.

7.10.3. Xét lại các ký hiệu của No. 7.6. Với mọi $i \in I$, cho
$$
\lambda_i = (P_i, G_i, B, \pi_i)
$$
là một phân thớ chính có cơ sở B và giả sử rằng $G_i$ tác động bên trái lên một không gian Banach $V_i$ bằng một đồng cấu
$$
\varphi_i : G_i \to GL(V_i).
$$
Cho $M_i$ là một không gian phân thớ liên kết với $\lambda_i$ có kiểu sợi $V_i$. Đặt $\mathcal{M} = (M_i)_{i \in I}$ và $\mathcal{V} = (V_i)_{i \in I}$ và cho $\lambda$ là phân thớ chính tích của các $\lambda_i$ trên B (6.2.5). Đặt $\hat{\lambda} = (\mathbf{P}, G, B, \pi_p)$, với $G = \prod_{i \in I} G_i$.

Bây giờ cho $\tau$ là một hàm tử vectơ. Với $g = (g_i) \in G$, cho $\varphi(g)$ là phần tử của $\mathrm{Hom}(\mathcal{V}, \mathcal{V})$ được xác định bởi:

$$
\varphi(g)_i = \varphi_i(g_i) \quad \text{nếu } i \in I_+
$$
$$
\varphi(g)_i = \varphi_i(g_i)^{-1} \quad \text{nếu } i \in I_-
$$

Khi đó nhóm $G$ tác động trên $\tau(\mathcal{V})$ bằng cấu xạ $g \mapsto \tau(\varphi(g))$ từ $G$ vào $\mathbf{GL}(\tau(\mathcal{V}))$.

Mặt khác, cho $x = (x_i)$ là một điểm của $\mathbf{P}$ và cho $b = \pi_p(x)$. Với mỗi $i$, ánh xạ $\theta_{x_i}$ được xác định ở No. 6.5.2 là một đẳng cấu từ $V_i$ lên $(M_i)_b$. Cho $\theta_x$ là phần tử của $\mathrm{Hom}(\mathcal{V}, ((M_i)_b)_{i \in I})$ được xác định bởi:

$$
(\theta_x)_i = \theta_{x_i} \quad \text{khi } i \in I_+
$$
$$
(\theta_x)_i = \theta_{x_i}^{-1} \quad \text{khi } i \in I_-
$$

Gọi $\rho$ là ánh xạ $(x, h) \mapsto (b, \tau(\theta_x)(h))$ từ $\mathbf{P} \times \tau(\mathcal{V})$ vào bó vectơ $\tau(\mathcal{M})$; ánh xạ $\rho$ trang bị cho $\tau(\mathcal{M})$ một cấu trúc không gian sợi liên kết với $\lambda$ có kiểu sợi là $\tau(\mathcal{V})$.

Các nhận xét này tổng quát hóa cho trường hợp các functor vectơ hữu hạn chiều, hoặc các functor vectơ trên một trường $L$ được trang bị một cấu trúc đại số trên K hữu hạn chiều.

### 7.11. Thay đổi cấu trúc

Các cấu trúc và các phép toán được mô tả trong đoạn này là tương thích với các thay đổi cấu trúc được mô tả trong các Số 5.13 và 5.14.
