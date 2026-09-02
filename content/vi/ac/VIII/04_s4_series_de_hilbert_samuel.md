---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 4
section_title: Séries de Hilbert-Samuel
lang: vi
source: ac-viii-ix-fr
book_pages: AC VIII.87-AC VIII.94
pdf_pages: 0041-0055, 0091-0098
extraction: ocr
subsections:
    - "no": 1
      title: L’anneau $\mathbf{Z}((T))$
      page: 0
      pdf_page: 41
    - "no": 2
      title: Série de Poincaré d’un module gradué sur un anneau de polynômes
      page: 39
      pdf_page: 43
    - "no": 3
      title: Série de Hilbert-Samuel d’un module bien filtré
      page: 43
      pdf_page: 47
    - "no": 4
      title: Degré de la fonction de Hilbert-Samuel
      page: 47
      pdf_page: 51
    - "no": 5
      title: Série de Hilbert-Samuel d’un module quotient
      page: 48
      pdf_page: 52
statements: 34
exercises: 12
content_sha256: 743db54e2b37b9488a060735e6da0b10ef05bbc2aa2793684daac441c43a3c21
translated_from: content/en-mt/ac/VIII/04_s4_series_de_hilbert_samuel.md
source_lang: en-mt
translation_method: machine
source_content_sha256: ae265f1a7682a184312fd25a18260a14a79b7cfae6b49715feaf4e96f8913054
translation_model: gpt-5.4
translation_run: translate-vi-7779bf41
glossary_version: 34
glossary_terms_sha256: 741c317d8d18eaa7d33119d49ffb17f6f7a4085a2caaf64cbd831da508a156be
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CHUỖI HILBERT-SAMUEL

### 1. Vành $\mathbf{Z}((T))$

Cho A là một vành. Trang bị cho A-môđun $A^\mathbf{Z}$ tôpô tích của các tôpô rời rạc. Các phần tử $(a_n) \in A^\mathbf{Z}$ sao cho tồn tại $n_0 \in \mathbf{Z}$ với $a_n = 0$ đối với $n < n_0$ tạo thành một môđun con B của $A^\mathbf{Z}$. Nếu với $a = (a_n) \in B, b \in (b_n) \in B$, đặt $ab = c$, với $c_n = \sum_{i+j=n} a_i b_j$, thì ta xác định trên B một cấu trúc đại số trên A. Gọi T là phần tử $(\theta_n)$ của B sao cho $\theta_n = 0$ đối với $n \neq 1$ và $\theta_1 = 1$. Khi đó T khả nghịch trong B; với mọi phần tử $a = (a_n)$ của B, họ $(a_n T^n)_{n \in \mathbf{Z}}$ là khả tổng trong $A^\mathbf{Z}$ và ta có

$$
a = \sum_{n \in \mathbf{Z}} a_n T^n .
$$

Trong phần sau của chương này, đại số trên A $B$ sẽ được ký hiệu là $A((T))$; nó chứa như các đại số con đại số $A[[T]]$ của các chuỗi hình thức và đại số $A[T, T^{-1}]$; giao của chúng là đại số $A[T]$ của các đa thức.

#### Nhận xét {#ac-viii-s4-n1-rem-1 .statement}

Vành $A((T))$ được đồng nhất một cách tự nhiên với vành phân thức $A[[T]]_T$ của vành $A[[T]]$ được xác định bởi tập hợp nhân tạo bởi các lũy thừa của $T$.

Với $n, p$ trong $\mathbf{Z}$, số tự nhiên $\left[ \begin{array}{c} n \\ p \end{array} \right]$ được xác định bởi

$$
\left( \begin{array}{ll}
\left[ \begin{array}{c} n \\ p \end{array} \right] = 0 & \text{nếu } p < 0 \text{ hoặc } p > n, \\
\left[ \begin{array}{c} n \\ p \end{array} \right] = \binom{n}{p} = \frac{n(n-1)...(n-p+1)}{p!} & \text{nếu } 0 \leq p \leq n .
\end{array} \right.
$$

Ta có $\left[ \begin{array}{c} n \\ p \end{array} \right] = \left[ \begin{array}{c} n \\ n-p \end{array} \right]$ với $n, p \in \mathbf{Z}$.

#### Bổ đề 1 {#ac-viii-s4-lem-1 .statement}

*Phần tử $1 - T$ của $\mathbf{Z}((T))$ là khả nghịch. Với mọi số nguyên $r > 0$ ta có*

$$
(1 - T)^{-r} = \sum_{n \in \mathbf{Z}} \left[ \begin{array}{c} n + r - 1 \\ r - 1 \end{array} \right] T^n = \sum_{n \in \mathbf{N}} \binom{n + r - 1}{r - 1} T^n .
$$

Thật vậy, $1 - T$ là khả nghịch trong vành $\mathbf{Z}[[T]]$, với nghịch đảo là $\sum_{m \geq 0} T^m$; do đó ta có

$$
(1 - T)^{-r} = (\sum_{m \geq 0} T^m)^r = \sum_{m_1, ..., m_r \geq 0} T^{m_1 + m_2 + ... + m_r},
$$

và công thức đã nêu suy ra từ E, III, p. 44, prop. 15.

Cho $Q(T) \in \mathbf{Z}[T, T^{-1}]$, cho $r$ là một số nguyên $> 0$, và cho $F = (1 - T)^{-r} Q \in \mathbf{Z}((T))$. Đặt

$$
Q(T) = \sum_{i \in \mathbf{Z}} a_i T^i , \quad F = \sum_{n \in \mathbf{Z}} \alpha_n T^n .
$$

Khi đó, theo bổ đề 1, ta có

$$
\alpha_n = \sum_{i \in \mathbf{Z}} a_i \left[ \begin{array}{c} n - i + r - 1 \\ r - 1 \end{array} \right] = \sum_{i \leq n} a_i \binom{n - i + r - 1}{r - 1}.
$$

Gọi $n_1$ là cận trên bé nhất trong $\overline{\mathbf{R}}$ của tập hợp các số nguyên $i \in \mathbf{Z}$ sao cho $a_i \neq 0$. Với mọi số nguyên $n \geq n_1$, ta có $\alpha_n = \tilde{\alpha}(n)$, trong đó $\tilde{\alpha}$ là đa thức của $\mathbf{Q}[X]$ được xác định bởi

$$
\tilde{\alpha}(X) = \frac{1}{(r-1)!} \sum_{i \in \mathbf{Z}} a_i \prod_{j=1}^{r-1} (X - i + j) .
$$

Nếu đặt $c = Q(1) = \sum_{i \in \mathbf{Z}} a_i$, ta có $\tilde{\alpha}(X) = c X^{r-1}/(r-1)! + \theta(X)$, trong đó $\theta$ là một đa thức bậc $\leq r-2$. Do đó, ta có

$$
\alpha_n = c \frac{n^{r-1}}{(r-1)!} + \rho_n n^{r-2},
$$

trong đó số hữu tỉ $\rho_n$ tiến tới một giới hạn khi $n$ tăng vô hạn. Do đó suy ra quan hệ

$$
Q(1) = (r-1)! \lim_{n \to \infty} n^{1-r} \alpha_n.
$$

Nếu $F = \sum_{n \in \mathbf{Z}} a_n T^n$ và $G = \sum_{n \in \mathbf{Z}} b_n T^n$ là hai phần tử của $\mathbf{Z}((T))$, người ta ký hiệu bởi “ $F \leq G$ ” quan hệ “ $a_n \leq b_n$ với mọi $n \in \mathbf{Z}$ ”. Đây là một quan hệ thứ tự tương thích với cấu trúc vành của $\mathbf{Z}((T))$ (A, VI, p. 18, Định nghĩa 1). Ta có $(1-T)^{-1} \geq 1$. Nếu $Q \in \mathbf{Z}[T, T^{-1}]$ là $\geq 0$, thì số nguyên $Q(1)$ là dương.

**Bổ đề 2. — a)** Cho $F$ là một phần tử khác không của $\mathbf{Z}((T))$ sao cho tồn tại $r \in \mathbf{Z}$, với $(1-T)^r F \in \mathbf{Z}[T, T^{-1}]$; khi đó $F$ có thể được viết duy nhất dưới dạng $F = (1-T)^{-d}.Q$, trong đó $Q \in \mathbf{Z}[T, T^{-1}]$, $Q(1) \neq 0$ và $d \in \mathbf{Z}$. Nếu $F \geq 0$, thì ta có $Q(1) > 0$ và $d \geq 0$.

