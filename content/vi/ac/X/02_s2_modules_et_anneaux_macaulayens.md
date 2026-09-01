---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 2
section_title: Modules et anneaux macaulayens
lang: vi
source: ac-x-fr
book_pages: AC X.154-AC X.157
pdf_pages: 0022-0035, 0153-0156
extraction: ocr
subsections:
    - "no": 1
      title: Modules macaulayens
      page: 0
      pdf_page: 22
    - "no": 2
      title: Support d’un module macaulayen
      page: 24
      pdf_page: 23
    - "no": 3
      title: Modules macaulayens sur un anneau local
      page: 26
      pdf_page: 25
    - "no": 4
      title: Parties fortement sécantes et quotients d’un module macaulayen
      page: 28
      pdf_page: 27
    - "no": 5
      title: Anneaux de Macaulay
      page: 30
      pdf_page: 29
    - "no": 6
      title: Modules macaulayens et algèbres finies
      page: 32
      pdf_page: 31
    - "no": 7
      title: Modules macaulayens et algèbres plates
      page: 0
      pdf_page: 33
statements: 46
exercises: 11
content_sha256: bdc20edf9e402c880fb0d3c2e80e2f04211e358fa7d05a348287bc73a3f718f0
translated_from: content/en-mt/ac/X/02_s2_modules_et_anneaux_macaulayens.md
source_lang: en-mt
translation_method: machine
source_content_sha256: a8db826b7ca09881d463dde0cdd85fdb21ded4664105d9fcd21f4d357498696b
translation_model: gpt-5.4
translation_run: translate-vi-cef242cf
glossary_version: 34
glossary_terms_sha256: 7f438f5cc8acdfbfb22fe4a4a27462e88c8bff657d34e441fc5e455e31c2cbe9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 2. MÔĐUN VÀ VÀNH MACAULAY

### 1. Môđun Macaulay

Cho $A$ là một vành Noether, $M$ là một $A$-môđun sinh hữu hạn và $p$ là một iđêan nguyên tố của $A$. Nếu $p \not\in \mathrm{Supp}(M)$, ta có $M_p = 0$, do đó $\mathrm{prof}_{A_p}(M_p) = +\infty$ và $\dim_{A_p}(M_p) = -\infty$. Nếu $p \in \mathrm{Supp}(M)$, ta có $0 \leq \mathrm{prof}_{A_p}(M_p) \leq \dim_{A_p}(M_p) < +\infty$ ($§ 1$, No. 4, Hệ quả 2 của Định lý 2).

#### Định nghĩa 1 {#ac-x-s2-def-1 .statement}

*Cho $A$ là một vành Noether và $M$ là một $A$-môđun sinh hữu hạn. Ta nói rằng $M$ là Macaulay hoặc là một môđun Macaulay nếu, với mọi iđêan cực đại $m \in \mathrm{Supp}(M)$, ta có $\mathrm{prof}_{A_m}(M_m) = \dim_{A_m}(M_m)$.*

Từ điều trên, điều đó tương đương với việc nói rằng ta có $\mathrm{prof}_{A_m}(M_m) \geq \dim_{A_m}(M_m)$ với mọi iđêan cực đại $m$ của $A$. Cho $A$ là một vành địa phương Noether; để một $A$-môđun sinh hữu hạn khác không là Macaulay, điều kiện cần và đủ là độ sâu của nó bằng chiều của nó.

#### Ví dụ 1 {#ac-x-s2-n1-exa-1 .statement}

Mọi $A$-môđun có độ dài hữu hạn đều là Macaulay.

#### Ví dụ 2 {#ac-x-s2-n1-exa-2 .statement}

Cho $M'$ là một môđun con hạng tử trực tiếp của một $A$-môđun Macaulay sinh hữu hạn $M$. Khi đó $M'$ là Macaulay; thật vậy, với mọi iđêan cực đại $m$ của $A$, $A_m$-môđun $M'_m$ là một nhân tử trực tiếp của $M_m$ và do đó ta có
$$
\mathrm{prof}_{A_m}(M'_m) \geq \mathrm{prof}_{A_m}(M_m) \geq \dim_{A_m}(M_m) \geq \dim_{A_m}(M'_m),
$$
theo Nhận xét 4 của $§ 1$, No. 1 và VIII, $§ 1$, No. 4, Mệnh đề 9 c).

#### Ví dụ 3 {#ac-x-s2-n1-exa-3 .statement}

Cho $M$ là một $A$-môđun Macaulay sinh hữu hạn và $(x_1, \ldots, x_n)$ là một dãy $M$-chính quy gồm các phần tử của $A$. Khi đó $A$-môđun $\overline{M} = M/(x_1M + \cdots + x_nM)$ là Macaulay. Thật vậy, cho $m$ là một iđêan cực đại của $A$ thuộc $\mathrm{Supp}(\overline{M})$; ta có $x_i \in m$ với mọi $i$ vì $x_i$ linh hóa $\overline{M}$, và các ảnh chính tắc của các $x_i$ trong $A_m$ tạo thành một dãy $M_m$-chính quy gồm các phần tử của $mA_m$. Do đó ta có ($§ 1$, No. 4, Mệnh đề 7 và VIII, $§ 3$, No. 2, Hệ quả của Mệnh đề 3) các đẳng thức
$$
\mathrm{prof}_{A_m}(\overline{M}_m) = \mathrm{prof}_{A_m}(M_m) - n,
$$
$$
\dim_{A_m}(\overline{M}_m) = \dim_{A_m}(M_m) - n,
$$
do đó có mệnh đề của chúng ta.

#### Ví dụ 4 {#ac-x-s2-n1-exa-4 .statement}

Cho $M$ là một $A$-môđun sinh hữu hạn, và cho $a$ là một iđêan của $A$ sao cho $aM = 0$. Để $A$-môđun $M$ là Macaulay, điều kiện cần và đủ là nó là Macaulay như một $(A/a)$-môđun. Thật vậy, đặt $B = A/a$; cho $n$ là một iđêan cực đại của $B$ và $m$ là ảnh ngược của nó trong $A$; khi đó $\dim_{A_m}(M_m) = \dim_{B_n}(M_n)$ và $\mathrm{prof}_{A_m}(M_m) = \mathrm{prof}_{B_n}(M_n)$ ($§ 1$, No. 3, hệ quả của mệnh đề 4).

#### Mệnh đề 1 {#ac-x-s2-prop-1 .statement}

Cho $\Lambda$ là một vành Noether, $M$ một $\Lambda$-môđun sinh hữu hạn, và $p$ và $q$ là các iđêan nguyên tố của $\mathrm{Supp}(M)$ sao cho $p \subset q$. Giả sử rằng $\dim_{\Lambda_q}(M_q) = \mathrm{prof}_{\Lambda_q}(M_q)$. Khi đó ta có $\dim_{\Lambda_p}(M_p) = \mathrm{prof}_{\Lambda_p}(M_p)$ và
$$
\dim_{\Lambda_q}(M_q) = \dim_{\Lambda_p}(M_p) + \dim(\Lambda_q/\mathfrak{p}\Lambda_q) .
$$
Điều này suy ra trực tiếp từ hệ quả 1 của mệnh đề 13 của § 1, No. 7.

#### Hệ quả {#ac-x-s2-n1-cor-1 .statement}

