---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 2
section_title: Primary decomposition
lang: vi
source: ac-i-vii
book_pages: 267-282, 290-301
pdf_pages: 0287-0302, 0310-0321
extraction: ocr
subsections:
    - "no": 1
      title: PRIMARY S BMODULES
      page: 267
      pdf_page: 287
    - "no": 2
      title: THE EXISTENCE OF A PRIMARY DECOMPOSITION
      page: 270
      pdf_page: 290
    - "no": 3
      title: UNIQUENESS PROPERTIES IN THE PRIMARY DECOMPOSITION
      page: 270
      pdf_page: 290
    - "no": 4
      title: THE LOCALIZATION OF A PRIMARY DECOMPOSITION
      page: 272
      pdf_page: 292
    - "no": 5
      title: RINGS AND MODULES OF FINITE LENGTH
      page: 274
      pdf_page: 294
    - "no": 6
      title: PRIMARY DECOMPOSITION AND EXTENSION OF SCALARS
      page: 279
      pdf_page: 299
statements: 39
exercises: 28
content_sha256: 5050cc6d89849d79deb5094fe9dba80a9328f7bf2dacb3ec325f44e5af8b231e
translated_from: content/en/ac/IV/02_s2_primary_decomposition.md
source_content_sha256: ec4d6e9f0689ebac0dfdea15b3a61e409c2f05eda1aaf2d6890f55706fd47486
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-4cde209c
glossary_version: 34
glossary_terms_sha256: ab1cb42338ff678cd97f1e149c9642a8869d85a24b6c8d0d602f21436bbb31ea
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 2. PHÂN TÍCH NGUYÊN SƠ

### 1. MÔĐUN CON NGUYÊN SƠ

#### Mệnh đề 1 {#ac-iv-s2-prop-1 .statement}

Cho $A$ là một vành Noether và $M$ là một $A$-môđun. Các điều kiện sau là tương đương:
(a) $\operatorname{Ass}(M)$ chỉ gồm một phần tử duy nhất.

(b) $M \neq 0$ và mọi phép vị tự của $M$ hoặc là đơn ánh hoặc gần lũy linh ($\S 1$, no. 4). *Nếu* các điều kiện này được thỏa mãn và $p$ là tập hợp các $a \in A$ sao cho phép vị tự $a_M$ là gần lũy linh, thì $\operatorname{Ass}(M) = \{p\}$.

Điều này suy ra ngay lập tức từ $\S 1$, no. 4, Hệ quả của Mệnh đề 9 và no. 1, Hệ quả 2 của Mệnh đề 2.

#### Định nghĩa 1 {#ac-iv-s2-def-1 .statement}

*Cho $A$ là một vành Noether, $N$ là một $A$-môđun và $Q$ là một môđun con của $N$. *Nếu* môđun $M = N/Q$ thỏa mãn các điều kiện của Mệnh đề 1, thì $Q$ được gọi là *p-nguyên sơ đối với* $N$ (hoặc *trong* $N$).

Khi không có sự nhập nhằng, ta sẽ đơn giản nói rằng $Q$ là "p-nguyên sơ" hoặc "nguyên sơ"; rõ ràng với mọi môđun con $N' \neq Q$ của $N$ chứa $Q$, $Q$ là p-nguyên sơ trong $N'$.

Định nghĩa 1 đặc biệt áp dụng cho trường hợp $N = A$; khi đó các môđun con của $N$ là các *iđêan* của $A$ và do đó một iđêan $q$ của $A$ được gọi là *nguyên sơ* nếu $\operatorname{Ass}(A/q)$ chỉ có một phần tử duy nhất hoặc, điều tương đương, nếu $A \neq q$ và mọi ước của không trong vành $A/q$ đều là *lũy linh*. Nếu $q$ là p-nguyên sơ, từ Định nghĩa 1 suy ra rằng $p$ là *căn* (Chương II, $\S 2$, no. 6) của iđêan $q$.

#### Nhận xét {#ac-iv-s2-n1-rem-1 .statement}

Cho $q$ là một môđun con p-nguyên sơ của một $A$-môđun $N$. Nếu $N/Q$ là *sinh hữu hạn*, tồn tại một số nguyên $k > 0$ sao cho $p^k N \subset Q$ theo $\S 1$, no. 4, Mệnh đề 9.

*Ví dụ*

#### Ví dụ 1 {#ac-iv-s2-n1-exa-1 .statement}

Nếu $p$ là một iđêan nguyên tố của $A$, thì $p$ là p-nguyên sơ ($\S 1$, no. 1, Mệnh đề 1).

#### Ví dụ 2 {#ac-iv-s2-n1-exa-2 .statement}

Cho $q$ là một iđêan của $A$ sao cho tồn tại *một iđêan nguyên tố duy nhất* $m$ (nhất thiết là cực đại) chứa $q$; khi đó, nếu $M$ là một $A$-môđun sao cho $qM \neq M$, thì $qM$ là *m-nguyên sơ* đối với $M$. Mọi phần tử của $\operatorname{Ass}(M/qM)$ đều chứa $q$, do đó bằng $m$ và $\operatorname{Ass}(M/qM) \neq 0$ ($\S 1$, no. 1, Hệ quả 1 của Mệnh đề 2). Đặc biệt $q$ là một iđêan *m-nguyên sơ* trong $A$.

#### Ví dụ 3 {#ac-iv-s2-n1-exa-3 .statement}

Cho $m$ là một iđêan *cực đại* của $A$; khi đó các iđêan m-nguyên sơ là các iđêan $q$ của $A$ sao cho tồn tại một số nguyên $n \geq 1$ thỏa mãn $m^n \subset q \subset m$. Vì nếu $m^n \subset q \subset m$, thì $m$ là iđêan nguyên tố duy nhất chứa $q$ (Chương 11, $\S 1$, no. 1, Hệ quả của Mệnh đề 1) và kết luận suy ra từ *Ví dụ 2*; ngược lại, nếu $q$ là m-nguyên sơ, $m$ là căn của $q$ và do đó tồn tại $n \geq 1$ sao cho $m^n \subset q$ (Chương II, $\S 2$, no. 6, Mệnh đề 15).

#### Ví dụ 4 {#ac-iv-s2-n1-exa-4 .statement}

Trong một *miền iđêan chính* $A$, các iđêan nguyên sơ là $(0)$ và các iđêan có dạng $Ap^n$, trong đó $p$ là một phần tử cực biên và $n \geq 1$; điều này suy ra ngay lập tức từ *Ví dụ 3*.

#### Ví dụ 5 {#ac-iv-s2-n1-exa-5 .statement}

Các lũy thừa của bất kỳ iđêan nguyên tố nào không nhất thiết là các iđêan nguyên sơ (Bài tập 1). Mặt khác, tồn tại các iđêan nguyên sơ không phải là các lũy thừa của các iđêan nguyên tố (Bài tập 1).

#### Mệnh đề 2 {#ac-iv-s2-prop-2 .statement}

Cho M là một môđun trên một vành Noether, p là một iđêan nguyên tố của A và $(\mathcal{Q}_i)_{i \in I}$ là một họ hữu hạn không rỗng các môđun con của M là p-nguyên sơ đối với M. Khi đó $\bigcap_{i \in I} \mathcal{Q}_i$ là p-nguyên sơ đối với M.

$M / (\bigcap_{i \in I} \mathcal{Q}_i)$ đẳng cấu với một môđun con $\neq 0$ của tổng trực tiếp $\bigoplus_{i \in I} (M / \mathcal{Q}_i)$. Khi đó

$$
\operatorname{Ass}\left( \bigoplus_{i \in I} (M / \mathcal{Q}_i) \right) = \bigcup_{i \in I} \operatorname{Ass}(M / \mathcal{Q}_i) = \{p\}
$$

(§ 1, no. 1, Hệ quả 1 của Mệnh đề 3). Do đó $\operatorname{Ass}\left(M / (\bigcap_{i \in I} \mathcal{Q}_i)\right) = \{p\}$ (§ 1, no. 1, Mệnh đề 3 và Hệ quả 1 của Mệnh đề 2).

#### Mệnh đề 3 {#ac-iv-s2-prop-3 .statement}

Cho A là một vành Noether, S là một tập con nhân của A, p là một iđêan nguyên tố của A, M là một A-môđun, N là một môđun con của M và $i = i_A^S$ là ánh xạ chính tắc từ M đến $S^{-1}M$.

(i) Giả sử rằng $p \cap S \neq \varnothing$. Nếu N là p-nguyên sơ đối với M, thì $S^{-1}N = S^{-1}M$.

