---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 3
section_title: Dimension des anneaux noethériens
lang: vi
source: ac-viii-ix-fr
book_pages: AC VIII.86-AC VIII.87
pdf_pages: 0028-0041, 0090-0091
extraction: ocr
subsections:
    - "no": 1
      title: Dimension d’un anneau quotient
      page: 24
      pdf_page: 28
    - "no": 2
      title: Dimension et suites sécantes
      page: 26
      pdf_page: 30
    - "no": 3
      title: Premières applications
      page: 0
      pdf_page: 33
    - "no": 4
      title: Changements d’anneaux
      page: 32
      pdf_page: 36
    - "no": 5
      title: Construction de suites sécantes
      page: 36
      pdf_page: 40
statements: 37
exercises: 7
content_sha256: 85498b6f13398e68adef318d9085dbf17b24324f439cb30bf039a1f170786697
translated_from: content/en-mt/ac/VIII/03_s3_dimension_des_anneaux_noetheriens.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 0976dc84de4c6a097918bcbae5d2ed7aef13d1d806c7d00142b71ad1346c74a4
translation_model: gpt-5.4
translation_run: translate-vi-cb41a630
glossary_version: 34
glossary_terms_sha256: 216638718bb0501da6904c2720d775c32c2298e9c2c02d8ba251fad3ff5040f9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CHIỀU CỦA CÁC VÀNH NOETHER

### 1. Chiều của một vành thương

#### Mệnh đề 1 {#ac-viii-s3-prop-1 .statement}

Cho $A$ là một miền nguyên Noether, $x$ là một phần tử khác không của $A$ và $p$ là một phần tử cực tiểu trong tập hợp các iđêan nguyên tố của $A$ chứa $x$. Khi đó $p$ có chiều cao 1.

Cho $q \subset p$ là một iđêan nguyên tố phân biệt với $p$. Ta có $x \notin q$ do tính chất cực tiểu của $p$. Vì $A$ là một miền nguyên, $A_p$ có thể được đồng nhất với một vành con của $A_q$; với mọi số nguyên $n \geq 0$, ký hiệu $q_n$ là iđêan $q^n A_q \cap A_p$ của $A_p$. Tính chất cực tiểu của $p$ có nghĩa là vành địa phương $A_p / xA_p$ có chiều 0; do đó nó có độ dài hữu hạn ($§ 1$, no 3, ví dụ 1), và tồn tại một số nguyên $n_0 \geq 0$ sao cho ta có

$$
q_n + xA_p = q_{n+1} + xA_p \quad \text{với mọi } n \geq n_0 .
$$

Cố định số nguyên $n \geq n_0$. Với $y \in q_n$, tồn tại $a \in A_p$ sao cho $y - ax \in q_{n+1}$; khi đó ta có $ax \in q_n$, do đó $a \in q_n$ vì $x \notin q$, và cuối cùng ta có $y \in q_{n+1} + xq_n$. Vậy ta có

$$
q_n = q_{n+1} + xq_n .
$$

Vì $x$ thuộc iđêan cực đại của vành địa phương Noether $A_p$, bổ đề Nakayama cho thấy rằng ta có $q_n = q_{n+1}$. Vì ta có $(qA_q)^n = q_n A_q$, suy ra

$$
(qA_q)^n = (qA_q)^{n+1} \quad \text{với mọi } n \geq n_0 .
$$

Vì vành $A_q$ là địa phương và Noether, ta có $\bigcap_{n \geq 0} (qA_q)^n = \{0\}$ (III, § 3, no 2, hệ quả của mệnh đề 5) do đó $(qA_q)^{n_0} = \{0\}$ và cuối cùng iđêan nguyên tố $qA_q$ của $A_q$ thu về 0. Vậy $q = \{0\}$, điều này chứng minh rằng $p$ có chiều cao 1.

#### Mệnh đề 2 {#ac-viii-s3-prop-2 .statement}

Cho $A$ là một vành Noether, $m$ là một số nguyên dương và $a$ là một iđêan được chứa trong căn của $A$ và được sinh bởi $m$ phần tử. Ta có

$$
\dim(A/a) \leq \dim(A) \leq \dim(A/a) + m .
$$

Bất đẳng thức $\dim(A/a) \leq \dim(A)$ suy ra từ mệnh đề 6 của § 1, no 3. Một phép quy nạp ngay lập tức theo $m$ cho thấy rằng chỉ cần thiết lập bất đẳng thức

$$
\dim(A) \leq \dim(A/xA) + 1
$$

đối với mọi phần tử $x$ của căn của $A$, nghĩa là chứng minh rằng ta có $\dim(A/xA) \geq n - 1$ đối với mọi chuỗi $p_0 \subset ... \subset p_n$ các iđêan nguyên tố của $A$, có độ dài $n \geqslant 1$, và sao cho $x \in p_n$. Chỉ cần xây dựng một chuỗi $q_1 \subset ... \subset q_n$ các iđêan nguyên tố của $A$, với $x \in q_1$ và điều này suy ra từ bổ đề sau:

#### Bổ đề 1 {#ac-viii-s3-lem-1 .statement}

Cho $A$ là một vành Noether, $p_0 \subset ... \subset p_n$ một chuỗi các iđêan nguyên tố của $A$ có độ dài $n \geqslant 1$, và $x$ là một phần tử của $p_n$. Tồn tại một chuỗi $p'_0 \subset ... \subset p'_n$ với $p'_0 = p_0$, $p'_n = p_n$ và $x \in p'_1$.

Ta lập luận bằng quy nạp theo $n$, trường hợp $n = 1$ là tầm thường. Vậy giả sử rằng ta có $n \geqslant 2$ và rằng $x$ không thuộc $p_{n-1}$. Gọi $p'_{n-1}$ là một phần tử cực tiểu của tập hợp các iđêan nguyên tố của $A$ được chứa trong $p'_n = p_n$ và chứa $p_{n-2} + Ax$ (II, § 2, No. 6, bổ đề 2). Theo mệnh đề 1, iđêan $p'_{n-1}/p_{n-2}$ của vành $A/p_{n-2}$ có chiều cao 1, và vì $p_{n-2} \subset p_{n-1} \subset p_n$ là một chuỗi có độ dài 2, điều tương tự cũng đúng với $p_{n-2} \subset p'_{n-1} \subset p'_n$. Ta có $x \in p'_{n-1}$. Giả thiết quy nạp áp dụng cho chuỗi $p_0 \subset p_1 \subset ... \subset p_{n-2} \subset p'_{n-1}$ cho thấy rằng tồn tại một chuỗi $p'_0 \subset p'_1 \subset ... \subset p'_{n-2} \subset p'_{n-1}$ với $x \in p'_1$ và $p'_0 = p_0$. Chuỗi
$$
p'_0 \subset p'_1 \subset ... \subset p'_{n-1} \subset p'_n
$$
thỏa mãn các điều kiện cần có.

#### Hệ quả 1 {#ac-viii-s3-lem-1-cor-1 .statement}

a) Mọi vành địa phương Noether đều hữu hạn chiều. Nói chung hơn, mọi vành nửa địa phương Noether khác không (II, § 3, No. 5, def. 4) đều hữu hạn chiều.
b) Cho $A$ là một vành Noether. Mọi iđêan của $A$, phân biệt với $A$, đều có chiều cao hữu hạn.
c) Mọi dãy giảm các iđêan nguyên tố của một vành Noether $A$ đều dừng.

