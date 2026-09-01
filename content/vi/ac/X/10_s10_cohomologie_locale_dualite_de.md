---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 10
section_title: Cohomologie locale, dualité de Grothendieck
lang: vi
source: ac-x-fr
pdf_pages: 0141-0150, 0178-0180
extraction: ocr
subsections:
    - "no": 1
      title: Cohomologie locale
      page: 0
      pdf_page: 141
    - "no": 2
      title: Cohomologie locale sur un anneau de Macaulay
      page: 145
      pdf_page: 144
    - "no": 3
      title: Dualité de Grothendieck sur un anneau de Macaulay
      page: 147
      pdf_page: 146
statements: 20
exercises: 11
content_sha256: af4b6263538812699d538a89c1512c5b179a2691698e0256b43b8ad8bb653f21
translated_from: content/en-mt/ac/X/10_s10_cohomologie_locale_dualite_de.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 5249772d053544eedc1734bed7c660da3174e2c1d5383a26977e65276609f491
translation_model: gpt-5.4
translation_run: translate-vi-61362ecd
glossary_version: 34
glossary_terms_sha256: d04858cc2552a2d75012ecca1ebdb98e81256a6d53b9b560eae2753ee5e5c396
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 10. ĐỐI ĐỒNG ĐIỀU ĐỊA PHƯƠNG, ĐỐI NGẪU GROTHENDIECK

### 1. Đối đồng điều địa phương

Trong No. này, ta xét một vành địa phương Noether $A$. Nhắc lại (VIII, § 3, No. 3, Bổ đề 2) rằng các iđêan định nghĩa của $A$ là các iđêan của $A$ phân biệt với $A$ và chứa một lũy thừa của $m_A$, hay cũng lại là các iđêan $a \subset m_A$ sao cho $A/a$ có độ dài hữu hạn. Ta ký hiệu bởi $\mathscr{D}$ tập hợp các iđêan định nghĩa của $A$, được trang bị quan hệ thứ tự đối với bao hàm; nó lọc phải.

Cho $M$ là một $A$-môđun. Với mỗi iđêan định nghĩa $a$ của $A$, ta liên kết A-môđun phân bậc $\mathrm{Ext}_A(A/a, M)$; nếu $a$ và $b$ là các iđêan định nghĩa với $a \subset b$, ký hiệu bởi $p_{ab} : A/a \to A/b$ ánh xạ chính tắc và xét ánh xạ $A$-tuyến tính $\mathrm{Ext}(p_{ab}, 1_M) : \mathrm{Ext}_A(A/b, M) \longrightarrow \mathrm{Ext}_A(A/a, M)$. Như vậy ta thu được một hệ quy nạp các A-môđun phân bậc và các ánh xạ $A$-tuyến tính phân bậc bậc 0 đối với tập hợp có thứ tự $\mathscr{D}$. A-môđun phân bậc $\varprojlim_{a \in \mathscr{D}} \mathrm{Ext}_A(A/a, M)$ được gọi là *môđun đối đồng điều địa phương* của $M$, và được ký hiệu bởi $H_A(M)$.

Các iđêan $m_A^n$ với $n \geq 1$ tạo thành một tập con đồng tận của $\mathscr{D}$; do đó có một đẳng cấu chính tắc của các môđun phân bậc $\varprojlim_n \mathrm{Ext}_A(A/m_A^n, M) \longrightarrow H_A(M)$. Suy ra rằng mọi phần tử của $H_A(M)$ đều bị triệt tiêu bởi một lũy thừa của $m_A$.

#### Nhận xét 1 {#ac-x-s10-n1-rem-1 .statement}

Cho $X$ là không gian tôpô $\mathrm{Spec}(A)$, $\mathcal{O}_X$ bó cấu trúc các vành và $\widetilde{M}$ môđun $\mathcal{O}_X$ liên kết với $M$. A-môđun phân bậc $H_A(M)$ được đồng nhất với môđun $H_{\{m_A\}}(X, \widetilde{M})$ của đối đồng điều có giá trong điểm đóng $m_A$ của $X$.

Với mọi đồng cấu $f : M \to N$ của các $A$-môđun, các ánh xạ $\mathrm{Ext}_A(1_{A/a}, f) : \mathrm{Ext}_A(A/a, M) \longrightarrow \mathrm{Ext}_A(A/a, N)$ tạo thành một hệ quy nạp các ánh xạ tuyến tính phân bậc. Khi chuyển qua giới hạn quy nạp, ta thu được một đồng cấu phân bậc $H_A(f) : H_A(M) \to H_A(N)$. Với mọi dãy $M \xrightarrow{f} N \xrightarrow{g} P$ các $A$-môđun và đồng cấu, ta có $H_A(g \circ f) = H_A(g) \circ H_A(f)$. Cho

$$
\begin{array}{ccccccccc}
0 & \to & M & \xrightarrow{f} & N & \xrightarrow{g} & P & \to & 0
\end{array}
$$

