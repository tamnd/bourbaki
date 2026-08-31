---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 5
section_title: Intersections complètes
lang: vi
source: ac-x-fr
pdf_pages: 0061-0069, 0164-0167
extraction: ocr
subsections:
    - "no": 1
      title: Idéal engendré par une suite complètement sécante
      page: 0
      pdf_page: 61
    - "no": 2
      title: Caractérisation des idéaux complètement sécants
      page: 63
      pdf_page: 62
    - "no": 3
      title: Idéaux complètement sécants et anneaux réguliers
      page: 65
      pdf_page: 64
    - "no": 4
      title: Anneaux gradués réguliers
      page: 66
      pdf_page: 65
    - "no": 5
      title: Suites régulières et extension des scalaires
      page: 0
      pdf_page: 67
    - "no": 6
      title: Idéaux complètement sécants et extension des scalaires
      page: 70
      pdf_page: 69
statements: 20
exercises: 11
content_sha256: b5e9caba93b7158f94aa59cbc1e2a5d7b10ca3e2baf4e16f3f77b192eaf16ff7
translated_from: content/en-mt/ac/X/05_s5_intersections_completes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 4fafd143f98fbe6ef018826b3c9a96a38e91001e0c825d883018688a1967178a
translation_model: gpt-5.4
translation_run: translate-vi-29c084ce
glossary_version: 34
glossary_terms_sha256: 14cec8c444c56e3f5fbb2ebb7173215c9fb5847fd43ef0f6b04faed39f599a82
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. GIAO HOÀN TOÀN

### 1. Iđêan sinh bởi một dãy hoàn toàn cát tuyến

#### Định nghĩa 1 {#ac-x-s5-def-1 .statement}

Cho $A$ là một vành, $J$ một iđêan của $A$. Ta nói rằng iđêan $J$ là hoàn toàn cát tuyến tại điểm $p$ của $V(J)$ nếu iđêan $J_p$ của $A_p$ được sinh bởi một dãy hoàn toàn cát tuyến đối với $A_p$. Ta nói rằng $J$ là hoàn toàn cát tuyến nếu nó có tính chất ấy tại mọi điểm của $V(J)$.

Nếu iđêan $J$ của $A$ là hoàn toàn cát tuyến, thì điều đó cũng đúng với iđêan $S^{-1}J$ của $S^{-1}A$ đối với mọi tập con nhân $S$ của $A$.

Mọi iđêan sinh bởi một dãy hoàn toàn cát tuyến đều là hoàn toàn cát tuyến. Chính xác hơn:

#### Mệnh đề 1 {#ac-x-s5-prop-1 .statement}

Cho $A$ là một vành, $J$ một iđêan của $A$, được sinh bởi một dãy hữu hạn $x = (x_1, \ldots, x_r)$ gồm các phần tử của $A$. Các điều kiện sau là tương đương:

