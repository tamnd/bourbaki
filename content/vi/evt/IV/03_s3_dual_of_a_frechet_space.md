---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 3
section_title: Dual of a Fréchet space
lang: vi
source: evt-i-v
book_pages: TVS IV.21-TVS IV.26, TVS IV.57-TVS IV.61
pdf_pages: 0203-0208, 0239-0243
extraction: ocr
subsections:
    - "no": 1
      title: Semi-barrelled spaces
      page: 21
      pdf_page: 203
    - "no": 2
      title: Dual of a locally convex metrizable space
      page: 22
      pdf_page: 204
    - "no": 3
      title: Bidual of a locally convex metrizable space
      page: 23
      pdf_page: 205
    - "no": 4
      title: Dual of a reflexive Fréchet space
      page: 23
      pdf_page: 205
    - "no": 5
      title: The topology of compact convergence on the dual of a Fréchet space
      page: 24
      pdf_page: 206
    - "no": 6
      title: Separately continuous bilinear mappings
      page: 26
      pdf_page: 208
statements: 15
exercises: 2
content_sha256: 800a8a85b81afaa32ab45cf793f762e7cbe734d8ecb28aaf896c51f6eca13449
translated_from: content/en/evt/IV/03_s3_dual_of_a_frechet_space.md
source_content_sha256: 0ee8d1a172c8e03fd1240af060b10128a084bd0f8c1ebf66c69a14c78f828f01
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-aa110db9
glossary_version: 34
glossary_terms_sha256: d614a7c6ec54ee61e87ab45388e30b10d90664e47bf5e4edbd339bdcdfb39db3
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 3. ĐỐI NGẪU CỦA MỘT KHÔNG GIAN FRÉCHET

### 1. Các không gian nửa thùng

#### Mệnh đề 1 {#evt-iv-s3-prop-1 .statement}

— Cho E là một không gian lồi địa phương. Các điều kiện sau là tương đương :

(i) Cho U là một tập con của E hấp thụ mọi tập hợp bị chặn của E, và là giao của một dãy các lân cận lồi, cân bằng và đóng của 0 trong E. Khi đó U là một lân cận của 0 trong E.

(ii) Đối với mọi không gian lồi địa phương F, mọi tập hợp bị chặn của $\mathcal{L}_b(E; F)$ là hợp của một họ đếm được các tập hợp liên tục đều, là liên tục đều.

(iii) Trong đối ngẫu mạnh $E'_b$ của E, mọi tập hợp bị chặn là hợp của một họ đếm được các tập hợp liên tục đều, là liên tục đều.

Hiển nhiên rằng (iii) là một trường hợp riêng của (ii).

(i) $\Rightarrow$ (ii) : cho H là một tập hợp bị chặn của $\mathcal{L}_b(E; F)$, và cho $(H_n)$ là một dãy các tập hợp liên tục đều của $\mathcal{L}_b(E; F)$ sao cho $H = \bigcup H_n$. Cho V là một lân cận lồi, cân bằng và đóng của 0 trong F. Với mọi $n$, tập hợp $W_n = \bigcap_{u \in H_n} u^{-1}(V)$ là một lân cận lồi, cân bằng và đóng của 0 trong E vì $H_n$ là liên tục đều. Tập hợp $W = \bigcap_{u \in H} u^{-1}(V)$ hấp thụ mọi tập hợp bị chặn của E, vì H bị chặn trong $\mathcal{L}_b(E; F)$ (III, p. 22), và ta có $W = \bigcap_n W_n$. Nếu E thỏa mãn (i), thì tập hợp W là một lân cận của 0 trong E, do đó H là liên tục đều.

(iii) $\Rightarrow$ (i) : cho $(U_n)$ là một dãy các lân cận lồi, cân bằng và đóng của 0 trong E. Ta giả sử rằng tập hợp $U = \bigcap_n U_n$ hấp thụ mọi tập hợp bị chặn của E, do đó cực của nó $U^\circ$ bị chặn trong $E'_b$. Khi đó tập hợp $B = \bigcup_n U_n^\circ$ được chứa trong $U^\circ$, do đó bị chặn trong $E'_b$. Nếu E thỏa mãn (iii), tập hợp B là liên tục đều trong $E'$; do đó, cực $B^\circ = \bigcap_n (U_n^\circ)^\circ = \bigcap_n U_n = U$ của B trong E là một lân cận của 0 trong E.

#### Định nghĩa 1 {#evt-iv-s3-def-1 .statement}

— Một không gian lồi địa phương E được gọi là nửa thùng nếu nó thỏa mãn các điều kiện tương đương của mệnh đề 1.

Mọi không gian thùng đều là nửa thùng. Điều này cũng đúng với mọi không gian sinh bởi bị chặn (III, p. 22, mệnh đề 10).

### 2. Đối ngẫu của một không gian lồi địa phương mêtric hóa

#### Mệnh đề 2 {#evt-iv-s3-prop-2 .statement}

— Cho E là một không gian lồi địa phương mêtric hóa và F là đối ngẫu mạnh của nó. Không gian F là đầy đủ, nửa thùng và thỏa mãn điều kiện sau :
(DB) Tồn tại một dãy $(A_n)_{n \in \mathbf{N}}$ các tập hợp bị chặn của F sao cho mọi tập hợp bị chặn của F được chứa trong một trong các $A_n$.

Không gian E là sinh bởi bị chặn (III, p. 12, mệnh đề 2), do đó đối ngẫu mạnh của nó là đầy đủ (III, p. 23, hệ quả 1).

Cho $(V_n)_{n \in \mathbf{N}}$ là một dãy giảm các lân cận của 0 trong E, sao cho mọi lân cận của 0 trong E chứa một trong các $V_n$. Cho $A_n$ là cực của $V_n$ trong F. Vì E là sinh bởi bị chặn, mọi tập hợp bị chặn của F là liên tục đều (III, p. 22, mệnh đề 10), do đó được chứa trong một trong các $A_n$. Nói cách khác, không gian F thỏa mãn điều kiện (DB).

Bây giờ ta chứng minh rằng F là nửa thùng. Cho $(U_n)_{n \in \mathbf{N}}$ là một dãy các lân cận lồi, cân bằng và đóng của 0 trong F. Ta giả sử rằng tập hợp $U = \bigcap_n U_n$ hấp thụ mọi tập hợp bị chặn của F. Ta sẽ chứng minh rằng U là một lân cận của 0 trong F. Để làm điều này, ta sẽ xây dựng, bằng quy nạp theo số nguyên $n \geqslant 0$, các số thực $\lambda_n > 0$ và các lân cận lồi cân bằng $W_n$ của 0 trong F, chúng đóng đối với $\sigma(F, E)$, và thỏa mãn các hệ thức sau

