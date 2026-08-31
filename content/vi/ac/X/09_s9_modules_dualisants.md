---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 9
section_title: Modules dualisants
lang: vi
source: ac-x-fr
pdf_pages: 0124-0140, 0174-0177
extraction: ocr
subsections:
    - "no": 1
      title: Modules dualisants
      page: 0
      pdf_page: 124
    - "no": 2
      title: Quotient par une suite régulière
      page: 128
      pdf_page: 127
    - "no": 3
      title: Changement d’anneaux
      page: 130
      pdf_page: 129
    - "no": 4
      title: Structure des modules dualisants
      page: 133
      pdf_page: 132
    - "no": 5
      title: Dualité des modules de type fini
      page: 134
      pdf_page: 133
    - "no": 6
      title: 'Exemple : le cas de la dimension 1'
      page: 0
      pdf_page: 136
statements: 31
exercises: 12
content_sha256: 8786def8238fb97fd190d72875a6cef631cedc683af9f11a06583f18402663f9
translated_from: content/en-mt/ac/X/09_s9_modules_dualisants.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 70b41f4e0959618816afc0363d5324215a447233f0a954a4c83161f076065312
translation_model: gpt-5.4
translation_run: translate-vi-56f32bd5
glossary_version: 34
glossary_terms_sha256: 2df5a09c648f3bdc9a3c61b13d5a2a35939e6abed501faa421987c778557e18c
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 9. MÔĐUN ĐỐI NGẪU HÓA

### 1. Môđun đối ngẫu hóa

#### Định nghĩa 1 {#ac-x-s9-def-1 .statement}

Cho $A$ là một vành Noether. Ta nói rằng một $\Lambda$-môđun $\Omega$ là đối ngẫu hóa nếu nó sinh hữu hạn và nếu, với mọi iđêan cực đại $m$ của $\Lambda$, không gian vectơ $A/m$ $\mathrm{Ext}_A^i(A/m, \Omega)$ bằng không với $i \neq \mathrm{ht}(m)$ và có chiều 1 với $i = \mathrm{ht}(m)$.

Với mọi iđêan cực đại $m$ của $A$ và mọi số nguyên $i$, không gian vectơ $A/m$ $\mathrm{Ext}_A^i(A/m, \Omega)$ đẳng cấu chính tắc với $\mathrm{Ext}_{A_m}^i(A/m, \Omega_m)$ ($\S$ 3, No. 2, mệnh đề 2). Do đó, để một $A$-môđun sinh hữu hạn $\Omega$ là đối ngẫu hóa, điều kiện cần và đủ là $A_m$-môđun $\Omega_m$ là đối ngẫu hóa với mọi iđêan cực đại $m$ của $A$.

#### Ví dụ 1 {#ac-x-s9-n1-exa-1 .statement}

Nếu vành $A$ là địa phương và Artin, thì các $A$-môđun đối ngẫu hóa là các $A$-môđun đơn ánh sinh hữu hạn $\Omega$ sao cho $\mathrm{Hom}_A(\kappa_A, \Omega)$ có chiều 1 ($\S$ 3, No. 3, mệnh đề 6), tức là các $A$-môđun Matlis ($\S$ 8, No. 3).

#### Ví dụ 2 {#ac-x-s9-n1-exa-2 .statement}

Để một vành Noether $A$ là Gorenstein, điều kiện cần và đủ là $A$-môđun $A$ là đối ngẫu hóa ($\S$ 3, No. 7, mệnh đề 11). Đặc biệt, $A$-môđun $A$ là đối ngẫu hóa khi $A$ là chính quy.

#### Nhận xét 1 {#ac-x-s9-n1-rem-1 .statement}

Cho $A$ là một vành địa phương Noether và $\Omega$ một $A$-môđun sinh hữu hạn. Trường thặng dư $\kappa_{\widehat{A}}$ được đồng nhất với $\kappa_A$, và $\widehat{A}$-môđun $\widehat{\Omega}$ với $\widehat{A} \otimes_A \Omega$ (III, $\S$ 3, No. 4, định lý 3). Khi đó suy ra từ A, X, p. 111, mệnh đề 10 rằng không gian vectơ $\kappa_A$ $\mathrm{Ext}_A^i(\kappa_A, \Omega)$ đẳng cấu chính tắc với $\mathrm{Ext}_{\widehat{A}}^i(\kappa_{\widehat{A}}, \widehat{\Omega})$. Do đó, để $A$-môđun $\Omega$ là đối ngẫu hóa, điều kiện cần và đủ là $\widehat{A}$-môđun $\widehat{\Omega}$ là đối ngẫu hóa.

#### Nhận xét 2 {#ac-x-s9-n1-rem-2 .statement}

Cho $\Omega$ là một $A$-môđun đối ngẫu hóa; với mọi $A$-môđun xạ ảnh $L$ hạng 1, $A$-môđun $\Omega \otimes_A L$ là đối ngẫu hóa (A, X, p. 108, mệnh đề 7, b)). Ta sẽ thấy dưới đây (No. 4, mệnh đề 6) rằng mọi $A$-môđun đối ngẫu hóa đều đẳng cấu với một môđun có dạng này.

#### Mệnh đề 1 {#ac-x-s9-prop-1 .statement}

Cho $A$ là một vành Noether và $\Omega$ là một A-môđun đối ngẫu hóa.

a) $A$ là một vành Macaulay, và A-môđun $\Omega$ là Macaulay.

b) Ta có $\mathrm{di}_A(\Omega) = \dim(\Omega) = \dim(A)$.

Trước hết giả sử rằng vành $A$ là địa phương, và ký hiệu $d$ là chiều của nó. Mệnh đề 6 của § 3, No. 3 kéo theo $\mathrm{di}_A(\Omega) = d$, do đó $\mathrm{prof}(A) = d$ theo mệnh đề 9 của § 3, No. 6, nên $A$ là một vành Macaulay. Hơn nữa, ta có $\mathrm{prof}(\Omega) = d$ theo định nghĩa của chiều sâu; vì ta có $\mathrm{prof}(\Omega) \leq \dim(\Omega) \leq d$, nên suy ra mệnh đề trong trường hợp này.

Trong trường hợp tổng quát, A$_m$-môđun $\Omega_m$ là đối ngẫu hóa với mọi iđêan cực đại $m$ của $A$, do đó $A_m$ là một vành Macaulay và $\Omega_m$ là một A$_m$-môđun Macaulay theo điều vừa đi trước, điều này kéo theo a). Hơn nữa ta có $\mathrm{di}_{A_m}(\Omega_m) = \dim(\Omega_m) = \dim(A_m)$ với mọi iđêan cực đại $m$, do đó có b) bằng cách chuyển qua cận trên bé nhất (§ 3, No. 2, mệnh đề 3).

#### Mệnh đề 2 {#ac-x-s9-prop-2 .statement}

*Cho A là một vành Noether, $\Omega$ là một A-môđun đối ngẫu hóa. Với mọi iđêan nguyên tố $p$ của A, A$_p$-môđun $\Omega_p$ là đối ngẫu hóa.*

Xét một dãy bão hòa $p \subset p_1 \subset \ldots \subset p_r$ các iđêan nguyên tố của A sao cho iđêan $p_r$ là cực đại. Lập luận quy nạp theo $r$, ta có thể giả sử rằng A$_{p_1}$-môđun $\Omega_{p_1}$ là đối ngẫu hóa. Thay thế A bởi $A_{p_1}$ và $p$ bởi $pA_{p_1}$, ta được đưa về trường hợp trong đó vành A là địa phương và dãy $p \subset m_A$ là bão hòa.

Khi đó đặt $d = \dim(A) = \mathrm{ht}(m_A)$. Ta có $\dim(A_p) = \mathrm{ht}(p) = d - 1$ vì A là một vành Macaulay (§ 2, No. 2, hệ quả của mệnh đề 2). Với mọi số nguyên $i$, A$_p$-môđun $\mathrm{Ext}^i_{A_p}(\kappa(p), \Omega_p)$ đẳng cấu với $\mathrm{Ext}^i_A(A/p, \Omega)_p$ (§ 3, No. 2, mệnh đề 2); do đó chỉ cần chứng minh rằng A/p-môđun $\mathrm{Ext}^i_A(A/p, \Omega)$ triệt tiêu với $i \neq d - 1$ và có hạng một với $i = d - 1$.

Cho $x$ là một phần tử của $m_A - p$, và $\overline{x}$ là lớp của nó trong $A/p$. Xét dãy khớp các A-môđun

$$
0 \to A/p \xrightarrow{\overline{x}} A/p \longrightarrow A/(p + xA) \to 0 .
$$

A-môđun $A/(p + xA)$ có độ dài hữu hạn vì giá của nó thu về $m_A$; vì A-môđun $\Omega$ là đối ngẫu hóa, ta có $\mathrm{Ext}^i_A(A/(p + xA), \Omega) = 0$ với $i \neq d$ ($§ 8$, No. 5, ví dụ 3). Khi đó từ dãy khớp các môđun mở rộng liên kết với dãy trên và với $\Omega$ suy ra rằng phép vị tự tỉ số $x$ trong A-môđun $\mathrm{Ext}^i_A(A/p, \Omega)$ là toàn ánh với $i \neq d - 1$, điều này kéo theo môđun này bằng không (bổ đề Nakayama). Đặc biệt $\mathrm{Ext}^d_A(A/p, \Omega)$ bằng không, và thu được một dãy khớp

$$
0 \to \mathrm{Ext}^{d-1}_A(A/p, \Omega) \xrightarrow{x} \mathrm{Ext}^{d-1}_A(A/p, \Omega) \longrightarrow \mathrm{Ext}^d_A(A/(p + xA), \Omega) \to 0 .
$$

Ta có $\mathrm{long}_A(\mathrm{Ext}^i_A(A/(p + xA), \Omega)) = \mathrm{long}_A(A/(p + xA))$ (*loc. cit.*); khi đó mệnh đề suy ra từ bổ đề sau đây, áp dụng cho vành $B = A/p$ và B-môđun $M = \mathrm{Ext}^{d-1}_A(A/p, \Omega)$:

#### Bổ đề 1 {#ac-x-s9-lem-1 .statement}

*Cho B là một vành nguyên địa phương Noether chiều 1, và M là một B-môđun xoắn-không sinh hữu hạn. Giả sử rằng ta có $\mathrm{long}_B(M/xM) = \mathrm{long}_B(B/xB)$ với mọi phần tử khác không x của B. Khi đó B-môđun M có hạng 1.*

Thật vậy, gọi $r$ là hạng của M; tồn tại một môđun con tự do L của M có hạng $r$ sao cho $M/L$ là một môđun xoắn (VII, § 4, No. 1, hệ quả của mệnh đề 1), do đó có độ dài hữu hạn (VII, § 2, No. 5, bổ đề 1). Linh hóa tử của $M/L$ không thu về 0, và vì vậy chứa một phần tử khác không $x$ của $m_B$. Xét biểu đồ giao hoán

$$
\begin{array}{cccccccc}
0 & \to & L & \longrightarrow & M & \longrightarrow & M/L & \to 0 \\
& & \downarrow_{x_L} & & \downarrow_{x_M} & & \downarrow_0 & \\
0 & \to & L & \longrightarrow & M & \longrightarrow & M/L & \to 0 .
\end{array}
$$

Theo bổ đề con rắn (A, X, p. 4, mệnh đề 2), từ đó suy ra một dãy khớp

$$
0 \to M/L \longrightarrow L/xL \longrightarrow M/xM \longrightarrow M/L \to 0 ,
$$

do đó $\operatorname{long}(M/xM) = \operatorname{long}(L/xL)$. Vì $\operatorname{long}(M/xM) = \operatorname{long}(B/xB)$ theo giả thiết và $\operatorname{long}(L/xL) = r \operatorname{long}(B/xB)$, suy ra $r = 1$.

#### Hệ quả 1 {#ac-x-s9-lem-1-cor-1 .statement}

*Với mọi tập con nhân tính S của A, S$^{-1}$A-môđun S$^{-1}\Omega$ là đối ngẫu hóa.*

#### Hệ quả 2 {#ac-x-s9-lem-1-cor-2 .statement}

*Giá của $\Omega$ bằng Spec(A).*

Thật vậy một môđun đối ngẫu hóa trên một vành địa phương theo định nghĩa là khác không.

#### Hệ quả 3 {#ac-x-s9-lem-1-cor-3 .statement}

*Cho M là một A-môđun sinh hữu hạn, và i là một số nguyên. A-môđun $\operatorname{Ext}_A^i(M, \Omega)$ là sinh hữu hạn, và giá của nó có đối chiều $\geqslant i$ trong Spec(A).*

Mệnh đề thứ nhất suy ra từ A, X, p. 108, hệ quả. Cho $\mathfrak{p}$ là một iđêan nguyên tố của giá của $\operatorname{Ext}_A^i(M, \Omega)$. Ta có $\operatorname{Ext}_A^i(M, \Omega)_\mathfrak{p} \neq 0$, do đó $\operatorname{Ext}_{A_\mathfrak{p}}^i(M_\mathfrak{p}, \Omega_\mathfrak{p}) \neq 0$ (§ 3, No. 2, mệnh đề 2), điều này kéo theo $\operatorname{di}_{A_\mathfrak{p}}(\Omega_\mathfrak{p}) \geqslant i$. Vì $\Omega_\mathfrak{p}$ là một $A_\mathfrak{p}$-môđun đối ngẫu hóa (mệnh đề 2), ta có $\operatorname{di}_{A_\mathfrak{p}}(\Omega_\mathfrak{p}) = \dim(A_\mathfrak{p})$ (mệnh đề 1), do đó có hệ quả.

#### Mệnh đề 3 {#ac-x-s9-prop-3 .statement}

*Cho A là một vành địa phương Noether, $\Omega$ là một A-môđun đối ngẫu hóa và M là một A-môđun sinh hữu hạn.

a) *Ta có $\operatorname{Ext}_A^i(M, \Omega) = 0$ với $i < \dim(A) - \dim_A(M)$.*

b) *Đặt $c = \dim(A) - \dim_A(M)$. Nếu M khác không, A-môđun $\operatorname{Ext}_A^c(M, \Omega)$ là khác không.*

c) *Ta có $\operatorname{Ext}_A^i(M, \Omega) = 0$ với $i > \dim(A) - \operatorname{prof}_A(M)$.*

Giả sử M khác không và ký hiệu F là giá của nó. Theo mệnh đề 9 của § 1, No. 5, phép hội của các mệnh đề a) và b) là tương đương với $\operatorname{prof}_F(\Omega) = c$. Nhưng vì $\Omega$ là Cohen-Macaulay và giá của nó bằng Spec(A) (mệnh đề 1 và hệ quả 2 của mệnh đề 2), ta có

$$
\operatorname{prof}_F(\Omega) = \operatorname{codim}(F, \operatorname{Spec}(A)) = c
$$

(§ 2, No. 1, hệ quả của mệnh đề 1 và No. 2, hệ quả của mệnh đề 2).

Ta sẽ chứng minh c) bằng quy nạp theo độ sâu của M. Nếu $\operatorname{prof}_A(M) = 0$, quả thật ta có $\operatorname{Ext}_A^i(M, \Omega) = 0$ với $i > \dim(A)$, vì $\operatorname{di}_A(\Omega) = \dim(A)$ (mệnh đề 1). Giả sử $\operatorname{prof}_A(M) > 0$; khi đó tồn tại một phần tử $x$ của $\mathfrak{m}_A$ sao cho phép vị tự tỉ số $x$ là đơn ánh trong M. Ta có $\operatorname{prof}_A(M/xM) = \operatorname{prof}_A(M) - 1$ (§ 1, No. 4, mệnh đề 7).

Xét dãy khớp các môđun mở rộng

$$
\operatorname{Ext}_A^i(M, \Omega) \xrightarrow{x} \operatorname{Ext}_A^i(M, \Omega) \longrightarrow \operatorname{Ext}_A^{i+1}(M/xM, \Omega)
$$

liên kết với dãy khớp

$$
0 \to M \xrightarrow{x} M \longrightarrow M/xM \to 0 .
$$

Với $i > \dim(A) - \operatorname{prof}_A(M)$, $A$-môđun $\operatorname{Ext}_A^{i+1}(M/xM, \Omega)$ là không theo giả thiết quy nạp; bởi vậy phép vị tự có tỉ số $x$ là toàn ánh trong $\operatorname{Ext}_A^i(M, \Omega)$, điều này suy ra $A$-môđun này là không (bổ đề Nakayama). Điều này chứng minh c).

#### Hệ quả {#ac-x-s9-n1-cor-1 .statement}

*Nếu $M$ là Macaulay, thì $\operatorname{Ext}_A^i(M, \Omega) = 0$ với $i \neq c$; $A$-môđun $\operatorname{Ext}_A^c(M, \Omega)$ là Macaulay, và giá của nó bằng giá của $M$.*

Mệnh đề thứ nhất suy ra từ Mệnh đề 3, a) và c). Cho $p \in \operatorname{Supp}(M)$; theo Mệnh đề 1 của § 2, No. 1, áp dụng cho $M$ và cho $A$, ta có

$$
\dim(A_p) - \dim_{A_p}(M_p) = \dim(A) - \dim_A(M) = c ;
$$

vì $A_p$-môđun $\Omega_p$ là đối ngẫu hóa (Mệnh đề 2), suy ra từ Mệnh đề 3, b) rằng $A_p$-môđun $\operatorname{Ext}_A^c(M_p, \Omega_p)$ khác không. Vậy giá của $\operatorname{Ext}_A^c(M, \Omega)$ bằng giá của $M$.

Sau cùng, hãy chứng minh, bằng quy nạp theo $\dim(M)$, rằng $A$-môđun $\operatorname{Ext}_A^c(M, \Omega)$ là Macaulay. Mệnh đề đúng khi $\dim(M) = 0$, vì mọi môđun có độ dài hữu hạn đều là Macaulay. Giả sử $\dim(M) > 0$ và chọn một phần tử $x$ của $\mathfrak{m}_A$ sao cho phép vị tự $x_M$ là đơn ánh. $A$-môđun $M/xM$ là Macaulay ($§ 2$, No. 3, Mệnh đề 4), có chiều $\dim(M) - 1$. Theo điều nói trên, dãy khớp của các môđun mở rộng liên kết với dãy khớp $0 \to M \xrightarrow{x} M \longrightarrow M/xM \to 0$ rút gọn thành

$$
0 \to \operatorname{Ext}_A^c(M, \Omega) \xrightarrow{x} \operatorname{Ext}_A^c(M, \Omega) \longrightarrow \operatorname{Ext}_A^{c+1}(M/xM, \Omega) \to 0 ;
$$

Mệnh đề 4 của § 2, No. 3 và giả thiết quy nạp khi đó suy ra $\operatorname{Ext}_A^c(M, \Omega)$ là Macaulay, do đó có hệ quả.

### 2. Thương bởi một dãy chính quy

#### Mệnh đề 4 {#ac-x-s9-prop-4 .statement}

*Cho $A$ là một vành Noether, $J$ là một iđêan của $A$ sinh bởi một $A$-dãy chính quy $x$, và $\Omega$ là một $A$-môđun sinh hữu hạn.

a) Nếu $A$-môđun $\Omega$ là đối ngẫu hóa, thì dãy $x$ là $\Omega$-chính quy và $A/J$-môđun $\Omega/J\Omega$ là đối ngẫu hóa;

b) Nếu $A/J$-môđun $\Omega/J\Omega$ là đối ngẫu hóa, nếu $J$ được chứa trong căn của $A$, và nếu dãy $x$ là $\Omega$-chính quy, thì $A$-môđun $\Omega$ là đối ngẫu hóa.*

Lập luận bằng quy nạp theo độ dài của dãy $x$, ta được đưa về trường hợp dãy sau chỉ gồm một phần tử $x$. Giả sử rằng A-môđun $\Omega$ là đối ngẫu hóa. Với mọi iđêan cực đại $m$ của $A$ chứa $x$, ta có $\dim(A_m/xA_m) = \dim(A_m) - 1$

