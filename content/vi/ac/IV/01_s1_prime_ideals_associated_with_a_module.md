---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 1
section_title: Prime ideals associated with a module
lang: vi
source: ac-i-vii
book_pages: 261-267, 286-290
pdf_pages: 0281-0287, 0306-0310
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF ASSOCIATED PRIME IDEALS
      page: 261
      pdf_page: 281
    - "no": 2
      title: LOCALIZATION OF ASSOCIATED PRIME IDEALS
      page: 263
      pdf_page: 283
    - "no": 3
      title: RELATIONS WITH THE SUPPORT
      page: 265
      pdf_page: 285
    - "no": 4
      title: THE CASE OF FINITELY GENERATED MODULES OVER A NOETHERIAN RING
      page: 265
      pdf_page: 285
statements: 24
exercises: 19
content_sha256: cd292f897a412048592c19c416a1b7b36aa47eefe472fa4f37babbac3992c2fd
translated_from: content/en/ac/IV/01_s1_prime_ideals_associated_with_a_module.md
source_content_sha256: a0083654b94c5bf51cd105c953d229508db86368fcf74e189f13c7e0aea21748
translation_model: gpt-5-6-mini
translation_run: translate-vi-8e55ed5d
glossary_version: 34
glossary_terms_sha256: cad1006a57d788a26d61d39fe9dbbcabeaece5892262ac4f1c740753812c83f9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 1. CÁC IĐÊAN NGUYÊN TỐ LIÊN KẾT VỚI MỘT MÔĐUN

### 1. ĐỊNH NGHĨA CÁC IĐÊAN NGUYÊN TỐ LIÊN KẾT

#### Định nghĩa 1 {#ac-iv-s1-def-1 .statement}

Cho M là một môđun trên một vành A. Một iđêan nguyên tố p được gọi là liên kết với M nếu tồn tại x ∈ M sao cho p bằng linh hóa tử & x. Tập hợp các iđêan nguyên tố liên kết với M được ký hiệu bởi Ass_A(M), hoặc đơn giản là Ass(M).

\* Ví dụ. Cho a là một iđêan trong vành đa thức A = \mathbf{C}[X_1, ..., X_n], V là đa tạp đại số affine tương ứng và V_1, ..., V_p là các thành phần bất khả quy của V. Nếu lấy M là vành A/a của các hàm chính quy trên V, tập hợp các iđêan nguyên tố liên kết với M gồm các iđêan của V_1, ..., V_p và nói chung các iđêan nguyên tố khác, mỗi iđêan trong số đó chứa một trong các iđêan của các V_i. \*

Vì linh hóa tử của 0 là A, một phần tử x ∈ M có linh hóa tử là một iđêan nguyên tố nhất thiết phải ≠ 0. Nói rằng một iđêan nguyên tố p liên kết với M

(*) Các kết quả của chương này chỉ phụ thuộc vào các Quyển I đến VI và các Chương I đến III của Quyển này, không kể Chương I, § 4 và Chương III, § 5.

có nghĩa là nói rằng $M$ chứa một môđun con *đẳng cấu với* $A/p$ (cụ thể là $Ax$, với mọi $x \in M$ có linh hóa tử là $p$).

Nếu một $A$-môđun $M$ là hợp của một họ $(M_i)_{i \in I}$ các môđun con, thì rõ ràng
$$
\operatorname{Ass}(M) = \bigcup_{i \in I} \operatorname{Ass}(M_i).
$$

#### Mệnh đề 1 {#ac-iv-s1-prop-1 .statement}

*Với mọi iđêan nguyên tố $p$ của một vành $A$ và mọi môđun con $M \neq 0$ của $A/p$, $\operatorname{Ass}(M) = \{p\}$.*

Vì vành $A/p$ là một miền nguyên, linh hóa tử của một phần tử $\neq 0$ của $A/p$ là $p$.

#### Mệnh đề 2 {#ac-iv-s1-prop-2 .statement}

*Cho $M$ là một môđun trên một vành $A$. Mọi phần tử cực đại của tập hợp các iđêan $\operatorname{Ann}(x)$ của $A$, trong đó x chạy qua tập hợp các phần tử $\neq 0$ của $M$, đều thuộc về $\operatorname{Ass}(M)$.*

