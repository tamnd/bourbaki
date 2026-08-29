---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 5
section_title: Anneaux locaux réguliers
lang: vi
source: ac-viii-ix-fr
book_pages: AC VIII.51-AC VIII.62, AC VIII.94-AC VIII.99
pdf_pages: 0055-0066, 0098-0103
extraction: ocr
subsections:
    - "no": 1
      title: Définition des anneaux locaux réguliers
      page: 51
      pdf_page: 55
    - "no": 2
      title: Anneau gradué associé à un anneau local régulier
      page: 0
      pdf_page: 57
    - "no": 3
      title: Quotients d’anneaux locaux réguliers
      page: 55
      pdf_page: 59
    - "no": 4
      title: Polynômes d’Eisenstein
      page: 56
      pdf_page: 60
statements: 31
exercises: 31
content_sha256: 8266133778da12243fad62bbb47b1468d7acdc4c36b9f2bce16333d70dbae410
translated_from: content/en-mt/ac/VIII/05_s5_anneaux_locaux_reguliers.md
source_lang: en-mt
translation_method: machine
source_content_sha256: f0890961783e65fe843b3637347cf0475429ec007565bdf26a6603b5d3542820
translation_model: gpt-5-mini, gpt-5-6
translation_run: translate-vi-4ee1992c
glossary_version: 34
glossary_terms_sha256: 2c3af4be2dcf61bf4d9ff361058bd1804adaf9aceb36f52e45f70ee3bb03b146
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 5. VÀNH ĐỊA PHƯƠNG CHÍNH QUY

### 1. Định nghĩa các vành địa phương chính quy

Cho A là một vành địa phương Noether. Cho $(x_i)_{i \in I}$ là một họ các phần tử của $m_A$. Theo Hệ quả 2 của Mệnh đề 4 trong II, § 3, No. 2, điều này tương đương với việc giả sử rằng họ $(x_i)_{i \in I}$ sinh iđêan $m_A$ của A, hoặc rằng các lớp của các $x_i$ modulo $m_A^2$ sinh không gian vectơ $\kappa_A$ $m_A/m_A^2$; nếu điều này xảy ra, ta có $\dim(A) \leq \mathrm{Card}(I)$ theo chú giải của § 3, No. 2. Do đó ta có bất đẳng thức

$$
\dim(A) \leq [m_A/m_A^2 : \kappa_A] \leq \mathrm{Card}(I)
$$

với mọi họ $(x_i)_{i \in I}$ sinh iđêan $m_A$ của A.

#### Định nghĩa 1 {#ac-viii-s5-def-1 .statement}

Vành địa phương Noether $A$ được gọi là chính quy nếu có $\dim(A) = [\mathfrak{m}_A/\mathfrak{m}_A^2 : \kappa_A]$. Một **hệ tọa độ** của $A$ khi đó là mọi họ các phần tử của $\mathfrak{m}_A$ mà các lớp của chúng modulo $\mathfrak{m}_A^2$ tạo thành một cơ sở của không gian vectơ $\kappa_A$ $\mathfrak{m}_A/\mathfrak{m}_A^2$.

Một hệ tọa độ trong một vành địa phương Noether chính quy $A$ do đó là một họ hữu hạn $(x_i)_{i \in I}$ sinh iđêan $\mathfrak{m}_A$ của $A$ và sao cho $\mathrm{Card}(I) = \dim(A)$. Ngược lại, nếu iđêan $\mathfrak{m}_A$ của một vành địa phương Noether $A$ được sinh bởi $d$ phần tử với $d \leq \dim(A)$, thì vành $A$ là chính quy.

#### Ví dụ 1 {#ac-viii-s5-n1-exa-1 .statement}

Các vành địa phương Noether chính quy có chiều 0 (tương ứng, 1) là các trường (tương ứng, các vành định giá rời rạc) (VI, § 3, No. 6, Mệnh đề 9 và Hệ quả 1 của Định lý 1 dưới đây). Cho $A$ là một vành định giá rời rạc; khi đó một phần tử $t$ của $\mathfrak{m}_A$ là một phần tử nguyên thủy khi và chỉ khi $\{ t \}$ là một hệ tọa độ của $A$.

#### Ví dụ 2 {#ac-viii-s5-n1-exa-2 .statement}

Cho $k$ là một trường và cho $n$ là một số nguyên dương. Vành các chuỗi lũy thừa hình thức $k[[X_1, ..., X_n]]$ là một vành địa phương Noether chính quy có chiều $n$ (§ 3, No. 4, Hệ quả 3 của Mệnh đề 8). Cho $F_1, ..., F_n$ là các chuỗi lũy thừa hình thức không có số hạng hằng trong $k[[X_1, ..., X_n]]$; để dãy $(F_1, ..., F_n)$ là một hệ tọa độ của $k[[X_1, ..., X_n]]$, điều kiện cần và đủ là ma trận $\left( \frac{\partial F_i}{\partial X_j}(0, ..., 0) \right)$ khả nghịch.

Tổng quát hơn, cho $A$ là một vành địa phương Noether chính quy có chiều $r$; khi đó $A[[X_1, ..., X_n]]$ là một vành địa phương Noether chính quy có chiều $r + n$. Nếu $(a_1, ..., a_r)$ là một hệ tọa độ của $A$, thì $(a_1, ..., a_r, X_1, ..., X_n)$ là một hệ tọa độ của $A[[X_1, ..., X_n]]$.

#### Ví dụ 3 {#ac-viii-s5-n1-exa-3 .statement}

Cho $A$ là một vành địa phương Noether chính quy đầy đủ có chiều $r$. Vành $A \{ X_1, ..., X_n \}$ các chuỗi lũy thừa hình thức hạn chế là một vành địa phương Noether chính quy có chiều $r + n$ (§ 3, No. 4, Nhận xét 1). Nếu $(a_1, ..., a_r)$ là một hệ tọa độ của $A$, thì $(a_1, ..., a_r, X_1, ..., X_n)$ là một hệ tọa độ của $A \{ X_1, ..., X_n \}$.

#### Ví dụ 4 {#ac-viii-s5-n1-exa-4 .statement}

