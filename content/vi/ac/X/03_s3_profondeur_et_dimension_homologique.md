---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 3
section_title: Profondeur et dimension homologique
lang: vi
source: ac-x-fr
pdf_pages: 0036-0051, 0156-0161
extraction: ocr
subsections:
    - "no": 1
      title: Dimension projective, dimension injective, dimension homologique
      page: 0
      pdf_page: 36
    - "no": 2
      title: Localisation de la dimension homologique
      page: 38
      pdf_page: 37
    - "no": 3
      title: Dimension homologique des anneaux noethériens
      page: 0
      pdf_page: 38
    - "no": 4
      title: Quotient par un élément simplifiable
      page: 43
      pdf_page: 42
    - "no": 5
      title: Profondeur et dimension projective
      page: 45
      pdf_page: 44
    - "no": 6
      title: Profondeur et dimension injective
      page: 0
      pdf_page: 46
    - "no": 7
      title: Anneaux de Gorenstein
      page: 48
      pdf_page: 47
    - "no": 8
      title: Anneaux de Gorenstein et algèbres plates
      page: 51
      pdf_page: 50
statements: 43
exercises: 16
content_sha256: 97074bf4e0b7d66ea426469d075d0d9947078be236d40dee52c0c092cbaa8a09
translated_from: content/en-mt/ac/X/03_s3_profondeur_et_dimension_homologique.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 927ab24cfb8adb74f59214b45fd1d9cb691be35e594a7fbdad39dd905060f696
translation_model: gpt-5.4
translation_run: translate-vi-d67fbc25
glossary_version: 34
glossary_terms_sha256: 527256ecf5d765a8484cc1836331d1c0aa49b5c95267d1a55a0561d8a74360b7
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ĐỘ SÂU VÀ CHIỀU ĐỒNG ĐIỀU

### 1. Chiều xạ ảnh, chiều nội xạ, chiều đồng điều

Cho A là một vành, M là một A-môđun. Nhắc lại (A, X, p. 134, Định nghĩa 1) rằng chiều xạ ảnh của M, ký hiệu là dp_A(M), là cận dưới lớn nhất (trong $\overline{\mathbf{Z}}$) của tập các độ dài của những phân giải xạ ảnh của M. Ta có dp_A(0) = -∞ và dp_A(M) ≥ 0 nếu M khác không. Để M là xạ ảnh, điều kiện cần và đủ là dp_A(M) ≤ 0.

#### Ví dụ {#ac-x-s3-n1-exa-1 .statement}

Cho J là một iđêan của A được sinh bởi một dãy A-chính quy $x = (x_1, \ldots, x_r)$. Ta có dp_A(A/J) ≤ r. Thật vậy, điều này hiển nhiên nếu A là không; trong trường hợp ngược lại, phức Koszul $K_\bullet(x, A)$ là một phân giải tự do của A/J có độ dài r (loc. cit., p. 159, Nhận xét 3). Hơn nữa, với mọi A-môđun N, các A-môđun Ext_A^r(A/J, N) và N/JN là đẳng cấu (loc. cit.); do đó, để có dp_A(A/J) = r, điều kiện cần và đủ là J phân biệt với A (loc. cit., p. 134, Mệnh đề 1).

Tương tự, người ta định nghĩa chiều nội xạ của M, ký hiệu là di_A(M), là cận dưới lớn nhất của tập các độ dài của những phân giải nội xạ của M. Ta có di_A(0) = -∞, và di_A(M) ≥ 0 nếu M ≠ 0. Để M là nội xạ, điều kiện cần và đủ là di_A(M) ≤ 0.

#### Mệnh đề 1 {#ac-x-s3-prop-1 .statement}

Cho A là một vành, M là một A-môđun và n là một số nguyên ≥ 0. Các điều kiện sau là tương đương:

(i) ta có di_A(M) ≤ n (nói cách khác, M có một phân giải nội xạ với độ dài ≤ n) ;
(ii) với mọi A-môđun N và mọi số nguyên i > n, ta có Ext_A^i(N, M) = 0 ;
(iii) với mọi iđêan a của A, ta có Ext_A^{n+1}(A/a, M) = 0 ;
(iv) với mọi dãy khớp các A-môđun

$$
0 \to M \to I^0 \to I^1 \to \ldots \to I^{n-1} \to Q \to 0,
$$

trong đó các $I^i$ là nội xạ, A-môđun Q là nội xạ.

(i) ⇒ (ii) : điều này suy ra từ A, X, p. 100, Định lý 1.
(ii) ⇒ (iii) : điều này hiển nhiên.
(iii) ⇒ (iv) : trong tình huống của (iv), với mọi A-môđun N ta có một đẳng cấu từ Ext_A^1(N, Q) lên Ext_A^{n+1}(N, M) (A, X, p. 128, Hệ quả 4) ; dưới giả thiết (iii), A-môđun Ext_A^1(A/a, Q) bằng không với mọi iđêan a của A, và Q là nội xạ (A, X, p. 93, Mệnh đề 11).
(iv) ⇒ (i) : xét dãy khớp (A, X, p. 52)

$$
0 \to M \to I^0(M) \to \ldots \to I^{n-1}(M) \to K^{n-1}(M) \to 0;
$$

nếu điều kiện (iv) được thỏa mãn thì A-môđun $K^{n-1}(M)$ là nội xạ, do đó có (i).

Nhắc lại (A, X, p. 138, Định nghĩa 2) rằng chiều đồng điều của vành $A$, ký hiệu là $\mathrm{dh}(A)$, là cận trên nhỏ nhất trong $\overline{\mathbf{Z}}$ của tập các số nguyên $n$ sao cho tồn tại hai $A$-môđun $M$ và $N$ để cho $\mathrm{Ext}^n_A(M, N)$ khác không. Vì vậy nó cũng là cận trên nhỏ nhất của tập các chiều xạ ảnh (hoặc các chiều nội xạ) của mọi $A$-môđun; khi $A$ là Noether, chỉ cần giới hạn vào các $A$-môđun hữu hạn sinh (A, X, p. 139, Hệ quả).

### 2. Địa phương hóa của chiều đồng điều

#### Mệnh đề 2 {#ac-x-s3-prop-2 .statement}

Cho $A$ là một vành, $M$ và $N$ là các $\Lambda$-môđun, $i$ là một số nguyên và $S$ là một tập con nhân tính của $\Lambda$. Ta có một đẳng cấu chính tắc của các $S^{-1}A$-môđun

$$
S^{-1} \mathrm{Tor}_i^\Lambda(M, N) \longrightarrow \mathrm{Tor}_i^{S^{-1}\Lambda}(S^{-1}M, S^{-1}N) .
$$

Nếu vành $A$ là Noether và A-môđun $M$ hữu hạn sinh, ta có một đẳng cấu chính tắc của các $S^{-1}\Lambda$-môđun

$$
S^{-1} \mathrm{Ext}_\Lambda^i(M, N) \longrightarrow \mathrm{Ext}_{S^{-1}\Lambda}^i(S^{-1}M, S^{-1}N) .
$$

Vì A-môđun $S^{-1}A$ là phẳng, điều này suy ra từ A, X, p. 110, Mệnh đề 9 và p. 111, Mệnh đề 10.

#### Hệ quả {#ac-x-s3-n2-cor-1 .statement}

Cho $A$ là một vành, $M$ và $N$ là các $\Lambda$-môđun, $i$ là một số nguyên.

a) Giá của $\mathrm{Tor}_i^\Lambda(M, N)$ được chứa trong $\mathrm{Supp}(M) \cap \mathrm{Supp}(N)$, và điều tương tự cũng đúng cho giá của $\mathrm{Ext}_\Lambda^i(M, N)$ nếu $A$ là Noether và $M$ hữu hạn sinh.

b) Giả sử rằng $A$ là Noether, và các môđun $M$ và $N$ là hữu hạn sinh; nếu $\Lambda$-môđun $M \otimes_A N$ có độ dài hữu hạn, thì điều tương tự cũng đúng với $\mathrm{Tor}_i^\Lambda(M, N)$ và với $\mathrm{Ext}_\Lambda^i(M, N)$.

Nếu $p$ là một iđêan nguyên tố của $A$ không thuộc $\mathrm{Supp}(M) \cap \mathrm{Supp}(N)$, thì một trong hai môđun $M_p$ hoặc $N_p$ bằng không, điều này kéo theo a) theo Mệnh đề 2.

Để một môđun hữu hạn sinh trên một vành Noether có độ dài hữu hạn, điều kiện cần và đủ là giá của nó gồm các iđêan cực đại (IV, § 2, No. 5, Mệnh đề 7). Dưới giả thiết b), các A-môđun $\mathrm{Tor}_i^\Lambda(M, N)$ và $\mathrm{Ext}_\Lambda^i(M, N)$ là hữu hạn sinh (A, X, p. 108, Hệ quả) ; do đó mệnh đề b) suy ra từ a).

#### Mệnh đề 3 {#ac-x-s3-prop-3 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun hữu hạn sinh, và $N$ là một $A$-môđun.

a) Ta có

$$
\mathrm{dp}_A(M) = \sup_p \mathrm{dp}_{A_p}(M_p) , \quad \mathrm{di}_A(N) = \sup_p \mathrm{di}_{A_p}(N_p) , \quad \mathrm{dh}(A) = \sup_p \mathrm{dh}(A_p) ,
$$

