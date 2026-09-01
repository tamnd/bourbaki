---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 8
section_title: Dimension homologique
lang: vi
source: alg-x-fr
book_pages: A X.134-A X.146, A X.202-A X.206
pdf_pages: 0140-0152, 0208-0212
extraction: ocr
subsections:
    - "no": 1
      title: Dimension projective d’un module
      page: 134
      pdf_page: 140
    - "no": 2
      title: L’homomorphisme $\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_A(\operatorname{Ext}_A^n(M, A), P)$
      page: 137
      pdf_page: 143
    - "no": 3
      title: Dimension homologique d’un anneau
      page: 138
      pdf_page: 144
    - "no": 4
      title: Anneaux de dimension homologique 0
      page: 140
      pdf_page: 146
    - "no": 5
      title: Anneaux de dimension homologique 1
      page: 140
      pdf_page: 146
    - "no": 6
      title: Dimension homologique des anneaux de polynômes
      page: 141
      pdf_page: 147
    - "no": 7
      title: Dimension homologique des modules gradués
      page: 143
      pdf_page: 149
statements: 34
exercises: 22
content_sha256: 4977c130c5bd65227e2dd42c798474cf244c220e678280d000986f10a7d7946b
translated_from: content/en-mt/alg/X/08_s8_dimension_homologique.md
source_lang: en-mt
translation_method: machine
source_content_sha256: a43e5824a369fc7cb54f0cf634d6c6c6ca549a1893ead639ca49ac83f5b3a298
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5-mini
translation_run: translate-vi-5f5f0ebc
glossary_version: 34
glossary_terms_sha256: 4cb5582fcbc630f4095c6116e302525a6775ff128530a14e988fe568bad32b35
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. CHIỀU ĐỒNG LUÂN

Trong tiết này, ta áp dụng các quy ước của § 5.

### 1. Chiều xạ ảnh của một môđun

#### Định nghĩa 1 {#alg-x-s8-def-1 .statement}

*Cho $M$ là một $A$-môđun. Chiều xạ ảnh của $M$, ký hiệu bởi $\mathrm{dp}_A(M)$, là cận dưới lớn nhất trong $\overline{\mathbf{Z}}$ của các độ dài của các giải xạ ảnh của $M$* (X, p. 48).

Do đó ta có $\mathrm{dp}_A(0) = -\infty$, $\mathrm{dp}_A(M) \geq 0$ nếu $M \neq 0$. Để $M$ là xạ ảnh, điều kiện cần và đủ là $\mathrm{dp}_A(M) \leq 0$.

#### Bổ đề 1 {#alg-x-s8-lem-1 .statement}

*Nếu $\mathrm{dp}_A(M) < n < +\infty$, thì $\mathrm{Ext}_A^n(M, N) = 0$ với mọi $A$-môđun $N$ và $\mathrm{Tor}_n^A(P, M) = 0$ với mọi $A$-môđun phải $P$.
Điều này suy ra ngay lập tức từ sự kiện rằng $M$ có một giải xạ ảnh có độ dài $< n$ và từ X, p. 100, Định lý 1.*

#### Mệnh đề 1 {#alg-x-s8-prop-1 .statement}

*Cho $M$ là một $A$-môđun và $n$ là một số nguyên $\geq 0$. Các điều kiện sau là tương đương* :
(i) $\mathrm{dp}_A(M) \leq n$ (*tức là* (định. 1), $M$ có một giải xạ ảnh có độ dài $\leq n$);
(ii) $\mathrm{Ext}_A^r(M, N) = 0$ với mọi $A$-môđun $N$ và mọi số nguyên $r > n$;
(iii) $\mathrm{Ext}_A^{n+1}(M, N) = 0$ với mọi $A$-môđun $N$;
(iv) *với mọi dãy khớp*
$$
0 \to K \to P_{n-1} \to \ldots \to P_0 \to M \to 0
$$
*trong đó các $P_i$ là xạ ảnh, $K$ là xạ ảnh*.

(i) ⇒ (ii): điều này suy ra từ Bổ đề 1.
(ii) ⇒ (iii): điều này là tầm thường.
(iii) ⇒ (iv): trong tình huống của (iv), với mọi $A$-môđun $N$ tồn tại một đẳng cấu từ $\mathrm{Ext}_A^1(K, N)$ lên $\mathrm{Ext}_A^{n+1}(M, N)$ (X, p. 128, Hệ quả 4); nếu (iii) đúng, thì
$$
\mathrm{Ext}_A^1(K, N) = 0
$$
với mọi $N$ và $K$ là xạ ảnh (X, p. 93, Mệnh đề 10).
(iv) ⇒ (i): xét dãy khớp (X, p. 50)
$$
0 \to Z_{n-1}(M) \to L_{n-1}(M) \to \ldots \to L_0(M) \to M \to 0 .
$$
Nếu (iv) đúng, thì $Z_{n-1}(M)$ là xạ ảnh và $M$ có một giải xạ ảnh có độ dài $\leq n$.

#### Hệ quả 1 {#alg-x-s8-prop-1-cor-1 .statement}

Cho $(M_i)_{i \in E}$ là một họ các $A$-môđun. Ta có
$$
\mathrm{dp}_A \left( \bigoplus_{i \in E} M_i \right) = \sup_{i \in E} \mathrm{dp}_A(M_i) .
$$
Điều này suy ra từ sự tương đương của các điều kiện (i) và (iii) của Mệnh đề 1 và Mệnh đề 7 của X, p. 89.

Trong mệnh đề sau, ta quy ước rằng $\pm \infty + 1 = \pm \infty - 1 = \pm \infty$.

#### Hệ quả 2 {#alg-x-s8-prop-1-cor-2 .statement}

Cho
$$
0 \to M' \to M \to M'' \to 0
$$
là một dãy khớp của các $A$-môđun.