(1)
$$
\lambda_n A_n \subset \frac{1}{2} U \cap \left( \bigcap_{0 \leq i < n} W_i \right)
$$

(2)
$$
\bigcup_{0 \leq i \leq n} \lambda_i A_i \subset W_n \subset U_n .
$$

Giả sử rằng các số $\lambda_i$ và các tập hợp $W_i$ đã được xây dựng với $0 \leq i < n$. Theo giả thiết, tập hợp U hấp thụ các tập hợp bị chặn của F; hơn nữa, với $0 \leq i < n$, $W_i$ là một lân cận của 0 trong F, do đó hấp thụ các tập hợp bị chặn của F. Vì vậy ta có thể tìm được một số $\lambda_n > 0$ thỏa mãn (1). Gọi C là bao lồi cân bằng đóng, đối với $\sigma(F, E)$, của $\bigcup_{0 \leq i \leq n} \lambda_i A_i$; tập hợp C là liên tục đều, do đó compact đối với $\sigma(F, E)$ (III, p. 17, hệ quả 2). Vì $U_n$ là một lân cận của 0 trong F, tồn tại một tập hợp bị chặn B của E sao cho $B^\circ \subset \frac{1}{2} U_n$. Đặt $W_n = C + B^\circ$. Vì $B^\circ$ là một lân cận của 0 trong F, ta thấy rằng $W_n$ là một lân cận lồi và cân bằng của 0 trong F. Ngoài ra, C là compact và $B^\circ$ đóng đối với $\sigma(F, E)$; theo hệ quả 1 của GT, III, § 4, No. 1, $W_n$ đóng đối với $\sigma(F, E)$. Cuối cùng, ta có $C \subset \frac{1}{2} U \subset \frac{1}{2} U_n$ và $B^\circ \subset \frac{1}{2} U_n$, do đó $W_n \subset U_n$ vì $U_n$ là lồi. Như vậy ta đã thiết lập được (2).

Đặt $W = \bigcap_n W_n$, khi đó $W \subset U$. Theo (1) và (2), ta có $\lambda_i A_i \subset W_j$ với mọi $i$ và $j$ trong $\mathbf{N}$, và do đó $\lambda_i A_i \subset W$ với mọi $i \in \mathbf{N}$. Đặc biệt, W là hấp thụ, do đó là một thùng đối với $\sigma(F, E)$. Theo nhận xét 3 của IV, p. 4, W là một lân cận của 0 trong F. A fortiori, U là một lân cận của 0 trong F, và F là nửa-thùng.

Hệ quả sau đây mở rộng định lý Banach-Steinhaus sang đối ngẫu của một không gian Fréchet (*cf.* III, p. 25, hệ quả 2).

#### Hệ quả {#evt-iv-s3-n2-cor-1 .statement}

— Cho G là một không gian lồi địa phương Hausdorff, và cho $(u_n)$ là một dãy các ánh xạ tuyến tính từ F vào G, hội tụ đơn giản đến một ánh xạ u từ F vào G. Khi đó u là liên tục, và dãy $(u_n)$ hội tụ đến u đều trên mọi tập con tiền compact của F.

Vì F là đầy đủ, tập hợp tất cả các $u_n$, bị chặn đối với tôpô hội tụ đơn giản, là bị chặn trong $\mathcal{L}_b(F; G)$ (III, p. 27, hệ quả 1). Vì không gian F là nửa-thùng (mệnh đề 2), mọi tập con đếm được và bị chặn của $\mathcal{L}_b(F; G)$ là đẳng liên tục theo mệnh đề 1 của IV, p. 21. Do đó tập hợp các $u_n$ là đẳng liên tục, và hệ quả suy ra từ III, p. 18, hệ quả.

### 3. Đối đối ngẫu của một không gian lồi địa phương mêtric hóa được

#### Mệnh đề 3 {#evt-iv-s3-prop-3 .statement}

— Cho E là một không gian lồi địa phương mêtric hóa được, $E'_b$ là đối ngẫu mạnh của nó và G là một không gian Fréchet. Không gian $\mathcal{L}_b(E'_b ; G)$ là một không gian Fréchet.

Theo mệnh đề 2 (IV, p. 22), tồn tại một dãy $(A_n)$ các tập con bị chặn của $E'_b$ sao cho mọi tập con bị chặn của $E'_b$ đều được chứa trong một trong các $A_n$. Cho $(V_n)$ là một hệ cơ bản đếm được các lân cận của 0 trong G. Cho $H_{mn}$ là tập hợp các ánh xạ tuyến tính $u$ từ $E'_b$ vào G sao cho $u(A_m) \subset V_n$. Khi đó $(H_{mn})$ là một hệ cơ bản các lân cận của 0 trong $\mathcal{L}_b(E'_b ; G)$, và không gian sau đó là mêtric hóa được.

Để chứng minh rằng $\mathcal{L}_b(E'_b ; G)$ là đầy đủ, chỉ cần chứng minh rằng mọi dãy Cauchy $(u_n)$ trong không gian này đều hội tụ; vì G là đầy đủ, tồn tại một ánh xạ tuyến tính $u : E'_b \to G$ sao cho $(u_n)$ hội tụ đơn giản đến u. Theo IV, p. 23, hệ quả, ta có $u \in \mathcal{L}_b(E'_b ; G)$. Khi đó suy ra từ mệnh đề 5 của GT, X, § 1, No. 5, rằng $(u_n)$ hội tụ đến u trong $\mathcal{L}_b(E'_b ; G)$.

#### Hệ quả {#evt-iv-s3-n3-cor-1 .statement}

— Đối đối ngẫu của một không gian lồi địa phương mêtric hóa được là một không gian Fréchet.

### 4. Đối ngẫu của một không gian Fréchet phản xạ

#### Mệnh đề 4 {#evt-iv-s3-prop-4 .statement}

— Cho E là một không gian Fréchet phản xạ. Đối ngẫu mạnh $E'_b$ của E là giới hạn quy nạp của một dãy các không gian Banach.

Cho $(V_n)_{n \in \mathbf{N}}$ là một dãy giảm các lân cận lồi, cân bằng và đóng của 0 trong E, sao cho mọi lân cận của 0 trong E đều chứa một trong các $V_n$. Cho $A_n$ là đối cực của $V_n$ trong $E'$. Khi đó $A_n$ là lồi, cân bằng và compact đối với $\sigma(E', E)$; theo III, p. 8, hệ quả không gian $E'_{A_n}$ là một không gian Banach. Ta sẽ chứng minh rằng $E'_b$ là giới hạn quy nạp của các không gian $E'_{A_n}$; nói cách khác, mọi tập con lồi và cân bằng U của $E'$ hấp thụ mỗi $A_n$ đều là một lân cận của 0 trong $E'_b$. Với mọi $n \in \mathbf{N}$, chọn một số thực $\lambda_n > 0$ sao cho $\lambda_n A_n \subset U$. Cho $B_n$ là bao lồi của tập hợp $\bigcup_{0 \leq i \leq n} \lambda_i A_i$; đặt $V = \bigcup_n B_n$, khi đó $V \subset U$. Với mọi $n \in \mathbf{N}$, tập hợp $B_n$ là lồi, cân bằng và compact đối với $\sigma(E', E)$ (II, p. 14, mệnh đề 15).