trong đó $p$ chạy trên tập hợp các iđêan nguyên tố (tương ứng là các iđêan cực đại) của $A$.

b) Ánh xạ $p \mapsto \mathrm{dp}_{A_p}(M_p)$ từ $\mathrm{Spec}(A)$ vào $\overline{\mathbf{Z}}$ là nửa liên tục trên.

Ta hãy chứng minh a). Cho $n$ là một số nguyên $\geqslant 0$. Giả sử rằng ta có $\mathrm{dp}_A(M) < n$. Với mọi iđêan nguyên tố $p$ của $A$ và mọi $A_p$-môđun $Q$, $A_p$-môđun $\mathrm{Ext}_A^n(M_p, Q)$ đẳng cấu với $(\mathrm{Ext}_A^n(M, Q))_p$ (Mệnh đề 2), do đó bằng không; suy ra bất đẳng thức

Ta hãy chứng minh b). Cho p là một iđêan nguyên tố của A và n = dp_{A_p}(M_p). Hãy chỉ ra rằng tồn tại một lân cận U của p trong Spec(A) sao cho ta có dp_{A_q}(M_q) \leq n với mọi q \in U. Điều này là hiển nhiên nếu n = +\infty ; nếu n = -\infty , điều này suy ra từ việc giá của M là đóng. Bây giờ giả sử rằng n là hữu hạn và chọn một dãy khớp các A-môđun
$$
P_{n-1} \xrightarrow{d_{n-1}} P_{n-2} \longrightarrow \ldots \longrightarrow P_0 \xrightarrow{d_0} M \to 0 ,
$$
trong đó các P_i là tự do kiểu hữu hạn (A, X, p. 53, Mệnh đề 6). Đặt P = Ker d_{n-1} ; đây là một môđun trình bày hữu hạn. A_p-môđun P_p là xạ ảnh (A, X, p. 134, Mệnh đề 1), do đó tự do (II, § 3, No. 2, Hệ quả 2 của Mệnh đề 5). Theo II, § 5, No. 1, Hệ quả của Mệnh đề 2, tồn tại một phần tử f của A - p sao cho A_f-môđun P_f là tự do; khi đó A_q-môđun P_q là tự do với mọi phần tử q của tập mở U của Spec(A) tạo bởi các iđêan nguyên tố không chứa f . Điều này chứng minh b).

#### Hệ quả 1 {#ac-x-s3-prop-3-cor-1 .statement}

Với mọi tập hợp nhân S của A , ta có
$$
\mathrm{dp}_{S^{-1}A}(S^{-1}M) \leq \mathrm{dp}_A(M) \quad , \quad \mathrm{di}_{S^{-1}A}(S^{-1}N) \leq \mathrm{di}_A(N) \quad , \quad \mathrm{dh}(S^{-1}A) \leq \mathrm{dh}(A) .
$$

#### Hệ quả 2 {#ac-x-s3-prop-3-cor-2 .statement}

Nếu ta có dp_{A_m}(M_m) < +\infty với mọi iđêan cực đại m của Supp(M) , thì ta có dp_A(M) < +\infty .

Thật vậy, không gian con X của Supp(M) tạo bởi các iđêan cực đại là quasi-compact (II, § 4, No. 2, Mệnh đề 8 và 9 và No. 3, Hệ quả 7 của Mệnh đề 11) ; ánh xạ m \mapsto dp_{A_m}(M_m) từ X vào \overline{\mathbf{R}} là nửa liên tục trên (Mệnh đề 3), do đó bị chặn (TG, IV, p. 30, Hệ quả của Định lý 3).

#### Nhận xét {#ac-x-s3-n2-rem-1 .statement}

Cho A là một vành Noether chính quy có chiều vô hạn (VIII, § 5, Bài tập 6 c)). Ta sẽ thấy dưới đây (No. 7, Định lý 2 và § 4, No. 1, Mệnh đề 1) rằng ta có di_{A_m}(A_m) = dh(A_m) < +\infty với mọi iđêan cực đại m của A ; do đó Mệnh đề 3 kéo theo di_A(A) = dh(A) = +\infty . Vì thế, các ánh xạ p \mapsto di_{A_p}(N_p) và p \mapsto dh(A_p) nói chung không nửa liên tục trên.

### 3. Chiều đồng điều của các vành Noether

Cho A là một vành địa phương Noether, M là một A-môđun hữu hạn sinh. Nhắc lại (A, X, § 3, No. 6) rằng một giải
$$
\ldots \longrightarrow L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \ldots \longrightarrow L_0 \xrightarrow{d_0} M \to 0
$$
của M là một giải xạ ảnh tối thiểu nếu mỗi môđun L_i đều là tự do kiểu hữu hạn, và nếu phức $\kappa_A \otimes_A L$ có vi phân bằng không. Với mọi số nguyên $i \geq 0$, khi đó ta có

(1) $$ \operatorname{Ext}_A^i(M, \kappa_A) : \kappa_A ] = [\operatorname{Tor}_i^A(M, \kappa_A) : \kappa_A ] = \operatorname{rg}_A(L_i) $$

(A, X, p. 103, Ví dụ 3). Mọi A-môđun hữu hạn sinh đều thừa nhận một giải như vậy (A, X, p. 56, Mệnh đề 10).

#### Mệnh đề 4 {#ac-x-s3-prop-4 .statement}

*Cho A là một vành địa phương Noether, M là một A-môđun hữu hạn sinh, và n là một số nguyên $\geq 0$. Các điều kiện sau là tương đương* :

(i) *ta có* $\operatorname{dp}_A(M) < n$ ;
(ii) *ta có* $\operatorname{Tor}_n^A(M, \kappa_A) = 0$ ;
(iii) *ta có* $\operatorname{Ext}_A^n(M, \kappa_A) = 0$ ;
(iv) *mọi giải xạ ảnh tối thiểu của M đều có độ dài* $< n$.

Các khẳng định (i) $\Rightarrow$ (ii) và (i) $\Rightarrow$ (iii) là ngay lập tức (A, X, p. 100, Định lý 1). Cho L là một giải xạ ảnh tối thiểu của M ; nếu (ii) hoặc (iii) được thỏa mãn, ta có $L_n = 0$ theo (1). Vì mọi giải xạ ảnh tối thiểu của M đều đẳng cấu với L (A, X, p. 54, Mệnh đề 8), suy ra (iv). Hệ quả (iv) $\Rightarrow$ (i) là tầm thường.

#### Hệ quả 1 {#ac-x-s3-prop-4-cor-1 .statement}

*Cho A là một vành địa phương Noether và n là một số nguyên $\geq 0$. Các điều kiện sau là tương đương* :

(i) *ta có* $\operatorname{dh}(A) < n$ ;
(ii) *ta có* $\operatorname{Ext}_A^i(M, N) = 0$ *và* $\operatorname{Tor}_i^A(M, N) = 0$ *với mọi cặp* $(M, N)$ *các A-môđun và mọi số nguyên* $i \geq n$ ;
(iii) *ta có* $\operatorname{Tor}_n^A(\kappa_A, \kappa_A) = 0$ ;
(iv) *ta có* $\operatorname{Ext}_A^n(\kappa_A, \kappa_A) = 0$ ;
(v) *ta có* $\operatorname{dp}_A(\kappa_A) < n$.

Hiển nhiên là (i) kéo theo (ii), và (ii) kéo theo (iii) và (iv). Theo Mệnh đề 4 áp dụng cho A-môđun $\kappa_A$, mỗi điều kiện (iii) và (iv) đều kéo theo (v). Ta hãy chứng minh rằng (v) kéo theo (i) : nếu $\operatorname{dp}_A(\kappa_A) < n$, ta có $\operatorname{Tor}_n^A(M, \kappa_A) = 0$ với mọi A-môđun M ; do đó mọi A-môđun hữu hạn sinh đều có chiều xạ ảnh $< n$ (Mệnh đề 4), điều này kéo theo $\operatorname{dh}(A) < n$ (A, X, p. 138, Mệnh đề 4).

#### Hệ quả 2 {#ac-x-s3-prop-4-cor-2 .statement}

*Ta có* $\operatorname{dh}(A) = \operatorname{dp}_A(\kappa_A)$.

#### Nhận xét 1 {#ac-x-s3-n3-rem-1 .statement}

Cho A là một vành địa phương. A-môđun $\operatorname{Tor}_1^A(\kappa_A, \kappa_A)$ đẳng cấu với $\mathfrak{m}_A / \mathfrak{m}_A^2$ (A, X, p. 72, Ví dụ). Do đó khi A là Noether, để $\operatorname{Tor}_1^A(\kappa_A, \kappa_A)$ bằng không, điều kiện cần và đủ là $\mathfrak{m}_A$ bằng không, nghĩa là A là một trường. Vì vậy Hệ quả 1 kéo theo rằng một vành địa phương Noether có chiều đồng điều 0 là một trường.

#### Nhận xét 2 {#ac-x-s3-n3-rem-2 .statement}

Cho A là một vành địa phương Noether, M là một A-môđun hữu hạn sinh có chiều xạ ảnh hữu hạn $n$, N là một A-môđun hữu hạn sinh khác không. *A-môđun* $\operatorname{Ext}_A^n(M, N)$ *là khác không*: thật vậy, gọi L là một phân giải xạ ảnh cực tiểu của M, và d là vi phân của nó. Ta có một dãy khớp

