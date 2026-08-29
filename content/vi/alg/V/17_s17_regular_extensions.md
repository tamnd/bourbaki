---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 17
section_title: Regular extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.180-A V.181
pdf_pages: 0251-0259, 0294-0295
extraction: ocr
subsections:
    - "no": 1
      title: Complements on the relative separable algebraic closure
      page: 137
      pdf_page: 251
    - "no": 2
      title: The tensor product of extensions
      page: 139
      pdf_page: 253
    - "no": 3
      title: Regular algebras
      page: 140
      pdf_page: 254
    - "no": 4
      title: Regular extensions
      page: 141
      pdf_page: 255
    - "no": 5
      title: Characterization of regular extensions
      page: 142
      pdf_page: 256
    - "no": 6
      title: Application to composite extensions
      page: 143
      pdf_page: 257
statements: 20
exercises: 5
content_sha256: 35e77827ac8ed1d593d4ef7f34dc8284f627af73c8f5cd59df6c2333b240c895
translated_from: content/en/alg/V/17_s17_regular_extensions.md
source_content_sha256: 0970c4aa41158ef33231d08b21a0ce6a9b85ee1660b0f424d771a6b9760e1253
translation_model: gpt-5.4
translation_run: translate-vi-ab1b1743
glossary_version: 34
glossary_terms_sha256: 45e22dc20ad4b0716440ad3c2ee1006c47c79d62bf7805bcfd790adfaa676a3f
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 17. CÁC MỞ RỘNG CHÍNH QUY

### 1. Bổ sung về bao đóng đại số tách được tương đối

#### Định lý 1 (Zariski) {#alg-v-s17-thm-1 .statement}

— *Cho K là một trường, L là một mở rộng của K, $K_1$ là bao đóng đại số tách được tương đối của K trong L (V, p. 44), $K_2$ là bao đóng đại số tương đối của K trong L (V, p. 19) và $(X_i)_{i \in I}$ là một họ các bất định. Khi đó $K_1(X_i)_{i \in I}$ là bao đóng đại số tách được tương đối của $K(X_i)_{i \in I}$ trong $L(X_i)_{i \in I}$, và $K_2(X_i)_{i \in I}$ là bao đóng đại số tương đối của $K(X_i)_{i \in I}$ trong $L(X_i)_{i \in I}$.

A) Giả sử E là một trường và F là một trường mở rộng của E, và mọi phần tử của F mà tách được đại số trên E đều thuộc về E. Cho $u$ là một phần tử của $F(X)$ mà tách được đại số trên $E(X)$; ta sẽ chứng minh rằng $u$ thuộc về $E(X)$. Tồn tại trong $F(X)$ hai đa thức nguyên tố cùng nhau P và Q sao cho $u = P/Q$ và ta có thể lấy Q là đơn nhất. Gọi S là tập con *hữu hạn* của F gồm các hệ số của P và Q, $F_0 = E(S)$ và gọi A là một đạo hàm E của $F_0$ vào $F_0$. Gọi $D$ là đạo hàm của $F_0(X)$ vào chính nó, trùng với $A$ trên $F_0$ và ánh xạ $X$ tới $0$ (V, p. 128, Mệnh đề 3).