a) Ta có
$$
\mathrm{dp}_A(M) \leq \sup (\mathrm{dp}_A(M'), \mathrm{dp}_A(M'')) .
$$
Đẳng thức xảy ra ngay khi $\mathrm{dp}_A(M'') \neq \mathrm{dp}_A(M') + 1$.

b) Ta có
$$
\mathrm{dp}_A(M'') \leq \sup (\mathrm{dp}_A(M), \mathrm{dp}_A(M') + 1) .
$$
Đẳng thức xảy ra ngay khi $\mathrm{dp}_A(M) \neq \mathrm{dp}_A(M')$.

c) Ta có
$$
\mathrm{dp}_A(M') \leq \sup (\mathrm{dp}_A(M), \mathrm{dp}_A(M'') - 1) .
$$
Đẳng thức xảy ra ngay khi $\mathrm{dp}_A(M) \neq \mathrm{dp}_A(M'')$.

Hãy chứng minh chẳng hạn a), các chứng minh của b) và c) là tương tự.
Nếu N là một A-môđun tùy ý và n là một số nguyên $\geq 0$, ta có một dãy khớp
$$
\mathrm{Ext}_A^{n+1}(M'', N) \to \mathrm{Ext}_A^{n+1}(M, N) \to \mathrm{Ext}_A^{n+1}(M', N) \to \mathrm{Ext}_A^{n+2}(M'', N)
$$
$$
\to \mathrm{Ext}_A^{n+2}(M, N) .
$$
Nếu $\mathrm{dp}_A(M'), \mathrm{dp}_A(M'') \leq n$, thì $\mathrm{Ext}_A^{n+1}(M', N) = 0$ và $\mathrm{Ext}_A^{n+1}(M'', N) = 0$ (mệnh đề 1), do đó $\mathrm{Ext}_A^{n+1}(M, N) = 0$ và $\mathrm{dp}_A(M) \leq n$ (mệnh đề 1), do đó
$$
\mathrm{dp}_A(M) \leq \sup (\mathrm{dp}_A(M'), \mathrm{dp}_A(M'')) .
$$

Nếu $\mathrm{dp}_A(M)<\sup\bigl(\mathrm{dp}_A(M'),\mathrm{dp}_A(M'')\bigr)$, thì tất yếu $\mathrm{dp}_A(M)<+\infty$. Với mọi $n>\mathrm{dp}_A(M)$ và mọi A-môđun N, ta có

$$
\operatorname{Ext}_A^{n+1}(M',N)\ne0\Longleftrightarrow\operatorname{Ext}_A^{n+2}(M'',N)\ne0,
$$

theo dãy khớp trước đó; theo mệnh đề 1, điều này ngay lập tức suy ra $\mathrm{dp}_A(M'')=\mathrm{dp}_A(M')+1$, vì một trong các đại lượng $\mathrm{dp}_A(M')$, $\mathrm{dp}_A(M'')$ là $>\mathrm{dp}_A(M)$.

**Ví dụ.** — Cho $a$ là một phần tử của A không khả nghịch cũng không là một ước của không phải.
Khi đó $\mathrm{dp}_A(A/Aa)=1$.

Thật vậy, theo dãy khớp $0\longrightarrow A_s\xrightarrow{\varphi} A_s\longrightarrow A/Aa\longrightarrow0$, trong đó $\varphi(x)=xa$, ta có $\mathrm{dp}_A(A/Aa)\leq1$. Nếu $\mathrm{dp}_A(A/Aa)<1$, thì $A/Aa$ là xạ ảnh, và tồn tại một ánh xạ A-tuyến tính $\psi:A_s\longrightarrow A_s$ sao cho $\psi\circ\varphi=\mathrm{Id}$; điều này suy ra

$$
1=\psi(\varphi(1))=\psi(a)=a.\psi(1)
$$

và $a$ là khả nghịch.

#### Mệnh đề 2 {#alg-x-s8-prop-2 .statement}

Giả sử A là Noether trái. Cho M là một A-môđun sinh hữu hạn và n là một số nguyên $\geq0$. Các điều kiện sau là tương đương:

(i) $\mathrm{dp}_A(M)\leq n$.

(i bis) M có một phân giải xạ ảnh P có độ dài $\leq n$ sao cho $P_i$ là một A-môđun sinh hữu hạn với mỗi $i$.

(ii) $\operatorname{Ext}_A^r(M,N)=0$ với mọi A-môđun sinh hữu hạn N và mọi số nguyên $r>n$.

(iii) $\operatorname{Ext}_A^{n+1}(M,N)=0$ với mọi A-môđun sinh hữu hạn N.

(iv) $\operatorname{Tor}^A_r(P,M)=0$ với mọi A-môđun phải P và mọi $r>n$.

(v) $\operatorname{Tor}^A_{n+1}(A/a,M)=0$ với mọi iđêan phải sinh hữu hạn $a$ của A.

(i bis) $\Rightarrow$ (i) : điều này là tầm thường.

(i) $\Rightarrow$ (ii) : điều này suy ra từ Bổ đề 1.

(ii) $\Rightarrow$ (iii) : điều này là tầm thường.

(iii) $\Rightarrow$ (i) : theo (iii) và X, p. 107, mệnh đề 5, ta có $\operatorname{Ext}_A^{n+1}(M,N)=0$ với mọi A-môđun N, do đó (i) theo mệnh đề 1.

(i) $\Rightarrow$ (iv) : điều này suy ra từ Bổ đề 1.

(iv) $\Rightarrow$ (v) : điều này là tầm thường.

(v) $\Rightarrow$ (i bis) : cho (L,d) là một phân giải tự do của M sao cho $L_r$ sinh hữu hạn với mọi $r$ (X, p. 53, mệnh đề 6). Đặt $K=\mathrm{Z}_{n-1}(L)$; khi đó K là sinh hữu hạn như một môđun con của $L_{n-1}$ và ta có một dãy khớp

$$
0\longrightarrow K\longrightarrow L_{n-1}\longrightarrow L_{n-2}\longrightarrow\cdots\longrightarrow L_1\longrightarrow L_0\longrightarrow M\longrightarrow0.
\tag{1}
$$

Theo (v) và X, p. 131, hệ quả 3, ta có $\operatorname{Tor}^A_1(A/a,K)=0$ với mọi iđêan phải sinh hữu hạn $a$ của A. Theo định lý 2 của X, p. 74, A-môđun K là phẳng; vì nó sinh hữu hạn, do đó có biểu diễn hữu hạn (X, p. 10, mệnh đề 5), nên nó là xạ ảnh (X, p. 13, hệ quả), vậy (1) là một phân giải xạ ảnh của M.

#### Hệ quả {#alg-x-s8-n1-cor-1 .statement}

Giả sử $A$ là Noether trái và gọi $\mathcal{C}_0$ (tương ứng $\mathcal{C}$) là tập hợp các lớp của các $A$-môđun xạ ảnh kiểu hữu hạn (tương ứng của các $A$-môđun có chiều xạ ảnh hữu hạn và kiểu hữu hạn). Khi đó đồng cấu của các nhóm Grothendieck $K(\mathcal{C}_0) \to K(\mathcal{C})$ là song ánh.

Điều này suy ra từ X, p. 58, th. 1 (chú ý rằng $\mathcal{C}_0$ và $\mathcal{C}$ là khớp trái theo hệ quả 2).

### 2. Đồng cấu $\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_A(\operatorname{Ext}_A^n(M, A), P)$

Cho $M$ là một $A$-môđun trái, $P$ là một $A$-môđun phải, $n$ là một số nguyên $\geqslant 0$. Ánh xạ $k$-song tuyến tính (X, p. 129)

$$
c_{P;M,A_s} : \operatorname{Ext}_A^n(M, A) \times \operatorname{Tor}_n^A(P, M) \to P \otimes_A A
$$

tương ứng với một ánh xạ $k$-tuyến tính

(2)
$$
\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_k(\operatorname{Ext}_A^n(M, A), P);
$$

hơn nữa, nếu trang bị cho $\operatorname{Ext}_A^n(M, A)$ cấu trúc của $A$-môđun phải xuất phát từ cấu trúc song môđun của $A$, ảnh của (2) gồm các ánh xạ $A$-tuyến tính, như được kiểm tra ngay lập tức; điều này cho ta một $k$-đồng cấu, gọi là chính tắc

(3)
$$
\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_A(\operatorname{Ext}_A^n(M, A), P).
$$

#### Mệnh đề 3 {#alg-x-s8-prop-3 .statement}

a) Nếu $\mathrm{dp}_A(M) \leqslant n$, đồng cấu chính tắc (3) là đơn ánh.
b) Nếu $\mathrm{dp}_A(M) \leqslant n$, nếu $A$ là Noether trái và nếu $M$ là kiểu hữu hạn, đồng cấu chính tắc (3) là song ánh.

Ta lập luận bằng quy nạp theo $n$. Nếu $n = 0$, $M$ là xạ ảnh, đồng cấu (3) thu gọn thành đồng cấu chính tắc $P \otimes_A M \to \operatorname{Hom}_A(M^*, P)$ của II, p. 77, và mệnh đề suy ra từ loc. cit., hệ quả. Nếu $n > 0$, xét

(4)
$$
0 \to N \to L \to M \to 0
$$

là một dãy khớp của các $A$-môđun trong đó $L$ là tự do (và kiểu hữu hạn trong trường hợp b); khi đó $\mathrm{dp}_A(N) \leqslant n - 1$ (X, p. 135, hệ quả 2, c)) và $N$ là kiểu hữu hạn trong trường hợp b.

Cho $\theta \in \operatorname{Ext}_A^1(M, N)$ là lớp liên kết với dãy khớp (4) (X, p. 117, định nghĩa 1). Ký hiệu
$$
u_n : \operatorname{Ext}_A^{n-1}(N, A) \to \operatorname{Ext}_A^n(M, A) \qquad v_n : \operatorname{Tor}_n^A(P, M) \to \operatorname{Tor}_{n-1}^A(P, N)
$$
là các ánh xạ được xác định bởi $u_n(\alpha) = \alpha \circ \theta$ và $v_n(\beta) = \theta \circ \beta$. Ta có
$$
(\alpha \circ \theta) \circ \beta = \alpha \circ (\theta \circ \beta)
$$

với mọi $\alpha\in\operatorname{Ext}_A^{n-1}(N,A)$, $\beta\in\operatorname{Tor}_n^A(P,M)$ (X, p. 129, mệnh đề 6), do đó biểu đồ

$$
\begin{array}{ccc}
\operatorname{Tor}_n^A(P,M)&\longrightarrow&\operatorname{Hom}_A(\operatorname{Ext}_A^n(M,A),P)\\
\downarrow v_n&&\downarrow\operatorname{Hom}(u_n,1)\\
\operatorname{Tor}_{n-1}^A(P,N)&\longrightarrow&\operatorname{Hom}_A(\operatorname{Ext}_A^{n-1}(N,A),P),
\end{array}
\tag{5}
$$

trong đó các mũi tên ngang là các đồng cấu chính tắc, là giao hoán.

Nếu $n=1$, do đó ta có một biểu đồ giao hoán:

$$
\begin{array}{ccccc}
0&&&&0\\
\downarrow&&&&\downarrow\\
\operatorname{Tor}_1^A(P,M)&\longrightarrow&\operatorname{Hom}_A(\operatorname{Ext}_A^1(M,A),P)\\
\downarrow v_1&&&&\downarrow\operatorname{Hom}(u_1,1)\\
P\otimes_A N&\longrightarrow&\operatorname{Hom}_A(N^*,P)\\
\downarrow&&&&\downarrow\\
P\otimes_A L&\longrightarrow&\operatorname{Hom}_A(L^*,P)
\end{array}
$$

trong đó các cột là khớp; điều này cho kết quả trong trường hợp này. Nếu $n\geq 2$, các ánh xạ $u_n$ và $v_n$ là song ánh (X, p. 128, hệ quả 4 và p. 131, hệ quả 3). Theo giả thiết quy nạp, đồng cấu chính tắc

$$
\operatorname{Tor}_{n-1}^A(P,N)\longrightarrow\operatorname{Hom}_A(\operatorname{Ext}_A^{n-1}(N,A),P)
$$

là đơn ánh (tương ứng song ánh); biểu đồ (5) cho thấy điều tương tự đúng với đồng cấu chính tắc $\operatorname{Tor}_n^A(P,M)\longrightarrow\operatorname{Hom}_A(\operatorname{Ext}_A^n(M,A),P)$, điều này hoàn tất chứng minh.

### 3. Chiều đồng điều của một vành

#### Định nghĩa 2 {#alg-x-s8-def-2 .statement}

Ta gọi chiều đồng điều của $A$ và ký hiệu bởi $\operatorname{dh}(A)$ là cận trên trong $\mathbf{Z}$ của tập hợp các số nguyên $n$ sao cho tồn tại hai $A$-môđun M và N thỏa mãn $\operatorname{Ext}_A^n(M,N)\neq 0$.

Ta có $\operatorname{dh}(0)=-\infty$, $\operatorname{dh}(A)\geq 0$ nếu $A\neq 0$. Ta sẽ thấy dưới đây rằng $\operatorname{dh}(A)=1$ nếu $A$ là chính và không phải là một trường, và rằng, nếu K là một trường giao hoán

$$
\operatorname{dh}(K[X_1,\ldots,X_n])=n.
$$

#### Mệnh đề 4 {#alg-x-s8-prop-4 .statement}

Cho $n$ là một số nguyên $\geq 0$. Các điều kiện sau là tương đương:

(i) $\operatorname{dh}(A)\leq n$,

(ii) với mọi $A$-môđun M, ta có $\mathrm{dp}_A(M)\leq n$,

(ii′) với mọi $A$-môđun M sinh hữu hạn, ta có $\mathrm{dp}_A(M)\leq n$,

(iii) với mọi dãy khớp

$$
0 \to K \to P_{n-1} \to P_{n-2} \to \ldots \to P_0
$$

trong đó các $P_i$ là xạ ảnh, $K$ là xạ ảnh,

(iv) với mọi dãy khớp

$$
I^0 \to I^1 \to \ldots \to I^{n-1} \to N \to 0
$$

trong đó các $I^i$ là đơn ánh, $N$ là đơn ánh,

(v) mọi $A$-môđun đều có một giải đơn ánh có độ dài $\leq n$.

Sự tương đương của các điều kiện (i), (ii) và (iii) suy ra từ mệnh đề 1. Hiển nhiên ta có (ii) $\Rightarrow$ (ii′). Do đó chỉ cần chứng minh (ii’) $\Rightarrow$ (iv) $\Rightarrow$ (v) $\Rightarrow$ (i).

(ii’) $\Rightarrow$ (iv): với ký hiệu của (iv), gọi $K$ là hạt nhân của $I^0 \to I^1$. Theo X, p. 128, hệ quả 4, ta có với mọi $A$-môđun $M$ một đẳng cấu $\mathrm{Ext}_A^1(M, N) \to \mathrm{Ext}_A^{n+1}(M, K)$; từ đó suy ra theo (ii’) rằng $\mathrm{Ext}_A^1(M, N)$ bằng không đối với mọi $A$-môđun $M$ sinh hữu hạn. Theo X, p. 93, mệnh đề 11, điều này kéo theo rằng $N$ là đơn ánh, do đó (iv).

(iv) $\Rightarrow$ (v): cho $M$ là một $A$-môđun. Áp dụng (iv) cho dãy khớp

$$
0 \to M \to I^0(M) \to I^1(M) \to \ldots \to I^{n-1}(M) \to K^{n-1}(M) \to 0
$$

của X, p. 52, ta kết luận rằng $K^{n-1}(M)$ là đơn ánh, do đó (v).

(v) $\Rightarrow$ (i): điều này suy ra từ X, p. 100, định lý 1.

#### Nhận xét 1 {#alg-x-s8-n3-rem-1 .statement}

Nếu $\mathrm{dh}(A) \leq n < +\infty$, ta có $\mathrm{Tor}_{n+1}^A(P, M) = 0$ đối với mọi $A$-môđun $M$ và mọi $A$-môđun phải $P$, vì $\mathrm{dp}_A(M) \leq n$ (xem bổ đề 1).

#### Nhận xét 2 {#alg-x-s8-n3-rem-2 .statement}

Để $\mathrm{dh}(A)$ hữu hạn, điều kiện cần và đủ là $\mathrm{dp}_A(M)$ hữu hạn đối với mọi $A$-môđun khác không $M$. Điều này thực sự suy ra từ điều trên và từ X, p. 135, hệ quả 1.

#### Hệ quả {#alg-x-s8-n3-cor-1 .statement}

Giả sử $A$ là Noether trái và cho $n$ là một số nguyên $> 0$. Các điều kiện sau là tương đương:

(i) $\mathrm{dh}(A) \leq n$,

(ii) với mọi cặp $A$-môđun $M$ và $N$ có kiểu hữu hạn, ta có $\mathrm{Ext}_A^{n+1}(M, N) = 0$,

(iii) với mọi A-môđun trái $M$ kiểu hữu hạn và mọi A-môđun phải $P$ kiểu hữu hạn, ta có $\mathrm{Tor}_{n+1}^A(P, M) = 0$.

Điều này suy ra từ các Mệnh đề 2 và 4.

#### Nhận xét {#alg-x-s8-n3-rem-3 .statement}

Theo sự tương đương của (i) và (iii), ta có $\mathrm{dh}(A) = \mathrm{dh}(A^\circ)$ nếu $A$ là Noether trái và phải. Đẳng thức này không đúng trong trường hợp tổng quát (X, p. 204, Bài tập 20).

#### Mệnh đề 5 {#alg-x-s8-prop-5 .statement}

Giả sử $A$ là Noether trái và có chiều đồng điều hữu hạn, và gọi $\mathcal{C}_0$ (tương ứng $\mathcal{C}$) là tập hợp các lớp tương đương của các A-môđun xạ ảnh sinh hữu hạn (tương ứng của các A-môđun). Khi đó đồng cấu chính tắc của các nhóm Grothendieck $K(\mathcal{C}_0) \to K(\mathcal{C})$ là song ánh.

Điều này suy ra từ X, p. 137, Hệ quả.

### 4. Các vành có chiều đồng điều 0

#### Mệnh đề 6 {#alg-x-s8-prop-6 .statement}

Các điều kiện sau là tương đương :
(i) mọi A-môđun đều xạ ảnh,
(ii) mọi A-môđun đều đơn ánh,
(iii) mọi iđêan của $A$ là một môđun đơn ánh,
(iv) $\mathrm{dh}(A) \leq 0$,
(v) $A$ là nửa đơn,
(vi) $A$ là Noether và mọi A-môđun đều phẳng;
(vii) mọi phức của các A-môđun đều tách,
(viii) mọi dãy khớp của các A-môđun đều tách.

Theo Mệnh đề 4, ta có (i) ⇔ (ii) ⇔ (iv); theo Hệ quả 1 của Mệnh đề 4, ta có (vi) ⇒ (iv). Theo X, p. 35, Ví dụ 4, ta có (i) ⇒ (vii); vì (ii) ⇒ (iii) và (vii) ⇒ (viii) là tầm thường và vì (viii) ⇒ (i) suy ra từ II, p. 39, Mệnh đề 4, còn lại phải chứng minh (iii) ⇒ (v) và (v) ⇒ (vi); khẳng định cuối cùng suy ra từ VIII, § 5, No. 1, các Mệnh đề 1 và 2; cuối cùng, nếu mọi iđêan của $A$ là đơn ánh, thì nó là một nhân tử trực tiếp trong $A$, do đó (iii) ⇒ (v).

### 5. Các vành có chiều đồng điều 1

#### Mệnh đề 7 {#alg-x-s8-prop-7 .statement}

Các điều kiện sau là tương đương :
(i) $\mathrm{dh}(A) \leq 1$,
(ii) mọi môđun con của một môđun xạ ảnh là xạ ảnh,
(ii') mọi iđêan của $A$ là xạ ảnh,
(iii) mọi môđun thương của một A-môđun đơn ánh là đơn ánh,
(iv) với mọi phức xạ ảnh $C$, tồn tại một đồng cấu $\varphi : C \to H(C)$ sao cho $H(\varphi) = 1_{H(C)}$,
(v) với mọi phức đơn ánh $C$, tồn tại một đồng cấu $\psi : H(C) \to C$ sao cho $H(\psi) = 1_{H(C)}$.

(i) ⇔ (ii) ⇔ (iii) : điều này suy ra từ Mệnh đề 4 của X, p. 138.
(ii) ⇒ (iv) : cho $C$ là một phức xạ ảnh. Nếu (ii) được thỏa mãn, môđun con $B(C)$ của $C$ là xạ ảnh, do đó (iv) theo X, p. 35, Nhận xét b).
(iii) ⇒ (v) : cho $C$ là một phức đơn ánh. Nếu (iii) được thỏa mãn, môđun thương $B_n(C)$ của $C_{n+1}$ là đơn ánh với mọi $n$, do đó (v) theo X, p. 35, Nhận xét a).
(iv) ⇒ (ii) : cho $P$ là một A-môđun xạ ảnh, $M$ là một môđun con của $P$, và $i : M \to P$ là đơn ánh chính tắc. Cho $p : L \to M$ là một đồng cấu toàn ánh từ một môđun tự do $L$ lên $M$. Xét phức xạ ảnh $C$ sao cho $C_1 = L$, $C_0 = P$, $C_i = 0$ với $i \ne 0, 1$, và $d_1 = i \circ p$. Nếu (iv) được thỏa mãn, cho $\varphi : C \to H(C)$ là một đồng cấu sao cho $H(\varphi) = 1_{H(C)}$. Vì $H_1(C) = \mathrm{Ker}\ p$, $\varphi_1$ là một phép chiếu của $L$ lên $\mathrm{Ker}\ p$, do đó dãy khớp

$$
0 \to \mathrm{Ker}\ p \to L \xrightarrow{p} M \to 0
$$

là tách và $M$ đẳng cấu với một nhân tử trực tiếp của $L$, do đó xạ ảnh.

$(v)\Rightarrow(iii)$ : cho $I$ là một môđun đơn ánh, $M$ là một môđun thương của $I$, và $\pi : I \to M$ là phép chiếu chính tắc. Cho $i : M \to J$ là một đơn cấu của $M$ vào một môđun đơn ánh $J$. Xét phức đơn ánh $C$ sao cho $C^0 = I$, $C^1 = J$, $C^i = 0$ với $i \ne 0, 1$, và $d^0 = i \circ \pi$. Nếu (v) được thỏa mãn, cho $\psi : H(C) \to C$ là một đồng cấu sao cho $H(\psi) = 1_{H(C)}$. Vì

$$
H^1(C) = \operatorname{Coker}i,
$$

$\psi^1$ là một tiết diện của phép chiếu chính tắc $J \to \operatorname{Coker}i$, và $M$ là một nhân tử trực tiếp trong $J$, do đó đơn ánh.

$(ii)\Rightarrow(ii')$ : điều này là tầm thường.

$(ii')\Rightarrow(ii)$ : điều này suy ra từ VII, § 3, Hệ quả 1 của Định lý 1.

#### Ví dụ {#alg-x-s8-n5-exa-1 .statement}

Nếu $A$ là chính, thì $\operatorname{dh}(A) \leq 1$.

#### Nhận xét {#alg-x-s8-n5-rem-1 .statement}

Nếu $A$ là một miền (giao hoán), các điều kiện trước đó cũng tương đương với các điều kiện sau :

(iii') : mọi A-môđun chia được đều đơn ánh,

(vi) : mọi A-môđun không xoắn đều phẳng và $A$ là Noether.

Các miền thỏa mãn các điều kiện này được gọi là các vành Dedekind (xem X, p. 204, Bài tập 12 và AC, VII, § 2, No. 2, Th. 1).

#### Hệ quả {#alg-x-s8-n5-cor-1 .statement}

Cho $A$ là một vành có chiều đồng điều $\leq 1$, $C$ là một phức các A-môđun xạ ảnh, $\widetilde{C}$ là một phức các A-môđun phải xạ ảnh, $C'$ là một phức các A-môđun đơn ánh, $P$ là một A-môđun phải, $M$ là một A-môđun trái, và $n$ là một số nguyên. Khi đó tồn tại các dãy khớp tách

$$
0\to\bigoplus_{p+q=n}H_p(\widetilde C)\otimes_A H_q(C)\xrightarrow{\gamma}H_n(\widetilde C\otimes_A C)\xrightarrow{\alpha}\bigoplus_{p+q=n-1}\operatorname{Tor}_1^A(H_p(\widetilde C),H_q(C))\to0,
$$

$$
0\to\prod_p\operatorname{Ext}_A^1(H_p(C),H^{n-p-1}(C'))\xrightarrow{\beta}H^n(\operatorname{Homgr}_A(C,C'))\xrightarrow{\lambda}\prod_p\operatorname{Homgr}_A(H_p(C),H^{n-p}(C'))\to0,
$$

$$
0\to P\otimes_A H_n(C)\xrightarrow{\gamma}H_n(P\otimes_A C)\xrightarrow{\alpha}\operatorname{Tor}_1^A(P,H_{n-1}(C))\to0,
$$

$$
0\to\operatorname{Ext}_A^1(H_{n-1}(C),M)\xrightarrow{\beta}H^n(\operatorname{Homgr}_A(C,M))\xrightarrow{\lambda}\operatorname{Hom}_A(H_n(C),M)\to0.
$$

Vì $Z(C)$, $B(C)$, $Z(\widetilde C)$, và $B(\widetilde C)$ là xạ ảnh và $B(C')$ là đơn ánh, điều này suy ra từ X, p. 78, Hệ quả 2, p. 96, Hệ quả 1, và p. 98, Hệ quả 2.

### 6. Chiều đồng điều của các vành đa thức

#### Bổ đề 2 {#alg-x-s8-lem-2 .statement}

Cho $\rho : A\to A'$ là một đồng cấu vành, M là một A-môđun, M′ là một A′-môđun. Nếu A-môđun $A'_d$ là phẳng, ta có $\mathrm{dp}_A(A'\otimes_A M)\leq\mathrm{dp}_A(M)$. Nếu A-môđun $A'_s$ là xạ ảnh, ta có $\mathrm{dp}_A(M')\leq\mathrm{dp}_{A'}(M')$.

Mệnh đề đầu tiên là hiển nhiên nếu $\mathrm{dp}_A(M) = \pm \infty$; nếu $\mathrm{dp}_A(M) = n \in \mathbf{N}$, tồn tại một dãy khớp của các A-môđun

$$
0 \to P_n \to P_{n-1} \to \ldots \to P_0 \to M \to 0
$$

trong đó các $P_i$ là xạ ảnh ; dãy các A′-môđun

$$
0 \to A' \otimes_A P_n \to A' \otimes_A P_{n-1} \to \ldots \to A' \otimes_A P_0 \to A' \otimes_A M \to 0
$$

là khớp, vì $A'_d$ là phẳng, và các $A'$-môđun $A' \otimes_A P_i$ là xạ ảnh (II, p. 89, Hệ quả) ; do đó $\mathrm{dp}_{A'}(A' \otimes_A M) \leq n = \mathrm{dp}_A(M)$. Mệnh đề thứ hai là hiển nhiên nếu $\mathrm{dp}_{A'}(M') = \pm \infty$; nếu $\mathrm{dp}_{A'}(M') = m \in \mathbf{N}$, tồn tại một dãy khớp các $A'$-môđun

$$
0 \to P'_m \to P'_{m-1} \to \ldots \to P'_0 \to M' \to 0 ,
$$

trong đó các $P'_i$ là xạ ảnh ; dãy cơ sở của các $A$-môđun là khớp. Hơn nữa mỗi $P'_i$ là một nhân tử trực tiếp môđun con-$A'$ của một môđun ${A'_s}^{(1)}$, do đó là một $A$-môđun xạ ảnh ; do đó ta có $\mathrm{dp}_A(M') \leq m = \mathrm{dp}_{A'}(M')$.

#### Bổ đề 3 {#alg-x-s8-lem-3 .statement}

*Giả sử A giao hoán và cho M là một a[X]-môđun.*
  a) *Ta có* $\mathrm{dp}_A(M) \leq \mathrm{dp}_{A[X]}(M) \leq \mathrm{dp}_A(M) + 1$.
  b) *Nếu phép vị tự* $X_M$ *là đơn ánh, ta có* $\mathrm{dp}_A(M/XM) \leq \mathrm{dp}_{A[X]}(M)$.
  c) *Nếu* $XM = 0$, *ta có* $\mathrm{dp}_A(M) + 1 = \mathrm{dp}_{A[X]}(M)$.
  a) Ta có một dãy khớp các $A[X]$-môđun (III, p. 106 và VII, § 5, No. 1)

$$
0 \to A[X] \otimes_A M \to A[X] \otimes_A M \to M \to 0 ;
$$

Mệnh đề *a)* suy ra từ X, p. 135, Hệ quả 2 và Bổ đề 2.

*b)* Nếu $\mathrm{dp}_{A[X]}(M) = \pm \infty$, mệnh đề là tầm thường. Nếu $M$ là xạ ảnh và khác không, thì $A$-môđun $M/XM$ được đồng nhất với $A \otimes_{A[X]} M$, do đó là xạ ảnh, và ta có $\mathrm{dp}_A(M/XM) \leq 0 = \mathrm{dp}_{A[X]}(M)$. Ta lập luận bằng quy nạp theo $\mathrm{dp}_{A[X]}(M) = n$, giả sử $> 0$. Xét một dãy khớp các $A[X]$-môđun $0 \to N \to L \to M \to 0$, trong đó $L$ là một $A[X]$-môđun tự do ; áp dụng vào biểu đồ

$$
\begin{array}{ccc}
0 & \longrightarrow & N \longrightarrow L \longrightarrow M \longrightarrow 0 \\
& & \downarrow \quad \downarrow \quad \downarrow \\
0 & \longrightarrow & N \longrightarrow L \longrightarrow M \longrightarrow 0
\end{array}
$$

Mệnh đề 2 của X, p. 4, ta thấy rằng $X_N$ là đơn ánh và rằng ta có dãy khớp

$$
0 \to N/XN \to L/XL \to M/XM \to 0 .
$$

Vì $L$ là tự do trên $A[X]$, $L/XL$ là tự do trên $A$ và ta có

$$
\mathrm{dp}_{A[X]}(N) = n - 1 , \quad \mathrm{dp}_A(M/XM) \leq 1 + \mathrm{dp}_A(N/XN) ;
$$

vì $\mathrm{dp}_A(N/XN) \leq n - 1$ theo giả thiết quy nạp, ta suy ra $\mathrm{dp}_A(M/XM) \leq n$, điều này phải được chứng minh.

c) Mệnh đề là tầm thường nếu $\mathrm{dp}_{A[X]}(M) = \pm \infty$, và cũng nếu $\mathrm{dp}_{A[X]}(M) = 0$ (điều này là không thể vì $XM = 0$). Do đó ta có thể giả sử $\mathrm{dp}_{A[X]}(M) = n > 0$. Xét như trên một dãy khớp $0 \to N \to L \to M \to 0$, trong đó $L$ là một $A[X]$-môđun tự do, ta thu được một dãy khớp các $A$-môđun

$$
0 \to M \to N/XN \to L/XL \to M \to 0 .
$$

Theo b), ta có $\mathrm{dp}_A(N/XN) \leq \mathrm{dp}_{A[X]}(N) = \mathrm{dp}_{A[X]}(M) - 1 = n - 1$; vì $\mathrm{dp}_A(L/XL) = 0$, ta suy ra từ dãy khớp trước đó, áp dụng X hai lần, p. 135, Hệ quả 2, rằng $\mathrm{dp}_A(M) \leq n - 1$. Nhưng, theo a), ta có

$$
\mathrm{dp}_A(M) \geq \mathrm{dp}_{A[X]}(M) - 1 = n - 1 ,
$$

do đó c).

#### Định lý 1 {#alg-x-s8-thm-1 .statement}

*Giả sử $A$ giao hoán. Khi đó*

$$
dh(A[X]) = dh(A) + 1 .
$$

Đối với mọi $A[X]$-môđun $M$, ta có (*bổ đề 3*)

$$
\mathrm{dp}_{A[X]}(M) \leq \mathrm{dp}_A(M) + 1 \leq dh(A) + 1
$$

do đó $dh(A[X]) \leq dh(A) + 1$; ngược lại, nếu $M$ là một $A$-môđun, gọi $\overline{M}$ là $A[X]$-môđun thu được bằng cách trang bị cho $M$ cấu trúc mà theo đó $XM = 0$, khi đó (*bổ đề 3*)

$$
\mathrm{dp}_A(M) = \mathrm{dp}_{A[X]}(\overline{M}) - 1 \leq dh(A[X]) - 1 ,
$$

do đó $dh(A) \leq dh(A[X]) - 1$.

#### Hệ quả 1 {#alg-x-s8-thm-1-cor-1 .statement}

*Giả sử $A$ giao hoán. Ta có*

$$
dh(A[X_1, ..., X_n]) = dh(A) + n .
$$

Điều này suy ra từ định lý bằng quy nạp theo $n$.

#### Hệ quả 2 {#alg-x-s8-thm-1-cor-2 .statement}

*Cho $K$ là một trường giao hoán* (tương ứng *một miền iđêan chính* *hoặc một vành Dedekind* *không là trường*). *Khi đó* $dh(K[X_1, ..., X_n])$ *bằng* $n$ (tương ứng $n + 1$). Điều này suy ra từ sự kiện rằng $dh(K) = 0$ (tương ứng $dh(K) = 1$).

### 7. Chiều đồng điều của các môđun phân bậc

Trong tiết diện này, ta giả sử rằng $A$ là một vành phân bậc với các bậc $\geq 0$. Ta ký hiệu bởi $(A_n)_{n \in \mathbf{Z}}$ sự phân bậc của nó; do đó ta có $A_n = 0$ với $n < 0$, $A_0$ là một vành con của $A$, $J_0 = \bigoplus_{n > 0} A_n$ là một iđêan hai phía của $A$ và vành thương phân bậc $A/J_0$ được đồng nhất với $A_0$.

#### Bổ đề 4 {#alg-x-s8-lem-4 .statement}

Cho $M$ là một $A$-môđun phân bậc bị chặn dưới (X, p. 56). Nếu $A_0 \otimes_A M = 0$, thì $M = 0$.

Vì $A_0 \otimes_A M$ đẳng cấu với $M/J_0 M$, đây chính là ll, p. 171, mệnh đề 6.

#### Bổ đề 5 {#alg-x-s8-lem-5 .statement}

Cho $M$ là một $A$-môđun phân bậc bị chặn dưới, và cho
$$
s : A \otimes_{A_0} M/J_0 M \to M
$$
là một đồng cấu $A$ phân bậc sao cho $1 \otimes_A s : A_0 \otimes_A (A \otimes_{A_0} M/J_0 M) \to A_0 \otimes_A M$ là đẳng cấu chính tắc. Khi đó $s$ là toàn ánh. Nếu $\mathrm{Tor}_1^A(A_0, M) = 0$, $s$ là song ánh.

Ta có một dãy khớp
$$
0 \to \mathrm{Ker}\ s \to A \otimes_{A_0} M J_0 M \to M \to \mathrm{Coker}\ s \to 0
$$
và các $A$-môđun phân bậc $\mathrm{Ker}\ s$ và $\mathrm{Coker}\ s$ bị chặn dưới. Từ dãy khớp $A_0 \otimes_A (A \otimes_{A_0} M/J_0 M) \xrightarrow{1 \otimes s} A_0 \otimes_A M \to A_0 \otimes_A \mathrm{Coker}\ s \to 0$, ta suy ra rằng $A_0 \otimes_A \mathrm{Coker}\ s = 0$, do đó $s$ là toàn ánh (Bổ đề 4). Khi đó ta có một dãy khớp
$$
\mathrm{Tor}_1^A(A_0, M) \to A_0 \otimes_A \mathrm{Ker}\ s \to A_0 \otimes_A (A \otimes_{A_0} M/J_0 M) \xrightarrow{1 \otimes s} A_0 \otimes_A M .
$$
Nếu $\mathrm{Tor}_1^A(A_0, M) = 0$, thì $A_0 \otimes_A \mathrm{Ker}\ s = 0$ và $s$ là đơn ánh (Bổ đề 4).

#### Mệnh đề 8 {#alg-x-s8-prop-8 .statement}

Cho $M$ là một $A$-môđun phân bậc bị chặn dưới.

a) Các điều kiện sau là tương đương :
(i) $M$ đẳng cấu với một $A$-môđun phân bậc có dạng $A \otimes_{A_0} N$, trong đó $N$ là một $A_0$-môđun phân bậc xạ ảnh (tương ứng, tự do phân bậc) ;
(ii) $M$ là một $A$-môđun xạ ảnh (tương ứng, tự do phân bậc) ;
(iii) $M/J_0 M$ là một $A_0$-môđun xạ ảnh (tương ứng, tự do phân bậc) và $\mathrm{Tor}_1^A(A_0, M) = 0$.

b) Giả sử thêm rằng $M$ có một hệ phần tử sinh gồm các phần tử thuần nhất có các bậc bị chặn. Khi đó các điều kiện sau là tương đương :
(i) $A$-môđun phân bậc $M$ có một chuỗi hợp thành hữu hạn mà các thương của nó đẳng cấu với các $A$-môđun phân bậc có dạng $A \otimes_{A_0} N$, trong đó $N$ là một $A_0$-môđun phân bậc phẳng ;
(ii) $M$ là một $A$-môđun phẳng ;
(iii) $M/J_0 M$ là một $A_0$-môđun phẳng và $\mathrm{Tor}_1^A(A_0, M) = 0$.

