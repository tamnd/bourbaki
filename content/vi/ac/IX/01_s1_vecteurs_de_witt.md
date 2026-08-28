---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 1
section_title: Vecteurs de Witt
lang: vi
source: ac-viii-ix-fr
book_pages: AC IX.42-AC IX.68
pdf_pages: 0113-0129, 0154-0180
extraction: ocr
subsections:
    - "no": 1
      title: Polynômes de Witt
      page: 0
      pdf_page: 113
    - "no": 2
      title: Les applications $f, v$ et $\Phi$
      page: 2
      pdf_page: 114
    - "no": 3
      title: Construction de polynômes
      page: 4
      pdf_page: 116
    - "no": 4
      title: L’anneau W(A) des vecteurs de Witt
      page: 6
      pdf_page: 118
    - "no": 5
      title: L’homomorphisme F et le décalage V
      page: 7
      pdf_page: 119
    - "no": 6
      title: Filtration et topologie de l’anneau W(A)
      page: 10
      pdf_page: 122
    - "no": 7
      title: Les anneaux $W_n(A)$ des vecteurs de Witt de longueur finie
      page: 12
      pdf_page: 124
    - "no": 8
      title: L’anneau des vecteurs de Witt à coefficients dans un anneau de caractéristique $p$
      page: 15
      pdf_page: 127
statements: 29
exercises: 58
content_sha256: 5413ca4ac506da861eaea5b090db2dfdff63161310058d6c290d01d11bea8546
translated_from: content/en-mt/ac/IX/01_s1_vecteurs_de_witt.md
source_lang: en-mt
translation_method: machine
source_content_sha256: c0158ff0fca29a6c022ba154b7a5d2962e4d246ffba5dba8e9f489b8bb2152f1
translation_model: gpt-5-6-mini, gpt-5-6, gpt-5-mini
translation_run: translate-vi-7f03bb74
glossary_version: 34
glossary_terms_sha256: 3dfc7e26993a7b9a19e05ebcbde846f68ce974a46a4e6bd2cd1b8aedfd87907b
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 1. VECTƠ WITT

Trong suốt đoạn này, $p$ ký hiệu một số nguyên tố.

### 1. Các đa thức Witt

Với mọi số nguyên $n \geqslant 0$, người ta gọi đa thức Witt thứ $n$ là phần tử $\Phi_n$ của $\mathbf{Z}[X_0, ..., X_n]$ được xác định bởi

$$
\Phi_n(X_0, ..., X_n) = \sum_{i=0}^n p^i X_i^{p^{n-i}} = X_0^{p^n} + p X_1^{p^{n-1}} + \cdots + p^n X_n .
$$

Ta hiển nhiên có $\Phi_0 = X_0$ và các hệ thức truy hồi

$$
\Phi_{n+1}(X_0, ..., X_{n+1}) = \Phi_n(X_0^p, ..., X_n^p) + p^{n+1} X_{n+1}
$$
$$
\Phi_{n+1}(X_0, ..., X_{n+1}) = X_0^{p^{n+1}} + p \Phi_n(X_1, ..., X_{n+1}) .
$$

Khi gán cho $X_i$ trọng số $p^i$, đa thức $\Phi_n$ là đẳng trọng của trọng số $p^n$ (A, IV, p. 3).

#### Mệnh đề 1 {#ac-ix-s1-prop-1 .statement}

Cho A là một vành lọc và $(\mathbf{J}_n)_{n \in \mathbf{Z}}$ là phép lọc của nó. Giả sử rằng có $\mathbf{J}_0 = \mathbf{A}$ và $p.1_A \in \mathbf{J}_1$. Cho m và n là các số nguyên sao cho $m \geqslant 1$ và $n \geqslant 0$, và cho $a_0, ..., a_n, b_0, ..., b_n$ là các phần tử của A.

a) Nếu có $a_i \equiv b_i \mod \mathbf{J}_m$ với $0 \leqslant i \leqslant n$, thì có
$$
\Phi_i(a_0, ..., a_i) \equiv \Phi_i(b_0, ..., b_i) \mod \mathbf{J}_{m+i} \quad \text{cho } 0 \leqslant i \leqslant n .
$$

b) Giả sử rằng, với mọi số nguyên $k \geqslant 1$, và mọi $x \in \mathbf{A}$, quan hệ $p.x \in \mathbf{J}_{k+1}$ kéo theo $x \in \mathbf{J}_k$. Nếu có $\Phi_i(a_0, ..., a_i) \equiv \Phi_i(b_0, ..., b_i) \mod \mathbf{J}_{m+i}$ với $0 \leqslant i \leqslant n$, thì có $a_i \equiv b_i \mod \mathbf{J}_m$ với $0 \leqslant i \leqslant n$.

#### Bổ đề 1 {#ac-ix-s1-lem-1 .statement}

Nếu x và y là hai phần tử của A đồng dư modulo $\mathbf{J}_m$, ta có
$$
x^{p^n} \equiv y^{p^n} \mod \mathbf{J}_{m+n} .
$$
Bằng quy nạp theo n, ta quy về trường hợp $n = 1$. Gọi P là đa thức $\sum_{i=0}^{p-1} X^i Y^{p-1-i}$ của $\mathbf{Z}[X, Y]$. Theo giả thiết đã đặt ra đối với x và y, ta có $P(x, y) \equiv P(x, x) \equiv p.x^{p-1} \mod \mathbf{J}_m$. Khi đó có $\mathbf{J}_m + p.\mathbf{A} \subset \mathbf{J}_1$, do đó $P(x, y) \in \mathbf{J}_1$. Cuối cùng, $x^p - y^p = (x - y) P(x, y)$ thuộc về $\mathbf{J}_m \mathbf{J}_1 \subset \mathbf{J}_{m+1}$.

Ta chứng minh a) bằng quy nạp theo n. Trường hợp $n = 0$ là ngay lập tức. Giả sử $n \geqslant 1$. Theo các giả thiết của a), ta có
(4) $a_i^p \equiv b_i^p \mod \mathbf{J}_{m+1}$ với $0 \leqslant i \leqslant n-1$ theo Bổ đề 1 ,
(5) $\Phi_{n-1}(a_0^p, ..., a_{n-1}^p) \equiv \Phi_{n-1}(b_0^p, ..., b_{n-1}^p) \mod \mathbf{J}_{m+n}$
theo giả thiết quy nạp được áp dụng cho các phần tử $a_0^p, ..., a_{n-1}^p, b_0^p, ..., b_{n-1}^p$ của A, và
(6) $\Phi_n(a_0, ..., a_n) - p^n.a_n \equiv \Phi_n(b_0, ..., b_n) - p^n.b_n \mod \mathbf{J}_{m+n}$
theo các công thức (2) và (5). Vì $a_n - b_n$ thuộc về $\mathbf{J}_m$, phần tử $p^n.a_n - p^n.b_n$ thuộc về $\mathbf{J}_{m+n}$ và từ (6) suy ra đồng dư thức
$$
\Phi_n(a_0, ..., a_n) \equiv \Phi_n(b_0, ..., b_n) \mod \mathbf{J}_{m+n} ,
$$
do đó a).

Ta hãy chứng minh b) bằng quy nạp theo n. Trường hợp $n = 0$ là ngay lập tức. Giả sử $n \geqslant 1$. Theo các giả thiết của b), ta có $a_i \equiv b_i \mod \mathbf{J}_m$ với $0 \leqslant i \leqslant n-1$ theo giả thiết quy nạp, và từ đó, như trước đây, ta suy ra các đồng dư (4), (5) và (6). Nhưng theo giả thiết $\Phi_n(a_0, ..., a_n)$ và $\Phi_n(b_0, ..., b_n)$ đồng dư mod. $\mathbf{J}_{m+n}$, và do đó ta có $p^n.(a_n - b_n) \in \mathbf{J}_{m+n}$. Vì quan hệ $p.x \in \mathbf{J}_{k+1}$ kéo theo $x \in \mathbf{J}_k$ đối với mọi $x \in \mathbf{A}$ và mọi $k \geqslant 1$, ta có $a_n - b_n \in \mathbf{J}_m$, điều này hoàn tất chứng minh.

### 2. Các ánh xạ $f, v$ và $\Phi$