Cho $\Lambda$ là một vành Noether và $M$ một $\Lambda$-môđun sinh hữu hạn. Các điều kiện sau là tương đương:
(i) $\Lambda$-môđun $M$ là Macaulay;
(ii) ta có $\mathrm{prof}_{\Lambda_p}(M_p) = \dim_{\Lambda_p}(M_p)$ với mọi $p \in \mathrm{Supp}(M)$;
(iii) ta có $\mathrm{prof}_F(M) = \mathrm{codim}(\mathrm{Supp}(M) \cap F', \mathrm{Supp}(M))$ với mọi tập con đóng $F$ của $\mathrm{Spec}(\Lambda)$;
(iv) ta có $\mathrm{prof}_A(p; M) = \dim_{\Lambda_p}(M_p)$ với mọi $p \in \mathrm{Supp}(M)$.

(i) $\Rightarrow$ (ii): điều này suy ra từ Mệnh đề 1.
(ii) $\Rightarrow$ (iii): theo mệnh đề 8 của § 1, No. 5, $\mathrm{prof}_F(M)$ là cận dưới lớn nhất của các số nguyên $\mathrm{prof}(M_p)$ khi $p$ chạy qua $\mathrm{Supp}(M) \cap F$. Nếu $M$ là Macaulay, thì đối với một iđêan như thế $p$ ta có các đẳng thức $\mathrm{prof}(M_p) = \dim(M_p) = \mathrm{codim}(V(p), \mathrm{Supp}(M))$ (VIII, § 1, No. 4, mệnh đề 9), do đó có (iii).
(iii) $\Rightarrow$ (iv): chỉ cần lấy $F = V(p)$.
(iv) $\Rightarrow$ (i): điều này suy ra từ các bất đẳng thức $\mathrm{prof}_A(p; M) \leq \mathrm{prof}(M_p) \leq \dim(M_p)$, đúng với mọi $p \in \mathrm{Supp}(M)$ ($§ 1$, No. 5, nhận xét 3 và No. 4, hệ quả 2 của định lý 2).

#### Nhận xét {#ac-x-s2-n1-rem-1 .statement}

Cho $S$ là một tập con nhân của $\Lambda$ và $M$ là một Macaulay $\Lambda$-môđun sinh hữu hạn. Khi đó $S^{-1}M$ là một Macaulay $S^{-1}\Lambda$-môđun. Thật vậy, cho $q \in \mathrm{Spec}(S^{-1}\Lambda)$; ký hiệu $i_A^S : \Lambda \to S^{-1}\Lambda$ là đồng cấu chính tắc và đặt $p = (i_A^S)^{-1}(q)$. Vành $(S^{-1}\Lambda)_q$ được đồng nhất với $A_p$ (II, § 2, No. 5, mệnh đề 11), và $A_p$-môđun $(S^{-1}M)_q$ được đồng nhất với $A_p$-môđun $M_p$ (II, § 2, No. 7, mệnh đề 20), môđun này là Macaulay theo hệ quả.

### 2. Giá của một môđun Macaulay

#### Mệnh đề 2 {#ac-x-s2-prop-2 .statement}

Cho $\Lambda$ là một vành Noether và $M$ là một Macaulay $\Lambda$-môđun sinh hữu hạn.
a) $\Lambda$-môđun $M$ không có iđêan nguyên tố liên kết nhúng nào.\footnote{Nhắc lại (xem IV, § 2, No. 3, nhận xét) rằng một iđêan nguyên tố liên kết của $M$ được gọi là nhúng nếu nó không phải là một phần tử cực tiểu của $\mathrm{Supp}(M)$. Do đó nói rằng $M$ không có iđêan nguyên tố liên kết nhúng nghĩa là các iđêan nguyên tố liên kết của $M$ là các phần tử cực tiểu của $\mathrm{Supp}(M)$.}
b) Cho $X$ là một tập con đóng bất khả quy của $\mathrm{Supp}(M)$ và $Y$ là một tập con đóng của $X$. Khi đó
$$
\mathrm{codim}(Y, X) + \mathrm{codim}(X, \mathrm{Supp}(M)) = \mathrm{codim}(Y, \mathrm{Supp}(M)) .
$$
c) Không gian tôpô $\mathrm{Supp}(M)$ là catenary (VIII, § 1, No. 2, định nghĩa 4).

d) Cho $X_1$ và $X_2$ là các thành phần bất khả quy của $\mathrm{Supp}(M)$ và $Y$ là một tập con đóng của $X_1 \cap X_2$. Khi đó $\mathrm{codim}(Y, X_1) = \mathrm{codim}(Y, X_2)$.

a) Cho $\mathfrak{p} \in \mathrm{Ass}(M)$. Khi đó $\mathrm{prof}_A(\mathfrak{p}; M) = 0$ (§ 1, No. 1, nhận xét 2), do đó $\dim(M_{\mathfrak{p}}) = 0$ (No. 1, hệ quả của mệnh đề 1), điều này kéo theo rằng $\mathfrak{p}$ là một phần tử cực tiểu của $\mathrm{Supp}(M)$.

b) Trước hết giả sử rằng $Y$ là bất khả quy. Cho $\mathfrak{p}$ và $\mathfrak{q}$ là các iđêan nguyên tố của $\mathrm{Supp}(M)$ sao cho ta có $Y = V(\mathfrak{q})$ và $X = V(\mathfrak{p})$. Từ mệnh đề 1 suy ra rằng ta có

$$
\begin{align*}
\mathrm{codim}(Y, X) &= \dim(A_{\mathfrak{q}}/\mathfrak{p}A_{\mathfrak{q}}) = \dim(M_{\mathfrak{q}}) - \dim(M_{\mathfrak{p}}) \\
&= \mathrm{codim}(Y, \mathrm{Supp}(M)) - \mathrm{codim}(X, \mathrm{Supp}(M)) .
\end{align*}
$$

Trường hợp tổng quát suy ra từ VIII, $\S$ 1, No. 2, nhận xét 3.

c) Cho $X$, $Y$, $Z$ là các tập con đóng bất khả quy của $\mathrm{Supp}(M)$ sao cho $Z \subset Y \subset X$. Đối chiều của mỗi tập con này trong $\mathrm{Supp}(M)$ là hữu hạn (VIII, $\S$ 1, No. 4, mệnh đề 9 và $\S$ 3, No. 1, hệ quả 1 của mệnh đề 2). Khi đó từ b) suy ra đẳng thức

$$
\mathrm{codim}(Z, Y) + \mathrm{codim}(Y, X) = \mathrm{codim}(Z, X)
$$

điều này suy ra c) (VIII, $\S$ 1, No. 2, mệnh đề 4).

d) Theo b), ta có $\mathrm{codim}(Y, X_1) = \mathrm{codim}(Y, \mathrm{Supp}(M)) = \mathrm{codim}(Y, X_2)$.

Đặc biệt, nếu tồn tại một A-môđun Macaulay sinh hữu hạn $M$, có giá bằng $\mathrm{Spec}(A)$, thì vành $A$ là catenary và do đó mọi vành phân thức hoặc mọi vành thương của $A$ đều là catenary (VIII, $\S$ 1, No. 3, nhận xét 2).

#### Nhận xét 1 {#ac-x-s2-n2-rem-1 .statement}

Dưới các giả thiết của Mệnh đề 2, có thể xảy ra trường hợp hai thành phần bất khả quy $X_1$ và $X_2$ của $\mathrm{Supp}(M)$ có giao $Y$ rút về một điểm và ta có $\dim X_1 \neq \dim X_2$ và $\dim X_2 \neq \mathrm{codim}(Y, X_2)$ (xem bài tập 4). Tuy nhiên, điều này không thể xảy ra khi vành $A$ là địa phương, như hệ quả sau đây chỉ ra.

#### Hệ quả {#ac-x-s2-n2-cor-1 .statement}

Cho $A$ là một vành địa phương Noether và $M$ là một A-môđun Macaulay sinh hữu hạn khác không.

a) Mọi chuỗi tối đại các tập con đóng bất khả quy của $\mathrm{Supp}(M)$ đều có độ dài bằng $\dim(M)$.

b) Với mọi tập con đóng $X$ của $\mathrm{Supp}(M)$, ta có

$$
\mathrm{codim}(X, \mathrm{Supp}(M)) = \dim(\mathrm{Supp}(M)) - \dim(X) .
$$

c) Mọi thành phần bất khả quy của $\mathrm{Supp}(M)$ đều có cùng chiều.

d) Với mọi iđêan $J$ của $A$, ta có

$$
\mathrm{prof}_A(J; M) = \dim(M) - \dim(M/JM) .
$$

a) Một chuỗi tối đại các tập con đóng bất khả quy của $\mathrm{Supp}(M)$ có phần tử nhỏ nhất là $\{m_A\}$ và phần tử lớn nhất là một thành phần bất khả quy $X$ của

