---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 6
section_title: Propriétés spéciales aux formes hermitiennes
lang: vi
source: alg-ix-fr
pdf_pages: 0088-0112
extraction: ocr
subsections:
    - "no": 1
      title: Bases orthogonales.
      page: 0
      pdf_page: 88
    - "no": 2
      title: Groupe unitaire et groupe orthogonal.
      page: 0
      pdf_page: 91
    - "no": 3
      title: Projecteurs orthogonaux et involutions.
      page: 0
      pdf_page: 93
    - "no": 4
      title: Symétries dans le groupe orthogonal.
      page: 0
      pdf_page: 95
    - "no": 5
      title: Groupe des similitudes.
      page: 0
      pdf_page: 96
    - "no": 6
      title: Géométrie hermitienne.
      page: 0
      pdf_page: 98
statements: 17
exercises: 0
content_sha256: dd3e7055202ca685d6a88023f3c4abf2bb71e56a54c9be1fb6ebe4c1c121c387
translated_from: content/en-mt/alg/IX/06_s6_proprietes_speciales_aux_formes.md
source_lang: en-mt
translation_method: machine
source_content_sha256: 0a78bb4f9097987044d8c3ed41f08dfb8b84d8c4686fda2d034f7fc2795186ac
translation_model: gpt-5-6, gpt-5-mini, gpt-5-6-mini
translation_run: translate-vi-fe17b08a
glossary_version: 34
glossary_terms_sha256: a68c45c4f90f40c51bbdadb36190b827848e03ecf765488fc5c3da6eed926069
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 6. Các tính chất đặc biệt của các dạng Hermit

### 1. Các cơ sở trực giao.

#### Định nghĩa 1 {#alg-ix-s6-def-1 .statement}

Cho $\Phi$ là một dạng Hermit trên $E$. Một cơ sở $(e_i)$ của $E$ được gọi là trực giao đối với $\Phi$ nếu hai phần tử bất kỳ của cơ sở này là trực giao đối với $\Phi$.

Nếu thêm vào đó $\Phi(e_i, e_i) = 1$ với mọi $i$, cơ sở $(e_i)$ được gọi là trực chuẩn.

Cho $(e_i)$ là một cơ sở trực giao; nếu đặt $\Phi(e_i, e_i) = \alpha_i$, ta có
$$
\Phi(\sum_i \xi_i e_i, \sum_i \eta_i e_i) = \sum_i \xi_i \alpha_i \overline{\eta_i}.
$$

#### Bổ đề 1 {#alg-ix-s6-lem-1 .statement}

Giả sử rằng $A$ là một trường và $\Phi$ là một dạng Hermit $\neq 0$ trên $E$. Nếu mọi vectơ của $E$ đều đẳng hướng, $A$ là một trường giao hoán có đặc số 2, phản tự đẳng cấu $J$ là đồng nhất và $\Phi$ là phản xứng.

Thật vậy, bằng cách khai triển $\Phi(x + y, x + y) = 0$, xét đến các giả thiết $\Phi(x, x) = \Phi(y, y) = 0$, ta thu được quan hệ $\Phi(x, y) = -\overline{\Phi(x, y)}$ với $x, y$ tùy ý trong $E$. Vì $\Phi$ là $\neq 0$, tồn tại $x, y$ trong $E$ sao cho $\Phi(x, y) = 1$. Viết rằng $\Phi(\lambda x, y) = -\Phi(\lambda x, y)$, ta thu được $\overline{\lambda} = -\lambda$ với mọi $\lambda \in A$. Trước hết lấy $\lambda = 1$, ta thấy rằng $A$ có đặc số 2; khi đó quan hệ $\overline{\lambda} = -\lambda$ chỉ ra rằng $J$ là đồng nhất, do đó $A$ là giao hoán và $\Phi$ là phản xứng.

#### Định lý 1 {#alg-ix-s6-thm-1 .statement}

Giả sử rằng $A$ là một trường và $E$ là một không gian vectơ hữu hạn chiều có chiều $n$ trên $A$. Khi đó, với mọi dạng Hermit $\Phi$ trên $E$, $E$ có một cơ sở trực giao, trừ khi đồng thời thỏa mãn các điều kiện sau:

(C) $A$ là giao hoán có đặc số 2, phản tự đẳng cấu $J$ là đồng nhất, $\Phi$ là phản xứng và khác không.

Ta lập luận bằng quy nạp theo $n$, kết quả là hiển nhiên đối với $n = 0$. Ta có thể giả sử $\Phi \neq 0$. Nếu (C) không thỏa mãn, bổ đề 1 chỉ ra rằng tồn tại một phần tử $x \in E$ sao cho $\Phi(x, x) \neq 0$. Gọi $H$ là không gian con của $E$ trực giao với $x$; nó có chiều $\geq n - 1$, và, vì $x \in \mathbf{H}$, $\mathbf{H}$ có đúng chiều $n - 1$. Nếu hạn chế $\Psi$ của $\Phi$ lên $\mathbf{H}$ không thỏa mãn (C), thì theo giả thiết quy nạp, tồn tại một cơ sở $(e_2, \ldots, e_n)$ của $\mathbf{H}$ trực giao đối với $\Psi$; đặt $e_1 = x$, ta thu được một cơ sở trực giao $(e_1, e_2, \ldots, e_n)$ của $\mathbf{E}$. Còn lại là xét trường hợp $\mathbf{A}$ là một trường giao hoán có đặc số 2, trong đó $\mathbf{J}$ là đồng nhất, và $\Psi$ là phản xứng và $\neq 0$. Khi đó tồn tại $y, z$ trong $\mathbf{H}$ sao cho $\Psi(y, z) \neq 0$; đặt $e_1 = x + y$; để $x + \lambda z (\lambda \in \mathbf{A})$ trực giao với $e_1$, điều kiện cần và đủ là $0 = \Phi(x + y, x + \lambda z) = \Phi(x, x) + \lambda \Psi(y, z)$, một điều kiện xác định $\lambda$ một cách duy nhất; vì vô hướng $\lambda$ được chọn như vậy, ta có $\Phi(x + \lambda z, x + \lambda z) = \Phi(x, x) \neq 0$, do đó hạn chế $\Psi'$ của $\Phi$ lên không gian con $\mathbf{H}'$ của $\mathbf{E}$ trực giao với $e_1$ không phải là phản xứng; do đó ta có thể áp dụng giả thiết quy nạp cho $\mathbf{H}'$, điều này chứng minh định lý.

Khi (C) thỏa mãn, hiển nhiên không có cơ sở trực giao nào đối với $\Phi$.

#### Hệ quả 1 {#alg-ix-s6-thm-1-cor-1 .statement}

*Các ký hiệu là những ký hiệu của định lý 1, giả sử thêm rằng (C) không thỏa mãn, rằng $\Phi$ không suy biến và rằng, với mọi $x \in \mathbf{E}$, tồn tại $\rho \in \mathbf{A}$ sao cho $\Phi(x, x) = \rho \bar{\rho}$. Khi đó $\mathbf{E}$ có một cơ sở trực chuẩn đối với $\Phi$*.

Quả vậy, giả sử $(e_i)$ ($i = 1, \ldots, n$) là một cơ sở trực giao của $\mathbf{E}$. Đặt $\Phi(e_i, e_i) = \alpha_i$. Ta có $\alpha_i \neq 0$ với $i = 1, \ldots, n$ vì $\Phi$ không suy biến. Theo giả thiết, tồn tại các phần tử $\beta_i$ của $\mathbf{A}$ sao cho $\alpha_i = \beta_i \overline{\beta_i}$ với $i = 1, \ldots, n$; ta có $\beta_i \neq 0$. Khi đặt $f_i = \beta_i^{-1} e_i$, ta có $\Phi(f_i, f_i) = \beta_i^{-1} \alpha_i \overline{\beta_i^{-1}} = 1$ với mọi $i$, và $\Phi(f_i, f_j) = 0$ với $i \neq j$. Do đó $(f_i)$ là một cơ sở trực chuẩn.

#### Nhận xét {#alg-ix-s6-n1-rem-1 .statement}

Giả thiết cuối cùng của hệ quả được thỏa mãn khi $\mathbf{J}$ là đồng nhất, và mọi phần tử của $\mathbf{A}$ là bình phương của một phần tử của $\mathbf{A}$ (chẳng hạn khi $\mathbf{A}$ đóng đại số).

#### Hệ quả 2 {#alg-ix-s6-thm-1-cor-2 .statement}

*Cho $\mathbf{A}$ là một trường và $R$ là một ma trận Hermit cấp $n$ và hạng $r$ trên $\mathbf{A}$. Khi điều kiện sau đây không được thỏa mãn:

(C') $\mathbf{A}$ là giao hoán có đặc số 2, $\mathbf{J}$ là đồng nhất, $R$ là phản xứng và khác không,* tồn tại một ma trận khả nghịch $P$ cấp $n$ trên $A$ sao cho

$$
tP . R . \overline{P} = \begin{pmatrix}
\alpha_1 & 0 \ldots 0 \ldots 0 \\
0 & \alpha_2 \ldots 0 \ldots 0 \\
\cdots & \cdots \\
0 & 0 \ldots \alpha_r \ldots 0 \\
0 & 0 \ldots 0 \ldots 0 \\
\cdots & \cdots \\
0 & 0 \ldots 0 \ldots 0
\end{pmatrix}
$$

trong đó $\overline{\alpha}_i = \alpha_i \neq 0$ với $i = 1, \ldots, r$.

#### Mệnh đề 1 {#alg-ix-s6-prop-1 .statement}

*Giả sử $A$ là một trường giao hoán. Cho $\Phi$ là một dạng Hermit trên $E$, và cho $(x_n)$ ($n = 1, 2, \ldots$) là một dãy (hữu hạn hoặc vô hạn) các vectơ độc lập tuyến tính của $E$ sao cho, với mọi $n$, không gian con $E_n = Ax_1 + \cdots + Ax_n$ là không đẳng hướng. Cho $D_{jn}$ ($j \leq n$) là phần bù đại số của $\Phi(x_j, x_n)$ trong ma trận $(\Phi(x_s, x_t))_{(s,t=1,\ldots,n)}$. Khi đó $D_{nn} \neq 0$ với mọi $n$. Đặt*

$$
e_n = \sum_{j=1}^n D_{nn}^{-1} D_{jn} x_j.
$$

Khi đó, với mọi $n$, $(e_1, \ldots, e_n)$ là một cơ sở trực giao của $E_n$ và ta có

$$
\Phi(e_n, e_n) = D_{nn}^{-1} D_{n+1, n+1}.
$$

Quả thực, vì hạn chế của $\Phi$ lên $E_{n-1}$ là không suy biến, ta có $D_{nn} \neq 0$ (§ 2, mệnh đề 3); chú ý rằng $D_{11} = 1$ vì định thức của ma trận rỗng bằng 1. Các công thức (2) trước hết suy ra rằng ta có $e_n \equiv x_n$ (mod. $E_{n-1}$) với mọi $n$, và do đó rằng các $e_n$ là độc lập tuyến tính, và rằng $(e_1, \ldots, e_n)$ là một cơ sở của $E_n$. Với mọi $j < n$, ta có

$$
\Phi(e_n, x_j) = D_{nn}^{-1} \sum_{k=1}^n D_{kn} \Phi(x_k, x_j) = 0
$$

(chap. III, § 6, no. 1, công thức (12)); do đó $e_n$ là trực giao với $E_{n-1}$, và đặc biệt là với $e_j$ với $j < n$. Mặt khác, ta có

$$
\Phi(e_n, e_n) = \Phi(e_n, \sum_{j=1}^n D_{nn}^{-1} D_{jn} x_j) = \Phi(e_n, x_n) = \Phi(\sum_{j=1}^n D_{nn}^{-1} D_{jn} x_j, x_n)
$$
$$
= D_{nn}^{-1} \sum_{j=1}^n D_{jn} \Phi(x_j, x_n) = D_{nn}^{-1} D_{n+1, n+1}
$$

(chap. III, § 6, no. 1, công thức (10)). Điều này chứng minh các mệnh đề của chúng ta.

Với ký hiệu của mệnh đề 1, ta nói rằng dãy $(e_n)$ thu được từ dãy $(x_n)$ bằng quy trình trực giao hóa Gram-Schmidt.

#### Mệnh đề 2 {#alg-ix-s6-prop-2 .statement}

Cho $\Phi$ là một dạng Hermit trên $E$, và cho $(e_i)$ $(i = 1, \ldots, n)$ là một cơ sở trực giao (tương ứng, trực chuẩn) của $E$ đối với $\Phi$. Khi đó, với mọi $p \geqslant 0$, cơ sở của $\bigotimes^p E$ được tạo bởi các $e_{i_1} \otimes \cdots \otimes e_{i_p}$ và cơ sở $(e_H)$ của $\wedge^p E$ (trong đó $H$ chạy qua tập hợp các phần có $p$ phần tử của $\{1, n\}$; cf. chap. III, § 5, no. 6) là trực giao (tương ứng, trực chuẩn) đối với các mở rộng của $\Phi$ lên $\bigotimes^p E$ và $\wedge^p E$ tương ứng ($§ 1$, no. 9). Hơn nữa, nếu các ánh xạ liên kết với $\Phi$ là song ánh, cơ sở $(e'_i)$ của $E^*$ đối ngẫu với $(e_i)$ là trực giao (tương ứng, trực chuẩn) đối với dạng nghịch đảo $\widehat{\Phi}$ của $\Phi$ ($§ 1$, no. 7).

Các mệnh đề liên quan đến $\bigotimes^p E$ và $\wedge^p E$ suy ra ngay từ các công thức (35) và (37) của $§ 1$, no. 9. Mệnh đề liên quan đến dạng nghịch đảo suy ra từ sự kiện rằng ma trận của $\widehat{\Phi}$ đối với $(e'_i)$ là nghịch đảo của ma trận của $\Phi$ đối với $(e_i)$ ($§ 1$, no. 10).

### 2. Nhóm Unitary và nhóm trực giao.

Cho $\Phi$ là một dạng Hermit trên $E$; các tự đẳng cấu của A-môđun $E$ giữ $\Phi$ bất biến được gọi là các tự đẳng cấu unita (hoặc các biến đổi unita) đối với $\Phi$, và nhóm của chúng được gọi là nhóm unita liên kết với $\Phi$; nó được ký hiệu bởi $\mathbf{U}(\Phi)$. Cho một dạng toàn phương $Q \neq 0$ trên $E$, các tự đẳng cấu của A-môđun $E$ giữ $Q$ bất biến được gọi là các tự đẳng cấu trực giao (hoặc các biến đổi trực giao) đối với $Q$; nhóm của chúng được gọi là nhóm trực giao liên kết với $Q$; nó được ký hiệu bởi $\mathbf{O}(Q)$.

Mọi biến đổi trực giao đối với một dạng toàn phương $Q$ đều là unita đối với dạng song tuyến tính liên kết với $Q$. Điều đảo lại đúng khi vô hướng 2 không bằng 0 hoặc không là một ước của không trong $A$ ($§ 3$, n° 4, (13)), chẳng hạn nếu $A$ là một trường có đặc số $\neq 2$.

Xét riêng, trên môđun $E = A^n$, dạng Hermit $\Phi_0$ mà ma trận của nó đối với cơ sở chính tắc (e_i) của E là ma trận đơn vị $I_n$. Các tự đẳng cấu unita liên kết với $\Phi_0$ đơn giản được gọi là các *tự đẳng cấu* (hoặc các *biến đổi*) *unita trong n biến*; nhóm của chúng được gọi là *nhóm unita trong n biến* và đôi khi được ký hiệu bởi $\mathbf{U}(n, A)$ hoặc $\mathbf{U}_n(A)$. Ma trận $U$ của một tự đẳng cấu unita đối với $(e_i)$ được gọi là một *ma trận unita*. Ma trận như vậy là khả nghịch, và thỏa mãn, theo công thức (48) của § 1, n° 10, quan hệ

$$(4)$$
$$
{}^t U \cdot \overline{U} = I_n;
$$

ngược lại, nếu A là một vành giao hoán hoặc là một trường, một ma trận $U$ thỏa mãn (4) là khả nghịch, và khi đó là unita.

Khi J là đơn vị và 2 không bằng 0 cũng không là một ước của 0 trong A, các thuật ngữ *nhóm trực giao trong n biến*, *tự đẳng cấu trực giao* (hoặc *biến đổi trực giao*) *trong n biến* và *ma trận trực giao* được dùng thay cho các thuật ngữ trước đó, và người ta viết $\mathbf{O}(n, A)$ (tương ứng $\mathbf{O}_n(A)$) thay cho $\mathbf{U}(n, A)$ (tương ứng $\mathbf{U}_n(A)$). Khi đó quan hệ (4) trở thành

$$(5)$$
$$
{}^t U \cdot U = I_n
$$

và, vì A là giao hoán, đó là một điều kiện cần và đủ để $U$ là một ma trận trực giao.

#### Mệnh đề 3 {#alg-ix-s6-prop-3 .statement}

*Giả sử rằng A là một trường giao hoán và rằng E có số chiều hữu hạn $> 0$. Cho $\Phi$ là một dạng Hermit không suy biến trên E. Ánh xạ $u \to \det u$ là một đồng cấu của nhóm unita $\mathbf{U}(\Phi)$ liên kết với $\Phi$ lên nhóm con nhân H của A tạo bởi các phần tử $\rho$ sao cho $\rho \overline{\rho} = 1$ (nhóm con thu gọn thành $\{1, -1\}$ khi J là đơn vị).*

Vậy hãy cho $u$ là một phần tử của $\mathbf{U}(\Phi)$, $U$ là ma trận của nó đối với một cơ sở của E, và $R$ là ma trận của $\Phi$ đối với cơ sở này. Quan hệ $R = {}^t U \cdot R \cdot \overline{U}$ ($§ 1$, n° 10, công thức (48)) cho thấy rằng $(\det U)(\det \overline{U}) = 1$ vì $R$ khả nghịch; do đó $(\det u)(\det u) = 1$. Đồng cấu $u \to \det u$ ánh xạ $\mathbf{U}(\Phi)$ lên H. Thật vậy, khi A có đặc số 2 và J là đồng nhất, H được thu gọn thành phần tử 1. Trong trường hợp ngược lại, tồn tại một cơ sở trực giao $(e_i)$ ($i = 1, \ldots, n$) của E (định lý 1); với mọi $\rho \in A$ sao cho $\rho \overline{\rho} = 1$, hãy cho $u$ là tự đẳng cấu của E xác định bởi $u(e_1) = \rho e_1$ và $u(e_i) = e_i$ với $i = 2, \ldots, n$; khi đó $u$ là unitary và $\det u = \rho$, do đó mệnh đề.

Dưới các điều kiện của mệnh đề 3, hạt nhân của đồng cấu $u \to \det u$ là một nhóm con chuẩn của $\mathbf{U}(\Phi)$, được gọi là nhóm unitary đặc liên kết với $\Phi$; đôi khi nó được ký hiệu bởi $\mathbf{SU}(\Phi)$.

Khi $J$ là đồng nhất và $A$ không có đặc số 2, nhóm này cũng được gọi là nhóm trực giao đặc liên kết với $\Phi$ (hoặc với dạng toàn phương $Q(x) = \Phi(x, x)$) và đôi khi được ký hiệu bởi $\mathbf{SO}(Q)$.

Nếu $E = A^n$ và $\Phi$ là dạng mà ma trận của nó đối với cơ sở chính tắc của $E$ là ma trận đơn vị, các ký hiệu $\mathbf{SU}(n, A)$ hoặc $\mathbf{SU}_n(A)$ và $\mathbf{SO}(n, A)$ hoặc $\mathbf{SO}_n(A)$ được dùng.

### 3. Các phép chiếu trực giao và các phép đối hợp.

Trong suốt No. này, ta giả sử rằng vô hướng 2 là khả nghịch trong $A$ (chẳng hạn, rằng $A$ là một trường có đặc số $\neq 2$), và rằng $\Phi$ là một dạng Hermit không suy biến trên $E$. Ta ký hiệu nghịch đảo của 2 bởi $\frac{1}{2}$.

#### Bổ đề 2 {#alg-ix-s6-lem-2 .statement}

Để một tự đồng cấu $u$ của $E$ thỏa mãn $u^2 = 1$, điều kiện cần và đủ là $\frac{1}{2}(1 - u)$ là một phép chiếu trong $E$; khi đó $u$ là hiệu của hai phép chiếu $\frac{1}{2}(1 + u)$ và $\frac{1}{2}(1 - u)$.

Thật vậy, trong vành $\mathcal{L}(E)$, quan hệ $\left( \frac{1}{2}(1 - u) \right)^2 = \frac{1}{2}(1 - u)$ tương đương với $u^2 = 1$. Phần còn lại là tầm thường.

Một tự đồng cấu $u$ của $E$ sao cho $u^2 = 1$ (khi đó tất nhiên là một tự đẳng cấu của $E$ bằng với nghịch đảo của nó) được gọi là một phép đối hợp. Đặt $\varphi = \frac{1}{2}(1 - u)$, $U^- = \varphi(E)$, $U^+ = \varphi^{-1}(0)$ ($= \omega(E)$ khi đặt $\omega = \frac{1}{2}(1 + u)$); ta biết rằng $E$ là tổng trực tiếp của $U^+$ và $U^-$ (Chương VIII, § 1, No. 1), và ta có $u(x) = x$ trong $U^+$, $u(x) = -x$ trong $U^-$. Khi $A$ là một trường và $E$ là hữu hạn chiều, suy ra, vì $A$ có đặc số $\neq 2$, rằng các vectơ riêng duy nhất $\neq 0$ của $u$ là các phần tử ≠ 0 trong U^+ hoặc trong U^-; chúng tương ứng lần lượt với các giá trị riêng + 1 và -1.

#### Mệnh đề 4 {#alg-ix-s6-prop-4 .statement}

Cho u ∈ GL(E) là một phép đối hợp. Các tính chất sau là tương đương:
a) u thuộc nhóm unita liên kết với Φ ;
b) các môđun con U^+ = $\frac{1}{2}(1 + u)(E)$ và U^- = $\frac{1}{2}(1 - u)(E)$
là trực giao (và do đó không đẳng hướng).
Ngoài ra, nếu A là một trường và E là hữu hạn chiều, các tính chất a) và b) tương đương với:
c) u = u*.
Thật vậy, với x ∈ U^+ và y ∈ U^-, quan hệ $\Phi(u(x), u(y)) = \Phi(x, y)$
cho $2\Phi(x, y) = 0$, do đó a) kéo theo b). Ngược lại, hiển nhiên ta có $\Phi(u(x), u(y)) = \Phi(x, y)$ khi x và y cùng thuộc U^+ hoặc cùng thuộc U^-, và, theo b), quan hệ này vẫn đúng khi một trong hai phần tử thuộc U^+ và phần tử kia thuộc U^-; vì E là tổng trực tiếp của U^+ và U^-, ta thấy rằng b) kéo theo a). Cuối cùng, khi E là một không gian vectơ hữu hạn chiều, tự đồng cấu liên hợp u* được xác định vì Φ không suy biến; quan hệ a) tương đương với $uu^* = 1$ (§ 1, No. 8, hệ quả của mệnh đề 8); vì $u^2 = 1$ theo giả thiết, a) và c) là tương đương.

#### Hệ quả 1 {#alg-ix-s6-prop-4-cor-1 .statement}

Giả sử rằng A là một trường và rằng E là hữu hạn chiều. Ánh xạ $u \to \frac{1}{2}(1 + u)(E)$ là một song ánh từ tập hợp các phép đối hợp u thuộc nhóm unita liên kết với Φ lên tập hợp các không gian con không đẳng hướng của E; không gian con U^+ tương ứng với u là tập hợp các phần tử của E bất biến dưới u.

Theo mệnh đề 4, chỉ cần chứng minh rằng mọi không gian con không đẳng hướng M của E là tập hợp các vectơ bất biến dưới một phép đối hợp $u \in \mathbf{U}(\Phi)$, và rằng phép đối hợp này là duy nhất. Bây giờ E là tổng trực tiếp của M và M^0 (§ 4, No. 1, hệ quả của mệnh đề 1), và tất nhiên $u(x) = x$ với $x \in M$ và $u(x) = -x$ với $x \in M^0$ theo mệnh đề 4; các quan hệ này xác định duy nhất u, và tự đồng cấu u được xác định như vậy hiển nhiên trả lời câu hỏi (mệnh đề 4).