Kí hiệu \overline{A} là vành A/xA; cho m là một iđêan cực đại của A chứa x, và \overline{m} là ảnh của nó trong \overline{A}. A-môđun A/m bị triệt tiêu bởi x, và được đồng nhất với \overline{A}/\overline{m} ; do đó với mọi số nguyên i \geqslant 1 có một đẳng cấu Ext^i_A(A/m, \Omega) \longrightarrow \operatorname{Ext}^{i-1}_{\overline{A}}(\overline{A}/\overline{m}, \Omega/x\Omega) (§ 3, n° 4, mệnh đề 7). Ta có

$$
\operatorname{ht}(\overline{m}) = \dim(\overline{A}_m) = \dim(A_m/xA_m) = \dim(A_m) - 1 = \operatorname{ht}(m) - 1
$$

(VIII, § 3, n° 1, hệ quả 2, a)). Bây giờ các iđêan cực đại của \overline{A} là các iđêan \overline{m}, trong đó m là một iđêan cực đại của A chứa x; và hơn nữa nếu x thuộc căn của A, thì mọi iđêan cực đại của A đều chứa x. Mệnh đề được chứng minh.

#### Hệ quả 1 {#ac-x-s9-prop-4-cor-1 .statement}

**Cho A là một vành nguyên Noether. Mọi A-môđun đối ngẫu hóa đều không xoắn và có hạng 1.**

Cho \Omega là một A-môđun đối ngẫu hóa; nó không xoắn theo mệnh đề 4. Kí hiệu K là trường các phân thức của A; không gian vectơ trên K K \otimes_A \Omega là đối ngẫu hóa (n° 1, mệnh đề 2), do đó có chiều 1.

#### Hệ quả 2 {#ac-x-s9-prop-4-cor-2 .statement}

**Cho A là một vành Macaulay địa phương, \Omega một A-môđun hữu hạn sinh, và x một dãy cát tuyến cực đại gồm các phần tử của m_A, sinh ra một iđêan J. Các điều kiện sau là tương đương:**

(i) A-môđun \Omega là đối ngẫu hóa ;
(ii) A-môđun \Omega là một môđun Macaulay có chiều bằng \dim(A), và \Omega/J\Omega là một môđun nội xạ không phân tích được trên vành Artin địa phương A/J ;
(iii) dãy x là \Omega-chính quy và \Omega/J\Omega là một môđun nội xạ không phân tích được trên vành Artin địa phương A/J ;
(iv) dãy x là \Omega-chính quy, ta có \operatorname{long}_A(\Omega/J\Omega) = \operatorname{long}_A(A/J) và không gian vectơ trên \kappa_A \operatorname{Hom}_A(\kappa_A, \Omega/J\Omega) có chiều 1.

(i) \Rightarrow (ii) : nếu \Omega là đối ngẫu hóa, thì nó là Macaulay và có chiều \dim(A) (n° 1, mệnh đề 1). Dãy x là A-chính quy vì A là một vành Macaulay; theo mệnh đề 4, A/J-môđun \Omega/J\Omega là đối ngẫu hóa, và do đó là một A/J-môđun Matlis (n° 1, ví dụ 1).

(ii) \Rightarrow (iii) : dưới giả thiết (ii), ta có \dim(\Omega) = \dim(A) và \dim(\Omega/J\Omega) = \dim(A/J) = 0, nên dãy x là cát tuyến đối với \Omega, do đó \Omega-chính quy (§ 2, n° 3, định lý 1).

(iii) \Rightarrow (i) : dưới các giả thiết của (iii), A/J-môđun \Omega/J\Omega là một A-môđun Matlis, và do đó là đối ngẫu hóa (n° 1, ví dụ 1) ; theo mệnh đề 4, A-môđun \Omega là đối ngẫu hóa.

(iii) \Leftrightarrow (iv) : điều này suy ra từ nhận xét ở § 8, n° 3.

### 3. Thay đổi vành

#### Mệnh đề 5 {#ac-x-s9-prop-5 .statement}

Cho $\rho : A \to B$ là một đồng cấu của các vành Noether, biến $B$ thành một $A$-môđun phẳng. Giả sử rằng với mọi iđêan cực đại $n$ của $B$, vành $\kappa(\rho^{-1}(n)) \otimes_A B$ là một vành Gorenstein. Cho $\Omega$ là một $A$-môđun đối ngẫu hóa ; $B$-môđun $\Omega_{(B)}$ là đối ngẫu hóa.

Cho $n$ là một iđêan cực đại của $B$, và $p$ là ảnh ngược của nó trong $A$. $A_p$-môđun $B_n$ là phẳng, $A_p$-môđun $\Omega_p$ là đối ngẫu hóa, $\Omega_{(B)} \otimes_B B_n$ được đồng nhất với $\Omega_p \otimes_{A_p} B_n$ và $\kappa_{A_p} \otimes_{A_p} B_n$, được đồng nhất với một vành phân thức của $\kappa(p) \otimes_A B$, là một vành Gorenstein. Vì vậy đủ để chứng minh mệnh đề trong trường hợp $\rho$ là một đồng cấu địa phương của các vành địa phương, điều mà từ nay ta sẽ giả sử.

Trước hết hãy xét trường hợp các vành $A$ và $B$ là Artin. Đặt $C = B/\mathfrak{m}_A B$. Vì $B$ là phẳng trên $A$, $B$-môđun $\mathrm{Hom}_B(C, \Omega_{(B)})$ đẳng cấu với $\mathrm{Hom}_A(\kappa_A, \Omega) \otimes_A B$ (I, § 2, n° 10, mệnh đề 11), do đó với $\mathrm{Hom}_A(\kappa_A, \Omega) \otimes_{\kappa_A} C$. Suy ra một dãy các đẳng cấu

$$
\mathrm{Hom}_B(\kappa_B, \Omega_{(B)}) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_B(C, \Omega_{(B)})) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_A(\kappa_A, \Omega) \otimes_{\kappa_A} C)
$$
$$
\longrightarrow \mathrm{Hom}_A(\kappa_A, \Omega) \otimes_{\kappa_A} \mathrm{Hom}_C(\kappa_C, C) .
$$

Không gian vectơ trên $\kappa_A$ $\mathrm{Hom}_A(\kappa_A, \Omega)$ có chiều 1 vì $\Omega$ là đối ngẫu hóa, và điều tương tự cũng đúng với không gian vectơ trên $\kappa_C$ $\mathrm{Hom}_C(\kappa_C, C)$ vì $C$ là một vành Gorenstein; do đó không gian vectơ trên $\kappa_B$ $\mathrm{Hom}_B(\kappa_B, \Omega_{(B)})$ có chiều 1.

Cho $M$ là một $B$-môđun có độ dài hữu hạn; ta hãy chứng minh bằng quy nạp theo $\mathrm{long}_B(M)$ rằng ta có $\mathrm{long}_B(\mathrm{Hom}_B(M, \Omega_{(B)})) \leqslant \mathrm{long}_B(M)$. Mệnh đề là hiển nhiên nếu $M = 0$, và điều đó suy ra từ điều đi trước nếu $M = \kappa_B$. Giả sử $\mathrm{long}_B(M) \geqslant 2$. Tồn tại một dãy khớp các $B$-môđun
$$
0 \to M' \to M \to \kappa_B \to 0
$$
với $\mathrm{long}_B(M') < \mathrm{long}_B(M)$. Từ đó suy ra một dãy khớp
$$
0 \to \mathrm{Hom}_B(\kappa_B, \Omega_{(B)}) \to \mathrm{Hom}_B(M, \Omega_{(B)}) \to \mathrm{Hom}_B(M', \Omega_{(B)}) ,
$$
và ta kết luận bằng cách áp dụng giả thiết quy nạp cho $M'$.

Cho $N$ là hạt nhân của toàn cấu chính tắc từ $\kappa_A \otimes_A B$ lên $\kappa_B$. Đặt $m = \mathrm{long}_B(\kappa_A \otimes_A B)$; ta có $\mathrm{long}_B(N) = m - 1$. Xét dãy khớp các $B$-môđun
$$
0 \to \mathrm{Hom}_B(\kappa_B, \Omega_{(B)}) \longrightarrow \mathrm{Hom}_B(\kappa_A \otimes_A B, \Omega_{(B)}) \longrightarrow \mathrm{Hom}_B(N, \Omega_{(B)})
$$
$$
\longrightarrow \mathrm{Ext}_B^1(\kappa_B, \Omega_{(B)}) \longrightarrow \mathrm{Ext}_B^1(\kappa_A \otimes_A B, \Omega_{(B)}) .
$$

Các $B$-môđun $\mathrm{Hom}_B(\kappa_A \otimes_A B, \Omega_{(B)})$ và $\mathrm{Ext}_B^1(\kappa_A \otimes_A B, \Omega_{(B)})$ lần lượt đẳng cấu với $\mathrm{Hom}_A(\kappa_A, \Omega) \otimes_A B$ và $\mathrm{Ext}_A^1(\kappa_A, \Omega) \otimes_A B$, nghĩa là với $\kappa_A \otimes_A B$ và với 0. Độ dài của các $B$-môđun $\mathrm{Hom}_B(\kappa_B, \Omega_{(B)})$ và $\mathrm{Hom}_B(\kappa_A \otimes_A B, \Omega_{(B)})$ là 1 và $m$, và độ dài của $\mathrm{Hom}_B(N, \Omega_{(B)})$) là $\leqslant m - 1$; từ đó suy ra $B$-môđun $\mathrm{Ext}_B^1(\kappa_B, \Omega_{(B)})$ là không. Theo Mệnh đề 6 của § 3, No. 3, $B$-môđun $\Omega_{(B)}$ là nội xạ; do đó nó là một môđun đối ngẫu hóa (No. 1, Ví dụ 1).

Ta chuyển sang trường hợp tổng quát. Đặt $C = \kappa_A \otimes_A B$; theo giả thiết đây là một vành Gorenstein, do đó là một vành Macaulay ($§ 3, n° 7$, mệnh đề 10). Theo mệnh đề 1 của No. 1, $A$ là một vành Macaulay, và $A$-môđun $\Omega$ là Macaulay. Do đó $B$ là một vành Macaulay, và $B$-môđun $\Omega_{(B)}$ là Macaulay ($§ 2, n° 7$, hệ quả 1 của mệnh đề 9). Đặt $r = \dim(A)$, $s = \dim(C)$. Tồn tại một dãy $(x_1, \ldots, x_r)$ các phần tử của $\mathfrak{m}_A$ chính quy đối với các $A$-môđun $A$ và $\Omega$, và một dãy $(y_1, \ldots, y_s)$ các phần tử của $\mathfrak{m}_B$ chính quy đối với $B$-môđun $C$; gọi $x$ là iđêan của $A$ và $\mathfrak{g}$ là iđêan của $B$ lần lượt được sinh bởi chúng. Dãy $(y_1, \ldots, y_s, \rho(x_1), \ldots, \rho(x_r))$ là chính quy đối với các $B$-môđun $B$ và $\Omega_{(B)}$ ($§ 1, n° 6$, mệnh đề 11), và $A$-môđun $B/\mathfrak{g}$ là phẳng (*loc. cit.*, mệnh đề 10). Đặt $A' = A/x$, $B' = B/(xB + \mathfrak{g})$ và gọi $\rho' : A' \to B'$ là đồng cấu suy ra từ $\rho$ bằng cách chuyển qua các thương. Các vành $A'$ và $B'$ là Artin, $A'$-môđun $B'$ là phẳng, vành $\kappa_{A'} \otimes_{A'} B'$, được đồng nhất với $C/\mathfrak{g}$, là một vành Gorenstein ($§ 3, n° 7$, ví dụ 2) và $A'$-môđun $\Omega_{(A')}$ là đối ngẫu hóa (No. 2, mệnh đề 4). Theo phần đầu của chứng minh, $B'$-môđun $\Omega_{(B')}$ là đối ngẫu hóa. Khi đó suy ra từ *loc. cit.* rằng $B$-môđun $\Omega_{(B)}$ là đối ngẫu hóa.