a) Cho $A$ là một vành Noether nửa địa phương khác không và $a$ là căn của nó; vành thương $A/a$ là Artin và khác không, do đó có chiều 0 ($§ 1$, No. 3, Ví dụ 1). Tồn tại một số nguyên $m \geqslant 0$ sao cho iđêan $a$ của $A$ được sinh bởi $m$ phần tử; do đó $0 \leqslant \dim(A) \leqslant m$ theo Mệnh đề 2.
b) Cho $a \neq A$ là một iđêan của $A$, và cho $m$ là một iđêan cực đại của $A$ chứa $a$. Ta có $0 \leqslant \mathrm{ht}(a) \leqslant \dim(A_m)$ theo Mệnh đề 7 của $§ 1$, No. 3, và $A_m$ là một vành Noether địa phương. Do đó $\mathrm{ht}(a)$ là hữu hạn theo a).
c) Mọi dãy giảm nghiêm ngặt hữu hạn $(p_i)_{0 \leqslant i \leqslant n}$ các iđêan nguyên tố của $A$ xác định một chuỗi $p_n \subset ... \subset p_0$, do đó $n \leqslant \dim(A_{p_0}) < + \infty$. Vậy không thể tồn tại một dãy giảm nghiêm ngặt vô hạn các iđêan nguyên tố của $A$, do đó c).

#### Hệ quả 2 {#ac-viii-s3-lem-1-cor-2 .statement}

Cho $A$ là một vành Noether địa phương.
a) Cho $x \in m_A$. Khi đó $\dim(A/xA)$ bằng $\dim(A)$ hoặc bằng $\dim(A) - 1$. Để có $\dim(A/xA) = \dim(A) - 1$, điều kiện cần và đủ là $x$ không thuộc iđêan nguyên tố cực tiểu nào $p$ của $A$ sao cho $\dim(A/p) = \dim(A)$, và điều kiện đủ là $x$ không là một ước của không trong $A$.
b) Cho $a$ là một iđêan của $A$ phân biệt với $A$ sao cho $\dim(A/a) < \dim(A)$. Tồn tại $x \in a$ sao cho $\dim(A/xA) = \dim(A) - 1$.
c) Nếu $\dim(A) \geqslant 1$, thì tồn tại $x \in m_A$ sao cho $\dim(A/xA) = \dim(A) - 1$.
Theo Mệnh đề 2, $\dim(A/xA)$ bằng $\dim(A)$ hoặc bằng $\dim(A) - 1$. Để có $\dim(A/xA) = \dim(A)$, điều kiện cần và đủ là tồn tại một chuỗi $p_0 \subset ... \subset p_n$ các iđêan nguyên tố của $A$ sao cho $x \in p_0$ và $n = \dim(A)$, nghĩa là tồn tại một iđêan nguyên tố $p_0$ của $A$ chứa $x$ sao cho $\dim(A/p_0) = \dim(A)$. Nhưng một iđêan nguyên tố như vậy $p_0$ tất yếu là cực tiểu, và do đó mọi phần tử của $p_0$ đều là một ước của không trong $A$ (IV, § 1, No. 1, Hệ quả 3 của Mệnh đề 2 và No. 4, Định lý 2). Điều này chứng minh a).

Gọi $\Phi$ là tập hợp các iđêan nguyên tố cực tiểu của $A$, và $\Phi'$ là tập hợp các $p \in \Phi$ sao cho $\dim(A/p) = \dim(A)$. Ta biết (II, § 4, No. 3, Hệ quả 3 của Mệnh đề 14) rằng $\Phi$ là hữu hạn, do đó $\Phi'$ là hữu hạn. Gọi $a$ là một iđêan của $A$ sao cho $\dim(A/a) < \dim(A)$. Với mọi $p \in \Phi'$, ta có $\dim(A/a) < \dim(A/p)$, do đó $a \not\subset p$. Bởi Mệnh đề 2 của II, § 1, No. 1, vì thế tồn tại một phần tử $x$ của $a$ không thuộc bất kỳ $p \in \Phi'$ nào, và khi đó ta có $\dim(A/xA) = \dim(A) - 1$ theo a). Điều này chứng minh b).

Mệnh đề c) là trường hợp riêng $a = m_A$ của b).

### 2. Chiều và các dãy cát tuyến

Cho $A$ là một vành Noether, $M$ là một $A$-môđun sinh hữu hạn, $S$ là một tập con của căn của $A$, $\mathfrak{S}$ là iđêan của $A$ sinh bởi $S$ và $a$ là linh hóa tử của $M$. Ta có

(6)
$$
\dim_A(M) = \dim(A/a) \leq \dim(A) ;
$$
do đó, nếu $A$ là địa phương, ta có $\dim_A(M) < + \infty$. Mặt khác, giá đỡ của $A$-môđun $M/SM$ bằng $V(a + \mathfrak{S})$ theo hệ quả của Mệnh đề 18 của II, § 4, No. 4, do đó

(7)
$$
\dim_A(M/SM) = \dim(A/(a + \mathfrak{S})) .
$$

Khi $S$ là hữu hạn, hoặc khi $M$ không thu về 0, ta có bất đẳng thức

(8)
$$
\dim_A(M/SM) \leq \dim_A(M) \leq \mathrm{Card}(S) + \dim_A(M/SM) ;
$$
khi $S$ là hữu hạn, điều này suy ra từ Mệnh đề 2 của No. 1 và các công thức (6) và (7) ở trên, còn trường hợp $S$ là vô hạn thì là tầm thường.

#### Định nghĩa 1 {#ac-viii-s3-def-1 .statement}

Cho $A$ là một vành địa phương Noether, $M$ là một $A$-môđun sinh hữu hạn khác không và $S$ là một tập con của iđêan cực đại $m_A$ của $A$. Ta nói rằng $S$ là cát tuyến đối với $M$ nếu ta có

(9)
$$
\dim_A(M) = \mathrm{Card}(S) + \dim_A(M/SM) .
$$

Nếu $S$ là cát tuyến đối với $M$, ta có $\mathrm{Card}(S) \leq \dim_A(M)$, do đó $S$ là hữu hạn. Ta nói rằng một họ $(x_i)_{i \in I}$ các phần tử của $m_A$ là cát tuyến đối với $M$ nếu ta có

(10)
$$
\dim_A(M) = \mathrm{Card}(I) + \dim_A(M/\sum_{i \in I} x_i M) ,
$$
nghĩa là nếu $i \mapsto x_i$ là một song ánh của $I$ lên một tập con cát tuyến của $m_A$ đối với $M$.

Một phần tử x của $m_A$ được gọi là cát tuyến đối với M nếu $\{ x \}$ là một tập con cát tuyến đối với M, nghĩa là nếu ta có
$$
\dim_A(M/xM) = \dim_A(M) - 1 .
$$

#### Nhận xét 1 {#ac-viii-s3-n2-rem-1 .statement}