Vì $u \in F_0(X)$ là đại số tách được trên $E(X)$ và $D$ bằng không trên $E(X)$, ta có $D(u) = 0$ (V, p.129, Mệnh đề 4), do đó $D(P) . Q = P . D(Q)$. Vì $P$ và $Q$ nguyên tố cùng nhau, ta kết luận rằng $Q$ chia hết $D(Q)$ (IV, p. 13, Hệ quả 4). Bây giờ $Q$ có thể được viết dưới dạng
$$
Q(X) = X^n + a_1 X^{n-1} + \ldots + a_{n-1} X + a_n
$$
với $a,, \ldots, a,$ thuộc $F_0$; vì $D(x) = 0$, do đó ta có
$$
D(Q) = \Delta(a_1) X^{n-1} + \cdots + \Delta(a_{n-1}) X + \Delta(a_n)
$$
do đó $\deg D(Q) < \deg Q$. Vì $Q$ chia hết $D(Q)$, điều này chỉ có thể xảy ra nếu $D(Q) = 0$. Nhưng khi đó $D(P) = 0$ vì $D(P) . Q = P . D(Q)$. Bây giờ (1) và một công thức tương tự đối với $P$ cho thấy rằng $A$ triệt tiêu tập hợp $S$ các hệ số của $P$ và $Q$, do đó $A = 0$, vì $F_0 = E(S)$. Theo V, p. 135, Hệ quả 2, mở rộng sinh hữu hạn $F_0$ của $E$ do đó là đại số tách được; theo các giả thiết trên $E$ và $F$ ta có $F_0 = E$, vậy cuối cùng $u \in E(X)$.

B) Bây giờ giả sử rằng $E$ đóng đại số tương đối trong trường mở rộng $F$ và ký hiệu $p$ là số mũ đặc số của $E$. Cho $u$ là một phần tử của $F(X)$ đại số trên $E(X)$. Tồn tại một số nguyên $f \geq 0$ sao cho $v = u^{p^f}$ là đại số tách được trên $E(X)$ (V, p. 44, Mệnh đề 13). Bởi A) do đó ta có $v \in E(X)$. Tồn tại một biểu diễn duy nhất của $u$ dưới dạng $P/Q$ với $P$ và $Q$ là các đa thức nguyên tố cùng nhau trong $F[X]$ và $Q$ đơn nhất; ta có một phân tích tương tự $v = P_1/Q_1$ với $P_1$ và $Q_1$ nguyên tố cùng nhau trong $E[X]$ và $Q_1$ đơn nhất. Suy ra rằng $P_1/Q_1 = P^{p^f}/Q^{p^f}$; các đa thức $P^{p^f}$ và $Q^{p^f}$ nguyên tố cùng nhau trong $F[X]$ (IV, p. 13, Hệ quả 6), cũng như $P_1$ và $Q_1$, và $Q^{p^f}$ là đơn nhất. Suy ra rằng $P^{p^f} = P_1 \in E[X]$ và $Q^{p^f} = Q_1 \in E[X]$. Vậy các hệ số của $P$ và $Q$ là $p$-căn trên $E$, và do đó thuộc $E$ vì $E$ đóng đại số tương đối trong $F$. Do đó ta có $P \in E[X]$, $Q \in E[X]$ và cuối cùng $u \in E(X)$. Điều này chứng tỏ $E(X)$ là đóng đại số tương đối trong $F(X)$.

C) Ta dùng ký hiệu của Định lý 1. Vì $K_1$ là một mở rộng đại số tách được của $K$, mở rộng $K_1(X_i)_{i \in I}$ của $K(X_i)_{i \in I}$ là đại số và tách được (V, p. 39, Mệnh đề 6). Hơn nữa, mọi phần tử của $L$ là đại số và tách được trên $K$ đều thuộc $K$, (V, p. 44, Mệnh đề 13, a)). Cho $J$ là một tập con hữu hạn của $I$; bằng một phép quy nạp ngay lập tức theo lực lượng của $J$ ta suy ra từ A) rằng mọi phần tử của $L(X_i)_{i \in I}$, là đại số và tách được trên $K(X_i)_{i \in I}$, đều thuộc $K_1(X_i)_{i \in J}$. Cuối cùng, cho $u$ là một phần tử của $L(X_i)_{i \in I}$, đại số và tách được trên $K(X_i)_{i \in I}$; tồn tại một tập con hữu hạn $J$ của $I$ sao cho $u$ thuộc $L(X_i)_{i \in I}$ và là đại số và tách được trên $K(X_i)_{i \in J}$; theo điều đã nói, $u$ thuộc $K_1(X_i)_{i \in J}$, và a fortiori thuộc $K_1(X_i)_{i \in I}$.

