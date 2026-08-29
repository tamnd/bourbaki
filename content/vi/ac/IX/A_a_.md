---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 0
section_title: ""
appendix: true
lang: vi
source: ac-viii-ix-fr
book_pages: AC IX.37-AC IX.42
pdf_pages: 0149-0154, 0196-0204
extraction: ocr
subsections:
    - "no": 1
      title: Limite inductive d’anneaux locaux
      page: 37
      pdf_page: 149
    - "no": 2
      title: Gonflement d’un anneau local
      page: 37
      pdf_page: 149
    - "no": 3
      title: Existence des $p$-anneaux
      page: 41
      pdf_page: 153
statements: 13
exercises: 6
content_sha256: 8d6da072ed6fcc319bccdad6120c6a1c8e97fbdc85483c20e03b29245316760d
translated_from: content/en-mt/ac/IX/A_a_.md
source_lang: en-mt
translation_method: machine
source_content_sha256: d57d3f281d99f0203bdf9e3c89e5b2992faec2ed6c8e9170c4846aa661bb34c4
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-vi-bb837d2a
glossary_version: 34
glossary_terms_sha256: 96e1a1c7c2da48f6ae67d634dfcb37ae2fcf1784ae37b4d2156eadbb971e2367
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

### PHỤ LỤC

### 1. Giới hạn quy nạp của các vành địa phương

Cho I là một tập hợp tiền thứ tự lọc phải khác rỗng và cho $(A_\alpha, \varphi_{\beta\alpha})$ là một hệ quy nạp của các vành đối với I. Giả sử rằng, với mọi $\alpha \in I$, vành $A_\alpha$ là địa phương, với iđêan cực đại $m_\alpha$, rằng các đồng cấu $\varphi_{\beta\alpha}$ là địa phương và phẳng, và rằng ta có $\varphi_{\beta\alpha}(m_\alpha)$ $A_\beta = m_\beta$ với $\beta \geq \alpha$. Ký hiệu A là giới hạn quy nạp của các $A_\alpha$, và với mọi $\alpha \in I$, ký hiệu $\varphi_\alpha : A_\alpha \to A$ là đồng cấu chính tắc.

#### Mệnh đề 1 {#ac-ix-a0-prop-1 .statement}

a) Vành A là địa phương, với iđêan cực đại $m = \lim \overrightarrow{m_\alpha}$. Với mọi $\alpha \in I$, đồng cấu $\varphi_\alpha$ là địa phương và phẳng, và ta có $\varphi_\alpha(m_\alpha)$ $A = m$.

b) Nếu $A_\alpha$ là Noether với mọi $\alpha \in A$, thì A là Noether.

a) Đặt $m = \lim \overrightarrow{m_\alpha}$; đây là một iđêan của A. Vành thương $A/m$ là giới hạn quy nạp của các trường $A_\alpha/m_\alpha$, do đó là một trường (A, I, p. 116, Mệnh đề 3). Mặt khác, mọi phần tử của $A - m$ đều khả nghịch trong A: thật vậy, cho $x \in A - m$; tồn tại $\alpha \in I$ và $\xi \in A_\alpha$ sao cho $x = \varphi_\alpha(\xi)$; ta có $\xi \notin m_\alpha$, do đó $\xi$ khả nghịch trong $A_\alpha$ và x khả nghịch trong A. Do đó, A là một vành địa phương, với iđêan cực đại m. Cho $\alpha \in I$. Từ các hệ thức $\varphi_{\beta\alpha}(m_\alpha)$ $A_\beta = m_\beta$ với $\beta \geq \alpha$, suy ra, bằng cách chuyển qua giới hạn quy nạp, $\varphi_\alpha(m_\alpha)$ $A = m$; cuối cùng, đồng cấu $\varphi_\alpha$ là phẳng theo I, § 2, No. 7, Mệnh đề 9.