Từ các công thức (6) và (7) suy ra rằng S là cát tuyến đối với M khi và chỉ khi nó là cát tuyến đối với $A/\alpha$, trong đó $\alpha$ là linh hóa tử của M.
2) Cho S và S’ là hai tập con rời nhau của $m_A$. Để $S \cup S'$ là cát tuyến đối với M, điều kiện cần và đủ là S cát tuyến đối với M và S’ cát tuyến đối với $M' = M/SM$. Điều này suy ra từ bất đẳng thức (8) và công thức
$$
\text{Card}(S \cup S') + \dim_A(M/(SM + S'M)) - \dim_A(M) =
= (\text{Card}(S) + \dim_A(M/SM) - \dim_A(M)) +
+ (\text{Card}(S') + \dim_A(M'/S'M') - \dim_A(M')) .
$$
3) Cho $x \in m_A$ và $n \geq 1$ là một số nguyên. Ngay lập tức thấy rằng các môđun $M/xM$ và $M/x^nM$ có cùng giá, do đó có cùng chiều. Do đó, x là cát tuyến đối với M khi và chỉ khi $x^n$ là cát tuyến đối với M. Từ điều này và Nhận xét 2, suy ra ngay lập tức kết quả sau: cho $x_1, ..., x_r$ là các phần tử của $m_A$ và $n_1, ..., n_r$ là các số nguyên $> 0$; khi đó dãy $(x_1, ..., x_r)$ là cát tuyến đối với M khi và chỉ khi dãy $(x_1^{n_1}, ..., x_r^{n_r})$ là cát tuyến đối với M.

#### Mệnh đề 3 {#ac-viii-s3-prop-3 .statement}

Cho A là một vành địa phương Noether và M là một A-môđun hữu hạn khác không. Để một phần tử x của $m_A$ là cát tuyến đối với M, điều kiện cần và đủ là nó không thuộc phần tử cực tiểu nào $p$ của $\mathrm{Supp}(M)$ sao cho $\dim(A/p) = \dim_A(M)$, và điều kiện đủ là phép vị tự $x_M$ có tỉ số x trong M là đơn ánh.
Cho $\alpha$ là linh hóa tử của M. Nói rằng x là cát tuyến đối với M có nghĩa là x là cát tuyến đối với $A/\alpha$; giá của M gồm các iđêan nguyên tố $p$ của A sao cho $\alpha \subset p$; và nếu $x_M$ là đơn ánh, thì ảnh của x trong $A/\alpha$ không phải là một ước của 0 trong $A/\alpha$. Khi đó Mệnh đề 3 suy ra từ Hệ quả 2 của Mệnh đề 2 của No. 1 áp dụng cho vành $A/\alpha$.

#### Hệ quả {#ac-viii-s3-n2-cor-1 .statement}

Mọi dãy các phần tử của $m_A$ hoàn toàn cát tuyến đối với M (A, X, p. 157, Định nghĩa 2) đều là cát tuyến đối với M.
Cho $(x_1, ..., x_r)$ là một dãy các phần tử của $m_A$ hoàn toàn cát tuyến đối với M. Đặt $M_0 = M$ và bằng quy nạp $M_i = M_{i-1}/x_i M_{i-1}$ với $1 \leq i \leq r$. Theo Hệ quả 1 của A, X, p. 160, phép vị tự có tỉ số $x_i$ trong $M_{i-1}$ là đơn ánh, do đó $\dim_A(M_i) = \dim_A(M_{i-1}) - 1$ (với $1 \leq i \leq r$) (Mệnh đề 3). Vì vậy ta có
$$
\dim_A(M) = r + \dim_A(M/(x_1M + \cdots + x_rM)) ,
$$
do đó dãy $(x_1, ..., x_r)$ là cát tuyến đối với M.

#### Nhận xét 4 {#ac-viii-s3-n2-rem-4 .statement}

Nói chung không đúng rằng một dãy cát tuyến đối với M thì hoàn toàn cát tuyến đối với M (p. 87, Bài tập 6). Chúng tôi sẽ nghiên cứu sau các môđun trên một vành địa phương Noether mà đối với chúng mọi dãy cát tuyến đều hoàn toàn cát tuyến.

#### Định lý 1 {#ac-viii-s3-thm-1 .statement}

Cho $A$ là một vành địa phương Noether, $M$ là một $A$-môđun hữu hạn khác không và $S$ là một tập con của iđêan cực đại $m_A$ của $A$.

a) Nếu $M/SM$ có độ dài hữu hạn, ta có $\mathrm{Card}(S) \geqslant \dim_A(M)$; nếu $S$ là cát tuyến đối với $M$, ta có $\mathrm{Card}(S) \leqslant \dim_A(M)$.

b) Mọi tập con cát tuyến đối với $M$ đều được chứa trong một tập con cát tuyến cực đại đối với $M$.

c) Các tính chất sau là tương đương:
(i) $S$ là một tập con cát tuyến cực đại đối với $M$;
(ii) $S$ là một tập con cát tuyến đối với $M$ và $\mathrm{Card}(S) = \dim_A(M)$;
(iii) $M/SM$ có độ dài hữu hạn và $\mathrm{Card}(S) = \dim_A(M)$;
(iv) $S$ là một tập con cát tuyến đối với $M$ và $M/SM$ có độ dài hữu hạn.

Vì ta có $S \subset m_A$, bổ đề Nakayama cho thấy rằng ta có $M/SM \neq \{0\}$, do đó $\dim_A(M/SM) \geqslant 0$ với đẳng thức xảy ra khi và chỉ khi $M/SM$ có độ dài hữu hạn. Mệnh đề a) suy ra từ các công thức (8) và (9), cũng như từ tính tương đương của các tính chất (ii), (iii) và (iv).

Mệnh đề b) suy ra từ việc lực lượng của mọi tập con của $m_A$ cát tuyến đối với $M$ đều bị chặn trên bởi số nguyên $\dim_A(M)$.

Theo a), mọi tập con cát tuyến đối với $M$ có lực lượng bằng $\dim_A(M)$ đều là cực đại. Còn phải chứng minh rằng, nếu $S$ cát tuyến đối với $M$ và nếu $\mathrm{Card}(S) < \dim_A(M)$, thì $S$ không cực đại. Gọi $a$ là linh hóa tử của $M$, và $B$ là vành địa phương Noether $A/(a + SA)$. Theo hệ quả 2 của mệnh đề 2 của No. 1, tồn tại một phần tử $x$ của $m_A$ sao cho $\dim(B/xB) = \dim(B) - 1$; do đó $x \notin S$. Theo nhận xét 2, tập con $S \cup \{x\}$ của $m_A$ là cát tuyến đối với $A/a$, nên cũng cát tuyến đối với $M$ theo nhận xét 1.

#### Hệ quả {#ac-viii-s3-n2-cor-2 .statement}

Chiều của $M$ là số nhỏ nhất trong các số nguyên $d \geqslant 0$ sao cho tồn tại một dãy $(x_1, ..., x_d)$ các phần tử của $m_A$ mà A-môđun $M / \sum_{i=1}^d x_i M$ có độ dài hữu hạn.

Vì $\varnothing$ là một tập con cát tuyến đối với $M$, Định lý 1, b) chứng minh sự tồn tại của một dãy cát tuyến cực đại đối với $M$, chẳng hạn $(x_1, ..., x_d)$. Nhưng khi đó ta có $d = \dim_A(M)$ và A-môđun $M / \sum_{i=1}^d x_i M$ có độ dài hữu hạn theo tính chất (iii) của Định lý 1, c). Ngược lại, nếu $(x'_1, ..., x'_{d'})$ là một dãy các phần tử của $m_A$ sao cho A-môđun $M / \sum_{j=1}^{d'} x'_j M$ có độ dài hữu hạn, thì ta có $d' \geqslant \dim_A(M)$ theo Định lý 1, a).

