---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 4
section_title: Strict morphisms of Fréchet spaces
lang: vi
source: evt-i-v
book_pages: TVS IV.26-TVS IV.32, TVS IV.62-TVS IV.67
pdf_pages: 0208-0214, 0244-0249
extraction: ocr
subsections:
    - "no": 1
      title: Characterizations of strict morphisms
      page: 27
      pdf_page: 209
    - "no": 2
      title: Strict morphisms of Fréchet spaces
      page: 28
      pdf_page: 210
    - "no": 3
      title: Criteria for surjectivity
      page: 31
      pdf_page: 213
statements: 13
exercises: 23
content_sha256: a3028ae0aab75ee80b041c51eeea5e335259789a3ec59194d01dda918683cce4
translated_from: content/en/evt/IV/04_s4_strict_morphisms_of_frechet_spaces.md
source_content_sha256: 4d9f753ed58d33db4d4b3dea16cf8a66e6a7677f9073f91db993b2b4767b89f4
translation_model: gpt-5-6, gpt-5-6-mini, gpt-5.4
translation_run: translate-vi-8fdd1692
glossary_version: 34
glossary_terms_sha256: dcf42480b4f4ae03b041048ac327a883649f476545919c46882ece0b74f63708
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. CÁC CẤU XẠ NGẶT CỦA CÁC KHÔNG GIAN FRÉCHET

Đối với mọi không gian lồi địa phương E, ký hiệu S(E) là tập hợp tất cả các nửa chuẩn liên tục trên E. Đối với mọi $p \in S(E)$, ký hiệu $H_p$ là tập hợp tất cả các dạng tuyến tính f trên E sao cho $|f| \leqslant p$. Họ $(H_p)_{p \in S(E)}$ là một cơ sở cho bornology gồm các tập con liên tục đều của $E'$.

### 1. Các đặc trưng của các cấu xạ ngặt

#### Mệnh đề 1 {#evt-iv-s4-prop-1 .statement}

Cho E và F là hai không gian lồi địa phương và u là một ánh xạ tuyến tính liên tục từ E vào F. Để u là một cấu xạ ngặt, điều kiện cần và đủ là điều kiện sau được thỏa mãn:

(MS) Đối với mọi nửa chuẩn $p \in S(E)$, triệt tiêu trên hạt nhân của u, tồn tại q trong S(F) sao cho $p \leq q \circ u$.

Gọi N là hạt nhân và M là ảnh của u; ta đưa vào phân tích chính tắc của u, đặt

$$
E \xrightarrow{\pi} E/N \xrightarrow{\tilde{u}} M \xrightarrow{} F .
$$

Các nửa chuẩn liên tục trên E triệt tiêu trên N là các nửa chuẩn $p_1 \circ \pi$ trong đó $p_1$ chạy trên S(E/N); tương tự S(M) gồm các nửa chuẩn $q_1$ sao cho tồn tại $q \in S(F)$ với $q_1 \leq q/F$. Cuối cùng, u là một cấu xạ ngặt khi và chỉ khi ánh xạ tuyến tính liên tục song ánh $\tilde{u}$ có ánh xạ nghịch đảo liên tục; điều này cũng có nghĩa là mọi nửa chuẩn trong S(E/N) đều có dạng $q_1 \circ \tilde{u}$ với $q_1$ trong S(M). Mệnh đề 1 suy ra ngay lập tức từ các nhận xét này.

#### Mệnh đề 2 {#evt-iv-s4-prop-2 .statement}

Cho E và F là hai không gian lồi địa phương Hausdorff và u là một ánh xạ tuyến tính liên tục từ E vào F. Để u là một cấu xạ ngặt, điều kiện cần và đủ là chuyển vị của nó $^t u : F' \to E'$ thỏa mãn các điều kiện sau:

a) Ảnh của $^t u$ là đóng trong $E'$ đối với $\sigma(E', E)$.

b) Mọi tập con đồng liên tục của $E'$, được chứa trong ảnh của $^t u$ đều là ảnh bởi $^t u$ của một tập con đồng liên tục của $F'$.

