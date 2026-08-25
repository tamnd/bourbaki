---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 16
section_title: Differential criteria of separability
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.127-A V.137, A V.177-A V.180
pdf_pages: 0241-0251, 0291-0294
extraction: ocr
subsections:
    - "no": 1
      title: 'Extension of derivations : the case of rings'
      page: 127
      pdf_page: 241
    - "no": 2
      title: 'Extension of derivations: the case of fields'
      page: 0
      pdf_page: 242
    - "no": 3
      title: Derivations in fields of characteristic zero
      page: 130
      pdf_page: 244
    - "no": 4
      title: Derivations in separable extensions
      page: 131
      pdf_page: 245
    - "no": 5
      title: The index of a linear mapping
      page: 132
      pdf_page: 246
    - "no": 6
      title: Differential properties of finitely generated extensions
      page: 133
      pdf_page: 247
    - "no": 7
      title: Separating transcendence bases
      page: 136
      pdf_page: 250
statements: 32
exercises: 9
content_sha256: aad149359b61de88af3cc28dc33dd42f6558d7a63633d2ee038a160bc21df963
translated_from: content/en/alg/V/16_s16_differential_criteria_of_separability.md
source_content_sha256: 9700b50da74a6fb09292a3200d612cf177fbdfc53c16974c386fb84910fa7680
translation_model: gpt-5-6-mini
translation_run: translate-vi-ff6e7523
glossary_version: 34
glossary_terms_sha256: e6a640852a52d6524eff23580a54838f4b60e17e809e9994419cac79cbe89543
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 16. CÁC TIÊU CHUẨN VI PHÂN CỦA TÍNH TÁCH ĐƯỢC

### 1. Mở rộng các đạo hàm : trường hợp các vành

Cho K là một vành giao hoán, A là một đại số giao hoán trên K và $x = (x_i)_{i \in I}$, một họ các phần tử của A. Ngoài ra, cho $A$ là một đạo hàm của K vào một A-môđun M, nói cách khác (III, p. 553) là một ánh xạ tuyến tính trên Z từ K vào M thỏa mãn quan hệ $\Delta(cc') = c \cdot \Delta(c') + c' \cdot \Delta(c)$ với $c, c'$ trong K. Với mỗi $i \in I$ cho $D_i$ là đạo hàm riêng theo $X_i$ trong vành đa thức $K[X_i]_{i \in I}$; đây là đạo hàm duy nhất của vành đó vào chính nó bằng không trên K và trên $X_j$ với $j \in I - \{i\}$, và nhận giá trị 1 trên $X_i$ (IV, p. 6). Với mọi đa thức $f = \sum_{a \in N^{(I)}} c_a \cdot X^\alpha$ trong $K[X_i]_{i \in I}$, ta ký hiệu $f^\Delta(x)$ là phần tử $\sum_{a \in N^{(I)}} x^\alpha \cdot A(c,)$ của M.

#### Mệnh đề 1 {#alg-v-s16-prop-1 .statement}

— Giả sử họ $x = (x_i)_{i \in I}$, sinh đại số trên K A. Cho $(m_i)_{i \in I}$, là một họ các phần tử của M và $(f_\lambda)_\lambda$, một họ các đa thức sinh iđêan $a$ gồm mọi đa thức $f \in K[X_i]_{i \in I}$ sao cho $f(x) = 0$. Để tồn tại một đạo hàm D của A vào M sao cho $D(c \cdot 1) = \Delta(c)$ với mọi $c \in K$ và $D(x_i) = m_i$ với mọi $i \in I$ thì điều kiện cần và đủ là

$$
f_\lambda^\Delta(x) + \sum_{i \in I} D_i f_\lambda(x) \cdot m_i = 0 \quad \text{với mọi} \quad \lambda \in A .
$$

Nếu điều này đúng, đạo hàm D là duy nhất và thỏa mãn

$$
D(f(x)) = f^\Delta(x) + \sum_{i \in I} D_i f(x) \cdot m_i \quad \text{với mọi} \quad f \in K[X_i]_{i \in I}
$$

Đặt $E = K[X_i]_{i \in I}$ và ký hiệu $\varphi$ là đồng cấu trên K của E lên A biến $X_i$ thành $x_i$ với mọi $i \in I$; do đó ta có $\varphi(f) = f(x)$ với mọi $f \in E$. Ta xét M như một E-môđun nhờ đồng cấu $\varphi : E \to A$ và định nghĩa một ánh xạ $D'$ từ E vào M bởi $D'(f) = f^\Delta(x) + \sum_{i \in I} D_i f(x) \cdot m_i$ (chú ý rằng họ $(D_i f)_{i \in I}$ có giá hữu hạn với mỗi $f \in E$). Hiển nhiên $D'$ là đạo hàm duy nhất của E vào M mở rộng A và biến $X_i$ thành $m_i$ với mỗi $i \in I$.

Cho D là một đạo hàm của A vào M sao cho $D(c \cdot 1) = \Delta(c)$ với mọi $c \in K$ và $D(x_i) = m_i$ với mọi $i \in I$. Khi đó $D \circ \varphi$ là một đạo hàm của E vào M mở rộng A và biến $X_i$ thành $m_i$ với mọi $i \in I$. Do đó ta có $D \circ \varphi = D'$, tức là quan hệ (2) đúng. Điều này chứng minh tính duy nhất của D; hơn nữa (1) là hệ quả của $f, (x) = 0$ và (2).