(i) dãy $x$ là hoàn toàn cát tuyến đối với $A$ ;
(ii) (resp. (ii')) với mọi iđêan nguyên tố (resp. iđêan cực đại) $p \in V(J)$, ảnh của $x$ trong $A_p$ là hoàn toàn cát tuyến đối với $A_p$ ;
(iii) (resp. (iii')) với mọi iđêan nguyên tố (resp. iđêan cực đại) $p \in V(J)$, iđêan $J$ là hoàn toàn cát tuyến tại $p$ và ảnh của $x$ trong không gian vectơ $\kappa(p)$ $\kappa(p) \otimes_A J$ lập thành một cơ sở của nó.

Khi $A$ là Noether, các điều kiện ấy còn tương đương với:

(iv) với mọi số nguyên $n \geq 0$, $A/J$-môđun $J^n / J^{n+1}$ là tự do, và các ảnh của các đơn thức $x_1^{\alpha_1} \ldots x_r^{\alpha_r}$ có tổng bậc $n$ lập thành một cơ sở của nó.

Cho $p$ là một iđêan nguyên tố của $A$; ký hiệu $x_p$ là ảnh của dãy $x$ trong $A_p$. Với mọi số nguyên $i \geq 0$, $A_p$-môđun $H_i(x_p, A_p)$ đẳng cấu với $(H_i(x, A))_p$ (A, X, p. 151, 2)) ; nó bằng không nếu $p$ không chứa $J$, vì khi đó ta có $J_p = A_p$ (A, X, p. 148, cor. 2). Sự tương đương của (i), (ii) và (ii') suy ra từ điều này và từ II, § 3, No. 3, cor. 2 của th. 1. Mặt khác, sự tương đương của (ii) và (iii), và của (ii') và (iii'), suy ra từ § 1, No. 3, cor. 2 của th. 1.

Hệ quả (i) $\Rightarrow$ (iv) là một hệ quả của th. 1 của A, X, p. 160. Cuối cùng, điều kiện (iv) suy ra bằng địa phương hóa điều kiện tương tự đối với các $(A_p/J_p)$-môđun $J_p^n / J_p^{n+1}$ với mọi $p \in V(J)$, và điều kiện sau suy ra (ii) theo cor. 1 của A, X, p. 160.

#### Nhận xét 1 {#ac-x-s5-n1-rem-1 .statement}

Khi vành $A$ là Noether, có thể thay thế trong các điều kiện (ii) và (ii') "hoàn toàn cát tuyến" bằng "chính quy" (A, X, p. 160, cor. 1).

Cần lưu ý rằng điều này không còn đúng trong điều kiện (i): một dãy hoàn toàn cát tuyến đối với A không nhất thiết là chính quy đối với A (exerc. 1).

#### Nhận xét 2 {#ac-x-s5-n1-rem-2 .statement}

Cho A là một vành, J một iđêan kiểu hữu hạn của A và p một iđêan nguyên tố của A chứa J. Theo cor. 2 của th. 1 của § 1, No. 3, ta có

$$
\operatorname{prof}_{A_p}(J_p; A_p) \leq [\kappa(p) \otimes_A J : \kappa(p)]
$$

và có đẳng thức nếu và chỉ nếu J là hoàn toàn cát tuyến tại p.

Giả sử rằng J phân biệt với A và được sinh bởi một dãy hoàn toàn cát tuyến $(x_1, \ldots, x_r)$. Khi đó ta có (mệnh đề 4 của § 1, No. 3, và mệnh đề 1 ở trên)

$$
\operatorname{prof}_A(J; A) = \inf_{p \in V(J)} \operatorname{prof}_{A_p}(J_p; A_p) = r.
$$

Nếu hơn nữa A là Noether, ta có $\operatorname{codim}(V(J), \operatorname{Spec}(A)) \leq r$ (VIII, § 3, No. 3, Mệnh đề 4) và $\operatorname{prof}_A(J; A) \leq \operatorname{codim}(V(J), \operatorname{Spec}(A))$ ($§ 1$, No. 7, Mệnh đề 12), do đó cuối cùng

$$
\operatorname{prof}_A(J; A) = r = \operatorname{codim}(V(J), \operatorname{Spec}(A)) = \operatorname{ht}(J).
$$

### 2. Đặc trưng hóa các iđêan cát tuyến hoàn toàn

Cho A là một vành và J một iđêan của A. A-môđun phân bậc $\bigoplus_{n \in \mathbf{N}} J^n$ có một cấu trúc tự nhiên của đại số phân bậc trên A, suy ra từ phép nhân trong vành A; do đó ánh xạ đồng nhất của J vào $J^1$ kéo dài thành một đồng cấu toàn ánh của các đại số phân bậc trên A, gọi là chính tắc,

$$
\alpha_J : S_A(J) \longrightarrow \bigoplus_{n \in \mathbf{N}} J^n.
$$

Bằng mở rộng vô hướng lên vành $A/J$, từ $\alpha_J$ ta suy ra một đồng cấu toàn ánh của các đại số phân bậc trên $A/J$, cũng gọi là chính tắc,

$$
\beta_J : S_{A/J}(J/J^2) \longrightarrow \operatorname{gr}_J(A),
$$

với $\operatorname{gr}_J(A) = \bigoplus_{n \in \mathbf{N}} J^n / J^{n+1}$.

#### Định lý 1 {#ac-x-s5-thm-1 .statement}

Cho A là một vành Noether và J một iđêan của A. Các điều kiện sau là tương đương:

(i) iđêan J là cát tuyến hoàn toàn;
(ii) iđêan J là cát tuyến hoàn toàn tại mọi iđêan cực đại $m \in V(J)$;
(iii) $A/J$-môđun $J/J^2$ là xạ ảnh và đồng cấu chính tắc $\alpha_J : S_A(J) \longrightarrow \bigoplus_{n \in \mathbf{N}} J^n$ là song ánh;
(iv) $A/J$-môđun $J/J^2$ là xạ ảnh và đồng cấu chính tắc $\beta_J : S_{A/J}(J/J^2) \longrightarrow \operatorname{gr}_J(A)$ là song ánh.

(i) ⇒ (ii): điều này là tầm thường.

(ii) ⇒ (iii): giả sử điều kiện (ii) được thỏa mãn. Chỉ cần chứng minh rằng với mọi iđêan cực đại m của A, $A_m/J_m$-môđun $J_m/J_m^2$ là tự do và đồng cấu $\alpha_{J_m} : S_{A_m}(J_m) \longrightarrow \bigoplus_n J_m^n$ là song ánh (II, § 5, No. 2, Định lý 1 và § 3, No. 3, Định lý 1). Nhưng các mệnh đề này là tầm thường khi m không thuộc V(J), vì khi đó ta có J_m = A_m, và chúng suy ra từ A, X, p. 160, Định lý 1 và p. 161, Nhận xét, khi m thuộc V(J).

(iii) ⇒ (iv): điều này là hiển nhiên.

(iv) ⇒ (i): giả sử điều kiện (iv) được thỏa mãn; lấy p là một iđêan nguyên tố của A chứa J. Khi đó $A_p/J_p$-môđun $J_p/J_p^2$ là tự do. Lấy x = (x_1, ..., x_r) là một dãy các phần tử của J_p nâng lên một cơ sở của $J_p/J_p^2$. Dãy x sinh ra J_p (Bổ đề Nakayama), và theo phép dựng nó thỏa mãn điều kiện (iv) của Mệnh đề 1. Suy ra iđêan J_p của A_p là cát tuyến hoàn toàn, và J là cát tuyến hoàn toàn tại p.

#### Nhận xét 1 {#ac-x-s5-n2-rem-1 .statement}

Giả sử iđêan J là cát tuyến hoàn toàn; lấy (x_1, ..., x_r) là một dãy các phần tử của J sao cho với mọi iđêan cực đại m ∈ V(J), các ảnh chính tắc của các x_i trong J/mJ tạo thành một cơ sở của không gian vectơ trên A/m này. Khi đó $A/J$-môđun $J/J^2$ là tự do và các ảnh chính tắc của các x_i trong J/J^2 tạo thành một cơ sở của nó: thực vậy chỉ cần kiểm tra rằng các ảnh của các x_i tạo thành một cơ sở của $A_m/J_m$-môđun $J_m/J_m^2$ với mọi m ∈ V(J) (II, § 3, No. 3, Định lý 1), điều này suy ra từ loc. cit., No. 2, Mệnh đề 5 và Hệ quả 2, vì $A_m/J_m$-môđun $J_m/J_m^2$ là xạ ảnh (Định lý 1).

#### Hệ quả 1 {#ac-x-s5-thm-1-cor-1 .statement}

Cho $\hat{A}$ là hoàn thành tách của A đối với tôpô J-adic và $\hat{J} = J\hat{A}$ là hoàn thành tách của J. Để iđêan $\hat{J}$ của $\hat{A}$ là cát tuyến hoàn toàn thì điều kiện cần và đủ là iđêan J của A là cát tuyến hoàn toàn.

Thật vậy, ánh xạ chính tắc gr_J(A) → gr_J(\hat{A}) là một đẳng cấu của các vành phân bậc; do đó chỉ cần áp dụng tiêu chuẩn (iv).

Nói chung hơn:

#### Hệ quả 2 {#ac-x-s5-thm-1-cor-2 .statement}

Cho ρ : A → B là một đồng cấu của các vành Noether biến B thành một A-môđun phẳng, và J một iđêan của A.

a) Nếu J là cát tuyến hoàn toàn, iđêan JB của B là cát tuyến hoàn toàn.

b) Giả sử rằng iđêan JB của B là cát tuyến hoàn toàn và mọi iđêan cực đại m ∈ V(J) đều là ảnh ngược của một iđêan cực đại của B. Chẳng hạn điều này xảy ra nếu B là một A-môđun phẳng trung thành.

Trước hết nhận thấy rằng, vì A-môđun B là phẳng, $J^n \otimes_A B$ được đồng nhất với $J^nB$ và $(J^n/J^{n+1}) \otimes_{A/J} (B/JB)$ với $J^nB/J^{n+1}B$ với mọi số nguyên $n \geq 0$. Mệnh đề a) khi đó suy ra từ tiêu chuẩn (iii). Dưới các giả thiết của b), $A/J$-môđun B/JB là phẳng trung thành (I, § 2, No. 7, Hệ quả 2 của Mệnh đề 8 và § 3, No. 5, Mệnh đề 9) và J là cát tuyến hoàn toàn theo tiêu chuẩn (iv), có tính đến I, § 3, No. 1, Mệnh đề 2 và No. 6, Mệnh đề 12. Khẳng định cuối cùng suy ra từ Mệnh đề 8 của I, § 3, No. 5.

#### Hệ quả 3 {#ac-x-s5-thm-1-cor-3 .statement}

Cho $A$ là một vành Noether và $J$ một iđêan cát tuyến hoàn toàn của $A$. Nếu $A$ là một vành Macaulay (resp. một vành Gorenstein), thì $A/J$ cũng vậy.

Thật vậy lấy $m$ là một iđêan cực đại của $A$ chứa $J$. Iđêan $J_m$ của $A_m$ được sinh bởi một dãy chính quy trên $A_m$; do đó $(A/J)_m$ là một vành Macaulay (resp. một vành Gorenstein) theo Ví dụ 6 của § 2, No. 5 (resp. Ví dụ 2 của § 3, No. 9).

#### Nhận xét 2 {#ac-x-s5-n2-rem-2 .statement}

Người ta nói rằng một vành Noether $A$ là một vành giao hoàn toàn nếu, với mọi iđêan cực đại $m$ của $A$, vành địa phương đầy đủ $\widehat{A_m}$ đẳng cấu với thương của một vành địa phương chính quy Noether đầy đủ bởi một iđêan cát tuyến hoàn toàn. Từ Hệ quả 3 trên đây và từ Hệ quả 2 của Mệnh đề 12 của § 3, No. 8 suy ra rằng một vành như vậy là một vành Gorenstein.

### 3. Các iđêan cát tuyến hoàn toàn và các vành chính quy

#### Mệnh đề 2 {#ac-x-s5-prop-2 .statement}

Cho $A$ là một vành Noether. Các điều kiện sau là tương đương:

(i) $A$ là chính quy;
(ii) mọi iđêan cực đại của $A$ đều là cát tuyến hoàn toàn;
(iii) mọi iđêan $J$ của $A$ sao cho $A/J$ là chính quy đều là cát tuyến hoàn toàn.

(i) $\Rightarrow$ (iii): giả sử vành $A$ là chính quy; cho $J$ là một iđêan của $A$ sao cho $A/J$ là chính quy, và cho $p$ là một iđêan nguyên tố của $A$ chứa $J$. Khi đó các vành địa phương $A_p$ và $A_p/J_p$ là chính quy, nên $J_p$ được sinh bởi một dãy cát tuyến hoàn toàn đối với $A_p$ (VIII, § 5, No. 3, Hệ quả 2 và Mệnh đề 2), điều đó có nghĩa là $J$ là cát tuyến hoàn toàn tại $p$.

(iii) $\Rightarrow$ (ii): điều này hiển nhiên vì một trường là một vành chính quy.

(ii) $\Rightarrow$ (i): cho $m$ là một iđêan cực đại của $A$; theo giả thiết (ii), iđêan cực đại $mA_m$ của $A_m$ được sinh bởi một dãy cát tuyến hoàn toàn đối với $A_m$, nên $A_m$ là chính quy (VIII, § 5, No. 2, Định lý 1). Do đó $A$ là chính quy.

#### Mệnh đề 3 {#ac-x-s5-prop-3 .statement}

Cho $A$ là một vành Noether và $J$ một iđêan của $A$ sao cho $A/J$ là chính quy. Các điều kiện sau là tương đương:

(i) iđêan $J$ là cát tuyến hoàn toàn;
(ii) với mọi iđêan nguyên tố (ứng với iđêan cực đại) $p$ của $A$ chứa $J$, vành $A_p$ là chính quy;
(iii) hoàn thành tách biệt của $A$ đối với tôpô $J$-adic là chính quy.

Theo Định lý 1, điều kiện (i) có nghĩa là với mọi iđêan nguyên tố (ứng với iđêan cực đại) $p$ của $A$ chứa $J$, iđêan $J_p$ của vành địa phương $A_p$ được sinh bởi một dãy cát tuyến hoàn toàn đối với $A_p$. Vì $A_p/J_p$ là chính quy theo giả thiết, điều kiện sau này tương đương với tính chính quy của $A_p$ (VIII, § 5, No. 3, Mệnh đề 2 và Hệ quả 2 của nó); điều này chứng minh tính tương đương của (i) và (ii). Tính tương đương của (ii) và (iii) suy ra từ § 4, No. 2, Hệ quả 3 của Mệnh đề 4.

#### Mệnh đề 4 {#ac-x-s5-prop-4 .statement}

Cho $A$ là một vành chính quy, $J$ một iđêan của $A$, và $A_0$ một vành con của $A$ sao cho đồng cấu chính tắc $A_0 \to A/J$ là song ánh.

a) Iđêan $J$ là cát tuyến hoàn toàn, $A_0$-môđun $J/J^2$ là xạ ảnh sinh hữu hạn, và vành $A_0$ là chính quy.