#### Hệ quả {#ac-x-s9-n3-cor-1 .statement}

*Cho $A$ là một vành Noether nhận một môđun đối ngẫu hóa $\Omega$; cho $B$ là một đại số đa thức trên $A$ theo một số hữu hạn bất định. $B$-môđun $\Omega_{(B)}$ là đối ngẫu hóa.*

Thật vậy, với mọi iđêan nguyên tố $\mathfrak{p}$ của $A$, vành $\kappa(\mathfrak{p}) \otimes_A A[X]$ được đồng nhất với $\kappa(\mathfrak{p})[X]$, là vành chính quy, do đó Gorenstein.

#### Mệnh đề 6 {#ac-x-s9-prop-6 .statement}

*Cho $\Lambda$ là một vành địa phương Noether và $\Omega$ là một A-môđun đối ngẫu hóa. Cho $B$ là một A-đại số hữu hạn; giả sử rằng A-môđun $B$ là Macaulay. B-môđun $\mathrm{Ext}_A^i(B, \Omega)$ bằng không với $i \neq \dim(A) - \dim(B)$ và là đối ngẫu hóa với $i = \dim(A) - \dim(B)$.

Ta có $\dim(B) = \dim_A(B) \leq \dim(\Lambda)$ (VIII, § 2, No. 3, Định lý 1 c)); đặt $c = \dim(A) - \dim(B)$. Ta có $\mathrm{Ext}_A^i(B, \Omega) = 0$ với $i \neq c$ vì A-môđun $B$ là Macaulay (No. 1, Hệ quả của Mệnh đề 3). Hãy chứng minh rằng B-môđun $\mathrm{Ext}_A^c(B, \Omega)$ là đối ngẫu hóa.

Trước hết giả sử rằng $\dim(B) = 0$. Phổ $X$ của $B$ là hữu hạn và gồm các iđêan cực đại (IV, § 2, No. 5, Mệnh đề 9); ánh xạ chính tắc $B \to \prod_{n \in X} B_n$ là một đẳng cấu (*loc. cit.*, Hệ quả 1). B-môđun $\Omega' = \mathrm{Ext}_A^c(B, \Omega)$ do đó là tổng trực tiếp của các môđun $\mathrm{Ext}_A^c(B_n, \Omega)$; vì $\mathrm{Ext}_A^c(B_n, \Omega)$ có giá trong $\{n\}$, nó được đồng nhất với $\Omega'_n$. Ta có $\dim(B_n) = 0$ với mọi $n$; do đó, để chứng minh rằng B-môđun $\Omega'$ là đối ngẫu hóa, chỉ cần chứng minh điều này cho B_n-môđun $\mathrm{Ext}_A^c(B_n, \Omega)$ với mọi $n \in X$, điều này đưa ta trở lại trường hợp vành $B$ là *địa phương*. Trong trường hợp này, theo Ví dụ 6 của § 8, No. 5, B-môđun $\mathrm{Ext}_A^c(B, \Omega)$ đẳng cấu với $\mathrm{Hom}_A(B, I)$, trong đó $I$ là một A-môđun Matlis; do đó nó là một B-môđun Matlis (§ 8, No. 6, Hệ quả của Mệnh đề 5), vậy nên là một B-môđun đối ngẫu hóa (No. 1, Ví dụ 1).

Bây giờ giả sử rằng $\dim(B) > 0$ và lập luận bằng quy nạp theo $\dim(B)$. Ta có $\mathrm{prof}_A(B) = \dim_A(B) = \dim(B)$, do đó $\mathrm{prof}_A(B) > 0$; mặt khác ta có $\mathrm{prof}(A) = \dim(A) > 0$ (No. 1, Mệnh đề 1), và do đó $\mathrm{prof}_A(A \oplus B) > 0$. Vì thế tồn tại một phần tử $x$ của $\mathfrak{m}_A$ sao cho các phép vị tự $x_A$ và $x_B$ là đơn ánh.

Xét dãy khớp các môđun mở rộng liên kết với dãy khớp $0 \to B \xrightarrow{x_B} B \longrightarrow B/xB \to 0$ và với $A$-môđun $\Omega$. $A$-môđun $B/xB$ là Macaulay ($§ 2$, No. 1, Ví dụ 3), có chiều $\dim(B) - 1$ (VIII, $§ 3$, No. 2, Mệnh đề 3) ; do đó ta có $\mathrm{Ext}_A^i(B/xB, \Omega) = 0$ với $i \neq c + 1$ (No. 1, Hệ quả của Mệnh đề 3). Vì ta có $\mathrm{Ext}_A^i(B, \Omega) = 0$ với $i \neq c$, nên ta thu được một dãy khớp các $B$-môđun

$$
0 \to \mathrm{Ext}_A^c(B, \Omega) \xrightarrow{x} \mathrm{Ext}_A^c(B, \Omega) \longrightarrow \mathrm{Ext}_A^{c+1}(B/xB, \Omega) \to 0 .
$$

Theo giả thiết quy nạp, $B/xB$-môđun $\mathrm{Ext}_A^{c+1}(B/xB, \Omega)$ là đối ngẫu hóa. Vì đại số trên $A$ $B$ là hữu hạn, ảnh của $m_A$ trong $B$ được chứa trong căn của $B$ (V, $§ 2$, No. 1, Mệnh đề 1) ; theo Mệnh đề 4 của No. 2, $B$-môđun $\mathrm{Ext}_A^c(B, \Omega)$ là đối ngẫu hóa.

#### Hệ quả 1 {#ac-x-s9-prop-6-cor-1 .statement}

*Cho A là một vành Noether, $\Omega$ một A-môđun đối ngẫu hóa, và B một đại số trên A hữu hạn; giả sử rằng A-môđun B là Macaulay. B-môđun $\mathrm{Ext}_A(B, \Omega)$ là đối ngẫu hóa.*

Ký hiệu $\Omega'$ là $B$-môđun $\mathrm{Ext}_A(B, \Omega)$. Cho $n$ là một iđêan cực đại của $B$; ảnh ngược của nó trong $A$ là một iđêan cực đại $m$ (V, $§ 2$, No. 1, mệnh đề 1). Đại số trên $A_m$ $B_m = A_m \otimes_A B$ là hữu hạn, và là một $A_m$-môđun Macaulay; theo mệnh đề, $B_m$-môđun $\Omega'_m$, đồng nhất với $\mathrm{Ext}_{A_m}(B_m, \Omega_m)$ ($§ 3$, No. 2, mệnh đề 2), là đối ngẫu hóa. Vì $B_n$ là một vành phân thức của $B_m$, nên $B_n$-môđun $\Omega'_n$ là đối ngẫu hóa, do đó có hệ quả.

#### Nhận xét {#ac-x-s9-n3-rem-1 .statement}

Giữ các giả thiết của hệ quả 1 và giả sử thêm rằng đồng cấu chính tắc $\rho : A \to B$ là đơn ánh. Khi đó ta có $\dim(A_m) = \dim(B_m)$ với mọi iđêan cực đại $m$ của $A$ (VIII, $§ 2$, No. 3, định lý 1 a)). Theo mệnh đề 6 và hệ quả 1, $\mathrm{Ext}_A^i(B, \Omega)$ bằng không với $i \neq 0$, và $B$-môđun $\mathrm{Hom}_A(B, \Omega)$ là đối ngẫu hóa.

#### Hệ quả 2 {#ac-x-s9-prop-6-cor-2 .statement}

*Nếu một vành Noether $A$ có một môđun đối ngẫu hóa, thì mọi đại số trên $A$ sinh hữu hạn là một vành Macaulay đều có một môđun đối ngẫu hóa.*

Điều này suy ra từ hệ quả 1 và hệ quả của mệnh đề 5.

#### Hệ quả 3 {#ac-x-s9-prop-6-cor-3 .statement}

*Mọi vành Macaulay biểu diễn được (đặc biệt, mọi vành địa phương Macaulay đầy đủ) đều có một môđun đối ngẫu hóa.*