Cho $k$ là một trường đầy đủ không rời rạc có giá trị. Vành các chuỗi lũy thừa hình thức theo $n$ biến hội tụ trong một lân cận của 0 trong $k^n$ là một vành địa phương Noether chính quy có chiều $n$ (§ 3, No. 4, Nhận xét 2).

#### Ví dụ 5 {#ac-viii-s5-n1-exa-5 .statement}

Cho $k$ là một trường, $A$ là một $k$-đại số nguyên hữu hạn kiểu, và $m$ là một iđêan cực đại của $A$. Vành địa phương Noether $A_m$ là chính quy khi và chỉ khi có $\dim(A) = [m/m^2 : A/m]$; thực vậy, có $\dim(A_m) = \dim(A)$ (§ 2, No. 4, Hệ quả 2 của Định lý 3) và các không gian vectơ $m/m^2$ và $mA_m/(mA_m)^2$ trên trường $A/m$ là đẳng cấu (II, § 3, No. 3, Mệnh đề 9). Đặc biệt, nếu $k$ là đóng đại số, điều kiện đã nêu là tương đương với $\dim(A) = [m/m^2 : k]$ (V, § 3, No. 3, Mệnh đề 1).

#### Ví dụ 6 {#ac-viii-s5-n1-exa-6 .statement}

Cho $X$ là một đa tạp đại số trên một trường hoàn hảo $k$. Khi đó $X$ không kì dị tại một điểm $x$ khi và chỉ khi vành địa phương của $X$ tại $x$ là chính quy.

#### Ví dụ 7 {#ac-viii-s5-n1-exa-7 .statement}

Cho $A$ là một vành địa phương Noether chính quy. Ta sẽ thấy sau này rằng vành địa phương Noether $A_p$ là chính quy với mọi iđêan nguyên tố $p$ của $A$.

#### Mệnh đề 1 {#ac-viii-s5-prop-1 .statement}

Cho $A$ và $B$ là các vành địa phương Noether và $\rho : A \to B$ là một đồng cấu địa phương làm cho $B$ là một $A$-môđun phẳng. Giả sử rằng có m_B = B.\rho(m_A). Khi đó dim(A) = dim(B) và B là chính quy khi và chỉ khi A là chính quy.

Mệnh đề đầu tiên suy ra từ Hệ quả 1 của Mệnh đề 7 của § 3, No. 4. Vì B là phẳng trên A, ta có thể đồng nhất m_B^k = B.\rho(m_A^k) với B \otimes_A m_A^k với mọi số nguyên k \geqslant 0, do đó đồng nhất m_B/m_B^2 với B \otimes_A (m_A/m_A^2), hoặc một lần nữa với \kappa_B \otimes_{\kappa_A} (m_A/m_A^2). Vì vậy ta có

(2)
$$
[m_B/m_B^2 : \kappa_B] = [m_A/m_A^2 : \kappa_A],
$$
do đó mệnh đề được suy ra ngay lập tức.

#### Hệ quả {#ac-viii-s5-n1-cor-1 .statement}

Một vành địa phương Noether A là chính quy khi và chỉ khi bao đầy đủ của nó $\hat{A}$ cũng như vậy.

Thực vậy, $\hat{A}$ là phẳng trên A, và có $m_{\hat{A}} = \hat{A}.m_A$ (III, § 3, No. 4, Định lý 3 và § 2, No. 12, Hệ quả 2 của Mệnh đề 16).

### 2. Vành phân bậc liên kết với một vành địa phương chính quy

#### Định lý 1 {#ac-viii-s5-thm-1 .statement}

Cho A là một vành địa phương Noether. Các điều kiện sau là tương đương:
(i) A là chính quy.
(ii) Iđêan $m_A$ được sinh bởi một tập con cắt ngang đối với A (§ 3, No. 2, Định nghĩa 1).
(iii) Iđêan $m_A$ được sinh bởi một dãy cắt ngang hoàn toàn đối với A (A, X, p. 157, Định nghĩa 2).
(iv) Gọi S là đại số đối xứng của không gian vectơ $\kappa_A$- $m_A/m_A^2$, và gọi gr(A) = $\bigoplus_{n \geqslant 0} m_A^n/m_A^{n+1}$ là vành phân bậc liên kết với A. Đồng cấu chính tắc $\gamma$ của S lên gr(A) là song ánh.
(v) Tồn tại một số nguyên $r \geqslant 0$ sao cho có $H_{A,m_A} = (1 - T)^{-r}$, nghĩa là $m_A = 0$ nếu $r = 0$ và $[m_A^n/m_A^{n+1} : \kappa_A] = \binom{n + r - 1}{r - 1}$ với mọi số nguyên $n \geqslant 0$ nếu $r > 0$.
(vi) Có $H_{A,m_A} = (1 - T)^{-d}$ với $d = \dim(A)$.

Nếu các điều kiện này được thỏa mãn, mọi hệ tọa độ của A là một dãy cắt ngang hoàn toàn đối với A.

(ii) \Rightarrow (i): mọi tập con secant có nhiều nhất $\dim(A)$ phần tử (§ 3, No. 2, Định lý 1).
(iii) \Rightarrow (ii): mọi dãy secant hoàn toàn đều là secant (§ 3, No. 2, hệ quả của Mệnh đề 3).
(iv) \Rightarrow (iii): cho $(x_1, ..., x_r)$ là một dãy các phần tử của $m_A$ mà các lớp của chúng modulo $m_A^2$ tạo thành một cơ sở $(\xi_1, ..., \xi_r)$ của $m_A/m_A^2$ trên trường $\kappa_A$. Nếu tính chất (iv) được thỏa mãn, $\mathrm{gr}(A)$ là đại số đa thức $\kappa_A[\xi_1, ..., \xi_r]$ và dãy $(x_1, ..., x_r)$ là secant hoàn toàn (A, X, p. 160, Định lý 1). Điều này cũng chứng minh khẳng định cuối cùng của Định lý 1.
(i) \Rightarrow (iv): đặt $r = [m_A/m_A^2 : \kappa_A]$. Theo công thức (6) của § 4, No. 2, chuỗi Poincaré của không gian vectơ phân bậc S trên trường $\kappa_A$ bằng