Cho $a = \operatorname{Ann}(x)$ ($x \in M, x \neq 0$) là một phần tử cực đại như vậy; chỉ cần chứng minh rằng $a$ là nguyên tố. Vì $x \neq 0$, $a \neq A$. Cho $b, c$ là các phần tử của $A$ sao cho $bc \in a$ và $c \notin a$. Khi đó $cx \neq 0$, $b \in \operatorname{Ann}(cx)$ và $a \subset \operatorname{Ann}(cx)$. Vì $a$ là cực đại, $\operatorname{Ann}(cx) = a$, do đó $b \in a$, vậy $a$ là nguyên tố.

#### Hệ quả 1 {#ac-iv-s1-prop-2-cor-1 .statement}

*Cho $M$ là một môđun trên một vành Noether $A$. Khi đó điều kiện $M \neq \{0\}$ tương đương với $\operatorname{Ass}(M) \neq \varnothing$.*

Nếu $M = \{0\}$, rõ ràng $\operatorname{Ass}(M)$ là rỗng (không có giả thiết nào về $A$). Nếu $M \neq \{0\}$, tập hợp các iđêan có dạng $\operatorname{Ann}(x)$, trong đó $x \in M$ và $x \neq 0$, là không rỗng và gồm các iđêan $\# A$; vì $A$ là Noether, tập hợp này có một phần tử cực đại; khi đó chỉ cần áp dụng Mệnh đề 2.

#### Hệ quả 2 {#ac-iv-s1-prop-2-cor-2 .statement}

*Cho $A$ là một vành Noether, $M$ là một $A$-môđun và $a$ là một phần tử của $A$. Để phép vị tự trên $M$ với tỉ số $a$ là đơn ánh, điều kiện cần và đủ là $a$ thuộc không iđêan nguyên tố liên kết nào với $M$.*

Nếu $a$ thuộc một iđêan nguyên tố $p \in \operatorname{Ass}(M)$, thì $p = \operatorname{Ann}(x)$, trong đó $x \in M, x \neq 0$; do đó $ax = 0$ và phép vị tự với tỉ số $a$ không là đơn ánh. Ngược lại, nếu $ax = 0$ với một $x \in M$ sao cho $x \# 0$, thì $Ax \# \{0\}$, do đó $\operatorname{Ass}(x) \neq \varnothing$ (Hệ quả 1). Cho $p \in \operatorname{Ass}(Ax)$; khi đó hiển nhiên $p \in \operatorname{Ass}(M)$ và $p = \operatorname{Ann}(bx)$, trong đó $b \in A$; do đó $a \in p$, vì $abx = 0$.

#### Hệ quả 3 {#ac-iv-s1-prop-2-cor-3 .statement}

*Tập hợp các ước của không trong một vành Noether $A$ là hợp của các iđêan $p \in \operatorname{Ass}(A)$.*

#### Mệnh đề 3 {#ac-iv-s1-prop-3 .statement}

*Cho $A$ là một vành, $M$ là một $A$-môđun và $N$ là một môđun con của $N$. Khi đó*
$$
\operatorname{Ass}(N) \subset \operatorname{Ass}(M) \subset \operatorname{Ass}(N) \cup \operatorname{Ass}(M/N).
$$
*Sự bao hàm $\operatorname{Ass}(N) \subset \operatorname{Ass}(M)$ là hiển nhiên. Cho $p \in \operatorname{Ass}(M)$, $E$ là một môđun con của $M$ đẳng cấu với $A/p$ và $F = E \cap N$. Nếu $F = \{0\}$, $E$ đẳng cấu với một* môđun con của $M/N$, do đó $p \in \operatorname{Ass}(M/N)$. Nếu $F \neq \{0\}$, linh hóa tử của mọi phần tử $\neq 0$ của $F$ là $p$ (Mệnh đề 1) và do đó $p \in \operatorname{Ass}(F) \subset \operatorname{Ass}(N)$.

#### Hệ quả 1 {#ac-iv-s1-prop-3-cor-1 .statement}

*Nếu một A-môđun $M$ là tổng trực tiếp của một họ $(M_i)_{i \in I}$ các môđun con, thì* $\operatorname{Ass}(M) = \bigcup_{i \in I} \operatorname{Ass}(M_i)$.