Như vậy ta đã suy ra từ A) rằng $K_1(X_i)_{i \in I}$ là bao đóng tách được tương đối của $K(X_i)_{i \in I}$ trong $L(X_i)_{i \in I}$; cũng theo cách ấy suy ra từ B) rằng $K_2(X_i)_{i \in I}$ là bao đóng đại số tương đối của $K(X_i)_{i \in I}$ trong $L(X_i)_{i \in I}$.

### 2. Tích tenxơ của các mở rộng

#### Mệnh đề 1 {#alg-v-s17-prop-1 .statement}

— Cho $\Omega$ là một mở rộng của một trường $K$ và cho $L, M$ là hai mở rộng con của $\Omega$ rời nhau về mặt đại số trên $K$. Giả sử bao đóng đại số tách được tương đối của $K$ trong $L$ bằng $K$^1. Gọi $\varphi$ là đồng cấu đại số $K$ của $L \otimes_K M$ vào $\Omega$ ánh xạ $x \otimes y$ thành $xy$ với $x \in L, y \in M$, và gọi $p$ là hạt nhân của $\varphi$. Khi đó $p$ là tập hợp các phần tử lũy linh của $L \otimes_K M$ và đó là iđêan nguyên tố nhỏ nhất của $L \otimes_K M$.

Khi cần thiết thay thế $\Omega$ bằng một bao đóng đại số, ta có thể giả sử $\Omega$ đóng đại số. Gọi $B$ là một cơ sở siêu việt của $M$ trên $K$, $N$ là bao đóng đại số tương đối của $K(B)$ trong $\Omega$ và $N_r$ (tương ứng $N_s$) là tập hợp các phần tử của $N$ tách được (tương ứng, p-căn) trên $K(B)$. Ta nhận xét rằng $M$ là đại số trên $K(B)$, do đó $N$ là bao đóng đại số tương đối của $M$ trong $\Omega$.

$$
\begin{array}{ccccccccc}
L & \longrightarrow & L(B) & \longrightarrow & L(B \cup N_s) \\
\uparrow & & \uparrow & & \uparrow \\
K & \longrightarrow & K(B) & \longrightarrow & N_s \\
& & \downarrow & & \downarrow \\
& & M & \longrightarrow & N \\
\uparrow & & \downarrow & & \downarrow \\
N_r & \longrightarrow & N & \longrightarrow & \Omega
\end{array}
$$

Hình 1.

Hãy định nghĩa chuỗi đồng cấu sau:

$$
L \otimes_K M \xrightarrow{\alpha} L \otimes_K N \xrightarrow{\beta} (L \otimes_K K(B)) \otimes_{K(B)} N \xrightarrow{\gamma} L(B) \otimes_{K(B)} N
$$
$$
\rightarrow L(B) \otimes_{K(B)} N_s \otimes_{K(B)} N_r \xrightarrow{\varepsilon} L(B \cup N_s) \otimes_{K(B)} N_r \xrightarrow{\zeta} \Omega .
$$

Ta có $\alpha = \mathrm{Id}_L \otimes u$ trong đó $u$ là đơn ánh chính tắc của $M$ vào $N$, do đó $\alpha$ là đơn ánh. Ánh xạ $\beta$ là đẳng cấu của các nhóm giao hoán biến $x \otimes y$ thành $(x \otimes 1) \otimes y$ (II, p. 278, Mệnh đề 2) với $x \in L$ và $y \in N$. Ta có $\gamma = v \otimes \mathrm{Id}_N$, trong đó $v$ là đồng cấu đại số $K$ của $L \otimes_K K(B)$ vào $L(B)$ biến $x \otimes y$ thành $xy$, với $x \in L$ và $y \in K(B)$; vì $L$ và $M$ độc lập đại số trên $K$, Mệnh đề 14 (V, p. 114) cho thấy rằng $L$ và $K(B)$ độc lập tuyến tính trên $K$, nói cách khác, $v$ là đơn ánh, do đó $y$ là đơn ánh. Vì $N$ là một mở rộng quasi-Galois của $K(B)$, tồn tại (V, p. 76, Mệnh đề 13) một đẳng cấu đại số $K(B)$ $w$ của $N_s \otimes_{K(B)} N_r$ lên $N$ biến $x \otimes y$ thành