Nếu đúng như vậy, ta có $\operatorname{Ker} ^t u = (\operatorname{Im} u)^{\circ}$ và $\operatorname{Im} ^t u = (\operatorname{Ker} u)^{\circ}$ và tồn tại các đẳng cấu chính tắc từ Coker $^t u$ lên đối ngẫu của Ker u và từ Ker $^t u$ lên đối ngẫu của Coker u.

Đặt N là hạt nhân và I là ảnh của u. Theo hệ quả 2 của II, p. 47, hạt nhân của $^t u$ là trực giao của I, và bao đóng của ảnh của $^t u$ đối với $\sigma(E', E)$ là trực giao $N^{\circ}$ của N. Phép hội của a) và b) khi đó tương đương với điều kiện sau:

b') Mọi tập con đồng liên tục của $E'$ được chứa trong $N^{\circ}$ đều là ảnh qua $^t u$ của một tập con đồng liên tục của $F'$.

Vì $N^{\circ}$ có thể được đồng nhất với đối ngẫu của E/N, mệnh đề 9, (i) của IV, p. 8, cho thấy rằng các tập con đẳng liên tục của $E'$ được chứa trong $N^{\circ}$ là các tập hợp được chứa trong một tập hợp có dạng $H_p$, trong đó p là một nửa chuẩn liên tục trên E, triệt tiêu trên N. Khi đó điều kiện b') nói rằng, với mọi nửa chuẩn $p \in S(E)$ bằng không trên N, tồn tại $q \in S(F)$ sao cho $H_p \subset ^t u(H_q)$. Theo định lý Hahn-Banach (II, p. 23, hệ quả 1 và 2, p. 63, định lý 1 và hệ quả 1), ta có $^t u(H_q) = H_{q \circ u}$, và các quan hệ $H_p \subset H_{p'}$ và $p \leq p'$ là tương đương đối với mọi nửa chuẩn $p$ và $p'$ trong S(E). Do đó, quan hệ $H_p \subset ^t u(H_q)$ là tương đương với quan hệ $p \leq q \circ u$. Theo mệnh đề 1, tính chất b') suy ra rằng u là một cấu xạ ngặt.

Giả sử u là một cấu xạ ngặt. Ta đã thấy rằng hạt nhân của $^t u$ là phần trực giao của I và ảnh của $^t u$ là phần trực giao của N. Đối hạt nhân của $u$ là không gian $F/I$ và đối ngẫu của nó có thể được đồng nhất với $I^\circ = \mathrm{Ker}\ ^t u$. Tương tự, đối ngẫu của $N = \mathrm{Ker}\ u$ có thể được đồng nhất với $E'/N^\circ$ (IV, p. 8), *tức là* với đối hạt nhân của $^t u$ vì $N^\circ$ là ảnh của $^t u$.

#### Nhận xét {#evt-iv-s4-n1-rem-1 .statement}

— Với các ký hiệu của mệnh đề 2, tính chất $b'$) cũng suy ra rằng $u$ là một cấu xạ ngặt đối với các tôpô đã làm yếu đi (II, p. 49, hệ quả 3).

#### Mệnh đề 3 {#evt-iv-s4-prop-3 .statement}

*Cho E và F là hai không gian lồi địa phương, và u là một ánh xạ tuyến tính liên tục từ E vào F. Giả sử rằng E là Hausdorff và F có thể mêtric hóa được. Để u là một cấu xạ ngặt, điều kiện cần và đủ là ảnh của $^t u$ đóng trong $E'$ đối với tôpô yếu $\sigma(E', E)$.*

Tính cần thiết suy ra từ mệnh đề 2.

