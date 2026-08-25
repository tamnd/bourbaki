---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 11
section_title: Abelian extensions
lang: vi
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.160-A V.166
pdf_pages: 0191-0207, 0274-0280
extraction: ocr
subsections:
    - "no": 1
      title: Abelian extensions and the abelian closure
      page: 77
      pdf_page: 191
    - "no": 2
      title: Roots of unity
      page: 78
      pdf_page: 192
    - "no": 3
      title: Primitive roots of unity
      page: 79
      pdf_page: 193
    - "no": 4
      title: Cyclotomic extensions
      page: 81
      pdf_page: 195
    - "no": 5
      title: Irreducibility of cyclotomic polynomials
      page: 83
      pdf_page: 197
    - "no": 6
      title: Cyclic extensions
      page: 85
      pdf_page: 199
    - "no": 7
      title: Duality of $\mathbf{Z}/n\mathbf{Z}$-modules
      page: 86
      pdf_page: 200
    - "no": 8
      title: Kummer theory
      page: 88
      pdf_page: 202
    - "no": 9
      title: Artin-Schreier theory
      page: 91
      pdf_page: 205
statements: 45
exercises: 23
content_sha256: 29a0968782cbcb815a88411147bbdb80bdc9e7ef3705e12ddc9e56ab1bdd9250
translated_from: content/en/alg/V/11_s11_abelian_extensions.md
source_content_sha256: 6948c79032d0ed93f4abaa213981181a5d1932d82792a48541b5e6e181c59fa4
translation_model: gpt-5.4-mini
translation_run: translate-vi-37cd9a2a
glossary_version: 34
glossary_terms_sha256: d56dffab09431ad0441361700d79bfd903754e3f0f5930f89920aad880e6b9fa
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 11. CÁC MỞ RỘNG ABEL

Trong toàn bộ đoạn này, K ký hiệu một trường.

### 1. Các mở rộng Abel và bao đóng Abel

#### Định nghĩa 1 {#alg-v-s11-def-1 .statement}

— Một mở rộng E của K được gọi là Abel nếu nó là Galois và nhóm Galois của nó là giao hoán.

Vì mọi nhóm con của một nhóm giao hoán đều chuẩn tắc, Hệ quả 4 của V, p. 68 cho thấy mọi mở rộng con của một mở rộng Abel đều là Abel.

#### Mệnh đề 1 {#alg-v-s11-prop-1 .statement}

— Cho E là một mở rộng Galois của K và Γ là nhóm Galois của nó. Cho A là nhóm dẫn xuất của Γ (I, p. 10, Định nghĩa 4) và F là trường bất biến của A. Để một mở rộng con L của E là Abel thì điều kiện cần và đủ là L phải được chứa trong F.

Trước hết ta nhận thấy rằng F cũng là trường bất biến của bao đóng $\bar{\Delta}$ của A trong Γ, và rằng $\bar{\Delta}$ là một nhóm con chuẩn tắc đóng của Γ. Theo V, p. 68, Hệ quả 4, do đó F là một mở rộng Galois của K. Hơn nữa, nhóm Galois của F trên K đẳng cấu với $\Gamma / \bar{\Delta}$ và vì vậy là giao hoán. Suy ra mọi mở rộng con của F đều là Abel. Ngược lại, cho L là một mở rộng Abel của K nằm trong E, và cho Π là nhóm Galois của E trên L. Vì L là Galois, Π là một nhóm con chuẩn tắc của Γ và nhóm Galois của L trên K đẳng cấu với $\Gamma / \Pi$ (V, p. 68, Hệ quả 4). Do đó $\Gamma / \Pi$ là giao hoán và Π chứa A, suy ra $L \subset F$.

#### Hệ quả {#alg-v-s11-n1-cor-1 .statement}

— Cho E là một mở rộng của K và cho $(E_i)_{i \in I}$ là một họ các mở rộng con của E sao cho $E = K \left( \bigcup_{i \in I} E_i \right)$. Giả sử rằng mỗi mở rộng $E_i$ đều Abel, thì E cũng vậy.

Trước hết E là một mở rộng Galois của K (V, p. 57, Mệnh đề 1). Nếu trường F được định nghĩa như trong Mệnh đề 1, thì ta có $E_i \subset F$ với mọi $i \in I$, suy ra $E = F$.