Bây giờ ta sẽ chứng minh rằng $\frac{1}{2} V^{oo} \subset V$. Cho $x \in E'_b - V$; với mọi $n \in \mathbf{N}$, ta có $x \notin B_n$, và vì $B_n$ là đóng đối với $\sigma(E', E)$ nên tồn tại một phần tử $y_n$ trong $B_n^\circ$ sao cho \langle y_n, x \rangle = 1 (\text{II, p. 38, mệnh đề 4}). Vì E là phản xạ, mọi tập con bị chặn của E đều tương đối compact đối với $\sigma(E, E')$ (IV, p. 16, định lý 2). Theo định nghĩa của $B_n$, ta có
$$
\lambda_i y_n \in V_i \quad \text{với mọi } n \geq i,
$$
do đó dãy $(y_n)$ là bị chặn. Gọi $y$ là một điểm giới hạn của $(y_n)$ đối với tôpô $\sigma(E, E')$. Ta có $y \in V^\circ = \bigcap_n B_n^\circ$ và $\langle y, x \rangle = 1$. Do đó $x \notin \frac{1}{2}V^{\circ\circ}$, và như vậy ta có bao hàm thức $\frac{1}{2}V^{\circ\circ} \subset V$ và *a fortiori*, $\frac{1}{2}V^{\circ\circ} \subset U$.

Vì mọi tập con bị chặn của $E'_b$ đều được chứa trong một trong các tập hợp $A_n$, tập hợp $V = \bigcup_n B_n$ hấp thụ mọi tập con bị chặn của $E'_b$. Do đó, $V^\circ$ bị chặn trong E, suy ra $\frac{1}{2}V^{\circ\circ}$ là một lân cận của 0 trong $E'_b$. *A fortiori*, U là một lân cận của trong $E'_b$.

#### Hệ quả {#evt-iv-s3-n4-cor-1 .statement}

*Đối ngẫu mạnh của một không gian Fréchet phản xạ là sinh Born và đầy thùng.*

Một giới hạn quy nạp của các không gian Banach là sinh Born theo định nghĩa. Hơn nữa, một không gian Banach là đầy thùng (III, p. 25, hệ quả) và mọi giới hạn quy nạp của các không gian đầy thùng là một không gian đầy thùng (III, p. 25, hệ quả 3).

### 5. Tôpô hội tụ compact trên đối ngẫu của một không gian Fréchet

#### Định lý 1 (Banach-Dieudonné) {#evt-iv-s3-thm-1 .statement}

— *Cho E là một không gian lồi địa phương mêtric hóa được. Các tôpô sau trùng nhau trên đối ngẫu $E'$ của E :*

a) *tôpô $\mathcal{T}_\mathfrak{N}$ của sự hội tụ $\mathfrak{N}$, trong đó $\mathfrak{N}$ là họ các tập con của E mỗi tập gồm các điểm của một dãy hội tụ về 0 ;*
b) *tôpô $\mathcal{T}_c$ của sự hội tụ đều trên các tập con compact của E ;*
c) *tôpô $\mathcal{T}_{pc}$ của sự hội tụ đều trên các tập con tiền compact của E ;*
d) *tôpô $\mathcal{T}_f$ là tôpô mịn nhất cảm sinh cùng tôpô như $\sigma(E', E)$ trên mọi tập con liên tục đều của $E'$.*

Trước hết nhận xét rằng *một tập con A của $E'$ là đóng đối với $\mathcal{T}_f$ khi và chỉ khi $A \cap H$ là đóng đối với $\sigma(E', E)$ với mọi tập con H của $E'$ là liên tục đều và đóng đối với $\sigma(E', E)$.* Tôpô yếu $\sigma(E', E)$ và $\mathcal{T}_{pc}$ cảm sinh cùng một tôpô trên mọi tập con liên tục đều của $E'$ (III, p. 17, mệnh đề 5). Do đó mỗi tôpô $\mathcal{T}_\mathfrak{N}$, $\mathcal{T}_c$, $\mathcal{T}_{pc}$, $\mathcal{T}_f$ đều thô hơn tôpô đứng sau nó. Vì vậy chỉ cần chứng minh rằng $\mathcal{T}_\mathfrak{N}$ mịn hơn $\mathcal{T}_f$. Hơn nữa, mọi phép tịnh tiến trong $E'$ là một đồng phôi đối với $\mathcal{T}_f$. Do đó chỉ cần chứng minh rằng, nếu F là một tập con của $E'$ đóng đối với $\mathcal{T}_f$, và không chứa 0, thì tồn tại một tập hợp $S \in \mathfrak{N}$ sao cho $S^\circ \cap F = \varnothing$.

Cho $(U_n)_{n \geq 0}$ là một dãy giảm các lân cận của 0 trong E lập thành một hệ cơ bản các lân cận của 0. Ta sẽ xây dựng, bằng quy nạp theo $n \geq 0$, các tập *hữu hạn* $X_n$ sao cho ta có
$$
X_n \subset U_n
$$
$$
\left( \bigcup_{0 \leq p \leq n} X_p \right)^\circ \cap U_{n+1}^\circ \cap F = \varnothing
$$

với mọi số nguyên $n \geqslant 0$. Cho $m \geqslant 0$ là một số nguyên sao cho $X_n$ đã được xây dựng với $0 \leqslant n < m$ và thỏa mãn (4) và (5) với $0 \leqslant n < m$. Với mọi $x \in U_m$, đặt
$$
F_x = (\bigcup_{0 \leqslant p < m} X_p)^{\circ} \cap \{x\}^{\circ} \cap U_{m+1}^{\circ} \cap F.
$$
Công thức (5) với $n = m - 1$ suy ra rằng $\bigcap_{x \in U_m} F_x = \varnothing$. Hơn nữa, tập $U_{m+1}^{\circ}$ là liên tục đều, và compact đối với $\sigma(E', E)$. Theo định nghĩa của $\mathcal{T}_f$, mỗi tập $F_x$ là compact đối với $\sigma(E', E)$; do đó tồn tại một tập con hữu hạn $X_m$ của $U_m$ sao cho $\bigcap_{x \in X_m} F_x = \varnothing$, *nghĩa là* quan hệ (5) được thỏa mãn với $n = m$.

Đặt $S = \bigcup_{n \geqslant 0} X_n$. Ta có $X_n \subset U_p$ với $n \geqslant p$, do đó $S$ là tập hợp các điểm của một dãy hội tụ về 0 trong $E$. Từ (5) ta suy ra rằng $S^{\circ} \cap U_{n+1}^{\circ} \cap F = \varnothing$, và vì $E'$ là hợp của dãy các tập hợp $U_{n+1}^{\circ}$, ta được $S^{\circ} \cap F = \varnothing$.

#### Hệ quả 1 {#evt-iv-s3-thm-1-cor-1 .statement}

*Cho $E$ là một không gian lồi địa phương mêtric hóa. Mọi tập con tiền compact của $E$ đều được chứa trong bao lồi cân bằng đóng của tập hợp các điểm của một dãy hội tụ về 0.*

Điều này suy ra từ sự kiện rằng các tôpô $\mathcal{T}_{pc}$ và $\mathcal{T}_{\mathfrak{H}}$ là đồng nhất, do Mệnh đề 2 của III, p. 15.

#### Hệ quả 2 {#evt-iv-s3-thm-1-cor-2 .statement}

*Cho $E$ là một không gian Fréchet. Để một tập con lồi $A$ của đối ngẫu $E'$ của $E$ là đóng đối với $\sigma(E', E)$, điều kiện cần và đủ là $A \cap U^{\circ}$ đóng đối với $\sigma(E', E)$ với mọi lân cận $U$ của 0 trong $E$.*

Vì $E$ là đầy đủ, tôpô $\mathcal{T}_c$ trên $E'$ là tương thích với đối ngẫu giữa $E'$ và $E$ (IV, p. 3, *Ví dụ*); do đó các tập con lồi đóng trong $E'$ là như nhau đối với $\mathcal{T}_c$ và $\sigma(E', E)$ (IV, p. 1, Mệnh đề 1). Hệ quả khi đó suy ra từ sự đồng nhất của các tôpô $\mathcal{T}_c$ và $\mathcal{T}_f$.

