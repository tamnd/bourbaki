---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 3
section_title: Subalgebras of split semi-simple Lie algebras
lang: vi
source: lie-vii-ix
book_pages: 86-95, 229-231
pdf_pages: 0094-0103, 0237-0239
extraction: native
subsections:
    - "no": 1
      title: SUBALGEBRAS STABLE UNDER ad $\mathfrak{h}$
      page: 86
      pdf_page: 94
    - "no": 2
      title: IDEALS
      page: 89
      pdf_page: 97
    - "no": 3
      title: BOREL SUBALGEBRAS
      page: 90
      pdf_page: 98
    - "no": 4
      title: PARABOLIC SUBALGEBRAS
      page: 92
      pdf_page: 100
    - "no": 5
      title: NON-SPLIT CASE
      page: 94
      pdf_page: 102
statements: 28
exercises: 14
content_sha256: 2ab4c019d5d44c56ad93695d6a9d45cb7fadb7825ff736f21813401ba8c40105
translated_from: content/en/lie/VIII/03_s3_subalgebras_of_split_semi_simple_lie.md
source_content_sha256: 043e172960e451fa011db5fc5b2cdd69d22334e7720054bdacde767c930f9a50
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-vi-51cb66b4
glossary_version: 34
glossary_terms_sha256: 954fe0b8ef0754dde4691613de5a0cc9c36a2d1bfad88a48862859105a239611
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. CÁC ĐẠI SỐ CON CỦA CÁC ĐẠI SỐ LIE NỬA ĐƠN TÁCH

Trong đoạn này, ta ký hiệu bởi $(\mathfrak{g},\mathfrak{h})$ một đại số Lie nửa đơn tách, và bởi R hệ nghiệm của nó.

### 1. CÁC ĐẠI SỐ CON ỔN ĐỊNH DƯỚI ad $\mathfrak{h}$

#### Bổ đề 1 {#lie-viii-s3-lem-1 .statement tag=00ZO}

Cho V là một không gian con vectơ của $\mathfrak{g}$ và R(V) là tập hợp các $\alpha \in R$ sao cho $\mathfrak{g}^{\alpha}\subset V$. Khi đó, $(V\cap \mathfrak{h}) +\sum_{\alpha\in R(V)}\mathfrak{g}^{\alpha}$ là không gian con vectơ lớn nhất của V ổn định dưới ad $\mathfrak{h}$.

Một không gian con vectơ W của V ổn định dưới ad $\mathfrak{h}$ khi và chỉ khi

$$
W = (W\cap \mathfrak{h}) +\sum_{\alpha\in R}(W\cap \mathfrak{g}^{\alpha})
$$

(Đại số, Chương VII, §2, no. 2, Hệ quả 1 của Định lý 1). Không gian con vectơ lớn nhất của V ổn định dưới ad $\mathfrak{h}$ do đó là $(V\cap \mathfrak{h}) +\sum_{\alpha\in R}(V\cap \mathfrak{g}^{\alpha})$. Nhưng $V\cap \mathfrak{g}^{\alpha}=\mathfrak{g}^{\alpha}$ với $\alpha \in R(V)$, và $V\cap \mathfrak{g}^{\alpha}= 0$ với $\alpha  \notin R(V)$ vì dim $\mathfrak{g}^{\alpha}= 1$. Điều phải chứng minh.

Với mọi tập con P của R, đặt

$$
\mathfrak{g}^P=\sum_{\alpha\in P}\mathfrak{g}^{\alpha}\mathfrak{h}_P=\sum_{\alpha\in P}\mathfrak{h}_{\alpha}
$$

Nếu $P\subset R$ và $Q\subset R$, ta rõ ràng có

$$
[\mathfrak{h},\mathfrak{g}^P]\subset \mathfrak{g}^P \tag{1}
$$

$$
[\mathfrak{g}^P,\mathfrak{g}^Q] =\mathfrak{g}^{(P+Q)\cap R}+\mathfrak{h}_{P\cap(-Q)} \tag{2}
$$

Nhắc lại (Chương VI, §1, no. 7, Định nghĩa 4) rằng một tập con P của R được gọi là đóng nếu các điều kiện $\alpha \in P, \beta \in P, \alpha +\beta \in R$ kéo theo $\alpha +\beta \in P$, nói cách khác nếu $(P + P)\cap R\subset P$.

#### Bổ đề 2 {#lie-viii-s3-lem-2 .statement tag=00ZP}

Cho $\mathfrak{h}'$ là một không gian con vectơ của $\mathfrak{h}$ và P là một tập con của R. Khi đó $\mathfrak{h}'+\mathfrak{g}^P$ là một đại số con của $\mathfrak{g}$ khi và chỉ khi P là một tập con đóng của R và

$$
\mathfrak{h}'\supset \mathfrak{h}_{P\cap(-P)}
$$

Thật vậy,

$$
[\mathfrak{h}'+\mathfrak{g}^P,\mathfrak{h}'+\mathfrak{g}^P] = [\mathfrak{h}',\mathfrak{g}^P] + [\mathfrak{g}^P,\mathfrak{g}^P] =\mathfrak{h}_{P\cap(-P)}+ [\mathfrak{h}',\mathfrak{g}^P] +\mathfrak{g}^{(P+P)\cap R}
$$

Vậy $\mathfrak{h}'+\mathfrak{g}^P$ là một đại số con của $\mathfrak{g}$ khi và chỉ khi

$\mathfrak{h}_{P\cap(-P)}\subset \mathfrak{h}'$ and $\mathfrak{g}^{(P+P)\cap R}\subset \mathfrak{g}^P$

điều này chứng minh bổ đề.

#### Mệnh đề 1 {#lie-viii-s3-prop-1 .statement tag=00ZQ}

(i) Các đại số con của $\mathfrak{g}$ ổn định dưới ad$\mathfrak{h}$ là các không gian vectơ có dạng $\mathfrak{h}'+\mathfrak{g}^P$, trong đó P là một tập con đóng của R và $\mathfrak{h}'$ là một không gian vectơ của $\mathfrak{h}$ chứa $\mathfrak{h}_{P\cap(-P)}$.

(ii) Cho $\mathfrak{h}',\mathfrak{h}''$ là các không gian vectơ của $\mathfrak{h}$ và $P,Q$ là các tập con đóng của R, với $\mathfrak{h}'\supset \mathfrak{h}_{P\cap(-P)},\mathfrak{h}''\subset \mathfrak{h}'$ và $Q\subset P$. Khi đó $\mathfrak{h}''+\mathfrak{g}^Q$ là một iđêan của $\mathfrak{h}'+\mathfrak{g}^P$ khi và chỉ khi