Ngược lại giả sử rằng (1) đúng; nói cách khác, ta có $D'(f_\lambda) = 0$ với mọi $\lambda \in A$. Cho $f \in a$; tồn tại một họ có giá hữu hạn $(q_\lambda)_{\lambda \in \Lambda}$ trong $E$ sao cho $f = \sum_{\lambda \in \Lambda} q_\lambda \cdot f_\lambda$. Ta có
$$
D'(f) = \sum_{\lambda \in \Lambda} [f_\lambda(x) \cdot D'(q_\lambda) + q_\lambda(x) \cdot D'(f_\lambda)]
$$
do đó $D'(f) = 0$ vì $f_\lambda(x)$ và $D'(f_\lambda)$ đều bằng không với mọi $\lambda \in A$. Vì $D'$ triệt tiêu trên $a$, tồn tại một ánh xạ $Z$-tuyến tính $D$ từ $A$ vào $M$ sao cho $D' = D \circ \varphi$; rõ ràng $D$ là đạo hàm cần tìm của $A$ vào $M$.

### 2. Mở rộng các đạo hàm: trường hợp các trường

Cho $K, L$ và $M$ là các trường sao cho $K \subset L \subset M$. Theo Mệnh đề 21 (III, p. 572) ta có một dãy khớp của các không gian $M$-vectơ
$$
(\mathrm{E}_{K,L,M}) \quad \Omega_K(L) \otimes_L M \xrightarrow{\alpha} \Omega_K(M) \xrightarrow{\beta} \Omega_L(M) \to 0 ;
$$
các ánh xạ $M$-tuyến tính $\alpha$ và $\beta$ được đặc trưng bởi các hệ thức
$$
(3) \quad \alpha(d_{L/K} x \otimes 1) = d_{M/K} x \quad \text{với } x \in L \\
(4) \quad \beta(d_{M/K} y) = d_{M/L} y \quad \text{với } y \in M
$$

Cho $V$ là một không gian $M$-vectơ, ký hiệu $D_K(M, V)$ là không gian vectơ của các đạo hàm $K$ của $M$ với giá trị trong $V$ và tương tự đưa vào $D_K(L, V)$ và $D_L(M, V)$. Theo III, p. 571, Biểu đồ (42) và III, p. 572, Biểu đồ (44), ta có một biểu đồ giao hoán của các đồng cấu của các không gian vectơ
$$
\begin{array}{ccccccccc}
0 \to \mathrm{Hom}_M(\Omega_L(M), V) & \xrightarrow{\mathrm{Hom}(\beta, 1)} & \mathrm{Hom}_M(\Omega_K(M), V) & \xrightarrow{\mathrm{Hom}(\alpha, 1)} & \mathrm{Hom}_M(\Omega_K(L) \otimes_L M, V) \\
\downarrow & & \downarrow & & \downarrow \\
0 \to \mathrm{Der}_L(M, V) & \xrightarrow{i_V} & \mathrm{Der}_K(M, V) & \xrightarrow{r_V} & \mathrm{Der}_K(L, V),
\end{array}
$$
trong đó các mũi tên đứng là các đẳng cấu, $i_V$ là đơn ánh chính tắc và $r_V$ là ánh xạ hạn chế.

Do đó từ II, p. 299, Định lý 5 và II, p. 301, Mệnh đề 10 ta thu được mệnh đề sau:

#### Mệnh đề 2 {#alg-v-s16-prop-2 .statement}

— *Các điều kiện sau là tương đương*:
a) *Ánh xạ $\alpha$ là đơn ánh*.
b) *Mọi đạo hàm $K$ của $L$ vào $M$ đều mở rộng được thành một đạo hàm $K$ của $M$ vào $M$*.
c) *Mọi đạo hàm $K$ của $L$ vào một không gian $M$-vectơ $V$ đều mở rộng được thành một đạo hàm $K$ của $M$ vào $V$*.

#### Mệnh đề 3 {#alg-v-s16-prop-3 .statement}

— *Cho $K$ là một trường, $L$ là một mở rộng thuần của $K$ và $(x_i)_{i \in I}$ là một cơ sở thuần của $L$* (V, p. 106, Định nghĩa 2).

a) Cho $V$ là một không gian vectơ trên $L$, $A$ là một đạo hàm của $K$ vào $V$ và $(v_i)_{i \in I}$ là một họ các phần tử của $V$. Tồn tại duy nhất một đạo hàm $D$ của $L$ vào $V$, mở rộng $A$ và sao cho $D(x_i) = v_i$ với mọi $i \in I$.

b) Không gian $L$-vectơ $\Omega_K(L)$ của các vi phân $K$ của $L$ có họ $(dx_i)_{i \in I}$ làm cơ sở.

Mệnh đề b) đã được chứng minh trong IV, p. 23 và Mệnh đề a) suy ra trực tiếp từ điều này.

#### Hệ quả {#alg-v-s16-n2-cor-1 .statement}

— Cho $P$ là một trường con của $K$. Ánh xạ chính tắc $\alpha$ của $\Omega_P(K) \otimes_K L$ vào $\Omega_P(L)$ là đơn ánh và họ $(d_{L/P} x_i)_{i \in I}$, là một cơ sở (trên $L$) của một không gian con của $\Omega_P(L)$ bổ sung cho ảnh của $\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$.

Mệnh đề 3, a) cho thấy mọi $P$-đạo hàm của $K$ vào một không gian vectơ $V$ trên $L$ đều mở rộng thành một $P$-đạo hàm của $L$ vào $V$; tính đơn ánh của $\alpha$ sau đó suy ra từ Mệnh đề 2. Mệnh đề thứ hai của hệ quả suy ra từ tính chính xác của dãy $(\mathbf{E}_{P,K,L})$ và Mệnh đề 3, b) (có tính đến Công thức (4)).

#### Mệnh đề 4 {#alg-v-s16-prop-4 .statement}

— Cho $K$ là một trường, $L$ là một mở rộng đại số tách được của $K$ và $V$ là một không gian vectơ trên $L$.

a) Mọi $K$-đạo hàm của $L$ vào $V$ đều là không.

b) Nếu $A$ là một đạo hàm của $K$ vào $V$, tồn tại duy nhất một đạo hàm $D$ của $L$ vào $V$ mở rộng $A$.