b) Cho $Q, R$ thuộc $\mathbf{Z}[T, T^{-1}]$, $d, d'$ thuộc $\mathbf{Z}$ với $Q(1) > 0$. Nếu

$$
(1-T)^{-d}.Q \leq (1-T)^{-d'}.R,
$$

thì hoặc $d < d'$, hoặc $d = d'$ và $Q(1) \leq R(1)$.

a) Ta có thể viết $F = (1-T)^{-r} T^n P(T)$ với $r, n \in \mathbf{Z}$ và $P(T) \in \mathbf{Z}[T]$. Bằng phép chia Euclid, ta có thể viết $P(T) = (1-T)^p R(T)$ với $R(T) \in \mathbf{Z}[T]$ và $R(1) \neq 0$. Do đó $F = (1-T)^{-(r-p)} Q(T)$, trong đó $Q(T) = T^n R(T) \in \mathbf{Z}[T, T^{-1}]$ và $Q(1) \neq 0$. Điều này chứng minh sự tồn tại của $d$ và $Q$. Hơn nữa, nếu $(1-T)^r Q(T) = (1-T)^s R(T)$ với $r > s$ và $Q, R$ trong $\mathbf{Z}[T, T^{-1}]$, thì ta có $R(T) = (1-T)^{r-s} Q(T)$, do đó $R(1) = 0$; điều này chứng minh tính duy nhất. Giả sử rằng $F$ là $\geq 0$; nếu ta có $d < 0$, thì ta sẽ có $F(1) = 0$, điều này là không thể vì $F$ khác không và mọi hệ số của nó đều dương; vậy ta có $d \geq 0$. Nếu $d = 0$, thì $Q = F \geq 0$, do đó $Q(1)$ là dương. Nếu $d \geq 1$, thì $Q(1)$ là dương theo công thức (3). Điều này chứng minh a).

b) Giả sử $d \geq d'$. Khi đó $(1-T)^{-d} ((1-T)^{d-d'} R - Q) \geq 0$; vì $S(T) = (1-T)^{d-d'} R - Q$ thuộc $\mathbf{Z}[T, T^{-1}]$, điều này suy ra $S(1) \geq 0$ theo điều vừa đi trước. Nếu $d > d'$, ta có $S(1) = -Q(1) < 0$, do đó có mâu thuẫn; nếu $d = d'$, ta có $S(1) = R(1) - Q(1)$, do đó $Q(1) \leq R(1)$.

### 2. Chuỗi Poincaré của một môđun phân bậc trên một vành đa thức

Cho $H_0$ là một vành, $I$ một tập hợp hữu hạn và $H$ là vành đa thức $H_0[(X_i)_{i \in I}]$. Với mỗi $i \in I$, cho $d_i$ là một số nguyên $> 0$. Trang bị cho $H$ cấu trúc vành phân bậc kiểu $\mathbf{Z}$ sao cho các phần tử của $H_0$ là thuần nhất bậc 0 và mỗi $X_i$ thuần nhất bậc $d_i$. Khi $d_i = 1$ với mọi $i$, ta thu được phân bậc thông thường của các vành đa thức.

Cho $M$ là một $H$-môđun phân bậc kiểu *sinh hữu hạn* mà các thành phần thuần nhất của nó đều là các $H_0$-môđun có độ dài hữu hạn; *chuỗi Poincaré* của $M$ theo định nghĩa là phần tử $P_M$ của $\mathbf{Z}((T))$ sao cho $P_M = \sum_{n \in \mathbf{Z}} \operatorname{long}_{H_0}(M_n) \cdot T^n$, và ta đặt $Q_M = P_M \cdot \prod_{i \in I} (1 - T^{d_i})$.

#### Định lý 1 {#ac-viii-s4-thm-1 .statement}

*Phần tử $Q_M$ của $\mathbf{Z}((T))$ thuộc $\mathbf{Z}[T, T^{-1}]$*.

Chia $H_0$ cho linh hóa tử của $H_0$-môđun $M$, ta quy về trường hợp $M$ là một $H_0$-môđun trung thành. Nếu $a, b \in \mathbf{Z}$ sao cho $M$ được sinh như một $H$-môđun bởi $M' = \sum_{a \leq i \leq b} M_i$, thì $M'$ là một $H_0$-môđun trung thành có độ dài hữu hạn; do đó vành $H_0$ là Artin (A, VIII, § 1, No. 3), vì thế Noether (*loc. cit.*, § 9, No. 1). Do đó vành đa thức $H$ là Noether (*loc. cit.*, § 1, No. 4). Nếu $I$ rỗng, thì $H = H_0$, và họ các số nguyên $(\operatorname{long}_{H_0}(M_n))_{n \in \mathbf{Z}}$ có giá hữu hạn, vì $M$ là một $H_0$-môđun hữu hạn sinh; do đó định lý đúng trong trường hợp này. Bây giờ ta lập luận bằng quy nạp theo lực lượng của tập hợp $I$, được giả sử là khác rỗng; lấy $j \in I$ và đặt $J = I - \{j\}$. Ký hiệu $H'$ là vành con phân bậc của $H$ được sinh bởi $H_0$ và các $X_i$ với $i$ thuộc $J$; xét phép vị tự $(X_j)_M$ trong $M$ với tỉ số $X_j$, hạt nhân $R$ của nó, và đối hạt nhân $S$ của nó. Với mỗi $n \in \mathbf{Z}$ có một dãy khớp các $H_0$-môđun

$$
0 \to R_{n-d_j} \to M_{n-d_j} \to M_n \to S_n \to 0 ,
$$

do đó $R_{n-d_j}$ và $S_n$ có độ dài hữu hạn, và ta có

$$
\operatorname{long}_{H_0}(M_n) - \operatorname{long}_{H_0}(M_{n-d_j}) = \operatorname{long}_{H_0}(S_n) - \operatorname{long}_{H_0}(R_{n-d_j}) .
$$

Vì $M$ là một môđun hữu hạn sinh trên vành Noether $H$, các $H$-môđun $R$ và $S$ là hữu hạn sinh; vì chúng bị triệt tiêu bởi $X_j$, chúng là các $H'$-môđun hữu hạn sinh. Theo giả thiết quy nạp, các phần tử $P_R \cdot \prod_{i \in J} (1 - T^{d_i})$ và $P_S \cdot \prod_{i \in J} (1 - T^{d_i})$ của $\mathbf{Z}((T))$ do đó thuộc $\mathbf{Z}[T, T^{-1}]$; từ (4), suy ra

$$
P_M - T^{d_j} \cdot P_M = P_S - T^{d_j} \cdot P_R ,
$$

nghĩa là, $(1 - T^{d_j}) \cdot P_M = P_S - T^{d_j} \cdot P_R$; vì thế

$$
P_M \cdot \prod_{i \in I} (1 - T^{d_i}) = P_S \cdot \prod_{i \in J} (1 - T^{d_i}) - T^{d_j} \cdot P_R \cdot \prod_{i \in J} (1 - T^{d_i}) ,
$$

do đó có kết luận.

#### Ví dụ 1 {#ac-viii-s4-n2-exa-1 .statement}

Giả sử $H_0$ là Artin và lấy $M = H$. Khi đó, với các ký hiệu trước đây, ta có $R = 0$ và $S = H'$, do đó theo (5), $Q_H = Q_{H'}$; vì ta có $Q_{H_0} = \operatorname{long}(H_0)$, suy ra bằng quy nạp rằng $Q_H = \operatorname{long}(H_0)$, nghĩa là,