$$
\operatorname{Hom}_A(L_{n-1}, N) \xrightarrow{\operatorname{Hom}(d_n, 1)} \operatorname{Hom}_A(L_n, N) \longrightarrow \operatorname{Ext}_A^n(M, N) \to 0 .
$$

Vì $d_n \otimes 1_{\kappa_A}$ bằng không, từ đó suy ra, bằng tích tenxơ với $\kappa_A$, một đẳng cấu $\kappa_A \otimes_A \mathrm{Hom}_A(L_n, N) \longrightarrow \kappa_A \otimes_A \mathrm{Ext}_A^n(M, N)$, do đó, có xét đến công thức (1) ở trên,

$$
[\kappa_A \otimes_A \mathrm{Ext}_A^n(M, N) : \kappa_A] = [\mathrm{Ext}_A^n(M, \kappa_A) : \kappa_A][\kappa_A \otimes_A N : \kappa_A],
$$

vế này là khác không theo Mệnh đề 4 và bổ đề Nakayama. Do đó, chiều xạ ảnh của M là số nguyên lớn nhất $i$ sao cho $\mathrm{Ext}_A^i(M, N)$ khác không.

#### Nhận xét 3 {#ac-x-s3-n3-rem-3 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun hữu hạn sinh có chiều xạ ảnh hữu hạn, $N$ là một $A$-môđun hữu hạn sinh mà giá của nó bằng $\mathrm{Spec}(A)$. Theo nhận xét trước và các Mệnh đề 2 và 3 của No. 2, chiều xạ ảnh $n$ của $M$ là số nguyên lớn nhất $i$ sao cho $\mathrm{Ext}_A^i(M, N)$ khác không; giá của $A$-môđun $\mathrm{Ext}_A^n(M, N)$ là tập hợp các phần tử $p$ của $\mathrm{Spec}(A)$ sao cho $\mathrm{dp}_{A_p}(M_p) = n$.

Có thể tồn tại những $A$-môđun hữu hạn sinh $M$ có chiều xạ ảnh $+\infty$, thỏa mãn $\mathrm{Ext}_A^i(M, A) = 0$ với $i$ đủ lớn: *đó chẳng hạn là trường hợp của $A$-môđun $\kappa_A$ khi $A$ là một vành địa phương Gorenstein không chính quy*.

#### Mệnh đề 5 {#ac-x-s3-prop-5 .statement}

*Cho $A$ là một vành Noether, $M$ là một $A$-môđun hữu hạn sinh và $n$ là một số nguyên $\geqslant 0$. Các điều kiện sau là tương đương :

(i) *ta có* $\mathrm{dp}_A(M) < n$ ;
(ii) *với mọi iđêan cực đại* $m$ *của* $A$, *ta có* $\mathrm{Ext}_A^n(M, A/m) = 0$ (resp. *ta có* $\mathrm{Tor}_n^A(M, A/m) = 0$) ;
(iii) *với mọi iđêan cực đại* $m$ *của* $A$, *ta có* $\mathrm{Ext}_{A_m}^n(M_m, A/m) = 0$ (resp. *ta có* $\mathrm{Tor}_n^{A_m}(M_m, A/m) = 0$).

(i) $\Rightarrow$ (ii) : điều này là hiển nhiên.
(ii) $\Rightarrow$ (iii) : điều này suy ra từ Mệnh đề 2 của No. 2.
(iii) $\Rightarrow$ (i) : theo Mệnh đề 4, điều kiện (iii) kéo theo bất đẳng thức $\mathrm{dp}_{A_m}(M_m) < n$ với mọi iđêan cực đại $m$ của $A$, và kết luận theo Mệnh đề 3.

#### Nhận xét 4 {#ac-x-s3-n3-rem-4 .statement}