là một dãy khớp các $A$-môđun. Theo $\Lambda$, X, p. 90, Prop. 8, các đồng cấu nối của các môđun mở rộng $\mathrm{Ext}_A(A/a, P) \longrightarrow \mathrm{Ext}_A(A/a, M)$ tạo thành một hệ quy nạp các ánh xạ $A$-tuyến tính, phân bậc bậc (tăng) +1. Khi chuyển qua giới hạn quy nạp, ta suy ra một đồng cấu $A$ $\partial(\mathscr{E}) : H_A(P) \to H_A(M)$, phân bậc bậc +1, làm cho dãy đồng cấu

$$
\ldots \longrightarrow H_A^{n-1}(P) \xrightarrow{\partial^{n-1}(\mathscr{E})} H_A^n(M) \xrightarrow{H_A^n(f)} H_A^n(N) \xrightarrow{H_A^n(g)} H_A^n(P) \xrightarrow{\partial^n(\mathscr{E})} H_A^{n+1}(M) \longrightarrow \ldots
$$

là khớp.

Cho M là một A-môđun. Với mọi iđêan $\alpha$ của A, A-môđun $\mathrm{Hom}_A(A/\alpha, M)$ được đồng nhất một cách chính tắc với môđun con của M gồm các phần tử bị triệt tiêu bởi $\alpha$. Do đó $H_A^0(M)$ được đồng nhất với môđun con của M gồm các phần tử $m$ bị triệt tiêu bởi một lũy thừa của $\mathfrak{m}_A$, nghĩa là sao cho $\mathrm{long}_A(Am) < +\infty$. Đặc biệt có $H_A^0(M) = M$ khi M là Artin.

#### Ví dụ 1 {#ac-x-s10-n1-exa-1 .statement}

Nếu M là nội xạ, A-môđun $H_A^i(M)$ bằng không với $i > 0$ và nội xạ với $i = 0$ (§ 8, No. 2, bổ đề 1, c)).

#### Ví dụ 2 {#ac-x-s10-n1-exa-2 .statement}

Nếu $H_A^0(M) = M$ (chẳng hạn nếu M là Artin), thì $H_A^i(M)$ bằng không với $i > 0$. Thật vậy, gọi (I, e) là một bao nội xạ của M. Môđun con $H_A^0(I)$ của I là nội xạ (ví dụ 1) và chứa $e(M)$, nên bằng I. Đặt $N = \mathrm{Coker}\,e$ và xét dãy khớp $0 \to M \xrightarrow{e} I \xrightarrow{p} N \to 0$. Vì $I = H_A^0(I)$, nên có $N = H_A^0(N)$ và đồng cấu $H_A^0(p)$ là toàn ánh. Vì $H_A^i(I)$ bằng không với $i > 0$ (ví dụ 1), $H_A^1(M)$ bằng không và $H_A^i(M)$ đẳng cấu với $H_A^{i-1}(N)$ với $i > 1$; kết luận bằng lập luận quy nạp theo số nguyên $i$.

#### Ví dụ 3 {#ac-x-s10-n1-exa-3 .statement}

Cho $\Omega$ là một A-môđun đối ngẫu hóa. Với $i \neq \dim(A)$, có $\mathrm{Ext}_A^i(A/\alpha, \Omega) = 0$ với mọi iđêan định nghĩa $\alpha$ của A (§ 8, No. 5, ví dụ 3), do đó $H_A^i(\Omega) = 0$; với $i = \dim(A)$, A-môđun $H_A^i(\Omega)$, đẳng cấu với $\varprojlim \mathrm{Ext}_A^i(A/\mathfrak{m}_A^n, \Omega)$, là một môđun Matlis (*loc. cit.*, ví dụ 6).

#### Ví dụ 4 {#ac-x-s10-n1-exa-4 .statement}

Cho A là một vành địa phương nguyên Noether; gọi K là trường phân thức của nó, và giả sử rằng $A \neq K$. Nó là một A-môđun nội xạ (A, X, p. 18, ví dụ 1), nên môđun $H_A(K)$ bằng không (ví dụ 1). Từ dãy khớp $0 \to A \to K \to K/A \to 0$, ta thu được với mọi $i$ một đẳng cấu $H_A^i(K/\Lambda) \to H_A^{i+1}(A)$.

Nói chung hơn, với mọi A-môđun không xoắn M và mọi số nguyên $i$, từ dãy khớp

$$
0 \to M \to K \otimes_A M \to (K/A) \otimes_A M \to 0
$$

ta suy ra một đẳng cấu $H_A^i((K/A) \otimes_A M) \to H_A^{i+1}(M)$.

#### Ví dụ 5 {#ac-x-s10-n1-exa-5 .statement}

Giữ các giả thiết của ví dụ trước và giả sử thêm rằng $\dim(A) = 1$. Cho N là một A-môđun xoắn; vì mọi iđêan khác không của A phân biệt với A đều là một iđêan định nghĩa (VIII, § 1, No. 3, mệnh đề 6, e)), nên có $H_A^0(N) = N$, và do đó $H_A^i(N) = 0$ với $i > 0$ (ví dụ 2).