b) Cho $\varphi : J/J^2 \to J$ là một tiết diện $A_0$-tuyến tính của toàn cấu chính tắc $J \to J/J^2$. Đồng cấu các $A_0$-đại số $S_{A_0}(J/J^2) \longrightarrow A$ kéo dài $\varphi$ kéo dài thành một đẳng cấu từ hoàn thành của vành phân bậc $S_{A_0}(J/J^2)$ lên hoàn thành tách của $A$ đối với tôpô $J$-adic.

a) Cho $\mathfrak{p}$ là một iđêan nguyên tố của $A$ chứa $J$. Ta có $\mathfrak{p} = (\mathfrak{p} \cap A_0) \oplus J$ và do đó $\mathfrak{p}^2 = (\mathfrak{p} \cap A_0)^2 \oplus \mathfrak{p}J$, vì thế $\mathfrak{p}^2 \cap J = \mathfrak{p}J$. Kí hiệu $i$ là đơn ánh chính tắc của $J$ vào $\mathfrak{p}$. Từ điều vừa nêu trên, ánh xạ $i \otimes 1_{A/\mathfrak{p}} : J \otimes_A A/\mathfrak{p} \longrightarrow \mathfrak{p} \otimes_A A/\mathfrak{p}$ là đơn ánh, và điều tương tự cũng đúng với $i_p \otimes 1_{\kappa(\mathfrak{p})} : J_p \otimes_{A_p} \kappa(\mathfrak{p}) \longrightarrow \mathfrak{p}A_p \otimes_{A_p} \kappa(\mathfrak{p})$. Bổ đề Nakayama suy ra rằng iđêan $J_p$ của $A_p$ được sinh bởi một tập con của một hệ tọa độ của vành địa phương chính quy $A_p$. Theo Mệnh đề 2 của VIII, § 5, No. 3, vành $A_p/J_p$ là chính quy và iđêan $J_p$ là hoàn toàn cát tuyến. Do đó $J$ là hoàn toàn cát tuyến, vành $A_0$, đẳng cấu với $A/J$, là chính quy, và $A_0$-môđun $J/J^2$ là xạ ảnh sinh hữu hạn theo Định lý 1 (No. 2).