Nhắc lại (I, p. 13) rằng các siêu phẳng của $E'$ đóng đối với $\sigma(E', E)$ là các hạt nhân của các dạng tuyến tính trên $E'$ liên kết với các phần tử của $E$. Hệ quả 2 do đó cho một chứng minh khác (đối với các không gian Fréchet) của Hệ quả 1 của III, p. 21.

#### Hệ quả 3 {#evt-iv-s3-thm-1-cor-3 .statement}

*Mệnh đề: Cho $E$ là một không gian Banach và $M$ là một không gian con vectơ của đối ngẫu $E'$ của $E$. Để $M$ đóng đối với tôpô yếu $\sigma(E', E)$, điều kiện cần và đủ là giao của nó với quả cầu đơn vị (đóng) trong $E'$ đóng đối với $\sigma(E', E)$.*

#### Ví dụ {#evt-iv-s3-n5-exa-1 .statement}

— *Cho $H$ là một không gian Hilbert thỏa mãn tiên đề đếm được thứ nhất; ký hiệu $H_{\sigma}$ là không gian $H$ với tôpô yếu hơn được gán cho nó. Cho $\mathcal{L}^1(H)$ là không gian Banach của các tự đồng cấu hạt nhân của $H$ (V, p. 51, và TS, V); chuẩn trong $\mathcal{L}^1(H)$ được xác định bởi $\|u\|_1 = \operatorname{Tr}((u^*u)^{1/2})$. Ta có thể đồng nhất $\mathcal{L}(H)$ với đối ngẫu của không gian Banach $\mathcal{L}^1(H)$ bằng cách gắn dạng tuyến tính $\phi_u : v \mapsto \operatorname{Tr}(uv)$ trên $\mathcal{L}^1(H)$ với mỗi $u \in \mathcal{L}(H)$. Cho $A$ là một đại số con của $\mathcal{L}(H)$, chứa 1 và ổn định đối với $u \mapsto u^*$; đây là một đại số von Neumann khi và chỉ khi nó đóng trong $\mathcal{L}(H)$ đối với tôpô yếu $\sigma(\mathcal{L}(H), \mathcal{L}^1(H))$. Từ Hệ quả 3, ta suy ra tiêu chuẩn sau: *để $A$ là một đại số von Neumann, điều kiện cần và đủ là nếu $(u_n)$ là một dãy bất kỳ các phần tử của $A$ có chuẩn $\leqslant 1$ có giới hạn $u$ trong không gian $\mathcal{L}_s(H ; H_{\sigma})$, thì $u$ thuộc $A$.*

### 6. Các ánh xạ song tuyến tính liên tục riêng biệt

#### Bổ đề 1 {#evt-iv-s3-lem-1 .statement}

Cho E và F là hai không gian lồi địa phương mêtric hóa được, và u là một ánh xạ tuyến tính liên tục từ $E'_b$ vào F. Khi đó tồn tại một lân cận U của 0 trong $E'_b$ mà ảnh của nó qua u bị chặn trong F.

Cho $(U_n)_{n \in \mathbf{N}}$ (tương ứng $(V_n)_{n \in \mathbf{N}}$) là một hệ cơ bản các lân cận của 0 trong E (tương ứng F). Ta giả sử rằng các tập hợp $U_n$ là cân bằng và tạo thành một dãy giảm. Vì u liên tục, với mọi $n \in \mathbf{N}$, tồn tại một tập hợp bị chặn $B_n$ trong E sao cho $u(B_n^\circ) \subset V_n$. Vì $B_n$ bị chặn, tồn tại một số thực $\lambda_n > 0$ sao cho $\lambda_n B_n \subset U_n$. Đặt $B = \bigcup_{n \in \mathbf{N}} \lambda_n B_n$.

Ta sẽ chứng minh rằng tập hợp B bị chặn trong E, nói cách khác, với mọi số nguyên $m \geqslant 0$, tồn tại một số thực $\mu > 0$ sao cho $\mu B \subset U_m$. Vì các tập hợp $B_n$ bị chặn, tồn tại một số thực $\mu$ sao cho $0 < \mu \leqslant 1$ và sao cho $\mu (\lambda_n B_n) \subset U_m$ với $0 \leqslant n \leqslant m$; ta cũng có $\lambda_n B_n \subset U_n \subset U_m$ nếu $n > m$; do đó $\mu B \subset U_m$ vì $U_m$ là cân bằng.