Ta nói rằng phép đối hợp $u$ được xác định như vậy là phép đối xứng đối với không gian con không đẳng hướng M.

#### Hệ quả 2 {#alg-ix-s6-prop-4-cor-2 .statement}

Giả sử rằng $\mathbf{A}$ là một trường và rằng $\mathbf{E}$ là hữu hạn chiều. Để một phép chiếu $\nu$ trong $\mathbf{E}$ có tính chất rằng $\nu(\mathbf{E})$ và $\nu(0)$ trực giao (và do đó không đẳng hướng), điều kiện cần và đủ là $\nu = \nu^*$.

Chỉ cần áp dụng mệnh đề 4 cho phép đối hợp $u = 1 - 2\nu$.

Một phép chiếu thỏa mãn điều kiện của Hệ quả 2 được gọi là một phép chiếu trực giao đối với $\Phi$.

### 4. Các phép đối xứng trong nhóm trực giao.

Trừ khi được phát biểu rõ ràng khác đi, trong No. này, ta giả sử rằng $\mathbf{A}$ là một trường giao hoán có đặc số $\neq 2$, và rằng $\Phi$ là dạng song tuyến tính đối xứng liên kết với một dạng toàn phương không suy biến Q trên $\mathbf{E}$. Nhắc lại rằng ta có $\Phi(x, x) = 2Q(x)$ với $x \in \mathbf{E}$ (§ 3, No. 4).

Cho $H$ là một siêu phẳng không đẳng hướng trong $\mathbf{E}$, và cho $u$ là phép đối xứng đối với $H$ (No. 3). Cho $a \neq 0$ là một vectơ vuông góc với $H$; theo giả thiết, $u(a) = -a$. Mọi vectơ $x \in \mathbf{E}$ đều có thể được viết theo một và chỉ một cách dưới dạng $x = \lambda a + y$ với $\lambda \in \mathbf{A}$ và $y \in \mathbf{H}$; vì $a$ và $y$ vuông góc với nhau, ta có $\Phi(x, a) = \lambda \Phi(a, a)$, do đó, vì $a$ là không đẳng hướng (§ 4, No. 1, hệ quả của Mệnh đề 1), $\lambda = \Phi(x, a)\Phi(a, a)^{-1}$. Do đó, ta có

$$
u(x) = \lambda u(a) + u(y) = -\lambda a + y = x - 2\lambda a,
$$

do đó

$$
u(x) = x - 2\Phi(x, a)\Phi(a, a)^{-1}.a = x - \Phi(x, a)Q(a)^{-1}.a.
$$

Cần lưu ý rằng vế cuối của (6) vẫn có nghĩa khi $\mathbf{A}$ là một trường có đặc số 2, và $a$ là một vectơ không suy biến của $\mathbf{E}$; ta kiểm tra ngay lập tức rằng khi đó vẫn có $Q(u(x)) = Q(x)$ với mọi $x \in \mathbf{E}$, nói cách khác $u \in \mathbf{O}(Q)$. Phép đối hợp $u$ được xác định như vậy lại được gọi là phép đối xứng đối với siêu phẳng vuông góc với $a$ (xem Bài tập 28).

#### Mệnh đề 5 {#alg-ix-s6-prop-5 .statement}

Giả sử không gian vectơ $\mathbf{E}$ có số chiều hữu hạn n. Nhóm trực giao $\mathbf{O}(Q)$ liên kết với $Q$ khi đó được sinh bởi các phép đối xứng đối với các siêu phẳng không đẳng hướng của $\mathbf{E}$.

Vì mệnh đề hiển nhiên đối với $n = 0$, ta lập luận bằng quy nạp theo $n$. Cho $u$ là một phép biến đổi trực giao của $E$, và cho $x$ là một vectơ không đẳng hướng của $E$ (Bổ đề 1); phân biệt ba trường hợp:

a) Trước hết giả sử rằng $u(x) = x$. Khi đó siêu phẳng $H$ vuông góc với $x$ là không đẳng hướng, và ta có $u(H) = H$. Phép hạn chế $u'$ của $u$ lên $H$ do đó thuộc nhóm trực giao $O(Q')$ liên kết với phép hạn chế $Q'$ của $Q$ lên $H$. Giả thiết quy nạp kéo theo, vì $Q'$ không suy biến, rằng ta có $u' = v_1' \ldots v_m'$, trong đó $v_i'$ là một phép đối xứng đối với một siêu phẳng $L_i$ của $H$. Tự đồng cấu $v_i$ của $E$ mở rộng $v_i'$ và thỏa mãn $v_i(x) = x$ khi đó là phép đối xứng đối với siêu phẳng $Ax + L_i$ của $E$. Hiển nhiên $u = v_1 v_2 \ldots v_m$.

b) Ở vị trí thứ hai, giả sử rằng $u(x) = -x$. Nếu $s$ ký hiệu phép đối xứng đối với siêu phẳng $H$ vuông góc với $x$, và nếu đặt $v = su$, ta có $v(x) = x$, và ta quy về trường hợp a).

c) Cuối cùng, ta xét trường hợp tổng quát, và đặt $y = u(x)$, sao cho $Q(y) = Q(x)$. Với các điều kiện này, các vectơ $x - y$ và $x + y$ không thể đồng thời là đẳng hướng, vì, từ các hệ thức $Q(x - y) = 0$ và $Q(x + y) = 0$, ta sẽ suy ra, bằng cách cộng vế với vế, $2(Q(x) + Q(y)) = 0$ ($§ 3$, no 4, déf. 2), do đó $4Q(x) = 0$, trái với giả thiết. Chẳng hạn, giả sử rằng $a = x - y$ không đẳng hướng; khi đó ta có

$$
\Phi(y, a) = Q(y + a) - Q(y) - Q(a) = Q(x) - Q(y) - Q(a) = -Q(a);
$$

do đó, nếu $s$ ký hiệu phép đối xứng đối với siêu phẳng vuông góc với $a$, công thức (6) chứng minh rằng $s(y) = y + a = x$; khi đặt $v = su$, ta có $v(x) = x$, và ta quy về trường hợp a). Nếu $a = x - y$ là đẳng hướng và $b = x + y$ không đẳng hướng, ta thấy tương tự rằng ta quy về trường hợp b).

### 5. Nhóm các phép đồng dạng.

Cho $\Phi$ là một dạng Hermit trên $E$. Một tự đẳng cấu $u$ của A-môđun $E$ được gọi là một phép đồng dạng (đối với $\Phi$) nếu tồn tại một phần tử khả nghịch $\alpha$ của $A$ sao cho

$$
\Phi(u(x), u(y)) = \alpha \Phi(x, y)
$$

với mọi $x, y$ trong $E$. Các phép đồng dạng tạo thành một nhóm $\Gamma$.

Khi $\Phi$ nhận các giá trị là những phần tử chính quy của $A$ (ví dụ khi $A$ là một trường và $\Phi \neq 0$), phần tử $\alpha$ của $A$ thỏa mãn (7) được xác định duy nhất bởi $u$; nó được gọi là *nhân tử* của phép đồng dạng $u$. Thay thế $x$ bởi $\lambda x$ trong (7), khi đó ta thấy rằng $\alpha$ thuộc *tâm* của $A$; đổi chỗ $x$ và $y$ trong (7), ta còn thấy thêm rằng $\overline{\alpha} = \alpha$. Nếu, với $u \in \Gamma$, ta ký hiệu bởi $\alpha(u)$ nhân tử của $u$, thì ánh xạ $u \to \alpha(u)$ là một đồng cấu của $\Gamma$ vào nhóm nhân của các phần tử khả nghịch của tâm của $A$. Hạt nhân của đồng cấu này là nhóm đơn vị liên kết với $\Phi$, do đó nó là một nhóm con chuẩn của $\Gamma$. Cho $\beta$ là một phần tử khả nghịch của tâm của $A$, $\nu$ là phép vị tự có tỉ số $\beta$, và $\omega$ là một tự đẳng cấu đơn vị của $E$; khi đó $\nu \omega = \omega \nu$ là một phép đồng dạng của $E$, và nhân tử của nó là $\beta \overline{\beta}$. Ngược lại, cho $u$ là một phép đồng dạng có nhân tử có dạng $\beta \overline{\beta}$ ($\beta$ ký hiệu một phần tử khả nghịch của tâm của $A$); khi đó $u \nu^{-1}$ là một tự đẳng cấu đơn vị $\omega$, và do đó $u$ có dạng $\nu \omega$.

Giả sử bây giờ rằng $A$ là một trường, $E$ là một không gian vectơ hữu hạn chiều, và rằng $\Phi$ là không suy biến. Với mọi phép đồng dạng $u$ có nhân tử $\alpha$ ta có
$$
\Phi(x, \alpha y) = \alpha \Phi(x, y) = \Phi(u(x), u(y)) = \Phi(x, u^*(u(y))),
$$
suy ra $u^* u$ là phép vị tự có tỉ số $\alpha$. Nếu $A$ là giao hoán, và nếu $n$ ký hiệu chiều của $E$, từ điều này và từ công thức (50) của § 1, No. 10 ta suy ra rằng ta có
$$
(\det u)(\overline{\det u}) = \alpha^n.
$$

Phân biệt khi đó hai trường hợp:
1°) Số nguyên $n$ là *lẻ*, nghĩa là, $n = 2q + 1$. Khi đó, đặt $\rho = \alpha^{-q} (\det u)$, ta có $\alpha = (\det u) (\det u)^{-2q} = \rho \overline{\rho}$. Do đó $u$ là tích của phép vị tự tỉ số $\rho$ và một tự đẳng cấu unita.
2°) Số nguyên $n$ là *chẵn*, nghĩa là, $n = 2q$. Khi đó, đặt $\rho = \alpha^{-q} (\det u)$, ta có $\rho \overline{\rho} = 1$. Đặc biệt, khi $J$ là đồng nhất, ta có $(\det u)^2 = \alpha(u)^{2q}$; các phép đồng dạng $u$ sao cho $\det u = \alpha(u)^q$ (tương ứng $\det u = -\alpha(u)^q$) được gọi là *trực tiếp* (tương ứng *nghịch đảo*); các phép đồng dạng trực tiếp tạo thành một nhóm con chuẩn tắc có chỉ No. 2 của $\Gamma$;

các phép vị tự tỉ số $\neq 0$ là các phép đồng dạng trực tiếp; điều này cũng đúng đối với các phép biến đổi trực giao có định thức 1 (Số 2); các phép biến đổi trực giao có định thức -1 là các phép đồng dạng nghịch đảo.

Các định nghĩa và kết quả trước đây vẫn đúng đối với các dạng $\varepsilon$-Hermit ($§ 3$, No. 1), và đặc biệt đối với các dạng phản xứng.

Cho A là một trường giao hoán và Q là một dạng toàn phương $\neq 0$ trên E. Một phép đồng dạng (đối với Q) là một tự đẳng cấu $u$ của E sao cho tồn tại một phần tử khác không $\alpha$ của A (được gọi là nhân tử của $u$) mà $Q(u(x)) = \alpha Q(x)$ với mọi $x \in E$. Rõ ràng rằng khi đó $u$ là một phép đồng dạng với nhân tử $\alpha$ đối với dạng song tuyến tính liên kết với Q; đảo lại đúng khi đặc số của A là $\neq 2$.

### 6. Hình học Hermit.

#### Định nghĩa 2 {#alg-ix-s6-def-2 .statement}

Cho A là một trường, L là một không gian affine trên A và T là không gian các phép tịnh tiến của L (Chương II, ấn bản thứ 2, Phụ lục II). Nếu T được trang bị một dạng Hermit không suy biến $\Phi$, thì L được gọi là một không gian Hermit trên A, và $\Phi$ là dạng metric của L.

Nếu J là đồng nhất (điều này kéo theo A là giao hoán), thì L được gọi là một không gian Euclid.

Nếu $a$ và $b$ là hai điểm của L, đặt $e(a, b) = \Phi(b - a, b - a)$. Cho c là một điểm thứ ba của L. Để $b - a$ và $c - a$ trực giao, theo công thức (17) của $§ 1$, No. 5, cần phải có $e(b, c) = e(a, b) + e(a, c)$, và điều kiện này là đủ khi $J = 1$ và A không có đặc số 2 (“định lý Pythagore”).

