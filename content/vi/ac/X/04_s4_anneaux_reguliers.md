---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 4
section_title: Anneaux réguliers
lang: vi
source: ac-x-fr
pdf_pages: 0052-0060, 0161-0164
extraction: ocr
subsections:
    - "no": 1
      title: Propriétés homologiques élémentaires des anneaux locaux réguliers
      page: 0
      pdf_page: 52
    - "no": 2
      title: Caractérisation homologique des anneaux noethériens réguliers
      page: 54
      pdf_page: 53
    - "no": 3
      title: Anneaux réguliers et algèbres finies
      page: 0
      pdf_page: 56
    - "no": 4
      title: Anneaux présentables
      page: 0
      pdf_page: 57
    - "no": 5
      title: Anneaux réguliers et extensions plates
      page: 59
      pdf_page: 58
statements: 29
exercises: 13
content_sha256: fb9026317d0a478d5e7f2deb6ba63efa2cad4fc4c680cb46c95ef19859c46ef5
translated_from: content/en-mt/ac/X/04_s4_anneaux_reguliers.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 3a9b79f63014ef951b00ee573dd100216a0d16c92c7c07a16d7c538bfed42cbf
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-70d8b5b4
glossary_version: 34
glossary_terms_sha256: 3f8310d30a959da94a677492cb56971cd8961b2cd5181aa4767a014b1cad4b46
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CÁC VÀNH CHÍNH QUY

### 1. Các tính chất đồng điều sơ cấp của các vành địa phương chính quy

#### Mệnh đề 1 {#ac-x-s4-prop-1 .statement}

Cho $A$ là một vành địa phương Noether chính quy và $n$ là chiều của nó. Khi đó $\mathrm{dh}(A) = n$ và, với mọi số nguyên $i \geqslant 0$,

$$
[\mathrm{Ext}_A^i(\kappa_A, \kappa_A) : \kappa_A] = [\mathrm{Tor}_i^A(\kappa_A, \kappa_A) : \kappa_A] = \binom{n}{i}.
$$

Cho $x = (x_1, \ldots, x_n)$ là một hệ tọa độ của $A$ (VIII, § 5, No. 1, def. 1). Dãy $x$ sinh ra $m_A$ và là hoàn toàn cát tuyến đối với $A$ (*loc. cit.*, No. 2, th. 1). Phức Koszul $K_\bullet(x, A)$ là một phân giải tự do của $\kappa_A$ (A, X, p. 159, nhận xét 3), có vi phân bằng không modulo $m_A$. Do đó, với mọi số nguyên $i \geqslant 0$, ta có (§ 3, No. 3, công thức (1))

$$
[\mathrm{Ext}_A^i(\kappa_A, \kappa_A) : \kappa_A] = [\mathrm{Tor}_i^A(\kappa_A, \kappa_A) : \kappa_A] = \mathrm{rg}_A(K_i(x, A)) = \binom{n}{i}.
$$

Từ đó suy ra theo hệ quả 1 của mệnh đề 4 của No. 3, § 3 rằng $\mathrm{dh}(A) = n$.

#### Mệnh đề 2 {#ac-x-s4-prop-2 .statement}

Một vành địa phương Noether chính quy là nhân tử.

Theo mệnh đề 1, mọi môđun sinh hữu hạn trên một vành địa phương Noether chính quy đều thừa nhận một phân giải xạ ảnh có độ dài hữu hạn bởi các môđun xạ ảnh sinh hữu hạn, do đó bởi các môđun tự do (II, § 3, No. 2, hệ quả 2 của mệnh đề 5). Từ đó suy ra theo VII, § 4, No. 7, hệ quả 3 của mệnh đề 16 rằng vành như vậy là nhân tử.

#### Mệnh đề 3 {#ac-x-s4-prop-3 .statement}

Cho $A$ là một vành địa phương Noether chính quy và $M$ là một $A$-môđun sinh hữu hạn khác không. Chiều xạ ảnh của nó là hữu hạn, và ta có

$$
\mathrm{dp}_A(M) + \mathrm{prof}_A(M) = \dim(A).
$$

Thật vậy, $M$ có chiều xạ ảnh hữu hạn (mệnh đề 1), và ta có $\mathrm{prof}(A) = \dim(A)$ vì $A$ là một vành Macaulay (§ 2, No. 5, ví dụ 7). Khi đó áp dụng định lý 1 của § 3, No. 5.

#### Hệ quả 1 {#ac-x-s4-prop-3-cor-1 .statement}

Ta có $\mathrm{dp}_A(M) \geqslant \dim(A) - \dim(M)$; để đẳng thức xảy ra, điều kiện cần và đủ là $M$ là một môđun Macaulay.