$(P + Q)\cap R\subset Q$ và $\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{h}''\subset \bigcap_{\alpha\in P,\alpha  \notin Q}$ Ker $\alpha$.

Mệnh đề (i) suy ra ngay lập tức từ Bổ đề 1 và 2. Cho $\mathfrak{h}',\mathfrak{h}'',P,Q$ như trong (ii). Khi đó

$$
[\mathfrak{h}'+\mathfrak{g}^P,\mathfrak{h}''+\mathfrak{g}^Q] =\mathfrak{h}_{P\cap(-Q)}+ [\mathfrak{h}',\mathfrak{g}^Q] + [\mathfrak{h}'',\mathfrak{g}^P] +\mathfrak{g}^{(P+Q)\cap R}
$$

Do đó, $\mathfrak{h}''+\mathfrak{g}^Q$ là một iđêan của $\mathfrak{h}'+\mathfrak{g}^P$ khi và chỉ khi

$$
\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{h}'',[\mathfrak{h}'',\mathfrak{g}^P]\subset \mathfrak{g}^Q,\mathfrak{g}^{(P+Q)\cap R}\subset \mathfrak{g}^Q
$$

Điều này kéo theo (ii).

#### Mệnh đề 2 {#lie-viii-s3-prop-2 .statement tag=00ZR}

Cho $\mathfrak{a}$ là một đại số con của $\mathfrak{g}$ ổn định dưới ad$\mathfrak{h}$, và cho $\mathfrak{h}'\subset \mathfrak{h}$, $P\subset R$ sao cho $\mathfrak{a}=\mathfrak{h}'+\mathfrak{g}^P$.

(i) Gọi $\mathfrak{k}$ là tập hợp các $x\in \mathfrak{h}'$ sao cho $\alpha (x) = 0$ với mọi $\alpha \in P\cap (-P)$. Căn của $\mathfrak{a}$ là $\mathfrak{k}+\mathfrak{g}^Q$, trong đó Q là tập hợp các $\alpha \in P$ sao cho $-\alpha  \notin P$. Hơn nữa, $\mathfrak{g}^Q$ là một iđêan lũy linh của $\mathfrak{a}$.

(ii) $\mathfrak{a}$ là nửa đơn khi và chỉ khi $P =-P$ và $\mathfrak{h}'=\mathfrak{h}_P$.

(iii) $\mathfrak{a}$ là giải được nếu và chỉ nếu $P\cap (-P) =\emptyset$. Khi đó $[\mathfrak{a},\mathfrak{a}] =\mathfrak{g}^S$, trong đó