(ii) Giả sử rằng $p \cap S = \varnothing$. Để N là p-nguyên sơ đối với M, điều kiện cần và đủ là N có dạng $i_1(N')$, trong đó $N'$ là một môđun con của $S^{-1}A$ của $S^{-1}M$ và là $(S^{-1}p)$-nguyên sơ đối với $S^{-1}M$; khi đó $N' = S^{-1}N$.

(i) Nếu $p \cap S \neq \varnothing$ và N là p-nguyên sơ đối với M, thì

$$
\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \varnothing
$$

(§ 1, no. 2, Hệ quả của Mệnh đề 5) và do đó $S^{-1}(M/N) = 0$ (§ 1, no. 1, Hệ quả 1 của Mệnh đề 2), do đó $S^{-1}M/S^{-1}N = 0$.

(ii) Giả sử rằng $p \cap S = \varnothing$. Nếu N là p-nguyên sơ đối với M, thì $\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \{S^{-1}p\}$ (§ 1, no. 2, Hệ quả của Mệnh đề 5) và do đó môđun con $N' = S^{-1}N$ của $S^{-1}M$ là $(S^{-1}p)$-nguyên sơ; hơn nữa, nếu $s \in S$ và $m \in M$ sao cho $sm \in N$, thì $m \in N$, vì phép vị tự với tỉ số s trong M/N là đơn ánh, do đó $N = i_1(N')$ (Chương II, § 2, no. 4, Mệnh đề 10). Ngược lại, cho $N'$ là một môđun con của $S^{-1}M$ là $(S^{-1}p)$-nguyên sơ đối với $S^{-1}M$; ta viết $N = i_1(N')$; khi đó $N' = S^{-1}N$ (Chương II, § 2, no. 4, Mệnh đề 10) và $\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \operatorname{Ass}_{S^{-1}A}((S^{-1}M)/N') = \{S^{-1}p\}$. Vì ánh xạ chính tắc $M/N \to S(M/N)$ là đơn ánh, không có iđêan nguyên tố nào của A liên kết với M/N giao với S (§ 1, no. 2, Mệnh đề 6); suy ra rằng $\operatorname{Ass}(M/N) = \{p\}$ (§ 1, no. 2, Hệ quả của Mệnh đề 5), do đó N là p-nguyên sơ đối với M.

### 2. SỰ TỒN TẠI CỦA MỘT PHÂN TÍCH NGUYÊN SƠ

#### Định nghĩa 2 {#ac-iv-s2-def-2 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun và $N$ là một môđun con của $M$. Một họ hữu hạn $(\mathcal{Q}_i)_{i \in I}$ các môđun con của $M$ là nguyên sơ đối với M và sao cho $N = \bigcap_{i \in I} \mathcal{Q}_i$ được gọi là một phân tích nguyên sơ của $N$ trong $M$.

#### Ví dụ {#ac-iv-s2-n2-exa-1 .statement}

Ta lấy $A = \mathbf{Z}$, $M = \mathbf{Z}$, $N = n\mathbf{Z}$ với một số nguyên $n > 0$. Nếu $n = p_1^{\alpha_1} \cdots p_k^{\alpha_k}$ là phân tích của $n$ thành các thừa số nguyên tố,
$$
n\mathbf{Z} = (p_1^{\alpha_1}\mathbf{Z}) \cap \ldots \cap (p_k^{\alpha_k}\mathbf{Z})
$$
là một phân tích nguyên sơ của $n\mathbf{Z}$ trong $\mathbf{Z}$ theo Ví dụ 4 của no. 1.

Do lạm dụng ngôn ngữ, quan hệ $N = \bigcap_{i \in I} \mathcal{Q}_i$ được gọi là một phân tích nguyên sơ của $N$ trong $M$. Điều này tương đương với việc nói rằng $\{0\} = \bigcap_{i \in I} (\mathcal{Q}_i/N)$ là một phân tích nguyên sơ của $\{0\}$ trong $M/N$. Nếu $(\mathcal{Q}_i)_{i \in I}$ là một phân tích nguyên sơ của $N$ trong $M$, ánh xạ chính tắc từ $M/N$ đến $\bigoplus_{i \in I} (M/\mathcal{Q}_i)$ là đơn ánh. Ngược lại, cho $N$ là một môđun con của $M$ và $f$ là một đơn ánh từ $M/N$ vào một tổng trực tiếp hữu hạn $P = \bigoplus_{i \in I} P_i$, trong đó mỗi tập hợp $\operatorname{Ass}(P_i)$ được rút gọn về một phần tử duy nhất $p_i$; gọi $f_i$ là đồng cấu $M/N \to P_i$ thu được bằng cách lấy hợp thành của $f$ với phép chiếu $P \to P_i$, và gọi $Q_i/N$ là hạt nhân của $f_i$.; khi đó các $Q_i$ khác $M$ là nguyên sơ đối với $M$ (no. 1, Định nghĩa 1) và $N = \bigcap_{i \in I} Q_i$. Hơn nữa, $\operatorname{Ass}(M/N) \subset \bigcup_{i \in I} \{p_i\}$ theo § 1, no. 1, Mệnh đề 3.

#### Định lý 1 {#ac-iv-s2-thm-1 .statement}

Cho $M$ là một môđun sinh hữu hạn trên một vành Noether và $N$ là một môđun con của $M$. Tồn tại một phân tích nguyên sơ của $N$ có dạng
$$
N = \bigcap_{p \in \operatorname{Ass}(M/N)} Q(p)
$$
trong đó, với mọi $p \in \operatorname{Ass}(M/N)$, $Q(p)$ là $p$-nguyên sơ đối với $M$.

Ta có thể thay $M$ bởi $M/N$ và do đó giả sử rằng $N = 0$. Theo § 1, no. 4, Hệ quả của Định lý 2, $\operatorname{Ass}(M)$ là hữu hạn; theo § 1, no. 1, Mệnh đề 4, với mỗi $p \in \operatorname{Ass}(M)$, tồn tại một môđun con $Q(p)$ của $M$ sao cho $\operatorname{Ass}(M/Q(p)) = \{p\}$ và $\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{p\}$. Ta viết $P = \bigcap_{p \in \operatorname{Ass}(M)} Q(p)$; với mọi $p \in \operatorname{Ass}(M)$, $\operatorname{Ass}(P) \subset \operatorname{Ass}(Q(p))$ và do đó $\operatorname{Ass}(P) = \varnothing$, điều này kéo theo $P = 0$ (§ 1, no. 1, Hệ quả 1 của Mệnh đề 2) và vì vậy chứng minh định lý.

### 3. CÁC TÍNH CHẤT VỀ TÍNH DUY NHẤT TRONG PHÂN TÍCH NGUYÊN SƠ

#### Định nghĩa 3 {#ac-iv-s2-def-3 .statement}

Cho $M$ là một môđun trên một vành Noether và $N$ là một môđun con của $M$. Một phân tích nguyên sơ $N = \bigcap_{i \in I} Q_i$ của $N$ trong $M$ được gọi là rút gọn nếu các điều kiện sau được thỏa mãn:

(a) *không tồn tại chỉ số* $i \in I$ *sao cho* $\bigcap_{j \neq i} Q_j \subset Q_i;$

(b) *nếu* $\operatorname{Ass}(M/Q_i) = \{p_i\}$, *các* $p_i$ (*i* $\in I$) *phân biệt*.

Từ mỗi phân tích nguyên sơ $N = \bigcap_{i \in I} Q_i$ của $N$ trong $M$ có thể suy ra một phân tích nguyên sơ *rút gọn* của $M$ trong $N$ như sau: cho $J$ là một phần tử cực tiểu của tập hợp các tập con $I'$ của $I$ sao cho $N = \bigcap_{i \in I'} Q_i$. Rõ ràng $(Q_i)_{i \in J}$ thỏa mãn điều kiện (a). Khi đó cho $\Phi$ là tập hợp các $p_i$ với $i \in J$; với mọi $p \in \Phi$, cho $H(p)$ là tập hợp các $i \in J$ sao cho $p_i = p$ và cho $Q(p) = \bigcap_{i \in H(p)} Q_i$; suy ra từ Mệnh đề 2 của no. 1 rằng $Q(p)$ là $p$-nguyên sơ đối với $M$; hơn nữa $N = \bigcap_{p \in \Phi} Q(p)$ và họ $Q((p))_{p \in \Phi}$ do đó là một phân tích nguyên sơ rút gọn của $N$ trong $M$.

Ta sẽ thấy rằng phân tích nguyên sơ được xác định trong chứng minh của Định lý 1 của no. 2 là *rút gọn*; điều này suy ra từ mệnh đề sau:

#### Mệnh đề 4 {#ac-iv-s2-prop-4 .statement}

*Cho* $M$ *là một môđun trên một vành Noether, N một môđun con của M, $N = \bigcap_{i \in I} Q_i$ *là một phân tích nguyên sơ của N trong M và, với mọi* $i \in I$, *cho* $\{p_i\} = \operatorname{Ass}(M/Q_i)$. *Để phân tích này là rút gọn, điều kiện cần và đủ là các* $p_i$ *phân biệt và thuộc* $\operatorname{Ass}(M/N)$; *khi đó*

(2)
$$
\operatorname{Ass}(M/N) = \bigcup_{i \in I} \{p_i\}
$$

(3)
$$
\operatorname{Ass}(Q_i/N) = \bigcup_{j \neq i} \{p_j\} \quad \text{cho mọi } i \in I.
$$

Nếu điều kiện của mệnh đề được thỏa mãn, $N = \bigcap_{j \neq i} Q_j$ không thể xảy ra, vì ta sẽ suy ra rằng $\operatorname{Ass}(M/N) \subset \bigcup_{j \neq i} \{p_j\}$ (\S 1, no. 1, Hệ quả 2 của Mệnh đề 3) trái với giả thiết; phân tích nguyên sơ $(Q_i)_{i \in I}$ của $N$ khi đó chắc chắn là rút gọn. Ngược lại, $\operatorname{Ass}(M/N) \subset \bigcup_{i \in I} \{p_i\}$ luôn đúng (\S 1, no. 1, Hệ quả 2 của Mệnh đề 3); mặt khác, với mọi $i \in I$, hãy viết $P_i = \bigcap_j Q_j$; khi đó $P_i \cap Q_i = N$ và $P_i \neq N$ nếu $(Q_i)_{i \in I}$ là rút gọn, do đó $P_i/N$ khác không và đẳng cấu với môđun con $(P_i + Q_i)/Q_i$ của $M/Q_i$, do đó $\{p_i\} = \operatorname{Ass}(P_i/N)$ (\S 1, no. 1, Mệnh đề 3 và Hệ quả 1 của Mệnh đề 2); vì $P_i/N \subset M/N, p_i \in \operatorname{Ass}(M/N)$, điều này hoàn tất chứng minh tính cần thiết của điều kiện trong mệnh đề và công thức (2). Cuối cùng, vì $N = \bigcap_{j \neq i} (Q_j \cap Q_i), \operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \operatorname{Ass}(Q_i/(Q_j \cap Q_i))$ (\S 1, no. 1, Hệ quả 2 của Mệnh đề 3); nhưng $Q_i/(Q_j \cap Q_i)$ đẳng cấu với môđun con $(Q_i + Q_j)/Q_j$ của $M/Q_j$, do đó $\operatorname{Ass}(Q_i/(Q_j \cap Q_i)) \subset \{p_j\}$ và
$$
\operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \{p_j\};
$$

#### Hệ quả {#ac-iv-s2-n3-cor-1 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun, $N$ là một môđun con của $M$ và $(Q_i)_{i \in I}$ là một phân tích nguyên sơ của $N$ trong $M$. Khi đó $\mathrm{Card}(I) \geq \mathrm{Card}(\mathrm{Ass}(M/N))$; để $(Q_i)_{i \in I}$ là một phân tích nguyên sơ rút gọn, điều kiện cần và đủ là $\mathrm{Card}(I) = \mathrm{Card}(\mathrm{Ass}(M/N))$.

Suy ra từ các nhận xét đứng trước Mệnh đề 4 rằng tồn tại một phân tích nguyên sơ rút gọn $(R_j)_{j \in J}$ của $N$ trong $M$ sao cho $\mathrm{Card}(J) \leq \mathrm{Card}(I)$; mệnh đề đầu tiên khi đó suy ra từ mệnh đề thứ hai và mệnh đề sau là một hệ quả của Mệnh đề 4.

#### Mệnh đề 5 {#ac-iv-s2-prop-5 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun, $N$ là một môđun con của $M$, $N = \bigcap_{i \in I} Q_i$ là một phân tích nguyên sơ rút gọn của $N$ trong $M$ và, với mọi $i \in I$, đặt $\{p_i\} = \mathrm{Ass}(M/Q_i)$. Nếu $p_i$ là một phần tử cực tiểu của $\mathrm{Ass}(M/N)$, thì $Q_i$ bằng phần bão hòa trên $N$ đối với $p_i$ (Chương 11, § 2, no. 4) (xem Bài tập 2).

Ta hiển nhiên có thể hạn chế sự chú ý của mình vào trường hợp $N = 0$, thay thế nếu cần $M$ bởi $M/N$. Nếu $p_i$ là cực tiểu trong $\mathrm{Ass}(M)$, tập hợp các phần tử của $\mathrm{Ass}(M)$ không gặp $A - p_i$ được thu gọn thành $p_i$; khi đó mệnh đề suy ra từ công thức (3) ở trên và § 1, no. 2, Mệnh đề 6, hạt nhân của ánh xạ chính tắc $M \to M_0$, bằng phần bão hòa của 0 đối với $p_i$ (Chương 11, § 2, no. 4).

#### Nhận xét {#ac-iv-s2-n3-rem-1 .statement}