1 Giả thiết này đôi khi được diễn đạt bằng cách nói rằng $L$ là một mở rộng nguyên sơ của $K$.

xy với $x \in \mathbf{N}$, và $y \in \mathbf{N}_r$; ta ký hiệu bởi 6 *đẳng cấu* $\mathrm{Id}_{L(B)} \otimes w \ ^1$. Theo Đl. 1 (V, p. 137) và giả thiết về mở rộng L của K, mọi phần tử của $L(B)$ là đại số và tách được trên $K(B)$ đều thuộc $K(B)$; đặc biệt, ta có $L(B) \cap N_s = K(B)$. Vì $N_r$ là một mở rộng Galois của $K(B)$, Đl. 5 (V, p. 71) cho thấy rằng tồn tại một đẳng cấu đại số trên $K(B)$ $w'$ của $L(B) \otimes_{K(B)} N_s$ lên $L(B U N_r)$ biến $x \otimes y$ thành $xy$ với $x \in L(B)$ và $y \in N_r$; ta ký hiệu bởi $\varepsilon$ *đẳng cấu* $w' \otimes \mathrm{Id}_{N_r}$. Cuối cùng, $\zeta$ là đồng cấu đại số trên K biến $x \otimes y$ thành $xy$ với $x \in L(B U N_r)$ và $y \in N_r$.

Điều đã nói cho thấy rằng $\eta = \varepsilon \delta \gamma \beta \alpha$ là một đồng cấu đại số trên K đơn ánh của $L \otimes_K M$ vào $L(B U N_r) \otimes_{K(B), N_r}$. Hơn nữa, mọi phần tử của M đều có dạng $\sum_{i=1}^n a_i b_i$ với $a_i \in \mathbf{N}$, và $b_i \in \mathbf{N}_r$ đối với $1 \leq i \leq n$; do đó ta thu được $\varphi = \zeta \eta$.

Hạt nhân $p$ của $\varphi$ là một iđêan nguyên tố của $L \otimes_K M$, nên mọi phần tử lũy linh của $L \otimes_K M$ đều thuộc $p$, theo Mệnh đề 2 (V, p. 118). Ngược lại, cho $a$ là một phần tử của $p$; đặt $\eta(a) = \sum_{r=1}^s b_i \otimes c_i$ với $b_i \in L(B U N_r)$ và $c_i \in N_r$ đối với $1 \leq i \leq s$. Vì $N_r$ là một mở rộng p-căn của $K(B)$, tồn tại một số nguyên $f \geq 0$ sao cho $c_i^{p^f}$ thuộc $K(B)$ đối với $1 \leq i \leq s$ (trong đó $p$ là số mũ đặc số của K). Nhưng ta có

$$
\eta(a^{p^f}) = \sum_{i=1}^s b_i^{p^f} \otimes c_i^{p^f} = \left( \sum_{i=1}^s b_i^{p^f} c_i^{p^f} \right) \otimes 1 - \zeta \eta(a)^{p^f} \otimes 1 = 0
$$

và vì $\eta$ là đơn ánh nên cuối cùng ta có $a^{p^f} = 0$. Như vậy ta đã chứng minh $p$ là tập hợp tất cả các phần tử lũy linh của $L \otimes_K M$. Bây giờ mọi iđêan nguyên tố của $L \otimes_K M$ đều chứa $p$ theo Mệnh đề 2 (V, p. 118).