(b) Cho $\hat{A}$ là hoàn thành tách được của A đối với tôpô $m$-adic và $\pi$ là ánh xạ chính tắc của A vào $\hat{A}$. Giả sử rằng các vành $A_\alpha$ là Noether. Cố định $\alpha \in I$ và chứng minh rằng vành $\hat{A}$ là Noether và phẳng trên $A_\alpha$. Theo giả thiết, $m_\alpha$ là một iđêan sinh hữu hạn của $A_\alpha$, do đó $m = \varphi_\alpha(m_\alpha)$. A là một iđêan sinh hữu hạn của A. Suy ra iđêan cực đại $\hat{m}$ của $\hat{A}$ bằng $mA$ (III, § 2, No. 12, Hệ quả 2 của Mệnh đề 16 và No. 13, Mệnh đề 19), do đó nó là sinh hữu hạn. Do đó, vành $\hat{A}$ là Noether (loc. cit., No. 10, Hệ quả 5 của Định lý 2). Mặt khác, với mọi $n \in \mathbf{N}$, thương $\hat{A}/\hat{m}^n$ đẳng cấu với $A/m^n$ (loc. cit., No. 12, Hệ quả 2 của Mệnh đề 16 và công thức (21)), điều đó có nghĩa là $\hat{A}/\pi \circ \varphi_\alpha(m_\alpha^n)$ $\hat{A}$ đẳng cấu với $A \otimes_A (A_\alpha/m_\alpha^n)$; vì A là một $A_\alpha$-môđun phẳng, môđun $(A_\alpha/m_\alpha^n)$-$\hat{A}/\pi \circ \varphi_\alpha(m_\alpha^n)$ $\hat{A}$ là phẳng với mọi $n \in \mathbf{N}$. Theo III, § 5, No. 4, Mệnh đề 2, $A_\alpha$-môđun $\hat{A}$ là tách được lý tưởng đối với $m_\alpha$; theo loc. cit., No. 2, Định lý 1, $A_\alpha$-môđun $\hat{A}$ do đó là phẳng. Suy ra bằng cách chuyển qua giới hạn quy nạp rằng $\hat{A}$ là phẳng (trung thành) trên A (I, § 2, No. 7, Mệnh đề 9), do đó A là Noether (I, § 3, No. 5, hệ quả của Mệnh đề 8).

### 2. Phồng của một vành địa phương

Cho A là một vành địa phương.

Ta ký hiệu bởi A]X[ vành địa phương của vành đa thức A[X] tại iđêan nguyên tố $m_A A[X]$. Nó là một vành địa phương với iđêan cực đại $m_A A[X]$, đồng cấu chính tắc $A \to A[X]$ là địa phương và phẳng, và trường thặng dư của $A[X]$ là mở rộng thuần của $\kappa_A$ sinh bởi lớp của $X$.

#### Bổ đề 1 {#ac-ix-a0-lem-1 .statement}

Cho $P \in A[X]$ là một đa thức đơn khởi mà ảnh $\overline{P}$ của nó trong $\kappa_A[X]$ là bất khả quy. Khi đó đại số $A$-đại số $B = A[X]/(P)$ là địa phương và hữu hạn trên A, với iđêan cực đại $m_A B$, đồng cấu chính tắc $\rho : A \to B$ là địa phương và phẳng, mở rộng thặng dư $\kappa_A \to \kappa_B$ là đại số và được sinh bởi lớp $x$ của $X$, và đa thức tối tiểu của $x$ trên $\kappa_A$ là $\overline{P}$.

Vì đa thức $P$ là đơn khởi, $A$-môđun $B$ là tự do kiểu hữu hạn (A, IV, p. 10). Vành $B/m_A B$ được đồng nhất với $\kappa_A[X]/(\overline{P})$, và do đó là một trường; suy ra iđêan $m_A B$ là cực đại. Cho $q$ là một iđêan cực đại của $B$; khi đó iđêan $\rho^{-1}(q)$ là cực đại (V, § 2, no 1, mệnh đề 1); do đó ta có $\rho^{-1}(q) = m_A$, do đó $q \supset m_A B$ và cuối cùng $q = m_A B$. Vậy vành $B$ là địa phương. Bổ đề 1 suy ra ngay.

#### Định nghĩa 1 {#ac-ix-a0-def-1 .statement}

Cho $A$ là một vành địa phương. Một $A$-đại số $B$ được gọi là một mở rộng sơ cấp của $A$ nếu $B$ đẳng cấu với $A$-đại số $A[X]$, hoặc nếu tồn tại một đa thức đơn khởi $P$ trong $A[X]$, có ảnh trong $\kappa_A[X]$ là bất khả quy, sao cho $B$ đẳng cấu với $A$-đại số $A[X]/(P)$.

Cho $B$ là một mở rộng sơ cấp của $A$. Từ những điều trên suy ra các tính chất sau:

a) Vành $B$ là địa phương và đồng cấu chính tắc từ $A$ vào $B$ là địa phương và phẳng, đặc biệt là đơn ánh (I, § 3, no 5, mệnh đề 8).