Supp(M). Độ dài của nó bằng đối chiều của $\{ m_A \}$ trong X (Mệnh đề 2, c)); theo Mệnh đề 2, b) áp dụng cho các tập con đóng $\{ m_A \} \subset X$, điều này bằng $\operatorname{codim}(\{ m_A \}, \operatorname{Supp}(M))$, tức là bằng $\dim(M)$.

b) Đây là một hệ quả của a) khi tập con X là bất khả quy (VIII, § 1, No. 2, mệnh đề 5); trường hợp tổng quát suy ra từ VIII, § 1, No. 1, mệnh đề 1 và § 1, No. 2, nhận xét 4.

c) Đây là một hệ quả của b).

d) Ta có $\operatorname{prof}_A(J; M) = \operatorname{codim}(\operatorname{Supp}(M) \cap V(J), \operatorname{Supp}(M))$ theo hệ quả của Mệnh đề 1 của No. 1. Khi đó chỉ cần áp dụng b) với $X = \operatorname{Supp}(M) \cap V(J) = \operatorname{Supp}(M/JM)$ (II, § 4, No. 4, hệ quả của Mệnh đề 18).

#### Nhận xét 2 {#ac-x-s2-n2-rem-2 .statement}

Cho M là một A-môđun Macaulay sinh hữu hạn, và $p$ là một phần tử của $\operatorname{Supp}(M)$. Theo Định lý 2 của § 1, No. 4, ta có $\operatorname{prof}_A(p; M) < +\infty$, và tồn tại một dãy M-chính quy có độ dài $\operatorname{prof}_A(p; M)$ gồm các phần tử của $p$. Gọi J là iđêan của A sinh bởi một dãy như vậy; khi đó A-môđun $M/JM$ là Macaulay (No. 1, ví dụ 3) và $p$ là một phần tử cực tiểu của giá của nó. Thật vậy, $p$ chứa J và do đó thuộc giá của $M/JM$ (II, § 4, No. 4, hệ quả của Mệnh đề 18); theo Hệ quả 1 của Định lý 2 trong § 1, No. 4, iđêan $p$ được chứa trong một phần tử của $\operatorname{Ass}(M/JM)$, nhưng mọi iđêan nguyên tố liên kết với một môđun Macaulay sinh hữu hạn đều là một phần tử cực tiểu của giá của nó (Mệnh đề 2).

### 3. Môđun Macaulay trên một vành địa phương

#### Mệnh đề 3 {#ac-x-s2-prop-3 .statement}

Cho A là một vành địa phương Noether, M là một A-môđun sinh hữu hạn khác không, và d là chiều của M. Các điều kiện sau là tương đương:

(i) A-môđun M là Macaulay;
(ii) ta có $\operatorname{prof}(M) = d$;
(iii) ta có $\operatorname{Ext}_A^i(\kappa_A, M) = 0$ với mọi số nguyên $i < d$;
(iv) ta có $\operatorname{Ext}_A^i(N, M) = 0$ với mọi A-môđun N có độ dài hữu hạn và mọi số nguyên $i < d$;
(v) ta có $\operatorname{Ext}_A^i(N, M) = 0$ với mọi A-môđun sinh hữu hạn N và mọi số nguyên $i < d - \dim(M \otimes_A N)$;
(vi) tồn tại một dãy M-chính quy gồm các phần tử của $m_A$ có độ dài d.

Điều kiện (i) tương đương với đẳng thức $\operatorname{prof}(M) = d$, tức là với điều kiện (ii), hay cũng tương đương với bất đẳng thức $\operatorname{prof}(M) \geq d$, tức là với (iii) và với (vi) (§ 1, No. 4, Định lý 2). Các hệ kéo theo (v) $\Rightarrow$ (iv) và (iv) $\Rightarrow$ (iii) là hiển nhiên.

Sau hết, giả sử $M$ là Macaulay và $N$ là một A-môđun hữu hạn sinh. Đặt $F = \operatorname{Supp}(N)$; theo II, § 4, No. 4, Prop. 18, ta có $\operatorname{Supp}(M) \cap F = \operatorname{Supp}(M \otimes_A N)$, sao cho

$$
\operatorname{prof}_F(M) = \operatorname{codim}(\operatorname{Supp}(M) \cap F, \operatorname{Supp}(M)) = \dim M - \dim(M \otimes_A N)
$$

(No. 1, hệ quả của Prop. 1 và No. 2, hệ quả của Prop. 2). Khi đó suy ra kéo theo (i) $\Rightarrow$ (v) từ Nhận xét 1 của § 1, No. 5.

Trong phần còn lại của số này, ta sẽ nói rằng một môđun hữu hạn sinh M trên một vành địa phương Noether A là thuần khiết nếu, với mọi iđêan nguyên tố p liên kết với M, ta có dim(A/p) = dim(M). Điều đó cũng có nghĩa là M không có iđêan nguyên tố liên kết nội nhúng nào và các thành phần bất khả quy của giá của M đều có cùng chiều. Mọi môđun Macaulay trên một vành địa phương Noether đều là thuần khiết (No. 2, Prop. 2 và hệ quả của nó).

Bổ đề 1:— Cho A là một vành địa phương Noether, M là một A-môđun hữu hạn sinh và thuần khiết, và x là một phần tử của mA. Các điều kiện sau là tương đương:

(i) ta có dim(M/xM) = dim(M) − 1 ;
(ii) phép vị tự xM là đơn ánh.

Ta có thể giả sử M khác không. Mệnh đề (i) tương đương với việc x không thuộc một phần tử cực tiểu nào p của Supp(M) sao cho dim(A/p) = dim(M) (VIII, § 3, No. 2, Prop. 3), và mệnh đề (ii) tương đương với việc x không thuộc iđêan nguyên tố nào liên kết với M (IV, § 1, No. 1, Cor. 2 to Prop. 2). Vì M là thuần khiết, các iđêan nguyên tố liên kết với nó là các phần tử cực tiểu của Supp(M); do đó (i) và (ii) là tương đương.

Cho A là một vành địa phương Noether và M là một A-môđun hữu hạn sinh khác không. Nhắc lại (VIII, § 3, No. 2) rằng một dãy (x₁, ..., x_r) các phần tử của mA được gọi là cát tuyến đối với M nếu ta có dim(M/(x₁M + ... + x_rM)) = dim(M) − r.

#### Mệnh đề 4 {#ac-x-s2-prop-4 .statement}

Cho A là một vành địa phương Noether, M là một A-môđun hữu hạn sinh khác không, và (x₁, ..., x_r) là một dãy các phần tử của mA cát tuyến đối với M. Các điều kiện sau là tương đương:

(i) A-môđun M là Macaulay ;
(ii) dãy (x₁, ..., x_r) là M-chính quy và A-môđun M/(x₁M + ... + x_rM) là Macaulay.

Giả sử rằng dãy (x₁, ..., x_r) là M-chính quy. Khi đó ta có

$$
\dim(M) = r + \dim(M/(x_1M + ... + x_rM))
$$
$$
\operatorname{prof}(M) = r + \operatorname{prof}(M/(x_1M + ... + x_rM))
$$

(§ 1, No. 4, Prop. 7), do đó có kéo theo (ii) ⇒ (i).

Giả sử A-môđun M là Macaulay, và chứng minh (ii) bằng quy nạp theo r. Mệnh đề là hiển nhiên nếu r = 0. Nếu r ≥ 1, A-môđun N = M/(x₁M + ... + x_{r−1}M) là Macaulay theo giả thiết quy nạp, và ta có dim(N/x_rN) = dim(N) − 1 vì dãy (x₁, ..., x_r) là cát tuyến; bởi vậy phép vị tự (x_r)_N là đơn ánh (Bổ đề 1), và N/x_rN là Macaulay (No. 1, Ví dụ 3), do đó suy ra (ii).

#### Định lý 1 {#ac-x-s2-thm-1 .statement}

Cho A là một vành địa phương Noether, M là một A-môđun hữu hạn sinh khác không, d là chiều của M, x = (x₁, ..., x_d) là một dãy các phần tử của mA cát tuyến đối với M, và J là iđêan do dãy đó sinh. Các điều kiện sau là tương đương:

(i) A-môđun M là Macaulay ;

(ii) dãy $x$ là M-chính quy ;
(iii) dãy $x$ là hoàn toàn cát tuyến đối với $M$ (A, X, p. 157, Def. 2) ;
(iv) bội số (VIII, § 7, No. 1, Def. 1) $e_J(M)$ của $M$ đối với iđêan $J$ bằng độ dài của A-môđun $M/JM$ ;
(v) với mỗi số nguyên $i$ sao cho $1 \leq i \leq d$, A-môđun $M/(x_1M + \ldots + x_{i-1}M)$ là thuần khiết.

Tính tương đương của (ii) và (iii) suy ra từ A, X, p. 160, Cor. 1 to Th. 1. Vì A-môđun $M/JM$ có độ dài hữu hạn (VIII, § 3, No. 2, Th. 1), tính tương đương của (iii) và (iv) suy ra từ VIII, § 4, No. 3, Prop. 4 và No. 4, Th. 3. Còn lại phải chứng minh tính tương đương của (i), (ii), và (v).

(i) $\Rightarrow$ (v) : nếu $M$ là Macaulay, mỗi môđun $M/(x_1M + \ldots + x_{i-1}M)$ đều là Macaulay (Prop. 4), nên thuần khiết.

(v) $\Rightarrow$ (ii) : điều này suy ra từ Bổ đề 1 áp dụng cho mỗi môđun $M/(x_1M + \ldots + x_{i-1}M)$.

(ii) $\Rightarrow$ (i) : điều này suy ra từ Prop. 4, vì $M/JM$ có độ dài hữu hạn, nên là Macaulay.

### 4. Các tập con cát tuyến mạnh và các thương của một môđun Macaulay

Cho $A$ là một vành Noether, $M$ là một A-môđun hữu hạn sinh, và $S$ là một tập con của $A$. Phù hợp với các quy ước của Chương VIII, ta sẽ ký hiệu bởi $SM$ môđun con $\sum_{s \in S} sM$ của $M$, và bởi $\mathcal{G}$ iđêan của $A$ do $S$ sinh.

#### Bổ đề 2 {#ac-x-s2-lem-2 .statement}

Cho $\overline{\mathcal{G}}$ là ảnh của $\mathcal{G}$ trong $A/\mathrm{Ann}(M)$. Ta có
$$
\mathrm{ht}(\overline{\mathcal{G}}) = \mathrm{codim}(\mathrm{Supp}(M/SM), \mathrm{Supp}(M)) .
$$
Hơn nữa, khi $SM \neq M$, ta có
$$
\mathrm{ht}(\overline{\mathcal{G}}) \leq \mathrm{Card}(S) .
$$

Ta ký hiệu bởi $\alpha$ linh hóa tử của $M$. Theo hệ quả của Prop. 18 của II, § 4, No. 4, giá của A-môđun $M/SM$ là $V(\mathcal{G} + \alpha)$. Do đó đối chiều của nó trong $\mathrm{Supp}(M)$ bằng đối chiều của $V(\mathcal{G} + \alpha)$ trong $V(\alpha)$, hay cũng bằng đối chiều của $V((\mathcal{G} + \alpha)/\alpha)$ trong $\mathrm{Spec}(A/\alpha)$, mà đó chính là chiều cao của $\overline{\mathcal{G}}$.

Giả sử $SM \neq M$; bất đẳng thức $\mathrm{ht}(\overline{\mathcal{G}}) \leq \mathrm{Card}(S)$ là hiển nhiên khi $S$ là vô hạn, và suy ra từ Prop. 4 b) của VIII, § 3, No. 3 khi $S$ là hữu hạn.

#### Định nghĩa 2 {#ac-x-s2-def-2 .statement}

Cho $A$ là một vành Noether, $M$ là một A-môđun hữu hạn sinh, và $S$ là một tập con hữu hạn của $A$. Ta nói rằng $S$ là cắt mạnh đối với $M$ nếu có
$$
\mathrm{Card}(S) \leq \mathrm{codim}(\mathrm{Supp}(M/SM), \mathrm{Supp}(M)) .
$$

#### Nhận xét 1 {#ac-x-s2-n4-rem-1 .statement}

Mọi tập con hữu hạn S của A sao cho SM = M đều là cắt mạnh đối với M. Khi SM ≠ M, suy ra từ bổ đề 2 rằng, để S là cắt mạnh đối với M, điều kiện cần và đủ là có Card(S) = codim(Supp(M/SM), Supp(M)), hay cũng vậy ht($\overline{\mathcal{G}}$) = Card(S).

#### Nhận xét 2 {#ac-x-s2-n4-rem-2 .statement}

Nếu vành A là địa phương và môđun M khác không, thì mọi tập con S của $m_A$ cắt mạnh đối với M đều là cắt đối với M. Thật vậy, vì $\Lambda$-môđun M/SM là khác không, ta có

$$
\text{Card}(S) \leq \operatorname{codim}(\operatorname{Supp}(M/SM), \operatorname{Supp}(M)) \leq \dim(M) - \dim(M/SM)
$$

(VIII, § 1, No. 2, Mệnh đề 3 a)), do đó mệnh đề của ta.

#### Mệnh đề 5 {#ac-x-s2-prop-5 .statement}

Cho A là một vành Noether, M là một A-môđun hữu hạn sinh, và S là một tập con hữu hạn của A. Các điều kiện sau là tương đương:

(i) tập con S của A là cắt mạnh đối với M;
(ii) với mọi phần tử $p$ của Supp(M/SM), ánh xạ chính tắc $\Lambda \to A_p$ cảm sinh một song ánh của S lên một tập con của $pA_p$ cắt đối với $M_p$.

(i) $\Rightarrow$ (ii) : Cho $p \in \operatorname{Supp}(M/SM)$ và gọi $S'$ là ảnh của S trong $A_p$. Tập hợp $S'$ được chứa trong iđêan cực đại $pA_p$, và ta có

$$
\dim(M_p/S'M_p) = \operatorname{codim}(V(p), \operatorname{Supp}(M/SM))
$$

(VIII, § 1, No. 4, Mệnh đề 9). Bất đẳng thức Card(S) $\leq \operatorname{codim}(\operatorname{Supp}(M/SM), \operatorname{Supp}(M))$ và Mệnh đề 3 b) của VIII, § 1, No. 2 suy ra các hệ thức