Một mở rộng E của K được gọi là bao đóng Abel của K nếu nó là một mở rộng Abel của K và mọi mở rộng Abel của K đều đẳng cấu với một mở rộng con của E. Mệnh đề 1 kéo theo sự tồn tại của một bao đóng Abel của K: thật vậy, cho $K_s$ là một bao đóng tách được của K, với nhóm Galois $\Gamma$ và cho $(\overline{\Gamma}, \overline{\Gamma})$ là bao đóng của nhóm dẫn xuất của $\Gamma$; ký hiệu $K_{ab}$ là trường bất biến của $(\overline{\Gamma}, \overline{\Gamma})$; vì mọi mở rộng đại số tách được của K đều đẳng cấu với một mở rộng con của $K_s$ (V, p. 45, Hệ quả). Mệnh đề 1 cho thấy $K_{ab}$ là một bao đóng Abel của K. Nhóm Galois của $K_{ab}$ trên K đẳng cấu chính tắc với $\Gamma / (\overline{\Gamma}, \overline{\Gamma})$. Bây giờ ta hãy chứng minh tính duy nhất của các bao đóng Abel: cho E, E' là hai bao đóng Abel của K; theo định nghĩa tồn tại các đồng cấu K $u : E \to E'$ và $v : E' \to E$ và Mệnh đề 1 (V, p. 52) suy ra rằng $v(u(E)) = E$ và $u(v(E')) = E'$, do đó $u$ là một đẳng cấu K của E lên E'. Mọi đẳng cấu K khác của E lên E' đều có dạng $u_1 = \sigma_0 \circ u$ với $\sigma_0 \in \mathrm{Gal}(E'/K)$; vì $\mathrm{Gal}(E'/K)$ là giao hoán, đẳng cấu $\sigma \mapsto u \circ \sigma \circ u^{-1}$ của $\mathrm{Gal}(E/K)$ lên $\mathrm{Gal}(E'/K)$ không phụ thuộc vào $u$; nó được gọi là đẳng cấu chính tắc của $\mathrm{Gal}(E/K)$ lên $\mathrm{Gal}(E'/K)$.

### 2. Các căn của đơn vị

#### Định nghĩa 2 {#alg-v-s11-def-2 .statement}

*Một phần tử $\zeta$ của K được gọi là một căn của đơn vị nếu tồn tại một số nguyên $n > 0$ sao cho $\zeta^n = 1$; với mọi số nguyên $n > 0$ sao cho $\zeta^n = 1$, $\zeta$ được gọi là căn bậc n của đơn vị.*

Tương đương với việc nói rằng các căn của đơn vị là các phần tử có cấp hữu hạn của nhóm nhân $K^*$ gồm các phần tử khác không của K (I, p. 51). Các căn của đơn vị tạo thành một nhóm con $\mu_\infty(K)$ của $K^*$, các căn bậc n tạo thành một nhóm con $\mu_n(K)$ của $\mu_\infty(K)$. Ta có $\mu_\infty(K) = \bigcup_{n \geq 1} \mu_n(K)$ và $\mu_n(K) \subset \mu_m(K)$ nếu $n$ chia hết $m$. Với mỗi căn của đơn vị $\zeta$ tồn tại một số nguyên nhỏ nhất $n \geq 1$ sao cho $\zeta$ thuộc $\mu_n(K)$, đó chính là cấp của $\zeta$ trong nhóm $K^*$.

#### Định lý 1 {#alg-v-s11-thm-1 .statement}

*Cho $p$ là số mũ đặc số của K và cho $n > 0$ là một số nguyên. Khi đó nhóm $\mu_n(K)$ các căn bậc n của đơn vị trong K là tuần hoàn và cấp của nó chia hết cho $n$; khi K là trường đóng đại số và $n$ nguyên tố cùng nhau với $p$, thì nhóm $\mu_n(K)$ là tuần hoàn cấp $n$.*

Đủ để chứng minh mệnh đề thứ nhất của định lý, điều này là hệ quả của bổ đề chính xác hơn sau đây:

#### Bổ đề 1 {#alg-v-s11-lem-1 .statement}

*Cho G là một nhóm con hữu hạn của $K^*$ có cấp $m$; khi đó G là tuần hoàn và ta có $G = \mu_m(K)$. \*

Xét G như một Z-môđun; ta có $mx = 0$ với mọi $x \in G$, do đó linh hóa tử của G là một iđêan có dạng $r\mathbf{Z}$, trong đó số nguyên $r \geq 1$ chia hết cho $m$. Vì vậy ta có $G \subset \mu_r(K)$. Theo Bổ đề 4 (V, p. 74) áp dụng với $A = \mathbf{Z}$ và $M = G$ tồn tại một phần tử $x$ của G có cấp $r$; gọi $G'$ là nhóm con tuần hoàn của G được sinh bởi $x$. Ta có $G' \subset \mu_r(K)$, Card $(G') = r$ và Card $\mu_r(K) \leq r$; do đó ta có

G' = μ_r(K) ⊃ G và G là tuần hoàn cấp r, suy ra bằng μ_r(K). Vì G có cấp m, ta có m = r và bổ đề được suy ra.

#### Mệnh đề 2 {#alg-v-s11-prop-2 .statement}

— Cho K là trường đóng đại số và cho p là số mũ đặc số của nó. Có một đẳng cấu của μ_∞(K) lên nhóm Q/Z[1/p].

Ta đã ký hiệu Z[1/p] là vành con của Q được sinh bởi 1/p, tức là tập các số hữu tỉ có dạng a/p^n với a ∈ Z và n ≥ 1; do đó ta có Z[1/p] = Z nếu K có đặc số 0.

Cho (v_n), là dãy tăng ngặt gồm tất cả các số nguyên không chia hết cho p, nếu p ≠ 1; đặt X = v_1 v_2 ... v_n và ký hiệu H_n là nhóm các căn bậc λ_n của đơn vị; ta có H_{n+1} ⊃ H_n và μ_∞(K) = U H_n. Vì H_n là tuần hoàn cấp X, (Th. 1), tồn tại một dãy (a_n), các căn của đơn vị sao cho a_n sinh H_n và a_n = α_n^{v_n + 1}.

Tiếp theo, gọi β_n là lớp thặng dư modulo Z[1/p] của 1/λ_n và gọi H'_n là nhóm con tuần hoàn của Q/Z[1/p] được sinh bởi β_n. Hiển nhiên ta có β_n = v_{n+1} β_{n+1} và H'_n có cấp λ_n vì X không chia hết cho p nếu p ≠ 1. Vì vậy với mọi n ≥ 1 tồn tại một đẳng cấu φ_n : H_n → H'_n sao cho φ_n(α_n) = β_n và các quan hệ α_n = α_{n+1}^{v_n + 1}, β_n = v_{n+1} β_{n+1}, cho thấy φ_n+, kéo dài φ_n. Cuối cùng tồn tại một đẳng cấu duy nhất φ của μ_∞(K) lên Q/Z[1/p] kéo dài các đẳng cấu φ_n, tức là, φ(α_n) = β_n với mọi n ≥ 1.

#### Nhận xét 1 {#alg-v-s11-n2-rem-1 .statement}

Khi K là một trường đóng đại số có đặc số 0, thì nhóm μ_∞(K) do đó đẳng cấu (không một cách chính tắc) với Q/Z. *Khi K là trường C của các số phức, ta có thể viết ra một đẳng cấu như vậy một cách tường minh: thực ra ánh xạ x ↦ e^{2πix} là một đồng cấu của Q vào C* với hạt nhân Z và ảnh μ_∞(C); do đó qua phép chuyển sang thương nó xác định một đẳng cấu của Q/Z lên μ_∞(C).*

#### Nhận xét 2 {#alg-v-s11-n2-rem-2 .statement}

Kết quả sau đây có thể được chứng minh (cf. V, p. 165, Ex. 21): cho G và H là hai nhóm giao hoán mà mọi phần tử đều có cấp hữu hạn. Giả sử rằng với mọi số nguyên n ≥ 1, phương trình nx = 0 có cùng số nghiệm, được giả thiết là hữu hạn trong G và trong H. Khi đó các nhóm G và H là đẳng cấu. Điều này cho một chứng minh mới của Mđ. 2.

#### Nhận xét 3 {#alg-v-s11-n2-rem-3 .statement}

Với mỗi số nguyên tố l đặt μ_{l∞}(K) = U μ_{ln}(K). Khi l là đặc số p của K, ta có μ_{p∞}(K) = {1}. Từ I, p. 80, Th. 4, suy ra rằng μ_∞(K) là một tổng trực tiếp của các nhóm con μ_{l∞}(K), trong đó l chạy qua tập tất cả các số nguyên tố khác với p. Với một số nguyên tố l cho trước chỉ có hai trường hợp có thể xảy ra: hoặc μ_{l∞}(K) là hữu hạn và khi đó μ_{l∞}(K) đẳng cấu với Z/l^nZ cho một n thích hợp (Th. 1), hoặc μ_{l∞}(K) là vô hạn và khi đó μ_{l∞}(K) đẳng cấu với Z[l^{-1}]/Z (cf. Nhận xét 2).

### 3. Các căn nguyên thủy của đơn vị

Cho n ≥ 1 là một số nguyên. Theo chỉ thị Euler của n, ký hiệu φ(n), ta hiểu số phần tử khả nghịch của vành Z/nZ các số nguyên modulo n. Theo mệnh đề sau, $\varphi(n)$ cũng là số các số nguyên $k$ nguyên tố cùng nhau với $n$ và sao cho $0 \leq k < n$.

#### Mệnh đề 3 {#alg-v-s11-prop-3 .statement}

*Cho $k$ và $n \geq 1$ là hai số nguyên. Khi đó các mệnh đề sau là tương đương*:

a) *lớp thặng dư của $k$ modulo $n$ là khả nghịch trong vành $\mathbf{Z}/n\mathbf{Z}$;*
b) *lớp thặng dư của $k$ modulo $n$ sinh ra nhóm tuần hoàn $\mathbf{Z}/n\mathbf{Z}$;*
c) *các số nguyên $k$ và $n$ nguyên tố cùng nhau* (*I*, p. 112).

Mỗi điều kiện a) và b) có nghĩa là tồn tại số nguyên $x$ sao cho $kx \equiv 1 \pmod{n}$, tức là tồn tại hai số nguyên $x$ và $y$ sao cho $kx + ny = 1$. Điều kiện sau cùng này chỉ có nghĩa là $k$ và $n$ nguyên tố cùng nhau.

#### Hệ quả 1 {#alg-v-s11-prop-3-cor-1 .statement}

*Cho $G$ là một nhóm tuần hoàn cấp $n$ và cho $d$ là một ước của $n$. Khi đó số phần tử có cấp $d$ trong $G$ bằng $\varphi(d)$. Đặc biệt, $\varphi(n)$ là số phần tử sinh của $G$.*

Vì $G$ đẳng cấu với $\mathbf{Z}/n\mathbf{Z}$, nên số phần tử sinh của $G$ bằng $\varphi(n)$ theo Mệnh đề 3. Cho $g$ là một phần tử sinh của $G$; khi đó các phần tử $h$ của $G$ thỏa $h^d = 1$ tạo thành nhóm con $H$ của $G$ sinh bởi $g^{n/d}$; nhóm này là nhóm tuần hoàn cấp $d$ và các phần tử có cấp $d$ của $G$ là các phần tử sinh của $H$, do đó số lượng của chúng là $\varphi(d)$.

#### Hệ quả 2 {#alg-v-s11-prop-3-cor-2 .statement}

*Với mọi số nguyên $n \geq 1$, ta có*
$$
\sum_{d \mid n} \varphi(d) = n,
$$
*trong đó số nguyên $d$ chạy qua tập các ước > 0 của $n$* ^1.

Theo ký hiệu của Hệ quả 1, mỗi phần tử của $G$ đều có một cấp hữu hạn là một ước $d$ của $n$, và với một $d$ cố định thì có $\varphi(d)$ phần tử như thế.

Việc tính $\varphi(n)$ dựa trên hai công thức:

(2) $\varphi(mn) = \varphi(m)\varphi(n)$ nếu $m$ và $n$ là nguyên tố cùng nhau ,
(3) $\varphi(p^a) = p^{a-1}(p-1)$ ($p$ nguyên tố, $a \geq 1$).

Điều đầu tiên suy ra ngay từ तथ्य là các vành $\mathbf{Z}/mn\mathbf{Z}$ và $(\mathbf{Z}/m\mathbf{Z}) \times (\mathbf{Z}/n\mathbf{Z})$ đẳng cấu (*I*, p. 112), và rằng $(A \times B)^* = A^* \times B^*$ đối với hai vành $A$ và $B$. Để chứng minh (3) ta nhận xét rằng các ước dương của $p^a$ là $1, p, p^2, \ldots, p^a$; do đó số nguyên $k$ không có ước chung nào với $p^a$ ngoài $1$ khi và chỉ khi nó không chia hết cho $p$; vì có $p^a - 1$ bội của $p$ giữa $0$ và $p^a - 1$, ta quả thực được (3).

Các công thức (2) và (3) cho ngay rằng
$$
\varphi(n) = n \prod_p (1 - 1/p),
$$
trong đó $p$ chạy qua tập hợp các ước nguyên tố của $n$.

^1 Quan hệ $d \mid n$ giữa các số nguyên > 0 có nghĩa là « d chia hết n » (VI, p. 5).

Một nghiệm bậc n của đơn vị được gọi là nguyên thủy nếu nó có cấp $n$; nếu tồn tại một nghiệm như thế $\zeta$, thì nhóm $\mu_n(K)$ có cấp $n$ và được sinh bởi $\zeta$. \* Chẳng hạn, các nghiệm bậc n nguyên thủy của đơn vị trong $\mathbf{C}$ là các số $e^{2\pi i k / n}$ với $0 \leq k < n$ và $k$ nguyên tố cùng nhau với $n$. \* Hệ quả 1 của Mệnh đề 3 nay suy ra kết quả sau.

#### Mệnh đề 4 {#alg-v-s11-prop-4 .statement}