Nhắc lại rằng (III, § 3, No. 2, Định nghĩa 1) một iđêan $q$ của một vành địa phương Noether $A$ là một iđêan xác định của $A$ nếu các tôpô $q$-adic và $m_A$-adic của $A$ trùng nhau.

#### Bổ đề 2 {#ac-viii-s3-lem-2 .statement}

Cho $A$ là một vành địa phương Noether và $q$ một iđêan của $A$. Các điều kiện sau là tương đương:

(i) $q$ là một iđêan xác định của $A$;
(ii) tồn tại một số nguyên $n \geqslant 0$ sao cho $m_A^n \subset q \subset m_A$;

(iii) ta có q ≠ A và A/q là một A-môđun có độ dài hữu hạn ;
(iv) V(q) bằng { m_A } (nói cách khác, m_A là iđêan nguyên tố duy nhất của A chứa q).

Thật vậy, tính tương đương của (i), (ii) và (iv) đã được chứng minh trong III, § 2, No. 5, và tính tương đương của (i) và (iii) suy ra từ IV, § 2, No. 5, Hệ quả 2 của Mệnh đề 9.

Hệ quả của Định lý 1 do đó cho phép phát biểu chú giải sau đây:

#### Chú giải {#ac-viii-s3-n2-sch-1 .statement}

Chiều của một vành địa phương Noether A là số nhỏ nhất trong các số nguyên d ≥ 0 sao cho tồn tại một iđêan xác định của A được sinh bởi d phần tử.

### 3. Những ứng dụng đầu tiên

Cho A là một vành Noether, V = Spec(A) phổ của nó. Trong số này, mọi tập con có dạng $^1 V(x)$ với $x \in A$ được gọi là một siêu mặt trong V.

#### Mệnh đề 4 {#ac-viii-s3-prop-4 .statement}

Cho X là một tập con đóng của V, và $H_1, ..., H_m$ là các siêu mặt trong V. Đặt $X' = X \cap H_1 \cap ... \cap H_m$.

a) Với mọi tập con đóng Y của V được chứa trong X', ta có

$$
\operatorname{codim}(Y, X') \geq \operatorname{codim}(Y, X) - m .
$$

b) Ta có $\operatorname{codim}(Z, X) \leq m$ với mọi thành phần bất khả quy Z của X'. Nếu X' khác rỗng, ta có $\operatorname{codim}(X', X) \leq m$.

c) Nếu Z là một tập con đóng bất khả quy của V được chứa trong X sao cho $\operatorname{codim}(Z, X) \leq m$, thì tồn tại các siêu mặt $H'_1, ..., H'_m$ sao cho Z là một thành phần bất khả quy của $X \cap H'_1 \cap ... \cap H'_m$.

Cho α là một iđêan của A và $x_1, ..., x_m$ là các phần tử của A sao cho $X = V(\alpha)$ và $H_i = V(x_i)$ với $1 \leq i \leq m$. Cho Z là một tập con đóng bất khả quy của V được chứa trong X; tồn tại một iđêan nguyên tố p của A chứa α và sao cho $Z = V(p)$.

Trước hết giả sử rằng Z được chứa trong X' và ký hiệu bởi $\xi_i$ ảnh của $x_i$ trong vành địa phương Noether $B = A_p/\alpha A_p$. Theo Mệnh đề 7, b) của § 1, No. 3, ta có

$$
\operatorname{codim}(Z, X) = \dim(B), \quad \operatorname{codim}(Z, X') = \dim(B/(\xi_1 B + \cdots + \xi_m B)) .
$$

Theo Mệnh đề 2 của No. 1, do đó ta có

(11)
$$
\operatorname{codim}(Z, X') \geq \operatorname{codim}(Z, X) - m .
$$

Nếu Z là một thành phần bất khả quy của X', ta có $\operatorname{codim}(Z, X') = 0$, do đó $\operatorname{codim}(Z, X) \leq m$; điều này chứng minh b). Ta chứng minh a) bằng cách lấy ở cả hai vế của (11) cận dưới lớn nhất trên tập hợp các thành phần bất khả quy Z của Y.

1 Nhắc lại rằng $V(x)$ gồm các iđêan nguyên tố của A chứa x.

Ngược lại, giả sử rằng ta có codim(Z, X) $\leq m$, nghĩa là dim(B) $\leq m$. Vì mọi phần tử của $A_p$ là tích của một phần tử khả nghịch của $A_p$ với ảnh của một phần tử của A, chú giải của No. 2 chứng minh sự tồn tại của các phần tử $x'_1, ..., x'_m$ của A mà các ảnh của chúng trong B sinh một iđêan xác định của B. Đặt $H'_i = V(x'_i)$ với $1 \leq i \leq m$. Hiển nhiên là Z là một thành phần bất khả quy của $X \cap H'_1 \cap ... \cap H'_m$.

#### Hệ quả 1 {#ac-viii-s3-prop-4-cor-1 .statement}

Cho H là một siêu mặt khác rỗng trong V. Đối chiều của H trong V bằng 0 hoặc 1.

Ta có codim(H, V) = 1 khi và chỉ khi H không chứa thành phần bất khả quy nào của V. Nếu như vậy, mọi thành phần bất khả quy của H đều có đối chiều 1 trong V.

Với mọi thành phần bất khả quy Z của H, ta có

$$
0 \leq \operatorname{codim}(Z, V) \leq 1
$$

theo Mệnh đề 4, b), và ta có codim(Z, V) = 0 khi và chỉ khi Z là một thành phần bất khả quy của V. Theo định nghĩa ta có

$$
\operatorname{codim}(H, V) = \inf_Z \operatorname{codim}(Z, V)
$$

trong đó Z chạy trên tập hợp các thành phần bất khả quy của H. Hệ quả 1 suy ra ngay từ các nhận xét này.

#### Hệ quả 2 {#ac-viii-s3-prop-4-cor-2 .statement}

Cho X là một tập con đóng bất khả quy của V và H là một siêu mặt trong V. Chỉ có thể xảy ra ba trường hợp:

1) ta có $X \subset H$;
2) tập hợp $X \cap H$ khác rỗng và mỗi thành phần bất khả quy Z của nó thỏa mãn $\operatorname{codim}(Z, X) = 1$;
3) tập hợp $X \cap H$ là rỗng.

Giả sử $X' = X \cap H$ khác rỗng và khác X; mọi thành phần bất khả quy Z của $X'$ đều phân biệt với X và thỏa mãn $\operatorname{codim}(Z, X) \leq 1$ theo Mệnh đề 4, b). Hệ quả 2 suy ra ngay từ điều này.

#### Hệ quả 3 {#ac-viii-s3-prop-4-cor-3 .statement}

Nếu A là phân tích duy nhất (VII, § 3, No. 3, Mệnh đề 2), thì các iđêan nguyên tố có chiều cao 1 của A là các iđêan chính được sinh bởi các phần tử extremal của A. Nếu hơn nữa A là địa phương, ta có $\dim(A/p) = \dim(A) - 1$ với mọi iđêan nguyên tố $p$ có chiều cao 1 của A.