$$
\text{Card}(S) + \dim(M_p/S'M_p) \leq \operatorname{codim}(V(p), \operatorname{Supp}(M)) = \dim(M_p) .
$$

Vì $M_p$ là khác không, mặt khác ta có $\dim(M_p) \leq \text{Card}(S') + \dim(M_p/S'M_p)$ (VIII, § 3, No. 2, công thức (8)). Khi đó điều kiện (ii) suy ra từ bất đẳng thức $\text{Card}(S') \leq \text{Card}(S)$.

(ii) $\Rightarrow$ (i) : Ta có thể giả sử SM $\neq$ M. Nếu điều kiện (ii) được thỏa mãn, thì với mọi iđêan nguyên tố $p$ của Supp(M/SM) ta có

$$
\text{Card}(S) = \text{Card}(S') \leq \dim(M_p) = \operatorname{codim}(V(p), \operatorname{Supp}(M)) ,
$$

điều này suy ra (i) bằng cách chuyển qua cận dưới lớn nhất.

#### Hệ quả {#ac-x-s2-n4-cor-1 .statement}

Cho A là một vành Noether và M là một A-môđun hữu hạn sinh. Mọi dãy M-chính quy đều cắt mạnh đối với M.

Cho x là một dãy M-chính quy, và J là iđêan của A do nó sinh. Với mọi iđêan nguyên tố $p \in \operatorname{Supp}(M/JM)$, ảnh của x trong $A_p$ là một dãy $M_p$-chính quy gồm các phần tử của $pA_p$, vì thế là một dãy cắt đối với $M_p$ (VIII, § 3, No. 2, hệ quả của Mệnh đề 3).

#### Mệnh đề 6 {#ac-x-s2-prop-6 .statement}

Cho A là một vành Noether, M là một Macaulay A-môđun hữu hạn sinh, và S là một tập con hữu hạn của A cắt mạnh đối với M. Khi đó A-môđun M/SM là Macaulay.

Với mọi iđêan cực đại $m \in \mathrm{Supp}(M/SM)$, ảnh của S trong $A_m$ là cắt đối với $M_m$ (Mệnh đề 5). Vì $M_m$ là một $A_m$-môđun Macaulay, $(M/SM)_m$ cũng vậy (Mệnh đề 4), do đó có mệnh đề.

**Định lý 2 (Macaulay-Cohen).**— *Cho A là một vành Noether và M là một A-môđun hữu hạn sinh. Các điều kiện sau là tương đương:*

(i) *A-môđun M là Macaulay;*

(ii) *với mọi iđêan J của A do một dãy M-chính quy gồm các phần tử của A sinh ra, A-môđun M/JM không có iđêan nguyên tố liên kết nhúng;*

(iii) *với mọi tập con hữu hạn S của A cắt mạnh đối với M, A-môđun M/SM không có iđêan nguyên tố liên kết nhúng.*

(i) $\Rightarrow$ (iii) : Cho S là một tập con hữu hạn của A cắt mạnh đối với M. A-môđun M/SM là Macaulay (Mệnh đề 6) và đặc biệt không có iđêan nguyên tố liên kết nhúng (No. 2, Mệnh đề 2, a)).

(iii) $\Rightarrow$ (ii) : Điều này suy ra từ hệ quả của Mệnh đề 5.

(ii) $\Rightarrow$ (i): Cho $p \in \mathrm{Supp}(M)$; ta sẽ chứng minh rằng $A_p$-môđun $M_p$ là Macaulay. Ta lập luận bằng quy nạp theo số nguyên $\dim(M_p)$. Nếu $\dim(M_p)$ bằng zero, thì $M_p$ là một $A_p$-môđun có độ dài hữu hạn, do đó là Macaulay (Ví dụ 1, No. 1). Giả sử $\dim(M_p)$ là khác không, nghĩa là $p$ không phải là một phần tử cực tiểu của $\mathrm{Supp}(M)$ (VIII, § 1, No. 4, Prop. 9 a)). Vì M không có iđêan nguyên tố liên kết nhúng, nên $p$ không được chứa trong bất kỳ iđêan nguyên tố liên kết nào của M, và tồn tại một phần tử $x$ của $p$ sao cho phép vị tự $x_M$ là đơn ánh (§ 1, Nhận xét 2). Khi đó phép vị tự $x_{M_p}$ là đơn ánh, và ta có $\dim(M_p/xM_p) < \dim(M_p)$ (VIII, § 3, No. 2, Prop. 3). Theo giả thiết quy nạp áp dụng cho A-môđun $M/xM$ và cho iđêan nguyên tố $p$ của $\mathrm{Supp}(M/xM)$, $A_p$-môđun $M_p/xM_p$ là Macaulay, điều này kéo theo rằng $A_p$-môđun $M_p$ là Macaulay (No. 3, Prop. 4).

### 5. Các vành Macaulay

#### Định nghĩa 3 {#ac-x-s2-def-3 .statement}

*Người ta nói rằng một vành $\Lambda$ là Macaulay, hay là một vành Macaulay, nếu nó là Noether và $\Lambda$-môđun $\Lambda$ là Macaulay.*

#### Ví dụ 1 {#ac-x-s2-n5-exa-1 .statement}

Mọi vành Artin đều là một vành Macaulay (No. 1, Ví dụ 1).

#### Ví dụ 2 {#ac-x-s2-n5-exa-2 .statement}

Một vành Macaulay không có iđêan nguyên tố liên kết nhúng (No. 2, Prop. 2). Ngược lại, cho $A$ là một vành Noether có chiều $\leqslant 1$ và không có iđêan nguyên tố liên kết nhúng; với mọi tập con hữu hạn khác rỗng phân cắt mạnh S của A, A-môđun $A/SA$ có chiều $\leqslant 0$, do đó là Macaulay (No. 1, Ví dụ 1); vì thế A là một vành Macaulay (No. 4, Định lý 2). Đặc biệt, một vành Noether rút gọn có chiều $\leqslant 1$ là một vành Macaulay.

#### Ví dụ 3 {#ac-x-s2-n5-exa-3 .statement}

Một vành Noether chuẩn tắc có chiều $\leqslant 2$ là một vành Macaulay (§ 1, No. 10, đoạn văn đứng trước Định lý 4). Ngược lại, cho $A$ là một vành Macaulay mà vành địa phương $A_p$ tại mọi iđêan nguyên tố $p$ có chiều cao $\leqslant 1$ đều đóng nguyên; khi đó A là chuẩn tắc (§ 1, No. 10, Định lý 4).

#### Ví dụ 4 {#ac-x-s2-n5-exa-4 .statement}

Nếu $A$ là một vành Macaulay, thì $S^{-1}A$ cũng vậy đối với mọi tập con nhân $S$ của $A$ (No. 1, Nhận xét). Ngược lại, nếu vành $A_m$ là một vành Macaulay với mọi iđêan cực đại $m$ của $A$, thì vành $A$ là Macaulay (No. 1, Def. 1).

#### Ví dụ 5 {#ac-x-s2-n5-exa-5 .statement}

Cho $A$ là một vành Noether và $J$ một iđêan của $A$. Để $A/J$ là một vành Macaulay, điều kiện cần và đủ là nó là một $\Lambda$-môđun Macaulay (No. 1, Ví dụ 4).

#### Ví dụ 6 {#ac-x-s2-n5-exa-6 .statement}

Cho $A$ là một vành địa phương Noether và $J$ một iđêan của $A$ được sinh bởi một dãy chính quy của $A$. Để $A/J$ là một vành Macaulay, điều kiện cần và đủ là $A$ là như vậy (Ví dụ 5 và Mệnh đề 4 của No. 3).

#### Ví dụ 7 {#ac-x-s2-n5-exa-7 .statement}

Để một vành địa phương Noether $A$ là một vành Macaulay, điều kiện cần và đủ là nó có một iđêan xác định sinh bởi một dãy $A$-chính quy: điều này suy ra từ Mệnh đề 3 của No. 3, và từ thực tế rằng một dãy $A$-chính quy gồm các phần tử của $m_A$ sinh ra một iđêan xác định khi và chỉ khi nó có độ dài $\dim(A)$ (VIII, § 3, No. 2, Định lý 1 và hệ quả của Mệnh đề 3). Đặc biệt, mọi vành địa phương Noether chính quy đều là một vành Macaulay (VIII, § 5, No. 2, Định lý 1). Nói chung hơn, thương của một vành địa phương Noether chính quy $A$ bởi một iđêan sinh bởi một dãy $A$-chính quy là một vành Macaulay (Ví dụ 6).

#### Mệnh đề 7 {#ac-x-s2-prop-7 .statement}

Cho $A$ là một vành Noether. Các điều kiện sau là tương đương:

(i) $A$ là một vành Macaulay;
(ii) với mọi tập con đóng $F$ của $\mathrm{Spec}(A)$, ta có $\mathrm{prof}_F(A) = \mathrm{codim}(F)$;
(iii) mọi iđêan $J$ của $A$ đều chứa một dãy $A$-chính quy có độ dài $\mathrm{ht}(J)$;
(iii') mọi iđêan cực đại $m$ của $A$ đều chứa một dãy $A$-chính quy có độ dài $\mathrm{ht}(m)$;
(iv) với mọi iđêan $J$ của $A$, ta có $\mathrm{Ext}_A^i(A/J, A) = 0$ với $i < \mathrm{ht}(J)$;
(iv') với mọi iđêan cực đại $m$ của $A$, ta có $\mathrm{Ext}_A^i(A/m, A) = 0$ với $i < \mathrm{ht}(m)$;
(v) với mọi iđêan nguyên tố $p$ của $A$ và mọi iđêan $J$ của $A_p$ sinh bởi một dãy cát tuyến cực đại đối với $A_p$, ta có $e_J(A_p) = \mathrm{long}(A_p/ JA_p)$;
(v') với mọi iđêan cực đại $m$ của $A$, tồn tại một iđêan $J$ của $A_m$, sinh bởi một dãy cát tuyến cực đại đối với $A_m$, thỏa mãn $e_J(A_m) = \mathrm{long}(A_m/ JA_m)$;
(vi) (tiêu chuẩn Macaulay-Cohen) với mọi tập con hữu hạn $S$ của $A$ sao cho iđêan $\mathfrak{S}$ sinh bởi $S$ có chiều cao $\mathrm{Card}(S)$, $A$-môđun $A/\mathfrak{S}$ không có iđêan nguyên tố liên kết nhúng.

Tính tương đương của (i) và (ii) suy ra từ No. 1, hệ quả của Mệnh đề 1. Theo Định lý 2 của § 1, No. 4, và định nghĩa của độ sâu, các điều kiện (iii) và (iv) (tương ứng (iii') và (iv')) có nghĩa là ta có $\mathrm{prof}_A(J; A) \geq \mathrm{ht}(J)$ với mọi iđêan (tương ứng mọi iđêan cực đại) $J$ của $A$. Do đó ta có

$$
(i) \Leftrightarrow (ii) \Rightarrow (iii) \Leftrightarrow (iv) \Rightarrow (iii') \Leftrightarrow (iv').
$$

Nhưng (iv') kéo theo, với mọi iđêan cực đại $m$ của $A$, $\mathrm{Ext}_{A_m}^i(\kappa(m), A_m) = 0$ với $i < \dim(A_m)$, do đó $\mathrm{prof}(A_m) \geq \dim(A_m)$, suy ra $A$ là một vành Macaulay.

Tính tương đương của (i), (v) và (v’) suy ra từ Định lý 1 của No. 3, và tính tương đương của (i) và (vi) suy ra từ Định lý 2 của No. 4.

### 6. Môđun Macaulay và các đại số hữu hạn

#### Nhận xét {#ac-x-s2-n6-rem-1 .statement}

Cho $\rho : A \to B$ là một đồng cấu vành, và lấy $p \in \mathrm{Spec}(A)$. Ta ký hiệu bởi $\overline{B}$ vành $\kappa(p) \otimes_A B$. Nó có thể được đồng nhất với $S^{-1}B/p(S^{-1}B)$, trong đó $S$ là tập con nhân $\rho(A - p)$ của $B$; do đó các iđêan nguyên tố của $\overline{B}$ là các iđêan $q\overline{B}$, trong đó $q$ là một iđêan nguyên tố của $B$ chứa $pB$ và không giao với $S$, nói cách khác là một iđêan nguyên tố của $B$ nằm trên $p$. Đối với một iđêan như vậy $q$, ta có $S \subset B - q$, nên vành địa phương của $\overline{B}$ tại $q\overline{B}$ có thể được đồng nhất với $B_q/pB_q$, tức là lại được đồng nhất với $\kappa(p) \otimes_A B_q$.

Tương tự, nếu $N$ là một $B$-môđun, thì $\overline{B}_{q\overline{B}}$-môđun $(\kappa(p) \otimes_A N)_{q\overline{B}}$ có thể được đồng nhất với $\kappa(p) \otimes_A N_q$. Giả sử thêm rằng $B$-môđun $N$ là sinh hữu hạn; theo bổ đề Nakayama, điều kiện $\kappa(p) \otimes_A N_q = 0$ là tương đương với $N_q = 0$. Vậy giá của $\overline{B}$-môđun $\kappa(p) \otimes_A N$ gồm các iđêan $q\overline{B}$, trong đó $q$ chạy qua các iđêan nguyên tố của $\mathrm{Supp}_B(N)$ nằm trên $p$. Đặc biệt, để môđun $\kappa(p) \otimes_A N$ khác không, điều kiện cần và đủ là tồn tại một iđêan nguyên tố của $\mathrm{Supp}_B(N)$ nằm trên $p$.

#### Mệnh đề 8 {#ac-x-s2-prop-8 .statement}

Cho $\rho : A \to B$ là một đồng cấu của các vành Noether và $N$ là một $B$-môđun đồng thời là một $A$-môđun sinh hữu hạn. Để $A$-môđun $N$ là Macaulay, điều kiện cần và đủ là $B$-môđun $N$ là Macaulay và, với mọi cặp $(n, n')$ các iđêan cực đại của $\mathrm{Supp}_B(N)$ sao cho $\rho^{-1}(n) = \rho^{-1}(n')$, ta có $\dim_{B_n}(N_n) = \dim_{B'_n}(N'_n)$.

A-môđun $B/\mathrm{Ann}_B(N)$ đẳng cấu với một môđun con của A-môđun sinh hữu hạn $\mathrm{End}_A(N)$, và vì vậy có kiểu hữu hạn. Thay thế $A$ bằng $A/\mathrm{Ann}_A(N)$ và $B$ bằng $B/\mathrm{Ann}_B(N)$, ta được đưa về trường hợp $\rho$ là đơn ánh và làm cho $B$ thành một A-đại số hữu hạn, đồng thời ta có $\mathrm{Supp}_A(N) = \mathrm{Spec}(A)$ và $\mathrm{Supp}_B(N) = \mathrm{Spec}(B)$. Ánh xạ $f : \mathrm{Spec}(B) \to \mathrm{Spec}(A)$ suy ra từ $\rho$ khi đó là toàn ánh, và một iđêan nguyên tố $q$ của $B$ là cực đại khi và chỉ khi $f(q)$ là một iđêan cực đại của $A$ (V, § 2, No. 1, đl. 1 và mđ. 1).

Cho $m$ là một iđêan cực đại của $A$. Theo nhận xét trên, các iđêan nguyên tố của vành $B_m$ chứa $mB_m$ là các iđêan có dạng $qB_m$, trong đó $q \in \mathrm{Spec}(B)$ là một iđêan của $B$ (tất yếu cực đại) sao cho $f(q) = m$. Ta có

$$
\mathrm{prof}_{A_m}(N_m) = \mathrm{prof}_{B_m}(mB_m; N_m) = \inf_{q \in f^{-1}(m)} (\mathrm{prof}_{B_q}(N_q))
$$

(§ 1, No. 3, mđ. 4 và No. 5, mđ. 8), và

$$
\dim_{A_m}(N_m) = \dim_{B_m}(N_m) = \sup_{q \in f^{-1}(m)} (\dim_{B_q}(N_q))
$$

(VIII, § 2, No. 3, đl. 1 và § 1, No. 4, mđ. 9). Vì ta có $\mathrm{prof}_{B_q}(N_q) \leq \dim_{B_q}(N_q)$ với mọi $q \in f^{-1}(m)$, mệnh đề được suy ra từ các đẳng thức này.

#### Hệ quả 1 {#ac-x-s2-prop-8-cor-1 .statement}

Cho $\rho : A \to B$ là một đồng cấu của các vành Noether. Nếu $B$ là một A-đại số hữu hạn và là một A-môđun Macaulay, thì nó là một vành Macaulay. Nếu hơn nữa $\rho$ là đơn ánh, thì ta có $\mathrm{ht}(aB) = \mathrm{ht}(a)$ đối với mọi iđêan $a$ của $A$, và $\mathrm{ht}(b) = \mathrm{ht}(\rho^{-1}(b))$ đối với mọi iđêan $b$ của $B$.

Mệnh đề đầu tiên suy ra từ Mệnh đề 8. Giả sử $\rho$ đơn ánh. Cho $a$ là một iđêan của $A$. Ta có $\mathrm{ht}(a) = \mathrm{prof}_A(a; B)$ vì $A$-môđun $B$ là Macaulay, có giá bằng $\mathrm{Spec}(A)$ (No. 1, hệ quả của Mệnh đề 1), $\mathrm{ht}(aB) = \mathrm{prof}_B(aB; B)$ (*loc. cit.*) và $\mathrm{prof}_A(a; B) = \mathrm{prof}_B(aB; B)$ ($§ 1$, No. 3, Mệnh đề 4), do đó $\mathrm{ht}(aB) = \mathrm{ht}(a)$. Cho $b$ là một iđêan của $B$. Từ điều ở trên, ta có $\mathrm{ht}(\rho^{-1}(b)) = \mathrm{ht}(\rho^{-1}(b)B)$. Nhưng $\rho^{-1}(b)B$ được chứa trong $b$, do đó có chiều cao nhỏ hơn $\mathrm{ht}(b)$, và ta có $\mathrm{ht}(b) \leq \mathrm{ht}(\rho^{-1}(b))$ theo VIII, $§ 2$, No. 3, Định lý 1, b).

#### Hệ quả 2 {#ac-x-s2-prop-8-cor-2 .statement}

Cho $A$ là một vành Noether nguyên đóng và $B$ là một vành chứa $A$. Giả sử rằng $B$ là một $A$-môđun không xoắn, kiểu hữu hạn. Nếu $B$ là một vành Macaulay thì $A$-môđun $B$ là Macaulay.

Thật vậy, hai iđêan nguyên tố của $B$ nằm trên cùng một iđêan của $A$ có cùng chiều cao (VIII, $§ 2$, No. 3, Định lý 2). Do đó có thể áp dụng Mệnh đề 8 với $N = B$.

#### Hệ quả 3 {#ac-x-s2-prop-8-cor-3 .statement}

Cho $A$ là một vành nguyên đóng, $K$ là trường phân thức của nó, $L$ là một $K$-đại số hữu hạn sao cho $[L : K] 1_A$ khả nghịch trong $A$, và $B$ là một dưới-$A$-đại số của $L$, hữu hạn trên $A$.

a) *Dưới*-$A$-*môđun* $Al_B$ của $B$ là một nhân tử trực tiếp.

b) *Với mọi iđêan* $J$ *của* $A$, *ta có bất đẳng thức* $\mathrm{prof}_A(J; A) \geq \mathrm{prof}_B(JB; B)$.

c) *Nếu* $B$ *là một vành Macaulay*, *thì điều đó cũng đúng với* $A$.

Ánh xạ tuyến tính $K$ $\mathrm{Tr}_{L/K} : L \to K$ ánh xạ $B$ vào $A$ (V, $§ 1$, No. 6, hệ quả 2 của Mệnh đề 17), và do đó xác định bằng hạn chế một ánh xạ tuyến tính $A$ $t : B \to A$. Với mọi $x \in A$, ta có $t(xl_B) = [L : K] x$, do đó a).