b) Trường thặng dư $\kappa_B$ của $B$ là một mở rộng đơn sinh của trường thặng dư $\kappa_A$ của $A$. Nếu $\kappa_A$ có bậc hữu hạn $d$ trên $\kappa_A$, thì $B$ là một $A$-môđun tự do có hạng $d$.

c) Ta có $m_B = m_A B$. Đặc biệt, nếu $A$ là một trường, điều tương tự cũng đúng với $B$. Một mở rộng của các trường là một mở rộng sơ cấp khi và chỉ khi nó là đơn sinh.

d) Nếu $A$ là Noether, thì điều tương tự cũng đúng với $B$.

#### Định nghĩa 2 {#ac-ix-a0-def-2 .statement}

Cho $A$ là một vành địa phương. Một $A$-đại số $B$ được gọi là một mở rộng của $A$ nếu tồn tại một tập được sắp tốt $\Lambda$ có một phần tử lớn nhất $\omega$, và một họ tăng $(B_\lambda)_{\lambda \in \Lambda}$ các đại số con của $B$ thỏa mãn các điều kiện sau:

a) Ta có $B_\omega = B$ và vành $B_\lambda$ là địa phương với mọi $\lambda \in \Lambda$.

b) Nếu $\alpha$ là phần tử nhỏ nhất của $\Lambda$, $A$-đại số $B_\alpha$ là đẳng cấu với $A$.

c) Cho $\nu \neq \alpha$ trong $\Lambda$ và cho $S_\nu$ là tập hợp các $\lambda \in \Lambda$ sao cho $\lambda < \nu$. Nếu $S_\nu$ không có phần tử lớn nhất, ta có $B_\nu = \bigcup_{\lambda \in S_\nu} B_\lambda$; nếu $S_\nu$ có một phần tử lớn nhất $\mu$, thì $B_\nu$ là một phép phình sơ cấp của $B_\mu$.

Cho $B$ là một vành và $\rho : A \to B$ là một đồng cấu vành. Ta nói rằng $\rho$ là một phép phình (tương ứng một phép phình sơ cấp) nếu $A$-đại số xác định bởi $\rho$ có tính chất này. Khi đó, $\rho$ là đơn ánh.

#### Ví dụ 1 {#ac-ix-a0-n2-exa-1 .statement}

Mọi mở rộng trường đều là một phép phình. Thật vậy, cho K là một mở rộng của một trường k. Ta trang bị cho K một cách sắp thứ tự tốt mà 0 là phần tử lớn nhất, và với $\lambda \in K$, cho $K_\lambda$ là mở rộng con-$k$ của K sinh bởi các phần tử $\beta$ của K sao cho $\beta < \lambda$. Việc kiểm tra các điều kiện a), b), c), đối với $k, K$ và họ $(K_\lambda)_{\lambda \in K}$, là ngay lập tức.

#### Ví dụ 2 {#ac-ix-a0-n2-exa-2 .statement}

Cho A là một vành địa phương, và I là một tập hợp các chỉ số. Ký hiệu bởi $A[(X_i)_{i \in I}]$ vành địa phương của vành đa thức $A[(X_i)_{i \in I}]$ tại iđêan nguyên tố $m_A A[(X_i)_{i \in I}]$. $A[(X_i)_{i \in I}]$-đại số là một phép phình của A. Thật vậy, trang bị cho tập hợp I một cách sắp thứ tự tốt; cho $\Lambda$ là tập được sắp thứ tự tốt thu được bằng cách thêm vào I một phần tử lớn nhất $\omega$. Với $i \in I$, đồng nhất $A[(X_j)_{j < i}]$ với một đại số con $B_i$ của $B = A[(X_i)_{i \in I}]$, và đặt $B_\omega = B$. Họ $(B_\lambda)_{\lambda \in \Lambda}$ thỏa mãn các điều kiện a), b), c).

#### Nhận xét {#ac-ix-a0-n2-rem-1 .statement}