$$
S = ((P + P)\cap R)\cup  \{\alpha \in P|\alpha (\mathfrak{h}')\not= 0\}
$$

(iv) $\mathfrak{a}$ khả quy trong $\mathfrak{g}$ nếu và chỉ nếu $P =-P$.

(v) $\mathfrak{a}$ gồm các phần tử lũy linh nếu và chỉ nếu $\mathfrak{h}'= 0$. Khi đó $P\cap (-P) =$ $\emptyset$, và $\mathfrak{a}$ là lũy linh.

Ta chứng minh (v). Nếu $\mathfrak{a}$ gồm các phần tử lũy linh thì $\mathfrak{a}$ rõ ràng là lũy linh, và $\mathfrak{h}'= 0$ vì các phần tử của $\mathfrak{h}$ là nửa đơn. Giả sử $\mathfrak{h}'= 0$. Theo Mệnh đề 1 (i), $P\cap (-P) =\emptyset$. Theo Chương VI, §1, no. 7, Mệnh đề 22, tồn tại một buồng C của R sao cho $P\subset R_+(C)$. Do đó tồn tại một số nguyên $n >0$ có tính chất sau: nếu $\alpha_1, . . . , \alpha_n\in P$ và $\beta \in R\cup  \{0\}$, thì

$$
\alpha_1+\cdots +\alpha_n+\beta  \notin R\cup  \{0\}
$$

Điều này kéo theo mọi phần tử của $\mathfrak{g}^P$ đều lũy linh, do đó có (v).

Ta chứng minh (iii). Nếu $P\cap (-P) =\emptyset ,\mathfrak{g}^P$ là một đại số con của $\mathfrak{g}$ (Mệnh đề 1 (i)), và là lũy linh theo (v). Bây giờ

$$
[\mathfrak{a},\mathfrak{a}] = [\mathfrak{h}',\mathfrak{g}^P] + [\mathfrak{g}^P,\mathfrak{g}^P] = [\mathfrak{h}',\mathfrak{g}^P] +\mathfrak{g}^{(P+P)\cap R}\subset \mathfrak{g}^P
$$

do đó $\mathfrak{a}$ là giải được và $[\mathfrak{a},\mathfrak{a}]$ được cho bởi công thức trong mệnh đề. Nếu $P\cap (-P)\not=\emptyset$, lấy $\alpha \in P$ sao cho $-\alpha \in P$. Khi đó $\mathfrak{h}_{\alpha}+\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$ là một đại số con đơn của $\mathfrak{a}$ nên $\mathfrak{a}$ không giải được.

Ta chứng minh (i). Vì P đóng, $(P + Q)\cap R\subset P$. Nếu $\alpha \in P, \beta \in Q$ và $\alpha +\beta \in R$, thì không thể có $\alpha +\beta \in  -P$, vì, do P đóng, điều này sẽ kéo theo $-\beta =-(\alpha +\beta ) +\alpha \in P$ trong khi $\beta \in Q$; do đó, $(P + Q)\cap R\subset Q$. Điều này chứng minh rằng $\mathfrak{g}^Q$ là một iđêan của $\mathfrak{a}$, lũy linh theo (v). Ta có $P\cap (-Q) =\emptyset$, và $P\cap (-P) = P\cap \complement Q$, nên $\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{k}\subset \bigcap_{\alpha\in P,\alpha  \notin Q}$ Ker$\alpha$. Theo Mệnh đề 1 (ii),

$\mathfrak{k}+\mathfrak{g}^Q$ là một iđêan của $\mathfrak{a}$. Vì $Q\cap (-Q) =\emptyset$, iđêan này giải được theo (iii). Do đó nó được chứa trong căn $\mathfrak{r}$ của $\mathfrak{a}$. Vì $\mathfrak{r}$ ổn định dưới mọi đạo hàm của $\mathfrak{a},\mathfrak{r}$ ổn định dưới ad $\mathfrak{h}$. Bởi vậy tồn tại một tập con S của P sao cho $\mathfrak{r}= (\mathfrak{r}\cap \mathfrak{h}) +\mathfrak{g}^S$. Giả sử $\alpha \in S$ và $-\alpha \in P$. Khi đó $\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]\subset \mathfrak{r}$, nên $\mathfrak{g}^{-\alpha}= [\mathfrak{h}_{\alpha},\mathfrak{g}^{-\alpha}]\subset \mathfrak{r}= 0$, do đó $-\alpha \in S$; theo (iii), điều này mâu thuẫn với việc $\mathfrak{r}$ là giải được. Do đó, $S\subset Q$. Cuối cùng, nếu $x\in \mathfrak{r}\cap \mathfrak{h}$ và nếu $\alpha \in P\cap (-P)$, thì $[x,\mathfrak{g}^{\alpha}]\subset \mathfrak{g}^{\alpha}\cap \mathfrak{r}= 0$, nên $\alpha (x) = 0$; điều này cho thấy $x\in \mathfrak{k}$. Vậy $\mathfrak{r}\subset \mathfrak{k}+\mathfrak{g}^Q$ và chứng minh của (i) là đầy đủ.

Ta chứng minh (iv). Theo (i), biểu diễn liên hợp của $\mathfrak{a}$ trên $\mathfrak{g}$ là nửa đơn khi và chỉ khi ad$_{\mathfrak{g}}x$ là nửa đơn với mọi $x\in \mathfrak{k}+\mathfrak{g}^Q$ (Chương I, §6, no. 5, Định lý 4); theo (v), điều này xảy ra khi và chỉ khi $Q =\emptyset$, nói cách khác $P =-P$.

Ta chứng minh (ii). Nếu $\mathfrak{a}$ là nửa đơn, thì $P =-P$ theo (i), nên $\mathfrak{h}_P\subset \mathfrak{h}'$; hơn nữa, $\mathfrak{a}= [\mathfrak{a},\mathfrak{a}]\subset \mathfrak{h}_P+\mathfrak{g}^P$ và do đó $\mathfrak{h}'=\mathfrak{h}_P$. Nếu $P =-P$ và $\mathfrak{h}'=\mathfrak{h}_P,\mathfrak{a}$ là khả quy theo (iv), và $\mathfrak{a}=\sum_{\alpha\in P}\mathfrak{s}_{\alpha}$, nên $\mathfrak{a}= [\mathfrak{a},\mathfrak{a}]$ và $\mathfrak{a}$ là nửa đơn.

#### Mệnh đề 3 {#lie-viii-s3-prop-3 .statement tag=00ZS}

Cho $\mathfrak{a}$ là một đại số con nửa đơn của $\mathfrak{g}$ ổn định dưới ad($\mathfrak{h}$) và gọi P là tập con của R sao cho $\mathfrak{a}=\mathfrak{h}_P+\mathfrak{g}^P$.

(i) $\mathfrak{h}_P$ là một đại số con Cartan tách của $\mathfrak{a}$.

(ii) Hệ nghiệm của $(\mathfrak{a},\mathfrak{h}_P)$ là tập hợp các hạn chế lên $\mathfrak{h}_P$ của các phần tử của P.

Vì $\mathfrak{h}_P$ ổn định dưới ad $\mathfrak{h}$, bộ chuẩn hóa của nó trong $\mathfrak{a}$ ổn định dưới ad $\mathfrak{h}$, và do đó có dạng $\mathfrak{h}_P+\mathfrak{g}^Q$ với $Q\subset P$ (Bổ đề 1). Nếu $\alpha \in Q$,

$$
\mathfrak{g}^{\alpha}= [\mathfrak{h}_{\alpha},\mathfrak{g}^{\alpha}]\subset [\mathfrak{h}_P,\mathfrak{g}^{\alpha}]\subset \mathfrak{h}_P
$$

điều đó là phi lý. Vậy $Q =\emptyset$ và $\mathfrak{h}_P$ là chuẩn hóa tử của chính nó trong $\mathfrak{a}$. Điều này chứng minh rằng $\mathfrak{h}_P$ là một đại số con Cartan của $\mathfrak{a}$. Nếu $x\in \mathfrak{h}_P$, ad$_{\mathfrak{g}}x$, và a fortiori ad$_{\mathfrak{a}}x$, tam giác hóa được. Vậy (i) được chứng minh, và (ii) là hiển nhiên.

Theo Mệnh đề 1 (i), các đại số con của $\mathfrak{g}$ chứa $\mathfrak{h}$ là các tập hợp $\mathfrak{h}+\mathfrak{g}^P$ trong đó P là một tập con đóng của R. Theo Chương VII, §3, Mệnh đề 3, mọi đại số con Cartan của $\mathfrak{h}+\mathfrak{g}^P$ đều là một đại số con Cartan của $\mathfrak{g}$.

#### Mệnh đề 4 {#lie-viii-s3-prop-4 .statement tag=00ZT}

Giả sử $\mathfrak{a}$ là một đại số con của $\mathfrak{g}$ chứa $\mathfrak{h},x$ là một phần tử của $\mathfrak{a},s$ và $n$ là các thành phần nửa đơn và lũy linh của nó. Khi đó $s\in \mathfrak{a}$ và $n\in \mathfrak{a}$.

Ta có (ad $x$)$\mathfrak{a}\subset \mathfrak{a}$, nên (ad $s$)$\mathfrak{a}\subset \mathfrak{a}$ và (ad $n$)$\mathfrak{a}\subset \mathfrak{a}$. Vì $\mathfrak{a}$ là bộ chuẩn hóa của chính nó trong $\mathfrak{g}$ (Chương VII, §2, no. 1, Hệ quả 4 của Mệnh đề $4$)$,s\in \mathfrak{a}$ và $n\in \mathfrak{a}$.

#### Mệnh đề 5 {#lie-viii-s3-prop-5 .statement tag=00ZU}

Cho P là một tập con đóng của R.

(i) $\mathfrak{h}+\mathfrak{g}^P$ giải được khi và chỉ khi $P\cap (-P) =\emptyset$. Trong trường hợp đó, $[\mathfrak{h}+\mathfrak{g}^P,\mathfrak{h}+\mathfrak{g}^P] =\mathfrak{g}^P$.

(ii) $\mathfrak{h}+\mathfrak{g}^P$ là khả quy khi và chỉ khi $P =-P$.

Mệnh đề (i) suy ra từ Mệnh đề 2 (iii). Nếu $P =-P,\mathfrak{h}+\mathfrak{g}^P$ là khả quy (Mệnh đề 2 (iv)). Giả sử $\mathfrak{a}=\mathfrak{h}+\mathfrak{g}^P$ là khả quy. Khi đó

$$
\mathfrak{g}^P= [\mathfrak{h},\mathfrak{g}^P]\subset [\mathfrak{a},\mathfrak{a}]\subset \mathfrak{h}+\mathfrak{g}^P
$$

nên $[\mathfrak{a},\mathfrak{a}]$ có dạng $\mathfrak{h}'+\mathfrak{g}^P$ với $\mathfrak{h}'\subset \mathfrak{h}$; vì $[\mathfrak{a},\mathfrak{a}]$ là nửa đơn, suy ra $P =-P$ (Mệnh đề 2 (ii)).

### 2. IĐÊAN

#### Mệnh đề 6 {#lie-viii-s3-prop-6 .statement tag=00ZV}

Cho $R_1, . . . ,R_p$ là các thành phần bất khả quy của R. Với $i= 1, . . . , p$, đặt $\mathfrak{g}_i=\mathfrak{h}_{R_i}+\mathfrak{g}^{R_i}$. Khi đó $\mathfrak{g}_1, . . . ,\mathfrak{g}_p$ là các thành phần đơn của $\mathfrak{g}$.

Các $\mathfrak{g}_i$ là các iđêan của $\mathfrak{g}$ (Mệnh đề 1 (ii)). Hiển nhiên $\mathfrak{g}$ là tổng trực tiếp của các $\mathfrak{g}_i$, do đó là tích của các $\mathfrak{g}_i$. Cho $\mathfrak{a}$ và $\mathfrak{b}$ là các iđêan bù nhau của $\mathfrak{g}$. Khi đó $\mathfrak{a}$ và $\mathfrak{b}$ là nửa đơn và ổn định dưới ad $\mathfrak{h}$, nên tồn tại các tập con $P,Q$ của R sao cho $\mathfrak{a}=\mathfrak{h}_P+\mathfrak{g}^P,\mathfrak{b}=\mathfrak{h}_Q+\mathfrak{g}^Q$. Khi đó $\mathfrak{h}_P,\mathfrak{h}_Q$ là các phần bù trực giao của nhau trong $\mathfrak{h}$ đối với dạng Killing, nên P và Q là các hợp của những thành phần bất khả quy của R. Điều này chứng minh rằng các $\mathfrak{g}_i$ là các iđêan cực tiểu của $\mathfrak{g}$.

#### Hệ quả 1 {#lie-viii-s3-prop-6-cor-1 .statement tag=01IZ}

$\mathfrak{g}$ là đơn khi và chỉ khi R là bất khả quy (nói cách khác, đồ thị Dynkin của nó là liên thông).

Điều này suy ra từ Mệnh đề 6.

Một đại số Lie $\mathfrak{a}$ được gọi là đơn tuyệt đối nếu, với mọi mở rộng $k'$ của $k$, đại số Lie trên $k'$ $\mathfrak{a}_{(k')}$ là đơn.

#### Hệ quả 2 {#lie-viii-s3-prop-6-cor-2 .statement tag=00ZW}

Một đại số Lie đơn phân rã được là đơn tuyệt đối.

Điều này suy ra từ Hệ quả 1.

Nếu $\mathfrak{g}$ thuộc kiểu $A_l(l\geq 1)$ hoặc $B_l(l\geq 1)$ hoặc $C_l(l\geq 1)$ hoặc $D_l(l\geq 3),\mathfrak{g}$ được gọi là một đại số Lie đơn phân rã được cổ điển. Nếu $\mathfrak{g}$ thuộc kiểu $E_6, E_7, E_8, F_4$, hoặc $G_2,\mathfrak{g}$ được gọi là một đại số Lie đơn phân rã được ngoại lệ.

### 3. CÁC ĐẠI SỐ CON BOREL

#### Mệnh đề 7 {#lie-viii-s3-prop-7 .statement tag=00ZX}

Cho $\mathfrak{b}=\mathfrak{h}+\mathfrak{g}^P$ là một đại số con của $\mathfrak{g}$ chứa $\mathfrak{h}$. Các điều kiện sau là tương đương:

(i) $\mathfrak{b}$ là một đại số con giải được cực đại của $\mathfrak{g}$;

(ii) tồn tại một buồng C của R sao cho $P = R_+(C)$;

(iii) $P\cap (-P) =\emptyset$ và $P\cup (-P) = R$.

(i) $=\Rightarrow$ (ii): Nếu $\mathfrak{b}$ giải được, thì $P\cap (-P) =\emptyset$. Khi đó tồn tại một buồng C của R sao cho $P\subset R_+(C)$ (Chương VI, §1, no. 7, Mệnh đề 22). Khi đó $\mathfrak{h}+\mathfrak{g}^{R_+(C)}$ là một đại số con giải được của $\mathfrak{g}$ chứa $\mathfrak{b}$, do đó bằng $\mathfrak{b}$ nếu $\mathfrak{b}$ là cực đại.

(ii) $=\Rightarrow$ (iii): Điều này hiển nhiên.

(iii) $=\Rightarrow$ (i): Giả sử rằng $P\cap (-P) =\emptyset$ và $P\cup (-P) = R$. Khi đó $\mathfrak{b}$ là giải được. Gọi $\mathfrak{b}'$ là một đại số con giải được của $\mathfrak{g}$ chứa $\mathfrak{b}$. Tồn tại một tập con Q của R sao cho $\mathfrak{b}'=\mathfrak{h}+\mathfrak{g}^Q$. Khi đó $Q\cap (-Q) =\emptyset$ và $Q\supset P$, nên Q = P và $\mathfrak{b}'=\mathfrak{b}$.

#### Định nghĩa 1 {#lie-viii-s3-def-1 .statement tag=00ZY}

Một đại số con của $\mathfrak{g}$ chứa $\mathfrak{h}$ và thỏa mãn điều kiện tương đương trong Mệnh đề 7 được gọi là một đại số con Borel của $(\mathfrak{g},\mathfrak{h})$.

Một đại số con $\mathfrak{b}$ của một đại số tách được $\mathfrak{g}$ được gọi là một đại số con Borel của $\mathfrak{g}$ nếu tồn tại một đại số con Cartan tách $\mathfrak{h}'$ của $\mathfrak{g}$ sao cho $\mathfrak{b}$ là một đại số con Borel của $(\mathfrak{g},\mathfrak{h}')$.

Cho $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie reductive tách được. Giả sử $\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$ với $\mathfrak{c}$ giao hoán và $\mathfrak{s}$ nửa đơn. Một đại số con của $\mathfrak{g}$ có dạng $\mathfrak{c}\times \mathfrak{b}$, trong đó $\mathfrak{b}$ là một đại số con Borel của $(\mathfrak{s},\mathfrak{h}\cap \mathfrak{s})$, được gọi là một đại số con Borel của $(\mathfrak{g},\mathfrak{h})$.

Với các ký hiệu của Mệnh đề 7, ta cũng nói rằng $\mathfrak{b}$ là đại số con Borel của $\mathfrak{g}$ được xác định bởi $\mathfrak{h}$ và C (hoặc bởi $\mathfrak{h}$ và cơ sở của R liên kết với C).

#### Nhận xét {#lie-viii-s3-n3-rem-1 .statement tag=00ZZ}

Ánh xạ gán $R_+(C)$ cho một buồng C của R là đơn ánh (Chap. VI, §1, no. 7, Cor. 1 of Prop. 20). Do đó, $C \rightarrow \mathfrak{h}+\mathfrak{g}^{R_+(C)}$ là một song ánh từ tập hợp các buồng của R lên tập hợp các đại số con Borel của $(\mathfrak{g},\mathfrak{h})$. Vì thế, số các đại số con Borel của $(\mathfrak{g},\mathfrak{h})$ bằng cấp của nhóm Weyl của R (Chap. VI, §1, no. 5, Th. 2).

#### Mệnh đề 8 {#lie-viii-s3-prop-8 .statement tag=0100}

Cho $\mathfrak{b}$ là một đại số con của $\mathfrak{g},k'$ là một mở rộng của $k$. Khi đó $\mathfrak{b}\otimes_kk'$ là một đại số con Borel của $(\mathfrak{g}\otimes_kk',\mathfrak{h}\otimes_kk')$ nếu và chỉ nếu $\mathfrak{b}$ là một đại số con Borel của $(\mathfrak{g},\mathfrak{h})$.

Điều này hiển nhiên từ điều kiện (iii) của Mệnh đề 7.

#### Mệnh đề 9 {#lie-viii-s3-prop-9 .statement tag=0101}

Cho $\mathfrak{b}$ là đại số con Borel của $(\mathfrak{g},\mathfrak{h})$ được xác định bởi một chamber C của R. Cho $\mathfrak{n}=\mathfrak{g}^{R_+(C)}=\sum_{\alpha\in R,\alpha >0}\mathfrak{g}^{\alpha}$. Đặt $l=$ dim$\mathfrak{h}$.

(i) Nếu $h\in \mathfrak{h}$ và $x\in \mathfrak{n}$, đa thức đặc trưng của ad$_{\mathfrak{g}}(h+x)$ là $T^l\prod_{\alpha\in R}(T-\alpha (h))$.

(ii) iđêan lũy linh lớn nhất của $\mathfrak{b}$ bằng $\mathfrak{n}$ và bằng $[\mathfrak{b},\mathfrak{b}]$. Đây cũng là tập hợp các phần tử của $\mathfrak{b}$ lũy linh trong $\mathfrak{g}$.

(iii) Gọi B là cơ sở của R liên kết với C. Với mọi $\alpha \in B$, gọi $X_{\alpha}$ là một phần tử khác không của $\mathfrak{g}^{\alpha}$. Khi đó $(X_{\alpha})_{\alpha\in B}$ sinh ra đại số Lie $\mathfrak{n}$. Ta có $[\mathfrak{n},\mathfrak{n}] =\sum_{\alpha\in R,\alpha >0,\alpha  \notin B}\mathfrak{g}^{\alpha}$.

Tồn tại một thứ tự toàn phần trên $\mathfrak{h}^*_{\mathbf{Q}}$ tương thích với cấu trúc không gian vectơ của nó và sao cho các phần tử của $R_+(C)$ là $>0$ (Chap. VI, §1, no. 7). Gọi $h, x$ như trong (i) và $y\in \mathfrak{g}^{\alpha}$. Khi đó $[h+x, y] =\alpha (h)y+z$ với $z\in \sum_{\beta >\alpha}\mathfrak{g}^{\beta}$. Khi đó,

đối với một cơ sở thích hợp của $\mathfrak{g}$, ma trận của ad$_{\mathfrak{g}}(h+x)$ có các tính chất sau:

1) nó là tam giác dưới;

2) các phần tử trên đường chéo của ma trận là số $0 (l$ lần) và các $\alpha (h)$ với $\alpha \in R$.