Cho M là một A-môđun; gọi $T(M)$ là môđun con xoắn của nó. Xét dãy đối đồng điều địa phương khớp dài liên kết với dãy khớp

$$
0 \to T(M) \to M \to M/T(M) \to 0 ;
$$

theo điều vừa nói ở trên, từ đó ta suy ra các đẳng cấu chính tắc $T(M) \to H_A^0(M)$ và $H_A^1(M) \to H_A^1(M/T(M))$. Vì đồng cấu chính tắc $(K/A) \otimes_A M \to (K/A) \otimes_A (M/T(M))$ là song ánh, cuối cùng ta thu được các *đẳng cấu chính tắc*

$$
H_A^0(M) \to T(M) , \qquad H_A^1(M) \to (K/A) \otimes_A M .
$$

#### Mệnh đề 1 {#ac-x-s10-prop-1 .statement}

Cho $A$ là một vành địa phương Noether và $M$ là một $A$-môđun sinh hữu hạn.

a) $A$-môđun $H_A(M)$ là Artin, và bằng không trong bậc $> \dim(M)$.

b) Đặt $p = \operatorname{prof}_A(M)$. Ta có $H_A^i(M) = 0$ với $i < p$, và $H_A^p(M) \neq 0$ nếu $M$ khác không.

Hãy chứng minh a) bằng quy nạp theo $\dim(M)$. Trường hợp $\dim(M) \leq 0$ suy ra từ Ví dụ 2 ở trên. Giả sử $\dim(M) > 0$ và trước hết lấy $M$ có dạng $A/\mathfrak{p}$, trong đó $\mathfrak{p}$ là một iđêan nguyên tố của $A$ phân biệt với $\mathfrak{m}_A$. Gọi $x$ là một phần tử của $\mathfrak{m}_A - \mathfrak{p}$; ta có một dãy khớp $0 \to M \xrightarrow{xM} M \longrightarrow M/xM \to 0$, với $\dim(M/xM) = \dim(M) - 1$. Do đó ta suy ra một dãy khớp của đối đồng điều địa phương

$$
H_A^{i-1}(M/xM) \longrightarrow H_A^i(M) \xrightarrow{x} H_A^i(M)
$$

Mọi phần tử của $H_A^i(M)$ đều bị triệt tiêu bởi một lũy thừa của $\mathfrak{m}_A$; để chứng minh rằng môđun này là Artin, do đó chỉ cần chứng minh rằng đế của $H_A^i(M)$ có số chiều hữu hạn trên $\kappa_A$ (§ 8, No. 3, Bổ đề 3). Theo giả thiết quy nạp, hạt nhân $N$ của phép vị tự tỉ số $x$ trong $H_A^i(M)$ là Artin; vì $x$ thuộc $\mathfrak{m}_A$, đế của $H_A^i(M)$ đồng nhất với đế của $N$, và do đó có số chiều hữu hạn. Nếu $i > \dim(M)$, ta có $H_A^{i-1}(M/xM) = 0$ theo giả thiết quy nạp, nên phép vị tự tỉ số $x$ là đơn ánh trong $H_A^i(M)$; vì mọi phần tử của $H_A^i(M)$ đều bị triệt tiêu bởi một lũy thừa của $x$, ta suy ra $H_A^i(M) = 0$, do đó được a) trong trường hợp đang xét.

Hãy chuyển sang trường hợp tổng quát. A-môđun $M$ thừa nhận một chuỗi hợp thành $(M_j)_{0 \leq j \leq n}$ sao cho mỗi thương $M_j/M_{j+1}$ đẳng cấu với $A/\mathfrak{p}_j$, trong đó $\mathfrak{p}_j$ là một iđêan nguyên tố của $A$ (IV, § 1, No. 4, Định lý 1). Hãy chứng minh bằng quy nạp theo $n$ rằng $M$ thỏa mãn a). Trường hợp $n = 0$ là tầm thường. Dãy khớp $0 \to M_1 \to M \to A/\mathfrak{p}_0 \to 0$ cho một dãy khớp của đối đồng điều địa phương

$$
H_A^i(M_1) \longrightarrow H_A^i(M) \longrightarrow H_A^i(A/\mathfrak{p}_0)
$$

A-môđun $H_A^i(M_1)$ là Artin theo giả thiết quy nạp, và điều đó cũng đúng với $H_A^i(A/\mathfrak{p}_0)$ theo các trường hợp đã xét; do đó $H_A^i(M)$ là Artin. Nếu $i > \dim(M)$, các môđun $M_1$ và $A/\mathfrak{p}_0$ có chiều $< i$; vì vậy các môđun $H_A^i(M_1)$ và $H_A^i(A/\mathfrak{p}_0)$ bằng không theo giả thiết quy nạp và các trường hợp đã xét, điều này suy ra $H_A^i(M) = 0$.