— Cho $n \geq 1$ là một số nguyên; giả sử rằng tồn tại n nghiệm bậc n của đơn vị trong K (điều này đúng chẳng hạn nếu K đóng tách được và $n . 1, \neq 0$). Khi đó số các nghiệm bậc n nguyên thủy của đơn vị trong K bằng $\varphi(n)$.

### 4. Mở rộng cyclotomic

Cho $p$ là số mũ đặc số của K và cho $n \geq 1$ là một số nguyên nguyên tố cùng nhau với $p$; theo một mở rộng cyclotomic cấp $n$ trên K ta hiểu là bất kỳ mở rộng tách E nào của đa thức $X^n - 1$ trên K (V, p. 21). Vì đa thức này là tách được, nên E là một mở rộng Galois của K, có bậc hữu hạn (V, p. 57). Trong E tồn tại một nghiệm bậc n nguyên thủy của đơn vị; nếu $\zeta$ là một nghiệm như thế, thì mọi nghiệm bậc n của đơn vị đều là một lũy thừa của $\zeta$, do đó $E = K(\zeta)$.

Trong phần còn lại của số này, ta sẽ chọn một bao đóng tách được $K_s$ của K. Với mọi $n \geq 1$ nguyên tố cùng nhau với $p$, nhóm $\mu_n(K_s)$ là cyclic có cấp $n$ và trường

$$
R_n(K) = K(\mu_n(K_s))
$$

là một mở rộng luân nguyên mức $n$ của K. Ta có thể xem $\mu_n(K_s)$ như một môđun tự do hạng 1 trên vành $\mathbf{Z}/n\mathbf{Z}$, và mỗi phần tử $a$ của $\mathrm{Gal}(K_s/K)$ xác định một tự đẳng cấu của $\mu_n(K_s)$; do đó tồn tại một đồng cấu $\chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^*$ được đặc trưng bởi công thức $u(\zeta) = \zeta^j$ với mọi căn bậc $n$ của đơn vị $\zeta$ trong $K_s$, mọi $u$ trong $\mathrm{Gal}(K_s/K)$ và mọi số nguyên $j$ trong lớp thặng dư $\chi_n(u)$ mod $n$. Vì $R_n(K) = K(\mu_n(K_s))$, hạt nhân của $\chi_n$ là nhóm con $\mathrm{Gal}(K_s/R_n(K))$ của $\mathrm{Gal}(K_s/K)$; suy ra ta có $\chi_n = \varphi_n \circ \psi_n$ trong đó $\psi_n$ là đồng cấu hạn chế của $\mathrm{Gal}(K_s/K)$ lên $\mathrm{Gal}(R_n(K)/K)$ và $\varphi_n$ là một đơn cấu của $\mathrm{Gal}(R_n(K)/K)$ vào $(\mathbf{Z}/n\mathbf{Z})^*$. Đặc biệt ta có kết quả sau :

#### Mệnh đề 5 {#alg-v-s11-prop-5 .statement}

— Với mọi số nguyên $n \geq 1$ nguyên tố cùng $p$ thì mở rộng $R_n(K)$ của K là Abel có bậc hữu hạn, nhóm Galois của nó đẳng cấu với một nhóm con của $(\mathbf{Z}/n\mathbf{Z})^*$ và bậc của nó chia cấp $\varphi(n)$ của $(\mathbf{Z}/n\mathbf{Z})^*$.

Cho Q là một bao đóng đại số của trường Q các số hữu tỉ, và cho $n$ là một số nguyên. Khi đó đa thức luân nguyên mức $n$ được xác định bởi

$$
\Phi_n(X) = \prod_{\zeta \in S_n} (X - \zeta),
$$

trong đó $S_n$ là tập hợp các căn bậc $n$ nguyên thủy của đơn vị trong Q. Đa thức $\Phi_n$ có bậc $\varphi(n)$ (Mệnh đề 4). Rõ ràng $\Phi_n(X)$ bất biến dưới mọi tự đẳng cấu của $\bar{\mathbf{Q}}$, nên thuộc $\mathbf{Q}[X]$. Vì mọi phần tử $\zeta$ của $S_n$ là một nghiệm của đa thức $X^n - 1$, nên đa thức $\Phi_n(X)$ chia hết $X^n - 1$, và bổ đề sau cho thấy rằng $\Phi_n(X)$ là một đa thức đơn khởi với các hệ số nguyên.

#### Bổ đề 2 {#alg-v-s11-lem-2 .statement}

*Cho f, g và h là các đa thức đơn khởi trong $\mathbf{Q}[X]$ sao cho $f = gh$. Nếu f có các hệ số nguyên, thì điều đó cũng đúng với g và h.*

Hãy cho $a$ (tương ứng $b$) là số nhỏ nhất trong các số nguyên $\alpha \geq 3$ (tương ứng $\beta \geq 1$) sao cho $\alpha g$ (tương ứng $\beta h$) có hệ số nguyên; ta đặt $g' = ag$ và $h' = bh$ và chứng minh bằng *phản chứng* rằng $a = b = 1$. Nếu điều này không đúng, sẽ có một ước nguyên tố $p$ của $ab$. Nếu $u \in \mathbf{Z}[X]$, ta ký hiệu $\bar{u}$ là đa thức với hệ số trong trường $\mathbf{F}_p$ thu được bằng phép giảm modulo $p$ các hệ số của $u$. Ta có $g'h' = abf$, do đó $\bar{g}'\bar{h}' = 0$; vì vành $\mathbf{F}_p[X]$ là một miền nguyên (IV, p. 9, Mệnh đề 8) nên suy ra $\bar{g}' = 0$ hoặc $\bar{h}' = 0$. Nói cách khác, $p$ chia hết mọi hệ số của $g'$ hoặc mọi hệ số của $h'$ và điều này mâu thuẫn với giả thiết.

Ta có quan hệ

$$
X^n - 1 = \prod_{d|n} \Phi_d(X) .
$$

Thật vậy, ta có $X^n - 1 = \prod_{\zeta \in \mu_n(\mathbf{Q})} (X - \zeta)$ và các tập hợp $S_d$ với $d$ chia hết $n$ lập thành một phân hoạch của $\mu_n(\mathbf{Q})$.

Công thức (6) xác định $\Phi_n(X)$ khi ta biết $\Phi_d(X)$ với mọi ước $d < n$ của $n$; vì $\Phi_1(X) = X - 1$, do đó ta có một thủ tục truy hồi để tính $\Phi_n$. Ví dụ với số nguyên tố $p$ ta có

$$
X^p - 1 = (X - 1)\Phi_p(X) ,
$$

do đó

$$
\Phi_p(X) = X^{p-1} + X^{p-2} + \cdots + X + 1 ,
$$

và

$$
\Phi_{p^r+1}(X) = \Phi_p(X^{p^r}) \quad \text{cho} \quad r \geq 0 .
$$

Hãy liệt kê các giá trị của các đa thức $\Phi_n(X)$ với $1 \leq n \leq 12$:

$$
\begin{align*}
\Phi_1(X) &= X - 1 \\
\Phi_2(X) &= X + 1 \\
\Phi_3(X) &= X^2 + X + 1 \\
\Phi_4(X) &= X^2 + 1 \\
\Phi_5(X) &= X^4 + X^3 + X^2 + X + 1 \\
\end{align*}
$$

$$
\Phi_6(X) = X^2 - X + 1
$$
$$
\Phi_7(X) = X^6 + X^5 + X^4 + X^3 + X^2 + X + 1
$$
$$
\Phi_8(X) = X^4 + 1
$$
$$
\Phi_9(X) = X^6 + X^3 + 1
$$
$$
\Phi_{10}(X) = X^4 - X^3 + X^2 - X + 1
$$
$$
\Phi_{11}(X) = X^{10} + X^9 + X^8 + X^7 + X^6 + X^5 + X^4 + X^3 + X^2 + X + 1
$$
$$
\Phi_{12}(X) = X^4 - X^2 + 1
$$

Các giá trị của $\Phi_1, \Phi_2, \Phi_3, \Phi_4, \Phi_5, \Phi_7, \Phi_8, \Phi_9$ và $\Phi_{11}$ suy ra trực tiếp từ (7); lúc này ta có $\Phi_1 \Phi_2 \Phi_3 \Phi_6 = X^6 - 1$ và $\Phi_1 \Phi_2 \Phi_3 \Phi_4 \Phi_6 \Phi_{12} = X^{12} - 1$, do đó $\Phi_4 \Phi_{12} = \frac{X^{12} - 1}{X^6 - 1} - X^6 + 1$ và cuối cùng $\Phi_{12} = \frac{X^6 + 1}{X^2 + 1} = X^4 - X^2 + 1$. Hai trường hợp $n = 6$ và $n = 10$ có thể xử lý tương tự.

#### Nhận xét {#alg-v-s11-n4-rem-1 .statement}

\* Với mỗi số nguyên $n > 0$ một hàm $\mu(n)$ được định nghĩa như sau: nếu $n$ chia hết cho bình phương của một số nguyên tố, ta đặt $\mu(n) = 0$, ngược lại $\mu(n) = (-1)^h$ nếu $n$ là tích của $h$ số nguyên tố phân biệt (« hàm Mobius »). Có thể chứng minh rằng