#### Hệ quả 2 {#ac-x-s4-prop-3-cor-2 .statement}

Để $A$-môđun $M$ là tự do, điều kiện cần và đủ là nó là một môđun Macaulay và có chiều $\dim(A)$, hay tương đương là nó có độ sâu $\geqslant \dim(A)$.

#### Hệ quả 3 {#ac-x-s4-prop-3-cor-3 .statement}

Mọi môđun phản xạ sinh hữu hạn trên một vành địa phương Noether chính quy có chiều 2 đều tự do.

Thật vậy, một vành địa phương Noether chính quy là đóng nguyên (VIII, § 5, No. 2, hệ quả 1 của định lý 1). Hệ quả 3 do đó suy ra từ hệ quả 2 và § 1, No. 10, mệnh đề 16.

#### Hệ quả 4 {#ac-x-s4-prop-3-cor-4 .statement}

Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether. Giả sử rằng $A$ là chính quy và rằng $\rho$ biến $B$ thành một $A$-môđun sinh hữu hạn. Khi đó $dp_A(B) \geq \dim(A) - \dim(B)$. Để $B$ là một vành Macaulay, điều kiện cần và đủ là ta có $dp_A(B) = \dim(A) - \dim(B)$. Để $B$ là một vành Macaulay có chiều bằng $\dim(A)$, điều kiện cần và đủ là $A$-môđun $B$ là tự do.

Thật vậy, ta có $\dim(B) = \dim_A(B)$ (VIII, § 2, No. 3, th. 1); hơn nữa, $B$ là một vành Macaulay khi và chỉ khi nó là một $A$-môđun Macaulay (§ 2, No. 6, mệnh đề 8). Vì vậy chỉ cần áp dụng các hệ quả 1 và 2.

#### Nhận xét {#ac-x-s4-n1-rem-1 .statement}

Hệ quả 4 cho phép đặc trưng các vành địa phương Macaulay trong một số trường hợp quan trọng. Cho $A$ là một vành địa phương Noether; nó là một vành Macaulay khi và chỉ khi điều tương tự đúng với $\hat{A}$ (§ 2, No. 7, hệ quả 4 của mệnh đề 9). Từ nay giả sử vành địa phương $A$ đầy đủ, và đặt $d = \dim(A)$.

a) Giả sử rằng $A$ chứa một trường con. Khi đó nó chứa một trường con hệ số $K$ (IX, § 3, No. 3), và tồn tại một đại số chuỗi lũy thừa hình thức $E = K[[T_1, \ldots, T_n]]$ và một đồng cấu toàn ánh của các $K$-đại số $E \to A$ (*loc. cit.*); cũng tồn tại một đại số chuỗi lũy thừa hình thức $E' = K[[T_1, \ldots, T_d]]$ và một đồng cấu địa phương đơn ánh của các $K$-đại số $E' \to A$ sao cho $A$ là một đại số hữu hạn trên $E'$ (*loc. cit.*). Các tính chất sau là tương đương :

(i) $A$ là một vành Macaulay;
(ii) $dp_E(A) = n - d$;
(iii) $A$ là một $E'$-môđun tự do.

b) Giả sử trường thặng dư của $A$ có đặc số $p > 0$. Tồn tại một vành-$p$ có độ dài $+\infty$, với trường thặng dư $\kappa_A$ (IX, § 2, No. 3, mệnh đề 5). Cho $C$ là một vành như vậy; tồn tại một đại số chuỗi lũy thừa hình thức $E = C[[T_1, \ldots, T_n]]$ và một đồng cấu toàn ánh $\rho : E \to A$ (IX, § 2, No. 5, định lý 3). Các tính chất sau là tương đương:

(i) $A$ là một vành Macaulay;
(ii) $dp_E(A) = n + 1 - d$.

Hơn nữa, giả sử rằng $p1_A$ không là một ước của không trong $A$; khi đó tồn tại một đại số chuỗi lũy thừa hình thức $E' = K[[T_1, \ldots, T_{d-1}]]$ và một đồng cấu địa phương đơn ánh của các đại số $K$, $E' \to A$, sao cho $A$ là một đại số hữu hạn trên $E'$ (*loc. cit.*). Vành địa phương $E'$ là chính quy, có chiều $n + 1$ (VIII, § 5, No. 5, ví dụ 2). Các điều kiện trước đó cũng tương đương với

(iii) $A$ là một $E'$-môđun tự do.

Để có các kết quả tương tự trong trường hợp các môđun, xem § 5, No. 5.

### 2. Đặc trưng hóa đồng điều của các vành Noether chính quy

#### Định lý 1 (Serre) {#ac-x-s4-thm-1 .statement}