Cho x là một phần tử cực biên của A. Khi đó Ax là một iđêan nguyên tố vì x là cực biên, có chiều cao 1 vì A là một miền nguyên (No. 1, Prop. 1). Cho p là một iđêan nguyên tố chiều cao 1 của A. Khi đó $V(p)$ là một thành phần bất khả quy của một siêu mặt $V(Ax)$ với một x thích hợp (Prop. 4, c)). Cho $x = \prod_i y_i^{n_i}$ là một phân tích của x thành một tích các phần tử cực biên sao cho $y_i$ và $y_j$ nguyên tố cùng nhau nếu $i \neq j$. Các thành phần bất khả quy của $V(Ax)$ là các $V(Ay_i)$. Do đó $p = Ay_i$ với một i thích hợp. Khẳng định cuối cùng suy ra từ Hệ quả 2 của Prop. 2 của No. 1.

#### Nhận xét 1 {#ac-viii-s3-n3-rem-1 .statement}

Giả sử A là một miền nguyên địa phương Noether chiều d; cho x là một phần tử khác không của m_A và đặt H = V(x). Theo Hệ quả 2 của Prop. 4, mọi thành phần bất khả quy của H đều có đối chiều 1 trong X, do đó có chiều $\leq d - 1$ ($§ 1$, No. 2, Prop. 3). Theo Hệ quả 2 của Prop. 2 của No. 1, H có chiều $d - 1$, và vì vậy một trong các thành phần ấy có chiều $d - 1$; tất cả đều như vậy nếu A là catenary. Tuy nhiên, nói chung có thể xảy ra rằng tồn tại một thành phần bất khả quy của H có chiều < $d - 1$ (x. p. 87, Exerc. 7).

#### Nhận xét 2 {#ac-viii-s3-n3-rem-2 .statement}

Cho $x_1, ..., x_n$ là các phần tử của A, và đặt $H_i = V(x_i)$ với $1 \leq i \leq n$. Giả sử tồn tại một A-môđun kiểu hữu hạn M có giá đỡ $V = \mathrm{Spec}(A)$, sao cho $(x_1, ..., x_n)$ là một dãy cát tuyến hoàn toàn đối với M. Khi đó mọi thành phần bất khả quy của $H_1 \cap ... \cap H_n$ đều có đối chiều n trong V: điều này suy ra dễ dàng từ hệ quả của Prop. 3 của No. 2.

#### Nhận xét 3 {#ac-viii-s3-n3-rem-3 .statement}

Nếu iđêan $\alpha$ của vành Noether A được sinh bởi m phần tử, thì ta có $\mathrm{ht}(\alpha) \leq m$. Điều này suy ra ngay từ Prop. 4.

#### Mệnh đề 5 {#ac-viii-s3-prop-5 .statement}

Cho A là một vành Noether và $p \subset q$ là một dây chuyền không bão hòa các iđêan nguyên tố của A. Tập hợp E các iđêan nguyên tố r của A sao cho $p \subset r \subset q$ là một dây chuyền thì là vô hạn. Ta có $\bigcup_{r \in E} r = q$ và $\bigcap_{r \in E} r = p$.

Nếu cần, thay thế A bởi $A/p$, ta được đưa về trường hợp $p = \{0\}$.

Theo Bổ đề 1 của No. 1, ta có $q = \bigcup_{r \in E} r$, và Prop. 2 của II, $§ 1$, No. 1 cho thấy E là vô hạn.

Cho $y \neq 0$ là một phần tử của $\bigcap_{r \in E} r$. Chiều cao của q là hữu hạn (No. 1, Cor. 1 of Prop. 2), và ta có $\mathrm{ht}(q) \geq 2$ theo giả thiết. Do đó tồn tại một iđêan nguyên tố $q' \subset q$ có chiều cao 2. Phần đầu của chứng minh áp dụng cho $q'$ cho thấy tập E’ các iđêan nguyên tố chiều cao 1 được chứa trong $q'$ là vô hạn; theo giả thiết, mỗi iđêan ấy đều chứa y. Bây giờ vành địa phương Noether $B = A_{q'}/yA_{q'}$ có chiều 1 theo Hệ quả 2 của Prop. 2 của No. 1. Với mọi $r \in E'$, iđêan nguyên tố $r/yA_{q'}$ của B do đó là cực tiểu; do đó, vành Noether B có vô số iđêan nguyên tố cực tiểu, điều này vô lý (II, $§ 4$, No. 3, Cor. 3 of Prop. 14). Vậy $\bigcap_{r \in E} r = \{0\}$.

#### Mệnh đề 6 {#ac-viii-s3-prop-6 .statement}

Cho A là một vành Noether có chiều $\geq 2$, và h là một số nguyên sao cho $0 < h < \dim(A)$.

a) A có vô số iđêan nguyên tố chiều cao h.

b) Nếu A hữu hạn chiều, nó có vô số iđêan nguyên tố p sao cho $\mathrm{ht}(p) = h$ và $\dim(A/p) = \dim(A) - h$.

Vì chiều của A là cận trên bé nhất của các chiều cao của các iđêan nguyên tố của A ($§ 1$, no. 3, prop. 8), vì mọi iđêan nguyên tố của A đều có chiều cao hữu hạn (no. 1, cor. 1 of prop. 2), và vì $h < \dim(A)$, nên tồn tại một số nguyên $n > h$ và một iđêan nguyên tố p có chiều cao n, do đó một dây chuyền $p_0 \subset ... \subset p_n = p$ các iđêan nguyên tố có độ dài n. Ta có $\mathrm{ht}(p_i) = i$ với $0 \leq i \leq n$, do đó $\mathrm{ht}(r) = h$ với mọi iđêan nguyên tố r của A sao cho $p_{h-1} \subset r \subset p_{h+1}$ là một dây chuyền. Tập E của các iđêan ấy là vô hạn theo prop. 5, do đó suy ra a).

Nếu $A$ có số chiều hữu hạn, có thể giả sử rằng trong phần trước ta có $n = \dim(A)$. Với mọi iđêan $r \in E$, ta có $\mathrm{ht}(r) = h$, do đó $\dim(A/r) \leq n - h$, và vì $r \subset p_{h+1} \subset ... \subset p_n$ là một dãy độ dài $n - h$, nên ta có $\dim(A/r) = n - h$.

Tồn tại các vành nguyên không Noether có chiều 2 mà chỉ có một iđêan nguyên tố chiều cao 1, chẳng hạn một vành định giá có chiều cao 2 (VI, § 4, no. 4, mệnh đề 5).

### 4. Thay đổi vành

#### Mệnh đề 7 {#ac-viii-s3-prop-7 .statement}

Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether, $M$ là một $A$-môđun sinh hữu hạn và $N$ là một $B$-môđun sinh hữu hạn. Đặt $\overline{B} = B \otimes_A \kappa_A = B/\rho(m_A).B$ và $\overline{N} = N \otimes_B \overline{B} = N/\rho(m_A).N$. Ta có

$$
\dim_B(M \otimes_A N) \leq \dim_A(M) + \dim_B(\overline{N}),
$$

và có đẳng thức nếu $N$ phẳng trên $A$.

Có thể giả sử $M$ và $N$ khác không. Theo hệ quả của định lý 1 (no. 2), tồn tại một tập con $S$ (ứng với $T$) của $m_A$ (ứng với $m_B$) sao cho $\mathrm{Card}(S) = \dim_A(M)$ (ứng với $\mathrm{Card}(T) = \dim_{\overline{B}}(\overline{N})$) và $M/SM$ là một $A$-môđun có độ dài hữu hạn (ứng với $\overline{N}/T\overline{N}$ là một $B$-môđun có độ dài hữu hạn). Ta có $\rho(S) \subset m_B$. Gọi $E$ là $B$-môđun $M \otimes_A N$; $B$-môđun $E/(\rho(S).E + T.E)$ đẳng cấu với $M/SM \otimes_A N/TN$, nên có độ dài hữu hạn: theo các mệnh đề 18 và 19 của II, § 4, no. 4, ta có

