---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 6
section_title: Dimension des anneaux gradués
lang: vi
source: ac-viii-ix-fr
book_pages: AC VIII.62-AC VIII.71, AC VIII.99-AC VIII.103
pdf_pages: 0066-0075, 0103-0107
extraction: ocr
subsections:
    - "no": 1
      title: Anneau filtré associé à un anneau gradué
      page: 62
      pdf_page: 66
    - "no": 2
      title: Dimension et chaînes d’idéaux gradués
      page: 0
      pdf_page: 67
    - "no": 3
      title: Dimension des modules gradués
      page: 0
      pdf_page: 69
    - "no": 4
      title: Semi-continuité de la dimension
      page: 69
      pdf_page: 73
    - "no": 5
      title: Algèbres graduées régulières
      page: 70
      pdf_page: 74
statements: 27
exercises: 12
content_sha256: 634531968e2e4dcbc916124e4ab036767603b27649e7a75e22024fe26672c96e
translated_from: content/en-mt/ac/VIII/06_s6_dimension_des_anneaux_gradues.md
source_lang: en-mt
translation_method: machine
source_content_sha256: cd74be55508776d60669c1571cc5c9338eb457742737242bb5c2cdb3474475d5
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5-6
translation_run: translate-vi-b495df1a
glossary_version: 34
glossary_terms_sha256: 83effe55b16562deaa4d2141a26bce4de9443f6a9fd14a201fd5c7f9545a66be
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. CHIỀU CỦA CÁC VÀNH PHÂN BẬC

Trong đoạn này, H ký hiệu một vành phân bậc kiểu $\mathbf{Z}$, với các bậc dương, và $(H_n)_{n \in \mathbf{Z}}$ là phép phân bậc của nó; do đó có $H_n = \{0\}$ với $n < 0$.

### 1. Vành lọc liên kết với một vành phân bậc

Với mọi $n \in \mathbf{Z}$, đặt $H_{\geq n} = \sum_{i \geq n} H_i$. Ta có $H = H_{\geq 0}$; các $H_{\geq n}$ là các iđêan phân bậc của H. Gọi S là tập con nhân $1 + H_{\geq 1}$ tạo bởi các phần tử của H mà thành phần có bậc 0 bằng 1, và xét vành phân thức $S^{-1}H$. Ta đồng nhất H với một vành con của phần hoàn thành của nó $\hat{H} = \prod_{n} H_n$ (III, § 2, No. 12, Ví dụ 1); vì các phần tử của S là khả nghịch trong $\hat{H}$ (III, § 2, No. 13, Bổ đề 3), $S^{-1}H$ được đồng nhất với một vành con của $\hat{H}$ chứa H. Với $s \in S$ và $h \in H_{\geq n}$, phần tử $s^{-1}h - h$ của $\hat{H}$ thuộc về $\prod_{i \geq n} H_i$; do đó ta có $S^{-1}H_{\geq n} = (S^{-1}H) \cap \prod_{i \geq n} H_i$.

Từ đó suy ra:

#### Mệnh đề 1 {#ac-viii-s6-prop-1 .statement}

a) Các iđêan $S^{-1}H_{\geq n}$ tạo thành một phép lọc đầy đủ và tách được của vành $S^{-1}H$.

b) Đồng cấu chính tắc của H vào $S^{-1}H$ cảm sinh với mỗi $n$ một đẳng cấu $u_n$ của $H_n$ lên $S^{-1}H_{\geq n}/S^{-1}H_{\geq n+1}$; các $u_n$ là các thành phần thuần nhất của một đẳng cấu của các vành phân bậc từ H lên vành phân bậc liên kết với $S^{-1}H$, được lọc bởi các $S^{-1}H_{\geq n}$.

#### Nhận xét 1 {#ac-viii-s6-n1-rem-1 .statement}

Một phần tử $h/s$ của $S^{-1}H$ với $h \in H, s \in S$, là khả nghịch khi và chỉ khi thành phần có bậc 0 của $h$ là khả nghịch trong $H_0$. Do đó, nếu vành $H_0$ là địa phương, vành $S^{-1}H$ là địa phương và đơn ánh chính tắc $H_0 \to S^{-1}H$ cảm sinh một đẳng cấu của các trường thặng dư.

#### Nhận xét 2 {#ac-viii-s6-n1-rem-2 .statement}

Giả sử rằng $H$ được sinh bởi $H_0$ và $H_1$; khi đó với mọi $n$, ta có $H_{n+1} = H_1.H_n$, do đó $H_{\geq n+1} = H_1.H_{\geq n}$ và $S^{-1}H_{\geq n+1} = H_1.S^{-1}H_{\geq n}$. Suy ra rằng phép lọc $(S^{-1}H_{\geq n})$ của $S^{-1}H$ là phép lọc $S^{-1}H_{\geq 1}$-adic.

#### Ví dụ 1 {#ac-viii-s6-n1-exa-1 .statement}

\* Cho $p$ là một iđêan nguyên tố phân bậc của $\mathbf{C}[X_0, ..., X_n]$ khác với iđêan sinh bởi các $X_i$; cho $V$ là đa tạp con đại số của $\mathbf{P}^n(\mathbf{C})$ được xác định bởi $p$ và $C$ là đa tạp con đại số của $\mathbf{C}^{n+1}$ được xác định bởi $p$. Khi đó $C$ là nón có cơ sở là $V$, $H = \mathbf{C}[X_0, ..., X_n]/p$ là đại số affine của $C$ và $S^{-1}H$ là vành địa phương của nón $C$ tại đỉnh của nó. \*
2) Cho $A$ là một vành địa phương và $a$ là một iđêan của $A$ phân biệt với $A$. Khi đó $H = \bigoplus_n a^n/a^{n+1}$ là một vành phân bậc sao cho $H_0 = A/a$ là địa phương; nó được sinh bởi $H_0$ và $H_1$. Do đó vành $S^{-1}H$ là địa phương và phép lọc $(S^{-1}H_{\geq n})$ là phép lọc $S^{-1}H_{\geq 1}$-adic. Cần lưu ý rằng nói chung các vành $A$ và $S^{-1}H$ không đẳng cấu. \* Đặc biệt, một đa tạp đại số nói chung không đẳng cấu địa phương trong một lân cận của một điểm với nón tiếp xúc của nó tại điểm đó. \*