Trong mỗi trường hợp, hiển nhiên có (i) ⇒ (ii) ⇒ (iii). Do đó, còn phải chứng minh (iii) ⇒ (i).

a) $A$-môđun phân bậc $A \otimes_{A_0} M/J_0 M$ là một $A$-môđun xạ ảnh vì $M/J_0 M$ là một $A_0$-môđun xạ ảnh. Đồng cấu chính tắc của các $A$-môđun
$$
p : M \to M/J_0 M
$$
là toàn ánh ; do đó tồn tại một đồng cấu $A$-môđun phân bậc bậc không
$$
s : A \otimes_{A_0} M/J_0 M \to M
$$
sao cho $p \circ s(a \otimes x) = ax$ với $a \in A$ và $x \in M/J_0 M$.

Theo Bổ đề 5, $s$ là một đẳng cấu của các $A$-môđun từ $A\otimes_{A_0}M/J_0M$ lên $M$, do đó (i).

b) Theo giả thiết về $M$, tồn tại các số nguyên $a,b$ với $a\leq b$ sao cho $M$ được sinh bởi $\displaystyle\bigoplus_{a\leq i\leq b}M_i$. Ta lập luận bằng quy nạp theo số nguyên dương $b-a$.

Nếu $b-a=0$, thì $M$ được sinh bởi $M_a$ và đồng cấu $A_0$-môđun chính tắc
$$
M_a\longrightarrow M/J_0M
$$
là song ánh; khi đó ta suy ra từ đồng cấu $A$-môđun $A\otimes_{A_0}M_a\longrightarrow M$ được xác định bởi cấu trúc $A$-môđun của $M$ một đồng cấu $A$-môđun phân bậc
$$
s:A\otimes_{A_0}M/J_0M\longrightarrow M
$$
thỏa mãn điều kiện của Bổ đề 5. Khi đó, theo Bổ đề 5, $s$ là song ánh, do đó (i).