#### Hệ quả {#alg-v-s17-n2-cor-1 .statement}

*Cho L và M là hai mở rộng của một trường K. Giả sử bao đóng đại số tách được tương đối của K trong L bằng K. Khi đó tập hợp p các phần tử lũy linh của $L \otimes_K M$ là một iđêan nguyên tố. Hơn nữa, nếu L hoặc M tách được trên K, thì $L \otimes_K M$ là một miền nguyên.*

Ta có thể giả sử rằng L và M là các mở rộng con rời nhau về mặt đại số của một mở rộng $\Omega$ của K (V, p. 116, Định lý 5); khi đó p là một iđêan nguyên tố theo Mệnh đề 1 (V, p. 139). Hơn nữa, nếu L hoặc M tách được trên K, thì $L \otimes_K M$ là một vành không có phần tử lũy linh khác không theo định nghĩa của mở rộng tách được (V, p. 119, Định nghĩa 1); do đó $p = 0$ và $L \otimes_K M$ là một miền nguyên vì p là nguyên tố.

### 3. Đại số chính quy

#### Định nghĩa 1 {#alg-v-s17-def-1 .statement}

*Cho K là một trường. Một đại số A trên K được gọi là chính quy nếu $L \otimes_K A$ là một miền nguyên với mọi mở rộng L của K.*

Một đại số chính quy, đặc biệt, là một miền nguyên, do đó là giao hoán.

#### Mệnh đề 2 {#alg-v-s17-prop-2 .statement}

— Cho $A$ và $B$ là hai đại số trên một trường $K$. Nếu $A$ là một miền nguyên và $B$ là chính quy thì $A \otimes_K B$ là một miền nguyên.

Gọi $L$ là trường phân thức của $A$. Vì $B$ là một $K$-đại số chính quy, $L \otimes_K B$ là một miền nguyên, do đó $A \otimes_K B$ cũng vậy, vì nó đẳng cấu với một vành con của $L \otimes_K B$.

#### Mệnh đề 3 {#alg-v-s17-prop-3 .statement}

— Cho $K$ là một trường.
a) Mọi đại số con của một $K$-đại số chính quy tự nó cũng chính quy.
b) Tích tenxơ của hai $K$-đại số chính quy lại chính quy.
c) Cho $A$ là một $K$-đại số và $K'$ là một mở rộng của $K$. Để $A$ là chính quy, điều kiện cần và đủ là $K'$-đại số $A_{(K')}$ dẫn xuất từ $A$ bởi mở rộng vô hướng phải chính quy.

Chứng minh của a) (tương ứng, c)) giống hệt chứng minh của phần a) (tương ứng, d)) của Mệnh đề 3, V, p. 119, sau khi thay thế ở mọi nơi « vành rút gọn » bằng « miền nguyên » và « đại số tách được » bằng « đại số chính quy ». Ta hãy chứng minh b).

Cho $A$ và $B$ là hai $K$-đại số chính quy. Cho $L$ là một mở rộng của $K$. Vì $A$ là chính quy, vành $L \otimes_K A$ là một miền nguyên. Theo Mệnh đề 2, vành $(L \otimes_K A) \otimes_K B$ là một miền nguyên, vì $B$ là chính quy. Sau cùng, vành $L \otimes_K (A \otimes_K B)$ đẳng cấu với $(L \otimes_K A) \otimes_K B$, và do đó là một miền nguyên. Điều này cho thấy $A \otimes_K B$ là một $K$-đại số chính quy.

### 4. Các mở rộng chính quy

#### Định nghĩa 2 {#alg-v-s17-def-2 .statement}

— Một mở rộng của một trường $K$ được gọi là chính quy nếu nó chính quy như một $K$-đại số.

#### Mệnh đề 4 {#alg-v-s17-prop-4 .statement}