Giả sử $M$ khác không, và hãy chứng minh b) bằng quy nạp theo số nguyên $p = \operatorname{prof}(M)$. Trường hợp $p = 0$ suy ra từ định nghĩa của độ sâu. Giả sử $p > 0$ và chọn một phần tử $x$ của $\mathfrak{m}_A$ sao cho phép vị tự $x_M$ là đơn ánh. Như trên ta thu được một dãy khớp đối đồng điều địa phương

$$
H_A^{i-1}(M/xM) \longrightarrow H_A^i(M) \xrightarrow{x} H_A^i(M)
$$

Ta có $\operatorname{prof}(M/xM) = \operatorname{prof}(M) - 1$ (§ 1, No. 4, prop. 7), do đó $H_A^{i-1}(M/xM) = 0$ với $i < p$ theo giả thiết quy nạp, điều này kéo theo như trên rằng $H_A^i(M) = 0$. Đặc biệt $H_A^{p-1}(M)$ bằng không, nên đồng cấu $H_A^{p-1}(M/xM) \longrightarrow H_A^p(M)$ là đơn ánh; vì thế $H_A^p(M)$ khác không theo giả thiết quy nạp.

Có thể chứng minh rằng môđun $H_A^{\dim(M)}(M)$ khác không khi $M$ khác không (bài tập 4; xem No. 3, hệ quả của định lý 2).

#### Hệ quả {#ac-x-s10-n1-cor-1 .statement}

**Cho $M$ là một $A$-môđun Macaulay khác không, kiểu hữu hạn. $A$-môđun $H_A^i(M)$ bằng không với $i \neq \dim(M)$ và khác không với $i = \dim(M)$.**

#### Nhận xét 2 {#ac-x-s10-n1-rem-2 .statement}

Với mọi iđêan định nghĩa $\alpha$ của $A$, $A$-môđun $\mathrm{Ext}_A(A/\alpha, M)$ bị triệt tiêu bởi $\alpha$, và $A/\alpha$ được đồng nhất với $\widehat{A}/\alpha \widehat{A}$; do đó, $A$-môđun phân bậc $\mathrm{Ext}_A(A/\alpha, M)$ được đồng nhất với $\widehat{A} \otimes_A \mathrm{Ext}_A(A/\alpha, M)$, vì thế cũng với $\mathrm{Ext}_{\widehat{A}}(\widehat{A}/\alpha \widehat{A}, \widehat{A} \otimes_A M)$ (A, X, p. 111, prop. 10). Tập hợp các iđêan $\alpha \widehat{A}$, với $\alpha \in \mathscr{D}$, chứa các lũy thừa của $m_{\widehat{A}}$, nên là đồng cuối trong tập hợp các iđêan định nghĩa của $\widehat{A}$; do đó từ những điều trên ta suy ra một đẳng cấu chính tắc của các $A$-môđun phân bậc

$$
H_A(M) \longrightarrow H_{\widehat{A}}(\widehat{A} \otimes_A M)
$$

Nếu $A$-môđun $M$ là kiểu hữu hạn, thì $A$-môđun $\widehat{A} \otimes_A M$ được đồng nhất với hoàn thành $\widehat{M}$ của $M$ (III, § 3, No. 4, th. 3), và ta có một đẳng cấu $H_A(M) \to H_{\widehat{A}}(\widehat{M})$, phân bậc bậc 0.

### 2. Đối đồng điều địa phương trên một vành Macaulay

Trong số này, giả sử rằng $A$ là một vành Macaulay địa phương; ta đặt $\dim(A) = d$.

Các iđêan sinh bởi một dãy phần tử của $m_A$ hoàn toàn cát tuyến đối với $A$ và có độ dài $d = \dim(A)$ tạo thành một tập con đồng cuối $\mathscr{D}_{cs}$ trong tập $\mathscr{D}$ các iđêan định nghĩa của $A$. Thật vậy, cho $(x_1, \ldots, x_d)$ là một dãy phần tử của $m_A$ hoàn toàn cát tuyến đối với $A$ (§ 2, Mệnh đề 3); với mọi số nguyên $n$, dãy $(x_1^n, \ldots, x_d^n)$ là hoàn toàn cát tuyến đối với $A$ (A, X, p. 158, Mệnh đề 6, c)), và sinh ra một iđêan định nghĩa (VIII, § 3, Hệ quả của Mệnh đề 3 và Định lý 1) được chứa trong $m_A^n$.

Cho $\alpha \in \mathscr{D}_{cs}$, và cho $\pi : L \to A/\alpha$ là một giải tự do hữu hạn, bằng không ở bậc $> d$ (chẳng hạn phức Koszul liên kết với một dãy hoàn toàn cát tuyến đối với $A$ sinh ra $\alpha$). Xét đối ngẫu $L^* = \mathrm{Homgr}_A(L, A)$ của $L$; vì độ sâu của $A$ bằng $d$, ta có $\mathrm{Ext}_A^i(A/\alpha, A) = 0$ với $i < d$ (§ 1, Hệ quả 2 của Mệnh đề 2). Vì $L^*$ có độ dài $\leq d$, suy ra $H^i(L^*)$ bằng không với $i \neq d$ và $H^d(L^*)$ được đồng nhất với $\mathrm{Ext}_A^d(A/\alpha, A)$ (A, X, p. 100, Định lý 1). Do đó có một đồng cấu