Cho U là cực của B trong $E'_b$. Đây là một lân cận của 0 trong $E'_b$ và ta có $\lambda_n B^\circ \subset B_n^\circ$, do đó $\lambda_n u(U) \subset V_n$ với mọi $n \in \mathbf{N}$. Do đó $u(U)$ bị chặn trong F.

#### Định lý 2 {#evt-iv-s3-thm-2 .statement}

Cho $E_1$ và $E_2$ là hai không gian Fréchet phản xạ, và G là một không gian lồi địa phương Hausdorff. Với $i = 1, 2$, cho $F_i$ là đối ngẫu mạnh của $E_i$. Khi đó mọi ánh xạ song tuyến tính liên tục riêng $u : F_1 \times F_2 \to G$ đều liên tục.

Không gian G đẳng cấu với một không gian con của một tích các không gian Banach (II, p. 5, Mệnh đề 3). Do đó chỉ cần chứng minh định lý với giả thiết bổ sung rằng G là một không gian Banach. Nhưng $F_1$ là barrelled và $F_2$ là bornological (IV, p. 24, Hệ quả), còn $\mathscr{L}_b(F_2 ; G)$ là một không gian Fréchet (IV, p. 23, Mệnh đề 3). Ký hiệu v là ánh xạ tuyến tính từ $F_1$ vào $\mathscr{L}_b(F_2 , G)$ liên kết với u bởi quan hệ

$$
u(x_1, x_2) = v(x_1)(x_2) \quad (x_1 \in F_1, x_2 \in F_2).
$$

Vì $F_1$ là barrelled và u liên tục riêng, v liên tục (III, p. 31, Mệnh đề 6).

Vì v liên tục, Bổ đề 1 suy ra sự tồn tại của một lân cận $U_1$ của 0 trong $F_1$ mà ảnh của nó qua v bị chặn trong $\mathscr{L}_b(F_2 ; G)$. Nói cách khác, với mọi tập con bị chặn $B_2$ trong $F_2$, tập hợp $u(U_1 \times B_2)$ bị chặn trong không gian Banach G. Gọi $U_2$ là tập hợp tất cả các $x_2 \in F_2$ sao cho $\|u(x_1, x_2)\| \leqslant 1$ với mọi $x_1 \in U_1$. Khi đó tập hợp $U_2$ hấp thụ mọi tập con bị chặn; vì $F_2$ là bornological, $U_2$ là một lân cận của 0 trong $F_2$, và điều này chứng minh rằng u liên tục.

### Bài tập {#evt-iv-s3-exercises}

**T 1**) Cho $E$ là một không gian lồi địa phương khả metric, và $E'_b$ là đối ngẫu mạnh của nó. Nếu $E'_b$ khả metric, hãy chứng minh rằng tôpô của $E$ có thể được xác định bởi một chuẩn duy nhất (sử dụng III, p. 37, bài tập 2 và p. 38, bài tập 5, đồng thời sử dụng sự kiện rằng $E$ là bornological).

**T 2**) Một không gian infra-barrelled là semi-barrelled. Một không gian lồi địa phương được gọi là một *không gian* (DF) nếu nó là semi-barrelled và nếu bornology chính tắc (III, p. 3, định nghĩa 5) có một cơ sở đếm được. Mọi không gian chuẩn và mọi giới hạn quy nạp ngặt của một dãy các không gian chuẩn (II, p. 33) đều là một không gian (DF). Mọi đối ngẫu mạnh của một không gian Fréchet đều là một không gian (DF).
*a*) Đối ngẫu mạnh của một không gian (DF) là một không gian Fréchet.
*b*) Cho $E$ là một không gian (DF) và $(A_n)$ là một dãy tăng các tập con bị chặn, lồi, cân bằng và đóng của $E$ sao cho mọi tập con bị chặn của $E$ đều được một trong các $A_n$ hấp thụ.

Cho U là hợp của các $A_n$; hãy chứng minh rằng bao đóng $\overline{U}$ của U trong E chính xác là tập hợp tất cả các $x \in E$ sao cho $\lambda x \in U$ với $0 \leq \lambda < 1$. (Nếu $x \notin \lambda U$ với một $\lambda > 1$, thì với mọi $n$, tồn tại một dạng tuyến tính $x'_n \in E'$ sao cho $x'_n \in A_n^\circ$ và $\langle x, x'_n \rangle = \lambda$, và dãy $(x'_n)$ là equicontinuous, do đó có một điểm giới hạn yếu.)
c) Hãy chứng minh rằng nếu một không gian (DF) là barrelled, thì nó cũng là bornological ($cf.$ III, p. 44, bài tập 13, b)). Hãy cho ví dụ về các không gian (DF) không ultrabornological nhưng bornological và barrelled (III, p. 46, bài tập 22), và cả các không gian (DF) không barrelled nhưng bornological.

¶ 3) Cho E là một không gian lồi địa phương mêtric được, và $E'_b$ là đối ngẫu mạnh của nó.
a) Chứng minh rằng mọi tập con lồi cân bằng $V'$ của $E'_b$ hấp thụ các tập con bị chặn mạnh của $E'_b$ đều chứa một thùng (đối với tôpô mạnh) hấp thụ các tập con bị chặn mạnh của $E'_b$. (Cho $(K'_n)$ là một cơ sở đếm được của bornology chính tắc của $E'_b$ và cho $\lambda_n$ sao cho $\lambda_n K'_n \subset \frac{1}{2}V'$; áp dụng Bài tập 2, b) cho dãy $A'_n$, trong đó $A'_n$ là bao lồi của hợp của các $\lambda_j K'_j$ với $j \leq n$.)
b) Suy ra từ a) rằng các tính chất sau là tương đương :
$\alpha)$ E là distinguished (IV, p. 52, Bài tập 4).
$\beta)$ $E'_b$ là infrabarrelled (III, p. 44, Bài tập 7).
$\gamma)$ $E'_b$ là bornological.
$\delta)$ $E'_b$ là barrelled.
$\varepsilon)$ $E'_b$ là ultrabornological (III, p. 45, Bài tập 19).
c) Chứng minh rằng nếu $E'_b$ là phản xạ, thì $\hat{E} = E''$ (vốn hiển nhiên là phản xạ) ($cf.$ IV, p. 52, Bài tập 4 và p. 53, Bài tập 11).