— Cho $A$ là một đại số trên trường $K$ là một miền nguyên, và $E$ là trường phân thức của nó. Cho $L$ là một mở rộng của $K$; nếu vành $L \otimes_K A$ là một miền nguyên thì điều tương tự cũng đúng với $L \otimes_K E$.

Nếu $L \otimes_K A$ là một miền nguyên, nó có thể được nhúng vào trường phân thức $F$ của nó. Viết $u(x) = x \otimes 1$ với $x \in L$ và ký hiệu bởi $v$ đồng cấu $K$ của $E$ vào $F$ mở rộng đơn cấu $y \mapsto 1 \otimes y$ của $A$ vào $F$. Theo Mệnh đề 6 (V, p. 14), các trường con $u(L)$ và $v(E)$ của $F$ độc lập tuyến tính trên $K$; do đó đồng cấu $u * v$ của $L \otimes_K E$ vào $F$ (V, p. 12) là đơn ánh. Điều này cho thấy $L \otimes_K E$ là một miền nguyên.

#### Hệ quả {#alg-v-s17-n4-cor-1 .statement}

— Để $A$ là một $K$-đại số chính quy thì điều kiện cần và đủ là trường phân thức của nó là một mở rộng chính quy của $K$.

Điều kiện đó là cần theo Mệnh đề 4 và là đủ theo Mệnh đề 3, a).

#### Mệnh đề 5 {#alg-v-s17-prop-5 .statement}

— Mọi mở rộng thuần của một trường $K$ đều là chính quy.

Theo hệ quả trên, chỉ cần chứng minh rằng mọi đại số đa thức $A = K[X_i]_i$ đều là một $K$-đại số chính quy. Cho $L$ là một mở rộng của $K$; vành $L \otimes_K A$ đẳng cấu với $L[X_i]_{i \in I}$ (III, p. 449, Nhận xét 2), và do đó là một miền nguyên (IV, p. 9, Mệnh đề 8).

#### Mệnh đề 6 {#alg-v-s17-prop-6 .statement}

— Cho L là một mở rộng của một trường K. Nếu L là chính quy, thì mọi mở rộng con của L đều chính quy. Ngược lại, nếu mọi mở rộng con sinh hữu hạn của L đều chính quy, thì L là chính quy.

Mệnh đề thứ nhất suy ra từ Mệnh đề 3, a).

Cho M là một mở rộng của K và $\mathcal{U}$ là tập hợp tất cả các mở rộng con sinh hữu hạn của L. Với mỗi E $\in \mathcal{U}$, vành $M \otimes_K E$ có thể được đồng nhất với một vành con của $M \otimes_K L$ và do đó ta có một họ tăng có hướng các vành con của $M \otimes_K L$ mà hợp là $M \otimes_K L$. Bây giờ mệnh đề thứ hai suy ra ngay lập tức.

#### Mệnh đề 7 {#alg-v-s17-prop-7 .statement}

— Cho L là một mở rộng của một trường K và M là một đại số trên L (ví dụ, một mở rộng của L). Nếu L là chính quy trên K và M là một đại số trên L chính quy, thì M là chính quy như một đại số trên K.

Cho E là một mở rộng của K; vì L là chính quy trên K, $E \otimes_K L$ là một miền nguyên. Theo Mệnh đề 2 (V, p. 141), vành $(E \otimes_K L) \otimes_L M$ do đó là một miền nguyên và điều tương tự cũng đúng với vành $E \otimes_K M$ đẳng cấu với nó (II. p. 278, Mệnh đề 2). Vậy có kết quả.

#### Mệnh đề 8 {#alg-v-s17-prop-8 .statement}

— Cho L và M là hai mở rộng của một trường K.

a) Nếu M là chính quy trên K, thì trường phân thức của miền nguyên $L \otimes_K M$ là một mở rộng chính quy của L.

b) Nếu L và M là các mở rộng chính quy của K, thì điều tương tự cũng đúng đối với trường phân thức của $L \otimes_K M$.