$$
P_S = \sum_{n \geqslant 0} [S^n(m_A/m_A^2) : \kappa_A] T^n = (1 - T)^{-r}.
$$

Giả sử rằng đồng cấu chính tắc $\gamma : S \to \mathrm{gr}(A)$ không song ánh. Vì $\gamma$ là toàn ánh, tồn tại một phần tử thuần nhất $u$ của $S$, có bậc $d > 0$, bị triệt tiêu bởi $\gamma$. Khi đó ta có

$$
H_{A,m_A} = P_S - P_{\mathrm{Ker}(\gamma)} \leq P_S - P_{uS} = (1 - T^d)/(1 - T)^r =
$$
$$
= (1 + T + \cdots + T^{d-1})/(1 - T)^{r-1}.
$$

Theo Định lý 3 của § 4, No. 4 và Bổ đề 2 của § 4, No. 1, do đó $\dim(A) < r$, và A không chính quy.

Cuối cùng, hãy chứng minh sự tương đương của các điều kiện (iv) đến (vi). Bây giờ (iv) có nghĩa là ta có $H_{A,m_A} = (1 - T)^{-s}$ với $s = [m_A/m_A^2 : \kappa_A]$. Do đó các điều kiện (iv), (v), (vi) có nghĩa là ta có $H_{A,m_A} = (1 - T)^{-m}$, tương ứng với $m = [m_A/m_A^2 : \kappa_A]$, $m \geq 0$, $m = \dim(A)$. Nhưng nếu ta có $H_{A,m_A} = (1 - T)^{-m}$, thì $\dim(A) = m$ theo § 4, No. 4, Định lý 3 và $[m_A/m_A^2 : \kappa_A] = m$ (vì $(1 - T)^{-m} = 1 + mT + \cdots$). Sự tương đương của các điều kiện (iv) đến (vi) suy ra ngay lập tức từ điều này.

#### Hệ quả 1 {#ac-viii-s5-thm-1-cor-1 .statement}

Mọi vành địa phương Noether chính quy đều đóng nguyên, và đặc biệt là một miền nguyên.

Giả sử rằng A là chính quy. Khi đó $\mathrm{gr}(A)$ đẳng cấu với một đại số đa thức trong một số hữu hạn các phần tử bất định trên một trường (Định lý 1, (iv)). Suy ra $\mathrm{gr}(A)$ là một vành Noether đóng nguyên (V, § 1, No. 3, Hệ quả 3 của Mệnh đề 13), và do đó A đóng nguyên (V, § 1, No. 4, Mệnh đề 15).

Ta sẽ thấy trong một chương sau rằng mọi vành địa phương Noether chính quy đều là nhân tử.

#### Hệ quả 2 {#ac-viii-s5-thm-1-cor-2 .statement}

Cho A và B là các vành địa phương Noether và $\sigma$ là một đồng cấu địa phương của B vào A. Giả sử rằng A là chính quy và B đầy đủ. Để $\sigma$ là song ánh, điều kiện cần và đủ là nó cảm sinh các song ánh của $\kappa_B$ lên $\kappa_A$ và của $m_B/m_B^2$ lên $m_A/m_A^2$.

Điều kiện đã nêu hiển nhiên là cần thiết.

Ngược lại, giả sử rằng $\sigma$ cảm sinh các đẳng cấu của $\mathrm{gr}_0(B)$ lên $\mathrm{gr}_0(A)$ và của $\mathrm{gr}_1(B)$ lên $\mathrm{gr}_1(A)$. Vì vành $\mathrm{gr}(B)$ được sinh bởi $\mathrm{gr}_0(B) \cup \mathrm{gr}_1(B)$ và $\mathrm{gr}(A)$ là đại số đối xứng của không gian vectơ $\mathrm{gr}_1(A)$ trên trường $\mathrm{gr}_0(A)$, đồng cấu $\mathrm{gr}(\sigma)$ là song ánh. Do đó $\sigma$ là song ánh (III, § 2, No. 8, Hệ quả 3 của Định lý 1).

#### Hệ quả 3 {#ac-viii-s5-thm-1-cor-3 .statement}

Cho k là một trường và A là một đại số trên k địa phương Noether có trường thặng dư bằng k. Để A là chính quy, điều kiện cần và đủ là phần đầy đủ của nó $\hat{A}$ đẳng cấu với một đại số chuỗi lũy thừa hình thức trên k $k[[X_1, ..., X_n]]$.

Điều này suy ra từ sự tương đương của (i) và (iv) trong Định lý 1, và từ Mệnh đề 11 của III, § 2, No. 9.

### 3. Các thương của các vành địa phương chính quy

#### Mệnh đề 2 {#ac-viii-s5-prop-2 .statement}

Cho $A$ là một vành địa phương Noether, $x = (x_1, ..., x_r)$ là một dãy các phần tử của $m_A$ và $x$ là iđêan sinh bởi $x$. Các điều kiện sau là tương đương:

(i) vành $A$ là chính quy, và $x$ tạo thành một phần của một hệ tọa độ của $A$;
(ii) vành $A/x$ là chính quy và $x$ là một dãy cắt đối với $A$;
(iii) vành $A/x$ là chính quy và $x$ là một dãy cắt hoàn toàn đối với $A$.

Hơn nữa, khi các điều kiện này được thỏa mãn, $x$ là một iđêan nguyên tố của $A$.

(iii) $\Rightarrow$ (ii): điều này suy ra từ hệ quả của Mệnh đề 3 của § 3, No. 2.

(ii) $\Rightarrow$ (i): giả sử rằng $x$ là một dãy cắt đối với $A$ và rằng vành địa phương Noether $A/x$ là chính quy. Gọi $(x_{r+1}, ..., x_d)$ là một dãy các phần tử của $A$ mà các lớp của chúng modulo $x$ tạo thành một hệ tọa độ của $A/x$. Khi đó dãy $(x_1, ..., x_d)$ sinh iđêan $m_A$ của $A$, và ta có

$$
\dim(A) = r + \dim(A/x) = r + (d - r) = d .
$$

Suy ra rằng $A$ là chính quy và rằng $(x_1, ..., x_d)$ là một hệ tọa độ của $A$.