Với ký hiệu của Định nghĩa 2, vành $B_\mu$ là một phép phình của $B_\lambda$ khi $\lambda \leq \mu$.

#### Mệnh đề 2 {#ac-ix-a0-prop-2 .statement}

Cho A là một vành địa phương và B là một phép phình của A.

a) Vành B là địa phương và có $m_A B = m_B$.

b) $A$-đại số B là phẳng trung thành.

c) Đồng cấu chính tắc

$$
\gamma_B : \operatorname{gr}(A) \otimes_{\kappa_A} \kappa_B \to \operatorname{gr}(B)
$$

là song ánh.

d) Nếu A là Noether, điều tương tự cũng đúng đối với B và các chuỗi Hilbert-Samuel (VIII, § 4, No. 3) của A và B là bằng nhau.

Cho $(B_\lambda)_{\lambda \in \Lambda}$ là một họ các đại số con của B thỏa mãn các điều kiện a), b) và c) của Định nghĩa 2.

Cho $\Lambda'$ là tập hợp các chỉ số $\lambda \in \Lambda$ sao cho, với mọi $\mu \leq \lambda$ trong $\Lambda$, đại số trên A $B_\mu$ là địa phương và phẳng trung thành, và sao cho có $m_{B_\mu} = m_A B_\mu$. Giả sử rằng $\Lambda' \neq \Lambda$ và cho $v$ là phần tử nhỏ nhất của $\Lambda - \Lambda'$. Ta có $\alpha \in \Lambda'$, do đó $v \neq \alpha$. Khi đó $S_v$ được chứa trong $\Lambda'$. Nếu $S_v$ không có phần tử lớn nhất, ta có $B_v = \bigcup_{\lambda \in S_v} B_\lambda$ và $v$ thuộc $\Lambda'$ theo Mệnh đề 1 của No. 1. Nếu $S_v$ có một phần tử lớn nhất $\mu$, ta có $\mu \in \Lambda'$ và $B_v$ là một phép thổi phồng sơ cấp của $B_\mu$: lại có $v \in \Lambda'$ theo các nhận xét sau Định nghĩa 1, do đó dẫn đến một mâu thuẫn.

Khi A là Noether, ta chứng minh tương tự rằng tập hợp $\Lambda''$ của các chỉ số $\lambda \in \Lambda$ sao cho vành $B_\lambda$ là Noether bằng $\Lambda$.

Do đó ta có $\omega \in \Lambda'$, do đó có các mệnh đề a) và b). Khi A là Noether, ta có $\omega \in \Lambda''$, suy ra $B = B_\omega$ là Noether.

Mệnh đề c) suy ra từ a), b), và Định lý 1 của III, § 5, No. 2. Giả sử rằng A (do đó B) là Noether; vì ta có

$$
[m_B^n / m_B^{n+1} : \kappa_B] = [m_A^n / m_A^{n+1} : \kappa_A]
$$

với mọi $n \in \mathbf{N}$, các chuỗi Hilbert-Samuel của A và B bằng nhau.

#### Hệ quả {#ac-ix-a0-n2-cor-1 .statement}

Giả sử rằng A là Noether.
a) Ta có dim(A) = dim(B).
b) Giả sử rằng A là chính quy, và cho $(x_1, ..., x_n)$ là một hệ tọa độ của A. Khi đó B là chính quy và dãy $(x_1 1_B, ..., x_n 1_B)$ là một hệ tọa độ của B.
Điều này suy ra từ Mệnh đề 1 của VIII, § 5, No. 1.

#### Mệnh đề 3 {#ac-ix-a0-prop-3 .statement}

Cho A, B, C là ba vành địa phương và $u : A \to B, v : B \to C$ là hai phép thổi phồng. Khi đó $v \circ u$ là một phép thổi phồng.
Cho $(B_\lambda)_{\lambda \in \Lambda}$ và $(C_\mu)_{\mu \in M}$ là các họ các đại số con trên A của B và các đại số con trên B của C tương ứng, có các tính chất a), b), c) của Định nghĩa 2. Trên tập hợp N là tổng của $\Lambda$ và M, xét quan hệ thứ tự cảm sinh trên $\Lambda$ và M các cấp đã cho và sao cho có $\lambda < \mu$ với $\lambda \in \Lambda, \mu \in M$. Đây là một quan hệ thứ tự tốt. Với $\lambda \in \Lambda \subset N$, đặt $C_\lambda = v(B_\lambda)$. Khi đó họ $(C_v)_{v \in N}$ thỏa mãn các điều kiện a), b), c) của Định nghĩa 1 đối với đại số trên A C.