Cho A là một vành. Trang bị $\mathbf{A}^\mathbf{N}$ cấu trúc vành tích. Ký hiệu bởi $f_A$, hoặc đơn giản là $f$, tự đồng cấu $(a_n)_{n \in \mathbf{N}} \mapsto (a_{n+1})_{n \in \mathbf{N}}$ của $\mathbf{A}^\mathbf{N}$. Ký hiệu bởi $v_A$, hoặc đơn giản là $v$, tự đồng cấu của nhóm cộng nền của $\mathbf{A}^{\mathbf{N}}$ gán $(0, p \cdot a_0, p \cdot a_1, ...)$ với $(a_n)_{n \in \mathbf{N}}$.

Với mỗi số nguyên $m \geqslant 0$, ký hiệu bởi $\Phi_m$ ánh xạ từ $\mathbf{A}^{\mathbf{N}}$ vào $\mathbf{A}$ gán $\Phi_m(a_0, ..., a_m)$ với $a = (a_n)_{n \in \mathbf{N}}$. Ta ký hiệu bởi $\Phi_A$, hoặc đơn giản là $\Phi$, ánh xạ $a \mapsto (\Phi_n(a))_{n \in \mathbf{N}}$ từ $\mathbf{A}^{\mathbf{N}}$ vào chính nó.

#### Bổ đề 2 {#ac-ix-s1-lem-2 .statement}

Cho $\mathbf{A}$ là một vành được trang bị một tự đồng cấu $\sigma$ thỏa mãn $\sigma(a) \equiv a^p \mod. p \cdot \mathbf{A}$ đối với mọi $a \in \mathbf{A}$. Cho $n \geqslant 1$ là một số nguyên và cho $a_0, ..., a_{n-1}$ là các phần tử của $\mathbf{A}$. Đặt $u_i = \Phi_i(a_0, ..., a_i)$ với $0 \leqslant i \leqslant n - 1$. Cho $u_n$ là một phần tử của $\mathbf{A}$. Các điều kiện sau là tương đương:

a) Tồn tại $a_n \in \mathbf{A}$ sao cho $u_n = \Phi_n(a_0, ..., a_n)$.

b) Ta có $\sigma(u_{n-1}) \equiv u_n \mod. p^n \cdot \mathbf{A}$.

Với $0 \leqslant i \leqslant n - 1$, ta có $\sigma(a_i) \equiv a_i^p \mod. p \cdot \mathbf{A}$. Theo mệnh đề 1 của no. 1 được áp dụng cho trường hợp $J_k = p^k \cdot \mathbf{A}$ (với $k \in \mathbf{N}$) và $m = 1$, ta có đồng dư

$$
\Phi_{n-1}(\sigma(a_0), ..., \sigma(a_{n-1})) \equiv \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) \mod. p^n \cdot \mathbf{A},
$$

nghĩa là

$$
\sigma(u_{n-1}) \equiv \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) \mod. p^n \cdot \mathbf{A}.
$$

Bây giờ, theo công thức (2), quan hệ $u_n = \Phi_n(a_0, ..., a_n)$ tương đương với

$$
u_n = \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) + p^n \cdot a_n.
$$

Bổ đề được suy ra.

#### Mệnh đề 2 {#ac-ix-s1-prop-2 .statement}

Cho $\mathbf{A}$ là một vành.

(a) Nếu $p \cdot 1_A$ không là một ước của 0 trong $\mathbf{A}$, ánh xạ $\Phi_A$ là đơn ánh.

(b) Nếu $p \cdot 1_A$ khả nghịch trong $\mathbf{A}$, ánh xạ $\Phi_A$ là song ánh.

(c) Nếu $\sigma$ là một tự đồng cấu của vành $\mathbf{A}$, thỏa mãn $\sigma(a) \equiv a^p \mod. p \cdot \mathbf{A}$ với mọi $a \in \mathbf{A}$, ảnh $\mathbf{A}'$ của $\Phi_A$ là một vành con của $\mathbf{A}^{\mathbf{N}}$, ổn định dưới $f_A$ và $v_A$. Nó là tập hợp các phần tử $(u_n)_{n \in \mathbf{N}}$ của $\mathbf{A}^{\mathbf{N}}$ sao cho $\sigma(u_n) \equiv u_{n+1} \mod. p^{n+1} \cdot \mathbf{A}$ với mọi $n \in \mathbf{N}$.

Nếu $a = (a_n)_{n \in \mathbf{N}}$ và $u = (u_n)_{n \in \mathbf{N}}$ là các phần tử của $\mathbf{A}^{\mathbf{N}}$, quan hệ $\Phi_A(a) = u$ là tương đương, theo công thức (2), với các đẳng thức

$$
\begin{cases}
u_0 = a_0, \\
u_n = \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) + p^n \cdot a_n & \text{với mọi } n \geqslant 1.
\end{cases}
$$

Cho $u = (u_n)_{n \in \mathbf{N}}$ thuộc $\mathbf{A}^{\mathbf{N}}$. Khi $p \cdot 1_A$ không là một ước của 0 trong $\mathbf{A}$ (tương ứng. khi $p \cdot 1_A$ khả nghịch trong $\mathbf{A}$), tồn tại nhiều nhất một dãy $(a_n)_{n \in \mathbf{N}}$ trong $\mathbf{A}$ (tương ứng. đúng một dãy $(a_n)_{n \in \mathbf{N}}$ trong $\mathbf{A}$) thỏa mãn các đẳng thức (10), do đó có a) và b).

Ta chứng minh c). Theo Bổ đề 2, ảnh $\mathbf{A}'$ của $\mathbf{A}^{\mathbf{N}}$ qua $\Phi_A$ là tập hợp các $u = (u_n)_{n \in \mathbf{N}}$ trong $\mathbf{A}^{\mathbf{N}}$ sao cho $\sigma(u_n) \equiv u_{n+1} \mod. p^{n+1} \cdot \mathbf{A}$ với mọi $n \in \mathbf{N}$. Suy ra ngay lập tức rằng $\mathbf{A}'$ là một vành con của $\mathbf{A}^{\mathbf{N}}$, ổn định dưới $f_A$ và $v_A$.

#### Nhận xét {#ac-ix-s1-n2-rem-1 .statement}

Cho $a = (a_n)_{n \in \mathbf{N}}$ và $u = (u_n)_{n \in \mathbf{N}}$ là các phần tử của $A^\mathbf{N}$ sao cho $u = \Phi_A(a)$, và cho $m$ là một số nguyên $\geqslant 0$. Từ (10) suy ra các khẳng định sau:

Nếu các $u_n$, với $0 \leqslant n \leqslant m$, thuộc một vành con $B$ của $A$ và nếu, với mọi $x \in A$, quan hệ $p.x \in B$ kéo theo $x \in B$, thì các $a_n$, với $0 \leqslant n \leqslant m$, thuộc $B$.

Nếu $A$ được trang bị một phép phân bậc kiểu $\mathbf{N}$, nếu $p.1_A$ không là một ước của 0 trong $A$, nếu $d \in \mathbf{N}$ và nếu $u_n$ là thuần nhất có bậc $dp^n$ với $0 \leqslant n \leqslant m$, thì $a_n$ là thuần nhất có bậc $dp^n$ với $0 \leqslant n \leqslant m$.

### 3. Phép dựng các đa thức

Cho $A$ là vành $\mathbf{Z}[X, Y]$ các đa thức với hệ số nguyên trong hai họ các bất định $X = (X_n)_{n \in \mathbf{N}}$ và $Y = (Y_n)_{n \in \mathbf{N}}$. Cho $\theta$ là tự đồng cấu của $A$ được xác định bởi $\theta(X_n) = X_n^p$ và $\theta(Y_n) = Y_n^p$ với mọi $n \in \mathbf{N}$. Khi đó $p$ không là một ước của 0 trong $A$ và tập hợp các $a$ trong $A$ sao cho $\theta(a) \equiv a^p \mod. p.A$ là một vành con của $A$ chứa các $X_n$ và các $Y_n$, do đó bằng chính $A$.

Theo mệnh đề 2, a) và c) của số 2, tồn tại các phần tử $S = (S_n)_{n \in \mathbf{N}}, P = (P_n)_{n \in \mathbf{N}}, I = (I_n)_{n \in \mathbf{N}}$ và $F = (F_n)_{n \in \mathbf{N}}$ của $A^\mathbf{N}$ được đặc trưng tương ứng bởi các đẳng thức