Một vành địa phương Noether là chính quy khi và chỉ khi chiều đồng điều của nó là hữu hạn.

Ta đã thấy rằng một vành địa phương Noether chính quy có chiều đồng điều hữu hạn (mệnh đề 1).

Ngược lại, cho $A$ là một vành địa phương Noether có chiều đồng điều hữu hạn $n$; theo § 3, No. 3, Hệ quả 2 của Mệnh đề 4 và No. 5, Định lý 1, ta có
$$
n = \mathrm{dh}(A) = \mathrm{dp}_A(\kappa_A) = \mathrm{prof}(A) .
$$
Nếu $n = 0$, $A$-môđun $\kappa_A$ là tự do, do đó $m_A = 0$ và $A$ là một trường. Giả sử $n > 0$ và lập luận bằng quy nạp theo $n$. Vì $\mathrm{prof}(A) > 0$, iđêan $m_A$ không liên kết với $A$ (§ 1, No. 1, Nhận xét 2), do đó không được chứa trong hợp của $m_A^2$ và các iđêan liên kết với $A$ (II, $§ 1$, No. 1, Mệnh đề 2). Do đó (IV, $§ 1$, No. 1, Hệ quả 2 của Mệnh đề 2), ta có thể tìm được một phần tử $x$ của $m_A - m_A^2$ sao cho phép vị tự $x_A$ là đơn ánh. Gọi $B$ là vành địa phương Noether $A/xA$ và xét dãy các $A$-môđun
$$
0 \to \kappa_A \xrightarrow{i} m_A/xm_A \xrightarrow{p} m_B \to 0
$$
trong đó ánh xạ $i$ được suy ra bằng cách chuyển qua các môđun thương từ ánh xạ $a \mapsto ax$ của $A$ vào $m_A$, và trong đó $p$ là toàn cấu chính tắc; nó là khớp. Vì lớp của $x$ trong không gian vectơ $\kappa_A$ $m_A/m_A^2$ là khác không, tồn tại một ánh xạ $A$-tuyến tính $\phi : m_A \to \kappa_A$ với $\phi(x) = 1$; bằng cách chuyển qua môđun thương, ta suy ra từ $\phi$ một phép rút của $i$, sao cho dãy khớp trước đó là tách. Điều này kéo theo các hệ thức
$$
\mathrm{dp}_B(m_B) \leq \mathrm{dp}_B(m_A/xm_A) = \mathrm{dp}_A(m_A) < +\infty
$$
(Hệ quả 2 của Mệnh đề 7 của § 3, No. 4 và $\Lambda$, X, p. 135, Hệ quả 1). Hệ quả 2 của loc. cit. áp dụng cho dãy khớp các $B$-môđun $0 \to m_B \to B \to \kappa_B \to 0$ suy ra $\mathrm{dp}_B(\kappa_B) < +\infty$. Do đó vành $B$ có chiều đồng điều hữu hạn (§ 3, No. 3, Hệ quả 2 của Mệnh đề 4), và có độ sâu $n - 1$ (§ 1, No. 4, Mệnh đề 7 và No. 3, Hệ quả của Mệnh đề 4). Theo giả thiết quy nạp, $B$ là chính quy, do đó $A$ là chính quy (VIII, $§ 5$, No. 3, Hệ quả 1 của Mệnh đề 2).

Do đó, nếu $A$ là một vành địa phương Noether, có một sự tương đương giữa ba tính chất sau:
(i) $A$ là chính quy;
(ii) $A$-môđun $\kappa_A$ có chiều xạ ảnh hữu hạn;
(iii) mọi $A$-môđun sinh hữu hạn đều có chiều xạ ảnh $< +\infty$.

#### Định nghĩa 1 {#ac-x-s4-def-1 .statement}

Người ta nói rằng một vành $A$ là chính quy nếu nó là Noether và nếu vành địa phương $A_m$ là chính quy đối với mọi iđêan cực đại $m$ của $A$.

#### Mệnh đề 4 {#ac-x-s4-prop-4 .statement}

Cho $A$ là một vành Noether. Các điều kiện sau là tương đương:
(i) $A$ là chính quy;
(ii) mọi $A$-môđun sinh hữu hạn đều có chiều xạ ảnh $< +\infty$;
(iii) với mọi iđêan cực đại $m$ của $A$, chiều xạ ảnh của $A/m$ là hữu hạn;
(iv) với mọi iđêan nguyên tố $p$ của $A$, vành địa phương $A_p$ là chính quy.

