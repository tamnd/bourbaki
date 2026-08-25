---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 3
section_title: Faithfully flat modules
lang: vi
source: ac-i-vii
book_pages: 27-36, 49-50
pdf_pages: 0047-0056, 0069-0070
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF FAITHFULLY FLAT MODULES
      page: 27
      pdf_page: 47
    - "no": 2
      title: TENSOR PRODUCTS OF FAITHFULLY FLAT MODULES
      page: 30
      pdf_page: 50
    - "no": 3
      title: CHANGE OF RING
      page: 31
      pdf_page: 51
    - "no": 4
      title: RESTRICTION OF SCALARS
      page: 31
      pdf_page: 51
    - "no": 5
      title: FAITHFULLY FLAT RINGS
      page: 32
      pdf_page: 52
    - "no": 6
      title: FAITHFULLY FLAT RINGS AND FINITENESS CONDITIONS
      page: 34
      pdf_page: 54
    - "no": 7
      title: LINEAR EQUATIONS OVER A FAITHFULLY FLAT RING
      page: 35
      pdf_page: 55
statements: 18
exercises: 10
content_sha256: 8b587a9f5f49785d7231e6426948fabc756a6cc0be21aea41054c0a7508c31bb
translated_from: content/en/ac/I/03_s3_faithfully_flat_modules.md
source_content_sha256: 6eca3d9ab803d413bfaf6f39a861f11ddce5dbf12fbed96d89ca819c7210a451
translation_model: gpt-5-6-mini, gpt-5.4-mini
translation_run: translate-vi-15ae5fed
glossary_version: 34
glossary_terms_sha256: d9c9956f5f2e4a64acd4a1a3a389567370f787763f32fd137ef5404a692d4338
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## 3. CÁC MÔĐUN PHẲNG TRUNG THÀNH

### 1. ĐỊNH NGHĨA CÁC MÔĐUN PHẲNG TRUNG THÀNH

#### Mệnh đề 1 {#ac-i-s3-prop-1 .statement}

Cho $E$ là một $A$-môđun phải. Bốn tính chất sau là tương đương:

(a) Đối với một dãy $N' \xrightarrow{v} N \xrightarrow{w} N''$ các $A$-môđun trái là khớp, điều kiện cần và đủ là dãy
$$
E \otimes_A N' \xrightarrow{1 \otimes v} E \otimes_A N \xrightarrow{1 \otimes w} E \otimes_A N''
$$
là khớp.

(b) $E$ là phẳng và, với mọi $A$-môđun trái $N$, quan hệ $E \otimes_A N = 0$ kéo theo $N = 0$.

(c) $E$ là phẳng và, với mọi đồng cấu $v : N' \to N$ của các $A$-môđun trái, quan hệ $1_E \otimes v = 0$ kéo theo $v = 0$.

(d) $E$ là phẳng và, với mọi iđêan trái cực đại $m$ của $A$, $E \neq Em$.

Để đơn giản hóa cách viết, ta đặt $T(Q) = E \otimes_A Q$ đối với mọi $A$-môđun trái $Q$ và $T(v) = 1_E \otimes v$ đối với mọi đồng cấu $v$ của các $A$-môđun trái.

Trước hết ta chứng minh sự tương đương của (a), (b) và (c).

Ta chứng minh rằng (a) kéo theo (b). Nếu (a) đúng, rõ ràng $E$ là phẳng (\$2, no. 3, Mệnh đề 1). Mặt khác, cho $N$ là một $A$-môđun trái sao cho $T(N) = 0$ và xét dãy $0 \to N \to 0$; giả thiết $T(N) = 0$ có nghĩa là dãy $0 \to T(N) \to 0$ là khớp. Theo (a), dãy $0 \to N \to 0$ là khớp, do đó $N = 0$.

Ta chứng minh rằng (b) kéo theo (c). Giả sử (b) đúng và cho $u : N' \to N$ là một đồng cấu và $I$ là ảnh của nó. Vì ảnh của $T(v)$ được đồng nhất với $T(I)$ (\$2, no. 3, Nhận xét 2), giả thiết $T(v) = 0$ kéo theo $T(I) = 0$, do đó $I = 0$ theo (b) và do đó $v = 0$.