Cho $A$ là một vành Noether và $n$ là một số nguyên $\geqslant 0$. Nếu $m$ và $m'$ là hai iđêan cực đại phân biệt của $A$, các $A$-môđun $\mathrm{Ext}_A^n(A/m, A/m')$ và $\mathrm{Tor}_n^A(A/m, A/m')$ bị triệt tiêu bởi $m + m'$, do đó bằng không. Bằng một chứng minh tương tự như chứng minh của Hệ quả 1 của Mệnh đề 4, từ Mệnh đề 5 người ta suy ra tính tương đương của các điều kiện sau:

(i) *ta có* $\mathrm{dh}(A) < n$ ;
(ii) *ta có* $\mathrm{Ext}_A^i(M, N) = 0$ *và* $\mathrm{Tor}_i^A(M, N) = 0$ *đối với mọi cặp* $(M, N)$ *gồm các* $A$-*môđun và mọi số nguyên* $i \geqslant n$ ;
(iii) *ta có* $\mathrm{Tor}_n^A(A/m, A/m) = 0$ *với mọi iđêan cực đại* $m$ *của* $A$ ;
(iv) *ta có* $\mathrm{Ext}_A^n(A/m, A/m) = 0$ *với mọi iđêan cực đại* $m$ *của* $A$ ;
(v) *ta có* $\mathrm{dp}_A(A/m) < n$ *với mọi iđêan cực đại* $m$ *của* $A$.

Đặc biệt, ta có $\mathrm{dh}(A) = \sup_m \mathrm{dp}_A(A/m)$, trong đó $m$ chạy qua tập hợp các iđêan cực đại của $A$.

#### Mệnh đề 6 {#ac-x-s3-prop-6 .statement}

Cho $A$ là một vành Noether, $N$ là một $A$-môđun, $n$ là một số nguyên $\geqslant 0$. Các điều kiện sau là tương đương:

(i) ta có $\operatorname{di}_A(N) < n$ ;
(ii) với mọi iđêan nguyên tố $p$ của $\Lambda$, ta có $\operatorname{Ext}_A^n(\Lambda/p, N) = 0$ ;
(iii) với mọi iđêan nguyên tố $p$ của $A$, ta có $\operatorname{Ext}_{A_p}^n(\kappa(p), N_p) = 0$.

Hơn nữa, nếu $A$-môđun $N$ là hữu hạn kiểu, thì các điều kiện này tương đương với:

(iv) với mọi iđêan cực đại $m$ của $A$, ta có $\operatorname{Ext}_A^i(A/m, N) = 0$ với $n \leqslant i \leqslant n + \operatorname{ht}(m)$.

Chú ý rằng điều kiện (iii) tương đương với

(iii') với mọi iđêan nguyên tố $p$ của $A$, ta có $\operatorname{Ext}_A^n(A/p, N) \otimes_A \kappa(p) = 0$.

Thật vậy, vì $\operatorname{Ext}_A^n(A/p, N)$ bị triệt tiêu bởi $p$, nên $A$-môđun $\operatorname{Ext}_A^n(A/p, N) \otimes_A \kappa(p)$ đẳng cấu với $\operatorname{Ext}_A^n(A/p, N) \otimes_A A_p$, do đó đẳng cấu với $\operatorname{Ext}_{A_p}^n(\kappa(p), N_p)$ (No. 2, Mệnh đề 2).

Các suy ra (i) $\Rightarrow$ (ii) và (i) $\Rightarrow$ (iv) là hệ quả của Mệnh đề 1 của No. 1, và suy ra (ii) $\Rightarrow$ (iii') là hiển nhiên.

(iii) $\Rightarrow$ (i): với mọi $A$-môđun $M$, đặt $T(M) = \operatorname{Ext}_A^n(M, N)$. Giả sử rằng (i) không được thỏa mãn. Khi đó tồn tại (No. 1, Mệnh đề 1) một iđêan $a$ của $A$ sao cho $T(A/a) \neq 0$. Gọi $p$ là một iđêan của $A$ cực đại trong số các iđêan có tính chất này; hãy chứng minh rằng $p$ là nguyên tố. Theo IV, § 1, No. 4, Định lý 1 và Định lý 2, tồn tại một dãy hợp thành $(M_i)_{0 \leqslant i \leqslant m}$ của $A/p$ sao cho mỗi thương $M_i/M_{i+1}$ đẳng cấu với một môđun $A/p_i$, trong đó $p_i$ ($0 \leqslant i \leqslant m-1$) là một iđêan nguyên tố chứa $p$. Nếu $T(A/p_i)$ bằng không với mọi $i$, thì người ta sẽ suy ra bằng quy nạp theo $i$ từ các dãy khớp

$$
T(M_0/M_i) \longrightarrow T(M_0/M_{i+1}) \longrightarrow T(M_i/M_{i+1})
$$

rằng $T(M_0/M_m) = T(A/p)$ bằng không, điều này không đúng. Vậy nên tồn tại một chỉ số $i$ sao cho $T(A/p_i) \neq 0$. Do tính cực đại của $p$, ta có $p = p_i$, nên $p$ là nguyên tố.

Gọi $x$ là một phần tử của $A - p$; từ dãy khớp

$$
0 \to A/p \xrightarrow{x_{A/p}} A/p \to A/(p + xA) \to 0
$$

suy ra một dãy khớp

$$
T(A/(p + xA)) \longrightarrow T(A/p) \xrightarrow{u} T(A/p),
$$

trong đó $u = \operatorname{Ext}_A^n(x_A, 1_N) = x_{T(A/p)}$ (A, X, p. 89, Mệnh đề 6). Do tính cực đại của $p$, ta có $T(A/(p + xA)) = 0$, vì thế đồng cấu $u$ là đơn ánh. Vậy $A/p$-môđun khác không $T(A/p)$ là không xoắn. Điều này kéo theo $T(A/p) \otimes_A \kappa(p)$ khác không (A, II, p. 117, Hệ quả 1), điều mâu thuẫn với (iii').

Giả sử $A$-môđun $N$ là kiểu hữu hạn, và hãy chứng minh rằng (iv) kéo theo (iii). Gọi $p$ là một iđêan nguyên tố của $A$ và $m$ là một iđêan cực đại của $A$ chứa $p$. Tồn tại một chuỗi bão hòa các iđêan nguyên tố của $A$ với hai đầu mút là $\mathfrak{p}$ và $\mathfrak{m}$. Độ dài $r$ của chuỗi này nhỏ hơn $\mathrm{ht}(\mathfrak{m})$; dưới giả thiết (iv), do đó ta có
$$
\mathrm{Ext}_{A_{\mathfrak{m}}}^{n+r}(\kappa(\mathfrak{m}), N_{\mathfrak{m}}) = \mathrm{Ext}_{A}^{n+r}(A/\mathfrak{m}, N) \otimes_{A} A_{\mathfrak{m}} = 0 .
$$
Khi đó suy ra từ Bổ đề 3 của § 1, No. 7 rằng ta có $\mathrm{Ext}_{A_{\mathfrak{p}}}^{n}(\kappa(\mathfrak{p}), N_{\mathfrak{p}}) = 0$, điều này chứng minh (iii).

#### Nhận xét 5 {#ac-x-s3-n3-rem-5 .statement}

Cho $N$ là một $A$-môđun sinh hữu hạn; điều kiện $\mathrm{Ext}_{A}^{n}(A/\mathfrak{m}, N) = 0$ với mọi iđêan cực đại $\mathfrak{m}$ của $A$ không nhất thiết kéo theo $\mathrm{di}_{A}(N) < n$. Chẳng hạn, nếu vành $A$ là địa phương và không phải là một vành Gorenstein (No. 7, Định nghĩa 1), thì ta có $\mathrm{Ext}_{A}^{n}(A/\mathfrak{m}, A) = 0$ với $n < \mathrm{prof}(A)$ nhưng $\mathrm{di}_{A}(A) = +\infty$.

### 4. Thương theo một phần tử giản ước được

Trong số này, $A$ ký hiệu một vành và $x$ một phần tử của $A$ *giản ước được*.

Cho $M$ là một $A$-môđun và $p : P \to M$ một phân giải xạ ảnh của $M$. Theo A, X, p. 101, hệ quả của định lý 1, $H_{n}(P/xP)$ được đồng nhất với $\mathrm{Tor}_{n}^{A}(M, A/xA)$, và do đó đẳng cấu với $M/xM$ nếu $n = 0$, với $\mathrm{Ker}(x_{M})$ nếu $n = 1$, và bằng không trong các trường hợp khác (*đd.*, p. 102, Ví dụ 1). Xét các phức của các $(A/xA)$-môđun $R$ và $R'$ sao cho
$$
\begin{aligned}
R_{n} & = P_{n}/xP_{n} & R'_{n} & = 0 & \text{với } n \geqslant 2, \\
R_{1} & = Z_{1}(P/xP) & R'_{1} & = (P_{1}/xP_{1})/R_{1}, \\
R_{n} & = 0 & R'_{n} & = P_{n}/xP_{n} & \text{với } n \leqslant 0,
\end{aligned}
$$
và các vi phân của chúng được suy ra từ vi phân của $P$. Các phức $R(1)$ và $R'$ lần lượt là các phân giải trái của $\mathrm{Ker}(x_{M})$ và $M/xM$, và ta có một dãy khớp các phức
$$
0 \to R \to P/xP \to R' \to 0 .
$$

Tương tự, cho $e : M \to E$ là một phân giải đơn ánh của $M$; ký hiệu $K$ là phức $\mathrm{Ker}(x_{E})$. Theo A, X, p. 101, hệ quả của định lý 1, $H_{n}(K)$ được đồng nhất với $\mathrm{Ext}_{A}^{n}(A/xA, M)$, và do đó đẳng cấu với $\mathrm{Ker}(x_{M})$ nếu $n = 0$, với $M/xM$ nếu $n = 1$, và bằng không trong các trường hợp khác (*đd.*, p. 102, Ví dụ 1). Từ $E$ ta suy ra các phức của các $(A/xA)$-môđun $S$ và $S'$ sao cho
$$
\begin{aligned}
S^{n} & = K^{n} & {S'}^{n} & = 0 & \text{với } n \leqslant 0, \\
S^{1} & = B^{1}(K) & {S'}^{1} & = K^{1}/S^{1}, \\
S^{n} & = 0 & {S'}^{n} & = K^{n} & \text{với } n \geqslant 2.
\end{aligned}
$$
Các phức $S$ và $S'(-1)$ lần lượt là các phân giải phải của $\mathrm{Ker}(x_{M})$ và $M/xM$, và ta có một dãy khớp các phức
$$
0 \to S \to \mathrm{Ker}(x_{E}) \to S' \to 0 .
$$

Cho $N$ là một $(A/xA)$-môđun, và $e' : N \to E'$ một phân giải đơn ánh của $N$. Từ dãy khớp (2) ta suy ra một dãy khớp các phức của các $(A/xA)$-môđun
$$
0 \to \mathrm{Homgr}_{A/xA}(R', E') \to \mathrm{Homgr}_{A/xA}(P/xP, E') \to \mathrm{Homgr}_{A/xA}(R, E') \to 0 .
$$

Xét dãy đồng điều khớp gắn với dãy khớp này. Theo A, X, p. 100, định lý 1, với mọi số nguyên $n \geqslant 0$ ta có các đẳng cấu

$$
H^n(\mathrm{Homgr}_{\Lambda/xA}(R', E')) \longrightarrow \mathrm{Ext}^n_{A/xA}(M/xM, N)
$$
$$
H^n(\mathrm{Homgr}_{\Lambda/xA}(P/xP, E')) \longrightarrow H^n(\mathrm{Homgr}_A(P, E')) \longrightarrow \mathrm{Ext}^n_A(M, N)
$$
$$
H^n(\mathrm{Homgr}_{A/xA}(R, E')) = H^{n-1}(\mathrm{Homgr}_{A/xA}(R(1), E')) \longrightarrow \mathrm{Ext}^{n-1}_{A/xA}(\mathrm{Ker}(x_M), N)
$$

do đó có một dãy khớp dài các $(A/xA)$-môđun

$$
\ldots \longrightarrow \mathrm{Ext}^n_{A/xA}(M/xM, N) \longrightarrow \mathrm{Ext}^n_A(M, N) \longrightarrow \mathrm{Ext}^{n-1}_{A/xA}(\mathrm{Ker}(x_M), N)
$$
$$
\longrightarrow \mathrm{Ext}^{n+1}_{A/xA}(M/xM, N) \longrightarrow \mathrm{Ext}^{n+1}_A(M, N) \longrightarrow \ldots
$$

(4)

Tương tự, cho $p' : P' \to N$ là một phân giải xạ ảnh của $(\Lambda/xA)$-môđun $N$. Từ dãy khớp (3) suy ra một dãy khớp các phức của các $(A/xA)$-môđun

$0 \to \mathrm{Homgr}_{A/xA}(P', S) \longrightarrow \mathrm{Homgr}_{A/xA}(P', \mathrm{Ker}(x_E)) \longrightarrow \mathrm{Homgr}_{A/xA}(P', S') \to 0$.

Xét theo đẳng cấu $\mathrm{Homgr}_{A/xA}(P', \mathrm{Ker}(x_E)) \longrightarrow \mathrm{Homgr}_A(P', E)$, dãy đồng điều khớp liên kết có thể được viết

$$
\ldots \longrightarrow \mathrm{Ext}^n_{A/xA}(N, \mathrm{Ker}(x_M)) \longrightarrow \mathrm{Ext}^n_A(N, M) \longrightarrow \mathrm{Ext}^{n-1}_{A/xA}(N, M/xM)
$$
$$
\longrightarrow \mathrm{Ext}^{n+1}_{A/xA}(N, \mathrm{Ker}(x_M)) \longrightarrow \mathrm{Ext}^{n+1}_A(N, M) \longrightarrow \ldots
$$

(5)

Cuối cùng, xét dãy khớp các phức của các $(A/xA)$-môđun

$0 \to R \otimes_{A/xA} P' \longrightarrow (P/xP) \otimes_{A/xA} P' \longrightarrow R' \otimes_{A/xA} P' \to 0$

suy ra từ dãy khớp (2); xét theo đẳng cấu $P \otimes_A P' \longrightarrow (P/xP) \otimes_{A/xA} P'$, dãy đồng điều khớp liên kết có thể được viết

$$
\ldots \longrightarrow \mathrm{Tor}^A_n(M, N) \longrightarrow \mathrm{Tor}^{A/xA}_n(M/xM, N) \longrightarrow \mathrm{Tor}^{A/xA}_{n-2}(\mathrm{Ker}\ x_M, N)
$$
$$
\longrightarrow \mathrm{Tor}^A_{n-1}(M, N) \longrightarrow \mathrm{Tor}^{A/xA}_{n-1}(M/xM, N) \longrightarrow \ldots
$$

(6)

#### Mệnh đề 7 {#ac-x-s3-prop-7 .statement}

*Cho $A$ là một vành, $x$ là một phần tử giản ước được của $A$, $M$ là một $A$-môđun sao cho phép vị tự $x_M$ là đơn ánh, $N$ là một $A$-môđun bị triệt tiêu bởi $x$, $n$ là một số nguyên. Các đồng cấu chính tắc của các $(A/xA)$-môđun*

$$
\mathrm{Ext}^n_{A/xA}(M/xM, N) \longrightarrow \mathrm{Ext}^n_A(M, N),
$$
$$
\mathrm{Ext}^n_A(N, M) \longrightarrow \mathrm{Ext}^{n-1}_{A/xA}(N, M/xM),
$$
$$
\mathrm{Tor}^A_n(M, N) \longrightarrow \mathrm{Tor}^{A/xA}_n(M/xM, N)
$$

*suy ra từ các dãy khớp (4), (5) và (6) là các đẳng cấu.*

#### Hệ quả {#ac-x-s3-n4-cor-1 .statement}

Cho $A$ là một vành địa phương Noether, $M$ là một $A$-môđun sinh hữu hạn và $J$ là một iđêan của $A$ sinh bởi một dãy $(x_1, \ldots, x_r)$ các phần tử của $m_A$ vừa là $A$-chính quy vừa là $M$-chính quy. Khi đó $\mathrm{dp}_{A/J}(M/JM) = \mathrm{dp}_A(M)$ và $\mathrm{di}_{A/J}(M/JM) = \mathrm{di}_A(M) - r$.

Chỉ cần xét trường hợp $r = 1$. Đặt $x = x_1$. Các $A$-môđun $\mathrm{Ext}^n_{A/xA}(M/xM, \kappa_A)$ và $\mathrm{Ext}^n_A(M, \kappa_A)$ đẳng cấu với nhau với mọi số nguyên $n$ (mệnh đề 7); đẳng thức $\mathrm{dp}_{A/xA}(M/xM) = \mathrm{dp}_A(M)$ suy ra từ mệnh đề 4 của No. 3. Tương tự, các $A$-môđun $\mathrm{Ext}^{n-1}_{A/xA}(\kappa_A, M/xM)$ và $\mathrm{Ext}^n_A(\kappa_A, M)$ đẳng cấu với nhau với mọi số nguyên $n$, và đẳng thức $\mathrm{di}_{A/xA}(M/xM) = \mathrm{di}_A(M) - 1$ suy ra từ mệnh đề 6 của No. 3.

### 5. Chiều sâu và chiều xạ ảnh

#### Định lý 1 (Auslander-Buchsbaum) {#ac-x-s3-thm-1 .statement}

Cho $A$ là một vành địa phương Noether và $M$ là một $A$-môđun sinh hữu hạn có chiều xạ ảnh hữu hạn. Khi đó có đẳng thức

$$
\mathrm{dp}_A(M) + \mathrm{prof}_A(M) = \mathrm{prof}(A)
$$

Lập luận bằng quy nạp theo $\mathrm{dp}_A(M)$.

a) Nếu $\mathrm{dp}_A(M)$ bằng không, thì $M$ là một $A$-môđun tự do sinh hữu hạn khác không; độ sâu của nó bằng $\mathrm{prof}(A)$ (§ 1, No. 1, nhận xét 4).

b) Giả sử $\mathrm{dp}_A(M) = 1$ và chọn một phân giải xạ ảnh cực tiểu

$$
0 \to L_1 \xrightarrow{d_1} L_0 \xrightarrow{d_0} M \to 0
$$

của $M$ (No. 3, mệnh đề 4, (iv)). Các $A$-môđun $L_0$ và $L_1$ là các môđun tự do sinh hữu hạn khác không, nên có độ sâu bằng $\mathrm{prof}(A)$ (§ 1, No. 1, nhận xét 4). Ánh xạ $1_{\kappa_A} \otimes d_1 : \kappa_A \otimes_A L_1 \to \kappa_A \otimes_A L_0$ bằng không, điều này kéo theo $d_1$ thuộc $m_A \mathrm{Hom}_A(L_1, L_0)$. Theo nhận xét 5 của § 1, No. 1, ta có $\mathrm{prof}_A(M) = \mathrm{prof}(A) - 1$.

c) Giả sử $\mathrm{dp}_A(M) > 1$. Chọn một dãy khớp

$$
0 \to N \to L \to M \to 0
$$

trong đó $L$ là một $A$-môđun tự do sinh hữu hạn. Khi đó ta có $\mathrm{prof}_A(L) = \mathrm{prof}(A)$ (§ 1, No. 1, nhận xét 4), $\mathrm{dp}_A(N) = \mathrm{dp}_A(M) - 1$ (A, X, p. 135, hệ quả 2 c)), do đó $\mathrm{prof}_A(N) = \mathrm{prof}(A) - \mathrm{dp}_A(N)$ (giả thiết quy nạp), và đặc biệt $\mathrm{prof}_A(N) < \mathrm{prof}_A(L)$. Theo mệnh đề 1 của § 1, No. 1, khi đó ta có $\mathrm{prof}_A(M) = \mathrm{prof}_A(N) - 1$, điều này hoàn tất chứng minh.

#### Nhận xét {#ac-x-s3-n5-rem-1 .statement}

Xét theo hệ quả 2 của mệnh đề 4 (No. 3), định lý 1 áp dụng cho $A$-môđun $\kappa_A$ kéo theo rằng xảy ra một trong hai trường hợp sau:

(i) ta có $\mathrm{dp}_A(\kappa_A) = \mathrm{dh}(A) = +\infty$ ;
(ii) ta có $\mathrm{dp}_A(\kappa_A) = \mathrm{dh}(A) = \mathrm{prof}(A) < +\infty$.

Ta sẽ thấy sau này (§ 4, No. 2) rằng (ii) đặc trưng các vành địa phương chính quy.

#### Hệ quả 1 {#ac-x-s3-thm-1-cor-1 .statement}

Giữ các giả thiết của định lý 1.

a) Ta có $dp_A(M) \leq \operatorname{prof}(\Lambda)$. Để có đẳng thức, điều kiện cần và đủ là iđêan cực đại $m_A$ liên kết với $M$.

b) Ta có $\operatorname{prof}_A(M) \leq \operatorname{prof}(\Lambda)$. Để có đẳng thức, điều kiện cần và đủ là $M$ tự do.

a) Thực vậy, “ $\operatorname{prof}_A(M) = 0$ ” tương đương với “ $m_A \in \operatorname{Ass}(A)$ ” ($§ 1$, No. 1, nhận xét 2).