$$
\left\{
\begin{array}{l}
\Phi_A(S) = \Phi_A(X) + \Phi_A(Y) \\
\Phi_A(P) = \Phi_A(X) \Phi_A(Y) \\
\Phi_A(I) = - \Phi_A(X) \\
\Phi_A(F) = f_A(\Phi_A(X))
\end{array}
\right.
$$

Các phần tử $S_n, P_n, I_n$ và $F_n$ của $A$ vì thế được đặc trưng bởi các công thức sau (trong đó $n$ chạy qua $\mathbf{N}$):

(12) $$ \Phi_n(S_0, ..., S_n) = \Phi_n(X_0, ..., X_n) + \Phi_n(Y_0, ..., Y_n), $$
(13) $$ \Phi_n(P_0, ..., P_n) = \Phi_n(X_0, ..., X_n) \Phi_n(Y_0, ..., Y_n), $$
(14) $$ \Phi_n(I_0, ..., I_n) = - \Phi_n(X_0, ..., X_n), $$
(15) $$ \Phi_n(F_0, ..., F_n) = \Phi_{n+1}(X_0, ..., X_{n+1}). $$

Gán cho $X_n$ và $Y_n$ trọng số $p^n$ với mọi $n \in \mathbf{N}$. Ta suy ra từ nhận xét của số 2 các khẳng định sau:

a) Ta có $S_n \in \mathbf{Z}[X_0, ..., X_n, Y_0, ..., Y_n]$ và $S_n$ là đẳng trọng có trọng số $p^n$.
b) Ta có $P_n \in \mathbf{Z}[X_0, ..., X_n, Y_0, ..., Y_n]$ và $P_n$ là đẳng trọng có trọng số $p^n$ trong mỗi họ $(X_0, ..., X_n)$ và $(Y_0, ..., Y_n)$.
c) Ta có $I_n \in \mathbf{Z}[X_0, ..., X_n]$ và $I_n$ là đẳng trọng có trọng số $p^n$.
d) Ta có $F_n \in \mathbf{Z}[X_0, ..., X_{n+1}]$ và $F_n$ là đẳng trọng có trọng số $p^{n+1}$.

Công thức (2) cho phép trong thực tế xác định lần lượt các đa thức $S_n, P_n, I_n$ và $F_n$.

#### Ví dụ 1 {#ac-ix-s1-n3-exa-1 .statement}

Ta có

$$
S_0 = X_0 + Y_0
$$
$$
S_1 = X_1 + Y_1 - \sum_{i=1}^{p-1} \frac{1}{p} \binom{p}{i} X_0^i Y_0^{p-i}.
$$

Hơn nữa, $S_n - X_n - Y_n$ thuộc về vành $\mathbf{Z}[X_0, ..., X_{n-1}, Y_0, ..., Y_{n-1}]$.

#### Ví dụ 2 {#ac-ix-s1-n3-exa-2 .statement}

Ta có

$$
P_0 = X_0 Y_0
$$
$$
P_1 = p X_1 Y_1 + X_0^p Y_1 + X_1 Y_0^p.
$$

#### Ví dụ 3 {#ac-ix-s1-n3-exa-3 .statement}

Khi $p \neq 2$, ta có $I_n = - X_n$. Với $p = 2$, ta có

$$
I_0 = - X_0
$$
$$
I_1 = - (X_0^2 + X_1)
$$
$$
I_2 = - X_0^4 - X_0^2 X_1 - X_1^2 - X_2.
$$

#### Ví dụ 4 {#ac-ix-s1-n3-exa-4 .statement}

Ta có

$$
F_0 = X_0^p + p X_1
$$
$$
F_1 = X_1^p + p X_2 - \sum_{i=0}^{p-1} \binom{p}{i} p^{p-i-1} X_0^{pi} X_1^{p-i}.
$$

Vì ta có $\Phi_n(F_0, ..., F_n) \equiv \Phi_n(X_0^p, ..., X_n^p) \mod. p^{n+1}$. Và với mọi $n \in \mathbf{N}$ (các công thức (2) và (15)), suy ra từ mệnh đề 1, b) rằng ta có $F_n \equiv X_n^p \mod. p$. Và với mọi $n \in \mathbf{N}$.

#### Nhận xét {#ac-ix-s1-n3-rem-1 .statement}

Cho $J$ là tập hợp các số nguyên $j \geq 1$. Với mỗi phần tử $j$ của $J$, định nghĩa đa thức $\varphi_j$ của $\mathbf{Z}[(X_j)_{j \in J}]$ bởi công thức

$$
\varphi_j = \sum_d d X_d^{j/d},
$$

trong đó tổng được lấy trên các phần tử của $J$ chia hết $j$. Với mỗi số nguyên $n \geq 0$, ta có

$$
\varphi_{p^n} = \Phi_n(X_{p^0}, ..., X_{p^n}).
$$

Với mỗi vành $A$ và mỗi phần tử $m$ của $J$, ta ký hiệu bởi $\varphi_m$ ánh xạ từ $A^J$ vào $A$ gán cho $(a_j)_{j \in J}$ phần tử $\varphi_m((a_j)_{j \in J})$; ta ký hiệu bởi $\varphi_A$, hoặc đơn giản là $\varphi$, ánh xạ từ $A^J$ vào chính nó gán cho $a = (a_j)_{j \in J}$ $(\varphi_m(a))_{m \in J}$.

Cho $\mathcal{A} = \mathbf{Z}[(X_j)_{j \in J}, (Y_j)_{j \in J}]$ là vành các đa thức với hệ số nguyên theo hai họ biến bất định $X = (X_j)_{j \in J}$ và $Y = (Y_j)_{j \in J}$. Người ta có thể chỉ ra (p. 51, bài tập 34) rằng tồn tại trong $\mathcal{A}$ các phần tử

$$
s = (s_j)_{j \in J}, \quad p = (p_j)_{j \in J} \quad \text{và} \quad i = (i_j)_{j \in J},
$$

được đặc trưng bởi các đẳng thức sau:

$$
\varphi_{\mathcal{A}}(s) = \varphi_{\mathcal{A}}(\mathbf{X}) + \varphi_{\mathcal{A}}(\mathbf{Y})
$$
$$
\varphi_{\mathcal{A}}(p) = \varphi_{\mathcal{A}}(\mathbf{X}) \varphi_{\mathcal{A}}(\mathbf{Y})
$$
$$
\varphi_{\mathcal{A}}(i) = - \varphi_{\mathcal{A}}(\mathbf{X}) .
$$

### 4. Vành W(A) của các vectơ Witt

Cho A là một vành. Nếu $a = (a_n)_{n \in \mathbf{N}}$ và $b = (b_n)_{n \in \mathbf{N}}$ là các phần tử của $A^\mathbf{N}$, ta sẽ ký hiệu bởi $S_A(a, b)$ (tương ứng $P_A(a, b)$, tương ứng $I_A(a)$) hoặc đơn giản là $S(a, b)$ (tương ứng $P(a, b)$, tương ứng $I(a)$) dãy $(S_n(a_0, ..., a_n; b_0, ..., b_n))_{n \in \mathbf{N}}$ (tương ứng $(P_n(a_0, ..., a_n; b_0, ..., b_n))_{n \in \mathbf{N}}$, tương ứng $(I_n(a_0, ..., a_n))_{n \in \mathbf{N}}$). Bằng cách thay $a_n$ cho $X_n$ và $b_n$ cho $Y_n$, với mọi $n \in \mathbf{N}$, trong các công thức (12), (13) và (14), ta thu được các đẳng thức

(16)
$$
\Phi_A(S_A(a, b)) = \Phi_A(a) + \Phi_A(b)
$$
(17)
$$
\Phi_A(P_A(a, b)) = \Phi_A(a) \Phi_A(b)
$$
(18)
$$
\Phi_A(I_A(a)) = - \Phi_A(a) .
$$

Ta sẽ ký hiệu bởi W(A) tập hợp $A^\mathbf{N}$ được trang bị các luật hợp thành $S_A$ và $P_A$.

Cho $\rho : B \to A$ là một đồng cấu vành. Ta sẽ ký hiệu bởi $\rho^\mathbf{N}$ hoặc cũng bởi W($\rho$) ánh xạ từ $B^\mathbf{N}$ vào $A^\mathbf{N}$ gán cho phần tử $b = (b_n)_{n \in \mathbf{N}}$ của $B^\mathbf{N}$ phần tử $(\rho(b_n))_{n \in \mathbf{N}}$. Từ các định nghĩa suy ra ngay lập tức rằng ta có

(19)
$$
W(\rho) \circ S_B = S_A \circ (W(\rho) \times W(\rho))
$$
(20)
$$
W(\rho) \circ P_B = P_A \circ (W(\rho) \times W(\rho))
$$
(21)
$$
W(\rho) \circ I_B = I_A \circ W(\rho)
$$
(22)
$$
\rho^\mathbf{N} \circ \Phi_B = \Phi_A \circ W(\rho) .
$$