### 2. Chiều và các dây chuyền của các iđêan phân bậc

Trong số này, ta sẽ ký hiệu dimgr(H) là cận trên nhỏ nhất của độ dài các dây chuyền các iđêan nguyên tố phân bậc của $H$; tương tự, nếu $p$ là một iđêan nguyên tố phân bậc của $H$, ta sẽ ký hiệu htgr(p) là cận trên nhỏ nhất của độ dài các dây chuyền các iđêan nguyên tố phân bậc của $H$ mà $p$ là phần tử lớn nhất. Nếu $p$ là một iđêan nguyên tố phân bậc của $H$, ta có $p \cap S = \varnothing$; thật vậy, nếu không thì $p$ sẽ chứa một phần tử mà thành phần có bậc 0 của nó bằng 1, do đó sẽ chứa 1 vì nó là phân bậc. Ánh xạ $p \mapsto S^{-1}p$ từ tập hợp các iđêan nguyên tố phân bậc của $H$ vào tập hợp các iđêan nguyên tố của $S^{-1}H$ do đó là đơn ánh và tăng (II, § 2, no. 5, prop. 11); do đó, xét đến § 1, no. 3, prop. 6 và hệ quả của prop. 7, ta có:

#### Mệnh đề 2 {#ac-viii-s6-prop-2 .statement}

a) Ta có $\dim_{\mathrm{gr}}(H) \leq \dim(S^{-1}H) \leq \dim(H)$.
b) Với mọi iđêan nguyên tố phân bậc $p$ của $H$, ta có $\operatorname{ht}_{\mathrm{gr}}(p) \leq \operatorname{ht}(S^{-1}p) = \operatorname{ht}(p)$.

Với mọi iđêan $a$ của $H$, ta ký hiệu $a^{\mathrm{gr}}$ là iđêan phân bậc lớn nhất được chứa trong $a$; ta có $a^{\mathrm{gr}} = \sum_n (a \cap H_n)$.

#### Bổ đề 1 {#ac-viii-s6-lem-1 .statement}

a) Nếu $p$ là một iđêan nguyên tố của $H$, thì $p^{gr}$ là một iđêan nguyên tố.

b) Mọi phần tử cực đại của tập hợp các iđêan phân bậc của $H$ phân biệt với $H$ là một iđêan cực đại của $H$ chứa $H_{\geq 1}$.

c) Mọi iđêan nguyên tố cực tiểu của $H$ đều phân bậc.

a) Điều này suy ra từ III, § 1, no. 4, prop. 4.

b) Cho $m$ là một iđêan phân bậc của $H$ phân biệt với $H$. Khi đó ta có
$$
m \subset (m \cap H_0) + H_{\geq 1} \neq H.
$$
Nếu $m$ là cực đại, thì ta có $m = m_0 + H_{\geq 1}$, trong đó $m_0$ là một iđêan cực đại của $H_0$, do đó $b$.

c) Cho $p$ là một iđêan nguyên tố cực tiểu của $H$. Vì $p^{gr}$ là nguyên tố theo $a$ và được chứa trong $p$, ta có $p = p^{gr}$, do đó $c$.

#### Bổ đề 2 {#ac-viii-s6-lem-2 .statement}

Cho $p$ và $q$ là các iđêan nguyên tố của $H$ sao cho $q \subset p$ và $q \neq p$. Nếu $q^{gr} = p^{gr}$, thì $q$ là phân bậc, $p$ không phải là phân bậc, và $ht(p/q) = 1$.

\* Nhận xét 1. --- Ta xét lại ký hiệu của ví dụ 1 của No. 1. Bổ đề 2 suy ra rằng, nếu hai đa tạp con bất khả quy $Y$ và $Z$ của $\mathbf{C}^{n+1}$ có cùng nón chiếu và nếu $Z \subset Y$ và $Z \neq Y$, thì $Y$ là nón chiếu của $Z$, và $Z$ có đối chiều 1 trong $Y$. \*

Thay thế $H$ bởi $H/q^{gr}$, ta quy về trường hợp $q^{gr} = \{0\}$. Khi đó $H$ là một miền nguyên (bổ đề 1, $a$), $p^{gr} = 0$, và vấn đề là chứng minh rằng $ht(p) \leq 1$: điều này thực sự sẽ suy ra rằng $ht(q) = 0$, do đó $q = \{0\}$. Vì $p^{gr} = \{0\}$, ta có $p \cap H_n = \{0\}$ với mọi $n$, và $p$ rời khỏi tập con nhân $T = \bigcup (H_n - \{0\})$. Vành $H_p$ do đó đẳng cấu với một vành các phân thức của $T^{-1}H$, và do đó ta có
$$
ht(p) = \dim(H_p) \leq \dim(T^{-1}H)
$$
(§ 1, No. 3, mệnh đề 6 và 7). Nhưng, theo bổ đề 4 của V, § 1, No. 8, $T^{-1}H$ là một trường hoặc đẳng cấu với một vành $K[X, X^{-1}]$, trong đó $K$ là một trường; do đó ta có $\dim(T^{-1}H) \leq 1$ và $ht(p) \leq 1$, điều phải chứng minh.