(i) $\Rightarrow$ (iii): nếu điều kiện (i) được thỏa mãn, dãy $x$ là cắt hoàn toàn (No. 2, Định lý 1), do đó là cắt theo hệ quả của Mệnh đề 3 của § 3, No. 2. Vì vậy ta có

(3)
$$
\dim(A/x) = \dim(A) - r ;
$$

hơn nữa, các lớp của $x_1, ..., x_r$ modulo $m_A^2$ là độc lập tuyến tính trên trường $\kappa_A$, và do đó ta có

(4)
$$
[m_A/(m_A^2 + x) : \kappa_A] = [m_A/m_A^2 : \kappa_A] - r .
$$

Các công thức (3) và (4) chỉ ra rằng $A/x$ là chính quy.

Mọi vành địa phương Noether chính quy đều là một miền nguyên theo Hệ quả 1 của Định lý 1 của No. 2. Suy ra rằng $x$ là nguyên tố nếu $A/x$ là chính quy.

#### Hệ quả 1 {#ac-viii-s5-prop-2-cor-1 .statement}

Cho $A$ là một vành địa phương Noether, và $t$ là một phần tử của $m_A$. Các điều kiện sau là tương đương:

(i) $A$ là chính quy, và $t$ không thuộc $m_A^2$;
(ii) $A/tA$ là chính quy và $\dim(A/tA) < \dim(A)$;
(iii) $A/tA$ là chính quy, và $t$ không là một ước của 0 trong $A$.

#### Hệ quả 2 {#ac-viii-s5-prop-2-cor-2 .statement}

Cho $A$ là một vành địa phương Noether chính quy, và $q$ là một iđêan của $A$. Khi đó $A/q$ là chính quy khi và chỉ khi $q$ được sinh bởi một tập con của một hệ tọa độ của $A$.

Điều kiện là đủ theo Mệnh đề 2.

Giả sử $A/q$ chính quy, và cho $x = (x_1, ..., x_r)$ là một dãy các phần tử của $q$ mà các lớp của chúng modulo $m_A^2$ tạo thành một cơ sở của $(q + m_A^2)/m_A^2$ trên trường $\kappa_A$. Gọi $x$ là iđêan của $A$ sinh bởi $x$. Khi đó $x \subset q$ và $x$ tạo thành một phần của một hệ tọa độ của $A$, do đó vành địa phương Noether $A/x$ là chính quy (Mệnh đề 2); hơn nữa, các không gian vectơ $m_A/(q + m_A^2)$ và $m_A/(x + m_A^2)$ có cùng chiều trên $\kappa_A$. Suy ra rằng các vành địa phương Noether chính quy $A/q$ và $A/x$ có cùng chiều. Vì các iđêan $q$ và $x$ là nguyên tố và có $x \subset q$, cuối cùng ta kết luận rằng $q = x$.

#### Ví dụ {#ac-viii-s5-n3-exa-1 .statement}

Cho $k$ là một trường, $A = k[[X_1, ..., X_n]]$ và $q$ là một iđêan của $A$, phân biệt với $A$. Để $A/q$ là chính quy, điều kiện cần và đủ là có thể tìm được một số nguyên $r \geqslant 0$ và các phần tử $F_1, ..., F_r$ của $A$, sinh ra $q$, sao cho ma trận $\left( \frac{\partial F_i}{\partial X_j}(0, ..., 0) \right)$ có hạng $r$ ("tiêu chuẩn jacobian"). Khi đó có $\dim(A/q) = n - r$.

#### Nhận xét {#ac-viii-s5-n3-rem-1 .statement}

Cho $A$ là một vành địa phương Noether chính quy và $q \subset m_A$ là một iđêan của $A$ sao cho $A/q$ là chính quy. Cho $(x_1, ..., x_r)$ là một dãy các phần tử của $q$ mà các lớp của chúng modulo $m_A^2$ sinh không gian vectơ $(q + m_A^2)/m_A^2$ trên trường $\kappa_A$. Chứng minh của Hệ quả 2 cho thấy rằng iđêan $q$ của $A$ được sinh bởi $(x_1, ..., x_r)$.

### 4. Đa thức Eisenstein

#### Định nghĩa 2 {#ac-viii-s5-def-2 .statement}

Cho $A$ là một vành, $p$ là một iđêan nguyên tố của $A$, và $P$ là một đa thức trong $A[T]$. Ta nói rằng $P$ là một đa thức Eisenstein đối với $p$ nếu nó thỏa mãn các điều kiện sau:
a) $P$ là đơn thức có bậc $d \geqslant 1$;
b) có $P(T) \equiv T^d \mod. pA[T]$;
c) có $P(0) \notin p^2$.

Nói cách khác, một đa thức Eisenstein đối với $p$ là một đa thức có dạng $P(T) = T^d + \sum_{i=1}^d a_i T^{d-i}$, với $d \geqslant 1$, trong đó $a_1, ..., a_{d-1}$ thuộc $p$ và $a_d$ thuộc $p - p^2$.

Người ta nói rằng $P$ là một đa thức Eisenstein đối với $pA_p$ nếu ảnh chính tắc của $P$ trong vành đa thức $A_p[T]$ là một đa thức Eisenstein đối với iđêan $pA_p$; điều này cũng có nghĩa là $P$ là một đa thức Eisenstein đối với $p$ và hơn nữa nó thỏa mãn điều kiện sau đây, mạnh hơn c):
c’) mọi phần tử $a$ của $A$ sao cho $aP(0) \in p^2$ đều thuộc $p$.

#### Mệnh đề 3 {#ac-viii-s5-prop-3 .statement}

Cho $A$ là một vành, $p$ là một iđêan nguyên tố của $A$ và $P \in A[T]$ là một đa thức Eisenstein đối với $p$.
a) Không tồn tại một phân tích có dạng $P = P_1 P_2$ trong đó $P_1$ và $P_2$ là hai đa thức monic của $A[T]$ khác 1.
b) Giả sử $A$ đóng nguyên, với trường phân thức $K$. Khi đó $P$ là bất khả quy trong $K[T]$.