Ngược lại, giả sử rằng ảnh của $^t u$ là đóng đối với $\sigma(E', E)$ và đưa vào phân tích chính tắc của $u$ như trong chứng minh của mệnh đề 1. Theo các nhận xét trên, ánh xạ nghịch đảo $\tilde{u}^{-1}$ của $\tilde{u}$ là liên tục đối với các tôpô làm yếu. Nhưng không gian con $M = u(E)$ của F là mêtric hóa được, nên là sinh bị chặn (III, p. 12, mệnh đề 2); do đó (IV, p. 7, mệnh đề 7, (ii)), $\tilde{u}^{-1}$ là liên tục, vì thế $u$ là một cấu xạ ngặt.

### 2. Các cấu xạ ngặt của các không gian Fréchet

#### Định lý 1 {#evt-iv-s4-thm-1 .statement}

*Cho E và F là hai không gian Fréchet và u là một ánh xạ tuyến tính liên tục từ E vào F. Các điều kiện sau là tương đương :

a) $u$ là một cấu xạ ngặt.
b) $u$ là một cấu xạ ngặt đối với các tôpô yếu hơn.
c) Ảnh của $u$ đóng trong F.
d) $^t u$ là một cấu xạ ngặt từ $F'$ vào $E'$ đối với các tôpô yếu.
e) Ảnh của $^t u$ đóng trong $E'$ đối với tôpô yếu $\sigma(E', E)$.
f) Ảnh của $^t u$ đóng trong $E'$ đối với tôpô mạnh $\beta(E', E)$.
g) $^t u$ là một cấu xạ ngặt từ $F'_c$ vào $E'_c$ (các đối ngẫu được trang bị tôpô hội tụ compact).

Sự tương đương của a), b) và e) suy ra từ mệnh đề 3 của IV, p. 28 và nhận xét đứng trước nó. Sự tương đương của a) và c) chính xác là hệ quả 3 của I, p. 19. Nhận xét của IV, p. 28, cũng cho thấy rằng d) tương đương với việc ảnh của $u$ là đóng đối với tôpô yếu đi $\sigma(F, F')$ của F; khi đó sự tương đương của c) và d) suy ra từ mệnh đề 2 của IV, p. 4.

Bây giờ ta chứng minh tính tương đương của e) và f). Chỉ cần chứng minh rằng f) kéo theo e). Giả sử rằng ảnh của $^t u$ là đóng đối với $\beta(E', E)$ trong $E'$. Chiếu theo định lý Banach-Dieudonné (IV, p. 25, hệ quả 2), chỉ cần chứng minh rằng với mọi lân cận lồi cân bằng U của 0 trong E, giao $B = ^t u(F') \cap U$ là compắc đối với $\sigma(E', E)$. Đối ngẫu mạnh $E'_b$ của không gian Fréchet E là đầy đủ (IV, p. 22, mệnh đề 2), do đó tập con đóng B của $E'_b$ là đầy đủ, và vì thế không gian định chuẩn $E'_B$ là đầy đủ (III, p. 8, hệ quả). Gọi $(V_n)$ là một dãy giảm tạo thành một hệ cơ bản các lân cận của 0 trong F. Khi đó $F'$ là hợp của các tập $C = V_n^\circ$ compắc đối với $\sigma(F', F)$, do đó $E'_B = \bigcup_n B_n$, với $B_n = E'_B \cap ^t u(C_n)$. Vì $E'_B$ là một không gian Baire, và mỗi tập $B_n$ đều lồi, cân bằng và đóng, tồn tại một số thực $r > 0$ và một số nguyên $n$ sao cho $B \subset r.B_n$. Khi đó ta có $B = U^\circ \cap {}^t u(r.C_n)$; vì các tập $U^\circ$ và $r.C_n$ là compắc và ${}^t u$ liên tục đối với các tôpô yếu, nên $B$ compắc đối với $\sigma(E', E)$. Điều này hoàn tất chứng minh tính tương đương của e) và f).

Sau cùng sự tương đương của g) với các điều kiện trước đó suy ra từ mệnh đề 18 của GT, X, § 2, No. 10 và bổ đề sau đây.

#### Bổ đề 1 {#evt-iv-s4-lem-1 .statement}

*Cho E và F là hai không gian Hausdorff lồi địa phương và đầy đủ giả, và u là một ánh xạ tuyến tính liên tục từ E vào F. Để ${}^t u$ là một cấu xạ ngặt từ $F'_c$ vào $E'_c$, điều kiện cần và đủ là ảnh $u(E)$ của u đóng, và mọi tập con compact của $u(E)$ đều là ảnh qua u của một tập con compact của E.*

Theo định lý của Mackey (IV, p. 2, th. 1) và sự kiện là trên $E'$ (resp. F) tôpô của sự hội tụ compact trùng với tôpô của sự hội tụ compact lồi (IV, p. 4), ta có thể đồng nhất E (resp. F) với đối ngẫu $E'_c$ (resp. $F'_c$). Khi đó $u$ là chuyển vị của ${}^t u$, và các tập con đồng liên tục của E (resp. F) là các tập tương đối compact. Bổ đề 1 khi ấy suy ra từ mệnh đề 2 (IV, p. 27), vì $u(E)$ đóng trong F khi và chỉ khi nó đóng đối với tôpô yếu đi $\sigma(F, F')$ (IV, p. 4, mệnh đề 2).

#### Hệ quả 1 {#evt-iv-s4-lem-1-cor-1 .statement}

*Dưới giả thiết của định lý 1, các điều kiện sau là tương đương :*
(i) *u là một cấu xạ đơn ánh ngặt ;*
(ii) *${}^t u$ là một cấu xạ toàn ánh ngặt đối với các tôpô yếu.*
(iii) *${}^t u$ là toàn ánh.*

Hàm ý (i) $\Rightarrow$ (ii) suy ra ngay lập tức từ sự tương đương của các điều kiện a), d) và e) của đl. 1 và từ IV, p. 6, mđ. 5. Rõ ràng là (ii) kéo theo (iii). Sau cùng, ta chứng minh rằng (iii) kéo theo (i) : nếu ${}^t u$ là toàn ánh thì $u$ là một cấu xạ ngặt theo sự tương đương của a) và e) trong đl. 1 ; việc $u$ là đơn ánh suy ra từ mđ. 5 của IV, p. 6.

