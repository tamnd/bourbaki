---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 7
section_title: Multiplicités
lang: vi
source: ac-viii-ix-fr
book_pages: AC VIII.71-AC VIII.81, AC VIII.103-AC VIII.108
pdf_pages: 0075-0085, 0107-0112
extraction: ocr
subsections:
    - "no": 1
      title: Multiplicité d’un module relativement à un idéal
      page: 71
      pdf_page: 75
    - "no": 2
      title: Multiplicités et extensions plates
      page: 0
      pdf_page: 77
    - "no": 3
      title: Multiplicités et extensions finies
      page: 74
      pdf_page: 78
    - "no": 4
      title: Multiplicités et suites sécantes
      page: 76
      pdf_page: 80
    - "no": 5
      title: Éléments superficiels
      page: 0
      pdf_page: 81
statements: 28
exercises: 25
content_sha256: 1eeb40001454ae2978561f7815b344e207290528b5db31569553f99dc344df0b
translated_from: content/en-mt/ac/VIII/07_s7_multiplicites.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 68115c9d8bf4b1a2b06c471d9339d5bb6256d795fcf17a9f580d192667524606
translation_model: gpt-5.4
translation_run: translate-vi-e477d8c2
glossary_version: 34
glossary_terms_sha256: 499a21694782e0ea4064fe4262bff73fec64b0890530edafa6203a77a4ffc2d4
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 7. BỘI SỐ

Trong suốt đoạn này, $A$ ký hiệu một vành Noether.

### 1. Bội số của một môđun đối với một iđêan

Cho $M$ là một A-môđun hữu hạn sinh và $q$ là một iđêan của $A$ được chứa trong căn của $A$ và sao cho $M/qM$ có độ dài hữu hạn. Giả sử rằng $M$ không quy về 0 và đặt $d = \dim_A(M)$. Theo § 4, No. 3, hệ quả của th. 2 và No. 4, nhận xét 2, tồn tại một số nguyên duy nhất $e_q(M) > 0$ sao cho, với mọi số nguyên $n \geqslant 1$

$$
\operatorname{long}_A(M/q^{n+1}M) = e_q(M) \frac{n^d}{d!} + \beta_n n^{d-1}
$$

trong đó $\beta_n$ tiến tới một giới hạn khi $n$ tăng vô hạn.

#### Định nghĩa 1 {#ac-viii-s7-def-1 .statement}

Số nguyên $e_q(M)$ được gọi là bội số của A-môđun M đối với iđêan q.

Nó cũng được ký hiệu bởi $e_q^A(M)$ khi muốn nhắc đến vành A. Khi A là địa phương với iđêan cực đại m, người ta viết $e(M)$ hoặc $e^A(M)$ thay cho $e_m(M)$ hoặc $e_m^A(M)$.

#### Nhận xét 1 {#ac-viii-s7-n1-rem-1 .statement}

Nếu q’ là một iđêan của A được chứa trong căn của A và chứa q, thì ta có $e_{q'}(M) \leqslant e_q(M)$ và, nếu lọc q’-adic của M là q-tốt, thì ta có $e_{q'}(M) = e_q(M)$ (§ 4, No. 3, th. 2).
2) Nếu M có độ dài hữu hạn, thì ta có $e_q(M) = \operatorname{long}_A(M)$ (§ 4, No. 3, nhận xét 3).
3) Nếu $d > 0$, thì ta có

$$
\operatorname{long}_{A/q}(q^nM/q^{n+1}M) = e_q(M) \frac{n^{d-1}}{(d-1)!} + \alpha_n n^{d-2}
$$

trong đó $\alpha_n$ tiến tới một giới hạn khi $n$ tăng vô hạn (§ 4, No. 3, hệ quả của th. 2).
4) Việc tính các bội số có thể được quy về trường hợp A là địa phương vì, theo § 4, No. 4, hệ quả của th. 3, ta có

$$
e_q(M) = \sum e_{q_m}(M_m)
$$

trong đó phép lấy tổng mở rộng trên các iđêan cực đại m của A sao cho

$$
m \in \operatorname{Supp}(M) \cap V(q) \quad \text{và} \quad \dim_{A_m}(M_m) = d .
$$

Từ các nhận xét 2 và 3 suy ra rằng $e_q(M)$ chỉ phụ thuộc vào A/q-môđun phân bậc $\operatorname{gr}_q(M)$. Do đó:

#### Mệnh đề 1 {#ac-viii-s7-prop-1 .statement}

Cho $\hat{A}$ và $\hat{M}$ là các hoàn thành của A và M đối với các tôpô q-adic của chúng; khi đó $e_q^A(M) = e_{q\hat{A}}(\hat{M})$.

#### Mệnh đề 2 {#ac-viii-s7-prop-2 .statement}

Giả sử rằng A là địa phương chính quy (§ 5, No. 1, def. 1); ta có $e(A) = 1$.
Điều này suy ra từ th. 1 của § 5, No. 2.

#### Nhận xét 5 {#ac-viii-s7-n1-rem-5 .statement}