Thật vậy, cho $R$ là một vành chính quy và $A$ là một thương của $R$ mà là một vành Macaulay. $A$-môđun $A$ là một môđun Macaulay ($§ 2$, No. 5, ví dụ 5), và $R$ có một môđun đối ngẫu hóa (No. 1, ví dụ 2); do đó điều ấy cũng đúng với $A$ theo hệ quả 1. Hơn nữa, đã nhận thấy rằng một vành địa phương Noether đầy đủ là biểu diễn được ($§ 4$, No. 4, mệnh đề 6, c)).

Nói chung hơn, mọi thương vành Macaulay của một vành Gorenstein đều có một môđun đối ngẫu hóa. Ngược lại, có thể chứng minh rằng một vành địa phương Macaulay có một môđun đối ngẫu hóa là một thương của một vành địa phương Gorenstein (bài tập 1).

### 4. Cấu trúc của các môđun đối ngẫu hóa

#### Bổ đề 2 {#ac-x-s9-lem-2 .statement}

Cho $A$ là một vành Noether, $M$ và $N$ là các $A$-môđun sinh hữu hạn, $u : M \to N$ là một đồng cấu. Cho $x$ là một phần tử của căn của $A$, sao cho phép vị tự $x_N$ là đơn ánh. Nếu đồng cấu $\overline{u} : M/xM \to N/xN$ được cảm sinh bởi $u$ là đơn ánh (tương ứng, toàn ánh, tương ứng, song ánh), thì $u$ cũng có tính chất đó.

Mệnh đề liên quan đến tính toàn ánh của $u$ suy ra từ bổ đề Nakayama (II, § 3, No. 2, hệ quả 1 của mệnh đề 4), không cần giả thiết nào trên $x_N$. Xét biểu đồ giao hoán với các hàng khớp

$$
\begin{array}{ccccccc}
M & \xrightarrow{x_M} & M & \longrightarrow & M/xM \\
\downarrow u & & \downarrow u & & \downarrow \overline{u} \\
0 & \longrightarrow & N & \xrightarrow{x_N} & N & \longrightarrow & N/xN ;
\end{array}
$$

nhờ bổ đề con rắn (I, § 1, No. 4, mệnh đề 2), ta suy ra từ đó một dãy khớp $\mathrm{Ker}\, u \xrightarrow{x} \mathrm{Ker}\, u \longrightarrow \mathrm{Ker}\, \overline{u}$. Nếu $\overline{u}$ là đơn ánh, thì phép vị tự với tỷ số $x$ là toàn ánh trong $\mathrm{Ker}\, u$, điều này kéo theo $\mathrm{Ker}\, u = 0$ bởi bổ đề Nakayama.

#### Mệnh đề 7 {#ac-x-s9-prop-7 .statement}

Cho $A$ là một vành Noether và $\Omega$ là một $A$-môđun đối ngẫu hóa.

a) Ta có $\mathrm{Ext}_A^i(\Omega, \Omega) = 0$ với $i > 0$.

b) Đồng cấu chính tắc $\gamma : A \to \mathrm{End}_A(\Omega)$ là song ánh.

c) Mọi $A$-môđun đối ngẫu hóa đều có dạng $\Omega \otimes_A L$ trong đó $L$ là một $A$-môđun xạ ảnh hạng 1.

A) Trước hết ta xét trường hợp vành $A$ là địa phương. Trong trường hợp này điều kiện c) đơn giản chỉ có nghĩa là hai môđun đối ngẫu hóa là đẳng cấu.

Cho $\Omega'$ là một $A$-môđun đối ngẫu hóa. Ta có $\mathrm{prof}_A(\Omega') = \dim_A(\Omega') = \dim(A)$ (No. 1, mệnh đề 1), do đó $\mathrm{Ext}_A^i(\Omega', \Omega) = 0$ với $i \neq 0$ (No. 1, mệnh đề 3, c)), do đó suy ra a).

Ta chứng minh b) và c) bằng quy nạp theo số nguyên $\dim(A)$ (bằng $\mathrm{prof}(A)$). Nếu nó bằng không, thì vành $A$ là Artin, $\Omega'$ và $\Omega$ là các Matlis $A$-môđun (No. 1, Ví dụ 1); do đó chúng đẳng cấu ($\S$ 8, No. 1, Prop. 1) và ánh xạ chính tắc $A \to \mathrm{End}_A(\Omega)$ là song ánh ($\S$ 8, No. 2, Prop. 3, c)). Giả sử $\dim(A) > 0$ và cho $x$ là một phần tử giản ước được của $\mathfrak{m}_A$. Phép vị tự $x_\Omega$ là đơn ánh (No. 2, Prop. 4), và ta có một dãy khớp

$$
0 \to \Omega \xrightarrow{x_\Omega} \Omega \longrightarrow \Omega/x\Omega \to 0 .
$$

Vì $\mathrm{Ext}_A^1(\Omega', \Omega)$ bằng không và $\mathrm{Hom}_A(\Omega', \Omega/x\Omega)$ được đồng nhất với $\mathrm{Hom}_{A/xA}(\Omega'/x\Omega', \Omega/x\Omega)$, ta suy ra một dãy khớp

$$
(1)\quad 0 \to \mathrm{Hom}_A(\Omega', \Omega) \xrightarrow{x} \mathrm{Hom}_A(\Omega', \Omega) \xrightarrow{p} \mathrm{Hom}_{A/xA}(\Omega'/x\Omega', \Omega/x\Omega) \to 0 ,
$$

trong đó $p$ là ánh xạ chính tắc. Theo Mệnh đề 4, các $A/xA$-môđun $\Omega/x\Omega$ và $\Omega'/x\Omega'$ là đối ngẫu hoá, nên đẳng cấu theo giả thiết quy nạp. Gọi $\overline{u}$ là một đẳng cấu từ $\Omega'/x\Omega'$ lên $\Omega/x\Omega$. Xét dãy khớp (1), tồn tại một đồng cấu $A$-môđun $u : \Omega' \to \Omega$ sao cho $p(u) = \overline{u}$; theo Bổ đề 2, $u$ là song ánh, điều này chứng minh c). Theo giả thiết quy nạp, đồng cấu chính tắc $A/xA \longrightarrow \mathrm{End}_{A/xA}(\Omega/x\Omega)$ là song ánh. Xét dãy khớp (1), đồng cấu này được đồng nhất với đồng cấu $\overline{\gamma} : A/xA \longrightarrow \mathrm{End}_A(\Omega)/x\mathrm{End}_A(\Omega)$ cảm sinh bởi $\gamma$; khi đó từ Bổ đề 2 suy ra $\gamma$ là song ánh, do đó b).

B) Ta chuyển sang trường hợp tổng quát. Với mọi iđêan cực đại $m$ của $A$ và mọi số nguyên $i > 0$, ta có $\mathrm{Ext}^i_{A_m}(\Omega_m, \Omega_m) = 0$ theo điều đã nói ở trên, nên $\mathrm{Ext}^i_A(\Omega, \Omega)_m = 0$ ($§ 3$, No. 2, Prop. 2), điều này kéo theo $\mathrm{Ext}^i_A(\Omega, \Omega) = 0$ (II, $§ 3$, No. 3, Hệ quả 2 của Định lý 1). Tương tự, đồng cấu $\gamma_m : A_m \to \mathrm{End}_A(\Omega)_m$ là song ánh với mọi iđêan cực đại $m$ của $A$, nên $\gamma$ là song ánh (*loc. cit.*, Định lý 1).

Cuối cùng, ta chứng minh c). Gọi $\Omega'$ là một $A$-môđun đối ngẫu hoá. Kí hiệu $L$ là $A$-môđun $\mathrm{Hom}_A(\Omega', \Omega)$, và $v : \Omega' \otimes_A L \to \Omega$ là đồng cấu sao cho $v(x \otimes f) = f(x)$ với $x \in \Omega'$, $f \in L$. Gọi $m$ là một iđêan cực đại của $A$. $A_m$-môđun $L_m$ được đồng nhất với $\mathrm{Hom}_{A_m}(\Omega'_m, \Omega_m)$; theo trường hợp đã xét, nó tự do hạng một, và mọi đẳng cấu $h : \Omega'_m \to \Omega_m$ là một phần tử sinh của nó. Khi đồng nhất $L_m$ với $A_m$ nhờ phần tử sinh $h$, đồng cấu $v_m : \Omega'_m \otimes_{A_m} L_m \to \Omega_m$ được đồng nhất với $h$, nên là song ánh. Vì điều này đúng với mọi iđêan cực đại $m$ của $A$, $A$-môđun $L$ là xạ ảnh hạng một (II, $§ 5$, No. 3, Định lý 2), và đồng cấu $v$ là song ánh (II, $§ 3$, No. 3, Định lý 1).

#### Hệ quả 1 {#ac-x-s9-prop-7-cor-1 .statement}

*Để $A$ là một vành Gorenstein, điều kiện cần và đủ là A-môđun $\Omega$ xạ ảnh hạng 1*.

Điều này suy ra từ Ví dụ 2 của No. 1 và Mệnh đề 7 c).

#### Hệ quả 2 {#ac-x-s9-prop-7-cor-2 .statement}

*Giả sử rằng vành $A$ là trình bày được. Tập hợp các iđêan nguyên tố $p$ của $A$ sao cho $A_p$ là một vành Gorenstein là mở trong $\mathrm{Spec}(A)$*.

Cho $p$ là một iđêan nguyên tố của $A$ sao cho $A_p$ là một vành Gorenstein. Khi đó nó là một vành Macaulay; nếu cần, thay thế $A$ bởi $A_f$, trong đó $f$ là một phần tử thích hợp của $A - p$, ta quy về trường hợp trong đó $A$ là một vành Macaulay ($§ 4$, No. 4, Mệnh đề 7, c)). Gọi $\Omega$ là một A-môđun đối ngẫu hóa (No. 3, Hệ quả 3 của Mệnh đề 6). Khi đó $\Omega_p$ là một môđun đối ngẫu hóa trên vành Gorenstein $A_p$ (No. 1, Mệnh đề 2), nên tự do hạng 1 (Hệ quả 1). Suy ra tồn tại một phần tử $g$ của $A - p$ sao cho A-môđun $\Omega_g$ tự do hạng 1 (II, $§ 5$, No. 1, Hệ quả của Mệnh đề 2). Do đó $A_g$ là một vành Gorenstein (Hệ quả 1) và điều tương tự cũng đúng với $A_q$ đối với mọi iđêan nguyên tố $q$ của $A$ không chứa $g$ ($§ 3$, No. 7, Ví dụ 1), điều này chứng minh hệ quả.