Hai đa tạp tuyến tính của L được gọi là trực giao nếu các phương của chúng (Chương II, ấn bản thứ 2, Phụ lục II, No. 3) trực giao. Một đa tạp tuyến tính của L được gọi là đẳng hướng (tương ứng toàn đẳng hướng) nếu phương của nó là đẳng hướng (tương ứng toàn đẳng hướng). Một vectơ của T được gọi là trực giao với một đa tạp tuyến tính của L nếu nó trực giao với phương của đa tạp đó.

Cho V là một đa tạp tuyến tính trong L, và $x$ là một điểm của L. Tập hợp các điểm $y$ của L sao cho $y - x$ trực giao với V là một đa tạp tuyến tính W đi qua $x$; W được gọi là đa tạp trực giao toàn phần (hoặc, đơn giản hơn, đa tạp trực giao) với V đi qua x. Nếu L có số chiều hữu hạn, chiều của W bằng đối chiều của V. Hơn nữa, nếu V không đẳng hướng, các phương của V và W là bù nhau (§ 4, No. 1, hệ quả của mệnh đề 1); khi đó W cắt V tại một điểm duy nhất $x_1$; lấy một gốc trong V, ta thấy ngay rằng, với V cố định, ánh xạ $x \to x_1$ là một ánh xạ tuyến tính lũy đẳng affine; nó được gọi là phép chiếu trực giao của L lên V; ánh xạ tuyến tính liên kết với nó (Chương II, ấn bản thứ 2, Phụ lục II, No. 4) là phép chiếu trực giao của T lên phương của V (No. 3).

#### Định nghĩa 3 {#alg-ix-s6-def-3 .statement}

Cho L là một không gian Hermit trên một trường A, T là không gian các phép tịnh tiến của L. Một phép dịch chuyển (tương ứng phép đồng dạng) của L là một song ánh affine $u$ của L lên L sao cho ánh xạ tuyến tính $\varphi$ liên kết với $u$ trong T (Chương II, ấn bản thứ 2, Phụ lục II, No. 4) là unita (tương ứng là một phép đồng dạng).

Nhóm các phép tịnh tiến là một nhóm con chuẩn tắc của nhóm affine; do đó nó là một nhóm con chuẩn tắc của nhóm các phép đồng dạng và của nhóm các phép dịch chuyển. Với mọi $a \in L$, cho $G_a$ là nhóm các phép đồng dạng (tương ứng phép dịch chuyển) giữ cố định a; nếu L được đồng nhất với T bằng cách lấy a làm gốc, $G_a$ là nhóm các phép đồng dạng (tương ứng nhóm unita) của T. Mọi phép đồng dạng (tương ứng phép dịch chuyển) u có thể được viết, theo một và chỉ một cách, dưới dạng $u = u_1 t_1$ trong đó $u_1 \in G_a$ và $t_1 \in T$, và cũng dưới dạng $u = t_2 u_2$ trong đó $u_2 \in G_a$ và $t_2 \in T$; hơn nữa $u_2 = u_1$ và $t_2 = u_1 t_1 u_1^{-1}$ (Chương II, ấn bản thứ 2, Phụ lục II, No. 4).

Cho $u$ là một phép vị tự trong L, $\varphi$ là phép vị tự liên kết trong T. Nhân tử của $\varphi$ cũng được gọi là nhân tử của $u$ (No. 5). Nếu nhân tử này được ký hiệu bởi $\alpha(u)$, ánh xạ $u \to \alpha(u)$ là một đồng cấu của nhóm các phép vị tự của L vào nhóm nhân của các phần tử khả nghịch của tâm của A; hạt nhân của nó là nhóm các phép tịnh tiến, do đó là một nhóm con chuẩn tắc của nhóm các phép vị tự. Khi A giao hoán và L có số chiều hữu hạn, giữa định thức det $u$ (bằng theo định nghĩa với det $\varphi$) và $\alpha(u)$ có cùng các quan hệ như trong No. 5. Các phép tịnh tiến $u$ sao cho det $u = 1$ tạo thành một nhóm con chuẩn tắc của nhóm các phép tịnh tiến; nhóm con này có chỉ số 2 nếu A là một trường giao hoán có đặc số $\neq 2$ và J là đồng nhất.

#### Mệnh đề 6 {#alg-ix-s6-prop-6 .statement}

*Cho L là một không gian Hermit hữu hạn chiều trên A, có dạng metric có chỉ số 0. Mọi phép vị tự u của L, với nhân tử $\mu \neq 1$, khi đó nhận đúng một điểm bất động.*

Thật vậy, cho $a$ là một điểm của L. Có một phép vị tự $\varphi$ của L giữ cố định $a$ và một phép tịnh tiến $t$ của L sao cho $u = t \varphi$. Nói rằng $b$ là một điểm bất động của $u$ tương đương với nói rằng $\varphi(b) - b = t$. Để chứng minh rằng phương trình này nhận đúng một nghiệm $b$, đồng nhất L với không gian các phép tịnh tiến T của nó bằng cách lấy $a$ làm gốc. Khi đó chỉ cần chứng minh rằng tự đồng cấu $\varphi - 1$ của T là khả nghịch, hay nói cách khác rằng quan hệ $\varphi(x) - x = 0$ ($x \in T$) kéo theo $x = 0$. Bây giờ, nếu $\varphi(x) - x = 0$, ta có $\Phi(x, x) = \Phi(\varphi(x), \varphi(x)) = \mu \Phi(x, x)$, do đó $\Phi(x, x) = 0$ vì $\mu \neq 1$; điều này kéo theo $x = 0$ vì $\Phi$ có chỉ số 0. QED.

Giả sử A là một trường có đặc số $\neq 2$. Mọi phép tịnh tiến $u$ của L sao cho $u^2 = 1$ đều nhận ít nhất một điểm bất động, chẳng hạn trung điểm $\frac{1}{2}(x + u(x))$ của hai điểm tương ứng; bằng cách lấy điểm này làm gốc, ta thấy rằng tự đẳng cấu đơn vị của T liên kết với $u$ là một phép đối xứng (No. 3). Cho V là một đa tạp tuyến tính không đẳng hướng trong L; một phép tịnh tiến $u$ được gọi là *phép đối xứng đối với V* nếu, bằng cách lấy một gốc trong V, $u$ được đồng nhất với phép đối xứng đối với V của T. Điều này tương đương với việc nói rằng $u(x)$ được thu được theo cách sau: ký hiệu $x_1$ là phép chiếu trực giao của $x$ lên V, ta có $u(x) - x = 2(x_1 - x)$.

*Bài tập.* — 1) Giả sử A là một trường giao hoán. Cho một ma trận Hermit $R$ cấp $n$ trên A, các *định thức con chính* cấp $r$ của $R$ được gọi là các định thức con nhận được bằng cách xóa trong $R$ $n - r$ hàng và $n - r$ cột có *cùng các chỉ số*.

a) Nếu một minor chính cấp $r$ của $R$ khác không, nhưng nếu tất cả các minor chính cấp $r + 1$ và $r + 2$ chứa minor cấp $r$ này đều bằng không, bây giờ chứng minh rằng $R$ có hạng $r$ (xem chương III, § 7, Bài tập 1 và § 8, Bài tập 11 và chương IV, § 2, Bài tập 10). Suy ra rằng, để $R$ có hạng $r$, điều kiện cần và đủ là tồn tại một minor chính cấp $r$ là $\neq 0$, và tất cả các minor chính cấp $r + 1$ và $r + 2$ đều bằng không.

b) Suy ra từ a) rằng nếu $R$ có hạng $r$, tồn tại một phép hoán vị $\sigma \in \mathfrak{S}_n$ sao cho, nếu cùng phép hoán vị $\sigma$ được thực hiện trên các hàng và cột của $R$, và nếu $S$ là ma trận thu được, và $\Delta_k$ là minor chính cấp $k$ của $S$ thu được bằng cách loại bỏ trong $S$ các hàng và cột có chỉ số $> k$, thì hai tính chất sau đúng: $1^\circ \Delta_r \neq 0$; $2^\circ$ không có chỉ số $k < r$ sao cho $\Delta_k = \Delta_{k+1} = 0$.

2) Giả sử rằng $A$ là một trường giao hoán, và rằng $E$ có số chiều hữu hạn $n$. Cho $\Phi$ là một dạng Hermit song tuyến sesqui trên $E$, thỏa mãn điều kiện (T) của § 4, No. 2, $R = (\alpha_{ij})$ là ma trận của $\Phi$ đối với một cơ sở $(e_i)$ của $E$.

a) Nếu $\Phi$ có hạng $r$, và nếu minor chính (Bài tập 1) thu được bằng cách loại bỏ trong $R$ các hàng và cột có chỉ số $> r$ là khác không, chứng minh rằng tồn tại một cơ sở mới $(f_i)$ của $E$ sao cho $e_i = f_i$ với $1 \leq i \leq r$ và ma trận của $\Phi$ đối với $(f_i)$ thu được bằng cách thay thế bởi 0 trong $R$ tất cả các $\alpha_{ij}$ sao cho $i > r$ hoặc $j > r$ (xét không gian con $E^0$ trực giao với $E$).

b) Suy ra từ a) rằng nếu $\Phi$ có hạng $n$, và nếu phần bù $\Delta_{n-1}$ của $\alpha_{nn}$ trong định thức $\Delta = \det R$ khác không, thì tồn tại một cơ sở mới $(f_i)$ của $E$ sao cho $f_i = e_i$ với $1 \leq i \leq n-1$, và sao cho

$$
\Phi(x, y) = \Phi\left( \sum_{i=1}^n \xi_i f_i, \sum_{i=1}^n \eta_i f_i \right) = \sum_{i=1}^{n-1} \sum_{j=1}^{n-1} \alpha_{ij} \xi_i \overline{\eta_j} + \frac{\Delta}{\Delta_{n-1}} \xi_n \overline{\eta_n}
$$

(xét dạng Hermit có ma trận đối với $(e_i)$ nhận được bằng cách thay thế $\alpha_{nn}$ bởi $\alpha_{nn} - \frac{\Delta}{\Delta_{n-1}}$ trong $R$).

c) Giả sử rằng $\Phi$ có hạng $n$, rằng $\Delta_{n-1} = 0$, nhưng rằng phần tử chính $\Delta_{n-2}$ của $R$ nhận được bằng cách xóa các hàng và cột có các chỉ số $n-1$ và $n$ trong $R$ khác không. Bây giờ chứng minh rằng tồn tại một cơ sở mới $(f_i)$ của $E$ sao cho $f_i = e_i$ với $1 \leq i \leq n-2$, và sao cho

$$
\Phi(x, y) = \left( \sum_{i=1}^n \xi_i f_i, \sum_{i=1}^n \eta_i f_i \right) = \sum_{i=1}^{n-2} \sum_{j=1}^{n-2} \alpha_{ij} \xi_i \overline{\eta_j} + \xi_{n-1} \overline{\eta_n} + \xi_n \overline{\eta_{n-1}}.
$$

(Nếu $H$ là siêu phẳng sinh bởi $e_1, \ldots, e_{n-1}$, là đẳng hướng, nhận xét rằng trực giao phải của $H$ không nằm trong không gian con sinh bởi $e_1, \ldots, e_{n-2}$, và sử dụng Mệnh đề 2 của § 4, No. 2).

3) Cho $A$ là một trường hữu hạn, $E$ là một không gian vectơ hữu hạn chiều trên $A$, $\Phi$ là một dạng song tuyến tính Hermit sesqui không suy biến trên $E$, đối với một tự đẳng cấu $J \neq 1$ của $A$. Bây giờ chứng minh rằng $E$ thừa nhận một cơ sở trực chuẩn đối với $\Phi$ (xem Chương V, § 11, No. 5, Hệ quả của Định lý 3).

4) Cho $A$ là một trường hữu hạn có đặc số $\neq 2$, $E$ là một không gian vectơ hữu hạn chiều có chiều $n$ trên $A$.