#### Mệnh đề 3 {#ac-viii-s6-prop-3 .statement}

Cho $p$ là một iđêan nguyên tố của $H$. Nếu $p \neq p^{gr}$, thì ta có $ht(p^{gr}) = ht(p) - 1$.

Theo Bổ đề 1, $a$, iđêan $p^{gr}$ là nguyên tố và được chứa trong $p$, do đó $ht(p^{gr}) \leq ht(p) - 1$. Vì mệnh đề là tầm thường khi $ht(p^{gr}) = + \infty$, ta có thể giả sử rằng $ht(p^{gr}) < + \infty$. Ta chứng minh bất đẳng thức $ht(p) \leq ht(p^{gr}) + 1$ bằng quy nạp theo $ht(p^{gr})$. Chỉ cần chứng minh rằng, với mọi iđêan nguyên tố $q$ được chứa trong $p$ và phân biệt với $p$, ta có $ht(q) \leq ht(p^{gr})$. Ta phân biệt hai trường hợp tùy theo $q^{gr} \neq p^{gr}$ hay $q^{gr} = p^{gr}$. Nếu $q^{gr} \neq p^{gr}$, thì có $ht(q^{gr}) < ht(p^{gr})$; ta có
$$
ht(q) \leq ht(q^{gr}) + 1,
$$
theo giả thiết quy nạp nếu $q \neq q^{gr}$ và một cách tầm thường nếu $q = q^{gr}$; do đó, ta có $ht(q) \leq ht(q^{gr}) + 1 \leq ht(p^{gr})$, điều phải chứng minh. Nếu $q^{gr} = p^{gr}$, thì ta có $q = q^{gr}$ theo Bổ đề 2, do đó $ht(q) = ht(q^{gr}) \leq ht(p^{gr})$, từ đó lại có kết luận mong muốn.

#### Định lý 1 {#ac-viii-s6-thm-1 .statement}

Giả sử rằng H là Noether.

a) Mọi chuỗi các iđêan nguyên tố phân bậc của H, bão hòa như một chuỗi các iđêan nguyên tố phân bậc, đều bão hòa như một chuỗi các iđêan nguyên tố.

b) Với mọi iđêan nguyên tố phân bậc p của H, ta có htgr(p) = ht(S^{-1}p) = ht(p).

c) Ta có dimgr(H) = dim(S^{-1}H) = dim(H).

Để chứng minh a), chỉ cần chứng minh rằng, nếu p và q là hai iđêan nguyên tố phân bậc phân biệt của H sao cho q ⊂ p và mọi iđêan nguyên tố phân bậc nằm giữa q và p đều bằng p hoặc bằng q, thì ht(p/q) = 1. Chuyển qua thương theo q, ta được quy về trường hợp q = {0}. Vì vậy, vấn đề là chứng minh rằng, nếu H là một miền nguyên, và nếu p là một iđêan của H, cực tiểu trong các iđêan nguyên tố phân bậc ≠ {0}, thì ta có ht(p) = 1. Bây giờ lấy a là một phần tử thuần nhất khác không của p, và lấy r là một iđêan nguyên tố của H sao cho a ∈ r ⊂ p và cực tiểu đối với các tính chất này (II, § 2, No. 6, Bổ đề 2). Vì r^{gr} là nguyên tố (Bổ đề 1, a)) và khác không, ta có r^{gr} = p, do đó p = r. Vì H là một miền nguyên và Noether, p có chiều cao 1 (§ 3, No. 1, Mệnh đề 1), do đó a).

Ta chứng minh b). Cho p là một iđêan nguyên tố phân bậc của H. Ta có

$$
\text{htgr}(p) \leq \text{ht}(S^{-1}p) \leq \text{ht}(p)
$$

(Mệnh đề 2); ta chứng minh bất đẳng thức ht(p) ≤ htgr(p) bằng quy nạp theo htgr(p). Nếu htgr(p) = 0, p là cực tiểu trong các iđêan nguyên tố phân bậc, do đó là cực tiểu (Bổ đề 1, c)), và ta có ht(p) = 0. Giả sử ta có htgr(p) > 0 và ta chứng minh bất đẳng thức ht(q) ≤ htgr(p) − 1 với mọi iđêan nguyên tố q được chứa trong p và phân biệt với p. Ta phân biệt hai trường hợp. Nếu q là phân bậc, ta kết luận theo giả thiết quy nạp. Nếu q không phân bậc, thì ta có q^{gr} ≠ p, do đó ht(q^{gr}) ≤ htgr(q^{gr}) theo giả thiết quy nạp, từ đó ht(q) ≤ htgr(q^{gr}) + 1 theo Mệnh đề 3; còn lại phải chứng minh bất đẳng thức htgr(q^{gr}) ≤ htgr(p) − 2; nhưng nếu có htgr(q^{gr}) = htgr(p) − 1, chuỗi q^{gr} ⊂ p sẽ bão hòa theo a), điều này không đúng vì q^{gr} ≠ q ≠ p.

Cuối cùng ta chứng minh c). Ta có dimgr(H) ≤ dim(S^{-1}H) ≤ dim(H) (Mệnh đề 2), và còn lại phải chứng minh dim(H) ≤ dimgr(H), hay một lần nữa ht(p) ≤ dimgr(H) với mọi iđêan nguyên tố p của H. Vậy lấy p là một iđêan nguyên tố của H. Nếu p là phân bậc, ta có ht(p) = htgr(p) ≤ dimgr(H). Nếu p không phân bậc, ta có ht(p) = htgr(p^{gr}) + 1 theo Mệnh đề 3; lấy m là một iđêan cực đại phân bậc của H chứa p^{gr}; theo Bổ đề 1, b), m là cực đại, do đó phân biệt với p^{gr}, và ta có htgr(p^{gr}) + 1 ≤ htgr(m) ≤ dimgr(H), từ đó lại có ht(p) ≤ dimgr(H). Điều này hoàn tất chứng minh.