$$
\pi^* : L^*(-d) \longrightarrow \mathrm{Ext}_A^d(A/\alpha, A)
$$

xác định một giải tự do hữu hạn của $\mathrm{Ext}_A^d(A/\alpha, A)$.

Cho $M$ là một $A$-môđun; xét các đẳng cấu chính tắc (*loc. cit.*)

$$
\varphi(L, M) : H(\mathrm{Homgr}_A(L, M)) \to \mathrm{Ext}_A(A/\alpha, M)
$$
$$
\psi(M, L^*(-d)) : \mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/\alpha, A)) \to H(M \otimes_A L^*)(-d)
$$

Vì phức L là tự do hữu hạn, cấu xạ chính tắc của các phức $M \otimes_A L^* \to \mathrm{Homgr}_A(L, M)$ là một đẳng cấu; suy ra có một đẳng cấu của các A-môđun phân bậc $H(M \otimes_A L^*) \to H(\mathrm{Homgr}_A(L, M))$. Bằng hợp thành của các đẳng cấu đi trước, ta thu được một đẳng cấu của các A-môđun phân bậc, gọi là *chính tắc*,

$$
\tau(L, M) : \mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/\alpha, A))(d) \longrightarrow \mathrm{Ext}_A(A/\alpha, M)
$$

đẳng cấu này cảm sinh, với mỗi số nguyên $i$, một đẳng cấu

$$
\tau^i(L, M) : \mathrm{Tor}_{d-i}^A(M, \mathrm{Ext}_A^d(A/\alpha, A)) \longrightarrow \mathrm{Ext}_A^i(A/\alpha, M)
$$

Với $M = A$, $\tau^d(L, A)$ là đẳng cấu chính tắc của $A \otimes_A \mathrm{Ext}_A^d(A/\alpha, A)$ lên $\mathrm{Ext}_A^d(A/\alpha, A)$.

Cho $b$ là một iđêan của $\mathcal{D}_{cs}$ được chứa trong $\alpha$. Cho $\rho : R \to A/b$ là một giải tự do hữu hạn có độ dài $\leq d$ và cho $p_{ab} : A/b \to A/\alpha$ là toàn cấu chính tắc. Theo A, X, p. 49, Mệnh đề 3, tồn tại một cấu xạ của các phức $P_{LR} : R \to L$ sao cho $\pi \circ P_{LR} = p_{ab} \circ \rho$. Theo Mệnh đề 2 của A, X, p. 103, ta có một biểu đồ giao hoán

$$
\begin{array}{ccc}
\mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/\alpha, A))(d) & \xrightarrow{\mathrm{Tor}(1_M, \mathrm{Ext}^d(p_{ab}, 1_A))} & \mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/b, A))(d) \\
\downarrow \psi(L^*(-d), M) & & \downarrow \psi(R^*(-d), M) \\
H(M \otimes_A L^*) & \xrightarrow{H(1_M \otimes^t P_{LR})} & H(M \otimes_A R^*) \\
\downarrow & & \downarrow \\
H(\mathrm{Homgr}_A(L, M)) & \xrightarrow{H(\mathrm{Homgr}(P_{LR}, M))} & H(\mathrm{Homgr}_A(R, M)) \\
\downarrow \varphi(L, M) & & \downarrow \varphi(R, M) \\
\mathrm{Ext}_A(A/\alpha, M) & \xrightarrow{\mathrm{Ext}(p_{ab}, 1_M)} & \mathrm{Ext}_A(A/b, M)
\end{array}
$$

Trước hết suy ra, bằng cách lấy $\alpha = b$, rằng đẳng cấu $\tau(L, M)$ không phụ thuộc vào lựa chọn phân giải L của $A/\alpha$; ta sẽ ký hiệu nó bởi $\tau_\alpha(M)$. Khi đó suy ra rằng các $\tau_\alpha(M)$ với $\alpha \in \mathcal{D}_{cs}$ tạo thành một hệ quy nạp các đẳng cấu. Chuyển qua giới hạn quy nạp, và có tính đến A, X, p. 70, mệnh đề 8, ta thu được với mỗi số nguyên $i$ một *đẳng cấu của các a-môđun*

$$
\tau^i(M) : \mathrm{Tor}_{d-i}^A(M, H_A^d(A)) \longrightarrow H_A^i(M)
$$

Với $M = A$, $\tau^d(A)$ là đẳng cấu chính tắc từ $A \otimes_A H_A^d(A)$ lên $H_A^d(A)$.