### 5. Đối ngẫu của các môđun kiểu hữu hạn

Trong số này ta xét một vành Noether $A$ *có số chiều hữu hạn* có một môđun đối ngẫu hóa $\Omega$. Khi đó $\mathrm{di}_A(\Omega) = \dim(A) < +\infty$ (No. 1, Prop. 1). *Chọn một phân giải nội xạ có độ dài hữu hạn* $e : \Omega \to (I, \delta)$. Với mọi phức $C$ các A-môđun, ký hiệu $D(C)$ là phức $\mathrm{Homgr}_A(C, I)$. Điều này đặc biệt áp dụng cho mọi A-môđun $M$, được xem như một phức tập trung ở bậc 0; khi đó ta có $D(M)^i = \mathrm{Hom}_A(M, I^i)$ với mọi số nguyên $i$. Nhắc lại rằng trong A, X, p. 100, Định lý 1, ta đã xây dựng một đẳng cấu chính tắc

$$
\varphi(M, I) : H(D(M)) \longrightarrow \mathrm{Ext}_A(M, \Omega)
$$

*Ví dụ.* 1) Phức $D(A) = \mathrm{Homgr}_A(A, 1)$ được đồng nhất với $I$. Ánh xạ $e : \Omega \to D(A)$ theo định nghĩa là một đồng cấu đồng điều.

2) Đồng cấu $e \in \mathrm{Homgr}_A(\Omega, I)^0$ là một phần tử của $D(\Omega)^0$; ánh xạ A-tuyến tính $\tilde{e} : A \to D(\Omega)$ sao cho $\tilde{e}(1) = e$ là một đồng cấu đồng điều (No. 4, Prop. 7, a) và b)).

3) Cho S là một tập con nhân tính của A. $S^{-1}A$-môđun $S^{-1}\Omega$ là đối ngẫu hoá (No. 1, Hệ quả 1 của Mệnh đề 2); các $S^{-1}A$-môđun $S^{-1}I^i$ là đơn ánh (Hệ quả 1 của Mệnh đề 3 của § 3, No. 2) và cấu xạ $e' : S^{-1}\Omega \to S^{-1}I$ suy ra từ $e$ là một phân giải đơn ánh của $S^{-1}\Omega$, do đó có thể áp dụng điều vừa nói ở trên cho nó. Với mọi phức C kiểu hữu hạn (và đặc biệt với mọi A-môđun M kiểu hữu hạn), đồng cấu chính tắc từ $S^{-1}D(C)$ vào $\mathrm{Homgr}_{S^{-1}A}(S^{-1}C, S^{-1}I) = D(S^{-1}C)$ là song ánh.

4) Cho A là một vành Dedekind, K trường phân thức của nó. A-môđun A là đối ngẫu hoá và có một phân giải đơn ánh I độ dài 1 được xác định bởi dãy khớp

$$
0 \to A \xrightarrow{e} K \xrightarrow{\delta} K/A \to 0
$$

trong đó $\delta$ là toàn cấu chính tắc. Với mọi A-môđun M, phức $D(M)$ là phức tập trung ở các bậc 0 và 1

$$
\ldots \longrightarrow 0 \longrightarrow \mathrm{Hom}_A(M, K) \xrightarrow{d} \mathrm{Hom}_A(M, K/A) \longrightarrow 0 \longrightarrow \ldots
$$

với $d = \mathrm{Hom}_A(1_M, \delta)$. Ta có một dãy khớp

$$
0 \to \mathrm{Hom}_A(M, A) \longrightarrow D(M)^0 \xrightarrow{d} D(M)^1 \longrightarrow \mathrm{Ext}_A^1(M, A) \to 0 .
$$

Với mọi cấu xạ của các phức $f : C \to C'$, ta ký hiệu bởi $D(f) : D(C') \to D(C)$ cấu xạ của các phức $\mathrm{Homgr}_A(f, 1_I)$. Nếu $f$ là một đồng cấu trên đồng điều, thì $D(f)$ là một đồng cấu trên đồng điều (A, X, p. 86, Mệnh đề 4, b)). Nếu $C' \xrightarrow{f} C \xrightarrow{g} C''$ là một dãy khớp của các phức, thì dãy các phức $D(C'') \xrightarrow{D(g)} D(C) \xrightarrow{D(f)} D(C')$ là khớp (A, X, p. 83, Mệnh đề 2, a)).

Cho M là một A-môđun. Với mỗi phần tử $m$ của M, ta gán ánh xạ $\alpha_M(m) : f \mapsto f(m)$ từ $D(M)$ vào I; đó là một phần tử của $D(D(M))_0 = \mathrm{Homgr}_A(D(M), I)_0$. Từ các định nghĩa suy ra rằng $\alpha_M(m)$ là một cấu xạ của các phức, vì vậy là một phần tử của $Z_0(D(D(M)))$.

Như vậy ta xác định được một cấu xạ các phức:

$$
\alpha_M : M \to D(D(M)),
$$

do đó, khi chuyển qua đồng điều, một đồng cấu các A-môđun

$$
\alpha_M : M \to H_0(D(D(M))).
$$

#### Định lý 1 {#ac-x-s9-thm-1 .statement}

**Cho $M$ là một $A$-môđun sinh hữu hạn. Khi đó $\alpha_M$ là một đồng cấu trên đồng điều: ta có $H_i(D(D(M))) = 0$ với $i \neq 0$ và đồng cấu $\alpha_M$ là song ánh.**

Trước hết hãy lấy $M = A$. Ánh xạ $e : \Omega \to D(A)$ là một đồng cấu (Ví dụ 1), do đó ánh xạ $D(e) : D(D(A)) \to D(\Omega)$ cũng vậy. Ánh xạ $\tilde{e} : A \to D(\Omega)$ là một đồng cấu (Ví dụ 2), và ta có $D(e) \circ \alpha_A = \tilde{e}$; do đó $\alpha_A$ là một đồng cấu, điều này chứng minh định lý trong trường hợp này. Suy ra rằng $\alpha_M$ là một đồng cấu khi A-môđun $M$ là một môđun tự do sinh hữu hạn.

Hãy chuyển sang trường hợp tổng quát; ta sẽ chứng minh bằng quy nạp theo số nguyên $n$ mệnh đề sau:

$(A_n)$ *với mọi $A$-môđun sinh hữu hạn $M$, đồng cấu $H_i(\alpha_M)$ là song ánh với $i \leq n$.*

Điều này cũng có nghĩa là $H_i(D(D(M)))$ bằng không với $i \neq 0$ và $i \leq n$, và rằng $\alpha_M$ là song ánh nếu $n \geq 0$. Ta nhận thấy rằng $(A_n)$ đúng với $n < -d$, trong đó $d$ là độ dài của phức $I$; thật vậy, A-môđun $D(D(M))_i$ bằng $\bigoplus_p \mathrm{Hom}_A(\mathrm{Hom}_A(M, I^p), I^{p-i})$, và do đó bằng không với $i < -d$ và $i > d$.

Ta hãy chứng minh kéo theo $(A_n) \Rightarrow (A_{n+1})$. Cho $M$ là một A-môđun sinh hữu hạn. Tồn tại một A-môđun tự do sinh hữu hạn $L$ và một dãy khớp $0 \to N \xrightarrow{u} L \xrightarrow{v} M \to 0$.

Dãy $0 \to D(M) \xrightarrow{D(v)} D(L) \xrightarrow{D(u)} D(N) \to 0$ là khớp; tương tự, nếu ta đặt $u' = D(D(u))$ và $v' = D(D(v))$, thì dãy $0 \to D(D(N)) \xrightarrow{u'} D(D(L)) \xrightarrow{v'} D(D(M)) \to 0$ là khớp.

Vì $H_i(D(D(L)))$ bằng không với $i \neq 0$, ta có các đẳng cấu

$$
H_i(D(D(M)))) \longrightarrow H_{i-1}(D(D(N))) \quad \text{với } i \neq 0, 1 ;
$$

điều này cho kéo theo $(A_n) \Rightarrow (A_{n+1})$ với $n \neq -1$ và $n \neq 0$. Xét biểu đồ giao hoán với các hàng khớp

$$
\begin{array}{ccccccccc}
0 & \to & N & \xrightarrow{u} & L & \xrightarrow{v} & M & \to & 0 \\
& & \downarrow{\alpha_N} & & \downarrow{\alpha_L} & & \downarrow{\alpha_M} & & \\
0 & \to & H_1(D(D(M))) & \longrightarrow & H_0(D(D(N))) & \xrightarrow{H_0(u')} & H_0(D(D(L))) & \xrightarrow{H_0(v')} & H_0(D(D(M))) \longrightarrow H_{-1}(D(D(N)))
\end{array}
$$

trong đó $\alpha_L$ là song ánh. Nếu $(A_0)$ đúng, đồng cấu $\alpha_N$ cũng song ánh, do đó $H_0(u')$ là đơn ánh và suy ra $H_1(D(D(M))) = 0$, do đó có $(A_1)$. Nếu $(A_{-1})$

Vậy $(A_n)$ đúng với mọi $n$, điều này chứng minh định lý.

Cho $M$ là một A-môđun sinh hữu hạn; đặt $c = \dim(A) - \dim_A(M)$. Ký hiệu $D'(M)$ là phức con của $D(M)$ bằng $\bigoplus_{i < c} D(M)^i \bigoplus Z^c(D(M))$, và

$$
j : D'(M) \to D(M)
$$

là đơn ánh chính tắc. Từ toàn cấu chính tắc $Z^c(D(M)) \to H^c(D(M))$ và đẳng cấu $\varphi(M, I)$ suy ra một cấu xạ của các phức

$$
p : D'(M)(-c) \to \mathrm{Ext}_A^c(M, \Omega)
$$

vì $H^i(D(M))$ bằng không với $i < c$ (No. 1, mệnh đề 3 a)), $(D'(M)(-c), p)$ là một phân giải trái của $\mathrm{Ext}_A^c(M, \Omega)$. Theo A, X, p. 100, định lý 1, ta có một đẳng cấu chính tắc

$$
\varphi^0(D'(M)(-c), I) : H_0(D(D'(M))) \to \mathrm{Ext}_A^c(\mathrm{Ext}_A^c(M, \Omega), \Omega)
$$