4) Cho E là một không gian lồi địa phương Hausdorff, E' là đối ngẫu của nó. Nếu M là một không gian con vectơ đóng của E, mêtric được và distinguished (IV, p. 52, Bài tập 4), thì tôpô mạnh $\beta(E'/M^\circ, M)$ là tôpô thương theo $M^\circ$ của tôpô mạnh $\beta(E', E)$ (dùng Bài tập 3, b) và IV, p. 51, Bài tập 22, b)).

¶ 5) Với mọi số nguyên $n > 0$, đặt $a^{(n)}$ là dãy kép $(a_{pq}^{(n)})$ ($p \in \mathbf{N}, q \in \mathbf{N}$) sao cho $a_{pq}^{(n)} = q$ nếu $p \leq n$ và $a_{pq}^{(n)} = 1$ nếu $p > n$. Gọi E là không gian vectơ của mọi dãy kép $x = (x_{pq})_{(p,q) \in \mathbf{N} \times \mathbf{N}}$ các số thực sao cho, với mọi số nguyên $n > 0$, số $r_n(x) = \sum_{p,q} a_{pq}^{(n)} |x_{pq}|$ là hữu hạn. Nếu E được trang bị tôpô xác định bởi các nửa chuẩn $r_n$, thì E là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất (IV, p. 47, bài tập 1, c)); đối ngẫu E' của E có thể được đồng nhất với không gian của mọi dãy kép $x' = (x'_{pq})$ các số thực sao cho tồn tại ít nhất một chỉ số $n$, với một $k_n > 0$ thỏa mãn $|x'_{pq}| \leq k_n a_{pq}^{(n)}$ đối với mọi cặp $(p, q)$; và $\langle x, x' \rangle = \sum_{p,q} x_{pq} x'_{pq}$ (IV, p. 47, bài tập 1, c)).
Với mọi số nguyên $p_0 > 0$ và mọi dãy $(m_p)$ các số nguyên $> 0$, gọi $J(p_0; (m_p))$ là tập hợp các cặp số nguyên $p > 0, q > 0$ sao cho $p \geq p_0$ và $q \geq m_p$; gọi $\mathcal{B}$ là cơ sở lọc trên $\mathbf{N} \times \mathbf{N}$ gồm các tập hợp $J(p_0; (m_p))$ và gọi $\mathfrak{F}$ là một siêu lọc mịn hơn lọc có cơ sở $\mathcal{B}$.
a) Chứng minh rằng với mọi $x' = (x'_{pq}) \in E'$, dãy kép $(x'_{pq})$ có một giới hạn $u(x')$ đối với siêu lọc $\mathfrak{F}$; nếu $V_n$ là một lân cận của 0 trong E được xác định bởi $r_n(x) \leq 1$, thì $|u(x')| \leq 1$ đối với mọi $x' \in V_n^\circ$.
b) Gọi $U'$ là một lân cận của 0 trong $E'$, đối với tôpô mạnh, lồi, cân bằng và đóng yếu, và với mỗi $n$, gọi $\alpha_n > 0$ sao cho $\alpha_n V_n^\circ \subset U'$. Với mọi số nguyên $p > 0$, gọi $m_p$ là một số nguyên sao cho $2^{p+1} \leq \alpha_p m_p$, và gọi $x' = (x'_{pq})$ là dãy kép với $x'_{pq} = 0$ khi $q < m_p$, $x'_{pq} = 2$ khi $q \geq m_p$. Chứng minh rằng $x' \in U'$ nhưng $u(x') = 2$; suy ra rằng $u$ không liên tục mạnh trên $E'$, mặc dù bị chặn trên mọi tập con bị chặn của $E'$. Kết luận (IV, p. 58, bài tập 3) rằng E không distinguished, và do đó đối ngẫu mạnh $E'_b$ là một không gian (DF) không infra-barrelled.
c) Dùng b) để xây dựng một ví dụ về một không gian con đóng M của một không gian Fréchet F sao cho tôpô mạnh $\beta(F'/M^\circ, M)$ phân biệt với tôpô thương theo $M^\circ$ của tôpô mạnh $\beta(F', F)$ (nhúng E vào một tích đếm được các không gian Banach).

**T 6) a)** Cho E là một không gian (DF) (IV, p. 57, exerc. 2), và cho U là một tập hợp lồi sao cho với mọi tập con bị chặn, lồi và cân bằng A của E, $U \cap A$ là một lân cận của 0 đối với tôpô cảm sinh trên A bởi tôpô của E. Chứng minh rằng U là một lân cận của 0 trong A. (Cho $(A_n)$ là một cơ sở đếm được cho bornologie chính tắc của E (III, p. 3, def. 5). Chứng minh rằng, bằng quy nạp ta có thể định nghĩa một dãy $(\lambda_n)$ các số $> 0$ và một dãy $(V_n)$ các lân cận đóng, lồi và cân bằng của 0 trong E sao cho $\lambda_n A_n \subset \frac{1}{3} U, \lambda_n A_n \subset \bigcap_{j=1}^\infty V_j, V_n \cap A_n \subset U$ với mọi $n$.

Trước hết chứng minh rằng nếu $\lambda_j$ và $V_j$ đã được xây dựng với $j \leq n$, thì ta có thể tìm $\lambda_{n+1}$ sao cho $\lambda_{n+1} A_{n+1} \subset \frac{1}{3} U$ và $\lambda_{n+1} A_{n+1} \subset V_j$ với $j \leq n$. Tiếp theo chứng minh rằng ta có thể tìm $V_{n+1}$ sao cho $\lambda_j A_j \subset V_{n+1}$ với $j \leq n + 1$ và $V_{n+1} \cap A_{n+1} \subset U$; về điều này, đặt A là bao lồi của $\lambda_j A_j$ với $j \leq n + 1$, chứng minh rằng ta có thể lấy $V_{n+1} = \overline{A + V}$ với một lân cận lồi cân bằng thích hợp V của 0; ta nhận xét rằng đối với điều này chỉ cần chứng minh rằng, nếu $B = A_{n+1} \cap \complement U$, thì 0 không thuộc bao đóng của tập hợp $B + 2A$.
$b)$ Suy ra từ $a)$ rằng nếu $u$ là một ánh xạ tuyến tính từ E vào một không gian lồi địa phương F, sao cho hạn chế của $u$ trên mọi tập con bị chặn của E là liên tục, thì $u$ là liên tục ($cf.$ IV, p. 50, exerc. 15).