#### Bổ đề 3 {#ac-ix-s1-lem-3 .statement}

Cho A là một vành. Tồn tại một đồng cấu toàn ánh của các vành $\rho : B \to A$, trong đó B là một vành thỏa mãn các điều kiện sau: p không là một ước của 0 trong B, và tồn tại một tự đồng cấu $\sigma$ của B sao cho $\sigma(b) \equiv b^p \mod. p.B$ với mọi $b \in B$.

Thật vậy, chỉ cần đặt $B = \mathbf{Z}[(X_a)_{a \in A}]$, lấy $\sigma$ là tự đồng cấu của B được xác định bởi $\sigma(X_a) = X_a^p$ với mọi $a \in A$, và lấy $\rho$ là đồng cấu từ B vào A được xác định bởi $\rho(X_a) = a$ với mọi $a \in A$.

#### Định lý 1 {#ac-ix-s1-thm-1 .statement}

a) Cho A là một vành (giao hoán). Được trang bị phép cộng $S_A$ và phép nhân $P_A$, W(A) là một vành (giao hoán). Phần tử đơn vị đối với phép cộng là dãy $0_A$ mà tất cả các số hạng của nó đều bằng không; phần tử đơn vị đối với phép nhân là dãy $1_A$ mà tất cả các số hạng của nó đều bằng không ngoại trừ số hạng có chỉ số 0 bằng $1_A$. Phần tử đối của một phần tử a của W(A) là $I_A(a)$.

b) Cho $\rho : B \to A$ là một đồng cấu của các vành. Khi đó $W(\rho) : W(B) \to W(A)$ là một đồng cấu của các vành.

c) Cho $A$ là một vành. Ánh xạ $\Phi_A$ là một đồng cấu của các vành từ $W(A)$ vào vành tích $A^\mathbf{N}$. Đặc biệt, với mọi $n \in \mathbf{N}$, ánh xạ $\Phi_n : a \mapsto \Phi_n(a_0, ..., a_n)$ là một đồng cấu của các vành từ $W(A)$ vào $A$.

Xét đến các công thức (16), (17), (19) và (20), chỉ cần chứng minh mệnh đề $a$.

Cho $\rho : B \to A$ là một đồng cấu của các vành thỏa mãn các điều kiện của Bổ đề 3. Gọi $B'$ là vành con của $B^\mathbf{N}$ được tạo thành bởi các phần tử $(b_n)_{n \in \mathbf{N}}$ sao cho $\sigma(b_n) \equiv b_{n+1} \mod. p^{n+1}$.B với mọi $n \in \mathbf{N}$. Theo Mệnh đề 2 của No. 2, $\Phi_B$ cảm sinh một song ánh $\Phi'_B$ từ $W(B)$ lên $B'$. Được xem như từ các công thức (16) đến (18) và các quan hệ $\Phi_n(0_B) = 0$ và $\Phi_n(1_B) = 1_B$ ($n \in \mathbf{N}$), ta thấy bằng phép chuyển cấu trúc rằng $W(B)$ là một vành, với phần tử đơn vị $0_B$ đối với phép cộng, $1_B$ đối với phép nhân, phần tử đối của $b$ là $I_B(b)$.

Ánh xạ $W(\rho) : W(B) \to W(A)$ là toàn ánh. Theo các công thức (19) và (20), quan hệ tương đương R trên $W(B)$ liên kết với ánh xạ $W(\rho)$ tương thích với cấu trúc vành của $W(B)$. Vì $W(\rho)$ cảm sinh một song ánh $\Psi$ từ vành thương $W(B)/R$ lên $W(A)$, tương thích với các luật của phép cộng và phép nhân, nên mệnh đề $a$ suy ra từ đây bằng phép chuyển cấu trúc.

#### Định nghĩa 1 {#ac-ix-s1-def-1 .statement}

Cho $A$ là một vành. Vành $W(A)$ được gọi là vành các vectơ Witt với các hệ số trong $A$.

Đối với $a$ trong $W(A)$ và $n$ trong $\mathbf{N}$, phần tử $\Phi_n(a) = \Phi_n(a_0, ..., a_n)$ đôi khi được gọi là thành phần ma của chỉ số $n$ của $a$.

#### Nhận xét {#ac-ix-s1-n4-rem-1 .statement}

Ta nhắc lại các ký hiệu của nhận xét ở No. 3. Cho $A$ là một vành. Nếu $a$ và $b$ là các phần tử của $A^J$ và $r = (r_j)_{j \in J}$ là một phần tử của $A^J$, ta ký hiệu bởi $r_A(a, b)$ phần tử $(r_j(a, b))_{j \in J}$ của $A^J$. Ta ký hiệu bởi $U(A)$ tập hợp $A^J$ được trang bị các luật hợp thành $s_A$ và $p_A$. Có thể chỉ ra (p. 52, Bài tập 35) rằng, được trang bị phép cộng $s_A$ và phép nhân $p_A$, $U(A)$ là một vành (giao hoán); nó được gọi là vành Witt phổ quát của $A$. Phần tử đơn vị đối với phép cộng là phần tử của $U(A)$ mà mọi thành phần của nó đều bằng không; phần tử đơn vị đối với phép nhân là phần tử của $U(A)$ mà mọi thành phần của nó đều bằng không ngoại trừ thành phần có chỉ số 1 bằng $1_A$; phần tử đối của một phần tử $a$ của $U(A)$ là $i_A(a)$. Ánh xạ $\varphi_A$ là một đồng cấu vành từ $U(A)$ vào vành tích $A^J$.

Cho $\rho : B \to A$ là một đồng cấu vành; ta ký hiệu bởi $U(\rho)$ ánh xạ từ $B^J$ vào $A^J$ gán cho phần tử $(b_j)_{j \in J}$ của $B^J$ phần tử $(\rho(b_j))_{j \in J}$ của $A^J$. Có thể chỉ ra (ntd.) rằng $U(\rho)$ là một đồng cấu vành từ $U(B)$ vào $U(A)$.

### 5. Đồng cấu F và phép dịch V

Cho $A$ là một vành. Trong phần tiếp theo của đoạn này, ta lần lượt ký hiệu bởi $+$ và $\times$ các luật phép cộng và phép nhân trong $W(A)$. Ta cũng sẽ viết $0$ thay cho $0_A$ và $1$ thay cho $1_A$. Ta định nghĩa $^1$ hai ánh xạ $F_A$ và $V_A$ (cũng ký hiệu đơn giản bởi $F$ và $V$) từ $W(A)$ vào chính nó bởi các công thức

$$
(23) \quad F_A(a) = (F_n(a_0, ..., a_{n+1}))_{n \in \mathbf{N}},
$$
$$
(24) \quad V_A(a) = (0, a_0, a_1, ...)
$$

(cho $a = (a_n)_{n \in \mathbf{N}}$ trong $W(A)$). Ánh xạ $V_A$ được gọi là phép dịch.

Công thức
$$
(25) \quad \Phi_n(F_0(a), ..., F_n(a)) = \Phi_{n+1}(a_0, ..., a_{n+1}) \quad (n \in \mathbf{N})
$$
suy ra ngay lập tức từ (15). Nó cũng có thể được viết dưới dạng
$$
(26) \quad \Phi_A \circ F_A = f_A \circ \Phi_A .
$$
Công thức
$$
(27) \quad \Phi_A \circ V_A = v_A \circ \Phi_A
$$
suy ra từ quan hệ (3).

Cho $\rho : B \to A$ là một đồng cấu của các vành. Các hệ thức
$$
(28) \quad W(\rho) \circ F_B = F_A \circ W(\rho)
$$
$$
(29) \quad W(\rho) \circ V_B = V_A \circ W(\rho)
$$
suy ra ngay lập tức từ các định nghĩa.

#### Mệnh đề 3 {#ac-ix-s1-prop-3 .statement}

*Cho A là một vành.*
  a) *Ánh xạ $F_A$ là một tự đồng cấu của vành $W(A)$.*
  b) *Ánh xạ $V_A$ là một tự đồng cấu của nhóm cộng nằm dưới vành $W(A)$.*
  c) *Với mọi $a$ trong $W(A)$, ta có $F_A(V_A(a)) = p.a$ (tổng trong $W(A)$ của $p$ số hạng bằng $a$).*
  d) *Cho dù $a$ và $b$ trong $W(A)$ là gì, ta đều có*