hợp thành nó với đồng cấu $H_0(D(j)) : H_0(D(D(M))) \to H_0(D(D'(M)))$

do đó ta thu được một đồng cấu

$$
H_0(D(D(M))) \to \mathrm{Ext}_A^c(\mathrm{Ext}_A^c(M, \Omega), \Omega),
$$

do đó cuối cùng, bằng hợp thành với $\alpha_M$, một đồng cấu chính tắc

$$
\beta_M : M \to \mathrm{Ext}_A^c(\mathrm{Ext}_A^c(M, \Omega), \Omega).
$$

#### Hệ quả {#ac-x-s9-n5-cor-1 .statement}

Nếu $A$-môđun $M$ là Macaulay, đồng cấu $\beta_M$ là song ánh.

Nếu $M$ là Macaulay, $A$-môđun $H^i(D(M))$ bằng không với $i \neq c$ (No. 1, hệ quả của mệnh đề 3), nên đơn ánh chính tắc $j : D'(M) \to D(M)$ là một tương đương đồng điều; do đó cấu xạ của các phức $D(j) : D(D(M)) \to D(D'(M))$ là một tương đương đồng điều (A, X, p. 86, mệnh đề 4). Vì thế $H_0(D(j))$ là song ánh; mặt khác $\alpha_M$ là song ánh theo định lý 1, do đó có hệ quả.

Khi $A$-môđun $M$ có độ dài hữu hạn, $A$-môđun $\mathrm{Ext}_A^c(M, \Omega)$ được đồng nhất với đối ngẫu Matlis của $M$ ($cf.$ § 8, No. 5, ví dụ 3 và định lý 3), và ta thu lại mệnh đề 4 của § 8, No. 4.

### 6. Ví dụ: trường hợp chiều 1

Trong số này, ta xét một vành nguyên Noether $A$ có chiều 1 và nhận một môđun đối ngẫu hóa $\Omega$. Ký hiệu $K$ là trường phân thức của $A$, và $V$ là không gian vectơ trên K $K \otimes_A \Omega$.

Đồng cấu chính tắc $\Omega \to V$ là đơn ánh, và không gian vectơ trên K V có chiều 1 (No. 2, hệ quả 1 của mệnh đề 4); ta đồng nhất $\Omega$ với một môđun con trên A của V.

#### Mệnh đề 8 {#ac-x-s9-prop-8 .statement}

*$A$-môđun $V/\Omega$ là một môđun Matlis.*

Xét dãy khớp

$$
0 \to \Omega \to V \to V/\Omega \to 0 ;
$$

môđun trên A V là nội xạ (A, X, p. 18, ví dụ 1), và ta có $\mathrm{di}_A(\Omega) = 1$ (No. 1, mệnh đề 1). Một mặt suy ra rằng $V/\Omega$ là nội xạ (§ 3, No. 1, mệnh đề 1), mặt khác, với mọi iđêan cực đại $m$ của A, không gian vectơ trên $A/m$ $\mathrm{Hom}_A(A/m, V/\Omega)$ đẳng cấu với $\mathrm{Ext}_A^1(A/m, \Omega)$, nên có chiều 1. Vì $V/\Omega$ là một môđun xoắn, các iđêan nguyên tố liên kết của nó là cực đại; điều đó chứng minh mệnh đề (§ 8, No. 4).

Cho M là một A-môđun; phù hợp với *loc. cit.*, ta sẽ ký hiệu bởi D(M) $A$-môđun $\mathrm{Hom}_A(M, V/\Omega)$. Có thể áp dụng các xây dựng của No. 5 bằng cách lấy cho I phức

$$
\cdots 0 \to V \xrightarrow{p} V/\Omega \to 0 \cdots
$$

trong đó V được đặt ở bậc 0, và p ký hiệu toàn cấu chính tắc. Phức $\mathbf{D}(M)$ là

$$
\cdots 0 \to \mathrm{Hom}_A(M, V) \xrightarrow{p_M} \mathbf{D}(M) \to 0 \cdots ,
$$

với $p_M = \mathrm{Hom}(1_M, p)$. Ta có một đẳng cấu chính tắc của các A-môđun phân bậc $\varphi(M, I) : \mathrm{H}(\mathbf{D}(M)) \to \mathrm{Ext}_A(M, \Omega)$ (A, X, p. 100, định lý 1).

Khi M là một môđun xoắn, môđun $\mathbf{D}(M)^0 = \mathrm{Hom}_A(M, V)$ bằng không, và $\varphi(M, I)$ là một đẳng cấu của $\mathbf{D}(M)$ lên $\mathrm{Ext}_A^1(M, \Omega)$; cấu xạ $\alpha_M : M \to \mathbf{D}(\mathbf{D}(M))$ không gì khác hơn là đồng cấu chính tắc của các A-môđun

$$
\alpha_M : M \to \mathbf{D}(\mathbf{D}(M))
$$

được định nghĩa trong § 8, No. 3, là một đẳng cấu khi M thuộc kiểu hữu hạn (nghĩa là, có độ dài hữu hạn). Trong trường hợp này ta thu lại tình huống của *loc. cit*.

Hãy trở lại trường hợp tổng quát, và giả sử A-môđun M thuộc kiểu hữu hạn. Khi đó $\mathbf{D}(M)$ là một môđun xoắn, nên A-môđun $\mathbf{D}(\mathbf{D}(M))^{-1} = \mathrm{Hom}_A(\mathbf{D}(M), V)$ bằng không. Mặt khác A-môđun $\mathrm{Hom}_A(\mathbf{D}(M)^0, V) = \mathrm{Hom}_A(\mathrm{Hom}_A(M, V), V)$ được đồng nhất một cách tự nhiên với $K \otimes_A M$, sao cho đồng cấu

$$
\mathrm{Hom}(1, p) : \mathrm{Hom}_A(\mathrm{Hom}_A(M, V), V) \to \mathbf{D}(\mathrm{Hom}_A(M, V))
$$

được đồng nhất với ánh xạ

$$
j : K \otimes_A M \to \mathbf{D}(\mathrm{Hom}_A(M, V))
$$

sao cho $j(\lambda \otimes m)(f) = p(\lambda f(m))$ với $\lambda \in K,\ m \in M,\ f \in \mathrm{Hom}_A(M, V)$. Do đó định lý 1 của No. 5 được chuyển thành tính khớp của dãy

$$
0 \longrightarrow M \xrightarrow{(i, \alpha_M)} (K \otimes_A M) \oplus D(D(M)) \xrightarrow{(j, -D(p_M))} D(\mathrm{Hom}_A(M, V)) \longrightarrow 0,
$$

trong đó $i$ ký hiệu ánh xạ chính tắc từ $M$ vào $K \otimes_A M$. Hạt nhân của $i$ đồng nhất với môđun con xoắn $T(M)$ của $M$, và đối hạt nhân của nó đồng nhất với $(K/A) \otimes_A M$. Xét biểu đồ giao hoán với các hàng khớp

$$
\begin{array}{ccccccccc}
0 & \to & T(M) & \longrightarrow & M & \xrightarrow{i} & K \otimes_A M & \longrightarrow & (K/A) \otimes_A M \longrightarrow 0 \\
& & \downarrow{\alpha_M} & & & & \downarrow{j} & & \\
0 & \to & D(\mathrm{Ext}_A^1(M, \Omega)) & \longrightarrow & D(D(M)) & \xrightarrow{D(p_M)} & D(\mathrm{Hom}_A(M, V)) & \longrightarrow & D(\mathrm{Hom}_A(M, \Omega)) \longrightarrow 0
\end{array}
$$

trong đó hàng thứ hai thu được bằng đối ngẫu Matlis từ dãy khớp

$$
0 \to \mathrm{Hom}_A(M, \Omega) \longrightarrow \mathrm{Hom}_A(M, V) \xrightarrow{p_M} \mathrm{Hom}_A(M, V/\Omega) \longrightarrow \mathrm{Ext}_A^1(M, \Omega) \to 0.
$$

Khi đó Định lý 1 có nghĩa là các đồng cấu của các $A$-môđun

$$
\gamma^0(M) : T(M) \longrightarrow D(\mathrm{Ext}_A^1(M, \Omega)) \quad \text{và} \quad \gamma^1(M) : (K/A) \otimes_A M \longrightarrow D(\mathrm{Hom}_A(M, \Omega))
$$

suy ra tương ứng từ $\alpha_M$ và $j$ đều là song ánh. Vì $A$-môđun $T(M)$ có độ dài hữu hạn, nên $A$-môđun $\mathrm{Ext}_A^1(M, \Omega)$ có độ dài hữu hạn và đồng nhất với đối ngẫu Matlis của $D(T(M))$, và ta có $[\mathrm{Ext}_A^1(M, \Omega)] = [T(M)]$ trong nhóm $Z_0(A)$ và $\mathrm{long}_A(\mathrm{Ext}_A^1(M, \Omega)) = \mathrm{long}_A(T(M))$ (§ 8, No. 4, Mệnh đề 4). Mặt khác, khi lấy $M = A$, ta thu được một đẳng cấu chính tắc $\gamma^1(A) : K/A \to D(\Omega)$.

Cho $B$ là một vành con của $K$ chứa $A$, hữu hạn trên $A$. Với mọi iđêan cực đại $m$ của $A$, ta có $\mathrm{prof}_{A_m}(B_m) = \dim_{A_m}(B_m) = 1$ (§ 1, No. 1, Nhận xét 2 và VIII, § 2, No. 3, Định lý 1), nên $B$ là một A-môđun Macaulay. Do đó B-môđun $\Omega_B = \mathrm{Hom}_A(B, \Omega)$ là đối ngẫu hóa (No. 3, Nhận xét). Ánh xạ chính tắc từ $\Omega_B = \mathrm{Hom}_A(B, \Omega)$ vào $\Omega = \mathrm{Hom}_A(A, \Omega)$ là đơn ánh; ảnh của nó gồm các phần tử $\omega$ của $\Omega$ sao cho B-môđun con $B\omega$ của $V$ được chứa trong $\Omega$. Vì thế $\Omega_B$ đồng nhất với B-môđun con lớn nhất của $\Omega$. A-môđun $B/A$ có độ dài hữu hạn; dãy khớp

$$
0 \to \Omega_B \to \Omega \to \mathrm{Ext}_A^1(B/A, \Omega) \to 0
$$

cho phép đồng nhất $\Omega/\Omega_B$ với $\mathrm{Ext}_A^1(B/A, \Omega)$, do đó theo điều nói trên với $D(B/A)$. Đặc biệt, ta có $[B/A] = [\Omega/\Omega_B]$ trong $Z_0(A)$ và $\mathrm{Ann}_A(B/A) = \mathrm{Ann}_A(\Omega/\Omega_B)$ (§ 8, No. 4, mệnh đề 4).

Iđêan $c = \mathrm{Ann}_A(B/A)$ là transporter $A : B$, nghĩa là (VII, § 1, No. 1) tập hợp các phần tử $x$ của $K$ sao cho $xB \subset A$. Nó là một iđêan (khác không) của

của A và của B; thực ra nó là iđêan lớn nhất của B được chứa trong A. Vì $\Omega_B : \Omega \subset \Omega : \Omega = A$ (No. 4, mệnh đề 7, b)), nên ta có $\operatorname{Ann}_A(\Omega/\Omega_B) = \Omega_B : \Omega$, do đó cuối cùng
$$
c = \operatorname{Ann}_A(B/A) = \operatorname{Ann}_A(\Omega/\Omega_B) = \Omega_B : \Omega .
$$
Vì $\Omega_B$ là một B-môđun, quan hệ $x \Omega \subset \Omega_B$ tương đương với $xB\Omega \subset \Omega_B$, nên ta cũng có $c = \Omega_B : B\Omega$.