Gọi $\varphi$ là đồng cấu chính tắc của $A$ vào trường phân thức $k$ của $A/p$ và gọi $\varphi': A[T] \to k[T]$ là mở rộng của $\varphi$ sao cho $\varphi'(T) = T$. Giả sử rằng có $P = P_1P_2$ trong đó $P_1$ và $P_2$ là hai đa thức monic của $A[T]$ khác 1. Khi đó ta có $T^d = \varphi'(P_1)\varphi'(P_2)$ trong $k[T]$, ký hiệu $d$ là bậc của $P$. Nếu $d_i$ là bậc của $P_i$, do đó ta có $\varphi'(P_i) = T^{d_i}$, nghĩa là $P_i(T) \equiv T^{d_i} \mod pA[T]$, và đặc biệt $P_i(0) \in p$. Nhưng khi đó $P(0) = P_1(0).P_2(0)$ thuộc $p^2$, trái với các giả thiết. Điều này chứng minh a).

Mệnh đề b) suy ra từ a) và mệnh đề 11 của V, § 1, no 3.

Cho $A$ là một vành địa phương Noether và $P_1, ..., P_r$ là các đa thức monic trong $A[T]$, có bậc $\geq 2$. Gọi $q$ là iđêan của $A[T_1, ..., T_r]$ sinh bởi $P_1(T_1), ..., P_r(T_r)$ và gọi $B$ là đại số thương $A$-đại số $A[T_1, ..., T_r]/q$. Với $1 \leq i \leq r$, gọi $d_i$ là bậc của $P_i$, $t_i$ là lớp của $T_i$ modulo $q$, và $\gamma_i$ là lớp của $c_i = P_i(0)$ modulo $m_A^2$. Giả sử rằng $P_i(T) \equiv T^{d_i} \mod m_A A[T]$ với $1 \leq i \leq r$.

**Mệnh đề 4. — a)** *Vành $B$ là địa phương và Noether, với iđêan cực đại*

$$
m_B = Bm_A + \sum_{i=1}^r Bt_i.
$$

*Ta có $\dim(A) = \dim(B)$ và $[\kappa_B : \kappa_A] = 1$. Các đơn thức $t_1^{\alpha(1)} ... t_r^{\alpha(r)}$, với $0 \leq \alpha(i) < d_i$ với $1 \leq i \leq r$, lập thành một cơ sở của $A$-môđun $B$.*

**b)** Gọi $\lambda$ là đồng cấu chính tắc từ $m_A/m_A^2$ vào $m_B/m_B^2$. Khi đó hạt nhân của $\lambda$ là không gian vectơ $\kappa_A$ sinh bởi $\gamma_1, ..., \gamma_r$. Các lớp của các phần tử $t_1, ..., t_r$ lập thành một cơ sở trên $\kappa_A$ của đối hạt nhân của $\lambda$.*

**c)** Để $B$ là chính quy, điều kiện cần và đủ là $A$ là chính quy và $\gamma_1, ..., \gamma_r$ độc lập tuyến tính trong không gian vectơ $\kappa_A$ $m_A/m_A^2$.*

Đại số $A$-đại số $B$ đẳng cấu với tích tenxơ $B_1 \otimes_A \cdots \otimes_A B_r$ với $B_i = A[T]/(P_i)$ với $1 \leq i \leq r$. Suy ra rằng các đơn thức $t_1^{\alpha(1)} ... t_r^{\alpha(r)}$, với $0 \leq \alpha(i) < d_i$ với $1 \leq i \leq r$, lập thành một cơ sở của $A$-môđun $B$. Đặc biệt, $B$ là nguyên trên $A$, do đó $A$ và $B$ có cùng chiều theo Định lý 1 của § 2, No. 3.

Theo Hệ quả 3 của Mệnh đề 9 của IV, § 2, No. 5, vành $B$ là Noether, và mọi iđêan cực đại của $B$ đều chứa $B.m_A$. Hơn nữa, theo giả thiết về $P_1, ..., P_r$ và quan hệ $P_i(t_i) = 0$, ta có $t_i^{d_i} \in B.m_A$ với $1 \leq i \leq r$. Do đó mọi iđêan cực đại của $B$ đều chứa $t_1, ..., t_r$, và vì vậy cũng chứa iđêan $q' = B.m_A + Bt_1 + \cdots + Bt_r$. Khi đó ta có $m_A = A \cap q'$ và $B = A + q'$, do đó $B/q'$ đẳng cấu với $A/m_A$ và $q'$ là một iđêan cực đại của $B$; do đó, $B$ là địa phương và ta có $[\kappa_B : \kappa_A] = 1$. Điều này chứng minh a).

Đặt $r = m_A^2 + \sum_{i=1}^r Ac_i$, và ký hiệu $\varphi$ là đồng cấu chính tắc từ $(A/m_A^2)[T_1, ..., T_r]$ lên $B/m_B^2$. Vì ta có $m_B = B.m_A + \sum_{i=1}^r Bt_i$, hạt nhân $n$ của $\varphi$ là iđêan sinh bởi các lớp $\overline{P}_i(T_i)$ của các đa thức $P_i(T_i)$ modulo $m_A^2.A[T_1, ..., T_r]$ và các đơn thức $T_iT_j$ và $xT_i$ với $1 \leq i, j \leq r$ và $x$ trong $m_A/m_A^2$. Theo giả thiết về $P_i$, cụ thể là $P_i(T) \equiv T^{d_i} \mod m_A.A[T]$, ta có thể thay thế $\overline{P}_i(T_i)$ bởi $\gamma_i$ trong mô tả này của $n$; do đó, vành $B/m_B^2$ đẳng cấu với thương của $(A/r)[T_1, ..., T_r]$ theo iđêan phân bậc sinh bởi các đơn thức $T_i T_j$ và $x T_i$ với $x$ trong $m_A / r$. Gọi $\tau_i$ là lớp của $t_i$ modulo $m_B^2$; do đó ta có

$$
B / m_B^2 = (A/r) \oplus \kappa_A \tau_1 \oplus \cdots \oplus \kappa_A \tau_r,
$$

do đó

$$
m_B / m_B^2 = (m_A / r) \oplus \kappa_A \tau_1 \oplus \cdots \oplus \kappa_A \tau_r.
$$

Mệnh đề b) suy ra ngay từ điều này.