#### Hệ quả 2 {#evt-iv-s4-lem-1-cor-2 .statement}

*Dưới giả thiết của đl. 1, các điều kiện sau là tương đương :*
(i) *u là toàn ánh ;*
(ii) *u là một cấu xạ toàn ánh ngặt ;*
(iii) *${}^t u$ là một cấu xạ đơn ánh ngặt đối với các tôpô yếu.*

Sự tương đương của (i) và (ii) suy ra từ đl. của Banach (I, p. 17, đl. 1).

Do sự tương đương của a) và c) trong định lý 1, điều kiện (ii) nói rằng $u$ là một cấu xạ ngặt và ảnh của nó trù mật trong F đối với $\sigma(F, F')$. Khi đó sự tương đương của (ii) và (iii) suy ra từ sự tương đương của a) và d) trong định lý 1 và từ mệnh đề 5 của IV, p. 6.

Nếu $u : E \to F$ là một cấu xạ ngặt của các không gian Fréchet, cấu xạ chuyển vị ${}^t u$ không nhất thiết là một cấu xạ ngặt từ $F'_b$ vào $E'_b$ (IV, p. 62, bài tập 3). Tuy nhiên, ta có kết quả bộ phận sau :

#### Hệ quả 3 {#evt-iv-s4-lem-1-cor-3 .statement}

— Dưới các giả thiết của đl. 1, tính chất sau kéo theo các tính chất a) đến g) :
h) $^t u$ là một cấu xạ ngặt từ $F'_b$ vào $E'_b$.
Khi E và F đều là các không gian Banach, hoặc đều là các không gian Montel, tính chất h) tương đương với các tính chất a) đến g) của đl. 1.
Giả sử rằng $^t u$ là một cấu xạ ngặt từ $F'_b$ vào $E'_b$. Ta sẽ chứng minh rằng ảnh H của $^t u$ là đóng trong $E'_b$, từ đó sẽ suy ra mệnh đề thứ nhất của hq. 3.
Gọi G là bao đóng của ảnh của $u$ trong F ; không gian G, được trang bị tôpô cảm sinh bởi tôpô của F, là một không gian Fréchet. Ánh xạ $u : E \to F$ phân tích thành $u = j \circ v$ trong đó j là đơn ánh chính tắc từ G vào F và $v \in \mathcal{L}(E; G)$. Khi đó ta có $^t u = ^t v \circ ^t j$, trong đó $^t j$ là toàn ánh, theo đl. Hahn-Banach (II, p. 24, mệnh đề 2); đồng thời $^t v$ là đơn ánh vì $v(E)$ trù mật trong G (IV, p. 6, mệnh đề 5). Theo giả thiết, ánh xạ $^t u$ từ $F'_b$ lên H là mở ; vì $^t j$ là toàn ánh và liên tục, ánh xạ $^t v$ cảm sinh một đồng phôi từ $G'_b$ lên H. Nhưng đối ngẫu $G'_b$ của không gian Fréchet G là đầy đủ (IV, p. 22, mệnh đề 2); do đó H là đầy đủ, vì thế đóng trong $E'_b$.
Nếu E và F là các không gian Montel, tôpô mạnh trên $E'$ (resp. $F'$) trùng với tôpô hội tụ compact, và h) chỉ là một sự phát biểu lại của g).
Nếu E và F là các không gian Banach, thì $E'_b$ và $F'_b$ cũng vậy, và điều kiện h) tương đương với f) bởi tính tương đương của a) và c) áp dụng cho $^t u : F'_b \to E'_b$.