b) Suy ra từ Định lý 1 rằng đồng cấu chính tắc $\beta_J : S_{A_0}(J/J^2) \longrightarrow \mathrm{gr}_J(A)$ là song ánh. Cho $f : S_{A_0}(J/J^2) \longrightarrow A$ là đồng cấu các $A_0$-đại số kéo dài ánh xạ $A_0$-tuyến tính $\varphi : J/J^2 \longrightarrow J$. Nếu $A$ được trang bị lọc $J$-adic và $S_{A_0}(J/J^2)$ được trang bị lọc liên kết với phân bậc của nó, thì $\beta_J$ được đồng nhất với đồng cấu suy ra từ $f$ bằng cách chuyển qua các vành phân bậc liên kết. Mệnh đề b) khi đó suy ra từ III, § 2, No. 8, Hệ quả 3 của Định lý 1.

### 4. Các vành phân bậc chính quy

Cho $A_0$ là một vành và $P$ là một $A_0$-môđun phân bậc kiểu $\mathbf{N}$ ở các bậc $> 0$. Kí hiệu $A$ là vành $S_{A_0}(P)$; trên $A$ tồn tại một phân bậc duy nhất kiểu $\mathbf{N}$ mà đối với nó $A_0$ có bậc 0 và $P$ là một $A_0$-môđun con phân bậc của $A$. Kí hiệu $A_+$ là iđêan $\bigoplus_{n>0} A_n$ của $A$. Khi đó ánh xạ chính tắc $P \longrightarrow A_+/A_+^2$ là một đẳng cấu các $A_0$-môđun phân bậc (xem A, III, p. 76, Mệnh đề 10).