Có thể xảy ra trường hợp $e(A) = 1$ mà A không chính quy (p. 104, exerc. 5). Thực vậy, một vành địa phương Noether A là chính quy khi và chỉ khi $\hat{A}$ là nguyên và ta có $e(A) = 1$ (p. 108, exerc. 24).

#### Ví dụ {#ac-viii-s7-n1-exa-1 .statement}

Theo định nghĩa ta có $e_{q,r}(M) = r^d e_q(M)$ trong đó $d = \dim_A(M)$. Do đó, nếu A là địa phương chính quy, thì ta có $e_{m_A^r}(A) = r^d$. Ví dụ, nếu A là một vành định giá rời rạc, thì ta có $e_q(A) = \operatorname{long}(A/q)$.

#### Mệnh đề 3 {#ac-viii-s7-prop-3 .statement}

*Cho M là một A-môđun hữu hạn sinh, có chiều d ≥ 0. Cho Φ là tập hợp các phần tử cực tiểu p của Supp(M) sao cho dim(A/p) = d. Cho q là một iđêan của A, được chứa trong căn của A, và sao cho M/qM có độ dài hữu hạn. Ta có*

$$
e_q(M) = \sum_{p \in \Phi} \operatorname{long}_{A_p}(M_p).e_q(A/p).
$$

#### Hệ quả {#ac-viii-s7-n1-cor-1 .statement}

*Giả sử A là nửa địa phương và cho q là một iđêan định nghĩa của A.
a) Ta có $e_q(A) = \sum_p e_q(A/p)$, trong đó p chạy qua tập hợp các iđêan nguyên tố cực tiểu của A sao cho $\dim(A/p) = \dim(A)$.
b) Giả sử A nguyên và cho M là một A-môđun hữu hạn sinh sao cho $\dim_A(M) = \dim(A)$. Khi đó ta có $e_q(M) = \operatorname{rg}(M).e_q(A)$.*

### 2. Bội số và các mở rộng phẳng

#### Mệnh đề 4 {#ac-viii-s7-prop-4 .statement}

*Cho ρ : A → B là một đồng cấu địa phương của các vành địa phương Noether, và cho N là một B-môđun hữu hạn sinh, phẳng trên A, và sao cho N ⊗_A κ_A là một B-môđun có độ dài hữu hạn. Nếu M là một A-môđun hữu hạn sinh khác không và q là một iđêan của A khác A và sao cho M/qM có độ dài hữu hạn, thì (M ⊗_A N)/(qB)(M ⊗_A N) là một B-môđun có độ dài hữu hạn, và ta có*

$$
e_{q_B}^B(M ⊗_A N) = \operatorname{long}_B(N ⊗_A κ_A).e_q^A(M).
$$

Cho L là một A-môđun có độ dài hữu hạn r. Khi đó L có một dãy Jordan-Hölder độ dài r, với các thương đẳng cấu với κ_A; vì N phẳng trên A, B-môđun L ⊗_A N có một dãy hợp thành độ dài r, với các thương đẳng cấu với N ⊗_A κ_A, do đó có độ dài $r \cdot \operatorname{long}_B(N \otimes_A \kappa_A)$. Vì B-môđun (M ⊗_A N)/(qB)^n(M ⊗_A N) đẳng cấu với (M/q^nM) ⊗_A N với mọi $n \in \mathbf{N}$, mệnh đề suy ra từ định nghĩa các bội số.

#### Hệ quả {#ac-viii-s7-n2-cor-1 .statement}

*Giả sử rằng B phẳng trên A và ρ(m_A) B = m_B. Khi đó*

$$
e_{q_B}^B(M ⊗_A B) = e_q^A(M).
$$

Điều này áp dụng đặc biệt khi B là hoàn thành \* hoặc Hensel hoá \* của A đối với một iđêan khác A, \* hoặc một phép nổ của A, chẳng hạn một Hensel hoá ngặt của A. \*

#### Ví dụ {#ac-viii-s7-n2-exa-1 .statement}

\* Cho X là một đa tạp đại số phức, $\mathcal{O}_{X,x}$ là vành địa phương của X tại một điểm hữu tỉ x, $X^{an}$ là không gian giải tích liên kết với X; lại ký hiệu bởi x điểm của $X^{an}$ tương ứng với x, và cho $\mathcal{O}_{X^{an},x}$ là vành địa phương của $X^{an}$ tại x. Khi đó $e(\mathcal{O}_{X^{an},x}) = e(\mathcal{O}_{X,x})$. \*

### 3. Bội số và các mở rộng hữu hạn

#### Mệnh đề 5 {#ac-viii-s7-prop-5 .statement}

Giả sử A là nửa địa phương, và gọi $\rho : A \to B$ là một đồng cấu vành làm cho B là một A-môđun hữu hạn sinh. Gọi N là một B-môđun hữu hạn sinh khác không, và q là một iđêan của A được chứa trong căn của A, sao cho $N/qN$ có độ dài hữu hạn. Trong các iđêan cực đại của B (hữu hạn về số lượng, theo IV, § 2, No. 5, hệ quả 3 của mệnh đề 9), ký hiệu bởi $m_1, ..., m_r$ những iđêan mà đối với chúng ta có $\dim_{B_{m_i}}(N_{m_i}) = \dim_B(N)$. Đặt $B_i = B_{m_i}$ và $q_i = qB_i$ với $1 \leq i \leq r$. Khi đó ta có các đẳng thức