#### Hệ quả 4 {#evt-iv-s4-lem-1-cor-4 .statement}

— Giả sử E và F là các không gian Banach. Để $^t u$ là toàn ánh, điều kiện cần và đủ là tồn tại một số thực $r > 0$ sao cho $\| x \| \leq r. \| u(x) \|$ với mọi $x \in E$.
Đây chỉ đơn giản là một sự phát biểu lại của tính tương đương giữa các điều kiện (i) và (iii) của hệ quả 1.

#### Hệ quả 5 {#evt-iv-s4-lem-1-cor-5 .statement}

- Cho E và F là hai không gian Fréchet và u là một ánh xạ tuyến tính liên tục từ E vào F. Các điều kiện sau là tương đương :
a) u là một đẳng cấu từ E lên F.
b) u là một đẳng cấu từ E lên F đối với các tôpô làm yếu.
c) $^t u$ là một đẳng cấu từ $F'$ lên $E'$ đối với các tôpô yếu.
d) $^t u$ là một đẳng cấu từ $F'$ lên $E'$ đối với các tôpô mạnh.
e) $^t u$ là một đẳng cấu từ $F'_c$ lên $E'_c$.
Vì một đẳng cấu không là gì khác ngoài một cấu xạ ngặt song ánh, nên tính tương đương của a) và b) suy ra từ tính tương đương của các điều kiện a) và b) của định lý 1.
Hiển nhiên a) kéo theo mỗi điều kiện c), d) và e).
Ngược lại, giả sử một trong các điều kiện c), d) hoặc e) được thỏa mãn. Từ định lý 1 và hệ quả 3 của nó suy ra rằng u là một cấu xạ ngặt từ E vào F, và hiển nhiên $^t u$ là song ánh. Đặt N (tương ứng I) là hạt nhân (tương ứng ảnh) của u. Vì $^t u$ là song ánh, ta có $\operatorname{Im} ^t u = E'$ và $\operatorname{Ker} ^t u = \{ 0 \}$, và do đó $N^\circ = E'$ và $I^\circ = \{ 0 \}$ theo mệnh đề 2 của IV, p. 27. Nhưng N (tương ứng I) là một không gian con vectơ đóng của E (tương ứng F), và định lý lưỡng cực (II, p. 44) suy ra rằng $N = \{ 0 \}$ và $I = F$, do đó u là song ánh. Vậy ta đã chứng minh rằng u là một đẳng cấu.

### 3. Các tiêu chuẩn cho tính toàn ánh

#### Mệnh đề 4 {#evt-iv-s4-prop-4 .statement}

— Cho E và F là hai không gian Fréchet, và u là một ánh xạ tuyến tính liên tục từ E vào F. Các điều kiện sau là tương đương :

(i) u là toàn ánh.

(ii) Với mọi nửa chuẩn $p \in S(E)$, tồn tại $q \in S(F)$ sao cho ta có $|f| \leq q$ với mọi dạng tuyến tính $f \in F'$ thỏa mãn $|f \circ u| \leq p$.