$$
P_H = \operatorname{long}(H_0) \cdot \prod_{i \in I} (1 - T^{d_i})^{-1} .
$$

Bây giờ giả sử H được trang bị phân bậc thông thường, trong đó $d_i = 1$ với mọi $i \in I$, và đặt $r = \mathrm{Card}(I)$; ta có $P_M = Q_M(T).(1 - T)^{-r}$. Đặt $c_M = Q_M(1)$. Khi đó, theo công thức (2) của No. 1, ta có:

#### Hệ quả {#ac-viii-s4-n2-cor-1 .statement}

a) Nếu $r = 0$, thì ta có $\mathrm{long}_{H_0}(M) = c_M$.

b) Nếu $r = 1$, thì ta có $\mathrm{long}_{H_0}(M_n) = c_M$ với $n$ đủ lớn.

c) Nếu $r > 1$, thì ta có $\mathrm{long}_{H_0}(M_n) = c_M \frac{n^{r-1}}{(r-1)!} + \rho_n n^{r-2}$, trong đó $\rho_n$ tiến tới một giới hạn trong $\mathbf{R}$ khi $n$ tăng vô hạn.

#### Nhận xét 1 {#ac-viii-s4-n2-rem-1 .statement}

Số nguyên $c_M$ là dương theo bổ đề 2. Có thể có $M \neq 0$ và $c_M = 0$ (x. mệnh đề 2).

#### Nhận xét 2 {#ac-viii-s4-n2-rem-2 .statement}

Cho $0 \to M' \to M \to M'' \to 0$ là một dãy khớp các H-môđun phân bậc và các đồng cấu bậc 0 sao cho M là kiểu hữu hạn trên H và $M_n$ có độ dài hữu hạn trên $H_0$ với mỗi $n$. Khi đó, với mỗi $n \in \mathbf{Z}$, ta có
$$
\mathrm{long}_{H_0}(M_n) = \mathrm{long}_{H_0}(M'_n) + \mathrm{long}_{H_0}(M''_n),
$$
do đó $P_M = P_{M'} + P_{M''}$, $Q_M = Q_{M'} + Q_{M''}$ và $c_M = c_{M'} + c_{M''}$.

#### Nhận xét 3 {#ac-viii-s4-n2-rem-3 .statement}

Cho $M(p)$ là môđun suy ra từ M bằng cách tịnh tiến phân bậc đi $p$ (A, II, p. 165, ví dụ 3). Vì ta có $M(p)_n = M_{p+n}$, nên ta có $P_{M(p)} = T^{-p}P_M$, $Q_{M(p)} = T^{-p}Q_M$ và $c_{M(p)} = c_M$.

#### Ví dụ 2 {#ac-viii-s4-n2-exa-2 .statement}

Giả sử $H_0$ là Artin, và cho M là một H-môđun phân bậc tự do được sinh bởi s phần tử thuần nhất, độc lập tuyến tính, có các bậc tương ứng $\delta_1, ..., \delta_s$. Khi đó M đẳng cấu với $H(-\delta_1) \oplus \cdots \oplus H(-\delta_s)$. Do các nhận xét 2 và 3 và ví dụ 1, vì vậy ta có
$$
P_M = \mathrm{long}(H_0)\left( \sum_{i=1}^s T^{\delta_i} \right)(1 - T)^{-r},
$$
$$
Q_M = \mathrm{long}(H_0)\left( \sum_{i=1}^s T^{\delta_i} \right),
$$
$$
c_M = s.\mathrm{long}(H_0).
$$

#### Ví dụ 3 {#ac-viii-s4-n2-exa-3 .statement}

Lại giả sử $H_0$ là Artin; cho M là một H-môđun phân bậc, và giả sử rằng tồn tại một dãy khớp các H-môđun phân bậc và các đồng cấu bậc 0
$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to M \to 0,
$$
trong đó, với $k = 0, 1, ..., n$, $L_k$ là một H-môđun phân bậc tự do được sinh bởi các phần tử thuần nhất độc lập tuyến tính, có các bậc tương ứng $\delta_{k,1}, ..., \delta_{k,m(k)}$. Khi đó, theo nhận xét 2 và ví dụ 2, ta có
$$
Q_M = \mathrm{long}(H_0).\sum_{0 \leq k \leq n} \sum_{1 \leq j \leq m(k)} (-1)^k T^{\delta_{k,j}},
$$
$$
c_M = \mathrm{long}(H_0).\sum_{0 \leq k \leq n} (-1)^k m(k).
$$

#### Nhận xét 4 {#ac-viii-s4-n2-rem-4 .statement}

Có thể chứng minh (p. 88, bài tập 4) rằng dưới các giả thiết của đ. lý 1, các $H_0$-môđun $\mathrm{Tor}_j^H(H_0, M)$ có độ dài hữu hạn, bằng không với $j > r$, và ta có
$$
c_M = \sum_{j=0}^r (-1)^j \mathrm{long}_{H_0}(\mathrm{Tor}_j^H(H_0, M)).
$$
Chính xác hơn, các $H$-môđun $T_j = \mathrm{Tor}_j^H(H_0, M)$ được trang bị một cách tự nhiên các phân bậc và ta có
$$
Q_M = \sum_{j=0}^r (-1)^j P_{T_j}.
$$

#### Mệnh đề 1 {#ac-viii-s4-prop-1 .statement}

Cho $M$ là một $H$-môđun phân bậc. Giả sử rằng $M$ được sinh bởi $M_0$ và $M_0$ là một $H_0$-môđun có độ dài hữu hạn. Khi đó ta có
$$
P_M \leq (1 - T)^{-r} \mathrm{long}_{H_0}(M_0), \quad c_M \leq \mathrm{long}_{H_0}(M_0).
$$
Hơn nữa, các điều kiện sau là tương đương:
(i) $c_M = \mathrm{long}_{H_0}(M_0)$;
(ii) $P_M = \mathrm{long}_{H_0}(M_0) \cdot (1 - T)^{-r}$, nghĩa là $M = M_0$ nếu $r = 0$ và
$$
\mathrm{long}_{H_0}(M_n) = \mathrm{long}_{H_0}(M_0) \binom{n + r - 1}{r - 1}
$$
với $n \in \mathbf{N}$ nếu $r > 0$;
(iii) đồng cấu chính tắc của các $H$-môđun
$$
\varphi : H \otimes_{H_0} M_0 \to M
$$
là song ánh.

Kí hiệu $R$ là hạt nhân của $\varphi$. Vì $\varphi$ là toàn ánh, ta có
$$
P_M = P_{H \otimes M_0} - P_R = \mathrm{long}_{H_0}(M_0) (1 - T)^{-r} - P_R \quad \text{and} \quad c_M = \mathrm{long}_{H_0}(M_0) - c_R.
$$
Các điều kiện (i), (ii) và (iii) lần lượt tương đương với $c_R = 0$, $P_R = 0$ và $R = 0$.
Do đó ta có (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i), và chỉ cần chứng minh rằng $c_R = 0$ suy ra $R = 0$. Giả sử $R \neq 0$ và cho $0 = N^h \subset N^{h-1} \subset ... \subset N^0 = M_0$ là một dãy Jordan-Hölder của $H_0$-môđun $M_0$. Gọi $R^m$ là giao của $R$ với ảnh của $H \otimes_{H_0} N^m$ trong $H \otimes_{H_0} M_0$; tồn tại một số nguyên $m$ giữa 1 và $h$ sao cho $R^m \neq R^{m-1}$. Đặt $L = R^{m-1}/R^m$; ta có $0 \leq c_L \leq c_R$ và chỉ cần chứng minh rằng $c_L \neq 0$. Bây giờ, nếu $k$ là trường thương của $H_0$ theo iđêan linh hóa tử cực đại của $N^{m-1}/N^m$, thì $L$ được đồng nhất với một môđun con phân bậc khác không của $k[(X_i)_{i \in I}]$. Do đó $L$ chứa một môđun con đẳng cấu với một môđun tịnh tiến của $k[(X_i)_{i \in I}]$; vì $c_{k[(X_i)_{i \in I}]} = 1$, suy ra $c_L \geq 1$ (Nhận xét 2 và 3), điều phải chứng minh.

#### Nhận xét 5 {#ac-viii-s4-n2-rem-5 .statement}

Theo A, X, p. 160, đ. lý 1, điều kiện (iii) có nghĩa là $(X_1, ..., X_r)$ là một dãy hoàn toàn cát tuyến đối với $H$-môđun $M$.

#### Mệnh đề 2 {#ac-viii-s4-prop-2 .statement}

Giả sử $H_0$ là một trường, và cho $M$ là một $H$-môđun phân bậc sinh hữu hạn. Gọi $K$ là trường phân thức của $H$. Khi đó $c_M$ bằng hạng của $H$-môđun $M$, nghĩa là bằng chiều của không gian vectơ $M \otimes_H K$ trên $K$.

Điều này là hiển nhiên nếu $M = H$, vì $c_H = 1$. Mặt khác, cho $x \in H$ thuần nhất bậc $d$, và khác không; ta có $(H/xH) \otimes_H K = 0$; từ dãy khớp
$$
0 \to H(-d) \to H \to H/xH \to 0,
$$
và các nhận xét 2 và 3, suy ra $c_{H/xH} = 0$. Do đó mệnh đề được kiểm chứng khi $M$ được sinh bởi một phần tử thuần nhất. Trường hợp tổng quát suy ra từ đây, vì mọi $H$-môđun phân bậc sinh hữu hạn đều có một chuỗi hợp thành mà các thương của nó có dạng trên.

#### Nhận xét 6 {#ac-viii-s4-n2-rem-6 .statement}

Do đó, dưới các giả thiết của Mệnh đề 2, ta có $c_M = 0$ khi và chỉ khi $M$ là một $H$-môđun xoắn, hay cũng tương đương khi $\dim_H(M) < r$ (§ 1, No. 5, ví dụ 4).

### 3. Chuỗi Hilbert-Samuel của một môđun được lọc tốt

Trong phần còn lại của số này, ta sẽ dùng ký hiệu sau: nếu $G \in \mathbf{Z}((T))$ và nếu $r \in \mathbf{N}$, ta đặt $G^{(r)} = (1 - T)^{-r}G$; đặc biệt, nếu $G = \sum_{n \in \mathbf{Z}} a_n T^n$, thì
$$
G^{(1)} = \sum_{n \in \mathbf{Z}} \left( \sum_{i \leq n} a_i \right) T^n.
$$
Nếu $G \geq 0$, thì ta có $G^{(r)} \geq 0$ với mọi $r \in \mathbf{N}$.

Cho $A$ là một vành Noether, $q$ một iđêan của $A$ và $M$ một $A$-môđun sinh hữu hạn. Nhắc lại (III, § 3, No. 1, Def. 1) rằng một lọc $q$-tốt trên $M$ là một ánh xạ $F : n \mapsto F_n$ từ $\mathbf{Z}$ vào tập hợp các môđun con của $M$ thỏa mãn ba điều kiện sau:
a) ta có $qF_n \subset F_{n+1} \subset F_n$ với mọi $n \in \mathbf{Z}$,
b) tồn tại $n_0 \in \mathbf{Z}$ sao cho $qF_n = F_{n+1}$ với $n \geq n_0$,
c) tồn tại $n_1 \in \mathbf{Z}$ sao cho $F_{n_1} = M$.
Nếu $n_0$ và $n_1$ thỏa mãn các điều kiện trên, thì với mọi $n \in \mathbf{Z}$, ta có
$$
q^{n-n_1}M \subset F_n \subset q^{n-n_0}M
$$
(nhớ rằng theo quy ước ta đã đặt $q^r = A$ với $r \leq 0$).