Điều này chứng minh (i). Nó cũng cho thấy rằng đa thức đặc trưng của ad$_{\mathfrak{b}}(h+x)$ là $T\prod_{\alpha\in R_+(C)}^l(T-\alpha (h))$. Suy ra từ điều trên rằng tập hợp

các phần tử của $\mathfrak{b}$ lũy linh trong $\mathfrak{g}$, cũng như iđêan lũy linh lớn nhất của $\mathfrak{b}$, đều bằng $\mathfrak{n}$. Ta có $\mathfrak{n}= [\mathfrak{b},\mathfrak{b}]$ theo Mệnh đề 5 (i). Cuối cùng, mệnh đề (iii) suy ra từ §2, Mệnh đề 4 (ii) và Chương VI, §1, no. 6, Mệnh đề 19.

#### Hệ quả {#lie-viii-s3-n3-cor-1 .statement tag=0102}

Cho $\mathfrak{b}$ là một đại số con Borel của $\mathfrak{g}$.

(i) Mọi đại số con Cartan của $\mathfrak{b}$ đều là một đại số con Cartan tách của $\mathfrak{g}$.

(ii) Nếu $\mathfrak{h}_1,\mathfrak{h}_2$ là các đại số con Cartan của $\mathfrak{b}$, thì tồn tại $x\in [\mathfrak{b},\mathfrak{b}]$ sao cho $e^{ad_{\mathfrak{g}}x}\mathfrak{h}_1=\mathfrak{h}_2$.