$$
(30) \quad V_A(a \times F_A(b)) = V_A(a) \times b
$$
$$
(31) \quad V_A(a) \times V_A(b) = p.V_A(a \times b)
$$
(tổng trong $W(A)$ của $p$ số hạng bằng $V_A(a \times b)$).
  e) *Đặt $\mu = V_A(1) = (0, 1, 0, ...)$. Với mọi $b$ trong $W(A)$, ta có*
$$
(32) \quad V_A(F_A(b)) = \mu \times b .
$$

$^1$ Chữ cái $F$ là chữ cái đầu của tên Frobenius, và chữ cái $V$ là chữ cái đầu của từ tiếng Đức *Verschiebung*.

f) Với mọi phần tử $a$ của $W(A)$, ký hiệu $a^{*p}$ là tích trong $W(A)$ của $p$ phần tử bằng $a$. Khi đó ta có

$$
(33) \quad F_A(a) \equiv a^{*p} \mod. p.W(A) \quad (\text{iđêan của } W(A) \text{ sinh bởi } p.\mathbf{1}) .
$$

Cho $\rho : B \to A$ là một đồng cấu của các vành thỏa mãn các điều kiện của Bổ đề 3 của No. 4. Khi đó $W(\rho) : W(B) \to W(A)$ là một đồng cấu toàn ánh của các vành, và $\Phi_B : W(B) \to B^N$ là một đơn cấu của các vành. Hơn nữa, $f_B : B^N \to B^N$ là một đồng cấu của các vành. Theo các công thức (26) và (28), ta có

$$
\Phi_B \circ F_B = f_B \circ \Phi_B, \quad W(\rho) \circ F_B = F_A \circ W(\rho),
$$

do đó ngay lập tức có mệnh đề $a$. Mệnh đề $b$ suy ra theo cách tương tự từ các công thức (27) và (29) và từ sự kiện rằng $v_B$ là một tự đồng cấu của nhóm cộng nằm dưới $B^N$.

Cho $a$ là một phần tử của $W(A)$, và chọn một phần tử $x$ của $W(B)$ mà $W(\rho)$ ánh xạ toàn ánh lên $a$. Đặt $\xi = \Phi_B(x)$. Từ các định nghĩa của $f_B$ và $v_B$, suy ra ngay lập tức rằng ta có $f_B(v_B(\xi)) = p.\xi$ (tổng trong $B^N$ của $p$ số hạng bằng $\xi$). Theo các công thức (26) và (27) (trong đó A được thay bởi B), các phần tử $F_B(V_B(x))$ và $p.x$ của $W(B)$ do đó có cùng ảnh $p.\xi$ qua ánh xạ đơn cấu $\Phi_B$, và vì thế chúng bằng nhau. Công thức $F_A(V_A(a)) = p.a$ sau đó suy ra từ các quan hệ (28) và (29). Điều này chứng minh $c$.

Lập luận theo cách tương tự, ta rút gọn chứng minh của công thức (30) về chứng minh của quan hệ

$$
v_B(\xi f_B(\eta)) = v_B(\xi) \eta
$$

đối với $\xi, \eta$ trong $B^N$. Bây giờ điều này suy ra từ các đẳng thức

$$
\xi f_B(\eta) = (\xi_0 \eta_1, \xi_1 \eta_2, ...)
$$
$$
v_B(\xi) \eta = (0, p\xi_0 \eta_1, p\xi_1 \eta_2, ...)
$$

Có tính đến $b$ và $c$, công thức (31) suy ra từ công thức (30), trong đó $b$ được thay bởi $V_A(b)$. Công thức (32) là trường hợp riêng $a = 1$ của công thức (30).

Theo cách tương tự, ta rút gọn chứng minh của công thức (33) về chứng minh của quan hệ

$$
f_B(\xi) \equiv \xi^p \mod. p.\Phi_B(B^N),
$$

trong đó $\xi^p$ chỉ tích trong $B^N$ của $p$ phần tử bằng $\xi$. Theo Mệnh đề 2, c) của No. 2, điều này tương đương với việc với mọi $n \geqslant 0$, ta có

$$
\sigma(\xi_{n+1} - \xi_n^p) \equiv \xi_{n+2} - \xi_{n+1}^p \mod. p^{n+2}B .
$$

Bây giờ, với mọi $n \geqslant 0$, theo loc. cit., ta có

$$
\sigma(\xi_n) \equiv \xi_{n+1} \mod. p^{n+1}B
$$

vì $\xi = \Phi_B(x)$; từ đó, nhờ Bổ đề 1 của No. 1, suy ra

$$
\sigma(\xi_n)^p \equiv \xi_{n+1}^p \mod. p^{n+2}\mathbf{B}.
$$

Điều này chứng minh quan hệ cần chứng minh.

#### Nhận xét {#ac-ix-s1-n5-rem-1 .statement}

Để biết định nghĩa các ánh xạ tương tự các ánh xạ F và V, trong trường hợp của vành Witt phổ quát, xem các bài tập 36, 37 và 38, p. 52 và các trang tiếp theo.

### 6. Lọc và tôpô của vành W(A)

#### Bổ đề 4 {#ac-ix-s1-lem-4 .statement}

Cho A là một vành và m $\geqslant 1$ là một số nguyên. Ta có

(34)
$$
a = (a_0, ..., a_{m-1}, 0, ...) + (\underbrace{0, ..., 0}_{m \text{ số hạng}}, a_m, a_{m+1}, ...)
$$
với mọi $a$ trong W(A).

Cho $\rho : B \to A$ là một đồng cấu vành thỏa mãn các điều kiện của Bổ đề 3 của No. 4. Khi đó $W(\rho) : W(B) \to W(A)$ là một đồng cấu toàn ánh của các vành, và $\Phi_B : W(B) \to B^N$ là một đồng cấu đơn ánh. Vì thế, chỉ cần chứng minh rằng ta có

(35)
$$
\Phi_n(b) = \Phi_n(b_0, ..., b_{m-1}, 0, ...) + \Phi_n(0, ..., 0, b_m, b_{m+1}, ...)
$$
với bất kỳ $b$ nào trong W(B) và các số nguyên $m \geqslant 1, n \geqslant 0$. Bây giờ ta có

$$
\Phi_n(b_0, ..., b_{m-1}, ...) = \Phi_n(b_0, ..., b_n) \quad \text{nếu} \quad 0 \leqslant n < m
$$
$$
= \sum_{i=0}^{m-1} p^i \cdot b_i^{p^{n-i}} \quad \text{nếu} \quad m \leqslant n
$$
$$
\Phi_n(0, ..., 0, b_m, b_{m+1}, ...) = 0 \quad \text{nếu} \quad 0 \leqslant n < m
$$
$$
= \sum_{i=m}^n p^i \cdot b_i^{p^{n-i}} \quad \text{nếu} \quad m \leqslant n,
$$
do đó công thức (35).

Cho A là một vành. Với mọi số nguyên $m \geqslant 0$, ký hiệu $V_m(A)$ là tập hợp các vectơ Witt $a = (a_n)_{n \in \mathbf{N}}$ sao cho $a_n = 0$ với $0 \leqslant n < m$. Nó là ảnh của lũy thừa thứ m $V^m$ của ánh xạ $V_A$. Các công thức

(36)
$$
V^m(a + b) = V^m(a) + V^m(b)
$$
(37)
$$
V^m(a) \times b = V^m(a \times F^m(b))
$$
suy ra từ mệnh đề 3 của No. 5 bằng quy nạp theo $m$. Chúng kéo theo rằng $V_m(A)$ là một iđêan của W(A).

Trong phần tiếp theo, ta sẽ trang bị cho $W(A)$ tôpô $\mathcal{T}$ liên kết với lọc $(V_m(A))_{m \in \mathbf{Z}}$. Vì $V_m(A)$ là một iđêan của $W(A)$ với mọi $m \in \mathbf{Z}$, tôpô $\mathcal{T}$ tương thích với cấu trúc vành của $W(A)$ (TG, III, p. 49, ví dụ 3). Cho $a \in W(A)$; các tập hợp $a + V_m(A)$, trong đó $m$ chạy qua $\mathbf{N}$, tạo thành một hệ cơ bản các lân cận của $a$ đối với $\mathcal{T}$. Bây giờ, từ bổ đề 4 suy ra rằng $a + V_m(A)$ gồm các vectơ Witt $b$ sao cho $a_i = b_i$ với $0 \leq i < m$. Do đó, $\mathcal{T}$ không gì khác ngoài tôpô tích trên $A^\mathbf{N}$ của tôpô rời rạc trên mỗi nhân tử, và vì thế $W(A)$ là một vành tôpô tách biệt và đầy đủ (TG, II, p. 17, mệnh đề 10 và TG, III, p. 22, mệnh đề 4).