a) Chứng minh rằng với mọi dạng song tuyến tính đối xứng không suy biến $\Phi$ trên $E$, tồn tại một cơ sở trực giao $(e_i)$ của $E$ sao cho $\Phi(e_i, e_i) = 1$ với $1 \leq i \leq n-1$, $\Phi(e_n, e_n) = \Delta$ (biệt thức của $\Phi$ đối với $(e_i)$). (Nhận xét rằng nếu $\alpha \beta \neq 0$, phương trình $\alpha \xi^2 + \beta \eta^2 = \gamma$ luôn có nghiệm $(\xi, \eta)$ trong $A$ nếu $\gamma \neq 0$ (chương V, § 11, bài tập 4)).

b) Để hai dạng song tuyến tính đối xứng không suy biến trên E là tương đương, điều kiện cần và đủ là thương của các biệt thức của chúng (đối với cùng một cơ sở của E) là một bình phương trong A. Suy ra rằng, nếu n là lẻ, thì đối với mọi dạng song tuyến tính đối xứng không suy biến $\Phi$ trên E, tồn tại một cơ sở trực giao sao cho ma trận của $\Phi$ có dạng $\lambda I_n \ (\lambda \in A)$; chỉ số của $\Phi$ khi đó là $(n-1)/2$.

c) Nếu $n = 2m$ là chẵn, chứng minh rằng chỉ số của một dạng song tuyến tính đối xứng không suy biến $\Phi$ trên E là m nếu $(-1)^m \Delta$ là một bình phương trong A, là $m-1$ trong trường hợp ngược lại.

5) Cho A là một trường giao hoán có đặc số $\neq 2$. Cho I là một đa thức với các hệ số trong A, đối với $n(n+1)/2$ phần tử bất định $X_{ij} \ (1 \leq i \leq j \leq n)$; đối với mọi ma trận đối xứng $R = (\alpha_{ij})$ trên một trường mở rộng giao hoán $A'$ của A, ký hiệu $I(R)$ là phần tử của $A'$ thu được bằng cách thay $\alpha_{ij}$ cho phần tử bất định $X_{ij} \ (i \leq j)$ trong I.

Giả sử I có tính chất là, đối với ma trận $U = (u_{ij})$ với $u_{ij} = X_{ij}$ với $i \leq j$, $u_{ij} = X_{ji}$ với $i > j$ và ma trận vuông $P = (Y_{ij})$ cấp n (trong đó các $Y_{ij}$ là $n^2$ phần tử bất định khác), ta có

$$
I(PUP) = (\det P)^h I(U)
$$

trong đó h là một số nguyên $> 0$. Chứng minh rằng h là chẵn và $I(U) = \gamma (\det U)^k$, trong đó $h = 2k$ và $\gamma \in A$. (Dùng định lý 1, chứng minh rằng đối với mọi ma trận đối xứng $R$ trên bao đóng đại số $\Omega$ của A, ta có $(I(R))^2 = \lambda (\det R)^h$, trong đó $\lambda \in \Omega$, và dùng sự kiện rằng đa thức $\det U$ theo các $X_{ij}$ không phải là một bình phương, bằng cách xét các số hạng của đa thức này chứa một $X_{ii}$.

Cho A là một trường định giá đầy đủ không rời rạc, giao hoán và có đặc số $\neq 2$ (Top. gén., chap. IX, § 3, no 2), $\Phi$ là một dạng Hermit không suy biến trên một không gian vectơ E có chiều hữu hạn n trên A, $R = (\alpha_{ij})$ là ma trận của $\Phi$ đối với một cơ sở $(e_i)$ của E. Chứng minh rằng tồn tại $\varepsilon > 0$ sao cho, đối với mọi ma trận Hermit $R' = (\chi'_{ij})$ thỏa mãn các điều kiện $|\alpha'_{ij} - \alpha_{ij}| \leq \varepsilon$ đối với mọi cặp $(i, j)$, dạng $\Phi'$ có $R'$ làm ma trận đối với cơ sở $(e_i)$ là tương đương với $\Phi$. (Rút gọn về trường hợp trong đó $R$ là đường chéo; dùng bài tập 2 b) bằng cách dựa vào bổ đề sau: tồn tại một số $a > 0$ sao cho với $|\eta| \leq a$, tồn tại trong A một phần tử $\xi$ sao cho $\xi^2 = 1 - \eta$. Để chứng minh bổ đề này, sẽ dùng chuỗi nhị thức của $(1-x)^{1/2}$.)

Cho A là một trường giao hoán không sắp thứ tự được (chương VI, § 2, bài tập 8) có đặc số $\neq 2$, E là một không gian vectơ hữu hạn chiều $n > 0$ trên A, Q là một dạng toàn phương không suy biến trên E, $(e_i)$ là một cơ sở trực giao đối với Q, sao cho $Q \left( \sum_{i=1}^n \xi_i e_i \right) = \sum_{i=1}^n \alpha_i \xi_i^2$. Với $1 \leq r \leq n$, đặt $Q_r(\xi_1, \ldots, \xi_r) = \sum_{i=1}^r \alpha_i \xi_i^2$, và ký hiệu $M_r$ là tập hợp các giá trị của Q_r khi các $\xi_i \ (1 \leq i \leq r)$ chạy qua A.

(a) Chứng minh rằng nếu, với một chỉ số r, ta có $M_r = M_{r+1}$, thì suy ra $M_r = A$ (nhận thấy rằng mọi phần tử của A là một tổng các bình phương (chương VI, § 2, bài tập 7)).

(b) Giả sử rằng nhóm con S của nhóm nhân $A^*$, tạo bởi các bình phương của các phần tử của A, có chỉ số hữu hạn s trong $A^*$. Suy ra từ (a) rằng nếu $n > s$, mọi dạng toàn phương không suy biến trên E có chỉ số $> 0$ (nhận thấy rằng mọi tập hợp $M_r$ là hợp của 0 và các lớp mod. S). *Áp dụng cho trường hợp A là một trường $p$-adic $\mathbf{Q}_p$ (Tôp. đại cương, chương III, § 5, bài tập 35).*

Cho A là một trường giao hoán có đặc số $\neq 2$, E là một không gian vectơ hữu hạn chiều n trên A, Q là một dạng toàn phương không suy biến có chỉ số 0 trên E. Cho $A'$ là một mở rộng đại số của A, có bậc hữu hạn và lẻ, $E'$ là không gian vectơ trên $A'$ nhận được bằng cách mở rộng đến $A'$ trường vô hướng của E. Chứng minh rằng mở rộng $Q'$ của Q đến $E'$ ($§ 3$, no 4, mệnh đề 3) vẫn có chỉ số 0. (Rút gọn về trường hợp $A' = A[X]/(f)$, f là một đa thức bất khả quy bậc lẻ m trên A. Gọi $(e_i)$ là một cơ sở trực giao của E đối với Q, và đặt $\rho_i = Q(e_i)$; chứng minh rằng, trong $A[X]$, một quan hệ dạng $\sum_i \rho_i(g_i(X))^2 = f(X)h(X)$, trong đó các $g_i$ là các đa thức khác không không đồng thời bằng không, có bậc $\leq m - 1$, là không thể xảy ra; nhận thấy rằng vì điều này h nhất thiết phải có bậc lẻ, và xét một nhân tử bất khả quy của h, có bậc lẻ).

Cho A là một trường, E là một không gian vectơ trên A nhận một cơ sở đếm được $(e_n)_{n \geq 1}$, $\Phi$ là một dạng nửa tuyến tính Hermit không suy biến trên E, thỏa mãn điều kiện (T) ($§ 4$, no 2).

(a) Chứng minh rằng nếu các điều kiện (C) của định lý 1 không được đồng thời thỏa mãn, thì tồn tại trong E một cơ sở trực giao đối với $\Phi$ (lý luận như trong bài tập 4 của $§ 5$).

b) Giả sử thêm rằng A là giao hoán, và tồn tại một số nguyên s sao cho trên mọi không gian vectơ hữu hạn chiều có chiều $> s$ trên A, mọi dạng nửa tuyến tính Hermit không suy biến đều có chỉ số $> 0$ (xem bài tập 7). Bây giờ chứng minh rằng khi đó tồn tại trong E một cơ sở trực chuẩn đối với $\Phi$. (Lý luận như trong a), nhận thấy rằng với mọi phần tử của A có dạng $\alpha = \lambda + \overline{\lambda}$, và mọi dạng Hermit không suy biến $\Psi$ trên một không gian F có chiều $> s$, tồn tại $z \in F$ sao cho $\Psi(z, z) = \alpha$ (xem $§ 4$, no 2, mệnh đề 4).)

¶ 10) a) Cho A là một miền iđêan chính trong đó chỉ có một iđêan cực đại $A\pi$, sao cho 2 không chia hết cho $\pi$ (chương VII, § 1, bài tập 4). Cho E là một môđun tự do trên A, có chiều n. Bây giờ chứng minh rằng mọi dạng song tuyến tính đối xứng $\Phi$ trên E đều nhận một cơ sở trực giao. (Gọi r là số mũ lớn nhất sao cho $\pi^r$ chia hết mọi phần tử $\Phi(x, y)$; chứng minh rằng tồn tại $a \in E$ sao cho $\Phi(a, a) = \alpha \pi^r$, trong đó $\alpha$ khả nghịch trong A; suy ra rằng E là tổng trực tiếp của $F = Aa$ và môđun con $F^0$ trực giao với F.)

b) Cho một ví dụ (với $n = 2$) trong đó $\Phi$ không suy biến và trong đó tồn tại một môđun con không đẳng hướng F của E, có hạng 1, nhận một môđun bù trong E nhưng sao cho $F^0$ không là môđun bù của F.

c) Cho $(e_i)$ là một cơ sở trực giao của $\Phi$, và $\alpha_i = \Phi(e_i, e_i)$. Bây giờ chứng minh rằng các iđêan $A\alpha_i$ là, sai khác bởi thứ tự, độc lập với cơ sở trực giao được xét đến (xem $§ 5$, th. 1).

Các iđêan này được gọi là các nhân tử bất biến của dạng $\Phi$. Hãy cho một ví dụ về hai dạng có cùng các nhân tử bất biến và không tương đương (lấy hai dạng sao cho thương của các biệt thức không phải là một bình phương).

d) Cho $F$ là một môđun con của $E$, $\Phi_F$ là hạn chế của $\Phi$ vào $F \times F$, $A\alpha_i$ ($1 \leq i \leq r$) là các nhân tử bất biến khác không của $\Phi$, được sắp xếp sao cho $\alpha_i$ chia hết $\alpha_{i+1}$, $A\beta_i$ ($1 \leq i \leq s$) là các nhân tử bất biến khác không của $\Phi_F$, được sắp xếp sao cho $\beta_i$ chia hết $\beta_{i+1}$. Chứng minh rằng ta có $s \leq r$ và rằng $\beta_i$ là bội của $\alpha_i$ với $1 \leq i \leq s$ (cùng phương pháp như trong Bài tập 1 a) của § 5).

e) Giả sử $\Phi$ không suy biến; cho $F$, $G$ là hai môđun con không đẳng hướng của $E$ sao cho $F^0$ (tương ứng $G^0$) là môđun phụ của $F$ (tương ứng $G$). Giả sử rằng các hạn chế của $\Phi$ vào $F$ và vào $G$ là tương đương; bây giờ chứng minh rằng tồn tại một tự đẳng cấu $u$ của $E$, giữ $\Phi$ bất biến, và sao cho $u(F) = G$. (Dùng $a)$, rút gọn về trường hợp $F = Aa, G = Ab, \Phi(a, a) = \Phi(b, b)$. Cho $(c_j)$ là một cơ sở của $G^0$, và cho $b', c'_j$ ($1 \leq j \leq n-1$) là các thành phần của $b$ và $c_j$ tương ứng trong $F^0$; bây giờ chứng minh rằng tồn tại các vô hướng $\mu_j$ ($1 \leq j \leq n-1$) sao cho các phần tử $d_j = c'_j + \mu_j b'$ thỏa mãn các hệ thức $\Phi(d_j, d_k) = \Phi(c_j, c_k)$ đối với mọi cặp chỉ số; chú ý rằng với điều này, với mọi $\lambda \in A$, một trong các phần tử $1 \pm \lambda$ là khả nghịch trong $A$.