$$
\dim_A(N) = \dim_B(N),
$$
$$
e_{qB}^B(N) = \sum_{i=1}^r e_{q_i}^{B_i}(N_{m_i}),
$$
$$
e_q^A(N) = \sum_{i=1}^r [B/m_i : A/\rho^{-1}(m_i)]\ e_{q_i}^{B_i}(N_{m_i}).
$$

Đẳng thức thứ nhất suy ra từ § 2, No. 3, định lý 1, c); đẳng thức thứ hai suy ra từ Nhận xét 4 của No. 1 (chú ý rằng $m_i$ thuộc $V(qB)$ với $1 \leq i \leq r$ vì $\rho^{-1}(m_i) \supset q$ theo V, § 2, No. 1, mệnh đề 1). Ta hãy chứng minh đẳng thức thứ ba. Gọi E là một B-môđun có độ dài hữu hạn; ta có

$$
\operatorname{long}_A(E) = \sum_m [B/m : A/\rho^{-1}(m)].\operatorname{long}_{B_m}(E_m),
$$

trong đó $m$ chạy trên tập hợp các iđêan cực đại của B; điều này thực ra là hiển nhiên khi E là một trong các $B/m$, và trường hợp tổng quát suy ra từ đó, vì E có một chuỗi hợp thành mà các thương của nó đẳng cấu với $B/m$. Áp dụng công thức này cho các B-môđun $N/q^{n+1}N$, ta suy ra đẳng thức cần chứng minh theo định nghĩa của các bội số.

#### Hệ quả {#ac-viii-s7-n3-cor-1 .statement}

Nếu $[B/m_i : A/\rho^{-1}(m_i)] = 1$ với mọi i, ta có $e_q^A(N) = e_{qB}^B(N)$.

#### Bổ đề 1 {#ac-viii-s7-lem-1 .statement}

Gọi $\rho : A \to B$ là một đồng cấu vành, và gọi $p$ là một iđêan nguyên tố của A. Xét hai tính chất sau:
(i) đồng cấu chính tắc $\tilde{\rho}$ từ $A_p$ vào $A_p \otimes_A B$ là song ánh;
(ii) tồn tại duy nhất một iđêan nguyên tố $r$ của B nằm trên $p$ và đồng cấu chính tắc $\rho_p$ từ $A_p$ vào $B_r$ là song ánh.
Ta có (i) $\Rightarrow$ (ii). Nếu $p$ là cực tiểu, hoặc nếu B là nguyên trên A, ta có (i) $\Leftrightarrow$ (ii) $^1$.

1 Bổ đề này vẫn đúng khi vành A không Noether.

Vành $A_p \otimes_A B$ được đồng nhất với vành phân thức $S^{-1}B$ của $B$ được xác định bởi tập hợp nhân $S = \rho(A - p)$ của $B$. Do đó các iđêan nguyên tố của $S^{-1}B$ là các $S^{-1}q$, trong đó $q$ là một iđêan nguyên tố của $B$ sao cho $\rho^{-1}(q) \subset p$; nếu $q$ là một iđêan như vậy, thì $(S^{-1}B)_{S^{-1}q}$ được đồng nhất với $B_q$ (II, § 2, No. 5, mệnh đề 11).

Nếu điều kiện (i) được thỏa mãn, thì tồn tại (V, § 2, No. 1, Bổ đề 1) một iđêan nguyên tố duy nhất $r$ của $B$ sao cho $\rho^{-1}(r) = p$. Hơn nữa, $B_r$ được đồng nhất với vành phân thức $(S^{-1}B)_{S^{-1}r}$, nên cũng được đồng nhất với $(A_p)_s$, trong đó $s$ là ảnh ngược của $S^{-1}r$ bởi đẳng cấu $\tilde{\rho}: A_p \to S^{-1}B$; bây giờ $\tilde{\rho}^{-1}(S^{-1}r) = (A - p)^{-1}p = pA_p$, do đó (ii).