Nếu $A_0$-môđun $P$ là tự do phân bậc (A, II, p. 167, Nhận xét 3) và nếu $(x_i)_{i \in I}$ là một cơ sở của $P$ gồm các phần tử thuần nhất, thì $A_0$-đại số phân bậc $S_{A_0}(P)$ đẳng cấu với đại số đa thức $A_0[(X_i)_{i \in I}]$, được trang bị phân bậc mà đối với nó mỗi $X_i$ là thuần nhất bậc $\deg(x_i)$. Mọi $A_0$-đại số phân bậc kiểu $\mathbf{N}$, đẳng cấu với một $A_0$-đại số phân bậc có dạng ở trên, được gọi là một $A_0$-đại số đa thức phân bậc.

Khi vành $A_0$ là chính quy và $A_0$-môđun $P$ là xạ ảnh sinh hữu hạn, vành $S_{A_0}(P)$ là chính quy (§ 4, No. 2, hệ quả 4 của Mệnh đề 4). Ngược lại:

#### Định lý 2 {#ac-x-s5-thm-2 .statement}

Cho $A$ là một vành chính quy, phân bậc kiểu $\mathbf{N}$. Vành $A_0$ gồm các phần tử bậc 0 trong $A$ là chính quy; tồn tại một $A_0$-môđun xạ ảnh sinh hữu hạn $P$ được phân bậc theo các bậc $> 0$ sao cho $A$ đẳng cấu, như một $A_0$-đại số phân bậc, với $S_{A_0}(P)$.

Ký hiệu $P$ là $A_0$-môđun phân bậc $A_+/A_+^2$. Theo Mệnh đề 4 của No. 3, vành $A_0$ là chính quy và $A_0$-môđun $P$ là xạ ảnh và sinh hữu hạn. Do đó các thành phần thuần nhất của $P$ là xạ ảnh, và tồn tại một tiết diện $A_0$-tuyến tính $\varphi : P \to A_+$, phân bậc bậc 0, của toàn cấu chính tắc $A_+ \to P$. Gọi $f : S_{A_0}(P) \longrightarrow \Lambda$ là đồng cấu các $A_0$-đại số phân bậc mở rộng $\varphi$. Theo Mệnh đề 4, $f$ mở rộng thành một đẳng cấu từ bổ toàn tách rời của $S_{A_0}(P)$ đối với tôpô $S_{A_0}(P)_+$-adic lên bổ toàn tách rời của $A$ đối với tôpô $A_+$-adic. Do đó, $f$ là đơn ánh và ảnh của nó trù mật trong $A$ đối với tôpô $A_+$-adic. Nhưng vì các tôpô cảm sinh trên các thành phần thuần nhất của $A$ là rời rạc và ảnh của $f$ là một môđun con phân bậc, điều này kéo theo rằng $f$ là song ánh.

#### Hệ quả 1 {#ac-x-s5-thm-2-cor-1 .statement}

*Cho B là một vành chính quy, phân bậc theo các bậc dương. Giả sử rằng mọi $B_0$-môđun xạ ảnh sinh hữu hạn đều tự do.*
a) *Vành $B_0$ là một miền nguyên và chính quy, và $B_0$-đại số $B$ là một $B_0$-đại số đa thức phân bậc sinh hữu hạn.*
b) *Cho A là một vành con phân bậc của B sao cho $A_0 = B_0$ và B là một A-môđun sinh hữu hạn. Các điều kiện sau là tương đương:
(i) A-môđun B là tự do phân bậc;
(ii) A-môđun B là phẳng;
(iii) A là một $A_0$-đại số đa thức phân bậc sinh hữu hạn.*