Mệnh đề (i) suy ra từ Mệnh đề 9 (i) và Chương VII, §3, no. 3, Mệnh đề 3. Mệnh đề (ii) suy ra từ Mệnh đề 9 (ii) và Chương VII, §3, no. 4, Định lý 3.

#### Mệnh đề 10 {#lie-viii-s3-prop-10 .statement tag=0103}

Cho $\mathfrak{b},\mathfrak{b}'$ là các đại số con Borel của $\mathfrak{g}$. Tồn tại một đại số con Cartan tách của $\mathfrak{g}$ được chứa trong $\mathfrak{b}\cap \mathfrak{b}'$.

Cho $\mathfrak{h}$ là một đại số con Cartan của $\mathfrak{b},\mathfrak{n}= [\mathfrak{b},\mathfrak{b}],\mathfrak{n}'= [\mathfrak{b}',\mathfrak{b}'],\mathfrak{p}=\mathfrak{b}\cap \mathfrak{b}'$, và $\mathfrak{s}$ là một không gian con vectơ của $\mathfrak{g}$ bù với $\mathfrak{b}+\mathfrak{b}'$. Ký hiệu bởi $\mathfrak{s}^{\bot},\mathfrak{b}^{\bot},\mathfrak{b}^{'\bot}$ các phần bù trực giao của $\mathfrak{s},\mathfrak{b},\mathfrak{b}'$ đối với dạng Killing của $\mathfrak{g}$. Đặt $l=$ dim$\mathfrak{h}, n=$ dim$\mathfrak{n}, p=$ dim$\mathfrak{p}$. Khi đó dim$\mathfrak{b}=$ dim$\mathfrak{b}'=l+n$,