#### Định lý 1 {#ac-ix-a0-thm-1 .statement}

Cho $f : A \to A'$ là một đồng cấu địa phương toàn ánh của các vành địa phương và cho $B'$ là một phép phình của $A'$. Tồn tại một phép phình B của A và một đẳng cấu các đại số trên A của $B \otimes_A A'$ lên $B'$.
A) Giả sử rằng $B'$ là một phép phình sơ cấp của $A'$. Ta phân biệt hai trường hợp:
1) Nếu $B'$ hữu hạn trên $A'$, chọn một đẳng cấu của $A'$-đại số $\varphi : A'[X]/(P') \to B'$, trong đó $P' \in A'[X]$ là một đa thức đơn khởi mà ảnh của nó là bất khả quy trong $\kappa_{A'}[X]$. Chọn một đa thức đơn khởi $P \in A[X]$ có ảnh trong $A'[X]$ là $P'$. Nó tất yếu là bất khả quy modulo iđêan cực đại của A. Đặt khi đó $B = A[X]/(P)$. Đại số trên A B là một phép phình sơ cấp của A và $\varphi$ cảm sinh một đẳng cấu các đại số trên A của $B \otimes_A A'$ lên $B'$.
2) Nếu $B'$ không hữu hạn trên $A'$, chọn một đẳng cấu của $A'$-đại số $\psi : A'[X] \to B'$. Đặt $B = A[X][$. Đại số trên A B là một phép phình sơ cấp của A, và $B \otimes_A A'$ là đẳng cấu chính tắc với $A'[X][$. Do đó $\psi$ cảm sinh một đẳng cấu các đại số trên A của $B \otimes_A A'$ lên $B'$.
B) Ta chuyển sang trường hợp tổng quát. Cho $(B'_\lambda)_{\lambda \in \Lambda}$ là một họ các đại số con-$A'$ của $B'$ có đối với $A'$ và $B'$ các tính chất a), b), c) của Định nghĩa 2. Ta sẽ định nghĩa bằng quy nạp siêu hạn một hệ quy nạp $(\tilde{B}_\lambda, i_{\mu \lambda})$ được chỉ số hóa bởi $\Lambda$ gồm các vành địa phương và các đồng cấu địa phương đơn ánh, cùng các đẳng cấu $u_\lambda : \tilde{B}_\lambda \otimes_A A' \to B'_\lambda$ sao cho, với $\lambda \leq \mu$, $u_\mu \circ (i_{\mu \lambda} \otimes \mathrm{Id}_{A'}) \circ u_\lambda^{-1}$ là đơn ánh chính tắc của $B'_\lambda$ vào $B'_{\mu}$.
Nếu $\alpha$ là phần tử nhỏ nhất của $\Lambda$, ta đặt $\tilde{B}_\alpha = A, i_{\alpha \alpha} = \mathrm{Id}_A$ và lấy cho $u_\alpha$ đẳng cấu chính tắc $A \otimes_A A' \to A'$.
Cho $\nu \in \Lambda$, và giả sử rằng $\tilde{B}_\lambda, u_\lambda$ và $i_{\mu \lambda}$ đã được xây dựng khi $\lambda \leq \mu < \nu$. Cho $S_\nu$ là tập hợp các phần tử $\varepsilon$ của $\Lambda$ sao cho $\varepsilon < \nu$. Nếu $S_\nu$ không có phần tử lớn nhất, ta lấy cho $\tilde{B}_\nu$ giới hạn quy nạp của các $\tilde{B}_\lambda$ với $\lambda \in S_\nu$, lấy cho $u_\nu$ đẳng cấu hợp thành $\tilde{B}_\nu \otimes_A A' \to \lim (\tilde{B}_\lambda \otimes_A A') \to \lim B'_\lambda \to B'_\nu$, và lấy cho $i_{\nu \lambda}$, khi $\lambda \in S_\nu$, ánh xạ chính tắc của $\tilde{B}_\lambda$ vào $\tilde{B}_\nu$. Nếu $S_\nu$ có một phần tử lớn nhất $\mu$, thì $B'_\nu$ là một phép phình sơ cấp của $B'_{\mu}$. Theo A), tồn tại một phép phình sơ cấp i_{v\mu}: \tilde{B}_{\mu} \to \tilde{B}_{v} et un isomorphisme de $\tilde{B}_{\mu}$-algèbres de $\tilde{B}_{v} \otimes_{\tilde{B}_{\mu}} B'_{\mu}$ sur $B'_{v}$. Ta lấy cho $u_{v}$ đẳng cấu hợp thành của các đại số trên A
$$
\tilde{B}_{v} \otimes_{A} A' \to \tilde{B}_{v} \otimes_{\tilde{B}_{\mu}} (\tilde{B}_{\mu} \otimes_{A} A') \to \tilde{B}_{v} \otimes_{\tilde{B}_{\mu}} B'_{\mu} \to B'_{v}
$$
và lấy cho $i_{v\lambda}$, khi $\lambda \in S_{v}$, đồng cấu $i_{v\mu} \circ i_{\mu\lambda}$.