Theo định lý 2, vành $B_0$ là chính quy, do đó là một tích của các vành nguyên chính quy ($§ 4$, No. 2, ví dụ 2). Với mọi phần tử lũy đẳng $e$ của $B_0$, $B_0$-môđun $B_0e$ là xạ ảnh, do đó tự do, điều này kéo theo $e = 0$ hoặc $1$; vì thế $B_0$ là nguyên. Khi đó mệnh đề a) suy ra từ định lý 2 và từ sự kiện rằng một $B_0$-môđun xạ ảnh sinh hữu hạn phân bậc là tự do phân bậc.

Ta chứng minh b).

(i) $\Leftrightarrow$ (ii): các $A_0$-môđun phân bậc sinh hữu hạn phẳng đều là tự do phân bậc (II, $§ 5$, No. 2, hệ quả 2 của định lý 1). Do đó tính tương đương của (i) và (ii) suy ra từ A, X, p. 144, mệnh đề 8.

(ii) $\Leftrightarrow$ (iii): vì $B$ là nguyên trên $A$ và là một đại số trên $A_0$ sinh hữu hạn, nên $A$ là một đại số trên $A_0$ sinh hữu hạn (V, $§ 1$, No. 9, bổ đề 5), do đó là một vành Noether. Khi đó tính tương đương của (ii) và (iii) suy ra từ hệ quả của mệnh đề 8 của $§ 4$, No. 5 và từ a) áp dụng cho $A$.

#### Hệ quả 2 {#ac-x-s5-thm-2-cor-2 .statement}

*Cho k là một trường, B là một đại số đa thức phân bậc trên k sinh hữu hạn, và A là một đại số con phân bậc của B. Các điều kiện sau là tương đương:
(i) B là một $\Lambda$-môđun phân bậc tự do;
(ii) B là một A-môđun phẳng;
(iii) có $\operatorname{Tor}_1^\Lambda(k, B) = 0$;
(iv) đại số A là một đại số đa thức phân bậc trên k sinh hữu hạn, và mọi dãy sinh tự do đại số của A gồm các phần tử thuần nhất đều là B-chính quy.*

Các hệ quả (i) $\Rightarrow$ (ii) và (ii) $\Rightarrow$ (iii) là hiển nhiên, và hệ quả (iii) $\Rightarrow$ (i) suy ra từ A, X, p. 144, mệnh đề 8, a).

(iv) ⇒ (iii): giả sử điều kiện (iv) được thỏa mãn, và gọi x là một dãy sinh tự do đại số của A gồm các phần tử thuần nhất. Dãy x, vì là A-chính quy, nên hoàn toàn cát tuyến đối với A (A, X, p. 157, mệnh đề 5), do đó A-môđun Tor_1^A(k, B) đẳng cấu với H_1(x, B) (A, X, p. 159, nhận xét 3); nhưng môđun sau bằng không, vì dãy x là B-chính quy.

Các hệ quả 1 và 2 kéo theo bổ đề 5 của LIE, V, § 5, No. 5.

### 5. Dãy chính quy và mở rộng vô hướng

#### Mệnh đề 5 {#ac-x-s5-prop-5 .statement}

Cho ρ : A → B là một đồng cấu địa phương của các vành địa phương Noether, N là một B-môđun sinh hữu hạn, x = (x_1, ..., x_r) là một dãy phần tử của m_B, và u : A[T_1, ..., T_r] → B là đồng cấu duy nhất của các đại số trên A sao cho u(T_i) = x_i với i = 1, ..., r. Các điều kiện sau là tương đương:

(i) đồng cấu u làm cho N thành một A[T_1, ..., T_r]-môđun phẳng;
(ii) A-môđun N là phẳng và, với mọi A-môđun M, dãy x là M ⊗_A N-chính quy;
(iii) A-môđun N là phẳng và dãy x là κ_A ⊗_A N-chính quy;
(iv) A-môđun N/(x_1N + ... + x_rN) là phẳng và dãy x là N-chính quy.

(i) ⇒ (ii): đặt T = (T_1, ..., T_r). Giả sử rằng A[T]-môđun N là phẳng. Vì A[T] phẳng trên A, A-môđun N là phẳng (I, § 2, No. 7, hệ quả 3 của mệnh đề 8). Gọi M là một A-môđun. Dãy T hiển nhiên là M[T]-chính quy, do đó là M[T] ⊗_{A[T]} N-chính quy, vì N phẳng trên A[T]. Bây giờ A[T]-môđun M[T] ⊗_{A[T]} N được đồng nhất với M ⊗_A N, phép vị tự với tỉ số T_i tương ứng với tự đồng cấu 1_M ⊗ (x_i)_N. Do đó điều kiện (ii) được thỏa mãn.

(ii) ⇒ (iii): điều này là tầm thường.

(iii) ⇒ (iv): điều này suy ra từ mệnh đề 10 của § 1, No. 6.

(iv) ⇒ (i): gọi t là iđêan của A[T] sinh bởi T. (A[T]/t)-môđun N/tN là phẳng theo giả thiết và N là phân ly theo iđêan đối với t (III, § 5, No. 4, mệnh đề 2). Để chứng minh rằng N phẳng trên A[T], chỉ cần chứng minh, theo định lý 1 của loc. cit., No. 2, rằng A-môđun Tor_1^{A[T]}(A[T]/t, N) bằng không. Nhưng vì dãy T là A[T]-chính quy, môđun này đẳng cấu với H_1(T, N) (A, X, p. 159, nhận xét 3), và môđun này bằng không vì dãy T là N-chính quy (loc. cit., p. 157, mệnh đề 5).