Mệnh đề a) suy ra từ Mệnh đề 3, c) (V, p. 141) và Hệ quả của V, p. 141; Mệnh đề b) suy ra từ Mệnh đề 3, b) (V, p. 141) và Hệ quả của V, p. 141.

### 5. Đặc trưng hóa các mở rộng chính quy

#### Mệnh đề 9 {#alg-v-s17-prop-9 .statement}

— Cho K là một trường, $\overline{K}$ là một bao đóng đại số của K và L là một mở rộng của K. Khi đó các điều kiện sau là tương đương:

a) L tách được trên K và K tương đối đóng đại số trong L.

b) L là một mở rộng chính quy của K.

c) Vành $\overline{K} \otimes_K L$ là một miền nguyên.

d) Cho $\overline{L}$ là một bao đóng đại số của L. Khi đó L tách rời tuyến tính trên K với bao đóng đại số tương đối của K trong $\overline{L}$.

Hơn nữa, khi các điều kiện này được thỏa mãn, thì $\overline{K} \otimes_K L$ là một trường.

a) $\Rightarrow$ b): Cho M là một mở rộng của K. Dưới các giả thiết của a), vành $M \otimes_K L$ là một miền nguyên, theo V, p. 140, Hệ quả.

b) $\Rightarrow$ c): Điều này suy ra từ Định nghĩa 2.

c) $\Rightarrow$ d): Với ký hiệu của d) ta có thể đồng nhất $\overline{K}$ với bao đóng đại số tương đối của K trong $\overline{L}$ (V, p. 22, Bài tập 2). Giả sử rằng vành $A = \overline{K} \otimes_K L$ là một miền nguyên. Cho E là một mở rộng con của K có bậc hữu hạn trên K; vành con

E $\otimes_K$ L của A là một miền nguyên và do đó là một đại số bậc hữu hạn trên L; theo Hệ quả của V, p. 10 nó là một trường. Vì $\bar{K}$ là hợp của tập có hướng tăng các mở rộng E thuộc kiểu trên, A là một trường (V, p. 11, Mệnh đề 3). Đồng cấu chính tắc từ A vào $\bar{L}$ ánh xạ $x \otimes y$ thành $xy$ (với $x \in \bar{K}$ và $y \in L$) vì thế là đơn ánh, nên L và $\bar{K}$ độc lập tuyến tính trên K.

$d) \Rightarrow a)$: Dưới các giả thiết của d) ta có $L \cap \bar{K} = K$, nên K đóng đại số tương đối trong L; hơn nữa nếu p là số mũ đặc số của K, trường $L$ độc lập tuyến tính với $K^{p^{-\infty}}$ trên $K$, do đó L tách được trên K (V, p. 123, Hệ quả 1).

#### Hệ quả 1 {#alg-v-s17-prop-9-cor-1 .statement}

— Để A là một đại số chính quy trên một trường K thì điều kiện cần và đủ là vành $\bar{K} \otimes_K A$ là một miền nguyên.

Điều kiện đã nêu rõ ràng là cần thiết. Ngược lại, giả sử rằng $\bar{K} \otimes_K A$ là một miền nguyên và ký hiệu bởi E trường phân thức của A. Theo Mệnh đề 4 (V, p. 141) vành $\bar{K} \otimes_K E$ là một miền nguyên, do đó E là một mở rộng chính quy của K, theo Mệnh đề 9; theo V, p. 141, Hệ quả, ta kết luận rằng A là chính quy như một đại số trên K.

#### Hệ quả 2 {#alg-v-s17-prop-9-cor-2 .statement}

— Cho K là một trường đóng đại số. Mọi đại số trên K là một miền nguyên đều là một đại số trên K chính quy. Đặc biệt, mọi mở rộng của K đều là chính quy.

Điều này suy ra từ Hệ quả 1.

#### Hệ quả 3 {#alg-v-s17-prop-9-cor-3 .statement}