#### Bổ đề 3 {#ac-viii-s4-lem-3 .statement}

Nếu $F$ và $F'$ là hai lọc $q$-tốt trên $M$, thì tồn tại một số nguyên $m$ sao cho $F'_n \subset F_{n-m}$ với mọi $n \in \mathbf{Z}$.
Thật vậy, tồn tại $n_2$ sao cho $F'_n \subset q^{n-n_2}M$ với mọi $n$, do đó $F'_n \subset F_{n-(n_2-n_1)}$ với mọi $n$.

#### Bổ đề 4 {#ac-viii-s4-lem-4 .statement}

Cho $F$ là một lọc $q$-tốt trên $M$. Nếu $M/qM$ có độ dài hữu hạn, thì $M/F_{n+1}$ và $F_n/F_{n+1}$ có độ dài hữu hạn với mọi $n \in \mathbf{Z}$.
Với ký hiệu của (7), ta có $\operatorname{long}(M/F_{n+1}) \leq \operatorname{long}(M/q^{n-n_1+1}M)$ và chỉ cần chứng minh rằng $q^nM/q^{n+1}M$ có độ dài hữu hạn với mọi $n$. Do đó ta được quy về trường hợp của lọc $q$-adic. Cho $(x_1, ..., x_r)$ là một hệ sinh hữu hạn của $A$-môđun $q$, và gọi $I$ là tập hợp hữu hạn các đơn thức có tổng bậc bằng $n$ theo $r$ biến

X_1, ..., X_r. Đồng cấu từ (M/qM)^l vào q^nM/q^{n+1}M biến họ (u_m)_{m\in I} thành phần tử $\sum m(x_1, ..., x_r)\ u_m$ là toàn ánh. Vì M/qM có độ dài hữu hạn, q^nM/q^{n+1}M cũng vậy.

Từ đây về sau giả sử M/qM có độ dài hữu hạn. Cho F là một lọc q-tốt trên M. Tồn tại $n_1 \in \mathbf{Z}$ sao cho $F_{n_1} = M$, do đó $F_n = M$ với $n \leq n_1$; vì thế ta định nghĩa một phần tử $H_{M,F}$ của $\mathbf{Z}((T))$ bằng cách đặt

(8)
$$
H_{M,F} = \sum_{n \in \mathbf{Z}} \operatorname{long}_{A/q}(F_n/F_{n+1}). T^n \in \mathbf{Z}((T)).
$$

#### Định nghĩa 1 {#ac-viii-s4-def-1 .statement}

Chuỗi $H_{M,F}$ được gọi là chuỗi Hilbert-Samuel của A-môđun M (đối với lọc q-tốt F).

Ánh xạ $n \mapsto \operatorname{long}_A(F_n/F_{n+1})$ thường được gọi là hàm Hilbert-Samuel của M (đối với F).

Điều này áp dụng đặc biệt cho trường hợp của lọc q-adic ($F_n = q^nM$); khi đó ta đặt $H_{M,F} = H_{M,q}$. Do đó ta có

(9)
$$
H_{M,q} = \sum_{n \in \mathbf{Z}} \operatorname{long}_{A/q}(q^nM/q^{n+1}M). T^n .
$$

#### Mệnh đề 3 {#ac-viii-s4-prop-3 .statement}

a) Nếu F là một lọc q-tốt trên M, ta có