**T 7) a)** Cho E là một không gian (DF), U là một tập hợp lồi, cân bằng và đóng trong E, hấp thụ các tập con bị chặn của E, và cho $(x_n)$ là một dãy các điểm của $\complement U$. Chứng minh rằng tồn tại một lân cận V của 0 trong E không chứa bất kỳ $x_n$ nào. (Cho $(A_n)$ là một cơ sở đếm được cho bornologie chính tắc của E. Chứng minh rằng, bằng quy nạp ta có thể định nghĩa một dãy $(\lambda_n)$ các số $> 0$ và một dãy $(V_n)$ các lân cận lồi, cân bằng và đóng của 0 sao cho $\lambda_n A_n \subset \bigcap_{j=1}^\infty V_j, \lambda_n A_n \subset U$ và $x_n \in \complement V_n$ với mọi $n$. Về điều này, nếu $\lambda_j$ và $V_j$ đã được xây dựng với $j \leq n$, lấy $\lambda_{n+1}$ sao cho $\lambda_{n+1} A_{n+1} \subset U$ và $\lambda_{n+1} A_{n+1} \subset V_j$ với mọi $j \leq n$, rồi lấy $V_{n+1}$ chứa bao đóng của bao lồi của hợp của các $\lambda_j A_j$ với $j \leq n + 1$.
$b)$ Suy ra từ $a)$ rằng nếu M là một tập con của E chứa một tập hợp đếm được trù mật khắp nơi, thì tôpô cảm sinh trên M bởi tôpô mạnh của song đối ngẫu $E''$ của E là đồng nhất với tôpô cảm sinh bởi tôpô của E. Đặc biệt, các dãy hội tụ trong E là như nhau đối với tôpô của E và đối với tôpô cảm sinh bởi tôpô mạnh của $E''$; với mọi tập con mêtric hóa được M của E, tôpô cảm sinh trên M bởi tôpô của E là đồng nhất với tôpô cảm sinh bởi tôpô mạnh của $E''$.
$c)$ Suy ra từ $a)$ rằng nếu tồn tại một tập hợp đếm được trù mật khắp nơi trong E, thì E là infra-barrelled.
$d)$ Suy ra từ $b)$ và từ exerc. 6 rằng nếu mọi tập con bị chặn của E là mêtric hóa được đối với tôpô cảm sinh bởi tôpô của E, thì E là infrabarrelled.

**T 8) Cho E là một không gian Fréchet, $E'_b$ là đối ngẫu mạnh của nó. Giả sử tồn tại một dãy trù mật khắp nơi $(x'_n)$ trong $E'_b$. Chứng minh rằng E thỏa mãn tiên đề đếm được thứ nhất. (Gọi $(K'_n)$ là một cơ sở đếm được của bao sinh chính tắc của $E'_b$ gồm các tập hợp lồi cân bằng đóng. Với mỗi hệ $\alpha$ gồm một điểm $x'_n$, một số hữu hạn tùy ý các số hữu tỉ $\lambda_k > 0 (1 \leq k \leq m)$ và m chỉ số $n_k$ sao cho $x'_n \notin 2 \sum_{k=1}^m \lambda_k K'_{n_k} = 2H'_\alpha$, hãy lấy $x_\alpha \in E$ sao cho siêu phẳng có phương trình $\langle x_\alpha, y' \rangle = 1$ phân cách nghiêm ngặt hai tập hợp compact yếu $H'_\alpha$ và $x'_n + H'_\alpha$. Chứng minh rằng với mọi $x' \neq 0$ trong $E'$, tồn tại một hệ $\alpha$ sao cho $\langle x_\alpha, x' \rangle \neq 0$. Để làm điều này, xét một lân cận V' của 0 trong $E'_b$ sao cho $V' \cap (x' + V') = \varnothing$, rồi với mỗi số nguyên $m$, lấy một số hữu tỉ $\lambda_m > 0$ sao cho $\lambda_m K'_m \subset V'$; sử dụng sự kiện rằng hợp $U' \subset V'$ của các $\lambda_m K'_m$ là một lân cận của 0 (exerc. 7, và IV, p. 58, exerc. 3, $b$) ) và rằng tồn tại $n$ sao cho $x'_n \in x' + U'$.)

**T 9) a)** Cho E là một không gian Hausdorff nửa-barrelled, M là một không gian vectơ con đóng của E và $E'$ là đối ngẫu của E. Chứng minh rằng $E/M$ là nửa-barrelled và tôpô mạnh $\beta(M^\circ, E/M)$ trùng với tôpô cảm sinh trên $M^\circ$ bởi tôpô mạnh $\beta(E', E)$. (Chú ý rằng chỉ cần chứng minh rằng một dãy $(x'_n)$ trong $M^\circ$ hội tụ về 0 đối với $\beta(E', E)$ là bị chặn đối với $\beta(M^\circ, E/M)$.) Suy ra rằng nếu E là một không gian (DF), thì $E/M$ cũng vậy ($cf.$ IV, p. 63, exerc. 8).

b) Cho E là một không gian lồi địa phương Hausdorff, M là một không gian vectơ con (không nhất thiết đóng) của E. Chứng minh rằng nếu M là một không gian nửa-barrelled, thì tôpô mạnh $\beta(E'/M^\circ, M)$ trùng với tôpô thương theo M^\circ của tôpô mạnh $\beta(E', E)$. (Lập luận như trong a.)

c) Chứng minh rằng một không gian Hausdorff và nửa-barrelled quasi-đầy đủ E là đầy đủ (áp dụng b) cho E và $\hat{E}$). Đặc biệt, một không gian nửa-barrelled, nửa-phản xạ là đầy đủ (*cf.* IV, p. 52, exerc. 6).

d) Chứng minh rằng phép hoàn thành của một không gian Hausdorff nửa-barrelled (tương ứng (DF)) là nửa-barrelled (tương ứng là một không gian (DF)).

e) Cho $(E_n)$ là một dãy các không gian nửa-barrelled (tương ứng (DF)), E là một không gian vectơ, và với mỗi n, cho $f_n$ là một ánh xạ tuyến tính từ $E_n$ vào E. Giả sử rằng E là hợp của các $f_n(E_n)$; hãy chứng minh rằng, E là nửa-barrelled (tương ứng là một không gian (DF)) đối với tôpô lồi địa phương mịn nhất mà tất cả các $f_n$ đều liên tục (trước hết xét trường hợp E là tổng trực tiếp tôpô của các $E_n$). Nếu các $E_n$ là nửa-phản xạ (tương ứng phản xạ) và nếu E là Hausdorff, thì E là nửa-phản xạ (tương ứng phản xạ).

10) Cho E là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất. Chứng minh rằng nếu trong đối ngẫu $E'$ của E, mọi dãy hội tụ đối với tôpô yếu $\sigma(E', E)$ cũng hội tụ đối với tôpô mạnh $\beta(E', E)$, thì E là một không gian Montel. (Chứng minh rằng mọi tập hợp bị chặn của $E'$ là tương đối compact đối với tôpô mạnh; sử dụng GT, II, § 4, exerc. 6; rồi sử dụng IV, p. 53, exerc. 11, b).)