Ký hiệu $\tau_A$ (hoặc đơn giản là $\tau$) là ánh xạ của $A$ vào $W(A)$ liên kết với một phần tử $a$ của $A$ phần tử $(a, 0, 0, ...)$ . Ta có $\Phi_n(\tau(a)) = a^{p^n}$ với mọi $n \in \mathbf{N}$. Với mọi đồng cấu vành $\rho : B \to A$, ta có $W(\rho) \circ \tau_B = \tau_A \circ \rho$.

#### Mệnh đề 4 {#ac-ix-s1-prop-4 .statement}

*Cho $a$ và $b$ thuộc $A$ và cho $x = (x_n)_{n \in \mathbf{N}}$ là một phần tử của $W(A)$.*

a) *Ta có các công thức*

$$
\tau(ab) = \tau(a) \times \tau(b)
$$
$$
\tau(a) \times x = (a^{p^n} x_n)_{n \in \mathbf{N}}.
$$

b) *Chuỗi có số hạng tổng quát $V^n(\tau(x_n))$ là hội tụ trong $W(A)$, với tổng là $x$.*
Cho $n$ là một số nguyên dương. Đa thức $P_n(X_0, ..., X_n; Y_0, ..., Y_n)$ được đưa vào trong No. 3 là đẳng trọng số với trọng số $p^n$ trong họ $(X_0, ..., X_n)$ khi $X_i$ được gán trọng số $p^i$. Do đó
$$
P_n(X_0, 0, ..., 0; Y_0, ..., Y_n) = X_0^{p^n} P_n(1, 0, ..., 0; Y_0, ..., Y_n).
$$
Vì $1 = (1, 0, 0, ...)$ là phần tử đơn vị của vành các vectơ Witt với các hệ số trong $\mathbf{Z}[(X_n)_{n \in \mathbf{N}}, (Y_n)_{n \in \mathbf{N}}]$, ta có
$$
P_n(1, 0, ..., 0; Y_0, ..., Y_n) = Y_n.
$$
Bằng cách thay $a$ vào chỗ $X_0$ và $x_i$ vào chỗ $Y_i$, ta suy ra từ (40) và (41) quan hệ:
$$
P_n(a, 0, ..., 0; x_0, ..., x_n) = a^{p^n} x_n.
$$
Theo định nghĩa của phép nhân trong $W(A)$, ta đã chứng minh (39); công thức (38) là một trường hợp riêng của (39).

*Ta hãy chứng minh b).* Theo định nghĩa, $V^n(\tau(x_n))$ là dãy mà tất cả các thành phần của nó đều bằng không, trừ thành phần có chỉ số $n$, thành phần này bằng $x_n$. Suy ra từ Bổ đề 4, bằng quy nạp theo $m$, rằng ta có
$$
\sum_{n=0}^m V^n(\tau(x_n)) = (x_0, ..., x_m, 0, 0, ...)
$$

với mọi số nguyên $m \geq 0$; ta suy ra b) bằng cách chuyển qua giới hạn vì tôpô $\mathcal{T}$ trên $W(A)$ là tích của các tôpô rời rạc của các thừa số $A$.

### 7. Các vành $W_n(A)$ của các vectơ Witt có độ dài hữu hạn

#### Định nghĩa 2 {#ac-ix-s1-def-2 .statement}

Cho $A$ là một vành và cho $n \geq 1$ là một số nguyên. Ta ký hiệu bởi $W_n(A)$ vành thương $W(A)/V_n(A)$.

Cho các phần tử $a_0, ..., a_{n-1}$ của $A$, ta ký hiệu bởi $[a_0, ..., a_{n-1}]$ hoặc $[a_i]_{0 \leq i < n}$ lớp modulo $V_n(A)$ của phần tử $(a_0, ..., a_{n-1}, 0, 0, ...)$ của $W(A)$. Theo Bổ đề 4 của No. 6, ánh xạ $(a_0, ..., a_{n-1}) \mapsto [a_0, ..., a_{n-1}]$ từ $A^n$ vào $W_n(A)$ là một song ánh. Vì lý do này, ta nói rằng các phần tử của $W_n(A)$ là các vectơ Witt có độ dài $n$; bằng phép tương tự, đôi khi người ta gọi các phần tử của $W(A)$ là các vectơ Witt có độ dài vô hạn.

Ta ký hiệu bởi $\pi_n$ đồng cấu chính tắc từ $W(A)$ vào $W_n(A)$. Theo Bổ đề 4 của No. 6, ta có
$$
\pi_n(a) = [a_0, ..., a_{n-1}]
$$
với mọi $a = (a_n)_{n \in \mathbf{N}}$ trong $W(A)$.

Theo định nghĩa của các phép toán trong $W(A)$, ta có mô tả sau đây về các phép toán trong $W_n(A)$:
$$
[a_0, ..., a_{n-1}] + [b_0, ..., b_{n-1}] = [S_i(a_0, ..., a_i; b_0, ..., b_i)]_{0 \leq i < n}
$$
$$
[a_0, ..., a_{n-1}] \times [b_0, ..., b_{n-1}] = [P_i(a_0, ..., a_i; b_0, ..., b_i)]_{0 \leq i < n}
$$
$$
- [a_0, ..., a_{n-1}] = [I_i(a_0, ..., a_i)]_{0 \leq i < n}.
$$

Hơn nữa, phần tử đơn vị của phép cộng trong $W_n(A)$ là $[0, ..., 0]$ và phần tử đơn vị của phép nhân là $[1, 0, ..., 0]$.

Cho $i$ là một số nguyên sao cho $0 \leq i \leq n$. Bằng cách chuyển qua thương, đồng cấu $\Phi_i$ từ $W(A)$ vào $A$ xác định một đồng cấu $\Phi_i$ từ $W_n(A)$ vào $A$. Điều này gắn với vectơ Witt $[a_0, ..., a_{n-1}]$ phần tử $\Phi_i(a_0, ..., a_i)$ của $A$ (còn được gọi là thành phần ma có chỉ số $i$ của $[a_0, ..., a_{n-1}]$).

Cho $\rho : B \to A$ là một đồng cấu vành. Bằng cách chuyển qua các thương, đồng cấu $W(\rho)$ từ $W(B)$ vào $W(A)$ xác định một đồng cấu $W_n(\rho)$ từ $W_n(B)$ vào $W_n(A)$. Nó được mô tả bởi công thức
$$
W_n(\rho)[b_0, ..., b_{n-1}] = [\rho(b_0), ..., \rho(b_{n-1})]
$$
với mọi $[b_0, ..., b_{n-1}]$ trong $W_n(B)$.

Cho $m$ và $n$ là hai số nguyên sao cho $1 \leq n \leq m$. Ta có $V_n(A) \supset V_m(A)$, do đó một đồng cấu chính tắc từ $W_m(A) = W(A)/V_m(A)$ lên $W_n(A) = W(A)/V_n(A)$; đồng cấu này sẽ được ký hiệu là $\pi_{n,m}$. Tường minh, ta có
$$
\pi_{n,m}[a_0, ..., a_{m-1}] = [a_0, ..., a_{n-1}]
$$

với $[a_0, ..., a_{m-1}]$ trong $W_m(A)$. Họ $(W_n(A), \pi_{n,m})$ là một hệ xạ ảnh các vành và ánh xạ $\pi : a \mapsto (\pi_n(a))_{n \geq 1}$ là một đồng cấu vành từ $W(A)$ vào $\lim_{\leftarrow} W_n(A)$, được gọi là chính tắc. Vì $W(A)$ là tách được và đầy đủ đối với lọc $(V_n(A))_{n \in \mathbf{Z}}$ (*cf.* No. 6), đồng cấu chính tắc $\pi$ là một đẳng cấu của các vành tôpô, khi $W_n(A)$ được trang bị tôpô rời rạc với mọi số nguyên $n \geq 1$ (III, § 2, No. 6).

Kể từ nay, các đồng cấu $\pi_n$ và $\pi_{n,m}$ sẽ được gọi là *các đồng cấu phép chiếu* từ $W(A)$ vào $W_n(A)$, và từ $W_m(A)$ vào $W_n(A)$ tương ứng.

#### Ví dụ 1 {#ac-ix-s1-n7-exa-1 .statement}

Đồng cấu $\Phi_0 : W_1(A) \to A$ là một đẳng cấu.

#### Ví dụ 2 {#ac-ix-s1-n7-exa-2 .statement}