(10)
$$
H_{M,F}^{(1)} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(M/F_{n+1}). T^n .
$$

b) Nếu F và F’ là hai lọc q-tốt trên M, thì tồn tại một số nguyên m sao cho $H_{M,F'}^{(1)} \geq T^m H_{M,F}^{(1)}$.

Phần a) suy ra ngay lập tức từ định nghĩa của $H_{M,F}^{(1)}$; phần b) suy ra từ a) và Bổ đề 3.

#### Định lý 2 {#ac-viii-s4-thm-2 .statement}

Cho A là một vành Noether, q là một iđêan của A, M là một A-môđun hữu hạn sinh sao cho M/qM khác không và có độ dài hữu hạn, và F là một lọc q-tốt trên M.

a) Tồn tại một số nguyên d $\geq 0$, và một phần tử R của $\mathbf{Z}[T, T^{-1}]$, được xác định duy nhất, sao cho $R(1) > 0$ và $H_{M,F} = (1 - T)^{-d}R$.

b) Các số nguyên d và R(1) độc lập với lọc q-tốt F đã chọn.

a) Xét vành phân bậc gr(A) sao cho $\operatorname{gr}_n(A) = q^n/q^{n+1}$ và gr(A)-môđun phân bậc gr(M) sao cho $\operatorname{gr}_n(M) = F_n/F_{n+1}$. Vì ta có $F_{n_1} = M$ và $qF_n = F_{n+1}$ với $n \geq n_0$, gr(M) được sinh bởi $\bigoplus_{n_1 \leq n \leq n_0} \operatorname{gr}_n(M)$, nên là sinh hữu hạn. Hơn nữa, nếu $(x_1, ..., x_r)$ là một hệ sinh hữu hạn của q như A-môđun, thì gr(A) được sinh bởi $\operatorname{gr}_0(A)$ và các lớp của $x_i$ modulo $q^2$, do đó đẳng cấu với một vành phân bậc thương của $H = (A/q)[X_1, ..., X_r]$. Theo Định lý 1 của No. 2, ta có
$$
(1 - T)^r H_{M,F} \in \mathbf{Z}[T, T^{-1}] .
$$
Ta có $H_{M,F} \neq 0$ và bởi vậy tồn tại $d \in \mathbf{N}$ và $R \in \mathbf{Z}[T, T^{-1}]$, được xác định duy nhất, sao cho $R(1) > 0$ và $H_{M,F} = (1 - T)^{-d}.R$ (Bổ đề 2 của No. 1).

b) Gọi $F'$ là một q-bộ lọc tốt khác và viết tương tự
$$
H_{M,F'} = (1 - T)^{-d'} R'.
$$
Theo Mệnh đề 3, b), tồn tại một số nguyên $m$ sao cho $(1 - T)^{-d' - 1} R' \geq T^m (1 - T)^{-d - 1} R$.
Theo Bổ đề 2, b) của No. 1, điều này suy ra $d' \geq d$ và, nếu $d' = d$, thì $R'(1) \geq R(1)$.
Đổi vai trò của $F$ và $F'$, ta được $d = d'$ và $R(1) = R'(1)$.

#### Nhận xét 1 {#ac-viii-s4-n3-rem-1 .statement}

Với ký hiệu của a), viết $R = \sum_{i \in \mathbf{Z}} a_i T^i$, và giả sử $d > 0$.
Theo No. 1, quan hệ $H_{M,F} = (1 - T)^{-d} R$ cũng có thể viết thành
$$
\text{(11)} \quad \operatorname{long}_A(F_n/F_{n+1}) = \sum_{i \in \mathbf{Z}} a_i \binom{n - i + d - 1}{d - 1} = \sum_{i \leq n} a_i \binom{n - i + d - 1}{d - 1}.
$$
Tương tự, vì $H^{(1)}_{M,F} = (1 - T)^{-d - 1} R$, ta có
$$
\text{(12)} \quad \operatorname{long}_A(M/F_{n+1}) = \sum_{i \in \mathbf{Z}} a_i \binom{n - i + d}{d} = \sum_{i \leq n} a_i \binom{n - i + d}{d}.
$$

Cho $A$ là một vành Noether, $q$ là một iđêan của $A$, $M$ là một $A$-môđun sinh hữu hạn sao cho $M/qM$ có độ dài hữu hạn. Nếu $M \neq qM$, theo Định lý 2, b) tồn tại các số nguyên $d_q(M) \geq 0$ và $e_q(M) > 0$ sao cho, với mọi q-bộ lọc tốt $F$ trên $M$, tồn tại $R \in \mathbf{Z}[T, T^{-1}]$ với
$$
H_{M,F} = (1 - T)^{-d_q(M)} R , \quad R(1) = e_q(M) .
$$
Nếu $M = qM$, theo quy ước ta đặt $d_q(M) = -\infty$, $e_q(M) = 0$.

#### Nhận xét 2 {#ac-viii-s4-n3-rem-2 .statement}

Nói rằng $M/qM$ có độ dài hữu hạn nghĩa là
$$
\operatorname{Supp}(M/qM) = \operatorname{Supp}(M) \cap V(q)
$$
gồm các iđêan cực đại (IV, § 2, No. 5, Mệnh đề 7). Ta sẽ thấy dưới đây (No. 4, hệ quả của Định lý 3) rằng $d_q(M)$ là cận trên bé nhất của các số $\dim_{A_m}(M_m)$, trong đó $m$ chạy qua tập hợp $\operatorname{Supp}(M) \cap V(q)$.

#### Hệ quả {#ac-viii-s4-n3-cor-1 .statement}

*Cho $A$ là một vành Noether, $q$ là một iđêan của $A$, $M$ là một $A$-môđun hữu hạn sinh sao cho $M/qM$ có độ dài hữu hạn, và $F$ là một filtration q-tốt trên $M$.
a) Để có $d_q(M) \leq 0$, điều kiện cần và đủ là dãy $(q^n M)$ dừng, hay cũng thế, dãy $(F_n)$ dừng. Khi đó, với mọi $n$ đủ lớn,
$$
\operatorname{long}(M/F_{n+1}) = \operatorname{long}(M/q^{n+1}M) = e_q(M) .
$$
b) Giả sử rằng ta có $d_q(M) > 0$. Khi đó ta có
$$
\text{(13)} \quad \operatorname{long}_A(F_n/F_{n+1}) = e_q(M) n^{d_q(M) - 1}/(d_q(M) - 1)! + \rho_n n^{d_q(M) - 2},
$$
$$
\text{(14)} \quad \operatorname{long}_A(M/F_{n+1}) = e_q(M) n^{d_q(M)}/d_q(M)! + \sigma_n n^{d_q(M) - 1},
$$
trong đó $\rho_n$ và $\sigma_n$ tiến tới một giới hạn khi $n$ tăng vô hạn.
Điều này suy ra ngay từ Định lý 2 và công thức (2) của No. 1.*

#### Nhận xét 3 {#ac-viii-s4-n3-rem-3 .statement}

Giả sử q được chứa trong căn của A. Khi đó, theo bổ đề Nakayama, dãy (q^nM) dừng nếu và chỉ nếu ta có q^nM = 0 với n đủ lớn. Khi đó suy ra từ phần a) của hệ quả rằng ta có d_q(M) \leq 0 nếu và chỉ nếu M có độ dài hữu hạn, và khi ấy ta có e_q(M) = \operatorname{long}_A(M).

#### Mệnh đề 4 {#ac-viii-s4-prop-4 .statement}

Cho A là một vành Noether, x_1, ..., x_r là các phần tử của A, x là iđêan do chúng sinh, và M là một A-môđun hữu hạn sinh sao cho M/xM khác không và có độ dài hữu hạn.
a) Ta có d_x(M) \leq r.
b) Nếu d_x(M) = r, thì e_x(M) \leq \operatorname{long}_A(M/xM).
c) Nếu dãy (x_1, ..., x_r) hoàn toàn cắt đối với M (A, X, p. 157), thì d_x(M) = r và e_x(M) = \operatorname{long}_A(M/xM). Điều đảo lại là đúng nếu các x_i thuộc căn của A.