$$
\begin{align*}
\mathrm{Supp}(M/SM \otimes_A N/TN) &= \mathrm{Supp}(N/TN) \cap {}^a\rho^{-1}(\mathrm{Supp}(M/SM)) \\
&= \mathrm{Supp}(N/TN) \cap {}^a\rho^{-1}(\mathrm{Supp}(\kappa_A)) \\
&= \mathrm{Supp}(N/TN \otimes_A \kappa_A) = \mathrm{Supp}(\overline{N}/T\overline{N}) = \{m_B\}.
\end{align*}
$$

Suy ra, theo định lý 1, ta có bất đẳng thức

$$
\dim_B(E) \leq \mathrm{Card}(S) + \mathrm{Card}(T) = \dim_A(M) + \dim_{\overline{B}}(\overline{N}).
$$

Bây giờ giả sử $N$ phẳng trên $A$, và hãy chứng minh rằng có đẳng thức trong công thức (12). Gọi $a$ (ứng với $b$) là linh hóa tử của $M$ (ứng với $N$). Theo các mệnh đề 18 và 19 của II, § 4, no. 4, ta có

$$
\begin{align*}
\mathrm{Supp}(E) &= \mathrm{Supp}(N) \cap {}^a\rho^{-1}(\mathrm{Supp}(M)) \\
&= V(b) \cap {}^a\rho^{-1}(V(a)) = V(b + \rho(a).B).
\end{align*}
$$

Do đó

$$
\dim_B(M \otimes_A N) = \dim(B/(b + \rho(a).B))
$$

và cũng có

$$
\dim_A(M) + \dim_{\overline{B}}(\overline{N}) = \dim(A/a) + \dim(B/(b + \rho(m_A).B)).
$$

$$
\dim(B') \geq \dim(A') + \dim(B'/\rho'(\mathfrak{m}_{A'}).B')
$$

và vì vành $B'/\rho'(\mathfrak{m}_{A'}).B'$ đẳng cấu với $B/(b + \rho(\mathfrak{m}_A).B)$, mệnh đề của ta suy ra từ các công thức (13), (14) và (15).

#### Hệ quả 1 {#ac-viii-s3-prop-7-cor-1 .statement}

*Cho $\rho : A \to B$ là một đồng cấu địa phương của các vành địa phương Noether.*

*a)* *Ta có*

$$
\dim(B) \leq \dim(A) + \dim(B \otimes_A \kappa_A)
$$

*nếu $\rho$ biến $B$ thành một $A$-môđun phẳng thì có đẳng thức.*

*b)* *Giả sử rằng $\rho$ làm cho $B$ thành một A-môđun phẳng, và gọi $S$ là một tập con của $\mathfrak{m}_A$. Khi đó $S$ là cát tuyến đối với $A$ nếu và chỉ nếu $\rho(S)$ là cát tuyến đối với $B$.*

Mệnh đề *a)* là trường hợp riêng $M = A, N = B$ của Mệnh đề 7.
Ta hãy chứng minh *b)*. Dưới các giả thiết đã nêu, ta có

$$
\dim(B) = \dim(A) + \dim(\overline{B})
$$

với $\overline{B} = B \otimes_A \kappa_A = B/\rho(\mathfrak{m}_A).B$. Vì $\rho$ là đơn ánh (I, § 3, No. 5, Mệnh đề 9), ta có

$$
\mathrm{Card}(\rho(S)) = \mathrm{Card}(S).
$$

Cuối cùng $B' = B/\rho(S).B$ là một môđun phẳng trên $A' = A/SA$, do đó

$$
\dim(B/\rho(S).B) = \dim(A/SA) + \dim(\overline{B})
$$

vì $B'/\rho(\mathfrak{m}_{A'}).B'$ đẳng cấu với $\overline{B}$. Mệnh đề cần chứng minh suy ra ngay từ các công thức (17), (18) và (19).

#### Hệ quả 2 {#ac-viii-s3-prop-7-cor-2 .statement}

*Cho $\rho : A \to B$ là một đồng cấu của các vành Noether. Khi đó*

$$
\dim(B) \leq \dim(A) + \sup_{p \in \mathrm{Spec}(A)} \dim(B \otimes_A \kappa(p)).
$$

Gọi $q$ là một iđêan nguyên tố của $B$ và $p = \rho^{-1}(q)$. Theo Hệ quả 1, ta có $\dim(B_q) \leq \dim(A_p) + \dim(B_q \otimes_A \kappa(p))$. Suy ra (Mệnh đề 6, *b*) của § 1, No. 3) ta có bất đẳng thức $\dim(B_q) \leq \dim(A) + \dim(B \otimes_A \kappa(p))$, và kết luận nhờ Mệnh đề 8 của § 1, No. 3.

#### Hệ quả 3 {#ac-viii-s3-prop-7-cor-3 .statement}

Cho $A$ là một vành Noether và $n$ là một số nguyên $\geqslant 0$. Khi đó ta có

$$
\dim(A[X_1, ..., X_n]) = \dim(A) + n .
$$

Đặt $B = A[X_1, ..., X_n]$. Với mọi iđêan nguyên tố $p$ của $A$, vành $B \otimes_A \kappa(p)$ là một vành đa thức theo $n$ biến trên một trường, nên có chiều $n$ ($§ 2$, No. 4, Hệ quả 1 của Định lý 3). Theo Hệ quả 2, ta có $\dim(B) \leqslant \dim(A) + n$; bất đẳng thức ngược lại suy ra từ Ví dụ 4 của $§ 1$, No. 3.

#### Hệ quả 4 {#ac-viii-s3-prop-7-cor-4 .statement}

Cho $\rho : A \to B$ là một đồng cấu của các vành Noether, và $a$ là một iđêan của $A$. Ta có bất đẳng thức

$$
\text{ht}(\rho(a).B) \leqslant \text{ht}(a)
$$

nếu ánh xạ $^a\rho : \mathrm{Spec}(B) \to \mathrm{Spec}(A)$ là toàn ánh. Nếu $B$ là một A-môđun phẳng trung thành, ta có $\text{ht}(\rho(a).B) = \text{ht}(a)$.

Nếu $B$ phẳng trung thành trên $A$, thì $^a\rho$ là toàn ánh (II, $§ 2$, No. 5, Hệ quả 4 của Mệnh đề 11) và ta có $\text{ht}(a) \leqslant \text{ht}(\rho(a).B)$ ($§ 2$, No. 1, hệ quả của Mệnh đề 2).

Vậy còn phải chứng minh bất đẳng thức (20) dưới giả thiết $^a\rho$ là toàn ánh. Cho $p$ là một iđêan nguyên tố của $A$ sao cho $a \subset p$ và $\text{ht}(a) = \text{ht}(p)$ ($§ 1$, no 3, mệnh đề 7). Đặt $\overline{B} = B \otimes_A \kappa(p)$ và ký hiệu bởi $h$ đồng cấu chính tắc từ $B$ vào $\overline{B}$. Nếu $X = {}^a\rho^{-1}(p)$ là tập hợp khác rỗng các iđêan nguyên tố của $B$ nằm trên $p$, thì ta đã biết ($§ 2$, no 1, bổ đề 1) rằng ánh xạ $^ah$ là một đồng phôi từ $\mathrm{Spec}(\overline{B})$ lên không gian con $X$ của $\mathrm{Spec}(B)$. Cho $q$ là ảnh qua $^ah$ của một iđêan nguyên tố cực tiểu của $\overline{B}$; ta có $\dim(B_q \otimes_A \kappa(p)) = 0$ và Hệ quả 1 cho bất đẳng thức $\dim(B_q) \leqslant \dim(A_p) = \text{ht}(p) = \text{ht}(a)$, cuối cùng