#### Nhận xét 1 {#ac-x-s10-n2-rem-1 .statement}

Cho $f : M \to N$ là một đồng cấu của các a-môđun. Dùng A, X, p. 103, mệnh đề 2, ta chứng minh được rằng các biểu đồ sau là giao hoán:

$$
\begin{array}{ccc}
\mathrm{Tor}_{d-i}^A(M, H_A^d(A)) & \xrightarrow{\tau^i(M)} & H_A^i(M) \\
\downarrow \mathrm{Tor}_{d-i}(f,1) & & \downarrow H^i(f) \\
\mathrm{Tor}_{d-i}^A(N, H_A^d(A)) & \xrightarrow{\tau^i(N)} & H_A^i(N)
\end{array}
$$

#### Nhận xét 2 {#ac-x-s10-n2-rem-2 .statement}

Cho
$$
(\mathcal{E}) \quad 0 \to M \to N \to P \to 0
$$
là một dãy khớp của các a-môđun. Dùng A, X, p. 104, mệnh đề 3 và p. 106, mệnh đề 4, ta chứng minh được rằng các biểu đồ sau là giao hoán:

$$
\begin{array}{ccc}
\mathrm{Tor}_{d-i}^A(P, H_A^d(A)) & \xrightarrow{\tau^i(P)} & H_A^i(P) \\
\downarrow \partial_{d-i}(\mathcal{E}, H_A^d(A)) & & \downarrow \partial^i(\mathcal{E}) \\
\mathrm{Tor}_{d-i-1}^A(M, H_A^d(A)) & \xrightarrow{\tau^{i+1}(M)} & H_A^{i+1}(M)
\end{array}
$$

#### Nhận xét 3 {#ac-x-s10-n2-rem-3 .statement}

Xét đẳng cấu
$$
\tau^d(M) : M \otimes_A H_A^d(A) \longrightarrow H_A^d(M)
$$
Với $x \in M$, ta ký hiệu bởi $f_x$ ánh xạ $a \mapsto ax$ từ A vào M. Với mọi $u \in H_A^d(A)$, ta có
$$
\tau^d(M)(x \otimes u) = H_A^d(f_x)(u)
$$
Điều này thực ra suy ra từ nhận xét 1 áp dụng cho đồng cấu $f_x : A \to M$.

### 3. Đối ngẫu Grothendieck trên một vành Macaulay

Ta vẫn giả sử rằng A là một vành Macaulay địa phương, có chiều d. Cho $\Omega$ là một A-môđun đối ngẫu hóa. A-môđun $H_A^d(\Omega)$ là một môđun Matlis (§ 8, No. 5, ví dụ 6); phù hợp với ký hiệu của § 8, ta sẽ đặt $D(M) = \mathrm{Hom}_A(M, H_A^d(\Omega))$ với mọi A-môđun M.

Xét đẳng cấu $\tau^d(\Omega) : \Omega \otimes H_A^d(A) \to H_A^d(\Omega)$ (No. 2). Từ đó suy ra một đồng cấu $\omega : H_A^d(A) \to \mathrm{Hom}_A(\Omega, H_A^d(\Omega))$ gán cho một phần tử $u$ của $H_A^d(A)$ đồng cấu $x \mapsto H_A^d(f_x)(u)$ (nhận xét 3 ở trên).

#### Mệnh đề 2 {#ac-x-s10-prop-2 .statement}

*Cho A là một vành Macaulay địa phương, có chiều d*, và cho $\Omega$ *là một A-môđun đối ngẫu hóa*. *Đồng cấu* $\omega : H_A^d(A) \to D(\Omega)$ *là song ánh*.

Đồng cấu $\omega$ là giới hạn của hệ quy nạp các ánh xạ $(\omega_\alpha)_{\alpha \in \mathscr{D}_{cs}}$, trong đó
$$
\omega_\alpha : \mathrm{Ext}_A^d(A/\alpha, A) \longrightarrow \mathrm{Hom}_A(\Omega, \mathrm{Ext}_A^d(A/\alpha, \Omega))
$$

gán cho một phần tử $u$ của $\mathrm{Ext}_A^d(A/\alpha, A)$ ánh xạ $x \mapsto f_x \circ u$ (A, X, p. 114). Do đó chỉ cần chứng minh rằng mỗi ánh xạ $\omega_\alpha$ là song ánh.

Cho $\alpha$ là một iđêan của $\mathscr{D}_{cs}$, sinh bởi một dãy hoàn toàn cắt $x = (x_1, \ldots, x_d)$ của $A$. Phức Koszul $K^\bullet(x, A)$ cung cấp một phân giải xạ ảnh của $A/\alpha$; với mọi $A$-môđun $M$, A-môđun $H^d(\mathrm{Homgr}_A(K^\bullet(x, A), M))$ được đồng nhất một cách chính tắc với $M/\alpha M$ (A, X, p. 155). Từ đó suy ra một đẳng cấu (A, X, p. 100)
$$
\varphi_M : M/\alpha M \longrightarrow \mathrm{Ext}_A^d(A/\alpha, M) .
$$
Cho $x \in \Omega$. Có tính đến loc. cit., p. 103, mệnh đề 2, ta có một biểu đồ giao hoán