(iii) Với mọi nửa chuẩn $p \in S(E)$, tồn tại $q \in S(F)$ thỏa mãn tính chất sau : nếu một dạng tuyến tính $f \in F'$ thỏa mãn $|f \circ u| \leq p$, thì $f$ triệt tiêu trên các điểm tại đó $q$ triệt tiêu và với mọi $y \in F$, $r \in S(F)$, tồn tại $x \in E$ sao cho $r(u(x) - y) = 0$.

(iv) Với mọi nửa chuẩn $p \in S(E)$, ta có

$$
\sup_{\substack{f \in F \\ |f \circ u| \leq p}} |f(y)| < +\infty \quad \text{với mọi} \quad y \in F .
$$

Chúng ta sẽ chứng minh mệnh đề theo lược đồ lôgic sau

![Biểu đồ biểu thị các quan hệ lôgic giữa (i), (ii), (iii), và (iv)](https://i.imgur.com/3Q5z5QG.png)

Nếu $u$ là toàn ánh, thì nó là một cấu xạ ngặt (IV, p. 28, đl. 1); khi đó với mọi nửa chuẩn $p \in S(E)$, tồn tại một nửa chuẩn $q \in S(F)$ sao cho, với mọi $y \in F$ thỏa mãn $q(y) \leq 1$, tồn tại $x \in E$ thỏa mãn $p(x) \leq 1$ và $u(x) = y$. Từ đó suy ra ngay lập tức rằng (i) kéo theo (ii) và (iii). Rõ ràng là (ii) kéo theo (iv).

Để chứng minh rằng (iii) kéo theo (iv), lấy $p$ và $q$ như trong (iii). Cho $y \in F$, theo (iii), tồn tại $x$ trong $E$ sao cho $q(u(x) - y) = 0$. Nếu $f \in F'$ thỏa mãn $|f \circ u| \leq p$, thì ta có $f(u(x) - y) = 0$, do đó

$$
|f(y)| = |f(u(x))| \leq p(x)
$$

và quan hệ (1) được thỏa mãn.

Cuối cùng ta chứng minh rằng (iv) kéo theo (i). Cho $p \in S(E)$ và cho $q$ là bao trên của các hàm $|f|$ với $f \in F'$ thỏa mãn $|f \circ u| \leq p$. Theo (iv), $q$ là hữu hạn trên $F$, và hiển nhiên là một nửa chuẩn nửa liên tục dưới trên $F$; vì $F$ là barrelled (III, p. 25, hệ quả), ta có $q \in S(F)$. Ký hiệu $B_p$ (tương ứng $B_q$) là tập hợp mọi $x \in E$ (tương ứng mọi $y \in F$) sao cho $p(x) \leq 1$ (tương ứng $q(y) \leq 1$). Ta có $q \circ u \leq p$, do đó $u(B_p) \subset B_q$. Cực của $u(B_p)$ trong $F'$ gồm các dạng tuyến tính $f \in F'$ sao cho $|f \circ u| \leq p$, nên $|f| \leq q$; nói cách khác, ta được $u(B_p)^{\circ} \subset B_q^{\circ}$, và sau cùng suy ra $\overline{u(B_p)} = B_q$ theo định lý song cực (II, p. 45, cor. 3). Nếu $U$ là một lân cận của 0 trong $E$, thì tồn tại $p \in S(E)$ sao cho $B_p \subset U$, do đó $\overline{u(U)}$ chứa lân cận $B_q$ của 0 trong $F$. Điều này suy ra rằng $u$ là toàn ánh (I, p. 17, th. 1).

#### Hệ quả {#evt-iv-s4-n3-cor-1 .statement}

— Giả sử E và F là các không gian Banach. Các điều kiện sau là tương đương :
(i) u là toàn ánh.
(ii) Tồn tại một số thực r > 0 sao cho $\|f\| \leq r.\|^{t}u(f)\|$ với mọi $f \in F'$.
(iii) Với mọi $y \in F$, ta có $\sup_{\substack{f \in F' \\ \|f \circ u\| \leq 1}} |f(y)| < + \infty$.

Các điều kiện (ii) và (iii) thực ra là những cách phát biểu lại của các điều kiện (ii) và (iv) của mệnh đề 4 đối với các không gian Banach.

### Bài tập {#evt-iv-s4-exercises}

Xem [các bài tập của § 4](exercises/s4/).