Gọi H là vành đa thức (A/x)[X_1, ..., X_r]. Trang bị cho G = \bigoplus_n x^nM/x^{n+1}M cấu trúc của một H-môđun phân bậc sao cho (X_i)_G là phép nhân bởi lớp của x_i modulo x^2. Với ký hiệu P_G, Q_G, c_G của No. 2, ta có H_{M,x} = P_G, do đó (1 - T)^{-d_x(M)}R = (1 - T)^{-r}Q_G, trong đó R(1) = e_x(M) > 0 và Q_G(1) = c_G.

Vậy hoặc d_x(M) < r và c_G = 0, hoặc d_x(M) = r và c_G = e_x(M). Hơn nữa, theo Mệnh đề 1 của No. 2, ta có c_G \leq \operatorname{long}(M/xM), và có đẳng thức nếu và chỉ nếu đồng cấu chính tắc A/x[X_1, ..., X_r] \otimes_{A/x} M/xM \to \bigoplus_n x^nM/x^{n+1}M là song ánh. Điều này kéo theo mệnh đề, xét theo A, X, p. 160, định lý 1.

#### Mệnh đề 5 {#ac-viii-s4-prop-5 .statement}

Cho 0 \to M' \to M \to M'' \to 0 là một dãy khớp của các môđun hữu hạn sinh trên một vành Noether A, và q là một iđêan của A.
a) Để M/qM có độ dài hữu hạn, điều kiện cần và đủ là M'/qM' và M''/qM'' cũng có tính chất đó.
b) Giả sử M/qM có độ dài hữu hạn. Khi đó ta ở trong một trong ba trường hợp sau:
1) d_q(M) = d_q(M') > d_q(M'') \text{ and } e_q(M) = e_q(M'),
2) d_q(M) = d_q(M'') > d_q(M') \text{ and } e_q(M) = e_q(M''),
3) d_q(M) = d_q(M') = d_q(M'') \text{ and } e_q(M) = e_q(M') + e_q(M'').
a) Ta có Supp(M) = Supp(M') \cup Supp(M'') và mệnh đề suy ra từ Nhận xét 2.
b) Trang bị cho M một filtration q-tốt F (chẳng hạn filtration q-adic), cho M'' filtration thương F'', và cho M' filtration cảm sinh F'. Các filtrations F' và F'' là q-tốt (III, § 3, No. 1, Mệnh đề 1). Khi đó với mỗi n ta có một dãy khớp các A-môđun
$$
0 \to F'_n/F'_{n+1} \to F_n/F_{n+1} \to F''_n/F''_{n+1} \to 0
$$
(III, § 2, No. 4, Mệnh đề 2), do đó ta có H_{M,F} = H_{M',F'} + H_{M'',F''}, hay cũng thế
$$
(1 - T)^{-d_q(M)}R = (1 - T)^{-d_q(M')}R' + (1 - T)^{-d_q(M'')}R''
$$
với R, R', R'' \in \mathbf{Z}[T, T^{-1}], R(1) = e_q(M), R'(1) = e_q(M'), R''(1) = e_q(M''). Mệnh đề b) suy ra từ đó ngay lập tức.

### 4. Bậc của hàm Hilbert-Samuel

#### Định lý 3 {#ac-viii-s4-thm-3 .statement}

Cho $A$ là một vành địa phương Noether, $q$ là một iđêan của $A$ phân biệt với $A$, và $M$ là một $A$-môđun hữu hạn sinh sao cho $M/qM$ có độ dài hữu hạn. Khi đó số nguyên $d_q(M)$ là chiều của $A$-môđun $M$ ($§ 1$, No. 4, Def. 8).

Ta có thể giả sử $M \neq 0$. Hãy chứng minh bất đẳng thức $d_q(M) \leq \dim_A(M)$. Theo Hệ quả 2 của Mệnh đề 9 của $§ 3$, No. 5, tồn tại $x_1, ..., x_r \in q$, với $r = \dim_A(M)$ và $\operatorname{long}(M / \sum_{i=1}^r x_i M) < +\infty$; đặt $x = \sum_{i=1}^r x_i A$. Theo Mệnh đề 4 của No. 3, ta có $d_x(M) \leq r$; ta có $x \subset q$, do đó $H^{(1)}_{M,q} \leq H^{(1)}_{M,x}$ và vì thế (Bổ đề 2 của No. 1)

$$
d_q(M) \leq d_x(M) \leq r = \dim_A(M).
$$

Bây giờ hãy chứng minh, bằng quy nạp theo $\dim_A(M)$, bất đẳng thức $\dim_A(M) \leq d_q(M)$, điều này hiển nhiên khi $\dim_A(M) = 0$.

Giả sử $\dim_A(M) > 0$, và $\dim_A(N) \leq d_q(N)$ với mọi $A$-môđun sinh hữu hạn $N$ sao cho $\dim_A(N) < \dim_A(M)$. Nếu $0 = M_0 \subset M_1 \subset ... \subset M_n = M$ là một chuỗi hợp thành của $M$, ta có $\dim_A(M) = \sup(\dim_A(M_i/M_{i-1}))$ ($§ 1$, No. 4, prop. 9) và $d_q(M) = \sup(d_q(M_i/M_{i-1}))$ (No. 3, prop. 5). Theo IV, $§ 1$, No. 4, th. 1, do đó có thể giả sử rằng $M$ có dạng $A/p$, trong đó $p$ là một iđêan nguyên tố của $A$, và ta có $p \neq m_A$ vì $\dim_A(M) > 0$. Lấy $x \in m_A - p$; phép vị tự $x_M$ của $M = A/p$ là đơn ánh, và ta có dãy khớp

$$
0 \longrightarrow M \xrightarrow{x_M} M \longrightarrow M/xM \longrightarrow 0.
$$

Theo $§ 3$, No. 2, prop. 3, ta có $\dim_A(M/xM) = \dim_A(M) - 1$; theo prop. 5 của No. 3, và dãy khớp trước đó, ta có $d_q(M/xM) \leq d_q(M) - 1$. Theo giả thiết quy nạp, do đó ta có

$$
\dim_A(M) = \dim_A(M/xM) + 1 \leq d_q(M/xM) + 1 \leq d_q(M),
$$

điều này hoàn tất chứng minh.

#### Hệ quả {#ac-viii-s4-n4-cor-1 .statement}

Cho $A$ là một vành Noether, $M$ là một $A$-môđun sinh hữu hạn và $q$ là một iđêan của $A$ sao cho $M/qM$ có độ dài hữu hạn. Khi đó $d_q(M)$ là cận trên bé nhất của các số chiều $\dim_{A_m}(M_m)$, khi $m$ chạy qua tập hợp hữu hạn $S = \operatorname{Supp}(M) \cap V(q)$, và $e_q(M)$ là tổng của các $e_{q_m}(M_m)$ lấy trên những phần tử $m$ của $S$ mà với chúng ta có $\dim_{A_m}(M_m) = d_q(M)$.

Với mỗi số nguyên $n$, độ dài của $M/q^nM$ là tổng của các $\operatorname{long}_{A_m}(M_m/q^n_m M_m)$ (IV, $§ 2$, No. 5, cor. 1 to prop. 7 and corollary to prop. 8). Do đó, ta có $H_{M,q} = \sum_{m \in S} H_{M_m,q_m}$, do đó có hệ quả.

#### Nhận xét 1 {#ac-viii-s4-n4-rem-1 .statement}

Ta cũng có $d_q(M) = \sup_{m \in V(q)} \dim(M_m)$, nghĩa là, $d_q(M) = \dim(\hat{M})$, trong đó $\hat{M}$ là bổ sung của $M$ đối với tôpô q-adic ($§ 3$, No. 4, prop. 8).

#### Nhận xét 2 {#ac-viii-s4-n4-rem-2 .statement}

Giả sử q được chứa trong căn của A; khi đó $\dim(\hat{M}) = \dim(M)$ (*loc. cit.*, cor. 1), do đó $d(M) = \dim(M)$.

### 5. Chuỗi Hilbert-Samuel của một môđun thương

#### Bổ đề 5 {#ac-viii-s4-lem-5 .statement}

Cho A là một vành, M là một A-môđun và $(P_n), (Q_n)$ là hai lọc giảm trên M gồm các môđun con. Giả sử rằng ta có $P_n \supset Q_n$ và $\operatorname{long}_A(P_n/Q_n) < +\infty$ với mọi $n \in \mathbf{Z}$ và rằng tồn tại một số nguyên $n_1$ sao cho $Q_{n_1} = M$. Trong $\mathbf{Z}((T))$, ta có các bất đẳng thức

$$
\sum_{n \in \mathbf{Z}} \operatorname{long}_A((P_{n+1} \cap Q_n)/Q_{n+1}).T^n \leq \sum_{n \in \mathbf{Z}} \operatorname{long}_A(P_{n+1}/Q_{n+1}).T^n \leq
$$
$$
\leq (1-T)^{-1} \sum_{n \in \mathbf{Z}} \operatorname{long}_A((P_{n+1} \cap Q_n)/Q_{n+1}).T^n .
$$

Vấn đề là chứng minh rằng ta có các bất đẳng thức

(15) $\operatorname{long}((P_{n+1} \cap Q_n)/Q_{n+1}) \leq \operatorname{long}(P_{n+1}/Q_{n+1})$,
(16) $\operatorname{long}(P_{n+1}/Q_{n+1}) \leq \sum_{i \leq n} \operatorname{long}((P_{i+1} \cap Q_i)/Q_{i+1})$.

Bất đẳng thức thứ nhất là hiển nhiên. Mặt khác, ta có $P_{n+1} \cap Q_i = P_{n+1}$ với $i \leq n_1$ và $P_{n+1} \cap Q_{n+1} = Q_{n+1}$; do đó suy ra bất đẳng thức
$$
\operatorname{long}(P_{n+1}/Q_{n+1}) \leq \sum_{i \leq n} \operatorname{long}((P_{n+1} \cap Q_i)/(P_{n+1} \cap Q_{i+1})) .
$$

Nhưng A-môđun $(P_{n+1} \cap Q_i)/(P_{n+1} \cap Q_{i+1})$ đẳng cấu với một môđun con của $(P_{i+1} \cap Q_i)/Q_{i+1}$, và bất đẳng thức (16) suy ra được.

#### Bổ đề 6 {#ac-viii-s4-lem-6 .statement}

Cho A là một vành, M một A-môđun và $(F_n)$ một lọc giảm trên M gồm các môđun con; giả sử rằng tồn tại một số nguyên $n_1$ sao cho $F_{n_1} = M$. Gọi f là một tự đồng cấu của M, $M'$ là hạt nhân của nó và $M''$ là đối hạt nhân của nó. Ta trang bị cho $M'$ lọc $(F'_n)$ cảm sinh bởi $(F_n)$ và cho $M''$ lọc thương $(F''_n)$ của $(F_n)$. Giả sử rằng $F_n/F_{n+1}$ có độ dài hữu hạn với mọi $n \in \mathbf{Z}$ và rằng tồn tại một số nguyên $\delta$ sao cho $f(F_n) \subset F_{n+\delta}$. Gọi $\varphi$ là tự đồng cấu phân bậc bậc $\delta$ của môđun phân bậc $\mathrm{gr}(M) = \bigoplus_{n \in \mathbf{Z}} F_n/F_{n+1}$ suy ra từ f. Giữa các phần tử sau của $\mathbf{Z}((T))$

$$
H_M = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(F_n/F_{n+1}).T^n
$$
$$
H_{M'} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(F'_n/F'_{n+1}).T^n
$$
$$
H_{M''} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(F''_n/F''_{n+1}).T^n
$$
$$
P_{\mathrm{Ker}(\varphi)} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(\mathrm{Ker}(\varphi_n)).T^n ,
$$

ta có các bất đẳng thức

(17) $H_{M'} \leq P_{\mathrm{Ker}(\varphi)}$

(18) $(1 - T^\delta).H_M^{(1)} + T^\delta.P_{\mathrm{Ker}(\varphi)} \leq H_{M''}^{(1)} \leq (1 - T^\delta).H_M^{(1)} + T^\delta.P_{\mathrm{Ker}(\varphi)}^{(1)}$.

Dãy các môđun con $G_n = f^{-1}(F_{n+\delta})$ của $M$ là một lọc giảm, và ta có $F_n \subset G_n$ với mọi số nguyên $n$.
Theo định nghĩa, ta có $\mathrm{Ker}(\varphi_n) = (G_{n+1} \cap F_n)/F_{n+1}$, do đó

(19) $P_{\mathrm{Ker}(\varphi)} = \sum_{n \in \mathbf{Z}} \mathrm{long}_A((G_{n+1} \cap F_n)/F_{n+1}).T^n$.

Với mọi $n$, A-môđun $(M' \cap F_n)/(M' \cap F_{n+1})$ được đồng nhất với một môđun con của $(G_{n+1} \cap F_n)/F_{n+1}$, và bất đẳng thức (17) suy ra ngay từ (19). Theo bổ đề 5, hơn nữa ta có

(20) $P_{\mathrm{Ker}(\varphi)} \leq \sum_{n \in \mathbf{Z}} \mathrm{long}_A(G_{n+1}/F_{n+1}).T^n \leq P_{\mathrm{Ker}(\varphi)}^{(1)}$.

Với mọi $n \in \mathbf{Z}$, ta có một dãy khớp các A-môđun

$$ 0 \longrightarrow G_{n+1}/F_{n+1} \longrightarrow M/F_{n+1} \xrightarrow{f_n} M/F_{n+\delta+1} \longrightarrow M''/F''_{n+\delta+1} \longrightarrow 0, $$

trong đó $f_n$ suy ra từ $f$ bằng cách chuyển qua các thương. Do đó ta có

$\mathrm{long}_A(M''/F''_{n+\delta+1}) = \mathrm{long}_A(M/F_{n+\delta+1}) - \mathrm{long}_A(M/F_{n+1}) + \mathrm{long}_A(G_{n+1}/F_{n+1})$.

Nhân với $T^{n+\delta}$ rồi lấy tổng theo $n$, ta thu được

(21) $H_{M''}^{(1)} = (1 - T^\delta)H_M^{(1)} + T^\delta.\sum_{n \in \mathbf{Z}} \mathrm{long}_A(G_{n+1}/F_{n+1}).T^n,$

và bất đẳng thức (18) suy ra ngay từ (20) và (21).

#### Bổ đề 7 {#ac-viii-s4-lem-7 .statement}

Giữ lại các ký hiệu của bổ đề 6.

a) Ta có bất đẳng thức $H_{M''}^{(1)} \geq \frac{1 - T^\delta}{1 - T} H_M$.

b) Để có đẳng thức, điều kiện cần và đủ là $\varphi$ đơn ánh.

c) Nếu đúng như vậy, ta có $M' \subset \bigcap_n F_n$, và dãy khớp các A-môđun

$$ 0 \longrightarrow \mathrm{gr}(M) \xrightarrow{\varphi} \mathrm{gr}(M) \xrightarrow{v} \mathrm{gr}(M'') \longrightarrow 0, $$

trong đó $v$ là ánh xạ chính tắc, là khớp.

Các khẳng định a) và b) suy ra từ công thức (18) của bổ đề 6, và từ định nghĩa $H_M^{(1)} = (1 - T)^{-1}.H_M$.

Giả sử rằng $\varphi$ là đơn ánh. Theo III, § 2, no 8, th. 1, (i), ta có

$$ \mathrm{Ker}(f) \subset f^{-1}(F_{n+\delta}) = F_n $$

với mọi $n$, do đó có mệnh đề thứ nhất của c). Hơn nữa, có một dãy khớp

