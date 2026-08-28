---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 4
section_title: Central filtrations
lang: vi
source: lie-i-iii
pdf_pages: 0160-0167, 0205-0211
extraction: ocr
subsections:
    - "no": 1
      title: REAL FILTRATIONS
      page: 0
      pdf_page: 160
    - "no": 2
      title: ORDER FUNCTION
      page: 0
      pdf_page: 161
    - "no": 3
      title: GRADED ALGEBRA ASSOCIATED WITH A FILTERED ALGEBRA
      page: 0
      pdf_page: 162
    - "no": 4
      title: CENTRAL FILTRATIONS ON A GROUP
      page: 0
      pdf_page: 163
    - "no": 5
      title: AN EXAMPLE OF A CENTRAL FILTRATION
      page: 0
      pdf_page: 165
    - "no": 6
      title: INTEGRAL CENTRAL FILTRATIONS
      page: 0
      pdf_page: 166
statements: 12
exercises: 18
content_sha256: 6a7b7f18f2b8d8580677a46069e377f8b9869cd34a6d48a99e5d111ae8472a87
translated_from: content/en/lie/II/04_s4_central_filtrations.md
source_content_sha256: 1325ad90b6f64f40c918361f53780fe37c172750b745daa70223fd8d6caff02f
translation_model: gpt-5-6, gpt-5-6-mini
translation_run: translate-vi-5f92d445
glossary_version: 34
glossary_terms_sha256: 1e5344a76f0a7048eeb380c5b092bff98ebff2877b34dd862601013d75483dea
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 4. LỌC TRUNG TÂM

### 1. CÁC LỌC THỰC

#### Định nghĩa 1 {#lie-ii-s4-def-1 .statement}

Cho $G$ là một nhóm. Một lọc thực trên $G$ là một họ $(G_\alpha)_{\alpha \in \mathbf{R}}$ của các nhóm con của $G$ sao cho
$$
G_\alpha = \bigcap_{\beta < \alpha} G_\beta \quad \text{với mọi } \alpha \in \mathbf{R}.
$$

Công thức (1) suy ra $G_\alpha \subset G_\beta$ với $\beta < \alpha$ và do đó họ $(G_\alpha)$ là *giảm*. Lọc $(G_\alpha)$ được gọi là *tách* nếu $\bigcap_\alpha G_\alpha$ thu gọn thành phần tử đơn vị và được gọi là *tràn* nếu $G = \bigcup_\alpha G_\alpha$.

#### Nhận xét {#lie-ii-s4-n1-rem-1 .statement}

Cho $(G_n)_{n \in \mathbf{Z}}$ là một dãy giảm các nhóm con của $G$. Nó là một lọc giảm theo nghĩa của *Đại số giao hoán*, Chương III, § 2, no. 1, Định nghĩa 1. Với mỗi số nguyên $n$ và mọi $\alpha$ trong khoảng $]n-1, n]$ của $\mathbf{R}$, ta viết $H_\alpha = G_n$, đặc biệt $H_n = G_n$. Hiển nhiên là bằng cách đó ta thu được một lọc thực $(H_\alpha)_{\alpha \in \mathbf{R}}$ trên $G$; một lọc như vậy sẽ được gọi là một *lọc nguyên*. Do đó các lọc giảm theo nghĩa của *Đại số giao hoán*, Chương III, § 2, có thể được đồng nhất với các lọc nguyên.

Cho $A$ là một đại số; một lọc thực $(A_\alpha)$ trên nhóm cộng của $A$ được gọi là tương thích với cấu trúc đại số nếu $A_\alpha . A_\beta \subset A_{\alpha + \beta}$ với $\alpha, \beta$ trong $\mathbf{R}$ và $K . A_\alpha \subset A_\alpha$ với $\alpha \in \mathbf{R}$. Nếu lọc là tràn, $(A_\alpha)$ là một hệ cơ bản các lân cận của 0 đối với tôpô trên $A$ tương thích với cấu trúc đại số. Cho $B$ là một đại số có đơn vị; một lọc thực $(B_\alpha)$ trên nhóm cộng của $B$ được gọi là tương thích với cấu trúc đại số có đơn vị nếu nó tương thích với cấu trúc đại số và $1 \in B_0$.

### 2. HÀM CẤP