Theo Mệnh đề 4 của $§ 1$, No. 3, ta có $\mathrm{prof}_A(J; B) = \mathrm{prof}_B(JB; B)$; nhưng theo a) và Nhận xét 4 của $§ 1$, No. 1, ta có $\mathrm{prof}_A(J; A) \geq \mathrm{prof}_A(J; B)$, do đó b).

Nếu vành $B$ là Noether, thì $A$ cũng vậy: thật vậy, theo a) ta có $aB \cap A = a$ đối với mọi iđêan $a$ của $A$; do đó mọi dãy tăng $(a_n)_{n \in \mathbf{N}}$ các iđêan của $A$ đều dừng vì dãy $(a_nB)_{n \in \mathbf{N}}$ là dừng. Dưới các giả thiết của c), $A$-môđun $B$ là Macaulay (Hệ quả 2), và điều đó cũng đúng với $A$-môđun $A$ (No. 1, Ví dụ 2).

#### Ví dụ {#ac-x-s2-n6-exa-1 .statement}

Hệ quả 3 được áp dụng đặc biệt trong hai tình huống sau:

a) Xét một vành Noether nguyên đóng $A$, một mở rộng tách được $L$ của trường phân thức của nó, có bậc hữu hạn $n$ sao cho $n1_A$ là khả nghịch trong $A$, và lấy $B$ là bao đóng nguyên của $A$ trong $L$ (V, $§ 1$, No. 6, Hệ quả 1 của Mệnh đề 18).