#### Hệ quả {#ac-x-s5-n5-cor-1 .statement}

Cho k là một trường, Λ là một đại số địa phương Noether trên k, x = (x_1, ..., x_r) là một dãy phần tử của m_A, và M là một Λ-môđun sinh hữu hạn. Gọi Ā và Ĝ là các đầy đủ hóa của A và M đối với tôpô $(x_1Ā + ... + x_rĀ)$-adic của chúng; gọi u : k[T_1, ..., T_r] → Ā là đồng cấu duy nhất của các đại số trên k sao cho u(T_i) = x_i với i = 1, ..., r, và gọi ū : k[[T_1, ..., T_r]] → Ā là đồng cấu liên tục duy nhất mở rộng nó. Các điều kiện sau là tương đương:

(i) dãy $x$ là $M$-chính quy;
(ii) đồng cấu $u$ làm cho $M$ thành một $k[T_1, \ldots, T_r]$-môđun phẳng;
(iii) đồng cấu $\hat{u}$ làm cho $\hat{M}$ thành một $k[[T_1, \ldots, T_r]]$-môđun phẳng.
Tính tương đương của (i) và (ii) suy ra từ tính tương đương của các điều kiện (i) và (iv) của mệnh đề 5; tính tương đương của (ii) và (iii) suy ra từ III, § 5, No. 4, mệnh đề 4.

Các kết quả này cho phép mô tả các môđun macaulay trong hai trường hợp quan trọng. Gọi $\Lambda$ là một vành địa phương Noether, $M$ là một $\Lambda$-môđun sinh hữu hạn. Việc nói rằng $\Lambda$-môđun $M$ là macaulay tương đương với việc nói rằng $\widehat{\Lambda}$-môđun $\hat{M}$ là macaulay (§ 2, No. 7, hệ quả 4 của mệnh đề 8). Từ đây về sau ta sẽ giả sử rằng vành địa phương Noether $\Lambda$ là đầy đủ.

1) Trước hết giả sử rằng $\Lambda$ chứa một trường con; khi đó nó thừa nhận một trường đại diện $k$ (IX, § 3, No. 3, Định lý 1). Gọi $(x_1, \ldots, x_r)$ là một dãy cát tuyến cực đại của $M$; gọi $u : k[[T_1, \ldots, T_r]] \longrightarrow \Lambda$ là đồng cấu liên tục duy nhất sao cho $u(T_i) = x_i$ với $i = 1, \ldots, r$. Theo Bổ đề 4 b) của IX, § 2, No. 5 và Nhận xét 1 của VIII, § 3, No. 2, $A/\mathrm{Ann}(M)$ là một $k[[T_1, \ldots, T_r]]$-môđun sinh hữu hạn và do đó $M$ là một $k[[T_1, \ldots, T_r]]$-môđun sinh hữu hạn. Khi đó, các điều kiện sau là tương đương:
(i) $k[[T_1, \ldots, T_r]]$-môđun $M$ là tự do;
(ii) $\Lambda$-môđun $M$ là Macaulay.

Thực vậy, nói rằng $M$ là một $\Lambda$-môđun Macaulay tương đương với nói rằng dãy $(x_1, \ldots, x_r)$ là $M$-chính quy (§ 2, No. 3, Định lý 1). Theo Hệ quả trên, điều kiện sau có nghĩa là $M$ là một $k[[T_1, \ldots, T_r]]$-môđun phẳng, hay cũng vậy, là tự do vì nó sinh hữu hạn.

2) Giả sử trường thặng dư $\kappa_\Lambda$ của $\Lambda$ có đặc số $p > 0$ và rằng ta có $\dim(M/pM) < \dim(M)$. Cho $(x_1, \ldots, x_r)$ là một dãy cát tuyến cực đại của $M/pM$, sao cho $(p1_\Lambda, x_1, \ldots, x_r)$ là một dãy cát tuyến cực đại của $M$. Cho $C$ là một $p$-vành có độ dài $+\infty$, với trường thặng dư $\kappa_\Lambda$ (IX, § 2, No. 3, Mệnh đề 5). Tồn tại một đồng cấu $u_0$ từ $C$ vào $\Lambda$ cảm sinh đồng nhất trên các trường thặng dư; cho $u : C[[T_1, \ldots, T_r]] \longrightarrow \Lambda$ là đồng cấu duy nhất mở rộng $u_0$ và gửi $T_i$ tới $x_i$ với mọi $i$. Suy ra như trên từ loc. cit., No. 5, Bổ đề 4 rằng $u$ làm cho $M$ thành một $C[[T_1, \ldots, T_r]]$-môđun sinh hữu hạn. Các điều kiện sau là tương đương:
(i) $M$ là một $C[[T_1, \ldots, T_r]]$-môđun tự do;
(ii) $M$ là một $\Lambda$-môđun Macaulay.