Ta sẽ chuyên biệt hóa phần bàn luận trước vào trường hợp B là bao đóng nguyên của A; giả thiết B là một A-môđun hữu hạn sinh được thỏa mãn khi vành A là vành Nhật (IX, § 4, No. 1, định nghĩa 1), điều này xảy ra khi nó địa phương và đầy đủ (*loc. cit.*, No. 2, định lý 2), hoặc khi nó về bản chất là kiểu hữu hạn trên một trường (*loc. cit.*, No. 1, nhận xét 2 và ví dụ). Khi đó vành B là một vành Dedekind (VII, § 2, No. 2, định lý 1), và các B-môđun không xoắn $\Omega_B$, $B\Omega$ và $c$ đều xạ ảnh hạng 1 (VII, § 4, No. 10, mệnh đề 22). Khi đó quan hệ $c = \Omega_B : B\Omega$ có nghĩa là ánh xạ tuyến tính $c \otimes_B B\Omega \to \Omega_B$ suy ra từ tác động của K trên V là một đẳng cấu (II, § 5, No. 6, mệnh đề 11). Đặc biệt ta có $\Omega_B = c(B\Omega) = c\Omega$.

#### Mệnh đề 9 {#ac-x-s9-prop-9 .statement}

*Cho B là bao đóng nguyên của A, và $c = A : B$. Giả sử B là một A-môđun hữu hạn sinh. Ta có bất đẳng thức $[B/c] \leq 2[B/A]$ trong $Z_0(A)$. Để có đẳng thức, điều kiện cần và đủ là A là một vành Gorenstein.*

Ta có $[B/c] = [B/A] + [A/c]$, nên bất đẳng thức đang xét tương đương với $[A/c] \leq [B/A]$.

A) Với mọi iđêan cực đại $m$ của A, bao đóng nguyên của $A_m$ là $B_m$ (V, § 1, No. 5, hệ quả 1), và ta có $c_m = A_m : B_m$. Hơn nữa, theo định nghĩa, ta có $[B/c] = \sum_m \operatorname{long}_{A_m}(B_m/c_m)[m]$ và $[B/A] = \sum_m \operatorname{long}_{A_m}(B_m/A_m)[m]$. Điều này đưa ta về việc chứng minh mệnh đề khi vành A là *địa phương*, và từ nay ta sẽ giả sử như vậy. Trong trường hợp này, nhóm có thứ tự $Z_0(A)$ được đồng nhất một cách chính tắc với $\mathbf{Z}$, sao cho lớp của một môđun có độ dài hữu hạn là độ dài của nó. Vành B là nửa địa phương và B-môđun $B\Omega$ là tự do hạng 1 (II, § 5, No. 3, mệnh đề 5).

B) Nếu A là một vành Gorenstein, A-môđun $\Omega$ là tự do hạng 1 (No. 4, hệ quả 1 của mệnh đề 7); hãy chọn một phần tử sinh $\omega$ của $\Omega$. Ta có $\Omega = A\omega$ và $\Omega_B = c\Omega = c\omega$, và do đó $\operatorname{long}(A/c) = \operatorname{long}(\Omega/\Omega_B) = \operatorname{long}(B/A)$.

C) Giả sử trường thặng dư $\kappa_A$ là vô hạn. Với mọi iđêan cực đại $n$ của B, ký hiệu $L(n)$ là không gian vectơ trên $B/n$ (có chiều 1) $B\Omega/nB\Omega$, và $\operatorname{pr}_n$ là phép chiếu chính tắc của $\bigoplus_n L(n)$ lên $L(n)$. Cho $\varphi : \Omega \longrightarrow \bigoplus_n L(n)$ là hạn chế lên $\Omega$ của đồng cấu chính tắc $B\Omega \longrightarrow \bigoplus_n L(n)$. Ảnh của $\varphi$ là một không gian con vectơ trên $\kappa_A$ của $\bigoplus_n L(n)$; nó không được chứa trong $\operatorname{Ker} \operatorname{pr}_n$, vì nếu không thì ta sẽ có $\Omega \subset nB\Omega$ và do đó $B\Omega \subset nB\Omega$, điều này mâu thuẫn. Vậy ảnh của $\varphi$ không được chứa trong hợp của các $\operatorname{Ker} \operatorname{pr}_n$ (A, V, p. 40, bổ đề 1); do đó tồn tại một phần tử $\omega$ của $\Omega$ mà ảnh của nó trong $B\Omega/nB\Omega$ là khác không với mọi $n$, điều này suy ra rằng $\omega$ sinh B-môđun $B\Omega$ (II, § 3, No. 3, mệnh đề 11).

Cho $a \in A$; nếu $a\omega$ thuộc $\Omega_B$, ta có $aB\omega \subset \Omega_B$, do đó $a\Omega \subset \Omega_B$, suy ra $a \in c$. Vì thế ánh xạ $a \mapsto a\omega$ cảm sinh một đơn ánh từ $A/c$ vào $\Omega/\Omega_B$; do đó ta có $\operatorname{long}(A/c) \leq \operatorname{long}(\Omega/\Omega_B) = \operatorname{long}(B/A)$.

Nếu $\operatorname{long}(A/c) = \operatorname{long}(B/A)$, ta có $A\omega + \Omega_B = \Omega$. Có thể giả sử iđêan $c$ được chứa trong $m_A$ (nếu không thì $A$ bằng $B$, do đó là một vành Gorenstein). Vì $\Omega_B = c\Omega$ được chứa trong $m_A\Omega$, theo bổ đề Nakayama suy ra $\omega$ sinh ra $\Omega$. Vậy $A$-môđun $\Omega$ là đơn sinh, do đó tự do hạng 1, nghĩa là $A$ là một vành Gorenstein (No. 4, hệ quả 1 của mệnh đề 7).

D) Xét trường hợp tổng quát. Kí hiệu bởi $A'$ vành $A[X]$, nghĩa là (IX, App., No. 2) vành địa phương của vành đa thức $A[X]$ tại iđêan nguyên tố $m_A A[X]$; đó là một $A$-đại số phẳng, nguyên, chiều 1, mà trường thặng dư $\kappa_{A'}$ được đồng nhất với $\kappa_A(X)$ và trường phân thức được đồng nhất với $K(X)$ (*nơi đã dẫn*). Theo hệ quả của mệnh đề 5 ở No. 3, $A'$-môđun $A' \otimes_A \Omega$ là đối ngẫu hóa. Đặt $B' = A' \otimes_A B$; đó là bao đóng nguyên của $A'$ trong $K(X)$ (V, § 1, No. 3, mệnh đề 13 và No. 5, mệnh đề 16). Phần tử dẫn $c' = A' : B'$ bằng $cA'$ (I, § 2, No. 10, công thức (11)). Với mọi $A$-môđun $M$ có độ dài hữu hạn, ta có $\operatorname{long}_{A'}(A' \otimes_A M) = \operatorname{long}_A(M)$: thật vậy, vì $A$-đại số $A'$ là phẳng, chỉ cần chứng minh quan hệ này khi $M$ là đơn, nghĩa là đẳng cấu với $\kappa_A$; nhưng trong trường hợp này $A' \otimes_A \kappa_A$ được đồng nhất với $\kappa_{A'}$, do đó có mệnh đề của ta. Vậy ta có

$$
\operatorname{long}_A(B/c) = \operatorname{long}_{A'}(B'/c') \quad \text{và} \quad \operatorname{long}_A(B/A) = \operatorname{long}_{A'}(B'/A') .
$$

Vành $A'$ thỏa mãn các giả thiết của mệnh đề, và trường thặng dư của nó là vô hạn. Theo phần C) của chứng minh, ta có $\operatorname{long}_{A'}(B'/c') \leq 2 \operatorname{long}_{A'}(B'/A')$, và đẳng thức kéo theo $A'$ là một vành Gorenstein; nhưng điều kiện sau cùng này kéo theo $A$ là một vành Gorenstein (§ 3, No. 8, hệ quả 1 của mệnh đề 12).

## BÀI TẬP {#ac-x-s9-exercises}

Xem [các bài tập của § 9](exercises/s9/).