Ta hãy chứng minh rằng (i) kéo theo (ii). Cho $M$ là một $A$-môđun sinh hữu hạn. Dưới giả thiết (i), ta có $\mathrm{dp}_{A_m}(M_m) \leq \mathrm{dh}(A_m) < +\infty$ với mọi iđêan cực đại $m$ của $A$ (No. 1, mệnh đề 1); do đó $M$ có chiều xạ ảnh $< +\infty$ ($§ 3$, No. 2, hệ quả 2 của mệnh đề 3), do đó (ii).

#### Ví dụ 1 {#ac-x-s4-n2-exa-1 .statement}

Nếu vành $A$ là chính quy, vành phân thức $S^{-1}A$ là chính quy với mọi tập con nhân $S$ của $A$: điều này suy ra chẳng hạn từ đặc trưng hóa (iii) ở trên.

#### Ví dụ 2 {#ac-x-s4-n2-exa-2 .statement}

Để một vành là chính quy, điều kiện cần và đủ là nó đẳng cấu với tích của một họ hữu hạn các vành nguyên chính quy; điều này thực tế suy ra từ sự kiện rằng mọi vành chính quy đều địa phương nguyên ($§ 1$, No. 8), vì các vành địa phương chính quy là nguyên.

#### Ví dụ 3 {#ac-x-s4-n2-exa-3 .statement}

Các vành nguyên chính quy có chiều $\leq 1$ là các vành Dedekind (VIII, $§ 5$, No. 1, ví dụ 1 và VII, $§ 2$, No. 2, định lý 1).

#### Hệ quả 1 {#ac-x-s4-prop-4-cor-1 .statement}

*Cho $A$ là một vành Noether. Các điều kiện sau là tương đương*:

(i) *ta có* $\mathrm{dh}(A) < +\infty$ ;
(ii) *$A$ là chính quy và ta có* $\dim(A) < +\infty$.

*Nếu các điều kiện này được thỏa mãn, ta có* $\dim(A) = \mathrm{dh}(A)$.

Nếu vành $A$ là chính quy, ta có với mọi iđêan cực đại $m$ của $A$ đẳng thức $\dim(A_m) = \mathrm{dh}(A_m)$ (No. 1, mệnh đề 1), và do đó

$$
\mathrm{dh}(A) = \sup_m \mathrm{dh}(A_m) = \sup_m \dim(A_m) = \dim A
$$

($§ 3$, No. 2, mệnh đề 3 và VIII, $§ 1$, No. 3, mệnh đề 8). Mặt khác, nếu $\mathrm{dh}(A) < +\infty$, vành $A$ là chính quy theo mệnh đề 4. Hệ quả suy ra.

Tồn tại các vành Noether chính quy có chiều vô hạn (VIII, $§ 5$, bài tập 6).

#### Hệ quả 2 {#ac-x-s4-prop-4-cor-2 .statement}

*Một vành chính quy là chuẩn, Gorenstein và Macaulay.*

Thực vậy, một vành địa phương chính quy là đóng nguyên (VIII, $§ 5$, No. 2, hệ quả 1 của định lý 1), Gorenstein ($§ 3$, No. 9, ví dụ 4) và Macaulay ($§ 2$, No. 5, ví dụ 6).

#### Hệ quả 3 {#ac-x-s4-prop-4-cor-3 .statement}

*Cho $A$ là một vành Noether, $J$ là một iđêan của $A$ và $\hat{A}$ là hoàn thành tách được của $A$ đối với tôpô $J$-adic.*

a) *Để vành $\hat{A}$ là chính quy, điều kiện cần và đủ là, với mọi iđêan cực đại $m$ của $A$ chứa $J$, vành $A_m$ là chính quy.*

b) *Nếu vành $A$ là chính quy, vành $\hat{A}$ là chính quy. Nếu vành $\hat{A}$ là chính quy và iđêan $J$ được chứa trong căn của $A$, vành $\Lambda$ là chính quy.*

#### Hệ quả 4 {#ac-x-s4-prop-4-cor-4 .statement}

*Cho $A$ là một vành chính quy và $P$ là một A-môđun xạ ảnh sinh hữu hạn. Đại số đối xứng $S_A(P)$ là một vành chính quy.*

Cho $p$ là một iđêan nguyên tố của $S_A(P)$ và $q$ là ảnh ngược của nó trong $A$. Vành địa phương $S_A(P)_p$ là một vành phân thức của vành $S_A(P)_q$, vành này đẳng cấu với $S_{A_q}(P_q)$ (A, III, p. 72, mệnh đề 7); chỉ cần chứng minh rằng vành sau là chính quy. Điều này đưa ta về trường hợp $A$ là địa phương; nhưng khi đó $P$ là tự do kiểu hữu hạn. Theo mệnh đề 1 của No. 1 và A, X, p. 143, hệ quả 1, ta có $dh(S_A(P)) = dh(A) + rg_A(P) < +\infty$, và $S_A(P)$ là chính quy theo mệnh đề 4.