b) Thực vậy, “ $dp_A(M) = 0$ ” tương đương với “ $M$ tự do ”.

HỆ QUẢ 2.: Giữ các giả thiết của định lý 1 và giả sử thêm rằng $A$ là một vành Macaulay. Khi đó $dp_A(M)$ là tổng của hai số nguyên dương $\dim(A) - \dim_A(M)$ và $\dim_A(M) - \operatorname{prof}(M)$.

Đặc biệt, khi đó $dp_A(M)$ lớn hơn $\dim(A) - \dim_A(M)$, và có đẳng thức khi và chỉ khi $M$ là Cohen-Macaulay.

#### Hệ quả 3 {#ac-x-s3-thm-1-cor-3 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun sinh hữu hạn có chiều xạ ảnh hữu hạn, $i$ là một số nguyên $\geq 0$, $N$ là một $A$-môđun sinh hữu hạn, và $F$ là giá đỡ của $A$-môđun $\operatorname{Ext}_A^i(M, N)$ (resp. $\operatorname{Tor}_i^\Lambda(M, N)$). Khi đó $\operatorname{prof}_F(\Lambda) \geq i$.

Thật vậy, cho $p \in F$. Ta có $\operatorname{Ext}_A^i(M_p, N_p) \neq 0$ (resp. $\operatorname{Tor}_i^\Lambda(M_p, N_p) \neq 0$) theo mệnh đề 2 của No. 2, do đó $i \leq dp_{A_p}(M_p) \leq dp_A(M) < +\infty$ (No. 2, mệnh đề 3). Định lý 1 suy ra $\operatorname{prof}(A_p) \geq i$. Do đó ($§ 1$, No. 5, mệnh đề 8)

$$
\operatorname{prof}_F(\Lambda) = \inf_{p \in F} \operatorname{prof}(A_p) \geq i .
$$

Với thuật ngữ của $§ 1$, No. 5, nhận xét 4, kết luận của hệ quả 3 có nghĩa là các môđun $\operatorname{Ext}_\Lambda^i(M, N)$ và $\operatorname{Tor}_i^\Lambda(M, N)$ có grade $\geq i$. Điều đó suy ra rằng đối chiều của giá của chúng trong $\operatorname{Spec}(A)$ là $\geq i$ ($§ 1$, No. 7, mệnh đề 12).

#### Hệ quả 4 {#ac-x-s3-thm-1-cor-4 .statement}

Cho $A$ là một vành Macaulay Noether và $M$ là một $A$-môđun sinh hữu hạn có chiều xạ ảnh hữu hạn.

a) Cho $p \in \operatorname{Spec}(\Lambda)$; ký hiệu bởi $\mathscr{C}(p)$ tập hợp các thành phần bất khả quy của $\operatorname{Supp}(M)$ chứa $p$. Ta có

$$
\dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p) = dp_{A_p}(M_p) - \inf_{X \in \mathscr{C}(p)} \operatorname{codim}(X, \operatorname{Spec}(A)) .
$$

b) Ánh xạ $p \mapsto \dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p)$ từ $\operatorname{Spec}(A)$ vào $\overline{\mathbf{Z}}$ là nửa liên tục trên.