11) Cho $A$ là một miền iđêan chính có đặc số 0, trong đó chỉ có một iđêan chính $\pi$, sao cho 2 chia hết cho $\pi$. Nếu $(e_1, e_2)$ là cơ sở chính tắc của $E = A^2$, $\Phi$ là dạng song tuyến tính đối xứng trên $E$ được xác định bởi $\Phi(\xi_1 e_1 + \xi_2 e_2, \eta_1 e_1 + \eta_2 e_2) = \xi_1 \eta_2 + \xi_2 \eta_1$, bây giờ chứng minh rằng không có cơ sở trực giao nào của $E$ đối với $\Phi$.

12) Cho $A$ là trường hữu hạn $\mathbf{F}_{q^2}$, $J$ là tự đẳng cấu đối hợp $\xi \to \xi^q$ của $A$, có trường bất biến là $\mathbf{F}_q$. Nếu $E$ là một không gian vectơ có chiều $n$ trên $A$, $\Phi$ là một dạng Hermit nửa song tuyến tính không suy biến (đối với $J$) trên $E$, bây giờ chứng minh rằng cấp của nhóm unita $\mathbf{U}(\Phi)$ bằng
$$
(q^n - (-1)^n) q^{n-1}(q^{n-1} - (-1)^{n-1}) q^{n-2} \ldots (q^2 - 1) q(q + 1)
$$
(phương pháp tương tự phương pháp của Bài tập 10 của § 5, sử dụng Bài tập 3).

13) Cho $A$ là trường hữu hạn $\mathbf{F}_q$ ($q$ không là bội của 2), $E$ là một không gian vectơ có chiều $n$ trên $A$, $Q$ là một dạng toàn phương không suy biến trên $E$. Bây giờ chứng minh rằng:
a) Nếu $n$ là lẻ, cấp của nhóm $\mathbf{SO}(Q)$ là
$$
(q^{n-1} - 1) q^{n-2}(q^{n-3} - 1) q^{n-4} \ldots (q^2 - 1) q.
$$
b) Nếu $n = 2m$ là chẵn, cấp của nhóm $\mathbf{SO}(Q)$ bằng
$$
(q^{2m-1} - \varepsilon q^{m-1}) (q^{2m-2} - 1) q^{2m-3} \ldots (q^2 - 1) q
$$
trong đó $\varepsilon = 1$ nếu $(-1)^m \Delta$ là một bình phương trong $A$, $\varepsilon = -1$ trong trường hợp ngược lại, $\Delta$ là biệt thức của $Q$ đối với bất kỳ cơ sở nào của $E$. (Phương pháp tương tự phương pháp của Bài tập 12, sử dụng Bài tập 3 của $§ 6$ và Bài tập 5 của Chương V, § 11.)

14) Giả sử rằng $A$ là một trường giao hoán, $E$ là một không gian vectơ có số chiều hữu hạn $n \geqslant 2$ trên $A$, $\Phi$ là một dạng sesquilinear Hermit không suy biến trên $E$, thỏa mãn điều kiện (T) ($§ 4$, No. 2). Bây giờ chứng minh rằng các tự đồng cấu duy nhất $\omega$ của $E$ giao hoán với mọi tự đẳng cấu $u$ thuộc nhóm unita đặc biệt $\mathbf{SU}(\Phi)$ là các phép vị tự, ngoại trừ khi đồng thời có $n = 2$, $J = 1$, $A$ có đặc số $\neq 2$. (Nếu $n \geqslant 3$, viết rằng $\omega$ giao hoán với các phép đối hợp $u \in \mathbf{SU}(\Phi)$, và sử dụng Exerc. 3 của $§ 4$; nếu $n = 2$ và $J \neq 1$, viết rằng $\omega$ giao hoán với các phần tử của $\mathbf{SU}(\Phi)$ mà ma trận của chúng có dạng $\begin{pmatrix} \lambda & 0 \\ 0 & \lambda^{-1} \end{pmatrix}$ đối với một cơ sở trực giao của $E$.)

$§ 15$) Cho $A$ là một trường giao hoán có đặc số $\neq 2$, $E$ là một không gian vectơ có chiều $n \geqslant 1$ trên $A$, $Q$ là một dạng toàn phương không suy biến trên $E$. Với mọi tự đẳng cấu $u \in \mathbf{O}(Q)$, đặt $\omega = u - 1$, và đặt $r$ là hạng của $\omega$, và $W = \overline{\omega}(0)$.

a) Chứng minh rằng $\omega(E)$ là không gian con $W^0$ trực giao với $W$.

b) Chứng minh rằng nếu $n = 2, r = 2$, thì $u$ là tích của hai phép đối xứng đối với các đường của $E$. (Thiết lập rằng nếu $\omega(x)$ là đẳng hướng đối với mọi vectơ không đẳng hướng $x \in E$, thì $\omega(x)$ là đẳng hướng đối với mọi $x \in E$; xét riêng trường hợp $A$ có ít nhất 5 phần tử và trường hợp $A = \mathbf{F}_3$.)

c) Giả sử rằng $n$ và $r$ là tùy ý. Chứng minh rằng nếu $\omega(E)$ không toàn đẳng hướng, $u$ là tích của $r$ phép đối xứng đối với các siêu phẳng của $E$, và không thể là tích của một số nhỏ hơn các phép đối xứng. (Rút gọn về trường hợp $W$ là toàn đẳng hướng, và tiến hành bằng quy nạp theo $n$ và $r$. Nếu $W \neq \{0\}$, chứng minh rằng tồn tại một vectơ $a \in W^0$ sao cho $\omega(a)$ không đẳng hướng, bằng lập luận phản chứng và sử dụng sự kiện rằng một mặt phẳng mà tất cả các đường thẳng trừ nhiều nhất một đường là đẳng hướng thì nhất thiết là toàn đẳng hướng; khi đó lấy phép đối xứng $s$ đối với siêu phẳng trực giao với $\omega(a)$, và xét tự đẳng cấu $su$. Nếu $W = \{0\}$, lấy $a \in E$ sao cho $\omega(a)$ không đẳng hướng, và, với cùng ý nghĩa đối với $s$, lại xét tự đẳng cấu $su$, và sử dụng b).)

d) Giả sử rằng $\omega(E)$ là toàn đẳng hướng. Nếu $s$ là một phép đối xứng đối với một siêu phẳng không đẳng hướng $H$, chứng minh rằng không gian con của các vectơ bất biến đối với $su$ là $H \cap W$, do đó có chiều $n - r - 1$, và suy ra rằng $su$ không thể là tích của ít hơn $r + 1$ phép đối xứng đối với các siêu phẳng. Từ c) suy ra rằng $u$ là tích của $r + 2$ phép đối xứng đối với các siêu phẳng, nhưng không thể là tích của một số nhỏ hơn các phép đối xứng.

e) Suy ra từ c) và d) rằng mọi tự đẳng cấu trực giao là tích của nhiều nhất $n$ phép đối xứng đối với các siêu phẳng.

f) Chứng minh rằng nếu $n$ là lẻ (tương ứng chẵn), đối với mọi tự đẳng cấu $u \in \mathbf{O}(Q)$ có định thức 1 (tương ứng – 1), tồn tại một vectơ $x \neq 0$ bất biến đối với $u$ (sử dụng e)).

16) Các giả thiết giống như trong Bài tập 15, chứng minh rằng, nếu $n \geqslant 3$, nhóm $\mathbf{SO}(Q)$ được sinh bởi các phép đối xứng đối với các không gian con không đẳng hướng của $E$ có chiều $n - 2$ (lập luận như trong Mệnh đề 5 của No. 4).

**¶ 17) Các giả thiết giống như trong Bài tập 15.**

a) Chứng minh rằng, với $n \geqslant 2$, nhóm giao hoán tử $\Omega(Q)$ của nhóm trực giao $O(Q)$ được sinh bởi các phần tử $(st)^2$, trong đó $s$ và $t$ chạy trên tập hợp các phép đối xứng đối với các siêu phẳng (sử dụng Mệnh đề 5 của No. 4, và nhận xét rằng với mọi nhóm $\Gamma$, nhóm con được sinh bởi các bình phương của các phần tử của $\Gamma$ chứa nhóm giao hoán tử của $\Gamma$).

b) Chứng minh rằng nếu $n \geqslant 3$, nhóm giao hoán tử của $SO(Q)$ được sinh bởi các bình phương của các phần tử của $SO(Q)$ (sử dụng Bài tập 16); suy ra rằng nhóm này trùng với $\Omega(Q)$, và rằng nhóm thương $SO(Q)/\Omega(Q)$ là một nhóm giao hoán mà mọi phần tử đều có cấp 2.

c) Một mặt phẳng $P \subset E$ được gọi là *hyperbolic* nếu nó không đẳng hướng và nếu nó chứa các đường thẳng đẳng hướng (nhất thiết có số lượng là 2). Một tự đẳng cấu $u \in O(Q)$ được gọi là *hyperbolic* nếu tồn tại một mặt phẳng hyperbolic $P$ sao cho $u(x) = x$ với mọi $x \in P^0$; khi đó $u$ được gọi là một biến đổi hyperbolic liên kết với $P$. Chứng minh rằng nếu $Q$ có chỉ số $\geqslant 1$, mọi $u \in O(Q)$ là một tích của các biến đổi hyperbolic (dùng Prop. 5 của No. 4 và Exerc. 4 a) của § 4). Suy ra rằng nếu $P$ là một mặt phẳng hyperbolic, mọi $u \in O(Q)$ có thể được viết $u = t \varphi$, trong đó $t$ là một biến đổi hyperbolic liên kết với $P$ và $\varphi \in \Omega(Q)$.

**¶ 18) Cho A là một trường giao hoán, E là một không gian vectơ có chiều $n$ trên A, $\Phi$ là một dạng Hermit sesquilinear không suy biến trên E, thỏa mãn điều kiện (T) ($§ 4$, No. 2). Cho V là một không gian con vectơ của E, $H_v$ là nhóm con của nhóm đơn vị $U(\Phi)$ tạo bởi các tự đẳng cấu đơn vị $u$ sao cho $u(V) = V$.

a) Chứng minh rằng, khi V không phải là một không gian con đẳng hướng toàn phần có chiều $n/2$, ảnh của $H_v$ qua ánh xạ $u \to \det u$ là nhóm con của $A^*$ tạo bởi các $\rho \in A$ sao cho $\rho \overline{\rho} = 1$.

b) Nếu $n$ là chẵn và nếu V là một không gian con đẳng hướng toàn phần có chiều $n/2$, chứng minh rằng ảnh của $H_v$ qua ánh xạ $u \to \det u$ là nhóm con của $A^*$ tạo bởi các phần tử có dạng $\bar{\lambda}/\lambda$ (dùng Prop. 2 của $§ 4$, No. 2).

c) Cho V, W là hai không gian con vectơ của E sao cho các hạn chế của $\Phi$ lên V và W là tương đương. Chứng minh rằng tồn tại $u \in SU(\Phi)$ sao cho $u(V) = W$ trong các trường hợp sau:
  1° J khác với phần tử đơn vị (dùng Th. 3 của Chap. V, § 11, No. 5).
  2° $J = 1$, A có đặc số $\neq 2$, V và W không phải là các không gian con đẳng hướng toàn phần có chiều $n/2$.

d) Giả sử rằng $J = 1$, rằng A có đặc số $\neq 2$, rằng $n = 2m$ là chẵn, và rằng $\Phi$ là một dạng song tuyến tính đối xứng không suy biến có chỉ số $m$. Cho V, W là hai không gian con đẳng hướng toàn phần có chiều $m$ trong E; chứng minh rằng nếu $\dim(V \cap W) = q$, thì, với mọi tự đẳng cấu trực giao $u$ sao cho $u(V) = W$, ta có $\det u = (-1)^{m-q}$ (dùng b) và prop. 2 của $§ 4$, no 2). Suy ra rằng tập hợp các không gian con đẳng hướng toàn phần có chiều $m$ là hợp của hai lớp không bắc cầu $N_1, N_2$ đối với nhóm $SU(\Phi)$; nếu V và W thuộc cùng một lớp (tương ứng, thuộc các lớp khác nhau), chiều của V ∩ W có cùng tính chẵn lẻ với m (tương ứng, không có cùng tính chẵn lẻ với m). Đối với một đồng dạng u (đối với Φ) là trực tiếp, điều kiện cần và đủ là $u(N₁) = N₁$ (dùng exerc. 4 c) của § 4).