Theo công thức (6) và quan hệ $[ \kappa_B : \kappa_A ] = 1$, ta có

$$
[m_B / m_B^2 : \kappa_B] = [m_A / m^2 : \kappa_A] + \{ r - [r / m_A^2 : \kappa_A] \}.
$$

Bây giờ, không gian vectơ $\kappa_A$-$r / m_A^2$ được sinh bởi $\gamma_1, ..., \gamma_r$ và ta có

$$
\dim(B) = \dim(A) \leq [m_A / m_A^2 : \kappa_A].
$$

Mệnh đề c) suy ra ngay từ các công thức (7) và (8).

#### Hệ quả {#ac-viii-s5-n4-cor-1 .statement}

*Cho A là một vành địa phương Noether chính quy và cho P $\in A[T]$ là một đa thức Eisenstein đối với $m_A$. Vành $B = A[T]/(P)$ là một vành địa phương Noether chính quy, có cùng chiều với A, và ta có $[ \kappa_A : \kappa_B ] = 1$. Cuối cùng, ta có $m_B = B.m_A + Bt$, trong đó t là lớp của T modulo (P).*

Trường hợp P có bậc $\geq 2$ suy ra từ mệnh đề 4, trong đó lấy $r = 1$; khi P có bậc 1, tức là có dạng $T - c$ với $c \in m_A$, thì hệ quả là ngay lập tức.

#### Mệnh đề 5 {#ac-viii-s5-prop-5 .statement}

*Cho A là một miền nguyên, với trường phân thức K, và cho L là một mở rộng đại số có bậc hữu hạn của K. Ta ký hiệu B là bao đóng nguyên của A trong L và p là một iđêan nguyên tố của A.

Giả sử rằng vành địa phương $A_p$ là Noether và chính quy; cho t là một phần tử của L sao cho $L = K(t)$ và giả sử rằng tồn tại trong $A[T]$ một phần tử P, một đa thức Eisenstein đối với $pA_p$, có t là một nghiệm.

a) Trong B tồn tại một iđêan nguyên tố q duy nhất nằm trên p.
b) Vành địa phương $B_q$ là Noether và chính quy, có cùng chiều với $A_p$.
c) Ta có $B_q = A_p[t]$.
d) Đồng cấu chính tắc của $A/p$ vào $B/q$ cảm sinh một đẳng cấu của các trường phân thức của các vành này.*

Đặt $C = A_p[t]$ và ký hiệu d là bậc của P. Theo mệnh đề 3 áp dụng cho vành $A_p$, đa thức Eisenstein P là bất khả quy trong $K[T]$ và $(1, t, ..., t^{d-1})$ là một cơ sở của L trên K, do đó cũng là một cơ sở của C trên $A_p$. Vì P là đơn nhất, hạt nhân của đồng cấu chính tắc từ $A_p[T]$ lên C bằng (P). Theo hệ quả của mệnh đề 4 ở trên, C do đó là một vành địa phương Noether chính quy có cùng chiều với $A_p$, iđêan cực đại $m_C$ của C được sinh bởi $p \cup \{ t \}$ và trường $\kappa_C$ là một mở rộng tầm thường của trường phân thức của $A/p$. Để chứng minh mệnh đề 5, do đó chỉ cần chỉ ra rằng tồn tại một iđêan nguyên tố q duy nhất của B nằm trên p, và rằng ta có $C = B_q$.

Đặt S = A − p. Ta biết (V, § 1, n° 5, mệnh đề 16) rằng bao đóng nguyên của

#### Hệ quả {#ac-viii-s5-n4-cor-2 .statement}

Giả sử rằng $A_p$ là một vành định giá rời rạc. Khi đó $B_q$ là một vành định giá rời rạc, t là một phần tử đồng nhất hóa của $B_q$, và ta có

$$
f(B_q/A_p) = 1 , \quad e(B_q/A_p) = [L : K]
$$

(VI, § 8, n° 1).

Thật vậy, các vành định giá rời rạc là các vành địa phương Noether chính quy có chiều 1; đặt d = [L : K], ta có $t^d \in m_A - m_A^2$, do đó $d = e(B_q/A_p)$. Ta có [\kappa_B : \kappa_A] = 1, do đó $f(B_q/A_p) = 1$.

#### Ví dụ 1 {#ac-viii-s5-n4-exa-1 .statement}

Đặt A = $\mathbf{Z}$ và L = $\mathbf{Q}(p^{1/d})$, trong đó p là một số nguyên tố và d là một số nguyên $\geqslant 2$. Gọi B là bao đóng nguyên của $\mathbf{Z}$ trong L. Vì đa thức $T^d - p$ của $\mathbf{Z}[T]$ là một đa thức Eisenstein đối với $p\mathbf{Z}_{(p)}$, tồn tại một iđêan nguyên tố q duy nhất của B nằm trên $p\mathbf{Z}$. Do đó tồn tại một định giá rời rạc chuẩn hóa duy nhất v của trường $\mathbf{Q}(p^{1/d})$ sao cho $v(p) > 0$; ta có [L : K] = v(p) = d, và B/q là một trường có p phần tử. Vành $B_q$ của định giá v bằng $\mathbf{Z}_{(p)}[p^{1/d}]$.

#### Ví dụ 2 {#ac-viii-s5-n4-exa-2 .statement}

Đặt A = $\mathbf{Z}$ và L = $R_{pf}(\mathbf{Q})$ trong đó p là một số nguyên tố và f là một số nguyên $\geqslant 1$ (xem A, V, p. 78). Do đó L = $\mathbf{Q}(\zeta)$ với $\zeta = \exp(2\pi i/p^f)$. Gọi B là bao đóng nguyên của $\mathbf{Z}$ trong L và P là đa thức của $\mathbf{Z}[T]$ sao cho

$$
P(T - 1) = (T^{p^f} - 1)/(T^{p^{f-1}} - 1) .
$$

Đặt d = p^f - p^{f-1}. Ta có P(\zeta - 1) = 0, P(0) = p và

$$
P(T - 1) \equiv (T - 1)^d \mod. p\mathbf{Z}[T] ,
$$