Cho $D$ là một $K$-đạo hàm của $L$ vào $V$. Nếu $E$ là một mở rộng con của $L$ có bậc hữu hạn trên $K$, thì $K$-đại số $E$ là étale, và do đó $\Omega_K(E) = 0$ ($V$, p. 33, Th. 3), do đó $D|_E = 0$ theo tính chất phổ quát của $\Omega_K(E)$ (III, p. 569). Vì $L$ là hợp của một họ các mở rộng con có bậc hữu hạn trên $K$, ta có $D = 0$, do đó $a)$.

Cho $A$ là một đạo hàm của $K$ vào $V$. Nếu $D'$ và $D''$ là hai mở rộng của $A$ thành một đạo hàm của $L$ vào $V$, thì hiệu $D' - D''$ là một $K$-đạo hàm của $L$ vào $V$; do đó nó bằng không theo $a)$ và suy ra $D' = D''$.

Còn phải chứng minh sự tồn tại của một mở rộng của $A$. Bổ đề Zorn (E, III, p. 20) suy ra sự tồn tại của một mở rộng cực đại $D_0$ của $A$ thành một đạo hàm xác định trên một trường con $L_0$ của $L$ chứa $K$.

Cho $x$ thuộc $L$ và $g$ là đa thức tối tiểu của $x$ trên $L_0$. Vì $L$ là đại số và tách được trên $K$, $x$ là đại số và tách được trên $L_0$ ($V$, p. 39, Mđ. 6 và p. 39, Hệ quả 2); do đó $x$ là nghiệm đơn của $g$ ($V$, p. 39, Mđ. 5), do đó $g'(x) \neq 0$ (IV, p. 17, Mđ. 7). Nếu ta định nghĩa $g^{D_0}(x)$ như trong $V$, p. 127, khi đó tồn tại một phần tử $u$ của $V$ sao cho $g^{D_0}(x) + g'(x) \cdot u = 0$; theo Mđ. 1 (V, p. 127), tồn tại một đạo hàm $D$ của $L_0(x)$ vào $V$ mở rộng $D_0$ và sao cho $D(x) = u$. Do tính cực đại của $(L_0, D_0)$, ta có $L_0(x) = L_0$, do đó $x \in L_0$. Vì $x$ là tùy ý, ta kết luận rằng $L_0 = L$.

#### Hệ quả 1 {#alg-v-s16-prop-4-cor-1 .statement}

— Ta có $\Omega_K(L) = 0$ nếu $L$ là đại số và tách được trên $K$.

Hệ quả này suy ra từ Mđ. 4, a) vì không gian vectơ $L$ $\Omega_K(L)$ được sinh bởi ảnh của đạo hàm $K$ chính tắc $d_{L/K} : L \to \Omega_K(L)$.

#### Hệ quả 2 {#alg-v-s16-prop-4-cor-2 .statement}

— *Nếu L là một mở rộng đại số và tách được của một trường K, ánh xạ chính tắc $\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$ là một đẳng cấu với mọi trường con P của K.*

Ánh xạ $\alpha$ là đơn ánh theo Mđ. 2 (V, p. 128) và Mđ. 4, *b*); vì $\Omega_K(L)$ quy về 0 (Hệ quả 1), tính chính xác của dãy $(E_{P.K.L})$ suy ra rằng $\alpha$ là toàn ánh.

#### Hệ quả 3 {#alg-v-s16-prop-4-cor-3 .statement}

— *Cho E là một mở rộng của một trường K và D là một đạo hàm của E vào E, ánh xạ K vào K. Nếu L là một mở rộng con của E đại số và tách được trên K, thì $D(L) \subset L$.*

Gọi A là đạo hàm của K vào L trùng với D trên K. Theo Mđ. 4 (V, p. 129), tồn tại một đạo hàm D' của L vào L mở rộng A. Bây giờ ta có thể xem D' và hạn chế D'' của D trên L như các đạo hàm của $L$ vào E; vì chúng trùng nhau trên K, ta có $D' = D''$ theo Mđ. 4, do đó

$$
D(L) = D''(L) = D'(L) \subset L .
$$

#### Nhận xét {#alg-v-s16-n2-rem-1 .statement}

— 1) Sau này (V, p. 131, Hệ quả 3 và p. 135, Hệ quả 2) ta sẽ chứng minh đảo lại của Hệ quả 1 của Mđ. 4.

2) Mọi mở rộng đại số của một trường nguyên tố đều tách được (V, p. 37, Hệ quả). Vì mọi đạo hàm của một trường nguyên tố đều bằng không, nên mọi đạo hàm của một mở rộng đại số của một trường nguyên tố đều bằng không (Mđ. 4).

### 3. Các đạo hàm trong các trường có đặc số không

#### Định lý 1 {#alg-v-s16-thm-1 .statement}

— *Cho K là một trường có đặc số 0, L là một mở rộng của K và V là một không gian vectơ trên L. Gọi A là một đạo hàm của K vào V, $(x_i)_{i \in I}$, là một cơ sở siêu việt của L trên K và $(u_i)_{i \in I}$, là một họ các phần tử của V. Khi đó tồn tại duy nhất một đạo hàm D của L vào V mở rộng A và sao cho $D(x_i) = u_i$ với mọi $i \in I$.*

Đặt $E = K(x_i)_{i \in I}$; Mđ. 3 (V, p. 128) chỉ ra rằng A mở rộng thành một đạo hàm duy nhất $D_0$ của E vào V sao cho $D_0(x_i) = u_i$ với mọi $i \in I$. Trường $L$ là một mở rộng đại số của E và vì L có đặc số 0, L tách được trên E (V, p. 37, Hệ quả). Do đó (V, p. 129, Mđ. 4) $D_0$ mở rộng thành một đạo hàm duy nhất D của $L$ vào V.

#### Hệ quả 1 {#alg-v-s16-thm-1-cor-1 .statement}

— *Mọi đạo hàm của K vào V đều mở rộng thành một đạo hàm của L vào V*

#### Hệ quả 2 {#alg-v-s16-thm-1-cor-2 .statement}