dim$\mathfrak{s}^{\bot}=$ dim($\mathfrak{b}+\mathfrak{b}'$) $= 2(l+n)-p$,

và do đó

dim($\mathfrak{s}^{\bot}\cap \mathfrak{p}$)$\geq$ dim$\mathfrak{s}^{\bot}+$ dim$\mathfrak{p}-$ dim$\mathfrak{g}$ (3)

$$
= 2(l+n)-p+p-(l+ 2n) =l
$$

Theo Mệnh đề 1 của §2, no. $2,\mathfrak{n}\subset \mathfrak{b}^{\bot},\mathfrak{n}'\subset \mathfrak{b}^{'\bot}$. Các phần tử của $\mathfrak{p}\cap \mathfrak{n}$ là lũy linh trong $\mathfrak{g}$ (Mệnh đề 9 (ii)), và thuộc $\mathfrak{b}'$, do đó thuộc $\mathfrak{n}'$ (Mệnh đề 9 (ii)). Do đó, $\mathfrak{p}\cap \mathfrak{n}\subset \mathfrak{n}\cap \mathfrak{n}'\subset \mathfrak{b}^{\bot}\cap \mathfrak{b}^{'\bot}$, nên $\mathfrak{s}^{\bot}\cap \mathfrak{p}\cap \mathfrak{n}= 0$. Theo (3), ta thấy rằng $\mathfrak{s}^{\bot}\cap \mathfrak{p}$ là một phần bù của $\mathfrak{n}$ trong $\mathfrak{b}$. Gọi $z$ là một phần tử của $\mathfrak{h}$ chính quy trong $\mathfrak{g}$; tồn tại $y\in \mathfrak{n}$ sao cho $y+z\in \mathfrak{s}^{\bot}\cap \mathfrak{p}$; theo Mệnh đề 9 (i), ad$_{\mathfrak{g}}(y+z)$ có cùng đa thức đặc trưng như ad$_{\mathfrak{g}}z$, nên $x=y+z$ là chính quy trong $\mathfrak{g}$ và a fortiori trong $\mathfrak{b}$ và $\mathfrak{b}'$ (Chương VII, §2, no. 2, Mệnh đề 9). Vì $\mathfrak{g},\mathfrak{b},\mathfrak{b}'$ có cùng hạng, $\mathfrak{b}^0(x) =\mathfrak{g}^0(x) ={\mathfrak{b}'}^0(x)$ đồng thời là một đại số con Cartan của $\mathfrak{b}$, của $\mathfrak{g}$ và của $\mathfrak{b}'$ (Chương VII, §3, no. 3, Định lý 2). Cuối cùng, đại số con Cartan này của $\mathfrak{g}$ là tách theo Hệ quả của Mệnh đề 9.

#### Hệ quả {#lie-viii-s3-n3-cor-2 .statement tag=0104}

Nhóm Aut$_e(\mathfrak{g})$ tác động bắc cầu trên tập hợp các cặp $(\mathfrak{t},\mathfrak{b})$ trong đó $\mathfrak{t}$ là một đại số con Cartan tách của $\mathfrak{g}$ và $\mathfrak{b}$ là một đại số con Borel của $(\mathfrak{g},\mathfrak{t})$.

Cho $(\mathfrak{t}_1,\mathfrak{b}_1)$ và $(\mathfrak{t}_2,\mathfrak{b}_2)$ là hai cặp như thế. Tồn tại một đại số con Cartan tách $\mathfrak{t}$ của $\mathfrak{g}$ được chứa trong $\mathfrak{b}_1\cap \mathfrak{b}_2$ (Mệnh đề 10). Theo Hệ quả của Mệnh đề 9, ta được quy về trường hợp $\mathfrak{t}_1=\mathfrak{t}_2=\mathfrak{t}$. Gọi S là hệ nghiệm của $(\mathfrak{g},\mathfrak{t})$. Tồn tại các cơ sở $B_1,B_2$ của S sao cho $\mathfrak{b}_i$ liên kết với $B_i(i= 1,2)$, và tồn tại $s\in W(S)$ biến đổi $B_1$ thành $B_2$. Cuối cùng, tồn tại $a\in$ Aut$_e(\mathfrak{g})$ sao cho $a|\mathfrak{t}=s($§2, no. 2, Hệ quả của Định lý 2). Khi đó $a(\mathfrak{t}) =\mathfrak{t}$ và $a(\mathfrak{b}_1) =\mathfrak{b}_2$.

### 4. CÁC ĐẠI SỐ CON PARABOLIC

#### Mệnh đề 11 {#lie-viii-s3-prop-11 .statement tag=0105}

Cho $\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P$ là một đại số con của $\mathfrak{g}$ chứa $\mathfrak{h}$. Các điều kiện sau là tương đương:

(i) $\mathfrak{p}$ chứa một đại số con Borel của $(\mathfrak{g},\mathfrak{h})$;

(ii) tồn tại một buồng C của R sao cho $P\supset R_+(C)$;

(iii) P là parabolic, nói cách khác (Chương VI, §1, no. 7, Định nghĩa 4), $P\cup (-P) =$ R.

Các điều kiện (i) và (ii) là tương đương theo Mệnh đề 7. Các điều kiện (ii) và (iii) là tương đương theo Chương VI, §1, no. 7, Mệnh đề 20.

#### Định nghĩa 2 {#lie-viii-s3-def-2 .statement tag=0106}

Một đại số con của $\mathfrak{g}$ chứa $\mathfrak{h}$ và thỏa mãn các điều kiện tương đương của Mệnh đề 11 được gọi là một đại số con parabolic của $(\mathfrak{g},\mathfrak{h})$. Một đại số con parabolic của $\mathfrak{g}$ là một đại số con parabolic của $(\mathfrak{g},\mathfrak{h}')$ trong đó $\mathfrak{h}'$ là một đại số con Cartan tách của $\mathfrak{g}$.

Định nghĩa này mở rộng ngay lập tức cho trường hợp trong đó $(\mathfrak{g},\mathfrak{h})$ là một đại số Lie reductive tách được.

#### Nhận xét {#lie-viii-s3-n4-rem-1 .statement tag=0107}

Cho B là một cơ sở của R, và $\mathfrak{b}$ là đại số con Borel tương ứng. Nếu $\Sigma \subset B$, ký hiệu $Q_{\Sigma}$ là tập hợp các nghiệm là tổ hợp tuyến tính của các phần tử của $\Sigma$ với các hệ số $\leq 0$; đặt $\mathfrak{p}(\Sigma ) = R_+(B)\cup Q_{\Sigma}$ và $\mathfrak{p}_{\Sigma}=\mathfrak{h}\oplus \mathfrak{g}^{P(\Sigma)}$. Theo Chương VI, §1, no. 7, Bổ đề 3 và Mệnh đề $20,\mathfrak{p}_{\Sigma}$ là một đại số con parabolic chứa $\mathfrak{b}$ và mọi đại số con parabolic của $\mathfrak{g}$ chứa $\mathfrak{b}$ đều thu được theo cách này.

#### Bổ đề 3 {#lie-viii-s3-lem-3 .statement tag=0108}

Cho V là một không gian vectơ thực hữu hạn chiều, S là một hệ nghiệm trong $V^*,\mathscr{P}$ là tập hợp các tập con parabolic của S; gọi $\mathscr{H}$ là tập hợp các Ker $\alpha$ với $\alpha \in S$, và $\mathscr{F}$ là tập hợp các mặt của V đối với $\mathscr{H}$ (Chương V, §1, no. 2, Định nghĩa 1).

Nếu $P\in \mathscr{P}$, gọi F(P) là tập hợp các $v\in V$ sao cho $\alpha (v)\geq 0$ với mọi $\alpha \in P$. Nếu $F\in \mathscr{F}$, gọi P(F) là tập hợp các $\alpha \in R$ sao cho $\alpha (v)\geq 0$ với mọi $v\in F$.

Khi đó $F \rightarrow P(F)$ là một song ánh từ $\mathscr{F}$ tới $\mathscr{P}$; với mọi $F\in \mathscr{F}$, F(P(F)) là bao đóng của F.

a) Cho $P\in \mathscr{P}$. Tồn tại một buồng C của S và một tập con $\Sigma$ của cơ sở B(C) sao cho $P = S_+(C)\cup Q$ trong đó Q là tập các tổ hợp tuyến tính của các phần tử của $\Sigma$ với các hệ số là số nguyên không dương (Chương VI, §1, no. 7, Mệnh đề 20). Đặt

$$
B(C) =\{\alpha_1, . . . , \alpha_l\}, \Sigma =\{\alpha_1, . . . , \alpha_m\}
$$

Nếu $v\in V$, ta có các tương đương sau:

$\alpha (v)\geq 0$ với mọi $\alpha \in P$

$$
\Leftarrow \Rightarrow \alpha_1(v)\geq 0, . . . \alpha_l(v)\geq 0, \alpha_1(v)\leq 0, . . . , \alpha_m(v)\leq 0
$$

$$
\Leftarrow \Rightarrow \alpha_1(v) =\cdots =\alpha_m(v) = 0, \alpha_{m+1}(v)\geq 0, . . . , \alpha_l(v)\geq 0
$$

vậy F(P) là bao đóng của tập

$$
\{v\in V|\alpha_1(v) =\cdots =\alpha_m(v) = 0, \alpha_{m+1}(v)>0, . . . , \alpha_l(v)>0\}
$$

một tập hợp là một diện F đối với $\mathscr{H}$ vì mọi phần tử của S là một tổ hợp tuyến tính của $\alpha_1, . . . , \alpha_l$ trong đó các hệ số hoặc đều $\geq 0$ hoặc đều $\leq 0$. Hơn nữa, nếu $\beta =u_1\alpha_1+\cdots +u_l\alpha_l\in S$,

$$
\beta \in P(F)\Leftarrow \Rightarrow u_{m+1}\geq 0, . . . , u_l\geq 0
$$

$\Leftarrow \Rightarrow \beta \in S_+(C)$ hoặc $(-\beta \in S_+(C)$ và $u_{m+1}=. . .=u_l= 0)$

$$
\Leftarrow \Rightarrow \beta \in S_+(C)\cup Q = P
$$

do đó P(F) = P.

b) Cho $F\in \mathscr{F}$. Rõ ràng là $P(F)\in \mathscr{P}$. Mặt khác, F được chứa trong bao đóng của một buồng đối với $\mathscr{H}$ (Chap. V, §1, no. 3, formulas (6)), và do đó là một mặt đối với tập hợp các tường của buồng này (Chap. V, §1, no. 4, Prop. 9). Do đó, $\overline{F}$ có dạng $\{v\in V|\alpha (v)\geq 0$ for all $\alpha \in T\}$, trong đó T là một tập con của S mà rõ ràng ta có thể lấy bằng P(F). Vậy, $\overline{F}= F(P(F))$. Q.E.D.