Ngược lại, giả sử rằng (ii) được thỏa mãn, và gọi $r$ là iđêan nguyên tố duy nhất của $B$ nằm trên $p$. Vì $(S^{-1}B)_{S^{-1}r}$ được đồng nhất với $B_r$, chỉ cần chứng minh rằng $S^{-1}B$ là địa phương với iđêan cực đại $S^{-1}r$, nghĩa là mọi iđêan nguyên tố $q$ của $B$ sao cho $\rho^{-1}(q) \subset p$ đều được chứa trong $r$. Nếu $p$ là cực tiểu, ta có $\rho^{-1}(q) = p$, do đó $q = r$. Nếu $B$ nguyên trên $A$, thì theo V, § 2, no. 1, hệ quả 2 của định lý 1, tồn tại một iđêan nguyên tố $r'$ của $B$ sao cho $q \subset r'$ và $\rho^{-1}(r') = p$; tất yếu có $r' = r$, do đó $q \subset r$.

#### Bổ đề 2 {#ac-viii-s7-lem-2 .statement}

*Giả sử rằng $A$ là nửa địa phương; gọi $q$ là một iđêan định nghĩa của $A$, và gọi $\rho : A \to B$ là một đồng cấu vành biến $B$ thành một $A$-môđun sinh hữu hạn. Giả sử rằng, với mọi iđêan nguyên tố (tất yếu là cực tiểu) $p$ của $A$ sao cho $\dim(A/p) = \dim(A)$, tồn tại một iđêan nguyên tố duy nhất $r$ của $B$ nằm trên $p$ và đồng cấu chính tắc $\rho_p : A_p \to B_r$ là song ánh. Khi đó có $\dim_A(B) = \dim(A)$ và $e_q^A(B) = e_q^A(A)$.*

Gọi $\mathfrak{S}_A$ (resp. $\mathfrak{S}_B$) là tập hợp các iđêan nguyên tố $p$ của $A$ sao cho

$$
\dim(A/p) = \dim(A) \quad (\text{resp. } \dim_A(B/pB) = \dim_A(B));
$$

ta có $\mathfrak{S}_A \neq \varnothing$. Lấy $p \in \mathfrak{S}_A$; theo giả thiết, tồn tại một iđêan nguyên tố của $B$ nằm trên $p$. Khi đó ta có $\rho^{-1}(pB) = p$ (II, § 2, no. 5, hệ quả 3 của mệnh đề 11), và

$$
\dim(A/p) = \dim(B/pB) = \dim_A(B/pB)
$$

theo định lý 1, b) và c) của § 2, no. 3. Do đó, ta có

$$
\dim_A(B) \geq \dim_A(B/pB) = \dim(A/p) = \dim(A) \geq \dim_A(B).
$$

Điều này suy ra $\mathfrak{S}_A \subset \mathfrak{S}_B$ và $\dim(A) = \dim_A(B)$. Ngược lại, nếu $p \in \mathfrak{S}_B$, ta có các bất đẳng thức

$$
\dim_A(B/pB) = \dim_A(B) = \dim(A) \geq \dim(A/p) \geq \dim_A(B/pB),
$$

do đó $p \in \mathfrak{S}_A$ và $\mathfrak{S}_B = \mathfrak{S}_A$. Theo mệnh đề 3 của no. 1 và hệ quả của nó, ta có

$$
e_q^A(A) = \sum_{p \in \mathfrak{S}_A} e_q^A(A/p) \quad \text{and} \quad e_q^A(B) = \sum_{p \in \mathfrak{S}_B} \operatorname{long}_{A_p}(A_p \otimes_A B) e_q^A(A/p);
$$

theo Bổ đề 1, ta có $\operatorname{long}_{A_p}(A_p \otimes_A B) = 1$ với mọi $p \in \mathfrak{S}_A$, do đó $e_q^A(A) = e_q^A(B)$.

#### Mệnh đề 6 {#ac-viii-s7-prop-6 .statement}

*Giả sử $A$ là nửa địa phương và rút gọn; gọi $q$ là một iđêan định nghĩa của $A$; gọi $A'$ là vành phân thức toàn phần của $A$, và gọi $B$ là một A-đại số con hữu hạn của $A'$. Khi đó $B$ là nửa địa phương và $qB$ là một iđêan định nghĩa của nó. Giả sử rằng, với mọi iđêan cực đại m của B sao cho dim(B_m) = dim(B), ta có [B/m : A/(A ∩ m)] = 1. Khi đó ta có $e_q^A(A) = e_{q_B}^B(B)$.

Theo IV, § 2, No. 5, hệ quả 3 của mệnh đề 9, B là nửa địa phương với iđêan định nghĩa qB. Ta có $e_{q_B}^B(B) = e_q^A(B)$ theo hệ quả của Mệnh đề 5. Vì A′ được đồng nhất với $\prod_p A_p$ trong đó p chạy qua tập hợp các iđêan nguyên tố cực tiểu của A (IV, § 2, No. 5, mệnh đề 10), ánh xạ chính tắc $A_p \to A_p \otimes_A B$ là song ánh với mọi iđêan nguyên tố cực tiểu p của A. Từ đó suy ra theo các Bổ đề 1 và 2 rằng $e_q^A(B) = e_q^A(A)$, do đó mệnh đề được chứng minh.

#### Ví dụ {#ac-viii-s7-n3-exa-1 .statement}

Cho k là một trường có đặc số $\neq 2$ và lấy A là vành địa phương $k[[X, Y]]/(X^2 + Y^2)$ với trường thặng dư k. Lấy $B = k[[X, T]]/(T^2 + 1)$ trong đó $T = Y/X$. Phân biệt hai trường hợp: nếu — 1 là bình phương của một phần tử i của k, B có hai iđêan cực đại được sinh tương ứng bởi {X, T + i} và {X, T − i}, chúng có trường thặng dư là k, và ta có $e_{m_A}^A(A) = e_{m_{AB}}^B(B) = 2$. Nếu — 1 không là một bình phương trong k, B có một iđêan cực đại duy nhất (X) với trường thặng dư $k[T]/(T^2 + 1)$, và ta có $e_{m_A}^A(A) = 2,\ e_{m_{AB}}^B(B) = 1$.

### 4. Bội số và các dãy cát tuyến