Có thể quy về trường hợp $I$ hữu hạn nhờ (1), rồi quy về trường hợp $\operatorname{Card}(I) = 2$ bằng quy nạp theo $\operatorname{Card}(I)$. Khi đó đặt $I = \{i, j\}$, với $i \neq j$; vì $M/M_i$ đẳng cấu với $M_j$, nên $\operatorname{Ass}(M) \subset \operatorname{Ass}(M_i) \cup \operatorname{Ass}(M_j)$ (Mệnh đề 3); hơn nữa, $\operatorname{Ass}(M_i)$ và $\operatorname{Ass}(M_j)$ được chứa trong $\operatorname{Ass}(M)$ (Mệnh đề 3), do đó có kết quả.

#### Hệ quả 2 {#ac-iv-s1-prop-3-cor-2 .statement}

*Cho $M$ là một A-môđun và $(Q_i)_{i \in I}$ là một họ hữu hạn các môđun con của $M$. Nếu* $\bigcap_{i \in I} Q_i = \{0\}$, *thì*
$$
\operatorname{Ass}(M) \subset \bigcup_{i \in I} \operatorname{Ass}(M/Q_i).
$$
Ánh xạ chính tắc $M \to \bigoplus_{i \in I} (M/Q_i)$ là đơn ánh; khi đó chỉ cần áp dụng Mệnh đề 3 và Hệ quả 1 của nó.

#### Mệnh đề 4 {#ac-iv-s1-prop-4 .statement}

*Cho $M$ là một A-môđun và $\Phi$ là một tập con của $\operatorname{Ass}(M)$. Khi đó tồn tại một môđun con $N$ của $M$ sao cho* $\operatorname{Ass}(N) = \operatorname{Ass}(M) - \Phi$ *và* $\operatorname{Ass}(M/N) = \Phi$.

Gọi $\mathcal{E}$ là tập hợp các môđun con $P$ của $M$ sao cho $\operatorname{Ass}(P) \subset \operatorname{Ass}(M) - \Phi$. Công thức (1) chỉ ra rằng tập hợp $\mathcal{E}$, có thứ tự bởi quan hệ bao hàm, là *quy nạp*; hơn nữa, $\{0\} \in \mathcal{E}$ và do đó $\mathcal{E} \neq \varnothing$. Gọi $N$ là một phần tử cực đại của $\mathcal{E}$. Khi đó $\operatorname{Ass}(N) \subset \operatorname{Ass}(M) - \Phi$. Ta sẽ thấy rằng $\operatorname{Ass}(M/N) \subset \Phi$, điều này, theo Mệnh đề 3, sẽ hoàn thành chứng minh. Cho $p \in \operatorname{Ass}(M/N)$; khi đó $M/N$ chứa một môđun con $F/N$ đẳng cấu với $A/p$. Theo các Mệnh đề 1 và 3, $\operatorname{Ass}(F) \subset \operatorname{Ass}(N) \cup \{p\}$. Vì $N$ là cực đại trong $\mathcal{E}$, $F \notin \mathcal{E}$ và do đó $p \in \Phi$.

### 2. ĐỊNH VỊ CỦA CÁC IĐÊAN NGUYÊN TỐ LIÊN KẾT

#### Mệnh đề 5 {#ac-iv-s1-prop-5 .statement}

*Cho $A$ là một vành, $S$ là một tập con nhân của $A$, $\Phi$ là tập hợp các iđêan nguyên tố của $A$ không gặp $S$ và $M$ là một A-môđun. Khi đó*:
(i) *Ánh xạ* $p \mapsto S^{-1}p$ *là một song ánh từ* $\operatorname{Ass}_A(M) \cap \Phi$ *lên một tập con của* $\operatorname{Ass}_{S^{-1}A}(S^{-1}M)$.
(ii) *Nếu* $p \in \Phi$ *là một iđêan sinh hữu hạn và* $S^{-1}p \in \operatorname{Ass}_{S^{-1}A}(S^{-1}M)$, *thì* $p \in \operatorname{Ass}_A(M)$.