$$
0 \longrightarrow M/M' \xrightarrow{f'} M \longrightarrow M/f(M) \longrightarrow 0,
$$

trong đó $f'$ được suy ra từ $f$ bằng cách chuyển qua thương. Nếu $\varphi$ là đơn ánh, như trên ta có ${f'}^{-1}(F_n) = F_{n-\delta}/M'$. Suy ra rằng lọc trên $M/M'$ suy ra như ảnh ngược bởi $f'$ của lọc $F$ trên $M$ là lọc $n \mapsto F_{n-\delta}/M'$; môđun phân bậc liên kết là $\mathrm{gr}(M)(-\delta)$ và có một dãy khớp các môđun phân bậc (III, § 2, no. 4, mệnh đề 2)

$$
0 \longrightarrow \mathrm{gr}(M)(-\delta) \xrightarrow{\varphi'} \mathrm{gr}(M) \longrightarrow \mathrm{gr}(M'') \longrightarrow 0,
$$

trong đó $\varphi'_n = \varphi_{n-\delta}$ với mọi $n$. Điều này hoàn tất chứng minh của c).

#### Mệnh đề 6 {#ac-viii-s4-prop-6 .statement}

*Cho A là một vành Noether, M là một A-môđun hữu hạn sinh và q là một iđêan của A sao cho M/qM có độ dài hữu hạn. Cho F là một lọc q-tốt của M, và $\mathrm{gr}(A) = \bigoplus_{n \geq 0} (q^n/q^{n+1})$ là vành phân bậc liên kết với A đối với lọc q-adic.*

*Cho $(x_1, ..., x_s)$ là một dãy các phần tử của A, $(\delta_1, ..., \delta_s)$ là một dãy các số nguyên dương ngặt sao cho $x_i \in q^{\delta_i}$ với $1 \leq i \leq s$, và gọi $\xi_i$ là lớp của $x_i$ trong $\mathrm{gr}_{\delta_i}(A) = q^{\delta_i}/q^{\delta_i+1}$.*

a) Trang bị cho A-môđun $\overline{M} = M/(x_1M + \cdots + x_sM)$ lọc q-tốt $\overline{F}$ là thương của F. Khi đó ta có trong $\mathbf{Z}((T))$ bất đẳng thức