#### Mệnh đề 7 {#ac-viii-s7-prop-7 .statement}

Giả sử A địa phương. Gọi s là một số nguyên $\geq 1$ và, với $1 \leq i \leq s$, gọi $\delta_i$ là một số nguyên $> 0$, $x_i$ là một phần tử của $m_A^{\delta_i}$, và $\xi_i$ là lớp của nó trong $m_A^{\delta_i}/m_A^{\delta_i+1}$. Giả sử rằng $(x_1, ..., x_s)$ là một dãy cát tuyến đối với A. Gọi x là iđêan của A được sinh bởi $(x_1, ..., x_s)$. Khi đó ta có $e(A/x) \geq \delta_1 ... \delta_s \cdot e(A)$, với đẳng thức nếu $(\xi_1, ..., \xi_s)$ là một dãy hoàn toàn cát tuyến đối với gr(A).

Đặt $B = A/x$, và xét các chuỗi hình thức

$$
H_A = \sum_{n \geq 0} \operatorname{long}(m_A^n/m_A^{n+1}) \cdot T^n, \quad H_B = \sum_{n \geq 0} \operatorname{long}(m_B^n/m_B^{n+1}) \cdot T^n
$$

và $H_B^{(s)} = (1 - T)^{-s} H_B$. Theo mệnh đề 6 của § 4, No. 5, ta có trong $\mathbf{Z}[[T]]$ bất đẳng thức

$$
H_B^{(s)} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) H_A,
$$

và có đẳng thức khi dãy $(\xi_1, ..., \xi_s)$ là hoàn toàn cát tuyến. Nhưng

$$
R(T) = \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T}
$$

là một đa thức của $\mathbf{Z}[T]$ sao cho $R(1) = \delta_1 ... \delta_s$. Đặt $\dim(A) = d$; ta có $\dim(B) = d - s$. Theo định lý 2 của § 4, No. 3, tồn tại các phần tử $R_A$ và $R_B$ của $\mathbf{Z}[T, T^{-1}]$ sao cho

$$
H_A = (1 - T)^{-d} R_A(T), \quad R_A(1) = e(A),
$$
$$
H_B = (1 - T)^{-d+s} R_B(T), \quad R_B(1) = e(A/x).
$$

Do đó ta có
$$
(1 - T)^{-d} R_B(T) = H_B^{(s)} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) H_A = (1 - T)^{-d} R(T) \, R_A(T),
$$
và đẳng thức xảy ra nếu dãy $(\xi_1, ..., \xi_s)$ là hoàn toàn cát tuyến. Kết luận theo Bổ đề 2 của § 4, No. 1.

#### Nhận xét {#ac-viii-s7-n4-rem-1 .statement}

Ngược lại, có thể chứng minh (*xem* p. 103, bài tập 4) rằng nếu A là chính quy và $e(A/x) = \delta_1 ... \delta_s$, thì dãy $(\xi_1, ..., \xi_s)$ là hoàn toàn cát tuyến.

#### Ví dụ {#ac-viii-s7-n4-exa-1 .statement}

Cho $A$ là một vành chuỗi hình thức $k[[X_1, ..., X_n]]$ trên một trường $k$; cho $F_1, ..., F_s$ là các phần tử của A, a là iđêan do chúng sinh ra, và $B = A/a$. Cho $P_1, ..., P_s \in k[X_1, ..., X_n]$ là các dạng ban đầu của các chuỗi $F_1, ..., F_s$ và $\delta_1, ..., \delta_s$ các bậc tương ứng của chúng. Nếu dãy $F_1, ..., F_s$ là secant trong A, ta có $e(B) \geq \delta_1 ... \delta_s$; nếu dãy $P_1, ..., P_s$ là hoàn toàn secant trong vành $k[X_1, ..., X_n]$, ta có $e(B) = \delta_1 ... \delta_s$.

Xét ví dụ vành $B = k[[X, Y]]/a$, trong đó a được sinh bởi $X^2 + Y^3$ và $X^2 + Y^4$; bất đẳng thức trên cho $e(B) \geq 4$; nhận thấy rằng a được sinh bởi các phần tử $X^2 + Y^3$ và $Y^4 - Y^3$, mà đối với chúng dãy các dạng ban đầu là hoàn toàn secant, ta thu được $e(B) = 6$.

### 5. Các phần tử hời hợt

Trong số này, q ký hiệu một iđêan của A được chứa trong căn của A, và M là một A-môđun hữu hạn sinh khác không sao cho $M/qM$ có độ dài hữu hạn.

#### Mệnh đề 8 {#ac-viii-s7-prop-8 .statement}

Cho $\delta > 0$ là một số nguyên, x là một phần tử của $q^\delta$, $\xi$ là lớp của nó trong $\mathrm{gr}_\delta(A) = q^\delta/q^{\delta+1}$ và $\varphi$ là phép nhân bởi $\xi$ trong gr(A)-môđun gr(M).

a) Chiều của A-môđun $M/xM$ bằng $\dim_A(M)$ hoặc bằng $\dim_A(M) - 1$. Trong trường hợp thứ hai, ta có $e_q(M/xM) \geq \delta e_q(M)$.