Cho $G$ là một nhóm có phần tử đơn vị $e$. Cho $(G_\alpha)$ là một lọc thực trên $G$. Với mọi $x$ trong $G$, ký hiệu $I_x$ là tập hợp các số thực $\alpha$ sao cho $x \in G_\alpha$. Nếu $\alpha \in I_x$ và $\beta < \alpha$, thì $\beta \in I_x$ và do đó $I_x$ là một khoảng (*Tôpô tổng quát*, Chương IV, § 2, no. 4, Mệnh đề 1). Sử dụng quan hệ (1), ta thấy rằng $I_x$ chứa cận trên bé nhất của nó khi cận này là hữu hạn. Vì vậy $I_x$ có dạng $]-\infty, v(x)] \cap \mathbf{R}$ với $v(x) \in \overline{\mathbf{R}}$; ta có $v(x) = \sup \{ \alpha \mid x \in G_\alpha \}$.

Ánh xạ $v$ từ $G$ vào $\overline{\mathbf{R}}$ được gọi là *hàm cấp* liên kết với lọc thực $(G_\alpha)$ và $v(x)$ được gọi là *cấp* của $x$. Ánh xạ này có các tính chất sau đây:

(a) *Với $x \in G$ và $\alpha \in \mathbf{R}$, các quan hệ $x \in G_\alpha$ và $v(x) \geq \alpha$ là tương đương.*

(b) *Với $x, y$ trong $G$,*
$$
v(x^{-1}) = v(x), \qquad v(e) = +\infty.
$$
$$
v(xy) \geq \inf(v(x), v(y)).
$$

*Hơn nữa, ta có đẳng thức trong (3) nếu $v(x) > v(y)$.*

(c) *Với mọi $\alpha \in \mathbf{R}$, gọi $G_\alpha^+$ là tập hợp các $x \in G$ sao cho $v(x) > \alpha$. Khi đó $G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta$ và đặc biệt $G_\alpha^+$ là một nhóm con của $G$.*

Ngược lại, cho $v$ là một ánh xạ của $G$ vào $\overline{\mathbf{R}}$ thỏa mãn các quan hệ (2) và (3). Với mọi $\alpha \in \mathbf{R}$, gọi $G_\alpha$ là tập hợp các $x \in G$ sao cho $v(x) \geq \alpha$. Khi đó $(G_\alpha)_{\alpha \in \mathbf{R}}$ là một lọc thực của $G$ và $v$ là hàm cấp liên kết với lọc này.