$$
\begin{array}{ccc}
A/\alpha & \xrightarrow{\varphi_A} & \mathrm{Ext}_A^d(A/\alpha, A) \\
\downarrow f_x & & \downarrow \mathrm{Ext}(1_{A/\alpha}, f_x) \\
\Omega/\alpha \Omega & \xrightarrow{\varphi_\Omega} & \mathrm{Ext}_A^d(A/\alpha, \Omega)
\end{array}
$$

trong đó $f_x$ là đồng cấu suy ra từ $f_x$ bằng cách chuyển qua các thương. Suy ra rằng nếu với mọi $A$-môđun $M$ ta đồng nhất $\mathrm{Ext}_A^d(A/\alpha, M)$ với $M/\alpha M$ nhờ $\varphi_M$, thì đồng cấu $\omega_\alpha$ được đồng nhất với ánh xạ $A$-tuyến tính từ $A/\alpha$ vào $\mathrm{Hom}_A(\Omega, \Omega/\alpha \Omega)$ gửi 1 tới toàn cấu chính tắc, tức lại chính là ánh xạ chính tắc $A/\alpha \longrightarrow \mathrm{End}_{A/\alpha}(\Omega/\alpha \Omega)$. Nhưng vì $A/\alpha$-môđun $\Omega/\alpha \Omega$ là đối ngẫu hóa (§ 9, No. 2, mệnh đề 4), ánh xạ này là song ánh (§ 9, No. 4, mệnh đề 6), điều đó chứng minh mệnh đề.

Hãy đồng nhất song đối ngẫu Matlis $D(D(\Omega))$ với $\widehat{\Omega}$ bởi đẳng cấu $\widehat{\alpha}_\Omega$ (§ 8, No. 3, định lý 2, b)).

#### Hệ quả {#ac-x-s10-n3-cor-1 .statement}

*Đồng cấu* $D(\omega) : \widehat{\Omega} \to D(H^d_A(A))$ *là một đẳng cấu*.

Cho $M$ là một $A$-môđun, và $i$ là một số nguyên. Xét các đồng cấu chính tắc (§ 8, No. 7)

$$
\rho_{d-i}(M, \Omega) : \mathrm{Tor}^A_{d-i}(M, D(\Omega)) \longrightarrow D(\mathrm{Ext}_A^{d-i}(M, \Omega))
$$
$$
\theta^{d-i}(M, H^d_A(A)) : \mathrm{Ext}_A^{d-i}(M, D(H^d_A(A))) \longrightarrow D(\mathrm{Tor}^A_{d-i}(M, H^d_A(A))) .
$$

Nhờ các đẳng cấu $\omega : H^d_A(A) \to D(\Omega)$, $D(\omega) : \widehat{\Omega} \to D(H^d_A(A))$ (hệ quả 1 của mệnh đề 2) và $\tau^i(M) : \mathrm{Tor}^A_{d-i}(M, H^d_A(A)) \to H^i_A(M)$ (No. 2), từ đó ta suy ra các *đồng cấu chính tắc của các $A$-môđun*

$$
\gamma^i(M) : H^i_A(M) \longrightarrow D(\mathrm{Ext}_A^{d-i}(M, \Omega))
$$
$$
\delta^i(M) : \mathrm{Ext}_A^{d-i}(M, \widehat{\Omega}) \longrightarrow D(H^i_A(M)) .
$$

#### Định lý 1 (Grothendieck Duality) {#ac-x-s10-thm-1 .statement}

Cho $A$ là một vành Macaulay địa phương, có chiều $d$, và $\Omega$ là một $A$-môđun đối ngẫu hóa.

a) $A$-môđun $H_A^d(\Omega)$ là một môđun Matlis; với mọi $A$-môđun $P$, ký hiệu $D(P)$ là đối ngẫu Matlis $\mathrm{Hom}_A(P, H_A^d(\Omega))$.

b) Với mọi $A$-môđun sinh hữu hạn $M$ và mọi số nguyên $i$, đồng cấu chính tắc
$$
\gamma^i(M) : H_A^i(M) \longrightarrow D(\mathrm{Ext}_A^{d-i}(M, \Omega))
$$
là một đẳng cấu của các $A$-môđun Artin.

c) Với mọi $A$-môđun $M$ và mọi số nguyên $i$, đồng cấu chính tắc
$$
\delta^i(M) : \mathrm{Ext}_A^{d-i}(M, \widehat{\Omega}) \longrightarrow D(H_A^i(M))
$$
là một đẳng cấu của các $\widehat{A}$-môđun.

Điều này suy ra từ mệnh đề 6 của § 8, No. 7.

#### Hệ quả {#ac-x-s10-n3-cor-2 .statement}