#### Nhận xét 2 {#ac-viii-s6-n2-rem-2 .statement}

Tồn tại các vành phân bậc không Noether H sao cho dimgr(H) < dim(H) (p. 99, Bài tập 1).

### 3. Chiều của các môđun phân bậc

Trong số này, M ký hiệu một H-môđun phân bậc (kiểu $\mathbf{Z}$).
Khi đó S^{-1}M là một S^{-1}H-môđun, và nếu đặt $M_{\geq n} = \bigoplus_{i \geq n} M_i$, ta thấy như trong No. 1 rằng dãy các tập hợp $S^{-1}M_{\geq n}$ là một lọc đầy đủ và tách được trên

$S^{-1}M$ và rằng ánh xạ chính tắc $M \to S^{-1}M$ cảm sinh một đẳng cấu của $M$ lên môđun phân bậc $\bigoplus_n S^{-1}M_{\geq n}/S^{-1}M_{\geq n+1}$.

#### Bổ đề 3 {#ac-viii-s6-lem-3 .statement}

Giả sử rằng $H$ được sinh bởi $H_0 \cup H_1$ và $M$ được sinh bởi $\bigoplus_{i \leq n_0} M_i$ với một số nguyên $n_0$ thích hợp. Khi đó lọc $(S^{-1}M_{\geq n})$ trên $S^{-1}M$ là tốt đối với iđêan $S^{-1}H_{\geq 1}$ của $S^{-1}H$.

Ta có, với $n \geq n_0$, $M_{\geq n+1} = H_1 \cdot M_{\geq n}$, do đó $S^{-1}M_{\geq n+1} = H_1 \cdot S^{-1}M_{\geq n} = S^{-1}H_{\geq 1} \cdot S^{-1}M_{\geq n}$.

#### Mệnh đề 4 {#ac-viii-s6-prop-4 .statement}

Giả sử rằng $H$ là Noether và $M$ sinh hữu hạn. Khi đó $\dim_H(M) = \dim_{S^{-1}H}(S^{-1}M)$.

Cho a là linh hóa tử của $H$-môđun $M$; đó là một iđêan phân bậc của $H$. Vì $M$ là một $H$-môđun sinh hữu hạn, linh hóa tử của $S^{-1}H$-môđun $S^{-1}M$ là iđêan $S^{-1}\alpha$ của $S^{-1}H$. Ta có $\dim_H(M) = \dim(H/\alpha)$ và $\dim_{S^{-1}H}(S^{-1}M) = \dim(S^{-1}H/S^{-1}\alpha)$. Mệnh đề 4 suy ra từ Định lý 1, c) của No. 2 áp dụng cho vành phân bậc $H/\alpha$.

#### Mệnh đề 5 {#ac-viii-s6-prop-5 .statement}

Giả sử $H_0$ địa phương và Artin, $H$ được sinh bởi $H_0 \cup H_1$, $H_1$ là một $H_0$-môđun hữu hạn sinh, $M$ khác không và là một $H$-môđun hữu hạn sinh. Khi đó $M_n$ là một $H_0$-môđun có độ dài hữu hạn với mỗi $n$, và tồn tại $Q(T) \in \mathbf{Z}[T, T^{-1}]$ sao cho $Q(1) > 0$ và ta có trong vành $\mathbf{Z}((T))$

$$
\sum_{n \in \mathbf{Z}} \operatorname{long}_{H_0}(M_n) \cdot T^n = (1 - T)^{-d} \cdot Q(T),
$$

trong đó $d = \dim_H(M)$.

Vành $S^{-1}H$ là địa phương và Noether (No. 1, nhận xét 1), $S^{-1}H$-môđun $S^{-1}M$ là khác không và hữu hạn sinh, và có chiều $d = \dim_H(M)$ (mệnh đề 4). Hơn nữa, $S^{-1}H_{\geq 1}$ là một iđêan định nghĩa của $S^{-1}H$ (§ 3, No. 2, bổ đề 2), và $S^{-1}M_{\geq n}$ là một lọc tốt bởi $S^{-1}H_{\geq 1}$ trên $S^{-1}M$ (bổ đề 3). Cuối cùng, ta có $\operatorname{long}_{S^{-1}H} S^{-1}M_{\geq n}/S^{-1}M_{\geq n+1} = \operatorname{long}_{H_0}(M_n)$ với mọi $n$. Do đó chỉ cần áp dụng các Định lý 2 và 3 của § 4 (No. 3 và 4).

#### Nhận xét {#ac-viii-s6-n3-rem-1 .statement}

Ngoại trừ việc xác định số nguyên $d$, mệnh đề 5 suy ra trực tiếp từ Định lý 1 của § 4, No. 2.

#### Hệ quả {#ac-viii-s6-n3-cor-1 .statement}

Cho $A$ là một vành địa phương Noether và $q$ là một iđêan định nghĩa của $A$. Khi đó ta có $\dim(A) = \dim(\operatorname{gr}_q(A))$.

Áp dụng mệnh đề 5 vào trường hợp $M = H = \operatorname{gr}_q(A)$, ta thu được quan hệ

$$
\sum_{n \geq 0} \operatorname{long}_{A/q}(q^n/q^{n+1}) \cdot T^n = (1 - T)^{-d} Q(T)
$$