Nhắc lại (Chương II, § 2, no. 5, Mệnh đề 11) rằng ánh xạ $p \mapsto S^{-1}p$ là một song ánh của $\Phi$ lên tập hợp các iđêan nguyên tố của $S^{-1}A$. Nếu $p \in \operatorname{Ass}_A(M) \cap \Phi$, $p$ là linh hóa tử của một môđun con đơn sinh $N$ của $M$; khi đó $S^{-1}p$ là linh hóa tử của môđun con đơn sinh $S^{-1}N$ của $S^{-1}M$ (Chương II, § 2, no. 4, công thức (9)) và do đó $S^{-1}\mathfrak{p} \in \mathrm{Ass}_{S^{-1}A}(S^{-1}M)$. Ngược lại, giả sử rằng $\mathfrak{p} \in \Phi$ là sinh hữu hạn và sao cho $S^{-1}\mathfrak{p}$ liên kết với $S^{-1}M$; khi đó tồn tại $x \in M$ và $t \in S$ sao cho $S^{-1}\mathfrak{p}$ là linh hóa tử của $x/t$. Gọi $(a_i)_{1 \leq i \leq n}$ là một hệ sinh của $\mathfrak{p}$; khi đó $(a_i/1)(x/t) = 0$ và do đó tồn tại $s_i \in S$ sao cho $s_i a_i x = 0 \ (1 \leq i \leq n)$. Ta viết $s = s_1 s_2 \ldots s_n$; với mọi $a \in \mathfrak{p}$, $s a x = 0$, do đó $p \subset \mathrm{Ann}(s x)$; mặt khác, nếu $b \in A$ thỏa mãn $b s x = 0$, thì $b/1 \in S^{-1}\mathfrak{p}$ theo định nghĩa, do đó $b \in \mathfrak{p}$. Khi đó $\mathfrak{p} = \mathrm{Ann}(s x)$ và $\mathfrak{p} \in \mathrm{Ass}_A(M)$.

#### Hệ quả {#ac-iv-s1-n2-cor-1 .statement}

*Nếu vành A là Noether, ánh xạ $\mathfrak{p} \mapsto S^{-1}\mathfrak{p}$ là một song ánh của $\mathrm{Ass}_A(M) \cap \Phi$ lên $\mathrm{Ass}_{S^{-1}A}(S^{-1}M)$.*

Nếu A không là Noether, ánh xạ $p \mapsto S^{-1}p$ của $\mathrm{Ass}_A(M) \cap \Phi$ đến $\mathrm{Ass}_{S^{-1}A}(S^{-1}M)$ không nhất thiết là toàn ánh (Bài tập 1).

#### Mệnh đề 6 {#ac-iv-s1-prop-6 .statement}

*Cho A là một vành Noether, M một A-môđun, S một tập con nhân của A và Y là tập hợp các phần tử của $\mathrm{Ass}_A(M)$ không giao với S. Khi đó hạt nhân N của ánh xạ chính tắc $M \to S^{-1}M$ là môđun con duy nhất của M thỏa mãn các hệ thức*

$$
\mathrm{Ass}(N) = \mathrm{Ass}(M) - \Psi, \quad \mathrm{Ass}(M/N) = \Psi.
$$