b) Xét một vành Noether nguyên đóng $B$ và một nhóm hữu hạn $G$ các tự đẳng cấu của $B$, sao cho $\mathrm{Card}(G) 1_B$ là khả nghịch trong $B$. Lấy $A$ là vành các phần tử của $B$ bất biến dưới tác động của $G$. Hãy kiểm tra rằng ta đang ở trong một trường hợp riêng của a). Nhóm $G$ tác động trên trường của

Đặc biệt, nếu B là một vành Macaulay, thì A cũng vậy.

### 7. Môđun Macaulay và Đại số Phẳng

#### Mệnh đề 9 {#ac-x-s2-prop-9 .statement}

Cho ρ : A → B là một đồng cấu của các vành Noether, M một A-môđun hữu hạn sinh và N một B-môđun hữu hạn sinh, phẳng trên A. Ký hiệu bởi $^a\rho : \mathrm{Spec}(B) \longrightarrow \mathrm{Spec}(\Lambda)$ ánh xạ liên kết với ρ. Các điều kiện sau là tương đương:

(i) B-môđun $M \otimes_A N$ là Macaulay;
(ii) $(\kappa(p) \otimes_A B)$-môđun $\kappa(p) \otimes_A N$ là Macaulay với mọi $p \in \mathrm{Supp}_A(M)$, và $A_p$-môđun $M_p$ là Macaulay với mọi $p \in ^a\rho(\mathrm{Supp}_B(N))$;
(iii) với mọi iđêan cực đại của $\mathrm{Supp}_B(N)$ mà ảnh ngược $p$ của nó trong A thuộc $\mathrm{Supp}_A(M)$, $A_p$-môđun $M_p$ và $(\kappa(p) \otimes_A B)$-môđun $\kappa(p) \otimes_A N$ đều là Macaulay.

Hơn nữa, nếu B-môđun N là phẳng trung thành, thì các điều kiện này suy ra rằng A-môđun M là Macaulay.

Cho q là một iđêan nguyên tố của B thuộc giá của $M \otimes_A N$. Đặt $p = \rho^{-1}(q)$. Vì môđun $(M \otimes_A N)_q$ được đồng nhất với $M_p \otimes_{A_p} N_q$, nên các môđun $M_p$ và $N_q$ khác không, và điều đó cũng đúng với $\kappa(p) \otimes_A N_q$ (No. 6, Nhận xét). $A_p$-môđun $N_q$, đẳng cấu với một môđun phân thức của $N_p$, là phẳng và ta có các đẳng thức

$$
\mathrm{prof}_{B_q}((M \otimes_A N)_q) = \mathrm{prof}_{A_p}(M_p) + \mathrm{prof}_{B_q}(\kappa(p) \otimes_A N_q)
$$
$$
\dim_{B_q}((M \otimes_A N)_q) = \dim_{A_p}(M_p) + \dim_{B_q}(\kappa(p) \otimes_A N_q)
$$

(§ 1, No. 6, mệnh đề 11, b) và nhận xét), trong đó mỗi số hạng là một số nguyên $\geq 0$. Tính đến sự kiện rằng $B_q$-môđun $\kappa(p) \otimes_A N_q$ là một môđun Macaulay khi và chỉ khi nó là như vậy với tư cách là một $(\kappa(p) \otimes_A B_q)$-môđun (No. 1, ví dụ 4), ta suy ra sự tương đương của hai điều kiện sau:

(α) $B_q$-môđun $(M \otimes_A N)_q$ là một môđun Macaulay;
(β) $A_p$-môđun $M_p$ và $(\kappa(p) \otimes_A B_q)$-môđun $\kappa(p) \otimes_A N_q$ là các môđun Macaulay.

Bây giờ chứng minh rằng (iii) suy ra (i). Cho n là một iđêan cực đại của B thuộc giá của $M \otimes_A N$, và đặt $p = \rho^{-1}(n)$. Từ phần trên ta có $p \in \mathrm{Supp}_A(M) \cap ^a\rho(\mathrm{Supp}_B(N))$; điều kiện (iii) và nhận xét của No. 6 suy ra rằng điều kiện (β) ở trên được thỏa mãn với $q = n$. Suy ra $B_n$-môđun $(M \otimes_A N)_n$ là một môđun Macaulay, do đó có (i).