với $d = \dim(\operatorname{gr}_q(A))$ và $Q(1) \neq 0$. Ta có $d = \dim(A)$ theo Định lý 3 của § 4, No. 4, do đó có hệ quả.

#### Mệnh đề 6 {#ac-viii-s6-prop-6 .statement}

Giả sử $H_0$ địa phương và Artin, $H$ sinh hữu hạn như một $H_0$-đại số và $M$ sinh hữu hạn như một $H$-môđun.

a) Cho $a_1, ..., a_n$ là các phần tử của $H$, thuần nhất với các bậc $> 0$, và cho $\varphi$ là đồng cấu (của các $H_0$-đại số) từ $H_0[X_1, ..., X_n]$ vào $H$ ánh xạ $X_i$ thành $a_i$ với $1 \leq i \leq n$. $S^{-1}H$-môđun $S^{-1}M / \sum_{i=1}^n (a_i/1).S^{-1}M$ có độ dài hữu hạn khi và chỉ khi $\varphi_*(M)$ là một môđun sinh hữu hạn trên $H_0[X_1, ..., X_n]$.

b) Tồn tại một họ $(a_1, ..., a_d)$ các phần tử của $H$, tất cả thuần nhất cùng một bậc $> 0$, với $d = \dim_H(M)$, và sao cho $(a_1/1, ..., a_d/1)$ là một dãy cát tuyến cực đại đối với $S^{-1}H$-môđun $S^{-1}M$. Hơn nữa, nếu $H$ được sinh bởi $H_1$ như một $H_0$-đại số, và nếu trường thặng dư của $H_0$ là vô hạn, thì có thể chọn các $a_i$ có bậc 1.

a) Đặt $N = M / \sum_{i=1}^n a_i M$. Ta có $\dim_H(N) = \dim_{S^{-1}H}(S^{-1}N)$ theo mệnh đề 4. Do đó, $S^{-1}H$-môđun $S^{-1}N$ có độ dài hữu hạn khi và chỉ khi $H$-môđun $N$ có độ dài hữu hạn, nghĩa là khi và chỉ khi $N$ là một môđun sinh hữu hạn trên $H_0$. Nếu $\varphi_*(M)$ là môđun trên $H_0[X_1, ..., X_n]$ suy ra từ $M$ bởi đồng cấu $\varphi : H_0[X_1, ..., X_n] \to M$, ta có $N = \varphi_*(M)/\sum_{i=1}^n X_i \cdot \varphi_*(M)$. Do đó (A, II, p. 171, hệ quả 3 và nhận xét) $\varphi_*(M)$ là một môđun sinh hữu hạn trên $H_0[X_1, ..., X_n]$ khi và chỉ khi $N$ là một môđun sinh hữu hạn trên $H_0$. Điều này chứng minh a).

Để chứng minh b), trước hết ta sẽ thiết lập một bổ đề.

#### Bổ đề 4 {#ac-viii-s6-lem-4 .statement}

Cho $b$ là một phần tử của $H$, thuần nhất có bậc $> 0$, và thuộc không một phần tử cực tiểu $p$ nào của $\mathrm{Supp}(M)$ sao cho $\dim(H/p) = \dim_H(M)$. Khi đó $\dim_H(M/bM) = \dim_H(M) - 1$.

Đặt $d = \dim_H(M)$. Theo định nghĩa của $b$, ta có $\dim_H(M/bM) < d$. Theo mệnh đề 4, ta có
$$
\dim_H(M/bM) = \dim_{S^{-1}H}(S^{-1}M/(b/1).S^{-1}M)
$$
và công thức (8) của § 3, no. 2 cho bất đẳng thức
$$
\dim_{S^{-1}H}(S^{-1}M/(b/1).S^{-1}M) \geq \dim_{S^{-1}H}(S^{-1}M) - 1 .
$$
Cuối cùng, ta có
$$
\dim_{S^{-1}H}(S^{-1}M) = \dim_H(M) = d
$$
theo mệnh đề 4. Do đó $\dim_H(M/bM) \geq d - 1$, từ đó suy ra bổ đề 4.

Ta tiếp tục lại chứng minh của Mệnh đề 6, b). Ta có thể giả sử $\dim_H(M) > 0$. Ta nhận xét rằng mọi phần tử cực tiểu của $\mathrm{Supp}(M)$ đều phân bậc (áp dụng Bổ đề 1 của No. 2 cho môđun thương của $H$ bởi linh hóa tử của $M$). Theo Mệnh đề 8 của III, § 1, No. 4, do đó tồn tại một phần tử thuần nhất $b$ của $H$, có bậc $> 0$, không thuộc bất kỳ phần tử cực tiểu $p$ nào của $\mathrm{Supp}(M)$ sao cho $\dim(H/p) = \dim_H(M)$. Theo Bổ đề 4, ta có $\dim_H(M/bM) = \dim_H(M) - 1$. Giả sử thêm rằng $H$ được sinh bởi $H_1$ như một $H_0$-đại số và rằng trường thặng dư $k$ của $H_0$ là vô hạn. Với mỗi phần tử cực tiểu $p$ của $\mathrm{Supp}(M)$ sao cho $\dim(H/p) = \dim_H(M)$, xét không gian con vectơ $V_p = (p \cap H_1) \otimes_{H_0} k$ của không gian vectơ $V = H_1 \otimes_{H_0} k$ trên $k$. Nếu có $V_p = V$, thì ta có $\mathfrak{p} \cap H_1 = H_1$ (II, § 3, No. 2, Mệnh đề 4), do đó $H_1 \subset \mathfrak{p}$ và $\dim_H(M) = \dim(H/\mathfrak{p}) \leq \dim(H/H_{\geq 1}) = 0$, điều này không đúng. Vì $k$ được giả sử là vô hạn, hợp của các $V_p$ khác $V$; nếu $b \in H_1$ sao cho $b \otimes 1$ không thuộc bất kỳ $V_p$ nào, thì ta có $\dim(M/bM) = \dim_H(M) - 1$.