— *Cho E là một mở rộng con của L và U là không gian con-vectơ trên L của $\Omega_K(L)$ được sinh bởi các vi phân của các phần tử của E. Đối với một phần tử x, điều kiện x đại số trên E là cần và đủ để $dx \in U$.*

Với mỗi $y \in L$ đặt D(y) là lớp thặng dư của $dy$ mod U. Khi đó D là một đạo hàm E của L vào $\Omega_K(L)/U$. Vì K có đặc số 0, mọi mở rộng đại số của E đều tách được (V, p. 37, Hệ quả) ; nếu $x \in L$ là đại số trên E, ta có $Dx = 0$ theo Mệnh đề 4 (V, p. 129), nghĩa là $dx \in U$.

Nếu $x \in L$ là siêu việt trên $E$, tồn tại một đạo hàm E $A$ của $E(x)$ vào $L$ sao cho $\Delta(x) = 1$ ($V$, p. 128, Mệnh đề 3); theo Định lý 1, $A$ mở rộng thành một đạo hàm E D của $L$ vào L. Gọi $\varphi$ là dạng tuyến tính trên $\Omega_K(L)$ sao cho $D = \varphi \circ d$; ta có $\varphi(dy) = 0$ với $y \in E$ và $\varphi(x) = 1$, do đó $dx \notin U$.

#### Hệ quả 3 {#alg-v-s16-thm-1-cor-3 .statement}

— *Đối với một phần tử x của L, để x đại số trên K là điều kiện cần và đủ để $dx = 0$ trong $\Omega_K(L)$. Đặc biệt, để L là một mở rộng đại số của K là điều kiện cần và đủ để $\Omega_K(L) = 0$.
Điều này suy ra ngay lập tức từ Hệ quả 2 của Định lý 1 khi lấy $E = K$.

#### Hệ quả 4 {#alg-v-s16-thm-1-cor-4 .statement}

— *Cho K, L và M là các trường có đặc số 0 sao cho $K \subset L \subset M$: khi đó ánh xạ chính tắc $a : \Omega_K(L) \otimes_L M \to \Omega_K(M)$ là đơn ánh.
Điều này suy ra ngay lập tức từ Hệ quả 1 và $V$, p. 128, Mệnh đề 2.

#### Định lý 2 {#alg-v-s16-thm-2 .statement}

— *Cho K là một trường có đặc số 0, L một mở rộng của K và $(x_i)_{i \in I}$, một họ các phần tử của L.
a) Để $(x_i)_{i \in I}$ là tự do đại số trên K là điều kiện cần và đủ để các vi phân $dx_i$ (với $i \in I$) trong $\Omega_K(L)$ là tự do tuyến tính trên L.
b) Để L là đại số trên $K(x_i)_{j \in I}$ là điều kiện cần và đủ để các vi phân $dx_i$, với $i \in I$ sinh không gian vectơ $\Omega_K(L)$ trên L.
c) Để $(x_i)_{i \in I}$ là một cơ sở siêu việt của L trên K là điều kiện cần và đủ để họ $(dx_i)_{i \in I}$ là một cơ sở của $\Omega_K(L)$ trên L.
Với mọi $i \in I$ đặt $E_i$ là trường con $K(x_j)_{j \in I, j \neq i}$ của L. Đối với họ $(x_i)_{i \in I}$, để là tự do đại số trên K là điều kiện cần và đủ ($V$, p. 108, Mệnh đề 5) để $x_i$ siêu việt trên $E_i$ với mỗi $i \in I$. Theo Hệ quả 2 của Định lý 1, điều này có nghĩa là với mỗi $i \in I$ vi phân $dx_i$ không là một tổ hợp tuyến tính với các hệ số trong L của các vi phân $dx_j$ với $j \neq i$ trong I; điều kiện sau này chỉ có nghĩa là họ $(dx_i)_{i \in I}$ là tự do trên L, do đó a).
Mệnh đề b) suy ra ngay lập tức từ Hệ quả 2 của Định lý 1 và c) là một hệ quả của a) và b).

#### Hệ quả {#alg-v-s16-n3-cor-1 .statement}

— *Ta có $[\Omega_K(L) : L] = \operatorname{tr} \cdot \deg_K L$ khi K có đặc số 0.

### 4. Các đạo hàm trong các mở rộng tách được

Chúng ta đã thấy ($V$, p. 122, Đl. 1) rằng mọi mở rộng $L$ của một trường $K$ có đặc số 0 đều tách được; hơn nữa, mọi đạo hàm của K vào một không gian vectơ trên $L$ khi đó mở rộng được thành một đạo hàm của $L$ ($V$, p. 130, Hệ quả 1). Nói chung hơn ta có mệnh đề sau:

#### Định lý 3 {#alg-v-s16-thm-3 .statement}

— *Cho K là một trường và L là một mở rộng của K. Để L tách được trên K thì điều kiện cần và đủ là mọi đạo hàm của K vào một không gian L-vectơ đều phải mở rộng được thành một đạo hàm của L.
Ta có thể giả sử rằng K có đặc số $\neq 0$. Trước hết giả sử rằng L tách được trên K. Cho $V$ là một không gian vectơ trên L và $A$ là một đạo hàm của K vào $V$. Theo tiêu chuẩn của Mac

Lane (V, p. 124, Nhận xét), các trường $L^p$ và $K$ rời nhau tuyến tính trên $K^p$. Vì $A$ là một ánh xạ tuyến tính $K^p$ của $K$ vào $V$, nó mở rộng một cách duy nhất thành một ánh xạ tuyến tính $L^p$ $A'$ của $K[L^p] = K(L^p)$ vào $V$. Rõ ràng rằng $A'$ là một đạo hàm của $K(L^p)$ vào $V$ triệt tiêu trên $L^p$; do đó nó mở rộng (V, p. 103, Hệ quả 3) thành một đạo hàm của $L$ vào $V$.