Hệ quả (ii) ⇒ (iii) là hiển nhiên; hãy chứng minh rằng (i) suy ra (ii). Giả sử B-môđun M ⊗_A N là một môđun Macaulay. Cho p là một phần tử của Supp_A(M). Ta có thể giả sử rằng $(\kappa(p) \otimes_A B)$-môđun κ(p) ⊗_A N là khác không, nghĩa là, tồn tại một iđêan nguyên tố q của Supp_B(N) nằm trên p (No. 6, nhận xét). B_q-môđun (M ⊗_A N)_q là một môđun Macaulay (No. 1, ví dụ 3); từ hệ quả (α) ⇒ (β) đã được chứng minh ở trên và từ nhận xét của No. 6 suy ra rằng A_p-môđun M_p và $(\kappa(p) \otimes_A B)$-môđun (κ(p) ⊗_A N) là các môđun Macaulay, do đó có (ii).

Nếu hơn nữa N là phẳng trung thành trên A, ta có κ(p) ⊗_A N ≠ 0 với mọi p ∈ Spec(A), do đó a_p(Supp_B(N)) = Spec(A) (No. 6, nhận xét), vì thế (ii) suy ra rằng M là một môđun Macaulay.

#### Hệ quả 1 {#ac-x-s2-prop-9-cor-1 .statement}

Cho ρ : Λ → B là một đồng cấu địa phương của các vành địa phương Noether, M là một A-môđun hữu hạn sinh khác không và N là một B-môđun hữu hạn sinh khác không đồng thời là một A-môđun phẳng. Để B-môđun M ⊗_A N là một môđun Macaulay, điều kiện cần và đủ là A-môđun M là một môđun Macaulay và B/m_A B-môđun N/m_A N là một môđun Macaulay.

Thật vậy, N là một A-môđun phẳng trung thành vì N/m_A N là khác không (I, § 3, No. 1, định nghĩa 1).

#### Hệ quả 2 {#ac-x-s2-prop-9-cor-2 .statement}

Cho ρ : A → B là một đồng cấu của các vành Noether biến B thành một A-môđun phẳng trung thành, và cho M là một A-môđun hữu hạn sinh. Để B-môđun M ⊗_A B là một môđun Macaulay, điều kiện cần và đủ là A-môđun M là một môđun Macaulay và κ(p) ⊗_Λ B là một vành Macaulay với mọi p ∈ Supp(M).

#### Hệ quả 3 {#ac-x-s2-prop-9-cor-3 .statement}

Cho A là một vành Noether, B là một Λ-đại số hữu hạn phẳng, M là một A-môđun Macaulay hữu hạn sinh. Khi đó B-môđun M ⊗_A B là một môđun Macaulay.

Thật vậy, với mọi p ∈ Spec(A), vành κ(p) ⊗_Λ B là một κ(p)-đại số hữu hạn, do đó là một vành Macaulay (No. 5, ví dụ 1), và ta áp dụng mệnh đề 9.

#### Hệ quả 4 {#ac-x-s2-prop-9-cor-4 .statement}

Cho A là một vành Noether, J là một iđêan của A và M là một A-môđun hữu hạn sinh. Ký hiệu Ā và Ĝ lần lượt là các hoàn thành tách của A và M đối với tôpô J-adic, và ký hiệu S là tập con nhân 1 + J của Λ. Xét các điều kiện sau:

(i) A-môđun M là một môđun Macaulay;
(ii) Ā-môđun Ĝ là một môđun Macaulay;
(iii) S^{-1}A-môđun S^{-1}M là một môđun Macaulay;
(iv) với mọi iđêan cực đại m ∈ Supp(M) ∩ V(J), A_m-môđun M_m là một môđun Macaulay;
(v) với mọi iđêan nguyên tố p ∈ Supp(M) sao cho p + J ≠ A, Λ_p-môđun M_p là một môđun Macaulay và vành κ(p) ⊗_A Ā là một vành Macaulay.

Các điều kiện (ii) đến (v) là tương đương, và được suy ra từ (i). Khi iđêan J được chứa trong căn của A, các điều kiện (i) đến (v) là tương đương.

Ta biết rằng (i) suy ra (iii) (No. 1, ví dụ 3), và (iii) trùng với (i) khi J được chứa trong căn của A (vì khi đó các phần tử của S là khả nghịch).

Hiển nhiên là (v) suy ra (iv) và (iv) suy ra (i).

(i) $\Rightarrow$ (ii) : Cho $m$ là một iđêan cực đại của $A$; khi đó $m\widehat{A}$ là một iđêan cực đại của $\widehat{A}$ nằm trên $m$, và mọi iđêan cực đại của $\widehat{A}$ đều thu được theo cách này (III, § 3, No. 4, mệnh đề 8). Vành $\kappa(m) \otimes_A \widehat{A}$ là một trường, do đó là một vành Macaulay; nếu $A$-môđun $M$ là một môđun Macaulay, thì điều tương tự cũng đúng với $\widehat{A}$-môđun $\widehat{M}$ theo hệ quả (iii) $\Rightarrow$ (i) của mệnh đề 9.

(ii) $\Rightarrow$ (v) : $\widehat{A}$-môđun $\widehat{M}$ đẳng cấu với $M \otimes_A \widehat{A}$ (III, § 3, No. 4, định lý 3); nếu nó là một môđun Macaulay, thì từ mệnh đề 9, (i) $\Rightarrow$ (ii) suy ra rằng $\kappa(p) \otimes_A \widehat{A}$ là một vành Macaulay với mọi $p \in \mathrm{Supp}(M)$, và rằng $A$-môđun $M$ là một môđun Macaulay.

#### Mệnh đề 10 {#ac-x-s2-prop-10 .statement}

*Cho $\rho : A \to B$ là một đồng cấu của các vành Noether biến $B$ thành một $\Lambda$-môđun phẳng. Các điều kiện sau là tương đương:*

(i) $B$ là một vành Macaulay;
(ii) với mọi iđêan nguyên tố $q$ của $B$, các vành $A_{\rho^{-1}(q)}$ và $\kappa(\rho^{-1}(q)) \otimes_A B$ là các vành Macaulay;
(iii) với mọi iđêan cực đại $n$ của $B$, các vành $A_{\rho^{-1}(n)}$ và $\kappa(\rho^{-1}(n)) \otimes_A B$ là các vành Macaulay.

*Nếu hơn nữa $B$ là phẳng trung thành trên $A$, thì các điều kiện này suy ra rằng $A$ là một vành Macaulay.*

Đây là trường hợp riêng $M = A$, $N = B$ của mệnh đề 9.

#### Hệ quả 1 {#ac-x-s2-prop-10-cor-1 .statement}

*Mọi đại số hữu hạn phẳng trên một vành Macaulay đều là một vành Macaulay.*

#### Hệ quả 2 {#ac-x-s2-prop-10-cor-2 .statement}

*Cho $A$ là một vành Macaulay và $n$ là một số nguyên dương; khi đó $A[X_1, \ldots, X_n]$ và $A[[X_1, \ldots, X_n]]$ là các vành Macaulay.*

Chỉ cần xét trường hợp $n = 1$. Vành $A[T]$ là Noether (A, VIII, § 1, No. 4, hệ quả 1), và, với mọi trường $k$, vành $k[T]$ là một vành Macaulay (No. 5, ví dụ 2); do đó, vành $A[T]$ là một vành Macaulay (mệnh đề 10) và vành $A[[T]]$ là một vành Macaulay (hệ quả 4 của mệnh đề 9).

#### Hệ quả 3 {#ac-x-s2-prop-10-cor-3 .statement}

*Mọi đại số kiểu hữu hạn trên một vành Macaulay Noether đều là catenary.*

Thật vậy, một đại số như thế là một thương của một vành đa thức trên một vành Macaulay, nên là một thương của một vành Macaulay (hệ quả 2), và vì thế là catenary (No. 2).

## BÀI TẬP {#ac-x-s2-exercises}

Xem [các bài tập cho § 2](exercises/s2/).