$$
\text{ht}(\rho(a).B) \leqslant \text{ht}(q) = \dim(B_q) \leqslant \dim(A_p) = \text{ht}(p) = \text{ht}(a),
$$

do đó có hệ quả.

#### Mệnh đề 8 {#ac-viii-s3-prop-8 .statement}

Cho $A$ là một vành Noether, $a$ là một iđêan của $A$, $M$ là một $A$-môđun sinh hữu hạn, $\hat{A}$ và $\hat{M}$ lần lượt là các hoàn thành tách của $A$ và $M$ đối với tôpô $a$-adic.

a) Cho $m$ là một iđêan nguyên tố của $A$ chứa $a$ và $\hat{m} = m\hat{A}$. Khi đó $\hat{m}$ là một iđêan nguyên tố của $\hat{A}$ và ta có $\dim_{\hat{A}_{\hat{m}}}(\hat{M}_{\hat{m}}) = \dim_{A_m}(M_m)$.

b) Ta có $\dim_{\hat{A}}(\hat{M}) = \sup_m \dim_{A_m}(M_m)$, trong đó $m$ chạy qua tập hợp các iđêan nguyên tố (tương ứng, cực đại) của $A$ chứa $a$. Đặc biệt, ta có $\dim_{\hat{A}}(\hat{M}) \leqslant \dim_A(M)$.

a) Vì $\hat{A}/\hat{m}$ được đồng nhất với $A/m$, nên $\hat{m}$ là một iđêan nguyên tố của $\hat{A}$. Theo Định lý 3 của III, $§ 3$, No. 4, $\hat{A}$ phẳng trên $A$, do đó $\hat{A}_{\hat{m}}$ phẳng trên $A_m$. Hơn nữa, ánh xạ chính tắc từ $A$ vào $\hat{A}$ cảm sinh một đẳng cấu của $A/a$ lên $\hat{A}/a\hat{A}$, do đó cũng cảm sinh một đẳng cấu của $A_m/mA_m$ lên $\hat{A}_{\hat{m}}/m\hat{A}_{\hat{m}}$. Kết luận suy ra bằng cách áp dụng Mệnh đề 7 cho các vành $A_m$ và $\hat{A}_{\hat{m}}$ và cho các môđun $M_m$ và $\hat{A}_{\hat{m}}$ vì $M_m \otimes_{A_m} \hat{A}_{\hat{m}}$ đẳng cấu với $\hat{M}_{\hat{m}}$ (III, loc. cit. và Mệnh đề 8).

b) Theo Mệnh đề 8 của III, $§ 3$, No. 4, ánh xạ $m \mapsto \hat{m}$ là một song ánh từ tập hợp các iđêan cực đại của $A$ chứa $a$ lên tập hợp các iđêan cực đại của $\hat{A}$. Mệnh đề b) suy ra từ điều này và từ Mệnh đề 9 của $§ 1$, No. 4.

#### Hệ quả 1 {#ac-viii-s3-prop-8-cor-1 .statement}

Cho $A$ là một vành Zariski (III, $§ 3$, No. 3, Định nghĩa 2). Với mọi $A$-môđun $M$ kiểu hữu hạn, ta có $\dim_{\hat{A}}(\hat{M}) = \dim_A(M)$.

Thật vậy, tôpô của $A$ là tôpô $a$-adic, trong đó $a$ là một iđêan được chứa trong căn của $A$ (*loc. cit.*), tức là được chứa trong mọi iđêan cực đại $m$ của $A$. Do đó chỉ cần áp dụng mệnh đề b) của Mệnh đề 8.

#### Hệ quả 2 {#ac-viii-s3-prop-8-cor-2 .statement}

Cho $A$ là một vành Noether, $a$ là một iđêan của $A$, và $\hat{A}$ là bổ sung tách của $A$ đối với tôpô $a$-adic. Ta có $\dim(\hat{A}) \leqslant \dim(A)$, với đẳng thức khi $A$ là địa phương và $a$ phân biệt với $A$.

#### Hệ quả 3 {#ac-viii-s3-prop-8-cor-3 .statement}

Cho $A$ là một vành Noether và $n$ là một số nguyên $\geqslant 0$. Ta có

$$
\dim(A[[X_1, ..., X_n]]) = \dim(A) + n .
$$

Vành $A[[X_1, ..., X_n]]$ là bổ sung tách của vành đa thức $A[X_1, ..., X_n]$ đối với tôpô $a$-adic, trong đó $a$ là iđêan sinh bởi $X_1, ..., X_n$; do đó ta có

$$
\dim(A[[X_1, ..., X_n]]) \leqslant \dim(A[X_1, ..., X_n])
$$

theo Hệ quả 2. Mặt khác, ta có

$$
\dim(A[X_1, ..., X_n]) = \dim(A) + n
$$

theo Hệ quả 3 của Mệnh đề 7. Cuối cùng, ta có

$$
\dim(A) + n \leqslant \dim(A[[X_1, ..., X_n]])
$$

theo Ví dụ 4 của $§ 1$, No. 3.

#### Nhận xét 1 {#ac-viii-s3-n4-rem-1 .statement}

Cho $A$ là một vành Noether và $a$ là một iđêan của $A$. Giả sử rằng $A$ tách biệt và đầy đủ đối với tôpô $a$-adic, và xét vành $R = A \{ X_1, ..., X_n \}$ các chuỗi lũy thừa hình thức hạn chế (III, $§ 4$, No. 2, Định nghĩa 2). Khi đó $\dim(R) = \dim(A) + n$. Thật vậy, $R$ là đầy đủ hóa của vành $B = A[X_1, ..., X_n]$ đối với tôpô $aB$-adic, do đó $\dim(R) \leqslant \dim(A[X_1, ..., X_n]) = \dim(A) + n$. Bất đẳng thức ngược lại được chứng minh như trong trường hợp các chuỗi lũy thừa hình thức.

#### Nhận xét 2 {#ac-viii-s3-n4-rem-2 .statement}

Cho $A$ là một vành địa phương Noether, được đồng nhất với một vành con của đầy đủ hóa $\hat{A}$ của nó, và $B$ là một vành con của $\hat{A}$ chứa $A$. Giả sử rằng $B$ là địa phương Noether và ta có $m_A B = m_B$. Khi đó đơn ánh chính tắc từ $A$ vào $B$ kéo dài thành một đẳng cấu từ $\hat{A}$ lên đầy đủ hóa $\hat{B}$ của $B$ (III, $§ 3$, No. 5, Mệnh đề 11), do đó $\dim(B) = \dim(A)$ (Hệ quả 2 của Mệnh đề 8). Điều này đặc biệt áp dụng cho tình huống sau. \* Cho $k$ là một trường định giá đầy đủ không rời rạc, $A$ là vành địa phương của vành đa thức $k[X_1, ..., X_n]$ tại iđêan nguyên tố sinh bởi $X_1, ..., X_n$, và $B$ là vành các chuỗi lũy thừa hội tụ theo $X_1, ..., X_n$ với hệ số trong $k$. Khi đó các giả thiết trên được thỏa mãn, và do đó ta có $\dim(B) = n$.*