Cho $A$ là một vành Macaulay địa phương, và $M$ là một $A$-môđun sinh hữu hạn khác không, có chiều $e$. $A$-môđun $H_A^e(M)$ khác không.

Theo Nhận xét 2 của No. 1, có thể giả sử rằng vành địa phương $A$ là đầy đủ. Trong trường hợp này $A$ có một môđun đối ngẫu hóa $\Omega$ ($§ 9$, No. 3, Hệ quả 3 của Mệnh đề 6); nếu $H_A^e(M)$ bằng không thì điều tương tự cũng đúng với đối ngẫu Matlis của nó $\mathrm{Ext}_A^{d-e}(M, \Omega)$, điều này mâu thuẫn với Mệnh đề 3, b) của $§ 9$, No. 1.

#### Nhận xét 1 {#ac-x-s10-n3-rem-1 .statement}

Khi A-môđun $M$ là sinh hữu hạn, $\widehat{A}$-môđun $\mathrm{Ext}_A^{d-i}(M, \widehat{\Omega})$ được đồng nhất với $\widehat{A} \otimes_A \mathrm{Ext}_A^{d-i}(M, \Omega)$ ($A$, X, p. 108, Mệnh đề 7, c)), và $\delta^i(M)$ cũng có thể thu được bằng cách hợp thành $D(\gamma^i(M))$ với đẳng cấu song đối ngẫu.

#### Nhận xét 2 {#ac-x-s10-n3-rem-2 .statement}

Cho $u : M \to M'$ là một đồng cấu của các A-môđun. Theo Nhận xét 1 của No. 2 và Nhận xét của $§ 8$, No. 7, các biểu đồ sau là giao hoán:

$$
\begin{array}{ccc}
H_A^i(M) & \xrightarrow{\gamma^i(M)} & D(\mathrm{Ext}_A^{d-i}(M, \Omega)) \\
\downarrow H_A^i(u) & & \downarrow D(\mathrm{Ext}(u,1)) \\
H_A^i(M') & \xrightarrow{\gamma^i(M')} & D(\mathrm{Ext}_A^{d-i}(M', \Omega))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{d-i}(M', \widehat{\Omega}) & \xrightarrow{\delta^i(M')} & D(H_A^i(M')) \\
\downarrow \mathrm{Ext}(u,1) & & \downarrow D(H_A^i(u)) \\
\mathrm{Ext}_A^{d-i}(M, \widehat{\Omega}) & \xrightarrow{\delta^i(M)} & D(H_A^i(M))
\end{array}
$$

#### Nhận xét 3 {#ac-x-s10-n3-rem-3 .statement}

Cho

$$(\mathcal{E})$$
$$0 \to M' \to M \to M'' \to 0$$

là một dãy khớp của các A-môđun. Theo Nhận xét 2 của No. 2 và Nhận xét của § 8, No. 7, các biểu đồ sau là giao hoán:

$$
\begin{array}{ccc}
H_A^{i-1}(M'') & \xrightarrow{\gamma^{i-1}(M'')} & D(\mathrm{Ext}_A^{d-i+1}(M'', \Omega)) \\
\downarrow & & \downarrow (-1)^{d-i+1}D(\delta^d i(\mathcal{E}, \Omega)) \\
H_A^i(M') & \xrightarrow{\gamma^i(M')} & D(\mathrm{Ext}_A^{d-i}(M', \Omega))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{d-i}(M', \widehat{\Omega}) & \xrightarrow{\delta^i(M')} & D(H_A^i(M')) \\
\downarrow & & \downarrow (-1)^{d-i+1}D(\partial^{i-1}(\mathcal{E})) \\
\mathrm{Ext}_A^{d-i+1}(M'', \widehat{\Omega}) & \xrightarrow{\delta^{i-1}(M'')} & D(H_A^{i-1}(M''))
\end{array}
$$

#### Ví dụ {#ac-x-s10-n3-exa-1 .statement}

Cho $A$ là một vành địa phương Noether nguyên có chiều 1; gọi $K$ là trường phân thức của nó. Cho $\Omega$ là một A-môđun đối ngẫu hóa, và cho $M$ là một A-môđun sinh hữu hạn. Các A-môđun $H_A^0(M)$ và $H_A^1(M)$ được đồng nhất một cách chính tắc với $T(M)$ và $(K/A) \otimes_A M$ (No. 1, Ví dụ 5). Với các sự đồng nhất này, các đẳng cấu đối ngẫu

$$\gamma^0(M) : T(M) \longrightarrow D(\mathrm{Ext}_A^1(M, \Omega)) \quad , \quad \gamma^1(M) : (K/A) \otimes_A M \longrightarrow D(\mathrm{Hom}_A(M, \Omega))$$

(Định lý 1) không là gì khác ngoài các đẳng cấu được xác định trong § 9, No. 6.

Bài tập

## BÀI TẬP {#ac-x-s10-exercises}

Xem [các bài tập của § 10](exercises/s10/).