c) Tập hợp các iđêan nguyên tố $p$ của $\Lambda$ sao cho $A_p$-môđun $M_p$ là Macaulay là mở và trù mật trong $\operatorname{Spec}(\Lambda)$. Giao của nó với $\operatorname{Supp}(M)$ là trù mật trong $\operatorname{Supp}(M)$.

a) Ta có thể giả sử rằng $p \in \operatorname{Supp}(M)$. Đặt $\varphi(p) = \dim(A_p) - \dim_{A_p}(M_p)$. Theo hệ quả 2 ở trên, ta có

$$
\dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p) = dp_{A_p}(M_p) - \varphi(p) .
$$

Vì $A$ là một vành Macaulay, ta có

$$
\dim(A_p) = \operatorname{codim}(V(p), \operatorname{Spec}(A)) = \operatorname{codim}(V(p), X) + \operatorname{codim}(X, \operatorname{Spec}(A))
$$

$$
\dim_{\Lambda_p}(M_p) = \operatorname{codim}(V(p), \operatorname{Supp}(M)) = \sup_{X \in \mathcal{C}(p)} \operatorname{codim}(V(p), X)
$$

và do đó

$$
\varphi(p) = \inf_{X \in \mathcal{C}(p)} \operatorname{codim}(X, \operatorname{Spec}(A)) .
$$

b) Cho $p \in \operatorname{Spec}(A)$, và cho $F$ là hợp của các thành phần bất khả quy của $\operatorname{Supp}(M)$ không chứa $p$. Với mọi phần tử $q$ của $\operatorname{Spec}(A) - F$, ta có $\mathcal{C}(q) \subset \mathcal{C}(p)$, do đó $\varphi(q) \geq \varphi(p)$ theo công thức trên. Do đó hàm $\varphi$ là nửa liên tục dưới; mệnh đề b) khi đó suy ra từ mệnh đề 3 của No. 2.

c) Cho $U$ là tập hợp các phần tử $p$ của $\operatorname{Spec}(A)$ sao cho $M_p$ là Cohen-Macaulay. Điều kiện $p \in U$ tương đương với $\dim(M_p) - \operatorname{prof}(M_p) \leq 0$, do đó $U$ là mở theo b). Vì $U$ chứa $\operatorname{Spec}(A) - \operatorname{Supp}(M)$, chỉ cần chứng minh rằng $U \cap \operatorname{Supp}(M)$ là trù mật trong $\operatorname{Supp}(M)$. Với mọi iđêan nguyên tố cực tiểu $p$ của $\operatorname{Supp}(M)$, $A_p$-môđun $M_p$ có độ dài hữu hạn (IV, § 2, No. 5, Hệ quả 2 của Mệnh đề 7 và § 1, No. 3, Hệ quả 1 của Mệnh đề 7), nên là Cohen-Macaulay; do đó $U$ giao với mọi thành phần bất khả quy của $\operatorname{Supp}(M)$. Kết luận theo Mệnh đề 1 của II, § 4, No. 1.

### 6. Độ sâu và chiều đơn ánh

#### Mệnh đề 8 {#ac-x-s3-prop-8 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun sinh hữu hạn. Khi đó $\dim_A(M) \leq \operatorname{di}_A(M)$.

Cho $r$ là một số nguyên dương nhỏ hơn $\dim_A(M)$. Tồn tại một chuỗi bão hòa các iđêan nguyên tố $p \subset p_1 \subset \ldots \subset p_{r-1} \subset q$ sao cho $p$ là một phần tử cực tiểu của giá của $M$; khi đó $A_p$-môđun $M_p$ có độ dài hữu hạn, nên $\operatorname{Hom}_{A_p}(\kappa(p), M_p) \neq 0$, do đó $\operatorname{Ext}^r_{A_q}(\kappa(q), M_q) \neq 0$ (§ 1, No. 7, Bổ đề 3), điều này kéo theo $\operatorname{di}_A(M) \geq r$ (No. 3, Mệnh đề 6).

#### Mệnh đề 9 {#ac-x-s3-prop-9 .statement}

Cho $A$ là một vành địa phương Noether và $M$ là một $A$-môđun khác không sinh hữu hạn có chiều đơn ánh hữu hạn. Khi đó $\operatorname{di}_A(M) = \operatorname{prof}(A)$.

Đặt $r = \operatorname{di}_A(M)$. Ta có $\operatorname{Ext}^i_A(\kappa_A, M) = 0$ với $i > r$, nên $\operatorname{Ext}^r_A(\kappa_A, M) \neq 0$ theo Mệnh đề 6 của No. 3, (iv) $\Rightarrow$ (i). Gọi $s$ là độ sâu của $A$ và cho $(x_1, \ldots, x_s)$ là một dãy chính quy trên $A$ gồm các phần tử của $\mathfrak{m}_A$ (§ 1, No. 4, Định lý 2); đặt $N = A/(x_1A + \ldots + x_sA)$. Theo ví dụ ở No. 1, ta có $\operatorname{dp}_A(N) = s$ và $\operatorname{Ext}^s_A(N, M) \neq 0$, nên $s \leq \operatorname{di}_A(M) = r$. Nhưng $N$ có độ sâu 0 (§ 1, No. 4, Mệnh đề 7), nên tồn tại một dãy khớp các $A$-môđun

$$
0 \to \kappa_A \to N \to N' \to 0 .
$$

Từ đó suy ra một dãy khớp các môđun mở rộng