Tiến hành quy nạp theo $d = \dim_H(M)$, khi đó ta xây dựng một dãy $(b_1, ..., b_d)$ các phần tử của $H$, với $b_i$ thuần nhất có bậc $n_i > 0$ và sao cho $M / \sum_{i=1}^n b_i M$ là một $H$-môđun có độ dài hữu hạn. Nếu giả sử rằng $H$ được sinh bởi $H_1$ như một $H_0$-đại số và trường thặng dư của $H_0$ là vô hạn, ta có thể giả sử $n_i = 1$ với $i = 1, ..., d$. Theo Mệnh đề 4, ta có $\dim_{S^{-1}H}(S^{-1}M) = d$ và
$$
\dim_{S^{-1}H}(S^{-1}M / \sum_{i=1}^d (b_i/1).S^{-1}M) = 0 .
$$
Khi đó $(b_1/1, ..., b_d/1)$ là một dãy cắt cực đại cho $S^{-1}H$-môđun $S^{-1}M$. Đặt $a_i = b_i^{(n_1 ... n_d)/n_i}$ với $1 \leq i \leq d$; khi đó các $a_i$ đều có cùng một bậc, và $(a_1/1, ..., a_d/1)$ là một dãy cắt cực đại cho $S^{-1}M$ (§ 3, No. 2, Nhận xét 3).

#### Hệ quả 1 {#ac-viii-s6-lem-4-cor-1 .statement}

*Giả sử $H_0$ là một trường và $H$ là một đại số trên $H_0$ sinh hữu hạn. Đặt $n = \dim(H)$. Tồn tại các phần tử thuần nhất $a_1, ..., a_n$ của $H$, tất cả cùng bậc $> 0$, sao cho đồng cấu $H_0$-đại số $\varphi : H_0[X_1, ..., X_n] \to H$ xác định bởi $\varphi(X_i) = a_i, i = 1, ..., n$, là đơn ánh và biến $H$ thành một đại số hữu hạn trên $H_0[X_1, ..., X_n]$. Nếu $H$ được sinh bởi $H_1$ như một đại số trên $H_0$ và nếu $H_0$ là vô hạn, có thể giả sử các $a_i$ có bậc 1.*

Theo Mệnh đề 6 tồn tại một đồng cấu $H_0$-đại số $\varphi$ có dạng đã chỉ ra, biến $H$ thành một đại số hữu hạn trên $H_0[X_1, ..., X_n]$. Theo Định lý 1 của § 2, No. 3, khi đó ta có
$$
\dim(H_0[X_1, ..., X_n]/(\mathrm{Ker}\ \varphi)) = \dim(H);
$$
vì ta có
$$
\dim(H) = n = \dim(H_0[X_1, ..., X_n]),
$$
và vì $H_0[X_1, ..., X_n]$ là một miền nguyên, điều này suy ra $\mathrm{Ker}\ \varphi = \{0\}$.

#### Nhận xét {#ac-viii-s6-n3-rem-2 .statement}

Cho $(h_1, ..., h_r)$ là một hệ sinh hữu hạn của không gian vectơ $H_1$ trên $H_0$. Với $\lambda = (\lambda_1, ..., \lambda_r) \in H_0^r$, đặt $h_\lambda = \lambda_1 h_1 + \cdots + \lambda_r h_r$. Các chứng minh của Mệnh đề 6 và Hệ quả 1 kéo theo kết quả sau: tập hợp các phần tử $(\lambda_1, ..., \lambda_n)$ của $(H_0^r)^n$ sao cho các phần tử $a_i = h_{\lambda_i} \in H_1$ thỏa mãn kết luận của Hệ quả 1 chứa phần bù của hợp của một số hữu hạn các không gian vectơ con của $(H_0^r)^n$ khác với toàn bộ không gian.

#### Hệ quả 2 {#ac-viii-s6-lem-4-cor-2 .statement}

*Cho $A$ là một vành địa phương Noether và $n \in \mathbf{N}$. Để có $\dim(A) \geq n$, điều kiện cần và đủ là với mọi số nguyên $r \geq 0$, ta có*
$$
[m_A^r/m_A^{r+1} : \kappa_A] \geq \binom{n+r-1}{n-1}, \quad \left( \text{resp. } \mathrm{long}_A(A/m_A^{r+1}) \geq \binom{n+r}{n} \right);
$$
*ta có đẳng thức với mọi $r$ khi và chỉ khi $A$ là chính quy có chiều $n$.*

Điều kiện là đủ (§ 4, No. 4, Định lý 3 và § 5, No. 2, Định lý 1). Ta hãy chứng minh rằng nó là cần. Xét vành phân bậc gr(A) = gr_{m_A}(A); cho $k$ là một mở rộng vô hạn của trường $\kappa_A$, và đặt $H = k \otimes_{\kappa_A} \mathrm{gr}(A)$. Vành H có chiều $\geq n$ (Mệnh đề 5 và hệ quả của nó); do đó suy ra từ Hệ quả 1 sự tồn tại của một đồng cấu phân bậc đơn ánh của các đại số phân bậc trên k $\varphi : H_0[X_1, ..., X_n] \to H$. Do đó ta có, với mọi số nguyên $r \geq 0$,

$$
[\mathrm{gr}_r(A) : \kappa_A] = [H_r : H_0] \geq \binom{n + r - 1}{n - 1},
$$