Ta hãy mô tả tường minh các phép toán trong $W_2(A)$. Ta có

$$
[a_0, a_1] + [b_0, b_1] = \left[ a_0 + b_0, a_1 + b_1 - \sum_{i=1}^{p-1} \frac{1}{p} \binom{p}{i} a_0^i b_0^{p-i} \right]
$$

$$
[a_0, a_1] \times [b_0, b_1] = [a_0 b_0, a_0^p b_1 + a_1 b_0^p + p \cdot a_1 b_1]
$$

với $[a_0, a_1]$ và $[b_0, b_1]$ trong $W_2(A)$. Các thành phần ma của $[a_0, a_1]$ là $a_0$ và $a_0^p + p \cdot a_1$.

#### Ví dụ 3 {#ac-ix-s1-n7-exa-3 .statement}

Cho $n \geq 1$ là một số nguyên. Nếu $a_0, ..., a_{n-1}, b_0, ..., b_{n-1}$ là các số nguyên sao cho $a_i \equiv b_i \bmod p$ với $0 \leq i < n$, ta có (No. 1, Mệnh đề 1)

$$
\Phi_{n-1}(a_0, ..., a_{n-1}) \equiv \Phi_{n-1}(b_0, ..., b_{n-1}) \bmod p^n.
$$

Do đó, $\Phi_{n-1}$ xác định qua phép chuyển qua các thương một đồng cấu vành $\varphi_n : W_n(\mathbf{Z}/p\mathbf{Z}) \to \mathbf{Z}/p^n\mathbf{Z}$. Ảnh của $\varphi_n$ là một nhóm con của $\mathbf{Z}/p^n\mathbf{Z}$ chứa 1, do đó $\varphi_n$ là toàn ánh. Vì các tập hợp hữu hạn $W_n(\mathbf{Z}/p\mathbf{Z})$ và $\mathbf{Z}/p^n\mathbf{Z}$ có cùng lực lượng $p^n$, $\varphi_n$ là một đẳng cấu.

Cho $m$ và $n$ là các số nguyên sao cho $1 \leq n \leq m$. Tồn tại một đồng cấu vành duy nhất $\alpha_{n,m} : \mathbf{Z}/p^m\mathbf{Z} \to \mathbf{Z}/p^n\mathbf{Z}$; do đó biểu đồ

$$
\begin{array}{ccc}
\mathbf{Z}/p^m\mathbf{Z} & \xrightarrow{\alpha_{n,m}} & \mathbf{Z}/p^n\mathbf{Z} \\
\varphi_m \uparrow & & \varphi_n \uparrow \\
W_m(\mathbf{Z}/p\mathbf{Z}) & \xrightarrow{\pi_{n,m}} & W_n(\mathbf{Z}/p\mathbf{Z})
\end{array}
$$

là giao hoán. Suy ra rằng $\varphi = \lim \varphi_n$ là một đẳng cấu của các vành tôpô từ $W(\mathbf{Z}/p\mathbf{Z}) = \lim_{\leftarrow} W_n(\mathbf{Z}/p\mathbf{Z})$ lên $\mathbf{Z}_p = \lim_{\leftarrow} \mathbf{Z}/p^n\mathbf{Z}$ (III, § 2, No. 12, ví dụ 3).

Cho $m$ và $n$ là hai số nguyên $\geq 1$. Theo phép dựng, ta có một dãy khớp của các nhóm cộng

(E)
$$
0 \longrightarrow W(A) \xrightarrow{\nu^m} W(A) \xrightarrow{\pi_m} W_m(A) \longrightarrow 0.
$$

Qua phép chuyển qua các thương, tự đồng cấu $V^n$ của nhóm cộng của $W(A)$ xác định một đồng cấu $V^n_m$ của nhóm cộng của $W_m(A)$ vào nhóm cộng của $W_{m+n}(A)$. Nói cách khác, ta có một biểu đồ giao hoán

$$
\begin{array}{ccc}
W(A) & \xrightarrow{V^n} & W(A) \\
\pi_m \downarrow & & \pi_{n+m} \downarrow \\
W_m(A) & \xrightarrow{V^n_m} & W_{n+m}(A)
\end{array}
$$

Qua phép chuyển qua các thương, từ dãy khớp (E) ta suy ra một dãy khớp

(E') $$ 0 \longrightarrow W_m(A) \xrightarrow{V^n_m} W_{n+m}(A) \xrightarrow{\pi_{n,n+m}} W_n(A) \longrightarrow 0 . $$

Ta có

(45) $$ V^n_m[a_0, ..., a_{m-1}] = [\underbrace{0, ..., 0}_{n \text{ lần}}, a_0, ..., a_{m-1}], $$

với mọi phần tử $[a_0, ..., a_{m-1}]$ của $W_m(A)$.

Theo Mệnh đề 3, c) của No. 5, ta có $FV^{m+1}(a) = p.V^m(a)$ với mọi $a$ trong $W(A)$ và do đó ta có $F(V_{m+1}(A)) \subset V_m(A)$. Bằng quy nạp theo $n$, ta suy ra rằng $F^n$ biến $V_{n+m}(A)$ vào $V_m(A)$, và vì thế xác định, qua phép chuyển qua các thương, một đồng cấu vành $F^n_m : W_{n+m}(A) \to W_m(A)$. Theo phép dựng, ta có một biểu đồ giao hoán

$$
\begin{array}{ccc}
W(A) & \xrightarrow{F^n} & W(A) \\
\pi_{n+m} \downarrow & & \pi_m \downarrow \\
W_{n+m}(A) & \xrightarrow{F^n_m} & W_m(A)
\end{array}
$$

Nhắc lại (No. 3) rằng đa thức $F_i$ thuộc về $\mathbf{Z}[X_0, ..., X_{i+1}]$ với mọi số nguyên $i \geqslant 0$; đồng cấu $F^1_m$ từ $W_{m+1}(A)$ vào $W_m(A)$ do đó được cho tường minh như sau:

(46) $$ F^1_m[a_0, ..., a_m] = [F_i(a_0, ..., a_{i+1})]_{0 \leqslant i < m}. $$

Cho $a \in W_m(A)$, $a' \in W_m(A)$ và $b \in W_{m+1}(A)$. Các công thức sau thu được bằng phép chuyển qua các thương từ Mệnh đề 3 của No. 5:

(47) $$ F^1_m(V^1_m(a)) = p.a $$
(48) $$ V^1_m(a \times F^1_m(b)) = V^1_m(a) \times b $$
(49) $$ V^1_m(a) \times V^1_m(a') = p.V^1_m(a \times a') $$
(50) $$ V^1_m(F^1_m(b)) = \mu_{m+1} \times b $$

(với $\mu_{m+1} = [0, 1, 0, ..., 0]$).

### 8. Vành các vectơ Witt với hệ số trong một vành có đặc số $p$

#### Mệnh đề 5 {#ac-ix-s1-prop-5 .statement}

Cho $A$ là một vành có đặc số $p$ (A, V, p. 2). Với mọi phần tử $a$ và $b$ của $W(A)$, và các số nguyên dương $m, n$, ta có, nếu $a = (a_n)_{n \in \mathbf{N}}$,

$$
(51) \quad F(a) = (a_n^p)_{n \in \mathbf{N}}
$$
$$
(52) \quad p.a = VF(a) = FV(a) = (0, a_0^p, a_1^p, ...)
$$
$$
(53) \quad V^m(a) \times V^n(b) = V^{m+n}(F^n(a) \times F^m(b)) .
$$

Công thức (51) suy ra từ Ví dụ 4 của No. 3. Từ đó ngay lập tức suy ra đẳng thức

$$
VF(a) = FV(a) = (0, a_0^p, a_1^p, ...) ,
$$

và đẳng thức $p.a = FV(a)$ đã được chứng minh (No. 5, mệnh đề 3), do đó có (52).

Ta hãy chứng minh (53). Theo công thức (37) (trong đó thay $V^n(b)$ cho $b$), ta có

$$
(54) \quad V^m(a) \times V^n(b) = V^m(a \times F^m(V^n(b))) .
$$

Từ công thức (37), ta cũng suy ra

$$
(55) \quad V^n(F^m(b)) \times a = V^n(F^m(b) \times F^n(a)) .
$$

Công thức (53) khi đó suy ra từ (54) và (55) và từ quan hệ $F^m \circ V^n = V^n \circ F^m$, bản thân nó là một hệ quả của (51).

#### Hệ quả {#ac-ix-s1-n8-cor-1 .statement}