do đó P(T) $\equiv T^d$. Suy ra P là một đa thức Eisenstein đối với $p\mathbf{Z}_{(p)}$. Do đó tồn tại một iđêan nguyên tố q duy nhất của B nằm trên $p\mathbf{Z}$, và ta có $B_q = \mathbf{Z}_{(p)}[\zeta]$ ; hơn nữa, $\zeta - 1$ là một phần tử đồng nhất hóa của $B_q$ và ta có

$$
[L : K] = d = p^f - p^{f-1} .
$$

Nếu v là định giá chuẩn hóa duy nhất của $\mathbf{Q}(\zeta)$ sao cho $v(p) > 0$, ta có $v(p) = d$. Hơn nữa, trường B/q có p phần tử. Ta có thể chứng minh (xem p. 96, bài tập 13) rằng B bằng $\mathbf{Z}[\zeta]$.

\* 5. Cấu trúc của các vành địa phương Noether chính quy đầy đủ

Trong số này, ta sử dụng các định nghĩa và các kết quả từ chương IX.

Cho A là một vành địa phương Noether chính quy đầy đủ; gọi $p$ là đặc số của trường thặng dư $\kappa_A$ của nó, và phân biệt hai trường hợp.

A) $p = 0$. Khi đó (IX, § 3, no 3, định lý 1), tồn tại một trường con K của A sao cho phép chiếu chính tắc của A lên $\kappa_A$ cảm sinh một đẳng cấu của K lên $\kappa_A$. Áp dụng khi đó hệ quả 3 của định lý 1 của số 2 cho đại số trên K A, ta suy ra:

#### Mệnh đề 6 {#ac-viii-s5-prop-6 .statement}

Cho A là một vành địa phương Noether chính quy đầy đủ, có trường thặng dư $\kappa_A$ có đặc số 0. Đặt $n = \dim(A)$. Khi đó A đẳng cấu với vành các chuỗi lũy thừa hình thức $\kappa_A[[X_1, ..., X_n]]$.

B) $p \neq 0$. Một vành con Cohen của A là một vành con V bất kỳ của A là một $p$-vành sao cho $A = m_A + V$ (IX, § 2, no 2, định nghĩa 2). Vành V là địa phương; iđêan cực đại $m_V$ của nó được sinh bởi $p.1_V$; do đó ta có $m_A \cap V = m_V$ và đơn ánh chính tắc của V vào A xác định, qua phép chuyển sang thương, một đẳng cấu của trường $\kappa_V$ lên trường $\kappa_A$. Nếu $p.1_A = 0$, V là một trường có đặc số p. Ngược lại V là một vành định giá rời rạc mà trường phân thức của nó có đặc số không (IX, § 2, no 1, hệ quả 1 của mệnh đề 1). Người ta chứng minh (IX, no 2, định lý 1) rằng A có các vành con Cohen.

#### Ví dụ 3 {#ac-viii-s5-n4-exa-3 .statement}

Cho k là một trường có đặc số $p \neq 0$ và cho $n$ là một số nguyên dương. Vành các chuỗi hình thức $k[[X_1, ..., X_n]]$ là đầy đủ chính quy địa phương Noether, có chiều $n$, và k là một vành con Cohen của $k[[X_1, ..., X_n]]$.

#### Ví dụ 4 {#ac-viii-s5-n4-exa-4 .statement}

Cho V là một vành định giá rời rạc đầy đủ và cho $n$ là một số nguyên dương. Vành các chuỗi hình thức $V_n = V[[X_1, ..., X_n]]$ là đầy đủ chính quy địa phương Noether, có chiều $n + 1$, và V là một vành con Cohen của $V_n$.

#### Ví dụ 5 {#ac-viii-s5-n4-exa-5 .statement}

Ta giữ lại ký hiệu ở trên. Một đa thức P trong $V_n[T]$ có bậc $d \geq 2$ được gọi là đặc biệt nếu nó có dạng $T^d + \sum_{i=1}^d a_i T^{d-i}$, trong đó $a_1, ..., a_{d-1}$ thuộc $m_{V_n}$, $a_d$ thuộc $m_V + m_{V_n}^2$ nhưng không thuộc $m_{V_n}^2$. Đặc biệt, P là một đa thức Eisenstein đối với $m_{V_n}$. Đặt $A = V_n[T]/(P)$. Theo hệ quả của Mệnh đề 4 của No. 4, vành A là đầy đủ chính quy địa phương Noether, có chiều $n + 1$. Nếu t là lớp của T modulo (P), thì dãy $(1, t, ..., t^{d-1})$ là một cơ sở của $V_n$-môđun A, và $(X_1, ..., X_n, t)$ là một hệ tọa độ của A: thật vậy, tồn tại một phần tử đồng nhất $\pi$ của V sao cho $a_d \equiv \pi \mod. m_{V_n}^2$; vì ta cũng có
$$
a_d = -t(t^{d-1} + a_1 t^{d-2} + \cdots + a_{d-1}),
$$
nên có $\pi \in m_A^2$; vì $m_A$ được sinh bởi $\{\pi, X_1, ..., X_n, t\}$, điều này chứng minh mệnh đề của ta. Hơn nữa, V là một vành con Cohen của A, vì $\kappa_V$ được đồng nhất với $\kappa_{V_n}$, và $\kappa_{V_n}$ với $\kappa_A$ theo hệ quả của Mệnh đề 4 của No. 4.

#### Định lý 2 {#ac-viii-s5-thm-2 .statement}

Cho $A$ là một vành đầy đủ chính quy địa phương Noether mà trường thặng dư của nó có đặc số $\neq 0$, và cho $V$ là một vành con Cohen của $A$. Đặt $n = \dim(A)$.

a) Giả sử rằng $V$ là một trường. Khi đó $V$-đại số $A$ đẳng cấu với đại số các chuỗi hình thức $V[[X_1, ..., X_n]]$.

b) Giả sử rằng $V$ là một vành định giá rời rạc đầy đủ và ta có $m_V \not\subset m_A^2$. Khi đó $V$-đại số $A$ đẳng cấu với đại số các chuỗi hình thức $V[[X_1, ..., X_{n-1}]]$.