$$
\Phi_n(X) = \prod_{d|n} (X^{n/d} - 1)^{\mu(d)},
$$

hoặc tường minh hơn

$$
\Phi_n(X) = \prod_{p_1 < \ldots < p_h} (X^{n/p_1 \cdots p_h} - 1)^{(-1)^h}
$$

trong đó $(p_1, \ldots, p_h)$ chạy qua tập hợp tất cả các dãy tăng ngặt các ước nguyên tố của $n$ (xem Lie, II, p. 207, Bài tập 1).

### 5. Tính bất khả quy của các đa thức cyclotomic

Cho $p$ là số mũ đặc số của $K$ và cho $n$ là một số nguyên nguyên tố cùng nhau với $p$. Ký hiệu bởi $\Phi_n \in K[X]$ ảnh của đa thức có hệ số nguyên $\Phi_n$ qua đồng cấu duy nhất của $\mathbf{Z}[X]$ vào $K[X]$ gửi $X$ thành $X$.

#### Bổ đề 3 {#alg-v-s11-lem-3 .statement}

*Các nghiệm của $\Phi_n$ trong $K_s$ là các căn nguyên thủy bậc $n$ của đơn vị.*

Ký hiệu $S$ là tập hợp các nghiệm của $\Phi_n$ trong $K_s$. Theo Công thức (6), tập hợp $\mu_n(K_s)$ là hợp của các $S_d$ với $d$ chia hết $n$. Vậy mọi căn nguyên thủy bậc $n$ của đơn vị đều thuộc $S_n$ và bổ đề suy ra từ Mệnh đề 4 (V, p. 81).

#### Mệnh đề 6 {#alg-v-s11-prop-6 .statement}

— Cho $p$ là số mũ đặc số của $K$ và cho $n \geq 1$ là một số nguyên nguyên tố cùng nhau với $p$. Để đa thức $\Phi_n(X)$ bất khả quy trong $K[X]$ thì điều kiện cần và đủ là đồng cấu $\chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^*$ phải toàn ánh.

Theo Bổ đề 3, ta có $R_n(K) = K(\zeta)$ với mỗi nghiệm $\zeta$ của $\Phi_n(X)$ và do đó $\Phi_n(X)$ bất khả quy trong $K[X]$ khi và chỉ khi bậc $\varphi(n)$ của $\Phi_n(X)$ bằng $[R_n(K):K]$. Hơn nữa, nhóm Galois của $R_n(K)$ trên $K$ có cấp $[R_n(K):K]$ và đẳng cấu với nhóm con của $(\mathbf{Z}/n\mathbf{Z})^*$ là ảnh của $\chi_n$. Mệnh đề 6 suy ra từ việc $(\mathbf{Z}/n\mathbf{Z})^*$ có cấp $\varphi(n)$.

#### Định lý 2 (Gauss) {#alg-v-s11-thm-2 .statement}

— Cho $Q$ là bao đóng đại số của $Q$ và cho $n \geq 1$ là một số nguyên.

a) Đa thức cyclotomic $\Phi_n(X)$ là bất khả quy trong $Q[X]$.

b) Bậc của $R_n(Q)$ trên $Q$ là $\varphi(n)$.

c) Đồng cấu $\chi_n$ của $\mathrm{Gal}(\bar{Q}/Q)$ vào $(\mathbf{Z}/n\mathbf{Z})^*$ là toàn ánh và xác định bằng cách đi qua các thương một đẳng cấu từ $\mathrm{Gal}(R_n(Q)/Q)$ lên $(\mathbf{Z}/n\mathbf{Z})^*$.

Xét đến Mệnh đề 6, ta chỉ cần chứng minh c). Mọi số nguyên $r$ nguyên tố cùng nhau với $n$ là một tích của các số nguyên tố $p_1, \ldots, p_s$ không chia hết cho $n$; do đó chỉ cần chứng minh rằng với mọi số nguyên tố $p$ không chia hết cho $n$, ánh xạ $x \mapsto x^p$ của $\mu_n(Q)$ vào chính nó mở rộng thành một tự đẳng cấu của $R_n(Q)$. Chỉ cần chứng minh rằng nếu $\zeta$ là một nghiệm đơn vị nguyên thủy bậc $n$, thì đa thức tối tiểu $f$ của $\zeta$ trên $Q$ bằng đa thức tối tiểu $g$ của $\zeta^p$ trên $Q$.

Ta sẽ giả sử rằng $f \neq g$ và lập luận bằng phản chứng. Các đa thức $f$ và $g$ là đơn thức bất khả quy trong $Q[X]$ và chia hết $X^n - 1$, nên tồn tại $u \in Q[X]$ sao cho $X^n - 1 = fg u$ (IV, p. 13, Mệnh đề 13). Bổ đề 2 (V, p. 82) cho thấy $f, g$ và $u$ có các hệ số nguyên. Ký hiệu $\bar{v}$ là đa thức với hệ số trong $\mathbf{F}_p$ thu được từ một đa thức $v \in \mathbf{Z}[X]$ bằng cách khử modulo $p$. Do đó ta có $X^n - 1 = \bar{f} \bar{g} \bar{u}$ trong $\mathbf{F}_p[X]$.

Hơn nữa, ta có $g(\zeta^p) = 0$ nên $g(X^p)$ là một bội của $f(X)$ trong $\mathbf{Q}[X]$. Theo Bổ đề 2 tồn tại $h \in \mathbf{Z}[X]$ sao cho $g(X^p) = f(X) \cdot h(X)$. Bây giờ ta có $v(X^p) = v(X)^p$ với mọi đa thức $v \in \mathbf{F}_p[X]$. Do đó khi giảm modulo $p$ ta thu được $\bar{g}^p = \bar{f} \bar{h}$. Nếu $v$ là một đa thức bất khả quy trong $\mathbf{F}_p[X]$ chia hết $\bar{f}$, thì nó phải chia hết $\bar{g}$. Vì $\bar{f} \bar{g}$ chia hết $X^n - 1$, ta suy ra rằng $v^2$ chia hết $X^n - 1$ trong $\mathbf{F}_p[X]$. Điều này là vô lý vì đa thức $X^n - 1$ là tách được trong $\mathbf{F}_p[X]$.

Có thể chứng minh rằng với mọi mở rộng Abel $E$ có bậc hữu hạn trên $Q$ tồn tại một số nguyên $n \geq 1$ sao cho $E$ đẳng cấu với một mở rộng con của $R_n(Q)$. \* Nói cách khác, trường $Q(\mu_{\infty}(C))$ là một bao đóng Abel của $Q$. *(« định lý Kronecker-Weber »).

### 6. Các mở rộng cyclic

#### Định nghĩa 3 {#alg-v-s11-def-3 .statement}

— *Một mở rộng E của K được gọi là cyclic nếu nó là Galois và nhóm Galois của nó là cyclic.*

*Ví dụ. — 1) Mọi mở rộng Galois có bậc nguyên tố đều là cyclic, vì mọi nhóm hữu hạn G có cấp nguyên tố $p$ đều cyclic (vì mọi phần tử $x \neq 1$ của G đều có cấp $p$, do đó sinh ra G).

2) Cho $F(X) = X^2 + aX + b$ là một đa thức bất khả quy trong $K[X]$. Trường hợp duy nhất mà $F(X)$ không tách được là trường hợp $K$ có đặc số 2 và $a = 0$. Ta sẽ bỏ qua trường hợp này; cho E là một mở rộng của K được sinh bởi một nghiệm $x$ của $F(X)$. Ta có $[E : K] = 2$ và $F(X) = (X - x)(X + a + x)$, do đó E là một mở rộng Galois của K. Nhóm Galois của E trên K có cấp 2, nên cyclic.

3) Cho $\mathbf{F}$ là một trường và $\sigma$ là một tự đẳng cấu có bậc hữu hạn. Trường E gồm các bất biến của $\sigma$ cũng là trường bất biến của nhóm cyclic có cấp $n$ được sinh bởi $\sigma$, và do đó (V, p. 66, Định lý 3) F là một mở rộng cyclic bậc $n$ của E.

Ta biết (I, p. 50) rằng mọi *nhóm con* và mọi *nhóm thương* của một nhóm cyclic đều cyclic. Do đó (V, p. 68, Hệ quả 4), nếu E là một mở rộng cyclic của một trường K, có bậc $n$, thì mọi mở rộng con F của E đều *cyclic trên K*, và *E cyclic trên F*. Với mọi ước d của $n$ tồn tại duy nhất một trường con F bậc d trên K được chứa trong E : vì trong một nhóm cyclic có cấp $n$ tồn tại duy nhất một nhóm con có chỉ số d.

#### Định lý 3 (*Hilbert*) {#alg-v-s11-thm-3 .statement}

— *Cho E là một mở rộng cyclic của K và cho a là một phần tử sinh của nhóm Galois $\Gamma$ của E trên K.

a) Để một phần tử $x \in E$ thỏa mãn $N_{E/K}(x) = 1$ thì cần và đủ rằng tồn tại $y \in E^*$ sao cho $x = y / \sigma(y)$; khi đó mọi $y_1 \in E^*$ thỏa $x = y_1 / \sigma(y_1)$ đều có dạng $\lambda y$ với $\lambda \in K^*$.