$$
H_{\overline{M}, \overline{F}}^{(s)} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H_{M, F}.
$$

b) *Để có đẳng thức trong (22), điều kiện cần và đủ là dãy $(\xi_1, ..., \xi_s)$ các phần tử của vành $\mathrm{gr}(A)$ là hoàn toàn cát tuyến đối với môđun $\mathrm{gr}(M) = \bigoplus_{n} (F_n/F_{n+1})$.*

*Trong trường hợp đó, đồng cấu chính tắc từ $\mathrm{gr}(M)/\sum_{i=1}^s \xi_i \cdot \mathrm{gr}(M)$ vào $\mathrm{gr}(\overline{M}) = \bigoplus (\overline{F}_n/\overline{F}_{n+1})$ là một đẳng cấu.*

c) *Giả sử các điều kiện của b) được thỏa mãn, và mỗi A-môđun $M_i = M/(x_1M + \cdots + x_iM)$ ($0 \leq i < s$) đều tách đối với tôpô q-adic¹. Khi đó dãy $(x_1, ..., x_s)$ là hoàn toàn cát tuyến đối với A-môđun M.*

Khi $s = 1$, ta có $\bigcap_n F_n = \bigcap_n q^nM$ và dãy $\{ \xi_1 \}$ là hoàn toàn cát tuyến đối với $\mathrm{gr}(M)$ khi và chỉ khi phép vị tự tỉ số $\xi_1$ trong $\mathrm{gr}(M)$ là đơn ánh. Khi đó mệnh đề 6 suy ra ngay từ bổ đề 7 áp dụng cho phép vị tự $f = (x_1)_M$ trong M.

Giả sử $s \geq 2$ và lập luận bằng quy nạp theo s. Giả thiết quy nạp áp dụng cho A-môđun $M_1 = M/x_1M$ được trang bị lọc G là thương của F, và cho dãy $(x_2, ..., x_s)$, cho bất đẳng thức

$$
H_{M_1, G}^{(s-1)} \geq \left( \prod_{i=2}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H_{M_1, G};
$$

¹ Điều này xảy ra đặc biệt nếu q được chứa trong căn của A (III, § 3, no. 3, mệnh đề 6).

có đẳng thức khi và chỉ khi dãy $(\xi_2, ..., \xi_s)$ là hoàn toàn cát tuyến đối với gr(A)-môđun $gr(M_1) = \bigoplus_n G_n/G_{n+1}$. Vì các phần tử $\frac{1 - T^{\delta_i}}{1 - T}$ của $\mathbf{Z}((T))$ là dương, trường hợp $s = 1$ đã được xét và công thức (23) cho các bất đẳng thức

$$
H^{(s)}_{M,F} \geq \left( \prod_{i=2}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H^{(1)}_{M_1,G} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H_{M,F}.
$$

Điều này chứng minh *a*).

Chỉ có thể có đẳng thức trong (22) nếu đồng thời có đẳng thức trong (23) và đẳng thức

$$
H^{(1)}_{M_1,G} = \left( \frac{1 - T^{\delta_1}}{1 - T} \right) \cdot H_{M,F}.
$$

Quan hệ cuối cùng này có nghĩa là $\{\xi_1\}$ hoàn toàn cắt đối với gr(M) và kéo theo rằng đồng cấu chính tắc từ gr(M)/$\xi_1\cdot$gr(M) vào gr(M_1) là một đẳng cấu. Nói cách khác, có đẳng thức trong (22) khi và chỉ khi $\{\xi_1\}$ hoàn toàn cắt đối với gr(M) và $\{\xi_2, ..., \xi_s\}$ hoàn toàn cắt đối với gr(M)/$\xi_1\cdot$gr(M). Điều này có nghĩa là $\{\xi_1, ..., \xi_s\}$ hoàn toàn cắt đối với gr(M) (A, X, p. 160, Hệ quả 2). Vậy sự tương đương của hai điều kiện của *b*) đã được chứng minh. Giả sử các điều kiện ấy được thỏa mãn; khi đó, theo giả thiết quy nạp, gr(M) được đồng nhất với $gr(M_1)/\sum_{i=2}^s \xi_i \cdot gr(M_1)$; hơn nữa, vì gr(M_1) được đồng nhất với gr(M)/$\xi_1\cdot$gr(M), nên khẳng định cuối cùng của *b*) vì thế được thỏa mãn.

Bây giờ giả sử rằng $\{\xi_1, ..., \xi_s\}$ hoàn toàn cắt đối với gr(M) và M_i tách biệt đối với tôpô q-adic (với $0 \leq i < s$). Từ điều trên và giả thiết quy nạp, dãy $(x_2, ..., x_s)$ hoàn toàn cắt đối với M_1; vì ta có $M_1 = M/x_1M$ và $\{x_1\}$ hoàn toàn cắt đối với M, nên dãy $(x_1, x_2, ..., x_s)$ hoàn toàn cắt đối với M (A, X, p. 160, Định lý 1).

## BÀI TẬP {#ac-viii-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