Ngược lại, giả sử rằng mọi đạo hàm của $K$ với các giá trị trong $L$ đều mở rộng được thành một đạo hàm của $L$ vào $L$. Cho $B$ là một p-cơ sở của $K$ (V, p. 99) và cho $A$ là tập hợp các họ $(\alpha_h)_{h \in R}$ có giá hữu hạn gồm các số nguyên giữa $()$ và $p - 1$. Với mỗi $b \in B$ tồn tại một đạo hàm $\Delta_b$ của $K$ vào $K$ được đặc trưng bởi $\Delta_b(b') = \delta_{bb'}$ (ký hiệu Kronecker) với mỗi $b' \in B$ (V, p. 103). Theo giả thiết tồn tại với mỗi $b \in B$ một đạo hàm $D_b$ của $L$ vào $L$ mở rộng $\Delta_b$. Ta có $D_b(b') = \delta_{bb'}$ với $b, b'$ trong $B$, điều này chứng minh rằng trong $\Omega_{1/p}(L)$ các vi phân $db$ (với $b \in B$) độc lập tuyến tính trên $L$. Vì vậy (V, p 102, Đl. 1), $B$ là p-tự do trên $L^p$. Suy ra (V, p. 98, Mđề 1 và p. 124, Nhận xét) rằng mở rộng $L$ của $K$ là tách được.

#### Hệ quả {#alg-v-s16-n4-cor-1 .statement}

— *Nếu $L$ là một mở rộng tách được của $K$, ánh xạ chính tắc $\alpha_p : \Omega_p(K) \otimes_K L \to \Omega_p(L)$ là đơn ánh với mọi trường con $P$ của $K$. Ngược lại, nếu tồn tại một trường con hoàn hảo $P$ của $K$ (chẳng hạn trường nguyên tố con của $K$) sao cho ánh xạ $\alpha_p$ là đơn ánh, thì $L$ là tách được trên $K$.*

Mệnh đề thứ nhất suy ra từ Mệnh đề 2 (V, p. 128) và Định lý 3. Ngược lại, cho $P$ là một trường con hoàn hảo của $K$; ta có $P = P^p \subset K^p$, do đó mọi đạo hàm của $K$ vào một không gian vectơ $L$ đều là một $P$-đạo hàm; mệnh đề thứ hai của hệ quả nay suy ra từ Hệ quả 2 (V, p. 130) và Định lý 3.

### 5. Chỉ số của một ánh xạ tuyến tính

Cho $L$ là một trường $^1$, cho $U$ và $V$ là hai không gian vectơ $^2$ trên $L$ và $f : U \to V$ là một ánh xạ $L$-tuyến tính; $f$ được gọi là có *chỉ số hữu hạn* nếu hạt nhân $N$ và đối hạt nhân $C$ của $f$ có chiều hữu hạn, và số nguyên

$$
\chi(f) = [C : L] - [N : L]
$$

được gọi là *chỉ số* của $f$.

#### Bổ đề 1 {#alg-v-s16-lem-1 .statement}

— *Cho $U$ và $V$ là hai không gian vectơ có chiều hữu hạn trên một trường $L$. Mọi ánh xạ tuyến tính $f : U \to V$ đều có một chỉ số bằng $[V : L] - [U : L]$.*

Cho $N$ là hạt nhân, $I$ là ảnh và $C$ là đối hạt nhân của $f$. Ta có $C = V/I$ và $I$ đẳng cấu với $U/N$; do đó ta có $[U : L] = [N : L] + [I : L]$ và $[V : L] = [C : L] + [I : L]$, do đó có kết quả.

$^1$ Không nhất thiết giao hoán.
$^2$ Ở bên trái.

#### Bổ đề 2 {#alg-v-s16-lem-2 .statement}

Cho $f : U \to V$ và $g : V \to W$ là hai ánh xạ $L$-tuyến tính. Nếu $f$ và $g$ mỗi ánh xạ đều có một chỉ số, thì điều tương tự cũng đúng với $g \circ f$ và ta có

$$
\chi(g \circ f) = \chi(f) + \chi(g).
$$

Đặt $h = g \circ f$, và ký hiệu N, N', N'' lần lượt là các hạt nhân của f, g, h và C, C', C'' là các đối hạt nhân của chúng. Ta có $N \subset N'' \subset U$ và $f(N'') = f(U) \cap N'$; do đó tồn tại một ánh xạ tuyến tính $\bar{f} : N'' \to N'$ trùng với f trên N'' và có hạt nhân N. Ánh xạ chính tắc $\pi$ của V lên $C = V / f(U)$ cảm sinh một ánh xạ $\pi'$ từ N' vào C có hạt nhân là $f(U) \cap N' = \bar{f}(N'')$. Qua phép lấy thương, g xác định một ánh xạ $\bar{g}$ từ $C = V/f(U)$ vào $C'' = W/g(f(U))$ có hạt nhân rõ ràng là $(N' + f(U))/f(U) = \pi'(N')$. Cuối cùng, ánh xạ chính tắc $\rho$ của $C'' = W/g(f(U))$ lên $C' = W/g(V)$ có hạt nhân $g(V)/g(f(U)) = \bar{g}(C)$. Tóm lại, ta đã chứng minh tính khớp của dãy

$$
0 \to N \xrightarrow{i} N'' \xrightarrow{\bar{f}} N' \xrightarrow{\pi'} C \xrightarrow{\bar{g}} C'' \xrightarrow{\rho} C' \to 0
$$