b) Giả sử rằng $\dim_A(M) \geq 1$ và hạt nhân của $\varphi$ có độ dài hữu hạn trên $A/q$. Khi đó ta có $\dim_A(M/xM) = \dim_A(M) - 1$. Hơn nữa:
(i) Nếu $\dim_A(M) > 1$, ta có $e_q(M/xM) = \delta e_q(M)$.
(ii) Nếu $\dim_A(M) = 1$, ta có với mọi số nguyên $n \geq 0$
$$
n \delta e_q(M) \leq \mathrm{long}_A(M/x^nM) \leq n \delta e_q(M) + \mathrm{long}_{A/q}(\mathrm{Ker}\ \varphi^n),
$$
trong đó $\varphi^n$ là lần lặp thứ n của tự đồng cấu $\varphi$, và
$$
\delta e_q(M) = e_{xA}(M) \leq \mathrm{long}_A(M/xM).
$$

Đặt $M'' = M/xM$; xét các chuỗi Hilbert-Samuel $H_M = H_{M,q}$ và $H_{M''} = H_{M'',q}$, cùng với chuỗi Poincaré $P(T) = \sum_{n \geq 0} \mathrm{long}_{A/q}(\mathrm{Ker}\ \varphi_n) \cdot T^n$. Theo § 4, No. 3, định lý 2 và No. 4, nhận xét 2, ta có
$$
H_M(T) = (1 - T)^{-d} R_M(T), \quad H_{M''}(T) = (1 - T)^{-d''} R_{M''}(T),
$$

với $d = \dim_A(M)$, $d'' = \dim_A(M'')$, $R_M$ và $R_{M''}$ trong $\mathbf{Z}[T]$, $R_M(1) = e_q(M)$, $R_{M''}(1) = e_q(M'')$. Theo bổ đề 6 của § 4, No. 5, ta có trong $\mathbf{Z}((T))$ các bất đẳng thức

$$
(1 - T^\delta) H_M^{(1)} \leq H_{M''}^{(1)} \leq (1 - T^\delta) H_M^{(1)} + T^\delta P^{(1)} .
$$

Đặt $R(T) = (1 - T^\delta)/(1 - T) = 1 + T + \cdots + T^{\delta-1}$, điều này cũng có thể viết thành

(1) $$ (1 - T)^{-d} R(T) R_M(T) \leq (1 - T)^{-d''-1} R_{M''}(T) \leq $$
$$ \leq (1 - T)^{-d} R(T) R_M(T) + (1 - T)^{-1} T^\delta P(T) . $$

Theo Bổ đề 2 của § 4, No. 1, bất đẳng thức thứ nhất (1) kéo theo hoặc $d'' \geq d$, hoặc $d'' = d - 1$ và $R(1) R_M(1) \leq R_{M''}(1)$, nghĩa là $\delta e_q(M) \leq e_q(M'')$. Điều này chứng minh a), vì $d'' \leq d$.

Dưới giả thiết của b), ta có $P(T) \in \mathbf{Z}[T]$ và $P(1) = \operatorname{long}_A(\operatorname{Ker} \varphi)$. Bất đẳng thức thứ hai (1) được viết là

$$
(1 - T)^{-d''-1} R_{M''}(T) \leq (1 - T)^{-d}(R(T) R_M(T) + T^\delta (1 - T)^{d-1} P(T)) .
$$

Giả sử rằng ta có $d > 1$; khi đó Bổ đề 2 của § 4, No. 1 cho $d'' + 1 \leq d$, do đó $d'' = d - 1$ theo phần a) của chứng minh; khi đó ta có

$$
R_{M''}(1) \leq R(1). R_M(1)
$$

(nơi đã dẫn), do đó (i).

Bây giờ giả sử $d = 1$. Theo nơi đã dẫn, ta có $d'' = 0$ và

$$
R_{M''}(1) \leq R(1). R_M(1) + P(1) .
$$

Do đó, $M''$ có độ dài hữu hạn bằng $e_q(M'') = R_{M''}(1)$, và ta thu được

(2) $$ \delta e_q(M) \leq \operatorname{long}_A(M/xM) \leq \delta e_q(M) + \operatorname{long}_A(\operatorname{Ker} \varphi) . $$

Cho $n \geq 1$ là một số nguyên. Thay $x$ bởi $x^n$ trong (2); vì thế ta có

(3) $$ n \delta e_q(M) \leq \operatorname{long}_A(M/x^nM) \leq n \delta e_q(M) + \operatorname{long}_A(\operatorname{Ker} \varphi^n) . $$

Ngay lập tức thấy rằng các môđun con $\operatorname{Ker} \varphi^n$ của gr(A)-môđun Noether gr(M) tạo thành một dãy tăng và do đó dừng, và mỗi môđun trong chúng đều có độ dài hữu hạn trên $A/q$. Chia cho $n \geq 1$ trong bất đẳng thức (3) và cho $n$ tiến tới $+ \infty$, ta được $e_{xA}(M) = \delta e_q(M)$ theo định nghĩa của $e_{xA}(M)$.

#### Bổ đề 3 {#ac-viii-s7-lem-3 .statement}