#### Hệ quả 5 {#ac-x-s4-prop-4-cor-5 .statement}

*Cho $A$ là một vành chính quy, và $(T_i)_{i \in I}$ là một họ hữu hạn các phần tử bất định. Vành đa thức $A[(T_i)_{i \in I}]$ và vành chuỗi hình thức $A[[T_i]_{i \in I}]$ là chính quy.*

Điều này suy ra từ hệ quả 4 và hệ quả 3 b).

### 3. Các vành chính quy và các đại số hữu hạn

#### Mệnh đề 5 {#ac-x-s4-prop-5 .statement}

*Cho $\rho : A \to B$ là một đồng cấu của các vành Noether và $N$ là một $B$-môđun. Giả sử rằng
a) vành $A$ là chính quy,
b) $N$ là một A-môđun sinh hữu hạn,
c) $B$-môđun $N$ là Cohen-Macaulay,
d) mọi iđêan nguyên tố cực tiểu của $\mathrm{Supp}_B(N)$ nằm trên một iđêan nguyên tố cực tiểu của $A$.
Khi đó $N$ là một A-môđun xạ ảnh (kiểu hữu hạn).*

Điểm cần chứng minh là, với mọi iđêan cực đại $m$ của $A$, $A_m$-môđun $N_m$ là tự do (II, § 5, No. 2, định lý 1). $A$-môđun $B/\mathrm{Ann}_B(N)$ là một môđun con của $A$-môđun sinh hữu hạn $\mathrm{End}_A(N)$, và do đó là sinh hữu hạn. Nếu thay $B$ bởi $B/\mathrm{Ann}_B(N)$, các giả thiết của mệnh đề vẫn được thỏa mãn ($§ 2$, No. 1, ví dụ 5); vì vậy ta có thể giả sử rằng $B$ là một A-môđun sinh hữu hạn và rằng $\mathrm{Supp}_B(N) = \mathrm{Spec}(B)$.

Cho $m$ là một iđêan cực đại của $\mathrm{Supp}_A(N)$; đặt $n = \dim(A_m)$. Theo Hệ quả 2 của Mệnh đề 3 của No. 1, chỉ cần chứng minh rằng $N_m$ là một A-môđun Macaulay $A_m$ có chiều $n$. Mọi iđêan cực đại của $B_m$ đều có dạng $nB_m$, trong đó $n$ là một iđêan nguyên tố của $B$ nằm trên $m$ (V, § 2, No. 1, Bổ đề 1 và Mệnh đề 1). Cho $p$ là một iđêan nguyên tố cực tiểu của $\mathrm{Supp}_B(N)$, được chứa trong $n$. Tập con đóng $V(pB_n)$ của $\mathrm{Supp}_{B_n}(N_n)$ khi đó có đối chiều không; vì $B_n$-môđun $N_n$ là Macaulay, Hệ quả của Mệnh đề 2, § 2, No. 2 suy ra đẳng thức $\dim_{B_n}(N_n) = \dim(B_n/pB_n)$. Nhưng $p$ nằm trên một iđêan nguyên tố cực tiểu của $A$, được chứa trong $m$, do đó

#### Hệ quả {#ac-x-s4-n3-cor-1 .statement}

Cho B là một vành nguyên Noether và cho A là một vành con chính quy của B. Giả sử rằng A-môđun B là sinh hữu hạn. Để vành B là một vành Macaulay, điều kiện cần và đủ là A-môđun B là xạ ảnh.

Nếu vành B là một vành Macaulay, A-môđun B là xạ ảnh theo Mệnh đề 5.

Ngược lại, giả sử rằng A-môđun B là xạ ảnh. A-môđun A là Macaulay (Hệ quả 2 của Mệnh đề 4); A-môđun B là một nhân tử trực tiếp của một A-môđun tự do kiểu hữu hạn, do đó là Macaulay (§ 2, No. 1, Ví dụ 2). Khi đó áp dụng Hệ quả 1 của Mệnh đề 8 của § 2, No. 6.

#### Ví dụ {#ac-x-s4-n3-exa-1 .statement}

Cho B là một đại số nguyên khác không kiểu hữu hạn trên một trường K. Theo VIII, § 2, No. 4, Hệ quả 1 của Định lý 3, tồn tại một đại số con A của B đẳng cấu với một đại số đa thức trên K và sao cho B là một A-môđun sinh hữu hạn. Các tính chất sau là tương đương:

(i) vành B là Macaulay;
(ii) A-môđun B là xạ ảnh;
*(iii) A-môđun B là tự do.*