$$
\operatorname{Ext}^r_A(N, M) \to \operatorname{Ext}^r_A(\kappa_A, M) \to \operatorname{Ext}^{r+1}_A(N', M) ;
$$

vì $\operatorname{Ext}^{r+1}_A(N', M) = 0$ và $\operatorname{Ext}^r_A(\kappa_A, M) \neq 0$, suy ra $\operatorname{Ext}^r_A(N, M) \neq 0$, do đó $r \leq \operatorname{dp}_A(N) = s$. Cuối cùng, ta có $r = s$, điều này hoàn tất chứng minh.

### 7. Các vành Gorenstein

#### Định nghĩa 1 {#ac-x-s3-def-1 .statement}

Một vành $A$ được gọi là một vành Gorenstein nếu nó là Noether và nếu $A_m$-môđun $A_m$ có chiều đơn ánh hữu hạn đối với mọi iđêan cực đại $m$ của $A$.

Để một vành địa phương Noether $A$ là một vành Gorenstein, điều kiện cần và đủ là $\mathrm{di}_A(A)$ hữu hạn; để một vành Noether $A$ là một vành Gorenstein, điều kiện cần và đủ là điều này đúng với $A_m$ đối với mọi iđêan cực đại $m$ của $A$.

#### Mệnh đề 10 {#ac-x-s3-prop-10 .statement}

Cho $A$ là một vành Gorenstein; khi đó $A$ là một vành Macaulay, và thỏa mãn $\mathrm{di}_A(A) = \dim(A)$.

Đối với mọi iđêan cực đại $m$ của $A$, ta có
$$
\begin{align*}
\dim(A_m) &\leq \mathrm{di}_{A_m}(A_m) & (\text{No. } 6, \text{Prop. } 8) \\
\mathrm{di}_{A_m}(A_m) &= \mathrm{prof}(A_m) & (\text{No. } 6, \text{Prop. } 9) \\
\mathrm{prof}(A_m) &\leq \dim(A_m) & (§ 1, \text{No. } 4, \text{Cor. } 2 \text{ of Th. } 2) ;
\end{align*}
$$
suy ra $A$ là một vành Macaulay, và $\mathrm{di}_A(A) = \dim(A)$ khi chuyển qua cận trên bé nhất (No. 2, Prop. 3).

Do đó các vành Noether $A$ sao cho $\mathrm{di}_A(A)$ hữu hạn là các vành Gorenstein hữu hạn chiều (Prop. 3 of No. 2), và các vành Noether sao cho $A$-môđun $A$ là đơn ánh là các vành Gorenstein Artin.

#### Ví dụ 1 {#ac-x-s3-n7-exa-1 .statement}

Đối với mọi tập con nhân $S$ của một vành Gorenstein $A$, vành phân thức $S^{-1}A$ là một vành Gorenstein: thật vậy, cho $q$ là một iđêan cực đại của $S^{-1}A$; nó có dạng $S^{-1}p$, trong đó $p$ là một iđêan nguyên tố của $A$ không giao với $S$. Cho $m$ là một iđêan cực đại của $A$ chứa $p$; khi đó vành $B = (S^{-1}A)_q$ đẳng cấu với $A_p$ (II, § 2, No. 5, Prop. 11), do đó đẳng cấu với một vành phân thức của $A_m$, và vì thế thỏa mãn $\mathrm{di}_B(B) < +\infty$ (No. 2, Cor. 1 of Prop. 3).

#### Ví dụ 2 {#ac-x-s3-n7-exa-2 .statement}

Cho $A$ là một vành Gorenstein và cho $J$ là một iđêan của $A$, được sinh bởi một dãy $A$-chính quy $x$. Vành thương $A/J$ là một vành Gorenstein: thật vậy, đối với mọi iđêan cực đại $m$ của $A$ chứa $J$, ảnh của dãy $x$ trong $A_m$ là $A_m$-chính quy và sinh iđêan $J_m$, do đó $A_m/J_m$ là một vành Gorenstein theo Cor. of Prop. 7 (No. 4).

#### Ví dụ 3 {#ac-x-s3-n7-exa-3 .statement}

Cho $A$ là một vành địa phương Noether, $J$ là một iđêan của $A$ được sinh bởi một dãy $A$-chính quy gồm các phần tử của $m_A$. Nếu $A/J$ là một vành Gorenstein, thì điều tương tự cũng đúng với $A$ (No. 4, Cor. of Prop. 7).

#### Ví dụ 4 {#ac-x-s3-n7-exa-4 .statement}

Cho $A$ là một vành địa phương Noether chính quy; khi đó $A$ là một vành Gorenstein. Thật vậy, gọi $x$ là một hệ tọa độ của $A$ (VIII, § 5, No. 1, Def. 1). Dãy $x$ là $A$-chính quy (*loc. cit.*, No. 2, định lý 1) và sinh iđêan $m_A$; do đó có thể áp dụng Ví dụ 3.

#### Ví dụ 5 {#ac-x-s3-n7-exa-5 .statement}

Mọi vành thương của một miền iđêan chính đều là một vành Gorenstein (Ví dụ 2). Đặc biệt, mọi đại số đơn sinh trên một trường đều là một vành Gorenstein.

#### Bổ đề 1 {#ac-x-s3-lem-1 .statement}

Cho $A$ là một vành địa phương Artin. Các điều kiện sau là tương đương:

(i) $A$ là một vành Gorenstein;
(ii) A-môđun $A$ là đơn ánh;
(iii) không gian vectơ $\mathrm{Hom}_A(\kappa_A, A)$ trên $\kappa_A$ có chiều 1.

Nhắc lại (A, VIII, p. 3.5) rằng $A$ có một iđêan cực tiểu khác không; một iđêan như vậy là một môđun đơn, nên đẳng cấu với $\kappa_A$. Do đó không gian vectơ $\mathrm{Hom}_A(\kappa_A, A)$ trên $\kappa_A$ là khác không; nói rằng nó có chiều 1 có nghĩa là $A$ chỉ chứa một iđêan cực tiểu khác không, và vì thế đó là đế của $A$ (A, VIII, § 4, No. 6).

Tính tương đương của (i) và (ii) đã được chứng minh sau Mệnh đề 10. Giả sử A-môđun $A$ là đơn ánh. Gọi $x$ và $y$ là hai phần tử khác không của $A$ bị $m_A$ triệt tiêu. Tồn tại duy nhất một ánh xạ $A$-tuyến tính $\varphi : Ax \to A$ sao cho $\varphi(x) = y$; vì $A$ là đơn ánh, nó kéo dài thành một tự đồng cấu của $A$, điều này kéo theo $y$ thuộc $Ax$, do đó có (iii).

Ngược lại, giả sử $\mathrm{Hom}_A(\kappa_A, A)$ có chiều 1. Gọi $M$ là một $A$-môđun sinh hữu hạn; nó có độ dài hữu hạn, nên có một chuỗi hợp thành mà các thương đều đẳng cấu với $\kappa_A$. Suy ra bằng quy nạp theo độ dài của $M$ bất đẳng thức $\mathrm{long}_A(\mathrm{Hom}_A(M, A)) \leqslant \mathrm{long}_A(M)$. Trong dãy khớp của các môđun mở rộng

$$
0 \to \mathrm{Hom}_A(\kappa_A, A) \to \mathrm{Hom}_A(A, A) \xrightarrow{\alpha} \mathrm{Hom}_A(m_A, A) \to \mathrm{Ext}_A^1(\kappa_A, A) \to 0 ,
$$

do đó có $\mathrm{long}_A(\mathrm{Hom}_A(m_A, A)) \leqslant \mathrm{long}_A(m_A) = \mathrm{long}(A) - 1 = \mathrm{long}_A(\mathrm{Im}\, \alpha)$. Do đó $\alpha$ là toàn ánh, $\mathrm{Ext}_A^1(\kappa_A, A)$ bằng không và A-môđun $A$ là đơn ánh (No. 3, Prop. 4).

#### Bổ đề 2 {#ac-x-s3-lem-2 .statement}

Cho $A$ là một vành địa phương Noether sao cho $\mathrm{di}_A(A) = +\infty$. Khi đó $\mathrm{Ext}_A^i(\kappa_A, A) \neq 0$ với mọi số nguyên $i \geqslant \dim(A)$.

Ta lập luận bằng quy nạp theo $\dim(A)$. Khi $\dim(A) = 0$, $m_A$ là iđêan nguyên tố duy nhất của $A$ và mệnh đề suy ra từ Mệnh đề 6 của No. 3. Vậy giả sử $\dim(A) > 0$ và gọi $p$ là một iđêan nguyên tố của $A$ phân biệt với $m_A$; khi đó $\dim(A_p) < \dim(A)$. Nếu $\mathrm{di}_{A_p}(A_p) = +\infty$, giả thiết quy nạp cho thấy $\mathrm{Ext}_{A_p}^j(\kappa(p), A_p) \neq 0$ với mọi số nguyên $j \geqslant \dim(A_p)$; theo Bổ đề 3 của § 1, No. 7, điều này kéo theo $\mathrm{Ext}_A^i(\kappa_A, A) \neq 0$ với mọi số nguyên $i \geqslant \dim(A_p) + \dim(A/p)$, và đặc biệt với $i \geqslant \dim(A)$ (VIII, § 1, No. 3, Mệnh đề 8, b)).

Còn lại ta phải xét trường hợp $\mathrm{di}_A(A)$ là vô hạn nhưng chiều đơn ánh của $A_p$ là hữu hạn với mọi iđêan nguyên tố $p$ của $A$ phân biệt với $m_A$. Với một iđêan như thế, trong trường hợp này, theo Mệnh đề 10, $\mathrm{di}_{A_p}(A_p) = \dim(A_p) < \dim(A)$, do đó $\mathrm{Ext}_{A_p}^i(\kappa(p), A_p) = 0$ với $i \geqslant \dim(A)$. Vì $\mathrm{di}_A(A)$ là vô hạn, Mệnh đề 6 của No. 3 khi đó cho thấy $\mathrm{Ext}_A^i(\kappa_A, A) \neq 0$ với mọi số nguyên $i \geqslant \dim(A)$.

#### Định lý 2 (Bass) {#ac-x-s3-thm-2 .statement}

Cho $A$ là một vành địa phương Noether; đặt $d = \dim(A)$. Gọi $x = (x_1, \ldots, x_d)$ là một dãy cát tuyến cực đại gồm các phần tử của $m_A$, và $x$ là iđêan mà nó sinh ra. Các điều kiện sau là tương đương:

(i) $\Lambda$ là một vành Gorenstein;
(ii) ta có $\operatorname{di}_\Lambda(A) = d$;
(iii) tồn tại một số nguyên $i > d$ sao cho $\operatorname{Ext}^i_\Lambda(\kappa_A, A) = 0$;
(iv) ta có $\operatorname{Ext}^i_\Lambda(\kappa_A, A) = 0$ với $i < d$ và không gian vectơ trên $\kappa_A$ $\operatorname{Ext}^d_\Lambda(\kappa_A, A)$ có chiều bằng 1;
(v) vành $A$ là Macaulay và không gian vectơ trên $\kappa_A$ $\operatorname{Hom}_A(\kappa_A, A/x)$ có chiều bằng 1;
(vi) dãy $x$ là $A$-chính quy và không gian vectơ trên $\kappa_A$ $\operatorname{Hom}_A(\kappa_A, A/x)$ có chiều bằng 1.

Tính tương đương của (i), (ii) và (iii) suy ra từ Bổ đề 2 và Mệnh đề 10. Nếu $\operatorname{Ext}^i_\Lambda(\kappa_A, A)$ bằng không với mọi số nguyên $i < d$, thì vành $A$ là Macaulay (§ 2, No. 3, Mệnh đề 3); nếu vành $A$ là Macaulay, thì dãy $x$ là $A$-chính quy (*loc. cit.*, Định lý 1); nếu dãy $x$ là $A$-chính quy, ta có $\operatorname{Ext}^i_\Lambda(\kappa_A, A) = 0$ với $i < d$ và các không gian vectơ trên $\kappa_A$ $\operatorname{Ext}^d_\Lambda(\kappa_A, A)$ và $\operatorname{Hom}_A(\kappa_A, A/x)$ là đẳng cấu (A, X, p. 166, Mệnh đề 9). Điều đó chứng minh tính tương đương của các điều kiện (iv), (v) và (vi).

Hãy chứng minh rằng (i) kéo theo (v): nếu $A$ là một vành Gorenstein, thì nó là một vành Macaulay (mệnh đề 10). Khi đó dãy $x$ là chính quy đối với $A$ (§ 2, No. 3, mệnh đề 4), do đó $A/x$ là một vành Gorenstein Artin (ví dụ 2), nên không gian vectơ $\operatorname{Hom}_A(\kappa_A, A/x)$ trên $\kappa_A$ có chiều bằng 1.

Sau cùng hãy chứng minh rằng (vi) kéo theo (i): dưới giả thiết (vi), vành $A/x$ là một vành Gorenstein (bổ đề 1), do đó $A$ là một vành Gorenstein (ví dụ 3).

#### Hệ quả {#ac-x-s3-n7-cor-1 .statement}

*Cho $\Lambda$ là một vành địa phương Noether có chiều d. $\Lambda$-môđun $\operatorname{Ext}^d_\Lambda(\kappa_A, A)$ khác không.*

Điều này suy ra từ định lý 2 nếu $\Lambda$ là một vành Gorenstein, và từ bổ đề 2 trong trường hợp ngược lại.

#### Mệnh đề 11 {#ac-x-s3-prop-11 .statement}

*Cho $A$ là một vành Noether. Các điều kiện sau là tương đương:*

(i) $A$ là một vành Gorenstein ;
(ii) với mọi iđêan nguyên tố $p$ của $A$, không gian vectơ $\kappa(p)$ $\operatorname{Ext}^i_{A_p}(\kappa(p), A_p)$ bằng không nếu $i \neq \operatorname{ht}(p)$ và có chiều bằng 1 nếu $i = \operatorname{ht}(p)$.
(iii) với mọi iđêan cực đại $m$ của $A$, tồn tại một số nguyên $i > \operatorname{ht}(m)$ sao cho $\operatorname{Ext}^i_{A_m}(A/m, A_m) = 0$.

(i) $\Rightarrow$ (ii) : điều này suy ra từ định lý 2 áp dụng cho vành Gorenstein địa phương $A_p$ (ví dụ 1).
(ii) $\Rightarrow$ (iii) : điều này là tầm thường.
(iii) $\Rightarrow$ (i) : dưới giả thiết (iii), $A_m$ là một vành Gorenstein với mọi iđêan cực đại $m$ của $A$ (định lý 2), và $A$ là Gorenstein.

### 8. Vành Gorenstein và Đại số Phẳng

#### Mệnh đề 12 {#ac-x-s3-prop-12 .statement}

Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether, khiến $B$ trở thành một A-môđun phẳng. Các điều kiện sau là tương đương:

(i) $B$ là một vành Gorenstein ;
(ii) $A$ và $\kappa_A \otimes_A B$ là các vành Gorenstein.

Trước hết hãy xét trường hợp các vành $A$ và $B$ là Artin. Ký hiệu $C$ là vành địa phương $\kappa_A \otimes_A B$; trường thặng dư của nó $\kappa_C$ được đồng nhất với $\kappa_B$. Vì $B$ phẳng trên $A$, $B$-môđun $\mathrm{Hom}_B(C, B)$ đẳng cấu với $\mathrm{Hom}_A(\kappa_A, A) \otimes_A B$ (I, § 2, No. 10, mệnh đề 11), do đó đẳng cấu với $\mathrm{Hom}_A(\kappa_A, A) \otimes_{\kappa_A} C$. Suy ra một dãy các đẳng cấu

$$
\mathrm{Hom}_B(\kappa_B, B) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_B(C, B)) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_A(\kappa_A, A) \otimes_{\kappa_A} C)
$$
$$
\longrightarrow \mathrm{Hom}_A(\kappa_A, A) \otimes_{\kappa_A} \mathrm{Hom}_C(\kappa_C, C) .
$$