Sau đó, ta đặt $B = \tilde{B}_{\omega}$ và, với mọi $\lambda \in \Lambda$, ký hiệu $B_{\lambda}$ là ảnh của $\tilde{B}_{\lambda}$ qua đơn ánh chính tắc $\tilde{B}_{\lambda} \to B$. Họ $(B_{\lambda})_{\lambda \in \Lambda}$ thỏa mãn các điều kiện a), b), c) của Định nghĩa 2, và B là một phép phình của A. Mặt khác, đồng cấu $u_{\omega}$ là một đẳng cấu A' của $B \otimes_{A} A'$ lên B'.

#### Hệ quả {#ac-ix-a0-n2-cor-2 .statement}

Cho A là một vành địa phương và K là một mở rộng của trường thặng dư của nó $\kappa_{A}$. Khi đó tồn tại một vành địa phương B và một phép phình $A \to B$ sao cho đại số-$\kappa_{A}$ $\kappa_{B}$ là đẳng cấu với K.

Thật vậy, đồng cấu $\kappa_{A} \to K$ là một phép phình (Ví dụ 1). Áp dụng Định lý 1 với $A' = \kappa_{A}$ và $B' = K$, ta thu được sự tồn tại của một phép phình B của A và của một đẳng cấu A của $B/m_{A}B$ lên K, do đó có hệ quả.

### 3. Sự tồn tại của các $p$-vành

#### Mệnh đề 4 {#ac-ix-a0-prop-4 .statement}

Cho p là một số nguyên tố, k là một trường có đặc số p, và cho n là một số nguyên $\geq 1$, hoặc $+ \infty$. Khi đó tồn tại một $p$-ring ($\S$ 2, No. 1, Định nghĩa 1) có độ dài n mà trường thặng dư là đẳng cấu với k.

Ta có thể xem k như một mở rộng của trường thặng dư $\mathbf{Z}/p\mathbf{Z}$ của vành địa phương $\mathbf{Z}_{(p)}$. Theo hệ quả của Định lý 1, tồn tại một vành địa phương B, là một phép phình của $\mathbf{Z}_{(p)}$, sao cho $\kappa_{B}$ là đẳng cấu với k. Vành địa phương $\mathbf{Z}_{(p)}$ là chính quy và $\{ p \}$ là một hệ tọa độ của $\mathbf{Z}_{(p)}$. Theo hệ quả của Mệnh đề 2 ở No. 2, vành B là chính quy và $\{ pl_{B} \}$ là một hệ tọa độ của B. Nói cách khác, B là một vành định giá rời rạc, với iđêan cực đại $pB$. Bao đầy đủ C của B khi đó là một $p$-vành có độ dài vô hạn và trường thặng dư $\kappa_{C}$ là đẳng cấu với $\kappa_{B}$, do đó với k. Hơn nữa, với mọi số nguyên $n \geq 1$, $C/p^{n}C$ là một $p$-vành có độ dài n, với trường thặng dư đẳng cấu với $\kappa_{C}$, do đó với k.

## Bài tập {#ac-ix-a0-exercises}

Xem [các bài tập cho Phụ lục 0](exercises/a0/).