### 5. Phép dựng các dãy chính quy

#### Mệnh đề 9 {#ac-viii-s3-prop-9 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun sinh hữu hạn, $a$ là một tập con của $A$ ổn định đối với phép cộng và phép nhân, $q_1, ..., q_m$ là các iđêan nguyên tố của $A$ không chứa $a$, và $r \geq 1$ là một số nguyên sao cho

$$
\text{codim}(V(a) \cap \operatorname{Supp}(M), \operatorname{Supp}(M)) \geq r .
$$

Tồn tại một dãy $(x_1, ..., x_r)$ gồm các phần tử của $a$, không thuộc iđêan nào trong các iđêan $q_1, ..., q_m$, và sao cho dãy $(x_1/1, ..., x_r/1)$ các phần tử của $A_p$ là cát tuyến đối với $A_p$-môđun $M_p$, với mọi iđêan nguyên tố $p \in V(a) \cap \operatorname{Supp}(M)$.

Ta lập luận bằng quy nạp theo $r$. Trước hết giả sử $r = 1$, và gọi $\Phi$ là tập hợp (hữu hạn) các phần tử cực tiểu của $\operatorname{Supp}(M)$. Ta lập luận bằng phản chứng và giả sử rằng không tồn tại phần tử nào $x_1$ của $a$ thỏa mãn các điều kiện của mệnh đề. Lấy $x \in a$, không thuộc $q_1 \cup ... \cup q_m$. Theo giả thiết tồn tại một phần tử $p$ của $V(a) \cap \operatorname{Supp}(M)$ sao cho ảnh $x/1$ của $x$ trong $A_p$ không phải là phần tử cắt đối với $M_p$. Gọi $\Psi$ là tập hợp các iđêan $q \in \Phi$ được chứa trong $p$; khi đó các phần tử cực tiểu của $\operatorname{Supp}(M_p)$ là các iđêan nguyên tố $qA_p$ của $A_p$, trong đó $q$ chạy qua $\Psi$. Do Mệnh đề 3 của No. 2, vì thế tồn tại một phần tử $q$ của $\Psi$ sao cho $x/1 \in qA_p$, do đó $x \in q$. Nói cách khác, ta có $a \subset q_1 \cup ... \cup q_m \cup \bigcup_{q \in \Phi} q$. Vì $a \not\subset q_j$ với $1 \leq j \leq m$, Mệnh đề 2 của II, § 1, No. 1 chứng minh sự tồn tại của một phần tử $q$ của $\Phi$ chứa $a$, do đó

$$
V(q) \subset V(a) \cap \operatorname{Supp}(M) .
$$

Vì $V(a)$ chứa một thành phần bất khả quy của $\operatorname{Supp}(M)$, điều này mâu thuẫn với giả thiết

$$
\text{codim}(V(a) \cap \operatorname{Supp}(M), \operatorname{Supp}(M)) \geq 1 .
$$

Bây giờ giả sử $r \geq 2$. Theo giả thiết quy nạp, có thể tìm được một dãy $(x_1, ..., x_{r-1})$ các phần tử của $a$, không thuộc $q_1 \cup ... \cup q_m$, và sao cho, với mọi $p \in V(a) \cap \operatorname{Supp}(M)$, dãy $(x_1/1, ..., x_{r-1}/1)$ các phần tử của $A_p$ là cắt đối với $M_p$. Đặt $N = M / \sum_{i=1}^{r-1} x_i M$. Chỉ cần xây dựng một phần tử $x_r$ của $a$ không thuộc $q_1 \cup ... \cup q_m$ và sao cho, với mọi $p \in V(a) \cap \operatorname{Supp}(M)$, phần tử $x_r/1$ của $A_p$ là cắt đối với $N_p$. Theo phần đầu của chứng minh, chỉ cần thiết lập hai hệ thức

$$
V(a) \cap \operatorname{Supp}(M) = V(a) \cap \operatorname{Supp}(N) ,
$$
$$
\text{codim}(V(a) \cap \operatorname{Supp}(N), \operatorname{Supp}(N)) \geq 1 .
$$

Bây giờ ta có

$$
\operatorname{Supp}(N) = V(x_1) \cap ... \cap V(x_{r-1}) \cap \operatorname{Supp}(M)
$$

$$
m = r - 1,\quad X = \operatorname{Supp}(M),\quad Y = V(\alpha) \cap \operatorname{Supp}(N),\quad H_i = V(x_i)
$$

do đó $X' = \operatorname{Supp}(N)$.

#### Hệ quả 1 {#ac-viii-s3-prop-9-cor-1 .statement}

*Cho A là một vành Noether, M là một A-môđun hữu hạn sinh, $p_1, ..., p_n, q_1, ..., q_m$ là các iđêan nguyên tố của A và r là một số nguyên $\geqslant 1$. Giả sử rằng ta có $p_i \not\subset q_j$ với $1 \leqslant i \leqslant n$ và $1 \leqslant j \leqslant m$, và $\dim_{A_{p_i}}(M_{p_i}) \geqslant r$ với $1 \leqslant i \leqslant n$. Khi đó tồn tại một dãy $(x_1, ..., x_r)$ các phần tử của A thuộc mọi $p_i$ và không thuộc $q_j$ nào, sao cho, với $1 \leqslant i \leqslant n$, các ảnh của $x_1, ..., x_r$ trong $A_{p_i}$ tạo thành một dãy cát tuyến của môđun $M_{p_i}$.

Đặt $\alpha = \bigcap_i p_i$. Ta có $M_{p_i} \neq \{0\}$, do đó $p_i \in \operatorname{Supp}(M)$ với $1 \leqslant i \leqslant n$, suy ra $V(\alpha) \subset \operatorname{Supp}(M)$. Ta có

$$
\operatorname{codim}(V(\alpha) \cap \operatorname{Supp}(M), \operatorname{Supp}(M)) = \operatorname{codim}(V(\alpha), \operatorname{Supp}(M)) =
= \inf_i (\operatorname{codim}(V(p_i), \operatorname{Supp}(M))) = \inf_i \dim(M_{p_i}) \geqslant r
$$

(§ 1, No. 4, Mệnh đề 9), và áp dụng Mệnh đề 9.

#### Hệ quả 2 {#ac-viii-s3-prop-9-cor-2 .statement}

*Cho A là một vành địa phương Noether, M là một A-môđun hữu hạn sinh khác không và $\alpha$ là một tập con của $m_A$, ổn định đối với phép cộng và phép nhân và sao cho $\operatorname{long}(M/\alpha M) < +\infty$. Tồn tại một tập con của $\alpha$ là một tập con cát tuyến cực đại của M.*

Thật vậy, ta có $V(\alpha) \cap \operatorname{Supp}(M) = \operatorname{Supp}(M/\alpha M) = \{m_A\}$ (§ 1, No. 4, Nhận xét 1), do đó $\operatorname{codim}(V(\alpha) \cap \operatorname{Supp}(M), \operatorname{Supp}(M)) = \dim(\operatorname{Supp}(M)) = \dim_A(M)$, và áp dụng Mệnh đề 9.

## BÀI TẬP {#ac-viii-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).*