(trong đó i là đơn ánh chính tắc của N vào N").

![Biểu đồ cho thấy các quan hệ giữa N, N', N'', U, V, W, C, C', C'', với các mũi tên chỉ các ánh xạ và hạt nhân](../images/fig_1.png)

Hình 1

Theo giả thiết N, N', C và C' có số chiều hữu hạn; do đó N'' và C cũng có tính chất ấy. Theo Hệ quả 2 (II, p. 295), ta có

$$
[N : L] - [N'' : L] + [N' : L] - [C : L] + [C'' : L] - [C' : L] = 0
$$

do đó $\chi(h) = \chi(f) + \chi(g)$.

### 6. Các tính chất vi phân của các mở rộng sinh hữu hạn

#### Định lý 4 {#alg-v-s16-thm-4 .statement}

Cho P là một trường hoàn hảo, L là một mở rộng của P và K là một mở rộng con của L; ta giả sử rằng L là một mở rộng sinh hữu hạn của K. Khi đó ánh xạ L-tuyến tính chính tắc $a : \Omega_p(K) \otimes_K L \to \Omega_p(L)$ có chỉ số bằng bậc siêu việt của L trên K.

Nếu $E$ và $F$ là hai mở rộng con của $L$ sao cho $E \subset F$, ta ký hiệu $\alpha(F/E)$ là ánh xạ F-tuyến tính chính tắc từ $\Omega_p(E) \otimes_E F$ vào $\Omega_p(F)$ và khi nó được xác định, chỉ số của $\alpha(F/E)$ sẽ được ký hiệu là $d(F/E)$. Nếu $E, F$ và $G$ là ba mở rộng con của $L$ sao cho $E \subset F \subset G$, ta có một biểu đồ giao hoán

$$
\begin{array}{ccc}
\Omega_p(F) \otimes_F G & \xrightarrow{\alpha(G/F)} & \Omega_p(G) \\
\uparrow \alpha(F/E) \otimes_F \mathrm{Id}_G & & \uparrow \alpha(G/E) \\
(\Omega_p(E) \otimes_E F) \otimes_F G & \xrightarrow{\beta} & \Omega_p(E) \otimes_E G
\end{array}
$$

trong đó $\beta$ là đẳng cấu chính tắc được xác định trong Mệnh đề 2 (II, p. 278). Vì chỉ số rõ ràng là bất biến qua mở rộng vô hướng và chỉ số của một đẳng cấu bằng không, Bổ đề 2 ($V$, p. 133) cho thấy chỉ số $d(G/E)$ được xác định khi $d(F/E)$ và $d(G/F)$ được xác định, và khi đó

$$
d(G/E) = d(G/F) + d(F/E).
$$

Vì $L$ là một mở rộng sinh hữu hạn của $K$, Công thức (5) và Hệ quả của $V$, p. 111 cho thấy chỉ cần xét trường hợp tồn tại $x$ sao cho $L = K(x)$; hơn nữa, nếu $x$ là đại số trên $K$, tồn tại một lũy thừa $q$ của số mũ đặc số của $L$ sao cho $x^q$ là đại số tách được trên $K$ ($V$, p. 44, Mệnh đề 13). Do đó chỉ cần chứng minh đẳng thức $d(L/K) = \operatorname{tr} . \deg_K L$ trong ba trường hợp đặc biệt dưới đây:

$a)$ $x$ là siêu việt trên $K$: khi đó $a$ là đơn ánh và đối hạt nhân của nó có hạng 1 trên $L$ ($V$, p. 129, Cor.) ; do đó $d(L/K) = 1$ và cũng $\operatorname{tr} . \deg_K L = 1$.

$b)$ $x$ là đại số tách được trên $K$: khi đó $a$ là song ánh ($V$, p. 130, Cor. 2), do đó $d(L/K) = 0$; rõ ràng cũng $\operatorname{tr} . \deg_K L = 0$.

$c)$ *Trường $L$ có đặc số $p \neq 0$, $x \notin K$ và $x^p = a$ thuộc $K$*: đối hạt nhân $C$ của $a$ đẳng cấu với $\Omega_K(L)$, và vì $\{ x \}$ là một $p$-cơ sở của $L$ trên $K$, không gian $C$ có chiều 1 trên $L$ ($V$, p. 102, Đl. 1). Vì $a$ là một lũy thừa $p$-th trong $L$, ta có $d_{L/pa} = 0$ và hạt nhân của $a$ chứa không gian con $R$ của $U = \Omega_p(K) \otimes_K L$ sinh bởi $d_{K/pa} \otimes 1$. Với mỗi $y \in K$ cho $\Delta(y)$ là lớp thặng dư của $d_{K/p}y \otimes 1$ mod $R$; khi đó $A$ là một $P$-đạo hàm của $K$ vào $U/R$ sao cho $\Delta(a) = 0$. Mệnh đề 5 ($V$, p. 101) chỉ ra rằng $A$ mở rộng thành một $P$-đạo hàm $D$ của $L$ vào $U/R$. Do đó tồn tại một ánh xạ tuyến tính $L$ $\beta : \Omega_p(L) \to U/R$ sao cho $D = \beta \circ d_{L/P}$ và $\beta \circ a$ là ánh xạ chính tắc của $U$ lên $U/R$. Điều này chứng minh rằng $R$ là hạt nhân của $a$. Vì $P$ hoàn hảo, ta có $P(K^P) = K^p$, do đó $a \notin P(K^P)$ và cuối cùng $d_{K/pa} \neq 0$ ($V$, p. 103, Mệnh đề 6). Hạt nhân và đối hạt nhân của $a$ do đó có chiều 1, do đó $d(L/K) = 0$, và ta cũng có $\operatorname{tr} . \deg_K L = 0$.

#### Hệ quả 1 {#alg-v-s16-thm-4-cor-1 .statement}

— *Cho $L$ là một mở rộng sinh hữu hạn của một trường $K$ có bậc siêu việt $s$. Không gian vectơ $\Omega_K(L)$ có chiều $\geq s$ trên $L$, với đẳng thức xảy ra khi và chỉ khi $L$ tách được trên $K$.*

Gọi P là trường con nguyên tố của K. Gọi N là hạt nhân của α, khi đó theo tính chính xác của dãy $(\mathbf{E}_{P,K,L})$ (V, p. 128) và Định lý 4, ta có $[ \Omega_K(L) : L ] = s + [N : L]$; theo V, p. 132, Hệ quả, mở rộng L của K là tách được khi và chỉ khi $N = 0$. Hệ quả được suy ra.