b) Để một phần tử $x \in E$ thỏa mãn $\mathrm{Tr}_{E/K}(x) = 0$ thì cần và đủ là tồn tại $z \in E$ sao cho $x = z - \sigma(z)$; khi đó mọi $z_1 \in E$ sao cho $x = z_1 - \sigma(z_1)$ đều có dạng $z + \mu$, với $\mu \in K$.

Trước hết hãy chứng minh một bổ đề.*

#### Bổ đề 4 {#alg-v-s11-lem-4 .statement}

*Cho $\Gamma$ là một nhóm cyclic cấp $n$, $\sigma$ là một phần tử sinh của $\Gamma$ và M là một nhóm giao hoán trên đó $\Gamma$ tác động theo quy tắc $\gamma . (m + m') = \gamma . m + \gamma . m'$ với mọi $\gamma \in \Gamma$ và $m, m' \in M$. Gọi Z là tập hợp mọi ánh xạ của $\Gamma$ vào M thỏa mãn quan hệ*

$$
f(\tau \tau') = f(\tau) + \tau . f(\tau') \quad \text{đối với } \tau, \tau' \text{ trong } \Gamma
$$

Đặt $u(f) = f(a)$ cho $f \in Z$ và $t(m) = \sum_{\tau \in \Gamma} \tau . m$ cho $m \in M$. Khi đó dãy

$$
0 \to Z \xrightarrow{u} M \xrightarrow{t} M
$$

là khớp.

Cho $f \in \mathbf{Z}$; lấy $\tau = \tau' = 1$ trong (10) ta thấy rằng $f(1) = 0$. Hơn nữa, bằng quy nạp theo $m \geqslant 0$ ta suy ra quan hệ

$$
f(\sigma^m) = f(\sigma) + \sigma \cdot f(\sigma) + \cdots + \sigma^{m-2} \cdot f(\sigma) + \sigma^{m-1} \cdot f(\sigma)
$$

Ta có $\sigma^n = 1$, do đó $f(\sigma^n) = 0$; quan hệ trước với $m = n$ tương đương với đẳng thức $t(u(f)) = 0$, do đó $\operatorname{Im}\ u \subset \operatorname{Ker}\ t$. Hơn nữa, từ (11) suy ra rằng $\operatorname{Ker}\ u = 0$.

Cho $m \in M$ sao cho $t(m) = 0$, tức là $m + \sigma \cdot m + \cdots + \sigma^{n-1} \cdot m = 0$. Đặt ánh xạ $f$ của $\Gamma$ vào $M$ bởi

$$
f(\sigma^j) = m + \sigma \cdot m + \cdots + \sigma^{j-2} \cdot m + \sigma^{j-1} \cdot m
$$

với $0 \leqslant j \leqslant n - 1$. Có thể để bạn đọc thiết lập quan hệ (10). Rõ ràng ta có $m = f(a)$, do đó $\operatorname{Im}\ u \supset \operatorname{Ker}\ t$.

Với bổ đề vừa được chứng minh, ta lấy $y \in E^*$ và $x = y/\sigma(y)$; ta có $N_{E/K}(\sigma(y)) = N_{E/K}(y)$, do đó $N_{E/K}(x) = 1$. Ngược lại, cho $x$ trong $E^*$ sao cho $N_{E/K}(x) = 1$; theo Bổ đề 4, áp dụng cho $M = E^*$, tồn tại một họ các phần tử $(c_\tau)_{\tau \in \Gamma}$ của $E^*$ thỏa mãn quan hệ $c_{\tau \tau'} = c_\tau \cdot \tau(c_{\tau'})$ với $\tau, \tau'$ trong $\Gamma$ và $c_\sigma = x$. Theo Hệ quả 1 của Mệnh đề 9 (V, p. 65) tồn tại $y \in E^*$ sao cho $c_\tau = y/\tau(y)$ với mọi $\tau \in \Gamma$, do đó đặc biệt $x = c_\sigma = y/\sigma(y)$. Nếu $y_1 \in E^*$ thỏa mãn $x = y_1/\sigma(y_1)$, thì ta có

$$
\sigma(y_1 y^{-1}) = y_1 y^{-1},
$$

suy ra $y_1 y^{-1}$ thuộc $K^*$ vì $a$ sinh ra nhóm Galois của $E$ trên $K$. Điều đó chứng minh a).

Mệnh đề b) suy ra theo cách tương tự từ Hệ quả 2 của Mệnh đề 9 (V, p. 65).

### 7. Tính đối ngẫu của các $\mathbf{Z}/n\mathbf{Z}$-môđun

Trong mục này, ta ký hiệu $n$ là một số nguyên $> 0$ và $T$ là một nhóm cyclic có cấp $n$. Một nhóm $G$ được gọi là bị triệt tiêu bởi $n$ nếu $g^n = 1$ với mọi $g \in G$; nếu hơn nữa $G$ giao hoán, cấu trúc nhóm của $G$ làm nền cho một cấu trúc $\mathbf{Z}/n\mathbf{Z}$-môđun duy nhất.

Với mọi nhóm $G$, ta ký hiệu $\operatorname{Hom}(G, T)$ là nhóm các đồng cấu từ $G$ vào $T$; đó là một nhóm giao hoán bị triệt tiêu bởi $n$.

#### Mệnh đề 7 {#alg-v-s11-prop-7 .statement}

— Cho $G$ là một nhóm giao hoán bị triệt tiêu bởi $n$ và $H$ là một nhóm con của $G$. Khi đó đồng cấu hạn chế $\operatorname{Hom}(G, T) \to \operatorname{Hom}(H, T)$ là toàn ánh.

Xét $f : H \to T$ là một đồng cấu; ta sẽ chứng minh rằng tồn tại một đồng cấu từ $G$ vào $T$ mở rộng $f$. Trước hết giả sử $G$ là một nhóm cyclic, sinh bởi một phần tử $g$ có cấp $r$ chia $n$; ký hiệu $t$ là một phần tử sinh của $T$. Tồn tại một ước s của r sao cho H được sinh bởi $g^s$ (I, p. 50, Mệnh đề 19), và với mọi $x \in \mathbf{Z}$ ta có $f(g^{sx}) = t^{ax}$, trong đó a là một số nguyên sao cho n chia $ar/s$. Khi đó $a/s = (ar/ns)(n/r)$ là một số nguyên và đồng cấu $g^x \mapsto t^{(a/s)x}$, $x \in \mathbf{Z}$, từ G vào T mở rộng f. Trong trường hợp tổng quát xét tập hợp các cặp $(H', f')$ trong đó $H'$ là một nhóm con của G chứa H và $f'$ là một đồng cấu của $H'$ vào T mở rộng $f$, và ta đặt thứ tự trên tập hợp này theo quan hệ $(H', f') \leq (H'', f'')$ nếu $H' \subset H''$ và phần hạn chế của $f''$ lên $H'$ là $f'$. Theo Lý thuyết tập hợp, III, p. 154, Định nghĩa 3 và Định lý 2, tập hợp này có một phần tử cực đại $(H_1, f_1)$ và chỉ cần chứng minh rằng $H_1 = G$; nếu không phải vậy, tồn tại $g \in G, g \notin H_1$ và chỉ cần chứng minh rằng $f_1$ có thể được mở rộng thành một đồng cấu vào T của nhóm con của G sinh bởi $H_1$ và g. Bây giờ nếu C ký hiệu nhóm cyclic sinh bởi g, thì phần hạn chế của $f_1$ lên $C \cap H_1$ mở rộng được thành một đồng cấu $f_2$ của C vào T và đồng cấu $xy \mapsto f_1(x) f_2(y), x \in H_1, y \in C,$ từ $H_1C$ vào T là ánh xạ mong muốn.

#### Hệ quả 1 {#alg-v-s11-prop-7-cor-1 .statement}

— Nếu G *là* một nhóm giao hoán bị triệt tiêu bởi *n*, và $G \neq \{1\}$, thì $\mathrm{Hom}(G, T) \neq \{1\}$.

Điều đó đủ vì chỉ cần nhận xét rằng nếu H là một nhóm con cyclic khác $\{1\}$ của G, thì $\mathrm{Hom}(H, T) \neq \{1\}$, và áp dụng Mệnh đề 7.

#### Hệ quả 2 {#alg-v-s11-prop-7-cor-2 .statement}

— Nếu G *là* một nhóm giao hoán *hữu hạn* bị triệt tiêu bởi *n*, thì các nhóm G và $\mathrm{Hom}(G, T)$ cùng cấp.

Nếu G là cyclic có cấp *r*, với phần tử sinh g, thì ánh xạ $f \mapsto f(g)$ là một song ánh từ $\mathrm{Hom}(G, T)$ lên tập hợp các phần tử t của T sao cho $t^r = 1$, do đó khẳng định suy ra trong trường hợp này. Mặt khác, nếu H là một nhóm con cyclic của G, ta có $\mathrm{Card}(G) = \mathrm{Card}(H) \cdot \mathrm{Card}(G/H)$; hơn nữa, ta có một dãy khớp

$$
\{1\} \to \mathrm{Hom}(G/H, T) \to \mathrm{Hom}(G, T) \to \mathrm{Hom}(H, T) \to \{1\}
$$