### 4. Các vành trình bày được

Một vành A được gọi là trình bày được nếu tồn tại một vành chính quy R và một đồng cấu toàn ánh từ R lên A.

Theo định nghĩa, các vành chính quy là trình bày được.

#### Mệnh đề 6 {#ac-x-s4-prop-6 .statement}

a) Mọi vành phân thức của một vành trình bày được đều là trình bày được. Mọi đại số kiểu hữu hạn trên một vành trình bày được đều là một vành trình bày được.

b) Cho A là một vành trình bày được và J là một iđêan của A. Hoàn thành đầy đủ $\widehat{A}$ của A đối với tôpô J-adic là trình bày được.

c) Mọi vành địa phương Noether đầy đủ đều là trình bày được.

d) Cho A là một vành địa phương trình bày được. Tồn tại một vành địa phương chính quy R và một đồng cấu địa phương toàn ánh từ R lên A.

Cho A là một vành trình bày được; chọn một vành chính quy R và một đồng cấu toàn ánh $\rho : R \to A$.

a) Cho S là một tập con nhân của A; đặt T = $\rho^{-1}(S)$. Đồng cấu $T^{-1}R \to S^{-1}A$ suy ra từ $\rho$ là toàn ánh và vành $T^{-1}R$ là chính quy (No. 3, Ví dụ 1), do đó $S^{-1}A$ là trình bày được.

Cho B là một đại số trên A kiểu hữu hạn; tồn tại một tập hữu hạn I và một đồng cấu toàn ánh $A[(T_i)_{i \in I}] \to B$, do đó có một đồng cấu toàn ánh $R[(T_i)_{i \in I}] \to B$. Vì vành $R[(T_i)_{i \in I}]$ là chính quy (No. 2, Hệ quả 5 của Mệnh đề 4), vành B là trình bày được.

b) Đặt $I = \rho^{-1}(J)$ và ký hiệu $\hat{R}$ là hoàn thành đầy đủ của R đối với tôpô I-adic; với mỗi số nguyên $n \geq 0$, ánh xạ chính tắc $I^n/I^{n+1} \to J^n/J^{n+1}$ là toàn ánh. Do đó, đồng cấu $\hat{R} \to \hat{A}$ suy ra từ $\rho$ là toàn ánh (III, § 2, No. 8, Hệ quả 2 của Định lý 1); vì $\hat{R}$ là chính quy (No. 2, Hệ quả 3 của Mệnh đề 4), vành $\hat{A}$ là trình bày được.

c) Điều này suy ra từ IX, § 2, No. 5, Định lý 3 a) và IX, § 3, No. 3, Định lý 2 a).

d) Cho $m_A$ là iđêan cực đại của A; khi đó $p = \rho^{-1}(m_A)$ là một iđêan nguyên tố của R, vành địa phương $R_p$ là chính quy và đồng cấu $R_p \to A$ suy ra từ $\rho$ là địa phương và toàn ánh.

Vì các trường và các vành Dedekind là chính quy, do đó là trình bày được, Mệnh đề 6 suy ra rằng phần lớn các vành thường gặp trong hình học đại số là trình bày được.

#### Mệnh đề 7 {#ac-x-s4-prop-7 .statement}

Cho A là một vành trình bày được.

a) Vành $\Lambda$ là Noether và catenary.

b) Cho M là một A-môđun sinh hữu hạn. Ánh xạ
$$
p \mapsto \dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p)
$$
từ $\operatorname{Spec}(A)$ vào $\mathbf{Z}$ là nửa liên tục trên.

c) Cho M là một $\Lambda$-môđun sinh hữu hạn. Tập hợp các $p \in \operatorname{Spec}(A)$ sao cho A-môđun $M_p$ là Macaulay là một tập mở trù mật. Giao của nó với $\operatorname{Supp}(M)$ là trù mật trong $\operatorname{Supp}(M)$.

Chọn một vành chính quy R và một đồng cấu toàn ánh $R \to A$.

a) Vành R là một vành Macaulay (No. 2, Hệ quả 2 của Mệnh đề 4), do đó A là catenary ($§ 2$, No. 2, Mệnh đề 2 và VIII, § 1, No. 3, Nhận xét 2).

b) Môđun $R$ M là sinh hữu hạn và có chiều xạ ảnh $< +\infty$ (No. 1, Mệnh đề 1). Ta đồng nhất $\operatorname{Spec}(A)$ với một tập con đóng của $\operatorname{Spec}(R)$. Khi đó hàm $p \mapsto \dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p)$ trên $\operatorname{Spec}(A)$ là hạn chế của hàm $q \mapsto \dim_{R_q}(M_q) - \operatorname{prof}_{R_q}(M_q)$ trên $\operatorname{Spec}(R)$; do đó chỉ cần áp dụng Hệ quả 4 của Định lý 1 của § 3, No. 5.