Để lọc $(G_\alpha)$ là nguyên, điều kiện cần và đủ là $v$ ánh xạ $G$ vào $\mathbf{Z} \cup \{+\infty, -\infty\}$. Để nó là toàn phần (tương ứng, tách được), điều kiện cần và đủ là $-v^{-1}(-\infty) = \varnothing$ (tương ứng, $-v^{-1}(+\infty) = \{\epsilon\}$.

Cho $A$ là một đại số trên K (tương ứng, đại số trên K có đơn vị). Theo điều trên, quan hệ

$$
"x \in A_\alpha \Leftrightarrow v(x) \geq \alpha \quad \text{đối với } x \in A \text{ và } \alpha \in \mathbf{R}"
$$

xác định một song ánh từ tập hợp các lọc thực toàn phần $(A_\alpha)_{\alpha \in \mathbf{R}}$ tương thích với cấu trúc đại số (tương ứng, đại số có đơn vị) trên $A$ lên tập hợp các ánh xạ $v : A \to \overline{\mathbf{R}}$ không nhận giá trị $-\infty$ và thỏa mãn các tiên đề (4) đến (7) (tương ứng, (4) đến (8)) dưới đây:

(4) $$v(x + y) \geq \inf(v(x), v(y)) \quad (x, y \text{ trong } A)$$
(5) $$v(-x) = v(x) \qquad (x \in A)$$
(6) $$v(\lambda x) \geq v(x) \qquad (\lambda \in K, x \in A)$$
(7) $$v(xy) \geq v(x) + v(y) \qquad (x, y \text{ trong } A)$$
(8) $$v(1) \geq 0.$$

#### Nhận xét {#lie-ii-s4-n2-rem-1 .statement}

Nếu $v(x)$ không đồng nhất bằng $+\infty$, các điều kiện (7) và (8) kéo theo $v(1) = 0$.

### 3. ĐẠI SỐ PHÂN BẬC LIÊN KẾT VỚI MỘT ĐẠI SỐ CÓ LỌC

Cho $G$ là một nhóm *giao hoán* với một lọc thực $(G_\alpha)_{\alpha \in \mathbf{R}}$. Như trước đây ta viết

$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta;
$$

rõ ràng $G_\alpha^+$ là một nhóm con của $G_\alpha$. Ta viết $\operatorname{gr}_\alpha(G) = G_\alpha / G_\alpha^+$ và

$$
\operatorname{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \operatorname{gr}_\alpha(G).
$$

*Nhóm phân bậc liên kết với nhóm có lọc* $G$ là nhóm $\operatorname{gr}(G)$ với phép phân bậc tự nhiên kiểu $\mathbf{R}$.

#### Nhận xét {#lie-ii-s4-n3-rem-1 .statement}

Khi lọc $(G_\alpha)$ là nguyên, $\operatorname{gr}_\alpha(G) = \{0\}$ đối với $\alpha$ không nguyên và $\operatorname{gr}_n(G) = G_n / G_{n-1}$ đối với mọi số nguyên $n$. Định nghĩa của nhóm phân bậc liên kết do đó về cơ bản trùng với định nghĩa trong *Đại số giao hoán*, chương III, § 2, no. 3.

Cho $A$ là một đại số (tương ứng đại số có đơn vị) và $(A_\alpha)_{\alpha \in \mathbf{R}}$ là một lọc thực tương thích với cấu trúc đại số (tương ứng đại số có đơn vị) (no. 1). Khi đó

$$
A_\alpha \cdot A_\beta \subset A_{\alpha + \beta}, \qquad A_\alpha^+ \cdot A_\beta + A_\alpha \cdot A_\beta^+ \subset A_{\alpha + \beta}^+
$$

và ánh xạ song tuyến tính từ $A_\alpha \times A_\beta$ vào $A_{\alpha + \beta}$ là hạn chế của phép nhân trên $A$ xác định, khi lấy các thương, một ánh xạ song tuyến tính

$$
\operatorname{gr}_\alpha(A) \times \operatorname{gr}_\beta(A) \to \operatorname{gr}_{\alpha + \beta}(A).
$$

Ta suy ra một ánh xạ song tuyến tính từ gr(A) × gr(A) vào gr(A), làm cho nó trở thành một đại số phân bậc (tương ứng đại số phân bậc có đơn vị) kiểu $\mathbf{R}$. Nếu A là một đại số kết hợp (tương ứng giao hoán, tương ứng Lie), thì gr(A) cũng vậy.

### 4. CÁC LỌC TRUNG TÂM TRÊN MỘT NHÓM

#### Định nghĩa 2 {#lie-ii-s4-def-2 .statement}

Cho G là một nhóm. Một lọc thực $(G_\alpha)$ trên G được gọi là trung tâm nếu $G = \bigcup_{\alpha > 0} G_\alpha$ và giao hoán tử $(x, y) = x^{-1}y^{-1}xy$ của một phần tử x của $G_\alpha$ và một phần tử y của $G_\beta$ thuộc về $G_{\alpha + \beta}$.

Theo hàm cấp v, định nghĩa trên được chuyển thành các quan hệ
$$
v(x) > 0, \quad v((x, y)) \geq v(x) + v(y) \quad \text{for all } x, y \text{ in } G.
$$
Ta suy ra rằng $v((x, y)) > v(x)$ nếu $v(x) \neq +\infty$; nếu ta viết $x^y = y^{-1}xy$ (xem Đại số, chương I, § 6, no. 2), thì $x^y = x.(x, y)$, do đó
$$
v(x^y) = v(x).
$$
Quan hệ này biểu thị sự kiện rằng mỗi nhóm con $G_\alpha$ của G là chuẩn. Các $G_\alpha$ tạo thành một hệ cơ bản các lân cận của e đối với một tôpô tương thích với cấu trúc nhóm trên G (Tôpô đại cương, chương III, § 1, no. 2, Ví dụ), được gọi là xác định bởi lọc $(G_\alpha)$.

Trong phần còn lại của số này, G ký hiệu một nhóm với một lọc trung tâm $(G_\alpha)$. Với mọi $\alpha \in \mathbf{R}$, ta định nghĩa nhóm con $G_\alpha^+$ của G bởi
$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta.
$$
Đặc biệt $G_\alpha^+ = G_\alpha = G$ đối với $\alpha \leq 0$. Nhắc lại rằng nếu A và B là hai nhóm con của G, (A, B) ký hiệu nhóm con của G sinh bởi các giao hoán tử $(a, b)$ với $a \in A$ và $b \in B$. Với ký hiệu này ta có các công thức
$$
(G_\alpha, G_\beta) \subset G_{\alpha + \beta}
$$
$$
(G_\alpha^+, G_\beta^+) \subset G_{\alpha + \beta}^+
$$
$$
(G, G_\alpha) \subset G_\alpha^+.
$$
Theo (14), $G_\alpha^+$ là một nhóm con chuẩn của $G_\alpha$ đối với mọi $\alpha \in \mathbf{R}$ và nhóm thương $\mathrm{gr}_\alpha(G) = G_\alpha / G_\alpha^+$ là giao hoán. Ta viết $\mathrm{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \mathrm{gr}_\alpha(G)$ và trang bị cho nhóm này phép phân bậc kiểu $\mathbf{R}$ trong đó $\mathrm{gr}_\alpha(G)$ gồm các phần tử có bậc $\alpha$. Khi đó $\mathrm{gr}_\alpha(G) = \{0\}$ đối với $\alpha \leq 0$.

#### Mệnh đề 1 {#lie-ii-s4-prop-1 .statement}

(i) Cho $\alpha, \beta$ thuộc $\mathbf{R}$. Tồn tại một ánh xạ song cộng
$$
\phi_{\alpha \beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha + \beta}(G)
$$

ánh xạ $(xG_\alpha^+, yG_\beta^+)$ lên $(x, y)G_{\alpha+\beta}^+$.

(ii) Cho $\phi$ là ánh xạ song cộng của $\mathrm{gr}(G) \times \mathrm{gr}(G)$ vào $\mathrm{gr}(G)$ mà hạn chế của nó lên $\mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G)$ là $\phi_{\alpha\beta}$ đối với mọi cặp có thứ tự $(\alpha, \beta)$. Ánh xạ $\phi$ trang bị cho $\mathrm{gr}(G)$ một cấu trúc đại số Lie trên $\mathbf{Z}$.

(i) Nhắc lại đẳng thức

$$(xx', y) = (x, y)x'(x', y)$$

với $x, x', y$ trong $G$ (*Đại số*, Chương I, § 6, no. 2, công thức (4 bis)).

Với $x \in G_\alpha$ và $y \in G_\beta$, lớp modulo $G_{\alpha+\beta}^+$ của phần tử $(x, y)$ của $G_{\alpha+\beta}$ sẽ được ký hiệu là $f(x, y)$. Với $a$ trong $G_{\alpha+\beta}$ và $x'$ trong $G$, $a^{-1}.ax' = (a, x') \in G_{\alpha+\beta}^+$; đặc biệt $f(x, y)$ bằng lớp modulo $G_{\alpha+\beta}^+$ của $(x, y)x'$. Do đó công thức (15) suy ra

$$f(xx', y) = f(x, y)f(x', y).$$

Bây giờ $(y, x) = (x, y)^{-1}$, do đó

$$f(y, x) = f(x, y)^{-1}.$$

Từ (16) và (17) ta suy ra

$$f(x, yy') = f(x, y)f(x, y').$$

Ta phải chứng minh rằng ánh xạ $f : G_\alpha \times G_\beta \to \mathrm{gr}_{\alpha+\beta}(G)$ xác định khi lấy các thương một ánh xạ $\phi_{\alpha\beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha+\beta}(G)$. Theo (16) và (18), chỉ cần chứng minh rằng $f(x, y) = 0$ nếu $x \in G_\alpha^+$ hoặc $y \in G_\beta^+$, điều này suy ra từ (13').

(ii) Vì $(x, x) = e$, từ (17) suy ra rằng $\phi$ là một ánh xạ song tuyến tính phản xứng trên $\mathbf{Z}$. Do đó còn phải chứng minh rằng, với $u \in \mathrm{gr}_\alpha(G)$, $v \in \mathrm{gr}_\beta(G)$ và $w \in \mathrm{gr}_\gamma(G)$,

$$\phi(u, \phi(v, w)) + \phi(v, \phi(w, u)) + \phi(w, \phi(u, v)) = 0.$$

Cho $x \in G_\alpha, y \in G_\beta$ và $z \in G_\gamma$ là các phần tử lần lượt đại diện cho $u, v$ và $w$. Ta biết rằng $x^y$ và $x$ là hai phần tử của $G_\alpha$ đồng dư theo môđun $G_\alpha^+$ và do đó $x^y$ là một đại diện của $u$ trong $G_\alpha$; vì $(y, z)$ là một đại diện của $\phi(v, w)$ trong $G_{\beta+\gamma}$, ta thấy rằng $(x^y, (y, z))$ là một đại diện của $\phi(u, \phi(v, w))$ trong $G_{\alpha+\beta+\gamma}$. Bằng phép hoán vị vòng, ta thấy rằng $(y^z, (z, x))$ và $(z^x, (x, y))$ lần lượt đại diện cho $\phi(v, \phi(w, u))$ và $\phi(w, \phi(u, v))$ trong $G_{\alpha+\beta+\gamma}$. Quan hệ (19) khi đó là một hệ quả của đẳng thức sau (*Đại số*, Chương I, § 6, no. 2, công thức (15)):

$$(x^y, (y, z)).(y^z, (z, x)).(z^x, (x, y)) = e.$$

Đại số Lie $\mathrm{gr}(G)$ trên $\mathbf{Z}$ được định nghĩa trong Mệnh đề 1 được gọi là *đại số Lie phân bậc liên kết với nhóm lọc* $G$.

### 5. MỘT VÍ DỤ VỀ MỘT LỌC TRUNG TÂM

Cho $A$ là một đại số kết hợp có đơn vị với một lọc đại số có đơn vị $(A_\alpha)$ sao cho $A_0 = A$; khi đó $A_\alpha$ là một iđêan hai phía của $A$ với mọi $\alpha \in \mathbf{R}$. Gọi $A^*$ là nhóm nhân của các phần tử khả nghịch của $A$. Với mọi $\alpha > 0$, gọi $\Gamma_\alpha$ là tập hợp các $x \in A^*$ sao cho $x - 1 \in A_\alpha$; ta viết $\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$ và $\Gamma_\beta = \Gamma$ với $\beta \leq 0$.

#### Mệnh đề 2 {#lie-ii-s4-prop-2 .statement}

*Tập hợp $\Gamma$ là một nhóm con của $A^*$ và $(\Gamma_\alpha)$ là một lọc trung tâm trên $\Gamma$.*

$\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$ theo phép dựng và quan hệ $\Gamma_\alpha = \bigcap_{\beta < \alpha} \Gamma_\beta$ suy ra từ $A_\alpha = \bigcap_{\beta < \alpha} A_\beta$.

Ta chứng minh rằng $\Gamma_\alpha$ là một nhóm con của $A^*$. Hiện tại $1 \in \Gamma_\alpha$; lấy $x, y$ thuộc $\Gamma_\alpha$, do đó $x - 1 \in A_\alpha, y - 1 \in A_\alpha$. Vì $A_\alpha$ là một iđêan hai phía của $A$, các công thức
$$
(21) \quad xy - 1 = (x - 1)(y - 1) + (x - 1) + (y - 1),
$$
$$
(22) \quad x^{-1} - 1 = -x^{-1}(x - 1),
$$
suy ra $xy - 1 \in A_\alpha$ và $x^{-1} - 1 \in A_\alpha$, do đó $xy \in \Gamma_\alpha$ và $x^{-1} \in \Gamma_\alpha$.

Vì $\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$, đây là một nhóm con của $A^*$.

Cuối cùng lấy $\alpha > 0, \beta > 0, x \in \Gamma_\alpha$ và $y \in \Gamma_\beta$. Đặt $x - 1 = \xi$ và $y - 1 = \eta$. Khi đó
$$
(23) \quad (x, y) - 1 = x^{-1}y^{-1}(\xi \eta - \eta \xi);
$$
theo giả thiết, $\xi \in A_\alpha$ và $\eta \in A_\beta$, do đó $\xi \eta - \eta \xi \in A_{\alpha + \beta}$. Vì $A_{\alpha + \beta}$ là một iđêan hai phía của $A$, $(x, y) - 1 \in A_{\alpha + \beta}$, do đó $(x, y) \in \Gamma_{\alpha + \beta}$.

#### Nhận xét {#lie-ii-s4-n5-rem-1 .statement}

Cho $\alpha \geq 0, \beta \geq 0$ và $x \in \Gamma_\alpha, y \in \Gamma_\beta$. Theo các công thức (21), (22) và (23),
$$
(24) \quad x^{-1} - 1 \equiv -(x - 1) \pmod{A_{2\alpha}}
$$
$$
(25) \quad xy - 1 \equiv (x - 1) + (y - 1) \pmod{A_{\alpha + \beta}}
$$
$$
(26) \quad (x, y) - 1 \equiv [(x - 1), (y - 1)] \pmod{A_{\alpha + \beta + \inf(\alpha, \beta)}}.
$$

Ta chứng minh chẳng hạn (26). Nếu $x - 1 = \xi$ và $y - 1 = \eta$, (23) cho:
$$
(x, y) - 1 - [\xi, \eta] = ((x^{-1} - 1) + (y^{-1} - 1) + (x^{-1} - 1)(y^{-1} - 1))[\xi, \eta].
$$
Bây giờ $[\xi, \eta] \in A_{\alpha + \beta}$, $(x^{-1} - 1) \in A_\alpha$, $(y^{-1} - 1) \in A_\beta$, do đó ta thu được (26).

Cho $G$ là một nhóm và $\rho : G \to \Gamma$ là một đồng cấu. Với mọi $\alpha$ thực, ta viết $G_\alpha = \rho^{-1}(\Gamma_\alpha)$. Vì $(\Gamma_\alpha)$ là một lọc trung tâm trên $\Gamma$, hiển nhiên rằng $(G_\alpha)$ là một lọc trung tâm trên $G$.

#### Mệnh đề 3 {#lie-ii-s4-prop-3 .statement}

(i) *Với mọi $\alpha \in \mathbf{R}$, tồn tại một đồng cấu nhóm duy nhất $g_\alpha : \mathrm{gr}_\alpha(G) \to \mathrm{gr}_\alpha(A)$ biến lớp modulo $G_\alpha^+$ của một phần tử $a \in G_\alpha$ thành lớp modulo $A_\alpha^+$ của $\rho(a) - 1$.*

(ii) Cho g là đồng cấu nhóm của gr(G) vào gr(A) mà hạn chế của nó trên gr_\alpha(G) là g_\alpha với mọi \alpha. Ánh xạ g là một đơn cấu đồng cấu của các đại số Lie $\mathbf{Z}$.

(i) Cho \alpha > 0. Theo giả thiết, với mọi $a$ trong $G_\alpha$, $\rho(a) - 1 \in A_\alpha$; ký hiệu $p_\alpha(a)$ là lớp của $\rho(a) - 1$ modulo $A_\alpha^+$. Vì $A_{2\alpha} \subset A_\alpha^+$, quan hệ (25) suy ra $p_\alpha(ab) = p_\alpha(a) + p_\alpha(b)$. Khi đó $a \in G_\alpha^+$ khi và chỉ khi $\rho(a) - 1 \in A_\alpha^+$; do đó $G_\alpha^+$ là hạt nhân của đồng cấu $p_\alpha$ của $G_\alpha$ vào gr_\alpha(A). Chuyển qua thương, $p_\alpha$ xác định một đơn cấu đồng cấu $g_\alpha$ của gr_\alpha(G) vào gr_\alpha(A).

Với $\alpha \leq 0$, gr_\alpha(G) = $\{0\}$ và lựa chọn duy nhất là $g_\alpha = 0$.

(ii) Vì $g_\alpha$ là đơn ánh với mọi $\alpha$ thực, g là đơn ánh. Ta chứng minh rằng g là một đồng cấu đại số Lie. Vì gr_\alpha(G) = $\{0\}$ với $\alpha \leq 0$, chỉ cần thiết lập công thức

$$
p_{\alpha+\beta}((a, b)) = [p_\alpha(a), p_\beta(b)]
$$

với $\alpha > 0$, $\beta > 0$, $\rightarrow \in G_\alpha$ và $b \in G_\beta$, điều này suy ra từ (26).

### 6. CÁC LỌC TRUNG TÂM NGUYÊN

Nhắc lại (no. 1, Nhận xét) rằng một lọc $(G_\alpha)$ trên nhóm G được gọi là nguyên nếu $G_\alpha = G_n$ với mọi số nguyên n và mọi $\alpha \in \{n-1, n\}$. Cho một lọc trung tâm nguyên trên một nhóm G tương đương với việc cho một dãy $(G_n)_{n \geq 1}$ các nhóm con của G thỏa mãn các điều kiện

(i) \quad G_1 = G
(ii) \quad G_n \supset G_{n+1} \quad \text{với mọi } n \geq 1
(iii) \quad (G_m, G_n) \subset G_{m+n} \quad \text{với } m \geq 1 \text{ và } n \geq 1.

Với mỗi số nguyên n $\geq 1$, $G_n$ là một nhóm con chuẩn của G và thương gr_n(G) = $G_n/G_{n+1}$ là giao hoán. Khi lấy các thương, ánh xạ $(x, y) \mapsto (x, y) = x^{-1}y^{-1}xy$ của $G_m \times G_n$ vào $G_{m+n}$ cho phép ta định nghĩa trên gr(G) = $\bigoplus_{n \geq 1} gr_n(G)$ một cấu trúc đại số Lie phân bậc kiểu $\mathbf{N}$ trên vành $\mathbf{Z}$.

Nhắc lại (Đại số, Chương I, § 6, no. 3, Định nghĩa 5) rằng chuỗi trung tâm dưới của nhóm G được định nghĩa bởi

$$
C^1G = G, \quad C^{n+1} = (G, C^nG) \quad \text{với } n \geq 1.
$$

Lọc tương ứng được gọi là lọc trung tâm dưới của G.

#### Mệnh đề 4 {#lie-ii-s4-prop-4 .statement}

(i) Chuỗi trung tâm dưới của G là một lọc trung tâm nguyên trên G.

(ii) Nếu $(G_n)_{n \in \mathbf{N}^*}$ là một lọc trung tâm nguyên trên G, thì $C^nG \subset G_n$ với mọi $n \in \mathbf{N}^*$.

Mệnh đề (i) đã được chứng minh trong Đại số, Chương I, § 6, no. 3, công thức (7).

Ta chứng minh (ii) bằng quy nạp theo n; $C^1G = G = G_1$; với n > 1,

$$
C^nG = (G, C^{n-1}G) \subset (G, G_{n-1}) \subset G_n.
$$

#### Mệnh đề 5 {#lie-ii-s4-prop-5 .statement}

Cho G là một nhóm và gr(G) là đại số Lie phân bậc $\mathbf{Z}$ liên kết với lọc trung tâm dưới trên G. Khi đó gr(G) được sinh bởi $\mathrm{gr}_1(G) = G/(G, G)$.

Cho L là đại số con Lie của gr(G) sinh bởi $\mathrm{gr}_1(G)$; ta chứng minh rằng $L \supset \mathrm{gr}_n(G)$ bằng quy nạp theo n, mệnh đề này là tầm thường đối với $n = 1$. Giả sử rằng $n > 1$ và $L \supset \mathrm{gr}_{n-1}(G)$. Vì $C^nG = (G, C^{n-1}G)$, phép dựng luật đại số Lie trên gr(G) cho thấy ngay lập tức rằng

$$
\mathrm{gr}_n(G) = [\mathrm{gr}_1(G), \mathrm{gr}_{n-1}(G)] \subset L.
$$

Chứng minh trên cho thấy chuỗi trung tâm dưới của đại số Lie gr(G) (§ 2, no. 7) được cho bởi

$$
\mathcal{C}^n(\mathrm{gr}(G)) = \sum_{m \geq n} \mathrm{gr}_m(G).
$$

#### Nhận xét {#lie-ii-s4-n6-rem-1 .statement}

Cho k là một vành, n là một số nguyên $> 0$ và A là tập hợp các ma trận tam giác dưới với n hàng và n cột và các phần tử trong k. Với $p \geq 0$, cho $A_p$ là tập hợp các $(x_{ij}) \in A$ sao cho $x_{ij} = 0$ đối với $i - j < p$. Khi đó $A_0 = A$ và $A_pA_q \subset A_{p+q}$. Cho $\Gamma_p = 1 + A_p$. Khi đó $\Gamma_1$ là một nhóm con của $\mathbf{GL}(n, k)$ được gọi là nhóm tam giác dưới ngặt cấp n trên k. Theo Mệnh đề 2 của no. 5, $(\Gamma_p)$ là một lọc nguyên trên $\Gamma_1$. Vì $\Gamma_n = \{1\}$, ta thấy rằng nhóm $\Gamma_1$ là lũy linh (Đại số, Chương I, § 6, no. 3, Định nghĩa 6).

### Bài tập {#lie-ii-s4-exercises}

Trong các bài tập sau, chữ G ký hiệu một nhóm.

Xem các [bài tập cho § 4](exercises/s4/).