(II, p. 227, Định lý 1 và Mệnh đề 7 ở trên), do đó

$$
\mathrm{Card}(\mathrm{Hom}(G, T)) = \mathrm{Card}(\mathrm{Hom}(H, T)) \cdot \mathrm{Card}(\mathrm{Hom}(G/H, T)).
$$

Vì $\mathrm{Card}(\mathrm{Hom}(H, T)) = \mathrm{Card}(H)$, việc chứng minh hệ quả cho G hay cho $G/H$ là như nhau. Bây giờ kết quả suy ra bằng quy nạp theo $\mathrm{Card}(G)$.

Bây giờ xét G và H là hai nhóm và $f : G \times H \to T$ là một ánh xạ song nhân, nghĩa là sao cho với mọi $g, g' \in G, h, h' \in H$ ta có

$$
f(gg', h) = f(g, h) f(g', h), \quad f(g, hh') = f(g, h) f(g, h')
$$

Ta định nghĩa các đồng cấu nhóm

$$
s_f : G \to \mathrm{Hom}(H, T), \quad d_f : H \to \mathrm{Hom}(G, T),
$$

bởi $s_f(g)(h) = d_f(h)(g) = f(g, h)$ (xem II, p. 268, Hệ quả của Mệnh đề 1, khi G và H giao hoán).

#### Mệnh đề 8 {#alg-v-s11-prop-8 .statement}

— *Giả sử G và H giao hoán và bị triệt tiêu bởi n. Nếu s_f là song ánh và H hữu hạn, thì d_f là song ánh và ta có Card(G) = Card(H).*

Nếu s_f là song ánh và H hữu hạn, theo Hệ quả 2 của Mệnh đề 7 ở trên ta có quan hệ Card(G) = Card(Hom(H, T)) = Card(H), do đó Card(G) là hữu hạn và bằng một lần áp dụng Hệ quả nữa, Card(Hom(G, T)) = Card(H). Vậy chỉ còn phải chứng minh rằng d_f là đơn ánh. Bây giờ nếu $h \in \mathrm{Ker}(d_f)$, ta có $f(g, h) = 1$ với mọi $g \in G$, nên vì s_f là song ánh, $\varphi(h) = 1$ với mọi $\varphi \in \mathrm{Hom}(H, T)$; theo Mệnh đề 7 điều đó suy ra $\mathrm{Hom}(\mathrm{Ker}(d_f), T) = \{1\}$, do đó $\mathrm{Ker}(d_f) = \{1\}$ theo Hệ quả 1 của Mệnh đề 7.

### 8. Lý thuyết Kummer

Trong mục này ta ký hiệu $n$ là một số nguyên > 0, và ta giả sử rằng $\mu_n(K)$ có $n$ phần tử; theo V, p. 78 điều đó cũng có nghĩa là $n$ nguyên tố cùng nhau với số mũ đặc số của K và rằng mọi căn bậc n của đơn vị trong một bao đóng đại số $\Omega$ của K đều nằm trong K.

Ta sẽ nói rằng một mở rộng L của K là *Abel có số mũ chia hết cho n* nếu nó là Abel (V, p. 77, Đn. 1) và nhóm Galois của nó $\mathrm{Gal}(L/K)$ bị triệt tiêu bởi $n$ (V, p. 86).

Cho A là một tập con của $K^*$; ta ký hiệu $K(A^{1/n})$ là tiểu mở rộng của $\Omega$ được sinh bởi mọi $0 \in \Omega$ sao cho $\theta^n \in A$.

#### Bổ đề 5 {#alg-v-s11-lem-5 .statement}

— *$K(A^{1/n})$ là một mở rộng Abel của K có số mũ chia hết cho n.*

Vì các đa thức $X^n - a, a \in A$ tách được trên K, nên $L = K(A^{1/n})$ là một mở rộng tách được, do đó là một mở rộng Galois của K. Lấy $\sigma \in \mathrm{Gal}(L/K)$ và lấy $0 \in \Omega$ sao cho $\theta^n \in A$. Ta có $\sigma(\theta)^n = \theta^n$; do đó tồn tại $\zeta \in \mu_n(\Omega) = \mu_n(K)$ sao cho $\sigma(\theta) = \zeta \theta$; điều này suy ra $\sigma^n(\theta) = \zeta^n \theta = 0$, do đó $\sigma^n = 1$. Nếu $\sigma'$ là một phần tử khác của $\mathrm{Gal}(L/K)$ thì tồn tại $\zeta' \in \mu_n(K)$ sao cho $\sigma'(\theta) = \zeta' \theta$, do đó $\sigma'\sigma(\theta) = \zeta \zeta' \theta = \sigma\sigma'(\theta)$ và vì vậy $\sigma'\sigma = \sigma\sigma'$.

#### Bổ đề 6 {#alg-v-s11-lem-6 .statement}

— *Cho L là một mở rộng Galois của K. Tồn tại một ánh xạ duy nhất $(\sigma, a) \mapsto \langle \sigma, a \rangle$ từ $\mathrm{Gal}(L/K) \times ((L^n \cap K^*)/K^{*n})$ vào $\mu_n(K)$ sao cho với mọi $\sigma \in \mathrm{Gal}(L/K)$ và mọi phần tử $0 \in L^*$ sao cho $\theta^n \in K$ ta có, khi ký hiệu $\overline{\theta^n}$ là lớp thặng dư của $\theta^n$ mod $K^{*n}$:*

$$
\langle \sigma, \overline{\theta^n} \rangle = \sigma(\theta)/\theta
$$

*Ánh xạ này là song tuyến tính.*

Thực vậy vế phải của (13) là một căn bậc n của đơn vị chỉ phụ thuộc vào lớp thặng dư mod $K^{*n}$ của $\theta^n$; điều này chứng minh mệnh đề thứ nhất. Mệnh đề thứ hai được kiểm tra không khó khăn.

Với mọi mở rộng Galois L của K ta viết

$$
k_L : (L^n \cap K^*)/K^{*n} \to \mathrm{Hom}(\mathrm{Gal}(L/K), \mu_n(K)) ,
$$
$$
k'_L : \mathrm{Gal}(L/K) \to \mathrm{Hom}((L^n \cap K^*)/K^{*n}, \mu_n(K)) ,
$$

cho các đồng cấu thu được từ ánh xạ song tuyến tính trên (V, p. 87).

#### Mệnh đề 9 {#alg-v-s11-prop-9 .statement}

*Với mọi mở rộng Galois hữu hạn L của K, đồng cấu $k_L$ là song ánh.*

Cho $0 \in L^*$ sao cho $0^n \in K$ và lớp thặng dư của $0^n \mod K^{*n}$ thuộc hạt nhân của $k_L$. Với mọi $\sigma \in \mathrm{Gal}(L/K)$ theo định nghĩa ta có $\sigma(\theta) = 0$; do đó $0 \in K^*$ và $\theta^n \in K^{*n}$. Điều này chứng minh tính đơn ánh của $k_L$. Bây giờ hãy cho $f : \mathrm{Gal}(L/K) \to \mu_n(K)$ là một đồng cấu; với mọi $\sigma, \tau \in \mathrm{Gal}(L/K)$ ta có

$$
f(\sigma \tau) = f(\sigma) f(\tau) = f(\sigma) \cdot \sigma f(\tau) , \quad f(\sigma)^n = 1 .
$$

Theo V, p. 65, Hệ quả 1 tồn tại $0 \in L^*$ sao cho $f(\sigma) = \sigma(\theta)/\theta$ với mọi $\sigma \in \mathrm{Gal}(L/K)$; vì $f(\sigma)^n = 1$, ta có $\sigma(\theta^n) = 0^n$ với mọi $\sigma \in \mathrm{Gal}(L/K)$, do đó $0^n \in K^*$; nếu $a$ là lớp thặng dư của $\theta^n \mod K^{*n}$, thì theo định nghĩa ta có $f(\sigma) = \langle \sigma, a \rangle$ với $\sigma \in \mathrm{Gal}(L/K)$, do đó $f = k_L(a)$.

#### Hệ quả {#alg-v-s11-n8-cor-1 .statement}

*Nếu L là một mở rộng Galois của K, thì đồng cấu $k_L$ là đơn ánh và ảnh của nó là nhóm $\mathrm{Hom}_c(\mathrm{Gal}(L/K), \mu_n(K))$ gồm các đồng cấu liên tục của nhóm tôpô $\mathrm{Gal}(L/K)$ vào nhóm rời rạc $\mu_n(K)$.*

Điều này suy ra ngay từ những gì đã nói, dùng तथ्य rằng L là một hợp có hướng tăng của các mở rộng Galois $L_i$ có bậc hữu hạn và rằng đồng cấu của $\mathrm{Gal}(L/K)$ vào $\mu_n(K)$ là liên tục khi và chỉ khi nó có thể được phân tích qua một trong các thương $\mathrm{Gal}(L_i/K)$ của $\mathrm{Gal}(L/K)$.

#### Định lý 4 {#alg-v-s11-thm-4 .statement}