Đặc biệt, ta có $[\mathrm{Hom}_B(\kappa_B, B) : \kappa_B] = [\mathrm{Hom}_A(\kappa_A, A) : \kappa_A] \ [\mathrm{Hom}_C(\kappa_C, C) : \kappa_C]$
và khi đó mệnh đề suy ra từ bổ đề 1 của No. 7.

Hãy chuyển sang trường hợp tổng quát. Nếu trong mệnh đề thay từ "Gorenstein" bằng từ "Macaulay", thì mệnh đề là một trường hợp riêng của Mệnh đề 10 của § 2, No. 7. Do đó ta có thể giả sử rằng các vành $A$, $B$ và $C = \kappa_A \otimes_A B$ là Macaulay. $B$-môđun $C$ là Macaulay (§ 2, No. 1, Ví dụ 4). Đặt $r = \dim(A)$, $s = \dim(C)$. Tồn tại một dãy $A$-chính quy $(x_1, \ldots, x_r)$ gồm các phần tử của $m_A$ và một dãy $(y_1, \ldots, y_s)$ gồm các phần tử của $m_B)$ là chính quy đối với $B$-môđun $C$ (§ 2, No. 3, Mệnh đề 3); gọi $x$ là iđêan của $A$ và $\mathfrak{y}$ là iđêan của $B$ tương ứng do chúng sinh ra. Dãy $(y_1, \ldots, y_s, \rho(x_1), \ldots, \rho(x_r))$ là $B$-chính quy (§ 1, No. 6, Mệnh đề 11), và $A$-môđun $B/\mathfrak{y}$ là phẳng (*loc. cit.*, Mệnh đề 10). Do đó đồng cấu từ $A/x$ vào $B/(xB + \mathfrak{y})$ suy ra từ $\rho$ khi chuyển qua các thương làm cho $B/(xB + \mathfrak{y})$ thành một $(A/x)$-môđun phẳng, và vành $\kappa_{A/x} \otimes_{A/x} B/(xB + \mathfrak{y})$ đẳng cấu với $C/\mathfrak{y}C$. Vì thế mệnh đề suy ra từ phần đầu của chứng minh, có kể đến Ví dụ 3 của No. 7.

#### Hệ quả 1 {#ac-x-s3-prop-12-cor-1 .statement}

Cho $\rho : A \to B$ là một đồng cấu của các vành Noether làm cho $B$ thành một $A$-môđun phẳng. Các điều kiện sau là tương đương:

(i) $B$ là một vành Gorenstein;
(ii) (resp. (iii)) với mọi iđêan nguyên tố (resp. iđêan cực đại) $q$ của $B$, các vành $A_{\rho^{-1}(q)}$ và $\kappa(\rho^{-1}(q)) \otimes_A B$ là Gorenstein.

Hơn nữa, nếu $B$ là một $A$-môđun phẳng trung thành, thì các điều kiện này suy ra rằng $A$ là một vành Gorenstein.

Cho $q$ là một iđêan nguyên tố của $B$; đặt $p = \rho^{-1}(q)$. Vành $B_q$, đẳng cấu với một vành phân thức của $B_p$, là phẳng trên $A_p$. Để $B_q$ là một vành Gorenstein, điều kiện cần và đủ là các vành $A_p$ và $\kappa(p) \otimes_{A_p} B_q$ cũng như vậy (Mệnh đề 12).

(i) $\Rightarrow$ (ii): cho $q$ là một iđêan nguyên tố của $B$ và $p = \rho^{-1}(q)$. Nếu $B$ là một vành Gorenstein, thì $B_q$ cũng vậy, do đó $A_p$ và $\kappa(p) \otimes_{A_p} B_q$ cũng vậy theo điều vừa nói trên. Theo nhận xét của § 2, No. 6, khi đó vành địa phương của $\kappa(p) \otimes_A B$ tại bất kỳ iđêan nguyên tố nào cũng là một vành Gorenstein, điều này kéo theo rằng $\kappa(p) \otimes_A B$ là một vành Gorenstein, do đó có (ii).

(ii) $\Rightarrow$ (iii): điều này hiển nhiên.

(iii) $\Rightarrow$ (i): với mọi iđêan cực đại $n$ của $B$, từ phần đầu của chứng minh (áp dụng với $q = n$) suy ra rằng $B_n$ là một vành Gorenstein, do đó suy ra (i).

Nếu $B$ là một A-môđun phẳng trung thành, ánh xạ $^a\rho : \mathrm{Spec}(B) \longrightarrow \mathrm{Spec}(\Lambda)$ là toàn ánh (II, § 2, No. 5, hệ quả 4 của mệnh đề 11), do đó suy ra khẳng định cuối cùng.

#### Hệ quả 2 {#ac-x-s3-prop-12-cor-2 .statement}

Cho $A$ là một vành Noether, $J$ là một iđêan của $A$, $\hat{A}$ là bổ toàn tách của $A$ đối với tôpô $J$-adic. Xét các điều kiện sau:

(i) $A$ là một vành Gorenstein;
(ii) $\hat{A}$ là một vành Gorenstein;
(iii) với mọi iđêan cực đại $m$ của $A$ chứa $J$, $A_m$ là một vành Gorenstein;
(iv) với mọi iđêan nguyên tố $p$ của $A$ sao cho $p + J \neq A$, $A_p$ và $\kappa(p) \otimes_A \hat{A}$ là các vành Gorenstein.

Các điều kiện từ (ii) đến (iv) là tương đương, và được suy ra từ (i). Khi iđêan $J$ được chứa trong căn của $A$, các điều kiện từ (i) đến (iv) là tương đương.

Hệ quả này được suy ra từ hệ quả 1 theo cùng cách như hệ quả 4 của mệnh đề 9 ở § 2, No. 7, đã được suy ra: trong chứng minh chỉ cần thay thế từ "Macaulay" bằng từ "Gorenstein".

#### Hệ quả 3 {#ac-x-s3-prop-12-cor-3 .statement}

Cho $A$ là một vành Gorenstein và $(T_i)_{i \in I}$ là một họ hữu hạn các bất định. Các vành $A[(T_i)_{i \in I}]$ và $A[[T_i]_{i \in I}]$ là các vành Gorenstein.

Với mọi trường $k$, vành $k[T]$ là Gorenstein (No. 7, ví dụ 5); hơn nữa vành $A[T]$ là Noether. Vì vậy nó là một vành Gorenstein (hệ quả 1). Từ đó, bằng quy nạp theo $\mathrm{Card}(I)$, suy ra rằng $A[(T_i)_{i \in I}]$ là một vành Gorenstein; rồi áp dụng hệ quả 2.

## BÀI TẬP {#ac-x-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).