và đẳng thức với mọi $r$ suy ra tính song ánh của $\varphi$, do đó tính chính quy của A (§ 5, No. 2, Định lý 1).

Các đẳng thức

$$
\mathrm{long}_A(A/m_A^{r+1}) = \sum_{i=0}^r [\mathrm{gr}_i(A) : \kappa_A]
$$

và

$$
\binom{n + r}{n} = \sum_{i=0}^r \binom{n + i - 1}{n - 1}
$$

sau đó suy ra các khẳng định tương tự đối với hàm $r \mapsto \mathrm{long}_A(A/m_A^{r+1})$.

### 4. Tính nửa liên tục của chiều

#### Bổ đề 5 {#ac-viii-s6-lem-5 .statement}

Cho A là một vành, r là căn của nó, $R = \bigoplus_{i \in \mathbf{Z}} R_i$ là một đại số phân bậc trên A, $M = \bigoplus_{i \in \mathbf{Z}} M_i$ là một môđun R phân bậc. Giả sử rằng mỗi $M_i$ là một A-môđun sinh hữu hạn và rằng $M/rM$ là một $R/rR$-môđun sinh hữu hạn. Khi đó M là một môđun R sinh hữu hạn.

Cho $m_1, ..., m_n$ là các phần tử thuần nhất của M mà các ảnh của chúng trong $M/rM$ sinh môđun $R/rR$-môđun $M/rM$. Cho N là môđun con $R$ (phân bậc) của M được sinh bởi $\{ m_1, ..., m_n \}$. Với mọi $i \in \mathbf{Z}$, ta có $M_i = N_i + rM_i$, do đó $M_i = N_i$ (II, § 3, No. 2, Prop. 4); do đó ta có $M = N$.

#### Bổ đề 6 {#ac-viii-s6-lem-6 .statement}

Cho $\rho : B \to C$ là một đồng cấu và S là một tập con nhân của B. Giả sử rằng C là một B-đại số kiểu hữu hạn, và rằng $S^{-1}C$ là một $S^{-1}B$-đại số hữu hạn. Khi đó tồn tại $f \in S$ sao cho $C_f$ là một $B_f$-đại số hữu hạn.

Cho X là một tập sinh hữu hạn của B-đại số C. Với mọi $x \in X$, ảnh của x trong $S^{-1}C$ là nguyên trên $S^{-1}B$, và do đó tồn tại một số nguyên $n(x) \geq 0$, các phần tử $b_1(x), ..., b_{n(x)}(x) \in B$ và một phần tử $f(x) \in S$ sao cho

$$
f(x)\ x^{n(x)} + b_1(x)\ x^{n(x)-1} + \cdots + b_{n(x)} = 0.
$$

Cho $f = \prod_{x \in X} f(x)$; ảnh của mọi phần tử x của X trong $C_f$ là nguyên trên $B_f$, do đó $C_f$ là một $B_f$-đại số hữu hạn (V, § 1, No. 1, Prop. 4).

#### Mệnh đề 7 {#ac-viii-s6-prop-7 .statement}

Giả sử rằng H là một $H_0$-đại số kiểu hữu hạn. Khi đó hàm $p \mapsto \dim(H \otimes_{H_0} \kappa(p))$ là nửa liên tục trên trên $\mathrm{Spec}(H_0)$.

Vì H là một đại số trên $H_0$ sinh hữu hạn, mỗi $H_i$ là một $H_0$-môđun sinh hữu hạn (III, § 1, No. 2, hệ quả của Mệnh đề 1) và H được sinh như một đại số trên $H_0$ bởi $H_0 \oplus H_1 \oplus \cdots \oplus H_r$ với một số nguyên $r \geq 0$ thích hợp. Cho $p \in \mathrm{Spec}(H_0)$ và đặt $\dim(H \otimes_{H_0} \kappa(p)) = n \geq 0$. Theo Hệ quả 1 của Mệnh đề 6, tồn tại các phần tử $a_1, ..., a_n$ của H, tất cả thuần nhất cùng bậc $d > 0$, sao cho đồng cấu $\kappa(p)$ $\overline{\varphi} : \kappa(p)[X_1, ..., X_n] \to H \otimes_{H_0} \kappa(p)$ ánh xạ $X_i$ vào $a_i \otimes 1$ với $1 \leq i \leq n$, biến $H \otimes_{H_0} \kappa(p)$ thành một đại số hữu hạn trên $\kappa(p)[X_1, ..., X_n]$. Ký hiệu $\varphi$ là đồng cấu $H_0$ của $H_0[X_1, ..., X_n] = R$ vào H ánh xạ $X_i$ vào $a_i$ với $1 \leq i \leq n$. Nếu, với mọi $m \in \mathbf{Z}$, ta đặt $H'_m = \sum_{(m-1)d < i \leq md} H_i$, ta thu được một phân bậc $\mathbf{Z}$ trên H, tương thích với cấu trúc môđun trên R được cho bởi $\varphi$. Mỗi $H'_m$ là sinh hữu hạn trên $H_0$. Theo Bổ đề 5, $H_p$ là một $R_p$-môđun sinh hữu hạn. Theo Bổ đề 6, do đó tồn tại $f \in H_0 - p$ sao cho $H_f$ là một $R_f$-môđun sinh hữu hạn. Với mọi $q \in \mathrm{Spec}(H_0)_f$, $H \otimes_{H_0} \kappa(q)$ là một đại số hữu hạn trên $\kappa(q)[X_1, ..., X_n]$, do đó $\dim(H \otimes_{H_0} \kappa(q)) \leq n$ (§ 2, No. 3, Định lý 1), điều này hoàn thành chứng minh.

#### Nhận xét 1 {#ac-viii-s6-n4-rem-1 .statement}