Ta chứng minh rằng (c) kéo theo (a). Khi đó giả sử (c) đúng và xét một dãy
$$
N' \xrightarrow{v} N \xrightarrow{w} N''
$$
các đồng cấu của các $A$-môđun trái và dãy tương ứng
$$
T(N') \xrightarrow{T(v)} T(N) \xrightarrow{T(w)} T(N'').
$$

Nếu dãy (1) là khớp, thì (2) cũng khớp, vì $E$ là phẳng (\$2, no. 3, Mệnh đề 1). Ngược lại, nếu (2) là khớp, trước hết ta có $T(w \circ v) = T(w) \circ T(v) = 0$, do đó $w \circ v = 0$ theo giả thiết. Đặt $I = v(N')$ và $K = \overline{w}(0)$; khi đó $I$ được chứa trong $K$ theo điều trên. Xét dãy khớp
$$
0 \to I \xrightarrow{i} K \xrightarrow{p} K/I \to 0
$$
trong đó $i$ và $p$ là các ánh xạ chính tắc. Vì $E$ là phẳng, dãy
$$
0 \to T(I) \xrightarrow{T(i)} T(K) \xrightarrow{T(p)} T(K/I) \to 0
$$
là khớp, nói cách khác, $T(K/I)$ là đẳng cấu với $T(K)/T(I)$, mà bằng 0 theo giả thiết, vì $T(I)$ (tương ứng $T(K)$) được đồng nhất với ảnh của $T(v)$ (tương ứng hạt nhân của $T(w)$) (\$2, no. 3, Nhận xét 2). Nhưng quan hệ $T(p) = 0$ suy ra $p = 0$ theo giả thiết, do đó $K = I$, điều này chứng minh rằng dãy (1) là khớp.

Cuối cùng ta chứng minh sự tương đương của (b) và (d). Nếu (b) đúng, thì

$$
E/E_m = E \otimes_A (A_s/m) \neq 0
$$

vì $A_s/m \neq 0$; do đó (d). Ngược lại, giả sử (d) đúng; mọi iđêan trái $a \neq A$ của $A$ đều được chứa trong một iđêan trái cực đại $m$ (*Algebra*, Chương I, §8, no. 7, Định lý 2), khi đó giả thiết $E \neq Em$ suy ra $E \neq Ea$, nói cách khác, $E \otimes_A (A_s/a) \neq 0$. Điều đó có nghĩa là, với mọi môđun trái $A$ đơn sinh $N \neq 0$, $T(N) \neq 0$. Nếu bây giờ $N$ là một môđun trái $A$ bất kỳ \#0, nó chứa một môđun con đơn sinh $N' \neq 0$; vì $E$ là phẳng, $T(N')$ được đồng nhất với một nhóm con của $T(N)$; ta vừa thấy rằng $T(N') \neq 0$, do đó $T(N) \neq 0$.

#### Định nghĩa 1 {#ac-i-s3-def-1 .statement}

*Một môđun phải $A$* $E$ *được gọi là phẳng trung thành nếu nó thỏa mãn bốn điều kiện tương đương của Mệnh đề 1.*

Các môđun trái $A$ phẳng trung thành được định nghĩa tương tự; rõ ràng, để một môđun trái $A$ $E$ là phẳng trung thành, điều kiện cần và đủ là $E$, được xem như một môđun phải $A^0$, là phẳng trung thành.

#### Nhận xét {#ac-i-s3-n1-rem-1 .statement}

Nếu $E$ là một môđun $A$ phẳng trung thành, thì $E$ là một môđun $A$ *trung thành*: thật vậy, nếu một phần tử $a \in A$ sao cho $xa = 0$ với mọi $x \in E$, phép vị tự $h : b \mapsto ba$ trong $A$ có tính chất $1, \otimes h = 0$; do đó $h = 0$ theo tính chất (c) của Mệnh đề 1, tức là $a = 0$ vì $A$ có một phần tử đơn vị.

*Ví dụ*
(1) Tổng trực tiếp của một môđun phẳng và một môđun phẳng trung thành là một môđun phẳng trung thành nhờ tính chất (d) của Mệnh đề 1 và § 2, no. 3, Mệnh đề 2.
(2) *Vì $A$*, là phẳng trung thành nhờ tiêu chuẩn (d) của Mệnh đề 1 và § 2, no. 4, *Ví dụ* 1, suy ra từ (1) rằng mọi môđun tự do *không rút gọn về 0* đều là phẳng trung thành. Mặt khác, tồn tại các nhân tử trực tiếp khác không của các môđun tự do (nói cách khác, các môđun xạ ảnh khác không) trung thành nhưng *không phẳng trung thành* (Bài tập 2).
(3) Cho $A$ là một *miền iđêan chính*. Để một $A$-môđun $E$ là phẳng trung thành, điều kiện cần và đủ là nó xoắn tự do và $E \neq Ep$ với mọi phần tử bất khả quy (*Đại số*, Chương VII, § 1, no. 3) $p$ của $A$; điều này suy ra ngay lập tức từ § 2, no. 4, Mệnh đề 3 và tiêu chuẩn (d) của Mệnh đề 1.
(4) Ví dụ (3) chỉ ra rằng $\mathbf{Z}$-môđun $\mathbf{Q}$ là một môđun phẳng và trung thành, nhưng *không phẳng trung thành*.

#### Mệnh đề 2 {#ac-i-s3-prop-2 .statement}

*Cho $E$ là một $A$-môđun phải phẳng trung thành và $u : N' \to N$ là một đồng cấu $A$-môđun trái. Để $u$ là đơn ánh (tương ứng. toàn ánh, song ánh), điều kiện cần và đủ là $1_E \otimes u : E \otimes_A N' \to E \otimes_A N$ cũng là như vậy.*

Đây là một hệ quả ngay lập tức của tiêu chuẩn (a) của Mệnh đề 1.

#### Mệnh đề 3 {#ac-i-s3-prop-3 .statement}

Cho $0 \to E' \to E \to E'' \to +0$ là một dãy khớp của các $A$-môđun phải. Giả sử rằng $E'$ và $E''$ là phẳng và một trong chúng là phẳng trung thành. Khi đó $E$ là phẳng trung thành.

Ta đã biết rằng $E$ là phẳng ($\S 2$, no. 5, Mệnh đề 5). Ta kiểm tra rằng $E$ có tính chất (b) của Mệnh đề 1. Cho $N$ là một $A$-môđun trái. Vì $E''$ là phẳng, có một dãy khớp

$$
0 \to E' \otimes_A N \to E \otimes_A N \to E'' \otimes_A N \to 0
$$

($\S 2$, no. 5, Mệnh đề 4). Nếu $E \otimes_A N = 0$, suy ra rằng $E' \otimes_A N$ và $E'' \otimes_A N$ bằng không; vì một trong các môđun $E'$, $E''$ là phẳng trung thành, điều này kéo theo $N = 0$.

### 2. TÍCH TENXƠ CỦA CÁC MÔĐUN PHẲNG TRUNG THÀNH

#### Mệnh đề 4 {#ac-i-s3-prop-4 .statement}

Cho $R, S$ là hai vành, $E$ là một $R$-môđun phải và $F$ là một song môđun $(R, S)$. Giả sử rằng $E$ là phẳng trung thành. Khi đó, để $F$ là một $S$-môđun phẳng (tương ứng. phẳng trung thành), điều kiện cần và đủ là $E \otimes_R F$ cũng như vậy.

(1) Nếu $F$ là phẳng, $E \otimes_R F$ là phẳng ($\S 2$, no. 7, Mệnh đề 8).

(2) Giả sử rằng $E \otimes_R F$ là phẳng và cho $\nu : N' \to N$ là một đồng cấu $S$-môđun trái đơn ánh. Đồng cấu

$$
l_E \otimes l_F \otimes \nu : E \otimes_R F \otimes_S N' \to E \otimes_R F \otimes_S N
$$

khi đó là đơn ánh ($\S 2$, no. 3, Mệnh đề 1). Suy ra từ Mệnh đề 2 của no. 1 rằng $l_F \otimes \nu : F \otimes_S N' \to F \otimes_S N$ là đơn ánh; khi đó $F$ là một $S$-môđun phẳng ($\S 2$, no. 3, Mệnh đề 1).

(3) Giả sử $F$ phẳng trung thành và cho $N$ là một môđun trái $S$ sao cho $E \otimes_R F \otimes_S N = 0$. Vì $E$ phẳng trung thành, điều này suy ra rằng $F \otimes_S N = 0$, do đó $N = 0$ vì $F$ phẳng trung thành; điều này chứng tỏ rằng $E \otimes_R F$ phẳng trung thành.

(4) Giả sử $E \otimes_R F$ phẳng trung thành và cho $N$ là một môđun trái $S$ sao cho $F \otimes_S N = 0$. Khi đó $E \otimes_R F \otimes_S N = 0$, do đó $N = 0$, điều đó cho thấy rằng $F$ phẳng trung thành.

#### Hệ quả {#ac-i-s3-n2-cor-1 .statement}

Cho $C$ là một vành giao hoán và $E$ và $F$ là hai C-môđun phẳng trung thành. Khi đó C-môđun $E \otimes_C F$ phẳng trung thành.

Áp dụng Mệnh đề 4 với $R = S = C$.

### 3. THAY ĐỔI VÀNH

#### Mệnh đề 5 {#ac-i-s3-prop-5 .statement}

Cho $\rho$ là một đồng cấu từ một vành $A$ đến một vành $B$. Nếu $E$ là một môđun phải $A$ phẳng trung thành, thì môđun phải $B$ $\rho^*(E) = E_{(B)} = E \otimes_A B$ phẳng trung thành.

Áp dụng Mệnh đề 4 của no. 2 với $R = A, S = F = B$, chú ý rằng $B$-môđun $B_d$ phẳng trung thành.

#### Hệ quả {#ac-i-s3-n3-cor-1 .statement}

*Nếu $E$ là một môđun phải $A$ phẳng trung thành và nếu $a$ là một iđêan hai phía của $A$, thì môđun phải $(A/a)$ $E/Ea$ phẳng trung thành.*

Áp dụng Mệnh đề 5 với $B = A/a, \rho$ là đồng cấu chính tắc.

#### Mệnh đề 6 {#ac-i-s3-prop-6 .statement}

Cho $A$ là một vành giao hoán, $B$ là một đại số trên $A$ và $\rho : a \mapsto a . 1$ là đồng cấu chính tắc của $A$ đến $B$. Giả sử rằng $B$ là một A-môđun phẳng trung thành. Khi đó, để một A-môđun $E$ là phẳng (tương ứng phẳng trung thành), cần và đủ rằng môđun phải $B$ $E_{(B)} = E \otimes_A B$ là phẳng (tương ứng phẳng trung thành).

(1) Nếu $E$ phẳng (tương ứng phẳng trung thành), thì $E_{(B)}$ phẳng (tương ứng phẳng trung thành) theo § 2, no. 7, Hệ quả 2 của Mệnh đề 8 (tương ứng bởi Mệnh đề 5).

(2) Giả sử rằng $E_{(B)}$ là phẳng và cho $\nu : N' \to N$ là một đồng cấu A-môđun đơn ánh. Theo § 2, no. 7, Hệ quả 3, $A$-môđun $E \otimes_A B$ là phẳng, do đó đồng cấu $1, \otimes 1_B \otimes \nu : E \otimes_A B \otimes_A N' \to E \otimes_A B \otimes_A N$ là đơn ánh. Vì các cấu trúc A-môđun phải và trái trên B trùng nhau, đồng cấu này được đồng nhất với

$$
1_E \otimes \nu \otimes 1_B : E \otimes_A N' \otimes_A B \to E \otimes_A N \otimes_A B.
$$

Vì $B$ là một A-môđun phẳng trung thành, suy ra $1_E \otimes \nu : E \otimes_A N' \to E \otimes_A N$ là đơn ánh (no. 1, Mệnh đề 2), điều đó cho thấy $E$ là phẳng.

(3) Cuối cùng, giả sử $E_{(B)}$ là phẳng trung thành. Trước hết $E$ là phẳng theo (2). Đồng thời, cho $N$ là một A-môđun sao cho $E \otimes_A N = 0$. Khi đó $E \otimes_A N \otimes_A B = 0$, do đó, vì các cấu trúc A-môđun phải và trái trên B trùng nhau, $E \otimes_A B \otimes_A N = 0$, cũng có thể viết là $(E \otimes_A B) \otimes_B (B \otimes_A N) = 0$. Vì $E_{(B)}$ là một B-môđun phẳng trung thành, suy ra $B \otimes_A N = 0$ (no. 1, Mệnh đề 1), do đó $N = 0$ vì $B$ là một A-môđun phẳng trung thành (no. 1, Mệnh đề 1).

### 4. HẠN CHẾ CỦA CÁC VÔ HƯỚNG

#### Mệnh đề 7 {#ac-i-s3-prop-7 .statement}

*Cho $A, B$ là hai vành và $\rho$ là một đồng cấu từ $A$ đến $B$. Cho $E$ là một B-môđun phải phẳng trung thành. Để $\rho^*(E)$ là một A-môđun phải phẳng (tương ứng phẳng trung thành), thì điều kiện cần và đủ là $B$ là một A-môđun phải phẳng (tương ứng phẳng trung thành).*

Áp dụng Mệnh đề 4 của no. 2 với $B, A, E, B$ lần lượt thay cho $R, S, E, F$, và với cấu trúc A-môđun phải trên $B$ được xác định bởi $\rho$, ta thấy rằng

B là một A-môđun phẳng (tương ứng phẳng trung thành) khi và chỉ khi $E \otimes_B B = \rho^*(E)$ là một A-môđun phẳng (tương ứng phẳng trung thành).

Nhận xét
(1) Mệnh đề 7 cho thấy rằng, để $B$ là một A-môđun phẳng trung thành, chỉ cần tồn tại một B-môđun phẳng trung thành cũng là một A-môđun phẳng trung thành.
(2) Cho $A, B, C$ là ba vành và $\rho : A \to B, \sigma : B \to C$ là hai đồng cấu vành. Mệnh đề 7 cho thấy rằng nếu $C$ là một B-môđun phẳng trung thành và $B$ là một A-môđun phẳng trung thành, thì $C$ là một A-môđun phẳng trung thành. Nếu $C$ là một B-môđun phẳng trung thành và một A-môđun phẳng trung thành, thì $B$ là một A-môđun phẳng trung thành (lấy các môđun là môđun phải, để cố định ý tưởng). Mặt khác $B$ và $C$ có thể là các A-môđun phẳng trung thành mà $C$ không là một B-môđun phẳng trung thành (Bài tập 7).

### 5. CÁC VÀNH PHẲNG TRUNG THÀNH

#### Mệnh đề 8 {#ac-i-s3-prop-8 .statement}

Cho $A, B$ là hai vành và $\rho$ là một đồng cấu từ $A$ đến $B$. Giả sử tồn tại một B-môđun phải $E$ sao cho $\rho_*(E)$ là một A-môđun phẳng trung thành. Khi đó:
(i) Với mọi A-môđun trái $F$, đồng cấu chính tắc $j : F \to F_{(B)} = B \otimes_A F$ (sao cho $j(x) = 1 \otimes x$ với mọi $x \in F$) là đơn ánh.
(ii) Với mọi iđêan trái cực đại $\mathfrak{a}$ của $A$, $\overline{\rho}^{-1}(B\mathfrak{a}) = \mathfrak{a}$.
(iii) Đồng cấu $\rho$ là đơn ánh.
(iv) Với mọi iđêan trái cực đại $\mathfrak{m}$ của $A$, tồn tại một iđêan trái cực đại $\mathfrak{n}$ của $B$ sao cho $\overline{\rho}^{-1}(\mathfrak{n}) = \mathfrak{m}$.

Chứng minh (i). Ta biết (Đại số, Chương 11, § 5, no. 2, Hệ quả của Mệnh đề 5) rằng với mọi B-môđun phải $M$, đồng cấu chính tắc của $A$-môđun $i : M \to \rho_*(M) \otimes_A B = \rho^*(\rho_*(M))$ được định nghĩa bởi $i(y) = y \otimes 1$ là đơn ánh và rằng A-môđun $i(M)$ là một nhân tử trực tiếp của $\rho_*(M) \otimes_A B$. Do đó, với mọi A-môđun trái $F$,

$$
i \otimes 1_F : \rho_*(M) \otimes_A F \to \rho_*(M) \otimes_A B \otimes_A F
$$

là đơn ánh (\S 2, no. 1, Bổ đề 2). Lấy $M = E$, suy ra (vì $i \otimes 1_F = 1_M \otimes j$) rằng $j$ là đơn ánh (no. 1, Mệnh đề 2).

Mệnh đề (ii) suy ra từ (i) bằng cách lấy $F = A_s/a$ và (iii) suy ra từ (ii) bằng cách lấy $a = \{0\}$.

Cuối cùng, nếu m là một iđêan trái cực đại của A, thì $\overline{\rho}^{-1}(Bm) = m$ theo (ii), và do đó $Bm \# B$. Khi đó tồn tại một iđêan trái cực đại n của B chứa Bm (Đại số, Chương I, § 8, no. 7, Định lý 2); khi đó $m \subset \overline{\rho}^{-1}(n)$ và vì $\rho(1) \notin n$, $1 \notin \overline{\rho}^{-1}(n)$. Do đó $\overline{\rho}^{-1}(n) = m$.

Nếu $A$ và $B$ thỏa mãn các điều kiện của Mệnh đề 8, thì $A$ thường được đồng nhất với một vành con của $B$ nhờ $\rho$.

#### Hệ quả {#ac-i-s3-n5-cor-1 .statement}

Dưới các giả thiết của Mệnh đề 8, nếu $B$ là Noether trái (resp. Artin), thì $A$ cũng vậy.

Nếu (a) là một dãy tăng (resp. giảm) không dừng của các iđêan trái của $A$, thì dãy $(\mathrm{Ba}_n)$ các iđêan của $B$ cũng không dừng và tăng (resp. giảm), vì $\rho^{-1}(\mathrm{Ba}_n) = a_n$ trái với giả thiết.

*Nhận xét (1). Nếu $A$ và $B$ giao hoán, ta sẽ thấy trong Chương II, § 2, no. 5, Hệ quả 4 của Mệnh đề 11, rằng giả thiết của Mệnh đề 8 suy ra rằng với mọi iđêan nguyên tố $p$ của $A$, tồn tại một iđêan nguyên tố $q$ của $B$ sao cho $\rho^{-1}(q) = p$ (trong đó $p = A \cap q$ khi $A$ được đồng nhất với một vành con của $B$).*

Một áp dụng quan trọng của Mệnh đề 8 là trường hợp $B$ tự nó là một $A$-môđun phẳng trung thành. Nhưng trong trường hợp này ta có mệnh đề chính xác hơn sau:

#### Mệnh đề 9 {#ac-i-s3-prop-9 .statement}

Cho $A, B$ là hai vành và $\rho$ là một đồng cấu từ $A$ đến $B$. Năm điều kiện sau là tương đương:
(a) A-môđun phải $B$ là phẳng trung thành.
(b) Đồng cấu $\rho$ là đơn ánh và A-môđun phải $B/\rho(A)$ là phẳng.
(c) A-môđun phải $B$ là phẳng và, với mọi A-môđun trái $F$, đồng cấu chính tắc $x \mapsto 1 @ x$ từ $F$ vào $B @ * F$ là đơn ánh.
(d) A-môđun phải $B$ là phẳng và, với mọi iđêan trái $a$ của $A$, $\rho^{-1}(\mathrm{Ba}) = a$.
(e) A-môđun phải $B$ là phẳng và, với mọi iđêan trái cực đại $m$ của $A$, tồn tại một iđêan trái cực đại $n$ của $B$ sao cho $\rho^{-1}(n) = m$.

Theo Mệnh đề 8, (a) kéo theo mỗi một trong các tính chất (c), (d), (e). Mặt khác, nếu (e) đúng, thì $Bm \# B$ với mọi iđêan trái cực đại $m$ của $A$ (vì tồn tại một iđêan trái cực đại $n$ của $B$ sao cho $Bm \subset n$), và $B$ là một A-môđun phẳng trung thành theo tiêu chuẩn (d) của Mệnh đề 1 của no. 1; do đó (e) kéo theo (a).

Bây giờ ta chứng minh rằng (c) $\Rightarrow$ (d) $\Rightarrow$ (b) $\Rightarrow$ (a), điều này sẽ hoàn tất chứng minh. Trước hết, (c) kéo theo (d) bằng cách lấy $F = A_s/a$ trong (c). Nếu (d) đúng, bằng cách lấy $a = \{0\}$ suy ra rằng $\rho$ là đơn ánh; (d) và § 2, no. 6, Hệ quả của Mệnh đề 7 suy ra rằng $B/\rho(A)$ là một A-môđun phải phẳng, tức là (d) kéo theo (b). Cuối cùng, nếu (b) đúng, Mệnh đề 3 của no. 1 áp dụng cho dãy khớp

$$
0 \longrightarrow A_a \xrightarrow{\rho} B \longrightarrow B/\rho(A) \longrightarrow 0
$$

cho thấy rằng $B$ là một A-môđun phải phẳng trung thành, vì $A_a$ là phẳng trung thành.

*Nhận xét (2).* Nếu $A$ và $B$ là giao hoán, ta sẽ thấy trong Chương II, § 2 no. 5, Hệ quả 4 của Mệnh đề 11 rằng các điều kiện của Mệnh đề 9 tương đương với điều sau:

(f) B *là một A-môđun phẳng và, với mọi iđêan nguyên tố* $\mathfrak{p}$ *của* $A$, *tồn tại một iđêan* $q$ *của* $B$ *sao cho* $\bar{\rho}^{-1}(q) = \mathfrak{p}$.

Dưới các điều kiện của Mệnh đề 9, ta đồng nhất $A$ với một *vành con* của $B$ bằng $\mathfrak{p}$. Khi đó quan hệ $\bar{\rho}^{-1}(Ba) = a$ viết thành $A \cap Ba = a$. Mặt khác, nếu $F$ là một môđun trái $A$, thì $F$ được đồng nhất với ảnh của nó trong $B \otimes_A F$ qua ánh xạ chính tắc $x \mapsto 1 @ x$; nếu $X$ là một nhóm con cộng tính của $F$, thì ta ký hiệu bởi $BX$ môđun con trái của $B \otimes_A F$ sinh bởi $X$. Với ký hiệu này, ta có:

#### Mệnh đề 10 {#ac-i-s3-prop-10 .statement}

*Cho* $B$ *là một vành và* $A$ *là một vành con của* $B$ *sao cho* $B$ *là một môđun phải phẳng trung thành trên* $A$. *Cho* $F$ *là một môđun trái* $A$, $F', F''$ *là hai môđun con của* $F$. *Khi đó:*
(i) *Ánh xạ chính tắc* $B \otimes_A F' \to B \otimes_A F$ *là một đẳng cấu từ* $B \otimes_A F'$ *lên* $BF'$.
(ii) $F \cap BF' = F'$.
(iii) $B(F' + F'') = BF' + BF''$.
(iv) $B(F' \cap F'') = BF' \cap BF''$.

Vì $B$ là một môđun phải phẳng trên $A$, ánh xạ chính tắc
$$
B \otimes_A F' \to B \otimes_A F
$$
là đơn ánh; xét các sự đồng nhất đã thực hiện, ảnh của nó là $BF'$, điều đó chứng minh (i). Mệnh đề (ii) suy ra từ § 2, no. 6, Mệnh đề 7, áp dụng với $E = B$, $E' = A$, và dùng các công thức $A \otimes_A F = F$ và $A \otimes_A F' = F'$. Mệnh đề (iii) là tầm thường và (iv) suy ra từ § 2, no. 6, Mệnh đề 6.

### 6. CÁC VÀNH PHẲNG TRUNG THÀNH VÀ CÁC ĐIỀU KIỆN HỮU HẠN TÍNH

#### Mệnh đề 11 {#ac-i-s3-prop-11 .statement}

*Cho* $B$ *là một vành và* $A$ *là một vành con của* $B$ *sao cho* $B$ *là một môđun phải phẳng trung thành trên* $A$. *Để một môđun trái* $A$ *là sinh hữu hạn (resp. trình bày hữu hạn), điều kiện cần và đủ là môđun* $B$-*môđun* $B \otimes_A F$ *là sinh hữu hạn (resp. trình bày hữu hạn).*

(1) Không cần giả thiết nào về $B$, hiển nhiên nếu $F$ là một $A$-môđun trái sinh hữu hạn, thì $B \otimes_A F$ là một $B$-môđun trái sinh hữu hạn. Ngược lại, nếu $B \otimes_A F$ là một $B$-môđun sinh hữu hạn, thì nó được sinh bởi một số hữu hạn các phần tử dạng $1 \otimes x_i$ với $x_i \in F$; nếu $M$ là một A-môđun con của $F$ được sinh bởi các $x_i$ và $j$ là đơn ánh chính tắc $M \to F$, $1, \otimes j : B \otimes_A M \to B \otimes_A F$ là một đồng cấu toàn ánh, do đó $j$ là toàn ánh (no. 1, Mệnh đề 2), điều này chứng tỏ rằng $F$ là sinh hữu hạn.

(2) *Nếu* F *có một trình bày hữu hạn, thì* $B \otimes_A F$ *cũng vậy mà không cần giả thiết nào* về B (\S 2, no. 8). Còn phải chứng minh rằng, nếu $B \otimes_A F$ có một trình bày hữu hạn, thì F cũng vậy. Ta đã biết từ (1) rằng F sinh hữu hạn, do đó tồn tại một đồng cấu toàn ánh $u : L \to F$, trong đó L là một A-môđun tự do sinh hữu hạn. Cho R là hạt nhân của u, khi đó $B \otimes_A R$ được đồng nhất với hạt nhân của đồng cấu toàn ánh $l_B \otimes u : B \otimes_A L \to B \otimes_A F$ (\S 2, no. 3, *Nhận xét 2*). Vì $B \otimes_A F$ theo giả thiết có một trình bày hữu hạn, suy ra (\S 2, no. 8, Bổ đề 9) rằng $B \otimes_A R$ sinh hữu hạn; rồi từ (1) suy ra R là một A-môđun sinh hữu hạn và do đó F có một trình bày hữu hạn.

#### Mệnh đề 12 {#ac-i-s3-prop-12 .statement}

*Cho B là một vành và A là một vành con giao hoán của tâm của B sao cho B là một A-môđun phẳng trung thực. Để một A-môđun F là xạ ảnh và sinh hữu hạn, điều kiện cần và đủ là $B \otimes_A F$ là một B-môđun trái xạ ảnh sinh hữu hạn.*

Điều kiện này hiển nhiên là cần mà không cần giả thiết nào về A hoặc B (*Đại số*, Chương II, \S 5, no. 1, Hệ quả của Mệnh đề 4); ta chứng minh rằng nó là đủ. Nếu một môđun xạ ảnh sinh hữu hạn có một trình bày hữu hạn (\S 2, no. 8, Bổ đề 8), thì giả thiết suy ra F có một trình bày hữu hạn nhờ Mệnh đề 11, do đó, với mọi A-môđun M, ta có một đẳng cấu chính tắc

$$
\omega : B \otimes_A \operatorname{Hom}_A(F, M) \to \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M)
$$

(\S 2, no. 10, Mệnh đề 11). Khi đó, cho $v : M \to M''$ là một đồng cấu A-môđun *toàn ánh* và xét biểu đồ giao hoán

$$
\begin{array}{ccc}
B \otimes_A \operatorname{Hom}_A(F, M) & \xrightarrow{\omega} & \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M) \\
1_B \otimes \operatorname{Hom}(1_F, v) \downarrow & & \downarrow \operatorname{Hom}(1_B \otimes F, 1_B \otimes v) \\
B \otimes_A \operatorname{Hom}_A(F, M'') & \xrightarrow{\omega} & \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M'')
\end{array}
$$

Vì $1_B \otimes v$ là toàn ánh và $B \otimes_A F$ được giả sử là xạ ảnh, $\operatorname{Hom}(1_{B \otimes F}, 1_B \otimes v)$ là *toàn ánh* (*Đại số*, Chương II, \S 2, no. 2, Mệnh đề 4) và do đó $1_B \otimes \operatorname{Hom}(1_F, v)$ cũng vậy. Nhưng vì B là một A-môđun phẳng trung thực, $\operatorname{Hom}(1_F, v)$ tự nó là toàn ánh (no. 1, Mệnh đề 2), do đó F là một A-môđun xạ ảnh (*Đại số*, Chương II, \S 2, no. 2, Mệnh đề 4).

### 7. PHƯƠNG TRÌNH TUYẾN TÍNH TRÊN MỘT VÀNH PHẲNG TRUNG THỰC

Cho B là một vành và A là một vành con của B. Ta sẽ nói rằng cặp có thứ tự (A, B) có *tính chất mở rộng tuyến tính* nếu nó thỏa mãn điều kiện sau:

(E) Mọi nghiệm $(y_k)_{1 \leq k \leq n}$, gồm các phần tử của $B$, của một hệ phương trình tuyến tính

$$
\sum_{k=1}^n y_k c_{ki} = d_i \quad (1 \leq i \leq m)
$$

mà các hệ số $c_{ki}$ và các vế phải $d_i$ của nó thuộc $A$, đều có dạng

$$
y_k = x_k + \sum_{j=1}^p b_j z_{jk} \quad (1 \leq k \leq n)
$$

trong đó $(x_k)$ là một nghiệm của (3) gồm các phần tử của $A$, các $b_j$ thuộc $B$ và mỗi $(z_{jk})_{1 \leq k \leq n}$ là một nghiệm của hệ phương trình tuyến tính thuần nhất liên kết với (3), gồm các phần tử của A.

#### Mệnh đề 13 {#ac-i-s3-prop-13 .statement}

Cho A là một vành con của một vành B. Để cặp có thứ tự $(A, B)$ thỏa mãn tính chất mở rộng tuyến tính, điều kiện cần và đủ là B là một A-môđun phẳng trung thực.

Điều kiện này là *đủ*. Thật vậy, vì B là một A-môđun phẳng, mọi nghiệm với các phần tử trong B của hệ phương trình tuyến tính *thuần nhất* liên kết với (3) đều là một tổ hợp tuyến tính với hệ số trong B của các nghiệm gồm các phần tử của A (\S 2, no. 11, Hệ quả 2 của Mệnh đề 13). Bài toán khi đó quy về chứng minh rằng sự tồn tại của một nghiệm của (3) với các phần tử trong B kéo theo sự tồn tại của *một* nghiệm với các phần tử trong A. Bây giờ, nếu ta đặt

$$
c_k = (c_{ki})_{1 \leq i \leq m} \in A_s^m, \qquad d = (d_i) \in A_s^m,
$$

Hệ (3) tương đương với phương trình $\sum_{k=1}^n y_k \otimes c_k = 1 \otimes \mathrm{din}\, B \otimes_A A_s^m = B_s^m$.

Nói cách khác, nếu $M$ là môđun con-$A$ của $A_s^m$ được sinh bởi các $c_k$ $(1 \leq k \leq n)$, thì sự tồn tại của nghiệm $(y_k)$ của (3) tương đương (với các đồng nhất đã thực hiện ở no. 5) với quan hệ $d \in BM \cap A_s^m$; nhưng vì $BM \cap A_s^m = M$ (no. 5, Mệnh đề 10, (ii)), điều đó suy ra $d \in M$, tức là, sự tồn tại của một nghiệm $(x_k)$ của hệ (3) với các phần tử trong $A$.

Điều kiện là cần thiết. Thật vậy, giả sử $(A, B)$ thỏa mãn tính chất mở rộng tuyến tính; ta đã biết rằng $B$ là một A-môđun phải phẳng (\S 2, no. 11, Hệ quả 2 của Mệnh đề 13); ta chứng minh rằng, với mọi iđêan trái $a$ của $A$, $Ba \cap A = a$, điều đó cho thấy rằng $B$ là một A-môđun phải phẳng trung thành (no. 5, Mệnh đề 9, (d)). Bây giờ, lấy $x \in Ba \cap A$; theo giả thiết tồn tại $y_i \in B$ và $a_i \in a$ sao cho $\sum_i y_i a_i = x$; tính chất (E) áp dụng cho phương trình tuyến tính này với các hệ số và vế phải trong $A$ cho thấy rằng tồn tại $x_i \in A$ sao cho $x = \sum_i x_i a_i$, do đó $x \in a$.

### Bài tập {#ac-i-s3-exercises}

Xem [các bài tập cho § 3](exercises/s3/).