*a) Ánh xạ $H \mapsto K(H^{1/n})$ là một song ánh bảo toàn bao hàm từ tập hợp các nhóm con của $K^*$ chứa $K^{*n}$ lên tập hợp các mở rộng con Abel của số mũ chia hết cho n của $\Omega$. Ánh xạ ngược là $L \mapsto L'' \cap K^*$.

b) Với mọi nhóm con H của $K^*$ chứa $K^{*n}$, đồng cấu

$$
k' : \mathrm{Gal}(K(H^{1/n})/K) \to \mathrm{Hom}(H/K^{*n}, \mu_n(K))
$$

là song ánh, và nó là một đồng phôi khi nhóm $\mathrm{Hom}(H/K^{*n}, \mu_n(K))$ được trang bị tôpô hội tụ đơn.

c) Cho H là một nhóm con của $K^*$ chứa $K^{*"n}$. Với mọi $a \in H/K^{*n}$ hãy lấy $\theta_a$ là một phần tử của $\Omega$ sao cho $\theta_a^n$ là một đại diện của a trong H. Khi đó các $\theta_a, a \in H/K^{*n}$, lập thành một cơ sở của không gian vectơ trên K $K(H^{1/n})$. Đặc biệt,

$$
[K(H^{1/n}):K] = (H:K^{*"n}) .
$$

A) Với mỗi mở rộng Abel của K có số mũ chia hết cho n, đặt $H_L = L'' \cap K^*$. Nếu $[L:K]$ là hữu hạn, thì đồng cấu $k'_L$ của $\mathrm{Gal}(L/K)$ vào $\mathrm{Hom}(H_L, \mu_n(K))$ là song ánh theo Mệnh đề 9 và V, p. 88, Mệnh đề 8.

Vì mọi mở rộng Abel của K có số mũ chia hết cho $n$ là một hợp có hướng tăng của các mở rộng con Abel hữu hạn bậc có số mũ chia hết cho $n$, ta suy ra bằng cách chuyển sang giới hạn ngược rằng $k'_L$ là một đồng phôi của các nhóm tôpô đối với mọi mở rộng Abel L của K có số mũ chia hết cho n.

B) Cho L là một mở rộng Abel của bậc hữu hạn, có số mũ chia hết cho $n$, của K, và cho $L' = K(H_L^{1/n})$; đây là một mở rộng con của L ; hơn nữa $H_{L'}$ chứa $H_L$ nên bằng nó. Vì các đồng cấu $k'_L$ và $k'_{L'}$ là song ánh theo A) và $H_L = H_{L'}$, nên các nhóm Gal$(L/K)$ và Gal$(L'/K)$ có cùng cấp và do đó bằng nhau. Điều này cho thấy rằng $L' = L$, và suy ra $L = K(H_L^{1/n})$. Nếu L là một mở rộng Abel có số mũ chia hết cho $n$ của K, thì ta có $K(H_L^{1/n}) = L$, vì $K(H_L^{1/n})$ là một mở rộng con của L chứa mọi mở rộng con hữu hạn của L.

C) Cho H là một nhóm con của $K^*$ chứa $K^{*n}$; đặt $L = K(H^{1/n})$, khi đó đây là một mở rộng Abel của K có số mũ chia hết cho $n$ (V, p. 88, Bổ đề 5). Ta có $H \subset H_L$, do đó ta thu được một dãy khớp của các nhóm giao hoán bị triệt tiêu bởi $n$

$$
\{1\} \to H/K^{*n} \to H_L/K^{*n} \to H_L/H \to \{1\}.
$$

Từ đó ta thu được một dãy khớp

$$
\{1\} \to \operatorname{Hom}(H_L/H, \mu_n(K)) \to \operatorname{Hom}(H_L/K^{*n}, \mu_n(K)) \xrightarrow{\iota} \operatorname{Hom}(H/K^{*n}, \mu_n(K)),
$$

trong đó $\iota$ là đồng cấu hạn chế.

Nếu ta đồng nhất $\operatorname{Hom}(H_L/K^{*n}, \mu_n(K))$ với Gal$(L/K)$ bằng đẳng cấu $k'_L$, thì hạt nhân của $\iota$ được đồng nhất với tập hợp các $\sigma \in \operatorname{Gal}(L/K)$ sao cho $\sigma(\theta) = \theta$ với mọi $\theta \in H^{1/n}$. Suy ra $\iota$ là đơn ánh, nên $\operatorname{Hom}(H_L/H, \mu_n(K))$ bị rút về (1) ; bởi Hệ quả 1 của V, p. 87 ta do đó có $H = H_L$. Điều này hoàn tất chứng minh của a) và b).

D) Chứng minh c). Nếu $a, b \in H$, ta có $\theta_a \theta_b / \theta_{ab} \in K$. Suy ra không gian con vectơ của $K(H^{1/n})$ được sinh bởi các $\theta_a$ là ổn định dưới phép nhân và do đó trùng với $K(H^{1/n})$. Chỉ còn phải chứng minh rằng các $\theta_a$ độc lập tuyến tính ; để làm điều này rõ ràng ta có thể giả sử rằng $H/K^{*n}$ là hữu hạn ; khi đó $[K(H^{1/n}) : K] = (\operatorname{Gal}(K(H^{1/n})/K) : \{1\}) = (H : K^{*n})$ theo b) và Hệ quả 2 của V, p. 87 ; vì số của các $\theta_a$ bằng $(H : K^{*n})$ và chúng sinh ra không gian vectơ K $K(H^{1/n})$, nên chúng độc lập tuyến tính.

#### Ví dụ 1 {#alg-v-s11-n8-exa-1 .statement}

Tồn tại một mở rộng Abel lớn nhất có số mũ chia hết cho $n$ của K, chứa trong $\Omega$ ; nó được thu được bằng cách thêm vào K các căn bậc n của mọi phần tử của nó ; nhóm Galois của nó có thể được đồng nhất với $\operatorname{Hom}(K^*/K^{*n}, \mu_n(K))$, do đó cũng với $\operatorname{Hom}(K^*, \mu_n(K))$.

#### Ví dụ 2 {#alg-v-s11-n8-exa-2 .statement}

Hãy lấy $K = \mathbf{Q}$ và $n = 2$. Khi đó $\mathbf{Q}^*/\mathbf{Q}^{*2}$ là một không gian vectơ $\mathbf{F}_2$ có làm cơ sở hợp của $\{-1\}$ và tập hợp mọi số nguyên tố. Mở rộng Abel lớn nhất có số mũ 2 của Q chứa trong $\mathbf{C}$ do đó là trường con $\mathbf{Q}(i, \sqrt{2}, \sqrt{3}, \sqrt{5}, \ldots)$ của $\mathbf{C}$. Nhóm Galois của nó gồm tất cả các tự đẳng cấu thu được bằng cách nhân từng phần tử $i,\ \sqrt{2},\ \sqrt{3},\ \sqrt{5}$ v.v. với $\pm 1$. \*

#### Ví dụ 3 {#alg-v-s11-n8-exa-3 .statement}

Cho L là một phần mở rộng cyclic của K bậc $n$; khi đó nhóm $(L^n \cap K^*)/K^{*n}$ là cyclic cấp $n$. Nếu $a \in K^*$ sao cho lớp thặng dư của $a$ modulo $K^{*n}$ là một phần tử sinh của nhóm này, thì L là K-đẳng cấu với $K[X]/(X^n - a)$ và nhóm $\mathrm{Gal}(L/K)$ gồm $n$ tự đẳng cấu gửi $X$ tới $\zeta X$, $\zeta \in \mu_n(K)$.

#### Ví dụ 4 {#alg-v-s11-n8-exa-4 .statement}

Ngược lại, cho $a \in K^*$ và cho $r$ là số nguyên nhỏ nhất $> 0$ sao cho $a' \in K^{*n}$; khi đó trường con $L$ của $\Omega$ được sinh bởi các nghiệm của đa thức $X^n - a$ là một phần mở rộng cyclic của K bậc $r$. Đặc biệt, $X^n - a$ bất khả quy khi và chỉ khi $r = n$.

#### Nhận xét {#alg-v-s11-n8-rem-1 .statement}

Cho $a \in K^*$ và cho r là số nguyên nhỏ nhất $> 0$ sao cho $a' \in K^n$. Gọi B là tập hợp các nghiệm trong K của đa thức $X^{n/r} - a$; khi đó ta có