#### Hệ quả 2 {#alg-v-s16-thm-4-cor-2 .statement}

— *Cho L là một mở rộng sinh hữu hạn của một trường K. Để L đại số và tách được trên K thì điều kiện cần và đủ là $\Omega_K(L) = 0$.* Điều này suy ra ngay lập tức từ Hệ quả 1.

#### Hệ quả 3 {#alg-v-s16-thm-4-cor-3 .statement}

— *Cho K là một trường có đặc số $p \neq 0$ và L là một mở rộng sinh hữu hạn của K có bậc siêu việt s. Nếu $[K : K^p]$ là hữu hạn, điều tương tự cũng đúng với $[L : L^p]$ và ta có $[L : L^p] = p^s$. $[K : K^p]$.* Gọi P là trường con nguyên tố của K. Nếu $[K : K^p]$ là hữu hạn, thì không gian vectơ $\Omega_P(K) = \Omega_{K^p}(K)$ có số chiều hữu hạn m trên K, và ta có $[K : K^p] = p^m$ (V, p. 103, Định lý 2); không gian vectơ $\Omega_P(K) \otimes_K L$ khi đó có số chiều hữu hạn m trên L. Hơn nữa, vì K có bậc hữu hạn trên $K^p$, trường $K(L^p)$ có bậc hữu hạn trên $K^p(L^p) = L^p$; vì trường L là một mở rộng sinh hữu hạn của K và là đại số trên $K(L^p)$, nó là một mở rộng có bậc hữu hạn của $K(L^p)$ (V, p. 18, Định lý 2); do đó ta kết luận rằng L có bậc hữu hạn trên $L^p$ (V, p. 10, Định lý 1). Khi đó $\Omega_P(L)$ là một không gian vectơ có số chiều hữu hạn n trên L và ta có $[L : L^p] = p^n$ (V, p. 103, Định lý 2). Theo Bổ đề 1 (V, p. 132) ánh xạ tuyến tính trên L $\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$ do đó có chỉ số $n - m$, do đó $n - m = s$ theo Định lý 4 (V, p. 133) và $p^n = p^s \cdot p^m$.

#### Nhận xét 1 {#alg-v-s16-n6-rem-1 .statement}

Cho K là một trường có đặc số $p \neq 0$ và L là một mở rộng của K. Ta có $\Omega_K(L) = 0$ khi và chỉ khi $L = K(L^p)$ (V, p. 103, Mệnh đề 6). Vì vậy nếu L là sinh hữu hạn trên K, thì nó là một mở rộng đại số và tách được khi và chỉ khi ta có $L = K(L^p)$. Khi L không là sinh hữu hạn trên K, kết quả này nói chung không còn đúng nữa như được chỉ ra bởi trường hợp L là bao đóng hoàn hảo của K.

#### Nhận xét 2 {#alg-v-s16-n6-rem-2 .statement}

Cho K là một trường, $F_1, \ldots, F_m$ là các đa thức trong $K[X_1, \ldots, X_n]$ và L là một mở rộng của K sinh bởi các phần tử $x_1, \ldots, x_n$. Giả sử rằng các đa thức $F_1, \ldots, F_m$ sinh iđêan của $K[X_1, \ldots, X_n]$ gồm tất cả các đa thức F sao cho $F(x_1, \ldots, x_n) = 0$. Từ Mệnh đề 1 (V, p. 127) và tính chất phổ quát của môđun vi phân (III, p. 569) ta dễ dàng suy ra kết quả sau: không gian vectơ $\Omega_K(L)$ trên L được sinh bởi $dx_1, \ldots, dx_n$; ta có các hệ thức

$$
\sum_{i=1}^n D_i F_j(x_1, \ldots, x_n) \cdot dx_i = 0 \quad \text{(với } 1 \leq j \leq m \text{)} ;
$$

cuối cùng nếu $u_1, \ldots, u_n$ là các phần tử của L sao cho $\sum_{i=1}^n u_i \cdot dx_i = 0$, tồn tại các phần tử $v_1, \ldots, v_m$ của L sao cho $u_i = \sum_{j=1}^m D_i F_j(x_1, \ldots, x_n) \ v_j$ với $1 \leq i \leq n$. Gọi r là hạng của ma trận $(D_i F_j(x_1, \ldots, x_n))$ có n hàng và m cột; gọi s là bậc siêu việt của $L$ trên $K$. Khi đó ta có $[ \Omega_K(L) : L ] = n - r$. Vì vậy mở rộng $L$ của $K$ là tách được khi và chỉ khi $r + s = n$ (Hệ quả 1). và nó là đại số và tách được khi và chỉ khi $r = n$ (Hệ quả 2).

### 7. Cơ sở siêu việt tách được

#### Định nghĩa 1 {#alg-v-s16-def-1 .statement}

*Một cơ sở siêu việt $B$ của một mở rộng $L$ của một trường $K$ được gọi là tách được nếu mở rộng đại số $L$ của $K(B)$ là tách được.*

Nếu $K$ có đặc số 0, mọi cơ sở siêu việt của $L$ trên $K$ đều tách được vì mọi mở rộng đại số của một trường có đặc số 0 đều tách được ($V$, p. 37, Hệ quả). Nếu một mở rộng có một cơ sở siêu việt tách được, thì nó tách được ($V$, p. 121, Mệnh đề 6 và p. 122, Mệnh đề 9). Định lý sau đây chỉ ra rằng mọi mở rộng tách được *sinh hữu hạn* đều có một cơ sở siêu việt tách được; hạn chế này là cốt yếu ($V$, p. 177, Bài tập 1).

#### Định lý 5 {#alg-v-s16-thm-5 .statement}