c) Điều này được chứng minh như trong phần c) của tài liệu đã dẫn.

### 5. Các vành chính quy và các mở rộng phẳng

#### Mệnh đề 8 {#ac-x-s4-prop-8 .statement}

Cho $\rho : A \to B$ là một đồng cấu của các vành Noether sao cho B là một A-môđun phẳng trung thành.

a) Với mọi A-môđun sinh hữu hạn M, ta có $dp_A(M) = dp_B(B \otimes_A M)$.

b) Nếu vành B là chính quy, thì vành A là chính quy.

$$
0 \to N \to L \to M \to 0
$$

trong đó $A$-môđun $L$ là tự do kiểu hữu hạn. Ta có $dp_A(N) = dp_A(M) - 1$ (A, X, p. 135, Hệ quả 2 của Mệnh đề 1). Vì $B$ là phẳng trên $A$, dãy

$$
0 \to B \otimes_A N \to B \otimes_A L \to B \otimes_A M \to 0
$$

là khớp và ta có $dp_B(B \otimes_A N) = dp_B(B \otimes_A M) - 1$. Giả thiết quy nạp áp dụng cho $N$ cho phép ta kết luận. Điều này chứng minh a); mệnh đề b) suy ra từ a) và Mệnh đề 4 của No. 2.

#### Hệ quả {#ac-x-s4-n5-cor-1 .statement}

*Cho $B$ là một vành nguyên chính quy và cho $A$ là một vành con Noether của $B$ sao cho $B$ là một A-môđun sinh hữu hạn. Các điều kiện sau là tương đương:*

(i) $A$ là chính quy ;
(ii) $B$ là một A-môđun xạ ảnh ;
(iii) $B$ là một A-môđun phẳng ;
(iv) $B$ là một A-môđun phẳng trung thành.

(i) $\Rightarrow$ (ii) : điều này suy ra từ Hệ quả của Mệnh đề 5 của No. 3.
(ii) $\Rightarrow$ (iii) : điều này suy ra từ I, § 3, No. 1, Mệnh đề 1.
(iii) $\Rightarrow$ (iv) : với mọi iđêan nguyên tố $\mathfrak{p}$ của $A$, ta có $\mathfrak{p}B \neq B$ (V, § 2, No. 1, Hệ quả 1 của Định lý 1). Do đó chỉ cần áp dụng I, § 3, No. 1, Mệnh đề 1.
(iv) $\Rightarrow$ (i) : điều này suy ra từ Mệnh đề 8, b).

Với mọi vành địa phương Noether $A$, ta ký hiệu số nguyên

$$
\delta(A) = [\mathfrak{m}_A / \mathfrak{m}_A^2 : \kappa_A] - \dim(A)
$$

bởi $\delta(A)$.

Nhắc lại (VIII, § 5, No. 1) rằng $\delta(A)$ luôn dương và sự triệt tiêu của nó đặc trưng các vành địa phương chính quy.

Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether; từ $\rho$ suy ra một đồng cấu $\kappa_A$-tuyến tính $\mathfrak{m}_A / \mathfrak{m}_A^2 \to \mathfrak{m}_B / \mathfrak{m}_B^2$, do đó một đồng cấu $\kappa_B$-tuyến tính

$$
d\rho : \kappa_B \otimes_{\kappa_A} (\mathfrak{m}_A / \mathfrak{m}_A^2) \to \mathfrak{m}_B / \mathfrak{m}_B^2 .
$$

*Bổ đề 1.— Ta có*

$$
\delta(B) + [\mathrm{Ker}(d\rho) : \kappa_B] = \delta(A) + \delta(\kappa_A \otimes_A B) + (\dim(A) - \dim(B) + \dim(\kappa_A \otimes_A B)) .
$$

Gọi $C$ là vành địa phương $\kappa_A \otimes_A B$. Xét dãy khớp các B-môđun

$$
B \otimes_A \mathfrak{m}_A \to \mathfrak{m}_B \to \mathfrak{m}_C \to 0 ;
$$

bằng tích tenxơ với $\kappa_B$, ta thu được một dãy khớp các không gian vectơ $\kappa_{13}$

$$
\kappa_B \otimes_{\kappa_A} (\mathfrak{m}_A/\mathfrak{m}_A^2) \xrightarrow{d\rho} \mathfrak{m}_B/\mathfrak{m}_B^2 \longrightarrow \mathfrak{m}_C/\mathfrak{m}_C^2 \to 0,
$$

do đó suy ra đẳng thức