Theo Mệnh đề 4 của no. 1, tồn tại một môđun con $N'$ của M thỏa mãn các hệ thức $\mathrm{Ass}(N') = \mathrm{Ass}(M) - Y$ và $\mathrm{Ass}(M/N') = \Psi$. Ta cần chứng minh $N = N'$. Xét biểu đồ giao hoán

$$
\begin{array}{ccc}
M & \xrightarrow{p} & M/N' \\
|u| & & |v| \\
S^{-1}M & \xrightarrow{S^{-1}p} & S^{-1}(M/N')
\end{array}
$$

trong đó $p, u, v$ là các đồng cấu chính tắc. Ta sẽ chứng minh rằng $S^{-1}p$ và $v$ là đơn ánh, điều này sẽ chứng minh rằng $u$ và $p$ có cùng hạt nhân và do đó $N = N'$.

Vì $\mathrm{Ass}(N') \cap \Psi = \varnothing$, mọi phần tử của $\mathrm{Ass}(N')$ đều gặp S. Khi đó $\mathrm{Ass}_{S^{-1}A}(S^{-1}N') = \varnothing$ (Hệ quả của Mệnh đề 5), do đó $S^{-1}N' = \{0\}$ (no. 1, Hệ quả 1 của Mệnh đề 2), điều này chứng minh rằng $S^{-1}p$ là đơn ánh (Chương II, §2, no. 4, Định lý 1). Mặt khác, nếu $x$ thuộc hạt nhân K của $v$, thì $\mathrm{Ann}(x) \cap S \neq \varnothing$ (Chương II, §2, no. 2, Mệnh đề 4); do đó $\mathrm{Ass}(K) = \varnothing$ vì $\mathrm{Ass}(K) \subset \mathrm{Ass}(M/N') = \Psi$; ta suy ra rằng $K = \{0\}$ (no. 1, Hệ quả 1 của Mệnh đề 2) và $v$ là đơn ánh.

### 3. CÁC QUAN HỆ VỚI GIÁ

Cho M là một môđun trên một vành A. Nhắc lại rằng tập hợp các iđêan nguyên tố $\mathfrak{p}$ của A sao cho $M, \neq 0$ được gọi là giá của M và được ký hiệu là $\operatorname{Supp}(M)$ (Chương II, § 4, no. 4, Định nghĩa 5).

#### Mệnh đề 7 {#ac-iv-s1-prop-7 .statement}

Cho A là một vành và M là một A-môđun.

(i) Mọi iđêan nguyên tố $\mathfrak{p}$ của A chứa một phần tử $\in \operatorname{Ass}(M)$ đều thuộc $\operatorname{Supp}(M)$.

(ii) Ngược lại, nếu A là Noether, mọi iđêan $\mathfrak{p} \in \operatorname{Supp}(M)$ đều chứa một phần tử $\in \operatorname{Ass}(M)$.

Nếu $\mathfrak{p}$ chứa một phần tử $q$ của $\operatorname{Ass}(M)$, thì $q \cap (A - \mathfrak{p}) = \varnothing$ và do đó, nếu ta viết $S = A - \mathfrak{p}$, $S^{-1}\mathfrak{p}$ là một iđêan nguyên tố liên kết với $S^{-1}M = M$, (no. 2, Mệnh đề 5) và *a fortiori* $M, \# 0$, do đó $\mathfrak{p} \in \operatorname{Supp}(M)$. Ngược lại, nếu A là Noether, thì A cũng là Noether, (Chương II, § 2, no. 4, Hệ quả 2 của Mệnh đề 10). Nếu $M_{\mathfrak{p}} \neq 0$, thì $\operatorname{Ass}_{A_{\mathfrak{p}}}(M_{\mathfrak{p}}) \neq 0$ (no. 1, Hệ quả 1 của Mệnh đề 2) và do đó tồn tại $q \in \operatorname{Ass}_A(M)$ sao cho $q \cap (A - \mathfrak{p}) = \varnothing$ (no. 2, Hệ quả của Mệnh đề 5).

#### Hệ quả 1 {#ac-iv-s1-prop-7-cor-1 .statement}

Nếu M là một môđun trên một vành Noether, thì $\operatorname{Ass}(M) \subset \operatorname{Supp}(M)$ và hai tập hợp này có cùng các phần tử cực tiểu.

#### Hệ quả 2 {#ac-iv-s1-prop-7-cor-2 .statement}

Căn lũy linh của một vành Noether A là giao của các iđêan $\mathfrak{p} \in \operatorname{Ass}(A)$.

Ta biết rằng căn lũy linh của A là giao của các phần tử cực tiểu của $\operatorname{Spec}(A) = \operatorname{Supp}(A)$ (Chương II, § 2, no. 6, Mệnh đề 13).

### 4. TRƯỜNG HỢP CÁC MÔĐUN SINH HỮU HẠN TRÊN MỘT VÀNH NOETHER

#### Định lý 1 {#ac-iv-s1-thm-1 .statement}

Cho A là một vành Noether và M là một A-môđun hữu hạn sinh. Tồn tại một chuỗi hợp thành $(M_i)_{0 \leq i \leq n}$ của M sao cho, với $0 \leq i \leq n - 1$, $M_i / M_{i+1}$ là đẳng cấu với $A / \mathfrak{p}_i$, trong đó $\mathfrak{p}_i$ là một iđêan nguyên tố của A.

Gọi $\mathcal{G}$ là tập hợp các môđun con của M có một chuỗi hợp thành với tính chất của mệnh đề. Vì $\mathcal{G}$ không rỗng (vì $\{0\}$ thuộc $\mathcal{G}$) và M là Noether, $\mathcal{G}$ có một phần tử cực đại N. Nếu $M \neq N$, thì $M/N \neq 0$ và do đó $\operatorname{Ass}(M/N) \neq \varnothing$ (no. 1, Hệ quả 1 của Mệnh đề 2); vì thế $M/N$ chứa một môđun con $N'/N$ đẳng cấu với một A-môđun có dạng $A/\mathfrak{p}$, trong đó $\mathfrak{p}$ là nguyên tố; khi đó theo định nghĩa $N' \in \mathcal{G}$, điều này mâu thuẫn với đặc trưng cực đại của N. Khi đó tất yếu $N = M$.

#### Định lý 2 {#ac-iv-s1-thm-2 .statement}

Cho M là một môđun hữu hạn sinh trên một vành Noether A và $(M_i)_{0 \leq i \leq n}$ là một chuỗi hợp thành của M sao cho, với $0 \leq i \leq n - 1$, $M_i / M_{i+1}$ là đẳng cấu với $A / \mathfrak{p}_i$ trong đó $\mathfrak{p}_i$ là một iđêan nguyên tố của A. Khi đó

(4)
$$
\operatorname{Ass}(M) \subset \{\mathfrak{p}_0, \ldots, \mathfrak{p}_{n-1}\} \subset \operatorname{Supp}(M);
$$

các phần tử cực tiểu của ba tập hợp này là như nhau và trùng nhau với các phần tử cực tiểu của tập hợp các iđêan nguyên tố chứa Ann(M).

Sự chứa $\operatorname{Ass}(M) \subset \{p_0, \ldots, p_{n-1}\}$ suy ra ngay lập tức từ các Mệnh đề 1 và 3 của no. 1. Với $0 \leq i \leq n - 1$,

$$
p_i \in \operatorname{Supp}(A/p_i) = \operatorname{Supp}(M_i/M_{i+1})
$$

(Chương II, § 4, no. 4, Ví dụ), do đó $p_i \in \operatorname{Supp}(M_i) \subset \operatorname{Supp}(M)$ (Chương II, § 4, no. 4, Mệnh đề 16), điều này chứng minh sự chứa

$$
\{p_0, \ldots, p_{n-1}\} \subset \operatorname{Supp}(M).
$$

Hệ quả 1 của Mệnh đề 7 trong no. 3 cho thấy $\operatorname{Ass}(M)$ và $\operatorname{Supp}(M)$ có cùng các phần tử cực tiểu và (4) cho thấy chúng chính là các phần tử cực tiểu của $\{p_0, \ldots, p_{n-1}\}$. Khẳng định cuối cùng khi đó suy ra từ Chương II, § 4, no. 4, Mệnh đề 17.

#### Hệ quả {#ac-iv-s1-n4-cor-1 .statement}

*Nếu M là một môđun hữu hạn sinh trên một vành Noether, thì $\operatorname{Ass}(M)$ là hữu hạn.*

Dưới các điều kiện của Định lý 2, tập hợp $\{p_0, \ldots, p_{n-1}\}$ không nhất thiết được xác định duy nhất bởi M; đặc biệt nó có thể phân biệt với $\operatorname{Ass}(M)$ (Bài tập 6).

#### Mệnh đề 8 {#ac-iv-s1-prop-8 .statement}

*Cho A là một vành Noether, a là một iđêan của A và M là một A-môđun hữu hạn sinh. Các điều kiện sau là tương đương:*

(a) *có một phần tử x $\# O$ của M sao cho $ax = 0$.*

(b) *với mọi $a \in a$, có một phần tử x $\neq O$ của M sao cho $ax = 0$;*

(c) *có một $p \in \operatorname{Ass}(M)$ sao cho $a \subset p$.*

Rõ ràng (a) kéo theo (b). Theo no. 1, Hệ quả 2 của Mệnh đề 2, điều kiện (b) có nghĩa là iđêan a được chứa trong hợp của các iđêan nguyên tố liên kết với M và do đó trong một trong chúng vì $\operatorname{Ass}(M)$ là hữu hạn (Chương 11, § 1, no. 1, Mệnh đề 2); do đó (b) kéo theo (c). Cuối cùng, nếu có $p \in \operatorname{Ass}(M)$ sao cho $a \subset p$, p là linh hóa tử của một phần tử $x \neq 0$ của M (no. 1, Định nghĩa 1) và $ax = 0$; do đó (c) kéo theo (a).

#### Mệnh đề 9 {#ac-iv-s1-prop-9 .statement}

*Cho A là một vành Noether, a là một iđêan của A và M là một A-môđun hữu hạn sinh. Để tồn tại một số nguyên $n > 0$ sao cho $a^n M = 0$, điều kiện cần và đủ là a được chứa trong giao của các iđêan nguyên tố liên kết với M.*

Giao này cũng là giao của các phần tử cực tiểu của $\operatorname{Supp}(M)$ (no. 3, Hệ quả 1 của Mệnh đề 7) và nói rằng a được chứa trong giao này tương đương với nói rằng $V(a) \supset \operatorname{Supp}(M)$ theo ký hiệu của Chương II, § 4; kết luận khi đó suy ra từ Chương 11, § 4, no. 4, Hệ quả 2 của Mệnh đề 17.

#### Định nghĩa 2 {#ac-iv-s1-def-2 .statement}

Cho một $A$-môđun $M$, một tự đồng cấu $u$ của $M$ được gọi là gần lũy linh nếu, với mọi $x \in M$, tồn tại một số nguyên $n(x) > 0$ sao cho $u^{n(x)}(x) = 0$.

Nếu $M$ sinh hữu hạn, mọi tự đồng cấu gần lũy linh đều lũy linh.

#### Hệ quả {#ac-iv-s1-n4-cor-2 .statement}

Cho $A$ là một vành Noether. $M$ là một $A$-môđun và $a$ là một phần tử của $A$. Để đồng cấu $a_M : x \mapsto ax$ của $M$ là gần lũy linh, điều kiện cần và đủ là $a$ thuộc mọi iđêan của $\operatorname{Ass}(M)$.

Điều kiện của mệnh đề tương đương với nói rằng với mọi $x \in M$ tồn tại $n(x) > 0$ sao cho $(Aa)^{n(x)}(Ax) = 0$; theo Mệnh đề 9 điều này cũng có nghĩa là $a$ thuộc tất cả các iđêan nguyên tố liên kết với môđun con $Ax$ của $M$; hệ quả khi đó suy ra từ sự kiện rằng $\operatorname{Ass}(M)$ là hợp của các $\operatorname{Ass}(Ax)$ khi x chạy qua M (no. 1, công thức (1)).

#### Mệnh đề 10 {#ac-iv-s1-prop-10 .statement}

Cho $A$ là một vành Noether, $E$ là một $A$-môđun hữu hạn sinh và $F$ là một $A$-môđun. Khi đó

$$
\operatorname{Ass}(\operatorname{Hom}_A(E, F)) = \operatorname{Ass}(F) \cap \operatorname{Supp}(E).
$$

Theo giả thiết, $E$ đẳng cấu với một A-môđun có dạng $A^n/R$, do đó $\operatorname{Hom}_A(E, F)$ đẳng cấu với một môđun con của $\operatorname{Hom}_A(A^n, F)$ và môđun sau đẳng cấu với $F^n$; khi đó, $\operatorname{Ass}(F^n) = \operatorname{Ass}(F)$ (no. 1, Hệ quả 1 của Mệnh đề 3); do đó $\operatorname{Ass}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Ass}(F)$. Mặt khác,

$$
\operatorname{Supp}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Supp}(E):
$$

với mọi iđêan nguyên tố $p$ của $A$, $\operatorname{Hom}_{A_p}(E_p, F_p)$ đẳng cấu với $(\operatorname{Hom}_A(E, F))_p$ (Chương 11, § 2, no. 7, Mệnh đề 19), do đó mệnh đề của ta được suy ra ngay lập tức; rồi từ Định lý 2 ta kết luận rằng

$$
\operatorname{Ass}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Supp}(E).
$$

Ngược lại, cho $p$ là một iđêan nguyên tố của $A$ thuộc $\operatorname{Ass}(F) \cap \operatorname{Supp}(E)$. Theo định nghĩa, $F$ chứa một môđun con đẳng cấu với $A/p$. Mặt khác, vì $E$ sinh hữu hạn và $E, \neq 0$, ta biết tồn tại một đồng cấu $w \neq 0$ từ $E$ vào $A/p$ (Chương II, § 4, no. 4, Mệnh đề 20). Vì tồn tại một đơn cấu $j$ từ $A/p$ vào $F$, $j \circ w \in \operatorname{Hom}(E, F)$ và $j \circ w \neq 0$. Mặt khác, quan hệ $aw = 0$ với một $a \in A$ nào đó tương đương với $a \in p$, vì linh hóa tử của mọi phần tử $\neq 0$ của $A/p$ đều là $p$; do đó chắc chắn $p \in \operatorname{Ass}(\operatorname{Hom}_A(E, F))$.

### Bài tập {#ac-iv-s1-exercises}

Xem [các bài tập của § 1](exercises/s1/).