19) Cho A là một trường, E là một không gian vectơ hữu hạn chiều và > 0 trên A, Φ là một dạng Hermit ε-sesquilinear trên E, không suy biến và không phản luân phiên. Cho u là một tự đẳng cấu của E sao cho có

$$
\Phi(u(x), u(x)) = \alpha \Phi(x, x)
$$

với mọi $x \in E$, với $\alpha \in A$. Chứng minh rằng u là một phép đồng dạng có nhân tử $\alpha$ trừ khi đồng thời thỏa mãn các điều kiện sau: A giao hoán và có đặc số 2, J là đồng nhất (dùng bài tập 8 của § 1).

20) Cho A là một trường, L là một không gian Hermit hữu hạn chiều trên A; giả sử rằng dạng mêtric Φ của L thỏa mãn điều kiện (T) (§ 4, no 2). Chứng minh rằng nếu chỉ số của Φ là > 0, thì có thể có các phép đồng dạng của L, có nhân tử $\neq 1$, và không có điểm bất động nào (dùng lập luận của mệnh đề 6 của no 6, và mệnh đề 2 của § 4, no 2).

21) Cho A là một trường giao hoán có đặc số $\neq 2$, L là một không gian Euclid hữu hạn chiều trên A, Φ là dạng mêtric của L.

a) Chứng minh rằng mọi song ánh u của L lên chính nó, sao cho

$$
\Phi(u(x) - u(y), u(x) - u(y)) = \Phi(x - y, x - y)
$$

với mọi x, y trong L, là một phép dời (dùng bài tập 7 của § 1).

b) Chứng minh rằng nhóm các phép dời được sinh bởi các phép đối xứng đối với các siêu phẳng không đẳng hướng của không gian afin L (dùng mệnh đề 5 của no 4, rút gọn về việc chứng minh rằng mọi phép tịnh tiến không đẳng hướng là tích của hai phép đối xứng như vậy).

22) Trong một không gian Hermit L, hai đa tạp tuyến tính được gọi là vuông góc nếu các phương của chúng là các không gian con trực giao yếu (§ 3, bài tập 11). Giả sử L hữu hạn chiều; cho V₁, V₂ là hai đa tạp tuyến tính, W₁, W₂ là các phương tương ứng của chúng. Giả sử rằng $p = \dim(W₁ + W₂) < n$; chứng minh rằng nếu $W₁ + W₂$ không đẳng hướng, tồn tại ít nhất một đa tạp tuyến tính U có chiều $n - p$, vuông góc với V₁ và V₂, và giao với mỗi đa tạp tuyến tính V₁, V₂ tại một điểm duy nhất; hơn nữa, nếu $q = \dim(W₁ \cap W₂)$, hợp của tất cả các đa tạp tuyến tính U có các tính chất trước là một đa tạp tuyến tính có chiều $n - p + q$.

23) Cho A là một trường giao hoán có đặc số $\neq 2$, E là một không gian vectơ hữu hạn chiều có chiều $n + 1 \geq 2$ trên A, Q là một dạng toàn phương trên E, Φ là dạng song tuyến tính đối xứng liên kết với Q. Tập C gồm các $x \in E$ sao cho $Q(x) = 0$ được gọi là nón đẳng hướng với đỉnh 0 và phương trình $Q(x) = 0$. Nếu nó không thu gọn về 0, ảnh S của C – {0} trong không gian xạ ảnh $\mathbf{P}(E)$, bởi ánh xạ chính tắc $\pi$ từ $E - \{0\}$ lên $\mathbf{P}(E)$ (chương II, 2e éd., Phụ lục III), được gọi là *mặt bậc hai xạ ảnh* (tương ứng *conic xạ ảnh* nếu $n = 2$) có phương trình thuần nhất $Q(x) = 0$. Ta nói rằng S là *suy biến* nếu Q suy biến. Ta nói rằng hai đa tạp tuyến tính xạ ảnh $V_1, V_2$ của $\mathbf{P}(E)$ là *liên hợp* đối với S nếu $\overline{\pi}(V_1)$ và $\overline{\pi}(V_2)$ trực giao (đối với $\Phi$). *Cực* $V^0$ của một đa tạp tuyến tính xạ ảnh $V \subset \mathbf{P}(E)$ đối với S là đa tạp sao cho $\overline{\pi}(V^0) \cup \{0\}$ là không gian con trực giao toàn phần (đối với $\Phi$) của $\overline{\pi}(V) \cup \{0\}$; nếu V là một siêu phẳng và nếu S không suy biến, $V^0$ thu gọn về một điểm, gọi là *cực điểm* của V. Một đa tạp tuyến tính xạ ảnh V được gọi là *tiếp xúc* với S nếu $\overline{\pi}(V) \cup \{0\}$ là một không gian con đẳng hướng (đối với $\Phi$).

Giả sử trong phần tiếp theo rằng S khác rỗng và không suy biến.

a) Chứng minh rằng giao của S và một đa tạp tuyến tính xạ ảnh V là rỗng hoặc là một mặt bậc hai *trong* V; để mặt bậc hai này suy biến, điều kiện cần và đủ là V tiếp xúc với S.

b) Chứng minh rằng siêu phẳng tiếp xúc với S tại một điểm $z \in S$ là hợp của các đường thẳng đi qua z và tiếp xúc với S.

c) Giả sử $z \notin S$. Với mọi đường thẳng D đi qua z và cắt S tại hai điểm $a, b$ (phân biệt hoặc không), gọi $z'$ là *liên hợp điều hòa* của z đối với $a$ và $b$, nghĩa là điểm của D sao cho $\begin{bmatrix} a & b \\ z' & z \end{bmatrix} = -1$ (chương II, 2e éd., Phụ lục III, bài tập 4); chứng minh rằng $z'$ thuộc siêu phẳng cực của z đối với S, và rằng tồn tại n điểm trong số các điểm này tạo thành một họ tự do xạ ảnh trong $\mathbf{P}(E)$ và thuộc S (xem § 4, bài tập 4 a)).

d) Giả sử rằng $n = 3$ và rằng $\Phi$ có chỉ số cực đại $v = 2$. Tập hợp các đường thẳng chứa trong S khi đó là hợp của hai tập hợp $N_1, N_2$ sao cho mọi đường thẳng của $N_1$ cắt mọi đường thẳng của $N_2$, nhưng hai đường thẳng phân biệt của $N_1$ (tương ứng $N_2$) không cắt nhau (bài tập 18 d)). Cho D, D’ là hai đường thẳng phân biệt thuộc $N_1$; với mọi $z \in D$ tồn tại duy nhất một đường thẳng $\Delta \in N_2$ đi qua z; nếu $u(z)$ là điểm tại đó $\Delta$ cắt D’, bây giờ chứng minh rằng $u$ là một ánh xạ tuyến tính xạ ảnh từ D lên D’.

e) Vẫn giả sử $n = 3$, cho D, D’, D’’ là ba đường thẳng của $\mathbf{P}(E)$ mà bất kỳ hai đường thẳng nào cũng không cắt nhau. Bây giờ chứng minh rằng hợp của các đường thẳng cắt D, D’ và D’’ là một mặt bậc hai không suy biến.

24) Các giả thiết và ký hiệu là những thứ của bài tập 23, mặt bậc hai S được giả sử là khác rỗng và không suy biến.

a) Bây giờ chứng minh rằng nhóm con $\Gamma$ của nhóm xạ ảnh $\mathbf{PGL}(E)$ tạo bởi các song ánh tuyến tính xạ ảnh biến S thành chính nó, là ảnh chính tắc của nhóm các phép đồng dạng đối với Q. (Sử dụng bài tập 23 c) ở trên, bài tập 2 a) của § 4 và bài tập 8 của § 1.)

b) Cho $a$ là một điểm của $\mathbf{P}(E)$ không thuộc S, và cho $\Phi_1$ là hạn chế của $\Phi$ vào siêu phẳng trực giao với $\overline{\pi}(a)$ trong E. Bây giờ chứng minh rằng nhóm con của $\Gamma$ giữ $a$ bất biến là đẳng cấu với thương của nhóm trực giao $\mathbf{U}(\Phi_1)$ bởi tâm của nó.

c) Cho $b$ là một điểm của $S$, $F$ là siêu phẳng (đẳng hướng) trực giao với $\overline{\pi}(b)$ trong $E$, $M$ là một không gian phụ không đẳng hướng của $\overline{\pi}(b)$ đối với $F$, và $\Phi_2$ là hạn chế của $\Phi$ vào $M$. Bây giờ chứng minh rằng nhóm con của $\Gamma$ giữ $b$ bất biến là đẳng cấu với nhóm các phép đồng dạng của một không gian Euclid $L$ có chiều $n - 1$, có dạng mêtric là dạng nghịch đảo ($§ 1$, no 7) của $\Phi_2$. (Lưu ý rằng nếu một phép đồng dạng đối với $\Phi$ biến đường thẳng $\overline{\pi}(b)$ thành chính nó, thì nó biến $F$ thành chính nó, và được xác định hoàn toàn bởi hạn chế của nó vào $F$).

25) Cho $A$ là một trường giao hoán có đặc số $\neq 2$, $L$ là một không gian afin hữu hạn chiều có chiều $n \geqslant 2$ trên $A$. Ta đồng nhất $L$ với phần bù của một siêu phẳng xạ ảnh $H_0$ (“siêu phẳng ở vô cực”) của một không gian xạ ảnh $\mathbf{P}(E)$ có chiều $n$ (chương II, ấn bản thứ 2, Phụ lục III, No. 4). Ta nói rằng một tập hợp khác rỗng $S \subset L$ là một mặt bậc hai afin (tương ứng là đường conic afin nếu $n = 2$) nếu $S$ là giao của $L$ và một mặt bậc hai xạ ảnh (tương ứng là conic) trong $\mathbf{P}(E)$ (bài tập 23).

(a) Chứng minh rằng nếu tồn tại một quadric xạ ảnh không suy biến $\overline{S} \subset \mathbf{P}(E)$ sao cho $S = L \cap \overline{S}$, thì quadric này là duy nhất có các tính chất đó, trừ khi $n = 2$, $A = \mathbf{F}_3$ và $S$ được rút gọn thành 2 phần tử (nhận xét rằng ngoài trường hợp ngoại lệ này, với mọi điểm $z \in H_0$ không thuộc $\overline{S}$, tồn tại một đường thẳng đi qua $z$ và gặp $S$ tại hai điểm phân biệt). Khi đó ta nói rằng $S$ là một quadric afin không suy biến. Ta nói rằng hai đa tạp tuyến tính afin $V_1, V_2$ được chứa trong $L$ là liên hợp đối với $S$ nếu các đa tạp tuyến tính xạ ảnh $\overline{V}_1, \overline{V}_2$ sao cho $V_i = L \cap \overline{V}_i \ (i = 1, 2)$ là liên hợp đối với $\overline{S}$; ta định nghĩa tương tự cực (khi nó không được chứa trong $H_0$) hoặc cực điểm của một đa tạp tuyến tính afin đối với $S$, và các đa tạp tuyến tính afin tiếp xúc với $S$.

(b) Ta giả sử rằng $S$ không suy biến; chứng minh rằng có thể lấy một gốc $a$ trong $L$ sao cho, bằng cách đồng nhất $L$ theo cách này với một không gian vectơ, tồn tại một cơ sở $(e_i)$ của $L$ sao cho $S$ là tập hợp các $x = \sum_{i=1}^n \xi_i e_i$ thỏa mãn một trong hai phương trình có dạng

$$
\alpha_1 \xi_1^2 + \cdots + \alpha_n \xi_n^2 = 1 \\
\alpha_1 \xi_1^2 + \cdots + \alpha_{n-1} \xi_{n-1}^2 + \xi_n = 0.
$$

Trong trường hợp thứ nhất, điểm $a$ được xác định hoàn toàn và là cực điểm đối với $\overline{S}$ của siêu phẳng ở vô tận $H_0$ (được gọi là tâm của $S$). (Phân biệt hai trường hợp tùy theo $H_0$ có tiếp xúc hay không tiếp xúc với $\overline{S}$; dùng Định lý 1 của § 6, No. 1 và Mệnh đề 2 của § 4, No. 2.)