Cho $R$ là một vành phân bậc Noether với các bậc $\geq 0$, $E$ là một $R$-môđun phân bậc kiểu hữu hạn sao cho $E_n$ là một $R_0$-môđun có độ dài hữu hạn với mọi $n \in \mathbf{Z}$.
Các điều kiện sau là tương đương:
(i) $E$ là một $R$-môđun có độ dài hữu hạn;
(ii) tồn tại một số nguyên $n_0$ sao cho $E_n = 0$ với $n \geq n_0$;
(iii) mọi iđêan nguyên tố của $R$ liên kết với $E$ đều chứa $R_+ = \bigoplus_{n \geq 1} R_n$.

(i) ⇔ (ii): điều này là hiển nhiên.
(iii) ⇒ (i): cho $p$ là một iđêan nguyên tố liên kết với E. Nếu (iii) được thỏa mãn, ta có $p = p_0 + R_+$ trong đó $p_0$ là một iđêan nguyên tố của $R_0$, và R-môđun $R/p$ đẳng cấu với $R_0/p_0$. Theo IV, § 3, No. 1, hệ quả của Mệnh đề 1, $R_0$-môđun $R_0/p_0$ đẳng cấu với một môđun con của một trong các $E_k$, nên có độ dài hữu hạn. Do đó, $R/p$ có độ dài hữu hạn. Theo IV, § 2, No. 5, Mệnh đề 7, vì vậy $p$ là cực đại. Do tính tùy ý của $p$, R-môđun E có độ dài hữu hạn (nơi đã dẫn).
(i) ⇒ (iii): cho $p$ là một iđêan nguyên tố liên kết với E. Khi đó $p$ là phân bậc (IV, § 3, No. 1, Mệnh đề 1) và cực đại (IV, § 2, No. 5, Mệnh đề 7), nên chứa $R_+$ (§ 6, No. 2, Bổ đề 1).

#### Mệnh đề 9 {#ac-viii-s7-prop-9 .statement}

Gọi $p_1, ..., p_r$ là những iđêan nguyên tố của vành phân bậc $\mathrm{gr}(A) = \bigoplus_n (q^n/q^{n+1})$ liên kết với môđun phân bậc $\mathrm{gr}(M) = \bigoplus_n (q^n M/q^{n+1} M)$ và không chứa $\mathrm{gr}_1(A) = q/q^2$. Gọi $\delta$ là một số nguyên $> 0$, $\xi$ là một phần tử của $\mathrm{gr}_\delta(A)$, và $\varphi : \mathrm{gr}(M) \to \mathrm{gr}(M)$ là phép vị tự tỉ số $\xi$ trong $\mathrm{gr}(M)$. Để $\varphi_n$ là đơn ánh với mọi $n$ đủ lớn, điều kiện cần và đủ là $\xi$ không thuộc iđêan nào trong các $p_i$.
Thật vậy, các iđêan nguyên tố liên kết với $\mathrm{gr}(A)$-môđun $\mathrm{Ker}\, \varphi$ chính là những iđêan nguyên tố trong số các iđêan nguyên tố liên kết với $\mathrm{gr}(M)$ mà chứa $\xi$ (IV, § 1, No. 1, Định nghĩa 1). Theo Bổ đề 3, $(\mathrm{Ker}\, \varphi)_n$ bằng không với $n$ đủ lớn khi và chỉ khi mọi iđêan ấy đều chứa $\mathrm{gr}_+(A)$ (hay, điều tương đương, $\mathrm{gr}_1(A)$), do đó suy ra mệnh đề.

#### Định nghĩa 2 {#ac-viii-s7-def-2 .statement}

Cho A là một vành Noether, q là một iđêan của A được chứa trong căn của A, và M là một A-môđun hữu hạn sinh sao cho $M/qM$ có độ dài hữu hạn. Một phần tử x của A được gọi là hời hợt đối với M tương đối với q nếu nó thuộc q và nếu, với mọi $n$ đủ lớn, ánh xạ $q^n M/q^{n+1} M \to q^{n+1} M/q^{n+2} M$ cảm sinh bởi phép nhân với x là đơn ánh.

#### Nhận xét 1 {#ac-viii-s7-n5-rem-1 .statement}