Thực vậy điều kiện (ii) tương đương với nói rằng dãy $(x_1, \ldots, x_r)$ là $M$-chính quy và rằng phép vị tự tỉ số $p$ trong $M/(x_1M + \ldots + x_rM)$ là đơn ánh (§ 2, No. 3, Định lý 1). Bây giờ điều kiện sau có nghĩa là $M/(x_1M + \ldots + x_rM)$ là một $C$-môđun không xoắn, do đó phẳng ($\Lambda$, X, p. 9, Ví dụ 7). Vậy, xét đến Mệnh đề 5, $(iv) $\Leftrightarrow$ (i)$, điều kiện (ii) tương đương với việc $M$ là một $C[T_1, \ldots, T_r]$-môđun phẳng, hay cũng vậy (III, § 5, No. 4, Mệnh đề 4), $M$ là một $C[[T_1, \ldots, T_r]]$-môđun phẳng, tức là tự do vì nó sinh hữu hạn.

### 6. Iđêan hoàn toàn cát tuyến và mở rộng các vô hướng

#### Mệnh đề 6 {#ac-x-s5-prop-6 .statement}

Cho $\rho : A \to B$ là một đồng cấu các vành Noether, và $J$ là một iđêan của $B$. Các điều kiện sau là tương đương:

(i) $B/J$ là một $A$-môđun phẳng và iđêan $J$ là hoàn toàn cát tuyến;

(ii) với mọi $q \in V(J)$, $B_q$ là một $A$-môđun phẳng và, với mọi $A$-đại số $A'$ sao cho vành $\Lambda' \otimes_A B$ là Noether, iđêan $J(A' \otimes_A B)$ của $A' \otimes_A B$ là hoàn toàn cát tuyến;

(iii) với mọi iđêan cực đại $n$ của $B$ chứa $J$, A-môđun $B_n$ là phẳng và iđêan $J(\kappa(\rho^{-1}(n)) \otimes_A B_n)$ của $\kappa(\rho^{-1}(n)) \otimes_A B_n$ là hoàn toàn cát tuyến.

Theo Định lý 1 của No. 2, điều kiện (i) tương đương với điều kiện sau đây (i') (tương ứng là (i'')):

(i') (tương ứng là (i'')) với mọi iđêan nguyên tố (tương ứng là iđêan cực đại) $q$ của $B$ chứa $J$, $A_{\rho^{-1}(q)}$-môđun $B_q/J_q$ là phẳng và iđêan $J_q$ của $B_q$ được sinh bởi một dãy $B_q$-chính quy.

(i') $\Rightarrow$ (ii): giả sử rằng (i') được thỏa mãn. Cho $A'$ là một $A$-đại số sao cho vành $B' = A' \otimes_A B$ là Noether. Cho $q$ là một iđêan nguyên tố của $B$ chứa $J$; đặt $p = \rho^{-1}(q)$. Vì $B'_q$ được đồng nhất với $A'_p \otimes_{A_p} B_q$, suy ra từ kéo theo (iv) $\Rightarrow$ (ii) của Mệnh đề 5 (No. 5) rằng iđêan $JB'_q$ của $B'_q$ được sinh bởi một dãy $B'_q$-chính quy và rằng $B_q$ là phẳng trên $A_p$, do đó trên $A$. Hơn nữa, với mọi iđêan nguyên tố $r$ của $B'$ chứa $JB'$, ảnh ngược $q$ của $r$ trong $B$ chứa $J$, và $B'_r$ được đồng nhất với một vành phân thức của $B'_q$. Do đó $JB'_r$ là một iđêan hoàn toàn cát tuyến của $B'_r$, và $JB'$ là một iđêan hoàn toàn cát tuyến của $B'$.

(ii) $\Rightarrow$ (iii): điều này là tầm thường.

(iii) $\Rightarrow$ (i''): giả sử rằng (iii) được thỏa mãn. Cho $n$ là một iđêan cực đại của $B$ chứa $J$; đặt $m = \rho^{-1}(n)$. Cho $x$ là một dãy các phần tử của $J_n$ mà các ảnh của chúng trong $J_n/nJ_n$ tạo thành một cơ sở của không gian vectơ $\kappa(n)$ này. Dãy $x$ sinh ra $J_n$; theo Mệnh đề 1 của No. 1, nó là $(\kappa(m) \otimes_A B_n)$-chính quy. Vì A-môđun $B_n$ là phẳng theo giả thiết, suy ra từ phép kéo theo (iii) $\Rightarrow$ (iv) của Mệnh đề 5 rằng điều kiện (i'') được thỏa mãn.

#### Nhận xét 1 {#ac-x-s5-n6-rem-1 .statement}

Giả sử rằng các điều kiện tương đương của Mệnh đề 6 được thỏa mãn. Vì $B/J$ là phẳng trên $A$, với mọi $A$-đại số $A'$, dãy chính tắc các $A'$-môđun
$$
0 \to A' \otimes_A J \to A' \otimes_A B \to A' \otimes_A (B/J) \to 0
$$
do đó là khớp, và đồng cấu chính tắc $A' \otimes_A J \to J(A' \otimes_A B)$ là song ánh.

## BÀI TẬP {#ac-x-s5-exercises}

Xem [các bài tập cho § 5](exercises/s5/).