— Cho K là một trường đóng đại số. Nếu A và B là hai đại số trên K là những miền nguyên, thì $A \otimes_K B$ cũng vậy.

Theo Hệ quả 2, A và B là các đại số trên K chính quy, và chỉ cần áp dụng Mệnh đề 2 (V, p. 141).

### 6. Ứng dụng cho các mở rộng hợp thành

#### Mệnh đề 10 {#alg-v-s17-prop-10 .statement}

— Cho L và M là hai mở rộng của một trường K và $(E, u, v)$ là một mở rộng hợp thành của L và M (V, p. 12). Giả sử rằng vành $L \otimes_K M$ là một miền nguyên và các mở rộng con $u(L)$ và $v(M)$ của E là đóng đại số rời nhau trên K. Khi đó $u(L)$ và $v(M)$ độc lập tuyến tính trên K.

Đặt $w = u * v$ (V, p. 12), ký hiệu bởi F trường phân thức của miền nguyên $L \otimes_K M$ và đồng nhất L (ứng với M) với một trường con của F bằng ánh xạ $x \mapsto x \otimes 1$ (ứng với $y \mapsto 1 \otimes y$); khi đó hạn chế của w lên L (ứng với M) là u (ứng với v). Cho B là một cơ sở siêu việt của M trên K (V, p. 109, Định lý 1).

Theo giả thiết, $u(L)$ và $v(M)$ rời nhau về mặt đại số trên K; do đó (V, p. 114, Mệnh đề 14), $u(L)$ và $v(K(B))$ rời nhau tuyến tính trên K. Vì vậy tồn tại một K-đồng cấu $u': L(B) \to E$ trùng với u trên L và với v trên K(B). Theo phép dựng, L và M rời nhau tuyến tính trên K trong F; theo Mệnh đề 8 (V, p. 15), các trường con $L(B)$ và $M$ của F rời nhau tuyến tính trên $K(B)$. Suy ra rằng tồn tại một K-đồng cấu $w' : M[L(B)] \to E$ trùng với $u'$ trên $L(B)$ và với $v$ trên $M$. Nhưng trường $F$ được sinh bởi $M \cup L(B)$ và $M$ là đại số trên $K(B)$; do đó ta có $M[L(B)] = F$ (V, p. 18, Hệ quả 2). Vậy ta kết luận rằng $w'$ là một K-đẳng cấu của $F$ lên $E$ mà hạn chế của nó trên $L$ (tương ứng, $M$) là $u$ (tương ứng, $v$). Điều này chứng tỏ $u(L)$ và $v(M)$ rời nhau tuyến tính trên $K$.

#### Hệ quả 1 {#alg-v-s17-prop-10-cor-1 .statement}

*Cho $\Omega$ là một mở rộng của một trường $K$ và $L$ là một mở rộng con của $\Omega$ chính quy trên $K$. Mọi mở rộng con $M$ của $\Omega$ rời nhau về mặt đại số với $L$ trên $K$ đều rời nhau tuyến tính.*

Vành $L \otimes_K M$ là một miền nguyên theo định nghĩa của mở rộng chính quy, và bây giờ chỉ cần áp dụng Mệnh đề 10.

#### Hệ quả 2 {#alg-v-s17-prop-10-cor-2 .statement}

*Cho $\Omega$ là một mở rộng của một trường $K$ và $L, M$ là hai mở rộng con của $\Omega$. Giả sử rằng $L$ tách được trên $K$ và bao đóng tách được tương đối của $K$ trong $M$ bằng $K$. Nếu $L$ và $M$ rời nhau đại số trên $K$, thì chúng rời nhau tuyến tính trên $K$.*

Theo Mệnh đề 10, chỉ cần nhận xét rằng vành $L \otimes_K M$ là một miền nguyên (V, p. 140, Hệ quả).

Bài tập

### Bài tập {#alg-v-s17-exercises}

Xem [bài tập cho § 17](exercises/s17/).