Cho $\delta$ là một số nguyên $> 0$. Đôi khi người ta nói rằng một phần tử x của A là hời hợt cấp $\delta$ đối với M tương đối với q nếu $x \in q^\delta$, và nếu, với mọi $n$ đủ lớn, ánh xạ $q^n M/q^{n+1} M \to q^{n+\delta} M/q^{n+\delta+1} M$ cảm sinh bởi phép nhân với x là đơn ánh. Theo thuật ngữ này, các phần tử hời hợt theo nghĩa của Định nghĩa 2 chính là các phần tử hời hợt cấp 1.
2) Với các ký hiệu của Mệnh đề 9, x là hời hợt cấp $\delta$ khi và chỉ khi lớp $\xi$ của nó trong $\mathrm{gr}_\delta(A)$ không thuộc iđêan nào trong các $p_i$.
3) Theo III, § 1, No. 4, Mệnh đề 8, tồn tại một phần tử thuần nhất của $\mathrm{gr}(A)$ có bậc $> 0$ mà không thuộc iđêan nào trong các $p_i$. Do đó, tồn tại một số nguyên $\delta > 0$ và một phần tử hời hợt cấp $\delta$ đối với M.
4) Giả sử A là địa phương với trường thặng dư k, và xét ánh xạ chính tắc toàn ánh $\lambda : q \to q \otimes_A k$. Nó là hợp thành của các ánh xạ chính tắc $q \to q/q^2$ và $\bar{\lambda} : q/q^2 \to q \otimes_A k$. Theo bổ đề Nakayama, mỗi không gian con vectơ $V_i = \bar{\lambda}(p_i \cap (q/q^2))$ của $q \otimes_A k$ đều phân biệt với $q \otimes_A k$; nếu $\alpha \in q \otimes_A k$ không thuộc không gian nào trong các $V_i$, thì $\lambda^{-1}(\alpha)$ gồm các phần tử hời hợt đối với M (Mệnh đề 9). Nếu k là vô hạn, hợp của các $V_i$ phân biệt với $q \otimes_A k$ và vì thế tồn tại các phần tử hời hợt đối với M.

#### Định lý 1 {#ac-viii-s7-thm-1 .statement}

Cho $A$ là một vành Noether, $q$ một iđêan của $A$ được chứa trong căn của $A$ và $M$ một $A$-môđun sinh hữu hạn sao cho $M/qM$ có độ dài hữu hạn. Cho $x_1, ..., x_m$ là một dãy hữu hạn các phần tử của $q$. Đặt $x = Ax_1 + \cdots + Ax_m \subset q$.

a) Ta có $\dim_A(M/xM) \geq \dim_A(M) - m$.

b) Nếu $\dim_A(M/xM) = \dim_A(M) - m$, thì $e_q(M/xM) \geq e_q(M)$.

c) Nếu $m < \dim_A(M)$, và nếu với $i = 1, ..., m$, phần tử $x_i$ của $A$ là nông đối với $M/(x_1M + \cdots + x_{i-1}M)$ tương đối với $q$, thì ta có

$$
\dim_A(M/xM) = \dim_A(M) - m \quad \text{và} \quad e_q(M/xM) = e_q(M) .
$$

d) Nếu $m = \dim_A(M)$, và nếu, với $i = 1, ..., m$, phần tử $x_i$ của $A$ là nông đối với $M/(x_1M + \cdots + x_{i-1}M)$ tương đối với $q$, thì ta có

$$
e_q(M) = e_x(M) \leq \operatorname{long}(M/xM) < + \infty .
$$

Các phần $a), b),$ và c) suy ra, với $m = 1$, từ Mệnh đề 8, và trường hợp tổng quát được suy ra bằng quy nạp. Giả sử các giả thiết của d) được thỏa mãn và đặt $x' = Ax_1 + \cdots + Ax_{m-1}$ và $M' = M/x'M$, sao cho $M/xM$ được đồng nhất với $M'/x_mM'$. Khi đó, theo c), ta có $\dim_A(M') = 1$ và $e_q(M) = e_q(M')$. Theo Mệnh đề 8, $M/xM$ có độ dài hữu hạn và ta có $e_q(M') = e_{x_mA}(M') \leq \operatorname{long}(M/xM)$. Nhưng, vì $x_m^nM' = x^nM'$ với mọi $n$, ta có $e_{x_mA}(M') = e_x(M')$. Mặt khác, ta có $e_x(M') \geq e_x(M)$: điều này suy ra từ b), trong đó $m$ được thay bằng $m - 1$, $x$ bằng $x'$, và $q$ bằng $x$. Do đó, ta có

$$
e_x(M) \leq e_x(M') = e_{x_mA}(M') = e_q(M') = e_q(M) .
$$

Vì $x$ được chứa trong $q$, điều này kéo theo $e_x(M) = e_q(M)$ (No. 1, Nhận xét 1), và hoàn thành chứng minh.

#### Hệ quả {#ac-viii-s7-n5-cor-1 .statement}

Giả sử rằng $A$ là địa phương, với trường thặng dư vô hạn, và đặt $d = \dim_A(M)$. Tồn tại một dãy $x_1, ..., x_d$ các phần tử của $q$ sao cho, khi đặt $x = Ax_1 + \cdots + Ax_d$, ta có

$$
e_q(M) = e_x(M) \leq \operatorname{long}(M/xM) < + \infty .
$$

Điều này suy ra ngay từ định lý và Nhận xét 4.

#### Nhận xét 5 {#ac-viii-s7-n5-rem-5 .statement}

Trong tình huống của hệ quả trước, ta có

$$
e_q(M) = e_x(M) \leq \operatorname{long}(M/xM)
$$

và $\operatorname{long}(M/qM) \leq \operatorname{long}(M/xM)$; cả ba trường hợp

$$
e_q(M) < \operatorname{long}(M/qM) , \quad e_q(M) = \operatorname{long}(M/qM) , \quad e_q(M) > \operatorname{long}(M/qM)
$$

đều có thể xảy ra (p. 106, Bài tập 16 và 17).

Bài tập

## BÀI TẬP {#ac-viii-s7-exercises}

Xem [các bài tập của § 7](exercises/s7/).