Nếu $P\in \mathscr{P}$, thì mặt F sao cho P = P(F) được gọi là liên kết với P; ta ký hiệu nó bởi F(P). Ta mở rộng các quy ước này cho trường hợp trong đó $(\mathfrak{g},\mathfrak{h})$ là khả quy tách.

#### Mệnh đề 12 {#lie-viii-s3-prop-12 .statement tag=0109}

Cho $\mathscr{H}$ là tập hợp các siêu phẳng của $\mathfrak{h}_{\mathbf{R}}$ gồm các hạt nhân của các căn trong R. Cho $\mathscr{F}$ là tập hợp các mặt của $\mathfrak{h}_{\mathbf{R}}$ đối với $\mathscr{H}$. Cho $\mathscr{S}$ là tập hợp các đại số con parabolic của $(\mathfrak{g},\mathfrak{h})$. Với mỗi $\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P\in \mathscr{S}$, gọi $F(\mathfrak{p})$ là mặt liên kết với P. Khi đó $\mathfrak{p} \rightarrow F(\mathfrak{p})$ là một song ánh từ $\mathscr{S}$ lên $\mathscr{F}$. Nếu $\mathfrak{p}_1,\mathfrak{p}_2\in \mathscr{P}$,

$$
\mathfrak{p}_1\supset \mathfrak{p}_2\Leftarrow \Rightarrow F(\mathfrak{p}_1)\subset \overline{F(\mathfrak{p}_2)}
$$