Nếu $m$ và $n$ là hai số nguyên dương, ta có

$$
V_m(A) \times V_n(A) \subset V_{m+n}(A) .
$$

Điều này suy ra từ công thức (53), vì $V_m(A)$ là ảnh của $V^m : W(A) \to W(A)$.

#### Mệnh đề 6 {#ac-ix-s1-prop-6 .statement}

Cho $A$ là một vành.

a) Với mọi số nguyên $k \geqslant 1$, ta có $(V_1(A))^k = p^{k-1} \cdot V_1(A)$.

b) Giả sử rằng $A$ là một vành có đặc số $p$. Trên vành $W(A)$, tôpô $V_1(A)$-adic và tôpô $p$-adic trùng nhau, và chúng mịn hơn tôpô tích $\mathcal{C}$ (xem No. 6). Vành $W(A)$ là tách được và đầy đủ đối với tôpô $p$-adic.

Ta hãy chứng minh a) bằng quy nạp theo $k$. Trường hợp $k = 1$ là hiển nhiên. Giả sử $k \geqslant 2$. Theo giả thiết quy nạp, ta có $V_1(A)^{k-1} = p^{k-2} \cdot V_1(A)$ và do đó $V_1(A)^k = p^{k-2} \cdot (V_1(A))^2$. Nhưng từ mệnh đề 3, d), công thức (31), của No. 5 suy ra rằng ta có $(V_1(A))^2 = p \cdot V_1(A)$, do đó có a).

Bây giờ giả sử rằng $A$ có đặc số $p$. Vì ta có

$$
p \cdot W(A) = VF(W(A)) \subset V_1(A) \quad (\text{công thức (52)}) ,
$$

ta suy ra từ a) các bao hàm $p^k.W(A) \subset (V_1(A))^k \subset p^{k-1}.W(A)$, và từ hệ quả của mệnh đề 5 bao hàm $(V_1(A))^k \subset V_k(A)$, với mọi số nguyên $k \geqslant 1$. Khẳng định thứ nhất của b) được suy ra.

Cho $k$ là một số nguyên $\geqslant 1$. Theo công thức (52), iđêan $p^k.W(A)$ của $W(A)$ là tập hợp các phần tử $a = (a_n)_{n \in \mathbf{N}}$ của $W(A)$ sao cho có $a_n = 0$ với $n < k$ và $a_n \in A^{p^k}$ với $n \geqslant k$. Do đó nó là đóng đối với tôpô $\mathcal{G}$. Vì $W(A)$ là tách được và đầy đủ đối với tôpô $\mathcal{G}$ (no 6) và vì các iđêan $p^k.W(A)$ của $W(A)$, với $k \geqslant 1$, tạo thành một cơ sở các lân cận của $0$ trong $W(A)$ đối với tôpô $p$-adic, nên vành $W(A)$ là tách được và đầy đủ đối với tôpô $p$-adic (TG, III, p. 26, hệ quả 1 của mệnh đề 10).

#### Mệnh đề 7 {#ac-ix-s1-prop-7 .statement}

*Cho A là một vành hoàn hảo có đặc số p.*

a) *Với mọi phần tử $a = (a_n)_{n \in \mathbf{N}}$ của $W(A)$, chuỗi có số hạng tổng quát $p^n \tau(a_n^{p^{-n}})$ là hội tụ trong $W(A)$, với tổng là $a$.*

b) *Trên $W(A)$, tôpô $V_1(A)$-adic, tôpô $p$-adic và tôpô $\mathcal{G}$ trùng nhau. Chính xác hơn, ta có $V_n(A) = p^n.W(A) = (V_1(A))^n$ với mọi số nguyên $n \geqslant 0$. Đặc biệt $\Phi_0$ xác định một đẳng cấu của $W(A)/p.W(A)$ lên $A$.*

Theo định nghĩa (A, V, p. 5), ánh xạ $a \mapsto a^p$ là một tự đẳng cấu của vành $A$. Theo mệnh đề 5, F do đó là một tự đẳng cấu của vành $W(A)$, và ta có, với mọi $n \in \mathbf{N}$,

$$
p^n.W(A) = V^n F^n(W(A)) = V^n(W(A)) = V_n(A).
$$

Đặc biệt, ta có $(V_1(A))^n = (p.W(A))^n = p^n.W(A)$. Mệnh đề b) suy ra từ đó.

Theo mệnh đề 5, ta có

$$
p^n.\tau(a_n^{p^{-n}}) = V^n F^n \tau(a_n^{p^{-n}}) = V^n \tau(a_n),
$$

và mệnh đề a) suy ra từ mệnh đề 4 của no 6.

#### Mệnh đề 8 {#ac-ix-s1-prop-8 .statement}

*Cho A là một trường có đặc số p. Vành $W(A)$ là một vành địa phương nguyên, tách được và đầy đủ, với iđêan cực đại $V_1(A)$ và trường thặng dư đẳng cấu với A. Nếu trường A là hoàn hảo, vành $W(A)$ là một vành định giá rời rạc, và iđêan cực đại của nó là $p.W(A)$.*

Đồng cấu $\Phi_0$ xác định một đẳng cấu của $W(A)/V_1(A)$ lên $A$ (no 7, ví dụ 1). Iđêan $V_1(A)$ của $W(A)$ do đó là cực đại. Vì vành $W(A)$ là tách được và đầy đủ đối với tôpô $V_1(A)$-adic (mệnh đề 6, $b$), nó là một vành địa phương, với iđêan cực đại $V_1(A)$ (III, § 2, no 13, mệnh đề 19).

Cho $a$ và $b$ là hai phần tử khác không của $W(A)$. Tồn tại các số nguyên $m \geqslant 0$ và $n \geqslant 0$, và các phần tử $a' = (a'_n)_{n \in \mathbf{N}}$ và $b' = (b'_n)_{n \in \mathbf{N}}$ của $W(A)$ sao cho $a = V^m(a')$, $b = V^n(b')$ và các phần tử $a'_0$ và $b'_0$ của $A$ là khác không. Khi đó thành phần có chỉ số $m + n$ của $a \times b$ bằng thành phần có chỉ số 0 của $F^n(a') \times F^m(b')$ (công thức (53)), nghĩa là bằng ${a'_0}^{p^n} {b'_0}^{p^m}$ (công thức (51) và No. 3, Ví dụ 2). Do đó $a \times b$ là khác không và $W(A)$ là một miền nguyên.

Nếu trường $A$ là hoàn hảo, iđêan cực đại $V_1(A)$ của $W(A)$ bằng $p.W(A)$ (Prop. 7, b)) và do đó W(A) là một vành định giá rời rạc (VI, § 3, No. 6, Prop. 9, c)).

#### Nhận xét 1 {#ac-ix-s1-n8-rem-1 .statement}

Cho A là một trường có đặc số p. Bây giờ có thể chứng minh rằng vành W(A) là Noether khi và chỉ khi A là hoàn hảo (p. 43, Bài tập 9).

#### Nhận xét 2 {#ac-ix-s1-n8-rem-2 .statement}

Cho A là một vành có đặc số p. Theo Prop. 5, ta có các công thức

$$
F_m^n[a_0, ..., a_{n+m-1}] = [a_0^{p^n}, ..., a_{m-1}^{p^n}]
$$
$$
p^n.[a_0, ..., a_{n+m-1}] = [\underbrace{0, ..., 0}_{n \text{ lần}}, a_0^{p^n}, ..., a_{m-1}^{p^n}]
$$

với mọi vectơ Witt $[a_0, ..., a_{n+m-1}]$ có độ dài $n + m$.

Thực vậy, ánh xạ $F : W(A) \to W(A)$ cho phép, bằng cách chuyển qua các thương bởi $V_m(A)$, định nghĩa một ánh xạ $\overline{F}_m : W_m(A) \to W_m(A)$. Ta có công thức

$$
\overline{F}_m[a_0, ..., a_{m-1}] = [a_0^p, ..., a_{m-1}^p].
$$

Các ánh xạ $V_m^1 \circ \overline{F}_m$ và $\overline{F}_{m+1} \circ V_m^1$ từ $W_m(A)$ vào $W_{m+1}(A)$ là bằng nhau và thu được, bằng cách chuyển qua thương, từ phép nhân với $p$ trong $W_{m+1}(A)$.

## BÀI TẬP {#ac-ix-s1-exercises}

Trong các Bài tập 1 đến 27, $p$ là một số nguyên tố cố định. Nếu $A$ là một vành, vành các vectơ Witt $W(A)$ là vành gắn với số nguyên tố $p$.