$$
X^n - a = \prod_{b \in B} (X' - b),
$$

bằng phép thế của $X'$ cho T trong quan hệ $T^{n/r} - a = \Pi (T - b)$. Theo Ví dụ 4, mỗi đa thức $X' - b$ đều bất khả quy, do đó (14) là phân tích của $X^n - a$ thành các đa thức bất khả quy trong $K[X]$.

### 9. Lý thuyết Artin-Schreier

Trong mục này, ta sẽ dùng $p$ để ký hiệu một số nguyên tố và giả thiết rằng K có đặc số $p$. Ta ký hiệu $\Omega$ là một bao đóng đại số của K và $\varphi$ là tự đồng cấu của nhóm cộng của $\Omega$ được xác định bởi

$$
\varphi(x) = x^p - x.
$$

Theo V, p. 93 hạt nhân của $\varphi$ là trường con nguyên tố $\mathbf{F}_p$ của K. Với mọi tập con $A$ của K, ta ký hiệu $K(\varphi^{-1}(A))$ là phần mở rộng con của $\Omega$ được sinh bởi mọi $x \in \Omega$ sao cho $\varphi(x) \in A$.

#### Bổ đề 7 {#alg-v-s11-lem-7 .statement}

$K(\varphi^{-1}(A))$ là một phần mở rộng Abel của K có số mũ chia hết cho $p$.

Vì các đa thức $\varphi - a = X^p - X - a,\ a \in A$ là tách được trên $K$, nên mở rộng $L = K(\varphi^{-1}(A))$ là Galois. Cho $a \in \mathrm{Gal}(L/K)$ và $x \in \varphi^{-1}(A)$; ta có $\varphi(\sigma(x)) = \varphi(x)$, do đó $\sigma(x) - x \in \mathbf{F}_p$, tức là $\sigma(x) = x + i,\ i \in \mathbf{F}_p$. Điều này suy ra $\sigma^p(x) = x + pi = x$, do đó $u^p = 1$; tương tự nếu $a' \in \mathrm{Gal}(L/K)$ và $\sigma'(x) = x + j$, thì ta có $\sigma \circ \sigma'(x) = x + i + j = a' \circ \sigma(x)$, nên $\sigma \circ \sigma' = \sigma' \circ \sigma$.

#### Bổ đề 8 {#alg-v-s11-lem-8 .statement}

Cho L là một mở rộng Galois của K. Tồn tại một ánh xạ duy nhất $(\sigma, a) \mapsto [a, a')$ của $\mathrm{Gal}(L/K) \times ((\varphi(L) \cap K)/\varphi(K))$ vào $\mathbf{F}_p$ sao cho với mọi $\sigma \in \mathrm{Gal}(L/K)$ và mọi phần tử $x \in L$ sao cho $\varphi(x) \in K$ ta có, ký hiệu $\overline{\varphi(x)}$ là lớp thặng dư của $\varphi(x)$ modulo $\varphi(K)$,

$$
[\sigma, \overline{\varphi(x)}] = \sigma(x) - x.
$$

Ánh xạ này là song tuyến tính trên Z (với $\sigma, \tau \in \mathrm{Gal}(L/K)$, $a, b \in (\mathcal{P}(L) \cap K)/\mathcal{P}(K)$, ta có $[\sigma \tau, a) = [\sigma, a) + [\tau, a)$, $[\sigma, a + b) = [\sigma, a) + [a, b)$).

Vế phải của (15) là một phần tử của $\mathbf{F}_p$ chỉ phụ thuộc vào lớp thặng dư của $\mathcal{P}(x) \mod \mathcal{P}(K)$; điều này chứng minh mệnh đề thứ nhất; mệnh đề thứ hai có thể được kiểm tra dễ dàng.

Với mọi mở rộng Galois $L$ của $K$, ta viết

$$
a_L : (\mathcal{P}(L) \cap K)/\mathcal{P}(K) \to \mathrm{Hom}(\mathrm{Gal}(L/K), \mathbf{F}_p)
$$
$$
a_L' : \mathrm{Gal}(L/K) \to \mathrm{Hom}((\mathcal{P}(L) \cap K)/\mathcal{P}(K), \mathbf{F}_p)
$$

cho các đồng cấu thu được từ ánh xạ song tuyến tính trên Z ở trên (V, p. 87).

#### Mệnh đề 10 {#alg-v-s11-prop-10 .statement}

*Với mọi mở rộng Galois $L$ có bậc hữu hạn của $K$, đồng cấu $a_L$ là song ánh.*

Cho $x \in L$ sao cho $\mathcal{P}(x) \in K$ và lớp thặng dư của $\mathcal{P}(x) \mod \mathcal{P}(K)$ nằm trong hạt nhân của $a_L$. Với mọi $\sigma \in \mathrm{Gal}(L/K)$ ta có theo định nghĩa $\sigma(x) = x$; do đó $x \in K$ và $\mathcal{P}(x) \in \mathcal{P}(K)$. Điều này chứng minh tính đơn ánh của $a_L$. Bây giờ cho $f : \mathrm{Gal}(L/K) \to \mathbf{F}_p$ là một đồng cấu; với mọi $\sigma, \tau \in \mathrm{Gal}(L/K)$ ta có

$$
f(\sigma \tau) = f(\sigma) + \sigma(f(\tau)), \quad f(\sigma) \in \mathbf{F}_p.
$$

Theo V, p. 65, Hệ quả 2 tồn tại $x \in L$ sao cho $f(u) = \sigma(x) - x$ với mọi $o \in \mathrm{Gal}(L/K)$. Vì $f(o) \in \mathbf{F}_p$ nên ta có $\mathcal{P}(\sigma(x)) = \mathcal{P}(x)$, do đó $\sigma(\mathcal{P}(x)) = \mathcal{P}(x)$ với mọi $a \in \mathrm{Gal}(L/K)$ và $\mathcal{P}(x) \in K$. Nếu $a$ là lớp thặng dư của $\mathcal{P}(x) \mod \mathcal{P}(K)$, ta có $f(\sigma) = [\sigma, a)$, nên $f = a_L(a)$.

#### Hệ quả {#alg-v-s11-n9-cor-1 .statement}

*Nếu $L$ là một mở rộng Galois của $K$, thì đồng cấu $a_L$ là đơn ánh và ảnh của nó là nhóm $\mathrm{Hom}_c(\mathrm{Gal}(L/K), \mathbf{F}_p)$ các đồng cấu liên tục của nhóm tôpô $\mathrm{Gal}(L/K)$ vào nhóm rời rạc $\mathbf{F}_p$.*

Điều này được chứng minh theo cùng cách như Hệ quả của Mệnh đề 9, V, p. 89.

#### Định lý 5 {#alg-v-s11-thm-5 .statement}

*a) Ánh xạ $A \mapsto K(\mathcal{P}^{-1}(A))$ là một song ánh từ tập hợp các nhóm con của $K$ chứa $\mathcal{P}(K)$ lên tập hợp các mở rộng con Abel của số mũ chia hết bởi $p$ trong $\Omega$. Ánh xạ nghịch đảo là $L \mapsto \mathcal{P}(L) \cap K$.
b) Với mọi nhóm con $A$ của $K$ chứa $\mathcal{P}(K)$, đồng cấu

$$
a' : \mathrm{Gal}(K(\mathcal{P}^{-1}(A))/K) \to \mathrm{Hom}(A/\mathcal{P}(K), \mathbf{F}_p)
$$

là song ánh, và nó là một đồng phôi khi $\mathrm{Hom}(A/\mathcal{P}(K), \mathbf{F}_p)$ được trang bị tôpô hội tụ đơn.
c) Cho $A$ là một nhóm con của $K$ chứa $\mathcal{P}(K)$ và cho $B$ là một cơ sở của không gian vectơ trên $\mathbf{F}_p$ là $A/\mathcal{P}(K)$. Với mỗi $a \in B$ hãy để $x_a$ là một phần tử của $\Omega$ sao cho $\mathcal{P}(x_a)$ là một đại diện của $a$ trong $A$. Khi đó các đơn thức $x^\alpha = \prod_{a \in B} x_a^{\alpha(a)}$ với a = (\alpha(a)) in N^{(B)} sao cho $0 \leq \alpha(a) < p$ với mỗi $a \in B$ tạo thành một cơ sở của không gian K-vectơ $K(\mathfrak{p}^{-1}(A))$. Đặc biệt ta có [K(\mathfrak{p}^{-1}(A)):K] = (A:\mathfrak{p}(K)).*

ĐLý 5 được chứng minh theo cùng cách như ĐLý 4 (V, p. 89), với những thay đổi thích hợp.

#### Ví dụ 1 {#alg-v-s11-n9-exa-1 .statement}

Tồn tại một mở rộng Abel lớn nhất của K có số mũ chia hết bởi p, được chứa trong \Omega; đó là K(B^1(K)), nhóm Galois của nó có thể được đồng nhất với Horn(K/\mathfrak{p}(K),\mathbf{F}_p).

#### Ví dụ 2 {#alg-v-s11-n9-exa-2 .statement}

Cho L là một mở rộng cyclic của K có bậc p; khi đó nhóm (\mathfrak{p}(L) \cap K)/\mathfrak{p}(K) là cyclic có cấp p. Nếu a \in K sao cho lớp thặng dư của a mod \mathfrak{p}(K) là một phần tử sinh của nhóm này, thì L là K-đẳng cấu với K[X]/(X^p - X - a) và nhóm Galois Gal(L/K) gồm p tự đẳng cấu gửi X thành X + i, i \in \mathbf{F}_p.

#### Ví dụ 3 {#alg-v-s11-n9-exa-3 .statement}

Ngược lại, nếu a \in K - \mathfrak{p}(K), thì đa thức X^p - X - a là bất khả quy và trường con L của \Omega được sinh bởi các nghiệm của nó là một mở rộng cyclic của K có bậc p. Nếu a \in \mathfrak{p}(K), thì X^p - X - a = \prod_{a \in \mathfrak{p}^{-1}(a)} (X - \alpha).

### Bài tập {#alg-v-s11-exercises}

Xem [các bài tập cho § 11](exercises/s11/).