26) Cho $A$ là một trường giao hoán đóng đại số có đặc số $\neq 2$, $E$ là một không gian vectơ hữu hạn chiều trên $A$, $Q$ là một dạng toàn phương không suy biến trên $E$. Cho $u \in \mathbf{O}(Q)$; với ký hiệu của Bài tập 12 của § 4, ta có $G(p, p) = \{0\}$ trừ khi $p(X) = X - 1$ và $p(X) = X + 1$. Cho $M$ là một phần tử cực tiểu của tập hợp các không gian con không đẳng hướng được chứa trong $G(p, p)$ và ổn định dưới $u$, và cho $p^h$ là đa thức tối tiểu của hạn chế của $u$ lên $M$. Bây giờ chứng minh rằng nếu $h$ là lẻ, $M$ là một môđun con không phân tích được của $E_u$, và nếu $h$ là chẵn, $M$ là một tổng trực tiếp của hai môđun con không phân tích được đẳng cấu của $E_u$. (Để thấy rằng nếu $h = 2k$ là chẵn, $M$ không thể không phân tích được, hãy chỉ ra rằng $N = p^k(u)(M)$ khi đó sẽ là toàn đẳng hướng; nếu $(e_i)_{1 \leq i \leq 2k}$ là một cơ sở của $M$ sao cho $u(e_i) = \varepsilon e_i + e_{i+1}$ với $i \leq 2k - 1$, $u(e_{2k}) = \varepsilon e_{2k}$ (với $\varepsilon = \pm 1$), hãy chỉ ra rằng $e_k$ không thể trực giao với $e_{k+1}$, và suy ra rằng quan hệ $Q(u(e_k)) = Q(e_k)$ dẫn đến một mâu thuẫn).

27) Cho $A$ là một trường giao hoán có đặc số 2, $E$ là một không gian vectơ trên $A$, có số chiều hữu hạn $n$, $Q$ là một dạng toàn phương trên $E$, $\Phi$ là dạng song tuyến tính liên kết, dạng này phản xứng, do đó có hạng chẵn $2m$ ($§ 5$, no 1, hệ quả 1 của định lý 1).

a) Chứng minh rằng nếu $E^0$ là không gian con của $E$ (có chiều $n - 2m$) trực giao với $E$ đối với $\Phi$, thì ta có $Q(\lambda x + \mu y) = \lambda^2 Q(x) + \mu^2 Q(y)$ với mọi $x, y$ trong $E^0$; nói cách khác, hạn chế $Q_0$ của $Q$ trên $E^0$ là một ánh xạ nửa tuyến tính từ $E^0$ (được xem như một không gian vectơ trên $A$) vào $A$ (được xem như một không gian vectơ trên trường con $A^2$), tương ứng với đẳng cấu $\xi \to \xi^2$ của $A$ lên $A^2$. Gọi $q$ là chiều (trên $A$) của hạt nhân $E^0 \cap \overline{Q}(0)$ của $Q$, và gọi $E_1$ là một không gian con bù của $E^0 \cap \overline{Q}(0)$ đối với $E^0$; ta có $n - 2m - q \leq [A : A^2]$.

b) Suy ra từ a) rằng tồn tại một cơ sở $(e_i)_{1 \leq i \leq n}$ của $E$, trong đó $2m$ vectơ đầu tiên tạo thành một cơ sở của một không gian con bù $E_2$ của $E^0$ trong $E$, $n - 2m - q$ vectơ tiếp theo tạo thành một cơ sở của $E_1$, sao cho, với $x = \sum_{i=1}^n \xi_i e_i$

$$
Q(x) = \sum_{i=1}^m (\alpha_i \xi_i^2 + \xi_i \xi_{m+i} + \beta_i \xi_{m+i}^2) + \sum_{i=2m+1}^{n-q} \gamma_i \xi_i^2
$$

các $\gamma_i$ ($2m + 1 \leq i \leq n - q$) là các phần tử của $A$ độc lập tuyến tính đối với $A^2$.

c) Chỉ số của $Q$ được gọi là chiều cực đại của các không gian con hoàn toàn suy biến $V$ của $E$ sao cho $V \cap E^0 = \{0\}$. Chứng minh rằng nếu $v$ là chỉ số của $Q$, ta có thể lấy cơ sở $(e_i)$ của $E$ có các tính chất đã nêu trong b) sao cho $\alpha_i = \beta_i = 0$ với $1 \leq i \leq v$ và hạn chế của $Q$ trên không gian con của $E_2$ sinh bởi $e_{v+1}, \ldots, e_m, e_{m+v+1}, \ldots, e_{2m}$ là một dạng toàn phương (không suy biến) có chỉ số 0.

d) Ta giả sử $q = 0$; gọi $O(Q)$ là nhóm tự đẳng cấu của $E$ giữ bất biến $Q$. Nếu $u \in O(Q)$, bây giờ chứng minh rằng $u(x) = x$ với mọi $x \in E^0$. Với mọi $x \in E_2$, đặt $u(x) = u_0(x) + u_2(x)$, trong đó $u_0(x) \in E^0$ và $u_2(x) \in E_2$; chứng minh rằng $u_2$ thuộc nhóm symplectic $Sp(\Phi_2)$ (trong đó $\Phi_2$ là hạn chế của $\Phi$ vào $E_2$) và rằng $Q(u_2(x)) + Q(x) \in Q(E^0)$. Ngược lại, với mọi tự đẳng cấu $u_2 \in Sp(\Phi_2)$ sao cho $Q(u_2(x)) + Q(x) \in Q(E^0)$ với mọi $x \in E_2$, chứng minh rằng tồn tại duy nhất một ánh xạ tuyến tính $u_0$ của $E_2$ vào $E^0$ sao cho ánh xạ tuyến tính bằng $u_0 + u_2$ trong $E_2$, bằng đồng nhất trong $E^0$, thuộc $\mathbf{O}(Q)$.

e) Ta giả sử rằng $A$ là một trường *hoàn hảo* ($A^2 = A$) và rằng $q = 0$. Suy ra từ b) rằng mọi không gian con vectơ của $E$, có chiều $\geqslant 3$, chứa ít nhất một vectơ $x$ sao cho $Q(x) = 0$. Nếu $n$ là *lẻ*, tất yếu có $m = \nu$ và $n = 2m + 1$, do đó tồn tại một cơ sở $(e_i)$ của $E$ đối với nó ta có

$$
Q(\sum_{i=1}^n \xi_i e_i) = \xi_1 \xi_{m+1} + \cdots + \xi_m \xi_{2m} + \xi_{2m+1}^2,
$$

và (với các ký hiệu của d)) $\mathbf{O}(Q)$ là đẳng cấu với $\mathbf{Sp}(\Phi_2)$; mọi dạng toàn phương sao cho $q = 0$ khi đó là tương đương. Nếu $n$ là *chẵn*, tất yếu có $n = 2m, \nu = m$ hoặc $\nu = m - 1$, và tồn tại một cơ sở $(e_i)$ của $E$ đối với nó ta có

$$
(1) \quad Q(\sum_{i=1}^n \xi_i e_i) = \xi_1 \xi_{m+1} + \cdots + \xi_{m-1} \xi_{2m-1} + \xi_m \xi_{2m} + \lambda(\xi_m^2 + \xi_{2m}^2)
$$

trong đó $\lambda \in A$. Gọi $A_1$ là trường thu được bằng cách ghép vào $A$ các nghiệm của đa thức $\lambda X^2 + X + \lambda$; chứng minh rằng trường này độc lập với cơ sở $(e_i)$ đối với nó $Q$ có thể được viết dưới dạng (1), và rằng để hai dạng toàn phương (sao cho $q = 0$) là tương đương, điều kiện cần và đủ là các mở rộng bậc hai của $A$ tương ứng với chúng theo cách này là đồng nhất (dùng định lý Witt). Trường hợp $A$ là một trường hữu hạn có đặc số 2.

Cho $A$ là một trường giao hoán có đặc số 2, khác với $\mathbf{F}_2$, $E$ là một không gian vectơ có chiều $n = 2m$ trên $A$, $Q$ là một dạng toàn phương không suy biến trên $E$.

(a) Chứng minh rằng nhóm trực giao $\mathbf{O}(Q)$ được sinh bởi các phép đối xứng (ở đây không gì khác hơn là các phép xuyên thuộc $\mathbf{O}(Q)$ ($§ 4$, bài tập 6)) (lập luận như trong bài tập 11 của $§ 5$). Suy ra rằng nhóm giao hoán tử của $\mathbf{O}(Q)$ được sinh bởi các bình phương của các phần tử của $\mathbf{O}(Q)$ (xem bài tập 17).

(b) Giả sử rằng $Q$ có chỉ số cực đại; gọi $V, W$ là hai không gian con toàn kỳ dị của $E$ ($§ 4$, No. 1) có chiều $m$. Gọi $u$ là một phép đối xứng $x \to x + \frac{\Phi(x, a)}{Q(a)} a$ ($§ 4$, bài tập 6) ; gọi $k$ là chiều của $V \cap W$. Chứng minh rằng chiều của $V \cap u(W)$ là $k + 1$ nếu $a$ trực giao với $V \cap W, k - 1$ trong trường hợp ngược lại (trong trường hợp thứ nhất, nhận xét rằng $a = x + y$, hoặc $x \in V, y \in W$, và chứng minh rằng $u(y) = x$; trong trường hợp thứ hai, nhận xét rằng $u$ không thể giữ bất biến bất kỳ vectơ kỳ dị không trực giao nào với $a$).

(c) Một lần nữa giả sử rằng chỉ số của $Q$ là tùy ý. Chứng minh rằng nhóm con $\mathbf{SO}(Q)$ của $\mathbf{O}(Q)$, gồm các tự đẳng cấu của $E$ là tích của một số *chẵn* các phép đối xứng, là một nhóm con phân biệt có chỉ số 2 của $\mathbf{O}(Q)$. (Chứng minh rằng tích của một số lẻ các phép đối xứng không thể là đồng nhất, bằng cách xét mở rộng của $Q$ lên không gian vectơ E' thu được bởi mở rộng trường vô hướng của $E$ đến bao đóng đại số của nó; sau đó dùng b).) (Xem § 9, bài tập 9.)

(d) Nếu V₁, V₂ là hai không gian con toàn kỳ dị của E, có cùng chiều < m, chứng minh rằng tồn tại một tự đẳng cấu u ∈ SO(Q) sao cho u(V₁) = V₂. Ngược lại, nếu V₁ và V₂ là hai không gian con toàn kỳ dị có chiều m, để tồn tại một tự đẳng cấu u ∈ SO(Q) sao cho u(V₁) = V₂, điều kiện cần và đủ là chiều của V₁ ∩ V₂ có cùng tính chẵn lẻ với m (lập luận như trong bài tập 18, sử dụng b)).

(e) Một mặt phẳng P ⊂ E được gọi là hypebol nếu nó không đẳng hướng và chứa các đường thẳng kỳ dị (nhất thiết có 2 đường thẳng). Một phép biến đổi u ∈ O(Q) được gọi là hypebol nếu tồn tại một mặt phẳng hypebol P sao cho u(x) = x với mọi x ∈ P⁰ ; khi đó ta nói rằng u là một phép biến đổi hypebol liên kết với P. Chứng minh rằng nếu Q có chỉ số > 0, mọi u ∈ O(Q) là tích của các phép biến đổi hypebol (dùng a)). Suy ra rằng nếu P là một mặt phẳng hypebol, mọi phép biến đổi u ∈ O(Q) có thể viết dưới dạng u = sv, trong đó s là một phép biến đổi hypebol liên kết với P và v thuộc nhóm giao hoán tử của O(Q).

Các giả thiết là những giả thiết của bài tập 28, giả sử thêm rằng Q có chỉ số cực đại m; gọi $(eᵢ)$ là một cơ sở symplectic của E (đối với dạng phản xứng Φ liên kết với Q) được lập bởi các vectơ kỳ dị (§ 4, No. 2, Mệnh đề 2), sao cho ma trận của Φ đối với cơ sở này là ma trận được ký hiệu R trong bài tập 14 của § 5. Với các ký hiệu của bài tập cuối cùng này, chứng minh rằng, để một ma trận symplectic (tD + S)⁻¹(D + S) là ma trận của một tự đẳng cấu u ∈ O(Q), điều kiện cần và đủ là S phản xứng (viết rằng mọi vectơ u(eᵢ) đều là kỳ dị, nhận xét rằng ta có (tD + S).u(eᵢ) = (D + S).eᵢ).