Điều này suy ra ngay lập tức từ Bổ đề 3.

#### Ví dụ {#lie-viii-s3-n4-exa-1 .statement tag=010A}

Các mặt tương ứng với các đại số con parabolic của $(\mathfrak{g},\mathfrak{h})$ chứa một đại số Borel $\mathfrak{b}$ là các mặt được chứa trong bao đóng của buồng liên kết với $\mathfrak{b}$ (xem Nhận xét trên).

#### Mệnh đề 13 {#lie-viii-s3-prop-13 .statement tag=010B}

Cho $\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P$ là một đại số con parabolic của $(\mathfrak{g},\mathfrak{h})$, Q là tập hợp các $\alpha \in P$ sao cho $-\alpha  \notin P$, và $\mathfrak{s}=\mathfrak{h}+\mathfrak{g}^{P\cap(-P)}$. Khi đó $\mathfrak{p}=\mathfrak{s}\oplus \mathfrak{g}^Q,\mathfrak{s}$ là khả quy trong $\mathfrak{g}$, và $\mathfrak{g}^Q$ là iđêan lũy linh lớn nhất của $\mathfrak{p}$ và là căn lũy linh của $\mathfrak{p}$. Tâm của $\mathfrak{p}$ bằng không.

Theo Mệnh đề $2,\mathfrak{s}$ là khả quy trong $\mathfrak{g}$ và $\mathfrak{g}^Q$ là một iđêan lũy linh của $\mathfrak{p}$. Nếu $\mathfrak{n}$ là iđêan lũy linh lớn nhất của $\mathfrak{p},\mathfrak{g}^Q\subset \mathfrak{n}\subset \mathfrak{h}+\mathfrak{g}^Q$ (Mệnh đề 2 (i)); nếu $x\in \mathfrak{n}\cap \mathfrak{h}$, ad$_{\mathfrak{p}}x$ là lũy linh, nên $\alpha (x) = 0$ đối với mọi $\alpha \in P$, và do đó $x= 0$; điều này chứng tỏ rằng $\mathfrak{n}=\mathfrak{g}^Q$. Vì $[\mathfrak{h},\mathfrak{g}^Q] =\mathfrak{g}^Q$, căn lũy linh của $\mathfrak{p}$ chứa $\mathfrak{g}^Q$ và do đó bằng $\mathfrak{g}^Q$. Cho $z=h+\sum_{\alpha\in P}u_{\alpha}$ (trong đó $h\in \mathfrak{h}, u_{\alpha}\in \mathfrak{g}^{\alpha}$) là một

phần tử của tâm của $\mathfrak{p}$. Với mọi $h'\in \mathfrak{h}, 0 = [h', z] =\sum\alpha (h')u_{\alpha}$, nên $u_{\alpha}= 0$ với mọi $\alpha \in P$; suy ra $[h,\mathfrak{g}^{\beta}] = 0$ với mọi $\beta \in P$, do đó $h= 0$.

### 5. TRƯỜNG HỢP KHÔNG TÁCH ĐƯỢC

#### Mệnh đề 14 {#lie-viii-s3-prop-14 .statement tag=010C}

Cho $k'$ là một mở rộng của $k$ và $\mathfrak{g}'=\mathfrak{g}\otimes_kk'$. Cho $\mathfrak{m}$ là một đại số con của $\mathfrak{g}$ và $\mathfrak{m}'=\mathfrak{m}\otimes_kk'$. Nếu $\mathfrak{m}'$ là một đại số con parabolic (tương ứng, Borel ) của $\mathfrak{g}',\mathfrak{m}$ thì là một đại số con parabolic (tương ứng, Borel ) của $\mathfrak{g}$.

Theo Mệnh đề 8 và 11, chỉ cần chứng minh rằng $\mathfrak{m}$ chứa một đại số con Cartan tách của $\mathfrak{g}$. Gọi $\mathfrak{b}$ là một đại số con Borel của $\mathfrak{g}$. Khi đó $\mathfrak{b}'=\mathfrak{b}\otimes_kk'$ là một đại số con Borel của $\mathfrak{g}'$, nên $\mathfrak{m}'\cap \mathfrak{b}'$ chứa một đại số con Cartan của $\mathfrak{g}'$ (Mệnh đề 10). Gọi $\mathfrak{t}$ là một đại số con Cartan của $\mathfrak{m}\cap \mathfrak{b}$. Khi đó $\mathfrak{t}\otimes_kk'$ là một đại số con Cartan của $\mathfrak{m}'\cap \mathfrak{b}'$, và do đó của $\mathfrak{g}'$ (Chap. VII, §3, no. 3, Mệnh đề 3). Do đó, $\mathfrak{t}$ là một đại số con Cartan của $\mathfrak{g}$, và nó là tách vì nó được chứa trong $\mathfrak{b}$.

#### Định nghĩa 3 {#lie-viii-s3-def-3 .statement tag=010D}

Cho $\mathfrak{a}$ là một đại số Lie nửa đơn (hoặc nói chung hơn là khả quy) và $\overline{k}$ là một bao đóng đại số của $k$. Một đại số con $\mathfrak{m}$ của $\mathfrak{a}$ được gọi là parabolic (tương ứng, Borel ) nếu $\mathfrak{m}\otimes_k\overline{k}$ là một đại số con parabolic (tương ứng, Borel ) của $\mathfrak{a}\otimes_k\overline{k}$.

Nếu $\mathfrak{a}$ phân rã được, Mệnh đề 14 cho thấy rằng định nghĩa này tương đương với Định nghĩa 2 (tương ứng, với Định nghĩa 1).

#### Mệnh đề 15 {#lie-viii-s3-prop-15 .statement tag=010E}

Cho $\mathfrak{a}$ là một đại số Lie khả quy, $k'$ là một mở rộng của $k$, và $\mathfrak{m}$ là một đại số con của $\mathfrak{a}$. Khi đó $\mathfrak{m}$ là một đại số con parabolic (tương ứng là Borel ) của $\mathfrak{a}$ nếu và chỉ nếu $\mathfrak{m}\otimes_kk'$ là một đại số con parabolic (tương ứng là Borel ) của $\mathfrak{a}\otimes_kk'$.

Điều này suy ra ngay lập tức từ Mệnh đề 14.

### Bài tập {#lie-viii-s3-exercises}

Xem [các bài tập của § 3](exercises/s3/).