Trong trường hợp tổng quát, đặt $M^{(a)}$ là môđun con-$A$ (phân bậc) của $M$ sinh bởi $M_a$ và $M'$ là môđun thương $M/M^{(a)}$. Ta có một dãy khớp
$$
0\longrightarrow M^{(a)}\xrightarrow{f}M\xrightarrow{g}M'\longrightarrow0,
$$
do đó, vì $\operatorname{Tor}_1^A(A_0,M)=0$ theo giả thiết, các dãy khớp
$$
\tag{6}
\operatorname{Tor}_2^A(A_0,M')\longrightarrow\operatorname{Tor}_1^A(A_0,M^{(a)})\longrightarrow0
$$
$$
\tag{7}
0\longrightarrow\operatorname{Tor}_1^A(A_0,M')\longrightarrow M^{(a)}/J_0M^{(a)}
\xrightarrow{1\otimes f}M/J_0M\xrightarrow{1\otimes g}M'/J_0M'\longrightarrow0.
$$

Nhưng đồng cấu chính tắc $M_a\longrightarrow M^{(a)}/J_0M^{(a)}$ là song ánh. Suy ra rằng đồng cấu $1\otimes f:M^{(a)}/J_0M^{(a)}\longrightarrow M/J_0M$ là đơn ánh và ảnh của nó là một môđun con hạng tử trực tiếp-$A_0$ của $M/J_0M$. Khi đó từ dãy khớp (7) suy ra $\operatorname{Tor}_1^A(A_0,M')=0$ và môđun-$A_0$ $M'/J_0M'$ là phẳng vì đẳng cấu với một nhân tử trực tiếp của $M/J_0M$. Theo giả thiết quy nạp (áp dụng cho $M'$ vì nó được sinh bởi các $M'_i$ với $a<i\leq b$), $M'$ thỏa mãn điều kiện (i), do đó là phẳng. Ta suy ra từ dãy khớp (6) rằng $\operatorname{Tor}_1^A(A_0,M^{(a)})=0$, nhưng $M^{(a)}/J_0M^{(a)}$ được đồng nhất với $M_a$, là một môđun-$A_0$ phẳng (như một môđun con hạng tử trực tiếp của $M/J_0M$) ; theo điều đã được chứng minh, môđun $A$ phân bậc $M^{(a)}$ đẳng cấu với $A\otimes_{A_0}M_a$, do đó cũng thỏa mãn (i), điều này hoàn tất chứng minh.

#### Hệ quả 1 {#alg-x-s8-prop-8-cor-1 .statement}

Cho $M$ là một môđun $A$ phân bậc kiểu hữu hạn. Nếu môđun-$A_0$ $M/J_0M$ là xạ ảnh (tương ứng, tự do phân bậc, tương ứng, phẳng) và nếu $\operatorname{Tor}_1^A(A_0,M)=0$, thì môđun-$A$ $M$ là xạ ảnh (tương ứng, tự do phân bậc, tương ứng, phẳng).

#### Hệ quả 2 {#alg-x-s8-prop-8-cor-2 .statement}

#### Hệ quả 3 (Định lý Syzygy của Hilbert) {#alg-x-s8-prop-8-cor-3 .statement}
*Giả sử rằng $A_0$ là một trường giao hoán và rằng $A$ được sinh như một $A_0$-đại số bởi $n$ phần tử thuần nhất có bậc > 0 và độc lập đại số. Với mọi môđun $a$ phân bậc $M$ bị chặn dưới (tương ứng, kiểu hữu hạn), tồn tại một dãy khớp của các môđun $a$ phân bậc và các ánh xạ thuần nhất bậc $0$*
$$
0 \to L_n \to L_{n-1} \to \ldots \to L_0 \to M \to 0,
$$
trong đó các $L_i$ là tự do phân bậc và bị chặn dưới (tương ứng, tự do phân bậc và kiểu hữu hạn).

Thật vậy, $dh(A) = n$ theo Định lý 1 của X, p. 143, và Hệ quả 2 được áp dụng.

#### Nhận xét {#alg-x-s8-n7-rem-1 .statement}
*Hệ quả 2 cũng áp dụng trong các trường hợp sau:
a) $A_0$ là chính và $A = A_0[X_1, ..., X_{n-1}]$;
b) $A_0$ là một vành Noether địa phương chính quy có chiều $r$ và $A = A_0[X_1, ..., X_n, r]$.*

#### Hệ quả 4 {#alg-x-s8-prop-8-cor-4 .statement}
*Giả sử rằng $A_0$ là nửa đơn. Cho $M$ là một $a$-môđun phân bậc bị chặn dưới và cho $n$ là một số nguyên $\geq 0$. Để $\mathrm{dp}_A(M) \leq n$, điều kiện cần và đủ là*
$$
\operatorname{Tor}_{n+1}^A(A_0, M) = 0.
$$
Nếu $\mathrm{dp}_A(M) \leq n$, thì $\operatorname{Tor}_{n+1}^A(A_0, M) = 0$ (X, p. 135, Bổ đề 1). Ngược lại, xét $\dots \to L_1 \to L_0 \to M \to 0$ là một dãy khớp của các $a$-môđun phân bậc bị chặn dưới sao cho $L_0, \dots, L_{n-1}$ là tự do phân bậc (X, p. 56, Mệnh đề 11); theo Hệ quả 3 của X, p. 131, đẳng thức $\operatorname{Tor}_{n+1}^A(A_0, M) = 0$ kéo theo $\operatorname{Tor}_1^A(A_0, K) = 0$; vì $K/J_0 K$ là một $A_0$-môđun xạ ảnh bởi vì $A_0$ là nửa đơn (X, p. 140, Mệnh đề 6), $K$ là xạ ảnh theo Mệnh đề 8 (X, p. 144), và $\mathrm{dp}_A(M) \leq n$.

#### Hệ quả 5 {#alg-x-s8-prop-8-cor-5 .statement}

*Giả sử vành $A_0$ nửa đơn. Nếu $\operatorname{Tor}_{n+1}^A(A_0, A_0) = 0$, ta có $\mathrm{dp}_A(M) \leq n$ đối với mọi $A$-môđun phân bậc bị chặn dưới.

Ký hiệu $A^\circ$ là vành phân bậc đối của $A$: ta có $(A^\circ)_0 = (A_0)^\circ$, do đó $(A^\circ)_0$ là nửa đơn (VIII, § 5, No. 1, nhận xét 3). Vì $\operatorname{Tor}_{n+1}^{A^\circ}(A_0^\circ, A_0^\circ) = 0$, ta có $\mathrm{dp}_A(A_{0s}^\circ) \leq n$ theo hệ quả 4: điều này kéo theo $\operatorname{Tor}_{n+1}^{A^\circ}(M_0, A_0^\circ) = 0$ đối với mọi $A$-môđun $M$, do đó $\operatorname{Tor}_{n+1}^A(A_0, M) = 0$ và ta áp dụng hệ quả 4.

## BÀI TẬP {#alg-x-s8-exercises}

Xem [các bài tập cho § 8](exercises/s8/).