c) Giả sử rằng $V$ là một vành định giá rời rạc đầy đủ và ta có $m_V \subset m_A^2$. Khi đó tồn tại một đa thức đặc biệt $P$ trong $V[[X_1, ..., X_{n-1}]] [T]$ và một $V$-đẳng cấu của $A$ lên $V[[X_1, ..., X_{n-1}]] [T]/(P)$.

Mệnh đề a) suy ra ngay từ Hệ quả 3 của Định lý 1 của No. 2.

Ta chứng minh b). Cho $(x_1, ..., x_m)$ là một dãy các phần tử của $m_A$, và cho $\varphi_0$ là đồng cấu từ $V[X_1, ..., X_m]$ vào $A$ trùng với đồng nhất trên $V$ và gửi $X_i$ tới $x_i$ với $1 \leq i \leq m$. Nếu $a$ là iđêan của $V[X_1, ..., X_m]$ sinh bởi $X_1, ..., X_m$, ta có $\varphi_0(a) \subset m_A$, do đó $\varphi_0$ mở rộng bởi tính liên tục thành một đồng cấu $\varphi$ từ $V_m = V[[X_1, ..., X_m]]$ vào $A$. Cho $\pi$ là một phần tử đồng nhất hóa của $V$. Theo Hệ quả 2 của Định lý 1 của No. 2, $\varphi$ là một đẳng cấu từ $V_m$ lên $A$ khi và chỉ khi $(\pi, x_1, ..., x_m)$ là một hệ tọa độ của $A$. Nhưng ánh xạ chính tắc của $m_V/m_V^2$ vào $m_A/m_A^2$ là đơn ánh, vì ta có $m_V \not\subset m_A^2$ và $m_V/m_V^2$ có hạng 1 trên $\kappa_V$. Do đó $m_A/(m_V + m_A^2)$ có hạng $n - 1$ và $(\pi, x_1, ..., x_m)$ là một hệ tọa độ của $A$ khi và chỉ khi các lớp của $x_i$ tạo thành một cơ sở của $m_A/(m_V + m_A^2)$ trên $\kappa_V$. Suy ra b).

Ta chứng minh c). Cho $(y_1, ..., y_n)$ là một hệ tọa độ của $A$. Như trên, đặt $V_n = V[[Y_1, ..., Y_n]]$ và xét đồng cấu $\varphi$ từ $V_n$ vào $A$ trùng với đồng nhất trên $V$ và gửi $Y_i$ tới $y_i$ với $1 \leq i \leq n$. Khi đó $\mathrm{gr}(\varphi)$ là toàn ánh, do đó $\varphi$ là toàn ánh (III, § 2, no 8, Hệ quả 2 của Định lý 1). Hạt nhân $p$ của $\varphi$ là một iđêan nguyên tố của $V_n$; vì ta có

$$
\dim(V_n) = n + 1 = \dim(V_n/p) + 1,
$$

iđêan nguyên tố $p$ có chiều cao 1 (§ 1, no 3, Mệnh đề 8). Nhưng vành $V_n$ là vành phân tích thành thừa số duy nhất theo Mệnh đề 8 của VII, § 3, no 9; do đó, iđêan $p$ là chính (VII, § 3, no 2, Định lý 1).

Cho $R$ là một phần tử sinh của iđêan $p$ của $V_n$. Theo Bổ đề 3 của VII, § 3, No. 7, tồn tại các số nguyên $u(1), ..., u(n-1)$ lớn hơn hoặc bằng 1, và một đẳng cấu $\sigma$ của $V[[X_1, ..., X_{n-1}, T]]$ lên $V_n$ sao cho

$$
\begin{align*}
\sigma(X_i) &= Y_i + Y_n^{u(i)} \quad \text{cho } 1 \leq i < n \\
\sigma(T) &= Y_n
\end{align*}
$$

và sao cho $\sigma^{-1}(R) = Q$ thỏa mãn $Q(0, ..., 0, T) \neq 0$. Hơn nữa, theo định lý chuẩn bị (VII, § 3, No. 8, Mệnh đề 6), tồn tại một đa thức P trong V[[X_1, ..., X_{n-1}]] [T] có dạng

$$
P = T^d + \sum_{i=1}^d a_i(X_1, ..., X_{n-1}) T^{d-i},
$$

sinh cùng một iđêan với Q trong V[[X_1, ..., X_{n-1}, T]], và sao cho $a_i(0, ..., 0) \in m_V$ với $1 \leq i \leq d$. Suy ra rằng A là V-đẳng cấu với V[[X_1, ..., X_{n-1}, T]]/(P). Nhưng V[[X_1, ..., X_{n-1}, T]] là tổng trực tiếp của iđêan (P) và của V[[X_1, ..., X_{n-1}]]-môđun có cơ sở 1, T, ..., $T^{d-1}$ (VII, § 3, No. 8, Mệnh đề 5); do đó A là V-đẳng cấu với V[[X_1, ..., X_{n-1}]] [T]/(P).

Đặt C = V[[X_1, ..., X_{n-1}]] và ký hiệu bởi α lớp của $a_d(X_1, ..., X_{n-1})$ modulo $m_C^2$. Ta có $\kappa_V = \kappa_C = \kappa_A$. Theo Mệnh đề 4 của No. 4, hạt nhân của đồng cấu chính tắc từ $m_C/m_C^2$ vào $m_A/m_A^2$ bằng $\kappa_C \alpha$. Vì ảnh của $m_V/m_V^2$ trong $m_A/m_A^2$ là không và $m_V/m_V^2$ có hạng 1 trên $\kappa_C$, suy ra rằng $a_d$ thuộc $m_V + m_C^2$, nhưng không thuộc $m_C^2$. Do đó, đa thức P là đặc biệt, như cần chứng minh.

\* Nhận xét. — Cho k là một trường, A là một đại số đầy đủ chính quy địa phương Noether trên k. Khi $\kappa_A$ không phải là một mở rộng tách được của k, nói chung không đúng rằng A là đẳng cấu như một k-đại số với $\kappa_A[[T_1, ..., T_n]]$ trong đó $n = \dim(A)$ (p. 98, Bài tập 29). \*

## BÀI TẬP {#ac-viii-s5-exercises}

Xem các [bài tập cho § 5](exercises/s5/).