Các iđêan nguyên tố $p_i \in \mathrm{Ass}(M/N)$ không phải là các phần tử cực tiểu của tập hợp này đôi khi được gọi là các iđêan nguyên tố *nhúng* liên kết với $M/N$; nếu $M/N$ sinh hữu hạn, để $p_0 \in \mathrm{Ass}(M/N)$ là nhúng, điều kiện cần và đủ là $V(p_0)$ *không phải* là một thành phần bất khả quy của $\mathrm{Supp}(M/N)$ (Chương II, § 4, no. 3, Hệ quả 2 của Mệnh đề 14); nếu $(Q(p))_{p \in \mathrm{Ass}(M/N)}$ và $(Q'(p))_{p \in \mathrm{Ass}(M/N)}$ là hai phân tích nguyên sơ rút gọn của $N$ trong $M$, có thể xảy ra rằng $Q'(p_0) \neq Q(p_0)$ (Bài tập 24 (c)); một phân tích nguyên sơ rút gọn *chính tắc* của $N$ trong $M$ luôn có thể được xác định bằng cách áp đặt các điều kiện bổ sung lên các môđun con nguyên sơ xuất hiện trong đó (Bài tập 4).

### 4. SỰ ĐỊA PHƯƠNG HÓA CỦA MỘT PHÂN TÍCH NGUYÊN SƠ

Cho một môđun con $N$ của một môđun $M$ trên một vành Noether $A$, để đơn giản ta sẽ ký hiệu bởi $D_I(M/N)$, trong số này, tập hợp các phân tích nguyên sơ rút gọn của $N$ trong $M$ có tập chỉ số là $I$ (song ánh với $\mathrm{Ass}(M/N)$).

#### Mệnh đề 6 {#ac-iv-s2-prop-6 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun, $N$ là một môđun con của $M$ và $I = \mathrm{Ass}(M/N)$. Cho $S$ là một tập con nhân của $A$ và $J$ là tập con của $I$ gồm các chỉ số i sao cho $S \cap p_i = \varnothing$. Cho $N'$ là phần bão hòa của $N$ đối với $S$ trong $M$. Khi đó:

(i) *Nếu* $(Q_i)_{i \in I}$ *là một phần tử của* $D_I(M/N)$, *họ* $(Q_i)_{i \in J}$ *là một phần tử của* $D_J(M/N')$ *và họ* $(S^{-1}Q_i)_{i \in J}$ *là một phần tử của* $D_J(S^{-1}M/S^{-1}N)$.

(ii) *Ánh xạ* $(Q_i)_{i \in J} \to (S^{-1}Q_i)_{i \in J}$ *là một song ánh từ* $D_J(M/N')$ *lên* $D_J(S^{-1}M/S^{-1}N)$.

(iii) *Nếu* $(Q_i)_{i \in J}$ *là một phần tử của* $D_J(M/N')$ *và* $(R_i)_{i \in I}$ *là một phần tử của* $D_I(M/N)$, *họ* $(T_i)_{i \in I}$ *sao cho* $T_i = Q_i$ *với* $i \in J$ *và* $T_i = R_i$ *với* $i \in I - J$ *là một phần tử của* $D_I(M/N)$.

(i) Ta biết (no. 1, Mệnh đề 3) rằng với $i \in J, S^{-1}Q_i$ là nguyên sơ đối với $S^{-1}p_i$ và rằng với $i \in I - J, S^{-1}Q_i = S^{-1}M$; vì $S^{-1}N = \bigcap S^{-1}Q_i$ (Chương II, § 2, no. 4), nên cũng có $S^{-1}N = \bigcap_{i \in J} S^{-1}Q_i$. Các $S^{-1}p_i$ với $i \in J$ là phân biệt và tập hợp của chúng là $\operatorname{Ass}(S^{-1}M/S^{-1}N)$ ($\S 1$, no. 2, Hệ quả của Mệnh đề 5); khi đó (Mệnh đề 4) $(S^{-1}Q_i)_{i \in J}$ là một phân tích nguyên sơ rút gọn của $S^{-1}N$. Hơn nữa, $Q_i = (i_M^S)^{-1}(S^{-1}Q_i)$ (no. 1 Mệnh đề 3), do đó $N' = (i_M^S)^{-1}(S^{-1}N) = \bigcap_{i \in J} Q_i$ và $(Q_i)_{i \in J}$ hiển nhiên là một phân tích nguyên sơ rút gọn của $N'$ trong $M$.

(ii) *Vì* $S^{-1}N' = S^{-1}N$, ta có thể thay thế $N$ bởi $N'$, nghĩa là giả sử rằng $J = I$. Gọi $(P_i)_{i \in I}$ là một phân tích nguyên sơ thu gọn của $S^{-1}N$ trong $S^{-1}M$ và viết $Q_i = (i_M^S)^{-1}(P_i)$; từ no. 1, Mệnh đề 3 suy ra rằng $Q_i$ là nguyên sơ đối với $p_i$ ($i \in I$) và $(Q_i)_{i \in I}$ khi đó là một phân tích nguyên sơ thu gọn của $N$ trong $M$ theo no. 3, Hệ quả của Mệnh đề 4. Cuối cùng, vì, với mọi $i \in I$ và mọi môđun con $Q'_i$ mà $M$ là $p_i$-nguyên sơ đối với $M, Q'_i = (i_M^S)^{-1}(S^{-1}Q'_i)$ theo no. 1, Mệnh đề 3 và giả thiết $J = I$, ta thấy rằng hai ánh xạ $D_I(M/N) \to D_I(S^{-1}M/S^{-1}N)$ và $D_I(S^{-1}M/S^{-1}N) \to D_I(M/N)$ đã được xác định mà hợp của chúng là các ánh xạ đồng nhất trên $D_I(M/N)$ và $D_I(S^{-1}M/S^{-1}N)$, điều này chứng minh (ii).

(iii) Theo (i), $N' = \bigcap_{i \in J} R_i$, do đó

$$
N = N' \cap \bigcap_{i \in I - J} R_i = \left( \bigcap_{i \in J} Q_i \right) \cap \left( \bigcap_{i \in I - J} R_i \right)
$$

và từ no. 3, Hệ quả của Mệnh đề 4 suy ra ngay lập tức rằng phân tích nguyên sơ này là thu gọn.

#### Hệ quả {#ac-iv-s2-n4-cor-1 .statement}

*Các ánh xạ*

$$
D_I(M/N) \to D_J(M/N') \quad \text{và} \quad D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)
$$

*được xác định trong Mệnh đề 6 (i)* *là toàn ánh*.

Mệnh đề 6 (iii) chỉ ra rằng ánh xạ $D_I(M/N) \to D_J(M/N')$ là toàn ánh và Mệnh đề 6 (ii) khi đó chỉ ra rằng ánh xạ
$$
D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)
$$
là toàn ánh.

### 5. VÀNH VÀ MÔĐUN CÓ ĐỘ DÀI HỮU HẠN

Nếu một $A$-môđun $M$ có độ dài hữu hạn, ta sẽ ký hiệu độ dài này bởi $\operatorname{long}_A(M)$ hoặc $\operatorname{long}(M)$. Nhắc lại rằng mọi vành Artin đều là Noether (Đại số, Chương VIII, § 6, no. 5, Hệ quả 3 của Mệnh đề 12) và rằng mọi môđun sinh hữu hạn trên một vành Artin đều có độ dài hữu hạn (*loc. cit.*, Hệ quả 1 của Mệnh đề 12). Hơn nữa, mọi miền nguyên Artin đều là một trường (Đại số, Chương VIII, § 6, no. 4, Mệnh đề 9).

#### Mệnh đề 7 {#ac-iv-s2-prop-7 .statement}

*Cho $M$ là một môđun sinh hữu hạn trên một vành Noether $A$. Các tính chất sau là tương đương:*
(a) $M$ có độ dài hữu hạn.
(b) *Mọi iđêan $p \in \operatorname{Ass}(M)$ là một iđêan cực đại của $A$.*
(c) *Mọi iđêan $p \in \operatorname{Supp}(M)$ là một iđêan cực đại của $A$.*

Cho $(M_i)_{0 \leq i \leq n}$ là một chuỗi hợp thành của $M$ sao cho, với $0 \leq i \leq n - 1$, $M_i/M_{i+1}$ là đẳng cấu với $A/p_i$, trong đó $p_i$ là nguyên tố ($\S 1$, no. 4, Định lý 1). Nếu $M$ có độ dài hữu hạn, thì mỗi môđun $A$ $A/p_i$ cũng vậy, điều này suy ra rằng mỗi vành $A/p_i$ là Artin; nhưng vì $A/p_i$ là một miền nguyên, nên nó là một trường, nói cách khác $p_i$ là cực đại; ta kết luận rằng (a) suy ra (b) ($\S 1$, no. 4, Định lý 2). Điều kiện (b) suy ra (c) theo $\S 1$, no. 3, Mệnh đề 7. Cuối cùng, nếu tất cả các iđêan của $\operatorname{Supp}(M)$ đều là cực đại, thì các $p_i$ cũng vậy ($\S 1$, no. 4, Định lý 2), do đó các $A/p_i$ là các môđun $A$ đơn và $M$ có độ dài hữu hạn, điều này hoàn tất chứng minh.

#### Hệ quả 1 {#ac-iv-s2-prop-7-cor-1 .statement}

*Với mọi môđun có độ dài hữu hạn $M$ trên một vành Noether $A$, $\operatorname{Ass}(M) = \operatorname{Supp}(M)$.*

Mọi phần tử của $\operatorname{Supp}(M)$ khi đó là cực tiểu trong $\operatorname{Supp}(M)$ và kết luận suy ra từ $\S 1$, no. 3, Hệ quả 1 của Mệnh đề 7.

#### Hệ quả 2 {#ac-iv-s2-prop-7-cor-2 .statement}

*Cho $M$ là một môđun sinh hữu hạn trên một vành Noether $A$ và $p$ là một iđêan nguyên tố của $A$. Để $M_p$ là một môđun $A_p$ khác không có độ dài hữu hạn, điều kiện cần và đủ là $p$ là một phần tử cực tiểu của $\operatorname{Ass}(M)$.*

Theo $\S 1$, no. 2, Hệ quả của Mệnh đề 5, $\operatorname{Ass}_{A_p}(M_p)$ là tập hợp các iđêan $q_p$, trong đó $q$ chạy qua tập hợp các iđêan của $\operatorname{Ass}(M)$ được chứa trong $p$. Mặt khác, $p_p$ là iđêan cực đại duy nhất của $A_p$; theo Mệnh đề 7, để $M_p$ là một môđun $A_p$ có độ dài hữu hạn, điều kiện cần và đủ là không có phần tử nào của $\operatorname{Ass}(M)$ được chứa thực sự trong $p$. Mặt khác, để $M_p \neq 0$, theo định nghĩa điều kiện cần và đủ là $p \in \operatorname{Supp}(M)$ (Chương 11, § 4, no. 4), nghĩa là $p$ chứa một phần tử của $\operatorname{Ass}(M)$ ($\S 1$, no. 3, Mệnh đề 7). Điều này chứng minh hệ quả.

Nhận xét (1). Cho $M$ là một môđun sinh hữu hạn trên một vành Noether $A$; hãy để $(M_1), \ldots$ là một chuỗi hợp thành của $M$ sao cho, với $0 \leq i \leq n - 1$, $M_i / M_{i+1}$ đẳng cấu với $A/p_i$, trong đó $p_i$ là một iđêan nguyên tố của $A$ ($\S 1$, no. 4, Định lý 1). Nếu $p$ là một phần tử cực tiểu của $\operatorname{Ass}(M)$, độ dài $\operatorname{long}_{A_p}(M_p)$ bằng *số chỉ số* $i$ sao cho $p_i = p$. Vì các $(M_i)_p$ tạo thành một chuỗi hợp thành của $M$, và $(M_i)_p / (M_{i+1})_p$ đẳng cấu với $(A/p_i)_p$ và do đó đẳng cấu với $\{0\}$ nếu $p_i \neq p$ (vì $p$ là cực tiểu trong tập hợp các $p_i$ theo $\S 1$, no. 4, Định lý 2) và với $(A/p)_p$ là một trường, nếu $p_i = p$.

#### Mệnh đề 8 {#ac-iv-s2-prop-8 .statement}

*Cho $M$ là một môđun có độ dài hữu hạn trên một vành Noether $A$.*

(i) *Chỉ tồn tại một phân tích nguyên sơ duy nhất của $\{0\}$ đối với $M$ được đánh chỉ số bởi $\operatorname{Ass}(M)$ (nhất thiết rút gọn) — hãy gọi $\{0\} = \bigcap_{p \in \operatorname{Ass}(M)} Q(p)$ là phân tích này, trong đó $Q(p)$ là $p$-nguyên sơ đối với $M$.*

(ii) *Tồn tại một số nguyên $n_0$ sao cho, với mọi $n \geq n_0$ và mọi $p \in \operatorname{Ass}(M)$, $Q(p) = p^n M$.*

(iii) *Với mọi $p \in \operatorname{Ass}(M)$, ánh xạ chính tắc từ $M$ vào $M_p$ là toàn ánh và hạt nhân của nó là $Q(p)$.*

(iv) *Đơn ánh chính tắc của $M$ vào $\bigoplus_{p \in \operatorname{Ass}(M)} (M/Q(p))$ là song ánh.*

Vì mọi phần tử $p \in \operatorname{Ass}(M)$ đều là cực tiểu trong $\operatorname{Ass}(M)$ (Mệnh đề 7), mệnh đề (i) suy ra từ no. 3, Mệnh đề 5. Vì $M$ sinh hữu hạn, tồn tại $n_0$ sao cho $p^n M \subset Q(p)$ với mọi $p \in \operatorname{Ass}(M)$ và mọi $n \geq n_0$ (no. 1, *Nhận xét*); nhưng vì $p$ là một iđêan cực đại, $p^n M$ là $p$-nguyên sơ đối với $M$ (no. 1, *Ví dụ 2 và 3*) và, vì $\bigcap_{p \in \operatorname{Ass}(M)} p^n M = \{0\}$, suy ra từ (i) rằng nhất thiết $p^n M = Q(p)$ với mọi $p \in \operatorname{Ass}(M)$; do đó có (ii). Vì các $p^n$, với $p \in \operatorname{Ass}(M)$, nguyên tố cùng nhau từng đôi (Chương 11, § 1, no. 2, Mệnh đề 3), ánh xạ chính tắc $M \to \bigoplus_{p \in \operatorname{Ass}(M)} (M/p^n M)$ là toàn ánh (Chương 11, § 1, no. 2, Mệnh đề 6), do đó có (iv). Khi đó $\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{p\}$ và $\operatorname{Ass}(M/Q(p)) = \{p\}$ (no. 3, Mệnh đề 4); vì các phần tử của $\operatorname{Ass}(M)$ là các iđêan cực đại, $p$ là phần tử duy nhất của $\operatorname{Ass}(M)$ không giao với $A - p$; do đó $Q(p)$ là hạt nhân của ánh xạ chính tắc $j : M \to M_p$ ($\S 1$, no. 2, Mệnh đề 6). Nếu $s \in A - p$, phép vị tự của $M/Q(p)$ với tỉ số $s$ là đơn ánh nhờ quan hệ $\operatorname{Ass}(M/Q(p)) = \{p\}$ (no. 1, Mệnh đề 1); vì $M/Q(p)$ là Artin, phép vị tự này là song ánh (*Đại số*, Chương VIII, § 1, no. 2, Bổ đề 3). Ánh xạ chính tắc $M \to M/Q(p)$ khi đó được viết $f \circ j$, trong đó $f : M_p \to M/Q(p)$ là một đồng cấu $A$ (Chương II, § 2, no. 2, Mệnh đề 3); vì $\operatorname{Ker}(j) = \operatorname{Ker}(f \circ j) = Q(p)$, $f$ là đơn ánh; ta kết luận rằng $j$ là toàn ánh và $f$ là song ánh.

#### Hệ quả {#ac-iv-s2-n5-cor-1 .statement}

*Nếu M là một môđun có độ dài hữu hạn trên một vành Noether A, thì*

$$
\operatorname{long}_A(M) = \sum_{p \in \operatorname{Ass}(M)} \operatorname{long}_{A_p}(M_p).
$$

Điều này sẽ suy ra từ Mệnh đề 8 (iv) nếu ta chứng minh rằng

$$
\operatorname{long}_A(M/\mathcal{Q}(p)) = \operatorname{long}_{A_p}(M_p).
$$

Bây giờ, từ Mệnh đề 1 của no. 1 suy ra rằng với mọi $s \in A - p$ phép vị tự với tỉ số s trên $M/\mathcal{Q}(p)$ là đơn ánh; phép vị tự với tỉ số s trên mọi môđun con R của $M/\mathcal{Q}(p)$ do đó là đơn ánh và, vì R là Artin, nó là song ánh (*Đại số*, Chương VIII, § 2, no. 2, Bổ đề 3); ta kết luận rằng các môđun con-A của $M/\mathcal{Q}(p)$ là các ảnh qua song ánh $f : M, \to M/\mathcal{Q}(p)$ của các môđun con-A, của M, (Chương 11, § 2, no. 3), do đó có mệnh đề của ta.

#### Mệnh đề 9 {#ac-iv-s2-prop-9 .statement}

*Một vành Noether A. Các điều kiện sau là tương đương :*
(a) *A là Artin.*
(b) *Mọi iđêan nguyên tố $\mathfrak{a}$ trong A là iđêan cực đại.*
(c) *Mọi phần tử của Ass(A) là iđêan cực đại.*

*Nếu các điều kiện này được thỏa mãn, A chỉ có một số hữu hạn các iđêan nguyên tố, tất cả đều là cực đại và liên kết với A-môđun A; hơn nữa, A là một vành nửa địa phương và căn Jacobson của nó là lũy linh.*

Nói rằng A là Artin tương đương với nói rằng nó là một A-môđun có độ dài hữu hạn; do đó (a) và (c) tương đương theo Mệnh đề 7. Rõ ràng (b) kéo theo (c). Cuối cùng, (a) kéo theo (b) vì mọi miền nguyên Artin đều là một trường. Vì vậy các tính chất (a), (b) và (c) là tương đương.

Giả sử chúng được thỏa mãn. Vì mọi iđêan nguyên tố của A thuộc Supp(A) và mọi phần tử của Supp(A) chứa một phần tử của Ass(A) ($\S$ 1, no. 3, Mệnh đề 7), suy ra từ (c) rằng Ass(A) là tập hợp tất cả các iđêan nguyên tố của A; khi đó A chỉ có một số hữu hạn các iđêan nguyên tố, tất cả chúng đều là cực đại và liên kết với A-môđun A. Điều này hiển nhiên suy ra rằng A là nửa địa phương; cuối cùng, ta biết rằng căn Jacobson của một vành Artin là lũy linh (*Đại số*, Chương VIII, § 6, no. 4, Định lý 3).

*Nhận xét (2)* Các điều kiện của Mệnh đề 9 đối với một vành *Noether* A kéo theo rằng phổ của A là *hữu hạn* và *rời rạc*, do đó mọi điểm của Spec(A) đều đóng (Chương 11, § 4, no. 3, Hệ quả 6 của Mệnh đề 11). Ngược lại, đối với một vành *Noether* A, nói rằng *mọi điểm* $\mathfrak{a}$ của Spec(A) *là đóng* có nghĩa là mọi iđêan nguyên tố của A là cực đại (*loc. cit.*.) và vì thế điều kiện này tương đương với điều kiện của Mệnh đề 9.

#### Hệ quả 1 {#ac-iv-s2-prop-9-cor-1 .statement}

*Mọi vành Artin A đều đẳng cấu với hợp thành trực tiếp của một họ hữu hạn các vành địa phương Artin.*

Từ Mệnh đề 9 và Mệnh đề 8 (iii) và (iv) suy ra rằng, nếu $(\mathfrak{m}_i)_{1 \leq i \leq n}$ là họ các iđêan cực đại của $A$, thì ánh xạ chính tắc $A \to \prod_i A_{\mathfrak{m}_i}$ là song ánh.

Nhận xét (3). Hệ quả này cũng có thể suy ra từ sự kiện rằng $\operatorname{Spec}(A)$ là hữu hạn và rời rạc và Chương 11, § 4, no. 3, Mệnh đề 15.

#### Hệ quả 2 {#ac-iv-s2-prop-9-cor-2 .statement}

Cho $A$ là một vành Noether và $m$ là một iđêan của $A$. Các điều kiện sau là tương đương:

(a) $A$ là một vành nửa địa phương và $m$ là một iđêan xác định của $A$.
(b) $A$ là một vành Zariski với tôpô $m$-adic và $A/m$ là Artin.

Nếu (a) đúng, $A$ là một vành Zariski với tôpô $m$-adic (Chương III, § 3, no. 3, Ví dụ 3); hơn nữa, theo giả thiết $m$ chứa một lũy thừa của căn Jacobson $r$ của $A$, mọi iđêan nguyên tố của $A$ chứa $m$ cũng chứa $r$ (Chương II, § 1, no. 1, Mệnh đề 1); do đó nó là cực đại, vì $r$ là một giao hữu hạn của các iđêan cực đại (\emph{loc. cit.}); Mệnh đề 9 khi đó chỉ ra rằng $A/m$ là Artin. Ngược lại, nếu (b) đúng, mọi iđêan cực đại $p$ của $A$ chứa căn Jacobson của $A$ và do đó chứa $m$ (Chương III, § 3, no. 3, Mệnh đề 6); vì $A/m$ là Artin, các iđêan $p/m$ là hữu hạn về số lượng (Mệnh đề 9) và do đó $A$ chỉ có một số hữu hạn các iđêan cực đại, điều này suy ra rằng nó là nửa địa phương.

#### Hệ quả 3 {#ac-iv-s2-prop-9-cor-3 .statement}

Cho $A, A'$ là hai vành và $h$ là một đồng cấu từ $A$ đến $A'$. Giả sử rằng $A$ là nửa địa phương và Noether và rằng $A'$ là một $A$-môđun sinh hữu hạn. Khi đó vành $A'$ là nửa địa phương và Noether; nếu $m$ là một iđêan xác định của $A$, thì $mA'$ là một iđêan xác định của $A'$.

Ta biết rằng $A'$ là một vành Zariski với tôpô $mA'$-adic (Chương III, § 3, no. 3, Mệnh đề 7). Vì $A/m$ là Artin (Hệ quả 2) và $A'/mA'$ là một $(A/m)$-môđun sinh hữu hạn, $A'/mA'$ là một vành Artin, do đó $A'$ là nửa địa phương và $mA'$ là một iđêan xác định của $A'$ (Hệ quả 2).

#### Hệ quả 4 {#ac-iv-s2-prop-9-cor-4 .statement}

Cho $A$ là một vành Noether nửa địa phương đầy đủ, $m$ là một iđêan xác định của $A$, $E$ là một $A$-môđun sinh hữu hạn và $(F_n)$ là một dãy giảm các môđun con của $E$ sao cho $\bigcap_n F_n = 0$. Khi đó, với mọi $p > 0$, tồn tại $n > 0$ sao cho $F_n \subset m^p E$.

Vì $A$ là một vành Zariski, $E$ là Hausdorff và các $F_n$ đóng đối với tôpô $m$-adic. Mặt khác, $E$ là đầy đủ (Chương III, § 2, no. 12, Hệ quả 1 của Mệnh đề 16). Cuối cùng, $E/m^p E$ là một môđun sinh hữu hạn trên vành $A/m^p$, vành này là Artin (Hệ quả 2); khi đó $E/m^p E$ là một $(A/m^p)$-môđun Artin và do đó là một $A$-môđun Artin. Hệ quả được suy ra từ Chương III, § 2, no. 7, Mệnh đề 8.

#### Hệ quả 5 {#ac-iv-s2-prop-9-cor-5 .statement}

Trong một vành Noether nửa địa phương đầy đủ, mọi dãy giảm $\phi$ iđêan có giao bằng 0 là một cơ sở lọc hội tụ về 0.

Chỉ cần áp dụng Hệ quả 4 cho A-môđun $\mathbf{A}$.

#### Mệnh đề 10 {#ac-iv-s2-prop-10 .statement}

Cho $A$ là một vành Noether và $p_1, \ldots, p_n$ là các iđêan nguyên tố liên kết với A-môđun $A$, trong đó $p_i \neq p_j$ với $i \neq j$.

(i) Tập hợp $S = \bigcap_{i=1}^n (A - p_i)$ là tập hợp các phần tử không là ước của 0 trong $A$.

(ii) Nếu mọi $p_i$ là các phần tử cực tiểu của $\operatorname{Ass}(A)$, vành phân thức toàn phần $S^{-1}A$ của $A$ là Artin.

(iii) Nếu vành $A$ là thu gọn, mọi $p_i$ là các phần tử cực tiểu của $\operatorname{Ass}(A)$ (và do đó là các phần tử cực tiểu của $\operatorname{Spec}(A)$) và mỗi $A_{p_i}$ là một trường; với mỗi chỉ số $i$, đồng cấu chính tắc $S^{-1}A \to A_{p_i}$ (Chương II, § 2, no. 1, Hệ quả 1 của Mệnh đề 2) là toàn ánh và hạt nhân của nó là $S^{-1}p_i$; cuối cùng đồng cấu chính tắc từ $S^{-1}A$ đến $\prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$ là song ánh.

Sự kiện rằng $S$ là tập hợp các phần tử không là ước của 0 trong $\mathbf{A}$ đã được thấy (§ 1, no. 1, Hệ quả 3 của Mệnh đề 2). Các iđêan nguyên tố của $S^{-1}A$ có dạng $S^{-1}p$, trong đó $p$ là một iđêan nguyên tố của $A$ được chứa trong $\bigcup_{i=1}^n p_i$ (Chương 11, § 2, no. 5, Mệnh đề 10) và được chứa trong một trong các $p_i$ (Chương II, § 1, no. 1, Mệnh đề 2). Nếu $p_i$ là một phần tử cực tiểu của $\operatorname{Ass}(A)$, thì nó là một phần tử cực tiểu của $\operatorname{Spec}(A)$ (§ 1, no. 3, Hệ quả của Mệnh đề 7); nếu mỗi $p_i$ là một phần tử cực tiểu của $\operatorname{Ass}(A)$, khi đó ta thấy rằng các iđêan nguyên tố của $S^{-1}A$ là các $S^{-1}p_i$ và do đó tất cả chúng đều là cực đại, điều này chứng minh rằng $S^{-1}A$ là Artin (Mệnh đề 9).

Giả sử cuối cùng rằng vành $A$ là rút gọn. Khi đó $\bigcap_{i=1}^n p_i = \{0\}$ (§ 1, no. 3, Hệ quả 2 của Mệnh đề 7). Ta suy ra rằng $\{0\} = \bigcap_{i=1}^n p_i$ là một phân tích nguyên sơ *rút gọn* của iđêan $\{0\}$ (no. 3, Hệ quả của Mệnh đề 4); đặc biệt, không có $p_i$ nào có thể chứa một $p_j$ với chỉ số $j \neq i$ và do đó các $p_i$ đều là các phần tử cực tiểu của $\operatorname{Ass}(A)$. Khi đó vành $S^{-1}A$ là Artin theo (ii). Các $S^{-1}p_i$ là các iđêan nguyên tố liên kết với $S^{-1}A$-môđun $S^{-1}A$ (§ 1, no. 2, Hệ quả của Mệnh đề 5) và $\{0\} = S^{-1} \left( \bigcap_{i=1}^n p_i \right) = \bigcap_{i=1}^n S^{-1}p_i$ (Chương II, § 2, no. 4); vì các $S^{-1}p_i$ là phân biệt, $(S^{-1}p_i)_{1 \leq i \leq n}$ là một phân tích nguyên sơ rút gọn của $\{0\}$ trong $S^{-1}A$ (no. 3, Hệ quả của Mệnh đề 4). Mệnh đề 8 khi đó chỉ ra rằng đồng cấu chính tắcg,: $S^{-1}A \to (S^{-1}A)_{p_i}$ là toàn ánh và có hạt nhân $S^{-1}p_i$, còn đồng cấu chính tắc $S^{-1}A \to \prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$ là song ánh. Ngoài ra ta biết rằng đồng cấu chính tắc $S^{-1}A \to A$, là hợp thành của g, và một đẳng cấu $(S^{-1}A)_{S^{-1}p_i} \to A$, (Chương II, § 2, no. 3, Mệnh đề 7). Cuối cùng, từ Mệnh đề 8 suy ra rằng $(S^{-1}A)_{S^{-1}p_i}$ đẳng cấu với $S^{-1}A/S^{-1}p_i$ và do đó là một trường vì $S^{-1}p_i$ là một iđêan cực đại.

### 6. PHÂN TÍCH NGUYÊN SƠ VÀ MỞ RỘNG VÔ HẠN

Trong no. này, A và B sẽ chỉ hai vành và ta sẽ xét một đồng cấu vành $\rho : A \to B$ làm cho $B$ trở thành một đại số trên A; nhắc lại rằng, với mọi B-môđun F, $\rho_*(F)$ là nhóm giao hoán F với cấu trúc môđun được xác định bởi $a.y = \rho(a)y$ với mọi $a \in A, y \in F$.

#### Bổ đề 1 {#ac-iv-s2-lem-1 .statement}

Cho A là một vành Noether, $p$ là một iđêan nguyên tố của A, E là một A-môđun có linh hóa tử chứa một lũy thừa của $p$ và thỏa mãn $\operatorname{Ass}(E) = \{p\}$, và F là một B-môđun sao cho $\rho_*(F)$ là một A-môđun phẳng. Điều kiện $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$ khi đó kéo theo $\rho^{-1}(\mathfrak{P}) = p$.

Nếu n là sao cho $p^nE = 0$, thì $p^nB \subset \operatorname{Ann}(E \otimes_A F)$, do đó $p^nB \subset \mathfrak{P}$, điều này kéo theo $p^n \subset \rho_1(\mathfrak{P})$ và do đó $p \subset \rho_1(\mathfrak{P})$ vì $\rho_1(\mathfrak{P})$ là nguyên tố. Hơn nữa, nếu $a \in A - p$, phép vị tự h với tỉ số a trên E là đơn ánh ($\S 1$, no. 1, Hệ quả 2 của Mệnh đề 2); vì $h \otimes 1_F$ là phép vị tự $h'$ với tỉ số $\rho(a)$ trên $E \otimes_A F$ và $\rho_*(F)$ là phẳng, $h'$ là đơn ánh (Chương I, § 2, no. 2, Định nghĩa 1); điều này chứng minh rằng $\rho(a) \notin \mathfrak{P}$, do đó $\rho^{-1}(\mathfrak{P}) = p$.

#### Định lý 2 {#ac-iv-s2-thm-2 .statement}

Cho $\rho : A \to B$ là một đồng cấu vành, E là một A-môđun và F là một B-môđun sao cho $\rho_*(F)$ là một A-môđun phẳng. Khi đó

$$
\operatorname{Ass}_B(E \otimes_A F) \supset \bigcup_{p \in \operatorname{Ass}_A(E)} \operatorname{Ass}_B(F/pF).
$$

Khi A là Noether, hai vế của (5) bằng nhau.

Cho $p \in \operatorname{Ass}_A(E)$; theo định nghĩa tồn tại một dãy khớp

$$
0 \to A/p \to E.
$$

Vì F là một A-môđun phẳng, ta suy ra một dãy khớp

$$
0 \to F/pF \to E \otimes_A F
$$

do đó $\operatorname{Ass}_B(F/pF) \subset \operatorname{Ass}_B(E \otimes_A F)$, điều này chứng minh bao hàm (5).

Bây giờ giả sử A là Noether và ta hãy chứng minh bao hàm ngược lại.

Ta tiến hành theo từng giai đoạn:

(i) Trước hết, giả sử rằng E là một A-môđun sinh hữu hạn và rằng Ass_A(E) được rút gọn về một phần tử duy nhất $p$. Theo § 1, no. 4, Định lý 1 tồn tại một chuỗi hợp thành $(E_i)_{0 \leq i \leq n}$ của E sao cho $E_i/E_{i+1}$ đẳng cấu với $A/p_i$, trong đó $p_i$ là một iđêan nguyên tố của A; hơn nữa ($§ 1$, no. 4, Định lý 2 và no. 3, Mệnh đề 7) mọi $p_i$ đều chứa $p$. Vì F là một A-môđun phẳng, các $E_i \otimes_A F$ tạo thành một chuỗi hợp thành của $E \otimes_A F$ và $(E_i \otimes_A F)/(E_{i+1} \otimes_A F)$ được đồng nhất với
$$
(A/p_i) \otimes_A F = F/p_i F.
$$
Khi đó, theo $§ 1$, no. 1, Mệnh đề 3
$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=0}^{n-1} \operatorname{Ass}_B(F/p_i F).
$$
Ta biết rằng E bị triệt tiêu bởi một lũy thừa của $p$ (no. 1, Nhận xét); Bổ đề 1 khi đó chỉ ra rằng, với mọi $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$, $\rho^{-1}(\mathfrak{P}) = p$. Vì $F/p_i F$ đẳng cấu với $(A/p_i) \otimes_A F$, nên $\rho^{-1}(\mathfrak{P}') = p_i$ với mọi $\mathfrak{P}' \in \operatorname{Ass}_B(F/p_i F)$ theo Bổ đề 1, do đó $\operatorname{Ass}_B(E \otimes_A F) \cap \operatorname{Ass}(F/p_i F) = \varnothing$ nếu $p_i \neq p$, điều này chứng minh định lý trong trường hợp đang xét.

(ii) Chỉ giả sử rằng E là một A-môđun sinh hữu hạn. Gọi $p_i$ ($1 \leq i \leq n$) là các phần tử của $\operatorname{Ass}_A(E)$ và giả sử $\{0\} = \bigcap^n Q_i$ là một phân tích nguyên sơ rút gọn tương ứng (no. 3); khi đó E đẳng cấu với một môđun con của tổng trực tiếp của các $E_i = E/Q_i$ và, vì F là một A-môđun phẳng, $E \otimes_A F$ đẳng cấu với một môđun con của tổng trực tiếp các B-môđun $E_i \otimes_A F$. Ta suy ra ($§ 1$, no. 1, Mệnh đề 3 và Hệ quả 1 của Mệnh đề 3) rằng
$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=1}^n \operatorname{Ass}_B(E_i \otimes_A F).
$$
Nhưng $E_i$ là một A-môđun sinh hữu hạn sao cho $\operatorname{Ass}_A(E_i)$ được rút gọn về một phần tử duy nhất $p_i$ (no. 1, Định nghĩa 1). Theo (i), $\operatorname{Ass}_B(E_i \otimes_A F) = \operatorname{Ass}_B(F/p_i F)$, do đó có định lý trong trường hợp này.

(iii) *Trường hợp tổng quát.* B-môđun $E \otimes_A F$ là hợp của các môđun con $E' \otimes_A F$, trong đó $E'$ chạy qua tập hợp các môđun con sinh hữu hạn của A-môđun E. Nếu $\mathfrak{P}$ thuộc về $\operatorname{Ass}_B(E \otimes_A F)$, thì tồn tại một môđun con sinh hữu hạn $E'$ của E sao cho $\mathfrak{P} \in \operatorname{Ass}_B(E' \otimes_A F)$. Theo (ii), tồn tại $p \in \operatorname{Ass}_A(E')$ sao cho $\mathfrak{P} \in \operatorname{Ass}_B(F/pF)$; vì $\operatorname{Ass}_A(E') \subset \operatorname{Ass}_A(E)$, điều này hoàn tất chứng minh Định lý 2.

#### Hệ quả 1 {#ac-iv-s2-thm-2-cor-1 .statement}

*Nếu A là Noether và $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$, thì $\rho^{-1}(\mathfrak{P}) \in \operatorname{Ass}_A(E)$ và $\rho^{-1}(\mathfrak{P})$ là iđêan nguyên tố $p$ duy nhất của A sao cho $\mathfrak{P} \in \operatorname{Ass}_B(F/pF)$.*

#### Hệ quả 2 {#ac-iv-s2-thm-2-cor-2 .statement}

Giả sử rằng $A$ và $B$ là Noether và rằng $B$ là một $A$-môđun phẳng. Cho $p$ là một iđêan nguyên tố của $A$, $Q \subset E$ là một môđun con $p$-nguyên sơ và $\mathfrak{P}$ là một iđêan nguyên tố của $B$. Để $Q \otimes_A B$ là một môđun con $q$-nguyên sơ của $E \otimes_A B$, điều kiện cần và đủ là $pB$ là một 'iđêan p-nguyên sơ' của $B$.

Ta áp dụng Định lý 2 cho $A$-môđun $E/Q$ và $B$-môđun $B$; khi đó $\operatorname{Ass}_A(E/Q) = \{p\}$ và $(E/Q) \otimes_A B$ đẳng cấu với $(E \otimes_A B)/(Q \otimes_A B)$ và do đó $\operatorname{Ass}_B((E \otimes_A B)/(Q \otimes_A B)) = \operatorname{Ass}_B(B/pB)$. Nói rằng $Q \otimes_A B$ là $\mathfrak{P}$-nguyên sơ trong $E \otimes_A B$ do đó có nghĩa là $\operatorname{Ass}_B(B/pB)$ được thu gọn thành $\mathfrak{P}$, do đó có hệ quả.

#### Nhận xét {#ac-iv-s2-n6-rem-1 .statement}

Giả sử rằng $A$ và $B$ là Noether. Cho $\mathfrak{P}$ là một iđêan nguyên tố của $B$ và đặt $p = \overline{\rho}^{-1}(\mathfrak{P})$; ta viết $S = A - p$ và đặt $k(p) = S^{-1}(A/p)$ là trường các phân thức của $A/p$. Vì $\mathfrak{P}$ chứa $pB$, $\mathfrak{P}/pB$ là một iđêan nguyên tố của $B/pB$. Nếu $\rho'$ là đồng cấu hợp thành $A \xrightarrow{\rho} B \to B/pB$, ta biết rằng $S^{-1}(B/pB)$ được đồng nhất với vành $(\rho'(S))^{-1}(B/pB)$ và $\mathfrak{P}' = S^{-1}(\mathfrak{P}/pB)$ với một iđêan của vành này (Chương II, § 2, no. 2, Mệnh đề 6); vì $\mathfrak{P}/pB$ không gặp $\rho'(S)$, $\mathfrak{P}'$ là một iđêan nguyên tố của $S^{-1}(B/pB)$ (Chương 11, § 2, no. 5, Mệnh đề 11); hơn nữa có các đẳng cấu chính tắc giữa $S^{-1}(B/pB)$, $S^{-1}((A/p) \otimes_A B)$ và $(S^{-1}(A/p)) \otimes_A B = k(p) \otimes_A B$; tương tự $S^{-1}(F/pF)$ được đồng nhất một cách chính tắc với $k(p) \otimes_A F$. Như vậy, dưới các giả thiết của Định lý 2, *để có* $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$, *điều kiện cần và đủ là* $p \in \operatorname{Ass}_A(E)$ và
$$
\mathfrak{P}' \in \operatorname{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F).
$$
Vì theo Định lý 2 và Hệ quả 1 của nó, điều này quy về việc kiểm tra rằng các điều kiện
$$
\text{``}\mathfrak{P} \in \operatorname{Ass}_B(F/pF)\text{''} \quad \text{and} \quad \text{``}\mathfrak{P}' \in \operatorname{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F)\text{''}
$$
là tương đương; nhưng, vì $B$ là Noether, điều này suy ra từ § 1, no. 2, Hệ quả của Mệnh đề 5 và các đồng nhất ở trên.

#### Mệnh đề 11 {#ac-iv-s2-prop-11 .statement}

Giả sử rằng $A$ và $B$ là Noether và rằng $B$ là một $A$-môđun phẳng. Cho $E$ là một $A$-môđun và $E'$ là một môđun con của $E$ sao cho, với mọi iđêan $p \in \operatorname{Ass}_A(E/E')$, $pB$ là một iđêan nguyên tố của $B$ hoặc bằng $B$. Gọi $E' = \bigcap_{p \in \operatorname{Ass}(E/E')} Q(p)$ là một phân tích nguyên sơ thu gọn của $E'$ trong $E$, $Q(p)$ là $p$-nguyên sơ với mọi $p \in \operatorname{Ass}(E/E')$.
(i) *Nếu* $p \in \operatorname{Ass}(E/E')$ *và* $pB = B$, *thì* $Q(p) \otimes_A B = E \otimes_A B$.
(ii) *Nếu* $p \in \operatorname{Ass}(E/E')$ *và* $pB$ *là nguyên tố*, $Q(p)$ *là* $pB$*-nguyên sơ* *trong* $E \otimes_A B$.
(iii) *Nếu* $\Phi$ *là tập hợp các* $\mathfrak{p} \in \operatorname{Ass}(E/E')$ *sao cho* $pB$ *là nguyên tố*, *thì*
$$
E' \otimes_A B = \bigcap_{p \in \Phi} (Q(p) \otimes_A B)
$$
*và quan hệ này là một phân tích nguyên sơ thu gọn của* $E' \otimes_A B$ *trong* $E \otimes_A B$.

Nếu $pB = B$, Định lý 2 áp dụng cho $E/\mathbf{Q}(p)$ và $B$ cho thấy rằng
$$
\operatorname{Ass}_B((E/\mathbf{Q}(p)) \otimes_A B) = \varnothing
$$
và, vì $B$ là Noether và là một $A$-môđun phẳng, ta kết luận (\S 1, no. 1, Hệ quả 1 của Mệnh đề 2) rằng $\mathbf{Q}(p) \otimes_A B = E \otimes_A B$. Mệnh đề (ii) suy ra từ Hệ quả 2 của Định lý 2, lấy $\mathfrak{P} = pB$. Cuối cùng, quan hệ $E' \otimes_A B = \bigcap_{p \in \Phi} (\mathbf{Q}(p) \otimes_A B)$ suy ra từ sự kiện rằng $B$ là một $A$-môđun phẳng (Chương I, \S 2, no. 6, Mệnh đề 6); vì $p = \overline{\rho}^{-1}(pB)$ với $p \in \Phi$ (Bổ đề 1), $pB \neq p'B$ đối với hai iđêan phân biệt $p, p'$ của tập hợp $\Phi$; mặt khác,
$$
\operatorname{Ass}((E \otimes_A B)/(E' \otimes_A B)) = \Phi
$$
theo Định lý 2; ta kết luận từ no. 3, Mệnh đề 4 rằng
$$
E' \otimes_A B = \bigcap_{p \in \Phi} (\mathbf{Q}(p) \otimes_A B)
$$
là một phân tích nguyên sơ thu gọn.

#### Hệ quả {#ac-iv-s2-n6-cor-1 .statement}

*Giả sử rằng* $pB$ *là nguyên tố đối với mọi* $p \in \operatorname{Ass}_A(E/E')$. *Khi đó, nếu* $p_1, \ldots, p_n$ *là các phần tử cực tiểu của* $\operatorname{Ass}_A(E/E')$, *thì* $p_iB$ *là các phần tử cực tiểu của*
$$
\operatorname{Ass}_A((E \otimes_A B)/(E' \otimes_A B)).
$$
Điều này suy ra từ Mệnh đề 11 rằng trong trường hợp này $p_iB \neq p_jB$ với $i \# j$.

*Ví dụ*
(1) Ta lấy $B = S^{-1}A$, trong đó $S$ là một tập con nhân của $A$; nếu $A$ là Noether, các giả thiết của Mệnh đề 11 được thỏa mãn và ta thu lại một phần của Mệnh đề 6 của no. 4.
(2) Cho $A$ là một vành Noether, $m$ một iđêan của $A$ và $B$ là bao hoàn Hausdorff của $A$ đối với tôpô $m$-adic; khi đó $B$ là một $A$-môđun phẳng và Định lý 2 có thể được áp dụng với $F = B$; nhưng nói chung các giả thiết của Mệnh đề 11 không được thỏa mãn đối với các iđêan nguyên tố của $A$ (Chương III, \S 2, Bài tập 15 (b)).
(3) Cho $A$ là một vành Noether và $B$ là đại số đa thức $A[X_1, \ldots, X_n]$; $B$ là Noether và là một $A$-môđun tự do, do đó phẳng. Ngoài ra, nếu $p$ là một iđêan nguyên tố của $A$, $B/pB$ là đẳng cấu với $(A/p)[X_1, \ldots, X_n]$, là một miền nguyên, và do đó $pB$ là nguyên tố; các giả thiết của Mệnh đề 11 vì vậy được thỏa mãn đối với mọi $A$-môđun $E$ và mọi môđun con $E'$ của $E$.
(4) Cho $A$ là một đại số sinh hữu hạn trên một trường $k$, $K$ là một mở rộng của $k$ và $B = A \otimes_k K$ là đại số trên $K$ thu được bằng mở rộng vô hướng; $A$ và $B$ là Noether và $B$ là một $A$-môđun tự do, do đó Định lý 2 có thể được áp dụng cho $F = B$. Trong một số trường hợp (chẳng hạn nếu $k$ đóng đại số) có thể chứng minh rằng đối với mọi iđêan nguyên tố $p$ của $A$, $pB$ là nguyên tố hoặc bằng $B$; ta sẽ trở lại sau với ví dụ này.

### Bài tập {#ac-iv-s2-exercises}

Xem các [bài tập cho § 2](exercises/s2/).