*Một cơ sở $K$ là một trường, $L$ là một mở rộng của $K$ và $(x_i)_{i \in I}$, là một họ các phần tử của $L$. Nếu họ $(x_i)_{i \in I}$, là một cơ sở siêu việt tách được của $L$ trên $K$, thì họ $(dx_i)_{i \in I}$, là một cơ sở của không gian vectơ $\Omega_K(L)$ trên $L$. Đảo lại đúng nếu $L$ là một mở rộng tách được sinh hữu hạn của $K$.

Đặt $M = K(x_i)_{i \in I}$, và ký hiệu $\alpha$ là ánh xạ chính tắc từ $\Omega_K(M) \otimes_M L$ vào $\Omega_K(L)$. Nếu $(x_i)_{i \in I}$ là một cơ sở siêu việt tách được của $L$ trên $K$, họ $(d_{M/K} x_i)_{i \in I}$, là một cơ sở của không gian $M$-vectơ $\Omega_K(M)$ ($V$, p. 128, Mệnh đề 3) và $\alpha$ là một đẳng cấu của các không gian $L$-vectơ vì $L$ là đại số và tách được trên $M$ ($V$, p. 130, Hệ quả 2). Vì $\alpha(d_{M/K} x_i \otimes 1) = d_{L/K} x_i$, họ $(d_{L/K} x_i)_{i \in I}$ do đó là một cơ sở của $\Omega_K(L)$ trên $L$.

Ngược lại, giả sử rằng $L$ là một mở rộng tách được sinh hữu hạn của $K$ và họ $(d_{L/K} x_i)_{i \in I}$ là một cơ sở của không gian vectơ $\Omega_K(L)$ trên $L$. Theo Hệ quả 1 của $V$, p. 134, bậc siêu việt của $L$ trên $K$ bằng chiều của $\Omega_K(L)$ trên $L$, do đó bằng lực lượng của $I$. Từ dãy khớp $(E_{K,M,L})$ ($V$, p. 128), ta có $\Omega_M(L) = 0$; vì $L$ là một mở rộng sinh hữu hạn của $M$, Hệ quả 2 của $V$, p. 135, cho thấy rằng $L$ là đại số và tách được trên $M = K(x_i)_{i \in I}$; vì bậc siêu việt của $L$ trên $K$ là hữu hạn và bằng lực lượng của $I$, họ $(x_i)_{i \in I}$ là một cơ sở siêu việt của $L$ trên $K$ ($V$, p. 110, Hệ quả 1).

#### Hệ quả {#alg-v-s16-n7-cor-1 .statement}

*Cho $L$ là một mở rộng tách được sinh hữu hạn của $K$ và cho $S$ là một tập con của $L$ sao cho $L = K(S)$. Khi đó tồn tại một cơ sở siêu việt tách được $B$ của $L$ trên $K$, được chứa trong $S$.*

Vì $\Omega_K(L)$ được sinh bởi các vi phân của các phần tử của $S$, tồn tại $s$ phần tử $x_1, \ldots, x_s$ của $S$ sao cho $(dx_1, \ldots, dx_s)$ là một cơ sở của $\Omega_K(L)$ trên $L$. Bây giờ chỉ cần áp dụng Định lý 5.

#### Nhận xét {#alg-v-s16-n7-rem-1 .statement}

— Cho $L$ là một mở rộng tách được sinh hữu hạn của một trường $K$ có đặc số $p \neq 0$; có thể tồn tại các cơ sở siêu việt của $L$ không tách được. Chỉ cần nhận thấy rằng $\{X^p\}$ là một cơ sở siêu việt của $K(X)$ nhưng $K(X)$ là một mở rộng căn $p$-của bậc $p$ của $K(X^p)$.

#### Mệnh đề 5 {#alg-v-s16-prop-5 .statement}

— *Cho L và M là hai mở rộng của một trường K được chứa trong một mở rộng đã cho và rời nhau đại số trên K. Nếu M tách được trên K, thì L(M) tách được trên L.*

Chỉ cần chứng minh rằng với mọi tập con hữu hạn S của M, $L(S)$ tách được trên L (V, p. 122, Mệnh đề 8). Cho S là một tập con hữu hạn của M. Vì trường $K(S)$ tách được trên K, nó có một cơ sở siêu việt tách được B (Hệ quả của Định lý 5). Vì L và M rời nhau đại số trên K, B là một cơ sở siêu việt của $L(B)$ trên L (V, p. 113, Mệnh đề 12). Hơn nữa, mọi phần tử của S đều đại số và tách được trên $K(B)$, do đó trên $L(B)$ (V, p. 39, Hệ quả 2). Ta suy ra (V, p. 39, Mệnh đề 6) rằng $L(S) = L(B)(S)$ là đại số và tách được trên $L(B)$, do đó $L(S)$, tách được trên L.

#### Hệ quả {#alg-v-s16-n7-cor-2 .statement}

— *Nếu L và M là các mở rộng tách được, rời nhau về mặt đại số trên K, thì trường $K(L \cup M)$ là tách được trên K.*

Vì $K(L \cup M) = L(M)$ là tách được trên L theo Mệnh đề 5 (do M là tách được trên K) và L là tách được trên K, do đó có hệ quả (V, p. 122, Mệnh đề 9).

Giả thiết rằng các mở rộng L và M là rời nhau về mặt đại số là không thể thiếu trong Mệnh đề 5 và hệ quả của nó. Thật vậy, cho K là một trường không hoàn hảo có đặc số $p \neq 0$ và E là một mở rộng có dạng $K(x, a)$ với x siêu việt trên K và a là một phần tử p-căn có chiều cao 1 trên K ; đặt $L = K(x)$ và $M = K(x + a)$. Khi đó $x + a$ là siêu việt trên K (nếu không, $x = (x + a) - a$ sẽ là đại số trên K) và các trường L và M là tách được trên K. Tuy nhiên, $K(L \cup M) = K(x, a)$ là p-căn có bậc $p$ trên $L = K(x)$ và không tách được trên L, cũng không trên K.

### Bài tập {#alg-v-s16-exercises}

Xem [các bài tập của § 16](exercises/s16/).