11) Cho $(c_{mn})$ là một dãy kép các số $> 0$ sao cho $c_{m,n} \leq c_{m+1,n}$ và cho E là không gian của tất cả các dãy $x = (x_n)$ các số thực sao cho $p_m(x) = \sum_n c_{mn} |x_n| < +\infty$ với mọi số nguyên m. Ta trang bị cho E tôpô được xác định bởi các nửa chuẩn $p_m$ và đối với tôpô này E là một không gian Fréchet thỏa mãn tiên đề đếm được thứ nhất; đối ngẫu $E'$ của E có thể được đồng nhất với không gian của tất cả các dãy $x' = (x'_n)$ sao cho $\sup_n c_{mn}^{-1} |x'_n| < +\infty$ với ít nhất một m, dạng song tuyến tính chính tắc $\langle x, x' \rangle$ được đồng nhất với $\sum_n x_n x'_n$ (IV, p. 47, bài tập 1, c)). Giả sử rằng không tồn tại dãy con nào $(n_k)$ sao cho tồn tại một dãy $(a_m)$ các số $\geq 0$ và một chỉ số $m_0$ sao cho $c_{m,n_k} \leq a_m c_{m_0,n_k}$ với mọi $m \geq m_0$ và với mọi k. Dưới các điều kiện này, mọi dãy hội tụ yếu trong $E'$ đều hội tụ mạnh và do đó (IV, p. 60, bài tập 10) E là một không gian Montel. (Lập luận bằng *reductio ad absurdum*; nếu cần thiết hãy thực hiện một biến đổi dạng $(x_n) \mapsto (a_n x_n)$ để rút gọn về trường hợp $c_{m_0 n} = 1$ với mọi n và một $m_0$ nào đó, và trong đó tồn tại một dãy $(x^{(p)})_{p \geq 0}$ hội tụ yếu về 0 trong E', và thỏa mãn $|x^{(p)}_n| \leq 1$ với mọi cặp $(p, n)$, đồng thời tồn tại một tập hợp bị chặn B trong E, được xác định bởi $p_m(x) \leq b_m$ với mọi $m \geq 0$ và sao cho $\sup_{x \in B} |\langle x, x^{(p)} \rangle| \geq 2\delta > 0$ với mọi số nguyên p. Với các giả thiết này, hãy chứng minh rằng tồn tại một dãy tăng ngặt $(r_q)$ các số nguyên, và một dãy $(x^{(q)})$ các điểm của B sao cho

$$
\sum_{k=r_q+1}^{r_q+1} |x^{(q)}_k| > \delta
$$

với mỗi chỉ số q. Sau đó hãy chứng minh, bằng *reductio ad absurdum*, rằng với mọi q, tồn tại ít nhất một chỉ số $s_q$ sao cho $r_q < s_q \leq r_{q+1}$ và rằng với mọi số nguyên m, ta có $c_{m,s_q} \leq b_m 2^{m+2}/\delta$, điều này mâu thuẫn với giả thiết.)

12) a) Cho F là một không gian Hausdorff (DF), và $F'_b$ là đối ngẫu mạnh của nó. Hãy chứng minh rằng nếu $F'_b$ là phản xạ, thì bao hoàn thiện $\hat{F}$ của F là phản xạ và bằng đối ngẫu kép $F''$ của F (*cf.* IV, p. 52, bài tập 4 và p. 53, bài tập 11).
b) Cho E là một không gian Fréchet. Hãy chứng minh rằng nếu đối ngẫu kép $E''$ của E là phản xạ, thì E là phản xạ.

13) a) Cho E, F là hai không gian Fréchet, G là một không gian lồi địa phương Hausdorff và E', F', G' lần lượt là các đối ngẫu của E, F, G. Cho $u$ là một ánh xạ song tuyến tính từ $E' \times F'$ vào $G'$, riêng liên tục (III, p. 28) khi E', F', G' được gán các tôpô yếu $\sigma(E', E)$, $\sigma(F', F)$ và $\sigma(G', G)$. Hãy chứng minh rằng dưới các điều kiện này, $u$ là một ánh xạ liên tục từ $E' \times F'$ vào $G'$ khi E', F' và G' được gán các tôpô mạnh. (Đối với $z \in G$, đặt \langle z, u(x', y') \rangle = \langle v_z(x'), y' \rangle \text{ trong đó } v_z(x') \in F. \text{ Trước hết hãy chứng minh rằng nếu } E' \text{ được gán tôpô mạnh và } F \text{ tôpô ban đầu, thì } \text{tập hợp của tất cả } v_z, \text{ khi } z \text{ chạy qua một tập hợp bị chặn } C \text{ trong } G, \text{ là liên tục đều; hãy dùng cho việc này IV, p. 51, bài tập 19, } d). \text{ Tiếp theo hãy chứng minh rằng tồn tại một lân cận } V' \text{ của } 0 \text{ đối với tôpô mạnh của } E' \text{ sao cho hợp của các tập hợp } v_z(V') \text{ khi } z \text{ chạy qua } C \text{ là bị chặn trong } F; \text{ hãy dùng cho việc này III, p. 47, bài tập 5.)}
b) Hãy cho một ví dụ để chỉ ra rằng kết luận của $a)$ không đúng nếu giả sử rằng $E$ là một không gian Fréchet và $F$ là một giới hạn quy nạp ngặt của các không gian Fréchet (III, p. 47, bài tập 3).

14) $a)$ Cho $E$ là một không gian Fréchet, $E'$ là đối ngẫu của nó. Hãy chứng minh rằng $E'$, được trang bị tôpô hội tụ compact hoặc một $\mathcal{S}$-tôpô mịn hơn, là đầy đủ ($cf.$ III, p. 22, *Nhận xét* 1). Nếu $E$ không phản xạ, hãy chứng minh rằng $E'$ không infrabarrelled đối với bất kỳ $\mathcal{S}$-tôpô nào mịn hơn tôpô hội tụ compact và thô hơn $\tau(E', E)$.
$b)$ Cho $(E_\alpha)_{\alpha \in A}$ là một họ các không gian Fréchet, $E$ là một không gian vectơ và với mọi $\alpha \in A$, cho $h_\alpha$ là một ánh xạ tuyến tính từ $E_\alpha$ vào $E$. Giả sử rằng $E$, được trang bị tôpô lồi địa phương mịn nhất mà đối với đó các $h_\alpha$ liên tục (II, p. 27), là Hausdorff. Hãy chứng minh rằng đối ngẫu $E'$ của $E$, được trang bị tôpô hội tụ compact hoặc bất kỳ $\mathcal{S}$-tôpô nào mịn hơn, là đầy đủ ($cf.$ III, p. 20, th.

Xem [các bài tập của § 3](exercises/s3/).