\* Trong hình học đại số, Mệnh đề 7 kéo theo rằng chiều của các thớ của một cấu xạ xạ ảnh của các đa tạp đại số là nửa liên tục trên. \*
2) Ta sẽ thấy sau này rằng nếu $\rho : A \to B$ là một đồng cấu vành biến B thành một đại số trên A sinh hữu hạn, thì hàm $q \mapsto \dim_q(B \otimes_A \kappa(\rho^{-1}(q)))$ là nửa liên tục trên trên $\mathrm{Spec}(B)$ (xem p. 101, Bài tập 10).

### 5. Các đại số phân bậc chính quy

Trong số này, giả sử rằng $H_0$ là một trường và H là một đại số trên $H_0$ sinh hữu hạn.

Ta đặt $H_+ = H_{\geq 1}$; nó là một iđêan cực đại của H. Vành $S^{-1}H$ được đồng nhất với vành địa phương $H_{H_+}$ của H tại iđêan $H_+$; iđêan cực đại của nó là $(H_+ )_{H_+} = S^{-1}H_+$, trường thặng dư của nó được đồng nhất với $H_0$.

#### Mệnh đề 8 {#ac-viii-s6-prop-8 .statement}

a) Ta có $\dim(H) \leq [H_+/H_+^2 : H_0]$.
b) Các điều kiện sau là tương đương:
(i) $\dim(H) = [H_+/H_+^2 : H_0]$;
(ii) vành địa phương Noether $S^{-1}H$ là chính quy;
(iii) $H$ được sinh như một đại số $H_0$ bởi một họ các phần tử thuần nhất có các bậc $> 0$, độc lập đại số trên $H_0$.
c) Giả sử các điều kiện của b) được thỏa mãn, và cho $a_1, ..., a_n \in H$ là các phần tử thuần nhất có các bậc $> 0$. Các điều kiện sau là tương đương:
(i) các lớp của $a_i$ tạo thành một cơ sở của không gian vectơ $H_0$- $H_+/H_+^2$;
(ii) $a_i/1$ tạo thành một hệ tọa độ của vành địa phương Noether chính quy $S^{-1}H$;

(iii) các $a_i$ độc lập đại số trên $H_0$ và sinh $H$ như một đại số $H_0$.

Ta có $\dim(H) = \dim(S^{-1}H)$ (No. 2, đl. 1), và $[H_+/H_+^2 : H_0] = [(S^{-1}H_+)/ (S^{-1}H_+)^2 : H_0]$ (II, § 3, No. 3, mđ. 9); sau § 5, No. 1, điều này suy ra a) và các tương đương (i) $\Leftrightarrow$ (ii) trong $b$ và $c$. Hai kéo theo (iii) $\Rightarrow$ (i) trong $b$ và $c$ là tầm thường. Ta chứng minh các kéo theo (i) $\Rightarrow$ (iii). Do đó giả sử rằng ta có $\dim(H) = [H_+/H_+^2 : H_0]$ và cho $a_1, ..., a_n$ là các phần tử thuần nhất của $H$, có các bậc $> 0$, mà các lớp của chúng tạo thành một cơ sở của $H_+/H_+^2$; xét đồng cấu của các đại số phân bậc $\varphi : H_0[X_1, ..., X_n] \to H$ gửi $X_i$ vào $a_i$. Iđêan $H_+$ của $H$ được sinh bởi các $a_i$ (A, II, p. 171, hq. 2 và nhận xét); do đó đồng cấu $\varphi$ là toàn ánh (III, § 1, No. 2, mđ. 1). Nhưng ta có

$$
\dim(H_0[X_1, ..., X_n]) = n = \dim(H) = \dim(H_0[X_1, ..., X_n]/(\mathrm{Ker}\, \varphi))
$$

(§ 2, No. 4, hq. 1 của đl. 3), do đó $\mathrm{Ker}\, \varphi = 0$ vì $H_0[X_1, ..., X_n]$ là một miền nguyên. Điều này suy ra các khẳng định (iii).

Dưới các giả thiết của $b$, người ta nói rằng $H$ là một đại số $H_0$-phân bậc chính quy, hoặc một đại số $H_0$-phân bậc đa thức. Dưới các giả thiết của $c$, người ta nói rằng các $a_i$ tạo thành một hệ tọa độ phân bậc của $H$.

#### Nhận xét 1 {#ac-viii-s6-n5-rem-1 .statement}

Với ký hiệu của $c$, gọi $d_i$ là bậc của $a_i$ ($1 \leq i \leq n$). Khi đó chuỗi Poincaré $P_H = \sum_{n \in \mathbf{Z}} [H_n : H_0]. T^n$ bằng $\prod_i (1 - T^{d_i})^{-1}$ (§ 4, No. 2, ví dụ 1).
Do đó, nếu $H$ là một đại số $H_0$-phân bậc đa thức, ta có

$$
P_H = \prod_n (1 - T^n)^{-\delta(n)}, \quad \text{với} \quad \delta(n) = [(H_+/H_+^2)_n : H_0].
$$

#### Nhận xét 2 {#ac-viii-s6-n5-rem-2 .statement}

Ngược lại, việc tồn tại các số nguyên $d_i > 0$ sao cho $P_H = \prod_i (1 - T^{d_i})^{-1}$ không kéo theo rằng $H$ là một đại số đa thức phân bậc; chẳng hạn, nếu $H$ được sinh bởi một phần tử $X$ có bậc 1 và một phần tử $Y$ có bậc 2, chỉ với quan hệ $X^2 = 0$, thì ta có $P_H = (1 - T)^{-1}$.

## BÀI TẬP {#ac-viii-s6-exercises}

Xem các [bài tập cho § 6](exercises/s6/).