$$
[\mathfrak{m}_B/\mathfrak{m}_B^2 : \kappa_B] + [\mathrm{Ker}(d\rho) : \kappa_B] = [\mathfrak{m}_A/\mathfrak{m}_A^2 : \kappa_A] + [\mathfrak{m}_C/\mathfrak{m}_C^2 : \kappa_C],
$$

điều này kéo theo bổ đề.

#### Mệnh đề 9 {#ac-x-s4-prop-9 .statement}

*Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether. Các điều kiện sau là tương đương:

(i) vành $B$ là chính quy và ánh xạ $\kappa_B$-tuyến tính

$$
d\rho : \kappa_B \otimes_{\kappa_A} (\mathfrak{m}_A/\mathfrak{m}_A^2) \longrightarrow \mathfrak{m}_B/\mathfrak{m}_B^2
$$*

là đơn ánh;
(ii) các vành $B$ và $\kappa_A \otimes_A B$ là chính quy và A-môđun $B$ là phẳng;
(iii) các vành $A$ và $\kappa_A \otimes_A B$ là chính quy và A-môđun $B$ là phẳng;
(iv) các vành $A$ và $\kappa_A \otimes_A B$ là chính quy, và ta có

$$
\dim(B) = \dim(A) + \dim(\kappa_A \otimes_A B).
$$

Ta có $\dim(B) \leq \dim(A) + \dim(\kappa_A \otimes_A B)$ (VIII, § 3, No. 4, Hệ quả 1 của Mệnh đề 7); do đó sự tương đương của (i) và (iv) suy ra từ Bổ đề 1. Dưới giả thiết (ii), A-môđun $B$ là phẳng trung thành vì ta có $\mathfrak{m}_A B \subset \mathfrak{m}_B \neq B$ (I, § 3, No. 1, Mệnh đề 1), điều này suy ra (iii) theo Mệnh đề 8. Kéo theo (iii) $\Rightarrow$ (iv) suy ra từ VIII, *loc. cit*.

Bây giờ còn lại là chứng minh rằng khi các điều kiện tương đương (i) và (iv) được thỏa mãn, A-môđun $B$ là phẳng. Cho $x$ là một hệ tọa độ của $A$. Vì $d\rho$ là đơn ánh, ảnh của dãy này qua $\rho$ tạo thành một phần của một hệ tọa độ của $B$. Do đó dãy $x$ là hoàn toàn cắt đối với $A$ và đối với $B$ (VIII, § 5, No. 3, Mệnh đề 2), và sinh ra iđêan $\mathfrak{m}_A$ của $A$. Theo Nhận xét 3 của A, X, p. 159, A-môđun $\mathrm{Tor}_1^A(\kappa_A, B)$ đẳng cấu với $H_1(x, B)$, và do đó là không; suy ra $B$ là phẳng trên $A$ (III, § 5, No. 2, Định lý 1 và No. 4, Mệnh đề 2).

#### Ví dụ {#ac-x-s4-n5-exa-1 .statement}

*Cho $X$, $Y$ là hai đa tạp giải tích phức, địa phương có số chiều hữu hạn, $f$ là một cấu xạ từ $X$ vào $Y$, và $x$ là một điểm của $X$. Xét đồng cấu địa phương $\rho : \mathcal{O}_{Y, f(x)} \to \mathcal{O}_{X, x}$ liên kết với $f$. Ánh xạ $d\rho$ là chuyển vị của ánh xạ tiếp xúc $T_x(f) : T_x(X) \to T_{f(x)}(Y)$. Các điều kiện (i) đến (iv) của Mệnh đề 9 do đó tương đương trong trường hợp này với việc $f$ là một cấu xạ chìm tại $x$ (VAR, R, 5.9.1).*

#### Hệ quả {#ac-x-s4-n5-cor-2 .statement}

*Cho $\rho : \Lambda \to B$ là một đồng cấu của các vành Noether làm cho $B$ là một A-môđun phẳng. Nếu $A$ là chính quy và nếu $\kappa(\rho^{-1}(\mathfrak{n})) \otimes_{\Lambda} B$ là chính quy đối với mọi iđêan cực đại $\mathfrak{n}$ của $B$, thì vành $B$ là chính quy.

Thật vậy, đối với mọi iđêan cực đại $\mathfrak{n}$ của $B$, A-môđun $B_n$ của $A_{\rho^{-1}(\mathfrak{n})}$ là phẳng (II, § 3, No. 4, Mệnh đề 15), do đó vành $B_n$ là chính quy theo Mệnh đề 9.

#### BÀI TẬP {#ac-x-s4-exercises}

Xem [các bài tập cho § 4](exercises/s4/).
